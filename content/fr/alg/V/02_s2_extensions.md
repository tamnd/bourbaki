---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 2
section_title: EXTENSIONS
lang: fr
source: alg-iv-vii-fr
book_pages: A V.140-A V.141
pdf_pages: 0112-0119, 0244-0245
extraction: ocr
subsections:
    - "no": 1
      title: La structure d’extension
      page: 8
      pdf_page: 112
    - "no": 2
      title: Degré d’une extension
      page: 9
      pdf_page: 113
    - "no": 3
      title: Adjonction
      page: 10
      pdf_page: 114
    - "no": 4
      title: Extensions composées
      page: 11
      pdf_page: 115
statements: 18
exercises: 4
content_sha256: 250c081eb584c11f7eac4d91a8f73c54227e3e2bb0e07fca4af64854d2088e19
---

## § 2. EXTENSIONS

### 1. La structure d’extension

#### Définition 1 {#alg-v-s2-def-1 .statement}

Soit $K$ un corps. On appelle extension de $K$ une $K$-algèbre dont l’anneau sous-jacent est un corps. On appelle sous-extension (ou sous-K-extension) de l’extension $E$ une sous-K-algèbre de $E$ qui est un corps.

Soit E une extension de K. L’application $u : \lambda \mapsto \lambda . 1$ de K dans E est un homomorphisme d’anneaux ; d’après I, p. 110, $u$ induit un isomorphisme de K sur le sous-corps $u(K)$ de E.

Réciproquement, soient K, E des corps et $u$ un homomorphisme de K dans E. La donnée de $u$ définit sur E une structure d’extension de K (III, p. 6). Par abus de langage, on dit parfois que (E, $u$) est une extension de K.

On dit que l’extension est triviale si $u(K) = E$, c’est-à-dire si E est un espace vectoriel de dimension 1 sur K.

Soit L un surcorps de K. Quand nous considérerons L comme extension de K, nous entendrons par là l’extension (L, $j$) de K où $j$ est l’injection canonique de K dans L, ou encore L muni de la structure de K-algèbre correspondante. Les sous-extensions de L sont alors les corps intermédiaires entre K et L, c’est-à-dire les sous-corps de L contenant K. Si L’ est un autre surcorps de K, un K-homomorphisme de L dans L’ est donc un homomorphisme $f$ de L dans L’ tel que $f(x) = x$ pour tout $x \in K$. On notera que si $f$ est un endomorphisme quelconque du corps L, l’ensemble des éléments de L invariants par $f$ est un sous-corps K’ de L, et que $f$ est donc un K’-endomorphisme de L.

En particulier, soit P le sous-corps premier d’un corps L. On peut considérer L comme extension de P, et tout endomorphisme de L est alors un P-endomorphisme.

Soit (E, $u$) une extension de K ; comme $u$ définit un isomorphisme de K sur un sous-corps $K_1$ de E, il n’y a en général aucun inconvénient à identifier K à $K_1$ par $u$. Un cas où il faudrait proscire une telle identification est celui où $K = E$ et où $u$ est donc un endomorphisme de K ; le plus souvent $u$ sera un automorphisme de K, ou bien l’application $x \mapsto x^p$, lorsque le corps K est de caractéristique $p \neq 0$.

Il est clair que toute extension de K est isomorphe à une extension (L, $j$) où L est un surcorps de K et $j$ l’injection canonique de K dans L.

### 2. Degré d’une extension

Soit A une algèbre sur un corps K. C’est en particulier un espace vectoriel sur K ; la dimension de cet espace vectoriel s’appelle le degré de A sur K et se note [A : K] (II, p. 97). Par définition, [A : K] est donc le cardinal de toute base de A sur K. Cette définition s’applique en particulier au cas des extensions de K.

Une extension de degré 1 est triviale. Une extension de degré 2 (resp. 3, etc.) est dite quadratique (resp. cubique, etc.). Une extension de degré fini sera parfois appelée par abus de langage extension finie.

#### Théorème 1 {#alg-v-s2-thm-1 .statement}

Soient E une extension de K et A une algèbre sur E. On a alors [A : K] = [A : E].[E : K]. En particulier, si F est une extension de E, on a

