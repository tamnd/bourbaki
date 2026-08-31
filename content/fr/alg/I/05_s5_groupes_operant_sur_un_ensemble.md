---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 5
section_title: Groupes opérant sur un ensemble
lang: fr
source: alg-i-iii-fr
book_pages: A I.49-A I.62, A I.129-A I.134
pdf_pages: 0059-0072, 0139-0144
extraction: ocr
subsections:
    - "no": 1
      title: Monoïde opérant sur un ensemble
      page: 49
      pdf_page: 59
    - "no": 2
      title: Stabilisateur, fixateur
      page: 51
      pdf_page: 61
    - "no": 3
      title: Automorphismes intérieurs
      page: 53
      pdf_page: 63
    - "no": 4
      title: Orbites
      page: 54
      pdf_page: 64
    - "no": 5
      title: Ensembles homogènes
      page: 56
      pdf_page: 66
    - "no": 6
      title: Ensembles principaux homogènes
      page: 58
      pdf_page: 68
    - "no": 7
      title: Groupe des permutations d’un ensemble fini
      page: 59
      pdf_page: 69
statements: 40
exercises: 29
content_sha256: 5406d1248da1a2881223a5d8c038d746c3be5a9f47a401375a0482461422333e
---

## § 5. GROUPES OPÉRANT SUR UN ENSEMBLE

### 1. Monoïde opérant sur un ensemble

#### Définition 1 {#alg-i-s5-def-1 .statement}

*Soient M un monoïde, de loi notée multiplicativement et d’élément neutre noté e, et E un ensemble. On dit qu’une action $\alpha \mapsto f_\alpha$ de M sur E est une opération à gauche (resp. à droite) de M sur E si l’on a $f_e = \mathrm{Id}_E$ et $f_{\alpha \beta} = f_\alpha \circ f_\beta$ (resp. $f_{\alpha \beta} = f_\beta \circ f_\alpha$) quels que soient $\alpha, \beta$ dans M.*

En d’autres termes, une opération à gauche (resp. à droite) d’un monoïde M sur un ensemble E est un *homomorphisme de monoïdes* de M dans le monoïde $E^E$ (resp. le monoïde opposé à $E^E$) muni de la composition des applications. Si l’on note multiplicativement à gauche (resp. à droite) l’une des lois d’action correspondant à l’action de M, le fait que cette action soit une opération à gauche (resp. à droite) se traduit par les formules

(1)
$$
e.x = x ; \alpha . (\beta . x) = (\alpha \beta) . x \quad \text{pour } \alpha, \beta \text{ dans } M \text{ et } x \in E
$$
(resp. $x.e = x ; (x.\alpha) . \beta = x . (\alpha \beta)$ pour $\alpha, \beta$ dans $M$ et $x \in E$).

Sous ces conditions, on dit encore que M *opère à gauche* (resp. *à droite*) sur E et que les lois d’action correspondantes sont des *lois d’opération à gauche* (resp. *à droite*) du monoïde M sur E.

Soit M un monoïde; un ensemble E muni d’une opération à gauche (resp. à droite) de M sur E est appelé un *M-ensemble* à gauche (resp. à droite). On dit que le monoïde M opère à gauche (resp. à droite) *fidèlement* si l’application $\alpha \mapsto f_\alpha$ de M dans $E^E$ est injective.

#### Exemple 1 {#alg-i-s5-n1-exa-1 .statement}

Soit E un ensemble; l’action canonique de $E^E$ sur E (I, p. 24, *Exemple 3*) est une opération à gauche.
2) Soit M un monoïde. L’action à gauche (resp. à droite) de M sur lui-même déduite de la loi de M (I, p. 24, *Exemple 7*) est une opération à gauche (resp. à droite) de M sur lui-même. Lorsqu’on considère cette opération, on dit que M opère sur lui-même *par translations à gauche* (resp. *à droite*).

Soient E un M-ensemble à gauche (resp. à droite) et $M^0$ le monoïde opposé à M. Pour la même action, le monoïde $M^0$ opère à droite (resp. à gauche) sur E. Le $M^0$-ensemble obtenu est dit *opposé* au M-ensemble E. Les définitions et résultats relatifs aux M-ensembles à gauche se transposent aux $M^0$-ensembles à droite par passage aux structures opposées.

Dans la suite de ce paragraphe, on ne considérera, sauf mention expresse du contraire, que des M-ensembles à gauche qu’on appellera simplement M-ensembles. Leur loi d’action sera notée multiplicativement à gauche.

Soit E un ensemble. Soit G un groupe opérant sur E. Pour tout $\alpha$ dans G, l’élément de $E^E$ défini par $\alpha$ est une permutation de E (I, p. 15, n° 3, *Exemple 2*). Se donner une opération de G sur E revient donc à se donner un homomorphisme de G dans $\mathfrak{S}_E$.

Conformément à I, p. 24, on pose la définition suivante:

#### Définition 2 {#alg-i-s5-def-2 .statement}

*Soient M un monoïde, E et E' des M-ensembles. On appelle homomorphisme de M-ensembles (ou M-morphisme, ou application compatible avec les opérations de M) une application f de E dans E' telle que, pour tout $x \in E$ et tout $\alpha \in M$, on ait $f(\alpha . x) = \alpha . f(x)$.*

L’application identique d’un M-ensemble est un M-morphisme. Le composé de deux M-morphismes en est un. Pour qu’une application d’un M-ensemble dans un autre soit un isomorphisme, il faut et il suffit que ce soit un M-morphisme bijectif et l’application réciproque est alors un M-morphisme.

Soit $(E_i)_{i \in I}$ une famille de $M$-ensembles, et soit $E$ l’ensemble produit des $E_i$. Le monoïde $M$ opère sur $E$ par $\alpha.(x_i)_{i \in I} = (\alpha.x_i)_{i \in I}$, et $E$, muni de cette action, est un $M$-ensemble; soit $E'$ un $M$-ensemble; une application $f$ de $E'$ dans $E$ est un $M$-morphisme si et seulement si $pr_i \circ f$ est un $M$-morphisme de $E'$ dans $E_i$ pour tout $i \in I$.

Soient $E$ un $M$-ensemble et $F$ une partie de $E$ stable pour l’action de $M$; muni de la loi induite, $F$ est un $M$-ensemble et l’injection canonique $F \to E$ est un $M$-morphisme.

Soient $E$ un $M$-ensemble et $R$ une relation d’équivalence sur $E$ compatible avec l’action de $M$; le quotient $E/R$ muni de l’action quotient est un $M$-ensemble et l’application canonique $E \to E/R$ est un $M$-morphisme.

