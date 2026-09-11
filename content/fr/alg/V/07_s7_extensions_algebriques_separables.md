---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 7
section_title: EXTENSIONS ALGÉBRIQUES SÉPARABLES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.35-A V.45, A V.145-A V.146
pdf_pages: 0139-0149, 0249-0250
extraction: ocr
subsections:
    - "no": 1
      title: Extensions algébriques séparables
      page: 35
      pdf_page: 139
    - "no": 2
      title: Polynômes séparables
      page: 36
      pdf_page: 140
    - "no": 3
      title: Éléments algébriques séparables
      page: 38
      pdf_page: 142
    - "no": 4
      title: Théorème de l’élément primitif
      page: 39
      pdf_page: 143
    - "no": 5
      title: Propriétés de stabilité des extensions algébriques séparables
      page: 40
      pdf_page: 144
    - "no": 6
      title: Un critère de séparabilité
      page: 0
      pdf_page: 145
    - "no": 7
      title: Fermeture algébrique séparable
      page: 42
      pdf_page: 146
    - "no": 8
      title: Clôture séparable d’un corps
      page: 43
      pdf_page: 147
    - "no": 9
      title: Degrés séparable et inséparable d’une extension de degré fini
      page: 44
      pdf_page: 148
statements: 42
exercises: 5
content_sha256: 8442ab006744ede6d0858b45206396bcd6fd8f4653e0ba6b462899ba01f3f5eb
---

## § 7. EXTENSIONS ALGÉBRIQUES SÉPARABLES

Dans tout ce paragraphe, on note $K$ un corps.

### 1. Extensions algébriques séparables

#### Définition 1 {#alg-v-s7-def-1 .statement}

Soit $E$ une extension algébrique de $K$. On dit que $E$ est séparable (sur $K$) si toute sous-extension $F$ de $E$, de degré fini sur $K$, est une algèbre étale sur $K$ (V, p. 28, déf. 1).

Soit $E$ une extension de degré fini de $K$. Comme toute sous-algèbre d’une algèbre étale est étale (V, p. 29, prop. 3), il revient au même de supposer que $E$ est une extension séparable de $K$, ou que $E$ est une algèbre étale sur $K$.

#### Proposition 1 {#alg-v-s7-prop-1 .statement}

Soit $E$ une extension algébrique de $K$. Si $E$ est séparable, toute sous-extension $E'$ de $E$ est séparable. Réciproquement, si toute sous-extension de degré fini de $E$ est séparable, $E$ est séparable.

Cela résulte immédiatement de la définition 1.

#### Proposition 2 {#alg-v-s7-prop-2 .statement}

Pour que le corps $K$ soit parfait, il faut et il suffit que toute extension algébrique de $K$ soit séparable.

Supposons d’abord $K$ parfait. Comme un corps est un anneau réduit, il résulte du lemme 5 (V, p. 34) que toute extension de degré fini de $K$ est une algèbre étale sur $K$; par suite, toute extension algébrique de $K$ est séparable.

Supposons maintenant que $K$ soit un corps imparfait de caractéristique $p \neq 0$. Soit $\Omega$ une clôture algébrique de $K$. Comme $K$ est imparfait, il existe $b \in K$ n’appartenant pas à $K^p$; posons $a = b^{1/p}$. Alors l’extension $K(a)$ de $K$ est radicielle de degré fini. D’après V, p. 25, prop. 3, il existe un seul $K$-homomorphisme de $K(a)$ dans $\Omega$, et comme on a $[K(a):K] > 1$, l’algèbre $K(a)$ n’est pas étale sur $K$ (V, p. 31, prop. 4). Autrement dit, l’extension $K(a)$ de degré fini de $K$ n’est pas séparable.

#### Corollaire {#alg-v-s7-n1-cor-1 .statement}

*Toute extension algébrique d’un corps de caractéristique 0, ou d’un corps fini, est séparable.*

Cela résulte de V, p. 7, prop. 5.

### 2. Polynômes séparables

#### Proposition 3 {#alg-v-s7-prop-3 .statement}

*Soient f un polynôme non nul dans $K[X]$ et $\Omega$ une extension algébriquement close de $K$. Les conditions suivantes sont équivalentes :*

a) *Le polynôme f est étranger à sa dérivée $f'$ dans $K[X]$*.
b) *On a, soit $\deg(f) = 0$, soit $\deg(f) > 0$ et $\operatorname{dis}(f) \neq 0$ (IV, p. 79)*.
c) *Il existe une extension L de $K$ telle que f se décompose dans $L[X]$ en produit de polynômes distincts de degré $\leq 1$*.
d) *Les racines de f dans $\Omega$ sont simples*.
e) *La K-algèbre $K[X]/(f)$ est étale* (V, p. 28, déf. 1).

$a) \Rightarrow d)$ : Sous les hypothèses de a), il existe deux polynômes $g$ et $h$ dans $K[X]$ tels que $fg + f'h = 1$ (IV, p. 12). Soit $a$ une racine de $f$ dans $\Omega$; on a

$$
f'(a)\ h(a) = f(a)\ g(a) + f'(a)\ h(a) = 1 ,
$$

d’où $f'(a) \neq 0$; par suite, $a$ est racine simple de $f$ dans $\Omega$ (IV, p. 16, prop. 7).

