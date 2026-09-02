---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ENSEMBLES ORDONNÉS, CARDINAUX, NOMBRES ENTIERS
section: 6
section_title: Ensembles infinis
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E III.45-E III.51, E III.87-E III.94
pdf_pages: 0149-0155, 0191-0198
extraction: ocr
subsections:
    - "no": 1
      title: L’ensemble des entiers naturels
      page: 45
      pdf_page: 149
    - "no": 2
      title: Définition d’applications par récurrence
      page: 46
      pdf_page: 150
    - "no": 3
      title: Calcul sur les cardinaux infinis
      page: 47
      pdf_page: 151
    - "no": 4
      title: Ensembles dénombrables
      page: 49
      pdf_page: 153
    - "no": 5
      title: Suites stationnaires
      page: 50
      pdf_page: 154
statements: 24
exercises: 33
content_sha256: 6bc1a96bfc0fa13351892267947be8e68da6e32aa23c8a59110ccaec5dd03a5f
---

## § 6. ENSEMBLES INFINIS

### 1. L’ensemble des entiers naturels

#### Définition 1 {#ens-iii-s6-def-1 .statement tag=03MV}

On dit qu’un ensemble est infini s’il n’est pas fini.

En particulier, un cardinal est infini s’il n’est pas un entier.

Remarquons que la relation « il existe un ensemble infini » entraîne que la relation « x est un entier » est collectivisante (II, p. 3); en effet, si α est un cardinal infini, et n un entier quelconque, on ne peut avoir α ≤ n (III, p. 31, prop. 2); on a donc n < α pour tout entier n, ce qui prouve que l’ensemble des entiers < α (III, p. 25, Remarque) contient tous les entiers. Inversement, si la relation « x est un entier » est collectivisante, l’ensemble des entiers E est un ensemble infini: en effet, pour tout entier n, l’intervalle {0, n} est une partie à n + 1 éléments de E (III, p. 38, prop. 5), donc Card (E) ≥ n + 1 > n; mais dire que Card (E) ≠ n pour tout entier n signifie que E est infini.

Introduisons l’axiome suivant:

A4 (« axiome de l’infini »). Il existe un ensemble infini.

On ne sait pas déduire cet axiome des axiomes et schémas d’axiomes introduits jusqu’ici, et, bien que la question ne soit pas définitivement tranchée, il est à présumer qu’il en est indépendant.

Les remarques qui précèdent prouvent alors le théorème suivant:

#### Théorème 1 {#ens-iii-s6-thm-1 .statement tag=03MW}

La relation « x est un entier » est collectivisante.

Nous désignerons par N l’ensemble des entiers (dit aussi « ensemble des entiers naturels » lorsqu’on veut éviter les confusions). Le cardinal de N se note aussi $\aleph_0$. Quand on considère N comme ensemble ordonné, il s’agit toujours de l’ordre (dit usuel) défini dans III, p. 24, sauf mention expresse du contraire.

#### Définition 2 {#ens-iii-s6-def-2 .statement tag=03MX}

On appelle suite (resp. suite d’éléments d’un ensemble E) une famille (resp. une famille d’éléments de E) dont l’ensemble d’indices est une partie de N; la suite est dite infinie si son ensemble d’indices est une partie infinie de N.

Soit P\{n\} une relation; notons I l’ensemble des entiers n tels que P\{n\} soit vraie, qui est donc une partie de N; une suite $(x_n)_{n \in I}$ se note souvent $(x_n)_{P\{n\}}$; on dit que $x_n$ est le terme d’indice n de la suite. Une suite dont l’ensemble d’indices est l’ensemble des entiers $n \geq k$ se note souvent $(x_n)_{k \leq n}$ ou $(x_n)_{n \geq k}$, ou même $(x_n)$ lorsque $k = 0$ ou $k = 1$. Dans les mêmes conditions, pour désigner, par exemple, le produit de la suite d’ensembles $(X_n)_{n \in I}$, on utilise les notations $\prod_{P\{n\}} X_n$ et $\prod_{n = k}^\infty X_n$; notations analogues pour la réunion, l’intersection, la somme cardinale et le produit cardinal.

