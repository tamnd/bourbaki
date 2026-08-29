---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 7
section_title: Limits
lang: en
source: top-i-iv
book_pages: 68-74, 132-133
pdf_pages: 0074-0080, 0138-0139
extraction: ocr
subsections:
    - "no": 1
      title: LIMIT OF A FILTER
      page: 68
      pdf_page: 74
    - "no": 2
      title: CLUSTER POINT OF A FILTER BASE
      page: 69
      pdf_page: 75
    - "no": 3
      title: LIMIT POINT AND CLUSTER POINT OF A FUNCTION
      page: 70
      pdf_page: 76
    - "no": 4
      title: LIMITS AND CONTINUITY
      page: 72
      pdf_page: 78
    - "no": 5
      title: LIMITS RELATIVE TO A SUBSPACE
      page: 73
      pdf_page: 79
    - "no": 6
      title: LIMITS IN PRODUCT SPACES AND QUOTIENT SPACES
      page: 74
      pdf_page: 80
statements: 23
exercises: 7
content_sha256: f4465bca5af48f4fe2251f95b010c5ca18b72eba266e16cfbc6dacf8a1cb9584
---

## 7. LIMITS

### 1. LIMIT OF A FILTER

#### Definition 1 {#top-i-s7-def-1 .statement}

Let $X$ be a topological space and $\mathfrak{F}$ a filter on $X$. A point $x \in X$ is said to be a limit point (or simply a limit) of $\mathfrak{F}$, if $\mathfrak{F}$ is finer than the neighbourhood filter $\mathcal{B}(x)$ of $x$; $\mathfrak{F}$ is also said to converge (or to be convergent) to $x$. *The point* $x$ *is said to be a limit of a filter base* $\mathcal{B}$ *on* $X$, *and* $\mathcal{B}$ *is said to converge to* $x$, *if the filter whose base is* $\mathcal{B}$ *converges to* $x$.

This definition, together with Proposition 4 of § 6, no. 3, gives the following criterion:

#### Proposition 1 {#top-i-s7-prop-1 .statement}

*A filter base* $\mathcal{B}$ *on a topological space* $X$ *converges to* $x$ *if and only if every set of a fundamental system of neighbourhoods of* $x$ *contains a set of* $\mathcal{B}$.

In accordance with the terminology introduced in § 1, no. 2 we can state Proposition 1 in the following way: $\mathcal{B}$ converges to $x$ if and only if there are sets of $\mathcal{B}$ *as near as we please to* $x$.

If a filter $\mathfrak{F}$ converges to $x$, then every filter *finer* than $\mathfrak{F}$ also converges to $x$, by reason of Definition 1. Likewise, if the topology of $X$ is replaced by a *coarser* topology, the neighbourhood filter of $x$ is replaced by a *coarser* filter ($\S$ 2, no. 2, Proposition 3), and therefore $\mathfrak{F}$ still converges to $x$ in this new topology.

We can therefore say that *the finer the topology, the fewer convergent filters there are in this topology*. In particular, in the discrete topology, the only convergent filters are the neighbourhood filters, for these are the trivial ultrafilters on $X$ ($\S$ 6, no. 4).

Let $\Phi$ be a set of filters on $X$, all of which converge to the same point $x$; the neighbourhood filter $\mathcal{B}(x)$ is coarser than all the filters of $\Phi$, hence also coarser than the *intersection* $\mathfrak{J}$ of these filters; in other words, $\mathfrak{J}$ also converges to $x$.

#### Proposition 2 {#top-i-s7-prop-2 .statement}

*A filter* $\mathfrak{F}$ *on a topological space* $X$ *converges to a point* $x$ *if and only if every ultrafilter which is finer than* $\mathfrak{F}$ *converges to* $x$.

This is an immediate consequence of the preceding remarks and Proposition 7 of § 6, no. 4.

In general a filter can have *several distinct limit points*; we shall revert to this question in § 8, no. 1.

### 2. CLUSTER POINT OF A FILTER BASE

#### Definition 2 {#top-i-s7-def-2 .statement}

*In a topological space* $X$, *a point* $x$ *is a cluster point of a filter base* $\mathcal{B}$ *on* $X$ *if it lies in the closure of all the sets of* $\mathcal{B}$.

