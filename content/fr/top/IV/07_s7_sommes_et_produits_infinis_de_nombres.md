---
book: top
book_title: General Topology
chapter: IV
chapter_title: NOMBRES RÉELS
section: 7
section_title: Sommes et produits infinis de nombres réels
lang: fr
source: top-i-iv-fr
book_pages: TG IV.32-TG IV.39, TG IV.59-TG IV.61
pdf_pages: 0303-0310, 0330-0332
extraction: ocr
subsections:
    - "no": 1
      title: Familles sommables dans $\mathbf{R}$ de nombres finis positifs
      page: 32
      pdf_page: 303
    - "no": 2
      title: Familles sommables dans $\mathbf{R}$ de nombres finis de signe quelconque
      page: 34
      pdf_page: 305
    - "no": 3
      title: Produit de deux sommes infinies
      page: 35
      pdf_page: 306
    - "no": 4
      title: Familles multipliables dans $\mathbf{R}^*$
      page: 35
      pdf_page: 306
    - "no": 5
      title: Familles sommables et familles multipliables dans $\overline{\mathbf{R}}$
      page: 37
      pdf_page: 308
    - "no": 6
      title: Séries et produits infinis de nombres réels
      page: 38
      pdf_page: 309
statements: 26
exercises: 22
content_sha256: bd260491dd1441dcc19d98698ff22398e4eb75bdf06991ab6d267d3178fc6a6b
---

## § 7. SOMMES ET PRODUITS INFINIS DE NOMBRES RÉELS

Comme tout point de $\mathbf{R}$ possède un système fondamental *dénombrable* de voisinages (IV, p. 4, corollaire), une famille $(x_i)$ de nombres réels *finis* ne peut être sommable dans $\mathbf{R}$ que si l’ensemble des indices $i$ tels que $x_i \neq 0$ est *dénombrable* (III, p. 39, cor. 1). L’étude des familles sommables dans $\mathbf{R}$ est donc essentiellement ramenée à celle des *suites* sommables. Toutefois, il arrivera qu’on ait à considérer une famille non dénombrable $(x_i)$ de nombres réels finis, dont les termes seront fonctions d’un paramètre $t$; il pourra se faire que cette famille soit sommable quel que soit $t$, mais que l’ensemble (dénombrable) des indices $i$ tels que $x_i \neq 0$ dépende de $t$. Aussi ne ferons-nous, dans ce qui suit, aucune hypothèse sur le cardinal de l’ensemble des indices.

### 1. Familles sommables dans $\mathbf{R}$ de nombres finis positifs

#### Théorème 1 {#top-iv-s7-thm-1 .statement}

*Pour qu’une famille $(x_i)$ de nombres réels finis $\geqslant 0$ soit sommable dans $\mathbf{R}$, il faut et il suffit que l’ensemble des sommes partielles finies de cette famille soit majoré dans $\mathbf{R}$. La borne supérieure de cet ensemble est alors la somme de la famille $(x_i)$.*.

En effet, pour toute partie finie $H$ de l’ensemble d’indices $I$, posons $s_H = \sum_{i \in H} x_i$; comme les $x_i$ sont $\geqslant 0$, la relation $H \subset H'$ entraîne $s_H \leqslant s_{H'}$. En d’autres termes, l’application $H \mapsto s_H$ est *croissante* dans l’ensemble filtrant $\mathcal{F}(I)$ des parties finies de $I$; donc (IV, p. 18, corollaire), pour qu’elle ait une limite finie, il faut et il suffit qu’elle soit *majorée*.

#### Remarque {#top-iv-s7-n1-rem-1 .statement}

