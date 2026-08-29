---
book: alg
book_title: Algebra
chapter: VII
chapter_title: Modules sur les anneaux principaux
section: 2
section_title: MODULES DE TORSION SUR UN ANNEAU PRINCIPAL
lang: fr
source: alg-iv-vii-fr
book_pages: A VII.6-A VII.13, A VII.53-A VII.57
pdf_pages: 0339-0346, 0386-0390
extraction: ocr
subsections:
    - "no": 1
      title: Modules sur un produit d’anneaux
      page: 6
      pdf_page: 339
    - "no": 2
      title: Décomposition canonique d’un module de torsion sur un anneau principal
      page: 7
      pdf_page: 340
statements: 24
exercises: 14
content_sha256: e8c67551fee721ba16eb39a2353408561379f3cf1ddfac653b03c1b284c8cb26
---

## § 2. MODULES DE TORSION SUR UN ANNEAU PRINCIPAL

### 1. Modules sur un produit d’anneaux

Soient A un anneau et $(b_i)_{i \in I}$ une décomposition directe de A, c’est-à-dire (I, p. 105, déf. 7) une famille finie d’idéaux bilatères de A telle que l’homomorphisme canonique de A dans le produit des $A/b_i$ soit bijectif. D’après *loc. cit.*, prop. 10, il existe une famille $(e_i)_{i \in I}$ d’idempotents centraux de A tels que $b_i = A(1 - e_i)$, $\sum_{i \in I} e_i = 1$ et $e_i e_j = 0$ pour $i \neq j$.

Pour tout A-module à gauche M, notons $M_i$ l’ensemble des $m \in M$ tels que $b_i m = 0$; comme $b_i$ est un idéal bilatère, c’est un sous-module de M ; de plus, si $a, b \in A$ et $a - b \in b_i$, les homothéties $a_{M_i}$ et $b_{M_i}$ coïncident ; il existe donc une unique structure de $A/b_i$-module sur $M_i$ telle que la structure de A-module de $M_i$ s’en déduise par l’homomorphisme $A \to A/b_i$.

#### Proposition 1 {#alg-vii-s2-prop-1 .statement}

*Le A-module M est somme directe de ses sous-modules $M_i$.*

Notons $p_i : M \to M$ l’homothétie $m \mapsto e_i m$; comme $e_i$ est central, $p_i$ est A-linéaire ; comme $e_i^2 = e_i$, $\sum_{i \in I} e_i = 1$, et $e_i e_j = 0$ pour $i \neq j$, on a

$$
p_i \circ p_i = p_i,\quad \sum_{i \in I} p_i = 1_M,\quad p_i \circ p_j = 0 \text{ pour } i \neq j,
$$

et les $p_i$ forment une famille orthogonale de projecteurs de somme l’identité (II, p. 18, déf. 7). D’après *loc. cit.*, prop. 12, M est somme directe des sous-modules $p_i(M) = e_i M$. Par ailleurs $e_i M$ est annulé par $b_i = A(1 - e_i)$; si $i \neq j$ et $m \in M$, on a $(1 - e_i) e_j m = e_j m$, de sorte qu’aucun élément non nul de $e_j M$ n’est annulé par $1 - e_i$ et *a fortiori* par $b_i$. Il s’ensuit que $e_i M = M_i$, d’où la proposition.

#### Remarque 1 {#alg-vii-s2-n1-rem-1 .statement}

Inversement, donnons-nous pour chaque $i$ un $A/b_i$-module $M'_i$, et considérons le A-module M somme directe des A-modules $M'_i$; alors les sous-modules $M_i$ construits ci-dessus coïncident avec les $M'_i$ (il suffit de noter que, si i ≠ j, aucun élément non nul de M_j n’est annulé par b_i puisque b_i + b_j = A). En termes imagés, il revient donc au même de se donner un A-module M ou une famille (M_i) de modules sur les anneaux A/b_i = A_i.

#### Remarque 2 {#alg-vii-s2-n1-rem-2 .statement}

D’après la démonstration précédente, les projecteurs de M sur ses composants M_i sont des homothéties.

#### Remarque 3 {#alg-vii-s2-n1-rem-3 .statement}

