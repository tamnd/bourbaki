---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Algèbres de Lie
section: 2
section_title: Algèbre enveloppante d’une algèbre de Lie
lang: fr
source: lie-i-fr
pdf_pages: 0020-0036, 0108-0111
extraction: ocr
subsections:
    - "no": 1
      title: Définition de l’algèbre enveloppante
      page: 0
      pdf_page: 20
    - "no": 2
      title: Algèbre enveloppante d’un produit d’algèbres de Lie
      page: 0
      pdf_page: 21
    - "no": 3
      title: Algèbre enveloppante d’une sous-algèbre de Lie
      page: 0
      pdf_page: 22
    - "no": 4
      title: Algèbre enveloppante de l’algèbre de Lie opposée
      page: 0
      pdf_page: 24
    - "no": 5
      title: Algèbre symétrique d’un module
      page: 0
      pdf_page: 24
    - "no": 6
      title: Filtration de l’algèbre enveloppante
      page: 0
      pdf_page: 25
    - "no": 7
      title: Le théorème de Poincaré-Birkhoff-Witt
      page: 0
      pdf_page: 28
    - "no": 8
      title: Prolongement des dérivations
      page: 0
      pdf_page: 33
    - "no": 9
      title: Extension de l’anneau de base
      page: 0
      pdf_page: 36
statements: 22
exercises: 10
content_sha256: c4c76c8e191b939527d3fa46a4177ccff60ede09336418aa449b43166a4c5cb2
---

## § 2. Algèbre enveloppante d’une algèbre de Lie

### 1. Définition de l’algèbre enveloppante

Soit g une algèbre de Lie sur K. Pour toute algèbre associative à élément unité L sur K, appelons α-application de g dans L une application K-linéaire σ de g dans L telle que

$$
\sigma([x, y]) = \sigma(x)\sigma(y) - \sigma(y)\sigma(x) \quad (x, y \text{ dans } g)
$$

(autrement dit un homomorphisme de g dans l’algèbre de Lie associée à L).

Si L' est une autre algèbre associative à élément unité sur K et τ un homomorphisme de L dans L' transformant 1 en 1, alors τ o σ est une α-application de g dans L'. Nous allons chercher une algèbre associative à élément unité sur K et une α-application de g dans cette algèbre qui soient universelles (Ens., chap. IV, § 3, n° 1).

#### Définition 1 {#lie-i-s2-def-1 .statement}

Soient g une algèbre de Lie sur K, T l’algèbre tensorielle du K-module g, et J l’idéal bilatère de T engendré par les tenseurs $x \otimes y - y \otimes x - [x, y]$ où $x \in g, y \in g$. L’algèbre associative $U = T / J$ s’appelle l’algèbre enveloppante de g. La restriction à g de l’application canonique de T sur U s’appelle l’application canonique de g dans U.

Soit $T_+$ l’idéal bilatère de T formé des tenseurs dont la composante d’ordre 0 est nulle. Soit $T_0 = K.1$ l’ensemble des éléments d’ordre 0 de T. Soient $U_+$ et $U_0$ les images canoniques de $T_+$ et $T_0$ dans U. Comme $J \subset T_+$, la décomposition en somme directe $T = T_0 + T_+$ entraîne une décomposition en somme directe $U = U_0 + U_+$. L’algèbre U a donc un élément unité distinct de 0, et $U_0 = K.1$. Pour tout $x \in U$, la composante de x dans $U_0$ s’appelle le terme constant de x. Les éléments de terme constant nul forment un idéal bilatère de U, à savoir l’idéal bilatère $U^+$ engendré par l’image canonique de g dans U.

L’algèbre associative U est engendrée par 1 et par l’image canonique de g dans U.

Si $x \in g$ et $y \in g$, $x \otimes y - y \otimes x$ et $[x, y]$ sont congrus dans T modulo J ; donc, si $\sigma_0$ désigne l’application canonique de g dans U, on a :

$$
\sigma_0(x)\sigma_0(y) - \sigma_0(y)\sigma_0(x) = \sigma_0([x, y])
$$

dans U. Autrement dit, $\sigma_0$ est une $\alpha$-application de g dans U.

#### Proposition 1 {#lie-i-s2-prop-1 .statement}

*Soit $\sigma$ une $\alpha$-application de g dans une algèbre associative L à élément unité. Il existe un homomorphisme $\tau$ et un seul de U dans L, transformant 1 en 1, tel que $\sigma = \tau \circ \sigma_0$, $\sigma_0$ désignant l’application canonique de g dans U.*

En effet, soit $\tau'$ l’homomorphisme unique de T dans L qui prolonge $\sigma$ et qui transforme 1 en 1. On a, pour $x, y$ dans g,

$$
\tau'(x \otimes y - y \otimes x - [x, y]) = \sigma(x)\sigma(y) - \sigma(y)\sigma(x) - \sigma([x, y]) = 0 ;
$$

donc $\tau'$ s’annule sur J et définit par passage au quotient un homomorphisme $\tau$ de U dans L, transformant 1 en 1, tel que $\sigma = \tau \circ \sigma_0$. L’unicité de $\tau$ est immédiate puisque $\sigma_0(g)$ et 1 engendrent l’algèbre U.

Soient $g'$ une autre algèbre de Lie sur K, $U'$ son algèbre enveloppante, $\sigma'_0$ l’application canonique de $g'$ dans $U'$. Soit $\varphi$ un homomorphisme de g dans $g'$. Alors $\sigma'_0 \circ \varphi$ est une $\alpha$-application de g dans $U'$; donc il existe un homomorphisme $\tilde{\varphi}$ et un seul de U dans $U'$ transformant 1 en 1 et tel que le diagramme

$$
\begin{array}{ccc}
g & \xrightarrow{\varphi} & g' \\
\sigma_0 \downarrow & & \downarrow \sigma'_0 \\
U & \xrightarrow{\tilde{\varphi}} & U'
\end{array}
$$

soit commutatif. Cet homomorphisme transforme les éléments de U dont le terme constant est nul en éléments de $U'$ dont le terme constant est nul. Si $g''$ est une autre algèbre de Lie sur K, et si $\varphi'$ est un homomorphisme de $g'$ dans $g''$, on a $(\varphi' \circ \varphi)^{\sim} = \tilde{\varphi}' \circ \tilde{\varphi}$.

### 2. Algèbre enveloppante d’un produit d’algèbres de Lie

