---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ENSEMBLES ORDONNÉS, CARDINAUX, NOMBRES ENTIERS
section: 3
section_title: Ensembles équipotents. Cardinaux
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E III.23-E III.30, E III.79
pdf_pages: 0127-0134, 0183-0183
extraction: ocr
subsections:
    - "no": 1
      title: Le cardinal d’un ensemble
      page: 23
      pdf_page: 127
    - "no": 2
      title: Relation d'ordre entre cardinaux
      page: 24
      pdf_page: 128
    - "no": 3
      title: Opérations sur les cardinaux
      page: 25
      pdf_page: 129
    - "no": 4
      title: Propriétés des cardinaux 0 et 1
      page: 27
      pdf_page: 131
    - "no": 5
      title: Exponentiation des cardinaux
      page: 28
      pdf_page: 132
    - "no": 6
      title: Relation d’ordre et opérations entre cardinaux
      page: 29
      pdf_page: 133
statements: 32
exercises: 1
content_sha256: 940b752b58440ebe4daea0c9c83ad9df3293b5b19ed7383cf81a7f119541f724
---

## § 3. ENSEMBLES ÉQUIPOTENTS. CARDINAUX

### 1. Le cardinal d’un ensemble

#### Définition 1 {#ens-iii-s3-def-1 .statement tag=03QU}

*On dit qu’un ensemble X est équipotent à un ensemble Y s’il existe une bijection de X sur Y. On note Eq(X, Y) la relation « X est équipotent à Y ».*

Il est clair que les relations Eq(X, Y) et Eq(Y, X) sont équivalentes, autrement dit, la relation Eq(X, Y) est *symétrique*; lorsqu’elle est vraie, on dit aussi que *X et Y sont équipotents*. D’autre part, Eq(X, X) est vraie. Enfin la relation Eq(X, Y) est *transitive*, puisque la composée de deux bijections est une bijection (II, p. 19, th. 1); c’est donc une *relation d’équivalence*, réflexive dans tout ensemble.

De ce qui précède résulte que, si X et Y sont équipotents, la relation $(\forall Z)(Eq(X, Z) \Leftrightarrow Eq(Y, Z))$ est vraie. Or, le schéma S7 (I, p. 38) fournit l’axiome suivant

$$
((\forall Z)(Eq(X, Z) \Leftrightarrow Eq(Y, Z))) \Rightarrow (\tau_Z(Eq(X, Z)) = \tau_Z(Eq(Y, Z))).
$$

Donc, si X et Y sont équipotents, on a

$$
\tau_Z(Eq(X, Z)) = \tau_Z(Eq(Y, Z)).
$$

Posons la définition suivante:

#### Définition 2 {#ens-iii-s3-def-2 .statement tag=03QV}

*L’ensemble $\tau_Z(Eq(X, Z))$ est appelé le cardinal de X* (ou la *puissance* de X) *et se note Card (X)*.

Comme Eq(X, X) est vraie, Card (X) est *équipotent* à X (I, p. 33, schéma S5). Nous avons donc démontré le résultat suivant:

#### Proposition 1 {#ens-iii-s3-prop-1 .statement tag=03QW}

*Pour que deux ensembles X, Y soient équipotents, il faut et il suffit que leurs cardinaux soient égaux*.

Exemples
1) On note 0 le cardinal Card ($\varnothing$). Le seul ensemble équipotent à $\varnothing$ étant $\varnothing$ (II, p. 10 et p. 14), on a $0 = \mathrm{Card}(\varnothing) = \varnothing$.

2) Tous les ensembles à un élément sont équipotents, car {(a, b)} est le graphe d'une bijection de {a} sur {b}; en particulier, ils sont équipotents à {\emptyset}. On note 1 le cardinal

$$
\operatorname{Card}(\{\emptyset\}) = \tau_Z(\operatorname{Eq}(\{\emptyset\}, Z)).
$$

3) On note 2 le cardinal Card ({\emptyset, \{\emptyset\}}); c'est le cardinal de tout ensemble à deux éléments dont les éléments sont différents.

