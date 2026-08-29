---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 4
section_title: EXTENSIONS ALGÉBRIQUEMENT CLOSES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.19-A V.23, A V.143-A V.144
pdf_pages: 0123-0127, 0247-0248
extraction: ocr
subsections:
    - "no": 1
      title: Corps algébriquement clos
      page: 19
      pdf_page: 123
    - "no": 2
      title: Extensions de décomposition
      page: 20
      pdf_page: 124
    - "no": 3
      title: Clôture algébrique d’un corps
      page: 22
      pdf_page: 126
statements: 17
exercises: 2
content_sha256: 534e509dbe20f60353cda50139274b7157fc2a4cff637503dab87467c16be3b5
---

## § 4. EXTENSIONS ALGÉBRIQUEMENT CLOSES

### 1. Corps algébriquement clos

#### Proposition 1 {#alg-v-s4-prop-1 .statement}

Soit K un corps. Les propriétés suivantes sont équivalentes :
(AC) Tout polynôme non constant de K[X] se décompose dans K[X] en un produit de polynômes de degré 1 (distincts ou non).
(AC') Tout polynôme non constant de K[X] a au moins une racine dans K.
(AC'') Tout polynôme irréductible dans K[X] est de degré 1.
(AC''') Toute extension algébrique de K est de degré 1 (autrement dit, K est algébriquement fermé dans tout surcorps de K).

Montrons d’abord que les propriétés (AC), (AC') et (AC'') sont équivalentes. Il est clair que (AC) entraîne (AC''). Comme tout polynôme non constant de K[X] est divisible par un polynôme irréductible (IV, p. 13, prop. 13) et que tout polynôme de degré 1 dans K[X] admet évidemment une racine dans K, on voit que (AC'') entraîne (AC'). La condition (AC') entraîne par récurrence sur n que tout polynôme de degré n dans K[X] est produit de n polynômes de degré 1 (IV, p. 14, prop. 1), donc (AC') entraîne (AC).

Il reste à voir que les propriétés (AC'') et (AC''') sont équivalentes. Si (AC'') est vérifiée, tout élément d’un surcorps L de K algébrique sur K est de degré 1 (V, p. 15, th. 1), donc appartient à K, ce qui établit (AC'''). Réciproquement, soit f un polynôme irréductible de degré n ≥ 1 dans K[X] ; l’algèbre quotient K[X]/(f) est de degré n sur K, et c’est un corps, donc une extension algébrique de degré n de K (V, p. 17, prop. 2). Il est alors clair que (AC''') entraîne (AC'').

#### Définition 1 {#alg-v-s4-def-1 .statement}

On dit qu’un corps K est algébriquement clos s’il possède les quatre propriétés (équivalentes) (AC), (AC'), (AC'') et (AC'''').

\* Exemple 1. — Le corps C des nombres complexes est algébriquement clos (TG, VIII, p. 1). \*
Un corps K algébriquement fermé dans un surcorps E de K n’est pas nécessairement algébriquement clos (tout corps est en effet algébriquement fermé dans luimême et il existe des corps non algébriquement clos, par exemple $\mathbf{Q}$ ou $\mathbf{F}_p$ \* ou $\mathbf{R}$ *) ; cependant :

#### Proposition 2 {#alg-v-s4-prop-2 .statement}

*Soient $\Omega$ un corps algébriquement clos et $K$ un sous-corps de $\Omega$. La fermeture algébrique $\overline{K}$ de $K$ dans $\Omega$ est un corps algébriquement clos.*

Soit $f$ un polynôme non constant dans $\overline{K}[X] \subset \Omega[X]$. Comme $\Omega$ est algébriquement clos, le polynôme $f$ a au moins une racine *dans* $\Omega$, et comme cette racine est algébrique sur $\overline{K}$, elle appartient à $\overline{K}$ (V, p. 19, prop. 4). Par suite, $\overline{K}$ satisfait à (AC').

#### Exemple 2 {#alg-v-s4-n1-exa-2 .statement}

D’après la prop. 2, l’ensemble des nombres complexes algébriques sur $\mathbf{Q}$ (appelés souvent en abrégé *nombres algébriques*) est un corps algébriquement clos. \*

#### Proposition 3 {#alg-v-s4-prop-3 .statement}

*Tout corps algébriquement clos est infini.*

Soit $K$ un corps fini ; posons $f(X) = 1 + \prod_{a \in K} (X - a)$. Le polynôme $f \in K[X]$ est non constant et l’on a $f(a) = 1$ pour tout $a \in K$. Le corps $K$ ne satisfait pas à (AC'), donc n’est pas algébriquement clos.

**Théorème 1** (Steinitz). — *Soient $K$ un corps, $E$ une extension algébrique de $K$ et $\Omega$ une extension algébriquement close de $K$. Il existe un $K$-homomorphisme de $E$ dans $\Omega$.*

D’après V, p. 13, scholie, il existe un surcorps $\Omega'$ de $\Omega$ et un $K$-homomorphisme $u$ de $E$ dans $\Omega'$. Soit $x \in E$; comme $x$ est algébrique sur $K$, $u(x)$ est algébrique sur $u(K)$ et *a fortiori* sur $\Omega$ (V, p. 16, cor. 2); comme $\Omega$ est algébriquement clos, on a donc $u(x) \in \Omega$. Par suite, $u$ applique $E$ dans $\Omega$.

### 2. Extensions de décomposition

#### Définition 2 {#alg-v-s4-def-2 .statement}

*Soient $K$ un corps et $(f_i)_{i \in I}$ une famille de polynômes non constants dans $K[X]$. On appelle extension de décomposition de $(f_i)_{i \in I}$ toute extension $E$ de $K$ qui possède les propriétés suivantes :

a) Pour tout $i \in I$, le polynôme $f_i$ se décompose dans $E[X]$ en produit de polynômes de degré 1.

b) Pour tout $i \in I$, soit $R_i$ l’ensemble des racines de $f_i$ dans $E$. On a $E = K(\bigcup_{i \in I} R_i)$.*

On dit parfois « *corps de décomposition* » au lieu de « *extension de décomposition* ».

d’un polynôme en facteurs irréductibles dans E[X] (IV, p. 13, prop. 13), on montre facilement qu’une extension de décomposition pour le polynôme $f$ est une extension de décomposition pour la famille $(f_i)_{i\in I}$, et réciproquement. Autrement dit, le cas d’une famille finie se ramène au cas d’un seul polynôme.

3) Soit $f \in K[X]$ un polynôme de degré $n \geq 1$, et soit $E$ une extension de décomposition de $f$. Si $x_1, ..., x_n$ sont les racines de $f$ dans $E$, on a donc $E = K(x_1, ..., x_n)$ et $[E : K]$ est fini (V, p. 17, th. 2); mais il se peut que $E$ soit distinct des sous-corps $K(x_1), ..., K(x_n)$ engendrés par une seule racine; ceci peut se produire même lorsque $f$ est irréductible $^1$. Remarquons cependant que, lorsque $f$ est irréductible, les corps $K(x_i)$ sont tous de degré $n$ sur $K$, et dès que $E$ est égal à l’un d’eux, on a $[E : K] = n$ donc $E = K(x_1) = ... = K(x_n)$.

#### Proposition 4 {#alg-v-s4-prop-4 .statement}

*Soient $K$ un corps et $(f_i)_{i\in I}$ une famille de polynômes non constants dans $K[X]$. Il existe une extension de décomposition pour la famille $(f_i)_{i\in I}$*.

On peut supposer les polynômes $f_i$ unitaires (remarque 1). Soit $i \in I$ et soit $d_i$ le degré de $f_i$. D’après IV, p. 68, prop. 5, il existe une algèbre commutative $A_i$ sur $K$, non réduite à 0, et des éléments $\xi_{i,1}, ..., \xi_{i,d_i}$ de $A_i$ tels que :

a) l’algèbre $A_i$ est engendrée par $(\xi_{i,1}, ..., \xi_{i,d_i})$;

b) on a $f_i(X) = \prod_{k=1}^{d_i} (X - \xi_{i,k})$ dans $A_i[X]$.

Soit $A$ le produit tensoriel de la famille d’algèbres $(A_i)_{i\in I}$, et soit $\varphi_i$ l’homomorphisme canonique de $A_i$ dans $A$ (III, p. 42 ). L’algèbre $A$ est commutative et non réduite à 0 ; d’après le théorème de Krull (I, p. 99), il existe donc un idéal maximal $a$ de $A$ et $E = A/a$ est une extension du corps $K$.

Notons $\psi$ l’homomorphisme canonique de $A$ dans $E$ et posons $x_{i,k} = \psi(\varphi_i(\xi_{i,k}))$ pour $i \in I$ et $1 \leq k \leq d_i$. Comme l’algèbre $A$ est engendrée par $\bigcup_{i\in I} \varphi_i(A_i)$, l’extension $E$ est engendrée par la famille $(x_{i,k})$. De plus, on a $f_i(X) = \prod_{k=1}^{d_i} (X - x_{i,k})$ dans $E[X]$.

Par suite, $E$ est une extension de décomposition de la famille $(f_i)_{i\in I}$.

#### Proposition 5 {#alg-v-s4-prop-5 .statement}

*Soient $K$ un corps, $(f_i)_{i\in I}$ une famille de polynômes non constants dans $K[X]$, $E$ une extension de $K$, $F$ et $F'$ des sous-extensions de $E$ qui sont chacune extension de décomposition de $(f_i)_{i\in I}$. Alors $F = F'$*.

Soit $R_i$ l’ensemble des racines de $f_i$ dans $E$ et soit $R = \bigcup_{i\in I} R_i$. Comme $f_i$ est produit de polynômes du premier degré appartenant à $F[X]$, on a $R_i \subset F$. D’après la déf. 2, on a $F = K(R)$. On prouve de même que l’on a $F' = K(R)$.

#### Corollaire {#alg-v-s4-n2-cor-1 .statement}

*Soient $K$ un corps, $(f_i)_{i\in I}$ une famille de polynômes non constants dans $K[X]$, et $F, F'$ des extensions de décomposition de $(f_i)_{i\in I}$. Il existe un $K$-isomorphisme de $F$ sur $F'$*.

Cela résulte de la prop. 5 et de V, p. 12, cor. de la prop. 4.

$^1$ Prendre par exemple $K = \mathbf{Q}$ et $f = X^3 - 2$.

### 3. Clôture algébrique d’un corps

#### Définition 3 {#alg-v-s4-def-3 .statement}

Soit K un corps. On appelle clôture algébrique de K toute extension de K qui est algébrique et algébriquement close.

#### Exemple 1 {#alg-v-s4-n3-exa-1 .statement}

Le corps C des nombres complexes est une clôture algébrique du corps R des nombres réels (TG, VIII, p. 1). \*
2) Soient K un corps et Ω une extension algébriquement close de K. Soit $\overline{K}$ la fermeture algébrique de K dans Ω. D’après V, p. 20, prop. 2, $\overline{K}$ est une clôture algébrique de K. \* En particulier, le corps des nombres algébriques (V, p. 20, exemple 2) est une clôture algébrique du corps Q des nombres rationnels. \*

#### Proposition 6 {#alg-v-s4-prop-6 .statement}

Soit Ω une extension d’un corps K. Pour que Ω soit une clôture algébrique de K, il faut et il suffit qu’elle soit algébrique et que tout polynôme non constant dans K[X] se décompose dans Ω[X] en produit de facteurs de degré 1.

La condition est nécessaire d’après (AC). Réciproquement, supposons que Ω soit algébrique sur K et que tout polynôme non constant dans K[X] soit produit dans Ω[X] de polynômes de degré 1. Soit Ω′ une extension algébrique de Ω et soit $x \in \Omega'$. Comme x est algébrique sur Ω et que Ω est algébrique sur K, x est algébrique sur K (V, p. 18, prop. 3). Soit f le polynôme minimal de x sur K. Par hypothèse, le polynôme $f \in K[X]$ se décompose dans Ω[X] en produit de polynômes de degré 1, d’où $x \in \Omega$. On a donc $\Omega' = \Omega$ et le corps Ω est algébriquement clos, car il satisfait à (AC''').

#### Remarque 1 {#alg-v-s4-n3-rem-1 .statement}

Si Ω est algébrique sur K et si tout polynôme non constant de K[X] possède une racine dans Ω, alors Ω est une clôture algébrique de K (V, p. 151, exerc. 20).

#### Proposition 7 {#alg-v-s4-prop-7 .statement}

Soit Ω une extension algébrique d’un corps K.

a) Si Ω est algébriquement close, toute extension algébrique de K est isomorphe à une sous-extension de Ω.

