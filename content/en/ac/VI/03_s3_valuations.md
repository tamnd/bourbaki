---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 3
section_title: Valuations
lang: en
source: ac-i-vii
book_pages: 385-393, 446-449
pdf_pages: 0403-0411, 0464-0467
extraction: ocr
subsections:
    - "no": 1
      title: VALUATIONS ON A RING
      page: 385
      pdf_page: 403
    - "no": 2
      title: VALUATIONS ON A FIELD
      page: 387
      pdf_page: 405
    - "no": 3
      title: TRANSLATIONS
      page: 389
      pdf_page: 407
    - "no": 4
      title: EXAMPLES OF VALUATIONS
      page: 389
      pdf_page: 407
    - "no": 5
      title: IDEALS OF A VALUATION RING
      page: 391
      pdf_page: 409
    - "no": 6
      title: DISCRETE VALUATIONS
      page: 392
      pdf_page: 410
statements: 15
exercises: 8
content_sha256: 7c8006eb587e0c29f6ccf241727bf3ea54908994e1ee0854ab2d41fc36b2d06d
---

## 3. VALUATIONS

### 1. VALUATIONS ON A RING

Let $\Gamma$ be a totally ordered commutative group written additively. In the rest of this chapter, we shall have to consider, for such a group, the set obtained by adjoining to $\Gamma$ an element denoted by $+\infty;$ we shall denote this set by $\Gamma_\infty$ and we shall give it: (1) a total ordering for which $+\infty$ is the greatest element, in other words, such that $a < +\infty$ for all $a \in \Gamma;$ (2) a commutative monoid structure whose law induces on $\Gamma$ the given group law and is defined by the equations

$$
(+\infty) + (+\infty) = +\infty, \quad a + (+\infty) = +\infty
$$

for all $\alpha \in \Gamma$; it is immediately verified that this law is associative and commutative and that the relation $\alpha_1 \leq \beta$ in $\Gamma_\infty$ implies $\alpha_1 + \gamma \leq \beta + \gamma$ for all $\gamma \in \Gamma_a$.

#### Definition 1 {#ac-vi-s3-def-1 .statement}

*Let $C$ be a (not necessarily commutative) ring and $\Gamma$ a totally ordered commutative group written additively. A valuation on $C$ with values in $\Gamma$ is any mapping $v : C \to \Gamma_\infty$ which satisfies the following conditions:*

(VL_I) $v(xy) = v(x) + v(y)$ for $x \in C, y \in C$.
(VL_{II}) $v(x + y) \geq \inf(v(x), v(y))$ for $x \in C, y \in C$.
(VL_{III}) $v(1) = 0$ and $v(0) = +\infty$.

If $C$ has no divisor of zero other than 0, the unique mapping $v_0$ of $C$ to $\Gamma_\infty$ such that $v_0(x) = 0$ for $x \neq 0$ and $v_0(0) = +\infty$ is a valuation, called the *improper valuation* on $C$. If $z \in C$ is such that $z^n = 1$ for some integer $n \geq 1$, then, by (VL_I), $nv(z) = v(z^n) = 0$ and hence $v(z) = 0$ for *every* valuation $v$ on $C$, since $\Gamma$ is a totally ordered group. In particular $v(-1) = 0$, whence $v(-x) = v(x)$ for all $x \in C$. Moreover, it follows from (VL_I) that $v(xy) = v(yx)$ for all $x, y$ in $C$. If $x$ is invertible in $C$, then $v(x^{-1}) = -v(x)$.

#### Proposition 1 {#ac-vi-s3-prop-1 .statement}

*Let $v$ be a valuation on a (not necessarily commutative) ring $C$. For any elements $x_i \in C$ ($1 \leq i \leq n$),*

$$
v \left( \sum_{i=1}^n x_i \right) \geq \inf_{1 \leq i \leq n} v(x_i)
$$

Moreover, if there exists a single index $k$ such that $v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$, the two sides of (1) are equal. In particular, if $v(x) \neq v(y)$, then $v(x + y) = \inf(v(x), v(y))$.

