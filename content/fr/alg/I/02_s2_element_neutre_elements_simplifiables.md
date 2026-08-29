---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 2
section_title: Élément neutre ; éléments simplifiables ; éléments inversibles
lang: fr
source: alg-i-iii-fr
book_pages: A I.12-A I.23, A I.119-A I.122
pdf_pages: 0022-0033, 0129-0132
extraction: ocr
subsections:
    - "no": 1
      title: Élément neutre
      page: 12
      pdf_page: 22
    - "no": 2
      title: Eléments simplifiables
      page: 14
      pdf_page: 24
    - "no": 3
      title: Eléments inversibles
      page: 15
      pdf_page: 25
    - "no": 4
      title: Monoïde des fractions d’un monoïde commutatif
      page: 17
      pdf_page: 27
    - "no": 5
      title: 'Applications : I. Entiers rationnels'
      page: 20
      pdf_page: 30
    - "no": 6
      title: 'Applications: II. Multiplication des entiers rationnels'
      page: 21
      pdf_page: 31
    - "no": 7
      title: 'Applications: III. Puissances généralisées'
      page: 22
      pdf_page: 32
    - "no": 8
      title: Notations
      page: 23
      pdf_page: 33
statements: 30
exercises: 17
content_sha256: 7f909885aa65ab7cf5e7e291cf91c1df75f83a7a5ec37dbb397e4a2ae5063959
---

## § 2. ÉLÉMENT NEUTRE; ÉLÉMENTS SIMPLIFIABLES; ÉLÉMENTS INVERSIBLES

### 1. Élément neutre

#### Définition 1 {#alg-i-s2-def-1 .statement}

*Pour une loi de composition $\top$ sur un ensemble $E$, un élément $e$ de $E$ est dit élément neutre si, pour tout $x \in E$, on a $e \top x = x \top e = x$.*

Il existe au plus un élément neutre pour une loi donnée $\top$, car si $e$ et $e'$ sont éléments neutres, on a $e = e \top e' = e'$. Un élément neutre est permutable avec tout élément : c’est un élément central.

#### Définition 2 {#alg-i-s2-def-2 .statement}

*On appelle magma unifère un magma qui possède un élément neutre. Si $E, E'$ sont des magmas unifères, on appelle homomorphisme (ou morphisme) unifère de $E$ dans $E'$ un homomorphisme du magma $E$ dans le magma $E'$ qui transforme l’élément neutre de $E$ en l’élément neutre de $E'$. On appelle monoïde un magma unifère associatif.*

Si $E, E'$ sont des monoïdes, on appelle *homomorphisme de monoïdes* ou *morphisme de monoïdes* de $E$ dans $E'$ un morphisme *unifère* de $E$ dans $E'$.

#### Exemple 1 {#alg-i-s2-n1-exa-1 .statement}

Dans l’ensemble $\mathbf{N}$ des entiers naturels, 0 est élément neutre pour l’addition et 1 est élément neutre pour la multiplication. Chacune de ces deux lois munit $\mathbf{N}$ d’une structure de monoïde commutatif (E, III, p. 27).

#### Exemple 2 {#alg-i-s2-n1-exa-2 .statement}

Dans l’ensemble des parties d’un ensemble $E$, $\varnothing$ est élément neutre pour la loi $\cup$, $E$ pour la loi $\cap$. Plus généralement, dans un ensemble ordonné réticulé, le plus petit élément, s’il existe, est élément neutre pour la loi sup ; réciproquement, s’il existe un élément neutre pour cette loi, il est le plus petit élément de l’ensemble. De même pour le plus grand élément et la loi inf.

#### Exemple 3 {#alg-i-s2-n1-exa-3 .statement}

L’ensemble $\mathbf{N}$ ne possède pas d’élément neutre pour la loi $(x, y) \mapsto x^y$. Pour la loi $(X, Y) \mapsto X \circ Y$ entre parties de $E \times E$, la diagonale $\Delta$ est l’élément neutre. Pour la loi $(f, g) \mapsto f \circ g$ entre applications de $E$ dans $E$, l’application identique de $E$ est l’élément neutre.

#### Exemple 4 {#alg-i-s2-n1-exa-4 .statement}

Soient E un magma et R une relation d’équivalence sur E, compatible avec la loi de E (I, p. 11). Si e est élément neutre de E, l’image canonique de e dans E/R est élément neutre du magma E/R.

L’application identique d’un magma unifère est un homomorphisme unifère; le composé de deux homomorphismes unifères en est un. Pour qu’une application soit un isomorphisme de magmas unifères, il faut et il suffit que ce soit un homomorphisme unifère bijectif et l’application réciproque est alors un homomorphisme unifère. Soient E et E' des magmas unifères, e' l’élément neutre de E'; l’application constante de E dans E' appliquant E en e' est un homomorphisme unifère, appelé homomorphisme trivial.

Le produit d’une famille de magmas unifères (resp. de monoïdes) est un magma unifère (resp. un monoïde).

Tout magma quotient d’un magma unifère (resp. d’un monoïde) est un magma unifère (resp. un monoïde).

Soient E un magma unifère, e son élément neutre. On appelle sous-magma unifère de E un sous-magma A de E tel que $e \in A$. Il est clair que e est élément neutre du magma A. Toute intersection de sous-magmas unifères de E est un sous-magma unifère de E. Si X est une partie de E, il existe donc un plus petit sous-magma unifère de E contenant X; on l’appelle le sous-magma unifère de E engendré par X; il est égal à \{e\} si X est vide. Si E est un monoïde, on appelle sous-monoïde de E un sous-magma unifère de E.

