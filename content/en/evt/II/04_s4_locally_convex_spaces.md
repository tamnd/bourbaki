---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 4
section_title: Locally convex spaces
lang: en
source: evt-i-v
book_pages: TVS II.23-TVS II.36, TVS II.74-TVS II.76
pdf_pages: 0060-0073, 0111-0113
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a locally convex space
      page: 23
      pdf_page: 60
    - "no": 2
      title: Examples of locally convex spaces
      page: 25
      pdf_page: 62
    - "no": 3
      title: Locally convex initial topologies
      page: 26
      pdf_page: 63
    - "no": 4
      title: Locally convex final topologies
      page: 27
      pdf_page: 64
    - "no": 5
      title: The direct topological sum of a family of locally convex spaces
      page: 29
      pdf_page: 66
    - "no": 6
      title: Inductive limits of sequences of locally convex spaces
      page: 31
      pdf_page: 68
    - "no": 7
      title: Remarks on Fréchet spaces
      page: 34
      pdf_page: 71
statements: 33
exercises: 17
content_sha256: 183fe64a493ca845f33b9a913efb97564a15e0840da57b85c2de74908bd6e51d
---

## § 4. LOCALLY CONVEX SPACES

### 1. Definition of a locally convex space

#### Definition 1 {#evt-ii-s4-def-1 .statement}

— *A topological vector space is locally convex (real) if there exists a fundamental system of neighbourhoods of 0 that are convex sets.*

Such a space is called a *locally convex space*. Its topology is called a *locally convex topology*.

The topological vector spaces over $\mathbf{R}$ which we study in the rest of this book are nearly all locally convex.

If $V$ is a convex neighbourhood of 0 in the locally convex space $E$, then $V \cap (-V)$ is a symmetric convex neighbourhood of 0. As the closure of a convex set is convex (II, p. 13, prop. 14) it follows from I, p. 7, prop. 4 that the neighbourhoods of 0 in $E$ which are *closed, symmetric and convex*, form a fundamental system of neighbourhoods invariant under homotheties of centre 0 and ratio $\neq 0$.

#### Proposition 1 {#evt-ii-s4-prop-1 .statement}

— *Let $\mathfrak{S}$ be a filter base on a vector space $E$ formed from sets that are absorbent, symmetric and convex. Then the set $\mathfrak{B}$ of transforms of the sets of $\mathfrak{S}$ by homotheties of ratio $> 0$ is a fundamental system of neighbourhoods of 0 for a locally convex topology on $E$.*

Clearly $\mathfrak{B}$ is a filter base satisfying (EV_I) and (EV_{II}) of I, p. 7, prop. 4; it also satisfies (EV_{III}) since if $V \in \mathfrak{S}$ then $\frac{1}{2}V + \frac{1}{2}V = V$.

Note that if $\mathcal{T}$ is the locally convex topology on E having $\mathfrak{B}$ for a fundamental system of neighbourhoods of 0, then the sets $(1/n) \ V$, where $n$ varies in the integers $> 0$ and V varies in $\mathfrak{S}$, form a fundamental system of neighbourhoods of 0 for the topology $\mathcal{T}$. Then $\mathcal{T}$ is Hausdorff, if and only if, for every $x \neq 0$ in E there exists an integer $n$ and a set $V \in \mathfrak{S}$, such that $nx \notin V$; if, further, $\mathfrak{S}$ is enumerable, then the topology $\mathcal{T}$ is a metrisable locally convex topology. Conversely, it is clear that if $\mathcal{T}$ is a metrisable locally convex topology, then there exists an enumerable fundamental system of closed symmetric convex neighbourhoods of 0 for $\mathcal{T}$.

#### Corollary {#evt-ii-s4-n1-cor-1 .statement}

— *The topology $\mathcal{T}$ of a topological vector space E, is defined by a set of semi-norms* (II, p. 3) *if, and only if, $\mathcal{T}$ is locally convex*.

The condition is necessary since every semi-norm on E is a convex function, and so, for $\alpha > 0$, the set of $x \in E$ for which $p(x) \leq \alpha$, is convex (II, p. 17, corollary). Conversely if V is a symmetric, closed, convex neighbourhood of 0 in E, the *gauge* $p$ of V is a semi-norm on E such that V is the set of points $x$ of E satisfying $p(x) \leq 1$ (II, p. 20, prop. 23).

This shows further that a locally convex topology $\mathcal{T}$ is defined by the set of *all semi-norms that are continuous for $\mathcal{T}$*. Further, if $\mathcal{T}$ is metrisable, then it is defined by an *enumerable* set of semi-norms.

From the corollary to prop. 1, all the results of § 1 on topologies defined by sets of semi-norms apply in particular to locally convex topologies over real vector spaces. A locally convex Hausdorff space E has a completion $\hat{E}$ that is locally convex. A complete, metrisable locally convex space is called a *Fréchet space*; every Banach space is a Fréchet space.

#### Proposition 2 {#evt-ii-s4-prop-2 .statement}

— *Let f be a continuous linear form defined over a vector subspace M, of a locally convex space E; then there exists a continuous linear form h that is defined over E and is an extension of f*.

From the corollary above and II, p. 7, cor. 2, there exists a continuous semi-norm $p$ on E, such that $|f(y)| \leq p(y)$ for all $y \in M$. By the Hahn-Banach th. (II, p. 23, cor. 1) there exists a linear form $h$ on E that extends $f$ and is such that $|h(x)| \leq p(x)$ for all $x \in E$, and this implies that $h$ is continuous (II, p. 6, prop. 5).

#### Remark {#evt-ii-s4-n1-rem-1 .statement}

— If $g$ is a continuous linear mapping of M in the product space $\mathbf{R}^I$, then there exists a continuous linear mapping $h$ of E in $\mathbf{R}^I$ that is an extension of $g$; for writing $g = (g_i)$, where the $g_i$ are continuous linear forms defined over M, there is an extension $h_i$ of $g_i$ for each $i \in I$, such that $h_i$ is a continuous linear form over E. The continuous linear mapping $h = (h_i)$ has the required properties.

Note that if F is a locally convex Hausdorff space and $g$ a continuous linear mapping of M in F, then there does not necessarily exist a continuous linear mapping of E in F which is an extension of $g$ (IV, p. 55, exerc. 16, c)). However there does exist such an extension when M is finite dimensional (*cf.* cor. 2, below).

#### Corollary 1 {#evt-ii-s4-prop-2-cor-1 .statement}

— *Let E be a locally convex space. If $x_0 \in E$ is not in the closure of $\{0\}$, then there exists a continuous linear form f defined over E with $f(x_0) \neq 0$*.

