---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 3
section_title: Complete spaces
lang: en
source: top-i-iv
book_pages: 181-198, 208-209
pdf_pages: 0187-0204, 0214-0215
extraction: ocr
subsections:
    - "no": 1
      title: CAUCHY FILTERS
      page: 181
      pdf_page: 187
    - "no": 2
      title: MINIMAL CAUCHY FILTERS
      page: 183
      pdf_page: 189
    - "no": 3
      title: COMPLETE SPACES
      page: 184
      pdf_page: 190
    - "no": 4
      title: SUBSPACES OF COMPLETE SPACES
      page: 186
      pdf_page: 192
    - "no": 5
      title: PRODUCTS AND INVERSE LIMITS OF COMPLETE SPACES
      page: 186
      pdf_page: 192
    - "no": 6
      title: EXTENSION OF UNIFORMLY CONTINUOUS FUNCTIONS
      page: 190
      pdf_page: 196
    - "no": 7
      title: THE COMPLETION OF A UNIFORM SPACE
      page: 191
      pdf_page: 197
    - "no": 8
      title: THE HAUSDORFF UNIFORM SPACE ASSOCIATED WITH A UNIFORM SPACE
      page: 196
      pdf_page: 202
    - "no": 9
      title: COMPLETION OF SUBSPACES AND PRODUCT SPACES
      page: 197
      pdf_page: 203
statements: 48
exercises: 7
content_sha256: d782c4a27c7dfb328d8d4bcb0a0fc179bed02b77ea87afcfdc15ece558d53cbb
---

## 3. COMPLETE SPACES

### 1. CAUCHY FILTERS

Once a set $X$ has been endowed with a uniform structure we can define what is meant by a "small" subset of $X$ (relative to this structure): a "small" subset of $X$ is one in which all the points are "very close" to each other. Precisely:

#### Definition 1 {#top-ii-s3-def-1 .statement}

If $X$ is a uniform space and if $V$ is an entourage of $X$, a subset $A$ of $X$ is said to be $V$-small if every pair of points of $A$ are $V$-close (in other words, if $A \times A \subset V$).

#### Proposition 1 {#top-ii-s3-prop-1 .statement}

In a uniform space $X$, if two sets $A$ and $B$ are $V$-small and intersect, then their union $A \cup B$ is $\vec{V}$-small.

Let $x$ and $y$ be any two points of $A \cup B$, and let $Z \in A \cap B$. Then $(x, z) \in V$ and $(z, y) \in V$, so that $(x, y) \in \overline{V}$.

#### Definition 2 {#top-ii-s3-def-2 .statement}

*A filter $\mathcal{F}$ on a uniform space $X$ is a Cauchy filter if for each entourage $V$ of $X$ there is a subset of $X$ which is $V$-small and belongs to $\mathcal{F}$.*

Here again we may make our language more expressive by the use of the expressions "sufficiently small set" and "a set as small as we please"; thus Definition 2 can be restated by saying that a Cauchy filter is one containing *arbitrarily small sets*.

An infinite sequence $(u_n)$ of points of a uniform space $X$ is said to be a *Cauchy sequence* if the elementary filter associated with the sequence is a Cauchy filter. It comes to the same thing to say that for each entourage $V$ of $X$ there is an integer $n_0$ such that for all integers $m \geq n_0$ and $n \geq n_0$ we have $(u_m, u_n) \in V$.

#### Proposition 2 {#top-ii-s3-prop-2 .statement}

*On a uniform space $X$ every convergent filter is a Cauchy filter.*

If $x$ is any point of $X$ and $V$ is any symmetric entourage of $X$, then the neighbourhood $V(x)$ of $x$ is $\overline{V}$-small. If $\mathcal{F}$ is a filter which converges to $x$, there is a set of $\mathcal{F}$ contained in $V(x)$, and therefore $V$-small.

Clearly every filter which is *finer* than a Cauchy filter is a Cauchy filter.

#### Proposition 3 {#top-ii-s3-prop-3 .statement}

*Let $f : X \to X'$ be a uniformly continuous mapping. Then the image under $f$ of a Cauchy filter base on $X$ is a Cauchy filter base on $X'$.*

Let $g = f \times f$. If $V'$ is an entourage of $X'$, then $\overline{g^{-1}(V')}$ is an entourage of $X$, and the image under $f$ of a $\overline{g^{-1}(V')}$-small set is $V'$-small; hence the result.

It follows in particular that if the uniformity of a uniform space $X$ is replaced by a *coarser* uniformity, then every Cauchy filter with respect to the original uniformity remains a Cauchy filter with respect to the new uniformity.

This fact can be easily remembered in the following form: *the finer the uniformity, the fewer Cauchy filters there are*.

#### Proposition 4 {#top-ii-s3-prop-4 .statement}

*Let $X$ be a set, let $(Y_i)_{i \in I}$ be a family of uniform spaces, and for each $i \in I$ let $f_i$ be a mapping of $X$ into $Y_i$. Let $X$ carry the coarsest uniformity $U$ for which the $f_i$ are uniformly continuous. Then in order that a filter base $\mathcal{B}$ on $X$ should be a Cauchy filter base it is necessary and sufficient that $f_i(\mathcal{B})$ should be a Cauchy filter base on $Y_i$, for each $i \in I$.*

The condition is necessary by Proposition 3. Conversely, suppose that it is satisfied, and let $U(V_{i_1}, \ldots, V_{i_n})$ be an entourage of the uniformity $\mathcal{U}$ [§ 2, no. 3, formula (1)]. By hypothesis, for each index $k$ there is a set $M_k \in \mathcal{B}$ such that $f_{i_k}(M_k)$ is $V_{i_k}$-small ($1 \leq k \leq n$). Let $M$ be a set of $\mathcal{B}$ contained in $M_k$ for $1 \leq k \leq n$; then for each pair of points $x, x'$ of $M$ we have $[f_{i_k}(x), f_{i_k}(x')] \in V_{i_k}$ for $1 \leq k \leq n$, so that
$$
(x, x') \in U(V_{i_1}, \ldots, V_{i_n}).
$$
This completes the proof.

#### Corollary 1 {#top-ii-s3-prop-4-cor-1 .statement}

*If a Cauchy filter on a uniform space $X$ induces a filter on a subset $A$ of $X$, then this filter is a Cauchy filter on the uniform subspace $A$.*

#### Corollary 2 {#top-ii-s3-prop-4-cor-2 .statement}

*A filter base $\mathcal{B}$ on a product $\prod_{i \in I} X_i$ of uniform spaces is a Cauchy filter base if and only if, for each $i \in I$, $\operatorname{pr}_i(\mathcal{B})$ is a Cauchy filter base on $X_i$.*

### 2. MINIMAL CAUCHY FILTERS

The minimal elements (with respect to inclusion) of the set of Cauchy filters on a uniform space $X$ are called *minimal Cauchy filters* on $X$.

#### Proposition 5 {#top-ii-s3-prop-5 .statement}

*Let $X$ be a uniform space. For each Cauchy filter $\mathfrak{F}$ on $X$ there is a unique minimal Cauchy filter $\mathfrak{F}_0$ coarser than $\mathfrak{F}$. If $\mathcal{B}$ is a base of $\mathfrak{F}$ and $\mathcal{G}$ is a fundamental system of symmetric entourages of $X$, then the sets $V(M)$ ($M \in \mathcal{B}, V \in \mathcal{G}$) form a base of $\mathfrak{F}_0$.

If $M, M'$ are in $\mathcal{B}$ and $V, V'$ are in $\mathcal{G}$, then there is a set $M'' \in \mathcal{B}$ (resp. $V'' \in \mathcal{G}$) such that $M'' \subset M \cap M'$ (resp. $V'' \subset V \cap V'$); hence $V''(M'') \subset V(M) \cap V'(M')$ and therefore the sets $V(M)$ ($M \in \mathcal{B}, V \in \mathcal{G}$) indeed form a base of a filter $\mathfrak{F}_0$ on $X$. Further, if $M$ is $V$-small, then $V(M)$ is $V$-small; hence $\mathfrak{F}_0$ is a Cauchy filter and is clearly coarser than $\mathfrak{F}$. To complete the proof it is enough to show that if $\mathfrak{G}$ is a Cauchy filter coarser than $\mathfrak{F}$, then $\mathfrak{G}$ is finer than $\mathfrak{F}_0$. For each $M \in \mathcal{B}$ and each $V \in \mathcal{G}$ there is a set $N \in \mathcal{G}$ which is $V$-small; since $N \in \mathfrak{F}$, $N$ meets $M$; hence $N \subset V(M)$ and so $V(M) \in \mathfrak{G}$.

