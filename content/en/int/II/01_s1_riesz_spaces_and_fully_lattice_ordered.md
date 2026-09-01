---
book: int
book_title: Integration
chapter: II
chapter_title: RIESZ SPACES
section: 1
section_title: Riesz spaces and fully lattice-ordered spaces
lang: en
source: int-i-vi
pdf_pages: 0025-0032, 0039-0043
extraction: ocr
subsections:
    - "no": 1
      title: Definition of Riesz spaces
      page: 0
      pdf_page: 25
    - "no": 2
      title: Generation of a Riesz space by its positive elements
      page: 3
      pdf_page: 27
    - "no": 3
      title: Fully lattice-ordered spaces
      page: 4
      pdf_page: 28
    - "no": 4
      title: Subspaces and product spaces of fully lattice-ordered spaces
      page: 5
      pdf_page: 29
    - "no": 5
      title: Bands in a fully lattice-ordered space
      page: 6
      pdf_page: 30
statements: 16
exercises: 12
content_sha256: 32113a7d90414afcb3827cb2317f4b388db9fa35a79b7d1a5cb9dfa7b2c1ccfb
---

## § 1. RIESZ SPACES AND FULLY LATTICE-ORDERED SPACES

### 1. Definition of Riesz spaces

Recall that, on a set E, a vector space structure over the field $\mathbf{R}$ and an order structure are said to be compatible if they satisfy the following two axioms:

(OVS_I) *The relation* $x \leq y$ *implies* $x + z \leq y + z$ *for all* $z \in E$.

(OVS_{II}) *The relation* $x \geq 0$ *implies* $\lambda x \geq 0$ *for every scalar* $\lambda > 0$.

The space E, equipped with these two structures, is called an *ordered vector space* (TVS, II, §2, No. 5).

Axiom (OVS_I) signifies that the order structure and the additive group structure on E are compatible, in other words that E, equipped with these two structures, is an *ordered group* (A, VI, §1, No. 1).

Axiom (OVS_I) implies that the relations $x \leq y$ and $x + z \leq y + z$ are equivalent. Similarly, it follows from (OVS_{II}) that, for every scalar $\lambda > 0$, the relations $x \leq y$ and $\lambda x \leq \lambda y$ are equivalent, because $\lambda^{-1} > 0$ and so the relation $\lambda x \leq \lambda y$ implies $\lambda^{-1}(\lambda x) \leq \lambda^{-1}(\lambda y)$. One can therefore say that, in an ordered vector space, the translations and the homotheties of ratio $> 0$ are automorphisms of the order structure; this fact is also expressed by saying that the order is *invariant* under every translation and every homothety of ratio $> 0$. Moreover, the symmetry $x \mapsto -x$ is an isomorphism of the order structure of E onto the *opposite* order structure.

#### Definition 1 {#int-ii-s1-def-1 .statement}

*An ordered vector space is said to be a Riesz space (or lattice-ordered vector space)*$^1$ *if its order structure is a lattice-ordering* (that is, if every pair of elements $x, y$ of E has a supremum $\sup(x, y)$ and an infimum $\inf(x, y)$ ).$^2$

(1) Also called a "vector lattice".

(2) Borne supérieure (supremum) is also translated as "least upper bound" (S, R, §6, 7). Similarly borne inférieure (infimum) is also translated as "greatest lower bound".

#### Example {#int-ii-s1-n1-exa-1 .statement}

The space $\mathbf{R}^A$ of all real-valued functions defined on any set $A$ is a Riesz space (for the order relation $\langle x(t) \leq y(t) \text{ for all } t \in A \rangle$); for, any two real-valued functions $x, y$ defined on $A$ have a supremum (resp. an infimum) equal to the mapping $t \mapsto \sup(x(t), y(t))$ (resp. $t \mapsto \inf(x(t), y(t))$).

One can also say that a Riesz space is a vector space $E$ equipped with an order structure such that, on the one hand, this structure and the additive group structure of $E$ define a *lattice-ordered group* structure on $E$ (A, VI, §1, No. 9), and on the other hand that the axiom (OVS$_{\mathrm{II}}$) is satisfied.

