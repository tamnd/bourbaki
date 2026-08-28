---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 1
section_title: Bigèbre enveloppante d'une algèbre de Lie
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0005-0015, 0071-0073
extraction: ocr
subsections:
    - "no": 1
      title: Éléments primitifs d’une cogèbre
      page: 0
      pdf_page: 5
    - "no": 2
      title: Éléments primitifs d’une bigèbre
      page: 0
      pdf_page: 7
    - "no": 3
      title: Bigèbres filtrées
      page: 0
      pdf_page: 8
    - "no": 4
      title: Bigèbre enveloppante d’une algèbre de Lie
      page: 0
      pdf_page: 8
    - "no": 5
      title: Structure de la cogèbre $U(g)$ en caractéristique 0.
      page: 0
      pdf_page: 10
    - "no": 6
      title: Structure des bigèbres filtrées en caractéristique 0
      page: 0
      pdf_page: 13
statements: 24
exercises: 12
content_sha256: 22da2cbed45b4318678470dd7c4d3b005e983ff04abf7ebf7469adeb16a4c033
---

## § 1. Bigèbre enveloppante d’une algèbre de Lie

Dans tout ce paragraphe, on note $g$ une algèbre de Lie sur $\mathbf{K}$, $U(g)$ ou simplement $U$ son algèbre enveloppante (chap. I, § 2, n° 1), $\sigma$ l’application canonique de $g$ dans $U(g)$ (*loc. cit.*) et $(U_n)_{n \geq 0}$ la filtration canonique de $U$ (*loc. cit.*, n° 6).

### 1. Éléments primitifs d’une cogèbre

Dans tout ce n°, on considère une *cogèbre* $E$ (A, III, p. 138), de coproduit
$$
c : E \to E \otimes E
$$
possédant une *coïunité* $\varepsilon$ (*loc. cit.*, p. 146). Rappelons que $\varepsilon$ est une forme linéaire sur le $\mathbf{K}$-module $E$ telle que (après identification canonique de $E \otimes \mathbf{K}$ et $\mathbf{K} \otimes E$ avec $E$) l’on ait:
$$
\mathrm{Id}_E = (\varepsilon \otimes \mathrm{Id}_E) \circ c = (\mathrm{Id}_E \otimes \varepsilon) \circ c.
$$
On note $E^+$ le noyau de $\varepsilon$ et on se donne un élément $u$ de $E$ tel que
$$
c(u) = u \otimes u \quad \text{et} \quad \varepsilon(u) = 1.
$$
Le $\mathbf{K}$-module $E$ est somme directe de $E^+$ et du sous-module $\mathbf{K}.u$, qui est libre de base $u$; on note $\pi_u : E \to E^+$ et $\eta_u : E \to \mathbf{K}.u$ les projecteurs associés à cette décomposition. On a
(1)
$$
\pi_u(x) = x - \varepsilon(x).u, \qquad \eta_u(x) = \varepsilon(x).u.
$$

#### Définition 1 {#lie-ii-s1-def-1 .statement}

*On dit qu’un élément $x$ de $E$ est $u$-primitif si l’on a*
(2)
$$
c(x) = x \otimes u + u \otimes x.
$$
Les éléments $u$-primitifs de $E$ forment un sous-module de $E$, noté $P_u(E)$.

¹ Les résultats des chapitres II et III dépendent des six premiers Livres (E, A, TG, FVR, EVT, INT) de LIE I, de AC et de VAR, R ; le n° 9 du § 6 du chap. III dépend en outre de TS I.

#### Proposition 1 {#lie-ii-s1-prop-1 .statement}

Tout élément u-primitif de E appartient à E^+.

En effet, (2) entraîne $x = \varepsilon(x).u + \varepsilon(u).x = \varepsilon(x).u + x$, d’où $\varepsilon(x) = 0$.

#### Remarque {#lie-ii-s1-n1-rem-1 .statement}

