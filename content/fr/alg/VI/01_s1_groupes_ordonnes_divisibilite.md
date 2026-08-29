---
book: alg
book_title: Algebra
chapter: VI
chapter_title: Groupes et corps ordonnés
section: 1
section_title: GROUPES ORDONNÉS. DIVISIBILITÉ
lang: fr
source: alg-iv-vii-fr
pdf_pages: 0290-0307, 0318-0324
extraction: ocr
subsections:
    - "no": 1
      title: Définition des monoïdes et groupes ordonnés
      page: 0
      pdf_page: 290
    - "no": 2
      title: Monoïdes et groupes préordonnés
      page: 3
      pdf_page: 292
    - "no": 3
      title: Éléments positifs
      page: 3
      pdf_page: 292
    - "no": 4
      title: Groupes filtrants
      page: 4
      pdf_page: 293
    - "no": 5
      title: Relations de divisibilité dans un corps
      page: 5
      pdf_page: 294
    - "no": 6
      title: Opérations élémentaires sur les groupes ordonnés
      page: 6
      pdf_page: 295
    - "no": 7
      title: Homomorphismes croissants de groupes ordonnés
      page: 7
      pdf_page: 296
    - "no": 8
      title: Bornes supérieure et inférieure dans un groupe ordonné
      page: 8
      pdf_page: 297
    - "no": 9
      title: Groupes réticulés
      page: 9
      pdf_page: 298
    - "no": 10
      title: Le théorème de décomposition
      page: 10
      pdf_page: 299
    - "no": 11
      title: Partie positive et partie négative
      page: 11
      pdf_page: 300
    - "no": 12
      title: Éléments étrangers
      page: 13
      pdf_page: 302
    - "no": 13
      title: Éléments extrémaux
      page: 16
      pdf_page: 305
statements: 52
exercises: 20
content_sha256: af0e37d4d46945de0a0c4108c90fd198171ff9250cd1b866a07a6baf0bc972be
---

## § 1. GROUPES ORDONNÉS. DIVISIBILITÉ

Les notions et résultats exposés dans ce paragraphe concernent l’étude des relations d’ordre dans les monoïdes commutatifs (I, p. 12, déf. 2), le cas le plus important étant celui des groupes commutatifs. Sauf mention expresse du contraire, la loi de composition dans les groupes et monoïdes étudiés sera notée additivement. D’autre part, nous exposerons chemin faisant certaines applications algébriques importantes de la théorie des monoïdes et groupes ordonnés, et nous traduirons au fur et à mesure une partie des résultats obtenus dans la notation multiplicative qui est propre à ces applications.

### 1. Définition des monoïdes et groupes ordonnés

#### Définition 1 {#alg-vi-s1-def-1 .statement}

Sur un ensemble $M$, on dit qu’une structure de monoïde commutatif (notée additivement) et une structure d’ordre (notée $\leq$) sont compatibles si elles satisfont à l’axiome suivant :
(MO) Quel que soit $z \in M$, la relation $x \leq y$ entraîne $x + z \leq y + z$.
Un ensemble $M$ muni d’une structure de monoïde commutatif et d’une structure d’ordre compatibles est appelé un monoïde ordonné ; si sa structure de monoïde commutatif est une structure de groupe, il est appelé groupe ordonné.

On peut définir de façon analogue la notion de monoïde ordonné non commutatif (VI, p. 29, exerc. 1).

Si une structure d’ordre est compatible avec la structure d’un monoïde, il en est de même de la structure d’ordre opposée.

#### Exemple 1 {#alg-vi-s1-n1-exa-1 .statement}

Le groupe additif des entiers rationnels et celui des nombres rationnels sont des groupes ordonnés quand on les munit des structures d’ordre définies en I, p. 20 et 112.
\* Il en est de même du groupe additif des nombres réels (TG, IV, p. 3). \*
2) \* Le groupe additif des fonctions numériques finies définies dans un ensemble E est un groupe ordonné pour la structure d’ordre définie par la relation « quel que soit $x \in E, f(x) \leq g(x)$ » que l’on écrit « $f \leq g$ ». Cette relation exprime que le graphe de la fonction $f$ est au-dessous de celui de la fonction $g$; le lecteur pourra trouver commode de se reporter quelquefois à cette interprétation graphique. \*

Conformément aux définitions générales (E, IV, p. 6), une application bijective $f$ d’un monoïde ordonné $M$ sur un monoïde ordonné $M'$ est appelée un isomorphisme de $M$ sur $M'$ si la structure de $M'$ est obtenue en transportant celle de $M$ au moyen de $f$. Il revient au même de dire que $f$ est une application de $M$ sur $M'$ telle que

$$
f(x + y) = f(x) + f(y)
$$

