---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: Idéaux premiers associés et décomposition primaire
section: 1
section_title: Idéaux premiers associés à un module
lang: fr
source: ac-i-iv-fr
pdf_pages: 0305-0313, 0337-0341
extraction: ocr
subsections:
    - "no": 1
      title: Définition des idéaux premiers associés.
      page: 0
      pdf_page: 305
    - "no": 2
      title: Localisation des idéaux premiers associés.
      page: 0
      pdf_page: 308
    - "no": 3
      title: Relations avec le support.
      page: 0
      pdf_page: 309
    - "no": 4
      title: Cas des modules de type fini sur un anneau nœthérien.
      page: 0
      pdf_page: 310
statements: 24
exercises: 19
content_sha256: 12e3449cdea5d289e622c60a35c5b01f157790d8830cb1e8b0cf0903b1563fde
---

## § 1. Idéaux premiers associés à un module.

### 1. Définition des idéaux premiers associés.

#### Définition 1 {#ac-iv-s1-def-1 .statement}

Soit M un module sur un anneau A. On dit qu’un idéal premier $p$ de A est associé à M s’il existe $x \in M$ tel que $p$ soit égal à l’annulateur de x. On note $\mathrm{Ass}_A(M)$, ou simplement $\mathrm{Ass}(M)$, l’ensemble des idéaux premiers associés à M.

*Exemple. — Soient $a$ un idéal de l’anneau de polynômes $A = \mathbf{C}[X_1, ..., X_r]$, V la variété algébrique affine correspondante, $V_1, ..., V_p$ les composantes irréductibles de V. Si on prend pour M l’anneau $A/a$ des fonctions régulières sur V, les idéaux de $V_1, ..., V_p$ sont des idéaux premiers associés à M mais ce ne sont pas les seuls en général.*

(*) Les résultats de ce chapitre ne dépendent d’aucun autre Livre de la deuxième partie, ni du chap. I, § 4 ou du chap. III, § 5.

Comme l’annulateur de 0 est A, un élément $x \in M$ dont l’annulateur est un idéal premier est nécessairement $\neq 0$. Dire qu’un idéal premier $p$ est associé à $M$ revient à dire que $M$ contient un sous-module *isomorphe à* $A/p$ (savoir $Ax$, pour tout $x \in M$ dont $p$ est l’annulateur).

Si un A-module $M$ est réunion d’une famille $(M_i)_{i \in I}$ de sous-modules il est clair que l’on a

$$
\text{Ass}(M) = \bigcup_{i \in I} \text{Ass}(M_i).
$$

#### Proposition 1 {#ac-iv-s1-prop-1 .statement}

*Pour tout idéal premier $p$ d’un anneau $A$ et tout sous-module $M \neq 0$ de $A/p$, on a* $\text{Ass}(M) = \{ p \}$.

En effet, comme l’anneau $A/p$ est intègre, l’annulateur d’un élément $\neq 0$ de $A/p$ est $p$.

#### Proposition 2 {#ac-iv-s1-prop-2 .statement}

*Soit $M$ un module sur un anneau $A$. Tout élément maximal de l’ensemble des idéaux $\text{Ann}(x)$ de $A$, où $x$ parcourt l’ensemble des éléments $\neq 0$ de $M$, appartient à $\text{Ass}(M)$*.

En effet, soit $a = \text{Ann}(x)$ ($x \in M,\ x \neq 0$) un tel élément maximal ; il suffit de montrer que $a$ est premier. Comme $x \neq 0$, on a $a \neq A$. Soient $b,\ c$ des éléments de $A$ tels que $bc \in a$ et $c \notin a$. On a alors $cx \neq 0,\ b \in \text{Ann}(cx)$ et $a \subset \text{Ann}(cx)$. Comme $a$ est maximal, on a $\text{Ann}(cx) = a$, d’où $b \in a$, de sorte que $a$ est premier.

#### Corollaire 1 {#ac-iv-s1-prop-2-cor-1 .statement}

*Soit $M$ un module sur un anneau noethérien $A$. Alors la condition $M \neq \{ 0 \}$ équivaut à $\text{Ass}(M) \neq \varnothing$*.

