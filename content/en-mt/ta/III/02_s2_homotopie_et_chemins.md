---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 2
section_title: Homotopie et chemins
lang: en
source: ta-i-iv-fr
book_pages: TA III.256-TA III.289, TA III.330-TA III.333
pdf_pages: 0272-0305, 0346-0349
extraction: native
subsections:
    - "no": 1
      title: Chemins
      page: 256
      pdf_page: 272
    - "no": 2
      title: Espaces connexes par arcs
      page: 258
      pdf_page: 274
    - "no": 3
      title: Espaces localement connexes par arcs
      page: 260
      pdf_page: 276
    - "no": 4
      title: Liens entre connexité et connexité par arcs
      page: 264
      pdf_page: 280
    - "no": 5
      title: Applications continues par arcs
      page: 267
      pdf_page: 283
    - "no": 6
      title: Compléments sur les espaces topologiques compacts métrisables
      page: 269
      pdf_page: 285
    - "no": 7
      title: Propriétés topologiques de l’image d’un chemin
      page: 272
      pdf_page: 288
    - "no": 8
      title: Caractérisations de l’intervalle
      page: 274
      pdf_page: 290
    - "no": 9
      title: Chemins injectifs
      page: 282
      pdf_page: 298
    - "no": 10
      title: Relèvement de chemins
      page: 284
      pdf_page: 300
statements: 63
exercises: 14
content_sha256: cab9fc5ba5b92b75bbb3ee22fc440f67b9b9db559ed7fb0d29ade6a5d0fb5596
translated_from: content/fr/ta/III/02_s2_homotopie_et_chemins.md
source_lang: fr
translation_method: machine
source_content_sha256: b214ad435328c152b9f50ea162a4637ba5cfe86644f618ffa88c8d9d23c86683
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5-6, gpt-5.4
translation_run: translate-en-mt-7f896573
glossary_version: 34
glossary_terms_sha256: 8cc43eeac3886ef58cdadf8f4af0811a63671ba02b517105896c6a7faa1fcd0d
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. HOMOTOPY AND PATHS

### 1. Paths

#### Definition 1 {#ta-iii-s2-def-1 .statement tag=01WN}

Let X be a topological space. A path in X is called any continuous mapping $c$ of $\mathbf{I}$ into X. The point $c(0)$ is called the origin, the point $c(1)$ the term of the path $c$. A loop in X is called a path in X whose origin is equal to the term.

Let $x$ and $y$ be points of X. One says that a path $c$ in X joins $x$ to $y$ if $x$ is its origin and $y$ is its term.

#### Definition 2 {#ta-iii-s2-def-2 .statement tag=01WO}

Let X be a topological space. One says that paths $c$ and $d$ in X are juxtaposed if one has $c(1) =d(0)$. One then calls juxtaposed path of $c$ and $d$ the path $c*d$ defined by the formula:

$c(2t)$ for $0\leqslant t\leqslant 1/2$,

$$
(c*d)(t) = \tag{1}
$$

$d(2t-1)$ for $1/2\leqslant t\leqslant 1$.

Its origin is that of $c$, its term that of $d$.

Let $c$ be a path in X; one calls the path opposite to $c$ and denotes by $\overline{c}$ the path defined by $\overline{c}(t) =c(1-t)$ for $t\in \mathbf{I}$.

one hasIf $cc$and$*dd=$are two juxtaposed paths in$\overline{d}*\overline{c}$. For every path $c$ in X, one hasX$,\overline{\overline{\overline{c}}d}=$and$c\overline{c.}$ are, and

#### Remark 1 {#ta-iii-s2-n1-rem-1 .statement tag=01WP}

Let X be a topological space and let P be a topological space reduced to a point. Identify $P\times \mathbf{I}$ with $\mathbf{I}$ by the projection pr$_2$. The set $\mathscr{C}(P\times \mathbf{I}; X)$ of homotopies between (necessarily continuous) mappings from P into X is then identified with the set $\mathscr{C}(\mathbf{I}; X)$ of paths in X. To a homotopy joining the constant mapping of image $x$ to the constant mapping of image $y$ there corresponds a path with origin $x$ and term $y$. The preceding identifications are compatible with the notions of juxtaposition and passing to the opposite (cf. III, p. 230).

#### Remark 2 {#ta-iii-s2-n1-rem-2 .statement tag=01WQ}

Let X and Y be topological spaces. The canonical mapping

$$
\mathscr{C}(X\times \mathbf{I}; Y)\rightarrow \mathscr{C}(\mathbf{I};\mathscr{C}_c(X; Y))
$$

associates to every homotopy $\sigma : X\times \mathbf{I}\rightarrow Y$ joining two mappings $f$ and $g$ from X into Y a path with origin $f$, term $g$, in the space $\mathscr{C}_c(X; Y)$. If X is a locally compact space, this canonical mapping is bijective (TG, X, p. 28, theorem 3).

Let X be a topological space. One calls the space of paths of X, and denotes by Λ(X), the topological space $\mathscr{C}_c(\mathbf{I}; X)$ whose elements are the paths in X and whose topology is that of compact convergence (cf. TG, X, p. 27). If $x$ is a point of X, one denotes by $\Lambda_x(X)$ the subspace of Λ(X) formed by paths with origin $x$. If $y$ is a second point of X, one denotes by $\Lambda_{x,y}(X)$ the subspace of Λ(X) formed by paths with origin $x$ and term $y$.

#### Proposition 1 {#ta-iii-s2-prop-1 .statement tag=01WR}

Let X and Z be topological spaces. For a mapping $\varphi$ of Z into the space of paths $\mathscr{C}_c(\mathbf{I}; X)$ to be continuous, it is necessary and sufficient that the mapping $(z, t)\mapsto \varphi (z)(t)$ be a continuous mapping of $Z\times \mathbf{I}$ into X. In particular, the mapping $(c, t)\mapsto c(t)$ of $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ into X is continuous.

The topological space $\mathbf{I}$ being locally compact, the proposition follows from TG, X, p. 28, th. 3.

We denote $o$ and call origin mapping the mapping $c\mapsto c(0)$ of Λ(X) into X; we denote $e$ and call term mapping the mapping $c\mapsto c(1)$ of Λ(X) into X. The mappings $o$ and $e$ are continuous (TG, X, p. 27, remark 1). The pairs of juxtaposed paths in X are the elements of the fibered product of the X-spaces $(\Lambda (X), e)$ and $(\Lambda (X), o)$.

#### Proposition 2 {#ta-iii-s2-prop-2 .statement tag=01WS}

Let X be a topological space. The map which associates with a path $c$ the opposite path $\overline{c}$ is a homeomorphism of Λ(X) onto itself. The juxtaposition of paths $(c, d)\mapsto c*d$ is a homeomorphism of the space $(\Lambda (X), e)\times_X(\Lambda (X), o)$ onto Λ(X).

The mapping $t\mapsto 1-t$ is a homeomorphism of the space $\mathbf{I}$ onto itself; the first assertion follows.

Let C denote the fibered product $(\Lambda (X), e)\times_X(\Lambda (X), o)$. Let $\gamma : C\rightarrow$ Λ(X) be the mapping $(c, d)\mapsto c*d$ and $\delta : C\times \mathbf{I}\rightarrow$ X the mapping $((c, d), t)\mapsto (c*d)(t)$. The restrictions of the mapping $\delta$ to $C\times [0,\frac{1}{2}]$ and $C\times [\frac{1}{2},1]$ are continuous by virtue of formula (1) and of prop. 1. The mapping $\delta$ is therefore continuous (TG, I, p. 19, prop. 4), as is the mapping $\gamma$ (prop. 1). We have $c(t) = (c*d)(\frac{t}{2})$ and $d(t) = (c*d)(\frac{1+t}{2})$, hence $\gamma$ is injective.

Let $g$ be a path in X; for $t\in \mathbf{I}$, put

$c_g(t) =g(\frac{t}{2})$ and $d_g(t) =g(\frac{1 + t}{2})$.

The mappings $c_g$ and $d_g$ thus defined are juxtaposed paths in X and we have $c_g*d_g=g$. Moreover, the mappings $g\mapsto c_g$ and $g\mapsto d_g$ are continuous mappings of the space Λ(X) into itself (prop. 1). It follows that the mapping $\gamma$ is a homeomorphism.

#### Corollary {#ta-iii-s2-n1-cor-1 .statement tag=01WT}

Let X be a topological space and let $x,y,z$ be points of X. The mappings $c\mapsto \overline{c}$ of $\Lambda_{x,y}(X)$ into $\Lambda_{y,x}(X)$ and $(c, d)\mapsto$ $c*d$ of $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ into $\Lambda_{x,z}(X)$ are continuous.

### 2. Arcwise connected spaces

#### Definition 3 {#ta-iii-s2-def-3 .statement tag=01WU}

A topological space X is said to be arcwise connected if for every pair $(x, y)$ of points of X, there exists a path of origin $x$ and of term $y$.

#### Example 1 {#ta-iii-s2-n2-exa-1 .statement tag=01WV}

Every interval of $\mathbf{R}$, every convex subset of a numerical space or, more generally, of a topological vector space over $\mathbf{R}$ is arcwise connected.

#### Proposition 3 {#ta-iii-s2-prop-3 .statement tag=01WW}

The image by a continuous mapping of an arcwise connected space is arcwise connected.

Let X be a path-connected space, $f: X\rightarrow Y$ a continuous mapping. Let $x$ and $y$ be two points of $f(X)$; let $x'$ and $y'$ be points of X such that $f(x') =x$ and $f(y') =y$. There exists a path $c$ in X whose origin is $x'$ and whose term is $y'$. Then, $f\circ c$ is a path in $f(X)$ with origin $x$ and term $y$.

#### Proposition 4 {#ta-iii-s2-prop-4 .statement tag=01WX}

A path-connected topological space is connected.

Since every interval of $\mathbf{R}$ is connected, the image of a path is connected (TG, I, p. 82, prop. 4). The empty space is connected. Since a nonempty path-connected space is the union of the images of the paths issuing from one of its points, it is connected (TG, I, p. 81, prop. 2).

Taking into account the identification (III, p. 256, remark 1) of the paths in X with the homotopies between mappings of a topological space P reduced to a point into X, Proposition 1 of III, p. 230 gives:

#### Proposition 5 {#ta-iii-s2-prop-5 .statement tag=01WY}

In a topological space, the relation “there exists a path with origin $x$ and term $y$” is an equivalence relation.

The path-connected components of a topological space X are called the equivalence classes for the above relation. A path-connected component is a path-connected space. Let $x$ be a point of X. The path-connected component of $x$ is the union of the path-connected subspaces of X containing $x$. It is also the union of the images of the paths with origin $x$ in X.

#### Example 2 {#ta-iii-s2-n2-exa-2 .statement tag=01WZ}

The union of a family of path-connected sets, whose intersection is nonempty, is path-connected (cf. TG, I, p. 81, prop. 2).

#### Example 3 {#ta-iii-s2-n2-exa-3 .statement tag=01X0}

A subset of a numerical space (or, more generally, a topological vector space over $\mathbf{R}$) which is star-shaped at one of its points is path-connected.

Let X be a topological space. We denote by $\pi_0(X)$ the set of path-connected components of X. Let P be a topological space reduced to a point. The mapping from X into [P; X] which, to every point $x$ of X, associates the homotopy class $\varphi_x$ of the mapping $f_x: P\rightarrow X$ having image $x$, defines by passing to the quotient a bijection, called canonical, of $\pi_0(X)$ onto [P; X]. We have $\pi_0(\emptyset ) =\emptyset$. For a nonempty topological space to be path-connected, it is necessary and sufficient that $\pi_0(X)$ be a set with one element.

Let X and Y be topological spaces and $f: X\rightarrow Y$ a continuous mapping. The image $f(C)$ of every path-connected component C of X is path-connected (III, p. 258, prop. 3), hence contained in a path-connected component of Y. We denote by $\pi_0(f):\pi_0(X)\rightarrow \pi_0(Y)$ the mapping which, to a path-connected component C of X, associates the unique path-connected component $C'$ of Y such that $f(C)\subset C'$. If we identify $\pi_0(X)$ and $\pi_0(Y)$ with [P; X] and [P; Y] respectively, the mapping $\pi_0(f)$ identifies with the mapping $\chi \mapsto [f]\circ \chi$ from [P; X] into [P; Y]. In particular, if $f$ and $g$ are homotopic mappings from X into Y, we have $\pi_0(f) =\pi_0(g)$ (III, p. 230, prop. 2).

Let Z be a topological space and let $g: Y\rightarrow$ Z be a continuous mapping; we have $\pi_0(g\circ f) =\pi_0(g)\circ \pi_0(f)$. In particular, if Z = X and if $f$ and $g$ are homotopy inverses of one another up to homotopy, we have $\pi_0(g)\circ \pi_0(f) =\pi_0$(Id$_X$) $=$ Id$_{\pi_0(X)}$ and $\pi_0(f)\circ \pi_0(g) =\pi_0$(Id$_Y$) $=$ Id$_{\pi_0(Y)}$, which proves that $\pi_0(f)$ and $\pi_0(g)$ are inverse bijections of one another. A space homotopy equivalent to a path-connected space is therefore itself path-connected. In particular, a space homotopy equivalent to a point is path-connected.

