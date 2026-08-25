---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 2
section_title: Dedekind domains
lang: en
source: ac-i-vii
book_pages: 493-502, 556-571
pdf_pages: 0511-0520, 0574-0589
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF DEDEKIND DOMAINS
      page: 493
      pdf_page: 511
    - "no": 2
      title: CHARACTERIZATIONS OF DEDEKIND DOMAINS
      page: 494
      pdf_page: 512
    - "no": 3
      title: DECOMPOSITION OF IDEALS INTO PRODUCTS OF PRIME IDEALS
      page: 496
      pdf_page: 514
    - "no": 4
      title: THE APPROXIMATION THEOREM FOR DEDEKIND DOMAINS
      page: 497
      pdf_page: 515
    - "no": 5
      title: THE KRULL-AKIZUKI THEOREM
      page: 499
      pdf_page: 517
statements: 14
exercises: 27
content_sha256: cc7d7aebe3c9feefed99d2b6823c6c99ac2960660a90318e1a3fa69f6af4754d
---

## 2. DEDEKIND DOMAINS

### 1. DEFINITION OF DEDEKIND DOMAINS

Let $A$ be an integral domain. Clearly the following conditions are equivalent:
(a) no two of the non-zero prime ideals of $A$ are comparable with respect to inclusion;
(b) the non-zero prime ideals of $A$ are maximal;
(c) the non-zero prime ideals of $A$ are of height 1.

#### Definition 1 {#ac-vii-s2-def-1 .statement}

A Krull domain all of whose non-zero prime ideals are maximal is called a Dedekind domain.

Examples of Dedekind domains
(1) Every principal ideal domain is a Dedekind domain.
(2) Let K be a finite extension of $\mathbf{Q}$ and A the integral closure of $\mathbf{Z}$ in K. The ring A is a Krull domain (\$ 1, no. 8, Proposition 12). Let $\mathfrak{p}$ be a non-zero prime ideal of A. Then $\mathfrak{p} \cap \mathbf{Z}$ is non-zero (Chapter V, \$ 2, no. 1, Corollary to Proposition 1) and hence is a maximal ideal of $\mathbf{Z}$; hence $\mathfrak{p}$ is a maximal ideal of A (*loc. cit.*, Proposition 1). Therefore, A is a Dedekind domain. In general, A is not a principal ideal domain (*Algebra*, Chapter VII, \$ 1, Exercise 12).
(3) \* Let V be an affine algebraic variety and A the ring of functions regular on V. Suppose that A is not a field (i.e. that V is not reduced to a point). For A to be a Dedekind domain, it is necessary and sufficient that V be an irreducible curve with no singular point: for to say that A is an integral domain amounts to saying that V is irreducible; to say that every non-zero prime ideal of A is maximal amounts to saying that A is a curve; finally, as A is Noetherian, to say that it is a Krull domain amounts to saying that it is integrally closed, that is that V is a normal curve, or also that it has no singular point. \*
(4) A ring of fractions $S^{-1}A$ of a Dedekind domain A is a Dedekind domain if $0 \notin S$. For $S^{-1}A$ is a Krull domain (\$ 1, no. 4, Proposition 6) and every non-zero prime ideal of $S^{-1}A$ is maximal by Chapter II, \$ 2, no. 5, Proposition 11.

### 2. CHARACTERIZATIONS OF DEDEKIND DOMAINS

#### Theorem 1 {#ac-vii-s2-thm-1 .statement}

Let A be an integral domain and K its field of fractions. The following conditions are equivalent:
(a) A is a Dedekind domain;
(b) A is a Krull domain and every non-improper valuation on K which is positive on A is equivalent to an essential valuation of A;
(c) A is a Krull domain and every fractional ideal $\mathfrak{J} \neq (0)$ of A is divisorial;
(d) every fractional ideal $3 \neq (0)$ of A is invertible;
(e) A is a Noetherian integrally closed domain and every non-zero prime ideal of A is maximal;
(f) A is Noetherian and, for every maximal ideal m of A, $A_m$ is either a field or a discrete valuation ring;
(g) A is Noetherian and, for every maximal ideal m of A, $A_m$ is a principal ideal domain.

