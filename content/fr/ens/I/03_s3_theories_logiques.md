---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION DE LA MATHÉMATIQUE FORMELLE
section: 3
section_title: Théories logiques
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
pdf_pages: 0026-0032, 0048-0049
extraction: ocr
subsections:
    - "no": 1
      title: Les axiomes
      page: 0
      pdf_page: 26
    - "no": 2
      title: Premières conséquences
      page: 0
      pdf_page: 26
    - "no": 3
      title: Méthodes de démonstration
      page: 0
      pdf_page: 28
    - "no": 4
      title: La conjonction
      page: 0
      pdf_page: 30
    - "no": 5
      title: L'équivalence
      page: 30
      pdf_page: 31
statements: 0
exercises: 5
content_sha256: a9e606302e0a28ffccc3bf015876fe5913aaa9bf423563abd3bbca7d01136a41
---

## § 3. THÉORIES LOGIQUES

### 1. Les axiomes

On appelle *théorie logique* toute théorie $\mathcal T$ dans laquelle les schémas S1 à S4 ci-dessous fournissent des axiomes impli.

S1. Si $A$ est une relation de $\mathcal T$, la relation $(A\text{ ou }A)\Rightarrow A$ est un axiome de $\mathcal T$.[^1]

S2. Si $A$ et $B$ sont des relations de $\mathcal T$, la relation $A\Rightarrow(A\text{ ou }B)$ est un axiome de $\mathcal T$.

S3. Si $A$ et $B$ sont des relations de $\mathcal T$, la relation $(A\text{ ou }B)\Rightarrow(B\text{ ou }A)$ est un axiome de $\mathcal T$.

S4. Si $A$, $B$ et $C$ sont des relations de $\mathcal T$, la relation

$$
(A\Rightarrow B)\Rightarrow((C\text{ ou }A)\Rightarrow(C\text{ ou }B))
$$

est un axiome de $\mathcal T$.

Ces règles sont effectivement des schémas; vérifions-le par exemple pour S2. Soit $R$ une relation obtenue par application de S2: il y a donc des relations $A$, $B$ de $\mathcal T$ telles que $R$ soit la relation $A\Rightarrow(A\text{ ou }B)$; soient $T$ un terme de $\mathcal T$ et $x$ une lettre; soient $A'$ et $B'$ les relations $(T\mid x)A$ et $(T\mid x)B$; alors $(T\mid x)R$ est identique à $A'\Rightarrow(A'\text{ ou }B')$, donc s’obtient par application de S2.

*Intuitivement, les règles S1 à S4 ne font qu’exprimer le sens qu’on attache aux mots « ou » et « implique » dans le langage mathématique usuel.*[^2]

Si une théorie logique $\mathcal T$ est contradictoire, *toute relation de $\mathcal T$ est un théorème de $\mathcal T$.* En effet, soit $A$ une relation de $\mathcal T$ telle que $A$ et « non $A$ » soient des théorèmes de $\mathcal T$, et soit $B$ une relation quelconque de $\mathcal T$. D’après S2, $(\text{non }A)\Rightarrow((\text{non }A)\text{ ou }B)$ est un théorème de $\mathcal T$, donc, d’après C1 (I, p. 23) « $(\text{non }A)\text{ ou }B$ », c’est-à-dire $A\Rightarrow B$, est un théorème de $\mathcal T$. Une nouvelle application de C1 montre que $B$ est un théorème de $\mathcal T$.

*Dans toute la suite, $\mathcal T$ désignera une théorie logique.*

### 2. Premières conséquences

C6. *Soient* $A$, $B$, $C$ *des relations de* $\mathcal T$. *Si* $A\Rightarrow B$ *et* $B\Rightarrow C$ *sont des théorèmes de* $\mathcal T$, $A\Rightarrow C$ *est un théorème de* $\mathcal T$.

DESCRIPTION DE LA MATHÉMATIQUE FORMELLE
§ 3