$d) \Rightarrow c)$ : Si d) est satisfaite, $f$ se décompose dans $\Omega[X]$ en produit de polynômes distincts de degré $\leq 1$.

$c) \Rightarrow b)$ : Sous les hypothèses de c), il existe un élément $\lambda \neq 0$ dans $L$ et des éléments *distincts* $\alpha_1, \ldots, \alpha_n$ de $L$ tels que $f(X) = \lambda (X - \alpha_1) \ldots (X - \alpha_n)$. Si $\deg(f) > 0$, on a (IV, p. 79, prop. 11)

$$
\operatorname{dis}(f) = \lambda^{2n-2} \prod_{i < j} (\alpha_i - \alpha_j)^2 \neq 0 .
$$

$b) \Rightarrow a)$ : Soient $c$ le coefficient dominant et $D$ le discriminant de $f$; le résultant de $f'$ et $f$ est égal à $\pm cD$ (IV, p. 79, formule (54)), donc n’est pas nul ; par suite (IV, p. 73, cor. 2), les polynômes $f$ et $f'$ sont étrangers dans $K[X]$.

$a) \Leftrightarrow e)$ : Soient $A$ la K-algèbre $K[X]/(f)$ et $x$ l’image de $X$ dans $A$; d’après III, p. 137, prop. 22, le $A$-module $\Omega_K(A)$ est engendré par l’élément $dx$, soumis à la seule relation $f'(x)\ dx = 0$. D’après V, p. 32, th. 3, la K-algèbre $A$ est donc étale si et seulement si $f'(x)$ est un élément inversible de $A$, ce qui signifie que $f$ et $f'$ sont étrangers dans $K[X]$.

#### Définition 2 {#alg-v-s7-def-2 .statement}

*On dit qu’un polynôme* $f \in K[X]$ *est séparable s’il est non nul et satisfait aux conditions équivalentes a), b), c), d) et e) de la prop. 3.*

#### Remarque 1 {#alg-v-s7-n2-rem-1 .statement}

Soient L une extension de K et $f$ un polynôme non constant de $K[X]$. D’après la condition e) de la prop. 3 et V, p. 32, cor. 2, il revient au même de supposer que $f$ est séparable qu’on le considère comme élément de $K[X]$ ou de $L[X]$. Par contre, il se peut fort bien que $f$ soit irréductible dans $K[X]$, mais non dans $L[X]$.

#### Remarque 2 {#alg-v-s7-n2-rem-2 .statement}

Soit $f \in K[X]$; on sait (IV, p. 13, prop. 13) qu’il existe des polynômes irréductibles $f_1, \ldots, f_m$ dans $K[X]$ tels que $f = f_1 \ldots f_m$. Soit $\Omega$ une clôture algébrique de K ; comme un polynôme irréductible $g \in K[X]$ est polynôme minimal sur K de chacune de ses racines dans $\Omega$, deux polynômes irréductibles distincts dans $K[X]$ n’ont aucune racine commune dans $\Omega$. La condition d) de la prop. 3 montre alors que $f$ est séparable si et seulement si les polynômes $f_1, \ldots, f_m$ sont séparables et deux à deux distincts.

#### Proposition 4 {#alg-v-s7-prop-4 .statement}

*Soit* $f$ *un polynôme irréductible dans* $K[X]$. *Les conditions suivantes sont équivalentes :*
a) $f$ *est séparable*.
b) *Il existe une extension* L *de* K *dans laquelle* $f$ *a une racine simple*.
c) *La dérivée* $f'$ *de* $f$ *n’est pas nulle*.
d) *Le corps* K *est de caractéristique* 0, *ou bien il est de caractéristique* $p \neq 0$ *et l’on a* $f \notin K[X^p]$.

Notons d’abord qu’un polynôme irréductible dans $K[X]$ n’est pas constant. Il est clair que a) entraîne b) (prendre pour L une clôture algébrique de K). Si x est une racine simple de $f$ dans une extension L de K, on a $f'(x) \neq 0$ (IV, p. 16, prop. 7), donc b) entraîne c). L’équivalence de c) et d) résulte de V, p. 8, cor.

Supposons enfin qu’on ait $f' \neq 0$; soit x une racine de $f$ dans une extension algébriquement close $\Omega$ de K. Comme $f$ est le polynôme minimal de x sur K et qu’on a $\deg f' < \deg f$, on a $f'(x) \neq 0$ et x est donc racine simple de $f$ (IV, p. 16, prop. 7). Par suite $f$ est séparable, et l’on a prouvé que c) entraîne a).

#### Corollaire 1 {#alg-v-s7-prop-4-cor-1 .statement}

*Pour que le corps* K *soit parfait, il faut et il suffit que tout polynôme irréductible de* $K[X]$ *soit séparable*.

Si le corps K est de caractéristique 0, K est parfait et tout polynôme irréductible de $K[X]$ est séparable d’après l’assertion d) ci-dessus. Supposons donc que K soit de caractéristique $p \neq 0$.

Supposons d’abord K parfait. On a $K[X^p] = K[X]^p$, donc il n’existe aucun polynôme irréductible de $K[X]$ appartenant à $K[X^p]$. D’après la prop. 4, tout polynôme irréductible de $K[X]$ est séparable.