We show first the equivalence of (a) and (b). Corollary 2 to Theorem 3, \$ 1, no. 6, shows immediately that (a) implies (b). Conversely, (b) implies (a), since, for every prime ideal $p$ of $A$, there exists a valuation ring of $K$ which dominates $A_p$ (Chapter VI, § 1, no. 2, Corollary to Theorem 2).

The remainder of the proof is carried out by proving the following implications:

$$
(a) \Rightarrow (c) \Rightarrow (d) \Rightarrow (e) \Rightarrow (f) \Rightarrow (g) \Rightarrow (a).
$$

If $A$ is a Dedekind domain and $b$ is a non-zero fractional ideal, then $bA_p = bA_p$ for every maximal ideal $p$ ($\S 1$, no. 4, Proposition 7) and hence $b = 6$ (Chapter II, $\S 3$, no. 3, Corollary 3 to Theorem 1); thus (a) implies (c).

We now show that (c) implies (d). If (c) holds, the mapping $a \mapsto \operatorname{div} a$ is a bijection of $I(A)$ onto $D(A)$ (cf. $\S 1$, no. 1); as it is a homomorphism ($\S 1$, no. 2) and $D(A)$ is a group, every element of $I(A)$ is invertible.

We show that (d) implies (e). If (d) holds, every integral ideal $\neq (0)$ of $A$ is finitely generated (Chapter 11, $\S 5$, no. 6, Theorem 4) and hence $A$ is Noetherian; as $I(A)$ is a group, $D(A)$ is a group and $A$ is therefore completely integrally closed ($\S 1$, no. 2, Theorem 1). Finally, if $p$ is a non-zero prime ideal of $A$ and $m$ is a maximal ideal of $A$ containing $p$, the ring $A_{m}$ is a principal ideal domain (Chapter II, $\S 5$, no. 6, Theorem 4); as $pA_m$ is prime and non-zero, necessarily $pA_m = mA_m$ (a principal ideal domain being a Dedekind domain) whence $p = m$ (Chapter 11, $\S 2$, no. 5, Proposition 11) and $p$ is maximal.

We now show that (e) implies (f). If $m$ is a maximal ideal of $A$ and (e) holds, $A_{m}$ is an integrally closed Noetherian domain and its maximal ideal $mA_m$ is, either (0), or the only non-zero prime ideal of $A_{m}$; hence $A_{m}$ is a field or a discrete valuation ring by Proposition 11 of $\S 1$, no. 7.

The fact that (f) implies (g) is obvious.

We show finally that (g) implies (a). As $A$ is the intersection of the $A_{m}$, where $m$ runs through the set of maximal ideals (Chapter II, $\S 3$, no. 3, Corollary 4 to Theorem 1), (g) implies that $A$ is integrally closed and Noetherian and hence that $A$ is a Krull domain ($\S 1$, no. 3, Corollary to Theorem 2). On the other hand, it can be shown that every non-zero prime ideal of $A$ is maximal as in the proof that (d) $\Rightarrow$ (e).

#### Proposition 1 {#ac-vii-s2-prop-1 .statement}

*A semi-local Dedekind domain is a principal ideal domain.*

Let $A$ be a semi-local Dedekind domain, $K$ its field of fractions, $p_1, \ldots, p_n$ its maximal ideals and $v_1, \ldots, v$, the corresponding essential valuations; these are the only essential valuations of $A$. Let $a$ be a non-zero integral ideal of $A$. Since it is divisorial, there exists ($\S 1$, no. 4, Proposition 5) integers $q_1, \ldots, q_n$ such that $a$ is the set of $x \in K$ such that $v_i(x) \geq q_i$ for $1 \leq i \leq n$. Let $x_0$ be an element of $K$ such that $v_i(x_0) = q_i$ for $1 \leq i \leq n$ (Chapter VI, $\S 7$, no. 2, Corollary 1 to Theorem 1). Then $a$ is the set of $x \in K$ such that $v_i(xx_0^{-1}) \geq 0$ for $1 \leq i \leq n$. Thus $a = Ax_0$.