If $x$ is a cluster point of a filter base $\mathcal{B}$, it is also a cluster point of every *equivalent* filter base by reason of § 6, no. 3, corollary to Proposition 4; in particular, $x$ is a cluster point of the *filter* whose base is $\mathcal{B}$.

#### Proposition 3 {#top-i-s7-prop-3 .statement}

*A point x is a cluster point of a filter base B if and only if every set of a fundamental system of neighbourhoods of x meets every set of B.*

This follows immediately from the definitions.

This proposition and Corollary 2 to Proposition 1 of § 6, no. 2 show that the property "x is a cluster point of the filter $\mathfrak{F}$" is equivalent to the property "there is a filter which is finer than both $\mathfrak{F}$ and the neighbourhood filter of x". In other words:

#### Proposition 4 {#top-i-s7-prop-4 .statement}

*A point x is a cluster point of a filter $\mathfrak{F}$ if and only if there is a filter finer than $\mathfrak{F}$ which converges to x.*

In particular, every *limit point* of a filter $\mathfrak{F}$ is a *cluster point* of $\mathfrak{F}$.

#### Corollary {#top-i-s7-n2-cor-1 .statement}

*An ultrafilter $\mathcal{U}$ converges to a point x if and only if x is a cluster point of $\mathcal{U}$.*

If x is a cluster point of a filter $\mathfrak{F}$, it is also a cluster point of every filter *coarser* than $\mathfrak{F}$; likewise, if we replace the topology of X by a *coarser* topology, x remains a cluster point of $\mathfrak{F}$ in the new topology.

The set of cluster points of a filter base $\mathcal{B}$ on X is by definition the set $\bigcap_{M \in \mathcal{B}} \overline{M}$, whence

#### Proposition 5 {#top-i-s7-prop-5 .statement}

*The set of cluster points of a filter base on a topological space X is closed in X.*

#### Proposition 6 {#top-i-s7-prop-6 .statement}

*Let $\mathcal{B}$ be a filter base on a subset A of a topological space X. Then every cluster point of $\mathcal{B}$ in X belongs to $\overline{A}$; and conversely every point of $\overline{A}$ is a limit point of a filter on A.*

The first assertion is trivial; on the other hand, if $x \in \overline{A}$, the trace on A of the neighbourhood filter of x in X is a filter on A which evidently converges to x.

#### Remark {#top-i-s7-n2-rem-1 .statement}

A filter on a topological space need have no cluster points (and *a fortiori* no limit points); for example, in an *infinite discrete space* the filter of complements of finite subsets has no cluster points. Spaces in which every filter has a cluster point play an important role in mathematics, and we shall study them in § 9.

### 3. LIMIT POINT AND CLUSTER POINT OF A FUNCTION

#### Definition 3 {#top-i-s7-def-3 .statement}

*Let f be a mapping of a set X into a topological space Y, and let $\mathfrak{F}$ be a filter on X. A point $y \in Y$ is said to be a limit point (or simply a limit) (resp. cluster point) of f with respect to the filter $\mathfrak{F}$ if y is a limit point (resp. cluster point) of the filter base $f(\mathfrak{F})$.*

The relation "y is a limit of f with respect to the filter $\mathfrak{F}$" is written $\lim_{\mathfrak{F}} f = y$, or $\lim_{x, \mathfrak{F}} f(x) = y$, or $\lim_x f(x) = y$ if there is no risk of confusion.

From Definition 3 and Propositions 1 (no. 1) and 3 (no. 2) we deduce the following criteria:

#### Proposition 7 {#top-i-s7-prop-7 .statement}

*A point $y \in Y$ is a limit of $f$ with respect to the filter $\mathfrak{F}$ if and only if, for each neighbourhood $V$ of $y$ in $Y$, there is a set $M \in \mathfrak{F}$ such that $f(M) \subset V$ (i.e. $\overline{f}(V) \in \mathfrak{F}$ for each neighbourhood $V$ of $y$).*
*A point $y \in Y$ is a cluster point of $f$ with respect to $\mathfrak{F}$ if and only if for each neighbourhood $V$ of $y$ and each $M \in \mathfrak{F}$ there is a point $x \in M$ such that $f(x) \in V$.*

#### Example 1 {#top-i-s7-n3-exa-1 .statement}

