---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 7
section_title: Multiplicités
lang: en
source: ac-viii-ix-fr
book_pages: AC VIII.71-AC VIII.81, AC VIII.103-AC VIII.108
pdf_pages: 0075-0085, 0107-0112
extraction: ocr
subsections:
    - "no": 1
      title: Multiplicité d’un module relativement à un idéal
      page: 71
      pdf_page: 75
    - "no": 2
      title: Multiplicités et extensions plates
      page: 0
      pdf_page: 77
    - "no": 3
      title: Multiplicités et extensions finies
      page: 74
      pdf_page: 78
    - "no": 4
      title: Multiplicités et suites sécantes
      page: 76
      pdf_page: 80
    - "no": 5
      title: Éléments superficiels
      page: 0
      pdf_page: 81
statements: 28
exercises: 25
content_sha256: 5e26504a0f5b5569f939a060fa77afe6e55574755284c4f13187435e0ede14b9
translated_from: content/fr/ac/VIII/07_s7_multiplicites.md
source_lang: fr
translation_method: machine
source_content_sha256: ab27f72b6ebd27b6e701e4d27ec3936f05f3a650bcf1b98764fd2ae1cd70f4ff
translation_model: gpt-5.4
translation_run: translate-en-mt-a9139937
glossary_version: 34
glossary_terms_sha256: 352f7df914458fd1c2c64900d77719c1ad0aebbe92e12693487096c3e71d0c3e
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 7. MULTIPLICITIES

Throughout this paragraph, $A$ denotes a noetherian ring.

### 1. Multiplicity of a module relative to an ideal

Let $M$ be a finitely generated $A$-module and $q$ an ideal of $A$ contained in the radical of $A$ and such that $M/qM$ is of finite length. Suppose that $M$ is not reduced to 0 and put $d = \dim_A(M)$. By § 4, No. 3, corollary of th. 2 and No. 4, remark 2, there exists a unique integer $e_q(M) > 0$ such that, for every integer $n \geqslant 1$

$$
\operatorname{long}_A(M/q^{n+1}M) = e_q(M) \frac{n^d}{d!} + \beta_n n^{d-1}
$$

where $\beta_n$ tends to a limit as $n$ increases indefinitely.

#### Definition 1 {#ac-viii-s7-def-1 .statement}

The integer $e_q(M)$ is called the multiplicity of the A-module M relative to the ideal q.

It is also denoted by $e_q^A(M)$ when it is desired to mention the ring A. When A is local with maximal ideal m, one writes $e(M)$ or $e^A(M)$ for $e_m(M)$ or $e_m^A(M)$.

#### Remark 1 {#ac-viii-s7-n1-rem-1 .statement}

If q’ is an ideal of A contained in the radical of A and containing q, one has $e_{q'}(M) \leqslant e_q(M)$ and, if the q’-adic filtration of M is q-good, one has $e_{q'}(M) = e_q(M)$ (§ 4, No. 3, th. 2).
2) If M is of finite length, one has $e_q(M) = \operatorname{long}_A(M)$ (§ 4, No. 3, remark 3).
3) If $d > 0$, one has

$$
\operatorname{long}_{A/q}(q^nM/q^{n+1}M) = e_q(M) \frac{n^{d-1}}{(d-1)!} + \alpha_n n^{d-2}
$$

where $\alpha_n$ tends to a limit as $n$ increases indefinitely (§ 4, No. 3, corollary to th. 2).
4) The calculation of multiplicities may be reduced to the case where A is local since, by § 4, No. 4, corollary to th. 3, one has

$$
e_q(M) = \sum e_{q_m}(M_m)
$$

the summation being extended to the maximal ideals m of A such that

$$
m \in \operatorname{Supp}(M) \cap V(q) \quad \text{and} \quad \dim_{A_m}(M_m) = d .
$$

It follows from remarks 2 and 3 that $e_q(M)$ depends only on the graded A/q-module $\operatorname{gr}_q(M)$. Consequently:

#### Proposition 1 {#ac-viii-s7-prop-1 .statement}

Let $\hat{A}$ and $\hat{M}$ be the completions of A and M for their q-adic topologies; then $e_q^A(M) = e_{q\hat{A}}(\hat{M})$.

#### Proposition 2 {#ac-viii-s7-prop-2 .statement}

