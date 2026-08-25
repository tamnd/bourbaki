---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 1
section_title: Formes sesquilinéaires
lang: fr
source: alg-ix-fr
pdf_pages: 0005-0038
extraction: ocr
subsections:
    - "no": 1
      title: Applications bilinéaires.
      page: 0
      pdf_page: 5
    - "no": 2
      title: Applications sesquilinéaires.
      page: 0
      pdf_page: 8
    - "no": 3
      title: Orthogonalité. Sommes directes d’applications bilinéaires ou sesquilinéaires.
      page: 0
      pdf_page: 10
    - "no": 4
      title: Changement d’anneaux de base.
      page: 0
      pdf_page: 11
    - "no": 5
      title: Quelques identités.
      page: 0
      pdf_page: 16
    - "no": 6
      title: Formes bilinéaires et sesquilinéaires. Rang.
      page: 0
      pdf_page: 16
    - "no": 7
      title: Forme inverse d’une forme bilinéaire ou sesquilinéaire.
      page: 0
      pdf_page: 21
    - "no": 8
      title: Adjoint d’un homomorphisme.
      page: 0
      pdf_page: 23
    - "no": 9
      title: Produits tensoriels et puissances extérieures de formes sesquilinéaires.
      page: 0
      pdf_page: 25
    - "no": 10
      title: Calculs matriciels.
      page: 0
      pdf_page: 30
statements: 45
exercises: 0
content_sha256: e02ca70e6485727bec2c4fbc8b27cc8126199083a8bd87ce7a3060466b192a62
---

## § 1. Formes sesquilinéaires

### 1. Applications bilinéaires.

Dans ce no l’on désigne par $A$ et $B$ deux anneaux, par $E$ un $A$-module à gauche, par $F$ un $B$-module à droite, et par $G$ un $(A, B)$-bimodule, c’est-à-dire un groupe commutatif muni d’une structure de $A$-module à gauche et d’une structure de $B$-module à droite telles que l’on ait $(ag)b = a(gb)$ quels que soient $a \in A$, $b \in B$, $g \in G$.

#### Définition 1 {#alg-ix-s1-def-1 .statement}

On dit qu’une application $\Phi$ du produit $E \times F$ dans $G$ est bilinéaire si elle satisfait aux conditions suivantes :

(1) $\Phi(x + x', y) = \Phi(x, y) + \Phi(x', y)$
    quels que soient $x \in E$, $x' \in E$, $y \in F$ ;
(2) $\Phi(x, y + y') = \Phi(x, y) + \Phi(x, y')$
    quels que soient $x \in E$, $y \in F$, $y' \in F$ ;
(3) $\Phi(ax, y) = a\Phi(x, y)$ quels que soient $a \in A$, $x \in E$, $y \in F$ ;
(4) $\Phi(x, yb) = \Phi(x, y)b$ quels que soient $x \in E$, $y \in F$, $b \in B$.

Le produit tensoriel $E \otimes_{\mathbf{Z}} F$ est canoniquement muni d’une structure de $(A, B)$-bimodule caractérisée par $a(x \otimes y)b = ax \otimes yb$ (Chap. III, 2e éd., App. II, n° 3), et la donnée d’une application bilinéaire $\Phi$ de $E \times F$ dans $G$ équivaut à celle d’une application $\Psi$ de $E \otimes_{\mathbf{Z}} F$ dans $G$ qui soit un homomorphisme pour les structures de $(A, B)$-bimodules et qui vérifie $\Psi(x \otimes y) = \Phi(x, y)$ quels que soient $x \in E$ et $y \in F$.

Les conditions imposées à $\Phi$ par la définition 1 signifient que les applications partielles $d_\Phi(y) : x \to \Phi(x, y)$ et $s_\Phi(x) : y \to \Phi(x, y)$ sont respectivement une application A-linéaire de $E$ dans $G$ et une application B-linéaire de $F$ dans $G$. Munissons le groupe commutatif $\mathcal{L}_A(E, G)$ (resp. $\mathcal{L}_B(F, G)$) de la structure de B-module à droite (resp. de A-module à gauche) définie par $ub(x) = u(x) . b$ ($u \in \mathcal{L}_A(E, G)$, $x \in E$, $b \in B$) (resp. $a \nu(y) = a . \nu(y)$ ($a \in A$, $\nu \in \mathcal{L}_B(F, G)$, $y \in F$)). Alors les conditions (1) à (4) sont respectivement équivalentes à :

$$
\begin{align*}
(1') & \quad s_\Phi(x + x') = s_\Phi(x) + s_\Phi(x') \\
(2') & \quad d_\Phi(y + y') = d_\Phi(y) + d_\Phi(y') \\
(3') & \quad s_\Phi(ax) = a.s_\Phi(x) \\
(4') & \quad d_\Phi(yb) = d_\Phi(y).b,
\end{align*}
$$

quels que soient $x, x'$ dans $E$, $y, y'$ dans $F$, $a \in A$, $b \in B$; autrement dit, l’application $d_\Phi$ de $F$ dans $\mathcal{L}_A(E, G)$ est B-linéaire, et l’application $s_\Phi$ de $E$ dans $\mathcal{L}_B(F, G)$ est A-linéaire. On a, par définition

$$(5) \quad \Phi(x, y) = d_\Phi(y)(x) = s_\Phi(x)(y) \text{ quels que soient } x \in E, y \in F.$$

#### Définition 2 {#alg-ix-s1-def-2 .statement}

Etant donnée une application bilinéaire $\Phi$ de $E \times F$ dans $G$, l’application $d_\Phi$ de $F$ dans $\mathcal{L}_A(E, G)$ (resp. l’application $s_\Phi$ de $E$ dans $\mathcal{L}_B(F, G)$) caractérisée par (5) est appelée l’application linéaire associée à droite (resp. à gauche) à $\Phi$.

Inversement la donnée d’une application B-linéaire $d$ de $F$ dans $\mathcal{L}_A(E, G)$ (resp. d’une application A-linéaire $s$ de $E$ dans $\mathcal{L}_B(F, G)$) détermine de façon unique, par la formule

$$
\Phi(x, y) = d(y)(x) \quad \text{(resp. } \Phi(x, y) = s(x)(y))
$$

une application bilinéaire $\Phi$ de $E \times F$ dans $G$, dont $d$ (resp. $s$) est l’application linéaire associée à droite (resp. à gauche).

#### Définition 3 {#alg-ix-s1-def-3 .statement}

Une application bilinéaire $\Phi$ de $E \times F$ dans $G$ est dite dégénérée à droite (resp. à gauche) s’il existe un élément non nul $y_0$ de $F$ (resp. $x_0$ de $E$) tel que $\Phi(x, y_0) = 0$ pour tout $x \in E$ (resp. $\Phi(x_0, y) = 0$ pour tout $y \in F$). On dit que $\Phi$ est dégénérée si elle est dégénérée à droite ou si elle est dégénérée à gauche.

Pour que $\Phi$ soit non dégénérée à droite (resp. à gauche) il faut et il suffit que l’application linéaire associée à droite (resp. à gauche) à $\Phi$ soit injective ; dire que $\Phi$ est non dégénérée signifie donc que les applications linéaires associées $d_\Phi$ et $s_\Phi$ sont toutes deux injectives.

Soient $(e_i)_{i \in I}$ et $(f_k)_{k \in K}$ deux familles d’éléments de $E$ et $F$, et soient $(a_i)_{i \in I}$ et $(b_k)_{k \in K}$ deux familles d’éléments de $A$ et $B$ nuls à l’exception d’un nombre fini d’entre eux. Il résulte des égalités (1) à (4), par récurrence sur le nombre des coefficients non nuls, que l’on a

$$
\Phi(\sum_i a_i e_i, \sum_k f_k b_k) = \sum_{i,k} a_i \Phi(e_i, f_k) b_k.
$$

Si $(e_i)$ et $(f_k)$ sont des systèmes de générateurs des modules $E$ et $F$, $\Phi$ est donc complètement déterminée par les éléments $g_{ik} = \Phi(e_i, f_k)$. Si $(e_i)$ et $(f_k)$ sont des bases de $E$ et $F$ et que l’on se donne des éléments $g_{ik}$ de $G$ ($i \in I, k \in K$), alors la formule

$$
\Phi(\sum_i a_i e_i, \sum_k f_k b_k) = \sum_{i,k} a_i g_{ik} b_k
$$

définit une application de $E \times F$ dans $G$, qui est bilinéaire et qui vérifie $\Phi(e_i, f_k) = g_{ik}$. Lorsque $(e_i)$ et $(f_k)$ sont des bases finies, on dit que $(\Phi(e_i, f_k))$ est la matrice de $\Phi$ par rapport à ces bases.

Les applications bilinéaires de $E \times F$ dans $G$ forment évidemment un sous-groupe du groupe additif des applications de $E \times F$ dans $G$. D’autre part soit $a$ (resp. $b$) un élément du centre de $A$ (resp. $B$) ; alors l’application $a \Phi b$ de $E \times F$ dans $G$ définie par $(a \Phi b)(x, y) = a . \Phi(x, y) . b$ est bilinéaire. L’ensemble des applications bilinéaires de $E \times F$ dans $G$ est ainsi muni d’une structure de bimodule sur les centres de $A$ et $B$.

Soient E' (resp. F') un A-module à gauche (resp. un B-module à droite), u (resp. v) un homomorphisme de E dans E' (resp. de F dans F') et $\Phi'$ une application bilinéaire de $E' \times F'$ dans G. On appelle *image réciproque* de $\Phi'$ (relativement à u et v) l’application bilinéaire $\Phi$ de $E \times F$ dans G définie par
$$
\Phi(x, y) = \Phi'(u(x), v(y)) \qquad (x \in E,\ y \in F).
$$
On vérifie aisément que l’on a
$$
d_{\Phi}(y) = d_{\Phi'}(v(y)) \circ u \qquad \text{et} \qquad s_{\Phi}(x) = s_{\Phi'}(u(x)) \circ v
$$
quels que soient $x \in E,\ y \in F$.

Soient $\Phi$ une application bilinéaire de $E \times F$ dans G, et h un homomorphisme (pour les structures de (A, B)-bimodules) de G dans un autre (A, B)-bimodule $G'$. Alors $h \circ \Phi$ est une application bilinéaire de $E \times F$ dans $G'$.

### 2. Applications sesquilinéaires.

Dans ce n° l’on désigne, sauf mention expresse du contraire, par A et B deux anneaux, par E un A-module à gauche et par F un B-module *à gauche* ; l’on désigne par $b \to b^J$ ($b \in B$) un *antiautomorphisme* de B, c’est-à-dire une bijection de B sur lui-même qui vérifie $(b + c)^J = b^J + c^J$ et $(bc)^J = c^J b^J$ quels que soient $b,\ c$ dans B ; on écrira $J'$ au lieu de $J^{-1}$. On désigne par G un (A, B)-bimodule (n° 1).

#### Définition 4 {#alg-ix-s1-def-4 .statement}

*On dit qu’une application $\Phi$ de $E \times F$ dans G est sesquilinéaire à droite pour J si elle satisfait aux conditions (1), (2), (3) (déf. 1, n° 1) ainsi qu’à*
(7) $\Phi(x, by) = \Phi(x, y) \cdot b^J$ quels que soient $x \in E,\ y \in F$ et $b \in B$.

Si J est l’identité (ce qui exige que B soit *commutatif*), on retrouve la notion d’application bilinéaire.

Soient $(e_i)_{i \in I}$ et $(f_k)_{k \in K}$ deux familles d’éléments de E et F, et soient $(a_i)_{i \in I}$ et $(b_k)_{k \in K}$ des éléments de A et B nuls à l’exception d’un nombre fini d’entre eux. On a alors
$$
\Phi(\sum_i a_i e_i, \sum_k b_k f_k) = \sum_{i,k} a_i \Phi(e_i, f_k) b_k^J.
$$

Comme dans le cas d’une application bilinéaire, les éléments $\Phi(e_i, f_k)$ déterminent $\Phi$ de façon unique lorsque $(e_i)$ et $(f_k)$ sont des systèmes de générateurs, et peuvent être pris arbitrairement lorsque $(e_i)$ et $(f_k)$ sont des bases de $E$ et $F$; lorsque $(e_i)$ et $(f_k)$ sont des bases finies, on dit que $(\Phi(e_i, f_k))$ est la matrice de $\Phi$ par rapport à ces bases.

Comme pour les applications bilinéaires, on définit sur l’ensemble des applications sesquilinéaires à droite (pour $J$) de $E \times F$ dans $G$ une structure de bimodule sur les centres de $A$ et $B$. On définit la notion d’image réciproque d’une application sesquilinéaire par la même formule que pour une application bilinéaire. Nous allons du reste voir que l’étude des applications sesquilinéaires peut se ramener à celle des applications bilinéaires.

#### Définition 5 {#alg-ix-s1-def-5 .statement}

Soient $B$ un anneau, $F$ un $B$-module à gauche (resp. à droite) et $J$ un antiautomorphisme de $B$. On désigne par $F^J$ le $B$-module à droite (resp. à gauche) ayant même groupe additif sous-jacent que $F$ et dans lequel la loi de composition externe est $(b, y) \to b^{J'}y$ (resp. $(b, y) \to yb^{J'}$) $(b \in B,\ y \in F,\ J' = J^{-1})$.

Avec les notations de la définition 5, une application linéaire de $F^J$ dans un $B$-module à droite (resp. à gauche) $H$ s’identifie donc à une application $\mathbf{Z}$-linéaire $u$ de $F$ dans $H$ vérifiant
$$
u(by) = u(y)b^J \quad \text{(resp. } u(yb) = b^Ju(y)) \quad (b \in B,\ y \in F).
$$

L’application $u$ de $F$ dans $H$ est une application semi-linéaire de $F$ dans $H$ relative à $J$ (chap. II, App. I, no 1), si l’on considère $J$ comme un isomorphisme de l’anneau $B^0$ opposé de $B$ sur $B$, et $F$ comme un $B^0$-module à droite (resp. à gauche).

De même une application sesquilinéaire à droite $\Phi$ (pour $J$) de $E \times F$ dans $G$, où $F$ est un $B$-module à gauche, s’identifie à une application bilinéaire de $E \times F^J$ dans $G$; si cette dernière est dégénérée à droite (resp. dégénérée à gauche, non dégénérée), on dit que $\Phi$ est dégénérée à droite (resp. dégénérée à gauche, non dégénérée).

#### Remarque {#alg-ix-s1-n2-rem-1 .statement}

Soient $A$ et $B$ deux anneaux, $J_1$ un antiautomorphisme de $A$, $M$ un $A$-module à droite, $N$ un $B$-module à droite et G un (A, B)-bimodule. On dit qu’une application $\Phi$ de $M \times N$ dans G est *sesquilinéaire à gauche pour $J_1$* si elle est $\mathbf{Z}$-bilinéaire et si elle vérifie

$$
\Phi(xa, yb) = a^{J_1} \Phi(x, y)b \quad (x \in M, y \in N, a \in A, b \in B).
$$

Une telle application s’identifie à une application bilinéaire de $M^{J_1} \times N$ dans G. Nous laisserons souvent au lecteur le soin de transposer aux applications sesquilinéaires à gauche les définitions et propriétés données pour les applications sesquilinéaires à droite ; lorsque nous parlerons d’application sesquilinéaire (sans préciser), il s’agira d’une application sesquilinéaire *à droite*.

### 3. Orthogonalité. Sommes directes d’applications bilinéaires ou sesquilinéaires.

Dans ce no , A et B désignent des anneaux, E un A-module à gauche, F un B-module à droite (resp. à gauche), G un (A, B)-bimodule, et $\Phi$ une application bilinéaire (resp. sesquilinéaire pour un antiautomorphisme donné J de B) de $E \times F$ dans G.

#### Définition 6 {#alg-ix-s1-def-6 .statement}

*Deux éléments $x \in E$ et $y \in F$ sont dits orthogonaux par rapport à $\Phi$ si $\Phi(x, y) = 0$. Deux parties $E' \subset E$ et $F' \subset F$ sont dites orthogonales si, quels que soient $x \in E'$ et $y \in F'$, $x$ et $y$ sont orthogonaux. L’ensemble des éléments de $E$ (resp. F) orthogonaux à un sous-module donné N de F (resp. M de E) est un sous-module de E (resp. F), qu’on appelle le sous-module totalement orthogonal (ou simplement orthogonal) à N (resp. M), et qu’on note $N^0$ (resp. $M^0$).

Soient H et $H'$ deux sous-modules de E ou de F. On a $H \subset (H^0)^0$ (que l’on note $H^{00}$) ; si $H \subset H'$, on a $H'^0 \supset H^0$. Il en résulte que l’on a $H^0 \supset (H^{00})^0$ et $H^0 \subset (H^0)^{00}$ ; en posant

$$
H^{000} = (H^{00})^0 = (H^0)^{00} = ((H^0)^0)^0,
$$

on a donc $H^0 = H^{000}$.

Pour que l’application $\Phi$ soit dégénérée (no 1, déf. 3) il faut et il suffit que l’un au moins des deux sous-modules $E^0, F^0$ soit $\neq \{0\}$. Il est clair que $\Phi(x, y)$ ne change pas lorsqu’on ajoute à $x$ (resp. $y$) un élément de $F^0$ (resp. $E^0$), et $\Phi$ définit donc par passage au quotient une application bilinéaire (ou sesquilinéaire) sur $(E/F^0) \times (F/E^0)$; celle-ci est visiblement non dégénérée; on l’appelle l’application bilinéaire (ou sesquilinéaire) non dégénérée associée à $\Phi$.

Soient $(E_i)_{i \in I}$ une famille de A-modules à gauche, $(F_i)_{i \in I}$ une famille de B-modules à droite (resp. à gauche), $\Phi_i$ une application bilinéaire (resp. sesquilinéaire à droite pour J) de $E_i \times F_i$ dans G. Notons $E$ (resp. $F$) le module somme directe des $E_i$ (resp. $F_i$). On voit aussitôt que l’application $\Phi$ de $E \times F$ dans G définie par
$$
\Phi((x_i), (y_i)) = \sum_i \Phi_i(x_i, y_i) \quad (x_i \in E_i, y_i \in F_i)
$$
(somme qui a un sens puisque ses termes sont nuls à l’exception d’un nombre fini d’entre eux) est bilinéaire (resp. sesquilinéaire à droite pour J). On l’appelle la somme directe des applications $\Phi_i$. Il est clair que $E_i$ est orthogonal à $F_j$ par rapport à $\Phi$ pour $i \neq j$. Réciproquement, soit $\Phi$ une application bilinéaire ou sesquilinéaire de $E \times F$ dans G, et supposons que E soit somme directe de sous-modules $(E_i)_{i \in I}$ et F somme directe de sous-modules $(F_i)_{i \in I}$ tels que $E_i$ soit orthogonal à $F_j$ pour $i \neq j$; alors $\Phi$ est la somme directe de ses restrictions aux produits $E_i \times F_i$ ($i \in I$).

Pour que $\Phi$ soit non dégénérée, il faut et il suffit que chacune des $\Phi_i$ le soit ; dans ces conditions, le sous-module orthogonal à $E_i$ est $\sum_{j \neq i} F_j$.

### 4. Changement d’anneaux de base.

Dans ce no, l’on désigne par A, B, A', B' quatre anneaux, par $h$ et $h'$ des homomorphismes de A dans A' et de B dans B' respectivement, par G un (A, B)-bimodule, par G' un (A', B')-bimodule, et par $u$ un homomorphisme du groupe abélien sous-jacent à G dans le groupe abélien sous-jacent à G', vérifiant
$$
u(agb) = h(a)u(g)h'(b) \quad (a \in A, g \in G, b \in B).
$$

Soit E (resp. F) un A-module à gauche (resp. un B-module à droite). Rappelons (Chap. III, 2e éd., App. II, no 10) que, si l’on considère $A'$ (resp. $B'$) comme un $A$-module à droite (resp. $B$-module à gauche), le produit tensoriel $E' = A' \otimes_A E$ (resp. $F' = F \otimes_B B'$) est muni d’une structure de $A'$-module à gauche (resp. $B'$-module à droite) définie par

