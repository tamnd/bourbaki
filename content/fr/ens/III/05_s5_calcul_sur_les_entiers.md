---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ENSEMBLES ORDONNÉS, CARDINAUX, NOMBRES ENTIERS
section: 5
section_title: Calcul sur les entiers
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E III.35-E III.44, E III.83-E III.87
pdf_pages: 0139-0148, 0187-0191
extraction: ocr
subsections:
    - "no": 1
      title: Opérations sur les entiers et les ensembles finis
      page: 35
      pdf_page: 139
    - "no": 2
      title: Inégalités strictes entre entiers
      page: 36
      pdf_page: 140
    - "no": 3
      title: Intervalles dans les ensembles d’entiers
      page: 37
      pdf_page: 141
    - "no": 4
      title: Suites finies
      page: 0
      pdf_page: 142
    - "no": 5
      title: Fonctions caractéristiques d’ensembles
      page: 0
      pdf_page: 142
    - "no": 6
      title: Division euclidienne
      page: 39
      pdf_page: 143
    - "no": 7
      title: Développement de base $ b $
      page: 40
      pdf_page: 144
    - "no": 8
      title: Analyse combinatoire
      page: 41
      pdf_page: 145
statements: 30
exercises: 18
content_sha256: 12f8e428428b5f7dc54975404f7164ebcd42072404d371fe2d384b67219ccb8d
---

## § 5. CALCUL SUR LES ENTIERS

### 1. Opérations sur les entiers et les ensembles finis

#### Proposition 1 {#ens-iii-s5-prop-1 .statement tag=03LP}

Soit $(a_i)_{i \in I}$ une famille finie d’entiers. Les cardinaux $\sum_{i \in I} a_i$ et $\prod_{i \in I} a_i$ sont alors des entiers.

Montrons d’abord que, si a et b sont des entiers, $a + b$ est un entier. Procédons par récurrence sur b. La proposition est vraie pour $b = 0$, car $a + 0 = a$. Si $a + b$ est entier, il en est de même de $(a + b) + 1$ (III, p. 31, prop. 1); mais $(a + b) + 1 = a + (b + 1)$ (III, p. 27, corollaire), donc $a + (b + 1)$ est entier, et par suite $a + b$ est un entier pour tout entier b.

Montrons maintenant, par récurrence sur $n = \mathrm{Card}\,(I)$, que $\sum_{i \in I} a_i$ est un entier. C’est évident si $n = 0$, car alors $I = \varnothing$ et $\sum_{i \in I} a_i = 0$. Si $\mathrm{Card}\,(I) = n + 1$, on a $I = J \cup \{k\}$, avec $\mathrm{Card}\,(J) = n$ et $k \notin J$; alors $\sum_{i \in I} a_i = a_k + \sum_{i \in J} a_i$ (III, p. 26, prop. 5). L’hypothèse de récurrence est que $\sum_{i \in J} a_i$ est un entier; il en est donc de même de $a_k + \sum_{i \in J} a_i$, d’après ce qui vient d’être démontré. Cela prouve que $\sum_{i \in I} a_i$ est entier pour tout $n$.

Comme le produit $ab$ de deux entiers a et b est la somme d’une famille finie d’entiers égaux à a (III, p. 27, cor. 2), $ab$ est un entier. Montrons, par récurrence sur $n = \mathrm{Card}\,(I)$, que $\prod_{i \in I} a_i$ est un entier. C’est vrai pour $n = 0$, car alors $\prod_{i \in I} a_i = 1$.

D'autre part, si Card (I) = n + 1, on a (avec les mêmes notations que ci-dessus),
$$
\prod_{i \in I} a_i = a_k \cdot \prod_{i \in J} a_i \quad (\text{III, p. 26, prop. 5}),
$$
donc l'hypothèse de récurrence entraîne que $\prod_{i \in I} a_i$ est un entier. Par suite, $\prod_{i \in I} a_i$ est un entier pour tout $n$.

#### Corollaire 1 {#ens-iii-s5-prop-1-cor-1 .statement tag=03LQ}

*La réunion E d'une famille finie* $(X_i)_{i \in I}$ *d'ensembles finis est un ensemble fini*.

En effet, l'ensemble somme S de la famille $(X_i)$ est fini. Comme il existe une application de S sur E (II, p. 30), l'ensemble E est fini (III, p. 32, cor. 3).

#### Corollaire 2 {#ens-iii-s5-prop-1-cor-2 .statement tag=03LR}

*Le produit d'une famille finie d'ensembles finis est un ensemble fini*.

#### Corollaire 3 {#ens-iii-s5-prop-1-cor-3 .statement tag=03LS}