Supposons maintenant K imparfait, d’où $K \neq K^p$. Soit a un élément de K n’appartenant pas à $K^p$; le polynôme $X^p - a$ est irréductible dans $K[X]$ (V, p. 24, lemme 1), et il appartient à $K[X^p]$, donc n’est pas séparable.

#### Corollaire 2 {#alg-v-s7-prop-4-cor-2 .statement}

*Soit* $f \in K[X]$ *un polynôme non nul*. *Pour que* $f$ *soit séparable, il faut et il suffit qu’il existe une extension* L *de* K, *qui soit un corps parfait et telle que* $f$ *soit sans facteur multiple dans* $L[X]$.

Soit $\Omega$ une clôture algébrique de K ; si $f$ est séparable, $f$ est sans facteur multiple dans $\Omega[X]$ (prop. 3, d)). Inversement, si L est une extension parfaite de K telle que $f$ soit sans facteur multiple dans $L[X]$, alors $f$ est séparable dans $L[X]$ (cor. 1 et remarque 2), donc dans $K[X]$ (remarque 1).

### 3. Éléments algébriques séparables

#### Définition 3 {#alg-v-s7-def-3 .statement}

Soit E une extension de K. On dit qu’un élément x de E, algébrique sur K, est séparable sur K si l’extension algébrique $K(x)$ de K est séparable.

#### Proposition 5 {#alg-v-s7-prop-5 .statement}

Soient E une extension de K, x un élément de E algébrique sur K, et f le polynôme minimal de x sur K. Les conditions suivantes sont équivalentes :
a) x est séparable sur K ;
b) le polynôme f est séparable ;
c) x est racine simple de f.
L’équivalence de a) et b) résulte de la proposition 3, celle de b) et c) des propositions 3 et 4 (cf. V, p. 36 et 37).

#### Corollaire 1 {#alg-v-s7-prop-5-cor-1 .statement}

Si un élément x de E est racine simple d’un polynôme g de K[X], il est séparable sur K.
En effet, le polynôme minimal f de x sur K divise g dans K[X] (V, p. 15, th. 1), donc x est racine simple de f.

#### Corollaire 2 {#alg-v-s7-prop-5-cor-2 .statement}

Si un élément x de E est algébrique et séparable sur K, il est algébrique et séparable sur toute extension K’ de K contenue dans E.
Soit f le polynôme minimal de x sur K. Alors x est racine simple de f d’après la prop. 5, et comme f appartient à K’[X], l’élément x de E est séparable sur K’ d’après le cor. 1.

#### Corollaire 3 {#alg-v-s7-prop-5-cor-3 .statement}

Supposons K de caractéristique $p \neq 0$. Pour qu’un élément x de E appartienne à K, il faut et il suffit qu’il soit à la fois algébrique séparable et radiciel sur K.
La condition énoncée est évidemment nécessaire. Réciproquement, supposons que x soit algébrique séparable sur K, et radiciel de hauteur e sur K. Comme x est séparable sur K, le polynôme minimal f de x sur K n’appartient pas à $K[X^p]$ (prop. 4 et 5) ; comme x est radiciel de hauteur e sur K, on a $f(X) = X^{p^e} - x^{p^e}$ (V, p. 23, prop. 1) ; on en conclut $e = 0$, d’où $x \in K$.

#### Proposition 6 {#alg-v-s7-prop-6 .statement}

Soit E une extension de K.
a) Si E est algébrique et séparable sur K, tout élément de E est algébrique et séparable sur K.
b) Réciproquement, soit A un ensemble d’éléments de E algébriques et séparables sur K tel que $E = K(A)$ ; alors E est algébrique et séparable sur K.
Si E est algébrique et séparable sur K, il en est de même de l’extension $K(x)$ de K pour tout $x \in E$, d’où a).

. Sous les hypothèses de b), l’extension E est algébrique sur K (V, p. 18, cor. 1). Soit F une sous-extension de E, de degré fini sur K. D’après V, p. 11, cor., il existe des éléments $x_1, ..., x_m$ de A tels que $F \subset K(x_1, ..., x_m)$, et l’on a
$$
K(x_1, ..., x_m) = K[x_1, ..., x_m] \quad (\text{V, p. 18, cor. 1}) .
$$
D’après l’hypothèse faite sur A, les algèbres $K[x_1], ..., K[x_m]$ sont étales sur K ; il en est donc de même de l’algèbre $K[x_1] \otimes ... \otimes K[x_m]$ (V, p. 31, cor. 1). Or F est isomorphe à une sous-algèbre d’une algèbre quotient de $K[x_1] \otimes ... \otimes K[x_m]$, donc est étale (V, p. 29, prop. 3).

#### Corollaire {#alg-v-s7-n3-cor-1 .statement}

*Pour qu’une extension algébrique E soit séparable sur K, il faut et il suffit que tout élément de E soit racine simple de son polynôme minimal sur K.*
Il suffit d’appliquer les prop. 5 et 6.

### 4. Théorème de l’élément primitif

Soit E une extension de K ; on dit qu’un élément x de E est *primitif* si $E = K[x]$. Pour que l’extension E possède un élément primitif, il est nécessaire que $[E : K]$ soit fini.

