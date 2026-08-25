---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 3
section_title: Factorial domains
lang: en
source: ac-i-vii
book_pages: 502-512
pdf_pages: 0520-0530
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF FACTORIAL DOMAINS
      page: 502
      pdf_page: 520
    - "no": 2
      title: CHARACTERIZATIONS OF FACTORIAL DOMAINS
      page: 502
      pdf_page: 520
    - "no": 3
      title: DECOMPOSITION INTO EXTREMAL ELEMENTS
      page: 504
      pdf_page: 522
    - "no": 4
      title: RINGS OF FRACTIONS OF A FACTORIAL DOMAIN
      page: 505
      pdf_page: 523
    - "no": 5
      title: POLYNOMIAL RINGS OVER A FACTORIAL DOMAIN
      page: 505
      pdf_page: 523
    - "no": 6
      title: FACTORIAL DOMAINS AND ZARISKI RINGS
      page: 506
      pdf_page: 524
    - "no": 7
      title: PRELIMINARIES ON AUTOMORPHISMS OF RINGS OF FORMAL POWER SERIES
      page: 506
      pdf_page: 524
    - "no": 8
      title: THE PREPARATION THEOREM
      page: 507
      pdf_page: 525
    - "no": 9
      title: FACTORIALITY OF RINGS OF FORMAL POWER SERIES
      page: 511
      pdf_page: 529
statements: 19
exercises: 0
content_sha256: 9a9045d263d1c89874a549163bdb7f5c0542895d8b247dce4869a232dfc8d799
---

## 3. FACTORIAL DOMAINS

### 1. DEFINITION OF FACTORIAL DOMAINS

#### Definition 1 {#ac-vii-s3-def-1 .statement}

A Krull domain all of whose divisorial ideals are principal is called a factorial (or unique factorization) domain.

In other words, the group of divisor classes (\S 1, no. 2) is reduced to 0.

Examples
(1) Every principal ideal domain is factorial (and, recall, is a Dedekind domain). Conversely, every factorial Dedekind domain is a principal ideal domain by \S 2, no. 2, Theorem 1 (c).
(2) In particular, if K is a field, the rings K[X] and K[[X]] are factorial domains (see Theorem 2 and Proposition 8 below for generalizations).
(3) \* The local ring of a simple point of an algebraic variety is a factorial domain. The ring of germs of functions analytic at the origin of $\mathbf{C}^n$ is a factorial domain. \*

### 2. CHARACTERIZATIONS OF FACTORIAL DOMAINS

Given a ring $A$, we need to consider the following condition:

(M) Every non-empty family of integral principal ideals of $A$ has a maximal element.

#### Theorem 1 {#ac-vii-s3-thm-1 .statement}

Let $A$ be an integral domain. The following conditions are equivalent:
(a) $A$ is factorial;
(b) the ordered group of non-zero fractional principal ideals of $A$ is a direct sum of groups isomorphic to $\mathbf{Z}$ (ordered by the product order);
(c) condition (M) is satisfied and the intersection of two principal ideals of $A$ is a principal ideal;
(d) condition (M) is satisfied and, for every extremal element $p$ of $A$, the ideal $Ap$ is prime;
(e) $A$ is a Krull domain and every prime ideal of height 1 is principal.

We shall denote by K the field of fractions of A and by $\mathcal{P}^*$ (or $\mathcal{P}^*(A)$) the ordered group of non-zero fractional principal ideals of A. The proof will be carried out by proving the following implications:

(a) ⇔ (b) ⇔ (c) ⇔ (d) ⇔ (e)

We show that (a) implies (b); if A is factorial, $\mathcal{P}^*$ is isomorphic to the group of divisors of A and hence to a direct sum of groups $\mathbf{Z}$ ($\S 1$, no. 3, Theorem 2).

Note now that the relation "the intersection of two integral principal ideals of A is a principal ideal" means that every ordered pair of elements of A admits a $lcm$, that is that $\mathcal{P}^*$ is a lattice-ordered group (Algebra, Chapter VI, $\S 1$, no. 9, Proposition 8). The fact that (b) implies (c) (and even is equivalent to it) therefore follows from Algebra, Chapter VI, $\S 1$, no. 13, Theorem 2. The fact that (c) implies (d) follows from Algebra, Chapter VI, $\S 1$, no. 13, Proposition 14 (DIV).

