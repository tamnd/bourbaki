---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 8
section_title: Produits de mesures
lang: fr
source: int-v-fr
pdf_pages: 0091-0107, 0131-0140
extraction: ocr
subsections:
    - "no": 1
      title: Interprétation de la mesure produit comme intégrale de mesures
      page: 0
      pdf_page: 91
    - "no": 2
      title: Fonctions mesurables par rapport à un produit de deux mesures
      page: 0
      pdf_page: 94
    - "no": 3
      title: Intégration de fonctions positives
      page: 0
      pdf_page: 96
    - "no": 4
      title: Intégration de fonctions à valeurs dans un espace de Banach
      page: 0
      pdf_page: 101
    - "no": 5
      title: Opérations sur le produit de deux mesures
      page: 0
      pdf_page: 103
    - "no": 6
      title: Intégration par rapport à un produit fini de mesures
      page: 0
      pdf_page: 105
    - "no": 7
      title: 'Application: Mesure de la boule euclidienne dans $\mathbf{R}^n$'
      page: 0
      pdf_page: 106
statements: 32
exercises: 21
content_sha256: 48b6392485704cebfa0776ee98533615adc0992ae238bb84b98cd9fab5b7fe0b
---

## § 8. — Produits de mesures

### 1. Interprétation de la mesure produit comme intégrale de mesures

Dans tout ce paragraphe on note $T, T'$ deux espaces localement compacts, $\mu$ une mesure positive sur $T$, $\mu'$ une mesure positive sur $T'$, $v = \mu \otimes \mu'$ la mesure produit sur $X = T \times T'$ (chap. III, 2e éd., § 4, n° 1).

Pour tout $t \in T$, l’application $t' \mapsto (t, t')$ de $T'$ dans $X$ est continue et propre. Soit $\lambda'_t$ l’image de $\mu'$ par cette application; $\lambda'_t$ est une mesure positive sur $X$, et si $f \in \mathscr{K}(X)$, on a, en désignant par $f_t$ l’application partielle $t' \mapsto f(t, t')$
$$
\int f d\lambda'_t = \int f_t d\mu'
$$
ce qui s’exprime encore par la relation $\lambda'_t = \varepsilon_t \otimes \mu'$.

$$
\int \langle f, \lambda_t' \rangle d\mu(t) = \int d\mu(t) \int f_t(t') d\mu'(t') = \int f(t, t') dv(t, t')
$$

(chap. III, 2e éd., § 4, n° 1, th. 2); on a donc $v = \int \lambda_t' d\mu(t)$.

De même, pour tout élément $t' \in T'$, soit $\lambda_{t'}$ l’image de $\mu$ par l’application $t \mapsto (t, t')$ de T dans X. L’application $t' \mapsto \lambda_{t'}$ est $\mu'$-adéquate et vaguement continue, et on a $v = \int \lambda_{t'} d\mu'(t')$. Nous aurons besoin des lemmes suivants:

#### Lemme 1 {#int-v-s8-lem-1 .statement}

*Pour toute fonction numérique $f \geq 0$ définie dans X on a*

$$
\int^* f_t d\mu' = \int^* f d\lambda_t'.
$$

Comme $t' \mapsto (t, t')$ est une application continue et propre, cela résulte de la prop. 2 du § 4, n° 2.

#### Lemme 2 {#int-v-s8-lem-2 .statement}

*Soit $f$ une application de X dans un espace topologique. Pour que $f$ soit $\lambda_t'$-mesurable, il faut et il suffit que $f_t$ soit $\mu'$-mesurable.*

C’est une conséquence de la prop. 3 du § 6, n° 2.

#### Lemme 3 {#int-v-s8-lem-3 .statement}

*Soit $\mathbf{f}$ une fonction définie dans X, à valeurs dans $\bar{\mathbf{R}}$ ou dans un espace de Banach. Pour que $\mathbf{f}$ soit $\lambda_t'$-intégrable, il faut et il suffit que $\mathbf{f}_t$ soit $\mu'$-intégrable, et on a alors*

$$
\int \mathbf{f}_t d\mu' = \int \mathbf{f} d\lambda_t'.
$$

Cela résulte du th. 2 du § 4, n° 4, compte tenu de ce que $t' \mapsto (t, t')$ est continue et propre.

#### Remarque {#int-v-s8-n1-rem-1 .statement}

On peut démontrer fort simplement les lemmes 1, 2, 3 sans faire usage des résultats des §§ 4 et 6, par un raisonnement direct. Par exemple, la relation (2) est évidente par définition si $f \in \mathscr{H}(T \times T')$. Si $f$ est semi-continue inférieurement dans $X = T \times T'$, il suffit de remarquer que $t' \mapsto f_t(t')$ est l’enveloppe supérieure des fonctions $t' \mapsto g_t(t') = g(t, t')$, où $g$ parcourt l’ensemble des fonctions de $\mathscr{K}(X)$ telles que $0 \leq g \leq f$. Enfin, pour $f$ quelconque, on notera que si $h \geq f$ est semi-continue inférieurement dans $X$, $t' \mapsto h(t, t')$ est semi-continue inférieurement dans $T'$; et réciproquement, si $t' \mapsto u(t')$ est semi-continue inférieurement dans $T'$ et telle que $u(t') \geq f(t, t')$ pour tout $t' \in T'$, la fonction $h$ telle que $h(t, t') = u(t'), h(t_1, t') = +\infty$ pour $t_1 \neq t$, est semi-continue inférieurement dans $X$ et telle que $h \geq f$. Une fois le lemme 1 démontré, on en déduit que l’ensemble $(T - \{t\}) \times T'$ est $\lambda'_t$-négligeable, et il est alors très facile de démontrer les lemmes 2 et 3.