#### Théorème 1 {#alg-v-s7-thm-1 .statement}

*Soit E une extension de K. Les conditions suivantes sont équivalentes :
a) E possède un élément primitif ;
b) il n’existe qu’un nombre fini de sous-extensions de E.
Ces conditions sont satisfaites lorsque E est une extension séparable de degré fini.*
Supposons d’abord que E possède un élément primitif x, et soit f le polynôme minimal de x sur K. Pour chaque polynôme unitaire $g \in E[X]$ divisant f dans E[X], notons $E_g$ la sous-extension de E engendrée par les coefficients de g. Comme les polynômes g possibles sont en nombre fini (si f se décompose dans E[X] en produit de r polynômes unitaires irréductibles, ce nombre est majoré par $2^r$), les sous-extensions $E_g$ sont en nombre fini. Il suffit donc, pour démontrer b), de prouver que toute sous-extension L de E est l’une des $E_g$. Or, si L est une sous-extension de E, on a $L[x] = E$; si g est le polynôme minimal de x sur L, on a $[E : L] = \deg(g)$. Par ailleurs, g est un diviseur de f dans L[X], donc dans E[X] ; on a $E_g \subset L$, et $E = E_g[x]$. Comme $g(x) = 0$, on a $[E : E_g] \leq \deg(g)$, donc $[E : E_g] \leq [E : L]$, donc $L = E_g$, ce qu’on voulait démontrer.

Notons maintenant que la condition b) implique que l’extension E est de degré fini : d’après la remarque 2 de V, p. 18, il suffit de prouver qu’elle est algébrique ; or, si z est un élément de E transcendant sur K, les sous-extensions $K(z^n)$, $n \in \mathbf{N}$, sont deux à deux distinctes.

Pour démontrer l’implication $b) \Rightarrow a)$ distinguons alors deux cas :

*A) Si le corps K est *fini*, le corps E, qui est un espace vectoriel de dimension finie sur K, est un ensemble fini. Par suite $^1$ (V, p. 75, lemme 1), il existe un élément x de E engendrant le groupe multiplicatif de E, et on a $E = K[x]$.

$^1$ Le lecteur vérifiera que le théorème 1 n’est utilisé nulle part avant la démonstration du lemme 1 de V, p. 75.

B) Supposons maintenant le corps $K$ *infini*. Si b) est vérifiée, l’extension $E$ est de degré fini, donc b) signifie aussi que $E$ ne possède qu’un nombre fini de sous-algèbres. Cela étant, l’implication $b) \Rightarrow a)$ résulte de la proposition plus générale suivante (pour laquelle l’hypothèse que le corps $K$ est infini est indispensable, cf. V, p. 146, exerc. 5 du § 7) :

#### Proposition 7 {#alg-v-s7-prop-7 .statement}

*Supposons $K$ infini ; soit $A$ une $K$-algèbre commutative ne possédant qu’un nombre fini de sous-algèbres (par exemple une $K$-algèbre étale, V, p. 29, prop. 3), et soit $V$ un sous-espace vectoriel de $A$ qui engendre $A$. Il existe $x \in V$ tel que $A = K[x]$.*

Soient $A_1, ..., A_n$ les sous-algèbres de $A$ distinctes de $A$. Si $x \notin A_1 \cup ... \cup A_n$, la sous-algèbre $K[x]$ ne peut être égale à aucune des $A_i$, donc coïncide avec $A$. Par ailleurs, puisque $V$ engendre $A$, il n’est contenu dans aucun des sous-espaces $A_i$. La proposition 7 résulte donc du lemme suivant :

#### Lemme 1 {#alg-v-s7-lem-1 .statement}

*Soient $A$ un $K$-espace vectoriel, $V, A_1, ..., A_n$ des sous-espaces de $A$. Si $\mathrm{Card}(K) \geq n$, et si $V$ n’est contenu dans aucun des $A_i$, $V$ n’est pas contenu dans $A_1 \cup ... \cup A_n$.

Raisonnant par récurrence sur $n$, il suffit de prouver que si $V \not\subset A_n$ et si $V \subset A_1 \cup ... \cup A_n$, alors $V \subset A_1 \cup ... \cup A_{n-1}$. Soit $x \in V, x \notin A_n$, et soit $y$ quelconque dans $V$. Si $y$ appartient à $Kx$, on a $y \in A_1 \cup ... \cup A_{n-1}$. Sinon, les éléments $x$ et $y + \lambda x, \lambda \in K$, sont en nombre strictement supérieur à $n$ et appartiennent à $A_1 \cup ... \cup A_n$; deux d’entre eux appartiennent donc au même $A_i$. Il existe donc $i, 1 \leq i \leq n$, avec, soit $x \in A_i$ et $y + \lambda x \in A_i$ pour un $\lambda \in K$, soit $y + \lambda x \in A_i$ et $y + \mu x \in A_i$ pour deux scalaires distincts $\lambda, \mu \in K$. Dans les deux cas, on en conclut que $x \in A_i$ et $y \in A_i$: mais cela implique $i \neq n$, donc $y \in A_1 \cup ... \cup A_{n-1}$, ce qu’on voulait démontrer.*

