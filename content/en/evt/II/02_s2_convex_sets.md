---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 2
section_title: Convex sets
lang: en
source: evt-i-v
book_pages: TVS II.7-TVS II.21
pdf_pages: 0044-0058, 0102-0109
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a convex set
      page: 7
      pdf_page: 44
    - "no": 2
      title: Intersections of convex sets. Products of convex sets
      page: 9
      pdf_page: 46
    - "no": 3
      title: Convex envelope of a set
      page: 9
      pdf_page: 46
    - "no": 4
      title: Convex cones
      page: 10
      pdf_page: 47
    - "no": 5
      title: Ordered vector spaces
      page: 12
      pdf_page: 49
    - "no": 6
      title: Convex cones in topological vector spaces
      page: 13
      pdf_page: 50
    - "no": 7
      title: Topologies on ordered vector spaces
      page: 15
      pdf_page: 52
    - "no": 8
      title: Convex functions
      page: 16
      pdf_page: 53
    - "no": 9
      title: Operations on convex functions
      page: 18
      pdf_page: 55
    - "no": 10
      title: Convex functions over an open convex set
      page: 18
      pdf_page: 55
    - "no": 11
      title: Semi-norms and convex sets
      page: 19
      pdf_page: 56
statements: 51
exercises: 43
content_sha256: d061692d94255710b80728ad96183b04426f05c7ca01a6b75fc9fee6cfd79e73
---

## § 2. CONVEX SETS

### 1. Definition of a convex set

For any two points $x, y$ of an affine space $E$, the set of points $\lambda x + \mu y$ where $\lambda \geq 0, \mu \geq 0, \lambda + \mu = 1$ is called the closed segment with end points $x$ and $y$; it reduces to a point when $x = y$. The complement of $x$ in this segment is called the segment with end points $x, y$ which is open at $x$ and closed at $y$; it is empty if $x = y$. Finally the complement of $\{ x, y \}$ in the closed segment with end points $x, y$ is called the open segment with end points $x, y$; it is empty when $x = y$.

#### Definition 1 {#evt-ii-s2-def-1 .statement}

— A subset $A$ of an affine space $E$ is convex if, for every two points $x, y$ of $A$, the closed segment with end points $x, y$ is contained in $A$.

As $(1 - \lambda) a + \lambda x = a + \lambda (x - a)$, this definition is equivalent to the following: the set $A$ is convex if, for every point $a \in A$, the transform of $A$ by a homothety of centre $a$ and ratio $\lambda$ where $0 < \lambda < 1$, is contained in $A$ (in other words, $A$ is stable for these homotheties).

#### Example 1 {#evt-ii-s2-n1-exa-1 .statement}

Every linear affine variety of $E$ (and in particular the empty set) is convex.

#### Example 2 {#evt-ii-s2-n1-exa-2 .statement}

The only non-empty convex sets in $\mathbf{R}$ are the intervals (GT, IV, § 2.4, prop. 1).

#### Example 3 {#evt-ii-s2-n1-exa-3 .statement}

Let $E$ be a vector space and $\|x\|$ a norm on $E$; the unit ball $B$, formed by the points $x$

such that $\|x\| \leq 1$, is convex since the relations $\|x\| \leq 1, \|y\| \leq 1$, imply for $0 \leq \lambda \leq 1$ that
$$
\|\lambda x + (1 - \lambda) y\| \leq \lambda \|x\| + (1 - \lambda) \|y\| \leq \lambda + (1 - \lambda) = 1 .
$$

#### Remark {#evt-ii-s2-n1-rem-1 .statement}

— Let $A$ be a convex subset of a vector space $E$; for any scalars $\alpha > 0$ and $\beta > 0$ we have $\alpha A + \beta A = (\alpha + \beta) A$. In other words, for any $x \in A, y \in A$, there exists $z \in A$ such that $(\alpha + \beta) z = \alpha x + \beta y$; in fact this relation can be written $z = \frac{\alpha}{\alpha + \beta} x + \frac{\beta}{\alpha + \beta} y$ and we have $\frac{\alpha}{\alpha + \beta} > 0, \frac{\beta}{\alpha + \beta} > 0$ and $\frac{\alpha}{\alpha + \beta} + \frac{\beta}{\alpha + \beta} = 1$, from which the assertion follows, on using def. 1.

#### Proposition 1 {#evt-ii-s2-prop-1 .statement}

*Let $(x_i)$ be a family of points of a convex subset $A$; every barycentre $\sum_i \lambda_i x_i$ of the $x_i$ formed using positive masses $\lambda_i$ (such that $\sum_i \lambda_i = 1$ and $\lambda_i = 0$ except for finitely many of the indices, cf. A, II, § 9.3) belongs to $A$.*

Clearly we need only consider the case when the indices are $1, 2, ..., p$ and $\lambda_i > 0$ for each $i$; the proposition is trivial if $p = 1$; we prove the result by induction on $p$. Put $\mu = \sum_{i=1}^{p-1} \lambda_i > 0$, and $y = \sum_{i=1}^{p-1} \frac{\lambda_i}{\mu} x_i$; the induction hypothesis implies that $y \in A$. Now as $\lambda_p = 1 - \mu$ and $\sum_{i=1}^p \lambda_i x_i = \mu y + (1 - \mu) x_p$, its follows from def. 1 that $\sum_{i=1}^p \lambda_i x_i$ belongs to $A$.

#### Proposition 2 {#evt-ii-s2-prop-2 .statement}

*Let $E$ and $F$ be two affine spaces and $f$ be an affine linear mapping of $E$ in $F$; then the image of a convex subset of $E$ under $f$, and the inverse image of a convex subset of $F$ under $f$ are both convex.*

The image under $f$ of the closed segment with end points $x, y$ is the closed segment with end points $f(x), f(y)$, hence the first statement. We deduce that the inverse image of a closed segment of $F$ under $f$ contains each closed segment whose end points belong to it; the second statement of prop. 2 follows.

In particular the image of a convex set under a homothety or a translation is a convex set.

