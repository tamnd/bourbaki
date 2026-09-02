---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ENSEMBLES ORDONNÉS, CARDINAUX, NOMBRES ENTIERS
section: 4
section_title: Entiers naturels. Ensembles finis
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E III.30-E III.35, E III.80-E III.83
pdf_pages: 0134-0139, 0184-0187
extraction: ocr
subsections:
    - "no": 1
      title: Définition des entiers
      page: 30
      pdf_page: 134
    - "no": 2
      title: Inégalités entre entiers
      page: 31
      pdf_page: 135
    - "no": 3
      title: Le principe de récurrence
      page: 32
      pdf_page: 136
    - "no": 4
      title: Parties finies d’ensembles ordonnés
      page: 34
      pdf_page: 138
    - "no": 5
      title: Propriétés de caractère fini
      page: 34
      pdf_page: 138
statements: 14
exercises: 11
content_sha256: cba69c356e78ad0bb33d0f0ec930a55926e64996fd34519666a29382bd1320e1
---

## § 4. ENTIERS NATURELS. ENSEMBLES FINIS

### 1. Définition des entiers

#### Définition 1 {#ens-iii-s4-def-1 .statement tag=03R9}

*On dit qu'un cardinal* $a$ *est fini si* $a \neq a + 1$; *un cardinal fini s'appelle aussi un entier naturel* (ou simplement un *entier* si aucune confusion n'est à craindre.)¹ On dit qu’un ensemble E est fini si Card (E) est un cardinal fini ; on dit alors que Card (E) est le nombre d’éléments de E.

On dit qu’une famille (II, p. 14) est finie si son ensemble d’indices est fini.

Quand nous dirons que le nombre des objets d’un certain type est un entier m, nous entendrons que ces objets sont les éléments d’un ensemble fini dont le nombre d’éléments est m. Un ensemble dont le nombre d’éléments est m est encore appelé un ensemble à m éléments.

#### Proposition 1 {#ens-iii-s4-prop-1 .statement tag=03RA}

Pour qu’un cardinal a soit fini, il faut et il suffit que a + 1 soit fini.

On sait en effet que les relations a = b et a + 1 = b + 1 entre cardinaux a et b sont équivalentes (III, p. 28, prop. 8); les relations a ≠ a + 1 et a + 1 ≠ (a + 1) + 1 sont donc équivalentes.

Il est clair que 0 ≠ 1; donc 0 est un entier; on en déduit que 1 et 2 sont des entiers. Les cardinaux 2 + 1 et (2 + 1) + 1 sont des entiers, que l’on note 3 et 4.

### 2. Inégalités entre entiers

#### Proposition 2 {#ens-iii-s4-prop-2 .statement tag=03RB}

Soit n un entier. Tout cardinal a tel que a ≤ n est un entier. Si n ≠ 0, il existe un entier m et un seul tel que n = m + 1, et la relation a < n est équivalente à a ≤ m.

Si a ≤ n, il existe un cardinal b tel que n = a + b (III, p. 29, prop. 13). Alors (a + 1) + b = (a + b) + 1 = n + 1 (III, p. 27, cor. de la prop. 5), et comme n ≠ n + 1, on a (a + 1) + b ≠ a + b; par suite a + 1 ≠ a, ce qui signifie que a est un entier. Si n ≠ 0, on a n ≥ 1 (III, p. 25), donc il existe un cardinal m et un seul tel que n = m + 1 (III, p. 29, prop. 13 et p. 28, prop. 8); comme m ≤ n, m est un entier un vertu de ce qui précède. Enfin, si un entier a est tel que a < n, on a n = a + b, avec b ≠ 0 (III, p. 29, prop. 13); comme b est entier, on a b = c + 1 et n = m + 1 = (a + c) + 1. On en conclut que m = a + c (III, p. 28, prop. 8), d’où a ≤ m (III, p. 29, prop. 13). Inversement, si a ≤ m, on a aussi a ≤ m + 1 = n, et si on avait a = n = m + 1, on aurait a > m, contrairement à l’hypothèse.

#### Corollaire 1 {#ens-iii-s4-prop-2-cor-1 .statement tag=03RC}

Toute partie d’un ensemble fini est finie.

#### Corollaire 2 {#ens-iii-s4-prop-2-cor-2 .statement tag=03RD}

Si X est une partie d’un ensemble fini E, distincte de E, on a Card (X) < Card (E).

En effet, X est contenu dans le complémentaire X’ d’une partie de E réduite à un seul élément; on a Card (X) ≤ Card (X’), et Card (E) = Card (X’) + 1, donc (prop. 2) Card (X’) < Card (E) et a fortiori Card (X) < Card (E).

La déf. 1 montre inversement que, si E est un ensemble tel que Card (X) < Card (E) pour toute partie X ≠ E de E, E est fini.

¹ La notion d’« entier » sera plus tard généralisée en Algèbre, où l’on définira les entiers rationnels (A, I, § 2, n° 5) et les entiers algébriques (AC, V, § 1, n° 1).

#### Corollaire 3 {#ens-iii-s4-prop-2-cor-3 .statement tag=03RE}

Si $f$ est une application d’un ensemble fini $E$ dans un ensemble $F$, (E) est une partie finie de $F$.

En effet, Card ($f(E)$) $\leqslant$ Card (E) (III, p. 25, prop. 3).

#### Corollaire 4 {#ens-iii-s4-prop-2-cor-4 .statement tag=03RF}

Soient $E$ et $F$ deux ensembles finis ayant le même nombre d’éléments, et $f$ une application de $E$ dans $F$. Les propriétés suivantes sont équivalentes :
a) $f$ est une injection ;
b) $f$ est une surjection ;
c) $f$ est une bijection.

