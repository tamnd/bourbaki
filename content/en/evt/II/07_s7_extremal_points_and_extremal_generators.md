---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 7
section_title: Extremal points and extremal generators
lang: en
source: evt-i-v
book_pages: TVS II.54-TVS II.60, TVS II.87-TVS II.95
pdf_pages: 0091-0097, 0124-0132
extraction: ocr
subsections:
    - "no": 1
      title: Extremal points of compact convex sets
      page: 54
      pdf_page: 91
    - "no": 2
      title: Extremal generators of convex cones
      page: 57
      pdf_page: 94
    - "no": 3
      title: Convex cones with compact sole
      page: 59
      pdf_page: 96
statements: 25
exercises: 41
content_sha256: ba5544881bc2d551481082f09b14e6852c10e86a0663b8e63d376fbaadf87175
---

## § 7. EXTREMAL POINTS AND EXTREMAL GENERATORS

### 1. Extremal points of compact convex sets

#### Definition 1 {#evt-ii-s7-def-1 .statement}

Let $A$ be a convex set in an affine space $E$. Then we say that a point $x \in A$ is an extremal point of $A$ if there does not exist an open segment that is contained in $A$ and contains $x$.

In other words, the relations $x = \lambda y + (1 - \lambda)z,\ y \in A,\ z \in A,\ y \neq z$ and $0 \leq \lambda \leq 1$ imply $\lambda = 0$ or $\lambda = 1$ (thus $x = y$ or $x = z$). This implies that $x$ cannot be the barycentre of a set of $n$ points $x_i$ of $A$ carrying positive masses unless $x$ is one of the $x_i$; for this is just the definition when $n = 2$; for arbitrary $n$ argue by induction on $n$, as $x$ is the barycentre of $x_1$ and of the barycentre $y_1$ of the $x_i$ with $2 \leq i \leq n$, therefore $x$ is identical with $x_1$ or $y_1$, and in the second case it is sufficient to apply the induction hypothesis.

To say that $x$ is an extremal point of $A$ also means that $A - \{x\}$ is convex.

#### Example 1 {#evt-ii-s7-n1-exa-1 .statement}

In the space $\mathbf{R}^n$, all the points of the sphere $S_{n-1}$ are extremal points of the closed ball $B_n$. For, if $\sum_i y_i^2 \leq 1,\ \sum_i z_i^2 \leq 1$ and $0 < \lambda < 1$, the relation
$$
\lambda^2 \sum_i y_i^2 + (1 - \lambda)^2 \sum_i z_i^2 + 2\lambda(1 - \lambda) \sum_i y_i z_i = 1 = (\lambda + (1 - \lambda))^2
$$
is possible only if
$$
\sum_i y_i^2 = \sum_i z_i^2 = \sum_i y_i z_i = 1.
$$
But this implies $\sum_i (y_i - z_i)^2 = 0$, thus $y_i = z_i$ for all $i$, which proves our assertion.

#### Example 2 {#evt-ii-s7-n1-exa-2 .statement}

In the normed space $\mathcal{B}(\mathbf{N})$ of bounded sequences of real numbers (I, p. 4) the extremal points of the unit ball are the points $x = (\xi_n)$ such that $|\xi_n| = 1$ for all $n$. For, suppose that we had $|\xi_n| \leq 1$ for all $n$ and $|\xi_p| < 1$ for one index $p$. We can then write
$$
x = \frac{1 + \xi_p}{2} y + \frac{1 - \xi_p}{2} z
$$
where $y$ (resp. $z$) is the point all of whose coordinates are equal to the coordinate of $x$ with the same index, except in the case of index $p$ where the coordinate is equal to 1 (resp. $-1$). This shows that $x$ is not extremal, since we have $\|y\| \leq 1$ and $\|z\| \leq 1$. Conversely, if $|\xi_n| = 1$ for all $n$, then $x$ is extremal, for the relation $\xi_n = \lambda \eta_n + (1 - \lambda) \zeta_n$ with $|\eta_n| \leq 1,\ |\zeta_n| \leq 1$ and $0 < \lambda < 1$ implies $\xi_n = \eta_n = \zeta_n$.

#### Example 3 {#evt-ii-s7-n1-exa-3 .statement}

Let $u : E \to E'$ be an affine mapping of an affine space $E$ in an affine space $E'$; let $C \subset E,\ C' \subset E'$ be two convex sets such that $u(C) \subset C'$. If $x'$ is an extremal point of $C'$ and $x$ is an extremal point of $u^{-1}(x') \cap C$, then $x$ is an extremal point of $C$, as it follows from def. 1.