#### Corollary 1 {#top-ii-s3-prop-5-cor-1 .statement}

*For each $x \in X$, the neighbourhood filter $\mathcal{B}(x)$ of $x$ in $X$ is a minimal Cauchy filter.*

Take $\mathfrak{F}$ in Proposition 5 to be the filter of all subsets of $X$ which contain $x$, and take $\mathcal{B}$ to consist of the single element $\{x\}$.

#### Corollary 2 {#top-ii-s3-prop-5-cor-2 .statement}

*Every cluster point* $x$ *of a Cauchy filter* $\mathfrak{F}$ *is a limit point of* $\mathfrak{F}$.

There is a filter $\mathcal{G}$ which is finer than both $\mathfrak{F}$ and $\mathcal{B}(x)$ (Chapter I, § 7, no. 2, Proposition 4); since $\mathfrak{F}$ is a Cauchy filter, so is $\mathcal{G}$. If $\mathfrak{F}_0$ is the unique minimal Cauchy filter coarser than $\mathfrak{F}$, then both $\mathfrak{F}_0$ and $\mathcal{B}(x)$ are minimal Cauchy filters coarser than $\mathcal{G}$. Hence $\mathfrak{F}_0 = \mathcal{B}(x)$, which shows that $\mathfrak{F}$ converges to $x$.

#### Corollary 3 {#top-ii-s3-prop-5-cor-3 .statement}

*Every Cauchy filter, which is coarser than a filter converging to a point* $x$, *also converges to* $x$.

This is a consequence of Corollary 2.

#### Corollary 4 {#top-ii-s3-prop-5-cor-4 .statement}

*If* $\mathfrak{F}$ *is a minimal Cauchy filter, then every set of* $\mathfrak{F}$ *has a non-empty interior which also belongs to* $\mathfrak{F}$ *(in other words, $\mathfrak{F}$ has a base consisting of open sets)*.

Let $V$ be any entourage of $X$; then there is an open entourage $U \subset V$ ($\S$ 1, no. 2, Corollary 2 to Proposition 2). For each subset $M$ of $X$, $U(M)$ is open and contained in $V(M)$; hence the result, in view of Proposition 5.

### 3. COMPLETE SPACES

In a uniform space $X$, *a Cauchy filter need not have a limit point*.

#### Example 1 {#top-ii-s3-n3-exa-1 .statement}

Consider the sequence $(u_n)$ on the rational line $\mathbf{Q}$ defined by $u_n = \sum_{p=0}^n 2^{-p(p+1)/2}$. If $m > n$ we have
$$
|u_m - u_n| \leq 2^{-n(n+3)/2}
$$
and therefore $(u_n)$ is a *Cauchy sequence*. But this sequence has no limit in $\mathbf{Q}$; for if the rational number $a/b$ were a limit of $(u_n)$, then by (1) we should have for all $n$
$$
|a/b - h_n/2^{n(n+1)/2}| \leq 1/2^{n(n+3)/2}
$$
where $h_n$ is an integer (depending on $n$); that is,
$$
|a \cdot 2^{n(n+1)/2} - b h_n| \leq b \cdot 2^{-n}
$$
for all $n$. Now the left-hand side of this inequality is an integer for all $n$, and must therefore be zero whenever $n$ is greater than an integer $n_0$ such that $b < 2^{n_0}$; we should therefore have $a/b = u_n$ for all $n > n_0$, which is absurd.

#### Example 2 {#top-ii-s3-n3-exa-2 .statement}

Let $X$ be an infinite set, and consider the uniformity of finite partitions on $X$ ($\S$ 2, no. 2, Remark 1). Every *ultrafilter* $\mathfrak{F}$ on $X$ is a

Cauchy filter with respect to this uniformity. For if $(A_i)$ is a finite partition of $X$ and
$$
V = \bigcup_i (A_i \times A_i)
$$
the corresponding entourage, then at least one of the $A_i$ belongs to $\mathcal{F}$ (Chapter I, § 6, no. 4, Corollary to Proposition 5), and $A_i$ is V-small. On the other hand, $X$ is an infinite discrete space, hence is not compact, and consequently there are ultrafilters on $X$ which do not converge.

#### Definition 3 {#top-ii-s3-def-3 .statement}

*A complete space is a uniform space in which every Cauchy filter converges.*

In a complete space every *Cauchy sequence* (no. 1) is therefore convergent.

#### Example {#top-ii-s3-n3-exa-3 .statement}

On a *discrete* uniform space $X$ a Cauchy filter is a trivial ultrafilter (Chapter I, § 6, no. 4), hence convergent; consequently, $X$ is complete.

From Definitions 2 and 3 of no. 1 and Proposition 2 of no. 1, we deduce the following proposition, known as *Cauchy’s criterion*:

#### Proposition 6 {#top-ii-s3-prop-6 .statement}

*Let $\mathcal{F}$ be a filter on a set $X$, and let $f$ be a mapping of $X$ into a complete uniform space $X'$. Then $f$ has a limit with respect to $\mathcal{F}$ if and only if the image of $\mathcal{F}$ under $f$ is a Cauchy filter base.*

This criterion shows the importance of complete spaces in all questions involving the notion of limit: if a function takes its values in a complete space we can prove the *existence* of a limit *without knowing in advance the value of the limit*; this would be impossible if the definition of limit were the only criterion of convergence at our disposal.

A uniformity which is *finer* than the uniformity of a complete space need not be a uniformity of a complete space (Exercise 2). However, we have the following proposition:

#### Proposition 7 {#top-ii-s3-prop-7 .statement}

