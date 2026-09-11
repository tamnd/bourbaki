---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 10
section_title: EXTENSIONS GALOISIENNES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.147-A V.152
pdf_pages: 0158-0177, 0251-0256
extraction: ocr
subsections:
    - "no": 1
      title: Définition des extensions galoisiennes
      page: 54
      pdf_page: 158
    - "no": 2
      title: Groupe de Galois
      page: 56
      pdf_page: 160
    - "no": 3
      title: Topologie du groupe de Galois
      page: 58
      pdf_page: 162
    - "no": 4
      title: Descente galoisienne
      page: 60
      pdf_page: 164
    - "no": 5
      title: Cohomologie galoisienne
      page: 62
      pdf_page: 166
    - "no": 6
      title: Le théorème d’Artin
      page: 63
      pdf_page: 167
statements: 51
exercises: 23
content_sha256: d5887dc184e32c14705ba2fd592afc40349b31482eec49a947ee4ea3c59c8fef
---

## § 10. EXTENSIONS GALOISIENNES

Dans tout ce paragraphe, on note K un corps.

### 1. Définition des extensions galoisiennes

#### Théorème 1 {#alg-v-s10-thm-1 .statement}

*Soient N une extension algébrique de K et Γ le groupe des K-auto-morphismes de N. Les assertions suivantes sont équivalentes :
a) Tout élément de N invariant par Γ appartient à l’image de K dans N.
b) N est une extension quasi-galoisienne et séparable de K.
c) Pour tout $x \in N$, le polynôme minimal de x sur K se décompose dans N[X] en produit de polynômes distincts de degré 1.*
L’équivalence de b) et c) résulte du cor. de la prop. 6 (V, p. 39) et de la définition des extensions quasi-galoisiennes (V, p. 52, déf. 2). Identifions K à son image canonique dans N.
$a) \Rightarrow c)$ : supposons que K soit le corps des invariants de Γ. Soit $x \in N$, de polynôme minimal f sur K et soit A l’ensemble des racines de f dans N. Posons
$$
g(X) = \prod_{y \in A} (X - y).
$$
Tout automorphisme $\sigma \in \Gamma$ induit une permutation de A, donc laisse invariants les coefficients du polynôme $g \in N[X]$. On a donc $g \in K[X]$ et comme $g(x) = 0$, le polynôme $g$ est multiple de $f$ dans $K[X]$ (V, p. 15, th. 1). Par ailleurs, $f$ et $g$ sont unitaires et $g$ divise $f$ (IV, p. 15, prop. 5); on a donc $f = g$, c'est-à-dire que le polynôme minimal $f$ de $x$ sur $K$ est produit dans $N[X]$ de polynômes distincts de degré 1.

$c) \Rightarrow a)$: soit $x$ un élément de $N$ n’appartenant pas à $K$. Notons $\Omega$ une clôture algébrique de $K$ contenant $N$ comme sous-extension (V, p. 22, th. 2). Soit $f$ le polynôme minimal de $x$ sur $K$, qui est de degré $\geq 2$ par hypothèse et soit $A$ l’ensemble des racines de $f(X)$ dans $N$. Si la condition c) est satisfaite, on a $f(X) = \prod_{y \in A} (X - y)$ et par suite (V, p. 51, cor. 1), $A$ est l’ensemble des conjugués de $x$ dans $\Omega$. Comme $f$ est de degré $\geq 2$, il existe dans $A$ un élément $y \neq x$, donc un $K$-automorphisme $u$ de $\Omega$ tel que $u(x) = y$. Or, sous les hypothèses de c), l’extension $N$ de $K$ est quasi-galoisienne, d’où $u(N) = N$ (V, p. 52, cor. 1); par suite, $u$ induit un $K$-automorphisme $\sigma$ de $N$ tel que $\sigma(x) = y \neq x$, et $K$ est le corps des invariants de $\Gamma$.

#### Définition 1 {#alg-v-s10-def-1 .statement}

*On dit qu’une extension $N$ du corps $K$ est galoisienne si elle est algébrique et si elle satisfait aux conditions équivalentes a), b) et c) du théorème 1.*

Soient $N$ un corps, $\Gamma$ un groupe d’automorphismes de $N$ et $N_0$ le corps des invariants de $\Gamma$. Lorsque $N$ est *algébrique* sur $N_0$, c’est une extension galoisienne de $N_0$. Il n’en est pas toujours ainsi : par exemple, supposons $K$ infini et prenons pour $N$ le corps des fractions rationnelles $K(X)$; pour tout $a \in K$, soit $\sigma_a$ l’automorphisme de $K(X)$ qui transforme $f(X)$ en $f(X + a)$. L’ensemble des $\sigma_a$ est un groupe d’automorphismes de $K(X)$ dont on montre facilement que $K$ est le corps des invariants ; pourtant, $K(X)$ n’est pas algébrique sur $K$.

Soit $\Omega$ une clôture algébrique de $K$. Notons $A$ un ensemble d’éléments de $\Omega$ séparables sur $K$ et $B$ l’ensemble des conjugués sur $K$ des éléments de $A$. Alors, $B$ se compose d’éléments algébriques et séparables sur $K$. Par suite (V, p. 38, prop. 6, et p. 54, prop. 5), le corps $K(B)$ est une extension séparable et quasi-galoisienne de $K$; autrement dit, l’extension quasi-galoisienne engendrée par $A$ (V, p. 54) est une extension galoisienne de $K$; on dit aussi que c’est *l’extension galoisienne de $K$ engendrée par la partie $A$ de $\Omega$*.

En particulier, le corps de décomposition dans $\Omega$ d’une famille de polynômes séparables sur $K$, une clôture séparable de $K$, sont des extensions galoisiennes de $K$.

#### Proposition 1 {#alg-v-s10-prop-1 .statement}

*Soient $N$ une extension de $K$, et $(N_i)_{i \in I}$ une famille non vide de sous-extensions de $N$. On pose $E = \bigcap_{i \in I} N_i$ et $F = K(\bigcup_{i \in I} N_i)$. Si les extensions $N_i$ sont galoisiennes sur $K$ il en est de même de $E$ et $F$.*

Tout d’abord $E$ est algébrique et séparable sur $K$ (V, p. 35, prop. 1) et il en est de même de $F$ (V, p. 40, prop. 8). De plus, $E$ et $F$ sont quasi-galoisiennes sur $K$ d’après la prop. 4 (V, p. 53).

#### Proposition 2 {#alg-v-s10-prop-2 .statement}

*Soient $N$ une extension galoisienne de $K$ et $E$ une sous-extension de $N$, de degré fini sur $K$. Il existe une sous-extension $F$ de $N$, contenant $E$, galoisienne et de degré fini sur $K$.*

Comme N est quasi-galoisienne sur K, le cor. 1 de V, p. 54, prouve l’existence d’une sous-extension quasi-galoisienne F de N contenant E et de degré fini sur K. Comme N est séparable sur K, il en est de même de F (V, p. 35, prop. 1), donc F est galoisienne sur K.

La prop. 2 entraîne le résultat suivant : soient Ω une clôture algébrique de K, et E₁, ..., Eₙ des extensions algébriques séparables de degré fini sur K, contenues dans Ω. Il existe une extension galoisienne N de K, de degré fini, contenue dans Ω et contenant E₁, ..., Eₙ.

### 2. Groupe de Galois

#### Définition 2 {#alg-v-s10-def-2 .statement}

Soit N une extension galoisienne du corps K. On appelle groupe de Galois de N sur K, et l’on note Gal(N/K), le groupe des K-automorphismes de N.

Soit N une extension finie et galoisienne de K. Alors N est une extension finie séparable et quasi-galoisienne de K. Par suite (V, p. 31, prop. 4, et V, p. 52, prop. 3), l’ordre de Gal(N/K) est égal à [N : K]. On démontrera plus loin que si N est une extension galoisienne de K telle que Gal(N/K) soit fini, alors N est de degré fini sur K (V, p. 64, th. 3).

Soient Ω une extension algébriquement close de K, et A l’ensemble des racines dans Ω d’un polynôme séparable f ∈ K[X]. Le corps N = K(A) est une extension galoisienne de K. Il est clair que tout K-automorphisme de N laisse stable A, et comme A engendre N sur K, l’application σ ↦ σ|A est un isomorphisme de Gal(N/K) sur un sous-groupe Γ du groupe symétrique S_A de l’ensemble A qu’on appelle groupe de Galois du polynôme f. Il résulte de la remarque 3 (V, p. 53) que si x et y appartiennent à A, les propriétés suivantes sont équivalentes :

a) x et y sont conjugués sur K,
b) x et y appartiennent à la même orbite de Γ,
c) x et y sont racines du même facteur irréductible de f.
En particulier f est irréductible si et seulement si A est non vide et Γ opère transitivement sur A.

#### Exemple 1 {#alg-v-s10-n2-exa-1 .statement}

Supposons la caractéristique de K différente de 2, et soit N une extension quadratique de K. Si x ∈ N − K, on a N = K(x), et le polynôme minimal de x sur K est de la forme f(X) = X² − aX + b, avec a, b ∈ K. On a alors f(X) = (X − x)(X − y) où y = a − x ; donc y est conjugué de x ; comme f(X) est séparable, l’extension N est galoisienne. Le groupe Gal(N/K) possède deux éléments qui induisent les deux permutations de l’ensemble {x, y}.

#### Exemple 2 {#alg-v-s10-n2-exa-2 .statement}

\* Soit f = X³ + X² − 2X − 1 ∈ Q[X]. Le polynôme f est irréductible, car sinon il posséderait une racine x ∈ Q ; écrivant x = a/b, avec a, b ∈ Z, a et b étrangers, on aurait a(a² + ab − 2b²) = b³ et a³ = b(b² + 2ab − a²) ; mais cela implique que a divise b et b divise a, donc x = ± 1, ce qui est impossible. Soit ξ ≡ e^{2πi/7} ∈ C. Le polynôme f admet les racines α = ξ + ξ⁻¹, β = ξ² + ξ⁻², γ = ξ³ + ξ⁻³. On a β = α² − 2 et γ = α³ − 3α, donc l’extension Q(α) est galoisienne sur Q. Le groupe de Galois de Q(α) sur Q est cyclique d’ordre 3 et il est engendré par un élément σ tel que σ(α) = β, σ(β) = γ, σ(γ) = α. \*

#### Exemple 3 {#alg-v-s10-n2-exa-3 .statement}

Supposons que $K = \mathbf{Q}$ et prenons $f = X^3 - 2$. Utilisant la décomposition des entiers en produit de facteurs premiers (I, p. 49), on voit facilement que 2 n’est pas le cube d’un élément de $\mathbf{Q}$. Le polynôme $f$ est donc irréductible car sinon il possèderait une racine dans $\mathbf{Q}$. Soient $A = \{ x_1, x_2, x_3 \}$ l’ensemble des racines de $f$ dans $\Omega$ et $\Gamma$ le groupe de Galois de $f$. Il opère transitivement sur $A$. Son ordre est donc divisible par trois. D’autre part le quotient $j = \frac{x_2}{x_1}$ est différent de 1 et l’on a $j^3 = 1$. Donc $j$ vérifie la relation $j^2 + j + 1 = 0$; or le polynôme $T^2 + T + 1 = (T + \frac{1}{2})^2 + \frac{3}{4}$ n’a pas de racines dans $\mathbf{Q}$, ce qui montre (cf. exemple 1) que $[\mathbf{Q}(j) : \mathbf{Q}] = 2$. Donc $[\mathbf{N} : \mathbf{Q}]$ est divisible par 2 et par suite l’ordre de $\Gamma$ est divisible par 6. Comme $\Gamma$ est contenu dans le groupe $\mathfrak{S}_A$ d’ordre 6, on a $\Gamma = \mathfrak{S}_A$.

