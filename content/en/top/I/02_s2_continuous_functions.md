---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 2
section_title: Continuous functions
lang: en
source: top-i-iv
book_pages: 25-35, 119-122
pdf_pages: 0031-0041, 0125-0128
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS FUNCTIONS
      page: 25
      pdf_page: 31
    - "no": 2
      title: COMPARISON OF TOPOLOGIES
      page: 28
      pdf_page: 34
    - "no": 3
      title: INITIAL TOPOLOGIES
      page: 30
      pdf_page: 36
    - "no": 4
      title: FINAL TOPOLOGIES
      page: 32
      pdf_page: 38
    - "no": 5
      title: PASTING TOGETHER OF TOPOLOGICAL SPACES
      page: 34
      pdf_page: 40
statements: 26
exercises: 10
content_sha256: 16e7ac6daa7f6e8d5016ffb450612e74265560ae6512c3a4b479d5b88d5f0cf7
---

## 2. CONTINUOUS FUNCTIONS

### 1. CONTINUOUS FUNCTIONS

#### Definition 1 {#top-i-s2-def-1 .statement}

A mapping $f$ of a topological space $X$ into a topological space $X'$ is said to be continuous at a point $x_0 \in X$ if, given any neighbourhood $V'$ of $f(x_0)$ in $X'$, there is a neighbourhood $V$ of $x_0$ in $X$ such that the relation $x \in V$ implies $f(x) \in V'$.

Definition 1 may be restated in the following more intuitive form: to say that $f$ is continuous at the point $x_0$ means that $f(x)$ is as near as we please to $f(x_0)$ whenever $x$ is sufficiently near $x_0$.

The relation "for each $x \in V, f(x) \in V'$" is equivalent to $f(V) \subset V'$ or again to $V \subset \overline{f}^{-1}(V')$; in view of the neighbourhood axiom ($V_I$), we see that Definition 1 is equivalent to the following: $f : X \to X'$ is said to be continuous at the point $x_0$ if, for each neighbourhood $V'$ of $f(x_0)$ in $X'$, $\overline{f}^{-1}(V')$ is a neighbourhood of $x_0$ in $X$. Moreover, it is sufficient that $\overline{f}^{-1}(V')$ is a neighbourhood of $x_0$ for each neighbourhood $V'$ belonging to a fundamental system of neighbourhoods of $f(x_0)$ in $X'$ ($§ 1$, no. 3).

#### Proposition 1 {#top-i-s2-prop-1 .statement}

Let $f$ be a mapping of a topological space $X$ into a topological space $X'$. If $f$ is continuous at $x$, and if $x$ lies in the closure of a subset $A$ of $X$, then $f(x)$ lies in the closure of $f(A)$.

Let $V'$ be a neighbourhood of $f(x)$ in $X'$. Since $f$ is continuous at $x$, $\overline{f}^{-1}(V')$ is a neighbourhood of $x$ in $X$. Hence $\overline{f}^{-1}(V')$ meets $A$, from which it follows that $V'$ meets $f(A)$, and therefore $f(x)$ is in the closure of $f(A)$.

#### Proposition 2 {#top-i-s2-prop-2 .statement}

Let $X, X', X''$ be three topological spaces; let $f$ be a mapping of $X$ into $X'$, continuous at $x \in X$; let $g$ be a mapping of $X'$ into $X''$, continuous at $f(x)$. Then the composition $h = g \circ f : X \to X''$ is continuous at $x$.

Let $V''$ be a neighbourhood of $h(x) = g(f(x))$ in $X''$. Since $g$ is continuous at $f(x)$ it follows that $\overline{g}^{-1}(V'')$ is a neighbourhood of $f(x)$ in $X'$. But $f$ is continuous at $x$, hence $\overline{f}^{-1}(\overline{g}^{-1}(V'')) = \overline{h}^{-1}(V'')$ is a neighbourhood of $x$ in $X$, and therefore $h$ is continuous at $x$.

#### Definition 2 {#top-i-s2-def-2 .statement}

A mapping of a topological space $X$ into a topological space $X'$ is said to be continuous on $X$ (or just continuous) if it is continuous at each point of $X$.

#### Example 1 {#top-i-s2-n1-exa-1 .statement}

The identity mapping of a topological space $X$ onto itself is continuous.
2) A constant map of a topological space into a topological space is continuous.
3) Every mapping of a discrete space into a topological space is continuous.

#### Theorem 1 {#top-i-s2-thm-1 .statement}

Let $f$ be a mapping of a topological space $X$ into a topological space $X'$. Then the following statements are equivalent:

a) $f$ is continuous in $X$.

