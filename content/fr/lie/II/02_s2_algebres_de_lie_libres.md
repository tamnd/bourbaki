---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 2
section_title: Algèbres de Lie libres
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0015-0030, 0073-0076
extraction: ocr
subsections:
    - "no": 1
      title: Rappels sur les algèbres libres
      page: 0
      pdf_page: 15
    - "no": 2
      title: Construction de l’algèbre de Lie libre
      page: 0
      pdf_page: 16
    - "no": 3
      title: Présentations d’une algèbre de Lie
      page: 0
      pdf_page: 17
    - "no": 4
      title: Polynômes de Lie et substitutions
      page: 0
      pdf_page: 17
    - "no": 5
      title: Propriétés fonctorielles
      page: 0
      pdf_page: 18
    - "no": 6
      title: Graduations
      page: 0
      pdf_page: 19
    - "no": 7
      title: Suite centrale descendante
      page: 0
      pdf_page: 21
    - "no": 8
      title: Dérivations des algèbres de Lie libres
      page: 0
      pdf_page: 23
    - "no": 9
      title: Théorème d’élimination
      page: 0
      pdf_page: 23
    - "no": 10
      title: Ensembles de Hall dans un magma libre
      page: 0
      pdf_page: 25
    - "no": 11
      title: Bases de Hall d’une algèbre de Lie libre
      page: 0
      pdf_page: 28
statements: 31
exercises: 16
content_sha256: ee60790af4838f7791a04f248934d4827aa44db7cb09352d6210e67f648e4a45
---

## § 2. Algèbres de Lie libres

### 1. Rappels sur les algèbres libres

Soit X un ensemble. Rappelons la construction du magma libre M(X) construit sur X (A, I, p. 77). Par récurrence sur l’entier $n \geq 1$, on définit les ensembles $X_n$ en posant $X_1 = X$ et en prenant pour $X_n$ l’ensemble somme des ensembles $X_p \times X_{n-p}$ pour $p = 1, 2, \ldots, n-1$; si X est fini, il en est de même de chacun des $X_n$. L’ensemble somme de la famille $(X_n)_{n \geq 1}$ est noté M(X); chacun des ensembles $X_n$ (et en particulier X) est identifié à une partie de M(X). Soient $w$ et $w'$ dans M(X); on note $p$ et $q$ les entiers tels que $w \in X_p$ et $w' \in X_q$ et l’on pose $n = p + q$; l’image du couple $(w, w')$ par l’injection canonique de $X_p \times X_{n-p}$ dans $X_n$ se note $w.w'$ et s’appelle le produit de $w$ et $w'$. Toute application de X dans un magma M se prolonge de manière unique en un homomorphisme de magmas de M(X) dans M.

Soit $w$ dans M(X); l’unique entier $n$ tel que $w \in X_n$ s’appelle la *longueur* de $w$ et se note $l(w)$. On a $l(w.w') = l(w) + l(w')$ pour $w, w'$ dans M(X). L’ensemble X est la partie de M(X) formée des éléments de longueur 1. Tout élément $w$ de longueur $\geq 2$ s’écrit de manière unique sous la forme $w = w'.w''$.

L’algèbre du magma M(X) à coefficients dans l’anneau K est notée Lib(X), ou Lib$_K$(X) lorsqu’il y a lieu de préciser l’anneau K. L’ensemble M(X) est une base du K-module Lib(X), et X sera donc identifié à une partie de Lib(X). Si A est une algèbre, toute application de X dans A se prolonge de manière unique en un homomorphisme de Lib(X) dans A (A, III, p. 22, prop. 7).

### 2. Construction de l’algèbre de Lie libre

#### Définition 1 {#lie-ii-s2-def-1 .statement}

On appelle algèbre de Lie libre sur l’ensemble X l’algèbre quotient L(X) = Lib(X)/a où a est l’idéal bilatère de Lib(X) engendré par les éléments de l’une des formes

(1) $ Q(a) = a.a $ pour a dans Lib(X),
(2) $ J(a, b, c) = a.(b.c) + b.(c.a) + c.(a.b) $
pour $ a, b, c $ dans Lib(X).

Il est clair que L(X) est une K-algèbre de Lie; le composé de deux éléments $ u, v $ de L(X) sera noté $[u, v]$. Lorsqu’il y a lieu de préciser l’anneau K, on écrit $ L_K(X) $ pour L(X).

La proposition suivante justifie le nom d’algèbre de Lie libre donné à L(X).

#### Proposition 1 {#lie-ii-s2-prop-1 .statement}

Soient $ \psi $ l’application canonique de Lib(X) sur L(X) et $ \varphi $ la restriction de $ \psi $ à X. Pour toute application f de X dans une algèbre de Lie g, il existe un homomorphisme F : L(X) $ \to g $ et un seul tel que $ f = F \circ \varphi $.

a) Existence de F : soit h l’homomorphisme de Lib(X) dans g prolongeant f (n° 1). Pour tout a dans Lib(X), on a $ h(Q(a)) = h(a.a) = [h(a), h(a)] = 0 $; de même, l’identité de Jacobi satisfaite par g entraîne $ h(J(a, b, c)) = 0 $ pour $ a, b, c $ dans Lib(X). On en déduit $ h(a) = 0 $, d’où un homomorphisme F de L(X) dans g tel que $ h = F \circ \psi $. Par restriction à X, on obtient $ f = F \circ \varphi $.

b) Unicité de F : soit $ F' : L(X) \to g $ un homomorphisme tel que $ f = F' \circ \varphi $. Les homomorphismes $ F \circ \psi $ et $ F' \circ \psi $ de Lib(X) dans g coïncident dans X, donc sont égaux; comme $ \psi $ est surjective, on a $ F = F' $.

#### Corollaire 1 {#lie-ii-s2-prop-1-cor-1 .statement}

La famille $ (\varphi(x))_{x \in X} $ est libre sur K dans L(X).

Soient $ x_1, x_2, \ldots, x_n $ des éléments distincts de X et $ \lambda_1, \ldots, \lambda_n $ dans K tels que
$$
\lambda_1 \cdot \varphi(x_1) + \cdots + \lambda_n \cdot \varphi(x_n) = 0.
$$
Soit g l’algèbre de Lie commutative ayant K comme module sous-jacent. Pour $ i = 1, 2, \ldots, n $, il existe un homomorphisme $ F_i $ de L(X) dans g tel que $ F_i(\varphi(x_i)) = 1 $ et $ F_i(\varphi(x)) = 0 $ pour $ x \neq x_i $ (prop. 1); appliquant $ F_i $ à la relation (3), on trouve $ \lambda_i = 0 $.

#### Corollaire 2 {#lie-ii-s2-prop-1-cor-2 .statement}

Soit a une algèbre de Lie. Toute extension de L(X) par a est inessentielle.

Soit $ a \xrightarrow{\lambda} g \xrightarrow{\mu} L(X) $ une telle extension (chap. I, § 1, n° 7). Comme $ \mu $ est surjective, il existe une application f de X dans g telle que $ \varphi = \mu \circ f $. Soit F l’homomorphisme de L(X) dans g tel que $ f = F \circ \varphi $ (prop. 1). On a $ (\mu \circ F) \circ \varphi = $

Comme l’anneau K n’est pas réduit à 0, le cor. 1 de la prop. 1 montre que φ est injective. On peut donc identifier au moyen de φ l’ensemble X à son image dans L(X); avec cette convention, X engendre L(X) et toute application de X dans une algèbre de Lie g se prolonge en un homomorphisme d’algèbres de Lie de L(X) dans g.

#### Remarque {#lie-ii-s2-n2-rem-1 .statement}

Lorsque X est vide, M(X) est vide, donc L(X) = {0}. Si X a un seul élément x, le sous-module K.x de L(X) est une sous-algèbre de Lie de L(X); comme X engendre L(X), le cor. 1 de la prop. 1 montre que L(X) est un module libre de base {x}.

