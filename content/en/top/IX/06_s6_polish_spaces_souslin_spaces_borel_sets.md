---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 6
section_title: Polish spaces, Souslin spaces, Borel sets
lang: en
source: top-v-x
pdf_pages: 0201-0216, 0264-0273
extraction: ocr
subsections:
    - "no": 1
      title: POLISH SPACES
      page: 0
      pdf_page: 201
    - "no": 2
      title: SOUSLIN SPACES
      page: 0
      pdf_page: 203
    - "no": 3
      title: BOREL SETS
      page: 0
      pdf_page: 205
    - "no": 4
      title: ZERO-DIMENSIONAL SPACES AND LUSIN SPACES
      page: 0
      pdf_page: 206
    - "no": 5
      title: SIEVES
      page: 0
      pdf_page: 208
    - "no": 6
      title: SEPARATION OF SOUSLIN SETS
      page: 0
      pdf_page: 210
    - "no": 7
      title: LUSIN SPACES AND BOREL SETS
      page: 0
      pdf_page: 211
    - "no": 8
      title: BOREL SECTIONS
      page: 0
      pdf_page: 212
    - "no": 9
      title: CAPACITABILITY OF SOUSLIN SETS
      page: 0
      pdf_page: 214
statements: 48
exercises: 1
content_sha256: 69f92cd78f330694f81aad84eec3ecfd43d27d5eacabcc416871a1736cb0f341
---

## 6. POLISH SPACES, SOUSLIN SPACES, BOREL SETS

### 1. POLISH SPACES

#### Definition 1 {#top-ix-s6-def-1 .statement}

*A topological space* $X$ *is said to be Polish if it is metrizable of countable type* ($§ 2$, no. 8) *and if there is a metric, compatible with the topology of* $X$, *with respect to which* $X$ *is complete*.

#### Proposition 1 {#top-ix-s6-prop-1 .statement}

a) *Every closed subspace of a Polish space is Polish*.
b) *The product of a countable family of Polish spaces is Polish*.
c) *The sum of a countable family of Polish spaces is Polish*.

Every subspace of a metrizable space of countable type is metrizable of countable type, and every closed subspace of a complete space is complete; (Chapter II, § 3, no. 4, Proposition 8). Every countable product of metrizable spaces of countable type is again metrizable of countable type: ($§ 2$, no. 8), and every countable product of complete metric spaces is a complete metric space with respect to a metric compatible with its topology (Chapter II, § 3, no. 5, Proposition 10 and Chapter IX, § 2, no. 4, Theorem 1, Corollary 2). Finally, let $(X_n)$ be a sequence of non-empty Polish spaces, and consider the product space $Y = \mathbf{N} \times \prod_n X_n$, where $\mathbf{N}$ carries the discrete topology; $Y$ is a Polish space by what has already been proved. On the other hand, let $a_n$ be a point of $X_n$ for each $n$, and let $f_n$ be the mapping of $X_n$ into $Y$ such that for each $x \in X_n$ we have

$$
f_n(x) = (n, (y_p)),
$$

where $y_p = a_p$ if $p \neq n$ and $y_n = x$. If $X$ is the topological sum of the $X_n$, it is clear that the mapping $f$ of $X$ into $Y$ which agrees with $f_n$ on $X_n$ for each $n$ is a homeomorphism of $X$ onto $f(X)$; also, for each $n$, $f_n(X_n)$ is closed in $Y$, and the family $(f_n(X_n))$ is locally finite because $\mathbf{N}$ is discrete; therefore $f(X) = \bigcup_n f_n(X_n)$ is closed in $Y$ (Chapter I, § 1, no. 5, Proposition 4), and thus $f(X)$ is a Polish space, by a).

#### Proposition 2 {#top-ix-s6-prop-2 .statement}

Every open subspace of a Polish space is Polish.

Let $X$ be a Polish space, let $d$ be a metric on $X$ compatible with its topology, and let $U \neq X$ be an open subset of $X$. Let $V$ be the subset of $\mathbf{R} \times X$ consisting of all points $(t, x)$ such that
$$
t \cdot d(x, X - U) = 1;
$$
$V$ is closed by Proposition 3 of § 2, no. 2 and is therefore Polish (Proposition 1). Since the restriction to $V$ of the projection $\mathrm{pr}_2 : \mathbf{R} \setminus X \to X$ is a homeomorphism of $V$ onto $U$ ($§ 2,$ no. 2, Proposition 3), $U$ is a Polish subspace of $X$.

#### Corollary {#top-ix-s6-n1-cor-1 .statement}

Every locally compact, metrizable space $X$ is Polish.

Let $X$ be the compact space obtained by adjoining a point at infinity to $X$; $X'$ is metrizable and of countable type ($§ 2,$ no. 9, Corollary to Proposition 16), and $X$ is complete with respect to its unique uniformity (Chapter II, $§ 4,$ no. 1, Theorem 1). Hence $X$ is a Polish space; since $X$ is open in $X'$, it follows that $X$ is Polish.

#### Proposition 3 {#top-ix-s6-prop-3 .statement}

Let $X$ be a Hausdorff topological space. Then the intersection of a sequence $(A_n)$ of Polish subspaces of $X$ is a Polish subspace.