b) For every subset $A$ of $X$, $f(\overline{A}) \subset \overline{f(A)}$.

c) The inverse image under $f$ of every closed subset of $X'$ is a closed subset of $X$.

d) The inverse image under $f$ of every open subset of $X'$ is an open subset of $X$.

We have already seen that a) implies b) (Proposition 1). To show that b) implies c), let $F'$ be a closed subset of $X'$ and let $F = \overline{f^{-1}(F')}$; then by hypothesis $f(\overline{F}) \subset \overline{f(F)} \subset \overline{F'} = F'$, hence $\overline{F} \subset \overline{f^{-1}(F')} = F \subset \overline{F}$, so that $F = \overline{F}$ and $F$ is closed. By virtue of the relation $\overline{f^{-1}(A')} = \overline{f^{-1}(CA')}$ for every subset $A'$ of $X'$, c) implies d). Finally, suppose that d) is satisfied. Let $x$ be any point of $X$ and let $V'$ be any neighbourhood of $f(x)$ in $X'$; then there is an open set $A'$ in $X'$ for which

$$
f(x) \in A' \subset V'
$$

and hence $x \in \overline{f^{-1}(A')} \subset \overline{f^{-1}(V')}$. By hypothesis, $\overline{f^{-1}(A')}$ is open in $X$, so that $\overline{f^{-1}(V')}$ is a neighbourhood of $x$ in $X$. Thus d) implies a).

Remarks. 1) Let $\mathcal{B}$ be a base (§ 1, no. 3) of the topology of $X'$; then for $f : X \to X'$ to be continuous, it is necessary and sufficient that $\overline{f^{-1}(U')}$ is open in $X$ for every $U' \in \mathcal{B}$.

#### Example {#top-i-s2-n1-exa-2 .statement}

Let $a$ be any rational number. The mapping $x \to a + x$ of the rational line $\mathbf{Q}$ into itself is continuous on $\mathbf{Q}$, for the inverse image under this mapping of an open interval $]b, c[$ is the open interval

$$
]b - a, c - a[.
$$

Likewise, the mapping $x \to ax$ is continuous on $\mathbf{Q}$; this is clear if $a = 0$, for then $ax = 0$ for all $x$; if $a \neq 0$ then the inverse image under this mapping of the open interval $]b, c[$ is the open interval with end-points $b/a$ and $c/a$.

2) The direct image of an open (resp. closed) set of $X$ under a continuous mapping $f : X \to X'$ is not necessarily open (resp. closed) in $X'$ (cf. § 5).

#### Example {#top-i-s2-n1-exa-3 .statement}

\* The mapping $f : x \to 1/(1 + x^2)$ of $\mathbf{R}$ into itself is continuous, but $f(\mathbf{R})$ is the half-open interval $]0, 1]$, which is neither open nor closed in $\mathbf{R}$. \*

#### Theorem 2 {#top-i-s2-thm-2 .statement}

1) If $f : X \to X'$ and $g : X' \to X''$ are two continuous mappings, then $g \circ f : X \to X''$ is continuous.

2) For a bijection $f$ of a topological space $X$ onto a topological space $X'$ to be a homeomorphism, it is necessary and sufficient that $f$ and the inverse of $f$ are continuous (or, as is also said, that $f$ is bicontinuous).

The first assertion is an immediate consequence of Proposition 2; the second follows from Theorem 1, d) and the definition of a homeomorphism (§ 1, no. 1).

#### Remark 1 {#top-i-s2-n1-rem-1 .statement}

It is possible to have a continuous bijection of a topological space $X$ onto a topological space $X'$ which is not bicontinuous: for example, take $X'$ to be the rational line $\mathbf{Q}$, and $X$ to be the set $\mathbf{Q}$ with the discrete topology; then the identity map $X \to X'$ is continuous but is not a homeomorphism.

#### Remark 2 {#top-i-s2-n1-rem-2 .statement}

To verify that a continuous bijection $f : X \to X'$ is a homeomorphism, it is enough to show that for each $x \in X$ and each neighbourhood $V$ of $x$, $f(V)$ is a neighbourhood of $f(x)$ in $X'$.

#### Remark 3 {#top-i-s2-n1-rem-3 .statement}