La relation (3) permet de noter les deux membres $\int \mathbf{f}(t, t')\ d\mu'(t')$ sans risque de confusion. On a évidemment des résultats analogues pour les mesures $\lambda_{t'} = \mu \otimes \varepsilon_{t'}$.

A la place des notations $\int^* f(t, t')\ dv(t, t')$, $\int^* f(t, t')\ dv(t, t')$, $\int \mathbf{f}(t, t')\ dv(t, t')$ nous utiliserons les notations $\iint^* f(t, t')\ d\mu(t)\ d\mu'(t')$, $\iint^* f(t, t')\ d\mu(t)\ d\mu'(t')$, $\iint \mathbf{f}(t, t')\ d\mu(t)\ d\mu'(t')$, en accord avec les notations adoptées au chap. III, 2e éd., § 4, n° 1.

L’interprétation de la mesure $v$ comme une intégrale $\int \lambda'_t\ d\mu(t)$ va nous permettre de traduire dans le langage des mesures produit les résultats du § 3. D’autre part, la mesure $\lambda'_t$ est portée par $\{t\} \times T' = \overline{\mathrm{pr}}_1^{-1}(t)$, de sorte que cette intégrale définit une décomposition en tranches de $v$, relativement à la projection $\mathrm{pr}_1$ de $T \times T'$ sur $T$ (§ 6, n° 6). Avant de donner une liste des résultats que l’on obtient ainsi, voici une propriété utile:

#### Proposition 1 {#int-v-s8-prop-1 .statement}

Soit $(\mu_\alpha)_{\alpha \in A}$ (resp. $(\mu'_\beta)_{\beta \in B}$) une famille sommable de mesures positives sur $T$ (resp. sur $T'$) dont on désigne la somme par $\mu$ (resp. par $\mu'$). La famille $(\mu_\alpha \otimes \mu'_\beta)_{(\alpha, \beta) \in A \times B}$ est alors sommable sur $T \times T'$, et on a
$$
\mu \otimes \mu' = \sum_{(\alpha, \beta) \in A \times B} \mu_\alpha \otimes \mu'_\beta.
$$
(4)

Ces propriétés sont évidentes lorsque $A$ et $B$ sont finis. Il en résulte qu’on a, si $A'$ (resp. $B'$) est une partie finie de $A$ (resp. de $B$),
$$
\sum_{(\alpha, \beta) \in A' \times B'} \mu_\alpha \otimes \mu'_\beta \leq \mu \otimes \mu'.
$$
La famille $(\mu_\alpha \otimes \mu'_\beta)$ est donc sommable. Pour montrer que les deux membres de (4) sont égaux, il suffit de prouver que le second membre satisfait à la propriété caractéristique des mesures

Soient $f$ un élément de $\mathcal{K}_+(T)$, $f'$ un élément de $\mathcal{K}_+(T')$; rappelons qu’on note $f \otimes f'$ la fonction $(t, t') \mapsto f(t)f'(t')$ sur $T \times T'$, qui appartient à $\mathcal{K}_+(T \times T')$ (Alg., chap. II, 3e éd., § 7, n° 7). On a alors d’après la définition des produits de mesures :

$$
\sum_{(\alpha, \beta) \in \mathbf{A} \times \mathbf{B}} \langle \mu_\alpha \otimes \mu'_\beta, f \otimes f' \rangle = \sum_{(\alpha, \beta) \in \mathbf{A} \times \mathbf{B}} (\langle \mu_\alpha, f \rangle \langle \mu'_\beta, f' \rangle)
= \left( \sum_{\alpha \in \mathbf{A}} \langle \mu_\alpha, f \rangle \right) \left( \sum_{\beta \in \mathbf{B}} \langle \mu'_\beta, f' \rangle \right)
= \langle \mu, f \rangle \langle \mu', f' \rangle
= \langle \mu \otimes \mu', f \otimes f' \rangle.
$$

### 2. Fonctions mesurables par rapport à un produit de deux mesures

#### Proposition 2 {#int-v-s8-prop-2 .statement}

Soit $f$ une fonction $v$-mesurable définie dans $T \times T'$, à valeurs dans un espace topologique $G$, et soit $M$ l’ensemble des $t \in T$ tels que l’application $t' \mapsto f(t, t')$ ne soit pas $\mu'$-mesurable.

a) Si $f$ est constante dans le complémentaire d’une partie $v$-modérée de $T \times T'$, $M$ est $\mu$-négligeable.

b) Si $\mu'$ est modérée, $M$ est localement $\mu$-négligeable.

L’assertion a) découle de la prop. 4b) du § 3, n° 2 et des remarques du n° 1. Pour traiter b), remarquons que $\mu'$ est somme d’une suite $\mu'_n$ de mesures bornées (\$ 2, n° 3, prop. 4); $f$ est mesurable par rapport à $\mu \otimes \mu'_n \leq v$, et l’ensemble $M$ est réunion des ensembles $M_n$ associés aux mesures $\mu'_n$ (\$ 2, n° 2, prop. 2). On est donc ramené au cas où $\mu'$ est bornée, qui résulte de la prop. 4 c) du § 3, n° 2.

Cet énoncé s’étend immédiatement aux mesures complexes (chap. III, 2e éd., § 4, n° 2, prop. 3).

#### Corollaire {#int-v-s8-n2-cor-1 .statement}

Soit $A$ une partie $v$-mesurable de $T \times T'$, et soit $M$ l’ensemble des $t \in T$ tels que la coupe $A(t)$ de $A$ suivant $t$ ne soit pas $\mu'$-mesurable.

a) Si $A$ est $v$-modéré, $M$ est $\mu$-négligeable.

b) Si la projection de $A$ sur $T'$ est $\mu$-modérée, $M$ est localement $\mu$-négligeable.

L’assertion a) découle immédiatement de la prop. 2. Pour établir b), désignons par $B$ un ensemble, réunion d’une suite d’ouverts $\mu'$-intégrables de $T'$, qui contient la projection de $A$ sur T', et désignons par $\mu'_1$ la mesure modérée $\varphi_B \cdot \mu'$; A étant mesurable par rapport à $\mu \otimes \mu'_1 \leq \mu \otimes \mu'$, la prop. 2 entraîne que $A(t)$ est $\mu'_1$-mesurable, sauf pour des $t$ qui forment un ensemble localement $\mu$-négligeable. Mais comme $A(t) \subset B$, dire que $A(t)$ est $\mu'_1$-mesurable équivaut à dire que $A(t)$ est $\mu'$-mesurable ($\S 5$, n° 3, prop. 4).

#### Proposition 3 {#int-v-s8-prop-3 .statement}