Soit $(H_\lambda)$ une famille de parties finies de $I$ telle que, pour toute partie finie $H$ de $I$, il existe un indice $\lambda$ tel que $H \subset H_\lambda$; pour que $(x_i)$ soit sommable, il faut et il suffit évidemment que la famille des $s_{H_\lambda}$ soit *majorée* dans $\mathbf{R}$. En particulier, soit $(x_n)$ une suite de nombres finis $\geqslant 0$, et posons, pour tout entier $n$, $s_n = \sum_{p=0}^n x_p$; pour que la suite $(x_n)$ soit sommable dans $\mathbf{R}$, il faut et il suffit que, pour *une suite* d’entiers strictement croissante $(n_k)$, la suite partielle $(s_{n_k})$ soit *majorée* dans $\mathbf{R}$.

#### Exemple 1 {#top-iv-s7-n1-exa-1 .statement}

Pour tout nombre $q$ tel que $0 \leqslant q < 1$, la suite $(q^n)$ (*« progression géométrique de raison $q$ »*) est sommable dans $\mathbf{R}$, car $s_n = \frac{1 - q^{n+1}}{1 - q} \leqslant \frac{1}{1 - q}$; la somme de cette suite est $\lim_{n \to \infty} s_n = \frac{1}{1 - q}$.

#### Exemple 2 {#top-iv-s7-n1-exa-2 .statement}

Soient $a$ et $b$ deux nombres tels que $0 \leqslant a < 1,\ 0 \leqslant b < 1$; la famille $(a^m b^n)_{(m,n) \in \mathbf{N} \times \mathbf{N}}$ est sommable dans $\mathbf{R}$. En effet, toute partie finie de $\mathbf{N} \times \mathbf{N}$ est contenue dans une partie de la forme $(0, p) \times (0, p)$; et l’on a
$$
\sum_{m=0}^p \sum_{n=0}^p a^m b^n = \left( \sum_{m=0}^p a^m \right) \left( \sum_{m=0}^p b^n \right) = \frac{1 - a^{p+1}}{1 - a} \cdot \frac{1 - b^{p+1}}{1 - b} \leqslant \frac{1}{(1 - a)(1 - b)}.
$$

#### Exemple 3 {#top-iv-s7-n1-exa-3 .statement}

Pour tout entier $p > 1$, la suite $(n^{-p})$ ($n > 0$) est sommable, car on a
$$
s_{2^n+1} - s_{2^n} = \sum_{k=1}^{2^n} (2^n + k)^{-p} < 2^n \cdot (2^n)^{-p}
$$
d’où, en ajoutant membre à membre ces inégalités
$$
s_{2^n} < \frac{1}{1 - 2^{1-p}}.
$$

#### Exemple 4 {#top-iv-s7-n1-exa-4 .statement}

La suite $(1/n)$ ($n > 0$) n’est pas sommable dans $\mathbf{R}$, car on a
$$
s_{2^n+1} - s_{2^n} = \sum_{k=1}^{2^n} \frac{1}{2^n + k} > \frac{2^n}{2^{n+1}} = \frac{1}{2}
$$
d’où, en ajoutant membre à membre
$$
s_{2^n} > n/2
$$
et le critère du th. 1 n’est donc pas satisfait.

#### Exemple 5 {#top-iv-s7-n1-exa-5 .statement}

Soit $(I_n)$ une suite d’intervalles ouverts non vides, sans point commun deux à deux, contenus dans un intervalle de longueur finie $l$; la somme des longueurs d’un nombre fini d’intervalles de cette famille est $\leq l$ (IV, p. 5), donc la famille des longueurs des $I_n$ est sommable dans $\mathbf{R}$, et sa somme est $\leq l$.

#### Théorème 2 (principe de comparaison) {#top-iv-s7-thm-2 .statement}

*Soient* $(x_i)_{i \in I}$ *et* $(y_i)_{i \in I}$ *deux familles de nombres finis* $\geq 0$, *telles que* $x_i \leq y_i$ *quel que soit* $i$. *Si* $(y_i)$ *est sommable dans* $\mathbf{R}$, *il en est de même de* $(x_i)$ *et on a* $\sum_i x_i \leq \sum_i y_i$; *si en outre il existe un indice* $\kappa$ *tel que* $x_\kappa < y_\kappa$, *on a* $\sum_i x_i < \sum_i y_i$.

