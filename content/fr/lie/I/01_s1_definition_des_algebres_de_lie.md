---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Algèbres de Lie
section: 1
section_title: Définition des algèbres de Lie
lang: fr
source: lie-i-fr
pdf_pages: 0005-0019, 0099-0108
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres
      page: 0
      pdf_page: 5
    - "no": 2
      title: Algèbres de Lie
      page: 0
      pdf_page: 7
    - "no": 3
      title: Algèbres de Lie commutatives
      page: 0
      pdf_page: 10
    - "no": 4
      title: Idéaux
      page: 0
      pdf_page: 10
    - "no": 5
      title: Série dérivée, série centrale descendante
      page: 0
      pdf_page: 11
    - "no": 6
      title: Série centrale ascendante
      page: 0
      pdf_page: 12
    - "no": 7
      title: Extensions
      page: 0
      pdf_page: 13
    - "no": 8
      title: Produits semi-directs
      page: 0
      pdf_page: 15
    - "no": 9
      title: Changement de l’anneau de base
      page: 0
      pdf_page: 19
statements: 21
exercises: 27
content_sha256: f9553c57b1a48fa1515184945910960cc3c2f3548c230c2ad8aac6ec385c693b
---

## § 1. Définition des algèbres de Lie

### 1. Algèbres

Soit M un module unitaire sur K, muni d’une application bilinéaire $(x, y) \mapsto xy$ de $M \times M$ dans M. Tous les axiomes des algèbres sont vérifiés à l’exception de l’associativité de la multiplication. Par abus de langage, on dit que M est une algèbre non nécessairement associative sur K, ou parfois, quand aucune confusion ne peut en résulter, une algèbre sur K. Dans le présent no, nous emploierons cette dernière terminologie.

Si on munit le K-module M de la multiplication $(x, y) \mapsto yx$, on obtient encore une algèbre qui est dite opposée à l’algèbre précédente.

Un sous-K-module N de M stable pour la multiplication est muni de manière évidente d’une structure d’algèbre sur K. On

¹ Les propositions démontrées dans ce Chapitre s’appuient exclusivement sur les propriétés établies dans les livres I à VI, et sur quelques résultats de Alg. comm., chap. III, § 2.

dit que N est une sous-algèbre de M. On dit que N est un idéal à gauche (resp. à droite) de M si les conditions $x \in N,\ y \in M$ entraînent $yx \in N$ (resp. $xy \in N$). Si N est à la fois un idéal à gauche et un idéal à droite, on dit que N est un idéal bilatère de M. Dans ce cas, la multiplication dans M permet de définir, par passage au quotient, une multiplication bilinéaire dans le module quotient $M/N$, de sorte que $M/N$ est muni d’une structure d’algèbre. On dit que $M/N$ est l’algèbre quotient de M par N.

Soient $M_1$ et $M_2$ deux algèbres sur K, et $\varphi$ une application de $M_1$ dans $M_2$. On dit que $\varphi$ est un homomorphisme si $\varphi$ est K-linéaire, et si $\varphi(xy) = \varphi(x)\varphi(y)$ pour $x \in M_1,\ y \in M_1$. Le noyau de $\varphi$ est un idéal bilatère de $M_1$, et l’image de $\varphi$ est une sous-algèbre de $M_2$. Par passage au quotient, $\varphi$ définit un isomorphisme de l’algèbre $M_1/N$ sur l’algèbre $\varphi(M_1)$.

Soit M une algèbre sur K. Une application D de M dans M est appelée une dérivation de M si elle est K-linéaire et si $D(xy) = (Dx)y + x(Dy)$, quels que soient $x \in M$ et $y \in M$. Cette définition généralise la déf. 3 d’Alg., chap. IV, § 4, no 3. Le noyau d’une dérivation de M est une sous-algèbre de M. Si $D_1$ et $D_2$ sont des dérivations de M, alors $D_1D_2 - D_2D_1$ est une dérivation de M (cf. Alg., chap. IV, § 4, no 3, prop. 5 : la démonstration de cette proposition n’utilise pas l’associativité de l’algèbre).

Soient $M_1$ et $M_2$ deux algèbres sur K. Sur le K-module produit $M = M_1 \times M_2$, définissons une multiplication en posant $(x_1, x_2)(y_1, y_2) = (x_1y_1, x_2y_2)$, quels que soient $x_1, y_1$ dans $M_1$, $x_2, y_2$ dans $M_2$. L’algèbre ainsi définie s’appelle l’algèbre produit de $M_1$ et $M_2$. L’application $x_1 \mapsto (x_1, 0)$ (resp. $x_2 \mapsto (0, x_2)$) est un isomorphisme de $M_1$ (resp. $M_2$) sur un idéal bilatère de M. Par ces isomorphismes, on identifie $M_1$ et $M_2$ à des idéaux bilatères de M. Le K-module M est alors somme directe de $M_1$ et $M_2$. Réciproquement, soient M une algèbre sur K, et $M_1, M_2$ deux idéaux bilatères de M tels que M soit la somme directe de $M_1$ et $M_2$. On a $M_1M_2 \subset M_1 \cap M_2 = \{0\}$; donc, si $x_1, y_1$ appartiennent à $M_1$ et $x_2, y_2$ à $M_2$, alors $(x_1 + x_2)(y_1 + y_2) = x_1y_1 + x_2y_2$, de sorte que M s’identifie à l’algèbre produit $M_1 \times M_2$. Tout idéal à gauche (resp. à droite, bilatère) de $M_1$ est un idéal à gauche (resp. à droite, bilatère) de M. Nous laissons au lecteur le soin de formuler les résultats analogues dans le cas d’une famille finie quelconque d’algèbres.