4) \* Un espace hilbertien de type dénombrable est équipotent à l'ensemble des nombres réels.*

### 2. Relation d'ordre entre cardinaux

La relation « X est équipotent à une partie de Y » est équivalente à « il existe une injection de X dans Y »; elle équivaut aussi à la relation « Card (X) est équipotent à une partie de Card (Y) » (II, p. 19, th. 1).

#### Théorème 1 {#ens-iii-s3-thm-1 .statement tag=03QX}

La relation R{\xi, \eta}:

« \xi et \eta sont des cardinaux et \xi est équipotent à une partie de \eta » est une relation de bon ordre (III, p. 15).

Comme R{\xi, \xi} est vraie pour tout cardinal \xi, tout revient à voir que, pour tout ensemble E de cardinaux, la relation « \xi \in E et \eta \in E et R{\xi, \eta} » est une relation de bon ordre dans E. Considérons l'ensemble A = \bigcup_{\xi \in E} \xi; tout cardinal \xi \in E est donc une partie de A. Il existe sur A une relation de bon ordre (III, p. 20, th. 1) que nous noterons x \leq y, et toute partie de A est équipotente à un segment de A (III, p. 22, cor. 3). Pour tout cardinal \xi \in E, considérons l'ensemble des segments de A équipotents à \xi; cet ensemble de segments n'est pas vide, et admet donc un plus petit élément (III, p. 16, prop. 2); soit \varphi(\xi) cet élément. La relation

« \xi \in E et \eta \in E et \xi est équipotent à une partie de \eta »

est équivalente à

« \xi \in E et \eta \in E et \varphi(\xi) \subset \varphi(\eta) ».

contredisant la définition de $\varphi(\varepsilon)$. Comme l’ensemble des segments de A est bien ordonné par inclusion (III, p. 16, prop. 2), le théorème est démontré.

Nous noterons $\varepsilon \leq \eta$ la relation $R \{ \varepsilon, \eta \}$. Pour qu’un ensemble X soit équivalent à une partie d’un ensemble Y, il faut et il suffit que Card (X) $\leq$ Card (Y).

Il est clair que l’on a $0 \leq \varepsilon$ pour tout cardinal $\varepsilon$, et $1 \leq \varepsilon$ pour tout cardinal $\varepsilon \neq 0$.

#### Corollaire 1 {#ens-iii-s3-thm-1-cor-1 .statement tag=03QY}

Étant donnés deux ensembles, l’un est équivalent à une partie de l’autre.

#### Corollaire 2 {#ens-iii-s3-thm-1-cor-2 .statement tag=03QZ}

Deux ensembles tels que chacun soit équivalent à une partie de l’autre sont équipotents.

#### Remarque {#ens-iii-s3-n2-rem-1 .statement tag=03R0}

Pour tout ensemble A, il existe un ensemble dont les éléments sont les cardinaux Card (X) pour toutes les parties X de A : en effet, c’est l’ensemble des objets de la forme Card (X) pour $X \in \mathfrak{P}(A)$ (II, p. 6). Pour tout cardinal $\alpha$, la relation « $\varepsilon$ est un cardinal et $\varepsilon \leq \alpha$ » est donc collectivisante en $\varepsilon$ (II, p. 5), puisqu’elle est équivalente à la relation « $\varepsilon$ est de la forme Card (X) pour $X \subset \alpha$ » ; l’ensemble des $\varepsilon$ satisfaisant à cette relation est appelé l’ensemble des cardinaux $\leq \alpha$.

#### Proposition 2 {#ens-iii-s3-prop-2 .statement tag=03KL}

Pour toute famille $(\alpha_i)_{i \in I}$ de cardinaux, il existe un cardinal et un seul $b$ tel que $\alpha_i \leq b$ pour tout $i \in I$ et que tout cardinal $c$ tel que $\alpha_i \leq c$ pour tout $i \in I$ soit $\geq b$.