$$
a'_1(a' \otimes x) = (a'_1 a') \otimes x \quad (a', a'_1 \in A', x \in E)
$$
(resp. $(y \otimes b') b'_1 = y \otimes (b' b'_1)$ $(b', b'_1 \in B', y \in F)$).

#### Proposition 1 {#alg-ix-s1-prop-1 .statement}

*Soient $E$ un $A$-module à gauche et $F$ un $B$-module à droite ; posons $E' = A' \otimes_A E$ et $F' = F \otimes_B B'$. Pour toute application bilinéaire $\Phi$ de $E \times F$ dans $G$, il existe une application bilinéaire $\Phi'$ et une seule de $E' \times F'$ dans $G'$ telle que l’on ait*

$$
\Phi'(a' \otimes x, y \otimes b') = a'.u(\Phi(x, y)).b'
$$

quels que soient $a' \in A'$, $b' \in B'$, $x \in E$, $y \in F$.

L’unicité de $\Phi'$ résulte du fait que les éléments $a' \otimes x$ et $y \otimes b'$ engendrent $E'$ et $F'$ respectivement. Pour en démontrer l’existence, considérons l’application

$$
m : (a', x, y, b') \to a'.u(\Phi(x, y)).b'
$$

de $A' \times E \times F \times B'$ dans $G$; elle est évidemment $\mathbf{Z}$-multilinéaire, et elle vérifie

$$
m(a', ax, y, b') = m(a'h(a), x, y, b')
$$
et
$$
m(a', x, yb, b') = m(a', x, y, h'(b)b')
$$
$(a \in A, b \in B, a' \in A', b' \in B', x \in E, y \in F)$.

Il existe donc une application $\mathbf{Z}$-bilinéaire $\Phi'$ de $E' \times F'$ dans $G'$ vérifiant (13) (Chap. III, 2e éd., App. II, n° 1, prop. 2). Cette relation et la définition des structures de modules de $E'$ et $F'$ par (12) montrent que $\Phi'$ est bilinéaire, ce qui termine la démonstration.

Les hypothèses et notations étant celles de la proposition 1, étudions maintenant les *applications linéaires associées* à $\Phi$ et à $\Phi'$ (n° 1, déf. 2). Pour cela nous allons d’abord définir un homomorphisme canonique de $\mathcal{L}_A(E, G)$ dans $\mathcal{L}_{A'}(E', G')$. Pour tout $\nu \in \mathcal{L}_A(E, G)$ l’application $(a', x) \to a'.u(\nu(x))$ de $A' \times E$ dans $G'$ est $\mathbf{Z}$-bilinéaire, et, vu (11), applique $(a'h(a), x)$ et $(a', ax)$ $(a \in A)$ sur le même élément de $G'$; elle définit donc (chap. III, 2e éd.,

App. II, n°s 1 et 10) une application $k(\nu)$ de $E' = A' \otimes_A E$ dans $G'$ telle que $k(\nu)(a' \otimes x) = a'.u(\nu(x))$, et qui, vu (12), est $A'$-linéaire. En outre l’on déduit immédiatement de (12) que l’application $\nu \to k(\nu)$ de $\mathcal{L}_A(E, G)$ dans $\mathcal{L}_{A'}(E', G')$ vérifie $k(\nu b) = k(\nu)h'(b)$ pour tout $b \in B$. Notons $i$ l’application canonique $y \to y \otimes 1$ de $F$ dans $F'$. Alors le diagramme

$$
\begin{array}{ccc}
F & \xrightarrow{d_\Phi} & \mathcal{L}_A(E, G) \\
|_i & & |_k \\
F' & \xrightarrow{d_{\Phi'}} & \mathcal{L}_{A'}(E', G')
\end{array}
$$

(où $d_\Phi$ et $d_{\Phi'}$ désignent les applications linéaires associées à droite à $\Phi$ et $\Phi'$) est *commutatif*. En effet, pour $x \in E, y \in F$ et $a' \in A'$, on a $d_{\Phi'}(i(y))(a' \otimes x) = \Phi'(a' \otimes x, y \otimes 1) = a'.u(\Phi(x, y)) = a'.u(d_\Phi(y)(x))$, c’est-à-dire $d_{\Phi'}(i(y))(a' \otimes x) = k(d_\Phi(y))(a' \otimes x)$. On a une relation de commutation analogue pour les applications linéaires $s_\Phi$ et $s_{\Phi'}$ associées à gauche à $\Phi$ et $\Phi'$.

#### Proposition 2 {#alg-ix-s1-prop-2 .statement}

*Supposons que B et B' soient munis d’anti-automorphismes J et I tels que*

$$(15)$$
$$ h'(b^J) = h'(b)^I \quad \text{pour tout } b \in B. $$

*Soient E un A-module à gauche et F un B-module à gauche ; posons $E' = A' \otimes_A E$ et $F' = B' \otimes_B F$. Pour toute application sesquilinéaire (pour J) $\Phi$ de $E \times F$ dans $G$, il existe une application sesquilinéaire (pour I) $\Phi'$ et une seule de $E' \times F'$ dans $G'$ telle que*

$$(16)$$
$$ \Phi'(a' \otimes x, b' \otimes y) = a'.u(\Phi(x, y)).b'^I $$

*quels que soient $a' \in A'$, $b' \in B'$, $x \in E$, $y \in F$.*

L’unicité de $\Phi'$ résulte du fait que les produits tensoriels $a' \otimes x$ et $b' \otimes y$ engendrent $E'$ et $F'$ respectivement. Pour en établir l’existence, considérons l’application

$$ m : (a, x, b', y) \to a'.u(\Phi(x, y)).b'^I $$

de $A' \times E \times B' \times F$ dans $G'$. Elle est évidemment $\mathbf{Z}$-multilinéaire, et, compte tenu de (11) et (15), vérifie $m(a', ax, b', y) = m(a'h(a), x, b', y)$ et $m(a', x, b', by) = a'.u(\Phi(x, y)).h'(b^J)b'^I = m(a', x, b'h'(b), y)$ ($a \in A, b \in B, a' \in A', b' \in B', x \in E, y \in F$). Il existe donc une application $\mathbf{Z}$-bilinéaire $\Phi'$ de $E' \times F'$ dans $G'$ vérifiant (16) (chap. III, 2e éd., App. II, no 1, prop. 2). Cette relation, ainsi que la définition des structures de modules de E' et F' par (12), montrent, compte tenu de (15), que $\Phi'$ est sesquilinéaire pour I, ce qui achève la démonstration.

Les exemples les plus importants de (A', B')-bimodules G', munis d’applications $\mathbf{Z}$-linéaires $u$ de G dans G' vérifiant (11), sont les suivants :

1) On prend pour G' le produit tensoriel $A' \otimes_A G \otimes_B B'$ (chap. III, 2e éd., App. II, no 9) et pour $u$ l’application
$$
g \to 1 \otimes g \otimes 1 \qquad (g \in G)
$$
de G dans G'. Le couple $(G', u)$ ainsi défini est visiblement *universel* dans le sens suivant : pour tout (A', B')-bimodule $G'_1$ et toute application $\mathbf{Z}$-linéaire $u_1$ de G dans $G'_1$ vérifiant l’analogue de (11), il existe une application $\mathbf{Z}$-linéaire $f$ et une seule de G' dans $G'_1$ telle que $f(a'g'b') = a'f(g')b'$ ($a' \in A'$, $g' \in G'$, $b' \in B'$; autrement dit $f$ est un homomorphisme pour les structures de bimodules de G' et $G'_1$) et que $u_1 = f \circ u$.

2) Lorsque $A = B = G$ (la structure de (A, A)-bimodule de A étant définie par les homothéties à gauche et à droite), $A' = B'$, et $h = h'$ on peut prendre pour G' l’anneau $A'$ et pour $u$ l’homomorphisme $h$ de A dans $A'$.

3) Supposons que l’on ait $A = B$, $A' = B'$, $h = h'$, que les anneaux A et A' soient *commutatifs*, et que la structure de A-module à gauche de G coïncide avec sa structure de A-module à droite. On peut alors prendre pour G' le produit tensoriel $A' \otimes_A G$ (la structure de A'-module à droite de G' coïncidant avec sa structure de A'-module à gauche) et pour $u$ l’application $g \to 1 \otimes g$ ($g \in G$) de G dans G'. Nous dirons alors que l’application bilinéaire (resp. sesquilinéaire) $\Phi'$ définie par la prop. 1 (resp. prop. 2) est obtenue à partir de $\Phi$ *par extension de l’anneau de base*, ou *par extension des scalaires*.

Ce qui suit est valable aussi bien pour les applications bilinéaires que pour les applications sesquilinéaires ; les hypothèses et notations sont celles de la prop. 1 (resp. prop. 2). Étant donné un sous-module M de E ou F, on désignera par M' le sous-module de E' ou F' engendré par l’image canonique de M.

#### Proposition 3 {#alg-ix-s1-prop-3 .statement}

Les hypothèses et notations étant celles de la prop. 1 (resp. prop. 2) supposons de plus que A, B, A', B' soient des corps et que les applications α et β de A' ⊗_A G et G ⊗_B B' dans G' caractérisées par $\alpha(a' \otimes g) = a'u(g)$ et $\beta(g \otimes b') = u(g)b'$ ($a' \in A'$, $b' \in B'$, $g \in G$) soient injectives. Soient M un sous-espace de E et N un sous-espace de F. Alors le sous-espace $(M')^0$ de F' orthogonal à M' par rapport à $\Phi'$ est égal à $(M^0)',$ et, de même, on a $(N')^0 = (N^0)'.$

En effet les inclusions $(M^0)' \subset (M')^0$ et $(N^0)' \subset (N')^0$ sont évidentes (et d’ailleurs vraies sans hypothèses sur A, B, A', B', $\alpha$ ni $\beta$). Nous allons démontrer l’inclusion $(M')^0 \subset (M^0)'$; nous laissons au lecteur la vérification de l’inclusion $(N')^0 \subset (N^0)',$ qui est tout à fait analogue. Soit $y'$ un élément de $(M')^0$. On peut écrire

$$
y' = \sum_{i=1}^s y_i \otimes b'_i \quad \text{(resp. } y' = \sum_{i=1}^s b'_i \otimes y_i)
$$

où $y_i \in F$ ($1 \leq i \leq s$), et où les $b'_i$ sont des éléments de B' qui sont linéairement indépendants sur B pour la structure de B-module à gauche (resp. à droite) de B'. Soient $x \in M$ et $x' = 1 \otimes x \in M'$. On a

$$
0 = \Phi'(x', y') = \sum_i u(\Phi(x, y_i)) b'_i = \beta(\sum_i \Phi(x, y_i) \otimes b'_i)
$$
(resp. $0 = \Phi'(x', y') = \sum_i u(\Phi(x, y_i)) b'^I_i = \beta(\sum_i \Phi(x, y_i) \otimes b'^I_i)$.

Comme $\beta$ est injective et que les $b'_i$ (resp. les $b'^I_i$, compte tenu de (15)) sont linéairement indépendants sur B pour la structure de B-module à gauche de B', ceci entraîne $\Phi(x, y_i) = 0$ pour $i = 1, \ldots, s$. Comme cette dernière relation est vraie pour tout $x \in M$, on a $y_i \in M^0$ pour $i = 1, \ldots, s$, d’où $y' \in (M^0)'$. CQFD.

#### Corollaire {#alg-ix-s1-n4-cor-1 .statement}

Les hypothèses et notations étant celles de la prop. 3, pour que $\Phi'$ soit non dégénérée, il faut et il suffit que $\Phi$ soit non dégénérée.

En effet, d’après la prop. 3, on a $(F')^0 = (F^0)'$ et $(E')^0 = (E^0)'$. D’autre part, pour que $\Phi$ (resp. $\Phi'$) soit non dégénérée, il faut et il suffit que l’on ait $F^0 = E^0 = \{0\}$ (resp. $(F')^0 = (E')^0 = \{0\}$).

#### Remarque {#alg-ix-s1-n4-rem-1 .statement}

Supposons que A, B, A' et B' soient des corps. Alors, pour les bimodules G' définis dans les trois exemples ci-dessus, les applications $\alpha$ et $\beta$ sont injectives, comme il résulte aussitôt du chap. III, 2e éd., App. II, n° 6.

### 5. Quelques identités.

Dans ce n°, l’on désigne par A un anneau muni d’un antiautomorphisme J, par E un A-module à gauche, par G un (A, A)-bimodule, et par $\Phi$ une application sesquilinéaire (à droite) pour J de $E \times E$ dans G. On pose $Q(x) = \Phi(x, x)$ ($x \in E$). On a évidemment

$$
\begin{align*}
(17) \quad & Q(x + y) = Q(x) + \Phi(x, y) + \Phi(y, x) + Q(y) \\
(18) \quad & Q(x - y) = Q(x) - \Phi(x, y) - \Phi(y, x) + Q(y)
\end{align*}
$$

quels que soient $x, y$ dans E. D’où, par soustraction,

$$
(19) \quad 2(\Phi(x, y) + \Phi(y, x)) = Q(x + y) - Q(x - y).
$$

Soit $a$ un élément de A ; en remplaçant $y$ par $ay$ dans (19), il vient

$$
(20) \quad 2(\Phi(x, y)a^j + a\Phi(y, x)) = Q(x + ay) - Q(x - ay).
$$

On tire de (19) et (20), en multipliant (19) par $a$ (à gauche) et en soustrayant :

$$
\begin{align*}
(21) \quad & 2(a\Phi(x, y) - \Phi(x, y)a^j) \\
& \quad = aQ(x + y) - aQ(x - y) - Q(x + ay) + Q(x - ay).
\end{align*}
$$

Supposons en particulier que A soit une extension quadratique $K(i)$ d’un anneau commutatif K, avec $i^2 = -1$ (chap. II, § 7, n° 7), que J soit le K-automorphisme $u + iv \to u - iv$ ($u, v$ dans K) de A, et que les structures de A-module à gauche et de A-module à droite de G coïncident. En faisant $a = i$ dans (21), on obtient

$$
(22) \quad 4\Phi(x, y) = Q(x + y) - Q(x - y) + iQ(x + iy) - iQ(x - iy).
$$

### 6. Formes bilinéaires et sesquilinéaires. Rang.

Dans ce n°, l’on désigne par A un anneau (resp. un anneau muni d’un antiautomorphisme J), par E un A-module à gauche, et par F un A-module à droite (resp. à gauche). On munit A de la structure de (A, A)-bimodule définie par les homothéties à gauche et les homothéties à droite. Dans ce cas une application bilinéaire (resp. sesquilinéaire à droite pour J) de E × F dans le bimodule A s’appelle une forme bilinéaire (resp. sesquilinéaire à droite pour J) sur E × F.

Lorsque E = F (ce qui implique qu’il s’agit d’une forme sesquilinéaire), on dit souvent qu’une forme sesquilinéaire sur E × F est une forme sesquilinéaire sur E.

Étant donnés deux A-modules à gauche E et E′, et deux formes Φ et Φ′ sesquilinéaires pour J sur E et E′ respectivement, on dit que Φ et Φ′ sont équivalentes s’il existe un isomorphisme u du A-module E sur le A-module E′ tel que Φ′(u(x), u(y)) = Φ(x, y) quels que soient x, y dans E ; alors Φ est l’image réciproque de Φ′ relativement à u et u, et Φ′ est l’image réciproque de Φ relativement à u^{-1} et u^{-1} (n° 2).

Soit Φ une forme bilinéaire sur E × F (F désignant un A-module à droite). Les applications linéaires s_{Φ} et d_{Φ} associées à Φ (n° 1, déf. 2) sont alors des applications de E dans le dual F* de F, et de F dans le dual E* de E.

On a donc par définition

$$
\Phi(x, y) = \langle x, d_{Φ}(y) \rangle = \langle y, s_{Φ}(x) \rangle.
$$

Nous allons maintenant définir les applications linéaires associées à une forme sesquilinéaire. Soient J un antiautomorphisme de A et Φ une forme sesquilinéaire (à droite) pour J sur E × F (F désignant un A-module à gauche) ; posons J′ = J^{-1}. L’application Φ′ de F × E dans A définie par

$$
Φ′(y, x) = Φ(x, y)^{J′} \quad (x ∈ E, y ∈ F)
$$

est, comme on le voit facilement, une forme sesquilinéaire (à droite) pour J′ sur F × E. D’après le n° 2 (dēf. 5) les formes sesquilinéaires Φ et Φ′ s’identifient respectivement à des formes bilinéaires sur E × F^{J′} et sur F × E^{J′}. Les applications d_{Φ} et d_{Φ′} associées à ces dernières sont appelées les applications associées à droite et à gauche à la forme sesquilinéaire $\Phi$, et sont notées $d_\Phi$ et $s_\Phi$. On a donc, par définition :

$$
(24)\quad \Phi(x, y) = \langle x, d_\Phi(y) \rangle = \langle y, s_\Phi(x) \rangle^J \qquad (x \in E,\ y \in F).
$$

Ainsi $d_\Phi$ (resp. $s_\Phi$) est une application linéaire de $F^J$ dans $E^*$ (resp. de $E^{J'}$ dans $F^*$), ou encore une application semi-linéaire de $F$ dans $E^*$ (resp. de $E$ dans $F^*$) relative à $J$ (resp. $J'$) si l’on considère $J$ (resp. $J'$) comme un isomorphisme de l’anneau $A^0$ (opposé de $A$) sur $A$, et $F$ (resp. $E$) comme un $A^0$-module à droite.

La formule (24) et la déf. 6 du no 3 entraînent aussitôt que pour tout sous-module $N$ de $F$ (resp. $M$ de $E$), on a

$$
(25)\quad N^0 = s_\Phi^{-1}(N') \qquad (\text{resp. } M^0 = d_\Phi^{-1}(M'))
$$

où $N'$ (resp. $M'$) est le sous-module du dual $F^*$ de $F$ (resp. du dual $E^*$ de $E$) orthogonal à $N$ (resp. $M$) (chap. II, § 4, no 2).

#### Proposition 4 {#alg-ix-s1-prop-4 .statement}

*Supposons que $A$ soit un corps, et soit $\Phi$ une forme bilinéaire (resp. sesquilinéaire pour $J$) sur $E \times F$; pour que $E/F^0$ soit de dimension finie, il faut et il suffit que $F/E^0$ soit de dimension finie, et ces dimensions sont alors égales.*

En effet, soit $\Phi_1$ la forme non dégénérée associée à $\Phi$, sur $(E/F^0) \times (F/E^0)$ (no 3). Supposons que $E/F^0$ soit de dimension finie $n$; comme l’application linéaire $d_{\Phi_1}$ de $F/E^0$ (resp. $(F/E^0)^J$) dans $(E/F^0)^*$ est injective, $F/E^0$ est de dimension finie $n' \leq n$; en considérant $s_{\Phi_1}$, on voit de même que $n \leq n'$.

#### Corollaire 1 {#alg-ix-s1-prop-4-cor-1 .statement}

*On suppose que $A$ est un corps et que $\Phi$ est non dégénérée. Pour qu’un sous-espace $M$ de $E$ soit de dimension finie, il faut et il suffit que $M^0$ soit de codimension finie dans $F$, et on a alors $\operatorname{codim} M^0 = \dim M$, et $M^{00} = M$.*

Comme $F^0 = \{0\}$, les deux premières assertions résultent de la prop. 4 appliquée à la restriction de $\Phi$ à $M \times F$. En outre, $M^0$ est l’orthogonal de $M^{00}$, donc $M^{00}$ est de dimension finie égale à $\operatorname{codim} M^0 = \dim M$; mais comme $M^{00} \supset M$, on a $M^{00} = M$.

#### Corollaire 2 {#alg-ix-s1-prop-4-cor-2 .statement}

*Les hypothèses étant celles du cor. 1, soient $M, N$ deux sous-espaces de $E$; on a alors $(M + N)^0 = M^0 \cap N^0$; si de plus $M$ et $N$ sont de dimension finie, on a $(M \cap N)^0 = M^0 + N^0$.*

La première assertion est triviale. Supposons M et N de dimension finie, et soit G = M^0 + N^0 ; on a G^0 = M^{00} \cap N^{00} = M \cap N d’après le cor. 1 ; la prop. 4 appliquée à la restriction de $\Phi$ à $M \times G$ montre alors (puisque $M^0 \subset G$ et $G^0 \subset M$) que l’on a $\dim M/(M \cap N) = \dim G/M^0 = \operatorname{codim} M^0 - \operatorname{codim} G$, et comme $\operatorname{codim} M^0 = \dim M$, on en déduit $\dim (M \cap N) = \operatorname{codim} G$. Mais on a aussi $\dim (M \cap N) = \operatorname{codim} (M \cap N)^0$ d’après le cor. 1, et comme $G \subset G^{00} = (M \cap N)^0$ on a $G = (M \cap N)^0$.

La prop. 4 permet de poser la définition suivante :

#### Définition 7 {#alg-ix-s1-def-7 .statement}

Soient A un corps (resp. un corps muni d’un antiautomorphisme J), E un espace vectoriel à gauche sur A, F un espace vectoriel à droite (resp. à gauche) sur A, et $\Phi$ une forme bilinéaire (resp. sesquilinéaire pour J) sur $E \times F$. Supposons que $E/F^0$ et $F/E^0$ soient de dimension finie sur A. On appelle rang de $\Phi$ la dimension (finie) commune des espaces vectoriels $E/F^0$ et $F/E^0$.

Lorsque $E/F^0$ et $F/E^0$ sont de dimension infinie, on dit que $\Phi$ est de rang infini.

#### Proposition 5 {#alg-ix-s1-prop-5 .statement}

Les hypothèses et notations étant celles de la déf. 7, les applications linéaires $s_\Phi$ et $d_\Phi$ associées à $\Phi$ ont même rang, et ce rang est égal au rang de la forme $\Phi$.

En effet le noyau de l’application $d_\Phi$ de F dans $E^*$ est évidemment $E^0$, donc son rang est égal à la dimension de $F/E^0$. De même le rang de $s_\Phi$ est égal à la dimension de $E/F^0$.

#### Proposition 6 {#alg-ix-s1-prop-6 .statement}

Les hypothèses et notations étant celles de la déf. 7, supposons de plus que E et F aient même dimension finie. Alors les conditions suivantes sont équivalentes :
a) $d_\Phi$ est injective ;
b) $d_\Phi$ est surjective ;
c) $s_\Phi$ est injective ;
d) $s_\Phi$ est surjective ;
e) $\Phi$ est non dégénérée.

En effet, comme E, F, $E^*$ et $F^*$ ont même dimension finie,

a) et b) sont équivalentes, ainsi que c) et d) (chap. II, § 3, no 4). Comme $s_\Phi$ et $d_\Phi$ ont même rang (prop. 5), a) et c) sont équivalentes. Comme e) équivaut à la relation $E^0 = F^0 = \{0\}$, elle équivaut à la conjonction de a) et c), d’où l’équivalence des conditions énoncées.

