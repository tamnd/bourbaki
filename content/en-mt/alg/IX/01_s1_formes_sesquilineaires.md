---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 1
section_title: Formes sesquilinéaires
lang: en
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
content_sha256: a788ed40848999c0d18ff945a803189841c5bd0cc9a81227b38d5b0ae7369e0a
translated_from: content/fr/alg/IX/01_s1_formes_sesquilineaires.md
source_lang: fr
translation_method: machine
source_content_sha256: b21644da462961bf5e76bb84af83bd25fbddfd44913e5d77b17fe0efb600df69
translation_model: gpt-5-6-mini
translation_run: translate-en-mt-019184ab
glossary_version: 34
glossary_terms_sha256: 8c5093eec2fb66288d37b2c9e6277da6562aca5edc333a7d4338779d8b066ee8
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. Sesquilinear Forms

### 1. Bilinear mappings.

In this No. $A$ and $B$ denote two rings, $E$ a left $A$-module, $F$ a right $B$-module, and $G$ an $(A, B)$-bimodule, that is to say, a commutative group endowed with a structure of left $A$-module and a structure of right $B$-module such that $(ag)b = a(gb)$ for all $a \in A$, $b \in B$, $g \in G$.

#### Definition 1 {#alg-ix-s1-def-1 .statement}

A mapping $\Phi$ of the product $E \times F$ into $G$ is said to be bilinear if it satisfies the following conditions:

(1) $\Phi(x + x', y) = \Phi(x, y) + \Phi(x', y)$
    for all $x \in E$, $x' \in E$, $y \in F$ ;
(2) $\Phi(x, y + y') = \Phi(x, y) + \Phi(x, y')$
    for all $x \in E$, $y \in F$, $y' \in F$ ;
(3) $\Phi(ax, y) = a\Phi(x, y)$ for all $a \in A$, $x \in E$, $y \in F$ ;
(4) $\Phi(x, yb) = \Phi(x, y)b$ for all $x \in E$, $y \in F$, $b \in B$.

The tensor product $E \otimes_{\mathbf{Z}} F$ is canonically endowed with a structure of $(A, B)$-bimodule characterized by $a(x \otimes y)b = ax \otimes yb$ (Chap. III, 2e éd., App. II, n° 3), and the giving of a bilinear mapping $\Phi$ of $E \times F$ into $G$ is equivalent to that of a mapping $\Psi$ of $E \otimes_{\mathbf{Z}} F$ into $G$ which is a homomorphism for the structures of $(A, B)$-bimodules and which satisfies $\Psi(x \otimes y) = \Phi(x, y)$ for all $x \in E$ and $y \in F$.

The conditions imposed on $\Phi$ by Definition 1 signify that the partial mappings $d_\Phi(y) : x \to \Phi(x, y)$ and $s_\Phi(x) : y \to \Phi(x, y)$ are respectively an A-linear mapping from $E$ into $G$ and a B-linear mapping from $F$ into $G$. Let us endow the commutative group $\mathcal{L}_A(E, G)$ (resp. $\mathcal{L}_B(F, G)$) with the structure of right B-module (resp. left A-module) defined by $ub(x) = u(x) . b$ ($u \in \mathcal{L}_A(E, G)$, $x \in E$, $b \in B$) (resp. $a \nu(y) = a . \nu(y)$ ($a \in A$, $\nu \in \mathcal{L}_B(F, G)$, $y \in F$)). Then conditions (1) to (4) are respectively equivalent to:

$$
\begin{align*}
(1') & \quad s_\Phi(x + x') = s_\Phi(x) + s_\Phi(x') \\
(2') & \quad d_\Phi(y + y') = d_\Phi(y) + d_\Phi(y') \\
(3') & \quad s_\Phi(ax) = a.s_\Phi(x) \\
(4') & \quad d_\Phi(yb) = d_\Phi(y).b,
\end{align*}
$$

for all $x, x'$ in $E$, $y, y'$ in $F$, $a \in A$, $b \in B$; in other words, the mapping $d_\Phi$ from $F$ into $\mathcal{L}_A(E, G)$ is B-linear, and the mapping $s_\Phi$ from $E$ into $\mathcal{L}_B(F, G)$ is A-linear. We have, by definition

$$(5) \quad \Phi(x, y) = d_\Phi(y)(x) = s_\Phi(x)(y) \text{ for all } x \in E, y \in F.$$

#### Definition 2 {#alg-ix-s1-def-2 .statement}

Given a bilinear mapping $\Phi$ from $E \times F$ into $G$, the mapping $d_\Phi$ from $F$ into $\mathcal{L}_A(E, G)$ (resp. the mapping $s_\Phi$ from $E$ into $\mathcal{L}_B(F, G)$) characterized by (5) is called the linear mapping associated on the right (resp. on the left) with $\Phi$.

Conversely, the data of a B-linear mapping $d$ from $F$ into $\mathcal{L}_A(E, G)$ (resp. of an A-linear mapping $s$ from $E$ into $\mathcal{L}_B(F, G)$) determines uniquely, by the formula

$$
\Phi(x, y) = d(y)(x) \quad \text{(resp. } \Phi(x, y) = s(x)(y))
$$

a bilinear mapping $\Phi$ from $E \times F$ into $G$, of which $d$ (resp. $s$) is the linear mapping associated on the right (resp. on the left).

#### Definition 3 {#alg-ix-s1-def-3 .statement}

A bilinear mapping $\Phi$ of $E \times F$ into $G$ is said to be degenerate on the right (resp. on the left) if there exists a nonzero element $y_0$ of $F$ (resp. $x_0$ of $E$) such that $\Phi(x, y_0) = 0$ for all $x \in E$ (resp. $\Phi(x_0, y) = 0$ for all $y \in F$). We say that $\Phi$ is degenerate if it is degenerate on the right or if it is degenerate on the left.

For $\Phi$ to be nondegenerate on the right (resp. on the left) it is necessary and sufficient that the linear mapping associated on the right (resp. on the left) to $\Phi$ be injective; saying that $\Phi$ is nondegenerate therefore means that the associated linear mappings $d_\Phi$ and $s_\Phi$ are both injective.

Let $(e_i)_{i \in I}$ and $(f_k)_{k \in K}$ be two families of elements of $E$ and $F$, and let $(a_i)_{i \in I}$ and $(b_k)_{k \in K}$ be two families of elements of $A$ and $B$, all but a finite number of which are zero. It follows from equalities (1) to (4), by induction on the number of nonzero coefficients, that we have

$$
\Phi(\sum_i a_i e_i, \sum_k f_k b_k) = \sum_{i,k} a_i \Phi(e_i, f_k) b_k.
$$

If $(e_i)$ and $(f_k)$ are systems of generators of the modules $E$ and $F$, $\Phi$ is therefore completely determined by the elements $g_{ik} = \Phi(e_i, f_k)$. If $(e_i)$ and $(f_k)$ are bases of $E$ and $F$ and if elements $g_{ik}$ of $G$ ($i \in I, k \in K$) are given, then the formula

$$
\Phi(\sum_i a_i e_i, \sum_k f_k b_k) = \sum_{i,k} a_i g_{ik} b_k
$$

defines a mapping of $E \times F$ into $G$, which is bilinear and satisfies $\Phi(e_i, f_k) = g_{ik}$. When $(e_i)$ and $(f_k)$ are finite bases, we call $(\Phi(e_i, f_k))$ the matrix of $\Phi$ with respect to these bases.

The bilinear mappings of $E \times F$ into $G$ obviously form a subgroup of the additive group of mappings of $E \times F$ into $G$. On the other hand, let $a$ (resp. $b$) be an element of the center of $A$ (resp. $B$); then the mapping $a \Phi b$ of $E \times F$ into $G$ defined by $(a \Phi b)(x, y) = a . \Phi(x, y) . b$ is bilinear. The set of bilinear mappings of $E \times F$ into $G$ is thus endowed with a bimodule structure over the centers of $A$ and $B$.

Let E' (resp. F') be a left A-module (resp. a right B-module), u (resp. v) a homomorphism of E into E' (resp. of F into F') and $\Phi'$ a bilinear mapping of $E' \times F'$ into G. The *inverse image* of $\Phi'$ (relative to u and v) is called the bilinear mapping $\Phi$ of $E \times F$ into G defined by
$$
\Phi(x, y) = \Phi'(u(x), v(y)) \qquad (x \in E,\ y \in F).
$$
One readily verifies that
$$
d_{\Phi}(y) = d_{\Phi'}(v(y)) \circ u \qquad \text{and} \qquad s_{\Phi}(x) = s_{\Phi'}(u(x)) \circ v
$$
for all $x \in E,\ y \in F$.

Let $\Phi$ be a bilinear mapping of $E \times F$ into G, and h a homomorphism (for the structures of (A, B)-bimodules) of G into another (A, B)-bimodule $G'$. Then $h \circ \Phi$ is a bilinear mapping of $E \times F$ into $G'$.

### 2. Sesquilinear mappings.

In this No. unless expressly stated otherwise, A and B denote two rings, E a left A-module and F a *left* B-module; $b \to b^J$ ($b \in B$) denotes an *antiautomorphism* of B, that is, a bijection of B onto itself satisfying $(b + c)^J = b^J + c^J$ and $(bc)^J = c^J b^J$ for all $b,\ c$ in B; we shall write $J'$ instead of $J^{-1}$. G denotes an (A, B)-bimodule (No. 1).

#### Definition 4 {#alg-ix-s1-def-4 .statement}

*We say that a mapping $\Phi$ of $E \times F$ into G is right sesquilinear for J if it satisfies conditions (1), (2), (3) (def. 1, No. 1) as well as*
(7) $\Phi(x, by) = \Phi(x, y) \cdot b^J$ for all $x \in E,\ y \in F$ and $b \in B$.

If J is the identity (which requires that B be *commutative*), we recover the notion of a bilinear mapping.

Let $(e_i)_{i \in I}$ and $(f_k)_{k \in K}$ be two families of elements of E and F, and let $(a_i)_{i \in I}$ and $(b_k)_{k \in K}$ be elements of A and B which are zero except for a finite number of them. Then
$$
\Phi(\sum_i a_i e_i, \sum_k b_k f_k) = \sum_{i,k} a_i \Phi(e_i, f_k) b_k^J.
$$

As in the case of a bilinear mapping, the elements $\Phi(e_i, f_k)$ determine $\Phi$ uniquely when $(e_i)$ and $(f_k)$ are generating systems, and may be chosen arbitrarily when $(e_i)$ and $(f_k)$ are bases of E and F; when $(e_i)$ and $(f_k)$ are finite bases, $(\Phi(e_i, f_k))$ is called the matrix of $\Phi$ with respect to these bases.

As for bilinear mappings, one defines on the set of right sesquilinear mappings (for $J$) from $E \times F$ into $G$ a bimodule structure over the centres of $A$ and $B$. One defines the notion of inverse image of a sesquilinear mapping by the same formula as for a bilinear mapping. We shall moreover see that the study of sesquilinear mappings can be reduced to that of bilinear mappings.

#### Definition 5 {#alg-ix-s1-def-5 .statement}

Let $B$ be a ring, $F$ a $B$-module to the left (resp. to the right) and $J$ an antiautomorphism of $B$. We denote by $F^J$ the $B$-module to the right (resp. to the left) having the same underlying additive group as $F$ and in which the external composition law is $(b, y) \to b^{J'}y$ (resp. $(b, y) \to yb^{J'}$) $(b \in B,\ y \in F,\ J' = J^{-1})$.

With the notations of Definition 5, a linear mapping from $F^J$ into a $B$-module to the right (resp. to the left) $H$ is therefore identified with a $\mathbf{Z}$-linear mapping $u$ from $F$ into $H$ satisfying
$$
u(by) = u(y)b^J \quad \text{(resp. } u(yb) = b^Ju(y)) \quad (b \in B,\ y \in F).
$$

The mapping $u$ from $F$ into $H$ is a semilinear mapping from $F$ into $H$ relative to $J$ (chap. II, App. I, no 1), if one considers $J$ as an isomorphism of the ring $B^0$ opposite to $B$ onto $B$, and $F$ as a $B^0$-module to the right (resp. to the left).

Analogously a right sesquilinear mapping $\Phi$ (for $J$) from $E \times F$ into $G$, where $F$ is a $B$-module to the left, is identified with a bilinear mapping from $E \times F^J$ into $G$; if the latter is degenerate to the right (resp. degenerate to the left, non-degenerate), one says that $\Phi$ is degenerate to the right (resp. degenerate to the left, non-degenerate).

#### Remark {#alg-ix-s1-n2-rem-1 .statement}

Let $A$ and $B$ be two rings, $J_1$ an antiautomorphism of $A$, $M$ an $A$-module to the right, $N$ a $B$-module to the right and G a (A, B)-bimodule. One says that a mapping $\Phi$ from $M \times N$ into G is *left sesquilinear for $J_1$* if it is $\mathbf{Z}$-bilinear and if it satisfies

$$
\Phi(xa, yb) = a^{J_1} \Phi(x, y)b \quad (x \in M, y \in N, a \in A, b \in B).
$$

Such a mapping is identified with a bilinear mapping from $M^{J_1} \times N$ into G. We shall often leave to the reader the task of transposing to left sesquilinear mappings the definitions and properties given for right sesquilinear mappings; when we speak of a sesquilinear mapping (without further specification), it will be a right sesquilinear mapping.

### 3. Orthogonality. Direct sums of bilinear or sesquilinear mappings.

In this No., A and B denote rings, E a left A-module, F a right B-module (resp. a left B-module), G an (A, B)-bimodule, and $\Phi$ a bilinear mapping (resp. sesquilinear mapping for a given antiautomorphism J of B) of $E \times F$ into G.

#### Definition 6 {#alg-ix-s1-def-6 .statement}

*Two elements $x \in E$ and $y \in F$ are said to be orthogonal with respect to $\Phi$ if $\Phi(x, y) = 0$. Two subsets $E' \subset E$ and $F' \subset F$ are said to be orthogonal if, whatever $x \in E'$ and $y \in F'$, $x$ and $y$ are orthogonal. The set of elements of $E$ (resp. F) orthogonal to a given submodule N of F (resp. M of E) is a submodule of E (resp. F), called the totally orthogonal submodule (or simply orthogonal submodule) to N (resp. M), and denoted by $N^0$ (resp. $M^0$).*

Let H and $H'$ be two submodules of E or F. We have $H \subset (H^0)^0$ (denoted by $H^{00}$); if $H \subset H'$, we have ${H'}^0 \supset H^0$. It follows that we have $H^0 \supset (H^{00})^0$ and $H^0 \subset (H^0)^{00}$; on putting

$$
H^{000} = (H^{00})^0 = (H^0)^{00} = ((H^0)^0)^0,
$$

we therefore have $H^0 = H^{000}$.

For the mapping $\Phi$ to be degenerate (No. 1, Def. 3), it is necessary and sufficient that at least one of the two submodules $E^0, F^0$ be $\neq \{0\}$. It is clear that $\Phi(x, y)$ does not change when an element of $F^0$ (resp. $E^0$) is added to $x$ (resp. $y$), and $\Phi$ therefore defines by passing to the quotient a bilinear mapping (or sesquilinear mapping) on $(E/F^0) \times (F/E^0)$; this is plainly non-degenerate; it is called the non-degenerate bilinear mapping (or sesquilinear mapping) associated with $\Phi$.

Let $(E_i)_{i \in I}$ be a family of left A-modules, $(F_i)_{i \in I}$ a family of right B-modules (resp. left B-modules), and $\Phi_i$ a bilinear (resp. right J-sesquilinear) mapping of $E_i \times F_i$ into G. Let $E$ (resp. $F$) denote the direct sum module of the $E_i$ (resp. $F_i$). It is immediately seen that the mapping $\Phi$ of $E \times F$ into G defined by
$$
\Phi((x_i), (y_i)) = \sum_i \Phi_i(x_i, y_i) \quad (x_i \in E_i, y_i \in F_i)
$$
(the sum having a meaning since all but a finite number of its terms are zero) is bilinear (resp. right J-sesquilinear). It is called the direct sum of the mappings $\Phi_i$. It is clear that $E_i$ is orthogonal to $F_j$ with respect to $\Phi$ for $i \neq j$. Conversely, let $\Phi$ be a bilinear or sesquilinear mapping of $E \times F$ into G, and suppose that E is the direct sum of submodules $(E_i)_{i \in I}$ and F the direct sum of submodules $(F_i)_{i \in I}$ such that $E_i$ is orthogonal to $F_j$ for $i \neq j$; then $\Phi$ is the direct sum of its restrictions to the products $E_i \times F_i$ ($i \in I$).

For $\Phi$ to be non-degenerate, it is necessary and sufficient that each of the $\Phi_i$ be so; under these conditions, the submodule orthogonal to $E_i$ is $\sum_{j \neq i} F_j$.

### 4. Change of base rings.

In this no, let A, B, A', B' denote four rings, $h$ and $h'$ homomorphisms of A into A' and of B into B' respectively, G an (A, B)-bimodule, G' an (A', B')-bimodule, and $u$ a homomorphism of the underlying abelian group of G into the underlying abelian group of G', satisfying
$$
u(agb) = h(a)u(g)h'(b) \quad (a \in A, g \in G, b \in B).
$$

Let E (resp. F) be a left A-module (resp. right B-module). Recall (Chap. III, 2e éd., App. II, no 10) that, if $A'$ (resp. $B'$) is considered as a right $A$-module (resp. left $B$-module), the tensor product $E' = A' \otimes_A E$ (resp. $F' = F \otimes_B B'$) is endowed with a structure of left $A'$-module (resp. right $B'$-module) defined by

$$
a'_1(a' \otimes x) = (a'_1 a') \otimes x \quad (a', a'_1 \in A', x \in E)
$$
(resp. $(y \otimes b') b'_1 = y \otimes (b' b'_1)$ $(b', b'_1 \in B', y \in F)$).

#### Proposition 1 {#alg-ix-s1-prop-1 .statement}

*Let $E$ be a left $A$-module and $F$ a right $B$-module; put $E' = A' \otimes_A E$ and $F' = F \otimes_B B'$. For every bilinear mapping $\Phi$ of $E \times F$ into $G$, there exists one and only one bilinear mapping $\Phi'$ of $E' \times F'$ into $G'$ such that*

$$
\Phi'(a' \otimes x, y \otimes b') = a'.u(\Phi(x, y)).b'
$$

whatever $a' \in A'$, $b' \in B'$, $x \in E$, $y \in F$.

The uniqueness of $\Phi'$ follows from the fact that the elements $a' \otimes x$ and $y \otimes b'$ generate $E'$ and $F'$ respectively. To prove its existence, consider the mapping

$$
m : (a', x, y, b') \to a'.u(\Phi(x, y)).b'
$$

from $A' \times E \times F \times B'$ into $G$; it is obviously $\mathbf{Z}$-multilinear, and it satisfies

$$
m(a', ax, y, b') = m(a'h(a), x, y, b')
$$
and
$$
m(a', x, yb, b') = m(a', x, y, h'(b)b')
$$
$(a \in A, b \in B, a' \in A', b' \in B', x \in E, y \in F)$.

There therefore exists a $\mathbf{Z}$-bilinear mapping $\Phi'$ from $E' \times F'$ into $G'$ satisfying (13) (Chap. III, 2nd ed., App. II, No. 1, prop. 2). This relation and the definition of the module structures of $E'$ and $F'$ by (12) show that $\Phi'$ is bilinear, which completes the proof.

The hypotheses and notations being those of Proposition 1, let us now study the *associated linear mappings* of $\Phi$ and $\Phi'$ (No. 1, def. 2). For this purpose we shall first define a canonical homomorphism from $\mathcal{L}_A(E, G)$ into $\mathcal{L}_{A'}(E', G')$. For every $\nu \in \mathcal{L}_A(E, G)$ the mapping $(a', x) \to a'.u(\nu(x))$ from $A' \times E$ into $G'$ is $\mathbf{Z}$-bilinear, and, viewed (11), maps $(a'h(a), x)$ and $(a', ax)$ $(a \in A)$ onto the same element of $G'$; it therefore defines (Chap. III, 2nd ed.,

App. II, Nos. 1 and 10) a mapping $k(\nu)$ from $E' = A' \otimes_A E$ into $G'$ such that $k(\nu)(a' \otimes x) = a'.u(\nu(x))$, and which, viewed (12), is $A'$-linear. Moreover one immediately deduces from (12) that the mapping $\nu \to k(\nu)$ from $\mathcal{L}_A(E, G)$ into $\mathcal{L}_{A'}(E', G')$ satisfies $k(\nu b) = k(\nu)h'(b)$ for every $b \in B$. Let $i$ denote the canonical mapping $y \to y \otimes 1$ from $F$ into $F'$. Then the diagram

$$
\begin{array}{ccc}
F & \xrightarrow{d_\Phi} & \mathcal{L}_A(E, G) \\
|_i & & |_k \\
F' & \xrightarrow{d_{\Phi'}} & \mathcal{L}_{A'}(E', G')
\end{array}
$$

(where $d_\Phi$ and $d_{\Phi'}$ denote the right associated linear mappings to $\Phi$ and $\Phi'$) is *commutative*. Indeed, for $x \in E, y \in F$ and $a' \in A'$, we have $d_{\Phi'}(i(y))(a' \otimes x) = \Phi'(a' \otimes x, y \otimes 1) = a'.u(\Phi(x, y)) = a'.u(d_\Phi(y)(x))$, that is, $d_{\Phi'}(i(y))(a' \otimes x) = k(d_\Phi(y))(a' \otimes x)$. There is an analogous commutation relation for the left associated linear mappings $s_\Phi$ and $s_{\Phi'}$ to $\Phi$ and $\Phi'$.

#### Proposition 2 {#alg-ix-s1-prop-2 .statement}

*Suppose that B and B' are provided with anti-automorphisms J and I such that*

$$(15)$$
$$ h'(b^J) = h'(b)^I \quad \text{for tout } b \in B. $$

*Let E be a left A-module and F a left B-module; put $E' = A' \otimes_A E$ and $F' = B' \otimes_B F$. For every sesquilinear mapping (for J) $\Phi$ of $E \times F$ into $G$, there exists one and only one sesquilinear mapping (for I) $\Phi'$ of $E' \times F'$ into $G'$ such that*

$$(16)$$
$$ \Phi'(a' \otimes x, b' \otimes y) = a'.u(\Phi(x, y)).{b'}^I $$

*for all $a' \in A'$, $b' \in B'$, $x \in E$, $y \in F$.*

The uniqueness of $\Phi'$ follows from the fact that the tensor products $a' \otimes x$ and $b' \otimes y$ generate $E'$ and $F'$, respectively. To establish its existence, consider the mapping

$$ m : (a, x, b', y) \to a'.u(\Phi(x, y)).{b'}^I $$

from $A' \times E \times B' \times F$ into $G'$. It is obviously $\mathbf{Z}$-multilinear, and, in view of (11) and (15), satisfies $m(a', ax, b', y) = m(a'h(a), x, b', y)$ and $m(a', x, b', by) = a'.u(\Phi(x, y)).h'(b^J){b'}^I = m(a', x, b'h'(b), y)$ ($a \in A, b \in B, a' \in A', b' \in B', x \in E, y \in F$). There therefore exists a $\mathbf{Z}$-bilinear mapping $\Phi'$ of $E' \times F'$ into $G'$ satisfying (16) (chap. III, 2e éd., App. II, no 1, prop. 2). This relation, together with the definition of the module structures of E' and F' by (12), shows, in view of (15), that $\Phi'$ is sesquilinear for I, which completes the proof.

The most important examples of $(A', B')$-bimodules G', provided with $\mathbf{Z}$-linear mappings $u$ from G into G' satisfying (11), are the following:

1) We take for $G'$ the tensor product $A' \otimes_A G \otimes_B B'$ (chap. III, 2nd ed., App. II, No. 9) and for $u$ the mapping
$$
g \to 1 \otimes g \otimes 1 \qquad (g \in G)
$$
from G into G'. The pair $(G', u)$ thus defined is clearly *universal* in the following sense: for every (A', B')-bimodule $G'_1$ and every $\mathbf{Z}$-linear mapping $u_1$ of G into $G'_1$ satisfying the analogue of (11), there exists one and only one $\mathbf{Z}$-linear mapping $f$ of G' into $G'_1$ such that $f(a'g'b') = a'f(g')b'$ ($a' \in A'$, $g' \in G'$, $b' \in B'$; in other words $f$ is a homomorphism for the bimodule structures of G' and $G'_1$) and such that $u_1 = f \circ u$.

2) When $A = B = G$ (the structure of (A, A)-bimodule of A being defined by the left and right homotheties), $A' = B'$, and $h = h'$ one can take for G' the ring $A'$ and for $u$ the homomorphism $h$ of A into $A'$.

3) Suppose that $A = B$, $A' = B'$, $h = h'$, that the rings A and A' are *commutative*, and that the structure of left A-module of G coincides with its structure of right A-module. One can then take for G' the tensor product $A' \otimes_A G$ (the structure of right A'-module of G' coinciding with its structure of left A'-module) and for $u$ the mapping $g \to 1 \otimes g$ ($g \in G$) from G into G'. We shall then say that the bilinear mapping (resp. sesquilinear mapping) $\Phi'$ defined by prop. 1 (resp. prop. 2) is obtained from $\Phi$ *by extension of the base ring*, or *by extension of scalars*.

The following is valid equally for bilinear mappings and for sesquilinear mappings; the hypotheses and notations are those of prop. 1 (resp. prop. 2). Given a submodule M of E or F, we shall denote by M' the submodule of E' or F' generated by the canonical image of M.

#### Proposition 3 {#alg-ix-s1-prop-3 .statement}

The hypotheses and notations being those of prop. 1 (resp. prop. 2) suppose in addition that A, B, A', B' are fields and that the mappings α and β of $A' \otimes_A G$ and $G \otimes_B B'$ into G' characterized by $\alpha(a' \otimes g) = a'u(g)$ and $\beta(g \otimes b') = u(g)b'$ ($a' \in A'$, $b' \in B'$, $g \in G$) are injective. Let M be a subspace of E and N a subspace of F. Then the subspace $(M')^0$ of F' orthogonal to M' with respect to $\Phi'$ is equal to $(M^0)',$ and, analogously, one has $(N')^0 = (N^0)'$.

Indeed the inclusions $(M^0)' \subset (M')^0$ and $(N^0)' \subset (N')^0$ are evident (and moreover true without hypotheses on A, B, A', B', $\alpha$ or $\beta$). We shall prove the inclusion $(M')^0 \subset (M^0)'$; we leave to the reader the verification of the inclusion $(N')^0 \subset (N^0)'$, which is quite analogous. Let $y'$ be an element of $(M')^0$. One can write

$$
y' = \sum_{i=1}^s y_i \otimes b'_i \quad \text{(resp. } y' = \sum_{i=1}^s b'_i \otimes y_i)
$$

where $y_i \in F$ ($1 \leq i \leq s$), and where the $b'_i$ are elements of B' which are linearly independent over B for the structure of left B-module (resp. right B-module) of B'. Let $x \in M$ and $x' = 1 \otimes x \in M'$. We have

$$
0 = \Phi'(x', y') = \sum_i u(\Phi(x, y_i)) b'_i = \beta(\sum_i \Phi(x, y_i) \otimes b'_i)
$$
(resp. $0 = \Phi'(x', y') = \sum_i u(\Phi(x, y_i)) {b'}^I_i = \beta(\sum_i \Phi(x, y_i) \otimes {b'}^I_i)$.

Comme $\beta$ is injective and the $b'_i$ (resp. the ${b'}^I_i$, taking account of (15)) are linearly independent over B for the structure of left B-module of B', this implies $\Phi(x, y_i) = 0$ for $i = 1, \ldots, s$. Since this last relation is true for all $x \in M$, we have $y_i \in M^0$ for $i = 1, \ldots, s$, whence $y' \in (M^0)'$. QED.

#### Corollary {#alg-ix-s1-n4-cor-1 .statement}

The hypotheses and notations being those of Prop. 3, in order that $\Phi'$ be non-degenerate, it is necessary and sufficient that $\Phi$ be non-degenerate.

Indeed, by Prop. 3, we have $(F')^0 = (F^0)'$ and $(E')^0 = (E^0)'$. On the other hand, in order that $\Phi$ (resp. $\Phi'$) be non-degenerate, it is necessary and sufficient that one have $F^0 = E^0 = \{0\}$ (resp. $(F')^0 = (E')^0 = \{0\}$).

#### Remark {#alg-ix-s1-n4-rem-1 .statement}

Suppose that A, B, A' and B' are fields. Then, for the bimodules G' defined in the three examples above, the mappings $\alpha$ and $\beta$ are injective, as follows immediately from Chap. III, 2nd ed., App. II, No. 6.

### 5. Some identities.

In this No., let A denote a ring endowed with an antiautomorphism J, E a left A-module, G an (A, A)-bimodule, and $\Phi$ a sesquilinear mapping (on the right) for J from $E \times E$ into G. Put $Q(x) = \Phi(x, x)$ ($x \in E$). One has obviously

$$
\begin{align*}
(17) \quad & Q(x + y) = Q(x) + \Phi(x, y) + \Phi(y, x) + Q(y) \\
(18) \quad & Q(x - y) = Q(x) - \Phi(x, y) - \Phi(y, x) + Q(y)
\end{align*}
$$

for any $x, y$ in E. Hence, by subtraction,

$$
(19) \quad 2(\Phi(x, y) + \Phi(y, x)) = Q(x + y) - Q(x - y).
$$

Let $a$ be an element of A; replacing $y$ by $ay$ in (19), one obtains

$$
(20) \quad 2(\Phi(x, y)a^j + a\Phi(y, x)) = Q(x + ay) - Q(x - ay).
$$

We deduce from (19) and (20), by multiplying (19) by $a$ (on the left) and subtracting:

$$
\begin{align*}
(21) \quad & 2(a\Phi(x, y) - \Phi(x, y)a^j) \\
& \quad = aQ(x + y) - aQ(x - y) - Q(x + ay) + Q(x - ay).
\end{align*}
$$

Suppose in particular that A is a quadratic extension $K(i)$ of a commutative ring K, with $i^2 = -1$ (Chap. II, § 7, No. 7), that J is the K-automorphism $u + iv \to u - iv$ ($u, v$ in K) of A, and that the left A-module and right A-module structures of G coincide. Taking $a = i$ in (21), one obtains

$$
(22) \quad 4\Phi(x, y) = Q(x + y) - Q(x - y) + iQ(x + iy) - iQ(x - iy).
$$

### 6. Bilinear and sesquilinear forms. Rank.

In this No., let A denote a ring (resp. a ring endowed with an antiautomorphism J), E a left A-module, and F a right A-module (resp. left A-module). We endow A with the structure of (A, A)-bimodule defined by left homotheties and right homotheties. In this case a bilinear mapping (resp. right sesquilinear mapping for J) from E × F into the bimodule A is called a bilinear form (resp. right sesquilinear form for J) on E × F.

When E = F (which implies that it is a sesquilinear form), one often says that a sesquilinear form on E × F is a sesquilinear form on E.

Given two left A-modules E and E′, and two sesquilinear forms Φ and Φ′ for J on E and E′ respectively, we say that Φ and Φ′ are equivalent if there exists an isomorphism u of the A-module E onto the A-module E′ such that Φ′(u(x), u(y)) = Φ(x, y) for all x, y in E; then Φ is the inverse image of Φ′ relative to u and u, and Φ′ is the inverse image of Φ relative to u^{-1} and u^{-1} (No. 2).

Let Φ be a bilinear form on E × F (F denoting a right A-module). The linear mappings s_{Φ} and d_{Φ} associated with Φ (No. 1, Def. 2) are then mappings from E into the dual F* of F, and from F into the dual E* of E.

By definition therefore

$$
\Phi(x, y) = \langle x, d_{Φ}(y) \rangle = \langle y, s_{Φ}(x) \rangle.
$$

We shall now define the linear mappings associated with a sesquilinear form. Let J be an antiautomorphism of A and Φ a sesquilinear form (on the right) for J on E × F (F denoting a left A-module); put J′ = J^{-1}. The mapping Φ′ from F × E into A defined by

$$
Φ′(y, x) = Φ(x, y)^{J′} \quad (x ∈ E, y ∈ F)
$$

is, as one easily sees, a sesquilinear form (on the right) for J′ on F × E. According to No. 2 (Def. 5) the sesquilinear forms Φ and Φ′ are identified respectively with bilinear forms on E × F^{J′} and on F × E^{J′}. The mappings d_{Φ} and d_{Φ′} associated with the latter are called the right and left associated mappings to the sesquilinear form $\Phi$, and are denoted by $d_\Phi$ and $s_\Phi$. We therefore have, by definition:

$$
(24)\quad \Phi(x, y) = \langle x, d_\Phi(y) \rangle = \langle y, s_\Phi(x) \rangle^J \qquad (x \in E,\ y \in F).
$$

Thus $d_\Phi$ (resp. $s_\Phi$) is a linear mapping from $F^J$ into $E^*$ (resp. from $E^{J'}$ into $F^*$), or again a semilinear mapping from $F$ into $E^*$ (resp. from $E$ into $F^*$) relative to $J$ (resp. $J'$) if $J$ (resp. $J'$) is considered as an isomorphism of the ring $A^0$ (opposite of $A$) onto $A$, and $F$ (resp. $E$) as a right $A^0$-module.

Formula (24) and Def. 6 of No. 3 immediately imply that for every submodule $N$ of $F$ (resp. $M$ of $E$), one has

$$
(25)\quad N^0 = s_\Phi^{-1}(N') \qquad (\text{resp. } M^0 = d_\Phi^{-1}(M'))
$$

where $N'$ (resp. $M'$) is the submodule of the dual $F^*$ of $F$ (resp. of the dual $E^*$ of $E$) orthogonal to $N$ (resp. $M$) (Chap. II, § 4, No. 2).

#### Proposition 4 {#alg-ix-s1-prop-4 .statement}

*Suppose that $A$ is a field, and let $\Phi$ be a bilinear form (resp. sesquilinear form for $J$) on $E \times F$; for $E/F^0$ to be of finite dimension, it is necessary and sufficient that $F/E^0$ be of finite dimension, and these dimensions are then equal.*

Indeed, let $\Phi_1$ be the non-degenerate form associated with $\Phi$, on $(E/F^0) \times (F/E^0)$ (No. 3). Suppose that $E/F^0$ is of finite dimension $n$; since the linear mapping $d_{\Phi_1}$ from $F/E^0$ (resp. $(F/E^0)^J$) into $(E/F^0)^*$ is injective, $F/E^0$ is of finite dimension $n' \leq n$; considering $s_{\Phi_1}$, we see similarly that $n \leq n'$.

#### Corollary 1 {#alg-ix-s1-prop-4-cor-1 .statement}

*Suppose that $A$ is a field and that $\Phi$ is non-degenerate. For a subspace $M$ of $E$ to be of finite dimension, it is necessary and sufficient that $M^0$ be of finite codimension in $F$, and one then has $\operatorname{codim} M^0 = \dim M$, and $M^{00} = M$.*

Comme $F^0 = \{0\}$, the first two assertions result from prop. 4 applied to the restriction of $\Phi$ to $M \times F$. Moreover, $M^0$ is the orthogonal of $M^{00}$, hence $M^{00}$ is of finite dimension equal to $\operatorname{codim} M^0 = \dim M$; but since $M^{00} \supset M$, we have $M^{00} = M$.

#### Corollary 2 {#alg-ix-s1-prop-4-cor-2 .statement}

*The hypotheses being those of cor. 1, let $M, N$ be two subspaces of $E$; then one has $(M + N)^0 = M^0 \cap N^0$; if moreover $M$ and $N$ are of finite dimension, one has $(M \cap N)^0 = M^0 + N^0$.*

The first assertion is trivial. Suppose that M and N are of finite dimension, and let G = M^0 + N^0; one has G^0 = M^{00} \cap N^{00} = M \cap N according to cor. 1; the prop. 4 applied to the restriction of $\Phi$ to $M \times G$ then shows (since $M^0 \subset G$ and $G^0 \subset M$) that one has $\dim M/(M \cap N) = \dim G/M^0 = \operatorname{codim} M^0 - \operatorname{codim} G$, and since $\operatorname{codim} M^0 = \dim M$, one deduces $\dim (M \cap N) = \operatorname{codim} G$. But one also has $\dim (M \cap N) = \operatorname{codim} (M \cap N)^0$ according to cor. 1, and since $G \subset G^{00} = (M \cap N)^0$ one has $G = (M \cap N)^0$.

Prop. 4 permits one to give the following definition:

#### Definition 7 {#alg-ix-s1-def-7 .statement}

Let A be a field (resp. a field endowed with an antiautomorphism J), E a left vector space over A, F a right (resp. left) vector space over A, and $\Phi$ a bilinear (resp. sesquilinear for J) form on $E \times F$. Suppose that $E/F^0$ and $F/E^0$ are of finite dimension over A. The rank of $\Phi$ is called the common (finite) dimension of the vector spaces $E/F^0$ and $F/E^0$.

When $E/F^0$ and $F/E^0$ are of infinite dimension, one says that $\Phi$ is of infinite rank.

#### Proposition 5 {#alg-ix-s1-prop-5 .statement}

The hypotheses and notations being those of def. 7, the linear mappings $s_\Phi$ and $d_\Phi$ associated with $\Phi$ have the same rank, and this rank is equal to the rank of the form $\Phi$.

Indeed the kernel of the mapping $d_\Phi$ from F into $E^*$ is obviously $E^0$, hence its rank is equal to the dimension of $F/E^0$. Analogously the rank of $s_\Phi$ is equal to the dimension of $E/F^0$.

#### Proposition 6 {#alg-ix-s1-prop-6 .statement}

The hypotheses and notations being those of def. 7, suppose in addition that E and F have the same finite dimension. Then the following conditions are equivalent:
a) $d_\Phi$ is injective ;
b) $d_\Phi$ is surjective ;
c) $s_\Phi$ is injective ;
d) $s_\Phi$ is surjective ;
e) $\Phi$ is non-degenerate.

Indeed, since E, F, $E^*$ and $F^*$ have the same finite dimension,

a) and b) are equivalent, as are c) and d) (chap. II, § 3, no 4). Since $s_\Phi$ and $d_\Phi$ have the same rank (prop. 5), a) and c) are equivalent. Since e) is equivalent to the relation $E^0 = F^0 = \{0\}$, it is equivalent to the conjunction of a) and c), whence the equivalence of the stated conditions.