Let $f$ be the diagonal mapping of $X$ into $X^\mathbf{N}$ ([Set Theory, Chapter II, $§ 5,$ no. 3; recall that $f(x) = (x, x, \ldots)$ where $x_n = x$ for all $n \in \mathbf{N}$]. We shall use the following lemma:

#### Lemma 1 {#top-ix-s6-lem-1 .statement}

Let $(A_n)$ be a sequence of subsets of a Hausdorff topological space $X$. Then the restriction of the diagonal mapping $f : X \to X^\mathbf{N}$ to the subspace $\bigcap_n A_n$ of $X$ is a homeomorphism of $\bigcap_n A_n$ into a closed subspace of $\prod_n A_n$.

This image is the intersection of $\prod_n A_n$ and the diagonal $\Delta = f(X)$, which is closed in $X^\mathbf{N}$ because $X$ is Hausdorff (Chapter I, $§ 8,$ no. 1); and $f$ is a homeomorphism of $X$ onto $\Delta$.

With the hypotheses of Proposition 3, $\prod_n A_n$ is a Polish space (Proposition 1), hence $\bigcap_n A_n$ is Polish by Lemma 1 and Proposition 1.

#### Corollary {#top-ix-s6-n1-cor-2 .statement}

The set of irrational numbers, endowed with the topology induced by that of the real line $\mathbf{R}$, is a Polish space.

It is the intersection of a countable family of open sets in $\mathbf{R}$, namely the complements of sets consisting of a single rational number.

#### Theorem 1 {#top-ix-s6-thm-1 .statement}

*A subspace* $Y$ *of a Polish space* $X$ *is Polish if and only if* $Y$ *is the intersection of a countable family of open sets in* $X$.

The sufficiency of the condition follows immediately from Propositions 2 and 3. To show necessity, let $d$ be a metric compatible with the topology of $Y$ and with respect to which $Y$ is complete. Let $\overline{Y}$ be the closure of $Y$ in $X$. For each integer $n > 0$, let $Y_n$ be the set of all $x \in \overline{Y}$ which have an open neighbourhood $U$ such that the diameter of $U \cap Y$ (with respect to the metric $d$) is $\leq 1/n$. Clearly $Y_n$ is open in $\overline{Y}$ and contains $Y$. Let $x \in \bigcap_n Y_n$; then $x \in \overline{Y}$, and the trace on $Y$ of the neighbourhood filter of $x$ in $X$ is a Cauchy filter (with respect to $d$); hence this filter converges to a point of $Y$, and thus $x \in Y$. Hence $Y = \bigcap_n Y_n$.

For each $n$, let $H_n$ be an open subset of $X$ such that $H_n \cap \overline{Y} = Y_n$, and let $(U_m)$ be a sequence of open subsets of $X$ such that $\overline{Y} = \bigcap_m U_m$ (§ 2, no. 5, Proposition 7); then $Y$ is the intersection of the countable family of open sets $(H_n \cap U_m)$.

#### Corollary 1 {#top-ix-s6-thm-1-cor-1 .statement}

*A space* $X$ *is Polish if and only if it is homeomorphic to a countable intersection of open sets in the cube* $\mathbf{I}^{\mathbf{N}}$, *where* $\mathbf{I}$ *is the interval* $[0, 1]$ *of* $\mathbf{R}$.

The condition is clearly sufficient, and it is necessary because every metrizable space of countable type is homeomorphic to a subspace of $\mathbf{I}^{\mathbf{N}}$ (§ 2, no. 8, Proposition 12).

#### Corollary 2 {#top-ix-s6-thm-1-cor-2 .statement}

*Let* $X$ *and* $Y$ *be two Polish spaces and let* $f : X \to Y$ *be a continuous mapping. If* $Z$ *is a Polish subspace of* $Y$, *then* $\overline{f}^{-1}(Z)$ *is a Polish subspace of* $X$.

For $Z = \bigcap_n Z_n$, where the $Z_n$ are open subsets of $Y$; hence
$$
\overline{f}^{-1}(Z) = \bigcap_n \overline{f}^{-1}(Z_n),
$$
and the sets $\overline{f}^{-1}(Z_n)$ are open in $X$.

### 2. SOUSLIN SPACES

#### Definition 2 {#top-ix-s6-def-2 .statement}

*A topological space* $X$ *is said to be a Souslin space if it is metrizable and if there exists a Polish space* $P$ *and a continuous mapping of* $P$ *onto* $X$. *A subset* $A$ *of a topological space* $X$ *is called a Souslin set if the subspace* $A$ *is a Souslin space.*

Clearly every Polish space is Souslin, and the image of a Souslin space $X$ under a continuous mapping of $X$ into a metrizable space $Y$ is a Souslin space.

#### Proposition 4 {#top-ix-s6-prop-4 .statement}

*Every Souslin space $X$ is of countable type.*

Let $P$ be a Polish space and $f$ a continuous mapping of $P$ onto $X$. Then the image under $f$ of a countable dense subset of $P$ is a countable dense subset of $X$.

#### Proposition 5 {#top-ix-s6-prop-5 .statement}

*Every closed (resp. open) subspace of a Souslin space $X$ is Souslin.*

For if $f$ is a continuous mapping of a Polish space $P$ onto $X$, then the inverse image under $f$ of a closed (resp. open) subset of $X$ is a closed (resp. open) subset of $P$, hence is a Polish subspace of $P$ (no. 1, Propositions 1 and 2).

#### Proposition 6 {#top-ix-s6-prop-6 .statement}

*Let $X$ be a Souslin space, let $Y$ be a Hausdorff space and let $f : X \to Y$ be a continuous mapping. Then the inverse image under $f$ of a Souslin subspace $A$ of $Y$ is a Souslin subspace of $X$.*

Let $P, Q$ be Polish spaces, let $g$ be a continuous mapping of $P$ onto $X$ and let $h$ be a continuous mapping of $Q$ onto $A$. Let $R$ be the set of all $(x, y) \in P \times Q$ such that $f(g(x)) = h(y)$; $R$ is closed in $P \times Q$ and is therefore a Polish subspace of $P \times Q$ (no. 1, Proposition 1). Let $\varphi$ be the restriction to $R$ of the projection $pr_1$. Then the subspace $\overline{f}^{-1}(A)$ of $X$ is the image of $R$ under the continuous mapping $g \circ \varphi$ and is therefore a Souslin space.

#### Proposition 7 {#top-ix-s6-prop-7 .statement}

*The product and the sum of a countable family of Souslin spaces are Souslin spaces.*

For each integer $n$, let $X_n$ be a metrizable space, $P_n$ a Polish space, and $f_n$ a continuous mapping of $P_n$ onto $X_n$. The product (resp. sum) of the spaces $P_n$ is Polish (no. 1, Proposition 1), and the image of this space under the mapping which is the product of the $f_n$ (resp. the mapping which agrees with $f_n$ on $P_n$ for all $n$) is the product (resp. sum) of the spaces $X_n$; the latter is metrizable, and is therefore a Souslin space.

#### Proposition 8 {#top-ix-s6-prop-8 .statement}

*Let $X$ be a metrizable space and let $(A_n)$ be a sequence of Souslin subspaces of $X$. Then the union and the intersection of the $A_n$ are Souslin spaces.*

These subspaces are certainly metrizable. The existence of the canonical map of the sum of the $A_n$ onto the subspace $\bigcup_n A_n$ of $X$ shows that the latter is a Souslin space; and $\bigcap_n A_n$ is Souslin by virtue of Propositions 5 and 7 and Lemma 1 of no. 1.

In general, even in a Polish space, the complement of a Souslin subspace is not necessarily Souslin (cf. Exercise 6); see, however, no. 6, Theorem 2, Corollary.

#### Proposition 9 {#top-ix-s6-prop-9 .statement}

*Let X be a metrizable space, and let A be a relatively compact Souslin subspace of X. Then there exists a compact metrizable space K, a decreasing sequence $(B_n)$ of subsets of K, each of which is a countable union of compact sets, and a continuous mapping $f : K \to X$, such that $A = f\left(\bigcap_n B_n\right)$.*

Replacing X by $\overline{A}$ if necessary, we may suppose that X is compact and that A is dense in X. Since A is a Souslin space, there is a Polish space P and a continuous mapping $g : P \to X$ such that $g(P) = A$. By no. 1, Theorem 1, Corollary 1, we may assume that P is the intersection of a decreasing sequence $(U_n)$ of open subsets of the cube $I^\mathbf{N}$. Let K be the space $I^\mathbf{N} \times X$, which is compact and metrizable (§ 2, no. 4, Theorem 1, Corollary 2). Let $G \subset P \times X$ be the graph of g, let $\overline{G}$ be the closure of G in K, and let f denote the projection of $K = I^\mathbf{N} \times X$ onto X; then clearly we have $f(G) = A$. Since g is continuous, G is closed in $P \times X$ (Chapter I, § 8, no. 1, Proposition 2, Corollary 2) and $G = \overline{G} \cap (P \times X)$; hence $G = \bigcap_n B_n$, where

$$
B_n = \overline{G} \cap (U_n \times X).
$$

Since each $U_n$ is a countable union of closed sets in $I^\mathbf{N}$ (§ 2, no. 5, Proposition 7), each $B_n$ is a countable union of compact sets and the proof is complete.

### 3. BOREL SETS

#### Definition 3 {#top-ix-s6-def-3 .statement}

*Let X be a set and let $\mathfrak{L}$ be a set of subsets of X. $\mathfrak{L}$ is said to be a $\sigma$-algebra on X if the following conditions are satisfied:

a) *The complement of every set of $\mathfrak{L}$ belongs to $\mathfrak{L}$*.

