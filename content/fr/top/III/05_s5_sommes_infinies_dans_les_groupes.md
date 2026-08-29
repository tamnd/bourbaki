---
book: top
book_title: General Topology
chapter: III
chapter_title: GROUPES TOPOLOGIQUES
section: 5
section_title: Sommes infinies dans les groupes commutatifs
lang: fr
source: top-i-iv-fr
book_pages: TG III.36-TG III.45, TG III.78-TG III.79
pdf_pages: 0219-0228, 0261-0262
extraction: ocr
subsections:
    - "no": 1
      title: Familles sommables dans un groupe commutatif
      page: 36
      pdf_page: 219
    - "no": 2
      title: Le critère de Cauchy
      page: 38
      pdf_page: 221
    - "no": 3
      title: Sommes partielles. Associativité
      page: 39
      pdf_page: 222
    - "no": 4
      title: Familles sommables dans un produit de groupes
      page: 41
      pdf_page: 224
    - "no": 5
      title: Image d’une famille sommable par un homomorphisme continu
      page: 41
      pdf_page: 224
    - "no": 6
      title: Séries
      page: 42
      pdf_page: 225
    - "no": 7
      title: Séries commutativement convergentes
      page: 44
      pdf_page: 227
statements: 21
exercises: 6
content_sha256: 4feb8ea76c1b1eafb8f7f4a619f2881784f62ff52bacf148b3e50053f846ff44
---

## § 5. SOMMES INFINIES DANS LES GROUPES COMMUTATIFS

### 1. Familles sommables dans un groupe commutatif

Dans ce paragraphe, il n’est question que de groupes topologiques commutatifs séparés, dont la loi de composition est notée additivement; la traduction en notation multiplicative ne sera donnée que pour les résultats les plus importants.

Soient G un groupe commutatif séparé, I un ensemble d’indices quelconque, $(x_i)_{i \in I}$ une famille de points de G, dont l’ensemble d’indices est I. A toute partie finie J de I, faisons correspondre l’élément $s_J = \sum_{i \in J} x_i$ de G, que nous appellerons somme partielle finie de la famille $(x_i)_{i \in I}$, correspondant à l’ensemble J, et qui a été défini en Algèbre (A, I, p. 13; on rappelle qu’on pose, par convention, $\sum_{i \in \emptyset} x_i = 0$). Si $\mathfrak{F}(I)$ désigne l’ensemble des parties finies de I, on définit ainsi une application $J \mapsto s_J$ de $\mathfrak{F}(I)$ dans G. Or, $\mathfrak{F}(I)$, ordonné par la relation $\subset$, est un ensemble filtrant pour cette relation (E, III, p. 12): en effet, si J et J’ sont deux éléments de $\mathfrak{F}(I)$, on a $J \subset J \cup J', J' \subset J \cup J'$, et $J \cup J'$ est encore une partie finie de I. Soit $\Phi$ le filtre des sections de l’ensemble filtrant $\mathfrak{F}(I)$.

#### Définition 1 {#top-iii-s5-def-1 .statement}

Soit $(x_i)_{i \in I}$ une famille de points d’un groupe commutatif séparé G; soit $\mathfrak{F}(I)$ l’ensemble des parties finies de l’ensemble d’indices I; pour tout partie-finie J de I, soit $s_J$ la somme des $x_i$ tels que $i \in J$. On dit que la famille $(x_i)_{i \in I}$ est sommable si l’application $J \mapsto s_J$ a une limite suivant le filtre $\Phi$ des sections de l’ensemble $\mathfrak{F}(I)$ des parties finies de I ordonné par la relation $\subset$; cette limite est alors appelée la somme de la famille $(x_i)_{i \in I}$ et se note $\sum_{i \in I} x_i$ (ou simplement $\sum_i x_i$, et même $\sum x_i$ lorsqu’aucune confusion ne peut en résulter).

La déf. 1 équivaut à la suivante: la famille $(x_i)$ est sommable et a pour somme s, si, pour tout voisinage V de l’origine dans G, il existe une partie finie $J_0$ de I telle que, pour toute partie finie $J \supset J_0$ de I, on ait $s_J \in s + V$.

