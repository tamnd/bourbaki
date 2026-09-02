---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION DE LA MATHÉMATIQUE FORMELLE
section: 4
section_title: Théories quantifiées
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0032-0039, 0049-0049
extraction: ocr
subsections:
    - "no": 1
      title: Définition des quantificateurs
      page: 31
      pdf_page: 32
    - "no": 2
      title: Axiomes des théories quantifiées
      page: 0
      pdf_page: 34
    - "no": 3
      title: Propriétés des quantificateurs
      page: 0
      pdf_page: 34
    - "no": 4
      title: Quantificateurs typiques
      page: 35
      pdf_page: 36
statements: 0
exercises: 8
content_sha256: 879345d89491de488fd8242011036b46a7a2f4f3b183c11fbe847caf8282b0c0
---

## § 4. THÉORIES QUANTIFIÉES

### 1. Définition des quantificateurs

Dans le § 3, les seuls signes logiques qui aient joué un rôle sont $\neg$ et $\vee$ ; les règles qui vont être énoncées concernent essentiellement l'emploi des signes logiques $\tau$ et $\Box$.

DESCRIPTION DE LA MATHÉMATIQUE FORMELLE
§ 4

Si $R$ est un assemblage, et $x$ une lettre, l’assemblage $(\tau_x(R) \mid x)R$ se désigne par « il existe un $x$ tel que $R$ », ou par $(\exists x)R$. L’assemblage $\operatorname{non}((\exists x)\operatorname{non} R)$ se désigne par « pour tout $x$, $R$ », ou par « quel que soit $x$, $R$ », ou par $(\forall x)R$. Les symboles abréviateurs $\exists$ et $\forall$ s’appellent respectivement quantificateur existentiel et quantificateur universel. La lettre $x$ ne figure pas dans l’assemblage désigné par $\tau_x(R)$ ; elle ne figure donc pas dans les assemblages désignés par $(\exists x)R$ et $(\forall x)R$.

