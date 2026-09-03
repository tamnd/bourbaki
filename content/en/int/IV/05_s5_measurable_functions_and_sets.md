---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 5
section_title: Measurable functions and sets
lang: en
source: int-i-vi
book_pages: INT IV.59-INT IV.89, INT IV.127-INT IV.134
pdf_pages: 0166-0196, 0234-0241
extraction: ocr
subsections:
    - "no": 1
      title: Definition of measurable functions and sets
      page: 59
      pdf_page: 166
    - "no": 2
      title: Principle of localization. Locally negligible sets
      page: 61
      pdf_page: 168
    - "no": 3
      title: Elementary properties of measurable functions
      page: 63
      pdf_page: 170
    - "no": 4
      title: Limits of measurable functions
      page: 64
      pdf_page: 171
    - "no": 5
      title: Criteria for measurability
      page: 66
      pdf_page: 173
    - "no": 6
      title: Criteria for integrability
      page: 71
      pdf_page: 178
    - "no": 7
      title: Measure induced on a locally compact subspace
      page: 73
      pdf_page: 180
    - "no": 8
      title: $\mu$-dense families of compact sets
      page: 76
      pdf_page: 183
    - "no": 9
      title: Locally countable partitions
      page: 77
      pdf_page: 184
    - "no": 10
      title: Measurable functions defined on a measurable subset
      page: 78
      pdf_page: 185
    - "no": 11
      title: Convergence in measure
      page: 80
      pdf_page: 187
    - "no": 12
      title: A property of vague convergence
      page: 86
      pdf_page: 193
statements: 79
exercises: 30
content_sha256: cafef13590e5fac8f8b8089f53dc63b8a0c799da5075967508e0612658483c73
---

## § 5. MEASURABLE FUNCTIONS AND SETS

### 1. Definition of measurable functions and sets

#### Definition 1 {#int-iv-s5-def-1 .statement}

*Let $X$ be a locally compact space, $\mu$ a measure on $X$. A mapping $f$ of $X$ into a topological space $F$ is said to be measurable for the measure $\mu$ (or to be $\mu$-measurable) if, for every compact subset $K$ of $X$, there exist a $\mu$-negligible set $N \subset K$ and a partition of $K - N$ formed by a sequence (finite or infinite) $(K_n)$ of compact sets, such that the restriction of $f$ to each $K_n$ is continuous.*

It is clear that every continuous mapping of $X$ into $F$ is measurable.

Note that if $\mu$ and $\nu$ are two measures on $X$ such that every $\mu$-negligible set is $\nu$-negligible, then *every $\mu$-measurable function is also $\nu$-measurable* (cf. Ch. V, §5, Nos. 5, 6).

Definition 1 may be transformed into the following criterion:

#### Proposition 1 {#int-iv-s5-prop-1 .statement}

*For a mapping $f$ of $X$ into $F$ to be measurable, it is necessary and sufficient that, for every compact set $K \subset X$ and every number $\varepsilon > 0$, there exist a compact set $K_1 \subset K$ such that $|\mu|(K - K_1) \leq \varepsilon$ and the restriction of $f$ to $K_1$ is continuous.*

If this condition is fulfilled, we may define recursively a sequence of pairwise disjoint compact sets $K_n \subset K$ such that $|\mu|(K - \bigcup_{i=1}^n K_i) \leq 1/n$ and such that the restriction of $f$ to each $K_n$ is continuous ($§ 4$, No. 6, Th. 4); the complement with respect to $K$ of the union of the $K_n$ is then negligible ($§ 4$, No. 5, Cor. of Prop. 7), thus $f$ is measurable. Conversely, suppose there exist a negligible set $N \subset K$ and a partition $(K_n)$ of $K - N$ formed of compact sets such that the restriction of $f$ to each $K_n$ is continuous; for every $\varepsilon > 0$ there exists an integer $n$ such that, if $H = \bigcup_{i=1}^n K_i$, then $|\mu|(K - H) \leq \varepsilon$ (§ 4, No. 5, Cor. of Prop. 7); the set $H$ is compact, the $K_i$ ($1 \leq i \leq n$) form a finite partition of $H$ into compact sets, and the restriction of $f$ to each $K_i$ is continuous; therefore the restriction of $f$ to $H$ is continuous.

#### Proposition 2 {#int-iv-s5-prop-2 .statement}

*Let* $(F_n)$ *be a sequence of topological spaces and, for each* $n$, *let* $f_n$ *be a measurable mapping of* $X$ *into* $F_n$. *For every compact set* $K \subset X$ *and every* $\varepsilon > 0$, *there exists a compact set* $K_0 \subset K$ *such that* $|\mu|(K - K_0) \leq \varepsilon$ *and the restriction to* $K_0$ *of each of the functions* $f_n$ *is continuous*.

For each integer $n \geq 1$ there exists a compact set $K_n \subset K$ such that $|\mu|(K - K_n) \leq \varepsilon / 2^n$ and the restriction of $f_n$ to $K_n$ is continuous. The set $K_0 = \bigcap_{n=1}^\infty K_n$ is compact, the restrictions to $K_0$ of all of the functions $f_n$ are continuous and, since $K - K_0$ is contained in the union of the $K - K_n$, $|\mu|(K - K_0) \leq \sum_{n=1}^\infty \varepsilon / 2^n = \varepsilon$.

#### Definition 2 {#int-iv-s5-def-2 .statement}

*A subset* $A$ *of* $X$ *is said to be measurable if its characteristic function* $\varphi_A$ *is measurable*.

In view of Def. 1, it comes to the same to say that a measurable set $A$ is a set such that, for every compact set $K$, there exist a negligible set $N \subset K$ and a partition $(K_n)$ of $K - N$ formed by a sequence of compact sets each of which is contained either in $K \cap A$ or in $K \cap \complement A$.

This definition yields at once the following criterion:

#### Proposition 3 {#int-iv-s5-prop-3 .statement}

*For a set* $A$ *to be measurable, it is necessary and sufficient that, for every compact set* $K$, $A \cap K$ *be integrable*.

The condition is necessary, because the union of a sequence of integrable sets $A_n$ is integrable when $\sum_n |\mu|(A_n)$ is finite (§ 4, No. 5, Cor. of Prop. 8). The condition is sufficient because, for every integrable set $B$, there exist a negligible set $N \subset B$ and a partition of $B - N$ into a sequence of compact sets (§ 4, No. 6, Cor. 2 of Th. 4).

#### Corollary 1 {#int-iv-s5-prop-3-cor-1 .statement}

*The open sets and the closed sets are measurable*.

In particular, the entire space $X$ is measurable.

#### Corollary 2 {#int-iv-s5-prop-3-cor-2 .statement}

— *If X is metrizable, then every Souslin subset A of X* (GT, IX, §6, No. 2) *is μ-measurable for every measure μ on X*.

By virtue of Prop. 3, it suffices to verify that every relatively compact Souslin set A is μ-integrable. Now, such a set A is capacitable for $|\mu|^*$ (GT, IX, §6, No. 9, Th. 5). Therefore, for every $ε > 0$ there exists a compact subset K of A such that $|\mu|^*(A) \leq |\mu|^*(K) + ε = |\mu|(K) + ε$. Let U be a relatively compact open set in X containing A such that

$$
|\mu|(U) = |\mu|^*(U) \leq |\mu|^*(A) + ε.
$$

Then $|\mu|^*(U - K) = |\mu|(U) - |\mu|(K) \leq 2ε$, therefore $|\mu|^*(A - K) \leq 2ε$, which proves that A is μ-integrable (§4, No. 6, Cor. 1 of Th. 4).

### 2. Principle of localization. Locally negligible sets

#### Proposition 4 (Principle of localization) {#int-iv-s5-prop-4 .statement}

— *Let f be a mapping of X into a topological space F. Suppose that for every $x \in X$, there exist an integrable neighborhood $V_x$ of x and a measurable mapping $g_x$ of X into F such that $f(y) = g_x(y)$ almost everywhere in $V_x$. Then f is measurable.*

Let K be a compact set; there exists a finite number of points $x_i \in K$ such that the $V_{x_i}$ form a covering of K. It follows at once (§4, No. 9, Lemma) that there exist a negligible set $N \subset K$ and a finite partition of $K - N$ formed of integrable sets $M_j$ such that each of the sets $K \cap V_{x_i}$ is the union of a subset of N and a certain number of the $M_j$, and such that on each of the $M_j$, $f$ is equal to one of the functions $g_{x_i}$. Now, for each $M_j$ there exist a negligible set $N_j \subset M_j$ and a partition of $M_j - N_j$ formed by a sequence of compact sets $K_{nj}\ (\mathbf{n} \in \mathbf{N})$; on the other hand, for each $K_{nj}$ there exist a negligible set $P_{nj} \subset K_{nj}$ and a partition of $K_{nj} - P_{nj}$ formed by a sequence of compact sets $K_{mnj}\ (\mathbf{m} \in \mathbf{N})$ such that the restriction of $f$ to each of the $K_{mnj}$ is continuous. Since the union of N, the $N_j$ and the $P_{nj}$ is negligible, $f$ is measurable.

The concept of measurable function is therefore a concept of local character.

#### Definition 3 {#int-iv-s5-def-3 .statement}

— *A set $A \subset X$ is said to be locally negligible (for the measure $μ$) if, for every $x \in X$, there exists a neighborhood $V$ of $x$ such that $V \cap A$ is negligible.*

By the principle of localization, every locally negligible set is *measurable*. The properties of negligible sets (§2) show that every subset of a locally negligible set is locally negligible, and that every countable union of locally negligible sets is locally negligible.

#### Proposition 5 {#int-iv-s5-prop-5 .statement}

— *For a set A to be locally negligible, it is necessary and sufficient that, for every compact set K, $A \cap K$ be negligible.*

The condition is obviously sufficient since every point of X has a compact neighborhood. It is necessary, because if, for every $x \in K$, there exists a neighborhood $V_x$ of $x$ such that $A \cap V_x$ is negligible, then there exists a finite number of points $x_i \in K$ such that the $V_{x_i}$ form a covering of K, and $A \cap K$ is contained in the union of the negligible sets $A \cap V_{x_i}$.

#### Corollary 1 {#int-iv-s5-prop-5-cor-1 .statement}

— *For a set A to be negligible, it is necessary and sufficient that it be locally negligible and of finite outer measure.*

The condition is obviously necessary. Conversely, if it is satisfied then A is contained in an integrable open set G, which is the union of a negligible set N and a sequence $(K_n)$ of compact sets (§ 4, No. 6, Cor. 2 of Th. 4); since $A \cap N$ and the sets $A \cap K_n$ are negligible, the same is true of their union A.

#### Corollary 2 {#int-iv-s5-prop-5-cor-2 .statement}

— *Every locally negligible open set is negligible* (and is therefore contained in the complement of the support of $\mu$).

For, the outer measure of an open set G is the supremum of the measures $|\mu|(K)$ of the compact sets $K \subset G$ (§ 4, No. 6, Cor. 4 of Th. 4); if G is locally negligible then $|\mu|(K) = 0$ for every compact set K contained in G, therefore $|\mu|^*(G) = 0$.

#### Corollary 3 {#int-iv-s5-prop-5-cor-3 .statement}

— *In a locally compact space X that is countable at infinity, every locally negligible set is negligible.*

Since X is the union of a sequence $(K_n)$ of compact sets, every locally negligible set A is the union of the negligible sets $A \cap K_n$, hence is negligible.

One can give examples of locally compact spaces that are not countable at infinity, and of measures on such a space X such that there exist sets in X that are locally negligible but not negligible (§ 1, Exer. 5).

#### Corollary 4 {#int-iv-s5-prop-5-cor-4 .statement}

— *Let f be a mapping of X into a topological space F. If the set N of points of discontinuity of f is locally negligible, then f is measurable.*

For every compact set $K \subset X$, $K \cap N$ is negligible (Prop. 5), therefore, for every $\varepsilon > 0$, there exists a compact set $K_1 \subset K - (K \cap N)$ such that $|\mu|(K - K_1) \leq \varepsilon$ (§ 4, No. 6, Th. 4), and by hypothesis the restriction of f to $K_1$ is continuous, whence the conclusion.

