---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: Idéaux premiers associés et décomposition primaire
section: 3
section_title: Décomposition primaire dans les modules gradués
lang: fr
source: ac-i-iv-fr
pdf_pages: 0332-0336, 0351-0352
extraction: ocr
subsections:
    - "no": 1
      title: Idéaux premiers associés à un module gradué.
      page: 0
      pdf_page: 332
    - "no": 2
      title: Sous-modules primaires correspondant aux idéaux premiers gradués.
      page: 0
      pdf_page: 334
    - "no": 3
      title: Décomposition primaire dans les modules gradués.
      page: 0
      pdf_page: 335
statements: 6
exercises: 3
content_sha256: b716f6cf2dd0bf60045addebda4ba042705d015e4eb20af7db7214000c6f8fa1
---

## § 3. Décomposition primaire dans les modules gradués

### 1. Idéaux premiers associés à un module gradué.

#### Proposition 1 {#ac-iv-s3-prop-1 .statement}

Soient $\Delta$ un groupe commutatif sans torsion, $A$ un anneau gradué de type $\Delta$, $M$ un $A$-module gradué de type $\Delta$. Tout idéal premier associé à $M$ est gradué, et est l’annulateur d’un élément homogène de $M$.

On sait qu’on peut munir $\Delta$ d’une structure d’ordre total compatible avec sa structure de groupe ($Alg.$, chap. II, 3e éd., § 11, no 4, lemme 2). Soit $p$ un idéal premier associé à $M$, annulateur d’un élément $x \in M$, et soit $(x_i)_{i \in \Delta}$ la famille des composantes homogènes de $x$; soient $i(1) < i(2) < \ldots < i(r)$ les valeurs de $i$ pour lesquelles $x_i \neq 0$. Considérons un élément $a \in p$, et soit $(a_i)_{i \in \Delta}$ la famille de ses composantes homogènes ; nous allons prouver que l’on a $a_i \in \mathfrak{p}$ pour tout $i \in \Delta$, ce qui montrera que $\mathfrak{p}$ est un idéal gradué.

Raisonnons par récurrence sur le nombre des indices $i$ tels que $a_i \neq 0$. Notre assertion est évidente si ce nombre est 0 ; sinon, soit $m$ le plus grand des indices $i$ pour lesquels $a_i \neq 0$ ; si nous prouvons que $a_m \in \mathfrak{p}$, l’hypothèse de récurrence appliquée à $a - a_m$ permettra de conclure. Or, on a $ax = 0$ ; pour tout $j \in \Delta$, en écrivant que la composante homogène de degré $m + j$ de $ax$ est 0, il vient $\sum_{i \in \Delta} a_{m-i} x_{j+i} = 0$ ; on en conclut que $a_m x_j$ est combinaison linéaire des $x_i$ pour les indices $i > j$. En particulier, on a donc $a_m x_{i(r)} = 0$, d’où, par récurrence descendante sur $n < r$, $a_m^{r-n+1} x_{i(n)} = 0$. On a par suite $a_m^r x = 0$, d’où $a_m^r \in \mathfrak{p}$, et comme $\mathfrak{p}$ est premier, $a_m \in \mathfrak{p}$.

Montrons maintenant que $\mathfrak{p}$ est l’annulateur d’un élément homogène de M. Posons $b_n = \operatorname{Ann}(x_{i(n)})$ pour $1 \leq n \leq r$. Pour tout élément homogène $b$ de $\mathfrak{p}$ et tout $n$, la composante homogène de $bx$ de degré $i(n) + \deg(b)$ est $bx_{i(n)}$, donc $bx_{i(n)} = 0$ et par suite $b \in b_n$ ; comme $\mathfrak{p}$ est engendré par ses éléments homogènes, on a $\mathfrak{p} \subset b_n$. D’autre part, il est clair que $\bigcap_{n=1}^r b_n \subset \operatorname{Ann}(x) = \mathfrak{p}$; comme $\mathfrak{p}$ est premier, il existe un $n$ tel que $b_n \subset \mathfrak{p}$ (chap. II, § 1, no 1, prop. 1), d’où $b_n = \mathfrak{p} = \operatorname{Ann}(x_{i(n)})$, ce qui achève la démonstration.