L’hypothèse entraîne que, pour toute partie finie $H$ de $I$, $\sum_{i \in H} x_i \leq \sum_{i \in H} y_i$, d’où la première partie du théorème, d’après le th. 1; l’inégalité sur les sommes résulte du principe de prolongement des inégalités (IV, p. 18, th. 1). Si $x_\kappa < y_\kappa$, on a
$$
\sum_i x_i = x_\kappa + \sum_{i \neq \kappa} x_i < y_\kappa + \sum_{i \neq \kappa} y_i = \sum_i y_i.
$$

Ce théorème fournit le critère le plus fréquemment employé pour décider si une suite $(x_n)$ de nombres positifs est ou non sommable dans $\mathbf{R}$; on cherche à la comparer à une suite $(y_n)$ plus simple, pour laquelle on sait déjà si elle est sommable ou non; s’il existe un nombre fini $a > 0$ tel que $x_n \leq ay_n$ pour tout $n$ à partir d’un certain rang, et si $(y_n)$ est sommable, il en est de même de $(x_n)$; si au contraire il existe un nombre fini $b > 0$ tel que $x_n \geq by_n$ pour tout $n$ à partir d’un certain rang, et si $(y_n)$ n’est pas sommable dans $\mathbf{R}$, $(x_n)$ n’est pas sommable dans $\mathbf{R}$. Nous verrons ultérieurement (FVR, V, §4) comment peut se faire cette recherche des suites de comparaison dans les cas qui se présentent le plus fréquemment.

#### Exemple 6 {#top-iv-s7-n1-exa-6 .statement}

Considérons, pour un nombre réel fini $a > 0$, la suite $\left( \frac{a^n}{n!} \right)$; soit $n_0$ le plus petit entier tel que $a < n_0$. Pour tout $n \geq n_0$, on a
$$
\frac{a^n}{n!} \leq \frac{a^{n_0}}{n_0!} \left( \frac{a}{n_0} \right)^{n-n_0}
$$

et comme $q = \frac{a}{n_0} < 1$, la suite $(q^{n-n_0})$ est sommable, donc aussi $\left( \frac{a^n}{n!} \right)$.

#### Exemple 7 {#top-iv-s7-n1-exa-7 .statement}

Soit $(a_n)$ une suite sommable de nombres positifs; comme $\lim_{n \to \infty} a_n = 0$, il existe un entier $n_0$ tel que, pour $n \geq n_0$, $a_n \leq 1$; par suite, pour tout $n \geq n_0$, $a_n^2 \leq a_n$, ce qui montre que la suite $(a_n^2)$ est sommable dans $\mathbf{R}$; il en est de même de $(a_n^p)$ pour tout entier $p > 1$.

#### Exemple 8 {#top-iv-s7-n1-exa-8 .statement}

Soient $a$ et $b$ deux nombres tels que $a > 1, b > 1$; on a

$$
\frac{1}{a^m + b^n} \leq \frac{1}{2(\sqrt{a})^m (\sqrt{b})^n},
$$

donc la famille $\left( \frac{1}{a^m + b^n} \right)$ est sommable dans $\mathbf{R}$.

#### Corollaire {#top-iv-s7-n1-cor-1 .statement}

*Soit* $(x_i)_{i \in I}$ *une famille sommable dans* $\mathbf{R}$ *de nombres finis* $\geq 0$; *pour toute partie* $\mathbf{H}$ *de* $\mathbf{I}$, *on a*

$$
\sum_{i \in \mathbf{H}} x_i \leq \sum_{i \in \mathbf{I}} x_i
$$

*les deux membres n’étant égaux que si* $x_i^i = 0$ *quel que soit* $i \in \mathbf{CH}$.

### 2. Familles sommables dans $\mathbf{R}$ de nombres finis de signe quelconque