(c’est-à-dire un homomorphisme du monoïde $M$ sur le monoïde $M'$), et que les relations $x \leq y$ et $f(x) \leq f(y)$ sont équivalentes (d’où résulte en particulier que $f(x) = f(y)$ entraîne $x = y$, c’est-à-dire que $f$ est injective).

#### Proposition 1 (« addition des inégalités ») {#alg-vi-s1-prop-1 .statement}

Dans un monoïde ordonné $M$, soient $(x_i)$ et $(y_i)$ ($1 \leq i \leq n$) deux suites de $n$ éléments telles que, pour tout $i$, on ait $x_i \leq y_i$; alors on a

$$
x_1 + \cdots + x_n \leq y_1 + \cdots + y_n.
$$

Si de plus tous les éléments $x_i, y_i$ sont simplifiables (I, p. 15, déf. 5) (en particulier si $M$ est un groupe), et s’il existe $i$ tel que $x_i < y_i$, on a $x_1 + \cdots + x_n < y_1 + \cdots + y_n$.

Le cas où $n$ est quelconque se ramène par récurrence au cas $n = 2$, en utilisant, pour la seconde assertion, le fait qu’une somme d’éléments simplifiables est un élément simplifiable (I, p. 15, prop. 2). La première assertion résulte des relations

$$
x_1 + x_2 \leq x_1 + y_2 \quad \text{et} \quad x_1 + y_2 \leq y_1 + y_2,
$$

conséquences des hypothèses et de (MO). Cela étant, la relation

$$
x_1 + x_2 = y_1 + y_2
$$

impliquerait $x_1 + x_2 = x_1 + y_2 = y_1 + y_2$, d’où $x_2 = y_2$ et $x_1 = y_1$ si $x_1$ et $y_2$ sont simplifiables, ce qui démontre la seconde assertion.

#### Proposition 2 {#alg-vi-s1-prop-2 .statement}

Dans un groupe ordonné $G$ les relations $x \leq y$ et $x + z \leq y + z$ sont équivalentes.

On passe en effet de l’une à l’autre par addition aux deux membres de $z$, ou de $(-z)$.

On exprime ce fait en disant que, dans un groupe ordonné $G$, la structure d’ordre est invariant par translation. En d’autres termes une translation est un automorphisme pour la structure d’ordre d’un groupe ordonné.

#### Corollaire {#alg-vi-s1-n1-cor-1 .statement}

Dans un groupe ordonné $G$, les relations $x \leq y,\ 0 \leq y - x,\ x - y \leq 0$ et $-y \leq -x$ sont équivalentes.

On applique en effet la prop. 2 en prenant successivement $z = -x, z = -y,$ et $z = -(x + y)$.

On déduit en particulier de ce corollaire que, si $G$ est un groupe ordonné, l’application $x \mapsto -x$ de $G$ sur lui-même transforme sa structure d’ordre en la structure opposée.

### 2. Monoïdes et groupes préordonnés

Rappelons que, si une relation $x \leqslant y$ entre éléments d’un ensemble $E$ est réflexive et transitive, on dit que c’est une relation de préordre (E, III, p. 3). La relation « $x \leqslant y$ et $y \leqslant x$ » est une relation d’équivalence $S$ dans $E$, compatible avec la relation $x \leqslant y$; par passage au quotient, la relation $\leqslant$ définit sur l’ensemble $E/S$ une relation d’ordre, dite associée à $\leqslant$.

#### Définition 2 {#alg-vi-s1-def-2 .statement}

Sur un ensemble $M$, on dit qu’une relation de préordre (notée $\leqslant$) et une structure de monoïde commutatif (notée additivement) sont compatibles si elles satisfont à l’axiome suivant :

(MPO) Quel que soit $z \in M$, $x \leqslant y$ entraîne $x + z \leqslant y + z$.
Un ensemble $M$ muni d’une structure de monoïde commutatif et d’une relation de préordre compatibles est appelé un monoïde préordonné.

Soient $M$ un monoïde préordonné, et $S$ la relation d’équivalence « $x \leqslant y$ et $y \leqslant x$ ». En vertu de (MPO), la relation $x \equiv x'$ (mod. $S$) entraîne, pour tout $y \in M$, $x + y \leqslant x' + y$ et $x' + y \leqslant x + y$, c’est-à-dire $x + y \equiv x' + y$ (mod. $S$). En d’autres termes la relation d’équivalence $S$ est compatible avec l’addition dans $M$ (I, p. 26). Alors le quotient par $S$ de la loi additive de $M$, et la structure d’ordre associée à $\leqslant$, définissent sur $M/S$ une structure de monoïde ordonné. Dans le cas où $M$ est un groupe préordonné, $M/S$ est le groupe quotient de $M$ par le sous-groupe des éléments $x$ qui satisfont à $x \leqslant 0$ et $0 \leqslant x$.

### 3. Éléments positifs

Soit $G$ un groupe préordonné par une relation de préordre $\leqslant$; de $0 \leqslant x$ et $0 \leqslant y$ on déduit $y \leqslant x + y$ en vertu de (MPO), et $0 \leqslant x + y$ par transitivité ; ceci exprime que l’ensemble $G_+$ des $x \in G$ tels que $0 \leqslant x$ est stable pour l’addition ; en outre, la relation $x \leqslant y$ est équivalente à $0 \leqslant y - x$, c’est-à-dire à $y - x \in G_+$. Inversement :

#### Proposition 3 {#alg-vi-s1-prop-3 .statement}

Si $P$ est une partie d’un groupe commutatif $G$, contenant $0$ et telle que $P + P \subset P$, la relation $y - x \in P$ est une relation de préordre compatible avec la structure de groupe de $G$. Pour que cette relation définisse sur $G$ une structure de groupe ordonné, il faut et il suffit que l’on ait $P \cap (-P) = \{0\}$; pour que $G$ soit un groupe totalement ordonné pour cette structure, il faut et il suffit que l’on ait en outre $P \cup (-P) = G$.

On vérifie aussitôt que la relation $y - x \in P$ est réflexive et transitive, et (si on la note $x \leq y$) satisfait à l’axiome (MPO). Pour démontrer la seconde assertion, il suffit de remarquer que $P \cap (-P)$ est le sous-groupe $G'$ des éléments $x$ tels que $x \leq 0$ et $0 \leq x$. Enfin, dire que $G$ est totalement ordonné signifie que, pour tout couple d’éléments $x, y$ de $G$, l’un des éléments $x - y, y - x$ appartient à $P$, ce qui achève la démonstration.

#### Définition 3 {#alg-vi-s1-def-3 .statement}

Dans un groupe ordonné $G$, on appelle élément positif (resp. négatif) tout élément $x$ tel que $0 \leq x$ (resp. $x \leq 0$).

On notera que $0$ est l’unique élément à la fois positif et négatif ; tout élément $x$ tel que $0 < x$ (resp. $x < 0$) est dit strictement positif (resp. strictement négatif).

#### Exemple {#alg-vi-s1-n3-exa-1 .statement}

Dans le groupe additif $\mathbf{Z} \times \mathbf{Z}$, soit $P$ l’ensemble des éléments $(x, y)$ satisfaisant à deux inégalités $ax + by \geq 0, cx + dy \geq 0$, où $a, b, c, d$ sont des entiers (* ou des nombres réels *) tels que $ad - bc \neq 0$; le « cône » $P$ satisfait aux deux premières conditions de la prop. 3. On définit ainsi sur $\mathbf{Z} \times \mathbf{Z}$ diverses structures d’ordre compatibles avec sa structure de groupe ; le groupe n’est totalement ordonné pour aucune de ces structures.

#### Remarque {#alg-vi-s1-n3-rem-1 .statement}

En vertu de la condition $P + P \subset P$, dans un groupe ordonné $G$, la relation $x \geq 0$ implique $nx \geq 0$ pour tout entier naturel $n$. Si, de plus, l’élément positif $x$ du groupe $G$ est d’ordre fini $n$, $-x = (n-1)x$ est positif ; comme
$$
P \cap (-P) = \{0\},
$$
ceci entraîne $x = 0$. En particulier, si tous les éléments de $G$ sont d’ordre fini, on a $P = \{0\}$; la relation $x \leq y$ est alors équivalente à $x = y$ (structure d’ordre discrète).

### 4. Groupes filtrants

Rappelons (E, III, p. 12, déf. 7) qu’un ensemble ordonné $G$ est dit filtrant à droite (resp. à gauche) si, pour tout couple $(x, y)$ d’éléments de $G$, il existe $z \in G$ tel que $x \leq z$ et $y \leq z$ (resp. $z \leq x$ et $z \leq y$). Tout groupe ordonné filtrant à droite $G$ est aussi filtrant à gauche, et réciproquement : en effet, comme il existe $z \in G$ tel que $-x \leq z$ et $-y \leq z$, on a $-z \leq x$ et $-z \leq y$ (VI, p. 2, cor.). Nous parlerons donc simplement de groupe filtrant.

#### Proposition 4 {#alg-vi-s1-prop-4 .statement}

Pour qu’un groupe ordonné $G$ soit filtrant, il faut et il suffit qu’il soit engendré par ses éléments positifs, c’est-à-dire que tout élément de $G$ soit différence de deux éléments positifs.

En effet, si $G$ est filtrant, il existe, pour tout $x \in G$, un élément positif $z$ tel que $x \leq z$, et $x$ est différence des éléments positifs $z$ et $z - x$. Si, réciproquement, on a $x = u - v$ et $y = w - t$ avec $u, v, w, t$ positifs, l’élément $u + w$ est supérieur à $x$ et à $y$.

#### Proposition 5 {#alg-vi-s1-prop-5 .statement}

Si $(x_i)$ est une famille finie d’éléments d’un groupe filtrant $G$, il existe $z \in G$ tel que $x_i + z$ soit positif pour tout $i$.

Si $x_i = u_i - v_i$, avec $u_i$ et $v_i$ positifs, il suffit de prendre pour $z$ la somme de la famille $(v_i)$.

### 5. Relations de divisibilité dans un corps

Nous allons ici définir certains groupes ordonnés qui jouent un rôle important en algèbre. Dans ces groupes c’est la notation multiplicative qui est usuelle ; l’application à ces groupes des résultats obtenus précédemment en notation additive suppose donc faite leur traduction en notation multiplicative — traduction qui ne présentera aucune difficulté au lecteur. Dans tout ce n°, A désignera un anneau intègre et K le corps des fractions de A (I, p. 110).

Dans le groupe multiplicatif K* des éléments non nuls de K, l’ensemble P des éléments non nuls de A est stable, puisque A est un anneau. Il définit donc sur K* la relation de préordre $x^{-1}y \in P$, c’est-à-dire « il existe $z \in P$ tel que $y = zx$ », qui en fait un groupe préordonné (noté multiplicativement) (VI, p. 3, prop. 3). Généralisant au cas où $x$ et $y$ sont des éléments de K* la terminologie relative aux éléments de A (I, p. 93), la relation $x^{-1}y \in P$ s’énonce aussi : $x$ divise $y$, ou $x$ est diviseur de $y$, ou $y$ est multiple de $x$ (relativement à l’anneau A) ; et nous dirons que la relation $x^{-1}y \in P$ est la relation de divisibilité dans K* relativement à l’anneau A. La relation « $x$ divise $y$ » se note $x|y$, et sa négation $x \nmid y$. Les éléments de P ne sont autres que les multiples de 1.

#### Remarque 1 {#alg-vi-s1-n5-rem-1 .statement}

La relation de divisibilité dans K* dépend essentiellement de l’anneau A choisi. Si A = K, on obtient la relation « triviale » où $x|y$ pour tout couple $(x, y)$ d’éléments de K*. Soit $p$ (resp. $q$) un nombre premier ; les nombres rationnels $r/s$ dont le dénominateur n’est pas multiple de $p$ (resp. $q$) forment un sous-anneau $\mathbf{Z}_{(p)}$ (resp. $\mathbf{Z}_{(q)}$) de $\mathbf{Q}$ ; les relations de divisibilité dans $\mathbf{Q}^*$ relatives à ces deux anneaux sont distinctes si $p \neq q$, le nombre $p/q$ étant multiple de 1 pour l’une et non pour l’autre.

#### Remarque 2 {#alg-vi-s1-n5-rem-2 .statement}

Nous étendrons parfois la définition de la relation $x|y$ à un couple d’éléments de K (et non plus seulement de K*), cette relation étant synonyme de « il existe $z \in A$ tel que $y = zx$ » ; on aura donc $x|0$ pour tout $x \in K$. Ceci permet d’énoncer sans restriction les résultats suivants : si $x|y$ et $x|z$, alors $x|(y - z)$; si $x|y$ et $x \nmid z$, alors $x \nmid (y - z)$. On étend de même la terminologie correspondante.

Pour déduire de la relation de divisibilité une relation d’ordre (n° 2), il faut passer au groupe quotient de K* par le sous-groupe A* des éléments $x \in K^*$ tels que $x|1$ et $1|x$ ; ces éléments sont ceux de P qui sont diviseurs de 1, c’est-à-dire les éléments inversibles de A ; on les appelle souvent, par abus de langage, les unités de l’anneau A. Le groupe quotient $K^*/A^*$ est alors un groupe ordonné. Deux éléments $x$ et $y$ de K* qui appartiennent à la même classe mod. A* sont dits associés ; ceci veut dire que l’on a $x|y$ et $y|x$. Lorsque au contraire $x$ divise $y$ sans que $y$ divise $x$, on dit que $x$ divise strictement $y$, ou que $x$ est un diviseur strict de $y$, ou que $y$ est un multiple strict de $x$.

On notera que $K^*/A^*$ est un groupe filtrant, puisque K est corps des fractions de A (VI, p. 4, prop. 4).

Dire que deux éléments $x$ et $y$ de K* sont associés revient, en vertu de la transitivité de la relation de divisibilité, à dire que $x$ et $y$ ont mêmes multiples dans K. Pour tout $x \in K$, nous noterons $Ax$ l’ensemble des $zx$, où $z \in A$ ; l’ensemble $Ax$ est un sous-module de K considéré comme A-module. Par extension de la terminologie relative au cas où $x \in A$, nous l’appellerons un idéal principal fractionnaire du corps K relativement à l’anneau A. Par opposition les idéaux de l’anneau A seront dits entiers.

On notera que, si $A \neq K$, un idéal principal fractionnaire $\neq \{0\}$ n’est pas un idéal de K considéré comme anneau.

L’idéal principal fractionnaire $Ax$ se note aussi $(x)$. On écrira $x \equiv 0$ (mod. $y$) pour $x \in Ay$, et $x \equiv x'$ (mod. $y$) pour $x - x' \in Ay$; si $x \equiv x'$ (mod. $y$), on aura $zx \equiv zx'$ (mod. $zy$) quel que soit $z \in K$.

On notera que $x \equiv x'$ (mod. $y$) n’entraîne pas $zx \equiv zx'$ (mod. $y$) à moins que l’on ait $z \in A$. Ainsi, dans $\mathbf{Q}$, relativement à $\mathbf{Z}$, on a $4 \equiv 2$ (mod. 2) mais non $2 \equiv 1$ (mod. 2).

La relation $x|y$ équivaut évidemment à $(x) \supset (y)$. L’application $x \mapsto (x)$ de $K^*$ sur l’ensemble $\mathcal{P}^*$ des idéaux principaux fractionnaires $\neq (0)$ de K définit donc, par passage au quotient, une application bijective de $K^*/A^*$ sur $\mathcal{P}^*$; en transportant à $\mathcal{P}^*$, au moyen de cette application, la structure de groupe de $K^*/A^*$, on est conduit à définir comme produit des idéaux principaux fractionnaires $(x)$ et $(y)$ l’idéal $(xy)$, celui-ci ne dépendant que de $(x)$ et $(y)$. Muni de cette loi et de la relation d’ordre $(x) \supset (y)$, $\mathcal{P}^*$ est un groupe ordonné, isomorphe à $K^*/A^*$, et qu’on conviendra d’identifier à $K^*/A^*$ au moyen de l’application ci-dessus.

On notera que la relation « $x$ divise $y$ » qui, dans le cas des entiers positifs, implique que $x$ est plus petit que $y$, correspond à l’inclusion $(x) \supset (y)$ où l’idéal $(x)$ est « plus grand » que l’idéal $(y)$. On se souviendra de ce « renversement d’ordre » en notant par exemple que 7 a « plus de multiples » que 91.

Lorsqu’on étend la relation $x|y$ à tous les éléments de K, cette relation est encore équivalente à $(x) \supset (y)$ dans l’ensemble $\mathcal{P}$ de tous les idéaux principaux fractionnaires de K (dans lequel $(0)$ est le plus petit élément pour la relation d’inclusion).

Comme dans les nos précédents, nous allons utiliser dans la suite de ce paragraphe la notation additive. Cependant l’introduction de la terminologie relative à la divisibilité sera faite après l’introduction de la terminologie additive correspondante, dans des alinéas précédés du signe (DIV) (où il est entendu que les notations sont celles de ce no). Afin de faciliter le travail du lecteur, certains résultats importants seront traduits dans le langage de la divisibilité, la traduction de la prop. 7, par exemple, étant notée « PROPOSITION 7 (DIV) ».

### 6. Opérations élémentaires sur les groupes ordonnés

Soit H un sous-groupe d’un groupe ordonné G ; il est clair que la structure d’ordre induite sur H par celle de G est compatible avec la structure de groupe de H ; c’est toujours de celle-ci dont H sera supposé muni, sauf mention expresse du contraire.

Si P est l’ensemble des éléments positifs de G, l’ensemble des éléments positifs de H est H ∩ P.

Soit (G_α) une famille de groupes ordonnés ; conformément à la définition du produit d’ensembles ordonnés (E, III, p. 6), le groupe produit G = $\prod_{\alpha} G_{\alpha}$ est muni d’une structure d’ordre, la relation « (x_α) ≤ (y_α) » entre deux éléments de G étant, par définition, synonyme de « quel que soit α, x_α ≤ y_α ». On voit aussitôt que cette structure d’ordre est compatible avec la structure de groupe de G ; muni de cette structure, G est un groupe ordonné, qu’on appelle le produit des groupes ordonnés G_α. Les éléments positifs de G sont ceux dont toutes les composantes sont positives. Dans le cas où tous les facteurs G_α sont identiques à un même groupe ordonné H, G est le groupe H^I des applications de l’ensemble d’indices I dans H, la relation « f ≤ g » entre deux applications de I dans H étant synonyme de « quel que soit α ∈ I, f(α) ≤ g(α) » ; les applications positives sont celles qui ne prennent que des valeurs positives. On définit la somme directe d’une famille (G_α) de groupes ordonnés comme sous-groupe ordonné de leur produit (II, p. 12).

Soit (G_i)_{i \in I} une famille de groupes ordonnés dont l’ensemble d’indices I est bien ordonné ; rappelons (E, III, p. 22) que l’on définit, sur l’ensemble produit G = $\prod_{i} G_{i}$, une relation d’ordre, dite lexicographique, la relation « (x_i) < (y_i) » entre deux éléments de G étant, par définition, synonyme de « si β est le plus petit des indices tels que x_i ≠ y_i, on a x_β < y_β ». Rappelons que le produit d’une famille bien ordonnée d’ensembles totalement ordonnés est totalement ordonné pour l’ordre lexicographique. Dans le cas général, la relation d’ordre lexicographique sur G est compatible avec sa structure de groupe, comme on le vérifie aussitôt ; muni de cette structure, G est donc un groupe ordonné, qu’on appelle le produit lexicographique de la famille bien ordonnée de groupes ordonnés (G_i).

#### Remarque 1 {#alg-vi-s1-n6-rem-1 .statement}

Le cas le plus fréquent est celui où l’ensemble bien ordonné d’indices I est un intervalle fini {1, n} de N.
    2) L’ensemble des éléments positifs du produit lexicographique G se compose de 0 et des éléments dont la composante non nulle de plus petit indice est positive.

