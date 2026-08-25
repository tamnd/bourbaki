---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 8
section_title: Groupes de Lie sur R ou Q_p
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0223-0227, 0273-0274
extraction: ocr
subsections:
    - "no": 1
      title: Morphismes continus
      page: 0
      pdf_page: 223
    - "no": 2
      title: Sous-groupes fermés
      page: 0
      pdf_page: 225
statements: 10
exercises: 7
content_sha256: 78521e2099e3f9384f38950c262118a0748b7272a54109b6e52efcd2e553264f
---

## § 8. Groupes de Lie sur $\mathbf{R}$ ou $\mathbf{Q}_p$

### 1. Morphismes continus

#### Théorème 1 {#lie-iii-s8-thm-1 .statement}

Soient $G$ et $H$ deux groupuscules de Lie sur $\mathbf{R}$ ou $\mathbf{Q}_p$. Soit $f$ un morphisme continu de $G$ dans $H$. Alors $f$ est analytique.

Munissons $L(G)$ et $L(H)$ de normes définissant leurs topologies et telles que $\|[x, y]\| \leq \|x\| \|y\|$ quels que soient $x, y$. Il existe une boule ouverte $V$ de centre 0 dans $L(G)$ et une application exponentielle $\varphi$ de $G$ définie dans $V$, telles que : 1) $\varphi(V)$ est un voisinage ouvert de $e$ dans $G$; 2) $\varphi$ est un isomorphisme de la variété analytique $V$ sur la variété analytique $\varphi(V)$; 3) $\varphi(nx) = \varphi(x)^n$ pour tout $x \in V$ et tout $n \in \mathbf{Z}$ tel que $nx \in V$. Définissons de même $W$ et $\psi$ pour $H$. En diminuant au besoin $V$, on peut supposer que $f(\varphi(V)) \subset \psi(W)$. Alors $g = \psi^{-1} \circ f \circ \varphi$ est une application continue de $V$ dans $W$.

Montrons que
$$(1)$$
$$(x \in V, \lambda \in \mathbf{Q} \text{ et } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).$$

On peut supposer $\lambda \neq 0$. Soit $\lambda = \frac{p}{q}$ avec $p, q$ dans $\mathbf{Z} - \{0\}$. Soit $y = \frac{p}{q} x$.

Si $K = \mathbf{R}$, nous poserons $z = \frac{x}{q} = \frac{y}{p} \in V$. On a $x = qz, y = pz$, d’où
$$g(x) = \psi^{-1}(f(\varphi(qz))) = \psi^{-1}(f(\varphi(z)^q)) = \psi^{-1}(f(\varphi(z))^q) = q\psi^{-1}(f\varphi(z))) = qg(z)$$
De même, $g(y) = pg(z)$, d’où (1).

Si $K = \mathbf{Q}_p$, nous poserons $z = px = qy \in V$, d’où $g(z) = pg(x) = qg(y)$, d’où encore (1).

Comme $\mathbf{Q}$ est dense dans $\mathbf{K}$, (1) entraîne que
$$(2)$$
$$(x \in V, \lambda \in K \text{ et } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).$$
Soient $x \in L(G)$, et $\lambda, \lambda'$ dans $K^*$ tels que $\lambda x \in V, \lambda' x \in V$. On a
$$
g(\lambda' x) = g\left( \frac{\lambda'}{\lambda} \lambda x \right) = \frac{\lambda'}{\lambda} g(\lambda x)
$$
d’après (2), donc $\frac{1}{\lambda} g(\lambda x) = \frac{1}{\lambda'} g(\lambda' x)$. On définit donc un prolongement $h$ de $g$ à $L(G)$ en posant $h(x) = \frac{1}{\lambda} g(\lambda x)$ pour tout $\lambda$ tel que $\lambda x \in V$. Il est clair que $h$ est continu. Montrons que
$$(3)$$
$$(x \in L(G) \text{ et } \lambda \in K) \Rightarrow h(\lambda x) = \lambda h(x).$$
Soit $\lambda' \in K^*$ tel que $\lambda' x \in V$ et $\lambda' \lambda x \in V$. On a
$$
h(\lambda x) = \frac{1}{\lambda'} g(\lambda' \lambda x) = \frac{1}{\lambda'} \lambda g(\lambda' x) = \lambda \frac{1}{\lambda'} g(\lambda' x) = \lambda h(x).
$$
Soient $x, y$ dans $L(G)$. On a, d’après la prop. 4 du § 4, n° 3,
$$
h(x) + h(y) = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(\lambda h(x)) \psi(\lambda h(y)))
= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(h(\lambda x)) \psi(h(\lambda y))).
$$
Pour $|\lambda|$ assez petit, on a $\lambda x \in V$ et $\lambda y \in V$, donc l’expression précédente est égale à
$$
\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(f(\varphi(\lambda x)) f(\varphi(\lambda y)))
= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} (\psi^{-1} \circ f)(\varphi(\lambda x) \varphi(\lambda y))
= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} g(\varphi^{-1}(\varphi(\lambda x) \varphi(\lambda y)))
= \lim_{\lambda \in K^*, \lambda \to 0} h(\lambda^{-1} \varphi^{-1}(\varphi(\lambda x) \varphi(\lambda y)))
= h(\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \varphi^{-1}(\varphi(\lambda x) \varphi(\lambda y)))
= h(x + y).
$$
Ainsi, $h$ est linéaire continu, donc $g = h|V$ est analytique, donc $f$ est analytique dans $\varphi(V)$, donc $f$ est analytique (§ 1, n° 10).

