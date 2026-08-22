---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 17
section_title: Reduced Norms and Traces
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.335-A VIII.353
pdf_pages: 0352-0370
extraction: native+ocr
subsections:
    - "no": 1
      title: Complements on Characteristic Polynomials
      page: 335
      pdf_page: 352
    - "no": 2
      title: Reduced Norms and Traces
      page: 339
      pdf_page: 356
    - "no": 3
      title: Properties of Reduced Norms and Traces
      page: 341
      pdf_page: 358
    - "no": 4
      title: The Reduced Norm is a Polynomial Function
      page: 344
      pdf_page: 361
    - "no": 5
      title: Transitivity of Reduced Norms and Traces
      page: 346
      pdf_page: 363
    - "no": 6
      title: Reduced Norms and Determinants
      page: 349
      pdf_page: 366
statements: 30
exercises: 7
content_sha256: 11f069df657704342996d2122efce87e5dccfa6a1cfa49a5616defd552614a6d
---

## § 17. REDUCED NORMS AND TRACES

In this section, K is a commutative field and A a central simple K-algebra of finite degree. We denote the reduced degree of A by $n$.

### 1. Complements on Characteristic Polynomials

Let L be a commutative ring and M a free L-module of finite rank $m$. If $u$ is an endomorphism of M and $r$ a natural number, then we denote by $c_r(u)$ the trace of the endomorphism $\wedge^r(u)$ of the free L-module $\wedge^r(M)$. In particular, we have

(1) $c_0(u) = 1,c_1(u) =$ Tr($u$)$,c_m(u) =$ det($u$),

and $c_r(u) = 0$ for $r > m$. By Proposition 7 of III, §8, No. 4, p. 527, the mapping $u\mapsto$ det($u$) from End(M) to L is a homogeneous polynomial mapping of degree $m$ (IV, §5, No. 9, p. 55). More generally, for every integer $r$ such that $0\leqslant r\leqslant m$, the mapping $c_r$ from End(M) to L is a homogeneous polynomial mapping of degree $r$; this follows from Proposition 10 of III, §8, No. 5, p. 529.

Let $u$ be an endomorphism of M and $\overline{u}$ the endomorphism of the L[X]module $M[X] = M\otimes_LL[X]$ deduced from $u$ by extension of scalars (II, §5, No. 1, p. 277). Recall (III, §8, No. 11, p. 541, Definition 3 and (50)) that the characteristic polynomial of $u$ is the determinant $\chi_u(X)$ of the L[X]endomorphism $X-\overline{u}$ of M[X] and that we have the relation

$$
\chi_u(X) =\sum_{r=0}^m(-1)^rc_r(u) X^{m-r} \tag{2}
$$

Proposition 1. — Let L be a commutative ring, M a free L-module of finite rank m $ \geqslant 1 $, and u an endomorphism of M. There exists a unique endomorphism $ \tilde{u} $ of M satisfying the relation

$$
\tilde{u}(x) \wedge w = x \wedge \wedge^{m-1}(u)(w)
$$

for $ x \in M $ and $ w \in \wedge^{m-1}(M) $. Moreover, we have the relations

$$
u \circ \tilde{u} = \tilde{u} \circ u = \det(u)_M,
$$
$$
\det(\tilde{u}) = \det(u)^{m-1},
$$
$$
\tilde{u} = \sum_{r=0}^{m-1} (-1)^r c_{m-1-r}(u) u^r.
$$

#### Lemma 1 {#alg-viii-s17-lem-1 .statement tag=00KE}

— Let p be an integer such that $ 0 \leqslant p \leqslant m $. For any w in $ \wedge^p(M) $, let $ h_p(w) $ be the linear mapping $ w' \mapsto w \wedge w' $ from $ \wedge^{m-p}(M) $ to $ \wedge^m(M) $. The linear mapping $ h_p : w \mapsto h_p(w) $ from $ \wedge^p(M) $ to $ \operatorname{Hom}_L(\wedge^{m-p}(M), \wedge^m(M)) $ is an isomorphism.

Let $ (e_i)_{i \in I} $ be a basis of M; we endow the set I with a total order. For any subset J of I, set $ e_J = e_{i_1} \wedge \cdots \wedge e_{i_r} $, where $ (i_1, \ldots, i_r) $ is the sequence of elements of J in increasing order. The L-module $ \wedge^{m-p}(M) $ admits as a basis the elements $ e_S $, where S runs through the set of subsets of I with $ m - p $ elements; $ \wedge^m(M) $ has $ \{e_I\} $ as a basis. Consequently, there exists a basis of $ \operatorname{Hom}_L(\wedge^{m-p}(M), \wedge^m(M)) $ consisting of linear mappings $ e_J^* $ characterized by the formula

$$
e_J^*(e_S) = \begin{cases}
e_I & \text{if } I = J \cup S, \\
0 & \text{otherwise},
\end{cases}
$$

where J runs through the set of subsets of I with p elements. It follows from formula (20) of III, §7, No. 8, p. 519 that for every subset J of I with p elements, we have $ h_p(e_J) \in \{e_J^*, -e_J^*\} $; since the elements $ e_J $ form a basis of $ \wedge^p(M) $, the linear mapping $ h_p $ is bijective.

Let us now prove Proposition 1. Let u and $ \tilde{u} $ be endomorphisms of M. Relation (3) is equivalent to

$$
h_1 \circ \tilde{u} = \operatorname{Hom}(\wedge^{m-1}(u) \cdot 1_{\wedge^m(M)}) \circ h_1;
$$

the mapping $ h_1 $ is an isomorphism from M to $ \operatorname{Hom}_L(\wedge^{m-1}(M), \wedge^m(M)) $ by Lemma 1. Consequently, for every endomorphism u of M, there exists a unique endomorphism $ \tilde{u} $ of M satisfying relation (3).