### 7. Homomorphismes croissants de groupes ordonnés

Soient G et G’ deux groupes ordonnés ; parmi les homomorphismes f du groupe additif sous-jacent de G dans celui de G’, il y a lieu de considérer les applications croissantes, c’est-à-dire celles pour lesquelles x ≤ y entraîne f(x) ≤ f(y). En vertu de la relation f(y − x) = f(y) − f(x), les homomorphismes croissants de G dans G’ sont caractérisés par le fait que l’image par un tel homomorphisme d’un élément positif de G est un élément positif de G’ ; si P (resp. P’) désigne l’ensemble des éléments positifs de G (resp. G’), ceci s’écrit f(P) ⊂ P’. Il est clair que l’injection canonique d’un sous-groupe G dans un groupe ordonné G’, et la projection d’un produit de groupes ordonnés sur un de ses facteurs sont des homomorphismes croissants.

Un isomorphisme (VI, p. 2) $f$ d’un groupe ordonné $G$ sur un groupe ordonné $G'$ est un homomorphisme bijectif de $G$ sur $G'$, tel que $f$ et l’homomorphisme réciproque soient tous deux croissants, ce qui s’écrit $f(P) = P'$.

Il peut arriver qu’un isomorphisme du groupe sous-jacent de $G$ sur celui de $G'$ soit croissant, sans que l’isomorphisme réciproque le soit aussi. Il en sera ainsi, par exemple, si $G = G'$, si $f$ est l’application identique de $G$ sur lui-même, et si $P \subset P'$ mais $P \neq P'$. Ainsi, sur $\mathbf{Z}$, on peut prendre pour $P'$ l’ensemble des entiers positifs (ordinaires) et pour $P$ celui des entiers positifs pairs.