Si $M = \{ 0 \}$, il est clair que $\text{Ass}(M)$ est vide (sans hypothèse sur $A$). Si $M \neq \{ 0 \}$, l’ensemble des idéaux de la forme $\text{Ann}(x)$, où $x \in M$ et $x \neq 0$, est non vide et formé d’idéaux $\neq A$ ; comme $A$ est noethérien, cet ensemble admet un élément maximal ; il suffit donc d’appliquer la prop. 2.

#### Corollaire 2 {#ac-iv-s1-prop-2-cor-2 .statement}

*Soient $A$ un anneau noethérien, $M$ un $A$-module, $a$ un élément de $A$. Pour que l’homothétie de $M$, de rapport $a$, soit injective , il faut et il suffit que $a$ n’appartienne à aucun idéal premier associé à $M$.*

Si $a$ appartient à un idéal premier $p \in \mathrm{Ass}(M)$, on a $p = \mathrm{Ann}(x)$ avec $x \in M, x \neq 0$; d’où $ax = 0$ et l’homothétie de rapport $a$ n’est pas injective. Réciproquement, si $ax = 0$ pour un $x \in M$ tel que $x \neq 0$, on a $Ax \neq \{0\}$, d’où $\mathrm{Ass}(Ax) \neq \emptyset$ (cor. 1). Soit $p \in \mathrm{Ass}(Ax)$; on a évidemment $p \in \mathrm{Ass}(M)$ et $p = \mathrm{Ann}(bx)$ avec $b \in A$; d’où $a \in p$, puisque $abx = 0$.

#### Corollaire 3 {#ac-iv-s1-prop-2-cor-3 .statement}

L’ensemble des diviseurs de zéro dans un anneau noethérien $A$ est la réunion des idéaux $p \in \mathrm{Ass}(A)$.

#### Proposition 3 {#ac-iv-s1-prop-3 .statement}

Soient $A$ un anneau, $M$ un $A$-module, $N$ un sous-module de $M$. On a

(2)
$$
\mathrm{Ass}(N) \subset \mathrm{Ass}(M) \subset \mathrm{Ass}(N) \cup \mathrm{Ass}(M/N).
$$

L’inclusion $\mathrm{Ass}(N) \subset \mathrm{Ass}(M)$ est évidente. Soient $p \in \mathrm{Ass}(M)$, $E$ un sous-module de $M$ isomorphe à $A/p$, et $F = E \cap N$. Si $F = \{0\}$, $E$ est isomorphe à un sous-module de $M/N$, d’où $p \in \mathrm{Ass}(M/N)$. Si $F \neq \{0\}$, l’annulateur de tout élément $\neq 0$ de $F$ est $p$ (prop. 1), donc $p \in \mathrm{Ass}(F) \subset \mathrm{Ass}(N)$.

#### Corollaire 1 {#ac-iv-s1-prop-3-cor-1 .statement}

Si un $A$-module $M$ est somme directe d’une famille $(M_i)_{i \in I}$ de sous-modules, on a $\mathrm{Ass}(M) = \bigcup_{i \in I} \mathrm{Ass}(M_i)$.

On se ramène au cas où $I$ est fini au moyen de (1), puis au cas où $\mathrm{Card}(I) = 2$ en procédant par récurrence sur $\mathrm{Card}(I)$. Soit alors $I = \{i, j\}, i \neq j$; comme $M/M_i$ est isomorphe à $M_j$, on a $\mathrm{Ass}(M) \subset \mathrm{Ass}(M_i) \cup \mathrm{Ass}(M_j)$ (prop. 3) ; par ailleurs, $\mathrm{Ass}(M_i)$ et $\mathrm{Ass}(M_j)$ sont contenus dans $\mathrm{Ass}(M)$ (prop. 3), d’où le résultat.

#### Corollaire 2 {#ac-iv-s1-prop-3-cor-2 .statement}

Soient $M$ un $A$-module, $(Q_i)_{i \in I}$ une famille finie de sous-modules de $M$. Si $\bigcap_{i \in I} Q_i = \{0\}$, on a
$$
\mathrm{Ass}(M) \subset \bigcup_{i \in I} \mathrm{Ass}(M/Q_i).
$$
En effet, l’application canonique $M \to \bigoplus_{i \in I} (M/Q_i)$ est injective ; il suffit donc d’appliquer la prop. 3 et son cor. 1.

#### Proposition 4 {#ac-iv-s1-prop-4 .statement}

Soient M un A-module, Φ une partie de Ass(M). Il existe alors un sous-module N de M tel que Ass(N) = Ass(M) − Φ et Ass(M/N) = Φ.