A sequence of points $(x_n)_{n \in \mathbf{N}}$ of a topological space is a mapping $n \to x_n$ of $\mathbf{N}$ into $X$. In analysis one frequently uses the notions of limit point and cluster point of such a mapping *with respect to the Fréchet filter* (§ 6, no. 1) on $\mathbf{N}$; if $y$ is a limit of $n \to x_n$ with respect to the Fréchet filter, $y$ is said to be a *limit of the sequence* $(x_n)$ *as n tends to infinity*, and we write $\lim_{n \to \infty} x_n = y$. A cluster point of the mapping $n \to x_n$ with respect to the Fréchet filter is called a *cluster point of the sequence* $(x_n)$.

Thus a point $y \in X$ is a limit (resp. cluster point) of a sequence $(x_n)$ of points of $X$ if it is a limit point (resp. cluster point) of the *elementary filter associated with* $(x_n)$ (§ 6, no. 8).

The point $y$ is a limit of a sequence $(x_n)$ in $X$ if and only if, for *every* neighbourhood $V$ of $y$ in $X$, *all but a finite number of the terms of the sequence* $(x_n)$ *are in* $V$, i.e. there is an integer $n_0$ such that $x_n \in V$ for all $n \geq n_0$. Likewise $y$ is a cluster point of the sequence $(x_n)$ if and only if, for *every* neighbourhood $V$ of $y$ in $X$ and *every* integer $n_0$, there is an integer $n \geq n_0$ such that $x_n \in V$.

#### Example 2 {#top-i-s7-n3-exa-2 .statement}

More generally, let $f$ be a mapping of a *directed* set $A$ into a topological space $X$. If $x \in X$ is a limit (resp. cluster point) of $f$ with respect to the *section filter* of $A$ then $x$ is said to be a *limit* (resp. *cluster point*) of $f$ *with respect to the directed set* $A$, and we write $x = \lim_{z \in A} f(z)$.

If $y$ is a limit (resp. cluster point) of a mapping $f : X \to Y$ with respect to a filter $\mathfrak{F}$ on $X$, then $y$ remains a limit (resp. cluster point) of $f$ with respect to $\mathfrak{F}$ if we replace the topology of $Y$ by a *coarser* topology, or if we replace the filter $\mathfrak{F}$ by a *finer* (resp. *coarser*) filter.

#### Proposition 8 {#top-i-s7-prop-8 .statement}

*Let $f$ be a mapping of a set $X$ into a topological space $Y$; then $y \in Y$ is a cluster point of $f$ with respect to $\mathfrak{F}$ if and only if there is a filter $\mathfrak{G}$ on $X$ which is finer than $\mathfrak{F}$ and such that $y$ is a limit of $f$ with respect to $\mathfrak{G}$.*

For if $y$ is a cluster point of $f$ with respect to $\mathfrak{F}$, and if $\mathcal{B}$ is the neighbourhood filter of $y$, then $\overline{f}^{-1}(\mathcal{B})$ is a filter base on $X$ since every set of $\overline{f}^{-1}(\mathcal{B})$ meets every set of $\mathfrak{F}$ (§ 6, no. 6). This remark shows also that there is a filter $\mathcal{G}$ on $X$ which is finer than both $\mathfrak{F}$ and the filter with base $\overline{f}^{-1}(\mathcal{B})$ (§ 6, no. 2, Proposition 1, Corollary 2), hence that $y$ is a limit point of $f$ with respect to $\mathcal{G}$.

Notice finally that if $f$ is a mapping of a set $X$ into a topological space $Y$, the set of cluster points of $f$ with respect to a filter $\mathfrak{F}$ on $X$ is *closed* in $Y$ (no. 2, Proposition 5) and possibly empty.

#### Remark {#top-i-s7-n3-rem-1 .statement}

If $y \in Y$ is a limit (resp. cluster point) of a mapping $f : X \to Y$ with respect to a filter $\mathfrak{F}$ on $X$, then $y$ is also a limit (resp. cluster point) of every function $g : X \to Y$ which has *the same germ* as $f$ with respect to $\mathfrak{F}$ (§ 6, no. 9); $y$ is said to be a *limit* (resp. *cluster point*) *of the germ* $\tilde{f}$ *of* $f$ with respect to $\mathfrak{F}$.

### 4. LIMITS AND CONTINUITY