Thus, all of the properties of lattice-ordered groups are applicable to Riesz spaces; we shall review here the principal ones (cf. A, VI, §1, Nos. 9 to 12), as well as indicating the consequences that flow from the axiom (OVS$_{\mathrm{II}}$).

We recall first that one writes $x^+ = \sup(x, 0)$ (the *positive part* of $x$), $x^- = (-x)^+ = \sup(-x, 0)$ (the *negative part* of $x$), $|x| = \sup(x, -x)$ (the *absolute value* of $x$); then $x = x^+ - x^-$ and $|x| = x^+ + x^-$; here, these two relations are equivalent to

$$
x^+ = \frac{1}{2}(|x| + x), \quad x^- = \frac{1}{2}(|x| - x).
$$

The relation $x \leq y$ is equivalent to $\langle x^+ \leq y^+ \text{ and } x^- \geq y^- \rangle$. For any $x$ and $y$, the *triangle inequality* holds:

(1)
$$
|x + y| \leq |x| + |y|.
$$

By the invariance of order under every homothety of ratio $> 0$,

(2)
$$
\sup(\lambda x, \lambda y) = \lambda \sup(x, y) \quad \text{for all } \lambda \geq 0.
$$

In particular,

(3)
$$
(\lambda x)^+ = \lambda x^+, \quad (\lambda x)^- = \lambda x^- \quad \text{for all } \lambda \geq 0.
$$

On the other hand, for $\lambda < 0$ we have $(\lambda x)^+ = (-\lambda x)^- = |\lambda| x^-$ and $(\lambda x)^- = (-\lambda x)^+ = |\lambda| x^+$; it follows that, for every $\lambda \in \mathbf{R}$ and every $x \in E$,

(4)
$$
|\lambda x| = |\lambda| \cdot |x|.
$$

The invariance of order under translation shows that for all $z \in E$,

(5)
$$
\sup(x + z, y + z) = z + \sup(x, y),
$$
whence, in particular,

(6)
$$
\sup(x, y) = x + (y - x)^+ = \frac{1}{2}(x + y + |x - y|).
$$

We have the relations

(7)    $\inf(x, y) = -\sup(-x, -y) ,$

(8)    $\sup(x, y) + \inf(x, y) = x + y .$

If $x, y, z$ are $\geq 0$ then (A, VI, §1, No. 12, Prop. 11)

(9)    $\inf(x + y, z) \leq \inf(x, z) + \inf(y, z) .$

If A and B are two subsets of E each of which has a supremum, then A + B also has a supremum and

(10)    $\sup(A + B) = \sup A + \sup B .$

Two elements $x, y$ of E are said to be alien$^3$ (to each other) if $\inf(|x|, |y|) = 0$; by (8), this relation is equivalent to $\sup(|x|, |y|) = |x| + |y|$, and also, by (6), to $||x| - |y|| = |x| + |y|$; 0 is the only element alien to itself; for every $x \in E$, $x^+$ and $x^-$ are alien and may be characterized as the only alien elements $y \geq 0, z \geq 0$ such that $x = y - z$. If $y$ is alien to $x$, then every $z \in E$ such that $|z| \leq |y|$ is also alien to $x$. If $y$ and $z$ are alien to $x$, then so is $|y| + |z|$, by the inequality (9); in particular, $n|y|$ is alien to $x$ for every integer $n > 0$, from which it follows that $\lambda y$ is alien to $x$ for every scalar $\lambda$, since there exists an integer $n$ such that $|\lambda| \leq n$, whence $|\lambda y| \leq n|y|$. If a subset A of E consists of elements alien to $x$ and if A has a supremum, then that supremum is also alien to $x$ (A, VI, §1, No. 12, Cor. of Prop. 13).

Finally, we have the decomposition lemma (A, VI, §1, No. 10, Th. 1):

*If* $(x_i)_{i \in I}, (y_j)_{j \in J}$ *are two finite sequences of elements* $\geq 0$ *of E such that* $\sum_{i \in I} x_i = \sum_{j \in J} y_j$, *then there exists a finite sequence* $(z_{ij})_{(i,j) \in I \times J}$ *of elements* $\geq 0$ *of E such that* $x_i = \sum_{j \in J} z_{ij}$ *for all* $i \in I$, *and* $y_j = \sum_{i \in I} z_{ij}$ *for all* $j \in J$.