b) Réciproquement, supposons que toute extension algébrique de degré fini de K soit isomorphe à une sous-extension de Ω. Alors Ω est algébriquement close.

L’assertion a) résulte du th. 1 (V, p. 20). Plaçons-nous sous les hypothèses de b) et considérons un polynôme non constant $f \in K[X]$. Soit E un corps de décomposition de f (V, p. 21, prop. 4) : comme E est algébrique de degré fini sur K (V, p. 17, th. 2), on peut supposer que E est une sous-extension de Ω. Le polynôme f est alors produit de polynômes de degré 1 dans Ω[X] et la prop. 6 montre que Ω est algébriquement close.

Nous pouvons maintenant prouver l’existence et l’unicité (à un isomorphisme près) de la clôture algébrique d’un corps.

#### Théorème 2 (Steinitz) {#alg-v-s4-thm-2 .statement}

Soit K un corps. Il existe une clôture algébrique de K ; si Ω et Ω′ sont deux clôtures algébriques de K, il existe un K-isomorphisme de Ω sur Ω′.

D’après la prop. 6, une clôture algébrique de K n’est autre qu’une extension de décomposition de l’ensemble des polynômes non constants dans K[X]. Le th. 2 résulte alors de V, p. 21, prop. 4, et de V, p. 21, cor.