#### Corollaire 1 {#lie-iii-s8-thm-1-cor-1 .statement}

Soit $G$ un groupe topologique. Il existe sur $G$ au plus une structure de variété analytique sur $\mathbf{R}$ (resp. $\mathbf{Q}_p$) compatible avec la structure de groupe et la topologie de $G$.
Cela résulte aussitôt du th. 1.

#### Définition 1 {#lie-iii-s8-def-1 .statement}

On dit qu’un groupe topologique $G$ est un groupe de Lie réel (resp. $p$-adique) s’il existe sur $G$ une structure de groupe de Lie réel (resp. $p$-adique) compatible avec sa topologie.

Cette structure est alors unique et on peut donc parler de la dimension d’un tel groupe. Si G et H sont deux tels groupes, tout morphisme continu de G dans H est analytique.

#### Corollaire 2 {#lie-iii-s8-def-1-cor-2 .statement}

Soient G un groupe topologique, V un voisinage ouvert de e. On suppose V muni d’une structure de variété analytique qui en fait un groupuscule de Lie réel (resp. p-adique). Alors G est un groupe de Lie réel (resp. p-adique).

Soit g ∈ G. Il existe un voisinage ouvert V’ de e dans G tel que V’ ∪ gV’g⁻¹ ⊂ V. L’application v ↦ gvvg⁻¹ de V’ dans V est un morphisme continu, donc analytique, du groupuscule de Lie V’ dans le groupuscule de Lie V. Il suffit alors d’appliquer la prop. 18 du § 1, n° 9.

#### Remarque 1 {#lie-iii-s8-n1-rem-1 .statement}

Le th. 1 et ses corollaires deviennent inexact si on y remplace R (resp. Q_p) par exemple par C (exerc. 1).

#### Remarque 2 {#lie-iii-s8-n1-rem-2 .statement}

Soit G un groupe topologique. On peut montrer¹ que les conditions suivantes sont équivalentes : a) G est un groupe de Lie réel de dimension finie ; b) G est localement compact et il existe un voisinage de e ne contenant aucun sous-groupe distinct de {e} ; c) il existe un voisinage ouvert de e homéomorphe à une boule ouverte d’un espace R^n. (Pour un résultat beaucoup moins difficile, cf. exerc. 6).

#### Proposition 1 {#lie-iii-s8-prop-1 .statement}

Soient G, G’ des groupes topologiques, f un morphisme continu de G dans G’. On suppose qu’on est dans l’un des trois cas suivants :

a) G est un groupe de Lie réel et G’ un groupe de Lie p-adique ;
b) G est un groupe de Lie p-adique et G’ un groupe de Lie réel ;
c) G est un groupe de Lie p-adique et G’ un groupe de Lie p’-adique, avec p ≠ p’.
Alors f est localement constant.

Cas a. Soit G_0 la composante neutre de G. Alors f(G_0) est un sous-groupe connexe de G’, donc f(G_0) = {e}, et G_0 est ouvert dans G.

Cas b. Soit V’ un voisinage de e dans G’ tel que tout sous-groupe de G’ contenu dans V’ soit réduit à {e} (§ 4, n° 2, cor. 1 du th. 2). Il existe un voisinage V de e dans G tel que f(V) ⊂ V’. Puis il existe un sous-groupe ouvert G_1 de G tel que G_1 ⊂ V (§ 7, n° 1, prop. 1). On a alors f(G_1) = {e}.

Cas c. D’après le § 7, th. 4 et cor. de la prop. 8, il existe un voisinage V’ de e dans G’ tel que, pour tout x’ ∈ V’ − {e}, x’^{p^n} ne tende pas vers e quand n tend vers +∞. Il existe un voisinage V de e dans G tel que f(V) ⊂ V’. D’après le § 7, th. 4 et prop. 9, il existe un sous-groupe ouvert G_1 de G tel que G_1 ⊂ V et tel que, pour tout x ∈ G_1, x^{p^n} tend vers e quand n tend vers +∞. On a alors f(G_1) = {e}.

