---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 9
section_title: ÉLÉMENTS CONJUGUÉS ET EXTENSIONS QUASI-GALOISIENNES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.50-A V.54, A V.146-A V.147
pdf_pages: 0154-0158, 0250-0251
extraction: ocr
subsections:
    - "no": 1
      title: Prolongement d’isomorphismes
      page: 50
      pdf_page: 154
    - "no": 2
      title: Extensions conjuguées. Éléments conjugués
      page: 50
      pdf_page: 154
    - "no": 3
      title: Extensions quasi-galoisiennes
      page: 52
      pdf_page: 156
    - "no": 4
      title: Extension quasi-galoisienne engendrée par un ensemble
      page: 53
      pdf_page: 157
statements: 19
exercises: 8
content_sha256: 9fea7e217246bdeb7cc834eb5a29cb9390bec66d9e459b4628079d553f8a1261
---

## § 9. ÉLÉMENTS CONJUGUÉS ET EXTENSIONS QUASI-GALOISIENNES

Dans tout ce paragraphe, on note $K$ un corps et $\Omega$ une clôture algébrique de $K$.

### 1. Prolongement d’isomorphismes

#### Proposition 1 {#alg-v-s9-prop-1 .statement}

Soient $E$ une extension de $K$ contenue dans $\Omega$ et $u$ un $K$-homomorphisme de $E$ dans $\Omega$.
a) Si $u$ applique $E$ dans $E$, $u$ induit un $K$-automorphisme de $E$.
b) Il existe un $K$-automorphisme $v$ de $\Omega$ prolongeant $u$.

Supposons qu’on ait $u(E) \subset E$; pour prouver a), il suffit de montrer que l’on a $u(E) = E$. Soient $x$ un élément de $E$, $f$ le polynôme minimal de $x$ sur $K$ et $\Phi$ l’ensemble des racines de $f$ dans $E$. L’ensemble $\Phi$ est fini, l’application $u$ de $E$ dans $E$ est injective, et l’on a $u(\Phi) \subset \Phi$. On a par suite $u(\Phi) = \Phi$, d’où $x \in u(\Phi) \subset u(E)$; on a donc $E = u(E)$.

Il est clair que $\Omega$ est une clôture algébrique de $E$ et de $u(E)$; par suite (V, p. 23, cor.), l’isomorphisme $u$ de $E$ sur $u(E)$ se prolonge en un isomorphisme $v$ de $\Omega$ sur $\Omega$.

### 2. Extensions conjuguées. Éléments conjugués

#### Définition 1 {#alg-v-s9-def-1 .statement}

Soient $E$ et $F$ deux extensions de $K$ contenues dans $\Omega$. On dit que $E$ et $F$ sont conjuguées (dans $\Omega$) s’il existe un $K$-automorphisme $u$ de $\Omega$ tel que $u(E) = F$. On dit que deux éléments $x$ et $y$ de $\Omega$ sont conjugués sur $K$ s’il existe un $K$-automorphisme $u$ de $\Omega$ tel que $u(x) = y$.

Soient $E$ et $F$ deux extensions de $K$ contenues dans $\Omega$. D’après la prop. 1, $E$ et $F$ sont conjuguées sur $K$ si et seulement si ce sont des extensions isomorphes de $K$. Il en est ainsi en particulier s’il existe deux parties $A$ et $B$ de $\Omega$ telles que $E = K(A)$ et $F = K(B)$ et un $K$-automorphisme $u$ de $\Omega$ tel que $u(A) = B$.

La relation « x et y sont conjugués sur K » est une relation d’équivalence dans $\Omega$ ; les classes suivant cette relation s’appellent les classes de conjugaison dans $\Omega$ ; ce sont les orbites dans $\Omega$ du groupe des K-automorphismes de $\Omega$.

#### Proposition 2 {#alg-v-s9-prop-2 .statement}