b) *Every countable intersection of sets of $\mathfrak{L}$ belongs to $\mathfrak{L}$*.

If $\mathfrak{L}$ is a $\sigma$-algebra on X, every *countable union* of sets of $\mathfrak{L}$ belongs to $\mathfrak{L}$ (for the complement of this union is an intersection of sets of $\mathfrak{L}$).

The set $\mathfrak{B}(X)$ of all subsets of X is clearly a $\sigma$-algebra. Every intersection of $\sigma$-algebras on X is a $\sigma$-algebra on X. For any subset of $\mathfrak{B}(X)$, there is therefore a *smallest* $\sigma$-algebra containing $\mathfrak{F}$; it is called the $\sigma$-algebra *generated by* $\mathfrak{F}$.

#### Definition 4 {#top-ix-s6-def-4 .statement}

In a topological space $X$, the elements of the $\sigma$-algebra generated by the set of all closed subsets of $X$ are called Borel sets in $X$.

#### Proposition 10 {#top-ix-s6-prop-10 .statement}

Let $f$ be a continuous mapping of a topological space $X$ into a topological space $Y$. Then the inverse image under $f$ of every Borel set in $Y$ is a Borel set in $X$.

Let $\mathfrak{I}$ be the set of all subsets $A$ of $Y$ such that $f^{-1}(A)$ is a Borel set in $X$. It follows immediately that $\mathfrak{I}$ is a $\sigma$-algebra which contains all the closed subsets of $Y$; hence $\mathfrak{I}$ contains all Borel sets in $Y$.

#### Proposition 11 {#top-ix-s6-prop-11 .statement}

In a Souslin space $X$, every Borel set is a Souslin set.

Let $\mathfrak{I}$ be the set of all subsets $A$ of $X$ such that both $A$ and $\overline{A}$ are Souslin sets. By Proposition 8 of no. 2, $\mathfrak{I}$ is a $\sigma$-algebra. Every closed subset $F$ of $X$ belongs to $\mathfrak{I}$, for both $F$ and $\overline{F}$ are Souslin sets (no. 2, Proposition 5); hence $\mathfrak{I}$ contains all Borel sets of $X$ (cf. no. 6, Theorem 2, Corollary).

#### Corollary {#top-ix-s6-n3-cor-1 .statement}

Let $f$ be a continuous mapping of a Souslin space $X$ into a metrizable space $Y$. If $B$ is any Borel set in $X$, then $f(B)$ is a Souslin set in $Y$.

For $B$ is a Souslin space, hence so is $f(B)$ by the remark following Definition 2 (no. 2).

#### Remark 1 {#top-ix-s6-n3-rem-1 .statement}

Even when $X$ and $Y$ are Polish spaces it is not in general true that the image of a Borel set in $X$ under a continuous mapping of $X$ into $Y$ is a Borel set in $Y$ (cf. Exercise 6; and no. 7, Theorem 3 Corollary).

#### Remark 2 {#top-ix-s6-n3-rem-2 .statement}

Let $X$ be a topological space and let $Y$ be a Borel subset of $X$. Then the Borel sets of the space $Y$ are exactly the Borel sets of $X$ which are contained in $Y$. For (i) the Borel sets in $X$ which are contained in $Y$ form a $\sigma$-algebra on $Y$ which contains the closed sets in $Y$ and hence contains all Borel sets of $Y$; (ii) the subsets $A$ of $X$ such that $A \cap Y$ is a Borel set of $Y$ form a $\sigma$-algebra on $X$ which contains all the closed sets of $X$ and therefore contains all Borel sets of $X$.