Let $x_1, . . . , x_m$ be elements of M. Let us replace $x$ with $u(x_1)$ and $w$ with $x_2\wedge  \cdots  \wedge x_m$ in (3); we obtain

$\widetilde{u}(u(x_1))\wedge x_2\wedge  \cdots  \wedge x_m=u(x_1)\wedge  \cdots  \wedge u(x_m) =$ det($u$)$x_1\wedge  \cdots  \wedge x_m$.

Consequently, $h_1(\widetilde{u}\circ u(x_1)) =h_1$(det($u$)$x_1$), which gives the relation $\widetilde{u}\circ u=$ det($u$)$_M$ by Lemma 1.

We denote by U the endomorphism $X-\overline{u}$ of the L[X]-module M[X] (VIII, p. 335). By the above applied to U, there exists an endomorphism $\widetilde{U}$ of the L[X]-module M[X] that satisfies the relations

$$
\widetilde{U}(x_1)\wedge x_2\wedge  \cdots  \wedge x_m=x_1\wedge (Xx_2-u(x_2))\wedge  \cdots  \wedge (Xx_m-u(x_m)) \tag{9}
$$

for $x_1, . . . , x_m$ in M and

(10) $\widetilde{U}\circ U =$ det(X $-\overline{u}$)$_{M[X]}$.

Let us view $\widetilde{U}$ as an element of End(M)[X] (VIII, p. 9); by formula (9) and Lemma 1, it has degree $\leqslant m-1$, so we can write it as

$$
\widetilde{U} =\sum^{m-1}_{r=0}(-1)^ru_rX^{m-1-r} \tag{11}
$$

where the $u_r$ are endomorphisms of M. By formula (2), relation (10) gives the equality

$$
(\sum^{m-1}_{r=0}(-1)^ru_rX^{m-1-r})(X-u) =\sum_{r=0}^m(-1)^rc_r(u)X^{m-r} \tag{12}
$$

in the ring End(M)[X]. By identifying the coefficients of the monomials in X on each side, we obtain the relations

(13) $u_r+u_{r-1}\circ u=c_r(u)_M$ for $1\leqslant r\leqslant m-1$

and

$$
u_0=c_0(u)_M,u_{m-1}\circ u=c_m(u)_M \tag{14}
$$

From this, we deduce

$$
u_{m-1}=\sum^{m-1}_{r=0}(-1)^rc_{m-1-r}(u)u^r \tag{15}
$$

Now, when we identify the constant terms, equalities (9) and (11) imply $u_{m-1}=\widetilde{u}$; formula (6) follows.

In particular, $\widetilde{u}$ belongs to the subalgebra of End(M) generated by $u$ and therefore commutes with $u$. We have already established the relation $\widetilde{u}\circ u=$ det($u$)$_M$; formula (4) follows.

Finally, let $x_1, . . . , x_m$ be elements of M. We replace $x$ with $x_1$ and $w$ with $\widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m)$ in formula (3). This gives

$$
\widetilde{u}(x_1)\wedge \widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m) =x_1\wedge u\circ (\widetilde{u}(x_2))\wedge  \cdots  \wedge u\circ (\widetilde{u}(x_m))
$$

= det($u$)$^{m-1}x_1\wedge x_2\wedge  \cdots  \wedge x_m$

and therefore formula (5).

#### Remark 1 {#alg-viii-s17-n1-rem-1 .statement tag=00KF}

The endomorphism $\widetilde{u}$ of M coincides with what we called the cotranspose of $u$ in III, §8, No. 6, p. 532.

#### Remark 2 {#alg-viii-s17-n1-rem-2 .statement tag=00KG}

From formulas (1), (2), (4), and (6), we deduce the relation $\chi_u(u) = 0$ and therefore another proof of the Cayley–Hamilton theorem (III, §8, No. 11, p. 541).

#### Remark 3 {#alg-viii-s17-n1-rem-3 .statement tag=00KH}

Since the mapping $c_r$ from End(M) to L is a homogeneous polynomial mapping of degree $r$ for $0\leqslant r\leqslant m-1$, it follows from formula (6) that the mapping $u\mapsto \widetilde{u}$ from End(M) to End(M) is a homogeneous polynomial mapping of degree $m-1$.

Let B be an algebra over the ring L; suppose that B is a free L-module of rank $m\geqslant 1$, and identify L with the subring $L\cdot 1$ of B. Let $b$ be an element of B. We apply the above to the endomorphism $\gamma (b) :x\mapsto bx$ of the L-module B. Set $\gamma_r(b) =c_r(\gamma (b))$ for $0\leqslant r\leqslant m$; we have, in particular, $\gamma_m(b) = N_{B/L}(b)$ (III, §9, No. 3, p. 543). The characteristic polynomial of $b$ (loc. cit.) can be written as

(16) Pc$_{B/L}(b; X) =\sum_{r=0}^m(-1)^r\gamma_r(b) X^{m-r}$.

Since the mapping $\gamma$ from B to End$_L(B)$ is L-linear, the mapping $\gamma_r$ from B to L is a homogeneous polynomial mapping of degree $r$. In particular, the mapping $b\mapsto N_{B/L}(b)$ from B to L is a homogeneous polynomial mapping of degree $m$.

For any element $b$ of B, set

$$
\widetilde{b}=\sum^{m-1}_{r=0}(-1)^r\gamma_{m-1-r}(b)b^r \tag{17}
$$

By Proposition 1, the linear mapping $\gamma (\widetilde{b})$ from B to B is the cotranspose of the mapping $\gamma (b)$; from this, we deduce