Si G est noté multiplicativement, et si on pose $p_J = \prod_{i \in J} x_i$ pour toute partie finie J de I, la famille $(x_i)$ sera dite multipliable si l’application $J \mapsto p_J$ a une limite suivant le filtre $\Phi$; cette limite sera appelée le produit de la famille $(x_i)$, et notée $\prod_{i \in I} x_i$.

#### Remarque 1 {#top-iii-s5-n1-rem-1 .statement}

Lorsque I est fini, la déf. 1 redonne la définition ordinaire de la somme d’une famille finie. Plus généralement, si I est quelconque, et si $x_i = 0$ sauf pour les indices i appartenant à une partie finie J de I, la somme $\sum_{i \in I} x_i$ est égale à $\sum_{i \in J} x_i$, et coïncide donc avec la somme définie dans ce cas en Algèbre (A, I, p. 14).

#### Remarque 2 {#top-iii-s5-n1-rem-2 .statement}

La définition d’une famille sommable ne fait intervenir aucune relation d’ordre sur l’ensemble d’indices I; on peut donc dire que la notion de somme ainsi définie est commutative. De façon plus précise, on a la propriété suivante: soit $(x_i)_{i \in I}$ une famille sommable, $\varphi$ une application bijective d’un ensemble d’indices K sur l’ensemble I; si on pose $y_k = x_{\varphi(k)}$, la famille $(y_k)_{k \in K}$ est sommable et a même somme que $(x_i)$. En effet, si $s = \sum_{i \in I} x_i$, et si $\sum_{i \in J} x_i \in s + V$ pour toute partie finie J contenant la partie finie $J_0$, on aura $\sum_{k \in L} y_k \in s + V$ pour toute partie finie L de K contenant $\varphi^{-1}(J_0)$.

#### Remarque 3 {#top-iii-s5-n1-rem-3 .statement}

La déf. 1, ainsi que les conventions et remarques qui la suivent, s’appliquent, plus généralement, à toute famille de points d’un espace topologique séparé E, muni d’une loi de monoïde commutatif.

### 2. Le critère de Cauchy

Soit $(x_i)_{i \in I}$ une famille sommable dans G; pour tout voisinage V de l’origine dans G, il existe une partie finie $J_0$ de I telle que, pour toute partie finie K de I ne rencontrant pas $J_0$, on ait $s_K \in V$; en effet, $J = J_0 \cup K$ est une partie finie quelconque contenant $J_0$; soient $s = \sum_{i \in I} x_i$ et W un voisinage symétrique de 0 tel que $W + W \subset V$; d’après la déf. 1, il existe $J_0$ tel que $s_J \in s + W, s_{J_0} \in s + W$, d’où $s_K = s_J - s_{J_0} \in W + W \subset V$.

Réciproquement, supposons que la famille $(x_i)$ possède cette propriété; alors l’image, par l’application $J \mapsto s_J$, du filtre $\Phi$, est une base de filtre de Cauchy dans G; en effet, soit J une partie finie contenant $J_0$, et posons $K = J \cap \complement J_0$; on a $K \cap J_0 = \varnothing$, et $s_K = s_J - s_{J_0}$, donc $s_J \in s_{J_0} + V$; si $J'$ est une seconde partie finie contenant $J_0$, on a donc $s_J - s_{J'} \in V + V$, d’où la proposition. Par suite:

#### Théorème 1 (critère de Cauchy) {#top-iii-s5-thm-1 .statement}

Dans un groupe commutatif séparé G, pour qu’une famille $(x_i)_{i \in I}$ soit sommable, il faut que, pour tout voisinage V de l’origine, il existe une partie finie $J_0$ de I telle que, pour toute partie finie K de I ne rencontrant pas $J_0$, on ait $\sum_{i \in K} x_i \in V$. Cette condition nécessaire est aussi suffisante lorsque G est complet.

D’une manière plus imagée, on peut dire qu’en ôtant de la famille $(x_i)$ un nombre fini (assez grand) de termes, toute somme partielle finie de la sous-famille restante doit être aussi voisine que l’on veut de 0.