#### Proposition 6 {#ta-iii-s2-prop-6 .statement tag=01X1}

Let $(Y_j)_{j\in J}$ be a family of topological spaces. The mapping

$(\pi_0$(pr$_j$))$:\pi_0(\prod_{j\in J}Y_j)\rightarrow \prod_{j\in J}\pi_0(Y_j)$

is bijective. In particular, the product space of a family of path-connected spaces is path-connected.

This follows from Proposition 3 of III, p. 231 where one takes for X a space reduced to a point.

### 3. Locally path-connected spaces

#### Definition 4 {#ta-iii-s2-def-4 .statement tag=01X2}

A topological space is said to be locally path-connected if each of its points possesses a fundamental system of path-connected neighbourhoods.

#### Proposition 7 {#ta-iii-s2-prop-7 .statement tag=01X3}

A locally path-connected topological space is locally connected. Its connected components coincide with its path-connected components. In particular, if a locally path-connected topological space is connected, it is path-connected.

The first assertion follows from prop. 4. Let us prove the second assertion. Let X be a locally path-connected topological space and let C be a path-connected component of X. Every point of C possesses a path-connected neighbourhood, hence contained in C; consequently, C is an open subset of X. The path-connected components forming a partition of X, such a component is also closed. Since it is connected (III, p. 258, prop. 4), it is a connected component (TG, I, p. 83). The third assertion follows from the second.

Thus we see that there is no ambiguity in saying that a topological space is connected and locally path-connected.

#### Corollary 1 {#ta-iii-s2-prop-7-cor-1 .statement tag=01X4}

Every connected open subset of a locally path-connected topological space is path-connected.

#### Corollary 2 {#ta-iii-s2-prop-7-cor-2 .statement tag=01X5}

Let B be a locally path-connected topological space and let E be a B-space étalé. The space E is locally path-connected. If it is connected, it is path-connected.

The first assertion follows immediately from def. 4 and the definition of an étale mapping (I, p. 28, def. 2). The second follows from it by prop. 7.

In order that a topological space X be locally path-connected, it is necessary and sufficient that every path-connected component of an open set of X be an open set of X (cf. I, p. 85, proof of prop. 11). If the space X is locally path-connected, every point of X therefore possesses a fundamental system of open path-connected neighbourhoods.

#### Proposition 8 {#ta-iii-s2-prop-8 .statement tag=01X6}

Every quotient space of a locally path-connected space is locally path-connected.

Let X be a locally path-connected space, let R be an equivalence relation in X and let $\varphi : X\rightarrow X/R$ be the canonical mapping. It suffices to prove that the path-connected components of an open subset of $X/R$ are open. Let thus A be an open subset of $X/R$ and let C be a path-connected component of A. Let $x\in \overset{-1}{\varphi}(C)$, and let K be the path-connected component of $x$ in $\overset{-1}{\varphi}(A)$. The set $\varphi (K)$ is path-connected (III, p. 258, prop. 3), contained in A and contains $\varphi (x)$; hence $\varphi (K)\subset C$, whence $K\subset \overset{-1}{\varphi}(C)$. This proves that $\overset{-1}{\varphi}(C)$ is the union of path-connected components of $\overset{-1}{\varphi}(A)$. Since X is locally path-connected and $\overset{-1}{\varphi}(A)$ is open in X$,\overset{-1}{\varphi}(C)$ is open in X. Consequently, C is open in $X/R$. This proves the proposition.

#### Proposition 9 {#ta-iii-s2-prop-9 .statement tag=01X7}

The product of a family of locally path-connected spaces, connected with the exception of a finite number of them, is locally path-connected.

Let $(X_j)_{j\in J}$ be a family of locally path-connected spaces which are connected, with the exception of a finite number of them. Let $x=$ $(x_j)_{j\in J}$ be a point of the product space X = $\prod_{j\in J}X_j$. By assumption, a fundamental system of neighbourhoods of $x$ in X consists of sets of the form $V =\prod_{j\in J}V_j$ where, for every $j\in J$, $V_j$ is a path-connected neighbourhood of $x_j$ in $X_j$ and where $V_j= X_j$ except for a finite set of indices $j\in J$ (TG, I, p. 24). These sets being path-connected (III, p. 260, prop. 6), X is locally path-connected.

#### Corollary {#ta-iii-s2-n3-cor-1 .statement tag=01X8}

Every open subset of a numerical space is locally path-connected.

Every point of $\mathbf{R}$ possesses a basis of neighbourhoods formed by intervals; consequently, $\mathbf{R}$ is locally path-connected. According to Proposition 9, the numerical space $\mathbf{R}^n$ is locally path-connected, for every integer $n\geqslant 1$. Moreover, an open subset of a locally path-connected topological space is again path-connected, whence the corollary.

#### Example {#ta-iii-s2-n3-exa-1 .statement tag=01X9}

Let G be the subgroup of $\mathbf{G}\mathbf{L}(n,\mathbf{R})$ formed by the square matrices of order $n$ whose determinant is strictly positive. The group G is connected and locally path-connected.

According to A, III, p. 104, prop. 17, the group $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ is generated by the elements $B_{ij}(\lambda )$ (for $1\leqslant i, j\leqslant n$ such that $i=\not j$ and $\lambda \in \mathbf{R}$). The mappings $\lambda \mapsto B_{ij}(\lambda )$ from $\mathbf{R}$ into $\mathbf{G}\mathbf{L}(n,\mathbf{R})$ are continuous, their images are connected subsets of $\mathbf{S}\mathbf{L}(n,\mathbf{R})$; since they all contain the identity matrix $I_n$, their union is connected (TG, I, p. 81, prop. 2). Consequently, the group $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ is connected (TG, III, p. 8, prop. 7). Let A be the subgroup of G formed by the matrices of the form diag(1$, . . . ,1, \lambda$ ), with $\lambda \in \mathbf{R}_+^*$; it is connected and one has $\mathbf{G}\mathbf{L}(n,\mathbf{R}) = A\cdot \mathbf{S}\mathbf{L}(n,\mathbf{R})$. It follows that the group G is connected. Since it is the inverse image of $\mathbf{R}_+^*$ by the determinant mapping of $\mathbf{M}_n(\mathbf{R})$ into $\mathbf{R}$, it is an open subset of $\mathbf{M}_n(\mathbf{R})$; it is therefore locally arcwise connected (corollary above), as well as arcwise connected (III, p. 261, corollary 1).

#### Proposition 10 {#ta-iii-s2-prop-10 .statement tag=01XA}

Let X be a topological space. The mapping $(o, e)$ of $\Lambda (X) =\mathscr{C}_c(\mathbf{I}; X)$ into $X\times X$, which associates with a path $c$ in X the pair $(c(0), c(1))$, is continuous. If the space X is locally arcwise connected, this mapping is open.

We already know that the origin mappings $o$ and term $e$ of Λ(X) into X are continuous (III, p. 257), whence the first assertion.

#### Lemma {#ta-iii-s2-n3-lem-1 .statement tag=01XB}

Let $c:\mathbf{I}\rightarrow X$ be a path and let W be a neighbourhood of $c$ in the space $\mathscr{C}_c(\mathbf{I}; X)$. There exists a real number $\varepsilon \in ]0,1/2]$, a neighbourhood $V_0$ of $c(0)$ and a neighbourhood $V_1$ of $c(1)$ in X having the following properties: one has $c([0, \varepsilon ])\subset V_0,c([1-\varepsilon ,1])\subset V_1$, and every path $c':\mathbf{I}\rightarrow X$ such that

$c'(t)\in V_0$ for $0\leqslant t\leqslant \varepsilon$,

(2) $c'(t) =c(t)$ for $\varepsilon \leqslant t\leqslant 1-\varepsilon$,

$c'(t)\in V_1$ for $1-\varepsilon \leqslant t\leqslant 1$,

belongs to W.

By definition of the topology of compact convergence (TG, X, p. 26, déf. 1), there exists a finite set J, a family $(U_j)_{j\in J}$ of open sets in X and a family $(K_j)_{j\in J}$ of compact subsets of $\mathbf{I}$ such that the set $W'$ of paths $c'$ satisfying $c'(K_j)\subset U_j$ for every index $j$ is a neighbourhood of $c$ contained in W. Let us then denote by $A_0$ (resp. $A_1$) the set of indices $j$ such that $0\in K_j$ (resp. $1\in K_j$); put $V_0=\bigcap_{j\in A_0}U_j$ and $V_1=\bigcap_{j\in A_1}U_j$.

Since the mapping $c$ is continuous, there exists a real number $\varepsilon \in$ $]0,1/2]$ such that $c([0, \varepsilon ])\subset V_0,c([1-\varepsilon ,1])\subset V_1,[0, \varepsilon ]\cap K_j=\emptyset$ for all $j\notin A_0$ and $[1-\varepsilon ,1]\cap K_j=\emptyset$ for all $j\notin A_1$. Let then $c'$ be a path satisfying the conditions (2). Let us prove that $c'\in W'$. Let $j\in J$ and let $t\in K_j$. If $\varepsilon \leqslant t\leqslant 1-\varepsilon ,c'(t) =c(t)$ belongs to $U_j$. If $0\leqslant t\leqslant \varepsilon ,c'(t)\in V_0$; by the choice of $\varepsilon$, we have $j\in A_0$, hence $c'(t)\in U_j$. Analogously, if $1-\varepsilon \leqslant t\leqslant 1$, we have $j\in A_1$ and $c'(t)\in V_1\subset U_j$. Thus, $c'(K_j)\subset U_j$ and $c'$ belongs to $W'$, hence to W.

Let us now prove the second assertion of Proposition 10. Suppose that the space X is locally connected by arcs. Let $c$ be a path in X and let W be a neighbourhood of $c$ in $\mathscr{C}_c(\mathbf{I}; X)$. Let $\varepsilon ,V_0$ and $V_1$ be as in the lemma. Let $T_0$ and $T_1$ be connected by arcs neighbourhoods of $c(0)$ and $c(1)$ contained in $V_0$ and $V_1$ respectively. There exists a real number $\theta$ such that $0< \theta  < \varepsilon$ and such that $c([0, \theta ])\subset T_0,c([1-\theta ,1])\subset T_1$. Let $x_0\in T_0$ and $x_1\in T_1$; let $c_0$ be a path of origin $x_0$ and of term $c(\theta )$ in $T_0$ and let $c_1$ be a path of origin $x_1$ and of term $c(1-\theta )$ in $T_1$. Put

$c_0(t/\theta )$ for $0\leqslant t\leqslant \theta$,

$c'(t) =c(t)$ for $\theta \leqslant t\leqslant 1-\theta$,

$c_1((1-t)/\theta )$ for $1-\theta \leqslant t\leqslant 1$.

One thus defines a path $c'$ joining $x_0$ to $x_1$ and satisfying the conditions (2). This proves that the image of W in $X\times X$ by the mapping $(o, e)$ contains the neighbourhood $T_0\times T_1$ of $(c(0), c(1))$, whence the proposition.

#### Corollary {#ta-iii-s2-n3-cor-2 .statement tag=01XC}

Soit X a topological space locally connected by arcs and let $x$ be a point of X. The mapping $c\mapsto c(1)$ of $\Lambda_x(X)$ into X is open.

According to the proposition, the mapping $\varphi : \Lambda (X)\rightarrow X\times X$ defined by $\varphi (c) = (c(0), c(1))$ is open and one has $\Lambda_x(X) =\overset{-1}{\varphi}(\{x\} \times X)$. Consequently, the mapping $\Lambda_x(X)\rightarrow  \{x\} \times X$ deduced from $\varphi$ is open (TG, I, p. 30, prop. 2), as is its composite with the second projection pr$_2$.

### 4. Links between connectedness and connectedness by arcs

A space connected by arcs is connected (III, p. 258, prop. 4). There exist connected spaces, even locally connected spaces, which are not connected by arcs (cf. III, p. 331, exerc. 2 and 4). However:

#### Proposition 11 {#ta-iii-s2-prop-11 .statement tag=01XD}

A connected and locally connected topological space, whose topology can be defined by a distance for which it is complete, is connected by arcs.