Soient $g_1, g_2$ deux algèbres de Lie sur K, $U_i$ l’algèbre enveloppante de $g_i$, et $\sigma_i$ l’application canonique de $g_i$ dans $U_i$ ($i = 1, 2$). Soient $g = g_1 \times g_2$, U son algèbre enveloppante, et $\sigma$ l’application canonique de g dans U. Les injections canoniques de g₁ et g₂ dans g définissent des homomorphismes canoniques de U₁ et U₂ dans U dont les images commutent, donc un homomorphisme φ de l’algèbre U₁ ⊗ₖ U₂ dans l’algèbre U, transformant 1 en 1.

#### Proposition 2 {#lie-i-s2-prop-2 .statement}

*L’homomorphisme φ est un isomorphisme d’algèbres.*

L’application σ′ : (x₁, x₂) ↦ σ₁(x₁) ⊗ 1 + 1 ⊗ σ₂(x₂) (x₁ ∈ g₁, x₂ ∈ g₂) est une α-application de g dans U₁ ⊗ₖ U₂, donc il existe (n° 1, prop. 1) un homomorphisme unique τ de U dans U₁ ⊗ₖ U₂ transformant 1 en 1, tel que :

(1)
$$
σ′ = τ \circ σ.
$$

On a φ ∘ τ ∘ σ = φ ∘ σ′ = σ, et τ ∘ φ ∘ σ′ = τ ∘ σ = σ′, donc φ ∘ τ et τ ∘ φ sont les applications identiques de U et U₁ ⊗ₖ U₂ respectivement. D’où la proposition.

On identifie U₁ ⊗ₖ U₂ à U par l’isomorphisme φ. Alors, l’application canonique de g dans U s’identifie, d’après (1), à l’application :
$$
(x₁, x₂) ↦ σ₁(x₁) ⊗ 1 + 1 ⊗ σ₂(x₂).
$$

De façon analogue, si g₁, ..., gₙ sont des algèbres de Lie sur K, d’algèbres enveloppantes U₁, ..., Uₙ, l’algèbre enveloppante U de g₁ × ... × gₙ s’identifie canoniquement à U₁ ⊗ₖ ... ⊗ₖ Uₙ, et l’application canonique de g₁ × ... × gₙ dans U s’identifie à l’application :
$$
(x₁, ..., xₙ) ↦ σ₁(x₁) ⊗ 1 ⊗ ... ⊗ 1 + ... + 1 ⊗ ... ⊗ 1 ⊗ σₙ(xₙ)
$$
(en désignant par σᵢ l’application canonique de gᵢ dans Uᵢ).

### 3. Algèbre enveloppante d’une sous-algèbre de Lie

Soient g une algèbre de Lie sur K, h une sous-algèbre de g, et σ, σ′ les applications canoniques de g, h dans leurs algèbres enveloppantes U, V. Alors l’injection canonique i de h dans g définit un homomorphisme $\tilde{i}$, dit *canonique*, de V dans U, tel que $σ \circ i = \tilde{i} \circ σ'$. L’algèbre $\tilde{i}(V)$ est engendrée par 1 et $σ(h)$. On verra (n° 7, cor. 5 du th. 1) que $\tilde{i}$ est injectif dans des cas importants.