If $P\{x\}$ is a property, the property « *P\{x\} locally almost everywhere (with respect to $\mu$)» is by definition equivalent to the property «*the set of x such that* (x $\in$ X and not $P\{x\}$) *is locally negligible (for the measure* $\mu$)». If F is any set, the relation «$f(x) = g(x)$ locally almost everywhere» is an equivalence relation in the set of mappings of X into F. In particular, if F is a vector space, a mapping $f$ of X into F such that f(x) = 0\text{ locally almost everywhere is said to be } \textit{locally negligible}. We leave to the reader the task of establishing for these concepts most of the properties corresponding to those that have been enumerated in §2, Nos. 4, 5 and 6 for functions equal almost everywhere. We shall limit ourselves to observing that if two \emph{continuous} mappings $f, g$ of X into a Hausdorff topological space F are equal \emph{locally almost everywhere}, then they are equal \emph{almost everywhere} by virtue of Cor. 2 of Prop. 5 (hence are equal at every point of the support of $\mu$ (§ 2, No. 4, Prop. 9)); however, we state explicitly the following proposition, which is an immediate consequence of the principle of localization:

#### Proposition 6 {#int-iv-s5-prop-6 .statement}

*Let $f$ be a measurable mapping of X into a topological space F. Every mapping of X into F, equal to $f$ locally almost everywhere, is measurable.*

### 3. Elementary properties of measurable functions

#### Theorem 1 {#int-iv-s5-thm-1 .statement}

*Let X be a locally compact space, $\mu$ a measure on X, $(F_n)$ a sequence of topological spaces, $F = \prod_n F_n$ their product. For each index n, let $f_n$ be a measurable mapping of X into $F_n$, and let $f(x) = (f_n(x)) \in F$; then, for every continuous mapping u of $f(X)$ into a topological space G, the function $x \mapsto u(f(x))$ is measurable.*

For every compact subset K of X and every number $\varepsilon > 0$, there exists a compact set $K_1 \subset K$ such that $|\mu|(K - K_1) \leq \varepsilon$ and such that the restrictions to $K_1$ of all the functions $f_n$ are continuous (No. 1, Prop. 2); it is clear that $u \circ f$ is continuous on $K_1$, whence the theorem.

#### Remark {#int-iv-s5-n3-rem-1 .statement}

— 1) The theorem does not extend to an \emph{arbitrary} product of topological spaces (Exer. 1).
2) If $f$ is a continuous mapping of X into itself, and $g$ is a measurable mapping of X into F, then $g \circ f$ is not necessarily measurable (Exer. 2).

#### Corollary 1 {#int-iv-s5-thm-1-cor-1 .statement}

*The upper envelope and the lower envelope of a finite number of measurable numerical functions (finite or not) are measurable.*
For, $\sup(u, v)$ and $\inf(u, v)$ are continuous on $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$.

#### Corollary 2 {#int-iv-s5-thm-1-cor-2 .statement}

*For a numerical function $f$ (finite or not) to be measurable, it is necessary and sufficient that $f^+$ and $f^-$ be measurable.*
The condition is necessary by Cor. 1; it is sufficient because the image A of X in $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ under the mapping $x \mapsto (f^+(x), f^-(x))$ does not contain the points $(+\infty, +\infty)$ and $(-\infty, -\infty)$, consequently the mapping $(u, v) \mapsto u - v$ is continuous on A.

#### Corollary 3 {#int-iv-s5-thm-1-cor-3 .statement}

— *If f and g are two measurable mappings of X into a topological vector space F, then f + g and αf are measurable (α any scalar).*

The set of measurable mappings of X into a topological vector space F is thus a vector space.

#### Corollary 4 {#int-iv-s5-thm-1-cor-4 .statement}

— *Let F be a vector space of dimension n over R and let (e_k)_{1 \leq k \leq n} be a basis of F. In order that a function f = \sum_{k=1}^{n} e_k f_k be measurable, it is necessary and sufficient that each of the numerical functions f_k be measurable.*

#### Corollary 5 {#int-iv-s5-thm-1-cor-5 .statement}

— *Let F, G, H be three topological vector spaces, and let (u, v) \to [u \cdot v] be a continuous bilinear mapping of F \times G into H. If f is a measurable mapping of X into F, and g is a measurable mapping of X into G, then [f \cdot g] is a measurable mapping of X into H.*

In particular, if f is a measurable mapping of X into a real (resp. complex) normed space F, and g is a measurable mapping of X into R (resp. C), then gf is measurable. If F is a *normed algebra* and f, g are two measurable mappings of X into F, then fg is measurable.

#### Corollary 6 {#int-iv-s5-thm-1-cor-6 .statement}

— *If f is a measurable mapping of X into a normed space F, then the numerical function |f| is measurable.*

### 4. Limits of measurable functions

#### Theorem 2 (Egoroff) {#int-iv-s5-thm-2 .statement}

— *Let X be a locally compact space, μ a measure on X, A a countable set, $\mathfrak{F}$ a filter on A having a countable base, and $(f_\alpha)_{\alpha \in A}$ a family of measurable mappings of X into a metrizable space F. Assume that $\lim_{\mathfrak{F}} f_\alpha(x) = f(x)$ exists in the complement of a locally negligible subset N of X. Under these conditions,
1° the function f (extended to N in any manner whatsoever) is measurable;
2° for every compact subset K of X and every $\varepsilon > 0$, there exists a compact set $K_1 \subset K$ such that $|\mu|(K - K_1) \leq \varepsilon$ and such that the restrictions of the $f_\alpha$ to $K_1$ are continuous and converge uniformly to f on $K_1$.

The first assertion obviously follows from the second, which we are going to prove. There exists a compact set $K_0 \subset K$ such that $|\mu|(K - K_0) \leq \varepsilon/2$ and such that the restrictions to $K_0$ of all the functions $f_\alpha$ are continuous (No. 1, Prop. 2). Let $(A_n)$ be a decreasing countable base for the filter $\mathfrak{F}$; let d be a metric on F compatible with the topology. For every pair of integers $n > 0,\ r > 0$, let $B_{n,r}$ be the set of points $x \in K_0$ such that, for at least one pair of indices $\alpha, \beta$ belonging to $A_n$, $d(f_\alpha(x), f_\beta(x)) \geq 1/r$; for fixed $\alpha$ and $\beta$, the set of $x \in K_0$ such that $d(f_\alpha(x), f_\beta(x)) \geq 1/r$ is closed in $K_0$, hence is compact; consequently, $B_{n,r}$ is a countable union of compact sets contained in $K_0$, hence is integrable (§ 4, No. 5, Props. 6 and 8). If $r$ is fixed, the intersection of the decreasing sequence of sets $B_{n,r}$ ($n = 1, 2, \ldots$) has measure zero, since $f_\alpha(x)$ tends to $f(x)$ almost everywhere in $K_0$ with respect to the filter $\mathfrak{F}$; thus $\lim_{n \to \infty} |\mu|(B_{n,r}) = 0$ (§ 4, No. 5, Cor. of Prop. 7), consequently there exists an integer $n_r$ such that $|\mu|(B_{n_r,r}) \leq \varepsilon/2^{r+2}$. Let $B$ be the union (for $r = 1, 2, \ldots$) of the sets $B_{n_r,r}$; $B$ is integrable and

$$
|\mu|(B) \leq \sum_{r=1}^\infty |\mu|(B_{n_r,r}) \leq \varepsilon/4
$$

(§ 4, No. 5, Cor. of Prop. 8). Let $C$ be the complement of $B$ in $K_0$; by construction, $f_\alpha(x)$ converges uniformly to $f(x)$ in $C$ with respect to the filter $\mathfrak{F}$, and since the restrictions of the $f_\alpha$ to $C$ are continuous, so is the restriction of $f$ to $C$. It then suffices to take a compact set $K_1 \subset C$ such that $|\mu|(C - K_1) \leq \varepsilon/4$ in order to satisfy the conditions of the statement, since $|\mu|(K - K_1) = |\mu|(K - K_0) + |\mu|(B) + |\mu|(C - K_1) \leq \varepsilon$.

The conclusions of Th. 2 do not necessarily hold if $F$ is not metrizable (Exer. 1). If $F$ is metrizable, and the set $A$ is not countable but the filter $\mathfrak{F}$ has a countable base, then the first conclusion of Th. 2 is again valid; for, if $(A_n)$ is a countable base for $\mathfrak{F}$ and $\alpha_n$ is an element of $A_n$, then $f$ is the limit of the sequence $(f_{\alpha_n})$ locally almost everywhere, hence is measurable; however, the second conclusion of Th. 2 is no longer necessarily valid (cf. Exer. 4).

#### Corollary 1 {#int-iv-s5-thm-2-cor-1 .statement}

— *Let* $(f_n)$ *be a sequence of numerical functions (finite or not)*. *If the* $f_n$ *are measurable, then the functions* $\sup_n f_n$, $\inf_n f_n$, $\limsup_{n \to \infty} f_n$ *and* $\liminf_{n \to \infty} f_n$ *are measurable*.

For, the extended real line $\overline{\mathbf{R}}$, being homeomorphic to a compact interval of $\mathbf{R}$, is metrizable. The function $\sup_n f_n$ is the pointwise limit of the increasing sequence of functions $g_n = \sup(f_1, f_2, \ldots, f_n)$, which are measurable (No. 3, Cor. 1 of Th. 1); similarly, $\limsup_{n \to \infty} f_n$ is the pointwise limit of the decreasing sequence of functions $h_n = \sup_{p \geq 0} f_{n+p}$, each of which is measurable by the foregoing. Finally, since $\inf_n f_n = -\sup(-f_n)$ and $\liminf_{n \to \infty} f_n = -\limsup_{n \to \infty} (-f_n)$, these functions are measurable.

#### Corollary 2 {#int-iv-s5-thm-2-cor-2 .statement}

— *The measurable sets in* $X$ *form a tribe* (GT, IX, §6, No. 3).

For, if M and N are measurable then the functions

$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N \quad \text{and} \quad \varphi_{M \cap C_N} = \varphi_M - \varphi_M \varphi_N
$$

are measurable by No. 3, Cors. 3 and 5 of Th. 1. If $(M_n)$ is a sequence of measurable sets and M is their union, then $\varphi_M = \sup_n \varphi_{M_n}$ is measurable by Cor. 1 of Th. 2, whence the corollary.

In particular, since the open sets are measurable:

#### Corollary 3 {#int-iv-s5-thm-2-cor-3 .statement}

*The Borel sets in X* (GT, IX, §6, No. 3, Def. 4) *are $\mu$-measurable for every measure $\mu$ on X*.

### 5. Criteria for measurability

When F is a topological vector space, every step function over the measurable sets (§4, No. 9, Def. 4), with values in F, is obviously measurable (No. 3, Cor. 3 of Th. 1); such a function $f$ takes on only a finite number of values, and for every $y \in F$, $f^{-1}(y)$ is measurable. More generally, let F be any topological space, $f$ a mapping of X into F taking on only a finite number of distinct values $a_i$ ($1 \leq i \leq m$); if the sets $A_i = f^{-1}(a_i)$ are measurable, then the function $f$ is measurable. For, for every compact set K and for each of the sets $A_i \cap K$, there exist a negligible set $N_i \subset A_i \cap K$ and a partition of $A_i \cap K \cap C N_i$ formed by a sequence $(K_{in})$ of compact sets; since K is the union of the sets $A_i \cap K$ and the restriction of $f$ to each of the $K_{in}$ is constant, therefore continuous, $f$ is measurable. By an abuse of language we shall say that a mapping $f$ of X into F is a *measurable step function* if it takes on only a finite number of values and if, for every $y \in F$, $f^{-1}(y)$ is measurable.

#### Theorem 3 {#int-iv-s5-thm-3 .statement}

*For a mapping $f$ of X into a metrizable space F to be measurable, it is necessary and sufficient that, for every compact set $K \subset X$, there exist a sequence $(g_n)$ of measurable step functions, with values in F, such that $g_n(x)$ tends to $f(x)$ for almost every $x \in K$*.