Soient x et y deux éléments de $\Omega$. Les conditions suivantes sont équivalentes :
a) x et y sont conjugués sur K.
b) Il existe un K-isomorphisme v de K(x) sur K(y) tel que $v(x) = y$.
c) x et y ont le même polynôme minimal sur K.
Supposons d’abord que x et y soient conjugués sur K ; soit u un K-automorphisme de $\Omega$ tel que $u(x) = y$ et soit f le polynôme minimal de x sur K. On a
$$
f(y) = f(u(x)) = u(f(x)) = 0,
$$
et f est un polynôme unitaire irréductible dans K[X] ; par suite (V, p. 16, th. 1, c)), f est le polynôme minimal de y sur K. Donc a) entraîne c).
Supposons maintenant que x et y aient même polynôme minimal f sur K. Il existe un K-isomorphisme du corps K[X]/(f) sur K(x) (resp. sur K(y)) transformant la classe de X modulo (f) en x (resp. y) (V, p. 16, th. 1, b)) ; il existe donc un K-isomorphisme v de K(x) sur K(y) tel que $v(x) = y$. Par suite, c) entraîne b).
Enfin, sous les hypothèses de b), la prop. 1 entraîne l’existence d’un K-automorphisme u de $\Omega$ prolongeant v ; on a alors $u(x) = y$, donc x et y sont conjugués sur K. Par suite, b) entraîne a).

#### Corollaire 1 {#alg-v-s9-prop-2-cor-1 .statement}

Soit x un élément de $\Omega$, de degré n sur K, et soit f le polynôme minimal de x sur K. Les conjugués de x sur K sont les racines de f dans $\Omega$, et leur nombre est au plus égal à n.

#### Corollaire 2 {#alg-v-s9-prop-2-cor-2 .statement}

Soit x un élément de $\Omega$, de degré n sur K. Pour que x soit séparable sur K, il faut et il suffit qu’il ait n conjugués dans $\Omega$ ; s’il en est ainsi, tous les conjugués de x sur K sont séparables sur K.
Soit f le polynôme minimal de x sur K ; ses racines sont les conjugués de x sur K, et chacune de ces racines admet f pour polynôme minimal sur K. Or x est séparable sur K si et seulement si le polynôme f est séparable (V, p. 38, prop. 5), c’est-à-dire si f a n racines distinctes dans $\Omega$. Le cor. 2 résulte de là.

#### Corollaire 3 {#alg-v-s9-prop-2-cor-3 .statement}

Soit G le groupe des K-automorphismes de $\Omega$. L’ensemble des invariants de G dans $\Omega$ est la fermeture radicielle de K dans $\Omega$ (V, p. 24).
En d’autres termes, un élément x de $\Omega$ est radiciel sur K si et seulement s’il ne possède aucun conjugué distinct de lui-même.
Soit p l’exposant caractéristique, et soit $x \in \Omega$. D’après V, p. 42, prop. 13, il existe un entier $m \geq 0$ tel que $y = x^{p^m}$ soit algébrique et séparable sur K. Or x est invariant par G si et seulement si y est invariant par G ; d’après le cor. 2, ceci a lieu si et seulement si y est de degré 1 sur K, ce qui équivaut à $y \in K$. Le corollaire résulte aussitôt de là.

### 3. Extensions quasi-galoisiennes

#### Définition 2 {#alg-v-s9-def-2 .statement}

Soit E une extension de K. On dit que E est quasi-galoisienne, ou normale (sur K), si elle est algébrique et si tout polynôme irréductible de K[X], ayant au moins une racine dans E, se décompose en produit de polynômes de degré 1 (distincts ou non) dans E[X].

Si E est une clôture algébrique de K, c’est une extension quasi-galoisienne de L ; en effet, la condition (AC) de la prop. 1 (V, p. 19) affirme que tout polynôme non constant dans E[X] est produit de polynômes de degré 1.

#### Proposition 3 {#alg-v-s9-prop-3 .statement}

Soit E une extension de K contenue dans Ω. Les conditions suivantes sont équivalentes :
a) E est une extension quasi-galoisienne de K.
b) Pour tout x ∈ E, les conjugués de x sur K dans Ω appartiennent à E.
c) Tout K-automorphisme de Ω applique le corps E dans lui-même.
d) Tout K-homomorphisme de E dans Ω applique le corps E dans lui-même.
e) E est l’extension de décomposition dans Ω d’une famille (f_i)_{i∈I} de polynômes non constants dans K[X] (V, p. 23, remarque 3).