#### Corollaire {#alg-v-s4-n3-cor-1 .statement}

Soient K et K’ deux corps, Ω une clôture algébrique de K et Ω’ une clôture algébrique de K’. Pour tout isomorphisme u de K sur K’, il existe un isomorphisme v de Ω sur Ω’ prolongeant u.
Il suffit d’appliquer le th. 2 aux clôtures algébriques Ω et (Ω’, u) de K.

#### Remarque 2 {#alg-v-s4-n3-rem-2 .statement}

Avec les notations du corollaire précédent, il existe en général des K-automorphismes de Ω distincts de l’identité. Il n’y a donc pas en général unicité de l’isomorphisme v de Ω sur Ω’ prolongeant l’isomorphisme u de K sur K’. Pour des raisons analogues, il y a en général plus d’un isomorphisme d’une extension de décomposition E sur une extension de décomposition E’ pour la même famille (f_i)_{i\in I} de polynômes. Rappelons par contre que, pour la clôture parfaite, on a un résultat d’unicité (V, p. 5).
3) Soient K un corps et Ω une clôture algébrique de K. On peut donner la construction suivante d’une extension de décomposition pour une famille (f_i)_{i\in I} de polynômes non constants dans K[X] : soit R_i l’ensemble des racines de f_i dans Ω, et soit R = \bigcup_{i\in I} R_i. Alors K(R) est l’unique sous-extension de Ω qui soit une extension de décomposition pour (f_i)_{i\in I} (V, p. 21, prop. 5).
4) Soient K un corps fini et Ω une clôture algébrique de K. Alors Ω est infini (V, p. 20, prop. 3); comme toute extension de degré fini de K est un corps fini, Ω est une extension algébrique de degré infini de K.

## EXERCICES {#alg-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
