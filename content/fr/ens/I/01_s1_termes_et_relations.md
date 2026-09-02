---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION DE LA MATHÉMATIQUE FORMELLE
section: 1
section_title: Termes et relations
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0015-0022, 0048-0048
extraction: ocr
subsections:
    - "no": 1
      title: Signes et assemblages
      page: 0
      pdf_page: 15
    - "no": 2
      title: Critères de substitution
      page: 0
      pdf_page: 17
    - "no": 3
      title: Constructions formatives
      page: 17
      pdf_page: 18
    - "no": 4
      title: Critères formatifs
      page: 0
      pdf_page: 20
statements: 8
exercises: 6
content_sha256: 14de471475b196e79411c41445b05c3903b39c5c82403ce3ceb0a73e9d31b79d
---

## § 1. TERMES ET RELATIONS

### 1. Signes et assemblages

Les signes d’une théorie mathématique $\mathcal{T}$[^1] sont les suivants:

1° Les signes logiques[^2]: $\square$, $\tau$, $\vee$, $\neg$.
2° Les lettres.

Nous entendons par là les lettres majuscules et minuscules latines, affectées d’accents. Ainsi, $A$, $A'$, $A''$, $A'''$, ..., sont des lettres. A tout endroit du texte, il est possible d’introduire des lettres autres que celles qui figureraient dans les raisonnements antérieurs.

3° Les signes spécifiques, qui dépendent de la théorie considérée.

En Théorie des Ensembles, nous n’utiliserons que les deux signes spécifiques:
$=$, $\in$.

Un assemblage de $\mathcal{T}$ est une succession de signes de $\mathcal{T}$ écrits les uns à côté des autres, certains signes distincts des lettres pouvant être joints deux à deux par des traits qui courent au-dessus de la ligne et qu’on appelle des liens. \* Ainsi, dans la théorie des ensembles, où $\in$ est une signe spécifique,

