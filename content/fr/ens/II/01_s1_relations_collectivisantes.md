---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THÉORIE DES ENSEMBLES
section: 1
section_title: Relations collectivisantes
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0053-0059, 0101-0101
extraction: ocr
subsections:
    - "no": 1
      title: La théorie des ensembles
      page: 0
      pdf_page: 53
    - "no": 2
      title: L’inclusion
      page: 0
      pdf_page: 54
    - "no": 3
      title: L’axiome d’extensionalité
      page: 0
      pdf_page: 55
    - "no": 4
      title: Relations collectivisantes
      page: 0
      pdf_page: 55
    - "no": 5
      title: L’axiome de l’ensemble à deux éléments
      page: 0
      pdf_page: 56
    - "no": 6
      title: Le schéma de sélection et réunion
      page: 0
      pdf_page: 56
    - "no": 7
      title: Complémentaire d’un ensemble. L’ensemble vide
      page: 0
      pdf_page: 58
statements: 8
exercises: 6
content_sha256: 8db79cf99e7fe9205dc6a9acc5d237684c289089d9d58e2cfcb3454ac791038f
---

## § 1. RELATIONS COLLECTIVISANTES

### 1. La théorie des ensembles

La théorie des ensembles est une théorie dans laquelle figurent les signes spécifiques $=$, $\in$, de poids 2; elle comporte, outre les schémas S1 à S7, donnés au chap. I, le schéma S8 qui sera introduit au no 6 (II, p. 4), et les axiomes explicites A1 (II, p. 2), A2 (II, p. 4), A3 (II, p. 30), et A4 (III, p. 45). Ces axiomes explicites ne contiennent pas de lettres; autrement dit, la théorie des ensembles est une théorie sans constantes.

Puisque la théorie des ensembles est un théorie égalitaire, les résultats du chap. I lui sont applicables.

Désormais, et sauf mention expresse du contraire, nous raisonnerons toujours dans une théorie plus forte (I, p. 24) que la théorie des ensembles; quand la théorie n’est pas mentionnée explicitement, c’est de la théorie des ensembles qu’il s’agit. Il sera évident dans bien des cas qu’une telle hypothèse n’est pas nécessaire, et le lecteur déterminera sans peine dans quelle théorie moins forte que la théorie des ensembles les résultats énoncés sont valables.

Si $T$ et $U$ sont des termes, l’assemblage $\in TU$ est une relation (dite relation d’appartenance) que nous noterons pratiquement de l’une quelconque des manières suivantes: $T\in U$, $(T)\in(U)$, « $T$ appartient à $U$ », « $T$ est élément de $U$ ». La relation « non $(T\in U)$ » se note $T\notin U$.

Du point de vue « naïf », beaucoup d’êtres mathématiques peuvent être considérés comme des collections ou « ensembles » d’objets. Nous ne chercherons pas à formaliser cette notion, et dans l’interprétation formaliste de ce qui suit, le mot « ensemble » doit être considéré comme strictement synonyme de « terme »; en particulier, des phrases telles que « soit $X$ un ensemble » sont, en principe, totalement superflues, puisque toute lettre est un terme; de telles phrases ne sont introduites que pour faciliter l’interprétation intuitive du texte.

N° 2
RELATIONS COLLECTIVISANTES
E II.2

### 2. L’inclusion

#### Définition 1 {#ens-ii-s1-def-1 .statement tag=03H5}

La relation désignée par $(\forall z)((z\in x)\Rightarrow(z\in y))$ dans laquelle ne figurent que les lettres $x$ et $y$, se note de l’une quelconque des manières suivantes : $x\subset y$, $y\supset x$, « $x$ est contenu dans $y$ », « $y$ contient $x$ », « $x$ est une partie de $y$ », « $x$ est un sous-ensemble de $y$ ». La relation non$(x\subset y)$ se note $x\not\subset y$ ou $y\not\supset x$.