Let X be a topological space. Call a train in X any nonempty finite sequence $T = (W_i)_{1\leqslant i\leqslant n}$ of connected open subsets of X such that $W_i\cap W_{i+1}=\not\emptyset$ for $1\leqslant i\leqslant n-1$. We say that $n$ is the length of the train T and that the $W_i$ are its wagons. If X is endowed with a distance compatible with its topology, we call the width of the train T the maximum of the diameters of its wagons. We say that the train joins a point $a$ to a point $b$ if $a$ belongs to the first and $b$ to the last wagon. We call a refinement of T any pair $(T', f)$ formed by a train $T'= (W'_j)_{1\leqslant j\leqslant m}$ and a strictly increasing mapping $f:\{0,1, . . . , n\} \rightarrow  \{0,1, . . . , m\}$ such that $f(0) = 0,f(n) =m$ and $W'_j\subset W_i$ for $1\leqslant i\leqslant n$ and $f(i-1)< j\leqslant f(i)$.

#### Lemma 1 {#ta-iii-s2-lem-1 .statement tag=01XE}

Let X be a connected and locally connected metric space, let $a$ and $b$ be points of X and let $\varepsilon$ be a real number $>0$. There exists in X a train of width $\leqslant \varepsilon$ joining $a$ to $b$.

More precisely, every train T joining $a$ to $b$ possesses a refinement $(T', f)$, where $T'$ is a train of width $\leqslant \varepsilon$ joining $a$ to $b$.

The relation “there exists a train of width $\leqslant \varepsilon$ joining $x$ to $y$” is an equivalence relation between $x$ and $y$ in X. The equivalence class of a point $x$ contains every connected open neighbourhood of $x$ of diameter $\leqslant \varepsilon$, and $x$ possesses such a neighbourhood since X is locally connected. The equivalence classes for this relation are therefore open, and consequently also closed. There is at most one of them, since X is connected. This proves the first assertion.

Let $T = (W_i)_{1\leqslant i\leqslant n}$ be a train in X joining $a$ to $b$. Put $x_0=a$, $x_n=b$ and choose for $1\leqslant i\leqslant n-1$ a point $x_i$ in the nonempty set $W_i\cap W_{i+1}$. For $1\leqslant i\leqslant n$, the open set $W_i$ is connected and locally connected and $x_{i-1},x_i$ are two of its points; there exists by the preceding paragraph a train $(W_{i,k})_{1\leqslant k\leqslant m_i}$ in $W_i$, of width $\leqslant \varepsilon$, joining $x_{i-1}$ to $x_i$.

Put $m=m_1+\cdots +m_n$. For $1\leqslant j\leqslant m$, put $W'_j= W_{i,k}$, where $(i, k)$ is the unique pair of integers such that $1\leqslant i\leqslant n,1\leqslant k\leqslant m_i$ and $j=m_1+\cdots +m_{i-1}+k$. For $0\leqslant i\leqslant n$, put $f(i) =m_1+\cdots +m_i$. Then $T'= (W'_j)_{1\leqslant j\leqslant m}$ is a train of width $\leqslant \varepsilon$ in X joining $a$ to $b$, and $(T', f)$ is a refinement of T.

Let us now prove Proposition 11. Equip the connected and locally connected space X with a distance $d$, compatible with its topology, for which it is complete. Let $a$ and $b$ be points of X. Lemma 1 permits us to construct by induction sequences $(T_s)_{s\geqslant 0}$ and $(f_s)_{s\geqslant 1}$ such that, for every $s\geqslant 0$, $T_s= (W_{s,i})_{1\leqslant i\leqslant n_s}$ is a train of width $\leqslant 2^{-s}$ joining $a$ to $b$ and $(T_{s+1}, f_{s+1})$ is a refinement of $T_s$.

We can choose by induction, for $s\geqslant 0$, a strictly increasing mapping $g_s:\{0,1, . . . , n_s\} \rightarrow \mathbf{I}$ such that $g_s(0) = 0$ and $g_s(n_s) = 1$, in such a way that $g_{s+1}\circ f_s=g_s$. Define, for $s\geqslant 0$, a subset $A_s$ of $\mathbf{I}\times X$ by putting

$$
A_s=\bigcup_{1\leqslant i\leqslant n_s}([g_s(i-1), g_s(i)]\times W_{s,i})
$$

The sequence $(A_s)_{s\geqslant 0}$ is decreasing: indeed, for every integer $j\in  \{1, . . . , n_{s+1}\}$, there exists a unique integer $i\in  \{1, . . . , n_s\}$ such that $f_s(i-1)< j\leqslant f_s(i)$, and one has

$$
[g_{s+1}(j-1), g_{s+1}(j)]\subset [g_s(i-1), g_s(i)],W_{s+1,j}\subset W_{s,i}
$$

Let $t\in \mathbf{I}$. For every $s\geqslant 0$, denote by $A_s(t)$ the set of the $x\in X$ such that $(t, x)\in A_s$. The set $A_s(t)$ is either one of the cars, or the union of two consecutive cars of the train $T_s$; it is therefore a nonempty subset of X, of diameter $\leqslant 2^{1-s}$. The sequence $(A_s(t))_{s\geqslant 0}$ is decreasing. The set of its terms is a Cauchy filter basis. This one converges to a point $c(t)$ since the metric space X is complete.

Since $a$ belongs to each of the sets $A_s(0) = W_{s,1}$, we have $c(0) =a$; analogously $c(1) =b$. Let $t\in \mathbf{I}$ and let $s$ be an integer $\geqslant 0$. The point $t$ possesses in $\mathbf{I}$ a neighbourhood V of one of the following forms: $[g_s(0), g_s(1)[$, $]g_s(i-1), g_s(i+ 1)[$ for an integer $i$ such that $1\leqslant i\leqslant$ $n_s-1$, or $]g_s(n_s-1), g_s(n_s)]$. According to the case, the set $c(V)$ is contained in the closure of the first car, of the union of two consecutive cars, or of the last car of the train $T_s$. It is therefore of diameter $\leqslant 2^{1-s}$, and we have $d(c(t), c(t'))\leqslant 2^{1-s}$ for $t'\in V$. This proves that the mapping $c:\mathbf{I}\rightarrow$ X is continuous. Thus $c$ is a path in X joining $a$ to $b$, and X is arcwise connected.

#### Corollary 1 {#ta-iii-s2-lem-1-cor-1 .statement tag=01XF}

A locally connected topological space, whose topology can be defined by a distance for which it is complete, is locally arcwise connected.

Let X be such a space and let U be an open and connected subset of X. According to Lemma 2 below, there exists a distance on U compatible with its topology for which U is complete. Since U is locally connected, it follows from Proposition 11 that U is arcwise connected.

#### Lemma 2 {#ta-iii-s2-lem-2 .statement tag=01XG}

Let X be a complete metric space and let U be an open subset of X. There exists a distance on U compatible with its topology for which U is complete.

We shall take up again the arguments of the proof of prop. 2 of TG, IX, p. 57. We may suppose U distinct from X. Let V be the subset of the product $\mathbf{R}\times X$ formed by the points $(t, x)$ such that $t d(x,X-U) = 1$ ; the subspace V of $\mathbf{R}\times X$ is closed and the mapping $(t, x)\mapsto x$ from V into U is a homeomorphism (TG, IX, p. 13, prop. 3). There exists on $\mathbf{R}\times X$ a distance $d'$ compatible with its topology for which $\mathbf{R}\times X$ is complete (TG, IX, p. 15, cor. 2 and TG, II, p. 17, prop. 10). The space V is complete for the distance induced by $d'$ (TG, II, p. 16, prop. 8), whence the lemma.

#### Corollary 2 {#ta-iii-s2-lem-2-cor-2 .statement tag=01XH}

A locally compact, locally connected and metrizable topological space is locally arcwise connected. If it is connected, it is arcwise connected.

It suffices to prove the first assertion (III, p. 260, prop. 7). Let X be a locally compact and locally connected metric space. The open, connected and relatively compact subsets of X constitute a basis of the topology of X. Let U be such a set; since U is an open subset of its closure, which is a compact metric space, hence complete, there exists according to Lemma 2 a distance on U compatible with its topology for which U is complete. It follows from prop. 11 of III, p. 264 that U is arcwise connected, whence the corollary.

### 5. Arcwise continuous mappings

#### Definition 5 {#ta-iii-s2-def-5 .statement tag=01XI}

Let X and Y be topological spaces. A mapping $f: X\rightarrow Y$ is said to be arcwise continuous if, for every path $c$ in X, the mapping $f\circ c:\mathbf{I}\rightarrow Y$ is continuous.

#### Remark {#ta-iii-s2-n5-rem-1 .statement tag=01XJ}

Suppose that the space X is arcwise connected. Let $x$ be a point of X. For $f$ to be arcwise continuous, it suffices that, for every path $c$ with origin $x$, the mapping $f\circ c$ be continuous. Indeed, let $d$ be an arbitrary path in X and let $c$ be a path in X with origin $x$ and with term $d(0)$. If the mapping $f\circ (c*d)$ is continuous, the same is true of the mapping $f\circ d$ because we have $f\circ d(t) =f\circ (c*d)((t+ 1)/2)$.

A continuous mapping is arcwise continuous. The converse is not always true; the propositions 12 and 13 below provide criteria making it possible to assert that an arcwise continuous mapping is continuous.

#### Proposition 12 {#ta-iii-s2-prop-12 .statement tag=01XK}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a mapping. Suppose that the space X is locally arcwise connected and that every point of X possesses a countable fundamental system of neighbourhoods. If the mapping $f$ is arcwise continuous, it is continuous.

According to (TG, IX, p. 18), it suffices to prove that, for every point $x$ of X and every sequence $(x_n)_{n\geqslant 1}$ of points of X which tends to $x$, the sequence $(f(x_n))_{n\geqslant 1}$ tends to $f(x)$. By deleting, if necessary, the first terms of the sequence $(x_n)_{n\geqslant 1}$, we reduce to the case where all the terms of the sequence belong to the same arc-connected neighbourhood of $x$ in X. According to the lemma below, there then exists a path $c:\mathbf{I}\rightarrow X$ such that $c(0) =x$ and $c(1/n) =x_n$ for $n\geqslant 1$. If the mapping $f$ is continuous by arcs, the mapping $f\circ c$ is continuous and the element $f(x) =f(c(0))$ is the limit of the sequence $(f(c(1/n)))_{n\geqslant 1}$, that is to say of the sequence $(f(x_n))_{n\geqslant 1}$, whence the corollary.

#### Lemma {#ta-iii-s2-n5-lem-1 .statement tag=01XL}

Let X be a topological space connected and locally connected by arcs and let $x$ be a point of X. Suppose that the point $x$ has a countable fundamental system of neighbourhoods. Then, for every sequence $(x_n)_{n\geqslant 1}$ of points of X tending to $x$, there exists a path $c$ in X such that $c(0) =x$ and $c(1/n) =x_n$ for $n\geqslant 1$.

Let $(W_m)_{m\geqslant 1}$ be a fundamental system of neighbourhoods of $x$. Put $V_0= X$ and for every $m\geqslant 1$, let $V_m$ be an arc-connected neighbourhood of $x$ contained in $V_{m-1}\cap W_m$.

For every integer $n\geqslant 1$, denote by $m_n$ the largest integer $m\leqslant n$ such that $x_k\in V_m$ for every $k\geqslant n$. The sequence $(m_n)_{n\geqslant 1}$ is increasing by definition; it tends to infinity, because the sequence $(x_n)_{n\geqslant 1}$ tends to $x$. For every integer $n\geqslant 1$, let $c_n:\mathbf{I}\rightarrow V_{m_n}$ be a path with origin $x_{n+1}$ and endpoint $x_n$ in $V_{m_n}$. Define a mapping $c:\mathbf{I}\rightarrow X$ by putting $c(0) =x$ and $c(t) =c_n(n(n+ 1)t-n)$ if $1/(n+ 1)< t\leqslant$ $1/n$. We have $c(1/n) =x_n$ for every $n\geqslant 1$. The mapping $c$ is therefore continuous on every interval of the form $[1/(n+ 1),1/n]$ with $n\geqslant 1$, hence on the interval $]0,1]$. If $t\leqslant 1/n$, the point $c(t)$ belongs to $V_{m_n}$; the mapping $c$ is therefore continuous at 0.

#### Proposition 13 {#ta-iii-s2-prop-13 .statement tag=01XM}

Let $p: E\rightarrow B$ be an étale and separated mapping and let $s: B\rightarrow E$ be a section of $p$. If the space B is locally path-connected and if the section $s$ is path-continuous, it is continuous.

Let $b$ be a point of B; let us prove that $s$ is continuous at the point $b$. Since $p$ is an étale mapping, there exist a neighbourhood V of $b$ and a continuous local section $s'$ of $p$ defined in V such that $s'(b) =s(b)$ (I, p. 33, prop. 9). Since B is locally path-connected, we may suppose that V is path-connected. For every path $c$ in V, with origin $b$, the mappings $s\circ c$ and $s'\circ c$ are two continuous liftings to B of the mapping $c:\mathbf{I}\rightarrow X$ and we have $s\circ c(0) =s'\circ c(0) =s(b)$. By Corollary 1 of I, p. 34, we have $s\circ c=s'\circ c$ and in particular $s\circ c(1) =s'\circ c(1)$. Since every point of V is the end point of a path in V with origin $b$, the mappings $s$ and $s'$ coincide in V. The mapping $s$ is therefore continuous in V.

#### Corollary {#ta-iii-s2-n5-cor-1 .statement tag=01XN}

Let B be a topological space, let $(E, p)$ and $(E', p')$ be two B-spaces. Suppose that the mapping $p$ is étale and separated and that the space $E'$ is locally path-connected. Then every path-continuous mapping $f: E'\rightarrow E$ such that $p\circ f=p'$ is continuous.

The mapping pr$_1: E'\times_BE\rightarrow E'$ is étale and separated (I, p. 31, prop. 8 and I, p. 27, prop. 4) and the mapping $x\mapsto (x, f(x))$ is a path-continuous section of it. By Proposition 13, it is continuous, hence $f$ is continuous.

### 6. Complements on compact metrizable topological spaces

Let us endow the set with two elements $\{0,1\}$ with the discrete topology and the set $\{0,1\}^{\mathbf{N}}$ with the product topology. The topological space $\{0,1\}^{\mathbf{N}}$ is compact (TG, I, p. 63, th. 3), metrizable (TG, IX, p. 15, cor. 2), nonempty, totally disconnected (TG, I, p. 84, prop. 10) and has no isolated point.

#### Proposition 14 {#ta-iii-s2-prop-14 .statement tag=01XO}

Every compact, metrizable, nonempty, totally disconnected topological space without isolated point is homeomorphic to $\{0,1\}^{\mathbf{N}}$.

Let X be such a topological space. Let us endow it with a distance compatible with its topology. Since the space X is compact, it is complete for this distance (TG, II, p. 27, th. 1).

#### Lemma 3 {#ta-iii-s2-lem-3 .statement tag=01XP}

Let $\varepsilon$ be a real number $>0$. There exists an integer $m\geqslant 1$ such that, for every integer $n\geqslant m$, X admits a partition formed of $n$ nonempty open and closed sets of diameter $\leqslant \varepsilon$.

Every point of X admits an open and closed neighbourhood of diameter $\leqslant \varepsilon$ (TG, II, p. 32, corollary of prop. 6). Since the space X is compact, it has a finite covering by such sets. Choose one, $(U_i)_{1\leqslant i\leqslant m}$, for which $m$ is minimal. We have $m\geqslant 1$ since X is nonempty. For $1\leqslant i\leqslant m$, denote by $V_i$ the intersection of $U_i$ and the $X-U_k$ for $k < i$. Then $(V_i)_{1\leqslant i\leqslant m}$ is a partition of X, formed of $m$ nonempty open and closed sets of diameter $\leqslant \varepsilon$.

Since X has no isolated point, every nonempty open and closed subset V of X contains at least two points. Since moreover X is compact and totally disconnected, V is the union of two disjoint nonempty open and closed subsets (loc. cit.). It follows, by induction, that for every integer $n\geqslant m$, X admits a partition formed of $n$ nonempty open and closed sets of diameter $\leqslant \varepsilon$.

Let us now finish the proof of the prop. 14. Every nonempty open and closed subspace of X is a compact, totally disconnected metric space and has no isolated point. Lemma 3 therefore allows us to construct by induction a sequence $(J_n)_{n\geqslant 0}$ of finite sets and, for every $n\geqslant 0$, a mapping $\varphi_n$ from the set $C_n= J_0\times  \cdots  \times J_n$ into the set of nonempty open and closed subsets of X of diameter $\leqslant 2^{-n}$, in such a way that :

(i) For every $n\geqslant 0$, there exists an integer $m_n\geqslant 1$ such that Card(J$_n$) $=$ $2^{m_n}$;

(ii) The family $(\varphi_0(c))_{c\in C_0}$ is a partition of X ;

(iii) For every $n\geqslant 0$ and every $c\in C_n$, the family $(\varphi_{n+1}(c, j))_{j\in J_{n+1}}$ is a partition of $\varphi_n(c)$.

Let us denote by $p_n$ the canonical projection of $C_{n+1}$ onto $C_n$. The sequence C = $(C_n, p_n)_{n\geqslant 0}$ is a sieve (TG, IX, p. 63, def. 8). The topological space associated with this sieve (TG, IX, p. 63) is identified with the topological space J, product of the discrete topological spaces $J_n$. The sieve C and the sequence of mappings $(\varphi_n)_{n\geqslant 0}$ define a strict sieving of the metric space X (TG, IX, p. 63 and p. 64). The mapping $f: J\rightarrow X$ deduced from this sieving is continuous and bijective (TG, IX, p. 65). Since the topological space J is compact (TG, I, p. 63, th. 3) and X is separated, $f$ is a homeomorphism (TG, I, p. 63, cor. 2). Since $J_n$ is homeomorphic to $\{0,1\}^{m_n}$ for every $n\geqslant 0$, J is homeomorphic to $\{0,1\}^{\mathbf{N}}$ (TG, I, p. 25, prop. 2).

#### Example {#ta-iii-s2-n6-exa-1 .statement tag=01XQ}

Let K be the triadic Cantor set (TG, IV, p. 9, example). For every $n\geqslant 0$, put $J_n=\{0,1\}$ and define a mapping $K_n$ from the set $C_n= J_0\times  \cdots  \times J_n$ into the set of closed intervals of $[0,1]$ in the following manner: put $K_0(0) = [0,\frac{1}{3}]$ and $K_0(1) = [\frac{2}{3},1]$; for every $n\geqslant 0$ and every $c\in C_n,K_{n+1}(c,0)$ and $K_{n+1}(c,1)$ are respectively the “left third” and the “right third” of $K_n(c)$. If $c= (j_0, j_1, . . . , j_n)\in C_n,K_n(c)$ is the interval denoted by $K_{n,p}$ in loc. cit., with $p= 2^nj_0+2^{n-1}j_1+\cdots +j_n+1$, it is also the interval $[a, a+\frac{1}{3^{n+1}}]$, where $a= 2(\frac{j_0}{3}+\frac{j_1}{3^2}+\cdots +\frac{j_n}{3^{n+1}})$. For $n\geqslant 0$ and $c\in C_n$, put $\varphi_n(c) = K_n(c)\cap K$. The family $(\varphi_n(c))_{c\in C_n}$ is a partition of K formed by closed sets. These sets are therefore also open in K; they are nonempty and have diameter $\frac{1}{3^{n+1}}$, because the endpoints of the intervals $K_n(c)$ belong to K. The sequence $C = (C_n, p_n)_{n\geqslant 0}$, where $p_n: C_{n+1}\rightarrow C_n$ is the canonical projection $(c, j)\mapsto c$, is a sieve, and the topological space associated with this sieve is identified with $\{0,1\}^{\mathbf{N}}$. The sieve C and the sequence of mappings $(\varphi_n)_{n\geqslant 0}$ define a strict sieving of the metric space K. The mapping $f:\{0,1\}^{\mathbf{N}}\rightarrow K$ deduced from this sieving is a homeomorphism, given by the formula

$$
f((j_n)_{n\geqslant 0}) = 2\sum_{n=0}^{\infty}\frac{j_n}{3^{n+1}}
$$

#### Corollary {#ta-iii-s2-n6-cor-1 .statement tag=01XR}

Let X be a metrizable, compact and nonempty topological space. There exists a continuous and surjective mapping from $\{0,1\}^{\mathbf{N}}$ into X.

Every compact and metrizable topological space is homeomorphic to a necessarily closed subspace of the topological space $\mathbf{I}^{\mathbf{N}}$ (TG, IX, p. 18, prop. 12 and p. 21, prop. 16). Let A be a closed subspace of $\mathbf{I}^{\mathbf{N}}$ and $h$ a homeomorphism of A onto X.

Let K = $\{0,1\}^{\mathbf{N}}$ and, for $\alpha = (a_n)\in$ K, put $f(\alpha ) =$ $\sum^{\infty}_{n=0}a_n2^{-n-1}$; we have $f(\alpha )\in \mathbf{I}$. The mapping $f: K\rightarrow \mathbf{I}$ thus resulting is surjective (TG, IV, p. 42) and continuous. Indeed, if two elements $\alpha$ and $\beta$ of K have the same coordinates of index $< n$, we have $|f(\beta )-f(\alpha )|\leqslant 2^{-n}$. Let $g$ denote the mapping $(\alpha_n)\mapsto (f(\alpha_n))$ of $K^{\mathbf{N}}$ into $\mathbf{I}^{\mathbf{N}}$; it is continuous and surjective. The topological space $K^{\mathbf{N}}$ is compact (TG, I, p. 63, th. 3), metrizable (TG, IX, p. 15, cor. 2) and totally disconnected (TG, I, p. 84, prop. 10) and the same is true of its closed subspace $\overset{-1}{g}(A)$; the latter is nonempty since the mappings $g$ and $h$ are surjective.

Then, the space $\overset{-1}{g}(A)\times K$ is homeomorphic to $\{0,1\}^{\mathbf{N}}$ (prop. 14), since it is a compact, metrizable, totally disconnected topological space without isolated point and the mapping $(x, y)\mapsto h(g(x))$ of $\overset{-1}{g}(A)\times K$ into X is continuous surjective.

### 7. Topological properties of the image of a path

#### Proposition 15 {#ta-iii-s2-prop-15 .statement tag=01XS}

The image of a path in a separated topological space is a compact, metrizable, connected and locally connected by arcs topological space.

Let X be a separated topological space and $c:\mathbf{I}\rightarrow X$ a continuous mapping. Let R denote the equivalence relation $c(s) =c(t)$ in $\mathbf{I}$. The topological space $c(\mathbf{I})$ is separated (TG, I, p. 63, cor. 1), the space $\mathbf{I}/R$ is quasi-compact (TG, I, p. 62, th. 2), hence the bijection $\mathbf{I}/R\rightarrow c(\mathbf{I})$ deduced from $c$ is a homeomorphism (TG, I, p. 63, cor. 2). Consequently, the space $c(\mathbf{I})$ is compact, metrizable (TG, IX, p. 22, prop. 17), connected (TG, I, p. 82, prop. 6) and locally connected by arcs (III, p. 261, prop. 8).

#### Theorem 1 (Hahn and Mazurkiewicz) {#ta-iii-s2-thm-1 .statement tag=01XT}

Every metrizable, compact, nonempty, connected and locally connected topological space is homeomorphic to a quotient space of the segment $[0,1]$.

#### Lemma 4 {#ta-iii-s2-lem-4 .statement tag=01XU}

Let K be a compact topological space and let $\mathscr{R}$ be a set of open subsets of K covering K. There exists an entourage V of the uniform structure of K (TG, II, p. 27, th. 1) such that, for every $x\in K$, $V(x)$ is contained in one of the sets belonging to $\mathscr{R}$.

For every point $x$ of K, there exists an entourage $W_x$ of the uniform structure of K such that $W_x(x)$ is contained in one of the sets belonging to $\mathscr{R}$. Let $V_x$ be an entourage of the uniform structure of K such that $\overset{2}{V_{x}}$ is contained in $W_x$. The interiors of the $V_x(x)$ cover K; since the space K is compact, there exists a finite subset F of K such that the family $(V_y(y))_{y\in F}$ is a covering of K (TG, I, p. 59). Let V denote the intersection of the family $(V_y)_{y\in F}$; the set V is an entourage of the uniform structure of K. For every point $x\in K$, there exists a point $y\in F$ such that $x$ belongs to $V_y(y)$. Consequently, the set

$V(x)$ is contained in $\overset{2}{V_{y}}(y)$, hence in one of the sets belonging to $\mathscr{R}$.

#### Lemma 5 {#ta-iii-s2-lem-5 .statement tag=01XV}

Let X and Y be uniform spaces and $f$ a mapping of X into Y. Let $\mathscr{F}$ be a set of closed subsets of X covering X and possessing the following properties:

(i) There exists a set $F_0\in \mathscr{F}$ which meets all the sets $F\in \mathscr{F}$;

(ii) For every entourage U of the uniform structure of X, there are only a finite number of sets $F\in \mathscr{F}$ which are not small of order U;

(iii) For every entourage V of the uniform structure of Y, there are only a finite number of sets $F\in \mathscr{F}$ such that $f(F)$ is not small of order V.

Thus, if the restriction of $f$ to each of the sets $F\in \mathscr{F}$ is continuous, $f$ is continuous.

Let $x$ be a point of X. Let us prove that $f$ is continuous at $x$. There exists a set $F_1\in \mathscr{F}$ such that $x\in F_1$. The restriction of $f$ to $F_0\cup F_1$ is continuous (TG, I, p. 19, prop. 4). By replacing $F_0$ by $F_0\cup F_1$, we reduce to the case where $x\in F_0$.

Let V be an entourage of the uniform structure of Y. Choose

an entourage $V'$ of this same uniform structure such that $\overset{2}{V'}\subset V$. Since the restriction of $f$ to $F_0$ is continuous, there exists an entourage U of the uniform structure of X such that $f(z)\in V'(f(x))$ for every $z\in F_0\cap U(x)$. Let $U'$ be an entourage of the uniform structure of X

such that $\overset{2}{U'}\subset U$. Let A denote the union of $F_0$, of the sets $F\in \mathscr{F}$ which are not small of order $U'$ and of those such that $f(F)$ is not small of order $V'$. By assumption, A is the union of a finite number of sets belonging to $\mathscr{F}$, and the restriction of $f$ to A is continuous (loc. cit.). There therefore exists a neighbourhood W of $x$ in X, contained in $U'(x)$, such that $f(y)\in V(f(x))$ for $y\in A\cap W$. To conclude, it will suffice to prove that one also has $f(y)\in V(f(x))$ for every point $y\in (X-A)\cap W$. Let $y$ be such a point. Let F be an element of $\mathscr{F}$ such that $y\in F$. By definition of A, F is small of order $U'$ and $f(F)$ is small of order $V'$. By assumption, F meets $F_0$. Let $z\in F\cap F_0$. We have $z\in U'(y)$ since F is small of order $U'$ and $y\in U'(x)$ since W

is contained in $U'(x)$, whence $z\in \overset{2}{U'}(x)$ and fortiori $z\in U(x)$. But then, since $z$ belongs to $F_0$, we have $f(z)\in V'(f(x))$. Moreover $f(F)$ is small of order $V'$, whence $f(y)\in V'(f(z))$. It follows that we have

$f(y)\in \overset{2}{V'}(f(x))$ and finally $f(y)\in V(f(x))$. This concludes the proof of lemma 5.

Let us now prove theorem 1. Let X be a compact nonempty, connected and locally connected metric space. Such a space is connected by arcs and locally connected by arcs (III, p. 267, corollary 2). According to the corollary and the example of III, p. 270, there exists a continuous and surjective mapping $f$ from the triadic Cantor set K (TG, IV, p. 9, example) into X. We shall construct a continuous extension $g$ of $f$ to $[0,1]$, which will prove theorem 1.

Let $\varepsilon$ be a real number $>0$. The open and arcwise connected subsets of X of diameter $\leqslant \varepsilon$ cover X. Let $\mathscr{R}$ denote the set of their inverse images by $f$: it is a set of open sets of K covering K. According to Lemma 4 of III, p. 272, there exists a real number $\alpha  >0$ such that every closed ball of K of radius $\alpha$ is contained in an element of $\mathscr{R}$. In particular, if $t$ and $t'$ are points of K such that $|t-t'|\leqslant \alpha$, there exists a path in X joining $f(t)$ to $f(t')$ whose image has diameter $\leqslant \varepsilon$.

The preceding paragraph makes it possible to construct by induction a strictly increasing sequence $(n_k)_{k\geqslant 0}$ of integers $\geqslant$ 0 possessing the following property: for every integer $k\geqslant 0$ and every pair $(t, t')$ of points of K such that $|t-t'|\leqslant 3^{-n_k}$, there exists a path in X joining $f(t)$ to $f(t')$ whose image has diameter $\leqslant 2^{-k}$. The complement of K in $[0,1]$ is the union of a family $(I_{n,p})$ of pairwise disjoint open intervals, where $n$ runs through the set of integers $\geqslant 0$ and $p$ the set of integers between 1 and $2^n$ (TG, IV, p. 9, example). Consider one of these intervals $I_{n,p}$ and write it $]a, b[$. The points $a$ and $b$ belong to K and we have $b-a= 3^{-n-1}$. The function $g$ is defined on the interval $I_{n,p}$ in the following way: one chooses a path $c$ in X joining $f(a)$ to $f(b)$, whose image has diameter $\leqslant 2^{-k}$ if $n_k\leqslant n < n_{k+1}$, and one sets $g(t) =c(\frac{t-a}{b-a})$ for $t\in I_{n,p}$. The function $g: [0,1]\rightarrow X$ thus defined extends $f$. It is continuous on K as well as on each of the closed intervals $\overline{I_{n,p}}$. The latter meet K. Moreover, for every real number $\varepsilon  >0$, there are only finitely many intervals $\overline{I_{n,p}}$ of length $> \varepsilon$, and there are only finitely many intervals $\overline{I_{n,p}}$ whose images by $g$ have diameter $> \varepsilon$. According to Lemma 5, the mapping $g$ is continuous.

### 8. Characterizations of the interval

#### Lemma 6 {#ta-iii-s2-lem-6 .statement tag=01XW}

Let D be a countable totally ordered set, not reduced to one element, possessing a smallest and a greatest element. Suppose that D has no gap (E, III, p. 73, exerc. 19), that is to say that every open interval $]x, y[$, where $x$ and $y$ are elements of D such that $x < y$, is nonempty. There then exists an isomorphism of ordered sets from $\mathbf{I}\cap \mathbf{Q}$ onto D.

Let $a$ be the smallest element and $b$ the greatest element of D. By assumption, we have $b=\not a$ and $]a, x[=\not\emptyset$ for every $x\in D-\{a\}$. The set D$-\{a\}$ is totally ordered, is not empty and has no smallest element; it is therefore infinite (E, III, p. 34, cor. 1 of prop. 3). The sets $\mathbf{I}\cap \mathbf{Q}$ and D, infinite and countable, are equipotent to $\mathbf{N}$.

Choose bijections $n\mapsto a_n$ and $n\mapsto b_n$ of $\mathbf{N}$ onto $\mathbf{I}\cap \mathbf{Q}$ and D respectively, such that $a_0= 0,a_1= 1,b_0=a,b_1=b$. There exists a unique strictly increasing mapping $f:\mathbf{I}\cap \mathbf{Q}\rightarrow D$ possessing the following properties: we have $f(0) =a$ and $f(1) =b$; for $n\geqslant 2$, we have $f(a_n) =b_m$, where $m$ is the smallest natural number for which the mapping of $\{a_0, . . . , a_n\}$ into D which coincides with $f$ in $\{a_0, . . . , a_{n-1}\}$ and maps $a_n$ onto $b_m$ is strictly increasing. These properties indeed define $f(a_n)$ by induction on $n$, the existence of the integer $m$ being ensured by the fact that D is without gaps.

Since the mapping $f$ is strictly increasing and $\mathbf{I}\cap \mathbf{Q}$ is totally ordered, $f$ defines an isomorphism of ordered sets from $\mathbf{I}\cap \mathbf{Q}$ onto its image (E, III, p. 14, prop. 11). It remains for us to prove that $f$ is surjective. For this, let us prove by induction that $b_m$ belongs to the image of $f$ for every $m\in \mathbf{N}$.

One has $b_0=f(0)$ and $b_1=f(1)$. Suppose that we have $m\geqslant 2$ and that, for $0\leqslant k\leqslant m-1$, there exists $c_k\in \mathbf{I}\cap \mathbf{Q}$ such that $f(c_k) =b_k$. We have $c_0= 0$ and $c_1= 1$, since $f$ is injective. Consider the smallest integer $n\in \mathbf{N}$ for which $a_n$ does not belong to $\{c_0, . . . , c_{m-1}\}$ and the mapping $g$ of $\{c_0, . . . , c_{m-1}, a_n\}$ into D which coincides with $f$ in $\{c_0, . . . , c_{m-1}\}$ and maps $a_n$ onto $b_m$ is strictly increasing; such an integer exists since $\mathbf{I}\cap \mathbf{Q}$ has no gap. Let $f'$ be the mapping of $\{a_0, . . . , a_n\}$ into D which coincides with $f$ in $\{a_0, . . . , a_{n-1}\}$ and which maps $a_n$ onto $b_m$. Let us prove that it is strictly increasing. Let $j\in  \{0, . . . , n-1\}$; by definition of the integer $n$, there exists $k\in  \{0, . . . , m-1\}$ such that $a_j=c_k$, or $a_j< c_k$ and $b_m\geqslant f(c_k)$, or $a_j> c_k$ and $b_m\leqslant f(c_k)$. Suppose $b_k< b_m$; we then have $g(c_k) =f(c_k) =b_k< b_m=g(a_n)$, whence $c_k< a_n$ since $g$ is strictly increasing, then $a_j\leqslant c_k< a_n$; moreover, $f'(a_j) =$ $f(a_j)\leqslant f(c_k) =b_k< b_m=f'(a_n)$. Analogously, if $b_k> b_m$, we obtain $a_n< c_k\leqslant a_j$ and $f'(a_j) =f(a_j)\geqslant f(c_k) =b_k> b_m=f'(a_n)$. Since $f$ itself is strictly increasing, it follows that the mapping $f'$ is strictly increasing.

If $m'$ is the integer such that $f(a_n) =b_{m'}$, we have $m'\leqslant m$, by definition of $f$. If we had $m'< m$, we would have $f(a_n) =b_{m'}=f(c_{m'})$, whence $a_n=c_{m'}$, since $f$ is injective, which contradicts the definition of $a_n$. Thus, $m'=m$ and $f(a_n) =b_m$, which proves that $b_m$ belongs to the image of $f$ and completes by induction the proof of the surjectivity of $f$.

#### Proposition 16 {#ta-iii-s2-prop-16 .statement tag=01XX}

Let E be a totally ordered set not reduced to one element. Suppose that every subset of E has a supremum and that there exists a countable subset of E which meets every open interval $]x, y[$, where $x$ and $y$ are elements of E such that $x < y$. There then exists an isomorphism of ordered sets of $\mathbf{I}$ onto E.

Since $\emptyset$ and E each have a supremum in E, E has a smallest element $a$ and a greatest element $b$. These are distinct since E is not reduced to one element. Let $D'$ be a countable subset of E which meets every open interval of E of the form $]x, y[$, with $x < y$. Put $D = D'\cup  \{a, b\}$. The set D is totally ordered and without gaps. By lemma 6, there exists an isomorphism of ordered sets $f$ of $\mathbf{I}\cap \mathbf{Q}$ onto D.

For every $t\in \mathbf{I}$, let $g(t)$ be the supremum of $f([0, t]\cap \mathbf{Q})$ in E. For every $x\in E$, let $h(x)$ be the supremum of $f^{-1}([a, x]\cap D)$ in $\mathbf{I}$. The mappings $g:\mathbf{I}\rightarrow E$ and $h: E\rightarrow \mathbf{I}$ thus defined are increasing, $g$ coincides with $f$ in $\mathbf{I}\cap \mathbf{Q}$ and $h$ coincides with $f^{-1}$ in D.

We therefore have $g(h(y)) =y$ for every $y\in D$. Let $x\in E$. If one had $g(h(x))> x$, the interval $]x, g(h(x))[$ would contain a point $y$ of D and the relations $g(h(y)) =y < g(h(x))$ would contradict the fact that $g\circ h$ is increasing. Analogously, one does not have $g(h(x))< x$. We therefore have $g(h(x)) =x$, which proves that $g\circ h$ is the identity mapping of E. One proves analogously that $h\circ g$ is the identity mapping of $\mathbf{I}$. Thus, $g:\mathbf{I}\rightarrow E$ and $h: E\rightarrow \mathbf{I}$ are reciprocal isomorphisms of ordered sets.

#### Remark {#ta-iii-s2-n8-rem-1 .statement tag=01XY}

Let E be a totally ordered set. The set of open intervals of E (bounded or not) is stable under finite intersection. It is a basis of a topology $\mathscr{T}_0(E)$ on E (TG, I, p. 91, exerc. 5). The topology $\mathscr{T}_0(\mathbf{I})$ is identical with the topology induced on $\mathbf{I}$ by that of $\mathbf{R}$. It follows that, in prop. 16, every isomorphism of ordered sets of $\mathbf{I}$ onto E is a homeomorphism of $\mathbf{I}$ onto the topological space obtained by endowing E with the topology $\mathscr{T}_0(E)$.

#### Corollary {#ta-iii-s2-n8-cor-1 .statement tag=01XZ}

Let R be an equivalence relation in $\mathbf{I}$. The following conditions are equivalent:

(i) Every equivalence class according to R is a closed interval of $\mathbf{I}$, distinct from $\mathbf{I}$;

(ii) There exists an increasing surjective mapping $u:\mathbf{I}\rightarrow \mathbf{I}$ such that R is the equivalence relation associated with $u$.

Such a mapping $u$, when it exists, is continuous and defines by passing to the quotient a homeomorphism of $\mathbf{I}/R$ onto $\mathbf{I}$.

We shall denote by $p:\mathbf{I}\rightarrow \mathbf{I}/R$ the canonical surjection.

Suppose condition (i) is satisfied. For A and B equivalence classes following R, write $A<B$ if one has $a < b$ for every $a\in A$ and every $b\in B$. In $\mathbf{I}/R$, the relation « A = B or $A<B$ » is an order relation. Indeed, it is reflexive; it is antisymmetric since one cannot have simultaneously $A<B$ and $B<A$; it is transitive since the relations $A<B$ and $B<C$ imply $A<C$. If A and B are distinct elements of $\mathbf{I}/R$, they are disjoint closed intervals of $\mathbf{I}$, and one then has either $A<B$, or $B<A$. Endowed with the order relation thus defined, $\mathbf{I}/R$ is therefore totally ordered. The mapping $p:\mathbf{I}\rightarrow \mathbf{I}/R$ is increasing.

The set $\mathbf{I}/R$ is not reduced to one element, by virtue of (i).

Let F be a subset of $\mathbf{I}/R$. Let us prove that F has a least upper bound in $\mathbf{I}/R$. Put $F'=\overset{-1}{p}(F)$; denote by $a$ the least upper bound of $F'$ in $\mathbf{I}$ and by A the equivalence class of $a$ following R. Since $a$ is an upper bound of $F'$ in $\mathbf{I}$, A is an upper bound of F in $\mathbf{I}/R$. Conversely, let $B\in \mathbf{I}/R$ be an upper bound of F; put $b=$ sup(B). Every element of $F'$ is then bounded above by $b$. We therefore have $a\leqslant b$. Since the equivalence classes following R are closed intervals, $a$ belongs to A and $b$ to B. Consequently we have $A =p(a)\leqslant p(b) = B$. This proves that A is the least upper bound of F.

Let A and B be elements of $\mathbf{I}/R$ such that $A<B$. Let $a$ be the greatest lower bound of A and $b$ the least upper bound of B. Since $a\in A$ and $b\in B$, we have $a < b$. The equivalence class following R of any element of $]a, b[$ is an element of the interval $]A,B[$ of $\mathbf{I}/R$. Since $\mathbf{I}\cap \mathbf{Q}$ meets $]a, b[$, its image by $p$ meets $]A,B[$.

We have thus proved that the totally ordered set $\mathbf{I}/R$ satisfies the hypotheses of prop. 16. There therefore exists an isomorphism of ordered sets $f:\mathbf{I}/R\rightarrow \mathbf{I}$. The mapping $u=f\circ p$ is a surjective and increasing mapping of $\mathbf{I}$ onto $\mathbf{I}$ and the equivalence relation associated with $u$ is the relation R; this proves that condition (ii) is satisfied.

Conversely, suppose that condition (ii) is satisfied. Let $u:\mathbf{I}\rightarrow \mathbf{I}$ be an increasing and surjective mapping such that R is the equivalence relation associated with $u$.

Let $a$ be a point of $\mathbf{I}$. The set $A =\overset{-1}{u}(a)$ is an interval of $\mathbf{I}$, since the mapping $u$ is increasing. Since $u$ is surjective, A is neither empty nor equal to $\mathbf{I}$. Let $b$ be the greatest lower bound of A in $\mathbf{I}$. We have $u(b)\geqslant a$. If $u(b)> a$, there exist $c\in ]a, u(b)[$ and $d\in \mathbf{I}$ such that $u(d) =c$ since $u$ is surjective. Since $u$ is increasing and $a < u(d)< u(b),d$ majorizes every element of A and we have $d < b$, which contradicts the assumption that $b$ is the greatest lower bound of A. We therefore have $u(b) =a$, that is to say $b\in A$. Analogously one proves that A contains its greatest lower bound. The set A is therefore a closed interval of $\mathbf{I}$, distinct from $\mathbf{I}$. This proves that condition (i) is satisfied.

Let us now prove that the mapping $u$ is continuous. It suffices for this to prove that, for every $a\in \mathbf{I}$, the sets $\overset{-1}{u}(]a,\rightarrow [)$ and $\overset{-1}{u}(]\leftarrow , a[)$ are open. Let $b$ be the greatest lower bound of $\overset{-1}{u}(a)$; we have $u(b) =a$. If $x\in \mathbf{I}$ satisfies $u(x)> a$, we necessarily have $x > b$; conversely, if $x > b$, we have $u(x)\geqslant a$ and $u(x)=\not a$ since $b$ is the greatest lower bound of $\overset{-1}{u}(a)$. Consequently $\overset{-1}{u}(]a,\rightarrow [) = ]b,\rightarrow [$, which proves that the inverse image by $u$ of the interval $]a,\rightarrow [$ is open. Analogously one proves that that of $]\leftarrow , a[$ is open. It follows that the mapping $u$ is continuous.

The mapping $v:\mathbf{I}/R\rightarrow \mathbf{I}$ deduced from $u$ by passing to the quotient is then continuous and bijective. Since $\mathbf{I}$ is compact, $\mathbf{I}/R$ is quasi-compact (TG, I, p. 62, th. 2) and $v$ is a homeomorphism (TG, I, p. 63, cor. 2).

#### Proposition 17 {#ta-iii-s2-prop-17 .statement tag=01Y0}

Let X be a connected and compact topological space. Let $a$ be a point of X, let U be a nonempty open and closed subset of X $-\{a\}$.

(a) The closure $\overline{U}$ of U in X is equal to $U\cup  \{a\}$ and is connected.

b) Let $a'$ be a point of X distinct from $a$, and let $U'$ be a nonempty open and closed subset of X $-\{a'\}$. If $a\notin U'$ and if $\overline{U}\cap \overline{U'}=\not\emptyset$, then $\overline{U'}\subset U$. Conversely, if $a\in U'$ and X $= U\not\cup U'$, then $\overline{U}\subset U'$.

c) There exists a point $b$ of U such that X $-\{b\}$ is connected.

Let us prove assertion a). Denote by V the complement of U in X $-\{a\}$. Since U is closed in X $-\{a\}$, V is open in X$-\{a\}$ and fortiori in X. We therefore have $U\subset \overline{U}\subset X-V = U\cup \{a\}$. Analogously, U is an open subset of X. Since X is connected, U is not closed in X, whence the equality $\overline{U}= U\cup  \{a\}$. We likewise have $\overline{V}= V\cup  \{a\}$.

Let F and G be disjoint closed subsets of $\overline{U}$ such that $U = F\cup G$. Suppose that $a\in G$ and let us prove that F is empty; one would reason in the same way if $a\in F$. The set $G\cup V = G\cup \overline{V}$ is a closed subset of X, disjoint from F, and we have $X =\overline{U}\cup V = F\cup (G\cup V)$. Since X is connected and G is not empty, F is empty. This proves that $\overline{U}$ is connected.

Let us prove b). Suppose that $a\notin U'$ and that $\overline{U}\cap \overline{U'}=\not\emptyset$. By assertion a), we have $U = U\cup  \{a\}$ and $\overline{U'}= U'\cup  \{a'\}$. Since $a\notin U'$ and $a=\not a'$, the subsets U and $\overline{U'}$ have a common point. Still by a), $\overline{U'}$ is a connected subset of X; since it is contained in X$-\{a\}$ and it meets the open and closed subset U of the latter, we have $\overline{U'}\subset U$, which was to be proved. The second assertion follows from the first by considering the complements in X of $\overline{U}$ and $\overline{U'}$ respectively.

Let us finally prove assertion c). Suppose, by contradiction, that, for every $x\in U$, the set X $-\{x\}$ is not connected and choose subsets $U_x$ and $V_x$, open and closed in X $-\{x\}$, disjoint and nonempty, such that X $-\{x\}= U_x\cup V_x$ and $a\in V_x$. By assertion b), applied to the open and closed subsets U, $U_x$ of X$-\{a\}$ and X$-\{x\}$ respectively, we have $\overline{U_x}\subset U$ for every $x\in U$. Let $x$ and $y$ be points of U such that $x\in U_y$; we then have $x=\not y$. Again by assertion b), applied to the open and closed subsets $U_x$ and $U_y$ of X $-\{x\}$ and X $-\{y\}$, the relation $x\in U_y$ implies the relation $\overline{U_x}\subset \overline{U_y}$. Consequently, the relations $x\in U_y$ and $\overline{U_x}\subset \overline{U_y}$ are equivalent.

