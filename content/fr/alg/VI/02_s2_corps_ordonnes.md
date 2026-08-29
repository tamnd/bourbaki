---
book: alg
book_title: Algebra
chapter: VI
chapter_title: Groupes et corps ordonnés
section: 2
section_title: CORPS ORDONNÉS
lang: fr
source: alg-iv-vii-fr
book_pages: A VI.35-A VI.44
pdf_pages: 0307-0318, 0324-0333
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux ordonnés
      page: 18
      pdf_page: 307
    - "no": 2
      title: Corps ordonnés
      page: 19
      pdf_page: 308
statements: 32
exercises: 5
content_sha256: ee612dde6081178bbeaa53c7197b09ae5e7000446bf05cbb41d6faa813c77501
---

## § 2. CORPS ORDONNÉS

### 1. Anneaux ordonnés

#### Définition 1 {#alg-vi-s2-def-1 .statement}

Étant donné un anneau commutatif A, on dit qu’une structure d’ordre sur A est compatible avec la structure d’anneau de A si elle est compatible avec la structure de groupe additif de A, et si elle vérifie l’axiome suivant :

(AO) Les relations $x \geq 0$ et $y \geq 0$ entraînent $xy \geq 0$.

L’anneau A, muni d’une telle structure d’ordre, est appelé un anneau ordonné.

#### Exemple 1 {#alg-vi-s2-n1-exa-1 .statement}

Les anneaux $\mathbf{Q}$ et $\mathbf{Z}$, ordonnés par l’ordre usuel, sont des anneaux ordonnés.
2) Un produit d’anneaux ordonnés, muni de la structure d’ordre produit, est un anneau ordonné. En particulier, l’anneau $A^E$ des applications d’un ensemble E dans un anneau ordonné A est un anneau ordonné.
3) Un sous-anneau d’un anneau ordonné, ordonné par l’ordre induit, est un anneau ordonné.

Dans un anneau ordonné, les relations $x \geq y$ et $z \geq 0$ entraînent $xz \geq yz$. En effet ces inégalités sont respectivement équivalentes à $x - y \geq 0, z \geq 0$ et $(x - y) z \geq 0$.

On démontre de façon analogue que les relations $x \leq 0$ et $y \geq 0$ (resp. $y \leq 0$) entraînent $xy \leq 0$ (resp. $xy \geq 0$). Ces résultats sont souvent invoqués sous le nom de règles des signes (deux éléments étant dits de même signe s’ils sont tous deux $\geq 0$ ou tous deux $\leq 0$). Ils entraînent que, si A est un anneau totalement ordonné, tout carré est positif, et, en particulier, que tout idempotent (par exemple l’élément unité) est positif.

#### Exemple {#alg-vi-s2-n1-exa-2 .statement}

Sur $\mathbf{Z}$ il n’y a qu’une seule structure d’anneau totalement ordonné : en effet on a $1 > 0$, d’où $n > 0$, par récurrence, pour tout entier naturel $n \neq 0$. Il existe par contre sur $\mathbf{Z}$ des structures d’anneau ordonné, mais non totalement ordonné (*cf.* ci-dessous).

Soit $P$ l’ensemble des éléments positifs d’un anneau ordonné $A$. On sait que $P$ détermine la structure d’ordre de $A$ (VI, p. 3, prop. 3). Dire que $A$ est un anneau ordonné équivaut à dire que $P$ jouit des propriétés suivantes :

$$
\begin{align*}
(\mathrm{AP}_I) &\quad P + P \subset P \\
(\mathrm{AP}_II) &\quad PP \subset P \\
(\mathrm{AP}_III) &\quad P \cap (-P) = \{0\}.
\end{align*}
$$

En effet ($\mathrm{AP}_I$) et ($\mathrm{AP}_{III}$) traduisent le fait que le groupe additif de $A$ est un groupe ordonné (VI, p. 3, prop. 3), tandis que ($\mathrm{AP}_{II}$) est la traduction de (AO).

Rappelons que, pour que la relation d’ordre définie sur $A$ soit *totale*, il faut et il suffit que la propriété suivante soit vraie :

$$
\mathrm{AP}_{IV} \qquad P \cup (-P) = A.
$$

#### Exemple {#alg-vi-s2-n1-exa-3 .statement}

Si, dans $\mathbf{Z}$, on prend pour $P$ l’ensemble des entiers positifs (au sens usuel) et pairs, on obtient une structure d’anneau *non* totalement ordonné.

Rappelons encore que, dans un groupe abélien totalement ordonné, la relation $n.x = 0$ (pour un entier naturel $n \neq 0$) entraîne $x = 0$ (VI, p. 4); cela nous donne le résultat suivant :

#### Proposition 1 {#alg-vi-s2-prop-1 .statement}

*Un anneau totalement ordonné est un $\mathbf{Z}$-module sans torsion* (II, p. 115).