$$
[F : K] = [F : E].[E : K].
$$

Le théorème n’est qu’un cas particulier de II, p. 31, prop. 25 ; de manière plus précise, si $(a_\lambda)_{\lambda \in L}$ est une base de $A$ sur $E$ et $(b_\mu)_{\mu \in M}$ une base de $E$ sur $K$, alors la famille $(a_\lambda b_\mu)_{(\lambda, \mu) \in L \times M}$ est une base de $A$ sur $K$.

#### Corollaire 1 {#alg-v-s2-thm-1-cor-1 .statement}

*Soient $K, E, F$ trois corps tels que $K \subset E \subset F$ et que $[F : K]$ soit fini. Les degrés $[E : K]$ et $[F : E]$ sont des diviseurs de $[F : K]$*.

Si le degré $[F : K]$ est premier, il n’existe donc aucune sous-extension de $F$ autre que $K$ et $F$. Mais on notera que, lorsque $[F : K]$ n’est pas premier, il n’existe pas nécessairement de sous-extension de $F$ autre que $K$ et $F$ (cf. V, p. 140, exerc. 1).

#### Corollaire 2 {#alg-v-s2-thm-1-cor-2 .statement}

*Soient $K, E$ et $F$ trois corps avec $K \subset E \subset F$. On suppose que $[F : K]$ est fini. Alors, la relation $[E : K] = [F : K]$ est équivalente à $E = F$ et la relation $[F : E] = [F : K]$ est équivalente à $E = K$.

En effet, si $L$ est un surcorps de $L'$, la relation $[L : L'] = 1$ équivaut à $L' = L$.

#### Proposition 1 {#alg-v-s2-prop-1 .statement}

*Soit $A$ une algèbre de degré fini sur un corps $K$. Si un élément $a \in A$ n’est pas diviseur de 0 à gauche (resp. à droite) dans $A$, il est inversible dans $A$.

En effet, par hypothèse l’espace vectoriel $A$ sur $K$ est de dimension finie, et l’application linéaire $x \mapsto ax$ (resp. $x \mapsto xa$) de $A$ dans $A$ est injective ; elle est donc bijective (II, p. 101, cor.), et par suite (I, p. 16, remarque) $a$ est inversible dans $A$.

COROLLAIRE — *Soit $A$ une algèbre commutative de degré fini sur un corps $K$. Si l’anneau $A$ est intègre, c’est un corps.*

### 3. Adjonction

Soit $E$ une extension d’un corps $K$. Étant donnée une famille $x = (x_i)_{i \in I}$ d’éléments de $E$, on désigne par $K(x_i)_{i \in I}$ (ou $K(x)$, ou encore $K(x_1, \ldots, x_n)$ lorsque $I$ est l’intervalle $[1, n]$ de $\mathbf{N}$) la plus petite sous-extension de $E$ contenant les éléments de la famille $(x_i)$; nous dirons que $K(x_i)_{i \in I}$ est obtenue par *adjonction* à $K$ des éléments de la famille $(x_i)_{i \in I}$, et que la famille $(x_i)_{i \in I}$ (ou l’ensemble de ses éléments) est une *famille génératrice de $K(x_i)_{i \in I}$ par rapport à $K$* (ou *sur $K$*). Le corps $K(x_i)_{i \in I}$ ne dépend que de l’ensemble $A$ des éléments de la famille $(x_i)_{i \in I}$; on le désigne encore par $K(A)$. On a en particulier $K(E) = E$ et $K(\emptyset) = K.1$. Tout ce qui précède s’applique en particulier lorsque $E$ est un surcorps de $K$.

On prendra garde que $A$ n’est pas un ensemble générateur de l’*algèbre* $K(A)$, autrement dit que l’on a $K(A) \neq K[A]$, en général. *Toutefois on verra que $K(A) = K[A]$ si $K(A)$ est une extension algébrique de $K$ (V, p. 18, cor. 1).*

#### Proposition 2 {#alg-v-s2-prop-2 .statement}

*Si $M$ et $N$ sont deux parties quelconques d’une extension d’un corps $K$, on a $K(M \cup N) = K(M)(N) = K(N)(M)$.