Pour que le A-module M soit monogène, il faut et il suffit que chacun des M_i le soit : si M = Am, alors M_i = A_i e_i m ; inversement, si M_i = A_i m_i, et si m = $\sum_{i \in I} m_i$, alors M = Am ; en effet, si n ∈ M se projette sur a_i m_i pour chaque i, et si a ∈ A est congru à a_i mod. b_i pour chaque i, am et n ont même projection sur chaque M_i, donc coïncident.

#### Remarque 4 {#alg-vii-s2-n1-rem-4 .statement}

Soient M et N deux A-modules, (M_i) et (N_i) leurs composants. Soit u ∈ Hom_A(M, N) une application A-linéaire de M dans N ; pour tout i et tout m ∈ M_i, on a u(m) ∈ N_i, d’où une application A_i-linéaire u_i ∈ Hom_{A_i}(M_i, N_i). On vérifie aussitôt que l’application u ↦ (u_i) est un isomorphisme de Z-modules (resp. de A-modules lorsque A est commutatif)

$$
\operatorname{Hom}_A(M, N) \to \prod_{i \in I} \operatorname{Hom}_{A_i}(M_i, N_i)
$$

### 2. Décomposition canonique d’un module de torsion sur un anneau principal

Soit M un module sur un anneau commutatif A. Pour tout α ∈ A, nous noterons M(α) le noyau de l’endomorphisme x ↦ αx de M. Si α et β sont deux éléments de A tels que α divise β, il est clair que M(α) ⊂ M(β). En particulier, lorsque n parcourt l’ensemble des entiers rationnels ≥ 1, les sous-modules M(α^n) forment une suite croissante ; la réunion M_α des M(α^n) est donc un sous-module de M, formé des éléments de M qui sont annulés par une puissance de α. Pour tout sous-module N de M, il est clair que N_α = N ∩ M_α.

#### Définition 1 {#alg-vii-s2-def-1 .statement}

Soit π un élément extrémal d’un anneau principal A ; on dit qu’un A-module M est π-primaire si, pour tout x ∈ M, il existe un entier n ≥ 1 tel que π^n x = 0 (en d’autres termes, si M est égal au sous-module M_π).

Il est clair que tout module monogène de la forme A/(π^s) est π-primaire. Pour un A-module quelconque M, le sous-module M_π est π-primaire.

#### Lemme 1 {#alg-vii-s2-lem-1 .statement}

Soit M un module sur un anneau principal A ; pour tout α ∈ A tel que α ≠ 0, soit α = ε $\prod_{i=1}^r \pi_i^{n(i)}$ une décomposition de α en facteurs extrémaux (VII, p. 3).

Le sous-module N = M(α) des éléments de M annulés par α est somme directe des sous-modules M(π_i^{n(i)}), et l’application qui, à tout x ∈ M(α), fait correspondre son composant dans M(π_i^{n(i)}), est de la forme x ↦ γ_i x (γ_i ∈ A). En outre, on a

$$
M(\pi_i^{n(i)}) = N \cap M_{\pi_i} = N_{\pi_i}.
$$

Notons d’abord que N est annulé par α, donc muni d’une structure naturelle de A/(α)-module. D’après la prop. 4 de VII, p. 3, l’homomorphisme canonique de $A/(\alpha)$ dans le produit des anneaux $A/(\pi_i^{n(i)})$ est un isomorphisme d’anneaux ; appliquant alors la prop. 1 de VII, p. 6, on en déduit que $N$ est somme directe des $M(\pi_i^{n(i)})$; les projecteurs de cette décomposition sont des homothéties d’après VII, p. 7, remarque 2. L’inclusion $M(\pi_i^{n(i)}) \subset M(\alpha) \cap M_{\pi_i}$ est évidente ; inversement, soit $x \in M(\alpha) \cap M_{\pi_i}$. Il existe une puissance $\pi_i^s$ de $\pi_i$ qui annule $x$; on peut supposer $s \geq n(i)$; d’après l’identité de Bezout, il existe $\lambda, \mu \in A$ tels que $\pi_i^{n(i)} = \lambda \pi_i^s + \mu \alpha$, donc $\pi_i^{n(i)} x = 0$ et finalement $x \in M(\pi_i^{n(i)})$.

#### Lemme 2 {#alg-vii-s2-lem-2 .statement}

Soit $M$ un module de torsion (II, p. 115) sur un anneau intègre $A$. Pour toute famille finie $(x_i)_{1 \leq i \leq n}$ d’éléments de $M$, il existe un élément $\gamma \neq 0$ dans $A$ tel que les $x_i$ appartiennent tous à $M(\gamma)$.