Relation (1) follows from axiom (VL_{II}) by induction on $n$. If there exists a single index $k$ such that $v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$, then, writing $y = \sum_{i \neq k} x_i$ and $z = \sum_{i=1}^n x_i$, $v(y) > v(x_k)$ and $v(z) \geq v(x_k)$ by (1); if $v(z) > v(x_k)$, the relation $x_k = z - y$ would give $v(x_k) \geq \inf(v(z), v(y)) > v(x_k)$, which is absurd; whence $v(z) = v(x_k)$, which proves the second assertion.

#### Corollary {#ac-vi-s3-n1-cor-1 .statement}

*If a finite sequence of elements $(x_i)_{1 \leq i \leq n}$ of $C$ (for $n \geq 2$) is such that $\sum_{i=1}^n x_i = 0$, there exist at least two distinct indices $j, k$ such that*

$$
v(x_j) = v(x_k) = \inf_{1 \leq i \leq n} v(x_i).
$$

If there were only a single index $k$ such that $v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$, Proposition 1 would show that $v(x_k) = v(0) = +\infty$, whence $v(x_i) = +\infty$ for all $i$, contrary to the relation $n \geq 2$ and the hypothesis made on $k$.

Remarks
(1) If $v : C \to \Gamma_\infty$ is a valuation on $C$ and $u : B \to C$ a homomorphism of a ring $B$ to $C$, it is immediate that the composite mapping $B \xrightarrow{u} C \xrightarrow{v} \Gamma_\infty$ is a valuation on $B$ with values in $\Gamma$.

(2) Conditions (VL$_I$) and (VL$_II$) show immediately that the set $\bar{v}^{-1}(+\infty)$ is a two-sided ideal $\mathfrak{p}$ in $C$ distinct from $C$ by virtue of (VL$_III$); moreover, if $x, y$ are two elements of $C$ such that $v(xy) = +\infty$, it follows from (VL,) that necessarily $v(x) = +\infty$ or $v(y) = +\infty$; in other words, the quotient ring $C/\mathfrak{p}$ has no divisor of 0 other than 0; it is immediately verified that the mapping $\bar{v} : C/\mathfrak{p} \to \Gamma_\infty$ derived from $v$ by passing to the quotient is a valuation on $C/\mathfrak{p}$, the inverse image of $+\infty$ under this valuation reducing to 0.

### 2. VALUATIONS ON A FIELD

#### Proposition 2 {#ac-vi-s3-prop-2 .statement}