### 2. Corps ordonnés

#### Définition 2 {#alg-vi-s2-def-2 .statement}

*Un corps commutatif, muni d’une structure d’ordre total, est appelé un corps ordonné si sa structure d’ordre et sa structure d’anneau sont compatibles*.

Nous nous restreignons aux relations d’ordre *total* sur les corps, car les autres sont très « pathologiques » (*cf.* VI, p. 36, exerc. 6).

*Exemples. — 1) Le corps $\mathbf{Q}$ des nombres rationnels est un corps ordonné.
2) Un sous-corps d’un corps ordonné, ordonné par l’ordre induit, est un corps ordonné.
3) *Le corps des nombres réels est un corps ordonné.* \*

Soit $K$ un corps ordonné. Pour tout $x \in K$, on pose

$$
\begin{align*}
\operatorname{sgn}(x) &= 1 \quad \text{si } x > 0, \\
\operatorname{sgn}(x) &= -1 \quad \text{si } x < 0, \\
\operatorname{sgn}(x) &= 0 \quad \text{si } x = 0.
\end{align*}
$$

On a alors $\operatorname{sgn}(xy) = \operatorname{sgn}(x) \operatorname{sgn}(y)$; on dit que $\operatorname{sgn}(x)$ est le *signe* de $x$. L’application $x \mapsto \operatorname{sgn}(x)$ de $K^*$ dans le groupe multiplicatif $\{-1, +1\}$ est un homomorphisme surjectif, dont le noyau, qui est l’ensemble des éléments strictement positifs de $K$, est un sous-groupe d’indice 2 de $K^*$.

Inversement, si $K$ est un corps commutatif et $s : K^* \to \{-1, +1\}$ un homomorphisme surjectif dont le noyau est stable pour l’addition, alors $s$ est l’application signe pour une unique structure de corps ordonné, dont les éléments strictement positifs sont ceux du noyau de $s$.

Pour tout $x$ et tout $y$ dans $K$, on a $x = \operatorname{sgn}(x) |x|$ et $|xy| = |x| |y|$.

D’autre part tout corps ordonné est de caractéristique nulle (prop. 1).

#### Proposition 2 {#alg-vi-s2-prop-2 .statement}

*Soit $A$ un anneau intègre totalement ordonné, et soit $K$ son corps des fractions. Il existe sur $K$ une structure d’ordre et une seule, induisant sur $A$ la structure d’ordre donnée, et pour laquelle $K$ est un corps ordonné.*

Tout $x \in K$ s’écrit sous la forme $x = ab^{-1}$, avec $a$ et $b$ dans $A$ et $b \neq 0$. Si $x$ est positif, $a$ et $b$ sont de même signe, et réciproquement. On voit donc que, s’il existe une relation d’ordre sur $K$ satisfaisant aux conditions prescrites, elle est unique, et l’ensemble $P$ de ses éléments positifs est identique à l’ensemble des $ab^{-1}$, où $a$ et $b$ sont des éléments de même signe de $A$ et $b \neq 0$. Reste donc à montrer que $P$ vérifie les conditions (AP$_I$), (AP$_II$), (AP$_III$) et (AP$_IV$). C’est évident pour (AP$_II$) et (AP$_IV$). Pour (AP$_I$), considérons $ab^{-1} + cd^{-1}$, où nous pouvons supposer que $a, b, c$ et $d$ sont positifs ; cette somme s’écrit $(ad + bc)(bd)^{-1}$, et $ad + bc$ et $bd$ sont positifs.

Pour (AP$_III$), considérons une égalité de la forme $ab^{-1} = -cd^{-1}$, d’où $ad + bc = 0$. Si l’on suppose que $a$ et $b$ sont de même signe, ainsi que $c$ et $d$, la règle des signes montre que $ad$ et $bc$ sont de même signe ; d’où $ad = bc = 0$, et $a = c = 0$ ; donc $P$ vérifie bien (AP$_III$).

#### Exemple {#alg-vi-s2-n2-exa-3 .statement}

Puisque $\mathbf{Z}$ n’admet qu’une seule structure d’anneau totalement ordonné (VI, p. 19, exemple), le corps $\mathbf{Q}$ n’admet qu’une seule structure d’ordre qui en fasse un corps ordonné ; cette structure est la structure usuelle.

3. **Extensions de corps ordonnés**

#### Définition 3 {#alg-vi-s2-def-3 .statement}

*Soit $K$ un corps ordonné. Une extension ordonnée de $K$ est un couple $(E, u)$, où $E$ est un corps ordonné et $u$ un homomorphisme croissant de $K$ dans $E$.

Soient $K$ un corps, $E$ un corps ordonné et $u : K \to E$ un homomorphisme. La relation

$$
x \leq y \quad \text{si} \quad u(x) \leq u(y)
$$

