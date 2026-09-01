---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 2
section_title: Produits infinis dans les algèbres normées
appendix: true
lang: fr
source: top-v-x-fr
book_pages: TG IX.125-TG IX.126
pdf_pages: 0198-0204, 0245-0246
extraction: ocr
subsections:
    - "no": 1
      title: Suites multipliables dans une algèbre normée
      page: 0
      pdf_page: 198
    - "no": 2
      title: Critères de multipliabilité
      page: 79
      pdf_page: 199
    - "no": 3
      title: Produits infinis
      page: 82
      pdf_page: 202
statements: 16
exercises: 8
content_sha256: 08e13ee94a1406e81b201e3c665c3629632ff1cabff45c15f5a1c0046f18485c
---

## APPENDICE 2

# PRODUITS INFINIS DANS LES ALGÈBRES NORMÉES

### 1. Suites multipliables dans une algèbre normée

Soit $A$ une algèbre normée sur un corps valué commutatif non discret (IX, p. 37, déf. 9); nous désignerons par $\|x\|$ la norme d’un élément $x \in A$, nous supposerons en outre que $A$ admet un élément unité $e$.

Soit $(x_n)_{n \geq N}$ une suite infinie de points de $A$; toute partie finie $J$ de $\mathbf{N}$, totalement ordonnée par l’ordre de $\mathbf{N}$, définit une séquence (A, I, p. 3) $(x_n)_{n \in J}$ de points de $A$; on a défini en Algèbre (A, I, p. 3) le produit $p_J = \prod_{n \in J} x_n$ de cette séquence, que nous appellerons produit partiel fini de la suite $(x_n)_{n \in \mathbf{N}}$, correspondant à la partie finie $J$ de $\mathbf{N}$ (on rappelle que, pour $J = \varnothing$, on pose $\prod_{n \in \varnothing} x_n = e$).

#### Définition 1 {#top-ix-a2-def-1 .statement}

On dit que la suite $(x_n)_{n \geq N}$ est multipliable dans l’algèbre normée $A$ si l’application $J \mapsto p_J$ a une limite suivant le filtre des sections de l’ensemble $\mathcal{F}(\mathbf{N})$ des parties finies de $\mathbf{N}$, ordonné par la relation $\subset$; cette limite est appelée le produit de la suite $(x_n)_{n \in \mathbf{N}}$, et noté $\prod_{n \in \mathbf{N}} x_n$ (ou simplement $\prod_n x_n$); les $x_n$ sont appelés les facteurs de ce produit.

La déf. 1 équivaut à la suivante: la suite $(x_n)$ est multipliable et a pour produit $p$ si, pour tout $\varepsilon > 0$, il existe une partie finie $J_0$ de $\mathbf{N}$ telle que, pour toute partie finie $J \supset J_0$ de $\mathbf{N}$, on ait $\|p_J - p\| \leq \varepsilon$.

#### Remarque 1 {#top-ix-a2-n1-rem-1 .statement}

Lorsque $A$ est une algèbre commutative, la déf. 1 est identique à celle qui a été donnée dans III, p. 37 (Remarque 3); mais lorsque $A$ n’est pas commutative, la structure d’ordre de l’ensemble d’indices $\mathbf{N}$ intervient de façon essentielle dans la déf. 1 ; si $\sigma$ est une permutation quelconque de $\mathbf{N}$, rien ne permet d’affirmer en général que la suite $(\mathbf{x}_{\sigma(n)})$ soit multipliable lorsque la suite $(\mathbf{x}_n)$ l’est ; en outre, lorsque ces deux suites sont multipliables, leurs produits sont en général différents.

#### Remarque 2 {#top-ix-a2-n1-rem-2 .statement}

La déf. 1 se généralise immédiatement au cas d’une famille $(\mathbf{x}_n)_{n \in I}$ dont l’ensemble d’indices $I$ est une partie de $\mathbf{Z}$ (totalement ordonnée par l’ordre induit par celui de $\mathbf{Z}$) ; nous laissons au lecteur le soin d’étendre à ce cas les propriétés qui suivent (cf. IX, p. 125, exerc. 1 et 2).

### 2. Critères de multipliabilité

Nous allons nous borner désormais au cas où l’algèbre normée $A$ est complète.

#### Théorème 1 {#top-ix-a2-thm-1 .statement}

Soit $(\mathbf{x}_n)_{n \in \mathbf{N}}$ une suite de points d’une algèbre normée complète $A$.