### 2. Generation of a Riesz space by its positive elements

Let E be an ordered vector space; the set P of elements $\geq 0$ of E is a convex cone with vertex 0, that is (TVS, II, §2, No. 4), a set such that

$^3$ The original is étrangers, also translated as "coprime" (A, VI, §1, No. 12); the terms "orthogonal", "disjoint" and "mutually singular" are also used.

P + P ⊂ P and λP ⊂ P for all λ > 0. Conversely, if, in a vector space E over $\mathbf{R}$, P is a convex cone with vertex 0, such that $P \cap (-P) = \{0\}$ (in other words, a *pointed* and *proper* convex cone), one knows (*loc. cit.*) that the relation $y - x \in P$ is an order relation (denoted $x \leq y$) compatible with the vector space structure of E. For this order structure to define a *Riesz space* structure on E, it is necessary and sufficient that:

$1^\circ$ P generates E, that is, every $z \in E$ is of the form $y - x$, where x and y belong to P;

$2^\circ$ P satisfies one of the following two conditions:
a) every pair of elements of P has a supremum in P;
b) every pair of elements of P has an infimum in P (A, VI, §1, No. 9, Prop. 8).

### 3. Fully lattice-ordered spaces

#### Definition 2 {#int-ii-s1-def-2 .statement}

*A Riesz space E is said to be fully lattice-ordered if every nonempty subset of E that is bounded above has a supremum in E.*

It is immediate that in a fully lattice-ordered space E, every nonempty subset that is bounded below has an infimum in E.

#### Example {#int-ii-s1-n3-exa-1 .statement}

— 1) If A is any set, the space $\mathbf{R}^A$ of real-valued functions defined on A is fully lattice-ordered, the supremum in $\mathbf{R}^A$ of a family that is bounded above being its *upper envelope* (GT, IV, §5, No. 5).

2) Let F be any set; the space $\mathcal{B}(F)$ of *bounded* real-valued functions on F, equipped with the order structure induced by that of $\mathbf{R}^F$, is fully lattice-ordered. However, if F is a topological space, the space $\mathcal{C}(F)$ of *continuous* real-valued functions on F (equipped with the order structure induced by that of $\mathbf{R}^F$) is a Riesz space that is not in general fully lattice-ordered (cf. Exer. 13). Consider for example the case that $F = \mathbf{R}$; let I be the interval ]0, 1[, $\varphi_I$ the characteristic function of I, and let H be the set of continuous functions $x(t)$ such that $x \leq \varphi_I$; it is clear that H is bounded above in $\mathcal{C}(F)$. The function $\varphi_I$ is the *upper envelope* of the $x \in H$, but it is not their supremum in $\mathcal{C}(F)$, since $\varphi_I$ is lower semi-continuous but not continuous. Let us show that, in fact, H has no supremum in $\mathcal{C}(F)$; it suffices to prove that if $u$ is a continuous function such that $u \geq \varphi_I$, then there exists a continuous function $v \neq u$ such that $u \geq v \geq \varphi_I$. Now, $u(0) \geq 1$, therefore there exists a number $\alpha > 0$ such that $u(t) > 0$ for $-\alpha \leq t \leq 0$; if w is a continuous function that is zero outside of the interval ]$-\alpha, 0$ and is such that $0 < w(t) < u(t)$ on this interval, then the function $v = u - w$ meets the requirements.

#### Proposition 1 {#int-ii-s1-prop-1 .statement}

*For an ordered vector space E to be fully lattice-ordered, it is necessary and sufficient that E be a Riesz space and that it satisfy one of the following two conditions:*

a) *every nonempty subset A, consisting of elements $\geq 0$ of E, that is bounded above and directed for the relation $\leq$, has a supremum in E;*

b) *every nonempty subset* $A$, *consisting of elements* $\geqslant 0$ *of* $E$ *and directed for the relation* $\geqslant$, *has an infimum in* $E$.