#### Proposition 3 {#evt-ii-s2-prop-3 .statement}

*In the affine space $E$, let $H$ be a hyperplane defined by the relation $g(x) = 0$, where $g$ is a non-constant affine function on $E$. Then the half-spaces defined by the relations $g(x) \geq 0, g(x) \leq 0, g(x) > 0, g(x) < 0$ are convex.*

For these are the inverse images under $g$ of intervals of $\mathbf{R}$ and thus are convex.

With the notations of prop. 3 the points of a subset $M$ of an affine space are *on the same side* (resp. *strictly on the same side*) of the hyperplane $H$ if $M$ is contained in one of the half-spaces defined by $g(x) \geq 0, g(x) \leq 0$ (resp. $g(x) > 0$ or $g(x) < 0$).

#### Proposition 4 {#evt-ii-s2-prop-4 .statement}

*The points of $A$, a convex subset of an affine space $E$ are strictly on the same side of a hyperplane $H$ if, and only if, $A$ does not meet $H$.*

Clearly the condition is necessary. Conversely suppose that it is satisfied and let $g(x) = 0$, be an equation defining H ($g$ is an affine linear mapping of E in $\mathbf{R}$). The set $g(A)$ is convex in $\mathbf{R}$, therefore it is an interval, and $0 \notin g(A)$. Hence $g(x)$ is of fixed sign for all $x \in A$.

### 2. Intersections of convex sets. Products of convex sets

#### Proposition 5 {#evt-ii-s2-prop-5 .statement}

— *The intersection of any family of convex subsets of an affine space* E *is convex*.

The proposition follows immediately from def. 1 of II, p. 7.

#### Proposition 6 {#evt-ii-s2-prop-6 .statement}

— *Let* $(E_i)_{i \in I}$ *be a family of vector spaces, and for each* $i \in I$, *let* $A_i$ *be a non-empty subset of* $E_i$. *Then the set* $A = \prod_{i \in I} A_i$ *is convex in* $E = \prod_{i \in I} E_i$, *if, and only if, for all* $i \in I$, *the set* $A_i$ *is convex in* $E_i$.

In fact, each projection $\mathrm{pr}_i$ is a linear mapping and we have $A_i = \mathrm{pr}_i A$ and $A = \bigcap_{i \in I} \mathrm{pr}_i^{-1}(A_i)$; the proposition follows from props. 2 and 5 above.

#### Corollary {#evt-ii-s2-n2-cor-1 .statement}

— *In the space* $\mathbf{R}^n$ *every parallelootope* (GT, VI, § 1.3) *is a convex subset*.

For it is the image under an affine linear mapping of a rectangular parallelepiped, and this last is convex by prop. 6.

#### Proposition 7 {#evt-ii-s2-prop-7 .statement}

— *Let* A *and* B *be two convex subsets of the vector space* E. *For any real numbers* $\alpha, \beta$ *the set* $\alpha A + \beta B$ *(set of points of the form* $\alpha x + \beta y$, *where* $x$ *varies in* A, *and* $y$ *in* B*) is convex*.

For $\alpha A + \beta B$ is the image of the convex subset $A \times B$ of $E \times E$ under the linear mapping $(x, y) \mapsto \alpha x + \beta y$ of $E \times E$ in $E$.

### 3. Convex envelope of a set

#### Definition 2 {#evt-ii-s2-def-2 .statement}

— *Given a subset* A *of an affine space* E, *we call the intersection of all convex sets containing* A, *the convex envelope of* A, *that is to say* (II, p. 9, prop. 5) *it is the smallest convex set containing* A.

#### Proposition 8 {#evt-ii-s2-prop-8 .statement}

— *For any family* $(A_i)_{i \in I}$ *of convex subsets of an affine space* E, *the convex envelope of* $\bigcup_{i \in I} A_i$ *is precisely the set of linear combinations* $\sum_{i \in I} \lambda_i x_i$, *where* $x_i \in A_i, \lambda_i \geq 0$ *for all* $i \in I$ ($\lambda_i = 0$ *except for finitely many indices*) *and* $\sum_{i \in I} \lambda_i = 1$.

Denote the set of these linear combinations by C, clearly C is contained in every convex set which contains all the $A_i$ (II, p. 8, prop. 1); on the other hand $A_i \subset C$ for every $i$. All that remains to be proved is that C is convex. Let $x = \sum \lambda_i x_i$, $y = \sum \mu_i y_i$ be two points of C and $\alpha$ be a number such that $0 < \alpha < 1$, write γ_i = αλ_i + (1 - α) μ_i for every i ∈ I, and let J be the set (finite) of the indices of I for which γ_i ≠ 0. We can write αx + (1 - α)y = ∑_{i∈J} γ_i z_i, where

$$ z_i = γ_i^{-1}(αλ_i x_i + (1 - α) μ_i y_i) $$

belongs to A_i for all i ∈ J; but $\sum_{i∈J} γ_i = α \sum_{i∈I} λ_i + (1 - α) \sum_{i∈I} μ_i = 1$, and we see that $ax + (1 - α) y ∈ C$. The proposition is proved.

#### Corollary 1 {#evt-ii-s2-prop-8-cor-1 .statement}

*The convex envelope of a subset A of E is identical with the set of linear combinations $\sum_i λ_i x_i$, where $(x_i)$ is any finite family of points of A, the numbers $λ_i > 0, \text{ for all } i$ and $\sum_i λ_i = 1$.*

The dimension of the affine linear variety (A, II, § 9.3) generated by the convex set A is called the *dimension* of A.