Suppose that A is local regular (§ 5, No. 1, def. 1); one has $e(A) = 1$.
This follows from th. 1 of § 5, No. 2.

#### Remark 5 {#ac-viii-s7-n1-rem-5 .statement}

It may happen that $e(A) = 1$ without A being regular (p. 104, exerc. 5). In fact, a local noetherian ring A is regular if and only if $\hat{A}$ is integral and if one has $e(A) = 1$ (p. 108, exerc. 24).

#### Example {#ac-viii-s7-n1-exa-1 .statement}

By definition one has $e_{q,r}(M) = r^d e_q(M)$ where $d = \dim_A(M)$. Consequently, if A is local regular, one has $e_{m_A^r}(A) = r^d$. For example, if A is a discrete valuation ring, one has $e_q(A) = \operatorname{long}(A/q)$.

#### Proposition 3 {#ac-viii-s7-prop-3 .statement}

*Let M be a finitely generated A-module, of dimension d ≥ 0. Let Φ be the set of minimal elements p of Supp(M) such that dim(A/p) = d. Let q be an ideal of A, contained in the radical of A, and such that M/qM is of finite length. One has*

$$
e_q(M) = \sum_{p \in \Phi} \operatorname{long}_{A_p}(M_p).e_q(A/p).
$$

#### Corollary {#ac-viii-s7-n1-cor-1 .statement}

*Suppose A semi-local and let q be an ideal of definition of A.
a) One has $e_q(A) = \sum_p e_q(A/p)$, where p runs through the set of minimal prime ideals of A such that $\dim(A/p) = \dim(A)$.
b) Suppose A integral and let M be a finitely generated A-module such that $\dim_A(M) = \dim(A)$. Then one has $e_q(M) = \operatorname{rg}(M).e_q(A)$.*

### 2. Multiplicities and flat extensions

#### Proposition 4 {#ac-viii-s7-prop-4 .statement}

*Let ρ : A → B be a local homomorphism of local noetherian rings, and let N be a finitely generated B-module, flat over A, and such that N ⊗_A κ_A is a B-module of finite length. If M is a nonzero finitely generated A-module and q an ideal of A distinct from A and such that M/qM is of finite length, then (M ⊗_A N)/(qB)(M ⊗_A N) is a B-module of finite length, and one has*

$$
e_{q_B}^B(M ⊗_A N) = \operatorname{long}_B(N ⊗_A κ_A).e_q^A(M).
$$

Let L be an A-module of finite length r. Then L possesses a Jordan-Hölder sequence of length r, with quotients isomorphic to κ_A; since N is flat over A, the B-module L ⊗_A N possesses a composition sequence of length r, with quotients isomorphic to N ⊗_A κ_A, hence is of length r · long_B(N ⊗_A κ_A). Since the B-module (M ⊗_A N)/(qB)^n(M ⊗_A N) is isomorphic to (M/q^nM) ⊗_A N for every $n \in \mathbf{N}$, the proposition follows from the definition of multiplicities.

#### Corollary {#ac-viii-s7-n2-cor-1 .statement}

*Suppose that B is flat over A and that ρ(m_A) B = m_B. Then*

$$
e_{q_B}^B(M ⊗_A B) = e_q^A(M).
$$

This applies in particular when B is the completion \* or the henselisation \* of A relative to an ideal distinct from A, \* or a blowing-up of A, for example a strict henselisation of A. \*

#### Example {#ac-viii-s7-n2-exa-1 .statement}

\* Let X be a complex algebraic variety, $\mathcal{O}_{X,x}$ the local ring of X at a rational point x, $X^{an}$ the analytic space associated with X; let x again denote the point of $X^{an}$ corresponding to x, and let $\mathcal{O}_{X^{an},x}$ be the local ring of $X^{an}$ at x. Then $e(\mathcal{O}_{X^{an},x}) = e(\mathcal{O}_{X,x})$. \*

### 3. Multiplicities and finite extensions

#### Proposition 5 {#ac-viii-s7-prop-5 .statement}

Suppose A semi-local, and let $\rho : A \to B$ be a ring homomorphism making B a finitely generated A-module. Let N be a nonzero finitely generated B-module, and let q be an ideal of A contained in the radical of A, such that $N/qN$ is of finite length. Among the maximal ideals of B (finite in number, by IV, § 2, No. 5, cor. 3 to prop. 9), let us denote by $m_1, ..., m_r$ those for which one has $\dim_{B_{m_i}}(N_{m_i}) = \dim_B(N)$. Put $B_i = B_{m_i}$ and $q_i = qB_i$ for $1 \leq i \leq r$. Then one has the equalities