Il suffit de prouver que $a)$ et $b)$ sont équivalentes. Si $f$ est injective, on a Card ($f(E)$) = Card (E) = Card (F), d’où $f(E) = F$ (cor. 2). Si $f$ n’est pas injective, soient $x, x'$ deux éléments de $E$ tels que $x \neq x'$ et $f(x) = f(x')$. Alors, en posant $E' = E - \{x\}$, on a $f(E') = f(E)$, d’où

$$
\text{Card } (f(E)) \leqslant \text{Card } (E') < \text{Card } (E)
$$

en vertu du cor. 2; mais comme Card (F) = Card (E), on a nécessairement $f(E) \neq F$.

### 3. Le principe de récurrence

C61 (principe de récurrence). Soit $R^{n}$ une relation dans une théorie $\mathcal{T}$ (n n’étant pas une constante de $\mathcal{T}$). On suppose que la relation

$$
R^{0} \text{ et } (\forall n)((n \text{ est un entier et } R^{n}) \Rightarrow R^{n + 1})
$$

soit un théorème de $\mathcal{T}$. Dans ces conditions, la relation

$$
(\forall n)((n \text{ est un entier}) \Rightarrow R^{n})
$$

est un théorème de $\mathcal{T}$.

Raisonnons par l’absurde et supposons que la relation

$$
(\exists n)(n \text{ est un entier et (non } R^{n}))
$$

soit vraie. Soit $q$ un entier tel que « non $R^{q}$ » (méthode de la constante auxiliaire; cf. I, p. 28 et p. 32). Les entiers $n$ tels que « $n \leq q$ et (non $R^{n}$) » forment un ensemble non vide bien ordonné (III, p. 25, Remarque) qui aurait donc un plus petit élément $s$. Si $s = 0$, on aurait « non $R^{0}$ », ce qui est contraire à l’hypothèse. Si $s > 0$, on aurait $s = s' + 1$, où $s'$ est un entier tel que $s' < s$ (III, p. 31, prop. 2). Par définition de $s$, on aurait donc $R^{s'}$, mais alors l’hypothèse entraînerait que $R^{s}$ est vraie, ce qui contredit la définition de $s$.

Pour appliquer le principe de récurrence, il faut en particulier démontrer la relation

$$
(n \text{ est un entier et } R^{n}) \Rightarrow R^{n + 1}.
$$

Pour ce faire, on utilise souvent la méthode de l’hypothèse auxiliaire (I, p. 27) et c’est pourquoi la relation « $n$ est un entier et $R^{n}$ » (ou même $R^{n}$) est appelée l’hypothèse de récurrence.

#### Remarque {#ens-iii-s4-n3-rem-1 .statement}

On utilise souvent, sous le nom de « principe de récurrence » divers critères qui se déduisent aisément de C61, et dont nous allons indiquer les plus importants:

1) Soit S\{n\} la relation
$$(\forall p)((n \text{ est un entier et } p \text{ est un entier et } p < n) \Rightarrow R\{p\})$$
et supposons que S\{n\} entraîne R\{n\}. Alors, la relation
$$(\forall n)((n \text{ est un entier}) \Rightarrow R\{n\})$$
est vraie. En effet, la relation S\{0\} est vraie, et par hypothèse S\{n\} entraîne R\{n\}; comme la relation $m < n + 1$ est équivalente à $m \leq n$ (III, p. 31, prop. 2), la relation S\{n + 1\} est équivalente à « S\{n\} et R\{n\} »; par suite, S\{n\} entraîne S\{n + 1\}. Le critère C61 prouve alors que la relation
$$(\forall n)((n \text{ est un entier}) \Rightarrow S\{n\})$$
est vraie, et comme S\{n\} entraîne R\{n\}, la relation
$$(\forall n)((n \text{ est un entier}) \Rightarrow R\{n\})$$
est vraie.

2) Soient k un entier, R\{n\} une relation telle que la relation
$$R\{k\} \text{ et } (\forall n)((n \text{ est un entier } \geq k \text{ et } R\{n\}) \Rightarrow R\{n + 1\})$$
sont vraie. Alors, la relation
$$(\forall n)((n \text{ est un entier } \geq k) \Rightarrow R\{n\})$$
est vraie (« récurrence à partir de k »). En effet, soit S\{n\} la relation « $(n \geq k) \Rightarrow R\{n\}$ »; alors, en utilisant la méthode de disjonction des cas, on voit que la relation S\{0\} est vraie; d’autre part, on vérifie aisément que la relation
$$(n \text{ est un entier et } S\{n\}) \Rightarrow S\{n + 1\}$$
est vraie. On conclut de C61 que la relation
$$(n \text{ est un entier}) \Rightarrow S\{n\}$$
est vraie, d’où notre assertion.