Si F est un magma sans élément neutre, un sous-magma de F peut posséder un élément neutre. Par exemple, si F est associatif et si h est un élément idempotent de F (I, p. 7), l’ensemble des $h \mathbin{\top} x \mathbin{\top} h$, où x parcourt F est un sous-magma de F admettant h pour élément neutre.

Si E est un magma d’élément neutre e, il peut se faire qu’un sous-magma A de E tel que $e \notin A$ possède un élément neutre.

#### Définition 3 {#alg-i-s2-def-3 .statement}

Soit E un magma unifère. On appelle composé de la famille vide d’éléments de E l’élément neutre de E.

Si $(x_\alpha)_{\alpha \in \varnothing}$ est la famille vide d’éléments de E, son composé e se note encore $\prod_{\alpha \in \varnothing} x_\alpha$. Par exemple, on écrit

$$
\prod_{q \leq i \leq p} x_i = e
$$

lorsque $p < q$ ($p, q \in \mathbf{N}$). On pose de même $^0 \mathbin{\top} x = e$ quel que soit x. Avec ces définitions, les théorèmes 1 (I, p. 4) et 3 (I, p. 9) du § 1 restent vrais dans un magma unifère, si on y supprime l’hypothèse que les ensembles A et B_i sont non vides. De même, les formules $^{m+n} \mathbin{\top} x = (^m \mathbin{\top} x) \mathbin{\top} (^n \mathbin{\top} x)$ et $^{mn} \mathbin{\top} x = ^m \mathbin{\top} (^n \mathbin{\top} x)$ sont vraies alors pour $m \geq 0, n \geq 0$.

Soient E un magma unifère dont la loi est notée $\mathbin{\top}$ et e son élément neutre. On appelle support d’une famille $(x_i)_{i \in I}$ d’éléments de E l’ensemble des indices i ∈ I tels que $x_i \neq e$. Soit $(x_i)_{i \in I}$ une famille à support fini d’éléments de E. Nous allons définir le composé $\prod_{i \in I} x_i$ dans les deux cas suivants:

a) l’ensemble I est totalement ordonné;
b) E est associatif et les $x_i$ sont permutables deux à deux.

Dans ces deux cas, soit S le support de la famille $(x_i)$. Si J est une partie finie de I contenant S, on a $\prod_{i \in J} x_i = \prod_{i \in S} x_i$, comme on le voit par récurrence sur le nombre d’éléments de J, en appliquant le th. 1 (I, p. 4) dans le cas a) et le th. 3 (I, p. 9) dans le cas b). On note $\prod_{i \in I} x_i$ la valeur commune des composés $\prod_{i \in J} x_i$ pour toutes les parties finies de I contenant S. Lorsque I est l’intervalle $[p, \rightarrow)$ de $\mathbf{N}$, on écrit aussi $\prod_{i = p}^{\infty} x_i$.

Avec ces définitions et notations, les théorèmes 1 (I, p. 4) et 3 (I, p. 9) du § 1 et les remarques qui suivent le th. 3 (I, p. 9 et p. 10) s’étendent aux familles à support fini.

L’élément neutre, pour une loi notée additivement, se note souvent 0 et s’appelle zéro ou élément nul (ou parfois origine). Pour une loi notée multiplicativement, il se note souvent 1 et s’appelle élément unité (ou unité).

### 2. Eléments simplifiables

#### Définition 4 {#alg-i-s2-def-4 .statement}

Etant donnée une loi de composition $\top$ sur un ensemble E, on appelle translation à gauche (resp. translation à droite) par un élément $a \in E$, l’application $x \mapsto a \top x$ (resp. $x \mapsto x \top a$) de E dans lui-même.

Par passage à la loi opposée, les translations à gauche deviennent translations à droite et réciproquement.

On note éventuellement $\gamma_a$, $\delta_a$ (ou $\gamma(a)$, $\delta(a)$) les translations à gauche et à droite par $a \in E$; on a

$$
\gamma_a(x) = a \top x, \qquad \delta_a(x) = x \top a.
$$

#### Proposition 1 {#alg-i-s2-prop-1 .statement}

Si la loi $\top$ est associative, on a, pour $x \in E$ et $y \in E$,

$$
\gamma_{x \top y} = \gamma_x \circ \gamma_y, \qquad \delta_{x \top y} = \delta_y \circ \delta_x.
$$

En effet, pour tout $z \in E$, on a:

$$
\begin{align*}
\gamma_{x \top y}(z) &= (x \top y) \top z = x \top (y \top z) = \gamma_x(\gamma_y(z)) \\
\delta_{x \top y}(z) &= z \top (x \top y) = (z \top x) \top y = \delta_y(\delta_x(z)).
\end{align*}
$$

Autrement dit, l’application $x \mapsto \gamma_x$ est un homomorphisme du magma E dans l’ensemble $E^E$ des applications de E dans lui-même, muni de la loi $(f, g) \mapsto f \circ g$; l’application $x \mapsto \delta_x$ est un homomorphisme de E dans l’ensemble $E^E$ muni de la loi opposée. Si E est un monoïde, ces homomorphismes sont unifères.

#### Définition 5 {#alg-i-s2-def-5 .statement}

Un élément $a$ d’un magma $E$ est dit simplifiable (ou régulier) à gauche (resp. à droite) si la translation à gauche (resp. à droite) par $a$ est injective. Un élément simplifiable à gauche et à droite est appelé élément simplifiable (ou régulier).