Une conséquence immédiate de la première partie du th. 1 est la proposition suivante:
Proposition 1. — Si la famille $(x_i)$ est sommable, tout voisinage de 0 contient tous les $x_i$, à l’exception d’une sous-famille finie (en d’autres termes, si I est infini, on a $\lim x_i = 0$ suivant le filtre des complémentaires des parties finies de I).

Cette condition nécessaire pour qu’une famille $(x_i)$ soit sommable n’est nullement suffisante en général, même lorsque G est complet; on en verra de nombreux exemples par la suite (voir IV, p. 33).

#### Corollaire 1 {#top-iii-s5-thm-1-cor-1 .statement}

Soit $(x_i)_{i \in I}$ une famille sommable dans un groupe commutatif dont l’élément neutre admet un système fondamental dénombrable de voisinages; l’ensemble des indices i tels que $x_i \neq 0$ est alors dénombrable.

En effet, soit $(V_n)$ un système fondamental dénombrable de voisinages de 0; si $H_n$ est l’ensemble des indices i tels que $x_i \notin V_n$, l’ensemble H des indices i tels que $x_i \neq 0$ est la réunion des $H_n$, et chacun des $H_n$ est fini d’après la prop. 1.

Ce corollaire n’est plus nécessairement valable lorsqu’on ne suppose pas que l’origine possède un système fondamental dénombrable de voisinages. *Considérons par exemple, le groupe produit $\mathbf{R}^\mathbf{R}$ (groupe additif des fonctions numériques finies d’une variable réelle, muni de la topologie de la convergence simple (cf. X, § 1, n° 3)) et soit $f_a$ l’élément de $\mathbf{R}^\mathbf{R}$ tel que $f_a(a) = 1, f_a(x) = 0$ pour $x \neq a$; la famille $(f_a)_{a \in \mathbf{R}}$ est sommable et a pour somme la fonction égale à 1 en tout point de $\mathbf{R}$. \* Toutefois:

#### Corollaire 2 {#top-iii-s5-thm-1-cor-2 .statement}

Soit $G$ un groupe topologique commutatif séparé et complet, tel qu’un système fondamental de voisinages de 0 soit formé de sous-groupes de $G$ (cf. III, p. 5, Exemple); pour qu’une famille $(x_i)_{i \in I}$ de points de $G$ soit sommable, il faut et il suffit que $\lim x_i = 0$ suivant le filtre des complémentaires des parties finies de $I$.

En effet, soient $V$ un voisinage de 0, $H$ un sous-groupe ouvert de $G$ contenu dans $V$; s’il existe une partie finie $J_0$ de $I$ telle que $x_i \in H$ pour tout $i \notin J_0$, on a aussi $\sum_{i \in K} x_i \in H$ pour toute partie finie $K$ de $I$ ne rencontrant pas $J_0$. Il suffit donc d’appliquer le th.1.

#### Remarque {#top-iii-s5-n2-rem-1 .statement}

Lorsque $G$ est noté multiplicativement, le critère de Cauchy s’exprime de la manière suivante: pour que la famille $(x_i)_{i \in I}$ soit multipliable, il faut que, pour tout voisinage $V$ de l’unité, il existe une partie finie $J_0$ de $I$ telle que, pour toute partie finie $K$ de $I$ ne rencontrant pas $J_0$, on ait $\prod_{i \in K} x_i \in V$; cette condition est suffisante lorsque $G$ est complet. On en déduit que, si $I$ est infini et si $(x_i)$ est multipliable, on a $\lim x_i = 1$, suivant le filtre des complémentaires des parties finies de $I$; si en outre l’unité possède un système fondamental dénombrable de voisinages, l’ensemble des indices $i$ tels que $x_i \neq 1$ est dénombrable.

### 3. Sommes partielles. Associativité

#### Proposition 2 {#top-iii-s5-prop-2 .statement}

Dans un groupe complet $G$, toute sous-famille d’une famille sommable est sommable.

En effet, le critère de Cauchy est trivialement vérifié pour une sous-famille de $(x_i)_{i \in I}$ s’il l’est pour cette famille.

