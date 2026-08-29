---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 3
section_title: EXTENSIONS ALGÉBRIQUES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.141-A V.143
pdf_pages: 0119-0123, 0245-0247
extraction: ocr
subsections:
    - "no": 1
      title: Éléments algébriques d’une algèbre
      page: 0
      pdf_page: 119
    - "no": 2
      title: Extensions algébriques
      page: 17
      pdf_page: 121
    - "no": 3
      title: Transitivité des extensions algébriques. Corps algébriquement fermé dans un surcorps
      page: 18
      pdf_page: 122
statements: 18
exercises: 15
content_sha256: 9262483c395c6781ac05cafecb34b42d034090ceee902dd8ae01fb18f81b56e0
---

## § 3. EXTENSIONS ALGÉBRIQUES

### 1. Éléments algébriques d’une algèbre

Soient A une algèbre sur un corps K et x un élément de A. Deux cas sont possibles :

a) La famille des monômes $(x^n)_{n \in \mathbf{N}}$ est libre sur K. On dit alors que x est transcendant sur K. Il existe un isomorphisme de l’algèbre de polynômes $K[X]$ sur la sous-algèbre $K[x]$ de A engendrée par x, et cette dernière est de degré infini sur K.

b) Il existe un entier $n \geq 1$ tel que les monômes $1, x, ..., x^{n-1}, x^n$ soient linéairement dépendants ; il revient au même de dire qu’il existe un polynôme $f \neq 0$ dans $K[X]$ tel que $f(x) = 0$. On dit alors que x est algébrique sur K. Le plus petit entier $n \geq 1$ satisfaisant à la propriété précédente s’appelle le degré de x sur K. Si n est le degré de x sur K, les monômes $1, x, ..., x^{n-1}$ sont linéairement indépendants sur K et il existe des éléments $a_0, a_1, ..., a_{n-1}$ de K tels que

$$
x^n = a_0 + a_1 x + \cdots + a_{n-1} x^{n-1}.
$$

Le polynôme $f(X) = X^n - \sum_{k=0}^{n-1} a_k X^k$ est l’unique polynôme unitaire de degré n dans $K[X]$ tel que $f(x) = 0$; on l’appelle le polynôme minimal de x sur K.

#### Théorème 1 {#alg-v-s3-thm-1 .statement}

Soient A une algèbre sur un corps K, x un élément de A algébrique sur K, n le degré et f le polynôme minimal de x sur K.

a) Pour qu’un polynôme $g \in K[X]$ soit tel que $g(x) = 0$, il faut et il suffit que g soit multiple de f.

b) L’application $g \mapsto g(x)$ définit par passage au quotient un isomorphisme de l’algèbre quotient $K[X]/(f)$ sur l’algèbre $K[x]$, et les éléments $1, x, \ldots, x^{n-1}$ forment une base de $K[x]$ sur $K$. En particulier, on a $[K[x]:K] = n$.

c) Supposons que $A$ soit intègre. Alors l’anneau $K[x]$ est un corps, et $f$ est l’unique polynôme unitaire irréductible dans $K[X]$ tel que $f(x) = 0$.

d) Pour que $x$ soit inversible dans $A$, il faut et il suffit qu’on ait $f(0) \neq 0$. On a alors $x^{-1} \in K[x]$.

Il existe un unique homomorphisme d’algèbres $\varphi : K[X] \to A$ tel que $\varphi(X) = x$; on a $\varphi(P) = P(x)$ pour tout $P \in K[X]$ et l’image de $\varphi$ est égale à $K[x]$. Soit $a$ le noyau de $\varphi$; par construction, le polynôme minimal $f$ de $x$ sur $K$ appartient à $a$ et c’est le polynôme unitaire de plus petit degré dans $a$. Par suite (IV, p. 11, prop. 11), on a $a = (f)$, d’où a). L’assertion b) résulte aussitôt de a) et du cor. de la prop. 10 de IV, p. 10.