$$
\dim_A(N) = \dim_B(N),
$$
$$
e_{qB}^B(N) = \sum_{i=1}^r e_{q_i}^{B_i}(N_{m_i}),
$$
$$
e_q^A(N) = \sum_{i=1}^r [B/m_i : A/\rho^{-1}(m_i)]\ e_{q_i}^{B_i}(N_{m_i}).
$$

The first equality follows from § 2, No. 3, th. 1, c); the second follows from Remark 4 of No. 1 (note that $m_i$ belongs to $V(qB)$ for $1 \leq i \leq r$ since $\rho^{-1}(m_i) \supset q$ by V, § 2, No. 1, prop. 1). Let us prove the third equality. Let E be a B-module of finite length; one has

$$
\operatorname{long}_A(E) = \sum_m [B/m : A/\rho^{-1}(m)].\operatorname{long}_{B_m}(E_m),
$$

$m$ ranging over the set of maximal ideals of B; this is in fact evident when E is one of the $B/m$, and the general case follows from this, since E possesses a composition series whose quotients are isomorphic to $B/m$. Applying this formula to the B-modules $N/q^{n+1}N$, one deduces the required equality by definition of the multiplicities.

#### Corollary {#ac-viii-s7-n3-cor-1 .statement}

If $[B/m_i : A/\rho^{-1}(m_i)] = 1$ for every i, one has $e_q^A(N) = e_{qB}^B(N)$.

#### Lemma 1 {#ac-viii-s7-lem-1 .statement}

Let $\rho : A \to B$ be a ring homomorphism, and let $p$ be a prime ideal of A. Consider the following two properties:
(i) the canonical homomorphism $\tilde{\rho}$ of $A_p$ into $A_p \otimes_A B$ is bijective;
(ii) there exists a single prime ideal $r$ of B lying over $p$ and the canonical homomorphism $\rho_p$ of $A_p$ into $B_r$ is bijective.
One has (i) $\Rightarrow$ (ii). If $p$ is minimal, or if B is integral over A, one has (i) $\Leftrightarrow$ (ii) $^1$.

1 This lemma remains valid when the ring A is not noetherian.

The ring $A_p \otimes_A B$ is identified with the ring of fractions $S^{-1}B$ of $B$ defined by the multiplicative subset $S = \rho(A - p)$ of $B$. The prime ideals of $S^{-1}B$ are therefore the $S^{-1}q$, where $q$ is a prime ideal of $B$ such that $\rho^{-1}(q) \subset p$; if $q$ is such an ideal, $(S^{-1}B)_{S^{-1}q}$ is identified with $B_q$ (II, § 2, No. 5, prop. 11).

If condition (i) is satisfied, there exists (V, § 2, No. 1, Lemma 1) a unique prime ideal $r$ of $B$ such that $\rho^{-1}(r) = p$. Moreover, $B_r$ is identified with the ring of fractions $(S^{-1}B)_{S^{-1}r}$, hence also with $(A_p)_s$, where $s$ is the inverse image of $S^{-1}r$ by the isomorphism $\tilde{\rho}: A_p \to S^{-1}B$; now $\tilde{\rho}^{-1}(S^{-1}r) = (A - p)^{-1}p = pA_p$, whence (ii).