#### Exemple 4 {#alg-v-s10-n2-exa-4 .statement}

Supposons $K$ de caractéristique $p \neq 0$ et soient $K(T)$ le corps des fractions rationnelles et $U = T^p - T$. On pose $E = K(U)$ et $F = K(T)$. Le polynôme $f(X) = X^p - X - U$ de $E[X]$ a les racines $T, T + 1, ..., T + p - 1$ dans $F$. Soit $\sigma$ le $K$-automorphisme de $F$ tel que $\sigma(T) = T + 1$. On a $\sigma^i(T) = T + i$ et $\sigma(U) = U$. Le groupe $G = \{ 1, \sigma, ..., \sigma^{p-1} \}$ est cyclique d’ordre $p$, et son corps des invariants contient $E$; comme $[F : E] \leq p$, le théorème de Dedekind (V, p. 27, cor. 2) implique que $E$ est le corps des invariants de $G$ et que $[F : E] = p$. Le polynôme $f$ est donc irréductible dans $E[X]$; l’extension $F$ de $E$ est galoisienne, son groupe de Galois $G$ est cyclique d’ordre $p$, et le groupe $\Gamma$ est le groupe des permutations circulaires de $T, T + 1, ..., T + p - 1$.

Pour une généralisation de cet exemple, voir V, p. 89, Exemple 2.

#### Exemple 5 {#alg-v-s10-n2-exa-5 .statement}

Soit $F = K(X_1, ..., X_n)$ le corps des fractions rationnelles en $n$ indéterminées $X_1, ..., X_n$ à coefficients dans $K$. Posons
$$
s_k = \sum_{1 \leq i_1 < ... < i_k \leq n} X_{i_1} ... X_{i_k}
$$
pour $1 \leq k \leq n$ et $E = K(s_1, ..., s_n)$; on note $f(T)$ le polynôme
$$
T^n - s_1 T^{n-1} + \cdots + (-1)^n s_n .
$$
On a $f(T) = \prod_{i=1}^n (T - X_i)$ de sorte que $F$ est un corps de décomposition du polynôme séparable $f(T) \in E[T]$. De plus, pour toute permutation $\sigma \in \mathfrak{S}_n$, il existe un $K$-automorphisme $h_\sigma$ de $F$ et un seul tel que $h_\sigma(X_i) = X_{\sigma(i)}$ pour $1 \leq i \leq n$; on a $h_\sigma(s_k) = s_k$ pour $1 \leq k \leq n$, donc $h_\sigma$ est un $E$-automorphisme de $F$. Autrement dit, $F$ est une extension galoisienne de $E$, et par restriction à l’ensemble $\{ X_1, ..., X_n \}$ des racines de $f(T)$, on définit un isomorphisme de $\mathrm{Gal}(F/E)$ sur le groupe $\mathfrak{S}_n$. En particulier, $E$ se compose des fractions rationnelles $f$ telles que
$$
f(X_{\sigma(1)}, ..., X_{\sigma(n)}) = f(X_1, ..., X_n)
$$
pour tout $\sigma \in \mathfrak{S}_n$ (cf. IV, p. 63, cor.).

#### Exemple 6 {#alg-v-s10-n2-exa-6 .statement}

Supposons $f$ unitaire de degré $> 0$ et $K$ de caractéristique $\neq 2$. Munissons $A$ d’un ordre total noté $\leq$. Posons $\delta(f) = \prod_{\alpha < \beta} (\beta - \alpha), (\alpha, \beta) \in A \times A$, et pour tout σ ∈ S_A posons δ_σ(f) = $\prod_{\alpha < \beta} (\sigma(\beta) - \sigma(\alpha))$. On a $\delta_\sigma(f) = \varepsilon(\sigma) \delta(f)$ où $\varepsilon(\sigma)$ est la signature de $\sigma$ (I, p. 61), et $\delta(f) \neq 0$. Pour tout $\tau \in \mathrm{Gal}(N/K)$, on a $\tau(\delta(f)) = \delta_{\tau|A}(f)$. Donc $\Gamma$ est contenu dans le groupe alterné $\mathfrak{A}_A$ si et seulement si $\delta(f) \in K$. Par ailleurs $\delta(f)^2 = \prod_{\alpha < \beta} (\beta - \alpha)^2 = d(f)$ est le discriminant du polynôme $f$ (IV, p. 76). Donc $\Gamma \subset \mathfrak{A}_A$ si et seulement si $d(f)$ est le carré d’un élément de $K$. Ainsi dans l’exemple 2, on a $d(f) = 49 = 7^2$ et dans l’exemple 3, $d(f) = -108$ (IV, p. 81).

Soit $N$ une extension galoisienne de $K$, et soit $L$ une sous-extension de $N$ galoisienne sur $K$. Tout $K$-automorphisme $\sigma$ de $N$ induit un $K$-automorphisme $\sigma_L$ de $L$ (V, p. 53, remarque 1). Par suite, l’application $\sigma \mapsto \sigma_L$ est un homomorphisme de $\mathrm{Gal}(N/K)$ dans $\mathrm{Gal}(L/K)$, appelé *homomorphisme de restriction*.

#### Proposition 3 {#alg-v-s10-prop-3 .statement}

*L’homomorphisme de restriction de Gal(N/K) dans Gal(L/K) est surjectif.*

Plus généralement, considérons deux sous-extensions $L$ et $L'$ de $N$, et un $K$-isomorphisme $u$ de $L$ sur $L'$. Choisissons une clôture algébrique $\Omega$ de $K$, contenant $N$ comme sous-extension (V, p. 22, th. 2). Il existe un $K$-automorphisme $v$ de $\Omega$ qui coïncide avec $u$ sur $L$ (V, p. 50, prop. 1), et comme $N$ est une extension quasi-galoisienne de $K$, $v$ induit un $K$-automorphisme $\sigma$ de $N$ (V, p. 53, remarque 1). Autrement dit, l’élément $\sigma$ de $\mathrm{Gal}(N/K)$ coïncide avec $u$ sur $L$.

### 3. Topologie du groupe de Galois

Soient $N$ une extension galoisienne de $K$ et $\Gamma$ le groupe de Galois de $N$ sur $K$. On munit $N$ de la topologie discrète, l’ensemble $N^N$ des applications de $N$ dans $N$ de la topologie produit des topologies discrètes des facteurs (« topologie de la convergence simple dans $N$ ») et le groupe $\Gamma$ de la topologie induite par celle de $N^N$.

Soit $\Lambda$ l’ensemble des sous-extensions de $N$ de degré fini sur $K$. Pour $\sigma \in \Gamma$ et $E \in \Lambda$, notons $U_E(\sigma)$ l’ensemble des éléments $\tau$ de $\Gamma$ qui ont même restriction que $\sigma$ à $E$. Si $E = K(x_1, ..., x_n)$, l’ensemble $U_E(\sigma)$ se compose des éléments $\tau$ de $\Gamma$ tels que $\tau(x_1) = \sigma(x_1), ..., \tau(x_n) = \sigma(x_n)$. Il en résulte que la famille $(U_E(\sigma))_{E \in \Lambda}$ est une base du filtre des voisinages de $\sigma$ dans $\Gamma$.

Lorsque $N$ est de degré fini sur $K$, on a $N \in \Lambda$ et $U_N(\sigma) = \{ \sigma \}$, donc la topologie de $\mathrm{Gal}(N/K)$ est discrète ; rappelons (V, p. 53, remarque) que le groupe $\mathrm{Gal}(N/K)$ est fini dans ce cas.

Cette description de la topologie de $\mathrm{Gal}(N/K)$ montre que l’*homomorphisme de restriction de Gal(N/K) sur Gal(L/K)* est *continu* pour toute sous-extension $L$ de $N$, galoisienne sur $K$.

Soit $A$ une partie de $\Gamma$. Dire que $A$ est *ouverte* signifie que, pour tout $\sigma \in \overline{A}$, il existe $E$ dans $\Lambda$ tel que l’ensemble $U_E(\sigma)$ soit contenu dans $A$. L’*adhérence* $\overline{A}$ de $A$ se compose des $\sigma \in \Gamma$ tels que pour tout $E \in \Lambda$, il existe $\tau \in A$ ayant même restriction à $E$ que $\sigma$ ; le corps des invariants de $\overline{A}$ est le même que celui de $A$.