Si $\mathfrak{h}$ est un idéal de $g$, l’idéal à gauche de U engendré par $\sigma(\mathfrak{h})$ coïncide avec l’idéal à droite engendré par $\sigma(\mathfrak{h})$, autrement dit est un idéal bilatère R. En effet, pour $x \in \mathfrak{h}$ et $x' \in g$, on a
$$
\sigma(x)\sigma(x') = \sigma(x')\sigma(x) + \sigma([x, x'])
$$
et $[x, x'] \in \mathfrak{h}$.

#### Proposition 3 {#lie-i-s2-prop-3 .statement}

*Soient $\mathfrak{h}$ un idéal de $g$, p l’homomorphisme canonique de $g$ sur $g/\mathfrak{h}$, et W l’algèbre enveloppante de $g/\mathfrak{h}$. L’homomorphisme :*
$$
\tilde{p} : U \to W
$$
*défini canoniquement par p est surjectif et son noyau est l’idéal R de U engendré par $\sigma(\mathfrak{h})$.*

Soit $\sigma''$ l’application canonique de $g/\mathfrak{h}$ dans W. Le diagramme commutatif :
$$
\begin{array}{ccccc}
\mathfrak{h} & \xrightarrow{i} & g & \xrightarrow{p} & g/\mathfrak{h} \\
\sigma' \downarrow & & \sigma \downarrow & & \downarrow \sigma'' \\
V & \xrightarrow{\tilde{i}} & U & \xrightarrow{\tilde{p}} & W
\end{array}
$$
prouve que $\tilde{p}$ s’annule sur $\sigma(\mathfrak{h})$, donc sur R. Soit $\psi$ l’homomorphisme canonique de U sur U/R. Il existe un homomorphisme $\varphi$ de U/R dans W tel que $\tilde{p} = \varphi \circ \psi$. L’application $\psi \circ \sigma$ de g dans U/R est une $\alpha$-application et s’annule sur $\mathfrak{h}$, donc définit une $\alpha$-application $\theta$ de $g/\mathfrak{h}$ dans U/R telle que $\theta \circ p = \psi \circ \sigma$. On a alors $\varphi \circ \theta \circ p = \varphi \circ \psi \circ \sigma = \sigma'' \circ p$. D’où $\varphi \circ \theta = \sigma''$. Il existe (n° 1, prop. 1) un homomorphisme $\varphi'$ et un seul de W dans U/R transformant 1 en 1 et tel que $\theta = \varphi' \circ \sigma''$. Alors, $\varphi' \circ \varphi \circ \theta = \varphi' \circ \sigma'' = \theta$ et $\varphi \circ \varphi' \circ \sigma'' = \varphi \circ \theta = \sigma''$, donc $\varphi' \circ \varphi$ et $\varphi \circ \varphi'$ sont les applications identiques de U/R et W respectivement. Ceci achève la démonstration.

On identifie U/R à W par l’isomorphisme $\varphi$. Alors, l’application canonique $\sigma''$ de $g/\mathfrak{h}$ dans W s’identifie à $\theta$, c’est-à-dire à l’application de $g/\mathfrak{h}$ dans U/R déduite de $\sigma$ par passage aux quotients.

### 4. Algèbre enveloppante de l’algèbre de Lie opposée

Soient g une algèbre de Lie sur K, g^0 l’algèbre de Lie opposée, σ et σ_0 les applications canoniques de g et g^0 dans leurs algèbres enveloppantes U et V. Alors, σ est une α-application de g^0 dans l’algèbre associative U^0 opposée à l’algèbre associative U. Donc il existe un homomorphisme φ et un seul de V dans U^0 transformant 1 en 1 et tel que σ = φ ∘ σ_0.

#### Proposition 4 {#lie-i-s2-prop-4 .statement}

L’homomorphisme φ est un isomorphisme de V sur U^0.

En effet, il existe un homomorphisme φ’ de U dans V^0 transformant 1 en 1 et tel que σ_0 = φ’ ∘ σ. On peut considérer φ’ comme un homomorphisme de U^0 dans V. On a σ_0 = φ’ ∘ φ ∘ σ_0, et σ = φ ∘ φ’ ∘ σ, donc φ’ ∘ φ et φ ∘ φ’ sont les applications identiques de V et U. D’où la proposition.

On identifie V à U^0 par l’isomorphisme φ. Alors, σ_0 s’identifie à σ.

Ceci posé, l’isomorphisme θ : x ↦ −x de g sur g^0 définit un isomorphisme ŝ de U sur V = U^0. Cet isomorphisme peut être considéré comme un antiautomorphisme de U. On l’appelle l’anti-automorphisme principal de U. Si x_1, ..., x_n sont dans g, on a :

(2) $\tilde{\theta}(\sigma(x_1) ... \sigma(x_n)) = \tilde{\theta}(\sigma(x_n)) ... \tilde{\theta}(\sigma(x_1)) = (-\sigma(x_n)) ... (-\sigma(x_1))$
$= (-1)^n \sigma(x_n) ... \sigma(x_1).$

### 5. Algèbre symétrique d’un module

Soit V un K-module. On peut, d’une manière unique, considérer V comme une algèbre de Lie commutative. L’algèbre enveloppante de V s’obtient alors de la manière suivante : soit T l’algèbre tensorielle de V ; soit I l’idéal bilatère de T engendré par les tenseurs x ⊗ y − y ⊗ x (x ∈ V, y ∈ V) ; on forme l’algèbre S = T/I.

Rappelons (Alg., chap. III, 3e éd., § 6) que S est appelée algèbre symétrique de V, et résumons brièvement les propriétés dont nous aurons besoin dans ce chapitre et dont les démonstrations sont immédiates. Soit T^n l’ensemble des tenseurs homogènes d’ordre $n$ dans $T$. On a $I = (I \cap T^2) + (I \cap T^3) + ...$, donc $S$ est somme directe des images canoniques $S^n$ des $T^n$. Les éléments de $S^n$ sont dits homogènes de degré $n$. On a $S^0 = K.1$, $S^1$ s’identifie à $V$, et $S^n S^p \subset S^{n+p}$. L’algèbre $S$ est engendrée par 1 et $S^1 = V$. Il est clair que deux éléments quelconques de $S^1$ sont permutables, donc $S$ est commutative. Si $V$ est un $K$-module libre de base $(x_\lambda)_{\lambda \in \Lambda}$, l’homomorphisme canonique $f$ de l’algèbre de polynômes $K[X_\lambda]_{\lambda \in \Lambda}$ sur $S$ qui transforme 1 en 1 et $X_\lambda$ en $x_\lambda$ pour tout $\lambda \in \Lambda$ est un isomorphisme : en effet, d’après la propriété universelle de $S$ (no 1, prop. 1), il existe un homomorphisme $g$ de $S$ dans $K[X_\lambda]_{\lambda \in \Lambda}$ qui transforme 1 en 1 et $x_\lambda$ en $X_\lambda$ pour tout $\lambda \in \Lambda$, et $f, g$ sont deux homomorphismes réciproques l’un de l’autre.

Soit ${S'}^n \subset T^n$ l’ensemble des tenseurs symétriques homogènes d’ordre $n$ ($Alg.$, chap. III, § 5, no 1, déf. 2). Si $K$ est un corps de caractéristique 0, ${S'}^n$ et $I \cap T^n$ sont supplémentaires dans $T^n$. En effet, soit $(x_\lambda)_{\lambda \in \Lambda}$ une base de $V$. Ordonnons totalement $\Lambda$ ($Ens.$, chap. III, § 2, no 3, th. 1). Soit $\Lambda_n$ l’ensemble des suites croissantes de $n$ éléments de $\Lambda$. Pour $M = (\lambda_1, \ldots, \lambda_n) \in \Lambda_n$, soit

$$
y_M = \frac{1}{n!} \sum_{\sigma \in S_n} x_{\lambda_{\sigma(1)}} \otimes \cdots \otimes x_{\lambda_{\sigma(n)}}.
$$

Les $y_M$, pour $M \in \Lambda_n$, forment un système de générateurs du $K$-espace vectoriel ${S'}^n$. Or, leurs images canoniques dans $S^n$ constituent, d’après l’alinéa précédent, une base de $S^n$. Donc $(y_M)_{M \in \Lambda_n}$ est une base d’un supplémentaire de $I \cap T^n$ dans $T^n$ ($Alg.$, chap. II, § 1, no 6, prop. 4), ce qui établit notre assertion.

Ainsi, lorsque $K$ est un corps de caractéristique 0, la restriction à ${S'}^n$ de l’application canonique : $T^n \to S^n$, est un isomorphisme de l’espace ${S'}^n$ sur l’espace $S^n$, et possède donc un isomorphisme réciproque. Les isomorphismes réciproques ainsi obtenus pour chaque $n$ définissent un isomorphisme canonique de l’espace $S$ sur l’espace $S' = \sum_{n \geq 0} {S'}^n$ des tenseurs symétriques.

### 6. Filtration de l’algèbre enveloppante

Soient $g$ une algèbre de Lie sur $K$, et $T$ l’algèbre tensorielle du $K$-module $g$. Soient $T^n$ le sous-module de $T$ formé des tenseurs

Soit $G^n$ le $K$-module $U_n / U_{n-1}$, et soit $G$ le $K$-module somme directe des $G^n$. La multiplication sur $U$ définit, par passage aux quotients, une application bilinéaire de $G^n \times G^m$ dans $G^{n+m}$, donc une application bilinéaire de $G \times G$ dans $G$, qui est associative. Ainsi, $G$ est muni d’une structure de $K$-algèbre associative. On a $G^n G^m \subset G^{n+m}$. Les éléments de $G^n$ sont dits de degré $n$. L’algèbre graduée ainsi obtenue n’est autre que l’algèbre graduée associée à l’algèbre filtrée $U$ (*Alg. comm.*, chap. III, § 2, no 3).

Soit $\varphi_n$ la composée des applications $K$-linéaires canoniques

$$
T^n \longrightarrow U_n \longrightarrow G^n.
$$

Comme $T^n$ est supplémentaire de $T_{n-1}$ dans $T_n$, $\varphi_n$ est surjective. Les $\varphi_n$ définissent une application $K$-linéaire $\varphi$ de $\sum_n T^n = T$ sur $\sum_n G^n = G$.

#### Proposition 5 {#lie-i-s2-prop-5 .statement}

*L’application $\varphi$ de $T$ sur $G$ est un homomorphisme d’algèbres transformant 1 en 1, et s’annule sur l’idéal bilatère engendré par les tenseurs $x \otimes y - y \otimes x$ ($x \in g, y \in g$).

Si $t \in T^n$ et $t' \in T^p$, on a $\varphi(t)\varphi(t') = \varphi(tt')$ par définition de la multiplication dans $G$. Donc $\varphi$ est un homomorphisme d’algèbres, et il est clair que $\varphi(1) = 1$. Si $x, y$ sont dans $g$, on a $x \otimes y - y \otimes x \in T^2$, et l’image canonique de cet élément dans $U_2$ est égale à celle de $[x, y]$, donc appartient à $U_1$. Donc $\varphi(x \otimes y - y \otimes x) = 0$, ce qui prouve la proposition.

Soient $S$ l’algèbre symétrique du $K$-module $g$ et $\tau$ l’homomorphisme canonique de $T$ sur $S$. La prop. 5 prouve qu’il existe un homomorphisme unique $\omega$, dit canonique, de l’algèbre $S$ sur l’algèbre $G$, transformant 1 en 1, tel que $\varphi = \omega \circ \tau$. On a $\omega(S^n) = \varphi(T^n) = G^n$. Soient $\tau_n$ la restriction de $\tau$ à $T^n$, $\omega_n$ la restriction de ω à S^n, ψ_n l’application canonique de T^n dans U_n, et θ_n l’application canonique de U_n sur G^n. La définition de ω_n prouve que le diagramme suivant est commutatif :

$$
\begin{array}{ccc}
 & & U_n \\
T^n & \xrightarrow{\psi_n} & U_n \\
 & \searrow & \downarrow \theta_n \\
 & & G^n \\
 & \swarrow & \downarrow \omega_n \\
 & & S^n \\
\end{array}
$$

(3)

#### Proposition 6 {#lie-i-s2-prop-6 .statement}

Si K est noethérien et si g est un module de type fini, l’anneau U est noethérien à droite et à gauche.

En effet, S est une algèbre de type fini sur K, donc un anneau noethérien (Alg. comm., chap. III, § 2, no 10, cor. 3 du th. 2). Donc G, qui est isomorphe à un anneau quotient de S, est noethérien. Donc U est noethérien à droite et à gauche (Alg. comm., chap. III, § 2, no 10, Remarque 2).

#### Corollaire {#lie-i-s2-n6-cor-1 .statement}

On suppose que K est un corps, et que g est de dimension finie sur K. Soient I_1, ..., I_m des idéaux à droite (resp. à gauche) de codimension finie de U. Alors l’idéal produit I_1I_2...I_m est de codimension finie.

Par récurrence sur m, il suffit d’envisager le cas de deux idéaux à droite par exemple. Le U-module à droite I_1 est engendré par un nombre fini d’éléments u_1, ..., u_p (prop. 6). Soient v_1, ..., v_q des éléments de U dont les classes modulo I_2 engendrent l’espace vectoriel U/I_2. Alors les images canoniques dans I_1/I_1I_2 des u_i v_j engendrent l’espace vectoriel I_1/I_1I_2, qui est donc de dimension finie. Par suite dim_K(U/I_1I_2) = dim_K(U/I_1) + dim_K(I_1/I_1I_2) < +∞.

#### Remarque {#lie-i-s2-n6-rem-1 .statement}

Soient g’ une autre algèbre de Lie sur l’anneau K, U’ son algèbre enveloppante, U'_n l’ensemble des éléments de U’ de filtration ≤ n, U^n (resp. U'^n) l’ensemble des images canoniques dans U (resp. U’) des tenseurs symétriques homogènes d’ordre n de g (resp. g’). Soit γ un homomorphisme de g dans g’, et soit $\tilde{\gamma}$ l’homomorphisme correspondant de U dans U’. On a

$$ \tilde{\gamma}(U_n) \subset U'_n, \quad \tilde{\gamma}(U^n) \subset {U'}^n. $$

En particulier, l’antiautomorphisme principal de U laisse stables U_n et U^n. L’application K-linéaire de T^n sur lui-même qui transforme $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ en $x_n \otimes x_{n-1} \otimes \cdots \otimes x_1$ quels que soient $x_1, ..., x_n$ dans g est un opérateur de symétrie, donc laisse fixes les tenseurs symétriques homogènes d’ordre n. Donc l’antiautomorphisme principal de U induit dans chaque U^n l’homothétie de rapport (−1)^n.

### 7. Le théorème de Poincaré-Birkhoff-Witt

#### Théorème 1 {#lie-i-s2-thm-1 .statement}

Soient g une K-algèbre de Lie, U son algèbre enveloppante, G l’algèbre graduée associée à l’algèbre filtrée U, et S l’algèbre symétrique du K-module g. Si g est un K-module libre, l’homomorphisme canonique ω : S → G est un isomorphisme.

En effet, soit (x_λ)_{λ ∈ Λ} une base du K-module g ; munissons Λ d’une structure d’ordre total (Ens., chap. III, § 2, no 3, th. 1). Soit P l’algèbre de polynômes K[z_λ]_{λ ∈ Λ} par rapport à des lettres z_λ en correspondance biunivoque avec les x_λ. Pour toute suite M = (λ₁, λ₂, ..., λ_n) d’éléments de Λ, on désignera par z_M le monôme z_{λ₁}z_{λ₂}...z_{λ_n}, par x_M le tenseur x_{λ₁} ⊗ x_{λ₂} ⊗ ... ⊗ x_{λ_n}.

Les z_M, pour M croissante, forment une base du K-module P (on convient que ∅ est une suite croissante, et que z_∅ = 1). Soit P_p le sous-module des polynômes de degré ≤ p. Nous démontrerons d’abord plusieurs lemmes. (Pour abréger, on écrit λ ≤ M si λ ≤ μ pour tout indice μ de la suite M.)

#### Lemme 1 {#lie-i-s2-lem-1 .statement}

Pour tout entier p ≥ 0, il existe un homomorphisme unique f_p du K-module g ⊗_K P_p dans le K-module P vérifiant les conditions suivantes :

(A_p) $f_p(x_λ ⊗ z_M) = z_λ z_M$ pour $λ ≤ M, z_M ∈ P_p$;
(B_p) $f_p(x_λ ⊗ z_M) - z_λ z_M ∈ P_q$ pour $z_M ∈ P_q, q ≤ p$;
(C_p) $f_p(x_λ ⊗ f_p(x_μ ⊗ z_N)) = f_p(x_μ ⊗ f_p(x_λ ⊗ z_N)) + f_p([x_λ, x_μ] ⊗ z_N)$
pour $z_N ∈ P_{p-1}$. (Les termes intervenant dans (C_p) ont un sens grâce à la condition (B_p).)

En outre, la restriction de f_p à g ⊗ P_{p-1} coïncide avec f_{p-1}.

La dernière assertion résulte des précédentes puisque la restriction de f_p à g ⊗_K P_{p-1} vérifie les conditions (A_{p-1}), (B_{p-1}), (C_{p-1}). Nous allons prouver l’existence et l’unicité de f_p par récurrence sur p. Pour p = 0, la condition (A_0) impose $f_0(x_λ ⊗ 1) = z_λ$ et les conditions (B_0), (C_0) sont alors évidemment satisfaites. Supposons maintenant prouvées l’existence et l’unicité de f_{p-1}. Montrons que f_{p-1} admet une extension unique $f_p$ à $g \otimes_k P_p$ satisfaisant aux conditions $(A_p), (B_p), (C_p)$.

Nous devons définir $f_p(x_\lambda \otimes z_M)$ pour une suite croissante M de $p$ éléments.

Si $\lambda \leq M$, le choix est imposé par la condition $(A_p)$. Dans le cas contraire, M s’écrit de manière unique sous la forme $(\mu, N)$, où $\mu < \lambda, \mu \leq N$. Alors, $z_M = z_\mu z_N = f_{p-1}(x_\mu \otimes z_N)$ d’après $(A_{p-1})$, de sorte que le premier membre de $(C_p)$ est $f_p(x_\lambda \otimes z_M)$. Or, le deuxième membre de $(C_p)$ est déjà défini ; en effet, $(B_{p-1})$ permet d’écrire :

$$
f_p(x_\lambda \otimes z_N) = f_{p-1}(x_\lambda \otimes z_N) = z_\lambda z_N + \omega
$$

avec $\omega \in P_{p-1}$; donc le deuxième membre de $(C_p)$ devient :

$$
z_\mu z_\lambda z_N + f_{p-1}(x_\mu \otimes \omega) + f_{p-1}([x_\lambda, x_\mu] \otimes z_N).
$$

Ainsi, $f_p$ est définie de manière unique, et satisfait évidemment aux conditions $(A_p)$ et $(B_p)$. La condition $(C_p)$ est satisfaite si $\mu < \lambda, \mu \leq N$. Comme $[x_\mu, x_\lambda] = -[x_\lambda, x_\mu]$, la condition $(C_p)$ est aussi satisfaite pour $\lambda < \mu, \lambda \leq N$. Comme $(C_p)$ est trivialement satisfaite pour $\lambda = \mu$, $(C_p)$ est donc satisfaite si l’on a $\lambda \leq N$ ou $\mu \leq N$. Si aucune de ces inégalités n’est vérifiée, on a $N = (\nu, Q)$, où $\nu \leq Q, \nu < \lambda, \nu < \mu$. Posant désormais pour abréger $f_p(x \otimes z) = xz$ pour $x \in g$ et $z \in P_p$, on a, d’après l’hypothèse de récurrence :

$$
x_\mu z_N = x_\mu(x_\nu z_Q) = x_\nu(x_\mu z_Q) + [x_\mu, x_\nu]z_Q.
$$

Or, $x_\mu z_Q$ est de la forme $z_\mu z_Q + \omega$, où $\omega \in P_{p-2}$. On peut appliquer $(C_p)$ à $x_\lambda(x_\nu(z_\mu z_Q))$ parce que $\nu \leq Q$ et $\nu < \mu$, et à $x_\lambda(x_\nu \omega)$ en vertu de l’hypothèse de récurrence, donc à $x_\lambda(x_\nu(x_\mu z_Q))$. D’où :

$$
x_\lambda(x_\mu z_N) = x_\nu(x_\lambda(x_\mu z_Q)) + [x_\lambda, x_\nu](x_\mu z_Q) + [x_\mu, x_\nu](x_\lambda z_Q)
+ [x_\lambda, [x_\mu, x_\nu]]z_Q.
$$

En échangeant $\lambda$ et $\mu$, et retranchant membre à membre :

$$
x_\lambda(x_\mu z_N) - x_\mu(x_\lambda z_N) = x_\nu(x_\lambda(x_\mu z_Q) - x_\mu(x_\lambda z_Q))
+ [x_\lambda, [x_\mu, x_\nu]]z_Q - [x_\mu, [x_\lambda, x_\nu]]z_Q
$$
$$
= x_\nu([x_\lambda, x_\mu]z_Q) + [x_\lambda, [x_\mu, x_\nu]]z_Q + [x_\mu, [x_\nu, x_\lambda]]z_Q
= [x_\lambda, x_\mu](x_\nu z_Q) + ([x_\nu, [x_\lambda, x_\mu]]) + [x_\lambda, [x_\mu, x_\nu]] + [x_\mu, [x_\nu, x_\lambda]])z_Q
$$