Soit E l’ensemble des sous-modules P de M tels que Ass(P) ⊂ Ass(M) − Φ. La formule (1) montre que l’ensemble E, ordonné par inclusion, est inductif ; en outre, on a {0} ∈ E, donc E ≠ ∅. Soit N un élément maximal de E. On a donc Ass(N) ⊂ Ass(M) − Φ. Nous allons voir que Ass(M/N) ⊂ Φ, ce qui, en vertu de la prop. 3, achèvera la démonstration. Soit p ∈ Ass(M/N) ; alors M/N contient un sous-module F/N isomorphe à A/p. En vertu des prop. 1 et 3, on a Ass(F) ⊂ Ass(N) ∪ {p}. Puisque N est maximal dans E, on a F ∈ E, donc p ∈ Φ.

### 2. Localisation des idéaux premiers associés.

#### Proposition 5 {#ac-iv-s1-prop-5 .statement}

Soient A un anneau, S une partie multiplicative de A, Φ l’ensemble des idéaux premiers de A qui ne rencontrent pas S, M un A-module. Alors :

(i) L’application p → S^{-1}p est une bijection de Ass_A(M) ∩ Φ sur une partie de Ass_{S^{-1}A}(S^{-1}M).

(ii) Si p ∈ Φ est un idéal de type fini et si S^{-1}p ∈ Ass_{S^{-1}A}(S^{-1}M), alors on a p ∈ Ass_A(M).

Rappelons (chap. II, § 2, n° 5, prop. 11) que l’application p → S^{-1}p est une bijection de Φ sur l’ensemble des idéaux premiers de S^{-1}A. Si p ∈ Ass_A(M) ∩ Φ, p est l’annulateur d’un sous-module monogène N de M ; alors S^{-1}p est l’annulateur du sous-module monogène S^{-1}N de S^{-1}M (chap. II, § 2, n° 4, formule (9)), donc S^{-1}p ∈ Ass_{S^{-1}A}(S^{-1}M). Réciproquement, supposons p ∈ Φ de type fini et tel que S^{-1}p soit associé à S^{-1}M ; il existe alors x ∈ M et t ∈ S tels que S^{-1}p soit l’annulateur de x/t. Soit (a_i)_{1 \leq i \leq n} un système de générateurs de p ; on a (a_i/1)(x/t) = 0, donc il existe s_i ∈ S tel que s_i a_i x = 0 (1 \leq i \leq n). Posons s = s_1 s_2 ... s_n ; pour tout a ∈ p, on a sax = 0, d’où p ⊂ Ann(sx) ; d’autre part, si b ∈ A est tel que bsx = 0, on a b/1 ∈ S^{-1}p par définition, d’où b ∈ p. Donc p = Ann(sx) et p ∈ Ass_A(M).

#### Corollaire {#ac-iv-s1-n2-cor-1 .statement}

Si l’anneau $\mathbf{A}$ est noethérien, l’application $p \to S^{-1}p$ est une bijection de $\mathrm{Ass}_\mathbf{A}(M) \cap \Phi$ sur $\mathrm{Ass}_{S^{-1}\mathbf{A}}(S^{-1}M)$.

Lorsque $\mathbf{A}$ n’est pas noethérien, l’application $p \to S^{-1}p$ de $\mathrm{Ass}_\mathbf{A}(M) \cap \Phi$ dans $\mathrm{Ass}_{S^{-1}\mathbf{A}}(S^{-1}M)$ n’est pas nécessairement surjective (exerc. 1).

#### Proposition 6 {#ac-iv-s1-prop-6 .statement}

Soient $\mathbf{A}$ un anneau noethérien, $M$ un $\mathbf{A}$-module, $S$ une partie multiplicative de $\mathbf{A}$, et $\Psi$ l’ensemble des éléments de $\mathrm{Ass}_\mathbf{A}(M)$ qui ne rencontrent pas $S$. Alors le noyau $N$ de l’application canonique $M \to S^{-1}M$ est l’unique sous-module de $M$ qui vérifie les relations

$$
\mathrm{Ass}(N) = \mathrm{Ass}(M) - \Psi, \qquad \mathrm{Ass}(M/N) = \Psi.
$$

