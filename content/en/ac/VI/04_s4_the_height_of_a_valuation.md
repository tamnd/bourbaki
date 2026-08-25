---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 4
section_title: The height of a valuation
lang: en
source: ac-i-vii
book_pages: 393-399, 449-453
pdf_pages: 0411-0417, 0467-0471
extraction: ocr
subsections:
    - "no": 1
      title: INCLUSION OF VALUATION RINGS OF THE SAME FIELD
      page: 393
      pdf_page: 411
    - "no": 2
      title: ISOLATED SUBGROUPS OF AN ORDERED GROUP
      page: 394
      pdf_page: 412
    - "no": 3
      title: COMPARISON OF VALUATIONS
      page: 395
      pdf_page: 413
    - "no": 4
      title: THE HEIGHT OF A VALUATION
      page: 396
      pdf_page: 414
    - "no": 5
      title: VALUATIONS OF HEIGHT 1
      page: 397
      pdf_page: 415
statements: 18
exercises: 11
content_sha256: 241b523bbe6a35c37704c2aac29a38f7afcc9e1e0df9204c949f3665e008f232
---

## 4. THE HEIGHT OF A VALUATION

### 1. INCLUSION OF VALUATION RINGS OF THE SAME FIELD

#### Proposition 1 {#ac-vi-s4-prop-1 .statement}

*Let $K$ be a field and $A$ a valuation ring of $K$. Then:*
(a) *Every ring $B$ such that $A \subset B \subset K$ is a valuation ring of $K$;
(b) *The maximal ideal $m(B)$ of such a ring is contained in $A$ and it is a prime ideal of $A$;
(c) *The mapping $\mathfrak{p} \mapsto A$, is a decreasing bijection of the set of prime ideals of $A$ onto the set of rings $B$ such that $A \subset B \subset K$; its inverse bijection is the mapping $B \mapsto m(B)$.

If $B$ is a ring such that $A \subset B \subset K$ and $x \in K - B$, then $x \in K - A$, whence $x^{-1} \in m(A) \subset B$, which proves both that $B$ is a valuation ring of $K$ and that $m(B) \subset m(A)$; as $m(B) = m(B) \cap A$ is a prime ideal of $A$, we have shown (a) and (b). Moreover, $A_{m(B)} \subset B$; conversely, if $x \in B - A$, then $x^{-1} \in A$ and $x^{-1} \notin m(B)$ and hence $x \in A_{m(B)}$; thus $A_{m(B)} = B$. Finally let $\mathfrak{p}$ be a prime ideal of $A$; we write $B = A_{\mathfrak{p}}$; then $m(B) \cap A = \mathfrak{p}$. (Chapter II, § 2, no. 5, Proposition 11) and $m(B) \subset A$ by (b); hence $m(B) = \mathfrak{p}$, which shows that the mappings $\mathfrak{p} \mapsto A$, and $B \mapsto m(B)$ of the statement are inverse bijections.

#### Corollary {#ac-vi-s4-n1-cor-1 .statement}

*The set & subrings of K containing A is totally ordered by inclusion.*

The set of prime ideals of $A$ is totally ordered by inclusion ($\S$ 1, no. 2, Theorem 1 (e)) and the mapping $\mathfrak{p} \mapsto A_{\mathfrak{p}}$ reverses the inclusion relations.

#### Proposition 2 {#ac-vi-s4-prop-2 .statement}

*Let K be a field, B a valuation ring of K and h, the place & K associated with B (with values in $\kappa(B)$). Then the mapping $A \mapsto h_B(A)$ defines a bijection of the set $\mathcal{A}$ of valuation rings of K contained in B onto the set $\mathcal{A}'$ of valuation rings of $\kappa(B)$.

If $A \in \mathcal{A}$, then $h_B(A) \in \mathcal{A}'$: for if $x' = h_B(x)$ (where $x \in B$) is an element of $\kappa(B) - h_B(A)$, then $x \notin A$, hence $x^{-1} \in A$ and $h_B(x)^{-1} \in h_B(A)$. On the other hand, for $A \in \mathcal{A}$, $A \supset m(B)$ (Proposition 1 (b)) and hence the mapping,