Conversely, suppose that (ii) is satisfied, and let $r$ be the unique prime ideal of $B$ lying over $p$. Since $(S^{-1}B)_{S^{-1}r}$ is identified with $B_r$, it is enough to prove that $S^{-1}B$ is local with maximal ideal $S^{-1}r$, that is to say, that every prime ideal $q$ of $B$ such that $\rho^{-1}(q) \subset p$ is contained in $r$. If $p$ is minimal, one has $\rho^{-1}(q) = p$, hence $q = r$. If $B$ is integral over $A$, there exists, by V, § 2, no. 1, cor. 2 to th. 1, a prime ideal $r'$ of $B$ such that $q \subset r'$ and $\rho^{-1}(r') = p$; necessarily one has $r' = r$, hence $q \subset r$.

#### Lemma 2 {#ac-viii-s7-lem-2 .statement}

*Suppose that $A$ is semi-local; let $q$ be an ideal of definition of $A$, and let $\rho : A \to B$ be a ring homomorphism making $B$ into a finitely generated $A$-module. Suppose that, for every prime ideal (necessarily minimal) $p$ of $A$ such that $\dim(A/p) = \dim(A)$, there exists a unique prime ideal $r$ of $B$ lying over $p$ and that the canonical homomorphism $\rho_p : A_p \to B_r$ is bijective. Then one has $\dim_A(B) = \dim(A)$ and $e_q^A(B) = e_q^A(A)$.*

Let $\mathfrak{S}_A$ (resp. $\mathfrak{S}_B$) be the set of prime ideals $p$ of $A$ such that

$$
\dim(A/p) = \dim(A) \quad (\text{resp. } \dim_A(B/pB) = \dim_A(B));
$$

one has $\mathfrak{S}_A \neq \varnothing$. Let $p \in \mathfrak{S}_A$; by assumption there exists a prime ideal of $B$ lying over $p$. Then one has $\rho^{-1}(pB) = p$ (II, § 2, no. 5, cor. 3 to prop. 11), and

$$
\dim(A/p) = \dim(B/pB) = \dim_A(B/pB)
$$

by th. 1, $b)$ and $c)$ of § 2, no. 3. Consequently, one has

$$
\dim_A(B) \geq \dim_A(B/pB) = \dim(A/p) = \dim(A) \geq \dim_A(B).
$$

This implies $\mathfrak{S}_A \subset \mathfrak{S}_B$ and $\dim(A) = \dim_A(B)$. Conversely, if $p \in \mathfrak{S}_B$, one has the inequalities

$$
\dim_A(B/pB) = \dim_A(B) = \dim(A) \geq \dim(A/p) \geq \dim_A(B/pB),
$$

whence $p \in \mathfrak{S}_A$ and $\mathfrak{S}_B = \mathfrak{S}_A$. By prop. 3 of no. 1 and its corollary, one has

$$
e_q^A(A) = \sum_{p \in \mathfrak{S}_A} e_q^A(A/p) \quad \text{and} \quad e_q^A(B) = \sum_{p \in \mathfrak{S}_B} \operatorname{long}_{A_p}(A_p \otimes_A B) e_q^A(A/p);
$$

by Lemma 1, one has $\operatorname{long}_{A_p}(A_p \otimes_A B) = 1$ for every $p \in \mathfrak{S}_A$, whence $e_q^A(A) = e_q^A(B)$.

#### Proposition 6 {#ac-viii-s7-prop-6 .statement}

*Suppose $A$ semi-local and reduced; let $q$ be an ideal of definition of $A$; let $A'$ be the total ring of fractions of $A$, and let $B$ be a finite $A$-subalgebra of $A'$. Then $B$ is semi-local and $qB$ is an ideal of definition of it. Suppose that, for every maximal ideal m of B such that dim(B_m) = dim(B), one has [B/m : A/(A ∩ m)] = 1. Then one has $e_q^A(A) = e_{q_B}^B(B)$.

By IV, § 2, No. 5, cor. 3 of prop. 9, B is semi-local with ideal of definition qB. One has $e_{q_B}^B(B) = e_q^A(B)$ by the corollary to Proposition 5. Since A′ is identified with $\prod_p A_p$ where p runs through the set of minimal prime ideals of A (IV, § 2, No. 5, prop. 10), the canonical mapping $A_p \to A_p \otimes_A B$ is bijective for every minimal prime ideal p of A. It then follows from Lemmas 1 and 2 that $e_q^A(B) = e_q^A(A)$, whence the proposition.

#### Example {#ac-viii-s7-n3-exa-1 .statement}

Let k be a field of characteristic $\neq 2$ and take for A the local ring $k[[X, Y]]/(X^2 + Y^2)$ with residue field k. Take $B = k[[X, T]]/(T^2 + 1)$ where $T = Y/X$. Distinguish two cases: if — 1 is the square of an element i of k, B has two maximal ideals generated respectively by {X, T + i} and {X, T − i}, they have residue field k, and one has $e_{m_A}^A(A) = e_{m_{AB}}^B(B) = 2$. If — 1 is not a square in k, B has a unique maximal ideal (X) with residue field $k[T]/(T^2 + 1)$, and one has $e_{m_A}^A(A) = 2,\ e_{m_{AB}}^B(B) = 1$.