**CS8.** Soient $R$ un assemblage, $x$ et $x'$ des lettres. Si $x'$ ne figure pas dans $R$, $(\exists x)R$ et $(\forall x)R$ sont identiques respectivement à $(\exists x')R'$ et $(\forall x')R'$, où $R'$ est $(x' \mid x)R$.

En effet $(\tau_x(R) \mid x)R$ est identique à $(\tau_x(R) \mid x')R'$ d’après CS1 (I, p. 17), et $\tau_x(R)$ est identique à $\tau_{x'}(R')$ d’après CS3 (I, p. 17). Donc $(\exists x)R$ est identique à $(\exists x')R'$. Il en résulte que $(\forall x)R$ est identique à $(\forall x')R'$.

**CS9.** Soient $R$ et $U$ des assemblages, $x$ et $y$ des lettres distinctes. Si $x$ ne figure pas dans $U$, $(U \mid y)(\exists x)R$ et $(U \mid y)(\forall x)R$ sont identiques respectivement à $(\exists x)R'$ et $(\forall x)R'$, où $R'$ est $(U \mid y)R$.

En effet $(U \mid y)(\tau_x(R) \mid x)R$ est identique, d’après CS2 (I, p. 17), à $(T \mid x)(U \mid y)R$, où $T$ est $(U \mid y)\tau_x(R)$, c’est-à-dire $\tau_x(R')$ d’après CS4. D’où l’identité de $(U \mid y)(\exists x)R$ avec $(\exists x)R'$, et par suite celle de $(U \mid y)(\forall x)R$ avec $(\forall x)R'$.

**CF11.** Si $R$ est une relation d’une théorie $\mathcal{T}$ et $x$ une lettre, $(\exists x)R$ et $(\forall x)R$ sont des relations de $\mathcal{T}$.

Ceci résulte aussitôt de CF3, CF8 et CF2 (I, p. 19–20).

Intuitivement, considérons $R$ comme exprimant une propriété de l’objet désigné par $x$. D’après la signification intuitive du terme $\tau_x(R)$, affirmer $(\exists x)R$ revient à dire qu’il y a un objet possédant la propriété $R$. Affirmer $\operatorname{non}(\exists x)\operatorname{non} R$, c’est dire qu’il n’existe aucun objet ayant la propriété « non $R$ » ; c’est donc dire que tout objet possède la propriété $R$.

Si, dans une théorie logique $\mathcal{T}$, on dispose d’un théorème de la forme $(\exists x)R$, où la lettre $x$ n’est pas une constante de $\mathcal{T}$, ce théorème peut servir de théorème de légitimation dans la méthode de la constante auxiliaire (I, p. 28), puisqu’il est identique à $(\tau_x(R) \mid x)R$. Soit alors $\mathcal{T}'$ la théorie obtenue par adjonction de $R$ aux axiomes de $\mathcal{T}$. Si on peut démontrer dans $\mathcal{T}'$ une relation $S$ où $x$ ne figure pas, $S$ est un théorème de $\mathcal{T}$.

**C26.** Soient $\mathcal{T}$ une théorie logique, $R$ une relation de $\mathcal{T}$ et $x$ une lettre. Les relations $(\forall x)R$ et $(\tau_x(\operatorname{non} R) \mid x)R$ sont équivalentes dans $\mathcal{T}$.

En effet, $(\forall x)R$ est identique à « $\operatorname{non}(\tau_x(\operatorname{non} R) \mid x)(\operatorname{non} R)$ », donc à « $\operatorname{non}\operatorname{non}(\tau_x(\operatorname{non} R) \mid x)R$ ».

**C27.** Si $R$ est un théorème d’une théorie logique $\mathcal{T}$ dont la lettre $x$ n’est pas une constante, $(\forall x)R$ est un théorème de $\mathcal{T}$.

En effet, $(\tau_x(\operatorname{non} R) \mid x)R$ est un théorème de $\mathcal{T}$, d’après C3 (I, p. 23).

N° 3                                                                             THÉORIES QUANTIFIÉES                                                                             E I.33

Par contre, si $x$ est une constante de $\mathcal{T}$, la vérité de $R$ dans $\mathcal{T}$ n’entraîne pas celle de $(\forall x)R$. Intuitivement, le fait que $R$ soit une propriété vraie de $x$, qui est, dans $\mathcal{T}$, un objet déterminé, n’entraîne évidemment pas que $R$ soit une propriété vraie de tout objet.

**C28.** Soient $\mathcal{T}$ une théorie logique, $R$ une relation de $\mathcal{T}$ et $x$ une lettre. Les relations « non $(\forall x)R$ » et « $(\exists x)(non R)$ » sont équivalentes dans $\mathcal{T}$.

En effet, « non $(\forall x)R$ » est identique à « non non $(\exists x)(non R)$ ».

### 2. Axiomes des théories quantifiées

On appelle théorie quantifiée toute théorie $\mathcal{T}$ dans laquelle les schémas S1 à S4 (I, p. 25) et le schéma S5 ci-dessous fournissent des axiomes impli.

S5. Si $R$ est une relation de $\mathcal{T}$, $T$ un terme de $\mathcal{T}$, et $x$ une lettre, la relation $(T \mid x)R \Rightarrow (\exists x)R$ est un axiome.

Cette règle est bien un schéma. En effet, soit $A$ un axiome de $\mathcal{T}$ obtenu par application de S5 : il y a donc une relation $R$ de $\mathcal{T}$, un terme $T$ de $\mathcal{T}$ et une lettre $x$ tels que $A$ soit $(T \mid x)R \Rightarrow (\exists x)R$. Soient $U$ un terme de $\mathcal{T}$, $y$ une lettre ; on va montrer que $(U \mid y)A$ s’obtient encore par application de S5. Par utilisation de CS1 (I, p. 17), et CS8 (I, p. 32), on peut se ramener au cas où $x$ est distincte de $y$ et ne figure pas dans $U$. Soient alors $R'$ la relation $(U \mid y)R$ et $T'$ le terme $(U \mid y)T$. Les critères CS2 (I, p. 17) et CS9 (I, p. 32) montrent que $(U \mid y)A$ est identique à $(T' \mid x)R' \Rightarrow (\exists x)R'$.

Le schéma S5 exprime que s’il y a un objet $T$ pour lequel la relation $R$, considérée comme exprimant une propriété de $x$, est vraie, alors $R$ est vraie pour l’objet $\tau_x(R)$ ; ce qui est en accord avec la signification intuitive que nous avons attribuée à $\tau_x(R)$ (I, p. 18, Remarque).

### 3. Propriétés des quantificateurs

Nous n’aurons désormais à considérer que des théories quantifiées. Dans toute la fin de ce paragraphe, on désigne par $\mathcal{T}$ une telle théorie, et par $\mathcal{T}_0$ la théorie sans axiomes expli qui possède les mêmes signes que $\mathcal{T}$ et les seuls schémas S1 à S5 ; $\mathcal{T}$ est plus forte que $\mathcal{T}_0$.

**C29.** Soient $R$ une relation de $\mathcal{T}$, et $x$ une lettre. Les relations « non $(\exists x)R$ » et « $(\forall x)(non R)$ » sont équivalentes dans $\mathcal{T}$.

En effet, il suffit d’établir le critère dans la théorie $\mathcal{T}_0$, dont $x$ n’est pas une constante. Le théorème $R \Leftrightarrow (non\ non\ R)$ donne par C3 (I, p. 23), les théorèmes

$$
(\exists x)R \Rightarrow (\tau_x(R) \mid x)(non\ non\ R)
$$

et

$$
(\exists x)(non\ non\ R) \Rightarrow (\tau_x(non\ non\ R) \mid x)R.
$$

Appliquant S5, on en déduit dans $\mathcal{T}_0$ les théorèmes

$$
(\exists x)R \Rightarrow (\exists x)(\mathrm{non}\ \mathrm{non}\ R),
$$

et

$$
(\exists x)(\mathrm{non}\ \mathrm{non}\ R) \Rightarrow (\exists x)R,
$$

d’où le théorème $(\exists x)R \Leftrightarrow (\exists x)(\mathrm{non}\ \mathrm{non}\ R)$. Or, $(\exists x)(\mathrm{non}\ \mathrm{non}\ R)$ est équivalente dans $\mathcal{T}_0$ à « non$(\forall x)(\mathrm{non}\ R)$ », c’est-à-dire à « non$(\forall x)(\mathrm{non}\ R)$ ». D’où le critère.

Les critères C28 et C29 permettent de déduire les propriétés d’un des quantificateurs de celles de l’autre.

**C30.** — Soient $R$ une relation de $\mathcal{T}$, $T$ un terme de $\mathcal{T}$, $x$ une lettre. La relation $(\forall x)R \Rightarrow (T|x)R$ est un théorème de $\mathcal{T}$.

D’après S5, $(T|x)(\mathrm{non}\ R) \Rightarrow (\tau_x(\mathrm{non}\ R)|x)(\mathrm{non}\ R)$ est un axiome. Cette relation est identique à

$$
(\mathrm{non}\ (T|x)R) \Rightarrow (\mathrm{non}\ (\tau_x(\mathrm{non}\ R)|x)R).
$$

Donc $(\tau_x(\mathrm{non}\ R)|x)R \Rightarrow (T|x)R$ est un théorème de $\mathcal{T}$. On conclut par application de C26 (I, p. 32).

Soit $R$ une relation de $\mathcal{T}$. D’après C26, C27 et C30, il revient au même (lorsque la lettre $x$ n’est pas une constante de $\mathcal{T}$) d’énoncer dans $\mathcal{T}$ le théorème $R$, ou le théorème $(\forall x)R$, ou enfin d’énoncer la règle métamathématique : si $T$ est un terme quelconque de $\mathcal{T}$, $(T|x)R$ est un théorème de $\mathcal{T}$.

**C31.** — Soient $R$ et $S$ des relations de $\mathcal{T}$, et $x$ une lettre qui n’est pas une constante de $\mathcal{T}$. Si $R \Rightarrow S$ (resp. $R \Leftrightarrow S$) est un théorème de $\mathcal{T}$, $(\forall x)R \Rightarrow (\forall x)S$ et $(\exists x)R \Rightarrow (\exists x)S$ (resp. $(\forall x)R \Leftrightarrow (\forall x)S$ et $(\exists x)R \Leftrightarrow (\exists x)S$) sont des théorèmes de $\mathcal{T}$.

En effet, supposons que $R \Rightarrow S$ soit un théorème de $\mathcal{T}$. Adjoignons l’hypothèse $(\forall x)R$ (où $x$ ne figure pas). Alors $R$, donc $S$, donc aussi $(\forall x)S$, sont vraies. Par suite $(\forall x)R \Rightarrow (\forall x)S$ est un théorème de $\mathcal{T}$. Il en résulte que, si $R \Leftrightarrow S$ est un théorème de $\mathcal{T}$, il en est de même de $(\forall x)R \Leftrightarrow (\forall x)S$. Les règles relatives à $\exists$ s’en déduisent par emploi de C29.

**C32.** — Soient $R$ et $S$ des relations de $\mathcal{T}$, et $x$ une lettre. Les relations

$$
(\forall x)(R\ \mathrm{et}\ S) \Leftrightarrow ((\forall x)R\ \mathrm{et}\ (\forall x)S)
$$

$$
(\exists x)(R\ \mathrm{ou}\ S) \Leftrightarrow ((\exists x)R\ \mathrm{ou}\ (\exists x)S)
$$

sont des théorèmes de $\mathcal{T}$.

En effet, il suffit d’établir ces critères dans $\mathcal{T}_0$, dont $x$ n’est pas une constante. Si $(\forall x)(R\ \mathrm{et}\ S)$ est vraie, « $R$ et $S$ » est vraie, donc chacune des relations $R$, $S$ est vraie ; par suite chacune des relations $(\forall x)R$, $(\forall x)S$ est vraie, donc

« $(\forall x)R$ et $(\forall x)S$ »

est vraie. On voit de même que, si « $(\forall x)R$ et $(\forall x)S$ » est vraie, $(\forall x)(R\ \mathrm{et}\ S)$ est vraie. D’où le premier théorème. Le deuxième s’en déduit par emploi de C29.

On aura soin de noter que si $(\forall x)(R$ ou $S)$ est un théorème de $\mathscr{T}$, on ne peut en conclure que $(\forall x)R$ ou $(\forall x)S$ soit un théorème de $\mathscr{T}$. Intuitivement, dire que la relation $(\forall x)(R$ ou $S)$ est vraie signifie que, pour tout objet $x$, l’une au moins des relations $R$, $S$ est vraie; mais, en général, une seule d’eux sera vraie, et suivant le choix de $x$, ce pourra être l’une ou l’autre des relations $R$, $S$. On voit de même que si $(\exists x)R$ et $(\exists x)S$ est un théorème de $\mathscr{T}$, on ne peut en conclure que $(\exists x)(R$ et $S)$ soit un théorème de $\mathscr{T}$. On a toutefois le critère suivant:

C33. Soient $R$ et $S$ des relations de $\mathscr{T}$, et $x$ une lettre qui ne figure pas dans $R$. Les relations

$$(\forall x)(R\ \mathrm{ou}\ S)\Leftrightarrow(R\ \mathrm{ou}\ (\forall x)S)$$

$$(\exists x)(R\ \mathrm{et}\ S)\Leftrightarrow(R\ \mathrm{et}\ (\exists x)S)$$

sont des théorèmes de $\mathscr{T}$.

En effet, il suffit d’établir le critère dans $\mathscr{T}_0$, dont $x$ n’est pas une constante. Soit $\mathscr{T}'$ la théorie obtenue en adjoignant $(\forall x)(R\ \mathrm{ou}\ S)$ aux axiomes de $\mathscr{T}_0$. Dans $\mathscr{T}'$, «$R$ ou $S$», donc $(\mathrm{non}\ R)\Rightarrow S$, sont des théorèmes. Si «non $R$» est vraie (hypothèse où $x$ ne figure pas), $S$, donc aussi $(\forall x)S$, sont vraies. Donc $(\mathrm{non}\ R)\Rightarrow(\forall x)S$ est un théorème de $\mathscr{T}'$, et par suite $(\forall x)(R\ \mathrm{ou}\ S)\Rightarrow(R\ \mathrm{ou}\ (\forall x)S)$ est un théorème de $\mathscr{T}_0$. De même, si «$R$ ou $(\forall x)S$» est vraie, «$R$ ou $S$», donc $(\forall x)(R\ \mathrm{ou}\ S)$, sont vraies. Par suite $(R\ \mathrm{ou}\ (\forall x)S)\Rightarrow(\forall x)(R\ \mathrm{ou}\ S)$ est un théorème de $\mathscr{T}_0$. La règle relative à $\exists$ en déduit par emploi de C29.

C34. Soient $R$ une relation, $x$ et $y$ des lettres. Les relations

$$(\forall x)(\forall y)R\Leftrightarrow(\forall y)(\forall x)R$$

$$(\exists x)(\exists y)R\Leftrightarrow(\exists y)(\exists x)R$$

$$(\exists x)(\forall y)R\Rightarrow(\forall y)(\exists x)R$$

sont des théorèmes de $\mathscr{T}$.

En effet, il suffit d’établir le critère dans $\mathscr{T}_0$, dont $x$, $y$ ne sont pas des constantes. Si $(\forall x)(\forall y)R$ est vraie, $(\forall y)R$, donc $R$, donc $(\forall x)R$, donc $(\forall y)(\forall x)R$ sont vraies. De même, si $(\forall y)(\forall x)R$ est vraie, $(\forall x)(\forall y)R$ est vraie. D’où le premier théorème. Le deuxième s’en déduit par emploi de C29. Enfin, puisque $(\forall y)R\Rightarrow R$ est un théorème de $\mathscr{T}_0$, il en est de même de $(\exists x)(\forall y)R\Rightarrow(\exists x)R$ d’après C31; si $(\exists x)(\forall y)R$ est vraie, $(\exists x)R$ est donc vraie, et par suite aussi $(\forall y)(\exists x)R$. D’où le troisième théorème.

Par contre, si $(\forall y)(\exists x)R$ est un théorème de $\mathscr{T}$, on ne peut en conclure que $(\exists x)(\forall y)R$ est un théorème de $\mathscr{T}$. Intuitivement, dire que la relation $(\forall y)(\exists x)R$ est vraie signifie qu’étant donné un objet $y$ quelconque, il y a un objet $x$ tel que $R$ soit une relation vraie entre les objets $x$ et $y$. Mais l’objet $x$ dépendra en général du choix de l’objet $y$. Au contraire, dire que $(\exists x)(\forall y)R$ est vraie signifie qu’il y a un objet fixe $x$ tel que $R$ soit une relation vraie entre cet objet et tout objet $y$.

### 4. Quantificateurs typiques

Soient $A$ et $R$ des assemblages, et $x$ une lettre. On désigne l’assemblage $(\exists_Ax)(A\ \mathrm{et}\ R)$ par $(\exists_Ax)R$, et l’assemblage «non $(\exists_Ax)(\mathrm{non}\ R)$» par $(\forall_Ax)R$. Les symboles

E I.36                                DESCRIPTION DE LA MATHÉMATIQUE FORMELLE                                § 4

abréviateurs $\exists_A$ et $\forall_A$ sont appelés quantificateurs typiques. On notera que la lettre $x$ ne figure pas dans les assemblages désignés par

$$
(\exists_Ax)R \qquad (\forall_Ax)R.
$$

**CS10.** — Soient $A$ et $R$ des assemblages, $x$ et $x'$ des lettres. Si $x'$ ne figure ni dans $R$ ni dans $A$, $(\exists_Ax)R$ et $(\forall_Ax)R$ sont identiques respectivement à $(\exists_{A'x'})R'$ et $(\forall_{A'x'})R'$, où $R'$ est $(x'|x)R$, et où $A'$ est $(x'|x)A$.

**CS11.** — Soient $A$, $R$, $U$ des assemblages, $x$ et $y$ des lettres distinctes. Si $x$ ne figure pas dans $U$, les assemblages $(U|y)(\exists_Ax)R$ et $(U|y)(\forall_Ax)R$ sont identiques respectivement à $(\exists_{A'x})R'$ et $(\forall_{A'x})R'$, où $R'$ est $(U|y)R$ et où $A'$ est $(U|y)A$.

Ces règles résultent aussitôt des critères CS8, CS9 (I, p. 32), CS5 (I, p. 17) et CS6 (I, p. 29).

**CF12.** — Soient $A$ et $R$ des relations de $\mathcal{J}$, et $x$ une lettre. Alors, $(\exists_Ax)R$ et $(\forall_Ax)R$ sont des relations de $\mathcal{J}$.

Cela résulte aussitôt de CF11 (I, p. 32), CF9 (I, p. 29) et CF2 (I, p. 19).

Intuitivement, considérons $A$ et $R$ comme exprimant des propriétés de $x$. Il peut arriver que, dans une série de démonstrations, on ne s’intéresse qu’aux objets vérifiant $A$. Dire qu’il existe un objet vérifiant $A$ tel que $R$, c’est dire qu’il existe un objet tel que « $A$ et $R$ » ; d’où la définition de $\exists_A$. Dire que tous les objets vérifiant $A$ ont la propriété $R$, c’est dire qu’il n’existe pas d’objets vérifiant $A$ et tels que « non $R$ » ; d’où la définition de $\forall_A$. Dans la pratique, ces signes sont remplacés par des phrases assez diverses suivant la nature de la relation $A$. \* On dira par exemple : « quel que soit l’entier $x$, $R$ », « il existe un élément $x$ de l’ensemble $E$ tel que $R$ », etc.*

**CS5.** — Soient $A$ et $R$ des relations de $\mathcal{J}$, $x$ une lettre. Les relations $(\forall_Ax)R$ et $(\forall x)(A\Rightarrow R)$ sont équivalentes dans $\mathcal{J}$.

En effet, la relation $(\forall_Ax)R$ est identique à

$$
\text{« non }(\exists x)(A\text{ et }(\text{non }R))\text{ »}.
$$

Or, « $A$ et (non $R$) » est équivalente dans $\mathcal{J}_0$ à non$(A\Rightarrow R)$, donc

$$
\text{« non }(\exists x)(A\text{ et }(\text{non }R))\text{ »}
$$

est équivalente dans $\mathcal{J}_0$ à « non $(\exists x)(\text{non }(A\Rightarrow R))$ » d’après C31 (I, p. 34), et cette dernière relation est identique à $(\forall x)(A\Rightarrow R)$. Le critère est donc établi dans $\mathcal{J}_0$, et par suite dans $\mathcal{J}$.

On a souvent à démontrer des relations de la forme $(\forall_Ax)R$. On le fait généralement en s’aidant d’un des deux critères suivants :

**C36.** — Soient $A$ et $R$ des relations de $\mathcal{J}$, $x$ une lettre. Soit $\mathcal{J}'$ la théorie obtenue en adjoignant $A$ aux axiomes de $\mathcal{J}$. Si $x$ n’est pas une constante de $\mathcal{J}$, et si $R$ est un théorème de $\mathcal{J}'$, $(\forall_Ax)R$ est un théorème de $\mathcal{J}$.

En effet, $A\Rightarrow R$ est un théorème de $\mathcal{J}$ d’après le critère de la déduction, donc $(\forall_Ax)R$ est un théorème de $\mathcal{J}$ d’après C27 (I, p. 32) et C35.

En pratique, on indique qu’on va employer cette règle par une phrase du genre suivant : « Soit $x$ un élément quelconque tel que $A$. » Dans la théorie $\mathcal{T}'$ ainsi constituée, on cherche à démontrer $R$. On ne peut naturellement affirmer que $R$ soit elle-même un théorème de $\mathcal{T}$.

C37. Soient $A$ et $R$ des relations de $\mathcal{T}$, $x$ une lettre. Soit $\mathcal{T}'$ la théorie obtenue en adjoignant les relations $A$ et « non $R$ » aux axiomes de $\mathcal{T}$. Si $x$ n’est pas une constante de $\mathcal{T}$, et si $\mathcal{T}'$ est contradictoire, $(\forall_A x)R$ est un théorème de $\mathcal{T}$.

En effet, la théorie $\mathcal{T}'$ est équivalente à la théorie obtenue en adjoignant « non $(A \Rightarrow R)$ » aux axiomes de $\mathcal{T}$. D’après la méthode de réduction à l’absurde, $A \Rightarrow R$ est un théorème de $\mathcal{T}$, donc aussi $(\forall_A x)R$ d’après C27 (I, p. 32) et C35.

En pratique, on dit : « Supposons qu’il existe un objet $x$ vérifiant $A$, pour lequel $R$ soit fausse », et on cherche à établir une contradiction.

Les propriétés des quantificateurs typiques sont analogues à celles des quantificateurs :

C38. Soient $A$ et $R$ des relations de $\mathcal{T}$, $x$ une lettre. Les relations

$$
\operatorname{non}(\forall_A x)R \Longleftrightarrow (\exists_A x)(\operatorname{non}\ R),
$$

$$
\operatorname{non}(\exists_A x)R \Longleftrightarrow (\forall_A x)(\operatorname{non}\ R)
$$

sont des théorèmes de $\mathcal{T}$.

C39. Soient $A$, $R$ et $S$ des relations de $\mathcal{T}$, et $x$ une lettre qui n’est pas une constante de $\mathcal{T}$. Si la relation $A \Rightarrow (R \Rightarrow S)$ (resp. $A \Rightarrow (R \Leftrightarrow S)$) est un théorème de $\mathcal{T}$, les relations

$$
(\exists_A x)R \Rightarrow (\exists_A x)S,\qquad (\forall_A x)R \Rightarrow (\forall_A x)S
$$

(resp.

$$
(\exists_A x)R \Leftrightarrow (\exists_A x)S,\qquad (\forall_A x)R \Leftrightarrow (\forall_A x)S
$$

)

sont des théorèmes de $\mathcal{T}$.

C40. Soient $A$, $R$ et $S$ des relations de $\mathcal{T}$, et $x$ une lettre. Les relations

$$
(\forall_A x)(R\ \text{et}\ S) \Leftrightarrow ((\forall_A x)R\ \text{et}\ (\forall_A x)S)
$$

$$
(\exists_A x)(R\ \text{ou}\ S) \Leftrightarrow ((\exists_A x)R\ \text{ou}\ (\exists_A x)S)
$$

sont des théorèmes de $\mathcal{T}$.

C41. Soient $A$, $R$ et $S$ des relations de $\mathcal{T}$, et $x$ une lettre qui ne figure pas dans $R$. Les relations

$$
(\forall_A x)(R\ \text{ou}\ S) \Leftrightarrow (R\ \text{ou}\ (\forall_A x)S)
$$

$$
(\exists_A x)(R\ \text{et}\ S) \Leftrightarrow (R\ \text{et}\ (\exists_A x)S)
$$

sont des théorèmes de $\mathcal{T}$.

C42. Soient $A$, $B$, $R$ des relations de $\mathcal{T}$, $x$ et $y$ des lettres. Si $x$ ne figure pas dans $B$, et si $y$ ne figure pas dans $A$, les relations

$$
(\forall_A x)(\forall_B y)R \Leftrightarrow (\forall_B y)(\forall_A x)R
$$

$$
(\exists_A x)(\exists_B y)R \Leftrightarrow (\exists_B y)(\exists_A x)R
$$

$$
(\exists_A x)(\forall_B y)R \Rightarrow (\forall_B y)(\exists_A x)R
$$

sont des théorèmes de $\mathcal{T}$.

E I.38                                     DESCRIPTION DE LA MATHÉMATIQUE FORMELLE                                     § 5

A titre d’exemple, démontrons une partie de C42. La relation $(\exists_a x)(\exists_b y)R$ est identique à $(\exists x)(A \text{ et } (\exists y)(B \text{ et } R))$, donc est équivalente dans $\mathcal{T}_0$ (puisque $y$ ne figure pas dans $A$) à $(\exists x)(\exists y)(A \text{ et } (B \text{ et } R))$, d’après C33 et C31. De même, $(\exists_b y)(\exists_a x)R$ est équivalente à $(\exists y)(\exists x)(B \text{ et } (A \text{ et } R))$. On conclut par application de C31 et C34 (I, p. 35).

\* Comme exemple d’application des critères précédents, considérons la relation suivante: « la suite de fonctions numériques $(f_n)$ converge uniformément vers 0 dans $[0,1]$ », ce qui signifie: « pour tout $\epsilon > 0$, il existe un entier $n$ tel que, pour tout $x \in [0,1]$ et pour tout entier $m \geq n$, on ait $|f_m(x)| \leq \epsilon$ ». Supposons qu’on veuille prendre la négation de cette relation (par exemple pour faire un raisonnement par l’absurde); le critère C38 montre que cette négation est équivalente à la relation suivante: « il existe un $\epsilon > 0$ tel que, pour tout entier $n$, il existe un $x \in [0,1]$ et un $m \geq n$ pour lesquels $|f_m(x)| > \epsilon$ ». \*

## EXERCICES {#ens-i-s4-exercises}

Dans tous ces exercices, $\mathcal{T}$ désigne une théorie quantifiée.

See the [exercises for § 4](exercises/s4/).