En vertu de la prop. 4 du n° 1, il existe un sous-module $N'$ de $M$ qui vérifie les relations $\mathrm{Ass}(N') = \mathrm{Ass}(M) - \Psi'$ et $\mathrm{Ass}(M/N') = \Psi'$. Il s’agit de prouver que $N' = N$. Considérons le diagramme commutatif

$$
\begin{array}{ccc}
M & \xrightarrow{p} & M/N' \\
u \downarrow & & \downarrow v \\
S^{-1}M & \xrightarrow{S^{-1}p} & S^{-1}(M/N')
\end{array}
$$

où $p, u, v$ sont les homomorphismes canoniques. Nous allons montrer que $S^{-1}p$ et $v$ sont injectifs, ce qui prouvera que $u$ et $p$ ont même noyau, donc que $N' = N$.

Comme $\mathrm{Ass}(N') \cap \Psi' = \emptyset$, tout élément de $\mathrm{Ass}(N')$ rencontre $S$. On a donc $\mathrm{Ass}_{S^{-1}\mathbf{A}}(S^{-1}N') = \emptyset$ (cor. de la prop. 5), d’où $S^{-1}N' = \{ 0 \}$ (n° 1, cor. 1 de la prop. 2), ce qui prouve que $S^{-1}p$ est injectif (chap. II, § 2, n° 4, th. 1). D’autre part, si $x$ appartient au noyau $K$ de $v$, on a $\mathrm{Ann}(x) \cap S \neq \emptyset$ (chap. II, § 2, n° 2, prop. 4); donc $\mathrm{Ass}(K) = \emptyset$ puisque $\mathrm{Ass}(K) \subset \mathrm{Ass}(M/N') = \Psi'$; on en déduit $K = \{ 0 \}$ (n° 1, cor. 1 de la prop. 2) et $v$ est injectif.

### 3. Relations avec le support.

Soit $M$ un module sur un anneau $\mathbf{A}$. Rappelons qu’on appelle support de $M$ et qu’on note $\mathrm{Supp}(M)$ l’ensemble des idéaux premiers $p$ de $\mathbf{A}$ tels que $M_p \neq 0$ (chap. II, § 4, n° 4, déf. 5).

#### Proposition 7 {#ac-iv-s1-prop-7 .statement}

Soient $A$ un anneau, $M$ un $A$-module.

(i) Tout idéal premier $p$ de $A$ contenant un élément de $\mathrm{Ass}(M)$ appartient à $\mathrm{Supp}(M)$.

(ii) Inversement, si $A$ est nœthérien, tout idéal $p \in \mathrm{Supp}(M)$ contient un élément de $\mathrm{Ass}(M)$.

Si $p$ contient un élément $q$ de $\mathrm{Ass}(M)$, on a $q \cap (A - p) = \varnothing$, donc si on pose $S = A - p$, $S^{-1}q$ est un idéal premier associé à $S^{-1}M = M_p$ (no 2, prop. 5), et $a fortiori$ $M_p \neq 0$, donc $p \in \mathrm{Supp}(M)$. Inversement, si $A$ est nœthérien, il en est de même de $A_p$ (chap. II, § 2, no 6, cor. 2 de la prop. 10). Si $M_p \neq 0$, on a donc $\mathrm{Ass}_{A_p}(M_p) \neq \varnothing$ (no 1, cor. 1 de la prop. 2) donc il existe $q \in \mathrm{Ass}_A(M)$ tel que $q \cap (A - p) = \varnothing$ (no 2, cor. de la prop. 5).

#### Corollaire 1 {#ac-iv-s1-prop-7-cor-1 .statement}

Si $M$ est un module sur un anneau nœthérien, on a $\mathrm{Ass}(M) \subset \mathrm{Supp}(M)$, et ces deux ensembles ont mêmes éléments minimaux.

#### Corollaire 2 {#ac-iv-s1-prop-7-cor-2 .statement}

Le nilradical d’un anneau nœthérien $A$ est l’intersection des idéaux $p \in \mathrm{Ass}(A)$.

On sait en effet que le nilradical de $A$ est l’intersection des éléments minimaux de $\mathrm{Spec}(A) = \mathrm{Supp}(A)$ (chap. II, § 2, no 6, prop. 13).

### 4. Cas des modules de type fini sur un anneau nœthérien.

#### Théorème 1 {#ac-iv-s1-thm-1 .statement}

Soient $A$ un anneau nœthérien, $M$ un $A$-module de type fini. Il existe une suite de composition $(M_i)_{0 \leq i \leq n}$ de $M$ telle que, pour $0 \leq i \leq n - 1$, $M_i / M_{i+1}$ soit isomorphe à $A / p_i$, où $p_i$ est un idéal premier de $A$.

Soit en effet $\mathcal{E}$ l’ensemble des sous-modules de $M$ qui possèdent une suite de composition ayant la propriété de l’énoncé. Comme $\mathcal{E}$ est non vide (car $\{0\}$ appartient à $\mathcal{E}$) et comme $M$ est nœthérien, $\mathcal{E}$ possède un élément maximal $N$. Si $M \neq N$, on a $M/N \neq 0$, donc $\mathrm{Ass}(M/N) \neq \varnothing$ (no 1, cor. 1 de la prop. 2); $M/N$ contient donc un sous-module $N'/N$ isomorphe à un $A$-module de la forme $A/p$, où $p$ est premier; on a alors par définition $N' \in \mathcal{E}$, ce qui contredit le caractère maximal de $N$. Par suite, on a nécessairement $N = M$.

C. Q. F. D.

#### Théorème 2 {#ac-iv-s1-thm-2 .statement}

Soient $M$ un module de type fini sur un anneau noethérien $A$, et $(M_i)_{0 \leq i \leq n}$ une suite de composition de $M$ telle que, pour $0 \leq i \leq n - 1$, $M_i / M_{i+1}$ soit isomorphe à $A / p_i$, où $p_i$ est un idéal premier de $A$. On a alors

$$
\text{Ass}(M) \subset \{ p_0, \ldots, p_{n-1} \} \subset \text{Supp}(M);
$$

les éléments minimaux de ces trois ensembles sont les mêmes, et coïncident avec les éléments minimaux de l’ensemble des idéaux premiers contenant $\text{Ann}(M)$.

L’inclusion $\text{Ass}(M) \subset \{ p_0, \ldots, p_{n-1} \}$ résulte aussitôt des prop. 1 et 3 du no 1. Pour $0 \leq i \leq n - 1$, on a

$$
p_i \in \text{Supp}(A/p_i) = \text{Supp}(M_i/M_{i+1})
$$

(chap. II, § 4, no 4, Exemple), d’où $p_i \in \text{Supp}(M_i) \subset \text{Supp}(M)$ (chap. II, § 4, no 4, prop. 16), ce qui démontre l’inclusion $\{ p_0, \ldots, p_{n-1} \} \subset \text{Supp}(M)$. Le cor. 1 de la prop. 7 du no 3 montre que $\text{Ass}(M)$ et $\text{Supp}(M)$ ont les mêmes éléments minimaux, et (4) montre que ceux-ci ne sont autres que les éléments minimaux de $\{ p_0, \ldots, p_{n-1} \}$. La dernière assertion résulte alors du chap. II, § 4, no 4, prop. 17.

#### Corollaire {#ac-iv-s1-n4-cor-1 .statement}

Si $M$ est un module de type fini sur un anneau noethérien $A$, $\text{Ass}(M)$ est fini.

Sous les conditions du th. 2, l’ensemble $\{ p_0, \ldots, p_{n-1} \}$ n’est pas nécessairement déterminé de façon unique par $M$; en particulier il peut être distinct de $\text{Ass}(M)$ (exerc. 6).

#### Proposition 8 {#ac-iv-s1-prop-8 .statement}

Soient $A$ un anneau noethérien, $a$ un idéal de $A$, $M$ un $A$-module de type fini. Les conditions suivantes sont équivalentes :

a) il existe un élément $x \neq 0$ de $M$ tel que $ax = 0$;

