---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 5
section_title: Extension de l'anneau des scalaires
lang: fr
source: alg-i-iii-fr
book_pages: A II.191
pdf_pages: 0258-0265, 0368-0368
extraction: ocr
subsections:
    - "no": 1
      title: Extension de l’anneau des scalaires d’un module
      page: 0
      pdf_page: 258
    - "no": 2
      title: Relations entre restriction et extension de l’anneau des scalaires
      page: 85
      pdf_page: 262
    - "no": 3
      title: Extension de l’anneau d’opérateurs d’un module d’homomorphismes
      page: 86
      pdf_page: 263
    - "no": 4
      title: Dual d’un module obtenu par extension des scalaires
      page: 0
      pdf_page: 264
    - "no": 5
      title: Un critère de finitude
      page: 88
      pdf_page: 265
statements: 15
exercises: 7
content_sha256: 5afb5d1e0795a8a611f1168349701804055a8be5b265bde56e85b3cdb44780eb
---

## § 5. EXTENSION DE L’ANNEAU DES SCALAIRE S

### 1. Extension de l’anneau des scalaires d’un module

Soient $A, B$ deux anneaux, $\rho : A \to B$ un homomorphisme d’anneaux; considérons le *A-module à droite* $\rho_* (B_d)$ défini par cet homomorphisme (II, p. 30); ce A-module est aussi muni d’une structure de *B-module à gauche*, à savoir celle de $B_s$, et comme $b' (b \rho(a)) = (b'b) \rho(a)$ pour $a \in A,\ b,\ b'$ dans $B$, ces deux structures de module sur $B$ sont *compatibles* (II, p. 33). Cela permet, pour tout *A-module à gauche* $E$, de définir sur le produit tensoriel $\rho_* (B_d) \otimes_A E$ une structure de *B-module à gauche*, telle que $\beta' (\beta \otimes x) = (\beta'\beta) \otimes x$ pour $\beta,\ \beta'$ dans $B$ et $x \in E$

(II, p. 54). On dit que ce B-module à gauche est déduit de E par extension à B de l’anneau des scalaires au moyen de ρ, et on le note ρ*(E), ou E(B) si cela n’entraîne pas confusion.

#### Proposition 1 {#alg-ii-s5-prop-1 .statement}

Pour tout A-module à gauche E, l’application φ : x ↦ 1 ⊗ x de E dans le A-module ρ*(ρ*(E)) est A-linéaire, et l’ensemble φ(E) engendre le B-module ρ*(E). En outre, pour tout B-module à gauche F, et toute application A-linéaire f de E dans le A-module ρ*(F), il existe une application B-linéaire ĝ et une seule de ρ*(E) dans F telle que ĝ(1 ⊗ x) = f(x) pour tout x ∈ E.

En effet, B peut être considéré comme un (B, A)-bimodule au moyen de ρ; on a donc un isomorphisme canonique de Z-modules

(1)
$$
\operatorname{Hom}_B(B \otimes_A E, F) \to \operatorname{Hom}_A(E, \operatorname{Hom}_B(B_s, F))
$$
comme on l’a vu dans II, p. 74, prop. 1. Mais le A-module à gauche Hom_B(B_s, F) s’identifie canoniquement à ρ*(F): en effet, par définition (II, p. 35), à un élément y ∈ F correspond l’homomorphisme θ(y) : B_s → F tel que (θ(y))(1) = y; pour tout λ ∈ A, il correspond donc à ρ(λ)y ∈ F l’homomorphisme μ ↦ μρ(λ)y de B_s dans F, qui n’est autre que λθ(y) pour la structure de A-module à gauche de Hom_B(B_s, F) (II, p. 35). Compte tenu de cette identification, on a donc un isomorphisme canonique de Z-modules, réciproque de (1)

(2)
$$
δ : \operatorname{Hom}_A(E, ρ_*(F)) \to \operatorname{Hom}_B(ρ^*(E), F)
$$
et il résulte aussitôt des définitions que si δ(f) = ĝ, on a ĝ(1 ⊗ x) = f(x) pour tout x ∈ E. En particulier, l’application φ_E : x ↦ 1 ⊗ x n’est autre que

(3)
$$
φ_E = δ^{-1}(1_{ρ^*(E)}).
$$

La prop. 1 est donc démontrée. L’application φ_E : E → ρ_*(ρ^*(E)) est dite canonique.

#### Remarque 1 {#alg-ii-s5-n1-rem-1 .statement}

La prop. 1 montre que le couple formé de E(B) et de φ_E est solution du problème d’application universelle (E, IV, p. 23), où Σ est l’espèce de structure de B-module à gauche (les morphismes étant les applications B-linéaires) et les α-applications les applications A-linéaires de E dans un B-module.

#### Remarque 2 {#alg-ii-s5-n1-rem-2 .statement}

Si E est un (A, (C'_i); (D'_j))-multimodule, F un (B, (C''_h); (D''_k))-multimodule, alors l’isomorphisme (2) est linéaire pour les structures de ((D'_j), (C''_h); (C'_i), (D''_k))-multimodules des deux membres (II, p. 34 et p. 54).

#### Remarque 3 {#alg-ii-s5-n1-rem-3 .statement}

Soient E un A-module à gauche, a un idéal bilatère de A, ρ : A → A/a l’homomorphisme canonique. Avec les notations de II, p. 60, cor. 2, le A-module E/aE est annulé par a, et est donc canoniquement muni d’une structure de (A/a)-module à gauche (II, p. 28); il est immédiat que l’application canonique π : ρ^*(E) → E/aE définie dans II, p. 60, cor. 2, est un isomorphisme pour les structures de (A/a)-module.

#### Corollaire {#alg-ii-s5-n1-cor-1 .statement}

Soient E, E’ deux A-modules à gauche; pour toute application A-linéaire u : E → E’, v = 1_B ⊗ u est l’unique application B-linéaire rendant commutatif le diagramme

$$
\begin{array}{ccc}
E & \xrightarrow{\varphi_E} & E_{(B)} \\
u \downarrow & & v \downarrow \\
E' & \longrightarrow & E'_{(B)} \\
& \xrightarrow{\varphi_{E'}} &
\end{array}
$$

où $\varphi_E$ et $\varphi_{E'}$ sont les applications canoniques.

Il suffit en effet d’appliquer la prop. 1 au A-homomorphisme $\varphi_{E'} \circ u : E \to E'_{(B)}$.

L’application $v$ définie dans le corollaire précédent se note $\rho^*(u)$ ou $u_{(B)}$.

Si $E''$ est un troisième A-module à gauche, $v : E' \to E''$ une application A-linéaire, il est immédiat que l’on a

$$(v \circ u)_{(B)} = v_{(B)} \circ u_{(B)}.$$

L’extension de l’anneau d’opérateurs d’un module est une opération transitive ; de façon précise :

#### Proposition 2 {#alg-ii-s5-prop-2 .statement}

*Soient $\rho : A \to B, \sigma : B \to C$ des homomorphismes d’anneaux. Pour tout A-module à gauche E, il existe un C-homomorphisme et un seul*

$$(4)$$
$$\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)$$

*transformant $1 \otimes (1 \otimes x)$ en $1 \otimes x$ pour tout $x \in E$, et cet homomorphisme est bijectif.*

En effet, les $\mathbf{Z}$-modules sous-jacents à $\sigma^*(\rho^*(E))$ et à $(\sigma \circ \rho)^*(E)$ sont respectivement $C \otimes_B (B \otimes_A E)$ et $C \otimes_A E$. Il existe un $\mathbf{Z}$-isomorphisme canonique $C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E$ (II, p. 64, prop. 8), qui est aussi un C-isomorphisme pour les structures de C-module à gauche de deux membres. En outre, le C-module $C \otimes_B B$ s’identifie canoniquement au C-module $C_s$ par l’isomorphisme qui à $\gamma \otimes \beta$ fait correspondre $\gamma \sigma(\beta)$ (II, p. 55, prop. 4), et cet isomorphisme est aussi un isomorphisme pour la structure de A-module à droite sur $C \otimes_B B$ définie par $\rho$ et la structure de A-module à droite sur C définie par $\sigma \circ \rho$. On obtient donc bien un isomorphisme canonique

$$(C \otimes_B B) \otimes_A E \to C \otimes_A E,$$

et en le composant avec l’isomorphisme $C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E$ défini plus haut, on obtient l’isomorphisme canonique cherché.

Si $\varphi, \varphi', \varphi''$ désignent les applications canoniques $E \to \rho^*(E), \rho^*(E) \to \sigma^*(\rho^*(E))$ et $E \to (\sigma \circ \rho)^*(E)$, $\varphi' \circ \varphi$ s’identifie à $\varphi''$ par l’isomorphisme canonique de la prop. 2.

#### Proposition 3 {#alg-ii-s5-prop-3 .statement}

*Soient A, B deux anneaux commutatifs, $\rho : A \to B$ un homomorphisme d’anneaux, E, $E'$ deux A-modules. Il existe un B-homomorphisme et un seul*

$$(5)$$
$$E_{(B)} \otimes_B E'_{(B)} \to (E \otimes_A E')_{(B)}$$

*transformant $(1 \otimes x) \otimes (1 \otimes x')$ en $1 \otimes (x \otimes x')$ pour $x \in E, x' \in E'$, et cet homomorphisme est bijectif.*

En effet, le premier membre de (5) s’écrit $(B \otimes_A E) \otimes_B (B \otimes_A E')$ et s’identifie à $(E \otimes_A B) \otimes_B (B \otimes_A E')$ puisque A et B sont commutatifs ; ce dernier produit s’identifie successivement à $E \otimes_A (B \otimes_B B) \otimes_A E'$, à $E \otimes_A (B \otimes_A E')$, à $E \otimes_A (E' \otimes_A B)$ et finalement à $(E \otimes_A E') \otimes_A B$, par utilisation de l’associativité du produit tensoriel (II, p. 64, prop. 8), de la prop. 4 de II, p. 55, et de la commutativité de A et B. L’isomorphisme cherché est le composé de ces isomorphismes canoniques successifs.

Il est clair que si S est un système générateur de E, l’image de S par l’application canonique $E \to E_{(B)}$ est un système générateur de $E_{(B)}$; en particulier, si E est un A-module de type fini, $E_{(B)}$ est un B-module de type fini.

#### Proposition 4 {#alg-ii-s5-prop-4 .statement}

*Soit E un A-module admettant une base $(a_\lambda)_{\lambda \in L}$; si $\varphi : x \mapsto 1 \otimes x$ est l’application canonique de E dans $\rho^*(E)$, alors $(\varphi(a_\lambda))_{\lambda \in L}$ est une base de $\rho^*(E)$. Si $\rho$ est injectif, il en est de même de $\varphi$.*

La première assertion résulte aussitôt de II, p. 62, cor. 1. En outre, on a, pour toute famille $(\xi_\lambda)_{\lambda \in L}$ d’éléments de A, de support fini, $\varphi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = \sum_{\lambda \in L} \rho(\xi_\lambda) \varphi(a_\lambda)$, et la relation $\varphi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = 0$ équivaut donc à $\rho(\xi_\lambda) = 0$ pour tout $\lambda \in L$, d’où la seconde assertion.

#### Corollaire {#alg-ii-s5-n1-cor-2 .statement}

*Pour tout A-module projectif E, le B-module $\rho^*(E)$ est projectif. Si en outre $\rho$ est injectif, l’application canonique de E dans $\rho^*(E)$ est injective.*

En effet, il existe par hypothèse un A-module libre M contenant E et dans lequel E admet un supplémentaire F. Il résulte aussitôt de II, p. 61, prop. 7 que $M_{(B)}$ s’identifie à la somme directe de $E_{(B)}$ et $F_{(B)}$, et si $\varphi$ et $\psi$ sont les applications canoniques $E \to E_{(B)}$ et $F \to F_{(B)}$, l’application canonique $M \to M_{(B)}$ n’est autre que $x + y \mapsto \varphi(x) + \psi(y)$. Le corollaire résulte aussitôt de la prop. 4 appliquée au A-module M.

Lorsque E est un A-module *à droite*, on pose de même $\rho^*(E) = E \otimes_A \rho_*(B_s)$, B étant cette fois considéré comme (A, B)-bimodule, et la structure de B-module à droite de $\rho^*(E)$ étant telle que $(x \otimes \beta)\beta' = x \otimes (\beta\beta')$ pour $\beta \in B$, $\beta' \in B$ et $x \in E$. Nous laissons au lecteur le soin d’énoncer pour les modules à droite les résultats correspondant à ceux de ce n° et du suivant.

*Remarque 4).* — Considérons le A-module *à gauche* $\rho_*(B_s)$ défini par $\rho$, et pour tout A-module à gauche E, considérons le $\mathbf{Z}$-module
$$
\tilde{\rho}(E) = \operatorname{Hom}_A(\rho_*(B_s), E).
$$
Comme $\rho_*(B_s)$ est muni d’une structure de B-*module à droite*, on en déduit sur $\tilde{\rho}(E)$ une structure de B-*module à gauche* (II, p. 35) telle que si $u \in \tilde{\rho}(E)$ et $b' \in B$, $b'u$ est l’homomorphisme $b \mapsto u(bb')$ de $\rho_*(B_s)$ dans E. On définit en outre une application *A-linéaire*, dite *canonique*:
$$
\eta : \rho_*(\tilde{\rho}(E)) \to E
$$
en faisant correspondre à tout homomorphisme $u \in \tilde{\rho}(E)$ l’élément $u(1)$ dans E. Comme B peut être considéré comme un (A, B)-bimodule au moyen de $\rho$, on a, pour tout B-module à gauche F, un isomorphisme canonique de $\mathbf{Z}$-modules
$$
\operatorname{Hom}_A(\rho_*(B_s) \otimes_B F, E) \to \operatorname{Hom}_B(F, \operatorname{Hom}_A(\rho_*(B_s), E))
$$

(II, p. 74, prop. 1). Comme le A-module à gauche $\rho_*(B_s) \otimes_B F$ s’identifie canoniquement à $\rho_*(F)$ en vertu de II, p. 55, prop. 4, on obtient donc un isomorphisme canonique de $\mathbf{Z}$-modules, réciproque du précédent
$$
\text{Hom}_B(F, \tilde{\rho}(E)) \to \text{Hom}_A(\rho_*(F), E)
$$
qui, à toute application B-linéaire $g$ de $F$ dans $\tilde{\rho}(E)$, fait correspondre l’application composée $\eta \circ g$, considérée comme application A-linéaire de $\rho_*(F)$ dans $E$. En particulier, sous les hypothèses de la prop. 2 (II, p. 83), si on remplace $F$ par $\sigma_*(C_s)$, on obtient un C-isomorphisme canonique
$$
\tilde{\sigma}(\tilde{\rho}(E)) \to (\sigma \circ \rho)^*(E).
$$

### 2. Relations entre restriction et extension de l’anneau des scalaires

Soit $\rho : A \to B$ un homomorphisme d’anneaux. Pour tout A-module à gauche $E$, nous avons défini au n° 1 une application A-linéaire canonique
$$
\varphi_E : E \to \rho_*(\rho^*(E))
$$
telle que $\varphi_E(x) = 1 \otimes x$. Considérons maintenant un B-module à gauche $F$, et appliquons la prop. 1 (II, p. 82) au A-homomorphisme $1_{\rho_*(F)} : \rho_*(F) \to \rho_*(F)$; on en déduit une application B-linéaire
$$
\psi_F : \rho^*(\rho_*(F)) \to F
$$
égale à $\delta(1_{\rho_*(F)})$, et telle par suite que pour tout $y \in F$ et tout $\beta \in B$, on ait $\psi_F(\beta \otimes y) = \beta y$.

#### Proposition 5 {#alg-ii-s5-prop-5 .statement}

*Soient E un A-module à gauche, F un B-module à gauche; les applications composées*
$$
\begin{array}{cccc}
\rho^*(E) & \xrightarrow{\rho^*(\varphi_E)} & \rho^*(\rho_*(\rho^*(E))) \\
& & \xrightarrow{\psi_{\rho^*(E)}} & \rho^*(E)
\end{array}
$$
$$
\begin{array}{cccc}
\rho_*(F) & \xrightarrow{\varphi_{\rho_*(F)}} & \rho_*(\rho^*(\rho_*(F))) \\
& & \xrightarrow{\rho_*(\psi_F)} & \rho_*(F)
\end{array}
$$
*sont respectivement égales aux applications identiques de $\rho^*(E)$ et de $\rho_*(F)$*.

Montrons-le par exemple pour (12); pour tout $x \in E$, l’application $\rho^*(\varphi_E)$ fait correspondre à $1 \otimes x$ l’élément $1 \otimes (1 \otimes x)$ et l’application $\psi_{\rho^*(E)}$ fait correspondre à $1 \otimes (1 \otimes x)$ l’élément $1 \otimes x$; la conclusion résulte de ce que les éléments de la forme $1 \otimes x$ engendrent le B-module $\rho^*(E)$; la démonstration est encore plus simple pour (13).

#### Corollaire {#alg-ii-s5-n2-cor-1 .statement}

*Les applications $\rho^*(\varphi_E)$ et $\varphi_{\rho^*(F)}$ sont injectives et identifient respectivement $\rho^*(E)$ à un facteur direct de $\rho^*(\rho_*(\rho^*(E)))$ et $\rho_*(F)$ à un facteur direct de $\rho_*(\rho^*(\rho_*(F)))$*.

C’est une conséquence de la prop. 5 et de II, p. 21, cor. 2.

#### Proposition 6 {#alg-ii-s5-prop-6 .statement}

*Soient E un A-module à gauche, F un B-module à droite. Il existe un $\mathbf{Z}$-homomorphisme et un seul*
$$
\rho_*(F) \otimes_A E \to F \otimes_B \rho^*(E)
$$

transformant $y \otimes x$ en $y \otimes (1 \otimes x)$ pour tout $x \in E$ et tout $y \in F$, et cet homomorphisme est bijectif.

En effet, par définition le second membre de (14) est $F \otimes_B (B \otimes_A E)$, où B est considéré comme $(B, A)$-bimodule, et on a un $\mathbf{Z}$-isomorphisme canonique $(F \otimes_B B) \otimes_A E \to F \otimes_B (B \otimes_A E)$ défini dans II, p. 64, prop. 8; d’autre part, l’isomorphisme canonique $F \to F \otimes_B B$ de II, p. 55, prop. 4 est un isomorphisme pour les structures de A-module à droite des deux membres, définies par $\rho$. D’où l’isomorphisme cherché.

Lorsque A et B sont *commutatifs*, l’isomorphisme (14) est un isomorphisme de *A-modules*
$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E)).
$$