Soit M une algèbre sur K, et supposons que le K-module M admette une base $(a_\lambda)_{\lambda \in L}$. Il existe un système unique $(\gamma_{\lambda \mu \nu})_{(\lambda, \mu, \nu) \in L \times L \times L}$ d’éléments de K tels que $a_\lambda a_\mu = \sum_\nu \gamma_{\lambda \mu \nu} a_\nu$ quels que soient $\lambda, \mu$ dans L. Les $\gamma_{\lambda \mu \nu}$ s’appellent les constantes de structure de M par rapport à la base $(a_\lambda)$.

Soient M une algèbre sur K, $K_0$ un anneau commutatif ayant un élément unité, $\rho$ un homomorphisme de $K_0$ dans K transformant l’élément unité en élément unité. Alors, M peut être considéré comme algèbre sur $K_0$ en posant $\alpha . x = \rho(\alpha) . x$ pour $\alpha \in K_0, x \in M$. Il en est ainsi, en particulier, lorsqu’on prend pour $K_0$ un sous-anneau de K contenant l’élément unité, et pour $\rho$ l’application identique de $K_0$ dans K.

Soient M une algèbre sur K, $K_1$ un anneau commutatif ayant un élément unité, $\sigma$ un homomorphisme de K dans $K_1$ transformant l’élément unité en élément unité. Soit $M_{(K_1, \sigma)} = M_{(K_1)}$ le $K_1$-module déduit de M par extension à $K_1$ de l’anneau des scalaires (Alg., chap. II, 3e éd., § 5). Le produit dans M définit canoniquement une application $K_1$-bilinéaire de $M_{(K_1)} \times M_{(K_1)}$ dans $M_{(K_1)}$ (Alg., chap. IX, § 1, no 4), de sorte que $M_{(K_1)}$ se trouve muni d’une structure d’algèbre sur $K_1$ (qui est dite déduite de M par extension à $K_1$ de l’anneau des scalaires). Il en est ainsi, en particulier, lorsque K est un sous-anneau de $K_1$ contenant l’élément unité et que $\sigma$ est l’application identique de K dans $K_1$.

### 2. Algèbres de Lie

#### Définition 1 {#lie-i-s1-def-1 .statement}

Une algèbre g sur K est appelée une algèbre de Lie sur K si sa multiplication (notée $(x, y) \mapsto [x, y]$) vérifie les identités :
(1) $[x, x] = 0$
(2) $[x, [y, z]] + [y, [z, x]] + [z, [x, y]] = 0$
quels que soient $x, y, z$ dans g.

Le produit $[x, y]$ est appelé le crochet de $x$ et $y$. L’identité (2) est appelée l’identité de Jacobi.

Le crochet $[x, y]$ est une fonction bilinéaire alternée de $x, y$. On a donc l’identité :

(3)
$$
[x, y] = -[y, x]
$$
de sorte que l’identité de Jacobi peut s’écrire :
(4)
$$
[x, [y, z]] = [[x, y], z] + [y, [x, z]].
$$

Toute sous-algèbre, toute algèbre quotient d’une algèbre de Lie sont des algèbres de Lie. Tout produit d’algèbres de Lie est une algèbre de Lie. Si $g$ est une algèbre de Lie, l’algèbre opposée $g^0$ est une algèbre de Lie, et l’application $x \mapsto -x$ est un isomorphisme de $g$ sur $g^0$, en vertu de l’identité (3).

#### Exemple 1 {#lie-i-s1-n2-exa-1 .statement}

Soit $L$ une algèbre associative sur $K$. Le crochet $[x, y] = xy - yx$ est une fonction bilinéaire de $x$ et $y$. On véri fie facilement que la loi de composition $(x, y) \mapsto [x, y]$ dans le $K$-module $L$ fait de $L$ une algèbre de Lie sur $K$.

#### Exemple 2 {#lie-i-s1-n2-exa-2 .statement}

Dans l’exemple 1, choisissons pour $L$ l’algèbre associative des endomorphismes d’un $K$-module $E$. On obtient l’algèbre de *Lie des endomorphismes de* $E$, notée $\mathrm{gl}(E)$. (Si $E = K^n$, on note $\mathrm{gl}(n, K)$ l’algèbre de Lie $\mathrm{gl}(E)$.)

Toute sous-algèbre de Lie de $\mathrm{gl}(E)$ est une algèbre de Lie sur $K$. En particulier :

1° Si $E$ est muni d’une structure d’algèbre (non nécessairement associative), les dérivations de $E$ forment une algèbre de Lie sur $K$.

2° Si $E$ admet une base finie, les endomorphismes de $E$ de trace nulle forment une algèbre de Lie sur $K$, qu’on désigne par $\mathfrak{sl}(E)$ (ou par $\mathfrak{sl}(n, K)$ si $E = K^n$).

