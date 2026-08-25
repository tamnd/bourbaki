---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 2
section_title: Uniformly continuous functions
lang: en
source: top-i-iv
pdf_pages: 0180-0187, 0213-0214
extraction: ocr
subsections:
    - "no": 1
      title: UNIFORMLY CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 180
    - "no": 2
      title: COMPARISON OF UNIFORMITIES
      page: 0
      pdf_page: 181
    - "no": 3
      title: INITIAL UNIFORMITIES
      page: 0
      pdf_page: 182
    - "no": 4
      title: INVERSE IMAGE OF A UNIFORMITY; UNIFORM SUBSPACES
      page: 0
      pdf_page: 183
    - "no": 5
      title: LEAST UPPER BOUND OF A SET OF UNIFORMITIES
      page: 0
      pdf_page: 184
    - "no": 6
      title: PRODUCT OF UNIFORM SPACES
      page: 0
      pdf_page: 185
    - "no": 7
      title: INVERSE LIMITS OF UNIFORM SPACES
      page: 0
      pdf_page: 186
statements: 25
exercises: 6
content_sha256: 09273b7b580428a931bd796fe11338d641c3001505f6f56764965ea50a1ca0c1
---

## 2. UNIFORMLY CONTINUOUS FUNCTIONS

### 1. UNIFORMLY CONTINUOUS FUNCTIONS

#### Definition 1 {#top-ii-s2-def-1 .statement}

*A mapping $f$ of a uniform space $X$ into a uniform space $X'$ is said to be uniformly continuous if, for each entourage $V'$ of $X'$, there is an entourage $V$ of $X$ such that the relation $(x, y) \in V$ implies $(f(x), f(y)) \in V'$.*

In more expressive terms we may say that $f$ is uniformly continuous if $f(x)$ and $f(y)$ are as close to each other as we please whenever $x$ and $y$ are close enough.

If we put $g = f \times f$, then Definition 1 means that *whenever $V'$ is an entourage of $X'$, $\overline{g^{-1}}(V')$ is an entourage of $X$*.

#### Example 1 {#top-ii-s2-n1-exa-1 .statement}

The identity mapping of a uniform space onto itself is uniformly continuous.
2) A constant mapping of a uniform space into a uniform space is uniformly continuous.
3) Every mapping of a discrete uniform space into a uniform space is uniformly continuous.

#### Proposition 1 {#top-ii-s2-prop-1 .statement}

Every uniformly continuous mapping is continuous.

This is an immediate consequence of the definitions.

On the other hand, a continuous mapping of a uniform space X into a uniform space X' need not be uniformly continuous, \* as is shown by the example $x \to x^3$, a homeomorphism of $\mathbf{R}$ onto itself, which is not uniformly continuous with respect to the additive uniformity. \* (See § 4, no. 1, Theorem 2.)

#### Proposition 2 {#top-ii-s2-prop-2 .statement}

(a) If $f : X \to X'$ and $g : X' \to X''$ are two uniformly continuous mappings, then $g \circ f : X \to X''$ is uniformly continuous.

(b) A bijection $f$ of a uniform space X onto a uniform space X' is an isomorphism if and only if $f$ and the inverse of $f$ are uniformly continuous.

This follows immediately from the interpretation of Definition 1 in terms of the product mapping $f \times f$.

### 2. COMPARISON OF UNIFORMITIES

Proposition 2 of no. 1 shows that we can take as morphisms of uniform structures the uniformly continuous mappings (Set Theory, Chapter IV, § 2, no. 1); we shall always assume in the future that the morphisms have been so chosen. In accordance with the general definitions (Set Theory, Chapter IV, § 2, no. 2), this allows us to define an order relation on the set of uniformities on a given set X:

#### Definition 2 {#top-ii-s2-def-2 .statement}

If $\mathcal{U}_1$ and $\mathcal{U}_2$ are two uniform structures on the same set X, $\mathcal{U}_1$ is said to be finer than $\mathcal{U}_2$ (and $\mathcal{U}_2$ coarser than $\mathcal{U}_1$) if, denoting by $X_i$ the set X with the uniform structure $\mathcal{U}_i$ ($i = 1,2$), the identity mapping $X_1 \to X_2$ is uniformly continuous.

If $\mathcal{U}_1$ is finer than $\mathcal{U}_2$ and distinct from $\mathcal{U}_2$, we say that $\mathcal{U}_1$ is strictly finer than $\mathcal{U}_2$ (and that $\mathcal{U}_2$ is strictly coarser than $\mathcal{U}_1$).

Two uniformities are said to be comparable if one is finer than the other.