The conditions are obviously necessary. Conversely, suppose that $E$ is a Riesz space satisfying the condition *a)*. Let $B$ be a nonempty subset of $E$ that is bounded above; the set $C$ consisting of the suprema of the finite subsets of $B$ is directed for the relation $\leqslant$; let $a$ be one its elements and $C_a$ the set of $x \in C$ that are $\geqslant a$; if we prove that $C_a$ has a supremum then it will also be the supremum of $B$. Now, $C_a - a$ is a set of elements $\geqslant 0$, bounded above and directed for the relation $\leqslant$; it therefore has a supremum $b$, consequently $a + b$ is the supremum of $C_a$.

On the other hand, the condition *b)* implies *a)*: for, if $F$ is a nonempty set of elements $\geqslant 0$ of $E$, bounded above and directed for $\leqslant$, and if $c$ is an upper bound for $F$, then $c - F$ is a set of elements $\geqslant 0$ that is directed for $\geqslant$; if it has an infimum $m$, then $c - m$ is the supremum of $F$.

#### Proposition 2 {#int-ii-s1-prop-2 .statement}

— *Let* $E$ *be a Riesz space equipped with a Hausdorff topology that is compatible with its ordered vector space structure* (TVS, II, §2, No. 7). *If, for every set* $H \subset E$ *that is bounded above and directed for the relation* $\leqslant$, *the section filter of* $H$ *is convergent, then* $E$ *is fully lattice-ordered*.

Indeed, one knows that the limit of the section filter of $H$ is the supremum of $H$ in $E$ (TVS, II, §2, No. 7, Prop. 18).

### 4. Subspaces and product spaces of fully lattice-ordered spaces

Let $E$ be a fully lattice-ordered space, $H$ a linear subspace of $E$. The order structure induced on $H$ by that of $E$ is compatible with the vector space structure of $H$, but the ordered vector space $H$ so defined *is not necessarily a fully lattice-ordered space*.

More precisely, it can happen that $H$ is not a Riesz space (Exer. 2), or that $H$ is a Riesz space but is not fully lattice-ordered: the latter is the case for the subspace $\mathcal{C}(\mathbf{R})$ of the space $\mathcal{B}(\mathbf{R})$ (No. 3, Example 2).

Moreover, if $H$ is a Riesz space (fully lattice-ordered or not) it can happen that the supremum *in* $H$ of two elements of $H$ is different from their supremum *in* $E$ (Exer. 3 *b*). Finally, it can happen that $H$ is fully lattice-ordered, that the supremum of each *finite* subset of $H$ is the same in $E$ and in $H$, but that there exist *infinite* subsets of $H$, bounded above in $H$, for which the suprema in $E$ and $H$ are different (Exer. 13 *f*)).

Let $(E_\iota)_{\iota \in I}$ be any family of ordered vector spaces. Recall that, in the product space $E = \prod_{\iota \in I} E_\iota$, the *product* order relation of the order relations of the factor spaces is the relation $« x_\iota \leqslant y_\iota \text{ for all } \iota \in I »$ (S, III, §1, No. 4). One verifies immediately that this relation is compatible with the vector space structure of E; E, equipped with this structure, is called the product space of the ordered spaces $E_\iota$.

#### Proposition 3 {#int-ii-s1-prop-3 .statement}

*Let $(E_\iota)_{\iota \in I}$ be a family of ordered vector spaces. For the product space $E = \prod_{\iota \in I} E_\iota$ to be a Riesz space (resp. a fully lattice-ordered space), it is necessary and sufficient that each of the spaces $E_\iota$ be a Riesz space (resp. a fully lattice-ordered space).*

Let us restrict ourselves to examining the case of fully lattice-ordered spaces. Suppose that all of the $E_\iota$ are fully lattice-ordered; let $A$ be a nonempty subset of $E$ that is bounded above and let $a = (a_\iota)$ be an upper bound for $A$. For every $\iota \in I$, $\operatorname{pr}_\iota A$ is bounded above by $a_\iota$, hence has a supremum $b_\iota$ in $E_\iota$; it is clear that $b = (b_\iota)$ is the supremum of $A$ in $E$.

Conversely, suppose $E$ is fully lattice-ordered. Let $A_\kappa$ be a subset of $E_\kappa$ that is bounded above, $A'_\kappa$ the subset of $E$ formed by the $x = (x_\iota)$ such that $x_\kappa \in A_\kappa$ and $x_\iota = 0$ for $\iota \neq \kappa$. It is immediate that $A'_\kappa$ is bounded above in $E$, hence has a supremum $b = (b_\iota)$; by the definition of the product order relation, necessarily $b_\iota = 0$ for $\iota \neq \kappa$, and $b_\kappa$ is the supremum of $A_\kappa$, which completes the proof.