Let $X$ be a topological space, and for each $x \in X$ let $\mathcal{B}(x)$ be the set of all neighbourhoods of $x$. Let $x_0$ be a point of $X$; for each $x \in X$, define a set $\mathcal{B}_0(x)$ of subsets of $X$ as follows: $\mathcal{B}_0(x_0) = \mathcal{B}(x_0)$, and if $x \neq x_0$ then $\mathcal{B}_0(x)$ is to be the set of all subsets of $X$ which contain $x$. It is immediately verified (§ 1, no. 2, Proposition 2) that the sets $\mathcal{B}_0(x)$ are sets of neighbourhoods of points of $X$ for a topology on $X$; let $X_0$ denote the topological space thus obtained, and let $j : X_0 \to X$ denote the identity map, which is continuous but not in general bicontinuous. A mapping $f$ of $X$ into a topological space $X'$ is continuous at the point $x_0$ if and only if the composition $X_0 \xrightarrow{j} X \xrightarrow{f} X'$ is continuous on $X_0$; this follows immediately from the definitions.

### 2. COMPARISON OF TOPOLOGIES

Theorem 2 of no. 1 shows that we may take the continuous mappings as morphisms of topological structures (Set Theory, Chapter IV, § 2, no. 1); from now on, we shall assume that we have made this choice of morphisms. In accordance with the general definitions (Set Theory, Chapter IV, § 2, no. 2), this allows us to define an ordering on the set of topologies on a given set $X$:

#### Definition 3 {#top-i-s2-def-3 .statement}

Given two topologies $\mathcal{T}_1, \mathcal{T}_2$ on the same set $X$, we say that $\mathcal{T}_1$ is finer than $\mathcal{T}_2$ (and that $\mathcal{T}_2$ is coarser than $\mathcal{T}_1$) if, denoting by $X_i$ the set $X$ with the topology $\mathcal{T}_i$ ($i = 1, 2$), the identity mapping $X_1 \to X_2$ is continuous. If in addition $\mathcal{T}_1 \neq \mathcal{T}_2$, we say that $\mathcal{T}_1$ is strictly finer than $\mathcal{T}_2$ (and that $\mathcal{T}_2$ is strictly coarser than $\mathcal{T}_1$).

Two topologies, one of which is finer than the other, are said to be comparable.

The criteria for a mapping to be continuous (no. 1, Definition 1 and Theorem 1) give the following proposition:

#### Proposition 3 {#top-i-s2-prop-3 .statement}

Given two topologies $\mathcal{T}_1, \mathcal{T}_2$ on a set $X$, the following statements are equivalent:
a) $\mathcal{T}_1$ is finer than $\mathcal{T}_2$.
b) For each $x \in X$, each neighbourhood of $x$ for $\mathcal{T}_2$ is a neighbourhood of $x$ for $\mathcal{T}_1$.
c) For each subset $A$ of $X$, the closure of $A$ in the topology $\mathcal{T}_1$ is contained in the closure of $A$ in the topology $\mathcal{T}_2$.
d) Every subset of $X$ which is closed in $\mathcal{T}_2$ is closed in $\mathcal{T}_1$.
e) Every subset of $X$ which is open in $\mathcal{T}_2$ is open in $\mathcal{T}_1$.

#### Example {#top-i-s2-n2-exa-1 .statement}

\* In Hilbert space $H$ consisting of sequences $x = (x_n)$ of real numbers such that
$$
\|x\|^2 = \sum_{n=0}^\infty x_n^2 < +\infty,
$$
the neighbourhoods of a point $x_0$ in the strong topology on $H$ are the sets which contain an open ball $\|x - x_0\| < \alpha$ centred at $x_0$; the neighbourhoods of $x_0$ in the weak topology on $H$ are the sets containing a set defined by a relation of the form $\sup_{1 \leq i \leq n} |(x - x_0|a_i)| \leq 1$, where the $a_i$ are points of $H$ and
$$
(x|y) = \sum_{n=0}^\infty x_n y_n
$$
if $x = (x_n)$ and $y = (y_n)$. Now if $\beta = \sup_{1 \leq i \leq n} \|a_i\|$, the relation $\|x - x_0\| \leq 1 / \beta$ implies that $|(x - x_0|a_i)| \leq \|x - x_0\| \cdot \|a_i\| \leq 1$ for $1 \leq i \leq n$; hence the strong topology on $H$ is finer than the weak topology. On the other hand, given any finite family $(a_i)_{1 \leq i \leq n}$ of points of $H$, there are points $x$ in $H$ such that $(x - x_0|a_i) = 0$ for $1 \leq i \leq n$ and such that $\|x - x_0\|$ is arbitrarily large; this shows that the strong topology is strictly finer than the weak topology. \*

#### Remark 1 {#top-i-s2-n2-rem-1 .statement}