En effet, $(B \Rightarrow C) \Rightarrow ((A \Rightarrow B) \Rightarrow (A \Rightarrow C))$ est un axiome de $\mathcal{T}$, d’après S4 où on remplace $A$ par $B$, $B$ par $C$, et $C$ par « non $A$ ». D’après C1 (I, p. 23), $(A \Rightarrow B) \Rightarrow (A \Rightarrow C)$ est un théorème de $\mathcal{T}$. On conclut par une nouvelle application de C1.

C7. Si $A$ et $B$ sont des relations de $\mathcal{T}$, $B \Rightarrow (A$ ou $B)$ est un théorème de $\mathcal{T}$.

En effet, $B \Rightarrow (B$ ou $A)$, et $(B$ ou $A) \Rightarrow (A$ ou $B)$ sont des axiomes de $\mathcal{T}$ d’après S2 et S3. On conclut par application de C6.

C8. Si $A$ est une relation de $\mathcal{T}$, $A \Rightarrow A$ est un théorème de $\mathcal{T}$.

En effet, $A \Rightarrow (A$ ou $A)$, et $(A$ ou $A) \Rightarrow A$ sont des axiomes d’après S2 et S1. On conclut par application de C6.

C9. Si $A$ est une relation, et $B$ un théorème de $\mathcal{T}$, $A \Rightarrow B$ est un théorème de $\mathcal{T}$.

En effet, $B \Rightarrow ((\text{non } A)$ ou $B)$ est un théorème d’après C7, donc

« $(\text{non } A)$ ou $B$ », c’est-à-dire $A \Rightarrow B$,

est un théorème d’après C1.

C10. Si $A$ est une relation de $\mathcal{T}$, « $A$ ou $(\text{non } A)$ » est un théorème de $\mathcal{T}$.

En effet, « $(\text{non } A)$ ou $A$ » est un théorème d’après C8. On conclut par S3 et C1.

C11. Si $A$ est une relation de $\mathcal{T}$, « $A \Rightarrow (\text{non non } A)$ » est un théorème de $\mathcal{T}$.

En effet, cette relation n’est autre que « $(\text{non } A)$ ou $(\text{non non } A)$ » et le critère résulte de C10.

C12. Soient $A$ et $B$ deux relations de $\mathcal{T}$. La relation

$$
(A \Rightarrow B) \Rightarrow ((\text{non } B) \Rightarrow (\text{non } A))
$$

est un théorème de $\mathcal{T}$.

En effet,

$$
((\text{non } A) \text{ ou } B) \Rightarrow ((\text{non } A) \text{ ou } (\text{non non } B))
$$

est un théorème d’après C11, S4 et C1. D’autre part,

$$
((\text{non } A) \text{ ou } (\text{non non } B)) \Rightarrow ((\text{non non } B) \text{ ou } (\text{non } A))
$$

est un axiome d’après S3. Donc

$$
((\text{non } A) \text{ ou } B) \Rightarrow ((\text{non non } B) \text{ ou } (\text{non } A))
$$

est un théorème d’après C6. Or, c’est la relation à établir.

C13. Soient $A$, $B$, $C$ des relations de $\mathcal{T}$. Si $A \Rightarrow B$ est un théorème de $\mathcal{T}$,

$$
(B \Rightarrow C) \Rightarrow (A \Rightarrow C)
$$

est un théorème de $\mathcal{T}$.

En effet, $(\text{non } B) \Rightarrow (\text{non } A)$ est un théorème d’après C12 et C1. Donc $(C$ ou $(\text{non } B)) \Rightarrow (C$ ou $(\text{non } A))$ est un théorème d’après S4 et C1. Par double application de S3 et de C6, on en conclut que $((\text{non } B)$ ou $C) \Rightarrow ((\text{non } A)$ ou $C)$ est un théorème. Or, ceci est la relation à démontrer.

Nº 3                                                                                     THÉORIES LOGIQUES                                                                                     E I.27