### 3. Présentations d’une algèbre de Lie

Soient g une algèbre de Lie et $ a = (a_i)_{i \in I} $ une famille d’éléments de g. On note $ f_a $ l’homomorphisme de L(I) dans g appliquant tout $ i \in I $ sur $ a_i $. L’image de $ f_a $ est la sous-algèbre de g engendrée par $ a $; les éléments du noyau de $ f_a $ s’appellent les relateurs de la famille $ a $. On dit que la famille $ a $ est génératrice (resp. libre, basique) si $ f_a $ est surjectif (resp. injectif, bijectif).

Soit g une algèbre de Lie. Une présentation de g est un couple $ (a, r) $ formé d’une famille génératrice $ a = (a_i)_{i \in I} $ et d’une famille $ r = (r_j)_{j \in J} $ de relateurs de $ a $ engendrant l’idéal de L(I) noyau de $ f_a $. On dit aussi que g est présentée par la famille $ a $ liée par les relateurs $ r_j $ ($ j \in J $).

Soient I un ensemble et $ r = (r_j)_{j \in J} $ une famille d’éléments de l’algèbre de Lie libre L(I); soit $ a_r $ l’idéal de L(I) engendré par $ r $. L’algèbre quotient $ L(I, r) = L(I)/a_r $ s’appelle l’algèbre de Lie définie par I et la famille de relateurs $ (r_j)_{j \in J} $; on dit aussi que $ L(I, r) $ est définie par la présentation $ (I, r) $, ou encore par $ (I; (r_j = 0)_{j \in J}) $. Lorsque la famille $ r $ est vide, on a $ L(I, r) = L(I) $.

Soient I et $ r $ comme précédemment; notons $ \xi_i $ l’image de $ i $ dans $ L(I, r) $. La famille génératrice $ \xi = (\xi_i)_{i \in I} $ et la famille de relateurs $ r $ constituent une présentation de $ L(I, r) $. Réciproquement, si g est une algèbre de Lie et $ (a, r) $, avec $ a = (a_i)_{i \in I} $, une présentation de g, il existe un unique isomorphisme $ u : L(I, r) \to g $ tel que $ u(\xi_i) = a_i $ pour tout $ i \in I $.

### 4. Polynômes de Lie et substitutions

Soit I un ensemble. Notons $ T_i $ l’image canonique de l’élément $ i $ de I dans L(I) (que l’on note aussi parfois $ L((T_i)_{i \in I}) $); les éléments de L(I) s’appellent polynômes de Lie en les indéterminées $ (T_i)_{i \in I} $.

Soit g une algèbre de Lie. Si $ t = (t_i)_{i \in I} $ est une famille d’éléments de g, notons $ f_t $ l’homomorphisme de L(I) dans g tel que $ f_t(T_i) = t_i $ pour $ i \in I $ (no 2, prop. 1). L’image par $ f_t $ de l’élément P de L(I) se note $ P((t_i)_{i \in I}) $. En particulier, on a $ P((T_i)_{i \in I}) = P $; l’élément $ P((t_i)_{i \in I}) $ précédent s’appelle parfois l’élément de g obtenu par substitution des $ t_i $ aux $ T_i $ dans le polynôme de Lie $ P((T_i)_{i \in I}) $.

Soit $ \sigma : g \to g' $ un homomorphisme d’algèbres de Lie. Pour toute famille $ t = (t_i)_{i \in I} $ d’éléments de $ g $ et tout $ P \in L(I) $, on a
$$
\sigma(P((t_i)_{i \in I})) = P((\sigma(t_i))_{i \in I}),
$$
car $ \sigma \circ f_t $ applique $ T_i $ sur $ \sigma(t_i) $, pour $ i \in I $.

Soit $ (Q_j)_{j \in J} $ une famille d’éléments de $ L(I) $, et soit $ P \in L(J) $. Par substitution des $ Q_j $ aux $ T_j $ dans $ P $, on obtient un polynôme de Lie $ R = P((Q_j)_{j \in J}) \in L(I) $. On a
$$
R((t_i)_{i \in I}) = P((Q_j((t_i)_{i \in I}))_{j \in J}),
$$
pour toute famille $ t = (t_i)_{i \in I} $ d’éléments d’une algèbre de Lie $ g $, comme on le voit en transformant par l’homomorphisme $ f_t $ l’égalité $ R = P((Q_j)_{j \in J}) $ et en tenant compte de (4).

Soient $ g $ une algèbre de Lie, $ I $ un ensemble fini, et $ P \in L(I) $. Supposons que $ g $ soit un $ K $-module libre. L’application
$$
\tilde{P} : g^I \to g
$$
définie par $ \tilde{P}((t_i)_{i \in I}) = P((t_i)_{i \in I}) $ est alors *polynomiale*.¹ En effet, l’ensemble $ F $ des applications de $ g^I $ dans $ g $ est une algèbre de Lie pour le crochet défini par
$$
[\varphi, \psi](t) = [\varphi(t), \psi(t)];
$$
l’ensemble $ F' $ des applications polynomiales de $ g^I $ dans $ g $ en est une sous-algèbre de Lie, d’après la bilinéarité du crochet. Notre assertion résulte alors de ce que l’application $ P \mapsto \tilde{P} $ est un homomorphisme d’algèbres de Lie et que $ \tilde{T}_i = \mathrm{pr}_i \in F' $ pour tout $ i $.

### 5. Propriétés fonctorielles

#### Proposition 2 {#lie-ii-s2-prop-2 .statement}

*Soient X et Y deux ensembles. Toute application $ u : X \to Y $ se prolonge de manière unique en un homomorphisme d’algèbres de Lie $ L(u) : L(X) \to L(Y) $. Pour toute application $ v : Y \to Z $, on a $ L(v \circ u) = L(v) \circ L(u) $.*

L’existence et l’unicité de $ L(u) $ résultent de la prop. 1 du n° 2. Les homomorphismes $ L(v \circ u) $ et $ L(v) \circ L(u) $ ont même restriction à $ X $, donc sont égaux (prop. 1).

#### Corollaire {#lie-ii-s2-n5-cor-1 .statement}

*Si $ u $ est injective (resp. surjective, bijective), il en est de même de $ L(u) $.*

L’assertion étant triviale pour $ X = \emptyset $, supposons $ X \neq \emptyset $. Si $ u $ est injective, il existe une application $ v $ de $ Y $ dans $ X $ telle que $ v \circ u $ soit l’application identique de $ X $; d’après la prop. 2, $ L(v) \circ L(u) $ est l’automorphisme identique de $ L(X) $, donc

¹ Rappelons (A, IV, § 5, n° 10, n°11e édition) la définition des applications polynomiales d’un module libre $ M $ dans un module $ N $: si $ q $ est un entier $ \geqslant 0 $, on dit qu’une application $ f : M \to N $ est *polynomiale homogène de degré* $ q $ s’il existe une application multilinéaire $ u $ de $ M^q $ dans $ N $ telle que
$$
f(x) = u(x, \ldots, x) \quad \text{pour tout } x \in M.
$$
Une application de $ M $ dans $ N $ est dite *polynomiale* si elle est somme finie d’applications polynomiales homogènes de degrés convenables.

L(u) est injective. Lorsque u est surjective, il existe une application w de Y dans X telle que u ∘ w soit l’application identique de Y; alors L(u) ∘ L(w) est l’application identique de L(Y), ce qui prouve que L(u) est surjective.

Soit X un ensemble et soit S une partie de X. Le corollaire précédent montre que l’injection canonique de S dans X se prolonge en un isomorphisme α de L(S) sur la sous-algèbre de Lie L'(S) de L(X) engendrée par S; nous identifierons L(S) et L'(S) au moyen de α.