$$
b\widetilde{b}=\widetilde{b}b= N_{B/L}(b) \tag{18}
$$

Moreover, the mapping $b\mapsto \widetilde{b}$ from B to B is a homogeneous polynomial mapping of degree $m-1$.

### 2. Reduced Norms and Traces

Recall that we denote by A a central simple algebra over the commutative field K of reduced degree $n$.

#### Proposition 2 {#alg-viii-s17-prop-2 .statement tag=00KI}

Let $a$ be an element of A and Pc($a; X$) its characteristic polynomial. There exists a unique monic polynomial P in K[X] such that we have Pc($a; X$) $= P(X)^n$.

A) The uniqueness of P follows from Lemma 2 below.

#### Lemma 2 {#alg-viii-s17-lem-2 .statement tag=00KJ}

Let P and Q be monic polynomials in K[X] and $s$ is a strictly positive integer. If $P^s= Q^s$, then we have P = Q.

Let $\mathscr{I}$ be the set of irreducible monic polynomials in K[X]. Since P and Q are monic, there exist elements $(a_F)$ and $(b_F)$ of $\mathbf{N}^{(\mathscr{I})}$ such that we have $P =\prod_{F\in\mathscr{I}}F^{a_F}$ and $Q =\prod_{F\in\mathscr{I}}F^{b_F}$. It follows from the equality $P^s= Q^s$ and the uniqueness of the decomposition into irreducible factors that we have $sa_F=sb_F$ for every $F\in \mathscr{I}$. Since $s$ is strictly positive, we consequently have $a_F=b_F$ for every $F\in \mathscr{I}$, and therefore P = Q.

B) Let us now prove the existence of P.

By Theorem 1 of VIII, p. 252, there exist a Galois extension L of K of finite degree and an isomorphism of L-algebras $\theta : A_{(L)}\rightarrow \mathbf{M}_n(L)$. By formula (12) of III, §9, No. 1, p. 542, the polynomial Pc($a; X$) is also the characteristic polynomial of the element $1\otimes a$ of the L-algebra $A_{(L)}$, hence of the element $\theta (1\otimes a)$ of the L-algebra $\mathbf{M}_n(L)$.

Set P(X) = det(X$I_n-\theta (1\otimes a)$); it is a monic polynomial in L[X]. By Example 3 of III, §9, No. 3, p. 545, we have

(19) Pc($a; X$) $= P(X)^n$.

Let G be the Galois group of L over K. For $\sigma \in G$, denote by $\overline{\sigma}$ the automorphism of the ring L[X] that coincides with $\sigma$ on L and fixes X. Then K[X] is the set of polynomials Q of L[X] such that we have $\overline{\sigma}(Q) = Q$ for every $\sigma \in G$ (V, §10, No. 1, p. 56, Theorem 1). Since the polynomial Pc($a; X$) $= P(X)^n$ belongs to K[X], we have $\overline{\sigma}(P)^n= P^n$ for every $\sigma \in G$. By Lemma 2, we therefore have $\overline{\sigma}(P) = P$ for every $\sigma \in G$, so P belongs to K[X].

#### Definition 1 {#alg-viii-s17-def-1 .statement tag=00RM}

Let $a$ be an element of the algebra A. The reduced characteristic polynomial of $a$ (with respect to A) is the unique monic polynomial in K[X], denoted by Pcrd$_{A/K}(a; X)$, that satisfies the relation

(20) Pc$_{A/K}(a; X) =$ Pcrd$_{A/K}(a; X)^n$.

Let $a$ be an element of A. Since A has degree $n^2$ over K, the polynomial Pc$_{A/K}(a; X)$ has degree $n^2$, so Pcrd$_{A/K}(a; X)$ is a monic polynomial of degree $n$; let us write it as

(21) Pcrd$_{A/K}(a; X) = X^n+\sum^{n-1}_{r=0}(-1)^rb_r(a)X^{n-r}$.

We set

(22) Trd$_{A/K}(a) =b_1(a)$, Nrd$_{A/K}(a) =b_n(a)$.

#### Definition 2 {#alg-viii-s17-def-2 .statement tag=00KK}

We call Trd$_{A/K}(a)$ the reduced trace of A and Nrd$_{A/K}(a)$ its reduced norm (with respect to the K-algebra A).

When there is no risk of confusion, we leave A and K out of the notation and simply write Pcrd($a; X$), Trd($a$), and Nrd($a$).

The following formulas result from formulas (20) and (22) and formulas (7) and (8) of III, §9, No. 1, p. 542:

(23) Tr$_{A/K}(a) =n$ Trd$_{A/K}(a)$,

(24) $N_{A/K}(a) =$ (Nrd$_{A/K}(a)$)$^n$.

#### Proposition 3 {#alg-viii-s17-prop-3 .statement tag=00KL}

An element $a$ of A is invertible if and only if its reduced norm is nonzero. In particular, A is a field if and only if we have Nrd$_{A/K}(a)\not= 0$ for every nonzero element $a$ of A.

An element $a$ of A is invertible if and only if its norm is nonzero (III, §9, No. 4, p. 545, Proposition 3). Proposition 3 therefore follows from formula (24).

#### Remark {#alg-viii-s17-n2-rem-1 .statement tag=00KM}

Let L be the field K(X) of rational fractions in one variable X. The reduced characteristic polynomial of an element $a$ of A is simply the reduced norm of the element $X\otimes 1-1\otimes a$ of the L-algebra $A_{(L)}$. This follows from the definition of the reduced characteristic polynomial and the formula (III, §9, No. 3, p. 544)

(25) Pc$_{A/K}(a; X) = N_{A_{(L)}/L}(X\otimes 1-1\otimes a)$.