Let E be a vector space. The convex envelope C, of the balanced envelope of a set A in E is called the *balanced convex envelope* (or the *symmetric convex envelope*) of A; clearly it is the smallest symmetric convex set that contains A; it is also the convex envelope of $A \cup (-A)$, since every point of the balanced envelope of A belongs to a segment with extremities a and −a where $a ∈ A$. The set C coincides with the set of linear combinations $\sum_i λ_i x_i$ where $x_i ∈ A$ and $\sum_i |λ_i| ≤ 1$; for it is clear that this set of points is convex and contains A and −A; it is sufficient to prove that it is contained in C, and for this we need consider only those linear combinations for which $μ = \sum_i |λ_i| > 0$; we can then write $\sum_i λ_i x_i = μ \cdot \sum_i α_i y_i$ with $α_i = λ_i/μ$ and $y_i = x_i$, if $λ_i ≥ 0$; and $α_i = -λ_i/μ$; $y_i = -x_i$ if $λ_i < 0$; clearly $\sum_i α_i = 1$, and our assertion is proved.

#### Corollary 2 {#evt-ii-s2-prop-8-cor-2 .statement}

*Let f be an affine linear mapping of the affine space E in the affine space F; for each subset A of E, the convex envelope of f(A) is the image under f of the convex envelope of A.*

There is a similar statement for linear mappings and balanced convex envelopes.

### 4. Convex cones

#### Definition 3 {#evt-ii-s2-def-3 .statement}

*A subset C of an affine space E is a cone with vertex x_0 if C is invariant for all homotheties of centre x_0 and ratio > 0.*

We shall suppose in this No. and in the one following, that we have chosen the vertex of the cone being considered, as origin in E; *i.e.* we suppose that E is a vector space, and when we speak of a cone, it is to be understood that this cone has vertex 0. The set of points of the form $λa$ for $λ > 0$ (resp. $λ ≥ 0$), where $a$ is a non-null vector, is called an *open half line* (resp. *closed half-line*) originating at 0.

A cone C of vertex 0 is said to be *pointed* if $0 ∈ C$, and *non-pointed* otherwise. A pointed cone is either the single point $\{0\}$ or is the union of a set of closed half-lines originating at 0. A non-pointed cone is the union (possibly empty) of open half lines originating at 0. If C is a non-pointed cone, then $C \cup \{0\}$ is a pointed cone. If C is a pointed cone, then $C - \{0\}$ is a non-pointed cone.

If C is a non-pointed *convex* cone, then $C \cup \{0\}$ is a pointed convex cone. However, if C is a pointed convex cone, $C - \{0\}$ is not necessarily convex. We say that a pointed convex cone is *proper* if it does not contain any line passing through 0. Then

#### Proposition 9 {#evt-ii-s2-prop-9 .statement}

*A pointed convex cone C is proper if and only if the non-pointed cone $C'$, which is the complement of 0 in C, is convex.*

If C contains a line through 0 then clearly $C'$ is not convex. Suppose now that C is proper and let x, y be two points of $C'$. The closed segment with end points x, y is contained in C; if it contains 0 then $\lambda x + (1 - \lambda) y = 0$ for some $\lambda$ with $0 < \lambda < 1$, therefore $x = \mu y$ with $\mu < 0$. Thus C contains the line through 0 and x, contrary to hypothesis.

#### Proposition 10 {#evt-ii-s2-prop-10 .statement}

*A subset C of E is a convex cone if and only if $C + C \subset C$ and $\lambda C \subset C$ for all $\lambda > 0$.*

For the condition $\lambda C \subset C$ for all $\lambda > 0$ characterises the cones. If C is convex we have $C + C = \frac{1}{2}C + \frac{1}{2}C = C$ (II, p. 8, *Remark*). Conversely, if the cone C is such that $C + C \subset C$, then for $0 < \lambda < 1$, we have $\lambda C + (1 - \lambda) C = C + C \subset C$, which shows that C is convex.

#### Corollary 1 {#evt-ii-s2-prop-10-cor-1 .statement}

*If C is a non-empty convex cone, the vector space generated by C is the set $C - C$ (the set of points $x - y$ where x, y vary in C).*

For, if $V = C - C$, then V is non empty, we have $\lambda V = V$ for all $\lambda \neq 0$, and $V + V = C + C - (C + C) \subset C - C = V$, which shows that V is a vector subspace. Finally every vector subspace that contains C also contains V.

#### Corollary 2 {#evt-ii-s2-prop-10-cor-2 .statement}

*If C is a pointed convex cone, the largest vector subspace contained in C is the set $C \cap (-C)$.*

For, if $W = C \cap (-C)$, then W is non-empty and $\lambda W = W$ for all $\lambda \neq 0$, also
$$
W + W \subset (C + C) \cap (-(C + C)) \subset C \cap (-C) = W,
$$
which shows that W is a vector subspace. Clearly every vector subspace contained in C is also contained in W.

Obviously, if $f$ is a linear mapping of E in a vector space F, then $f(C)$, the image of a convex cone C in E, is a convex cone in F. Every intersection of convex cones (with vertex 0) in E is a convex cone. For every subset A of E the intersection of convex cones containing A (these exist, E itself is one such cone) is the smallest convex cone that contains A; it is called the convex cone *generated* by A.

#### Proposition 11 {#evt-ii-s2-prop-11 .statement}

*Let $(C_i)_{i \in I}$ be a family of convex cones in E; the convex cone generated by the union of the $C_i$ is identical with the set of points $\sum_{i \in J} x_i$, where J is any finite subset of I and $x_i \in C_i$ for all $i \in J$.*

In fact, it is obvious that C, the set of such points, is a convex cone containing the union of the $C_i$, and that it is contained in any convex cone which contains this union.

#### Corollary {#evt-ii-s2-n4-cor-1 .statement}

— *For any subset A of E, the convex cone generated by A, is identical with the set of linear combinations* $\sum_{i \in J} \lambda_i x_i$, *where* $(x_i)_{i \in J}$ *is any finite non-empty family of points of A, and where* $\lambda_i > 0$ *for all* $i \in J$.

It is sufficient to see that, if a convex cone contains a point $x \neq 0$ of A then it also contains the half-line $C_x$ of the points $\lambda x$ where $\lambda$ varies in the set of positive numbers and that $C_x$ is a convex cone.

#### Proposition 12 {#evt-ii-s2-prop-12 .statement}

— *If A is a convex set in E, then the convex cone generated by A is identical with* $C = \bigcup_{\lambda > 0} \lambda A$.