### 4. Multiplicities and secant sequences

#### Proposition 7 {#ac-viii-s7-prop-7 .statement}

Suppose A local. Let s be an integer $\geq 1$ and, for $1 \leq i \leq s$, let $\delta_i$ be an integer $> 0$, $x_i$ an element of $m_A^{\delta_i}$, and $\xi_i$ its class in $m_A^{\delta_i}/m_A^{\delta_i+1}$. Suppose that $(x_1, ..., x_s)$ is a secant sequence for A. Let x denote the ideal of A generated by $(x_1, ..., x_s)$. Then one has $e(A/x) \geq \delta_1 ... \delta_s \cdot e(A)$, with equality if $(\xi_1, ..., \xi_s)$ is a completely secant sequence for gr(A).

Put $B = A/x$, and consider the formal series

$$
H_A = \sum_{n \geq 0} \operatorname{long}(m_A^n/m_A^{n+1}) \cdot T^n, \quad H_B = \sum_{n \geq 0} \operatorname{long}(m_B^n/m_B^{n+1}) \cdot T^n
$$

and $H_B^{(s)} = (1 - T)^{-s} H_B$. By prop. 6 of § 4, No. 5, one has in $\mathbf{Z}[[T]]$ the inequality

$$
H_B^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) H_A,
$$

and there is equality when the sequence $(\xi_1, ..., \xi_s)$ is completely secant. But

$$
R(T) = \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T}
$$

is a polynomial of $\mathbf{Z}[T]$ such that $R(1) = \delta_1 ... \delta_s$. Put $\dim(A) = d$; one has $\dim(B) = d - s$. By th. 2 of § 4, No. 3, there exist elements $R_A$ and $R_B$ of $\mathbf{Z}[T, T^{-1}]$ such that

$$
H_A = (1 - T)^{-d} R_A(T), \quad R_A(1) = e(A),
$$
$$
H_B = (1 - T)^{-d+s} R_B(T), \quad R_B(1) = e(A/x).
$$

Hence one has
$$
(1 - T)^{-d} R_B(T) = H_B^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) H_A = (1 - T)^{-d} R(T) \, R_A(T),
$$
and equality holds if the sequence $(\xi_1, ..., \xi_s)$ is completely secant. One concludes by Lemma 2 of § 4, No. 1.

#### Remark {#ac-viii-s7-n4-rem-1 .statement}

One can prove conversely (*cf.* p. 103, exerc. 4) that if A is regular and $e(A/x) = \delta_1 ... \delta_s$, then the sequence $(\xi_1, ..., \xi_s)$ is completely secant.

#### Example {#ac-viii-s7-n4-exa-1 .statement}

Let $A$ be a ring of formal series $k[[X_1, ..., X_n]]$ over a field $k$; let $F_1, ..., F_s$ be elements of A, a the ideal which they generate, and $B = A/a$. Let $P_1, ..., P_s \in k[X_1, ..., X_n]$ be the initial forms of the series $F_1, ..., F_s$ and $\delta_1, ..., \delta_s$ their respective degrees. If the sequence $F_1, ..., F_s$ is secant in A, one has $e(B) \geq \delta_1 ... \delta_s$; if the sequence $P_1, ..., P_s$ is completely secant in the ring $k[X_1, ..., X_n]$, one has $e(B) = \delta_1 ... \delta_s$.

Consider for example the ring $B = k[[X, Y]]/a$, where a is generated by $X^2 + Y^3$ and $X^2 + Y^4$; the preceding inequality gives $e(B) \geq 4$; observing that a is generated by the elements $X^2 + Y^3$ and $Y^4 - Y^3$, for which the sequence of initial forms is completely secant, one obtains $e(B) = 6$.

### 5. Superficial elements

In this number, q denotes an ideal of A contained in the radical of A, and M a nonzero finitely generated A-module such that $M/qM$ is of finite length.

#### Proposition 8 {#ac-viii-s7-prop-8 .statement}

Let $\delta > 0$ be an integer, x an element of $q^\delta$, $\xi$ its class in $\mathrm{gr}_\delta(A) = q^\delta/q^{\delta+1}$ and $\varphi$ the multiplication by $\xi$ in the gr(A)-module gr(M).

a) The dimension of the A-module $M/xM$ is equal to $\dim_A(M)$ or to $\dim_A(M) - 1$. In the second case, one has $e_q(M/xM) \geq \delta e_q(M)$.

