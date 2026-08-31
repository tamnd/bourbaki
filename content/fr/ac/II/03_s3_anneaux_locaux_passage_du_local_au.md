---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: Localisation
section: 3
section_title: Anneaux locaux. Passage du local au global
lang: fr
source: ac-i-iv-fr
pdf_pages: 0100-0116, 0164-0168
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux locaux.
      page: 0
      pdf_page: 100
    - "no": 2
      title: Modules sur un anneau local.
      page: 0
      pdf_page: 103
    - "no": 3
      title: Passage du local au global.
      page: 0
      pdf_page: 108
    - "no": 4
      title: Localisation de la platitude.
      page: 0
      pdf_page: 113
    - "no": 5
      title: Anneaux semi-locaux.
      page: 0
      pdf_page: 114
statements: 47
exercises: 16
content_sha256: 371747b867ef287ed5c3614c06b50b96ba9579116d40576da189e40fc42ad561
---

## § 3. Anneaux locaux. Passage du local au global

### 1. Anneaux locaux.

#### Proposition 1 {#ac-ii-s3-prop-1 .statement}

Soient A un anneau, I l’ensemble des éléments non inversibles de A. L’ensemble I est la réunion des idéaux de A distincts de A. En outre, les conditions suivantes sont équivalentes :

a) I est un idéal.
b) L’ensemble des idéaux de A distincts de A possède un plus grand élément.
c) A possède un idéal maximal unique.

En effet, la relation $x \in I$ équivaut à $1 \notin xA$, donc à $xA \neq A$. Si $a$ est un idéal de A distinct de A et si $x \in a$, on a $xA \subset a$, donc $xA \neq A$ et $x \in I$. Donc tout idéal distinct de A est contenu dans I et tout élément $x \in I$ appartient à un idéal principal $xA \neq A$. Ceci prouve la première assertion, et celle-ci entraîne aussitôt l’équivalence des propriétés a), b), c).

Remarque 1). — On notera que, si c) est vérifiée, I est le radical de l’anneau A (Alg., chap. VIII, § 6, no 3, déf. 3).

#### Définition 1 {#ac-ii-s3-def-1 .statement}

On dit qu’un anneau A est un anneau local s’il vérifie les conditions équivalentes a), b), c) de la prop. 1. Le quotient de A par son radical (qui est alors l’unique idéal maximal de A) s’appelle le corps résiduel de A.

#### Définition 2 {#ac-ii-s3-def-2 .statement}

Soient A, B deux anneaux locaux, m, n leurs idéaux maximaux respectifs. On dit qu’un homomorphisme $u : A \to B$ est local si $u(m) \subset n$.

Il revient au même de dire que $\bar{u}(n) = m$, car $\bar{u}(n)$ est alors un idéal contenant m et ne contenant pas 1, donc égal à m. Par passage aux quotients, on déduit alors canoniquement de $u$ un homomorphisme injectif $A/m \to B/n$ du corps résiduel de A dans celui de B.

#### Exemple 1 {#ac-ii-s3-n1-exa-1 .statement}

Un corps est un anneau local. Un anneau réduit à 0 n’est pas un anneau local.

#### Exemple 2 {#ac-ii-s3-n1-exa-2 .statement}

Soient $A$ un anneau local, $k$ son corps résiduel. L’anneau de séries formelles $B = A[[X_1, ..., X_n]]$ est un anneau local, car les éléments non inversibles de $B$ sont les séries formelles dont le terme constant est non inversible dans $A$ ($Alg.$, chap. IV, § 5, no 6, prop. 4). L’injection canonique de $A$ dans $B$ est un homomorphisme local, et l’injection correspondante des corps résiduels est un isomorphisme.

#### Exemple 3 {#ac-ii-s3-n1-exa-3 .statement}

Soit $b$ un idéal d’un anneau $A$ qui n’est contenu que dans un seul idéal maximal $m$; alors $A/b$ est un anneau local d’idéal maximal $m/b$ et de corps résiduel canoniquement isomorphe à $A/m$. Ceci s’applique en particulier au cas où $b = m^k$, $m$ étant un idéal maximal quelconque de $A$ ($§ 1$, no 1, cor. de la prop. 1). Si $A$ est lui-même un anneau local d’idéal maximal $m$, alors, pour tout idéal $b \neq A$ de $A$, $A/b$ est un anneau local, l’homomorphisme canonique $A \to A/b$ un homomorphisme local, l’homomorphisme correspondant des corps résiduels étant bijectif.

#### Exemple 4 {#ac-ii-s3-n1-exa-4 .statement}

Soient $X$ un espace topologique, $x_0$ un point de $X$, $A$ l’anneau des germes au point $x_0$ des fonctions numériques continues dans un voisinage de $x_0$ (*Top. gén.*, chap. I, 3e éd., § 6, no 10). Il est clair que, pour que le germe en $x_0$ d’une fonction continue $f$ soit inversible dans $A$, il faut et il suffit que $f(x_0) \neq 0$, car cette condition entraîne que $f(x) \neq 0$ dans un voisinage de $x_0$. L’anneau $A$ est donc un anneau local dont l’idéal maximal $m$ est l’ensemble des germes des fonctions *nulles en* $x_0$; par passage au quotient, l’application $g \to g(x_0)$ de $A$ dans $\mathbf{R}$ donne un *isomorphisme* du corps résiduel $A/m$ sur $\mathbf{R}$.

#### Proposition 2 {#ac-ii-s3-prop-2 .statement}

*Soient* $A$ *un anneau*, $p$ *un idéal premier de* $A$. *L’anneau* $A_p^{m_p}$ *est local ; son idéal maximal est l’idéal* $pA_p = p_p$, *engendré par l’image canonique de* $p$ *dans* $A_p$; *son corps résiduel est canoniquement isomorphe au corps des fractions de* $A/p$.

En effet, soit $S = A - p$, et soit $j : A \to A_p$ l’homomorphisme canonique ; l’hypothèse que $p$ est premier entraîne que $p$ est saturé pour $S$, donc $j^{-1}(pA_p) = p$ ($§ 2$, no 4, prop. 10), et comme les idéaux de $A$ disjoints de $S$ sont ceux contenus dans $p$, les deux premières assertions sont des cas particuliers du § 2, n° 5, prop. 11, (ii). En outre, si $f$ est l’homomorphisme canonique $A \to A/p$, $f(S)$ est l’ensemble des éléments $\neq 0$ de l’anneau intègre $A/p$, donc la dernière assertion est un cas particulier du § 2, n° 5, prop. 11, (i).