Si $(x_i)_{i \in I}$ est sommable, la somme $\sum_{i \in J} x_i$ est donc définie pour toute partie (finie ou non) $J$ de $I$; on l’appelle encore somme partielle de la famille $(x_i)$, correspondant à la partie $J$ de l’ensemble d’indices. L’ensemble des sommes partielles d’une famille sommable est évidemment contenu dans l’adhérence de l’ensemble des sommes partielles finies.

#### Théorème 2 (associativité de la somme) {#top-iii-s5-thm-2 .statement}

Soit $(x_i)_{i \in I}$ une famille sommable dans un groupe complet $G$, et soit $(I_\lambda)_{\lambda \in L}$ une partition quelconque de $I$; si on pose $s_\lambda = \sum_{i \in I_\lambda} x_i$, la famille $(s_\lambda)_{\lambda \in L}$ est sommable et a même somme que la famille $(x_i)_{i \in I}$.

D’une manière plus imagée, on peut dire que, si on a une famille sommable dans un groupe complet, on peut associer arbitrairement ses termes en sous-familles et former la somme de chaque sous-famille ainsi obtenue; la famille de ces sommes partielles est encore sommable, et sa somme est égale à celle de la famille donnée.

Posons $s = \sum_{i \in I} x_i$, et soit $V$ un voisinage fermé quelconque de 0 dans $G$; il existe une partie finie $J_0$ de $I$ telle que, pour toute partie finie $J$ de $I$, contenant $J_0$, on ait $\sum_{t \in J} x_t \in s + V$. Soit $K_0$ la partie de $L$ formée des indices $\lambda$ tels que $J_\lambda = I_\lambda \cap J_0$ ne soit pas vide ; $K_0$ est évidemment finie. Soit $K$ une partie finie quelconque de $L$, contenant $K_0$; on va montrer que $\sum_{\lambda \in K} s_\lambda \in s + V$, ce qui établira le théorème. Or, $s_\lambda$ est très voisin d’une somme partielle finie de $(x_t)$, dont les indices appartiennent tous à $I_\lambda$; de façon précise, étant donné un voisinage symétrique $W$ de 0, il existe pour chaque $\lambda \in K$ une partie finie $H_\lambda$ de $I_\lambda$, contenant $J_\lambda$, et telle que $s_\lambda - \sum_{t \in H_\lambda} x_t \in W$. Posons $J = \bigcup_{\lambda \in K} H_\lambda$; $J$ est une partie finie de $I$ contenant $J_0$, et on a

$$
\sum_{t \in J} x_t = \sum_{t \in \bigcup_{\lambda \in K} H_\lambda} x_t = \sum_{\lambda \in K} \left( \sum_{t \in H_\lambda} x_t \right)
$$

d’après l’associativité de la somme finie (A, I, p. 9). En vertu du choix de $J_0$ et des $H_\lambda$, on a donc

$$
\sum_{\lambda \in K} s_\lambda \in s + V + nW
$$

où $n$ désigne le nombre d’éléments de $K$; cette relation a lieu pour tout $W$, donc on a aussi $\sum_{\lambda \in K} s_\lambda \in s + V$, puisque $V$, étant fermé, est l’intersection des voisinages $V + nW$ (III, p. 20, formule (1)).

C.Q.F.D.

On peut donc écrire la *formule d’associativité* de la somme:

(1)

$$
\sum_{\lambda \in L} \left( \sum_{t \in I_\lambda} x_t \right) = \sum_{t \in \bigcup_{\lambda \in L} I_\lambda} x_t
$$

valable lorsque la famille $(I_\lambda)$ est une *partition* de sa réunion, et que le *second* membre est défini. En particulier, si l’ensemble d’indices $I = L \times M$ est un *produit*, et si la famille « double » $(x_{\lambda \mu})_{(\lambda, \mu) \in L \times M}$ est *sommable*, on a la *formule d’échange des signes de sommation*

(2)

$$
\sum_{(\lambda, \mu) \in L \times M} x_{\lambda \mu} = \sum_{\lambda \in L} \left( \sum_{\mu \in H} x_{\lambda \mu} \right) = \sum_{\mu \in M} \left( \sum_{\lambda \in L} x_{\lambda \mu} \right).
$$