b) Suppose that one has $\dim_A(M) \geq 1$ and that the kernel of $\varphi$ is of finite length over $A/q$. Then one has $\dim_A(M/xM) = \dim_A(M) - 1$. Moreover:
(i) If $\dim_A(M) > 1$, one has $e_q(M/xM) = \delta e_q(M)$.
(ii) If $\dim_A(M) = 1$, one has for every integer $n \geq 0$
$$
n \delta e_q(M) \leq \mathrm{long}_A(M/x^nM) \leq n \delta e_q(M) + \mathrm{long}_{A/q}(\mathrm{Ker}\ \varphi^n),
$$
where $\varphi^n$ is the n-th iterate of the endomorphism $\varphi$, and
$$
\delta e_q(M) = e_{xA}(M) \leq \mathrm{long}_A(M/xM).
$$

Put $M'' = M/xM$; consider the Hilbert-Samuel series $H_M = H_{M,q}$ and $H_{M''} = H_{M'',q}$, together with the Poincaré series $P(T) = \sum_{n \geq 0} \mathrm{long}_{A/q}(\mathrm{Ker}\ \varphi_n) \cdot T^n$. By § 4, No. 3, th. 2 and No. 4, remark 2, one has
$$
H_M(T) = (1 - T)^{-d} R_M(T), \quad H_{M''}(T) = (1 - T)^{-d''} R_{M''}(T),
$$

with $d = \dim_A(M)$, $d'' = \dim_A(M'')$, $R_M$ and $R_{M''}$ in $\mathbf{Z}[T]$, $R_M(1) = e_q(M)$, $R_{M''}(1) = e_q(M'')$. By lemma 6 of § 4, No. 5, one has in $\mathbf{Z}((T))$ the inequalities

$$
(1 - T^\delta) H_M^{(1)} \leq H_{M''}^{(1)} \leq (1 - T^\delta) H_M^{(1)} + T^\delta P^{(1)} .
$$

Putting $R(T) = (1 - T^\delta)/(1 - T) = 1 + T + \cdots + T^{\delta-1}$, this may also be written

(1) $$ (1 - T)^{-d} R(T) R_M(T) \leq (1 - T)^{-d''-1} R_{M''}(T) \leq $$
$$ \leq (1 - T)^{-d} R(T) R_M(T) + (1 - T)^{-1} T^\delta P(T) . $$

By Lemma 2 of § 4, No. 1, the first inequality (1) implies either $d'' \geq d$, or $d'' = d - 1$ and $R(1) R_M(1) \leq R_{M''}(1)$, that is to say $\delta e_q(M) \leq e_q(M'')$. This proves $a)$, since $d'' \leq d$.

Under the assumption of $b)$, one has $P(T) \in \mathbf{Z}[T]$ and $P(1) = \operatorname{long}_A(\operatorname{Ker} \varphi)$. The second inequality (1) is written

$$
(1 - T)^{-d''-1} R_{M''}(T) \leq (1 - T)^{-d}(R(T) R_M(T) + T^\delta (1 - T)^{d-1} P(T)) .
$$

Suppose that one has $d > 1$; then Lemma 2 of § 4, No. 1 yields $d'' + 1 \leq d$, whence $d'' = d - 1$ by part $a)$ of the proof; one then has

$$
R_{M''}(1) \leq R(1). R_M(1)
$$

(loc. cit.), whence (i).

Now suppose $d = 1$. By loc. cit., one has $d'' = 0$ and

$$
R_{M''}(1) \leq R(1). R_M(1) + P(1) .
$$

Consequently, $M''$ is of finite length equal to $e_q(M'') = R_{M''}(1)$, and one obtains

(2) $$ \delta e_q(M) \leq \operatorname{long}_A(M/xM) \leq \delta e_q(M) + \operatorname{long}_A(\operatorname{Ker} \varphi) . $$

Let $n \geq 1$ be an integer. Replace $x$ by $x^n$ in (2); one therefore has

(3) $$ n \delta e_q(M) \leq \operatorname{long}_A(M/x^nM) \leq n \delta e_q(M) + \operatorname{long}_A(\operatorname{Ker} \varphi^n) . $$