#### Définition 3 {#ac-ii-s3-def-3 .statement}

Soient $A$ un anneau, $p$ un idéal premier de $A$. L’anneau $A_p$ s’appelle l’anneau local de $A$ en $p$, ou l’anneau local de $p$ lorsqu’aucune confusion n’est à craindre.

Remarque 2). — Si $A$ est un anneau local et $m$ son idéal maximal, les éléments de $A - m$ sont inversibles (prop. 1), donc $A_m$ s’identifie canoniquement à $A$ ($§ 2$, n° 1, Remarque 5).

#### Exemple 5 {#ac-ii-s3-n1-exa-5 .statement}

Soit $p$ un nombre premier. L’anneau local $\mathbf{Z}_{(p)}$ est l’ensemble des nombres rationnels $a/b$, où $a, b$ sont des entiers rationnels tels que $b$ soit étranger à $p$; le corps résiduel de $\mathbf{Z}_{(p)}$ est isomorphe au corps premier $\mathbf{F}_p = \mathbf{Z}/(p)$.

#### Exemple 6 {#ac-ii-s3-n1-exa-6 .statement}

Soient $V$ une variété algébrique affine, $A$ l’anneau des fonctions régulières sur $V$, $W$ une sous-variété irréductible de $V$, et $p$ l’idéal (nécessairement premier) de $A$ formé par les fonctions nulles en tout point de $W$. L’anneau $A_p$ s’appelle l’anneau local de $W$ sur $V$*

#### Proposition 3 {#ac-ii-s3-prop-3 .statement}

Soient $A$ un anneau, $p$ un idéal premier de $A$, $S = A - p$. Pour tout idéal $b'$ de $A_p$ distinct de $A_p$, soit $b$ l’idéal $(i_A^S)^{-1}(b')$ de $A$, de sorte que $b' = bA_p$.

(i) Soit $f$ l’homomorphisme canonique $A \to A/b$. L’homomorphisme de $A_p$ dans $(A/b)_{p/b}$ canoniquement associé à $f$ ($§ 2$, n° 1, prop. 2) est surjectif et son noyau est $b'$, ce qui définit par passage aux quotients un isomorphisme canonique de $A_p/b'$ sur $(A/b)_{p/b}$.

(ii) L’application $b' \to b = (i_A^S)^{-1}(b')$, restreinte à l’ensemble des idéaux premiers de $A_p$, est un isomorphisme (pour la relation d’inclusion) de cet ensemble sur l’ensemble des idéaux premiers de $A$ contenus dans $p$. Si $b'$ est premier dans $A_p$ il existe un isomorphisme de l’anneau $A_b$ sur l’anneau $(A_p)_{b'}$ qui applique $a/s$ sur $(a/1)/(s/1)$ pour $a \in A, s \in A - b$.

Ceci n’est qu’un cas particulier du § 2, n° 5, prop. 11.

#### Remarque 3 {#ac-ii-s3-n1-rem-3 .statement}

Si $a$ est un idéal de $A$ non contenu dans $p$, on a $aA_p = A_p$ et $(A/a)_p = 0$ ($§ 2$, no 5, Remarque).

#### Remarque 4 {#ac-ii-s3-n1-rem-4 .statement}

Soient $A, B$ deux anneaux, $\rho : A \to B$ un homomorphisme, $q$ un idéal premier de $B$, $p$ l’idéal premier $\bar{\rho}^{-1}(q)$ de $A$. Comme $\rho(A - p) \subset B - q$, on déduit canoniquement de $\rho$ un homomorphisme $\rho_q : A_p \to B_q$ ($§ 2$, no 1, prop. 2), et il est immédiat que $\rho_q(pA_p) \subset qB_q$, donc $\rho_q$ est un homomorphisme local.

### 2. Modules sur un anneau local.

#### Proposition 4 {#ac-ii-s3-prop-4 .statement}

Soient $A$ un anneau non nécessairement commutatif, $m$ un idéal à droite de $A$ contenu dans le radical de $A$, $M$ un $A$-module à gauche. On suppose vérifiée l’une des conditions suivantes :

(i) $M$ est de type fini ;
(ii) $m$ est nilpotent.

Alors la relation $(A_d/m) \otimes_A M = 0$ entraîne $M = 0$.

L’assertion relative à l’hypothèse (i) n’est autre que le cor. 3 de la prop. 6 d’Alg., chap. VIII, $§ 6$, no 3. D’autre part, la relation $(A_d/m) \otimes_A M = 0$ équivaut à $M = mM$ et entraîne donc $M = m^nM$ pour tout entier $n > 0$; d’où l’assertion relative à l’hypothèse (ii).

#### Corollaire 1 {#ac-ii-s3-prop-4-cor-1 .statement}

Soient $A$ un anneau non nécessairement commutatif, $m$ un idéal à droite de $A$ contenu dans le radical de $A$, $M$ et $N$ deux $A$-modules à gauche, $u : M \to N$ une application $A$-linéaire. Si $N$ est de type fini ou si $m$ est nilpotent, et si $1 \otimes u : (A_d/m) \otimes_A M \to (A_d/m) \otimes_A N$ est surjective, alors $u$ est surjective.

En effet, $(A_d/m) \otimes_A (N/u(M))$ est canoniquement isomorphe à $((A_d/m) \otimes_A N)/\mathrm{Im}\,(1 \otimes u)$ (Alg., chap. II, 3e éd., $§ 3$, no 6, cor. 1 de la prop. 6); l’hypothèse entraîne donc $(A_d/m) \otimes_A (N/u(M)) = 0$, donc $N/u(M) = 0$ en vertu de la prop. 4.

#### Corollaire 2 {#ac-ii-s3-prop-4-cor-2 .statement}

Soient $A$ un anneau non nécessairement commutatif, $m$ un idéal bilatère de $A$ contenu dans le radical de $A$, $M$ un $A$-module à gauche, $(x_i)_{i \in I}$ une famille d’éléments de $M$. Si $M$ est de type fini ou si $m$ est nilpotent, et si les éléments $1 \otimes x_i$, (t \in I) engendrent le (A/m)-module à gauche (A/m) \otimes_A M, les x_t engendrent M.