est une relation d’ordre total sur $K$ qui le munit d’une structure de corps ordonné, dite *induite* par celle de $E$. Si $K$ et $E$ sont deux corps ordonnés, un homomorphisme $u : K \to E$ est croissant si et seulement si la structure de corps ordonné de $K$ est induite par celle de $E$. Nous identifierons le plus souvent $K$ à son image dans $E$ par $u$.

#### Exemple 1 {#alg-vi-s2-n2-exa-1 .statement}

Tout corps ordonné K est extension ordonnée de Q. En effet, K, étant de caractéristique nulle, est extension de Q, et d’autre part Q ne peut être ordonné que d’une seule manière, comme nous venons de le voir.

#### Exemple 2 {#alg-vi-s2-n2-exa-2 .statement}

Soient K un corps ordonné, et K(X) le corps des fractions rationnelles en une indéterminée sur K. Définissons une structure d’ordre sur l’anneau de polynômes K[X] en prenant pour éléments positifs 0 et les polynômes dont le coefficient dominant est positif. On obtient ainsi un anneau totalement ordonné dont l’ordre prolonge celui de K. En appliquant la prop. 2, on définit sur K(X) une structure d’extension ordonnée de K.
\* Pour K = R, on peut montrer que la relation d’ordre ainsi définie sur K(X) est celle de la croissance au voisinage de +∞ (cf. VI, p. 23, prop. 4). \*

#### Théorème 1 {#alg-vi-s2-thm-1 .statement}

Pour qu’une extension E d’un corps ordonné K admette une structure d’extension ordonnée de K, il faut et il suffit qu’elle vérifie la condition suivante :

(EO) La relation $p_1 x_1^2 + \cdots + p_n x_n^2 = 0$ entraîne
$$
p_1 x_1 = \cdots = p_n x_n = 0
$$
pour toute suite finie $(x_i, p_i)$ de couples d’éléments $x_i$ de E et d’éléments positifs $p_i$ de K.

(EO) est visiblement équivalente à :
(EO’) L’élément — 1 n’est pas somme d’éléments de la forme $px^2$ ($x \in E, p \in K, p \geqslant 0$).

La condition (EO) est nécessaire : si E admet une structure d’extension ordonnée de K, les éléments $p_i x_i^2$ sont positifs dans E, donc nuls si leur somme est nulle ; d’autre part, $p_i x_i^2 = 0$ équivaut à $p_i x_i = 0$.

Inversement, supposant la condition (EO) satisfaite, nous allons définir une relation d’ordre sur E en construisant une partie P de E, qui satisfasse à (AP_I), (AP_{II}), (AP_{III}) et (AP_{IV}), et qui contienne l’ensemble $K_+$ des éléments positifs de K. Une telle partie P définira bien sur E une structure d’extension ordonnée de K, car on aura $K \cap P = K_+$; en effet, si P contenait un élément — $a < 0$ de K, $a$ appartiendrait à $P \cap (-P)$, contrairement à (AP_{III}).

Pour définir P, considérons l’ensemble $M$ des parties de E, qui vérifient (AP_I), (AP_{II}) et (AP_{III}), et qui contiennent la réunion de $K_+$ et de l’ensemble C des carrés d’éléments de E. Cet ensemble $M$ n’est pas vide, car il contient l’ensemble $P_0$ des éléments de la forme $\sum_i p_i x_i^2$ (que $P_0$ satisfasse à (AP_{III}) résulte aussitôt de (EO)).

De plus $M$ est inductif (E, III, p. 20, déf. 3). Il existe alors, d’après le th. 2 de E, III, p. 20, un élément maximal de $M$, dont il nous reste à montrer qu’il satisfait à (AP_{IV}); or ceci résulte du lemme suivant :

#### Lemme {#alg-vi-s2-n2-lem-1 .statement}

Soient $P \in M$ et $x \notin P$; il existe alors $P' \in M$ tel que $P \subset P'$ et que $-x \in P'$

Prenons $P' = P - xP$, et vérifions que $P'$ possède les propriétés requises. Comme $0 \in C \subset P$, on a $P \subset P'$. D’où $C \subset P'$ et $K_+ \subset P'$. Comme $1 \in C \subset P$, on a $-x \in P'$. On a
$$
P' + P' = P - xP + P - xP = P + P - x(P + P) \subset P - xP = P',
$$

d’où (AP₁). On a

$$
P'P' = (P - xP)(P - xP)
$$
$$
\subset PP + x^2PP - x(PP + PP) \subset P + CP - xP \subset P - xP = P',
$$

d’où (AP₂). Vérifions enfin (AP₃) : supposons que nous ayons une égalité de la forme $p - xq = -(r - xs)$ où $p, q, r, s$ appartiennent à $P$; on en déduit la relation $x(s + q) = p + r$; si $(s + q) \neq 0$, on a $x = (s + q)^{-2}(s + q)(p + r) \in CPP \subset P$ contrairement à l’hypothèse ; on a donc $s + q = 0$, d’où $p + r = 0$; comme $P$ vérifie (AP₃) on en déduit $s = q = r = p = 0$, ce qui achève la démonstration.