En effet, pour chaque indice $i$, il existe un élément $\alpha_i \neq 0$ dans $A$ qui annule $x_i$; l’élément $\gamma = \prod_{i=1}^n \alpha_i$ répond à la question.

#### Théorème 1 {#alg-vii-s2-thm-1 .statement}

Soit $M$ un module de torsion sur un anneau principal $A$; pour tout élément extrémal $\pi$ de $A$, soit $M_\pi$ le sous-module de $M$ formé des éléments annulés par une puissance de $\pi$. Si $P$ est un système représentatif d’éléments extrémaux de $A$, $M$ est somme directe des sous-modules $M_\pi$, pour $\pi \in P$.

Tout élément $x \in M$ appartient à un sous-module $M(\alpha)$ pour un $\alpha \neq 0$, donc, en vertu du lemme 1 est somme d’un nombre fini d’éléments dont chacun appartient à un sous-module $M_\pi$. D’autre part, si l’on a $\sum_{\pi \in P} x_\pi = \sum_{\pi \in P} y_\pi$, où $x_\pi \in M_\pi$ et $y_\pi \in M_\pi$ pour tout $\pi \in P$ et où les $x_\pi$ et $y_\pi$ sont nuls sauf un nombre fini d’entre eux, le lemme 2 montre qu’il existe $\gamma \neq 0$ dans $A$ tel que les $x_\pi$ et $y_\pi$ appartiennent à un même sous-module $M(\gamma)$; l’application du lemme 1 à $M(\gamma)$ montre que $x_\pi = y_\pi$ pour tout $\pi \in P$, ce qui achève la démonstration.

Il est clair que, si $\pi$ et $\pi'$ sont deux éléments extrémaux associés, on a $M_\pi = M_{\pi'}$; pour un module donné $M$, le sous-module $M_\pi$ ne dépend donc que de l’idéal $(\pi)$ de $A$; on dit que c’est le composant $\pi$-primaire du module $M$, et la décomposition de $M$ en somme directe des $M_\pi$ est appelée la décomposition canonique de $M$ en somme directe de ses composants $\pi$-primaires.

#### Corollaire 1 {#alg-vii-s2-thm-1-cor-1 .statement}

Tout sous-module $N$ d’un module de torsion $M$ est somme directe des sous-modules $N \cap M_\pi$.

Cela résulte de ce que $N \cap M_\pi$ est le composant $\pi$-primaire $N_\pi$ de $N$.

#### Corollaire 2 {#alg-vii-s2-thm-1-cor-2 .statement}

Pour que le sous-module $N$ du $A$-module de torsion $M$ soit facteur direct, il faut et il suffit que $N_\pi$ soit facteur direct dans $M_\pi$ pour tout élément extrémal $\pi$ de $A$.

En effet, si $N$ et $N'$ sont deux sous-modules de $M$, on a $M = N \oplus N'$ si et seulement si $M_\pi = N_\pi \oplus N'_\pi$ pour tout élément extrémal $\pi$ de $A$ (cor. 1).

#### Corollaire 3 {#alg-vii-s2-thm-1-cor-3 .statement}

Soit $N$ un sous-module du $A$-module de torsion $M$. Si, pour tout élément extrémal $\pi$ de $A$, on a, soit $N_{\pi} = 0$, soit $(M/N)_{\pi} = 0$, alors $N$ est facteur direct dans $M$.

En effet, la condition $(M/N)_{\pi} = 0$ implique $N_{\pi} = M_{\pi}$, et on applique le cor. 2.

On dit qu’un $A$-module $M$ est *semi-simple* si tout sous-module de $M$ est facteur direct (*cf.* A, VIII, § 4).

#### Corollaire 4 {#alg-vii-s2-thm-1-cor-4 .statement}

Soient $A$ un anneau principal qui n’est pas un corps, et $M$ un $A$-module. Alors $M$ est semi-simple si et seulement s’il est de torsion et si $M_{\pi} = M(\pi)$ pour tout élément extrémal $\pi$ de $A$.