Soit ε l’élément neutre de Γ, et soit Λ’ l’ensemble des sous-extensions de N qui sont galoisiennes et de degré fini sur K. D’après la prop. 2 (V, p. 55), l’ensemble Λ’ est cofinal dans Λ et la famille $(U_E(\varepsilon))_{E \in \Lambda'}$ est donc une base du filtre des voisinages de ε dans Γ. De plus, pour E ∈ Λ’, l’ensemble $U_E(\varepsilon)$ est le noyau de l’homomorphisme de restriction de Gal(N/K) = Γ dans Gal(E/K). Comme le groupe Gal(E/K) est fini, il en résulte que $U_E(\varepsilon)$ est un sous-groupe ouvert et fermé, distingué et d’indice fini dans Γ.

On a évidemment $U_E(\sigma) = \sigma U_E(\varepsilon) = U_E(\varepsilon) \sigma$ pour $σ \in Γ$ et $E \in Λ'$. Comme $U_E(\varepsilon)$ est un sous-groupe distingué de Γ pour tout $E \in Λ'$, et que la famille $(U_E(\varepsilon))_{E \in Λ'}$ est une base de voisinages de ε, la topologie de Γ est compatible avec sa structure de groupe (TG, III, p. 5). Autrement dit, l’application $(σ, τ) \mapsto στ^{-1}$ de $Γ \times Γ$ dans Γ est continue.

#### Proposition 4 {#alg-v-s10-prop-4 .statement}

*Soit N une extension galoisienne de K. Le groupe de Galois Γ = Gal(N/K) est compact et totalement discontinu.*

Tout élément σ de Γ a une base de voisinages formée des ensembles ouverts et fermés $U_E(σ)$, donc Γ est totalement discontinu (TG, I, p. 83). On a $\{σ\} = \bigcap_{E \in Λ} U_E(σ)$, donc Γ est séparé. Pour tout $x \in N$, l’ensemble des conjugués $σ(x)$ de x, où σ parcourt Γ, est *fini* puisque x est algébrique sur K (V, p. 51, cor. 1); toutes les projections de Γ sur les espaces facteurs de $N^N$ sont donc des ensembles finis, ce qui prouve que Γ est relativement compact dans $N^N$ (TG, I, p. 64). Il reste à prouver que Γ est *fermé* dans $N^N$. Or, si u est adhérent à Γ dans $N^N$, pour tout couple $(x, y)$ de points de N, il existe $σ \in Γ$ avec $u(x) = σ(x), u(y) = σ(y), u(x + y) = σ(x + y), u(xy) = σ(xy)$, d’où $u(x + y) = u(x) + u(y)$ et $u(xy) = u(x) u(y)$. Par le même raisonnement, on a $u(x) = x$ pour $x \in K$, donc u est un K-homomorphisme de N dans N; comme N est algébrique sur K, u est un K-automorphisme de N (V, p. 50, prop. 1), donc $u \in Γ$.

Soient N une extension galoisienne de K et $(N_i)_{i \in I}$ une famille filtrante croissante de sous-extensions de N. On suppose que $N_i$ est galoisienne sur K pour tout $i \in I$ et que $N = \bigcup_{i \in I} N_i$. Pour tout $i \in I$, notons $Γ_i$ le groupe de Galois de $N_i$ sur K ; pour $i \leq j$ dans I, on a $N_i \subset N_j$ et l’homomorphisme de restriction $\varphi_{ij}$ de $Γ_j$ dans $Γ_i$ est défini. Il est continu et la famille $(Γ_i, \varphi_{ij})$ est donc un système projectif de groupes topologiques. Par ailleurs, pour tout $i \in I$, notons $\lambda_i$ l’homomorphisme de restriction de Gal(N/K) dans Gal(N_i/K) = $Γ_i$; il est continu et l’on a $\lambda_i = \varphi_{ij} \circ \lambda_j$ pour $i \leq j$, donc la famille $(\lambda_i)_{i \in I}$ définit un homomorphisme continu $λ$ de Gal(N/K) dans $\lim_{\leftarrow} Γ_i$.

#### Proposition 5 {#alg-v-s10-prop-5 .statement}

*L’homomorphisme λ de Gal(N/K) dans $\lim_{\leftarrow} \mathrm{Gal}(N_i/K)$ est un isomorphisme de groupes topologiques.*

Comme Gal(N/K) est compact, que λ est continu et que le groupe $\lim_{\leftarrow} \mathrm{Gal}(N_i/K)$ est séparé, il suffit de prouver que λ est bijectif (TG, I, p. 63, cor. 2). Soit $u = (u_i)_{i \in I}$ un élément de $\lim_{\leftarrow} \mathrm{Gal}(N_i/K)$; pour tout $i \in I$, $u_i$ est un K-automorphisme de $N_i$, et $u_i$ est la restriction de $u_j$ à $N_i$ pour $i \leq j$. Comme on a $N = \bigcup_{i \in I} N_i$, il existe un unique élément $\sigma$ de $\mathrm{Gal}(N/K)$ qui coïncide avec $u_i$ sur $N_i$ pour tout $i \in I$. Alors $\sigma$ est l’unique élément de $\mathrm{Gal}(N/K)$ tel que $\lambda(\sigma) = u$, donc $\lambda$ est bijectif.

Cela s’applique notamment lorsqu’on prend pour famille $(N_i)$ la famille de toutes les sous-extensions galoisiennes finies de $N$; alors chaque groupe $\mathrm{Gal}(N_i/K)$ est discret et fini. Le groupe topologique $\mathrm{Gal}(N/K)$ est donc isomorphe à une limite projective filtrante de groupes finis, munis de la topologie discrète ; on dit parfois que c’est un groupe topologique profini.

### 4. Descente galoisienne

Dans tout ce numéro, on note $N$ un corps, $\Gamma$ un groupe d’automorphismes de $N$, $\varepsilon$ l’élément neutre de $\Gamma$, et $K$ le corps des invariants de $\Gamma$.

Soit $V$ un espace vectoriel sur $N$. Rappelons (II, p. 119) qu’une $K$-structure sur $V$ est un sous-$K$-espace vectoriel $V_0$ de $V$ tel que l’application $K$-linéaire $\varphi : N \otimes_K V_0 \to V$ qui transforme $\lambda \otimes x$ en $\lambda x$ soit bijective. Soit $V_0$ une telle $K$-structure ; pour tout $\sigma \in \Gamma$, on pose $u_\sigma = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0}) \circ \varphi^{-1}$. On a alors $u_\sigma(\sum_{i \in I} \lambda_i e_i) = \sum_{i \in I} \sigma(\lambda_i) e_i$ pour toute famille d’éléments $\lambda_i$ de $N$ et $e_i$ de $V_0$, d’où les relations
$$
\begin{align*}
(1) \quad &u_\sigma(x + y) = u_\sigma(x) + u_\sigma(y) \\
(2) \quad &u_\sigma(\lambda x) = \sigma(\lambda) u_\sigma(x) \\
(3) \quad &u_\sigma \circ u_\tau = u_{\sigma \tau} \\
(4) \quad &u_\varepsilon = \mathrm{Id}_V
\end{align*}
$$
pour $\sigma, \tau$ dans $\Gamma$, $x, y$ dans $V$ et $\lambda$ dans $N$.

#### Proposition 6 {#alg-v-s10-prop-6 .statement}

a) Soit $V$ un espace vectoriel sur $N$ muni d’une $K$-structure. Pour qu’un vecteur $x \in V$ soit rationnel sur $K$, il faut et il suffit qu’on ait $u_\sigma(x) = x$ pour tout $\sigma \in \Gamma$. Pour qu’un sous-N-espace vectoriel $W$ de $V$ soit rationnel sur $K$, il faut et il suffit qu’on ait $u_\sigma(W) \subset W$ pour tout $\sigma \in \Gamma$.

b) Soient $V_1$ et $V_2$ deux espaces vectoriels sur $N$, munis chacun d’une $K$-structure. Pour qu’une application linéaire $f$ de $V_1$ dans $V_2$ soit rationnelle sur $K$, il faut et il suffit qu’on ait $f(u_\sigma(x)) = u_\sigma(f(x))$ pour tout $\sigma \in \Gamma$ et tout $x \in V_1$.

Il est clair que $K$ est l’ensemble des $x \in N$ tels que $\sigma(xy) = x \sigma(y)$ pour tout $\sigma \in \Gamma$ et tout $y \in N$. La proposition résulte alors du th. 1 (II, p. 125).

#### Corollaire {#alg-v-s10-n4-cor-1 .statement}

Soit $V_0$ un espace vectoriel sur $K$ et soit $W$ un sous-N-espace vectoriel de $N \otimes_K V_0$. On suppose que $W$ est stable par les applications $\sigma \otimes \mathrm{Id}_{V_0}$ pour tout $\sigma \in \Gamma$. Soit $W_0$ l’ensemble des $x \in V_0$ tels que $1 \otimes x \in W$. Alors $W_0$ est l’unique sous-K-espace vectoriel de $V_0$ tel que $W = N \otimes_K W_0$.

Il suffit de noter que l’ensemble des éléments de la forme $1 \otimes x$ ($x \in V_0$) est une $K$-structure sur $N \otimes_K V_0$ pour laquelle on a $u_\sigma = \sigma \otimes \mathrm{Id}_{V_0}$ pour $\sigma \in \Gamma$.

#### Proposition 7 {#alg-v-s10-prop-7 .statement}

Soient V un espace vectoriel sur N, $(u_\sigma)_{\sigma \in \Gamma}$ une famille d’applications de V dans V satisfaisant aux relations (1) à (4) et $V_0$ l’ensemble des $x \in V$ tels que $u_\sigma(x) = x$ pour tout $\sigma \in \Gamma$.

a) $V_0$ est un sous-$\mathbf{K}$-espace vectoriel de V et l’application $\mathbf{K}$-linéaire $\varphi$ de $N \otimes_K V_0$ dans V qui transforme $\lambda \otimes x$ en $\lambda x$ est injective.

b) Si $\Gamma$ est fini, alors $\varphi$ est bijective et $V_0$ est une $\mathbf{K}$-structure sur V.

Il est clair que $V_0$ est un sous-$\mathbf{K}$-espace vectoriel de V.

La formule $u_\sigma \circ \varphi = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0})$ montre que le noyau W de $\varphi$ est stable par les applications $\sigma \otimes \mathrm{Id}_{V_0}$; d’après le corollaire de la prop. 6, il existe donc un sous-espace $W_0$ de $V_0$ tel que $W = N \otimes_K W_0$. Si $x$ appartient à $W_0$, on a donc $x = \varphi(1 \otimes x) = 0$, d’où $W_0 = 0$ et donc $W = 0$. Ceci prouve a).

Supposons $\Gamma$ fini; il s’agit de prouver que $\varphi$ est surjective, ou encore que $V_0$ engendre le N-espace vectoriel V. Soit donc $f$ une forme N-linéaire sur V, dont la restriction à $V_0$ soit nulle. Soit $x \in V$; pour tout $\lambda \in N$, l’élément $y_\lambda = \sum_{\sigma \in \Gamma} u_\sigma(\lambda x)$ de V appartient évidemment à $V_0$, d’où $f(y_\lambda) = 0$, c’est-à-dire $\sum_{\sigma \in \Gamma} f(u_\sigma(x)) \sigma(\lambda) = 0$. D’après le théorème de Dedekind (V, p. 27, cor. 2), on a donc $f(u_\sigma(x)) = 0$ pour tout $\sigma \in \Gamma$; faisant en particulier $\sigma = \varepsilon$, on trouve $f(x) = 0$, c’est-à-dire $f = 0$. Ceci prouve b).

Soit M un espace vectoriel sur N; pour tout $\sigma \in \Gamma$, soit $M^\sigma$ l’espace vectoriel sur N ayant même groupe additif sous-jacent que M, avec la loi externe $(\lambda, x) \mapsto \sigma(\lambda)x$. Posons $V = \prod_{\sigma \in \Gamma} M^\sigma$; le groupe additif sous-jacent de V est celui des applications de $\Gamma$ dans M, avec la loi externe définie par

$$(5)$$
$$(\lambda . h)(\sigma) = \sigma(\lambda) h(\sigma) \quad (\lambda \in N, h \in V, \sigma \in \Gamma).$$

(Le produit $\sigma(\lambda) h(\sigma)$ est calculé dans l’espace vectoriel M.) Par ailleurs on définit sur $N \otimes_K M$ une structure d’espace vectoriel sur N par la formule
$$\lambda (\sum_i \mu_i \otimes x_i) = \sum_i \lambda \mu_i \otimes x_i.$$

Enfin, on note $\psi$ l’application $\mathbf{K}$-linéaire de $N \otimes_K M$ dans V caractérisée par la relation
$$(6)$$
$$\psi(\lambda \otimes x)(\sigma) = \sigma(\lambda) . x$$
pour $\lambda \in N, x \in M$ et $\sigma \in \Gamma$. Il est immédiat que $\psi$ est N-linéaire.

#### Proposition 8 {#alg-v-s10-prop-8 .statement}

L’application N-linéaire $\psi$ de $N \otimes_K M$ dans $V = \prod_{\sigma \in \Gamma} M^\sigma$ est injective, et elle est bijective si $\Gamma$ est fini.

Pour tout $\sigma \in \Gamma$, on définit une application $u_\sigma$ de V dans V par
$$(7)$$
$$(u_\sigma h)(\tau) = h(\tau \sigma)$$
pour $h \in V$ et $\tau \in \Gamma$. La vérification des formules (1) à (4) est immédiate. Notons $V_0$ l’ensemble des $h \in V$ tels que $u_\sigma(h) = h$ pour tout $\sigma \in \Gamma$. Pour tout $x \in M$, soit $\theta(x)$ l’application constante de $\Gamma$ dans $M$ de valeur $x$; alors $\theta$ est un $K$-isomorphisme de $M$ sur $V_0$. Définissons l’homomorphisme $\varphi : N \otimes_K V_0 \to V$ comme plus haut; on a $\psi = \varphi \circ (\mathrm{Id}_N \otimes \theta)$, et la prop. 8 résulte alors de la prop. 7.

#### Corollaire {#alg-v-s10-n4-cor-2 .statement}

*Soit $\psi$ l’application $K$-linéaire de $N \otimes_K N$ dans l’espace vectoriel produit $N^\Gamma$ telle que $\psi(x \otimes y)(\sigma) = \sigma(x)\ y$ pour $x,\ y$ dans $N$ et $\sigma \in \Gamma$. Alors $\psi$ est injective et elle est bijective si $\Gamma$ est fini.*

C’est le cas particulier $M = N$ de la proposition 8.

#### Remarque 1 {#alg-v-s10-n4-rem-1 .statement}

Soient $F$ une extension de $K$ et $N$ une sous-extension de $F$. Soit $\Gamma$ un groupe *fini* d’automorphismes de $N$, dont $K$ soit le corps des invariants. La prop. 8 entraîne l’existence d’un isomorphisme de $K$-algèbres $\theta : N \otimes_K F \to F^\Gamma$ caractérisé par $\theta(x \otimes y)(\sigma) = \sigma(x)\ y$ pour $x \in N,\ y \in F$ et $\sigma \in \Gamma$.