#### Proposition 1 {#evt-ii-s7-prop-1 .statement}

Let $B$ be the set of extremal points of $A$, a non-empty compact convex set in a Hausdorff locally convex space $E$, and let $f$ be a convex function defined in $A$ and upper semi-continuous. Then $f$ attains its upper bound in $A$ at one point (at least) of $B$.

Use $\mathcal{F}$ to denote the family of subsets X of A that are *non-empty, closed, and such that every open segment that is contained in A and meets X necessarily lies in X*. It has the following properties;
(i) A belongs to $\mathcal{F}$.
(ii) A point $a \in A$ is such that $\{a\} \in \mathcal{F}$, if, and only if, $a$ is an extremal point of A.
(iii) Every non-empty intersection X of a family $(X_\alpha)$ of sets of $\mathcal{F}$ also belongs to $\mathcal{F}$.

The properties (i), (ii) and (iii) follow immediately from the definitions.

(iv) Let $X \in \mathcal{F}$, and let $h$ be a function that is convex and upper semi-continuous in A; then the set Y of the points of X where the restriction $h|X$ attains its upper bound in X is such that Y belongs to $\mathcal{F}$.

For, $h|X$ being upper semi-continuous in X attains its upper bound $\alpha$ over X in at least one point of X (GT, IV, § 6.2, th. 3); thus Y is non-empty, it is also closed (GT, IV, § 6.2, prop. 1). On the other hand let $x, y$ be two distinct points of A and let $z = \lambda x + (1 - \lambda) y$ be a point of Y such that $0 < \lambda < 1$; as $Y \subset X$ and $X \in \mathcal{F}$, we have $x \in X$ and $y \in X$; on the other hand, as $h$ is convex, we have

$$
h(z) \leq \lambda h(x) + (1 - \lambda) h(y)
$$

but as $h(x) \leq \alpha, h(y) \leq \alpha$ and $h(z) = \alpha$, of necessity $h(x) = h(y) = \alpha$, that is to say $x \in Y$ and $y \in Y$. Therefore $Y \in \mathcal{F}$.

With these properties established, let M be the set of $x \in A$ where $f$ attains its upper bound in A; by (iv), $M \in \mathcal{F}$. On the other hand, by (iii) and the fact that the sets of $\mathcal{F}$ are closed subsets ot the compact set A, it follows that $\mathcal{F}$ is *inductive* for the order relation $\supset$. By th. 2 of S, III, § 2.4, M contains a subset N which is a minimal element of $\mathcal{F}$. We shall show that N consists of a single point and this will complete the proof of the proposition. Since E is a Hausdorff locally convex space, it is sufficient to show that every continuous linear form $u$ on E is constant in N (II, p. 38, cor. 1). Now it follows from (iv) that the set $N'$ of the $x \in N$ where $u|N$ attains its upper bound in N is such that $N'$ belongs to $\mathcal{F}$; since N is minimal in $\mathcal{F}$ we necessarily have $N' = N$.

#### Corollary {#evt-ii-s7-n1-cor-1 .statement}

*Let A be a compact convex set in a Hausdorff locally convex space E. Then every closed support hyperplane H of A contains at least one extremal point of A.*

For, if $f(x) = \alpha$ is an equation of H and $f(x) \leq \alpha$ in A, it is sufficient to apply prop. 1 to $f$.

#### Theorem 1 (Krein-Milman) {#evt-ii-s7-thm-1 .statement}

— *In a Hausdorff locally convex space E, every compact convex set A is the closed convex envelope of the set of its extremal points.*

For, let C be the closed convex envelope of the set of extremal points of A; clearly $C \subset A$. To see that $A \subset C$, it is sufficient to prove that, if $u$ is an affine linear function, continuous in E and if $u(x) \geq 0$ in C then also $u(x) \geq 0$ in A (II, p. 39, cor. 4); but this follows from prop. 1 applied to $-u$.

#### Proposition 2 {#evt-ii-s7-prop-2 .statement}

*Let x be an extremal point of a compact convex set A in a Hausdorff* locally convex space E. Then for every open neighbourhood V of x in E, there exists an open half-space F in E such that $x \in F \cap A \subset V \cap A$ (in other words, the traces on A of the open half-spaces containing x, form a fundamental system of neighbourhoods of x in A).