Supposons d’abord $M$ semi-simple ; soit $x \in M$ et soit $\pi$ un élément extrémal de $A$. Si $N$ est un supplémentaire de $A\pi x$ dans $M$, on peut écrire $x = \alpha \pi x + y$, avec $\alpha \in A$ et $y \in N$; mais cela implique $y = (1 - \alpha \pi) x$, donc
$$
\pi(1 - \alpha \pi) x \in A\pi x \cap N = 0 .
$$
Il en résulte d’abord que $M$ est de torsion ; de plus, si $x \in M_{\pi}$, on a $\pi(1 - \alpha \pi) x = 0$ donc $\pi x = \alpha \pi^2 x = \alpha^2 \pi^3 x = \cdots = \alpha^n \pi^{n+1} x$ est nul et l’on a $M_{\pi} = M(\pi)$.

Inversement, il suffit, d’après le cor. 2, de prouver qu’un $A$-module $M$ annulé par un élément extrémal $\pi$ est semi-simple ; mais cela est clair, puisque $M$ est alors muni d’une structure naturelle d’espace vectoriel sur le corps $A/(\pi)$, et que les sous-modules de $M$ ne sont autres que les sous-espaces vectoriels de cette structure.

#### Remarque 1 {#alg-vii-s2-n2-rem-1 .statement}

Il est clair que l’annulateur de tout élément $\neq 0$ d’un module $\pi$-primaire est de la forme $A\pi^k$ ($k$ entier $> 0$), puisque c’est un idéal principal contenant une puissance de $\pi$. Soit $x$ un élément de $M$ ; pour chaque $\pi \in P$, soit $x_{\pi}$ le composant de $x$ dans $M_{\pi}$ ; l’annulateur de $x$ est le ppcm des annulateurs de ceux des $x_{\pi}$ qui sont $\neq 0$, mais en vertu de ce qui précède il est ici égal au *produit* des annulateurs des $x_{\pi} \neq 0$ (VI, p. 15, prop. 12 (DIV)).

#### Proposition 2 {#alg-vii-s2-prop-2 .statement}

Si $M$ est un module de torsion de type fini sur un anneau principal $A$, les composants $\pi$-primaires de $M$ sont nuls à l’exception d’un nombre fini d’entre eux, et les projections de $M$ sur ses composants $M_{\pi}$ sont des homothéties.

Cela résulte aussitôt du lemme 1, car, en vertu du lemme 2, il existe $\alpha \neq 0$ dans $A$ tel que $M = M(\alpha)$.

#### Remarque 2 {#alg-vii-s2-n2-rem-2 .statement}

D’après VII, p. 7, remarque 3, un $A$-module de torsion de type fini est monogène si et seulement si chacun de ses composants $\pi$-primaires l’est.

Un cas particulier important d’application du th. 1 et de la prop. 2 est celui où $A = \mathbf{Z}$ ; les $\mathbf{Z}$-modules ne sont autres que les *groupes commutatifs*. On dit qu’un groupe commutatif est un *groupe de torsion* si c’est un $\mathbf{Z}$-module de torsion, c’est-à-dire si tous ses éléments sont d’*ordre fini*. On prend alors pour $P$ l’ensemble des nombres premiers $> 0$ ; pour tout nombre premier $p > 0$, on dit qu’un groupe (commutatif) est de $p$-torsion si tous ses éléments ont pour ordre une puissance de $p$. Avec cette terminologie, le th. 1 montre que *tout groupe commutatif de torsion est somme directe de groupes de p-torsion*. Dans le cas des groupes finis, cela résulte aussi de I, p. 76, th. 4.

#### Remarque 3 {#alg-vii-s2-n2-rem-3 .statement}

Applications : I. Décomposition canonique des nombres rationnels et des fractions rationnelles à une indéterminée

#### Théorème 2 {#alg-vii-s2-thm-2 .statement}

Soient $A$ un anneau principal, $K$ son corps des fractions et $P$ un système représentatif d’éléments extrémaux de $A$. Étant donné un élément $x \in K$, il existe une partie finie $H$ de $P$, des éléments $a_0 \in A$ et $a_p \in A$ non multiple de $p$ dans $A$ ($p \in H$), et des entiers $s(p) > 0$ ($p \in H$) tels que

$$
x = a_0 + \sum_{p \in H} a_p p^{-s(p)},
$$

où $H$ et les $s(p)$ sont déterminés de façon unique par ces conditions.

