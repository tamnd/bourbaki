---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 4
section_title: Relations between uniform spaces and compact spaces
lang: en
source: top-i-iv
pdf_pages: 0204-0211, 0215-0221
extraction: ocr
subsections:
    - "no": 1
      title: UNIFORMITY OF COMPACT SPACES
      page: 0
      pdf_page: 204
    - "no": 2
      title: COMPACTNESS OF UNIFORM SPACES
      page: 0
      pdf_page: 207
    - "no": 3
      title: COMPACT SETS IN A UNIFORM SPACE
      page: 0
      pdf_page: 209
    - "no": 4
      title: CONNECTED SETS IN A COMPACT SPACE
      page: 0
      pdf_page: 210
statements: 24
exercises: 23
content_sha256: 33d413c1fed78b55146ebc22613f337b5e448d7bf43b8d118b1324178c5c0724
---

## 4. RELATIONS BETWEEN UNIFORM SPACES AND COMPACT SPACES

### 1. UNIFORMITY OF COMPACT SPACES

#### Definition 1 {#top-ii-s4-def-1 .statement}

*A uniformity on a topological space $X$ is said to be compatible with the topology of $X$ if the latter coincides with the topology induced by the uniformity.*

A topological space is said to be uniformizable, and its topology is said to be uniformizable, if there exists a uniformity on the space which is compatible with its topology.

There are topological spaces which are not uniformizable, for example any space which does not satisfy axiom $(O_{III})$ ($\S 1$, no. 2, Corollary 3 of Proposition 2); hence the question arises of determining under what conditions a topological space is uniformizable.

We shall not give a complete answer to this question until Chapter IX, $\S 1$. In this section we shall examine only one important particular case, that in which $X$ is compact. We have then the following theorem:

#### Theorem 1 {#top-ii-s4-thm-1 .statement}

*On a compact space $X$ there is exactly one uniformity compatible with the topology of $X$; the entourages of this uniformity are all the neighbourhoods of the diagonal $\Delta$ in $X \times X$. Furthermore, $X$ endowed with this uniformity is a complete uniform space.*

The last part of the theorem is straightforward; for every Cauchy filter on $X$ has a cluster point [axiom (C)] and is therefore convergent ($\S 3$, no. 2, Proposition 5, Corollary 2).

Let us show next that if there is a uniformity on $X$ compatible with the topology of $X$, then the set $U$ of entourages of this uniformity is the set of all neighbourhoods of $\Delta$. We know already that every entourage is a neighbourhood of $\Delta$ ($\S 1$, no. 2, Proposition 2), hence we have to show that conversely every neighbourhood of $\Delta$ belongs to $U$. Suppose that there is a neighbourhood $U$ of $\Delta$ which is not in $U$; then the sets $V \cap C_U$, as $V$ runs through $U$, form a base of a filter $G$ on the compact space $X \times X$; consequently $G$ has a cluster point $(a, b)$ not belonging to $\Delta$. Since $U$ is a filter coarser than $G$, $(a, b)$ is also a cluster point of $U$. But the uniformity defined by $U$ is Hausdorff by hypothesis; hence the intersection of the closures of the sets of $U$ is $\Delta$ ($\S 1$, no. 2, Corollary 2 to Proposition 2 and Proposition 3); thus we arrive at a contradiction.

It remains therefore to show that the set $B$ of neighbourhoods of $\Delta$ in $X \times X$ is the set of entourages of a uniformity compatible with the topology of $X$. For this it is enough to show that $B$ is the set of entourages of a *Hausdorff* uniformity on $X$; for then the topology induced by this uniformity will be *coarser* than the topology of $X$ (Chapter I, $\S 2$, no. 2, Proposition 3) and must therefore coincide with the latter (Chapter I, $\S 9$, no. 4, Theorem 2, Corollary 3).

$B$ clearly satisfies axioms $(F_I)$ and $(F_{II})$. Let us show that axioms $(U_{II})$ and $(U_{III})$ are also satisfied and that $\Delta$ is the intersection of the sets of $B$. Take the last point first: every set consisting of a single point $(x, y) \in X \times X$ is closed, since $X$ is Hausdorff; hence if $x \neq y$, the complement of $(x, y)$ in $X \times X$ is a neighbourhood of $\Delta$. Since the symmetry $(x, y) \to (y, x)$ is a homeomorphism of $X \times X$ onto itself,