Il faut observer que le *premier membre* de (1) peut avoir un sens, sans que le second soit défini. Considérons par exemple le cas où $I = L \times \{1, 2\}$ (L infini), $I_\lambda$ étant formé des deux éléments $(\lambda, 1)$ et $(\lambda, 2)$; si on prend $x_{\lambda, 1} = a, x_{\lambda, 2} = -a$, où $a$ est un élément $\neq 0$ de $G$, toutes les sommes partielles correspondant aux $I_\lambda$ sont nulles, donc le premier membre de (1) est défini et égal à 0, tandis que le second membre de (1) n’a pas de sens, comme le montre la prop. 1 de III, p. 38.

De même, si le premier membre de (2) n’est pas défini, chacun des deux derniers membres de (2) peut avoir un sens, sans que les éléments de $G$ qu’ils représentent soient nécessairement égaux (voir IV, p. 61, exerc. 17).

D’une manière plus imagée, on peut dire que, s’il est toujours possible d'« associer » arbitrairement les termes d’une somme, on ne peut, par contre, « dissocier » en leurs éléments ceux des termes d’une somme qui se présentent eux-mêmes comme des sommes. Cette opération est toutefois légitime lorsque ces termes « dissociables » sont en nombre fini. En effet:

#### Proposition 3 {#top-iii-s5-prop-3 .statement}

*Soit* $(x_i)_{i \in I}$ *une famille de points d’un groupe* $G$, *et* $(I_\lambda)_{\lambda \in L}$ *une partition finie de* $I$; *si chacune des sous-familles* $(x_i)_{i \in I_\lambda}$ *est sommable, la famille* $(x_i)_{i \in I}$ *est sommable, et on a la formule* (1).

Il suffit de la démontrer lorsque $L = \{1, 2\}$; on procédera ensuite par récurrence sur le nombre d’éléments de $L$. Posons $s_1 = \sum_{i \in I_1} x_i$, $s_2 = \sum_{i \in I_2} x_i$; pour tout voisinage $V$ de l’origine, il existe une partie finie $J_1$ (resp. $J_2$) de $I_1$ (resp. $I_2$) telle que pour toute partie finie $H_1$ (resp. $H_2$) de $I_1$ (resp. $I_2$) contenant $J_1$ (resp. $J_2$), on ait $\sum_{i \in H_1} x_i \in s_1 + V$ (resp. $\sum_{i \in H_2} x_i \in s_2 + V$). Si on pose $J_0 = J_1 \cup J_2$, on en déduit que, pour toute partie finie $H$ de $I$, contenant $J_0$, on a $\sum_{i \in H} x_i \in s_1 + s_2 + V + V$, d’où la proposition.

### 4. Familles sommables dans un produit de groupes

#### Proposition 4 {#top-iii-s5-prop-4 .statement}

*Soit* $G = \prod_{\lambda \in L} G_\lambda$ *un produit d’une famille de groupes commutatifs séparés.* *Pour qu’une famille* $(x_i)_{i \in I}$ *de points de* $G$ *soit sommable, il faut et il suffit que, pour tout* $\lambda \in L$, *la famille* $(\mathrm{pr}_\lambda x_i)_{i \in I}$ *soit sommable; si* $s_\lambda$ *est sa somme, $s = (s_\lambda)$ est la somme de la famille* $(x_i)$.

Cela résulte aussitôt de la condition de convergence, suivant un filtre, d’une fonction prenant ses valeurs dans un espace produit (I, p. 51, cor. 1); on a en effet, pour toute partie finie $J$ de $I$, $\mathrm{pr}_\lambda (\sum_{i \in J} x_i) = \sum_{i \in J} \mathrm{pr}_\lambda x_i$.

### 5. Image d’une famille sommable par un homomorphisme continu

#### Proposition 5 {#top-iii-s5-prop-5 .statement}

*Soit* $f$ *un homomorphisme continu d’un groupe commutatif* $G$ *dans un groupe commutatif* $G'$.* *Si* $(x_i)$ *est une famille sommable dans* $G$, *($f(x_i)$) est une famille sommable dans* $G'$, *et on a*