Soient $\varphi : M \to M'$ un homomorphisme de monoïdes, $E$ un $M$-ensemble et $E'$ un $M'$-ensemble. On appelle $\varphi$-morphisme de $E$ dans $E'$ une application $f$ de $E$ dans $E'$ telle que, pour tout $x \in E$ et tout $\alpha \in M$, on ait $f(\alpha.x) = \varphi(\alpha).f(x)$ (cf. I, p. 25).

Extension d’une loi d’opération. — Etant donnés (par exemple) trois ensembles $F_1, F_2, F_3$, des permutations $f_1, f_2, f_3$ de $F_1, F_2, F_3$ respectivement, et un échelon $F$ sur les ensembles de base $F_1, F_2, F_3$ (E, IV, p. 2), on sait définir, en procédant de proche en proche sur la construction de l’échelon $F$, une permutation de $F$ appelée extension canonique de $f_1, f_2, f_3$ à $F$ (E, IV, p. 2); nous la noterons $\varphi_F(f_1, f_2, f_3)$.

Soient alors $G$ un groupe, $h_i$ un homomorphisme de $G$ dans le groupe symétrique de $F_i$ ($i = 1, 2, 3$), autrement dit une opération de $G$ dans $F_i$. L’application $x \mapsto x_F = \varphi_F(h_1(x), h_2(x), h_3(x))$ est un homomorphisme de $G$ dans $\mathfrak{S}_F$, autrement dit une opération de $G$ dans $F$, qu’on appelle l’extension de $h_1, h_2, h_3$ à $F$. Soit $P$ une partie de $F$ telle que, pour tout $x \in G$, on ait $x_F(P) = P$; soit $x_P$ la restriction de $x_F$ à $P$; alors l’application $x \mapsto x_P$ est une opération de $G$ dans $P$ qu’on appelle encore l’extension de $h_1, h_2, h_3$ à $P$.

Par exemple, soient $K$ et $L$ deux échelons sur $F_1, F_2, F_3$; prenons pour $F$ l’ensemble des parties de $K \times L$, et pour $P$ l’ensemble des applications de $K$ dans $L$, identifiées à leurs graphes. Si $\omega \in P$ et si $x \in G$, $x_P(\omega)$ est l’application $k \mapsto x_L(\omega(x_K^{-1}(k)))$ de $K$ dans $L$.

### 2. Stabilisateur, fixateur

#### Définition 3 {#alg-i-s5-def-3 .statement}

Soient $M$ un monoïde opérant sur un ensemble $E$, $A$ et $B$ des parties de $E$. On appelle transporteur (resp. transporteur strict) de $A$ dans $B$ l’ensemble des $\alpha \in M$ tels que $\alpha A \subset B$ (resp. $\alpha A = B$). Le transporteur (resp. transporteur strict) de $A$ dans $A$ est appelé le stabilisateur (resp. stabilisateur strict) de $A$. On appelle fixateur de $A$ l’ensemble des $\alpha \in M$ tels que $\alpha a = a$ pour tout $a \in A$.

On dit qu’un élément $\alpha$ de $M$ stabilise (resp. stabilise strictement, resp. fixe) une partie A de E si $\alpha$ appartient au stabilisateur (resp. au stabilisateur strict, resp. au fixateur) de A. On dit qu’une partie P de M stabilise (resp. stabilise strictement, resp. fixe) une partie A de E si tous les éléments de P stabilisent (resp. stabilisent strictement, resp. fixent) A. Le fixateur de A est contenu dans le stabilisateur strict de A qui est lui-même contenu dans le stabilisateur de A.

#### Proposition 1 {#alg-i-s5-prop-1 .statement}

*Soient M un monoïde opérant sur un ensemble E et A une partie de E.*
    a) *Le stabilisateur, le stabilisateur strict et le fixateur de A sont des sous-monoïdes de M.*
    b) *Soit $\alpha$ un élément inversible de M ; si $\alpha$ appartient au stabilisateur strict (resp. au fixateur) de A, il en est de même de $\alpha^{-1}$.*
    Soit e l’élément neutre de M ; on a $ea = a$ pour tout élément $a \in A$ et par suite e appartient au fixateur de A. Soient $\alpha$ et $\beta$ des éléments de E qui stabilisent A. On a $(\alpha\beta)A = \alpha(\beta A) \subset \alpha A \subset A$ et par suite le stabilisateur de A est un sous-monoïde de M. De même pour le stabilisateur strict et le fixateur de A, d’où a). Si $\alpha A = A$, on a $A = \alpha^{-1}(\alpha A) = \alpha^{-1}A$. Si pour tout $a \in A$, on a $\alpha a = a$, on a $a = \alpha^{-1}(\alpha a) = \alpha^{-1}a$, d’où b).

#### Corollaire {#alg-i-s5-n2-cor-1 .statement}

*Soient G un groupe opérant sur un ensemble E, et A une partie de E. Le stabilisateur strict S et le fixateur F de A sont des sous-groupes de G, et F est un sous-groupe distingué de S.*
    La première assertion découle de la prop. 1, et F est le noyau de l’homomorphisme de S dans $\mathfrak{S}_A$ associé à l’opération de S sur A.

Un groupe G opère fidèlement sur un ensemble E si et seulement si le fixateur de E est réduit à l’élément neutre de G. En effet, le fixateur de E est le noyau de l’homomorphisme donné de G dans $\mathfrak{S}_E$; cet homomorphisme est injectif si et seulement si son noyau est réduit à l’élément neutre (I, p. 36, th. 3).

Soient M un monoïde, E un M-ensemble, $a$ un élément de E. Le fixateur, le stabilisateur strict et le stabilisateur de $\{a\}$ sont égaux ; ce sous-monoïde est appelé indifféremment le fixateur ou le stabilisateur de $a$. Le fixateur d’une partie A de E est l’intersection des fixateurs des éléments de A. On dit que $a$ est un élément *invariant* de E si le fixateur de $a$ est le monoïde M. On dit que M opère *trivialement* sur E si tout élément de E est invariant.

#### Proposition 2 {#alg-i-s5-prop-2 .statement}

*Soit G un groupe opérant sur un ensemble E et, pour tout $x \in E$, soit $S_x$ le stabilisateur de x. Pour tout $\alpha \in G$, on a $S_{\alpha x} = \alpha S_x \alpha^{-1}$.*
    Si $s \in S_x$, on a $\alpha s \alpha^{-1}(\alpha x) = \alpha s x = \alpha x$, d’où $\alpha S_x \alpha^{-1} \subset S_{\alpha x}$. Comme $x = \alpha^{-1}(\alpha x)$, on a $\alpha^{-1} S_{\alpha x} \alpha \subset S_x$, d’où $S_{\alpha x} \subset \alpha S_x \alpha^{-1}$.