It is immediate that the submodules $\operatorname{Ker} \varphi^n$ of the noetherian gr(A)-module gr(M) form an increasing sequence and hence are stationary, and that each of them is of finite length over $A/q$. Dividing by $n \geq 1$ in inequality (3) and making $n$ tend to $+ \infty$, one finds $e_{xA}(M) = \delta e_q(M)$ by definition of $e_{xA}(M)$.

#### Lemma 3 {#ac-viii-s7-lem-3 .statement}

Let $R$ be a noetherian graded ring with degrees $\geq 0$, $E$ a graded $R$-module of finite type such that $E_n$ is an $R_0$-module of finite length for every $n \in \mathbf{Z}$.
The following conditions are equivalent:
(i) $E$ is an $R$-module of finite length;
(ii) there exists an integer $n_0$ such that $E_n = 0$ for $n \geq n_0$;
(iii) every prime ideal of $R$ associated with $E$ contains $R_+ = \bigoplus_{n \geq 1} R_n$.

(i) ⇔ (ii): this is clear.
(iii) ⇒ (i): let $p$ be a prime ideal associated with E. If (iii) is satisfied, one has $p = p_0 + R_+$ where $p_0$ is a prime ideal of $R_0$, and the R-module $R/p$ is isomorphic to $R_0/p_0$. By IV, § 3, No. 1, corollary of Prop. 1, the $R_0$-module $R_0/p_0$ is isomorphic to a submodule of one of the $E_k$, hence is of finite length. Consequently, $R/p$ is of finite length. By IV, § 2, No. 5, Prop. 7, $p$ is therefore maximal. In view of the arbitrariness of $p$, the R-module E is of finite length (loc. cit.).
(i) ⇒ (iii): let $p$ be a prime ideal associated with E. Then $p$ is graded (IV, § 3, No. 1, Prop. 1) and maximal (IV, § 2, No. 5, Prop. 7), hence contains $R_+$ (§ 6, No. 2, Lemma 1).

#### Proposition 9 {#ac-viii-s7-prop-9 .statement}

Let us denote by $p_1, ..., p_r$ those prime ideals of the graded ring $\mathrm{gr}(A) = \bigoplus_n (q^n/q^{n+1})$ which are associated with the graded module $\mathrm{gr}(M) = \bigoplus_n (q^n M/q^{n+1} M)$ and do not contain $\mathrm{gr}_1(A) = q/q^2$. Let $\delta$ be an integer $> 0$, $\xi$ an element of $\mathrm{gr}_\delta(A)$, and $\varphi : \mathrm{gr}(M) \to \mathrm{gr}(M)$ the homothety of ratio $\xi$ in $\mathrm{gr}(M)$. For $\varphi_n$ to be injective for every $n$ sufficiently large, it is necessary and sufficient that $\xi$ belong to none of the $p_i$.
In fact, the prime ideals associated with the $\mathrm{gr}(A)$-module $\mathrm{Ker}\, \varphi$ are those of the prime ideals associated with $\mathrm{gr}(M)$ which contain $\xi$ (IV, § 1, No. 1, Def. 1). By Lemma 3, $(\mathrm{Ker}\, \varphi)_n$ is zero for $n$ sufficiently large, if and only if all these ideals contain $\mathrm{gr}_+(A)$ (or, what amounts to the same, $\mathrm{gr}_1(A)$), whence the proposition.

#### Definition 2 {#ac-viii-s7-def-2 .statement}

Let A be a noetherian ring, q an ideal of A contained in the radical of A, and M a finitely generated A-module such that $M/qM$ is of finite length. An element x of A is said to be superficial for M relative to q if it belongs to q and if, for every $n$ sufficiently large, the mapping $q^n M/q^{n+1} M \to q^{n+1} M/q^{n+2} M$ induced by multiplication by x is injective.

#### Remark 1 {#ac-viii-s7-n5-rem-1 .statement}