#### Théorème 3 {#top-iv-s7-thm-3 .statement}

*Soit* $(x_i)_{i \in I}$ *une famille de nombres réels finis*. *Les propriétés suivantes sont équivalentes*:

a) *la famille* $(x_i)$ *est sommable dans* $\mathbf{R}$;
b) *la famille* $(|x_i|)$ *est sommable dans* $\mathbf{R}$;
c) *l’ensemble des sommes partielles finies de la famille* $(x_i)$ *est borné dans* $\mathbf{R}$.

Soit $I_1$ l’ensemble des $i \in I$ tels que $x_i \geq 0$, $I_2$ l’ensemble des $i \in I$ tels que $x_i < 0$. Pour que la famille $(x_i)_{i \in I}$ (resp. $(|x_i|)_{i \in I}$) soit sommable, il faut et il suffit que chacun des familles $(x_i)_{i \in I_1}$ et $(x_i)_{i \in I_2}$ (resp. $(|x_i^i|)_{i \in I_1}$ et $(|x_i|)_{i \in I_2}$) le soit (III, p. 39, prop. 2 et III, p. 41, prop. 3). Or, il revient au même de dire que $(x_i)_{i \in I_1}$ est sommable, ou que $(|x_i|)_{i \in I_1}$ est sommable, ou que l’ensemble des sommes partielles finies de la famille $(x_i)_{i \in I_1}$ est borné (IV, p. 32, th. 1); et la même assertion est valable en remplaçant $I_1$ par $I_2$. D’où aussitôt le théorème.

Le th. 3 montre que l’étude de la sommabilité dans $\mathbf{R}$ d’une famille de nombres réels finis est entièrement ramenée à celle de la famille de leurs valeurs absolues.

Rappelons (III, p. 42, prop. 6) que, si $(x_i)$ et $(y_i)$ sont deux familles sommables de nombres réels finis, la famille $(x_i + y_i)$ est sommable, et

$$
\sum_i (x_i + y_i) = \sum_i x_i + \sum_i y_i.
$$

En outre, si $(x_i)$ est une famille sommable de nombres réels finis, et $a$ un nombre fini quelconque, la famille $(ax_i)$ est sommable dans $\mathbf{R}$, et on a $\sum_i ax_i^i = a \sum_i x_i$.

### 3. Produit de deux sommes infinies

#### Proposition 1 {#top-iv-s7-prop-1 .statement}

Si les familles $(x_\lambda)_{\lambda \in L}$ et $(y_\mu)_{\mu \in M}$ de nombres réels finis sont sommables dans $\mathbf{R}$, il en est de même de la famille $(x_\lambda y_\mu)_{(\lambda, \mu) \in L \times M}$ et on a

$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = (\sum_{\lambda \in L} x_\lambda)(\sum_{\mu \in M} y_\mu).
$$

Toute partie finie de $L \times M$ est contenue dans une partie finie de la forme $H \times K$, où $H$ est une partie finie de $L$, $K$ une partie finie de $M$. Par hypothèse, il existe un nombre $a > 0$ tel que $\sum_{\lambda \in H} |x_\lambda| \leq a$ et $\sum_{\mu \in K} |y_\mu| \leq a$, quelles que soient les parties finies $H$ et $K$ de $L$ et $M$ respectivement; donc

$$
\sum_{(\lambda, \mu) \in H \times K} |x_\lambda y_\mu| = (\sum_{\lambda \in H} |x_\lambda|)(\sum_{\mu \in K} |y_\mu|) \leq a^2,
$$

ce qui prouve que la famille $(x_\lambda y_\mu)$ est sommable dans $\mathbf{R}$, d’après les th. 1 (IV, p. 32) et 3 (IV, p. 34). D’après l’associativité de la somme, on peut écrire (III, p. 40, formule (2))