soit, en vertu de l’identité de Jacobi

$$
x_\lambda(x_\mu z_N) - x_\mu(x_\lambda z_N) = [x_\lambda, x_\mu]z_N
$$

ce qui achève la démonstration du lemme 1.

#### Lemme 2 {#lie-i-s2-lem-2 .statement}

*Il existe une α-application σ de g dans $\mathcal{L}_K(P)$ telle que* :

$1^\circ$ $\sigma(x_\lambda)z_M = z_\lambda z_M$ pour $\lambda \leq M$;
$2^\circ$ $\sigma(x_\lambda)z_M \equiv z_\lambda z_M$ (mod. $P_p$) si $M$ a $p$ éléments.

En effet, d’après le lemme 1, il existe un homomorphisme $f$ du K-module $g \otimes_K P$ dans $P$ vérifiant, quel que soit $p$, les conditions (A_p), (B_p), (C_p) (où l’on remplace $f_p$ par $f$). Cet homomorphisme définit un homomorphisme $\sigma$ du K-module $g$ dans le K-module $\mathcal{L}_K(P)$, et $\sigma$ est une $\alpha$-application à cause de la condition (C_p). Enfin, $\sigma$ vérifie les propriétés $1^\circ$ et $2^\circ$ du lemme à cause des conditions (A_p) et (B_p).