(DIV) Soit $K$ le corps des fractions rationnelles $\mathbf{F}_2(X)$ sur le corps à deux éléments $\mathbf{F}_2$. Les relations de divisibilité relatives aux anneaux $\mathbf{F}_2[X] = A'$ et $\mathbf{F}_2[X^2, X^3] = A$ définissent sur $K^*$ deux structures de groupe ordonné distinctes, telles que $A \subset A'$ (ce sont des structures de groupe ordonné puisque 1 est la seule unité de $A$ et la seule de $A'$).

### 8. Bornes supérieure et inférieure dans un groupe ordonné

Rappelons (E, III, p. 10) que, si l’ensemble des majorants d’une partie $F$ d’un ensemble ordonné $E$ (c’est-à-dire l’ensemble des $z \in E$ tels que $x \leq z$ pour tout $x \in F$) admet un plus petit élément $a$, celui-ci, qui est alors unique, est appelé la borne supérieure de $A$. Si $F$ est l’ensemble des éléments d’une famille $(x_i)_{i \in I}$ d’éléments de $E$, sa borne supérieure, si elle existe, se note $\sup_{i \in I} x_i$ (ou $\sup x_i$ ou simplement $\sup(x_i)$); s’il s’agit d’une famille finie $(x_i)$ ($1 \leq i \leq n$), cette borne se note aussi $\sup(x_1, ..., x_n)$. La borne inférieure se définit d’une manière analogue et se note inf. Les opérations sup et inf sont associatives et commutatives.

Rappelons (E, loc. cit.) que, si $F$ est une partie d’un ensemble ordonné $E$, et $(x_i)$ une famille d’éléments de $F$, l’existence de $\sup(x_i)$ dans $E$ (que l’on peut noter $\sup_E(x_i)$) n’entraîne pas l’existence d’une borne supérieure des $x_i$ dans $F$ (que l’on peut noter $\sup_F(x_i)$ lorsqu’elle existe); si toutes deux existent, on a seulement $\sup_E(x_i) \leq \sup_F(x_i)$; en revanche si $\sup_E(x_i)$ existe et appartient à $F$, $\sup_F(x_i)$ existe et est égal à $\sup_E(x_i)$. Par exemple, dans l’anneau de polynômes $A = K[X, Y]$ ($K$ corps commutatif), les idéaux principaux $AX$ et $AY$ ont l’idéal $AX + AY$ pour borne supérieure (pour la relation $\subset$) dans l’ensemble ordonné de tous les idéaux de $A$, mais ont l’anneau $A$ pour borne supérieure dans l’ensemble des idéaux principaux de $A$.

(DIV) On dit qu’un élément $d$ de $K^*$ est un plus grand commun diviseur, ou, en abrégé, un $pgcd$, d’une famille $(x_i)$ d’éléments de $K^*$, si l’idéal principal fractionnaire $(d)$ est, dans $\mathcal{P}^*$, la borne supérieure (pour la relation $\subset$) de la famille d’idéaux $((x_i))$, ou, autrement dit, si, pour $z \in K^*$, la relation $z|d$ équivaut à « $z|x_i$ pour tout $i$ ». On dira de même que $m \in K^*$ est un plus petit commun multiple ou un $ppcm$ de la famille $(x_i)$ si $(m)$ est, dans $\mathcal{P}^*$, la borne inférieure de la famille d’idéaux $((x_i))$, c’est-à-dire si $m|z$ équivaut à « $x_i|z$ pour tout $i$ ». Il revient au même de dire que $(m) = \bigcap (x_i)$; en effet, la condition $x_i|z$ pour tout $i$ équivaut à $z \in Ax_i$ pour tout $i$, c’est-à-dire à $z \in \bigcap (x_i)$, et la condition $m|z$ équivaut à $z \in (m)$^1.

1 Lorsque $A$ est l’anneau des entiers (resp. l’anneau des polynômes à une indéterminée à coefficients dans un corps commutatif), ces définitions coïncident avec celles de I, p. 106 (resp. IV, p. 12, déf. 1).

On notera que si un idéal principal fractionnaire $(d)$ est tel que $(d) = \sum_i (x_i)$, $d$ est un pgcd de la famille $(x_i)$; mais inversement, un pgcd de $(x_i)$ ne vérifie pas nécessairement la condition précédente (cf. VI, p. 32, exerc. 24).

Le pgcd et le ppcm, s’ils existent, sont définis modulo le sous-groupe U des unités de $\mathbf{K}^*$, c’est-à-dire que deux pgcd (ou deux ppcm) d’une famille donnée sont associés; par abus de langage on écrira souvent $\operatorname{pgcd}(x_i)$ et $\operatorname{ppcm}(x_i)$ pour l’un quelconque des pgcd ou des ppcm de la famille $(x_i)$ lorsque de tels éléments existent.

(DIV) Par abus de langage on étend parfois la notion de pgcd à une famille $(x_i)$ d’éléments de K dont certains peuvent être nuls; ce pgcd est encore défini comme un élément $d$ de K tel que la relation $z|d$ soit équivalente à «$z|x_i$ pour tout i»; il est clair que $d$ est 0 si tous les $x_i$ sont nuls; dans le cas contraire, $d$ est un pgcd de la famille de ceux des $x_i$ qui ne sont pas nuls. De même le ppcm d’une famille dont certains éléments sont nuls est 0.

Dans un groupe ordonné G, il résulte aussitôt de l’invariance de l’ordre par translation (VI, p. 2, prop. 2) que l’on a :

$$
\sup(z + x_i) = z + \sup(x_i)
$$

en ce sens que, chaque fois que l’un des deux membres existe, l’autre existe aussi et lui est égal. De même, du fait que l’application $x \mapsto -x$ transforme l’ordre de G en l’ordre opposé (VI, p. 2, cor.) il résulte que l’on a

$$
\inf(-x_i) = - (\sup(x_i)),
$$

cette relation étant entendue dans le même sens que la précédente.

#### Proposition 6 {#alg-vi-s1-prop-6 .statement}

Soient $(x_\alpha)_{\alpha \in A}$, $(y_\beta)_{\beta \in B}$ deux familles d’éléments d’un groupe ordonné G, ayant chacune une borne supérieure. Alors la famille $(x_\alpha + y_\beta)_{(\alpha, \beta) \in A \times B}$ a une borne supérieure, et l’on a $\sup_{(\alpha, \beta) \in A \times B} (x_\alpha + y_\beta) = \sup_{\alpha \in A} x_\alpha + \sup_{\beta \in B} y_\beta$.

En effet, de $x_\alpha + y_\beta \leq z$ pour tout $\alpha$ et tout $\beta$, on déduit $\sup(x_\alpha) + y_\beta \leq z$ pour tout $\beta$, et de là $\sup(x_\alpha) + \sup(y_\beta) \leq z$.

### 9. Groupes réticulés

Rappelons qu’un ensemble ordonné dans lequel toute partie finie non vide a une borne supérieure et une borne inférieure est dit réticulé (E, III, p. 13). Il est clair qu’un produit de groupes réticulés, et en particulier un produit de groupes totalement ordonnés, est un groupe réticulé. Par contre un sous-groupe d’un groupe réticulé n’est pas nécessairement réticulé.

Ainsi, dans le groupe ordonné produit $\mathbf{Z} \times \mathbf{Z}$, la « seconde bissectrice » (ensemble des couples $(n, n')$ tels que $n + n' = 0$) est ordonnée par l’ordre discret, et n’est donc pas un groupe réticulé. \* Le groupe additif des polynômes à une variable réelle (VI, p. 1, exemple 2) est un groupe filtrant (puisque $p(x)$ et $q(x)$ sont majorés par $(p(x))^2 + (q(x))^2 + 1$) dont on peut montrer qu’il n’est pas réticulé. \*

#### Proposition 7 {#alg-vi-s1-prop-7 .statement}

Si x et y sont deux éléments d’un groupe ordonné G, et si l’un des éléments inf(x, y), sup(x, y) existe, il en est de même de l’autre, et l’on a x + y = inf(x, y) + sup(x, y).

En effet, d’après les relations (1) et (2) (VI, p. 9), on a

$$
\sup(a - x, a - y) = a + \sup(-x, -y) = a - \inf(x, y),
$$

et il suffit de prendre $a = x + y$.

#### Proposition 7 {#alg-vi-s1-div-prop-7 .statement}

Si $a, b \in \mathbf{K}^*$, et si d est un pgcd de a et b et m un ppcm de a et b, alors le produit dm est associé à ab.

#### Proposition 8 {#alg-vi-s1-prop-8 .statement}

Soit P l’ensemble des éléments positifs d’un groupe ordonné G. Pour que G soit réticulé, il faut et il suffit que l’on ait $G = P - P$, et que de plus P, muni de l’ordre induit, satisfasse à l’une ou l’autre des conditions suivantes :

a) Tout couple d’éléments de P a une borne supérieure dans P.
b) Tout couple d’éléments de P a une borne inférieure dans P.