*Si a et b sont des entiers, $a^b$ est un entier*.

En effet, $a^b$ est le produit d'une famille finie d'entiers égaux à $a$ (III, p. 28, prop. 10).

#### Corollaire 4 {#ens-iii-s5-prop-1-cor-4 .statement tag=03LT}

*L'ensemble des parties d'un ensemble fini E est fini*.

En effet, son cardinal est $2^{\text{Card}(E)}$ (III, p. 29, prop. 12).

### 2. Inégalités strictes entre entiers

#### Proposition 2 {#ens-iii-s5-prop-2 .statement tag=03LU}

*Soient a et b deux entiers ; pour que a < b, il faut et il suffit qu'il existe un entier c > 0 tel que b = a + c*.

En effet, si $a < b$, on sait qu'il existe un cardinal $c \leq b$ (qui est donc un entier (III, p. 31, prop. 2)) tel que $b = a + c$ (III, p. 29, prop. 13); si $a \neq b$, on a nécessairement $c \neq 0$. Inversement, si $b = a + c$ et $c \neq 0$, on a $c \geq 1$, donc $a < a + 1 \leq a + c = b$.

#### Proposition 3 {#ens-iii-s5-prop-3 .statement tag=03LV}

*Soient* $(a_i)_{i \in I}$ *et* $(b_i)_{i \in I}$ *deux familles finies d'entiers telles que* $a_i \leq b_i$ *pour tout* $i \in I$ *et* $a_i < b_i$ *pour un indice i au moins*. *On a alors* $\sum_{i \in I} a_i < \sum_{i \in I} b_i$. *Si on suppose de plus* $b_i > 0$ *pour tout* $i \in I$, *on a* $\prod_{i \in I} a_i < \prod_{i \in I} b_i$.

Soit $j$ un indice tel que $a_j < b_j$, et posons $J = I - \{j\}$. On a $b_j = a_j + c_j$ avec $c_j > 0$ (prop. 2), donc (III, p. 30, prop. 14)
$$
\sum_{i \in I} b_i = a_j + c_j + \sum_{i \in J} b_i \geq c_j + a_j + \sum_{i \in J} a_i = c_j + \sum_{i \in I} a_i
$$
et comme $c_j > 0$, on en déduit la première assertion (prop. 2). De même
$$
\prod_{i \in I} b_i = (a_j + c_j) \prod_{i \in J} b_i = a_j \prod_{i \in J} b_i + c_j \prod_{i \in J} b_i \geq \prod_{i \in I} a_i + c_j \prod_{i \in J} b_i;
$$
or, comme $c_j$ et tous les $b_i$ sont $\neq 0$, le produit $c_j \prod_{i \in J} b_i$ est $\neq 0$ (III, p. 28, prop. 7); la seconde assertion en résulte, compte tenu de la prop. 2.

#### Corollaire 1 {#ens-iii-s5-prop-3-cor-1 .statement tag=03LW}

Soient $a, a'$ et $b$ des entiers tels que $a < a'$ et $b > 0$; alors $a^b < a'^b$.

Il suffit d’exprimer $a^b$ et $a'^b$ comme produits de familles finies d’entiers (III, p. 28, prop. 10) et d’appliquer la prop. 3, en remarquant que la relation $a < a'$ implique $a' > 0$.

#### Corollaire 2 {#ens-iii-s5-prop-3-cor-2 .statement tag=03LX}

Soient $a, b$ et $b'$ des entiers tels que $a > 1$ et $b < b'$; on a alors $a^b < a^{b'}$.

En effet, il existe un entier $c > 0$ tel que $b' = b + c$ (prop. 2); comme $c \geqslant 1$, on a $a^c \geqslant a > 1$; d’où $a^{b'} = a^b a^c > a^b$.

#### Corollaire 3 {#ens-iii-s5-prop-3-cor-3 .statement tag=03LY}