Désormais, nous emploierons le plus souvent les règles C1 et C6 sans nous y référer expli.

### 3. Méthodes de démonstration

I. Méthode de l’hypothèse auxiliaire. — Elle repose sur la règle suivante:

C14 (critère de la déduction). Soient $A$ une relation de $\mathcal{T}$, et $\mathcal{T}'$ la théorie obtenue en adjoignant $A$ aux axiomes de $\mathcal{T}$. Si $B$ est un théorème de $\mathcal{T}'$, $A \Rightarrow B$ est un théorème de $\mathcal{T}$. Soit $B_1, B_2, \ldots, B_n$ une démonstration de $\mathcal{T}'$ dans laquelle figure $B$. Nous allons montrer de proche en proche que les relations $A \Rightarrow B_k$ sont des théorèmes de $\mathcal{T}$. Supposons ceci établi pour les relations qui précèdent $B_i$, et prouvons que $A \Rightarrow B_i$ est un théorème de $\mathcal{T}$. Si $B_i$ est un axiome de $\mathcal{T}'$, $B_i$ est, soit un axiome de $\mathcal{T}$, soit $A$. Dans les deux cas, $A \Rightarrow B_i$ est un théorème de $\mathcal{T}$, par application de C9 ou de C8. Si $B_i$ est précédée des relations $B_j$ et $B_j \Rightarrow B_i$, on sait que $A \Rightarrow B_j$ et $A \Rightarrow (B_j \Rightarrow B_i)$ sont des théorèmes de $\mathcal{T}$. Alors $(B_j \Rightarrow B_i) \Rightarrow (A \Rightarrow B_i)$ est un théorème de $\mathcal{T}$ d’après C13. Donc, d’après C6, $A \Rightarrow (A \Rightarrow B_i)$, c’est-à-dire « (non $A$) ou $(A \Rightarrow B_i)$ » est un théorème de $\mathcal{T}$, et par suite aussi

$$((A \Rightarrow B_i) ou (non A)) \Rightarrow ((A \Rightarrow B_i) ou (A \Rightarrow B_i))$$

d’après S3. Or, $(non A) \Rightarrow ((non A) ou B_i)$, c’est-à-dire $(non A) \Rightarrow (A \Rightarrow B_i)$ est un théorème de $\mathcal{T}$ d’après S2. Par application de S4, on voit que

$$((A \Rightarrow B_i) ou (non A)) \Rightarrow ((A \Rightarrow B_i) ou (A \Rightarrow B_i))$$

est un théorème de $\mathcal{T}$, donc que « $(A \Rightarrow B_i)$ ou $(A \Rightarrow B_i)$ » est un théorème de $\mathcal{T}$. Par S1, on conclut que $A \Rightarrow B_i$ est un théorème de $\mathcal{T}$.

En pratique, on indique qu’on va employer ce critère par une phrase du genre suivant: « Supposons que $A$ soit vraie ». Cette phrase signifie qu’on va raisonner pour un moment dans la théorie $\mathcal{T}'$. On reste dans $\mathcal{T}'$ jusqu’à ce que l’on y ait démontré la relation $B$. Ceci fait, il est établi que $A \Rightarrow B$ est un théorème de $\mathcal{T}$, et on continue (s’il y a lieu) à raisonner dans $\mathcal{T}$ sans indiquer en général qu’on a abandonné $\mathcal{T}'$. La relation $A$ que l’on a introduite comme nouvel axiome s’appelle l’hypothèse auxiliaire. \* Par exemple, quand on dit: « Soit $x$ un nombre réel », on construit une théorie dans laquelle la relation « $x$ est un nombre réel » est une hypothèse auxiliaire.\*

II. Méthode de réduction à l’absurde. — Elle repose sur la règle suivante:

C15. Soient $A$ une relation de $\mathcal{T}$, et $\mathcal{T}'$ la théorie obtenue en adjoignant l’axiome « non $A$ » aux axiomes de $\mathcal{T}$. Si $\mathcal{T}'$ est contradictoire, $A$ est un théorème de $\mathcal{T}$.

