---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION DE LA MATHÉMATIQUE FORMELLE
section: 5
section_title: Théories égalitaires
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E I.49
pdf_pages: 0039-0043, 0050-0050
extraction: ocr
subsections:
    - "no": 1
      title: Les axiomes
      page: 0
      pdf_page: 39
    - "no": 2
      title: Propriétés de l’égalité
      page: 39
      pdf_page: 40
    - "no": 3
      title: Relations fonctionnelles
      page: 40
      pdf_page: 41
statements: 3
exercises: 7
content_sha256: f56d99d868f32a4b67ae8e64b9fe1d26da9c4ad08fc39e6dfdbf1ae94b6db6f8
---

## § 5. THÉORIES ÉGALITAIRES

### 1. Les axiomes

On appelle théorie égalitaire une théorie $\mathcal{T}$ dans laquelle figure un signe relationnel de poids 2 noté = (qui se lit « égal »), et dans laquelle les schémas S1 à S5 (I, p. 25 et p. 33) ainsi que les schémas S6 et S7 ci-dessous fournissent des axiomes impli; si $T$ et $U$ sont des termes de $\mathcal{T}$, l’assemblage $=TU$ est une relation de $\mathcal{T}$ (dite relation d’égalité) d’après CF4; on la désigne pratiquement par $T = U$ ou $(T) = (U)$.

S6. Soient $x$ une lettre, $T$ et $U$ des termes de $\mathcal{T}$, et $R\{x\}$ une relation de $\mathcal{T}$; la relation
$$
(T = U) \Rightarrow (R\{T\} \Leftrightarrow R\{U\})
$$
est un axiome.

S7. Si $R$ et $S$ sont des relations de $\mathcal{T}$ et $x$ une lettre, la relation
$$
(\forall x)(R \Leftrightarrow S) \Rightarrow (\tau_x(R) = \tau_x(S))
$$
est un axiome.