#### Corollaire 1 (« Théorème d’Artin-Schreier ») {#alg-vi-s2-thm-1-cor-1 .statement}

*Pour qu’il existe sur un corps commutatif* E *une structure d’ordre qui en fasse un corps ordonné, il faut et il suffit que la relation* $x_1^2 + \cdots + x_n^2 = 0$ *entraîne* $x_1 = \cdots = x_n = 0$.

La nécessité est évidente. Réciproquement la condition énoncée entraîne que E est de caractéristique nulle, donc extension de $\mathbf{Q}$; alors la condition (EO) est vérifiée, et le th. 1 montre qu’il existe sur E une structure d’extension ordonnée de $\mathbf{Q}$, c’est-à-dire une structure de corps ordonné.

Il n’existe *pas* de structure de corps ordonné sur un corps E où $-1$ est un carré, et, en particulier, sur un corps algébriquement clos.

#### Corollaire 2 {#alg-vi-s2-thm-1-cor-2 .statement}

*Soit* E *une extension de* K *admettant une structure d’extension ordonnée de* K. *Pour qu’un élément* $x \in E$ *soit positif pour toutes les structures d’extension ordonnée de* K *sur* E, *il faut et il suffit que* $x$ *soit de la forme* $\sum_i p_i x_i^2$, *où* $x_i \in E$ *et où les* $p_i$ *sont des éléments positifs de* K.

La condition est évidemment suffisante ; elle est aussi nécessaire, car (avec les notations de la démonstration du th. 1), si $x \notin P_0$, il existe un élément maximal P de $\mathfrak{M}$ tel que $x \notin P$; on a alors $-x \in P$ d’après le lemme, et comme $x \neq 0$, $x$ n’est pas positif pour la structure d’ordre définie par P.

4. Extensions algébriques de corps ordonnés

Soient K un corps ordonné, et $f$ un polynôme de $K[X]$. Nous dirons que $f$ change de signe dans K s’il existe deux éléments $a$ et $b$ de K tels que $f(a)\ f(b) < 0$; on dit alors que $f$ change de signe entre $a$ et $b$.

#### Proposition 3 {#alg-vi-s2-prop-3 .statement}

*Soient* K *un corps ordonné et* $f$ *un polynôme irréductible sur* K *et changeant de signe entre* a *et* b *dans* K. *L’extension* E = $K[X]/(f)$ *de* K *admet alors une structure d’extension ordonnée*.

Nous raisonnons par récurrence sur le degré $n$ de $f$. Pour $n = 1$, la vérification est triviale. Supposons le résultat vrai pour les degrés $\leq n - 1$, et démontrons-le par l’absurde pour $n$; d’après le th. 1, nous supposons donc vraie une relation de la forme

$$
1 + \sum_i p_i f_i^2(X) \equiv 0 \ (\text{mod. } f(X)) , \quad \text{où} \quad f_i \in K[X] , \quad p_i \in K \quad \text{et} \quad p_i \geqslant 0 .
$$

On peut, sans restreindre la généralité, supposer que les $f_i$ sont de degré $\leq n - 1$ (IV, p. 10, cor.). On a alors

$$
1 + \sum_i p_i f_i^2(X) = h(X) \ f(X)
$$

où $h \neq 0$ est au plus de degré $n - 2$. En remplaçant dans l’égalité précédente $X$ par $a$ et $b$, on voit que $h(a) \ f(a) > 0$ et $h(b) \ f(b) > 0$. Comme $f$ change de signe entre $a$ et $b$ par hypothèse, on en conclut que $h(a) \ h(b) < 0$. On a alors une inégalité de même nature pour un des facteurs irréductibles $g(X)$ de $h(X) : g(a) \ g(b) < 0$. Mais l’on a $1 + \sum_i p_i f_i^2(X) \equiv 0$ (mod. $g(X)$), ce qui montre que le corps $K[X]/(g)$ n’admet pas de structure d’extension ordonnée de $K$ (th. 1), contrairement à l’hypothèse de récurrence.

#### Remarque {#alg-vi-s2-n2-rem-1 .statement}

Il existe des polynômes irréductibles $f$ sur un corps ordonné $K$ qui ne changent pas de signe dans $K$, mais qui sont tels que $K[X]/(f)$ admette une structure d’extension ordonnée de $K$ (*cf.* VI, p. 41, exerc. 26, *c*).

Pour appliquer la proposition précédente, nous aurons besoin du résultat suivant :

#### Proposition 4 {#alg-vi-s2-prop-4 .statement}