$A \mapsto h_B(A)$ is injective. Finally, let $A' \in \mathcal{A}'$ and $A = h_B(A') \subset B$; we shall show, which will complete the proof, that $A \in \mathcal{A}$; if $x \in K - A$, then either $x \notin B$, or $x \in B$; if $x \notin B$, then $x^{-1} \in m(B) \subset A$; if $x \in B$, then $h_B(x) \in \kappa(B)$ and $h_B(x) \notin A$, hence $h_B(x^{-1}) \in A$ and we conclude again that $x^{-1} \in A$; hence $A \in \mathcal{A}$.

#### Corollary {#ac-vi-s4-n1-cor-2 .statement}

*Let A and B be two valuation rings of K, where $A \subset B$; let $A' = h_B(A)$, which is a valuation ring of $\kappa(B)$. The residue field $\kappa(A')$ of $A'$ is canonically isomorphic to the residue field $\kappa(A)$ of A and the place $h_A$ associated with A is the composition $h_{A'} \circ h_B$ of the places associated with A and B.*

Since the local ring $A'$ is a quotient of the local ring $A$, their residue fields are canonically isomorphic and the equation $h_A(x) = h_{A'}(h_B(x))$ holds for $x \in A$. On the other hand, if $x \in B - A$, then $h_B(x) \notin A'$ and the two sides of the equation are equal to $\infty$; the same is true if $x \in K - B$.

#### Remark {#ac-vi-s4-n1-rem-1 .statement}

Conversely, let $f$ be a place of K with values in $K'$ and $f'$ a place of $K'$ with values in $K''$. Then $f' \circ f$ is a place of K whose ring is contained in the ring of the place $f$.

### 2. ISOLATED SUBGROUPS OF AN ORDERED GROUP

To study the situation in no. 1 from the point of view of valuations we shall need Definition 1 and Proposition 3 below.

#### Definition 1 {#ac-vi-s4-def-1 .statement}

*A subgroup H of an ordered group G is called isolated if the relations $0 \leq y \leq x$ and $x \in H$ imply $y \in H$.*

Example (1) Let $A$ and $B$ be two ordered groups; let $A \times B$ be given the lexicographic order (i.e. "$(a, b) \leq (a', b')$" is equivalent to "$(a < a') \text{ or } (a = a' \text{ and } b \leq b')$"). The second factor $B$ of $A \times B$ is then, as is seen immediately, an isolated subgroup of $A \times B$.

#### Proposition 3 {#ac-vi-s4-prop-3 .statement}

Let $G$ be an ordered group and $P$ the set of its positive elements.

(a) *The kernel of an increasing homomorphism of $G$ to an ordered group is an isolated subgroup of $G$.*

(b) *Conversely, let $H$ be an isolated subgroup of $G$ and $g$ the canonical homomorphism of $G$ onto $G/H$. Then $g(P)$ is the set of positive elements of an ordered group structure on $G/H$. Moreover, if $G$ is totally ordered, so is $G/H$.*

(a) Let $f$ be an increasing homomorphism from $G$ to an ordered group; let $H$ denote the kernel off. If $0 \leq y \leq x$ and $x \in H$, then $0 \leq f(y) \leq f(x) = 0$, whence $f(y) = 0$, that is $y \in H$. Hence $H$ is isolated.

(b) Let $H$ be an isolated subgroup of $G$ and $g : G \to G/H$. Let $P' = g(P)$. Clearly $P' + P' \subset P'$. Also

$$
P' \cap (-P') = \{0\},
$$