The condition is sufficient by Egoroff’s theorem and the principle of localization. Let us show that it is necessary: by hypothesis, there exist a negligible set $N \subset K$ and a partition $(K_m)$ of $K - N$ formed of compact sets such that the restriction of $f$ to each $K_m$ is continuous. To define the sequence $(g_n)$, it suffices to proceed in the following manner: let $d$ be a metric compatible with the topology of F; for each $K_i$ with index $i \leq n$, there exists a finite partition of $K_i$ into integrable sets $A_{ij}$ ($1 \leq j \leq q_i$) sufficiently small that the oscillation of $f$ on each of the $A_{ij}$ is $\leq 1/n$ (§ 4, No. 9, Lemma); take $g_n$ to be constant on each $A_{ij}$, equal to one of the values of $f$ in this set (for $1 \leq i \leq n,\ 1 \leq j \leq q_i$), and equal to a fixed element $a \in \mathbf{F}$ for every point of $X$ that does not belong to any of the $A_{ij}$. It is clear that the sequence $(g_n(x))$ converges to $f(x)$ at every point of $K$ not belonging to $N$.

#### Corollary 1 {#int-iv-s5-thm-3-cor-1 .statement}

*Let $f$ be a measurable mapping of $X$ into a Banach space $F$; for every compact set $K \subset X$, there exists a sequence $(g_n)$ of measurable step functions, with supports contained in $K$, such that $|g_n(x)| \leq |f(x)|$ for all $x \in X$ and such that $g_n(x)$ tends to $f(x)$ for almost every $x \in K$.*

With notations as in the proof of Th. 3, and denoting by $a_{ij}$ one of the values of $f$ in $A_{ij}$, it suffices to take, as the value of $g_n$ in $A_{ij}$, the point 0 if $|a_{ij}| \leq 1/n$ and the point $a_{ij}(1 - 1/(n|a_{ij}|))$ otherwise; finally, set $g_n(x) = 0$ on the complement of the union of the $A_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq q_i$).

#### Corollary 2 {#int-iv-s5-thm-3-cor-2 .statement}

*Let $X$ be a locally compact space that is countable at infinity. If $f$ is a measurable mapping of $X$ into a metrizable space $F$, then there exists a sequence $(g_n)$ of measurable step functions, with values in $F$, such that $g_n(x)$ tends to $f(x)$ for almost every $x \in X$.*

If $X$ is the union of an increasing sequence $(A_n)$ of compact sets, the sets $A_n - A_{n-1}$ that are nonempty form a partition of $X$ into integrable sets; consequently, there exist a negligible set $N \subset X$ and a partition of $\mathbf{C}N$ formed by a sequence $(K_n)$ of compact sets such that the restriction of $f$ to each $K_n$ is continuous; the proof can then be concluded as in Th. 3 without modification.

#### Proposition 7 {#int-iv-s5-prop-7 .statement}

*Let $f$ be a measurable mapping of $X$ into a topological space $F$; the inverse image under $f$ of every closed (resp. open) set in $F$ is measurable.*

It suffices to carry out the proof for the inverse image $^{-1}f(A)$ of a closed set $A$ in $F$. Let $K$ be a compact subset of $X$; there exist a negligible set $N \subset K$ and a partition $(K_n)$ of $K - N$ formed of compact sets such that the restriction of $f$ to each $K_n$ is continuous. The intersection $K_n \cap ^{-1}f(A)$ is thus the inverse image of the closed set $A$ under the restriction of $f$ to $K_n$; it is therefore a closed set in $K_n$, hence is compact. The set $K \cap ^{-1}f(A)$ is therefore the union of the negligible set $N \cap ^{-1}f(A)$ and the compact sets $K_n \cap ^{-1}f(A)$, which proves that $^{-1}f(A)$ is measurable.

#### Theorem 4 {#int-iv-s5-thm-4 .statement}

— Let F be a metrizable space and let d be a metric on F compatible with the topology. For a mapping f of X into F to be measurable, it is necessary and sufficient that it satisfy the following two conditions:
a) the inverse image under f of every closed ball of F is measurable;
b) for every compact set K ⊂ X, there exists a countable subset H of F such that $f(x) \in \overline{H}$ for almost every $x \in K$.

The condition a) is necessary by Prop. 7; on the other hand, in the notations of Th. 3, condition b) is satisfied by taking H to be the countable set formed by the values of all of the functions $g_n$.

Let us now show that the conditions a) and b) are sufficient. Let K be any compact subset of X; there exists a negligible subset N of K such that $f(K - N)$ is contained in the closure of a countable set of points of F, which we arrange in a sequence $(a_n)$. Let $A_{n,p}$ be the set of $x \in K - N$ such that $d(f(x), a_n) \leq 1/p$. It follows from condition a) that $A_{n,p}$ is measurable. For fixed $p$, define a sequence of sets $B_{n,p} \subset K - N$ recursively by setting

$$
B_{1,p} = A_{1,p} \quad \text{and} \quad B_{n+1,p} = A_{n+1,p} \cap C \left( \bigcup_{k \leq n} A_{k,p} \right);
$$

the sets $B_{n,p}$ are measurable, and those that are nonempty form a partition of $K - N$. Let $g_{m,p}$ be the function equal to $a_i$ on the set $B_{i,p}$ for $1 \leq i \leq m$ and equal to a constant $b \in F$ on the complement of the union of these sets; $g_{m,p}$ is a measurable step function; as $m$ tends to infinity, $g_{m,p}$ converges pointwise to the function $f_p$ equal to $a_n$ on $B_{n,p}$ ($n \geq 1$) and to $b$ on $N \cup C K$, therefore (Th. 2) $f_p$ is measurable. As $p$ tends to infinity, $f_p(x)$ tends to $f(x)$ for every $x \in K - N$, and to $b$ for $x \in N \cup C K$; the limit of the $f_p$ is therefore measurable, and the principle of localization proves that $f$ itself is measurable.

#### Remark 1 {#int-iv-s5-n5-rem-1 .statement}

Condition a) alone is not sufficient for $f$ to be measurable (Exer. 7).

#### Remark 2 {#int-iv-s5-n5-rem-2 .statement}

If the topology of F has a countable base then condition b) of Th. 4 is automatically satisfied for every mapping of X into F. The proof shows, moreover, that it suffices to assume that the inverse images under $f$ of the closed balls with rational radii, whose centers belong to a dense countable subset of F, are measurable sets.

#### Remark 3 {#int-iv-s5-n5-rem-3 .statement}

The hypothesis a) can be replaced by the condition that the inverse image under $f$ of every open ball of F is measurable.

The case of numerical functions (finite or not) deserves special mention:

#### Proposition 8 {#int-iv-s5-prop-8 .statement}

— Let D be a countable dense subset of $\mathbf{R}$. In order that a numerical function $f$ (finite or not) be measurable, it is sufficient (and necessary) that for every $a \in D$, the set of $x \in X$ such that $f(x) \geq a$ be measurable.

For, if this is so, for every $b \in \overline{\mathbf{R}}$ the set of $x$ such that $f(x) \geqslant b$ is measurable, being the intersection of the sets (which form a countable family) of the $x$ such that $f(x) \geqslant a$, as $a$ runs over the set of points of D that are $\leqslant b$. The set of $x$ such that $f(x) < b$ is measurable, being the complement of a measurable set. Next, if $b$ is finite then the set of $x$ such that $f(x) \leqslant b$ is measurable, being the intersection of the sets of the $x$ such that $f(x) < b + 1/n$; and $f(-\infty)^{-1}$ is measurable, being the intersection of the sets of the $x$ such that $f(x) < n$, as $n$ runs over $\mathbf{Z}$. Finally, the inverse image under $f$ of every closed interval of $\overline{\mathbf{R}}$ is measurable, being the intersection of two measurable sets, and Th. 4 may be applied.

One could show similarly that it suffices that for every $a \in \mathrm{D}$, the set of $x$ such that $f(x) > a$ be measurable.

#### Corollary {#int-iv-s5-n5-cor-1 .statement}

— *Every lower* (resp. *upper*) *semi-continuous function is measurable*.

For, if $f$ is lower semi-continuous, then the set of $x \in \mathrm{X}$ such that $f(x) \leqslant a$ is closed for every $a \in \overline{\mathbf{R}}$.

When F is metrizable and *compact*, Prop. 7 makes it possible to sharpen Th. 3 as follows:

#### Proposition 9 {#int-iv-s5-prop-9 .statement}

— *If F is a metrizable compact space, then every measurable mapping f of X into F is the uniform limit (on all of X) of a sequence of measurable step functions*.

Let $d$ be a metric compatible with the topology of F. For every positive integer $n$ there exists a *finite* number of points $a_k \in \mathrm{F}$ such that the closed balls $B_k$ with center $a_k$ and radius $1/n$ form a covering of F; the sets $A_k = f^{-1}(B_k)$ are therefore measurable (Prop. 7) and form a covering of X. Consequently (§ 4, No. 9, Lemma) there exists a partition $(C_i)$ of X into a finite number of measurable sets such that each $A_k$ is the union of certain of the $C_i$. Let $c_i$ be a point of $C_i$ and let $g_n$ be the measurable step function equal to $f(c_i)$ on $C_i$ (for each index $i$). It is clear that $d(f(x), g_n(x)) \leqslant 2/n$ for all $x \in \mathrm{X}$.

#### Proposition 10 {#int-iv-s5-prop-10 .statement}

— *Let F be a separable Banach space, F' its dual, and $(\mathbf{a}'_n)$ a weakly dense sequence in the unit ball of F' (TVS, III, § 3, No. 4, Cor. 2 of Prop. 6).*¹ *For a mapping f of X into F to be measurable, it is necessary and sufficient that for every n the scalar function $x \mapsto \langle \mathbf{f}(x), \mathbf{a}'_n \rangle$ be measurable*.

The condition being obviously necessary (No. 3, Th. 1), let us prove that it is sufficient; it suffices to verify condition a) of Th. 4 and, to this end,

¹ See the footnote at the end of § 2, No. 4.

it will suffice by the principle of localization to prove that, for every compact subset K of X and every closed ball $B \subset F$, with center $a$ and radius $r$, the set $A = K \cap f^{-1}(B)$ is measurable; now, for every $z \in F$,

$$
|z| = \sup_n |\langle z, a'_n \rangle| / |a'_n|;
$$

$A$ is thus the intersection of $K$ and the sets defined by

$$
|\langle f(x), a'_n \rangle - \langle a, a'_n \rangle| \leq r |a'_n|;
$$

as these sets are measurable by hypothesis, $A$ is measurable.

#### Corollary 1 {#int-iv-s5-prop-10-cor-1 .statement}

*Let F be a Banach space. In order that a mapping f of X into F be measurable, it is necessary and sufficient that it satisfy the following two conditions:*

a) *for every $a' \in F'$, the scalar function $x \mapsto \langle f(x), a' \rangle$ is measurable;*

b) *for every compact set $K \subset X$, there exists a countable subset H of F such that $f(x) \in \overline{H}$ for almost every $x \in K$.*

The necessity of the conditions follows from No. 3, Th. 1, and Th. 4. To prove that the conditions are sufficient, it again suffices to verify condition a) of Th. 4. With notations as in the proof of Prop. 10, we may (on account of b)) suppose, after modifying $f$ if necessary on a negligible set, that $f(K) \subset \overline{H}$, where $H$ is a countable subset of $F$. If $V$ is the closed linear subspace of $F$ generated by the set $H \cup \{a\}$, then $V$ is a separable Banach space and every continuous linear form on $V$ is the restriction of a form $a' \in F'$; the same reasoning as in Prop. 10 then shows that $K \cap f^{-1}(B)$ is measurable.

#### Corollary 2 {#int-iv-s5-prop-10-cor-2 .statement}

*Let F be a locally convex space that is metrizable and separable, and let $F'$ be its dual. For a mapping f of X into F to be measurable, it is necessary and sufficient that for every $a' \in F'$, the scalar function $x \mapsto \langle f(x), a' \rangle$ be measurable.*

We may regard F as a subspace of a countable product $\prod_n E_n$ of Banach spaces (TVS, II, §4, No. 3), and we can suppose that $\operatorname{pr}_n(F)$ is dense in $E_n$, which is therefore separable. For every $n$, the mapping $\operatorname{pr}_n \circ f$ is then measurable by Prop. 10, therefore $f$ is measurable by No. 3, Th. 1.

#### Proposition 11 {#int-iv-s5-prop-11 .statement}