*Soient $K$ un corps ordonné et $f \in K[X]$. Il existe un intervalle de $K$ dans le complémentaire duquel $f$ a même signe que son terme de plus haut degré.*

On se ramène aussitôt au cas d’un polynôme unitaire ; on peut alors écrire $f(x) = x^n (1 + a_1 x^{-1} + \cdots + a_n x^{-n})$ pour $x \neq 0$. Soit

$$
M = \sup(1, |a_1| + \cdots + |a_n|) .
$$

Pour $|x| > M$, on a $1 + a_1 x^{-1} + \cdots + a_n x^{-n} > 0$, ce qui démontre la proposition.

#### Corollaire 1 {#alg-vi-s2-prop-4-cor-1 .statement}

*Toute extension de degré fini impair d’un corps ordonné admet une structure d’extension ordonnée.*

Une telle extension étant monogène (V, p. 39, th. 1) est isomorphe à $K[X]/(f)$ où $f$ est un polynôme irréductible de degré impair. Il suffit alors de montrer que $f$ change de signe dans $K$ (prop. 3), ce qui résulte aussitôt de la prop. 4.

#### Corollaire 2 {#alg-vi-s2-prop-4-cor-2 .statement}

*Si $a$ est un élément positif d’un corps ordonné $K$, tout corps de décomposition $E$ du polynôme $X^2 - a$ admet une structure d’extension ordonnée de $K$.*

Le résultat est trivial si $a$ est un carré dans $K$. Sinon le polynôme $f(X) = X^2 - a$ est irréductible et change de signe, puisque $f(0) < 0$, et que $f(x)$ est du signe de $x^2$, donc $> 0$, pour $x$ dans le complémentaire d’un certain intervalle de $K$. Il suffit alors d’appliquer la prop. 3.

#### Remarque {#alg-vi-s2-n2-rem-2 .statement}

Lorsque le corps ordonné K contient les « racines carrées » d’un élément positif a de K (racines du polynôme $X^2 - a$), on réserve en général la notation $\sqrt{a}$ à celle de ces racines qui est positive. Si K ne contient pas les racines carrées b et – b de a dans le corps E, ce dernier admet deux structures d’extension ordonnée de K, se déduisant l’une de l’autre par le K-automorphisme défini par $b \mapsto -b$; le choix d’une de ces structures d’ordre détermine alors $\sqrt{a}$: c’est celui des éléments b et – b qui est positif.

Si a et a’ sont deux éléments positifs de K, dont les racines carrées sont dans K, on a $\sqrt{aa'} = (\sqrt{a})(\sqrt{a'})$, comme il résulte de la définition de $\sqrt{a}$, et de la règle des signes.

5. Corps ordonnés maximaux

#### Définition 4 {#alg-vi-s2-def-4 .statement}

Un corps ordonné K est dit maximal si toute extension algébrique ordonnée de K est triviale.

#### Exemple {#alg-vi-s2-n2-exa-4 .statement}

\* On verra plus tard (TG, VIII, p. 1) que le corps R des nombres réels est un corps ordonné maximal. \*

L’existence de corps ordonnés maximaux résulte du théorème suivant :

#### Théorème 2 {#alg-vi-s2-thm-2 .statement}

Tout corps ordonné K admet une extension algébrique ordonnée qui est un corps ordonné maximal.

On peut montrer que cette extension ordonnée est bien déterminée à un K-isomorphisme près (VI, p. 38, exerc. 15).

Soit $\Omega$ une clôture algébrique de K, et soit $\mathfrak{N}$ l’ensemble des couples (A, $\omega$), où A est une sous-K-extension de $\Omega$, et $\omega$ une structure d’extension ordonnée sur l’extension A de K. Ordonnons $\mathfrak{N}$ par la relation « L est une extension ordonnée de M » entre M et L. Muni de cette structure d’ordre, $\mathfrak{N}$ est un ensemble ordonné inductif : en effet, si $(L_i)$ est une famille totalement ordonnée d’éléments de $\mathfrak{N}$, le corps $L = \bigcup_i L_i$ ordonné en prenant $L_+ = \bigcup_i (L_i)_+$ est un majorant des $L_i$. En vertu de E III, p. 20, th. 2, $\mathfrak{N}$ possède un élément maximal qui répond à la question.

#### Proposition 5 {#alg-vi-s2-prop-5 .statement}

Soient K un corps ordonné maximal, et f un polynôme de K[X] changeant de signe entre deux éléments a et b de K (avec $a < b$). Alors f admet une racine x dans K, telle que $a < x < b$.

L’un au moins des facteurs irréductibles de f change de signe entre a et b, soit h. Le corps K[X]/(h) admet alors (VI, p. 22, prop. 3) une structure d’extension ordonnée de K, et h est de degré 1 (déf. 4). Comme $h(a)\ h(b) < 0$, l’unique racine x de h est telle que $a < x < b$ puisqu’une fonction polynôme de degré 1 est monotone.