#### Lemme 3 {#lie-i-s2-lem-3 .statement}

*Soit t un tenseur de $T_n \cap J$. La composante homogène $t_n$ d’ordre $n$ de $t$ est dans le noyau I de l’homomorphisme canonique $T \to S$*.

En effet, écrivons $t_n$ sous la forme $\sum_{i=1}^r x_{M_i}$, où les $M_i$ sont des suites de $n$ éléments de $\Lambda$. L’application $\sigma$ se prolonge en un homomorphisme de l’algèbre $T$ dans l’algèbre $\mathcal{L}_K(P)$ (que nous noterons encore $\sigma$), qui s’annule sur $J$. D’après le lemme 2, $\sigma(t).1$ est un polynôme dont les termes de plus haut degré sont $\sum_{i=1}^r z_{M_i}$. Comme $t \in J$, on a $\sigma(t) = 0$, donc $\sum_{i=1}^r z_{M_i} = 0$ dans $P$. Or, $P$ s’identifie canoniquement à $S$, grâce à la donnée de la base $(x_\lambda)$ de $g$. Donc l’image canonique de $t_n$ dans $S$ est nulle, c’est-à-dire que $t_n \in I$.

Nous pouvons maintenant démontrer le théorème 1. Il faut prouver que l’homomorphisme canonique de $S$ sur $G$ est injectif. Autrement dit, si $t \in T^n$ et si $\psi$ désigne l’homomorphisme canonique de $T$ sur $U$, il faut montrer que la condition $\psi(t) \in U_{n-1}$ entraîne $t \in I$. Or $\psi(t) \in U_{n-1}$ signifie qu’il existe un tenseur $t' \in T_{n-1}$ tel que $t - t' \in J$. Le tenseur $t - t'$ admet $t$ pour composante homogène d’ordre $n$, donc $t \in I$ d’après le lemme 3.