The set C is clearly a cone; it is sufficient to show that C is convex. Let $\lambda x, \mu y$ be two points of C ($\lambda > 0, \mu > 0, x \in A, y \in A$). Let $\alpha, \beta$ be two numbers $> 0$ such that $\alpha + \beta = 1$. Then $\alpha \lambda x + \beta \mu y = (\alpha \lambda + \beta \mu) z$, with $z \in A$, and $\alpha \lambda + \beta \mu > 0$; hence $\alpha \lambda x + \beta \mu y \in C$.

#### Remark {#evt-ii-s2-n4-rem-1 .statement}

— 1) With the hypotheses of prop. 12, if $0 \notin A$, then the cone C is non-pointed, thus $C \cup \{0\}$ is *proper*.

2) Let A be any convex set in E; consider the convex set $A_1 = A \times \{1\}$ in the space $F = E \times \mathbf{R}$ and the convex cone C with vertex 0 that is generated by $A_1$. Prop. 12 shows that $A_1$ is the intersection of C and of the hyperplane $E \times \{1\}$ in F. Every convex set in E can, therefore, be considered as the projection on E of the intersection of a convex cone with vertex 0 in F and the hyperplane $E \times \{1\}$.

### 5. Ordered vector spaces

A *preorder* structure, on a vector space E, denoted by $x \leqslant y$ or $y \geqslant x$, is *compatible* with the vector space structure of E if it satisfies the following two axioms;

*(EO$_I$)* *If* $x \leqslant y$ *then* $x + z \leqslant y + z$ *for all* $z \in E$.

*(EO$_II$)* *If* $x \geqslant 0$ *then* $\lambda x \geqslant 0$ *for every scalar* $\lambda \geqslant 0$.

The vector space E, carrying these two structures, is called a *preordered vector space* (resp. *an ordered vector space* when the relation of preorder on E is an order).

Note that axiom (EO$_I$) means that the preorder structure and the additive group structure of E are compatible, that is to say, E carrying these two structures, is a *preordered group* (A, VI, p. 3).

#### Example {#evt-ii-s2-n5-exa-1 .statement}

— On the space $E = \mathbf{R}^A$ of all finite real-valued functions defined over A, the relation of order given by « for all $t \in A$, $x(t) \leqslant y(t)$ » is compatible with the vector space structure of E.

#### Proposition 13 {#evt-ii-s2-prop-13 .statement}

— (i) *The set P, of elements* $\geqslant 0$, *of a preordered vector space E, is a pointed convex cone*.

(ii) *Conversely, if P is a pointed convex cone in E, then the relation* $y - x \in P$ *is a preorder relation on E, and the preorder structure that it defines is the only one that is* compatible with the vector space structure of E and for which P is the set of elements $\geqslant 0$.

(iii) The relation $y - x \in P$, with P a pointed convex cone, is an order relation on E if and only if P is a proper cone.

(i) Axioms (EO_I) and (EO_{II}) imply $P + P \subset P$ and $\lambda P \subset P$ for all $\lambda > 0$. As $0 \in P$, it follows that P is a pointed convex cone (II, p. 11, prop. 10).

(ii) Conversely, if P is a pointed convex cone, the relation $P + P \subset P$ implies that the relation $y - x \in P$ is a preorder compatible with the additive group structure of E (A, VI, p. 3, prop. 3); clearly writing it $x \leqslant y$, the set P is identical with the set of $x \geqslant 0$; further the relation $\lambda P \subset P$ for all $\lambda \geqslant 0$ shows that axiom (EO_{II}) is satisfied.

(iii) To say that P is proper means that $P \cap (-P) = \{0\}$ (II, p. 11, cor. 2), hence that $y - x \in P$ is an order relation.

#### Example {#evt-ii-s2-n5-exa-2 .statement}

\* Let H be a real Hilbert space; in the vector space $\mathcal{L}(H)$ of continuous endomorphisms of H, the positive hermitian endomorphisms form a proper pointed convex cone; this cone, therefore, defines an order structure compatible with the vector space structure of $\mathcal{L}(H)$ and for which the relation $A \leqslant B$ means that $B - A$ is a positive hermitian endomorphism. \*

For any pointed convex cone P in the vector space E, the set $P \cap (-P)$ is a vector subspace, H, of E (II, p. 11, cor. 2). The canonical image $P'$ of P in $E/H$ is a convex cone and the inverse image of $P'$ in E is P. Thus $P' \cap (-P') = \{0\}$, and $P'$ defines an order structure on $E/H$ that is compatible with its vector space structure.

A linear form $f$ on a preordered vector space E is said to be positive if $x \geqslant 0$ in E implies $f(x) \geqslant 0$. Or, alternatively, if the convex cone P of elements $\geqslant 0$ in E is contained in the half space of those $x$ for which $f(x) \geqslant 0$. Clearly, in the dual $E^*$ to E, the set of positive linear forms is a pointed convex cone.

### 6. Convex cones in topological vector spaces

#### Proposition 14 {#evt-ii-s2-prop-14 .statement}

In a topological vector space E, the closure of a convex set (resp. of a convex cone) is a convex set (resp. a convex cone with the same vertex).

For, let A be a convex set; the mapping $(x, y) \mapsto \lambda x + (1 - \lambda) y$, where $0 < \lambda < 1$, is continuous in $E \times E$ and maps $A \times A$ in A; thus (GT, I, § 2.1, th. 1) it maps $\overline{A} \times \overline{A}$ in $\overline{A}$, which shows that $\overline{A}$ is convex. Similarly, if C is a convex cone with vertex 0 then $\overline{C} + \overline{C} \subset \overline{C}$ and $\lambda \overline{C} \subset \overline{C}$ for all $\lambda > 0$.

#### Definition 4 {#evt-ii-s2-def-4 .statement}

For any set A of a topological vector space E, the intersection of all the closed convex sets containing A is called the convex closed envelope of A; it is the smallest convex closed set containing A.