The set of subsets S of U such that $\bigcap_{x\in S}\overline{U_x}=\not\emptyset$ is of finite character (E, III, p. 34), since the space X is compact. By E, III, p. 35, th. 1, there exists a maximal subset S of U such that $C =\bigcap_{x\in S}\overline{U_x}$ is not empty. Let $c$ be a point of C. For every element $x$ of S, we have $c\in \overline{U_x}$, whence $c\in U$ and then $\overline{U_c}\subset \overline{U_x}$. Consequently, we have $\overline{U_c}\subset C$ and then, by maximality of S, $C = U_c$. For every $x\in C$ such that $x=\not c$, we also have $\overline{U_x}\subset \overline{U_c}$ and $\overline{U_x}= U\not_c$. By maximality of S, $C =\{c\}$, hence $\overline{U_c}=\{c\}$, which contradicts the hypothesis that $U_c$ is a nonempty open and closed subset of X $-\{c\}$.

#### Corollary {#ta-iii-s2-n8-cor-2 .statement tag=01Y1}

Let X be a compact connected topological space, let N be the set of points of X whose complement is connected. The set X is the unique connected and compact subset of X which contains N.

Let S be a connected and compact subset of X such that $N\subset S$. Suppose that S $= X\not$ and let $x\in X-S$. By hypothesis, X $-\{x\}$ is not connected; there therefore exist open and closed subsets U and V of X $-\{x\}$, disjoint and nonempty, such that X $-\{x\}= U\cup V$. We may suppose that $S\subset V$. We have $\overline{U}= U\cup \{x\}$ and $V = V\cup  \{x\}$ and these spaces are connected (III, p. 278, prop. 17, a)). By assertion c) of this proposition, there exists $y\in U$ such that X $-\{y\}$ is connected, which contradicts the inclusions $N\subset S\subset V$.