#### Corollaire 1 {#lie-i-s2-lem-3-cor-1 .statement}

Supposons que g soit un K-module libre. Soit W un sous-K-module de T^n. Si, avec les notations du diagramme (3), la restriction de τ_n à W est un isomorphisme de W sur S^n, alors la restriction de ψ_n à W est un isomorphisme de W sur un supplémentaire de U_{n-1} dans U_n.

En effet, la restriction à W de ω_n ∘ τ_n est une bijection de W sur G^n ; il en est donc de même de la restriction de θ_n ∘ ψ_n à W. D’où le corollaire.

#### Corollaire 2 {#lie-i-s2-lem-3-cor-2 .statement}

Si g est un K-module libre, l’application canonique de g dans son algèbre enveloppante est injective.

Ceci résulte du cor. 1, où l’on prend W = T^1.

Lorsque g est un K-module libre (en particulier lorsque K est un corps), on identifie g à un sous-module de U par l’application canonique de g dans U. Cette convention est adoptée dès le corollaire suivant.

#### Corollaire 3 {#lie-i-s2-lem-3-cor-3 .statement}

Si g admet une base totalement ordonnée (x_λ)_{λ ∈ Λ}, les éléments x_{λ_1} x_{λ_2} ... x_{λ_n} de l’algèbre enveloppante U, où (λ_1, ..., λ_n) est une suite finie croissante quelconque d’éléments de Λ, forment une base du K-module U.

Soit Λ_n l’ensemble des suites croissantes de n éléments de Λ. Pour M = (λ_1, ..., λ_n) ∈ Λ_n, soit y_M = x_{λ_1} ⊗ x_{λ_2} ⊗ ... ⊗ x_{λ_n}. Soit W le sous-module de T^n qui admet pour base (y_M)_{M ∈ Λ_n}. Le cor. 1 montre que la restriction de ψ_n à W est un isomorphisme de W sur un supplémentaire de U_{n-1} dans U_n. Or, ψ_n(y_M) = x_{λ_1} x_{λ_2} ... x_{λ_n}, d’où le corollaire.

#### Corollaire 4 {#lie-i-s2-lem-3-cor-4 .statement}

Soit S'^n ⊂ T^n l’ensemble des tenseurs symétriques homogènes d’ordre n. Supposons que K soit un corps de caractéristique 0. Alors, l’application composée des applications canoniques

$$
S^n \longrightarrow {S'}^n \longrightarrow U_n
$$

est un isomorphisme de l’espace vectoriel S^n sur un supplémentaire de U_{n-1} dans U_n.

Ceci résulte du cor. 1, où l’on prend W = S'^n.

Supposons toujours que K soit un corps de caractéristique 0.

Soit $\eta_n$ l’application de $S^n$ dans $U_n$ qu’on vient de définir. Soit $U^n = \eta_n(S^n)$. L’espace vectoriel $U$ est somme directe des $U^n$. Les $\eta_n$ définissent un isomorphisme $\gamma$ de l’espace vectoriel $S = \sum_n S^n$ sur l’espace vectoriel $U = \sum_n U^n$, appelé *isomorphisme canonique de S sur U* ; ce n’est *pas* un isomorphisme d’algèbre. On a le diagramme commutatif :

$$
\begin{array}{ccc}
& & U^n \\
& \nearrow \psi_n & \searrow \theta_n \\
{S'}^n & & G^n \\
\swarrow \tau_n & & \nwarrow \omega_n \\
& & S^n
\end{array}
$$

où chaque flèche représente un isomorphisme d’espaces vectoriels. Si $x_1, x_2, \ldots, x_n$ sont dans $g$, $\eta_n$ transforme le produit $x_1 x_2 \ldots x_n$, calculé dans $S$, en l’élément $\frac{1}{n!} \sum_{\sigma \in S_n} x_{\sigma(1)} x_{\sigma(2)} \ldots x_{\sigma(n)}$ calculé dans $U$.

#### Corollaire 5 {#lie-i-s2-lem-3-cor-5 .statement}

*Soient $\mathfrak{h}$ une sous-algèbre de l’algèbre de Lie $g$ et $U'$ son algèbre enveloppante. Supposons que les K-modules $\mathfrak{h}$ et $g/\mathfrak{h}$ soient libres (par exemple que $K$ soit un corps). Soit $(x_\alpha)_{\alpha \in L}$ une base de $\mathfrak{h}$, et $(y_\beta)_{\beta \in M}$ une famille d’éléments de $g$ dont les images canoniques dans $g/\mathfrak{h}$ forment une base de $g/\mathfrak{h}$.

a) *L’homomorphisme canonique de $U'$ dans $U$ est injectif*.

b) *Si $M$ est totalement ordonné, les éléments $y_{\beta_1} \ldots y_{\beta_q}$, où $\beta_1 \leq \cdots \leq \beta_q$, forment une base de $U$ considéré comme module à gauche ou à droite sur $U'$*.