#### Remarque 2 {#alg-v-s10-n4-rem-2 .statement}

Les notations $K, N$ et $\Gamma$ ont la signification précédente. Pour tout entier $n \geqslant 1$, soit $A_n$ le produit tensoriel de $n$ $K$-algèbres identiques à $N$; soit $B_n$ l’ensemble des applications de $\Gamma^{n-1}$ dans $N$. Par récurrence sur $n$, on déduit du corollaire de la prop. 8 l’existence d’un isomorphisme $\varphi_n : A_n \to B_n$ transformant $x_1 \otimes \ldots \otimes x_n$ en la fonction $(\sigma_1, \ldots, \sigma_{n-1}) \mapsto \sigma_1(x_1) \ldots \sigma_{n-1}(x_{n-1})\ x_n$.

### 5. Cohomologie galoisienne

Soient $N$ un corps, $\Gamma$ un groupe *fini* d’automorphismes de $N$ et $K$ le corps des invariants de $\Gamma$. Pour tout entier $n \geqslant 1$, on note $\mathbf{GL}(n, N)$ le groupe des matrices carrées d’ordre $n$, à coefficients dans $N$ et de déterminant non nul (II, p. 149). On fait opérer le groupe $\Gamma$ sur le groupe $\mathbf{GL}(n, N)$ par la règle $\sigma(A) = (\sigma(a_{ij}))$ pour $A = (a_{ij})$.

#### Proposition 9 {#alg-v-s10-prop-9 .statement}

*Soit $(U_\sigma)_{\sigma \in \Gamma}$ une famille d’éléments de $\mathbf{GL}(n, N)$. Pour qu’il existe $A$ dans $\mathbf{GL}(n, N)$ avec $U_\sigma = A^{-1} \cdot \sigma(A)$ pour tout $\sigma \in \Gamma$, il faut et il suffit que l’on ait $U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau)$ pour $\sigma, \tau$ dans $\Gamma$.

La condition est nécessaire : si l’on a $U_\sigma = A^{-1} \cdot \sigma(A)$, on a
$$
U_\sigma \cdot \sigma(U_\tau) = A^{-1} \cdot \sigma(A) \ \sigma(A^{-1} \cdot \tau(A)) = A^{-1} \sigma \tau(A) = U_{\sigma \tau}.
$$
La condition est *suffisante* : on identifie les éléments de $N^n$ aux matrices à $n$ lignes et une colonne à coefficients dans $N$. On fait agir le groupe $\Gamma$ sur $N^n$ par
$$
\sigma(x) = (\sigma(x_i))_{1 \leqslant i \leqslant n} \text{ pour } x = (x_i)_{1 \leqslant i \leqslant n}.
$$
Pour tout $\sigma \in \Gamma$, on note $u_\sigma$ l’application $x \mapsto U_\sigma \cdot \sigma(x)$ de $N^n$ dans lui-même. La vérification des formules (1) à (3) de V, p. 60, est immédiate. De plus, on a $u_\varepsilon \circ u_\varepsilon = u_\varepsilon$ et comme $u_\varepsilon$ est bijective, on a $u_\varepsilon = \mathrm{Id}_{N^n}$. Soit $V_0$ l’ensemble des vecteurs $x \in N^n$ tels que $u_\sigma(x) = x$ pour tout $\sigma \in \Gamma$. D’après la prop. 7 (V, p. 61), $V_0$ est une $K$-structure sur $N^n$; en particulier, il existe dans $V_0$ des vecteurs $b_1, \ldots, b_n$ formant une base de $N^n$ sur $N$. La matrice $B$ ayant pour colonnes $b_1, \ldots, b_n$ est donc inversible, et la relation $u_\sigma(b_i) = b_i$ pour $1 \leqslant i \leqslant n$ équivaut à $U_\sigma \cdot \sigma(B) = B$. Posant $A = B^{-1}$, on obtient $U_\sigma = A^{-1} \sigma(A)$ pour tout $\sigma \in \Gamma$.

#### Corollaire 1 {#alg-v-s10-prop-9-cor-1 .statement}

Soit $(c_\sigma)_{\sigma \in \Gamma}$ une famille d’éléments non nuls de $\mathbf{N}$. Pour qu’il existe $a \neq 0$ dans $\mathbf{N}$ tel que $c_\sigma = \sigma(a) \cdot a^{-1}$ pour tout $\sigma \in \Gamma$, il faut et il suffit qu’on ait $c_{\sigma \tau} = c_\sigma \cdot \sigma(c_\tau)$ pour $\sigma, \tau$ dans $\Gamma$.

#### Corollaire 2 {#alg-v-s10-prop-9-cor-2 .statement}

Soit $(a_\sigma)_{\sigma \in \Gamma}$ une famille d’éléments de $\mathbf{N}$. Pour qu’il existe $b$ dans $\mathbf{N}$ avec $a_\sigma = \sigma(b) - b$ pour tout $\sigma \in \Gamma$, il faut et il suffit que l’on ait $a_{\sigma \tau} = a_\sigma + \sigma(a_\tau)$ pour $\sigma, \tau$ dans $\Gamma$.

On a $\sigma \tau(b) - b = [\sigma(b) - b] + \sigma[\tau(b) - b]$ pour tout $b$ dans $\mathbf{N}$, et $\sigma, \tau$ dans $\Gamma$, d’où la nécessité.

Réciproquement, supposons qu’on ait $a_{\sigma \tau} = a_\sigma + \sigma(a_\tau)$ quels que soient $\sigma$ et $\tau$ dans $\Gamma$. Posons $U_\sigma = \begin{pmatrix} 1 & a_\sigma \\ 0 & 1 \end{pmatrix}$ pour $\sigma \in \Gamma$. On a alors $U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau)$ pour $\sigma, \tau$ dans $\Gamma$; d’après la prop. .9, il existe donc une matrice $A = \begin{pmatrix} x & y \\ z & t \end{pmatrix}$ de déterminant non nul, telle que $\sigma(A) = AU_\sigma$ pour tout $\sigma \in \Gamma$; en explicitant la relation $\sigma(A) = AU_\sigma$, on trouve

$$
\begin{pmatrix} \sigma(x) & \sigma(y) \\ \sigma(z) & \sigma(t) \end{pmatrix} = \begin{pmatrix} x & xa_\sigma + y \\ z & za_\sigma + t \end{pmatrix} \quad (\sigma \in \Gamma).
$$

En particulier, $x$ et $z$ appartiennent à $\mathbf{K}$ et l’on a

$$
\sigma(y) = xa_\sigma + y, \quad \sigma(t) = za_\sigma + t \quad (\sigma \in \Gamma).
$$

Si $x \neq 0$, on a $a_\sigma = \sigma(b) - b$ avec $b = x^{-1}y$; si $z \neq 0$, on a la même relation avec $b = z^{-1}t$. Or $x$ et $z$ ne sont pas tous deux nuls puisque l’on a

$$
xt - yz = \det A \neq 0.
$$

### 6. Le théorème d’Artin

#### Théorème 2 (Artin) {#alg-v-s10-thm-2 .statement}

Soient $\mathbf{N}$ un corps, $\Gamma$ un groupe d’automorphismes de $\mathbf{N}$ et $\mathbf{K}$ le corps des invariants de $\Gamma$. Soit $V$ un sous-$\mathbf{K}$-espace vectoriel de $\mathbf{N}$, de dimension finie sur $\mathbf{K}$. Alors toute application $\mathbf{K}$-linéaire $u$ de $V$ dans $\mathbf{N}$ est combinaison linéaire à coefficients dans $\mathbf{N}$ de restrictions à $V$ d’éléments de $\Gamma$.

Soit $u$ une application $\mathbf{K}$-linéaire de $V$ dans $\mathbf{N}$ et soit $V_{(\mathbf{N})} = \mathbf{N} \otimes_{\mathbf{K}} V$ le $\mathbf{N}$-espace vectoriel déduit de $V$ par extension des scalaires; notons $\tilde{u}$ la forme $\mathbf{N}$-linéaire sur $V_{(\mathbf{N})}$ telle que $\tilde{u}(x \otimes y) = x \cdot u(y)$ pour $x \in \mathbf{N}$ et $y \in V$. Pour tout $\sigma \in \Gamma$, il existe une forme $\mathbf{N}$-linéaire $h_\sigma$ sur $V_{(\mathbf{N})}$ telle que $h_\sigma(x \otimes y) = x \sigma(y)$ pour $x \in \mathbf{N}$ et $y \in V$. L’application canonique de $V_{(\mathbf{N})} = \mathbf{N} \otimes_{\mathbf{K}} V$ dans $\mathbf{N} \otimes_{\mathbf{K}} \mathbf{N}$ est injective. Le cor. de la prop. 8 (V, p. 62) montre alors que l’intersection des noyaux des formes linéaires $h_\sigma$ sur $V_{(\mathbf{N})}$ est réduite à 0. Par suite (II, p. 104, cor. 1), il existe $\sigma_1, ..., \sigma_n$ dans $\Gamma$ et $a_1, ..., a_n$ dans $\mathbf{N}$ tels que $\tilde{u} = \sum_{i=1}^n a_i h_{\sigma_i}$, d’où $u(x) = \sum_{i=1}^n a_i \sigma_i(x)$ pour tout $x \in V$.

Munissons l’ensemble $\mathbf{N}^\mathbf{N}$ de toutes les applications de $\mathbf{N}$ dans $\mathbf{N}$ de la topologie produit des topologies discrètes des facteurs. Le th. 2 signifie que l’ensemble des combinaisons linéaires à coefficients dans $\mathbf{N}$ des éléments de $\Gamma$ est dense dans l’ensemble des applications $\mathbf{K}$-linéaires de $\mathbf{N}$ dans $\mathbf{N}$.

#### Théorème 3 {#alg-v-s10-thm-3 .statement}

*Soient $\mathbf{N}$ un corps, $\Gamma$ un groupe fini d’automorphismes de $\mathbf{N}$ et $\mathbf{K}$ le corps des invariants de $\Gamma$. Soit $n$ le cardinal de $\Gamma$.
a) *On a $[\mathbf{N} : \mathbf{K}] = n$ et $\mathbf{N}$ est une extension galoisienne de $\mathbf{K}$, de groupe de Galois $\Gamma$.
b) *Soient $\sigma_1, \ldots, \sigma_n$ les éléments de $\Gamma$ et $(x_1, \ldots, x_n)$ une base de $\mathbf{N}$ sur $\mathbf{K}$. Alors on a $\det (\sigma_i(x_j)) \neq 0$.
c) *Soit $u$ une application $\mathbf{K}$-linéaire de $\mathbf{N}$ dans $\mathbf{N}$. Il existe une unique famille $(a_\sigma)_{\sigma \in \Gamma}$ d’éléments de $\mathbf{N}$ telle que $u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x)$ pour tout $x \in \mathbf{N}$.*