#### Example {#top-ii-s2-n2-exa-1 .statement}

In the ordered set of uniformities on a set X, the discrete uniformity is the finest, and the coarsest uniformity is that in which the set of entourages consists of the single element $X \times X$.

The following proposition is an immediate consequence of Definition 1 of no. 1:

#### Proposition 3 {#top-ii-s2-prop-3 .statement}

If $\mathcal{U}_1$ and $\mathcal{U}_2$ are two uniformities on a set X, then $\mathcal{U}_1$ is finer than $\mathcal{U}_2$ if and only if every entourage of $\mathcal{U}_2$ is an entourage of $\mathcal{U}_1$.

#### Corollary {#top-ii-s2-n2-cor-1 .statement}

Let $\mathcal{U}_1$ and $\mathcal{U}_2$ be two uniformities on a set X, and suppose that $\mathcal{U}_1$ is finer than $\mathcal{U}_2$; then the topology induced by $\mathcal{U}_1$ is finer than the topology induced by $\mathcal{U}_2$.

#### Remark 1 {#top-ii-s2-n2-rem-1 .statement}

It can happen that a uniformity $\mathcal{U}_1$ is strictly finer than a uniformity $\mathcal{U}_2$ but that the two induced topologies are identical. The following example shows this:

Let $X$ be a non-empty set. For each finite partition $\varpi = (A_i)_{1 \leq i \leq n}$ of $X$, let $V_{\overline{\varpi}}$ denote
$$
\bigcup_i A_i \times A_i.
$$
The sets $V_{\overline{\varpi}}$ then form a fundamental system of entourages of a uniformity $\mathcal{U}$ on $X$. For if $\varpi$ is any finite partition of $X$ we have $\Delta \subset V_{\overline{\varpi}}$ and $V_{\overline{\varpi}} \circ V_{\overline{\varpi}} = \overline{V_{\overline{\varpi}}} = V_{\overline{\varpi}}$ (\S 1, no. 1, Example 2); and if $\varpi' = (B_j)$ and $\varpi'' = (C_k)$ are two finite partitions of $X$, then those of the sets $B_j \cap C_k$ which are not empty form a finite partition $\varpi$ of $X$, and we have $V_{\overline{\varpi}} \subset V_{\overline{\varpi'}} \cap V_{\overline{\varpi''}}$. $\mathcal{U}$ is called the uniformity of finite partitions on $X$. The topology induced by $\mathcal{U}$ is the discrete topology, since for each $x \in X$ the sets $\{x\}$ and $C\{x\}$ form a finite partition of $X$. Nevertheless, if $X$ is infinite, it is clear that $\mathcal{U}$ is strictly coarser than the discrete uniformity.

#### Remark 2 {#top-ii-s2-n2-rem-2 .statement}

If $f : X \to X'$ is a uniformly continuous mapping, then $f$ remains uniformly continuous if we replace the uniformity of $X$ by a finer uniformity and that of $X'$ by a coarser uniformity (no. 1, Proposition 2). In other words, the finer the uniformity of $X$ and the coarser the uniformity of $X'$, the more uniformly continuous mappings there are of $X$ into $X'$.

### 3. INITIAL UNIFORMITIES

#### Proposition 4 {#top-ii-s2-prop-4 .statement}

Let $X$ be a set, let $(Y_i)_{i \in I}$ be a family of uniform spaces, and for each $i \in I$ let $f_i$ be a mapping of $X$ into $Y_i$. For each $i \in I$ let $g_i$ denote $f_i \times f_i$. Let $\mathfrak{S}$ be the set of subsets of $X \times X$ of the form $\overline{g_i}(V_i)$, where $i \in I$ and $V_i$ is an entourage of $Y_i$, and let $\mathcal{B}$ be the set of all finite intersections

$$
\text{(1)} \quad U(V_{i_1}, \ldots, V_{i_n}) = \overline{g_{i_1}}(V_{i_1}) \cap \cdots \cap \overline{g_{i_n}}(V_{i_n})
$$

of sets of $\mathfrak{S}$. Then $\mathcal{B}$ is a fundamental system of entourages of a uniformity $\mathcal{U}$ on $X$ which is the initial uniform structure on $X$ with respect to the family $(f_i)$ (Set Theory, Chapter IV, § 2, no. 3), and in particular $\mathcal{U}$ is the coarsest uniformity on $X$ for which all the mappings $f_i$ are uniformly continuous. But otherwise, let $h$ be a mapping of a uniform space $Z$ into $X$; then $h$ is uniformly continuous (when $X$ is endowed with the uniformity $\mathcal{U}$) if and only if each of the mappings $f_i \circ h$ is uniformly continuous.