Soit (S_α)_{α ∈ I} une famille filtrante croissante de parties de X, de réunion S. La relation S_α ⊂ S_β entraîne L(S_α) ⊂ L(S_β), donc la famille des sous-algèbres de Lie L(S_α) de L(X) est filtrante croissante. Par suite, g = ⋃_{α ∈ I} L(S_α) est une sous-algèbre de Lie de L(X); on a S ⊂ g, d’où L(S) ⊂ g, et comme L(S_α) ⊂ L(S) pour tout α ∈ I, on a g ⊂ L(S). Donc

$$
L(\bigcup_{α ∈ I} S_α) = \bigcup_{α ∈ I} L(S_α)
$$

pour toute famille filtrante croissante (S_α)_{α ∈ I} de parties de X.

Appliquant ce qui précède à la famille des parties finies de X, on voit que tout élément de L(X) est de la forme P(x_1, ..., x_n) où P est un polynôme de Lie à n indéterminées et x_1, ..., x_n sont des éléments de X.

#### Proposition 3 {#lie-ii-s2-prop-3 .statement}

Soit K' un anneau commutatif non réduit à {0}, et soit u : K → K' un homomorphisme d’anneaux. Pour tout ensemble X, il existe un homomorphisme de K'-algèbres de Lie et un seul

$$ v : L_K(X) \otimes K' \to L_{K'}(X) $$

tel que v(x ⊗ 1) = x pour x ∈ X. De plus, v est un isomorphisme.

Appliquant la prop. 1 à g = L_{K'}(X) considérée comme K'-algèbre de Lie, et à l’application x ↦ x de X dans g, on obtient un K-homomorphisme L_K(X) → L_{K'}(X), d’où un K'-homomorphisme v : L_K(X) ⊗ K' → L_{K'}(X). Le fait que v soit unique et soit un isomorphisme résulte du ce que le couple (L_K(X) ⊗ K', x ↦ x ⊗ 1) est solution du même problème universel que le couple (L_{K'}(X), x ↦ x).

#### Remarque {#lie-ii-s2-n5-rem-1 .statement}

Soient h' une K'-algèbre de Lie et h la K-algèbre de Lie déduite de h' par restriction de l’anneau des scalaires. Si P ∈ L_K(X), on peut définir $ \tilde{P} : h^X \to h $ (n° 4). On voit aussitôt que

$$
\tilde{P} = (v(P \otimes 1))^\sim.
$$

### 6. Graduations

Soit Δ un monoïde commutatif, noté additivement. On note φ_0 une application de X dans Δ et φ l’homomorphisme du magma libre M(X) dans Δ qui prolonge φ_0. Pour tout δ ∈ Δ, soit Lib^δ(X) le sous-module de Lib(X) ayant pour base la partie $ \varphi^{-1}(\delta) $ de $ M(X) $. La famille $ (\mathrm{Lib}^\delta(X))_{\delta \in \Delta} $ est une graduation de l’algèbre $ \mathrm{Lib}(X) $, c’est-à-dire que l’on a

(8)
$$
\mathrm{Lib}(X) = \bigoplus_{\delta \in \Delta} \mathrm{Lib}^\delta(X)
$$
(9)
$$
\mathrm{Lib}^\delta(X) \cdot \mathrm{Lib}^{\delta'}(X) \subset \mathrm{Lib}^{\delta + \delta'}(X) \quad \text{pour } \delta, \delta' \text{ dans } \Delta
$$
(A, III, p. 31, Exemple 3).

**Lemme 1. — L’idéal a de la définition 1 est gradué.**

Pour $ a, b $ dans $ \mathrm{Lib}(X) $, posons $ B(a, b) = a.b + b.a $. Les formules
(10)
$$
B(a, b) = Q(a + b) - Q(a) - Q(b)
$$
(11)
$$
Q(\lambda_1.w_1 + \cdots + \lambda_n.w_n) = \sum_i \lambda_i^2 Q(w_i) + \sum_{i < j} \lambda_i \lambda_j B(w_i, w_j)
$$
pour $ w_1, \ldots, w_n $ dans $ M(X) $ et $ \lambda_1, \ldots, \lambda_n $ dans $ K $, montrent que les familles $ (Q(a))_{a \in \mathrm{Lib}(X)} $ et $ (Q(w), B(w, w'))_{w, w' \in M(X)} $ engendrent le même sous-module de $ \mathrm{Lib}(X) $. Comme $ J $ est trilinéaire, l’idéal $ a $ est engendré par les éléments homogènes $ Q(w), B(w, w') $ et $ J(w, w', w'') $ pour $ w, w', w'' $ dans $ M(X) $, donc est gradué (A, III, p. 32, prop. 1).

C.Q.F.D.

Munissons l’algèbre de Lie $ L(X) = \mathrm{Lib}(X)/a $ de la graduation quotient. La composante homogène de degré $ \delta $ de $ L(X) $ est notée $ L^\delta(X) $; c’est le sous-module de $ L(X) $ engendré par les images des éléments $ w \in M(X) $ tels que $ \varphi(w) = \delta $.

Nous utiliserons surtout les deux cas particuliers suivants:

a) *Graduation totale*: on prend $ \Delta = \mathbf{N} $ et $ \varphi_0(x) = 1 $ pour tout $ x \in X $, d’où $ \varphi(w) = l(w) $ pour $ w $ dans $ M(X) $. Le $ K $-module $ L^n(X) $ est engendré par les images des éléments de longueur $ n $ dans $ M(X) $, que nous appellerons *alternants de degré n*. Nous verrons plus tard que le module $ L^n(X) $ est libre et admet une base formée d’alternants de degré $ n $ (n° 11, th. 1). On a $ L(X) = \bigoplus_{n \geq 1} L^n(X) $, et $ L^1(X) $ admet $ X $ pour base (n° 2, cor. 1 de la prop. 1). Par construction de $ M(X) $, on a
(12)
$$
L^n(X) = \sum_{p=1}^{n-1} [L^p(X), L^{n-p}(X)]
$$
et en particulier
(13)
$$
[L^m(X), L^n(X)] \subset L^{m+n}(X).
$$