Toute sous-famille d’une suite est une suite, qu’on dit extraite de la suite considérée.

On dit que deux suites $(x_n)_{n \in I}, (y_n)_{n \in I}$ ayant même ensemble d’indices ne diffèrent que par l’ordre des termes s’il existe une permutation $f$ de l’ensemble d’indices $I$ telle que l’on ait $x_{f(n)} = y_n$ pour tout $n \in I$.

On appelle suite multiple une famille dont l’ensemble d’indices est une partie d’un produit $\mathbf{N}^p$ ($p$ entier) (on dit encore « suite $p$-uple », « suite double » pour $p = 2$, « suite triple » pour $p = 3$, etc.).

Soient $I$ un ensemble équipotent à $\mathbf{N}$, $f$ une bijection de $\mathbf{N}$ sur $I$. Pour toute famille $(x_i)_{i \in I}$ ayant $I$ pour ensemble d’indices, la suite $n \mapsto x_{f(n)}$ est dite obtenue en rangeant dans l’ordre défini par $f$ la famille $(x_i)_{i \in I}$. Les suites correspondant ainsi à deux bijections distinctes de $\mathbf{N}$ sur $I$ ne diffèrent que par l’ordre des termes. Pour une famille finie ayant un ensemble d’indices $I$ à $n$ éléments, on définit de même une suite finie ayant pour ensemble d’indices $[1, n]$ ou $[0, n - 1]$ en rangeant la famille dans l’ordre défini par une bijection de $I$ sur l’un des intervalles précédents.

### 2. Définition d’applications par récurrence

L’ensemble $\mathbf{N}$ étant bien ordonné, on peut lui appliquer le critère C60 (III, p. 18), qui s’écrit ici (avec les mêmes notations):