En effet, $K(M \cup N)$ contient $K(M)$ et $N$, donc $K(M)(N)$; comme $K(M)(N)$ est un corps contenant $K \cup M \cup N$, il contient $K(M \cup N)$, d’où la proposition.

On écrit parfois $K(M, N)$ au lieu de $K(M \cup N)$.

#### Remarque {#alg-v-s2-n3-rem-1 .statement}

Soit P le sous-corps premier d’un corps E (V, p. 2) ; pour toute partie A de E, P(A) est le plus petit sous-corps de E contenant A. En particulier, si K est un sous-corps de E, on a P(K ∪ A) = K(A). Si K et K’ sont deux sous-corps de E, on a donc P(K ∪ K’) = K(K’) = K’(K) ; ce corps est le plus petit sous-corps de E contenant K et K’, ou encore la borne supérieure de K et K’ dans l’ensemble des sous-corps de E, ordonné par inclusion ; on dit parfois que ce corps est le corps engendré par K et K’ dans E.

#### Proposition 3 {#alg-v-s2-prop-3 .statement}

Soit $\mathcal{F}$ un ensemble de sous-corps d’un corps E, filtrant pour la relation $\subset$. La réunion L des corps de $\mathcal{F}$ est un corps.

En effet, si x et y sont deux éléments de L, il existe deux corps R, S de $\mathcal{F}$ tels que $x \in R, y \in S$; soit T un corps de $\mathcal{F}$ contenant R et S ; alors $x \in T, y \in T$, donc $x + y, xy$ et $x^{-1}$ (si $x \neq 0$) appartiennent à T, donc à L.

#### Corollaire {#alg-v-s2-n3-cor-1 .statement}

Soient E une extension d’un corps K, et A $\subset$ E. Le corps K(A) est la réunion des corps K(F), où F parcourt l’ensemble des parties finies de A.

En effet, l’ensemble des corps K(F) est filtrant pour la relation $\subset$, car F $\subset$ F’ entraîne K(F) $\subset$ K(F’). La réunion L de ces corps est donc un corps contenant K $\cup$ A et contenu dans K(A), et par suite identique à K(A).

#### Définition 2 {#alg-v-s2-def-2 .statement}

On dit qu’une extension E d’un corps K est de type fini si elle possède une famille génératrice finie. Elle est dite monogène s’il existe x dans E tel que $E = K(x)$.

Le cor. de la prop. 3 montre que toute extension E d’un corps K est réunion filtrante des extensions de type fini contenues dans E. Il est clair que toute extension E de K de degré fini est aussi de type fini, puisqu’une base de E (considéré comme espace vectoriel sur K) est aussi une famille génératrice de E sur K ; nous verrons plus loin que la réciproque est inexacte.

### 4. Extensions composées

Soient E et F deux extensions d’un corps K. On appelle extension composée de E et F tout triplet (L, u, v) où L est une extension de K, où u est un K-homomorphisme de E dans L et v un K-homomorphisme de F dans L, et où le corps L est engendré par $u(E) \cup v(F)$ (cf. fig. 1).

$$
\begin{array}{ccc}
& & L \\
& u & \\
E & & F \\
& v & \\
& & K
\end{array}
$$

Fig. 1.

Conformément aux définitions générales (E, IV, p. 6), un isomorphisme d’une extension composée (L, u, v) de E et F sur une extension composée (L’, u’, v’) de E et F est un K-isomorphisme $\varphi$ de L sur L’ tel que $u' = \varphi \circ u$ et $v' = \varphi \circ v$.

Soit $(L, u, v)$ une extension composée de $E$ et $F$. L’application $K$-linéaire $w$ de $E \otimes_K F$ dans $L$ qui transforme $x \otimes y$ en $u(x)\ v(y)$ est un homomorphisme de $K$-algèbres ; dans ce numéro, nous la désignerons par $u * v$. Son image est le sous-anneau de $L$ engendré par $u(E) \cup v(F)$.

#### Proposition 4 {#alg-v-s2-prop-4 .statement}

*Soient $E, F$ deux extensions de $K$.*