Munissons $L \cup M$ d’une structure d’ordre total telle que tout élément de $L$ soit majoré par tout élément de $M$. Les éléments $x_{\alpha_1} x_{\alpha_2} \ldots x_{\alpha_p}$ calculés dans $U'$ (où $\alpha_1 \leq \cdots \leq \alpha_p$) forment une base de $U'$ (cor. 3). Les éléments $x_{\alpha_1} \ldots x_{\alpha_p} y_{\beta_1} \ldots y_{\beta_q}$ calculés dans $U$ (où $\alpha_1 \leq \cdots \leq \alpha_p \leq \beta_1 \leq \cdots \leq \beta_q$) forment de même une base de $U$. Donc l’homomorphisme canonique de $U'$ dans $U$ transforme les éléments d’une base de $U'$ en éléments linéairement indépendants de $U$, et par suite est injectif. On voit en outre que les $y_{\beta_1} \ldots y_{\beta_q}$ (où $\beta_1 \leq \cdots \leq \beta_q$) forment une base de $U$ considéré comme $U'$-module à gauche. En ordonnant $L \cup M$ de façon que tout élément de $M$ soit majoré par tout élément de $L$, on voit de même que les $y_{\beta_1} \ldots y_{\beta_q}$ (où $\beta_1 \leq \cdots \leq \beta_q$) forment une base de $U$ considéré comme $U'$-module à droite.

Dans les conditions du cor. 5, on identifie U' à la sous-algèbre de U engendrée par h, grâce à l’homomorphisme canonique de U' dans U.

#### Corollaire 6 {#lie-i-s2-lem-3-cor-6 .statement}

Supposons que le K-module g soit somme directe de sous-algèbres g₁, g₂, ..., gₙ, et que chaque gᵢ soit un K-module libre. Soit Uᵢ l’algèbre enveloppante de gᵢ (1 ≤ i ≤ n). Soit φ l’application K-linéaire du K-module U₁ ⊗ₖ ... ⊗ₖ Uₙ dans U définie par l’application multilinéaire (u₁, ..., uₙ) → u₁ ... uₙ de U₁ × ... × Uₙ dans U. Alors φ est un isomorphisme de K-modules.

Soit (xᵢλ)λ∈Lᵢ une base de gᵢ. Ordonnons totalement L₁ ∪ ... ∪ Lₙ de telle manière que tout élément de Lᵢ majore tout élément de Lⱼ pour i ≥ j. Alors les éléments :

$$(x_{λ₁}^{₁} x_{λ₂}^{₁} ... x_{λₚ}^{₁}) ⊗ ... ⊗ (x_{ν₁}^{ⁿ} x_{ν₂}^{ⁿ} ... x_{ν_q}^{ⁿ}),$$

où λ₁ ≤ λ₂ ≤ ... ≤ λₚ ≤ ... ≤ ν₁ ≤ ν₂ ≤ ... ≤ ν_q, constituent une base de U₁ ⊗ₖ ... ⊗ₖ Uₙ. Ils sont transformés par φ en les éléments :

$$x_{λ₁}^{₁} x_{λ₂}^{₁} ... x_{λₚ}^{₁} ... x_{ν₁}^{ⁿ} x_{ν₂}^{ⁿ} ... x_{ν_q}^{ⁿ}$$

qui constituent une base de U. D’où le corollaire.

#### Corollaire 7 {#lie-i-s2-lem-3-cor-7 .statement}

Si K est intègre, et si g est un K-module libre, l’algèbre U est sans diviseur de zéro.

En effet, G est isomorphe à une algèbre de polynômes sur K (th. 1), donc est intègre (Alg., chap. IV, § 1, no 4, th. 1). D’où le corollaire (Alg. comm., chap. III, § 2, no 3, prop. 1).

### 8. Prolongement des dérivations

#### Lemme 4 {#lie-i-s2-lem-4 .statement}

Soient V un K-module, T l’algèbre tensorielle de V. Soit u un endomorphisme de V. Il existe une dérivation de T et une seule qui prolonge u. Cette dérivation permuté aux opérateurs de symétrie dans T.

Soit F = V × V × ... × V (n facteurs). L’application

$$(x₁, ..., xₙ) ↦ ux₁ ⊗ x₂ ⊗ ... ⊗ xₙ + x₁ ⊗ ux₂ ⊗ ... ⊗ xₙ + ... + x₁ ⊗ x₂ ⊗ ... ⊗ uxₙ$$

de F dans $\bigotimes^n V$ est multilinéaire. Donc il existe un endomorphisme $u_n$ de $\bigotimes^n V$ tel que :

$$
u_n(x_1 \otimes \cdots \otimes x_n) = ux_1 \otimes \cdots \otimes x_n + \cdots + x_1 \otimes \cdots \otimes ux_n
$$

quels que soient $x_1, \ldots, x_n$ dans V. On a $u_1 = u$. Soit $\nu$ l’endomorphisme du K-module T qui coïncide avec $u_n$ sur chaque $T^n = \bigotimes^n V$, et qui s’annule dans $T^0 = K.1$. Montrons que $\nu$ est une dérivation de T. Si $x_1, \ldots, x_n, y_1, \ldots, y_p$ sont des éléments de V, on a

$$
\nu((x_1 \otimes \cdots \otimes x_n) \otimes (y_1 \otimes \cdots \otimes y_p))
$$
$$
= \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes ux_i \otimes x_{i+1} \otimes \cdots \otimes x_n \otimes y_1 \otimes \cdots \otimes y_p
$$
$$
+ \sum_{j=1}^p x_1 \otimes \cdots \otimes x_n \otimes y_1 \otimes \cdots \otimes y_{j-1} \otimes uy_j \otimes y_{j+1} \otimes \cdots \otimes y_n
$$
$$
= \nu(x_1 \otimes \cdots \otimes x_n) \otimes (y_1 \otimes \cdots \otimes y_p) + (x_1 \otimes \cdots \otimes x_n) \otimes \nu(y_1 \otimes \cdots \otimes y_p).
$$

Par linéarité, on en déduit bien que $\nu$ est une dérivation. L’unicité de $\nu$ est évidente. Enfin, il est clair que $u_n$ permuté aux opérateurs de symétrie dans $\bigotimes^n V$, d’où la dernière assertion.