*Let F be a locally convex space that is the direct limit of a sequence of separable metrizable locally convex spaces $F_n$, F being the union of the $F_n$. Let $F'$ be the dual of F, equipped with the weak topology $\sigma(F', F)$. For a mapping f of X into $F'$ to be measurable, it is necessary and sufficient that, for every $a \in F$, the scalar function $x \mapsto \langle a, f(x) \rangle$ be measurable.*

The condition is necessary by No. 3, Th. 1; let us prove that it is sufficient. Suppose first that F is metrizable and separable, and let D be a countable dense set in F. Let $(V_n)$ be a decreasing fundamental sequence of balanced convex open neighborhoods of 0 in F; the polar sets $V_n^\circ$ are equicontinuous and their union is all of $F'$. Let $X_n = f^{-1}(V_n^\circ)$; the sequence $(X_n)$ is increasing and $X = \bigcup_n X_n$; let us show that each $X_n$ is $\mu$-measurable. Indeed, $D \cap V_n$ is dense in $V_n$; for every $y \in D \cap V_n$ let $S_y$ be the set of $x \in X$ such that $|\langle y, f(x) \rangle| \leq 1$; the hypothesis implies that each of the $S_y$ is measurable, and $X_n$ is the intersection of the countable family of $S_y$ for $y \in D \cap V_n$. This being so, for every compact subset K of X and every $\varepsilon > 0$, there exists an integer n such that $|\mu|(K - (K \cap X_n)) \leq \varepsilon/4$, and then a compact subset $K_1$ of $K \cap X_n$ such that $|\mu|((K \cap X_n) - K_1) \leq \varepsilon/4$; finally, there exists a compact subset $K_2$ of $K_1$ such that $|\mu|(K_1 - K_2) \leq \varepsilon/2$ and such that the restrictions to $K_2$ of all of the functions $\langle y, f \rangle$, where $y \in D$, are continuous (No. 1, Prop. 2). Since the set $f(K_2) \subset f(X_n) \subset V_n^\circ$ is equicontinuous, the topology induced by $\sigma(F', F)$ on $f(K_2)$ is identical to the topology of pointwise convergence in D (GT, X, §2, No. 4, Th. 1); the restriction of f to $K_2$ is therefore continuous, whence our assertion in this first case.

Let us pass to the general case. If $z'$ is a continuous linear form on F, its restriction $z'_n$ to $F_n$ is continuous; since $F = \bigcup_n F_n$, the dual $F'$ of F may be identified (algebraically) with a linear subspace of the product $\prod_n F'_n$, and then $\operatorname{pr}_n(z') = z'_n$. Moreover, since each finite subset of F is contained in one of the $F_n$, the topology $\sigma(F', F)$ is none other than the topology induced by the product topology of the topologies $\sigma(F'_n, F_n)$. This being so, if $\langle a, f \rangle$ is measurable for every $a \in F$, then so is $\langle a_n, \operatorname{pr}_n \circ f \rangle$ for every n and every $a_n \in F_n$, since $\langle a_n, \operatorname{pr}_n \circ f \rangle = \langle a_n, f \rangle$; the first part of the proof then shows that $\operatorname{pr}_n \circ f$ is measurable for every n, therefore so is f (No. 3, Th. 1).

### 6. Criteria for integrability

#### Theorem 5 {#int-iv-s5-thm-5 .statement}

— In order that a mapping f of X into a Banach space F be p-th power integrable ($1 \leq p < +\infty$), it is necessary and sufficient that f be measurable and that $N_p(f)$ be finite.

The condition is necessary: for, if $f \in \mathcal{L}_F^p$ then there exists a sequence $(g_n)$ of continuous functions with compact support that converges almost everywhere to f ($§ 3$, No. 4, Cor. 2 of Th. 3); by Th. 2 of No. 4, f is measurable.

To prove that the conditions are sufficient, we first establish a lemma:

#### Lemma 1 {#int-iv-s5-lem-1 .statement}

*Let g be a function with values in F, such that N_p(g) < +\infty* (in other words, a function in $\mathcal{F}_F^p$). *The set A of points x \in X such that g(x) \neq 0 is contained in the union of a negligible set and a sequence of compact sets.*

Let $A_n$ be the set of points $x \in X$ such that $|g(x)| \geq 1/n$; A is the union of the $A_n$, and $\varphi_{A_n} \leq n|g|$, whence $|\mu|^*(A_n) \leq (n N_p(g))^p$; it follows that $A_n$ is contained in the union of a negligible set and a sequence of compact sets (§ 4, No. 6, Cor. 3 of Th. 4), therefore so is A.

The lemma proved, consider first the case that f has *compact* support K. By Cor. 1 of Th. 3 of No. 5, there exists a sequence $(g_n)$ of measurable step functions such that $|g_n(x)| \leq |f(x)|$ at every point $x \in X$ and such that $g_n(x)$ tends to $f(x)$ almost everywhere. Now, $g_n$ is a linear combination of characteristic functions of measurable sets contained in K; since these sets are integrable by Prop. 3 of No. 1, $g_n$ belongs to $\mathcal{L}_F^p$. Since $N_p(f) < +\infty$, Lebesgue’s theorem (§ 3, No. 7, Th. 6) shows that f belongs to $\mathcal{L}_F^p$.

In the general case, it follows from Lemma 1 that there exists an increasing sequence $(K_n)$ of compact sets such that $f(x)$ is zero almost everywhere in the complement of the union of the $K_n$. Let $f_n$ be the function equal to $f(x)$ on $K_n$ and to 0 elsewhere; $f_n$ is measurable by No. 3, Cor. 5 of Th. 1; since $|f_n| \leq |f|$, $f_n$ belongs to $\mathcal{L}_F^p$ by the first part of the argument. Since $f(x)$ is equal almost everywhere to the limit of the sequence $f_n(x)$, Lebesgue’s theorem again proves that $f \in \mathcal{L}_F^p$, which completes the proof.

One should take care to note that a function that is *locally negligible but not negligible* is not integrable; thus, a function equal *locally almost everywhere* to an integrable function is not necessarily integrable.

#### Corollary 1 {#int-iv-s5-lem-1-cor-1 .statement}

*For a set to be integrable, it is necessary and sufficient that it be measurable and have finite outer measure.*

#### Corollary 2 {#int-iv-s5-lem-1-cor-2 .statement}

*Let $(F_n)$ be a sequence of topological spaces; for every index n, let $f_n$ be a measurable mapping of X into $F_n$ and let $f(x) = (f_n(x)) \in F = \prod_n F_n$; finally, let u be a continuous mapping of $f(X)$ into a Banach space G. For the function $g(x) = u(f(x))$ to be integrable, it is necessary and sufficient that $N_1(g) < +\infty$.*

For, g is measurable (No. 3, Th. 1).

#### Corollary 3 {#int-iv-s5-lem-1-cor-3 .statement}

*For every integrable function f and every measurable set A, the function $f \varphi_A$ is integrable.*

For, it follows from Th. 5 and No. 3, Cor. 5 of Th. 1 that $f \varphi_A$ is measurable, and $N_1(f \varphi_A) \leq N_1(f)$.

We write $\int_A f d\mu = \int f \varphi_A d\mu$ (or $\int_A f \mu$) for every integrable function $f$ and every measurable set $A$. We also write $\int^* f d|\mu|$ (or $\int^*_A f |\mu|$) in place of $\int^* f \varphi_A d|\mu|$ for every numerical function (finite or not) $f \geqslant 0$ (on setting $f(x)\varphi_A(x) = 0$ if $f(x) = +\infty$ and $\varphi_A(x) = 0$).

#### Corollary 4 {#int-iv-s5-lem-1-cor-4 .statement}

*For every sequence* $(f_n)$ *of measurable functions* $\geqslant 0$ *on* $X$,

$$
\int^*\left( \sum_n f_n \right) d|\mu| = \sum_n \int^* f_n d|\mu|.
$$

In view of §1, No. 3, Th. 3, we are reduced to proving that for any two measurable functions $f \geqslant 0, g \geqslant 0$ on $X$,

$$
\int^*(f + g) d|\mu| = \int^* f d|\mu| + \int^* g d|\mu|.
$$

This is nothing more than the additivity of the integral when $f$ and $g$ are integrable. In the contrary case, if for example $f$ is not integrable, then $\int^* f d|\mu| = +\infty$ by Th. 5; *a fortiori*, $\int^*(f + g) d|\mu| = +\infty$.

#### Corollary 5 {#int-iv-s5-lem-1-cor-5 .statement}

*For every sequence* $(A_n)$ *of pairwise disjoint measurable sets*,

$$
|\mu|^*\left( \bigcup_n A_n \right) = \sum_n |\mu|^*(A_n).
$$

This follows from Cor. 4 applied to the $\varphi_{A_n}$.

### 7. Measure induced on a locally compact subspace

Let $X$ be a locally compact space, $\mu$ a measure on $X$, and $Y$ a *locally compact subspace* of $X$. Since $Y$ is the intersection of an open set and a closed set in $X$ (GT, I, §9, No. 7, Prop. 12), it is $\mu$-measurable (No. 1, Cor. of Prop. 3). For every function $g \in \mathcal{H}(Y; \mathbf{C})$ let $g'$ be the function, defined on all of $X$, equal to $g$ on $Y$ and to 0 on $X - Y$; let us show that $g'$ is $\mu$-*integrable*. We can restrict ourselves to the case that $g$ is real and $\geqslant 0$ (on writing $g$ as a linear combination of such functions); since $g'$ is bounded and has compact support, it suffices to show that $g'$ is $\mu$-measurable (No. 6, Th. 5); but this follows from the fact that $g'$ is upper semi-continuous on $X$ (No. 5, Cor. of Prop. 8). We may therefore make the following definition:

#### Definition 4 {#int-iv-s5-def-4 .statement}

— *Given a locally compact subspace Y of a locally compact space X, we call measure induced on Y by a measure $\mu$ on X, and denote by $\mu_Y$ or $\mu|Y$, the measure defined by the formula*

$$
\int g \, d\mu_Y = \int g' \, d\mu
$$

*for every function $g \in \mathcal{K}(Y; \mathbf{C})$, where $g'$ denotes the function equal to $g$ on $Y$ and to 0 on $X - Y$.*

#### Example {#int-iv-s5-n7-exa-1 .statement}

— Let $\mu$ be Lebesgue measure on $\mathbf{R}$, I *any* interval in $\mathbf{R}$; I is a locally compact subspace of $\mathbf{R}$, and the measure induced by $\mu$ on I is the linear form

$$
g \mapsto \int_a^b g(x) \, dx
$$

on $\mathcal{K}(I; \mathbf{C})$, where $a$ and $b$ are the endpoints (finite or not) of I (cf. § 4, No. 4, *Example*), in other words, what we have called *Lebesgue measure on I*.

When Y is an *open* subspace of X, Def. 4 coincides with the definition of the measure induced by $\mu$ on Y (or the restriction of $\mu$ to Y) given in Ch. III, §2, No. 1: indeed, for every function $g \in \mathcal{K}(Y; \mathbf{C})$ the function $g'$ is then continuous on X.

We shall study integration with respect to an induced measure in detail in Ch. V, §7, and until then we shall need only the following results:

#### Lemma 2 {#int-iv-s5-lem-2 .statement}

— *Let $\mu$ be a positive measure on X, and let K be a compact subset of X.*

(i) *For every compact (resp. open) subset H of K*, $\mu_K(H) = \mu(H)$.

(ii) *For a subset N of K to be $\mu_K$-negligible, it is necessary and sufficient that it be $\mu$-negligible*.

(iii) *If S is the support of $\mu_K$, then* $\mathrm{Supp}(\mu_S) = S$.

(i) We can restrict ourselves to the case that H is compact. Denote by $f$ the characteristic function of H in the space K; $f$ is upper semi-continuous, hence is the lower envelope of a decreasing directed family $(g_\alpha)$ of functions in $\mathcal{K}_+(K)$; we have $\mu_K(H) = \inf_\alpha \int g_\alpha \, d\mu_K$ (§ 4, No. 4, Cor. 2 of Prop. 5). If $g'_\alpha$ is the function equal to $g_\alpha$ on K and to 0 on $X - K$, then $g'_\alpha$ is upper semi-continuous, and the lower envelope of the decreasing directed family $(g'_\alpha)$ is the characteristic function $\varphi_H$ of H in the space X; therefore

$$
\mu(H) = \inf_\alpha \int g'_\alpha \, d\mu = \inf_\alpha \int g_\alpha \, d\mu_K = \mu_K(H)
$$

by (1).

(ii) If N is $\mu$-negligible then, for every $\varepsilon > 0$, there exists a relatively compact open neighborhood U of N in X such that $\mu(U) \leq \varepsilon$; since $K - (U \cap K)$ is compact, it follows from (i) that $\mu_K(U \cap K) \leq \mu(U) \leq \varepsilon$, thus N is $\mu_K$-negligible. Conversely, if N is $\mu_K$-negligible then there exists an open neighborhood V of N in X such that $\mu_K(V \cap K) \leq \varepsilon$; by (i), we have $\mu(V \cap K) = \mu_K(V \cap K)$, therefore $\mu(N) = 0$ since $\varepsilon$ is arbitrary.

(iii) For every open set U in K that intersects S, by hypothesis $\mu_K(U \cap S) \neq 0$, therefore $\mu(U \cap S) \neq 0$ by (i), and since $U \cap S$ is open in S, $\mu_S(U \cap S) \neq 0$ by (i); since every nonempty open set in S is of the form $U \cap S$, where U is open in K, this proves that $\operatorname{Supp}(\mu_S) = S$.

#### Lemma 3 {#int-iv-s5-lem-3 .statement}

*Let Y be a locally compact subspace of X; for every measure $\mu$ on X, $|\mu_Y| = |\mu|_Y$.*

Let f be a function in $\mathcal{K}_+(Y)$ and $\varepsilon$ any number $> 0$; by definition, there exists a function $g \in \mathcal{K}(Y; \mathbf{C})$ such that $|g| \leq f$ and $|\mu_Y|(f) \leq |\mu_Y(g)| + \varepsilon$. Denoting by $f'$ and $g'$ the functions obtained by extending f and g, respectively, to be 0 on $X - Y$, we have $\mu_Y(g) = \mu(g')$ and, since $|g'| \leq f'$,

$$
|\mu(g')| \leq |\mu|(|g'|) \leq |\mu|(f') = |\mu|_Y(f),
$$

whence $|\mu_Y|(f) \leq |\mu|_Y(f) + \varepsilon$ and, since $\varepsilon$ is arbitrary,

$$
|\mu_Y|(f) \leq |\mu|_Y(f).
$$

On the other hand, let K be the support of f and let U be a compact neighborhood of K in X such that $|\mu|(U - K) \leq \varepsilon$; by Urysohn's theorem, there exists a function $f_1 \in \mathcal{K}_+(X)$, extending f, with support contained in U and such that $\|f_1\| = \|f\|$. There exists a function $h_1 \in \mathcal{K}(X; \mathbf{C})$ such that $|h_1| \leq f_1$ and $|\mu|(f_1) \leq |\mu(h_1)| + \varepsilon$. If h is the restriction of $h_1$ to Y, then $h \in \mathcal{K}(Y; \mathbf{C})$, $|h| \leq f$ and $\mu(h_1) - \mu_Y(h) = \mu(h_1 \varphi_{U-K})$, therefore

$$
|\mu(h_1) - \mu_Y(h)| \leq \|f\| \cdot |\mu|(U - K) \leq \varepsilon \|f\|;
$$

moreover, we have similarly

$$
|\mu|(f_1) - |\mu|_Y(f) = |\mu|(f_1 \varphi_{U-K}) \quad \text{and} \quad ||\mu|(f_1) - |\mu|_Y(f)|| \leq \varepsilon \|f\|.
$$

From this we infer that

$$
|\mu|_Y(f) \leq |\mu_Y(h)| + \varepsilon(1 + 2\|f\|) \leq |\mu_Y|(f) + \varepsilon(1 + 2\|f\|)
$$

and since $\varepsilon$ is arbitrary, $|\mu|_Y(f) \leq |\mu_Y|(f)$, which completes the proof.

### 8. $\mu$-dense families of compact sets

#### Proposition 12 {#int-iv-s5-prop-12 .statement}

— Let $\mu$ be a measure on a locally compact space $X$, $A$ a $\mu$-measurable subset of $X$, and $\mathcal{K}$ a set of compact subsets of $A$ satisfying the following conditions:
(PLI) Every closed (hence compact) subset of a set of $\mathcal{K}$ belongs to $\mathcal{K}$.
(PLII) Every finite union of sets of $\mathcal{K}$ belongs to $\mathcal{K}$.
The following four properties are then equivalent:
a) For a subset $B$ of $A$ to be locally $\mu$-negligible, it is necessary and sufficient that $|\mu|^*(B \cap K) = 0$ for all $K \in \mathcal{K}$.
b) For every compact subset $K_0$ of $A$ and every $\varepsilon > 0$, there exists a set $K \in \mathcal{K}$, contained in $K_0$ and such that $|\mu|(K_0 - K) \leq \varepsilon$.
c) For every compact subset $B$ of $A$, there exists a partition of $B$ formed by a $\mu$-negligible set $N$ and a sequence $(H_n)$ of compact sets belonging to $\mathcal{K}$.
d) For every compact subset $B$ of $A$, there exists an increasing sequence $(K_n)$ of compact sets belonging to $\mathcal{K}$, contained in $B$ and such that the set $N = B - \bigcup_n K_n$ is $\mu$-negligible.