a) Si $(\mathbf{x}_n)$ est multipliable et a pour produit un élément inversible de $A$, pour tout $\varepsilon > 0$, il existe une partie finie $J_0$ de $\mathbf{N}$ telle que, pour toute partie finie $L$ de $\mathbf{N}$ ne rencontrant pas $J_0$, on ait $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon$.

b) Inversement, si la suite $(\mathbf{x}_n)$ satisfait à cette condition, elle est multipliable. En outre, si chacun des $\mathbf{x}_n$ est inversible, $\prod_{n \in \mathbf{N}} \mathbf{x}_n$ est inversible.

a) Soit $\mathbf{p}$ le produit de la suite multipliable $(\mathbf{x}_n)$, et supposons $\mathbf{p}$ inversible dans $A$; alors (IX, p. 40, prop. 14), il existe $\alpha > 0$ et $a > 0$ tels que, pour tout $y \in A$ tel que $\| y - \mathbf{p} \| \leq \alpha$, $y$ soit inversible, et $\| y^{-1} \| \leq a$. Par hypothèse, pour tout $\varepsilon$ tel que $0 < \varepsilon < \alpha$, il existe une partie finie $H_0$ de $\mathbf{N}$ telle que, pour toute partie finie $H$ de $\mathbf{N}$ contenant $H_0$, on ait $\| \mathbf{p}_H - \mathbf{p} \| \leq \varepsilon$. Soit $J_0 = \{0, m\}$ un intervalle de $\mathbf{N}$ contenant $H_0$; pour toute partie finie $L$ de $\mathbf{N}$ ne rencontrant pas $J_0$ les entiers appartenant à $L$ sont tous supérieurs à ceux appartenant à $H_0$; donc, si on pose $H = H_0 \cup L$, on a $\mathbf{p}_H = \mathbf{p}_{H_0} \mathbf{p}_L$. Or, comme $\| \mathbf{p}_{H_0} - \mathbf{p} \| \leq \varepsilon \leq \alpha$, $\mathbf{p}_{H_0}$ est inversible, et on a $\| \mathbf{e} - \mathbf{p}_{H_0}^{-1} \mathbf{p} \| \leq \varepsilon \| \mathbf{p}_{H_0}^{-1} \| \leq a \varepsilon$; de la relation $\| \mathbf{p}_{H_0} \mathbf{p}_L - \mathbf{p} \| \leq \varepsilon$, on tire $\| \mathbf{p}_L - \mathbf{p}_{H_0}^{-1} \mathbf{p} \| \leq \varepsilon \| \mathbf{p}_{H_0}^{-1} \| \leq a \varepsilon$ et finalement $\| \mathbf{e} - \mathbf{p}_L \| \leq 2a \varepsilon$.

b) Supposons que, pour tout $\varepsilon > 0$, il existe une partie finie $J_0$ de $\mathbf{N}$ telle que, pour toute partie finie $L$ de $\mathbf{N}$ ne rencontrant pas $J_0$, on ait $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon$. Soit $H_0 = \{0, p\}$ un intervalle de $\mathbf{N}$ contenant $J_0$; toute partie finie $H$ de $\mathbf{N}$ contenant $H_0$ peut s’écrire $H_0 \cup L$, où les entiers appartenant à $L$ sont supérieurs à ceux appartenant à $H_0$; on a donc $\mathbf{p}_H = \mathbf{p}_{H_0} \mathbf{p}_L$, et comme $L$ ne rencontre pas $J_0$, $\| \mathbf{p}_H - \mathbf{p}_{H_0} \| \leq \varepsilon \| \mathbf{p}_{H_0} \|$, et par suite $\| \mathbf{p}_H \| \leq (1 + \varepsilon) \| \mathbf{p}_{H_0} \|$. Si $\mathbf{p}_{H_0} = 0$, la suite $(\mathbf{x}_n)$ est évidemment multipliable et a pour produit 0 ; en écartant ce cas trivial, il existe un intervalle $H_1 = \{0, q\}$, contenant $H_0$ et tel que, pour toute partie finie $L$ de $\mathbf{N}$ ne rencontrant pas $H_1$, on ait $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon (\| \mathbf{p}_{H_0} \|)^{-1}$. On en déduit comme ci-dessus que, pour toute partie finie $H \supset H_1$