Cela achève la démonstration de l’équivalence de a) et b) dans le théorème 1. Enfin, si l’extension $E$ est séparable et de degré fini, la condition b) est satisfaite, d’après V, p. 29, prop. 3.

### 5. Propriétés de stabilité des extensions algébriques séparables

#### Proposition 8 {#alg-v-s7-prop-8 .statement}

*Soient $E$ une extension de $K$ et $(E_i)_{i \in I}$ une famille de sous-extensions de $E$ telles que $E = K(\bigcup_{i \in I} E_i)$. Si chacune des extensions $E_i$ est algébrique et séparable sur $K$, il en est de même de $E$.*

Ceci résulte aussitôt de la prop. 6 (V, p. 38).

#### Proposition 9 {#alg-v-s7-prop-9 .statement}

*Soient $F$ une extension algébrique de $K$, et $E$ une sous-extension de $F$. Pour que $F$ soit séparable sur $K$, il faut et il suffit que $F$ soit séparable sur $E$ et $E$ séparable sur $K$.*

Supposons d’abord que $F$ soit séparable sur $K$. Alors $E$ est séparable sur $K$ d’après la prop. 1 (V, p. 35). De plus, tout élément de $F$ est séparable sur $K$ (V, p. 38, prop. 6), donc sur E (V, p. 38, cor. 2), et par suite F est séparable sur E (V, p. 38, prop. 6).

Réciproquement, supposons que F soit séparable sur E et E séparable sur K. Notons x un élément de F et $f \in E[X]$ le polynôme minimal de x sur E. Comme E est algébrique sur K, le th. 2 (V, p. 17) montre qu’il existe une sous-extension E’ de E de degré fini sur K, et telle que $f \in E'[X]$; alors, $f$ est à la fois le polynôme minimal de x sur E et sur E’, et comme x est séparable sur E (V, p. 38, prop. 6), il l’est aussi sur E’ (V, p. 38, prop. 5). Posons $F' = E'(x)$; alors F’ est séparable et de degré fini sur E’, et comme E est séparable sur K, E’ est séparable et de degré fini sur K (V, p. 35, prop. 1). Alors F’ est séparable et de degré fini sur K d’après V, p. 32, cor. 2. Par suite (V, p. 38, prop. 6), x est séparable sur K. On a prouvé que tout élément de F est séparable sur K, donc F est séparable sur K (V, p. 38, prop. 6).

#### Proposition 10 {#alg-v-s7-prop-10 .statement}

*Soient E et K’ deux sous-extensions d’une même extension de K et E’ = K’(E). On suppose E algébrique sur K, donc E’ algébrique sur K’* (V, p. 18, cor. 2).

a) *Si E est séparable sur K, alors E’ est séparable sur K’*.

b) *Réciproquement, si E’ est séparable sur K’ et si E et K’ sont linéairement disjointes sur K, alors E est séparable sur K*.

L’assertion a) résulte aussitôt de la prop. 6 (V, p. 38).