#### Corollaire {#alg-ix-s1-n6-cor-1 .statement}

Les hypothèses et notations étant celles de la déf. 7, on suppose de plus que E est de dimension finie et que $\Phi$ est non dégénérée. Alors on a $\dim E = \dim F$ et, pour toute base $(e_i)$ ($1 \leq i \leq \dim E$) de E, il existe une base $(f_i)$ de F telle que $\Phi(e_i, f_k) = \delta_{ik}$ ($i, k = 1, ..., \dim E$).

En effet, comme $\Phi$ est non dégénérée, on a $E^0 = F^0 = \{0\}$, d’où $\dim E = \dim F$ (prop. 4). Il s’ensuit (prop. 6) que $d_\Phi$ est un isomorphisme de F (resp. $F^j$) sur $E^*$; donc, si $(e_i^*)$ est la base duale de $(e_i)$, les éléments $f_i = d_\Phi^{-1}(e_i^*)$ forment une base de F qui, vu la formule (23) (resp. la formule (24)), vérifie $\Phi(e_i, f_k) = \delta_{ik}$.

Il est immédiat que, dans ce corollaire, on peut échanger les rôles de E et de F, en remplaçant $d_\Phi$ par $s_\Phi$ dans la démonstration.

#### Remarque {#alg-ix-s1-n6-rem-1 .statement}