On voit de même que, si A et B sont deux parties de E et T le transporteur (resp. transporteur strict) de A dans B, alors le transporteur (resp. transporteur strict) de $\alpha A$ dans $\alpha B$ est égal à $\alpha T \alpha^{-1}$.

### 3. Automorphismes intérieurs

Soit G un groupe. L’ensemble Aut(G) des automorphismes du groupe G est un sous-groupe de $\mathfrak{S}_G$ (I, p. 29, Exemple 2)

#### Proposition 3 {#alg-i-s5-prop-3 .statement}

Soit G un groupe. Pour tout élément x de G, l’application Int(x): $y \mapsto xyx^{-1}$ de G dans lui-même est un automorphisme de G. L’application Int: $x \mapsto \operatorname{Int}(x)$ de G dans Aut(G) est un homomorphisme de groupes, dont le noyau est le centre de G et dont l’image Int(G) est un sous-groupe distingué de Aut(G).

Si x, y et z sont des éléments de G, on a $(xyx^{-1})(xzx^{-1}) = xyzx^{-1}$, donc Int(x) est un endomorphisme de G. Pour x et y éléments de G, on a $\operatorname{Int}(x) \circ \operatorname{Int}(y) = \operatorname{Int}(xy)$: en effet, pour tout $z \in G$, $x(yzy^{-1})x^{-1} = (xy)z(xy)^{-1}$. D’autre part, Int(e) est l’application identique de G. L’application Int est donc un homomorphisme de monoïde de G dans le monoïde End(G) des endomorphismes du groupe G. Comme les éléments de G sont inversibles, l’application Int prend ses valeurs dans l’ensemble Aut(G) des éléments inversibles de End(G) (I, p. 15). On a $xyx^{-1} = y$ si et seulement si x et y commutent, donc Int(x) est l’application identique de G si et seulement si x est un élément central. Enfin, soit $\alpha$ un automorphisme de G et soit $x \in G$; on a

$$
\operatorname{Int}(\alpha(x)) = \alpha \circ \operatorname{Int}(x) \circ \alpha^{-1}.
$$

En effet, pour $y \in G$, on a

$$
\alpha(x) \cdot y \cdot \alpha(x)^{-1} = \alpha(x) \cdot \alpha(\alpha^{-1}(y)) \cdot \alpha(x)^{-1} = \alpha(x \cdot \alpha^{-1}(y) \cdot x^{-1}).
$$

D’où $\alpha \cdot \operatorname{Int}(G) \cdot \alpha^{-1} \subset \operatorname{Int}(G)$.

#### Définition 4 {#alg-i-s5-def-4 .statement}

Soient G un groupe et $x \in G$. L’automorphisme $y \mapsto xyx^{-1}$ est appelé l’automorphisme intérieur de G défini par x, et est noté Int x.

Pour $x, y \in G$, on pose aussi $x^y = y^{-1}xy = (\operatorname{Int} y^{-1})(x)$.

Un sous-groupe de G est distingué si et seulement s’il est stable par tous les automorphismes intérieurs de G (I, p. 34, déf. 5). On dit qu’un sous-groupe de G est caractéristique s’il est stable par tous les automorphismes de G. Le centre d’un groupe G est un sous-groupe caractéristique (formule (2)).

Le centre d’un groupe G n’est pas nécessairement stable par tous les endomorphismes de G (I, p. 132, exerc. 22). En particulier, le centre d’un groupe à opérateurs n’est pas nécessairement un sous-groupe stable.

#### Proposition 4 {#alg-i-s5-prop-4 .statement}

Soient G un groupe, H un sous-groupe caractéristique (resp. distingué) de G, K un sous-groupe caractéristique de H. Alors K est un sous-groupe caractéristique (resp. distingué) de G.

En effet, la restriction à H d’un automorphisme (resp. d’un automorphisme intérieur) de G est un automorphisme de H et laisse donc stable K.

Soient G un groupe, A $\subset G$ et $b \in G$. On dit que b normalise A si $bAb^{-1} = A$; on dit que b centralise A si, pour tout $a \in A$, on a $bab^{-1} = a$. Soient A et B des parties de G; on dit que B normalise (resp. centralise) A si tout élément de B normalise (resp. centralise) A.

L’ensemble des $g \in G$ qui normalisent (resp. centralisent) A est appelé le normalisateur (resp. centralisateur, ou commutant) de A (cf. I, p. 7, déf. 9); on le note souvent $N_G(A)$ ou simplement $N(A)$ (resp. $C_G(A)$ ou $C(A)$). C’est un sous-groupe de G. Lorsque A est un sous-groupe de G, on peut caractériser $N_G(A)$ comme le plus grand sous-groupe de G qui contienne A et dans lequel A soit distingué.

#### Remarque 1 {#alg-i-s5-n3-rem-1 .statement}

Le normalisateur (resp. le centralisateur) de A est le stabilisateur strict (resp. le fixateur) de A lorsqu’on fait opérer G sur lui-même par automorphismes intérieurs. En particulier, le centralisateur est un sous-groupe distingué du normalisateur.

#### Remarque 2 {#alg-i-s5-n3-rem-2 .statement}

L’ensemble des éléments $b \in G$ tels que $bAb^{-1} \subset A$ est un sous-monoïde de G. Même lorsque A est un sous-groupe de G, cet ensemble n’est pas nécessairement un sous-groupe de G (I, p. 134, exerc. 27).

### 4. Orbites

#### Définition 5 {#alg-i-s5-def-5 .statement}

Soient G un groupe, E un G-ensemble, et $x \in E$. On dit qu’un élément $y \in E$ est conjugué à x par l’opération de G s’il existe un élément $\alpha \in G$ tel que $y = \alpha x$. L’ensemble des éléments conjugués à x est appelé l’orbite de x dans E.

La relation « y est conjugué à x » est une relation d’équivalence. En effet, $x = ex$; si $y = \alpha x$, on a $x = \alpha^{-1} y$; si $y = \alpha x$ et $z = \beta y$, on a $z = \beta \alpha x$. Les orbites sont les classes d’équivalence pour cette relation.

Une partie X de E est stable si et seulement si elle est saturée pour la relation de conjugaison.

L’application $\alpha \mapsto \alpha x$ de G dans E est parfois appelée l’application orbitale définie par x. C’est un G-morphisme de G (muni de l’opération de G sur lui-même par translations à gauche) dans E. L’image $G.x$ de G par cette application est l’orbite de x.