b) pour tout $a \in a$, il existe un élément $x \neq 0$ de $M$ tel que $ax = 0$;

c) il existe $p \in \text{Ass}(M)$ tel que $a \subset p$.

Il est clair que a) implique b). En vertu du no 1, cor. 2 de la prop. 2, la condition b) signifie que l’idéal $a$ est contenu dans la réunion des idéaux premiers associés à $M$, donc dans l’un d’eux puisque Ass(M) est fini (chap. II, § 1, n° 1, prop. 2) ; ainsi b) entraîne c). Enfin, s’il existe $p \in \mathrm{Ass}(M)$ tel que $a \subset p$, $p$ est l’annulateur d’un élément $x \neq 0$ de $M$ (n° 1, déf. 1), et on a $ax = 0$; donc c) implique a).

#### Proposition 9 {#ac-iv-s1-prop-9 .statement}

*Soient A un anneau noethérien, a un idéal de A, M un A-module de type fini. Pour qu’il existe un entier $n > 0$ tel que $a^n M = 0$, il faut et il suffit que a soit contenu dans l’intersection des idéaux premiers associés à M.*

En effet, cette intersection est aussi celle des éléments minimaux de Supp(M) (n° 3, cor. 1 de la prop. 7), et dire que a est contenu dans cette intersection équivaut à dire que $V(a) \supset \mathrm{Supp}(M)$ avec les notations du chap. II, § 4 ; la conclusion résulte alors du chap. II, § 4, n° 4, cor. 2 de la prop. 17.