*Let $\mathcal{U}_1, \mathcal{U}_2$ be two uniformities on a set $X$, and let $\mathcal{T}_1, \mathcal{T}_2$ be the topologies induced by these uniformities respectively. Suppose that $\mathcal{U}_1$ is finer than $\mathcal{U}_2$, and that there is a fundamental system of entourages for $\mathcal{U}_1$ which are closed in $X \times X$ in the topology $\mathcal{T}_2 \times \mathcal{T}_2$. Then a filter $\mathcal{F}$ on $X$ converges in the topology $\mathcal{T}_1$ if and only if it is a Cauchy filter in the uniformity $\mathcal{U}_1$ and converges in the topology $\mathcal{T}_2$.*

The conditions are clearly necessary, because $\mathcal{T}_2$ is coarser than $\mathcal{T}_1$. Conversely, suppose that the conditions are satisfied, and let $x$ be a limit point of $\mathcal{F}$ with respect to $\mathcal{T}_2$; we shall show that $x$ is a limit of $\mathcal{F}$ with respect to $\mathcal{T}_1$. Let $V$ be a symmetric entourage of $\mathcal{U}_1$ which is closed in the topology $\mathcal{T}_2 \times \mathcal{T}_2$. By hypothesis, $\mathcal{F}$ contains a set $M$ which is V-small; hence if $x' \in M$ we have $M \subset V(x')$. But $V(x')$ is closed in the topology $\mathcal{T}_2$; hence $x$, which lies in the closure of $M$ with respect to $\mathcal{T}_2$, must belong to $V(x')$. It follows that $M \subset \hat{V}(x)$, and the proposition is proved.

#### Corollary {#top-ii-s3-n3-cor-1 .statement}

In the conditions of Proposition 7, if $U_2$ is a uniformity of a complete space, then so is $U_1$.

For every Cauchy filter with respect to $U_1$ is then a Cauchy filter with respect to $U_2$ and therefore converges in the topology $\mathcal{T}_2$.

Note that the hypotheses of the Corollary to Proposition 7 are satisfied when $\mathcal{T}_1 = \mathcal{T}_2$ (§ 1, no. 2, Corollary 2 to Proposition 2).

### 4. SUBSPACES OF COMPLETE SPACES

#### Proposition 8 {#top-ii-s3-prop-8 .statement}

Every closed subspace of a complete space is complete. Every complete subspace of a Hausdorff uniform space (complete or not) is closed.

Let $X$ be a complete space and let $A$ be a closed subspace of $X$. If $\mathfrak{F}$ is a Cauchy filter on $A$, then it is a Cauchy filter base on $X$ (no. 1, Proposition 3) and therefore converges to a point $x \in X$; but since $A$ is closed we have $x \in A$, and therefore $\mathfrak{F}$ converges in the subspace $A$.

Now let $\overline{A}$ be a non-closed subset of a Hausdorff uniform space $X$, and let $b \in \overline{A} - A$. The trace $\mathfrak{B}_A$ on $A$ of the neighbourhood filter $\mathfrak{B}$ of $b$ in $X$ is a Cauchy filter on $A$; but it cannot converge to a point $c \in A$, otherwise $c$ would be a limit point of $\mathfrak{B}$ (no. 2, Proposition 5, Corollary 3) which is absurd since $b \neq c$ and $X$ is Hausdorff.

#### Proposition 9 {#top-ii-s3-prop-9 .statement}

Let $X$ be a uniform space and let $A$ be a dense subset of $X$ such that every Cauchy filter base on $A$ converges in $X$. Then $X$ is complete.

It is enough to show that every minimal Cauchy filter $\mathfrak{F}$ on $X$ is convergent. Since $A$ is dense and since every set of $\mathfrak{F}$ has a non-empty interior (no. 2, Corollary 4 to Proposition 5), the trace $\mathfrak{F}_A$ of $\mathfrak{F}$ on $A$ is a Cauchy filter on $A$, hence converges to a point $x_0 \in X$. Since $\mathfrak{F}$ is coarser than the filter on $X$ generated by $\mathfrak{F}_A$, it follows that $\mathfrak{F}$ converges to $x_0$ (no. 2, Corollary 3 to Proposition 5).

### 5. PRODUCTS AND INVERSE LIMITS OF COMPLETE SPACES

#### Proposition 10 {#top-ii-s3-prop-10 .statement}

Every product of complete uniform spaces is complete. Conversely, if a product of non-empty uniform spaces is complete, then each of the factors is a complete uniform space.

The first assertion is a consequence of the characterization of Cauchy filters and convergent filters on a product space (no. 1, Corollary 2 to Proposition 4 and Chapter I, § 7, no. 6, Corollary 1 to Proposition 10). Conversely, suppose

$$
X = \prod_{i \in I} X_i
$$

is complete (the $X_i$ being non-empty) and let $\mathfrak{F}_x$ be a Cauchy filter on $X_x$. For each $i \neq x$ let $\mathfrak{F}_i$ be a Cauchy filter on $X_i$, and consider the product filter (Chapter I, § 6, no. 7)

$$
\mathfrak{F} = \prod_{i \in I} \mathfrak{F}_i \text{ on } X;
$$

$\mathfrak{F}$ is a Cauchy filter (no. 1, Corollary 2 to Proposition 4), hence is convergent, and therefore so is each $\operatorname{pr}_x \mathfrak{F} = \mathfrak{F}_x$ (Chapter I, § 7, no. 6, Corollary 1 to Proposition 10).

#### Corollary {#top-ii-s3-n5-cor-1 .statement}

*Let* $(X_\alpha, f_{\alpha\beta})$ *be an inverse system of uniform spaces.* *If the* $X_\alpha$ *are Hausdorff and complete, then so is* $X = \varprojlim X_\alpha$.

For $X$ is Hausdorff and can be identified with a *closed* subspace of $\prod_{i \in I} X_\alpha$ (Chapter I, § 8, no. 2, Corollary 2 to Proposition 7); the corollary therefore follows from Proposition 10 and Proposition 8 (no. 4).

An inverse limit of complete Hausdorff uniform spaces $X_\alpha$ can be *empty*, even if all the $X_\alpha$ are non-empty and all the $f_{\alpha\beta}$ are surjective, as is shown by the case of discrete spaces (*Set Theory*, Chapter III, § 1, Exercise 32). However, we have the following theorem:

#### Theorem 1 (Mittag-Leffler) {#top-ii-s3-thm-1 .statement}

*Let* $(X_\alpha, f_{\alpha\beta})$ *be an inverse system of complete Hausdorff uniform spaces, indexed by a directed set* $I$ *which has a countable cofinal subset; suppose also that, for each* $\alpha \in I$, $X_\alpha$ *has a countable fundamental system of entourages* (*). *Finally, suppose that for each* $\alpha \in I$ *there is an index* $\beta \geq \alpha$ *satisfying the following condition*:

(ML$_{\alpha\beta}$) *For each* $\gamma \geq \beta$, $f_{\alpha\gamma}(X_\gamma)$ *is dense in* $f_{\alpha\beta}(X_\beta)$.