$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = \sum_{\lambda \in L} (\sum_{\mu \in M} x_\lambda y_\mu) = \sum_{\lambda \in L} x_\lambda (\sum_{\mu \in M} y_\mu) = (\sum_{\lambda \in L} x_\lambda)(\sum_{\mu \in M} y_\mu)
$$

d’où la proposition.

### 4. Familles multipliables dans $\mathbf{R}^*$

Dans le groupe multiplicatif $\mathbf{R}^*$ des nombres réels finis et $\neq 0$, une famille $(x_i)_{i \in I}$ ne peut être multipliable que si $\lim x_i = 1$ suivant le filtre des complémentaires des parties finies de $I$ (III, p. 38, prop. 1). En particulier, il ne peut y avoir qu’un nombre fini d’indices $i$ tels que $x_i < 0$. Nous pouvons donc nous borner à ne considérer que des familles $(x_i)$ dont tous les termes soient strictement positifs; il est commode alors de poser $x_i = 1 + u_i$, où les $u_i$ sont soumis aux conditions $-1 < u_i < +\infty$ quel que soit $i$. Comme tout point de $\mathbf{R}^*$ a un système fondamental dénombrable de voisinages, l’ensemble des $i$ tels que $u_i \neq 0$ est dénombrable si la famille $(1 + u_i)$ est multipliable dans $\mathbf{R}^*$.

#### Théorème 4 {#top-iv-s7-thm-4 .statement}

Pour que la famille $(1 + u_i)$ soit multipliable dans $\mathbf{R}^*$, il faut et il suffit que la famille $(u_i)$ soit sommable dans $\mathbf{R}$.

#### Lemme {#top-iv-s7-n4-lem-1 .statement}

1° Si $(a_i)_{1 \leq i \leq p}$ est une suite finie de nombres $> 0$,

$$
\prod_{i=1}^p (1 + a_i) \geq 1 + \sum_{i=1}^p a_i.
$$

2° Si en outre $a_i < 1$ quel que soit $i$,

$$
\prod_{i=1}^p (1 - a_i) \geq 1 - \sum_{i=1}^p a_i.
$$

Ces relations sont évidentes si $p = 1$; elles se démontrent par récurrence sur $p$.

Si
$$
\prod_{i=1}^{p-1} (1 + a_i) \geq 1 + \sum_{i=1}^{p-1} a_i,
$$
on a
$$
\prod_{i=1}^p (1 + a_i) \geq (1 + a_p)(1 + \sum_{i=1}^{p-1} a_i)
$$
$$
= 1 + \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 + \sum_{i=1}^p a_i.
$$

De même, si
$$
\prod_{i=1}^{p-1} (1 - a_i) \geq 1 - \sum_{i=1}^{p-1} a_i,
$$
on a
$$
\prod_{i=1}^p (1 - a_i) \geq (1 - a_p)(1 - \sum_{i=1}^{p-1} a_i) = 1 - \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 - \sum_{i=1}^p a_i.
$$

Ce lemme étant démontré, remarquons que, si la famille $(1 + u_\iota)$ est multipliable, il en est de même des familles $(1 + u_\iota^+)$ et $(1 - u_\iota^-)$ puisque $\mathbf{R}^*$ est un groupe complet (III, p. 39, prop. 2); et réciproquement, si les familles $(1 + u_\iota^+)$ et $(1 - u_\iota^-)$ sont multipliables, il en est de même de $(1 + u_\iota)$ (III, p. 41, prop. 3). On peut donc se borner à considérer séparément le cas où tous les $u_\iota$ sont $\geq 0$, et celui où ils sont tous $\leq 0$.

Supposons d’abord $u_\iota \geq 0$ quel que soit $\iota$. Si la famille $(1 + u_\iota)$ est multipliable, pour tout $\varepsilon > 0$ il existe une partie finie $J$ de l’ensemble d’indices $I$ telle que, pour toute partie finie $H$ de $I$ ne rencontrant pas $J$, on ait
$$
1 \leq \prod_{\iota \in H} (1 + u_\iota) \leq 1 + \varepsilon;
$$
d’après (2), il en résulte que $\sum_{\iota \in H} u_\iota \leq \varepsilon$, ce qui montre que $(u_\iota)$ est sommable dans $\mathbf{R}$ en vertu du critère de Cauchy (III, p. 38, th. 1).