Soit en effet (e_t)_{t \in I} la base canonique du A-module à gauche $A_s^{(I)}$ : il suffit d’appliquer le cor. 1 à l’application A-linéaire $u : A_s^{(I)} \to M$ telle que $u(e_t^i) = x_t$ pour tout $t \in I$.

#### Proposition 5 {#ac-ii-s3-prop-5 .statement}

Soient A un anneau non nécessairement commutatif, m un idéal bilatère de A contenu dans le radical de A, M un A-module à gauche. On suppose vérifiée l’une des conditions suivantes :

(i) M admet une présentation finie ;
(ii) m est nilpotent.

Alors, si $(A/m) \otimes_A M = M/mM$ est un (A/m)-module à gauche libre et si l’homomorphisme canonique de $m \otimes_A M$ dans M est injectif, M est un A-module libre. De façon précise, si $(x_t)_{t \in I}$ est une famille d’éléments de M telle que $(1 \otimes x_t)$ soit une base du (A/m)-module $M/mM$, $(x_t)$ est une base de M.

Si $a \in A$, $x \in M$ et si $\bar{a}$ est la classe de a dans $A/m$, on a $\bar{a} \otimes x = 1 \otimes (ax)$, donc l’hypothèse entraîne qu’il existe une famille $(x_t)_{t \in I}$ d’éléments de M telle que $(1 \otimes x_t)$ soit une base du (A/m)-module $(A/m) \otimes_A M$. On sait déjà que les $x_t$ engendrent M (cor. 2 de la prop. 4) ; nous allons voir qu’ils sont linéairement indépendants sur A. Pour cela, considérons le A-module libre $L = A_s^{(I)}$; soit $(e_t)$ sa base canonique, et soit $u : A_s^{(I)} \to M$ l’application A-linéaire telle que $u(e_t) = x_t$ pour tout $t \in I$; si R est le noyau de u, nous allons prouver que $R = 0$. Dans l’hypothèse (i), $(A/m) \otimes_A M$ est un (A/m)-module de type fini, donc I est nécessairement fini et R est un A-module de type fini en vertu du chap. I, § 2, n° 8, lemme 9. D’après la prop. 4, il suffira donc de prouver (dans l’une ou l’autre hypothèse) que l’on a $R = mR$.

Soit j l’injection canonique $R \to L$; on a donc le diagramme commutatif

$$
\begin{array}{ccccc}
m \otimes R & \xrightarrow{1 \otimes i} & m \otimes L & \xrightarrow{1 \otimes u} & m \otimes M \\
a \downarrow & & b \downarrow & & c \downarrow \\
R & \xrightarrow{j} & L & \xrightarrow{u} & M
\end{array}
$$

dans lequel les deux lignes sont exactes, j est injectif et $1 \otimes u$ est surjectif (chap. I, § 2, n° 1, lemme 1); comme par hypothèse Ker (c) = 0, on a donc une suite exacte

$$
0 \xrightarrow{d} \mathrm{Coker}(a) \to \mathrm{Coker}(b) \xrightarrow{\varphi} \mathrm{Coker}(c)
$$

(chap. I, § 1, n° 4, prop. 2); il suffit de vérifier que $\varphi$ est bijectif, car on en déduira Coker (a) = 0, autrement dit que a est surjectif et par suite R = mR. Or, Coker (b) = (A/m) \otimes_A L et Coker (c) = (A/m) \otimes_A M, et par définition $\varphi(1 \otimes e_i) = 1 \otimes x_i$; comme $(1 \otimes e_i)$ est une base de (A/m) \otimes_A L, la définition des $x_i$ montre que $\varphi$ est bijectif.

#### Corollaire 1 {#ac-ii-s3-prop-5-cor-1 .statement}

Soient A un anneau non nécessairement commutatif, m le radical de A, M un A-module à gauche. On suppose que A/m est un corps, que l’homomorphisme canonique de m \otimes_A M dans M est injectif, et que l’une des conditions (i), (ii) de la prop. 5 est satisfaite. Pour qu’une famille $(y_\lambda)$ d’éléments de M soit une base d’un facteur direct de M, il faut et il suffit que la famille $(1 \otimes y_\lambda)$ soit libre dans M/mM.

En effet, si cette condition est vérifiée, on peut supposer que $(y_\lambda)$ est une sous-famille d’une famille $(x_i)$ d’éléments de M telle que $(1 \otimes x_i)$ soit une base de M/mM (Alg., chap. II, 3e éd., § 7, n° 1, th. 2), et la prop. 5 prouve alors que $(x_i)$ est une base de M.

#### Corollaire 2 {#ac-ii-s3-prop-5-cor-2 .statement}

Soient A un anneau non nécessairement commutatif, m le radical de A, M un A-module à gauche. On suppose que A/m est un corps, et que l’une des conditions suivantes est vérifiée :

(i) M admet une présentation finie ;
(ii) m est nilpotent.

Alors les propriétés suivantes sont équivalentes :
a) M est libre ;
b) M est projectif ;
c) M est plat ;
d) l’homomorphisme canonique $m \otimes_A M \to M$ est injectif ;
*e) on a $\mathrm{Tor}_1^A(A/m, M) = 0.$*

Les implications $a \Rightarrow b) \Rightarrow c) \Rightarrow d)$ sont immédiates. Comme A/m est un corps, $(A/m) \otimes_A M$ est un (A/m)-module libre, et la prop. 5 montre que d) implique a).

*Enfin, on sait que Tor$_1^A(A, M) = 0$, et de la suite exacte $0 \to m \to A \to A/m \to 0$, on déduit donc la suite exacte
$$
0 \to \mathrm{Tor}_1^A(A/m, M) \to m \otimes_A M \to M;
$$
cela prouve que Tor$_1^A(A/m, M)$ est isomorphe au noyau de l'homomorphisme canonique $m \otimes_A M \to M$; d'où l'équivalence de d) et e).*

On peut montrer que, pour tout anneau $A$ ayant un radical $m$ tel que $A/m$ soit un corps, *tout* $A$-module projectif est libre (exerc. 3).

#### Proposition 6 {#ac-ii-s3-prop-6 .statement}

*Soient $A$ un anneau non nécessairement commutatif*, $m$ son radical ; supposons que $A/m$ soit un corps. *Soient $M$ et $N$ deux $A$-modules libres de type fini, et soit $u : M \to N$ un homomorphisme. Les propriétés suivantes sont équivalentes* :
a) *$u$ est un isomorphisme de $M$ sur un facteur direct de $N$* ;
b) $1 \otimes u : (A/m) \otimes_A M \to (A/m) \otimes_A N$ est injectif ;
c) *$u$ est injectif et $\operatorname{Coker}(u)$ est un $A$-module libre* ;
d) *l'homomorphisme transposé $t u : N^* \to M^*$ est surjectif*.