3° L’ensemble $\mathbf{M}_n(K)$ des matrices carrées d’ordre $n$ peut être considéré comme une algèbre de Lie sur $K$ canoniquement isomorphe à $\mathrm{gl}(n, K)$. Soit $(E_{ij})$ la base canonique de $\mathbf{M}_n(K)$ (*Alg.*, chap. II, 3e éd., § 10, no 3). On a facilement :

(5)
$$
\begin{cases}
[E_{ij}, E_{kl}] = 0 & \text{si } j \neq k \quad \text{et} \quad i \neq l \\
[E_{ij}, E_{\eta l}] = E_{i\eta} & \text{si } i \neq l \\
[E_{ij}, E_{ki}] = -E_{kj} & \text{si } j \neq k \\
[E_{ij}, E_{\eta i}] = E_{i\eta} - E_{\eta i}
\end{cases}
$$

\* Exemple 3. — Soit V une variété indéfiniment différentiable réelle. Les opérateurs différentiels à coefficients réels indéfiniment différentiables sur V constituent une algèbre associative sur $\mathbf{R}$, donc, d’après l’exemple 1, une algèbre de Lie $\Delta$ sur $\mathbf{R}$. Le crochet de deux champs de vecteurs indéfiniment différentiables sur V est un champ de vecteurs indéfiniment différentiable, donc les champs de vecteurs indéfiniment différentiables sur V constituent une sous-algèbre de Lie $\mathfrak{f}$ de $\Delta$. Si V est un groupe de Lie réel, les champs de vecteurs invariants à gauche constituent une sous-algèbre de Lie g de $\mathfrak{f}$ appelée algèbre de Lie de V. L’espace vectoriel g s’identifie à l’espace tangent à V en e (élément neutre de V). Soient V’ un autre groupe de Lie réel, $e'$ son élément neutre, g’ son algèbre de Lie. Tout homomorphisme analytique de V dans V’ définit une application linéaire de l’espace tangent à V en e dans l’espace tangent à V’ en $e'$; cette application est un homomorphisme de l’algèbre de Lie g dans l’algèbre de Lie g’. Si V est le groupe linéaire d’un espace vectoriel réel E de dimension finie, il existe un isomorphisme canonique de gl(E) sur l’algèbre de Lie g de V, par lequel on identifie g et gl(E).*

#### Définition 2 {#lie-i-s1-def-2 .statement}

Soient g une algèbre de Lie, x un élément de g. L’application linéaire $y \mapsto [x, y]$ de g dans g s’appelle l’application linéaire adjointe de x et se désigne par $\operatorname{ad}_g x$ ou par $\operatorname{ad} x$.

#### Proposition 1 {#lie-i-s1-prop-1 .statement}

Soit g une algèbre de Lie. Pour tout $x \in g$, $\operatorname{ad} x$ est une dérivation de g. L’application $x \mapsto \operatorname{ad} x$ est un homomorphisme de l’algèbre de Lie g dans l’algèbre de Lie $\mathfrak{D}$ des dérivations de g. Si $D \in \mathfrak{D}$ et $x \in g$, on a $[D, \operatorname{ad} x] = \operatorname{ad} (Dx)$.

En effet, l’identité (4) peut s’écrire :

$$
(\operatorname{ad} x) \cdot [y, z] = [(\operatorname{ad} x) \cdot y, z] + [y, (\operatorname{ad} x) \cdot z]
$$

ou :

$$
(\operatorname{ad} [x, y]) \cdot z = (\operatorname{ad} x) \cdot ((\operatorname{ad} y) \cdot z) - (\operatorname{ad} y) \cdot ((\operatorname{ad} x) \cdot z)
$$

d’où les deux premières assertions. D’autre part, si $D \in \mathfrak{d}$, $x \in g$, $y \in g$, on a $[D, \operatorname{ad} x].y = D([x, y]) - [x, Dy] = [Dx, y] = (\operatorname{ad} Dx).y$, d’où la dernière assertion.

L’application $\operatorname{ad} x$ s’appelle aussi la *dérivation intérieure* définie par $x$.

### 3. Algèbres de Lie commutatives

#### Définition 3 {#lie-i-s1-def-3 .statement}

*Deux éléments $x, y$ d’une algèbre de Lie sont dits permutables lorsque $[x, y] = 0$. On dit que $g$ est commutative si deux quelconques de ses éléments sont permutables.*

#### Exemple 1 {#lie-i-s1-n3-exa-1 .statement}

Soient $L$ une algèbre associative, $g$ l’algèbre de Lie qu’elle définit (n° 2, *Exemple 1*). Deux éléments $x, y$ sont permutables dans $g$ si et seulement si $xy = yx$ dans $L$.

#### Exemple 2 {#lie-i-s1-n3-exa-2 .statement}

Si un groupe de Lie réel $G$ est commutatif, son algèbre de Lie est commutative. \*

Tout $K$-module peut évidemment être muni, d’une manière unique, d’une structure d’algèbre de Lie commutative sur $K$.

Si $g$ est une algèbre de Lie, tout sous-module monogène de $g$ est une sous-algèbre de Lie commutative de $g$.

### 4. Idéaux

Il résulte de l’identité (3) que, dans une algèbre de Lie $g$, il n’y a pas à distinguer entre les idéaux à gauche et les idéaux à droite, tout idéal étant bilatère. On parlera donc simplement d’idéal.