La nécessité de ces conditions est évidente : en effet la relation $G = P - P$ exprime que G est filtrant (VI, p. 4, prop. 4) ; d’autre part les bornes inférieure et supérieure dans G de deux éléments de P sont positives, donc sont aussi leurs bornes dans P.

Réciproquement, remarquons d’abord que dans l’hypothèse a) (resp. b)), tout couple d’éléments x, y de P a une borne supérieure (resp. inférieure) dans G égale à sa borne supérieure a (resp. à sa borne inférieure b) dans P. Ceci est évident pour a, tout majorant de x et y étant positif ; pour b, soit $z \in G$ un minorant de x et y ; il existe alors $u \in P$ tel que $z + u \in P$, puisque $G = P - P$ ; or $\inf_P(x + u, y + u)$ majore $b + u$, et est donc de la forme $b + c + u$ ($c \geqslant 0$) ; comme $b + c$ est inférieur à x et à y, on a $c = 0$ ; donc $\inf_P(x + u, y + u) = b + u$, ce qui implique $z + u \leqslant b + u$, donc $z \leqslant b$, et b est bien la borne inférieure de x et y dans G. Si maintenant x et y sont des éléments quelconques de G, nous les translaterons dans P : soit $v \in P$ tel que $x + v$ et $y + v$ soient positifs (VI, p. 4, prop. 5) ; dans l’hypothèse a) (resp. b)) $x + v$ et $y + v$ admettent une borne supérieure (resp. inférieure) dans P, donc aussi dans G d’après ce qui vient d’être vu ; par translation x et y admettent une borne supérieure (resp. inférieure) dans G ; l’existence d’une des deux espèces de bornes pour tout couple (x, y) entraînant celle de l’autre en vertu de la prop. 7, ceci montre que les conditions sont suffisantes.

### 10. Le théorème de décomposition

#### Théorème 1 (théorème de décomposition) {#alg-vi-s1-thm-1 .statement}

Soient $(x_i)_{1 \leq i \leq p}$ et $(y_j)_{1 \leq j \leq q}$ deux suites finies d’éléments positifs d’un groupe réticulé G telles que $\sum_{i=1}^p x_i = \sum_{j=1}^q y_j$; il existe alors une suite double $(z_{ij})_{1 \leq i \leq p, 1 \leq j \leq q}$ d’éléments positifs de G telle que l’on ait $x_i = \sum_{j=1}^q z_{ij}$ pour tout i, et $y_j = \sum_{i=1}^p z_{ij}$ pour tout j.

1° Démontrons d’abord le théorème lorsque $p = q = 2$. Soient $x, x', y, y'$ des éléments positifs de $G$ tels que $x + x' = y + y'$, et posons $a = \sup(0, x - y')$. Comme
$$
x - y' = y - x'
$$
est inférieur à $x$ et $y$, $b = x - a$ et $c = y - a$ sont positifs, ainsi que $d = a - (x - y')$. Et l’on a $x = a + b, x' = c + d, y = a + c$ et $y' = b + d$.

2° Montrons maintenant que, si le théorème est vrai pour $p < m$ et $q = n$ ($m > 2, n \geq 2$) il est vrai pour $p = m$ et $q = n$. On a par hypothèse l’égalité
$$
x_m + \sum_{i=1}^{m-1} x_i = \sum_{j=1}^n y_j.
$$
Le théorème étant vrai pour $p = 2$ et $q = n$, il existe deux suites finies $(z'_j), (z''_j)$ de $n$ termes positifs telles que $\sum_{i=1}^{m-1} x_i = \sum_{j=1}^n z'_j, x_m = \sum_{j=1}^n z''_j$, et $y_j = z'_j + z''_j$ pour $1 \leq j \leq n$. D’autre part, le théorème étant vrai pour $p = m - 1$ et $q = n$, il existe une suite double $(u_{ij})_{1 \leq i \leq m-1, 1 \leq j \leq n}$ telle que $x_i = \sum_{j=1}^n u_{ij}$ pour $1 \leq i \leq m - 1$, et $z'_j = \sum_{i=1}^{m-1} u_{ij}$ pour $1 \leq j \leq n$. En posant
$$
z_{ij} = u_{ij} \text{ pour } 1 \leq i \leq m - 1, \text{ et } z_{mj} = z''_j \quad (1 \leq j \leq n),
$$
on obtient bien une suite double satisfaisant aux conditions du théorème.

3° En échangeant les rôles des $x_i$ et des $y_j$ on voit de même que, si le théorème est vrai pour $p = m$ et $q < n$ ($m \geq 2, n > 2$), il est vrai pour $p = m$ et $q = n$. Le théorème est donc démontré par double récurrence à partir du cas $p = q = 2$, puisqu’il est trivial lorsque $p \leq 1$ ou $q \leq 1$.

#### Corollaire {#alg-vi-s1-n10-cor-1 .statement}

*Soient* $y, x_1, x_2, ..., x_n, n + 1$ *éléments positifs de* $G$ *tels que* $y \leq \sum_{i=1}^n x_i ;$ *il existe alors* $n$ *éléments positifs* $y_i$ *$(1 \leq i \leq n)$ tels que* $y_i \leq x_i$ *et*
$$
y = \sum_{i=1}^n y_i.
$$
Il suffit d’appliquer le th. 1 à la suite $(x_i)$ et à la suite formée des deux éléments $y$ et $z = (\sum_{i=1}^n x_i) - y$.

### 11. Partie positive et partie négative

#### Définition 4 {#alg-vi-s1-def-4 .statement}

*Dans un groupe réticulé* $G$ *on appelle partie positive* (resp. *partie négative, valeur absolue*) *d’un élément* $x \in G$, *et on note* $x^+$ (resp. $x^-$, $|x|$) *l’élément* $\sup(x, 0)$ (resp. $\sup(-x, 0)$, $\sup(x, -x)$).

Malgré son nom, la partie négative $x^-$ de $x$ est un élément *positif*.

Il est clair que l’on a $x^- = (-x)^+$ et $|-x| = |x|$. Notons aussi les formules suivantes, dont la première est conséquence immédiate des définitions et de l’invariance de l’ordre par translation, et dont la seconde se déduit de la première au moyen de la prop. 7 de VI, p. 10 :

$$
\left\{
\begin{array}{l}
\sup(x, y) = x + (y - x)^+ , \\
\inf(x, y) = y - (y - x)^+ .
\end{array}
\right.
$$

#### Proposition 9 {#alg-vi-s1-prop-9 .statement}

a) Pour tout élément $x$ d’un groupe réticulé $G$, on a $x = x^+ - x^-$ et $\inf(x^+, x^-) = 0$.

b) Pour toute expression de $x$ comme différence de deux éléments positifs, $x = u - v$, on a $u = x^+ + w$ et $v = x^- + w$ avec $w = \inf(u, v)$. Si, en particulier, $\inf(u, v) = 0$, on a $u = x^+$ et $v = x^-$.

c) La relation « $x \leq y$ » est équivalente à « $x^+ \leq y^+$ et $x^- \geq y^-$ ».

d) On a $|x| = x^+ + x^- \geq 0$.