L’équivalence de c) et d) provient de ce que tout K-homomorphisme de E dans Ω est induit par un K-automorphisme de Ω (V, p. 50, prop. 1).

Par définition, une extension quasi-galoisienne est le corps de décomposition de la famille des polynômes minimaux (sur K) de ses éléments, donc a) entraîne e). Sous les hypothèses de e), soit u un automorphisme de Ω ; pour tout i ∈ I, u permutte l’ensemble R_i des racines de f_i, et comme on a E = K(∪_{i∈I} R_i), on a u(E) = E ; donc e) entraîne c). La définition des éléments conjugués montre que c) entraîne b). Supposons enfin b) vérifiée ; soit f un polynôme unitaire irréductible dans K[X] admettant au moins une racine x dans E ; comme Ω est algébriquement clos, il existe des éléments a_k de Ω (1 ≤ k ≤ n) tels que f(x) = ∏_{k=1}^n (X - a_k), et comme les a_k sont conjugués de x sur K (V, p. 51, cor. 1), ils appartiennent à E par hypothèse. On a prouvé que b) entraîne a).

#### Corollaire 1 {#alg-v-s9-prop-3-cor-1 .statement}

Pour qu’une extension E de K contenue dans Ω soit quasi-galoisienne, il faut et il suffit qu’elle soit identique à toutes ses conjuguées sur K.

Cela résulte de la prop. 1, a) (V, p. 50) et de l’équivalence des conditions a) et c) de la prop. 3.

#### Corollaire 2 {#alg-v-s9-prop-3-cor-2 .statement}

Soient E et F deux extensions algébriques de K telles que E ⊂ F. Si F est quasi-galoisienne sur K, elle est quasi-galoisienne sur E.

On peut supposer que F ⊂ Ω. Soit u un E-automorphisme de Ω. Comme u est un K-automorphisme de Ω et que F est quasi-galoisienne sur K, on a u(F) = F. Par suite, F est quasi-galoisienne sur E.

#### Corollaire 3 {#alg-v-s9-prop-3-cor-3 .statement}

Soient N une extension quasi-galoisienne de K contenue dans Ω, et E une sous-extension de N. Soit u un K-homomorphisme de E dans Ω ; on a u(E) ⊂ N et il existe un K-automorphisme v de N qui induit u sur E.

Soit w un K-automorphisme de Ω prolongeant u (V, p. 50, prop. 1) ; comme N est quasi-galoisienne sur K, on a w(N) = N d’où u(E) ⊂ N, et w induit un K-automorphisme v de N.

#### Corollaire 4 {#alg-v-s9-prop-3-cor-4 .statement}

Soient E' une extension de K, et E, K' deux sous-extensions de E'. On suppose que E est quasi-galoisienne sur K et que E' = K'(E). Alors E' est quasi-galoisienne sur K'.

Soit (f_i)_{i \in I} une famille de polynômes non constants dans K[X] dont E soit le corps de décomposition sur K. Il est immédiat que E' est le corps de décomposition de la famille (f_i)_{i \in I} sur K', donc est quasi-galoisienne sur K'.

#### Remarque 1 {#alg-v-s9-n3-rem-1 .statement}

Soient F une extension de K et E une sous-extension de F ; on suppose que E est quasi-galoisienne sur K. Montrons que tout K-automorphisme u de F laisse invariant E. En effet, soient x \in E et f le polynôme minimal de x sur K. Comme E est quasi-galoisienne sur K, il existe a_1, ..., a_n \in E tels que f(X) = \Pi(X - a_i) ; on a f(u(x)) = u(f(x)) = 0, donc u(x) est l’un des a_i, donc appartient à E. On a prouvé l’inclusion u(E) \subset E, d’où u(E) = E par V, p. 50, prop. 1.

#### Remarque 2 {#alg-v-s9-n3-rem-2 .statement}