The fact that (d) implies (b) follows from Algebra, Chapter VI, $\S 1$, no. 13, Theorem 2 applied to the group $\mathcal{S}^*$.

We show that (b) implies (e). If (b) holds, there is an isomorphism of $\mathcal{P}^*$ onto $\mathbf{Z}^{(l)}$; let $(v_i(x))_{i \in I}$ denote the element of $\mathbf{Z}^{(l)}$ corresponding to the ideal $Ax$ ($x \in K^*$). It is seen immediately that each $v_i$ is a discrete valuation on K, that A is the intersection of the rings of the $v_i$ and that, for $x \in K^*$, $v_i(x) = 0$ except for a finite number of indices $i$; hence A is a Krull domain. On the other hand, let q be a prime ideal of A of height 1; it contains a non-zero element a which is necessarily not invertible and hence also (by definition of a prime ideal) one of the extremal elements of A; as $Ap$ is prime and non zero, $q = Ap$, which proves that q is principal.

Finally we show that (e) implies (a). Let a be a divisorial ideal of A. There exist prime ideals $p_i$ of A of height 1 such that $\operatorname{div} a = \sum_i n_i \operatorname{div} p_i$ where $n_i \in \mathbf{Z}$. If (e) holds, $p_i$ is of the form $Ap_i$, whence $\operatorname{div} a = \operatorname{div} \left( \prod_i Ap_i^{n_i} \right)$ and hence $a = \prod_i Ap_i^{n_i}$ since a is divisorial.

#### Proposition 1 {#ac-vii-s3-prop-1 .statement}

*Let A be a Krull domain. If every divisorial ideal of A is invertible, then, for every maximal ideal m of A, $A_m$ is factorial. The converse is true if it is also assumed that every divisorial ideal of A is finitely generated (in particular if A is Noetherian).*

Suppose that every divisorial ideal of $A$ is invertible; as $A_{,,}$ is a Krull domain ($\S 1$, no. 4, Proposition 6), every divisorial ideal $a$ of $A_{,,}$ is the intersection of two principal fractional ideals ($\S 1$, no. 5, Corollary 2 to Proposition 9); hence $a = bA_m$, where $b$ is a divisorial ideal of $A$ (Chapter II, $\S 2$, no. 4); as $b$ is invertible by hypothesis, we deduce from Chapter II, $\S 5$, no. 6, Theorem 4 that $a$ is principal and hence $A_{,,}$ is a factorial domain (no. 1, Definition 1). Conversely, if all the $A_{,,}$ are factorial and $c$ is a finitely generated divisorial ideal of $A$, $cA_m$ is a divisorial ideal of $A_{,,}$, as follows from $\S 1$, no. 5, Corollary 2 to Proposition 9 and Chapter II, $\S 2$, no. 4; by hypothesis $cA_m$ is principal and hence it follows from Chapter 11, $\S 5$, no. 6, Theorem 4 that $c$ is invertible.

### 3. DECOMPOSITION INTO EXTREMAL ELEMENTS

Let $A$ be an integral domain, $K$ its field of fractions and $U$ the multiplicative group of invertible elements of $A$. Recall (Algebra, Chapter VI, $\S 1$, no. 5) that there is a canonical isomorphism of $K^*/U$ onto the group $\mathcal{P}^*$ of non-zero fractional principal ideals of $A$. Condition (b) of Theorem 1 may then be translated as follows:

#### Proposition 2 {#ac-vii-s3-prop-2 .statement}

*Let $A$ be an integral domain. For $A$ to be factorial, it is necessary and sufficient that there exist a subset $P$ of $A$ such that every $a \in A - \{0\}$ may be written uniquely in the form $a = u \prod_{p \in P} p^{n(p)}$, where $u \in U$ and the $n(p)$ are positive integers which are zero except for a finite number of them.*

If $P$ satisfies this condition, clearly all its elements are *extremal* and every extremal element of $A$ is associated with a unique element of $P$. Recall that $P$ is then called a *representative system of extremal elements* of $A$ (Algebra, Chapter VII, $\S 1$, no. 3, Definition 2).