En effet, $A$ est un théorème de $\mathcal{T}'$. Par suite (méthode de l’hypothèse auxiliaire), $(non A) \Rightarrow A$ est un théorème de $\mathcal{T}$. D’après S4,

$$(A ou (non A)) \Rightarrow (A ou A)$$

est un théorème de $\mathcal{T}$. D’après C10, « $A$ ou $A$ » est un théorème de $\mathcal{T}$. On conclut par application de S1.

En pratique, on indique qu’on va employer ce critère par une phrase du genre suivant: « Supposons que $A$ soit fausse ». Cette phrase signifie qu’on va raisonner pour un moment dans $\mathcal{T}'$. On reste dans $\mathcal{T}'$ jusqu’à ce que l’on ait établi deux théorèmes de la forme $B$ et « non $B$ ». Ceci fait, il est établi que $A$ est un théorème de $\mathcal{T}$, ce qu’on indique en général par une phrase du genre suivant : « Or ceci (à savoir, dans les notations précédentes, $B$ et « non $B$ ») est absurde; donc $A$ est vrai ». On revient alors à la théorie $\mathcal{T}$ dont on s’occupait précédemment.

Comme premières applications de ces méthodes, démontrons les critères suivants :

C16. Si $A$ est une relation de $\mathcal{T}$, (non non $A$) $\Rightarrow A$ est un théorème de $\mathcal{T}$.

En effet, supposons « non non $A$ » vraie; il faut prouver $A$. Supposons $A$ fausse. Dans la théorie ainsi fondée, « non non $A$ » et « non $A$ » sont des théorèmes. Ceci est absurde; donc $A$ est vraie.

C17. Si $A$ et $B$ sont des relations de $\mathcal{T}$,

$((\text{non } B) \Rightarrow (\text{non } A)) \Rightarrow (A \Rightarrow B)$

est un théorème de $\mathcal{T}$.

En effet, supposons $(\text{non } B) \Rightarrow (\text{non } A)$ vraie. Il faut prouver que $A \Rightarrow B$ est vraie. Or, supposons $A$ vraie et prouvons que $B$ est vraie. Supposons « non $B$ » vraie. Alors, « non $A$ » est vraie, ce qui est absurde.

III. Méthode de disjonction des cas. — Elle repose sur la règle suivante:

C18. Soient $A$, $B$, $C$ des relations de $\mathcal{T}$. Si « $A$ ou $B$ », $A \Rightarrow C$, $B \Rightarrow C$ sont des théorèmes de $\mathcal{T}$, alors $C$ est un théorème de $\mathcal{T}$.

En effet, d’après S4, $(A \text{ ou } B) \Rightarrow (A \text{ ou } C)$, et $(C \text{ ou } A) \Rightarrow (C \text{ ou } C)$ sont des théorèmes de $\mathcal{T}$. Compte tenu de S3 et S1, $(A \text{ ou } B) \Rightarrow C$ est un théorème de $\mathcal{T}$; d’où la règle.

Pour démontrer $C$, il suffit donc, quand on dispose d’un théorème « $A$ ou $B$ », de démontrer $C$ en adjoignant $A$ aux axiomes de $\mathcal{T}$, puis de démontrer $C$ en adjoignant $B$ aux axiomes de $\mathcal{T}$. L’intérêt de cette méthode provient du fait que, si « $A$ ou $B$ » est vraie, rien ne permet en général d’affirmer que l’une des relations $A$, $B$ soit vraie.

En particulier, d’après C10, si $A \Rightarrow C$, et $(\text{non } A) \Rightarrow C$, sont toutes deux des théorèmes de $\mathcal{T}$, $C$ est un théorème de $\mathcal{T}$.

IV. Méthode de la constante auxiliaire. — Elle repose sur la règle suivante:

C19. Soient $x$ une lettre, $A$ et $B$ des relations de $\mathcal{T}$ telles que:

1° La lettre $x$ n’est pas une constante de $\mathcal{T}$ et ne figure pas dans $B$.

2° On connaît un terme $T$ de $\mathcal{T}$ tel que $(T \mid x)A$ soit un théorème de $\mathcal{T}$.

Soit $\mathcal{T}'$ la théorie obtenue en adjoignant $A$ aux axiomes de $\mathcal{T}$. Si $B$ est un théorème de $\mathcal{T}'$, $B$ est un théorème de $\mathcal{T}$.

En effet, $A \Rightarrow B$ est un théorème de $\mathcal{T}$ (critère de la déduction). Puisque $x$ n’est pas une constante de $\mathcal{T}$, $(T \mid x)(A \Rightarrow B)$ est un théorème de $\mathcal{T}$ d’après C3. Comme $x$ ne figure pas dans $B$, $(T \mid x)(A \Rightarrow B)$ est identique, d’après CS5 (I, p. 17), à $((T \mid x)A) \Rightarrow B$. Enfin, $(T \mid x)A$ est un théorème de $\mathcal{T}$, donc aussi $B$.

Intuitivement, la méthode consiste à utiliser, pour démontrer $B$, un objet arbitraire $x$ (la constante auxiliaire) qu’on suppose doué de certaines propriétés qui sont

N° 4                                  THÉORIES LOGIQUES                                  E I.29

exprimées par A. \* Par exemple, dans une démonstration de géométrie où il s’agit, entre autres choses, d’une droite D, on peut « prendre » un point $x$ sur cette droite; la relation A est alors $x \in D$. \* Pour qu’on puisse se servir, au cours d’une démonstration, d’un objet doué de certaines propriétés, il faut évidemment qu’il existe de tels objets. Le théorème $(T \mid x)A$, dit théorème de légitimation, garantit cette existence.

En pratique, on indique qu’on va utiliser cette méthode par une phrase du genre suivant : « Soit $x$ un objet tel que A ». Contrairement à ce qui se passe dans la méthode de l’hypothèse auxiliaire, la conclusion du raisonnement ne concerne pas $x$.

### 4. La conjonction

Soient $A$, $B$ des assemblages. L’assemblage

$$
\text{non }((\text{non } A)\text{ ou }(\text{non } B))
$$

sera désigné par « $A$ et $B$ ».

CS6. Soient $A$, $B$, $T$ des assemblages, $x$ une lettre. L’assemblage $(T \mid x)(A \text{ et } B)$ est identique à « $(T \mid x)A$ et $(T \mid x)B$ ».

Ceci résulte aussitôt de CS5 (I, p. 17).

CF9. Si $A$, $B$ sont des relations de $\mathcal{T}$, « $A$ et $B$ » est une relation de $\mathcal{T}$ (appelée conjonction de $A$ et de $B$).

Ceci résulte aussitôt de CF1 et CF2 (I, p. 19).

C20. Si $A$, $B$ sont des théorèmes de $\mathcal{T}$, « $A$ et $B$ » est un théorème de $\mathcal{T}$.

Supposons « $A$ et $B$ » fausse, c’est-à-dire

$$
\text{non non }((\text{non } A)\text{ ou }(\text{non } B))
$$

vraie. D’après C16, « $(\text{non } A)$ ou $(\text{non } B)$ », c’est-à-dire $A \Rightarrow (\text{non } B)$, est vraie, donc « $\text{non } B$ » est vraie. Or, ceci est absurde. Donc « $A$ et $B$ » est vraie.

C21. Si $A$, $B$ sont des relations de $\mathcal{T}$, $(A \text{ et } B) \Rightarrow A$, $(A \text{ et } B) \Rightarrow B$ sont des théorèmes de $\mathcal{T}$.

En effet, les relations

$$
(\text{non } A) \Rightarrow ((\text{non } A)\text{ ou }(\text{non } B)),
$$