#### Proposition 6 {#alg-vi-s2-prop-6 .statement}

Tout élément positif d’un corps ordonné maximal K a une racine carrée dans K. Tout polynôme de degré impair de K[X] a au moins une racine dans K.

Ceci résulte aussitôt des cor. 2 et 1 de la prop. 4 de VI, p. 23.

#### Corollaire {#alg-vi-s2-n2-cor-1 .statement}

Sur un corps ordonné maximal K, il n’existe qu’une seule structure d’ordre compatible avec la structure de corps.

En effet les éléments positifs de K sont déterminés par la structure algébrique : ce sont les carrés.

6. Caractérisation des corps ordonnés maximaux. Théorème d’Euler-Lagrange

La propriété exprimée par la prop. 6 de VI, p. 24 caractérise les corps ordonnés maximaux. De façon plus précise :

#### Théorème 3 (Euler-Lagrange) {#alg-vi-s2-thm-3 .statement}

Soit K un corps ordonné. Les trois propriétés suivantes sont équivalentes :
a) Le corps K(i) est algébriquement clos (i désignant une racine carrée de − 1).
b) Le corps K est ordonné maximal.
c) Tout élément positif de K est un carré, et tout polynôme de degré impair de K[X] a une racine dans K.

Il est clair que a) implique b) : en effet, K ne possède, à un isomorphisme près, que deux extensions algébriques, K lui-même et K(i), qui ne peut être ordonné, − 1 étant un carré.

Le fait que b) implique c) n’est autre que la prop. 6 de VI, p. 24.

Il nous reste à démontrer que c) entraîne a). Cela va résulter des deux propositions suivantes.

#### Proposition 7 {#alg-vi-s2-prop-7 .statement}

Soit K un corps ordonné dans lequel tout élément positif est un carré. Alors tout élément de K(i) est un carré, et tout polynôme du second degré sur K(i) a une racine dans K(i).

Montrons d’abord que la seconde assertion se ramène à la première. On peut mettre le polynôme du second degré $aX^2 + bX + c$, où $a \neq 0$ sous la forme suivante, souvent appelée forme canonique du trinôme :

$$
a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2)
$$

Si $d$ est une racine carrée de $(b^2 - 4ac)/4a^2$, alors $d - (b/2a)$ est une racine du polynôme du second degré étudié.

Montrons maintenant que tout élément $a + bi (a \in K, b \in K)$ est un carré ; cherchons un élément $x + yi$ tel que

$$
(x + yi)^2 = a + bi ;
$$

cela se traduit par $x^2 - y^2 = a$ et $2xy = b$. On en tire

$$
(x^2 + y^2)^2 = a^2 + b^2 .
$$

Désignons par $c$ la racine positive de $a^2 + b^2$; on a $c \geq |a|,\ c \geq |b|$ et $x^2 + y^2 = c$. D’où $x^2 = (c + a)/2$ et $y^2 = (c - a)/2$. Comme $c \geq |a|$, ces équations sont résolubles dans K, et, si $x_0$ et $y_0$ en sont des solutions, on a $x_0^2 - y_0^2 = a$, et $2x_0y_0 = \pm b$. En prenant $x = x_0$ et $y = b/2x_0$, on obtient une racine carrée cherchée.

#### Proposition 8 {#alg-vi-s2-prop-8 .statement}

Soient $K$ un corps commutatif (de caractéristique quelconque) et $K'$ un corps de décomposition du polynôme $X^2 + 1 \in K[X]$ (V, p. 20). On suppose que :
a) tout polynôme de $K[X]$, de degré impair, a une racine dans $K'$;
b) tout polynôme de $K'[X]$, de degré 2, a une racine dans $K'$.
Alors $K'$ est algébriquement clos.

Notons d’abord qu’il suffit de prouver que tout polynôme non constant de $K[X]$ a une racine dans $K'$ : cela est en effet clair si $K' = K$; si $K' \neq K$, alors $[K':K] = 2$; notons $a \mapsto \overline{a}$ l’unique $K$-automorphisme de $K'$ distinct de l’application identique ; si $f \in K'[X]$, et si $\overline{f}$ désigne le polynôme obtenu en appliquant $a \mapsto \overline{a}$ aux coefficients de $f$, on a $f \overline{f} \in K[X]$; si $a \in K'$ est une racine de $f \overline{f}$, alors $a$ est une racine de $f$ ou de $\overline{f}$, donc $a$ ou $\overline{a}$ est une racine de $f$.

Soit donc $f$ un polynôme sur $K$, de degré $2^n p$, $p$ impair. La propriété étant vraie pour $n = 0$ d’après l’hypothèse a), nous allons procéder par récurrence sur $n$. Soit $E$ une extension de $K$, où $f$ se décompose en facteurs linéaires :