#### Lemma 7 {#ta-iii-s2-lem-7 .statement tag=01Y2}

Soit T un espace topologique localement connexe. Soit $\mathscr{U}$ un ensemble filtrant croissant de parties ouvertes de T, de réunion T. Pour $t\in T$ et $U\in \mathscr{U}$, notons $U_t$ la composante connexe de $t$ dans U si $t\in U$ et posons $U_t=\emptyset$ si $t\notin U$. Pour tout $t\in T,\bigcup_{U\in\mathscr{U}}U_t$ est la composante connexe de $t$ dans T.

For $t\in T$, put $C_t=\bigcup_{U\in\mathscr{U}}U_t$. We have $t\in C_t$. The sets $U_t$ are open and connected and the same is true of $C_t$ since we have $t\in U_t$ if $U_t=\not\emptyset$ (TG, I, p. 81, prop. 2). Let $u,v$ be points of T such that $C_u\cap C_v=\not\emptyset$. Let $t$ be a point of $C_u\cap C_v$; let $U\in \mathscr{U}$ be such that $t\in U_u$ and let $V\in \mathscr{U}$ be such that $v\in V_v$. Since $\mathscr{U}$ is increasing filtrant, there exists $W\in \mathscr{U}$ which contains $U\cup V$. Then, $W_u\cap W_v=\not\emptyset$, hence $W_u= W_v$. More generally, one has $W'_u= W'_v$ for every $W'\in \mathscr{U}$ such that $W\subset W'$, hence $C_u= C_v$. This proves that the sets of the form $C_t$ form a partition of T into open connected subsets. Consequently, for every $t\in T$, $C_t$ is the connected component of $t$ in T.