Réciproquement, supposons $(u_\iota)$ sommable dans $\mathbf{R}$. Pour tout $\varepsilon$ tel que $0 < \varepsilon < 1$, il existe une partie finie $J$ de $I$ telle que, pour toute partie finie $H$ de $I$ ne rencontrant pas $J$, on ait $0 \leq \sum_{\iota \in H} u_\iota \leq \varepsilon$. D’après (3), on a donc
$$
\prod_{\iota \in H} (1 - u_\iota) \geq 1 - \varepsilon; \text{ mais on a } 1 + u \leq \frac{1}{1 - u} \text{ pour tout nombre } u \text{ tel que } 0 \leq u < 1,
$$
donc
$$
1 \leq \prod_{\iota \in H} (1 + u_\iota) \leq \frac{1}{1 - \varepsilon}
$$
ce qui montre que $(1 + u_\iota)$ est multipliable (critère de Cauchy).

La démonstration est analogue lorsque tous les $u_i$ sont $\leq 0$. Pour établir que $(u_i)$ est sommable lorsque $(1 + u_i)$ est multipliable, on utilisera ici la formule (2), ainsi que l’inégalité $1 - u \leq \frac{1}{1 + u}$ pour $0 \leq u < 1$; pour montrer que $(1 + u_i)$ est multipliable lorsque $(u_i)$ est sommable, on utilisera la formule (3).

Dans V, §4, l’étude topologique du groupe $\mathbf{R}^*$ nous permettra de donner un autre critère de multipliabilité d’une famille dans $\mathbf{R}^*$; à l’aide de la fonction logarithme; nous retrouverons plus tard l’équivalence de ce critère et du précédent, au moyen des propriétés différentielles du logarithme (FVR, V, §4, n° 3).

### 5. Familles sommables et familles multipliables dans $\overline{\mathbf{R}}$

Dans l’intervalle $(0, +\infty)$ de $\overline{\mathbf{R}}$, l’addition est une loi de composition associative et commutative (IV, p. 16); donc la notion de famille sommable de nombres de cet intervalle est encore définie (III, p. 37, Remarque 3).

#### Proposition 2 {#top-iv-s7-prop-2 .statement}

Toute famille $(x_i)$ de nombres réels positifs est sommable dans $\overline{\mathbf{R}}$.

En effet, l’application $H \mapsto s_H$ de l’ensemble ordonné filtrant $\mathfrak{F}(I)$ dans $\overline{\mathbf{R}}$ est croissante, donc (IV, p. 18, th. 2) a une limite.

Le même raisonnement montre que toute famille de nombres réels négatifs est sommable dans $\overline{\mathbf{R}}$.

De même, la multiplication est une loi de composition associative et commutative dans chacun des intervalles $(0, 1)$ et $(1, +\infty)$ de $\overline{\mathbf{R}}$; la notion de famille multipliable est donc définie dans chacun de ces intervalles.

#### Proposition 3 {#top-iv-s7-prop-3 .statement}

Toute famille $(1 + u_i)$ (resp. $(1 - u_i)$) de nombres $\geq 1$ (resp. $\geq 0$ et $\leq 1$) est multipliable dans $\overline{\mathbf{R}}$.

Même démonstration que pour la prop. 2.

#### Corollaire {#top-iv-s7-n5-cor-1 .statement}

Pour que le produit $\prod_i (1 + u_i)$ (resp. $\prod_i (1 - u_i)$) de nombres $\geq 1$ (resp. strictement positifs et $\leq 1$) soit égal à $+\infty$ (resp. à 0), il faut et il suffit que $\sum_i u_i = +\infty$.

