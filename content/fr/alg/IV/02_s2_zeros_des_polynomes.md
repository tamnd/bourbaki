---
book: alg
book_title: Algebra
chapter: IV
chapter_title: Polynômes et fractions rationnelles
section: 2
section_title: ZÉROS DES POLYNÔMES
lang: fr
source: alg-iv-vii-fr
book_pages: A IV.83-A IV.84
pdf_pages: 0021-0025, 0090-0091
extraction: ocr
subsections:
    - "no": 1
      title: Racines d’un polynôme à une indéterminée. Multiplicité
      page: 0
      pdf_page: 21
    - "no": 2
      title: Critère différentiel pour la multiplicité d’une racine
      page: 16
      pdf_page: 23
    - "no": 3
      title: Fonctions polynomiales sur un anneau intègre infini
      page: 16
      pdf_page: 23
statements: 20
exercises: 13
content_sha256: d8d29a6444b75ad45f6377e9b2679890fd9713ff6d0e7284c5915f17b9d13d0a
---

## § 2. ZÉROS DES POLYNÔMES

### 1. Racines d’un polynôme à une indéterminée. Multiplicité

Soit $g \in \mathbf{A}[(X_i)_{i \in I}]$ et soit E une A-algèbre associative unifère. Soit $x = (x_i)_{i \in I}$ une famille d’éléments deux à deux permutables de E. On dit que x est un zéro de g dans $E^l$ si $g(x) = 0$. Si $f$ est un polynôme par rapport à une seule indéterminée, un zéro de $f$ dans E s’appelle encore une racine de $f$ dans E.

#### Proposition 1 {#alg-iv-s2-prop-1 .statement}

Soient $f \in \mathbf{A}[X]$ et $\alpha \in \mathbf{A}$. Le reste de la division de $f$ par $X - \alpha$ est $f(\alpha)$. Pour que $\alpha$ soit racine de $f$, il faut et il suffit que $X - \alpha$ soit un diviseur de $f$ dans $\mathbf{A}[X]$.

En effet, soient $u, v \in \mathbf{A}[X]$ tels que $f = (X - \alpha)u + v$, et $\deg v < 1$. Alors $v$ est un scalaire, et $f(\alpha) = (\alpha - \alpha)u(\alpha) + v = v$. Cela prouve la première assertion. La deuxième résulte de la première.

#### Proposition 2 {#alg-iv-s2-prop-2 .statement}

Soient $f \in \mathbf{A}[X]$, $\alpha \in \mathbf{A}$, et $h$ un entier $\geqslant 0$. Les conditions suivantes sont équivalentes :
(i) $f$ est divisible par $(X - \alpha)^h$ mais non par $(X - \alpha)^{h+1}$;
(ii) il existe $g \in \mathbf{A}[X]$ tel que $f = (X - \alpha)^h g$ et $g(\alpha) \neq 0$.
(i) $\Rightarrow$ (ii) : cela résulte aussitôt de la prop. 1.
(ii) $\Rightarrow$ (i) : supposons que $f = (X - \alpha)^h g$, où $g$ n’admet pas la racine $\alpha$. Alors $f$ est divisible par $(X - \alpha)^h$. Supposons qu’il existe $g_1 \in \mathbf{A}[X]$ tel que $f = (X - \alpha)^{h+1} g_1$, où $g_1 \in \mathbf{A}[X]$. Comme $(X - \alpha)^h$ n’est pas diviseur de 0 dans $\mathbf{A}[X]$ (IV, p. 8, prop. 7), on a $g = (X - \alpha)g_1$, donc $g(\alpha) = 0$, ce qui est absurde.

#### Proposition 3 {#alg-iv-s2-prop-3 .statement}

Soient $f$ un élément non nul de $\mathbf{A}[X]$, et $\alpha \in \mathbf{A}$. Il existe un entier $h \geqslant 0$ et un seul qui satisfait aux conditions (i) et (ii) de la prop. 2.
C’est évident sur la condition (i), compte tenu du fait que, si $f$ est divisible par $(X - \alpha)^h$, on a $\deg f \geqslant h$ (IV, p. 8, prop. 7).

#### Définition 1 {#alg-iv-s2-def-1 .statement}