C62. Soient $u$ une lettre, $T\{u\}$ un terme. Il existe un ensemble $U$ et une application $f$ de $\mathbf{N}$ sur $U$ tels que, pour tout entier $n$, on ait $f(n) = T\{f^{(n)}\}$, en désignant par $f^{(n)}$ l’application de $[0, n[$ sur $f([0, n[)$ qui coïncide avec $f$ dans $[0, n[$. L’ensemble $U$ et l’application $f$ sont alors déterminés de façon unique par cette condition.

Nous allons en déduire le critère suivant:

C63. Soient $S\{v\}$ et $a$ deux termes. Il existe un ensemble $V$ et une application $f$ de $\mathbf{N}$ sur $V$ tels que l’on ait $f(0) = a$ et, pour tout entier $n \geqslant 1$, $f(n) = S\{f(n - 1)\}$. En outre, l’ensemble $V$ et l’application $f$ sont déterminés de façon unique par ces conditions.

Pour déduire C63 de C62,$^1$ convenons, pour toute lettre $u$, de poser

$$
D(u) = \mathcal{E}_x(x \in \mathbf{N} \text{ et } (\exists y)((x, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))))
$$

Lorsque $u$ est une application d’une partie de $\mathbf{N}$ dans un ensemble, $D(u)$ n’est donc pas autre chose que l’ensemble de définition de $u$ (II, p. 10). Soit $M(u)$ la borne supérieure de $D(u)$ dans $\mathbf{N}.$^2 Soit $\varphi$ l’application vide (ayant $\varnothing$ comme ensemble de départ et ensemble d’arrivée, autrement dit (II, p. 14) le triplet $(\varnothing, \varnothing, \varnothing)$); considérons la relation

$$(u = \varphi \text{ et } y = a) \text{ ou } (u \neq \varphi \text{ et } y = S\{u(M(u))\})$$

que nous désignerons par $R\{y, u\}$; enfin, soit $T\{u\}$ le terme $\tau_y(R\{y, u\})$. Appliquons

$1$ On pourrait aussi démontrer C63 directement, par un raisonnement analogue à la démonstration de C60 (III, p. 18).
$2$ La définition de la borne supérieure (III, p. 10) peut être formulée de telle sorte qu’elle garde un sens même pour un ensemble non majoré (elle désigne un terme du langage formalisé de la forme $\tau_x(R\{x\}),$ que le lecteur explicitera sans peine).

le critère C62 au terme T$$u$$; comme $f^{(0)}$ est égal à $\varphi$, on a $T[f^{(0)}] = a$, donc $f(0) = a$; si au contraire $n > 0$, on a $D(f^{(n)}) = \{0, n - 1\}$ et $M(f^{(n)}) = n - 1$, d'où $T[f^{(n)}] = S[f^{(n)}(n - 1)] = S[f(n - 1)]$.

*Exemples*

1) Supposons que $a$ soit un élément d'un ensemble $E$ et $S[u]$ le terme $g(u)$, où $g$ est une application de $E$ dans lui-même.$^1$ Alors, on voit aussitôt par récurrence sur $n$ que, pour tout $n \in \mathbf{N}$, on a $f(n) \in E$; $f$ est par suite une application de $\mathbf{N}$ dans $E$ telle que $f(0) = a$ et $f(n + 1) = g(f(n))$ pour tout entier $n$.

De même, soit $h$ une application de $\mathbf{N} \times E$ dans $E$, et soit $\psi$ l'application de $\mathbf{N} \times E$ dans lui-même définie par $\psi(n, x) = (n + 1, h(n, x))$. D'après ce qui précède, il existe une application $g = (\theta, f)$ de $\mathbf{N}$ dans $\mathbf{N} \times E$ et une seule telle que $g(0) = (0, a)$ et $g(n + 1) = \psi(g(n))$ pour tout $n$; on en conclut l'existence et l'unicité d'une application $f$ de $\mathbf{N}$ dans $E$ telle que $f(0) = a$ et $f(n + 1) = h(n, f(n))$ pour tout entier $n$.

2) Soient $X$ un ensemble, $E$ l'ensemble des applications de $X$ dans lui-même; soient $e$ l'application identique de $X$ dans lui-même, et $f$ un élément quelconque de $E$. Prenons pour $S[u]$ le terme $f \circ u$.$^2$ On voit, par application de C63, qu'il existe une application de $\mathbf{N}$ dans $E$ et une seule, notée $n \mapsto f^n$, telle que $f^0 = e$ et $f^{n+1} = f \circ f^n$. On dit que $f^n$ est la *n-ème itérée* de l'application $f$.

3) Si on prend pour $S[u]$ le terme $\mathfrak{P}(u)$, et pour $a$ un ensemble $E$, on voit de même qu'il existe une application, notée $n \mapsto \mathfrak{P}^n(E)$ de $\mathbf{N}$ dans un ensemble $V(E)$, telle que $\mathfrak{P}^0(E) = E$, $\mathfrak{P}^1(E) = \mathfrak{P}(E)$ et $\mathfrak{P}^{n+1}(E) = \mathfrak{P}(\mathfrak{P}^n(E))$ pour tout entier $n$.

#### Remarque {#ens-iii-s6-n2-rem-1 .statement tag=03MY}

Soient $E$ un ensemble, $A$ une partie de $E$, $g$ une application de $A$ dans $E$, $a$ un élément de $A$. Prenons pour $S[u]$ le terme $g(u)$. On peut appliquer le critère C63, qui prouve l'existence d'une application $f$ de $\mathbf{N}$ sur un ensemble $V$, telle que $f(0) = a$ et $f(n + 1) = g(f(n))$ pour tout entier $n$. Il peut se faire que $V \subset A$; sinon, soit $p$ le plus grand entier tel que $f(\{0, p\}) \subset A$; on a alors $f(p + 1) = g(p) \notin A$ et $g(g(p))$ est un terme dont on ne peut plus rien dire. Aussi considère-t-on dans ce cas que $f$ est définie seulement dans l'intervalle $[0, p + 1]$ (*récurrence limitée*).

### 3. Calcul sur les cardinaux infinis

#### Théorème 2 {#ens-iii-s6-thm-2 .statement tag=03MZ}

*Pour tout cardinal infini $a$, on a $a^2 = a$.* Nous utiliserons deux lemmes.

#### Lemme 1 {#ens-iii-s6-lem-1 .statement tag=03N0}

*Tout ensemble infini $E$ contient un ensemble équipotent à $\mathbf{N}$.* Il existe sur $E$ une relation de bon ordre (III, p. 20, th. 1) que nous noterons $x \leq y$. L'hypothèse entraîne que l'ensemble bien ordonné $E$ ne peut être isomorphe à un segment de $\mathbf{N}$ distinct de $\mathbf{N}$, car un tel segment est de la forme

$1$ Si $g = (G, E, E)$, le terme $g(u)$ est le terme désigné par $\tau_y((u, y) \in G)$.

$2$ Il s'agit ici du terme désigné par $(T, X, X)$, $T$ étant le terme désigné par $\{z \mid z \text{ est un couple et } (\exists y)((pr_1 z, y) \in pr_1(pr_1(u)) \text{ et } (y, pr_2z) \in pr_1(pr_1(f)))\}$.

(0, n) (III, p. 16, prop. 1), donc est fini (III, p. 38, prop. 5). Il en résulte que $\mathbf{N}$ est isomorphe à un segment de E (III, p. 21, th. 3), d'où le lemme.

#### Lemme 2 {#ens-iii-s6-lem-2 .statement tag=03N1}

L'ensemble $\mathbf{N} \times \mathbf{N}$ est équipotent à $\mathbf{N}$.

Comme $\mathbf{N} \times \mathbf{N}$ contient l'ensemble $\{0\} \times \mathbf{N}$, équipotent à $\mathbf{N}$, on a Card ($\mathbf{N}$) $\leqslant$ Card ($\mathbf{N} \times \mathbf{N}$). D'autre part, nous allons définir une injection $f$ de $\mathbf{N} \times \mathbf{N}$ dans $\mathbf{N}$. Pour cela, remarquons qu'il existe une injection $\varphi$ de $\mathbf{N}$ dans l'ensemble des applications de $\mathbf{N}$ dans $I = \{0, 1\}$, obtenue comme suit : si $r$ est le plus petit entier tel que $n < 2^r$, et $\sum_{k=0}^{r-1} \varepsilon_k 2^{r-k-1}$ le développement dyadique de $n$ (III, p. 41), $\varphi(n)$ est la suite $(u_m)_{m \in \mathbf{N}}$ telle que $u_m = \varepsilon_{r-m-1}$ pour $m < r$ et $u_m = 0$ pour $m \geqslant r$; la prop. 8 de III, p. 40 montre que $\varphi$ est injective. Cela étant, pour tout couple $(n, n') \in \mathbf{N} \times \mathbf{N}$, nous définirons $f(n, n')$ de la façon suivant : si $\varphi(n) = (u_m)$ et $\varphi(n') = (v_m)$, $f(n, n')$ sera l'entier $s$ tel que $\varphi(s) = (w_m)$, où $w_{2m} = u_m$ et $w_{2m+1} = v_m$ pour tout $m \in \mathbf{N}$; il est clair que la relation $f(n, n') = f(n_1, n'_1)$ entraîne $\varphi(n) = \varphi(n_1)$ et $\varphi(n') = \varphi(n'_1)$ donc $(n, n') = (n_1, n'_1)$, ce qui prouve que $f$ est injective. On a par suite Card ($\mathbf{N} \times \mathbf{N}$) $\leqslant$ Card ($\mathbf{N}$), ce qui achève de démontrer le lemme.

Ces lemmes étant établis, soit E un ensemble tel que Card (E) = $\alpha$. Soit D une partie de E équipotente à $\mathbf{N}$ (lemme 1) ; il existe une application bijective $\psi_0$ de D sur D $\times$ D (lemme 2). Soit $\mathfrak{M}$ l'ensemble des couples $(X, \psi)$, où X est une partie de E contenant D, et $\psi$ une application bijective de X sur X $\times$ X prolongeant $\psi_0$. Ordonnons l'ensemble $\mathfrak{M}$ par la relation

« $X \subset X'$ et $\psi'$ est un prolongement de $\psi$ »

entre $(X, \psi)$ et $(X', \psi')$ ; on vérifie aussitôt que $\mathfrak{M}$ est un ensemble *inductif* (cf. III, p. 20, *Exemple* 2). Il existe donc dans $\mathfrak{M}$ un élément maximal (F, f) en vertu de III, p. 20, th. 2. Montrons que Card (F) = $\alpha$, ce qui démontrera le théorème. Dans le cas contraire, comme $b = \mathrm{Card}(F)$ est tel que $b = b^2$ et est infini, on a $b \leqslant 2b \leqslant 3b \leqslant b^2 = b$ (III, p. 30, prop. 14), donc $2b = b$ et $3b = b$. De l'hypothèse $b < \alpha$, il résulte que Card (E - F) > $b$, car dans le cas contraire, on aurait Card (E) $\leqslant 2b = b$, et on a supposé $b < \mathrm{Card}(E)$. Il existe donc une partie $Y \subset E - F$ équipotente à F ; posons $Z = F \cup Y$, et montrons qu'il existe une bijection g de Z sur Z $\times$ Z qui prolonge f. On a en effet

$$
Z \times Z = (F \times F) \cup (F \times Y) \cup (Y \times F) \cup (Y \times Y).
$$

et les quatre ensembles dont le second membre est réunion sont deux à deux disjoints ; comme F et Y sont équipotents, on a

$$
\mathrm{Card}(F \times Y) = \mathrm{Card}(Y \times F) = \mathrm{Card}(Y \times Y) = b^2 = b,
$$

d'où

$$
\mathrm{Card}((F \times Y) \cup (Y \times F) \cup (Y \times Y)) = 3b = b.
$$

Il y a donc une application bijective $f_1$ de $Y$ sur l’ensemble
$$
(F \times Y) \cup (Y \times F) \cup (Y \times Y);
$$
l’application $g$ de $Z$ dans $Z \times Z$ égale à $f$ dans $F$ et à $f_1$ dans $Y$ est alors une bijection qui prolonge $f$, ce qui est contraire à la définition de $f$.

#### Corollaire 1 {#ens-iii-s6-lem-2-cor-1 .statement}

*Si $a$ est un cardinal infini, on a $a^n = a$ pour tout entier $n \geqslant 1$.*
C’est évident par récurrence sur $n$.

#### Corollaire 2 {#ens-iii-s6-lem-2-cor-2 .statement}

*Le produit d’une famille finie $(\alpha_i)_{i \in I}$ de cardinaux non nuls, dont le plus grand est un cardinal infini $\alpha$, est égal à $\alpha$.*
Soit $b$ ce produit, et soit $n$ le nombre d’éléments de $I$; on a $b \leqslant \alpha^n = \alpha$ (III, p. 30, prop. 14); d’autre part, comme $\alpha_i \geqslant 1$ pour tout $i$, on a $b \geqslant \alpha$ (III, p. 30, prop. 14).

#### Corollaire 3 {#ens-iii-s6-lem-2-cor-3 .statement}

*Soient $a$ un cardinal infini, et $(\alpha_i)_{i \in I}$ une famille de cardinaux $\leqslant a$ dont l’ensemble d’indices $I$ ait un cardinal $\leqslant a$. On a alors $\sum_{i \in I} \alpha_i \leqslant a$; en outre, si $\alpha_i = a$ pour un indice $i$ au moins, $\sum_{i \in I} \alpha_i = a$.*
Soit $b$ le cardinal de $I$; on a alors $\sum_{i \in I} \alpha_i \leqslant ab \leqslant a^2 = a$ (III, p. 30, prop. 14) et $\sum_{i \in I} \alpha_i \geqslant \alpha_\kappa$ pour tout $\kappa \in I$.

#### Corollaire 4 {#ens-iii-s6-lem-2-cor-4 .statement}

*Si $a$ et $b$ sont deux cardinaux non nuls dont l’un est infini, on a $ab = a + b = \sup(a, b)$.*
Cela résulte aussitôt des cor. 2 et 3.

### 4. Ensembles dénombrables

#### Définition 3 {#ens-iii-s6-def-3 .statement tag=03N6}

*On dit qu’un ensemble est dénombrable s’il est équipotent à une partie de l’ensemble $\mathbf{N}$ des entiers.*

#### Proposition 1 {#ens-iii-s6-prop-1 .statement tag=03N7}

*Toute partie d’un ensemble dénombrable est dénombrable. Le produit d’une famille finie d’ensembles dénombrables est dénombrable. La réunion d’une suite d’ensembles dénombrables est dénombrable.*
La première assertion est évidente. Les autres résultent des corollaires du th. 2 (III, p. 47 et 49).

On a déjà vu (III, p. 48, lemme 1) que, pour tout cardinal infini $a$, on a $\mathrm{Card}(\mathbf{N}) \leqslant a$. On en déduit les conséquences suivantes:

#### Proposition 2 {#ens-iii-s6-prop-2 .statement tag=03N8}

*Tout ensemble infini dénombrable $E$ est équipotent à $\mathbf{N}$.*
En effet, on a $\mathrm{Card}(E) \leqslant \mathrm{Card}(\mathbf{N})$ par définition, et comme $E$ est infini, $\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(E)$.

#### Proposition 3 {#ens-iii-s6-prop-3 .statement tag=03N9}

Tout ensemble infini E admet une partition $(X_i)_{i \in I}$ formée d'ensembles infinis dénombrables $X_i$, l'ensemble d'indices I étant équipotent à E.
On a en effet Card(E) = Card(E)Card(\mathbf{N}) (III, p. 49, cor. 4).

#### Proposition 4 {#ens-iii-s6-prop-4 .statement tag=03NA}

Soit f une application d'un ensemble E sur un ensemble infini F, telle que, pour tout $y \in F$, $f^{-1}(y)$ soit dénombrable. Alors F est équipotent à E.
En effet, les $f^{-1}(y)$ ($y \in F$) forment une partition de E, donc
$$
\text{Card}(E) \leq \text{Card}(F)\text{Card}(\mathbf{N}) = \text{Card}(F);
$$
on sait d'autre part que $\text{Card}(F) \leq \text{Card}(E)$ (III, p. 25, prop. 3).

#### Proposition 5 {#ens-iii-s6-prop-5 .statement tag=03NB}

L'ensemble $\mathfrak{F}(E)$ des parties finies d'un ensemble infini E est équipotent à E.
Pour tout entier n, notons $\mathfrak{F}_n$ l'ensemble des parties à n éléments de E. Pour tout $X \in \mathfrak{F}_n$, il existe une bijection de $\{1, n\}$ sur X, donc le cardinal de $\mathfrak{F}_n$ est au plus égal à celui de l'ensemble des applications de $\{1, n\}$ dans E, c'est-à-dire à $\text{Card}(E^n) = \text{Card}(E)$ (III, p. 49, cor. 1). Donc
$$
\text{Card}(\mathfrak{F}(E)) = \sum_{n \in \mathbf{N}} \text{Card}(\mathfrak{F}_n) \leq \text{Card}(E)\text{Card}(\mathbf{N}) = \text{Card}(E).
$$
D'autre part, comme $x \mapsto \{x\}$ est une application injective de E dans $\mathfrak{F}(E)$, on a $\text{Card}(E) \leq \text{Card}(\mathfrak{F}(E))$.

#### Corollaire {#ens-iii-s6-n4-cor-1 .statement}

L'ensemble S des suites finies d'éléments d'un ensemble infini E est équipotent à E.
En effet, S est la réunion des $E^I$, où I parcourt l'ensemble $\mathfrak{F}(\mathbf{N})$ des parties finies de $\mathbf{N}$. Or, pour $I \in \mathfrak{F}(\mathbf{N})$ et $I \neq \varnothing$, $E^I$ est équipotent à E, et $\mathfrak{F}(\mathbf{N})$ est dénombrable en vertu de la prop. 5. On a donc
$$
\text{Card}(E) \leq \text{Card}(S) \leq \text{Card}(E)\text{Card}(\mathbf{N}) = \text{Card}(E).
$$

#### Définition 4 {#ens-iii-s6-def-4 .statement tag=03NC}

On dit qu'un ensemble a la puissance du continu s'il est équipotent à l'ensemble des parties de $\mathbf{N}$.

Un ensemble qui a la puissance du continu n'est pas dénombrable (III, p. 30, th. 2).

\* Le nom de « puissance du continu » provient de ce que l'ensemble des nombres réels est équipotent à $\mathfrak{P}(\mathbf{N})$ (TG, IV, § 8).* L'hypothèse du continu est l'assertion que tout ensemble non dénombrable contient une partie ayant la puissance du continu; l'hypothèse du continuum généralisée est l'assertion que, pour tout cardinal infini $\alpha$, tout cardinal $> \alpha$ est $\geq 2^\alpha$. Un théorème de métamathématique (Gödel–P.Cohen) affirme que ni ces assertions, ni leurs négations, ne peuvent être démontrées dans la théorie des ensembles telle qu'elle a été définie dans cet ouvrage (II, p. 1).

### 5. Suites stationnaires

#### Définition 5 {#ens-iii-s6-def-5 .statement tag=03ND}

On dit qu'une suite $(x_n)_{n \in \mathbf{N}}$ d'éléments d'un ensemble E est stationnaire s'il existe un entier m tel que $x_n = x_m$ pour tout entier $n \geq m$.

#### Proposition 6 {#ens-iii-s6-prop-6 .statement tag=03NE}

Soit E un ensemble ordonné. Les propositions suivantes sont équivalentes:
a) Toute partie non vide de E a un élément maximal.
b) Toute suite croissante $(x_n)$ d’éléments de E est stationnaire.