Apply prop. 2 to the one dimensional vector space M generated by $x_0$ and to the linear form $\xi x_0 \mapsto \xi$ defined over M, which, by I, p. 12, prop. 2, is continuous.

#### Corollary 2 {#evt-ii-s4-prop-2-cor-2 .statement}

— Let M be a finite dimensional vector subspace of E, a locally convex Hausdorff space. Then there exists a closed vector subspace N of E, which is the topological complement of M in E.

There exists a topological complement to M in E if, and only if, the identity mapping of M on itself can be extended to a continuous linear mapping of E on M, which mapping is then necessarily a continuous projector (GT, III, § 6.2, corollary). Now, this follows from the remark above since M is isomorphic to a space $\mathbf{R}^n$ (I, p. 13, th. 2).

#### Proposition 3 {#evt-ii-s4-prop-3 .statement}

— In a locally convex space E, the balanced convex envelope of a precompact set is itself a precompact set.

Let A be a precompact set in E. Given V, a balanced convex neighbourhood of 0 in E, there exist finitely many points $a_i \in A$ ($1 \leq i \leq n$) such that A is contained in S, the union of the neighbourhoods $a_i + V$ ($1 \leq i \leq n$). Thus C, the balanced convex envelope of A, is contained in T the balanced convex envelope of S; but T is contained in B + V, where B denotes the convex envelope of the finite set of points $a_i, -a_i$ ($1 \leq i \leq n$). Now B is precompact (II, p. 14, cor. 2); hence there exist finitely many points $b_k \in B$ ($1 \leq k \leq m$) such that $B_k$ is contained in the union of the neighbourhoods $b_k + V$. Then C is contained in the union of the neighbourhoods $b_k + 2V$, and the proposition is proved.

Note that, in an infinite dimensional locally convex Hausdorff space, the convex envelope of a compact set is not necessarily closed (II, p. 74, exerc. 3).

#### Corollary {#evt-ii-s4-n1-cor-2 .statement}

— If, in a locally convex Hausdorff space E, a compact set X is contained in a complete convex set (complete in the uniform structure induced by that of E) then the convex closed envelope of X is compact.

For this envelope is a closed subset of a complete space, therefore it is complete, but it is also precompact and Hausdorff.

However in a non complete locally convex Hausdorff space, the convex closed envelope of a compact set need not be compact (II, p. 87, exerc. 2).

### 2. Examples of locally convex spaces

1) The space $\mathbf{R}^n$ is locally convex since the open cubes with centre 0 are convex (II, p. 9, prop. 6). This is, therefore, also true for all real topological vector spaces of finite dimension; in fact it follows from the above and I, § 2.3, th. 2 provided that E is Hausdorff; if not, the Hausdorff space F associated with E is of finite dimension, therefore locally convex, and the inverse images of convex neighbourhoods of 0 in F under the canonical mapping $E \to F$ are convex and form a fundamental system of neighbourhoods of 0 in E.

2) Let E be a vector space in $\mathbf{R}$, and $\mathfrak{B}$ be the family of all subsets of E that are absorbent, symmetric and convex. By prop. 1 of II, p. 23 we see that $\mathfrak{B}$ is a fundamental system of neighbourhoods of 0 for a locally convex topology $\mathcal{T}_\omega$ on E that is the finest of all locally convex topologies on E. This topology is Hausdorff; for let $x \neq 0$ be any point of E; there exists a basis $(i_i)_{i \in I}$ of E with an $\alpha \in I$ such that $e_\alpha = x$; the set of points $y = \sum_i y_i e_i$ such that $|y_\alpha| < 1$ is absorbent, symmetric and convex. It does not contain $x$. From II, p. 24, corollary, it follows that $\mathcal{T}_\omega$ is also the topology defined by the set of *all* semi-norms on E, thus every semi-norm is continuous in $\mathcal{T}_\omega$.

In particular, if $u$ is a linear mapping of E in any locally convex space F, the inverse image, under $u$, of every convex neighbourhood of 0 in F is an *absorbent* convex set in E; therefore it is a neighbourhood of 0 for $\mathcal{T}_\omega$ and thus $u$ is *continuous* for $\mathcal{T}_\omega$.

Given a convex set C in E, we say that a point $a \in C$ is an *internal point* of C if, for every line D containing $a$, the intersection $D \cap C$ contains an open segment which contains $a$; in other words — $a + C$ is *absorbent*. The point $a$ of the set A in E is *interior to A for* $\mathcal{T}_\omega$ if, and only if, there exists a convex set C with $a \in C \subset A$, and such that $a$ is an internal point of C.

More generally, let V be an affine linear variety in E, and C be a convex set contained in V; a point $a \in C$ is an *internal point of C relative to* V if, in the vector subspace $V_0 = -a + V$, the point 0 is an internal point of the set $C_0 = -a + C$.

When E is of finite dimension, the topology $\mathcal{T}_\omega$ is just the canonical topology on E (I, p. 13, th. 2); which shows that every internal point of a convex set C in E, is interior to C for the canonical topology (*cf.* II, p. 74, exerc. 5).

3) Let A be a symmetric convex set in the vector space E over $\mathbf{R}$. The vector subspace F *generated* by A is also the convex cone generated by A, since $-A = A$; this set is the set of $\lambda x$ where $x \in A$ and $\lambda \in \mathbf{R}$; the set A is *absorbent in* F and the sets $\lambda A$ where $\lambda > 0$, form a fundamental system of neighbourhoods of 0 for a locally convex topology *on* F (said to be *defined* by A), which is defined by the semi-norm $p_A$, the *gauge* of A (II, p. 20, prop. 22); we write $E_A$ for the locally convex space obtained by giving F this semi-norm. The space $E_A$ is *Hausdorff* if, and only if, $p_A$ is a *norm* or alternatively A does not contain *any line*. If B is a second symmetric convex set in E and if $A \subset B$, then clearly $E_A \subset E_B$, and the canonical injection of $E_A$ in $E_B$ is *continuous* for the topologies defined respectively by A and by B. Further, if $f$ is a linear mapping of E in a real vector space $E'$, then $f(A)$ is convex and symmetric in $E'$ and $f$ is a *continuous* linear mapping of $E_A$ *on* $E'_{f(A)}$.

Finally, note that if E carries a topology $\mathcal{T}$ compatible with its vector space structure, and if V is a symmetric *convex* neighbourhood of 0 for $\mathcal{T}$, then the vector space generated by V is identical with E, since V is absorbent, and the identity mapping of E in $E_V$ is *continuous*.

### 3. Locally convex initial topologies

#### Proposition 4 {#evt-ii-s4-prop-4 .statement}