(3)
$$
\sum f(x_i) = f(\sum x_i).
$$

Pour toute partie finie $J$ de l’ensemble d’indices, on a en effet
$$
f(\sum_{i \in J} x_i) = \sum_{i \in J} f(x_i),
$$
et l’image par $f$ d’une base de filtre convergente est une base de filtre convergente (I, p. 50, cor. 1).

#### Proposition 6 {#top-iii-s5-prop-6 .statement}

Soient $(x_i), (y_i)$ deux familles sommables dans un groupe $G$, correspondant au même ensemble d’indices ; les familles $(-x_i), (nx_i)$ ($n \in \mathbf{Z}$), $(x_i + y_i)$ sont sommables, et on a

(4) $$
\sum (-x_i) = -\sum x_i
$$
(5) $$
\sum (nx_i) = n \sum x_i
$$
(6) $$
\sum (x_i + y_i) = \sum x_i + \sum y_i.
$$

En effet, $x \mapsto -x$ et $x \mapsto nx$ sont des homomorphismes continus de $G$ dans $G$ ; d’autre part, si $(x_i)$ et $(y_i)$ sont sommables, la famille $((x_i, y_i))$ est sommable dans $G \times G$, et comme $(x, y) \mapsto x + y$ est un homomorphisme continu de $G \times G$ dans $G$, on en déduit (6).

#### Remarque {#top-iii-s5-n5-rem-1 .statement}

Les prop. 4 et 5 s’appliquent encore au cas, signalé plus haut, des familles sommables dans un espace topologique $E$ muni d’une loi de monoïde commutatif il en est de même de la prop. 3 (III, p. 41) et de la formule (6) si on suppose en outre que l’application $(x, y) \mapsto x + y$ est continue dans $E \times E$.

### 6. Séries

Dans un groupe topologique commutatif séparé $G$, noté additivement, considérons une suite de points $(x_n)_{n \in \mathbf{N}}$, et faisons-lui correspondre la suite des sommes partielles $s_n = \sum_{p=0}^n x_p$ ($n \in \mathbf{N}$) ; l’application $(x_n) \mapsto (s_n)$ est une application bijective de l’ensemble $G^\mathbf{N}$ des suites $(x_n)$ de points de $G$, sur lui-même ; car, si la suite $(s_n)$ est donnée, la suite $(x_n)$ est déterminée par les relations $x_0 = s_0,\ x_n = s_n - s_{n-1}$ ($n \geqslant 1$).

On appelle série définie par la suite $(x_n)$, ou série de terme général $x_n$ (ou simplement série $(x_n)$, par abus de langage, s’il ne risque pas d’y avoir de confusion), le couple des suites $(x_n)$ et $(s_n)$ ainsi associées. La série définie par la suite $(x_n)$ est dite convergente si la suite $(s_n)$ est convergente ; la limite de cette suite est appelée la somme de la série et se note $\sum_{n=0}^\infty x_n$ (ou $\sum_{n=0}^\infty x_n$ par abus de notation).

Si la série de terme général $x_n$ est convergente, on se permettra parfois, par abus de langage, de l’appeler « la série $\sum_{n=0}^\infty x_n$ », ou encore « la série $x_0 + x_1 + \cdots + x_n + \cdots$ ».

Une condition nécessaire pour la convergence de la série de terme général $x_n$, est que la suite $(s_n)$ soit une suite de Cauchy, c’est-à-dire que, pour tout voisinage $V$ de l’origine dans $G$, il existe un entier $n_0$ tel que, pour tout couple d’entiers $n \geqslant n_0,\ p > 0$, on ait

$$
s_{n+p} - s_n = \sum_{i=n+1}^{n+p} x_i \in V.
$$

Si G est complet, cette condition est aussi suffisante (critère de Cauchy pour les séries).

Si la série de terme général $x_n$ est convergente, on a en particulier $\lim_{n \to \infty} x_n = \lim_{n \to \infty} (s_n - s_{n-1}) = 0$; mais cette condition nécessaire de convergence n’est nullement suffisante en général, même lorsque G est complet (voir IV, p. 33).