Soient $a, b, b'$ des entiers (resp. des entiers tels que $a > 0$). Pour que l’on ait $a + b = a + b'$ (resp. $ab = ab'$), il faut et il suffit que l’on ait $b = b'$.

En effet, si $b \neq b'$, on a par exemple $b < b'$, et la prop. 3 montre que $a + b < a + b'$ et $ab < ab'$ (si $a > 0$).

#### Corollaire 4 {#ens-iii-s5-prop-3-cor-4 .statement tag=03LZ}

Si $a$ et $b$ sont des entiers tels que $a \leqslant b$, il existe un entier $c$ et un seul tel que $b = a + c$.

L’existence de $c$ résulte de la prop. 13 de III, p. 29, et son unicité du cor. 3 ci-dessus.

L’entier $c$ tel que $b = a + c$ (pour $a \leqslant b$) s’appelle la différence des entiers $b$ et $a$, et se note $b - a$. On vérifie aussitôt que, si $a, b, a', b'$ sont des entiers tels que $a \leqslant b$ et $a' \leqslant b'$, on a
$$(b - a) + (b' - a') = (b + b') - (a + a').$$

### 3. Intervalles dans les ensembles d’entiers

Tout ensemble d’entiers, étant un ensemble de cardinaux, est bien ordonné (III, p. 24, th. 1); en outre, pour tout entier $a$, la relation « $x$ est un cardinal et $x \leqslant a$ » est collectivisante (III, p. 25, Remarque), et l’ensemble des $x$ vérifiant cette relation est un ensemble d’entiers (III, p. 31, prop. 2) que l’on peut donc noter $\{0, a\}$.

#### Proposition 4 {#ens-iii-s5-prop-4 .statement tag=03M0}

Soient $a$ et $b$ des entiers; l’application $x \mapsto a + x$ est un isomorphisme strictement croissant de l’intervalle $[0, b]$ sur l’intervalle $[a, a + b]$, et $y \mapsto y - a$ est l’isomorphisme réciproque.

Il est clair que les relations $0 \leqslant x \leqslant b$ entraînent
$$a \leqslant a + x \leqslant a + b;$$
l’application $x \mapsto a + x$ est strictement croissante (donc injective) en raison de la prop. 3 de III, p. 36. Enfin, les relations $a \leqslant y \leqslant a + b$ entraînent $y = a + x$ avec $x \geqslant 0$ et $a + x \leqslant a + b$, d’où $x \leqslant b$ (III, p. 36, prop. 3), ce qui achève la démonstration.

#### Proposition 5 {#ens-iii-s5-prop-5 .statement tag=03M1}

Si $a$ et $b$ sont des entiers tels que $a \leq b$, l’intervalle $[a, b]$ est un ensemble fini dont le nombre d’éléments est $(b - a) + 1$.

En vertu de la prop. 4, on peut se limiter au cas où $a = 0$. Démontrons la proposition par récurrence sur $b$. Elle est évidente pour $b = 0$. D’autre part, la relation $0 \leq x \leq b + 1$ équivaut à « $0 \leq x < b + 1$ ou $x = b + 1$ » et la relation $0 \leq x < b + 1$ équivaut à $0 \leq x \leq b$ (III, p. 31, prop. 2); autrement dit, l’intervalle $[0, b + 1]$ est réunion de $[0, b]$ et de $\{b + 1\}$, et ces deux ensembles ne se rencontrent pas; en vertu de l’hypothèse de récurrence, le nombre d’éléments de $[0, b + 1]$ est égal à $(b + 1) + 1$, ce qui établit la proposition.

#### Proposition 6 {#ens-iii-s5-prop-6 .statement tag=03M2}

Pour tout ensemble fini $E$, totalement ordonné, ayant $n$ éléments ($n \geq 1$), il existe un isomorphisme et un seul de $E$ sur l’intervalle $[1, n]$.

Comme $E$ et $[1, n]$ sont bien ordonnés (III, p. 34, cor. 1), et ont même nombre d’éléments (prop. 5), la proposition résulte de III, p. 21, th. 3 et p. 31, cor. 2.

### 4. Suites finies

On appelle suite finie (resp. suite finie d’éléments d’un ensemble $E$) une famille (resp. une famille d’éléments de $E$) dont l’ensemble d’indices est un ensemble fini $I$ d’entiers; le nombre d’éléments de $I$ s’appelle alors la longueur de la suite.

Soit $(t_i)_{i \in I}$ une suite finie de longueur $n$. En vertu de la prop. 6, il existe un isomorphisme $f$ et un seul de l’intervalle $[1, n]$ sur l’ensemble d’entiers $I$. Pour tout $k \in [1, n]$, on dit que $t_{f(k)}$ est le $k$-ème terme de la suite; $t_{f(1)}$ (resp. $t_{f(n)}$) s’appelle le premier (resp. dernier) terme de la suite.

Soit $P \{ i \}$ une relation telle que les $i$ pour lesquels on a $P \{ i \}$ forment un ensemble fini $I$ d’entiers; une suite finie $(t_i)_{i \in I}$ se note alors souvent $(t_i)_{P \{ i \}}$. Par exemple, lorsque $I = [a, b]$, on emploie souvent la notation $(t_i)_{a \leq i \leq b}$. Dans les mêmes conditions, pour désigner, par exemple, le produit d’une famille d’ensembles $(X_i)_{i \in I}$, on utilise les notations $\prod_{P \{ i \}} X_i$ et $\prod_{i = a}^{b} X_i$; notations analogues pour la réunion, l’intersection, le produit cardinal, la somme cardinale, *les lois de composition en Algèbre (A, I, § 1)*, etc.

### 5. Fonctions caractéristiques d’ensembles

Soient $E$ un ensemble, $A$ une partie de $E$. On appelle fonction caractéristique de la partie $A$ de $E$ l’application $\varphi_A$ de $E$ dans l’ensemble $\{0, 1\}$ définie par les conditions:

$$
\varphi_A(x) = 1 \quad \text{pour } x \in A; \qquad \varphi_A(x) = 0 \quad \text{pour } x \in E - A.
$$

Il est immédiat que la relation $\varphi_A = \varphi_B$ équivaut à $A = B$; on a $\varphi_E(x) = 1$ pour tout $x \in E$, $\varphi_\emptyset(x) = 0$ pour tout $x \in E$ et ce sont les seules fonctions caractéristiques constantes dans $E$. En outre, la proposition suivante découle aussitôt des définitions:

#### Proposition 7 {#ens-iii-s5-prop-7 .statement tag=03M3}

*Pour tout couple de parties A, B d’un ensemble E, on a*

(1) $$
\varphi_{E-A}(x) = 1 - \varphi_A(x)
$$
(2) $$
\varphi_{A \cap B}(x) = \varphi_A(x)\varphi_B(x)
$$
(3) $$
\varphi_{A \cup B}(x) + \varphi_{A \cap B}(x) = \varphi_A(x) + \varphi_B(x)
$$

*pour tout* $x \in E$.

### 6. Division euclidienne

#### Théorème 1 {#ens-iii-s5-thm-1 .statement tag=03M4}

*Soient a et b des entiers tels que $b > 0$; il existe des entiers q et r tels que $a = bq + r$ et $r < b$, et les entiers q et r sont déterminés de façon unique par ces conditions.*

Les conditions imposées sont équivalentes à $bq \leq a < b(q + 1)$ et $r = a - bq$ (III, p. 36, prop. 2). Tout revient donc à trouver q tel que $bq \leq a < b(q + 1)$; autrement dit, q doit être le plus petit entier tel que $a < b(q + 1)$, ce qui montre que q et $r = a - bq$ sont déterminés de façon unique. Pour montrer leur existence, remarquons qu’il existe des entiers p tels que $a < bp$, ne serait-ce que $a + 1$, puisque $b > 0$. Soit m le plus petit de ces entiers; on a $m \neq 0$, et on peut donc écrire $m = q + 1$ avec $q \leq m$ (III, p. 31, prop. 2); il en résulte que $bq \leq a < b(q + 1)$.

#### Définition 1 {#ens-iii-s5-def-1 .statement tag=03M5}

*Les notations étant celles du th. 1, on dit que r est le reste de la division de a par b. Si $r = 0$, on dit que a est multiple de b, ou que a est divisible par b, ou que b est un diviseur de a, ou que b divise a; le nombre q s’appelle alors le quotient de a par b et se note $\frac{a}{b}$ ou $a/b$.*

Lorsque a n’est pas multiple de b, le nombre q s’appelle la *partie entière du quotient de a par b* (cf. TG, IV, § 8).

Dans ce chapitre, le seul fait d’écrire $a/b$ ou $\frac{a}{b}$ impliquera que b divise a.

Les relations $a = bq$ et $q = a/b$ sont équivalentes (si $b > 0$). Tout multiple $a'$ d’un multiple a de b est multiple de b, et l’on a $a'/b = (a'/a)(a/b)$ si $a \neq 0$. D’autre part, si c et d sont des multiples de b, $c + d$, et $c - d$ (lorsque $d \leq c$) sont des multiples de b, et l’on a

$$
\frac{c + d}{b} = \frac{c}{b} + \frac{d}{b} \quad \text{et} \quad \frac{c - d}{b} = \frac{c}{b} - \frac{d}{b}.
$$

Les entiers multiples de 2 sont dits *pairs*, les autres *impairs*; ces derniers sont de la forme $2n + 1$, d’après le th. 1.

### 7. Développement de base $b$

#### Proposition 8 {#ens-iii-s5-prop-8 .statement tag=03M6}

Soit $b$ un entier $> 1$. Pour tout entier $k > 0$, soit $E_k$ le produit lexicographique (III, p. 22) de la famille $(J_n)_{0 \leq n \leq k-1}$ d’intervalles tous identiques à $(0, b-1)$. Pour tout $r = (r_0, r_1, \ldots, r_{k-1}) \in E_k$, soit $f_k(r) = \sum_{h=0}^{k-1} r_h b^{k-h-1}$; l’application $f_k$ est un isomorphisme de l’ensemble ordonné $E_k$ sur l’intervalle $(0, b^k - 1)$.

Nous démontrerons la proposition par récurrence sur $k$; elle découle aussitôt des définitions pour $k = 1$. Pour tout $r = (r_0, \ldots, r_{k-1}, r_k) \in E_{k+1}$, posons $\varphi(r) = (r_0, \ldots, r_{k-1}) \in E_k$; l’application $r \mapsto (\varphi(r), r_k)$ est un isomorphisme de $E_{k+1}$ sur le produit lexicographique de $E_k$ et de $J = (0, b-1)$, comme il résulte des définitions. On peut écrire $f_{k+1}(r) = b \cdot f_k(\varphi(r)) + r_k$; montrons que la relation $r < r'$ dans $E_{k+1}$ entraîne $f_{k+1}(r) < f_{k+1}(r')$. En effet, on a alors, ou bien $\varphi(r) < \varphi(r')$, ou bien $\varphi(r) = \varphi(r')$ et $r_k < r'_k$. Dans le premier cas, l’hypothèse de récurrence entraîne que $f_k(\varphi(r)) < f_k(\varphi(r'))$, donc (III, p. 31, prop. 2) $f_k(\varphi(r')) \geq f_k(\varphi(r)) + 1$; par suite $f_{k+1}(r') \geq b \cdot f_k(\varphi(r)) + b > f_{k+1}(r)$, puisque $r_k \leq b-1$ (III, p. 36, prop. 3). Si au contraire $\varphi(r) = \varphi(r')$ et $r_k < r'_k$, il est immédiat que $f_{k+1}(r) < f_{k+1}(r')$. D’autre part, l’hypothèse de récurrence montre que $f_k(\varphi(r)) \leq b^k - 1$, d’où $f_{k+1}(r) \leq b(b^k - 1) + b - 1 = b^{k+1} - 1$. On en conclut que $f_{k+1}$ est un isomorphisme de $E_{k+1}$ sur une partie de l’intervalle $(0, b^{k+1} - 1)$; mais comme cet intervalle et $E_{k+1}$ ont le même nombre d’éléments $b^{k+1}$ (III, p. 38, prop. 5), $f_{k+1}$ est une bijection (III, p. 32, cor. 4), ce qui achève la démonstration.

Remarquons maintenant que, pour tout entier $a$, on a $a < b^a$: il suffit de raisonner par récurrence sur $a$, la proposition étant évidente pour $a = 0$, et l’hypothèse $a < b^a$ entraînant $a + 1 \leq b^a < b \cdot b^a = b^{a+1}$ (III, p. 36, prop. 3 et p. 31, prop. 2). Il existe donc un plus petit entier $k$ tel que $a < b^k$, et la prop. 8 prouve alors qu’il existe une suite finie et une seule $(r_h)_{0 \leq h \leq k-1}$ telle que $0 \leq r_h \leq b-1$ pour $0 \leq h \leq k-1$ et $a = \sum_{h=0}^{k-1} r_h b^{k-h-1}$; en outre, on a nécessairement $r_0 > 0$, sans quoi on déduirait de la prop. 8 que $a < b^{k-1}$. On dit que $\sum_{h=0}^{k-1} r_h b^{k-h-1}$ est le développement de base $b$ du nombre entier $a$.

* Dans toutes les parties des mathématiques où on n’a pas en vue le calcul numérique, la prop. 8 sera surtout utile lorsqu’elle sera appliquée à un entier $b$ premier.*

Lorsque l’entier $b$ est assez petit pour que cela soit praticable, on peut représenter chaque entier $< b$ par un symbole distinctif appelé chiffre, les chiffres représentant 0 et 1 étant en général 0 et 1. Soient $a$ un entier et $\sum_{h=0}^{k-1} r_h b^{k-h-1}$ son développement de base $b$; si l’entier $k$ figurant dans ce développement est assez petit pour que ce soit praticable, on convient d’associer à l’entier $a$ la succession de symboles obtenue en écrivant de gauche à droite $r_0 r_1 \ldots r_{k-2} r_{k-1}$ et en remplaçant chaque entier $r_i$ par le chiffre qui le représente; le symbole ainsi obtenu est appelé le symbole numérique associé à $a$. On remplace alors souvent $a$ par son symbole numérique dans les termes ou relations où il figure.

Par exemple, si $C, Q, F, D$ sont des chiffres, les symboles numériques $CQ, CQF, CQFD$ sont respectivement associés à $Cb + Q, Cb^2 + Qb + F, Cb^3 + Qb^2 + Fb + D$.

Il résulte de la prop. 8 que le symbole numérique associé à un entier $a$ est unique, et que, si $a < b^k$, il contient $k$ chiffres au plus. On notera que le symbole numérique associé à l’entier $b^k$ est formé du chiffre 1 suivi de $k$ chiffres 0.

Ce système de représentation des entiers par des symboles numériques s’appelle le système de numération de base $b$. Dans la pratique du Calcul numérique, on utilise les systèmes suivants : $a)$ le système de base 2 ou système dyadique, où les chiffres sont 0 et 1 ; $b)$ le système décimal, dans lequel les chiffres sont 0, 1, 2, 3, 4, 5 = 4 + 1, 6 = 5 + 1, 7 = 6 + 1, 8 = 7 + 1, 9 = 8 + 1, et où $b$ est l’entier 9 + 1 (dont le symbole numérique est donc 10 dans ce système).

Depuis le Moyen Age, le système décimal est traditionnellement utilisé dans le Calcul numérique, et c’est celui dont nous nous servirons lorsque nous aurons à écrire un entier explicité dans la suite de cet ouvrage. Nous renvoyons à la partie de ce Traité consacrée au Calcul numérique pour l’exposé des méthodes qui permettent d’obtenir les symboles numériques associés à la somme, la différence, le produit ou la partie entière du quotient de deux entiers donnés par leurs symboles numériques.

### 8. Analyse combinatoire

#### Proposition 9 (principe des bergers) {#ens-iii-s5-prop-9 .statement tag=03M7}

Soient $E$ et $F$ deux ensembles, $a$ et $b$ leurs cardinaux, $f$ une surjection de $E$ sur $F$ telle que les ensembles $f^{-1}(y)$, pour $y \in F$, aient tous même cardinal $c$; on a alors $a = bc$.

En effet, la famille $(f^{-1}(y))_{y \in F}$ est une partition de $E$, dont chaque élément est un ensemble de cardinal $c$; d’où la proposition (III, p. 27, cor. 2).

#### Définition 2 {#ens-iii-s5-def-2 .statement tag=03M8}

Soit $n$ un entier ; on note $n!$ (qui se lit « factorielle $n$ ») le produit $\prod_{i < n} (i + 1)$.

On a $0! = 1$ (II, p. 32) et $1! = 1$; il est clair que, pour tout entier $n$, $(n + 1)! = n!(n + 1)$. Cette dernière relation, jointe à la relation $0! = 1$, caractérise le terme $n!$, comme on le voit par récurrence sur $n$.

#### Proposition 10 {#ens-iii-s5-prop-10 .statement tag=03M9}

Soient $m$ et $n$ des entiers tels que $m \leq n$. Alors $n!/(n - m)!$ est le nombre des applications injectives d’un ensemble $A$ à $m$ éléments dans un ensemble $B$ à $n$ éléments.

Procédons par récurrence sur le nombre $m \leq n$ d’éléments de $A$. La proposition est évidente pour $m = 0$. Supposons que $m + 1 \leq n$, et soient $A$ un ensemble à $m + 1$ éléments, $A'$ une partie de $A$ ayant $m$ éléments, et $\{a\} = A - A'$. Soient $F$ et $F'$ les ensembles d’applications injectives de $A$ et $A'$ respectivement dans $B$, et soit $\varphi$ l’application $f \mapsto f|_{A'}$ qui, à toute fonction $f \in F$, fait correspondre sa restriction à $A'$. Pour toute fonction $f' \in F'$, un élément $f$ de $\varphi(f')$ est déterminé de façon unique par sa valeur $f(a)$; comme $f$ est injective, on doit avoir f(a) \in \mathbf{B} - f'(A'). Il en résulte $\varphi^{-1}(f')$ a même nombre d'éléments $n - m$ que $\mathbf{B} - f'(A')$; le principe des bergers montre alors que F possède

$$
(n - m) \frac{n!}{(n - m)!} = \frac{n!}{(n - m - 1)!}
$$

éléments, en vertu de l'hypothèse de récurrence, et cela démontre la proposition.

#### Corollaire {#ens-iii-s5-n8-cor-1 .statement tag=03MA}

*Le nombre de permutations d'un ensemble fini à n éléments est égal à n!*.

En effet, ce nombre est égal au nombre des injections de l'ensemble dans lui-même (III, p. 32, cor. 4).

#### Proposition 11 {#ens-iii-s5-prop-11 .statement tag=03MB}

*Soient E un ensemble fini à n éléments, et $(p_i)_{1 \leq i \leq h}$ une suite finie d'entiers telle que $\sum_{i=1}^{h} p_i = n$. Alors le nombre des recouvrements $(X_i)_{1 \leq i \leq h}$ de E par des ensembles mutuellement disjoints tels que Card $(X_i) = p_i$ pour $1 \leq i \leq h$, est égal à $n! / \prod_{i=1}^{h} p_i!$*.

Soient G l'ensemble des permutations de E, P l'ensemble des recouvrements $(X_i)_{1 \leq i \leq h}$ satisfaisant aux conditions de l'énoncé. Comme $\sum_{i=1}^{h} p_i = n$, P n'est pas vide. Soit $(A_i)_{1 \leq i \leq h}$ un élément de P. Pour toute permutation $f \in G$, la famille $(f(A_i))_{1 \leq i \leq h}$ appartient encore à P; désignons-la par $\varphi(f)$. Pour tout élément $(X_i)_{1 \leq i \leq h}$ de P, cherchons le nombre d'éléments $f \in G$ tels que $\varphi(f) = (X_i)$. Pour qu'il en soit ainsi, il faut et il suffit que, pour tout indice $i$, on ait $f(A_i) = X_i$; donc l'ensemble des permutations $f$ considérées est équipotent au produit des ensembles de bijections de $A_i$ sur $X_i$ (II, p. 29, prop. 8); par conséquent l'ensemble $\varphi^{-1}((X_i)_{1 \leq i \leq h})$ a $\prod_{i=1}^{h} p_i!$ éléments (cor. de la prop. 10). Comme G a $n!$ éléments, il suffit d'appliquer le principe des bergers pour obtenir la prop. 11.

#### Corollaire 1 {#ens-iii-s5-prop-11-cor-1 .statement tag=03MC}

*Soient A un ensemble à n éléments, et p un entier $\leq n$. Le nombre des parties à p éléments de A est $\frac{n!}{p!(n-p)!}$*.

Il suffit d'appliquer la prop. 11 au cas où $h = 2$, $p_1 = p$, $p_2 = n - p$.

Le nombre des parties à $p$ éléments d'un ensemble à $n$ éléments (si $p \leq n$) se note $\binom{n}{p}$ et s'appelle (pour des raisons qui apparaîtront en A, I, § 8, n° 2) le *coefficient binomial d'indices n et p*. De la relation $\binom{n}{p} = \frac{n!}{p!(n-p)!}$ résulte aussitôt que l'on a

$$
\binom{n}{p} = \binom{n}{n-p}.
$$

Ceci résulte aussi du fait que, si E est un ensemble à n éléments, X ↦ E − X est une bijection de l’ensemble des parties à p éléments de E sur l’ensemble des parties à n − p éléments de E.

On pose $\binom{n}{p} = 0$ pour tout couple d’entiers naturels tels que $p > n$. Avec cette convention, le nombre des parties à p éléments d’un ensemble à n éléments est $\binom{n}{p}$ pour tout entier naturel $p$.

#### Corollaire 2 {#ens-iii-s5-prop-11-cor-2 .statement tag=03RG}

Soient E et F des ensembles finis totalement ordonnés ayant respectivement p et n éléments. Le nombre des applications strictement croissantes de E dans F est alors $\binom{n}{p}$.

En effet, une telle application est une injection de E dans F et, comme E et F sont bien ordonnés (III, p. 34, cor. 1), pour toute partie X à p éléments de F, il existe une application strictement croissante de E sur X et une seule (III, p. 21, th. 3).

#### Proposition 12 {#ens-iii-s5-prop-12 .statement tag=03RH}

Pout tout entier n, on a $\sum_p \binom{n}{p} = 2^n$.

En effet, si E est un ensemble à n éléments, le premier membre est le nombre des parties de E et on applique III, p. 29, prop. 12.

#### Proposition 13 {#ens-iii-s5-prop-13 .statement tag=03RI}

Soient n et p des entiers ; on a

$$
\binom{n+1}{p+1} = \binom{n}{p+1} + \binom{n}{p}.
$$

Soient E un ensemble à $n + 1$ éléments, P l’ensemble des parties à $p + 1$ éléments de E, a un élément de E, et $E' = E - \{a\}$. Notons P’ (resp. P”) l’ensemble des parties à $p + 1$ éléments de E qui contiennent a (resp. qui ne contiennent pas a). L’ensemble P” est l’ensemble des parties à $p + 1$ éléments de E’, et a donc $\binom{n}{p+1}$ éléments. L’application $X \mapsto X \cap E'$ est une bijection de P’ sur l’ensemble des parties à p éléments de E’ ; P’ a donc $\binom{n}{p}$ éléments. La proposition résulte de ce que P est réunion des ensembles disjoints P’ et P”.

On peut démontrer la prop. 13 par un calcul facile utilisant la formule $\binom{n}{p} = \frac{n!}{p!(n-p)!}$ pour $p \leq n$.

#### Proposition 14 {#ens-iii-s5-prop-14 .statement tag=03RJ}

Soit n un entier > 0 ; le nombre $a_n$ (resp. $b_n$) des couples $(i, j)$ d’entiers tels que $1 \leq i \leq j \leq n$ (resp. $1 \leq i < j \leq n$) est $\frac{n(n+1)}{2}$ (resp. $\frac{n(n-1)}{2}$).

En effet, $b_n$ est le nombre des parties à 2 éléments de $\{1, n\}$; donc $b_n = \frac{n!}{2!(n-2)!} = \frac{n(n-1)}{2}$. On en déduit $a_n$ en remarquant que l’ensemble des couples $(i, j)$ tels que $1 \leq i \leq j \leq n$ est la réunion de l’ensemble des couples $(i, j)$ tels que $1 \leq i < j \leq n$ et de l’ensemble des couples $(i, i)$ où $1 \leq i \leq n$; d’où $a_n = n + b_n = \frac{n(n+1)}{2}$.

#### Corollaire {#ens-iii-s5-n8-cor-2 .statement tag=03RK}

*Pour tout entier $n > 0$, on a* $\sum_{i=1}^{n} i = \frac{n(n+1)}{2}$.

Dans l’ensemble $A$ des couples d’entiers $(i, j)$ tels que $1 \leq i \leq j \leq n$, notons $A_k$ l’ensemble des couples $(i, k)$, où $1 \leq i \leq k$ (pour un entier quelconque $k \leq n$); le nombre d’éléments de $A_k$ est $k$; d’autre part $(A_k)_{1 \leq k \leq n}$ est une partition de $A$, d’où le corollaire.

#### Proposition 15 {#ens-iii-s5-prop-15 .statement tag=03RL}

*Soient $n$ et $h$ des entiers, et $E$ un ensemble à $h$ éléments. Le nombre des applications $u$ de $E$ dans $\{0, n\}$ telles que $\sum_{x \in E} u(x) \leq n$ (resp. $\sum_{x \in E} u(x) = n$ pour $h > 0$) est $\binom{n+h}{n}$ (resp. $\binom{n+h-1}{h-1}$).

Soit $A(h, n)$ (resp. $B(h, n)$) le nombre des applications $u$ de $E$ dans $\{0, n\}$ telles que $\sum_{x \in E} u(x) \leq n$ (resp. $\sum_{x \in E} u(x) = n$ pour $h > 0$). Montrons d’abord que $A(h-1, n) = B(h, n)$; en effet, soit $E'$ une partie de $E$ à $h-1$ éléments, et soit $\{a\} = E - E'$; si $u$ est une application de $E$ dans $\{0, n\}$ telle que $\sum_{x \in E} u(x) = n$, sa restriction $u'$ à $E'$ est telle que $\sum_{x \in E'} u'(x) \leq n$, et en outre $u(a) = n - \sum_{x \in E'} u'(x)$. Réciproquement, toute application $u'$ de $E'$ dans $\{0, n\}$ satisfaisant à $\sum_{x \in E'} u'(x) \leq n$ définit une application et une seule $u$ de $E$ dans $\{0, n\}$, dont elle est la restriction, et telle que $\sum_{x \in E} u(x) = n$.

Remarquons maintenant que si $\sum_{x \in E} u(x) \leq n$, on a, soit $\sum_{x \in E} u(x) = n$, soit $\sum_{x \in E} u(x) \leq n-1$, les deux éventualités s’excluant mutuellement. Par suite
$$
A(h, n) = A(h, n-1) + B(h, n) = A(h, n-1) + A(h-1, n).
$$
Comme $A(0, 0) = 1 = \binom{0}{0}$, la formule $A(h, n) = \binom{n+h}{h}$ résulte de ce qui précède et de la prop. 13 (III, p. 43), par récurrence sur $n + h$.

\* Le nombre des monômes à $h$ indéterminées $X_1^{\alpha_1}X_2^{\alpha_2}\ldots X_h^{\alpha_h}$ de degré total $\leq n$ est évidemment égal au nombre des applications $i \mapsto \alpha_i$ de $\{1, h\}$ dans $\{0, n\}$ telles que $\sum_{i=0}^h \alpha_i \leq n$; il est par suite égal à $\binom{n+h}{h}$ en vertu de la prop. 15; ce nombre est aussi celui des monômes à $h+1$ indéterminées de degré total $n$ (cf. A, IV, § 1).*

## EXERCICES {#ens-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