Suppose always that $A$ is factorial. It has been seen (no. 2, Theorem 1) that the group $\mathcal{P}^*$ is a lattice. We may therefore apply the results of Algebra, Chapter VI, $\S 1$, nos. 9 and 13. In particular, every element of $K^*$ may be written in an essentially unique way in the form of an *irreducible fraction*. Any two elements $a, b$ of $K^*$ have a g.c.d. and a l.c.m.; if $a = u \prod_{p \in P} p^{n(p)}$ and
$$
b = u' \prod_{p \in P} p^{m(p)}
$$
are decompositions of $a$ and $b$ as products of extremal elements, then:
$$
\text{(1)} \quad \text{g.c.d.}(a, b) = w \prod_{p \in P} p^{\inf(m(p), n(p))}
$$
$$
\text{(2)} \quad \text{l.c.m.}(a, b) = w' \prod_{p \in P} p^{\sup(m(p), n(p))}
$$

where $w, w'$ are in U. We recover, in particular, the results of Algebra, Chapter VIII, § 1, no. 3.

For all $p \in P$, the mapping $a \mapsto n(p)$ is a discrete valuation $v_p$ on K whose ring is obviously $A_{A_p}$. It follows from Theorem 1(e) that the $v_p$ are just the essential valuations of A and that the ideals $Ap$ ($p \in P$) are just the prime ideals of A of height 1.

### 4. RINGS OF FRACTIONS OF A FACTORIAL DOMAIN

#### Proposition 3 {#ac-vii-s3-prop-3 .statement}

*Let A be a Krull domain and S a multiplicative subset of A not containing 0.*

(i) *If A is factorial, $S^{-1}A$ is factorial.*
(ii) *If S is generated by a family of elements $p_i$ such that the principal ideals $Ap_i$ are prime and $S^{-1}A$ is factorial, then A is factorial.*

This follows immediately from Definition 1 of no. 1 and § 1, no. 10, Proposition 17.

### 5. POLYNOMIAL RINGS OVER A FACTORIAL DOMAIN

Let A be a factorial domain, K its field of fractions and $f$ a non-zero element of $K[X]$; an element c of $K^*$ will be called a *content* of $f$ if it is a g.c.d. of the coefficients off. Let $\nu$ be a valuation on K which is essential for A and $\bar{\nu}$ its canonical extension to $K[X]$ (defined by $\bar{\nu}\left(\sum a_i X^i\right) = \inf \nu(a_i)$; cf. Chapter VI, § 10, no. 1, Proposition 2); then $\bar{\nu}(f) = \nu(c)$.

#### Lemma 1 (Gauss) {#ac-vii-s3-lem-1 .statement}

*Let $f, f'$ be non-zero elements of $K[X]$ and c, $c'$ contents off, $f', f'$. Then $cc'$ is a content of $ff'$.*

Let d be a content of $ff'$. For every valuation $\nu$ on K which is essential for A, let $\bar{\nu}$ denote its canonical extension to $K[X]$. Then
$$
\nu(d) = \bar{\nu}(ff') = \bar{\nu}(f) + \bar{\nu}(f') = \nu(c) + \nu(c') = \nu(cc').
$$
Hence $cc'd^{-1}$ is an invertible element of A.

#### Theorem 2 {#ac-vii-s3-thm-2 .statement}

*Let A be a factorial domain, K its field of fractions, $(p_\lambda)$ a representative system of extremal elements of A and $(P_\lambda)$ a representative system of irreducible polynomials of $K[X]$, each $P_\lambda$ having 1 as a content. Then:*
(i) *A[X] is a factorial domain;*
(ii) *the set of $p_\lambda$ and $P_\lambda$ is a representative system of extremal elements of A[X].*

Let $f$ be a non-zero element of $A[X]$. In the ring $K[X]$ $f$ can be decomposed uniquely in the form:
$$
f = a \prod_\lambda P_\lambda^{n(\lambda)} \quad (a \in K^*, n(\lambda) \geq 0).
$$

Lemma 1 proves that $a$ is a content off. Hence $a \in A$. As $A$ is factorial, $a$ can be decomposed uniquely in the form:

$$
a = u \prod p_i^{m(i)} \quad (u \text{ invertible in } A,\ m(i) \geqslant 0).
$$

Whence the existence and uniqueness of the decomposition:

$$
f = u \prod p_i^{m(i)} \bigcap_{\lambda} p_{\lambda}^{n(\lambda)}.
$$

Note that this theorem proves that every element of $A$ admits the *same* decomposition into extremal elements in $A$ and $A[X]$. The g.c.d. of a family of elements of $A$ is therefore the same in $A$ and in $A[X]$.

We may also use Proposition 18 of § 1, no. 10 to show that $A[X]$ *is* a factorial domain if and only if $A$ is a factorial domain.

#### Corollary {#ac-vii-s3-n5-cor-1 .statement}

*If $A$ is a factorial domain, the domain $A[X_1, \ldots, X_n]$ is factorial.*

Argue by induction on $n$.

This corollary may be extended to the case of an infinite family of indeterminates (cf. Exercise 2).

### 6. FACTORIAL DOMAINS AND ZARISKI RINGS

#### Proposition 4 {#ac-vii-s3-prop-4 .statement}

*Let $A$ be a Zariski ring and $\hat{A}$ its completion. If $\hat{A}$ is a factorial domain, $A$ is a factorial domain.*

This follows from no. 1, Definition 1 and § 1, no. 10, Proposition 16.

#### Corollary {#ac-vii-s3-n6-cor-1 .statement}

*If the completion of a Noetherian local ring $A$ is a factorial domain, $A$ is a factorial domain.*

### 7. PRELIMINARIES ON AUTOMORPHISMS OF RINGS OF FORMAL POWER SERIES

#### Lemma 2 {#ac-vii-s3-lem-2 .statement}

*Let $f(X_1, X_2, \ldots, X_n)$ be a formal power series $\neq 0$ with coefficients in a ring $E$. There exist integers $u(i) \geqslant 1$ ($1 \leqslant i \leqslant n - 1$) such that*

$$
f(T^{u(1)}, \ldots, T^{u(n-1)}, T) \neq 0.
$$

Suppose that integers $u(i) \geqslant 1$ ($1 \leqslant i \leqslant k - 1$) are determined such that $f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_k, \ldots, X_n) \neq 0$. We shall determine an integer $u(k) \geqslant 1$ such that

$$
f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_n^{u(k)}, X_{k+1}, \ldots, X_n) \neq 0.
$$

The lemma will then be proved by induction.

Observe that the series $f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_k, \ldots, X)$ can be considered as a series in $X_k$ and $X_n$ with coefficients in $E[[X_{k+1}, \ldots, X_{n-1}]]$. Thus we see that it suffices to establish the lemma for $n = 2$.

Therefore let
$$
f = \sum_{i,j} e_{ij} X^i Y^j \in E[[X, Y]]
$$
where $f \neq 0$. Let $G \subset \mathbf{N} \times \mathbf{N}$ be the non-empty set of ordered pairs $(i, j)$ such that $e_{ij} \neq 0$. Let $\mathbf{N} \times \mathbf{N}$ be given the lexicographical ordering. Let $(c, d)$ be the least element of $G$. Choose an integer $p > d$. In the expansion of
$$
f(T^p, T) = \sum_{(i, j) \in G} e_{ij} T^{ip + j}
$$
we look for the terms of degree $cp + d$. If $ip + j = cp + d, i \geq c + 1$ is impossible, for this would give
$$
ip + j \geq (c + 1)p + j \geq (c + 1)p > cp + d;
$$
nor is $i < c$ possible, for $(c, d)$ is the least element of $G$; therefore $i = c$ and then $j = d$. The term of degree $cp + d$ in $f(T^p, T)$ is therefore $e_{cd} T^{cp + d}$. Since $e_{cd} \neq 0, f(T^p, T) \neq 0$. Whence the lemma.

In the ring $E[[X_1, \ldots, X]]$, let $a$ be the ideal of formal power series without constant term. If $w_1, \ldots, w_n$ are elements of $a$, recall that the mapping $f(X_1, \ldots, X,) \mapsto f(w_1, \ldots, w,)$ is the unique endomorphism $s$ of the ring $E[[X_1, \ldots, X_n]]$ such that $s(X_i) = w_i$ for $1 \leq i \leq n$ (Chapter III, § 4, no. 5, Proposition 6).