$$
(\text{non } B) \Rightarrow ((\text{non } A)\text{ ou }(\text{non } B))
$$

sont des théorèmes de $\mathcal{T}$ d’après S2 et C7. Or

$$
((\text{non } A)\text{ ou }(\text{non } B)) \Rightarrow \text{non }(A \text{ et } B)
$$

est un théorème de $\mathcal{T}$ d’après C11. Donc

$$
(\text{non } A) \Rightarrow \text{non}(A \text{ et } B),
$$

$$
(\text{non } B) \Rightarrow \text{non}(A \text{ et } B)
$$

sont des théorèmes de $\mathcal{T}$. On conclut par application de C17.

On convient de désigner par « $A$ et $B$ et $C$ » (resp. « $A$ ou $B$ ou $C$ ») la relation

« $A$ et $(B$ et $C)$ » (resp. « $A$ ou $(B$ ou $C$) »). Plus généralement, si on a des relations $A_1, A_2, \ldots, A_h$, on désigne par « $A_1$ et $A_2$ et ... et $A_h$ » une relation qui se construit de proche en proche par la convention que « $A_1$ et $A_2$ et ... et $A_h$ » désigne la même relation que « $A_1$ et $(A_2$ et ... et $A_h)$ ». On définit de même « $A_1$ ou $A_2$ ou ... ou $A_h$ ». La relation « $A_1$ et $A_2$ et ... et $A_h$ » est un théorème de $\mathcal{T}$ si et seulement si chacune des relations $A_1, A_2, \ldots, A_h$ est un théorème de $\mathcal{T}$.

Il en résulte que toute théorie logique $\mathcal{T}$ est équivalente à une théorie logique $\mathcal{T}'$ possédant au plus un axiome explicite. C'est évident si $\mathcal{T}$ ne possède aucun axiome explicite. Si $\mathcal{T}$ possède les axiomes expli $A_1, A_2, \ldots, A_h$, soit $\mathcal{T}'$ la théorie qui admet les mêmes signes et les mêmes schémas que $\mathcal{T}$, et l'axiome explicite « $A_1$ et $A_2$ et ... et $A_h$ ». On voit aussitôt que tout axiome de $\mathcal{T}$ (resp. $\mathcal{T}'$) est un théorème de $\mathcal{T}'$ (resp. $\mathcal{T}$).

Soit $\mathcal{T}_0$ la théorie sans axiome explicite qui admet les mêmes signes que $\mathcal{T}$ et les seuls schémas S1, S2, S3, S4. L'étude de $\mathcal{T}$ se ramène, en principe, à l'étude de $\mathcal{T}_0$ : pour que la relation $A$ soit un théorème de $\mathcal{T}$, il faut et il suffit qu'il y ait des axiomes $A_1, A_2, \ldots, A_h$ de $\mathcal{T}$ tels que $(A_1$ et $A_2$ et ... et $A_h) \Rightarrow A$ soit un théorème de $\mathcal{T}_0$. En effet, la condition est évidemment suffisante. Supposons d'autre part que $A$ soit un théorème de $\mathcal{T}$, et soient $A_1, A_2, \ldots, A_h$ les axiomes de $\mathcal{T}$ qui figurent dans une démonstration de $\mathcal{T}$ contenant $A$. Soit $\mathcal{T}'$ (resp. $\mathcal{T}''$) la théorie déduite de $\mathcal{T}_0$ par adjonction des axiomes $A_1, A_2, \ldots, A_h$ (resp. de l'axiome « $A_1$ et $A_2$ et ... et $A_h$ »). La démonstration de $A$ dans $\mathcal{T}$ est une démonstration de $A$ dans $\mathcal{T}'$, donc $A$ est un théorème de $\mathcal{T}'$ et par suite de $\mathcal{T}''$, puisqu'on a vu ci-dessus que $\mathcal{T}'$ et $\mathcal{T}''$ sont équivalentes. D'après le critère de la déduction,