### 2. Sous-groupes fermés

#### Théorème 2 {#lie-iii-s8-thm-2 .statement}

Soit G un groupe de Lie de dimension finie sur R ou Q_p. Tout sous-groupe fermé de G est un sous-groupe de Lie de G. Plus généralement, soient U un voisinage

¹ Voir par exemple D. MONTGOMERY et L. ZIPPIN, Topological transformation groups, Interscience tracts in pure and applied mathematics, n° 1, Interscience publishers, New York 1955 (en particulier p. 169 et 184).

ouvert symétrique de e dans G, et H un sous-espace fermé non vide de U tel que les conditions x ∈ H, y ∈ H et xy⁻¹ ∈ U entraînent xy⁻¹ ∈ H. Alors H est un sous-groupuscule de Lie de G.

Soit 𝔤 la sous-algèbre de Lie tangente en e à H (§ 4, n° 5, déf. 2). Il existe un sous-groupuscule de Lie H₀ de G d’algèbre de Lie 𝔤, et contenu dans H. Nous allons montrer que H₀ est ouvert dans H pour la topologie induite par celle de G. Ceci prouvera que H est une sous-variété analytique de G et le théorème sera établi.

Il existe un sous-espace vectoriel t supplémentaire de 𝔤 dans L(G), des voisinages ouverts symétriques V₁, V₂ de zéro dans 𝔤 et t respectivement, et une application exponentielle φ de G définie dans V₁ + V₂, possédant les propriétés suivantes:

a) l’application (a₁, a₂) ↦ φ(a₁)φ(a₂) est un isomorphisme analytique de V₁ × V₂ sur une partie ouverte V de G;
b) φ(V₁) ⊂ H₀;
c) V² ⊂ U.

Nous allons montrer (ce qui achèvera la démonstration) qu’il existe un voisinage ouvert V₂′ de 0 dans V₂ tel que H ∩ (φ(V₁)φ(V₂′)) = φ(V₁).

Supposons cette assertion inexacte. Alors on peut trouver une suite (xₙ) dans V₁ et une suite (yₙ) dans V₂ − {0} tendant vers 0, telles que φ(xₙ)φ(yₙ) ∈ H pour tout n. On a φ(yₙ) ∈ H d’après c).

Si K = Q_p, on peut de plus supposer que V₂ est un sous-groupe additif de t et que φ(pa) = φ(a)^p pour tout a ∈ V₂ et tout p ∈ Z. Alors φ(λy₁) ∈ H pour tout λ ∈ Z, donc par continuité pour tout λ ∈ Z_p. L’application f : λ ↦ φ(λy₁) de Z_p dans G est analytique, prend ses valeurs dans H, et (T₀f)(1) = y₁. Donc y₁ ∈ 𝔤, ce qui est absurde. Le théorème est donc établi dans le cas de Q_p.

Si K = R, on peut supposer que V₂ est convexe et que yₙ appartient à $\frac{1}{4} V₂ - \{0\}$. Quitte à extraire de (yₙ) une suite partielle, on peut trouver une suite (λₙ) de scalaires non nuls tels que $\lambdaₙ^{-1} yₙ$ tende vers un élément y de V₂ − {0}. La suite (λₙ) tend vers 0. Soit λ ∈ R tel que $\lambda y \in \frac{1}{4} V₂$, et prouvons que exp(λy) ∈ H. On peut supposer que $\lambda \lambdaₙ^{-1} yₙ \in \frac{1}{4} V₂$ pour tout n. Soit kₙ ∈ Z tel que $|\lambda - kₙ \lambdaₙ|$ tende vers 0. Pour n assez grand, on a $(\lambda - kₙ \lambdaₙ) \lambdaₙ^{-1} yₙ \in \frac{1}{4} V₂$, donc $kₙ yₙ \in \frac{1}{2} V₂$. Donc exp(hyₙ) ∈ H pour h entier et $0 \leq |h| \leq |kₙ|$ (comme on le voit par récurrence sur |h|). Alors

$$
\exp(\lambda y) = \lim_{n \to \infty} \exp(\lambda \lambdaₙ^{-1} yₙ) = \lim_{n \to \infty} (\exp((\lambda - kₙ \lambdaₙ) \lambdaₙ^{-1} yₙ) \exp(kₙ yₙ))
= \lim_{n \to \infty} \exp kₙ yₙ \in H.
$$

Donc l’application f : λ ↦ exp λy, où $\lambda y \in \frac{1}{4} V₂$, prend ses valeurs dans H, et (T₀f)(1) = y. Donc y ∈ 𝔤, ce qui est absurde. Le théorème est ainsi établi dans le cas de R.