$$
\overline{\tau\ \vee\ \neg\ \in\ \square\ A'\ \in\ \square\ A''}
$$

est un assemblage. \*

L’usage exclusif des assemblages conduirait à des difficultés typographiques et mentales insurmontables. C’est pourquoi les textes courants utilisent des symboles abréviateurs (notamment des mots du langage ordinaire), qui n’appartiennent pas à la mathématique formelle. L’introduction de ces symboles est l’objet des définitions. Leur emploi n’est pas théoriquement indispensable, et prête souvent à des confusions que seule une certaine habitude permet d’éviter.

#### Exemple 1 {#ens-i-s1-n1-exa-1 .statement tag=03P0}

L’assemblage $\vee \neg$ se représente par $\Rightarrow$.

#### Exemple 2 {#ens-i-s1-n1-exa-2 .statement tag=03P1}

Les symboles suivants représentent des assemblages (d’ailleurs fort longs):

$$
\begin{array}{c}
\text{« 3 et 4 »} \\
\varnothing \\
\mathbf{N} \\
\mathbf{Z} \\
\text{« la droite numérique »} \\
\text{« la fonction } \Gamma \text{ »} \\
f \circ g \\
\pi = \sqrt{2} + \sqrt{3} \\
1 \in 2 \\
\text{« tout corps fini est commutatif »}
\end{array}
$$

« les zéros de $\zeta(s)$ autres que $-2, -4, -6, \ldots$ sont sur la droite $\Re(s) = \frac{1}{2}$. »

En général, le symbole qu’on utilise pour représenter un assemblage contient toutes les lettres qui figurent dans cet assemblage. Parfois cependant, on peut enfreindre ce principe sans grand risque de confusion. \* Par exemple « la complétion de E » représente un assemblage qui contient la lettre E, mais qui contient aussi la lettre représentant l’ensemble des entourages de la structure uniforme de E. Par contre $\int_0^1 f(x)\ dx$ représente un assemblage où ne figure pas la lettre x (ni la lettre d); les assemblages représentés par $\mathbf{N}, \mathbf{Z}, \text{« la fonction } \Gamma \text{ »}$ ne contiennent aucune lettre.*

Une théorie mathématique (ou simplement théorie) comporte des règles permettant de dire que certains assemblages de signes sont des termes ou des relations de la théorie, et d’autres règles permettant de dire que certains assemblages sont des théorèmes de la théorie.

La description de ces règles, qui va être faite dans ce chapitre, n’appartient pas à la mathématique formelle; il y intervient des assemblages plus ou moins indéterminés, par exemple des lettres indéterminées. Pour alléger l’exposé, il est commode de désigner ces assemblages par des symboles peu encombrants. Nous utiliserons notamment des combinaisons de signes (d’une théorie mathématique), de lettres italiques grasses (éventuellement affectées d’indices ou d’accents) et de symboles particuliers, dont on va donner quelques exemples. Comme on veut seulement éviter des circonlocutions (cf. note ¹ de I, p. 25), on n’énoncera pas de règles strictes et générales relatives à l’emploi de ces symboles; le lecteur pourra reconstituer sans peine, dans chaque cas particulier, l’assemblage dont il s’agit. Par abus de langage, on dira souvent que les symboles employés sont des assemblages, au lieu de dire qu’ils désignent des assemblages; des expressions telles que « l’assemblage A » ou « la lettre x », dans l’énoncé des règles qui suivent, devraient donc être remplacées par « l’assemblage désigné par A » ou « la lettre désignée par x ».

Soient $A$ et $B$ des assemblages. On désignera par $AB$ l’assemblage obtenu en écrivant l’assemblage $B$ à la droite de l’assemblage $A$. On désignera par $\vee\ A\ \neg\ B$ l’assemblage obtenu en écrivant de gauche à droite le signe $\vee$, l’assemblage $A$, le signe $\neg$, l’assemblage $B$. Etc.

Soient $A$ un assemblage, et $x$ une lettre. On désignera par $\tau_x(A)$ l’assemblage

E I.16                                             DESCRIPTION DE LA MATHÉMATIQUE FORMELLE                                             § 1

obtenu de la manière suivante: on forme l’assemblage $\tau A$, on joint par un lien chaque occurrence de $x$ dans $A$ au $\tau$ écrit à la gauche de $A$, et on remplace $x$, en chacune de ses occurrences, par un $\square$. L’assemblage désigné par $\tau_x(A)$ ne contient donc pas $x$.

#### Exemple {#ens-i-s1-n1-exa-3 .statement tag=03RY}

Le symbole $\tau_x(\in xy)$ représente l’assemblage $\tau\in\square y$.

Soient $A$ et $B$ des assemblages, et $x$ une lettre. L’assemblage obtenu en remplaçant $x$, en chacune de ses occurrences dans $A$, par l’assemblage $B$, se désigne par $(B|x)A$ (lire: $B$ remplace $x$ dans $A$). Si $x$ ne figure pas dans $A$, $(B|x)A$ est donc identique à $A$; en particulier $(B|x)\tau_x(A)$ est identique à $\tau_x(A)$.

#### Exemple {#ens-i-s1-n1-exa-4 .statement tag=03TO}

Lorsque dans l’assemblage

$$
\vee\in xy=xx
$$

on remplace $x$ par $\square$ en chacune de ses occurrences, on obtient l’assemblage

$$
\vee\in\square y=\square\square.
$$

Lorsque, étant donné un assemblage $A$, on s’intéresse particulièrement à une lettre $x$, ou à deux lettres distinctes $x$ et $y$ (qui peuvent ou non figurer dans $A$), on écrit souvent $A\{x\}$ ou $A\{x,y\}$. Dans ce cas, on écrit $A\{B\}$ au lieu de $(B|x)A$. On désigne par $A\{B,C\}$ l’assemblage obtenu en remplaçant simultanément $x$ par $B$ et $y$ par $C$ en toutes leurs occurrences dans $A$ (on notera que $x$ et $y$ peuvent figurer dans $B$ et dans $C$); si $x'$ et $y'$ sont des lettres distinctes de $x$ et de $y$ et distinctes entre elles, ne figurant ni dans $A$, ni dans $B$, ni dans $C$, $A\{B,C\}$ n’est autre que $(B|x')(C|y')(x'|x)(y'|y)A$.

#### Remarque {#ens-i-s1-n1-rem-1 .statement tag=03P2}

Quand on introduit, par une définition, un symbole abréviateur $\Sigma$ pour représenter un certain assemblage, on convient (en général de façon tacite) de représenter l’assemblage obtenu par la substitution à une lettre $x$ d’un assemblage $B$ dans l’assemblage initial, par le symbole obtenu en remplaçant la lettre $x$ dans $\Sigma$ par l’assemblage $B$ (ou plus fréquemment par un symbole abréviateur représentant l’assemblage $B$).

\* Par exemple, après avoir précisé quel assemblage représente le symbole $E\otimes F$, où $E$ et $F$ sont des lettres, — assemblage qui, d’ailleurs, contient d’autres lettres que $E$ et $F$ — on utilisera sans explications le symbole $Z\otimes F$.\*

Cette règle peut conduire à des confusions qu’on évite par des artifices typographiques variés, dont le plus fréquent consiste à remplacer $x$ par $(B)$ au lieu de $B$.

\* Par exemple, $M\cap N$ désigne un assemblage contenant la lettre $N$. Si on substitue à $N$ l’assemblage représenté par $P\cup Q$ on obtient un assemblage que l’on désigne par $M\cap(P\cup Q)$.\*

### 2. Critères de substitution

La mathématique formelle ne comporte que des assemblages expli écrits. Cependant, même avec l’usage des symboles abréviateurs, un développement de la mathématique strictement conforme à ce principe conduirait à des raisonnements extrêmement longs. Aussi allons-nous établir dans ce Livre des critères, concernant des assemblages indéterminés, et dont chacun décrira une fois pour toutes le résultat final d'une succession déterminée de manipulations sur ces assemblages. Ces critères ne sont donc pas théoriquement indispensables; leur justification appartient à la métamathématique.

Le développement de la métamathématique nécessite lui-même pratiquement l'usage de symboles abréviateurs, dont certains ont déjà été indiqués. La plupart de ces symboles seront aussi utilisés en mathématique.

On se servira des critères suivants, appelés critères de substitution:

CS1. Soient $A$ et $B$ des assemblages, $x$ et $x'$ des lettres. Si $x'$ ne figure pas dans $A$, $(B \mid x)A$ est identique à $(B \mid x')(x' \mid x)A$.

CS2. Soient $A, B$ et $C$ des assemblages, $x$ et $y$ des lettres distinctes¹. Si $y$ ne figure pas dans $B$, $(B \mid x)(C \mid y)A$ est identique à $(C' \mid y)(B \mid x)A$, où $C'$ est l'assemblage $(B \mid x)C$.

CS3. Soient $A$ un assemblage, $x$ et $x'$ des lettres. Si $x'$ ne figure pas dans $A$, $\tau_x(A)$ est identique à $\tau_{x'}(A')$, où $A'$ est l'assemblage $(x' \mid x)A$.

CS4. Soient $A$ et $B$ des assemblages, $x$ et $y$ des lettres distinctes. Si $x$ ne figure pas dans $B$, $(B \mid y)\tau_x(A)$ est identique à $\tau_x(A')$, où $A'$ est l'assemblage $(B \mid y)A$.

CS5. Soient $A, B, C$ des assemblages, $x$ une lettre. Les assemblages $(C \mid x)(\neg A)$, $(C \mid x)(\lor AB)$, $(C \mid x)(\Rightarrow AB)$, $(C \mid x)(sAB)$ (s signe spécifique) sont identiques respectivement à $\neg A'$, $\lor A'B'$, $\Rightarrow A'B'$, $sA'B'$, où $A', B'$ sont respectivement $(C \mid x)A$, $(C \mid x)B$.

Indiquons par exemple le principe de la vérification de CS2. Comparons l'opération qui fait passer de $A$ à $(B \mid x)(C \mid y)A$ à l'opération qui fait passer de $A$ à $(C' \mid y)(B \mid x)A$. Dans les deux opérations, aucun signe figurant dans $A$ et distinct de $x$ et de $y$ n'est modifié. À chaque endroit où figure $x$ dans $A$, on doit substituer $B$ à $x$ dans la première comme dans la seconde opération: c'est évident pour la première, et pour la seconde cela résulte de ce que $y$ ne figure pas dans $B$. Enfin, à chaque endroit où figure $y$ dans $A$, la première opération consiste à substituer $C$ à $y$, puis $B$ à $x$ à chaque endroit où figure $x$ dans $C$; mais il est clair que cela revient à substituer à $y$, à chaque endroit où il figure dans $A$, l'assemblage $(B \mid x)C$.

### 3. Constructions formatives

A chaque signe spécifique est associé un nombre entier, appelé son poids (pratiquement toujours le nombre 2).

Un assemblage est dit de première espèce s'il commence par un $\tau$, ou s'il se réduit à une lettre, de deuxième espèce dans les autres cas.

Une construction formative d'une théorie $\mathcal{T}$ est une suite d'assemblages qui

¹ Conformément à ce qui a été signalé (I, p. 15), la phrase « $x$ et $y$ sont des lettres distinctes » est un abus de langage pour dire que $x$ et $y$ désignent des lettres distinctes dans les assemblages que l'on considère.

possède la propriété suivante: pour chaque assemblage $A$ de la suite, l’une des conditions ci-dessous est vérifiée:
a) $A$ est une lettre.
b) Il y a, dans la suite, un assemblage de deuxième espèce $B$ précédant $A$, tel que $A$ soit $\neg B$.
c) Il y a deux assemblages de deuxième espèce $B$ et $C$ précédant $A$ (distincts ou non) tels que $A$ soit $\lor BC$.
d) Il y a un assemblage de deuxième espèce $B$ précédant $A$ et une lettre $x$ tels que $A$ soit $\tau_x(B)$.
e) Il y a un signe spécifique $s$ de poids $n$[^3] de $\mathcal{T}$, et $n$ assemblages de première espèce $A_1,A_2,\ldots,A_n$ précédant $A$, tels que $A$ soit $sA_1A_2\ldots A_n$.