From prop. 14, the convex closed envelope of A is the closure of the convex envelope of A; it is clearly the same as the convex closed envelope of $\overline{A}$.

Similarly we call the smallest symmetric, convex, closed set that contains A, the symmetric convex closed envelope (or the balanced convex closed envelope) of A; it is the closure of the symmetric convex envelope of A (II, p. 10); it is also the symmetric convex closed envelope of $\overline{A}$.

#### Proposition 15 {#evt-ii-s2-prop-15 .statement}

— Let $A_i$ ($1 \leq i \leq n$) be a finite number of compact convex sets in a Hausdorff topological vector space E. Then the convex envelope of the union of the $A_i$ is compact (and is, therefore, the same as the convex closed envelope of this union).

Let B be the compact set in $\mathbf{R}^n$ defined by the points $(\lambda_1, \lambda_2, ..., \lambda_n)$ where $\lambda_i \geq 0$ ($1 \leq i \leq n$), and $\sum_{i=1}^n \lambda_i = 1$. Define a continuous mapping of $B \times \prod_{i=1}^n A_i \subset \mathbf{R}^n \times E^n$ in E by the formula $(\lambda_1, \lambda_2, ..., \lambda_n, x_1, x_2, ..., x_n) \mapsto \sum_{i=1}^n \lambda_i x_i$. The convex envelope C of $\bigcup_{i=1}^n A_i$ is the image of $B \times \prod_{i=1}^n A_i$ under this mapping; as $B \times \prod_{i=1}^n A_i$ is compact and E is Hausdorff, it follows that C is compact.

#### Corollary 1 {#evt-ii-s2-prop-15-cor-1 .statement}

— In a Hausdorff topological vector space the convex envelope of a finite set is compact.

#### Corollary 2 {#evt-ii-s2-prop-15-cor-2 .statement}

— In a topological vector space E, the convex envelope of a finite set is precompact.

In fact, let j be the canonical mapping of E in its Hausdorff completion $\hat{E}$; if C is the convex envelope of A, then $j(C)$ is the convex envelope of the finite set $j(A)$ in $\hat{E}$, hence $j(C)$ is compact (cor. 1) and therefore C is precompact (GT, II, § 4.2).

#### Proposition 16 {#evt-ii-s2-prop-16 .statement}

— Let A be a convex subset, with at least one interior point $x_0$, of a topological vector space E. For any point $x \in \overline{A}$, every point of the open segment with end points $x_0, x$ lies in the interior of A.

For any point y of this segment, let f be the homothety of centre y and ratio $\lambda < 0$, which transforms $x_0$ into x. If V is an open neighbourhood of $x_0$ contained in A, then $f(V)$ is a neighbourhood of x and therefore contains a point $f(z) \in A$; now

$$
f(z) - y = \lambda (z - y) = \lambda (z - f(z)) + \lambda (f(z) - y),
$$

hence $y - f(z) = \frac{\lambda}{\lambda - 1} (z - f(z))$, so that y is transformed into z by the homothety g, of centre $f(z)$ and ratio $\mu = \lambda / (\lambda - 1)$; since $0 < \mu < 1$, g transforms V into a neighbourhood of 0 contained in A. The proposition is proved.

#### Corollary 1 {#evt-ii-s2-prop-16-cor-1 .statement}

— The interior $\overset{\circ}{A}$ of a convex set $\overline{A}$, is itself a convex set; if $\overset{\circ}{A}$ is not empty, then it coincides with the interior of $\overline{A}$, and $\overline{A}$ is a convex set that coincides with the closure of $\overset{\circ}{A}$.

It follows from prop. 16, that if $\overset{\circ}{A}$ is not empty, then it is a convex set and every point of $\overline{A}$ is a cluster point of $\overset{\circ}{A}$. Next we show that every interior point of $\overline{A}$ belongs to $\overset{\circ}{A}$. Let x be an interior point of $\overline{A}$ and suppose, for definiteness that $x = 0$. Let V be a symmetric neighbourhood of 0 that is contained in $\overline{A}$ and let $y \in \overset{\circ}{A} \cap V$; now $-y \in \overline{A}$, and therefore, by prop. 16, we see that $0 \in \overset{\circ}{A}$, if $y \neq 0$; this is obviously true if $y = 0$.

#### Corollary 2 {#evt-ii-s2-prop-16-cor-2 .statement}

— *The interior* $\dot{C}$ *of a convex cone* C, *is itself a convex cone; if* $\dot{C}$ *is not empty then it coincides with the interior of* $\overline{C}$, *and* $\overline{C}$ *is a pointed convex cone that coincides with the closure of* $\dot{C}$.

Since homotheties of ratio $> 0$ and centre 0 transform C into itself, they do the same for $\dot{C}$, thus $\dot{C}$ is a cone; the remainder of the corollary follows from cor. 1 and the obvious remark that if C is not empty then $\overline{C}$ contains the vertex of C.

Let H be a closed hyperplane in the topological vector space E over $\mathbf{R}$; it has an equation of the form $f(x) = \alpha$, where $f$ is a continuous linear form that is not identically zero in E (I, p. 13, th. 1). The closed half spaces defined respectively by $f(x) \leqslant \alpha$ and $f(x) \geqslant \alpha$ are therefore *closed* convex sets; their complements defined respectively by $f(x) > \alpha$ and $f(x) < \alpha$, are *open* convex sets. We say that these half-spaces are the closed (resp. open) half spaces *determined* by H.

#### Proposition 17 {#evt-ii-s2-prop-17 .statement}

— *In a topological vector space* E, *let* A *be a set with at least one interior point, and such that all its points lie on the same side of an hyperplane* H. *Then* H *is closed, the interior points of* A *lie strictly on the same side of* H, *and the cluster points of* A *lie on the same side of* H. *In particular open (resp. closed) half spaces are determined by closed hyperplanes*.