*a) Soit $(L, u, v)$ une extension composée de $E$ et $F$. Alors le noyau $p$ de l’homomorphisme $u * v$ de $E \otimes_K F$ dans $L$ est un idéal premier.*

*b) Soit $p$ un idéal premier de $E \otimes_K F$. Il existe une extension composée $(L, u, v)$ de $E$ et $F$ telle que $p$ soit le noyau de $u * v$, et deux telles extensions composées sont isomorphes.*

L’assertion *a)* résulte du fait que le noyau d’un homomorphisme d’un anneau dans un corps est un idéal premier (I, p. 111).

Soient $p$ un idéal premier de $E \otimes_K F$, A l’anneau quotient $(E \otimes_K F)/p$ et $L$ le corps des fractions de $A$. Pour $x \in E$ (resp. $y \in F$), on note $u(x)$ (resp. $v(y)$) la classe modulo $p$ de $x \otimes 1$ (resp. $1 \otimes y$). Alors $u$ (resp. $v$) est un $K$-homomorphisme de $E$ (resp. $F$) dans $L$, et $u(E) \cup v(F)$ engendre $A$ comme anneau, donc $L$ comme corps. Par suite $(L, u, v)$ est une extension composée de $E$ et $F$ ; on voit immédiatement que $u * v$ est l’homomorphisme canonique de $E \otimes_K F$ dans $L$, et son noyau est donc égal à $p$.

Soit $(L', u', v')$ une extension composée de $E$ et $F$ telle que le noyau de $u' * v'$ soit égal à $p$. Comme $u * v$ et $u' * v'$ ont même noyau, il existe un isomorphisme $\psi$ de $A$ sur l’image $A'$ de $u' * v'$ caractérisé par $u' * v' = \psi \circ (u * v)$. Mais $A'$ est le sous-anneau de $L'$ engendré par $u'(E) \cup v'(F)$, donc $L'$ est le corps des fractions de $A'$. Par suite, $\psi$ se prolonge en un isomorphisme $\varphi$ de $L$ sur $L'$, et il est immédiat que $\varphi$ est un isomorphisme de $(L, u, v)$ sur $(L', u', v')$.

#### Remarque {#alg-v-s2-n4-rem-1 .statement}

Si $p$ et $p'$ sont deux idéaux premiers distincts de $E \otimes_K F$, les *extensions composées* de $E$ et $F$ correspondantes (construites par le procédé de la démonstration précédente) ne sont pas isomorphes. Elles peuvent cependant être isomorphes en tant qu’*extensions* de $K$ (V, p. 140, exerc. 2).

#### Corollaire {#alg-v-s2-n4-cor-1 .statement}

*Il existe des extensions composées de $E$ et $F$.*

En effet, comme l’anneau commutatif $E \otimes_K F$ n’est pas réduit à 0, il possède des idéaux premiers : le théorème de Krull (I, p. 99) prouve l’existence d’idéaux maximaux, et tout idéal maximal est premier.

On peut préciser ce corollaire comme suit. Soient $(E, u)$ et $(F, v)$ deux extensions de $K$. Choisissons un idéal maximal $m$ de l’anneau commutatif $E \otimes_K F$ et posons $L = (E \otimes_K F)/m$ ; alors $L$ est une extension de $K$. Pour $x \in E$, notons $u'(x)$ la classe de $x \otimes 1$ modulo $m$, et de même notons $v'(y)$ la classe de $1 \otimes y$ modulo $m$ pour tout $y \in F$. On a alors un diagramme commutatif d’homomorphismes de corps