On appelle termes (resp. relations) de $\mathcal{T}$ les assemblages de première espèce (resp. de deuxième espèce) figurant dans les constructions formatives de $\mathcal{T}$.

#### Exemple {#ens-i-s1-n3-exa-1 .statement}

\* Dans la théorie des ensembles, où $\in$ est un signe spécifique de poids 2, la suite des assemblages que voici est une construction formative:

$$
\begin{array}{c}
A\\
A'\\
A''\\
\in AA''\\
\in AA''\\
\neg\in AA'\\
\lor\neg\in AA'\in AA''\\
\left.
\begin{array}{c}
\neg\lor\neg\in AA'\in AA''\\
\end{array}
\right\}
\begin{array}{c}
A'\\
A''
\end{array}
\\
\tau\lor\neg\in AA'\in AA''.
\end{array}
$$

Donc l’assemblage donné en exemple au no 1 est un terme de la théorie des ensembles.\*

#### Remarque {#ens-i-s1-n3-rem-1 .statement}

Intuitivement, les termes sont des assemblages qui représentent des objets, les relations sont des assemblages qui représentent des assertions que l’on peut faire sur des objets. La condition a) signifie que les lettres représentent des objets. La condition b) signifie que, si $B$ est une assertion, $\neg B$, qu’on appelle la négation de $B$, est une assertion (qui se lit: non $B$). La condition c) signifie que, si $B$ et $C$ sont des assertions, $\lor BC$, qu’on appelle la disjonction de $B$ et $C$, est une assertion (qui se lit: $B$ ou $C$); ainsi $\Rightarrow BC$ est une assertion (qui se lit: « non $B$ ou $C$ », ou « $B$ implique $C$ », ou « $B$ entraîne $C$ »). La condition d) signifie que, si $B$ est une assertion et $x$ une lettre, $\tau_x(B)$ est un objet; considérons l’assertion $B$ comme exprimant une propriété de l’objet $x$; alors, s’il existe un objet possédant la propriété en question, $\tau_x(B)$ représente un objet privilégié qui possède cette propriété; sinon, $\tau_x(B)$ représente un objet dont on ne peut rien dire. Enfin, la condition e) signifie que, si $A_1,A_2,\ldots,A_n$ sont des objets, et $s$ un signe spécifique de poids $n$, $sA_1A_2\ldots A_n$ est une assertion relative aux objets $A_1,\ldots,A_n$.