#### Theorem 2 {#ta-iii-s2-thm-2 .statement tag=01Y3}

Let X be a compact connected topological space possessing a countable everywhere dense subset. Let $a,b$ be distinct points of X. The following conditions are equivalent:

(i) There exists a homeomorphism $f:\mathbf{I}\rightarrow X$ such that $f(0) =a$ and $f(1) =b$;

(ii) Every connected subset of X which contains $\{a, b\}$ is equal to X ;

(iii) The space X is locally connected and every connected compact subset of X which contains $\{a, b\}$ is equal to X ;

(iv) For every $x\in X-\{a, b\}$, the space X $-\{x\}$ is not connected.

Assertion (i) implies all the others.

Let $x$ be a point of X $-\{a, b\}$. Since X $-\{x\}$ contains $\{a, b\}$, assertion (ii) implies that it is not a connected subset of X, so that (ii) implies (iv).

Let us show that (iii) implies (iv). Suppose the assumptions of (iii) are satisfied. Let $x\in X-\{a, b\}$ and suppose that X$-\{x\}$ is connected. Let T be the space X $-\{x\}$ and let $\mathscr{U}$ be the set of subsets of T of the form X-V, where V is a compact neighbourhood of $x$. By Lemma 7, there exists a compact neighbourhood V of $x$ such that $a$ and $b$ belong to the same connected component of X-V. They belong in particular to the same connected component of $X-\mathring{V}$; this is a compact connected set of X, distinct from X, which contradicts the assumption (iii).

It remains to prove that assertion (iv) implies condition (i).

Let $x$ be a point of X $-\{a, b\}$ and let U, V be open and closed, disjoint and nonempty subsets of X$-\{x\}$, such that X$-\{x\}= U\cup V$. According to III, p. 278, prop. 17, c), there exists a point of U (resp. of V) whose complement in X is connected. Since X admits only two such points, $a$ and $b$, one of them, say $a$, is contained in U and the other in V. According to loc. cit., a nonempty open and closed subset, $U'$ of U, contains a point of $\{a, b\}$, hence contains $a$. Applying this to $U-U'$, it follows that $U = U'$. Consequently, U is connected; it is the connected component of $a$ in X$-\{x\}$. Analogously, V is the connected component of $b$ in X $-\{x\}$.

For every $x\in X-\{a, b\}$, denote thus by $U_x$ and $V_x$ the connected components of $a$ and $b$ in X $-\{x\}$. From what precedes, they are open and closed in X $-\{x\}$, disjoint, and their union is equal to X $-\{x\}$.