Sous les hypothèses de b), soit F une sous-extension de E, de degré fini sur K. Alors F et K’ sont linéairement disjointes sur K, donc la K’-algèbre $F_{(K')} = K' \otimes_K F$ est isomorphe à K’(F). Comme K’(F) est une sous-extension de E’, de degré fini sur K’, et que E’ est algébrique et séparable sur K’, la K’-algèbre K’(F) est étale. Autrement dit, la K’-algèbre $F_{(K')}$ est étale, et le cor. 2 de la prop. 4 (V, p. 32) montre que F est étale sur K. On a prouvé que E est séparable sur K.

### 6. Un critère de séparabilité

#### Proposition 11 {#alg-v-s7-prop-11 .statement}

*Supposons que K soit d’exposant caractéristique p et soit E une extension algébrique de K, engendrée par un ensemble S. Si E est séparable sur K, on a $E = K(S^{p^n})$ pour tout entier $n \geq 0$; réciproquement, si E est de degré fini sur K et si $E = K(S^p)$, alors E est séparable sur K*.

Le cas $p = 1$ est trivial d’après le cor. de V, p. 36. Supposons désormais $p \neq 1$. Par hypothèse, E est algébrique sur K et l’on a $E = K(S)$; on a donc

$$
K(S^p) = K(E^p) = K[E^p]
$$

d’après V, p. 18, cor. 1 .

Si E est de degré fini sur K, c’est une extension séparable de K si et seulement si c’est une algèbre étale sur K ; le cor. de V, p. 34, montre que ceci se produit si et seulement si l’on a $E = K[E^p]$.

Supposons maintenant E séparable et de degré infini sur K. Alors $K[E^p]$ est réunion des sous-anneaux $K[{E'}^p]$ où $E'$ parcourt l’ensemble des sous-extensions de E, de degré fini sur K ; mais une telle extension E’ est séparable sur K (V, p. 35, prop. 1), d’où

E' = K[E'^p] \subset K[E^p] par ce qui précède ; finalement, on a E = K[E^p]. Par récurrence sur $n \geq 0$, la relation $E = K[E^p]$ entraîne $E = K[E^{p^n}]$.

#### Corollaire 1 {#alg-v-s7-prop-11-cor-1 .statement}

*Toute extension algébrique d’un corps parfait est un corps parfait.*
Soient K un corps parfait d’exposant caractéristique $p$, et E une extension algébrique de K. Alors E est séparable sur K (V, p. 35, prop. 2), d’où $E = K(E^p)$ d’après la prop. 11 ; mais on a $K = K^p \subset E^p$, d’où $E = K(E^p) = E^p$, et par suite, E est parfait.

#### Corollaire 2 (MacLane) {#alg-v-s7-prop-11-cor-2 .statement}

*Soient $\overline{K}$ une clôture algébrique de K et $K^{p^{-\infty}}$ la clôture parfaite de K dans $\overline{K}$. Pour qu’une sous-extension E de $\overline{K}$ soit séparable sur K, il faut et il suffit qu’elle soit linéairement disjointe de $K^{p^{-\infty}}$ sur K.*
On se ramène immédiatement au cas où [E : K] est fini. Soit $(x_i)_{i \in I}$ une base de E sur K. Pour que E soit linéairement disjointe de $K^{p^{-\infty}}$, il faut et il suffit qu’elle le soit de $K^{p^{-n}}$ pour tout $n \geq 0$. Ceci signifie aussi que la relation $\sum_{i \in I} x_i a_i^{p^{-n}} = 0$ entraîne $a_i = 0$ pour tout $i \in I$, quelle que soit la famille $(a_i)_{i \in I}$ d’éléments de K. Ceci signifie encore que la famille $(x_i^{p^n})_{i \in I}$ est libre sur K, ou encore que c’est une base de l’espace vectoriel E sur K. Autrement dit, E est linéairement disjointe de $K^{p^{-n}}$ si et seulement si l’on a $E = K(E^{p^n})$. Il suffit alors d’appliquer la prop. 11.

#### Remarque 1 {#alg-v-s7-n6-rem-1 .statement}

Lorsque E est algébrique et de degré infini sur K, la condition $E = K(E^p)$ n’assure pas nécessairement que E soit séparable sur K. Par exemple, si K est imparfait et si E est une clôture parfaite de K, on a $E = K(E^p)$, mais E n’est pas extension séparable de K (V, p. 38, cor. 3).

#### Remarque 2 {#alg-v-s7-n6-rem-2 .statement}

Soit E une extension algébrique séparable d’un corps K d’exposant caractéristique $p$. On a alors $E^p \cap K = K^p$ (cor. 2) ; par suite, si E est parfait, il en est de même de K.

### 7. Fermeture algébrique séparable

#### Proposition 12 {#alg-v-s7-prop-12 .statement}

*Soient E une extension de K et $E_s$ l’ensemble des éléments de E qui sont algébriques et séparables sur K. Alors $E_s$ est la plus grande sous-extension de E qui soit algébrique et séparable sur K.*
D’après la prop. 6, *a*) (V, p. 38), toute sous-extension de E qui est algébrique et séparable sur K est contenue dans $E_s$. D’après la prop. 6, *b*) (*loc. cit.*), l’extension $K(E_s)$ de K est algébrique et séparable, d’où $K(E_s) \subset E_s$ et finalement $K(E_s) = E_s$.

Avec les notations de la proposition précédente, on dit que $E_s$ est la *fermeture* (algébrique) *séparable de K dans E*. Lorsque K est parfait, $E_s$ est la fermeture algébrique de K dans E (V, p. 35, prop. 2).

#### Proposition 13 {#alg-v-s7-prop-13 .statement}

*Soit E une extension algébrique de K, et soit $E_s$ la fermeture algébrique séparable de K dans E.*
a) *E est extension radicielle de $E_s$*.
b) *Si F est une sous-extension de E, telle que E soit radiciel sur F, on a $F \supset E_s$.*

c) $E_s$ est l’unique sous-extension de $E$ qui soit séparable sur $K$ et sur laquelle $E$ soit radicielle.

Il suffit de prouver a) dans le cas où $K$ est de caractéristique $p \neq 0$. Soit $x$ un élément de $E$, et soit $f$ son polynôme minimal sur $K$. Il existe un entier $m \geqslant 0$ tel que $f$ appartienne à $K[X^{p^m}]$, mais non à $K[X^{p^{m+1}}]$; autrement dit, on a $f(X) = g(X^{p^m})$ avec $g \in K[X]$, $g \notin K[X^p]$. Comme $f$ est irréductible, il en est de même de $g$, donc $g$ est le polynôme minimal de $x^{p^m}$ sur $K$. D’après V, p. 37, prop. 4 et p. 38, prop. 5, on a donc $x^{p^m} \in E_s$, donc $E$ est radiciel sur $E_s$.

Plaçons-nous sous les hypothèses de b), et soit $x \in E_s$. Comme $x$ est séparable sur $K$, il l’est aussi sur $F$ (V, p. 38, cor. 2); mais comme $E$ est radiciel sur $F$, $x$ est aussi radiciel sur $F$, d’où $x \in F$ (V, p. 38, cor. 3).

Enfin, c) résulte de a) et b) et de la prop. 12.

#### Corollaire 1 {#alg-v-s7-prop-13-cor-1 .statement}

*Soient* $E$ et $K'$ *deux extensions de* $K$, *contenues dans une même extension de* $K$. *On suppose que* $E$ *est algébrique sur* $K$ *et l’on note* $E_s$ *la fermeture algébrique séparable de* $K$ *dans* $E$. *Alors* $K'(E_s)$ *est la fermeture algébrique séparable de* $K'$ *dans* $K'(E)$.