### 4. ZERO-DIMENSIONAL SPACES AND LUSIN SPACES

#### Definition 5 {#top-ix-s6-def-5 .statement}

A topological space is said to be zero-dimensional if it is Hausdorff and if every point has a fundamental system of neighbourhoods which are both open and closed.

Every zero-dimensional space $X$ is totally disconnected; for the component of a point $x$ is contained in all the sets containing $x$ which are both open and closed (Chapter I, § II, no. 5), and the intersection of these sets is just $\{ x \}$ if $X$ is zero-dimensional.

Conversely, a locally compact totally disconnected space is zero-dimensional (Chapter II, § 4, no. 4, Proposition 6); but there exist totally disconnected metrizable spaces which are not zero-dimensional [Exercise 3 b)].

Every subspace of a zero-dimensional space is zero-dimensional, and topological sums and products of zero-dimensional spaces are zero-dimensional.

#### Definition 6 {#top-ix-s6-def-6 .statement}

A topological space $X$ is a Lusin space if it is metrizable and if there exists a zero-dimensional Polish space $P$ and a continuous bijective mapping of $P$ onto $X$.

Every Lusin space is clearly a Souslin space.

#### Proposition 12 {#top-ix-s6-prop-12 .statement}

A metrizable space is a Lusin space if and only if it is the image of a Polish space under a continuous bijective mapping.

The condition is clearly necessary; let us show that it is also sufficient. If $f$ is a continuous bijection of a Lusin space $X$ onto a metrizable space $Y$, it follows from Definition 6 that $Y$ is a Lusin space. Hence we need only show that a Polish space is a Lusin space.

Notice first that, if $X$ is a Lusin space, every closed (resp. open) subspace $A$ of $X$ is a Lusin space (cf. no. 7, Theorem 3); for if $f$ is a continuous bijection of a zero-dimensional Polish space $P$ onto $X$, then $f^{-1}(A)$ is closed (resp. open) in $P$ and is therefore a zero-dimensional Polish subspace of $P$ (no. 1, Propositions 1 and 2).

Every countable product of Lusin spaces is a Lusin space; this follows from Proposition 1 of no. 1 and the fact that every product of zero-dimensional spaces is zero-dimensional. Every countable intersection of Lusin subspaces of a Hausdorff topological space is a Lusin subspace; this follows from the preceding remarks and from Lemma 1 of no. 1. Furthermore:

#### Lemma 2 {#top-ix-s6-lem-2 .statement}

If a metrizable space $X$ is such that there exists a countable partition $(A_n)$ of $X$ formed of Lusin subspaces, then $X$ is a Lusin space.

For each $n$, let $P_n$ be a zero-dimensional Polish space and let $f_n$ be a continuous bijection of $P_n$ onto $A_n$. If $P$ is the topological sum of the $P_n$, then $P$ is Polish (no. 1, Proposition 1) and zero-dimensional, and the mapping $f : P \to X$ which agrees with $f_n$ on $P_n$ for each $n$ is a continuous bijection of $P$ onto $X$; hence the result.

Let us now show that the interval $I = [0, 1]$ of $\mathbf{R}$ is a Lusin space. Let $J$ be the subspace of $I$ consisting of all irrational numbers; then $J$ is Polish (no. 1, Corollary to Proposition 3); also J is zero-dimensional, for if x is any point of J, the traces on J of intervals of R of the form ]r, s[, where r and s are rational and r < x < s, form a fundamental system of open and closed neighbourhoods of x in J (because the traces on J of ]r, s[ and [r, s] are the same). Hence J is a Lusin subspace of I. Now J and the subspaces of I which consist each of a single rational point form a countable partition of I, and therefore I is a Lusin space by Lemma 2.

Let P be an arbitrary Polish space. By Corollary 1 to Theorem 1 (no. 1), P is homeomorphic to a subspace of the cube IN which is a countable intersection of open sets in IN. Since I is a Lusin space, the remarks at the beginning of the proof show that P is a Lusin space, and the proof of Proposition 12 is therefore complete.

### 5. SIEVES

#### Definition 7 {#top-ix-s6-def-7 .statement}

A sieve is a sequence C = (C_n, p_n)_{n \geq 0} such that, for each n, C_n is a countable set and p_n is a surjection of C_{n+1} onto C_n.

For each pair of integers m, n such that 0 \leq m \leq n, let p_{mn} denote the identity mapping of C_m onto itself if m = n, and the surjection p_m \circ p_{m+1} \circ \cdots \circ p_{n-1} of C_n onto C_m if m < n. Clearly p_{mq} = p_{mn} \circ p_{nq} whenever m \leq n \leq q, and we may therefore consider the inverse limit L(C) of the family (C_n) with respect to the family of mappings (p_{mn}) (Set Theory, Chapter III, § 7). If each C_n is endowed with the discrete topology, then L(C) is an inverse limit of topological spaces (Chapter I, § 4, no. 4); as such, L(C) is called the topological space associated with the sieve C. L(C) is a closed subspace of the topological product $\prod_n C_n$, and it follows immediately that L(C) is a zero-dimensional Polish space (no. 4).

A sifting of a metric space X consists of a sieve C = (C_n, p_n) and for each integer n \geq 0 a mapping \varphi_n of C_n into the set of non-empty closed subsets of X of diameter \leq 2^{-n}, such that:

a) X is the union of the sets \varphi_0(c) as c runs through C_0;
b) for each n and each c \in C_n, \varphi_n(c) is the union of the sets \varphi_{n+1}(c'), where c' runs through p_n^{-1}(c).

A sifting is said to be strict if in addition, for each n, the sets \varphi_n(c), as c runs through C_n, are mutually disjoint.

#### Lemma 3 {#top-ix-s6-lem-3 .statement}

Every metric space X of countable type possesses a sifting. If also X is zero-dimensional, then X has a strict sifting.

Note first that if $Y$ is a metric space of countable type and if $\varepsilon$ is a real number $> 0$, then there is a countable covering of $Y$ by sets of diameter $\leq \varepsilon$ ($§ 2$, no. 8, Proposition 13). If, moreover, $Y$ is zero-dimensional, there is such a covering $(V_n)$ formed of sets which are both open and closed; if $W_n$ is the intersection of $V_n$ and $\bigcap_{k < n} (Y - V_k)$, we see that the $W_n$ are closed, of diameter $\leq \varepsilon$, pairwise disjoint and cover $X$. In any case, the closures of the non-empty sets of the covering form a countable covering of $Y$ whose elements are non-empty closed sets of diameter $\leq \varepsilon$.

Let $X$ be a metric space of countable type. Let $C_0$ be the set of indices of a countable covering of $X$ formed of non-empty closed sets of diameter $\leq 1$, which are pairwise disjoint if $X$ is zero-dimensional; $\varphi_0$ shall be the mapping which associates with each index $c \in C_0$ the corresponding set of the covering. Suppose that we have already defined the $C_i$ and the $\varphi_i$ and the surjective mappings $p_i : C_{i+1} \to C_i$ for $i \leq n$ in such a way that condition b) is satisfied for these indices. If $c \in C_n$, the space $\varphi_n(c)$ has a countable covering by non-empty closed sets of diameter $\leq 1/2^{n+1}$, which are mutually disjoint if $X$ [and therefore $\varphi_n(c)$] is zero-dimensional; if $I(c)$ denotes the index set of this covering, we take $c_{n+1}$ to be the sum of the sets $I(c)$ as $c$ runs through $C_n$; for each $c' \in C_{n+1}$, let $p_n(c')$ denote the element $c \in C_n$ such that $c' \in I(c)$, and let $\varphi_{n+1}(c')$ denote the set with index $c'$ in the covering of $\varphi_n(c)$ under consideration. Clearly we thus define by induction a sifting of $X$, and this sifting is strict if $X$ is zero-dimensional; hence Lemma 3.