*Let E be a vector space and let $(E_i)_{i \in I}$ be a family of locally convex spaces. For each $i \in I$, let $f_i$ be a linear mapping of E in $E_i$; then the topology* $\mathcal{T}$ on E, which is the coarsest making each mapping $f_i$ continuous, is a locally convex topology.

Using II, p. 24, corollary, this is a particular case of the corresponding property for topologies defined by semi-norms (II, p. 5).

In particular, every vector subspace of a locally convex space, and every product space of locally convex spaces, is locally convex. Every projective limit of locally convex spaces is locally convex.

Every *enumerable product* of Fréchet spaces (and in particular every enumerable product of Banach spaces) is a Fréchet space.

Every locally convex Hausdorff space E is isomorphic to a subspace of a product of Banach spaces and this subspace is closed if E is complete (II, p. 5, prop. 3). Every Fréchet space is isomorphic to a closed subspace of an enumerable product of Banach spaces (*loc. cit.*).

### 4. Locally convex final topologies

#### Proposition 5 {#evt-ii-s4-prop-5 .statement}

*Let E be a vector space, and $(F_\alpha)_{\alpha \in A}$ be a family of topological vector spaces and for each $\alpha \in A$, let $g_\alpha$ be a linear mapping of $F_\alpha$ in E.*

(i) *Denote by $\mathfrak{B}$ the family of absorbent, symmetric convex subsets V of E such that $g_\alpha^{-1}(V)$ is a neighbourhood of 0 in $F_\alpha$ for every $\alpha$; the family $\mathfrak{B}$ is a fundamental system of neighbourhoods of 0 in E for a topology $\mathcal{T}$ that is compatible with the vector space structure.*

(ii) *A linear mapping f of E in a locally convex space G (resp. a semi-norm p on E) is continuous for $\mathcal{T}$ if and only if, for every index $\alpha$, $f \circ g_\alpha$ (resp. $p \circ g_\alpha$) is continuous in $F_\alpha$.*

(iii) *The topology $\mathcal{T}$ is the finest of the locally convex topologies on E for which the $g_\alpha$ are continuous.*

*Further, the topology $\mathcal{T}$ is the only locally convex topology on E that satisfies condition (ii) for linear mappings (resp. for the semi-norms).*

As $\mathfrak{B}$ is a filter base invariant under homotheties of ratio > 0, the assertion (i) follows immediately from II, p. 23, prop. 1. By the definition of $\mathfrak{B}$, the topology $\mathcal{T}$ is the finest of locally convex topologies on E making the $g_\alpha$ continuous; whence (iii). Finally, it is clear that if $f$ is continuous, so is $f \circ g_\alpha$; conversely if the $f \circ g_\alpha$ are continuous for every $\alpha$, then for each symmetric convex neighbourhood W of 0 in G, the set $g_\alpha^{-1}(f^{-1}(W))$ is a neighbourhood of 0 in $F_\alpha$ for each $\alpha$. Now $f^{-1}(W)$ is absorbent, symmetric and convex thus $f^{-1}(W)$ is a neighbourhood of 0 in $\mathcal{T}$, and $f$ is continuous. Similarly if $p$ is a semi-norm on E such that $p \circ g_\alpha$ is continuous for every $\alpha$, and if U is the set of points $x \in E$ such that $p(x) < 1$, then, for every $\alpha$, the set $g_\alpha^{-1}(U)$ is a convex neighbourhood of 0 in $E_\alpha$ that is symmetric and absorbent; thus U is a neighbourhood of 0 in E and $p$ is continuous (II, p. 2, prop. 1).

The last statement follows from S, IV, § 2.5, criterion CST 18.

We say that $\mathcal{T}$ is the *locally convex final topology* of the family of topologies $\mathcal{T}_\alpha$ of the $F_\alpha$, for the family of linear mappings $g_\alpha$.

It may happen that $\mathcal{T}$ is not the finest of the topologies on E compatible with its vector space structure and making the $f_\alpha$ continuous (II, p. 75, exerc. 15; see also II, p. 75, exerc. 14).

In the most important case $E = \sum_{\alpha \in A} g_\alpha(F_\alpha)$, we get a fundamental system of neighbourhoods of 0 for $\mathcal{T}$ as follows; for each $\alpha \in A$, let $V_\alpha$ be a symmetric neighbourhood of 0 for $\mathcal{T}_\alpha$, form the union of the $g_\alpha(V_\alpha)$ for $\alpha \in A$ and denote the convex envelope in E of this union by $\Gamma((g_\alpha(V_\alpha)))$; since every element of E is of the form $\sum_{\alpha \in J} x_\alpha$, where J is a finite subset of I and $x_\alpha \in g_\alpha(F_\alpha)$, it is immediate that $\Gamma((g_\alpha(V_\alpha)))$ is an *absorbent* symmetric convex set in E (each of the $V_\alpha$ is absorbent in $F_\alpha$); as $\Gamma((g_\alpha(V_\alpha)))$ contains all the $g_\alpha(V_\alpha)$, it is a neighbourhood of 0 for $\mathcal{T}$. On the other hand, it is clear that for every symmetric convex neighbourhood V of 0 for $\mathcal{T}$, we have $V \supset \Gamma((V \cap g_\alpha(F_\alpha)))$, from which our assertion follows.

#### Corollary 1 {#evt-ii-s4-prop-5-cor-1 .statement}

*With the notations of prop. 5, let H be a set of linear mappings of E in the locally convex space G. Suppose that E is the sum of its subspaces $g_\alpha(F_\alpha)$; then H is equicontinuous for $\mathcal{T}$, if, and only if, for every $\alpha$, the set $f \circ g_\alpha$ where $f$ varies in H, is equicontinuous in $F_\alpha$.*

Remembering I, p. 9, prop. 6 the argument is similar to that of (ii) prop. 5. Let W be a symmetric convex neighbourhood of 0 in G and note that if the set $f \circ g_\alpha$, where $f \in H$ is equicontinuous, then the intersection $\bigcap_{f \in H} g_\alpha^{-1}(f^{-1}(W))$ is a symmetric convex neighbourhood of 0 in $F_\alpha$. As this intersection is the same as $g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W))$ and the set $\bigcap_{f \in H} f^{-1}(W)$ is symmetric and convex, everything depends on showing that it is also *absorbent*. Now, by hypothesis, every $x \in E$ can be written as $\sum_{i=1}^n g_{\alpha_i}(z_{\alpha_i})$, where $z_{\alpha_i} \in F_{\alpha_i}$. To show that there exists $\lambda > 0$ such that $f(\lambda x) \in W$ for all $f \in H$, it is sufficient to consider the case $x = g_\alpha(z_\alpha)$ with $z_\alpha \in F_\alpha$ (since we can pass to the general case by replacing W by $W/n$). But this case follows from the fact that $g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W))$ is a neighbourhood of 0 in $F_\alpha$.