Autrement dit, pour que $a$ soit simplifiable pour la loi $\tau$, il faut et il suffit que chacune des relations $a \tau x = a \tau y, x \tau a = y \tau a$, entraîne $x = y$ (on dit qu’on peut « simplifier par $a$ » ces égalités). S’il existe un élément neutre $e$ pour la loi $\tau$, il est simplifiable pour cette loi : les translations $\gamma_e$ et $\delta_e$ sont alors l’application identique de $E$ sur lui-même.

#### Exemple 1 {#alg-i-s2-n2-exa-1 .statement}

Tout entier naturel est simplifiable pour l’addition ; tout entier naturel $\neq 0$ est simplifiable pour la multiplication.
2) Dans un ensemble ordonné réticulé, il ne peut y avoir d’autre élément simplifiable pour la loi sup que l’élément neutre (plus petit élément) s’il existe ; de même pour inf. En particulier, dans l’ensemble des parties d’un ensemble $E$, $\varnothing$ est le seul élément simplifiable pour la loi $\cup$, $E$ le seul élément simplifiable pour la loi $\cap$.

#### Proposition 2 {#alg-i-s2-prop-2 .statement}

L’ensemble des éléments simplifiables (resp. simplifiables à gauche, resp. simplifiables à droite) d’un magma associatif est un sous-magma.

En effet, si $\gamma_x$ et $\gamma_y$ sont injectives, il en est de même de $\gamma_{x \tau y} = \gamma_x \circ \gamma_y$ (I, p. 14, prop. 1). De même pour $\delta_{x \tau y}$.

### 3. Eléments inversibles

#### Définition 6 {#alg-i-s2-def-6 .statement}

Soient $E$ un magma unifère, $\tau$ sa loi de composition, $e$ son élément neutre, $x$ et $x'$ deux éléments de $E$. On dit que $x'$ est inverse à gauche (resp. inverse à droite, resp. inverse) de $x$ si l’on a $x' \tau x = e$ (resp. $x \tau x' = e$, resp. $x' \tau x = x \tau x' = e$).

On dit qu’un élément $x$ de $E$ est inversible à gauche (resp. inversible à droite, resp. inversible) s’il possède un inverse à gauche (resp. inverse à droite, resp. inverse).

Un monoïde dont tous les éléments sont inversibles s’appelle un groupe.

On dit parfois symétrique et symétrisable au lieu d’inverse et inversible. Lorsque la loi de $E$ est notée additivement, on dit généralement opposé au lieu d’inverse.

#### Exemple 1 {#alg-i-s2-n3-exa-1 .statement}

Un élément neutre est son propre inverse.
2) Dans l’ensemble des applications de $E$ dans $E$, un élément $f$ est inversible à gauche (resp. inversible à droite) si $f$ est une injection (resp. surjection). Les inverses à gauche (resp. inverses à droite) sont alors les rétractions (resp. sections) associées à $f$ (E, II, p. 18, déf. 11). Pour que $f$ soit inversible, il faut et il suffit que $f$ soit une bijection. Son unique inverse est alors la bijection réciproque de $f$.

Soient $E$ et $F$ deux magmas unifères, et $f$ un homomorphisme unifère de $E$ dans $F$. Si $x'$ est inverse de $x$ dans $E$, $f(x')$ est inverse de $f(x)$ dans $F$. Par suite, si $x$ est un élément inversible de $E$, $f(x)$ est un élément inversible de $F$.

En particulier, si $R$ est une relation d’équivalence compatible avec la loi d’un magma unifère E, l’image canonique dans E/R d’un élément inversible de E est inversible.

#### Proposition 3 {#alg-i-s2-prop-3 .statement}

Soient E un monoïde et x un élément de E.

(i) Pour que x soit inversible à gauche (resp. à droite), il faut et il suffit que la translation à droite (resp. à gauche) par x soit surjective.

(ii) Pour que x soit inversible, il faut et il suffit qu’il soit inversible à gauche et inversible à droite. Dans ce cas, x possède un unique inverse, qui est aussi son unique inverse à gauche (resp. à droite).

Si x' est un inverse à gauche de x, on a (I, p. 14, prop. 1)
$$
\delta_x \circ \delta_{x'} = \delta_{x' \top x} = \delta_e = \mathrm{Id}_E
$$
et $\delta_x$ est surjective. Réciproquement, si $\delta_x$ est surjective, il existe un élément $x'$ de E tel que $\delta_x(x') = e$ et $x'$ est inverse à gauche de $x$. On démontre de même l’autre assertion de (i).

Si $x'$ (resp. $x''$) est un inverse à gauche (resp. à droite) de $x$, on a
$$
x' = x' \top e = x' \top (x \top x'') = (x' \top x) \top x'' = e \top x'' = x''
$$
d’où (ii).

#### Remarque {#alg-i-s2-n3-rem-1 .statement}

Soient E un monoïde et x un élément de E. Si x est inversible à gauche, il est simplifiable à gauche; en effet, si $x'$ est un inverse à gauche de $x$, on a
$$
\gamma_{x'} \circ \gamma_x = \gamma_{x' \top x} = \gamma_e = \mathrm{Id}_E
$$
et $\gamma_x$ est injective. En particulier, si $x$ est inversible, les translations à gauche et à droite par $x$ sont bijectives. Réciproquement, supposons $\gamma_x$ bijective; il existe $x' \in E$ tel que $xx' = \gamma_x(x') = e$; on a $\gamma_x(x'x) = (xx')x = x = \gamma_x(e)$, donc $x'x = e$, de sorte que $x$ est inversible. On voit de même que si $\delta_x$ est bijective, $x$ est inversible.

#### Proposition 4 {#alg-i-s2-prop-4 .statement}

Soient E un monoïde, x et y deux éléments inversibles de E, d’inverses $x'$ et $y'$ respectivement. Alors $y' \top x'$ est inverse de $x \top y$.

Cela résulte de la relation $(y' \top x') \top (x \top y) = y' \top (x' \top x) \top y = y' \top y = e$, et du calcul analogue pour $(x \top y) \top (y' \top x')$.

