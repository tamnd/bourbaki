---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION DE LA MATHÉMATIQUE FORMELLE
section: 0
section_title: Caractérisation des termes et des relations
appendix: true
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0043-0047, 0050-0052
extraction: ocr
subsections:
    - "no": 1
      title: Signes et mots
      page: 42
      pdf_page: 43
    - "no": 2
      title: Mots significatifs
      page: 43
      pdf_page: 44
    - "no": 3
      title: Caractérisation des mots significatifs
      page: 43
      pdf_page: 44
    - "no": 4
      title: Application aux assemblages d’une théorie mathématique
      page: 45
      pdf_page: 46
statements: 7
exercises: 8
content_sha256: 1687bd895d5f8fe5d63bf17d4ad4a21f61a12637b2e654e620f89a03efb97913
---

## APPENDICE

# CARACTÉRISATION DES TERMES ET DES RELATIONS

La métamathématique, lorsqu’elle dépasse le niveau très élémentaire du présent chapitre, utilise largement les résultats de la mathématique; nous l’avons signalé dans l’Introduction. Le but de cet Appendice est de donner un exemple simple de ce genre de raisonnements. Nous commencerons par établir certains résultats qui se rattachent à la théorie mathématique des monoïdes libres (A, I, § 7, no 2); nous en ferons ensuite l’ « application » métamathématique à la caractérisation des termes et relations d’une théorie.

### 1. Signes et mots

\* Soit $S$ un ensemble non vide, dont les éléments seront appelés signes dans ce qui suit (cette terminologie étant appropriée à l’application métamathématique que nous avons en vue). Soit $L_0(S)$ le monoïde libre construit sur $S$ (A, I, § 7, no 2) dont les éléments (appelés mots) sont identifiés aux suites finies $A=(s_i)_{0\leq i\leq n}$ d’éléments de $S$; nous noterons multiplicativement la loi de composition dans $L_0(S)$, $AB$ étant donc la suite obtenue par juxtaposition de $A$ et de $B$. Le mot vide $\varnothing$ est élément neutre de $L_0(S)$. Rappelons que la longueur $l(A)$ d’un mot $A\in L_0(S)$ est le nombre d’éléments de la suite $A$; on a $l(AB)=l(A)+l(B)$; les mots de longueur $1$ sont les signes. Nous désignerons par $L(S)$ l’ensemble des mots non vides de $L_0(S)$.

Supposons en outre donnée une application $s\mapsto n(s)$ de $S$ dans l’ensemble $\mathbf{N}$ des entiers $\geq 0$; pour tout mot non vide $A=(s_i)_{0\leq i\leq k}$ de $L(S)$, on pose $n(A)=$ $\sum_{i=0}^{k} n(s_i)$, et $n(\varnothing)=0$; on dit que $n(A)$ est le poids de $A$. On a évidemment
$n(AB)=n(A)+n(B)$.