b) *Multigraduation*: on prend pour $ \Delta $ le monoïde commutatif libre $ \mathbf{N}^{(X)} $ construit sur $ X $. L’application $ \varphi_0 $ de $ X $ dans $ \Delta $ est définie par $ (\varphi_0(x))(x') = \delta_{xx'} $, où $ \delta_{xx'} $ est le symbole de Kronecker. Pour $ w \in M(X) $ et $ x \in X $, l’entier $ (\varphi(w))(x) $ est « le nombre d’occurrences de la lettre $ x $ dans $ w $ ». Pour $ \alpha $ dans $ \mathbf{N}^{(X)} $, on pose $ |\alpha| = \sum_{x \in X} \alpha(x) $, d’où $ |\varphi(w)| = l(w) $ pour tout $ w $ dans $ M(X) $. On en déduit

(14) $$
L^n(X) = \bigoplus_{|\alpha|=n} L^\alpha(X);
$$
on a évidemment

(15) $$
[L^\alpha(X), L^\beta(X)] \subset L^{\alpha+\beta}(X) \quad \text{pour } \alpha, \beta \text{ dans } N^{(X)}.
$$

#### Proposition 4 {#lie-ii-s2-prop-4 .statement}

*Soit S une partie de X. Si l’on identifie $ N^{(S)} $ à son image canonique dans $ N^{(X)} $* (A, I, p. 89), *on a* $ L(S) = \sum_{\alpha \in N^{(S)}} L^\alpha(X) $. *De plus, pour tout* $ \alpha \in N^{(S)} $, *la composante homogène de degré* $ \alpha $ *pour la multigraduation de* $ L(S) $ *est égale à* $ L^\alpha(X) $.

Soit $ \alpha \in N^{(S)} $. Le module $ L^\alpha(S) $ est engendré par les images dans $ L(X) $ des éléments $ w $ *de* $ M(S) $ tels que $ \varphi(w) = \alpha $, c’est-à-dire (A, I, p. 91, formules (23) et (24)) l’ensemble des $ w $ *de* $ M(X) $ tels que $ \varphi(w) = \alpha $. On a donc $ L^\alpha(S) = L^\alpha(X) $.

La proposition résulte de là et de la relation $ L(S) = \sum_{\alpha \in N^{(S)}} L^\alpha(S) $.

#### Corollaire {#lie-ii-s2-n6-cor-1 .statement}

*Pour toute famille* $ (S_i)_{i \in I} $ *de parties de* $ X $, *on a*

(16) $$
L\left(\bigcap_{i \in I} S_i\right) = \bigcap_{i \in I} L(S_i).
$$

Cela résulte de la prop. 4 et de la formule évidente

(17) $$
N^{(S)} = \bigcap_{i \in I} N^{(S_i)}
$$
où l’on a posé $ S = \bigcap_{i \in I} S_i $.

### 7. Suite centrale descendante

#### Proposition 5 {#lie-ii-s2-prop-5 .statement}

*Soient* $ g $ *une algèbre de Lie et* $ P $ *un sous-module de* $ g $. *Définissons les sous-modules* $ P_n $ *de* $ g $ *par les formules* $ P_1 = P $ *et* $ P_{n+1} = [P, P_n] $ *pour* $ n \geqslant 1 $. *Alors on a*

(18) $$
[P_m, P_n] \subset P_{m+n},
$$
(19) $$
P_n = \sum_{p=1}^{n-1} [P_p, P_{n-p}] \quad \text{pour } n \geqslant 2.
$$

Démontrons (18) par récurrence sur $ m $. Le cas $ m = 1 $ est clair. D’après l’identité de Jacobi, on a
$$
[[P, P_m], P_n] \subset [P_m, [P, P_n]] + [P, [P_m, P_n]],
$$
c’est-à-dire
$$
[P_{m+1}, P_n] \subset [P_m, P_{n+1}] + [P, [P_m, P_n]].
$$
L’hypothèse de récurrence entraîne $ [P_m, P_{n+1}] \subset P_{m+n+1} $ et $ [P_m, P_n] \subset P_{m+n} $, d’où
$$
[P_{m+1}, P_n] \subset P_{m+n+1} + [P, P_{m+n}] = P_{m+n+1}.
$$

D’après la formule (18), on a $ P_n \supset \sum_{p=1}^{n-1} [P_p, P_{n-p}] \supset [P_1, P_{n-1}] = P_n $, d’où (19).

Lorsque l’on prend $ P = g $, la suite $ (P_n) $ est la suite centrale descendante $ (\mathcal{C}^n g) $ de $ g $ (chap. I, § 1, n° 5, 2ème édition).¹ On a donc:

#### Proposition 6 {#lie-ii-s2-prop-6 .statement}

*Soient g une algèbre de Lie et $ (\mathcal{C}^n g)_{n \geq 1} $ la suite centrale descendante de g. On a*
$$
[\mathcal{C}^m g, \mathcal{C}^n g] \subset \mathcal{C}^{m+n} g \quad \text{pour } m \geq 1 \text{ et } n \geq 1.
$$

Généralisant la déf. 1 du chap. I, § 4, n° 1, nous dirons qu’une algèbre de Lie $ g $ est *nilpotente* si $ \mathcal{C}^n g = \{0\} $ pour $ n $ assez grand. On appelle *classe de nilpotence* d’une algèbre de Lie nilpotente $ g $ le plus petit entier $ n $ tel que $ \mathcal{C}^{n+1} g = \{0\} $.

#### Proposition 7 {#lie-ii-s2-prop-7 .statement}

*Soit X un ensemble et soit n un entier $ \geq 1 $.*
a) *On a $ L^{n+1}(X) = [L^1(X), L^n(X)] $.*
b) *Le module $ L^n(X) $ est engendré par les éléments $ [x_1, [x_2, \ldots, [x_{n-1}, x_n] \ldots]] $ où $ (x_1, \ldots, x_n) $ parcourt l’ensemble des suites de n éléments de X.*
c) *La suite centrale descendante de $ L(X) $ est donnée par $ \mathcal{C}^n(L(X)) = \sum_{p \geq n} L^p(X) $.*

a) Nous appliquerons la prop. 5 avec $ g = L(X) $ et $ P = L^1(X) $. Par récurrence sur $ n $, on déduit de (12) (n° 6) et (19) l’égalité $ P_n = L^n(X) $. La relation cherchée équivaut alors à la définition $ [P, P_n] = P_{n+1} $.
b) Cela résulte de a) par récurrence sur $ n $.
c) Posons $ g = L(X) $ et $ g_n = \sum_{p \geq n} L_p(X) $. On a $ g = g_1 $ et la formule (13) du n° 6 entraîne $ [g_n, g_m] \subset g_{n+m} $, et en particulier $ [g, g_n] \subset g_{n+1} $. Par récurrence sur $ n $, on a $ \mathcal{C}^n g \subset g_n $. Par ailleurs, de a) on déduit $ L^n(X) \subset \mathcal{C}^n g $ par récurrence sur $ n $. Comme $ \mathcal{C}^n g $ est un idéal de $ g $, la relation $ L^p(X) \subset \mathcal{C}^n g $ entraîne
$$
L^{p+1}(X) = [L^1(X), L^p(X)] \subset \mathcal{C}^n g
$$
d’après a). On a donc $ L^p(X) \subset \mathcal{C}^n g $ pour $ p \geq n $, d’où $ g_n \subset \mathcal{C}^n g $.

#### Corollaire {#lie-ii-s2-n7-cor-1 .statement}

*Soient g une algèbre de Lie et $ (x_i)_{i \in I} $ une famille génératrice dans g. Le n-ième terme $ \mathcal{C}^n g $ de la suite centrale descendante de g est le module engendré par les crochets itérés $ [x_{i_1}, [x_{i_2}, \ldots, [x_{i_{p-1}}, x_{i_p}] \ldots]] $ pour $ p \geq n $ et $ i_1, \ldots, i_p $ dans I.*
Soit $ f $ l’homomorphisme de $ L(I) $ dans $ g $ tel que $ f(i) = x_i $ pour tout $ i \in I $. Comme $ (x_i)_{i \in I} $ engendre $ g $, on a $ g = f(L(I)) $, d’où $ \mathcal{C}^n g = f(\mathcal{C}^n(L(I))) $ d’après la prop. 4 du chap. I, § 1, n° 5. Le corollaire résulte alors des assertions b) et c) de la prop. 7.

¹ Avec la définition adoptée dans la première édition du chap. I, on aurait $ P_n = \mathcal{C}^{n-1} g $.

### 8. Dérivations des algèbres de Lie libres

#### Proposition 8 {#lie-ii-s2-prop-8 .statement}

Soit X un ensemble, soit M un L(X)-module et soit d une application de X dans M. Il existe une application linéaire D de L(X) dans M, et une seule, prolongeant d et satisfaisant à la relation:

(20) $ D([a, a']) = a.D(a') - a'.D(a) $ pour $ a, a' $ dans $ L(X) $.

On définit une algèbre de Lie g ayant pour module sous-jacent $ M \times L(X) $ au moyen du crochet

(21) $$ [(m, a), (m', a')] = (a.m' - a'.m, [a, a']), $$

pour $ a, a' $ dans $ L(X) $ et $ m, m' $ dans $ M $ (chap. I, § 1, n° 8). Soit $ f $ l’homomorphisme de $ L(X) $ dans $ g $ tel que $ f(x) = (d(x), x) $ pour tout $ x $ dans $ X $; posons $ f(a) = (D(a), u(a)) $ pour tout $ a $ dans $ L(X) $. D’après la formule (21), $ u $ est un homomorphisme de $ L(X) $ dans elle-même; comme on a $ u(x) = x $ pour $ x $ dans $ X $, on a $ u(a) = a $ pour tout $ a $ dans $ L(X) $, d’où

(22) $ f(a) = (D(a), a) $.

D’après (21) et (22), la relation (20) découle alors de $ f([a, a']) = [f(a), f(a')] $.

Réciproquement, soit $ D' $ une application de $ L(X) $ dans $ M $ qui satisfasse à la relation (20’) analogue à (20) et prolonge $ d $. Posons $ f'(a) = (D'(a), a) $ pour $ a \in L(X) $; d’après (20’) et (21), $ f' $ est un homomorphisme de $ L(X) $ dans $ g $, coïncidant avec $ f $ dans $ X $, d’où $ f' = f $ et $ D' = D $.

#### Corollaire {#lie-ii-s2-n8-cor-1 .statement}

Toute application de X dans $ L(X) $ se prolonge de manière unique en une dérivation de $ L(X) $.

Lorsque $ M $ est égal à $ L(X) $ muni de la représentation adjointe, la relation (20) signifie que $ D $ est une dérivation.

### 9. Théorème d’élimination

#### Proposition 9 {#lie-ii-s2-prop-9 .statement}

Soient $ S_1 $ et $ S_2 $ deux ensembles disjoints et d une application de $ S_1 \times S_2 $ dans $ L(S_2) $. Soit $ g $ l’algèbre de Lie quotient de $ L(S_1 \cup S_2) $ par l’idéal qu’engendrent les éléments $ [s_1, s_2] - d(s_1, s_2) $ pour $ s_1 \in S_1, s_2 \in S_2 $; soit $ \psi $ l’application canonique de $ L(S_1 \cup S_2) $ sur $ g $.

a) Pour $ i = 1, 2 $, la restriction $ \varphi_i $ de $ \psi $ à $ S_i $ se prolonge en un isomorphisme de $ L(S_i) $ sur une sous-algèbre $ a_i $ de $ g $.

b) On a $ g = a_1 + a_2, a_1 \cap a_2 = \{0\} $ et $ a_2 $ est un idéal de $ g $.

Pour $ i = 1, 2 $, notons $ \psi_i $ l’homomorphisme de $ L(S_i) $ dans $ g $ qui prolonge $ \varphi_i $, et $ a_i $ son image. Il est clair que $ \varphi_i(S_i) $ engendre $ a_i $.

Soit $ s_1 \in S_1 $; on pose $ D = \mathrm{ad}\, \varphi_1(s_1) $. La dérivation $ D $ de $ g $ applique $ \varphi_2(S_2) $ dans $ a_2 $ d’après la relation

$$
[\varphi_1(s_1), \varphi_2(s_2)] = \psi_2(d(s_1, s_2)) \quad \text{pour } s_2 \in S_2;
$$

comme la sous-algèbre $ a_2 $ de $ g $ est engendrée par $ \varphi_2(S_2) $, on a donc $ D(a_2) \subset a_2 $. L’ensemble des $ x \in g $ tels que $ \mathrm{ad}\, x $ laisse stable $ a_2 $ est une sous-algèbre de Lie de $ g $, qui contient $ \varphi_1(S_1) $ d’après ce qui précède, donc aussi $ a_1 $. On a donc

(23)
$$
[a_1, a_2] \subset a_2.
$$

Par suite $ a_1 + a_2 $ est une sous-algèbre de Lie de $ g $, et comme elle contient l’ensemble générateur $ \varphi_1(S_1) \cup \varphi_2(S_2) $, on a

(24)
$$
a_1 + a_2 = g.
$$

Pour tout $ s_1 \in S_1 $, il existe une dérivation $ D_{s_1} $ de $ L(S_2) $ telle que $ D_{s_1}(s_2) = d(s_1, s_2) $ pour tout $ s_2 $ dans $ S_2 $ (n° 8, cor. de la prop. 8). L’application $ s_1 \mapsto D_{s_1} $ se prolonge en un homomorphisme $ D $ de $ L(S_1) $ dans l’algèbre de Lie des dérivations de $ L(S_2) $. Soit $ \mathfrak{h} $ le produit semi-direct de $ L(S_1) $ par $ L(S_2) $ correspondant à $ D $ (chap. I, § 1, n° 8). En tant que module, $ \mathfrak{h} $ est égal à $ L(S_1) \times L(S_2) $, et l’on a en particulier

(25)
$$
[(s_1, 0), (0, s_2)] = (0, d(s_1, s_2))
$$

pour $ s_1 \in S_1 $ et $ s_2 \in S_2 $.

De (25) on déduit l’existence d’un homomorphisme $ f $ de $ g $ dans $ \mathfrak{h} $ tel que $ f(\varphi_1(s_1)) = (s_1, 0) $ et $ f(\varphi_2(s_2)) = (0, s_2) $ pour $ s_1 \in S_1 $ et $ s_2 \in S_2 $. On en déduit aussitôt la relation

(26)
$$
f(\psi_1(a_1) + \psi_2(a_2)) = (a_1, a_2)
$$

pour $ a_1 \in L(S_1) $ et $ a_2 \in L(S_2) $.

La relation (26) montre que $ \psi_1 $ et $ \psi_2 $ sont injectifs et que $ a_1 \cap a_2 = \{0\} $. Les formules (23) et (24) entraînent alors la proposition.

#### Proposition 10 (théorème d’élimination) {#lie-ii-s2-prop-10 .statement}

Soient $ X $ un ensemble, $ S $ une partie de $ X $, et $ T $ l’ensemble des suites $ (s_1, \ldots, s_n, x) $ avec $ n \geqslant 0 $, $ s_1, \ldots, s_n $ dans $ S $ et $ x $ dans $ X - S $.\footnote{Pour $ n = 0 $, on obtient les éléments de $ X - S $, d’où $ X - S \subset T $.}

a) Le module $ L(X) $ est somme directe de la sous-algèbre $ L(S) $ de $ L(X) $ et de l’idéal $ a $ de $ L(X) $ engendré par $ X - S $.

b) Il existe un isomorphisme d’algèbres de Lie $ \varphi $ de $ L(T) $ sur $ a $ qui transforme $ (s_1, \ldots, s_n, x) $ en $ (\mathrm{ad}\, s_1 \circ \ldots \circ \mathrm{ad}\, s_n)(x) $.

Soit $ g $ l’algèbre de Lie construite comme dans la prop. 9 avec les données
$$
S_1 = S, \quad S_2 = T, \quad d(s, t) = (s, s_1, \ldots, s_n, x) \in T \subset L(T)
$$
pour $ t = (s_1, \ldots, s_n, x) $ dans $ T $ et $ s \in S_1 $. Nous identifions $ L(S) $ et $ L(T) $ à leurs images canoniques dans $ g $ (prop. 9, $ a $).

Soit $ \psi $ l’application $ (s_1, \ldots, s_n, x) \mapsto (\operatorname{ad} s_1 \circ \cdots \circ \operatorname{ad} s_n)(x) $ de $ T $ dans $ L(X) $. On a évidemment $ \psi(d(s, t)) = [s, \psi(t)] $ pour $ s \in S $ et $ t \in T $, et il existe donc un homomorphisme $ \alpha : g \to L(X) $ dont la restriction à $ S $ est l’identité et dont la restriction à $ T $ est $ \psi $. On a $ X - S \subset T $, d’où un homomorphisme $ \beta : L(X) \to g $ dont la restriction à $ X = S \cup (X - S) $ est l’identité.