#### Example 1 {#alg-viii-s17-n2-exa-1 .statement tag=00RN}

By Theorem 1 of VIII, p. 120, there exist an integer $r\geqslant 1$ and a field D such that A is isomorphic to $\mathbf{M}_r(D)$. Let $d$ be the reduced degree of D over K; we have $r=n/d$. Let M be an A-module of finite length $\ell$; we will prove the formula

(26) Pc$_{M/K}(a_M; X) =$ Pcrd$_{A/K}(a; X)^{d\ell}$

for every element $a$ of A. The A-module $A_s$ has length $r$ (VIII, p. 121, Lemma 2). The A-modules $M^r$ and $A^{\ell}_s$ have the same length, so they are isomorphic, and we have

Pc$_{M/K}(a_M; X)^r=$ Pc$_{A/K}(a; X)^{\ell}$

by formula (15) of III, §9, No. 2, p. 542. Since we have $rd=n$, formula (26) follows from formula (20) and Lemma 2 (VIII, p. 339).

#### Example 2 {#alg-viii-s17-n2-exa-2 .statement tag=00RO}

Consider the specific case when A is the algebra End$_K(V)$ of endomorphisms of a finite-dimensional K-vector space V. Taking M to be the simple A-module V, we obtain the relations

Pcrd$_{A/K}(u; X) =\chi_u(X)$,

(27) Nrd$_{A/K}(u) =$ det($u$),

Trd$_{A/K}(u) =$ Tr($u$)

for every endomorphism $u$ of V.

### 3. Properties of Reduced Norms and Traces

#### Proposition 4 {#alg-viii-s17-prop-4 .statement tag=00KN}

Let L be an extension of K and $a$ an element of the central simple algebra A. We have the relations

(28) Pcrd$_{A_{(L)}/L}(1\otimes a; X) =$ Pcrd$_{A/K}(a; X)$,

(29) Trd$_{A_{(L)}/L}(1\otimes a) =$ Trd$_{A/K}(a)$,

(30) Nrd$_{A_{(L)}/L}(1\otimes a) =$ Nrd$_{A/K}(a)$

(“invariance under extension of scalars”).

The two sides of equality (28) have the same $n$-th power by the definition (formula (20) of VIII, p. 340) and the relation

Pc$_{A_{(L)}/L}(1\otimes a; X) =$ Pc$_{A/K}(a; X)$ (III, §9, No. 3, p. 544, formula (21)). Equality (28) therefore follows from Lemma 2 of VIII, p. 339. Formulas (29) and (30) follow from (28), (21), and (22).

#### Corollary 1 {#alg-viii-s17-prop-4-cor-1 .statement tag=00KO}

Let L be an extension of K. Let V be a vector space of dimension $n$ over L and $\theta$ a K-algebra homomorphism from A to End$_L(V)$. For every element $a$ of A, we have

(31) Pcrd$_{A/K}(a; X) =\chi_{\theta(a)}(X)$,

(32) Trd$_{A/K}(a) =$ Tr($\theta (a)$),

(33) Nrd$_{A/K}(a) =$ det($\theta (a)$).

Let $\theta '$ be the L-algebra homomorphism from $A_{(L)}$ to End$_L(V)$ such that $\theta '(\lambda \otimes a) =\lambda \theta (a)$ for $\lambda \in L$ and $a\in A$. The algebra $A_{(L)}$ is simple by Corollary 2 of VIII, p. 222; the homomorphism $\theta '$ is therefore injective. But the algebras $A_{(L)}$ and End$_L(V)$ over the field L have the same degree, equal to $n^2$, so $\theta '$ is an isomorphism. Corollary 1 then follows from Proposition 4 and Example 2 above.

#### Corollary 2 {#alg-viii-s17-prop-4-cor-2 .statement tag=00KP}

Let $a$ and $a'$ be elements of A and $\lambda$ an element of K. We have the relations

(34) Pcrd$_{A/K}(a;a) = 0$,

(35) Pcrd$_{A/K}(\lambda a;\lambda X) =\lambda^n$ Pcrd$_{A/K}(a; X)$,

(36) Trd$_{A/K}(a+a') =$ Trd$_{A/K}(a) +$ Trd$_{A/K}(a')$,

Trd$_{A/K}(\lambda a) =\lambda$ Trd$_{A/K}(a)$,

(37) Trd$_{A/K}(aa') =$ Trd$_{A/K}(a'a)$,

(38) Nrd$_{A/K}(aa') =$ Nrd$_{A/K}(a)\cdot$ Nrd$_{A/K}(a')$,

Nrd$_{A/K}(\lambda a) =\lambda^n$ Nrd$_{A/K}(a)$,

(39) Trd$_{A/K}(1) =n$, Nrd$_{A/K}(1) = 1$.

Since A is central simple and has reduced degree $n$ over K, there exist an extension L of K and a vector space V of dimension $n$ over L such that $A_{(L)}$ is isomorphic to the algebra End$_L(V)$ (VIII, p. 252, Theorem 1). Corollary 2 then follows from Corollary 1 and the properties of the trace and determinant of an endomorphism. In particular, formula (34) follows from the Cayley– Hamilton theorem (III, §8, No. 11, p. 541, Proposition 20, cf. also VIII, p. 338, Remark 2).

#### Corollary 3 {#alg-viii-s17-prop-4-cor-3 .statement tag=00RP}

Let $A^o$ be the opposite algebra of A. For every $a$ in A, we have

(40) Pcrd$_{A^o/K}(a; X) =$ Pcrd$_{A/K}(a; X)$,

(41) Trd$_{A^o/K}(a) =$ Trd$_{A/K}(a)$,

(42) Nrd$_{A^o/K}(a) =$ Nrd$_{A/K}(a)$.

