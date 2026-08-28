---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 3
section_title: Subspaces, quotient spaces
lang: en
source: top-i-iv
pdf_pages: 0041-0049, 0128-0131
extraction: ocr
subsections:
    - "no": 1
      title: SUBSPACES OF A TOPOLOGICAL SPACE
      page: 0
      pdf_page: 41
    - "no": 2
      title: CONTINUITY WITH RESPECT TO A SUBSPACE
      page: 0
      pdf_page: 43
    - "no": 3
      title: LOCALLY CLOSED SUBSPACES
      page: 0
      pdf_page: 44
    - "no": 4
      title: QUOTIENT SPACES
      page: 0
      pdf_page: 45
    - "no": 5
      title: CANONICAL DECOMPOSITION OF A CONTINUOUS MAPPING
      page: 0
      pdf_page: 46
    - "no": 6
      title: QUOTIENT SPACE OF A SUBSPACE
      page: 0
      pdf_page: 48
statements: 24
exercises: 16
content_sha256: 3268e44c8c9d9e92545692b234c169a265647c5944508f6c4bba34e83499677d
---

## 3. SUBSPACES; QUOTIENT SPACES

### 1. SUBSPACES OF A TOPOLOGICAL SPACE

Let $A$ be a subset of a topological space $X$. We have defined the *topology induced* on $A$ by the topology of $X$ as the inverse image of the latter under the canonical injection $A \to X$ (§ 2, no. 3, Example 1). An equivalent definition is as follows:

#### Definition 1 {#top-i-s3-def-1 .statement}

Let $A$ be a subset of a topological space $X$. The topology induced on $A$ by the topology of $X$ is that in which the open sets are the intersections with $A$ of open sets of $X$. The set $A$ with this topology is called a subspace of $X$.

#### Example {#top-i-s3-n1-exa-1 .statement}

The topology induced on the set $\mathbf{Z}$ of rational integers by the topology of the rational line is the discrete topology, for the intersection of $\mathbf{Z}$ and the open interval $]n - 1/2, n + 1/2[$ is the set $\{ n \}$.

By Proposition 5 of § 2, no. 3 (or directly from Definition 1) we see that, if $B \subset A \subset X$, the subspace $B$ of $X$ is identical with the subspace $B$ of the subspace $A$ of $X$ (transitivity of induced topologies). If $\mathcal{G}$ is a subbase (resp. a base) of the topology of $X$ ($§ 2$, no. 3, Example 3) its trace $\mathcal{G}_A$ on $A$ is a subbase (resp. a base) of the topology induced on $A$.

In all questions which involve the elements or subsets of $A$, it is essential to distinguish carefully between their properties as points (resp. subsets) of $X$, and their properties as points (resp. subsets) of the subspace $A$. We shall make this distinction by using the phrases "in $A$", "with respect to $A$", or "relative to $A$" to refer to properties in the latter category (possibly contrasting them with the phrases "in $X$", "with respect to $X$", "relative to $X$").

An open set of the subspace $A$ need not be open in $X$; in order that every set which is open in $A$ should be open in $X$ it is necessary and sufficient that $A$ is open in $X$. The condition is necessary, since $A$ is open in $A$, and it is sufficient by virtue of $(O_{II})$ and Definition 1.

The sets which are closed in $A$ are the intersections with $A$ of the closed sets in $X$ ($§ 2$, no. 3, Example 1); as above we see that every set which is closed in $A$ is closed in $X$ if and only if $A$ is closed in $X$.

The neighbourhoods of a point $x \in A$ relative to $A$ are the intersections with $A$ of neighbourhoods of $x$ relative to $X$. Every neighbourhood of $x$ relative to $A$ is a neighbourhood of $x$ relative to $X$ if and only if $A$ is a neighbourhood of $x$ in $X$.

#### Proposition 1 {#top-i-s3-prop-1 .statement}

If $A$ and $B$ are two subsets of a topological space $X$, and $B \subset A$, then the closure of $B$ in the subspace $A$ is the intersection with $A$ of the closure $\overline{B}$ of $B$ in $X$.

If $x \in A$, every neighbourhood of $x$ in $A$ is of the form $V \cap A$, where $V$ is a neighbourhood of $x$ in $X$. Since $V \cap B = (V \cap A) \cap B$, it follows that $x$ lies in the closure of $B$ with respect to $A$ if and only if $x$ lies in the closure of $B$ with respect to $X$.

#### Corollary {#top-i-s3-n1-cor-1 .statement}

A subset $B$ of $A$ is dense in $A$ if and only if $\overline{B} = \overline{A}$ in $X$ (i.e. if and only if $A \subset \overline{B}$).

It follows that if $A, B, C$ are three subsets of $X$ such that $A \supset B \supset C$, and if $B$ is dense in $A$, and $C$ is dense in $B$, then $C$ is dense in $A$ (*transitivity* of density), for we have $\overline{A} = \overline{B} = \overline{C}$ in $X$.

#### Proposition 2 {#top-i-s3-prop-2 .statement}

*Let $A$ be a dense subset of a topological space $X$; then for each $x \in A$ and each neighbourhood $V$ of $x$ relative to $A$, the closure $\overline{V}$ of $V$ in $X$ is a neighbourhood of $x$ in $X$.*

For $V$ contains $U \cap A$, where $U$ is an open subset of $X$ which contains $x$, hence $\overline{V}$ contains $U \cap \overline{A} = U$ (§ 1, no. 6, Proposition 5).

#### Proposition 3 {#top-i-s3-prop-3 .statement}

*Let $(A_i)_{i \in I}$ be a family of subsets of a topological space $X$, such that one of the following properties holds:
a) The interiors of the $A_i$ cover $X$.
b) $(A_i)_{i \in I}$ is a locally finite closed covering of $X$ (§ 1, no. 5).*