Let $X, Y$ be two topological spaces, $f$ a mapping of $X$ into $Y$, $\mathcal{B}$ the neighbourhood filter in $X$ of a point $a \in X$. Instead of saying that $y \in Y$ is a limit of $f$ with respect to the filter $\mathcal{B}$ and writing $y = \lim_{\mathcal{B}} f$, we use the special notation

$$
y = \lim_{i \in I} f(x),
$$

and we say that $y$ is a *limit of* $f$ *at the point* $a$, or that $f(x)$ *tends to* $y$ *as* $x$ *tends to* $a$. Similarly, instead of saying that $y$ is a cluster point of $f$ with respect to $\mathcal{B}$, we say that $y$ *is a cluster point of* $f$ *at the point* $a$.

A consideration of the definition of continuity (§ 2, no. 1, Definition 1) Proposition 7 of no. 3 shows that:

#### Proposition 9 {#top-i-s7-prop-9 .statement}

*A mapping* $f$ *of a topological space* $X$ *into a topological space* $Y$ *is continuous at a point* $a \in X$ *if and only if* $\lim_{i \in I} f(x) = f(a)$.

#### Corollary 1 {#top-i-s7-prop-9-cor-1 .statement}

*Let* $X, Y$ *be two topological spaces, $f$ a mapping of* $X$ *into* $Y$ *which is continuous at a point* $a \in X$; *then, for every filter base* $\mathcal{B}$ *on* $X$ *which converges to* $a$, *the filter base* $f(\mathcal{B})$ *converges to* $f(a)$. *Conversely if, for every ultrafilter* $\mathcal{U}$ *on* $X$ *which converges to* $a$, *the ultrafilter base* $f(\mathcal{U})$ *converges to* $f(a)$, *then* $f$ *is continuous at* $a$.

The first assertion is an immediate consequence of Proposition 9. To prove the second, suppose that $f$ is not continuous at $a$; then there is a neighbourhood W of $f(a)$ in Y such that $\overline{f}^{-1}(W)$ does not belong to the filter $\mathfrak{B}$ of neighbourhoods of $a$ in X. Hence (§ 6, no. 4, Proposition 7) there is an ultrafilter $\mathfrak{U}$, finer than $\mathfrak{B}$, which does not contain $\overline{f}^{-1}(W)$ and therefore contains its complement $A = X - \overline{f}^{-1}(W)$ (§ 6, no. 4, Proposition 5); since $f(A) \cap W = \varnothing$, $f(\mathfrak{U})$ does not converge to $f(a)$.

#### Corollary 2 {#top-i-s7-prop-9-cor-2 .statement}

*Let g be a mapping of a set Z into a topological space X, which has a limit a with respect to a filter $\mathfrak{F}$ on Z; then if the map $f : X \to Y$ is continuous at a, the composition $f \circ g$ has $f(a)$ as a limit point with respect to $\mathfrak{F}$.*

### 5. LIMITS RELATIVE TO A SUBSPACE

Let X, Y be two topological spaces, let A be a subset of X, and let $a \in X$ be a point of the *closure* of A (but not necessarily in A). Let $\mathfrak{F}$ be the *trace* on A of the neighbourhood filter of $a$ in X. If $f$ is a mapping of A into Y, then instead of saying that $y \in Y$ is a limit of $f$ with respect to $\mathfrak{F}$ and writing $y = \lim_{\mathfrak{F}} f$, we write

$$
y = \lim_{x \to a, x \in A} f(x)
$$

and we say that $y$ is a *limit of f at a, relative to the subspace* A, or that $f(x)$ *tends to y as x tends to a while remaining in* A. We have then $y \in f(A)$.

If $A = \mathbf{C}\{a\}$ where $a$ is *not* an isolated point of X, then we write

$$
y = \lim_{x \to a, x \neq a} f(x)
$$

instead of $y = \lim_{x \to a, x \in A} f(x)$.

We make analogous definitions for cluster points.

If $f$ is the *restriction* to A of a mapping $g : X \to Y$, we say that $g$ has a limit (resp. cluster point) $y$ relative to A at a point $a \in \overline{A}$, if $y$ is a limit (resp. cluster point) of $f$ at $a$, relative to A.

Let B be a subset of A and let $a \in X$ be a point of the closure of B; if $y$ is a limit at $a$, *relative to* A, of a map $f : A \to Y$, then $y$ is also a limit of $f$ at $a$, *relative to* B; the converse is not necessarily true.