Si $A=A'BA''$, on dit que le mot $B$ est un segment de $A$ (segment propre si en outre $B\ne A$). Si $A'$ (resp. $A''$) est vide, on dit que $B$ est un segment initial (resp. final) de $A$. Si $l(A')=k$, on dit que $B$ commence à la $(k+1)$-ème place.

Si $A=BCDEF$ (où les mots $B,C,D,E,F$ peuvent être vides), on dit que les segments $C$ et $E$ de $A$ sont disjoints.

### 2. Mots significatifs

Nous appellerons suite significative toute suite $(A_i)_{1\leq i\leq n}$ de mots de $L_0(S)$ qui possède la propriété suivante: pour chaque mot $A_i$ de la suite, l’une des deux conditions suivantes est vérifiée:

1° $A_i$ est un signe de poids 0.

2° Il existe $p$ mots $A_{i_1},A_{i_2},\ldots,A_{i_p}$ de la suite, d’indices $<i$, et un signe $f$ de poids $p$, tels que $A_i=fA_{i_1}A_{i_2}\ldots A_{i_p}$.

On appelle mots significatifs les mots qui figurent dans les suites significatives.
On a immédiatement le résultat suivant:

#### Proposition 1 {#ens-i-a0-prop-1 .statement tag=03P6}

Si $A_1,A_2,\ldots,A_p$ sont $p$ mots significatifs et $f$ un signe de poids $p$, le mot $fA_1A_2\ldots A_p$ est significatif.

### 3. Caractérisation des mots significatifs

Un mot $A\in L_0(S)$ est dit équilibré s’il possède les deux propriétés suivantes:

1° $l(A)=n(A)+1$ (ce qui implique que $A$ n’est pas vide).

2° Pour tout segment initial propre $B$ de $A$, on a $l(B)\leq n(B)$.

#### Proposition 2 {#ens-i-a0-prop-2 .statement tag=03P7}

Pour qu’un mot soit significatif, il faut et il suffit qu’il soit équilibré.

En effet, soit $A$ un mot significatif, figurant dans une suite significative $A_1,A_2,\ldots,A_n$; nous allons montrer, par récurrence sur $k$, que chacun de ces $A_k$ est équilibré. Supposons ceci établi pour les $A_j$ d’indice $j<k$, et prouvons-le pour $A_k$. Si $A_k$ est un signe de poids 0 (ce qui est la seule hypothèse possible pour $k=1$), $A_k$ est équilibré puisque $l(A_k)=1$ et $n(A_k)=0$. Sinon, $A_k=fB_1B_2\ldots B_p$ où $f$ est un signe de poids $p$, et les $B_j$ sont de la forme $A_{i_j}$, avec $i_j<k$, donc sont des mots équilibrés par hypothèse. On a

$$
l(A_k)=1+l(B_1)+l(B_2)+\ldots+l(B_p)
$$

$$
=1+(n(B_1)+1)+(n(B_2)+1)+\ldots+(n(B_p)+1)
$$

$$
=1+p+n(B_1)+n(B_2)+\ldots+n(B_p)=1+n(A_k).
$$

Soit d’autre part $C$ un segment initial propre de $A_k$, et soit $q$ le plus grand des

E I.44                                                     DESCRIPTION DE LA MATHÉMATIQUE FORMELLE                                 Appendice

entiers $m < p$ tels que $B_m$ soit un segment de $C$; on a donc $C = fB_1B_2\ldots B_qD$,
où $D$ est un segment initial propre de $B_{q+1}$. Donc

$$
l(C)=1+l(B_1)+\cdots+l(B_q)+l(D)
$$

$$
\leq 1+(n(B_1)+1)+\cdots+(n(B_q)+1)+n(D)
$$

$$
\leq p+n(B_1)+\cdots+n(B_q)+n(D)=n(C).
$$

Donc $A_k$ est équilibré.
Pour prouver que, réciproquement, tout mot équilibré est significatif, nous avons besoin des deux lemmes suivants:

#### Lemme 1 {#ens-i-a0-lem-1 .statement tag=03P8}

Soit $A$ un mot équilibré. Pour tout entier $k$ tel que $0\leq k<l(A)$, il existe un segment équilibré $S$ de $A$ et un seul qui commence à la $(k+1)$-ième place.

L’unicité de $S$ résulte aussitôt de la remarque suivante: si $T$ est un mot équilibré, aucun segment initial propre de $T$ n’est équilibré par définition.
Prouvons l’existence de $S$. Posons $A=BC$ où $l(B)=k$. Pour tout $i$ tel que $0\leq i\leq q=l(C)$, soit $C_i$ le segment initial de $C$ de longueur $i$. Comme $B$ est un segment initial propre de $A$, on a

$$
l(C_q)=l(A)-l(B)\geq n(A)+1-n(B)=n(C_q)+1.
$$

D’autre part, on a $0=l(C_0)\leq n(C_0)=0$. Soit $i$ le plus grand des entiers
$j<q$ tels que $l(C_h)\leq n(C_h)$ pour $0\leq h\leq j$; on a donc $l(C_i)\leq n(C_i)$ et $l(C_{i+1})\geq n(C_{i+1})+1$. Montrons que $C_{i+1}$ est équilibré. La condition relative aux segments initiaux propres est vérifiée en raison de la définition de $i$. D’autre part, on a

$$
n(C_{i+1})+1\leq l(C_{i+1})=l(C_i)+1\leq n(C_i)+1\leq n(C_{i+1})+1
$$

donc $l(C_{i+1})=n(C_{i+1})+1$, ce qui achève la démonstration.

#### Lemme 2 {#ens-i-a0-lem-2 .statement tag=03GT}

Tout mot équilibré $A$ peut se mettre sous la forme $A=fA_1A_2\ldots A_p$, où les $A_i$ sont équilibrés et où $n(f)=p$.

En effet, soit $f$ le signe initial de $A$. D’après le lemme 1, $A$ peut s’écrire $fA_1A_2\ldots A_p$, où les $A_i$ sont équilibrés; il suffit de définir par récurrence $A_i$ comme étant le segment équilibré de $A$ commençant à la $k(i)$-ième place, où $k(i)=2+\sum_{j<i}l(A_j)$. On a en outre

$$
1+l(A_1)+\cdots+l(A_p)=l(A)=n(A)+1
$$

$$
=n(f)+n(A_1)+\cdots+n(A_p)+1
$$

$$
=n(f)+(l(A_1)-1)+\cdots+(l(A_p)-1)+1
$$

d’où $n(f)=p$.

Ces lemmes étant établis, on voit aussitôt, par récurrence sur la longueur de $A$, que tout mot équilibré $A$ est significatif, en raison du lemme 2 et de la prop. 1.

#### Corollaire 1 {#ens-i-a0-lem-2-cor-1 .statement tag=03GU}

Soit $A$ un mot significatif. Pour tout entier $k$ tel que $0\leq k<l(A)$,
il existe un segment significatif de $A$ et un seul qui commence à la $(k+1)$-ième place.

#### Corollaire 2 {#ens-i-a0-lem-2-cor-2 .statement tag=03GV}

Tout mot significatif $A$ peut se mettre, d’une manière et d’une seule, sous la forme $fA_1A_2\ldots A_p$, où les $A_i$ sont significatifs et où $n(f)=p$.

### 4. Application aux assemblages d’une théorie mathématique

Supposons que l’ensemble $S$ soit l’ensemble des signes d’une théorie mathématique $\mathcal T$. Nous poserons $n([\,])=0$, $n(\tau)=n(\neg)=1$, $n(\vee)=2$, $n(x)=0$ pour toute lettre $x$; enfin, pour tout signe spécifique $s$ de $\mathcal T$, $n(s)$ est le poids de $s$, fixé par la donnée de $\mathcal T$.

Soit $A$ un assemblage de $\mathcal T$. Nous désignerons par $A^*$ le mot obtenu en effaçant les liens de $A$, et nous dirons que $A$ est équilibré si $A^*$ est équilibré (dans $L_0(S)$). Nous appellerons segment de $A$ tout assemblage obtenu en munissant un segment $S$ de $A^*$ des liens qui, dans $A$, joignent deux signes de $S$.

**Critère 1.** — Si $A$ est un terme ou une relation de $\mathcal T$, $A$ est équilibré.

Soit en effet $A_1,A_2,\ldots,A_n$ une construction formative de $\mathcal T$ où figure $A$. Raisonnant par récurrence, supposons démontré que les $A_j$ d’indice $j<i$ sont équilibrés, et prouvons que $A_i$ est équilibré. Cela s’établit comme dans la première partie de la démonstration de la prop. 2, sauf lorsque $A_i$ est de la forme $\tau_x(B)$, avec $B=A_j$, $j<i$. Dans ce cas, soit $C$ l’assemblage obtenu en remplaçant $x$, en chacune de ses occurrences dans $B$, par $[\,]$; le mot $A_i^*$ est identique à $\tau C^*$; or $B^*$ est équilibré, donc $C^*$ est équilibré (puisque $n([\,])=n(x)=0$); par suite $A_i^*$ est équilibré.

Nous avons donc obtenu une condition nécessaire pour qu’un assemblage de $\mathcal T$ soit un terme ou une relation. Cette condition, on va le voir, n’est pas suffisante.

Soit $A$ un assemblage équilibré de $\mathcal T$. Si $A$ commence par une lettre ou un $[\,]$, $A$ se réduit nécessairement à ce signe initial (cor. 2 de la prop. 2). Dans tous les autres cas, nous allons définir le ou les assemblages antécédents à $A$.

1° Si $A$ commence par un $\tau$, ou un $\vee$, ou un signe spécifique, $A^*$ se met de manière unique sous la forme $fB_1B_2\ldots B_p$, $f$ étant un signe de poids $p\geq 1$ et les $B_i$ étant équilibrés (cor. 2 de la prop. 2). Nous appellerons assemblages antécédents à $A$ les segments $A_1,A_2,\ldots,A_p$ de $A$ qui correspondent aux segments $B_1,B_2,\ldots,B_p$ de $A^*$. En outre, nous dirons que $A$ est parfaitement équilibré si $A$ est identique à $fA_1A_2\ldots A_p$, autrement dit si, dans $A$, aucun lien ne joint $f$ à l’un des $B_i$, ou deux des $B_i$ distincts entre eux.

2° Si $A$ commence par un $\tau$, $A^*$ est de la forme $\tau B$, $B$ étant équilibré (cor. 2 de la prop. 2). Nous appellerons assemblage antécédent à $A$ l’un quelconque des assemblages $A_1$ définis de la façon suivante: on remplace les $[\,]$ de $B$ qui sont liés dans $A$ au $\tau$ initial par une lettre $x$ distincte des autres lettres figurant dans $B$, et on rétablit les liens qui joignent, dans $A$, deux signes de $B$. (Si, au lieu de $x$, on substitue une lettre $y$ qui ne figure pas non plus dans $B$, on obtient un assemblage qui n’est autre que $(y|x)A_1$.) En outre, nous dirons que $A$ est parfaitement

E I.46                                      DESCRIPTION DE LA MATHÉMATIQUE FORMELLE                                      Appendice

équilibré si A est identique à $\tau_x(A_1)$, autrement dit si aucun lien ne joint le $\tau$ initial à des signes de $B$ autres que des $\square$.

On peut alors énoncer le critère suivant:

**CRITÈRE 2.** — Soit $A$ un assemblage équilibré de $\mathcal{T}$.

Pour que $A$ soit un terme, il faut et il suffit que l’une des conditions suivantes soit vérifiée: 1) $A$ se réduit à une lettre; 2) $A$ commence par un $\tau$, est parfaitement équilibré, et les assemblages antécédents sont des relations (d’après CF8, il suffit de vérifier qu’un assemblage antécédent est une relation).