Si $x \in E$ et si $c(x) = x' \otimes u + u \otimes x''$, où $x', x''$ sont dans $E^+$, alors $x = \varepsilon(x').u + \varepsilon(u).x'' = x''$; de même $x = x'$, et $x$ est u-primitif.

Pour tout $x \in E^+$, on pose

$$
c_u^+(x) = c(x) - x \otimes u - u \otimes x.
$$

#### Proposition 2 {#lie-ii-s1-prop-2 .statement}

On a

$$
(\pi_u \otimes \pi_u) \circ c = c_u^+ \circ \pi_u.
$$

En effet, soit $x$ dans $E$; on a

$$
\begin{align*}
(\pi_u \otimes \pi_u)(c(x)) &= ((1 - \eta_u) \otimes (1 - \eta_u))(c(x)) \\
&= c(x) - (1 \otimes \eta_u)(c(x)) - (\eta_u \otimes 1)(c(x)) + (\eta_u \otimes \eta_u)(c(x)).
\end{align*}
$$

Comme $\varepsilon$ est coïunité de $E$, on a

$$
(1 \otimes \eta_u)(c(x)) = x \otimes u, \quad (\eta_u \otimes 1)(c(x)) = u \otimes x
$$

d’où

$$
(\eta_u \otimes \eta_u)((c(x))) = (\eta_u \otimes 1)((1 \otimes \eta_u)(c(x))) = \varepsilon(x).u \otimes u;
$$

de tout ceci, on tire

$$
(\pi_u \otimes \pi_u)(c(x)) = c(x) - x \otimes u - u \otimes x + \varepsilon(x).u \otimes u.
$$

D’autre part, on a

$$
c_u^+(\pi_u(x)) = c(x) - x \otimes u - u \otimes x + \varepsilon(x).u \otimes u,
$$

d’où la formule (4).

Comme $E^+$ est un sous-module facteur direct de $E$, on peut identifier $E^+ \otimes E^+$ à un sous-module facteur direct de $E \otimes E$. Avec cette identification, $\pi_u \otimes \pi_u$ est un projecteur de $E \otimes E$ sur $E^+ \otimes E^+$. D’après la formule (4), $c_u^+$ applique $E^+$ dans $E^+ \otimes E^+$ et $\pi_u$ est un morphisme de la cogèbre $(E, c)$ dans la cogèbre $(E^+, c_u^+)$.

#### Proposition 3 {#lie-ii-s1-prop-3 .statement}

Si la cogèbre $(E, c)$ est coassociative (resp. cocommutative) (A, III, p. 143–144), il en est de même de la cogèbre $(E^+, c_u^+)$.

Cela résulte du lemme suivant:

#### Lemme 1 {#lie-ii-s1-lem-1 .statement}

Soit $\pi : E \to E'$ un morphisme surjectif de cogèbres. Si $E$ est coassociative (resp. cocommutative), il en est de même de $E'$.

Soit $B$ une $K$-algèbre associative; l’application $f \mapsto f \circ \pi$ est un homomorphisme injectif d’algèbres de $\mathrm{Hom}_K(E', B)$ dans $\mathrm{Hom}_K(E, B)$. Il suffit alors d’appliquer la prop. 1 (resp. la prop. 2) de A, III, p. 143 (resp. p. 144).

### 2. Éléments primitifs d’une bigèbre

Soient E une bigèbre (A, III, p. 148), c son coproduit, ε sa coïunité, 1 son élément unité. Comme ε(1) = 1 et c(1) = 1 ⊗ 1, on peut appliquer les résultats du n° précédent avec u = 1. On appelle simplement primitifs (cf. A, III, p. 164) les éléments 1-primitifs de E (n° 1, déf. 1), c’est-à-dire les éléments x de E tels que

$$
c(x) = x \otimes 1 + 1 \otimes x.
$$

On écrira simplement π, η, P(E), c⁺ au lieu de π₁, η₁, P₁(E), c₁⁺.

#### Proposition 4 {#lie-ii-s1-prop-4 .statement}

L’ensemble P(E) des éléments primitifs de E est une sous-algèbre de Lie de E.

Si x, y sont dans P(E), on a

$$
\begin{align*}
c(xy) &= c(x)c(y) = (x \otimes 1 + 1 \otimes x)(y \otimes 1 + 1 \otimes y) \\
&= xy \otimes 1 + 1 \otimes xy + x \otimes y + y \otimes x,
\end{align*}
$$

d’où

$$
c([x, y]) = [x, y] \otimes 1 + 1 \otimes [x, y].
$$

#### Proposition 5 {#lie-ii-s1-prop-5 .statement}

Soit f : E → E' un morphisme de bigèbres. Si x est un élément primitif de E, alors f(x) est un élément primitif de E', et la restriction de f à P(E) est un homomorphisme d’algèbres de Lie P(f) : P(E) → P(E').

Soit c (resp. c') le coproduit de E (resp. E'). Puisque f est un morphisme de cogèbres, on a c' ∘ f = (f ⊗ f) ∘ c, d’où

$$
c'(f(x)) = (f \otimes f)(c(x)) = (f \otimes f)(x \otimes 1 + 1 \otimes x) = f(x) \otimes 1 + 1 \otimes f(x),
$$

pour x primitif. Donc f applique P(E) dans P(E') et l’on a f([x, y]) = [f(x), f(y)] puisque f est un homomorphisme d’algèbres.

#### Remarque 1 {#lie-ii-s1-n2-rem-1 .statement}

Soit p un nombre premier tel que p . 1 = 0 dans K. La formule du binôme et les congruences $\binom{p}{i} \equiv 0 \pmod{p}$ pour $1 \leq i \leq p - 1$ entraînent que P(E) est stable par l’application $x \mapsto x^p$.

#### Remarque 2 {#lie-ii-s1-n2-rem-2 .statement}

Par définition, le diagramme

$$
0 \to P(E) \to E^+ \xrightarrow{c^+} E^+ \otimes E^+
$$

est une suite exacte. Si K' est un anneau commutatif et ρ : K → K' un homomorphisme d’anneaux, $\rho^*(E) = E \otimes_K K'$ est une K'-bigèbre et l’inclusion P(E) → E définit un homomorphisme de K'-algèbres de Lie

$$
\alpha : P(E) \otimes_K K' \to P(E \otimes_K K').
$$

$$
0 \to P(E) \otimes_K K' \to E^+ \otimes_K K' \xrightarrow{\varepsilon^+ \otimes_K \mathrm{Id}_{K'}} (E^+ \otimes_K K') \otimes_{K'} (E^+ \otimes_K K')
$$

est une suite exacte, ce qui entraîne que $\alpha$ est un isomorphisme.

### 3. Bigèbres filtrées

#### Définition 2 {#lie-ii-s1-def-2 .statement}

Soit E une bigèbre de coproduit c. On appelle filtration compatible avec la structure de bigèbre de E une suite croissante $(E_n)_{n \geq 0}$ de sous-modules de E telle que

$$
E_0 = K . 1, \quad E = \bigcup_{n \geq 0} E_n
$$
$$
E_m . E_n \subset E_{m+n} \quad \text{pour } m \geq 0, n \geq 0
$$
(6)
$$
c(E_n) \subset \sum_{i+j=n} \operatorname{Im}(E_i \otimes E_j) \quad \text{pour } n \geq 0.
$$
\footnote{1}

On appelle bigèbre filtrée une bigèbre munie d’une filtration compatible avec sa structure de bigèbre.

#### Exemple {#lie-ii-s1-n3-exa-1 .statement}

Soient E une bigèbre graduée (A, III, p. 148, déf. 3), $(E^n)_{n \geq 0}$ sa graduation. Posons $E_n = \sum_{i=0}^n E^i$. La suite $(E_n)$ est une filtration compatible avec la structure de bigèbre de E.

#### Proposition 6 {#lie-ii-s1-prop-6 .statement}

Soient E une bigèbre filtrée, $(E_n)_{n \geq 0}$ sa filtration. Pour tout entier $n \geq 0$, soit $E_n^+ = E_n \cap E^+$. Alors $E_0^+ = \{0\}$ et
(7)
$$
c^+(E_n^+) \subset \sum_{i=1}^{n-1} \operatorname{Im}(E_i^+ \otimes E_{n-i}^+) \quad \text{pour } n \geq 0.
$$
\footnote{1}

Comme $E_0 = K . 1$, on a $E_0^+ = 0$. Si $x \in E_n$, on a $\pi(x) = x - \varepsilon(x) . 1$ (formule (1)), d’où $\pi(x) \in E_n^+$ et $\pi(E_n) \subset E_n^+$. Il en résulte que $\pi \otimes \pi$ applique $\operatorname{Im}(E_i \otimes E_j)$ dans $\operatorname{Im}(E_i^+ \otimes E_j^+)$ pour $i \geq 0, j \geq 0$. Comme $c^+ = (\pi \otimes \pi) \circ c$ dans $E^+$ (n° 1, prop. 2), on a d’après (6)

$$
c^+(E_n^+) \subset \sum_{i=0}^n \operatorname{Im}(E_i^+ \otimes E_{n-i}^+) = \sum_{i=1}^{n-1} \operatorname{Im}(E_i^+ \otimes E_{n-i}^+).
$$

#### Corollaire {#lie-ii-s1-n3-cor-1 .statement}

Les éléments de $E_1^+$ sont primitifs.
Si $x \in E_1^+$, on a $c^+(x) = 0$ d’après (7), d’où (5).

### 4. Bigèbre enveloppante d’une algèbre de Lie

Rappelons que g désigne une algèbre de Lie, et U son algèbre enveloppante, munie de sa filtration canonique $(U_n)_{n \geq 0}$.

1 Si A et B sont deux sous-modules de E, on désigne par $\operatorname{Im}(A \otimes B)$ l’image de l’application canonique $A \otimes B \to E \otimes E$.

a) Soit $x \in g$; posons $c_0(x) = \sigma(x) \otimes 1 + 1 \otimes \sigma(x) \in U \otimes U$. Si $x, y$ sont dans $g$, on a $c_0(x)c_0(y) = (\sigma(x)\sigma(y)) \otimes 1 + 1 \otimes (\sigma(x)\sigma(y)) + \sigma(x) \otimes \sigma(y) + \sigma(y) \otimes \sigma(x)$, d’où

$$
[c_0(x), c_0(y)] = c_0([x, y]).
$$

D’après la propriété universelle de U (chap. I, § 2, n° 1, prop. 1), il existe un homomorphisme d’algèbres unifères, et un seul

$$
c : U \to U \otimes U
$$

tel que $c(\sigma(x)) = \sigma(x) \otimes 1 + 1 \otimes \sigma(x)$ pour $x \in g$. Cela démontre l’assertion d’unicité de la prop. 7.

b) Montrons que c est coassociatif. En effet, les applications linéaires $c'$ et $c''$ de U dans $U \otimes U \otimes U$ définies par

$$
c' = (c \otimes \mathrm{Id}_U) \circ c \quad \text{et} \quad c'' = (\mathrm{Id}_U \otimes c) \circ c
$$

sont des homomorphismes d’algèbres unifères qui coïncident dans $\sigma(g)$ car, pour $a \in \sigma(g)$, on a

$$
c'(a) = a \otimes 1 \otimes 1 + 1 \otimes a \otimes 1 + 1 \otimes 1 \otimes a = c''(a),
$$

d’où le résultat.

c) Montrons que c est cocommutatif. Soit $\tau$ l’automorphisme de $U \otimes U$ tel que $\tau(a \otimes b) = b \otimes a$ pour $a, b$ dans U. Les applications $\tau \circ c$ et $c$ de U dans $U \otimes U$ sont des homomorphismes d’algèbres unifères qui coïncident dans $\sigma(g)$, d’où le résultat.

d) Montrons que $\varepsilon$ est une coïunité pour c. En effet, les applications $(\mathrm{Id}_U \otimes \varepsilon) \circ c$ et $(\varepsilon \otimes \mathrm{Id}_U) \circ c$ de U dans U sont des homomorphismes d’algèbres unifères qui coïncident avec $\mathrm{Id}_U$ dans $\sigma(g)$.