Denote by $\preccurlyeq$ the relation in X defined in the following way: on the one hand, $a\preccurlyeq x$ and $x\preccurlyeq b$ for every $x\in X$, on the other hand, if $x$ and $y$ belong to X $-\{a, b\}$, then $x\preccurlyeq y$ if $x\in \overline{U_y}$. For $x$ and $y$ in X $-\{a, b\}$, the subsets $V_x$ and $V_y$ have the point $b$ in common, the relation $x\preccurlyeq y$ is in fact equivalent to the assertion $\overline{U_x}\subset \overline{U_y}($III, p. 278, prop. 17, b)). It follows that the relation $\preccurlyeq$ is an order relation in X.

Let $x$ and $y$ be points of X such that one does not have $x\preccurlyeq y$. Necessarily, $x=\not a$ and $y=\not b$, and $x\in V_y$. If $x=b$ or $y=a$, one has $y\preccurlyeq x$. Suppose then that $x$ and $y$ are distinct from $a$ and $b$. Since the parts $U_x$ and $U_y$ have the point $a$ in common, one has the inclusion $\overline{V_x}\subset \overline{V_y}($loc. cit.), whence, taking the closures of the complements, $\overline{U_y}\subset \overline{U_x}$ and, fortiori, $y\preccurlyeq x$. The relation $\preccurlyeq$ in the space X is therefore a total order relation. For every $x\in X-\{a, b\}$, one moreover has $U_x= ]\leftarrow , x[$ and $V_x= ]x,\rightarrow [$; for $x, y\in X-\{a, b\}$, one has $]x, y[ = U_y\cap V_x$. When $x, y$ run through the points of X $-\{a, b\}$, the sets $U_y\cap V_x$, the sets $U_y$ and the sets $V_x$ form a basis of a topology on X. Let $\widetilde{X}$ be the topological space corresponding to it and let $i: X\rightarrow \widetilde{X}$ be the identical mapping of X. Since, for every $x\in X$, the sets $U_x$ and $V_x$ are open in X, the mapping $i$ is continuous.

The space $\widetilde{X}$ is separated. Indeed, let $x$ and $y$ be distinct points of $\widetilde{X}$ such that $x\preccurlyeq y$. The parts $]\leftarrow , y[$ and $]x,\rightarrow [$ are open neighbourhoods of $x$ and $y$; if they have a common point $z,]\leftarrow , z[$ and $]z,\rightarrow [$ are then disjoint open neighbourhoods of $x$ and $y$. Since X is compact, the mapping $i$ is therefore a homeomorphism (TG, I, p. 63, cor. 2).

Consequently, the image by $i$ of a countable everywhere dense subset of X meets every nonempty open interval of the ordered set $(X,\preccurlyeq )$. It follows then from Prop. 16 of III, p. 276 that there exists an isomorphism $c$ of the ordered set $\mathbf{I}$ onto $(X,\prec )$. According to the remark following this proposition, this isomorphism is a homeomorphism of $\mathbf{I}$ onto the topological space $\widetilde{X}$. The mapping $f=i^{-1}\circ c$ is then a homeomorphism of $\mathbf{I}$ onto X which maps 0 onto $a$ and 1 onto $b$.

### 9. Injective paths

#### Proposition 18 {#ta-iii-s2-prop-18 .statement tag=01Y4}

Let X be a separated topological space. Let $a$ and $b$ be distinct points of X which belong to the same arcwise connected component of X. There exists an injective path joining $a$ to $b$ in X.

Let $f:\mathbf{I}\rightarrow X$ be a path joining $a$ to $b$ in X. Let $\mathscr{U}$ be the set of open subsets U of $]0,1[$ such that $f(x) =f(y)$ for every connected component $]x, y[$ of U.

#### Lemma 8 {#ta-iii-s2-lem-8 .statement tag=01Y5}

The set $\mathscr{U}$, ordered by inclusion, is inductive.

Let $\mathscr{V}$ be a totally ordered subset of $\mathscr{U}$. Let us prove that the union V of the sets belonging to $\mathscr{V}$ is an element of $\mathscr{U}$, that is to say that, for every connected component $]u, v[$ of V, one has $f(u) =f(v)$.

Let $x$ be a point of $]u, v[$. Let $\mathscr{V}_x$ be the set of the $U\in \mathscr{V}$ such that $x\in U$; for such a U, denote by $]u_U, v_U[$ the connected component of $x$ in U. One has $u_{U'}\leqslant u_U< v_U\leqslant v_{U'}$ if U and $U'$ are elements of $\mathscr{V}_x$ such that $U\subset U'$. Since the union for $U\in \mathscr{U}_x$ of the $]u_U, v_U[$ is equal to $]u, v[$ according to Lemma 7 of III, p. 280, one has $u=$ lim $u_U$ and $v=$ lim $v_U$, where the limits are taken following the filtered set $\mathscr{V}_x$. Since the mapping $f$ is continuous and the topological space X is separated, the equalities $f(u_U) =f(v_U)$ for every $U\in \mathscr{V}_x$ imply that $f(u) =f(v)$, which was to be proved.

By virtue of E, III, p. 20, Th. 2, there exists an open subset U belonging to $\mathscr{U}$ which is maximal for the relation of inclusion.

Let $g:\mathbf{I}\rightarrow X$ be the mapping defined as follows. If $t\notin U$, we put $g(t) =f(t)$; otherwise, denoting by $]u, v[$ the connected component of $t$ in U, we put $g(t) =f(u) =f(v)$, so that the mapping $g|[u, v]$ is constant with image $f(u)$.

Prop. 18 follows from the following lemma.

#### Lemma 9 {#ta-iii-s2-lem-9 .statement tag=01Y6}

There exists a continuous, increasing and surjective mapping $u:\mathbf{I}\rightarrow \mathbf{I}$ and an injective path $c:\mathbf{I}\rightarrow X$ joining $a$ to $b$ such that $g=c\circ u$.

Let us first prove that the mapping $g$ is continuous. Let $t$ be a point of $\mathbf{I}$. If $t\in U,g$ is constant in a neighbourhood of $t$, hence continuous at $t$. Suppose that $t\notin U$ and let W be an open neighbourhood of $g(t)$ in X. Let V be an open interval in $\mathbf{I}$ containing $t$ such that $f(V)\subset W$; such an interval exists since $f$ is continuous at $t$. Let us prove that $g(V)\subset W$. Let $x\in V$; if $x\notin U$, we have $g(x) =f(x)$, hence $g(x)\in W$. Suppose then that $x\in U$ and let $]u, v[$ be the connected component of $x$ in U. Observe that $]u, v[$ does not contain $t$. Consequently, if $x < t$, we have $x < v\leqslant t$ whence $v\in V$ and $g(x) =g(v) =f(v)\in f(V)\subset W$. The same argument shows that $g(x)\in W$ if $x > t$. Thus, $g$ is continuous at $t$.

Let $u$ and $v$ be points of $\mathbf{I}$ such that $g(u) =g(v)$ and $u < v$. Let us prove that $]u, v[\subset U$. Put $U'= U\cup ]u, v[$; it is an open subset of $]0,1[$.

If $u$ belongs to U, let $u'$ denote the greatest lower bound in $\mathbf{I}$ of the connected component of $u$ in U; put $u'=u$ if $u$ does not belong to U. Analogously, if $v$ belongs to U, let $v'$ denote the least upper bound in $\mathbf{I}$ of the connected component of $v$ in U; put $v'=v$ if $v$ does not belong to U. Then, $]u', v'[$ is a connected component of $U'$ and one has $f(u') =g(u) =g(v) =f(v')$. Since the connected components of $U'$ distinct from $]u', v'[$ are connected components of U, the open set $U'$ is an element of $\mathscr{U}$. Since U is a maximal element of $\mathscr{U}$ for the relation of inclusion, one has $U'= U$ and $]u, v[$ is contained in U. This proves that $g$ is constant on the interval $[u, v]$. The fibres of $g$ are therefore intervals of $\mathbf{I}$, and these intervals are closed because $g$ is continuous.

Let R be the equivalence relation associated with $g$ and let $p$ be the canonical surjection of $\mathbf{I}$ onto $\mathbf{I}/R$. There exists a unique continuous mapping $g'$ of $\mathbf{I}/R$ into X such that $g=g'\circ p$; this mapping is injective. By the corollary, III, p. 276, of prop. 16, there exists a mapping $u$, increasing, continuous and surjective, such that R is the equivalence relation associated with $u$. Since the space $\mathbf{I}$ is compact and the space X is separated, the mapping $u$ is closed, hence strict (I, p. 18, example 2). It defines by passing to the quotient a homeomorphism $u'$ of $\mathbf{I}/R$ onto $\mathbf{I}$. Then, the mapping $g'\circ (u')^{-1}$ of $\mathbf{I}$ into X is an injective path of origin $a$ and of term $b$.

### 10. Lifting of paths

#### Theorem 3 {#ta-iii-s2-thm-3 .statement tag=01Y7}

Let I be an interval of $\mathbf{R}$ and let X be a nonempty and separated topological space. Let $p: X\rightarrow I$ be a continuous, open and proper mapping whose fibres are totally disconnected (TG, I, p. 83). The mapping $p$ is surjective. For every point $x$ of X, it possesses a continuous section $s$ such that $s(p(x)) =x$.

The set $p(X)$ is an open, closed (TG, I, p. 72, prop. 1), nonempty subset of I. Since I is connected, one has $p(X) = I$; the mapping $p$ is therefore surjective.

For every pair $(a, b)\in I\times I$ such that $a\leqslant b$, let $F_{a,b}$ denote the set of pairs $(y, z)\in \overset{-1}{p}(a)\times \overset{-1}{p}(b)$ such that $y$ and $z$ belong to one and the same connected component of $\overset{-1}{p}([a, b])$.

#### Lemma 10 {#ta-iii-s2-lem-10 .statement tag=01Y8}

Let $a,b$ be points of I such that $a\leqslant b$.

a) The set $F_{a,b}$ is closed in $\overset{-1}{p}(a)\times \overset{-1}{p}(b)$.

b) One has pr$_1(F_{a,b}) =\overset{-1}{p}(a)$ and pr$_2(F_{a,b}) =\overset{-1}{p}(b)$.

c) Let $c\in I$ such that $b\leqslant c$. If $(y, z)$ belongs to $F_{a,b}$ and $(z, t)$ belongs to $F_{b,c}$, then $(y, t)$ belongs to $F_{a,c}$.

The set $\overset{-1}{p}([a, b])$ is compact (TG, I, p. 77, Prop. 7). Hence, for a pair $(y, z)\in \overset{-1}{p}(a)\times \overset{-1}{p}(b)$ to belong to $F_{a,b}$, it is necessary and sufficient that every open and closed subset of $\overset{-1}{p}([a, b])$ which contains $y$ should contain $z$ (TG, II, p. 32, Prop. 6).

Put $Y =\overset{-1}{p}([a, b])$. For every open and closed subset U of Y, the set $((U\times U)\cup ((Y-U)\times (Y-U)))\cap (\overset{-1}{p}(a)\times \overset{-1}{p}(b))$ is closed in $\overset{-1}{p}(a)\times \overset{-1}{p}(b)$. The intersection of these sets is equal to $F_{a,b}$, whence a).

Let $y\in \overset{-1}{p}(a)$. Let $\mathscr{U}$ denote the set of open and closed neighbourhoods of $y$ in Y. The mapping of Y into $[a, b]$ deduced from $p$ by passing to subspaces is open and proper (I, p. 17, Prop. 8), hence also closed. It follows that, for every set U belonging to $\mathscr{U},p(U)$ is a nonempty open and closed subset of $[a, b]$; since the interval $[a, b]$ is connected, one has $p(U) = [a, b]$ and in particular $U\cap \overset{-1}{p}(b)=\not\emptyset$. Hence, $(U\cap \overset{-1}{p}(b))_{U\in\mathscr{U}}$ is a decreasing filtering family of nonempty closed subsets of the compact space $\overset{-1}{p}(b)$. The intersection of this family is not empty (TG, I, p. 59); let $z$ be one of its elements. One has $(y, z)\in F_{a,b}$. We have proved the relation pr$_1(F_{a,b}) =\overset{-1}{p}(a)$. The relation pr$_2(F_{a,b}) =\overset{-1}{p}(b)$ is deduced from it by replacing $p$, I$,a,b$ by $-p$, $-I,-b,-a$.

Under the hypotheses of c), the pair $(y, t)$ belongs to $\overset{-1}{p}(a)\times \overset{-1}{p}(c)$, the set $\{y, z\}$ is contained in a connected part C of $\overset{-1}{p}([a, b])$ and the set $\{z, t\}$ is contained in a connected part $C'$ of $\overset{-1}{p}([b, c])$. Then, $C\cup C'$ is a connected part of $\overset{-1}{p}([a, c])$ (TG, I, p. 81, prop. 2) and contains $\{y, t\}$, whence the relation $(y, t)\in F_{a,c}$.