*Let* $X = \varprojlim X_\alpha$ *and let* $f_\alpha$ *be the canonical mapping* $X \to X_\alpha$. *Then for each* $\alpha \in I$ *and each* $\beta \geq \alpha$ *satisfying* (ML$_{\alpha\beta}$), $f_\alpha(X)$ *is dense in* $f_{\alpha\beta}(X_\beta)$ *(and consequently* $X$ *is non-empty if the* $X_\alpha$ *are all non-empty)*.

Let $(\lambda_n)$ be a sequence of indices cofinal in $I$. Start with an index $\alpha_0 \in I$ and define recursively an increasing sequence $(\alpha_n)$ such that $\alpha_n \geq \lambda_n$ and such that (ML$_{\alpha_n, \alpha_{n+1}}$) is true. Clearly the sequence

(*) *This condition signifies that the Hausdorff uniform space* $X_\alpha$ *is metrizable; cf. Chapter IX, § 2, no. 4, Theorem 1.*

(α_n) is cofinal in I. We shall write f_{mn} in place of f_{α_mα_n} for m ≤ n, and we shall put f_{n, n+1}(X_{α_{n+1}}) = Y_n. Then, if m ≤ n, f_{mn}(Y_n) is dense in Y_m; for by definition f_{m, n+1}(X_{α_{n+1}}) is dense in

f_{m, m+1}(X_{α_{m+1}}) = Y_m, and f_{m, n+1}(X_{α_{n+1}}) = f_{mn}[f_{n, n+1}(X_{α_{n+1}})] = f_{mn}(Y_n).

By induction on n and k we can define a fundamental system (V_{kn})_{k∈\mathbf{N}} of closed symmetric entourages of X_{α_n} for each n such that

(2)
$\overset{2}{V}_{k+1, n} \subset V_{kn}$,

(3)
$(f_{n, n+1} \times f_{n, n+1})(V_{k, n+1}) \subset V_{kn}$.

In effect, let (U_{kn})_{k∈\mathbf{N}} be a fundamental system of entourages of X_{α_n}. If we suppose that the V_{kn} have been defined for a given n and for all k ∈ \mathbf{N}, then since f_{n, n+1} is uniformly continuous we can define the entourage V_{k, n+1} by induction on k so that (3) is satisfied and

$\overset{2}{V}_{k+1, n+1} \subset V_{k, n+1} ∩ U_{k+1, n+1}$

The assertion follows.

Now let x_0 ∈ Y_0. We shall show that for each integer k > 0 there is a point z ∈ X such that [x_0, f_{α_0}(z)] ∈ V_{k-1, 0}; this will prove the theorem. Since f_{n, n+1} (Y_{n+1}) is dense in Y_n, we can define by induction a sequence of points x_n ∈ Y_n such that

(4)
$$ [x_n, f_{n, n+1}(x_{n+1})] ∈ V_{k+n, n} $$

By reason of (3) it follows that if m ≤ n then

(5)
$$ [f_{mn}(x_n), f_{m, n+1}(x_{n+1})] ∈ V_{k+n, m} $$

From this we conclude that for fixed m the sequence (f_{mn}(x_n))_{n≥m} is a Cauchy sequence in X_{α_m} and therefore converges to a point z_m; for by induction it follows from (5) that, for each pair of integers p ≥ m, q > 0, we have

(6)
$$ [f_{mp}(x_p), f_{m, p+q}(x_{p+q})] ∈ V_{k+p+q-1, m} ∘ V_{k+p+q-2, m} ∘ ... ∘ V_{k+p, m} $$

and by virtue of (2) it is clear that the right-hand side of (6) is contained in V_{k+p-1, m}. Let q increase indefinitely; we infer in particular that, for m = p = 0, we have (x_0, z_0) ∈ V_{k-1, 0}, since V_{k-1, 0} is closed. On the other hand, from the relations z_m = \lim_{n→∞} f_{mn}(x_n) and from the continuity of f_{m, m+1}, we deduce that f_{m, m+1}(z_{m+1}) = z_m for each m ≥ 0. For each γ ∈ I there is at least one integer n such that α_n ≥ γ; putting $z_\gamma = f_{\gamma, \alpha_n}(z_n)$ we verify immediately that $z_\gamma$ does not depend on the value of $n$ such that $\alpha_n \geq \gamma$, and that the family $(z_\alpha)_{\alpha \in I}$ so defined is a point $z$ of $X = \varprojlim X_\alpha$. Since $f_{\alpha_0}(z) = z_0$, the proof is complete.

#### Corollary 1 {#top-ii-s3-thm-1-cor-1 .statement}

*Let* $(X_\alpha, f_{\alpha \beta})$ *be an inverse system of sets indexed by a directed set* $I$ *which has a countable cofinal subset, and suppose that the* $f_{\alpha \beta}$ *are surjective. Then if* $X = \varprojlim X_\alpha$, *the canonical mapping* $f_\alpha : X \to X_\alpha$ *is surjective for each* $\alpha \in I$.

Let each $X_\alpha$ carry the discrete uniformity, and apply Theorem 1.

#### Corollary 2 {#top-ii-s3-thm-1-cor-2 .statement}

*Let* $I$ *be a directed set which has a countable cofinal subset. Let* $(X_\alpha, f_{\alpha \beta})$ *and* $(X'_\alpha, f'_{\alpha \beta})$ *be two inverse systems of sets indexed by* $I$, *and for each* $\alpha \in I$ *let* $u_\alpha : X_\alpha \to X'_\alpha$ *be a mapping, such that the* $u_\alpha$ *form an inverse system of mappings. Let* $u = \varprojlim u_\alpha$. *Let* $x = (x'_\alpha)$ *be an element of*

$$
X' = \varprojlim X'_\alpha
$$