Choose an extension L of K, a vector space V of dimension $n$ over L, and a homomorphism $\theta$ from A to End$_L(V)$ (VIII, p. 252, Theorem 1). Let $V^*$ be the dual vector space of V. The mapping that sends an element $a$ of A to the endomorphism $^t\theta (a)$ of $V^*$ is a K-algebra homomorphism from $A^o$ to End$_L(V^*)$. Corollary 3 then follows from Corollary 1 and Corollary 3 of III, §8, No. 4, p. 528.

The trace, norm, and characteristic polynomial of $a$ are therefore the same whether we view $a$ as an element of A or as an element of $A^o$. This property does not always hold when A is not assumed central simple (III, §9, p. 644, Exercise 1).

#### Proposition 5 {#alg-viii-s17-prop-5 .statement tag=00KQ}

For any $x$ in A, let $t_x$ be the linear form $y\mapsto$ Trd$_{A/K}(xy)$ on A.

a) The mapping $t:x\mapsto t_x$ is an isomorphism of $(A,A)$-bimodules from A to its dual Hom$_K(A,K)$.

b) Let $h$ be a linear form on A. The following properties are equivalent:

(i) There exists an element $\lambda$ of K such that $h(x) =\lambda$ Trd$_{A/K}(x)$

for every $x\in A$.

(ii) We have $h(xy) =h(yx)$ for all $x, y$ in A.

Recall (II, §1, No. 14, p. 225–226) that the $(A$, A)-bimodule structure on $A^*=$ Hom$_K(A,K)$ is defined by the relation

$$
\langle atb, c\rangle =\langle t, bca\rangle \tag{43}
$$

for $a, b, c\in A$ and $t\in A^*$. In particular, for every $x$ in A, we have

$\langle at_xb, c\rangle =\langle t_x, bca\rangle =$ Trd$_{A/K}(xbca)$,

$\langle t_{axb}, c\rangle =$ Trd$_{A/K}(axbc)$,

and these two elements are equal by formula (37) of VIII, p. 342. We therefore have $at_xb=t_{axb}$, which means that $t$ is a homomorphism of $(A$, A)-bimodules from A to $A^*$.

We choose an extension L of the field K and an isomorphism $\theta$ from the L-algebra $A_{(L)}$ to the matrix algebra $\mathbf{M}_n(L)$ (VIII, p. 252, Theorem 1). We identify the vector space $(A^*)_{(L)}$ with the dual of the vector space $A_{(L)}$ over the field L. By Proposition 4 of VIII, p. 341, with these conventions, we have

(44) Trd$_{A_{(L)}/L}= 1_L\otimes$ Trd$_{A/K}$.

Let $t_{(L)}$ be the L-linear mapping from $A_{(L)}$ to $A^*_{(L)}$ deduced from $t$ by extension of scalars; by formula (44) and Corollary 1, we have

(45) $\langle t_{(L)}(x), y\rangle =$ Trd$_{A_{(L)}/L}(xy) =$ Tr($\theta (x)\theta (y)$)

for $x, y$ in $A_{(L)}$. By Proposition 7 of II, §10, No. 11, p. 358, the mapping $t_{(L)}$ is bijective; it follows that $t$ is bijective. We have proved a).

Let $h$ be in $A^*$; by the above, there exists an element $a$ of A such that $h$ is equal to $t_a$. By a), we have

$$
h(xy)-h(yx) =t_a(xy-yx) =t_{ax}(y)-t_{xa}(y)
$$

Consequently, the relation “$h(xy) =h(yx)$ for $x, y$ in A” is equivalent to “$t_{ax-xa}= 0$ for every $x\in$ A”, and by part a) of the proof, this means that $a$ belongs to the center K of A. This proves b) in view of formula (36).

#### Corollary {#alg-viii-s17-n3-cor-1 .statement tag=00KR}

The linear subspace of A generated by the elements of the form $xy-yx$, where $x$ and $y$ run through A, is a hyperplane, the kernel of the nonzero linear form Trd$_{A/K}$.

#### Remark {#alg-viii-s17-n3-rem-1 .statement tag=00KS}

By formula (23) of VIII, p. 340, we have

Tr$_{A/K}(a) =n$ Trd$_{A/K}(a)$

for every $a\in A$. If the characteristic of the field K is equal to 0 or a prime number $p$ that does not divide $n$, then we can replace the reduced trace with the trace in Proposition 5. On the other hand, if the characteristic of K is a prime number that divides $n$, then we have Tr$_{A/K}(a) = 0$ for every $a\in A$.

### 4. The Reduced Norm is a Polynomial Function

#### Lemma 3 {#alg-viii-s17-lem-3 .statement tag=00KT}

Let L be an extension of K, and let I be a set and $\mathbf{T}= (T_i)_{i\in I}$ a family of variables. We have $K(\mathbf{T})\cap L[\mathbf{T}] = K[\mathbf{T}]$.

Let P and Q be elements of $K[\mathbf{T}]$ with $Q\not= 0$. The coefficients of the polynomials R in $L[\mathbf{T}]$ such that P = QR are the solutions of a system of linear equations with coefficients in K. Consequently, if there exists a polynomial $R\in L[\mathbf{T}]$ such that P = QR, then there also exists one in $K[\mathbf{T}]$ (II, §8, No. 5, p. 321, Proposition 6). This proves the inclusion $K(\mathbf{T})\cap L[\mathbf{T}]\subset K[\mathbf{T}]$; the reverse inclusion is obvious.

Recall that the reduced characteristic polynomial of an element $a$ of A can be written as

(46) Pcrd$_{A/K}(a; X) =\sum_{r=0}^n(-1)^rb_r(a) X^{n-r}$