Quitte à remplacer $(L, u')$ par une extension isomorphe de $E$, on peut supposer que $L$ est un surcorps de $E$ et $u'$ l’injection canonique de $E$ dans $L$. Changeant de notations, on obtient ainsi le scholie suivant :

#### Scholie {#alg-v-s2-n4-sch-1 .statement}

*Soient $K$ et $E$ deux corps et $u$ un homomorphisme de $K$ dans $E$. Si $K'$ est un surcorps de $K$, il existe un surcorps $E'$ de $E$ et un homomorphisme $u'$ de $K'$ dans $E'$ qui prolonge $u$*.

5. **Extensions linéairement disjointes**

*Dans ce numéro, on note $\Omega$ une extension d’un corps $K$*.

Soient $A$ et $B$ deux sous-$K$-algèbres de $\Omega$. Il existe un homomorphisme d’algèbres $\varphi : A \otimes_K B \to \Omega$ qui applique $x \otimes y$ sur $xy$. L’image de $\varphi$ est le sous-anneau $C$ de $\Omega$ engendré par $A \cup B$. En outre, d’après II, p. 62, si $(b_\mu)$ est une base de $B$ sur $K$ et $(a_\lambda)$ une base de $A$ sur $K$, $C$ est identique à l’ensemble des combinaisons linéaires $\sum_{\mu} \alpha_\mu b_\mu$, où $\alpha_\mu \in A$, à l’ensemble des $\sum_{\lambda} \beta_\lambda a_\lambda$, où $\beta_\lambda \in B$, et à l’ensemble des $\sum_{\lambda,\mu} \gamma_{\lambda\mu} a_\lambda b_\mu$, où $\gamma_{\lambda\mu} \in K$.

On dit que $A$ et $B$ sont *linéairement disjointes sur $K$* si $\varphi$ est un *isomorphisme* de $A \otimes_K B$ sur $C$. On a alors $A \cap B = K$; toute partie libre de $B$ (resp. $A$) par rapport à $K$ est alors libre par rapport à $A$ (resp. $B$); inversement, pour que $A$ et $B$ soient linéairement disjointes sur $K$, il suffit qu’il existe *une* base de $B$ sur $K$ (par exemple), qui soit libre par rapport à $A$ (II, p. 62 et III, p. 41).

Considérons plus particulièrement le cas où $A$ et $B$ sont des *sous-extensions* de $\Omega$.

#### Proposition 5 {#alg-v-s2-prop-5 .statement}

*Soient $E$ et $F$ deux extensions de $K$ contenues dans $\Omega$.

a) *Si $F$ est de degré fini sur $K$, le sous-anneau de $\Omega$ engendré par $E \cup F$ est un corps, identique à $E(F)$, et le degré de $E(F)$ sur $E$ est fini; on a $[E(F):E] \leq [F:K]$, avec égalité si et seulement si $E$ et $F$ sont linéairement disjointes sur $K$. Dans ce cas $E(F)$ est $E$-isomorphe à $E \otimes_K F$.

b) *Si en outre $E$ est de degré fini sur $K$, alors $E(F) = K(E \cup F)$ est de degré fini sur $K$. On a $[K(E \cup F):K] \leq [E:K][F:K]$, avec égalité si et seulement si $E$ et $F$ sont linéairement disjointes sur $K$*.

En effet, soit $C$ le sous-anneau de $\Omega$ engendré par $E \cup F$; si $(b_j)_{1 \leq j \leq n}$ est une base de $F$ sur $K$, $C$ est le sous-$E$-espace vectoriel de $\Omega$ engendré par les $b_j$, donc $C$ est une algèbre de rang *fini* $\leq n$ sur $E$; comme l’anneau $C$ est contenu dans un corps, il est intègre et par suite est un *corps* d’après le cor. de la prop. 1 (V, p. 10), d’où $C = E(F)$ et $[E(F):E] \leq [F:K]$. La relation $[E(F):E] = [F:K]$ signifie que les $b_j$ sont linéairement indépendants sur $E$, donc que $E$ et $F$ sont linéairement disjoints sur $K$; ceci démontre la partie a) de la proposition. La partie b) s’en déduit aussitôt, puisque $[E(F):K] = [E(F):E][E:K]$.

Soient $E$ et $F$ des extensions de $K$ contenues dans $\Omega$; si $E$ et $F$ sont de degré infini sur $K$, le sous-anneau $C = K[E \cup F]$ n’est pas nécessairement un corps $^1$; toutefois, le *corps des fractions* de $C$ est alors identique à $K(E \cup F)$. Plus généralement, soient $A$ un sous-anneau de $E$ tel que $E$ soit le corps des fractions de $A$, et $B$ un sous-anneau de $F$ tel que $F$ soit le corps des fractions de $B$; alors, si $C$ est le sous-anneau de $\Omega$ engendré par $A \cup B$, $K(E \cup F)$ est identique au *corps des fractions* de $C$, puisque ce dernier corps est le plus petit sous-corps de $\Omega$ contenant $C$, et qu’il contient $E$ et $F$. En outre :