for, *if* $x$ and $y$ are elements of $P$ such that $g(x) = -g(y)$, then $x + y \in H$, whence $x \in H$ and $y \in H$ since $H$ is isolated; hence $g(x) = g(y) = 0$. Thus $P'$ is the set of positive elements of an ordered group structure on $G/H$ (*Algebra*, Chapter VI, § 1, no. 3, Proposition 3). Finally, if $G$ is totally ordered, then $P \cap (-P) = G$, whence $P' \cup (-P') = G/H$ and therefore $G/H$ is totally ordered (*loc. cit.*).

Example (2) If we reconsider the example where $G$ is a lexicographic product $A \times B$ and $H = B$, the ordered group $G/H$ is canonically identified with $A$.

### 3. COMPARISON OF VALUATIONS

Let $K$ be a field and $A$ a valuation ring of $K$. For every subring $B$ of $K$ containing $A$, $U(A) \subset U(B)$. Then there is a canonical homomorphism $\lambda$ of $\Gamma_A = K^*/U(A)$ onto $\Gamma_B = K^*/U(B)$, whose kernel is $U(B)/U(A)$. Then, letting $v_A$ and $v_B$ denote the canonical valuations on $K$ defined by $A$ and $B$ (§ 3, no. 2),

(1)

$$
v_B = \lambda \circ v_A.
$$

As $A \subset B$, $\lambda$ maps the positive elements of $\Gamma_A$ to positive elements of $\Gamma_B$ and hence is increasing. Therefore (Proposition 3) the kernel $H$, of $\lambda$ is an isolated subgroup of $\Gamma_A$ and $\lambda$ factors into $\Gamma_A \to \Gamma_A/H_B \xrightarrow{\mu} \Gamma_B$, where $\mu$ is an increasing bijective homomorphism and hence an *isomorphism* of totally ordered groups; hence $\Gamma_B$ is identified with the quotient totally ordered group $\Gamma_A/H_B$.

#### Proposition 4 {#ac-vi-s4-prop-4 .statement}

*The mapping* $B \mapsto H_B$ *is an increasing bijection of the set of subrings of* $K$ *containing* $A$ *onto the set of isolated subgroups of* $\Gamma_A$.

Given $H$, $v_B$ is defined up to equivalence and hence $B$ is determined uniquely. On the other hand, let $H$ be an isolated subgroup of $\Gamma_A$; considering $\Gamma_A / H$ as a totally ordered group (Proposition 3), the composite mapping

$$
K^* \xrightarrow{v_A} \Gamma_A \longrightarrow \Gamma_A / H
$$

is a valuation on $K$ whose ring contains $A$.

#### Remark {#ac-vi-s4-n3-rem-1 .statement}

Under the above hypotheses, let $f$ denote the canonical homomorphism of $B$ onto $\kappa(B)$ and $A' = f(A)$; it is a valuation ring of $\kappa(B)$ (Proposition 2, no. 1). Then $f^{-1}(\kappa(B)^*) = U(B), f^{-1}(A') = A, f^{-1}(m(A')) = m(A)$, hence

$$
f^{-1}(U(A')) = U(A).
$$

Then there is a canonical isomorphism of $U(B)/U(A)$ onto $\kappa(B)^*/U(A') = \Gamma_{A'}$. The exact sequence

$$
0 \to U(B)/U(A) \to \Gamma_A \to \Gamma_B \to 0
$$

then gives an exact sequence

$$
0 \to \Gamma_{A'} \to \Gamma_A \to \Gamma_B \to 0.
$$

#### Example {#ac-vi-s4-n3-exa-1 .statement}

Let $k$ be a field,

$$
E = k(X) \quad \text{and} \quad K = k(X, Y) = E(Y)
$$

$(X, Y$ indeterminates). Let $B = E[Y]_{(Y)}$ be the valuation ring of $K$ defined by the extremal element $Y$ of the principal ideal domain $E[Y]$ (\S 1, no. 4, Proposition 3). The residue field $\kappa(B)$ is canonically identified with $E[Y]/(Y) = E$. Similarly, let $A' = k[X]_{(X)}$ be the valuation ring of $E = k(X)$ defined by the extremal element $X$ of $k[X]$. Denoting by $h$, the place of $E$ associated with $B$ and writing $A = h_B^{-1}(A')$, a valuation ring $A$ of $K$ is defined which is contained in $B$ and $\kappa(A) = \kappa(A') = k$. The canonical place $h$: $K \to k$ can be described as follows: iff $(X, Y)$ is an element of $K$, then we first put $Y = 0$ inf (which gives an element of $\tilde{E} = k(X)^*$), then $X = 0$ in the result obtained. The groups $\Gamma_{A'}$ and $\Gamma_B$ are canonically isomorphic to $\mathbf{Z}$ (\S 3, no. 4, Example 4). *It is not difficult to show (cf. \S 10, no. 2, Lemma 2) that the group $\Gamma_A$ is isomorphic to the lexicographic product $\mathbf{Z} \times \mathbf{Z}$ and that the valuation $v_A$ is equivalent to the valuation defined in \S 3, no. 4, end of Example 6.*

### 4. THE HEIGHT OF A VALUATION

Let $G$ be a totally ordered group. Given two isolated subgroups $H$ and $H'$ of $G$, one of them is contained in the order: for otherwise there would exist a positive element $x$ of $H$ not belonging to $H'$ and a positive element $x'$ of $H'$ not belonging to H; let, for example $x \geq x'$; as H is isolated, $x' \in H$, which is a contradiction.

This also follows from Proposition 4 of no. 3 and the Corollary to Proposition 1 of no. 1, taking account of the fact that every totally ordered group is the order group of a valuation (\$ 3, no. 4, Example 6).

#### Definition 2 {#ac-vi-s4-def-2 .statement}

*Let G be a totally ordered group. If the number of isolated subgroups of G distinct from G is finite and equal to n, G is said to be of height n. If this number is infinite, G is said to be of infinite height.*

Examples
(1) The height of the group $G = \{0\}$ is 0.
(2) The groups $\mathbf{Z}$ and $\mathbf{R}$ are of height 1.
(3) Let $G$ be a totally ordered group and $H$ an isolated subgroup of $G$. If $h(H)$ and $h(G/H)$ denote the heights of the totally ordered groups $H$ and $G/H$, then
$$
h(G) = h(H) + h(G/H),
$$
since the set of isolated subgroups of $G$ is totally ordered by inclusion. In particular, if $G$ is the lexicographic product of two totally ordered groups $H$ and $H'$, then
$$
h(G) = h(H) + h(H')
$$
(cf. no. 2, Example 2); thus the lexicographic product $\mathbf{Z} \times \mathbf{Z}$ is of height 2.

On the other hand the height of $\mathbf{Z} \times \mathbf{Z}$ ordered by embedding in $\mathbf{R}$ (cf. § 3, no. 4, end of Example 6) is equal to 1 (cf. Proposition 8 below).

#### Definition 3 {#ac-vi-s4-def-3 .statement}

*The height of the order group of a valuation is called the height of that valuation.*

For example a discrete valuation is of height 1. Only improper valuations are of height 0. Propositions 1 and 4 imply:

#### Proposition 5 {#ac-vi-s4-prop-5 .statement}

*The height of a valuation is equal to the number of non-zero prime ideals in its ring.*

### 5. VALUATIONS OF HEIGHT 1

#### Proposition 6 {#ac-vi-s4-prop-6 .statement}

*Let $\mathbf{K}$ be a field and $A$ a subring of $\mathbf{K}$. Suppose that $A$ is not a field. Then the following conditions are equivalent:*
(a) $A$ is the ring of a valuation of height 1 on $\mathbf{K}$;
(b) $A$ is a valuation ring of $\mathbf{K}$ and has no prime ideals other than $(O)$ and $m(A)$;
(c) $A$ is maximal among the subrings of $\mathbf{K}$ distinct from $\mathbf{K}$.

Proposition 5 of no. 4 shows that (a) implies (b) and Proposition 1 of no. 1 shows that (b) implies (c). It remains to show that (c) implies (a). Suppose A is maximal among the subrings of K distinct from K. Let m be a maximal ideal of A and V a valuation ring of K dominating A,, (§ 1, no. 2, Corollary to Theorem 2); as m(V) ∩ A = m and m ≠ (0) (since A is not a field), V ≠ K, whence V = A, which proves that A is not the ring of a valuation v on K. This being so, v is of height 1 by Propositions 1 (no. 1) and 5 (no. 4).

#### Proposition 7 {#ac-vi-s4-prop-7 .statement}

For a valuation on a field to be of height 1, it is necessary and sufficient that its order group be isomorphic to a non-zero ordered subgroup of \mathbf{R}.

This follows in fact from the following proposition:

#### Proposition 8 {#ac-vi-s4-prop-8 .statement}

Let G be a totally ordered group not reduced to O. The following conditions are equivalent:
(a) G is of height 1;
(b) for all x > 0 and y ≥ 0 in G, there exists an integer n ≥ 0 such that y ≤ nx;
(c) G is isomorphic to a subgroup of the ordered additive group \mathbf{R} which is not reduced to O.

Let x be a positive element of G and let H, be the set of y ∈ G such that there exists an integer n ≥ 0 satisfying |y| ≤ nx. It is easily verified that H, is an isolated subgroup of G and that every isolated subgroup of G containing x contains H,. Condition (a) is therefore equivalent to “H, = G for all x > 0”, that is, to condition (b).

Clearly (c) implies (b). Conversely, suppose condition (b) holds and let Q denote the set of elements >0 of G. Suppose first that Q has a least element x; for all y ∈ Q, let n be the least integer such that y ≤ nx; if y < nx, then also nx − y ≥ x, whence y ≤ (n − 1)x contrary to the choice of n; then y = nx, which shows that G = \mathbf{Z}x is isomorphic to \mathbf{Z} ⊂ \mathbf{R}. Suppose now that Q has no least element; we apply to the ordered set P = Q ∪ (0) Proposition 1 of General Topology, Chapter V, § 2 (which is possible, since condition (b) is just “Archimedes’ axiom”); it is seen that there exists a strictly increasing mapping f of P to \mathbf{R}_+ such that

$$
f(x + y) = f(x) + f(y)
$$

for x ∈ P and y ∈ P; by linearity f can be extended to an isomorphism of G onto a subgroup of \mathbf{R}, which proves that (b) implies (c).

#### Proposition 9 {#ac-vi-s4-prop-9 .statement}

Let K be a field, v a non-improper valuation on K and A the ring of v. For A to be completely integrally closed (Chapter V, § 1, no. 4, Definition 5), it is necessary and sufficient that v be of height 1.

Suppose v is of height 1. Let x ∈ K be such that the x^n (n ≥ 0) are all contained in a finitely generated sub-A-module of K. There exists d ∈ A − {0} such that dx^n ∈ A for all n ≥ 0. Then v(d) + nv(x) ≥ 0, that is n(−v(x)) ≤ v(d) for all $n \geqslant 0$, whence $-v(x) \leqslant 0$ (Proposition 8 (b)) and $x \in A$. Thus A is completely integrally closed.

Suppose now that v is not of height 1. Then there exist $y \in m(A)$ and $t \in A$ such that $nv(y) < v(t)$ for all $n \geqslant 0$ (Proposition 8 (b)). Then $ty^{-n} \in A$ for all $n \geqslant 0$, but $y^{-1} \notin A$. Hence A is not completely integrally closed.

#### Corollary {#ac-vi-s4-n5-cor-1 .statement}

*Let K be a field, $(v_\alpha)_{\alpha \in I}$ a family of valuations of height 1 on K and A the intersection of the rings of the v.* Then A is a completely integrally closed domain.

A completely integrally closed domain is not always an intersection of valuation rings of height 1 (Exercise 6).

### Exercises {#ac-vi-s4-exercises}

See the [exercises for § 4](exercises/s4/).