e) Quels que soient $x$ et $y$ dans $G$, on a l’inégalité $|x + y| \leq |x| + |y|$, et plus généralement $\left| \sum_{i=1}^n x_i \right| \leq \sum_{i=1}^n |x_i|$ pour toute famille finie $(x_i)$ d’éléments de $G$.

f) Quels que soient $x$ et $y$ dans $G$, on a $||x| - |y|| \leq |x - y|$.

Nous démontrerons a) et b) simultanément. Si $x = u - v$, avec $u$ et $v$ positifs, on a $u \geq x$, donc $u \geq \sup(x, 0) = x^+$, et $w = u - x^+$ est positif. D’autre part on a
$$
x^+ - x = \sup(x, 0) - x = \sup(x - x, - x) = x^-
$$
d’où résulte $x = x^+ - x^-$, et $v - x^- = w$. De $z \leq x^-$, on tire $z \leq x^+ - x$, et $x \leq x^+ - z$; si de plus $z \leq x^+$, $x^+ - z$ est positif, d’où on tire $x^+ \leq x^+ - z$ en vertu de la définition de $x^+$. On a donc $z \leq 0$, ce qui entraîne $\inf(x^+, x^-) = 0$, d’où, par translation, $\inf(u, v) = w$.

c) La relation $x \leq y$ entraîne $\sup(y, 0) \geq x$ et $\sup(y, 0) \geq 0$, d’où $x^+ \leq y^+$; de $-y \leq -x$ on déduit de même $x^- \geq y^-$. L’implication inverse se déduit aussitôt de $x = x^+ - x^-$ et $y = y^+ - y^-$.

d) Comme $x \leq x^+$ et $-x \leq x^-$, il est clair que
$$
|x| = \sup(x, -x) \leq x^+ + x^- .
$$

Inversement, de $a \geq x$ et $a \geq -x$, on déduit, en vertu de c), $a^+ \geq x^+$, $a^+ \geq x^-$, $a^- \leq x^-$ et $a^- \leq x^+$; comme $a^-$ est positif et que $\inf(x^+, x^-) = 0$, les deux dernières inégalités entraînent $a^- = 0$ et $a = a^+$; les deux premières donnent alors $a \geq \sup(x^+, x^-)$, élément qui est égal à $x^+ + x^-$ en vertu de a) et de la prop. 7 de VI, p. 10.

e) De $x \leq |x|$ et $y \leq |y|$, on tire $x + y \leq |x| + |y|$; de $-x \leq |x|$ et $-y \leq |y|$, on tire $-x - y \leq |x| + |y|$; d’où la première inégalité. La seconde s’en déduit par récurrence sur $n$.

f) En remplaçant dans e) $x$ et $y$ par $y$ et $x - y$, il vient
$$
|x| - |y| \leq |x - y| ;
$$
on a de même $|y| - |x| \leq |y - x| = |x - y|$; d’où le résultat annoncé.

#### Remarque {#alg-vi-s1-n11-rem-1 .statement}

On déduit de d) que $|x| = 0$ entraîne $x = 0$ (car $x^+$ et $x^-$ sont positifs); donc $x \neq 0$ entraîne $|x| > 0$.

#### Proposition 9 {#alg-vi-s1-div-prop-9 .statement}

Si le groupe $\mathcal{P}^*$ des idéaux principaux fractionnaires de $K$ est réticulé, tout élément $x$ de $K^*$ peut être mis sous la forme $x = uv^{-1}$, où $u$ et $v$ sont des éléments de $A$ tels que $1 = \operatorname{pgcd}(u, v)$; pour toute autre expression $x = u'{v'}^{-1}$ de $x$ comme quotient de deux éléments de $A$, on a $u' = uw, v' = vw$, où $w \in A$ est un pgcd de $u'$ et $v'$; en particulier si $1 = \operatorname{pgcd}(u', v')$, $u'$ et $v'$ sont respectivement associés à $u$ et $v$.

Une telle expression $uv^{-1}$ d’un élément $x$ de $K^*$ est souvent appelée une fraction irréductible.

### 12. Éléments étrangers

#### Définition 5 {#alg-vi-s1-def-5 .statement}

Dans un groupe ordonné, deux éléments $x$ et $y$ sont dits étrangers si l’on a $\inf(x, y) = 0$.

On est conduit, dans certains cas, à appeler étrangers deux éléments tels que $\inf(|x|, |y|) = 0$ (cf. INT, II, § 1), ou à introduire la terminologie correspondante en théorie de la divisibilité. Nous ne le ferons pas ici.

Deux éléments étrangers sont nécessairement positifs. Les parties positive et négative $x^+$ et $x^-$ de $x$ sont des éléments étrangers (VI, p. 12, prop. 9, a)). On dit que les éléments $x_i$ d’une famille $(x_i)_{i \in I}$ sont étrangers dans leur ensemble si l’on a $\inf x_i = 0$; si les $x_i$ sont $\geqslant 0$, il suffit pour cela qu’il existe une partie finie $J$ de $I$ telle que les éléments correspondants soient étrangers dans leur ensemble. Les éléments d’une famille $(x_i)$ sont dits étrangers deux à deux si l’on a $\inf(x_i, x_x) = 0$ pour tout couple $(i, x)$ d’indices distincts.

Les $x_i$ peuvent être étrangers dans leur ensemble sans être étrangers deux à deux.

Si $x$ et $y$ sont étrangers, on dit aussi que $x$ est étranger à $y$, ou que $y$ est étranger à $x$.

(DIV) On dit que deux éléments $x$ et $y$ de $K$ sont étrangers si les idéaux principaux $(x)$ et $(y)$ sont non nuls et étrangers dans $\mathcal{P}^*$; ceci revient à dire que $1$ est un pgcd de $x$ et $y$, et implique que $x$ et $y$ appartiennent à $A$. Par exemple le numératuer et le dénominateur d’une fraction irréductible sont étrangers. On définit de même les notions d’éléments étrangers deux à deux, et d’éléments étrangers dans leur ensemble.

(DIV) On dit souvent, quand $x$ et $y$ sont étrangers, que $x$ et $y$ sont « premiers entre eux »; il convient d’éviter cette terminologie, qui entraîne confusion avec la notion d’entier premier (I, p. 48, déf. 16).

#### Proposition 10 {#alg-vi-s1-prop-10 .statement}

Soient x, y, z trois éléments d’un groupe ordonné ; pour que x − z et y − z soient étrangers, il faut et il suffit que l’on ait z = inf(x, y).
En effet les relations z = inf(x, y) et 0 = inf(x − z, y − z) sont équivalentes.

#### Proposition 10 {#alg-vi-s1-div-prop-10 .statement}

Soient a, b, c trois éléments de K tels que c ≠ 0 ; pour que les quotients ac−1 et bc−1 soient étrangers, il faut et il suffit que c soit un pgcd de a et de b.