and that we have

$b_0(a) = 1,b_1(a) =$ Trd$_{A/K}(a),b_n(a) =$ Nrd$_{A/K}(a)$.

#### Proposition 6 {#alg-viii-s17-prop-6 .statement tag=00KU}

For every integer $r$ such that $0\leqslant r\leqslant n$, the mapping $b_r$ from A to K is a homogeneous polynomial mapping of degree $r$. In particular, the reduced norm is a homogeneous polynomial mapping of degree $n$ from A to K.

Let $(e_i)_{i\in I}$ be a basis of A over K and $\mathbf{T}= (T_i)_{i\in I}$ a family of variables.

#### Lemma 4 {#alg-viii-s17-lem-4 .statement tag=00KV}

Let $u$ be the element $\sum_{i\in I}T_i\otimes e_i$ of the central simple $K(\mathbf{T})$-algebra $A_{(K(\mathbf{T}))}$. Let P be the reduced characteristic polynomial of $u$. Then P belongs to the ring $K[\mathbf{T}][X]$; viewed as an element of the ring $K[\mathbf{T},X]$, it is homogeneous of degree $n$.

We choose an extension L of K and an L-algebra isomorphism $\theta$ from $A_{(L)}$ to $\mathbf{M}_n(L)$. We denote by $\overline{\theta}: A_{(L(\mathbf{T}))}\rightarrow \mathbf{M}_n(L(\mathbf{T}))$ the isomorphism of $L(\mathbf{T})$-algebras deduced from $\theta$ by extension of scalars. By Corollary 1 of VIII, p. 342, we have

(47) $P(X) =\chi_{\overline{\theta}(u)}(X) =$ det(X$I_n-\overline{\theta}(u)$) $=$ det$(XI_n-\sum_{i\in I}T_i\theta (1\otimes e_i))$.

Since the matrices $\theta (1\otimes e_i)$ belong to $\mathbf{M}_n$(L), this formula shows that P is a homogeneous polynomial of degree $n$ in $L[\mathbf{T},X]$. It also belongs to $K(\mathbf{T})[X]$ and can be written as $P(X) =\sum_{j\geqslant 0}c_jX^j$, where each $c_j$ belongs to the intersection $K(\mathbf{T})\cap L[\mathbf{T}]$. By Lemma 3, each of the elements $c_j$ belongs to $K[\mathbf{T}]$; Lemma 4 follows.

#### Lemma 5 {#alg-viii-s17-lem-5 .statement tag=00KW}

For every extension $K'$ of K and every element $(t_i)_{i\in I}$ of ${K'}^I$, we have

(48) Pcrd$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i)= P((t_i)_{i\in I},X)$.

Let $\varphi : K[\mathbf{T}]\rightarrow K'$ be the unique K-algebra homomorphism that sends $T_i$ to $t_i$ for every $i\in I$; it defines on $K'$ the structure of a $K[\mathbf{T}$]-algebra. The $K'$-algebra $A_{(K[\mathbf{T}])(K')}$ can be identified with $A_{(K')}$ (transitivity of extension of scalars), where the element $1\otimes (\sum T_i\otimes e_i)$ is identified with the element $\sum t_i\otimes e_i$ of $A_{(K')}$. We denote by $\overline{\varphi}: K[\mathbf{T}][X]\rightarrow K'[X]$ the K-algebra homomorphism deduced from $\varphi$. By formula (21) of III, §9, No. 3, p. 544, the characteristic polynomial of $\sum t_i\otimes e_i$ with respect to the $K'$-algebra $A_{(K')}$ is the image by $\overline{\varphi}$ of the characteristic polynomial of $\sum T_i\otimes e_i$ with respect to the $K[\mathbf{T}$]-algebra $A_{(K[\mathbf{T}])}$, that is, of $P^n$. In other words, we have

(49) Pc$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i; X)= P((t_i)_{i\in I},X)^n$;

Lemma 5 then follows from Lemma 2 of VIII, p. 339.

Consider the specific case $K'= K$ of Lemma 5. We have

(50) Pcrd$_{A/K}(\sum_{i\in I}t_ie_i; X)= P((t_i)_{i\in I},X)$

for every element $(t_i)_{i\in I}$ of $K^I$. Since the polynomial P in $K[\mathbf{T},X]$ is homogeneous of degree $n$, it can be expanded uniquely as

$$
P(\mathbf{T},X) =\sum_{r=0}^n(-1)^rB_r(\mathbf{T}) X^{n-r} \tag{51}
$$

where $B_r$ is a homogeneous polynomial of degree $r$ in $K[\mathbf{T}]$. By formulas (46), (50), and (51), we have

$$
b_r(\sum_{i\in I}t_ie_i)= B_r((t_i)_{i\in I})
$$

for every element $(t_i)_{i\in I}$ of $K^I$. Proposition 6 follows.

#### Remark {#alg-viii-s17-n4-rem-1 .statement tag=00KX}

Let $K'$ be a commutative K-algebra. Every element $t$ of $A_{(K')}$ can be written as $\sum_{i\in I}t_i\otimes e_i$, where $(t_i)\in {K'}^I$. It follows from the proof of Lemma 5 that the characteristic polynomial Pc$_{A_{(K')}/K'}(t; X)$ is equal to $P((t_i),X)^n$.

### 5. Transitivity of Reduced Norms and Traces

#### Proposition 7 {#alg-viii-s17-prop-7 .statement tag=00KY}

Let L be a maximal commutative semisimple subalgebra of A and $a$ an element of L. We have

(52) Pcrd$_{A/K}(a; X) =$ Pc$_{L/K}(a; X)$,

(53) Trd$_{A/K}(a) =$ Tr$_{L/K}(a)$,