#### Exemple {#ens-i-s1-n3-exa-2 .statement}

Les symboles $\varnothing$, $\mathbf{N}$, « la droite numérique », « la fonction $\Gamma$ », $f$, $g$, représentent des termes. Les symboles $\pi=\sqrt{2}+\sqrt{3}$, $\iota\in 2$, « tout corps fini est commutatif », « les zéros de $\zeta(s)$ autres que $-2,-4,-6,\ldots$ sont sur la droite $\mathcal{R}(s)=\frac12$ », représentent des relations. Le symbole « 3 et 4 » ne représente ni un terme, ni une relation.

N° 4                                      TERMES ET RELATIONS                                      E I.19

Le signe initial d’une relation est $\vee$, $\neg$ ou un signe spécifique; le signe initial d’un terme est $\tau$, à moins que le terme ne se réduise à une lettre. En effet, l’assertion relative aux termes résulte de ce qu’un terme est un assemblage de première espèce. Si $A$ est une relation, $A$ figure dans une construction formative, n’est pas une lettre et ne commence pas par un $\tau$; donc trois cas sont possibles: 1) $A$ est précédé d’un assemblage $B$ tel que $A$ soit $\neg B$; 2) $A$ est précédé par deux assemblages $B$ et $C$ tels que $A$ soit $\vee BC$; 3) $A$ est précédé par des assemblages $A_1,A_2,\ldots,A_n$ tels que $A$ soit $sA_1A_2\ldots A_n$, $s$ étant un signe spécifique.

