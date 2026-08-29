---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 1
section_title: Algèbres de Lie compactes
lang: fr
source: lie-ix-fr
book_pages: LIE IX.107-LIE IX.108
pdf_pages: 0004-0010, 0110-0111
extraction: ocr
subsections:
    - "no": 1
      title: Formes hermitiennes invariantes
      page: 0
      pdf_page: 4
    - "no": 2
      title: Groupes de Lie réels commutatifs connexes
      page: 2
      pdf_page: 5
    - "no": 3
      title: Algèbres de Lie compactes
      page: 3
      pdf_page: 6
    - "no": 4
      title: Groupes dont l’algèbre de Lie est compacte
      page: 5
      pdf_page: 8
statements: 13
exercises: 9
content_sha256: 80e6589dc4619ad20bee2aab29b24ac20c8da7a662d382de7080a64e023d4e02
---

## § 1. ALGÈBRES DE LIE COMPACTES

### 1. Formes hermitiennes invariantes

Dans ce numéro, la lettre $k$ désigne l’un des corps $\mathbf{R}$ ou $\mathbf{C}$. Soient $V$ un $k$-espace vectoriel de dimension finie, $\Phi$ une forme hermitienne positive séparante² sur $V$, $G$ un groupe, $g$ une $\mathbf{R}$-algèbre de Lie, $\rho : G \to \mathbf{GL}(V)$ un homomorphisme de groupes, $\varphi : g \to \mathbf{gl}(V)$ un homomorphisme de $\mathbf{R}$-algèbres de Lie.

a) La forme $\Phi$ est invariante par $G$ (resp. $g$) si et seulement si $\rho(g)$ est unitaire pour $\Phi$ quel que soit $g \in G$ (resp. $\varphi(x)$ est antihermitien³ pour $\Phi$ quel que soit $x \in g$).

¹ Dans tout ce chapitre les renvois à A, VIII se réfèrent à la nouvelle édition (à paraître).
² Rappelons (A, IX, à paraître) qu’une forme hermitienne $H$ sur $V$ est dite séparante (ou non dégénérée) si pour tout élément non nul $u$ de $V$ il existe $v \in V$ tel que $H(u, v) \neq 0$.
³ On dit que $a \in \mathrm{End}(V)$ est antihermitien pour $\Phi$ si l’adjoint $a^*$ de $a$ relativement à $\Phi$ est égal à $-a$. Lorsque $k = \mathbf{C}$ (resp. $k = \mathbf{R}$), cela signifie aussi que l’endomorphisme $ia$ de $V$ (resp. de $\mathbf{C} \otimes_{\mathbf{R}} V$) est hermitien.

En effet, notons $a^*$ l’adjoint relativement à $\Phi$ d’un endomorphisme $a$ de $V$; pour $g$ dans $G$, $x$ dans $g$, $u$ et $v$ dans $V$, on a

$$
\Phi(\rho(g)\ u,\ \rho(g)\ v) = \Phi(\rho(g)^*\rho(g)\ u,\ v),
$$
$$
\Phi(\varphi(x)\ u,\ v) + \Phi(u,\ \varphi(x)\ v) = \Phi((\varphi(x) + \varphi(x)^*)\cdot u,\ v);
$$

pour que $\Phi(\rho(g)\ u,\ \rho(g)\ v) = \Phi(u,\ v)$ pour tous $u,\ v$ dans $V$, il est donc nécessaire et suffisant que $\rho(g)^*\rho(g) = \mathrm{Id}_V$; de même, pour que $\Phi(\varphi(x)\ u,\ v) + \Phi(u,\ \varphi(x)\ v) = 0$ pour tous $u,\ v$ dans $V$, il est nécessaire et suffisant que $\varphi(x) + \varphi(x)^* = 0$, d’où l’assertion annoncée.

b) Si la forme $\Phi$ est invariante par $G$ (resp. $g$), l’orthogonal d’un sous-espace stable de $V$ est stable; en particulier, la représentation $\rho$ (resp. $\varphi$) est alors semi-simple ($cf.$ A, IX); de plus, pour tout $g \in G$ (resp. tout $x \in g$), l’endomorphisme $\rho(g)$ (resp. $\varphi(x)$) de $V$ est alors semi-simple, à valeurs propres de valeur absolue 1 (resp. à valeurs propres imaginaires pures); en effet $\rho(g)$ est unitaire (resp. $i\varphi(x)$ est hermitien, $cf.$ A, IX).