On munit l’anneau $\mathbf{N} \otimes_\mathbf{K} \mathbf{N}$ de la structure de $\mathbf{N}$-algèbre dont la loi externe est caractérisée par $\lambda(x \otimes y) = x \otimes \lambda y$ pour $\lambda, x, y$ dans $\mathbf{N}$. Alors la dimension du $\mathbf{N}$-espace vectoriel $\mathbf{N} \otimes_\mathbf{K} \mathbf{N}$ est égale à $[\mathbf{N} : \mathbf{K}]$. La dimension du $\mathbf{N}$-espace vectoriel produit $\mathbf{N}^\Gamma$ est égale à $n$. L’application $\psi$ définie dans le cor. de la prop. 8 (V, p. 62) est un $\mathbf{N}$-isomorphisme de $\mathbf{N} \otimes_\mathbf{K} \mathbf{N}$ sur $\mathbf{N}^\Gamma$, d’où $[\mathbf{N} : \mathbf{K}] = n$. Soit $\Delta$ le groupe des $\mathbf{K}$-automorphismes de $\mathbf{N}$. On a $\Gamma \subset \Delta$, donc $\mathbf{K}$ est le corps des invariants de $\Delta$, et $\mathbf{N}$ est extension galoisienne de $\mathbf{K}$. De plus, l’ordre de $\Delta$ est au plus égal à $[\mathbf{N} : \mathbf{K}]$ d’après le théorème de Dedekind (V, p. 27, cor. 2) et comme l’ordre de $\Gamma$ est égal à $[\mathbf{N} : \mathbf{K}]$, on a $\Gamma = \Delta$. Donc $\Gamma$ est le groupe de Galois de $\mathbf{N}$ sur $\mathbf{K}$. Ceci prouve a).
Avec les notations de b), posons $f_i = \psi(x_i \otimes 1)$; on a $f_i(\sigma) = \sigma(x_i)$ pour $1 \leq i \leq n$ et $\sigma \in \Gamma$. Comme $\psi$ est un isomorphisme de $\mathbf{N}$-espaces vectoriels, la suite $(f_1, \ldots, f_n)$ est une base de $\mathbf{N}^\Gamma$ sur $\mathbf{N}$, d’où $\det(f_j(\sigma_i)) \neq 0$, c’est-à-dire
$$
\det (\sigma_i(x_j)) \neq 0.
$$
Ceci prouve b).
Enfin, l’assertion c) résulte du th. 2 (V, p. 63) qui prouve l’*existence* d’une famille $(a_\sigma)_{\sigma \in \Gamma}$ telle que $u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x)$ (pour tout $x \in \mathbf{N}$), et du théorème de Dedekind (V, p. 27, cor. 2) qui prouve l’unicité de $(a_\sigma)_{\sigma \in \Gamma}$.

7. **Le théorème fondamental de la théorie de Galois**

#### Théorème 4 {#alg-v-s10-thm-4 .statement}

*Soient $\mathbf{N}$ une extension galoisienne de $\mathbf{K}$ et $\Gamma$ son groupe de Galois. Soit $\mathcal{K}$ l’ensemble des sous-extensions de $\mathbf{N}$ et soit $\mathcal{G}$ l’ensemble des sous-groupes fermés de $\Gamma$. Pour tout sous-groupe $\Delta \in \mathcal{G}$, on note $k(\Delta)$ le corps des invariants de $\Delta$ et pour tout sous-corps $E \in \mathcal{K}$, on note $g(E)$ le groupe des $E$-automorphismes de $\mathbf{N}$. Alors $\Delta \mapsto k(\Delta)$ est une bijection de $\mathcal{G}$ sur $\mathcal{K}$, et $E \mapsto g(E)$ est la bijection réciproque.*
A) La relation $E = k(g(E))$ (pour $E \in \mathcal{K}$) résulte du lemme plus précis suivant :

#### Lemme 1 {#alg-v-s10-lem-1 .statement}

*Soit $E$ une sous-extension de $\mathbf{N}$. Alors $\mathbf{N}$ est extension galoisienne de $E$, et $\mathrm{Gal}(\mathbf{N}/E)$ est un sous-groupe fermé de $\mathrm{Gal}(\mathbf{N}/\mathbf{K})$, avec la topologie induite.*
Soit $x \in \mathbf{N}$; le polynôme minimal $f$ de $x$ sur $E$ divise dans $E[X]$ le polynôme minimal $g$ de $x$ sur $\mathbf{K}$ (V, p. 16, cor. 2). Comme $\mathbf{N}$ est galoisienne sur $\mathbf{K}$, le polynôme $g$ est produit dans $\mathbf{N}[X]$ de facteurs distincts de degré 1 ; il en est donc de même de $f$, donc $\mathbf{N}$ est galoisienne sur $E$.

Soient $\Gamma$ le groupe de Galois de $\mathbf{N}$ sur $K$ et $\Delta$ celui de $\mathbf{N}$ sur $E$. Par définition, $\Delta$ est le sous-groupe de $\Gamma$ formé des $\sigma$ tels que $\sigma(x) = x$ pour tout $x \in E$. Or, pour tout $x \in E$, l’application $\sigma \mapsto \sigma(x)$ de $\Gamma$ dans l’espace discret $\mathbf{N}$ est continue, donc $\Delta$ est fermé dans $\Gamma$. Soit $\sigma \in \Gamma$. Pour $x_1, \ldots, x_n$ dans $\mathbf{N}$, soit $U(x_1, \ldots, x_n)$ l’ensemble des $\tau \in \Gamma$ tels que $\tau(x_i) = \sigma(x_i)$ pour $1 \leq i \leq n$; posons
$$
V(x_1, \ldots, x_n) = U(x_1, \ldots, x_n) \cap \Delta.
$$
Alors la famille des ensembles $U(x_1, \ldots, x_n)$ (resp. $V(x_1, \ldots, x_n)$) est une base de voisinages de $\sigma$ dans $\Gamma$ (resp. $\Delta$). Donc la topologie de $\Delta$ est induite par celle de $\Gamma$.

B) La relation $\Delta = g(k(\Delta))$ (pour $\Delta \in \mathcal{G}$) résulte du lemme plus précis suivant :

#### Lemme 2 {#alg-v-s10-lem-2 .statement}

*Soit $\Delta$ un sous-groupe de $\Gamma$. Soit $E$ le corps des invariants de $\Delta$. Alors le groupe de Galois de $\mathbf{N}$ sur $E$ est l’adhérence de $\Delta$ dans $\Gamma$.*

Le groupe de Galois de $\mathbf{N}$ sur $E$ est fermé dans $\Gamma$ (lemme 1) et contient $\Delta$, donc il contient l’adhérence $\overline{\Delta}$ de $\Delta$. Soit $\sigma$ un $E$-automorphisme de $\mathbf{N}$ et soient $x_1, \ldots, x_n$ dans $\mathbf{N}$. Comme $\mathbf{N}$ est galoisien sur $E$ (lemme 1), il existe (V, p. 55, prop. 2) une sous-extension $\mathbf{N}_0$ de $\mathbf{N}$, galoisienne et de degré fini sur $E$, contenant $x_1, \ldots, x_n$. Soit $\Delta_0$ l’image du sous-groupe $\Delta$ de $\mathrm{Gal}(\mathbf{N}/E)$ par l’homomorphisme de restriction de $\mathrm{Gal}(\mathbf{N}/E)$ dans $\mathrm{Gal}(\mathbf{N}_0/E)$. Comme $[\mathbf{N}_0 : E]$ est fini, le théorème de Dedekind (V, p. 27, cor. 2) montre que $\mathrm{Gal}(\mathbf{N}_0/E)$ est fini. Donc $\Delta_0$ est fini, et comme $E$ est le corps des invariants de $\Delta_0$, on a $\Delta_0 = \mathrm{Gal}(\mathbf{N}_0/E)$ (V, p. 64, th. 3). En particulier, $\Delta_0$ contient la restriction de $\sigma$ à $\mathbf{N}_0$. Il existe donc $\tau \in \Delta$ tel que $\sigma$ et $\tau$ aient même restriction à $\mathbf{N}_0$, d’où $\sigma(x_1) = \tau(x_1), \ldots, \sigma(x_n) = \tau(x_n)$. Par suite, $\sigma$ est adhérent à $\Delta$ dans $\Gamma$, donc $\mathrm{Gal}(\mathbf{N}/E) \subset \overline{\Delta}$.

#### Corollaire 1 {#alg-v-s10-lem-2-cor-1 .statement}

*Soient $E$ et $E'$ deux sous-corps de $\mathbf{N}$ contenant $K$ ; on a $E \subset E'$ si et seulement si l’on a $g(E) \supset g(E')$. Si $\Delta$ et $\Delta'$ sont deux sous-groupes fermés de $\Gamma$, on a $\Delta \subset \Delta'$ si et seulement si $k(\Delta) \supset k(\Delta')$.*

En effet les deux bijections réciproques $E \mapsto g(E)$ et $\Delta \mapsto k(\Delta)$ sont décroissantes.

#### Corollaire 2 {#alg-v-s10-lem-2-cor-2 .statement}

*Soit $(E_i)_{i \in I}$ une famille de sous-corps de $\mathbf{N}$ contenant $K$ ; posons $L = \bigcap_{i \in I} E_i$ et $M = K(\bigcup_{i \in I} E_i)$. Alors $g(L)$ est le plus petit sous-groupe fermé de $\Gamma$ contenant $\bigcup_{i \in I} g(E_i)$ et l’on a $g(M) = \bigcap_{i \in I} g(E_i)$.*

La première assertion résulte du cor. 1 et la deuxième est immédiate.

#### Corollaire 3 {#alg-v-s10-lem-2-cor-3 .statement}

*Pour $i = 1, 2$, soit $E_i$ un sous-corps de $\mathbf{N}$ contenant $K$ et soit $\Delta_i = g(E_i)$. Pour tout $\sigma \in \Gamma$, les relations $\sigma(E_1) = E_2$ et $\sigma \Delta_1 \sigma^{-1} = \Delta_2$ sont équivalentes.*

En effet, on a $\tau \in g(\sigma(E_1))$ si et seulement si l’on a $\tau \sigma(x) = \sigma(x)$, c’est-à-dire $\sigma^{-1} \tau \sigma(x) = x$, pour tout $x \in E_1$ ; ceci équivaut encore à $\sigma^{-1} \tau \sigma \in \Delta_1$, d’où $g(\sigma(E_1)) = \sigma \Delta_1 \sigma^{-1}$.

#### Corollaire 4 {#alg-v-s10-lem-2-cor-4 .statement}

Soit $E$ un sous-corps de $N$ contenant $K$ et soit $\Delta = g(E)$. Pour que $E$ soit galoisien sur $K$, il faut et il suffit que $\Delta$ soit un sous-groupe distingué de $\Gamma$. S’il en est ainsi, l’homomorphisme de restriction de $\Gamma$ dans $\mathrm{Gal}(E/K)$ définit par passage au quotient un isomorphisme de groupes topologiques de $\Gamma / \Delta$ sur $\mathrm{Gal}(E/K)$.

Comme $N$ est séparable sur $K$, il en est de même de $E$ (V, p. 35, prop. 1). Par suite, $E$ est galoisien sur $K$ si et seulement s’il est quasi-galoisien sur $K$; ceci signifie aussi qu’on a $\sigma(E) = E$ pour tout $K$-automorphisme $\sigma$ de $N$ (V, p. 50, prop. 1 et p. 52, prop. 3). D’après le cor. 3, ceci équivaut à $\sigma \Delta \sigma^{-1} = \Delta$ pour tout $\sigma \in \Gamma$.

L’homomorphisme de restriction $\varphi : \mathrm{Gal}(N/K) \to \mathrm{Gal}(E/K)$ est continu et surjectif (V, p. 58, prop. 3), et son noyau est évidemment égal à $\Delta = \mathrm{Gal}(N/E)$. Comme $\Gamma$ est compact, l’homomorphisme de $\Gamma / \Delta$ sur $\mathrm{Gal}(E/K)$ déduit de $\varphi$ par passage au quotient est un isomorphisme de groupes topologiques (TG, I, p. 63, cor. 2).

#### Corollaire 5 {#alg-v-s10-lem-2-cor-5 .statement}

Soit $E$ un sous-corps de $N$ contenant $K$. Pour que $E$ soit de degré fini sur $K$, il faut et il suffit que $g(E)$ soit ouvert dans $\Gamma$. S’il en est ainsi, l’indice $(\Gamma : g(E))$ est fini et égal à $[E : K]$.