e) On sait que $U_0 = K.1$, $U_n \subset U_{n+1}$, $U = \bigcup_{n \geq 0} U_n$ et $U_n \cdot U_m \subset U_{n+m}$ (chap. I, § 2, n° 6). Soient $a_1, \ldots, a_n$ dans $\sigma(g)$. On a

$$
c(a_1 \ldots a_n) = \prod_{i=1}^n c(a_i) = \prod_{i=1}^n (a_i \otimes 1 + 1 \otimes a_i)
$$
$$
= \sum_{i=0}^n \sum_{\alpha \in I(i)} (a_{\alpha(1)} \ldots a_{\alpha(i)}) \otimes (a_{\alpha(i+1)} \ldots a_{\alpha(n)}),
$$

où $I(i)$ désigne l’ensemble des permutations de $\{1, n\}$ croissantes dans chacun des intervalles $\{1, i\}$ et $\{i+1, n\}$. Comme $U_n$ est le K-module engendré par les produits d’au plus n éléments de $\sigma(g)$, la formule (8) entraîne que la filtration $(U_n)$ est compatible avec la structure de bigèbre de $(U, c)$.

#### Définition 3 {#lie-ii-s1-def-3 .statement}

*La bigèbre* $(U, c)$ *est appelée* bigèbre enveloppante *de l’algèbre de Lie* g.