*Soit f une application de T dans un espace topologique F. Si f est $\mu$-mesurable, l’application $(t, t') \mapsto f(t)$ est $\nu$-mesurable. Inversement, si $\mu' \neq 0$, et si cette application est $\nu$-mesurable, la fonction f est $\mu$-mesurable.*

La première assertion résulte du cor. 1 de la prop. 10 du $\S 6$, n° 6. Supposons qu’on ait $\mu' \neq 0$, désignons par $\mu'_1$ une mesure à support compact non nulle majorée par $\mu'$, par $\nu_1$ la mesure $\mu \otimes \mu'_1$, et posons $a = \| \mu'_1 \|$. La projection $pr_1$ de $T \times T'$ sur $T$ est alors $\nu_1$-propre, et la mesure image $pr_1(\nu_1)$ est égale à $a \mu$ ($\S 6$, n° 6, prop. 10). Si $(t, t') \mapsto f(t)$ est $\nu$-mesurable, elle est aussi $\nu_1$-mesurable, donc $f$ est mesurable par rapport à la mesure $a \mu$ ($\S 6$, n° 2, prop. 3), d’où le résultat puisque $a \neq 0$.

L’énoncé précédent s’étend immédiatement aux mesures complexes (chap. III, $\S 4$, n° 2, prop. 3), ainsi que les corollaires ci-dessous.

#### Corollaire 1 {#int-v-s8-prop-3-cor-1 .statement}

*Soient F, F' et G trois espaces topologiques, et soit u une application continue de $F \times F'$ dans G. Soit f (resp. $f'$) une fonction définie dans T (resp. T') à valeurs dans F (resp. F') et mesurable pour $\mu$ (resp. $\mu'$). Alors la fonction $(t, t') \mapsto u(f(t), f'(t'))$ est mesurable pour $\mu \otimes \mu'$.

Les applications $(t, t') \mapsto f(t), (t, t') \mapsto f'(t')$ étant $\nu$-mesurables d’après la prop. 3, cela résulte du th. 1 du chap. IV, $\S 5$, n° 3.

#### Corollaire 2 {#int-v-s8-prop-3-cor-2 .statement}

*Si $A \subset T$ et $A' \subset T'$ sont mesurables (pour $\mu$ et $\mu'$ respectivement), $A \times A'$ est mesurable pour $\mu \otimes \mu'$.

Cela résulte aussitôt du cor. 1.

#### Corollaire 3 {#int-v-s8-prop-3-cor-3 .statement}

*Considérons deux fonctions numériques positives (resp. à valeurs complexes), f définie dans T, $f'$ définie dans T'. Si ces fonctions sont mesurables pour $\mu$ et $\mu'$ respectivement, la fonction $f \otimes f' : (t; t') \mapsto f(t)f'(t')$ est mesurable pour $\mu \otimes \mu'$.*

Le cas des fonctions complexes, ou des fonctions réelles finies, est une conséquence immédiate du cor. 1. Pour traiter le cas des fonctions numériques positives, on pose pour tout entier $n \geq 0,\ f_n = \inf(f, n),\ f'_n = \inf(f', n)$ et on a (avec la convention habituelle $0 . (+\infty) = 0$) $f \otimes f' = \sup_n (f_n \otimes f'_n)$, d’où le résultat.

#### Proposition 4 {#int-v-s8-prop-4 .statement}

*Soit A une partie de T. Si A est localement $\mu$-négligeable, $A \times T'$ est localement $v$-négligeable. Inversement, si $A \times T'$ est localement $v$-négligeable, et si $\mu' \neq 0$, A est localement $\mu$-négligeable.*

La première assertion résulte du cor. 1 de la prop. 10 du § 6, n° 6. Pour établir la seconde assertion, reprenons les notations de la démonstration de la prop. 3; $A \times T' = \overline{\mathrm{pr}}_1(A)$ est localement négligeable pour la mesure $v_1$, donc A est localement négligeable pour $a\mu$ ($\S 6$, n° 2, cor. 2 de la prop. 2), d’où le résultat puisque $a \neq 0$.

L’énoncé précédent s’étend aussitôt au produit de deux mesures complexes (chap. III, 2e éd., § 4, n° 2, prop. 3), ainsi que le corollaire ci-dessous.

#### Corollaire {#int-v-s8-n2-cor-2 .statement}

*Si la mesure $\mu$ (resp. $\mu'$) est concentrée sur M (resp. $M'$), $\mu \otimes \mu'$ est concentrée sur $M \times M'$.

En effet, $(T \times T') - (M \times M')$ est réunion de $(T - M) \times T'$ et de $T \times (T' - M')$ qui sont localement négligeables pour $\mu \otimes \mu'$ en vertu de la prop. 4.*

### 3. Intégration de fonctions positives

Rappelons que nous avons convenu de définir le produit $0 . (+\infty)$ comme égal à 0. Cette convention a en particulier la conséquence suivante: si $f$ est une fonction numérique $\geq 0$ définie dans un espace localement compact muni d’une mesure positive $\lambda$, on a $\lambda^*(af) = a . \lambda^*(f)$ pour toute constante $a$ telle que $0 \leq a \leq +\infty$. C’est évident si $a = 0$; si $a = +\infty$, on a $\lambda^*(af) = a . \lambda^*(f) = 0$ ou $\lambda^*(af) = a . \lambda^*(f) = +\infty$ suivant que $f$ est ou n’est pas $\lambda$-négligeable; enfin, si $0 < a < +\infty$, on sait que $\lambda^*(af) = a . \lambda^*(f)$.

#### Proposition 5 {#int-v-s8-prop-5 .statement}

*Soit $f$ une fonction numérique $\geq 0$, semi-continue inférieurement dans $T \times T'$. Alors, la fonction*

$$
t \mapsto \int^* f(t, t')\ d\mu'(t')
$$

est semi-continue inférieurement dans T, et on a

(5) $\iint^* f(t, t')\ d\mu(t)\ d\mu'(t') = \int^* d\mu(t) \int^* f(t, t')\ d\mu'(t').$

C’est une conséquence de la prop. 2 du § 3, n° 1, compte tenu du lemme 1 du n° 1.

#### Corollaire 1 {#int-v-s8-prop-5-cor-1 .statement}

Soit $f$ (resp. $f'$) une fonction semi-continue inférieurement $\geqslant 0$ définie dans T (resp. dans T'); la fonction $f \otimes f': (t, t') \mapsto f(t)f'(t')$ est alors semi-continue inférieurement dans $T \times T'$, et on a

(6) $\iint^* f(t)f'(t')\ d\mu(t)\ d\mu'(t') = \left( \int^* f(t)\ d\mu(t) \right) \left( \int^* f'(t')\ d\mu'(t') \right).$