We take $w_1 = X_1 + X_n^{u(1)}, \ldots, w_{n-1} = X_{n-1} + X_n^{u(n-1)}, w_n = X_n$, where the $u(i)$ are integers $\geq 1$. Let $s'$ be the endomorphism of $E[[X_1, \ldots, X_n]]$ which maps $X_1$ to $X_1 - X_n^{u(1)}, \ldots, X_{n-1}$ to $X_{n-1} - X_n^{u(n-1)}$ and $X_n$ to $X_n$. Then $s'(s(X_i)) = X_i$ for $1 \leq i \leq n$ and hence $s' \circ s$ is the identity automorphism; similarly for $s \circ s'$. Hence $s$ is an *automorphism*.

#### Lemma 3 {#ac-vii-s3-lem-3 .statement}

*Let $f$ be a non-zero element of $E[[X_1, \ldots, X_n]]$. There exist integers $u(i) \geq 1 (1 \leq i \leq n-1)$ such that the automorphism $s$ of $E$ defined by*
$$
s(X_i) = X_i + X_n^{u(i)} \quad (1 \leq i \leq n-1)
$$
*and $s(X_n) = X_n$, maps $f$ to an element $g$ such that $g(0, \ldots, 0, X,) \neq 0$.*

$g(0, \ldots, 0, X,) = f(X_n^{u(1)}, \ldots, X_n^{u(n-1)}, X,)$. Lemma 3 is therefore a consequence of Lemma 2.

### 8. THE PREPARATION THEOREM

In this no. A will denote a *local* ring, $m$ its maximal ideal and $k = A/m$ its residue field. Suppose that A is *Hausdorff and complete* with the $m$-adic topology. Let $B = A[[X]]$; it is local ring whose maximal ideal $\mathfrak{n}$ is generated by $m$ and $X$; with the $\mathfrak{A}$-adic topology, B is Hausdorff and complete (Chapter III, § 2, no. 6, Proposition 6).

For every formal power series
$$
f = \sum_{i=0}^{\infty} a_i X^i \in B,
$$
we write
$$
\tilde{f} = \sum_{i=0}^{\infty} \bar{a}_i X^i \in k[[X]],
$$
where $\bar{a}_i$ denotes the canonical image of $a_i$ in $k$. The series $\tilde{f}$ will be called the *reduced series* off; if $\tilde{f} \neq 0$, the order of $\tilde{f}$ (that is the least integer $s$ such that $a_s \notin m$) will be called the *reduced order* off.

#### Proposition 5 {#ac-vii-s3-prop-5 .statement}

*Let $f \in B$ be a series whose reduced series is non-zero. Let $s$ denote its reduced order and $M$ the sub-A-module of $B$ with basis $\{1, X, \ldots, X^{s-1}\}$. Then $B$ is the direct sum of $M$ and $f$ is not a divisor of zero in $B$.*

(a) We show that $f \mid B \cap M = (0)$. Suppose that there is a relation:
$$
\left( \sum_{i=0}^{\infty} b_i X^i \right) f = r_0 + r_1 X + \cdots + r_{s-1} X^{s-1} \qquad (b_i \in A, r_j \in A).
$$
We show that the $b_i$ (and hence the $r_j$) are all zero, which will prove in particular that $f$ is not a divisor of zero in $B$. Since $A$ is Hausdorff, it suffices to show that $b_i \in m^n$ for all $i \geq 0$ and all $n \geq 0$. It is obvious for $n = 0$. We shall argue by double induction: we shall assume that $b_i \in m^{n-1}$ for all $i$ and $b_i \in m^n$ for $i < k$ and show that this implies that $b_k \in m^n$. For this, we write $f = \sum_{i=1}^{\infty} a_i X^i$ and compare the coefficients of $X^{s+k}$ in (3); then:
$$
(b_0 a_{s+k} + \cdots + b_{k-1} a_{s+1}) + b_k a_s + (b_{k+1} a_{s-1} + \cdots + b_{k+s} a_0) = 0.
$$
The terms in the first bracket belong to $m^n$ since the $b_i \in m^n$ for $i < k$; similarly for those in the second, since the $b_i \in m^{n-1}$ for all $i$ and the $a_i \in m$ for $i \leq s-1$. Hence $b_k a_s \in m^n$ and, as $a_s$ is an invertible element of $A$, $b_k \in m^n$.