Supposons que E soit une extension quasi-galoisienne de K et F une extension quasi-galoisienne de E ; il n’est pas toujours vrai que F soit quasi-galoisienne sur K (V, p. 146, exerc. 1). La raison en est la suivante : soit u un K-automorphisme de Ω ; on a u(E) = E, mais, si f est le polynôme minimal sur E d’un élément x de F, il n’est pas nécessairement invariant par u ; par suite, u(x) n’est pas nécessairement conjugué de x sur E et n’appartient donc pas nécessairement à F. Dans ce cas, F et u(F) sont deux extensions quasi-galoisiennes distinctes de E, qui sont K-isomorphes, mais non E-isomorphes.

#### Remarque 3 {#alg-v-s9-n3-rem-3 .statement}

Soient E une extension algébrique de K et x, y deux éléments de E. S’il existe un K-automorphisme de E transformant x en y, alors x et y ont même polynôme minimal sur K et sont donc conjugués sur K d’après la prop. 2 (V, p. 51). La réciproque est vraie si E est quasi-galoisienne, car tout K-automorphisme de Ω induit un K-automorphisme de E. L’hypothèse que E est quasi-galoisienne n’est pas superflue, comme le montre l’exemple suivant : \* soient K = Q et Ω le corps des nombres algébriques ; posons E = Ω \cap \mathbf{R}. On peut montrer (V, p. 146, exerc. 2) que tout automorphisme de E est l’application identique, et que $\sqrt{2}$ et $-\sqrt{2}$ sont des éléments de E conjugués sur Q. \*

### 4. Extension quasi-galoisienne engendrée par un ensemble

#### Proposition 4 {#alg-v-s9-prop-4 .statement}

Soit (N_i)_{i \in I} une famille d’extensions quasi-galoisiennes de K contenues dans Ω. Soient N = \bigcap_{i \in I} N_i et M = K(\bigcup_{i \in I} N_i) ; les extensions N et M de K sont quasi-galoisiennes.

Soit u un K-automorphisme de Ω. On a u(N_i) = N_i pour tout i \in I et l’on déduit évidemment de là les égalités u(N) = N et u(M) = M ; la proposition résulte alors du cor. 1 (V, p. 52).

Soit A un ensemble d’éléments de Ω. Soit B l’ensemble des éléments de Ω qui sont conjugués d’un élément de A ; autrement dit, si G est le groupe des K-auto-morphismes de Ω, on a B = $\bigcup_{u \in G} u(A)$. Pour tout $u \in G$, on a $u(B) = B$, d’où $u(K(B)) = K(B)$. Par suite, K(B) est une extension quasi-galoisienne de K contenant A, et il est immédiat que toute extension quasi-galoisienne N de K contenant A contient B, donc K(B). On dira que K(B) est l’extension quasi-galoisienne engendrée par A. Cette définition s’applique en particulier lorsque A est une extension de K.

La proposition suivante résulte immédiatement de ce qui précède.

#### Proposition 5 {#alg-v-s9-prop-5 .statement}

*Soient E une extension de K contenue dans Ω et N l’extension quasi-galoisienne engendrée par E. Si A est une partie de Ω telle que E = K(A), on a N = K(B), où B est l’ensemble des éléments de Ω qui sont conjugués à un élément de A.*

#### Corollaire 1 {#alg-v-s9-prop-5-cor-1 .statement}

*Si E est une extension de degré fini de K, l’extension quasi-galoisienne N de K engendrée par E est de degré fini sur K.*
On a en effet E = K(A) où A est fini, donc l’ensemble B des conjugués des éléments de A est fini, d’où le corollaire par le th. 2 (V, p. 17).

#### Corollaire 2 {#alg-v-s9-prop-5-cor-2 .statement}

*Toute extension quasi-galoisienne N de K est réunion des sous-extensions quasi-galoisiennes de N, de degré fini sur K.*
Soit $x \in N$ et soit $N_x$ l’extension quasi-galoisienne de K engendrée par $\{x\}$. Comme K(x) est de degré fini sur K, il en est de même de $N_x$ (cor. 1), et l’on a $x \in N_x$.

## EXERCICES {#alg-v-s9-exercises}

See the [exercises for § 9](exercises/s9/).
