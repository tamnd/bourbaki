---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THÉORIE DES ENSEMBLES
section: 2
section_title: Couples
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E II.7-E II.9
pdf_pages: 0059-0061, 0101-0101
extraction: ocr
subsections:
    - "no": 1
      title: Définition des couples
      page: 7
      pdf_page: 59
    - "no": 2
      title: Produit de deux ensembles
      page: 0
      pdf_page: 60
statements: 5
exercises: 1
content_sha256: dce45c4fed9a109155a33741cf73d71851258dd23b7562a7adc8ef6a30078403
---

## § 2. COUPLES

### 1. Définition des couples

#### Proposition 1 {#ens-ii-s2-prop-1 .statement tag=03PE}

La relation $\{\{x\},\{x,y\}\}=\{\{x'\},\{x',y'\}\}$ est équivalente à « $x=x'$ et $y=y'$ ».

Il suffit de prouver que la première de ces relations entraîne la seconde. Or, si l’on avait $x\ne x'$, on en déduirait que $\{x\}\ne\{x'\}$ (II, p. 4), donc (loc. cit.) $\{x\}=\{x',y'\}$, donc $x'=x$, contrairement à l’hypothèse. On a donc nécessairement $x=x'$ et $\{x,y\}=\{x',y'\}$; mais cela entraîne $y=x$ ou $y=y'$; dans le premier cas, on a $\{x,y\}=\{x\}$, donc $y'=x$; comme $x=y$, on a $y'=y$ dans tous les cas. CQFD.

On dit que le terme $\{\{x\},\{x,y\}\}$ est le couple formé de $x$ et de $y$, et on le note de façon abrégée $(x,y)$, de sorte que la relation $(x,y)=(x',y')$ est équivalente à « $x=x'$ et $y=y'$ ».

La relation $(\exists x)(\exists y)(z=(x,y))$ se désigne par « $z$ est un couple ». Si $z$ est un couple, les relations $(\exists y)(z=(x,y))$ et $(\exists x)(z=(x,y))$ sont fonctionnelles par rapport à $x$ et $y$ respectivement, comme il résulte aussitôt de la prop. 1.

On désigne les termes $\tau_x((\exists y)(z=(x,y)))$ et $\tau_y((\exists x)(z=(x,y)))$ par $\mathrm{pr}_1z$ et $\mathrm{pr}_2z$ respectivement; on les appelle respectivement première coordonnée (ou première projection) et seconde coordonnée (ou seconde projection) de $z$. Si $z$ est un couple, la relation $(\exists y)(z=(x,y))$ est donc équivalente à $x=\mathrm{pr}_1z$ et la relation $(\exists x)(z=(x,y))$ à $y=\mathrm{pr}_2z$ (I, p. 41).

La relation $z=(x,y)$ est équivalente à « $z$ est un couple et $x=\mathrm{pr}_1z$ et $y=\mathrm{pr}_2z$ »; en effet, cette dernière relation est équivalente à
$$(\exists x')(\exists y')(\exists x'')(\exists y'')(z=(x',y')\text{ et }z=(x,y'')\text{ et }z=(x'',y));$$
d’après prop. 1, « $z=(x',y')$ et $z=(x,y'')$ et $z=(x'',y)$ » est équivalente à « $z=(x,y)$ et $x=x'$ et $x=x''$ et $y=y'$ et $y=y''$ »; « $z$ est un couple et $x=\mathrm{pr}_1z$ et $y=\mathrm{pr}_2z$ » est équivalente, d’après C33 (I, p. 35), à
$$z=(x,y)\text{ et }(\exists x')(\exists y')(\exists x'')(\exists y'')(x=x'\text{ et }x=x''\text{ et }y=y'\text{ et }y=y'')$$
ce qui établit notre assertion. On a évidemment $\mathrm{pr}_1(x,y)=x$, $\mathrm{pr}_2(x,y)=y$, et la relation $z=(\mathrm{pr}_1z,\mathrm{pr}_2z)$ est équivalente à « $z$ est un couple ».

Soient $R\{x,y\}$ une relation, les lettres $x$ et $y$ étant distinctes et figurant dans $R$. Soit $z$ une lettre distincte de $x$ et de $y$ et ne figurant pas dans $R$. Désignons par $S\{z\}$ la relation $(\exists x)(\exists y)(z=(x,y))$ et $R\{x,y\}$; c’est une relation qui contient une lettre de moins que $R$, et qui est équivalente à « $z$ est un couple et $R\{\mathrm{pr}_1z,\mathrm{pr}_2z\}$ »: cela résulte de ce que $z=(x,y)$ est équivalent à « $z$ est un couple et $x=\mathrm{pr}_1z$ et $y=\mathrm{pr}_2z$ », et des critères C33 (I, p. 35) et C47 (I,

N° 2                                                                     COUPLES                                                                     E II.8

p. 42). On en déduit aussitôt que $R\{x,y\}$ est équivalente à $S\{(x,y)\}$, et aussi à $(\exists z)(z=(x,y)$ et $S\{z\})$ d’après C47.

Cela signifie qu’on peut interpréter une relation entre les objets $x$ et $y$ comme une propriété du couple formé par ces objets.

### 2. Produit de deux ensembles

#### Théorème 1 {#ens-ii-s2-thm-1 .statement tag=03PC}

La relation

$$
(\forall X)(\forall Y)(\exists Z)(\forall z)((z\in Z)\Longleftrightarrow(\exists x)(\exists y)(z=(x,y)\ \text{et}\ x\in X\ \text{et}\ y\in Y))
$$

est vraie. Autrement dit, quels que soient $X$ et $Y$, la relation « $z$ est un couple et $\mathrm{pr}_1z\in X$ et $\mathrm{pr}_2z\in Y$ » est collectivisante en $z$.

En effet, désignons par $A_y$ l’ensemble des objets de la forme $(x,y)$ pour $x\in X$ (II, p. 5, critère C53). Soit $R$ la relation $z\in A_y$, qui est équivalente à $(\exists x)(z=(x,y)\ \text{et}\ x\in X)$. Il est clair que la relation $(\forall y)(\exists A)(\forall z)(R\Rightarrow(z\in A))$ est vraie en vertu de S5 (I, p. 33). Il résulte alors de S8 que la relation $(\exists y)(y\in Y\ \text{et}\ R)$ est collectivisante en $z$. Or, cette relation est équivalente à $(\exists x)(\exists y)(y\in Y\ \text{et}\ x\in X\ \text{et}\ z=(x,y))$ ; d’où le théorème.

#### Définition 1 {#ens-ii-s2-def-1 .statement tag=03PD}

Etant donnés deux ensembles $X$ et $Y$, l’ensemble

$$
\{z\mid(\exists x)(\exists y)(z=(x,y)\ \text{et}\ x\in X\ \text{et}\ y\in Y)\}
$$

s’appelle le produit de $X$ et de $Y$ et se désigne par $X\times Y$.

La relation $z\in X\times Y$ est donc équivalente à « $z$ est un couple et $\mathrm{pr}_1z\in X$ et $\mathrm{pr}_2z\in Y$ ». Les ensembles $X$ et $Y$ sont appelés le premier et le second ensemble facteur de $X\times Y$.

#### Proposition 2 {#ens-ii-s2-prop-2 .statement tag=03PF}

Si $A'$, $B'$ sont des ensembles non vides, la relation $A'\times B'\subset A\times B$ est équivalente à « $A'\subset A$ et $B'\subset B$ ».

En premier lieu, la relation $z\in A'\times B'$ est équivalente à « $z$ est un couple et $\mathrm{pr}_1z\in A'$ et $\mathrm{pr}_2z\in B'$ » ; donc, sans hypothèse sur $A'$ et $B'$, la relation « $A'\subset A$ et $B'\subset B$ » entraîne $A'\times B'\subset A\times B$. Réciproquement, montrons d’abord que, si $B'\neq\varnothing$ (sans hypothèse sur $A'$), la relation $A'\times B'\subset A\times B$ entraîne $A'\subset A$. Soit $x$ un élément de $A'$ ; puisque $B'\neq\varnothing$, il y a un objet $y$ qui est élément de $B'$ ; on a $(x,y)\in A'\times B'$, d’où $(x,y)\in A\times B$ et par suite $x\in A$ ; cela montre que $A'\subset A$. On voit de même que si $A'\neq\varnothing$, la relation $A'\times B'\subset A\times B$ entraîne $B'\subset B$, d’où la proposition.