Conformément aux usages signalés dans I, p. 16, cette définition entraîne la convention métamathématique suivante : soient $T$ et $U$ des assemblages ; si, dans l’assemblage $x\subset y$, on substitue simultanément $T$ à $x$ et $U$ à $y$, on obtient un assemblage qui sera désigné par $T\subset U$ ; si on désigne par $x$, $y$ des lettres quelconques distinctes de $x$ et de $y$, distinctes entre elles, et ne figurant ni dans $T$, ni dans $U$, l’assemblage $T\subset U$ est donc identique à $(T\mid x)(U\mid y)(x\mid x)(y\mid y)(x\subset y)$, donc, d’après CS8, CS9 (I, p. 32) et CS5 (I, p. 17), à $(\forall z)((z\in T)\Rightarrow(z\in U))$, à condition que $z$ soit une lettre ne figurant ni dans $T$, ni dans $U$.

Désormais, quand on posera une définition mathématique, on ne signalera plus la convention métamathématique qui en résulte.

CS12. Soient $T$, $U$, $V$ des assemblages, et $x$ une lettre. L’assemblage $(V\mid x)(T\subset U)$ est identique à $(V\mid x)T\subset(V\mid x)U$.

Ceci résulte aussitôt de CS9 (I, p. 32) et CS5 (I, p. 17).

CF13. Si $T$ et $U$ sont des termes, $T\subset U$ est une relation.

Ceci résulte aussitôt de CF8 (I, p. 20).

Toute relation de la forme $T\subset U$ (où $T$ et $U$ sont des termes) est dite relation d’inclusion.

Désormais, nous n’expli plus les critères de substitution et les critères formatifs qui devraient suivre les définitions. On notera cependant que ces critères seront souvent utilisés impli dans les démonstrations.

Pour démontrer dans une théorie $\mathcal{T}$ la relation $x\subset y$, il suffit, d’après C27 (I, p. 32), de démontrer $z\in y$ dans la théorie obtenue en adjoignant $z\in x$ aux axiomes de $\mathcal{T}$, $z$ étant une lettre distincte de $x$, de $y$ et des constantes de la théorie. En pratique on dit : « soit $z$ un élément de $x$ » ; et on cherche à démontrer $z\in y$.

#### Proposition 1 {#ens-ii-s1-prop-1 .statement tag=03P9}

$x\subset x$.

Cette proposition est immédiate.

On dit que $x$ est la partie pleine de $x$.

#### Proposition 2 {#ens-ii-s1-prop-2 .statement tag=03PA}

$(x\subset y\ \text{et}\ y\subset z)\Rightarrow(x\subset z)$.

Adjoignons les hypothèses $x\subset y$, $y\subset z$ et $u\in x$. Alors les relations

$$(u\in x)\Rightarrow(u\in y),\qquad (u\in y)\Rightarrow(u\in z)$$

sont vraies, donc la relation $u\in z$ est vraie.

E II.3                                      THÉORIE DES ENSEMBLES                                      § 1

### 3. L’axiome d’extensionalité

On appelle *axiome d’extensionalité* l’axiome suivant:

A1.

$$
(\forall x)(\forall y)((x \subset y\ \text{et}\ y \subset x)\Rightarrow(x=y)).
$$

Intuitivement, cet axiome exprime que deux ensembles ayant les mêmes éléments sont égaux.

Pour démontrer $x=y$, il suffit donc de démontrer $z\in y$ dans la théorie obtenue en adjoignant l’hypothèse $z\in x$, et $z\in x$ dans la théorie obtenue en adjoignant l’hypothèse $z\in y$, $z$ étant une lettre distincte de $x$, de $y$ et des constantes.

C48. Soient $R$ une relation, $x$ une lettre, $y$ une lettre distincte de $x$ et ne figurant pas dans $R$. La relation $(\forall x)((x\in y)\Leftrightarrow R)$ est unique en $y$.