$$(A_1 \text{ et } A_2 \text{ et } \ldots \text{ et } A_h) \Rightarrow A$$

est un théorème de $\mathcal{T}_0$.

Si $\mathcal{T}$ est contradictoire, il existe d'après ce qui précède une conjonction $A$ d'axiomes de $\mathcal{T}$ et une relation $R$ de $\mathcal{T}$ telles que $A \Rightarrow (R$ et (non $R$)) soit un théorème de $\mathcal{T}_0$. Donc

$$((\text{non }R) \text{ ou } (\text{non non }R)) \Rightarrow (\text{non }A)$$

est un théorème de $\mathcal{T}_0$, et comme « (non $R$) ou (non non $R$) » est un théorème de $\mathcal{T}_0$, « non $A$ » est un théorème de $\mathcal{T}_0$. Réciproquement, s'il existe une conjonction $A$ d'axiomes de $\mathcal{T}$ telle que « non $A$ » soit un théorème de $\mathcal{T}_0$, $A$ et « non $A$ » sont des théorèmes de $\mathcal{T}$, de sorte que $\mathcal{T}$ est contradictoire.

### 5. L'équivalence

Soient $A$ et $B$ des assemblages. L'assemblage

$$(A \Rightarrow B) \text{ et } (B \Rightarrow A)$$

sera désigné par $A \Leftrightarrow B$.

CS7. Soient $A, B, T$ des assemblages, $x$ une lettre. L'assemblage $(T|x)(A \Leftrightarrow B)$ est identique à $(T|x)A \Leftrightarrow (T|x)B$.

Ceci résulte aussitôt de CS5 (I, p. 17) et CS6 (I, p. 29).

CF10. Si $A$ et $B$ sont des relations de $\mathcal{T}$, $A \Leftrightarrow B$ est une relation de $\mathcal{T}$.

Ceci résulte aussitôt de CF5 (I, p. 19) et CF9 (I, p. 29).

Si $A \Leftrightarrow B$ est un théorème de $\mathcal{T}$, nous dirons que $A$ et $B$ sont équivalentes dans $\mathcal{T}$; si $x$ est une lettre qui n'est pas une constante de $\mathcal{T}$, et si $A$ et $B$ sont considérées comme relations en $x$, tout terme de $\mathcal{T}$ qui vérifie l'une vérifie aussi l'autre.

Il résulte des critères C20 et C21 que, pour démontrer dans $\mathcal{T}$ un théorème de la forme $A \Leftrightarrow B$, il faut et il suffit qu'on puisse démontrer $A \Rightarrow B$ et $B \Rightarrow A$ dans $\mathcal{T}$. Cela se fait souvent en démontrant $B$ dans la théorie déduite de $\mathcal{T}$ par adjonction de l'axiome $A$, puis en démontrant $A$ dans la théorie déduite de $\mathcal{T}$ par adjonction de l'axiome $B$. Ces remarques permettent d'établir aussitôt les critères suivants, dont nous laissons la démonstration au lecteur.

C22. Soient $A$, $B$, $C$ des relations de $\mathcal{T}$. Si $A \Leftrightarrow B$ est un théorème de $\mathcal{T}$, $B \Leftrightarrow A$ est un théorème de $\mathcal{T}$. Si $A \Leftrightarrow B$ et $B \Leftrightarrow C$ sont des théorèmes de $\mathcal{T}$, $A \Leftrightarrow C$ est un théorème de $\mathcal{T}$.

C23. Soient $A$ et $B$ des relations équivalentes dans $\mathcal{T}$, et $C$ une relation de $\mathcal{T}$. Alors, on a dans $\mathcal{T}$ les théorèmes suivants :

$$
(\mathrm{non}\ A) \Leftrightarrow (\mathrm{non}\ B) ;
\qquad
(A \Rightarrow C) \Leftrightarrow (B \Rightarrow C) ;
\qquad
(C \Rightarrow A) \Leftrightarrow (C \Rightarrow B) ;
$$