c) Supposons $k = \mathbf{R}$. Si $G$ est un groupe de Lie connexe, $\rho$ un morphisme de groupes de Lie, $g$ l’algèbre de Lie de $G$ et $\varphi$ l’homomorphisme déduit de $\rho$, alors $\Phi$ est invariante par $G$ si et seulement si elle est invariante par $g$ (III, § 6, n° 5, cor. 3).

d) Pour qu’il existe sur $V$ une forme hermitienne positive séparante invariante par $G$, il faut et il suffit que le sous-groupe $\rho(G)$ de $\mathbf{GL}(V)$ soit relativement compact (INT, VII, § 3, n° 1, prop. 1).

### 2. Groupes de Lie réels commutatifs connexes

Soit $G$ un groupe de Lie (réel) commutatif connexe. L’application exponentielle

$$
\exp_G : \mathbf{L}(G) \to G
$$

est un morphisme de groupes de Lie, surjectif à noyau discret (III, § 6, n° 4, prop. 11), donc fait de $\mathbf{L}(G)$ un revêtement connexe de $G$.

a) Les conditions suivantes sont équivalentes : $G$ est simplement connexe, $\exp_G$ est un isomorphisme, $G$ est isomorphe à $\mathbf{R}^n$ ($n = \dim G$). Si on transporte alors à $G$ par l’isomorphisme $\exp_G$ la structure d’espace vectoriel de $\mathbf{L}(G)$, on obtient sur $G$ une structure d’espace vectoriel, qui est la seule compatible avec la structure de groupe topologique de $G$. Les groupes de Lie commutatifs simplement connexes sont appelés groupes (de Lie) *vectoriels* ; sauf mention expresse du contraire, on les munit toujours de la structure de $\mathbf{R}$-espace vectoriel définie ci-dessus.

b) Notons $\Gamma(G)$ le noyau de $\exp_G$. D’après TG, VII, p. 4, th. 1, le groupe $G$ est compact si et seulement si $\Gamma(G)$ est un *réseau* de $\mathbf{L}(G)$, c’est-à-dire (*loc. cit.*) si le rang du $\mathbf{Z}$-module libre $\Gamma(G)$ est égal à la dimension de $G$. Inversement, si $L$ est un $\mathbf{R}$-espace vectoriel de dimension finie et $\Gamma$ un réseau de $L$, le groupe topologique quotient $L/\Gamma$ est un groupe de Lie commutatif compact connexe.

Les groupes de Lie commutatifs compacts connexes sont appelés *tores réels*, ou (dans ce chapitre) *tores*.

c) Dans le cas général, soit E le sous-espace vectoriel de L(G) engendré par Γ(G), et soit V un sous-espace supplémentaire. Alors G est produit direct de ses sous-groupes de Lie exp(E) et exp(V); le premier est un tore, le second est vectoriel. Enfin tout sous-groupe compact de G est contenu dans exp(E) (puisque sa projection dans exp(V) est nécessairement réduite à l’élément neutre); le sous-groupe exp(E) est donc l’unique sous-groupe compact *maximal* de G.

Prenons par exemple G = C*; identifions L(G) à C de sorte que l’application exponentielle de G soit x ↦ e^x. Alors Γ(G) = 2πiZ, E = iR, donc exp(E) = U; si on prend V = R, on a exp(V) = R*_+, et on retrouve l’isomorphisme C* → U × R*_+ construit en TG, VIII, p. 4.

d) Notons enfin que exp_G : L(G) → G est un revêtement universel de G, donc que Γ(G) s’identifie naturellement au groupe fondamental de G.

### 3. Algèbres de Lie compactes

#### Proposition 1 {#lie-ix-s1-prop-1 .statement tag=019D}

Soit g une algèbre de Lie (réelle). Les conditions suivantes sont équivalentes :
(i) g est isomorphe à l’algèbre de Lie d’un groupe de Lie compact.
(ii) Le groupe Int(g) (III, § 6, no 2, déf. 2) est compact.
(iii) g possède une forme bilinéaire invariante (I, § 3, no 6) qui est symétrique, positive et séparante.
(iv) g est réductive (I, § 6, no 4, déf. 4); pour tout x ∈ g, l’endomorphisme ad x est semi-simple, à valeurs propres imaginaires pures.
(v) g est réductive et sa forme de Killing B est négative.

(i) ⇒ (ii) : si g est l’algèbre de Lie du groupe de Lie compact G, le groupe Int(g) est séparé et isomorphe à un quotient du groupe compact G_0 (III, § 6, no 4, cor. 4), donc est compact.

(ii) ⇒ (iii) : si le groupe Int(g) est compact, il existe sur g une forme bilinéaire symétrique qui est positive, séparante, et invariante par Int(g) (no 1), donc aussi invariante pour la représentation adjointe de g.