Avec les notations précédentes, on dit que $\alpha$ est d’ordre $h$, ou de multiplicité $h$, relativement à $f$.

Si $h > 0$, on dit aussi que $\alpha$ est racine d’ordre $h$, ou de multiplicité $h$, de $f$. Une racine d’ordre 1 est dite racine simple, une racine d’ordre 2 est dite racine double,… Une racine d’ordre $> 1$ est dite multiple.

#### Remarque 1 {#alg-iv-s2-n1-rem-1 .statement}

Si $f = 0$, on convient de dire que $\alpha$ est d’ordre $\geqslant h$ relativement à $f$, quels que soient $\alpha \in \mathbf{A}$ et l’entier $h \geqslant 0$. Quels que soient $f \in \mathbf{A}[X]$ et $\alpha \in \mathbf{A}$, dire que $\alpha$ est d’ordre $\geqslant h$ relativement à $f$ signifie que $(X - \alpha)^h$ divise $f$.

#### Remarque 2 {#alg-iv-s2-n1-rem-2 .statement}

Soit B un anneau commutatif contenant A comme sous-anneau. Soient $f \in \mathbf{A}[X]$ non nul et $\alpha \in \mathbf{A}$. L’ordre de $\alpha$ relativement à $f$ est le même, que l’on considère $f$ comme élément de $\mathbf{B}[X]$ ou comme élément de $\mathbf{A}[X]$. C’est évident sur la condition (ii) de la prop. 2.

#### Proposition 4 {#alg-iv-s2-prop-4 .statement}

Soient $f$ et $g$ des éléments non nuls de $\mathbf{A}[X]$. Soit $\alpha \in \mathbf{A}$, et soient $p$ et $q$ les ordres de $\alpha$ relativement à $f$ et $g$.

(i) L’ordre de $\alpha$ relativement à $f + g$ est $\geq \inf(p, q)$. Il est égal à $\inf(p, q)$ si $p \neq q$.
(ii) L’ordre de $\alpha$ relativement à $fg$ est $\geq p + q$. Il est égal à $p + q$ si $\mathbf{A}$ est intègre.

En effet, on a $f(X) = (X - \alpha)^p f_1(X)$, $g(X) = (X - \alpha)^q g_1(X)$ avec $f_1(\alpha) \neq 0$, $g_1(\alpha) \neq 0$. Supposons par exemple que $p \leq q$; on a alors

$$
f(X) + g(X) = (X - \alpha)^p(f_1(X) + (X - \alpha)^{q-p}g_1(X)),
$$

et, si $p < q$, $\alpha$ n’est pas racine de $f_1(X) + (X - \alpha)^{q-p}g_1(X)$; cela prouve (i). D’autre part, on a $f(X)g(X) = (X - \alpha)^{p+q}f_1(X)g_1(X)$, et $f_1(\alpha)\ g_1(\alpha) \neq 0$ si $\mathbf{A}$ est intègre ; cela prouve (ii).

#### Proposition 5 {#alg-iv-s2-prop-5 .statement}

Supposons $\mathbf{A}$ intègre. Soient $f$ un élément non nul de $\mathbf{A}[X]$, $\alpha_1, \ldots, \alpha_p$ des racines de $f$ dans $\mathbf{A}$ deux à deux distinctes, d’ordres $k_1, \ldots, k_p$. On a

$$
f(X) = (X - \alpha_1)^{k_1}(X - \alpha_2)^{k_2} \ldots (X - \alpha_p)^{k_p}g(X)
$$

où $g \in \mathbf{A}[X]$ et où $\alpha_1, \ldots, \alpha_p$ ne sont pas racines de $g$.

Procédons par récurrence sur $p$, la proposition étant évidente pour $p = 1$ en vertu de la déf. 1. Supposons donc qu’on ait $f(X) = g_1(X)\ g_2(X)$, où

$$
g_1(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_{p-1})^{k_{p-1}}, \quad g_2(X) \in \mathbf{A}[X].
$$

Comme $\mathbf{A}$ est intègre et que $\alpha_p$ est distinct de $\alpha_1, \ldots, \alpha_{p-1}$, alors $\alpha_p$ n’est pas racine de $g_1(X)$, donc $\alpha_p$ est racine d’ordre $k_p$ de $g_2(X)$ (prop. 4, (ii)). Par suite, $g_2(X)$ est divisible par $(X - \alpha_p)^{k_p}$, et par conséquent