*Under these conditions, a subset $B$ of $X$ is open (resp. closed) in $X$ if and only if each of the sets $B \cap A_i$ is open (resp. closed) in $A_i$.*

Clearly if $B$ is open (resp. closed) in $X$, then $B \cap A_i$ is open (resp. closed) in $A_i$. Conversely, suppose first that condition a) is satisfied; since $(\complement B) \cap A_i = A_i - (B \cap A_i)$, it is enough, by duality, to consider the case in which each of the $B \cap A_i$ is *open* with respect to $A_i$. In this case $B \cap \dot{A}_i$ is open in $\dot{A}_i$ for each $i \in I$, and therefore open in $X$; and since $B = \bigcup_i (B \cap \dot{A}_i)$ by hypothesis, it follows that $B$ is open in $X$.

Now suppose that b) is satisfied; by duality again, we need only consider the case in which each of the $B \cap A_i$ is *closed* in $A_i$, and therefore closed in $X$. Since the family $(B \cap A_i)$ is locally finite and $B = \bigcup_i (B \cap A_i)$, it follows from § 1, no. 5, Proposition 4 that $B$ is closed in $X$.

#### Remark {#top-i-s3-n1-rem-1 .statement}

Let $(U_i)_{i \in I}$ be an *open* covering of a topological space $X$, and for each $i \in I$ let $\mathcal{B}_i$ be a *base* of the topology of the subspace $U_i$ of $X$; then it is clear that $\mathcal{B} = \bigcup_{i \in I} \mathcal{B}_i$ is a *base* of the topology of $X$.

### 2. CONTINUITY WITH RESPECT TO A SUBSPACE

Let $X$ and $Y$ be two topological spaces, $f$ a mapping of $X$ into $Y$, $B$ a subset of $Y$ which contains $f(X)$. The definition of the induced topology as an initial topology (§ 2, no. 3, Proposition 4) shows that $f$ is continuous at $x \in X$ if and only if the mapping of $X$ into the *subspace* $B$ of $Y$, having the same graph as $f$, is continuous at $x$.

Now let $A$ be a subset of $X$; if $f$ is continuous at $x \in A$ (resp. continuous on $X$), its restriction $f|A$ is a mapping of the subspace $A$ into $Y$, which is continuous at $x$ (resp. continuous on $A$) by Proposition 2 of § 2, no. 1. We shall sometimes say that a mapping $f : X \to Y$ is *continuous relative to $A$ at $x \in A$* (resp. *continuous relative to $A$*) if its restriction $f|A$ is continuous at $x$ (resp. continuous on $A$).