3) Soient a, b deux entiers tels que $a \leq b$, et soit R\{n\} une relation telle que l’on ait
$$R\{a\} \text{ et } (\forall n)((n \text{ est un entier et } a \leq n < b \text{ et } R\{n\}) \Rightarrow R\{n + 1\}).$$
Alors la relation
$$(\forall n)((n \text{ est un entier et } a \leq n \leq b) \Rightarrow R\{n\})$$
est vraie. On procède comme dans le cas précédent, en prenant pour S\{n\} la relation « $(a \leq n < b) \Rightarrow R\{n\}$ » (« récurrence limitée à un intervalle »).

4) Soient a, b deux entiers tels que $a \leq b$, et soit R\{n\} une relation telle que l’on ait
$$R\{b\} \text{ et } (\forall n)((n \text{ est un entier et } a \leq n < b \text{ et } R\{n + 1\}) \Rightarrow R\{n\}).$$

Alors, la relation

$$(\forall n)((n \text{ est un entier et } a \leq n \leq b) \Rightarrow R_{\{n\}})$$

est vraie. On a en effet la relation

$$(n \text{ est un entier et } a \leq n < b \text{ et (non } R_{\{n\}})) \Rightarrow (\text{non } R_{\{n + 1\}}).$$

Si, pour un $n$ tel que $a \leq n \leq b$, on avait (non $R_{\{n\}}$), on déduirait de 3) que l’on aurait (non $R_{\{b\}}$) contrairement à l’hypothèse; d’où le critère (« récurrence descendante »).

### 4. Parties finies d’ensembles ordonnés

#### Proposition 3 {#ens-iii-s4-prop-3 .statement tag=03L9}

Soit $E$ un ensemble préordonné filtrant à droite (resp. un ensemble ordonné réticulé, resp. un ensemble totalement ordonné). Toute partie finie non vide de $E$ est majorée (resp. admet une borne supérieure et une borne inférieure, resp. admet un plus grand et un plus petit élément).

Démontrons la proposition par récurrence sur le nombre $n$ d’éléments de la partie considérée. Le résultat est trivial pour $n = 1$. Soit $X$ une partie à $n + 1$ éléments de $E$ (avec $n \geq 1$), et posons $X = Y \cup \{x\}$, où $Y$ a $n$ éléments, donc n’est pas vide. L’hypothèse de récurrence implique qu’il existe un majorant (resp. une borne supérieure, resp. un plus grand élément) $y$ de $Y$. Puisque $E$ est filtrant à droite (resp. réticulé, resp. totalement ordonné), $\{x, y\}$ possède un majorant (resp. une borne supérieure, resp. un plus grand élément), qui est évidemment un majorant (resp. une borne supérieure, resp. un plus grand élément) de $X$.

#### Corollaire 1 {#ens-iii-s4-prop-3-cor-1 .statement tag=03LA}

Tout ensemble fini totalement ordonné est bien ordonné et admet un plus grand élément.

#### Corollaire 2 {#ens-iii-s4-prop-3-cor-2 .statement tag=03LB}

Tout ensemble ordonné fini admet un élément maximal.

En effet, un tel ensemble est inductif en vertu du cor. 1 (cf. III, p. 20, th. 2).

### 5. Propriétés de caractère fini

#### Définition 2 {#ens-iii-s4-def-2 .statement tag=03LC}

Soit $E$ un ensemble. On dit qu’un ensemble $\mathcal{S}$ de parties de $E$ est de caractère fini si la relation $X \in \mathcal{S}$ est équivalente à la relation « toute partie finie de $X$ appartient à $\mathcal{S}$ ».

On dit qu’une propriété $P_{\{X\}}$ d’une partie $X$ d’un ensemble $E$ est de caractère fini si l’ensemble des parties $X$ de $E$ pour lesquelles $P_{\{X\}}$ est vraie est de caractère fini.

#### Exemple 1 {#ens-iii-s4-n5-exa-1 .statement tag=03T9}