(iii) ⇒ (iv) : si (iii) est satisfaite, la représentation adjointe de g est semi-simple (no 1), donc g est réductive ; de plus les endomorphismes ad x, pour x ∈ g, possèdent les propriétés indiquées (no 1).

(iv) ⇒ (v) : pour tout x ∈ g, on a B(x, x) = Tr((ad x)^2); par suite, B(x, x) est la somme des carrés des valeurs propres de ad x, et est par conséquent négative si celles-ci sont imaginaires pures.

(v) ⇒ (i) : supposons g réductive, donc produit d’une sous-algèbre commutative c et d’une sous-algèbre semi-simple s (I, § 6, no 4, prop. 5). La forme de Killing de s est la restriction à s de la forme B, donc est négative et séparante si B est négative. Le sous-groupe Int(s) de GL(s) est fermé (c’est la composante neutre de Aut(s),

III, § 10, n° 2, cor. 2) et laisse invariante la forme positive séparante — B ; il est donc compact, et s est isomorphe à l’algèbre de Lie du groupe de Lie compact Int(s). Par ailleurs, comme c est commutative, elle est isomorphe à l’algèbre de Lie d’un tore T. Ainsi g est isomorphe à l’algèbre de Lie du groupe de Lie compact Int(s) × T.

#### Définition 1 {#lie-ix-s1-def-1 .statement tag=019E}

On appelle algèbre de Lie compacte¹ toute algèbre de Lie qui possède les propriétés (i) à (v) de la proposition 1.

Les algèbres de Lie compactes sont donc les algèbres produit d’une algèbre commutative par une algèbre semi-simple compacte. En d’autres termes, pour qu’une algèbre de Lie soit compacte, il faut et il suffit qu’elle soit réductive et que son algèbre dérivée soit compacte.

L’algèbre de Lie d’un groupe de Lie compact est compacte.

#### Proposition 2 {#lie-ix-s1-prop-2 .statement tag=019F}

a) Le produit d’un nombre fini d’algèbres de Lie est une algèbre de Lie compacte si et seulement si chaque facteur est compact.
b) Une sous-algèbre d’une algèbre de Lie compacte est compacte.
c) Soit h un idéal d’une algèbre de Lie compacte g. Alors l’algèbre g/h est compacte et l’extension h → g → g/h est triviale.

Les assertions a) et b) résultent de la caractérisation (iii) de la prop. 1. La partie c) résulte de a) et du fait que dans une algèbre de Lie réductive, tout idéal est facteur direct (I, § 6, n° 4, cor. à la prop. 5).

#### Proposition 3 {#lie-ix-s1-prop-3 .statement tag=019G}

Soit G un groupe de Lie dont le groupe des composantes connexes est fini. Les conditions suivantes sont équivalentes :
(i) L’algèbre de Lie L(G) est compacte.
(ii) Le groupe Ad(G) est compact.
(iii) Il existe sur L(G) une forme bilinéaire symétrique positive séparante invariante pour la représentation adjointe de G.
*(iv) G possède une métrique riemannienne invariante par translations à droite et à gauche.*

(i) ⇒ (ii) : si L(G) est compacte, le groupe Ad(G₀) = Int(L(G)) est compact ; comme il est d’indice fini dans Ad(G), ce dernier groupe est compact.
(ii) ⇒ (iii) : cela résulte du n° 1.
(iii) ⇒ (i) : comme Int(L(G)) ⊂ Ad(G), cela résulte de la caractérisation (iii) de la proposition 1.
*(iii) ⇔ (iv) : cela résulte de III, § 3, n° 13. \*

¹ On notera qu’un espace vectoriel topologique réel ne peut être un espace topologique compact que s’il est réduit à 0.

### 4. Groupes dont l’algèbre de Lie est compacte

#### Théorème 1 (H. Weyl) {#lie-ix-s1-thm-1 .statement tag=019H}

Soit G un groupe de Lie connexe dont l’algèbre de Lie est semi-simple compacte. Alors G est compact et son centre est fini.

Comme G est semi-simple, son centre D est discret. De plus, le groupe quotient G/D est isomorphe à Ad(G) (III, § 6, no 4, cor. 4), donc compact (prop. 3). Enfin, le groupe G/D est égal à son groupe dérivé (III, § 9, no 2, cor. à la prop. 4). Le théorème résulte alors de INT, VII, § 3, no 2, prop. 5.

#### Proposition 4 {#lie-ix-s1-prop-4 .statement tag=019I}