Montrons que $ \alpha $ est un isomorphisme, et $ \beta $ l’isomorphisme réciproque. Comme on a $ \psi(x) = x $ pour $ x $ dans $ X - S $, on voit que $ \alpha \circ \beta $ coïncide avec l’identité dans $ X $, d’où $ \alpha \circ \beta = \operatorname{Id}_{L(X)} $. On a par ailleurs $ [s, t] = d(s, t) $ dans $ g $ pour $ s \in S, t \in T $, par construction même; on en déduit que $ t = (s_1, \ldots, s_n, x) $ est égal dans $ g $ à $ (\operatorname{ad} s_1 \circ \cdots \circ \operatorname{ad} s_n)(x) $, d’où $ t = \beta(\alpha(s)) $. Comme on a $ \beta(\alpha(s)) = s $ pour $ s \in S $ et que $ S \cup T $ engendre $ g $, on a $ \beta \circ \alpha = \operatorname{Id}_g $.

Comme $ \alpha $ est un isomorphisme de $ g $ sur $ L(X) $, la prop. 9 montre que la restriction de $ \alpha $ à $ L(T) $ est un isomorphisme $ \varphi $ de $ L(T) $ sur un idéal $ b $ de $ L(X) $, tel que le module $ L(X) $ soit somme directe de $ L(S) $ et $ b $. On a évidemment
$$
\varphi(s_1, \ldots, s_n, x) = (\operatorname{ad} s_1 \circ \ldots \circ \operatorname{ad} s_n)(x)
$$
pour $ (s_1, \ldots, s_n, x) $ dans $ T $.

On a donc $ \varphi(T) \subset a $, d’où $ b \subset a $ puisque $ \varphi(T) $ engendre la sous-algèbre $ b $ de $ L(X) $. Mais $ b $ est un idéal et $ X - S \subset \varphi(T) \subset b $, d’où $ a \subset b $.

#### Corollaire {#lie-ii-s2-n9-cor-1 .statement}

Soit $ y \in X $. *L’algèbre de Lie libre* $ L(X) $ *est somme directe du sous-module libre* $ K.y $ *et de la sous-algèbre de Lie admettant comme famille basique la famille des* $ ((\operatorname{ad} y)^n.z) $ *pour* $ n \geqslant 0 $ *et* $ z \in X - \{y\} $.

Il suffit de faire $ S = \{y\} $ dans la prop. 10.

### 10. Ensembles de Hall dans un magma libre

Soient $ X $ un ensemble, $ M(X) $ le magma libre construit sur $ X $ et $ M^n(X) $, pour $ n \in \mathbf{N}^* $, l’ensemble des éléments de $ M(X) $ de longueur $ n $ (n° 1). Si $ w \in M(X) $ et $ l(w) \geqslant 2 $, on note $ \alpha(w) $ et $ \beta(w) $ les éléments de $ M(X) $ déterminés par la relation $ w = \alpha(w)\beta(w) $; on a $ l(\alpha(w)) < l(w) $, $ l(\beta(w)) < l(w) $. Enfin, pour $ u, v $ dans $ M(X) $, on note $ u^m v $ l’élément défini par récurrence sur l’entier $ m \geqslant 0 $ par $ u^0 v = v $ et $ u^{m+1} v = u(u^m v) $.

#### Définition 2 {#lie-ii-s2-def-2 .statement}

*On appelle* ensemble de Hall relatif à $ X $ *toute partie* $ H $ *de* $ M(X) $ *munie d’une relation d’ordre total satisfaisant aux conditions suivantes*:
(A) *Si* $ u \in H, v \in H $ *et* $ l(u) < l(v) $, *on a* $ u < v $.

(B) On a $ X \subset H $ et $ H \cap M^2(X) $ se compose des produits $ xy $ avec $ x, y $ dans $ X $ et $ x < y $.

(C) Un élément $ w $ de $ M(X) $ de longueur $ \geq 3 $ appartient à $ H $ si et seulement s’il est de la forme $ a(bc) $ avec $ a, b, c $ dans $ H $, $ bc \in H $, $ b \leq a < bc $ et $ b < c $.

#### Proposition 11 {#lie-ii-s2-prop-11 .statement}

Il existe un ensemble de Hall relatif à $ X $.

Nous allons construire par récurrence sur l’entier $ n \geq 1 $ des ensembles $ H_n \subset M^n(X) $ et une relation d’ordre total sur chacun de ces ensembles:

a) On pose $ H_1 = X $ et on le munit d’une relation d’ordre total.

b) L’ensemble $ H_2 $ se compose des produits $ xy $ avec $ x, y $ dans $ X $ et $ x < y $. On le munit d’un ordre total.

c) Soit $ n \geq 3 $ tel que les ensembles totalement ordonnés $ H_1, \ldots, H_{n-1} $ soient déjà définis. L’ensemble $ H'_{n-1} = H_1 \cup \cdots \cup H_{n-1} $ est muni de la relation d’ordre total qui induit les relations données sur $ H_1, \ldots, H_{n-1} $ et telle que l’on ait $ w < w' $ si $ l(w) < l(w') $. On définit $ H_n $ comme l’ensemble des produits $ a(bc) \in M^n(X) $ avec $ a, b, c $ dans $ H'_{n-1} $ satisfaisant aux relations $ bc \in H'_{n-1} $, $ b \leq a < bc $, $ b < c $ et on munit $ H_n $ d’une structure d’ordre total.

Posons $ H = \bigcup_{n \geq 1} H_n $; on munit $ H $ de l’ordre total défini ainsi : on a $ w \leq w' $ si et seulement si $ l(w) < l(w') $ ou bien $ l(w) = l(w') = n $ et $ w \leq w' $ dans l’ensemble $ H_n $. Il est immédiat que $ H $ est un ensemble de Hall relatif à $ X $.

Pour toute partie $ S $ de $ X $, nous identifions le magma libre $ M(S) $ à son image canonique dans $ M(X) $.

#### Proposition 12 {#lie-ii-s2-prop-12 .statement}

Soit $ H $ un ensemble de Hall relatif à $ X $ et soient $ x, y $ dans $ X $.

a) On a $ H \cap M(\{x\}) = \{x\} $.

b) Supposons $ x < y $ et soit $ d_y $ l’homomorphisme de $ M(X) $ dans $ \mathbf{N} $ tel que $ d_y(y) = 1 $ et $ d_y(z) = 0 $ pour $ z \in X, z \neq y $. L’ensemble des éléments $ w \in H \cap M(\{x, y\}) $ tels que $ d_y(w) = 1 $ se compose des éléments $ x^n y $ pour $ n $ entier $ \geq 0 $.

D’après la déf. 2 (B), on a $ x \in H $ et $ H \cap M^2(\{x\}) = \emptyset $. Si $ w \in H \cap M(\{x\}) $, avec $ n = l(w) \geq 3 $, les éléments $ \alpha(w) $ et $ \beta(w) $ appartiennent aussi à $ H \cap M(\{x\}) $ d’après la déf. 2 (C). On en déduit aussitôt par récurrence sur $ n $ que $ H \cap M^n(\{x\}) = \emptyset $ pour $ n \geq 2 $, d’où a).

Démontrons maintenant b). D’après la déf. 2 (B), on a $ y \in H $ et $ xy \in H $. Démontrons par récurrence sur $ n $ que $ x^n y \in H $ pour $ n $ entier $ \geq 2 $. On a $ x^n y = x(x(x^{n-2} y)) $ et l’hypothèse de récurrence entraîne que $ x^{n-2} y \in H $. On a $ l(x) < l(x^{n-2} y) $ pour $ n > 2 $ et $ x < y $, d’où $ x < x^{n-2} y $ dans tous les cas ; la condition (C) de la déf. 2 montre que $ x^n y \in H $. D’autre part, on a bien $ d_y(x^n y) = 1 $. Inversement, soit $ w \in H \cap M(\{x, y\}) $, avec $ d_y(w) = 1 $. Si $ l(w) = 1 $, on a $ w = y $; si $ l(w) = 2 $, on a $ w = xy $ d’après la déf. 2 (B). Si $ l(w) \geq 3 $, on a $ w = a(bc) $, avec $ a, b, c, bc $ dans $ H \cap M(\{x, y\}) $ (déf. 2 (C)). On ne peut pas avoir $ d_y(bc) = 0 $, car ceci entraînerait $ bc \in M(\{x\}) $, ce qui est impossible d’après a).