*which satisfies the following condition: for each* $\alpha \in I$ *there is an index* $\beta \geq \alpha$ *such that for all* $\gamma \geq \beta$ *we have* $f_{\alpha \gamma}(\overline{u}_\gamma^{-1}(x_\gamma)) = f_{\alpha \beta}(\overline{u}_\beta^{-1}(x'_\beta))$. *Then there is an element* $x \in X$ *such that* $u(x) = x'$.

Apply Theorem 1 to the inverse system of sets $\overline{u}_\alpha^{-1}(x'_\alpha)$, each carrying the discrete uniformity.

#### Example {#top-ii-s3-n5-exa-1 .statement}

Suppose we are given in $C$: (i) a sequence $(a_n)$ of distinct points such that the sequence $(|a_n|)$ is increasing and tends to $+\infty$; (ii) for each $n$, a rational function $z \to R_n(z)$ defined in $C - \{a_n\}$ and having a pole at $a_n$; (iii) an increasing sequence $(B_n)$ of open discs centred at 0, whose union is $C$, and such that none of the $a_k$ is on the frontier of any of the discs $B_n$. For each $n$, let $B'_n$ denote the intersection of $\overline{B}_n$ and the complement in $C$ of the set of points $a_n$; and let $X_n$ denote the set of all mappings

$$
z \to S(z) = P(z) + \sum_{a_k \in B'_n} R_k(z)
$$

of $B'_n$ into $C$, where $P$ is the restriction to $B'_n$ of a function which is continuous in $\overline{B}_n$ and holomorphic in $B_n$. We define a metric in $X_n$ by putting

$$
d_n(S_1, S_2) = \sup_{z \in B'_n} |S_1(z) - S_2(z)|.
$$

It is easily verified that $X_n$ is *complete* with respect to this metric. Finally, for $n \leq m$, we define a mapping $f_{nm} : X_m \to X_n$ such that if $S \in X_m$ then $f_{nm}(S)$ is the *restriction* of $S$ to $B'_n$. It is clear that the $f_{nm}$ are *uniformly continuous* and that $(X_n, f_{nm})$ is an inverse system of uniform spaces. This being so, an element of the inverse limit $X = \lim_{\leftarrow} X_n$ can be canonically identified with a meromorphic function $F$ in $\mathbf{C}$, whose only poles are the points $a_n$, and which is such that for each $n$, $F(z) - R_n(z)$ is holomorphic at $a_n$. The classical theorem of Mittag-Leffler asserts that $X$ is not empty; by virtue of Theorem 1, we have only to verify the condition (ML$_{nn}$) for all $n$. Let
$$
S_n = P_n + \sum_{a_k \in B_n} R_k
$$
be an element of $X_n$, where $P_n$ is continuous in $\overline{B}_n$ and holomorphic in $B_n$; for any $m \geq n$, let $Q_{mn}$ be the restriction of
$$
\sum_{a_h \in B_m - B_n} R_h \text{ to } B'_n;
$$
this latter sum is a holomorphic function in some neighbourhood of $\overline{B}_n$, hence (by Taylor's theorem) for each $\varepsilon > 0$ there is a polynomial $P_{mn}$ such that $|Q_{mn}(z) - P_{mn}(z)| \leq \varepsilon$ in $B_n$; if $S_m$ is the restriction of $S_n + Q_{mn} - P_{mn}$ to $B'_m$, we have $S_m \in X_m$ and $|S_m(z) - S_n(z)| \leq \varepsilon$ in $B'_n$. This completes the proof. \*

### 6. EXTENSION OF UNIFORMLY CONTINUOUS FUNCTIONS

The theorem of extension by continuity (Chapter I, § 8, no. 5, Theorem 1) has important additions when the functions in question take their values in a complete Hausdorff uniform space.

#### Proposition 11 {#top-ii-s3-prop-11 .statement}

*Let $A$ be a dense subset of a topological space $X$, and let $f$ be a mapping of $A$ into a complete Hausdorff uniform space $X'$. Then $f$ can be extended by continuity to $X$ if and only if, for each $x \in X$, the image under $f$ of the trace on $A$ of the neighbourhood filter of $x$ in $X$ is a Cauchy filter base in $X'$.

This follows from the theorem of extension by continuity (loc. cit.) because $X'$ is regular (§ 1, no. 2, Proposition 3) and because on $X'$ convergent filters are the same as Cauchy filters.

When $X$ is also a uniform space, there is the following theorem:

#### Theorem 2 {#top-ii-s3-thm-2 .statement}

*Let $f$ be a function defined on a dense subspace $A$ of a uniform space $X$, taking its values in a complete Hausdorff uniform space $X'$, and suppose that $f$ is uniformly continuous on $A$. Then $f$ can be extended to the whole of $X$ by continuity, and the extended function $\overline{f}$ is uniformly continuous.*

The existence of $\overline{f}$ is an immediate consequence of Propositions 3 and 11 of no. 1. Let us show that $\overline{f}$ is uniformly continuous. Let $V'$ be a closed symmetric entourage of $X'$, and let $V$ be an entourage of $X$ such that, when $x$ and $y$ are in $A$ and are $V$-close, then $f(x)$ and $f(y)$ are $V'$-close. We may assume that $V$ is the closure in $X \times X$ of an entourage $W$ of $A$ ($\S$ 2, no. 4, Proposition 6). We have $[ \bar{f}(x), \bar{f}(y) ] \in V'$ when $(x, y) \in W$; since $\bar{f} \times \bar{f}$ is continuous in $X \times X$ (Chapter I, $\S$ 4, no. 1, Proposition 1) we have also $[ \bar{f}(x), \bar{f}(y) ] \in V'$ when $(x, y) \in V = \overline{W}$, since $V'$ is closed (Chapter I, $\S$ 2, no. 1, Theorem 1).

Q.E.D.

#### Corollary {#top-ii-s3-n6-cor-1 .statement}

*Let $X_1, X_2$ be two complete Hausdorff uniform spaces, and let $Y_1, Y_2$ be dense subspaces of $X_1, X_2$ respectively. Then every isomorphism $f$ of $Y_1$ onto $Y_2$ extends to an isomorphism of $X_1$ onto $X_2$.*

$f$ is uniformly continuous in $Y_1$, hence (Theorem 2) extends to a uniformly continuous mapping $\bar{f} : X_1 \to X_2$. Likewise the inverse $g$ of $f$ extends to a uniformly continuous mapping $\bar{g} : X_2 \to X_1$. The function $\bar{g} \circ \bar{f}$ is therefore a continuous mapping of $X_1$ into itself whose restriction to $Y_1$ is the identity mapping; by the principle of extension of identities (Chapter I, $\S$ 8, no. 1, Corollary 1 to Proposition 2) $\bar{g} \circ \bar{f}$ is therefore the identity mapping of $X_1$; similarly $\bar{f} \circ \bar{g}$ is the identity map of $X_2$. Consequently (*Set Theory*, R, $\S$ 2, no. 12) $\bar{f}^{-1}$ and $\bar{g}$ are bijections and are inverses of each other; they are also uniformly continuous and are therefore isomorphisms ($\S$ 2, no. 1, Proposition 2).

It should be remarked that if $f$ is a *bijective* uniformly continuous mapping of $Y_1$ onto $Y_2$, its extension by continuity *need be neither injective nor surjective* (Exercise 3).

### 7. THE COMPLETION OF A UNIFORM SPACE

#### Theorem 3 {#top-ii-s3-thm-3 .statement}

*Let $X$ be a uniform space. Then there exists a complete Hausdorff uniform space $\hat{X}$ and a uniformly continuous mapping $i : X \to \hat{X}$ having the following property:*

(P) *Given any uniformly continuous mapping $f$ of $X$ into a complete Hausdorff uniform space $Y$, there is a unique uniformly continuous mapping $g : \hat{X} \to Y$ such that $f = g \circ i$.*

*If $(i_1, X_1)$ is another pair consisting of a complete Hausdorff uniform space $X_1$ and a uniformly continuous mapping $i_1 : X \to X_1$ having the property (P), then there is a unique isomorphism $\varphi : \hat{X} \to X_1$ such that $i_1 = \varphi \circ i$.*

1) Definition of $\hat{X}$. Let $\hat{X}$ be the set of minimal Cauchy filters (no. 2) on $X$. We shall define a uniform structure on $\hat{X}$. For this purpose, if $V$ is any symmetric entourage of $X$, let $\tilde{V}$ denote the set of all pairs $(\mathcal{K}, \mathcal{Y})$ of minimal Cauchy filters which have in common a $V$-small set. We shall show that the sets $\tilde{V}$ form a fundamental system of entourages of a uniform structure on $\hat{X}$:

(i) Since each $\mathcal{K} \in \hat{X}$ is a Cauchy filter, we have by definition $(\mathcal{K}, \mathcal{K}) \in \tilde{V}$ for every symmetric entourage $V$ of $X$; hence axiom $(U'_1)$ is satisfied.

(ii) If $V$ and $V'$ are two symmetric entourages of $X$, then $W = V \cap V'$ is a symmetric entourage, and every set which is $W$-small is also $V$-small and $V'$-small; hence $\tilde{W} \subset \tilde{V} \cap \tilde{V}'$, which prove $(B_1)$.

(iii) The sets $\tilde{V}$ are symmetric by definition, hence $(U''_1)$ is satisfied.

(iv) Given a symmetric entourage $V$ of $X$, let $W$ be a symmetric entourage such that $\tilde{V} \subset V$. Consider three minimal Cauchy filters $\mathcal{K}, \mathcal{Y}, \mathcal{B}$ such that $(\mathcal{K}, \mathcal{Y}) \in \tilde{W}$ and $(\mathcal{Y}, \mathcal{B}) \in \tilde{W}$; then there are two $W$-small sets $M, N$ such that $M \in \mathcal{K} \cap \mathcal{Y}$ and $N \in \mathcal{Y} \cap \mathcal{B}$. Since $M$ and $N$ belong to $\mathcal{Y}$, $M \cap N$ is not empty and therefore (no. 1, Proposition 1) $M \cup N$ is $\tilde{W}$-small and hence $V$-small; since $M \cup N$ belongs to $\mathcal{K}$ and to $\mathcal{B}$ we have $\tilde{W} \subset \tilde{V}$; hence $(U'''_1)$ is satisfied.

We show next that the uniform space $\hat{X}$ is Hausdorff. Let $\mathcal{K}, \mathcal{Y}$ be two minimal Cauchy filters on $X$ such that $(\mathcal{K}, \mathcal{Y}) \in \hat{X}$ for all symmetric entourages $V$ of $X$. It follows immediately that the sets $M \cup N$, where $M \in \mathcal{K}$ and $N \in \mathcal{Y}$, form a base of a filter $\mathcal{B}$ coarser than $\mathcal{K}$ and $\mathcal{Y}$. Now $\mathcal{B}$ is a Cauchy filter, since for every symmetric entourage $V$ of $X$ there is by hypothesis a $V$-small set $P$ belonging to both $\mathcal{K}$ and $\mathcal{Y}$ and therefore belonging to $\mathcal{B}$. By the definition of minimal Cauchy filters, we have $\mathcal{K} = \mathcal{B} = \mathcal{Y}$, and this shows that $\hat{X}$ is Hausdorff.

2) Definition of $i$; the uniform structure of $X$ is the inverse image under $i$ of that of $\hat{X}$. We know that for each $x \in X$ the neighbourhood filter $\mathfrak{B}(x)$ of $x$ in $X$ is a minimal Cauchy filter (no. 2, Proposition 5, Corollary 1). So we define $i(x) = \mathfrak{B}(x)$. Let $f = i \times i$; we shall show that for each symmetric entourage $V$ of $X$ we have $j^{-1}(\tilde{V}) \subset V \cup j^{-1}[(\tilde{V})^3]$, and this will prove our assertion (§ 2, no. 4). Now, if $[i(x), i(y)] \in \tilde{V}$, there is a $V$-small set $M$ which is a neighbourhood of each of $x$ and $y$, hence $(x, y) \in V$. Conversely, if $(x, y) \in V$, it is immediately seen that the set $V(x) \cup V(y)$ is $V$-small and is a neighbourhood of each of $x$ and $y$.

3) $\hat{X}$ is complete and $i(X)$ is dense in $\hat{X}$. The trace on $i(X)$ of a neighbourhood $\tilde{V}(\mathcal{X})$ of a point $\mathcal{X} \in X$ is the set of all $i(x)$ such that

$$
(\mathcal{X}, i(x)) \in \tilde{V}.
$$

This relation means that there is a $V$-small neighbourhood of $x$ in $X$ which belongs to $\mathcal{X}$, i.e. that $x$ is an interior point of a $V$-small set of $\mathcal{X}$. Let $M$ be the union of the interiors of all $V$-small sets of $\mathcal{X}$; then $M$ belongs to $\mathcal{X}$ (no. 2, Proposition 5, Corollary 4) and from what has been said it follows that $\tilde{V}(\mathcal{X}) \cap i(X) = i(M)$. We conclude that:

(i) $\tilde{V}(\mathcal{X}) \cap i(X)$ is not empty, hence $i(X)$ is dense in $\hat{X}$.
(ii) The trace of $\tilde{V}(\mathcal{X})$ on $i(X)$ belongs to the filter base $i(\mathcal{X})$ on $X$; hence this filter base converges in $\hat{X}$ to the point $\mathcal{X}$.

Now let $\mathfrak{F}$ be a Cauchy filter on $i(X)$; then from 2) above and Proposition 4 of no. 1, $\overline{i^1}(\mathfrak{F})$ is a base of a Cauchy filter $\mathfrak{G}$ on $X$. Let $\mathcal{X}$ be a minimal Cauchy filter coarser than $\mathfrak{G}$ (no. 2, Proposition 5); then $i(\mathcal{X})$ is a Cauchy filter base on $i(X)$ (no. 1, Proposition 3), and $\mathfrak{F} = i[\overline{i^1}(\mathfrak{F})]$ is finer than the filter whose base is $i(\mathcal{X})$. Since the latter converges in $\hat{X}$, so does $\mathfrak{F}$, and Proposition 9 of no. 4 therefore shows that $\hat{X}$ is complete.

4) Verification of the property (P). Let $f$ be a uniformly continuous mapping of $X$ into a complete Hausdorff uniform space $Y$. Let us first show that there is a unique uniformly continuous mapping $g_0 : i(X) \to Y$ such that $f = g_0 \circ i$. Since $f$ is continuous, we have

$$
f(x) = \lim f(\mathfrak{B}(x)),
$$

hence if we put $g_0(i(x)) = \lim f(\mathfrak{B}(x))$, we have $f = g_0 \circ i$; so it remains to show that $g_0$ is uniformly continuous in $i(X)$. Let $U$ be an entourage of $Y$ and let $V$ be a symmetric entourage of $X$ such that the relation $(x, x') \in V$ implies $(f(x), f(x')) \in U$; we have seen in 2) that the relation $(i(x), i(x')) \in \tilde{V}$ implies $(x, x') \in V$, hence also is implied
$$
(g_0(i(x)), g_0(i(x'))) \in U,
$$
which proves our assertion.

Let $g$ be the extension of $g_0$ by continuity to $\hat{X}$ (no. 6, Theorem 2); then $f = g \circ i$, and it is clear that $g$ is the unique continuous mapping of $\hat{X}$ into $Y$ satisfying this relation, since $i(X)$ is dense in $\hat{X}$ (Chapter I, § 8, no. 1, Proposition 2, Corollary 1).

Q.E.D.

#### Definition 4 {#top-ii-s3-def-4 .statement}

*The complete Hausdorff uniform space* $\hat{X}$ *defined in the proof of Theorem 3 is called the Hausdorff completion of* $X$, *and the mapping* $i : X \to \hat{X}$ *is called the canonical mapping of* $X$ *into its Hausdorff completion.*

We note also the following facts:

#### Proposition 12 {#top-ii-s3-prop-12 .statement}

(i) *The subspace* $i(X)$ *is dense in* $\hat{X}$.
(ii) *The graph of the equivalence relation* $i(x) = i(x')$ *is the intersection of the entourages of* $X$.
(iii) *The uniform structure of* $X$ *is the inverse image under* $i$ *of that of* $\hat{X}$ *[or of that of the subspace* $i(X)$].
(iv) *The entourages of* $i(X)$ *are the images under* $i \times i$ *of the entourages of* $X$, *and the closures in* $\hat{X} \times \hat{X}$ *of the entourages of* $i(X)$ *form a fundamental system of entourages of* $\hat{X}$.

(i) and (iii) have been proved in the course of the proof of Theorem 3; (iv) is a consequence of (i) and (iii) by virtue of general results proved earlier (§ 2, no. 4, Remark and Proposition 6). The relation
$$
i(x) = i(x')
$$
means by definition that $x$ and $x'$ have the same neighbourhood filter. But this implies, by definition, that $(x, x') \in V$ for every entourage $V$ of $X$, and the converse is obvious.

#### Corollary {#top-ii-s3-n7-cor-1 .statement}

*If* $X$ *is a Hausdorff uniform space, then the canonical mapping* $i : X \to \hat{X}$ *is an isomorphism of* $X$ *onto a dense subspace of* $\hat{X}$.

When $X$ is Hausdorff, $\hat{X}$ is said to be the *completion* of $X$, and we generally *identify* $X$ with a dense subset of $\hat{X}$ by means of $i$.

#### Remark {#top-ii-s3-n7-rem-1 .statement}

If this identification is made, the minimal Cauchy filters on X are just the traces on X of the neighbourhood filters of points of $\hat{X}$; this follows from the proof of Theorem 3.

The Corollary to Proposition 12 characterizes the completion of a Hausdorff uniform space:

#### Proposition 13 {#top-ii-s3-prop-13 .statement}

*If Y is a complete Hausdorff uniform space and X a dense subspace of Y, then the canonical injection $X \to Y$ extends to an isomorphism of $\hat{X}$ onto Y.*

For every uniformly continuous mapping of X into a complete Hausdorff uniform space Z extends uniquely to a uniformly continuous mapping of Y into Z by Theorem 2 of no. 6.

#### Proposition 14 {#top-ii-s3-prop-14 .statement}

*Let X be a complete Hausdorff uniform space, $\mathcal{U}$ its uniformity, and let Z be a dense subspace of X. If $\mathcal{U}'$ is a uniformity on X which is coarser than $\mathcal{U}$ and which induces the same uniformity as $\mathcal{U}$ on Z, then $\mathcal{U} = \mathcal{U}'$.*

Let X' denote the set X with the uniformity $\mathcal{U}'$. The composition of the canonical mapping $X' \to \hat{X}'$ and the identity mapping $X \to X'$ is a uniformly continuous mapping $\varphi : X \to \hat{X}'$. Since Z is Hausdorff for the uniform structure induced by $\mathcal{U}'$, the restriction of $\varphi$ to Z is by hypothesis an isomorphism of Z onto the dense subspace $\varphi(Z)$ of $\hat{X}'$; it follows (no. 6, Corollary to Theorem 2) that $\varphi$ itself is an isomorphism of X onto $\hat{X}'$, hence $X' = \hat{X}'$ and $\mathcal{U}' = \mathcal{U}$.

#### Proposition 15 {#top-ii-s3-prop-15 .statement}

*Let X and X' be two uniform spaces. For each uniformly continuous mapping $f : X \to X'$ there is a unique uniformly continuous mapping $\hat{f} : \hat{X} \to \hat{X}'$ such that the diagram

$$
\begin{array}{ccc}
X & \xrightarrow{i'} & X' \\
i \downarrow & & \downarrow i' \\
\hat{X} & \xrightarrow{\hat{f}} & \hat{X}'
\end{array}
$$

is commutative (*), where $i : X \to \hat{X}$ and $i' : X' \to \hat{X}'$ are the canonical mappings.

Apply Theorem 3 to the function $i' \circ f : X \to \hat{X}'$.

#### Corollary {#top-ii-s3-n7-cor-2 .statement}

*If $f : X \to X'$ and $g : X' \to X''$ are two uniformly continuous mappings and $h = g \circ f$, then $\hat{h} = \hat{g} \circ \hat{f}$.*

This is an immediate consequence of the uniqueness in Proposition 15.

(*) In other words, $i' \circ f = \hat{f} \circ i$.

### 8. THE HAUSDORFF UNIFORM SPACE ASSOCIATED WITH A UNIFORM SPACE

#### Proposition 16 {#top-ii-s3-prop-16 .statement}

Let $X$ be a uniform space and $i$ the canonical mapping of $X$ into its Hausdorff completion $\hat{X}$. For each uniformly continuous mapping $f$ of $X$ into a Hausdorff uniform space $Y$, there is a unique uniformly continuous mapping $h : i(X) \to Y$ such that $f = h \circ i$.

We may identify $Y$ with a subspace of its completion $\hat{Y}$ (no. 7, Corollary to Proposition 12), and $f$ can then be considered as a uniformly continuous mapping of $X$ into $\hat{Y}$. By virtue of Theorem 3, $f$ is then of the form $f = g \circ i$, where $g$ is a uniformly continuous mapping of $\hat{X}$ into $\hat{Y}$. If $h$ is the restriction of $g$ to $i(X)$, then clearly $f = h \circ i$, and $h$ maps $i(X)$ into $Y$. The uniqueness of $h$ is trivial.

The pair $(i, i(X))$ is therefore the solution of a universal mapping problem (Set Theory, Chapter IV, § 3, no. 1), where this time we take the $\Sigma$-sets to be Hausdorff uniform spaces, and the $\sigma$-morphisms (resp. $\alpha$-mappings) to be uniformly continuous mappings (resp. uniformly continuous mappings of $X$ into a Hausdorff uniform space).

#### Definition 5 {#top-ii-s3-def-5 .statement}

The Hausdorff uniform space $i(X)$ defined in the proof of Theorem 3 is called the Hausdorff uniform space associated with $X$.

The Hausdorff completion of $X$ is thus the completion of the Hausdorff uniform space associated with $X$.

#### Corollary {#top-ii-s3-n8-cor-1 .statement}

Let $X, Y$ be two uniform spaces and $X', Y'$ the associated Hausdorff spaces. For each uniformly continuous mapping $f : X \to Y$ there is a unique uniformly continuous mapping $f' : X' \to Y'$ for which the diagram

$$
\begin{array}{ccc}
X & \xrightarrow{f} & Y \\
i \downarrow & & \downarrow i' \\
X' & \xrightarrow{f'} & Y'
\end{array}
$$

is commutative, where $i$ and $i'$ are the canonical mappings.

Apply Proposition 16 to $i' \circ f : X \to Y'$.

The Hausdorff space associated with a uniform space may also be characterized by the following property:

#### Proposition 17 {#top-ii-s3-prop-17 .statement}

Let $X$ be a uniform space, $i(X)$ its associated Hausdorff space, and let $f$ be a mapping of $X$ onto a Hausdorff uniform space $X'$, such that the uniformity of $X$ is the inverse image under $f$ of the uniformity of $X'$. Then the mapping $g : i(X) \to X'$ such that $f = g \circ i$ is an isomorphism.

By Proposition 16, $g$ is uniformly continuous; also $g$ is obviously surjective, and is also injective because the relation $f(x) = f(y)$ implies by definition that $(x, y)$ belongs to all the entourages of $X$, and therefore that $i(x) = i(y)$ (no. 7, Proposition 12). Finally, the entourages of $X'$ are the images under $f \times f$ of the entourages of $X$ ($§ 2$, no. 4, Remark), hence they are also the images under $g \times g$ of the entourages of $i(X)$ (no. 7, Proposition 12); hence the result.

#### Remark {#top-ii-s3-n8-rem-1 .statement}

Let $R$ be the equivalence relation $i(x) = i(x')$ on $X$. We have seen (no. 7, Proposition 12) that the graph $C$ of $R$ is the intersection of all the entourages of $X$. It is clear that every open set (and therefore also every closed set) in $X$ is *saturated* with respect to $R$; taking account of the definition of the inverse image of a topology, we conclude that the canonical bijection of the quotient space $X/R$ onto $i(X)$ induced by $i$ is a *homeomorphism*. The Hausdorff space associated with $X$ can therefore be identified, *qua* topological space, with $X/R$. The canonical mapping $i : X \to i(X)$ is open and closed, and even proper (Chapter I, $§ 10$, no. 2, Example).

Let $X'$ be another uniform space, $C'$ the intersection of all the entourages of $X'$, and $R'$ the equivalence relation whose graph is $C'$. Let $f : X \to X'$ be a *continuous* mapping. Since the inverse image under $f$ of any neighbourhood of $f(x)$ is a neighbourhood of $x$, it follows that the inverse image under $f$ of $C'(f(x))$ contains $C(x)$, and therefore $f$ is *compatible* with $R$ and $R'$, and induces a continuous mapping $X/R \to X'/R'$ (Chapter I, $§ 3$, no. 4, Corollary to Proposition 6). This generalizes the corollary to Proposition 16.

### 9. COMPLETION OF SUBSPACES AND PRODUCT SPACES

#### Proposition 18 {#top-ii-s3-prop-18 .statement}

*Let $X$ be a set, let $(Y_\lambda)_{\lambda \in L}$ be a family of uniform spaces, and for each $\lambda \in L$ let $f_\lambda$ be a mapping of $X$ into $Y_\lambda$. Let $X$ carry the coarsest uniformity $U$ which makes all the $f_\lambda$ uniformly continuous. Then the uniformity of the Hausdorff completion $\hat{X}$ of $X$ is the coarsest for which all the mappings $\hat{f}_\lambda : \hat{X} \to \hat{Y}_\lambda$ ($\lambda \in L$) (no. 7, Proposition 15) are uniformly continuous. Furthermore, if $j_\lambda$ is the canonical mapping of $Y_\lambda$ into $\hat{Y}_\lambda$, and if $g_\lambda = j_\lambda \circ f_\lambda$, then $\hat{X}$ may be identified with the closure in $\prod_{\lambda \in L} \hat{Y}_\lambda$ of the image of $X$ under the mapping $x \to (g_\lambda(x))$.*

Let $X'$ (resp. $Y'_\lambda$) be the Hausdorff uniform space associated with $X$ (resp. $Y_\lambda$), and let $f'_\lambda : X' \to Y'_\lambda$ be the uniformly continuous mapping which makes the diagram

$$
\begin{array}{ccc}
X & \xrightarrow{f_\lambda} & Y_\lambda \\
i \downarrow & & \downarrow j_\lambda \\
X' & \xrightarrow{f'_\lambda} & Y'_\lambda
\end{array}
$$

commutative (*i* being the canonical mapping).

The transitivity of initial uniformities (§ 2, no. 3, Proposition 5) shows on the one hand that $\mathcal{U}$ is the coarsest uniformity for which the mappings $j_\lambda \circ f_\lambda : X \to Y'_\lambda$ are uniformly continuous, and on the other hand that $\mathcal{U}$ is also the inverse image under $i$ of the coarsest uniformity $\mathcal{U}'$ on the set $X'$ for which the $f'_\lambda$ are uniformly continuous. Now $\mathcal{U}'$ is *Hausdorff*, for if $x_1, x_2$ are two points of $X$ such that $j_\lambda(f_\lambda(x_1)) = j_\lambda(f_\lambda(x_2))$ for each $\lambda \in L$, then $(x_1, x_2)$ belongs to all the entourages of $\mathcal{U}$ and hence $i(x_1) = i(x_2)$. Proposition 17 of no. 8 therefore shows that $\mathcal{U}'$ is the uniformity of the Hausdorff space $X'$ associated with $X$.

This being so, the bijection $x' \to (f'_\lambda(x'))$ identifies $X$ with a uniform subspace of the product $\prod_\lambda Y'_\lambda$ (§ 2, no. 6, Proposition 8). Since the $Y'_\lambda$ are Hausdorff, each $Y'_\lambda$ can be identified with a dense subspace of its completion $\hat{Y}_\lambda$, and hence $\prod_\lambda Y'_\lambda$ can be identified with a dense subspace of $\prod_\lambda \hat{Y}_\lambda$ (Chapter I, § 4, no. 3, Proposition 7). But $\prod_\lambda \hat{Y}_\lambda$ is Hausdorff and complete (no. 5, Proposition 10); the closure $\overline{X'}$ of $X'$ in $\prod_\lambda \hat{Y}_\lambda$ is therefore a complete Hausdorff subspace (no. 4, Proposition 8) which can be identified with the Hausdorff completion $\hat{X}$ of $X$; under this identification the mappings $\hat{f}_\lambda$ become the projections onto the factors $\hat{Y}_\lambda$, and the proposition is proved.

#### Corollary 1 {#top-ii-s3-prop-18-cor-1 .statement}

*Let $X$ be a uniform space and let $i$ be the canonical mapping of $X$ into its Hausdorff completion $\hat{X}$; let $A$ be a subspace of $X$ and $j : A \to X$ the canonical injection. Then $\hat{j} : \hat{A} \to \hat{X}$ is an isomorphism of $\hat{A}$ onto the closure of $i(A)$ in $\hat{X}$.*

#### Corollary 2 {#top-ii-s3-prop-18-cor-2 .statement}

*Let $(Y_\lambda)_{\lambda \in L}$ be a family of uniform spaces. Then the Hausdorff completion of the product space $\prod_{\lambda \in L} Y_\lambda$ is canonically isomorphic to the product $\prod_{\lambda \in L} \hat{Y}_\lambda$.*

### Exercises {#top-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