If $A$ is a Dedekind domain, it has been seen, in the proof of Theorem 1, that the group D(A) of divisors of A is identified with the group I(A) of fractional ideals $a \neq (0)$ (as A is Noetherian, every non-zero fractional ideal is finitely generated). The divisor class group C(A) of A ($\S 1$, no. 2) is then identified with the group of classes of ideals $\neq 0$ of A (defined in Chapter II, $\S 5$, no. 7).

### 3. DECOMPOSITION OF IDEALS INTO PRODUCTS OF PRIME IDEALS

Let A be a Dedekind domain, I(A) the ordered multiplicative group of non-zero fractional ideals of A and D(A) the group of divisors of A. The isomorphism $a \mapsto \operatorname{div} a$ of I(A) onto D(A) maps the extremal divisors to the non-zero prime ideals of A ($\S 1$, no. 6, Theorem 3) and hence the multiplicative group I(A) admits as basis the set of non-zero prime ideals of A ($\S 1$, no. 3, Theorem 2). In other words, *every non-zero fractional ideal a of A admits a unique decomposition of the form*:

$$
a = \prod_p p^{n(p)}
$$

where the product extends to the non-zero prime ideals of A, the exponents $n(p)$ being zero except for a finite number of them. Further a is integral if and only if the $n(p)$ are all positive. The relation (1) is called the *decomposition of a into prime factors*. In particular, if a is a principal ideal $Ax$, then, for all $p$, $n(p) = v_p(x)$, where $v_p$ denotes the essential valuation corresponding to $p$; this follows from formula (4) of $\S 1$, no. 3. Let

$$
a = \prod_p p^{m(p)}, \quad b = \prod_p p^{n(p)}
$$

be two non-zero fractional ideals of A. Then

$$
ab = \prod_p p^{m(p) + n(p)} \tag{2}
$$
$$
a : b = ab^{-1} = \prod_p p^{m(p) - n(p)} \tag{3}
$$
$$
a + b = \prod_p p^{\inf(m(p), n(p))} \tag{4}
$$
$$
a \cap b = \prod_p p^{\sup(m(p), n(p))} \tag{5}
$$

Relation (2) is obvious; relation (3) follows from it, the equation $a : b = ab^{-1}$ following from the equation

$$
\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b
$$

($\S 1$, no. 2, Corollary to Theorem 1); formulae (4) and (5) follow from Proposition 2, $\S 1$, no. 1.

These results apply in particular to the integral closure of $\mathbf{Z}$ in a finite extension of $\mathbf{Q}$.

If $A$ is a principal ideal domain, the above results again give those of Algebra, Chapter VII, § 1, no. 3.

### 4. THE APPROXIMATION THEOREM FOR DEDEKIND DOMAINS

In Dedekind domains there is an "approximation theorem" which strengthens both Theorem 1 of Chapter VI, § 7, no. 2 and Proposition 9 of § 1, no. 5:

#### Proposition 2 {#ac-vii-s2-prop-2 .statement}

Let $A$ be a Dedekind domain, $K$ its field of fractions and $P$ the set of non-zero prime ideals of $A$; for $p \in P$ let $v_p$ denote the corresponding essential valuation of $A$. Let $p_1, \ldots, p_q$ be distinct elements of $P$ and $n_1, \ldots, n_q$ rational integers and $x_1, \ldots, x_q$ elements of $K$. Then there exists $x \in K$ such that $v_{p_i}(x - x_i) \geq n_i$ for $1 \leq i \leq q$ and $v_p(x) \geq 0$ for all $p \in P$ distinct from the $p_i$.

Replacing if need be the $n_i$ by greater integers, they may be assumed all to be positive. We examine first the case where the $x_i$ are in $A$; it obviously amounts to finding an $x \in A$ satisfying the congruences