#### Corollary 2 {#evt-ii-s4-prop-5-cor-2 .statement}

*Let $(J_\lambda)_{\lambda \in L}$ be a partition of the index set A. Let $(G_\alpha)_{\alpha \in A}$ be a family of locally convex spaces and $(F_\lambda)_{\lambda \in L}$ be a family of vector spaces. For each $\lambda \in L$, let $h_\lambda$ be a linear mapping of $F_\lambda$ in a vector space E; for each $\lambda \in L$ and $\alpha \in J_\lambda$, let $g_{\lambda \alpha}$ be a linear mapping of $G_\alpha$ in $F_\lambda$. Write $f_\alpha = h_\lambda \circ g_{\lambda \alpha}$. Suppose that each $F_\lambda$ carries the finest locally convex topology that makes the $g_{\lambda \alpha}$ ($\alpha \in J_\lambda$) continuous. Then, the finest locally convex topology on E that makes the $f_\alpha$ continuous, is identical with the finest locally convex topology making the $h_\lambda$ continuous.*

This is a particular case of S, IV, § 2.5 criterion CST 19, and can also be proved directly using prop. 5.

Examples of locally convex final topologies.

I. Quotient space.

Let M be a subspace of the locally convex space F, and φ be the canonical mapping of F on F/M. As the quotient topology on F/M is locally convex and is the finest of all the topologies (locally convex or not) which make φ continuous, it is also the locally convex final topology for the family consisting of the single mapping φ.

II. Inductive limits of locally convex spaces.

Let A be an ordered set directed to the right and let $(E_\alpha, f_{\beta\alpha})$ be an inductive system of vector spaces relative to the set A (A, II, § 6.2); let $E = \varinjlim E_\alpha$ and let $f_\alpha : E_\alpha \to E$ be the canonical linear mapping for each $\alpha \in A$. Suppose that each $E_\alpha$ carries a locally convex topology $\mathcal{T}_\alpha$, and further suppose that for $\alpha \leq \beta$, the mapping $f_{\beta\alpha} : E_\alpha \to E_\beta$ is *continuous*. Then we say that the locally convex final topology $\mathcal{T}$ of the family $(\mathcal{T}_\alpha)$ relative to the linear mappings $f_\alpha$ (resp. the space E carrying the topology $\mathcal{T}$) is the *inductive limit* of the family $(\mathcal{T}_\alpha)$ (resp. the *inductive limit* space of the system $(E_\alpha, f_{\beta\alpha})$, or simply of the locally convex spaces $E_\alpha$). Recall that E is the union of the vector subspaces $f_\alpha(E_\alpha)$ and that when $\alpha \leq \beta$, we have $f_\alpha(E_\alpha) \subset f_\beta(E_\beta)$; if we endow $f_\alpha(E_\alpha)$ with the final topology for the mapping $f_\alpha$ (which is the same as identifying $f_\alpha(E_\alpha)$ with the quotient space $E_\alpha/f_\alpha^{-1}(0)$), the topology $\mathcal{T}$ is also the final topology of the family of the topologies of the $f_\alpha(E_\alpha)$, relative to the canonical injections (II, cor. 2 above). Further, the continuity of $f_{\beta\alpha}$ for $\alpha \leq \beta$ implies that the canonical injection $j_{\beta\alpha} : f_\alpha(E_\alpha) \to f_\beta(E_\beta)$ is continuous, so that E is also the inductive limit of $f_\alpha(E_\alpha)$ carrying the preceding topologies relative to the injection $j_{\beta\alpha}$.

#### Example {#evt-ii-s4-n4-exa-1 .statement}

— Let X be a locally compact space and $E = \mathscr{K}(X; \mathbf{R})$ the vector space of finite continuous real valued functions defined over X with compact support. For every compact subset K of X, let $E_K$ be the vector subspace of E formed by those functions $f \in E$ which are such that $x \notin K \Rightarrow f(x) = 0$. Denote by $\mathcal{T}_K$ the topology induced on $E_K$ and by $\mathcal{T}_u$ the topology of *uniform convergence* on X. The inductive limit $\mathcal{T}$ of the topologies $\mathcal{T}_K$ is finer than $\mathcal{T}_u$; we can show that if X is paracompact and not compact, then $\mathcal{T}$ is strictly finer than $\mathcal{T}_u$ (*cf.* INT, III, 2nd ed., § 1.8). The importance of $\mathcal{T}$ lies in the fact that the linear forms on E that are continuous in $\mathcal{T}$ are precisely the real *measures* on X (INT, III, 2nd., § 1.3).

#### Remark {#evt-ii-s4-n4-rem-1 .statement}

— In the last example, the topology induced by $\mathcal{T}$ on $E_K$ is identical with $\mathcal{T}_K$, since by definition it is coarser than $\mathcal{T}_K$ and, since $\mathcal{T}$ is finer than $\mathcal{T}_u$, the topology induced by $\mathcal{T}$ on $E_K$ is finer than that induced by $\mathcal{T}_u$, that is to say $\mathcal{T}_K$.

This reasoning generalises immediately to an inductive limit of locally convex topologies $(\mathcal{T}_\alpha)$ when there is a locally convex topology $\mathcal{T}'$ on E such that $\mathcal{T}_\alpha$ is the topology induced on $E_\alpha$ by $\mathcal{T}'$.

More generally one can ask, when we suppose that $E_\beta \subset E_\alpha$ and $\mathcal{T}_\beta$ is the topology induced by $\mathcal{T}_\alpha$, under what circumstances $\mathcal{T}$ induces $\mathcal{T}_\alpha$ on each of the $E_\alpha$. In general this is not so (II, p. 80, exerc. 26); but we shall see in the Nos following two important situations where this does occur.

### 5. The direct topological sum of a family of locally convex spaces

#### Definition 2 {#evt-ii-s4-def-2 .statement}

*Let E be the vector space which is the direct sum* (A, II, § 1.6) *of the family of locally convex spaces* $(E_i)_{i \in I}$. *For each* $i \in I$, *let* $f_i$ *be the canonical injection* of $E_i$ in $E$. *By the topological direct sum of the family* $(E_i)$ *we mean the space* $E$ *with the finest locally convex topology which makes each* $f_i$ *continuous (this topology is called the direct sum of the topologies of the* $E_i$).

In the remainder of this No. we keep the same notations as in def. 2 (unless the contrary is expressly stated) and we identify, canonically, each $E_i$ with a subspace of $E$, by means of $f_i$.