#### Definition 3 {#int-ii-s1-def-3 .statement}

*Let $E$ be an ordered vector space, $V$ and $W$ two supplementary linear subspaces of $E$. One says that $E$ is the ordered direct sum of $V$ and $W$ if the canonical mapping $(x, y) \mapsto x + y$ of the ordered vector space $V \times W$ onto the ordered vector space $E$ is an isomorphism.*

#### Proposition 4 {#int-ii-s1-prop-4 .statement}

*For an ordered vector space $E$ to be the ordered direct sum of two supplementary linear subspaces $V, W$, it is necessary and sufficient that the relations $x \in V, y \in W, x + y \geq 0$ imply $x \geq 0$ and $y \geq 0$.*

Since $x \geq 0$ and $y \geq 0$ imply $x + y \geq 0$ in $E$, the condition in the statement says that $(x, y) \mapsto x + y$ transforms the set of elements $\geq 0$ of $V \times W$ into the set of elements $\geq 0$ of $E$.

### 5. Bands in a fully lattice-ordered space

#### Definition 4 {#int-ii-s1-def-4 .statement}

*In a fully lattice-ordered space $E$, a linear subspace $B$ of $E$ is said to be a band if it satisfies the following conditions: 1) the relations $x \in B, y \in E$ and $|y| \leq |x|$ imply $y \in B$; 2) for every nonempty subset $X$ of $B$ that is bounded above in $E$, the supremum $\sup X$ of $X$ in $E$ belongs to $B$.*

#### Example {#int-ii-s1-n5-exa-1 .statement}

In the space $\mathbf{R}^A$ of real-valued functions defined on a set $A$, the set of functions that are zero at all the points of a subset $M$ of $A$ is a band.

#### Remark {#int-ii-s1-n5-rem-1 .statement}

In the space $\mathbf{R}^A$, the subspace $\mathcal{B}(A)$ of bounded real-valued functions on $A$ satisfies condition 1) of Def. 4; moreover, for every subset $X$ of $\mathcal{B}(A)$ that is bounded above *in* $\mathcal{B}(A)$, the upper envelope of $X$ belongs to $\mathcal{B}(A)$. However, if $A$ is infinite, a subset of $\mathcal{B}(A)$ may be *bounded above in* $\mathbf{R}^A$ *without being bounded above in* $\mathcal{B}(A)$, in which case $\mathcal{B}(A)$ is not a band in $\mathbf{R}^A$.

It follows at once from Def. 4 that if $B$ is a band in $E$ then, for every nonempty subset $X$ of $B$ that is bounded below in $E$, $\inf X$ belongs to $B$. Every band $B$ in $E$, equipped with the ordered vector space structure induced by that of $E$, is a fully lattice-ordered space and, for every subset $X \subset B$ that is bounded above in $B$, the supremum of $X$ in $B$ is identical with its supremum in $E$.

The intersection of any family of bands in a fully lattice-ordered space $E$ is also a band. For every subset $M \subset E$, there exists a *smallest band* containing $M$ (since $E$ itself is a band); this band will be called the band *generated* by $M$.

The properties of bands in a fully lattice-ordered space rest on the following proposition:

#### Proposition 5 {#int-ii-s1-prop-5 .statement}

— *Let $E$ be a fully lattice-ordered space, $A$ a non-empty subset of $E$ consisting of elements $\geqslant 0$, such that: 1) $A + A \subset A$, and 2) the relations $x \in A,\ 0 \leqslant y \leqslant x$ imply $y \in A$. Let $M$ be the set of suprema in $E$ of those subsets of $A$ that are bounded above in $E$. Under these conditions, every element $x \geqslant 0$ of $E$ may be written in the form $y + z$, where $y \in M$ is the supremum of the elements $v \in A$ such that $v \leqslant x$, and where $z$ is an element $\geqslant 0$ that is alien to every element of $M$.*