It is immediate (No. 2, Prop. 5) that d) implies $a); c)$ implies d) on taking $K_n$ to be the union of the $H_p$ for $p \leq n$ and citing (PLII). To prove that b) implies c), one defines recursively a sequence $(H_p)$ of sets of $\mathcal{K}$ such that $H_{n+1} \subset B - \bigcup_{p \leq n} H_p$ and $|\mu|(B - \bigcup_{p \leq n} H_p) \leq 1/n$ (§ 4, No. 6, Th. 4).

It remains to prove that a) implies b). Let us argue by contradiction, and suppose that the supremum $\alpha$ of the numbers $|\mu|(K)$, where $K$ runs over the set of subsets of $K_0$ belonging to $\mathcal{K}$, is $< |\mu|(K_0)$. By (PLII), there exists an increasing sequence $(L_n)$ of compact subsets of $K_0$, belonging to $\mathcal{K}$ and such that $\sup_n |\mu|(L_n) = \alpha$. Set $B = \bigcup_n L_n$; $B$ is integrable and $|\mu|(B) = \alpha$, therefore $|\mu|(K_0 - B) = |\mu|(K_0) - \alpha > 0$. On the other hand, we shall see that for every set $K \in \mathcal{K}$, $|\mu|(K \cap (K_0 - B)) = 0$, which, by virtue of a), will imply a contradiction. Indeed, if there existed a set $K \in \mathcal{K}$ such that $|\mu|(K \cap (K_0 - B)) > 0$, then there would exist a compact subset $H$ of $K \cap (K_0 - B)$ such that $|\mu|(H) > 0$. By (PLI), we would have $H \in \mathcal{K}$, and, for $n$ sufficiently large,

$$
|\mu|(L_n \cup H) = |\mu|(L_n) + |\mu|(H) > \alpha .
$$

But $L_n \cup H$ belongs to $\mathcal{K}$ by (PLII), and this contradicts the definition of $\alpha$.

#### Definition 6 {#int-iv-s5-def-6 .statement}

— Let $A$ be a $\mu$-measurable subset of $X$. A set $\mathcal{K}$ of compact subsets of $A$ is said to be $\mu$-dense in $A$ if it satisfies the conditions (PLI), (PLII), $a), b), c), d)$ of Prop. 12.

The set of *all* compact subsets of $A$ is $\mu$-dense in $A$.

When $A = X$, we shall say simply ' $\mu$-dense set' in place of 'set $\mu$-dense in $X$'. If $X - A$ is locally $\mu$-negligible, then every set of compact subsets of $A$ that is $\mu$-dense in $A$ is also $\mu$-dense in $X$.

#### Remark {#int-iv-s5-n8-rem-1 .statement}

— Suppose that $A$ is the union of a sequence $(L_n)$ of compact sets and a $\mu$-negligible (resp. locally $\mu$-negligible) set, and let $\mathcal{K}$ be a set of compact subsets that is $\mu$-dense in $A$. Applying to each $L_n$ the property *c*) of the statement of Prop. 12, we see that $A$ is the union a sequence of compact sets *belonging to* $\mathcal{K}$ and a $\mu$-negligible (resp. locally $\mu$-negligible) set.

If $K$ is a compact subset of $X$, it comes to the same to say that a set of compact subsets of $K$ is $\mu$-dense in $K$ or that it is $\mu_K$-*dense* in $K$; this follows from Lemmas 2 and 3 of No. 7 and condition *b*) of Prop. 12.

#### Proposition 13 {#int-iv-s5-prop-13 .statement}

*Let $A$ be a $\mu$-measurable subset of $X$, $\mathcal{K}$ a set of compact subsets that is $\mu$-dense in $A$. Let $\mathfrak{H}$ be a set of compact subsets of $A$ satisfying (PL$_I$) and (PL$_{II}$) and such that, for every $K \in \mathcal{K}$, the set of $H \in \mathfrak{H}$ such that $H \subset K$ is $\mu_K$-*dense* (or, what amounts to the same, $\mu$-*dense*) in $K$. Then $\mathfrak{H}$ is $\mu$-dense in $A$.*

For, let $L$ be a compact subset of $A$. For every $\varepsilon > 0$ there exists a $K \in \mathcal{K}$ such that $K \subset L$ and $|\mu|(L - K) \leq \varepsilon/2$, and then an $H \in \mathfrak{H}$ such that $H \subset K$ and $|\mu|(K - H) \leq \varepsilon/2$; it follows that $|\mu|(L - H) \leq \varepsilon$, whence the proposition.

### 9. Locally countable partitions

#### Definition 7 {#int-iv-s5-def-7 .statement}

*A set $\mathfrak{A}$ of subsets of a topological space $T$ is said to be *locally countable* if, for every $t \in T$, there exists a neighborhood $V$ of $t$ such that the set of $A \in \mathfrak{A}$ that intersect $V$ is countable.*

If the set $\mathfrak{A}$ of subsets of $T$ is locally countable then, for every compact subset $K$ of $T$, the set of $A \in \mathfrak{A}$ that intersect $K$ is countable, since $K$ can be covered by a finite number of open neighborhoods of points of $K$, each of which intersects only a countable set of subsets belonging to $\mathfrak{A}$.

Def. 7 shows that the *union* of a locally countable set of $\mu$-measurable (resp. locally $\mu$-negligible) subsets of a locally compact space is $\mu$-measurable (resp. locally $\mu$-negligible) (No. 1, Prop. 3 and No. 2, Prop. 5).

#### Proposition 14 {#int-iv-s5-prop-14 .statement}

*Let $X$ be a locally compact space, $\mu$ a measure on $X$, $A$ a $\mu$-measurable subset of $X$, and $\mathcal{K}$ a set of compact subsets of $A$ that is $\mu$-dense in $A$. There exists a locally countable set $\mathfrak{H} \subset \mathcal{K}$, formed of pairwise disjoint sets, such that $A - \bigcup_{K \in \mathfrak{H}} K$ is locally $\mu$-negligible and such that, for every $K \in \mathfrak{H}$, the support of $\mu_K$ is all of $K$.*

Consider sets $\mathcal{L} \subset \mathfrak{K}$ formed of pairwise disjoint sets such that, for every $L \in \mathcal{L}$, $\operatorname{Supp}(\mu_L) = L$. The sets $\mathcal{L}$ form a subset $\mathcal{H}$ of $\mathcal{P}(\mathfrak{K})$ that is nonempty (because it contains the element $\varnothing$) and which we shall order by the relation of inclusion in $\mathcal{P}(\mathfrak{K})$. It is immediate that $\mathcal{H}$ is *inductive*; let $\mathfrak{H}$ be a maximal element of $\mathcal{H}$ (S, R, §6, No. 10). Let us first show that $\mathfrak{H}$ is *locally countable*. Indeed, for every $x \in X$, let $V$ be a relatively compact open neighborhood of $x$; if $(K_i)_{1 \leq i \leq n}$ is a finite family of distinct sets of $\mathfrak{H}$ that intersect $V$, then

$$
\sum_{i=1}^n |\mu|(K_i \cap V) = |\mu|\left(V \cap \left( \bigcup_{i=1}^n K_i \right)\right)
$$