#### Proposition 7 {#top-iii-s5-prop-7 .statement}

Si les séries définies par les suites $(x_n)$ et $(y_n)$ sont convergentes, il en est de même des séries définies par les suites $(-x_n)$ et $(x_n + y_n)$, et on a

$$
\sum_{n=0}^{\infty} (-x_n) = - \sum_{n=0}^{\infty} x_n
$$

$$
\sum_{n=0}^{\infty} (x_n + y_n) = \sum_{n=0}^{\infty} x_n + \sum_{n=0}^{\infty} y_n.
$$

C’est une conséquence évidente de la continuité de $-x$ dans G, et de $x + y$ dans $G \times G$.

#### Corollaire {#top-iii-s5-n6-cor-1 .statement}

Si $(x_n), (y_n)$ sont deux suites de points de G telles que $x_n = y_n$ sauf pour un nombre fini d’indices, et si la série de terme général $x_n$ converge, il en est de même de la série de terme général $y_n$.

En effet, la série de terme général $x_n - y_n$ a tous ses termes nuls à partir d’un certain rang.

On exprime encore ce corollaire en disant qu’on peut modifier arbitrairement un nombre fini de termes d’une série convergente sans qu’elle cesse d’être convergente.

En particulier, si $y_n = 0$ pour $n < m, y_n = x_n$ pour $n \geq m$, la série de terme général $y_n$ converge en même temps que la série de terme général $x_n$; sa somme se note $\sum_{n=m}^{\infty} x_n$ et s’appelle le reste d’indice m de la série $(x_n)$; comme $\sum_{n=m}^{\infty} x_n = \sum_{n=0}^{\infty} x_n - s_{m-1}$, le reste d’indice m d’une série convergente tend vers 0 lorsque m augmente indéfiniment.

Si une suite $(x_n)_{n \in I}$ a pour ensemble d’indices une partie infinie I de $\mathbf{N}$, et si $\varphi$ désigne l’application bijective strictement croissante de $\mathbf{N}$ sur I, on appelle encore, par abus de language, série définie par la suite $(x_n)_{n \in I}$, la série définie par la suite $(x_{\varphi(n)})_{n \in \mathbf{N}}$; si elle est convergente, sa somme se note $\sum_{n \in I}^{\infty} x_n$. On vérifie immédiatement que cette série converge en même temps que la série de terme général $z_n$, où on pose $z_n = x_n$ si $n \in I, z_n = 0$ si $n \in \mathbf{C}I$.

Il importe de remarquer que, si la série définie par une suite $(x_n)_{n \in \mathbf{N}}$ est convergente, il peut exister des parties infinies I de $\mathbf{N}$ telles que la série définie par la suite partielle $(x_n)_{n \in I}$ ne soit pas convergente (voir III, p. 79, exerc. 5, et IV, p. 38, Exemples).

Les prop. 4 et 5 s’étendent de même aux séries; nous laissons au lecteur le soin de les énoncer.

#### Proposition 8 (associativité restreinte des séries) {#top-iii-s5-prop-8 .statement}

Soit $(k_n)$ une suite strictement croissante d’entiers $\geq 0$ avec $k_0 = 0$; si la série de terme général $x_n$ converge, et si on pose

$$
u_n = \sum_{p=k_{n-1}}^{k_n-1} x_p, \text{ la série de terme général } u_n \text{ est convergente, et on a } \sum_{n=1}^{\infty} u_n = \sum_{n=0}^{\infty} x_n.
$$

En effet, la suite des sommes partielles de la série $(u_n)$ n’est autre que la suite $(s_{k_n-1})$ *extraite* de la suite $(s_n)$ des sommes partielles de la série $(x_n)$.

### 7. Séries commutativement convergentes