On sait (*Alg.*, chap. II, 3e éd., § 1, no 11, prop. 21) que, si $N/u(M)$ est libre, $u(M)$ est facteur direct dans $N$, donc c) implique a) ; inversement, a) implique que $\operatorname{Coker}(u)$, isomorphe à un supplémentaire de $u(M)$ dans $N$, est un $A$-module projectif de type fini, et *a fortiori* de présentation finie (chap. I, § 2, no 8, lemme 8) ; donc ce module est libre en vertu du cor. 2 de la prop. 5, et a) implique c). Il est évident d'autre part que a) entraîne b). Posons pour simplifier $M' = (A/m) \otimes_A M,\ N' = (A/m) \otimes_A N$ ; comme $M$ et $N$ sont de type fini, les duals ${M'}^*$ et ${N'}^*$ des $(A/m)$-modules $M'$ et $N'$ s'identifient canoniquement à $M^* \otimes_A (A/m)$ et $N^* \otimes_A (A/m)$ et $t(1 \otimes u)$ à $(t u) \otimes 1$ (*Alg.*, chap. II, 3e éd., § 5, no 4, prop. 8) ; comme $M'$ et $N'$ sont des espaces vectoriels sur le corps $A/m$, l'hypothèse que $1 \otimes u$ est injectif entraîne que $t(1 \otimes u)$ est surjectif (*Alg.*, chap. II, 3e éd., § 7, no 5, prop. 10) ; le cor. 1 de la prop. 4 montre alors que $t u$ est surjectif, et nous avons ainsi prouvé que b) entraîne d). Montrons enfin que d) entraîne a). Supposons $t u$ surjectif ; comme $M^*$ est libre, il existe un homomorphisme $f$ de $M^*$ dans $N^*$ tel que $1_{M^*} = t u \circ f$ (*Alg.*, chap. II, 3e éd., § 1, no 11, prop. 21) ; comme $M$ et $N$ sont libres de type fini, il existe un homomorphisme g de N dans M tel que $f = ^t g$; on a donc $^t 1_M = 1_{M^*} = ^t u \circ ^t g = t(g \circ u)$, d'où $1_M = g \circ u$; ceci prouve que $u$ est un isomorphisme de M sur un sous-module facteur direct de N (Alg., chap. II, 3e éd., § 1, n° 9, cor. 2 de la prop. 15).

#### Corollaire {#ac-ii-s3-n2-cor-1 .statement}

Sous les hypothèses de la prop. 6, les propriétés suivantes sont équivalentes :
a) $u$ est un isomorphisme de M sur N ;
b) M et N ont même rang (Alg., chap. II, 3e éd., § 7; n° 2) et $u$ est surjectif ;
c) $1 \otimes u : M/mM \to N/mN$ est bijectif.

Il est clair que a) entraîne b) ; b) entraîne que $1 \otimes u$ est surjectif ; en outre l'hypothèse que M et N ont même rang entraîne qu'il en est de même des espaces vectoriels $(A/m) \otimes_A M$ et $(A/m) \otimes_A N$ sur $A/m$, donc $1 \otimes u$ est bijectif (Alg., chap. II, 3e éd., § 7, n° 4, cor. de la prop. 9) et b) entraîne c). Enfin, la condition c) entraîne, en vertu de la prop. 6, que N est somme directe de $u(M)$ et d'un sous-module libre P et $u$ un isomorphisme de $u$ sur $u(M)$; si on avait $P \neq 0$, on aurait $(A/m) \otimes_A P \neq 0$, et $1 \otimes u$ ne serait pas surjectif ; donc c) entraîne a).

Les propositions démontrées ci-dessus dans ce n° seront le plus souvent appliquées lorsque A est un anneau local et m son idéal maximal. Le cor. 2 de la prop. 5 se complète alors par la

#### Proposition 7 {#ac-ii-s3-prop-7 .statement}

Soient A un anneau local réduit, m son idéal maximal, $(\mathfrak{p}_i)_{i \in I}$ la famille des idéaux premiers minimaux de A, $K_i$ le corps des fractions de $A/\mathfrak{p}_i$, M un A-module de type fini. Pour que M soit libre, il faut et il suffit que l'on ait

(1) $$ [(A/m) \otimes_A M : (A/m)] = [K_i \otimes_A M : K_i] \quad \text{pour tout } i \in I. $$

Si M est libre, il est clair que les deux membres de (1) sont égaux au rang de M pour tout $i \in I$. Supposons maintenant la condition satisfaite, et notons n la valeur commune des deux membres de (1); en vertu du cor. 2 de la prop. 4, M possède un système de n générateurs $x_j$ ($1 \leq j \leq n$). Supposons d'abord A intègre, auquel cas $\mathfrak{p}_i = 0$ pour tout $i \in I$. Les éléments $1 \otimes x_j$ ($1 \leq j \leq n$) engendrent l'espace vectoriel $K \otimes M$ sur le corps des fractions K de A ; mais comme par hypothèse cet espace est de rang n sur K, les éléments $1 \otimes x_j$ sont linéairement indépendants sur K. On en déduit (Alg., chap. II, 3e éd., § 1, no 13, Remarque 1) que les $x_j$ sont linéairement indépendants sur A, donc forment une base de M.

Passons au cas général ; il existe un homomorphisme surjectif $\nu$ de $L = A^n$ sur M. Considérons le diagramme commutatif