#### Corollaire 1 {#alg-i-s2-prop-4-cor-1 .statement}

Soit E un monoïde; si chacun des éléments $x_\alpha$ d’une séquence $(x_\alpha)_{\alpha \in A}$ d’éléments de E a un inverse $x'_\alpha$, le composé $\prod_{\alpha \in A} x_\alpha$ a pour inverse $\prod_{\alpha \in A'} x'_\alpha$, où $A'$ est l’ensemble totalement ordonné déduit de A en remplaçant l’ordre de A par l’ordre opposé.

On déduit ce corollaire de la prop. 4 en raisonnant par récurrence sur le nombre d’éléments de A.

En particulier, si $x$ et $x'$ sont inverses, $\top^n x$ et $\top^n x'$ sont inverses, pour tout entier $n \geqslant 0$.

#### Corollaire 2 {#alg-i-s2-prop-4-cor-2 .statement}

Dans un monoïde, l’ensemble des éléments inversibles est stable.

#### Proposition 5 {#alg-i-s2-prop-5 .statement}

Si, dans un monoïde, x et x' sont inverses, et si x commute avec y, alors x' commute avec y.

En effet, de $x \top y = y \top x$, on tire $x' \top (x \top y) \top x' = x' \top (y \top x) \top x'$ puis $(x' \top x) \top (y \top x') = (x' \top y) \top (x \top x')$, c’est-à-dire $y \top x' = x' \top y$.

#### Corollaire 1 {#alg-i-s2-prop-5-cor-1 .statement}

Soient E un monoïde, X une partie de E et X' le commutant de X. L’inverse de tout élément inversible de X' appartient à X'.

#### Corollaire 2 {#alg-i-s2-prop-5-cor-2 .statement}

Dans un monoïde, l’inverse d’un élément central inversible est un élément central.

### 4. Monoïde des fractions d’un monoïde commutatif

Dans ce n°, on notera e l’élément neutre d’un monoïde E, et $x^*$ l’inverse d’un élément inversible x de E.

Soient E un monoïde *commutatif*, S une partie de E et S' le sous-monoïde de E engendré par S.

#### Lemme 1 {#alg-i-s2-lem-1 .statement}

Dans $E \times S'$, la relation $R \mathbin{\mathcal{R}} x, y$ que voici:
« il existe a, b dans E et p, q, s dans S' tels que $x = (a, p), y = (b, q)$, et $aqs = bps$ » est une relation d’équivalence compatible avec la loi du monoïde produit $E \times S'$.

Il est immédiat que R est réflexive et symétrique. Soient $x = (a, p), y = (b, q)$ et $z = (c, r)$ des éléments de $E \times S'$ tels que l’on ait $R \mathbin{\mathcal{R}} x, y$ et $R \mathbin{\mathcal{R}} y, z$. Il existe donc deux éléments s et t de S' tels que
$$
aqs = bps, \qquad brt = cqt,
$$
d’où l’on déduit
$$
ar(stq) = bpsrt = cp(stq)
$$
donc $R \mathbin{\mathcal{R}} x, z$, car stq appartient à S'. La relation R est donc transitive.

Soient par ailleurs $x = (a, p), y = (b, q), x' = (a', p')$ et $y' = (b', q')$ des éléments de $E \times S'$ tels que l’on ait $R \mathbin{\mathcal{R}} x, y$ et $R \mathbin{\mathcal{R}} x', y'$. Il existe s et s' dans S' tels que
$$
aqs = bps, \qquad a'q's' = b'p's'
$$
d’où l’on déduit $(aa')(qq')(ss') = (bb')(pp')(ss')$, donc $R \mathbin{\mathcal{R}} xx', yy'$ car ss' $\in S'$. La relation d’équivalence R est donc compatible avec la loi de composition de $E \times S'$.

Le magma quotient $(E \times S')/R$ est un monoïde commutatif.

#### Définition 7 {#alg-i-s2-def-7 .statement}

Soient E un monoïde commutatif, S une partie de E et S' le sous-monoïde de E engendré par S. On note $E_S$ et l’on appelle monoïde des fractions¹ de E associé à S (ou à dénominateurs dans S) le monoïde quotient $(E \times S')/R$, où la relation d’équivalence R est décrite comme dans le lemme 1.

Pour $a \in E$ et $b \in S'$, la classe de $(a, p)$ modulo R se note en général $a/p$ et

¹ On dit aussi monoïde des différences si la loi de E est notée additivement.

s’appelle la fraction de numératuer $a$ et dénominateur $p$. On a donc par définition $(a/p).(a'/p') = aa'/pp'$. Les fractions $a/p$ et $a'/p'$ sont égales si et seulement s’il existe $s$ dans $S'$ avec $spa' = sp'a$; s’il en est ainsi, il existe $\sigma$ et $\sigma'$ dans $S'$ avec $a\sigma = a'\sigma'$ et $p\sigma = p'\sigma'$. En particulier, on a $a/p = sa/sp$ pour $a \in A$ et $s, p$ dans $S'$. L’élément neutre de $E_S$ est la fraction $e/e$.