En effet, soit $z$ une lettre distincte de $x$ et ne figurant pas dans $R$. Adjoignons les hypothèses $(\forall x)((x\in y)\Leftrightarrow R)$ et $(\forall x)((x\in z)\Leftrightarrow R)$. Alors, on a successivement les théorèmes

$$
(\forall x)(((x\in y)\Leftrightarrow R)\ \text{et}\ ((x\in z)\Leftrightarrow R)),
$$

$$
(\forall x)((x\in y)\Leftrightarrow(x\in z)),
$$

$y\subset z,\ z\subset y$.

D’après A1, on a $y=z$. Ceci établit C48.

### 4. Relations collectivisantes

Soient $R$ une relation, $x$ une lettre. Si $y$ et $y'$ désignent des lettres distinctes de $x$ et ne figurant pas dans $R$, les relations $(\exists y)(\forall x)((x\in y)\Leftrightarrow R)$ et $(\exists y')(\forall x)((x\in y')\Leftrightarrow R)$ sont identiques d’après C8 (I, p. 32). La relation ainsi définie (qui ne contient pas $x$) se désigne par Coll$_xR$.

Lorsque Coll$_xR$ est un théorème d’une théorie $\mathcal{T}$, on dit que $R$ est collectivisante en $x$ dans $\mathcal{T}$. S’il en est ainsi, on peut introduire une constante auxiliaire $a$, distincte de $x$, des constantes de $\mathcal{T}$, et ne figurant pas dans $R$, avec l’axiome introducteur $(\forall x)((x\in a)\Leftrightarrow R)$, ou, ce qui revient au même si $x$ n’est pas une constante de $\mathcal{T}$, $(x\in a)\Leftrightarrow R$.

Intuitivement, dire que $R$ est collectivisante en $x$, c’est dire qu’il existe un ensemble $a$ tel que les objets $x$ possédant la propriété $R$ soient précisément les éléments de $a$.

**Exemples**

1) La relation $x\in y$ est évidemment collectivisante en $x$.

2) La relation $x\notin x$ n’est pas collectivisante en $x$; autrement dit, $(\text{non Coll}_x(x\notin x))$ est un théorème. Raisonnons par l’absurde en supposant $x\notin x$ collectivisante. Soit $a$ une constante auxiliaire, distincte de $x$ et des constantes de la théorie, avec l’axiome introducteur $(\forall x)((x\notin x)\Leftrightarrow(x\in a))$. Alors, la relation $(a\notin a)\Leftrightarrow(a\in a)$ est vraie d’après C30 (I, p. 34). La méthode de disjonction de cas (I, p. 28) prouve d’abord que la relation $a\notin a$ est vraie, puis que la relation $a\in a$ est vraie, ce qui est absurde.

C49. Soient $R$ une relation et $x$ une lettre. Si $R$ est collectivisante en $x$, la relation

N° 6                                             RELATIONS COLLECTIVISANTES                                             E II.4

$(\forall x)((x\in y)\Leftrightarrow R)$, où $y$ est une lettre distincte de $x$ et ne figurant pas dans $R$, est fonctionnelle en $y$.

Ceci résulte aussitôt de C48.

Très fréquemment, dans la suite, on disposera d’un théorème de la forme $\mathrm{Coll}_xR$. On introduira alors, pour représenter le terme $\tau_y(\forall x)((x\in y)\Leftrightarrow R)$, qui ne dépend pas du choix de la lettre $y$ (distincte de $x$ et ne figurant pas dans $R$) un symbole fonctionnel; dans ce qui suit, nous utiliserons le symbole $\{x\mid R\}$; le terme correspondant ne contient pas $x$. C’est de ce terme qu’il s’agira quand on parlera de «l’ensemble des $x$ tels que $R$». Par définition (I, p. 32) la relation $(\forall x)((x\in\{x\mid R\})\Leftrightarrow R)$ est identique à $\mathrm{Coll}_xR$; par suite la relation $R$ est équivalente à $x\in\{x\mid R\}$.