But if V is a *neighbourhood* in X of a point $a \in \overline{A}$ and if $f$ has a limit $y$ at $a$, *relative to* $V \cap A$, then $y$ is still a limit of $f$ at $a$, *relative to* A.

Let $a$ be a *non-isolated* point of X, so that $a$ is in the closure of $\mathbf{C}\{a\}$. Then a mapping $f : X \to Y$ is *continuous at* $a$ if and only if we have $f(a) = \lim_{x \to a, x \neq a} f(x)$; this follows immediately from the definitions.

### 6. LIMITS IN PRODUCT SPACES AND QUOTIENT SPACES

#### Proposition 10 {#top-i-s7-prop-10 .statement}

Let $X$ be a set, let $(Y_i)_{i \in I}$ be a family of topological spaces, and for each $i \in I$ let $f_i$ be a mapping of $X$ into $Y_i$. Let $X$ be given the coarsest topology $\mathcal{T}$ for which the $f_i$ are continuous. Then a necessary and sufficient condition for a filter $\mathfrak{F}$ on $X$ to converge to $a \in X$ is that for each $i \in I$ the filter base $f_i(\mathfrak{F})$ should converge to $f_i(a)$ in $Y_i$.

The condition is necessary since the $f_i$ are continuous (no. 4, Proposition 9, Corollary 1). Conversely, suppose that the condition is satisfied, and let $V$ be an open neighbourhood of $a$ in $X$. By the definition of $\mathcal{T}$ (§ 2, no. 3, Proposition 4) there is a finite subset $J$ of $I$, and for each $i \in J$ an open subset $U_i$ of $Y_i$, such that $f_i(a) \in U_i$ for $i \in J$ and such that $V$ contains the set
$$
\bigcap_{i \in J} f_i^{-1}(U_i).
$$
The hypothesis implies that $f_i^{-1}(U_i) \in \mathfrak{F}$ (no. 3, Proposition 7); since $J$ is finite, it follows that
$$
M = \bigcap_{i \in J} f_i^{-1}(U_i)
$$
belongs to $\mathfrak{F}$, and $M \subset V$. This completes the proof.

#### Corollary 1 {#top-i-s7-prop-10-cor-1 .statement}

A filter $\mathfrak{F}$ on a product space $X = \prod_{i \in I} X_i$ converges to a point $x$ if and only if for each $i \in I$ the filter base $\operatorname{pr}_i(\mathfrak{F})$ converges to $\operatorname{pr}_i(x)$.

#### Corollary 2 {#top-i-s7-prop-10-cor-2 .statement}

Let $f = (f_i)$ be a mapping of a set $X$ into a product space $Y = \prod_{i \in I} Y_i$. Then $f$ has a limit $y = (y_i)$ with respect to a filter $\mathfrak{F}$ on $X$ if and only if for each $i \in I$ $f_i$ has limit $y_i$ with respect to $\mathfrak{F}$.

#### Proposition 11 {#top-i-s7-prop-11 .statement}

Let $R$ be an open equivalence relation on a topological space $X$ and let $\varphi$ be the canonical mapping $X \to X/R$. Then for each $x \in X$ and each filter base $\mathcal{B}'$ on $X/R$ which converges to $\varphi(x)$, there is a filter base $\mathcal{B}$ on $X$ which converges to $x$ and is such that $\varphi(\mathcal{B})$ is equivalent to $\mathcal{B}'$.

If $U$ is any neighbourhood of $x$ in $X$, then $\varphi(U)$ is a neighbourhood of $\varphi(x)$ in $X/R$ (§ 5, no. 3, Proposition 5), hence there is a set $M' \in \mathcal{B}'$ such that $M' \subset \varphi(U)$; if we put $M = U \cap \varphi^{-1}(M')$, then $M' = \varphi(M)$. This shows that as $M'$ runs through $\mathcal{B}'$ and $U$ runs through the neighbourhood filter of $x$, the sets $U \cap \varphi^{-1}(M')$ form a filter base $\mathcal{B}$ on $X$; clearly $\mathcal{B}$ converges to $x$ and $\varphi(\mathcal{B})$ is equivalent to $\mathcal{B}'$.

### Exercises {#top-i-s7-exercises}

See the [exercises for § 7](exercises/s7/).