$$
\begin{array}{ccc}
L & \xrightarrow{\nu} & M \\
u \downarrow & & \downarrow u' \\
\prod_l ((A/p_l) \otimes L) & \xrightarrow{\nu'} & \prod_l ((A/p_l) \otimes M)
\end{array}
$$

où $u$ (resp. $u'$) est l’application $x \to (\varphi_l(x))$ (resp. $y \to (\psi_l(y))$), $\varphi_l : L \to (A/p_l) \otimes L$ (resp. $\psi_l : M \to (A/p_l) \otimes M$) étant l’application canonique, et $\nu'$ est l’application produit des $1_{A/p_l} \otimes \nu$. On a $(A/p_l)/(m/p_l) \otimes_{A/p_l} ((A/p_l) \otimes_A M) = (A/m) \otimes_A M$, et comme $A/p_l$ est un anneau local intègre, il résulte de la première partie du raisonnement que chacun des $1_{A/p_l} \otimes \nu$ est un isomorphisme ; il en est donc de même de $\nu'$. D’autre part, comme A est réduit, on a

$$
\bigcap_l p_l = (0) \quad (§ 2, \text{no } 6, \text{prop. } 13),
$$
d’où $\bigcap_l (p_l L) = 0$ puisque L est libre (Alg., chap. II, 3e éd., § 3, no 7, Remarque) ; comme $p_l L$ est le noyau de $\varphi_l$, cela montre que $u$ est injectif. On en conclut que $\nu' \circ u = u' \circ \nu$ est injectif, donc $\nu$ est injectif, et comme $\nu$ est surjectif par définition, cela montre que M est libre.

### 3. Passage du local au global.

#### Proposition 8 {#ac-ii-s3-prop-8 .statement}

Soient A un anneau, m un idéal maximal de A, M un A-module. S’il existe un idéal a de A tel que m soit le seul idéal maximal de A contenant a, et que $aM = 0$, alors l’homomorphisme canonique $M \to M_m$ est bijectif.

En effet, $A/a$ est alors un anneau local d’idéal maximal $m/a$; on peut considérer M comme un $(A/a)$-module ; pour tout $s \in A - m$, l’image canonique de s dans $A/a$ est inversible, donc l’homothétie $x \to sx$ de M est bijective d’après la définition de $M_m$ comme solution d’un problème universel (§ 2, no 2) ; d’où la proposition.

En particulier, s’il existe $k \geqslant 0$ tel que $m^k M = 0$, l’homomorphisme $M \to M_m$ est bijectif ($§ 1$, n° 1, cor. de la prop. 1).

#### Proposition 9 {#ac-ii-s3-prop-9 .statement}

Soient $A$ un anneau, $m$ un idéal maximal de $A$, $M$ un $A$-module, $k$ un entier $\geqslant 0$. L’homomorphisme canonique $M \to M_m / m^k M_m$ est surjectif, admet $m^k M$ pour noyau, et définit un isomorphisme de $M / m^k M$ sur $M_m / m^k M_m$.

Le cas où $k = 0$ étant trivial, supposons $k \geqslant 1$. Il résulte de la prop. 8 que l’homomorphisme canonique $M / m^k M \to (M / m^k M)_m$ est bijectif. D’autre part $(M / m^k M)_m$ s’identifie canoniquement à $M_m / (m^k M)_m$ ($§ 2$, n° 4, th. 1) et on a $(m^k M)_m = m^k M_m$ ($§ 2$, n° 7, cor. de la prop. 18), d’où un isomorphisme de $M / m^k M$ sur $M_m / m^k M_m$ qui transforme la classe d’un élément $x \in M$ en la classe de $x/1$.

#### Corollaire {#ac-ii-s3-n3-cor-1 .statement}

Soient $A$ un anneau, $m_1, m_2, ..., m_n$ des idéaux maximaux de $A$ deux à deux distincts, $M$ un $A$-module, $k_1, k_2, ..., k_n$ des entiers $\geqslant 0$. L’homomorphisme canonique de $M$ dans $\prod_{i=1}^n M_{m_i} / m_i^{k_i} M_{m_i}$ est surjectif, et son noyau est $\left( \bigcap_{i=1}^n m_i^{k_i} \right) M$.

Cela résulte aussitôt de la prop. 9 et du $§ 1$, n° 2, prop. 6, les $m_i^{k_i}$ étant deux à deux étrangers ($§ 1$, n° 2, prop. 3).

Dans la suite de ce n°, $A$ désigne un anneau, et $\Omega(A)$ (ou $\Omega$) l’ensemble des idéaux maximaux de $A$.

#### Proposition 10 {#ac-ii-s3-prop-10 .statement}

Le $A$-module $\bigoplus_{m \in \Omega} A_m$, somme directe des $A_m$ pour $m \in \Omega$, est fidèlement plat.

En effet, chacun des $A_m$ est un $A$-module plat ($§ 2$, n° 4, th. 1), donc $E = \bigoplus_{m \in \Omega} A_m$ est plat (chap. I, $§ 2$, n° 3, prop. 2). En outre, pour tout idéal maximal $m$ de $A$, $mA_m$ est l’unique idéal maximal de $A_m$, donc $mA_m \neq A_m$, d’où on conclut que $mE \neq E$, et par suite $E$ est fidèlement plat (chap. I, $§ 3$, n° 1, prop. 1, d)).

#### Théorème 1 {#ac-ii-s3-thm-1 .statement}

Soient $M, N$ deux $A$-modules, $u : M \to N$ un $A$-homomorphisme et pour tout $m \in \Omega$, soit $u_m : M_m \to N_m$ le $A_m$-homomorphisme correspondant ($§ 2$, n° 2, Remarque 5). Pour que $u$ soit injectif (resp. surjectif, bijectif, nul) il faut et il suffit que, pour tout $m \in \Omega$, $u_{m}$ soit injectif (resp. surjectif, bijectif, nul).

En effet, dire que pour tout $m \in \Omega$, $u_{m}$ est injectif (resp. surjectif, bijectif, nul) équivaut à dire que l’homomorphisme $\bigoplus_{m} u_{m} : \bigoplus_{m} M_{m} \to \bigoplus_{m} N_{m}$ a la même propriété. Mais $\bigoplus_{m} M_{m} = M \otimes_{A} E$, $\bigoplus_{m} N_{m} = N \otimes_{A} E$ et $\bigoplus_{m} u_{m} = u \otimes 1$, avec $E = \bigoplus_{m} A_{m}$; comme $E$ est fidèlement plat (prop. 10), le théorème résulte du chap. I, § 3, no 1, prop. 1 c) et prop. 2.

#### Corollaire 1 {#ac-ii-s3-thm-1-cor-1 .statement}

Soient $M$ un $A$-module, $N$ un sous-module de $M$, $x$ un élément de $M$. Pour que $x \in N$, il faut et il suffit que, pour tout $m \in \Omega$, l’image canonique de $x$ dans $M_{m}$ appartienne à $N_{m}$.