By the general description of neighbourhoods of a locally convex final topology given in II, p. 28, we can here obtain a fundamental system of neighbourhoods of 0 in $E$ for the direct sum topology, in the following manner; for *every* family $(V_i)_{i \in I}$ where $V_i$ is a symmetric convex neighbourhood of 0 in $E_i$, consider the convex envelope $\Gamma((V_i))$, of the union of the $V_i$; the $\Gamma((V_i))$ for all the families $(V_i)$ (or only taking $V_i$ for each $i$ to be in a fundamental system of neighbourhoods of 0 in $E_i$) form a fundamental system of neighbourhoods of 0 in $E$.

#### Example {#evt-ii-s4-n5-exa-1 .statement}

— Let $(a_i)_{i \in I}$ be a basis of the vector space $E$ and consider the canonical topology (I, p. 2, *Example 5*) on each line $Ra_i$; the direct sum of these topologies is the *finest* locally convex topology on $E$ (II, p. 26); in fact, if $V$ is an absorbent, symmetric, convex set in $E$, then $V_i = V \cap Ra_i$ is a neighbourhood of 0 in $Ra_i$ and $V$ clearly contains the convex envelope $\Gamma((V_i))$.

#### Proposition 6 {#evt-ii-s4-prop-6 .statement}

*A locally convex topology* $\mathcal{T}$ *on* $E$ *is the direct sum of the topologies of the* $E_i$, *if and only if, the following property holds: a linear mapping of* $E$ *in a locally convex space* $G$ *(resp. a semi-norm* $p$ *on* $E$) *is continuous, if and only if, for every* $i \in I$, *the mapping* $g \circ f_i$ *(resp. $p \circ f_i$) is continuous in* $E_i$.

This is a particular case of prop. 5, II, p. 27.

Recalling the definition of the direct sum of a family of vector spaces (A, II, p. 12, prop. 6), we can say that the topology $\mathcal{T}$ is the only one for which the canonical mapping $g \mapsto (g \circ f_i)$ is a *bijection*

$$
\mathcal{L}(E; G) \to \prod_{i \in I} \mathcal{L}(E_i; G)
$$

for every locally convex space $G$.

#### Corollary {#evt-ii-s4-n5-cor-1 .statement}

*With the notation of prop. 5, II, p. 27, suppose that* $E$ *is the sum of the* $g_\alpha(F_\alpha)$. *Let* $F$ *be the topological direct sum of the family* $(F_\alpha)_{\alpha \in A}$, *and let* $j_\alpha : F_\alpha \to F$ *be the canonical injection; suppose that* $g : F \to E$ *is the linear mapping such that* $g \circ j_\alpha = g_\alpha$ *for all* $\alpha \in A$. *If* $N$ *is the kernel of* $g$, *then the canonical bijection* $F/N \to E$ *associated with* $g$ *is a topological isomorphism of* $F/N$ *on* $E$ *with the topology* $\mathcal{T}$.

This is a particular case of II, p. 28, cor. 2 remembering II, p. 29, *Example I*.

#### Proposition 7 {#evt-ii-s4-prop-7 .statement}

*The canonical injection* $j : E \to \prod_{i \in I} E_i$ *is continuous when* $E$ *carries the direct sum topology of the* $E_i$ *and* $\prod_{i \in I} E_i$ *carries the product topology. When* $I$ *is finite, this mapping is an isomorphism of topological vector spaces.*

The first assertion follows from the fact that the canonical injections $E_\kappa \to \prod_{\iota \in I} E_\iota$ are continuous for each $\kappa \in I$. If $I$ is finite then $j$ is the identity mapping, and it is sufficient to show that the product topology $\mathcal{T}'$ is finer than the direct sum topology $\mathcal{T}$. Now, let $V$ be a convex neighbourhood of 0 for $\mathcal{T}$; each set $V \cap E_\iota$ is a convex neighbourhood of 0 in $E_\iota$; if $n$ is the number of elements of $I$, then the set $V$ contains the set $\frac{1}{n} \sum_n (V \cap E_\iota)$, which is a neighbourhood of 0 for $\mathcal{T}'$, and the proposition is proved.

When $I$ is infinite, if, for each finite subset $J$ of $I$, we write $E_J$ for the space $\prod_{\iota \in J} E_\iota$, with the product topology, then $E$ is the *inductive limit* of the $E_J$ (identified as subspaces of $E$).

#### Proposition 8 {#evt-ii-s4-prop-8 .statement}

*Let $N_\iota$ be a subspace of $E_\iota$, for every $\iota \in I$,*

(i) *The topology induced on $N = \sum_\iota N_\iota$ by the direct sum topology $\mathcal{T}$ on $E$ is identical with the direct sum of the topologies of the $N_\iota$.*

(ii) *The canonical mapping $h$ of the topological direct sum space of the $E_\iota / N_\iota$ on $E/N$ (A, II, § 1.6, formula (26)) is an isomorphism between topological vector spaces.*

(i) With the notations introduced above, we consider $x = \sum_\iota \lambda_\iota x_\iota$ belonging to $N \cap \Gamma((V_\iota))$ ($(\lambda_\iota)$ is a family of numbers $\geqslant 0$ of which at most finitely many are non-zero, such that $\sum_\iota \lambda_\iota = 1$, and $x_\iota \in V_\iota$, for all $\iota \in I$). Since the sum of the $N_\iota$ is direct, we have $\lambda_\iota x_\iota \in N_\iota$ for all $\iota \in I$; therefore, for all $\iota$ such that $\lambda_\iota > 0$ we also have $x_\iota \in N_\iota \cap V_\iota$, and $x$ belongs to the convex envelope $\Gamma((N_\iota \cap V_\iota))$, thus (i) is proved.

(ii) Denote canonical mappings as follows: $f_\iota : E_\iota \to E, h_\iota : E_\iota / N_\iota \to E/N, p_\iota : E_\iota \to E_\iota / N_\iota$ and $p : E \to E/N$. For every $\iota \in I$, $h_\iota \circ p_\iota = p \circ f_\iota$ and the proposition follows from II, p. 28, cor. 2 and p. 29 *Example I*.

#### Corollary 1 {#evt-ii-s4-prop-8-cor-1 .statement}

*If $N_\iota$ is closed in $E_\iota$ for every $\iota \in I$, then $N = \sum_\iota N_\iota$ in closed in $E$.*

For, the canonical mapping $p_\iota : E \to E_\iota$ is continuous (II, § 4.5, prop. 6) for every $\iota \in I$, hence $p_\iota^{-1}(N_\iota)$ is closed in $E$, and thus the same is true of the intersection $N = \bigcap_{\iota \in I} p_\iota^{-1}(N_\iota)$.