On a donc $ d_y(bc) = 1 $ et $ d_y(a) = 0 $, d’où $ a = x $ d’après $ a $. On en déduit aussitôt par récurrence sur $ n = l(w) $ que $ w = x^{n-1}y $, ce qui achève la démonstration de $ b $.

#### Corollaire {#lie-ii-s2-n10-cor-1 .statement}

Si Card $ X \geq 2 $, on a $ H \cap M^n(X) \neq \emptyset $, pour tout entier $ n \geq 1 $.

#### Proposition 13 {#lie-ii-s2-prop-13 .statement}

Soit $ X $ un ensemble fini possédant au moins deux éléments. On note $ H $ un ensemble de Hall relatif à $ X $. Il existe alors une bijection strictement croissante $ p \mapsto w_p $ de $ \mathbf{N} $ sur $ H $ et une suite $ (P_p)_{p \in \mathbf{N}} $ de parties de $ H $ avec les propriétés suivantes:
a) On a $ P_0 = X $.
b) Pour tout entier $ p \geq 0 $, on a $ w_p \in P_p $.
c) Pour tout entier $ n \geq 1 $, il existe un entier $ p(n) $ tel que tout élément de $ P_p $ soit de longueur $ > n $ pour tout $ p \geq p(n) $.
d) Pour tout entier $ p \geq 0 $, l’ensemble $ P_{p+1} $ se compose des éléments de la forme $ w_p^i w $ avec $ i \geq 0 $, $ w \in P_p $ et $ w \neq w_p $.

Comme $ X $ est fini, chacun des ensembles $ M^n(X) $ est fini. Posons $ H_n = H \cap M^n(X) $ pour tout $ n \geq 1 $. Le cor. de la prop. 12 montre que l’ensemble fini $ H_n $ est non vide. Soit $ u_n $ le cardinal de $ H_n $; posons $ v_0 = 0 $ et $ v_n = u_1 + \cdots + u_n $ pour $ n \geq 1 $. Comme $ H_n $ est un ensemble fini totalement ordonné, il existe une bijection strictement croissante $ p \mapsto w_p $ de l’intervalle $ [v_{n-1}, v_n - 1] $ de $ \mathbf{N} $ sur $ H_n $. Il est immédiat que $ p \mapsto w_p $ est une bijection strictement croissante de $ \mathbf{N} $ sur $ H $.

Posons $ P_0 = X $ et pour tout entier $ p \geq 1 $, soit $ P_p $ l’ensemble des éléments $ w $ de $ H $ tels que $ w \geq w_p $ et que l’on ait, ou bien $ w \in X $, ou bien $ \alpha(w) < w_p $ (remarquons que si $ w $ est de longueur $ \geq 2 $, la relation $ w \in H $ entraîne $ \alpha(w) \in H $ d’après la condition (C) de la déf. 2). On a $ w_p \in P_p $; cela est clair si $ w_p \in X $ et cela résulte de l’inégalité $ l(\alpha(w_p)) < l(w_p) $ et de la condition (A) de la déf. 2 lorsque $ w_p \notin X $.

Les conditions $ a) $ et $ b) $ sont donc satisfaites.

Soit $ n $ un entier $ \geq 1 $ et soit $ p \geq v_n $. Pour tout $ w \in P_p $, on a $ l(w) \geq l(w_p) > n $ d’après la définition même de l’application $ p \mapsto w_p $. Ceci établit $ c) $.

Montrons que tout élément de la forme $ u = w_p^i w $ avec $ i \geq 0 $, $ w \in P_p $ et $ w \neq w_p $ appartient à $ P_{p+1} $. Si $ i \neq 0 $, on a $ l(u) > l(w_p) $ d’où $ u > w_p $ et $ u \geq w_{p+1} $; on a $ u \notin X $ et $ \alpha(u) = w_p < w_{p+1} $, d’où $ u \in P_{p+1} $. Si $ i = 0 $, on a $ u \in P_p $ et $ u \neq w_p $; on a donc $ u > w_p $, d’où $ u \geq w_{p+1} $; si $ u $ n’appartient pas à $ X $, on a $ \alpha(w) < w_p $ d’où $ \alpha(w) < w_{p+1} $; on a encore $ u \in P_{p+1} $.

Réciproquement, soit $ u \in P_{p+1} $. Distinguons deux cas:
$ \alpha) $ Il n’existe aucun élément $ v $ de $ M(X) $ tel que $ u = w_p v $. Par définition de $ P_{p+1} $, on a $ u > w_p $. De plus, si $ u \notin X $, on a $ \alpha(u) \neq w_p $ par l’hypothèse faite, et l’on a $ \alpha(u) < w_{p+1} $ puisque $ u \in P_{p+1} $; donc $ \alpha(u) < w_p $. Donc on a $ u \in P_p $ et $ u \neq w_p $.
$ \beta) $ Il existe $ v $ dans $ M(X) $ tel que $ u = w_p v $. D’après la déf. 2, on a nécessairement, soit $ w_p \in X $, $ v \in X $ et $ w_p < v $, soit $ v \notin X $ et $ \alpha(v) \leq w_p < v $. Dans les deux eventualités, on a $ v \in P_{p+1} $.

Ceci posé, il existe un entier $ i \geq 0 $ et un élément $ w $ de $ M(X) $ tels que $ u = w_p^i w $, et ou bien $ w \in X $, ou bien $ w \notin X $ et $ \alpha(w) \neq w_p $. Si $ i = 0 $, on est dans le cas $ \alpha $) ci-dessus, d’où $ w \in P_p $ et $ w \neq w_p $. Si $ i > 0 $, la démonstration de $ \beta $) ci-dessus établit, par récurrence sur $ i $, les relations $ w \in P_{p+1} $ et $ w \neq w_p $. Supposons $ w \notin X $; de $ w \in P_{p+1} $ on déduit $ \alpha(w) \leq w_p $ et comme on a $ \alpha(w) \neq w_p $, on conclut que $ w \in P_p $. Ceci achève de prouver $ d $).

#### Exemple {#lie-ii-s2-n10-exa-1 .statement}

Supposons que $ X $ ait deux éléments $ x, y $; ordonnons $ X $ de telle sorte que l’on ait $ x < y $. La construction donnée dans la démonstration de la prop. 11 fournit un ensemble $ H $ qui a 14 éléments de longueur $ \leq 5 $ donnés dans le tableau suivant:

$$
\begin{array}{ll}
H_1 & w_1 = x \\
H_2 & w_3 = (xy) \\
H_3 & w_4 = (x(xy)) \\
H_4 & w_6 = (x(x(xy)))) \\
H_5 & w_9 = (x(x(x(xy)))) \\
w_{12} = (y(y(y(xy)))) \\
w_2 = y \\
w_5 = (y(xy)) \\
w_7 = (y(x(xy)))) \\
w_{10} = (y(x(x(xy)))) \\
w_{13} = ((xy)(x(xy))) \\
w_8 = (y(y(xy)))) \\
w_{11} = (y(y(x(xy)))) \\
w_{14} = ((xy)(y(xy))).
\end{array}
$$

(On a numéroté les éléments de $ H $ suivant les relations d’ordre total choisies dans chaque $ H_n $.)

### 11. Bases de Hall d’une algèbre de Lie libre

On conserve les notations du n° précédent.

#### Théorème 1 {#lie-ii-s2-thm-1 .statement}

*Soient $ H $ un ensemble de Hall relatif à $ X $ et $ \Psi $ l’application canonique de $ M(X) $ dans l’algèbre de Lie libre $ L(X) $. La restriction de $ \Psi $ à $ H $ est une base du module $ L(X) $.

Pour tout élément $ w $ de $ H $, on pose $ \overline{w} = \Psi(w) $.