Supposons que $A$ soit intègre. L’algèbre $K[x]$ est intègre et de degré fini sur $K$, donc c’est un corps (V, p. 10, cor.). L’idéal $(f)$ de $K[x]$ est donc maximal, c’est-à-dire que $f$ est irréductible dans $K[X]$ (IV, p. 13). Enfin, soit $g$ un polynôme unitaire irréductible dans $K[X]$ tel que $g(x) = 0$; d’après a), c’est un multiple de $f$, d’où $g = f$. Ceci prouve c).

Il reste à prouver d). Il existe un polynôme $g \in K[X]$ de degré $n - 1$ et un élément $a$ de $K$ tels que $f(X) = Xg(X) + a$, d’où $f(0) = a$. Si $a = 0$, on a $xg(x) = f(x) = 0$ et $g(x) \neq 0$, donc $x$ n’est pas inversible dans $A$. Si au contraire on a $a \neq 0$, on a $x.[ - a^{-1}g(x)] = 1$, donc $x$ est inversible dans $A$ et $x^{-1} = -a^{-1}g(x)$.

#### Corollaire 1 {#alg-v-s3-thm-1-cor-1 .statement}

Soit $A$ une algèbre sur un corps $K$. Pour qu’un élément $x$ de $A$ soit algébrique sur $K$, il faut et il suffit que la sous-algèbre $K[x]$ de $A$ engendrée par $x$ soit de degré fini sur $K$. En particulier, si $A$ est de degré fini sur $K$, tout élément de $A$ est algébrique sur $K$.

#### Corollaire 2 {#alg-v-s3-thm-1-cor-2 .statement}

Soient $E$ une extension de $K$, $A$ une algèbre sur $E$ et $x$ un élément de $A$ algébrique sur $K$. Alors $x$ est algébrique sur $E$, le polynôme minimal de $x$ sur $E$ divise le polynôme minimal de $x$ sur $K$, et le degré de $x$ sur $E$ est au plus égal au degré de $x$ sur $K$.

En effet, soit $f$ le polynôme minimal de $x$ sur $K$; on a $f(x) = 0$ et $f \in E[X]$, donc $x$ est algébrique sur $E$, et $f$ est un multiple du polynôme minimal de $x$ sur $E$ (th. 1, a)).

#### Remarque {#alg-v-s3-n1-rem-1 .statement}

Soient $E$ une extension d’un corps $K$ et $x$ un élément de $E$ racine d’un polynôme unitaire irréductible $f \in K[X]$. Le th. 1, c) montre que $f$ est le polynôme minimal de $x$ sur $K$.

#### Exemple 1 {#alg-v-s3-n1-exa-1 .statement}

Dans le corps des nombres complexes $\mathbf{C}$, le nombre $i$ est algébrique et de degré 2 sur le corps premier $\mathbf{Q}$; en effet, si $f(X) = X^2 + 1$, on a $f(i) = 0$, et $x^2 + 1 \neq 0$ pour tout $x \in \mathbf{Q}$, donc $i \notin \mathbf{Q}$. Le corps $\mathbf{Q}(i)$ est donc une extension de degré 2 de $\mathbf{Q}$; il est formé des nombres $a + bi$, où $a$ et $b$ sont rationnels. De même, $i$ est algébrique et de degré 2 sur le corps $\mathbf{R}$ des nombres réels et $\mathbf{C}$ est une extension de degré 2 de $\mathbf{R}$. \*

#### Exemple 2 {#alg-v-s3-n1-exa-2 .statement}