It should be noted that $f|A$ can be continuous without $f$ being continuous at any point of $X$; an example of this phenomenon is provided by the characteristic function $\varphi_A$ of a subset $A$ of $X$ which is such that both $A$ and its complement are dense in $X$ ($§ 2$, Exercise 11), $\varphi_A$ being regarded as a mapping of $X$ into the discrete space $\{0, 1\}$. $\varphi_A$ is not continuous at any point of $X$, but its restriction to $A$ is constant and therefore continuous.

If $A$ is a neighbourhood in $X$ of a point $x \in A$, and if $f : X \to Y$ is such that $f|A$ is continuous at $x$, then $f$ is continuous at $x$; for each neighbourhood of $x$ in $A$ is a neighbourhood of $x$ in $X$ (*local* character of continuity).

#### Proposition 4 {#top-i-s3-prop-4 .statement}

*Let* $(A_i)_{i \in I}$ *be a family of subsets of a topological space* $X$ *whose interiors cover* $X$, *or which is a locally finite closed covering of* $X$. *Let* $f$ *be a mapping of* $X$ *into a topological space* $X'$. *If the restriction of* $f$ *to each of the subspaces* $A_i$ *is continuous, then* $f$ *is continuous.*

For if $F'$ is a closed subset of $X'$ and if $F = \overline{f}(F')$, then $F \cap A_i$ is closed in $A_i$ for each $i \in I$ ($§ 2$, no. 1, Theorem 1) and therefore $F$ is closed in $X$ by Proposition 3 of no. 1; the result now follows from Theorem 1 of $§ 2$, no. 1.

### 3. LOCALLY CLOSED SUBSPACES

#### Definition 2 {#top-i-s3-def-2 .statement}

*A subset* $L$ *of a topological space* $X$ *is said to be locally closed at a point* $x \in L$ *if there is a neighbourhood* $V$ *of* $x$ *in* $X$ *such that* $L \cap V$ *is a closed subset of the subspace* $V$. *L is said to be locally closed in* $X$ *if it is locally closed at each* $x \in L$.

#### Remark {#top-i-s3-n3-rem-1 .statement}

Let $F$ be a subset of $X$ such that *for each point* $x$ *of* $X$ *there is a neighbourhood* $V$ *of* $x$ *such that* $V \cap F$ *is closed in the subspace* $V$; *then it follows from Proposition 3 of no. 1 that* $F$ *is closed in* $X$. *On the other hand, Proposition 5 below shows that in general there are locally closed sets which are not closed in* $X$.

#### Proposition 5 {#top-i-s3-prop-5 .statement}

*For a subset* $L$ *of a topological space* $X$, *the following properties are equivalent*:

a) $L$ *is locally closed in* $X$.

b) $L$ is the intersection of an open subset and a closed subset of $X$.

c) $L$ is open in its closure $\overline{L}$ in $X$.

If $L$ is locally closed, then, for each $x \in L$, there is an open neighbourhood $V_x$ of $x$ in $X$ such that $L \cap V_x$ is closed in $V_x$; $U = \bigcup_{x \in L} V_x$ is open in $X$, and Proposition 3 of no. 1 shows that $L$ is closed in $U$; therefore a) implies b). If $L = U \cap F$, where $U$ is open and $F$ closed in $X$, we have $L \subset F$; hence $L \subset U \cap L \subset U \cap F = L$, which shows that $L = U \cap L$ is open in $L$, so that b) implies c). Finally, if $L = U \cap L$, where $U$ is open in $X$, $L$ is closed in $U$, hence locally closed, and thus c) implies a).

#### Corollary {#top-i-s3-n3-cor-1 .statement}

*Let $f : X \to X'$ be a continuous map and $L'$ a locally closed subset of $X'$; then $f^{-1}(L')$ is locally closed in $X$*.

This follows immediately from Proposition 5 above and Theorem 1 of § 2, no. 1.

### 4. QUOTIENT SPACES

