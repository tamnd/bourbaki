---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THÉORIE DES ENSEMBLES
section: 4
section_title: Réunion et intersection d’une famille d’ensembles
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E II.50-E II.51
pdf_pages: 0074-0082, 0102-0103
extraction: ocr
subsections:
    - "no": 1
      title: Définition de la réunion et de l’intersection d’une famille d’ensembles
      page: 0
      pdf_page: 74
    - "no": 2
      title: Propriétés de la réunion et de l’intersection
      page: 0
      pdf_page: 76
    - "no": 3
      title: Images d’une réunion et d’une intersection
      page: 25
      pdf_page: 77
    - "no": 4
      title: Complémentaire d'une réunion ou d'une intersection
      page: 26
      pdf_page: 78
    - "no": 5
      title: Réunion et intersection de deux ensembles
      page: 26
      pdf_page: 78
    - "no": 6
      title: Recouvrements
      page: 27
      pdf_page: 79
    - "no": 7
      title: Partitions
      page: 29
      pdf_page: 81
    - "no": 8
      title: Somme d’une famille d’ensembles
      page: 29
      pdf_page: 81
statements: 22
exercises: 8
content_sha256: 2c0ff941f524dfb20cbf59d979331790b68181ef8729cc4e27073ec105cf244f
---

## § 4. RÉUNION ET INTERSECTION D’UNE FAMILLE D’ENSEMBLES

### 1. Définition de la réunion et de l’intersection d’une famille d’ensembles

Soient X une famille (II, p. 14), I son ensemble d’indices; pour faciliter l’interprétation intuitive de ce qui suit, nous dirons que X est une famille d’ensembles.

Si $(X, I, \mathscr{G})$ est une famille de parties d’un ensemble E (c’est-à-dire une famille d’éléments dont l’ensemble d’arrivée $\mathscr{G}$ est tel que la relation $Y \in \mathscr{G}$ entraîne $Y \subset E$), nous la noterons $(X_i)_{i\in I}$ ($X_i \in \mathscr{G}$), ou simplement $(X_i)_{i\in I}$ (II, p. 16); par abus de notation, nous noterons aussi $(X_i)_{i\in I}$ une famille d’ensembles quelconque, ayant I pour ensemble d’indices.

Comme la relation $(\forall x)((i \in I \text{ et } x \in X_i) \Rightarrow (x \in X))$ est vraie, il résulte de S5 (I, p. 33) que la relation