En effet, $K'(E_s)$ est une extension algébrique séparable de $K'$ d’après la prop. 10 (V, p. 41); comme $E$ est radicielle sur $E_s$, l’extension $K'(E)$ de $K'(E_s)$ est radicielle (V, p. 24, cor.). Il suffit alors d’appliquer la prop. 13.

#### Corollaire 2 {#alg-v-s7-prop-13-cor-2 .statement}

*Si* $E$ *est de degré fini sur* $K$, *on a* $E_s = \bigcap_{n \geqslant 0} K(E^{p^n})$.

Pour tout entier $n \geqslant 0$, notons $F_n$ la sous-extension $K(E^{p^n})$ de $E$. La suite $(F_n)_{n \geqslant 0}$ de sous-espaces vectoriels de $E$ est décroissante et $E$ est de dimension finie sur $K$. Il existe donc un entier $m \geqslant 0$ tel que $F_m = F_n$ pour tout $n \geqslant m$. On a alors $K(F_m^p) = F_{m+1} = F_m$, donc $F_m$ est extension séparable de $K$ (V, p. 41, prop. 11); il est clair que $E$ est radiciel sur $F_m$ et la prop. 13 entraîne alors $E_s = F_m = \bigcap_{n \geqslant 0} F_n$.

#### Remarque {#alg-v-s7-n7-rem-1 .statement}

Soient $E$ une extension algébrique de $K$, et $E_r$ la fermeture radicielle de $E$ dans $K$ (V, p. 24). Alors $E_r$ est la plus grande sous-extension de $E$ qui soit radicielle sur $K$ (V, p. 24, prop. 2). Cependant $E$ n’est pas en général séparable sur $E_r$ (V, p. 145, exerc. 2); pour le cas des extensions quasi-galoisiennes, voir V, p. 73.

### 8. Clôture séparable d’un corps

#### Définition 4 {#alg-v-s7-def-4 .statement}

*On dit qu’un corps* $K$ *est séparablement clos si toute extension algébrique séparable de* $K$ *est triviale*.

Un corps algébriquement clos est séparablement clos. Réciproquement, si un corps *parfait* $K$ est séparablement clos, il est algébriquement clos, car toute extension algébrique de $K$ est séparable (V, p. 35, prop. 2).

#### Définition 5 {#alg-v-s7-def-5 .statement}

*Soit* $K$ *un corps*. *On appelle clôture algébrique séparable, ou par abus de langage clôture séparable, de* $K$ *toute extension* $E$ *de* $K$ *qui est algébrique et séparable sur* $K$, *et telle que le corps* $E$ *soit séparablement clos*.

Lorsque K est parfait, il y a identité entre les notions de clôture séparable et de clôture algébrique de K (V, p. 35, prop. 2 et p. 42, cor. 1).

#### Proposition 14 {#alg-v-s7-prop-14 .statement}

Soit $\Omega$ une extension algébriquement close de K.
a) La fermeture algébrique séparable $\Omega_s$ de K dans $\Omega$ est une clôture séparable de K.
b) Si E et E' sont deux clôtures séparables de K, il existe un K-isomorphisme de E sur E'.

Soit F une extension algébrique séparable de $\Omega_s$; comme $\Omega$ est algébriquement clos, il existe un $\Omega_s$-homomorphisme $u$ de F dans $\Omega$ (V, p. 20, th. 1). D’après la prop. 9 (V, p. 40), $u(F)$ est séparable sur K, donc $u(F) = \Omega_s$. Par suite, F est une extension triviale de $\Omega_s$, et $\Omega_s$ est séparablement clos, d’où a).

Soit E une clôture séparable de K. Comme E est une extension algébrique de K, il existe un K-homomorphisme $v$ de E dans $\Omega$ (V, p. 20, th. 1). Alors, $v(E)$ est algébrique séparable sur K, d’où $v(E) \subset \Omega_s$. D’après V, p. 40, prop. 9, $\Omega_s$ est séparable sur $v(E)$ et comme le corps $v(E)$ est séparablement clos, on a $v(E) = \Omega_s$. Par suite, $v$ est un K-isomorphisme de E sur $\Omega_s$. L’assertion b) résulte immédiatement de là.

#### Corollaire {#alg-v-s7-n8-cor-1 .statement}

Soient E une extension séparablement close de K et F une extension algébrique séparable de K. Il existe un K-homomorphisme de F dans E.

Soit $\Omega$ une clôture algébrique de E ; on a $\Omega_s \subset E$, et il suffit de traiter le cas où $E = \Omega_s$. Comme F est une extension algébrique de K, il existe un K-homomorphisme $u$ de F dans $\Omega$ (V, p. 20, th. 1). Comme le corps $u(F)$ est séparable sur K, on a $u(F) \subset \Omega_s$, et $u$ définit un K-homomorphisme de F dans $\Omega_s = E$.

#### Remarque 1 {#alg-v-s7-n8-rem-1 .statement}