#### Exemple {#lie-i-s1-n4-exa-1 .statement}

Soient $G$ un groupe de Lie, $g$ son algèbre de Lie, $H$ un sous-groupe de Lie de $G$. Tout champ de vecteurs invariant à gauche sur $H$ définit canoniquement un champ de vecteurs invariant à gauche sur $G$, d’où une injection canonique de l’algèbre de Lie $\mathfrak{h}$ de $H$ dans $g$; on identifie $\mathfrak{h}$ à une sous-algèbre de Lie de $g$ par cette injection. Si $H$ est distingué dans $G$, l’image canonique de $\mathfrak{h}$ dans $g$ est un idéal de $g$.*

Un idéal de g est un sous-module de g stable pour les dérivations intérieures de g.

#### Définition 4 {#lie-i-s1-def-4 .statement}

Un sous-module de g stable pour toute dérivation de g est appelé un idéal caractéristique de g.

#### Proposition 2 {#lie-i-s1-prop-2 .statement}

Soient g une algèbre de Lie, a un idéal (resp. un idéal caractéristique) de g, et b un idéal caractéristique de a. Alors, b est un idéal (resp. un idéal caractéristique) de g.
En effet, toute dérivation intérieure (resp. toute dérivation) de g laisse stable a et induit dans a une dérivation, donc laisse stable b.

Soient g une algèbre de Lie. Si a et b sont des idéaux de g, a + b et a ∩ b sont des idéaux de g.
Soient a et b deux sous-modules de g. Par abus de notations, on notera [a, b] le sous-module de g engendré par les éléments de la forme [x, y] (x ∈ a, y ∈ b). On a [a, b] = [b, a] d’après l’identité (3). Si z ∈ g, on note [z, a], ou [a, z], le sous-module [Kz, a] = (ad z)(a).

#### Proposition 3 {#lie-i-s1-prop-3 .statement}

Si a et b sont des idéaux (resp. des idéaux caractéristiques) de g, [a, b] est un idéal (resp. un idéal caractéristique) de g.
En effet, soit D une dérivation intérieure (resp. une dérivation quelconque) de g. Si x ∈ a et y ∈ b, on a
$$
D([x, y]) = [Dx, y] + [x, Dy] \in [a, b].
$$
D’où la proposition.

Si a est un sous-module de g, l’ensemble des x ∈ g tels que (ad x).a ⊂ a est une sous-algèbre n de g, appelée normalisateur de a dans g. Si de plus a est une sous-algèbre de g, on a a ⊂ n, et a est un idéal de n.

### 5. Série dérivée, série centrale descendante

On appelle idéal dérivé d’une algèbre de Lie g, et on note $\mathcal{O}g$, l’idéal caractéristique [g, g].
Tout sous-module de g contenant $\mathcal{O}g$ est un idéal de g.

On appelle série dérivée de g la suite décroissante $\mathcal{O}^0g, \mathcal{O}^1g, \ldots$ d’idéaux caractéristiques de g définis par récurrence de la manière suivante : 1) $\mathcal{O}^0g = g$; 2) $\mathcal{O}^{p+1}g = [\mathcal{O}^p g, \mathcal{O}^p g]$.

On appelle série centrale descendante de g la suite décroissante $C^1g, C^2g, \ldots$ d’idéaux caractéristiques de g définis par récurrence de la manière suivante : 1) $C^1g = g$; 2) $C^{p+1}g = [g, C^p g]$. On a $C^2g = \mathcal{O}g$, et $C^{p+1}g \supset \mathcal{O}^p g$ pour tout $p$, comme on le voit aussitôt par récurrence sur $p$.

#### Proposition 4 {#lie-i-s1-prop-4 .statement}

*Soient g et h deux algèbres de Lie sur K, et f un homomorphisme de g sur h. On a $f(\mathcal{O}^p g) = \mathcal{O}^p h, f(C^p g) = C^p h$. Si a et b sont des sous-modules de g, on a aussitôt $f([a, b]) = [f(a), f(b)]$.* La proposition est alors immédiate par récurrence sur $p$.

#### Corollaire {#lie-i-s1-n5-cor-1 .statement}

*Soient g une algèbre de Lie, a un idéal de g. Pour que l’algèbre de Lie $g/a$ soit commutative, il faut et il suffit que $a \supset \mathcal{O}g$.*

En effet, dire que $g/a$ est commutative revient à dire que $\mathcal{O}(g/a) = \{ 0 \}$. Or, $\mathcal{O}(g/a)$ est, d’après la prop. 4, l’image canonique de $\mathcal{O}g$ dans $g/a$.

### 6. Série centrale ascendante

Soient g une algèbre de Lie, et P une partie de g. On appelle commutant de P dans g l’ensemble des éléments de g permutables à ceux de P. Ce commutant est l’intersection des noyaux des ad $y$, où $y$ parcourt P ; c’est donc une sous-algèbre de g.

#### Proposition 5 {#lie-i-s1-prop-5 .statement}

*Soient g une algèbre de Lie, a un idéal (resp. un idéal caractéristique) de g. Le commutant $a'$ de a dans g est un idéal (resp. un idéal caractéristique) de g.*

