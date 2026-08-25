---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: Espaces vectoriels topologiques sur un corps valué
section: 1
section_title: Espaces vectoriels topologiques
lang: fr
source: evt-i-v-fr
pdf_pages: 0007-0017, 0028-0031
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’un espace vectoriel topologique
      page: 0
      pdf_page: 7
    - "no": 2
      title: Espaces normés sur un corps valué
      page: 3
      pdf_page: 9
    - "no": 3
      title: Sous-espaces vectoriels et espaces quotients d’un espace vectoriel topologique ; produits d’espaces vectoriels topologiques ; somme directe topologique de sous-espaces
      page: 4
      pdf_page: 10
    - "no": 4
      title: Structure uniforme et complétion d’un espace vectoriel topologique
      page: 5
      pdf_page: 11
    - "no": 5
      title: Voisinages de l’origine dans un espace vectoriel topologique sur un corps valué
      page: 6
      pdf_page: 12
    - "no": 6
      title: Critères de continuité et d’équicontinuité
      page: 8
      pdf_page: 14
    - "no": 7
      title: Topologies initiales d’espaces vectoriels
      page: 9
      pdf_page: 15
statements: 26
exercises: 14
content_sha256: 0eb670b83af5ce67de8c2fa13f552cbfd7773188b5145b333c3829c489d27fc4
---

## § 1. ESPACES VECTORIELS TOPOLOGIQUES

### 1. Définition d’un espace vectoriel topologique

#### Définition 1 {#evt-i-s1-def-1 .statement}

Étant donné un corps topologique K (TG, III, p. 54), on appelle espace vectoriel topologique à gauche sur K un ensemble E, muni :
  1° d’une structure d’espace vectoriel à gauche sur K ;
  2° d’une topologie compatible avec la structure de groupe additif de E (TG, III, p. 1),
et satisfaisant en outre à l’axiome suivant :
  (EVT) l’application $(\lambda, x) \mapsto \lambda x$ de $K \times E$ dans E est continue.

Il revient au même de dire que E est un K-module topologique à gauche (TG, III, p. 52).

Une structure d’espace vectoriel à gauche par rapport à K et une topologie étant données sur un ensemble E, on dira qu’elles sont compatibles si la topologie et la structure de groupe additif de E sont compatibles, et si en outre l’axiome (EVT) est vérifié. Il revient au même de dire que les deux applications $(x, y) \mapsto x + y$ et $(\lambda, x) \mapsto \lambda x$ de $E \times E$ et de $K \times E$ respectivement dans E sont continues, car cela entraîne la continuité de l’application $x \mapsto -x = (-1)x$, donc le fait que la topologie de E est compatible avec sa structure de groupe additif.

Si E est un espace vectoriel topologique à gauche sur K, on dit que E, muni seulement de sa structure d’espace vectoriel, est sous-jacent à l’espace vectoriel topologique E.

#### Exemple 1 {#evt-i-s1-n1-exa-1 .statement}

Si E est un espace vectoriel à gauche sur un corps topologique discret K, la topologie discrète sur E est compatible avec la structure d’espace vectoriel de E (il n’en est pas de même si K est non discret et E non réduit à 0).
  2) Soit A un anneau topologique (TG, III, p. 48) et soit K un sous-anneau de A qui est un corps, et tel que la topologie induite sur K par celle de A soit compatible avec la structure de corps de K ; alors la topologie de A est compatible avec sa structure d’espace vectoriel à gauche sur K.
  3) Soient K un corps topologique quelconque, I un ensemble quelconque. Sur l’espace vectoriel produit $K_s^I$ (A, II, p. 10), la topologie produit est compatible avec la structure d’espace vectoriel (TG, III, p. 53). On peut encore dire que l’espace $K_s^I$ des applications de I dans K, muni de la topologie de la convergence simple, est un espace vectoriel topologique sur K (TG, X, p. 4).

4) Soit X un espace topologique ; sur l’ensemble E = $\mathcal{C}(X ; \mathbf{R})$ des fonctions numériques finies continues dans X, la topologie de la convergence compacte (TG, X, p. 4) est compatible avec la structure d’espace vectoriel de E sur $\mathbf{R}$. En effet, soient $u_0$ un point de E, H une partie compacte de X, $\varepsilon$ un nombre > 0 arbitraire. La fonction numérique $u_0$ est bornée dans H ; soit $a = \sup_{t \in H} |u_0(t)|$; si $u$ est un point quelconque de E, on peut écrire, pour tout $t \in H$,

$$
|\lambda u(t) - \lambda_0 u_0(t)| \leq |\lambda| \cdot |u(t) - u_0(t)| + a \; |\lambda - \lambda_0|.
$$

Par suite, si $|\lambda - \lambda_0| \leq \varepsilon$ et si $|u(t) - u_0(t)| \leq \varepsilon$ pour tout $t \in H$, on aura, pour $t \in H$,
$$
|\lambda u(t) - \lambda_0 u_0(t)| \leq \varepsilon (\varepsilon + |\lambda_0| + a),
$$
ce qui montre que l’axiome (EVT) est vérifié ; on vérifie de même que la topologie de la convergence compacte est compatible avec la structure de groupe additif de E.

Par contre, si X n’est pas compact, la topologie de la convergence uniforme (dans X) n’est pas nécessairement compatible avec la structure d’espace vectoriel de E ; par exemple si $X = \mathbf{R}$, et si $u_0$ est une fonction continue non bornée dans $\mathbf{R}$, l’application $\lambda \mapsto \lambda u_0$ de $\mathbf{R}$ dans E n’est pas continue quand on munit E de la topologie de la convergence uniforme.