### 3. Extension de l’anneau d’opérateurs d’un module d’homomorphismes

Soient A un anneau *commutatif*, B un anneau, $\rho : A \to B$ un homomorphisme d’anneaux, E, F deux A-modules; comme B est un $(A, A)$-bimodule (au moyen de $\rho$) et que F peut être considéré comme un $(A, A)$-bimodule, on a, sur le $\mathbf{Z}$-module $B \otimes_A F$, *deux* structures de A-module, pour lesquelles on a respectivement $a(b \otimes y) = (\rho(a)b) \otimes y$ et $a(b \otimes y) = b \otimes (ay)$ pour $a \in A,\ b \in B,\ y \in F$. Nous désignerons par $G'$ et $G''$ les deux A-modules ainsi définis; $G'$ n’est autre d’ailleurs que le A-module $\rho_*(\rho^*(F))$.

Cela étant, dans la définition de l’homomorphisme canonique de II, p. 75, formule (7), remplaçons B par A, le B-module F par l’anneau B considéré comme A-module au moyen de $\rho$, et G par F considéré comme $(A, A)$-bimodule; comme A est commutatif, on peut écrire le *$\mathbf{Z}$*-homomorphisme *canonique* obtenu
$$
B \otimes_A \mathrm{Hom}_A(E, F) \to \mathrm{Hom}_A(E, G'').
$$
D’autre part (II, p. 82, formule (2)), on a un *$\mathbf{Z}$*-*isomorphisme canonique*
$$
\mathrm{Hom}_A(E, G') = \mathrm{Hom}_A(E, \rho_*(\rho^*(F))) \to \mathrm{Hom}_B(\rho^*(E), \rho^*(F)).
$$
Supposons maintenant que $\rho(A)$ soit contenu dans le *centre* de B, auquel cas on dit encore que $\rho$ est un homomorphisme *central* *(ou que $\rho$ définit sur B une structure de A-*algèbre*, cf. III, p. 6)*. Alors les structures de A-module de $G'$ et $G''$ sont *identiques*, et en composant les homomorphismes (16) et (15), on obtient donc un *$\mathbf{Z}$*-homomorphisme canonique
$$
\omega : B \otimes_A \mathrm{Hom}_A(E, F) \to \mathrm{Hom}_B(E_{(B)}, F_{(B)})
$$
qui est caractérisé par le fait que pour tout $u \in \mathrm{Hom}_A(E, F)$ et tout $b \in B$, on a
$$
\omega(b \otimes u) = r_b \otimes u
$$
en désignant par $r_b$ la multiplication à droite par $b$ dans B.

En outre, l’hypothèse que $\rho$ est un homomorphisme *central* entraîne que l’on a $(bb')\rho(a) = (b\rho(a))b'$ pour $b,\ b'$ dans B et $a \in A$; autrement dit la structure de

B-module à droite de $B_d$ est compatible avec sa structure de A-module; elle définit donc sur $B \otimes_A \mathrm{Hom}_A(E, F)$ une structure de B-module à droite (II, p. 54) ainsi que sur $F_{(B)} = B \otimes_A F$, et finalement, comme les structures de B-module à gauche et à droite sur $F_{(B)}$ sont compatibles, on obtient aussi sur $\mathrm{Hom}_B(E_{(B)}, F_{(B)})$ une structure de B-module à droite (II, p. 35). On vérifie alors aussitôt que (17) est un homomorphisme de B-modules à droite pour ces structures.

#### Proposition 7 {#alg-ii-s5-prop-7 .statement}

Soient A un anneau commutatif, B un anneau, $\rho : A \to B$ un homomorphisme central, E, F deux A-modules.
(i) Si B est un A-module projectif (resp. projectif de type fini), l’homomorphisme (17) est injectif (resp. bijectif).
(ii) Si E est un A-module projectif de type fini, l’homomorphisme (17) est bijectif.
Comme (16) est bijectif, la proposition résulte de II, p. 75, prop. 2, appliquée à l’homomorphisme canonique (15).

### 4. Dual d’un module obtenu par extension des scalaires

Soient A, B deux anneaux, $\rho : A \to B$ un homomorphisme d’anneaux, E un A-module à gauche, E* son dual. Nous allons définir une application B-linéaire canonique

$$
v_E : (E^*)_{(B)} \to (E_{(B)})^*.
$$

En effet, le premier membre de (19) s’écrit $\mathrm{Hom}_A(E, A) \otimes_A \rho_*(B_s)$, où dans $\mathrm{Hom}_A(E, A)$, A est considéré comme (A, A)-bimodule. On a donc un $\mathbf{Z}$-homomorphisme canonique (II, p. 75, formule (7))

$$
\nu : \mathrm{Hom}_A(E, A) \otimes_A \rho_*(B_s) \to \mathrm{Hom}_A(E, A \otimes_A \rho_*(B_s)) = \mathrm{Hom}_A(E, \rho_*(B_s))
$$

avec l’identification fournie par l’isomorphisme canonique de II, p. 55, prop. 4. D’autre part, le second membre de (19) s’écrit $\mathrm{Hom}_B(\rho_*(B_d) \otimes_A E, B_s)$; comme B est un (B, A)-bimodule, on a un $\mathbf{Z}$-isomorphisme canonique (II, p. 74, prop. 1)

$$
\beta : \mathrm{Hom}_B(\rho_*(B_d) \otimes_A E, B_s) \to \mathrm{Hom}_A(E, \mathrm{Hom}_B(B_s, B_s))
$$

et $\mathrm{Hom}_B(B_s, B_s)$ s’identifie canoniquement, en tant que A-module, à $\rho_*(B_s)$ (voir la démonstration de II, p. 82, prop. 1). Tenant compte de ces identifications, on obtient l’homomorphisme $v_E$; on vérifie aisément que cet homomorphisme est caractérisé par l’équation

$$
\langle \xi \otimes x, v_E(x^* \otimes \eta) \rangle = \xi \rho(\langle x, x^* \rangle) \eta,
$$

pour $x \in E, x^* \in E^*, \xi, \eta$ dans B, ce qui montre aussitôt que $v_E$ est B-linéaire.

En outre, pour toute application A-linéaire $u : E \to F$, le diagramme

$$
\begin{array}{ccc}
(F^*)_{(B)} & \xrightarrow{u_F} & (F_{(B)})^* \\
(tu)_{(B)} \downarrow & & \downarrow t(u_{(B)}) \\
(E^*)_{(B)} & \xrightarrow{v_E} & (E_{(B)})^*
\end{array}
$$

est commutatif.

#### Proposition 8 {#alg-ii-s5-prop-8 .statement}

*Si l’un des A-modules* $E$, $\rho_*(B_s)$ *est projectif de type fini, l’homomorphisme* $v_E$ *est bijectif*.
Cela résulte de ce qui précède et de II, p. 75, prop. 2.

Supposons en particulier que $E$ soit un A-module *libre de type fini* et soient $(e_i)_{1 \leq i \leq n}$ une base de $E$, $(e_i^*)_{1 \leq i \leq n}$ la base duale; alors l’isomorphisme canonique (19) de II, p. 87 fait correspondre à la base $(e_i^* \otimes 1)$ de $(E^*)_{(B)}$ la base duale de la base $(1 \otimes e_i)$ de $E_{(B)}$.

### 5. Un critère de finitude

#### Proposition 9 {#alg-ii-s5-prop-9 .statement}

*Soient B un anneau, A un sous-anneau de B, P un A-module à gauche projectif. Alors, si* $P_{(B)}$ *est un B-module de type fini, P est lui-même un A-module de type fini*.

On sait (II, p. 46, prop. 12) qu’il existe une famille $(a_\lambda)_{\lambda \in L}$ d’éléments de $P$ et une famille $(a_\lambda^*)_{\lambda \in L}$ d’éléments du dual $P^*$ telles que, pour tout $x \in P$, la famille $(\langle x, a_\lambda^* \rangle)$ soit de support fini et que l’on ait $x = \sum_\lambda \langle x, a_\lambda^* \rangle a_\lambda$. Puisque $P_{(B)}$ est de type fini, il existe une famille finie $(y_i)_{i \in I}$ d’éléments de $P$ telle que $P_{(B)}$ soit engendré par les éléments $1 \otimes y_i$. Pour chaque indice $i$, la famille $(\langle y_i, a_\lambda^* \rangle)$ a un support fini. Il existe donc une partie finie $H$ de $L$ telle que $\langle y_i, a_\lambda^* \rangle = 0$ pour $i \in I$ et $\lambda \notin H$. Puisque $\langle 1 \otimes y_i, \mathrm{Id}_B \otimes a_\lambda^* \rangle = \langle y_i, a_\lambda^* \rangle$, il en résulte que $\mathrm{Id}_B \otimes a_\lambda^* = 0$ pour $\lambda \notin H$. Quel que soit $x \in P$, on a donc $\langle x, a_\lambda^* \rangle = \langle 1 \otimes x, \mathrm{Id}_B \otimes a_\lambda^* \rangle = 0$ pour $\lambda \notin H$. Ceci montre que le A-module $P$ est engendré par les $a_\lambda$ tels que $\lambda \in H$.

## EXERCICES {#alg-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