#### Corollary 2 {#evt-ii-s4-prop-8-cor-2 .statement}

*If each $E_\iota$ is Hausdorff, so also is $E$ and each $E_\iota$ is closed in $E$.*

To prove the first statement apply cor. 1 taking $N_\iota = \{0\}$ for all $\iota \in I$; for the second apply cor. 1 with $N_\iota = E_\iota$ and $N_\kappa = \{0\}$ for every $\kappa \neq \iota$.

We shall show in III, p. 21, cor. 2 that if the $E_\iota$ are Hausdorff and *complete* then so is their topological direct sum $E$.

### 6. Inductive limits of sequences of locally convex spaces

In this No. we shall consider an *increasing sequence* $(E_n)$ of vector subspaces of a vector space $E$, such that $E$ is the *union* of the $E_n$; we suppose that each $E_n$ carries a locally convex topology $\mathcal{T}_n$, such that, for every $n$, the topology induced on $E_n$ by $\mathcal{T}_{n+1}$ is *coarser* than $\mathcal{T}_n$, and we give to $E$ the locally convex topology $\mathcal{T}$ that is the *inductive limit* of the sequence $(\mathcal{T}_n)$ (II, p. 29, *Example II*); these hypotheses and notations will be used throughout the rest of this No. without restatement.

It may happen that each $\mathcal{T}_n$ is Hausdorff but that $\mathcal{T}$ is not; it may also happen that for each pair of integers $n, m$ such that $n \leq m$, the subspace $E_n$ is closed in $E_m$ (using topology $\mathcal{T}_m$) but that $E_n$ is not closed in $E$ using $\mathcal{T}$ (II, p. 80, exerc. 26).

#### Lemma 1 {#evt-ii-s4-lem-1 .statement}

— *Let $\mathfrak{F}$ be a Cauchy filter on $E$ (for $\mathcal{T}$); then there exists an integer $k$, such that for all $N \in \mathfrak{F}$ and every neighbourhood $V$ of $0$ in $E$, the subspace $E_k$ meets $N + V$.*

We assume the contrary and obtain a contradiction. Suppose that for every $k$ there exists a convex neighbourhood $V_k$ of $0$ and a set $M_k \in \mathfrak{F}$ such that
$$
(E_k + V_k) \cap M_k = \varnothing.
$$
Clearly we can suppose that $V_{k+1} \subset V_k$ for all $k$. Let $V$ be the convex envelope of $\bigcup_k (E_k \cap V_k)$, this is clearly a neighbourhood of $0$ for $\mathcal{T}$. For all $n$ we have $V \subset V_n + E_n$; in fact, every $x \in V$ can be written $\sum_i \lambda_i x_i$ where $\lambda_i \geq 0$, $\sum_i \lambda_i = 1$ and $x_i \in V_i \cap E_i$ for all $i$; now for $i < n$ we have $x_i \in E_n$, therefore $\sum_{i < n} \lambda_i x_i \in E_n$; and for $i \geq n$ we have $x_i \in V_n$, therefore $\sum_{i \geq n} \lambda_i x_i \in V_n$ since $V_n$ is convex, contains $0$ and $\sum_{i \geq n} \lambda_i \leq 1$. Hence $V + E_n \subset V_n + E_n$ for all $n$. This being so, let $M \in \mathfrak{F}$ be a set that is $V$-small. For some integer $m$, $E_m \cap M$ is not empty; and we conclude that
$$
M \subset E_m + V \subset E_m + V_m;
$$
as $\mathfrak{F}$ is a filter, the set $M_m$ meets $M$ and therefore $E_m + V_m$; we have a contradiction which establishes the lemma.

#### Proposition 9 {#evt-ii-s4-prop-9 .statement}

*Suppose that the topology induced on $E_n$ by $\mathcal{T}_{n+1}$ is identical with $\mathcal{T}_n$ for every integer $n$. Then
(i) The topology induced by $\mathcal{T}$ on $E_n$ is identical with $\mathcal{T}_n$ for each $n$; if the $\mathcal{T}_n$ are Hausdorff then $\mathcal{T}$ is Hausdorff.
(ii) If, for every $n$, $E_n$ is closed in $E_{n+1}$ (for $\mathcal{T}_{n+1}$), then $E_n$ is closed in $E$ (using $\mathcal{T}$) for every $n$.
(iii) If each $E_n$ is complete (using $\mathcal{T}_n$) then $E$ is complete using $\mathcal{T}$.*

(i) To prove the first assertion, it is sufficient to prove that the topology $\mathcal{T}'_n$ induced by $\mathcal{T}$ on $E_n$ is finer than $\mathcal{T}_n$. For this, let $V_n$ be a convex neighbourhood of $0$ in $E_n$ for the topology $\mathcal{T}_n$; we are going to construct an increasing sequence of convex neighbourhoods of $0$ in $E_{n+p}$ for $\mathcal{T}_{n+p}$, say $(V_{n+p})_{p \geq 1}$, such that $V_{n+p} \cap E_n = V_n$ for every index $p \geq 1$. Then the union $V$ of the increasing sequence $(V_{n+p})$ will be a convex set such that $V \cap E_k$ is a neighbourhood of $0$ in $E_k$ (using $\mathcal{T}_k$), for every index $k$; therefore $V$ will be a neighbourhood of $0$ in $E$ for $\mathcal{T}$ and as $V \cap E_n = V_n$, we have proved that $\mathcal{T}'_n$ is finer than $\mathcal{T}_n$.

To define the $V_{n+p}$ we proceed by induction on $p$ using the following lemma:

#### Lemma 2 {#evt-ii-s4-lem-2 .statement}

*Let $V$ be a convex neighbourhood of 0 in $M$, a vector subspace of a locally convex space $F$. Then there exists a convex neighbourhood $W$ of 0 in $F$ such that $W \cap M = V$. Further, if $M$ is closed in $F$, then, for every point $x_0 \in \complement M$, there exists a convex neighbourhood $W_0$ of 0 in $F$ such that $W_0 \cap M = V$ and $x_0 \notin W_0$.*

In fact, by hypothesis there exists a convex neighbourhood $U$ of 0 in $F$ such that $U \cap M \subset V$. Clearly, the convex envelope $W$ of $U \cup V$ in $F$ is a neighbourhood of 0 in $F$; we show that $W \cap M = V$. For, every point $z \in W$ is of the form $\lambda x + (1-\lambda) y$ with $x \in V, y \in U$, and $0 \leq \lambda \leq 1$ (II, p. 9, prop. 8); if $z \in M$, and $\lambda \neq 1$ then necessarily $y \in M$, therefore $y \in U \cap M \subset V$ and hence $z \in V$; the result is obviously true if $\lambda = 1$. If $M$ is closed in $F$, the space $F/M$ is Hausdorff, thus there exists a convex neighbourhood $U_0 \subset U$ of 0 in $F$ such that $U_0$ does not meet $x_0 + M$; then the convex envelope $W_0$ of $U_0 \cup V$ fulfils the required conditions.