Pour que $g(E)$ soit ouvert, il faut et il suffit qu’il existe une sous-extension $F$ de $N$, de degré fini sur $K$, telle que, avec les notations de V, p. 58, $g(E)$ contienne $U_F(\mathrm{Id}_N) = g(F)$. La relation $g(E) \supset g(F)$ équivaut à $E \subset F$ d’après le cor. 1 (V, p. 65), d’où la première assertion du cor. 5.

Supposons $[E : K]$ fini. Soit $\Omega$ une clôture algébrique de $K$ contenant $N$ comme sous-extension (V, p. 22, th. 2) et soit $\mathcal{H}$ l’ensemble des $K$-homomorphismes de $E$ dans $\Omega$. Tout élément de $\mathcal{H}$ est induit par un $K$-automorphisme de $\Omega$ (V, p. 50, prop. 1), et comme $N$ est quasi-galoisienne sur $K$, l’application $\sigma \mapsto \sigma|E$ de $\Gamma$ dans $\mathcal{H}$ est surjective. Pour que $\sigma \in \Gamma$ et $\sigma' \in \Gamma$ aient même restriction à $E$, il faut et il suffit qu’on ait $\sigma^{-1} \sigma' \in g(E)$, d’où $\mathrm{Card} \, \mathcal{H} = (\Gamma : g(E))$. Enfin, comme $E$ est une algèbre étale sur $K$, on a $\mathrm{Card} \, \mathcal{H} = [E : K]$ (V, p. 31, prop. 4). En conclusion, on a $(\Gamma : g(E)) = [E : K]$.

#### Corollaire 6 {#alg-v-s10-lem-2-cor-6 .statement}

Pour $i = 1, 2$, soient $E_i$ une sous-extension de $N$ et $\Gamma_i$ le groupe de Galois de $N$ sur $E_i$. Les conditions suivantes sont équivalentes :
a) Le groupe $\Gamma$ est produit direct des sous-groupes $\Gamma_1$ et $\Gamma_2$.
b) Les extensions $E_1$ et $E_2$ sont galoisiennes sur $K$, on a $E_1 \cap E_2 = K$ et
$$
K(E_1 \cup E_2) = N.
$$

Pour que $\Gamma$ soit produit direct des sous-groupes $\Gamma_1$ et $\Gamma_2$, il faut et il suffit que les conditions suivantes soient remplies (A, I, p. 46, prop. 15) :
(i) les sous-groupes $\Gamma_1$ et $\Gamma_2$ sont distingués dans $\Gamma$;
(ii) on a $\Gamma_1 \cap \Gamma_2 = \{ \varepsilon \}$, où $\varepsilon$ est l’élément neutre de $\Gamma$;
(iii) on a $\Gamma = \Gamma_1 . \Gamma_2$.

Or (i) signifie que $E_1$ et $E_2$ sont galoisiennes sur $K$ (cor. 4). D’après le cor. 2, la condition (ii) équivaut à $N = K(E_1 \cup E_2)$. Enfin si (i) et (ii) sont vérifiées, $\Gamma_1 \Gamma_2$ est le plus petit sous-groupe de $\Gamma$ contenant $\Gamma_1 \cup \Gamma_2$; il est fermé car $\Gamma_1$ et $\Gamma_2$ sont compacts et l’application $(\sigma, \tau) \mapsto \sigma \tau$ de $\Gamma_1 \times \Gamma_2$ dans $\Gamma$ est continue (TG, I, p. 63, cor. 1). Le cor. 2 montre alors que (iii) équivaut à $E_1 \cap E_2 = K$. Ceci prouve l’équivalence de a) et b).

#### Remarque {#alg-v-s10-n6-rem-3 .statement}

Avec les notations du cor. 6, supposons les conditions a) et b) remplies. Les homomorphismes de restriction $\varphi_i : \Gamma \to \mathrm{Gal}(E_i/K)$ pour $i = 1, 2$ induisent des isomorphismes de groupes topologiques

$$
\Psi_1 : \Gamma_2 \to \mathrm{Gal}(E_1/K) , \quad \Psi_2 : \Gamma_1 \to \mathrm{Gal}(E_2/K) .
$$

D’après a), on voit que l’application $\sigma \mapsto (\varphi_1(\sigma), \varphi_2(\sigma))$ est un isomorphisme de groupes topologiques de $\mathrm{Gal}(N/K)$ sur $\mathrm{Gal}(E_1/K) \times \mathrm{Gal}(E_2/K)$.

8. Changement du corps de base

Soient $N$ une extension galoisienne de $K$ et $\Gamma$ le groupe de Galois de $N$ sur $K$; soit aussi $N'$ une extension galoisienne d’un corps $K'$, de groupe de Galois $\Gamma'$. On identifie $K$ (resp. $K'$) à son image dans $N$ (resp. $N'$). Soient $u$ un homomorphisme

$$
\begin{array}{ccc}
N & \xrightarrow{v} & N' \\
| & & | \\
K & \xrightarrow{u} & K'
\end{array}
$$

Fig. 1.

de $K$ dans $K'$ et $v$ un homomorphisme de $N$ dans $N'$, dont la restriction à $K$ soit égale à $u$ (cf. fig. 1). Soit $\sigma \in \Gamma'$; comme on a $u(K) \subset K'$, $\sigma$ est un $u(K)$-automorphisme de $N'$; de plus, $v(N)$ est extension galoisienne de $u(K)$, donc $\sigma$ induit un $u(K)$-automorphisme de $v(N)$ (V, p. 53, remarque 1). Autrement dit, pour tout $\sigma \in \Gamma'$, il existe un unique élément $v^*(\sigma)$ de $\Gamma$ tel que

$$
v \circ v^*(\sigma) = \sigma \circ v .
$$

L’application $v^*$ est un homomorphisme de $\mathrm{Gal}(N'/K')$ dans $\mathrm{Gal}(N/K)$. Pour tout $x \in N$, l’application $\sigma \mapsto v^*(\sigma)(x) = v^{-1}(\sigma(v(x)))$ de $\Gamma'$ dans l’espace discret $N$ est continue, donc $v^*$ est continue.

Trois cas particuliers sont importants :

a) Si $F$ est une extension galoisienne de $K$ et $E$ une sous-extension de $F$, on sait (V, p. 64, lemme 1) que $F$ est extension galoisienne de $E$. Appliquons ce qui précède au cas où $N = F, K' = E, N' = F$ et $v = \mathrm{Id}_F$. Alors $v^*$ n’est autre que l’injection canonique

$$
j : \mathrm{Gal}(F/E) \to \mathrm{Gal}(F/K) .
$$

On l’appelle parfois l’homomorphisme d’inflation.

b) Supposons de plus que $E$ soit galoisienne sur $K$. Appliquons ce qui précède au cas où $N = E, K' = K, N' = F$ et où $v$ est l’injection canonique de $E$ dans $F$. Alors $v^*$ n’est autre que l’homomorphisme de restriction

$$
\pi : \mathrm{Gal}(F/K) \to \mathrm{Gal}(E/K) .
$$

On sait (V, p. 58, prop. 3) que $\pi$ est surjectif, de noyau $\mathrm{Gal}(F/E)$, et définit par passage au quotient un isomorphisme de groupes topologiques de $\mathrm{Gal}(F/K)/\mathrm{Gal}(F/E)$ sur $\mathrm{Gal}(E/K)$ (V, p. 66, cor. 4).