En effet, il existe un ensemble E contenant tous les ensembles $\alpha_i$ (par exemple la somme de ces ensembles (II, p. 30)), d’où $\alpha_i \leq \alpha = \mathrm{Card}(E)$ pour tout $i \in I$. L’ensemble F des cardinaux $\leq \alpha$ étant bien ordonné et tous les $\alpha_i$ appartenant à F, la famille $(\alpha_i)_{i \in I}$ admet une borne supérieure $b$ dans cet ensemble. En outre, soit $c$ un cardinal $\geq \alpha_i$ pour tout $i \in I$; si on avait $c < b \leq \alpha$, on aurait $c \in F$, et l’inégalité $\alpha_i \leq c$ contredirait alors la définition de la borne supérieure de la famille $(\alpha_i)$ dans l’ensemble ordonné F ; d’où la proposition.

Par abus de langage, on dit que le cardinal $b$ est la borne supérieure de la famille $(\alpha_i)_{i \in I}$ de cardinaux et on le note $\sup_{i \in I} \alpha_i$.

#### Proposition 3 {#ens-iii-s3-prop-3 .statement tag=03KM}

Soient X et Y des ensembles. S’il existe une surjection f de X sur Y, on a $\mathrm{Card}(Y) \leq \mathrm{Card}(X)$.

En effet, il existe une section s associée à f (II, p. 18, prop. 8) et s est une injection de Y dans X.

### 3. Opérations sur les cardinaux

#### Définition 3 {#ens-iii-s3-def-3 .statement tag=03KN}

Soit $(\alpha_i)_{i \in I}$ une famille de cardinaux. Le cardinal de l’ensemble produit (resp. somme) des ensembles $\alpha_i$ s’appelle le produit cardinal (resp. la somme cardinale) des $\alpha_i$ et se note $\prod_{i \in I} \alpha_i$ (resp. $\sum_{i \in I} \alpha_i$).

Lorsque aucune confusion n’est à craindre, on dit simplement « produit » et «somme» au lieu de «produit cardinal» et «somme cardinale», et on écrit $\prod_{i \in I} a_i$ au lieu de $\prod_{i \in I} a_i$ (cf. III, p. 80, exerc. 2).

#### Proposition 4 {#ens-iii-s3-prop-4 .statement tag=03KO}

*Soient* $(E_i)_{i \in I}$ *une famille d'ensembles*, P *son produit*, S *sa somme*, $a_i$ *le cardinal de* $E_i$; *le cardinal de* P (resp. S) *est le produit cardinal* (resp. *la somme cardinale*) *de la famille* $(a_i)_{i \in I}$.

Il existe en effet une bijection de P (resp. S) sur l'ensemble produit des ensembles $a_i$ (resp. sur l'ensemble somme des $a_i$) (II, p. 30, prop. 10 et p. 38, cor. de la prop. 11).

#### Corollaire {#ens-iii-s3-n3-cor-1 .statement tag=03KP}

*Pour toute famille* $(E_i)_{i \in I}$ *d'ensembles*, le *cardinal de la réunion* $\bigcup_{i \in I} E_i$ *est au plus égal à la somme* $\sum_{i \in I} \mathrm{Card}(E_i)$.

En effet, il existe une application de la somme S des $E_i$ sur leur réunion (II, p. 30); le corollaire résulte donc des prop. 3 et 4.

#### Proposition 5 {#ens-iii-s3-prop-5 .statement tag=03R1}

a) *Soit* $(a_i)_{i \in I}$ *une famille de cardinaux*, et soit $f$ *une bijection d'un ensemble* K *sur l'ensemble* I; *on a*

$$
\sum_{\kappa \in K} a_{f(\kappa)} = \sum_{i \in I} a_i \quad \text{et} \quad \prod_{\kappa \in K} a_{f(\kappa)} = \prod_{i \in I} a_i.
$$

b) *Soient* $(a_i)_{i \in I}$ *une famille de cardinaux*, et $(J_\lambda)_{\lambda \in L}$ *une partition de* I; *on a* (*associativité de la somme et du produit*)

$$
\sum_{i \in I} a_i = \sum_{\lambda \in L} \left( \sum_{i \in J_\lambda} a_i \right)
$$
$$
\prod_{i \in I} a_i = \prod_{\lambda \in L} \left( \prod_{i \in J_\lambda} a_i \right).
$$