(54) Nrd$_{A/K}(a) = N_{L/K}(a)$.

By Proposition 3 of VIII, p. 262, the L-modules A and $L^n$ are isomorphic; we therefore have the relation

Pc$_{A/K}(a; X) =$ Pc$_{L/K}(a; X)^n$.

Since the polynomial Pc$_{L/K}(a; X)$ is monic, it is therefore equal to the reduced characteristic polynomial Pcrd$_{A/K}(a; X)$ (VIII, p. 339, Lemma 2); this gives formula (52). By comparing the coefficients of $X^{n-1}$ (resp. the constant terms) on each side of (52), we obtain formula (53) (resp. (54)).

#### Corollary {#alg-viii-s17-n5-cor-1 .statement tag=00KZ}

Let D be a field of finite degree over K with center K. Let $a$ be an element of K and L a maximal commutative subfield of D containing $a$. We have

Pcrd$_{D/K}(a; X) =$ Pc$_{L/K}(a; X)$,

(55) Tr$_{D/K}(a) =$ Tr$_{L/K}(a)$,

Nrd$_{D/K}(a) = N_{L/K}(a)$.

Indeed, a maximal commutative subfield L of D is a maximal commutative semisimple subalgebra of D by Corollary 2 of VIII, p. 265.

#### Proposition 8 {#alg-viii-s17-prop-8 .statement tag=00L0}

Let B be a simple subalgebra of A. Denote the center of B by L and the commutant of B in A by $B'$. Then $B'$ is a central simple algebra over the field L; we denote its reduced degree by $r$. For every element $b$ of B, we have the relations

(56) Pcrd$_{A/K}(b; X) = N_{L[X]/K[X]}$(Pcrd$_{B/L}(b; X)$)$^r$,

(57) Trd$_{A/K}(b) =r$ Tr$_{L/K}$(Trd$_{B/K}(b)$),

(58) Nrd$_{A/K}(b) = N_{L/K}$(Nrd$_{B/L}(b)$)$^r$.

#### Lemma 6 {#alg-viii-s17-lem-6 .statement tag=00L1}

Let $K'$ be a commutative algebra of finite degree $d$ over K and

$$
P(X) = X^s+a_1X^{s-1}+\cdots +a_s
$$

a monic polynomial with coefficients in $K'$. Then the polynomial Q = $N_{K'[X]/K[X]}(P)$ in K[X] is monic of degree $sd$, the coefficient of $X^{sd-1}$ in Q(X) is equal to Tr$_{K'/K}(a_1)$, and the constant term of Q is $N_{K'/K}(a_s)$.

We denote the $K'$-algebra $K'[T]/(P(T))$ by $K''$ and the canonical class of T in $K''$ by $t$. The sequence $(1, t, . . . , t^{s-1})$ is a basis of $K''$ over $K'$, and the matrix of multiplication by $ t $ in this basis is of the form