$$
x \equiv x_i \pmod{p_i^{n_i}}
$$

and the existence of $x$ then follows from Chapter II, § 1, no. 2, Proposition 5.

We pass now to the general case. We may write $x_i = s^{-1} y_i$ where $s, y_i$ are in $A$; writing $x = s^{-1} y$, it amounts to finding a $y \in A$ such that, on the one hand, $v_{p_i}(y - y_i) \geq n_i + v_{p_i}(s)$ and, on the other, $v_p(y) \geq v_p(s)$ for all $p \in P$ distinct from the $p_i$; as $v_p(s) = 0$ except for a finite number of indices $p$, it is thus reduced to the above case; whence the proposition.

Proposition 2 may be interpreted as a density theorem. To be precise, for all $p \in P$, let $\hat{K}_p$ (resp. $\hat{A}_p$) be the completion of $K$ (resp. $A$) with respect to the discrete valuation $v_p$ and consider the product $\prod_{p \in P} \hat{K}_p$; an element $x = (x_p)$ of this product is called a restricted adèle of $A$ if $x_p \in \hat{A}_p$ for all $p \in P$ with the exception of a finite number of them. Clearly the set $A$ of restricted adtles is a subring of $\prod_{p \in P} \hat{K}_p$, which contains the product ring $A, = \prod_{p \in P} \hat{A}_p$. Consider on $A$, the product topology, with respect to which $A,$ is complete; there is on $A$ a unique topology $\mathcal{T}$ which is compatible with its additive group structure and for which the neighbourhoods of 0 in $A$, form a fundamental system $\mathcal{G}$ of neighbourhoods of 0. The topology $\mathcal{T}$ is compatible with the ring structure on $A$; for clearly axiom (AVII) of General Topology, Chapter 111, § 6, no. 3, holds, the topology induced by $\mathcal{T}$ on $A,$ being compatible with the ring structure on $A,$. On the other hand, for all $x \in A$ there exists a finite subset $J$ of $P$ such that, if we write $J' = P - J, \ K_J \leq \prod_{p \in J} \hat{K}_p, \ A_{J'} = \prod_{p \in J'} \hat{A}_p,$ then x \in K_J \times A_{J'} and, as $\hat{A}_p$ is open in $\hat{K}_p$ for all p, $\mathcal{G}$ is a fundamental system of neighbourhoods of 0 for the product topology on $K_J \times A_{J'}$; since the latter is compatible with the ring structure on this product, axiom (AV_1) of *General Topology*, Chapter III, *loc. cit.* is also seen to hold, which proves our assertion. Clearly A, is an *open* subring of A and hence A is also a *complete* ring (*General Topology*, Chapter III, § 3, no. 3, Proposition 4).

For all $x \in K$, let $\Delta(x)$ be the element $(x_p) \in \prod_{p \in P} \hat{K}_p$ such that $x_p = x$ for all $p \in P$; as $x_p \in \hat{A}_p$ except for a finite number of values of p, $\Delta(x) \in A$; hence we have thus defined a homomorphism $A : K \to A$ which is *injective* if $P \neq \varnothing$ (that is if A is not a field); the elements of $\Delta(K)$ are called *principal restricted adèles* and clearly $\Delta(A) \subset A$.

#### Proposition 3 {#ac-vii-s2-prop-3 .statement}

*The ring A, (resp. A ) is identified with the completion of A (resp. K) with respect to the ring topology for which a fundamental system of neighbourhoods & 0 consists & all the integral ideals $\neq (0)$ of A.*

It is immediate that the topology considered on A (or K) is Hausdorff. Taking account of no. 3, the assertion concerning A, follows from Chapter 111, § 2, no. 13, Proposition 17. This shows therefore that $\Delta(A)$ is dense in A,; to see similarly that $\Delta(K)$ is dense in A, note that for all $x = (x_i) \in A$ there is only a finite number of $p \in P$ such that $v_p(x_p) < 0$; by § 1, no. 5, Proposition 9 there is therefore an $s \in K$ such that $sx_p \in \hat{A}_p$ for all $p \in P$, in other words $\Delta(s)x \in A$, and, as multiplication by $\Delta(s)$ is a homomorphism from A to itself, it suffices to apply the fact that $\Delta(A)$ is dense in A , to deduce that $\Delta(K)$ is dense in A.

We could of course also prove that $\Delta(K)$ is dense in A by using Proposition 2.

Consider now the multiplicative group $\mathbf{SL}(n, A)$ consisting of the matrices $U \in \mathbf{M}_n(A)$ such that $\det(U) = 1$; if $\mathbf{M}_n(A) = A^{n^2}$ is given the product topology, it induces on $\mathbf{SL}(n, A)$ a topology *compatible with the group structure* on $\mathbf{SL}(n, A)$. It suffices to verify that the mapping $U \mapsto U^{-1}$ is continuous on $\mathbf{SL}(n, A)$; but as U is unimodular, it is known (*Algebra*, Chapter III, § 6, no. 5, formula (17)) that the elements of $U^{-1}$ are *minors* of U and hence polynomials in the elements of U, which proves our assertion. If K is identified with a subring of A by means of A, the group $\mathbf{SL}(n, K)$ is a subgroup of $\mathbf{SL}(n, A)$.

#### Proposition 4 {#ac-vii-s2-prop-4 .statement}

*The group $\mathbf{SL}(n, K)$ is dense in $\mathbf{SL}(n, A)$.*

Let G be the closure of $\mathbf{SL}(n, K)$ in $\mathbf{SL}(n, A)$; as K is dense in A (Proposition 3), G contains all the matrices of the form $I + a . E_{ij}$ for $i \neq j$ and $a \in A$. For all $p \in P$ and all $\lambda \in \hat{K}_p$, let $\lambda(p)$ be the restricted adèle $x = (x_q)_{q \in P}$ such that $x_p = \lambda$ and $x_q = 0$ for $q \neq p$; the above shows that G contains the matrices $I + \lambda(p)E_{ij}$ for $i \neq j$. But we know that the matrices of the form $I + \lambda E_{ij}$ for $\lambda \in \hat{K}_p$ generate the group $\mathbf{SL}(n, \hat{K}_p)$ (*Algebra*, Chapter 111). For every matrix $U \in \mathbf{SL}(n, A)$ let $U_p$ denote the canonical image of $U$ in $\mathbf{SL}(n, \hat{\mathbf{K}}_p)$; it is therefore seen that, for all $p \in P$, $G$ contains the matrices $U \in \mathbf{SL}(n, A)$ such that $U_q = I$ for all $q \# p$. Since $G$ is a group, it also contains all the matrices $U \in \mathbf{SL}(n, A)$ such that $U_p = I$ except for a *finite* number of $p \in P$; now, the definition of the topology on $A$ shows immediately that the set of these matrices is dense in $\mathbf{SL}(n, A)$.

### 5. THE KRULL-AKIZUKI THEOREM

#### Lemma 1 {#ac-vii-s2-lem-1 .statement}

*Let $A$ be a Noetherian domain in which every non-zeroprime ideal is maximal and $M$ afinitely generated torsion $A$-module. Then the length $\operatorname{long}_A(M)$ of $M$ is infinite.*

As $M$ is a torsion module, every prime ideal associated with $M$ is $\neq (0)$ and therefore maximal. The lemma then follows from Chapter IV, § 2, no. 5, Proposition 7.

#### Lemma 2 {#ac-vii-s2-lem-2 .statement}

*Let $A$ be a ring, $T$ an $A$-module and $(T_i)$ a right directed family of submodules of $T$ with union $T$. Then $\operatorname{long}_A(T) = \sup_i (\operatorname{long}_A(T_i))$.*

$\operatorname{long}_A(T_i) \leq \operatorname{long}_A(T)$ for all $i$. The lemma is obvious if no integer exceeds the $\operatorname{long}_A(T_i)$, both sides then being infinite. Otherwise, let $i_0$ be an index for which $\operatorname{long}_A(T_{i_0})$ takes its greatest value; then $T_{i_0} = T$ since the family $(T_i)$ is directed; whence our assertion in this case.

#### Remark {#ac-vii-s2-n5-rem-1 .statement}

This proof does not assume that $A$ is commutative.

#### Lemma 3 {#ac-vii-s2-lem-3 .statement}

*Let $A$ be a Noetherian domain such that every non-zero prime ideal $\& A$ is maximal, $M$ a torsion-free $A$-module of finite rank $r$ and a non-zero element of $A$. Then $A/Aa$ is an $A$-module of finite length and:*
$$
\operatorname{long}_A(M/aM) \leq r \cdot \operatorname{long}_A(A/Aa).
$$
Lemma 1 shows that $\operatorname{long}_A(A/Aa)$ is finite. We show (6) first in the case where $M$ is *finitely generated*. As $M$ is torsion-free and of rank $r$, there exists a submodule $L$ of $M$ which is isomorphic to $A'$ and such that $Q = M/L$ is a finitely generated torsion $A$-module and hence of finite length (Lemma 1). For every integer $n \geq 1$, the kernel of the canonical surjection $M/a^nM \to Q/a^nQ$ is equal to $(L + a^nM)/a^nM$ and isomorphic to $L/(a^nM \cap L)$; as
$$
a^nL \subset a^nM \cap L,
$$
therefore
$$
\operatorname{long}_A(M/a^nM) \leq \\
\operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q/a^nQ) \leq \operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q).
$$
Now, since $M$ is torsion-free, multiplication by $a$ defines an isomorphism of