Soit G (resp. G') l’ensemble des fonctions $g \in \mathscr{K}_+(T)$ (resp. $g' \in \mathscr{K}_+(T')$) telles que $g \leqslant f$ (resp. $g' \leqslant f'$); on a

$$
f \otimes f' = \sup_{g \in G,\ g' \in G'} g \otimes g'.
$$

Les fonctions $g \otimes g'$ appartenant à $\mathscr{K}_+(T \times T')$, $f \otimes f'$ est bien semi-continue inférieurement, et (6) résulte aussitôt de la prop. 5 (ou directement d’un passage à la limite à partir de la formule précédente).

#### Corollaire 2 {#int-v-s8-prop-5-cor-2 .statement}

Soient A une partie $\mu$-modérée de T, A' une partie $\mu'$-modérée de T'; A $\times$ A' est alors $\nu$-modérée dans $T \times T'$.

Compte tenu de la définition des ensembles modérés (§ 1, n° 2, prop. 5), il suffit de montrer que si B est un ouvert intégrable de T, et B' un ouvert intégrable de T', l’ouvert B $\times$ B' est intégrable. Cela résulte aussitôt du cor. 1.

#### Corollaire 3 {#int-v-s8-prop-5-cor-3 .statement}

Soient A une partie $\mu$-négligeable de T, B' une partie $\mu'$-modérée de T'; A $\times$ B' est alors $\nu$-négligeable.

En effet, A $\times$ B' est localement $\nu$-négligeable (prop. 4) et $\nu$-modéré (cor. 2), donc $\nu$-négligeable (§ 1, n° 2, cor. 1 de la prop. 7).

Les cor. 2 et 3 s’étendent au produit de deux mesures complexes, en appliquant l’énoncé à leurs valeurs absolues (chap. III, 2e éd., § 4, prop. 3).

#### Proposition 6 {#int-v-s8-prop-6 .statement}

Soit $f$ une fonction numérique $\geqslant 0$ définie dans $T \times T'$. On a

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t') \geqslant \int^* d\mu(t) \int^* f(t, t') \, d\mu'(t').
$$

Cela résulte de la prop. 3 du § 3, n° 2, compte tenu de (2).

#### Proposition 7 {#int-v-s8-prop-7 .statement}

Soit $f$ une fonction numérique positive $v$-mesurable définie dans $T \times T'$.

a) Si $f$ est $v$-modérée, les fonctions $t \mapsto \int^* f(t, t') \, d\mu'(t')$, $t' \mapsto \int^* f(t, t') \, d\mu(t)$ sont mesurables respectivement pour $\mu$ et $\mu'$, et on a

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') \, d\mu'(t')
$$
$$
= \int^* d\mu'(t') \int^* f(t, t') \, d\mu(t).
$$

b) Si la mesure $\mu'$ est modérée, la fonction $t \mapsto \int^* f(t, t') \, d\mu'(t')$ est $\mu$-mesurable, et on a

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') \, d\mu'(t').
$$

L’assertion a), ainsi que l’assertion b) lorsque $\mu'$ est bornée, sont des conséquences de la prop. 5 du § 3, n° 2. Pour traiter le cas où $\mu'$ est modérée, représentons $\mu'$ comme une somme $\sum_{n \in \mathbf{N}} \mu'_n$ d’une suite de mesures bornées ($\S 2$, n° 3, prop. 4). La fonction $t \mapsto \int^* f(t, t') \, d\mu'_n(t')$ est alors $\mu$-mesurable, et on a

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'_n(t') = \int^* d\mu(t) \int^* f(t, t') \, d\mu'_n(t').
$$

Mais on a $\mu \otimes \mu' = \sum_{n \in \mathbf{N}} (\mu \otimes \mu'_n)$ (prop. 1); l’assertion b) s’obtient alors en sommant sur $n$ ($\S 2$, n° 2, prop. 1).

#### Corollaire 1 {#int-v-s8-prop-7-cor-1 .statement}

Soit $H$ une partie de $T \times T'$, et soit $A$ l’ensemble des $t \in T$ tels que la coupe $H(t)$ de $H$ suivant $t$ ne soit pas $\mu'$-négligeable.
a) Si $H$ est $v$-négligeable, $A$ est $\mu$-négligeable.
b) Si $H$ est localement $v$-négligeable, et si $\mu'$ est modérée, $A$ est localement $\mu$-négligeable.

La propriété a) résulte aussitôt de la prop. 7 (ou de la prop. 6). Sous l’hypothèse de b), il revient au même de dire que H(t) est localement $\mu'$-négligeable, ou $\mu'$-négligeable, puisque $\mu'$ est modérée ($\S 1$, n° 2, prop. 7). La propriété b) résulte donc de la formule (8).

Ce corollaire s’étend aussitôt, par passage aux valeurs absolues, au produit de deux mesures complexes. Il en est de même du corollaire suivant.

#### Corollaire 2 {#int-v-s8-prop-7-cor-2 .statement}

Si un ensemble $A \subset T \times T'$ est $v$-intégrable, alors, pour presque tout $t \in T$, la coupe $A(t)$ de $A$ suivant $t$ est $\mu'$-intégrable, la fonction $t \mapsto \mu'(A(t))$ est $\mu$-intégrable, et on a

$$
v(A) = \int \mu'(A(t))\ d\mu(t).
$$

#### Proposition 8 {#int-v-s8-prop-8 .statement}

Pour tout couple de fonctions numériques $f \geqslant 0, f' \geqslant 0$, définies respectivement dans $T$ et dans $T'$, on a

$$
\iint^* f(t)f'(t')\ d\mu(t)\ d\mu'(t') = \left( \int^* f(t)\ d\mu(t) \right) \left( \int^* f'(t')\ d\mu'(t') \right).
$$

Nous commencerons par traiter le cas où $\mu$ et $\mu'$ sont des mesures à support compact ; il en est alors de même pour $\mu \otimes \mu'$, et tous les symboles $\int^*$, $\iint^*$ peuvent être remplacés par des intégrales supérieures. Nous avons, d’après la prop. 6 :

$$
\iint^* f(t)f'(t')\ d\mu(t)\ d\mu'(t') \geqslant \int^* d\mu(t) \int^* f(t)f'(t')\ d\mu'(t')
$$
$$
= \left( \int^* f(t)\ d\mu(t) \right) \left( \int^* f'(t')\ d\mu'(t') \right).
$$