#### Proposition 6 {#alg-v-s2-prop-6 .statement}

*Soient $E$ et $F$ deux extensions de $K$ contenues dans $\Omega$, $A$ et $B$ deux sous-algèbres de $\Omega$ sur $K$, telles que $E$ soit le corps des fractions de $A$ et $F$ le corps des fractions de $B$. Pour que $E$ et $F$ soient linéairement disjointes sur $K$, il faut et il suffit que $A$ et $B$ soient linéairement disjointes sur $K$.*

La condition est évidemment nécessaire. Réciproquement, si $A$ et $B$ sont linéairement disjointes sur $K$, $A$ et $F$ le sont aussi, car si une famille d’éléments de $\Omega$ est libre par rapport à $B$, elle est libre par rapport au corps des fractions $F$ de $B$ (II, p. 117, cor. 1 et p. 118, cor. 3); le même raisonnement prouve ensuite que $E$ et $F$ sont linéairement disjointes sur $K$.

#### Proposition 7 {#alg-v-s2-prop-7 .statement}

*Soient $E$ et $F$ deux extensions de $K$, contenues dans $\Omega$. Si $E$ et $F$ sont linéairement disjointes sur $K$, toute sous-extension de $E$ et toute sous-extension de $F$ sont linéairement disjointes sur $K$. Inversement, si, pour tout couple de sous-extensions de type fini $E', F'$ de $E$ et $F$ respectivement, $E'$ et $F'$ sont linéairement disjointes sur $K$, alors $E$ et $F$ sont linéairement disjointes sur $K$.*

En effet, la condition pour que $E$ et $F$ soient linéairement disjointes sur $K$ s’exprime de la façon suivante : si $(a_\alpha)$ est une famille libre de $E$ et $(b_\beta)$ une famille libre de $F$, la relation $\sum_{\alpha, \beta} \lambda_{\alpha \beta} a_\alpha b_\beta = 0$, où $\lambda_{\alpha \beta} \in K$, doit entraîner $\lambda_{\alpha \beta} = 0$ pour tout couple d’indices. Or, cette condition est vérifiée pour tout couple de familles libres si elle l’est pour tout couple de familles libres *finies*.

On peut donc dire, d’une façon imagée, que la disjonction linéaire est une propriété « de caractère fini ».

#### Proposition 8 {#alg-v-s2-prop-8 .statement}

*Soient $E, F, G$ trois extensions d’un corps $K$, contenues dans $\Omega$, et telles que $F \subset G$. Pour que $E$ et $G$ soient linéairement disjointes sur $K$, il faut et il suffit que $E$ et $F$ soient linéairement disjointes sur $K$, et que $E(F)$ et $G$ soient linéairement disjointes sur $F$.*

$^1$ Il suffit de considérer par exemple le cas où $\Omega$ est le corps $K(X, Y)$ des fractions rationnelles en deux indéterminées $X$ et $Y$, et où l’on a $E = K(X), F = K(Y)$.

$$
\begin{array}{ccc}
E & \longrightarrow & E(F) \\
\uparrow & & \uparrow \\
K & \longrightarrow & F \longrightarrow G.
\end{array}
$$

Fig. 2.

La condition est nécessaire : supposons que E et G soient linéairement disjointes sur K. Il en est alors de même de E et F (prop. 7); d’autre part, si B est une base de E sur K, c’est aussi une base de l’algèbre F[E] sur F; comme par hypothèse B est libre par rapport à G, F[E] et G sont linéairement disjointes sur F, et il en est donc de même de E(F) = F(E) et G d’après la prop. 6.

La condition est suffisante : avec les mêmes notations, elle entraîne que B est libre sur F, donc est une base de F[E] sur F; comme F[E] et G sont par hypothèse linéairement disjointes sur F, B est libre sur G, ce qui montre que E et G sont linéairement disjointes sur K.

## EXERCICES {#alg-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