$$
\| \mathbf{p}_H - \mathbf{p}_{H_1} \| \leq (\| \mathbf{p}_{H_0} \|)^{-1} \| \mathbf{p}_{H_1} \| \varepsilon \leq \varepsilon (1 + \varepsilon).
$$

Le critère de Cauchy montre donc que $J \mapsto \mathbf{p}_J$ a une limite dans $A$ suivant l’ensemble filtrant $\mathcal{F}(\mathbf{N})$.

Si tous les $x_n$ sont inversibles, il en est de même de tous les produits partiels finis $p_J$; pour toute partie finie $H$ contenant $H_0$, on peut donc écrire

$$
\| e - p_{H_0}^{-1} p_H \| \leq \varepsilon;
$$

cela montre que, dans le groupe multiplicatif $G$ des éléments inversibles de $A$, l’image par l’application $J \mapsto p_J$ du filtre des sections de $\mathfrak{F}(N)$ est une base de filtre de Cauchy pour la structure uniforme gauche du groupe $G$; mais comme $G$ est complet ($IX$, p. 40, prop. 14), la limite de l’application $J \mapsto p_J$ appartient à $G$.

#### Remarque {#top-ix-a2-n2-rem-1 .statement}

Lorsque $(x_n)$ est multipliable et a un produit non inversible, la condition du th. 1 n’est plus nécessairement vérifiée; par exemple, si tous les $x_n$ sont égaux à un même élément $x$ tel que $\| x \| < 1$, la suite $(x_n)$ est multipliable et a pour produit 0, et pour toute partie finie non vide $H$ de $N$, on a $\| p_H \| \leq \| x \| < 1 \leq \| e \|$.

#### Corollaire 1 {#top-ix-a2-thm-1-cor-1 .statement}

*Si* $(x_n)$ *est une suite multipliable dont le produit est inversible dans* $A$, $\lim_{n \to \infty} x_n = e$.

#### Corollaire 2 {#top-ix-a2-thm-1-cor-2 .statement}

*Si* $(x_n)$ *est une suite multipliable dont le produit est inversible dans* $A$, *toute suite* $(x_{n_k})_{k \in \mathbf{N}}$ *extraite de* $(x_n)$ *(($n_k$) étant une suite strictement croissante d’entiers) est multipliable*.

C’est ce que montre aussitôt le critère du th. 1 ($IX$, p. 79).

#### Théorème 2 {#top-ix-a2-thm-2 .statement}

*Soit* $A$ *une algèbre normée complète; si* $(u_n)$ *est une série absolument convergente de points de* $A$, *la suite* $(e + u_n)$ *est multipliable dans* $A$; *en outre, si tous les éléments* $e + u_n$ *sont inversibles dans* $A$, *il en est de même de* $\prod_{n \in \mathbf{N}} (e + u_n)$.

Appliquons le critère de $IX$, p. 79, th. 1; pour toute partie finie $L$ de $N$, on a $p_L = e - \prod_{n \in L} (e + u_n) - e = \sum_M \left( \prod_{n \in M} u_n \right)$, $M$ parcourant l’ensemble des parties non vides de $L$ (totalement ordonnées par l’ordre induit). Comme $\left| \prod_{n \in M} u_n \right| \leq \prod_{n \in M} \| u_n \|$, on peut écrire

$$
\| p_L - e \| \leq \sum_M \left( \prod_{n \in M} \| u_n \| \right) = \prod_{n \in L} (1 + \| u_n \|) - 1.
$$

Or, comme la série de terme général $\| u_n \|$ est convergente par hypothèse, la suite $(1 + \| u_n \|)$ est multipliable dans $\mathbf{R}_+^*$ ($IV$, p. 35, th. 4); pour tout $\varepsilon > 0$, il existe donc une partie finie $J_0$ de $N$ telle que, pour toute partie finie $L$ de $N$ ne rencontrant pas $J_0$, on ait $\left| \prod_{n \in L} (1 + \| u_n \|) - 1 \right| \leq \varepsilon$; d’où le théorème.

#### Corollaire {#top-ix-a2-n2-cor-1 .statement}

*Si la série de terme générale* $u_n$ *est absolument convergente, et si aucun des éléments* $e + u_n$ *n’est diviseur de 0 dans* $A$, *le produit* $\prod_{n \in \mathbf{N}} (e + u_n)$ *n’est pas diviseur de 0 dans* $A$.