Let us return to the proof of theorem 3. Each fibre of the mapping $p$ is compact (TG, I, p. 77, prop. 7). According to Tychonoff's theorem (TG, I, p. 63, th. 3), the product space $K =\prod_{a\in I}\overset{-1}{p}(a)$ is compact. Let $K'$ be the set of elements $(y_a)_{a\in I}$ of K such that $y_{p(x)}$ is equal to $x$ and such that one has $(y_a, y_b)\in F_{a,b}$ for every pair $(a, b)$ of elements of I such that $a < b$. Theorem 3 follows from the following lemma.

#### Lemma 11 {#ta-iii-s2-lem-11 .statement tag=01Y9}

a) The set $K'$ is not empty.

b) Let $(s_a)_{a\in I}$ be an element of $K'$. The mapping $s:a\mapsto s_a$ from I into X is a continuous section of $p$ such that $s(p(x)) =x$.

For every finite subset S of I containing the point $p(x)$, denote by $K_S$ the set of elements $(y_a)_{a\in I}$ of K satisfying the relation $y_{p(x)}=x$ and the relations $(y_a, y_b)\in F_{a,b}$ for every pair $(a, b)$ of elements of S such that $a < b$. The sets $K_S$ are closed in K (lemma 10, a)) and form a decreasing filtering family of subsets of K, whose intersection is $K'$. To prove that $K'$ is not empty, it is enough to prove that, for every finite subset S of I containing the point $p(x)$, the set $K_S$ is not empty (TG, I, p. 59).

Let S be such a subset; order its elements in a strictly increasing sequence $(a_1, . . . , a_n)$ and denote by $i$ the integer such that $p(x) =a_i$. Put $y_{a_i}=x$. Lemma 10, b), permits us to construct by induction elements $y_{a_j}\in \overset{-1}{p}(a_j)$, for $i < j\leqslant n$, and by descending induction elements $y_{a_j}\in \overset{-1}{p}(a_j)$ for $1\leqslant j < i$, in such a way that one has $(y_{a_j}, y_{a_{j+1}})\in F_{a_j,a_{j+1}}$ for every integer $j$ such that $1\leqslant j < n$. According to lemma 10, c), one has $(y_a, y_b)\in F_{a,b}$ for every pair $(a, b)$ of elements of S such that $a < b$. Since the mapping $p$ is surjective, we can choose for every $a\in I-S$ an element $y_a\in \overset{-1}{p}(a)$. The family $(y_a)_{a\in I}$ thus constructed belongs to $K_S$, hence $K_S$ is not empty.

Let us prove b). By definition of $K',s$ is a section of $p$ such that $s(p(x)) =x$. Let $a\in I$; let us prove the continuity of $s$ at the point $a$. Let U be an open neighbourhood of $s_a$ in X. Since $\overset{-1}{p}(a)$ is a compact space (TG, I, p. 77, prop. 7) and totally disconnected, $s_a$ possesses in $\overset{-1}{p}(a)$ an open and closed neighbourhood C, contained in U (TG, II, p. 32, corollary). The sets C and $\overset{-1}{p}(a)-C$ are closed in $\overset{-1}{p}(a)$, hence compact, and they are disjoint. Since X is separated, they possess in X open and disjoint neighbourhoods V and $V'$ (TG, I, p. 61, prop. 3). The set $(V\cap U)\cup V'$ is an open neighbourhood of the fibre $\overset{-1}{p}(a)$ in X; since the mapping $p$ is closed (TG, I, p. 72, prop. 1), $(V\cap U)\cup V'$ contains a set of the form $\overset{-1}{p}(J)$, where $J\subset I$ is an open interval containing $a($I, p. 75, lemma). Put $W = V\cap U\cap \overset{-1}{p}(J)$. The set W is open in $\overset{-1}{p}(J)$; it is also closed in $\overset{-1}{p}(J)$ since one has $\overset{-1}{p}(J)-W = V'\cap \overset{-1}{p}(J)$. Let $b\in J$. The closed interval of I with endpoints $a$ and $b$ is contained in J. By assumption, $(s_a, s_b)$ belongs to $F_{a,b}$ if $a\leqslant b$ and $(s_b, s_a)$ belongs to $F_{b,a}$ if $b\leqslant a$. There therefore exists a connected subset of $\overset{-1}{p}(J)$ containing $\{s_a, s_b\}$. Consequently, the point $s_b$ belongs to every open and closed subset of $\overset{-1}{p}(J)$ which contains $s_a$, hence in particular to W; fortiori, $s_b$ belongs to U. We therefore have $s(J)\subset U$, which proves the continuity of $s$ at the point $a$.

#### Corollary {#ta-iii-s2-n10-cor-1 .statement tag=01YA}

Let X and B be topological spaces and let $p: X\rightarrow B$ be a continuous, open, proper and separated mapping whose fibres are totally disconnected. Let I be an interval of $\mathbf{R}$, let $f: I\rightarrow B$ be a continuous mapping, let $a$ be a point of I and let $x$ be a point of X such that $f(a) =p(x)$. There exists a continuous mapping $g: I\rightarrow X$ such that $p\circ g=f$ and $g(a) =x$.

Posons $X'= I\times_BX$ and denote by $p': X'\rightarrow$ I and $f': X'\rightarrow$ X the canonical projections. The mapping $p'$ is continuous, open, proper and separated (I, p. 17, prop. 8 and p. 27, prop. 4). Since the space I is separated, the space $X'$ is separated (I, p. 26, remark 3). The fibres of $p'$ are totally disconnected ( I, p. 10, corollary, a)). According to Theorem 3, there exists a continuous section $s'$ of $p'$ which takes in $a$ the value $(a, x)$. The mapping $g=f'\circ s'$ of I into X is continuous, we have $p\circ g=p\circ f'\circ s'=f\circ p'\circ s'=f$ and $g(a) =x$, whence the corollary.

#### Theorem 4 {#ta-iii-s2-thm-4 .statement tag=01YB}

Let X be a topological space, let G be a discrete group operating properly in X and let $p: X\rightarrow X/G$ be the canonical mapping. Let I be an interval of $\mathbf{R}$, let $f: I\rightarrow X/G$ be a continuous mapping, let $a$ be a point of I and let $x$ be a point of X such that $f(a) =p(x)$. There exists a continuous mapping $\varphi : I\rightarrow X$ such that $p\circ \varphi =f$ and $\varphi (a) =x$.

We first treat the case where I is a closed bounded interval of $\mathbf{R}$.

According to TG, III, p. 29, prop. 3, the space X is separated.

Let $y$ be a point of $X/G$ and let $x\in X$ such that $y=p(x)$. The stabilizer $K_x$ of $x$ is a finite subgroup of G; moreover, there exist neighbourhoods $U_x$ of $x$ in X and $V_y$ of $y$ in $X/G$ such that $U_x$ is stable by $K_x,gU_x\cap U_x=\emptyset$ if $g\notin K_x$ and $p$ induces a homeomorphism of $U_x/K_x$ onto $V_y$ (TG, III, p. 32, proposition 8). Moreover, for every $g\in G,p$ induces a homeomorphism of $gU_x$ onto $V_y$. Since I is compact, there exist integers $m$ and $n$ such that $m\leqslant 0\leqslant n$ and a finite sequence $(a_i)_{m\leqslant i\leqslant n}$ of elements of I such that $a_0=a,I = [a_m, a_n]$, and such that, for every $i\in  \{m, . . . , n-1\},f([a_i, a_{i+1}])$ is contained in an open set $V_{y_i}$ of $X/G$ constructed as above.

Soit $x_0$ the unique element of $\overset{-1}{p}(y_0)$ such that $x\in U_{x_0}$. Let $q_0$ be the canonical mapping of $U_{x_0}$ onto $U_{x_0}/K_{x_0}$; by passing to the quotient, the mapping $p$ induces a homeomorphism $i_0$ of $U_{x_0}/K_{x_0}$ onto $V_{y_0}$ such that $i_0\circ q_0=p|U_{x_0}$. The mapping $q_0$ is proper (TG, III, p. 29, prop. 3), open (TG, I, p. 31, example 1) and separated, since X is separated. Its fibres are totally disconnected, since they are finite. According to the corollary, III, p. 286, there exists a continuous mapping $\varphi_0: [a_0, a_1]\rightarrow U_{x_0}$ such that $p\circ \varphi_0=f|[a_0, a_1]$.

In the same way, by induction on the integer $i\in  \{0, . . . , n-1\}$, one constructs a point $x_i\in \overset{-1}{p}(y_i)$, a continuous mapping $\varphi_i: [a_i, a_{i+1}]\rightarrow X$ whose image is contained in $U_{x_i}$ such that $p\circ \varphi_i=f|[a_i, a_{i+1}]$ and such that $\varphi_i(a_{i+1}) =\varphi_{i+1}(a_{i+1})$ if $0\leqslant i < n-1$.

Analogously, by decreasing induction on the integer $i\in  \{m, . . . ,-1\}$, one constructs a point $x_i\in \overset{-1}{p}(y_i)$, a continuous mapping $\varphi_i: [a_i, a_{i+1}]\rightarrow X$ whose image is contained in $U_{x_i}$ such that $p\circ \varphi_i=$ $f|[a_i, a_{i+1}]$ and such that $\varphi_i(a_{i+1}) =\varphi_{i+1}(a_{i+1})$ if $m\leqslant i <0$.

There exists a unique mapping $\varphi : I\rightarrow$ X which coincides with $\varphi_i$ in $[a_i, a_{i+1}]$ for $m\leqslant i < n$. It is continuous (TG, I, p. 19, prop. 4). It is a continuous lifting of $f$ to X such that $\varphi (a) =x$.

This proves the theorem when I is compact. In the general case, there exist sequences $(a_n)_{n\in\mathbf{N}}$ and $(b_n)_{n\in\mathbf{N}}$ such that $(a_n)$ is stationary with limit inf(I), $(b_n)$ is stationary with limit sup(I)$,a=a_0=b_0$, and such that $(a_n)$ (resp. $(b_n)$) is constant if I has a smallest (resp. greatest) element. From what precedes, there exists for every integer $n\in \mathbf{N}$ a continuous lifting $\varphi_n$ of $f|[a_n, a_{n+1}]$ to X, a continuous lifting $\varphi '_n$ of $f|[b_{n+1}], b_n]$ to X such that $\varphi_0(a_0) =\varphi '_0(b_0) =x$ $\varphi_{n+1}(a_{n+1}) =\varphi_n(a_{n+1}),\varphi '_{n+1}(b_{n+1}) =\varphi '_n(b_{n+1})$. There exists a unique mapping $\varphi : I\rightarrow X$ which coincides with $\varphi_n$ in $[a_n, a_{n+1}]$ and with $\varphi '_n$ in $[b_{n+1}, b_n]$, for every $n\in \mathbf{N}$. It is continuous (loc. cit.) and it is a continuous lifting of $f$ to X such that $phi(a) =x$. The theorem is thus proved.

#### Example 1 {#ta-iii-s2-n10-exa-1 .statement tag=01YC}

Let X be a separated topological space and let G be a finite group, endowed with the discrete topology, which operates continuously in X. The operation is then proper (TG, III, p. 28, prop. 2). The assertion of theorem 4 follows directly from the corollary of theorem 3.

#### Example 2 {#ta-iii-s2-n10-exa-2 .statement tag=01YD}

Soit $n$ an integer $\geqslant 0$. Let $P_n$ denote the set of monic polynomials $P\in$ $\mathbf{C}[X]$ of degree $n$, endowed with the topology for which the mapping $(c_0, . . . , c_{n-1})\mapsto X^n+c_{n-1}X^{n-1}+\cdots +c_0$ is a homeomorphism of $\mathbf{C}^n$ onto $P_n$. The mapping $p$ of $\mathbf{C}^n$ into $P_n$ defined by $p(z_1, . . . , z_n) = (X-z_1). . .(X-z_n)$ is continuous. The symmetric group $\mathfrak{S}_n$ operates on $\mathbf{C}^n$ by permutation of the factors and $p$ defines by passing to the quotient a homeomorphism of $\mathbf{C}^n/\mathfrak{S}_n$ onto $P_n$ (TG, VIII, p. 22, prop. 1, I, p. 23, cor. 1 and TG, VIII, p. 20). We therefore deduce the following statement:

Let I be an interval of $\mathbf{R}$, let $(c_0, . . . , c_{n-1})$ be a sequence of continuous mappings from I into $\mathbf{C}$, let $a$ be a point of I and let $(z_1, . . . , z_n)$ be a sequence of complex numbers such that one has $(X-z_1). . .(X-z_n) = X^n+$ $c_{n-1}(a)X^{n-1}+\cdots +c_0(a)$. There exists a sequence $(\lambda_1, . . . , \lambda_n)$ of continuous mappings from I into $\mathbf{C}$ such that one has $\lambda_i(a) =z_i$ for $1\leqslant i\leqslant n$ and $(X-\lambda_1(t)). . .(X-\lambda_n(t)) = X^n+c_{n-1}(t)X^{n-1}+\cdots +c_0(t)$ for every $t\in I$.

## EXERCISES {#ta-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