$$
W = \bigcup_{i=1,2,3} (U_i \times U_i) \text{ of } \Delta \text{ in } X \times X.
$$

It follows immediately from these definitions that if $(u, v) \in W$ and $u \in V_1$ (resp. $u \in U_1$), then we must have $v \in U_1$ (resp. $v \in U_1 \cup U_3 = \mathcal{C}V_2$); hence the neighbourhood $V_1 \times V_2$ of $(x, y)$ in $X \times X$ does not meet $\hat{W}$, and we have a contradiction. This completes the proof.

#### Remark 1 {#top-ii-s4-n1-rem-1 .statement}

For every *finite open covering* $\mathcal{R} = (U_i)_{1 \leq i \leq n}$ of $X$, the set

$$
V_{\mathcal{R}} = \bigcup_{i=1}^n (U_i \times U_i)
$$

is a neighbourhood of $\Delta$ in $X \times X$, and these sets $V_{\mathcal{R}}$ form a *fundamental system of neighbourhoods* of $\Delta$ (and therefore a *fundamental system of entourages* of the unique uniformity on $X$). Let $W$ be any neighbourhood of $\Delta$ in $X \times X$; then for each $x \in X$ there is an open neighbourhood $U_x$ of $x$ in $X$ such that $U_x \times U_x \subset W$. Since the $U_x$ ($x \in X$) form an open covering of $X$, there exist a finite number of points $x_i$ ($1 \leq i \leq n$) such that the $U_{x_i}$ ($1 \leq i \leq n$) form a covering $\mathcal{R}$ of $X$. We have then $V_{\mathcal{R}} \subset W$, which proves the assertion.

For this reason the unique uniformity on $X$ is often called the *uniformity of finite open coverings* (cf. Chapter IX, § 4, Exercise 17).

#### Corollary 1 {#top-ii-s4-thm-1-cor-1 .statement}

*Every subspace of a compact space is uniformizable.*

#### Corollary 2 {#top-ii-s4-thm-1-cor-2 .statement}

*Every locally compact space is uniformizable.*

For by Alexandroff’s theorem (Chapter I, § 9, no. 8, Theorem 4) a locally compact space is homeomorphic to a subspace of a compact space.

#### Remark 2 {#top-ii-s4-n1-rem-2 .statement}

It can happen that there are several distinct uniformities compatible with the topology of a locally compact space.

For example, we have seen that on an infinite discrete space there is more than one distinct uniformity compatible with the discrete topology (§ 2, no. 2, Remark).

Nevertheless it is not the case that the uniqueness of the uniformity compatible with the topology of a uniformizable space is a property which characterizes compact spaces; there exist locally compact spaces which are not compact but whose uniformity is unique (Exercise 4).

#### Theorem 2 {#top-ii-s4-thm-2 .statement}

Every continuous mapping $f$ of a compact space $X$ into a uniform space $X'$ is uniformly continuous.