(b) We show that $f \mid B + M = B$. We write
$$
g = a_s + a_{s+1} X + a_{s+2} X^2 + \cdots;
$$
it is an invertible element of $B$. Then
$$
f - X^s g = a_0 + a_1 X + \cdots + a_{s-1} X^{s-1};
$$
if therefore we write $fg^{-1} - X^s = (f - X^s g) g^{-1} = -h$, the coefficients of $h$ belong to $m$. Then let $r$ be an element of $B$. By induction on $n$ we define a sequence $(q^{(n)})$ of elements of B: we take $q^{(0)}$ to be the unique series satisfying:
$$
r \equiv X^s q^{(0)} \pmod{M};
$$
writing $h = \sum_{i=0}^m h_i X^i$ and $q^{(n)} = \sum_{i=0}^\infty q_i^{(n)} X^i$, the $q_i^{(n)}$ are defined by:
$$
q_i^{(n)} = \sum_{j=0}^{i+s} h_j q_{i+s-j}^{(n-1)}
$$
It follows immediately from (6) that:
$$
X^s q^{(n)} \equiv h q^{(n-1)} \pmod{M}.
$$
As $h_j \in m$ for all $j$, it also follows from (6), by induction on $n$, that $q_i^{(n)} \in m^n$ for all $i$ and all $n$. As A is complete, it follows that the series
$$
q^{(0)} + q^{(1)} + \ldots + q^{(n)} + \ldots
$$
converges to an element $q$ of B. By (5) and (7),
$$
X^s(q^{(0)} + q^{(1)} + \ldots + q^{(n)}) \equiv r + h(q^{(0)} + \ldots + q^{(n-1)}) \pmod{M}.
$$
As M is closed, at the limit (8) gives $r \equiv (X^s - h)q \pmod{M}$, that is
$$
r \in fg^{-1}q + M \subset fB + M.
$$
We may also use the results of Chapter III, § 2 to show the relation $B = fB + M$ (cf. Exercise 12). The method followed here has the advantage of being applicable to convergent series.

#### Corollary {#ac-vii-s3-n8-cor-1 .statement}

*With the hypotheses and notation of Proposition 5, suppose that $s \geq 1$, so that $f \in Bm + BX$. Then the A-homomorphism $h$ of $B' = A[[T]]$ to $B = A[[X]]$ such that $h(T) = f$ (Chapter III, § 2, no. 9, Proposition 11 (a)) defines on B a free $B'$-module structure admitting $\{1, X, \ldots, X^{s-1}\}$ as basis. In particular $h$ is injective.*

Let the $B'$-module B be given the (T)-adic filtration, which consists of the $f^n B$ for $n \geq 0$ (Chapter 111, § 2, no. 1). Then $B/fB$ is a free module over the ring $A = B'/TB'$ and the images of the $X^i$ ($0 \leq i \leq s-1$) in this A-module form a basis of it (Proposition 5); as moreover $f$ is not a divisor of zero in B (Proposition 5), $Bf^n/Bf^{n+1}$ is also a free $(B'/TB')$-module of rank s, so that condition (GR) of Chapter 111, § 2, no. 8 is satisfied (replacing A by B' and M by B). On the other hand, since B' is Hausdorff and complete with respect to the (T)-adic filtration and gr(B) is a finitely generated gr(B')-module by the above, it is seen first (Chapter III, § 2, no. 9, Corollary 1 to Proposition 12) that B is a finitely generated B' module. The first assertion of the corollary then follows from Chapter III, § 2, no. 9, Proposition 13. The second follows immediately from it.

#### Definition 2 {#ac-vii-s3-def-2 .statement}

*A polynomial* $F \in \mathbf{A}[X]$ *is called distinguished if it is of the form*
$$
F = X^s + a_{s-1} X^{s-1} + \cdots + a_0,
$$
*where* $a_i \in \mathfrak{m}$ *for* $0 \leq i \leq s - 1$.