$$
(\forall x)(\exists Z)(\forall x)(((i \in I \text{ et } x \in X_i) \Rightarrow (x \in Z))
$$

est vraie. En vertu du schéma S8 (II, p. 4), la relation $(\exists i)(i \in I \text{ et } x \in X_i)$ est donc collectivisante en x.

#### Définition 1 {#ens-ii-s4-def-1 .statement tag=03I1}

Soit $(X_i)_{i\in I}$ une famille d’ensembles (resp. une famille de parties d’un ensemble E). On appelle réunion de cette famille, et on désigne par $\bigcup_{i\in I} X_i$, l’ensemble

$$
\{x \mid (\exists i)(i \in I \text{ et } x \in X_i)\},
$$

c’est-à-dire l’ensemble des x qui appartiennent à un ensemble au moins de la famille $(X_i)_{i\in I}$.

Si $(X_i)_{i\in I}$ est une famille de parties d’un ensemble E, sa réunion est une partie de E; on observera qu’elle ne dépend pas de E, ni de l’ensemble d’arrivée $\mathscr{G}$ de l’application $i \mapsto X_i$.

Il est immédiat que si $I = \varnothing$, on a $\bigcup_{i\in I} X_i = \varnothing$, puisque la relation $(\exists i)(i \in I \text{ et } x \in X_i)$ est alors fausse.

Supposons maintenant $I \neq \varnothing$. Si $\alpha$ est un élément de I, la relation $(\forall i)((i \in I) \Rightarrow (x \in X_i))$ entraîne $x \in X_\alpha$, donc, en vertu de C52 (II, p. 5), cette relation est collectivisante en x.

#### Définition 2 {#ens-ii-s4-def-2 .statement tag=03PT}

Soit $(X_i)_{i\in I}$ une famille d’ensembles dont l’ensemble d’indices I n’est pas vide. On appelle intersection de cette famille, et on désigne par $\bigcap_{i\in I} X_i$, l’ensemble

$$
\{x \mid (\forall i)((i \in I) \Rightarrow (x \in X_i))\},
$$

c’est-à-dire l’ensemble des x qui appartiennent à tous les ensembles de la famille $(X_i)_{i\in I}$.

Si $I = \varnothing$, la relation $(\forall i)((i \in I) \Rightarrow (x \in X_i))$ n’est pas collectivisante en x: en effet, c’est une relation vraie et il n’existe pas d’ensemble Y tel que $x \in Y$ soit une relation vraie, car ce serait l’ensemble de tous les objets (cf. II, p. 6, Remarque).

Si $(X_t)_{t \in I}$ est une famille de parties d’un ensemble $E$, et si $I \neq \varnothing$, la relation « $x \in E$ et $(\forall t)((t \in I) \Rightarrow (x \in X_t))$ » est équivalente à $(\forall t)((t \in I) \Rightarrow (x \in X_t))$; par suite elle est collectivisante en $x$ et l’ensemble des $x$ vérifiant cette relation est égal à $\bigcap_{t \in I} X_t$. Lorsque $I = \varnothing$, la relation « $x \in E$ et $(\forall t)((t \in I) \Rightarrow (x \in X_t))$ » est équivalente à $x \in E$; elle est donc encore collectivisante en $x$, et l’ensemble des $x$ vérifiant cette relation est $E$. On pose par suite la définition suivante:

#### Définition 3 {#ens-ii-s4-def-3 .statement tag=03PU}

Soit $(X_t)_{t \in I}$ une famille de parties d’un ensemble $E$. On appelle intersection de cette famille, et on désigne par $\bigcap_{t \in I} X_t$, l’ensemble
$$
\{x \mid x \in E \text{ et } (\forall t)((t \in I) \Rightarrow (x \in X_t))\},
$$
autrement dit l’ensemble des $x$ qui appartiennent à $E$ et à tous les ensembles de la famille $(X_t)_{t \in I}$.

Pour une famille $(X_t)_{t \in \varnothing}$ de parties de $E$, on a donc $\bigcap_{t \in \varnothing} X_t = E$. Mais pour une famille $(X_t)_{t \in I}$ de parties de $E$ dont l’ensemble d’indices n’est pas vide, l’intersection $\bigcap_{t \in I} X_t$ ne dépend ni de $E$, ni de l’ensemble d’arrivée de $t \mapsto X_t$, ce qui justifie l’emploi de la même notation dans les déf. 2 et 3.

#### Proposition 1 {#ens-ii-s4-prop-1 .statement tag=03PV}

Soit $(X_t)_{t \in I}$ une famille d’ensembles, et soit $f$ une application d’un ensemble $K$ sur $I$. On a alors $\bigcup_{\kappa \in K} X_{f(\kappa)} = \bigcup_{t \in I} X_t$, et, si $I \neq \varnothing$, $\bigcap_{\kappa \in K} X_{f(\kappa)} = \bigcap_{t \in I} X_t$.

Soit $x$ un élément de $\bigcup_{t \in I} X_t$. Il existe un indice $t \in I$ tel que $x \in X_t$. Puisque $f(K) = I$, il existe un indice $\kappa \in K$ tel que $t = f(\kappa)$, d’où $x \in X_{f(\kappa)}$, et par suite $x \in \bigcup_{\kappa \in K} X_{f(\kappa)}$. Réciproquement, si $x \in \bigcup_{\kappa \in K} X_{f(\kappa)}$, il existe un $\kappa \in K$ tel que $x \in X_{f(\kappa)}$, d’où, puisque $f(\kappa) \in I$, $x \in \bigcup_{t \in I} X_t$. On a donc $\bigcup_{\kappa \in K} X_{f(\kappa)} = \bigcup_{t \in I} X_t$.

Supposons maintenant $I \neq \varnothing$, et soit $x$ un élément de $\bigcap_{t \in I} X_t$. Pour tout élément $\kappa$ de $K$, on a $f(\kappa) \in I$, d’où $x \in X_{f(\kappa)}$ et $x \in \bigcap_{\kappa \in K} X_{f(\kappa)}$. Soit réciproquement $x$ un élément de $\bigcap_{\kappa \in K} X_{f(\kappa)}$. Si $t$ est un élément quelconque de $I$, il existe un élément $\kappa$ de $K$ tel que $t = f(\kappa)$, d’où $x \in X_t$, et par suite $x \in \bigcap_{t \in I} X_t$. On a donc $\bigcap_{\kappa \in K} X_{f(\kappa)} = \bigcap_{t \in I} X_t$.

Pour les familles de parties d’un ensemble donné, il est clair que la seconde partie de la prop. 1 est encore valable sans la restriction $I \neq \varnothing$.

#### Corollaire {#ens-ii-s4-n1-cor-1 .statement tag=03I2}

Soit $(X_t)_{t \in I}$ une famille d’ensembles telle que $X_t = X_\kappa$ pour tout couple d’indices $(t, \kappa)$. Alors, pour tout $\alpha \in I$, on a $\bigcup_{t \in I} X_t = X_\alpha$, et (si $I \neq \varnothing$) $\bigcap_{t \in I} X_t = X_\alpha$.

Il suffit d’appliquer la prop. 1 à l’application constante $t \mapsto \alpha$ de $I$ sur $\{\alpha\}$.

#### Définition 4 {#ens-ii-s4-def-4 .statement tag=03I3}

Soit $\mathcal{F}$ un ensemble d’ensembles, et soit $\Phi$ la famille d’ensembles

N° 2                                             RÉUNION ET INTERSECTION D’UNE FAMILLE D’ENSEMBLES                                             E II.24

constituée par l’application identique de $\mathscr{F}$. La réunion des ensembles de $\Phi$, et (si $\mathscr{F}$ est non vide) l’intersection des ensembles de $\Phi$, s’appellent respectivement la réunion et l’intersection des ensembles de $\mathscr{F}$, et se désignent par $\bigcup_{X\in\mathscr{F}}X$ et $\bigcap_{X\in\mathscr{F}}X$.

Il résulte tout de suite de la prop. 1 que, si $(X_t)_{t\in I}$ est une famille d’ensembles, la réunion et (si $I\neq\varnothing$) l’intersection de cette famille sont respectivement égales à la réunion et à l’intersection des ensembles de l’ensemble des éléments de cette famille.

### 2. Propriétés de la réunion et de l’intersection

Si $(X_t)_{t\in I}$ et $(Y_t)_{t\in I}$ sont des familles d’ensembles ayant le même ensemble d’indices $I$, et si on a $Y_t\subset X_t$ pour tout $t\in I$, il est immédiat que l’on a
$$
\bigcup_{t\in I}Y_t\subset\bigcup_{t\in I}X_t,
$$
et (si $I\neq\varnothing$)
$$
\bigcap_{t\in I}Y_t\subset\bigcap_{t\in I}X_t.
$$

Soit $(X_t)_{t\in I}$ une famille d’ensembles. Si $J\subset I$, on a
$$
\bigcup_{t\in J}X_t\subset\bigcup_{t\in I}X_t,
$$
et (si $J\neq\varnothing$)
$$
\bigcap_{t\in J}X_t\supset\bigcap_{t\in I}X_t.
$$

#### Proposition 2 {#ens-ii-s4-prop-2 .statement tag=03I4}

Soit $(X_t)_{t\in I}$ une famille d’ensembles dont l’ensemble d’indices $I$ est réunion d’une famille $(J_\lambda)_{\lambda\in L}$ d’ensembles. On a alors
$$
\bigcup_{t\in I}X_t=\bigcup_{\lambda\in L}\left(\bigcup_{t\in J_\lambda}X_t\right)
$$
et (si $L\neq\varnothing$ et $J_\lambda\neq\varnothing$ pour tout $\lambda\in L$)
$$
\bigcap_{t\in I}X_t=\bigcap_{\lambda\in L}\left(\bigcap_{t\in J_\lambda}X_t\right)
$$
(« associativité » de la réunion et de l’intersection).

Soit $x$ un élément de $\bigcup_{t\in I}X_t$. Il existe un indice $t\in I$ tel que $x\in X_t$. Puisque $I$ est la réunion de la famille $(J_\lambda)_{\lambda\in L}$, il existe un indice $\lambda\in L$ tel que $t\in J_\lambda$, d’où
$$
x\in\bigcup_{t\in J_\lambda}X_t,
$$
et par suite
$$
x\in\bigcup_{\lambda\in L}\left(\bigcup_{t\in J_\lambda}X_t\right).
$$
Soit inversement $x$ un élément de l’ensemble
$$
\bigcup_{\lambda\in L}\left(\bigcup_{t\in J_\lambda}X_t\right).
$$
Il existe un indice $\lambda\in L$ tel que
$$
x\in\bigcup_{t\in J_\lambda}X_t,
$$
d’où il résulte qu’il existe un indice $t\in J_\lambda$ (donc $t\in I$) tel que $x\in X_t$; on en conclut que
$$
x\in\bigcup_{t\in I}X_t.
$$

Supposons maintenant que $L\neq\varnothing$ et $J_\lambda\neq\varnothing$ pour tout $\lambda\in L$; alors $I\neq\varnothing$. Soit $x$ un élément de
$$
\bigcap_{t\in I}X_t.
$$
Si $\lambda\in L$, on a $x\in X_t$ pour tout $t\in J_\lambda$ (puisque $J_\lambda\subset I$), d’où
$$
x\in\bigcap_{t\in J_\lambda}X_t.
$$
Ceci étant vrai pour tout $\lambda\in L$, on en conclut que $x$ appartient à
$$
\bigcap_{\lambda\in L}\left(\bigcap_{t\in J_\lambda}X_t\right).
$$
Soit réciproquement $x$ un élément de ce dernier ensemble, et soit $t$ un élément quelconque de $I$. Il existe un $\lambda\in L$ tel que $t\in J_\lambda$; puisque
$$
x\in\bigcap_{t\in J_\lambda}X_t,
$$
on a $x\in X_t$. Ceci étant vrai pour tout $t\in I$, on a
$$
x\in\bigcap_{t\in I}X_t.
$$
La prop. 2 est donc démontrée.

Pour les familles de parties d’un ensemble, la seconde partie de la prop. 2 est encore valable sans les restrictions sur L et J_λ.

### 3. Images d’une réunion et d’une intersection

#### Proposition 3 {#ens-ii-s4-prop-3 .statement tag=03I5}

Soient (X_i)_{i \in I} une famille de parties d’un ensemble A, et Γ une correspondance entre A et B. On a alors $\Gamma \langle \bigcup_{i \in I} X_i \rangle = \bigcup_{i \in I} \Gamma \langle X_i \rangle$, et
$$
\Gamma \langle \bigcap_{i \in I} X_i \rangle \subset \bigcap_{i \in I} \Gamma \langle X_i \rangle.
$$
La relation $(\exists x)(x \in \bigcup_{i \in I} X_i \text{ et } y \in \Gamma(x))$ est équivalente à $(\exists x)(\exists i)(i \in I \text{ et } x \in X_i \text{ et } y \in \Gamma(x))$, donc à $(\exists i)(i \in I \text{ et } y \in \Gamma \langle X_i \rangle)$, c’est-à-dire à $y \in \bigcup_{i \in I} \Gamma \langle X_i \rangle$, ce qui démontre la première formule. D’autre part, pour tout $i \in I$, on a $\bigcap_{i \in I} X_i \subset X_i$, d’où (II, p. 10, prop. 2) $\Gamma \langle \bigcap_{i \in I} X_i \rangle \subset \Gamma \langle X_i \rangle$, et par suite
$$
\Gamma \langle \bigcap_{i \in I} X_i \rangle \subset \bigcap_{i \in I} \Gamma \langle X_i \rangle.
$$
Si Γ est une correspondance quelconque (et en particulier une fonction quelconque), la formule $\Gamma \langle \bigcap_{i \in I} X_i \rangle = \bigcap_{i \in I} \Gamma \langle X_i \rangle$ est en général fausse.

\* Par exemple, dans le plan $\mathbf{R}^2$, les premières projections des droites $y = x$ et $y = x + 1$ sont identiques à $\mathbf{R}$, mais l’intersection de ces droites est vide, et par suite aussi la première projection de cette intersection.¹ \*

On a cependant l’important résultat suivant:

#### Proposition 4 {#ens-ii-s4-prop-4 .statement tag=03I6}

Soient f une application de A dans B, et $(Y_i)_{i \in I}$ une famille de parties de B. On a alors $f^{-1} \langle \bigcap_{i \in I} Y_i \rangle = \bigcap_{i \in I} f^{-1} \langle Y_i \rangle$.

En effet, soit x un élément de $\bigcap_{i \in I} f^{-1} \langle Y_i \rangle$. On a $f(x) \in Y_i$ pour tout $i \in I$, d’où $f(x) \in \bigcap_{i \in I} Y_i$, et par suite $x \in f^{-1} \langle \bigcap_{i \in I} Y_i \rangle$. Donc $\bigcap_{i \in I} f^{-1} \langle Y_i \rangle \subset f^{-1} \langle \bigcap_{i \in I} Y_i \rangle$, ce qui, avec la prop. 3, achève la démonstration.

#### Corollaire {#ens-ii-s4-n3-cor-1 .statement tag=03I7}

Si f est une injection de A dans B et si $(X_i)_{i \in I}$ est une famille de parties de A dont l’ensemble d’indices n’est pas vide, on a $f \langle \bigcap_{i \in I} X_i \rangle = \bigcap_{i \in I} f \langle X_i \rangle$.

On peut en effet écrire $f = i \circ g$, où i est l’injection canonique de $f \langle A \rangle$ dans B et g une bijection de A sur $f \langle A \rangle$. Alors, pour toute partie X de A, on a $f \langle X \rangle = h^{-1} \langle X \rangle$, en désignant par h l’application réciproque de g; on est donc ramené à la prop. 4.

¹ Une erreur célèbre provenant de l’application de la formule précédente est celle commise par H. Lebesgue dans sa tentative pour démontrer que la projection sur un axe d’un ensemble borélien du plan est encore un ensemble borélien (résultat depuis reconnu inexact, et dont la discussion est à l’origine de la théorie des ensembles « sousliniens »): il écrit que la projection de l’intersection d’une suite décroissante d’ensembles est égale à l’intersection de leurs projections (Journal de Mathématiques, (6), t, I (1905), p. 191–192).

### 4. Complémentaire d'une réunion ou d'une intersection

#### Proposition 5 {#ens-ii-s4-prop-5 .statement tag=03I8}

Pour toute famille $(X_i)_{i \in I}$ de parties d'un ensemble $E$, on a

$$
\mathcal{C}_E(\bigcup_{i \in I} X_i) = \bigcap_{i \in I} (\mathcal{C}_E X_i) \quad \text{et} \quad \mathcal{C}_E(\bigcap_{i \in I} X_i) = \bigcup_{i \in I} (\mathcal{C}_E X_i).
$$

Soit $x \in \mathcal{C}_E(\bigcup_{i \in I} X_i)$. On a $x \in E$, et, pour tout $i \in I$, $x \notin X_i$, donc $x \in \mathcal{C}_E X_i$; par suite $x \in \bigcap_{i \in I} (\mathcal{C}_E X_i)$. Réciproquement, soit $x \in \bigcap_{i \in I} (\mathcal{C}_E X_i)$; par définition de l'intersection (II, p. 23, déf. 3), on a $x \in E$. En outre, si on avait $x \in \bigcup_{i \in I} X_i$, il existerait $\kappa \in I$ tel que $x \in X_\kappa$, ce qui est contraire à l'hypothèse $x \in \bigcap_{i \in I} (\mathcal{C}_E X_i)$; donc $x \in \mathcal{C}_E(\bigcup_{i \in I} X_i)$. Ceci achève la démonstration de la première formule. La seconde en résulte immédiatement, compte tenu de la relation $\mathcal{C}_E(\mathcal{C}_E X) = X$ pour toute partie $X$ de $E$.

### 5. Réunion et intersection de deux ensembles

Si $A$ et $B$ sont des ensembles, on pose

$$
A \cup B = \bigcup_{X \in \{A, B\}} X, \qquad A \cap B = \bigcap_{X \in \{A, B\}} X.
$$

Il est clair que $A \cup B$ est l'ensemble des objets qui appartiennent soit à $A$, soit à $B$ (et éventuellement à tous deux), tandis que $A \cap B$ est l'ensemble des objets qui appartiennent à la fois à $A$ et à $B$. En particulier $\{x, y\} = \{x\} \cup \{y\}$.

Posons $\{x, y, z\} = \{x, y\} \cup \{z\}$. L'ensemble $\{x, y, z\}$ est l'ensemble dont les seuls éléments sont $x, y$ et $z$. On pose de même $\{x, y, z, t\} = \{x, y, z\} \cup \{t\}$. Etc.

Si maintenant $A, B, C, D$ sont des ensembles, on pose

$$
A \cup B \cup C = \bigcup_{X \in \{A, B, C\}} X, \qquad A \cap B \cap C = \bigcap_{X \in \{A, B, C\}} X
$$
$$
A \cup B \cup C \cup D = \bigcup_{X \in \{A, B, C, D\}} X, \qquad A \cap B \cap C \cap D = \bigcap_{X \in \{A, B, C, D\}} X. \text{ Etc.}
$$

Soient $A, B, C$ des ensembles. Les prop. 1 et 2 entraînent les formules

$$
A \cup B = B \cup A, \qquad A \cap B = B \cap A
$$
$$
A \cup (B \cup C) = (A \cup B) \cup C = A \cup B \cup C
$$
$$
A \cap (B \cap C) = (A \cap B) \cap C = A \cap B \cap C.
$$

Ces formules sont d'ailleurs des conséquences immédiates de théorèmes énoncés dans le critère C24 (I, p. 31); on démontre de la même façon les formules

$$
A \cup (B \cap C) = (A \cup B) \cap (A \cup C), \qquad A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$

(« distributivité » de la réunion par rapport à l'intersection et de l'intersection par rapport à la réunion; cf. II, p. 35).

La relation $A \subset B$ est équivalente à $A \cup B = B$ et à $A \cap B = A$. Si $A$ et $B$ sont des parties d’un ensemble $E$, on déduit de la prop. 5 (ou du critère C24) les formules

$$
\mathcal{C}_E(A \cup B) = (\mathcal{C}_E A) \cap (\mathcal{C}_E B), \qquad \mathcal{C}_E(A \cap B) = (\mathcal{C}_E A) \cup (\mathcal{C}_E B);
$$

on a en outre

$$
A \cup (\mathcal{C}_E A) = E, \qquad A \cap (\mathcal{C}_E A) = \varnothing.
$$

Si $\Gamma$ est une correspondance entre $E$ et $F$, $A$ et $B$ des parties de $E$, on déduit de la prop. 3 (II, p. 25) que

$$
\Gamma \langle A \cup B \rangle = \Gamma \langle A \rangle \cup \Gamma \langle B \rangle, \qquad \Gamma \langle A \cap B \rangle \subset \Gamma \langle A \rangle \cap \Gamma \langle B \rangle
$$

et si $f$ est une application de $F$ dans $E$

$$
f^{-1} \langle A \cap B \rangle = f^{-1} \langle A \rangle \cap f^{-1} \langle B \rangle
$$

en vertu de la prop. 4.

Notons aussi la proposition correspondante pour les complémentaires:

#### Proposition 6 {#ens-ii-s4-prop-6 .statement tag=03PW}

*Soit $f$ une application de $A$ dans $B$; pour toute partie $Y$ de $B$, on a*

$$
f^{-1} \langle B - Y \rangle = f^{-1} \langle B \rangle - f^{-1} \langle Y \rangle.
$$

En effet, pour que $x$ appartienne à $f^{-1} \langle B - Y \rangle$, il faut et il suffit que $f(x)$ appartienne à $B$ mais non à $Y$, c’est-à-dire que $x$ appartienne à $f^{-1} \langle B \rangle$, mais non à $f^{-1} \langle Y \rangle$.

#### Corollaire {#ens-ii-s4-n5-cor-1 .statement tag=03PX}

*Soit $f$ une injection de $A$ dans $B$; pour toute partie $X$ de $A$, on a*

$$
f \langle A - X \rangle = f \langle A \rangle - f \langle X \rangle.
$$

En écrivant $f = i \circ g$, où $i$ est l’injection canonique de $f \langle A \rangle$ dans $B$, on se ramène à la prop. 6 appliquée à $g^{-1}$.

L’intersection $X \cap A$ s’appelle quelquefois *trace* de $X$ sur $A$. Si $\mathfrak{F}$ est une famille d’ensembles, on appelle encore *trace* de $\mathfrak{F}$ sur $A$ l’ensemble des traces sur $A$ des ensembles appartenant à $\mathfrak{F}$.

### 6. Recouvrements

#### Définition 5 {#ens-ii-s4-def-5 .statement tag=03PY}

*On dit qu’une famille d’ensembles $(X_i)_{i \in I}$ est un recouvrement d’un ensemble $E$ si $E \subset \bigcup_{i \in I} X_i$. Si $(X_i)_{i \in I}$ et $(Y_\kappa)_{\kappa \in K}$ sont des recouvrements de $E$, on dit que le second de ces recouvrements est plus fin que le premier (ou que le premier est moins fin que le second) si, pour tout $\kappa \in K$, il existe un $i \in I$ tel que $Y_\kappa \subset X_i$.*

Un ensemble d’ensembles $\mathfrak{F}$ est un recouvrement de $E$ si la famille d’ensembles constituée par l’application identique de $\mathfrak{F}$ est un recouvrement de $E$, autrement dit si $E \subset \bigcup_{X \in \mathfrak{F}} X$.

Si $\mathfrak{R}, \mathfrak{R}', \mathfrak{R}''$ sont trois recouvrements de $E$ tels que $\mathfrak{R}'$ soit plus fin que $\mathfrak{R}$, et $\mathfrak{R}''$ plus fin que $\mathfrak{R}'$, il est clair que $\mathfrak{R}''$ est plus fin que $\mathfrak{R}$.

Soit $(X_i)_{i \in I}$ un recouvrement de $E$; si $J$ est une partie de $I$ telle que $(X_i)_{i \in J}$ soit encore un recouvrement de $E$, ce recouvrement est évidemment plus fin que $(X_i)_{i \in I}$.

Soient $(X_i)_{i \in I}$ et $(Y_\kappa)_{\kappa \in K}$ des recouvrements d’un ensemble $E$. La famille d’ensembles $(X_i \cap Y_\kappa)_{(i, \kappa) \in I \times K}$ est encore un recouvrement de $E$. En effet, si $x \in E$, il existe des indices $i \in I$ et $\kappa \in K$ tels que $x \in X_i$ et $x \in Y_\kappa$, d’où $x \in X_i \cap Y_\kappa$. De plus, il est clair que le recouvrement $(X_i \cap Y_\kappa)_{(i, \kappa) \in I \times K}$ est plus fin que chacun des recouvrements $(X_i)_{i \in I}, (Y_\kappa)_{\kappa \in K}$. Soit réciproquement $(Z_\lambda)_{\lambda \in L}$ un recouvrement de $E$ qui est plus fin que chacun des recouvrements $(X_i)_{i \in I}$ et $(Y_\kappa)_{\kappa \in K}$; si $\lambda \in L$, il existe alors des indices $i \in I$ et $\kappa \in K$ tels que $Z_\lambda \subset X_i$ et $Z_\lambda \subset Y_\kappa$, d’où $Z_\lambda \subset X_i \cap Y_\kappa$, ce qui montre que le recouvrement $(Z_\lambda)_{\lambda \in L}$ est plus fin que le recouvrement $(X_i \cap Y_\kappa)_{(i, \kappa) \in I \times K}$.

Soit $(X_i)_{i \in I}$ un recouvrement d’un ensemble $A$, et soit $f$ une application de $A$ sur un ensemble $B$. La famille $(f \langle X_i \rangle)_{i \in I}$ est alors un recouvrement de $B$ (II, p. 25, prop. 3) qui s’appelle l’image du recouvrement $(X_i)_{i \in I}$ par $f$. Si $g$ est une application d’un ensemble $C$ dans l’ensemble $A$, la famille $(\overline{g}^{-1}\langle X_i \rangle)_{i \in I}$ est un recouvrement de $C$, qu’on appelle l’image réciproque du recouvrement $(X_i)_{i \in I}$ par $g$.

Soient $E$ et $F$ des ensembles, $(X_i)_{i \in I}$ un recouvrement de $E$ et $(Y_\kappa)_{\kappa \in K}$ un recouvrement de $F$. La famille $(X_i \times Y_\kappa)_{(i, \kappa) \in I \times K}$ est alors un recouvrement de $E \times F$ qu’on appelle le produit des recouvrements $(X_i)_{i \in I}$ de $E$ et $(Y_\kappa)_{\kappa \in K}$ de $F$.

#### Proposition 7 {#ens-ii-s4-prop-7 .statement tag=03PZ}

1° Soient $E$ un ensemble et $(X_i)_{i \in I}$ un recouvrement de $E$. Si deux fonctions $f, g$, ayant $E$ pour ensemble de définition, sont telles que, pour tout $i \in I$, $f$ et $g$ coïncident dans $E \cap X_i$, alors $f$ et $g$ coïncident dans $E$.

2° Soient $(X_i)_{i \in I}$ une famille d’ensembles, $(f_i)_{i \in I}$ une famille de fonctions ayant même ensemble d’arrivée $F$, telle que, pour tout $i \in I$, l’ensemble de définition de $f_i$ soit $X_i$, et que, pour tout couple $(i, \kappa) \in I \times I$, $f_i$ et $f_\kappa$ coïncident dans $X_i \cap X_\kappa$. Il existe alors une fonction $f$ et une seule, ayant $A = \bigcup_{i \in I} X_i$ pour ensemble de définition et $F$ pour ensemble d’arrivée, et qui prolonge toutes les fonctions $f_i$ ($i \in I$).

1° Soit $x$ un élément quelconque de $E$; il existe un $i \in I$ tel que $x \in X_i$, d’où $f(x) = g(x)$ par hypothèse.

2° Soit $G_i$ le graphe de $f_i$, et $G = \bigcup_{i \in I} G_i$; montrons que $G$ est un graphe fonctionnel. En effet, si $(x, y) \in G$ et $(x, y') \in G$, il existe deux indices $i, \kappa$ dans $I$ tels que $(x, y) \in G_i$ et $(x, y') \in G_\kappa$. Cela entraîne $x \in X_i, x \in X_\kappa, y = f_i(x), y' = f_\kappa(x)$; mais comme $x \in X_i \cap X_\kappa$, on a $f_i(x) = f_\kappa(x)$, c’est-à-dire $y = y'$. Le graphe $G$ a pour ensemble de définition $\operatorname{pr}_1 G = \bigcup_{i \in I} \operatorname{pr}_1 G_i = A$; la fonction $f = (G, A, F)$ répond donc à la question. Son unicité résulte de la première partie de la proposition.

### 7. Partitions

#### Définition 6 {#ens-ii-s4-def-6 .statement tag=03Q0}

On dit que deux ensembles $A, B$ sont disjoints (ou sans élément commun) si $A \cap B = \varnothing$; s’il n’en est pas ainsi, on dit que $A$ et $B$ se rencontrent. Soit $(X_i)_{i \in I}$ une famille d’ensembles; on dit que les ensembles de cette famille sont mutuellement (ou deux à deux) disjoints si les conditions $i \in I, \kappa \in I, i \neq \kappa$ entraînent $X_i \cap X_\kappa = \varnothing$.

Soit $f$ une application de $A$ dans $B$, $(Y_i)_{i \in I}$ une famille de parties de $B$, mutuellement disjointes; la prop. 4 (II, p. 25) montre que les ensembles de la famille $(f^{-1}(Y_i))_{i \in I}$ de parties de $A$ sont mutuellement disjoints. Par contre, si $(X_i)_{i \in I}$ est une famille de parties de $A$, mutuellement disjointes, les ensembles de la famille $(f(X_i))_{i \in I}$ ne sont pas en général mutuellement disjoints.

#### Proposition 8 {#ens-ii-s4-prop-8 .statement tag=03Q1}

Soient $(X_i)_{i \in I}$ une famille d’ensembles mutuellement disjoints, $(f_i)_{i \in I}$ une famille de fonctions ayant même ensemble d’arrivée $F$, et telles que, pour tout $i \in I$, l’ensemble de définition de $f_i$ soit $X_i$. Il existe alors une fonction $f$ et une seule, ayant $\bigcup_{i \in I} X_i$ pour ensemble de définition et $F$ pour ensemble d’arrivée, et qui prolonge toutes les fonctions $f_i$ ($i \in I$).

C’est un corollaire immédiat de la prop. 7 (II, p. 28), puisque $f_i$ et $f_\kappa$ coïncident évidemment dans $X_i \cap X_\kappa = \varnothing$ lorsque $i \neq \kappa$.

#### Définition 7 {#ens-ii-s4-def-7 .statement tag=03Q2}

On appelle partition d’un ensemble $E$ une famille de parties mutuellement disjointes de $E$, qui est un recouvrement de $E$.

#### Exemple {#ens-ii-s4-n7-exa-1 .statement tag=03I9}

Pour tout ensemble non vide $A$, la famille $(\{x\})_{x \in A}$ des parties de $A$ réduites à un seul élément est une partition de $A$.

Si $(X_i)_{i \in I}$ est une partition d’un ensemble $E$ formée d’ensembles non vides, l’application $i \mapsto X_i$ de $I$ sur l’ensemble $\mathfrak{F}$ des éléments $X_i$ de la partition est bijective. La donnée de $\mathfrak{F}$ définit donc la partition à une bijection près des ensembles d’indices. Lorsqu’on parle d’une partition en ensembles non vides, c’est de l’ensemble des éléments de la partition qu’il est question le plus souvent.

### 8. Somme d’une famille d’ensembles

#### Proposition 9 {#ens-ii-s4-prop-9 .statement tag=03Q3}

Soit $(X_i)_{i \in I}$ une famille d’ensembles. Il existe un ensemble $X$ possédant la propriété suivante : $X$ est réunion d’une famille $(X'_i)_{i \in I}$ d’ensembles mutuellement disjoints, telle que, pour tout $i \in I$, il existe une application bijective de $X_i$ sur $X'_i$.

Soit $A = \bigcup_{i \in I} X_i$. Si $i \in I$, l’application $x \mapsto (x, i)$ ($x \in X_i$) est une application bijective de $X_i$ sur une partie $X'_i$ de $A \times I$. De plus, l’image de $X'_i$ par la seconde fonction coordonnée sur $A \times I$ est contenue dans l’ensemble $\{i\}$; il en résulte que $X'_i \cap X'_\kappa = \varnothing$ si $i \neq \kappa$. Il suffit alors de poser $X = \bigcup_{i \in I} X'_i$.

#### Définition 8 {#ens-ii-s4-def-8 .statement tag=03Q4}

Soit $(X_i)_{i \in I}$ une famille d’ensembles. On appelle somme de cette famille d’ensembles la réunion de la famille des ensembles $X_i \times \{i\} (i \in I)$.

#### Proposition 10 {#ens-ii-s4-prop-10 .statement tag=03IA}

Soit $(X_i)_{i \in I}$ une famille d’ensembles mutuellement disjoints. Soient $A$ sa réunion et $S$ sa somme. Il existe une application bijective de $A$ sur $S$.

Pour tout $i \in I$, soit $f_i$ une bijection de $X_i$ sur $X_i \times \{i\}$. En vertu de la prop. 8 (II, p. 29), il existe une application $f$ de $A$ dans $S$ qui prolonge toutes les applications $f_k$. On vérifie aussitôt que $f$ est une application bijective de $A$ sur $S$.

Par abus de langage, on dit qu’un ensemble $E$ est somme d’une famille d’ensembles $(X_i)_{i \in I}$ lorsqu’il existe une bijection de $E$ sur la somme de cette famille définie par la déf. 8.

On notera que, si $(X_i)_{i \in I}$ est une famille d’ensembles quelconque, le raisonnement de la prop. 10 montre qu’il existe une application de la somme $S$ de cette famille sur sa réunion $A$.

On dit encore qu’un ensemble somme d’un ensemble $X$ et d’un ensemble $\{a\}$ réduit à un élément est obtenu par adjonction de $a$ à $X$.

## EXERCICES {#ens-ii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