For every open half-space D of E containing x, the set $A \cap \overline{D}$ is a compact neighbourhood of x in A, and the intersection of all these neighbourhoods is precisely the point x (any two distinct points can be strictly separated by a closed hyperplane (II, p. 38, prop. 4). By prop. 1 of GT, I, § 9.2, it is sufficient to prove that the sets $A \cap \overline{D}$ form a filter base. Now if we write $L_D = A \cap (E - D)$, the set $L_D$ is convex, compact and contained in the convex set $A - \{x\}$; if $D_1, D_2$ are two open half-spaces of E containing x, the convex envelope B of $L_{D_1} \cup L_{D_2}$ is therefore contained in $A - \{x\}$; but B is a compact set (II, p. 14, prop. 15), therefore there exists a closed hyperplane H that separates x strictly from B (II, p. 38, prop. 4) and if the open half-space determined by H and containing x is D, then we have $L_{D_1} \cup L_{D_2} \subset L_D$, therefore $A \cap \overline{D} \subset (A \cap \overline{D_1}) \cap (A \cap \overline{D_2})$.

#### Corollary {#evt-ii-s7-n1-cor-2 .statement}

— In a Hausdorff locally convex space let K be a compact subset of a compact convex set A. Then the following conditions are equivalent.

a) A is the closed convex envelope of K.

b) K meets every set that is the intersection of A with one of its support hyperplanes.

c) K contains the set of extremal points of A.

a) $\Rightarrow$ b). Suppose that there exists a support hyperplane H of A whose equation is $f(x) = \alpha$, such that $(H \cap A) \cap K = \varnothing$ and suppose, for example, that $f(x) \geq \alpha$ in A. As $f(x) - \alpha > 0$ for all $x \in K$ by hypothesis and as K is compact we have

$$
\beta = \inf_{x \in K} f(x) > \alpha ,
$$

and K is, therefore, contained in the closed half-space $f(x) \geq \beta$; therefore the same is true of the closed convex envelope A of K and this is absurd.

b) $\Rightarrow$ c). Suppose that an extremal point x of A does not belong to K; there is a neighbourhood V of x in E such that $V \cap A \cap K = \varnothing$. But by prop. 2, we can suppose that V is an open half-space defined by a hyperplane H with the equation $f(z) = \alpha$. If for example $f(x) > \alpha$, then for all $y \in K$, we have $f(y) \leq \alpha$, therefore K does not meet the intersection of A and the support hyperplane $f(z) = \gamma > \alpha$ parallel to H (II, p. 37, prop. 2); this is absurd.

c) $\Rightarrow$ a). This is an obvious consequence of the Krein-Milman theorem.

#### Remark 1 {#evt-ii-s7-n1-rem-1 .statement}

Even if the vector space E is finite dimensional the set of extremal points of a compact convex set is not necessarily closed (II, p. 89, exerc. 11).

#### Remark 2 {#evt-ii-s7-n1-rem-2 .statement}

If K is a compact set in a non complete Hausdorff locally convex space, and A, the closed convex envelope of K is not compact, there can be extremal points of A that do not belong to K (II, p. 87, exerc. 2).

#### Remark 3 {#evt-ii-s7-n1-rem-3 .statement}

In a Banach space E of infinite dimension, it may happen that the closed ball of centre 0 and radius 1 does not possess any extremal point (II, p. 89, exerc. 14).

#### Remark 4 {#evt-ii-s7-n1-rem-4 .statement}

If A is a compact convex set in a Hausdorff locally convex space, it may happen that an extremal point of A does not belong to any support hyperplane of A (II, p. 78, exerc. 11). The proof of theorem 1 (II, p. 56) shows that in any case A is the convex closed envelope of the set of extremal points of A which belong to a support hyperplane.

### 2. Extremal generators of convex cones

Let C be a convex cone with vertex 0 in a vector space E; clearly no other point of C than the vertex can be an extremal point; the vertex is an extremal point of C if and only if C is pointed and proper.

#### Definition 2 {#evt-ii-s7-def-2 .statement}

Let C be a convex cone of vertex 0 in a vector space E. We say that a half-line D ⊂ C originating at 0 is an extremal generator of C, if every open segment contained in C, not containing 0 and meeting D is contained in D.

It comes to the same thing to say that for all x ∈ D such that x ≠ 0, if y ≠ 0, y' ≠ 0 are two points of C such that x = y + y', then, it is necessarily the case that y ∈ D and y' ∈ D.