Let $g = f \times f$, then $g$ is continuous on $X \times X$ (Chapter I, § 4, no. 1, Proposition 1, Corollary 1); hence for each open entourage $V'$ of $X'$, $\overline{g^{-1}}(V')$ is an open subset of $X \times X$, which evidently contains the diagonal. The theorem thus follows from Theorem 1, since the open entourages of $X'$ form a fundamental system of entourages (§ 1, no. 2, Proposition 2, Corollary 2).

Under the hypotheses of Theorem 2, the restriction of $f$ to any subspace $A$ of $X$ is uniformly continuous; hence (§ 3, no. 6, Theorem 2):

#### Corollary {#top-ii-s4-n1-cor-1 .statement}

Let $A$ be a dense subspace of a compact space $X$, and let $f$ be a mapping of $A$ into a complete Hausdorff uniform space $X'$. Then $f$ can be extended by continuity to the whole of $X$ if and only if $f$ is uniformly continuous.

### 2. COMPACTNESS OF UNIFORM SPACES

#### Definition 2 {#top-ii-s4-def-2 .statement}

A uniform space $X$ is said to be precompact if its Hausdorff completion $\hat{X}$ is compact. A subset $A$ of a uniform space $X$ is said to be a precompact subset if the uniform subspace $A$ of $X$ is precompact.

Thus a subset $A$ of a uniform space $X$ is precompact if and only if the closure of $i(A)$ in $\hat{X}$ is compact ($i : X \to \hat{X}$ being the canonical map) (§ 3, no. 9, Proposition 18, Corollary 1).

#### Example {#top-ii-s4-n2-exa-1 .statement}

In any uniform space $X$, the set of points of a Cauchy sequence $(x_n)$ is precompact. Since the images of the $x_n$ in $\hat{X}$ again form a Cauchy sequence, we can assume that $X$ is Hausdorff; the closure in $\hat{X}$ of the set of points $x_n$ then consists of the points $x_n$ and $\lim_{n \to \infty} x_n$ and is therefore compact (Chapter I, § 9, no. 3, Example 2).

#### Theorem 3 {#top-ii-s4-thm-3 .statement}

A uniform space $X$ is precompact if and only if, for each entourage $V$ of $X$, there is a finite covering of $X$ by $V$-small sets.

We may express this condition more intuitively by saying that $X$ can be covered by a finite number of sets which are as small as we please.

Let $i : X \to \hat{X}$ be the canonical mapping, then the entourages of $X$ are the inverse images under $i \times i$ of the entourages of $\hat{X}$ (\S 3, no. 7, Proposition 12). Suppose $X$ is precompact, and let $U$ be any entourage of $\hat{X}$; then there is a symmetric entourage $U'$ of $\hat{X}$ such that $\hat{U}' \subset U$. Since $\hat{X}$ is compact, there exist a finite number of points $x_j \in \hat{X}$ such that the $U'(x_j)$ (which are $U$-small) cover $\hat{X}$. If $V$ is the inverse image of $U$ by $i \times i$, the sets $i^{-1}(U'(x_j))$ are $V$-small and cover $X$. Conversely, suppose that for each entourage $V$ of $X$ there is a finite covering of $X$ by $V$-small sets. We have to show that every ultrafilter $\mathfrak{F}$ on $\hat{X}$ is convergent; since $\hat{X}$ is complete, it is enough to show that $\mathfrak{F}$ is a *Cauchy filter*, i.e. that for each *closed* entourage $U$ of $\hat{X}$ there is a $U$-small set in $\mathfrak{F}$ (\S 1, no. 2, Proposition 2, Corollary 2). Let $V$ be the inverse image of $U$ under $i \times i$, and let $(B_j)$ be a finite covering of $X$ by $V$-small sets; then the sets $C_j = i(B_j)$ are $U$-small and cover $i(X)$, so that
$$
\hat{X} = \bigcup_j \overline{C}_j.
$$
On the other hand, since $C_j \times C_j \subset U$, and $U$ is closed in $\hat{X} \times \hat{X}$, we have $\overline{C}_j \times \overline{C}_j \subset U$, so that the $\overline{C}_j$ are also $U$-small. Since $\mathfrak{F}$ is an ultrafilter, one of the $\overline{C}_j$ belongs to $\mathfrak{F}$ (Chapter I, \S 6, no. 4, Corollary to Proposition 5).

Q.E.D.

#### Corollary {#top-ii-s4-n2-cor-1 .statement}

*A uniform space $X$ is compact if and only if it is Hausdorff and complete and can be covered by a finite number of $V$-small sets, where $V$ is any entourage of $X$.*

This follows from Theorem 3 and Theorem 1 of no. 1.

#### Remark 1 {#top-ii-s4-n2-rem-1 .statement}

A non-Hausdorff *quasi-compact* space is not necessarily uniformizable, since it need not satisfy axiom $(O_{III})$ (cf. Chapter I, \S 9, no. 2); for example most of the non-Hausdorff quasi-compact spaces which appear in algebraic geometry do not satisfy axiom $(O_{III})$ (cf. Exercise 2).

#### Proposition 1 {#top-ii-s4-prop-1 .statement}

*In a uniform space every subset of a precompact set, every finite union of precompact sets and the closure of every precompact set are precompact.*

The first two assertions are immediate consequences of Theorem 3. Let $X$ be a uniform space, $A$ a precompact subset of $X$, and let $i : X \to \hat{X}$ be the canonical mapping. $i(\overline{A})$ is contained in the closure of $i(A)$ in $\hat{X}$ (Chapter I, \S 2, no. 1, Theorem 1), hence the closure of $i(\overline{A})$ in $\hat{X}$ is contained in a compact set and is therefore compact.