La règle S6 est bien un schéma. Soit en effet $A$ un axiome de $\mathcal{T}$, obtenu par application de S6: il y a une relation $R$ de $\mathcal{T}$, des termes $T$ et $U$ de $\mathcal{T}$, et une lettre $x$, tels que $A$ soit $(T = U) \Rightarrow ((T|x)R \Leftrightarrow (U|x)R)$. On va voir que, si $y$ est une lettre et $V$ un terme de $\mathcal{T}$, la relation $(V|y)A$ s’obtient encore par application de S6. Par utilisation de CS1 (I, p. 17), on peut se ramener au cas où $x$ est distinct de $y$ et ne figure pas dans $V$. Désignons par $T'$, $U'$, $R'$ les assemblages $(V|y)T$, $(V|y)U$, $(V|y)R$. D’après CS2 et CS5 (I, p. 17), $(V|y)A$ est identique à
$$
(T' = U') \Rightarrow ((T'|x)R' \Leftrightarrow (U'|x)R'),
$$
ce qui établit notre assertion. On vérifie de façon analogue que S7 est un schéma.

Intuitivement, le schéma S6 signifie que, si deux objets sont égaux, ils ont les mêmes propriétés. Le schéma S7 est plus éloigné de l’intuition courante; il signifie que, lorsque deux propriétés $R$ et $S$ d’un objet $x$ sont équivalentes, alors les objets privilégiés $\tau_x(R)$ et $\tau_x(S)$ (choisis respectivement parmi ceux qui vérifient $R$, et parmi ceux qui vérifient $S$, s’il y a de tels objets) sont égaux. Le lecteur notera que la présence dans S7 du quantificateur $\forall x$ est essentielle (cf. exerc. 7).

La négation de la relation $=$ ou se désigne par $T \ne U$, ou $(T) \ne (U)$ (où le signe $\ne$ se lit « différent de »).

On déduit de S6 le critère suivant :

**C43.** Soient $x$ une lettre, $T$ et $U$ des termes de $\mathcal{T}$, et $R\{x\}$ une relation de $\mathcal{T}$ ; les relations $(T = U$ et $R\{T\})$ et $(T = U$ et $R\{U\})$ sont équivalentes.

En effet, si on adjoint les hypothèses $T = U$ et $R\{T\}$, $R\{U\}$ est vraie d’après S6, donc $(T = U$ et $R\{U\})$ est vraie.

Par abus de langage, lorsqu’on a démontré une relation de la forme $T = U$ dans une théorie $\mathcal{T}$, on dit souvent que les termes $T$ et $U$ sont « les mêmes » ou sont « identiques ». De même, lorsque $T \ne U$ est vraie dans $\mathcal{T}$, on dit que $T$ et $U$ sont « distincts » au lieu de dire que $T$ est différent de $U$.

### 2. Propriétés de l’égalité

Nous ne considérerons plus désormais que des théories égalitaires. Soit $\mathcal{T}$ une telle théorie. Soit $\mathcal{T}_0$ la théorie dont les signes sont ceux de $\mathcal{T}$, et dont les axiomes sont fournis par les seuls schémas S1 à S7. La théorie $\mathcal{T}_0$ est moins forte que $\mathcal{T}$ (I, p. 24) et ne possède pas de constantes. Les trois théorèmes qui suivent sont des théorèmes de $\mathcal{T}_0$.

#### Théorème 1 {#ens-i-s5-thm-1 .statement tag=03P3}

$x = x$.

Désignons par $S$ la relation $x = x$ de $\mathcal{T}_0$. D’après C27 (I, p. 32), pour toute relation $R$ de $\mathcal{T}_0$, $(\forall x)(R \iff R)$ est un théorème de $\mathcal{T}_0$, donc, d’après S7, $\tau_x(R) = \tau_x(R)$, c’est-à-dire $(\tau_x(R) \mid x)S$, est un théorème de $\mathcal{T}_0$. En prenant pour $R$ la relation « non $S$ », et tenant compte de C26 (I, p. 32), on voit que $(\forall x)S$ est un théorème de $\mathcal{T}_0$. D’après C30 (I, p. 34), $S$ est donc un théorème de $\mathcal{T}_0$.

La relation $(\forall x)(x = x)$ est aussi un théorème de $\mathcal{T}_0$ ; et si $T$ est une terme de $\mathcal{T}_0$, $T = T$ est un théorème de $\mathcal{T}_0$ (cf. I, p. 34). Il est possible de transformer de la même façon les théorèmes ultérieurs en des théorèmes où ne figure aucune lettre, ou en des critères métamathématiques. Nous ne ferons plus désormais ces transformations mais nous les utiliserons souvent impli.

#### Théorème 2 {#ens-i-s5-thm-2 .statement tag=03P4}

$(x = y) \iff (y = x)$.

Supposons que la relation $x = y$ soit vraie. D’après S6, la relation

$$
(x = y) \Rightarrow ((x \mid y)(y = x) \iff (y \mid y)(y = x)),
$$

c’est-à-dire $(x = y) \Rightarrow ((x = x) \iff (y = x))$ est vraie. Donc $(x = x) \iff (y = x)$ est vraie. En vertu du théorème 1, $y = x$ est vraie, ce qui établit le théorème.

#### Théorème 3 {#ens-i-s5-thm-3 .statement tag=03P5}

$((x = y) \text{ et } (y = z)) \Rightarrow (x = z)$.

Adjignons les hypothèses $x = y$, $y = z$ aux axiomes de $\mathcal{T}_0$. D’après §6, la relation $(x = y) \Rightarrow ((x = z) \Leftrightarrow (y = z))$ est vraie. Donc $(x = z) \Leftrightarrow (y = z)$, et par suite $x = z$, sont vraies, ce qui établit le théorème.

C44. Soient $x$ une lettre, $T$, $U$, $V\{x\}$ des termes de $\mathcal{T}_0$. La relation

$$(T = U) \Rightarrow (V\{T\} = V\{U\})$$

est un théorème de $\mathcal{T}_0$.

En effet, soient $y$ et $z$ deux lettres distinctes entre elles, distinctes de $x$ et des lettres qui figurent dans $T$, $U$, $V$. Adjoignons l’hypothèse $y = z$. Alors, d’après §6,

$$((y \mid z)(V\{y\} = V\{z\})) \Leftrightarrow (V\{y\} = V\{z\})$$

c’est-à-dire $(V\{y\} = V\{y\}) \Leftrightarrow (V\{y\} = V\{z\})$ est vraie. Or, $V\{y\} = V\{y\}$ est vraie d’après le th. 1. Donc $V\{y\} = V\{z\}$ est vraie. De tout ceci résulte que $(y = z) \Rightarrow (V\{y\} = V\{z\})$ est un théorème de $\mathcal{T}_0$, soit $A$. Or, $(T \mid y)(U \mid z)A$ n’est autre que $(T = U) \Rightarrow (V\{T\} = V\{U\})$.

On dit qu’une relation de la forme $T = U$, où $T$ et $U$ sont des termes de $\mathcal{T}$, est une équation; une solution (dans $\mathcal{T}$) de la relation $T = U$, considérée comme équation en une lettre $x$, est donc (I, p. 22) un terme $V$ de $\mathcal{T}$ tel que $T\{V\} = U\{V\}$ soit un théorème de $\mathcal{T}$.

Soient $T$ et $U$ deux termes de $\mathcal{T}$, $x_1, x_2, \ldots, x_n$ les lettres figurant dans $T$ et non dans $U$. Si la relation $(\exists x_1)\ldots(\exists x_n)(T = U)$ est un théorème de $\mathcal{T}$, on dit que $U$ se met sous la forme $T$ (dans $\mathcal{T}$). Soient $R$ une relation de $\mathcal{T}$, $y$ une lettre. Soit $V$ une solution (dans $\mathcal{T}$) de $R$, considérée comme relation en $y$. Si toute solution (dans $\mathcal{T}$) de $R$, considérée comme relation en $y$, peut se mettre sous la forme $V$, on dit que $V$ est solution complète (ou solution générale) de $R$ (dans $\mathcal{T}$).

### 3. Relations fonctionnelles

Soient $R$ un assemblage, $x$ une lettre. Soient $y$, $z$ des lettres distinctes entre elles, distinctes de $x$ et ne figurant pas dans $R$. Soient $y'$, $z'$ deux autres lettres ayant les mêmes propriétés. En vertu de CS8, CS9 (I, p. 32), CS2, CS5 (I, p. 17), CS6 (I, p. 29), les assemblages

$$(\forall y)(\forall z)(((y \mid x)R \text{ et } (z \mid x)R) \Rightarrow (y = z))$$

et

$$(\forall y')(\forall z')(((y' \mid x)R \text{ et } (z' \mid x)R) \Rightarrow (y' = z'))$$

sont identiques. Si $R$ est une relation de $\mathcal{T}$, l’assemblage ainsi défini est une relation de $\mathcal{T}$ qui se désigne par «il existe au plus un $x$ tel que $R$»; la lettre $x$ n’y figure pas. Lorsque cette relation est un théorème de $\mathcal{T}$, on dit que $R$ est univoque en $x$ dans $\mathcal{T}$. Pour prouver que $R$ est univoque en $x$ dans $\mathcal{T}$, il suffit de prouver $y = z$ dans la théorie déduite de $\mathcal{T}$ par adjonction des axiomes $(y \mid x)R$ et $(z \mid x)R$,

N° 3                                                                     THÉORIES ÉGALITAIRES                                                                     E I.41

$y$ et $z$ étant des lettres distinctes entre elles, distinctes de $x$, ne figurant ni dans $R$, ni dans les axiomes expli de $\mathcal{T}$.

**C45.** — Soient $R$ une relation de $\mathcal{T}$, et $x$ une lettre qui n’est pas une constante de $\mathcal{T}$. Si $R$ est univoque en $x$ dans $\mathcal{T}$, $R \Rightarrow (x = \tau_x(R))$ est un théorème de $\mathcal{T}$. Réciproquement, si, pour un terme $T$ de $\mathcal{T}$ ne contenant pas $x$, $R \Rightarrow (x = T)$ est un théorème de $\mathcal{T}$, $R$ est univoque en $x$ dans $\mathcal{T}$.

Supposons que $R$ soit univoque en $x$ dans $\mathcal{T}$, et prouvons que $R \Rightarrow (x = \tau_x(R))$ est un théorème de $\mathcal{T}$. Adjoignons l’hypothèse $R$. Alors, $(\tau_x(R) \mid x)R$ est vraie d’après S5, donc « $R$ et $(\tau_x(R) \mid x)R$ » est vraie. Or, comme $R$ est univoque en $x$,

$$(R \text{ et } (\tau_x(R) \mid x)R) \Rightarrow (x = \tau_x(R))$$

est un théorème de $\mathcal{T}$ d’après C30 (I, p. 34). Donc $x = \tau_x(R)$ est vraie.

Réciproquement, supposons que $R \Rightarrow (x = T)$ soit un théorème de $\mathcal{T}$. Soient $y$, $z$ des lettres distinctes entre elles et distinctes de $x$, ne figurant ni dans $R$, ni dans les axiomes expli de $\mathcal{T}$. Comme $x$ n’est pas une constante de $\mathcal{T}$ et ne figure pas dans $T$, les relations $(y \mid x)R \Rightarrow (y = T)$ et $(z \mid x)R \Rightarrow (z = T)$ sont des théorèmes de $\mathcal{T}$. Adjoignons les hypothèses $(y \mid x)R$ et $(z \mid x)R$. Alors $y = T$ et $z = T$ sont vraies, donc $y = z$ est vraie.

Soit $R$ une relation de $\mathcal{T}$. La relation

$$((\exists x)R \text{ et il existe au plus un } x \text{ tel que } R)$$

se désigne par « il existe un $x$ et un seul tel que $R$ ». Si cette relation est un théorème de $\mathcal{T}$, on dit que $R$ est une relation fonctionnelle en $x$ dans $\mathcal{T}$.

**C46.** — Soient $R$ une relation de $\mathcal{T}$, et $x$ une lettre qui n’est pas une constante de $\mathcal{T}$. Si $R$ est fonctionnelle en $x$ dans $\mathcal{T}$, $R \Leftrightarrow (x = \tau_x(R))$ est un théorème de $\mathcal{T}$. Réciproquement, si, pour un terme $T$ de $\mathcal{T}$ ne contenant pas $x$, $R \Leftrightarrow (x = T)$ est un théorème de $\mathcal{T}$, $R$ est fonctionnelle en $x$ dans $\mathcal{T}$.

Supposons que $R$ soit fonctionnelle en $x$ dans $\mathcal{T}$. Alors, $R \Rightarrow (x = \tau_x(R))$ est un théorème de $\mathcal{T}$ d’après C45. D’autre part, $(\exists x)R$ est un théorème de $\mathcal{T}$. D’après S6, la relation

$$(x = \tau_x(R)) \Rightarrow (R \Leftrightarrow (\exists x)R)$$

est un théorème de $\mathcal{T}$. Si nous adjoignons l’hypothèse $x = \tau_x(R)$, on voit que $R$ est vraie. Donc $(x = \tau_x(R)) \Rightarrow R$ est un théorème de $\mathcal{T}$.

Réciproquement, si $R \Leftrightarrow (x = T)$ est un théorème de $\mathcal{T}$, $R$ est univoque en $x$ dans $\mathcal{T}$ d’après C45. En outre, $(T \mid x)R \Leftrightarrow (T = T)$ est un théorème de $\mathcal{T}$, donc $(T \mid x)R$, et par suite $(\exists x)R$, sont des théorèmes de $\mathcal{T}$.

Lorsqu’une relation $R$ est fonctionnelle en $x$ dans $\mathcal{T}$, $R$ est donc équivalente à la relation, souvent plus maniable, $x = \tau_x(R)$. Aussi introduit-on généralement un symbole abréviateur $\Sigma$ pour représenter le terme $\tau_x(R)$. Un tel symbole s’appelle symbole fonctionnel dans $\mathcal{T}$.

Intuitivement, $\Sigma$ représente l’objet unique qui possède la propriété définie par $R$.

\* Par exemple, dans une théorie où « $y$ est un nombre réel $\geq 0$ » est un théorème, la relation « $x$ est un nombre réel $\geq 0$ et $y=x^2$ » est fonctionnelle en $x$. On prend comme symbole fonctionnel correspondant $\sqrt{y}$ ou $y^{1/2}$. \*

C47. Soient $x$ une lettre qui n’est pas une constante de $\mathcal{T}$, $R\{x\}$ et $S\{x\}$ deux relations de $\mathcal{T}$. Si $R\{x\}$ est fonctionnelle en $x$ dans $\mathcal{T}$, la relation $S\{\tau_x(R)\}$ est équivalente à
$$
(\exists x)(R\{x\}\ \text{et}\ S\{x\}).
$$

En effet, il résulte de C46 et C43 que $(R\{x\}\ \text{et}\ S\{x\})$ est équivalente à $(R\{x\}\ \text{et}\ S\{\tau_x(R)\})$ ; comme $S\{\tau_x(R)\}$ ne contient pas $x$, $(\exists x)(R\{x\}\ \text{et}\ S\{\tau_x(R)\})$ est équivalente à

$$
S\{\tau_x(R)\}\ \text{et}\ (\exists x)R
$$

d’après C33 (I, p. 35) ; on conclut en remarquant que $(\exists x)R$ est vraie, puisque $R$ est fonctionnelle en $x$.

## EXERCICES {#ens-i-s5-exercises}

Dans tous ces exercices, $\mathscr{T}$ désigne une théorie égalitaire.

See the [exercises for § 5](exercises/s5/).