Soient K un corps, F le corps K(X) des fractions rationnelles en une indéterminée sur K. Soit E le sous-corps K(X³) de F ; on a F = E(X), et X est algébrique sur E, puisqu’il est racine du polynôme Y³ − X³ de l’anneau E[Y] ; ce polynôme est irréductible dans E[Y], car dans le cas contraire, il aurait au moins un facteur du premier degré, et il existerait donc deux polynômes non nuls u, v de K[X] tels que l’on ait (u(X³))³ = X³(v(X³))³, ceci est absurde, car si m et n sont les degrés de u et de v, cela implique 9m = 9n + 3 ou 3m = 3n + 1. Le corps F est donc de degré 3 sur E, et tout élément de F peut s’écrire d’une seule manière comme combinaison linéaire f(X³) + Xg(X³) + X²h(X³), où f, g, h sont trois fractions rationnelles de K(X).

#### Exemple 3 {#alg-v-s3-n1-exa-3 .statement}

Dans le corps R des nombres réels, on peut montrer¹ que le nombre π est transcendant sur le corps premier Q. \*

### 2. Extensions algébriques

#### Définition 1 {#alg-v-s3-def-1 .statement}

On dit qu’une extension E d’un corps K est algébrique (sur K) si tout élément de E est algébrique sur K. Une extension E de K qui n’est pas algébrique est dite transcendante (sur K).

#### Proposition 1 {#alg-v-s3-prop-1 .statement}

Pour qu’une extension E de K soit algébrique, il faut et il suffit que toute sous-K-algèbre A de E soit un corps.

La condition est nécessaire : si E est algébrique sur K, et x ≠ 0 un élément d’une sous-K-algèbre A de E, on a x⁻¹ ∈ K[x] ⊂ A d’après V, p. 15, théorème 1, c). Par suite, A est un corps.

La condition est suffisante : si elle est remplie, et si x est un élément ≠ 0 dans E, l’anneau K[x] est un corps, donc x⁻¹ ∈ K[x] ; autrement dit, il existe un polynôme g ∈ K[X] tel que x⁻¹ = g(x), ou encore xg(x) − 1 = 0 ; ceci prouve que x est algébrique sur K, donc que E est une extension algébrique de K.

#### Proposition 2 {#alg-v-s3-prop-2 .statement}

Si une extension E d’un corps K est de degré fini n, elle est algébrique, et le degré sur K de tout élément de E divise n.

En effet, pour tout x ∈ E, [K(x) : K] est fini et divise n (V, p. 10, cor. 1) et par suite x est algébrique sur K (V, p. 16, cor. 1).

\* Il existe des extensions algébriques de degré infini. C’est le cas par exemple de la clôture algébrique d’un corps fini (V, p. 23, remarque 4). \*

#### Théorème 2 {#alg-v-s3-thm-2 .statement}

Soit E une extension de type fini de K, engendrée par des éléments a₁, ..., aₘ algébriques sur K ; alors E est une extension de degré fini de K. Si nᵢ est le degré de aᵢ sur K(a₁, a₂, ..., aᵢ₋₁) (pour 1 ≤ i ≤ m), le degré de E sur K est n₁n₂ ... nₘ, et les éléments a₁^{ν₁}a₂^{ν₂} ... aₘ^{νₘ} (0 ≤ νᵢ ≤ nᵢ − 1) forment une base de E sur K.

Les éléments aᵢ^{νᵢ} (0 ≤ νᵢ ≤ nᵢ − 1) forment une base de K(a₁, a₂, ..., aᵢ) sur K(a₁, a₂, ..., aᵢ₋₁) d’après le th. 1, b) de V, p. 16 ; le théorème résulte alors, par récurrence sur m, de la prop. 25 de II, p. 31.

¹ Cf. par exemple D. Hilbert, Gesammelte Abhandlungen, t. I, p. 1 (Berlin (Springer), 1932).

#### Corollaire 1 {#alg-v-s3-thm-2-cor-1 .statement}

Soient E une extension de K et A une partie de E formée d’éléments algébriques sur K. Alors K(A) est algébrique sur K, et l’on a K[A] = K(A).