$$
f(X) = \prod_i (X - a_i)
$$

Soit $b \in K$; posons $y_{ij} = a_i + a_j + ba_i a_j \in E$ et

$$
h(X) = \prod_{i < j} (X - y_{ij}) \in E[X]
$$

Ce polynôme a pour coefficients des fonctions symétriques des $a_i$, à coefficients dans $K$; il appartient donc à $K[X]$ (IV, p. 58, théorème 1); comme il est de degré $2^n p (2^n p - 1)/2 = 2^{n-1} p'$ ($p'$ impair), il a une racine $y_{ij}$ dans $K'$ d’après l’hypothèse de récurrence. Si l’on remarque que ceci a lieu pour tout $b \in K$, et que $K$ est un corps infini (en effet un corps fini, qui a des extensions monogènes de degré impair arbitrairement grand (V, p. 90, prop. 3), ne peut vérifier a)), on en déduit l’existence d’au moins un couple $(i, j)$ tel que

$$
a_i + a_j + ba_i a_j \in K' \quad \text{et} \quad a_i + a_j + b'a_i a_j \in K'
$$

avec $b \neq b'$. Alors $a_i + a_j$ et $a_i a_j$ sont éléments de $K'$, donc aussi $a_i$ et $a_j$, puisque ce sont les racines de l’équation du second degré $x^2 - (a_i + a_j)x + a_i a_j = 0$.

C.Q.F.D.

Pour une généralisation et une autre démonstration de la prop. 8, basée sur la théorie de Galois, voir VI, p. 43, exerc. 33.

Soit $K$ un corps ordonné et soit $K' = K(i)$; pour tout élément $z = a + bi$ de $K'$, la norme $\overline{z}z = a^2 + b^2$ de $z$ par rapport à $K$ (III, p. 111, exemple 1) est un élément positif de $K$, qui n’est nul que pour $z = 0$. Si dans $K$ tout élément positif est un carré (et en particulier si $K$ est un corps ordonné maximal), on appelle valeur absolue de $z$ et l’on note $|z|$ la racine carrée positive de la norme $\overline{z}z$. Comme $|zz'|^2 = |z|^2 |z'|^2$, on a $|zz'| = |z| |z'|$.

En outre, on a l’inégalité du triangle

$$
|z + z'| \leq |z| + |z'|
$$

pour tout couple d’éléments $z, z'$ de $K'$. En effet, si $z = a + bi, z' = a' + b'i$, cette inégalité équivaut à

$$
(a + a')^2 + (b + b')^2 \leq a^2 + b^2 + {a'}^2 + {b'}^2 + 2 \sqrt{(a^2 + b^2)({a'}^2 + {b'}^2)}
$$

ou encore à

$$
(aa' + bb')^2 \leq (a^2 + b^2)({a'}^2 + {b'}^2)
$$

qui s’écrit elle-même $(ab' - ba')^2 \geq 0$.

Le th. 3 nous permet de déterminer tous les polynômes irréductibles sur un corps ordonné maximal :

#### Proposition 9 {#alg-vi-s2-prop-9 .statement}

*Si $K$ est un corps ordonné maximal, les seuls polynômes irréductibles de $K[X]$ sont les polynômes du premier degré, et les polynômes du second degré $aX^2 + bX + c$ tels que $b^2 - 4ac < 0$.*

Comme $K(i)$ est algébriquement clos, toute extension algébrique de $K$ est de degré 1 ou 2, donc aussi tout polynôme irréductible sur $K$. Pour voir quels sont les polynômes du second degré qui sont irréductibles, il suffit de considérer la forme canonique $a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2)$ (*cf.* VI, p. 25, prop. 7).

#### Remarque {#alg-vi-s2-n2-rem-3 .statement}

La mise sous forme canonique des trinômes donne le résultat plus fort que voici : étant donné un corps ordonné $K$, pour que le polynôme $aX^2 + bX + c$ ait un signe constant dans $K$, il faut et il suffit que $b^2 - 4ac < 0$, et le signe du polynôme est alors celui de $a$.

7. Espaces vectoriels sur un corps ordonné

Soient $K$ un corps ordonné, $E$ un espace vectoriel sur $K$. Dans l’ensemble $E - \{0\}$, la relation « il existe $\lambda > 0$ dans $K$ tel que $y = \lambda x$ » entre $x$ et $y$ est une *relation d’équivalence*. Les classes d’équivalence pour cette relation sont appelées les *demi-droites ouvertes d’origine* 0 ; la réunion d’une demi-droite ouverte et de $\{0\}$ est appelée *demi-droite fermée* (ou quelquefois simplement *demi-droite*) d’origine 0. Tout vecteur $a \neq 0$ contenu dans une demi-droite ouverte (resp. fermée) $\Delta$ est dit *vecteur directeur* de $\Delta$, et $\Delta$ est l’ensemble des vecteurs $\lambda a$ pour tous les scalaires $\lambda > 0$ (resp. $\lambda \geq 0$). Toute droite $D$ passant par 0 contient exactement deux demi-droites ouvertes (resp. fermées) d’origine 0 ; si $\Delta$ est l’une d’elles, l’autre est $-\Delta$ (dite *opposée* de $\Delta$).