Let $K$ be a (not necessarily commutative) field and $v$ a valuation on $K$ with values in $\Gamma$. Then:
(i) For $x \neq 0$, $v(x) \neq +\infty$.
(ii) The set $A$ of $x \in K$ such that $v(x) \geq O$ is a subring of $K$.
(iii) For all $a \geq O$ in $\Gamma$, the set $V$, (resp. $V'_a$) of $x \in A$ such that $v(x) > a$ (resp. $v(x) \geq a$) is a two-sided ideal of $A$ and every (left or right) ideal $\neq (O)$ of $A$ contains $m$ of the $V'_a$.
(iv) The set $m(A)$ of $x \in A$ such that $v(x) > O$ is the greatest ideal $\#A$ in $A$; $U(A) = A - m(A)$ is the set of invertible elements of $A$ and $\kappa(A) := A/m(A)$ is a (not necessarily commutative) field.
(v) For all $x \in K - A$, $x^{-1} \in m(A)$.

Assertion (i) follows from the fact that $\bar{v}^{-1}(+\infty)$ is an ideal of $K$ not equal to $K$. The verification of the fact that $A$ is a ring and the $V$, and $V'_a$ two-sided ideals is trivial by virtue of axioms (VL$_I$), (VL$_II$) and (VL$_III$). If $a$ is a (left, for example) ideal of $A$ and $x \neq 0$ belongs to $A$, every $y \in A$ such that $v(y) \geq v(x)$ can be written $y = zx$ where $z = yx^{-1}$, hence $v(z) = v(y) - v(x) \geq O$ and therefore $z \in A$; in other words the left ideal $Ax$ contains the $V'_a$ for $a > v(x)$. The set $U(A) = A - m(A)$ is the set of $x \in K$ such that $v(x) = 0$; if $x \in U(A)$, then
$$
v(x^{-1}) = -v(x) = 0,
$$
whence $x^{-1} \in U(A)$; conversely, if $y \in A$ is invertible in $A$, then $v(y) \geq 0$, $v(y^{-1}) \geq 0$ and $v(y) + v(y^{-1}) = 0$, whence $v(y) = 0$ and $y \in U(A)$; this proves (iv) and (v) follows immediately from the definitions.

$A$ (resp. $m(A)$, $\kappa(A)$) is called the ring (resp. ideal, residue field) of the valuation $v$ on $K$.

Clearly U(A) is the kernel of the homomorphism $v : K^* \to \Gamma$ and the image $v(K^*)$ under $v$ of the multiplicative group $K^*$ is a subgroup of the additive group $\Gamma$, called the order group or value group of $v$, which is therefore isomorphic to $K^*/U(A)$; for $x \in K$, the element $v(x)$ of $\Gamma_\infty$ is sometimes called the valuation or order of $x$ for $v$. Two valuations $v, v'$ on $K$ are called equivalent if they have the same ring.

#### Proposition 3 {#ac-vi-s3-prop-3 .statement}

*For two valuations $v, v'$ over a (not necessarily commutative) field $K$ to be equivalent, it is necessary and sufficient that there exist an isomorphism $\lambda$ of the ordered group $v(K^*)$ onto the ordered group $v'(K^*)$ such that $v' = A \circ v$.*

Suppose $v$ and $v'$ are equivalent; by hypothesis, the ring $A$ of the valuation $v$ being the same as that of $v'$, $v$ and $v'$ (restricted to $K^*$) factor into homomorphisms $K^* \to K^*/U(A) \xrightarrow{\mu} v(K^*)$, $K^* \to K^*/U(A) \xrightarrow{\nu} v'(K^*)$, where $\mu$ and $\nu$ are isomorphisms; moreover, the set of positive elements of $v(K^*)$ (resp. $v'(K^*)$) is the image under $\mu$ (resp. $\nu$) of the set of classes mod. $U(A)$ of elements $\neq 0$ of $m(A)$; we conclude that $A = v \circ \mu^{-1}$ solves the problem, the converse being obvious.

Suppose now that $K$ is a commutative field; then, for all valuations $v$ on $K$, the ring $A$ of the valuation $v$ is a valuation ring of $K$ in the sense of § 1, no. 2, Definition 2 (which justifies the terminology); this follows immediately from Proposition 2 (c) and § 1 no. 2, Theorem 1 (c). *Conversely*, recall that for every integral domain $B$ whose field of fractions is $K$ the relation of divisibility $x|y$ (equivalent to $y \in Bx$) makes $K^*$ into a preordered group, whose *associated ordered group* $\Gamma_B$ is the quotient $K^*/U(B)$ of $K^*$ by the group $U(B)$ of invertible elements of $B$, the positive elements of this group being those of $B^*/U(B)$ (where $B^* = B - \{0\}$); the mapping $x \mapsto Bx$ defines, by passing to the quotient, an isomorphism of the ordered group $K^*/U(B)$ onto the group (ordered by the relation $\supset$) of non-zero principal fractional ideals of $K$ (*Algebra*, Chapter VI, § 1, no. 5). The rings $A$ with field of fractions $K$ and for which the group $\Gamma_A = K^*/U(A)$ is *totally ordered* are precisely the *valuation rings of K* (§ 1, no. 2, Theorem 1 (d)). If $v_A$ denotes the canonical homomorphism of $K^*$ onto $\Gamma_A$, it is immediate that $v_A$ (extended by $v_A(0) = +\infty$) is a valuation (called *canonical*) on $K$ whose ring is $A$; every valuation equivalent to $v_A$ may be written $v = \sigma \circ v_A$, where $\sigma$ is an isomorphism of $\Gamma_A$ onto a subgroup of the group where $v$ takes its values (Proposition 3); $\sigma \circ v_A$ is called the *canonical factorization* of $v$.

#### Proposition 4 {#ac-vi-s3-prop-4 .statement}

*Let $C$ be an integral domain, $K$ its field of fractions, $C^* = C - \{0\}$ and $v : C \to \Gamma_\infty$ a valuation on $C$. Then there exists a unique valuation $w$ on $K$ which extends $v$ and $w(K^*)$ is the subgroup of $\Gamma$ generated by $v(C^*)$.*

By Theorem 2 of *Algebra*, Chapter I, § 2, no. 7, there exists a unique homomorphism $w$ from $K^*$ to $\Gamma$ which extends $v|C^*$ and $w(K^*)$ is generated by $v(C^*)$. It remains to prove that $w$ satisfies axiom (VL,,). Then let $x' \in K^*, y \in K^*$ be such that $x + y \in K^*$; there exists $a \in \mathbf{C}^*$ such that $ax \in \mathbf{C}^*$ and $ay \in \mathbf{C}^*$, whence $a(x + y) \in \mathbf{C}^*$. Since the restriction of $w$ to $\mathbf{C}^*$ satisfies (VL$_{\text{II}}$),

$$
w(a(x + y)) \geq \inf(w(ax), w(ay)).
$$

Eliminating $w(a)$ from both sides, we obtain

$$
w(x + y) \geq \inf(w(x), w(y)).
$$

### 3. TRANSLATIONS

Let $K$ be a (commutative) field, $f$ a place of $K$, $v$ a valuation on $K$ and $A$ a valuation ring of $K$. We shall say that $A, f$ and $v$ are *associated* if $A$ is the ring of $f$ and the ring of $v$. By virtue of no. 1 and § 2, no. 3, each of the three objects $A$, $f$ and $v$ then determines the other two (up to an equivalence as far as places and valuations are concerned). In particular there are the following equivalences:

$$
\begin{array}{lll}
x \in A & \Leftrightarrow & f(x) \neq \infty \\
x \in m(A) & \Leftrightarrow & f(x) = 0 \\
x \in A - m(A) = U(A) & \Leftrightarrow & f(x) \neq 0 \quad \text{and} \quad f(x) \neq \infty \Leftrightarrow v(x) = 0 \\
x \in K - A & \Leftrightarrow & f(x) = \infty & \Leftrightarrow & v(x) < 0
\end{array}
$$

Every result relating to valuation rings, places or valuations can be translated into a result relating to the other two notions. Thus Proposition 4 of § 2, no. 4 gives:

#### Proposition 5 {#ac-vi-s3-prop-5 .statement}

*Let $K$ be a field, $v$ a valuation on $K$ and $K'$ an extension of $K$. There exists a valuation $v'$ on $K'$ whose restriction to $K$ is equivalent to $v$.*

Let $\Gamma_v$ and $\Gamma_{v'}$ be the order groups of $v$ and $v'$. Since the restriction of $v'$ to $K$ is equivalent to $v$, there exists an isomorphism $A$ of $\Gamma_v$ onto a subgroup of $\Gamma_{v'}$, such that $v' = A \circ v$ on $K$. If $\Gamma_v$ is identified with $\lambda(\Gamma_v)$ by means of $\lambda$, it is seen that $v'$ extends $v$.

Note that $\Gamma_{v'}$ is in general *distinct from* $\lambda(\Gamma_v)$ and the equivalence class of $v'$ is not necessarily unique. We shall return *to* this in § 8.

Translating Theorem 3 of § 1, no. 3 (or Proposition 6 of § 2, no. 5), we obtain:

#### Proposition 6 {#ac-vi-s3-prop-6 .statement}

*Let $K$ be a field, $A$ a subring of $K$ and $x$ an element of $K$. For $x$ to be integral over $A$, it is necessary and sufficient that every valuation on $K$ which is positive on $A$ be positive at $x$.*

From now on, we shall in general leave to the reader the trouble of performing translations analogous to the above.

### 4. EXAMPLES OF VALUATIONS

The examples of valuation rings given in § 1, no. 4 provide us with *Examples 1 to 4* below:

Example (1) Every valuation on a finite field F is improper, since every element of F* is a root unity.

Example (2) If K is a subfield of a field K', the restriction to K of a valuation on K' is a valuation on K.

Example (3) Let k be a field and K = k((T)). The mapping v which maps every non-zero formal power series to its order (Algebra, Chapter IV, § 5, no. 7) is a valuation on K whose order group is Z and whose ring is k[[T]]. The associated place is the canonical homomorphism f: k[[T]] → k extended to k((T)) by setting f(u) = ∞ if u ∉ k[[T]].

Example (4) Let A be a principal ideal domain, K its field of fractions and p an extremal element of A. For x ∈ K* let v_p(x) denote the exponent of p in the decomposition of x into extremal elements (Algebra, Chapter VII, § 1, no. 3, Theorem 2); it is immediately seen that v_p is a valuation whose order group is Z and whose ring is A_{A_p}. By Proposition 3 of § 1, no. 4 we thus obtain, up to equivalence, all the valuations on K which are not improper and are positive on A. Taking A = Z we recover the p-adic valuations on Q (General Topology, Chapter IX, § 3, no. 2); these valuations are, up to equivalence, the only valuations on Q which are not improper (§ 1, no. 4, Corollary 1 to Proposition 3). Taking A = k[X], where k is a field, the non-improper valuations on k(X) whose restrictions to k are improper are (up to equivalence): on the one hand the valuations v_P where P runs through the set of irreducible monic polynomials of k[X] and on the other hand the valuation v defined by

$$
v(P/Q) = \deg(Q) - \deg(P)
$$

for P ∈ k[X] and Q ∈ k[X] (§ 1, no. 4, Corollary 2 to Proposition 3); all these valuations obviously have Z as order group and their residue fields are monogenous algebraic extensions of k (Algebra, Chapter V, § 3, no. 1).

Example (5) The mapping P(X, Y) ↦ P(T, e^T) of C[X, Y] to C((T)) is injective (Functions of a real variable, Chapter IV, §2, Proposition 9) and therefore can be extended to an isomorphism of C(X, Y) onto a subfield of C((T)). The restriction to this subfield of the valuation on C((T)) defined in Example 3 defines a valuation on C(X, Y) which is improper on C, whose order group is Z and whose residue field is C.

Proposition 4 of no. 2 allows us to construct a valuation whose order group and residue field are given:

Example (6) Let Γ be a totally ordered group and k a field. Let Γ_+ be the monoid of positive elements of Γ and C the algebra of Γ_+ over k. By definition, C has a basis (x_\alpha)_{\alpha \in \Gamma_-} over k whose multiplication table is x_\alpha x_\beta = x_{\alpha + \beta}. If $x = \sum a_\alpha x_\alpha$ is a non-zero element of C, we write $v(x) = \inf_{a_\alpha \neq 0} (a)$ and $v(0) = +\infty$; it is immediately verified that the mapping $v$ of $C$ to $\Gamma_\infty$ satisfies conditions (VL_I) and (VL_{II}) of no. 1 and that $C$ is an integral domain. Let $K$ be the field of fractions of $C$ and $w$ the valuation on $K$ which extends $v$ (Proposition 4, no. 2). As every element of $\Gamma$ is the difference of two positive elements, $w$ admits $\Gamma$ as order group. Let $A$ be the ring of $w$ and $m$ its maximal ideal; we shall show that $A$ is the direct sum of $m$ and $k$ (identified with $k \cdot 1$), which will prove that the residue field of $w$ is isomorphic to $k$. Clearly $m \cap k = (0)$. On the other hand, denoting by $p$ the ideal of $C$ generated by the $x_a$ where $a > 0$, every element $x$ of valuation 0 in $K$ can be written in the form $(a + y)/(b + z)$ where $a \in k^*, b \in k^*, y \in p$ and $z \in p$; then

$$
x = ab^{-1} + (by - az)b^{-1}(b + z)^{-1}
$$

whence $w(x - ab^{-1}) > 0$ and $x \equiv ab^{-1} \pmod{m}$; this shows our assertion.

If $\Gamma = \mathbf{Z} \times \mathbf{Z}$, then $K = k(X, Y)$ and the above construction then provides valuations on $k(X, Y)$ which are improper on $k$, whose order group is $\mathbf{Z} \times \mathbf{Z}$ and whose residue field is $k$. These valuations depend on the order structure chosen on $\mathbf{Z} \times \mathbf{Z}$. For example, $\mathbf{Z} \times \mathbf{Z}$ can be given the lexicographic ordering. Or indeed, for an irrational number $a$, $\mathbf{Z} \times \mathbf{Z}$ may be identified with a subgroup of $\mathbf{R}$ under the homomorphism $(m, n) \mapsto m + n\alpha$ (a homomorphism which is injective since $a$ is irrational) and given the ordering induced by that on $\mathbf{R}$.

Other constructions of valuations using Proposition 4 of no. 2 will be described in § 10.

### 5. IDEALS OF A VALUATION RING

#### Definition 2 {#ac-vi-s3-def-2 .statement}

*Let G be an ordered set. A subset of G is called major if the relations $x \in M$ and $y \geq x$ imply $y \in M$.*

Let $K$ be a field, $v$ a valuation on $K$, $A$ the ring of $v$ and $G$ the order group of $v$. For every major subset $M \subset G$, let $a(M)$ be the set of $x \in K$ such that $v(x) \in M \cup \{+\infty\}$. Clearly $a(M)$ is a sub-A-module of $K$.

#### Proposition 7 {#ac-vi-s3-prop-7 .statement}

*The mapping $M \mapsto a(M)$ is an increasing bijection of the set of major subsets of $G$ onto the set of sub-A-modules of $K$.*

Let $b$ be a sub-A-module of $K$. The set of $v(x)$ for $x \in b - (0)$ is a major subset $M(b)$ of $G$. Proposition 7 will be shown if the following equations are proved:

(2) $M(a(N)) = N$ for every major subset $N$ of $G$;
(3) $a(M(b)) = b$ for every sub-A-module $b$ of $K$.

Formula (2) is easy, since, for all $m \in N$, there exists $x \in K$ such that $v(x) = m$. Then obviously $b \subset a(M(b))$; conversely, let $x \in a(M(b))$ and suppose $x \neq 0$;

then $v(x) \in M(b)$ and therefore there exists $y \in b$ such that $v(x) = v(y)$; whence $x = uy$ where $v(u) = 0$, which proves that $x \in A$ $y \subset b$ and completes the proof.

#### Corollary {#ac-vi-s3-n5-cor-1 .statement}

Let $G_+$ be the set of positive elements in $G$. The mapping $M \mapsto a(M)$ is a bijection of the set of major subsets of $G_+$, onto the set of ideals of $A$.

As $A = a(G_+)$, $a(M) \subset A$ is equivalent to $M \subset G_+$.

For example the maximal ideal $m(A)$ is equal to $a(S)$, where $S$ denotes the set of strictly positive elements of $G$.

### 6. DISCRETE VALUATIONS

#### Definition 3 {#ac-vi-s3-def-3 .statement}

Let $K$ be a (not necessarily commutative) field, $v$ a valuation on $K$ and $\Gamma$ the order group of $v$. $v$ is called discrete if there exists a (necessarily unique) isomorphism of the ordered group $\Gamma$ onto $\mathbf{Z}$. Let $\gamma$ be the element of $\Gamma$ corresponding to $1$ under this isomorphism; every element $u$ of $K$ such that $v(u) = \gamma$ is called a uniformizer of $v$. A discrete valuation is called normed if its order group is $\mathbf{Z}$.

For example the valuation $v_p$ defined by an extremal element $p$ of a principal ideal *or factorial, domain is a normed discrete valuation which admits $p$ as a uniformizer. In particular, if $k$ is a field, $k[[T]]$ is the ring of a discrete valuation on $k((T))$ which admits $T$ as a uniformizer. Let $S$ be a connected complex analytic variety of dimension 1, $K$ the field of meromorphic functions on $S$ and $z_0$ a point of $S$; the set off $\in K$ which are holomorphic at $z_0$ is the ring of a discrete valuation $v$; for a function $f \in K$ to be uniformizing for $v$, it is necessary and sufficient that it be holomorphic and zero at $z_0$ and that there exist a neighbourhood $V$ of $z_0$ in $S$ such that the restriction off to $V$ be a homomorphism of $V$ onto a neighbourhood of the origin in $\mathbf{C}$. It is this example and other analogues which are the origin of the word "uniformizer".*

#### Proposition 8 {#ac-vi-s3-prop-8 .statement}

Let $K$ be a (not necessarily commutative) field, $v$ a discrete valuation on $K$, $A$ the ring of $v$ and $u$ a uniformizer for $v$. The non-zero ideals of $A$ are two-sided and of the form $Au^n$ ($n \geq 0$).

It may be assumed that $v$ is normed, so that $v(u) = 1$. For all $x \in K^*$, there is an integer $n \in \mathbf{Z}$ such that $(v(x) = n = v(u^n)$ and hence we may write

$$
x = zu^n = u^n z',
$$

where $z, z'$ are two invertible elements of the ring $A$; whence the proposition.

#### Proposition 9 {#ac-vi-s3-prop-9 .statement}

Let $A$ be a local integral domain distinct from its field of fractions. The following conditions are equivalent:
(a) $A$ is the ring of a discrete valuation.
(b) $A$ is a principal ideal domain.
(c) The ideal $m(A)$ is principal and $\bigcap_{n=1}^{\infty} m(A)^n = (0)$.

(d) $A$ is a *Noetherian ring* and $m(A)$ is *principal*.
(e) $A$ is a *Noetherian valuation ring*.

Proposition 8 shows that (a) implies (b), (d) and (e). If $A$ is a principal ideal domain, then $m(A) = Au$ and every non-zero ideal of $A$ is of the form $Au^n$ since $A$ is local (*Algebra*, Chapter VII, § 1, no. 3, Theorem 2); therefore $\bigcap_{n=1}^\infty m(A)^n = 0$; this shows that (b) implies (c). On the other hand (d) implies (c) (Chapter III, § 3, no. 2, Corollary to Proposition 5); by Proposition 2 of § 1, no. 4, (c) implies (a). Thus conditions (a), (b), (c), (d) are equivalent and imply (e). Finally suppose (e) holds and let us show that (b) holds; it will be sufficient to prove the following lemma:

#### Lemma 1 {#ac-vi-s3-lem-1 .statement}

*Let $A$ be a valuation ring. Every finitely generated torsion-free $A$-module is free. Every finitely generated ideal $\mathfrak{a}$ of $A$ is principal. Every torsion-free $A$-module is flat.*

Let $E$ be a finitely generated torsion-free $A$-module and let $x_1, \ldots, x_n$ be generators of $E$ which are minimal in number; we show that they are linearly independent. If $\sum_{i=1}^n a_i x_i = 0$ ($a_i \in A$) is a non-trivial relation between the $x_i$, one of the $a_i$, say $a_1$, divides all the others since the set of principal ideals of $A$ is totally ordered by inclusion (§ 1, no. 2, Theorem 1); then $a_1 \neq 0$ since the relation is non-trivial. As $E$ is torsion-free, we can divide by $a_1$, which amounts to assuming that $a_1 = 1$. But then $x_1$ is a linear combination of $x_2, \ldots, x_n$, contrary to the minimal character of $n$. Hence $E$ is free.

In particular every finitely generated ideal $\mathfrak{a}$ of $A$ is principal, all the elements of a system of generators of $\mathfrak{a}$ being multiples of one of them. Proposition 3 of Chapter I, § 2, no. 4 then shows that every torsion-free $A$-module is flat.

### Exercises {#ac-vi-s3-exercises}

See the [exercises for § 3](exercises/s3/).