It is immediately seen that $\mathcal{B}$ satisfies axioms $(B_1)$ and $(U'_1)$. If $W_i = \overline{g}_i^{-1}(V_i)$, then $\overline{W}_i = \overline{g}_i^{-1}(\overline{V}_i)$ and $\dot{W}_i = \dot{g}_i^{-1}(\dot{V}_i)$; hence $\mathcal{B}$ also satisfies axioms $(U'_{II})$ and $(U'_{III})$ and is therefore a fundamental system of entourages of a uniformity $\mathcal{U}$ on $X$. Furthermore, it follows immediately from the definition of $\mathcal{U}$ and Definition 1 and no. 1 that $f_i$ is uniformly continuous for each index $i \in I$; hence (no. 1, Proposition 2) $f_i \circ h$ is uniformly continuous for each $i \in I$ if $h$ is. Conversely, suppose that $f_i \circ h$ is uniformly continuous for each $i \in I$, and consider a set $U(V_{i_1}, \ldots, V_{i_n})$; by hypothesis, for each $k$ such that $1 \leq k \leq n$, there is an entourage $W_k$ of $Z$ such that the relation $(z, z') \in W_k$ implies $[f_{i_k}(h(z)), f_{i_k}(h(z'))] \in V_k$; if
$$
W = \bigcap_k W_k,
$$
these $n$ relations are simultaneously satisfied whenever $z$ and $z'$ are $W$-close, so that we have then $(h(z), h(z')) \in U(V_{i_1}, \ldots, V_{i_n})$, and the proof is complete.

#### Corollary {#top-ii-s2-n3-cor-1 .statement}

*The topology on $X$ induced by the coarsest uniformity $\mathcal{U}$ for which the $f_i$ are uniformly continuous is also the coarsest topology for which the $f_i$ are continuous.*

This is an immediate consequence of the definition of the neighbourhoods of a point in this latter topology (Chapter I, § 2, no. 3, Proposition 4).

The general properties of initial structures (*Set Theory*, Chapter IV, § 2, no. 3, criterion CST 10) imply in particular the following *transitivity* property:

#### Proposition 5 {#top-ii-s2-prop-5 .statement}

*Let $X$ be a set, let $(Z_i)_{i \in I}$ be a family of uniform spaces, let $(J_\lambda)_{\lambda \in L}$ be a partition of $I$ and let $(Y_\lambda)_{\lambda \in L}$ be a family of sets indexed by $L$. For each $\lambda \in L$, let $h_\lambda$ be a mapping of $X$ into $Y_\lambda$; for each $\lambda \in L$ and each $i \in J_\lambda$, let $g_{i\lambda}$ be a mapping of $Y_\lambda$ into $Z_i$; and let $f_i = g_{i\lambda} \circ h_\lambda$. Let each $Y_\lambda$ carry the coarsest uniform structure for which the mappings $g_{i\lambda}$ ($i \in J_\lambda$) are uniformly continuous. Then the coarsest uniform structure on $X$ for which the $f_i$ are uniformly continuous is the same as the coarsest uniform structure on $X$ for which the $h_\lambda$ are uniformly continuous.*

### 4. INVERSE IMAGE OF A UNIFORMITY; UNIFORM SUBSPACES

Let $X$ be a set, $Y$ a uniform space, $f$ a mapping of $X$ into $Y$. The coarsest uniformity $\mathcal{U}$ on $X$ for which $f$ is uniformly continuous is called the *inverse image* under $f$ of the uniform structure of $Y$. It follows from Proposition 4 of no. 3, and from the formulae which give the inverse image of an intersection, that the inverse images under $g = f \times f$ of the entourages of $Y$ form a fundamental system of entourages for $\mathcal{U}$. The topology induced by $\mathcal{U}$ is the *inverse image* under $f$ of the topology of $Y$ (no. 3, Corollary to Proposition 4).

#### Remark {#top-ii-s2-n4-rem-1 .statement}

If $f : X \to Y$ is surjective, then the entourages of $Y$ are the direct images under $g$ of the entourages of $X$.

A mapping $f$ of a uniform space $X$ into a uniform space $X'$ is uniformly continuous if and only if the inverse image under $f$ of the uniformity of $X'$ is coarser than the uniformity of $X$.

Let $A$ be a subset of a uniform space $X$. The uniformity induced on $A$ by the uniformity of $X$ is the inverse image of the latter under the canonical injection $A \to X$. By Proposition 4 of no. 3, this is equivalent to the following definition:

#### Definition 3 {#top-ii-s2-def-3 .statement}

Let $A$ be a subset of a uniform space $X$. The uniformity on $A$ whose set of entourages is the trace on $A \times A$ of the set of entourages of $X$ is called the uniformity induced on $A$ by the uniformity of $X$.

The topology induced by the uniformity induced on $A$ is the same as the topology induced on $A$ by the topology of $X$; the set $A$, together with the uniformity and the topology induced by those of $X$, is called a uniform subspace of $X$.

If $A$ is a subset of a uniform space $X$ and if $f : X \to X'$ is a uniformly continuous mapping, then the restriction $f|A$ is a uniformly continuous mapping of $A$ into $X'$. If $A' \subset X'$ is such that $f(X) \subset A'$, then the mapping of $X$ into the uniform subspace $A'$ of $X'$, having the same graph as $f$, is again uniformly continuous (no. 3, Proposition 4).

If $B \subset A \subset X$, then the uniform subspace $B$ of $X$ is identical with the uniform subspace $B$ of the uniform subspace $A$ of $X$ (transitivity of induced uniform structures; no. 3, Proposition 5).

#### Proposition 6 {#top-ii-s2-prop-6 .statement}

Let $A$ be a dense subset of a uniform space $X$. Then the closures, in $X \times X$, of the entourages of the uniform subspace $A$ form a fundamental system of entourages of $X$.

$A \times A$ is dense in $X \times X$ (Chapter I, § 4, no. 3, Proposition 7). Let $V$ be an open entourage of $A$; it is the intersection of $A \times A$ with an open entourage $U$ of $X$. We have $U \subset \overline{V}$ (Chapter I, § 1, no. 6, Proposition 5), and this relation together with $\overline{V} \subset \overline{U}$ establishes the proposition, in view of § 1, no. 2, Corollary 2 of Proposition 2.

### 5. LEAST UPPER BOUND OF A SET OF UNIFORMITIES

Every family $(\mathcal{U}_i)_{i \in I}$ of uniformities on a set $X$ has a least upper bound $\mathcal{U}$ in the ordered set of all uniformities on $X$; we have only to apply Proposition 4 of no. 3, taking $Y_i$ to be the set $X$ with the uniformity $\mathcal{U}_i$, and $f_i$ to be the identity mapping $X \to Y_i$. The topology induced by $\mathcal{U}$ is just the least upper bound of the topologies induced by the $\mathcal{U}_i$.

It follows also from Proposition 4 of no. 3 that if $X$ is not empty and if $\mathcal{U}_i$ is the filter of entourages of $\mathcal{U}_i$, then the filter of entourages of $\mathcal{U}$ is the least upper bound of the filters $\mathcal{U}_i$ (Chapter I, § 6, no. 2).

#### Example {#top-ii-s2-n5-exa-1 .statement}

If $\varpi$ is any finite partition $(A_i)_{1 \leq i \leq n}$ of a non-empty set $X$, the set $V_\varpi = \bigcup_i (A_i \times A_i)$ by itself constitutes a fundamental system of entourages of a uniformity $\mathcal{U}_\varpi$ on $X$ (\S 1, no. 1, Example 2); the uniformity of finite partitions on $X$ (no. 2, Remark 1) is then the least upper bound of the uniformities $\mathcal{U}_\varpi$.

#### Remark {#top-ii-s2-n5-rem-1 .statement}

A family $(\mathcal{U}_i)$ of uniformities on $X$ also has a greatest lower bound in the ordered set of all uniformities on $X$, namely the least upper bound of the set of all uniformities on $X$ which are coarser than each of the $\mathcal{U}_i$ (such uniformities exist, since the set of all uniformities on $X$ has a least element). But (supposing $X$ not empty) the filter of entourages of this uniformity is not necessarily the intersection of the filters of entourages of the $\mathcal{U}_i$, because this latter filter need not satisfy axiom $(U_{III})$ (Exercise 4).

### 6. PRODUCT OF UNIFORM SPACES

#### Definition 4 {#top-ii-s2-def-4 .statement}

*If* $(X_i)_{i \in I}$ *is a family of uniform spaces, the product uniform space of this family is the product set*
$$
X = \prod_{i \in I} X_i
$$
*endowed with the coarsest uniformity for which the projections* $pr_i : X \to X_i$
*are uniformly continuous. This uniformity is called the product of the uniformities of the* $X_i$, *and the uniform spaces* $X_i$ *are called the factors of* $X$.

The topology induced by the product uniformity on $X$ is same as the product of the topologies of the $X_i$ (no. 3, Corollary to Proposition 4).

#### Proposition 7 {#top-ii-s2-prop-7 .statement}

*Let* $f = (f_i)$ *be a mapping of a uniform space* $Y$ *into a product uniform space* $X = \prod_{i \in I} X_i$. *Then* $f$ *is uniformly continuous if and only if each* $f_i$ *is uniformly continuous*.

Since $f_i = pr_i \circ f$, this is a particular case of Proposition 4 of no. 3.

#### Corollary {#top-ii-s2-n6-cor-1 .statement}

*Let* $(X_i)_{i \in I}, (Y_i)_{i \in I}$ *be two families of uniform spaces indexed by the same set* $I$. *For each* $i \in I$, *let* $f_i$ *be a mapping of* $X_i$ *into* $Y_i$. *If each of the* $f_i$ *is uniformly continuous, then so is the product mapping*
$$
f : (x_i) \to (f_i(x_i)).
$$
*Conversely, if the* $X_i$ *are non-empty and* $f$ *is uniformly continuous, then each* $f_i$ *is uniformly continuous.*

The general criterion of transitivity of initial uniformities (no. 3, Proposition 5) shows that, as for the product of topological spaces (Chapter I, § 4, no. 1), the product of uniform spaces is associative and that the following is true:

#### Proposition 8 {#top-ii-s2-prop-8 .statement}

*Let $X$ be a set, let $(Y_i)_{i \in I}$ be a family of uniform spaces, and for each $i \in I$ let $f_i$ be a mapping of $X$ into $Y_i$. Let $f$ be the mapping $x \to (f_i(x))$ of $X$ into $Y = \prod_{i \in I} Y_i$, and let $U$ be the coarsest uniformity on $X$ for which the $f_i$ are uniformly continuous. Then $U$ is the inverse image under $f$ of the uniformity induced on $f(X)$ by the product uniformity on $Y$.*

#### Corollary {#top-ii-s2-n6-cor-2 .statement}

*For each $i \in I$, let $A_i$ be a subspace of $Y_i$. Then the uniformity induced on $A = \prod_{i \in I} A_i$ by the product uniformity on $\prod_{i \in I} Y_i$ is the same as the product of the uniformities of the subspaces $A_i$.*

In addition, we see immediately that if $X_1, X_2$ are two uniform spaces and $a_1$ is any point of $X_1$, the mapping $x_2 \to (a_1, x_2)$ is an isomorphism of $X_2$ onto the subspace $\{a_1\} \times X_2$ of $X_1 \times X_2$; hence:

#### Proposition 9 {#top-ii-s2-prop-9 .statement}

*Let $f$ be a uniformly continuous mapping of a product uniform space $X_1 \times X_2$ into a uniform space $Y$; then every partial mapping*

$$
x_2 \to f(x_1, x_2)
$$

*of $X_2$ into $Y$ is uniformly continuous.*

In other words, a uniformly continuous function of two arguments is uniformly continuous with respect to each of them separately.

\* The example given in Chapter I, § 4, no. 2, Remark 2, shows that the converse of this proposition is false. \*

### 7. INVERSE LIMITS OF UNIFORM SPACES

Let $I$ be a partially ordered set in which the partial ordering is written $\alpha \leq \beta$. For each $\alpha \in I$ let $X_\alpha$ be a uniform space, and for each pair of indices $\alpha, \beta$ such that $\alpha \leq \beta$ let $f_{\alpha \beta}$ be a mapping of $X_\beta$ into $X_\alpha$.

#### Proposition 10 {#top-ii-s2-prop-10 .statement}

Let $I$ be a directed set, let $(X_\alpha, f_{\alpha\beta})$ be an inverse system of uniform spaces indexed by $I$, and let $J$ be a cofinal subset of $I$. For each $\alpha \in I$ let $f_\alpha$ be the canonical mapping of $X = \varprojlim X_\alpha$ into $X_\alpha$, and let $g_\alpha$ denote $f_\alpha \times f_\alpha$. Then the family of sets $\overline{g}_\alpha^{-1}(V_\alpha)$, where $\alpha$ runs through $J$ and where, for each $\alpha \in J$, $V_\alpha$ runs through a fundamental system of entourages of $X_\alpha$, is a fundamental system of entourages of $X$.

We leave the proof to the reader; it is a straightforward adaptation of the proof of Proposition 9 of Chapter I, § 4, no. 4.

Finally, the topology on $X = \varprojlim X_\alpha$ induced by the inverse limit of the uniformities of the $X_\alpha$ is the inverse limit of the topologies of the $X_\alpha$.

### Exercises {#top-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