#### Definition 3 {#top-i-s3-def-3 .statement}

*Let $X$ be a topological space, $R$ an equivalence relation on $X$. The quotient space of $X$ by $R$ is the quotient set $X/R$ with the topology which is the quotient of the topology of $X$ by the relation $R$ (§ 2, no. 4, Example 1)*.

Unless the contrary is expressly stated, whenever we speak of $X/R$ as a topological space, it is to be understood that we mean the quotient space of $X$ by $R$. We shall often say that this topological space is the space obtained by identifying the points of $X$ which belong to the same equivalence class mod $R$.

Let $\varphi$ be the canonical mapping $X \to X/R$. By definition (§ 2, no. 4, Proposition 6 and its corollary) the open (resp. closed) sets in $X/R$ are the sets $A$ such that $\varphi^{-1}(A)$ is open (resp. closed) in $X$; in other words, the open (resp. closed) sets in $X/R$ are in one-to-one correspondence with the open (resp. closed) subsets of $X$ which are saturated with respect to $R$ and are the canonical images of these subsets.

#### Proposition 6 {#top-i-s3-prop-6 .statement}

*Let $X$ be a topological space, $R$ an equivalence relation on $X$, $\varphi$ the canonical mapping of $X$ onto $X/R$; then a mapping $f$ of $X/R$ into a topological space $Y$ is continuous if and only if $f \circ \varphi$ is continuous on $X$*.

This is a particular case of § 2, no. 4, Proposition 6; it expresses the fact that the quotient topology is the final topology for the mapping $\varphi$.

Proposition 6 shows that there is a one-to-one correspondence between the continuous mappings of $X/R$ into $Y$ and the continuous maps of $X$ into $Y$ *which are constant on each equivalence class mod $R$*.

#### Example {#top-i-s3-n4-exa-1 .statement}

*Consider the equivalence relation $x \equiv y \pmod{1}$ on the real line $\mathbf{R}$; the quotient space of $\mathbf{R}$ by this relation is called the *one-dimensional torus* and is denoted by $T$. The equivalence class of a point $x \in \mathbf{R}$ consists of all the points $x + n$, where $n$ runs through the set $\mathbf{Z}$ of rational integers. By Proposition 6 there is a one-to-one correspondence between the continuous functions on $T$ and the continuous functions on $\mathbf{R}$ which are *periodic* with period 1. We shall return to this important example in Chapter V, § 1.*

#### Corollary {#top-i-s3-n4-cor-1 .statement}

*Let $X, Y$ be two topological spaces, $R$ (resp. $S$) an equivalence relation on $X$ (resp. $Y$), and let $f : X \to Y$ be a continuous mapping which is compatible with the equivalence relations $R$ and $S$ (Set Theory R, § 5, no. 8); then the mapping $g : X/R \to Y/S$ induced by $f$ (Set Theory R, § 5, no. 8) is continuous.*

This is a particular case of a general property of quotient structures (Set Theory, Chapter IV, § 2, no. 6, criterion CST 20).

#### Proposition 7 (Transitivity of quotient spaces) {#top-i-s3-prop-7 .statement}

*Let $R$ and $S$ be two equivalence relations on a topological space $X$ such that $R$ implies $S$, and let $S/R$ be the quotient equivalence relation on the quotient space $X/R$ (Set Theory R, § 5, no. 9). Then the canonical bijection $(X/R)/(S/R) \to X/S$ is a homeomorphism.*

This is a particular case of the transitivity of final topologies (§ 2, no. 4, Proposition 7. Cf. Set Theory, Chapter IV, § 2, no. 3, criterion CST 21).

### 5. CANONICAL DECOMPOSITION OF A CONTINUOUS MAPPING

Let $X$ and $Y$ be two topological spaces, $f : X \to Y$ a continuous map, $R$ the equivalence relation $f(x) = f(y)$ on $X$. Consider the *canonical decomposition*

$$
f : X \xrightarrow{\varphi} X/R \xrightarrow{g} f(X) \xrightarrow{\psi} Y
$$