On posera $a/e = \varepsilon(a)$ pour tout $a \in E$. Ce qui précède montre que $\varepsilon$ est un homomorphisme de $E$ dans $E_S$, dit canonique. Pour tout $p \in S'$, on a $(p/e).(e/p) = e/e$, donc $e/p$ est inverse de $\varepsilon(p) = p/e$; tout élément de $\varepsilon(S')$ est donc inversible. On a $a/p = (\varepsilon(a)(e/p))$, d’où

$$(1)$$
$$
a/p = \varepsilon(a).\varepsilon(p)^*
$$

pour $a \in A$ et $p \in S$; le monoïde $E_S$ est donc engendré par $\varepsilon(E) \cup \varepsilon(S)^*$.

#### Proposition 6 {#alg-i-s2-prop-6 .statement}

*Les notations sont celles de la déf. 7 et $\varepsilon$ désigne l’homomorphisme canonique de $E$ dans $E_S$.*

(i) *Soient $a$ et $b$ dans $E$; pour qu’on ait $\varepsilon(a) = \varepsilon(b)$, il faut et il suffit qu’il existe $s \in S'$ avec $sa = sb$.*

(ii) *Pour que $\varepsilon$ soit injectif, il faut et il suffit que tout élément de $S$ soit simplifiable.*

(iii) *Pour que $\varepsilon$ soit bijectif, il faut et il suffit que tout élément de $S$ soit inversible.*

L’assertion (i) est claire, et entraîne que $\varepsilon$ est injectif si et seulement si tout élément de $S'$ est simplifiable; mais l’ensemble des éléments simplifiables de $E$ étant un sous-monoïde de $E$ (I, p. 15, prop. 2), il revient au même de dire que tout élément de $S$ est simplifiable.

Si $\varepsilon$ est bijective, tout élément de $S$ est inversible, car $\varepsilon(S)$ se compose d’éléments inversibles de $E_S$. Réciproquement, supposons tout élément de $S$ inversible; alors tout élément de $S'$ est inversible (I, p. 16, cor. 2), donc simplifiable. Alors $\varepsilon$ est injectif d’après (ii) et l’on a $a/p = \varepsilon(a.p^*)$ d’après (1), donc $\varepsilon$ est surjectif.

#### Théorème 1 {#alg-i-s2-thm-1 .statement}

*Soient $E$ un monoïde commutatif, $S$ une partie de $E$, $E_S$ le monoïde de fractions associé à $S$ et $\varepsilon : E \to E_S$ l’homomorphisme canonique. Soit de plus $f$ un homomorphisme de $E$ dans un monoïde $F$ (non nécessairement commutatif ), tel que tout élément de $f(S)$ soit inversible dans $F$. Il existe un homomorphisme $\bar{f}$ et un seul de $E_S$ dans $F$ tel que $f = \bar{f} \circ \varepsilon$.

Si $\bar{f}$ est un homomorphisme de $E_S$ dans $F$ tel que $f = \bar{f} \circ \varepsilon$, on a $\bar{f}(a/p) = \bar{f}(\varepsilon(a)\varepsilon(p)^*) = \bar{f}(\varepsilon(a))\bar{f}(\varepsilon(p))^* = f(a)f(p)^*$ pour $a \in E$ et $p \in S'$, d’où l’unicité de $\bar{f}$.