#### Proposition 8 {#lie-ii-s1-prop-8 .statement}

*Soit* E *une bigèbre de coproduit noté* $c_E$ *et soit* h *un homomorphisme d’algèbres de Lie de* g *dans* P(E) *(n° 2, prop. 4)*. *L’homomorphisme d’algèbres unifères* $f : U \to E$ *tel que* $f(\sigma(x)) = h(x)$ *pour tout* $x \in g$ *est un morphisme de bigèbres*.

Montrons que $(f \otimes f) \circ c = c_E \circ f$. Ce sont là deux homomorphismes d’algèbres unifères de U dans $E \otimes E$, et pour $a \in \sigma(g)$, on a

$$
(f \otimes f)(c(a)) = f(a) \otimes 1 + 1 \otimes f(a) = c_E(f(a))
$$

puisque $f(a) \in P(E)$. De même, si $\varepsilon_E$ est la coïunité de E, $\varepsilon_E \circ f$ est un homomorphisme d’algèbres unifères $U \to K$ nul dans $\sigma(g)$ (n° 1, prop. 1) et coïncide donc avec $\varepsilon$.

Il résulte des propositions 5 et 8 que l’application $f \mapsto f \circ \sigma$ définit une correspondance biunivoque entre homomorphismes de bigèbres $U(g) \to E$ et homomorphismes d’algèbres de Lie $g \to P(E)$.

#### Corollaire {#lie-ii-s1-n4-cor-1 .statement}

*Soient* $g_i$ ($i = 1, 2$) *une algèbre de Lie*, $U(g_i)$ *sa bigèbre enveloppante*, $\sigma_i : g_i \to U(g_i)$ *l’application canonique*. *Pour tout homomorphisme d’algèbres de Lie* $h : g_1 \to g_2$, *l’homomorphisme d’algèbres unifères* $U(h) : U(g_1) \to U(g_2)$ *tel que* $U(h) \circ \sigma_1 = \sigma_2 \circ h$ *(chap. I, § 2, n° 1)* *est un morphisme de bigèbres*.