Pour établir l’inégalité inverse, choisissons une fonction $h \geqslant f$ (resp. $h' \geqslant f'$), enveloppe inférieure d’une suite $(h_n)$ (resp. $(h'_n)$) de fonctions semi-continues inférieurement, et telle que

$$
\int^* h(t)\ d\mu(t) = \int^* f(t)\ d\mu(t)
$$

(resp. $\int^* h'(t')\ d\mu'(t') = \int^* f'(t')\ d\mu'(t')$); l’existence de telles fonctions résulte immédiatement de la définition de l’intégrale

$$
\iint^* f(t)f'(t')\,d\mu(t)\,d\mu'(t') \leq \iint^* h(t)h'(t')\,d\mu(t)\,d\mu'(t')
$$
$$
= \left( \int^* h(t)\,d\mu(t) \right) \left( \int^* h'(t')\,d\mu'(t') \right)
$$
$$
= \left( \int^* f(t)\,d\mu(t) \right) \left( \int^* f'(t')\,d\mu'(t') \right),
$$

qui est l’inégalité cherchée. La proposition est donc établie lorsque $\mu$ et $\mu'$ sont des mesures à support compact. Pour traiter le cas général, il suffit de représenter $\mu$ (resp. $\mu'$) comme la somme d’une famille $(\mu_\alpha)_{\alpha \in A}$ (resp. $(\mu'_\beta)_{\beta \in B}$) de mesures à support compact (\S 2, n° 3, prop. 4), d’écrire la formule (10) pour chaque mesure $\mu_\alpha \otimes \mu'_\beta$, et de sommer sur $(\alpha, \beta)$ en tenant compte de la prop. 1 (\S 2, n° 1, prop. 1).

#### Corollaire 1 {#int-v-s8-prop-8-cor-1 .statement}

Avec les mêmes notations que dans la prop. 8, on a

$$
\iint^* f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int^* f(t)\,d\mu(t) \right) \left( \int^* f'(t')\,d\mu'(t') \right)
$$

sauf au plus lorsque l’un des facteurs du second membre est égal à 0 et l’autre égal à $+\infty$.

Lorsque les deux facteurs du second membre sont finis, les fonctions $f$ et $f'$ sont modérées (\S 1, n° 2, prop. 7), la fonction $f \otimes f'$ est donc modérée (cor. 2 de la prop. 5); l’égalité ci-dessus se réduit donc à la formule (10) (\S 1, n° 2, prop. 7). Lorsque l’un des facteurs du second membre vaut $+\infty$, et que l’autre n’est pas nul, le second membre vaut $+\infty$, et l’égalité ci-dessus résulte de la prop. 6.

#### Corollaire 2 {#int-v-s8-prop-8-cor-2 .statement}

Soient $f$ et $f'$ deux fonctions à valeurs dans $\mathbf{C}$ ou dans $\overline{\mathbf{R}}$, définies respectivement dans $T$ et dans $T'$, essentiellement intégrables (resp. intégrables) pour les mesures $\mu$ et $\mu'$ respectivement. La fonction $f \otimes f'$ est alors essentiellement intégrable (resp. intégrable) pour la mesure $\mu \otimes \mu'$ et on a

$$
\iint f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int f(t)\,d\mu(t) \right) \left( \int f'(t')\,d\mu'(t') \right)
$$

Lorsque $f$ et $f'$ sont positives, $f \otimes f'$ est mesurable d’après le cor. 3 de la prop. 3, et l’énoncé résulte de la formule (10) (resp. (11)), et du critère d’intégrabilité essentielle ($\S 1$, n° 3, prop. 9) (resp. du critère d’intégrabilité du chap. IV, $\S 5$, n° 6, th. 5). Le cas général en résulte immédiatement.

Le corollaire 2 s’étend aussitôt au produit de deux mesures complexes.

### 4. Intégration de fonctions à valeurs dans un espace de Banach

#### Théorème 1 (Lebesgue–Fubini) {#int-v-s8-thm-1 .statement}

Soit $\mathbf{f}$ une fonction définie dans $T \times T'$, à valeurs dans un espace de Banach $F$ ou dans $\overline{\mathbf{R}}$; soit $N$ l’ensemble des $t \in T$ tels que la fonction $t' \mapsto \mathbf{f}(t, t')$ ne soit pas $\mu'$-intégrable.

a) Supposons que $\mathbf{f}$ soit $v$-intégrable ; $N$ est alors $\mu$-négligeable, la fonction $t \mapsto \int \mathbf{f}(t, t')\, d\mu'(t')$ (définie pour $t \notin N$) est $\mu$-intégrable, et on a

$$
\iint \mathbf{f}(t, t')\, d\mu(t)\, d\mu'(t') = \int d\mu(t) \int \mathbf{f}(t, t')\, d\mu'(t').
$$

b) Supposons que $\mathbf{f}$ soit essentiellement $v$-intégrable, et que la mesure $\mu'$ soit modérée ; $N$ est alors localement $\mu$-négligeable, la fonction $t \mapsto \int \mathbf{f}(t, t')\, d\mu'(t')$ (définie pour $t \notin N$) est essentiellement $\mu'$-intégrable, et on a (13).

L’assertion a) résulte aussitôt du th. 1 du $\S 3$, n° 3. Pour établir b), désignons par $g$ une fonction $v$-intégrable, égale à $\mathbf{f}$ localement presque partout, et par $H$ l’ensemble des $(t, t')$ tels que $\mathbf{f}(t, t') \neq g(t, t')$. D’après le cor. 1 de la prop. 7, la coupe $H(t)$ est $\mu'$-négligeable, sauf pour des $t \in T$ qui forment un ensemble localement $\mu$-négligeable. Le résultat relatif à $\mathbf{f}$ se déduit donc de l’énoncé a), appliqué à $g$.

#### Scholie {#int-v-s8-n4-sch-1 .statement}

Soit $\mathbf{f}$ une fonction définie dans $T \times T'$, à valeurs dans $\overline{\mathbf{R}}$ ou dans un espace de Banach, $v$-mesurable et $v$-modérée. Pour que les trois intégrales