Soit $g$ l’application de $E \times S'$ dans $F$ définie par $g(a, p) = f(a).f(p)^*$. Montrons que $g$ est un homomorphisme de $E \times S'$ dans $F$. Tout d’abord, on a $g(e, e) = f(e)f(e)^* = e$. Soient $(a, p)$ et $(a', p')$ deux éléments de $E \times S'$; comme $a'$ et $p$ commutent dans $E$, $f(a')$ et $f(p)$ commutent dans $F$, d’où $f(a')f(p)^* = *(pf)f(a')$ d’après I, p. 16, prop. 5. On a par ailleurs $f(pp')^* = f(p'p)^* = (f(p')f(p))^* = f(p)^*f(p')^*$ d’après I, p. 16, prop. 4, d’où

$$
g(aa', pp') = f(aa')f(pp')^* = f(a)f(a')f(p)^*f(p')^* = f(a)f(p)^*f(a')f(p')^*
= g(a, p)g(a', p').
$$

Montrons que $g$ est compatible avec la relation d’équivalence $R$ dans $E \times S'$; si $(a, p)$ et $(a', p')$ sont congrus mod. $R$, il existe $s \in S'$ avec $spa' = sap'$, d’où $f(s)f(p)f(a') = f(s)f(a)f(p')$. Comme $f(s)$ est inversible, on en déduit $f(p)f(a') = f(a)f(p')$, puis, après multiplication à gauche par $f(p)^*$ et à droite par $f(p')^*$,

$$
g(a', p') = f(a')f(p')^* = f(p)^*f(a) = f(a)f(p)^* = g(a, p).
$$

Il existe donc un homomorphisme $\tilde{f}$ de $E_S$ dans $F$ tel que $\tilde{f}(a/p) = g(a, p)$ d’où $\tilde{f}(\varepsilon(a)) = \tilde{f}(a/e) = f(a)f(e)^* = f(a)$. On a donc $\tilde{f} \circ \varepsilon = f$.

#### Corollaire {#alg-i-s2-n4-cor-1 .statement}

*Soient $E$ et $F$ deux monoïdes commutatifs, $S$ et $T$ des parties de $E$ et $F$ respectivement, $f$ un homomorphisme de $E$ dans $F$ tel que $f(S) \subset T$, et $\varepsilon : E \to E_S, \eta : F \to F_T$ les homomorphismes canoniques. Il existe un homomorphisme $g : E_S \to F_T$ et un seul tel que $g \circ \varepsilon = \eta \circ f$.*

En effet, l’homomorphisme $\eta \circ f$ de $E$ dans $F_T$ transforme tout élément de $S$ en un élément inversible de $F_T$.

#### Remarque 1 {#alg-i-s2-n4-rem-1 .statement}

Le th. 1 peut encore s’énoncer en disant que $(E_S, \varepsilon)$ est solution du problème d’application universelle pour $E$, relativement aux monoïdes, aux homomorphismes de monoïdes, et aux homomorphismes de $E$ dans les monoïdes qui transforment les éléments de $S$ en éléments inversibles (E, IV, p. 23). Il en résulte (*loc. cit.*) que toute autre solution de ce problème est isomorphe de façon unique à $(E_S, \varepsilon)$.

#### Remarque 2 {#alg-i-s2-n4-rem-2 .statement}

Pour l’existence d’une solution du problème d’application universelle ci-dessus, il est inutile de supposer le monoïde $E$ commutatif, ainsi qu’il résulte de E, IV, p. 23 et p. 24 (cf. I p. 121, exerc. 17).

Mentionnons deux cas particuliers importants de monoïdes de fractions.

a) Soit $\overline{E} = E_E$. Comme le monoïde $\overline{E}$ est engendré par l’ensemble $\varepsilon(E) \cup \varepsilon(E)^*$ qui se compose d’éléments inversibles, tout élément de $\overline{E}$ est inversible (I, p. 16, cor. 2). Autrement dit, $\overline{E}$ est un groupe commutatif. De plus d’après le th. 1, tout homomorphisme $f$ de $E$ dans un groupe $G$ se factorise de manière unique sous la forme $f = \tilde{f} \circ \varepsilon$ où $\tilde{f} : \overline{E} \to G$ est un homomorphisme. On dit que $\overline{E}$ est le *groupe des fractions de* $E$ (ou *groupe des différences de* $E$ dans le cas de la notation additive).

b) Soit $\Phi = E_\Sigma$, où $\Sigma$ se compose des éléments simplifiables de $E$. D’après I, p. 18, prop. 6, (ii), l’homomorphisme canonique de $E$ dans $\Phi$ est injectif; on en profitera pour identifier $E$ à son image dans $\Phi$. Par suite, $E$ est un sous-monoïde de $\Phi$, tout élément simplifiable de $E$ a un inverse dans $\Phi$, et tout élément de $\Phi$ est de la forme $a/p = a.p^*$ avec $a \in E$ et $p \in \Sigma$; on a $a/p = a'/p'$ si et seulement si l’on a $ap' = pa'$. On voit facilement que les éléments inversibles de $\Phi$ sont les fractions $a/p$ avec $a$ et $p$ simplifiables et que $p/a$ est l’inverse de $a/p$.

Soit maintenant S un ensemble d’éléments simplifiables de E, et soit S’ le sous-monoïde de E engendré par S. Si $a/p$ et $a'/p'$ sont deux éléments de $E_S$, on a $a/p = a'/p'$ si et seulement si $ap' = pa'$ (car $sap' = spa'$ entraîne $ap' = pa'$ pour tout $s \in S'$). On peut donc identifier $E_S$ au sous-monoïde de $\Phi$ engendré par $E \cup S^*$.

Lorsque tout élément de E est simplifiable, on a $\Phi = \overline{E}$ et E est un sous-monoïde du groupe commutatif $\Phi$. Inversement, si E est isomorphe à un sous-monoïde d’un groupe, tout élément de E est simplifiable.

### 5. Applications : I. Entiers rationnels

Considérons le monoïde commutatif $\mathbf{N}$ des entiers naturels, la loi de composition étant l’addition ; tous les éléments de $\mathbf{N}$ sont simplifiables pour cette loi (E, III, p. 37, cor. 3). Le groupe des différences de $\mathbf{N}$ se note $\mathbf{Z}$; ses éléments sont appelés les entiers rationnels ; sa loi s’appelle addition des entiers rationnels et se note encore $+$ . L’homomorphisme canonique de $\mathbf{N}$ dans $\mathbf{Z}$ est injectif, et nous identifierons chaque élément de $\mathbf{N}$ à son image dans $\mathbf{Z}$. Les éléments de $\mathbf{Z}$ sont, par définition, les classes d’équivalence déterminées dans $\mathbf{N} \times \mathbf{N}$ par la relation $m_1 + n_2 = m_2 + n_1$ entre $(m_1, n_1)$ et $(m_2, n_2)$; un élément $m$ de $\mathbf{N}$ est identifié avec la classe formée des éléments $(m + n, n)$ où $n \in \mathbf{N}$; il admet pour opposé dans $\mathbf{Z}$ la classe des éléments $(n, m + n)$. Tout élément $(p, q)$ de $\mathbf{N} \times \mathbf{N}$ peut s’écrire sous la forme $(m + n, n)$ si $p \geq q$, sous la forme $(n, m + n)$ si $p \leq q$; il s’ensuit que $\mathbf{Z}$ est la réunion de $\mathbf{N}$ et de l’ensemble des opposés des éléments de $\mathbf{N}$. L’élément neutre 0 est le seul élément de $\mathbf{N}$ dont l’opposé appartienne à $\mathbf{N}$.

Pour tout entier naturel $m$, on note $-m$ l’entier rationnel opposé de $m$, et on note $-\mathbf{N}$ l’ensemble des éléments $-m$ pour $m \in \mathbf{N}$. On a

$$
\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N}) \quad \text{et} \quad \mathbf{N} \cap (-\mathbf{N}) = \{0\}.
$$