### 5. Structure de la cogèbre $U(g)$ en caractéristique 0.

Dans ce n°, on suppose que K est un *corps de caractéristique* 0.

Soient S(g) l’algèbre symétrique de l’espace vectoriel g, $c_S$ son coproduit (A, III, p. 139, *Exemple* 6), $\eta$ l’isomorphisme canonique de l’espace vectoriel S(g) sur l’espace vectoriel U (chap. I, § 2, n° 7). Rappelons que si $x_1, \ldots, x_n$ sont dans g, on a

$$
\eta(x_1 \ldots x_n) = \frac{1}{n!} \sum_{\tau \in S_n} \sigma(x_{\tau(1)}) \ldots \sigma(x_{\tau(n)}).
$$

En particulier, pour $x \in g$ et $n \geqslant 0$, on a

$$
\eta(x^n) = \sigma(x)^n.
$$

Remarquons, d’après A, III, p. 68, *Remarque* 3, que $\eta$ est l’unique application linéaire de S(g) dans U satisfaisant à la condition (10).

#### Proposition 9 {#lie-ii-s1-prop-9 .statement}

Pour tout entier $n \geqslant 0$, soit $U^n$ le sous-espace vectoriel de $U$ engendré par les $\sigma(x)^n$ pour $x \in g$.

a) La suite $(U^n)_{n \geqslant 0}$ est une graduation de l’espace vectoriel $U$ compatible avec sa structure de cogèbre.
Munissons $U$ de la graduation $(U^n)$.
b) L’application canonique $\eta : S(g) \to U$ est un isomorphisme de cogèbres graduées.
Soient $x \in g$ et $n \in \mathbf{N}$. On a
$$
c_S(x^n) = c_S(x)^n = (x \otimes 1 + 1 \otimes x)^n = \sum_{i=0}^n \binom{n}{i} x^i \otimes x^{n-i}
$$
puisque $c_S$ est un homomorphisme d’algèbres. De même, d’après (10),
$$
c(\eta(x^n)) = c(\sigma(x)^n) = c(\sigma(x))^n = (\sigma(x) \otimes 1 + 1 \otimes \sigma(x))^n
$$
$$
= \sum_{i=0}^n \binom{n}{i} \sigma(x)^i \otimes \sigma(x)^{n-i} = \sum_{i=0}^n \binom{n}{i} \eta(x^i) \otimes \eta(x^{n-i}),
$$
d’où
$$
(\eta \otimes \eta)(c_S(x^n)) = c(\eta(x^n)).
$$
Comme les $x^n$, pour $x \in g$ et $n \in \mathbf{N}$, engendrent l’espace vectoriel $S(g)$, on a $(\eta \otimes \eta) \circ c_S = c \circ \eta$, et $\eta$ est un isomorphisme de cogèbres.
Par ailleurs, la formule (10) montre que $\eta(S^n(g)) = U^n$, ce qui achève de démontrer a) et b) compte tenu de ce que la graduation de $S(g)$ est compatible avec sa structure de cogèbre.

La graduation $(U^n)_{n \geqslant 0}$ de $U$ est appelée graduation canonique.

#### Corollaire {#lie-ii-s1-n5-cor-1 .statement}

L’application canonique $\sigma$ définit un isomorphisme de $g$ sur l’algèbre de Lie $P(U)$ des éléments primitifs de $U$.
Comme $c^+$ est un homomorphisme gradué de degré 0, on a
$$
P(U) = \sum_{n \geqslant 1} (P(U) \cap U^n).
$$
Il suffit de prouver que si $n > 1$ et si $a \in U^n$ est primitif, alors $a = 0$. Or $a$ s’écrit $\sum_i \lambda_i a_i^n$, où $\lambda_i \in K$, $a_i \in \sigma(g)$. D’après (12), le terme de bidegré $(1, n-1)$ de $c^+(a)$ est $n \sum_i \lambda_i a_i \otimes a_i^{n-1}$. On a donc $\sum_i \lambda_i a_i \otimes a_i^{n-1} = 0$. Si $\mu : U \otimes U \to U$ est l’application linéaire définie par la multiplication de $U$, on a donc
$$
a = \sum_i \lambda_i a_i^n = \mu \left( \sum_i \lambda_i a_i \otimes a_i^{n-1} \right) = 0.
$$

#### Remarque 1 {#lie-ii-s1-n5-rem-1 .statement}