En effet, si $\sum_i u_i$ est finie, $\prod_i (1 + u_i)$ et $\prod_i (1 - u_i)$ appartiennent à $\mathbf{R}^*$, et réciproquement, d’après le th. 4 de IV, p. 35.

#### Remarque {#top-iv-s7-n5-rem-1 .statement}

Le théorème d’associativité (III, p. 39, th. 2) est encore valable quand on remplace G par $\overline{\mathbf{R}}$ et qu’on suppose les $x_i \geq 0$. En effet, cela est évident si $\sum_{i \in I} x_i$ est fini; supposons au contraire $\sum_{i \in I} x_i = +\infty$. Alors, pour tout $a$ fini et $> 0$ il existe une partie finie H de I telle que $\sum_{i \in H} x_i \geq a$; soit K une partie finie de L telle que $H \subset \bigcup_{\lambda \in K} I_\lambda$; comme on a $s_\lambda \geq \sum_{i \in I_\lambda \cap H} x_i$ pour tout $\lambda \in K$, on a

$$
\sum_{\lambda \in K} s_\lambda \geq \sum_{i \in H} x_i \geq a, \text{ ce qui prouve que } \sum_{\lambda \in L} s_\lambda = +\infty. \text{ Nous laissons au lecteur le soin d'énoncer la proposition analogue pour les familles multipliables de nombres de } \{0, 1\} \text{ ou de } \{1, +\infty\}.
$$

### 6. Séries et produits infinis de nombres réels

On dit simplement qu’une série de nombres réels finis est convergente lorsqu’elle est convergente dans $\mathbf{R}$.

#### Définition 1 {#top-iv-s7-def-1 .statement}

Une série de nombres réels finis est dite absolument convergente si la série des valeurs absolues de ses termes est convergente.

#### Proposition 4 {#top-iv-s7-prop-4 .statement}

Pour qu’une série de nombres réels finis soit commutativement convergente, il faut et il suffit qu’elle soit absolument convergente.

Cela résulte en effet de III, p. 44, prop. 9 et du th. 3 de IV, p. 34.

Autrement dit, si $(u_n)$ est une suite de nombres réels finis, il revient au même de dire que la série de terme général $u_n$ est commutativement convergente, ou qu’elle est absolument convergente, ou que la suite $(u_n)$ est sommable dans $\mathbf{R}$. Toutes les propriétés des familles sommables, démontrées dans III, p. 39 à p. 42, s’appliquent donc aux séries absolument convergentes. En particulier, si la série de terme général $u_n$ est absolument convergente, la somme $\sum_{n \in H} u_n$ existe quelle que soit la partie $H$ de $\mathbf{N}$; et, si $(H_p)$ est une partition de $\mathbf{N}$, on a $\sum_{n=0}^\infty u_n = \sum_p (\sum_{n \in H_p} u_n)$ (associativité des séries absolument convergentes).

Comme on l’a déjà signalé (III, p. 43), une série de nombres réels peut être convergente sans être commutativement convergente, ou, ce qui revient au même, sans être absolument convergente.

#### Exemple {#top-iv-s7-n6-exa-1 .statement}

Séries alternées. — Une série définie par une suite $(u_n)$ de nombres réels finis, est dite alternée si $u_n = (-1)^n v_n$, avec $v_n \geq 0$ quel que soit $n$. Montrons qu’une condition suffisante pour qu’une telle série converge, est que la suite $(v_n)$ soit décroissante et ait pour limite 0. En effet, si on pose $s_n = \sum_{p=0}^n u_p$, l’hypothèse que $(v_n)$ est décroissante entraîne que

$$
s_{2n+1} \leq s_{2n+3} \leq s_{2n+2} \leq s_{2n}
$$

quel que soit $n \geq 0$. La suite $(s_{2n})$ (resp. $(s_{2n+1})$) est décroissante et minorée (resp. croissante et majorée); elle a donc une limite finie $a$ (resp. $b$), et on a $b \leq a$; comme $a - b = \lim_{n \to \infty} (s_{2n} - s_{2n+1}) = \lim_{n \to \infty} v_{2n+1} = 0$, la proposition est démontrée.

Si on prend par exemple $v_n = 1/n$, les hypothèses précédentes sont satisfaites, donc la série de terme général $(-1)^n / n$ (« série harmonique alternée ») est convergente; on a vu (IV, p. 33) que la série de terme général $1/n$ (« série harmonique ») n’est pas convergente, donc la série harmonique alternée n’est pas absolument convergente.

Rappelons (III, p. 43, prop. 7) que, si $(u_n)$ et $(v_n)$ sont deux séries convergentes de nombres réels finis, la série $(u_n + v_n)$ est convergente, et

$$
\sum_{n=0}^{\infty} (u_n + v_n) = \sum_{n=0}^{\infty} u_n + \sum_{n=0}^{\infty} v_n;
$$

de même, si la série $(u_n)$ est convergente, la série $(au_n)$ est convergente, quel que soit le nombre fini $a$, et $\sum_{n=0}^{\infty} au_n = a \cdot \sum_{n=0}^{\infty} u_n$.

Enfin, si les séries $(u_n)$ et $(v_n)$ sont convergentes, et si $u_n \leq v_n$ quel que soit $n$, on a $\sum_{n=0}^{\infty} u_n \leq \sum_{n=0}^{\infty} v_n$, d’après le principe de prolongement des inégalités (IV, p. 18, th. 1).

Il faut noter que, si on suppose la série $(v_n)$ convergente mais non absolument convergente, et si $|u_n| \leq |v_n|$ pour tout $n$, on ne peut nullement en conclure que la série $(u_n)$ soit convergente, comme on le voit en prenant $u_n = |v_n|$.

On dit simplement qu’un produit infini de nombres réels finis et $\neq 0$ est convergent s’il est convergent dans $\mathbf{R}^*$; sa valeur est donc un nombre fini et non nul.

#### Définition 2 {#top-iv-s7-def-2 .statement}

Un produit infini de facteur général $1 + u_n$ est dit absolument convergent si le produit de facteur général $1 + |u_n|$ est convergent.

#### Proposition 5 {#top-iv-s7-prop-5 .statement}

Pour qu’un produit infini de nombres réels finis soit commutativement convergent, il faut et il suffit qu’il soit absolument convergent.

Cela résulte de III, p. 44, prop. 9 et du th. 4 de IV, p. 35.

De plus, pour que le produit de facteur général $1 + u_n$ soit absolument convergent, il faut et il suffit que la série de terme général $u_n$ soit absolument convergente.

Un produit de nombres réels $\neq 0$ peut être convergent sans être commutativement convergent, ou, ce qui revient au même, sans être absolument convergent.

#### Exemple {#top-iv-s7-n6-exa-2 .statement}

Si on prend, pour $n \geq 2$, $u_{2n-1} = -1/n, u_{2n} = 1/n$, le produit $(1 + u_n)$ n’est pas absolument convergent, puisque la série $(u_n)$ n’est pas absolument convergente; mais, comme

$$
\prod_{p=3}^{2n} (1 + u_p) = \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right), \quad \prod_{p=3}^{2n+1} (1 + u_p) = \left(1 - \frac{1}{n+1}\right) \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right)
$$

il résulte du th. 4 que le produit est convergent, et a pour valeur

$$
\prod_{n=2}^{\infty} \left(1 - \frac{1}{n^2}\right).
$$

En outre, il faut observer que la convergence de la série de terme général $u_n$ n’est ni nécessaire ni suffisante pour que le produit de facteur général $1 + u_n$ soit convergent (voir IV, p. 60, exerc. 21 et 22).

## EXERCICES {#top-iv-s7-exercises}

See the [exercises for § 7](exercises/s7/).