$$
f(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_p)^{k_p}g(X)
$$

où $g(X) \in \mathbf{A}[X]$. Il est clair que $\alpha_1, \ldots, \alpha_p$ ne sont pas racines de $g$.

#### Théorème 1 {#alg-iv-s2-thm-1 .statement}

Supposons $\mathbf{A}$ intègre. Soient $f$ un élément non nul de $\mathbf{A}[X]$, $n$ son degré. La somme des ordres de toutes les racines de $f$ dans $\mathbf{A}$ est $\leq n$.

Cela résulte aussitôt de la prop. 5.

#### Corollaire {#alg-iv-s2-n1-cor-1 .statement}

On suppose $\mathbf{A}$ intègre. Soient $f, g \in \mathbf{A}[X]$, de degrés $\leq n$. S’il existe $n + 1$ éléments $x_1, \ldots, x_{n+1}$ de $\mathbf{A}$, deux à deux distincts, tels que $f(x_i) = g(x_i)$ pour $1 \leq i \leq n + 1$, on a $f = g$.

Il suffit d’appliquer le th. 1 à $f - g$.

#### Proposition 6 (formule d’interpolation de Lagrange) {#alg-iv-s2-prop-6 .statement}

Soient $\mathbf{K}$ un corps commutatif, $\alpha_1, \alpha_2, \ldots, \alpha_n$ des éléments distincts de $\mathbf{K}$, et $\beta_1, \beta_2, \ldots, \beta_n$ des éléments de $\mathbf{K}$. Pour $i = 1, 2, \ldots, n$, posons

$$
f_i(X) = \prod_{j \in U(i)} (X - \alpha_j)/(\alpha_i - \alpha_j),
$$

où U(i) est l’ensemble des entiers j tels que $j \neq i$ et $1 \leq j \leq n$. Alors $\beta_1 f_1 + \cdots + \beta_n f_n$ est l’unique élément $f$ de $K[X]$ tel que $\deg f < n$ et $f(\alpha_i) = \beta_i$ pour $1 \leq i \leq n$.

L’unicité de $f$ résulte du cor. du th. 1. Soit $f = \beta_1 f_1 + \cdots + \beta_n f_n$. Comme $f_i$ est de degré $n - 1$, on a $\deg f < n$. D’autre part, $f_i(\alpha_j) = 0$ pour $j \neq i$, et $f_i(\alpha_i) = 1$. Donc $f(\alpha_i) = \beta_i$ pour $1 \leq i \leq n$.

#### Corollaire {#alg-iv-s2-n1-cor-2 .statement}

Supposons A intègre. Soit $f \in A[X]$, de degré $< n$, et soit K un sous-anneau de A qui est un corps. S’il existe n éléments $\alpha_1, \ldots, \alpha_n$ de A, distincts, et tels que $\alpha_i \in K$ et $f(\alpha_i) \in K$ pour $i = 1, \ldots, n$, alors $f \in K[X]$.

### 2. Critère différentiel pour la multiplicité d’une racine

#### Proposition 7 {#alg-iv-s2-prop-7 .statement}

Soient $f \in A[X]$, et $\alpha \in A$ une racine de $f$. Pour que $\alpha$ soit racine simple de $f$, il faut et il suffit que $\alpha$ ne soit pas racine de la dérivée $Df$ de $f$.

Par hypothèse, on a $f = (X - \alpha) g$, où $g \in A[X]$. Pour que $\alpha$ soit racine simple de $f$, il faut et il suffit que $g(\alpha) \neq 0$. Or, on a $Df = g + (X - \alpha) Dg$, d’où $(Df)(\alpha) = g(\alpha)$.

Plus généralement :

#### Proposition 8 {#alg-iv-s2-prop-8 .statement}

Soient $f \in A[X]$, et $\alpha \in A$. Supposons que $\alpha$ soit d’ordre $k \geq 1$ relativement à $f$. Alors $\alpha$ est d’ordre $\geq k - 1$ relativement à $Df$. Si $k . 1$ est simplifiable dans A, alors $\alpha$ est d’ordre $k - 1$ relativement à $Df$.