#### Définition 2 {#ac-iv-s1-def-2 .statement}

*Étant donné un A-module M, on dit qu’un endomorphisme u de M est presque nilpotent si, pour tout $x \in M$, il existe un entier $n(x) > 0$ tel que $u^{n(x)}(x) = 0$.*

Si M est de type fini, tout endomorphisme presque nilpotent est nilpotent.

#### Corollaire {#ac-iv-s1-n4-cor-2 .statement}

*Soient A un anneau noethérien, M un A-module, a un élément de A. Pour que l’homomorphisme $a_M : x \to ax$ de M soit presque nilpotent, il faut et il suffit que a appartienne à tout idéal de Ass(M).*

En effet, la condition de l’énoncé équivaut à dire que pour tout $x \in M$, il existe $n(x) > 0$ tel que $(Aa)^{n(x)}(Ax) = 0$ ; en vertu de la prop. 9, cela signifie encore que a appartient à tous les idéaux premiers associés au sous-module $Ax$ de $M$ ; le corollaire résulte donc de ce que Ass(M) est la réunion des Ass(Ax) lorsque $x$ parcourt M (n° 1, formule (1)).

#### Proposition 10 {#ac-iv-s1-prop-10 .statement}

*Soient A un anneau noethérien, E un A-module de type fini, F un A-module. On a alors*

$$
\mathrm{Ass}(\mathrm{Hom}_A(E, F)) = \mathrm{Ass}(F) \cap \mathrm{Supp}(E).
$$

Par hypothèse, E est isomorphe à un A-module de la forme $A^n / R$, donc $\mathrm{Hom}_A(E, F)$ est isomorphe à un sous-module de $\mathrm{Hom}_A(A^n, F)$, et ce dernier est isomorphe à $F^n$; or, on a $\mathrm{Ass}(F^n) = \mathrm{Ass}(F)$ (n° 1, cor. 1 de la prop. 3); donc $\mathrm{Ass}(\mathrm{Hom}_A(E, F)) \subset \mathrm{Ass}(F)$. D'autre part, on a $\mathrm{Supp}(\mathrm{Hom}_A(E, F)) \subset \mathrm{Supp}(E)$: en effet, pour tout idéal premier $p$ de $A$, $\mathrm{Hom}_{A_p}(E_p, F_p)$ est isomorphe à $(\mathrm{Hom}_A(E, F))_p$ (chap. II, § 2, n° 7, prop. 19), d'où aussitôt notre assertion; on conclut alors du th. 2 que $\mathrm{Ass}(\mathrm{Hom}_A(E, F)) \subset \mathrm{Supp}(E)$.

Inversement, soit $p$ un idéal premier de $A$ appartenant à $\mathrm{Ass}(F) \cap \mathrm{Supp}(E)$. Par définition, $F$ contient un sous-module isomorphe à $A/p$. D'autre part, puisque $E$ est de type fini et $E_p \neq 0$, on sait qu'il existe un homomorphisme $\omega \neq 0$ de $E$ dans $A/p$ (chap. II, § 4, n° 4, prop. 20). Comme il existe un homomorphisme injectif $j$ de $A/p$ dans $F$, on a $j \circ \omega \in \mathrm{Hom}(E, F)$, et $j \circ \omega \neq 0$. D'autre part, la relation $a \omega = 0$ pour un $a \in A$ équivaut à $a \in p$, l'annulateur de tout élément $\neq 0$ de $A/p$ étant $p$; on a donc bien $p \in \mathrm{Ass}(\mathrm{Hom}_A(E, F))$.

C. Q. F. D.

## EXERCICES {#ac-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