#### Proposition 7 {#lie-i-s2-prop-7 .statement}

*Soient g une algèbre de Lie, U son algèbre enveloppante, $\sigma$ l’application canonique de g dans U, et D une dérivation de g.*

a) *Il existe une dérivation $D_U$ de U et une seule telle que $\sigma \circ D = D_U \circ \sigma$ (c’est-à-dire telle que $D_U$ prolonge D, quand on peut identifier g à un sous-module de U par $\sigma$).

b) $D_U$ laisse stables $U_n$ et l’ensemble $U^n$ des images dans U des tenseurs symétriques homogènes d’ordre n sur g.

c) $D_U$ commute à l’antiautomorphisme principal de U.

d) *Si D est la dérivation intérieure de g définie par un élément x de g, $D_U$ est la dérivation intérieure de U définie par $\sigma(x)$.

En effet, soit $D_T$ la dérivation de l’algèbre tensorielle T de g qui prolonge D (lemme 4). L’idéal bilatère J de T engendré par les $x \otimes y - y \otimes x - [x, y]$ ($x, y$ dans g) est stable pour $D_T$. En effet :

$$
D_T(x \otimes y - y \otimes x - [x, y]) = Dx \otimes y - y \otimes Dx - [Dx, y]
$$
$$
+ x \otimes Dy - Dy \otimes x - [x, Dy].
$$

Par passage aux quotients, $D_T$ définit une dérivation $D_U$ de $U$, telle que $\sigma \circ D = D_U \circ \sigma$. L’unicité de $D_U$ est immédiate, puisque 1 et $\sigma(g)$ engendrent l’algèbre $U$. L’assertion b) est évidente. Soit $A$ l’antiautomorphisme principal de $U$, et prouvons c). Si $x_1, \ldots, x_n$ sont dans $g$, on a

$$
D_U A(\sigma(x_1) \ldots \sigma(x_n)) = D_U((-1)^n \sigma(x_n) \ldots \sigma(x_1))
$$
$$
= (-1)^n \sum_{i=1}^n \sigma(x_n) \ldots D_U(\sigma(x_i)) \ldots \sigma(x_1)
$$
$$
= (-1)^n \sum_{i=1}^n \sigma(x_n) \ldots \sigma(Dx_i) \ldots \sigma(x_1)
$$
$$
= A(\sum_{i=1}^n \sigma(x_1) \ldots \sigma(Dx_i) \ldots \sigma(x_n))
$$
$$
= AD_U(\sigma(x_1) \ldots \sigma(x_n)).
$$

Enfin, soit $x \in g$. Soit $\Delta$ la dérivation intérieure $y \mapsto \sigma(x)y - y\sigma(x)$ de $U$ (Alg., chap. IV, § 4, no 3, exemple 2). On a, pour $x' \in g$,
$$
(\Delta \circ \sigma)(x') = \sigma(x)\sigma(x') - \sigma(x')\sigma(x) = \sigma([x, x']) = (\sigma \circ \mathrm{ad}\ x)(x'), \text{ d'où } \Delta \circ \sigma = \sigma \circ \mathrm{ad}\ x. $$
Ceci achève la démonstration.

Appliquant la prop. 7 au cas d’une algèbre de Lie commutative, on voit que tout endomorphisme $u$ d’un $K$-module se prolonge de manière unique en une dérivation de l’algèbre symétrique de ce module ; cette dérivation se déduit par passage aux quotients de la dérivation de l’algèbre tensorielle qui prolonge $u$.

Reprénons une algèbre de Lie $g$ sur $K$, et soit $D$ une dérivation de $g$. Utilisons les notations $T, S, U, G$ antérieures. Soient $D_T, D_S$ les dérivations de $T, S$ qui prolongent $D$, et soit $D_U$ la dérivation unique de $U$ telle que $\sigma \circ D = D_U \circ \sigma$. Puisque $D_U$ laisse stables les $U_n$, $D_U$ définit par passage aux quotients une dérivation $D_G$ de $G$. Puisque $D_U$ et $D_S$ se déduisent de $D_T$ par passage aux quotients, le diagramme commutatif (3) prouve que $D_G$ peut aussi se déduire de $D_S$ par l’homomorphisme $\omega$ défini au no 6. Si en outre $K$ est un corps de caractéristique 0, les isomorphismes du diagramme (4) transforment entre elles les restrictions de $D_T, D_S, D_U, D_G$ à $S^n, S^n, U^n, G^n$. Donc l’isomorphisme canonique de $S$ sur $U$ transforme $D_S$ en $D_U$.

### 9. Extension de l’anneau de base

Soient g une algèbre de Lie sur K, T son algèbre tensorielle, J l’idéal bilatère de T engendré par les $x \otimes y - y \otimes x - [x, y]$ ($x, y$ dans g), et U = T/J. Soit $K_1$ un anneau commutatif à élément unité, et soit $\sigma$ un homomorphisme de K dans $K_1$ transformant 1 en 1. Alors, l’algèbre tensorielle de $g_{(K_1)}$ s’identifie canoniquement à $T_{(K_1)}$. Soit $J'$ l’idéal bilatère de $T_{(K_1)}$ engendré par les $x' \otimes y' - y' \otimes x' - [x', y']$ ($x', y'$ dans $g_{(K_1)}$). Il est clair que l’image canonique de $J_{(K_1)}$ dans $T_{(K_1)}$ est contenue dans $J'$. Pour voir qu’elle est égale à $J'$, il suffit de montrer que, si $x'$ et $y'$ désignent deux éléments de $g_{(K_1)}$, $x' \otimes y' - y' \otimes x' - [x', y']$ appartient à cette image. Or $x' = \sum_i x_i \otimes \lambda_i, y' = \sum_j y_j \otimes \mu_j$ ($x_i, y_j$ dans g, $\lambda_i, \mu_j$ dans $K_1$); d’où $x' \otimes y' - y' \otimes x' - [x', y'] = \sum_{i,j} (x_i \otimes y_j - y_j \otimes x_i - [x_i, y_j]) \otimes \lambda_i \mu_j$, ce qui prouve notre assertion. Ceci posé, on voit que $U_{(K_1)} = (T/J)_{(K_1)}$ s’identifie canoniquement à $T_{(K_1)}/J' : l’algèbre enveloppante de g_{(K_1)}$ s’identifie canoniquement à $U_{(K_1)}$, et l’application canonique de $g_{(K_1)}$ dans son algèbre enveloppante s’identifie à $\sigma \otimes 1$ (en désignant par $\sigma$ l’application canonique de g dans U).

## EXERCICES {#lie-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