On a $U_n = \sum_{i=0}^n U^i$ (chap. I, § 2, no 7, cor. 4 du th. 1).
2) L’application $\eta$ est l’unique morphisme de cogèbres graduées de $S(g)$ dans $U$ tel que $\eta(1) = 1$ et $\eta(x) = \sigma(x)$ pour $x \in g$. En effet, si $\eta'$ est un morphisme satisfaisant à ces conditions, prouvons par récurrence sur $n$ que $\eta'(x^n) = \eta(x^n)$ pour $x \in \mathfrak{g}$ et $n > 1$. Comme $c_S^+(x^n) = \sum_{i=1}^{n-1} \binom{n}{i} x^i \otimes x^{n-i}$ d’après (3) et (11), on a $(\eta \otimes \eta)(c_S^+(x^n)) = (\eta' \otimes \eta')(c_S^+(x^n))$ par l’hypothèse de récurrence. Il s’ensuit que $c^+(\eta(x^n)) = c^+(\eta'(x^n))$; il en résulte que $\eta(x^n) - \eta'(x^n)$ est un élément primitif de degré $n$, donc est nul (cor. de la prop. 9).

3) Soit $\psi$ l’isomorphisme canonique de la bigèbre TS($\mathfrak{g}$) sur la bigèbre S($\mathfrak{g}$) (A, IV, § 5, cor. 1 de la prop. 12). L’application
$$
\eta \circ \psi : \mathrm{TS}(\mathfrak{g}) \to \mathbf{U}
$$
est dite *canonique*. C’est l’unique morphisme $\eta'$ de cogèbres graduées de TS($\mathfrak{g}$) dans $\mathbf{U}$ tel que $\eta'(1) = 1$ et $\eta'(x) = \sigma(x)$ pour tout $x \in \mathfrak{g}$.

4) Soit V un espace vectoriel. Les éléments primitifs de la bigèbre S(V) sont les éléments de degré 1. Cela résulte en effet du cor. de la prop. 9 appliqué à l’algèbre de Lie commutative V.

Soit $(e_i)_{i \in I}$ une base du K-espace vectoriel $\mathfrak{g}$, où l’ensemble d’indices I est muni d’un ordre total. Pour tout $\alpha \in \mathbf{N}^{(I)}$, on pose
$$
e_\alpha = \prod_{i \in I} \frac{\sigma(e_i)^{\alpha(i)}}{\alpha(i)!}.
$$
Les $e_\alpha$, pour $|\alpha| \leq n$, forment une base du K-espace vectoriel $U_n$ (chap. I, § 2, n° 7, cor. 3 du th. 1). On a
$$
e_0 = 1, \quad e_{e_i} = \sigma(e_i) \text{ pour } i \in I.
$$
Comme l’algèbre graduée associée à l’algèbre filtrée U est commutative (*loc. cit.*, th. 1), on a, pour $\alpha, \beta$ dans $\mathbf{N}^{(I)}$,
$$
e_\alpha \cdot e_\beta \equiv ((\alpha, \beta)) \cdot e_{\alpha + \beta} \mod U_{|\alpha| + |\beta| - 1},
$$
où $((\alpha, \beta)) = \prod_{i \in I} \frac{(\alpha(i) + \beta(i))!}{\alpha(i)! \beta(i)!}$.

D’autre part, on a aussitôt
$$
\varepsilon(e_0) = 1, \quad \varepsilon(e_\alpha) = 0 \quad \text{pour } |\alpha| \geq 1.
$$
Enfin, la formule (12) entraîne que, pour $\alpha \in \mathbf{N}^{(I)}$, on a
$$
c(e_\alpha) = \sum_{\beta + \gamma = \alpha} e_\beta \otimes e_\gamma.
$$
Cette formule permet de déterminer l’algèbre $U' = \mathrm{Hom}(U, K)$ *duale* de la cogèbre U (A, III, p. 143). Soit en effet $K[[X_i]]_{i \in I}$ l’algèbre des séries formelles par rapport à des indéterminées $(X_i)_{i \in I}$ (cf. A, III, p. 28); si $\lambda \in U'$, notons $f_\lambda$ la série formelle
$$
f_\lambda = \sum_\alpha \langle \lambda, e_\alpha \rangle X^\alpha, \quad \text{avec } X^\alpha = \prod_{i \in I} X_i^{\alpha(i)},
$$
l’indice de sommation $\alpha$ parcourant $\mathbf{N}^{(I)}$.

#### Proposition 10 {#lie-ii-s1-prop-10 .statement}

*L’application* $\lambda \mapsto f_\lambda$ *est un isomorphisme de l’algèbre* $U'$ *sur l’algèbre de séries formelles* $K[[X_i]]_{i \in I}$.
Du fait que $(e_\alpha)$ est une base de $U$, l’application $\lambda \mapsto f_\lambda$ est $K$-linéaire et bijective.
D’autre part, pour $\lambda, \mu$ dans $U'$, on a
$$
f_{\lambda \mu} = \sum_\alpha \langle \lambda \mu, e_\alpha \rangle X^\alpha = \sum_\alpha \langle \lambda \otimes \mu, c(e_\alpha) \rangle X^\alpha
$$
$$
= \sum_\alpha \langle \lambda \otimes \mu, \sum_{\beta + \gamma = \alpha} e_\beta \otimes e_\gamma \rangle X^\alpha \tag{d’après (16)}
$$
$$
= \sum_{\beta, \gamma} \langle \lambda, e_\beta \rangle \langle \mu, e_\gamma \rangle X^{\beta + \gamma} = f_\lambda f_\mu,
$$
ce qui montre que $\lambda \mapsto f_\lambda$ est un isomorphisme *d’algèbres*, et achève la démonstration.