Si maintenant $F$ est un *espace affine* sur $K$, et $E$ l’espace des translations de $F$, on appelle *demi-droite ouverte* (resp. *fermée*) *d’origine* $a \in F$ toute partie de $F$ de la forme $\Delta = a + \Delta_0$, où $\Delta_0$ est une demi-droite ouverte (resp. fermée) de $E$, qui est bien déterminée par la donnée de $\Delta$ (car, pour $b \neq a$ dans $\Delta$, c’est la demi-droite de vecteur directeur $b - a$) et est appelée la *direction* de $\Delta$ ; un vecteur directeur de $\Delta_0$ est aussi appelé *vecteur directeur de* $\Delta$.

Supposons maintenant que $E$ soit de dimension *finie n* sur $K$ ; alors on sait (III, p. 87, cor. 1) que la puissance extérieure n-ième $\Lambda^n E$ est un espace vectoriel de dimension 1 sur K, donc réunion de deux demi-droites fermées opposées d’origine 0. On appelle ces demi-droites les orientations sur E ; l’espace E muni de la structure définie par la donnée d’une de ces demi-droites Δ est dit orienté ; un n-vecteur z est alors dit positif (resp. négatif ) pour cette orientation s’il appartient à Δ (resp. à − Δ) ; il est négatif (resp. positif) pour l’orientation opposée.

Une orientation d’un espace affine F sur K, de dimension finie, est par définition une orientation de l’espace des translations de F ; muni d’une telle orientation, F est appelé un espace affine orienté.

Soit E un espace vectoriel orienté sur K, de dimension n ; une base ordonnée $(a_i)_{1 \leq i \leq n}$ de E est dite positive ou directe (resp. négative ou rétrograde) si le n-vecteur $a_1 \wedge a_2 \wedge \ldots \wedge a_n$ est positif (resp. négatif). Si u est un automorphisme de l’espace vectoriel E, on a $(\Lambda^n u)(z) = \det(u).z$ pour tout $z \in \Lambda^n E$, donc pour que $\Lambda^n u$ laisse invariante l’orientation de E (ou comme on dit encore, pour que u conserve l’orientation) il faut et il suffit que $\det(u) > 0$ ; les automorphismes ayant cette propriété ne sont autres que les automorphismes de la structure d’espace vectoriel orienté de E ; ils forment un sous-groupe distingué $GL^+(E)$ du groupe linéaire $GL(E)$, qui est d’indice 2 dans ce dernier lorsque $E \neq 0$.

Lorsque $E = 0$, $GL(E) = \mathrm{End}(E)$ est réduit à l’application identique $1_E$ et l’on a par définition $\det(1_E) = 1$. On notera que dans ce cas $\Lambda^n E = \Lambda^0 E = K$ par définition ; la demi-droite de K formée des scalaires $\geq 0$ est appelée l’orientation canonique de l’espace réduit à 0.

Soient M, N deux sous-espaces supplémentaires de dimensions p et $n - p$ respectivement dans un espace vectoriel E de dimension n ; si $z'$ (resp. $z''$) est un vecteur $\neq 0$ de $\Lambda^p M$ (resp. de $\Lambda^{n-p} N$), $z' \wedge z''$ est un vecteur $\neq 0$ de $\Lambda^n E$. Lorsqu’on s’est donné une orientation sur M et une orientation sur N, les vecteurs $z' \wedge z''$, pour $z'$ et $z''$ positifs, forment une orientation de E, dite orientation produit de l’orientation de M par l’orientation de N (qui dépend de l’ordre des facteurs lorsque $p(n - p)$ est impair). Inversement, si l’on s’est donné des orientations sur E et sur M, il existe sur N une seule orientation telle que l’orientation donnée sur E soit produit de l’orientation donnée sur M et de cette orientation sur N (dans cet ordre) ; on dit que cette orientation est supplémentaire de l’orientation de M par rapport à celle de E. Si N’ est un second sous-espace supplémentaire de M, la projection canonique $N \to N'$ parallèlement à M transforme l’orientation supplémentaire de N en celle de N’. L’image de l’orientation supplémentaire de N par l’application canonique $N \to E/M$ ne dépend donc pas du supplémentaire choisi N ; on dit que, sur $E/M$, c’est l’orientation quotient de celle de E par celle de M.

Exercises

## EXERCICES {#alg-vi-s2-exercises}

Tous les anneaux considérés sont supposés *commutatifs* sauf mention expresse du contraire.

See the [exercises for § 2](exercises/s2/).