Si de plus $R_p$ désigne une partie de $A$ contenant un élément et un seul de chaque classe de $A$ mod. $p$ ($p \in P$), tout $x \in K$ s’écrit, d’une manière et d’une seule, sous la forme

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} r_{ph} p^{-h} \right)
$$

où $a \in A$ et $r_{ph} \in R_p$ quels que soient $h$ et $p$, les $r_{ph}$ étant nuls sauf un nombre fini d’entre eux.

Considérons $K$ comme muni de sa structure de $A$-module ; alors $A$ est le sous-module de $K$ engendré par 1. Le module quotient $K/A$ est le quotient de $K$ par la relation d’équivalence $x' - x \in A$, qui, avec les notations de VI, p. 6, s’écrit aussi $x \equiv x'$ (mod. 1) ; nous noterons $f$ l’application canonique de $K$ sur $M = K/A$.

Le module quotient $M$ est un module de torsion, car tout élément de $M$ est de la forme $f(a/b)$ ($a \in A, b \in A, b \neq 0$), d’où $bf(a/b) = f(a) = 0$. On peut donc lui appliquer le th. 1 de VII, p. 8. Soit $M_p$ ($p \in P$) le sous-module des éléments de $M$ annulés par une puissance de $p$ ; alors $\overline{f}(M_p)$ est le sous-anneau $A_p$ des éléments de $K$ de la forme $ap^{-n}$ où $a \in A$ et où $n$ est un entier $\geqslant 0$. Le module $M$ étant somme directe des $M_p$, tout $x \in K$ est congru mod. 1 à un élément de la somme des $A_p$ ; en d’autres termes, on peut écrire la formule (1), où les $s(p)$ sont des entiers $> 0$, et les $a_p$ des éléments de $A$ en nombre fini tels que $a_p$ ne soit pas multiple de $p$.

Montrons que ces conditions sur les $s(p)$ et les $a_p$ déterminent complètement $H$ et les $s(p)$. En effet, $H$ est alors l’ensemble des $p \in P$ tels que le composant de $f(x)$ dans $M_p$ soit $\neq 0$. D’autre part si $s$ et $s'$ sont deux entiers $> 0$ tels que $s \geqslant s'$, $a$ et $a'$ des éléments de $A$ non multiples de $p$ tels que $ap^{-s} \equiv a'p^{-s'}$ (mod. 1) on en déduit que $a \equiv a'p^{s-s'}$ (mod. $p^s$) ; si l’on avait $s > s'$, on aurait $a \equiv 0$ (mod. $p$), contrairement à l’hypothèse. Ce raisonnement montre de plus que chaque $a_p$ est bien déterminé mod. $p^{s(p)}$.

Pour achever la démonstration, remarquons d’abord que, dans chaque classe de $A$ mod. $p^s$, il existe un élément et un seul de la forme $\sum_{h=0}^{s-1} r_h p^h$ avec $r_h \in R_p$ pour $0 \leqslant h \leqslant s-1$. Procédons en effet par récurrence sur $s$ (la propriété résultant de la définition de $R_p$ pour $s = 1$) : soit $x \in A$; dans la classe de $x$ mod. $p^{s-1}$ il existe par hypothèse, un élément et un seul de la forme $\sum_{h=0}^{s-2} r_h p^h$ ($r_h \in R_p$); alors $x - \sum_{h=0}^{s-2} r_h p^h$ est un multiple $ap^{s-1}$ de $p^{s-1}$; or il existe un élément $r_{s-1}$ et un seul de $R_p$ tel que $a \equiv r_{s-1}$ (mod. $p$); d’où $x \equiv \sum_{h=0}^{s-1} r_h p^h$ (mod. $p^s$). Il suffit alors d’appliquer ceci à chaque $a_p$ de la formule (1) pour obtenir la formule (2). L’unicité est évidente en vertu de ce qui précède.

Les cas les plus importants d’application du th. 2 sont les suivants :

I. *L’anneau A est l’anneau $\mathbf{Z}$ des entiers rationnels, et $K = \mathbf{Q}$*. On prend pour $P$ l’ensemble des nombres premiers $> 0$, et, pour tout $p \in P$, on prend pour $R_p$ l’intervalle $[0, p-1]$ de $\mathbf{Z}$. D’où la décomposition canonique

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} e_{ph} p^{-h} \right)
$$