#### Proposition 3 {#ens-ii-s2-prop-3 .statement}

Soient $A$ et $B$ deux ensembles. La relation $A\times B=\varnothing$ est équivalente à « $A=\varnothing$ ou $B=\varnothing$ ».

En effet, la relation $z\in A\times B$ entraîne $\mathrm{pr}_1z\in A$ et $\mathrm{pr}_2z\in B$, donc $A\neq\varnothing$ et $B\neq\varnothing$ ; inversement, la relation « $x\in A$ et $y\in B$ » entraîne $(x,y)\in A\times B$,

THÉORIE DES ENSEMBLES

§ 3

donc $A \times B \neq \varnothing$. Autrement dit, la relation $A \times B \neq \varnothing$ est équivalente à «$A \neq \varnothing$ et $B \neq \varnothing$»; d'où la proposition.

Si $A$, $B$, $C$ sont des ensembles, on pose

$$(A \times B) \times C = A \times B \times C;$$

un élément $((x,y),z)$ de $A \times B \times C$ s’écrit aussi $(x,y,z)$ et s’appelle un triplet. De même, si $A$, $B$, $C$, $D$ sont des ensembles, on pose $(A \times B \times C) \times D =$
$A \times B \times C \times D$. Etc.

## EXERCICES {#ens-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