In the ordered set of all topologies on a set $X$, the topology in which the only open sets are $\varnothing$ and $X$ is the coarsest and the discrete topology is the finest.
2) The finer the topology, the more open sets, closed sets and neighbourhoods; the finer the topology, the smaller (resp. the larger) the closure (resp. the interior) of a set; the finer the topology, the fewer dense sets.
3) If $f : X \to X'$ is a continuous mapping, it remains continuous if the topology of $X$ is replaced by a finer topology and the topology of $X'$ is replaced by a coarser topology (no. 1, Theorem 2). In other words, the finer the topology of $X$ and the coarser the topology of $X'$, the more continuous mappings there are of $X$ into $X'$.

### 3. INITIAL TOPOLOGIES

#### Proposition 4 {#top-i-s2-prop-4 .statement}

Let $X$ be a set, let $(Y_i)_{i \in I}$ be a family of topological spaces, and for each $i \in I$ let $f_i$ be a mapping of $X$ into $Y_i$. Let $\mathcal{S}$ be the set of subsets of $X$ of the form $\overline{f}_i^{-1}(U_i)$ ($i \in I$, $U_i$ open in $Y_i$), and let $\mathcal{B}$ be the set of finite intersections of sets of $\mathcal{S}$. Then $\mathcal{B}$ is a base of a topology $\mathcal{T}$ on $X$ which is the initial topological structure on $X$ for the family $(f_i)$ (Set Theory, Chapter IV, § 2, no. 3) and in particular is the coarsest topology on $X$ for which the mappings $f_i$ are continuous. More precisely, if $g$ is a mapping of a topological space $Z$ into $X$, then $g$ is continuous at a point $z \in Z$ (X carrying the topology $\mathcal{T}$) if and only if each of the functions $f_i \circ g$ is continuous at $z$.

Let $\mathcal{D}$ be the set of all unions of sets belonging to $\mathcal{B}$; clearly $\mathcal{D}$ satisfies axiom $(O_1)$ since formation of unions is associative; and $\mathcal{D}$ satisfies axiom $(O_{II})$ by reason of the definition of $\mathcal{B}$ and the fact that finite intersection is distributive over arbitrary union [Set Theory, R § 4, formula (37)]. The set $\mathcal{D}$ is therefore the set of open subsets of $X$ for a topology $\mathcal{T}$ of which $\mathcal{B}$ is a base. We shall prove the last assertion of the proposition, which implies the others by reason of the general properties of initial structures (Set Theory, Chapter IV, § 2, no. 3, criterion CST 9). In the first place, the definition of $\mathcal{S}$ shows that the $f_i$ are continuous on $X$ (no. 1, Theorem 1); hence, if $g$ is continuous at $z$, so are the mappings $f_i \circ g$ (no. 1, Proposition 2). Conversely, suppose that all the mappings $f_i \circ g$ are continuous at $z$, and let $V$ be a neighbourhood of $g(z)$ in $X$; by definition, there is a finite subset $J$ of $I$, and for each $i \in J$ an open subset $U_i$ of $Y_i$ such that $V$ contains the set $\bigcap_{i \in J} \overline{f}_i^{-1}(U_i)$ and $g(z)$ belongs to this set. It follows that
$$
\overline{g}^{-1}(V) \supset \bigcap_{i \in J} \overline{g}^{-1}(\overline{f}_i^{-1}(U_i)),
$$
and the hypothesis implies that each of the sets $\overline{g}^{-1}(\overline{f}_i^{-1}(U_i))$ is a neighbourhood of $z$ in $Z$; hence $\overline{g}^{-1}(V)$ is also a neighbourhood of $z$ in $Z$. This completes the proof.

Let $\mathcal{B}_i$ be a base of the topology of $Y_i (i \in I)$; let $\mathcal{S}'$ denote the set of subsets of $X$ of the form $\overline{f}_i^{-1}(U_i)$ for $i \in I$ and $U_i \in \mathcal{B}_i$ for each $i \in I$; if $\mathcal{B}'$ is the set of finite intersections of sets of $\mathcal{S}'$, it is evident that $\mathcal{B}'$ is a base of the topology $\mathcal{T}$.

The general properties of initial structures (Set Theory, Chapter IV, § 2, no. 3, criterion CST 10) imply in particular the following transitivity property (the direct proof of which is quite straightforward):

#### Proposition 5 {#top-i-s2-prop-5 .statement}