M/aM onto aA/a^2M; similarly for L; whence, by induction on n, the formulae:

$$
\text{long}_A(M/a^nM) = n \cdot \text{long}_A(M/aM).
$$
$$
\text{long}_A(L/a^nL) = n \cdot \text{long}_A(L/aL).
$$

Taking account of (7) we deduce:

$$
\text{long}_A(M/aM) \leq \text{long}_A(L/aL) + n^{-1}\text{long}_A(Q)
$$

for all $n > 0$; as L is isomorphic to A', $\text{long}_A(L/aL) = r \text{long}_A(A/Aa)$; whence (6) by letting $n$ tend to infinity in (9).

We now pass to the general case. Let $(M_i)$ be the family of finitely generated submodules of M. The module $T = M/aM$ is the union of the submodules $T_i = (M_i + aM)/aM = M_i/(M_i \cap aM)$. Now, T, is isomorphic to a quotient of $M_i/aM_i$ and hence

$$
\text{long}_A(T_i) \leq r \text{long}_A(A/Aa)
$$

by what we have just proved. Whence

$$
\text{long}_A(T) \leq r \text{long}_A(A/Aa)
$$

by Lemma 2.

Proposition 5 (Krull-Akizuki). *Let A be a Noetherian domain each of whose non-zeroprime ideals is maximal, K its field of fractions, L a finite extension of K and B a subring of L containing A. Then B is Noetherian and every non-zero prime ideal of B is maximal. Moreover, for every ideal $b \neq (0)$ of B, B/b is a finitely generated A-module.*