### 4. Critères formatifs

**CF1.** Si $A$ et $B$ sont des relations d’une théorie $\mathcal{T}$, $\vee AB$ est une relation de $\mathcal{T}$. En effet, considérons deux constructions formatives (de $\mathcal{T}$) dont l’une contient $A$ et l’autre $B$. Considérons la suite d’assemblages obtenue en écrivant d’abord les assemblages de la première construction, puis les assemblages de la deuxième, puis $\vee AB$. Comme $A$ et $B$ sont de deuxième espèce, on vérifie aussitôt que cette suite est une construction formative de $\mathcal{T}$. L’assemblage $\vee AB$ est de deuxième espèce, donc est une relation de $\mathcal{T}$.

On établit de façon analogue les trois critères suivants:

**CF2.** Si $A$ est une relation d’une théorie $\mathcal{T}$, $\neg A$ est une relation de $\mathcal{T}$.

**CF3.** Si $A$ est une relation d’une théorie $\mathcal{T}$, et $x$ une lettre, $\tau_x(A)$ est un terme de $\mathcal{T}$.

**CF4.** Si $A_1,A_2,\ldots,A_n$ sont des termes d’une théorie $\mathcal{T}$, et $s$ un signe spécifique de poids $n$ de $\mathcal{T}$, $sA_1A_2\ldots A_n$ est une relation de $\mathcal{T}$.

Ces critères entraînent aussitôt le suivant:

**CF5.** Si $A$ et $B$ sont des relations d’une théorie $\mathcal{T}$, $\Rightarrow AB$ est une relation de $\mathcal{T}$.

**CF6.** Soit $A_1,A_2,\ldots,A_n$ une construction formative d’une théorie $\mathcal{T}$, $x$ et $y$ des lettres. Supposons que $y$ ne figure pas dans les $A_i$. Alors, $(y\mid x)A_1,(y\mid x)A_2,\ldots,(y\mid x)A_n$ est une construction formative de $\mathcal{T}$.

En effet, soit $A'_i$ l’assemblage $(y\mid x)A_i$. Si $A_i$ est une lettre, $A'_i$ est une lettre. Si $A_i$ est de la forme $\neg A_j$, où $A_j$ est un assemblage de deuxième espèce qui précède $A_i$ dans la construction, $A'_i$ est identique à $\neg A'_j$ d’après CF5, et $A'_j$ est un assemblage de deuxième espèce. On raisonne de façon analogue si $A_i$ est de la forme $\vee A_jA_k$ ou $sA_{i_1}A_{i_2}\ldots A_{i_m}$, $s$ étant un signe spécifique de $\mathcal{T}$. Si enfin $A_i$ est de la forme $\tau_z(A_j)$, où $A_j$ est un assemblage de deuxième espèce précédant $A_i$ dans la construction, plusieurs cas peuvent se présenter:

a) $z$ est une lettre distincte de $x$ et de $y$; alors $A'_i$ est identique à $\tau_z(A'_j)$ d’après CF4, et $A'_j$ est un assemblage de deuxième espèce;

b) $z$ est identique à $x$: alors $A_i$ ne contient pas $x$, donc $A'_i$ est identique à $A_i$, c’est-à-dire à $\tau_x(A_j)$; comme $y$ ne figure pas dans $A_j$, $\tau_x(A_j)$ est identique à $\tau_y(A'_j)$ d’après CF3;

c) $z$ est identique à $y$: alors $A_i$ est l’assemblage $\tau A_j$, puisque $y$ ne figure pas dans $A_j$; donc $A'_i$ est l’assemblage $\tau A'_j$, c’est-à-dire $\tau_u(A'_j)$, $u$ étant une lettre qui ne figure pas dans $A'_j$.

CF7. Soient $A$ une relation (resp. un terme) d’une théorie $\mathcal{T}$, $x$ et $y$ des lettres. Alors $(y \mid x)A$ est une relation (resp. un terme) de $\mathcal{T}$.

Soit $A_1, A_2, \ldots, A_n$ une construction formative où figure $A$. Montrons de proche en proche que, si $A_t$ est une relation (resp. un terme), $(y \mid x)A_t$, que nous désignerons par $A'_t$, est une relation (resp. un terme). Supposons ce point établi pour $A_1, A_2, \ldots, A_{i-1}$ et établissons-le pour $A_i$. Si $A_i$ est une lettre, $A'_i$ est une lettre. Si $A_i$ est précédé dans la construction par une relation $A_j$ telle que $A_i$ soit $\neg A_j$, $A'_i$ est identique à $\neg A'_j$, d’après CS5, et $\neg A'_j$ est une relation d’après CF2. On procède de façon analogue si $A_i$ est précédé par des relations $A_j, A_k$ telles que $A_i$ soit $\vee A_jA_k$, ou par des termes $A_{j_1}, \ldots, A_{j_m}$ tels que $A_i$ soit $sA_{j_1} \ldots A_{j_m}$, où $s$ est une signe spécifique de $\mathcal{T}$ de poids $m$. Si enfin $A_i$ est précédé par une relation $A_j$ telle que $A_i$ soit $\tau_x(A_j)$, plusieurs cas peuvent se présenter:

a) $z$ est distinct de $x$ et de $y$: alors $A'_i$ est identique à $\tau_z(A'_j)$ d’après CS4, et on sait déjà que $A'_j$ est une relation, donc $A'_i$ est un terme d’après CF3;

b) $z$ est identique à $x$: alors $A_i$ ne contient pas $x$, donc $A'_i$ est identique à $A_i$, et par suite est un terme;

c) $z$ est identique à $y$. Soit alors $u$ une lettre distincte de $x$ et de $y$, et qui ne figure pas dans $A_1, A_2, \ldots, A_j$; d’après CF6, la suite d’assemblages $(u \mid y)A_1, \ldots, (u \mid y)A_j$, que nous désignerons par $A''_1, \ldots, A''_j$, constitue une construction formative de $\mathcal{T}$; comme $y$ ne figure plus dans cette nouvelle construction, $(y \mid x)A''_1, \ldots, (y \mid x)A''_j$ est une construction formative en vertu de CF6, de sorte que $(y \mid x)A''_j$ est une relation de $\mathcal{T}$; par suite, $\tau_u((y \mid x)A''_j)$ est un terme de $\mathcal{T}$. Mais ce terme est identique à $(y \mid x)\tau_u(A''_j)$ d’après CS4, donc à $(y \mid x)\tau_y(A_j)$ d’après CS3, donc à $A'_i$.