At any rate $y \leqslant x$, so it all comes down to showing that $z = x - y$ is alien to every element $t \in A$ (No. 1), in other words that $u = \inf(z, t)$ is zero. By hypothesis, $u \in A$ and $u \leqslant x - y$, thus $u + y \leqslant x$; for every $v \in A$ such that $v \leqslant x$, by definition $v \leqslant y$, thus $u + v \leqslant u + y \leqslant x$; since $u + v \in A$ by hypothesis, also $u + v \leqslant y$ by the definition of $y$; finally, since $u + y$ is the supremum in $E$ of the elements $u + v$ such that $v \in A$ and $v \leqslant x$, we have $u + y \leqslant y$, whence $u \leqslant 0$, which completes the proof.

#### Theorem 1 (F. Riesz) {#int-ii-s1-thm-1 .statement}

— *Let $A$ be a subset of a fully lattice-ordered space $E$. The set $A'$ of elements that are alien to every element of $A$ is a band; the band $A''$ of elements that are alien to every element of $A'$ is identical to the band generated by $A$, and $E$ is the ordered direct sum of the bands $A'$ and $A''$.*

The properties of alien elements, reviewed in No. 1, and the definition of a band, show at once that $A'$ is a band, hence so is $A''$. By Proposition 5 and the definition of a band, every element $x \geqslant 0$ of $E$ may be written $x = y + z$, with $y \in A'$ and $z \in A''$, $y$ and $z$ being $\geqslant 0$; since every element of $E$ is the difference of two elements $\geqslant 0$, we have $E = A' + A''$; on the other hand, since $0$ is the only element alien to itself, we have $A' \cap A'' = \{0\}$, which proves that $E$ is the direct sum of $A'$ and $A''$; finally, since the components in $A'$ and $A''$ of an element $\geqslant 0$ of $E$ are $\geqslant 0$, $E$ is the ordered direct sum of $A'$ and $A''$ (No. 4, Prop. 4).

It remains to show that $A''$ is identical to the band $B$ generated by $A$. Now, $E$ is the direct sum of $B$ and the band $B'$ formed by the elements alien to all the elements of $B$; since $A \subset B$, we have $B' \subset A'$; on the other hand $B \subset A''$ and $E$ is also the direct sum of $A'$ and $A''$; therefore necessarily $B = A''$, $B' = A'$.

Theorem 1 and Proposition 5 make it possible to give another definition of the band generated by a set of elements of $E$:

#### Proposition 6 {#int-ii-s1-prop-6 .statement}

— *Let $E$ be a fully lattice-ordered space, $M$ a subset of $E$, and $B$ the band generated by $M$. Let $M_1$ be the set of elements $\geqslant 0$ of $E$ each of which is $\leqslant$ some element of the form $\sum_i |x_i|$, where $x_i \in M$; let $M_2$ be the set of suprema of those subsets of $M_1$ that are bounded above; then the set $M_2$ is identical with the set of elements $\geqslant 0$ of $B$.*

Clearly $M_2 \subset B$ by the definition of a band; on the other hand, if $B'$ is the band of elements that are alien to every element of $M_1$, Theorem 1 shows that $E$ is the ordered direct sum of $B$ and $B'$. But Proposition 5 shows that every element $\geqslant 0$ of $E$ is the sum of an element of $M_2$ and an element of $B'$, whence the proposition.

#### Corollary {#int-ii-s1-n5-cor-1 .statement}

— *Let $a$ be an element of a fully lattice-ordered space $E$, $B_a$ the band generated by $a$, $B'_a$ the band of elements alien to $a$. For every element $x \geqslant 0$ of $E$, the component of $x$ in $B_a$ (for the decomposition of $E$ as the ordered direct sum of $B_a$ and $B'_a$) is equal to $\sup_{n \in \mathbf{N}} (\inf(n|a|, x))$.*

This follows from Proposition 6, applied to $M = \{a\}$, and Proposition 5.

Note that the bands generated by $a$ and $|a|$ are identical. If $a$ and $b$ are two elements of $E$ that are alien to each other, and if $A$ and $B$ are the bands generated by $a$ and $b$, respectively, then every element of $A$ is alien to every element of $B$; for, $b$ belongs to the band $A'$ of elements alien to $a$, whence $B \subset A'$, and, by Theorem 1, every element of $A$ is alien to every element of $A'$.

### Exercises {#int-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