because the $K_i$ are pairwise disjoint, whence $\sum_{i=1}^n |\mu|(K_i \cap V) \leq |\mu|(V)$. It follows that if $\mathfrak{H}_V$ is the set of $K \in \mathfrak{H}$ that intersect $V$, then

$$
\sum_{K \in \mathfrak{H}_V} |\mu|(K \cap V) < +\infty,
$$

and since $|\mu|(K \cap V) > 0$ for every $K \in \mathfrak{H}_V$, $\mathfrak{H}_V$ is necessarily countable. Next, let us prove that $N = A - \bigcup_{K \in \mathfrak{H}} K$ is locally $\mu$-negligible. We saw above that $N$ is $\mu$-measurable. If $N$ were not locally negligible, it would contain a non-negligible compact set $L_0$, hence (No. 8, Prop. 12) a non-negligible compact set $L \subset L_0$ belonging to $\mathfrak{K}$. Since $|\mu_L|(L) = |\mu|(L) > 0$ (No. 7, Lemmas 2 and 3), the measure $\mu_L$ induced on $L$ by $\mu$ is nonzero; its support $S$ is therefore a nonempty compact set belonging to $\mathfrak{K}$ by (PL₁), and $\operatorname{Supp}(\mu_S) = S$ (No. 7, Lemma 2, (iii)). It follows that the set $\mathfrak{H} \cup \{S\}$ belongs to $\mathcal{H}$, which contradicts the definition of $\mathfrak{H}$; the set $N$ is therefore locally negligible, which completes the proof.

### 10. Measurable functions defined on a measurable subset

#### Proposition 15 {#int-iv-s5-prop-15 .statement}

*Let $X$ be a locally compact space, $\mu$ a measure on $X$, $A$ a $\mu$-measurable subset of $X$, and $f$ a mapping of $A$ into a topological space $F$. The following conditions are equivalent:

a) The set $\mathfrak{H}$ of compact subsets $K$ of $A$ such that the restriction of $f$ to $K$ is continuous, is $\mu$-dense in $A$.

b) There exists a set $\mathfrak{K}$ of compact subsets of $A$, $\mu$-dense in $A$, such that the restriction of $f$ to every $K \in \mathfrak{K}$ is $\mu_K$-measurable.

c) There exist a homeomorphism $j$ of $F$ onto a subspace of a topological space $G$ and a $\mu$-measurable mapping $g$ of $X$ into $G$, such that $g|A = j \circ f$.*

d) Every extension of $f$ to a mapping of $X$ into $F$, constant on $X - A$, is $\mu$-measurable.

It is clear that a) implies b) and that d) implies c). The fact that c) implies a) follows from condition c) of Prop. 12 of No. 8. On the other hand, b) implies a): for, Def. 1 shows that, for each $K \in \mathcal{K}$, the set of subsets $H \in \mathcal{H}$ contained in $K$ is $\mu_K$-dense in $K$ (No. 8, Prop. 12, c)), and Prop. 13 of No. 8 shows that $\mathcal{H}$ is $\mu$-dense in $A$. It remains to see that a) implies d). Let $g$ be an extension of $f$ to $X$, constant on $X - A$. For every compact subset $L$ of $X$, $L \cap A$ and $L \cap (X - A)$ are $\mu$-integrable; therefore, for every $\varepsilon > 0$, there exist a compact subset $P \subset L \cap A$ and a compact subset $Q \subset L \cap (X - A)$ such that

$$
|\mu|((L \cap A) - P) \leq \varepsilon/4 \quad \text{and} \quad |\mu|\left((L \cap (X - A)) - Q\right) \leq \varepsilon/4.
$$

On the other hand, there exists a set $H \in \mathcal{H}$ contained in $P$ such that $|\mu|(P - H) \leq \varepsilon/2$; the restriction of $g$ to the compact set $K = H \cup Q$ is then continuous ($g$ being constant on $Q$) and $|\mu|(L - K) \leq \varepsilon$, which completes the proof.

#### Definition 8 {#int-iv-s5-def-8 .statement}

*Let $X$ be a locally compact space, $\mu$ a measure on $X$, and $A$ a $\mu$-measurable subset of $X$. A mapping $f$ of $A$ into a topological space $F$ is said to be $\mu$-measurable if it satisfies the equivalent conditions of Prop. 15.*

If $A$ is locally $\mu$-negligible, then *every* mapping of $A$ into $F$ is therefore $\mu$-measurable.

#### Corollary 1 {#int-iv-s5-def-8-cor-1 .statement}

*Let $X$ be a locally compact space, $\mu$ a measure on $X$, $A$ a $\mu$-measurable subset of $X$, and $f$ a $\mu$-measurable mapping of $A$ into a topological space $F$. Let $\mathcal{K}$ be a set of compact subsets of $X$, $\mu$-dense in $X$. Then, there exists a partition of $A$ formed by a locally negligible set $N$ and a locally countable family $(K_\lambda)_{\lambda \in L}$ of sets $K_\lambda \in \mathcal{K}$, such that $f|K_\lambda$ is continuous for every $\lambda \in L$.

In view of No. 9, Prop. 14, it suffices to show that the set $\mathcal{H} \subset \mathcal{K}$ of subsets $K \in \mathcal{K}$ such that $K \subset A$ and $f|K$ is continuous, is $\mu$-dense in $A$. Now, it follows at once from Prop. 1 of No. 1 and condition d) of Prop. 15 that, for every compact subset $K_0$ of $A$ and every $\varepsilon > 0$, there exists a subset $K \subset K_0$ belonging to $\mathcal{K}$ such that $|\mu|(K_0 - K) \leq \varepsilon$ and $f|K$ is continuous; the conclusion therefore follows from Prop. 12 of No. 8.

#### Corollary 2 {#int-iv-s5-def-8-cor-2 .statement}

*Let $K$ be a compact subspace of $X$; in order that a mapping $f$ of $K$ into a topological space $F$ be $\mu$-measurable, it is necessary and sufficient that it be $\mu_K$-measurable.*

In view of Lemma 2 of No. 7, this follows at once from Prop. 1 of No. 1 and condition a) of Prop. 15.

#### Proposition 16 {#int-iv-s5-prop-16 .statement}

*Let $\mathfrak{A}$ be a locally countable set of $\mu$-measurable subsets of $X$ and let $B = \bigcup_{A \in \mathfrak{A}} A$. For a mapping $f$ of $B$ into a topological space $F$ to be $\mu$-measurable, it is necessary and sufficient that the restriction of $f$ to every $A \in \mathfrak{A}$ be $\mu$-measurable.*

We have already observed (No. 9) that $B$ is $\mu$-measurable. The condition being obviously necessary, let us prove that it is sufficient. Thus, let $K$ be a compact subset of $B$. By hypothesis, there exists a sequence $(A_n)$ of sets belonging to $\mathfrak{A}$ such that the $K \cap A_n$ form a covering of $K$. Set $C_0 = K \cap A_0$ and
$$
C_n = K \cap A_n \cap \mathbf{C}\left( \bigcup_{i < n} C_i \right)
$$
for $n > 0$, so that the nonempty $C_n$ form a partition of $K$ into $\mu$-integrable sets. Since the restriction of $f$ to $C_n$ is $\mu$-measurable, there exists a partition of $C_n$ formed by a $\mu$-negligible set $N_n$ and a sequence $(L_{mn})_{m \geq 0}$ of compact sets such that $f|L_{mn}$ is continuous. Since $N = \bigcup_n N_n$ is $\mu$-negligible, we see that condition a) of Prop. 15 is satisfied, whence the proposition.

Property d) of Prop. 15 makes it possible to immediately generalize the properties of measurable functions defined on all of $X$, observed in Nos. 2 to 5, to measurable functions defined on a measurable subset $A$ of $X$; these generalizations are left to the reader. We only point out explicitly that the principle of localization (No. 2, Prop. 4) remains valid when it is assumed that each of the functions $g_x$ is only defined in $V_x$ (or almost everywhere in $V_x$) and is measurable.

### 11. Convergence in measure

Let $X$ be a locally compact space, $\mu$ a measure on $X$, $A$ a $\mu$-measurable subset of $X$, and $F$ a *uniform space*; we shall denote by $\mathcal{S}(A, \mu; F)$, or $\mathcal{S}_F(A, \mu)$ (or simply $\mathcal{S}_F(\mu)$, or even $\mathcal{S}_F$, when $A = X$) the set of $\mu$-*measurable mappings of $A$ into $F*$ (No. 10, Def. 8). For every entourage $V$ of the uniform structure of $F$, every $\mu$-integrable set $B \subset A$ and every number $\delta > 0$, we shall denote by $W(V, B, \delta)$ the set of pairs $(f, g)$ of functions in $\mathcal{S}(A, \mu; F)$ having the following property: the set $M$ of all $x \in B$ for which $(f(x), g(x)) \notin V$ is such that $|\mu|^*(M) \leq \delta$. Let us show that the sets $W(V, B, \delta)$ form a *fundamental system of entourages* for a uniform structure on $\mathcal{S}(A, \mu; F)$: it is clear that $W(V, B, \delta)$ is symmetric if $V$ is, and that if $V' \subset V,\ B' \supset B$ and $\delta' \leq \delta$, then