On dit que G opère librement sur E si pour tout $x \in E$, l’application orbitale définie par x est injective ou encore si l’application $(g, x) \mapsto (gx, x)$ de $G \times E$ dans $E \times E$ est injective.

#### Exemple 1 {#alg-i-s5-n4-exa-1 .statement}

Soit G un groupe, et considérons l’opération de G sur lui-même par automorphismes intérieurs. Deux éléments de G conjugués pour cette opération sont dits conjugués par automorphismes intérieurs ou simplement conjugués. Les orbites sont appelées classes de conjugaison. De même, deux parties H et $H'$ de G sont dites conjuguées s’il existe un élément $\alpha \in G$ tel que $H' = \alpha.H.\alpha^{-1}$, c’est-à-dire si elles sont conjuguées pour l’extension à $\mathfrak{P}(G)$ de l’opération de G sur lui-même par automorphismes intérieurs.

#### Exemple 2 {#alg-i-s5-n4-exa-2 .statement}

\* Dans l’espace $\mathbf{R}^n$, l’orbite d’un point x pour l’opération du groupe orthogonal $\mathbf{O}(n, \mathbf{R})$ est la sphère euclidienne de rayon $\|x\|_*$.

Les stabilisateurs de deux éléments conjugués de E sont des sous-groupes conjugués de G (I, p. 52, prop. 2).

L’ensemble quotient de E par la relation de conjugaison est l’ensemble des orbites de E; on le note parfois E/G ou $G\backslash E$. (On réserve parfois la notation E/G au cas où E est un G-ensemble à droite, et la notation $G \backslash E$ au cas où E est un G-ensemble à gauche).

Soit G un groupe opérant à droite dans un ensemble E. Soit H un sous-groupe distingué de G. Le groupe G opère à droite sur E/H, la loi d’action à droite correspondante étant $(xH, g) \mapsto xHg = xgH$; pour cette opération, H opère trivialement, d’où une opération à droite de G/H sur E/H. Soit $\varphi$ l’application canonique de E/H sur E/G; les images réciproques par $\varphi$ des points de E/G sont les orbites de G (ou de G/H) dans E/H. Donc $\varphi$ définit par passage au quotient une bijection, dite canonique, de $(E/H)/G = (E/H)/(G/H)$ sur E/G.

Soit G (resp. H) un groupe opérant à gauche (resp. à droite) sur un ensemble E. Supposons que les actions de G et H sur E commutent, c’est-à-dire que l’on ait

$$
(g.x).h = g.(x.h) \quad \text{pour } g \in G,\ x \in E \text{ et } h \in H.
$$

L’action de H sur E est aussi une opération à gauche du groupe H$^0$ opposé à H. Il résulte alors de I, p. 45, prop. 12 que l’application qui, à l’élément $(g, h) \in G \times H^0$ fait correspondre l’application $x \mapsto g.x.h$ de E dans lui-même est une opération à gauche de $G \times H^0$ sur E. L’orbite d’un élément $x \in E$ pour cette opération est l’ensemble $GxH$. L’ensemble de ces orbites se note $G \backslash E/H$. D’autre part, l’opération de G (resp. H) est compatible avec la relation de conjugaison pour l’opération de H (resp. G) et l’ensemble des orbites $G \backslash (E/H)$ (resp. $(G \backslash E)/H$) s’identifie à $G \backslash E/H$: dans le diagramme

$$
\begin{array}{ccc}
E & & \\
| & & | \\
G\backslash E & \alpha & E/H \\
| & & | \\
G\backslash E/H & \gamma & G\backslash E/H \\
| & & | \\
& \varepsilon & \\
& & \\
& & \\
\end{array}
$$

(où $\alpha, \beta, \gamma, \delta, \varepsilon$ désignent les applications canoniques de passage au quotient), on a $\gamma \circ \alpha = \delta \circ \beta = \varepsilon$.

Soient G un groupe et H un sous-groupe de G. Considérons l’opération à droite de H sur G par translations à droite (I, p. 50, Exemple 2). L’ensemble des orbites G/H est l’ensemble des classes à gauche suivant H; remarquons que G opère à gauche sur G/H par la loi $(g, xH) \mapsto gxH$ (cf. I, p. 56). De même, l’ensemble des classes à droite suivant H est l’ensemble $H \backslash G$ des orbites de l’opération à gauche de H sur G par translations à gauche. Si K est un sous-groupe de G contenant H et si $\Gamma$ est une classe à gauche (resp. à droite) suivant H, alors $\Gamma K$ (resp. $K\Gamma$) est une classe à gauche (resp. à droite) suivant K. L’application

Γ ↦ ΓK (resp. Γ ↦ KΓ) est appelée l’application canonique de G/H dans G/K (resp. de $H\backslash G$ dans $K\backslash G$). Elle est surjective.

Soient G un groupe, H et K deux sous-groupes de G. Faisons opérer H à gauche sur G par translations à gauche et K à droite par translations à droite; ces deux opérations commutent, ce qui permet de considérer l’ensemble $H\backslash G/K$. Les éléments de $H\backslash G/K$ s’appellent les doubles classes de G suivant (ou modulo) H et K. Lorsque K = H, on dit simplement doubles classes suivant H. Pour que l’application canonique de $G/H$ sur $H\backslash G/H$ soit une bijection, il faut et il suffit que H soit un sous-groupe distingué de G.

### 5. Ensembles homogènes

#### Définition 6 {#alg-i-s5-def-6 .statement}

Soit G un groupe. On dit qu’une opération de G sur un ensemble E est transitive s’il existe un élément x ∈ E dont l’orbite soit E. Un G-ensemble E est dit homogène si l’opération de G sur E est transitive.

On dit aussi que G opère transiti vement sur E; ou que E est un ensemble homogène sous G. Il revient au même de dire que E n’est pas vide et que, quels que soient les éléments x et y de E, il existe un élément α ∈ G tel que α.x = y.

#### Exemple {#alg-i-s5-n5-exa-4 .statement}

Si E est un G-ensemble, chaque orbite de E, munie de l’opération induite, est un ensemble homogène sous G.

Soient G un groupe et H un sous-groupe de G. Considérons l’ensemble G/H des classes à gauche suivant H. Le groupe G opère à gauche sur G/H par (g, xH) ↦ gxH. Soit N le normalisateur de H. Le groupe N opère à droite sur G/H par (xH, n) ↦ xHn = xnH. Cette opération induit sur H l’opération triviale, donc, par passage au quotient, N/H opère à droite sur G/H. Soit φ : (N/H)^0 → S_{G/H} l’homomorphisme correspondant à cette opération.