Returning to the theorem, to prove the second part of (i) note that if $x \in E$ then $x \in E_n$ for some $n$; if $x \neq 0$ and $\mathcal{T}_n$ is Hausdorff then there is a neighbourhood $V_n$ of 0 for $\mathcal{T}_n$, which does not contain $x$. We see that there is a neighbourhood $V$ of 0 for $\mathcal{T}$ such that $V \cap E_n = V_n$, hence $x \notin V$, and it follows that $\mathcal{T}$ is Hausdorff.

(ii) Let $x \in E - E_n$; there exists $m > n$ such that $x \in E_m$, thus, as $E_n$ is closed in $E_m$ for $\mathcal{T}_m$ (because of the hypothesis that $\mathcal{T}_{n+1}$ induces $\mathcal{T}_n$ on $E_n$ for every $n$) there exists in the topology $\mathcal{T}_m$ a convex neighbourhood $V_m$ of 0 in $E_m$ such that $(x + V_m) \cap E_n$ is empty. Now we saw in (i) that there exists a convex neighbourhood $V$ of 0 for $\mathcal{T}$ such that $V \cap E_m = V_m$; and thus $(x + V) \cap E_m = x + V_m$, therefore $(x + V) \cap E_n = \varnothing$, which proves (ii).

(iii) From lemma 1, if $\mathfrak{F}$ is a *minimal* Cauchy filter for $\mathcal{T}$ (GT, II, § 3.2) then there exists a $k$ such that the trace of $\mathfrak{F}$ on $E_k$ is a filter $\mathfrak{F}_k$; from (i) this last is a Cauchy filter for $\mathcal{T}_k$ and thus $\mathfrak{F}_k$ converges in $E_k$ by hypothesis; but as the filter on $E$ generated by $\mathfrak{F}_k$ is finer than $\mathfrak{F}$, we see that $\mathfrak{F}$ has a cluster point for $\mathcal{T}$ and thus converges for $\mathcal{T}$.

When for all $n$ the topology induced on $E_n$ by $\mathcal{T}_{n+1}$ is just $\mathcal{T}_n$ we say that $\mathcal{T}$ is the *strict inductive limit* of the sequence $(\mathcal{T}_n)$ and that the space $E$ with the topology $\mathcal{T}$ is the *strict inductive limit* of the sequence of locally convex spaces $E_n$.

#### Remark {#evt-ii-s4-n6-rem-1 .statement}

— 1) Suppose that $E$ is the union of an increasing directed, *non-enumerable* family of subspaces $(E_\alpha)_{\alpha \in I}$, each $E_\alpha$ having a locally convex topology $\mathcal{T}_\alpha$, such that, for $E_\alpha \subset E_\beta$, the topology induced on $E_\alpha$ by $\mathcal{T}_\beta$ is identical with $\mathcal{T}_\alpha$. It may be the case that the topology induced on each $E_\alpha$ by the topology $\mathcal{T}$ is equal to $\mathcal{T}_\alpha$ and that the $E_\alpha$ are *Hausdorff and complete, but that $E$ is not complete for $\mathcal{T}$* (INT, III, 2nd ed., § 1, exerc. 2).

2) Let $F$ be a locally convex space, which is the union of an increasing sequence of vector subspaces $(F_n)$, and for each index $n$, let $\mathcal{T}_n$ be the topology induced on $F_n$ by the topology $\mathcal{T}$ of $F$. One should beware that in general $\mathcal{T}$ is not the inductive limit of the $\mathcal{T}_n$.

3) Suppose that $E$ is the strict inductive limit of the sequence $(E_n)$; if $F$ is a closed (in $\mathcal{T}$) vector subspace of $E$, it may be the case that the strict inductive limit of the topologies induced by the $\mathcal{T}_n$ on $F \cap E_n$ *is strictly finer* than the topology induced by $\mathcal{T}$ (IV, p. 63, exerc. 10).

#### Proposition 10 {#evt-ii-s4-prop-10 .statement}

*Let E, F be two locally convex spaces. Suppose that :*

1) *There exists a family of Fréchet spaces* $(E_\alpha)$, *and for each $\alpha$ a linear mapping* $g_\alpha : E_\alpha \to E$, *such that the topology of E is the final locally convex topology for the family* $(g_\alpha)$.

2) *There exists a sequence of Fréchet spaces* $(F_n)$ *and for each n a continuous linear injection* $j_n : F_n \to F$ *such that* $F = \bigcup_n j_n(F_n)$.

*Then every linear mapping u of E in F, whose graph is closed in* $E \times F$, *is necessarily continuous.*

To prove that $u$ is continuous, it is sufficient to show that for every $\alpha$, the mapping $u \circ g_\alpha : E_\alpha \to F$ is continuous (II, p. 27, prop. 5). Now the graph of $u \circ g_\alpha$ is the inverse image of the graph of $u$ under the continuous mapping $g_\alpha \times 1_F : E_\alpha \times F \to E \times F$, and therefore is, by hypothesis, closed in $E_\alpha \times F$. We can, therefore, restrict ourselves to the case when E itself is a *Fréchet space*. But then the proposition is a particular case of I, p. 20, prop. 1.

#### Corollary {#evt-ii-s4-n6-cor-1 .statement}

*With the same hypotheses on E and F as in prop. 10 and assuming that E is Hausdorff, then every continuous surjective mapping v of F in E is a strict morphism.*

Let N be the kernel of $v$ and write $N_n = j_n^{-1}(N)$; then the mapping $j'_n : F_n / N_n \to F / N$, deduced from $j_n$ by taking quotients, is injective and continuous, also $F_n / N_n$ is a Fréchet space (since $N_n$ is closed) and $F / N$ is the union of the images under $j'_n$. By hypothesis, in the canonical factorisation $v : F \to F / N \xrightarrow{w} E$, the linear mapping $w$ is bijective and continuous and its graph in $(F / N) \times E$ is therefore *closed* (GT, I, § 8.1, cor. 2 of prop. 2). By the remarks at the beginning and by prop. 10, the inverse mapping $u$ of $w$ is therefore continuous and the corollary is proved.

\* Prop. 10 and its corollary apply in particular when E is a *complete bornological space* (III, p. 12) and F is the inductive limit of a sequence of Fréchet spaces. \*

### 7. Remarks on Fréchet spaces