5) Soit E un espace vectoriel de dimension finie $n$ sur un corps topologique K ; il existe donc un isomorphisme $u : K_s^n \to E$ de K-espaces vectoriels, et en outre, si $v$ est un second isomorphisme de $K_s^n$ sur E, on peut écrire $v = u \circ f$, où $f$ est un automorphisme du K-espace vectoriel $K_s^n$. Considérons alors sur $K_s^n$ la topologie produit, qui est compatible avec sa structure d’espace vectoriel (Exemple 3) ; comme toute application linéaire de $K_s^n$ dans lui-même est continue pour cette topologie, tout automorphisme de l’espace vectoriel $K_s^n$ est bicontinu. Par suite, si l’on transporte à E la topologie produit de $K_s^n$ au moyen d’un isomorphisme quelconque de $K_s^n$ sur E, la topologie obtenue sur E est indépendante de l’isomorphisme considéré ; on dit que c’est la topologie canonique sur E ; nous la caractériserons autrement (I, p. 14) lorsque K est un corps valué complet non discret. Toute application linéaire de E dans un espace vectoriel topologique sur K est continue pour la topologie canonique sur E.

De la même manière que dans la déf. 1, on définit un espace vectoriel topologique à droite sur un corps topologique K ; mais tout espace vectoriel à droite sur K peut être considéré comme espace vectoriel à gauche sur le corps opposé $K^0$ de K (A, II, p. 2), et la topologie de K est compatible avec la structure de corps de $K^0$. Pour cette raison, nous ne considérerons en principe que des espaces vectoriels topologiques à gauche ; quand nous parlerons d’« espace vectoriel topologique » sans préciser, il sera sous-entendu qu’il s’agit d’un espace vectoriel à gauche.

Si K’ est un sous-corps de K, et E un espace vectoriel topologique sur K, il est clair que la topologie de E est encore compatible avec la structure d’espace vectoriel de E par rapport à K’, obtenue par restriction à K’ du corps des scalaires ; on dit que l’espace vectoriel topologique sur K’ ainsi obtenu est sous-jacent à l’espace vectoriel topologique E sur K.

Pour qu’un espace vectoriel topologique E soit séparé, il faut et il suffit que, pour tout point $x \neq 0$ de E, il existe un voisinage de 0 ne contenant pas $x$ (TG, III, p. 5).

Considérons, sur un espace vectoriel E par rapport à un corps topologique K, une topologie compatible avec la structure de groupe additif de E. En vertu de l’identité

$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0) x_0 + \lambda_0 (x - x_0) + (\lambda - \lambda_0) (x - x_0)
$$

l’axiome (EVT) est équivalent au système des trois axiomes suivants :