**C50.** Soient $R$, $S$ deux relations et $x$ une lettre. Si $R$ et $S$ sont collectivisantes en $x$, la relation $(\forall x)(R\Rightarrow S)$ est équivalente à $\{x\mid R\}\subset\{x\mid S\}$; la relation $(\forall x)(R\Leftrightarrow S)$ est équivalente à $\{x\mid R\}=\{x\mid S\}$.

Cela résulte aussitôt de la remarque qui précède, de la déf. 1 et de l’axiome A1.

### 5. L’axiome de l’ensemble à deux éléments

A2.

$$(\forall x)(\forall y)\mathrm{Coll}_z(z=x\ \mathrm{ou}\ z=y).$$

Cet axiome exprime que, si $x$ et $y$ sont des objets, il existe un ensemble dont les seuls éléments sont $x$ et $y$.

#### Définition 2 {#ens-ii-s1-def-2 .statement tag=03H6}

L’ensemble $\{z\mid z=x\ \mathrm{ou}\ z=y\}$, dont les seuls éléments sont $x$ et $y$, se note $\{x,y\}$.

La relation $z\in\{x,y\}$ est donc équivalente à «$z=x$ ou $z=y$»; il résulte de C50 que l’on a $\{y,x\}=\{x,y\}$.

Soit $R\! \not\ni z$ une relation, $x$ et $y$ des lettres distinctes de $z$. Des critères C32, C33 (I, p. 35) et C43 (I, p. 39) il résulte aisément que la relation $(\exists z)((z\in\{x,y\})\ \mathrm{et}\ R\! \not\ni z)$ est équivalente à $R\! \not\ni x$ ou $R\! \not\ni y$; on en déduit que la relation $(\forall z)((z\in\{x,y\})\Rightarrow R\! \not\ni z)$ est équivalente à $R\! \not\ni x$ et $R\! \not\ni y$.

L’ensemble $\{x,x\}$, qu’on désigne simplement par $\{x\}$, s’appelle l’ensemble dont le seul élément est $x$ (ou l’ensemble réduit au seul élément $x$); la relation $z\in\{x\}$ est équivalente à $z=x$; la relation $x\in X$ est équivalente à $\{x\}\subset X$.

### 6. Le schéma de sélection et réunion

On appelle schéma de sélection et réunion le schéma suivant:

S8. Soient $R$ une relation, $x$ et $y$ des lettres distinctes, $X$ et $Y$ des lettres distinctes de $x$ et $y$ et ne figurant pas dans $R$. La relation

(1)

$$(\forall y)(\exists X)(\forall x)(R\Rightarrow(x\in X))\Rightarrow(\forall Y)\mathrm{Coll}_x((\exists y)((y\in Y)\ \mathrm{et}\ R))$$

est un axiome.

THÉORIE DES ENSEMBLES

§ 1

Montrons d’abord que cette règle est bien un schéma. En effet, désignons par $S$ la relation (1), et, dans $S$, substituons un terme $T$ à une lettre $z$; d’après CS8 (I, p. 32), on peut supposer $x,y,X,Y$ distincts de $z$ et ne figurant pas dans $T$. Alors $(T|z)S$ est identique à

$$
(\forall y)(\exists X)(\forall x)(R' \Rightarrow (x\in X)) \Rightarrow (\forall Y)\operatorname{Coll}_x((\exists y)((y\in Y)\text{ et }R'))
$$

où $R'$ est $(T|z)R$.