Let b be a non-zero ideal of B. We shall show that B/b is an A-module of finite length (hence, *a fortiori*, a B-module of finite length) and that b is a finitely generated B-module.

A non-zero element y of b satisfies an equation of the form:

$$
a_r y^r + a_{r-1} y^{r-1} + \cdots + a_1 = 0 \quad (a_i \in A, a_1 \neq 0).
$$

This equation shows that $a_1 \in By \subset b$. Applying Lemma 3 to $M = B$, it is seen that $B/a_0B$ is an A-module of finite length; so is B/b which is a quotient module of it. Further the B-module b contains, as a submodule, $a_0B$ which is finitely generated; as $b/a_0B$ is of finite length (as a submodule of $B/a_0B$) and hence finitely generated, b is certainly a finitely generated B-module.

The above shows first that B is Noetherian. On the other hand, if $p$ is a non-zero prime ideal of B, the ring $B/p$ is an integral domain and of finite length and hence is a field (*Algebra*, Chapter VIII, § 6, no. 4, Proposition 9), so that $p$ is maximal.

#### Corollary 1 {#ac-vii-s2-lem-3-cor-1 .statement}

*For every prime ideal p of A, the set of prime ideals of B lying above p is finite.*

Suppose first that $p = (0)$; then the only prime ideal $q$ of $B$ such that $q \cap A = (0)$ is $(0)$; otherwise, writing $S = A - \{0\}, S^{-1}q$ would be a non-zero prime ideal of $S^{-1}B$ (Chapter 11, § 2, no. 5, Proposition 11) and $S^{-1}B$ is just the field of fractions of $B$, for it is a subring of $L$ containing $K$ (\emph{Algebra}, Chapter V, § 3, no. 2, Proposition 3); whence an absurd conclusion. If now $p \neq (0)$, it follows from Proposition 5 that $B/pB$ is a finite-dimensional vector space over the field $A/p$, hence an \emph{Artinian} ring and therefore has only a finite number of prime ideals (Chapter IV, § 2, no. 5, Proposition 9), which proves that there is only a finite number of prime ideals of $B$ containing $p$.