#### Remark 2 {#top-ii-s4-n2-rem-2 .statement}

In a uniform space $X$ a *relatively compact* set $A$ is *precompact*, since $A$ is contained in a compact set. On the other hand, even if $X$ is Hausdorff, a precompact set *need not be relatively compact* in $X$, as is shown by the case where $X$ itself is precompact but not compact.

#### Proposition 2 {#top-ii-s4-prop-2 .statement}

*Let $f : X \to Y$ be a uniformly continuous mapping. If $A$ is any precompact subset of $X$, then $f(A)$ is a precompact subset of $Y$.*

For if $i : X \to \hat{X}$ and $j : Y \to \hat{Y}$ are the canonical mappings, we have $j(f(A)) = \hat{f}(i(A))$ (\S 3, no. 7, Proposition 15) and hence $j(f(A))$ is relatively compact in $\hat{Y}$ (Chapter I, \S 9, no. 4, Theorem 2, Corollary 1).

#### Proposition 3 {#top-ii-s4-prop-3 .statement}

*Let $X$ be a set, let $(Y_\lambda)_{\lambda \in L}$ be a family of uniform spaces, and for each $\lambda \in L$ let $f_\lambda$ be a mapping of $X$ into $Y_\lambda$. Let $X$ carry the coarsest uniformity for which the $f_\lambda$ are uniformly continuous. Then a subset $A$ of $X$ is precompact if and only if $f_\lambda(A)$ is a precompact subset of $Y_\lambda$ for each $\lambda \in L$.*

The condition is necessary by virtue of Proposition 2. Sufficiency follows from the characterization of the Hausdorff completion of $X$ given in \S 3, no. 9, Proposition 18, and Tychonoff’s theorem (Chapter I, \S 9, Theorem 3, Corollary).

### 3. COMPACT SETS IN A UNIFORM SPACE

The following proposition for an arbitrary uniform space is a sharper form of Proposition 2 of Chapter I, \S 9, no. 2 for compact spaces.

#### Proposition 4 {#top-ii-s4-prop-4 .statement}

*In a uniform space $X$, let $A$ be a compact set and $B$ a closed set such that $A \cap B = \varnothing$. Then there is an entourage $V$ of $X$ such that $V(A)$ and $V(B)$ do not intersect.*

If the proposition were false, then none of the sets $A \cap \overline{V}(B)$, where $V$ runs through the set of symmetric entourages of $X$, would be empty; hence these sets would form a filter base on $A$, which would have a cluster point $x_0 \in A$. Hence for each symmetric entourage $V$ of $X$, $\overline{V}(x_0)$ would meet $B$ and therefore, as $B$ is closed, we should have $x_0 \in B$, contrary to hypothesis.

#### Corollary {#top-ii-s4-n3-cor-1 .statement}

*Let $A$ be a compact set in a uniform space $X$; then as $V$ runs through the set of entourages of $X$, the sets $V(A)$ form a fundamental system of neighbourhoods of $A$.*

Let $U$ be any open neighbourhood of $A$, then $B = \complement U$ is closed and does not meet $A$; hence, by Proposition 4, there is an entourage $V$ such that $V(A) \cap V(B) = \varnothing$, and therefore $V(A) \subset U$.

### 4. CONNECTED SETS IN A COMPACT SPACE

#### Definition 3 {#top-ii-s4-def-3 .statement}

*Let $V$ be a symmetric entourage of a uniform space $X$. A finite sequence $(x_i)_{0 \leq i \leq n}$ of points of $X$ is said to be a $V$-chain if $x_i$ and $x_{i+1}$ are $V$-close for $0 \leq i < n$. The points $x_0$ and $x_n$ are called the ends of the $V$-chain, and they are said to be joined by the $V$-chain.*

Given a symmetric entourage $V$, the relation "there is a $V$-chain joining $x$ and $y$" is an equivalence relation between $x$ and $y$ in $X$. Let $A_{x, v}$ be the equivalence class of $x$ for this relation, i.e. the set of all $y \in X$ which can be joined to $x$ by a $V$-chain. Clearly if $y \in A_{x, v}$ then $V(y) \subset A_{x, v}$; hence $A_{x, v}$ is open in $X$; and the complement of $A_{x, v}$, being a union of equivalence classes, is also open. Hence:

#### Proposition 5 {#top-ii-s4-prop-5 .statement}

*In a uniform space $X$, the set $A_{x, v}$ of points which can be joined by a $V$-chain to a given point $x$ is both open and closed in $X$.*

For each $x \in X$, let $A_x$ denote the intersection of the sets $A_{x, v}$ as $V$ runs through the set of symmetric entourages of $X$; $A_x$ is the equivalence class of $x$ for the equivalence relation "for all symmetric entourages $V$, there is a $V$-chain joining $x$ and $y$".

#### Proposition 6 {#top-ii-s4-prop-6 .statement}

*In a compact space $X$, the component of $x$, the set $A_x$, and the intersection of the neighbourhoods of $x$ which are both open and closed, are all three identical.*

It is enough to show that $A_x$ is *connected*: for in any uniform space $X$ the component of $x$ is contained in the intersection of the neighbourhoods of $x$ which are both open and closed, and this intersection is contained in $A_x$ by Proposition 5.

Suppose $A_x$ is not connected. Since $A_x$ is *closed*, there are two non-empty disjoint closed sets $B$ and $C$ such that $B \cup C = A_x$. By Proposition 4 of § 3 there is an entourage $U$ of $X$ such that $U(B) \cap U(C)$ is empty.

Let $W$ be an *open* entourage such that $\hat{W} \subset U$, and let $H$ be the *closed* set which is the complement of $W(B) \cup W(C)$ in $X$. Suppose for example that $x \in B$, and let $y$ be a point of $C$. Then for each symmetric entourage $V \subset W$ one sees immediately, by induction on $i$, that every $V$-chain $(x_i)_{0 \leq i \leq n}$ joining $x$ and $y$ in $X$ must have a point in $H$, by the choice of $W$. Since by hypothesis $x$ and $y$ can be joined by a $V$-chain for each symmetric entourage $V$, we see that $H \cap A_{x, v}$ is not empty if $V \subset W$. On the other hand, if $V' \subset V$ then clearly $A_{x, v'} \subset A_{x, v}$; thus it follows that, as $V$ runs through the set of symmetric entourages of $X$, the sets $H \cap A_{x, v}$ form a filter base of *closed* sets in the compact space $H$. Hence all these sets have a common point and therefore $H$ meets $A_x$; but this contradicts the definition of $H$.

#### Corollary {#top-ii-s4-n4-cor-1 .statement}

*Let X be a locally compact space and let K be a compact component of X. Then the neighbourhoods of K which are both open and closed form a fundamental system of neighbourhoods of K.*

Let V be a relatively compact open neighbourhood of K in X (Chapter I, § 9, no. 7, Proposition 10) and let F be its frontier. Let U ⊂ \overline{V} be a set which is both open and closed *with respect to* \overline{V}. Then U is closed in X, and if in addition U does not meet F, then U is open in X (for then U ⊂ V and U is open in V). Hence it is enough to show that there is a subset of \overline{V} which contains K, does not meet F and is both open and closed with respect to \overline{V}.

Suppose this is not the case: then the intersections of F with the subsets of \overline{V} which contain K and are open and closed in \overline{V} form a filter base of closed sets in F; F is compact, so these sets have a common point y ∈ F. But this is absurd; since \overline{V} is compact, K is a component of \overline{V}, and by virtue of Proposition 6, the intersection of the sets which contain K and are both open and closed in \overline{V} is just K. The Corollary is thus proved.

#### Proposition 7 {#top-ii-s4-prop-7 .statement}

*Let X be a compact space and let R be the equivalence relation on X whose classes are the components of X. Then the quotient space X/R is compact and totally disconnected.*

We know from Chapter I, § II, no. 5, Proposition 9 that X/R is totally disconnected; hence we have to show that X/R is *Hausdorff* (Chapter I, § 10, no. 4, Proposition 8.) Let A and B be two distinct components of X. By Proposition 6 there is a symmetric entourage U of X such that no point of A can be joined to any point of B by a U-chain. The set V (resp. W) of points of X which can be joined to a point x ∈ A (resp. y ∈ B) by a U-chain is both open and closed in X (Proposition 5) and contains A (resp. B); these sets are therefore open neighbourhoods of A and B respectively, are saturated with respect to R and do not intersect. This completes the proof.

### Exercises {#top-ii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