c) *Soit* $((a_{\lambda i})_{i \in J_\lambda})_{\lambda \in L}$ *une famille (admettant* L *comme ensemble d'indices)* de *familles de cardinaux*. *Soit* $I = \prod_{\lambda \in L} J_\lambda$; *on a* (*distributivité du produit par rapport à la somme*)

$$
\prod_{\lambda \in L} \left( \sum_{i \in J_\lambda} a_{\lambda i} \right) = \sum_{f \in I} \left( \prod_{\lambda \in L} a_{\lambda, f(\lambda)} \right).
$$

Les relations de *a*) résultent des formules analogues pour la réunion et le produit d'ensembles, car le fait que $f$ est une bijection implique que, si $(X_i)_{i \in I}$ est une famille d'ensembles mutuellement disjoints, il en est de même de la famille $(X_{f(\kappa)})_{\kappa \in K}$ (cf. II, p. 23, prop. 1 et p. 33, prop. 4).

Les relations de *b*) sont conséquences immédiates des formules d'associativité de la réunion et du produit (II, 24, prop. 2 et p. 35, prop. 7) et de la distributivité de l'intersection par rapport à la réunion (II, p. 35, prop. 8) qui prouve que, si $(X_i)_{i \in I}$ est une famille d'ensembles mutuellement disjoints, il en est de même de la famille $(\bigcup_{i \in J_\lambda} X_i)_{\lambda \in L}$.

Enfin, c) est conséquence de la distributivité du produit par rapport à la réunion et à l’intersection (II, p. 36, prop. 9 et p. 37, cor. 1).

Soient $a$ et $b$ deux cardinaux. Si I est un ensemble à deux éléments distincts (par exemple le cardinal 2), il existe une application $f$ de I sur $\{a, b\}$, ce qui définit une famille de cardinaux; la somme et le produit de celle-ci ne dépendent que de $a$ et $b$ (en vertu de la prop. 5 a)); on appelle ces cardinaux la somme et le produit de $a$ et de $b$, et on les note $a + b$ et $ab$. On définit et note de même la somme et le produit de plusieurs cardinaux. La prop. 5 entraîne alors le corollaire suivant:

#### Corollaire {#ens-iii-s3-n3-cor-2 .statement tag=03R2}

Soient $a, b, c$ des cardinaux; on a

(1) $$
a + b = b + a,\qquad ab = ba,
$$
(2) $$
a + (b + c) = (a + b) + c,\qquad a(bc) = (ab)c,
$$
(3) $$
a(b + c) = ab + ac.
$$

### 4. Propriétés des cardinaux 0 et 1

#### Proposition 6 {#ens-iii-s3-prop-6 .statement tag=03R3}

Soient $(a_i)_{i \in I}$ une famille de cardinaux, et J (resp. K) une partie de I telle que l’on ait $a_i = 0$ pour tout $i \notin J$ (resp. $a_i = 1$ pour tout $i \notin K$); on a alors

$$
\sum_{i \in I} a_i = \sum_{i \in J} a_i
$$
(resp. $\prod_{i \in I} a_i = \prod_{i \in K} a_i$).

C’est immédiat pour la somme, car l’ensemble somme $S_I$ de la famille d’ensembles $(a_i)_{i \in I}$ est équipotent à la réunion de l’ensemble somme $S_J$ de la famille $(a_i)_{i \in J}$ et de l’ensemble vide, donc équipotent à $S_J$. Pour le produit, cela résulte de ce que la projection $\mathrm{pr}_K$ de l’ensemble produit $\prod_{i \in I} a_i$ sur le produit partiel $\prod_{i \in K} a_i$ est une bijection (II, p. 35, Remarque 1).

#### Corollaire 1 {#ens-iii-s3-prop-6-cor-1 .statement tag=03R4}

Pour tout cardinal $a$, on a $a + 0 = a.1 = a$.

#### Corollaire 2 {#ens-iii-s3-prop-6-cor-2 .statement tag=03R5}