In fact suppose that H contains the origin and that $f(x) = 0$ is an equation of H; suppose, for definiteness, that $f(x) \geqslant 0$ for all $x \in A$. The half space formed by the points y such that $f(y) > -1$ contains at least one interior point, and, by translation, the same is true of the half space of points y such that $f(y) > 0$; this shows that H is closed (I, p. 11, corollary). Then we know that $f$ is a strict morphism of E on $\mathbf{R}$ (I, p. 13, corollary), therefore $f(\dot{A})$ is an open set in $\mathbf{R}$. This set cannot contain 0 or it would contain numbers $< 0$ contrary to hypothesis; it is thus contained in the open interval $]0, +\infty[$. On the other hand, the half space of those y for which $f(y) \geqslant 0$ is closed and contains A, therefore it contains $\overline{A}$.

#### Corollary {#evt-ii-s2-n6-cor-1 .statement}

— *Let* P *be a pointed convex cone, with at least one interior point, of the topological vector space* E. *Then each linear form* f *that is not identically zero on* E, *and is positive for the preorder structure defined by* P (II, p. 13), *is necessarily continuous*. *Further, if* x *is interior to* P *then* $f(x) > 0$ *and if* x *is a cluster point of* P *then* $f(x) \geqslant 0$.

Apply prop. 17 to the case $A = P$ where H is the hyperplane with the equation $f(x) = 0$.

#### Remark {#evt-ii-s2-n6-rem-1 .statement}

In a topological vector space E, every convex set C is connected. In fact, if $a \in C$, then C is a union of segments with end point a and closed at a; these are connected and the result follows from GT, I, § 11.1, prop. 2.

### 7. Topologies on ordered vector spaces

Let E be an ordered vector space. A topology on E is *compatible* with the ordered vector space structure of E if it is both compatible with the vector space structure of E and subject to the following axiom :

(TO) *The convex cone of the* x *with* $x \geqslant 0$, *is closed in* E.

An ordered vector space E with a compatible topology is called an ordered topological vector space.

#### Example {#evt-ii-s2-n7-exa-1 .statement}

The space $\mathbf{R}^n$ with its usual topology and the order structure that is the product of the order structure of its factors is an ordered topological vector space. On the other hand, for $n \geq 2$, when $\mathbf{R}^n$ carries the lexicographical order (S, III, § 2.6), the usual topology is not compatible with the ordered vector space structure of $\mathbf{R}^n$.

Let A be a set; the vector space $\mathcal{B}(A ; \mathbf{R})$ of real valued bounded functions defined on A, with the topology defined by the norm $\|x\| = \sup_{t \in A} |x(t)|$ and the order structure induced by the product order structure of $\mathbf{R}^A$, is an ordered topological vector space.

In an ordered topological vector space E, the set of elements $x \leq 0$ is closed; since translations are homeomorphisms, we deduce that, for all $a \in E$, the set of elements $x \geq a$ (resp. $x \leq a$) is closed. Since $\{0\}$ is the intersection of the sets $x \geq 0$ and $x \leq 0$, it follows that $\{0\}$ is closed and that E is Hausdorff.

#### Proposition 18 {#evt-ii-s2-prop-18 .statement}

In an ordered topological vector space E, let H be a set directed by the relation $\leq$. If the section filter of H has a limit in E, then this limit is the upper bound of H.

For, let $b = \lim_{x \in H} x$; for every $y \in H$, the set of $x \in H$ such that $x \geq y$ is a set of the section filter of H, therefore b is a cluster point of this set; but as the set $x \geq y$ is closed in E, we have $b \geq y$, thus b is an upper bound of H. On the other hand, if a is an upper bound of H, then H is contained in the closed set $x \leq a$; as b is a cluster point of H, we have $b \leq a$, which completes the proof (II, p. 72, exerc. 42).

### 8. Convex functions

#### Definition 5 {#evt-ii-s2-def-5 .statement}

Let X be a convex subset of the affine space E. A real-valued finite function, defined over X is convex (resp. strictly convex) if for any two distinct points x, y of X and any real number $\lambda, 0 < \lambda < 1$, we have:

(1)
$$
f(\lambda x + (1 - \lambda) y) \leq \lambda f(x) + (1 - \lambda) f(y)
$$
(resp.

(2)
$$
f(\lambda x + (1 - \lambda) y) < \lambda f(x) + (1 - \lambda) f(y)).
$$

When $E = \mathbf{R}$, this definition of convex function is the same as that in FVR, I, p. 32. Further, f is convex (resp. strictly convex) in X if, and only if, for every affine line $D \subset E$, the restriction of f to $X \cap D$ is convex (resp. strictly convex) in $X \cap D$.

#### Example {#evt-ii-s2-n8-exa-1 .statement}

If f is an affine linear function on E, then f and $f^2$ are convex functions on E; this is obvious for f since
$$
f(\lambda x + (1 - \lambda) y) = \lambda f(x) + (1 - \lambda) f(y);
$$
on the other hand, if $\alpha = f(x), \beta = f(y)$, then;
$$
\lambda \alpha^2 + (1 - \lambda) \beta^2 - (\lambda \alpha + (1 - \lambda) \beta)^2 = \lambda(1 - \lambda) (\alpha - \beta)^2 \geq 0
$$

for $0 < \lambda < 1$; further, the restriction of $f^2$ to an affine line $D \subset E$ is *strictly convex if $f|D$ is not a constant*.

A real-valued function $f$, defined over $X$, is *concave* (resp. *strictly concave*) if — $f$ is convex (resp. strictly convex). That is to say, for every two distinct points $x, y$ of $X$ and every number $\lambda$, such that $0 < \lambda < 1$, we have

$$
f(\lambda x + (1 - \lambda) y) \geqslant \lambda f(x) + (1 - \lambda) f(y)
$$

(resp.

$$
f(\lambda x + (1 - \lambda) y) > \lambda f(x) + (1 - \lambda) f(y)).
$$

A mapping of $X$ in $\mathbf{R}$ is *affine* if it is both convex and concave (*cf.* II, p. 78, exerc. 11).

#### Proposition 19 {#evt-ii-s2-prop-19 .statement}

*Let $X$ be a convex set of the affine space $E$; and let $f$ be a real-valued function defined over $X$. Denote the set of points $(x, a) \in E \times \mathbf{R}$ for which $x \in X$ and $f(x) \leqslant a$ (resp. $x \in X$ and $f(x) < a$) by $F$ (resp. $F'$). Then the following conditions are equivalent*:

a) *The function $f$ is convex*.
b) *The set $F$ in the affine space $E \times \mathbf{R}$ is convex*.
c) *The set $F'$ in the affine space $E \times \mathbf{R}$ is convex*.