#### Proposition 5 {#alg-i-s5-prop-5 .statement}

Avec les notations ci-dessus, G/H est un G-ensemble homogène. L’application φ induit un isomorphisme de (N/H)^0 sur le groupe des automorphismes du G-ensemble G/H.

L’orbite dans G/H de l’élément e = H est G/H, d’où la première assertion. Démontrons la seconde. Si n ∈ N définit par translation à droite l’application identique de G/H, on a e.n = e, soit H.n = H, d’où n ∈ H. Par suite, N/H opère à droite fidèlement sur G/H et φ est injectif. Les opérations de G à gauche et de N/H à droite sur G/H commutent, donc les opérateurs de N/H définissent des G-morphismes de G/H dans lui-même, qui sont nécessairement des G-automorphismes car ils sont bijectifs. Par suite, φ prend ses valeurs dans le groupe Φ des G-automorphismes de G/H. Montrons que l’image de φ est Φ. Soit f ∈ Φ. Par transport de structure, le stabilisateur de f(e) dans G est égal au stabilisateur de e, donc à H. Soit n ∈ G tel que f(e) = ne. Le stabilisateur de ne dans G est nHn^{-1} (I, p. 52, prop. 2), d’où nHn^{-1} = H, et n ∈ N. Pour tout élément xH de G/H, on a f(xH) = f(x.e) = x.f(e) = xnH = xHn, et f coïncide avec l’application définie par n.

#### Remarque 1 {#alg-i-s5-n5-rem-1 .statement}

Soient G un groupe, H un sous-groupe de G et $\varphi : G \to \mathcal{S}_{G/H}$ l’opération de G sur G/H. Le noyau de $\varphi$ est l’intersection des conjugués de H (I, p. 52, prop. 2). C’est aussi le plus grand sous-groupe distingué contenu dans H (I, p. 54). En particulier, G opère fidèlement sur G/H si et seulement si l’intersection des conjugués de H est réduite à e.

#### Remarque 2 {#alg-i-s5-n5-rem-2 .statement}

Soient G un groupe, H et K deux sous-groupes tels que H soit un sous-groupe distingué de K. Alors K/H opère à droite sur le G-ensemble G/H et l’application canonique de G/H sur G/K définit par passage au quotient un isomorphisme de G-ensembles $(G/H)/(K/H) \to G/K$ (cf. I, p. 55).

#### Proposition 6 {#alg-i-s5-prop-6 .statement}

Soient G un groupe, E un G-ensemble homogène, $a \in E$, H le stabilisateur de a, K un sous-groupe de G contenu dans H. Il existe un et un seul G-morphisme f de G/K dans E tel que $f(K) = a$ et f est surjectif. Si K = H, f est un isomorphisme.

Si f répond à la question, on a $f(x.K) = x.a$ pour tout x de G, d’où l’unicité; démontrons l’existence. L’application orbitale définie par a est compatible avec la relation d’équivalence $y \in xK$ dans G. En effet, si $y = xk, k \in K$, on a $y.a = xk.a = x.a$. On en déduit donc une application f de G/K dans E qui vérifie $f(x.K) = x.a$ pour tout x de G. Cette application est un G-morphisme et $f(K) = a$. Cette application est surjective car son image est une partie stable non vide de E. Supposons maintenant que K = H et montrons que f est injective. Si $f(x.H) = f(y.H)$, on a $x.a = y.a$ d’où $x^{-1}y.a = a$ et $x^{-1}y \in H$, d’où $x.H = y.H$.

#### Théorème 1 {#alg-i-s5-thm-1 .statement}

Soit G un groupe.

a) Tout G-ensemble homogène est isomorphe à un G-ensemble homogène de la forme G/H, où H est un sous-groupe de G.

b) Soient H et H’ deux sous-groupes de G. Les G-ensembles G/H et G/H’ sont isomorphes si et seulement si H et H’ sont conjugués.

Comme un G-ensemble homogène n’est pas vide, l’assertion a) résulte de la prop. 6. Démontrons b). Soit $f : G/H \to G/H'$ un isomorphisme de G-ensembles. Le sous-groupe H est le stabilisateur de H, donc, par transport de structure, le stabilisateur d’un élément de G/H’. Les sous-groupes H et H’ sont donc conjugués (I, p. 52, prop. 2). Si $H' = \alpha H \alpha^{-1}$, H’ est le stabilisateur de l’élément $\alpha.H$ de G/H (I, p. 52, prop. 2), donc G/H’ est isomorphe à G/H (prop. 6).

#### Exemple 1 {#alg-i-s5-n5-exa-1 .statement}

Soit E un ensemble non vide. Le groupe $\mathcal{S}_E$ opère transitivement sur E. En effet, si x et y sont deux éléments de E, l’application $\tau : E \to E$, telle que $\tau(x) = y, \tau(y) = x$ et $\tau(z) = z$ pour $z \neq x, y$, est une permutation de E. Soit $a \in E$. Le stabilisateur de a s’identifie à $\mathcal{S}_F$, où $F = E - \{a\}$. Le $\mathcal{S}_E$-ensemble homogène E est donc isomorphe à $\mathcal{S}_E/\mathcal{S}_F$.

#### Exemple 2 {#alg-i-s5-n5-exa-2 .statement}

Soient E un ensemble à n éléments et $(p_i)_{i \in I}$ une famille finie d’entiers > 0 telle que $\sum_i p_i = n$. Soit X l’ensemble des partitions $(F_i)_{i \in I}$ de E telles que Card$(F_i) = p_i$ pour tout i. Le groupe $\mathcal{S}_E$ opère transitivement sur X. Le stabilisateur H d’un élément $(F_i)_{i \in I}$ de X est canoniquement isomorphe à $\prod_{i \in I} \mathcal{S}_{F_i}$, donc d’ordre $\prod_{i \in I} p_i!$.

En appliquant le th. 1 et I, p. 34, corollaire on obtient une nouvelle démonstration du fait que

$$
\operatorname{Card}(X) = \frac{n!}{\prod_{i \in I} p_i!}
$$

En particulier, prenons $I = \{1, 2, \ldots, r\}, E = \{1, 2, \ldots, n\},$