Soient $a$ et $b$ des cardinaux, et soit I un ensemble équipotent à $b$; pour tout $i \in I$, soit $a_i = a, c_i = 1$; on a

$$
ab = \sum_{i \in I} a_i \quad \text{et} \quad b = \sum_{i \in I} c_i.
$$

La seconde formule résulte de ce qu’un ensemble est réunion de l’ensemble de ses parties à un élément. La première s’en déduit par multiplication par $a$, en utilisant le cor. 1.

#### Proposition 7 {#ens-iii-s3-prop-7 .statement tag=03R6}

Soit $(\alpha_i)_{i \in I}$ une famille de cardinaux; pour que l’on ait $P_{i \in I} \alpha_i \neq 0$, il faut et il suffit que l’on ait $\alpha_i \neq 0$ pour tout $i \in I$.

Cela ne fait que traduire la condition pour qu’un ensemble produit soit non vide (II, p. 34, cor. 2).

#### Proposition 8 {#ens-iii-s3-prop-8 .statement tag=03R7}

Si $a$ et $b$ sont des cardinaux tels que $a + 1 = b + 1$, on a $a = b$.

Soit $X = a + 1 = b + 1$. Il existe des parties $A, B$ de $X$, de cardinaux $a$ et $b$, telles que les complémentaires $X - A$ et $X - B$ soient chacun réduits à un seul élément; soient $u$ et $v$ ces éléments. L’intersection $C = A \cap B$ a pour complémentaire dans $X$ l’ensemble $\{u, v\}$. Si $u = v$, on a $A = B = C$, d’où $a = b$. Sinon $A = C \cup \{v\}$, $B = C \cup \{u\}$, et $a = 1 + \mathrm{Card}(C) = b$.

On se gardera de croire que $a + m = b + m$ entraîne $a = b$ pour tout cardinal $m$ (cf. III, p. 48); *nous verrons cependant qu’il en est bien ainsi lorsque $m$ est fini (III, p. 37, cor. 4 et p. 49, cor. 4).*

### 5. Exponentiation des cardinaux

#### Définition 4 {#ens-iii-s3-def-4 .statement tag=03KQ}

Soient $a$ et $b$ des cardinaux; le cardinal de l’ensemble des applications de $b$ dans $a$ se note $a^b$, par abus de notation.

L’abus provient de ce que cette notation désigne déjà l’ensemble des graphes fonctionnels d’applications de $b$ dans $a$ (II, p. 31) et que ce dernier ensemble n’est pas nécessairement un cardinal (III, p. 80, exerc. 2). Le contexte indiquera toujours clairement le sens qu’il faut donner à $a^b$.

#### Proposition 9 {#ens-iii-s3-prop-9 .statement tag=03KR}

Soient $X$ et $Y$ deux ensembles, $a$ et $b$ leurs cardinaux; l’ensemble $X^Y$ a pour cardinal $a^b$.

En effet, il existe une bijection de $X^Y$ sur l’ensemble des applications de $b$ dans $a$ (II, p. 31, corollaire).

#### Proposition 10 {#ens-iii-s3-prop-10 .statement tag=03KS}

Soient $a$ et $b$ des cardinaux, et $I$ un ensemble tel que $\mathrm{Card}(I) = b$; si $\alpha_i = a$ pour tout $i \in I$, on a $a^b = P_{i \in I} \alpha_i$.

Cela résulte de la définition du produit d’une famille d’ensembles comme ensemble de graphes fonctionnels (II, p. 32).

#### Corollaire 1 {#ens-iii-s3-prop-10-cor-1 .statement tag=03KT}

Soient $a$ un cardinal et $(b_i)_{i \in I}$ une famille de cardinaux. On a
$$
a^{\sum_{i \in I} b_i} = P_{i \in I} a^{b_i}.
$$
En effet, soit $S$ l’ensemble somme des $b_i$, et posons $\alpha_s = a$ pour tout $s \in S$. Les deux membres de l’égalité à démontrer sont alors égaux à $P_{s \in S} \alpha_s$, en vertu de la prop. 10 et de la formule d’associativité du produit (III, p. 26, prop. 5 b)).