$$
\iint \mathbf{f}(t, t')\, d\mu(t)\, d\mu'(t'), \quad \int d\mu(t) \int \mathbf{f}(t, t')\, d\mu'(t'), \quad \int d\mu'(t') \int \mathbf{f}(t, t')\, d\mu(t)
$$

existent et soient égales, il faut et il suffit que l’un des deux nombres $\int^* d\mu(t) \int^* |\mathbf{f}(t, t')|\, d\mu'(t'), \int^* d\mu'(t') \int^* |\mathbf{f}(t, t')|\, d\mu(t)$ soit fini.

C’est une conséquence immédiate du th. 1, de la prop. 7 et du critère d’intégrabilité (chap. IV, $\S 5$, n° 6, th. 5).

#### Remarque 1 {#int-v-s8-n4-rem-1 .statement}

Lorsque la mesure $\mu'$ n’est pas modérée, il se peut que $f$ soit essentiellement $\nu$-intégrable, et que la fonction $t \mapsto f(t, t')$ ne soit essentiellement $\mu'$-intégrable pour aucune valeur de $t \in T$ (\S 3, exerc. 4).

#### Remarque 2 {#int-v-s8-n4-rem-2 .statement}

Soient $\mu$ et $\mu'$ deux mesures complexes, et soit $\nu = \mu \otimes \mu'$. Si $f$ est $\nu$-intégrable (autrement dit, $|\nu|$-intégrable), le théorème appliqué aux mesures $|\mu|$ et $|\mu'|$, dont le produit est $|\nu|$ (chap. III, 2e éd., \S 4, n° 2, prop. 3), entraîne que $t' \mapsto f(t, t')$ est $\mu'$-intégrable pour $\mu$-presque tout $t$. On en déduit, en décomposant les mesures $\mu$ et $\mu'$ en combinaison linéaire de mesures positives, que l’énoncé de a) s’étend aux mesures complexes. On peut raisonner de même pour b).

#### Proposition 9 {#int-v-s8-prop-9 .statement}

Soient $F, F'$ et $G$ trois espaces de Banach, et soit $(x, y) \mapsto [x . y]$ une application bilinéaire continue de $F \times F'$ dans $G$. Soit $f$ (resp. $f'$) une fonction définie dans $T$ (resp. $T'$) à valeurs dans $F$ (resp. $F'$) et essentiellement intégrable pour $\mu$ (resp. $\mu'$). Soit $g$ la fonction $(t, t') \mapsto [f(t) . f'(t')]$; $g$ est alors essentiellement intégrable pour $\mu \otimes \mu'$, et on a

$$
\iint [f(t) . f'(t')] \, d\mu(t) \, d\mu'(t') = \left[ \left( \int f(t) \, d\mu(t) \right) \cdot \left( \int f'(t') \, d\mu'(t') \right) \right].
$$

Si de plus $f$ et $f'$ sont intégrables, $g$ est intégrable.

La fonction $(t, t') \mapsto [f(t) . f'(t')]$ est $(\mu \otimes \mu')$-mesurable d’après le cor. 1 de la prop. 3. D’autre part, si $b$ désigne la norme de l’application bilinéaire $(x, y) \mapsto [x . y]$, on a

$$
\iint^\bullet |[f(t) . f'(t')]| \, d\mu(t) \, d\mu'(t') \leq b \int^\bullet |f(t)| \cdot |f'(t')| \, d\mu(t) \, d\mu'(t')
$$
$$
= b \left( \int^\bullet |f(t)| \, d\mu(t) \right) \left( \int^\bullet |f'(t')| \, d\mu'(t') \right)
$$

en vertu de la prop. 8. Cela montre que $[f(t) . f'(t')]$ est essentiellement intégrable pour $\mu \otimes \mu'$ (\S 1, n° 3, prop. 9). Supposons que $f$ et $f'$ soient intégrables : $f$ et $f'$ sont alors modérées, $g$ est modérée (cor. 2 de la prop. 5), donc intégrable (\S 1, n° 3, cor. de la prop. 9). Dans ce cas la formule (14) résulte du théorème de Lebesgue–Fubini et de la linéarité de l’intégrale (chap. IV, \S 4, n° 2, th. 1). Pour achever de traiter le cas où $f$ et $f'$ sont essentiellement intégrables, on applique alors (14) à deux fonctions intégrables $f_1$ et $f'_1$, égales localement presque partout à $f$ et $f'_1$, en remarquant que $[f . f'] = [f_1 . f'_1]$ localement presque partout dans $T \times T'$ (prop. 4).

Ce résultat s’étend au produit de deux mesures complexes.

### 5. Opérations sur le produit de deux mesures

#### Proposition 10 {#int-v-s8-prop-10 .statement}

Soit g (resp. g') une fonction complexe (ou une fonction à valeurs dans $\bar{\mathbf{R}}$) définie dans T (resp. T').

a) Si g (resp. g') est localement intégrable pour $\mu$ (resp. $\mu'$), la fonction $g \otimes g': (t, t') \mapsto g(t)g'(t')$ est localement intégrable pour $\nu = \mu \otimes \mu'$, et on a

$$
(g . \mu) \otimes (g' . \mu') = (g \otimes g') . (\mu \otimes \mu').
$$

(15)

b) Inversement, si $g \otimes g'$ est localement $\nu$-intégrable, et si $g'$ n’est pas localement $\mu'$-négligeable, $g$ est localement $\mu$-intégrable.