Note that the product of two distinguished polynomials is a distinguished polynomial.

#### Proposition 6 (Preparation Theorem) {#ac-vii-s3-prop-6 .statement}

*Let* $f \in B$ *be a series whose reduced series is not zero and* $s$ *its reduced order. Then there exists a unique ordered pair* $(u, F)$ *such that* $u$ *is an invertible element of* $B$, $F$ *a distinguished polynomial of degree* $s$ *and* $f = uF$.

We write $F = X^s + G$, where $G = g_0 + \cdots g_{s-1} X^{s-1}$ ($g_i \in \mathbf{A}$). The relation $f = uF$ is equivalent to $F = u^{-1}f$, that is to $X^s = u^{-1}f - G$. Hence Proposition 5 shows the uniqueness of $G$ and $u^{-1}$ and therefore of $F$ and $u$. It also shows that there exist $v \in B$ and a polynomial $G = g_0 + \cdots + g_{s-1} X^{s-1}$ ($g_i \in \mathbf{A}$) such that $X^s = v - G$; it remains to show that $v$ is invertible in $B$ and that $g_i \in \mathfrak{m}$ for all $i$. Now, writing $\bar{g}_i$ for the canonical image of $g_i$ in $k$ and $\bar{f}, \bar{v}$ for the reduced series of $f, g$,
$$
X^s + \bar{g}_0 + \bar{g}_1 X + \cdots + \bar{g}_{s-1} X^{s-1} = \bar{f} \bar{v};
$$
since $\bar{f}$ is of order $s$, $\bar{g}_i = 0$ for all $i$ and $\bar{v}$ is of order 0, hence $v$ is invertible.

#### Proposition 7 {#ac-vii-s3-prop-7 .statement}

*Let* $F$ *be a distinguished polynomial and* $g, h$ *two formal power series of* $B$ *such that* $F = gh$. *Then there exists an invertible element* $u$ *of* $B$ *such that* $ug$ *and* $u^{-1}h$ *are distinguished polynomials and* $F = (ug)(u^{-1}h)$.

In fact, the reduced series of $g$ and $h$ are $\neq 0$; hence, by Proposition 6, there exist invertible elements $u, v$ of $B$ such that $ug$ and $vh$ are distinguished polynomials. Then $uvF = (ug)(vh)$ is a distinguished polynomial and $uv$ is invertible. Passing to the reduced series, it is seen immediately that $F$ and $uvF$ have the same reduced order, that is the same degree. The uniqueness assertion in Proposition 6 therefore shows that $F = uvF$, whence $uv = 1$.

#### Corollary {#ac-vii-s3-n8-cor-2 .statement}

*Suppose further that* $\mathbf{A}$ *is an integral domain and* $F$ *a distinguished polynomial of degree* $s$. *For* $F$ *to be extremal in* $\mathbf{A}[X]$, *it is necessary and sufficient that it be extremal in* $B = \mathbf{A}[[X]]$.

Suppose that $F$ is not extremal in $\mathbf{A}[X]$, so that $F = f_1 f_2$, where $f_1$ and $f_2$ are non-invertible elements of $\mathbf{A}[X]$; the product of the dominant coefficients of $f_1$ and $f_2$ being equal to 1, these coefficients are invertible in $\mathbf{A}$ and the hypothesis implies that $f_1$ and $f_2$ are of degrees $> 0$ and $< s$; as the reduced polynomials $\bar{f}_1, \bar{f}_2$ satisfy $\bar{f}_1 \bar{f}_2 = X^s$, neither $\bar{f}_1$ nor $\bar{f}_2$ can be invertible in $k[[X]]$, for, if $\bar{f}_1$ were invertible, $\bar{f}_2$ would be of order $s$, which is absurd. *A fortiori*, neither $f_1$ nor $f_2$ is invertible in $B$ and $F$ is not extremal in $B$.

Conversely, if F is not extremal in $A[[X]]$, then $F = gh$, where neither g nor his invertible in B; their reduced orders are therefore $\geq 1$; then the distinguished polynomials $ug$ and $u^{-1}h$ of Proposition 7 are not constant, which shows that F is not extremal in $A[X]$.