CF8. Soient $A$ une relation (resp. un terme) d’une théorie $\mathcal{T}$, $x$ une lettre et $T$ un terme de $\mathcal{T}$. Alors $(T \mid x)A$ est une relation (resp. un terme) de $\mathcal{T}$.

Soit $A_1, A_2, \ldots, A_n$ une construction formative où figure $A$. Soient $x_1, x_2, \ldots, x_p$, les lettres distinctes qui figurent dans $T$. Associons à chaque lettre $x_i$ une lettre $x'_i$ distincte de $x_1, \ldots, x_p$ et des lettres figurant dans $A_1, \ldots, A_n$, de façon que les lettres $x'_1, \ldots, x'_p$ soient deux à deux distinctes. L’assemblage

$$
(x'_1 \mid x_1)(x'_2 \mid x_2) \ldots (x'_p \mid x_p)T
$$

est une terme $T'$ d’après CF7, et $(T \mid x)A$ est identique à

$$
(x_1 \mid x'_1)(x_2 \mid x'_2) \ldots (x_p \mid x'_p)(T' \mid x)A
$$

par application de CS1. Il suffit donc de montrer que $(T' \mid x)A$ est une relation (resp. un terme): autrement dit, on peut supposer désormais que les lettres qui figurent dans $T$ ne figurent pas dans $A_1, \ldots, A_n$.

Montrons alors de proche en proche que, si $A_i$ est une relation (resp. un terme), $(T | x)A_i$, que nous désignerons par $A'_i$, est une relation (resp. un terme). Supposons ce point établi pour $A_1, A_2, \ldots, A_{i-1}$ et établissons-le pour $A_i$. Si $A_i$ est une lettre, $A'_i$ est, soit cette lettre, soit $T$, donc un terme. Si $A_i$ est de la forme $\neg A_j$, $A_j$ étant une relation qui précède $A_i$ dans la construction, $A'_i$ est identique à $\neg A'_j$ d’après CS5, et on sait déjà que $A'_j$ est une relation, donc $A'_i$ est une relation d’après CF2. On procède de façon analogue si $A_i$ est de la forme $\vee A_jA_k$, ou $sA_{j_1}\ldots A_{j_m}$. Si enfin $A_i$ est de la forme $\tau_z(A_j)$, où $A_j$ est une relation qui précède $A_i$ dans la construction, plusieurs cas peuvent se présenter:

a) $z$ est distinct de $x$ et des lettres figurant dans $T$; alors $A'_i$ est identique à $\tau_z(A'_j)$ d’après CS4, et on sait déjà que $A'_j$ est une relation; donc $A'_i$ est un terme d’après CF3;

b) $z$ est identique à $x$: alors $A_i$ ne contient pas $x$, donc $A'_i$ est identique à $A_i$, et est par suite un terme;

c) $z$ figure dans $T$; alors $z$ ne figure pas dans $A_j$, de sorte que $A_i$ est identique à $\tau A_j$, donc $A'_i$ à $\tau A'_j$; or, on sait déjà que $A'_j$ est une relation, et $\tau A'_j$ est identique à $\tau_u(A'_j)$, $u$ étant une lettre qui ne figure pas dans $A'_j$; il en résulte que $A'_i$ est un terme d’après CF3.

Intuitivement, si $A$ est une relation de $\mathcal{T}$, que nous pouvons considérer comme exprimant une propriété de l’objet $x$, affirmer $(B | x)A$ revient à dire que l’objet $B$ possède cette propriété. Si $A$ est un terme de $\mathcal{T}$, il représente un objet qui dépend d’une certaine manière de l’objet désigné par $x$; le terme $(B | x)A$ représente ce que devient l’objet $A$ quand on prend pour $x$ l’objet $B$.

## EXERCICES {#ens-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).

[^1]: Le sens de cette expression se précisera progressivement au cours de ce chapitre.
[^2]: Pour la signification intuitive de ces signes, voir I, p. 18, Remarque.
[^3]: Comme il a été dit ci-dessus, on pourrait, pour développer les théories mathématiques actuelles, se borner à ne considérer que des signes spécifiques de poids 2, et par conséquent ne pas utiliser l’expression « nombre entier $n$ » dans la définition d’une construction formative.