Let $X$ be a set, $(Z_i)_{i \in I}$ a family of topological spaces, $(J_\lambda)_{\lambda \in L}$ a partition of $I$ and $(Y_\lambda)_{\lambda \in L}$ a family of sets indexed by $L$. Also for each $\lambda \in L$ let $h_\lambda$ be a mapping of $X$ into $Y_\lambda$; for each $\lambda \in L$ and each $i \in J_\lambda$ let $g_{i\lambda}$ be a mapping of $Y_\lambda$ into $Z_i$, and put $f_i = g_{i\lambda} \circ h_\lambda$. If each $Y_\lambda$ carries the coarsest topology for which the mappings $g_{i\lambda} (i \in J_\lambda)$ are continuous, then the coarsest topology on $X$ for which the $f_i$ are continuous is the same as the coarsest topology for which the $h_\lambda$ are continuous.

#### Example 1 {#top-i-s2-n3-exa-1 .statement}

Inverse image of a topology. Let $X$ be a set, $Y$ a topological space, $f$ a mapping of $X$ into $Y$; the coarsest topology $\mathcal{T}$ on $X$ for which $f$ is continuous is called the inverse image under $f$ of the topology of $Y$. It follows from Proposition 4 and the formulae for the inverse image of a union and an intersection [Set Theory, R, § 4, formulae (34) and (46)] that the open (resp. closed) sets in the topology $\mathcal{T}$ are the inverse images under $f$ of the open (resp. closed) sets of $Y$; consequently, for each $x \in X$, the sets $f^{-1}(W)$, where $W$ runs through a fundamental system of neighbourhoods of $f(x)$ in $Y$, form a fundamental system of neighbourhoods of $x$ in the topology $\mathcal{T}$. In § 3 we shall study, under the name of induced topology, the particular case in which $X$ is a subset of $Y$ and $f$ is the canonical injection $X \to Y$; $X$, with the induced topology, is then called a subspace of $Y$.

For a mapping $f$ of a topological space $X$ into a topological space $X'$ to be continuous it is necessary and sufficient that the topology of $X$ is finer than the inverse image under $f$ of the topology of $X'$.

#### Example 2 {#top-i-s2-n3-exa-2 .statement}

Least upper bound of a set of topologies. Every family $(\mathcal{T}_i)_{i \in I}$ of topologies on a set $X$ has a least upper bound $\mathcal{T}$ in the ordered set of all topologies on $X$, i.e. there exists a topology on $X$ which is coarsest among all the topologies on $X$ which are finer than each of the $\mathcal{T}_i$. To see this we may apply Proposition 4, taking $Y_i$ to be the set $X$ with the topology $\mathcal{T}_i$, and $f_i$ to be the identity map $X \to Y_i$; $\mathcal{T}$ is the coarsest topology for which all the mappings $f_i$ are continuous.

Let $\mathfrak{S}$ be an arbitrary set of subsets of a set $X$; amongst the topologies $\mathcal{T}$ on $X$ for which the sets of $\mathfrak{S}$ are open, there is a topology $\mathcal{T}_0$ which is coarser than all the others and which is called the topology generated by $\mathfrak{S}$. For each set $U \in \mathfrak{S}$ let $\mathcal{T}_U$ be the topology whose open sets are $\varnothing, U$ and $X$ [it is clear that this set of subsets of $X$ satisfies (O_I) and (O_{II})]; then $\mathcal{T}_0$ is just the least upper bound of the topologies $\mathcal{T}_U$. By Proposition 4, if $\mathfrak{B}$ is the set of finite intersections of sets belonging to $\mathfrak{S}$, then $\mathfrak{B}$ is a base of the topology $\mathcal{T}_0$. We say that $\mathfrak{S}$ is a subbase of $\mathcal{T}_0$.

#### Example 3 {#top-i-s2-n3-exa-3 .statement}

Product topology. Let $(X_i)_{i \in I}$ be a family of topological spaces. The coarsest topology on the product set $X = \prod_{i \in I} X_i$ for which the projec-

### 4. FINAL TOPOLOGIES

#### Proposition 6 {#top-i-s2-prop-6 .statement}

*Let $X$ be a set, let $(Y_i)_{i \in I}$ be a family of topological spaces, and for each $i \in I$ let $f_i$ be a mapping of $Y_i$ into $X$. Let $\mathcal{D}$ be the set of subsets $U$ of $X$ such that $\overline{f}_i^{-1}(U)$ is open in $Y_i$ for each $i \in I$; then $\mathcal{D}$ is the set of open subsets of $X$ in a topology $\mathcal{T}$ on $X$ which is the final structure on $X$ for the family $(f_i)$ (Set Theory, Chapter IV, § 2, no. 5), and in particular $\mathcal{T}$ is the finest topology on $X$ for which the mappings $f_i$ are continuous. In other words, if $g$ is a mapping of $X$ into a topological space $Z$, then $g$ is continuous ($X$ carrying the topology $\mathcal{T}$) if and only if each of the mappings $g \circ f_i$ is continuous.*