où $a \in \mathbf{Z}$, $e_{ph} \in \mathbf{Z}$, $0 \leq e_{ph} \leq p-1$.

II. *L’anneau A est l’anneau $E[X]$ des polynômes à une indéterminée sur un corps commutatif $E$, et $K = E(X)$*. On prend pour $P$ l’ensemble des polynômes unitaires irréductibles de $E[X]$ (VII, p. 5). Pour $p \in P$, on peut, en vertu de la division euclidienne des polynômes (IV, p. 10), prendre pour $R_p$ l’ensemble des polynômes de degré strictement inférieur à celui de $p$. D’où la décomposition (dite canonique) d’une fraction rationnelle $r(X) \in E(X)$ :

$$
r(X) = a(X) + \sum_{p \in P} \left( \sum_{h=1}^{\infty} v_{ph}(X) \cdot p(X)^{-h} \right)
$$

où $a(X)$ est un polynôme, où $v_{ph}(X)$ est un polynôme de degré strictement inférieur à celui de $p(X)$, quels que soient $p$ et $h$. Si, en particulier, $E$ est un corps *algébriquement clos*, les $p(X)$ sont de la forme $X - \alpha$ avec $\alpha \in E$ (V, p. 19) et les $v_{ph}(X)$ sont donc des constantes.

On peut donc dire que l’espace vectoriel $E(X)$ sur le corps $E$ admet pour *base* l’ensemble formé des monômes $X^n$ (*n* entier $\geq 0$) et des fractions rationnelles de la forme $X^m/(p(X))^h$ où $p$ parcourt l’ensemble $P$, et où, pour chaque $p$, $h$ parcourt l’ensemble des entiers $\geq 1$, et $m$ l’ensemble des entiers tels que $0 \leq m < \deg(p)$.

#### Remarque 4 {#alg-vii-s2-n2-rem-4 .statement}

Applications : II. Groupe multiplicatif des entiers inversibles modulo $a$

Soit $a$ un entier rationnel $> 1$, et soit $(\mathbf{Z}/a\mathbf{Z})^*$ le groupe multiplicatif des éléments inversibles de l’anneau $\mathbf{Z}/a\mathbf{Z}$. Si $a = \prod_i p_i^{n(i)}$ est la décomposition de $a$ en facteurs premiers, l’anneau $\mathbf{Z}/a\mathbf{Z}$ est isomorphe au produit des anneaux $\mathbf{Z}/p_i^{n(i)}\mathbf{Z}$ (VII, p. 3, prop. 4), et le groupe $(\mathbf{Z}/a\mathbf{Z})^*$ isomorphe au produit des groupes $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$. Nous sommes ainsi ramenés à étudier les groupes $(\mathbf{Z}/p^n\mathbf{Z})^*$, où $p$ est un nombre premier ; rappelons (V, p. 77) que l’ordre $\varphi(p^n)$ de $(\mathbf{Z}/p^n\mathbf{Z})^*$ est $p^n - p^{n-1} = p^{n-1}(p-1)$.

Supposons d’abord $p > 2$; l’homomorphisme canonique $\mathbf{Z}/p^n\mathbf{Z} \to \mathbf{Z}/p\mathbf{Z}$ induit par passage aux sous-ensembles un homomorphisme de groupes de $(\mathbf{Z}/p^n\mathbf{Z})^*$ dans $(\mathbf{Z}/p\mathbf{Z})^*$, dont nous noterons le noyau $\mathrm{U}(p^n)$; d’après VII, p. 3, prop. 3, pour que la classe mod. $p^n$ d’un entier $m$ soit inversible, il faut et il suffit que $m$ soit étranger à $p$, c’est-à-dire que la classe de $m$ mod. $p$ soit inversible. On en déduit que $\mathrm{U}(p^n)$ est formé des classes mod. $p^n$ des entiers congrus à 1 mod. $p$, donc possède $p^{n-1}$ éléments, et qu’on a la suite exacte

(3)
$$
\{1\} \to \mathrm{U}(p^n) \to (\mathbf{Z}/p^n\mathbf{Z})^* \to (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}.
$$

De même, pour $n \geqslant 2$, on note $\mathrm{U}(2^n)$ le noyau de l’homomorphisme canonique de $(\mathbf{Z}/2^n\mathbf{Z})^*$ dans $(\mathbf{Z}/4\mathbf{Z})^*$; c’est un groupe à $2^{n-2}$ éléments, formé des classes mod. $2^n$ des entiers congrus à 1 mod. 4, et l’on a la suite exacte