Let $\delta$ be an integer $> 0$. One sometimes says that an element x of A is superficial of order $\delta$ for M relative to q if $x \in q^\delta$, and if, for all $n$ sufficiently large, the mapping $q^n M/q^{n+1} M \to q^{n+\delta} M/q^{n+\delta+1} M$ induced by multiplication by x is injective. With this terminology, the superficial elements in the sense of Def. 2 are the superficial elements of order 1.
2) With the notation of Prop. 9, x is superficial of order $\delta$ if and only if its class $\xi$ in $\mathrm{gr}_\delta(A)$ does not belong to any of the $p_i$.
3) By III, § 1, No. 4, Prop. 8, there exists a homogeneous element of $\mathrm{gr}(A)$ of degree $> 0$ which does not belong to any of the $p_i$. Consequently, there exist an integer $\delta > 0$ and a superficial element of order $\delta$ for M.
4) Suppose A local with residue field k, and consider the canonical surjective mapping $\lambda : q \to q \otimes_A k$. It is the composite of the canonical mappings $q \to q/q^2$ and $\bar{\lambda} : q/q^2 \to q \otimes_A k$. By Nakayama's lemma, each of the vector subspaces $V_i = \bar{\lambda}(p_i \cap (q/q^2))$ of $q \otimes_A k$ is distinct from $q \otimes_A k$; if $\alpha \in q \otimes_A k$ does not belong to any of the $V_i$, then $\lambda^{-1}(\alpha)$ consists of superficial elements for M (Prop. 9). If k is infinite, the union of the $V_i$ is distinct from $q \otimes_A k$ and there therefore exist superficial elements for M.

#### Theorem 1 {#ac-viii-s7-thm-1 .statement}

Let $A$ be a noetherian ring, $q$ an ideal of $A$ contained in the radical of $A$ and $M$ a finitely generated $A$-module such that $M/qM$ is of finite length. Let $x_1, ..., x_m$ be a finite sequence of elements of $q$. Put $x = Ax_1 + \cdots + Ax_m \subset q$.

a) One has $\dim_A(M/xM) \geq \dim_A(M) - m$.

b) If $\dim_A(M/xM) = \dim_A(M) - m$, then $e_q(M/xM) \geq e_q(M)$.

c) If $m < \dim_A(M)$, and if for $i = 1, ..., m$, the element $x_i$ of $A$ is superficial for $M/(x_1M + \cdots + x_{i-1}M)$ relative to $q$, then one has

$$
\dim_A(M/xM) = \dim_A(M) - m \quad \text{and} \quad e_q(M/xM) = e_q(M) .
$$

d) If $m = \dim_A(M)$, and if, for $i = 1, ..., m$, the element $x_i$ of $A$ is superficial for $M/(x_1M + \cdots + x_{i-1}M)$ relative to $q$, then one has

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM) < + \infty .
$$

Parts $a), b),$ and $c)$ follow, for $m = 1$, from Prop. 8, and the general case is deduced by induction. Suppose the hypotheses of $d)$ are satisfied and set $x' = Ax_1 + \cdots + Ax_{m-1}$ and $M' = M/x'M$, so that $M/xM$ is identified with $M'/x_mM'$. Then, by $c)$, one has $\dim_A(M') = 1$ and $e_q(M) = e_q(M')$. By Prop. 8, $M/xM$ is of finite length and one has $e_q(M') = e_{x_mA}(M') \leq \operatorname{long}(M/xM)$. But, since $x_m^nM' = x^nM'$ for every $n$, one has $e_{x_mA}(M') = e_x(M')$. On the other hand, one has $e_x(M') \geq e_x(M)$: this follows from $b)$, where $m$ is replaced by $m - 1$, $x$ by $x'$, and $q$ by $x$. Consequently, one has

$$
e_x(M) \leq e_x(M') = e_{x_mA}(M') = e_q(M') = e_q(M) .
$$

Since $x$ is contained in $q$, this implies $e_x(M) = e_q(M)$ (No. 1, Remark 1), and completes the proof.

#### Corollary {#ac-viii-s7-n5-cor-1 .statement}

Suppose that $A$ is local, with infinite residue field, and set $d = \dim_A(M)$. There exists a sequence $x_1, ..., x_d$ of elements of $q$ such that, on setting $x = Ax_1 + \cdots + Ax_d$, one has

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM) < + \infty .
$$

This follows at once from the theorem and Remark 4.

#### Remark 5 {#ac-viii-s7-n5-rem-5 .statement}

In the situation of the preceding corollary, one has

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM)
$$

and $\operatorname{long}(M/qM) \leq \operatorname{long}(M/xM)$; the three cases

$$
e_q(M) < \operatorname{long}(M/qM) , \quad e_q(M) = \operatorname{long}(M/qM) , \quad e_q(M) > \operatorname{long}(M/qM)
$$

are possible (p. 106, Exerc. 16 and 17).

Exercises

## EXERCISES {#ac-viii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