where $\varphi$ is the canonical (surjective) mapping of $X$ onto the quotient space $X/R$, $\psi$ is the canonical injection of the subspace $f(X)$ into $Y$, and $g$ is the bijection associated with $f$ (Set Theory R, § 5, no. 3). It is immediately seen that $g$ is continuous (by Proposition 6 of no. 4); this is also a particular case of a general result on quotient structures. (Cf. Set Theory, Chapter IV, § 2, no. 6). But the bijection $g$ *is not necessarily a homeomorphism*.

#### Proposition 8 {#top-i-s3-prop-8 .statement}

Let $f = \psi \circ g \circ \varphi$ be the canonical decomposition of a continuous mapping $f : X \to Y$, and let $R$ denote the equivalence relation
$$
f(x) = f(y).
$$
Then the following three conditions are equivalent:
a) $g$ is a homeomorphism of $X/R$ onto $f(X)$.
b) The image under $f$ of every open set which is saturated with respect to $R$ is an open set in the subspace $f(X)$.
c) The image under $f$ of every closed set which is saturated with respect to $R$ is a closed set in the subspace $f(X)$.

For the condition b) [resp. c)] expresses that the image under $g$ of every open (resp. closed) set in $X/R$ is an open (resp. closed) set in $f(X)$.

#### Example {#top-i-s3-n5-exa-1 .statement}

Let $X$ be a topological space, $(X_i)_{i \in I}$ a covering of $X$, $Y$ the sum of the subspaces $X_i$ of $X$; then there is a partition $(Y_i)_{i \in I}$ of $Y$ into subspaces which are both open and closed, and for each $i \in I$ there is a homeomorphism $f_i : Y_i \to X_i$. Let $f : Y \to X$ be the continuous mapping which agrees with $f_i$ on $Y_i$ for each $i \in I$, and let $R$ be the equivalence relation $f(x) = f(y)$; the quotient space $Y/R$ is thus obtained by "pasting together" the $Y_i$ (§ 2, no. 5). Consider the bijection $g : Y/R \to X$ associated with $f$; in general $g$ is not a homeomorphism, as is shown by the example in which each $X_i$ consists of a single point and $X$ is not discrete. However, if the interiors of the $X_i$ cover $X$, or if $(X_i)$ is a locally finite closed covering of $X$, then $g$ is a homeomorphism: for if $U$ is any open subset of $Y$ which is saturated with respect to $R$, then for each $i \in I$ the set
$$
f(U) \cap X_i = f_i(U \cap Y_i)
$$
is open in $X_i$, and the assertion follows from Proposition 3 of no. 1.

The following proposition gives a simple sufficient condition for $g$ to be a homeomorphism:

#### Proposition 9 {#top-i-s3-prop-9 .statement}

Let $f : X \to Y$ be a continuous surjection, and let $R$ denote the equivalence relation $f(x) = f(y)$. If there is a continuous section $s : Y \to X$ associated with $f$ (Set Theory, Chapter II, § 3, no. 8, Definition 11), then the mapping $g : X/R \to Y$ associated with $f$ is a homeomorphism, and $s$ is a homeomorphism of $Y$ onto the subspace $s(Y)$ of $X$.

For if $\varphi : X \to X/R$ is the canonical mapping, then $g$ and $\varphi \circ s$ are bijective, continuous and inverse to each other; likewise $s$ and the restriction of $f$ to $s(Y)$ are bijective, continuous and inverse to each other.

If $R$ is an equivalence relation on a topological space $X$ and
$$
\varphi : X \to X/R
$$
is the canonical mapping, a *continuous section* $s : X/R \to X$ associated with $\varphi$ is also called a *continuous section* of $X$ with respect to $R$ (cf. *Set Theory*, Chapter II, § 6, no. 2); the subspace $s(X/R)$ of $X$ is then homeomorphic to $X/R$. If we are given $s(X/R)$, then $s$ is uniquely determined; $s(X/R)$ is often called, by abuse of language, a (continuous) *section* of $X$ with respect to $R$.

A continuous section of a topological space with respect to an equivalence relation need not exist (Exercise 12).

### 6. QUOTIENT SPACE OF A SUBSPACE