### 9. FACTORIALITY OF RINGS OF FORMAL POWER SERIES

#### Proposition 8 {#ac-vii-s3-prop-8 .statement}

Let C be a ring which is either a field or a discrete valuation ring. Then the domain of formal power series $C[[X_1, \ldots, X_n]]$ is factorial.

Let $p$ be the maximal ideal of C and $x$ a generator of $p$ (if C is a field, then $\pi = 0$). Let C be given the $p$-adic topology, which is Hausdorff. As C is a Noetherian local ring, $B = C[[X_1, \ldots, X_n]]$ is a Noetherian local ring and its completion is $\hat{C}[[X_1, \ldots, X_n]]$ (Chapter III, §2, no. 6, Proposition 6). By the Corollary to Proposition 4 (no. 6), it suffices to prove that $\hat{C}[[X_1, \ldots, X_n]]$ is factorial. Now, if C is a field, then $\hat{C} = C$; if C is a discrete valuation ring, the same is true of $\hat{C}$ (Chapter VI, §5, no. 3, Proposition 5). We shall therefore assume in the remainder of the proof that C is complete.

Arguing by induction starting with the trivial case $n = 0$, we shall assume that it has been proved that $A = C[[X_1, \ldots, X_{n-1}]]$ is factorial. We shall identify B with $A[[X_n]]$ and denote by m the maximal ideal of A (generated by $\pi, X_1, \ldots, X_{-1}$). We shall prove that every non-zero element g of B is, in an essentially unique way, a product of extremal elements.

Let K be the field $C/C\pi$; as $B/B\pi$ is identified with $K[[X_1, \ldots, X_n]]$, the ideal $Bx$ is prime and $x$ is extremal. If $x \neq 0$, $B_{B\pi}$ is therefore the ring of a normed discrete valuation w (Chapter VI, §3, no. 6, Proposition 9); every non-zero element g of B may therefore be written as $g = \pi^{w(g)} f$, where $f \in B$ and f is not a multiple of $\pi$. It will therefore suffice to show that $f$ is an essentially unique product of extremal elements. Now the canonical image of $f$ in $K[[X_1, \ldots, X_n]]$ is not zero; Lemma 3 (no. 7) therefore shows that there exists an automorphism of B which maps $f$ to an element $f'$ such that the coefficients of $f'(0, \ldots, 0, X,)$ are not all in $Cx$; this means that the coefficients of the series $f'$, considered as a formal power series in $X,,$ are not all in m. It will suffice to prove our assertion for $f'$.

In what follows, all the elements of B will be considered as formal power series in X, with coefficients in A. By Proposition 6 of no. 8 (applicable since C and therefore A are separable and complete and the reduced series off' is $\neq 0$), $f'$ is associated, in B, with a unique distinguished polynomial F. By Proposition 7 of no. 8, every series which divides $f'$ (or, what amounts to the same, which divides F) is associated with a distinguished polynomial which divides F and every decomposition off' is, to within invertible factors, of the form $f' = u F_1 \cdots F_q$, where $u$ is invertible and the $F_i$ are extremal distinguished polynomials (in B) such that $F = F_1 \cdots F_q$. By the Corollary to Proposition 7 of no. 8, the F, are also extremal in $\mathbf{A}[X_n]$. Now, as $\mathbf{A}$ is factorial by the induction hypothesis, so is $\mathbf{A}[X_n]$ (Theorem 2, no. 5); hence, since they are monic, the $F_i$ are uniquely determined by $F$ (up to a permutation). This shows the uniqueness of the decomposition $f' = u F_1 \ldots F_r$; its existence follows from the fact that $B$ is Noetherian, which completes the proof.

Remarks
(1) There exist factorial rings $\mathbf{A}$ such that the ring $\mathbf{A}[[X]]$ is not factorial (Exercise 8). However, if $\mathbf{A}$ is a principal ideal domain, $\mathbf{A}[[X_1, \ldots, X_n]]$ is factorial (Exercise 9).
(2) \* We shall see later, by homological methods, that every regular local ring is factorial (cf. § 4, no. 7, Corollary 3 to Proposition 16). This will give another proof, conceptually simpler, of Proposition 8. \*