It is immediately verified that $\mathcal{D}$ satisfies the axioms $(O_I)$ and $(O_{II})$. [Set Theory, R, § 4, formulae (34) and (46)]. We shall prove the last assertion of the proposition, which implies the other assertions by reason of the general properties of final structures (Set Theory, Chapter IV, § 2, no. 5, criterion CST 18). It is clear that the $f_i$ are continuous in the topology $\mathcal{T}$, by the definition of $\mathcal{D}$ (no. 1, Theorem 1); hence if $g$ is continuous, so is each mapping $g \circ f_i$ (no. 1, Theorem 2). Conversely, suppose that each $g \circ f_i$ is continuous, and let $V$ be an open set in $Z$; by hypothesis, $\overline{f}_i^{-1}(\overline{g}^{-1}(V))$ is open in $Y_i$ for each $i \in I$; hence $\overline{g}^{-1}(V) \in \mathcal{D}$, and the proof is complete.

#### Corollary {#top-i-s2-n4-cor-1 .statement}

*Under the hypotheses of Proposition 6, a subset $F$ of $X$ is closed in the topology $\mathcal{T}$ if and only if $\overline{f}_i^{-1}(F)$ is closed in $Y_i$ for each $i \in I$.*

This follows from the definition of the open sets in the topology $\mathcal{T}$ by taking complements.

The general properties of final structures (Set Theory, Chapter IV, § 2, no. 5, criterion CST 19) imply the following *transitivity* property (the direct proof of which is also straightforward):

#### Proposition 7 {#top-i-s2-prop-7 .statement}

*Let $X$ be a set, $(Z_i)_{i \in I}$ a family of topological spaces, $(J_\lambda)_{\lambda \in L}$ a partition of $I$, and $(Y_\lambda)_{\lambda \in L}$ a family of sets indexed by $L$. Also, for each $\lambda \in L$ let $h_\lambda$ be a mapping of $Y_\lambda$ into $X$; for each $\lambda \in L$ and each $i \in J_\lambda$ let $g_{\lambda i}$ be a mapping of $Z_i$ into $Y_\lambda$, and put $f_i = h_\lambda \circ g_{\lambda i}$. If each $Y_\lambda$ carries the finest topology for which the mappings $g_{\lambda i} (i \in J_\lambda)$ are continuous, then the finest topology on $X$ for which the $f_i$ are continuous is the same as the finest topology for which the $h_\lambda$ are continuous.*

Examples

1) Quotient topology. Let $X$ be a topological space, $R$ an equivalence relation on $X$, $Y = X/R$ the quotient set of $X$ with respect to the relation $R$, $\varphi : X \to Y$ the canonical mapping. The finest topology on $Y$ for which $\varphi$ is continuous is called the quotient of the topology of $X$ by the relation $R$; we shall study it in more detail in § 3.

2) Greatest lower bound of a set of topologies. Every family $(\mathcal{T}_i)_{i \in I}$ of topologies on a set $X$ has a greatest lower bound $\mathcal{T}$ in the set of all topologies on $X$, i.e. $\mathcal{T}$ is the finest of all the topologies on $X$ which are coarser than each of the $\mathcal{T}_i$. To see this we may apply Proposition 6, taking $Y_i$ to be the set $X$ with the topology $\mathcal{T}_i$, and $f_i$ to be the identity mapping $Y_i \to X$. If $\mathcal{D}_i$ is the set of subsets of $X$ which are open in the topology $\mathcal{T}_i$, then the set $\bigcap_{i \in I} \mathcal{D}_i$ is the set of subsets of $X$ which are open in $\mathcal{T}$. $\mathcal{T}$ is also called the intersection of the topologies $\mathcal{T}_i$.

3) Sum of topological spaces. Let $(X_i)_{i \in I}$ be a family of topological spaces, $X$ the set which is the sum of the $X_i$ (Set Theory, Chapter II, § 4, no. 8, Definition 8); for each $i \in I$, let $j_i$ be the canonical (injective) mapping of $X_i$ into $X$. The finest topology $\mathcal{T}$ on $X$ for which the mappings $j_i$ are continuous is called the sum of the topologies of the $X_i$, and $X$ with this topology is said to be the sum of the topological spaces $X_i$. Let us identify each of the $X_i$ with a subset of $X$ by means of $j_i$; then a set $A \subset X$ is open (resp. closed) in the topology $\mathcal{T}$ if and only if each of the sets $A \cap X_i$ is open (resp. closed) in $X_i$. In particular, each of the $X_i$ is both open and closed.

The following proposition generalizes the situation of Example 3:

#### Proposition 8 {#top-i-s2-prop-8 .statement}

Let $X$ be a set, $(X_\lambda)_{\lambda \in L}$ a family of subsets of $X$. Suppose each $X_\lambda$ carries a topology $\mathcal{T}_\lambda$ such that, for each pair of indices $(\lambda, \mu)$:
1) $X_\lambda \cap X_\mu$ is open (resp. closed) in each of the topologies $\mathcal{T}_\lambda, \mathcal{T}_\mu$.
2) The topologies induced on $X_\lambda \cap X_\mu$ by $\mathcal{T}_\lambda$ and $\mathcal{T}_\mu$ coincide. Let $\mathcal{T}$ be the finest topology on $X$ for which the injections $j_\lambda : X_\lambda \to X$ are continuous. Then, for each $\lambda \in L$, $X_\lambda$ is open (resp. closed) in $X$ in the topology $\mathcal{T}$, and the topology induced by $\mathcal{T}$ on $X_\lambda$ coincides with $\mathcal{T}_\lambda$.

In view of Proposition 6 and its corollary, it is enough to show that for each $\lambda$ and each subset $A_\lambda$ of $X_\lambda$ the following statements are equivalent:
(i) $A_\lambda$ is open (resp. closed) in the topology $\mathcal{T}_\lambda$.
(ii) For each $\mu \in L$, $A_\lambda \cap X_\mu$ is open (resp. closed) in the topology $\mathcal{T}_\mu$.

It is clear that (ii) implies (i) by taking $\mu = \lambda$. Conversely, if (i) is satisfied, then $A_\lambda \cap X_\mu$ is open (resp. closed) in $X_\lambda \cap X_\mu$ for the topology $\mathcal{T}_{\lambda \mu}$ induced on $X_{\lambda} \cap X_{\mu}$ by $\mathcal{T}_{\lambda}$; but $\mathcal{T}_{\lambda \mu}$ is also the topology induced on $X_{\lambda} \cap X_{\mu}$ by $\mathcal{T}_{\mu}$; hence $A_{\lambda} \cap X_{\mu}$ is also the intersection of $X_{\lambda} \cap X_{\mu}$ with a subset $B_{\mu}$ of $X_{\mu}$ which is open (resp. closed) in the topology $\mathcal{T}_{\mu}$; since $X_{\lambda} \cap X_{\mu}$ is open (resp. closed) in $\mathcal{T}_{\mu}$, so is $A_{\lambda} \cap X_{\mu}$. This completes the proof.

We remark that if the union of the $X_{\lambda}$ is different from $X$, then the topology induced by $\mathcal{T}$ on $X - \left( \bigcup_{\lambda \in L} X_{\lambda} \right)$ is *discrete*. For if $x \in X$ belongs to none of the $X_{\lambda}$, then $\{ x \} \cap X_{\lambda} = \varnothing$ is open in each topology $\mathcal{T}_{\lambda}$ and therefore $\{ x \}$ is open in the topology $\mathcal{T}$.

### 5. PASTING TOGETHER OF TOPOLOGICAL SPACES

Let $(X_{\lambda})_{\lambda \in L}$ be a family of sets, and let $X$ be the set which is the *sum* of the $X_{\lambda}$ (*Set Theory*, Chapter II, § 4, no. 8, Definition 8); we shall identify each $X_{\lambda}$ with a subset of $X$ by means of the canonical injection $j_{\lambda} : X_{\lambda} \to X$.

Let $R$ be an equivalence relation on $X$ such that *each equivalence class of* $R$ *has at most one element in each* $X_{\lambda}$; for each pair of indices $(\lambda, \mu)$ let $A_{\lambda \mu}$ be the subset of $X_{\lambda}$ consisting of the elements $x$ for which there is an element $y \in X_{\mu}$ which belongs to the equivalence class of $X$. Clearly to each $x \in A_{\lambda \mu}$ corresponds a unique $y \in A_{\mu \lambda}$ which is congruent to $x$ mod $R$; the mappings $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ so defined satisfy the following conditions:

(i) For each $\lambda \in L$, $h_{\lambda \lambda}$ is the identity mapping of $A_{\lambda \lambda} = X_{\lambda}$.

(ii) For each triple of indices $(\lambda, \mu, \nu)$ of $L$ and each $x \in A_{\lambda \mu} \cap A_{\lambda \nu}$, we have $h_{\mu \lambda}(x) \in A_{\mu \nu}$ and

$$
h_{\nu \lambda}(x) = h_{\nu \mu}(h_{\mu \lambda}(x)).
$$