Let $X$ be a topological space, $A$ a subspace of $X$, $R$ an equivalence relation on $X$, $f$ the canonical map $X \to X/R$, $g$ the restriction of $f$ to $A$. The equivalence relation $g(x) = g(y)$ on $A$ is just the relation $R_A$ *induced* by $R$ on $A$ (*Set Theory* R, § 5, no. 5). Let $g = \psi \circ h \circ \varphi$ be the canonical decomposition of $g$, so that if $j$ is the canonical injection of $A$ into $X$ we have a commutative diagram (*)

$$
\begin{array}{ccc}
A & \xrightarrow{\varphi} & A/R_A \xrightarrow{h} f(A) \xrightarrow{\psi} X/R. \\
& & \\
& \searrow_j & \nearrow_s \\
& & X
\end{array}
$$

#### Proposition 10 {#top-i-s3-prop-10 .statement}

*The canonical bijection* $h : A/R_A \to f(A)$ *is continuous*. *Furthermore, the following three statements are equivalent*:

a) $h$ *is a homeomorphism*.

b) *Every open subset of* $A$ *which is saturated with respect to* $R_A$ *is the intersection with* $A$ *of an open subset of* $X$ *which is saturated with respect to* $R$.

c) *Every closed subset of* $A$ *which is saturated with respect to* $R_A$ *is the intersection with* $A$ *of a closed subset of* $X$ *which is saturated with respect to* $R$.

The first part of the proposition is immediate (no. 5). The second part follows from Proposition 8 of no. 5: if $B$ is an open (resp. closed) subset of $A$ which is saturated with respect to $R_A$, and $g(B) = f(B)$ is the intersection with $f(A)$ of an open (resp. closed) subset $C$ of $X/R$, then $B$ is the intersection with $A$ of the open (resp. closed) subset $f^{-1}(C)$

(*) This expression means that $f \circ j = \psi \circ h \circ \varphi$.

of X, which is saturated with respect to R; and conversely, if B is the intersection with A of an open (resp. closed) subset D which is saturated with respect to R, then $f(B)$ is the intersection of $f(A)$ and $f(D)$, which is open (resp. closed) in $X/R$.

#### Corollary 1 {#top-i-s3-prop-10-cor-1 .statement}

*If A is an open (resp. closed) subset of X which is saturated with respect to R, then the canonical mapping $h : A/R_A \to f(A)$ is a homeomorphism.*

For if A is open (resp. closed) in X and saturated with respect to R, and if $B \subset A$ is open (resp. closed) in A and saturated with respect to $R_A$, then B is open (resp. closed) in X and saturated with respect to R.

#### Corollary 2 {#top-i-s3-prop-10-cor-2 .statement}

*If there is a continuous mapping $u : X \to A$ such that $u(x)$ is congruent to $x$ mod R for each $x \in X$, then $f(A) = X/R$ and the canonical mapping $h : A/R_A \to X/R$ is a homeomorphism.*

Since each equivalence class mod R meets A, the canonical image of $A/R_A$ in $X/R$ is the whole of $X/R$; on the other hand, if U is open in A and is saturated with respect to $R_A$, it follows from the hypothesis that $\bar{u}^1(U)$ is the set obtained by saturating U with respect to R; since $u$ is continuous, $\bar{u}^1(U)$ is open in X (§ 2, no. 1, Theorem 1). The corollary follows from this fact by virtue of Proposition 10.

#### Example {#top-i-s3-n6-exa-1 .statement}

Let R denote the equivalence relation $x \equiv y \pmod{1}$ on the real line $\mathbf{R}$ (no. 4, Example) and let A denote the closed interval $[0, 1]$; A contains at least one point of each equivalence class mod R. The canonical mapping of $A/R_A$ onto the torus T is a homeomorphism; for if F is closed in A (and hence in R), in order to saturate F with respect to the relation R we have to take the union of the closed sets $F + n$ (for all $n \in \mathbf{Z}$), which evidently form a locally finite family, so that their union is closed (§ 1, no. 5, Proposition 4); the assertion follows from this. We remark that $A/R_A$ is obtained by identifying the points 0 and 1 in A. \*

### Exercises {#top-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