(4)
$$
\{1\} \to \mathrm{U}(2^n) \to (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

#### Lemme 3 {#alg-vii-s2-lem-3 .statement}

*Soient $x, y$ des entiers, $k$ un entier $\geqslant 0$, et $p$ un nombre premier $> 2$. Si $x \equiv 1 + py$ mod. $p^2$, on a $x^{p^k} \equiv 1 + p^{k+1} y$ mod. $p^{k+2}$. Si $x \equiv 1 + 4y$ mod. 8, on a $x^{2^k} \equiv 1 + 2^{k+2}y$ mod. $2^{k+3}$.

Pour démontrer la première assertion, il suffit de prouver que si $k \geqslant 1$ et si $x \equiv 1 + p^k y$ mod. $p^{k+1}$, alors $x^p \equiv 1 + p^{k+1} y$ mod. $p^{k+2}$, et on conclura par récurrence sur l’entier $k$. Or on a aussitôt, pour $a \in \mathbf{Z}$ et $k \geqslant 1$,
$$
(1 + p^k a)^p \equiv 1 + p^{k+1} a \text{ mod. } p^{k+2},
$$
donc
$$
(1 + p^k y + p^{k+1} z)^p = (1 + p^k (y + pz))^p \equiv 1 + p^{k+1} (y + pz) \equiv 1 + p^{k+1} y \text{ mod. } p^{k+2}.
$$
De même, pour $k \geqslant 1$, on a $(1 + 2^{k+1} a)^2 \equiv 1 + 2^{k+2} a$ mod. $2^{k+3}$, donc
$$
(1 + 2^{k+1} y + 2^{k+2} z)^2 \equiv 1 + 2^{k+2} y \text{ mod. } 2^{k+3},
$$
d’où la deuxième assertion par récurrence sur $k$.

#### Proposition 3 {#alg-vii-s2-prop-3 .statement}

*Soient $p$ un nombre premier $> 2$ et $n$ un entier $> 0$; le groupe $\mathrm{U}(p^n)$ est cyclique d’ordre $p^{n-1}$; si $n \geqslant 2$, pour que la classe modulo $p^n$ d’un entier $x$ congru à 1 mod. $p$ soit un générateur de $\mathrm{U}(p^n)$, il faut et il suffit que $x$ ne soit pas congru à 1 mod. $p^2$. Soit $m$ un entier $> 1$; le groupe $\mathrm{U}(2^m)$ est cyclique d’ordre $2^{m-2}$; si $m \geqslant 3$, pour que la classe modulo $2^m$ d’un entier $x$ congru à 1 mod. 4 soit un générateur de $\mathrm{U}(2^m)$, il faut et il suffit que $x$ ne soit pas congru à 1 mod. 8.

Comme $\mathrm{U}(p^n)$ est d’ordre $p^{n-1}$, l’ordre de tout élément $u$ de $\mathrm{U}(p^n)$ est une puissance de $p$, et $u$ est un générateur de $\mathrm{U}(p^n)$ si et seulement si $u^{p^{n-2}} \neq 1$. Or, si $u$ est la classe de $x = 1 + py$, $u^{p^{n-2}}$ est d’après le lemme 3 la classe de $1 + p^{n-1} y$, de sorte que $u$ engendre $\mathrm{U}(p^n)$ si et seulement si $y \not\equiv 0$ mod. $p$, c’est-à-dire $x \not\equiv 1$ mod. $p^2$. Par exemple, la classe de $1 + p$ engendre $\mathrm{U}(p^n)$. De même, la classe $u$ de $x$ mod. $2^n$ engendre $\mathrm{U}(2^n)$ si et seulement si $u^{2^{n-3}} \neq 1$, ce qui d’après le lemme 3 signifie que $x$ n’est pas congru à 1 mod. 8 ; cela est vérifié pour $x = 5$.

#### Lemme 4 {#alg-vii-s2-lem-4 .statement}

Soient $A$ un anneau principal, et $0 \to N \to M \to P \to 0$ une suite exacte de $A$-modules. Supposons qu’il existe $a, b \in A$, étrangers, tels que $aN = 0$, $bP = 0$. Alors la suite exacte est scindée. Si de plus $N$ et $P$ sont monogènes, $M$ est monogène.

On a $abM = 0$, donc $M$ est de torsion. La première assertion résulte du cor. 3 de VII, p. 9. Si $N$ et $P$ sont monogènes, ils sont de type fini, ainsi par conséquent que $M$ (II, p. 17, cor. 5) ; comme les composants $p$-primaires de $M$ sont isomorphes à des composants $p$-primaires, soit de $N$, soit de $P$, $M$ est monogène d’après la remarque 2 de VII, p. 9.

#### Théorème 3 {#alg-vii-s2-thm-3 .statement}

Si $a = \prod_i p_i^{n(i)}$ est la décomposition en facteurs premiers de l’entier $a > 1$, le groupe $(\mathbf{Z}/a\mathbf{Z})^*$ des éléments inversibles de l’anneau $\mathbf{Z}/a\mathbf{Z}$ est isomorphe au produit des groupes $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$. Si $p$ est un nombre premier $> 2$, et $n$ un entier $\geqslant 1$, le groupe $(\mathbf{Z}/p^n\mathbf{Z})^*$ est cyclique d’ordre $p^{n-1}(p-1)$. Le groupe $(\mathbf{Z}/2\mathbf{Z})^*$ est réduit à l’élément neutre ; pour $n \geqslant 2$, le groupe $(\mathbf{Z}/2^n\mathbf{Z})^*$ est le produit direct du groupe cyclique d’ordre $2^{n-2}$ engendré par la classe de 5 mod. $2^n$ et du groupe cyclique d’ordre 2 formé des classes de 1 et $-1$ mod. $2^n$.

Les ordres $p^{n-1}$ de $U(p^n)$ et $p-1$ de $(\mathbf{Z}/p\mathbf{Z})^*$ sont étrangers ; comme $U(p^n)$ et $(\mathbf{Z}/p\mathbf{Z})^*$ sont cycliques (prop. 3 et V, p. 75, lemme 1), le groupe $(\mathbf{Z}/p^n\mathbf{Z})^*$ est cyclique (appliquer le lemme 4 à la suite exacte (3)). Si $n \geqslant 2$, la restriction de l’homomorphisme canonique $v : (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^*$ au sous-groupe $\{1, -1\}$ est bijectif ; le groupe $(\mathbf{Z}/2^n\mathbf{Z})^*$ est donc produit direct de ce sous-groupe et du noyau $U(2^n)$ de $v$; on conclut grâce à la prop. 3.

#### Remarque {#alg-vii-s2-n2-rem-5 .statement}

Soient $p$ un nombre premier $> 2$ et $x$ un entier congru à 1 mod. $p$ et non congru à 1 mod. $p^2$; on a une suite exacte de groupes

$$
\{0\} \to \mathbf{Z}/p^{n-1}\mathbf{Z} \xrightarrow{u} (\mathbf{Z}/p^n\mathbf{Z})^* \xrightarrow{v} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\},
$$

où $v$ est la projection canonique et où $u$ est déduit par passage aux quotients de l’application $r \mapsto x^r$. Soit $\mathbf{Z}_p$ l’anneau des entiers $p$-adiques (V, p. 92), et soit $x$ un élément de $\mathbf{Z}_p$ tel que $x-1 \in p\mathbf{Z}_p$, $x-1 \notin p^2\mathbf{Z}_p$; par passage à la limite projective, on déduit des suites exactes (5) une suite exacte

$$
\{0\} \to \mathbf{Z}_p \xrightarrow{u} \mathbf{Z}_p^* \xrightarrow{v} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

où $v$ est l’application canonique, et où l’application continue $u$ prolonge l’application $n \mapsto x^n$, $n \in \mathbf{Z}$. On pose souvent $x^n = u(x)$ pour $n \in \mathbf{Z}_p$.

De même, si $x \in \mathbf{Z}_2$, avec $x-1 \in 4\mathbf{Z}_2$, $x-1 \notin 8\mathbf{Z}_2$, on a une suite exacte scindée

$$
\{0\} \to \mathbf{Z}_2 \xrightarrow{u} \mathbf{Z}_2^* \xrightarrow{v} (\mathbf{Z}/4\mathbf{Z})^* \to \{1\},
$$

où $u$ prolonge par continuité l’application $n \mapsto x^n$.

## EXERCICES {#alg-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