Soit $\overline{x}$ la classe de $x$ dans $M/N$; dire que $x \in N$ signifie que l’application $A$-linéaire $u : \alpha \to \alpha \overline{x}$ de $A$ dans $M/N$ est nulle. Or $(M/N)_{m}$ s’identifie à $M_{m}/N_{m}$ (§ 2, no 4, th. 1) et $u_{m} : A_{m} \to M_{m}/N_{m}$ à l’application $\lambda \to \lambda \overline{x}_{m}$, où $\overline{x}_{m}$ est la classe mod. $N_{m}$ de l’image canonique de $x$ dans $M_{m}$. Comme la relation $u = 0$ équivaut à $u_{m} = 0$ pour tout $m$ en vertu du th. 1, cela prouve le corollaire.

#### Corollaire 2 {#ac-ii-s3-thm-1-cor-2 .statement}

Soit $M$ un $A$-module et, pour tout $m \in \Omega$, soit $f_{m}$ l’homomorphisme canonique $M \to M_{m}$. L’homomorphisme $x \to (f_{m}(x))$ de $M$ dans $\prod_{m \in \Omega} M_{m}$ est injectif.

En effet, en appliquant le cor. 1 à $N = 0$, on voit que la relation $x = 0$ équivaut à $f_{m}(x) = 0$ pour tout $m \in \Omega$.

#### Corollaire 3 {#ac-ii-s3-thm-1-cor-3 .statement}

(i) Soient $b$ un idéal de $A$, $a$ un élément de $A$. Pour que $a \in b$, il faut et il suffit que, pour tout $m \in \Omega$, l’image canonique de $a$ dans $A_{m}$ appartienne à $bA_{m}$.

(ii) En particulier, soient $b$ et $c$ deux éléments de $A$. Pour que $c$ soit multiple de $b$, il faut et il suffit que, pour tout $m \in \Omega$, l’image canonique de $c$ dans $A_{m}$ soit multiple de celle de $b$.

Comme $bA_{m} = b_{m}$ (§ 2, no 7, cor. de la prop. 18), (i) est un cas particulier du cor. 1 ; (ii) résulte de (i) appliqué à l’idéal $Ab$.

#### Corollaire 4 {#ac-ii-s3-thm-1-cor-4 .statement}

Soient $A$ un anneau intègre, $K$ son corps des fractions, $M$ un $A$-module sans torsion, de sorte que $M$ s’identifie canoniquement à un sous-A-module de $K \otimes_A M$. Alors, pour tout $m \in \Omega$, $M_m$ s’identifie canoniquement à un sous-A-module de $K \otimes_A M$, et on a $M = \bigcap_{m \in \Omega} M_m$.

En effet, comme $M$ est identifié à un sous-module de $K \otimes_A M$, $M_m$ l’est à un sous-$A_m$-module de $(K \otimes_A M)_m = K_m \otimes_A M$ (§ 2, no 4, th. 1); comme $K_m = K$, on voit déjà que $M_m$ est sans torsion; en outre, la commutativité du diagramme

$$
\begin{array}{ccc}
M & \longrightarrow & K \otimes_A M \\
\downarrow & & \downarrow \\
M_m & \rightarrow & (K \otimes_A M)_m
\end{array}
$$

prouve que l’application canonique $M \to M_m$ est injective. Le corollaire résulte donc du cor. 1 appliqué au A-module $K \otimes_A M$ et à son sous-module $M$.

En particulier, pour tout anneau intègre $A$, on a

$$(2)$$
$$
A = \bigcap_{m \in \Omega} A_m.
$$

#### Corollaire 5 {#ac-ii-s3-thm-1-cor-5 .statement}

Soit $A$ un anneau. Tout système de générateurs du $A$-module $A^n$ ayant $n$ éléments est une base de $A^n$.

Soient $(e_i)_{1 \leq i \leq n}$ la base canonique de $A^n$, $(x_i)_{1 \leq i \leq n}$ un système de générateurs de $A^n$ ayant $n$ éléments, $u : A^n \to A^n$ l’application $A$-linéaire telle que $u(e_i) = x_i$ pour $1 \leq i \leq n$. Par hypothèse $u$ est surjective et il faut montrer que $u$ est injective. On se ramène aussitôt, en vertu du th. 1, au cas où $A$ est un anneau local; si $m$ est l’idéal maximal de $A$, les éléments $1 \otimes x_i (1 \leq i \leq n)$ dans $(A/m)^n$ forment alors un système de générateurs du $(A/m)$-module libre $(A/m)^n$; comme $A/m$ est un corps, ce système est une base de $(A/m)^n$; comme $A^n$ est un $A$-module libre, on déduit de la prop. 5 que $(x_i)$ est une base de $A^n$.

#### Proposition 11 {#ac-ii-s3-prop-11 .statement}

Soient $M$ un $A$-module, $N$ un $A$-module de type fini, $u : M \to N$ un homomorphisme. Pour que $u$ soit surjectif, il faut et il suffit que, pour tout $m \in \Omega$, l’homomorphisme $M/mM \to N/mN$ déduit de $u$ par passage aux quotients soit surjectif.

En effet, il résulte du th. 1 que, pour que $u$ soit surjectif, il faut et il suffit que $u_m : M_m \to N_m$ soit surjectif pour tout $m \in \Omega$. Comme $A_m$ est un anneau local et que $N_m$ est un $A_m$-module de type fini, il revient au même de dire que l’homomorphisme $u'_m : M_m / mM_m \to N_m / mN_m$, obtenu par passage aux quotients, est surjectif (no 2, cor. 1 de la prop. 4); mais $M_m / mM_m$ (resp. $N_m / mN_m$) s’identifie à $M / mM$ (resp. $N / mN$) (prop. 9), d’où la proposition.

#### Proposition 12 {#ac-ii-s3-prop-12 .statement}

Soient $E, F, G$ trois $A$-modules, $\nu : G \to F$ et $u : E \to F$ des homomorphismes. On suppose que $E$ est de présentation finie. Pour qu’il existe un homomorphisme $\omega : E \to G$ tel que $u$ se factorise en $u : E \xrightarrow{\nu} G \xrightarrow{v} F$, il faut et il suffit que, pour tout $m \in \Omega$, il existe un homomorphisme $\omega^m : E_m \to G_m$ tel que $u_m : E_m \to F_m$ se factorise en $E_m \xrightarrow{\omega^m} G_m \xrightarrow{v^m} F_m$.