Montrons d’abord que a) entraîne b); en effet, soit X l’ensemble des éléments de la suite $(x_n)$, et soit $x_m$ un élément maximal de X; pour $n \geq m$, on a par hypothèse $x_n \geq x_m$, d’où $x_n = x_m$ par définition de $x_m$. Réciproquement, supposons qu’il existe une partie non vide A de E n’ayant pas d’élément maximal; pour tout $x \in A$, soit $T_x$ l’ensemble des $y \in A$ tels que $y > x$. Par hypothèse, $T_x \neq \varnothing$ pour tout $x \in A$, donc il existe une application $f$ de A dans A telle que $f(x) > x$ pour tout $x \in A$ (II, p. 34, prop. 6); si $a \in A$, et si la suite $(x_n)_{n \in \mathbf{N}}$ est définie par récurrence par les conditions $x_0 = a$, $x_{n+1} = f(x_n)$, il est clair que cette suite est croissante et non stationnaire.

#### Corollaire 1 {#ens-iii-s6-prop-6-cor-1 .statement tag=03NF}

Pour qu’un ensemble totalement ordonné E soit bien ordonné, il faut et il suffit que toute suite décroissante d’éléments de E soit stationnaire.

En effet, dire que E est bien ordonné revient à dire que toute partie non vide de E admet un élément minimal (III, p. 13, prop. 10), et notre assertion résulte alors de la prop. 6.

#### Corollaire 2 {#ens-iii-s6-prop-6-cor-2 .statement tag=03NG}

Toute suite croissante d’éléments d’un ensemble ordonné fini est stationnaire.

En effet, tout ensemble ordonné fini admet un élément maximal (III, p. 34, cor. 2).

On dit parfois qu’un ensemble ordonné E vérifiant les conditions équivalentes de la prop. 6 est nœthérien (pour la relation $\leq$).

#### Proposition 7 (« principe de récurrence nœthérienne ») {#ens-iii-s6-prop-7 .statement tag=03RM}

Soient E un ensemble nœthérien, F une partie de E ayant la propriété suivante: si $a \in E$ est tel que la relation $x > a$ entraîne $x \in F$, alors $a \in F$. Dans ces conditions, on a $F = E$.

En effet, supposons $E \neq F$; alors $E - F$ aurait un élément maximal $b$. Par définition, on a $x \in F$ pour tout $x > b$; mais cela entraîne $b \in F$, ce qui est absurde.

## EXERCICES {#ens-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