Soit G un groupe de Lie connexe d’algèbre de Lie compacte. Il existe un tore T, un groupe de Lie compact semi-simple simplement connexe S, un groupe vectoriel V et un morphisme surjectif de noyau fini f : V × T × S → G. Si G est compact, le groupe V est réduit à l’élément neutre.

Soit C (resp. S) un groupe de Lie simplement connexe dont l’algèbre de Lie est isomorphe au centre (resp. à l’algèbre dérivée) de L(G). Alors C est un groupe vectoriel, S un groupe compact de centre fini (th. 1) et G s’identifie au quotient de C × S par un sous-groupe discret D, qui est central (INT, VII, § 3, no 2, lemme 4). Comme la projection de D dans S est d’image centrale, donc finie, D ∩ C est d’indice fini dans D. Soient C’ le sous-espace vectoriel de C engendré par D ∩ C, et V un sous-espace supplémentaire. Alors le groupe T = C’/(D ∩ C) est un tore, et G est isomorphe au quotient du groupe produit V × T × S par un groupe fini.

Si G est compact, il en est de même de V × T × S (TG, III, p. 29, cor. 2), donc de V, ce qui entraîne V = {e}.

#### Corollaire 1 {#lie-ix-s1-prop-4-cor-1 .statement tag=019J}

Soit G un groupe de Lie compact connexe. Alors C(G)_0 est un tore, D(G) un groupe de Lie connexe semi-simple compact et le morphisme (x, y) ↦ xy de C(G)_0 × D(G) dans G est un revêtement fini.

Avec les notations de la prop. 4, on a V = {e} et les sous-groupes f(T) et f(S) de G sont compacts, donc fermés. Il suffit donc de montrer que f(T) = C(G)_0, f(S) = D(G). Or, on a L(G) = L(f(T)) × L(f(S)); comme S est semi-simple et T commutatif, cela implique L(f(T)) = C(L(G)) = L(C(G)_0) (III, § 9, no 3, prop. 8) et L(f(S)) = D(L(G)) = L(D(G)) (III, § 9, no 2, cor. de la prop. 4), d’où l’assertion annoncée.

#### Corollaire 2 {#lie-ix-s1-prop-4-cor-2 .statement tag=019K}

Le centre et le groupe fondamental d’un groupe de Lie compact connexe semi-simple sont finis. Son revêtement universel est compact.

Avec les notations de la prop. 4, les groupes V et T sont réduits à l’élément neutre ; S est donc un revêtement universel de G, et le groupe fondamental de G est isomorphe à Ker f, donc fini. Le centre D de G est discret car G est semi-simple, donc D est fini.

#### Corollaire 3 {#lie-ix-s1-prop-4-cor-3 .statement tag=019L}

Le groupe fondamental d’un groupe de Lie compact connexe G est un $\mathbf{Z}$-module de type fini, de rang égal à la dimension de C(G).

En effet, avec les notations du cor. 1, le groupe fondamental de $C(G)_0$ est isomorphe à $\mathbf{Z}^n$, avec $n = \dim C(G)_0$, et le groupe fondamental de $D(G)$ est fini (cor. 2).

#### Corollaire 4 {#lie-ix-s1-prop-4-cor-4 .statement tag=019M}

Soit $G$ un groupe de Lie compact connexe. Les conditions suivantes sont équivalentes :
(i) $G$ est semi-simple ;
(ii) $C(G)$ est fini ;
(iii) $\pi_1(G)$ est fini.
Si $G$ est simplement connexe, il est semi-simple.
Cela résulte des cor. 1 à 3.

#### Corollaire 5 {#lie-ix-s1-prop-4-cor-5 .statement tag=019N}

Soit $G$ un groupe de Lie compact connexe. Alors $\mathrm{Int}(G)$ est la composante neutre du groupe de Lie $\mathrm{Aut}(G)$ (III, § 10, no 2).
Soit $f \in \mathrm{Aut}(G)_0$. Alors $f$ induit un automorphisme $f_1$ de $C(G)_0$ et un automorphisme $f_2$ de $D(G)$, et on a $f_1 \in \mathrm{Aut}(C(G)_0)_0, f_2 \in \mathrm{Aut}(D(G))_0$. Puisque $\mathrm{Aut}(C(G)_0)$ est discret (TG, VII, p. 15, prop. 5), on a $f_1 = \mathrm{Id}$; puisque $D(G)$ est semi-simple, il existe, d’après III, § 10, no 2, cor. 2 au th. 1, un élément $g$ de $D(G)$ tel que $f_2(x) = gxg^{-1}$ pour tout $x \in D(G)$. Pour tout $x \in C(G)_0$, on a $gxg^{-1} = x = f_1(x)$; comme $G = C(G)_0 . D(G)$, il en résulte que $gxg^{-1} = f(x)$ pour tout $x \in G$, donc $f = \mathrm{Int}\, g$.