We are going to consider prop. 2 of GT, IX, § 3.1 in the case of locally convex spaces.

#### Proposition 11 {#evt-ii-s4-prop-11 .statement}

*Let E be a metrisable locally convex space. The topology of E can be defined by a distance that is invariant under translations, and for which the open balls are convex.*

Let $(p_n)_{n \in \mathbf{N}}$ be a sequence of semi-norms that define the topology of E. Let $d_n$ be the pseudometric defined by $d_n(x, y) = \inf(p_n(x - y), 1/n)$ for $x, y$ in E; it is invariant under translations. For every $n \geq 0$, and every real number $R \geq 0$, let $B_{n, R}$ be the set of $x \in E$ for which $d_n(x, 0) < R$. If $R \geq 1/n$, then $B_{n, R} = E$, and in the other case $B_{n, R}$ is formed from the $x \in E$ such that $p_n(x) < R$; in all cases $B_{n, R}$ is convex.

For $x, y$ in $E$ define $d(x, y) = \sup_{n \in \mathbf{N}} d_n(x, y)$. We see immediately that $d$ is a distance, invariant under translations on $E$ and defining the topology of $E$. For $x_0 \in E$ and $R \geq 0$, the open ball with centre $x_0$ and radius $R$ (for the distance $d$) is equal to $\bigcap_{n \in \mathbf{N}} (x_0 + B_{n, R})$, therefore it is convex.

#### Proposition 12 {#evt-ii-s4-prop-12 .statement}

*Let $E$ and $F$ be two Fréchet spaces and $u$ a continuous linear mapping of $E$ on $F$. Then there exists a section of $u$ that is continuous though not necessarily linear.*

By prop. 11 there exists a distance $d$ in $E$, invariant under translations, defining the topology of $E$ and for which open balls are convex. Given $y$ and $y'$ in $F$, let $\delta(y, y')$ be the distance apart of the closed sets $u^{-1}(y)$ and $u^{-1}(y')$ in $E$. As $u$ is a strict morphism (I, p. 17, th. 1) the remark of GT, IX, § 3.1 shows that $\delta$ is a distance on $F$ defining the topology of $F$. We shall construct, inductively, a sequence of continuous mappings $(s_n)_{n \in \mathbf{N}}$ of $F$ in $E$ satisfying the following inequalities for all $y \in F$:

$$
\delta(y, u(s_n(y))) < 2^{-n}
$$
$$
d(s_n(y), s_{n-1}(y)) < 2^{-n+1} \quad \text{(only if } n \geq 1 \text{)}.
$$

Suppose then that either $n = 0$, or $n \geq 1$ and that $s_{n-1}$ has been constructed. Let $y_0 \in F$; as $u$ is surjective, the set $u^{-1}(y_0)$ is non-empty, and for $n \geq 1$, we have $d(u^{-1}(y_0), s_{n-1}(y_0)) < 2^{-n+1}$ by the induction hypothesis. Therefore there exists a point $x_0$ of $E$ such that $u(x_0) = y_0$ and for $n \geq 1$, $d(x_0, s_{n-1}(y_0)) < 2^{-n+1}$. As the mapping $s_{n-1}$ is continuous, the set of points $y$ of $F$ which satisfy the inequalities $\delta(y, y_0) < 2^{-n}$ and $d(x_0, s_{n-1}(y)) < 2^{-n+1}$ is an open neighbourhood of $y_0$. Hence there exist an open covering $(V_i)_{i \in I}$ of $F$ and constant mappings $s_{n,i}$ of $F$ in $E$ which satisfy the inequalities (2) and (3) *in* $V_i$ where one replaces $s_n$ by $s_{n,i}$. As the space $F$ is metrisable, there exists a continuous partition of unity $(f_i)_{i \in I}$, that is locally finite and subordinate to the covering $(V_i)_{i \in I}$ (GT, IX, § 4.5, th. 4 and § 4.4, cor. 1). For every $y \in F$, put $s_n(y) = \sum_{i \in I} f_i(y) \cdot s_{n,i}(y)$. The mapping $s_n$ of $F$ in $E$ is continuous; as the open balls are convex in $E$ and in $F$, the mapping $s_n$ satisfies the inequalities (2) and (3) for all $y \in F$.

From inequality (3) the mappings $s_n : F \to E$ form a Cauchy sequence, for uniform convergence. As $E$ is complete, the sequence $(s_n)_{n \in \mathbf{N}}$ converges uniformly to a continuous mapping $s : F \to E$ (GT, X, § 1.6); formula (2) shows that $u \circ s$ is the identity mapping of $F$, thus $s$ is a continuous section of $u$.

#### Corollary {#evt-ii-s4-n7-cor-1 .statement}

*If $L$ is a compact set in $F$, then there exists a compact set $K$ in $E$ such that $u(K) = L$.*

It is sufficient to put $K = s(L)$, where $s$ is a continuous section of $u$.

#### Remark {#evt-ii-s4-n7-rem-1 .statement}

— 1) The corollary to prop. 12 can also be deduced from th. 1 of I, p. 17 and prop. 18 of GT, IX, § 2.10.
2) We keep the notations of prop. 12. Let $p$ be a continuous semi-norm on $E$;

for all $y \in F$, put $q(y) = \inf_{u(x)=y} p(x)$, so that $q$ is a continuous semi-norm on $F$ (II, p. 4). Let $\phi$ be a lower semi-continuous mapping of $F$ in the interval $]0, +\infty[$ of $\overline{\mathbf{R}}$. We show that there exists a *continuous section s of u such that* $p \circ s < q + \phi$.

Let $s_0$ be a continuous section of $u$ (prop. 12) and $N$ the kernel of $u$. Let $y_0 \in F$, then there exists $z_0 \in N$ such that $p(s_0(y_0) + z_0) < q(y_0) + \phi(y_0)$. There exists an open neighbourhood $W$ of $y_0$ in $F$ such that $p(s_0(y) + z_0) < q(y) + \phi(y)$ for all $y \in W$. Hence there is an open covering $(W_i)_{i \in I}$ of $F$ and constant mappings $t_i : F \to N$ such that $p(s_0(y) + t_i(y)) < q(y) + \phi(y)$ for all $y \in W_i$. As $F$ is metrisable, there exists a locally finite continuous partition of unity subordinated to the covering $(W_i)_{i \in I}$, say $(g_i)_{i \in I}$ (GT, IX, § 4.5, th. 4 and § 4.4, cor. 1). The mapping $s$ of $F$ in $E$ defined by $s(y) = s_0(y) + \sum_{i \in I} g_i(y) \cdot t_i(y)$ fulfils the stated conditions.

### Exercises {#evt-ii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