En effet, soit D une dérivation intérieure (resp. une dérivation quelconque) de g. Si $x \in a'$ et $y \in a$, on a
$$
[Dx, y] = D([x, y]) - [x, Dy] = 0;
$$
donc $Dx \in a'$. D’où la proposition.

Soit g une algèbre de Lie. On appelle centre de g le commutant de g dans g, c’est-à-dire l’idéal caractéristique des $x \in g$ tels que $[x, y] = 0$ pour tout $y \in g$. Le centre de g est le noyau de l’homomorphisme $x \mapsto \mathrm{ad}\, x$.

On appelle série centrale ascendante de g la suite croissante $C_0g, C_1g, \ldots$ d’idéaux caractéristiques de g définis par récurrence de la manière suivante : 1) $C_0g = \{0\}$; 2) $C_{p+1}g$ est l’image réciproque, pour l’application canonique de g sur $g/C_pg$, du centre de $g/C_pg$.

L’idéal $C_1g$ est le centre de g.

### 7. Extensions

#### Définition 5 {#lie-i-s1-def-5 .statement}

Soient a et b deux algèbres de Lie sur K. On appelle extension de b par a une suite :

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

où g est une algèbre de Lie sur K, où $\mu$ est un homomorphisme surjectif de g sur b, et où $\lambda$ est un homomorphisme injectif de a sur le noyau de $\mu$.

Le noyau n de $\mu$ s’appelle le noyau de l’extension. L’homomorphisme $\lambda$ est un isomorphisme de a sur n et l’homomorphisme $\mu$ définit un isomorphisme de $g/n$ sur b par passage au quotient.

Par abus de langage, on dit aussi que g est extension de b par a.

Deux extensions :

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b, \quad a \xrightarrow{\lambda'} g' \xrightarrow{\mu'} b
$$

sont dites équivalentes s’il existe un homomorphisme f de g dans g' tel que le diagramme suivant :

$$
\begin{array}{ccc}
& & g \\
& \nearrow_{\lambda} & \downarrow \\
a & \xrightarrow{f} & g' \\
& \searrow_{\lambda'} & \uparrow_{\mu'} \\
& & b
\end{array}
$$

soit commutatif (c’est-à-dire tel que $f \circ \lambda = \lambda', \mu' \circ f = \mu$). Montrons qu’un tel homomorphisme est nécessairement bijectif.

D’abord $f$ est injectif. En effet, si $x \in g$ est tel que $f(x) = 0$, on a $\mu(x) = \mu'(f(x)) = 0$, donc $x = \lambda(y)$ avec un $y \in a$; et $\lambda'(y) = f(\lambda(y)) = f(x) = 0$, donc $y = 0$, donc $x = 0$. D’autre part, $f$ est surjectif. En effet $\mu' \circ f = \mu$ est surjectif, donc $f(g) + \lambda'(a) = g'$; et par ailleurs $f(g) \supset f(\lambda(a)) = \lambda'(a)$.

Il résulte de là que la relation qu’on vient de définir entre deux extensions de $b$ par $a$ est une *relation d’équivalence*.

#### Proposition 6 {#lie-i-s1-prop-6 .statement}

*Soient*:

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*une extension de b par a*, *et n son noyau*.

a) *S’il existe une sous-algèbre m de g supplémentaire de n dans g, la restriction de $\mu$ à m est un isomorphisme de m sur b. Si $\nu$ désigne l’isomorphisme réciproque de cette restriction, $\nu$ est un homomorphisme de b dans g, et $\mu \circ \nu$ est l’automorphisme identique de b*.

b) *Réciproquement, s’il existe un homomorphisme $\nu$ de b dans g tel que $\mu \circ \nu$ soit l’automorphisme identique de b, alors $\nu(b)$ est une sous-algèbre supplémentaire de n dans g*.

Les assertions de a) sont immédiates. D’autre part, soit $\nu$ un homomorphisme de b dans g tel que $\mu \circ \nu$ soit l’automorphisme identique de b. Alors, $\nu(b)$ est une sous-algèbre de g, et g est somme directe de $\nu(b)$ et de $\bar{\mu}'(0) = n$ (*Alg.*, chap. VIII, § 1, no 1).

#### Définition 6 {#lie-i-s1-def-6 .statement}

*Soient*:

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*une extension de b par a*, *et n son noyau*. *On dit que cette extension est inessentielle* (resp. *triviale*) *s’il existe une sous-algèbre* (resp. *un idéal*) *de g supplémentaire de n dans g*. *On dit que cette extension est centrale si n est contenu dans le centre de g*.

Si l’extension est triviale, soit m un idéal de g supplémentaire de n dans g. Alors (cf. no 1) g s’identifie canoniquement à l’algèbre de Lie $m \times n$, donc à l’algèbre de Lie $a \times b$. Réciproquement, soient a et b deux algèbres de Lie ; alors $a \times b$ est extension triviale de a par b.

Une extension centrale et inessentielle est triviale. En effet, soient $g$ une algèbre de Lie, $n$ un idéal de $g$ contenu dans le centre de $g$, et $m$ une sous-algèbre de $g$ supplémentaire de $n$ dans $g$. On a $[m, g] = [m, m] + [m, n] = [m, m] \subset m$, donc $m$ est un idéal de $g$.

### 8. Produits semi-directs