We show that $a) \Rightarrow c)$. Let $(x, a)$ and $(y, b)$ be two points of $F'$ and $0 < \lambda < 1$, then $f(x) < a,\ f(y) < b$ and if $f$ is convex

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda f(x) + (1 - \lambda) f(y) < \lambda a + (1 - \lambda) b
$$

which shows that the point $\lambda(x, a) + (1 - \lambda)(y, b)$ of $E \times \mathbf{R}$ belongs to $F'$. Thus $F'$ is convex.

Next we show that $c) \Rightarrow b)$. If $(x, a), (y, b)$ are two points of $F$ then for every $\varepsilon > 0$, $(x, a + \varepsilon)$ and $(y, b + \varepsilon)$ belong to $F'$ and, if $0 < \lambda < 1$, the same is true of $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b + \varepsilon)$; by the definition of $F$ this implies that $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$ belongs to $F$.

Finally $b) \Rightarrow a)$, for (with the above notation), if $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$ belongs to $F$ then

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda a + (1 - \lambda) b
$$

provided $a \geqslant f(x)$ and $b \geqslant f(y)$; hence (1) follows and $f$ is convex.

#### Corollary {#evt-ii-s2-n8-cor-1 .statement}

*If $f$ is convex in $X$, then for all $\alpha \in \mathbf{R}$, the set of $x \in X$ such that $f(x) \leqslant \alpha$ (resp. $f(x) < \alpha$) is convex*.

In fact, it is the projection on $E$ of the intersection of $F$ (resp. $F'$) and the hyperplane $E \times \{\alpha\}$ in $E \times \mathbf{R}$.

#### Proposition 20 {#evt-ii-s2-prop-20 .statement}

*Let $f$ be a convex function, defined over a convex set $X$ of the affine* space E. Then for every family $(x_i)_{1 \leq i \leq p}$ of $p$ points of X and every family $(\lambda_i)_{1 \leq i \leq p}$ of $p$ real numbers, all $\geq 0$, such that $\sum_{i=1}^p \lambda_i = 1$, we have:

(3)
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

If $f$ is strictly convex and if $\lambda_i > 0$ for all $i$, then

(4)
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i),
$$
unless all the $x_i$ are equal.

The inequality (3) follows from II, prop. 19 above and II, p. 8, prop. 1. Suppose that the $x_i$ are not all equal (which implies $p \geq 2$) and that the $\lambda_i$ are all $> 0$; then the point $z = \sum_{i=1}^p \lambda_i x_i$ differs from at least one $x_i$. Suppose for definiteness that $z \neq x_1$, write $z = \lambda_1 x_1 + (1 - \lambda_1) y_1$ where $y_1 = \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} x_i$. Then $y_1 \neq x_1$ and, as $0 < \lambda_1 < 1$, we have, by hypothesis,
$$
f(z) < \lambda_1 f(x_1) + (1 - \lambda_1) f(y_1).
$$
But by (3) $f(y_1) \leq \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} f(x_i)$, and the inequality (4) follows.

### 9. Operations on convex functions

Let X be a convex set of an affine space E. If $f_i (1 \leq i \leq p)$ are finitely many convex functions defined over X and $c_i (1 \leq i \leq p)$ are numbers $\geq 0$ then the function $f = \sum_{i=1}^p c_i f_i$ is convex over X.

If $(f_i)$ is any family of convex functions defined over X and if $g$, the upper envelope of the family in X, is finite then $g$ is convex.

Finally if H is a set of convex functions defined over X, and $\mathfrak{F}$ is a filter on H that converges simply in X to the finite real valued function $f_0$, then $f_0$ is convex over X.

### 10. Convex functions over an open convex set

#### Proposition 21 {#evt-ii-s2-prop-21 .statement}

Let $f$ be a convex function, defined over the non-empty open convex set X in the topological vector space E. Then $f$ is continuous if, and only if, it is bounded above when restricted to some non-empty open subset U of X.

The condition is obviously necessary, we prove that it is sufficient. Let $x_0 \in X$ be a point such that $f$ is bounded above in a neighbourhood V of $x_0$; we show firstly that $f$ is continuous at $x_0$. By translation, we can restrict ourselves to the case when $x_0 = 0$ and $f(x_0) = 0$; moreover we can suppose that the neighbourhood V is balanced (I, p. 7, prop. 4). Suppose that $f(x) \leq a$ in V; for every $\varepsilon, 0 < \varepsilon < 1$, we observe that if $x \in \varepsilon V$, then $x/\varepsilon \in V$ and $-x/\varepsilon \in V$. Applying inequality (1) of II, p. 16 to the points $x/\varepsilon$ and 0 and to the number $\lambda = \varepsilon$, we see that $f(x) \leq \varepsilon f(x/\varepsilon) \leq \varepsilon a$; applying it to points $x$ and $-x/\varepsilon$ and the number $\lambda = 1/(1 + \varepsilon)$, gives $f(x) \geq -\varepsilon f(-x/\varepsilon) \geq -\varepsilon a$. Thus $f(x)$ is arbitrarily small in $\varepsilon V$, if $\varepsilon$ is sufficiently small, and $f$ is continuous at $x = 0$.

Now let $y$ be some point of X; since X is open, there is a number $\rho > 1$ such that $z = \rho y$ belongs to X. Let $g$ be the homothety $x \mapsto \lambda x + (1 - \lambda)z$ of centre $z$ and ratio $\lambda = 1 - \frac{1}{\rho}$, which transforms 0 into $y$; for every point $g(x) \in g(V)$, we have from (1)