$$
F_i = \{p_1 + \cdots + p_{i-1} + 1, \ldots, p_1 + \cdots + p_i\}
$$
pour $1 \leq i \leq r$. Soit S l’ensemble des $\tau \in \mathfrak{S}_E$ tels que $\tau|F_i$ soit croissante pour $1 \leq i \leq r$. Si $(G_1, \ldots, G_r) \in X$ il existe une $\tau \in S$ et une seule qui transforme $(F_1, \ldots, F_r)$ en $(G_1, \ldots, G_r)$. Autrement dit, chaque classe à gauche de $\mathfrak{S}_E$ suivant H rencontre S en un point et un seul.

#### Exemple 3 {#alg-i-s5-n5-exa-3 .statement}

\* Soit $n$ un entier $\geq 1$. Le groupe orthogonal $\mathbf{O}(n, \mathbf{R})$ opère transitivement sur la sphère unité $S_{n-1}$ de $\mathbf{R}^n$. Le stabilisateur du point $(0, \ldots, 0, 1)$ s’identifie au groupe orthogonal $\mathbf{O}(n-1, \mathbf{R})$. Le $\mathbf{O}(n, \mathbf{R})$-ensemble homogène $S_{n-1}$ est donc isomorphe à $\mathbf{O}(n, \mathbf{R})/\mathbf{O}(n-1, \mathbf{R})$.*

### 6. Ensembles principaux homogènes

#### Définition 7 {#alg-i-s5-def-7 .statement}

Soit G un groupe. On dit qu’une opération de G sur un ensemble E est simplement transitive s’il existe un élément x de E tel que l’application orbitale définie par x soit une bijection. Un ensemble E muni d’une opération à gauche simplement transitive de G sur E est appelé G-ensemble principal homogène à gauche (ou ensemble principal homogène à gauche sous G).

Il revient au même de dire que G opère librement et transitivement sur E, ou encore qu’il existe un élément $x \in E$ tel que l’application orbitale définie par x soit un isomorphisme du G-ensemble G (où G opère par translations à gauche) sur E; ou encore que les deux conditions suivantes sont satisfaites:

(i) E n’est pas vide;
(ii) quels que soient les éléments x et y de E, il existe un élément $\alpha \in G$ et un seul tel que $\alpha x = y$.

La condition (ii) est encore équivalente à la condition suivante:
(iii) l’application $(\alpha, x) \mapsto (\alpha x, x)$ est une bijection de $G \times E$ sur $E \times E$.

Nous laissons au lecteur le soin de définir les G-ensembles principaux homogènes à droite.

#### Exemple 1 {#alg-i-s5-n6-exa-1 .statement}

Faisons opérer G sur lui-même par translations à gauche (resp. à droite). On définit ainsi sur l’ensemble G une structure de G-ensemble principal homogène à gauche (resp. à droite), qu’on note parfois $G_s$ (resp. $G_d$).

#### Exemple 2 {#alg-i-s5-n6-exa-2 .statement}

Soit E un ensemble homogène sous un groupe commutatif G. Si G opère fidèlement sur E, celui-ci est un G-ensemble principal homogène.

#### Exemple 3 {#alg-i-s5-n6-exa-3 .statement}

Soient E et F deux ensembles munis de structures de même espèce isomorphes, et soit Isom(E, F) l’ensemble des isomorphismes de E sur F (pour les structures données). Le groupe Aut(E) des automorphismes de E (muni de la structure donnée) opère à droite sur Isom(E, F) par la loi $(\sigma, f) \mapsto f \circ \sigma$ et Isom(E, F) est un Aut(E)-ensemble principal homogène à droite. De même, le groupe Aut(F) opère à gauche sur Isom(E, F) par la loi $(\sigma, f) \mapsto \sigma \circ f$ et Isom(E, F) est un Aut(F)-ensemble principal homogène à gauche.

#### Exemple 4 {#alg-i-s5-n6-exa-4 .statement}

Un ensemble principal homogène sous le groups additif d’un espace vectoriel est appelé un espace affine (cf. II, p. 126).*

Le groupe des automorphismes du G-ensemble principal homogène $G_s$ (Exemple 1) est le groupe des translations à droite de G qu’on identifie à $G^0$ (I. p. 56, prop. 5). Soient E un G-ensemble principal homogène, $a$ un élément de E. L’application orbitale $\omega_a$ définie par $a$ est un isomorphisme du G-ensemble $G_s$ sur E. Par transport de structure on en déduit un isomorphisme $\psi_a$ de $G^0$ sur Aut(E). On prendra garde que $\psi_a$ dépend en général de $a$; plus précisément, pour $\alpha \in G$, on a

$$
\psi_{\alpha a} = \psi_a \circ \mathrm{Int}_{G^0}(\alpha) = \psi_a \circ \mathrm{Int}(\alpha^{-1}).
$$

En effet, en notant $\delta_\alpha$ la translation $x \mapsto x\alpha$ dans G, on a

$$
\omega_{\alpha a} = \omega_a \circ \delta_\alpha
$$

et

$$
\psi_a(x) = \omega_a \circ \delta_x \circ \omega_a^{-1}, \quad x \in G,
$$

d’où

$$
\psi_{\alpha a}(x) = \omega_a \circ \delta_\alpha \circ \delta_x \circ \delta_\alpha^{-1} \circ \omega_a^{-1} = \omega_a \circ \delta_{\alpha^{-1} x \alpha} \circ \omega_a^{-1} = \psi_a(\alpha^{-1} x \alpha).
$$

### 7. Groupe des permutations d’un ensemble fini

Si E est un ensemble fini à $n$ éléments, le groupe symétrique $\mathfrak{S}_E$ (I, p. 29) est un groupe fini d’ordre $n!$. Lorsque E est l’intervalle $\{1, n\}$ de l’ensemble $\mathbf{N}$ des entiers naturels, le groupe symétrique correspondant se note $\mathfrak{S}_n$; le groupe symétrique d’un ensemble quelconque à $n$ éléments est isomorphe à $\mathfrak{S}_n$.

#### Définition 8 {#alg-i-s5-def-8 .statement}

Soient E un ensemble fini, $\zeta \in \mathfrak{S}_E$ une permutation de E, $\bar{\zeta}$ le sous-groupe de $\mathfrak{S}_E$ engendré par $\zeta$. On dit que $\zeta$ est un cycle si, pour l’opération de $\bar{\zeta}$ sur E, il existe une orbite et une seule qui ne soit pas réduite à un élément. Cette orbite est appelée le support de $\zeta$.

Soit $\zeta$ un cycle. Le support de $\zeta$, noté $\mathrm{supp}(\zeta)$ est l’ensemble des $x \in E$ tels que $\zeta(x) \neq x$.