A) *Cas où $ X $ est fini*.

Si $ X $ est vide, il en est de même de $ M(X) $ et donc de $ H $, et $ L(X) $ est réduit à 0. Si $ X $ a un seul élément $ x $, $ H \cap M^n(X) $ est vide pour $ n \geq 2 $ (prop. 12 a)). Par suite, on a $ H = \{x\} $; on sait aussi (n° 2, *Remarque*) que le module $ L(X) $ est libre de base $ \{\overline{x}\} $. Le théorème est donc vrai lorsque $ X $ a au plus un élément.

Supposons désormais que $ X $ ait au moins deux éléments; choisissons des suites $ (w_p) $ et $ (P_p) $ ayant les propriétés énoncées dans la prop. 13. Pour tout entier $ p \geq 0 $, on note $ L_p $ le sous-module de $ L(X) $ engendré par les éléments $ \overline{w}_i $ pour $ 0 \leq i < p $ et $ g_p $ la sous-algèbre de Lie de $ L(X) $ engendrée par la famille $ (\overline{u})_{u \in P_p} $.

#### Lemme 2 {#lie-ii-s2-lem-2 .statement}

*Pour tout entier $ p \geq 0 $, le module $ L_p $ admet la famille $ (\overline{w}_i)_{0 \leq i < p} $ pour base, l’algèbre de Lie $ g_p $ admet $ (\overline{u})_{u \in P_p} $ pour famille basique, et le module $ L(X) $ est somme directe de $ L_p $ et $ g_p $*.

On a $ L_0 = \{0\} $ et $ g_0 = L(X) $, et le lemme est vrai pour $ p = 0 $. Raisonnons par récurrence sur $ p $. Supposons donc que le lemme soit vrai pour un entier $ p \geq 0 $. Posons $ u_{i,w} = (\mathrm{ad}\ \overline{w}_p)^i.\overline{w} = \Psi(w_p^i w) $ pour $ i \geq 0, w \in P_p, w \neq w_p $. D’après le cor.

de la prop. 10 du n° 9, l’algèbre de Lie libre $ g_p $ est somme directe du module $ T_p $ de base $ \{ \overline{w}_p \} $ et d’une sous-algèbre de Lie $ h_p $ admettant $ \mathcal{F} = (u_{i,w})_{i \geq 0, w \in P_p, w \neq w_p} $ pour famille basique. D’après la prop. 13d), la famille $ (\overline{u})_{u \in P_{p+1}} $ est égale à $ \mathcal{F} $, donc est une famille basique de $ h_p = g_{p+1} $. On a donc $ L(X) = L_p \oplus T_p \oplus g_{p+1} $ et comme $ L_{p+1} = L_p + T_p $, on a $ L(X) = L_{p+1} \oplus g_{p+1} $ et $ (\overline{w}_0, \overline{w}_1, \ldots, \overline{w}_{p-1}, \overline{w}_p) $ est une base du module $ L_{p+1} $.

C.Q.F.D.

Soit $ n $ un entier positif. D’après la prop. 13c), il existe un entier $ p(n) $ tel que $ P_p $ n’ait que des éléments de longueur $ > n $ pour $ p \geq p(n) $. Pour $ p \geq p(n) $, la sous-algèbre de Lie $ g_p $ de $ L(X) $ est engendrée par des éléments de degré $ > n $, donc $ L^n(X) \cap g_p = \{0\} $. Par ailleurs, les éléments $ \overline{w}_i $ de $ L(X) $ sont homogènes et la famille $ (\overline{w}_i)_{0 \leq i < p} $ est une base d’un module supplémentaire de $ g_p $. Il en résulte immédiatement que la famille des éléments $ \overline{w}_i $ de degré $ n $ est une base du module $ L^n(X) $, et que la suite $ (\overline{w}_i)_{i \geq 0} $ est une base du module $ L(X) $.

B) *Cas général*.

Si $ S $ est une partie de $ X $, rappelons que $ M(S) $ est identifié au sous-magma de $ M(X) $ engendré par $ S $ et $ L(S) $ est identifiée à la sous-algèbre de Lie de $ L(X) $ engendrée par $ S $; on a vu que si $ w \in M(S) $ est de longueur $ \geq 2 $, on a $ \alpha(w) \in M(S) $ et $ \beta(w) \in M(S) $. Il en résulte immédiatement que $ H \cap M(S) $ est un ensemble de Hall relatif à $ S $.

Pour toute partie finie $ \Phi $ de $ H $, il existe une partie finie $ S $ de $ X $ telle que $ \Phi \subset M(S) $. Le cas A) montre alors que les éléments $ \overline{w} $ pour $ w \in \Phi $ sont linéairement indépendants dans $ L(S) $, donc dans $ L(X) $. Par suite, la famille $ (\overline{w})_{w \in H} $ est libre.

Pour tout élément $ a $ de $ L(X) $, il existe une partie finie $ S $ de $ X $ telle que $ a \in L(S) $. D’après le cas A), la partie $ \Psi'(H \cap M(S)) $ de $ \Psi'(H) $ engendre le module $ L(S) $, donc $ a $ est combinaison linéaire d’éléments de $ \Psi'(H) $. Donc $ \Psi'(H) $ engendre le module $ L(X) $, ce qui achève la démonstration.

#### Corollaire {#lie-ii-s2-n11-cor-1 .statement}

*Le module* $ L(X) $ *est libre, ainsi que chacun des sous-modules* $ L^\alpha(X) $ *pour* $ \alpha \in \mathbf{N}^{(X)} $ *et* $ L^n(X) $ *pour* $ n \in \mathbf{N} $. *Les modules* $ L^\alpha(X) $ *sont de rang fini, et il en est de même des modules* $ L^n(X) $ *si* $ X $ *est fini*.

Il existe un ensemble de Hall $ H $ relatif à $ X $ (prop. 11). Pour tout $ w \in H $, l’élément $ \Psi(w) $ de $ L(X) $ appartient à l’un des modules $ L^\alpha(X) $ (avec $ \alpha \in \mathbf{N}^{(X)} $), et le module $ L(X) $ est somme des sous-modules $ L^\alpha(X) $. De plus, pour tout $ \alpha \in \mathbf{N}^{(X)} $, l’ensemble des éléments de $ M(X) $ dont l’image canonique dans $ \mathbf{N}^{(X)} $ est égale à $ \alpha $ est fini; ceci montre que chacun des modules $ L^\alpha(X) $ est libre de rang fini, et que $ L(X) $ est libre. On a $ L^n(X) = \sum_{|\alpha|=n} L^\alpha(X) $, donc $ L^n(X) $ est libre; lorsque $ X $ est fini, l’ensemble des $ \alpha \in \mathbf{N}^{(X)} $ tels que $ |\alpha|=n $ est fini, donc $ L^n(X) $ est alors de rang fini.

#### Définition 3 {#lie-ii-s2-def-3 .statement}

On appelle base de Hall d’une algèbre de Lie libre $ L(X) $ toute base de $ L(X) $ qui est l’image canonique d’un ensemble de Hall relatif à $ X $.

#### Remarque {#lie-ii-s2-n11-rem-1 .statement}

Supposons que $ X $ se compose de deux éléments distincts $ x $ et $ y $ et soit $ L^{(1)} $ le sous-module de $ L(X) $ somme des $ L^\alpha(X) $ pour $ \alpha \in \mathbf{N}^X $, avec $ \alpha(y) = 1 $. On déduit aussitôt du th. 1 et de la prop. 12 du n° 10 que les éléments $ (\mathrm{ad}\,x)^n.y $ pour $ n $ entier $ \geqslant 0 $ forment une base du sous-module $ L^{(1)} $. Il en résulte que la restriction à $ L^{(1)} $ de l’application $ \mathrm{ad}\,x $ est injective.

## EXERCICES {#lie-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