Pour $m \in \mathbf{N}$, on a $m = -m$ si et seulement si $m = 0$.

Soient $m$ et $n$ deux entiers naturels ;
a) si $m \geq n$, on a $m + (-n) = p$, où $p$ est l’élément de $\mathbf{N}$ tel que $m = n + p$;
b) si $m \leq n$, on a $m + (-n) = -p$, où $p$ est l’élément de $\mathbf{N}$ tel que $m + p = n$;
c) on a $(-m) + (-n) = -(m + n)$.

Les propriétés b) et c) résultent de I, p. 16, prop. 4; comme $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$, l’addition de $\mathbf{N}$ et les propriétés a), b) et c) caractérisent entièrement l’addition de $\mathbf{Z}$.

Plus généralement on désigne par $-x$ l’opposé d’un entier rationnel quelconque $x$; le composé $x + (-y)$ se note, de façon abrégée, $x - y$ (cf. I, p. 23).

La relation d’ordre $\leq$ entre entiers naturels est caractérisée par la propriété suivante : on a $m \leq n$ si et seulement s’il existe un entier $p \in \mathbf{N}$ tel que $m + p = n$ (E, III, p. 29, prop. 13 et p. 36, prop. 2). La relation $y - x \in \mathbf{N}$ entre entiers rationnels $x$ et $y$ est une relation d’ordre total sur $\mathbf{Z}$, qui prolonge la relation d’ordre $\leq$ sur $\mathbf{N}$. En effet, pour tout $x \in \mathbf{Z}$, on a $x - x = 0 \in \mathbf{N}$; si $y - x \in \mathbf{N}$ et $z - y \in \mathbf{N}$, on a $z - x = (z - y) + (y - x) \in \mathbf{N}$ car $\mathbf{N}$ est stable pour l’addition; si $y - x \in \mathbf{N}$ et $x - y \in \mathbf{N}$, on a $y - x = 0$, car 0 est le seul élément de $\mathbf{N}$ dont l’opposé appartienne à $\mathbf{N}$; quels que soient les entiers rationnels $x$ et $y$, on a $y - x \in \mathbf{N}$ ou $x - y \in \mathbf{N}$, car $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$; enfin si $x$ et $y$ sont des entiers naturels, on a $y - x \in \mathbf{N}$ si et seulement s’il existe $p \in \mathbf{N}$ tel que $x + p = y$. Cette relation d’ordre est encore notée $\leq$.

Lorsqu’on considérera désormais $\mathbf{Z}$ comme un ensemble ordonné, il s’agira toujours, sauf mention expresse du contraire, de l’ordre qui vient d’être défini; les entiers naturels sont identifiés aux entiers $\geq 0$: on les appelle encore entiers *positifs*; les entiers $\leq 0$, opposés des entiers positifs, sont dits entiers *négatifs*; les entiers $> 0$ (resp. $< 0$) sont dits *strictement positifs* (resp. *strictement négatifs*); l’ensemble des entiers $> 0$ se note parfois $\mathbf{N}^*$.

Soient $x$, $y$ et $z$ trois entiers rationnels; on a $x \leq y$ si et seulement si $x + z \leq y + z$. En effet $x - y = (x + z) - (y + z)$. On exprime cette propriété en disant que la relation d’ordre de $\mathbf{Z}$ est *invariante par translation*.

### 6. Applications: II. Multiplication des entiers rationnels

#### Lemme 2 {#alg-i-s2-lem-2 .statement}

*Soient E un monoïde et x un élément de E.*

(i) *Il existe un unique homomorphisme f de $\mathbf{N}$ dans E tel que $f(1) = x$, et l’on a $f(x) = \frac{n}{\top} x$ pour tout $n \in \mathbf{N}$.*

(ii) *Si x est inversible, il existe un unique homomorphisme g de $\mathbf{Z}$ dans E tel que $g(1) = x$ et g coïncide avec f dans $\mathbf{N}$.*

Posons $f(n) = \frac{n}{\top} x$ pour tout $n \in \mathbf{N}$; les formules $\frac{0}{\top} x = e$ et $(\frac{m}{\top} x) \top (\frac{n}{\top} x) = \frac{m+n}{\top} x$ (I, p. 13) expriment que $f$ est un homomorphisme de $\mathbf{N}$ dans E, et l’on a évidemment $f(1) = x$. Si $f'$ est un homomorphisme de $\mathbf{N}$ dans E tel que $f'(1) = x$, on a $f = f'$ d’après I, p. 6, prop. 1 (iv).

Supposons $x$ inversible. D’après I, p. 16, cor. 2, $f(n) = \frac{n}{\top} x$ est inversible pour tout entier $n \geq 0$. Par construction, $\mathbf{Z}$ est le groupe des différences de $\mathbf{N}$, donc (I, p. 18, th. 1), $f$ se prolonge de manière unique en un homomorphisme $g$ de $\mathbf{Z}$ dans E. Si $g'$ est un homomorphisme de $\mathbf{Z}$ dans E tel que $g'(1) = x$, la restriction $f'$ de $g'$ à $\mathbf{N}$ est un homomorphisme de $\mathbf{N}$ dans E tel que $f'(1) = x$. On a donc $f' = f$, d’où $g' = g$.

Nous appliquerons le lemme 2 au cas où le monoïde E est $\mathbf{Z}$; pour tout entier $m \in \mathbf{Z}$, il existe donc un endomorphisme $f_m$ de $\mathbf{Z}$ caractérisé par $f_m(1) = m$. Lorsque $m \in \mathbf{N}$, l’application $n \mapsto mn$ de $\mathbf{N}$ dans $\mathbf{N}$ est un endomorphisme du magma $\mathbf{N}$ (E, III, p. 27, corollaire); donc $f_m(n) = mn$ pour $m, n$ dans $\mathbf{N}$.