Soient $(x_n)$ une suite *sommable* dans $G$, $s = \sum_{n \in \mathbf{N}} x_n$ sa somme. Pour tout voisinage $V$ de $s$, il existe $J_0 \in \mathcal{F}(\mathbf{N})$ telle que l’on ait $s_J \in s + V$ pour $J \in \mathcal{F}(\mathbf{N})$ et $J_0 \subset J$; soit $m$ le plus grand entier dans $J_0$; pour $n \geq m$, on a donc $s_n \in s + V$, ce qui montre que *la série* $(x_n)$ est *convergente* et a pour somme $s$. Mais la réciproque est *inexacte*: la suite des termes d’une série convergente peut fort bien ne pas être sommable (voir IV, p. 38).

En outre, la structure d’*ordre* de $\mathbf{N}$ intervient de façon essentielle dans la définition d’une série convergente; si la série $(x_n)$ est convergente, et si $\sigma$ est une *permutation* de $\mathbf{N}$, la série $(x_{\sigma(n)})$ n’est pas nécessairement convergente (cf. IV, p. 60, exerc. 15).

#### Définition 2 {#top-iii-s5-def-2 .statement}

*On dit qu’une série définie par une suite* $(x_n)$ *est commutativement convergente si, pour toute permutation* $\sigma$ *de* $\mathbf{N}$, *la série définie par la suite* $(x_{\sigma(n)})$ *est convergente*.

#### Proposition 9 {#top-iii-s5-prop-9 .statement}

*Pour que la série définie par la suite* $(x_n)$ *soit commutativement convergente, il faut et il suffit que la suite* $(x_n)$ *soit sommable; pour toute permutation* $\sigma$ *de* $\mathbf{N}$, *on a alors*

$$
\sum_{n=0}^{\infty} x_{\sigma(n)} = \sum_{n \in \mathbf{N}} x_n.
$$

La condition est évidemment suffisante. Pour voir qu’elle est nécessaire, raisonnons par l’absurde, en supposant la série $(x_n)$ commutativement convergente, mais la suite $(x_n)$ non sommable. L’image par l’application $H \mapsto s_H$ du filtre $\Phi$ ne peut alors être la base d’un filtre de Cauchy dans $G$, sans quoi ce filtre, qui a un point adhérent par hypothèse, convergerait (II, p. 14, cor. 2 de la prop. 5). Il existe donc un voisinage $V$ de $0$ tel que, pour toute partie finie $J$ de $\mathbf{N}$, il existe une partie finie $H$ de $\mathbf{N}$ ne rencontrant pas $J$ et telle que $\sum_{n \in H} x_n \notin V$. On peut alors définir, par récurrence, une *partition* de $\mathbf{N}$ en sous-ensembles *finis* $H_k$ ($k \in \mathbf{N}$) telle que $\sum_{n \in H_k} x_n \notin V$ pour une infinité d’indices $k$. Il est clair qu’il existe une permutation $\sigma$ de $\mathbf{N}$ telle que, pour tout $k$, les valeurs de $n$ telles que $\sigma(n) \in H_k$ soient consécutives. Pour une telle permutation, la série de terme général $x_{\sigma(n)}$ ne saurait être convergente, d’où la contradiction annoncée.

#### Remarque {#top-iii-s5-n7-rem-1 .statement}

Soit $G$ un groupe topologique séparé et complet, tel qu’un système fondamental de voisinages de 0 soit formé de sous-groupes de G (cf. III, p. 5, Exemple); alors, pour toute suite $(x_n)$ de points de G telle que $\lim_{n \to \infty} x_n = 0$, la série définie par la suite $(x_n)$ est *commutativement convergente*, en vertu de la prop. 9 et de III, p. 39, cor. 2.

Si le groupe G est noté *multiplicativement*, on appelle *produit infini défini par une suite* $(x_n)$ de points de G (ou *produit infini de facteur général* $x_n$, ou même *produit* $(x_n)$ si aucune confusion n’est possible) le couple formé de la suite $(x_n)$ et de la suite des produits partiels $p_n = \prod_{k=0}^n x_k$; le produit infini est dit *convergent* si la suite $(p_n)$ converge, et la limite de cette suite se note $\prod_{n=0}^\infty x_n$ (ou $\prod_{n=0}^\infty x_n$ par abus de notation). Nous laissons au lecteur le soin de traduire en notation multiplicative les propriétés des séries que nous venons d’établir.

## EXERCICES {#top-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