Par hypothèse, il existe $g \in A[X]$ tel que $f = (X - \alpha)^k g$ et $g(\alpha) \neq 0$. Alors $Df = k(X - \alpha)^{k-1} g + (X - \alpha)^k Dg = (X - \alpha)^{k-1}(kg + (X - \alpha) Dg)$, ce qui établit la première partie de la proposition. La valeur de $kg + (X - \alpha) Dg$ pour $X = \alpha$ est $kg(\alpha)$, donc est non nulle si $k . 1$ est simplifiable dans A ; cela prouve la deuxième partie de la proposition.

Soit $k$ un entier $> 0$ tel que $k . 1 = 0$ dans A. Soit $f(X) = X^k \in A[X]$. Alors 0 est racine d’ordre $k$ de $f$, et racine d’ordre arbitrairement grand de $Df$.

#### Corollaire {#alg-iv-s2-n2-cor-1 .statement}

Soient $f \in A[X]$, $\alpha \in A$, et $p$ un entier $\geq 0$. On suppose que $p!.1$ est simplifiable dans A. Alors, pour que $\alpha$ soit racine d’ordre $p$ de $f$, il faut et il suffit que $\alpha$ soit racine de $f, Df, \ldots, D^{p-1}f$, et ne soit pas racine de $D^pf$.

Cela résulte de la prop. 8 par récurrence sur $p$.

### 3. Fonctions polynomiales sur un anneau intègre infini

#### Proposition 9 {#alg-iv-s2-prop-9 .statement}

On suppose A intègre. Soient I un ensemble, $(H_i)_{i \in I}$ une famille de parties infinies de A, et $H = \prod_{i \in I} H_i \subset A^I$. Soit $f$ un élément non nul de $A[(X_i)_{i \in I}]$.

Soit $H_f$ l’ensemble des $x \in H$ tels que $f(x) \neq 0$. Alors H et $H_f$ sont équipotents.

a) Supposons d’abord I fini et soit $n = \mathrm{Card}\ I$. La proposition est évidente pour $n = 0$, et nous la démontrerons par récurrence sur $n$. Choisissons un élément $i_0$ de I, et soient $J = I - \{ i_0 \}$, $B = A[(X_i)_{i \in J}]$. Comme $f \neq 0$, on peut écrire f = \sum_{k=0}^{m} g_k X_{i_0}^k \text{ où } g_0, ..., g_m \in \mathbf{B}, \text{ et } g_m \neq 0. \text{ D’après l’hypothèse de récurrence, l’ensemble K des } x \in \prod_{i \in J} H_i \text{ tels que } g_m(x) \neq 0 \text{ est équipotent à } \prod_{i \in J} H_i. \text{ Pour } x \in K, \text{ le polynôme}

$$
h(X_{i_0}) = \sum_{k=0}^{m} g_k(x) X_{i_0}^k \in A[X_{i_0}]
$$

est non nul. D’après le th. 1 (IV, p. 15), l’ensemble des $\alpha \in H_{i_0}$ tels que $h(\alpha) \neq 0$ est équipotent à $H_{i_0}$, d’où

$$
\text{Card H} \geq \text{Card H}_f \geq (\text{Card K}).(\text{Card H}_{i_0}) = \text{Card H},
$$

et par suite Card H = Card H_f.