Intuitivement, la relation $(\forall y)(\exists X)(\forall x)(R\Rightarrow (x\in X))$ signifie que, pour tout objet $y$, il existe un ensemble $X$ (qui peut dépendre de $y$), tel que les objets $x$ qui sont dans la relation $R$ avec l’objet $y$ donné soient des éléments de $X$ (sans constituer nécessairement tout l’ensemble $X$). Le schéma de sélection et réunion affirme que, s’il en est ainsi, et si $Y$ est un ensemble quelconque, il existe un ensemble dont les éléments sont exactement tous les objets $x$ se trouvant dans la relation $R$ avec un objet $y$ au moins de l’ensemble $Y$.

C51. Soient $P$ une relation, $A$ un ensemble et $x$ une lettre ne figurant pas dans $A$. La relation « $P$ et $x\in A$ » est collectivisante en $x$.

Désignons par $R$ la relation « $P$ et $x=y$ », où $y$ est une lettre distincte de $x$ et ne figurant ni dans $P$ ni dans $A$. La relation $(\forall x)(R\Rightarrow (x\in\{y\}))$ est vraie d’après C27 (I, p. 32). Soit $X$ une lettre distincte de $x$ et de $y$ et ne figurant pas dans $P$. La relation précédente est identique à $\{y\}|X)((\forall x)(R\Rightarrow (x\in X)))$ (notamment parce que $x$ est distincte de $y$), donc la relation $(\forall y)(\exists X)(\forall x)(R\Rightarrow (x\in X))$ est vraie en vertu de S5 et de C27 (I, p. 33 et p. 32). Il résulte de S8 et de C30 (I, p. 34) que la relation $(A|Y)\operatorname{Coll}_x(\exists y)(y\in Y\text{ et }R)$ (où $Y$ est une lettre ne figurant pas dans $R$) est vraie, et cette relation est identique à $\operatorname{Coll}_x(\exists y)(y\in A\text{ et }R)$ (notamment parce que ni $x$, ni $y$ ne figurent dans $A$). Enfin, la relation « $y\in A$ et $R$ » est équivalente à « $x=y$ et $x\in A$ et $P$ » d’après C43 (I, p. 39); comme $y$ ne figure ni dans $P$ ni dans $A$, la relation $(\exists y)(x=y\text{ et }x\in A\text{ et }P)$ est équivalente à « $(\exists y)(x=y)$ et $x\in A$ et $P$ » d’après C33 (I, p. 35) donc à « $P$ et $x\in A$ » puisque $(\exists y)(x=y)$ est vraie.

L’ensemble $\{x\mid P\text{ et }x\in A\}$ est appelé l’ensemble des $x\in A$ tels que $P$ et se note parfois $\{x\in A\mid P\}$ *(c’est ainsi qu’on parlera de l’ensemble des nombres réels tels que $P$)*.

C52. Soient $R$ une relation, $A$ un ensemble, $x$ une lettre ne figurant pas dans $A$. Si la relation $R\Rightarrow (x\in A)$ est un théorème, $R$ est collectivisante en $x$.

En effet, $R$ est alors équivalente à « $R$ et $x\in A$ ».

#### Remarque {#ens-ii-s1-n6-rem-1 .statement tag=03H7}

Soient $R$ une relation collectivisante en $x$, et $S$ une relation telle que $(\forall x)(S\Rightarrow R)$ soit un théorème. Alors $S$ est collectivisante en $x$, car $R$ est équivalente à $x\in\{x\mid R\}$, donc $S\Rightarrow (x\in\{x\mid R\})$ est un théorème et il suffit d’appliquer C52. On notera en outre que, dans ce cas, on a $\{x\mid S\}\subset\{x\mid R\}$ d’après C50.

C53. Soient $T$ un terme, $A$ un ensemble, $x$ et $y$ des lettres distinctes. On suppose que $x$

Nº 7                                                                             RELATIONS COLLECTIVISANTES                                                                             E II.6

ne figure pas dans A, et que y ne figure ni dans T ni dans A. La relation
$$
(\exists x)(y=T\text{ et }x\in A)
$$
est collectivisante en y.