### 6. Structure des bigèbres filtrées en caractéristique 0

Dans ce n°, on continue de supposer que $K$ est un *corps de caractéristique 0*.
Si $E$ est une bigèbre, l’injection canonique $P(E) \to E$ se prolonge en un morphisme de bigèbres $f_E : U(P(E)) \to E$ (n° 4, prop. 8).

#### Théorème 1 {#lie-ii-s1-thm-1 .statement}

*Soit* $E$ *une bigèbre cocommutative*.
a) *Le morphisme de bigèbres* $f_E : U(P(E)) \to E$ *est injectif*.
b) *S’il existe sur* $E$ *une filtration compatible avec sa structure de bigèbre* (n° 3, déf. 2), *le morphisme* $f_E$ *est un isomorphisme*.
(Dans le cas b), la bigèbre $E$ s’identifie donc à la bigèbre enveloppante de l’algèbre de Lie de ses éléments primitifs.)
Soit $c_E$ (resp. $\varepsilon_E$) le coproduit (resp. la coïunité) de $E$. Posons $g = P(E)$; soit $(e_i)_{i \in I}$ une base du $K$-espace vectoriel $g$, où l’ensemble d’indices $I$ est muni d’un ordre total, et soit $(e_\alpha)_{\alpha \in N^{(I)}}$ la base de $U(g)$ introduite au n° précédent. Posons $X_\alpha = f_E(e_\alpha)$ pour $\alpha \in N^{(I)}$. D’après (15) et (16), on a:
$$
\varepsilon_E(X_0) = 1, \quad \varepsilon_E(X_\alpha) = 0 \quad \text{pour } |\alpha| \geq 1, \tag{17}
$$
$$
c_E(X_\alpha) = \sum_{\beta + \gamma = \alpha} X_\beta \otimes X_\gamma \quad \text{pour } \alpha \in N^{(I)}, \tag{18}
$$
puisque $f_E$ est un morphisme de cogèbres.
*Montrons que* $f_E$ *est injectif*. Cela résulte du lemme suivant:

#### Lemme 2 {#lie-ii-s1-lem-2 .statement}

*Soit* $V$ *un espace vectoriel*, *et soient* $E$ *une cogèbre*, $f : S(V) \to E$ *un morphisme de cogèbres*. *Si la restriction de* $f$ *à* $S^0(V) + S^1(V)$ *est injective, alors* $f$ *est injectif*.
Soit $n \geq 0$; posons $S_n = \sum_{i \leq n} S^i(V)$, notons $c_S$ le coproduit de $S(V)$, et montrons par récurrence sur $n$ que $f|_{S_n}$ est injectif. L’assertion étant triviale pour $n = 0$ et $n = 1$, supposons $n \geq 2$ et soit $u \in S_n$ tel que $f(u) = 0$. On a

$$
0 = c_E(f(u)) = (f \otimes f)(c_S(u))
= f(u) \otimes 1 + 1 \otimes f(u) + (f \otimes f)(c_S^+(u))
= (f \otimes f)(c_S^+(u)).
$$

Comme $c_S^+(u) \in S_{n-1} \otimes S_{n-1}$, d’après (11) l’hypothèse de récurrence montre que $u$ est un élément primitif de $S(V)$, donc est de degré 1 (n° 5, Remarque 4), donc nul, puisque $f | S^1(V)$ est injectif.

Il en résulte en particulier que la famille $(X_\alpha)$ est libre.

Montrons que $f_E$ est surjectif si $E$ possède une filtration compatible avec sa structure de bigèbre. Soit $(E_n)_{n \geq 0}$ une telle filtration, et posons $E_n^+ = E_n \cap \mathrm{Ker}(\varepsilon_E)$. Démontrons par récurrence sur $n$ que $E_n^+$ est contenu dans l’image de $f_E$. Comme $E = K.1 + \bigcup_{n \geq 0} E_n^+$, cela entraînera la surjectivité de $f_E$. L’assertion est triviale pour $n = 0$, et résulte du cor. de la prop. 6 du n° 3 pour $n = 1$; supposons désormais $n \geq 2$, et soit $x \in E_n^+$. D’après la prop. 6 du n° 3, on a

$$
c_E^+(x) \in \sum_{i=1}^{n-1} E_i^+ \otimes E_{n-i}^+
$$

et il existe d’après l’hypothèse de récurrence des scalaires $\lambda_{\alpha,\beta}$, pour $\alpha, \beta$ dans $\mathbf{N}^{(I)}$, nuls sauf un nombre fini d’entre eux, tels que