#### Corollaire {#ac-iv-s3-n1-cor-1 .statement}

Pour tout idéal premier (nécessairement gradué) $\mathfrak{p}$ associé à un A-module gradué M, il existe un indice $k \in \Delta$ tel que le A-module gradué $(A/\mathfrak{p})(k)$ obtenu par décalage des degrés de $k$ à partir du A-module gradué $A/\mathfrak{p}$ (Alg., chap. II, 3e éd., § 11, no 2) soit isomorphe à un sous-module gradué de M.

Avec les notations de la démonstration de la prop. 1, considérons en effet l’homomorphisme déduit par passage au quotient de l’homomorphisme $a \to ax_{i(n)}$ de A dans M ; ce dernier est un homomorphisme gradué de degré $i(n)$, donc il donne par passage au quotient un homomorphisme bijectif gradué de degré $i(n)$ de $A/\mathfrak{p}$ sur un sous-module gradué de M.

#### Proposition 2 {#ac-iv-s3-prop-2 .statement}

Soient $\Delta$ un groupe commutatif sans torsion, $A$ un anneau noethérien gradué de type $\Delta$, $M$ un $A$-module de type fini, gradué de type $\Delta$. Il existe une suite de composition $(M_i)_{0 \leq i \leq n}$ formée de sous-modules gradués de $M$ telle que, pour $0 \leq i \leq n - 1$, le module gradué $M_i / M_{i+1}$ soit isomorphe à un module gradué décalé $(A/p_i)(k_i)$, où $p_i$ est un idéal premier gradué de $A$ et $k_i \in \Delta$.

Il suffit de reprendre le raisonnement du § 1, no 4, th. 1, en prenant cette fois pour $\mathfrak{G}$ l’ensemble des sous-modules gradués de $M$ possédant une suite de composition ayant les propriétés de l’énoncé ; on conclut en utilisant le cor. de la prop. 1.

### 2. Sous-modules primaires correspondant aux idéaux premiers gradués.

#### Proposition 3 {#ac-iv-s3-prop-3 .statement}

Soient $\Delta$ un groupe commutatif sans torsion, $A$ un anneau noethérien gradué de type $\Delta$, $p$ un idéal gradué de $A$, $M$ un $A$-module gradué de type $\Delta$, non réduit à 0. On suppose que pour tout élément homogène $a$ de $p$, l’homothétie de rapport $a$ dans $M$ est presque nilpotente et que pour tout élément homogène $b$ de $A - p$, l’homothétie de rapport $b$ dans $M$ est injective. Alors $p$ est premier et le sous-module $\{0\}$ de $M$ est $p$-primaire.

Il suffit de montrer que $\operatorname{Ass}(M) = \{p\}$ (§ 2, no 1, prop. 1). Soit $q$ un idéal premier associé à $M$; c’est un idéal gradué, et il est l’annulateur d’un élément homogène $x \neq 0$ de $M$ (no 1, prop. 1). Pour tout élément homogène $a$ de $q$, on a $ax = 0$, donc l’homothétie de rapport $a$ dans $M$ n’est pas injective, d’où $a \in p$. Inversement, soit $b$ un élément homogène de $p$; il existe un entier $n > 0$ tel que $b^n x = 0$, d’où $b^n \in \operatorname{Ann}(x) = q$, et comme $q$ est premier, $b \in q$. Comme $p$ et $q$ sont engendrés par leurs éléments homogènes respectifs, on a $p = q$, ce qui prouve que $\operatorname{Ass}(M) \subset \{p\}$. Comme $M \neq \{0\}$, on a $\operatorname{Ass}(M) \neq \emptyset$ (§ 1, no 1, cor. 1 de la prop. 2), d’où $\operatorname{Ass}(M) = \{p\}$.

#### Proposition 4 {#ac-iv-s3-prop-4 .statement}

Soient $\Delta$ un groupe commutatif sans torsion, $A$ un anneau noethérien gradué de type $\Delta$, $M$ un $A$-module gradué de type $\Delta$. Soient $p$ un idéal premier de $A$, $N$ un sous-module de $M$, $p$-primaire par rapport à $M$.