L’existence de $\omega$ vérifiant l’énoncé est équivalente à la propriété suivante : $u$ appartient à l’image $P$ de l’application $r = \mathrm{Hom}(1_E, \nu) : \mathrm{Hom}_A(E, G) \to \mathrm{Hom}_A(E, F)$. Or, $(\mathrm{Hom}_A(E, F))_m$ (resp. $(\mathrm{Hom}_A(E, G))_m$) s’identifie canoniquement à $\mathrm{Hom}_{A_m}(E_m, F_m)$ (resp. $\mathrm{Hom}_{A_m}(E_m, G_m)$) (§ 2, no 7, prop. 19, (i)), l’image canonique de $u$ dans $(\mathrm{Hom}_A(E, F))_m$ s’identifie à $u_m$, $r_m$ s’identifie à $\mathrm{Hom}_{A_m}(1_{E_m}, \nu_m)$ et $P_m$ à l’image de $r_m$. La proposition résulte alors du cor. 1 du th. 1 appliqué à $\mathrm{Hom}_A(E, F)$ et à son sous-module $P$.

#### Corollaire 1 {#ac-ii-s3-prop-12-cor-1 .statement}

Soient $M$ un $A$-module, $N$ un sous-module de $M$ tel que $M/N$ admette une présentation finie. Pour que $N$ soit facteur direct de $M$, il faut et il suffit que, pour tout $m \in \Omega$, $N_m$ soit facteur direct de $M_m$.

En effet, dire que $N$ est facteur direct de $M$ signifie que l’homomorphisme identique de $M/N$ se factorise en $M/N \xrightarrow{\omega} M \xrightarrow{\varphi} M/N$ où $\varphi$ est l’homomorphisme canonique et $\omega$ un homomorphisme ($Alg.$, chap. II, 3e éd., § 1, no 9, prop. 14); comme $(M/N)_m = M_m / N_m$ et que $\varphi_m$ est l’homomorphisme canonique $M_m \to M_m / N_m$, le corollaire résulte aussitôt de la prop. 12.

#### Corollaire 2 {#ac-ii-s3-prop-12-cor-2 .statement}

Soient $M$ un $A$-module libre de type fini, $N$ un sous-module de $M$ qui est un $A$-module libre de type fini. Pour que $N$ soit facteur direct de $M$, il faut et il suffit que, pour tout $m \in \Omega$, on ait $mN = N \cap (mM)$.

En effet, par définition $M/N$ admet une présentation finie ; d’autre part, $N_m$ et $M_m$ sont des $A_m$-modules libres de type fini. Pour que $N_m$ soit facteur direct de $M_m$, il faut et il suffit que l’application canonique $N_m/mN_m \to M_m/mM_m$ soit injective (no 2, prop. 6) ; il revient au même de dire que l’application canonique $N/mN \to M/mM$ doit être injective (prop. 9), et comme son noyau est $(N \cap mM)/mN$, cela démontre le corollaire.

La prop. 12 (resp. son corollaire 1) s’appliquera en particulier lorsque $A$ est noethérien et $E$ (resp. $M/N$) un $A$-module de type fini (chap. I, § 2, no 8, lemme 8).

### 4. Localisation de la platitude.

#### Proposition 13 {#ac-ii-s3-prop-13 .statement}

Soient $S$ une partie multiplicative d’un anneau $A$, et $M$ un $A$-module. Si $M$ est plat (resp. fidèlement plat), $S^{-1}M$ est un $S^{-1}A$-module plat (resp. fidèlement plat), et un $A$-module plat.

Comme $S^{-1}M = M \otimes_A S^{-1}A$, la première assertion résulte du chap. I, § 2, no 7, cor. 2 de la prop. 8 (resp. du chap. I, § 3, no 3, prop. 5) ; en outre, $S^{-1}A$ est un $A$-module plat ($§ 2$, no 4, th. 1) ; donc, si $M$ est un $A$-module plat, il en est de même de $S^{-1}M$ en vertu du chap. I, § 2, no 7, cor. 3 de la prop. 8.

#### Remarque {#ac-ii-s3-n4-rem-1 .statement}

Si $N$ est un $S^{-1}A$-module, $S^{-1}N$ s’identifie à $N$, et il est par suite équivalent de dire que $N$ est un $S^{-1}A$-module plat ou un $A$-module plat.

#### Proposition 14 {#ac-ii-s3-prop-14 .statement}

Soient $A$ un anneau, $B$ une $A$-algèbre commutative, $T$ une partie multiplicative de $B$. Si $N$ est un $B$-module qui est plat en tant que $A$-module, $T^{-1}N$ est un $A$-module plat.

On a en effet $T^{-1}N = T^{-1}B \otimes_B N$ ; la proposition résulte alors du chap. I, § 2, no 7, prop. 8, appliquée en remplaçant $A$ par $B$, $B$ par $A$, $E$ par $T^{-1}B$ et $F$ par $N$.

#### Proposition 15 {#ac-ii-s3-prop-15 .statement}

Soient $A, B$ deux anneaux, $\varphi : A \to B$ un homomorphisme, $N$ un $B$-module. Les propriétés suivantes sont équivalentes :

a) $N$ est un $A$-module plat.

b) Pour tout idéal maximal $n$ de $B$, $N_n$ est un $A$-module plat.

c) Pour tout idéal maximal $n$ de $B$, si l’on pose $m = \overline{\varphi}(n)$, $N_n$ est un $A_m$-module plat.