#### Proposition 5 {#lie-ix-s1-prop-5 .statement tag=019O}

Soit $G$ un groupe de Lie d’algèbre de Lie compacte.
a) Supposons $G$ connexe. Alors $G$ possède un plus grand sous-groupe compact $K$; celui-ci est connexe. Il existe un sous-groupe vectoriel (no 2) central fermé $N$ de $G$ tel que $G$ soit le produit direct $N \times K$.
b) Supposons le groupe des composantes connexes de $G$ fini. Alors :
(i) Tout sous-groupe compact de $G$ est contenu dans un sous-groupe compact maximal.
(ii) Si $K_1$ et $K_2$ sont deux sous-groupes compacts maximaux de $G$, il existe $g \in G$ tel que $K_2 = gK_1g^{-1}$.
(iii) Soit $K$ un sous-groupe compact maximal de $G$. Alors $K \cap G_0$ est égal à $K_0$; c’est le plus grand sous-groupe compact de $G_0$.
(iv) Il existe un sous-groupe vectoriel central fermé $N$ de $G_0$, distingué dans $G$, tel que, pour tout sous-groupe compact maximal $K$ de $G$, $G_0$ soit le produit direct de $K_0$ par $N$ et $G$ le produit semi-direct de $K$ par $N$.
a) Reprenons les notations de la prop. 4. La projection de $\mathrm{Ker}\, f$ sur $V$ est un sous-groupe fini du groupe vectoriel $V$, donc est réduite à l’élément neutre. Il s’ensuit que $\mathrm{Ker}\, f$ est contenu dans $T \times S$, donc que $G$ est le produit direct du groupe vectoriel $N = f(V)$ et du groupe compact $K = f(T \times S)$. Tout sous-groupe compact de $G$ a une projection dans $N$ réduite à l’élément neutre, donc est contenu dans $K$. Cela démontre a).
b) Supposons maintenant $G/G_0$ fini. D’après a), $G_0$ est le produit direct de son plus grand sous-groupe compact $M$ par un sous-groupe vectoriel $P$; le sous-groupe

M de G est évidemment distingué. Soit n un sous-espace vectoriel de L(G), supplémentaire de L(M) et stable pour la représentation adjointe de G (n° 1 et n° 3, prop. 3); c’est un idéal de L(G) et on a L(G) = L(M) × n. Soit N le sous-groupe intégral de G d’algèbre de Lie n ; d’après III, § 6, n° 6, prop. 14, il est distingué dans G. La projection de L(G) sur L(P), de noyau L(M), induit un isomorphisme de n sur L(P); il en résulte que la projection de G₀ sur P induit un morphisme étale de N sur P; comme P est simplement connexe, c’est un isomorphisme, et N est un groupe vectoriel. Le morphisme (x, y) ↦ xy de M × N dans G₀ est un morphisme étale injectif (puisque M ∩ N est réduit à l’élément neutre), donc un isomorphisme. Il s’ensuit que N est un sous-groupe fermé de G et que le quotient G/N est compact, puisque G₀/N est compact et que G/G₀ est fini (TG, III, p. 29, cor. 2).

D’après INT, VII, § 3, n° 2, prop. 3, tout sous-groupe compact de G est contenu dans un sous-groupe compact maximal, ceux-ci sont conjugués, et pour tout sous-groupe compact maximal K de G, G est produit semi-direct de K par N. Comme G₀ contient N, il est alors produit semi-direct de N par G₀ ∩ K ; il s’ensuit que G₀ ∩ K est connexe, donc égal à K₀, puisque K/(G₀ ∩ K) est isomorphe à G/G₀, donc fini ; enfin, K₀ est évidemment le plus grand sous-groupe compact de G₀ d’après a).

#### Corollaire {#lie-ix-s1-n4-cor-1 .statement tag=019P}

Si N satisfait aux conditions de b) (iv), et si K₁ et K₂ sont deux sous-groupes compacts maximaux de G, il existe n ∈ N tel que nK₁n⁻¹ = K₂.

Il existe en effet d’après (ii) un élément g ∈ G tel que gK₁g⁻¹ = K₂ ; d’après (iv), il existe n ∈ N et k ∈ K₁ tels que g = nk. L’élément n possède alors la propriété exigée.

## EXERCICES {#lie-ix-s1-exercises}

See the [exercises for § 1](exercises/s1/).