b) Dans le cas général, il existe une partie finie I’ de I telle que $f \in A[(X_i)_{i \in I'}]$. Soit $H'_f$ l’ensemble des $x \in \prod_{i \in I'} H_i$ tels que $f(x) \neq 0$. Alors $H_f = H'_f \times (\prod_{i \in I - I'} H_i)$, et il suffit d’appliquer à $H'_f$ la première partie de la démonstration.

#### Corollaire 1 {#alg-iv-s2-prop-9-cor-1 .statement}

*On conserve les hypothèses et les notations de la prop. 9. Si I est non vide, $H_f$ est infini.*

#### Corollaire 2 {#alg-iv-s2-prop-9-cor-2 .statement}

*On suppose que A est intègre et infini ou que A est une algèbre sur un corps infini. Pour tout $f \in A[(X_i)_{i \in I}]$, soit $\tilde{f} : A^I \to A$ la fonction polynomiale définie par $f$ (IV, p. 4). Alors l’application $f \mapsto \tilde{f}$ est injective.*

Lorsque A est intègre infini, le corollaire résulte aussitôt de la prop. 9. Supposons que A soit une algèbre sur un corps infini k. Soit $f = \sum_{v \in N^{(I)}} \alpha_v X^v$ un élément non nul de $A[(X_i)_{i \in I}]$. Il existe un $v_0 \in N^{(I)}$ tel que $\alpha_{v_0} \neq 0$, et une forme k-linéaire $\varphi$ sur A telle que $\varphi(\alpha_{v_0}) \neq 0$. Soit $g = \sum_{v \in N^{(I)}} \varphi(\alpha_v) X^v \in k[(X_i)_{i \in I}]$. On a $g \neq 0$, donc il existe un $x \in k^I$ tel que $g(x) \neq 0$. Alors $\varphi(f(x)) = g(x) \neq 0$, donc $f(x) \neq 0$.

Lorsque A est intègre infini, ou lorsque A est une algèbre sur un corps infini, on identifie le plus souvent $f$ à $\tilde{f}$.

Supposons A fini. Soit $f(X) = \prod_{\alpha \in A} (X - \alpha)$. Alors $f \neq 0$ mais $\tilde{f} = 0$. Pour d’autres exemples, cf. IV, p. 84, exerc. 7 et 8.

#### Théorème 2 (principe du prolongement des identités algébriques) {#alg-iv-s2-thm-2 .statement}

*Supposons A intègre et infini. Soient $g_1, ..., g_m, f$ des éléments de $A[(X_i)_{i \in I}]$. On fait les hypothèses suivantes :

a) $g_1 \neq 0, ..., g_m \neq 0$;
b) pour tout $x \in A^I$ tel que $g_1(x) \neq 0, ..., g_m(x) \neq 0$, on a $f(x) = 0$.

Alors $f = 0$.

En effet, si $f \neq 0$, on a $fg_1 ... g_m \neq 0$ (IV, p. 9, prop. 8), donc il existe $x \in A^I$ tel que $f(x) g_1(x) ... g_m(x) \neq 0$ (IV, p. 17, cor. 2), ce qui contredit l’hypothèse.

#### Scholie {#alg-iv-s2-n3-sch-1 .statement}

Soient A un anneau intègre et $f \in A[(X_i)_{i \in I}]$. Le th. 2 fournit un moyen commode pour prouver que $f = 0$. Il suffit de considérer un anneau intègre infini E contenant A comme sous-anneau ; si l’on démontre que $f((x_i)) = 0$ pour tout $(x_i) \in E^I$ (ou seulement pour les $(x_i) \in E^I$ qui n’annulent pas un nombre fini de polynômes donnés non nuls), il en résulte que $f = 0$. Si A lui-même n’est pas infini, on peut par exemple prendre pour E l’anneau A[X] ou son corps des fractions.

Une fois démontrée la relation $f = 0$, on en déduit évidemment $f((y_i)) = 0$ pour tout $(y_i) \in F^I$, où F est une A-algèbre unifière associative et commutative quelconque ; en particulier, F peut être finie ou non intègre.

En d’autres termes, la démonstration de l’identité $f((x_i)) = 0$ lorsque les $x_i$ parcourent un anneau intègre infini contenant A comme sous-anneau (avec éventuellement la restriction que $g_k((x_i)) \neq 0$ pour $1 \leq k \leq m$, les $g_k$ étant des polynômes non nuls) entraîne la même identité lorsque les $x_i$ parcourent une A-algèbre unifière associative et commutative quelconque.

En particulier, soit $f \in \mathbf{Z}[(X_i)]$. Si $f((x_i)) = 0$ lorsque les $x_i$ parcourent $\mathbf{Z}$ (avec éventuellement la restriction que $g_k((x_i)) \neq 0$ pour $1 \leq k \leq m$, les $g_k$ étant des éléments non nuls de $\mathbf{Z}[(X_i)]$), on a la même identité lorsque les $x_i$ parcourent un anneau commutatif quelconque.

## EXERCICES {#alg-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