En effet, il n’y a qu’un nombre fini d’entiers $n$ tels que $\|u_n\| > 1$. Soit $J = \{0, m\}$ un intervalle de $\mathbf{N}$ contenant tous ces entiers. Le produit de la suite $(\mathbf{e} + u_n)$ est produit de $p_J$ et de l’élément $\prod_{n > m} (\mathbf{e} + u_n)$, dont tous les facteurs sont inversibles (IX, p. 39, corollaire), et qui est par suite inversible lui-même; comme $p_J$ est produit d’un nombre fini d’éléments non diviseurs de 0, il n’est pas diviseur de 0, et il en est de même de $\prod_{n \in \mathbf{N}} (\mathbf{e} + u_n)$.

La condition *suffisante* de multipliabilité donnée dans le th. 2 n’est pas nécessaire en général (cf. IX, p. 126, exerc. 6). Elle l’est toutefois dans le cas important où $A$ est une algèbre de rang *fini* sur le corps $\mathbf{R}$ (en particulier lorsque $A$ est le corps des quaternions $\mathbf{K}$, ou une algèbre de matrices $\mathbf{M}_n(\mathbf{R})$):

#### Proposition 1 {#top-ix-a2-prop-1 .statement}

*Soit $A$ une algèbre normée de rang fini sur $\mathbf{R}$. Si $(\mathbf{e} + u_n)$ est une suite multipliable dans $A$, dont le produit est inversible, la série de terme générale $u_n$ est absolument convergente.*

On sait (VII, p. 16, prop. 2) qu’il existe un nombre $c > 0$ tel que, pour toute famille finie $(\mathbf{x}_i)_{i \in I}$ de points de $A$, on ait

(1)
$$
\sum_{i \in I} \|\mathbf{x}_i\| \leq c \cdot \sup_{J \subset I} \left\| \sum_{i \in J} \mathbf{x}_i \right\|.
$$

Soit $(a_n)_{n \in \mathbf{N}}$ une suite quelconque d’éléments de $A$. Pour toute partie finie $I$ de $\mathbf{N}$, posons
$$
p_I = \prod_{i \in I} (\mathbf{e} + a_i) \qquad s_I = \sum_{i \in I} a_i, \qquad \sigma_I = \sum_{i \in I} \|a_i\|.
$$

#### Lemme 1 {#top-ix-a2-lem-1 .statement}

*Pour toute partie finie $I$ de $\mathbf{N}$, soit $\varphi(I) = \sup_{J \subset I} \|p_J - \mathbf{e}\|.$ Pour toute partie $J$ de $I$, on a*
$$
\|p_J - \mathbf{e} - s_J\| \leq \varphi(I) \sigma_J.
$$
Le lemme est évident si $J$ est vide; démontrons-le par récurrence sur le nombre d’éléments de $J$. Soit $J = K \cup \{j\}$, où $j$ est strictement supérieur à tous les éléments de $K$; alors $p_J = p_K(\mathbf{e} + a_j)$ et $s_J = s_K + a_j$, d’où
$$
p_J - \mathbf{e} - s_J = (p_K - \mathbf{e} - s_K) + (p_K - \mathbf{e}) a_j
$$
et, en vertu de l’hypothèse de récurrence et de la définition de $\varphi(I)$
$$
\|p_J - \mathbf{e} - s_J\| \leq \varphi(I) \sigma_K + \varphi(I) \|a_j\| = \varphi(I) \sigma_J
$$
ce qui démontre le lemme.

#### Lemme 2 {#top-ix-a2-lem-2 .statement}

*Si $I$ est une partie finie de $\mathbf{N}$ telle que $\varphi(I) < 1/c$, on a $\sigma_I \leq \frac{c \varphi(I)}{1 - c \varphi(I)}$*.

En effet, comme $\sigma_J \leq \sigma_I$ pour toute partie $J$ de $I$, on a, après (2),
$$
\|s_J\| \leq \varphi(I) \sigma_I + \|p_J - \mathbf{e}\| \leq (1 + \sigma_I) \varphi(I);
$$

comme, en vertu de (1), on a $\sigma_I \leq c \cdot \sup_{J \subset I} \| s_J \|$, on en déduit $\sigma_I \leq c \varphi(I)(1 + \sigma_I)$, d’où le lemme.