$$
(A \ \mathrm{et}\ C) \Leftrightarrow (B \ \mathrm{et}\ C) ;
\qquad
(A \ \mathrm{ou}\ C) \Leftrightarrow (B \ \mathrm{ou}\ C).
$$

C24. Soient $A$, $B$, $C$ des relations de $\mathcal{T}$; on a dans $\mathcal{T}$ les théorèmes suivants :

$$
(\mathrm{non}\ \mathrm{non}\ A) \Leftrightarrow A ;
\qquad
(A \Rightarrow B) \Leftrightarrow ((\mathrm{non}\ B) \Rightarrow (\mathrm{non}\ A)) ;
$$

$$
(A \ \mathrm{et}\ A) \Leftrightarrow A ;
\qquad
(A \ \mathrm{et}\ B) \Leftrightarrow (B \ \mathrm{et}\ A) ;
$$

$$
(A \ \mathrm{et}\ (B \ \mathrm{et}\ C)) \Leftrightarrow ((A \ \mathrm{et}\ B) \ \mathrm{et}\ C) ;
$$

$$
(A \ \mathrm{ou}\ B) \Leftrightarrow \mathrm{non}\ ((\mathrm{non}\ A) \ \mathrm{et}\ (\mathrm{non}\ B)) ;
$$

$$
(A \ \mathrm{ou}\ A) \Leftrightarrow A ;
\qquad
(A \ \mathrm{ou}\ B) \Leftrightarrow (B \ \mathrm{ou}\ A) ;
$$

$$
(A \ \mathrm{ou}\ (B \ \mathrm{ou}\ C)) \Leftrightarrow ((A \ \mathrm{ou}\ B) \ \mathrm{ou}\ C) ;
$$

$$
(A \ \mathrm{et}\ (B \ \mathrm{ou}\ C)) \Leftrightarrow ((A \ \mathrm{et}\ B) \ \mathrm{ou}\ (A \ \mathrm{et}\ C)) ;
$$

$$
(A \ \mathrm{ou}\ (B \ \mathrm{et}\ C)) \Leftrightarrow ((A \ \mathrm{ou}\ B) \ \mathrm{et}\ (A \ \mathrm{ou}\ C)) ;
$$

$$
(A \ \mathrm{et}\ (\mathrm{non}\ B)) \Leftrightarrow \mathrm{non}\ (A \Rightarrow B) ;
\qquad
(A \ \mathrm{ou}\ B) \Leftrightarrow ((\mathrm{non}\ A) \Rightarrow B).
$$

C25. Si $A$ est un théorème de $\mathcal{T}$ et $B$ une relation de $\mathcal{T}$, $(A \ \mathrm{et}\ B) \Leftrightarrow B$ est un théorème de $\mathcal{T}$. Si « $\mathrm{non}\ A$ » est un théorème de $\mathcal{T}$, $(A \ \mathrm{ou}\ B) \Leftrightarrow B$ est un théorème de $\mathcal{T}$.

En principe, dans tout le reste de ce Traité, les critères C1 à C25 seront désormais utilisés sans référence.

## EXERCICES {#ens-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).

[^1]: L’expression de ce schéma n’utilisant pas la lettre $A$ ni le symbole abréviateur $\Rightarrow$ est la suivante : *Lorsqu’on a une relation, on obtient un théorème en écrivant de gauche à droite $\vee$, $\neg$, $\vee$, puis trois fois de suite la relation donnée.* Le lecteur pourra s’exercer à traduire de même l’expression des autres schémas.
[^2]: Dans le langage courant, le mot « ou » peut avoir deux sens distincts suivant le contexte : lorsqu’on relie deux affirmations par le mot « ou », on peut vouloir affirmer, soit l’une au moins des deux (et éventuellement toutes les deux à la fois), soit l’une à l’exclusion de l’autre.