#### Corollaire 2 {#ens-iii-s3-prop-10-cor-2 .statement tag=03KU}

Soient $(a_i)_{i \in I}$ une famille de cardinaux, et $b$ un cardinal ; on a
$$
(\mathcal{P}_{i \in I} a_i)^b = \mathcal{P}_{i \in I} a_i^b.
$$
En effet, posons $a_{i,\beta} = a_i$ pour tout couple $(i, \beta) \in I \times b$. On a alors, en vertu de l’associativité du produit
$$
(\mathcal{P}_{i \in I} a_i)^b = \mathcal{P}_{\beta \in b} (\mathcal{P}_{i \in I} a_{i,\beta}) = \mathcal{P}_{i \in I} (\mathcal{P}_{\beta \in b} a_{i,\beta}) = \mathcal{P}_{i \in I} a_i^b.
$$

#### Corollaire 3 {#ens-iii-s3-prop-10-cor-3 .statement tag=03KV}

Soient $a, b, c$ des cardinaux ; on a $a^{bc} = (a^b)^c$.
En effet, posons $b_\gamma = b$ pour tout $\gamma \in c$. On a
$$
a^{bc} = a^{\sum_{\gamma \in c} b_\gamma} = \mathcal{P}_{\gamma \in c} a^{b_\gamma} = (a^b)^c,
$$
en vertu du cor. 1.

#### Proposition 11 {#ens-iii-s3-prop-11 .statement tag=03KW}

Soit $a$ un cardinal. On a $a^0 = 1$, $a^1 = a$, $1^a = 1$ ; si $a \neq 0$, on a $0^a = 0$.
En effet, il existe une application et une seule de $\varnothing$ dans un ensemble quelconque (l’application de graphe vide) ; l’ensemble des applications d’un ensemble à un seul élément dans un ensemble quelconque $X$ est équipotent à $X$ (II, p. 32) ; il existe une application et une seule d’un ensemble quelconque dans un ensemble à un élément ; enfin, il n’existe aucune application d’un ensemble non vide dans $\varnothing$.

On notera en particulier que l’on a $0^0 = 1$.

#### Proposition 12 {#ens-iii-s3-prop-12 .statement tag=03KX}

Soient $X$ un ensemble et $a$ son cardinal ; le cardinal de l’ensemble $\mathfrak{P}(X)$ des parties de $X$ est $2^a$.
Soient $\alpha$ et $\beta$ les éléments du cardinal 2 ; pour toute partie $Y$ de $X$, soit $f_Y$ l’application de $X$ dans 2, définie par $f_Y(x) = \alpha$ pour $x \in Y$ et $f_Y(x) = \beta$ pour $x \in X - Y$ ; soit $u$ l’application $Y \mapsto f_Y$ de $\mathfrak{P}(X)$ dans $2^X$. Inversement, à toute application $g$ de $X$ dans 2, faisons correspondre la partie $\bar{g}^{-1}(\alpha)$ de $X$, et soit $v$ l’application $g \mapsto \bar{g}^{-1}(\alpha)$ de $2^X$ dans $\mathfrak{P}(X)$. Il est clair que les applications $u \circ v$ et $v \circ u$ sont les applications identiques de $2^X$ et de $\mathfrak{P}(X)$. Donc $u$ et $v$ sont des bijections (II, p. 18, corollaire), ce qui montre que Card $(\mathfrak{P}(X)) = 2^a$.

### 6. Relation d’ordre et opérations entre cardinaux

#### Proposition 13 {#ens-iii-s3-prop-13 .statement tag=03KY}

Soient $a$ et $b$ des cardinaux ; pour que l’on ait $a \geq b$, il faut et il suffit qu’il existe un cardinal $c$ tel que $a = b + c$.
En effet, la relation $a \geq b$ signifie qu’il existe une partie $B$ de $a$ équipotente à $b$ (III, p. 24), c’est-à-dire que $a$ est équipotent à l’ensemble somme de $b$ et d’un ensemble $C$.