Pour que $A$ soit une relation, il faut et il suffit que l’une des conditions suivantes soit vérifiée: 1) $A$ commence par un $\vee$ ou un $\neg$, est parfaitement équilibré, et les assemblages antécédents sont des relations; 2) $A$ commence par un signe spécifique, est parfaitement équilibré, et les assemblages antécédents sont des termes.

Les conditions sont suffisantes d’après les critères CF1 à CF4 (I, p. 19). Montrons qu’elles sont nécessaires. Si $A$ est une relation, on a vu (I, p. 19) que $A$ commence par un $\vee$, ou un $\neg$, ou un signe spécifique. On raisonne de façon analogue dans les trois cas. Si par exemple $A$ commence par un $\vee$, $A$ est de la forme $\vee BC$, où $B$ et $C$ sont des relations, de sorte que $B$, $C$ sont les assemblages antécédents à $A$; $A$ est donc parfaitement équilibré. Si $A$ est un terme, ou bien il se réduit à une lettre, ou bien il commence par un $\tau$. Si $A$ commence par un $\tau$, la définition d’une construction formative prouve que $A$ est de la forme $\tau_x(B)$, où $B$ est une relation et $x$ une lettre, de sorte qu’on peut prendre $B$ pour assemblage antécédent à $A$ et que $A$ est parfaitement équilibré.

Lorsqu’on veut savoir si un assemblage donné $A$ (non réduit à une lettre) est une relation (resp. un terme) de $\mathcal{T}$, on vérifie d’abord que $A$ est équilibré, et qu’il commence par un $\vee$, un $\neg$ ou un signe spécifique (resp. un $\tau$). On forme le ou les assemblages antécédents, et on vérifie s’il y a lieu que $A$ est parfaitement équilibré. Ceci fait, on est ramené à un problème analogue, mais concernant des assemblages plus courts. De proche en proche, on est ramené à des assemblages dont chacun est réduit à un signe, pour lesquels la solution est immédiate.

#### Remarque {#ens-i-a0-n4-rem-1 .statement tag=03GW}

Sauf pour certaines théories mathématiques particulièrement pauvres en axiomes (I, p. 50, exerc. 7), on ne dispose pas, en général, d’un procédé du type précédent, permettant de savoir si une relation donnée $R$ d’une théorie $\mathcal{T}$ est un théorème de $\mathcal{T}$.

## EXERCICES {#ens-i-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