a) Soient K et K' deux parties compactes de T et de T' respectivement; le cor. 2 de la prop. 8 montre que la fonction $(t, t') \mapsto g(t)g'(t')\varphi_{K \times K'}(t, t')$, égale à $(g\varphi_K) \otimes (g'\varphi_{K'})$, est $\nu$-intégrable. Par conséquent, $g \otimes g'$ est localement $\nu$-intégrable. On vérifie alors aussitôt que le second membre de (15) satisfait à la propriété caractéristique des mesures produit (chap. III, § 4, n° 1, th. 1).

b) Supposons maintenant que $g \otimes g'$ soit localement $\nu$-intégrable, et que $g'$ ne soit pas localement $\mu'$-négligeable. Soit $\mu_1$ une mesure positive à support compact telle que $\mu_1 \leq \mu$; $g \otimes g'$ étant $(\mu_1 \otimes \mu')$-mesurable, $t \mapsto g(t)g'(t')$ est $\mu_1$-mesurable, sauf pour un ensemble localement $\mu'$-négligeable de valeurs de $t'$ (prop. 2). Comme $g'$ n’est pas nulle localement $\mu'$-presque partout, on en déduit que $g$ est $\mu_1$-mesurable, puis $\mu$-mesurable en décomposant $\mu$ en somme d’une famille de mesures à support compact (\S 2, n° 3, prop. 4 et \S 2, n° 2, prop. 2). Ce point étant établi, en peut se ramener au cas où $g$ et $g'$ sont $\geq 0$, en remplaçant $g$ et $g'$ par leurs valeurs absolues si nécessaire. Soit K un compact quelconque de T, et soit K' un compact de T' tel que $\int g'\varphi_{K'} d\mu' \neq 0$. On a d’après la prop. 8

$$
(\int g\varphi_K d\mu)(\int g'\varphi_{K'} d\mu') = \iint (g \otimes g')\varphi_{K \times K'} d\mu d\mu' < +\infty.
$$

Le premier facteur du premier membre est donc fini, et cela achève la démonstration.

Cette proposition s’étend aux mesures complexes, grâce à la prop. 3 du chap. III, 2e éd., § 4, n° 2.

#### Proposition 11 {#int-v-s8-prop-11 .statement}

Soit $\pi$ (resp. $\pi'$) une application de T (resp. T') dans un espace localement compact $T_1$ (resp. $T'_1$).

a) Si $\pi$ (resp. $\pi'$) est $\mu$-propre (resp. $\mu'$-propre), l’application $\pi \times \pi'$ est $(\mu \otimes \mu')$-propre, et on a $(\pi \times \pi')(\mu \otimes \mu') = \pi(\mu) \otimes \pi'(\mu')$.

b) Inversement, si $\pi \times \pi'$ est $(\mu \otimes \mu')$-propre, et si $\mu' \neq 0$, $\pi$ est $\mu$-propre.

a) En effet, $\pi \times \pi'$ est $(\mu \otimes \mu')$-mesurable en vertu du cor. 1 de la prop. 3 du n° 2. D’autre part, si K (resp. K') est une partie compacte de $T_1$ (resp. $T'_1$), $\pi^{-1}(K)$ et $\pi'^{-1}(K')$ sont essentiellement intégrables pour $\mu$ et $\mu'$ respectivement, donc $\pi^{-1}(K) \times \pi'^{-1}(K')$ est essentiellement intégrable pour $\mu \otimes \mu'$ (cor. 2 de la prop. 8). Ceci prouve que $\pi \times \pi'$ est $(\mu \otimes \mu')$-propre. Soient alors $\mu_1 = \pi(\mu)$, $\mu'_1 = \pi'(\mu')$, $v_1 = (\pi \times \pi')(\mu \otimes \mu')$; pour $f \in \mathcal{K}(T_1)$ et $f' \in \mathcal{K}(T'_1)$, on a
$$
\iint f(\pi(t))f'(\pi'(t'))\ d\mu(t)\ d\mu'(t') = \left( \int f(\pi(t))\ d\mu(t) \right) \left( \int f'(\pi'(t'))\ d\mu'(t') \right)
$$
(cor. 2 de la prop. 8), ce qui prouve que $v_1 = \mu_1 \otimes \mu'_1$ (chap. III, 2e éd., § 4, n° 1, th. 1).

b) Supposons maintenant que $\pi \times \pi'$ soit $\mu \otimes \mu'$-propre, et que $\mu' \neq 0$. Soit $\mu_1$ une mesure à support compact majorée par $\mu$. La fonction $\pi \times \pi'$ étant mesurable pour $\mu_1 \otimes \mu'$, l’application $t \mapsto (\pi(t), \pi'(t'))$ est $\mu$-mesurable, sauf pour des $t'$ qui forment un ensemble localement $\mu'$-négligeable (n° 2, prop. 2). Comme $\mu' \neq 0$, il en résulte que $\pi$ est $\mu_1$-mesurable, et finalement que $\pi$ est $\mu$-mesurable (\$ 2, n° 3, prop. 4 et \$ 2, n° 2, prop. 2). Reste à montrer qu’on a $\mu^*(f \circ \pi) < +\infty$ pour toute fonction $f \in \mathcal{K}_+(T_1)$. Si $\mu$ est nulle, cette propriété est évidente. Si $\mu$ n’est pas nulle, $\mu \otimes \mu'$ ne l’est pas non plus, et on a par conséquent $(\pi \times \pi')(\mu \otimes \mu') \neq 0$ (\$ 6, n° 2, prop. 2). D’après le lemme 1 du chap. III, 2e éd., § 4, il existe deux fonctions $g \in \mathcal{K}_+(T_1)$, $g' \in \mathcal{K}_+(T'_1)$, telles que
$$
\langle (\pi \times \pi')(\mu \otimes \mu'), g \otimes g' \rangle \neq 0.
$$
Cette expression étant égale à $\langle \mu \otimes \mu', (g \circ \pi) \otimes (g' \circ \pi') \rangle$ d’après la définition des mesures images, la prop. 8 entraîne que $\mu'^*(g' \circ \pi') \neq 0$. Nous avons alors, d’après la prop. 8 et la prop. 2 du § 6, n° 2,
$$
\left| \int^\bullet (f \circ \pi)\ d\mu \right| \left| \int^\bullet (g' \circ \pi')\ d\mu' \right| = \iint^\bullet (f \circ \pi) \otimes (g' \circ \pi')\ d\mu\ d\mu'
$$
$$
= \iint^\bullet (f \otimes g')\ d((\pi \times \pi')(\mu \otimes \mu')) < +\infty.
$$
La première intégrale au premier membre est donc finie, ce qui achève la démonstration.

Ce résultat s’étend aussitôt au produit de deux mesures complexes (appliquer l’énoncé à leurs valeurs absolues). Il en est de même de la proposition suivante.

#### Proposition 12 {#int-v-s8-prop-12 .statement}

Soit X (resp. X') un sous-espace localement compact de T (resp. T'). Alors la mesure induite $(\mu \otimes \mu')_{X \times X'}$ sur le sous-espace localement compact $X \times X'$ de $T \times T'$ est égale au produit $\mu_X \otimes \mu'_{X'}$ des mesures induites sur X et X' par $\mu$ et $\mu'$ respectivement.

En effet, si $f \in \mathcal{H}(X)$ et $f' \in \mathcal{H}(X')$, on a

$$
\iint_{X \times X'} f(t)f'(t')\, d\mu(t)\, d\mu'(t') = \left( \int_X f(t)\, d\mu(t) \right) \left( \int_{X'} f'(t')\, d\mu'(t') \right)
$$