#### Corollary 2 {#ac-vii-s2-lem-3-cor-2 .statement}

*The integral closure of $A$ in $L$ is a Dedekind domain.*

This integral closure is an integrally closed Noetherian domain all of whose non-zero prime ideals are maximal; it suffices therefore to apply Theorem 1 of no. 2.

In particular:

#### Corollary 3 {#ac-vii-s2-lem-3-cor-3 .statement}

*The integral closure of a Dedekind domain in a finite extension of its field of fractions is a Dedekind domain.*

#### Proposition 6 {#ac-vii-s2-prop-6 .statement}

*Let $A$ be a Dedekind domain, $K$ its field of fractions, $L$ a finite extension of $K$ and $B$ the integral closure of $A$ in $L$. Let $p$ be a non-zero prime ideal of $A$, $v$ the corresponding essential valuation of $K$ and*

$$
Bp = \prod_i p_i^{e(i)}
$$

*the decomposition of the ideal $Bp$ as a product of prime ideals. Then:*
(a) *the prime ideals of $B$ lying above $p$ are the $p_i$ such that $e(i) > 0$;*
(b) *the valuations $v_i$ on $L$ corresponding to these ideals $p_i$ are, up to equivalence, the valuations on $L$ extending $v$;*
(c) $[B/p_i : A/p] = f(v_i/v);$
(d) $e_i = e(v_i/v)$ (cf. Chapter VI, § 8, no. 1, Definitions 1 and 2).

(a) To say that a prime ideal $q$ of $B$ lies above $p$ amounts to saying that $q \supseteq p$, hence that $q \supseteq Bp$ and that $q$ contains one of the $p_i$ such that $e(i) > 0$ (Chapter 11, § 1, no. 1, Proposition 1).
(b) This follows, taking account of (a), from § 1, no. 8, Corollary to Proposition 12.
(c) The residue field of $v$ is identified with $A/p$ and that of $v_i$ with $B/p_i$ (§ 1, no. 4, Corollary 1 to Proposition 6).

(d) Let $a$ (resp. $a_i$) be a uniformizer for $v$ (resp. $v_i$). Then
$$
a B_{p_i} = a A_p B_{p_i} = p A_p B_{p_i} = p B . B_{p_i} = \left( \prod_j p_j^{e(j)} \right) B_{p_i} = \prod_j (p_j B_{p_i})^{e(j)} \\
= (p_i B_{p_i})^{e(i)} = a_i^{e(i)} B_{p_i}
$$
since $p_j B_{p_i} = B_j$ for $j \neq i$; whence (d), since $e(v_i/v) = v_i(a)$.

### Exercises {#ac-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