#### Corollary {#alg-ix-s1-n6-cor-1 .statement}

The hypotheses and notations being those of Definition 7, we suppose in addition that E is of finite dimension and that $\Phi$ is non degenerate. Then we have $\dim E = \dim F$ and, for every basis $(e_i)$ ($1 \leq i \leq \dim E$) of E, there exists a basis $(f_i)$ of F such that $\Phi(e_i, f_k) = \delta_{ik}$ ($i, k = 1, ..., \dim E$).

Indeed, since $\Phi$ is non degenerate, we have $E^0 = F^0 = \{0\}$, whence $\dim E = \dim F$ (prop. 4). It follows (prop. 6) that $d_\Phi$ is an isomorphism of F (resp. $F^j$) onto $E^*$; therefore, if $(e_i^*)$ is the dual basis of $(e_i)$, the elements $f_i = d_\Phi^{-1}(e_i^*)$ form a basis of F which, in view of formula (23) (resp. formula (24)), satisfies $\Phi(e_i, f_k) = \delta_{ik}$.

It is immediate that, in this corollary, one can exchange the roles of E and of F, replacing $d_\Phi$ by $s_\Phi$ in the proof.

#### Remark {#alg-ix-s1-n6-rem-1 .statement}

Let A be a ring endowed with an antiautomorphism J, M and N right A-modules, and $\Phi$ a left sesquilinear form for J on $M \times N$ (No. 2, Remark); it therefore satisfies the equality