L’ensemble des parties totalement ordonnées d’un ensemble ordonné $E$ est de caractère fini : en effet, pour qu’une partie $X$ de $E$ soit totalement ordonnée, il faut et il suffit que toute partie à deux éléments de $X$ le soit.
    2) \* L’ensemble des parties libres d’un module est de caractère fini (A, II, § 1, n° 11). Il en est de même de l’ensemble des parties algébriquement libres d’une extension d’un corps commutatif (A, V, § 5).

3) L’ensemble des sous-modules d’un module E n’est pas de caractère fini, car une partie finie d’un sous-module de E n’est pas nécessairement un sous-module de E.*

#### Théorème 1 {#ens-iii-s4-thm-1 .statement tag=03LD}

Tout ensemble $\mathcal{S}$ de parties d’un ensemble E, de caractère fini, admet un élément maximal (quand on l’ordonne par inclusion).

En vertu du th. 2 de III, p. 20, il suffit de prouver que $\mathcal{S}$ est inductif; pour cela, nous montrerons que, pour toute partie $\mathcal{G}$ de $\mathcal{S}$, totalement ordonnée par inclusion, la réunion X des ensembles de $\mathcal{G}$ appartient à $\mathcal{S}$ (III, p. 21, cor. 2). Comme $\mathcal{S}$ est de caractère fini, il suffit d’établir que toute partie finie Y de X appartient à $\mathcal{S}$. Or, pour tout $y \in Y$, il existe un ensemble $Z_y \in \mathcal{G}$ tel que $y \in Z_y$; comme l’ensemble des $Z_y$ ($y \in Y$) est fini et totalement ordonné par inclusion, il admet un plus grand élément S (III, p. 34, cor. 1); autrement dit, il existe un ensemble $S \in \mathcal{G}$ tel que $Y \subset S$. Mais comme $S \in \mathcal{S}$ et que Y est une partie finie de S, on a $Y \in \mathcal{S}$, puisque $\mathcal{S}$ est de caractère fini, et ceci achève la démonstration.

## EXERCICES {#ens-iii-s4-exercises}

F telles que B' = F - A', de sorte que l'on ait A' = f(A) et B = g(B'). (Soit R = E - g(F), et posons h = g o f; prendre pour A l'intersection des parties M de E telle que M ⊃ R ∪ h(M).)

2) Si E et F sont des ensembles distincts, montrer que E^F ≠ F^E. En déduire que, si E et F sont les cardinaux 2 et 4 = 2 + 2, l'un au moins des ensembles E^F, F^E n'est pas un cardinal.

§ 3) Soient (a_t)_{t \in I}, (b_t)_{t \in I} deux familles de cardinaux, telles que b_t ≥ 2 pour tout t ∈ I.
a) Montrer que si a_t ≤ b_t pour tout t ∈ I, on a
$$
\sum_{t \in I} a_t \leq \prod_{t \in I} b_t.
$$
b) Montrer que si a_t < b_t pour tout t ∈ I, on a
$$
\sum_{t \in I} a_t < \prod_{t \in I} b_t.
$$
(Remarquer qu'un produit $\prod_{t \in I} E_t$ ne peut être réunion d'une famille $(A_t)_{t \in I}$ telle que Card(A_t) < Card(E_t) pour tout t ∈ I, en observant que l'on a Card(pr_t(A_t)) < Card(E_t)).

4) Soient E un ensemble, f une application de $\mathcal{P}(E) - \{ \varnothing \}$ dans E telle que, pour toute partie X ≠ $\varnothing$ de E, on ait f(X) ∈ X (« fonction de choix »).
a) Soit b un cardinal, et soit A l'ensemble des x ∈ E tels que Card(f(x)) ≤ b. Montrer que si a = Card(A), on a 2^a ≤ 1 + ab (remarquer que si Y ⊂ A et Y ≠ $\varnothing$, on a f(Y) ∈ A).
b) Soit B l'ensemble des x ∈ E tels que pour toute partie X ≠ $\varnothing$ de E appartenant à $f^{-1}(x)$, on ait Card(X) ≤ b. Montrer que Card(B) ≤ b.

5) Soit $(\lambda_t)_{t \in I}$ une famille de types d'ordre (III, p.76, exerc. 13), I étant un ensemble ordonné. Montrer que Card $\left( \sum_{t \in I} \lambda_t \right) = \sum_{t \in I} \mathrm{Card}(\lambda_t)$ et (si I est bien ordonné) Card $\left( \prod_{t \in I} \lambda_t \right) = \prod_{t \in I} \mathrm{Card}(\lambda_t)$.

6) Montrer que pour tout ensemble E, il existe X ⊂ E tel que X $\notin$ E (utiliser III, p. 20, th. 2).

- § 4

See the [exercises for § 4](exercises/s4/).