Now suppose that $X$ is a complete metric space of countable type, and consider a sifting of $X$ by a sieve $C$ and mappings $\varphi_n$. If $\gamma = (c_n)$ is a point of the space $L(C)$ associated with $C$, the sequence $(\varphi_n(c_n))$ is a decreasing sequence of closed sets in $X$ whose diameters tend to 0; the intersection of this sequence of sets consists therefore of a single point, which we denote by $f(\gamma)$. Thus we have defined a mapping $f : L(C) \to X$. If two points $\gamma, \gamma'$ of $L(C)$ have the same $i$-th coordinates for $i \leq n$, it is clear that the distance between $f(\gamma)$ and $f(\gamma')$ is $\leq 1/2^n$, and therefore $f$ is continuous, by virtue of the definition of the topology of $L(C)$. For each $x \in X$ it follows from the definition of a sifting that we can define by induction on $n$ a sequence $\gamma = (c_n)$ such that $x \in \varphi_n(c_n)$ for each $n \geq 0$, and $c_n = p_n(c_{n+1})$; hence $x = f(\gamma)$ and so $f$ is surjective. Furthermore, if the sifting is strict, the sequence $\gamma = (c_n)$ such that $x = f(\gamma)$ is unique, and so in this case $f$ is bijective. $f$ is said to be the mapping induced by the sifting considered.

#### Proposition 13 {#top-ix-s6-prop-13 .statement}

*If $X$ is any Lusin (resp. Souslin) space, there exists a sieve $C$ and a continuous bijection (resp. surjection) of $L(C)$ onto $X$.*

Referring to the definition of a Lusin space (no. 4, Definition 6) [resp. a Souslin space (no. 2, Definition 2)], we reduce to the case where

X is Polish and zero-dimensional (resp. Polish), and the preceding argument then proves the result.

### 6. SEPARATION OF SOUSLIN SETS

#### Theorem 2 {#top-ix-s6-thm-2 .statement}

Let X be a metrizable space. If we are given a sequence $(X_n)$ of mutually disjoint Souslin subspaces of X, then there exists a sequence $(B_n)$ of mutually disjoint Borel sets in X such that $X_n \subset B_n$ for each n.

The proof rests on two lemmas:

#### Lemma 4 {#top-ix-s6-lem-4 .statement}

Let $(A_n), (A'_m)$ be two sequences of subsets of a topological space X. Suppose that for each pair $(A_n, A'_m)$ there is a Borel set $B_{nm}$ of X such that $B_{nm} \supset A_n$ and $B_{nm} \cap A'_m = \emptyset$. Then there is a Borel set B of X which contains $\bigcup_n A_n$ and does not meet $\bigcup_m A'_m$.

For the Borel set $B = \bigcup_n \left( \bigcap_m B_{nm} \right)$ satisfies these conditions.

#### Lemma 5 {#top-ix-s6-lem-5 .statement}

Let X be a Hausdorff space and let A, A' be two disjoint Souslin subspaces of X. Then there is a Borel set B of X such that $B \supset A$ and $B \cap A' = \emptyset$.

By Proposition 13 of no. 5 there exist two sieves C, C' and continuous mappings f of L(C) onto A, $f'$ of L(C') onto A', constructed by the method described in no. 5. For each $n \geq 0$ and each $c \in C_n$, let $q_n(c)$ denote the subspace of L(C) formed of all sequences $(c_k)_{k \geq 0}$ such that $c_n = c$; $q_n(c)$ is a closed subspace of L(C). For each $\gamma = (c_n) \in L(C)$ the sequence of closed sets $q_n(c_n)$ is decreasing and forms a filter base with $\gamma$ as limit. Moreover, for each $c \in C_n$, the sets $q_{n+1}(d)$, where d runs through the set $p_n^{-1}(c)$ in $C_{n+1}$, form a partition of $q_n(c)$. Make the analogous definitions of notation for the sieve $c'$.

We shall argue by contradiction and assume that every Borel set which contains A meets A'. In the first place, it follows from Lemma 4 and the definition of a sifting that there exist $c_0 \in C_0$ and $c'_0 \in C'_0$ such that every Borel set containing $f(q_0(c_0))$ meets $f'(q'_0(c'_0))$. We can then define, by induction on n,