#### Proposition 11 {#alg-vi-s1-prop-11 .statement}

Si (x_i), (y_j) sont deux familles finies d’éléments ≥ 0 d’un groupe réticulé, on a
$$
\inf(\sum_i x_i, \sum_j y_j) \leq \sum_{i,j} \inf(x_i, y_j).
$$
Raisonnant par récurrence sur le nombre d’éléments des familles (x_i) et (y_j), il suffit de prouver que si x, y, z sont des éléments ≥ 0, on a
$$
\inf(x, y + z) \leq \inf(x, y) + \inf(x, z).
$$
En effet, posons t = inf(x, y + z) ; en vertu de VI, p. 11, cor., on peut écrire t = t_1 + t_2 avec 0 ≤ t_1 ≤ y et 0 ≤ t_2 ≤ z ; comme t_1 et t_2 sont positifs, on a aussi t_1 ≤ x et t_2 ≤ x, d’où t_1 ≤ inf(x, y) et t_2 ≤ inf(x, z).

#### Corollaire 1 {#alg-vi-s1-prop-11-cor-1 .statement}

Si x et y sont deux éléments étrangers et z un élément ≥ 0 d’un groupe réticulé, on a inf(x, z) = inf(x, y + z).

En effet, inf(x, y + z) ≤ inf(x, z) en vertu de la prop. 11, et comme y ≥ 0, inf(x, z) ≤ inf(x, y + z), d’où le corollaire.

#### Corollaire 2 {#alg-vi-s1-prop-11-cor-2 .statement}

Dans un groupe réticulé, si x et y sont étrangers et si on a z ≥ 0 et x ≤ y + z, alors on a x ≤ z.

#### Corollaire 3 {#alg-vi-s1-prop-11-cor-3 .statement}

Dans un groupe réticulé, si x est étranger à y et z, il l’est aussi à y + z.

#### Corollaire 4 {#alg-vi-s1-prop-11-cor-4 .statement}

Si (x_i)_{1 ≤ i ≤ n}, (y_j)_{1 ≤ j ≤ m} sont deux familles finies d’éléments d’un groupe réticulé G telles que chacun des x_i soit étranger à chacun des y_j, alors x_1 + ⋯ + x_n est étranger à y_1 + ⋯ + y_m.
Ceci se déduit du cor. 3 par récurrence sur m et n.

#### Corollaire 5 {#alg-vi-s1-prop-11-cor-5 .statement}

Quel que soit l’entier n ≥ 0, on a (nx)^+ = nx^+ et (nx)^- = nx^- ; pour tout n ∈ \mathbf{Z}, on a |nx| = |n|.|x|.
On a en effet nx = nx^+ − nx^- ; comme x^+ et x^- sont étrangers, il en est de même de nx^+ et nx^- si n ≥ 0 (cor. 4) ; d’où la première assertion en vertu de la prop. 9, b) de VI, p. 12. La seconde s’ensuit en vertu de la prop. 9, d) dans le cas n ≥ 0 ; on passe de là au cas n < 0 grâce à la relation |− x| = |x|.

#### Proposition 11 {#alg-vi-s1-div-prop-11 .statement}

L’ensemble $\mathcal{P}^*$ étant supposé réticulé, soient $(a_i), (b_j)$ deux familles finies d’éléments de $\mathbf{A}$. Alors tout pgcd de $\prod_i a_i$ et de $\prod_j b_j$ divise le produit $\prod_{i,j} \operatorname{pgcd}(a_i, b_j)$.

#### Corollaire 1 {#alg-vi-s1-div-prop-11-cor-1 .statement}

Si $a, b, c$ sont trois éléments de $\mathbf{A}$ tels que $a$ soit étranger à $b$, tout pgcd de $a$ et de $c$ est aussi un pgcd de $a$ et de $bc$.

#### Corollaire 2 (lemme d’Euclide) {#alg-vi-s1-div-prop-11-cor-2 .statement}

Soient $a, b, c$ trois éléments de $\mathbf{A}$. Si $a$ est étranger à $b$ et divise $bc$, il divise $c$.

#### Corollaire 3 {#alg-vi-s1-div-prop-11-cor-3 .statement}

Si $x$ est étranger à $y$ et $z$, il l’est à $yz$.

#### Corollaire 4 {#alg-vi-s1-div-prop-11-cor-4 .statement}

Si $(x_i)$ et $(y_j)$ sont deux familles finies d’éléments de $\mathbf{A}$ telles que chaque $x_i$ soit étranger à chaque $y_j$, alors le produit des $x_i$ est étranger au produit des $y_j$.

#### Corollaire 5 {#alg-vi-s1-div-prop-11-cor-5 .statement}

Si $d$ est un pgcd de $x$ et $y$, $d^n$ est un pgcd de $x^n$ et $y^n$ pour tout entier positif $n$.
En effet $xd^{-1}$ et $yd^{-1}$ sont étrangers (prop. 10 (DIV)), et il en est de même de $x^n d^{-n}$ et $y^n d^{-n}$ (cor. 4).

#### Proposition 12 {#alg-vi-s1-prop-12 .statement}

Soient $x_i$ ($1 \leq i \leq n$) $n$ éléments étrangers deux à deux dans un groupe réticulé. Alors

$$
\sup(x_1, ..., x_n) = x_1 + \cdots + x_n.
$$

Ceci se déduit de la formule $u + v = \sup(u, v) + \inf(u, v)$ (VI, p. 10, prop. 7) par récurrence sur $n$, en tenant compte de ce que $x_i$ est étranger à $x_1 + \cdots + x_{i-1}$ pour $2 \leq i \leq n$ (cor. 4 de la prop. 11).

#### Remarque {#alg-vi-s1-n12-rem-1 .statement}

La prop. 7 de VI, p. 10 montre aussi que, pour que $x$ et $y$ soient étrangers, il faut et il suffit que l’on ait $x + y = \sup(x, y)$.

#### Proposition 12 {#alg-vi-s1-div-prop-12 .statement}

Soient $a_i$ des éléments de $\mathbf{A}$ en nombre fini $n$ et étrangers deux à deux ; alors le produit $a_1 \ldots a_n$ est un ppcm de $a_1, ..., a_n$.

#### Proposition 13 {#alg-vi-s1-prop-13 .statement}

Dans un groupe réticulé $\mathbf{G}$, soit $(x_\alpha)$ une famille admettant une borne inférieure (resp. supérieure), et soit $z$ un élément quelconque de $\mathbf{G}$; alors la famille $(\sup(z, x_\alpha))$ (resp. $(\inf(z, x_\alpha))$) admet une borne inférieure (resp. supérieure) et l’on a respectivement

$$
\begin{cases}
\inf(\sup(z, x_\alpha)) = \sup(z, \inf x_\alpha) \\
\sup(\inf(z, x_\alpha)) = \inf(z, \sup x_\alpha)
\end{cases}
$$

Supposons que la famille $(x_\alpha)$ admette une borne inférieure $y$ et démontrons que $\sup(z, y)$ est une borne inférieure de la famille $(\sup(z, x_\alpha))$.

On a en effet $\sup(z, x_\alpha) = z + (x_\alpha - z)^+$, et, par translation, nous sommes ramenés au cas $z = 0$, c’est-à-dire qu’il nous faut montrer que la famille $(x_\alpha^+)$ admet une borne inférieure qui est $y^+$. Comme on a $y \leq x_\alpha$, on a $y^+ \leq x_\alpha^+$ pour tout $\alpha$ (VI, p. 12, prop. 9, c)). Si, inversement, on a $a \leq x_\alpha^+$ pour tout $\alpha$, on en déduit $a \leq x_\alpha + x_\alpha^-$ (prop. 9, a)); or, de $y \leq x_\alpha$, on déduit $y^- \geq x_\alpha^-$; on a donc $a \leq x_\alpha + y^-$ pour tout $\alpha$, c’est-à-dire $a \leq y + y^- = y^+$.

L’autre formule s’en déduit par passage à la relation d’ordre opposée.

#### Corollaire {#alg-vi-s1-n12-cor-1 .statement}

*Si, dans un groupe réticulé G, un élément z est étranger à chacun des éléments $x_\alpha$ d’une famille admettant une borne supérieure y, alors z est étranger à y.*