$$(19)$$
$$
c_E^+(x) = \sum_{\alpha, \beta \neq 0} \lambda_{\alpha,\beta} X_\alpha \otimes X_\beta.
$$

D’après la formule (18), on a donc

$$
(c_E^+ \otimes \mathrm{Id}_E)(c_E^+(x)) = \sum_{\alpha, \beta, \gamma \neq 0} \lambda_{\alpha+\beta, \gamma} X_\alpha \otimes X_\beta \otimes X_\gamma
$$
$$
(\mathrm{Id}_E \otimes c_E^+)(c_E^+(x)) = \sum_{\alpha, \beta, \gamma \neq 0} \lambda_{\alpha, \beta+\gamma} X_\alpha \otimes X_\beta \otimes X_\gamma.
$$

D’après la prop. 3 du n° 1, et l’indépendance linéaire des $X_\alpha$, on a donc

$$(20)$$
$$
\lambda_{\alpha+\beta, \gamma} = \lambda_{\alpha, \beta+\gamma} \quad \text{pour } \alpha, \beta, \gamma \text{ dans } \mathbf{N}^{(I)} - \{0\}.
$$

Par ailleurs, le coproduit $c_E$ est cocommutatif; le même raisonnement que ci-dessus entraîne

$$(21)$$
$$
\lambda_{\alpha, \beta} = \lambda_{\beta, \alpha} \quad \text{pour } \alpha, \beta \text{ dans } \mathbf{N}^{(I)} - \{0\}.
$$

Supposons qu’il existe une famille de scalaires $(\mu_\alpha)$ pour $|\alpha| \geq 2$, telle que

$$(22)$$
$$
\mu_{\alpha+\beta} = \lambda_{\alpha, \beta} \quad \text{pour } \alpha, \beta \text{ dans } \mathbf{N}^{(I)} - \{0\}.
$$

On a alors

$$
c_E^+(x) = \sum_{\alpha, \beta \neq 0} \mu_{\alpha+\beta} X_\alpha \otimes X_\beta = \sum_{|\gamma| \geq 2} \mu_\gamma c_E^+(X_\gamma),
$$

d’après la formule (18), donc $y = x - \sum_{|\gamma| \geq 2} \mu_\gamma X_\gamma$ est primitif, donc appartient à $P(E) \subset \mathrm{Im}(f_E)$. On a donc

$$
x = y + \sum_{|\gamma| \geq 2} \mu_\gamma f_E(e_\gamma) \in \operatorname{Im}(f_E).
$$

La démonstration sera donc achevée lorsque nous aurons démontré le lemme suivant:

#### Lemme 3 {#lie-ii-s1-lem-3 .statement}

*Si une famille de scalaires* $(\lambda_{\alpha,\beta})$ *de support fini* (pour $\alpha, \beta$ dans $\mathbf{N}^{(1)} - \{0\}$) *satisfait aux relations* (20) *et* (21), *il existe une famille* $(\mu_\alpha)_{|\alpha| \geq 2}$ *de support fini telle que* $\mu_{\alpha+\beta} = \lambda_{\alpha,\beta}$ *pour* $\alpha, \beta$ *non nuls*.

Il suffit de prouver que

(23)
$$
\alpha + \beta = \gamma + \delta
$$
entraîne $\lambda_{\alpha,\beta} = \lambda_{\gamma,\delta}$ pour $\alpha, \beta, \gamma, \delta$ non nuls. D’après le lemme de décomposition de Riesz (A, VI, § 1, n° 10, th. 1), il existe $\pi, \rho, \sigma$ et $\tau$ dans $\mathbf{N}^{(1)}$ tels que
$$
\alpha = \pi + \sigma, \quad \beta = \rho + \tau, \quad \gamma = \pi + \rho, \quad \delta = \sigma + \tau.
$$
Supposons $\pi \neq 0$; comme on a $\sigma + \beta = \rho + \delta$, la relation (20) entraîne
$$
\lambda_{\alpha,\beta} = \lambda_{\pi+\sigma,\beta} = \lambda_{\pi,\sigma+\beta} = \lambda_{\pi,\rho+\delta} = \lambda_{\pi+\rho,\delta} = \lambda_{\gamma,\delta}.
$$
Si par contre on a $\pi = 0$, on a $\beta = \gamma + \tau$ et $\delta = \alpha + \tau$, d’où
$$
\lambda_{\alpha,\beta} = \lambda_{\alpha,\gamma+\tau} = \lambda_{\alpha+\tau,\gamma} = \lambda_{\delta,\gamma}
$$
d’après (20), mais on a aussi $\lambda_{\delta,\gamma} = \lambda_{\gamma,\delta}$ d’après (21), d’où $\lambda_{\alpha,\beta} = \lambda_{\gamma,\delta}$.

## EXERCICES {#lie-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