c) Supposons que l’on ait $v^{-1}(K') = K$ et $N' = K'(v(N))$. Montrons que l’homomorphisme

$$
v^*: \mathrm{Gal}(N'/K') \to \mathrm{Gal}(N/K),
$$

est un isomorphisme de groupes topologiques, appelé parfois la translation. En effet, le groupe $\mathrm{Gal}(N'/K')$ est compact, le groupe $\mathrm{Gal}(N/K)$ est séparé et $v^*$ est continu ; il suffit donc (TG, I, p. 63, cor. 2) de prouver que $v^*$ est bijectif. Or tout élément $\sigma$ du noyau de $v^*$ est un automorphisme de $N'$ qui induit l’identité sur $K'$ et sur $v(N)$, donc $\sigma = \varepsilon$ puisque $N' = K'(v(N))$; par suite, $v^*$ est injectif. Par ailleurs, l’image de $v^*$ est un sous-groupe fermé $\Delta$ de $\mathrm{Gal}(N/K)$ (TG, I, p. 63, *ibid.*) et le corps des invariants de $\Delta$ est égal à $v^{-1}(K') = K$; par suite, on a $\Delta = \mathrm{Gal}(N/K)$ (V, p. 64, th. 4), donc $v^*$ est surjectif.

Le cas général se ramène par composition aux précédents. Remarquons tout d’abord que $K'(v(N))$ est le corps des invariants dans $N'$ du noyau $\Delta$ de $v^*$; comme $\Delta$ est un sous-groupe distingué de $\mathrm{Gal}(N'/K')$, l’extension $K'(v(N))$ de $K'$ est galoisienne (V, p. 66, cor. 4). Alors $v^*$ est composé des homomorphismes

$$
\mathrm{Gal}(N'/K') \xrightarrow{\pi} \mathrm{Gal}(K'(v(N))/K') \xrightarrow{\psi} \mathrm{Gal}(N/v^{-1}(K')) \xrightarrow{j} \mathrm{Gal}(N/K);
$$

dans cette suite, $\pi$ est l’homomorphisme de restriction associé au triplet $K' \subset K'(v(N)) \subset N'$, $\psi$ est l’isomorphisme de translation associé au carré central du diagramme (fig. 2) et $j$ est l’homomorphisme d’inflation associé au triplet $K \subset v^{-1}(K') \subset N$.

$$
\begin{array}{ccc}
N & \to & K'(v(N)) \to N' \\
\uparrow & & \uparrow \\
K & \to & v^{-1}(K') \to K'
\end{array}
$$

Fig. 2.

Le théorème suivant précise la structure des isomorphismes de translation.

#### Théorème 5 {#alg-v-s10-thm-5 .statement}

*Soient $N'$ une extension de $K$, engendrée par deux sous-extensions $K'$ et $N$. On suppose que $N$ est galoisienne sur $K$, de groupe de Galois $\Gamma$ et que $K' \cap N = K$. Alors l’extension $N'$ de $K'$ est galoisienne et l’homomorphisme canonique $\varphi$ de $K' \otimes_K N$ dans $N'$ est un isomorphisme. Soit $\sigma \in \mathrm{Gal}(N/K)$ et soit $\sigma'$ l’élément de $\mathrm{Gal}(N'/K')$ qui lui correspond par l’isomorphisme de translation ; on a $\sigma' \circ \varphi = \varphi \circ (\mathrm{Id}_{K'} \otimes \sigma)$.

On a $N' = K'(N)$ et $N$ est algébrique et séparable sur $K$; donc (V, p. 41, prop. 10), l’extension $N'$ de $K'$ est algébrique et séparable. D’après le cor. 4 de V, p. 53, l’extension $N'$ de $K'$ est quasi-galoisienne. Par suite, l’extension $N'$ de $K'$ est galoisienne. D’après c) ci-dessus, l’application $\sigma \mapsto \sigma|N$ est un isomorphisme $\lambda$ de $\mathrm{Gal}(N'/K')$ sur $\mathrm{Gal}(N/K)$.

On a $N' = K'[N]$ puisque $N$ est algébrique sur $K$ (V, p. 18, cor. 1), donc $\varphi$ est surjectif. Si $\sigma$ appartient à $\mathrm{Gal}(N/K)$, on a

$$
\lambda^{-1}(\sigma) \circ \varphi = \varphi \circ (\mathrm{Id}_{K'} \otimes \sigma)
$$

Par suite, le noyau de $\varphi$ est stable par les applications $\mathrm{Id}_{K'} \otimes \sigma$, donc de la forme $K' \otimes_K N_0$ avec $N_0 \subset N$ (V, p. 60, cor.). Pour $x$ dans $N_0$, on a $x = \varphi(1 \otimes x) = 0$, d’où $N_0 = 0$ et donc $\varphi$ est injectif.

#### Corollaire 1 {#alg-v-s10-thm-5-cor-1 .statement}

*Soit $E'$ un sous-corps de $N'$ contenant $K'$. Il existe un unique sous-corps $E$ de $N$, contenant $K$ et tel que $E' = K'(E)$. On a $E = E' \cap N$.*

Posons $E = E' \cap N$, d’où $E' \supset K'(E)$. Posons $\Gamma = \mathrm{Gal}(N/K)$ et $\Delta = \mathrm{Gal}(N/E)$, et définissons de manière analogue $\Gamma'$ et $\Delta'$. L’application $\hat{\lambda} : \sigma \mapsto \sigma|N$ est un isomorphisme de $\Gamma'$ sur $\Gamma$, et aussi de $\Delta'$ sur $\Delta$; autrement dit, $\Delta'$ se compose des $\sigma \in \Gamma'$ tels que $\hat{\lambda}(\sigma)$ appartienne à $\Delta$. Si $\sigma \in \Gamma'$ laisse fixes les éléments de $K'(E)$, on a $\hat{\lambda}(\sigma) \in \Delta$, d’où $\sigma \in \Delta'$ et $\sigma$ laisse fixes les éléments de $E'$; d’après le cor. 1 de V, p. 65, on a donc $K'(E) \supset E'$.

On a prouvé l’égalité $E' = K'(E)$, d’où $\varphi^{-1}(E') = K' \otimes_K E$. Si $F$ est un sous-corps de $N$ contenant $K$ et tel que $E' = K'(F)$, on a de même $\varphi^{-1}(E') = K' \otimes_K F$, d’où $F = E$.

#### Corollaire 2 {#alg-v-s10-thm-5-cor-2 .statement}

*Soit $N$ une extension galoisienne de $K$. On suppose que le groupe de Galois $\Gamma$ de $N$ sur $K$ est produit direct de deux sous-groupes fermés $\Gamma_1$ et $\Gamma_2$, et l’on note $E_i$ le corps des invariants de $\Gamma_i$ pour $i = 1, 2$. L’homomorphisme canonique de $E_1 \otimes_K E_2$ dans $N$ est un isomorphisme.*

On a $E_1 \cap E_2 = K$ et $N = K(E_1 \cup E_2)$ d’après le cor. 6 (V, p. 66), et il suffit alors d’appliquer le théorème 5.

#### Remarque {#alg-v-s10-n6-rem-4 .statement}

Soient $K$ et $K'$ deux corps et $u$ un homomorphisme de $K$ dans $K'$. Soit $K_s$ (resp. $K'_s$) une clôture séparable (V, p. 44, prop. 14) de $K$ (resp. $K'$) et $\Pi$ (resp. $\Pi'$) le groupe de Galois de $K_s$ sur $K$ (resp. $K'_s$ sur $K'$). Comme $K_s$ est une extension algébrique et séparable de $K$, et que l’extension $(K'_s, u)$ de $K$ est séparablement close, il existe (V, p. 44, cor.) un homomorphisme $v$ de $K_s$ dans $K'_s$ prolongeant $u$. On déduit de $v$ un homomorphisme continu $v^*$ de $\Pi'$ dans $\Pi$. Soit $v_1$ un autre prolongement de $u$. Comme $K_s$ est une extension quasi-galoisienne de $K$, il existe un élément $\sigma_0$ de $\Pi$ tel que $v_1 = v \circ \sigma_0$. On en déduit $v_1^*(\tau) = \sigma_0^{-1} v^*(\tau) \sigma_0$ pour tout $\tau \in \Pi$.

9. Théorème de la base normale

Soit $N$ une extension galoisienne de $K$, de groupe de Galois $\Gamma$. Identifions $\Gamma$ à la base canonique de l’algèbre de groupe $K^{(\Gamma)}$ (III, p. 19); on peut considérer $N$ comme un $K^{(\Gamma)}$-module à gauche (III, p. 20, exemple), de sorte qu’on a

$$
u \cdot x = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x) \text{ pour } x \in N \text{ et } u = \sum_{\sigma \in \Gamma} a_\sigma \sigma \text{ dans } K^{(\Gamma)}.
$$

Si $N$ est de degré fini sur $K$, le groupe $\Gamma$ est fini d’après le théorème de Dedekind (V, p. 27, cor. 2), et l’on peut définir l’élément $t = \sum_{\sigma \in \Gamma} \sigma$ de $K^{(\Gamma)}$; on a alors

$$
\operatorname{Tr}_{N/K}(x) = \sum_{\sigma \in \Gamma} \sigma(x),
$$

c’est-à-dire $\operatorname{Tr}_{N/K}(x) = t.x$ pour tout $x \in N$.

Définissons une action à droite de $\Gamma$ sur $N$ par $x^\sigma = \sigma^{-1}(x)$. De manière analogue, on peut considérer le groupe multiplicatif $N^*$ comme un $\mathbf{Z}^{(\Gamma)}$-module à droite, la loi externe étant notée $(x, u) \mapsto x^u$. Par exemple, la notation $x^{2\sigma + 3\tau + \pi}$, où $\sigma, \tau, \pi$ sont des éléments de $\Gamma$, désigne le produit $(x^\sigma)^2 \cdot (x^\tau)^3 \cdot x^\pi$. Si $N$ est de degré fini sur $K$, et si $t = \sum_{\sigma \in \Gamma} \sigma$ comme plus haut, on a $N_{N/K}(x) = \prod_{\sigma \in \Gamma} x^\sigma$, c’est-à-dire $N_{N/K}(x) = x^t$ pour tout $x \in N^*$.

Supposons désormais $N$ de degré fini sur $K$. Soit $x \in N$; pour que $\{ x \}$ soit une base du $K^{(\Gamma)}$-module $N$, il faut et il suffit que la famille $(\sigma(x))_{\sigma \in \Gamma}$ soit une base de $N$ sur $K$. On dit qu’une telle base est une *base normale de $N$ sur $K$*.

#### Théorème 6 {#alg-v-s10-thm-6 .statement}

*Soit $N$ une extension galoisienne de degré fini sur $K$ et soit $\Gamma$ le groupe de Galois de $N$ sur $K$. Il existe une base normale de $N$ sur $K$. Autrement dit, le $K^{(\Gamma)}$-module $N$ est libre de rang 1.*

Nous donnerons deux démonstrations de cet énoncé. La première utilise le lemme suivant qui sera démontré au chapitre VIII (§ 2, n° 5).
\* Lemme 3. — *Soient $A$ une $K$-algèbre, $M_1$ et $M_2$ deux $A$-modules de rang fini sur $K$. On suppose qu’il existe une extension $L$ de $K$ telle que les modules $L \otimes_K M_1$ et $L \otimes_K M_2$ sur l’anneau $L \otimes_K A$ soient isomorphes. Alors les $A$-modules $M_1$ et $M_2$ sont isomorphes.*

On appliquera le lemme 3 au cas où $A = K^{(\Gamma)}$, $M_1 = N$, $M_2 = A_s$ et $L = N$
D’après le cor. de V, p. 62, il existe un $K$-isomorphisme $\varphi$ de $N \otimes_K N$ sur $N \otimes_K K^{(\Gamma)}$ qui transforme $x \otimes y$ en $\sum_{\sigma \in \Gamma} x \sigma^{-1}(y) \otimes \sigma$. Il est immédiat que $\varphi$ est un isomorphisme de $N \otimes_K K^{(\Gamma)}$-modules, et le théorème résulte alors du lemme 3. \*

Pour la deuxième démonstration, nous utiliserons la proposition suivante :

#### Proposition 10 {#alg-v-s10-prop-10 .statement}

*Soit $x \in N$. Pour que $\{ x \}$ soit une base du $K^{(\Gamma)}$-module $N$, il faut et il suffit que $\det(\sigma \tau(x))_{\sigma, \tau \in \Gamma}$ soit non nul.*

Comme $K^{(\Gamma)}$ et $N$ ont même dimension sur $K$, dire que $\{ x \}$ est une base de $N$ sur $K^{(\Gamma)}$ signifie que l’application $a \mapsto ax$ de $K^{(\Gamma)}$ dans $N$ est injective. Cela signifie aussi que l’application $b \mapsto b(1 \otimes x)$ de $N \otimes_K K^{(\Gamma)}$ dans $N \otimes_K N$ est injective (II, p. 108, prop. 14). Or, il existe un isomorphisme de $N \otimes_K K^{(\Gamma)}$-modules de $N \otimes_K N$ sur $N \otimes_K K^{(\Gamma)}$ qui transforme $1 \otimes x$ en $\sum_{\sigma} \sigma^{-1}(x) \otimes \sigma$. Il s’ensuit que $\{ x \}$ est une base de $N$ sur $K^{(\Gamma)}$ si et seulement si, pour toute famille non nulle $(n_\tau)_{\tau \in \Gamma}$ d’éléments de $N$, on a $(\sum n_\tau \otimes \tau)(\sum \sigma^{-1}(x) \otimes \sigma) \neq 0$. Mais cette dernière relation signifie qu’il existe $\tau \in \Gamma$ tel que $\sum n_\tau \sigma^{-1} \tau(x) \neq 0$, d’où la proposition.

A) Supposons K infini ; l’application $x \mapsto \det(\sigma \tau(x))$ de N dans N est polynômiale sur K (IV, p. 51). Par extension des scalaires de K à N elle donne l’application analogue pour le N-espace vectoriel $N \otimes_K N$, et on vient de voir que cette dernière n’est pas identiquement nulle (puisque $N \otimes_K N$ est bien libre de rang 1 sur $N \otimes_K K^{(\Gamma)}$). Il existe donc $x \in N$ tel que $\det(\sigma \tau(x)) \neq 0$ (IV, p. 17, th. 2) ; plus généralement, d’après la même référence on a :

#### Proposition 11 {#alg-v-s10-prop-11 .statement}

Supposons K infini, et soit $P : N \to K$ une application polynômiale sur K non nulle. Il existe $x \in N$ tel que $P(x) \neq 0$ et que $\{ x \}$ soit une base de N sur $K^{(\Gamma)}$.

B) Supposons K fini. D’après la prop. 4 (V, p. 91) $^1$ toute extension de degré fini de K a un groupe de Galois cyclique. Nous allons donc considérer plus généralement le cas où le groupe $\Gamma$ est cyclique d’ordre $n$ ; on note $\gamma$ un générateur de $\Gamma$.

Le lemme suivant est un cas particulier de résultats plus généraux démontrés au chapitre VII. L’anneau A est, soit l’anneau $\mathbf{Z}$ des entiers rationnels, soit l’anneau de polynômes $K[X]$ sur le corps K.

#### Lemme 4 {#alg-v-s10-lem-4 .statement}

Soit M un A-module de torsion engendré par un nombre fini d’éléments $x_1, \ldots, x_h$. Il existe alors un élément x de M dont l’annulateur (II, p. 28) est égal à l’annulateur de M.

Dans les deux cas, A est un anneau intègre et tout idéal de A est principal. Lorsque $A = \mathbf{Z}$ (resp. $A = K[X]$), on note $\mathcal{P}$ l’ensemble des nombres premiers (resp. l’ensemble des polynômes unitaires irréductibles de $K[X]$). Pour tout élément $a \neq 0$ de A, il existe alors un élément inversible u de A et une famille $(v_p(a))_{p \in \mathcal{P}}$ à support fini d’entiers positifs tels que $a = u \prod_{p \in \mathcal{P}} p^{v_p(a)}$, et u et les entiers $v_p(a)$ sont déterminés de manière unique (I, p. 49 et IV, p. 13, prop. 13).

Soient $a_i$ l’annulateur de $x_i$ (pour $1 \leq i \leq h$) et a l’annulateur de M. Soient $a_1, \ldots, a_h, a$ des éléments non nuls de A tels que $a_i = Aa_i$ et $a = Aa$; comme on a $a = a_1 \cap \ldots \cap a_h$, il résulte de ce qui précède qu’on a

$$
v_p(a) = \sup_{1 \leq i \leq h} v_p(a_i) \quad \text{pour tout } p \in \mathcal{P}.
$$

Écrivons $a$ sous la forme $up_1^{n(1)} \cdots p_r^{n(r)}$ avec $p_1, \ldots, p_r$ distincts dans $\mathcal{P}$, des entiers $n(1) > 0, \ldots, n(r) > 0$ et un élément inversible u de A. Soit $j = 1, \ldots, r$; d’après la formule (10), il existe un entier $c(j)$ tel que $1 \leq c(j) \leq h$ et $v_{p_j}(a_{c(j)}) = n(j)$; il existe $b_j$ dans A avec $a_{c(j)} = p_j^{n(j)} b_j$, et l’élément $y_j = b_j x_{c(j)}$ a pour annulateur l’idéal $Ap_j^{n(j)}$.

Montrons que l’annulateur b de $y = y_1 + \cdots + y_r$ est égal à l’annulateur a de M. On a en tout cas $a \subset b$, donc b est de la forme $Ap_1^{m(1)} \cdots p_r^{m(r)}$ avec $0 \leq m(j) \leq n(j)$

1 Le lecteur vérifiera aisément que le théorème de la base normale n’est utilisé nulle part avant la démonstration de cette proposition.

pour $1 \leq j \leq r$. Si l’on avait $a \neq b$, il existerait un entier $j$ tel que $1 \leq j \leq r$ et $m(j) < n(j)$ et par suite $d_j = a/p_j$ annulerait $y$. Or on a $d_j y_k = 0$ pour $k \neq j$, d’où l’on déduirait $d_j y_j = 0$; mais l’annulateur de $y_j$ est $A p_j^{m(j)}$ et $d_j$ n’est pas multiple de $p_j^{m(j)}$. L’hypothèse $a \neq b$ est donc absurde.

Nous appliquerons le lemme 4 au cas où $A$ est l’anneau de polynômes $K[X]$, et où $M$ est le groupe commutatif $N$ muni de la loi externe définie par
$$
a . x = \sum_{k=0}^{\infty} c_k \gamma^k(x) \text{ pour } a = \sum_{k=0}^{\infty} c_k X^k \text{ dans } K[X] \text{ et } x \in N.
$$
On a $\gamma^n = 1$, donc le polynôme $X^n - 1$ appartient à $a$. Soit $F \in a$; d’après IV, p. 10, cor., il existe des éléments $c_0, c_1, \ldots, c_{n-1}$ de $K$ et $G \in K[X]$ tels que
$$
(11) \quad F(X) = c_0 + c_1 X + \cdots + c_{n-1} X^{n-1} + (X^n - 1) G(X).
$$
On a alors $c_0 + c_1 \gamma + \cdots + c_{n-1} \gamma^{n-1} = 0$ dans $\operatorname{Hom}_K(N, N)$, et comme les automorphismes $1, \gamma, \gamma^2, \ldots, \gamma^{n-1}$ de $N$ sont distincts, le théorème de Dedekind (V, p. 27, cor. 2) entraîne $c_0 = c_1 = \cdots = c_{n-1} = 0$. Finalement, on a
$$
F(X) = (X^n - 1) G(X), \text{ c’est-à-dire } a = (X^n - 1) K[X].
$$
D’après le lemme 4, il existe un élément $x$ de $N$ dont l’annulateur dans $K[X]$ est égal à $(X^n - 1) K[X]$. Comme les monômes $1, X, \ldots, X^{n-1}$ forment la base d’un sous-espace vectoriel de $K[X]$ supplémentaire de $(X^n - 1) K[X]$ (IV, p. 10, cor.) les éléments $x, \gamma(x), \ldots, \gamma^{n-1}(x)$ de $N$ sont linéairement indépendants sur $K$. Comme on a $[N : K] = n$ (V, p. 64, th. 3), la suite $(x, \gamma(x), \ldots, \gamma^{n-1}(x))$ est donc une base (normale) de $N$ sur $K$.

10. $\Gamma$-ensembles finis et algèbres étalées

Soient $K_s$ une clôture séparable de $K$ (V, p. 44, prop. 14) et $\Gamma$ le groupe de Galois de $K_s$ sur $K$. On appelle $\Gamma$-ensemble un ensemble $X$ muni d’une action $(\sigma, x) \mapsto \sigma x$ du groupe $\Gamma$, telle que le stabilisateur de tout point de $X$ soit un sous-groupe ouvert de $\Gamma$. Il revient au même de dire que l’application $(\sigma, x) \mapsto \sigma x$ de $\Gamma \times X$ dans $X$ est continue lorsqu’on munit $X$ de la topologie discrète.

Soit $X$ un $\Gamma$-ensemble fini. On définit une action du groupe $\Gamma$ sur la $K$-algèbre $K_s^X$ des applications de $X$ dans $K_s$ par la formule
$$
(12) \quad u_\sigma f(x) = \sigma(f(\sigma^{-1} x))
$$
pour $\sigma \in \Gamma$, $f \in K_s^X$ et $x \in X$. Soit $\Theta(X)$ l’ensemble des invariants de $\Gamma$ dans $K_s^X$; c’est la sous-$K$-algèbre de $K_s^X$ formée des applications $f : X \to K_s$ telles que $f(\sigma x) = \sigma(f(x))$ pour $\sigma \in \Gamma$ et $x \in X$.

#### Lemme 5 {#alg-v-s10-lem-5 .statement}

Soit $X$ un $\Gamma$-ensemble fini et soient $x_1, \ldots, x_n$ des points de $X$ tels que les orbites $\Gamma x_1, \ldots, \Gamma x_n$ forment une partition de $X$. Pour $1 \leq i \leq n$, soit $\Delta_i$ le stabilisateur de $x_i$ dans $\Gamma$, et soit $L_i$ le corps des invariants de $\Delta_i$. Alors $L_1, \ldots, L_n$ sont des extensions séparables de degré fini de $K$, et l’application $f \mapsto (f(x_1), \ldots, f(x_n))$ est un isomorphisme de $K$-algèbres de $\Theta(X)$ sur $L_1 \times \cdots \times L_n$.

Par hypothèse, les sous-groupes $\Delta_1, \ldots, \Delta_n$ de $\Gamma$ sont ouverts et le cor. 5 de V, p. 66, montre que les sous-extensions $L_1, \ldots, L_n$ de $K_s$ sont de degré fini sur $K$. Elles sont évidemment séparables. La dernière assertion du lemme 5 est immédiate.

Du lemme 5 et du th. 4 (V, p. 34), on déduit immédiatement le résultat suivant.

#### Proposition 12 {#alg-v-s10-prop-12 .statement}

Pour tout $\Gamma$-ensemble fini $X$, l’algèbre $\Theta(X)$ est étale sur $K$, de degré égal au cardinal de $X$. De plus, toute algèbre étale sur $K$ est isomorphe à une algèbre de la forme $\Theta(X)$.

#### Remarque 1 {#alg-v-s10-n6-rem-1 .statement}

On montre facilement que pour tout homomorphisme de $K$-algèbres $\varphi$ de $\Theta(X)$ dans $K_s$, il existe un unique élément $x$ de $X$ tel que $\varphi(f) = f(x)$ pour tout $f \in \Theta(X)$.

#### Remarque 2 {#alg-v-s10-n6-rem-2 .statement}

Soient $X$ et $Y$ deux $\Gamma$-ensembles finis. Soit $\mathfrak{F}_\Gamma(X, Y)$ l’ensemble des applications $u$ de $X$ dans $Y$ telles que $u(\sigma x) = \sigma u(x)$ pour tout $\sigma \in \Gamma$ et tout $x \in X$. Pour $u \in \mathfrak{F}_\Gamma(X, Y)$, on définit un homomorphisme de $K$-algèbres $u^*: \Theta(Y) \to \Theta(X)$ par $u^*(f) = f \circ u$. Pour tout homomorphisme $\Psi$ de $\Theta(Y)$ dans $\Theta(X)$, il existe un unique élément $u$ de $\mathfrak{F}_\Gamma(X, Y)$ tel que $\Psi = u^*$.

11. Structure des extensions quasi-galoisiennes

#### Proposition 13 {#alg-v-s10-prop-13 .statement}

Soit $N$ une extension quasi-galoisienne de $K$. On note $N_r$ le corps des invariants du groupe des $K$-automorphismes de $N$ et $N_s$ la fermeture algébrique séparable de $K$ dans $N$ (V, p. 42). Alors :
a) $N_r$ est la fermeture radicielle de $K$ dans $N$ (V, p. 24).
b) $N_s$ est une extension galoisienne de $K$ et tout $K$-automorphisme de $N_s$ se prolonge de manière unique en un $N_r$-automorphisme de $N$.
c) Les corps $N_r$ et $N_s$ sont linéairement disjoints sur $K$ et l’on a $N = K[N_r \cup N_s]$; autrement dit, l’homomorphisme canonique de $N_r \otimes_K N_s$ dans $N$ est un isomorphisme.