Soient E et E' deux clôtures séparables de K. Si K n’est pas séparablement clos, il existe plusieurs K-isomorphismes de E sur E'. \* En effet, E est alors une extension galoisienne non triviale de K, et il existe donc des K-automorphismes de E distincts de l’identité (V, p. 54, th. 1). \*

#### Remarque 2 {#alg-v-s7-n8-rem-2 .statement}

\* Soit E une extension algébrique et séparable de K. Si toute extension algébrique et séparable de K est isomorphe à une sous-extension de E, alors E est une clôture séparable de K. En effet, si E' est une clôture séparable de K, chacune des extensions E et E' est isomorphe à une sous-extension de l’autre ; par suite, E et E' sont des extensions isomorphes de K (V, p. 50, prop. 1, a)). \*

### 9. Degrés séparable et inséparable d’une extension de degré fini

Soient E une extension de degré fini de K et $\Omega$ une clôture algébrique de K. Rappelons (V, p. 30) que l’on appelle degré séparable de E sur K, et que l’on note $[E : K]_s$, le nombre des K-homomorphismes de E dans $\Omega$.

#### Proposition 15 {#alg-v-s7-prop-15 .statement}

Soit $E_s$ la fermeture séparable de K dans E. On a $[E : K]_s = [E_s : K]$.

Le corps $\Omega$ est parfait, et E est radiciel sur $E_s$ d’après V, p. 42, prop. 13 ; par suite, la proposition 3 (V, p. 25) montre que tout K-homomorphisme de $E_s$ dans $\Omega$ se prolonge de manière unique en un K-homomorphisme de E dans $\Omega$; on a donc $[E : K]_s = [E_s : K]_s$. Comme $E_s$ est une extension séparable de degré fini de K, c’est une algèbre étale sur $K$, et l’on a donc $[E_s : K]_s = [E_s : K]$ d’après V, p. 31, prop. 4. D’où la proposition.

Avec les notations précédentes, on appelle *degré inséparable* de $E$ sur $K$, et l’on note $[E : K]_i$, le degré de $E$ sur $E_s$. On a donc

(1)
$$
[E : K] = [E : K]_s \cdot [E : K]_i
$$
d’après la proposition 15.

Lorsque $K$ est de caractéristique 0, on a $E = E_s$, d’où $[E : K]_s = [E : K]$ et $[E : K]_i = 1$. Si $K$ est de caractéristique $p \neq 0$, le nombre $[E : K]_i$ est une puissance de $p$ car $E$ est radiciel sur $E_s$ (V, p. 42, prop. 13 et p. 25, prop. 4). On prendra garde que $[E : K]_i$ n’est pas nécessairement égal à la plus grande puissance de $p$ qui divise $[E : K]$, ni au degré $[E_r : K]$ de la fermeture radicielle de $E$ dans $K$ (V, p. 145, exerc. 3 et 2).

#### Proposition 16 {#alg-v-s7-prop-16 .statement}

*Soient $\Omega$ une extension de $K$ et $E, F$ deux sous-extensions de $\Omega$, de degré fini sur $K$.*

a) *Si l’on a $E \subset F$, on a $[F : K]_s = [F : E]_s \cdot [E : K]_s$ et $[F : K]_i = [F : E]_i \cdot [E : K]_i$.*

b) *Soit $K'$ une sous-extension de $\Omega$. On a*
$$
[K'(E) : K']_s \leq [E : K]_s \quad \text{et} \quad [K'(E) : K']_i \leq [E : K]_i,
$$
*et il y a égalité si $K'$ est linéairement disjointe de $E$ sur $K$.*

c) *On a $[K(E \cup F) : K]_s \leq [E : K]_s \cdot [F : K]_s$ et $[K(E \cup F) : K]_i \leq [E : K]_i \cdot [F : K]_i$, et il y a égalité si $E$ et $F$ sont linéairement disjointes sur $K$.*

L’assertion sur les degrés séparables dans a) résulte de la formule (9) (V, p. 31). Comme on a $[F : K] = [F : E] \cdot [E : K]$, l’assertion sur les degrés inséparables résulte de là et de la formule (1).

D’après le cor. 1 de la prop. 13 (V, p. 43) et la prop. 15, on a

(2)
$$
[K'(E) : K']_s = [K'(E_s) : K'] , \quad [K'(E) : K']_i = [K'(E) : K'(E_s)] ;
$$
lorsque $K'$ est linéairement disjointe de $E$ sur $K$, alors $E_s$ est linéairement disjointe de $K'$ sur $K$ et $E$ est linéairement disjointe de $K'(E_s)$ sur $E_s$ (V, p. 14, prop. 8). L’assertion b) résulte alors de la prop. 5 (V, p. 13).

D’après *a)*, on a $[K(E \cup F) : K]_s = [F(E) : F]_s \cdot [F : K]_s$; d’après *b)*, on a $[F(E) : F]_s \leq [E : K]_s$, avec égalité si $E$ et $F$ sont linéairement disjointes sur $K$. On en déduit l’inégalité $[K(E \cup F) : K]_s \leq [E : K]_s \cdot [F : K]_s$, avec égalité si $E$ et $F$ sont linéairement disjointes sur $K$. L’assertion de *c)* sur les degrés inséparables se démontre de manière analogue.

## EXERCICES {#alg-v-s7-exercises}

See the [exercises for § 7](exercises/s7/).