Soient A un anneau muni d’un antiautomorphisme J, M et N des A-modules à droite, et $\Phi$ une forme sesquilinéaire à gauche pour J sur $M \times N$ (no 2, Remarque) ; elle vérifie donc l’égalité

$$
\Phi(xa, xa') = a^j \Phi(x, y)a' \quad (a, a' \in A, x \in M, y \in N).
$$

L’application $\Phi'$ de $N \times M$ dans A définie par $\Phi'(y, x) = \Phi(x, y)^{J'}$ (où $J' = J^{-1}$) est une forme sesquilinéaire à gauche pour $J'$, et $\Phi$ et $\Phi'$ s’identifient à des formes bilinéaires sur $M^{J'} \times N$ et $N^{J'} \times M$ respectivement. Les applications $s_\Phi$ et $s_{\Phi'}$ associées à ces formes bilinéaires sont appelées les applications associées à gauche et à droite à la forme sesquilinéaire $\Phi$, et sont notées $s_\Phi$ et $d_\Phi$. On a donc, par définition

$$(26)$$
$$
\Phi(x, y) = \langle y, s_\Phi(x) \rangle = \langle x, d_\Phi(y) \rangle^j \quad (x \in M, y \in N),
$$

et $s_\Phi$ (resp. $d_\Phi$) est une application linéaire de $M^{J'}$ dans $N^*$ (resp.

de $N'$ dans $M^*$). On énoncerait et démontrerait facilement les analogues, pour le cas envisagé ici, de la déf. 7 et des prop. 4, 5, 6.

### 7. Forme inverse d’une forme bilinéaire ou sesquilinéaire.

Soient $A$ un anneau, $E$ un $A$-module à gauche, $F$ un $A$-module à droite et $\Phi$ une forme bilinéaire sur $E \times F$. On suppose ici que les applications associées à $\Phi$, qui seront notées $s$ et $d$, sont *bijectives*. Alors l’application produit $(s, d)$ est une bijection de $E \times F$ sur $F^* \times E^*$, et définit, par transport de structure, une forme bilinéaire $\hat{\Phi}$ sur $F^* \times E^*$. Celle-ci vérifie donc

$$
(27)\quad \hat{\Phi}(y', x') = \Phi(s^{-1}(y'), d^{-1}(x')) \\
= \langle s^{-1}(y'), x' \rangle = \langle d^{-1}(x'), y' \rangle \qquad (x' \in E^*, y' \in F^*).
$$

#### Définition 8 {#alg-ix-s1-def-8 .statement}

*Soit $\Phi$ une forme bilinéaire sur $E \times F$ dont les applications associées $s$ et $d$ sont bijectives. La forme bilinéaire $\hat{\Phi}$ sur $F^* \times E^*$ définie par (27) s’appelle la forme inverse de $\Phi$.*

Soient maintenant $\hat{s}$ et $\hat{d}$ les applications linéaires de $F^*$ dans $E^{**}$ et de $E^*$ dans $F^{**}$ associées à gauche et à droite à $\hat{\Phi}$. Comme, pour $x' \in E^*$ et $y' \in F^*$, on a par définition

$$
\hat{\Phi}(y', x') = \langle y', \hat{d}(x') \rangle = \langle x', \hat{s}(y') \rangle
$$

on voit, en comparant avec (27), que la forme linéaire $\hat{d}(x')$ sur $F^*$ est égale à celle définie par l’élément $d^{-1}(x')$ de $F$. Il en résulte que l’application composée $\hat{d} \circ d$ est l’application canonique de $F$ dans son bidual $F^{**}$, et que celle-ci est *bijective* puisque $d$ et $\hat{d}$ (cette dernière par transport de structure) sont bijectives ; donc, si l’on identifie canoniquement $F$ à $F^{**}$, on a $\hat{d} = d^{-1}$. De même $E$ s’identifie canoniquement à $E^{**}$, l’application canonique de $E$ dans $E^{**}$ est $\hat{s} \circ s$, et l’on a $\hat{s} = s^{-1}$. Il résulte de ceci que la forme inverse de $\hat{\Phi}$ est $\Phi$.

Considérons maintenant un anneau $A$ muni d’un antiautomorphisme $J$, deux $A$-modules à gauche $E$ et $F$, et une forme sesquilinéaire à droite $\Phi$ pour $J$ sur $E \times F$ telle que les applications associées à $\Phi$, qui seront notées $s$ et $d$, soient *bijectives*. Définissons une application $\widehat{\Phi}$ de $F^* \times E^*$ dans $A$ par la première équation (27). Cette application vérifie, d’après (24) (n° 6), la relation

$$
(28)\quad \widehat{\Phi}(y', x') = \langle s^{-1}(y'), x' \rangle = \langle d^{-1}(x'), y' \rangle^J \qquad (x' \in E^*,\ y' \in F^*).
$$

L’application $\widehat{\Phi}$ est évidemment $\mathbf{Z}$-bilinéaire ; en outre, on a, pour $a,\ b$ dans $A$, $x' \in E^*$ et $y' \in F^*$, et en vertu des définitions de $s$ et $d$,

$$
\widehat{\Phi}(y'a,\ x'b) = \Phi(a^j s^{-1}(y'),\ b^{j'} d^{-1}(x')) = a^j \widehat{\Phi}(y',\ x') b;
$$

donc $\widehat{\Phi}$ est une *forme sesquilinéaire à gauche* pour $J$ (n° 2) sur $F^* \times E^*$.

#### Définition 9 {#alg-ix-s1-def-9 .statement}

*Soit $\Phi$ une forme sesquilinéaire à droite pour $J$ sur $E \times F$, dont les applications associées $s$ et $d$ sont bijectives. La forme sesquilinéaire à gauche $\widehat{\Phi}$ pour $J$ sur $F^* \times E^*$ s’appelle la forme inverse de $\Phi$.*

Nous laissons au lecteur le soin de définir et d’étudier la forme inverse d’une forme sesquilinéaire à gauche. Cette forme inverse est une forme sesquilinéaire à droite.

Soient $\widehat{s}$ et $\widehat{d}$ les applications associées à $\widehat{\Phi}$ ; d’après (26) (n° 6) on a

$$
(29)\quad \widehat{\Phi}(y', x') = \langle y',\ \widehat{d}(x') \rangle^J = \langle x',\ \widehat{s}(y') \rangle.
$$

Du fait que $s$ est bijective, et de l’égalité $\langle s^{-1}(y'),\ x' \rangle = \langle y',\ \widehat{d}(x') \rangle^J$ qui résulte de (28) et (29), on déduit que $\widehat{d}$ est bijective ; donc $\widehat{d} \circ d$ est bijective. Or l’égalité $\langle d^{-1}(x'),\ y' \rangle = \langle y',\ \widehat{d}(x') \rangle$, qui résulte de (28) et (29), montre que $\widehat{d} \circ d$ est l’application canonique de $F$ dans son bidual $F^{**}$. On voit de même que $\widehat{s}$ est bijective et que $\widehat{s} \circ s$ est l’application canonique de $E$ dans $E^{**}$. Donc, si l’on identifie $E^{**}$ à $E$ et $F^{**}$ à $F$ au moyen de ces applications canoniques, on a $\widehat{s} = s^{-1},\ \widehat{d} = d^{-1}$, et $\Phi$ est la forme inverse de $\widehat{\Phi}$.

Avec les mêmes notations et hypothèses soit $a$ un élément inversible du centre de $A$. Alors les applications associées à la forme $a\Phi$ sont, d’après (23) (resp. (24)) égales à $a.d$ et $a.s$ (resp. $a^{J'}.s$), donc sont bijectives. Il résulte ainsi de (27) que la forme inverse de $a\Phi$ est $a^{-1}\widehat{\Phi}$ (resp. $(a^{J'})^{-1}\widehat{\Phi}$).

### 8. Adjoint d’un homomorphisme.

Dans ce n°, l’on désigne par A un anneau (resp. un anneau muni d’un antiautomorphisme J), par E et E’ deux A-modules à gauche, par F et F’ deux A-modules à droite (resp. à gauche), et par $\Phi$ et $\Phi'$ deux formes bilinéaires (resp. sesquilinéaires pour J) sur $E \times F$ et $E' \times F'$ respectivement. On suppose que $\Phi$ est non dégénérée, autrement dit (n° 1) que les applications linéaires $d_{\Phi}$ et $s_{\Phi}$ associées à $\Phi$ sont injectives.

Étant donné un homomorphisme $u$ de E dans E’, considérons l’ensemble $F'_1$ des éléments $y'$ de $F'$ tels qu’il existe $y \in F$ pour lequel on ait $d_{\Phi'}(y') \circ u = d_{\Phi}(y)$, c’est-à-dire $\Phi'(u(x), y') = \Phi(x, y)$ pour tout $x \in E$. Il est clair que $F'_1$ est un sous-module de $F'$. Comme $d_{\Phi}$ est injective, il existe, pour tout $y' \in F'_1$, un élément $y$ de F et un seul tel que $\Phi'(u(x), y') = \Phi(x, y)$. L’application $y' \to y$ de $F'_1$ dans F ainsi définie est A-linéaire ; en la notant $u^*$, on a, pour tout $x \in E$ et tout $y \in F'_1$

$$
\Phi'(u(x), y') = \Phi(x, u^*(y')).
$$

#### Définition 10 {#alg-ix-s1-def-10 .statement}

Les hypothèses et notations étant comme précédemment, on dit que l’homomorphisme $u^*$ de $F'_1$ dans F vérifiant (30) est l’adjoint à gauche de $u$, et que $F'_1$ est le sous-module de définition de $u^*$.

On définit de même l’adjoint à droite d’un homomorphisme $\varphi$ de F dans $F'$ par la formule

$$
\Phi'(x', \varphi(y)) = \Phi(\varphi^*(x'), y) \quad (x' \in E'_1, y \in F),
$$

où $E'_1$ désigne le sous-module de $E'$ défini de façon analogue à $F'_1$.

#### Remarque {#alg-ix-s1-n8-rem-1 .statement}

Si l’adjoint à gauche $u^*$ de $u : E \to E'$ est partout défini, et si $s_{\Phi'}$ et $d_{\Phi'}$ sont injectives, la formule (30) montre que $u$ est l’adjoinat à droite de $u^*$.

On déduit de (30) que, si $u_1$ et $u_2$ sont deux homomorphismes de $E$ dans $E'$ admettant des adjoints partout définis, et si $c$ est un élément du centre de $A$, on a

$$
\begin{cases}
(u_1 + u_2)^* = u_1^* + u_2^* ; 1^* = 1 ; \\
(cu_1)^* = c . u_1^* \text{ lorsque } \Phi \text{ et } \Phi' \text{ sont bilinéaires ;} \\
(cu_1)^* = c^{j'} . u_1^* \text{ lorsque } \Phi \text{ et } \Phi' \text{ sont sesquilinéaires.}
\end{cases}
$$

De plus, si $E''$ est un troisième $A$-module à gauche, $F''$ un troisième $A$-module à droite (resp. à gauche), $\Phi''$ une forme bilinéaire (resp. sesquilinéaire pour $J$) sur $E'' \times F''$, et si $u'$ est un homomorphisme de $E'$ dans $E''$ admettant un adjoint (à gauche) partout défini, on a

$$(u' \circ u)^* = u^* \circ u'^*.$$

En particulier, si $u$ est un *isomorphisme* de $E$ sur $E'$, et si les adjoints $u^*$ et $(u^{-1})^*$ sont partout définis, $u^*$ est un isomorphisme de $F'$ sur $F$, et l’on a $(u^*)^{-1} = (u^{-1})^*$. Propriétés analogues pour les adjoints à droite.

#### Proposition 7 {#alg-ix-s1-prop-7 .statement}

Avec les mêmes notations que précédemment, on suppose que $d_{\Phi}$ est bijective. Alors tout homomorphisme $u$ de $E$ dans $E'$ admet un adjoint à gauche partout défini, et l’on a $u^* = (d_{\Phi})^{-1} \circ {}^t u \circ d_{\Phi'}$.

En effet, comme $d_{\Phi}$ est bijective, on a, avec les notations du début du no, $F'_1 = F'$, et $u^*$ est donc partout défini. D’autre part (30) équivaut à

$$\langle u(x), d_{\Phi'}(y') \rangle = \langle x, (d_{\Phi} \circ u^*)(y') \rangle \quad (x \in E, y' \in F');$$

or $\langle d_{\Phi'}(y'), u(x) \rangle = \langle {}^t u(d_{\Phi'}(y')), x \rangle$; on a donc ${}^t u(d_{\Phi'}(y')) = d_{\Phi}(u^*(y'))$ pour tout $y' \in F'$, d’où ${}^t u \circ d_{\Phi'} = d_{\Phi} \circ u^*$, et par conséquent l’expression annoncée de $u^*$. CQFD.

#### Remarque {#alg-ix-s1-n8-rem-2 .statement}

Lorsque $s_{\Phi}$ est bijective, tout homomorphisme $\nu$ de $F$ dans $F'$ admet un adjoint à droite partout défini, et on a

$$(34)$$
$$\nu^* = (s_{\Phi})^{-1} \circ {}^t \nu \circ s_{\Phi'}.$$

#### Proposition 8 {#alg-ix-s1-prop-8 .statement}

Avec les mêmes notations que précédemment, on suppose que $s_{\Phi}$ et $d_{\Phi}$ sont bijectives. Soient $u$ et $\nu$ des isomorphismes de E sur E' et de F sur F' respectivement. Alors, pour que Φ soit l’image réciproque de Φ' relativement à u et v (c’est-à-dire pour que l’on ait Φ(x, y) = Φ'(u(x), v(y)) quels que soient x ∈ E, y ∈ F), il faut et il suffit que l’on ait u^{-1} = v^* et v^{-1} = u^*.

En effet Φ'(u(x), v(y)) = Φ(x, y) s’écrit aussi Φ (x, u^*(v(y))) = Φ(x, y). Si ceci a lieu quels que soient x ∈ E et y ∈ F, on a u^* ∘ v = 1 puisque Φ est non dégénérée. On a donc aussi v^* ∘ u = 1 d’après (33). La réciproque est immédiate.

#### Corollaire {#alg-ix-s1-n8-cor-1 .statement}

Soient A un anneau muni d’un antiautomorphisme J, E un A-module à gauche, Φ une forme sesquilinéaire pour J sur E × E dont les applications associées sont bijectives, et u un automorphisme du A-module E. Pour que u laisse Φ invariante (c’est-à-dire pour que l’on ait Φ(u(x), u(y)) = Φ(x, y) quels que soient x, y dans E), il faut et il suffit que les deux adjoints de u soient égaux et que l’on ait u^* = u^{-1}.

Ceci résulte aussitôt de la prop. 8.

#### Remarque {#alg-ix-s1-n8-rem-3 .statement}

Sous les hypothèses du cor. de la prop. 8, supposons de plus que A soit un corps et que E soit de dimension finie sur A. Soient ω un endomorphisme de E, ω_1 et ω_2 ses adjoints à droite et à gauche. Chacune des conditions ωω_1 = 1, ωω_2 = 1, ω_1ω = 1, ω_2ω = 1 entraîne que ω est un automorphisme de E laissant Φ invariante, et que ω_1 = ω_2.

### 9. Produits tensoriels et puissances extérieures de formes sesquilinéaires.

Dans ce n°, on désigne par A un anneau commutatif. Une forme bilinéaire sur un produit de deux A-modules est donc un cas particulier de forme sesquilinéaire. On désignera par J un automorphisme de A, et par J' son inverse.

Soient E_i (i = 1, ..., m) des A-modules. L’application

$$(x_1, ..., x_m) \to x_1 \otimes \cdots \otimes x_m$$

de $\prod_{i=1}^m E_i^J$ dans $(\bigotimes_{i=1}^m E_i)^J$ (x_i \in E_i^J) (cf. déf. 5, n° 2) est évidemment A-multilinéaire ; elle définit donc (chap. III, § 1, n° 7) une application A-linéaire $f$ de $\bigotimes_i E_i^j$ dans $(\bigotimes_i E_i)^j$; cette application transforme $x_1 \otimes \cdots \otimes x_m$ (où les signes $\otimes$ désignent les produits tensoriels dans $\bigotimes_i E_i^j$) en $x_1 \otimes \cdots \otimes x_m$ (où les signes $\otimes$ désignent les produits tensoriels dans $(\bigotimes_i E_i)^j$). Donc $f$ est un isomorphisme de $\bigotimes_i E_i^j$ sur $(\bigotimes_i E_i)^j$. Nous identifierons ces deux modules au moyen de cet isomorphisme.

De même soit $E$ un A-module. L’application
$$
(x_1, \ldots, x_m) \to x_1 \wedge \ldots \wedge x_m
$$
de $(E^j)^m$ dans $(\wedge^m E)^j$ est évidemment A-multilinéaire et alternée. Elle définit donc une application A-linéaire $f$ de $\wedge^m E^j$ dans $(\wedge^m E)^j$, qui est évidemment un isomorphisme. Nous identifierons $\wedge^m E^j$ et $(\wedge^m E)^j$ au moyen de cet isomorphisme.

Soit $x'$ un élément du dual $E^*$ de $E$. L’application $x \to \langle x, x' \rangle^j$ ($x \in E$) est un élément $x'^j$ de $(E^j)^*$, et il est immédiat que $x' \to x'^j$ est une bijection $g$ de $E^*$ sur $(E^j)^*$ vérifiant $g(ax') = a^j g(x')$ pour tout $a \in A$. Par suite l’application composée de $g$ et de l’application identique de $(E^*)^j$ sur $E^*$ est un isomorphisme de $(E^*)^j$ sur $(E^j)^*$. Nous identifierons ces modules au moyen de cet isomorphisme, et nous les noterons $E_j^*$.

Soient $E_i, F_i \ (i = 1, \ldots, m)$ des A-modules, et $\Phi_i \ (i = 1, \ldots, m)$ une forme sesquilinéaire pour $J$ sur $E_i \times F_i$. L’application
$$
(x_1, \ldots, x_m, y_1, \ldots, y_m) \to \Phi_1(x_1, y_1) \Phi_2(x_2, y_2) \ldots \Phi_m(x_m, y_m)
$$
$(x_i \in E_i, y_i \in F_i, i = 1, \ldots, m)$ est une application A-multilinéaire de $E_1 \times \cdots \times E_m \times F_1^j \times \cdots \times F_m^j$ dans $A$, et définit donc une forme bilinéaire sur $(\bigotimes_i E_i) \times (\bigotimes_i F_i^j)$ (chap. III, § 1, no 7). Puisque le deuxième facteur a été identifié à $(\bigotimes_i F_i)^j$, on a donc défini une forme sesquilinéaire $\Phi$ pour $J$ sur $(\bigotimes_i E_i) \times (\bigotimes_i F_i)$. Celle-ci est caractérisée par
$$
\Phi(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \prod_{i=1}^m \Phi_i(x_i, y_i) \quad (x_i \in E_i, y_i \in F_i).
$$

#### Définition 11 {#alg-ix-s1-def-11 .statement}

Etant donnés des A-modules $E_i, F_i (i = 1, \ldots, m)$ et, pour chaque $i$, une forme sesquilinéaire $\Phi_i$ pour $J$ sur $E_i \times F_i$, la forme sesquilinéaire $\Phi$ pour $J$ sur $(\bigotimes_i E_i) \times (\bigotimes_i F_i)$ caractérisée par (35) est appelée le produit tensoriel des formes sesquilinéaires $\Phi_i$.

Dans le cas où les $E_i$ et les $F_i$ sont égaux à un même module $E$, et où les $\Phi_i$ sont égales à une même forme $\Psi$, on dit que $\Phi$ est l’extension de $\Psi$ à $\bigotimes^m E$.

Les notations étant celles de la déf. 11, étudions les applications associées à $\Phi$. On tire de la formule (24) (n° 6) et de (35) la relation

$$
\Phi(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \prod_{i=1}^m \langle x_i, d_{\Phi_i}(y_i) \rangle = \prod_{i=1}^m \langle y_i, s_{\Phi_i}(x_i) \rangle^J.
$$

On a donc :

(36) $s_\Phi = j_s \circ (s_{\Phi_1} \otimes \cdots \otimes s_{\Phi_m}), \quad d_\Phi = j_d \circ (d_{\Phi_1} \otimes \cdots \otimes d_{\Phi_m})$

où $j_s$ (resp. $j_d$) désigne l’application canonique de $\bigotimes_i F_i^*$ dans $(\bigotimes_i F_i)^*$ (resp. de $\bigotimes_i E_i^*$ dans $(\bigotimes_i E_i)^*$) (chap. III, § 1, n°s 4 et 7).

#### Proposition 9 {#alg-ix-s1-prop-9 .statement}

Soient $A$ un corps commutatif muni d’un automorphisme $J$, $E_i, F_i$ des espaces vectoriels de dimension finie sur $A$, et $\Phi_i$ une forme sesquilinéaire pour $J$ sur $E_i \times F_i$ ($1 \leqslant i \leqslant m$). Si les formes $\Phi_i$ sont non dégénérées, il en est de même de leur produit tensoriel $\Phi$. Dans ce cas la forme inverse $\widehat{\Phi}$ de $\Phi$ est le produit tensoriel des formes inverses $\widehat{\Phi}_i$.

En effet, comme $A$ est un corps, il résulte des prop. 6 et 7 du chap. III, § 1, n° 3 qu’un produit tensoriel d’applications linéaires injectives (resp. surjectives) de $A$-modules est une application linéaire injective (resp. surjective). Comme les $s_{\Phi_i}$ sont bijectives par hypothèse (prop. 6, n° 6), il en est donc de même de leur produit tensoriel. D’autre part l’application canonique $j_s$ de $\bigotimes_i F_i^*$ dans $(\bigotimes_i F_i)^*$ est bijective (chap. III, § 1, n° 5, prop. 11). Donc, en vertu de (36), $s_\Phi$ est bijective, et ceci établit notre première assertion (prop. 6, n° 6). De même $d_\Phi$ est bijective.

Dans la seconde assertion nous avons implicitement identifié $\bigotimes_i F_i^*$ à $(\bigotimes_i F_i)^*$ et $\bigotimes_i E_i^*$ à $(\bigotimes_i E_i)^*$ au moyen des applications $j_s$ et $j_d$, qui sont ici des isomorphismes. Les formes inverses citées dans l’énoncé existent puisque les $s_{\Phi_i}$, les $d_{\Phi_i}$, $s_\Phi$ et $d_\Phi$ sont bijectives (n° 7). Posons alors $x' = x'_1 \otimes \cdots \otimes x'_m$, $y' = y'_1 \otimes \cdots \otimes y'_m$ ($x'_i \in E_i^*$, $y'_i \in F_i^*$, $i = 1, \ldots, m$). Par définition des formes inverses, et vu (36), on a

$$
\widehat{\Phi}(j_s(y'), j_d(x')) = \Phi(s_{\Phi_1}^{-1}(y'_1) \otimes \cdots \otimes s_{\Phi_m}^{-1}(y'_m), d_{\Phi_1}^{-1}(x'_1) \otimes \cdots \otimes d_{\Phi_m}^{-1}(x'_m))
$$
$$
= \prod_{i=1}^m \Phi_i(s_{\Phi_i}^{-1}(y'_i), d_{\Phi_i}^{-1}(x'_i)) = \prod_{i=1}^m \widehat{\Phi}_i(y'_i, x'_i),
$$

d’où notre seconde assertion.

C. Q. F. D.

Soient E et F deux modules sur l’anneau commutatif A, et $\Phi$ une forme sesquilinéaire pour J sur $E \times F$. L’application
$$
(x_1, \ldots, x_m, y_1, \ldots, y_m) \to \det(\Phi(x_i, y_k)) \quad (x_i \in E, y_i \in F, i = 1, \ldots, m)
$$
de $E^m \times (F^j)^m$ dans A est A-multilinéaire. Elle définit donc une forme bilinéaire $\Phi'$ sur $(\bigotimes^m E) \times (\bigotimes^m F^j)$ caractérisée par
$$
\Phi'(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \det(\Phi(x_i, y_k)).
$$
Comme le premier membre est nul lorsque $x_i = x_k$ ou que $y_i = y_k$ ($i \neq k$), $\Phi'$ définit, par passage aux quotients, une forme bilinéaire sur $(\wedge^m E) \times (\wedge^m F^j)$, ou encore, puisque $\wedge^m F^j$ s’identifie à $(\wedge^m F)^j$, une forme $\Phi_{(m)}$ sesquilinéaire pour J sur $(\wedge^m E) \times (\wedge^m F)$. Celle-ci est caractérisée par
$$
\left\{
\begin{array}{l}
\Phi_{(m)}(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \det(\Phi(x_i, y_k)) \\
(x_i \in E, y_i \in F, i = 1, \ldots, m).
\end{array}
\right.
$$
(37)

#### Définition 12 {#alg-ix-s1-def-12 .statement}

Etant donnés deux A-modules E, F et une forme $\Phi$ sesquilinéaire pour J sur $E \times F$, la forme $\Phi_{(m)}$ sesquilinéaire pour J sur $(\wedge^m E) \times (\wedge^m F)$ caractérisée par (37) s’appelle l’extension de $\Phi$ aux m-ièmes puissances extérieures.

Les notations étant celles de la déf. 12, étudions les applications associées à $\Phi_{(m)}$. On tire de la formule (24) (n° 6) et de (37) les relations

$$
\Phi_{(m)}(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \det(\langle x_i, d_\Phi(y_k) \rangle)
= \det(\langle y_i, s_\Phi(x_k) \rangle^j).
$$

On a donc

$$
s_{\Phi(m)} = k_s \circ (\wedge^m s_\Phi), \quad d_{\Phi m} = k_d \circ (\wedge^m d_\Phi),
$$

où $k_s$ (resp. $k_d$) désigne l’application canonique de $\wedge^m F^*$ dans $(\wedge^m F)^*$ (resp. de $\wedge^m E^*$ dans $(\wedge^m E)^*$) (cf. chap. III, § 8, n° 2).

#### Proposition 10 {#alg-ix-s1-prop-10 .statement}

*Soient A un corps commutatif muni d’un automorphisme J, E et F deux espaces vectoriels de dimension finie sur A, et $\Phi$ une forme sesquilinéaire pour J sur $E \times F$. Si $\Phi$ est non dégénérée, alors son extension $\Phi_{(m)}$ aux m-ièmes puissances extérieures est non dégénérée, et la forme inverse de $\Phi_{(m)}$ est l’extension aux m-ièmes puissances extérieures de la forme inverse $\widehat{\Phi}$ de $\Phi$.*

En effet, comme $s_\Phi$ et $d_\Phi$ sont bijectives par hypothèse (prop. 6, n° 6), il en est de même de leurs puissances extérieures (chap. III, § 5, n° 7). D’autre part les applications canoniques $k_s$ et $k_d$ sont bijectives (chap. III, § 8, n° 2, th. 1). Donc, en vertu de (38), $s_{\Phi(m)}$ et $d_{\Phi(m)}$ sont bijectives, ce qui démontre que $\Phi_{(m)}$ est non dégénérée (prop. 6, n° 6). Dans la seconde assertion nous avons implicitement identifié $\wedge^m F^*$ à $(\wedge^m F)^*$ et $\wedge^m E^*$ à $(\wedge^m E)^*$ au moyen des applications $k_s$ et $k_d$, qui sont ici des isomorphismes (*loc. cit.*). Les formes inverses considérées dans l’énoncé existent puisque $s_\Phi, d_\Phi, s_{\Phi(m)}, d_{\Phi(m)}$ sont bijectives (n° 7). Posons alors $x' = x'_1 \wedge \ldots \wedge x'_m$ et $y' = y'_1 \wedge \ldots \wedge y'_m$ ($x'_i \in E^*, y'_i \in F^*, i = 1, \ldots, m$). Par définition des formes inverses (n° 7) et vu (38), on a

$$
\widehat{\Phi}_{(m)}(k_s(y'), k_d(x')) = \Phi_{(m)}(s^{-1}_\Phi(y'_1) \wedge \ldots \wedge s^{-1}_\Phi(y'_m), d^{-1}_\Phi(x'_1) \wedge \ldots \wedge d^{-1}_\Phi(x'_m))
= \det(\Phi(s^{-1}_\Phi(y'_i), d^{-1}_\Phi(x'_k))) = \det(\widehat{\Phi}(y'_i, x'_k))
$$

d’où notre seconde assertion.

#### Remarque {#alg-ix-s1-n9-rem-1 .statement}

Soient E un A-module libre, et θ l’isomorphisme canonique de $\bigwedge^m E$ sur le sous-module des tenseurs antisymétrisés d’ordre m (chap. III, § 5, n° 6, prop. 6). Soient $\Phi$ une forme sesquilinéaire sur E, $\Phi_{(m)}$ l’extension de $\Phi$ à $\bigwedge^m E$, et $\Theta$ la forme sesquilinéaire sur $\bigwedge^m E$ qui est l’image réciproque par $\theta$ de l’extension de $\Phi$ à $\bigotimes^m E$. D’après la définition de $\theta$ et de l’antisymétrisé d’un tenseur, et d’après (35), on a

$$
\Theta(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \sum_{\sigma, \tau} \varepsilon_\sigma \varepsilon_\tau \Phi(x_{\sigma(1)}, y_{\tau(1)}) \ldots \Phi(x_{\sigma(m)}, y_{\tau(m)})
$$

où $\sigma$ et $\tau$ parcourent le groupe symétrique $S_m$. D’après la formule de calcul des déterminants et la formule (37), cette expression peut s’écrire

$$
\sum_{\tau \in S_m} \varepsilon_\tau \det(\Phi(x_i, y_{\tau(k)})) = m! \det(\Phi(x_i, y_k));
$$

autrement dit, on a $\Theta = m! \Phi_{(m)}$.

### 10. Calculs matriciels.

Nous nous proposons, dans le présent n°, d’assouplir le calcul matriciel introduit au chap. II, § 6, et de l’appliquer à traduire certains résultats démontrés dans ce paragraphe.

I. — Soient I et K deux ensembles finis d’indices, H un ensemble non vide, et $M = (m_{ik})_{(i,k) \in I \times K}$ une matrice sur H (chap. II, § 6, n° 1, déf. 1).

On appelle transposée de $M$, et on note ${}^tM$, la matrice $(m'_{ki})_{(k,i) \in K \times I}$ vérifiant $m'_{ki} = m_{ik} \ ((i, k) \in I \times K)$. On a évidemment

$$(39)$$
$$
{}^t({}^tM) = M.
$$

Ceci généralise la notion introduite au chap. II, § 6, n° 6.

Supposons que H soit un groupe commutatif (noté additivement). L’ensemble des matrices sur H ayant I et K pour ensembles d’indices admet une structure de groupe commutatif, puisque c’est l’ensemble des applications de $I \times K$ dans H. Ce groupe est noté additivement.

Soient H', H'' deux ensembles non vides, H un groupe commutatif (noté additivement) et $f : (h', h'') \to h'h''$ une application de $\mathbf{H}' \times \mathbf{H}''$ dans $\mathbf{H}$. Etant données deux matrices
$$
M' = (m_{ik}')_{(i,k) \in I \times K}, \qquad M'' = (m_{kl}'')_{(k,l) \in K \times L}
$$
sur $\mathbf{H}'$ et $\mathbf{H}''$ respectivement, telles que l’ensemble $K$ des indices des colonnes de $M'$ soit égal à l’ensemble des indices de lignes de $M''$, on appelle *produit* de $M'$ et $M''$ (suivant $f$) et on note $M'M''$ la matrice
$$
M'.M'' = (\sum_{k \in K} m_{ik}' m_{kl}'' )_{(i,l) \in I \times L}
$$
sur $\mathbf{H}$. Ceci généralise la notion introduite au chap. II, § 6, no 4.
Si $\mathbf{H}' = \mathbf{H}'' = \mathbf{H}$ et si $\mathbf{H}$ est un anneau, le produit $M'M''$ sera, sauf mention expresse du contraire, calculé « dans $\mathbf{H}$ », c’est-à-dire suivant l’application $(x, y) \to xy$. Lorsque $\mathbf{H}'$ et $\mathbf{H}''$ sont des groupes commutatifs (notés additivement) et que $f$ est bilinéaire, on a
$$
\left\{
\begin{array}{l}
(M' + M'_1)M'' = M'M'' + M'_1M'', \\
M'(M'' + M''_1) = M'M'' + M'M''_1,
\end{array}
\right.
$$
où $M', M'_1$ sont des matrices sur $\mathbf{H}'$, $M'', M''_1$ des matrices sur $\mathbf{H}''$, et où les sommes et produits écrits sont supposés définis. Soient $M', M''$ des matrices sur les ensembles $\mathbf{H}', \mathbf{H}''$, et $f^0$ l’application de $\mathbf{H}'' \times \mathbf{H}'$ dans $\mathbf{H}$ définie par $(h'', h') \to h'h''$; alors on a
$$
t(M'M'') = tM'' . tM'
$$
où le produit dans le premier (resp. second) membre est calculé suivant $f$ (resp. $f^0$).

Dans le cas où $\mathbf{H}' = \mathbf{H}'' = \mathbf{H}$ est un anneau, on retrouve la formule (12) du chap. II, § 6, no 6.

Soient $A$ un anneau, $J$ un antiautomorphisme de $A$. Pour toute matrice $M = (m_{ik})$ sur $A$, nous noterons $M^J$ la matrice $(m_{ik}^J)$. Soient $M_1, M_2$ deux matrices sur $A$ telle que $M_1M_2$ soit défini. Comme $J$ est un isomorphisme de $A$ sur l’anneau opposé $A^0$, on a $(M_1M_2)^J = M_1^J . M_2^J$ où le premier (resp. second) membre est calculé dans $A$ (resp. $A^0$). Vu (42) et (39), ceci donne
$$
(M_1M_2)^J = t(tM_2^J . tM_1^J)
$$
où les *deux* membres sont calculés dans $A$.

Bourbaki XXIV.

Soient $H_1, H_2, H_3, H_{12}, H_{23}$ et $H$ des groupes commutatifs (notés additivement), $f_{12} : H_1 \times H_2 \to H_{12}$, $f_{23} : H_2 \times H_3 \to H_{23}$, $f_3 : H_{12} \times H_3 \to H$, $f_1 : H_1 \times H_{23} \to H$ des applications, et soient $M_1, M_2, M_3$ des matrices sur $H_1, H_2, H_3$ respectivement. Si $f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))$ quels que soient les $x_i \in H_i$ ($i = 1, 2, 3$), alors les produits $(M_1 M_2) M_3$ et $M_1 (M_2 M_3)$ (calculés suivant $f_{12}, f_3, f_{23}$ et $f_1$), s’ils sont définis, sont égaux ; on les notera $M_1 M_2 M_3$. Lorsque $H_1 = H_2 = H_3 = H_{12} = H_{23} = H$, que $H$ est un anneau, et que $f_{12}, f_{23}, f_3, f_1$ sont égales à l’application $(x, y) \to xy$, la condition précédente exprime l’associativité de cette dernière, et est donc vérifiée. On fera des conventions analogues pour les produits de plus de trois facteurs.

Soient $A, B$ deux anneaux, $M = (m_{ik})_{(i,k) \in I \times K}$ et $M' = (m'_{ik})_{(i,k) \in I \times K}$ deux matrices sur un $(A, B)$-bimodule $G$ (no 1). Si, pour toute matrice à une ligne $L = (a_i)_{i \in I}$ à éléments dans $A$ et toute matrice à une colonne $C = (b_k)_{k \in K}$ à éléments dans $B$, on a $L . M . C = L . M' . C$ (les produits étant calculés suivant les applications qui définissent la structure de $(A, B)$-bimodule de $G$), alors les matrices $M$ et $M'$ sont égales. En effet, si l’on prend $a_i = 1, a_s = 0$ pour $s \neq i$, $b_k = 1, b_t = 0$ pour $t \neq k$, les matrices $L . M . C$ et $L . M' . C$, qui sont des matrices scalaires, sont respectivement égales à $m_{ik}$ et $m'_{ik}$.

II. — On considère un anneau $A$ et un $A$-module (à droite ou à gauche) $E$, admettant une base finie $(e_i)_{i \in I}$. Pour tout élément $x$ de $E$, on appelle matrice de $x$ par rapport à la base $(e_i)$, et on note $M(x)$ ou $x$, la matrice à une colonne formée des composantes $x_i$ ($i \in I$) de $x$ par rapport à $(e_i)$ (cf. chap. II, § 6, no 4); dans les calculs il sera commode, afin de rappeler que l’indice $i$ est un indice de ligne, de lui adjoindre un indice de colonne susceptible d’une seule valeur, et d’écrire $(x_{i0})$ la matrice $M(x)$.

Considérons maintenant deux $A$-modules (à gauche ou à droite) $E$ et $F$, ayant des bases finies $(e_i)_{i \in I}$ et $(f_k)_{k \in K}$ respectivement; soit $(f_k^*)$ la base de $F^*$ duale de $(f_k)$. Nous allons définir la matrice, par rapport à ces bases, d’une application $u$ de $E$ dans $F$ dans les quatre cas suivants :

(D) $E$ et $F$ sont des modules à droite, $u$ est $A$-linéaire ;

(G) E et F sont des modules à gauche, u est A-linéaire ;
(GD) E est un module à gauche, F un module à droite, A est muni d’un antiautomorphisme J, u est $\mathbf{Z}$-linéaire et vérifie $u(ax) = u(x)a^J$ ($a \in A,\ x \in E$) (autrement dit u est une application A-linéaire de $E^J$ dans F (no 2, déf. 5)).
(DG) E est un A-module à droite, F un A-module à gauche, A est muni d’un autiautomorphisme J, u est $\mathbf{Z}$-linéaire et vérifie $u(xa) = a^Ju(x)$ ($x \in E,\ a \in A$) (autrement dit u est une application A-linéaire de $E^J$ dans F).
Dans chacun de ces quatre cas, la matrice de l’application u est, par définition, la matrice $(u_{ki})_{(k,i) \in \mathbb{K} \times I}$ telle que
$$
u_{ki} = \langle u(e_i), f_k^* \rangle.
$$
Cette définition coïncide, dans le cas (D), avec celle donnée au chap. II, § 6, no 3. Dans ces conditions la matrice $M(u(x))$ de l’image d’un élément x de E est donnée par les formules suivantes :
$$
\begin{align*}
(45\ D)\quad &M(u(x)) = M(u) \cdot M(x) \\
(45\ G)\quad &{}^tM(u(x)) = {}^tM(x) \cdot {}^tM(u) \\
(45\ GD)\quad &M(u(x)) = M(u) \cdot M(x)^J \\
(45\ DG)\quad &{}^tM(u(x)) = {}^tM(x)^J \cdot {}^tM(u).
\end{align*}
$$
Vérifions, par exemple (45 DG), les autres vérifications étant analogues et un peu plus faciles. Posons $x = \sum e_ix_{io}$, $u(x) = \sum y_{ko}f_k$; on a $u(x) = u(\sum e_ix_{io}) = \sum x_{io}^ju(e_i) = \sum x_{io}^ju_{ki}/k$; d’où $y_{ko} = \sum x_{io}^ju_{ki}$; afin de mettre les deux indices i à côté l’un de l’autre, considérons les matrices transposées ${}^tM(x) = (x'_{oi})$ où $x'_{oi} = x_{io}$, et ${}^tM(u) = (u'_{ik})$ où $u'_{ik} = u_{ki}$; on a alors $y_{ko} = \sum x'_{oi}u'_{ik}$; comme le second membre est l’élément d’indice k de la matrice à une ligne ${}^tM(x)^J \cdot {}^tM(u)$, la formule (45 DG) est vérifiée.

#### Remarque 1 {#alg-ix-s1-n10-rem-1 .statement}

Lorsque A est commutatif, (45 G) se ramène à (45 D), et (45 DG) à (45 GD), au moyen de la formule ${}^t(M'M'') = {}^tM'' \cdot {}^tM'$ (cf. (42)), où les deux membres sont ici calculés dans A.
2) Soient E, F, G trois modules à gauche ayant des bases finies, et $u : E \to F,\ v : F \to G$ des applications A-linéaires. Il résulte de (45 G) que l’on a
$$
{}^tM(v \circ u) = {}^tM(u) \cdot {}^tM(v).
$$

En effet, on a, quel que soit $x \in E$,

$$
{}^t M(x) \cdot {}^t M(\varphi \circ u) = {}^t M(\varphi(u(x))) = {}^t M(u(x)) \cdot {}^t M(\varphi)
= {}^t M(x) \cdot {}^t M(u) \cdot {}^t M(\varphi),
$$

d’où (46).

Rappelons que, dans le cas des modules à droite, on a

$$
M(\varphi \circ u) = M(\varphi) M(u).
$$

III. — On désigne désormais par A un anneau, par B un anneau (resp. un anneau muni d’un antiautomorphisme J, pour lequel on pose $J' = J^{-1}$), par E un A-module à gauche ayant une base finie $(e_i)_{i \in I}$, et par F un B-module à droite (resp. à gauche) ayant une base finie $(f_k)_{k \in K}$. On note $(e_i^*)$ et $(f_k^*)$ les bases duales de E* et F*. Sauf mention expresse du contraire les matrices considérées sont prises par rapport à ces bases.

Soient G un (A, B)-bimodule (n° 1), Φ une application bilinéaire (resp. sesquilinéaire à droite pour J) de $E \times F$ dans G, et $R = (\Phi(e_i, f_k))$ la matrice de Φ. Alors, pour $x \in E$ et $y \in F$, la formule (6) du n° 1 (resp. (8) du n° 2), s’écrit, moyennant les conventions ci-dessus,

(47) $\Phi(x, y) = {}^t M(x) \cdot R \cdot M(y)$ (resp. $\Phi(x, y) = {}^t M(x) \cdot R \cdot M(y)^J$),

où les produits sont calculés suivant les applications qui définissent la structure de (A, B)-bimodule de G ; en particulier, si $A = B = G$ (auquel cas Φ est une forme), les produits sont calculés dans A.

Soient E’ un A-module à gauche ayant une base finie $(e'_s)_{s \in S}$, F’ un A-module à droite (resp. à gauche) ayant une base finie $(f'_t)_{t \in T}$, $u : E \to E'$ et $\varphi : F \to F'$ des applications A-linéaires, et $\Phi'$ une application bilinéaire (resp. sesquilinéaire à droite pour J) de $E' \times F'$ dans G. Notons Φ l’image réciproque de $\Phi'$ (relativement à $u$ et $\varphi$), $U, V, R, R'$ les matrices de $u, \varphi, \Phi, \Phi'$ par rapport aux bases considérées. On a alors

(48) $R = {}^t U \cdot R' \cdot V$ (resp. $R = {}^t U \cdot R' \cdot V^J$),

les produits étant calculés comme dans (47). En effet, quels que soient $x \in E$ et $y \in F$, on a par définition $\Phi(x, y) = \Phi'(u(x), v(y))$, d’où, d’après (47),

$$
'M(x).R.M(y) = 'M(u(x)).R'.M(v(y))
$$
(resp. $'M(x).R.M(y)^J = 'M(u(x)).R'.M(v(y))^J$);

d’après (45 G) et (45 D) (resp. (45 G)) et (43) on en déduit

$$
'M(x).R.M(y) = 'M(x).'U.R'.V.M(y)
$$
(resp. $'M(x).R.M(y)^J = 'M(x).'U.R'.('M(y).'V)^J$
$= 'M(x).'U.R'.V^J.M(y)^J$);

ceci démontre notre assertion.

IV. — On suppose ici que les anneaux $A$ et $B$ sont égaux, et on désigne par $\Phi$ une forme bilinéaire (resp. sesquilinéaire à droite pour J) sur $E \times F$, et par $R$ sa matrice. Calculons les matrices des applications $s_\Phi$ et $d_\Phi$ associées à $\Phi$, que nous noterons $s$ et $d$ pour alléger. Comme on a $\Phi(x, y) = \langle y, s(x) \rangle = \langle x, d(y) \rangle$ d’après (23), n° 6 (resp. $\Phi(x, y) = \langle x, d(y) \rangle = \langle y, s(x) \rangle^J$ d’après (24), n° 6), on a $\Phi(e_i, f_k) = \langle f_k, s(e_i) \rangle = \langle e_i, d(f_k) \rangle$ (resp. $\Phi(e_i, f_k) = \langle e_i, d(f_k) \rangle = \langle f_k, s(e_i) \rangle^J$), d’où, d’après (44) et puisque $(e_i)$ est la base duale de $(e_i^*)$ et $(f_k)$ la base duale de $(f_k^*)$:

(49) $M(d) = R, \ M(s) = 'R$   (resp. $M(d) = R, \ M(s) = 'R^{J'}$).

#### Remarque 2 {#alg-ix-s1-n10-rem-2 .statement}

Lorsque $A$ est un corps, les applications linéaires $s$ et $d$ ont même rang. Nous voyons ici que leurs matrices $M(s)$ et $M(d)$ ont même rang ; en effet, une matrice sur $A$ et sa transposée ont même rang (chap. II, § 6, n° 7, prop. 3) et, lorsque $\Phi$ est sesquilinéaire, l’égalité des rangs de $R$ sur $A$ et de $'R$ sur $A^0$ (ibid.) et le fait que $J'$ est un isomorphisme de $A^0$ sur $A$, entraînent l’égalité des rangs de $R$ et de $'R^J$ sur $A$.

#### Remarque 3 {#alg-ix-s1-n10-rem-3 .statement}

Si $M$ et $N$ sont des $A$-modules à droite ayant des bases finies $(m_i)$ et $(n_k)$, $\Phi$ une forme sesquilinéaire à gauche pour $J$ sur $M \times N$ (n° 6, Remarque), $s$ et $d$ ses applications associées, et $R = (\Phi(m_i, n_k))$ sa matrice, les formules (26) du n° 6 montrent que l’on a

$$
M(d) = R^{J'}, \quad M(s) = 'R.
$$

Supposons maintenant que les applications $s$ et $d$ associées à $\Phi$ sont bijectives et calculons la matrice $\hat{R}$ de la forme inverse de $\Phi$ (n° 7). Lorsque $\Phi$ est bilinéaire, $\Phi$ est l’image réciproque de $\hat{\Phi}$ relativement aux applications linéaires $s : E \to F^*$ et $d : F \to E^*$; on a donc, en vertu de (48) et (49), $R = R . \hat{R} . R$, d’où, puisque $R$ est inversible ($d$ étant bijective), $\hat{R} = R^{-1}$. Cette formule s’étend au cas où $\Phi$ est sesquilinéaire, car, si l’on considère $\Phi$ comme une forme bilinéaire sur $E \times F^J$, et si l’on identifie $(F^J)^*$ à $(F^*)^J$ (cf. n° 9), la forme inverse de cette forme bilinéaire coïncide avec $\hat{\Phi}$ considérée comme forme bilinéaire sur $(F^*)^J \times E^*$. Dans les deux cas *la matrice de la forme inverse de $\Phi$ est l’inverse de la matrice de $\Phi$*.

Soient enfin $E'$ un A-module à gauche, $F'$ un A-module à droite (resp. à gauche), admettant tous deux des bases finies $(e'_s)$ et $(f'_t)$; soit $\Phi'$ une forme bilinéaire (resp. sesquilinéaire pour J) sur $E' \times F'$, et soit $R'$ sa matrice. Supposons $s_\Phi$ et $d_\Phi$ bijectives. Soient $u : E \to E'$ et $\nu : F \to F'$ des applications linéaires, $u^* : F' \to F$ et $\nu^* : E' \to E$ leurs *adjointes* (n° 8, prop. 7) ; notons $U, V, U^*, V^*$ les matrices de $u, \nu, u^*, \nu^*$ par rapport aux bases données. On a alors

$$
U^* = R^{-1} . {}^t U . R', \quad {}^t V^* = R'. V . R^{-1}
$$
(resp. $U^{*J} = R^{-1} . {}^t U . R', \ {}^t V^* = R'. V^J . R^{-1}$).

En effet, quels que soient $x \in E$ et $y \in F'$, on a $\Phi'(u(x), y) = \Phi(x, u^*(y))$ (n° 8, déf. 10). D’où, lorsque $\Phi$ est bilinéaire, en vertu de (47), ${}^t M(u(x)) . R' . M(y) = {}^t M(x) . R . M(u^*(y))$; ceci donne, en vertu de (45 G) et (45 D), ${}^t M(x) . {}^t U . R' . M(y) = {}^t M(x) . R . U^* . M(y)$, d’où ${}^t U . R' = R . U^*$ et la première formule annoncée puisque, $d$ étant bijective, $R$ est inversible. Lorsque $\Phi$ est sesquilinéaire (47) et (45 G) donnent ${}^t M(x) . {}^t U . R' . M(y)^J = {}^t M(x) . R . {}^t ({}^t M(y) . {}^t U^*)^J$; or, d’après (43), on a $({}^t M(y) . {}^t U^*)^J = {}^t ({}^t U^{*J} . {}^t M(y)^J)$, d’où ${}^t ({}^t M(y) . {}^t U^*)^J = U^{*J} . M(y)^J$; il vient donc ${}^t M(x) . {}^t U . R' . M(y)^J = {}^t M(x) . R . U^{*J} . M(y)^J$, d’où ${}^t U . R' = R . U^{*J}$, et $U^{*J} = R^{-1} . {}^t U . R'$. La vérification des formules pour $V^*$ est analogue.

*Exercices.* — 1) Soient A un corps commutatif, E un espace vectoriel sur A admettant une base infinie dénombrable $(e_n)_{n \geqslant 1}$. On définit une forme bilinéaire $\Phi$ sur E en posant $\Phi(e_{i+1}, e_i) = 1$ pour $i \geqslant 1$, $\Phi(e_k, e_j) = 0$ pour $k \neq j + 1$ et $j \geqslant 1$. Montrer que l’application linéaire $d_\Phi$ associée à droite à $\Phi$ est injective, mais que l’application linéaire $s_\Phi$ associée à gauche à $\Phi$ n’est pas injective.

2) Soit E le $\mathbf{Z}$-module somme directe de $\mathbf{Z}$ et de $\mathbf{Z}/(2)$, et soit $E^*$ son dual (isomorphe à $\mathbf{Z}$). Montrer que la forme bilinéaire $(x, x') \to \langle x, x' \rangle$ sur $E \times E^*$ est telle que l’application linéaire associée à droite est injective, mais non l’application linéaire associée à gauche.

#### Remarque 4 {#alg-ix-s1-n10-rem-4 .statement}

Donner un exemple de forme bilinéaire $\Phi$ définie sur un produit $E \times F$ de deux espaces vectoriels, telle que $d_\Phi$ soit bijective, $s_\Phi$ injective mais non bijective (prendre $E$ de dimension infinie et $F$ égal au dual $E^*$ de $E$; cf. chap. II, § 5, exerc. 3).

#### Remarque 5 {#alg-ix-s1-n10-rem-5 .statement}

Soient $A$ un anneau muni d’un antiautomorphisme $J$, $E$ un $A$-module à gauche, $G$ un $(A, A)$-bimodule et $\Phi$ une application de $E \times E$ dans $G$, sesquilinéaire à droite pour $J$. Démontrer l’identité (où $Q(x) = \Phi(x, x)$) :

$$
2\Phi(x, y)\ (\mu^J\lambda^J - \lambda^J\mu^J) = Q(x - \mu\lambda y) - Q(x + \mu\lambda y) + \mu Q(x + \lambda y)
- \mu Q(x - \lambda y) + Q(x + \mu y)\lambda^J - Q(x - \mu y)\lambda^J + \mu Q(x - y)\lambda^J - \mu Q(x + y)\lambda^J.
$$

#### Remarque 6 {#alg-ix-s1-n10-rem-6 .statement}

Soient $K$ un corps commutatif de caractéristique 2, $A$ une extension quadratique séparable de $K$; on a $A = K(\theta)$, où $\theta$ est racine d’un polynôme irréductible $X^2 + X + \beta$ de $K[X]$ et le $K$-automorphisme $J$ de $A$, distinct de l’identité, est tel que $\theta^J = \theta + 1$ (chap. V, § 11, exerc. 8). Montrer que si $E$ et $G$ sont des espaces vectoriels sur $A$, $\Phi$ une application sesquilinéaire (pour $J$) de $E \times E$ dans $G$, on a, en posant $Q(x) = \Phi(x, x)$,

$$
\Phi(x, y) = Q(\theta x + y) - \beta Q(x) - Q(y) - (\theta + 1)(Q(x + y) - Q(x) - Q(y)).
$$

#### Remarque 7 {#alg-ix-s1-n10-rem-7 .statement}

Soient $A$ un corps, $E$ un espace vectoriel sur $A$, $\Phi$ une forme sesquilinéaire sur $E$, $u$ un endomorphisme de $E$.

a) Pour qu’il existe un endomorphisme $u^*$ et un seul de $E$ tel que $\Phi(u(x), y) = \Phi(x, u^*(y))$ pour $x, y$ dans $E$, il faut et il suffit que $d_\Phi$ soit injective et que $u(d_\Phi(E)) \subset d_\Phi(E)$.

b) Donner un exemple où $E$ est de dimension infinie et $d_\Phi$ injective, mais où $u(d_\Phi(E))$ n’est pas contenu dans $d_\Phi(E)$.

#### Remarque 8 {#alg-ix-s1-n10-rem-8 .statement}

Soient $E, E_1$ deux $A$-modules, $\Phi$ (resp. $\Phi_1$) une forme sesquilinéaire sur $E$ (resp. $E_1$). On suppose que $\Phi_1$ est non dégénérée et qu’il existe un élément $\alpha \in A$ et une bijection $u$ de $E$ sur $E_1$ telle que $\Phi_1(u(x), u(y)) = \Phi(x, y)\alpha$ quels que soient $x, y$ dans $E$. Montrer que : 1° $\Phi$ est non dégénérée ; 2° $u$ est linéaire ; 3° si $E_1$ est un $A$-module fidèle, il en est de même de $E$, et $\alpha$ n’est pas diviseur de 0 à droite dans $A$ ; 4° si $\Phi_1$ prend des valeurs dans $A$ qui ne sont pas diviseurs à gauche de 0, il en est de même de $\Phi$.

#### Remarque 9 {#alg-ix-s1-n10-rem-9 .statement}

Soient $A$ un corps, $E_1, E_2$ deux espaces vectoriels non réduits à 0 sur $A$, $\Phi_1$ (resp. $\Phi_2$) une forme sesquilinéaire non dégénérée sur $E_1$ (resp. $E_2$) pour un antiautomorphisme $J_1$ (resp. $J_2$) de $A$. Soit $u$ une application linéaire de $E_1$ sur $E_2$ telle que la relation $\Phi_1(x, y) = 0$ entraîne $\Phi_2(u(x), u(y)) = 0$.

a) Montrer que $u$ est une bijection de $E_1$ sur $E_2$. (Si $u(0)$ n’était pas réduit à 0, montrer qu’il existerait dans $E_1$ deux vecteurs $a, b$ tels que $u(a) \neq 0, u(b) = 0$ et $\Phi_1(a, b) \neq 0$; si $H$ est l’hyperplan des $x \in E_1$ tels que $\Phi_1(a, x) = 0$, remarquer que l’on aurait $u(H) = E_2$.

b) Montrer que si dim $E_1 \geqslant 2$, il existe $\alpha \in A$ tel que l’on ait $\Phi_2(u(x), u(y)) = \Phi_1(x, y)\alpha$ quels que soient $x, y$ dans $E_1$. (Pour tout $y \in E_1$, montrer qu’il existe un élément $m(y) \in A$ tel que $\Phi_2(u(x), u(y)) = \Phi_1(x, y)m(y)$ pour tout $x \in E_1$, et que si $y$ et $y'$ sont linéairement indépendants dans $E_1$, on a $m(y + y') = m(y) = m(y')$).

#### Remarque 10 {#alg-ix-s1-n10-rem-10 .statement}

Soient $A$ un corps, $E, F$ deux espaces vectoriels à gauche sur $A$, $\Phi$ une forme sesquilinéaire non dégénérée sur $E \times F$ pour un antiautomorphisme $J$ de $A$.

a) Soient $M$ un sous-espace de $E$, $N$ un sous-espace de $F$ tels que $N \supset M^0$ et $M \supset N^0$. Montrer que si l’un des espaces $N/M^0, M/N^0$ est de dimension finie, il en est de même de l’autre, et les dimensions de ces deux espaces sont égales.

b) Soient $M, M'$ deux sous-espaces de $E$ tels que $M^{00} = M$ et que $M'$ soit de dimension finie ; montrer que l’on a $(M \cap M')^0 = M^0 + M'^0$ et $(M + M')^{00} = M + M'$. (En appliquant $a$) aux sous-espaces $M'$ et $M^0 + M'^0$, montrer que $\dim(M \cap M') = \operatorname{codim}(M^0 + M'^0)$; en appliquant $a$ aux sous-espaces $M + M'$ et $M^0$, montrer que
$$
\dim((M + M')^{00}/M) = \dim((M + M')/M)).
$$

c) Si $E = F$ et si $M$ est un sous-espace de $E$ tel que $E = M^0 + M^{00}$, montrer que $E$ est somme directe de $M^0$ et $M^{00}$.

d) Soit $E$ un espace vectoriel sur un corps commutatif $A$ admettant une base infinie dénombrable $(e_n)_{n \geqslant 0}$, et soit $\Phi$ la forme bilinéaire symétrique sur $E$ telle que $\Phi(e_n, e_n) = 1$ pour tout $n$, $\Phi(e_i, e_j) = 0$ pour $i \geqslant 1, j \geqslant 1$ et $i \neq j$, et $\Phi(e_0, e_n) = 1$ pour tout $n \geqslant 1$. Montrer que $\Phi$ est non dégénérée. Soit $M$ (resp. $N$) le sous-espace de $E$ engendré par les $e_{2k}$ (resp. $e_{2k-1}$) pour $k \geqslant 1$, et soit $H = M + N$, qui est un hyperplan dans $E$. Montrer que l’on a $M^0 = N, N^0 = M, H^{00} = E \neq H, (M \cap N)^0 \neq M^0 + N^0$ et $(M + N)^{00} \neq M + N$, bien que $M^{00} = M, N^{00} = N$; si $L$ est le sous-espace de dimension 2 engendré par $e_0$ et $e_1$, on a $(L \cap H)^0 \neq L^0 + H^0$.

#### Remarque 11 {#alg-ix-s1-n10-rem-11 .statement}

Soient $E, E'$ deux espaces vectoriels à gauche sur des corps $A, A'$ respectivement, de dimension $\geqslant 3$; soit $\mathfrak{F}(E)$ (resp. $\mathfrak{F}(E')$) l’ensemble réticulé (pour la relation d’inclusion) formé des sous-espaces de dimension finie de $E$ (resp. $E'$).

a) Soit $p$ une application de $\mathfrak{F}(E)$ dans $\mathfrak{F}(E')$ telle que pour tout $M \in \mathfrak{F}(E)$, $\dim p(M) = \dim M$, et que pour tout couple $(M, N)$ d’éléments de $\mathfrak{F}(E)$, $p(M + N) = p(M) + p(N)$. Montrer que $p$ est injective ; si $p$ est bijective, il existe une application semi-linéaire bijective $u$ de $E$ dans $E'$ telle que l’on ait $u(M) = p(M)$ pour tout $M \in \mathfrak{F}(E)$ (utiliser l’exerc. 10 du chap. II, 2e éd., App. III).

b) Donner un exemple où $A' = A$ est commutatif, $E' = E$ est de dimension finie, et où il existe une application $p$ de $\mathfrak{F}(E)$ dans lui-même, telle que $\dim p(M) = \dim M, p(M + N) = p(M) + p(N), p(M \cap N) = p(M) \cap p(N)$, mais il n’existe aucune application semi-linéaire injective $u$ de $E$ dans lui-même telle que $u(M) = p(M)$ pour $M \in \mathfrak{F}(E)$. (Considérer le cas où il existe un surcorps $A''$ de $A$ de degré fini et isomorphe à $A$,