#### Remark 1 {#evt-ii-s7-n2-rem-1 .statement}

Let C be a pointed proper convex cone in E, and consider on E the order structure for which C is the set of elements ≥ 0 (II, p. 12, prop. 13); in order that an element of E, say x > 0, belongs to an extremal generator of C, it is necessary and sufficient that every element y ≥ 0, that is bounded above by x, is of the form λx with 0 ≤ λ ≤ 1 : in fact, to say that y is bounded above by x means that x = y + y' where y' ∈ C, whence the conclusion follows.

#### Proposition 3 {#evt-ii-s7-prop-3 .statement}

In a vector space E, let C be a convex cone with vertex 0, and let x₀ ≠ 0 be a point of C, and D a half-line that is contained in C, originating from 0 and containing x₀. Let H be a hyperplane containing x₀ and not passing through 0. Then D is an extremal generator of C if and only if x₀ is an extremal point of H ∩ C.

The condition is clearly necessary. Conversely, suppose that it is satisfied; suppose that there is a line D' not containing D, passing through x₀ and such that D' ∩ C contains an open segment to which x₀ belongs. Let y ≠ 0 be a direction vector of D'; the hypotheses imply that the point (1 + λ)x₀ + μy belongs to C for |λ| and |μ| sufficiently small. But then, in the plane P determined by D and D' and carrying the canonical topology, x₀ is an interior point of P ∩ C, and it follows that the line P ∩ H contains an open segment contained in H ∩ C and to which x₀ belongs. This contradicts the hypothesis.

#### Definition 3 {#evt-ii-s7-def-3 .statement}

Let C be a convex set in a Hausdorff topological vector space E. A compact convex non-empty set A of C is called a cap of C if the complement C − A of A in C is convex.

Let C be a pointed convex cone with vertex 0 in E and let A be a cap of C. Write B = C − A. For every closed half-line L ⊂ C originating at 0, the sets L ∩ A and L ∩ B are convex sets that are complements in L, whose union is L, and such that L ∩ A is compact. As L ∩ A is non-empty for at least one half-line L, we see that 0 ∈ A, thus L ∩ A is a closed segment with an end point at 0. If A exists then C is proper.

#### Proposition 4 {#evt-ii-s7-prop-4 .statement}

— Let C be a pointed convex cone with vertex 0 in E, a Hausdorff locally convex space.

a) Let A be a cap of C. Let p be the restriction to C of the gauge of A (II, p. 20). The set of the x ∈ C such that p(x) ≤ 1 is the set A. The function p is lower semi-continuous and has the following properties :
(i) For any x, y in C, we have p(x + y) = p(x) + p(y).
(ii) For any x ∈ C and λ ∈ R_+^*, we have p(λx) = λp(x).
(iii) If x ∈ C, the relation p(x) = 0 is equivalent to x = 0.

b) Conversely, let p be a function defined in C with values in [0, +∞], satisfying the conditions (i), (ii) of a). Let A be the set of the x ∈ C such that p(x) ≤ 1. Then A and C − A are convex. A is a cap, if and only if A is compact and non-empty.

The statement b) is obvious. The properties stated in a) are consequences of the remarks preceding prop. 4 and of the prop. 22 of II, p. 20 and prop. 23 of II, p. 20 with the exception of

$$
p(x + y) \geq p(x) + p(y).
$$

It is sufficient to prove this last when x ≠ 0 and y ≠ 0; we have therefore p(x) > 0, p(y) > 0. Let μ, λ be two numbers > 0 such that λ < p(x), μ < p(y), and denote the complement of A in C by B. We have x ∈ λB, y ∈ μB, therefore x + y ∈ λB + μB; by the convexity of B, we have λB + μB ⊂ (λ + μ)B, whence p(x + y) > λ + μ, which implies the inequality stated above.

#### Corollary 1 {#evt-ii-s7-prop-4-cor-1 .statement}

— Let C be a pointed convex cone of vertex 0 in E, a Hausdorff locally convex space and let p be the gauge of A, a cap of C. The extremal points of A are then the point 0, and the points x on the extremal generators of C such that p(x) = 1.