Pour tout $a \in m$, l’homothétie de $N_n$ produite par $a$ est bijective, donc $N_n$ s’identifie canoniquement à $(N_n)_m$, et l’équivalence de b) et c) résulte de la Remarque suivant la prop. 13 ; le fait que a) entraîne b) est un cas particulier de la prop. 14. Reste à prouver que b) entraîne a), c’est-à-dire que, si b) est vérifiée, pour tout homomorphisme injectif $u : M \to M'$ de $A$-modules, l’homomorphisme $\varphi = 1 \otimes u : N \otimes_A M \to N \otimes_A M'$ est injectif. Or, $\varphi$ est aussi un homomorphisme de $B$-modules, et pour qu’il soit injectif, il faut et il suffit que $\varphi_n : (N \otimes_A M)_n \to (N \otimes_A M')_n$ le soit pour tout idéal maximal $n$ de $B$ (no 3, th. 1). Comme

$$
(N \otimes_A M)_n = B_n \otimes_B (N \otimes_A M) = N_n \otimes_A M,
$$

$\varphi_n$ n’est autre que l’homomorphisme $1 \otimes u : N_n \otimes_A M \to N_n \otimes_A M'$, qui est injectif puisque $N_n$ est un $A$-module plat par hypothèse.

#### Corollaire {#ac-ii-s3-n4-cor-1 .statement}

Pour qu’un $A$-module $M$ soit plat (resp. fidèlement plat) il faut et il suffit que, pour tout idéal maximal $m$ de $A$, $M_m$ soit un $A_m$-module plat (resp. fidèlement plat).

La nécessité des conditions résulte de la prop. 13. Inversement, si $M_m$ est un $A_m$-module plat pour tout idéal maximal $m$ de $A$, $M$ est un $A$-module plat en vertu de la prop. 15 appliquée au cas où $\varphi$ est l’identité. Enfin, si $M_m$ est un $A_m$-module fidèlement plat pour tout $m$, on a $mM_m = mA_m M_m \neq M_m$, donc $mM \neq M$ pour tout $m$ (no 3, prop. 9), ce qui prouve que $M$ est un $A$-module fidèlement plat (chap. I, § 3, no 1, prop. 1, d)).

### 5. Anneaux semi-locaux.

#### Proposition 16 {#ac-ii-s3-prop-16 .statement}

Soit $A$ un anneau. Les conditions suivantes sont équivalentes :

a) l’ensemble des idéaux maximaux de $A$ est fini ;

b) le quotient de $A$ par son radical est composé direct d’un nombre fini de corps.

Supposons que le quotient de $A$ par son radical $\mathcal{R}$ soit composé direct d’un nombre fini de corps. Alors $A/\mathcal{R}$ ne possède qu’un nombre fini d’idéaux et *a fortiori* n’a qu’un nombre fini d’idéaux maximaux. Comme tout idéal maximal contient $\mathcal{R}$ (*Alg.*, chap. VIII, § 6, n° 2, déf. 2), les idéaux maximaux de $A$ sont les images réciproques des idéaux maximaux de $A/\mathcal{R}$ par l’homomorphisme canonique $A \to A/\mathcal{R}$; ils sont donc en nombre fini.

Réciproquement, supposons que $A$ ne possède qu’un nombre fini d’idéaux maximaux distincts $m_1, ..., m_n$. Les $A/m_i$ sont des corps, et il résulte du § 1, n° 2, prop. 5, que l’application canonique $A \to \prod_{i=1}^n A/m_i$ est surjective ; comme son noyau $\bigcap_{i=1}^n m_i$ est le radical $\mathcal{R}$ (*Alg.*, chap. VIII, § 6, n° 2, déf. 2), $A/\mathcal{R}$ est isomorphe à $\prod_{i=1}^n A/m_i$.

#### Définition 4 {#ac-ii-s3-def-4 .statement}

*On dit qu’un anneau est semi-local s’il satisfait aux conditions équivalentes a), b) de la prop. 16.*

#### Exemple {#ac-ii-s3-n5-exa-1 .statement}

Tout anneau local est semi-local. Tout quotient d’un anneau semi-local est semi-local. Tout produit fini d’anneaux semi-locaux est semi-local. *Si $A$ est un anneau semi-local noethérien, et si $B$ est une $A$-algèbre qui est un $A$-module de type fini, alors $B$ est semi-local (chap. IV, § 2, n° 5, cor. 3 de la prop. 9).*

Un autre exemple, généralisant la construction des anneaux locaux $A_p$, est fourni par la proposition suivante :

#### Proposition 17 {#ac-ii-s3-prop-17 .statement}

*Soient $A$ un anneau, $p_1, ..., p_n$ des idéaux premiers de $A$. Posons $S = \bigcap_{i=1}^n (A - p_i) = A - \bigcup_{i=1}^n p_i$.

a) *L’anneau $S^{-1}A$ est semi-local ; si $q_1, ..., q_r$ sont les éléments maximaux distincts (pour la relation d’inclusion) de l’ensemble des p_i, les idéaux maximaux de S^{-1}A sont les S^{-1}q_j (1 \leq j \leq r), et ces idéaux sont deux à deux distincts.

b) L’anneau $A_{p_i}$ est canoniquement isomorphe à $(S^{-1}A)_{S^{-1}p_i}$ pour $1 \leq i \leq n$.

c) Si A est intègre, on a $S^{-1}A = \bigcap_{i=1}^{n} A_{p_i}$ dans le corps des fractions de A.

a) Les idéaux de A ne rencontrant pas S sont les idéaux contenus dans la réunion des $p_i$, donc dans l’un des $p_i$ au moins ($§ 1$, no 1, prop. 2); les $q_j$ sont donc les éléments maximaux de l’ensemble des idéaux ne rencontrant pas S; par suite, les $S^{-1}q_j$ sont les idéaux maximaux de $S^{-1}A$ en vertu du $§ 2$, no 5, prop. 11, (ii).

b) est un cas particulier du $§ 2$, no 5, prop. 11, (iii).

c) Supposons A intègre. Si $p_i \subset p_k$, on a $A_{p_i} \supset A_{p_k}$; pour prouver c), on peut donc supposer les $p_i$ non comparables deux à deux. Il résulte alors de a) et du no 3, cor. 4 du th. 1, que l’on a
$$
S^{-1}A = \bigcap_{i=1}^{n} (S^{-1}A)_{S^{-1}p_i}; \text{ d’où } c),
$$
en vertu de b).

Si A est intègre, il en est de même de $S^{-1}A$, et la prop. 17 fournit donc un exemple d’anneau semi-local qui n’est pas composé direct d’anneaux locaux (cf. chap. III, $§ 2$, no 13).

#### Corollaire {#ac-ii-s3-n5-cor-1 .statement}

Soient A un anneau intègre, $p_1, ..., p_n$ des idéaux premiers de A, non comparables deux à deux pour la relation d’inclusion. Si $A = \bigcap_{i=1}^{n} A_{p_i}$ dans le corps des fractions de A, les idéaux maximaux de A sont $p_1, ..., p_n$.

Posant $S = \bigcap_{i=1}^{n} (A - p_i)$, on a $S^{-1}A = A$ en vertu de la prop. 17 c); donc les éléments de S sont inversibles dans A, et on a $S^{-1}p_i = p_i$ pour tout $i$. D’où notre assertion en vertu de la prop. 17 a).

## EXERCICES {#ac-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