L’ordre d’un cycle $\zeta$ est égal au cardinal de son support. En effet, le sous-groupe $\bar{\zeta}$ engendré par $\zeta$ opère transitiivement et fidèlement sur $\mathrm{supp}(\zeta)$. Comme $\bar{\zeta}$ est commutatif, $\mathrm{supp}(\zeta)$ est un ensemble principal sous $\bar{\zeta}$ (I, p. 58, Exemple 2), donc $\mathrm{Card}(\mathrm{supp}(\zeta)) = \mathrm{Card}(\bar{\zeta})$.

#### Lemme 1 {#alg-i-s5-lem-1 .statement}

Soit $(\zeta_i)_{i \in I}$ une famille de cycles dont les supports $S_i$ sont deux à deux disjoints. Alors les $\zeta_i$ sont deux à deux permutables. Posons $\sigma = \prod_{i \in I} \zeta_i$ et soit $\bar{\sigma}$ le sous-groupe engendré par $\sigma$. On a $\sigma(x) = \zeta_i(x)$ pour $x \in S_i, i \in I$, et $\sigma(x) = x$ pour $x \notin \bigcup_{i \in I} S_i$. L’application $i \mapsto S_i$ est une bijection de I sur l’ensemble des $\bar{\sigma}$-orbites non réduites à un élément.

Soient $\zeta$ et $\zeta'$ deux cycles dont les supports sont disjoints. Si
$$
x \notin \operatorname{supp}(\zeta) \cup \operatorname{supp}(\zeta'),
$$
on a $\zeta \zeta'(x) = \zeta' \zeta(x) = x$. Si $x$ appartient au support de $\zeta$, on a $\zeta'(x) = x$ et $\zeta(x)$ appartient au support de $\zeta$, d’où $\zeta \zeta'(x) = \zeta' \zeta(x) = \zeta(x)$. De même lorsque $x$ appartient au support de $\zeta'$, on a $\zeta' \zeta(x) = \zeta \zeta'(x) = \zeta'(x)$. Donc $\zeta \zeta' = \zeta' \zeta$. Par suite, les $\zeta_i$ sont deux à deux permutables, et pour $i \in I$ et $x \in S_i$, on a $\sigma(x) = \zeta_i(x) \in S_i$. Les applications $\sigma$ et $\zeta_i$ coïncident dans $S_i$, donc $S_i$ est stable par $\sigma$ et le sous-groupe de $\mathfrak{S}_{S_i}$ engendré par la restriction de $\sigma$ à $S_i$ opère transitiivement sur $S_i$; par suite $S_i$ est une $\bar{\sigma}$-orbite. Comme les $S_i$ ne sont pas vides et sont deux à deux disjoints, l’application $i \mapsto S_i$ est injective. Comme $\bigcup_i S_i$ est l’ensemble des $x$ tel que $\sigma(x) \neq x$, toute $\bar{\sigma}$-orbite non réduite à un élément est l’un des $S_i$.

#### Proposition 7 {#alg-i-s5-prop-7 .statement}

*Soient E un ensemble fini et $\sigma$ une permutation de E. Il existe un ensemble fini C de cycles et un seul, satisfaisant aux deux conditions suivantes:*
a) *les supports des éléments de C sont deux à deux disjoints;*
b) *on a $\sigma = \prod_{\zeta \in C} \zeta$* (les éléments de C étant deux à deux permutables d’après le lemme 1).

Soit $\bar{\sigma}$ le sous-groupe engendré par $\sigma$ et soit S l’ensemble des $\bar{\sigma}$-orbites non réduites à un élément. Pour $s \in S$, posons $\zeta_s(x) = \sigma(x)$ si $x \in s$ et $\zeta_s(x) = x$ si $x \notin s$. Pour tout $s \in S$, $\zeta_s$ est un cycle dont le support est $s$, et l’on a $\sigma = \prod_{s \in S} \zeta_s$, comme on le voit en appliquant les deux membres à un élément quelconque de E. L’unicité de C résulte du lemme 1.

#### Définition 9 {#alg-i-s5-def-9 .statement}

*Un cycle d’ordre 2 est appelé une transposition.*

Soient $x$ et $y$ deux éléments *distincts* de E. On note $\tau_{x,\ y}$ l’unique transposition de support $\{x, y\}$.

Pour toute permutation $\sigma$ de E, la permutation $\sigma . \tau_{x,\ y} . \sigma^{-1}$ est une transposition dont le support est $\{\sigma(x), \sigma(y)\}$. On a donc:

(4)
$$
\sigma . \tau_{x,\ y} . \sigma^{-1} = \tau_{\sigma(x),\ \sigma(y)}.
$$

Les transpositions forment donc dans le groupe $\mathfrak{S}_E$ une classe de conjugaison.

#### Proposition 8 {#alg-i-s5-prop-8 .statement}

*Soit E un ensemble fini. Le groupe $\mathfrak{S}_E$ est engendré par les transpositions.*