$$
\gamma = (c_n) \in L(C) \quad \text{and} \quad \gamma' = (c'_n) \in L(C')
$$

as follows: suppose that $c_i$ and $c'_i$ have already been defined for $i < n$, in such a way that for each index $i < n$ every Borel set containing $f(q_i(c_i))$ meets $f'(q'_i(c'_i))$; applying Lemma 4 and the definition of a sifting to the sets $f(q_{n-1}(c_{n-1}))$ and $f'(q'_{n-1}(c'_{n-1}))$, we see that there exist $c_n \in C_n$ and $c'_n \in C'_n$ such that $p_{n-1}(c_n) = c_{n-1}$ and $p_{n-1}(c'_n) = c'_{n-1}$ and such that every Borel set containing $f(q_n(c_n))$ meets $f'(q'_n(c'_n))$. Now the sequence $f(q_n(c_n))$ converges to a point $a = f(\gamma) \in A$, and the sequence $f'(q'_n(c'_n))$ converges to a point $a' = f'(\gamma') \in A'$. Since $A \cap A' = \emptyset$ and $X$ is Hausdorff, there is a closed neighbourhood $V$ of $a$ which does not contain $a'$, and thus for $n$ sufficiently large, $V$ contains $f(q_n(c_n))$ and does not meet $f'(q'_n(c'_n))$. This is a contradiction, since $V$ is a Borel set.