Cela étant, soit $(e + u_n)$ une suite multipliable dans $A$, dont le produit est inversible; d’après le th. 1 (IX, p. 79), il existe une partie finie $J_0$ de $\mathbf{N}$ telle que, pour toute partie finie $H$ de $\mathbf{N}$ ne rencontrant pas $J_0$, on ait
$$
\left\| \prod_{i \in H} (e + u_i) - e \right\| \leq 1/2c.
$$
D’après le lemme 2, on ne déduit $\sum_{i \in H} \| u_i \| \leq 1$ pour toute partie finie $H$ de $\mathbf{N}$ ne rencontrant pas $J_0$, ce qui entraîne que la famille $(\| u_n \|)$ est sommable dans $\mathbf{R}$ (IV, p. 32, th. 1).

### 3. Produits infinis

A toute suite $(x_n)$ de points d’une algèbre normée $A$, faisons correspondre la suite des *produits partiels* $p_n = \prod_{k=0}^n x_k$; on appelle *produit infini* de facteur général $x_n$, le *couple* des suites $(x_n)$ et $(p_n)$. Le produit infini de facteur général $x_n$ est dit *convergent* si la suite $(p_n)$ est convergente dans $A$; la limite de cette suite s’appelle alors le *produit* de la suite $(x_n)$, et se note $\prod_{n=0}^\infty x_n$.

#### Proposition 2 {#top-ix-a2-prop-2 .statement}

*Soit $(x_n)$ une suite de points d’une algèbre normée complète $A$.*

a) *Si le produit infini de facteur général $x_n$ est convergent et si $\prod_{n=0}^\infty x_n$ est inversible, pour tout $\varepsilon > 0$, il existe $n_0$ tel que, pour $n_0 \leq m \leq n$, on ait* $\left\| \prod_{k=m}^n x_k - e \right\| \leq \varepsilon$.

b) *Inversement, si la suite $(x_n)$ satisfait à cette condition, le produit infini de facteur général $x_n$ est convergent; en outre, si chacun des $x_n$ est inversible, $\prod_{n=0}^\infty x_n$ est inversible.*

Nous laissons au lecteur le développement de la démonstration de cette proposition, qui est calquée pas à pas sur celle du th. 1 de IX, p. 79 (les parties finies $L$ de $\mathbf{N}$ qui figurent dans cette dernière devant simplement être remplacées par des intervalles).

#### Corollaire 1 {#top-ix-a2-prop-2-cor-1 .statement}

*Si le produit infini de facteur général $x_n$ est convergent, et si $\prod_{n=0}^\infty x_n$ est inversible, $\lim_{n \to \infty} x_n = e$.*

#### Corollaire 2 {#top-ix-a2-prop-2-cor-2 .statement}

*Si le produit infini de facteur général $x_n$ est convergent, et si $\prod_{n=0}^\infty x_n$ est inversible, le produit infini de facteur général $y_n = x_{n+h} (n \geq 0)$ est convergent.*

Le produit de la suite $(y_n)$ se note $\prod_{n=h}^\infty x_n$, et s’appelle encore le *reste d’indice h* du produit infini de facteur général $x_n$.

En supposant toujours que $\prod_{n=0}^{\infty} x_n$ est inversible, on déduit encore de la prop. 2 (IX, p. 82) que, si $(z_n)$ est une suite telle que $z_n = x_n$ sauf pour un nombre fini d’indices, le produit de facteur général $z_n$ est convergent.

#### Proposition 3 {#top-ix-a2-prop-3 .statement}

*Soit* $(k_n)$ *une suite strictement croissante d’entiers* $\geqslant 0$ ($k_0 = 0$) : *si le produit infini de facteur général* $x_n$ *converge, et si on pose* $u_n = \prod_{p=k_n}^{k_{n+1}-1} x_n$, *le produit infini de facteur général* $u_n$ *est convergent, et on a* $\prod_{n=0}^{\infty} u_n = \prod_{n=0}^{\infty} x_n$.

En effet, la suite des produits partiels de la suite $(u_n)$ est extraite de la suite des produits partiels de la suite $(x_n)$.

Enfin, par le même raisonnement que pour les groupes commutatifs (III, p. 44), on voit que si, dans une algèbre normée $A$, une suite $(x_n)$ est *multipliable*, le produit de facteur général $x_n$ est convergent, et on a $\prod_{n=0}^{\infty} x_n = \prod_{n \in \mathbf{N}} x_n$ (qu’on écrit aussi $\prod_{n=0}^{\infty} x_n$); la réciproque est bien entendu inexacte (cf. IX, p. 126, exerc. 7).

Exercises

## EXERCICES {#top-ix-a2-exercises}

See the [exercises for Appendix 2](exercises/a2/).