Soit R la relation $y=T$. La relation $(\forall y)(R\Rightarrow (y\in\{T\}))$ est vraie, donc il en est de même de $(\forall x)(\exists X)(\forall y)(R\Rightarrow (y\in X))$, où X est une lettre distincte de y et ne figurant pas dans R. En vertu de S8, la relation $(\exists x)(x\in A\text{ et }R)$ est collectivisante en y, ce qui démontre C53.

La relation $(\exists x)(y=T\text{ et }x\in A)$ se lit souvent : « y peut se mettre sous la forme T pour un x appartenant à A ». L’ensemble $\{y\mid(\exists x)(y=T\text{ et }x\in A)\}$ est généralement appelé l’ensemble des objets de la forme T pour x∈A. L’assemblage ainsi désigné ne contient ni x ni y, et ne dépend pas du choix de la lettre y vérifiant les conditions de C53.

### 7. Complémentaire d’un ensemble. L’ensemble vide

La relation $(x\notin A\text{ et }x\in X)$ est collectivisante en x d’après C51.

#### Définition 3 {#ens-ii-s1-def-3 .statement tag=03H8}

Soit A une partie d’un ensemble X. On appelle complémentaire de A par rapport à X, et on désigne par $\complement_XA$ ou $X-A$ (ou par $\complement A$ lorsqu’il n’y a pas de confusion à craindre) l’ensemble des éléments de X qui n’appartiennent pas à A, c’est-à-dire l’ensemble $\{x\mid x\notin A\text{ et }x\in X\}$.

Soit A une partie d’un ensemble X ; les relations « $x\in X$ et $x\notin A$ » et $x\in\complement_XA$ sont donc équivalentes. Par suite, la relation « $x\in X$ et $x\notin\complement_XA$ » est équivalente à « $x\in X$ et $(x\notin X\text{ ou }x\in A)$ », donc à $x\in A$. Autrement dit, $A=\complement_X(\complement_XA)$ est une relation vraie. On voit de même que, si B est une partie de X, les relations $A\subset B$ et $\complement_XB\subset\complement_XA$ sont équivalentes.

#### Théorème 1 {#ens-ii-s1-thm-1 .statement tag=03H9}

La relation $(\forall x)(x\notin X)$ est fonctionnelle en X.

En effet, la relation $(\forall x)(x\notin X)$ entraîne $(\forall Y)(X\subset Y)$ ; en vertu de l’axiome d’extensionalité, la relation $(\forall x)(x\notin X)$ est donc univoque en X. D’autre part, la relation $(\forall x)(x\notin\complement_XY)$ est vraie, ce qui prouve que $(\exists X)(\forall x)(x\notin X)$ est vraie.

Le terme $\tau_X((\forall x)(x\notin X))$ correspondant à cette relation fonctionnelle se représente par le symbole fonctionnel $\varnothing$, qu’on appelle l’ensemble vide[^1] ; la relation $(\forall x)(x\notin X)$, qui est équivalente à $X=\varnothing$, se lit : « l’ensemble X est vide ». On a les théorèmes $x\notin\varnothing$, $\varnothing\subset X$, $\complement_XX=\varnothing$, $\complement_X\varnothing=X$ ; la relation $X\subset\varnothing$ est équivalente à $X=\varnothing$. Si $R\{x\}$ est une relation, la relation $(\forall x)((x\in\varnothing)\Rightarrow R\{x\})$ est vraie.

#### Remarque {#ens-ii-s1-n7-rem-1 .statement tag=03PB}

Il n’existe pas d’ensemble dont tous les objets soient éléments ; autrement dit, « non $(\exists X)(\forall x)(x\in X)$ » est un théorème. En effet, s’il existait un tel ensemble, toute relation serait collectivisante d’après C52. Or, nous avons vu (II, p. 3) que la relation $x \ne x'$ n’est pas collectivisante.

## EXERCICES {#ens-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).

[^1]: Le terme désigné par $\varnothing$ est donc ⟪illegible⟫.