En effet, tout x ∈ K(A) appartient à un corps K(F), où F est une partie finie de A (V, p. 11, cor.) ; or, K(F) est algébrique sur K et égal à K[F] d’après le th. 2, donc x est algébrique sur K et K(A) = K[A].

#### Corollaire 2 {#alg-v-s3-thm-2-cor-2 .statement}

Soient L une extension de K, E et F deux sous-extensions de L. Si F est algébrique sur K, le sous-anneau K[E, F] de L engendré par E ∪ F est un corps, identique à E(F), et algébrique sur E.

En effet, tout élément de F, étant algébrique sur K, est algébrique sur E (V, p. 16, cor. 2), donc E(F) est une extension algébrique de E, et l’on a E(F) = E[F] d’après le cor. 1.

#### Remarque 1 {#alg-v-s3-n2-rem-1 .statement}

Avec les notations du th. 2, E = K[a_1, a_2, ..., a_m], et par suite E est isomorphe à un quotient K[X_1, X_2, ..., X_m]/α ; comme E est un corps, α est un idéal maximal dans K[X_1, ..., X_m].

#### Remarque 2 {#alg-v-s3-n2-rem-2 .statement}

Soit E une extension algébrique de K, de degré infini. D’après le th. 2, il existe une suite infinie (a_n)_{n \geq 1} d’éléments de E telle que a_n \notin K(a_1, a_2, ..., a_{n-1}) ; le th. 2 montre en outre que le degré de K(a_1, a_2, ..., a_n) sur K prend des valeurs arbitrairement grandes. En d’autres termes, si E est une extension algébrique de K telle que les degrés [F : K] des sous-extensions F de E de degré fini sur K soient bornés, E est une extension de degré fini de K.

### 3. Transitivité des extensions algébriques. Corps algébriquement fermé dans un surcorps

#### Proposition 3 {#alg-v-s3-prop-3 .statement}

Soient E et F deux surcorps d’un corps K tels que K ⊂ E ⊂ F. Pour que F soit algébrique sur K, il faut et il suffit que E soit algébrique sur K et F algébrique sur E.

La condition est nécessaire, d’après V, p. 16, cor. 2. Montrons qu’elle est suffisante ; soit x un élément quelconque de F ; il est algébrique sur E ; soit g ∈ E[X] son polynôme minimal sur E. Si A est l’ensemble (fini) des coefficients de g, on a g ∈ K(A)[X], donc x est algébrique sur K(A) et K(A ∪ {x}) = K(A)(x) est de degré fini sur K(A) ; on a A ⊂ E et E est algébrique sur K, donc K(A) est de degré fini sur K d’après le th. 2. Par suite (V, p. 9, th. 1), K(A ∪ {x}) est de degré fini sur K, ce qui montre que x est algébrique sur K (V, p. 17, prop. 2).

#### Définition 2 {#alg-v-s3-def-2 .statement}

On dit qu’un sous-corps K d’un corps E est algébriquement fermé dans E si tout élément de E, algébrique sur K, appartient à K.

Il revient au même de dire que K est la seule extension algébrique de K contenue dans E. Tout corps K est algébriquement fermé dans lui-même. Nous étudierons au § 4 les corps qui sont algébriquement fermés dans tout surcorps.

#### Proposition 4 {#alg-v-s3-prop-4 .statement}

Soit E une extension d’un corps K ; l’ensemble L des éléments de E qui sont algébriques sur K est une sous-extension de E, algébriquement fermée dans E.

En effet (cor. 1 du th. 2), le corps K(L) est algébrique sur K, donc K(L) ⊂ L ; par suite, on a K(L) = L, et L est un corps. D’autre part, si x ∈ E est algébrique sur L, il l’est aussi sur K (prop. 3), donc appartient à L.

On dit que l’extension L de K formée des éléments de E algébriques sur K est la fermeture algébrique de K dans E ; c’est la plus grande extension algébrique de K contenue dans E.

## EXERCICES {#alg-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