To prove Theorem 2, let $Y_n$ denote the union of the sets $X_i$ such that $i \neq n$; then $Y_n$ is a Souslin subspace of $X$ (no. 2, Proposition 8). For each index $n$ there exists a Borel set $B'_n$ which contains $X_n$ and does not meet $Y_n$, by Lemma 5. Let $B_n$ be the intersection of $B'_n$ and $\bigcap_{i < n} (X - B'_i)$. Then the $B_n$ are Borel sets, are mutually disjoint, and are such that $B_n \supset X_n$ for each $n$.

#### Corollary {#top-ix-s6-n6-cor-1 .statement}

*If a countable partition of a metrizable space is formed of Souslin sets, then these sets are Borel sets. In particular, every Souslin set in a metrizable space, whose complement is a Souslin set, is a Borel set.*

### 7. LUSIN SPACES AND BOREL SETS

#### Theorem 3 {#top-ix-s6-thm-3 .statement}

*Let $X$ be a Lusin space. Then a subspace of $X$ is a Lusin space if and only if it is a Borel set.*

This theorem is a consequence of the following two lemmas:

#### Lemma 6 {#top-ix-s6-lem-6 .statement}

*In a Lusin space $X$, every Borel set is a Lusin subspace of $X$.*

Let $\mathfrak{T}$ be the set of all subsets $A$ of $X$ such that both $A$ and $\complement A$ are Lusin subspaces of $X$. Since every closed set and every open set in $X$ is a Lusin subspace of $X$ (no. 4), $\mathfrak{T}$ contains all closed subsets of $X$, and the lemma will therefore be proved if we can show that $\mathfrak{T}$ is a $\sigma$-algebra on $X$. For this it is enough to show that if $(A_n)$ is a sequence of sets of $\mathfrak{T}$, then $\bigcap_n A_n$ and $\bigcup_n A_n$ are Lusin subspaces of $X$. Now we have seen in no. 4 that every countable intersection of Lusin subspaces is a Lusin subspace. On the other hand, if $B_n$ is the intersection of $A_n$ and $\bigcap_{i < n} \complement A_i$, it follows from the hypothesis and the preceding remark that $B_n$ is a Lusin subspace; and since $\bigcup_n A_n = \bigcup_n B_n$, the subspace $\bigcup_n A_n$ is a Lusin subspace by Lemma 2 of no. 4.

#### Lemma 7 {#top-ix-s6-lem-7 .statement}

*Every Lusin subspace $A$ of a metrizable space $X$ is a Borel set in $X$.*

By Proposition 13 of no. 5 there exist a sieve C and a continuous bijection f of L(C) onto A. With the notation of Lemma 5 of no. 6, for each integer n and each c ∈ C_n, let g_n(c) denote the subspace f(q_n(c)) of X; it is a Lusin subspace and therefore a Souslin subspace of X. As c runs through C_n, the sets g_n(c) are pairwise disjoint, because f is bijective; hence, by Theorem 2 of no. 6, there is a family c → g'_n(c) (c ∈ C_n) of Borel sets in X, pairwise disjoint and such that g'_n(c) ⊃ g_n(c) for all c ∈ C_n. Replacing g'_n(c) by its intersection with the closure g_n(c) of g_n(c) in X if necessary, we may suppose that g'_n(c) ⊂ g_n(c). Let c_{n-1}, c_{n-2}, ..., c_0 denote the images of c in C_{n-1}, C_{n-2}, ..., C_0, under the surjections

$$
p_{n-1,n} = p_{n-1},\ p_{n-2,n} = p_{n-2} \circ p_{n-1},\ ...,\ p_{0n} = p_0 \circ p_1 \circ ... \circ p_{n-1}
$$

respectively; and let h_n(c) denote the intersection of the sets

g'_n(c),\ g'_{n-1}(c_{n-1}),\ ...\ ,\ g'_0(c_0).

Since q_i(c_i) ⊃ q_n(c) for 0 ≤ i ≤ n − 1, h_n(c) contains g_n(c); it is clear also that h_n(c) is a Borel set and is contained in g_n(c), and that as c runs through C_n, the h_n(c) are mutually disjoint sets; finally, by construction, for each c' ∈ C_{n+1} we have h_{n+1}(c') ⊂ h_n(p_n(c')). Let then B_n be the union of the sets h_n(c) as c runs through C_n; B_n is a Borel set, and B_{n+1} ⊂ B_n; also B_n contains the union of the sets g_n(c) (c ∈ C_n), which is A. Let B be the intersection of the decreasing sequence of sets B_n; B is a Borel set and contains A. We shall show that B = A, and this will complete the proof.

Let x be a point of B. Then, for each integer n, there exists a unique c ∈ C_n such that x ∈ h_n(c); let us denote this c by c_n(x). The sequence (c_n(x))_{n≥0} belongs to L(C). The decreasing sequence (g_n(c_n(x))) converges by definition to a point a ∈ A; the sequence of closures of these sets also converges to a in X, hence a fortiori so does the sequence (h_n(c_n(x))). Now x belongs to all the sets h_n(c_n(x)), therefore x = a ∈ A. Lemma 7 is thus proved, and with it Theorem 3.

#### Corollary {#top-ix-s6-n7-cor-1 .statement}

*If f is a continuous injective mapping of a Lusin space (or, in particular, a Polish space) X into a metrizable space Y, then f(X) is a Borel set in Y.*

### 8. BOREL SECTIONS

#### Theorem 4 {#top-ix-s6-thm-4 .statement}

*Let X be a Polish space and let R be an equivalence relation on X, such that the equivalence classes mod R are closed in X and the saturation (with respect to R) of each closed set in X is a Borel set. Then there is a Borel set in X which meets each equivalence class in exactly one point.*

Consider a metric on $X$ compatible with its topology, and with respect to which $X$ is complete. By Lemma 3 of no. 5, there exists a sifting of $X$, defined by a sieve $C = (C_n, p_n)$ and a sequence of mappings $(\varphi_n)$. For each $c \in C_n$, let $g_n(c)$ be the saturation of the closed set $\varphi_n(c)$ with respect to $R$; by hypothesis, $g_n(c)$ is a Borel set in $X$.

Since each set $C_n$ is countable, we can linearly order each $C_n$ in such a way that the set of elements smaller than a given element is finite. For each $c \in C_n$ we define a set $h_n(c)$ by induction on $n$, as follows. In the first place, for $c \in C_0$, $h_0(c)$ is the intersection of $\varphi_0(c)$ and the sets $X - g_0(c')$, where $c' \in C_0$ and $c' < c$. For $c \in C_{n+1}$, $h_{n+1}(c)$ is the intersection of $\varphi_{n+1}(c), h_n(P_n(c))$ and the sets $X - g_{n+1}(c')$ for $c' \in C_{n+1}$, $p_n(c') = p_n(c)$ and $c' < c$. The $h_n(c)$ are clearly Borel sets.

We shall prove the following assertion: for each integer $n \geq 0$ and each equivalence class $H$ mod $R$, there is a unique element $c \in C_n$ such that $h_n(c)$ meets $H$, and we have
$$
h(c_n) \cap H = \varphi_n(c) \cap H,
$$
which is therefore a *closed* set. For $n = 0$, consider the smallest element $c \in C_0$ such that $\varphi_0(c)$ meets $H$; then $\varphi_0(c) \cap H$ does not meet any set $g_0(c')$ for which $c' \in C_0$ and $c' < c$; hence it is contained in $h_0(c) \cap H$ and consequently is equal to this set; moreover, we have $H \subset g_0(c)$ and therefore $h_0(c') \cap H$ is empty for $c' \in C_0$ and $c' > c$; thus the assertion is proved for $n = 0$. We continue by induction on $n$: if there exists $c \in C_{n+1}$ such that $h_{n+1}(c)$ meets $H$, then it follows from the relation $h_{n+1}(c) \subset h_n(p_n(c))$ and the inductive hypothesis that $p_n(c)$ is the unique element $d \in C_n$ such that $h_n(d)$ meets $H$. Observe that $h_n(d)$, which is contained in $\varphi_n(d)$, is contained in the union of the sets $\varphi_n(c)$ for which $c \in p_n^{-1}(d)$, by the definition of a sifting; there is therefore a smallest element $c \in p_n^{-1}(d)$ such that $\varphi_{n+1}(c)$ meets $H$. We have therefore
$$
\varphi_{n+1}(c) \cap H \subset \varphi_n(d) \cap H = h_n(d) \cap H
$$
by the inductive hypothesis. Hence
$$
\varphi_{n+1}(c) \cap H \subset \varphi_{n+1}(c) \cap h_n(d),
$$
and since by definition $\varphi_{n+1}(c) \cap H$ meets none of the sets $g_{n+1}(c')$ for which $c' \in p_n^{-1}(d)$ and $c' < c$, it follows from the definition of $h_{n+1}(c)$ that $\varphi_{n+1}(c) \cap H = h_{n+1}(c) \cap H$. Moreover, we have $H \subset g_{n+1}(c)$ and therefore, if $c' \in p_n^{-1}(d)$ is such that $c' > c$, $h_{n+1}(c') \cap H$ is empty. Hence the assertion is proved for all $n$.

For each integer $n$, let $S_n$ be the union of the sets $h_n(c)$, where $c$ runs through $C_n$. The set $S_n$ is a Borel set, and we have $S_{n+1} \subset S_n$.

Let S be the intersection of the sets S_n, which is also a Borel set in X; we shall show that S meets each equivalence class H mod R in exactly one point. For each n, let c_n(H) be the unique element c \in C_n such that h_{c_n(H)} meets H; then S_n \cap H = \varphi_n(c_n(H)) \cap H, and S \cap H is the intersection of the sets \varphi_n(c_n(H)) \cap H. Since the sequence (c_n(H)) belongs to L.C., the decreasing sequence of closed sets \varphi_n(c_n(H)), whose diameter tends to 0, converges to a point x \in X, since X is complete. The intersection of the closed sets \varphi_n(c_n(H)) \cap H therefore consists of the point x alone, and the proof of Theorem 4 is complete.

#### Remark {#top-ix-s6-n8-rem-1 .statement}

In particular a closed equivalence relation R satisfies the hypotheses of Theorem 4. When X is a compact metrizable space, Theorem 4 therefore applies to any Hausdorff equivalence relation R, since a Hausdorff equivalence relation on a compact space is closed (Chapter I, § 10, no. 4, Proposition 8).

### 9. CAPACITABILITY OF SOUSLIN SETS

#### Definition 8 {#top-ix-s6-def-8 .statement}

Let X be a Hausdorff topological space. A capacity on X is a mapping f of the set \mathcal{P}(X) of all subsets of X into the extended real line \overline{\mathbf{R}}, satisfying the following conditions:

(CA_1) If A \subset B, then f(A) \leq f(B).

(CA_2) If (A_n) is any increasing sequence of subsets of X, then
$$
f\left(\bigcup_n A_n\right) = \sup_n f(A_n).
$$

(CA_3) If (K_n) is any decreasing sequence of compact subsets of X, then
$$
f\left(\bigcap_n K_n\right) = \inf_n f(K_n).
$$

#### Example {#top-ix-s6-n9-exa-1 .statement}

\* Let \mu be a positive measure on a locally compact space X; then the corresponding outer measure \mu^* is a capacity on X.
It can be shown that in Euclidean space \mathbf{R}^n (n \geq 3), the "Newtonian outer capacity" is a capacity in the sense of Definition 8.

#### Definition 9 {#top-ix-s6-def-9 .statement}

Let f be a capacity on X; a subset A of X is said to be capacitable (with respect to f) if $f(A) = \sup_k f(K)$, where K runs through the set of compact subsets of A.

\* For example, if f is an outer measure \mu^*, every open set is capacitable; the capacitable sets A such that \mu^*(A) < +\infty are precisely the \mu-integrable sets. \*

#### Proposition 14 {#top-ix-s6-prop-14 .statement}

Let K be a compact space and let f be a capacity on K. If A is the intersection of a decreasing sequence $(A_n)$ of subsets of K, each of which is a countable union of closed sets, then A is capacitable.

It is enough to show that, for each $a < f(A)$, there is a closed set $C \subset A$ such that $f(C) \geq a$. Let us first show that there exists a sequence $(B_n)_{n \geq 1}$ of closed sets such that $B_n \subset A_n$ and such that, if we define a sequence $(C_n)$ inductively by the conditions $C_0 = A, C_n = C_{n-1} \cap B_n$ for $n \geq 1$, then $f(C_n) > a$ for each $n \geq 0$. Suppose the $B_i$ have been defined for $i < n$; by hypothesis we have $C_{n-1} \subset A \subset A_n$ and $f(C_{n-1}) > a$; since $A_n$ is the union of an increasing sequence of closed sets $D_j$, it follows from (CAII) that
$$
f(C_{n-1}) = \sup_j f(C_{n-1} \cap D_j).
$$
Hence there is an index $j$ such that $f(C_{n-1} \cap D_j) > a$, and we may take $B_n = D_j$.

Now let $C = \bigcap_n C_n$. Since $A = \bigcap_n A_n$ and $B_n \subset A_n$, we have
$$
C = \bigcap_n B_n;
$$
the set C is therefore compact and contained in A.

Let $B'_n = B_1 \cap B_2 \cap \cdots \cap B_n$; $(B'_n)$ is a decreasing sequence of compact subsets of K; as $C_n \subset C_i \subset B_i$ for $i < n$ we also have $C_n \subset B'_n$. By (CAIII), $f(C) = \inf_n f(B'_n)$, and since $C \subset C_n \subset B'_n$ we also have $f(C) = \inf_n f(C_n) \geq a$. This completes the proof.