Ceci est conséquence immédiate de la seconde formule (4).

#### Remarque {#alg-vi-s1-n12-rem-2 .statement}

En appliquant les formules de la prop. 13 à une famille de deux éléments $(x, y)$, on obtient les formules suivantes qui expriment que, dans un groupe réticulé, chacune des lois de composition sup, inf est *distributive* par rapport à l’autre :

$$
\begin{align*}
\sup(z, \inf(x, y)) &= \inf(\sup(z, x), \sup(z, y)) \\
\inf(z, \sup(x, y)) &= \sup(\inf(z, x), \inf(z, y)).
\end{align*}
$$

Cette propriété de distributivité est spéciale aux *groupes* réticulés et ne s’étend ni aux ensembles, ni même aux monoïdes réticulés (*cf.* VI, p. 32, exerc. 24).

### 13. Éléments extrémaux

#### Définition 6 {#alg-vi-s1-def-6 .statement}

*On dit qu’un élément x d’un groupe ordonné G est extrémal si c’est un élément minimal de l’ensemble des éléments strictement positifs de G.*

Soit $x$ un élément extrémal du groupe ordonné $G$; si $y$ est un élément positif de $G$, l’élément $\inf(x, y)$, s’il existe, ne peut donc être égal qu’à $x$ ou à 0. Ainsi, dans un groupe réticulé $G$, tout $y$ positif est, soit supérieur, soit étranger à l’élément extrémal $x$; en particulier deux éléments extrémaux distincts sont étrangers.

(DIV) Un élément $p$ de $A$ est dit *extrémal* si l’idéal $(p)$ est un élément extrémal du groupe ordonné $\mathcal{P}^*$; ceci exprime que $p$ n’est ni nul, ni inversible, et que tout élément de $A$ qui divise $p$ est associé, soit à $p$, soit à 1. Si $\mathcal{P}^*$ est réticulé, tout $a \in A$ est, soit étranger à $p$, soit multiple de $p$.

*Exemples* (DIV). — 1) Un entier $p > 0$ est extrémal dans $\mathbf{Z}$ si et seulement s’il est *premier* (I, p. 48).
2) Un polynôme à une indéterminée sur un corps $K$ est extrémal dans l’anneau $K[X]$ si et seulement s’il est *irréductible* (IV, p. 13).

#### Proposition 14 {#alg-vi-s1-prop-14 .statement}

*Pour qu’un élément $x > 0$ d’un groupe ordonné G soit extrémal, il suffit qu’il possède la propriété suivante :*
(P) *Les relations* $x \leq y + z,\ y \geq 0,\ z \geq 0$ *entraînent* $x \leq y$ *ou* $x \leq z$.
*Cette condition est nécessaire lorsque* G *est réticulé*.

Si G est réticulé et si x est extrémal, nous venons de voir que y est, soit supérieur à x, soit étranger à x ; dans ce dernier cas le cor. 2 de VI, p. 14 montre que z est supérieur à x. Réciproquement, supposons la condition satisfaite : de $0 \leq y \leq x$, on déduit, en posant $x = y + z$ ($z \geq 0$) que l’on a, soit $x \leq y$, soit $x \leq z$; dans le premier cas on a $x = y$; dans le second on a $x \leq x - y$, donc $y \leq 0$ et par suite $y = 0$; ceci montre que x est bien extrémal.

#### Proposition 14 {#alg-vi-s1-div-prop-14 .statement}

Pour qu’un élément p non nul de A soit extrémal, il suffit qu’il ne soit pas une unité, et qu’il ne puisse diviser un produit de deux éléments de A sans diviser l’un d’eux. Cette condition est nécessaire si $\mathcal{P}^*$ est réticulé.

#### Remarque {#alg-vi-s1-n13-rem-1 .statement}

On peut aussi exprimer la proposition 14 (DIV) comme suit : si p est un élément non nul de A tel que l’idéal (p) soit premier (I, p. 111, déf. 3), alors p est extrémal ; inversement, si $\mathcal{P}^*$ est réticulé et p extrémal, l’idéal (p) est premier.

#### Proposition 15 {#alg-vi-s1-prop-15 .statement}

Dans un groupe ordonné G, soit $(p_i)_{i \in I}$ une famille d’éléments $> 0$ deux à deux distincts et vérifiant la propriété (P) (donc extrémaux). Alors l’application

$$
(n_i)_{i \in I} \mapsto \sum_{i \in I} n_i p_i
$$

est un isomorphisme du groupe ordonné $\mathbf{Z}^{(I)}$, somme directe des groupes ordonnés $\mathbf{Z}$ (VI, p. 7), sur le sous-groupe ordonné de G engendré par les $p_i$.

Il suffit de montrer que la relation $\sum_{i \in I} n_i p_i \geq 0$ est équivalente à $n_i \geq 0$ pour tout $i \in I$, car en particulier la relation $\sum_{i \in I} n_i p_i = 0$ entraînera $n_i = 0$ pour tout $i \in I$, donc cela montrera que la famille $(p_i)$ est libre. Or, soit $I'$ (resp. $I''$) la partie finie de I formée des $i$ tels que $n_i > 0$ (resp. $n_i < 0$); on a

$$
\sum_{i \in I'} n_i p_i \geq \sum_{i \in I''} (-n_i) p_i .
$$

En particulier, pour $\lambda \in I''$, cela entraîne $p_\lambda \leq \sum_{i \in I'} n_i p_i$, et, par récurrence, il résulte de la propriété (P) que l’on doit avoir $p_\lambda \leq p_i$ pour un $i \in I'$; comme $p_i$ est extrémal, cela entraînerait $p_\lambda = p_i$, ce qui est absurde. Donc $I''$ est vide, ce qui prouve la proposition.

#### Théorème 2 {#alg-vi-s1-thm-2 .statement}

Soit G un groupe ordonné filtrant. Les propriétés suivantes sont équivalentes :
a) G est isomorphe à un groupe ordonné de la forme $\mathbf{Z}^{(I)}$.
b) G est réticulé et vérifie la condition suivante :
(MIN) Tout ensemble non vide d’éléments positifs de G admet un élément minimal.
c) G vérifie la condition (MIN) et tout élément extrémal de G possède la propriété (P).
d) G est engendré par ses éléments extrémaux et tout élément extrémal de G possède la propriété (P).

Montrons d’abord que a) entraîne b). Le groupe $\mathbf{Z}^{(l)}$ est réticulé, en tant que somme directe de groupes totalement ordonnés. Soit d’autre part E un ensemble non vide d’éléments positifs de $\mathbf{Z}^{(l)}$, et soit $x = \sum n_i e_i$ un élément de E (($e_i$) désignant la base canonique de $\mathbf{Z}^{(l)}$); les éléments $y$ de $\mathbf{Z}^{(l)}$ tels que $0 \leq y \leq x$ sont en nombre fini égal à $\prod (n_i + 1)$, donc l’ensemble F des éléments de E qui sont $\leq x$ est $a fortiori$ fini ; comme il n’est pas vide, il contient un élément minimal (E, III, p. 34, cor. 2), qui est évidemment élément minimal de E.

Il est clair que b) entraîne c), en vertu de la prop. 14. Montrons que c) entraîne d). Comme G est filtrant, il suffit (VI, p. 4, prop. 4) de voir que l’ensemble F des éléments $> 0$ de G qui sont sommes d’éléments extrémaux est égal à $G_+ - \{0\}$. Sinon, il résulterait de (MIN) que le complémentaire de F dans $G_+ - \{0\}$ aurait un élément minimal $a$; $a$ n’est pas extrémal par définition, donc est somme de deux éléments positifs $x, y$ non nuls ; comme $x < a$ et $y < a$, ces éléments appartiennent à F, donc sont sommes d’éléments extrémaux, et on en déduit qu’il en est de même de $a$, ce qui est contradictoire. Enfin, d) entraîne a), en vertu de la prop. 15.

Nous appliquerons le th. 2 à la théorie de la divisibilité dans les anneaux principaux (VII, p. 3), et dans les anneaux factoriels (AC, VII, § 3), ainsi qu’à l’étude des idéaux d’un anneau de Dedekind (AC, VII, § 2).

## EXERCICES {#alg-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