(EVT$_1'$) *Quel que soit* $x_0 \in E$, *l’application* $\lambda \mapsto \lambda x_0$ *est continue au point* $\lambda = 0$.
(EVT$_2'$) *Quel que soit* $\lambda_0 \in K$, *l’application* $x \mapsto \lambda_0 x$ *est continue au point* $x = 0$.
(EVT$_3'$) *L’application* $(\lambda, x) \mapsto \lambda x$ *est continue au point* $(0, 0)$.

En particulier :

#### Proposition 1 {#evt-i-s1-prop-1 .statement}

*Pour tout* $\alpha \in K$ *et tout point* $b \in E$, *l’application* $x \mapsto \alpha x + b$ *de* $E$ *dans lui-même est continue.* *En outre, si* $\alpha \neq 0$, *cette application est un homéomorphisme de* $E$ *sur lui-même*.

La seconde partie de la proposition résulte du fait que, si $\alpha \neq 0$, $x \mapsto \alpha^{-1} x - \alpha^{-1} b$ est l’application réciproque de $x \mapsto \alpha x + b$.

#### Corollaire {#evt-i-s1-n1-cor-1 .statement}

*Si* $A$ *est un ensemble ouvert* (resp. *fermé*) *dans* $E$, $\alpha A$ *est ouvert* (resp. *fermé*) *dans* $E$ *pour tout* $\alpha \neq 0$ *dans* $K$.

Soient $E$ et $F$ deux espaces vectoriels topologiques sur un même corps topologique $K$. Pour qu’une application bijective $f$ de $E$ sur $F$ soit un *isomorphisme* de l’espace vectoriel topologique $E$ sur l’espace vectoriel topologique $F$, il faut et il suffit que $f$ soit *linéaire et bicontinue*. En particulier, si $\gamma \neq 0$ appartient au *centre* de $K$, l’homothétie $x \mapsto \gamma x$ est un *automorphisme* de la structure d’espace vectoriel topologique de $E$.

### 2. Espaces normés sur un corps valué

Rappelons (TG, IX, p. 28) qu’une *valeur absolue* sur un corps $K$ est une application $\xi \mapsto |\xi|$ de $K$ dans $\mathbf{R}_+$, telle que $|\xi| = 0$ soit équivalent à $\xi = 0$, et qu’on ait $|\xi \eta| = |\xi| \cdot |\eta|$, et $|\xi + \eta| \leq |\xi| + |\eta|$; une valeur absolue définit sur $K$ une distance $|\xi - \eta|$, et par suite une topologie séparée, compatible avec la structure de corps de $K$. Si $|\xi| = 1$ pour tout $\xi \neq 0$, la valeur absolue est dite *impropre*, et la topologie qu’elle définit sur $K$ est la topologie *discrète* ; si, au contraire, il existe $\alpha \neq 0$ dans $K$ tel que $|\alpha| \neq 1$, il existe $\beta \neq 0$ dans $K$ tel que $|\beta| < 1$ (il suffit de prendre $\beta = \alpha$ ou $\beta = \alpha^{-1}$), et la suite $(\beta^n)_{n \geq 1}$ converge vers $0$, donc la topologie de $K$ n’est pas discrète.

Rappelons d’autre part (TG, IX, p. 31) que si $E$ est un espace vectoriel sur un corps valué *non discret* $K$, une *norme* sur $E$ est une application $x \mapsto \|x\|$ de $E$ dans $\mathbf{R}_+$, telle que la relation $\|x\| = 0$ soit équivalente à $x = 0$, et qu’on ait $\|\lambda x\| = |\lambda| \cdot \|x\|$ pour tout scalaire $\lambda \in K$, et $\|x + y\| \leq \|x\| + \|y\|$. Une norme définit sur $E$ une distance $\|x - y\|$, et par suite une topologie, qui est compatible avec la structure d’espace vectoriel de $E$ (*loc. cit.*). *Sauf mention expresse du contraire*, on considérera qu’un espace normé est muni de la structure d’espace vectoriel topologique définie par sa norme. Les espaces normés sont parmi les plus importants des espaces vectoriels topologiques.

On sait (TG, IX, p. 32) que deux normes distinctes sur $E$ peuvent définir la même topologie sur $E$ ; il faut et il suffit pour cela que les deux normes soient *équivalentes* (*loc. cit.*). Une structure d’espace normé est donc plus riche qu’une structure d’espace vectoriel topologique ; si E et F sont deux espaces normés, on aura soin de distinguer entre la notion d’isomorphisme de la structure d’espace normé de E sur celle de F, et la notion d’isomorphisme de la structure d’espace vectoriel topologique de E sur celle de F.

#### Exemple {#evt-i-s1-n2-exa-1 .statement}

Soit I un ensemble d’indices quelconque ; on sait (TG, X, p. 21) que sur l’ensemble $\mathcal{B}(I; K)$ des applications bornées $x = (\xi_j)$ de I dans K (qu’on note aussi $\mathcal{B}_K(I)$ ou $\ell_K^\infty(I)$), on définit une norme $\|x\| = \sup_{i \in I} |\xi_i|$. Lorsque I est un espace topologique, l’ensemble des applications bornées et continues de I dans K est un sous-espace fermé de l’espace $\mathcal{B}(I; K)$ (TG, X, p. 21, cor. 2). Un autre sous-espace de $\mathcal{B}(I; K)$ est l’ensemble $\ell_K^1(I)$ des familles $x = (\xi_i)$ absolument sommables (TG, IX, p. 36) ; on peut définir sur ce sous-espace une autre norme $\|x\|_1 = \sum_{i \in I} |\xi_i|$, qui en général n’est pas équivalente à la norme $\|x\| = \sup_{i \in I} |\xi_i|$ (I, p. 23, exerc. 6) ; quand on considère $\ell_K^1(I)$ comme un espace normé, sans préciser sa norme, c’est toujours de la norme $\|x\|_1$ qu’il s’agit. On écrira $\mathcal{B}(I)$ et $\ell^1(I)$ au lieu de $\mathcal{B}(I; \mathbf{R})$ et $\ell^1_\mathbf{R}(I)$.

### 3. Sous-espaces vectoriels et espaces quotients d’un espace vectoriel topologique ; produits d’espaces vectoriels topologiques ; somme directe topologique de sous-espaces

Tout ce qui a été dit pour les modules topologiques (TG, III, p. 45-48 et 52-54) s’applique en particulier aux espaces vectoriels topologiques. Si M est un sous-espace vectoriel d’un espace vectoriel topologique E, la topologie induite sur M par celle de E est compatible avec la structure d’espace vectoriel de M, et l’adhérence $\overline{M}$ de M dans E est un sous-espace vectoriel de E. La topologie quotient de celle de E par M est compatible avec la structure d’espace vectoriel de E/M.

Si E est un espace vectoriel topologique non nécessairement séparé, l’adhérence N de {0} dans E (intersection des voisinages de 0) est un sous-espace vectoriel fermé de E ; l’espace vectoriel quotient E/N, qui est séparé, est appelé l’espace vectoriel séparé associé à E.

Soit $(E_i)_{i \in I}$ une famille d’espaces vectoriels topologiques sur un même corps topologique K, et soit E l’espace vectoriel produit des $E_i$. La topologie produit des topologies des $E_i$ est compatible avec la structure d’espace vectoriel de E. Dans l’espace produit E, le sous-espace F, somme directe des $E_i$, est partout dense (TG, III, p. 17, prop. 25).

Pour certains types d’espaces vectoriels topologiques sur le corps $\mathbf{R}$ ou le corps $\mathbf{C}$, nous définirons au chap. II, p. 32, une topologie sur une somme directe d’une famille $(E_i)$ d’espaces vectoriels topologiques, distincte en général de la topologie induite par la topologie produit de celle des $E_i$.

Tout ce qui a été dit sur les sommes directes finies de sous-groupes stables de groupes topologiques à opérateurs (TG, III, p. 46-48) s’applique aux espaces vectoriels topologiques en remplaçant partout « sous-groupe stable » par « sous-espace vectoriel ».

#### Remarque {#evt-i-s1-n3-rem-1 .statement}

Étant donné un sous-espace vectoriel fermé M d’un espace vectoriel topologique séparé E, il n’existe pas nécessairement de sous-espace vectoriel supplémentaire (algébrique) de M qui soit fermé dans E (même si E est un espace normé ; cf. IV, p. 55, exerc. 16, c)) ; à plus forte raison il n’existe pas nécessairement de supplémentaire topologique de M dans E (cf. I, p. 26, exerc. 8). Toutefois, nous verrons au § 2 que lorsque K est un corps valué complet non discret, tout sous-espace fermé M de E, de codimension finie, admet un supplémentaire topologique dans E (I, p. 15, prop. 3).

### 4. Structure uniforme et complétion d’un espace vectoriel topologique

La topologie d’un espace vectoriel topologique E, étant compatible avec la structure de groupe additif de E, définit sur E une structure uniforme (TG, III, p. 20) ; lorsque nous parlerons de la structure uniforme d’un espace vectoriel topologique, c’est toujours de cette structure qu’il sera question, sauf mention expresse du contraire. Toute application linéaire continue d’un espace vectoriel topologique E dans un espace vectoriel topologique F est uniformément continue (TG, III, p. 21, prop. 3) ; toute application de E dans lui-même de la forme $x \mapsto \alpha x + b$ est uniformément continue. Un ensemble équicontinu d’applications linéaires de E dans F est uniformément équicontinu (TG, X, p. 15, prop. 5).

#### Remarque 1 {#evt-i-s1-n4-rem-1 .statement}

Si B est une partie précompacte de K, alors, pour tout voisinage V de 0 dans E, il y a un voisinage U de 0 dans E tel que BU ⊂ V. En effet, soit W un voisinage de 0 dans E tel que W + W ⊂ V ; il y a un voisinage T_0 de 0 dans K et un voisinage U_0 de 0 dans E tels que T_0 U_0 ⊂ W, en vertu de (EVT'_III). Comme B est précompact, il y a un nombre fini de points $\lambda_i \in B$ (1 ≤ i ≤ n) tels que les $\lambda_i + T_0$ recouvrent B ; en vertu de (EVT'_II), il y a ensuite un voisinage U ⊂ U_0 de 0 dans E tel que $\lambda_i U \subset W$ pour tout i ; il est clair que U répond à la question. De la même façon (en utilisant (EVT'_I) au lieu de (EVT'_II)), on montre que si H est une partie précompacte de E, alors, pour tout voisinage V de 0 dans E, il y a un voisinage T de 0 dans K tel que TH ⊂ V.

#### Remarque 2 {#evt-i-s1-n4-rem-2 .statement}

On déduit de 1) que, si B est une partie précompacte de K et H une partie précompacte de E, alors la restriction à B × H de l’application ($\lambda, x$ ↦ $\lambda x$) est uniformément continue. En effet, étant donné un voisinage V de 0 dans E, il y a un voisinage T de 0 dans K et un voisinage U de 0 dans E tels que TH + BU ⊂ V. Comme on peut écrire $\lambda x - \lambda' x' = (\lambda - \lambda') x + \lambda'(x - x')$, on voit que pour $\lambda, \lambda'$ dans B, x, x' dans H, $\lambda - \lambda' \in T$ et $x - x' \in U$, on a $\lambda x - \lambda' x' \in V$, ce qui prouve notre assertion.

Un espace vectoriel topologique est dit complet si, muni de sa structure uniforme, c’est un espace uniforme complet.

#### Définition 2 {#evt-i-s1-def-2 .statement}

On appelle espace de Banach un espace normé complet sur un corps valué non discret.

#### Exemple {#evt-i-s1-n4-exa-1 .statement}

Lorsque K est un corps valué non discret et complet, l’espace $\mathcal{B}(I; K)$ (I, p. 4, Exemple) est complet (TG, X, p. 21, cor. 1). Il en est de même de l’espace $\ell_K^1(I)$ (I, p. 4, Exemple), muni de la norme $\|x\|_1 = \sum_{i \in I} |\xi_i|$ : en effet, soit $(x_n)$ une suite de Cauchy dans cet espace ; si $x_n = (\xi_{n,i})_{i \in I}$, on a, pour tout $i \in I$,
$$
|\xi_{m,i} - \xi_{n,i}| \leq \|x_m - x_n\|_1 ;
$$
donc, pour chaque $i \in I$, la suite $(\xi_{n,i})_{n \geq 1}$ converge dans K vers une limite $\xi_i$. En outre, pour toute partie finie J de I, on a
$$
\sum_{i \in J} |\xi_{m,i} - \xi_{n,i}| \leq \|x_m - x_n\|_1 ;
$$

on en déduit d’abord qu’il existe une constante $a > 0$, indépendante de $J$, $m$ et $n$, telle que $\sum_{\xi_{m_1} \in J} |\xi_{m_1} - \xi_{n_1}| \leq a$. En faisant tendre $m$ vers $+\infty$, on en tire $\sum_{\xi_1 \in J} |\xi_1 - \xi_{n_1}| \leq a$, d’où $\sum_{\xi_1 \in I} |\xi_1| \leq a + \|x_n\|_1$, ce qui prouve que $z = (\xi_i)_{i \in I}$ appartient à $\ell_K^1(I)$; de plus, pour tout $\varepsilon > 0$, il existe $n_0$ tel que, pour $n \geq n_0$, on ait $\sum_{\xi_1 \in J} |\xi_1 - \xi_{n_1}| \leq \varepsilon$ pour toute partie finie $J$ de $I$; en passant à la limite suivant l’ensemble filtrant des parties finies de $I$, on voit que $\|z - x_n\|_1 \leq \varepsilon$ pour $n \geq n_0$, ce qui montre que $z$ est limite de la suite $(x_n)$ dans l’espace normé $\ell_K^1(I)$.

Soient $K$ un corps topologique séparé, $E$ un espace vectoriel topologique sur $K$, et supposons que l’anneau complété $\hat{K}$ soit un corps (ce qui s’appliquera en particulier au cas où $K$ est un corps valué (TG, IX, p. 30, prop. 7)). Alors le séparé complété $\hat{E}$ de $E$ est muni d’une structure d’espace vectoriel topologique complet sur $\hat{K}$ (TG, III, p. 54); on dit que $\hat{E}$, muni de cette structure, est le séparé complété de l’espace vectoriel topologique $E$, ou simplement le complété de $E$ lorsque $E$ est séparé.

### 5. Voisinages de l’origine dans un espace vectoriel topologique sur un corps valué

#### Définition 3 {#evt-i-s1-def-3 .statement}

Soient $K$ un corps valué, $E$ un espace vectoriel à gauche sur $K$; on dit qu’une partie $M$ de $E$ est équilibrée si, pour tout $x \in M$ et tout $\lambda \in K$ tel que $|\lambda| \leq 1$, on a $\lambda x \in M$ (ou, en d’autres termes, si $\lambda M \subset M$ pour $|\lambda| \leq 1$).

#### Proposition 2 {#evt-i-s1-prop-2 .statement}

Dans un espace vectoriel topologique $E$ sur un corps valué $K$, l’adhérence d’un ensemble équilibré $M$ est un ensemble équilibré.

En effet, soit $B$ l’ensemble des $\xi \in K$ tels que $|\xi| \leq 1$; il est fermé dans $K$. L’application continue $(\lambda, x) \mapsto \lambda x$ applique $B \times M$ dans $M$, donc elle applique $B \times \overline{M}$ dans $\overline{M}$ (TG, I, p. 9, th. 1), ce qui prouve que $\overline{M}$ est équilibré.

Lorsque $M$ est un ensemble quelconque dans un espace vectoriel $E$ sur un corps valué $K$, l’ensemble $M_1$ des $\lambda x$, où $x$ parcourt $M$ et $\lambda$ l’ensemble des éléments de $K$ tels que $|\lambda| \leq 1$, est évidemment le plus petit ensemble équilibré contenant $M$; on l’appelle l’enveloppe équilibrée de $M$.

#### Proposition 3 {#evt-i-s1-prop-3 .statement}

Soit $K$ un corps valué localement compact et non discret, et soit $E$ un espace vectoriel topologique séparé (resp. un espace vectoriel topologique) sur $K$. Pour toute partie compacte (resp. précompacte) $H$ de $E$, l’enveloppe équilibrée de $H$ est compacte (resp. précompacte).

En effet, si $B$ désigne la boule $|\xi| \leq 1$ dans $K$, l’enveloppe équilibrée de $H$ est l’image de $B \times H$ par l’application continue $m : (\lambda, x) \mapsto \lambda x$; si $H$ est compact et $E$ séparé, cette image est donc compacte, puisqu’il en est ainsi de $B$; si $H$ est précompact, la restriction à $B \times H$ de $m$ est uniformément continue (I, p. 5, Remarque 2), et comme $B \times H$ est précompact, il en est de même de son image par $m$ (TG, II, p. 30, prop. 2).

On notera que l’enveloppe équilibrée d’un ensemble fermé n’est pas nécessairement fermée. Par exemple, dans $\mathbf{R}^2$, l’enveloppe équilibrée de l’hyperbole définie par l’équation $xy = 1$ n’est pas fermée.

Comme la réunion d’une famille de parties équilibrées de E est équilibrée, pour toute partie M de E, il y a un plus grand ensemble équilibré N contenu dans M, que l’on appelle le noyau équilibré de M ; pour qu’il soit non vide, il faut et il suffit que $0 \in M$. Dire que $x \in N$ signifie que, pour tout $\lambda \in K$ tel que $|\lambda| \leq 1$, on a $\lambda x \in M$, ou encore (si $0 \in M$) que, pour tout $\mu \in K$ tel que $|\mu| \geq 1$, on a $x \in \mu M$. Si $0 \in M$, le noyau équilibré N de M est donc l’intersection $\bigcap_{|\mu| \geq 1} \mu M$. Ceci montre en particulier que si M est fermé, il en est de même de N.

#### Définition 4 {#evt-i-s1-def-4 .statement}

Soient K un corps valué non discret, E un espace vectoriel à gauche sur K, A et B deux parties de E. On dit que A absorbe B s’il existe $\alpha > 0$ tel que l’on ait $\lambda A \supset B$ pour $|\lambda| \geq \alpha$ (ce qui équivaut à $\mu B \subset A$ pour $\mu \neq 0$ et $|\mu| \leq \alpha^{-1}$). Une partie A de E est dite absorbante si elle absorbe toute partie réduite à un point.

Soit A une partie équilibrée de E ; pour qu’elle absorbe une partie B de E, il suffit qu’il existe $\lambda \neq 0$ tel que $\lambda A \supset B$; en effet, pour $|\mu| \geq |\lambda|$, on a $\lambda A = (\lambda \mu^{-1}) \mu A$, et comme $\mu A$ est équilibré et $|\lambda \mu^{-1}| \leq 1$, $\lambda A \subset \mu A$, d’où $B \subset \mu A$. En particulier, pour qu’une partie équilibrée A de E soit absorbante, il faut et il suffit que pour tout $x \in E$, il existe $\lambda \neq 0$ dans K tel que $\lambda x \in A$. Toute partie absorbante de E engendre l’espace vectoriel E. Toute intersection finie d’ensembles absorbants est un ensemble absorbant.

#### Proposition 4 {#evt-i-s1-prop-4 .statement}

Dans un espace vectoriel topologique E sur un corps valué non discret K, il existe un système fondamental $\mathcal{B}$ de voisinages fermés de 0, tel que :
(EV₁) Tout ensemble $V \in \mathcal{B}$ est équilibré et absorbant.
(EV₂) Quels que soient $V \in \mathcal{B}$ et $\lambda \neq 0$ dans K, on a $\lambda V \in \mathcal{B}$ (invariance de $\mathcal{B}$ par les homothéties de rapport $\neq 0$).
(EV₃) Pour tout $V \in \mathcal{B}$, il existe $W \in \mathcal{B}$ tel que $W + W \subset V$.

Réciproquement, soit E un espace vectoriel sur K, et soit $\mathcal{B}$ une base de filtre sur E satisfaisant aux conditions (EV₁), (EV₂) et (EV₃). Il existe alors une topologie (et une seule) sur E, compatible avec la structure d’espace vectoriel de E, et pour laquelle $\mathcal{B}$ soit un système fondamental de voisinages de 0.

Remarquons d’abord qu’en vertu de l’axiome (EVT'₃), le noyau équilibré d’un voisinage V de 0 est un voisinage de 0, car il existe un nombre $\alpha > 0$ et un voisinage W de 0 tels que les relations $|\lambda| \leq \alpha$ et $x \in W$ entraînent $\lambda x \in V$; comme il y a par hypothèse un élément $\mu \neq 0$ dans K tel que $|\mu| \leq \alpha$, $\mu W$ est un voisinage de 0 contenu dans V, et pour $|\lambda| \leq 1$ et $x \in \mu W$, on a $\lambda x \in V$ en vertu du choix de W, d’où notre assertion. En outre, si V est fermé, il en est de même de son noyau équilibré ; donc, en vertu de l’axiome (O₃), vérifié par tout groupe topologique (TG, III, p. 20 et TG, II, p. 5, cor. 3), l’ensemble $\mathcal{B}$ des voisinages équilibrés et fermés est un système fondamental de voisinages de 0 dans E. D’autre part, en vertu de (EVT'₁), tout voisinage de 0 dans E est absorbant ; il est clair en outre que $\mathcal{B}$ vérifie (EV₂) (cf. I, p. 3, corollaire) ; enfin, tout système fondamental de voisinages de 0 dans E satisfait à (EV₃) en vertu de la continuité de $(x, y) \mapsto x + y$ au point $(0, 0)$. L’ensemble $\mathcal{B}$ répond donc à la question.

Soient maintenant E un espace vectoriel sur K, et $\mathcal{B}$ une base de filtre sur E satisfaisant à (EV₁), (EV₂) et (EV₃). L’axiome (EV₁) montre d’abord que pour tout $V \in \mathcal{B}$, on a $-V = V$ et $0 \in V$; ces relations et l’axiome (EV₃) montrent que $\mathcal{B}$ est un système fondamental de voisinages de 0 pour une topologie sur E compatible avec la structure de groupe additif de E (TG, III, p. 4). Comme d’autre part les axiomes (EVT₁'), (EVT₂') et (EVT₃') sont des conséquences immédiates de (EV₁) et (EV₂), la topologie ainsi définie satisfait à l’axiome (EVT), ce qui achève la démonstration.

#### Remarque 1 {#evt-i-s1-n5-rem-1 .statement}

Dans un espace normé sur un corps valué non discret, l’ensemble des boules ouvertes (resp. des boules fermées) de centre 0 est un système fondamental de voisinages de 0 qui satisfait aux conditions (EV₁), (EV₂) et (EV₃).

#### Remarque 2 {#evt-i-s1-n5-rem-2 .statement}

Lorsque le corps K des scalaires est le corps $\mathbf{R}$ ou le corps $\mathbf{C}$, toute base de filtre $\mathcal{B}$ sur E qui satisfait aux deux seuls axiomes (EV₁) et (EV₃) est un système fondamental de voisinages de 0 pour une topologie compatible avec la structure d’espace vectoriel de E. En effet, tout revient à prouver que, dans ces conditions, pour tout $\lambda \neq 0$ dans K et tout $V \in \mathcal{B}$, il existe $W \in \mathcal{B}$ tel que $\lambda W \subset V$. Or, il résulte aussitôt de (EV₃) qu’il existe $W_1 \in \mathcal{B}$ tel que $2W_1 \subset V$, d’où on déduit, par récurrence sur n, que pour tout entier $n > 0$ il existe $W_n \in \mathcal{B}$ tel que $2^n W_n \subset V$. Comme V est équilibré, il suffit de prendre n assez grand pour que $2^n = |2^n| > |\lambda|$; $W = W_n$ répond à la question.

Ce résultat ne s’étend pas à un corps valué non discret K quelconque, car dans un tel corps on n’a plus nécessairement $|m\varepsilon| = m$ pour tout entier naturel m ($\varepsilon$ désignant l’élément unité du corps ; cf. I, p. 22, exerc. 1).

#### Remarque 3 {#evt-i-s1-n5-rem-3 .statement}

Si K est un corps discret, les conditions (EVT₁') et (EVT₃') sont vérifiées pour une topologie quelconque sur E. En raisonnant comme dans la prop. 4, on voit aisément que si E est un espace vectoriel topologique sur K, il existe un système fondamental $\mathcal{B}$ de voisinages fermés de 0 dans E satisfaisant aux conditions (EV₂) et (EV₃). Réciproquement, si une base de filtre $\mathcal{B}$ sur un espace vectoriel E par rapport à K est telle que 0 appartienne à tous les ensembles de $\mathcal{B}$, et satisfait à (EV₂) et (EV₃), $\mathcal{B}$ est un système fondamental de voisinages de 0 pour une topologie compatible avec la structure d’espace vectoriel de E.

### 6. Critères de continuité et d’équicontinuité

Soient E et F deux espaces vectoriels topologiques sur un même corps K ; pour qu’une application linéaire $f$ de E dans F soit continue, il suffit qu’elle soit continue à l’origine (TG, III, p. 15, prop. 23). Cette proposition se généralise de la façon suivante :

#### Proposition 5 {#evt-i-s1-prop-5 .statement}

Soient $E_i$ (1 $\leq i \leq n$) et F des espaces vectoriels topologiques sur un corps valué commutatif et non discret K. Pour qu’une application multilinéaire $f$ de $\prod_{i=1}^n E_i$ dans F soit continue dans l’espace produit $\prod_{i=1}^{n'} E_i$, il suffit qu’elle soit continue au point (0, 0, ..., 0).

En effet, soit $(a_1, a_2, ..., a_n)$ un point quelconque de $\prod_{i=1}^n E_i$; il faut montrer que pour tout voisinage W de 0 dans F, il existe dans chaque $E_i$ (1 $\leq i \leq n$) un voisinage $V_i$ de 0 tel que les n relations $z_i \in V_i$ entraînent

$$
f(a_1 + z_1, a_2 + z_2, ..., a_n + z_n) - f(a_1, a_2, ..., a_n) \in W .
$$

Or, on peut écrire

$$
f(a_1 + z_1, ..., a_n + z_n) - f(a_1, ..., a_n) = \sum_H u_H
$$

où H parcourt les $2^n - 1$ parties de l’intervalle $I = \{1, n\}$ de $\mathbf{N}$ distinctes de I, et où, pour chaque H, on a $u_H = f(y_1, y_2, ..., y_n)$, avec $y_i = a_i$ pour $i \in H$ et $y_i = z_i$ pour $i \notin H$. Il existe $2^n - 1$ voisinages équilibrés $W_H$ de 0 dans F tels que $\sum_H W_H \subset W$; d’autre part, comme $f$ est continue au point $(0, ..., 0)$ par hypothèse, il existe dans chaque $E_i$ un voisinage $U_i$ de 0 $(1 \leq i \leq n)$ tel que les $n$ relations $x_i \in U_i$ entraînent $f(x_1, ..., x_n) \in \bigcap_H W_H$. Comme $U_i$ est absorbant, il existe $\lambda_i \neq 0$ dans K tel que $\lambda_i a_i \in U_i$. Soit $\lambda$ un élément de K tel que $|\lambda| \geq \prod_{i \in H} |\lambda_i|^{-1}$ pour toute partie H de I ; montrons que les voisinages $V_i = \lambda^{-1} U_i$ répondent à la question. En effet, si $p$ est le nombre d’éléments de $I - H$, on peut alors écrire $u_H = \mu f(x_1, ..., x_n)$, avec $x_i \in U_i$ pour $1 \leq i \leq n$, et $\mu = \lambda^{-np} (\prod_{i \in H} \lambda_i^{-1})$, et il résulte des choix précédents que $|\mu| \leq 1$, d’où $u_H \in \mu W_H \subset W_H$, puisque $W_H$ est équilibré. La proposition est donc démontrée.

#### Proposition 6 {#evt-i-s1-prop-6 .statement}

*Les hypothèses sur $E_i$ ($1 \leq i \leq n$) et F étant celles de la prop. 5, pour qu’un ensemble $\mathcal{E}$ d’applications multilinéaires de $\prod_{i=1}^n E_i$ dans F soit équicontinu, il suffit qu’il soit équicontinu au point $(0, 0, ..., 0)$*.

En effet, dans la démonstration de la prop. 5, les $U_i$ ($1 \leq i \leq n$) peuvent être pris tels que les relations $x_i \in U_i$ ($1 \leq i \leq n$) entraînent $f(x_1, ..., x_n) \in \bigcap_H W_H$ pour toute application $f \in \mathcal{E}$.

### 7. Topologies initiales d’espaces vectoriels

#### Proposition 7 {#evt-i-s1-prop-7 .statement}

*Soit $(E_i)_{i \in I}$ une famille d’espaces vectoriels topologiques sur un corps topologique K. Soit E un espace vectoriel sur K, et pour chaque $i \in I$, soit $f_i$ une application linéaire de E dans $E_i$. Alors la moins fine des topologies sur E qui rendent continues toutes les fonctions $f_i$ est une topologie $\mathcal{T}$ compatible avec la structure d’espace vectoriel de E. En outre, si pour tout $x \in E$, $\varphi(x)$ désigne le point $(f_i(x))$ de l’espace produit $F = \prod_{i \in I} E_i$, la topologie $\mathcal{T}$ est l’image réciproque par l’application linéaire $\varphi$ de la topologie du sous-espace $\varphi(E)$ de F.*

La dernière partie de la proposition est un cas particulier de TG, I, p. 26, prop. 3. La proposition est alors conséquence du lemme suivant :

*Lemme. — Soient M et N deux espaces vectoriels, g une application linéaire de M dans N. Si $\mathcal{T}_0$ est une topologie compatible avec la structure d’espace vectoriel de N, l’image réciproque de $\mathcal{T}_0$ par g est compatible avec la structure d’espace vectoriel de M.*

Montrons par exemple que $(\lambda, x) \mapsto \lambda x$ est continue en tout point $(\lambda_0, x_0)$ de $K \times M$. Posons $y = g(x_0)$. Tout voisinage de 0 dans $M$ contient un voisinage de la forme $\overline{g^{-1}}(U)$, où $U$ est un voisinage de 0 dans $N$; par hypothèse, il existe un voisinage $V$ de 0 dans $K$ et un voisinage $W$ de 0 dans $N$ tels que les relations $\lambda - \lambda_0 \in V$, $y - y_0 \in W$ entraînent $\lambda y - \lambda_0 y_0 \in U$. Les relations $\lambda - \lambda_0 \in V$, $x - x_0 \in \overline{g^{-1}}(W)$ entraînent donc $\lambda x - \lambda_0 x_0 \in \overline{g^{-1}}(U)$. On démontre de même que $(x, y) \mapsto x - y$ est continue dans $M \times M$.

Pour chaque indice $i \in I$, soit $\mathcal{B}_i$ un système fondamental de voisinages de 0 dans $E_i$. D’après la définition de la topologie $\mathcal{T}$, le filtre des voisinages de 0 pour cette topologie est engendré par la réunion des ensembles de parties $\overline{f_i^{-1}}(\mathcal{B}_i)$; autrement dit, les ensembles de la forme $\bigcap_k \overline{f_{i_k}^{-1}}(V_{i_k})$ forment un système fondamental de voisinages de 0 pour $\mathcal{T}$, $(i_k)_{1 \leq k \leq n}$ étant une suite finie quelconque d’indices de $I$, et, pour chaque indice $k$, $V_{i_k}$ un ensemble quelconque de $\mathcal{B}_{i_k}$.

#### Corollaire 1 {#evt-i-s1-prop-7-cor-1 .statement}

*Soit G un espace vectoriel topologique sur K. Pour qu’un ensemble H d’applications de G dans E soit équicontinu, il faut et il suffit que, pour tout $i \in I$, l’ensemble des $f_i \circ u$, où $u$ parcourt H, soit équicontinu.*
C’est un cas particulier de TG, X, p. 14, prop. 3.

#### Corollaire 2 {#evt-i-s1-prop-7-cor-2 .statement}

*Les espaces $E_i$ étant supposés séparés, pour que la topologie $\mathcal{T}$ soit séparée, il faut et il suffit que, pour tout $x \neq 0$ dans $E$, il existe un indice $i \in I$ tel que $f_i(x) \neq 0$.*
En effet, $\varphi(E)$ est alors un espace séparé, et pour que $\mathcal{T}$ soit séparée, il faut et il suffit évidemment que $\varphi$ soit injective; on notera qu’on peut alors identifier $E$ (muni de $\mathcal{T}$) au sous-espace $\varphi(E)$ de $\prod_{i \in I} E_i$ par l’application $\varphi$.

#### Corollaire 3 {#evt-i-s1-prop-7-cor-3 .statement}

*Supposons les $E_i$ complets et $\varphi(E)$ fermé dans $F = \prod_{i \in I} E_i$. Alors E est complet pour la topologie $\mathcal{T}$.*
En effet, le sous-espace $\varphi(E)$ de $F$ est alors complet (TG, II, p. 16, prop. 8 et p. 17, prop. 10), donc il en est de même de $E$ pour la topologie image réciproque par $\varphi$ de celle de $\varphi(E)$ (TG, I, p. 51, prop. 10, et TG, II, p. 13, prop. 4).

#### Exemple {#evt-i-s1-n7-exa-1 .statement}

Soient $\mathscr{D}'(\mathbf{R})$ l’espace des distributions sur $\mathbf{R}$, $p$ un nombre tel que $1 \leq p \leq +\infty$, $j : L^p(\mathbf{R}) \to \mathscr{D}'(\mathbf{R})$ l’injection canonique, qui est continue (lorsque $L^p(\mathbf{R})$ est muni de sa topologie d’espace normé et $\mathscr{D}'(\mathbf{R})$ de la topologie forte). Pour toute distribution $f \in \mathscr{D}'(\mathbf{R})$, $D(f)$ désigne sa dérivée; on rappelle que $f \mapsto D(f)$ est un endomorphisme continu de $\mathscr{D}'(\mathbf{R})$. Soit alors $E$ le sous-espace vectoriel de $L^p(\mathbf{R})$ formé des $f \in L^p(\mathbf{R})$ telles que $D(f) \in L^p(\mathbf{R})$, et munissons $E$ de la topologie la moins fine rendant continues les injections canoniques $i : E \to L^p(\mathbf{R})$ et $D : E \to L^p(\mathbf{R})$ ($L^p(\mathbf{R})$ étant muni de sa topologie d’espace normé). Pour cette topologie, l’espace $E$ est *complet*. En effet, l’image de $E$ dans $F = L^p(\mathbf{R}) \times L^p(\mathbf{R})$ par l’application $\varphi : f \mapsto (f, D(f))$ est fermée, car c’est la trace sur $L^p(\mathbf{R}) \times L^p(\mathbf{R})$ de l’image G de $\mathcal{D}'(\mathbf{R})$ dans $\mathcal{D}'(\mathbf{R}) \times \mathcal{D}'(\mathbf{R})$ par l’application

$$
\varphi_0 : f \mapsto (f, D(f)) ;
$$

or G est le graphe de $\varphi_0$, donc est fermé dans $\mathcal{D}'(\mathbf{R}) \times \mathcal{D}'(\mathbf{R})$ (TG, I, p. 53, cor. 2 de la prop. 2), et comme $\varphi(E)$ est l’image réciproque de G par $i \times i$, qui est continue, $\varphi(E)$ est fermé dans F. \*

#### Corollaire 4 {#evt-i-s1-prop-7-cor-4 .statement}

*Soit E un espace vectoriel sur un corps topologique K, et soit $(\mathcal{T}_i)_{i \in I}$ une famille de topologies compatibles avec la structure d’espace vectoriel de E ; alors la borne supérieure $\mathcal{T}$ des topologies $\mathcal{T}_i$ est compatible avec la structure d’espace vectoriel de E.*

En effet, si $E_i$ désigne l’espace vectoriel topologique obtenu en munissant E de $\mathcal{T}_i$, et $f_i$ l’application identique de E sur $E_i$, $\mathcal{T}$ est la moins fine des topologies rendant continues les $f_i$.

## EXERCICES {#evt-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