It is clear that 0 is an extremal point of A. Let x be a point on L an extremal generator of C and such that p(x) = 1. Let y, z be two points of A such that x = $\frac{1}{2}(y + z)$. As L is extremal, we have y = λx and z = μx, where λ and μ are numbers ≥ 0 such that $\frac{1}{2}(\lambda + \mu) = 1$, $\lambda = \lambda p(x) = p(y) \leq 1$ and $\mu = \mu p(x) = p(z) \leq 1$, from which $\lambda = \mu = 1$ and hence y = z = x; so, x is an extremal point of A. Conversely, let x ≠ 0 be an extremal point of A. Obviously p(x) = 1. Let y, y' be two points of C such that x = y + y', and we shall show that y, y' are proportional to x. Without loss of generality we can suppose that the numbers $\lambda = p(y)$ and $\lambda' = p(y')$ are finite and > 0. Then $\lambda^{-1}y \in A, {\lambda'}^{-1}y' \in A, \lambda + \lambda' = 1$ by prop. 4, (i) and the equality $x = \lambda(\lambda^{-1}y) + \lambda'({\lambda'}^{-1}y')$ implies, by hypothesis that

$$
x = \lambda^{-1}y = {\lambda'}^{-1}y'.
$$

#### Corollary 2 {#evt-ii-s7-prop-4-cor-2 .statement}

— Every point of C that belongs to a cap of C, also belongs to the convex closed envelope of the union of the extremal generators of C.

This follows immediately from cor. 1 and the Krein-Milman theorem (II, p. 55, th. 1).

\* Example. — Let X be a locally compact space that is σ-compact. Let C be a closed convex cone of vertex 0 in $\mathcal{M}_+(X)$ with the vague topology. We shall show that C is the union of its caps. Let $(X_n)$ be an increasing sequence of open, relatively compact sets of X whose union is X. Let μ be an element $\neq 0$ of C. There exist $\alpha_n > 0$ such that $\sum_n \alpha_n \mu(X_n) = 1$.

For every measure $v \in C$, put $p(v) = \sum_n \alpha_n v(X_n) \in [0, +\infty]$. The function p on C satisfies conditions (i) and (ii) of prop. 4. It is lower semi-continuous for the vague topology (INT, IV, 2nd ed., § 1, No. 1, prop. 4). The set A of the $\gamma \in C$ such that $p(\gamma) \leq 1$ is therefore closed and non-empty. On the other hand, every compact set of X is contained in one of the $X_n$, thus A being vaguely bounded is also vaguely compact (INT, III, 2nd ed., § 1, No. 9, prop. 15). The set A is therefore a cap of C containing μ. \*

#### Proposition 5 {#evt-ii-s7-prop-5 .statement}

Let C be a proper convex cone with vertex 0 in E, a Hausdorff weak space; suppose that C is complete for the uniform structure induced by that of E, and that there is an enumerable fundamental system of neighbourhoods of 0 in C. Then C is the union of its caps and is the closed convex envelope of the union of its extremal generators.

The second statement follows from the first and from cor. 2 above. Using prop. 11 of II, p. 52 reduces the proposition to the case when $E = \mathbf{R}^l$ and $C \subset \mathbf{R}_+^l$. For all $\alpha \in I$, denote the projection $pr_\alpha$ in E by $f_\alpha$; then $f_\alpha$ is a continuous linear form. On the other hand let $(V_n)_{n \in \mathbf{N}}$ be an enumerable fundamental system of neighbourhoods of 0 in C. By the definition of the topology of E, for each $n \in \mathbf{N}$, there exists a finite subset $J_n$ of I and a number $\varepsilon_n > 0$ such that $V_n$ contains the set $W_n$ of the $x \in C$ such that $f_\alpha(x) \leq \varepsilon_n$ for all $\alpha \in J_n$; put $J = \bigcup_{n \in \mathbf{N}} J_n$. Let $y \neq 0$ be a point of C, and p be the function $\sum_{\alpha \in J} \lambda_\alpha (f_\alpha|C)$ where the $\lambda_\alpha > 0$ are chosen so that $p(y) = 1$; this is possible, since if $f_\alpha(y) = 0$ for all $\alpha \in J$, then $y \in V_n$ for all $n$, which implies that $y = 0$, and this is contrary to hypothesis. Now we remark that for all $\alpha \in I$, the function $f_\alpha|C$ is continuous at the point 0, therefore there is an $n \in \mathbf{N}$, such that $f_\alpha$ is bounded in a $W_n$, therefore bounded above in C by a linear combination of a finite number of functions $f_\beta|C$, where $\beta \in J$. It follows that if A in the set of $x \in C$ such that $p(x) \leq 1$, then $f_\alpha$ is bounded in A for all $\alpha \in I$. As p is lower semi-continuous in C, it follows that A is closed and non-empty in C and therefore is compact. Since it is clear that p verifies the conditions (i) and (ii) of prop. 4 of II, p. 58, we see that A is a cap in C and contains y.

#### Remark 2 {#evt-ii-s7-n2-rem-2 .statement}

There exist proper convex cones that are weakly complete and which have no extremal generator (II, p. 92, exerc. 31).

### 3. Convex cones with compact sole

#### Proposition 6 {#evt-ii-s7-prop-6 .statement}

Let E be a Hausdorff locally convex space and K a convex compact set in E which does not contain 0. Then the smallest pointed cone C of vertex 0 which contains $K$ is a proper convex cone in $E$ and is a locally compact and complete subspace of $E$; also, there exists a closed hyperplane $H$ in $E$ that does not contain 0 and is such that $H$ meets all the half-lines originating at 0 contained in $C$ and such that $H \cap C$ is compact. Further, if $D$ is the half-space containing 0 determined by $H$, a closed hyperplane with these properties, then $C \cap D$ is a cap of $C$ and $C$ is the union of the $\lambda(C \cap D)$ for $\lambda > 0$.

By prop. 4 of II, p. 38, there exists a closed hyperplane $H$ which separates 0 strictly from $K$. Now, the convex envelope $A$ of the union of $\{0\}$ and of $K$ is compact (II, p. 14, prop. 15) and is the union of the $\lambda K$ with $0 \leq \lambda \leq 1$. As 0 and $K$ are strictly on opposite sides of $H$, for every $x \in K$ there exists $\lambda$ such that $0 < \lambda < 1$ and $\lambda x \in H$. As $C$ is the union of the $\lambda A$ for $\lambda \geq 1$, we see that $H$ meets every half-line originating at 0 contained in $C$ and that $H \cap A = H \cap C$ is compact. Further, $C$ is also the union of the $\lambda(H \cap C)$ for $\lambda \geq 0$; let $C_n$ be the union of the $\lambda(H \cap C)$ for $0 \leq \lambda \leq n$. Clearly $C_n$ is the convex envelope of the union of $\{0\}$ and of $n(H \cap C)$, therefore it is compact. Also, for all $x \in E$, there is a closed neighbourhood $V$ of $x$ in $E$ and an integer $n$ such that $V \cap C \subset C_n$; in fact, if $H$ is defined by the equation $f(z) = \alpha$, where $\alpha > 0$, it is sufficient to take for $V$ the closed half-space determined by $nH$ and containing 0, where $n$ is so large that $n\alpha > f(x)$. This shows that $C$ is locally compact (taking $x \in C$), and that it is closed in $E$. We can also consider $K$ as a subset of the completion $\hat{E}$, therefore $C$ is also closed in $\hat{E}$ and therefore complete.

Given a cone $C$ and a closed hyperplane $H$ in a Hausdorff topological vector space $E$, such that $H$ does not contain the vertex $s$ of $C$ and $C$ is the smallest cone with vertex $s$ containing $H \cap C$, then we call the intersection $H \cap C$ a « sole » of the cone $C$. Prop. 6 shows that in a Hausdorff locally convex space $E$, the smallest cone of vertex 0, containing a compact convex set $K$ to which 0 does not belong, is a cone of compact sole, and that every convex cone having a compact sole $S$, is locally compact and complete.

#### Example 1 {#evt-ii-s7-n3-exa-1 .statement}

Every proper closed convex cone in $E$, a vector space of finite dimension, has a compact sole. In fact, by II, p. 52, prop. 11 we need only consider the case where $E = \mathbf{R}^n$ and $C = \mathbf{R}_+^n$. If $(e_i)_{1 \leq i \leq n}$ is the canonical basis of $\mathbf{R}^n$, it is clear that the compact convex set which is the convex envelope of the $e_i$ ($1 \leq i \leq n$) is a compact sole for $\mathbf{R}_+^n$.

#### Example 2 {#evt-ii-s7-n3-exa-2 .statement}

If $X$ is a compact space, then the cone $\mathcal{M}_+(X)$ of positive measures on $X$, with the vague topology, is a cone with a compact sole (INT, III, 2nd ed., § 1, No. 9, cor. 3 of prop. 15). \*

### Exercises {#evt-ii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