Pour toute permutation $\sigma$, soit $F_\sigma$ l’ensemble des $x \in E$ tels que $\sigma(x) = x$. Montrons, par récurrence descendante sur $p$, que toute permutation $\sigma$ telle que $\operatorname{Card}(F_\sigma) = p$ est un produit de transpositions. Si $p \geq \operatorname{Card}(E)$, la permutation $\sigma$ est l’application identique de E; c’est le produit de la famille vide de transpositions. Si $p < \operatorname{Card}(E)$, supposons la propriété démontrée pour toute permutation $\sigma'$ telle que $\operatorname{Card}(F_{\sigma'}) > p$. On a $E - F_\sigma \neq \varnothing$; soient $x \in E - F_\sigma$ et $y = \sigma(x)$. On a $y \neq x$ et $y \in E - F_\sigma$. Posons $\sigma' = \tau_{x,\ y} . \sigma$. L’ensemble $F_{\sigma'}$ contient $F_{\sigma}$ et $x$, donc $\mathrm{Card}(F_{\sigma'}) > \mathrm{Card}(F_{\sigma}) = p$. Par l’hypothèse de récurrence, $\sigma'$ est produit de transpositions, donc $\sigma = \tau_{x,y} \cdot \sigma'$ est produit de transpositions.

#### Proposition 9 {#alg-i-s5-prop-9 .statement}

*Soit n un entier $\geqslant 0$. Le groupe $\mathfrak{S}_n$ est engendré par la famille des transpositions $(\tau_{i,i+1})_{1 \leqslant i \leqslant n-1}$*.

En vertu de la prop. 8, il suffit de montrer que toute transposition $\tau_{p,q}$ pour $1 \leqslant p < q \leqslant n$, appartient au sous-groupe $H$ engendré par les $\tau_{i,i+1}$ pour $1 \leqslant i \leqslant n-1$. Démontrons ceci par récurrence sur $q - p$. Pour $q - p = 1$, c’est évident. Si $q - p > 1$, on a (I, p. 60, formule (4)) $\tau_{p,q} = \tau_{q-1,q} \tau_{p,q-1} \tau_{q-1,q}$. Par l’hypothèse de récurrence, $\tau_{p,q-1} \in H$, et par suite $\tau_{p,q} \in H$.

Si $\sigma \in \mathfrak{S}_n$, on appelle *inversion* de $\sigma$ tout couple $(i,j)$ d’éléments de $[1,n]$ tel que $i < j$ et $\sigma(i) > \sigma(j)$. Notons $v(\sigma)$ le nombre d’inversions de $\sigma$.

Soit $P$ le groupe additif des applications de $\mathbf{Z}^n$ dans $\mathbf{Z}$. Pour $f \in P$ et $\sigma \in \mathfrak{S}_n$, soit $\sigma f$ l’élément de $P$ défini par
$$
\sigma f(z_1, \ldots, z_n) = f(z_{\sigma(1)}, \ldots, z_{\sigma(n)}).
$$
L’action de $\mathfrak{S}_n$ sur $P$ ainsi définie est une opération; en effet, pour $\sigma, \tau$ dans $\mathfrak{S}_n$ et $f \in P$, on a $ef = f$ et
$$
\begin{align*}
(\tau(\sigma f))(z_1, \ldots, z_n) &= \sigma f(z_{\tau(1)}, \ldots, z_{\tau(n)}) = f(z_{\tau \sigma(1)}, \ldots, z_{\tau \sigma(n)}) \\
&= ((\tau \sigma)f)(z_1, \ldots, z_n).
\end{align*}
$$
La formule (5) montre que $\sigma(-f) = -\sigma f$ pour $\sigma \in \mathfrak{S}_n$ et $f \in P$.

Soit $p$ l’élément de $P$ défini par
$$
p(z_1, \ldots, z_n) = \prod_{i < j} (z_j - z_i).
$$

#### Lemme 2 {#alg-i-s5-lem-2 .statement}

*On a $p \neq 0$ et $\sigma p = (-1)^{v(\sigma)} p$ pour $\sigma \in \mathfrak{S}_n$*.

On a $p(1,2,\ldots,n) = \prod_{i < j} (j-i) \neq 0$, donc $p \neq 0$. D’autre part, si $\sigma \in \mathfrak{S}_n$, on a
$$
\sigma p(z_1, \ldots, z_n) = p(z_{\sigma(1)}, \ldots, z_{\sigma(n)}) = \prod_{i < j} (z_{\sigma(j)} - z_{\sigma(i)}).
$$

Soit $C$ l’ensemble des couples $(i,j)$ tels que $1 \leqslant i \leqslant n, 1 \leqslant j \leqslant n, i < j$. On définit une permutation $\theta$ de $C$ en posant $\theta(i,j) = (\sigma(i), \sigma(j))$ si $(i,j)$ n’est pas une inversion, $\theta(i,j) = (\sigma(j), \sigma(i))$ si $(i,j)$ est une inversion. Cela entraîne $\sigma p = (-1)^{v(\sigma)} p$.

#### Théorème 2 {#alg-i-s5-thm-2 .statement}

*Soit $E$ un ensemble fini. Il existe un homomorphisme $\varepsilon$ et un seul de $\mathfrak{S}_E$ dans le groupe multiplicatif $\{-1,+1\}$ tel que $\varepsilon(\tau) = -1$ pour toute transposition $\tau$*.

L’unicité résulte de I, p. 60, prop. 8. Démontrons l’existence. Par transport de structure, on peut supposer que $E = \{1,n\}$. Avec les notations précédentes, posons $\varepsilon(\sigma) = (-1)^{v(\sigma)}$. On a (lemme 2)
$$
\sigma(\sigma' p) = \sigma(\varepsilon(\sigma') p) = \varepsilon(\sigma') (\sigma p) = \varepsilon(\sigma') \varepsilon(\sigma) p.
$$
D’autre part,
$$
\sigma(\sigma' p) = (\sigma \sigma') p = \varepsilon(\sigma \sigma') p.
$$

Comme $p \neq -p$, on en déduit $\varepsilon(\sigma\sigma') = \varepsilon(\sigma)\varepsilon(\sigma')$, donc $\varepsilon$ est un homomorphisme. Montrons que, pour toute transposition $\tau$, on a $\varepsilon(\tau) = -1$. On a $\nu(\tau_{n-1,n}) = 1$, d’où $\varepsilon(\tau_{n-1,n}) = -1$. Comme toute transposition $\tau$ est conjuguée de $\tau_{n-1,n}$ et que le groupe $\{-1,+1\}$ est commutatif, on a $\varepsilon(\tau) = \varepsilon(\tau_{n-1,n}) = -1$.

#### Définition 10 {#alg-i-s5-def-10 .statement}

Avec les notations du théorème 2, le nombre $\varepsilon(\sigma)$ (noté aussi $\varepsilon_\sigma$) est appelé la signature de la permutation $\sigma$. Le noyau de l’homomorphisme $\varepsilon$ est appelé le groupe alterné de $E$.

On dit que $\sigma$ est *paire* (resp. *impaire*) si $\varepsilon(\sigma) = 1$ (resp. $\varepsilon(\sigma) = -1$). Le groupe alterné de $E$ est noté $\mathfrak{A}_E$. C’est un sous-groupe distingué de $\mathfrak{S}_E$. Lorsque $E = \{1, n\}$, on le note simplement $\mathfrak{A}_n$. Lorsque le cardinal $n$ de $E$ est $\geqslant 2$, $\mathfrak{A}_n$ est un sous-groupe d’indice 2 de $\mathfrak{S}_n$, donc d’ordre $\frac{n!}{2}$. On peut montrer que, pour $n = 3$ ou $n \geqslant 5$, le groupe $\mathfrak{A}_n$ est un groupe simple (cf. I, p. 131, exerc. 16).

#### Exemple {#alg-i-s5-n7-exa-1 .statement}

Si $\sigma$ est un cycle d’ordre $d$, on a
$$
\varepsilon(\sigma) = (-1)^{d-1}.
$$
En effet, le nombre d’inversions de la permutation
$$
(1, 2, 3, \ldots, d) \mapsto (d, 1, 2, \ldots, d-1)
$$
est égal à $d-1$.

## EXERCICES {#alg-i-s5-exercises}

See the [exercises for § 5](exercises/s5/).