$$
\tau = \begin{pmatrix}
0 & 0 & \cdots & 0 & -a_s \\
1 & 0 & \cdots & 0 & -a_{s-1} \\
0 & 1 & \cdots & 0 & -a_{s-2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
0 & \cdots & \cdots & 1 & -a_1
\end{pmatrix}.
$$

The determinant of $ XI_n - \tau $ is calculated by induction on $ s $, by expanding along the first row. We obtain $ \det(XI_n - \tau) = P(X) $. In other words, we have $ P(X) = Pc_{K''/K'}(t; X) $. In particular, $ \operatorname{Tr}_{K''/K'}(t) = -a_1 $ and $ N_{K''/K'}(t) = (-1)^s a_s $. By the transitivity formula (III, §9, No. 4, p. 548, Corollary), we have

$$
\operatorname{Tr}_{K''/K}(t) = -\operatorname{Tr}_{K'/K}(a_1), \quad N_{K''/K}(t) = (-1)^{sd} N_{K'/K}(a_s),
$$
$$
Q(X) = Pc_{K''/K}(t; X).
$$

On the other hand, $[K'' : K] = [K'' : K'][K' : K] = sd$, so $ Q(X) $ is a monic polynomial of degree $ sd $. Lemma 6 follows.

Let us prove Proposition 8. Since the ring $ B $ is simple, its center $ L $ is a field (VIII, p. 121, Corollary 1). By Theorem 5 of VIII, p. 259, the commutant $ B' $ of $ B $ in $ A $ is a simple ring with center $ L $, and we have the equality $[A : K] = [B : K][B' : K]$. We denote the reduced degree of $ B' $ over $ L $ by $ r $, that of $ B $ over $ L $ by $ s $, and the degree of $ L $ over $ K $ by $ d $. We have

$$
[A : K] = n^2, \quad [B' : K] = r^2 d, \quad [B : K] = s^2 d,
$$

and therefore $ n^2 = r^2 s^2 d^2 $, that is, $ n = rsd $.

Let $ b $ be an element of $ B $, and let $ P(X) $ be its reduced characteristic polynomial over the $ L $-algebra $ B $; it is monic of degree $ s $. By Lemma 6, the polynomial $ Q = N_{L[X]/K[X]}(P) $ is monic of degree $ sd $. The polynomial $ R = Q^r $ is therefore monic of degree $ rsd = n $. Again by Lemma 6, the coefficient of $ X^{n-1} $ in $ R(X) $ is equal to $ -r \operatorname{Tr}_{L/K}(\operatorname{Trd}_{B/L}(b)) $, and the constant term of $ R(X) $ is $ (N_{L/K}((-1)^s \operatorname{Nrd}_{B/L}(b)))^r = (-1)^n N_{L/K}(\operatorname{Nrd}_{B/L}(b))^r $.

Since $[A : K] = r^2 d[B : K]$, the left $ B $-module $ A $ is free of rank $ r^2 d $ (VIII, p. 124, Proposition 5). We therefore have

$$
\operatorname{Pc}_{A/K}(b; X) = \operatorname{Pc}_{B/K}(b; X)^{dr^2}.
$$

By the corollary of III, §9, No. 4, p. 548, we have

$$
\operatorname{Pc}_{B/K}(b; X) = N_{L[X]/K[X]}(\operatorname{Pc}_{B/L}(b; X)),
$$

and since P(X) is the reduced characteristic polynomial of $b$ over the L-algebra B, we have

(62) Pc$_{B/L}(b; X) = P(X)^s$.

Finally, by formulas (60)—(62) and the definition of R(X), we have

(63) Pc$_{A/K}(b; X) = N_{L[X]/K[X]}(P(X))^{dr^2s}= Q(X)^{dr^2s}= R(X)^{rsd}= R(X)^n$,

so R(X) is the reduced characteristic polynomial of $b$ over the K-algebra A.

We have proved formula (56). Formulas (57) and (58) follow immediately from formula (56) and Lemma 6 because the coefficient of $X^{n-1}$ in Pcrd$_{A/K}(b; X)$ is equal to $-$ Trd$_{A/K}(b)$ and the constant term is $(-1)^n$ Nrd$_{A/K}(b)$.

### 6. Reduced Norms and Determinants

In this subsection, D is a field of finite degree over K with center K. We denote by $D^*_{ab}$ the quotient of the multiplicative group $D^*$ by its derived (or commutator) group and by $\pi$ the canonical homomorphism from $D^*$ to $D^*_{ab}$. The mapping Nrd$_{D/K}$ induces a group homomorphism from $D^*$ to $K^*$; the kernel of this homomorphism contains the derived group of $D^*$ because K is commutative. Hence there exists a unique homomorphism Nrd from $D^*_{ab}$ to $K^*$ such that Nrd$_{D/K}(x) =$ Nrd $\circ \pi (x)$ for every $x\in D^*$.

#### Proposition 9 {#alg-viii-s17-prop-9 .statement tag=00L2}

Let V be a finite-dimensional right vector space over the field D. Let E be the algebra End$_D(V)$ over the field K; it is central simple and of finite degree. For every invertible element $u$ of E, we have

(64) Nrd$_{E/K}(u) =$ Nrd(det $u$)

(cf. VIII, p. 452, Proposition 2 for the definition of the determinant det $u$ of $u$).

We denote the dimension of V over D by $n$ and identify E with the matrix algebra $\mathbf{M}_n(D)$ using a basis of V over D. The multiplicative group GL$_n(D)$ of the algebra E is generated by the diagonal matrices and the matrices $B_{ij}(\lambda )$ (II, §10, No. 13, p. 362, Corollary 1). Proposition 9 therefore follows from the two specific cases below.

A) Suppose that $u$ is the diagonal matrix diag($a_1, . . . , a_n$). For every $1\leqslant i\leqslant n$, let $L_i$ be a maximal commutative subfield of D containing $a_i$; let L be the subalgebra of E consisting of the diagonal matrices diag($t_1, . . . , t_n$) with $t_i\in L_i$ for $1\leqslant i\leqslant n$. Let $d$ be the reduced degree of D over K. We have $[L_i: K] =d$ for $1\leqslant i\leqslant n$ (VIII, p. 265, Corollary 2). The K-algebra L is isomorphic to $L_1\times  \cdots  \times L_n$ and therefore semisimple of degree $nd$; now, we have $[E : K] =n^2[D : K] =n^2d^2= [L : K]^2$. It follows that L is a maximal commutative semisimple subalgebra of E (VIII, p. 262, Proposition 3). By Proposition 7 of VIII, p. 346, we have Nrd$_{E/K}(u) = N_{L/K}(u)$. Consequently, by formula (18) of III, §9, No. 3, p. 544, we have

Nrd$_{E/K}(u) =\prod_{i=1}^nN_{L_i/K}(a_i) =\prod_{i=1}^n$ Nrd$_{D/K}(a_i)$

= Nrd$_{D/K}(a_1\cdots a_n) =$ Nrd($\pi (a_1\cdots a_n)$).

Moreover, we have det $u=\pi (a_1\cdots a_n)$ by Proposition 3 of VIII, p. 453, which gives formula (64) in this case.

B) Suppose that $u$ is equal to $B_{ij}(\lambda )$, where $\lambda$ is an element of D and $i, j$ are distinct integers in the interval $[1, n]$. Denote by $d$ the reduced degree of D over K and by M the vector space over K deduced from V by restriction of scalars from D to K. Then M is a simple E-module, and we have

(65) Pc$_{M/K}(u; X) =$ Pcrd$_{E/K}(u; X)^d$

by formula (26) of VIII, p. 341. Moreover, M is a vector space of dimension $nd^2$ over K, and $u-1_M$ is a nilpotent endomorphism of M; we therefore have

(66) Pc$_{M/K}(u; X) = (X-1)^{nd^2}$.

By comparing formulas (65) and (66), we obtain

(67) Pcrd$_{E/K}(u; X) = (X-1)^{nd}$

and, in particular, Nrd$_{E/K}(u) = 1$. We also have det $u= 1$ by Proposition 3 of VIII, p. 453; formula (64) therefore holds in this case.

#### Remark {#alg-viii-s17-n6-rem-1 .statement tag=00L3}

We have Nrd$_{E/K}(u) = 0$ if the element $u$ of E is not invertible (VIII, p. 340, Proposition 3).

### Exercises {#alg-viii-s17-exercises}

See the [exercises for § 17](exercises/s17/).