$$
f(g(x)) \leq \lambda f(x) + (1 - \lambda) f(z) \leq \lambda a + (1 - \lambda) f(z) .
$$

Thus $f$ is bounded above in a neighbourhood of $y$ and hence, by the first part, is continuous at $y$. The proposition is proved.

#### Corollary {#evt-ii-s2-n10-cor-1 .statement}

*Every convex function f defined over an open convex set X in $\mathbf{R}^n$ is continuous in X.*

We can suppose that X is not empty. Then there exist, in X, $n + 1$ affinely independent points $a_i$ ($0 \leq i \leq n$) and the convex envelope of these points, S, contains the open non-empty set formed of the points $\sum_{i=0}^n \lambda_i a_i$ with $0 < \lambda_i < 1$ for all $i$ and $\sum_{i=0}^n \lambda_i = 1$. By II, p. 17, prop. 20, $f$ is bounded above in S and therefore is continuous.

In a topological vector space of infinite dimensions there exist, in general, linear non-continuous forms (II, p. 80, exerc. 25) and thus convex functions that are not continuous at any point.

### 11. Semi-norms and convex sets

Let E be a vector space over $\mathbf{R}$; a mapping $p$ of E in $\mathbf{R}$ is *positively homogeneous* if, for every $\lambda \geq 0$ and all $x \in E$ we have

$$
p(\lambda x) = \lambda p(x) .
$$

A positively homogeneous function $p$ on E is convex if, and only if, it satisfies axiom (SN$_{\text{II}}$) of II, p. 1 for all $x, y$ of E;

$$
p(x + y) \leq p(x) + p(y) .
$$

In fact, if $p$ is convex, then for $x, y$ in E,

$$
p(\frac{1}{2}(x + y)) \leq \frac{1}{2}p(x) + \frac{1}{2}p(y)
$$

and, by (5), this relation is equivalent to (6). Conversely, if (6) holds, then we also have for all $\lambda$ such that $0 < \lambda < 1$,

$$
p(\lambda x + (1 - \lambda) y) \leq p(\lambda x) + p((1 - \lambda) y) = \lambda p(x) + (1 - \lambda) p(y)
$$

using (5).

A convex positively homogeneous function on E is called *sub-linear*.

If $p$ is a sub-linear function defined on E; then, by II, § 2.8, corollary, for all $a > 0$, the set $V(p, a)$ (resp. $W(p, a)$) of points $x \in E$ for which $p(x) \leq a$ (resp. $p(x) < a$) is convex; further this set is *absorbent*, since for all $x \in E$, there exists $\lambda > 0$ such that $p(\lambda x) = \lambda p(x) < a$.

There is a partial converse of this result:

#### Proposition 22 {#evt-ii-s2-prop-22 .statement}

*Let A be a convex set, containing 0, in the vector space E. For all $x \in E$, put*

$$
p_A(x) = \inf_{\rho > 0, x \in \rho A} \rho
$$
(0 $\leq p_A(x) \leq \infty$). *The function $p_A$ satisfies*
$$
p_A(x + y) \leq p_A(x) + p_A(y), \qquad p_A(\lambda x) = \lambda p_A(x)
$$
*for all $x, y$ in E and $\lambda > 0$. If $V(p_A, \alpha)$ (resp. $W(p_A, \alpha)$) denotes the set of $x \in E$ for which $p_A(x) \leq \alpha$ (resp. $p_A(x) < \alpha$), then*
$$
W(p_A, 1) \subset A \subset V(p_A, 1).
$$
*If A is absorbent then $p_A$ is finite* (therefore *sublinear*).

Since the relations $x \in \rho A$ and $\lambda x \in \lambda \rho A$ are equivalent when $\lambda > 0$, we have $p_A(\lambda x) = \lambda p_A(x)$ for $\lambda > 0$. Let $x, y$ be two points of E. If $x$ (resp. $y$) is not absorbed by A then $p_A(x) = +\infty$ (resp. $p_A(y) = +\infty$) and the inequality $p_A(x + y) \leq p_A(x) + p_A(y)$ is obviously true. Suppose there exist $\alpha > 0, \beta > 0$ such that $x \in \alpha A$, and $y \in \beta A$; then $x + y \in \alpha A + \beta A = (\alpha + \beta) A$ (II, p. 8, *Remark*); and thus $p_A(x + y) \leq p_A(x) + p_A(y)$. The inclusion $A \subset V(p_A, 1)$ is clearly true. The inclusion $W(p_A, 1) \subset A$ follows because A is convex and contains 0. Finally if A is absorbent then $p_A$ is obviously finite.

The function $p_A$ defined by (7) is called the *gauge* of the convex set A. If A is absorbent and symmetric, then $p_A$ is a semi-norm.

#### Proposition 23 {#evt-ii-s2-prop-23 .statement}

*Let E be a topological vector space. If A is an open convex set which contains 0, then $p_A$ is finite and continuous, and $A = W(p_A, 1)$. If A is a closed convex set containing 0, then $p_A$ is lower semi-continuous and $A = V(p_A, 1)$.*

If A is open and contains 0, then it is absorbent. For $x \in A$, there exists $\rho < 1$ such that $x / \rho \in A$, and thus $p_A(x) < 1$; this, combined with (9) gives $A = W(p_A, 1)$. Since the convex function $p_A$ is bounded above in the open set A, it is continuous in E (II, p. 18, prop. 21).

Suppose A is closed and contains 0. For every $x \in E$ with $p_A(x) \leq 1$, we have $x \in \rho A$ for all $\rho > 1$, therefore $x \in A$ since A is closed; remembering (9), this shows that $A = V(p_A, 1)$. For all $\mu > 0$, $\mu A$ is therefore the set of $x$ such that $p_A(x) \leq \mu$; as $p_A(x) \geq 0$ in E, this shows that $p_A$ is lower semi-continuous in E (GT, IV, § 6.2).

A positive sublinear function $p$ over E is the gauge of each convex set A where $W(p, 1) \subset A \subset V(p, 1)$.

### Exercises {#evt-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