en vertu du cor. 2 de la prop. 8, ce qui prouve, par définition de la mesure induite (chap. IV, 2e éd., § 5, n° 7) que

$$(\mu \otimes \mu')_{X \times X'} = \mu_X \otimes \mu'_{X'}$$

(chap. III, 2e éd., § 4, n° 1, th. 1).

### 6. Intégration par rapport à un produit fini de mesures

Les résultats précédents s’étendent sans peine à un produit d’un nombre fini de mesures. Par exemple, soient $T_1, T_2, T_3$ trois espaces localement compacts, $\mu_i$ une mesure positive sur $T_i$ ($i = 1, 2, 3$) et soit $\nu = \mu_1 \otimes \mu_2 \otimes \mu_3$ la mesure produit sur $T = T_1 \times T_2 \times T_3$. Soit $f$ une fonction $\nu$-intégrable à valeurs dans $\bar{\mathbf{R}}$ ou dans un espace de Banach ; une première application du th. de Lebesgue–Fubini montre que, sauf en des points $(t_1, t_2) \in T_1 \times T_2$ formant un ensemble négligeable (pour $\mu_1 \otimes \mu_2$), la fonction $t_3 \mapsto f(t_1, t_2, t_3)$ est $\mu_3$-intégrable, que la fonction $(t_1, t_2) \mapsto \int f(t_1, t_2, t_3)\, d\mu_3(t_3)$, définie presque partout dans $T_1 \times T_2$, est $(\mu_1 \otimes \mu_2)$-intégrable, et que l’on a

$$\iiint f(t_1, t_2, t_3)\, dv(t_1, t_2, t_3) = \iint d\mu_1(t_1)\, d\mu_2(t_2)\, \int f(t_1, t_2, t_3)\, d\mu_3(t_3).$$

Une seconde application du même théorème montre que, pour presque tout $t_1 \in T_1$, la fonction $t_2 \mapsto \int f(t_1, t_2, t_3)\, d\mu_3(t_3)$ est définie presque partout dans $T_2$ et est $\mu_2$-intégrable ; en outre, la fonction $t_1 \mapsto \int d\mu_2(t_2)\, \int f(t_1, t_2, t_3)\, d\mu_3(t_3)$, définie presque partout dans $T_1$, est $\mu_1$-intégrable, et on a

$$\iiint f(t_1, t_2, t_3)\, dv(t_1, t_2, t_3) = \int d\mu_1(t_1)\, \int d\mu_2(t_2)\, \int f(t_1, t_2, t_3)\, d\mu_3(t_3).$$

On prouve de même que, pour presque tout $t_1 \in T_1$, la fonction $(t_2, t_3) \mapsto f(t_1, t_2, t_3)$ est $(\mu_2 \otimes \mu_3)$-intégrable, que la fonction $t_1 \mapsto \int \int f(t_1, t_2, t_3)\, d\mu_2(t_2)\, d\mu_3(t_3)$, définie presque partout, est μ₁-intégrable, et que l’on a

$$ \iiint f(t_1, t_2, t_3) dv(t_1, t_2, t_3) = \int d\mu_1(t_1) \iint f(t_1, t_2, t_3) d\mu_2(t_2) d\mu_3(t_3). $$

Nous laissons au lecteur le soin de généraliser de la même manière les autres résultats démontrés ci-dessus pour le produit de deux mesures.

### 7. Application: Mesure de la boule euclidienne dans $\mathbf{R}^n$

Soient $\mu$ la mesure de Lebesgue sur $\mathbf{R}$, $\mu_n$ la mesure de Lebesgue sur $\mathbf{R}^n$, produit de $n$ facteurs égaux à $\mu$. Proposons-nous de calculer la mesure $V_n = \mu_n(\mathbf{B}_n)$ de la boule euclidienne unité. D’après le cor. 2 de la prop. 7, on a

(16)
$$
V_n = \int_{-1}^{+1} \mu_{n-1}(\mathbf{B}_n(z_n)) \, dz_n.
$$

Or, la coupe $\mathbf{B}_n(z_n)$ est la partie de $\mathbf{R}^{n-1}$ définie par la relation
$$
\sum_{i=1}^{n-1} z_i^2 \leq 1 - z_n^2,
$$
autrement dit, c’est la transformée de la boule $\mathbf{B}_{n-1}$ par l’homothétie de rapport $\sqrt{1 - z_n^2}$. Mais il résulte immédiatement de la prop. 11 et de la formule
$$
\alpha \int_{-\infty}^{+\infty} f(\alpha x) \, dx = \int_{-\infty}^{+\infty} f(z) \, dz
$$
pour $f \in \mathcal{K}(\mathbf{R})$, que l’image de $\mu_{n-1}$ par une homothétie $\mathbf{x} \mapsto \alpha \mathbf{x}$ est la mesure $\alpha^{1-n} \mu_{n-1}$. On a donc
$$
\mu_{n-1}(\mathbf{B}_n(z_n)) = (\sqrt{1 - z_n^2})^{n-1} V_{n-1}.
$$
Portant dans (16), et faisant le changement de variable $z_n = \sin \varphi \left( \text{avec } -\frac{\pi}{2} \leq \varphi \leq \frac{\pi}{2} \right)$, il vient
(17)
$$
V_n = V_{n-1} \int_{-\pi/2}^{+\pi/2} \cos^n \varphi \, d\varphi = 2 V_{n-1} \int_0^{\pi/2} \cos^n \varphi \, d\varphi.
$$
Mais on a (Fonct. var. réelle, chap. VII, § 1, n° 3, formule (20))
$$
\int_0^{\pi/2} \cos^m \varphi \, d\varphi = \frac{1}{2} \frac{\Gamma\left(\frac{1}{2}\right) \Gamma\left(\frac{m+1}{2}\right)}{\Gamma\left(\frac{m+2}{2}\right)}
$$

$$
V_n = \frac{\pi^{n/2}}{\Gamma\left(\frac{n}{2} + 1\right)}
$$

## EXERCICES {#int-v-s8-exercises}

See the [exercises for § 8](exercises/s8/).