#### Theorem 5 {#top-ix-s6-thm-5 .statement}

Let X be a metrizable space and let Y be a relatively compact Souslin subspace of X. Then Y is capacitable with respect to every capacity f on X.

We have seen (no. 2, Proposition 9) that there exists a compact space K, a decreasing sequence $(A_n)$ of subsets of K, each of which is a countable union of compact sets, and a continuous mapping $\varphi : K \to X$ such that $Y = \varphi \left( \bigcap_n A_n \right)$. By Proposition 14, $\bigcap_n A_n$ is capacitable with respect to every capacity on K. Theorem 5 is therefore a consequence of the following proposition:

#### Proposition 15 {#top-ix-s6-prop-15 .statement}

Let $\varphi$ be a continuous mapping of a Hausdorff space K into a Hausdorff space X, and let f be a capacity on X. If for each subset A of K we put $g(A) = f(\varphi(A))$, then g is a capacity on K; moreover, if A is capacitable with respect to g, then $\varphi(A)$ is capacitable with respect to f.

It is clear that $g$ satisfies axioms $(\mathrm{CA}_I)$ and $(\mathrm{CA}_{II})$. On the other hand, let $(C_n)$ be a decreasing sequence of compact subsets of $K$, and let $C = \bigcap_n C_n$; the sets $\varphi(C)$ are compact, and their intersection is $\varphi(C)$; for this intersection certainly contains $\varphi(C)$, and if $x \in \varphi(C_n)$ for all $n$, then the sets $\overline{\varphi^1}(x) \cap C_n$ form a decreasing sequence of non-empty compact subsets of $K$, and therefore their intersection is not empty. We have therefore $f(\varphi(C)) = \inf_n f(\varphi(C_n))$, that is $g(C) = \inf_n g(C_n)$; thus $g$ satisfies axiom $(\mathrm{CA}_{III})$ and is therefore a capacity on $K$.

Now let $A$ be a subset of $K$ which is capacitable with respect to $g$; if $a < f(\varphi(A)) = g(A)$, then there is a compact set $C \subset A$ such that $g(C) \geq a$; thus $\varphi(C)$ is a compact set contained in $\varphi(A)$, and $f(\varphi(C)) \geq a$. This shows that $\varphi(A)$ is capacitable with respect to $f$, and completes the proof of Proposition 15 and hence of Theorem 5.

#### Remark {#top-ix-s6-n9-rem-1 .statement}

\* If $\mu$ is a positive measure on a locally compact metrizable space $X$, then every Souslin subset $A$ of $X$ is $\mu$-measurable. For if $K$ is any compact subset of $X$, $K \cap A$ is a relatively compact Souslin set, hence is capacitable with respect to $\mu^*$ and consequently $\mu$-integrable. Note that the complement in $X$ of a Souslin set, although not in general a Souslin set, is $\mu$-measurable *.

### Exercises {#top-ix-s6-exercises}

See the [exercises for § 6](exercises/s6/).