Si $a \geq b$, il existe en général plusieurs cardinaux $c$ tels que $a = b + c$ (cf. III, p. 30); on ne peut donc en général définir une « différence » $a - b$ de deux tels cardinaux (cf. III, p. 37).

#### Proposition 14 {#ens-iii-s3-prop-14 .statement tag=03KZ}

*Soient* $(\alpha_i)_{i \in I}$ et $(b_i)_{i \in I}$ *deux familles de cardinaux ayant même ensemble d'indices* $I$, *et telles que* $\alpha_i \geq b_i$ *pour tout* $i \in I$; *on a alors*

$$
\sum_{i \in I} \alpha_i \geq \sum_{i \in I} b_i \quad \text{et} \quad \prod_{i \in I} \alpha_i \geq \prod_{i \in I} b_i.
$$

La seconde inégalité résulte des relations d'inclusion entre produits d'ensembles (II, p. 34, cor. 3). D'autre part, si un ensemble $E$ est réunion d'une famille $(A_i)_{i \in I}$ de parties mutuellement disjointes et si $B_i \subset A_i$ pour tout $i$, les $B_i$ sont mutuellement disjointes et $\bigcup_i B_i \subset \bigcup_i A_i$ (II, p. 24), d'où la première inégalité.

#### Corollaire 1 {#ens-iii-s3-prop-14-cor-1 .statement tag=03L0}

*Soit* $(\alpha_i)_{i \in I}$ *une famille de cardinaux*. *Pour toute partie* $J$ *de* $I$, *on a* $\sum_{i \in J} \alpha_i \leq \sum_{i \in I} \alpha_i$. *Si en outre on a* $\alpha_i \neq 0$ *pour tout* $i \in I - J$, *on a* $\prod_{i \in J} \alpha_i \leq \prod_{i \in I} \alpha_i$.

Posons $b_i = \alpha_i$ pour $i \in J$, et $b_i = 0$ (resp. $b_i = 1$) pour $i \in I - J$. Il suffit d'appliquer la prop. 14, en remarquant que la relation $\alpha \neq 0$ entraîne $\alpha \geq 1$.

#### Corollaire 2 {#ens-iii-s3-prop-14-cor-2 .statement tag=03L1}

*Si* $a, a', b, b'$ *sont des cardinaux tels que* $a \leq a'$, $b \leq b'$ *et* $a' > 0$, *on a* $a^{b'} \leq a'^{b'}$.

On a en effet $a^b \leq a'^{b'}$ d'après les prop. 10 (III, p. 28) et 14, et $a'^b \leq a'^{b'}$ d'après la prop. 10 et le cor. 1 de la prop. 14.

**Théorème 2** (Cantor). — *Pour tout cardinal* $a$, *on a* $2^a > a$.

En effet, on a $\mathrm{Card}(\mathfrak{P}(a)) = 2^a$ (III, p. 29, prop. 12). L'application $x \mapsto \{x\}$ ($x \in a$) est une injection de $a$ dans $\mathfrak{P}(a)$; d'où $a \leq 2^a$. Il suffit de montrer que $a \neq 2^a$, c'est-à-dire que, pour toute application $f$ de $a$ dans $\mathfrak{P}(a)$, l'image $f(a)$ est distincte de $\mathfrak{P}(a)$. Or, soit $X$ l'ensemble des $x \in a$ tels que $x \notin f(x)$; si $x \in X$, on a $x \notin f(x)$, d'où $f(x) \neq X$; si $x \in a - X$, on a $x \in f(x)$ et $x \notin X$, donc $f(x) \neq X$. Ceci démontre que $X \notin f(a)$, d'où le théorème.

#### Corollaire {#ens-iii-s3-n6-cor-1 .statement tag=03L2}

*Il n'existe pas d'ensemble dont tout cardinal soit élément*.

Si $U$ était un tel ensemble, il existerait un ensemble $S$, somme de la famille d'ensembles $(X)_{X \in U}$, et tout cardinal serait équipotent à une partie de $S$. En particulier, soit $s = \mathrm{Card} (S)$; comme $2^s$ est un cardinal, on aurait $2^s \leq s$, ce qui est absurde.

## EXERCICES {#ens-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