On peut donc prolonger la multiplication dans $\mathbf{N}$ en une multiplication dans \textbf{Z} par la formule $mn = f_m(n)$ pour $m, n$ dans $\mathbf{Z}$. Nous allons établir les formules:

(2) $$ xy = yx $$
(3) $$ (xy)z = x(yz) $$
(4) $$ x(y + z) = xy + xz $$
(5) $$ (x + y)z = xz + yz $$
(6) $$ 0.x = x.0 = 0 $$
(7) $$ 1.x = x.1 = x $$
(8) $$ (-1).x = x.(-1) = -x $$

pour $x, y, z$ dans $\mathbf{Z}$. (*Autrement dit, $\mathbf{Z}$ est un anneau commutatif.*) Les formules $x(y + z) = xy + xz$ et $x.0 = 0$ expriment que $f_x$ est un endomorphisme du monoïde additif $\mathbf{Z}$ et $f_x(1) = x$ s’écrit $x.1 = x$. L’endomorphisme $f_x \circ f_y$ de $\mathbf{Z}$ transforme 1 en $xy$, donc est égal à $f_{xy}$, d’où (3). On a $f_x(-y) = -f_x(y)$, c’est-à-dire $x(-y) = -xy$; de même, l’endomorphisme $y \mapsto -xy$ de $\mathbf{Z}$ transforme 1 en $-x$ d’où $(-x)y = -xy$, et par suite $(-x)(-y) = -(x(-y)) = -(-xy) = xy$. Pour $m, n$ dans $\mathbf{N}$, on a $mn = nm$ (E, III, p. 27, corollaire) d’où $(-m)n = n(-m)$ et $(-m)(-n) = (-n)(-m)$; comme $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$, on a donc $xy = yx$ pour $x, y$ dans $\mathbf{Z}$, et cette formule permet de déduire (5) de (4) et de compatible compléter les formules (6) à (8).

### 7. Applications: III. Puissances généralisées

Soit E un monoïde, d’élément neutre $e$, de loi de composition notée $\top$. Si $x$ est inversible dans E, soit $g_x$ l’homomorphisme de $\mathbf{Z}$ dans E appliquant 1 sur $x$. On pose $g_x(n) = \frac{n}{\top} x$ pour tout $n \in \mathbf{Z}$; d’après le lemme 2 (I, p. 21), cette notation est compatible pour $n \in \mathbf{N}$ avec la notation introduite antérieurement. On a

(9) $$ \frac{m+n}{\top} x = (\frac{m}{\top} x) \top (\frac{n}{\top} x) $$
(10) $$ \frac{0}{\top} x = e $$
(11) $$ \frac{1}{\top} x = x $$

pour $x$ inversible dans E et $m, n$ dans $\mathbf{Z}$. De plus, si $y = \frac{m}{\top} x$, l’application $n \mapsto g_x(mn)$ de $\mathbf{Z}$ dans E est un homomorphisme appliquant 1 sur $y$, d’où $g_x(mn) = g_y(n)$, c’est-à-dire

(12) $$ \frac{mn}{\top} x = \frac{n}{\top} (\frac{m}{\top} x). $$

Comme $-1$ est opposé de 1 dans $\mathbf{Z}$, $\frac{-1}{\top} x$ est l’inverse de $x = \frac{1}{\top} x$ dans E. Si l’on fait $n = -m$ dans (9) on voit que $\frac{-m}{\top} x$ est l’inverse de $\frac{m}{\top} x$.

### 8. Notations

a) Le plus souvent, on note additivement la loi d’un monoïde commutatif. On convient alors que $-x$ désigne l’opposé de $x$. On écrit de manière abrégée $x - y$ pour $x + (-y)$ et de même

$$
x + y - z, \quad x - y - z, \quad x - y + z - t, \quad \text{etc.} \ldots
$$

représentent respectivement

$$
x + y + (-z), \ x + (-y) + (-z), \ x + (-y) + z + (-t), \text{ etc.} \ldots
$$

Pour $n \in \mathbf{Z}$, la notation $\overset{n}{\top} x$ se remplace par $nx$. Les formules (9) à (12) (I. p. 22) se traduisent par

(13) $$ (m + n) . x = m . x + n . x $$
(14) $$ 0 . x = 0 $$
(15) $$ 1 . x = x $$
(16) $$ m . (n . x) = (mn) . x $$

où $m$ et $n$ appartiennent à $\mathbf{N}$ ou même à $\mathbf{Z}$ si $x$ admet un opposé. On a aussi dans ce dernier cas la relation $(-1) . x = -x$. Notons encore la formule

(17) $$ n . (x + y) = nx + ny. $$

b) Soit $E$ un monoïde noté multiplicativement. Pour $n \in \mathbf{Z}$, la notation $\overset{n}{\top} x$ se remplace par $x^n$. On a les relations

$$
x^{m+n} = x^m . x^n \\
x^0 = 1 \\
x^1 = x \\
(x^m)^n = x^{mn}
$$

et aussi $(xy)^n = x^ny^n$ si $x$ et $y$ commutent.

Lorsque $x$ a un inverse, celui-ci n’est autre que $x^{-1}$. On écrit aussi $\frac{1}{x}$ au lieu de $x^{-1}$. Enfin, lorsque le monoïde $E$ est commutatif, on écrit aussi $\frac{x}{y}$ ou $x/y$ pour $xy^{-1}$.

## EXERCICES {#alg-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