Soit $\Omega$ une clôture algébrique de $K$, contenant $N$ comme sous-extension (V, p. 22, th. 2). Tout $K$-automorphisme de $\Omega$ induit un automorphisme de $N$ puisque $N$ est quasi-galoisienne. Par suite, tout élément de $N_r$ est invariant par le groupe des $K$-automorphismes de $\Omega$, donc est radiciel sur $K$ (V, p. 51, cor. 3). Réciproquement, tout élément de $N$ radiciel sur $K$ est évidemment invariant par tout $K$-automorphisme de $N$, donc appartient à $N_r$. Ceci prouve a).

Tout $K$-automorphisme de $\Omega$ applique $N$ dans $N$, donc $N_s$ dans $N_s$, et $N_s$ est donc une extension quasi-galoisienne de $K$ (V, p. 52, prop. 3). Par suite, $N_s$ est une extension galoisienne de $K$. Tout élément de $N_r \cap N_s$ est algébrique séparable et radiciel sur $K$, donc appartient à $K$ (V, p. 38, cor. 3) ; on a donc $N_r \cap N_s = K$. Or $N$ est radiciel sur $N_s$ (V, p. 42, prop. 13) et algébrique séparable sur $N_r$ (V, p. 54, th. 1), donc à la fois radiciel et séparable sur $K(N_r \cup N_s)$. On a donc $N = K(N_r \cup N_s)$ (V, p. 38, cor. 3) et les assertions b) et c) résultent du th. 5 (V, p. 68).

#### Corollaire {#alg-v-s10-n6-cor-1 .statement}

Soient $p$ l’exposant caractéristique de $K$, $\overline{K}$ une clôture algébrique de $K$, $K_s$ la fermeture séparable de $K$ dans $\overline{K}$ et $K^{p^{-\infty}}$ la clôture parfaite de $K$. Alors l’homomorphisme canonique de $K^{p^{-\infty}} \otimes K_s$ dans $K$ est un isomorphisme.

#### Remarque {#alg-v-s10-n6-rem-5 .statement}

Soit $R$ (resp. $S$) une extension radicielle (resp. algébrique séparable) de $K$. Alors l’algèbre $R \otimes_K S$ est un corps : en effet, $R$ (resp. $S$) est isomorphe à une sous-extension de $K^{p^{-\infty}}$ (resp. $K_s$) et il suffit d’appliquer le cor. ci-dessus et la prop. 1 de V, p. 17.

## EXERCICES {#alg-v-s10-exercises}

See the [exercises for § 10](exercises/s10/).