Soient $a$ et $b$ deux algèbres de Lie sur $K$. Il n’est pas facile de construire toutes les extensions de $b$ par $a$. Mais nous allons décrire assez simplement les extensions inessentielles de $b$ par $a$.

Soit $g$ une extension inessentielle de $b$ par $a$. Identifions $a$ à un idéal de $g$, $b$ à une sous-algèbre de $g$ supplémentaire de $a$, et le module $g$ au module $a \times b$. Pour tout $b \in b$, soit $\varphi_b$ la restriction à $a$ de $\mathrm{ad}_g b$; c’est une dérivation de $a$, et l’application $b \mapsto \varphi_b$ est un homomorphisme de $b$ dans l’algèbre de Lie des dérivations de $a$. D’autre part, pour $a, a'$ dans $a$ et $b, b'$ dans $b$, on a :

(6)
$$
[(a, b), (a', b')] = [a + b, a' + b']
= [a, a'] + [a, b'] + [b, a'] + [b, b']
= ([a, a'] + \varphi_b a' - \varphi_{b'} a, [b, b']).
$$

Réciproquement, soient $a$ et $b$ des algèbres de Lie sur $K$, et $b \mapsto \varphi_b$ un homomorphisme de $b$ dans l’algèbre de Lie des dérivations de $a$. Dans le produit $g$ des $K$-modules $a$ et $b$, définissons le crochet de deux éléments en posant :
$$
[(a, b), (a', b')] = ([a, a'] + \varphi_b a' - \varphi_{b'} a, [b, b'])
$$
quels que soient $a, a'$ dans $a$, $b, b'$ dans $b$. Il est immédiat que ce crochet est une fonction bilinéaire et alternée de $(a, b), (a', b')$; montrons que, étant donnés 3 éléments $(a, b), (a', b'), (a'', b'')$ de $a \times b$, on a :

(7)
$$
[(a, b), [(a', b'), (a'', b'')]] + [(a', b'), [(a'', b''), (a, b)]]
+ [(a'', b''), [(a, b), (a', b')]] = 0.
$$

Comme le premier membre de (7) est une fonction trilinéaire alternée de $(a, b), (a', b'), (a'', b'')$, il suffit de faire la vérification quand ce système d’éléments a l’une des formes suivantes :

(8) $(a, 0), (a', 0), (a'', 0)$
(9) $(a, 0), (a', 0), (0, b'')$
(10) $(a, 0), (0, b'), (0, b'')$
(11) $(0, b), (0, b'), (0, b'')$.

Dans les cas (8) et (11), la relation (7) est conséquence immédiate de l’identité de Jacobi dans $a$ et $b$. Dans le cas (9), on a

$$
[(a, 0), [(a', 0), (0, b'')]] = [(a, 0), (-\varphi_{b''}a', 0)] = (-[a, \varphi_{b''}a'], 0)
$$
$$
[(a', 0), [(0, b''), (a, 0)]] = [(a', 0), (\varphi_{b''}a, 0)] = ([a', \varphi_{b''}a]), 0)
$$
$$
[(0, b''), [(a, 0), (a', 0)]] = [(0, b''), ([a, a'], 0)] = (\varphi_{b''}([a, a']), 0)
$$

et la relation (7) résulte de l’égalité :

$$
\varphi_{b''}([a, a']) = [\varphi_{b''}a, a'] + [a, \varphi_{b''}a']
$$

Dans le cas (10), on a :

$$
[(a, 0), [(0, b'), (0, b'')]] = [(a, 0), (0, [b', b''])] = (-\varphi_{[b', b'']}a, 0)
$$
$$
[(0, b'), [(0, b''), (a, 0)]] = [(0, b'), (\varphi_{b''}a, 0)] = (\varphi_{b'}\varphi_{b''}a, 0)
$$
$$
[(0, b''), [(a, 0), (0, b')]] = [(0, b''), (-\varphi_{b'}a, 0)] = (-\varphi_{b''}\varphi_{b'}a, 0)
$$

et la relation (7) résulte de l’égalité :

$$
\varphi_{[b', b'']} = \varphi_{b'}\varphi_{b''} - \varphi_{b''}\varphi_{b'}
$$

On a donc défini une structure d’algèbre de Lie sur $g$. L’application $(a, b) \mapsto b$ de $g$ sur $b$ est un homomorphisme $\mu$, dont le noyau $n$ est l’idéal des éléments de $g$ de la forme $(a, 0)$. L’application $a \mapsto (a, 0)$ est un isomorphisme $\lambda$ de $a$ sur $n$. Donc :

$$
\begin{array}{ccc}
a & \xrightarrow{\lambda} & g \\
& & \xrightarrow{\mu} b
\end{array}
$$

est une extension de $b$ par $a$, de noyau $n$, qui est dite définie canoniquement *par* $a, b, \varphi$. L’application $b \mapsto (0, b)$ est un isomorphisme $\nu$ de $b$ sur une sous-algèbre de $g$ supplémentaire de $n$ dans $g$; donc l’extension est inessentielle.

Si on identifie $a$ à $n$ par $\lambda$ et $b$ à $\nu(b)$ par $\nu$, on a, pour $a \in a$ et $b \in b$ :

$$
(\mathrm{ad}\ b).a = [(0, b), (a, 0)] = (\varphi_b a, 0) = \varphi_b a.
$$

Lorsque $\varphi = 0$, $g$ est l’algèbre de Lie produit de $b$ et $a$. Dans le cas général, $g$ s’appelle le *produit semi-direct de $b$ par $a$* (correspondant à l’homomorphisme $b \mapsto \varphi_b$ de $b$ dans l’algèbre de Lie des dérivations de $a$).

Nous avons donc établi la proposition suivante :

#### Proposition 7 {#lie-i-s1-prop-7 .statement}

Soient $a$ et $b$ deux algèbres de Lie sur $K$,

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

une extension inessentielle de $b$ par $a$, $\nu$ un isomorphisme de $b$ sur une sous-algèbre de $g$ tel que $\mu \circ \nu$ soit l’automorphisme identique de $b$, et $\varphi$ l’homomorphisme correspondant de $b$ dans l’algèbre de Lie des dérivations de $a$. Soit

$$
a \xrightarrow{\lambda_0} g_0 \xrightarrow{\mu_0} b
$$

l’extension inessentielle de $b$ par $a$ définie canoniquement par $\varphi$. Alors l’application $(a, b) \mapsto \lambda(a) + \nu(b)$ est un isomorphisme de $g_0$ sur $g$, et le diagramme suivant

$$
\begin{array}{ccc}
 & g_0 & \\
{\lambda_0} \nearrow & \downarrow f & \searrow {\mu_0} \\
a & & b \\
{\lambda} \searrow & & \nearrow {\mu} \\
 & g &
\end{array}
$$

est commutatif, de sorte que les deux extensions sont équivalentes.

#### Exemple 1 {#lie-i-s1-n8-exa-1 .statement}

Soient $g$ une algèbre de Lie sur $K$, $D$ une dérivation de $g$. Soit $\mathfrak{h}$ l’algèbre de Lie commutative $K$. L’application $\lambda \mapsto \lambda D$ ($\lambda \in K$) est un homomorphisme de $\mathfrak{h}$ dans l’algèbre de Lie des dérivations de $g$. Formons le produit semi-direct correspondant $\mathfrak{k}$ de $\mathfrak{h}$ par $g$. Soit $x_0$ l’élément $(0,1)$ de $\mathfrak{k}$. Pour tout $x \in g$, on a $Dx = [x_0, x]$.

#### Exemple 2 {#lie-i-s1-n8-exa-2 .statement}

Soient $g$ une algèbre de Lie sur $K$, $M$ un $K$-module, $\rho$ un homomorphisme de $g$ dans $\mathrm{gl}(M)$. Si on considère $M$ comme une algèbre de Lie commutative, l’algèbre de Lie des dérivations de $M$ est $\mathrm{gl}(M)$. On peut donc former le produit semi-direct $\mathfrak{h}$ de $g$ par $M$ correspondant à $\rho$.

Plus particulièrement, prenons $g = \mathrm{gl}(M)$, et prenons pour $\rho$ l’application identique de $\mathrm{gl}(M)$. Le produit semi-direct de $g$ par $M$ se note alors $\mathfrak{af}(M)$ (ou $\mathfrak{af}(n, K)$ si $M = K^n$). Un élément de $\mathfrak{af}(M)$ est un couple $(m, u)$, où $m \in M$, $u \in \mathrm{gl}(M)$; et le crochet est défini par

$$
[(m, u), (m', u')] = (u(m') - u'(m), [u, u']).
$$

\* Lorsque $M$ est un espace vectoriel de dimension finie sur $\mathbf{R}$, $\mathfrak{af}(M)$ s’identifie canoniquement à l’algèbre de Lie du *groupe affine* de $M$.*

Soit $t$ une algèbre de Lie sur $K$. Une application linéaire $\theta$ de $t$ dans $\mathfrak{af}(M)$ peut s’écrire $x \mapsto ((\zeta(x), \eta(x))$, où $\zeta$ est une application linéaire de $t$ dans $M$ et où $\eta$ est une application linéaire de $t$ dans $\mathrm{gl}(M)$. Cherchons quelles conditions doivent vérifier $\zeta$ et $\eta$ pour que $\theta$ soit un homomorphisme. Pour $x \in t, y \in t$, on doit avoir

$$
\theta([x, y]) = [\theta(x), \theta(y)]
$$

c’est-à-dire

$$
(\zeta([x, y]), \eta([x, y])) = [(\zeta(x), \eta(x)), (\zeta(y), \eta(y))] \\
= (\eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x), [\eta(x), \eta(y)]).
$$

Donc, pour que $\theta$ soit un homomorphisme de $t$ dans $\mathfrak{af}(M)$, il faut et il suffit que $\eta$ soit un homomorphisme de $t$ dans $\mathrm{gl}(M)$, et que $\zeta$ vérifie la relation :

(13)
$$
\zeta([x, y]) = \eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x).
$$

Soit $N$ le $K$-module $M \times K$. Prenons pour $t$ la sous-algèbre de $\mathrm{gl}(N)$ formée des $\omega \in \mathrm{gl}(N)$ tels que $\omega(N) \subset M$. Pour tout $\omega \in t$, soit $\eta(\omega) \in \mathrm{gl}(M)$ la restriction de $\omega$ à $M$, et soit $\zeta(\omega) = \omega(0, 1) \in M$. Pour $\omega_1 \in t, \omega_2 \in t$, on a

$$
\zeta([\omega_1, \omega_2]) = \omega_1(\zeta(\omega_2)) - \omega_2(\zeta(\omega_1)) = \eta(\omega_1) \cdot \zeta(\omega_2) - \eta(\omega_2) \cdot \zeta(\omega_1).
$$

Donc l’application $\omega \mapsto (\zeta(\omega), \eta(\omega))$ est un homomorphisme $\theta$ de $t$ dans $\mathfrak{af}(M)$. Il est clair que $\theta$ est *bijectif*. Soit $\varphi = \theta^{-1}$. Si $(m, u) \in \mathfrak{af}(M)$, $\varphi(m, u)$ est l’élément $\omega$ de $t$ défini par

$$
\omega(m', \lambda) = (u(m') + \lambda m, 0).
$$

On identifie souvent $\mathfrak{af}(M)$ à la sous-algèbre $t$ de $\mathrm{gl}(N)$ grâce à l’isomorphisme $\varphi$.

\* Lorsque $M$ est un espace vectoriel de dimension finie sur $\mathbf{R}$, l’homomorphisme $\varphi$ de $\mathfrak{af}(M)$ dans $\mathrm{gl}(N)$ correspond à un homomorphisme canonique $\psi$ du groupe affine $A$ de $M$ dans le groupe $\mathbf{GL}(N)$; si $a \in A$, $\psi(a)$ est l’unique élément $g$ de $\mathbf{GL}(N)$ tel que $g(m, 1) = (a(m), 1)$ pour tout $m \in M$. Cet homomorphisme est injectif, et $\psi(A)$ est l’ensemble des automorphismes de $N$ qui laissent stables toutes les variétés linéaires de $N$ parallèles à $M$.*

### 9. Changement de l’anneau de base

Soient $K_0$ un anneau commutatif à élément unité, $\rho$ un homomorphisme de $K_0$ dans $K$ transformant l’élément unité en élément unité. Soit $g$ une algèbre de Lie sur $K$. Soit $g'$ l’algèbre obtenue en considérant $g$ comme algèbre sur $K_0$ grâce à $\rho$ (cf. n° 1). Alors $g'$ est une algèbre de Lie. Les sous-algèbres (resp. idéaux) de $g$ sont des sous-algèbres (resp. idéaux) de $g'$. Si $a$ et $b$ sont des sous-modules de $g$, le crochet $[a, b]$ est le même dans $g$ et dans $g'$; en effet, $[a, b]$ est l’ensemble des éléments de la forme $\sum_{i=1}^n [x_i, y_i]$ où $x_i \in a, y_i \in b$. Il en résulte que $\mathcal{O}^p g = \mathcal{O}^p g'$, $\mathcal{C}^p g = \mathcal{C}^p g'$ pour tout $p$. Le commutant d’une partie est le même dans $g$ et $g'$. Donc $\mathcal{C}_p g = \mathcal{C}_p g'$ pour tout $p$.

Soient $K_1$ un anneau commutatif à élément unité, $\sigma$ un homomorphisme de $K$ dans $K_1$ transformant l’élément unité en élément unité. Soit $g$ une algèbre de Lie sur $K$. Soit $g_{(K_1)}$ l’algèbre sur $K_1$ déduite de $g$ par extension de l’anneau de base (cf. n° 1). Alors $g_{(K_1)}$ est une algèbre de Lie. Si $a$ est une sous-algèbre (resp. un idéal) de $g$, l’image canonique de $a_{(K_1)}$ dans $g_{(K_1)}$ est une sous-algèbre (resp. un idéal) de $g_{(K_1)}$. Si $a$ et $b$ sont des sous-modules de $g$, l’image canonique dans $g_{(K_1)}$ de $[a, b]_{(K_1)}$ est égale au crochet des images canoniques de $a_{(K_1)}$ et $b_{(K_1)}$. Il en résulte que $\mathcal{O}^p(g_{(K_1)})$ est l’image canonique de $(\mathcal{O}^p g)_{(K_1)}$, et que $\mathcal{C}^p(g_{(K_1)})$ est l’image canonique de $(\mathcal{C}^p g)_{(K_1)}$.

Si $K$ est un corps, $K_1$ un surcorps de $K$, et $\sigma$ l’injection canonique de $K$ dans $K_1$, alors on a, avec les identifications habituelles,

$$
[a, b]_{(K_1)} = [a_{(K_1)}, b_{(K_1)}], \quad \mathcal{O}^p(g_{(K_1)}) = (\mathcal{O}^p g)_{(K_1)}, \quad \mathcal{C}^p(g_{(K_1)}) = (\mathcal{C}^p g)_{(K_1)}.
$$

Ces résultats seront complétés au § 2, n° 9.

Si $M$ est un espace vectoriel de dimension finie sur le corps $K$, $M_{(K_1)}$ est un espace vectoriel de dimension finie sur $K_1$, et l’algèbre associative $\mathcal{L}(M_{(K_1)})$ s’identifie canoniquement à l’algèbre associative $\mathcal{L}(M)_{(K_1)}$. Donc l’algèbre de Lie $\mathrm{gl}(M_{(K_1)})$ s’identifie canoniquement à l’algèbre de Lie $\mathrm{gl}(M)_{(K_1)}$.

## EXERCICES {#lie-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