$$
\Phi(xa, xa') = a^j \Phi(x, y)a' \quad (a, a' \in A, x \in M, y \in N).
$$

The mapping $\Phi'$ of $N \times M$ into A defined by $\Phi'(y, x) = \Phi(x, y)^{J'}$ (where $J' = J^{-1}$) is a left sesquilinear form for $J'$, and $\Phi$ and $\Phi'$ identify with bilinear forms on $M^{J'} \times N$ and $N^{J'} \times M$ respectively. The mappings $s_\Phi$ and $s_{\Phi'}$ associated with these bilinear forms are called the left and right associated mappings to the sesquilinear form $\Phi$, and are denoted by $s_\Phi$ and $d_\Phi$. Thus, by definition

$$(26)$$
$$
\Phi(x, y) = \langle y, s_\Phi(x) \rangle = \langle x, d_\Phi(y) \rangle^j \quad (x \in M, y \in N),
$$

and $s_\Phi$ (resp. $d_\Phi$) is a linear mapping of $M^{J'}$ into $N^*$ (resp.

of $N'$ into $M^*$). One would state and prove easily the analogues, for the case considered here, of Definition 7 and of props. 4, 5, 6.

### 7. Inverse form of a bilinear or sesquilinear form.

Let $A$ be a ring, $E$ a left $A$-module, $F$ a right $A$-module and $\Phi$ a bilinear form on $E \times F$. We suppose here that the mappings associated with $\Phi$, which will be denoted by $s$ and $d$, are *bijective*. Then the product mapping $(s, d)$ is a bijection of $E \times F$ onto $F^* \times E^*$, and defines, by transport of structure, a bilinear form $\hat{\Phi}$ on $F^* \times E^*$. The latter therefore satisfies

$$
(27)\quad \hat{\Phi}(y', x') = \Phi(s^{-1}(y'), d^{-1}(x')) \\
= \langle s^{-1}(y'), x' \rangle = \langle d^{-1}(x'), y' \rangle \qquad (x' \in E^*, y' \in F^*).
$$

#### Definition 8 {#alg-ix-s1-def-8 .statement}

*Let $\Phi$ be a bilinear form on $E \times F$ whose associated mappings $s$ and $d$ are bijective. The bilinear form $\hat{\Phi}$ on $F^* \times E^*$ defined by (27) is called the inverse form of $\Phi$.*

Let now $\hat{s}$ and $\hat{d}$ be the linear mappings from $F^*$ into $E^{**}$ and from $E^*$ into $F^{**}$ associated on the left and on the right with $\hat{\Phi}$. Since, for $x' \in E^*$ and $y' \in F^*$, one has by definition

$$
\hat{\Phi}(y', x') = \langle y', \hat{d}(x') \rangle = \langle x', \hat{s}(y') \rangle
$$

one sees, by comparing with (27), that the linear form $\hat{d}(x')$ on $F^*$ is equal to that defined by the element $d^{-1}(x')$ of $F$. It follows that the composed mapping $\hat{d} \circ d$ is the canonical mapping of $F$ into its bidual $F^{**}$, and that this mapping is *bijective* since $d$ and $\hat{d}$ (the latter by transport of structure) are bijective; therefore, if one identifies canonically $F$ with $F^{**}$, one has $\hat{d} = d^{-1}$. Analogously $E$ is identified canonically with $E^{**}$, the canonical mapping of $E$ into $E^{**}$ is $\hat{s} \circ s$, and one has $\hat{s} = s^{-1}$. It follows from this that the inverse form of $\hat{\Phi}$ is $\Phi$.

Consider now a ring $A$ endowed with an antiautomorphism $J$, two left $A$-modules $E$ and $F$, and a right sesquilinear form $\Phi$ for $J$ on $E \times F$ such that the mappings associated with $\Phi$, which will be denoted by $s$ and $d$, are *bijective*. Define a mapping $\widehat{\Phi}$ from $F^* \times E^*$ into $A$ by the first equation (27). This mapping satisfies, by (24) (No. 6), the relation

$$
(28)\quad \widehat{\Phi}(y', x') = \langle s^{-1}(y'), x' \rangle = \langle d^{-1}(x'), y' \rangle^J \qquad (x' \in E^*,\ y' \in F^*).
$$

The mapping $\widehat{\Phi}$ is obviously $\mathbf{Z}$-bilinear; moreover, one has, for $a,\ b$ in $A$, $x' \in E^*$ and $y' \in F^*$, and by virtue of the definitions of $s$ and $d$,

$$
\widehat{\Phi}(y'a,\ x'b) = \Phi(a^j s^{-1}(y'),\ b^{j'} d^{-1}(x')) = a^j \widehat{\Phi}(y',\ x') b;
$$

hence $\widehat{\Phi}$ is a *left sesquilinear form* for $J$ on $F^* \times E^*$ (No. 2).

#### Definition 9 {#alg-ix-s1-def-9 .statement}

*Let $\Phi$ be a right sesquilinear form for $J$ on $E \times F$, whose associated mappings $s$ and $d$ are bijective. The left sesquilinear form $\widehat{\Phi}$ for $J$ on $F^* \times E^*$ is called the inverse form of $\Phi$.*

We leave it to the reader to define and study the inverse form of a left sesquilinear form. This inverse form is a right sesquilinear form.

Let $\widehat{s}$ and $\widehat{d}$ be the mappings associated with $\widehat{\Phi}$; according to (26) (No. 6) we have

$$
(29)\quad \widehat{\Phi}(y', x') = \langle y',\ \widehat{d}(x') \rangle^J = \langle x',\ \widehat{s}(y') \rangle.
$$

Since $s$ is bijective, and from the equality $\langle s^{-1}(y'),\ x' \rangle = \langle y',\ \widehat{d}(x') \rangle^J$ which follows from (28) and (29), we deduce that $\widehat{d}$ is bijective; hence $\widehat{d} \circ d$ is bijective. Now the equality $\langle d^{-1}(x'),\ y' \rangle = \langle y',\ \widehat{d}(x') \rangle$, which follows from (28) and (29), shows that $\widehat{d} \circ d$ is the canonical mapping from $F$ into its bidual $F^{**}$. One sees analogously that $\widehat{s}$ is bijective and that $\widehat{s} \circ s$ is the canonical mapping from $E$ into $E^{**}$. Hence, if one identifies $E^{**}$ with $E$ and $F^{**}$ with $F$ by means of these canonical mappings, one has $\widehat{s} = s^{-1},\ \widehat{d} = d^{-1}$, and $\Phi$ is the inverse form of $\widehat{\Phi}$.

With the same notation and hypotheses let $a$ be an invertible element of the center of $A$. Then the associated mappings of the form $a\Phi$ are, according to (23) (resp. (24)) equal to $a.d$ and $a.s$ (resp. $a^{J'}.s$), and are therefore bijective. It follows thus from (27) that the inverse form of $a\Phi$ is $a^{-1}\widehat{\Phi}$ (resp. $(a^{J'})^{-1}\widehat{\Phi}$).

### 8. Adjoint of a homomorphism.

In this No., $A$ denotes an anneau (resp. an anneau endowed with an antiautomorphism $J$), $E$ and $E'$ two left $A$-modules, $F$ and $F'$ two right $A$-modules (resp. left), and $\Phi$ and $\Phi'$ two bilinear forms (resp. sesquilinear forms for $J$) on $E \times F$ and $E' \times F'$ respectively. It is assumed that $\Phi$ is non-degenerate, in other words (No. 1) that the linear mappings $d_{\Phi}$ and $s_{\Phi}$ associated with $\Phi$ are injective.

Given a homomorphism $u$ from E into E’, consider the set $F'_1$ of the elements $y'$ of $F'$ such that there exists $y \in F$ for which one has $d_{\Phi'}(y') \circ u = d_{\Phi}(y)$, that is to say $\Phi'(u(x), y') = \Phi(x, y)$ for all $x \in E$. It is clear that $F'_1$ is a submodule of $F'$. Since $d_{\Phi}$ is injective, there exists, for every $y' \in F'_1$, one and only one element $y$ of F such that $\Phi'(u(x), y') = \Phi(x, y)$. The mapping $y' \to y$ from $F'_1$ into F thus defined is A-linear; denoting it by $u^*$, one has, for all $x \in E$ and all $y \in F'_1$

$$
\Phi'(u(x), y') = \Phi(x, u^*(y')).
$$

#### Definition 10 {#alg-ix-s1-def-10 .statement}

The hypotheses and notations being as previously, one says that the homomorphism $u^*$ from $F'_1$ into F satisfying (30) is the left adjoint of $u$, and that $F'_1$ is the defining submodule of $u^*$.

The right adjoint of a homomorphism $\varphi$ from F into $F'$ is defined analogously by the formula

$$
\Phi'(x', \varphi(y)) = \Phi(\varphi^*(x'), y) \quad (x' \in E'_1, y \in F),
$$

where $E'_1$ denotes the submodule of $E'$ defined analogously to $F'_1$.

#### Remark {#alg-ix-s1-n8-rem-1 .statement}

If the left adjoint $u^*$ of $u : E \to E'$ is everywhere defined, and if $s_{\Phi'}$ and $d_{\Phi'}$ are injective, formula (30) shows that $u$ is the right adjoint of $u^*$.

It follows from (30) that, if $u_1$ and $u_2$ are two homomorphisms from $E$ into $E'$ admitting everywhere defined adjoints, and if $c$ is an element of the center of $A$, one has

$$
\begin{cases}
(u_1 + u_2)^* = u_1^* + u_2^* ; 1^* = 1 ; \\
(cu_1)^* = c . u_1^* \text{ when } \Phi \text{ and } \Phi' \text{ are bilinear ;} \\
(cu_1)^* = c^{j'} . u_1^* \text{ when } \Phi \text{ and } \Phi' \text{ are sesquilinear.}
\end{cases}
$$

Moreover, if $E''$ is a third $A$-left module, $F''$ a third $A$-right module (resp. left module), $\Phi''$ a bilinear form (resp. sesquilinear for $J$) on $E'' \times F''$, and if $u'$ is a homomorphism from $E'$ into $E''$ admitting an everywhere defined (left) adjoint, one has

$$(u' \circ u)^* = u^* \circ {u'}^*.$$

In particular, if $u$ is an *isomorphism* of $E$ onto $E'$, and if the adjoints $u^*$ and $(u^{-1})^*$ are everywhere defined, $u^*$ is an isomorphism of $F'$ onto $F$, and one has $(u^*)^{-1} = (u^{-1})^*$. Analogous properties for right adjoints.

#### Proposition 7 {#alg-ix-s1-prop-7 .statement}

With the same notations as previously, suppose that $d_{\Phi}$ is bijective. Then every homomorphism $u$ of $E$ into $E'$ admits an everywhere defined left adjoint, and one has $u^* = (d_{\Phi})^{-1} \circ {}^t u \circ d_{\Phi'}$.

Indeed, since $d_{\Phi}$ is bijective, one has, with the notations of the beginning of the No., $F'_1 = F'$, and $u^*$ is therefore everywhere defined. On the other hand (30) is equivalent to

$$\langle u(x), d_{\Phi'}(y') \rangle = \langle x, (d_{\Phi} \circ u^*)(y') \rangle \quad (x \in E, y' \in F');$$

now $\langle d_{\Phi'}(y'), u(x) \rangle = \langle {}^t u(d_{\Phi'}(y')), x \rangle$; hence one has ${}^t u(d_{\Phi'}(y')) = d_{\Phi}(u^*(y'))$ for all $y' \in F'$, whence ${}^t u \circ d_{\Phi'} = d_{\Phi} \circ u^*$, and consequently the announced expression for $u^*$. Q.E.D.

#### Remark {#alg-ix-s1-n8-rem-2 .statement}

When $s_{\Phi}$ is bijective, every homomorphism $\nu$ of $F$ into $F'$ admits an everywhere defined right adjoint, and one has

$$(34)$$
$$\nu^* = (s_{\Phi})^{-1} \circ {}^t \nu \circ s_{\Phi'}.$$

#### Proposition 8 {#alg-ix-s1-prop-8 .statement}

With the same notations as previously, suppose that $s_{\Phi}$ and $d_{\Phi}$ are bijective. Let $u$ and $\nu$ be isomorphisms of E onto E' and of F onto F' respectively. Then, in order that Φ be the inverse image of Φ' relative to u and v (that is to say that one have Φ(x, y) = Φ'(u(x), v(y)) whatever x ∈ E, y ∈ F may be), it is necessary and sufficient that one have u^{-1} = v^* and v^{-1} = u^*.

Indeed Φ'(u(x), v(y)) = Φ(x, y) may also be written Φ (x, u^*(v(y))) = Φ(x, y). If this holds whatever x ∈ E and y ∈ F may be, one has u^* ∘ v = 1 since Φ is non-degenerate. One therefore also has v^* ∘ u = 1 by (33). The converse is immediate.

#### Corollary {#alg-ix-s1-n8-cor-1 .statement}

Let A be a ring endowed with an antiautomorphism J, E a left A-module, Φ a sesquilinear form for J on E × E whose associated mappings are bijective, and u an automorphism of the A-module E. In order that u leave Φ invariant (that is to say that one have Φ(u(x), u(y)) = Φ(x, y) whatever x, y in E may be), it is necessary and sufficient that the two adjoints of u be equal and that one have u^* = u^{-1}.

This follows at once from prop. 8.

#### Remark {#alg-ix-s1-n8-rem-3 .statement}

Under the hypotheses of the cor. of prop. 8, suppose in addition that A be a field and that E be of finite dimension over A. Let ω be an endomorphism of E, ω_1 and ω_2 its right and left adjoints. Each of the conditions ωω_1 = 1, ωω_2 = 1, ω_1ω = 1, ω_2ω = 1 entails that ω is an automorphism of E leaving Φ invariant, and that ω_1 = ω_2.

### 9. Tensor products and exterior powers of sesquilinear forms.

In this No., A will denote a commutative ring. A bilinear form on a product of two A-modules is therefore a particular case of a sesquilinear form. We shall denote by J an automorphism of A, and by J' its inverse.

Let E_i (i = 1, ..., m) be A-modules. The mapping

$$(x_1, ..., x_m) \to x_1 \otimes \cdots \otimes x_m$$

of $\prod_{i=1}^m E_i^J$ into $(\bigotimes_{i=1}^m E_i)^J$ (x_i \in E_i^J) (cf. déf. 5, n° 2) is obviously A-multilinear; it therefore defines (chap. III, § 1, n° 7) an A-linear mapping $f$ of $\bigotimes_i E_i^j$ into $(\bigotimes_i E_i)^j$; this mapping transforms $x_1 \otimes \cdots \otimes x_m$ (where the signs $\otimes$ denote the tensor products in $\bigotimes_i E_i^j$) into $x_1 \otimes \cdots \otimes x_m$ (where the signs $\otimes$ denote the tensor products in $(\bigotimes_i E_i)^j$). Thus $f$ is an isomorphism of $\bigotimes_i E_i^j$ onto $(\bigotimes_i E_i)^j$. We shall identify these two modules by means of this isomorphism.

Similarly let $E$ be an A-module. The mapping
$$
(x_1, \ldots, x_m) \to x_1 \wedge \ldots \wedge x_m
$$
of $(E^j)^m$ into $(\wedge^m E)^j$ is obviously A-multilinear and alternating. It therefore defines an A-linear mapping $f$ of $\wedge^m E^j$ into $(\wedge^m E)^j$, which is obviously an isomorphism. We shall identify $\wedge^m E^j$ and $(\wedge^m E)^j$ by means of this isomorphism.

Let $x'$ be an element of the dual $E^*$ of $E$. The mapping $x \to \langle x, x' \rangle^j$ ($x \in E$) is an element ${x'}^j$ of $(E^j)^*$, and it is immediate that $x' \to {x'}^j$ is a bijection $g$ of $E^*$ onto $(E^j)^*$ satisfying $g(ax') = a^j g(x')$ for all $a \in A$. Consequently the composite mapping of $g$ and the identity mapping of $(E^*)^j$ onto $E^*$ is an isomorphism of $(E^*)^j$ onto $(E^j)^*$. We shall identify these modules by means of this isomorphism, and shall denote them by $E_j^*$.

Let $E_i, F_i \ (i = 1, \ldots, m)$ be A-modules, and $\Phi_i \ (i = 1, \ldots, m)$ a sesquilinear form for $J$ on $E_i \times F_i$. The mapping
$$
(x_1, \ldots, x_m, y_1, \ldots, y_m) \to \Phi_1(x_1, y_1) \Phi_2(x_2, y_2) \ldots \Phi_m(x_m, y_m)
$$
$(x_i \in E_i, y_i \in F_i, i = 1, \ldots, m)$ is an A-multilinear mapping of $E_1 \times \cdots \times E_m \times F_1^j \times \cdots \times F_m^j$ into $A$, and therefore defines a bilinear form on $(\bigotimes_i E_i) \times (\bigotimes_i F_i^j)$ (Chap. III, § 1, No. 7). Since the second factor has been identified with $(\bigotimes_i F_i)^j$, we have therefore defined a sesquilinear form $\Phi$ for $J$ on $(\bigotimes_i E_i) \times (\bigotimes_i F_i)$. This form is characterized by
$$
\Phi(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \prod_{i=1}^m \Phi_i(x_i, y_i) \quad (x_i \in E_i, y_i \in F_i).
$$

#### Definition 11 {#alg-ix-s1-def-11 .statement}

Given A-modules $E_i, F_i (i = 1, \ldots, m)$ and, for each $i$, a sesquilinear form $\Phi_i$ for $J$ on $E_i \times F_i$, the sesquilinear form $\Phi$ for $J$ on $(\bigotimes_i E_i) \times (\bigotimes_i F_i)$ characterized by (35) is called the tensor product of the sesquilinear forms $\Phi_i$.

In the case where the $E_i$ and the $F_i$ are equal to one and the same module $E$, and where the $\Phi_i$ are equal to one and the same form $\Psi$, we say that $\Phi$ is the extension of $\Psi$ to $\bigotimes^m E$.

With the notations of Def. 11, let us study the mappings associated with $\Phi$. From formula (24) (No. 6) and from (35) one obtains the relation

$$
\Phi(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \prod_{i=1}^m \langle x_i, d_{\Phi_i}(y_i) \rangle = \prod_{i=1}^m \langle y_i, s_{\Phi_i}(x_i) \rangle^J.
$$

We have therefore:

(36) $s_\Phi = j_s \circ (s_{\Phi_1} \otimes \cdots \otimes s_{\Phi_m}), \quad d_\Phi = j_d \circ (d_{\Phi_1} \otimes \cdots \otimes d_{\Phi_m})$

where $j_s$ (resp. $j_d$) denotes the canonical mapping of $\bigotimes_i F_i^*$ into $(\bigotimes_i F_i)^*$ (resp. of $\bigotimes_i E_i^*$ into $(\bigotimes_i E_i)^*$) (Chap. III, § 1, Nos. 4 and 7).

#### Proposition 9 {#alg-ix-s1-prop-9 .statement}

Let $A$ be a commutative field endowed with an automorphism $J$, $E_i, F_i$ finite-dimensional vector spaces over $A$, and $\Phi_i$ a sesquilinear form for $J$ on $E_i \times F_i$ ($1 \leqslant i \leqslant m$). If the forms $\Phi_i$ are non-degenerate, the same is true of their tensor product $\Phi$. In this case the inverse form $\widehat{\Phi}$ of $\Phi$ is the tensor product of the inverse forms $\widehat{\Phi}_i$.

Indeed, since $A$ is a field, it follows from props. 6 and 7 of chap. III, § 1, no. 3 that a tensor product of injective (resp. surjective) linear mappings of $A$-modules is an injective (resp. surjective) linear mapping. Since the $s_{\Phi_i}$ are bijective by assumption (prop. 6, no. 6), the same is therefore true of their tensor product. On the other hand the canonical mapping $j_s$ of $\bigotimes_i F_i^*$ into $(\bigotimes_i F_i)^*$ is bijective (chap. III, § 1, no. 5, prop. 11). Therefore, by virtue of (36), $s_\Phi$ is bijective, and this establishes our first assertion (prop. 6, no. 6). Analogously $d_\Phi$ is bijective.

In the second assertion we have implicitly identified $\bigotimes_i F_i^*$ with $(\bigotimes_i F_i)^*$ and $\bigotimes_i E_i^*$ with $(\bigotimes_i E_i)^*$ by means of the mappings $j_s$ and $j_d$, which are here isomorphisms. The inverse forms  in the statement exist since the $s_{\Phi_i}$, the $d_{\Phi_i}$, $s_\Phi$ and $d_\Phi$ are bijective (no. 7). Let us then put $x' = x'_1 \otimes \cdots \otimes x'_m$, $y' = y'_1 \otimes \cdots \otimes y'_m$ ($x'_i \in E_i^*$, $y'_i \in F_i^*$, $i = 1, \ldots, m$). By definition of the inverse forms, and viewed (36), we have

$$
\widehat{\Phi}(j_s(y'), j_d(x')) = \Phi(s_{\Phi_1}^{-1}(y'_1) \otimes \cdots \otimes s_{\Phi_m}^{-1}(y'_m), d_{\Phi_1}^{-1}(x'_1) \otimes \cdots \otimes d_{\Phi_m}^{-1}(x'_m))
$$
$$
= \prod_{i=1}^m \Phi_i(s_{\Phi_i}^{-1}(y'_i), d_{\Phi_i}^{-1}(x'_i)) = \prod_{i=1}^m \widehat{\Phi}_i(y'_i, x'_i),
$$

whence our second assertion.

C. Q. F. D.

Let E and F be two modules over the commutative ring A, and $\Phi$ a sesquilinear form for $J$ on $E \times F$. The mapping
$$
(x_1, \ldots, x_m, y_1, \ldots, y_m) \to \det(\Phi(x_i, y_k)) \quad (x_i \in E, y_i \in F, i = 1, \ldots, m)
$$
of $E^m \times (F^j)^m$ into A is A-multilinear. It therefore defines a bilinear form $\Phi'$ on $(\bigotimes^m E) \times (\bigotimes^m F^j)$ characterized by
$$
\Phi'(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \det(\Phi(x_i, y_k)).
$$
Since the first member is zero when $x_i = x_k$ or when $y_i = y_k$ ($i \neq k$), $\Phi'$ defines, by passing to the quotients, a bilinear form on $(\wedge^m E) \times (\wedge^m F^j)$, or again, since $\wedge^m F^j$ is identified with $(\wedge^m F)^j$, a sesquilinear form $\Phi_{(m)}$ for J on $(\wedge^m E) \times (\wedge^m F)$. This one is characterized by
$$
\left\{
\begin{array}{l}
\Phi_{(m)}(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \det(\Phi(x_i, y_k)) \\
(x_i \in E, y_i \in F, i = 1, \ldots, m).
\end{array}
\right.
$$
(37)

#### Definition 12 {#alg-ix-s1-def-12 .statement}

Given two A-modules E, F and a form $\Phi$ sesquilinear for J on $E \times F$, the form $\Phi_{(m)}$ sesquilinear for J on $(\wedge^m E) \times (\wedge^m F)$ characterized by (37) is called the extension of $\Phi$ to the m-th exterior powers.

The notations being those of Def. 12, let us study the mappings associated with $\Phi_{(m)}$. From formula (24) (No. 6) and (37) we obtain the relations

$$
\Phi_{(m)}(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \det(\langle x_i, d_\Phi(y_k) \rangle)
= \det(\langle y_i, s_\Phi(x_k) \rangle^j).
$$

We therefore have

$$
s_{\Phi(m)} = k_s \circ (\wedge^m s_\Phi), \quad d_{\Phi m} = k_d \circ (\wedge^m d_\Phi),
$$

where $k_s$ (resp. $k_d$) denotes the canonical mapping of $\wedge^m F^*$ into $(\wedge^m F)^*$ (resp. of $\wedge^m E^*$ into $(\wedge^m E)^*$) (cf. Chap. III, § 8, No. 2).

#### Proposition 10 {#alg-ix-s1-prop-10 .statement}

*Let A be a commutative field endowed with an automorphism J, E and F two finite-dimensional vector spaces over A, and $\Phi$ a sesquilinear form for J on $E \times F$. If $\Phi$ is nondegenerate, then its extension $\Phi_{(m)}$ to the m-th exterior powers is nondegenerate, and the inverse form of $\Phi_{(m)}$ is the extension to the m-th exterior powers of the inverse form $\widehat{\Phi}$ of $\Phi$.*

Indeed, since $s_\Phi$ and $d_\Phi$ are bijective by assumption (Prop. 6, No. 6), the same is true of their exterior powers (Chap. III, § 5, No. 7). On the other hand the canonical mappings $k_s$ and $k_d$ are bijective (Chap. III, § 8, No. 2, Th. 1). Hence, by virtue of (38), $s_{\Phi(m)}$ and $d_{\Phi(m)}$ are bijective, which proves that $\Phi_{(m)}$ is nondegenerate (Prop. 6, No. 6). In the second assertion we have implicitly identified $\wedge^m F^*$ with $(\wedge^m F)^*$ and $\wedge^m E^*$ with $(\wedge^m E)^*$ by means of the mappings $k_s$ and $k_d$, which are here isomorphisms (*loc. cit.*). The inverse forms considered in the statement exist since $s_\Phi, d_\Phi, s_{\Phi(m)}, d_{\Phi(m)}$ are bijective (No. 7). Let then $x' = x'_1 \wedge \ldots \wedge x'_m$ and $y' = y'_1 \wedge \ldots \wedge y'_m$ ($x'_i \in E^*, y'_i \in F^*, i = 1, \ldots, m$). By definition of the inverse forms (No. 7) and in view of (38), we have

$$
\widehat{\Phi}_{(m)}(k_s(y'), k_d(x')) = \Phi_{(m)}(s^{-1}_\Phi(y'_1) \wedge \ldots \wedge s^{-1}_\Phi(y'_m), d^{-1}_\Phi(x'_1) \wedge \ldots \wedge d^{-1}_\Phi(x'_m))
= \det(\Phi(s^{-1}_\Phi(y'_i), d^{-1}_\Phi(x'_k))) = \det(\widehat{\Phi}(y'_i, x'_k))
$$

whence our second assertion.

#### Remark {#alg-ix-s1-n9-rem-1 .statement}

Let E be a free A-module, and let θ be the canonical isomorphism of $\bigwedge^m E$ onto the submodule of antisymmetrized tensors of order m (Chap. III, § 5, No. 6, Prop. 6). Let $\Phi$ be a sesquilinear form on E, $\Phi_{(m)}$ the extension of $\Phi$ to $\bigwedge^m E$, and $\Theta$ the sesquilinear form on $\bigwedge^m E$ which is the inverse image by $\theta$ of the extension of $\Phi$ to $\bigotimes^m E$. From the definition of $\theta$ and of the antisymmetrized tensor, and from (35), we have

$$
\Theta(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \sum_{\sigma, \tau} \varepsilon_\sigma \varepsilon_\tau \Phi(x_{\sigma(1)}, y_{\tau(1)}) \ldots \Phi(x_{\sigma(m)}, y_{\tau(m)})
$$

where $\sigma$ and $\tau$ run through the symmetric group $S_m$. From the formula for calculating determinants and formula (37), this expression can be written

$$
\sum_{\tau \in S_m} \varepsilon_\tau \det(\Phi(x_i, y_{\tau(k)})) = m! \det(\Phi(x_i, y_k));
$$

in other words, we have $\Theta = m! \Phi_{(m)}$.

### 10. Matrix calculations.

We propose, in the present No., to make more flexible the matrix calculus introduced in Chap. II, § 6, and to apply it to translating certain results proved in this paragraph.

I. — Let I and K be two finite sets of indices, H a nonempty set, and $M = (m_{ik})_{(i,k) \in I \times K}$ a matrix over H (Chap. II, § 6, No. 1, Def. 1).

The transpose of $M$ is called, and is denoted by ${}^tM$, the matrix $(m'_{ki})_{(k,i) \in K \times I}$ satisfying $m'_{ki} = m_{ik} \ ((i, k) \in I \times K)$. We obviously have

$$(39)$$
$$
{}^t({}^tM) = M.
$$

This generalizes the notion introduced in Chap. II, § 6, No. 6.

Suppose that H is a commutative group (written additively). The set of matrices over H having I and K for sets of indices admits a commutative group structure, since it is the set of mappings from $I \times K$ into H. This group is written additively.

Let $H', H''$ be two non-empty sets, $H$ a commutative group (written additively) and $f : (h', h'') \to h'h''$ a mapping from $\mathbf{H}' \times \mathbf{H}''$ into $\mathbf{H}$. Given two matrices
$$
M' = (m_{ik}')_{(i,k) \in I \times K}, \qquad M'' = (m_{kl}'')_{(k,l) \in K \times L}
$$
on $\mathbf{H}'$ and $\mathbf{H}''$ respectively, such that the set $K$ of the indices of the columns of $M'$ is equal to the set of indices of rows of $M''$, one calls the *product* of $M'$ and $M''$ (following $f$) and denotes by $M'M''$ the matrix
$$
M'.M'' = (\sum_{k \in K} m_{ik}' m_{kl}'' )_{(i,l) \in I \times L}
$$
on $\mathbf{H}$. This generalises the notion introduced in Chapter II, § 6, No. 4.
If $\mathbf{H}' = \mathbf{H}'' = \mathbf{H}$ and if $\mathbf{H}$ is a ring, the product $M'M''$ will, unless expressly stated otherwise, be calculated “in $\mathbf{H}$”, that is to say following the mapping $(x, y) \to xy$. When $\mathbf{H}'$ and $\mathbf{H}''$ are commutative groups (written additively) and $f$ is bilinear, one has
$$
\left\{
\begin{array}{l}
(M' + M'_1)M'' = M'M'' + M'_1M'', \\
M'(M'' + M''_1) = M'M'' + M'M''_1,
\end{array}
\right.
$$
where $M', M'_1$ are matrices on $\mathbf{H}'$, $M'', M''_1$ matrices on $\mathbf{H}''$, and where the sums and products written are supposed to be defined. Let $M', M''$ be matrices on the sets $\mathbf{H}', \mathbf{H}''$, and $f^0$ the mapping from $\mathbf{H}'' \times \mathbf{H}'$ into $\mathbf{H}$ defined by $(h'', h') \to h'h''$; then one has
$$
t(M'M'') = tM'' . tM'
$$
where the product in the first (resp. second) member is calculated following $f$ (resp. $f^0$).

In the case where $\mathbf{H}' = \mathbf{H}'' = \mathbf{H}$ is a ring, one obtains again formula (12) of Chapter II, § 6, No. 6.

Let $A$ be a ring, $J$ an antiautomorphism of $A$. For every matrix $M = (m_{ik})$ on $A$, we shall denote by $M^J$ the matrix $(m_{ik}^J)$. Let $M_1, M_2$ be two matrices on $A$ such that $M_1M_2$ is defined. Since $J$ is an isomorphism of $A$ onto the opposite ring $A^0$, one has $(M_1M_2)^J = M_1^J . M_2^J$ where the first (resp. second) member is calculated in $A$ (resp. $A^0$). Viewed (42) and (39), this gives
$$
(M_1M_2)^J = t(tM_2^J . tM_1^J)
$$
where the *two* members are calculated in $A$.

Bourbaki XXIV.

Soient $H_1, H_2, H_3, H_{12}, H_{23}$ et $H$ des groupes commutatifs (notés additivement), $f_{12} : H_1 \times H_2 \to H_{12}$, $f_{23} : H_2 \times H_3 \to H_{23}$, $f_3 : H_{12} \times H_3 \to H$, $f_1 : H_1 \times H_{23} \to H$ des mappings, et soient $M_1, M_2, M_3$ des matrices over $H_1, H_2, H_3$ respectivement. Si $f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))$ quels que soient les $x_i \in H_i$ ($i = 1, 2, 3$), alors les produits $(M_1 M_2) M_3$ et $M_1 (M_2 M_3)$ (calculés suivant $f_{12}, f_3, f_{23}$ et $f_1$), s’ils sont définis, sont égaux ; on les notera $M_1 M_2 M_3$. Lorsque $H_1 = H_2 = H_3 = H_{12} = H_{23} = H$, que $H$ est un anneau, et que $f_{12}, f_{23}, f_3, f_1$ sont égales à la mapping $(x, y) \to xy$, la condition précédente exprime l’associativité de cette dernière, et est donc vérifiée. On fera des conventions analogues pour les produits de plus de trois facteurs.

Soient $A, B$ deux anneaux, $M = (m_{ik})_{(i,k) \in I \times K}$ et $M' = (m'_{ik})_{(i,k) \in I \times K}$ deux matrices over un $(A, B)$-bimodule $G$ (No. 1). Si, pour toute matrice à une ligne $L = (a_i)_{i \in I}$ à éléments dans $A$ et toute matrice à une colonne $C = (b_k)_{k \in K}$ à éléments dans $B$, on a $L . M . C = L . M' . C$ (les produits étant calculés suivant les mappings qui définissent la structure de $(A, B)$-bimodule de $G$), alors les matrices $M$ et $M'$ sont égales. En effet, si l’on prend $a_i = 1, a_s = 0$ pour $s \neq i$, $b_k = 1, b_t = 0$ pour $t \neq k$, les matrices $L . M . C$ et $L . M' . C$, qui sont des matrices scalaires, sont respectivement égales à $m_{ik}$ et $m'_{ik}$.

II. — On considère un anneau $A$ et un $A$-module (à droite ou à gauche) $E$, admettant une base finie $(e_i)_{i \in I}$. Pour tout élément $x$ de $E$, on appelle matrice de $x$ par rapport à la base $(e_i)$, et on note $M(x)$ ou $x$, la matrice à une colonne formée des composantes $x_i$ ($i \in I$) de $x$ par rapport à $(e_i)$ (cf. Chapter II, § 6, No. 4); dans les calculs il sera commode, afin de rappeler que l’indice $i$ est un indice de ligne, de lui adjoindre un indice de colonne susceptible d’une seule valeur, et d’écrire $(x_{i0})$ la matrice $M(x)$.

Consider now two $A$-modules (left or right) $E$ and $F$, having finite bases $(e_i)_{i \in I}$ and $(f_k)_{k \in K}$ respectively; let $(f_k^*)$ be the basis of $F^*$ dual to $(f_k)$. We shall define the matrix, with respect to these bases, of a mapping $u$ from $E$ into $F$ in the following four cases:

(D) $E$ and $F$ are right modules, $u$ is $A$-linear ;

(G) E and F are left modules, u is A-linear ;
(GD) E is a left module, F a right module, A is endowed with an antiautomorphism J, u is $\mathbf{Z}$-linear and satisfies $u(ax) = u(x)a^J$ ($a \in A,\ x \in E$) (in other words u is an A-linear mapping from $E^J$ into F (no 2, def. 5)).
(DG) E is a right A-module, F a left A-module, A is endowed with an autiautomorphism J, u is $\mathbf{Z}$-linear and satisfies $u(xa) = a^Ju(x)$ ($x \in E,\ a \in A$) (in other words u is an A-linear mapping from $E^J$ into F).
In each of these four cases, the matrix of the mapping u is, by definition, the matrix $(u_{ki})_{(k,i) \in \mathbb{K} \times I}$ such that
$$
u_{ki} = \langle u(e_i), f_k^* \rangle.
$$
This definition coincides, in case (D), with that given in chap. II, § 6, no 3. Under these conditions the matrix $M(u(x))$ of the image of an element x of E is given by the following formulas:
$$
\begin{align*}
(45\ D)\quad &M(u(x)) = M(u) \cdot M(x) \\
(45\ G)\quad &{}^tM(u(x)) = {}^tM(x) \cdot {}^tM(u) \\
(45\ GD)\quad &M(u(x)) = M(u) \cdot M(x)^J \\
(45\ DG)\quad &{}^tM(u(x)) = {}^tM(x)^J \cdot {}^tM(u).
\end{align*}
$$
Let us verify, for example (45 DG), the other verifications being analogous and a little easier. Put $x = \sum e_ix_{io}$, $u(x) = \sum y_{ko}f_k$; we have $u(x) = u(\sum e_ix_{io}) = \sum x_{io}^ju(e_i) = \sum x_{io}^ju_{ki}/k$; whence $y_{ko} = \sum x_{io}^ju_{ki}$; in order to put the two indices i next to one another, consider the transposed matrices ${}^tM(x) = (x'_{oi})$ where $x'_{oi} = x_{io}$, and ${}^tM(u) = (u'_{ik})$ where $u'_{ik} = u_{ki}$; we then have $y_{ko} = \sum x'_{oi}u'_{ik}$; since the second member is the element of index k of the one-row matrix ${}^tM(x)^J \cdot {}^tM(u)$, formula (45 DG) is verified.

#### Remark 1 {#alg-ix-s1-n10-rem-1 .statement}

When A is commutative, (45 G) reduces to (45 D), and (45 DG) to (45 GD), by means of the formula ${}^t(M'M'') = {}^tM'' \cdot {}^tM'$ (cf. (42)), where the two members are here calculated in A.
2) Let E, F, G be three left modules having finite bases, and $u : E \to F,\ v : F \to G$ A-linear mappings. It follows from (45 G) that one has
$$
{}^tM(v \circ u) = {}^tM(u) \cdot {}^tM(v).
$$

Indeed, for whatever $x \in E$,

$$
{}^t M(x) \cdot {}^t M(\varphi \circ u) = {}^t M(\varphi(u(x))) = {}^t M(u(x)) \cdot {}^t M(\varphi)
= {}^t M(x) \cdot {}^t M(u) \cdot {}^t M(\varphi),
$$

whence (46).

Recall that, in the case of right modules, one has

$$
M(\varphi \circ u) = M(\varphi) M(u).
$$

III. — We shall henceforth denote by A a ring, by B a ring (resp. a ring endowed with an antiautomorphism J, for which one puts $J' = J^{-1}$), by E a left A-module having a finite basis $(e_i)_{i \in I}$, and by F a right (resp. left) B-module having a finite basis $(f_k)_{k \in K}$. We denote by $(e_i^*)$ and $(f_k^*)$ the dual bases of E* and F*. Unless express mention to the contrary the matrices considered are taken with respect to these bases.

Let G be an (A, B)-bimodule (no 1), Φ a bilinear mapping (resp. a right sesquilinear mapping for J) from $E \times F$ into G, and $R = (\Phi(e_i, f_k))$ the matrix of Φ. Then, for $x \in E$ and $y \in F$, formula (6) of no 1 (resp. (8) of no 2), is written, with the above conventions,

(47) $\Phi(x, y) = {}^t M(x) \cdot R \cdot M(y)$ (resp. $\Phi(x, y) = {}^t M(x) \cdot R \cdot M(y)^J$),

where the products are calculated according to the mappings which define the structure of the (A, B)-bimodule of G ; in particular, if $A = B = G$ (in which case Φ is a form), the products are calculated in A.

Let $E’$ be a left A-module having a finite basis $(e'_s)_{s \in S}$, $F’$ a right (resp. left) A-module having a finite basis $(f'_t)_{t \in T}$, $u : E \to E'$ and $\varphi : F \to F'$ A-linear mappings, and $\Phi'$ a bilinear (resp. right sesquilinear for $J$) mapping from $E' \times F'$ into $G$. Let $\Phi$ denote the inverse image of $\Phi'$ (with respect to $u$ and $\varphi$), $U, V, R, R'$ the matrices of $u, \varphi, \Phi, \Phi'$ with respect to the bases under consideration. We then have

(48) $R = {}^t U \cdot R' \cdot V$ (resp. $R = {}^t U \cdot R' \cdot V^J$),

the products being calculated as in (47). Indeed, for any $x \in E$ and $y \in F$, we have by definition $\Phi(x, y) = \Phi'(u(x), v(y))$, whence, according to (47),

$$
'M(x).R.M(y) = 'M(u(x)).R'.M(v(y))
$$
(resp. $'M(x).R.M(y)^J = 'M(u(x)).R'.M(v(y))^J$);

according to (45 G) and (45 D) (resp. (45 G)) and (43) we deduce

$$
'M(x).R.M(y) = 'M(x).'U.R'.V.M(y)
$$
(resp. $'M(x).R.M(y)^J = 'M(x).'U.R'.('M(y).'V)^J$
$= 'M(x).'U.R'.V^J.M(y)^J$);

this proves our assertion.

IV. — We suppose here that the rings $A$ and $B$ are equal, and we denote by $\Phi$ a bilinear (resp. right sesquilinear for $J$) form on $E \times F$, and by $R$ its matrix. Let us calculate the matrices of the mappings $s_\Phi$ and $d_\Phi$ associated with $\Phi$, which we shall denote by $s$ and $d$ for simplicity. Since we have $\Phi(x, y) = \langle y, s(x) \rangle = \langle x, d(y) \rangle$ according to (23), No. 6 (resp. $\Phi(x, y) = \langle x, d(y) \rangle = \langle y, s(x) \rangle^J$ according to (24), No. 6), we have $\Phi(e_i, f_k) = \langle f_k, s(e_i) \rangle = \langle e_i, d(f_k) \rangle$ (resp. $\Phi(e_i, f_k) = \langle e_i, d(f_k) \rangle = \langle f_k, s(e_i) \rangle^J$), whence, according to (44) and since $(e_i)$ is the dual basis of $(e_i^*)$ and $(f_k)$ the dual basis of $(f_k^*)$:

(49) $M(d) = R, \ M(s) = 'R$   (resp. $M(d) = R, \ M(s) = 'R^{J'}$).

#### Remark 2 {#alg-ix-s1-n10-rem-2 .statement}

When $A$ is a field, the linear mappings $s$ and $d$ have the same rank. We see here that their matrices $M(s)$ and $M(d)$ have the same rank; indeed, a matrix over $A$ and its transpose have the same rank (chap. II, § 6, No. 7, prop. 3) and, when $\Phi$ is sesquilinear, the equality of the ranks of $R$ over $A$ and of $'R$ over $A^0$ (ibid.) and the fact that $J'$ is an isomorphism of $A^0$ onto $A$, entail the equality of the ranks of $R$ and of $'R^J$ over $A$.

#### Remark 3 {#alg-ix-s1-n10-rem-3 .statement}

If $M$ and $N$ are right $A$-modules having finite bases $(m_i)$ and $(n_k)$, $\Phi$ a left sesquilinear form for $J$ on $M \times N$ (No. 6, Remark), $s$ and $d$ its associated mappings, and $R = (\Phi(m_i, n_k))$ its matrix, the formulas (26) of No. 6 show that one has

$$
M(d) = R^{J'}, \quad M(s) = 'R.
$$

Suppose now that the mappings $s$ and $d$ associated to $\Phi$ are bijective and calculate the matrix $\hat{R}$ of the inverse form of $\Phi$ (No. 7). When $\Phi$ is bilinear, $\Phi$ is the inverse image of $\hat{\Phi}$ relative to the linear mappings $s : E \to F^*$ and $d : F \to E^*$; one therefore has, by virtue of (48) and (49), $R = R . \hat{R} . R$, whence, since $R$ is invertible ($d$ being bijective), $\hat{R} = R^{-1}$. This formula extends to the case where $\Phi$ is sesquilinear, because, if one considers $\Phi$ as a bilinear form on $E \times F^J$, and if one identifies $(F^J)^*$ with $(F^*)^J$ (cf. No. 9), the inverse form of this bilinear form coincides with $\hat{\Phi}$ considered as a bilinear form on $(F^*)^J \times E^*$. In both cases *the matrix of the inverse form of $\Phi$ is the inverse of the matrix of $\Phi$*.

Let finally $E'$ be a left A-module, $F'$ a right A-module (resp. left A-module), both admitting finite bases $(e'_s)$ and $(f'_t)$; let $\Phi'$ be a bilinear form (resp. sesquilinear form for J) on $E' \times F'$, and let $R'$ be its matrix. Suppose $s_\Phi$ and $d_\Phi$ are bijective. Let $u : E \to E'$ and $\nu : F \to F'$ be linear mappings, $u^* : F' \to F$ and $\nu^* : E' \to E$ their *adjoints* (No. 8, prop. 7); denote by $U, V, U^*, V^*$ the matrices of $u, \nu, u^*, \nu^*$ with respect to the given bases. One then has

$$
U^* = R^{-1} . {}^t U . R', \quad {}^t V^* = R'. V . R^{-1}
$$
(resp. $U^{*J} = R^{-1} . {}^t U . R', \ {}^t V^* = R'. V^J . R^{-1}$).

Indeed, for all $x \in E$ and $y \in F'$, we have $\Phi'(u(x), y) = \Phi(x, u^*(y))$ (No. 8, def. 10). Whence, when $\Phi$ is bilinear, by virtue of (47), ${}^t M(u(x)) . R' . M(y) = {}^t M(x) . R . M(u^*(y))$; this gives, by virtue of (45 G) and (45 D), ${}^t M(x) . {}^t U . R' . M(y) = {}^t M(x) . R . U^* . M(y)$, whence ${}^t U . R' = R . U^*$ and the first formula announced since, $d$ being bijective, $R$ is invertible. When $\Phi$ is sesquilinear (47) and (45 G) give ${}^t M(x) . {}^t U . R' . M(y)^J = {}^t M(x) . R . {}^t ({}^t M(y) . {}^t U^*)^J$; now, by (43), we have $({}^t M(y) . {}^t U^*)^J = {}^t ({}^t U^{*J} . {}^t M(y)^J)$, whence ${}^t ({}^t M(y) . {}^t U^*)^J = U^{*J} . M(y)^J$; it follows therefore that ${}^t M(x) . {}^t U . R' . M(y)^J = {}^t M(x) . R . U^{*J} . M(y)^J$, whence ${}^t U . R' = R . U^{*J}$, and $U^{*J} = R^{-1} . {}^t U . R'$. The verification of the formulas for $V^*$ is analogous.

*Exercises.* — 1) Let A be a commutative field, E a vector space over A admitting an infinite countable basis $(e_n)_{n \geqslant 1}$. A bilinear form $\Phi$ is defined on E by setting $\Phi(e_{i+1}, e_i) = 1$ for $i \geqslant 1$, $\Phi(e_k, e_j) = 0$ for $k \neq j + 1$ and $j \geqslant 1$. Prove that the linear mapping $d_\Phi$ associated on the right to $\Phi$ is injective, but that the linear mapping $s_\Phi$ associated on the left to $\Phi$ is not injective.

2) Let E be the $\mathbf{Z}$-module direct sum of $\mathbf{Z}$ and of $\mathbf{Z}/(2)$, and let $E^*$ be its dual (isomorphic to $\mathbf{Z}$). Prove that the bilinear form $(x, x') \to \langle x, x' \rangle$ on $E \times E^*$ is such that the linear mapping associated on the right is injective, but the linear mapping associated on the left is not.

#### Remark 4 {#alg-ix-s1-n10-rem-4 .statement}

Give an example of a bilinear form $\Phi$ defined on a product $E \times F$ of two vector spaces, such that $d_\Phi$ is bijective, $s_\Phi$ injective but not bijective (take $E$ of infinite dimension and $F$ equal to the dual $E^*$ of $E$; cf. Chap. II, § 5, exer. 3).

#### Remark 5 {#alg-ix-s1-n10-rem-5 .statement}

Let $A$ be a ring endowed with an antiautomorphism $J$, $E$ a left $A$-module, $G$ an $(A, A)$-bimodule and $\Phi$ a mapping from $E \times E$ into $G$, right sesquilinear for $J$. Prove the identity (where $Q(x) = \Phi(x, x)$) :

$$
2\Phi(x, y)\ (\mu^J\lambda^J - \lambda^J\mu^J) = Q(x - \mu\lambda y) - Q(x + \mu\lambda y) + \mu Q(x + \lambda y)
- \mu Q(x - \lambda y) + Q(x + \mu y)\lambda^J - Q(x - \mu y)\lambda^J + \mu Q(x - y)\lambda^J - \mu Q(x + y)\lambda^J.
$$

#### Remark 6 {#alg-ix-s1-n10-rem-6 .statement}

Soient $K$ a commutative field of characteristic 2, $A$ a separable quadratic extension of $K$; one has $A = K(\theta)$, where $\theta$ is root of an irreducible polynomial $X^2 + X + \beta$ of $K[X]$ and the $K$-automorphism $J$ of $A$, distinct from the identity, is such that $\theta^J = \theta + 1$ (Chapter V, § 11, Exercise 8). Now prove that if $E$ and $G$ are vector spaces over $A$, $\Phi$ a sesquilinear mapping (for $J$) from $E \times E$ into $G$, one has, putting $Q(x) = \Phi(x, x)$,

$$
\Phi(x, y) = Q(\theta x + y) - \beta Q(x) - Q(y) - (\theta + 1)(Q(x + y) - Q(x) - Q(y)).
$$

#### Remark 7 {#alg-ix-s1-n10-rem-7 .statement}

Soient $A$ a field, $E$ a vector space over $A$, $\Phi$ a sesquilinear form on $E$, $u$ an endomorphism of $E$.

a) For there to exist one and only one endomorphism $u^*$ of $E$ such that $\Phi(u(x), y) = \Phi(x, u^*(y))$ for $x, y$ in $E$, it is necessary and sufficient that $d_\Phi$ be injective and that $u(d_\Phi(E)) \subset d_\Phi(E)$.

b) Give an example where $E$ is of infinite dimension and $d_\Phi$ is injective, but where $u(d_\Phi(E))$ is not contained in $d_\Phi(E)$.

#### Remark 8 {#alg-ix-s1-n10-rem-8 .statement}

Let $E, E_1$ be two $A$-modules, $\Phi$ (resp. $\Phi_1$) a sesquilinear form on $E$ (resp. $E_1$). Suppose that $\Phi_1$ is non-degenerate and that there exist an element $\alpha \in A$ and a bijection $u$ of $E$ onto $E_1$ such that $\Phi_1(u(x), u(y)) = \Phi(x, y)\alpha$ for all $x, y$ in $E$. Show that: 1° $\Phi$ is non-degenerate ; 2° $u$ is linear ; 3° if $E_1$ is a faithful $A$-module, the same is true of $E$, and $\alpha$ is not a right divisor of 0 in $A$ ; 4° if $\Phi_1$ takes values in $A$ which are not left divisors of 0, the same is true of $\Phi$.

#### Remark 9 {#alg-ix-s1-n10-rem-9 .statement}

Let $A$ be a field, $E_1, E_2$ two vector spaces not reduced to 0 over $A$, $\Phi_1$ (resp. $\Phi_2$) a non-degenerate sesquilinear form on $E_1$ (resp. $E_2$) for an antiautomorphism $J_1$ (resp. $J_2$) of $A$. Let $u$ be a linear mapping of $E_1$ onto $E_2$ such that the relation $\Phi_1(x, y) = 0$ implies $\Phi_2(u(x), u(y)) = 0$.

a) Show that $u$ is a bijection of $E_1$ onto $E_2$. (If $u(0)$ were not reduced to 0, show that there would exist in $E_1$ two vectors $a, b$ such that $u(a) \neq 0, u(b) = 0$ and $\Phi_1(a, b) \neq 0$; if $H$ is the hyperplane of the $x \in E_1$ such that $\Phi_1(a, x) = 0$, remark that one would have $u(H) = E_2$.

b) Show that if dim $E_1 \geqslant 2$, there exists $\alpha \in A$ such that one has $\Phi_2(u(x), u(y)) = \Phi_1(x, y)\alpha$ whatever $x, y$ in $E_1$. (For every $y \in E_1$, show that there exists an element $m(y) \in A$ such that $\Phi_2(u(x), u(y)) = \Phi_1(x, y)m(y)$ for every $x \in E_1$, and that if $y$ and $y'$ are linearly independent in $E_1$, one has $m(y + y') = m(y) = m(y')$).

#### Remark 10 {#alg-ix-s1-n10-rem-10 .statement}

Let $A$ be a field, $E, F$ two left vector spaces over $A$, $\Phi$ a non-degenerate sesquilinear form on $E \times F$ for an antiautomorphism $J$ of $A$.

a) Let $M$ be a subspace of $E$, $N$ a subspace of $F$ such that $N \supset M^0$ and $M \supset N^0$. Show that if one of the spaces $N/M^0, M/N^0$ is of finite dimension, the same is true of the other, and the dimensions of these two spaces are equal.

b) Let $M, M'$ be two subspaces of $E$ such that $M^{00} = M$ and that $M'$ is of finite dimension; show that one has $(M \cap M')^0 = M^0 + {M'}^0$ and $(M + M')^{00} = M + M'$. (Applying $a$) to the subspaces $M'$ and $M^0 + {M'}^0$, show that $\dim(M \cap M') = \operatorname{codim}(M^0 + {M'}^0)$; applying $a$ to the subspaces $M + M'$ and $M^0$, show that
$$
\dim((M + M')^{00}/M) = \dim((M + M')/M)).
$$

c) If $E = F$ and if $M$ is a subspace of $E$ such that $E = M^0 + M^{00}$, show that $E$ is direct sum of $M^0$ and $M^{00}$.

d) Let $E$ be a vector space over a commutative field $A$ admitting an infinite countable basis $(e_n)_{n \geqslant 0}$, and let $\Phi$ be the symmetric bilinear form on $E$ such that $\Phi(e_n, e_n) = 1$ for all $n$, $\Phi(e_i, e_j) = 0$ for $i \geqslant 1, j \geqslant 1$ and $i \neq j$, and $\Phi(e_0, e_n) = 1$ for all $n \geqslant 1$. Now prove that $\Phi$ is nondegenerate. Let $M$ (resp. $N$) be the subspace of $E$ generated by the $e_{2k}$ (resp. $e_{2k-1}$) for $k \geqslant 1$, and let $H = M + N$, which is a hyperplane in $E$. Now prove that one has $M^0 = N, N^0 = M, H^{00} = E \neq H, (M \cap N)^0 \neq M^0 + N^0$ and $(M + N)^{00} \neq M + N$, though $M^{00} = M, N^{00} = N$; if $L$ is the subspace of finite dimension 2 generated by $e_0$ and $e_1$, one has $(L \cap H)^0 \neq L^0 + H^0$.

#### Remark 11 {#alg-ix-s1-n10-rem-11 .statement}

Let $E, E'$ be two left vector spaces over fields $A, A'$ respectively, of dimension $\geqslant 3$; let $\mathfrak{F}(E)$ (resp. $\mathfrak{F}(E')$ be the lattice ordered set (for the relation of inclusion) formed by the finite-dimensional subspaces of $E$ (resp. $E'$).

a) Let $p$ be a mapping from $\mathfrak{F}(E)$ into $\mathfrak{F}(E')$ such that for all $M \in \mathfrak{F}(E)$, $\dim p(M) = \dim M$, and such that for every pair $(M, N)$ of elements of $\mathfrak{F}(E)$, $p(M + N) = p(M) + p(N)$. Now prove that $p$ is injective; if $p$ is bijective, there exists a bijective semilinear mapping $u$ from $E$ into $E'$ such that one has $u(M) = p(M)$ for all $M \in \mathfrak{F}(E)$ (use Exercise 10 of Chapter II, 2nd ed., App. III).

(b) Give an example where $A' = A$ is commutative, $E' = E$ is of finite dimension, and where there exists a mapping $p$ from $\mathfrak{F}(E)$ into itself, such that $\dim p(M) = \dim M, p(M + N) = p(M) + p(N), p(M \cap N) = p(M) \cap p(N)$, but there does not exist any injective semilinear mapping $u$ from $E$ into itself such that $u(M) = p(M)$ for $M \in \mathfrak{F}(E)$. (Consider the case where there exists a superfield $A''$ of $A$ of finite degree and isomorphic to $A$,