$$
W(V', B', \delta') \subset W(V, B, \delta);
$$

it therefore suffices to verify the axiom $(U'_{III})$ (GT, II, §1, No. 1). Now, if $V'$ is an entourage such that ${V'}^2 \subset V$, then

$$
W(V', B, \delta/2) \circ W(V', B, \delta/2) \subset W(V, B, \delta).
$$

Note that as $K$ runs over a $\mu$-dense set $\mathfrak{K}$ of *compact* subsets of $A$, the sets $W(V, K, \delta)$ also form a fundamental system of entourages for the preceding uniform structure: for, for every integrable set $B \subset A$, there exists a compact set $K \in \mathfrak{K}$ contained in $B$ such that $|\mu|(B - K) \leq \delta$, and therefore $W(V, K, \delta) \subset W(V, B, 2\delta)$.

#### Definition 9 {#int-iv-s5-def-9 .statement}

*The uniform structure on $\mathcal{S}(A, \mu; F)$ of which the $W(V, B, \delta)$ form a fundamental system of entourages is called the uniform structure of convergence in measure in $A$.*.

The corresponding topology is called the *topology of convergence in measure in $A$*, and a filter (or a sequence) that converges for this topology is said to be *convergent in measure in $A$*; the mention of $A$ is often suppressed when $A = X$.

Suppose $F$ is *Hausdorff*; then, for every $\mu$-integrable set $B \subset A$, the intersection of the entourages $W(V, B, \delta)$, where $V$ runs over a fundamental system of entourages of $F$ and $\delta$ runs over the set of numbers $> 0$, is the set of pairs $(f, g)$ such that $f(x) = g(x)$ *almost everywhere in $B$* (*with respect to $\mu$*). For, the set $M$ of $x \in B$ such that $f(x) \neq g(x)$ is $\mu$-integrable, because it is the inverse image, under the $\mu$-measurable mapping $x \mapsto (f(x), g(x))$, of the complement of the diagonal in $F \times F$, which is open (No. 5, Prop. 7); if $|\mu|(M) = \alpha > 0$, there exists a compact subset $K \subset M$ such that $|\mu|(M - K) < \alpha/2$ and such that the restrictions of $f$ and $g$ to $K$ are continuous; therefore, there exists an entourage $V_0$ of $F$ such that $(f(x), g(x)) \notin V_0$ for all $x \in K$, consequently $(f, g) \notin W(V_0, B, \alpha/2)$.

From this it follows that if $F$ is Hausdorff, then the intersection of *all* the entourages of $\mathcal{S}(A, \mu; F)$ is the set of pairs $(f, g)$ such that $f(x) = g(x)$ *locally almost everywhere in $A$*. The Hausdorff uniform space associated with $\mathcal{S}(A, \mu; F)$, which we shall denote $S(A, \mu; F)$ or $S_F(A, \mu)$ (or even $S_F(\mu)$ or $S_F$ when $A = X$), therefore consists of the *equivalence classes* for the relation « $f(x) = g(x)$ locally almost everywhere in $A$ » in the set $\mathcal{S}(A, \mu; F)$.

#### Proposition 17 {#int-iv-s5-prop-17 .statement}

— Let $(A_\lambda)_{\lambda \in L}$ be a locally countable family of $\mu$-measurable subsets of $A$, pairwise disjoint and such that $A - \bigcup_{\lambda \in L} A_\lambda$ is locally $\mu$-negligible. If, for every class $f \in S(A, \mu; F)$ and every $\lambda \in L$, $f_\lambda$ denotes the class of the restriction to $A_\lambda$ of any of the functions in the class $f$, then the mapping $\psi : f \mapsto (f_\lambda)_{\lambda \in L}$ is an isomorphism of the uniform space $S(A, \mu; F)$ onto the product uniform space $\prod_{\lambda \in L} S(A_\lambda, \mu; F)$.

It follows from No. 10, Prop. 16 that $\psi$ is bijective. Consider an entourage $T$ of $S(A, \mu; F)$ that is the canonical image of a $W(V, B, \delta)$, where $B$ is a compact subset of $A$; we know that the set $J$ of $\lambda \in L$ such that $B \cap A_\lambda \neq \varnothing$ is countable (No. 9), and $|\mu|(B) = \sum_{\lambda \in J} |\mu|(B \cap A_\lambda)$; therefore, there exists a finite subset $H$ of $J$ such that

$$
\sum_{\lambda \in J - H} |\mu|(B \cap A_\lambda) \leq \frac{\delta}{2}.
$$

The image of $T$ under $\psi \times \psi$ is then contained in the canonical image of the product $\prod_{\lambda \in H} W(V, B \cap A_\lambda, \delta)$. On the other hand, if $m$ is the number of elements of $H$, then the image of $T$ under $\psi \times \psi$ contains the canonical image of the entourage $\prod_{\lambda \in H} W(V, A_\lambda, \delta/2m)$, which proves the proposition.

#### Proposition 18 {#int-iv-s5-prop-18 .statement}

— *If $F$ is metrizable, and $A$ is the union of a locally $\mu$-negligible set and a sequence $(A_n)$ of $\mu$-integrable sets, then the space $S(A, \mu; F)$ is metrizable.*

Since each $A_n$ is the union of a negligible set and a sequence of compact sets, we can suppose that the $A_n$ are already *compact* and pairwise disjoint. Prop. 17 then allows us to suppose that $A$ is compact. If $(V_n)$ is a countable fundamental system of entourages of $F$, it is clear that the $W(V_n, A, 1/n)$ form a fundamental system of entourages of $S(A, \mu; F)$ as $n$ runs over $\mathbf{N}$, whence the proposition.

#### Lemma 4 {#int-iv-s5-lem-4 .statement}

— *Let $F$ be a metrizable uniform space, and let $B \subset A$ be a countable union of $\mu$-integrable sets. Then, for every Cauchy sequence $(f_n)$ in $S(A, \mu; F)$, there exists a subsequence $(f_{n_k})$ of $(f_n)$ such that $(f_{n_k}(x))$ is a Cauchy sequence in $F$ for almost every $x \in B$.*

Suppose first that $B$ is integrable, and denote by $d$ a metric compatible with the uniform structure of $F$. We shall define recursively a double sequence $(f_{mn})$ of functions in $S(A, \mu; F)$ such that $f_{0n} = f_n$ for every $n$, $(f_{mn})_{n \geq 0}$ is a subsequence of $(f_{m-1,n})_{n \geq 0}$ for every $m > 0$ and, finally, such that for every $m > 0$ the set $M_{mn}$ of $x \in B$ for which $d(f_{mn}(x), f_{m,n+1}(x)) > 1/2^{m+n+1}$ has measure $|\mu|(M_{mn}) \leq 1/2^{m+n+1}$;

the possibility of such a definition follows from the fact that $(f_n)$ is a Cauchy sequence in $\mathcal{S}(A, \mu; F)$. Set $M_m = \bigcup_{n \geq 0} M_{mn}$; then

$$
|\mu|(M_m) \leq \sum_{n=0}^{\infty} |\mu|(M_{mn}) \leq 1/2^m
$$

and, for every $x \in B - M_m$, we have $d(f_{mn}(x), f_{m,n+p}(x)) \leq 1/2^{m+n}$ for all $n \geq 0$ and all $p > 0$; the sequence $(f_{mn}(x))_{n \geq 0}$ is therefore a Cauchy sequence in $F$. Now let $N = \bigcap_{m=0}^{\infty} M_m$; $N$ is negligible. Set $g_n = f_{nn}$ for every $n \geq 0$; for every $m$, the sequence $(g_n)_{n \geq m}$ is a subsequence of the sequence $(f_{mn})_{n \geq 0}$; if $x \in B - N$, there exists an index $m$ such that $x \notin M_m$, which proves that the sequence $(g_n(x))$ is a Cauchy sequence in $F$.

If now $B$ is the union of a sequence $(B_m)$ of integrable sets, one can define recursively a double sequence $(g_{mn})$ such that $g_{0n} = f_n$, $(g_{mn})_{n \geq 0}$ is a subsequence of $(g_{m-1,n})_{n \geq 0}$ for every $m > 0$, and such that the sequence $(g_{mn}(x))_{n \geq 0}$ is a Cauchy sequence in $B_m - P_m$, where $P_m$ is negligible. Set $h_n = g_{nn}$ for every $n \geq 0$, so that, for every $m$, the sequence $(h_n)_{n \geq m}$ is a subsequence of $(g_{mn})_{n \geq 0}$; the sequence $(h_n(x))_{n \geq 0}$ is then a Cauchy sequence in $F$ for every $x \in B - P$, where $P = \bigcup_{m=0}^{\infty} P_m$ is negligible.

#### Proposition 19 {#int-iv-s5-prop-19 .statement}

*If the uniform space $F$ is metrizable and complete, then the uniform space $S(A, \mu; F)$ is complete.*

There exists a locally countable family $(K_{\lambda})_{\lambda \in L}$ of compact subsets of $A$ such that the $K_{\lambda}$ are pairwise disjoint and $A - \bigcup_{\lambda} K_{\lambda}$ is locally negligible (No. 9, Prop. 14). By Prop. 17, $S(A, \mu; F)$ is isomorphic to the product $\prod_{\lambda \in L} S(K_{\lambda}, \mu; F)$; we are thus reduced to proving the proposition when $A$ is *integrable*; $S(A, \mu; F)$ is then metrizable (Prop. 18) and, by Lemma 4, for every Cauchy sequence $(f_n)$ in $\mathcal{S}(A, \mu; F)$ there exists a subsequence $(f_{n_k})$ that is convergent in $A - N$, where $N$ is negligible; the limit $f$ of $(f_{n_k})$ (extended in any way whatsoever to all of $A$) is then $\mu$-measurable, and it follows from the extension of Egoroff’s theorem mentioned in No. 10 that the sequence $(f_{n_k})$ *converges in measure* to $f$ in $A$. This implies that $f$ is a cluster point of the sequence $(f_n)$ in $\mathcal{S}(A, \mu; F)$, and since the sequence $(f_n)$ is by hypothesis a Cauchy sequence, it converges to $f$.

Q.E.D.

#### Corollary {#int-iv-s5-n11-cor-1 .statement}

— Let F be a metrizable uniform space.

(i) Every sequence $(f_n)$ of elements of $\mathcal{S}(A, \mu; F)$ that converges locally almost everywhere to a mapping $f$ (necessarily $\mu$-measurable) of A into F, converges in measure to $f$ in A.

(ii) Let $(f_n)$ be a sequence of elements of $\mathcal{S}(A, \mu; F)$ that converges in measure to a mapping $f$ of A into F. For every set $B \subset A$ that is a countable union of integrable sets, there exists a subsequence $(f_{n_k})$ of $(f_n)$ such that the sequence $(f_{n_k}(x))$ converges in F to $f(x)$ for almost every $x \in B$.

(i) The assertion follows at once from the extension of Egoroff’s theorem mentioned in No. 10.

(ii) By Lemma 4, there exists a subsequence $(f_{n_k})$ of $(f_n)$ such that $(f_{n_k}(x))$ is a Cauchy sequence in F for every $x \in B - N$, where N is negligible; let $f'(x) \in \widehat{F}$ be the limit of this sequence for $x \in B - N$. It is clear that $f'$ is a $\mu$-measurable mapping of $B - N$ into $\widehat{F}$, and the sequence $(f_n)$ converges in measure to $f'$ in $B - N$ by (i); $f'$ is therefore equal to $f$ almost everywhere in B.

#### Proposition 20 {#int-iv-s5-prop-20 .statement}

— Let F be a Banach space, equipped with the uniform structure defined by its norm.

(i) For every $\mu$-measurable subset A of X, the topology of convergence in measure is compatible with the vector space structure of $\mathcal{S}(A, \mu; F)$.

(ii) The space $\mathcal{K}(X; F)$ is dense in $\mathcal{S}(X, \mu; F)$.

(iii) For every real number $p \geq 1$, the topology induced on the space $\mathcal{L}_F^p(X, \mu)$ by the topology of convergence in measure is coarser than the topology of convergence in mean of order $p$.

(i) For every $\mu$-integrable subset B of A and every $\delta > 0$, denote by $T(B, \delta)$ the set of $f \in \mathcal{S}(A, \mu; F)$ for which the set C of $x \in B$ such that $|f(x)| \geq \delta$ satisfies the relation $|\mu|(C) \leq \delta$; it is clear that if $V_\delta$ is the entourage of F formed by the pairs $(y, z)$ such that $|y - z| \leq \delta$, the entourage $W(V_\delta, B, \delta)$ is the set of pairs $(f, g)$ of measurable mappings of A into F such that $f - g \in T(B, \delta)$. It is clear that the sets $T(B, \delta)$ are symmetric, and that $T(B, \delta) + T(B, \delta) \subset T(B, 2\delta)$ and $T(B, |\alpha|\delta) \subset \alpha T(B, \delta)$ for every nonzero scalar $\alpha$ such that $|\alpha| \leq 1$; it therefore suffices to verify that the sets $T(B, \delta)$ are absorbent (TVS, I, §1, No. 5, Prop. 4). Now, if $f$ is a $\mu$-measurable mapping of A into F, the numerical function $|f|$ is also $\mu$-measurable (No. 3, Cor. 6 of Th. 1). Let $C_n$ be the set of $x \in B$ such that $|f(x)| \geq n$; the $C_n$ form a decreasing sequence of integrable sets whose intersection is empty; therefore there exists an integer $n$ such that $|\mu|(C_n) \leq \delta$ (§ 4, No. 5, Cor. of Prop. 7); we can moreover suppose that $n$ is taken sufficiently large that $1/n \leq \delta$; then $f/n^2 \in T(B, \delta)$, which completes the proof of assertion (i).

(iii) The relation $\int |f|^p d|\mu| \leq \delta^{p+1}$ implies that if $C$ is the set of $x \in X$ such that $|f(x)| \geq \delta$, then

$$
\delta^p |\mu|^*(C) \leq \int |f|^p d|\mu| \leq \delta^{p+1},
$$

whence $|\mu|^*(C) \leq \delta$, which proves (iii).

(ii) In view of (iii), it suffices to show for example that $\mathcal{L}_F^1$ is dense in $\mathcal{S}_F$, since by definition $\mathcal{H}(X; F)$ is dense in $\mathcal{L}_F^1$ for the topology of convergence in mean. Now, let $f$ be any element of $\mathcal{S}_F$ and let $T(B, \delta)$ be a neighborhood of 0 in this space; we see as in (i) that there exists an integrable subset $C$ of $B$ such that $|\mu|(C) \leq \delta$ and such that $f$ is *bounded* on $B - C$; denoting then by $g$ the function equal to $f$ on $B - C$ and to 0 on $X - (B - C)$, it follows from No. 6, Th. 5 that $g$ is integrable, and obviously $f - g \in T(B, \delta)$.

#### Remark {#int-iv-s5-n11-rem-1 .statement}

— 1) The topological vector space $\mathcal{S}(X, \mu; F)$ is not necessarily locally convex (Exer. 24).
2) The topology induced on the set of $f$ such that $N_p(f) \leq 1$ by the topology of convergence in measure may be strictly coarser than the topology induced on this set by the topology of convergence in mean of order $p$ (Exer. 22). However, see Prop. 21 below.

#### Definition 10 {#int-iv-s5-def-10 .statement}

*Let $X$ be a locally compact space, $\mu$ a measure on $X$, $F$ a Banach space, and $p \in [1, +\infty[$. A subset $H$ of $\mathcal{L}_F^p(X, \mu)$ is said to be equi-integrable of order $p$ (for $\mu$) if it satisfies the following conditions:*

(i) *For every $\varepsilon > 0$ there exists a $\delta > 0$ such that, for every integrable set $A$ of measure $|\mu|(A) \leq \delta$ and every $f \in H$,*

$$
\int |f|^p \varphi_A d|\mu| \leq \varepsilon.
$$

(ii) *For every $\varepsilon > 0$ there exists a compact subset $K$ of $X$ such that, for every $f \in H$,* $\int |f|^p \varphi_{X-K} d|\mu| \leq \varepsilon$.

When $p = 1$ we say 'equi-integrable' instead of 'equi-integrable of order 1'.

#### Remark {#int-iv-s5-n11-rem-2 .statement}

— Suppose $\mu$ is bounded. For every $a > 0$, the set of measurable mappings of $X$ into $F$ such that $|f(x)| \leq a$ almost everywhere is equi-integrable of order $p$, and this is true for any $p \in [1, +\infty[$.

#### Proposition 21 {#int-iv-s5-prop-21 .statement}

*Let $H$ be a subset of $\mathcal{L}_F^p(X, \mu)$ that is equi-integrable of order $p$. On $H$, the uniform structure of convergence in measure is equal to the uniform structure induced by that of $\mathcal{L}_F^p(X, \mu)$.*

Let $\varepsilon > 0$. There exist $\delta$ and $K$ with the properties (i) and (ii) of Def. 10. Let $f, g$ in $H$ be such that

$$
|f(x) - g(x)| \leq \left( \frac{\varepsilon}{|\mu|(K)} \right)^{1/p}
$$

for $x \in K$, except on a set $M$ of measure $\leq \delta$. Then

$$
\left( \int_{X-K} |f-g|^p d|\mu| \right)^{1/p} \leq \left( \int_{X-K} |f|^p d|\mu| \right)^{1/p} + \left( \int_{X-K} |g|^p d|\mu| \right)^{1/p}
$$
$$
\leq 2\varepsilon^{1/p}
$$

and similarly
$$
\left( \int_M |f-g|^p d|\mu| \right)^{1/p} \leq 2\varepsilon^{1/p},
$$
therefore
$$
\int |f-g|^p d|\mu| = \int_{X-K} |f-g|^p d|\mu| + \int_M |f-g|^p d|\mu| + \int_{K-M} |f-g|^p d|\mu|
$$
$$
\leq 2^p \varepsilon + 2^p \varepsilon + \frac{\varepsilon}{|\mu|(K)} |\mu|(K-M) \leq (2^{p+1} + 1)\varepsilon.
$$

Thus, the uniform structure of convergence in measure on $H$ is finer than the uniform structure induced by that of $\mathcal{L}_F^p(X, \mu)$. It then suffices to apply Prop. 20.

### 12. A property of vague convergence

#### Lemma 5 {#int-iv-s5-lem-5 .statement}

*Let $X$ be a locally compact space, $\mu$ a bounded positive measure on $X$, $F$ a Banach space, and $f$ a bounded function on $X$ with values in $F$. The following conditions are equivalent:*

(i) *The set of points of discontinuity of $f$ is $\mu$-negligible.*

(ii) *For every $\varepsilon > 0$, there exist elements $a_1, \ldots, a_n$ of $F$, functions $g_1, \ldots, g_n$ belonging to $\mathscr{K}(X)$, and a bounded continuous function $h \geq 0$ on $X$ such that $|f - g_1 a_1 - \cdots - g_n a_n| \leq h \leq 2 \sup |f|$ on $X$, and $\int h d\mu \leq \varepsilon$.*

Denote by $N$ the set of points of discontinuity of $f$, and let $M = \sup |f|$.

(i) $\Rightarrow$ (ii). Suppose that condition (i) is satisfied. Let $\varepsilon > 0$. The function $f$ is $\mu$-integrable (No. 2, Cor. 4 of Prop. 5, and No. 6, Th. 5), therefore there exist $a_1, \ldots, a_n$ in $F$ and $g_1, \ldots, g_n$ in $\mathscr{K}(X)$ such that, on setting $k = |f - g_1 a_1 - \cdots - g_n a_n|$, we have $\int k d\mu \leq \varepsilon/2$ (§ 3, No. 5,

Prop. 10). Multiplying $g_1, \ldots, g_n$ by a suitable same element of $\mathcal{K}(X)$, we can suppose in addition that

$$
|g_1 a_1 + \cdots + g_n a_n| \leq M = \sup |f|
$$

on X, whence $k \leq 2M$. The set $N'$ of points of discontinuity of $k$ is contained in $N$, hence is negligible. For every $x \in X$, set $l(x) = \limsup_{y \to x} k(y)$.

Then $2M \geq l \geq k$ on X, and $l = k$ on $X - N'$, that is, almost everywhere for $\mu$, therefore $\int l \, d\mu \leq \varepsilon / 2$. On the other hand, $l$ is bounded and upper semi-continuous, hence is the lower envelope of the set of bounded continuous functions $\geq l$. Therefore there exists a bounded continuous function $h \geq l$ on X such that $h \leq 2M$ and $\int h \, d\mu \leq \int l \, d\mu + \varepsilon / 2$ (§ 4, No. 4, Cor. 2 of Prop. 5). Then $\int h \, d\mu \leq \varepsilon$ and $|f - g_1 a_1 - \cdots - g_n a_n| \leq h$.

(ii) $\Rightarrow$ (i). Suppose that condition (ii) is satisfied. For every $x \in X$ let $\omega(x)$ be the oscillation of f at x (GT, IX, § 2, No. 3). Let $\varepsilon > 0$. There exist $a_1, \ldots, a_n, g_1, \ldots, g_n, h$ with the properties of (ii). For every $x \in X$, $\omega(x)$ is the oscillation of $f - g_1 a_1 - \cdots - g_n a_n$ at x, therefore $\omega(x) \leq 2h(x)$. Thus $\int \omega \, d\mu \leq 2\varepsilon$. Consequently, the set $A_\varepsilon$ of $x \in X$ such that $\omega(x) \geq \sqrt{\varepsilon}$ satisfies $\mu(A_\varepsilon) \leq 2\sqrt{\varepsilon}$. This proves that $\mu(N) \leq 2\sqrt{\varepsilon}$, whence $\mu(N) = 0$.

#### Proposition 22 {#int-iv-s5-prop-22 .statement}

— *Let F be a Banach space, X a locally compact space, $\mathcal{E}$ the set of bounded positive measures on X, $\mu$ an element of $\mathcal{E}$, and $\mathcal{B}$ a filter base on $\mathcal{E}$. Assume that $\mathcal{B}$ converges vaguely to $\mu$ and that $\| \nu \|$ tends to $\| \mu \|$ with respect to $\mathcal{B}$. Let f be a mapping of X into F satisfying the following conditions:

(i) f is bounded, and is integrable for $\mu$ and for every measure that belongs to some element of $\mathcal{B}$;
(ii) the set of points of discontinuity of f is $\mu$-negligible.
Then $\int f \, d\nu$ tends to $\int f \, d\mu$ with respect to $\mathcal{B}$.

Let $\varepsilon > 0$. There exist elements $a_1, \ldots, a_n$ in F, functions $g_1, \ldots, g_n$ in $\mathcal{K}(X)$, and a bounded continuous function $h \geq 0$ on X, such that

$$
|f - g_1 a_1 - \cdots - g_n a_n| \leq h \leq 2 \sup |f|
$$

on X and $\int h \, d\mu \leq \varepsilon$ (Lemma 5). Let $M = \sup |f|$. There exist a compact subset K of X such that $\mu^*(X - K) \leq \varepsilon$ (§ 4, No. 7, Prop. 12 and No. 6, Th. 4), a compact neighborhood $K'$ of K in X, and a continuous mapping $h'$ of X into $[0, 2M]$ such that $h' = h$ on K, $h' = 2M$ on $X - K'$; replacing $h'$ by $\sup(h, h')$, we can suppose in addition that $h' \geq h$. Then $\int (h' - h) \, d\mu \leq 2M \mu^*(X - K) \leq 2M \varepsilon$. On the other hand, $h' = h_1 + 2M$, where $h_1 \in \mathcal{K}(X)$. Taking into account § 4, No. 7, Prop. 12, the number

$$
\int h' \, d\nu = \int h_1 \, d\nu + 2M \|\nu\| \text{ tends to } \int h_1 \, d\mu + 2M \|\mu\| = \int h' \, d\mu \text{ with respect to } \mathcal{B}. \text{ There then exists an } A \in \mathcal{B} \text{ such that, for every } \nu \in A,
$$
$$
\left| \int (g_1 a_1 + \cdots + g_n a_n) \, d\nu - \int (g_1 a_1 + \cdots + g_n a_n) \, d\mu \right| \leq \varepsilon,
$$
$$
\int h \, d\nu \leq \int h' \, d\nu \leq \int h' \, d\mu + \varepsilon \leq \int h \, d\mu + 2M \varepsilon + \varepsilon \leq 2(M + 1)\varepsilon.
$$
These inequalities imply
$$
\left| \int f \, d\nu - \int f \, d\mu \right| \leq
$$
$$
\int h \, d\nu + \left| \int (g_1 a_1 + \cdots + g_n a_n) \, d\nu - \int (g_1 a_1 + \cdots + g_n a_n) \, d\mu \right| + \int h \, d\mu
$$
$$
\leq 2(M + 2)\varepsilon,
$$
which proves the proposition.

#### Remark {#int-iv-s5-n12-rem-1 .statement}

The conditions (i) and (ii) of Proposition 22 are satisfied if $f$ is continuous and bounded.

#### Example {#int-iv-s5-n12-exa-1 .statement}

Let us take for $X$ the compact space $\mathbf{U}$ of complex numbers of absolute value 1. On setting $\mu(f) = \int_0^1 f(e^{2i\pi t}) \, dt$ for every $f \in \mathcal{H}(\mathbf{U})$, one defines a positive measure of mass 1 on $\mathbf{U}$. On the other hand, let $\theta$ be a real number; for every integer $n \geq 0$, let $\nu_n$ be the unit mass placed at the point $e^{2i\pi n \theta}$ of $\mathbf{U}$, and let
$$
\mu_n = \frac{1}{n+1} (\nu_0 + \cdots + \nu_n),
$$
so that $\mu_n$ is a positive measure of mass 1 on $\mathbf{U}$. Then, if $\theta$ is irrational, $\mu_n$ tends vaguely to $\mu$. For, since the linear combinations of the functions $z \mapsto z^k$ ($k \in \mathbf{Z}$) are dense in $\mathcal{H}(\mathbf{U})$ (GT, X, §4, No. 4, Prop. 8), it suffices to prove that $\mu_n(z^k)$ tends to $\mu(z^k)$ for $k \in \mathbf{Z}$. Now, for $k = 0$, $\mu_n(z^k) = \mu(z^k) = 1$; for $k \neq 0$,
$$
\mu_n(z^k) = \frac{1}{n+1} (1 + e^{2i\pi k \theta} + e^{4i\pi k \theta} + \cdots + e^{2i\pi k n \theta}).
$$
Since $e^{2i\pi k \theta} \neq 1$ (because $\theta$ is irrational), we infer that
$$
|\mu_n(z^k)| = \left| \frac{1}{n+1} \frac{e^{2i\pi k(n+1)\theta} - 1}{e^{2i\pi k \theta} - 1} \right| \leq \frac{1}{n+1} \frac{2}{|e^{2i\pi k \theta} - 1|},
$$

therefore $\mu_n(z^k)$ tends to $0 = \mu(z^k)$. Under these conditions, Proposition 22 can be applied, and we see in particular that if $A$ is a subset of $U$ with negligible boundary with respect to $\mu$, then $\mu_n(A)$ tends to $\mu(A)$. In other words, if $p_n$ denotes the number of integers $k \in [0, n]$ such that $e^{2i\pi k \theta} \in A$, then $n^{-1} p_n$ tends to $\mu(A)$ as $n$ tends to $+\infty$.

### Exercises {#int-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