*Conversely*, suppose that for each pair of indices $(\lambda, \mu)$ we are given a subset $A_{\lambda \mu}$ of $X_{\lambda}$ and a mapping $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ satisfying the conditions (i) and (ii) above. It follows first of all from (ii) applied to the triples $(\lambda, \mu, \lambda)$ and $(\mu, \lambda, \mu)$ that $h_{\lambda \mu} \circ h_{\mu \lambda}$ (resp. $h_{\mu \lambda} \circ h_{\lambda \mu}$) is the restriction of $h_{\lambda \lambda}$ (resp. $h_{\mu \mu}$) to $A_{\lambda \mu}$ (resp. $A_{\mu \lambda}$); hence we deduce from (i) that $h_{\lambda \mu}$ and $h_{\mu \lambda}$ are *bijections* which are inverses of each other. Now let $R \{ x, y \}$ be the relation "there exist $\lambda, \mu$ such that $x \in A_{\lambda \mu}$, $y \in A_{\mu \lambda}$ and $y = h_{\mu \lambda}(x)$". It follows from (i) and from what precedes that $R$ is *reflexive* and *symmetric*; on the other hand, if $x \in A_{\lambda \mu}$,

$$
y = h_{\mu \lambda}(x) \in A_{\mu \lambda} \cap A_{\mu \nu} \quad \text{and} \quad z = h_{\nu \mu}(y),
$$

then also $x = h_{\lambda \mu}(y)$ and therefore, by (ii), $x \in A_{\lambda \mu} \cap A_{\lambda \nu}$; the relation (i) thus shows that $R$ is *transitive*, and therefore $R$ is an equivalence relation on $X$. It follows also from (i) and from the definition of $R$ that each equivalence class mod $R$ has at most one element in each of the sets $X_\lambda$, and that $A_{\lambda \mu}$ is the set of all $x \in X_\lambda$ for which there is an element $y \in X_\mu$ congruent to $x$ mod $R$. We say that the quotient set $X/R$ is obtained by *pasting together the* $X_\lambda$ *along the* $A_{\lambda \mu}$ *by means of the bijections* $h_{\mu \lambda}$. If $\varphi : X \to X/R$ is the canonical mapping, the restriction of $\varphi$ to each $X_\lambda$ is a *bijection* of $X_\lambda$ onto $\varphi(X_\lambda)$.

Now suppose that each $X_\lambda$ is a *topological space*, and let $\mathcal{T}_\lambda$ be its topology. Let $\mathcal{T}$ be the finest topology on the set $X/R$ for which the mappings $\varphi \circ j_\lambda$ are continuous; $\mathcal{T}$ is the quotient by $R$ of the topology on $X$ which is the *sum* of the topologies $\mathcal{T}_\lambda$. We say that the topological space $X/R$ (with the topology $\mathcal{T}$) is obtained by *pasting together the topological spaces* $X_\lambda$ *along the* $A_{\lambda \mu}$ *by means of the bijections* $h_{\mu \lambda}$. The *open* (resp. *closed*) subsets of $X/R$ are thus the canonical images of the subsets $B$ of $X$ which are *saturated* with respect to $R$ and are such that $B \cap X_\lambda$ is *open* (resp. *closed*) in $X_\lambda$ for each $\lambda \in L$.

Since the restriction of $\varphi$ to each $X_\lambda$ is a bijection onto the subset $X'_\lambda = \varphi(X_\lambda)$ of $X/R$, we can transport the topology $\mathcal{T}_\lambda$ to $X'_\lambda$ by means of this bijection, so that $X'_\lambda$ carries a topology $\mathcal{T}'_\lambda$; and the topology $\mathcal{T}$ on $X/R$ is the *finest* for which the canonical injections $X'_\lambda \to X/R$ are continuous. In general, the topology induced by $\mathcal{T}$ on $X'_\lambda$ is *coarser* than $\mathcal{T}'_\lambda$, but not identical with the latter; even if the $h_{\mu \lambda}$ are homeomorphisms (§ 3, Exercise 15). However, it follows from no. 4, Proposition 8 that, with the preceding notation:

#### Proposition 9 {#top-i-s2-prop-9 .statement}

*Suppose that the* $h_{\mu \lambda}$ *are homeomorphisms and that each* $A_{\lambda \mu}$ *is open (resp. closed)* *in* $X_\lambda$; *then each* $\varphi(X_\lambda)$ *is open (resp. closed)* *in* $X/R$ *and the restriction of* $\varphi$ *to* $X_\lambda$ *is a homeomorphism of* $X_\lambda$ *onto the subspace* $\varphi(X_\lambda)$ *of* $X/R$.

### Exercises {#top-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