(i) Le plus grand idéal gradué $p'$ de $A$ contenu dans $p$ (Alg., chap. II, 3e éd., § 11, no 3) est premier.

(ii) Le plus grand sous-module gradué $N'$ de $N$ est $p'$-primaire par rapport à $M$.

On sait (loc. cit.) que les éléments homogènes de $p'$ (resp. $N'$) ne sont autres que les éléments homogènes de $p$ (resp. $N$). Soit $a$ un élément homogène de $p$; si $x$ est un élément homogène de $M$, il existe un entier $n > 0$ tel que $a^n x \in N$; comme $a^n x$ est homogène, on a $a^n x \in N'$; comme tout $y \in M$ est somme d’un nombre fini d’éléments homogènes, on en conclut qu’il existe un entier $q > 0$ tel que $a^q y \in N'$, de sorte que l’homothétie de rapport $a$ dans $M/N'$ est presque nilpotente.

Considérons maintenant un élément homogène $b$ de $A - p'$; on a $b \notin p$ puisque $b$ est homogène. Soit $x$ un élément de $M$ tel que $bx \in N'$, et soit $(x_i)_{i \in \Delta}$ la famille des composantes homogènes de $x$. Comme $N'$ est gradué, on a $bx_i \in N'$ pour tout $i$, donc $bx_i \in N$, et comme $b \notin p$ on en conclut que $x_i \in N$; comme $x_i$ est homogène, on a $x_i \in N'$, d’où $x \in N'$ et l’homothétie de rapport $b$ dans $M/N'$ est injective. La prop. 4 résulte alors de la prop. 3 appliquée à $p'$ et à $M/N'$.

### 3. Décomposition primaire dans les modules gradués.

#### Proposition 5 {#ac-iv-s3-prop-5 .statement}

Soient $\Delta$ un groupe commutatif sans torsion, $A$ un anneau noethérien gradué de type $\Delta$, $M$ un $A$-module gradué de type $\Delta$, $N$ un sous-module gradué de $M$, et soit $N = \bigcap_{i \in I} Q_i$ une décomposition primaire de $N$ dans $M$.

(i) Soit $Q'_i$ le plus grand sous-module gradué de $M$ contenu dans $Q_i$. Alors les $Q'_i$ sont primaires et on a $N = \bigcap_{i \in I} Q'_i$.

(ii) Si la décomposition primaire $N = \bigcap_{i \in I} Q_i$ est réduite, il en est de même de la décomposition primaire $N = \bigcap_{i \in I} Q'_i$, et pour tout $i \in I$, les idéaux premiers correspondant à $Q_i$ et à $Q'_i$ sont égaux.

(iii) Si $Q_i$ correspond à un idéal premier $p_i$ qui est un élément minimal de $\operatorname{Ass}(M/N)$, $Q_i$ est un sous-module gradué de $M$.

On a vu (n° 2, prop. 4) que les $Q'_i$ sont primaires par rapport à $M$, et on a $N \subset Q'_i \subset Q_i$, ce qui démontre (i). La prop. 4 du n° 2 montre aussi que l’idéal premier $p'_i$ correspondant à $Q'_i$ est le plus grand idéal gradué contenu dans l’idéal premier $p_i$ correspondant à $Q_i$. Si la décomposition $N = \bigcap_{i \in I} Q_i$ est réduite, on a $p_i \in \operatorname{Ass}(M/N)$ pour tout $i$ (§ 2, n° 3, prop. 4), donc $p_i$ est un idéal gradué (n° 1, prop. 1) et par suite $p'_i = p_i$; on a donc $\operatorname{Ass}(M/N) = \bigcup_{i \in I} \{ p'_i \}$ (§ 2, n° 3, prop. 4), ce qui prouve que la décomposition $N = \bigcap_{i \in I} Q'_i$ est réduite (§ 2, n° 3, prop. 4). Enfin, si $p_i$ est un élément minimal de $\operatorname{Ass}(M/N)$, on a $p'_i = p_i$ puisque $p_i$ est gradué (n° 1, prop. 1), d’où $Q'_i = Q_i$ en vertu du § 2, n° 3, prop. 5.

## EXERCICES {#ac-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