Le th. 2 devient inexact si on ne suppose pas G de dimension finie (exerc. 12.)

#### Corollaire 1 {#lie-iii-s8-thm-2-cor-1 .statement}

Soient $G'$ un groupe localement compact, $G$ un groupe de Lie de dimension finie sur $\mathbf{R}$ (resp. $\mathbf{Q}_p$), $f$ un morphisme continu de $G'$ dans $G$. Si le noyau de $f$ est discret, $G'$ est un groupe de Lie réel (resp. $p$-adique) de dimension finie.

Il existe un voisinage compact $V$ de $e$ dans $G'$ tel que $f|V$ soit un homéomorphisme de $V$ sur un sous-espace compact de $G$. Si $U$ est un voisinage ouvert de $e$ assez petit dans $G$, les hypothèses du th. 2 sont vérifiées avec $H = f(V) \cap U$. Donc $H$ est un sous-groupuscule de Lie de $G$. Soit $W$ l’image réciproque de $H$ par $f|V$. Alors $W$ est un voisinage de $e$ dans $G'$. Munissons $W$ de la structure de variété analytique transportée de celle de $H$ par $(f|W)^{-1}$. Pour tout $z \in G'$, l’application $x \mapsto f(z)x f(z)^{-1}$ de $G$ dans $G$ est analytique; donc il existe un voisinage ouvert $W'$ de $e$ dans $W$ tel que l’application $x' \mapsto zx'z^{-1}$ de $W'$ dans $W$ soit analytique. D’après la prop. 18 du § 1, n° 9, il existe sur $G'$ une structure de groupe de Lie qui induit, sur un voisinage ouvert assez petit de $e$, la même structure analytique que $W$, et donc la même topologie que la topologie initialement donnée de $G'$.

#### Corollaire 2 {#lie-iii-s8-thm-2-cor-2 .statement}

Soient $G$ un groupe de Lie de dimension finie sur $K$, $H$ un sous-groupe de $G$, $V$ un voisinage ouvert de $e$ dans $G$, $(M_i)_{i \in I}$ une famille de variétés analytiques sur $K$; pour tout $i \in I$, soit $f_i$ une application $K$-analytique de $V$ dans $M_i$ telle que $H \cap V = \{ x \in V | f_i(x) = f_i(e) \text{ pour tout } i \in I \}$.

(i) Si $K = \mathbf{C}$, $H$ est un sous-groupe de Lie de $G$.

(ii) Si $K$ est une extension de degré fini de $\mathbf{Q}_p$, et si $I$ est fini, $H$ est un sous-groupe de Lie de $G$.

(i) Supposons $K = \mathbf{C}$. Considérons $G$ comme un groupe de Lie réel. Alors $H$ est un sous-groupe de Lie réel de $G$ (th. 2). Soit $a \in L(H)$. Il existe un voisinage ouvert connexe $W$ de $0$ dans $\mathbf{C}$ tel que $\exp \lambda a \in V$ pour tout $\lambda \in W$. Soit $i \in I$. On a $f_i(\exp \lambda a) = f_i(e)$ si $\lambda \in \mathbf{R} \cap W$. Donc $f_i(\exp \lambda a) = f_i(e)$ si $\lambda \in W$ par prolongement analytique. Ainsi, $\exp \lambda a \in H$ pour $\lambda \in W$, et par suite $\mu a \in L(H)$ pour tout $\mu \in \mathbf{C}$. Par suite, $H$ est un sous-groupe de Lie du groupe de Lie complexe $G$ (\S 4, n° 2, prop. 2).

(ii) Supposons que $K$ soit une extension de degré fini de $\mathbf{Q}_p$. Considérons $G$ comme un groupe de Lie sur $\mathbf{Q}_p$. Il est de dimension finie, et le th. 2 implique que $H$ est un sous-groupe de Lie $p$-adique de $G$. Puisque $I$ est fini, $\prod_{i \in I} M_i$ est une variété, et on peut supposer que la famille $(f_i)$ se réduit à une seule application $f$. Soit $a \in L(G)$. Soit $\varphi$ une application exponentielle de $G$. On a $f(\varphi(\lambda a)) = f(e)$ pour $\lambda \in \mathbf{Q}_p$ et $|\lambda|$ assez petit. Puisque $f$ est $K$-analytique, on en déduit que $f(\varphi(\lambda a)) = f(e)$ pour $\lambda \in K$ et $|\lambda|$ assez petit. Donc $\varphi(\lambda a) \in H$ pour $\lambda \in K$ et $|\lambda|$ assez petit, et par suite $\mu a \in L(H)$ pour tout $\mu \in K$. On termine comme dans (i).

Le cor. 2 (ii) devient inexact si l’on omet l’hypothèse que I est fini.

## EXERCICES {#lie-iii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
