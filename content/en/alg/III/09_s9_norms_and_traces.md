---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 9
section_title: Norms and traces
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0565-0574, 0668-0668
extraction: ocr
subsections:
    - "no": 1
      title: NORMS AND TRACES RELATIVE TO A MODULE
      page: 0
      pdf_page: 565
    - "no": 2
      title: PROPERTIES OF NORMS AND TRACES RELATIVE TO A MODULE
      page: 0
      pdf_page: 566
    - "no": 3
      title: NORM AND TRACE IN AN ALGEBRA
      page: 0
      pdf_page: 567
    - "no": 4
      title: PROPERTIES OF NORMS AND TRACES IN AN ALGEBRA
      page: 0
      pdf_page: 569
    - "no": 5
      title: DISCRIMINANT OF AN ALGEBRA
      page: 0
      pdf_page: 573
statements: 13
exercises: 1
content_sha256: 8434084d69552b8f7b8ee7ec79fb769815bf1868b7a0b4a9cde2013668383c85
---

## § 9. NORMS AND TRACES

Throughout this paragraph, $K$ will denote a commutative ring and $A$ a unital associative $K$-algebra. Every $A$-module will be assumed to be given the $K$-module structure obtained by restricting the scalars to $K$.

### 1. NORMS AND TRACES RELATIVE TO A MODULE

#### Definition 1 {#alg-iii-s9-def-1 .statement}

Let $M$ be an $A$-module admitting a finite basis as a $K$-module. For all $a \in A$, let $a_M$ be the endomorphism $x \mapsto ax$ of the $K$-module $M$. The trace, determinant and characteristic polynomial of $a_M$ are called respectively the trace, norm and characteristic polynomial of $z$ relative to $M$.

The trace and norm of $a$ are therefore elements of $K$, denoted respectively by $\operatorname{Tr}_{M/K}(a)$ and $N_{M/K}(a)$; the characteristic polynomial of $a$ is an element of $K[X]$, denoted by $\mathrm{Pc}_{M/K}(a; X)$. We omit $K$ in the above notation when there is no risk of confusion.

From the properties of the trace and determinant of an endomorphism (II, § 4, no. 3 and § 8, no. 1) we obtain the relations

$$
\operatorname{Tr}_M(a + a') = \operatorname{Tr}_M(a) + \operatorname{Tr}_M(a')
$$

(2)    $\mathrm{Tr}_M(aa') = \mathrm{Tr}_M(a'a)$
(3)    $N_M(aa') = N_M(a)N_M(a')$

for all $a, a'$ in $A$.

Let $(e_i)_{1 \leq i \leq n}$ be a basis of the $K$-module $M$ and $(m_{ij}(a))$ the matrix of the endomorphism $a_M$ with respect to this basis. The functions $m_{ij}$ are linear forms on the $K$-module $A$ and

(4)    $\mathrm{Tr}_M(a) = \sum_{i=1}^n m_{ii}(a)$
(5)    $N_M(a) = \det(m_{ij}(a))$
(6)    $\mathrm{Pc}(a; X) = \det(\delta_{ij}X - m_{ij}(a)).$

It follows from the method of calculating a determinant (§ 8, no. 11, formula (50)) that

(7)    $\mathrm{Pc}_M(a; X) = X^n + c_1 X^{n-1} + \cdots + c_n$

where

(8)    $c_1 = -\mathrm{Tr}_M(a), \quad c_n = (-1)^n N_M(a).$

For $\lambda \in K$,

(9)    $\mathrm{Tr}_M(\lambda) = n.\lambda, \quad N_M(\lambda) = \lambda^n, \quad \mathrm{Pc}_M(\lambda; X) = (X - \lambda)^n.$

Let $K'$ be a commutative $K$-algebra. Let $M' = K' \otimes_K M$ and $A' = K' \otimes_K A$, so that $M'$ has an $A'$-module structure (§ 4, Example 2). As a $K'$-module $M'$ admits the basis consisting of the $1 \otimes e_i$ ($1 \leq i \leq n$) and the matrix of $a_M$ with respect to $(e_i)$ is equal to the matrix of $(1 \otimes a)_M'$ with respect to $(e'_i)$. Then

(12)    $\mathrm{Tr}_{M'}(1 \otimes a) = \mathrm{Tr}_M(a).1, \quad N_{M'}(1 \otimes a) = N_M(a).1$
        $\mathrm{Pc}_{M'}(1 \otimes a; X) = \mathrm{Pc}_M(a; X).1$

for all $a \in A$, where 1 denotes the unit element of $K'$. If in particular we take $K' = K[X]$, then

(13)    $\mathrm{Pc}_{M/K}(a; X) = N_{M[X]/K[X]}(X - a).$

### 2. PROPERTIES OF NORMS AND TRACES RELATIVE TO A MODULE

If $M$ and $M'$ are two *isomorphic* $A$-modules with finite bases over $K$, then, for all $a \in A$,

(14)    $\mathrm{Tr}_{M'}(a) = \mathrm{Tr}_M(a), \quad N_{M'}(a) = N_M(a), \quad \mathrm{Pc}_{M'}(a; X) = \mathrm{Pc}_M(a; X)$

for if $f$ is an isomorphism of $M$ onto $M'$, the matrix of $a_M$ with respect to a basis $B$ of $M$ over $K$ is the same as the matrix of $a_{M'}$ with respect to the basis $f(B)$ of $M'$.

#### Proposition 1 {#alg-iii-s9-prop-1 .statement}

Let $M = M_0 \supset M_1 \supset \ldots \supset M_r = \{0\}$ be a decreasing sequence of submodules of an $A$-module $M$ such that each of the $K$-modules $P_i = M_{i-1}/M_i$ ($1 \leq i \leq r$) admits a finite basis. Then the $K$-module $M$ admits a finite basis and

$$
\operatorname{Tr}_M(a) = \sum_{i=1}^r \operatorname{Tr}_{P_i}(a), \qquad N_M(a) = \prod_{i=1}^r N_{P_i}(a)
$$
(15)

$$
P_{C_M}(a; X) = \prod_{i=1}^r P_{C_{P_i}}(a; X).
$$

Let $B'_i$ be a basis of $P_i$ over $K$; then a system of representatives $B_i$ of $B'_i$ (mod. $M_i$) is a basis of a supplementary submodule of the $K$-module $M_i$ in the $K$-module $M_{i-1}$ (II, § 1, no. 11, Proposition 21). The union $B$ of the $B_i$ ($1 \leq i \leq r$) is a basis of $M$ over $K$. Let $X_{tt}$ be the matrix of the endomorphism $a_{P_i}$ with respect to the basis $B'_i$. It is immediate that the matrix of $a_M$ with respect to $B$ is of the form

$$
\begin{pmatrix}
X_{rr} & X_{r,r-1} & \cdots & X_{r,1} \\
0 & X_{r-1,r-1} & \cdots & X_{r-1,1} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & X_{11}
\end{pmatrix}
$$

and the proposition follows from formulae (4), (5) and (6) of no. 1 and formula (31) of § 8, no. 6.

#### Proposition 2 {#alg-iii-s9-prop-2 .statement}

Let $A, A'$ be two $K$-algebras, $M$ an $A$-module and $M'$ an $A'$-module. Suppose that $M$ and $M'$ are free $K$-modules of respective dimensions $n$ and $n'$ and consider $M \otimes_K M'$ as an $(A \otimes_K A')$-module ($§ 4$, no. 3, Example 2). Then, for $a \in A$ and $a' \in A'$,

$$
\operatorname{Tr}_{M \otimes M'}(a \otimes a') = \operatorname{Tr}_M(a) \operatorname{Tr}_{M'}(a')
$$
(16)

$$
N_{M \otimes M'}(a \otimes a') = (N_M(a))^{n'} (N_{M'}(a'))^n.
$$
(17)

Formula (16) follows from II, § 4, no. 4, formula (26) and formula (17) from § 8, no. 6, formula (33).

### 3. NORM AND TRACE IN AN ALGEBRA

#### Definition 2 {#alg-iii-s9-def-2 .statement}

Let $A$ be a $K$-algebra which is a finite-dimensional free $K$-module. For every element $a \in A$, the trace (resp. norm,\footnote{† This notion should not be confused with the notion for norm in an algebra over a valued field (\emph{General Topology}), IX, § 3, no. 7.) resp. characteristic polynomial) of $a$ relative to $A$ and $K$ is the trace (resp. determinant, resp. characteristic polynomial) of the endomorphism $x \mapsto ax$ of the $K$-module $A$.

The trace, norm and characteristic polynomial of $a \in A$ relative to $A$ and $K$ are denoted by $\mathrm{Tr}_{A/K}(a)$, $N_{A/K}(a)$ and $\mathrm{Pc}_{A/K}(a; X)$; we omit $K$ and even $A$ from this notation when there is no risk of confusion. Note that the trace (resp. norm, characteristic polynomial) of $a \in A$ is just the trace (resp. norm, characteristic polynomial) of $a$ relative to the $A$-module $A_s$.

Suppose that $A$ is the product $A_1 \times A_2 \times \cdots \times A_m$ of a finite number finite-dimensional algebras over $K$ which are free $K$-modules. Using the above remark and Proposition 1 of no. 2, we have, for every element

$$
a = (a_1, \ldots, a_m) \in A,
$$

$$
\mathrm{Tr}_{A/K}(a) = \sum_{i=1}^m \mathrm{Tr}_{A_i/K}(a_i), \qquad N_{A/K}(a) = \prod_{i=1}^m N_{A_i/K}(a_i)
$$
(18)

$$
\mathrm{Pc}_{A/K}(a; X) = \prod_{i=1}^m \mathrm{Pc}_{A_i/K}(a_i; X).
$$

Similarly, Proposition 2 of no. 2 shows that if $A$ and $A'$ are two algebras, which are free $K$-modules, of finite dimensions $n, n'$ respectively over $K$, then, for $a \in A, a' \in A'$.

$$
\mathrm{Tr}_{A \otimes A'}(a \otimes a') = \mathrm{Tr}_A(a) \, \mathrm{Tr}_{A'}(a')
$$
(19)

$$
N_{A \otimes A'}(a \otimes a') = (N_A(a))^{n'} (N_{A'}(a'))^n.
$$
(20)

Finally let $A$ be a finite-dimensional algebra over $K$ which is a free $K$-module, $h$ a homomorphism of $K$ into a commutative ring $K'$ and $A' = A_{(K')}$ the $K'$-algebra derived from $A$ by extending the scalars by means of $h$. It follows from formula (12) of no. 1 that, for all $a \in A$,

$$
\mathrm{Tr}_{A'/K'}(1 \otimes a) = h(\mathrm{Tr}_{A/K}(a)), \qquad N_{A'/K'}(1 \otimes a) = h(N_{A/K}(a))
$$
(21)

$$
\mathrm{Pc}_{A'/K'}(1 \otimes a; X) = \bar{h}(\mathrm{Pc}_{A/K}(a; X))
$$

where $\bar{h}$ is the homomorphism $K[X] \to K'[X]$ derived from $h$. In particular, for $K' = K[X]$, we obtain, writing $A[X] = A \otimes_K K[X]$,

$$
\mathrm{Pc}_{A/K}(a; X) = N_{A[X]/K[X]}(X - a).
$$
(22)

More generally, if $K'$ is a commutative $K$-algebra and $A' = A \otimes_K K'$, then, for all $x \in A'$,

$$
\mathrm{Pc}_{A/K}(a; x) = N_{A'/K'}(x - a).
$$

#### Example {#alg-iii-s9-n3-exa-1 .statement}

(1) Let $A$ be a quadratic algebra over $K$ of type $(\alpha, \beta)$ and $(e_1, e_2)$ a basis of type $(\alpha, \beta)$ (§ 2, no. 3). For $x = \xi e_1 + \eta e_2$, $\mathrm{Tr}_{A/K}(x) = 2\xi + \beta \eta$ and $N_{A/K}(x) = \xi^2 + \beta \xi \eta - \alpha \eta^2$; these functions are therefore identical with the Cayley trace and norm of $x$ (§ 2, no. 24).

(2) Let $A$ be a quaternion algebra over $K$. A direct calculation allows us to verify that $\mathrm{Tr}_{A/\mathbf{K}}(x) = 2T(x)$ and $N_{A/\mathbf{K}}(x) = (N(x))^2$, where T and N are the Cayley trace and norm (§ 2, no. 4).

(3) Let $A = \mathbf{M}_n(\mathbf{K})$ and let the canonical basis $(E_{ij})$ of A (II, § 10, no. 3) be arranged in lexicographic order. Then it is immediately seen that for every matrix $X = \sum_{i,j} \xi_{ij} E_{ij}$ the matrix (of order $n^2$) of the endomorphism $Y \mapsto XY$ is of the form

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

whence $\mathrm{Tr}_{A/\mathbf{K}}(X) = n \cdot \mathrm{Tr}(X)$ and $N_{A/\mathbf{K}}(X) = (\det(X))^n$.

### 4. PROPERTIES OF NORMS AND TRACES IN AN ALGEBRA

#### Proposition 3 {#alg-iii-s9-prop-3 .statement}

*Let A be a K-algebra admitting a finite basis. For an element $a \in A$ to be invertible, it is necessary and sufficient that its $N_{A/\mathbf{K}}(a)$ be invertible in $\mathbf{K}$.*

If $a$ admits an inverse $a'$ in $A$, then

$$
N_{A/\mathbf{K}}(a) N_{A/\mathbf{K}}(a') = N_{A/\mathbf{K}}(aa') = N_{A/\mathbf{K}}(1) = 1
$$

by formula (3) of no. 1. Conversely, if $N_{A/\mathbf{K}}(a)$ is invertible, the endomorphism $h : x \mapsto ax$ is bijective (§ 8, no. 2, Theorem 1). Then there exists $a' \in A$ such that $aa' = 1$; then $h(a'a - 1) = aa'a - a = (aa' - 1)a = 0$, whence $aa' = 1$ since $h$ is injective. Hence $a'$ is the inverse of $a$.

#### Proposition 4 {#alg-iii-s9-prop-4 .statement}

*Let A be a K-algebra admitting a finite basis. For all $a \in A$, $\mathrm{Pc}_{A/\mathbf{K}}(a; a) = 0$.*

This follows immediately from the Cayley-Hamilton theorem (§ 8, no. 11, Proposition 20).

#### Proposition 5 {#alg-iii-s9-prop-5 .statement}

*Let A be a K-algebra and m a two-sided ideal of A. Suppose that $A_0 = A/m$ is a free K-module of finite dimension n, that there exists an integer $r > 0$ such that $m^r = \{0\}$ and that $m^{i-1}/m^i$ is a free $A_0$-module of finite dimension $s_i$ for $1 \leq i \leq r$. Let $s = s_1 + \cdots + s_r$ and for all $a \in A$ let $a_0$ denote the class of $a$ mod. m. Then A is a free K-module of dimension $ns$ and, for all $a \in A$,

$$
\mathrm{Tr}_A(a) = s \cdot \mathrm{Tr}_{A_0}(a_0), \qquad N_A(a) = (N_{A_0}(a_0))^s
$$
$$
\mathrm{Pc}_A(a; X) = (\mathrm{Pc}_{A_0}(a_0; X))^s.
$$

By virtue of II, § 1, no. 13, Proposition 25, $m^{i-1}/m^i$ is a free K-module of dimension $ns_i$. Hence Proposition 1 of no. 2 can be applied with $P_i = m^{i-1}/m^i$;

this shows in the first place that $A$ is a free $K$-module of dimension $n(s_1 + \cdots + s_r) = ns$. Moreover, the hypothesis implies that the $A$-module $P_i$ is isomorphic to a direct sum of $s_i$ submodules isomorphic to the $A$-module $A_0$; by Proposition 1 of no. 2, therefore $N_{P_i}(a) = N_{A_0}(a)^{s_i}$; finally therefore
$$
N_A(a) = N_{A_0}(a)^s.
$$
In this formula $N_{A_0}(a)$ is defined by considering $A_0$ as a left $A$-module and it is equal to the determinant of the $K$-linear mapping $x \mapsto ax$ of $A_0$ into itself; but, as $ax = a_0x$ for $x \in A_0$, $N_{A_0}(a) = N_{A_0}(a_0)$, which completes the proof of formula (23) for the norm. The two others are shown analogously.

#### Proposition 6 {#alg-iii-s9-prop-6 .statement}

*Let $A$ be a commutative $K$-algebra admitting a finite basis over $K$ and $V$ an $A$-module admitting a finite basis over $A$. Then $V$ admits a finite basis over $K$ and for every $A$-endomorphism $u$ of $V$, if $u_K$ is the mapping $u$ considered as a $K$-endomorphism of $V$,*
$$
\begin{align*}
\operatorname{Tr}(u_K) &= \operatorname{Tr}_{A/K}(\operatorname{Tr}(u)), \qquad \det(u_K) = N_{A/K}(\det(u)) \\
\operatorname{Pc}(u_K; X) &= N_{A[X]/K[X]}(\operatorname{Pc}(u; X)).
\end{align*}
$$
(24)

Let $(a_i)_{1 \leq i \leq m}$ be a basis of $A$ over $K$ and $(e_j)_{1 \leq j \leq n}$ a basis of $V$ over $A$; then $(a_i e_j)$ is a basis of $V$ over $K$ (II, § 1, no. 13, Proposition 25). On the other hand the third of formulae (24) can be deduced from the second applied to the endomorphism $X - \bar{u}$ of the $A[X]$-module $A[X] \otimes_A V$ (§ 8, no. 10). It will therefore suffice to show the first two formulae in (24). We shall first establish the following lemma:

*Lemma 1. Let $X_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq n$) be $n^2$ indeterminates, $X$ the square matrix $(X_{ij})$ of order $n$ and $D(X_{11}, \ldots, X_{nn}) \in \mathbf{Z}[X_{11}, \ldots, X_{nn}]$ the determinant $\det(X)$. On the other hand let $A$ be a commutative ring, $M_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq n$) $n^2$ matrices of order $m$ over $A$, which are pairwise permutable, and $M$ the square matrix of order $mn$ over $A$ which can be expressed as a square matrix of matrices (II, § 10, no. 7)
$$
M = \begin{pmatrix}
M_{11} & M_{12} & \cdots & M_{1n} \\
M_{21} & M_{22} & \cdots & M_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
M_{n1} & M_{n2} & \cdots & M_{nn}
\end{pmatrix}
$$
Then the determinant of $M$ is equal to the determinant of the square matrix
$$
D(M_{11}, \ldots, M_{nn})
$$
of order $m$.

We proceed by induction on $n$, the cases $n = 0$ and $n = 1$ being trivial.

Let $Z$ be a new indeterminate and $N_{ij}$ the matrix $M_{ij} + \delta_{ij} Z I_m$ ($\delta_{ij}$ the Kronecker index). If $D^{ij}(X_{11}, \ldots, X_{nn})$ is the *cofactor* of $X_{ij}$ in the matrix $X$ (§ 8, no. 6), then

$$
\text{(25)} \quad X_{ji} D^{ki}(X_{11}, \ldots, X_{nn}) = \delta_{jk} D(X_{11}, \ldots, X_{nn})
$$

(§ 8, no. 6, formula (28)). We write $N'_{ij} = D^{ij}(N_{11}, \ldots, N_{nn})$, which is a square matrix of order $m$ over $\mathbf{A}[Z]$ and consider the product $N . U$, where

$$
U = \begin{pmatrix}
N'_{11} & 0 & \cdots & 0 \\
N'_{12} & I_m & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots \\
N'_{1n} & 0 & \cdots & I_m
\end{pmatrix},
$$
$$
N = \begin{pmatrix}
N_{11} & N_{12} & \cdots & N_{1n} \\
N_{21} & N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
N_{n1} & N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

Performing this product in blocks (II, § 10, no. 5) and using formulae (25), we obtain

$$
N . U = \begin{pmatrix}
P & N_{12} & \cdots & N_{1n} \\
0 & N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
0 & N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

where we have written $P = D(N_{11}, \ldots, N_{nn})$. Let

$$
Q = \begin{pmatrix}
N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots \\
N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

which is a matrix of order $m(n-1)$; then (§ 8, no. 6, formula (31)) (det $N$) (det $U$) = (det $P$)(det $Q$) and det $U = \det N'_{11}$. But by the induction hypothesis, det $Q = \det(D^{11}(N_{11}, \ldots, N_{nn})) = \det N'_{11}$ and by virtue of the definition of the $N_{ij}$, clearly det $Q$ is a polynomial in $\mathbf{A}[Z]$ of degree $m(n-1)$, whose term in $Z^{m(n-1)}$ has coefficient 1 ; it follows immediately that det $Q$ is not a divisor of zero in the graded algebra $\mathbf{A}[Z]$. We therefore conclude that det $N = \det(D(N_{11}, \ldots, N_{nn}))$ in $\mathbf{A}[Z]$; if we substitute 0 for $Z$ in these polynomials, then det $M = \det(D(M_{11}, \ldots, M_{nn}))$.

Having shown this lemma, the K-module V is the direct sum of the K-modules $Ae_j$ ($1 \leq j \leq n$); we write $u(e_j) = \sum_{k=1}^n c_{jk} e_k$. For every element $xe_j \in Ae_j$, with $x \in A$, the component of $u(xe_j)$ in $Ae_k$ is $xc_{jk} e_k$; it follows that the matrix of $u_k$ with respect to the basis $(a_i e_j)$ of the K-module V can be expressed in the form of a square matrix of matrices $(M_{jk})$, where $M_{jk}$ is the matrix of the K-linear mapping $xe_j \mapsto xc_{jk} e_k$ of $Ae_j$ into $Ae_k$ with respect to the bases $(a_i e_j)_{1 \leq i \leq m}$ and $(a_i e_k)_{1 \leq i \leq m}$ of these two K-modules (II, § 10, no. 5). If for all $t \in A$, $M(t)$ denotes the matrix, with respect to the basis $(a_i)_{1 \leq i \leq m}$ of A over K, of the endomorphism $x \mapsto xt$ of A, then $M_{jk} = M(c_{jk})$; as $t \mapsto M(t)$ is a ring homomorphism the matrices $M_{jk}$ are *permutable with one another*. Then
$$
\det u_K = \det(D(M_{11}, \ldots, M_{nn}))
$$
by Lemma 1. But as $t \mapsto M(t)$ is a ring homomorphism, $D(M_{11}, \ldots, M_{nn})$ is the matrix of the K-endomorphism $x \mapsto x.\det(c_{jk})$ of A with respect to basis $(a_i)$; by definition its determinant is therefore $N_{A/K}(\det(u))$, which proves the second formula of (24). On the other hand,
$$
\operatorname{Tr}(u_K) = \sum_{j=1}^n \operatorname{Tr}(M_{jj}) = \sum_{j=1}^n \operatorname{Tr}_{A/K}(c_{jj}) = \operatorname{Tr}_{A/K}\left( \sum_{j=1}^n c_{jj} \right) = \operatorname{Tr}_{A/K}(\operatorname{Tr}(u))
$$
and the proof of Proposition 6 is complete.

#### Corollary {#alg-iii-s9-n4-cor-1 .statement}

*Let A be a commutative K-algebra admitting a finite basis over K and B an A-algebra admitting a finite basis over A. Then B admits a finite basis over K, and, for all $b \in B$ ("transitivity formulae")*
$$
\begin{align*}
\operatorname{Tr}_{B/K}(b) &= \operatorname{Tr}_{A/K}(\operatorname{Tr}_{B/A}(b)), \quad N_{B/K}(b) = N_{A/K}(N_{B/A}(b)) \\
P_{C_{B/K}}(b; X) &= N_{A[X]/K[X]}(P_{C_{B/A}}(b; X)).
\end{align*}
$$
(26)
This follows immediately from Proposition 6, setting $V = B$ and $u(x) = bx$.

#### Remark {#alg-iii-s9-n4-rem-1 .statement}

Suppose that the homomorphism $\lambda \mapsto \lambda . 1$ of K into A is injective and let K be identified with its image in A; suppose that A admits a finite basis $(e_i)_{1 \leq i \leq n}$ as a K-module. Let s be an automorphism of A such that $s(K) = K$. Let a be an element of A; then, by transporting the structure
$$
\begin{align*}
\operatorname{Tr}_{A/K}(s(a)) &= s(\operatorname{Tr}_{A/K}(a)) \\
N_{A/K}(s(a)) &= s(N_{A/K}(a)).
\end{align*}
$$
(27) (28)
*Consider also a derivation D of A ($§ 10$, no. 2) such that $D(K) \subset K$ and write $D(e_i) = \sum_{j=1}^n e_j \mu_{ji}$ where $\mu_{ji} \in K$; write*
$$
ae_i = \sum_{j=1}^n e_j \lambda_{ji} \quad \text{with} \quad \lambda_{ji} \in K.
$$

Then
$$
D(a)e_i + aD(e_i) = D(ae_i) = \sum_{j=1}^n (D(e_j)\lambda_{ji} + e_j D(\lambda_{ji})).
$$
It follows that
$$
D(a)e_i = \sum_{j=1}^n e_j v_{ji}
$$
with $v_{ji} = D(\lambda_{ji}) + \sum_{k=1}^n (\mu_{jk}\lambda_{ki} - \lambda_{jk}\mu_{ki})$. As $\sum_{i,k} (\mu_{ik}\lambda_{ki} - \lambda_{ik}\mu_{ki}) = 0$, therefore $\operatorname{Tr}_{A/\mathbf{K}}(D(a)) = \sum_{i=1}^n D(\lambda_{ii})$, in other words
$$
\operatorname{Tr}_{A/\mathbf{K}}(D(a)) = D(\operatorname{Tr}_{A/\mathbf{K}}(a)). *
$$

### 5. DISCRIMINANT OF AN ALGEBRA

#### Definition 3 {#alg-iii-s9-def-3 .statement}

*Let A be a K-algebra admitting a finite basis of n elements. The discriminant of a sequence $(x_1, \ldots, x_n)$ of n elements of A, with respect to K, denoted by $D_{A/\mathbf{K}}(x_1, \ldots, x_n)$, is the discriminant of the square matrix*
$$
(\operatorname{Tr}_{A/\mathbf{K}}(x_i x_j))_{1 \leq i \leq n, 1 \leq j \leq n}.
$$
Consider first a basis $(e_i)_{1 \leq i \leq n}$ of A over K and write
$$
e_i e_j = \sum_{k=1}^n c_{ij k} e_k \quad \text{with} \quad c_{ij k} \in \mathbf{K}.
$$
Then $\operatorname{Tr}_{A/\mathbf{K}}(e_i) = \sum_{s=1}^n c_{iss}$, whence $\operatorname{Tr}_{A/\mathbf{K}}(e_i e_j) = \sum_{k,s} c_{ij k} c_{kss}$ and therefore
$$
D_{A/\mathbf{K}}(e_1, \ldots, e_n) = \det \left( \left( \sum_{k,s} c_{ij k} c_{kss} \right)_{1 \leq i \leq n, 1 \leq j \leq n} \right).
$$
Now let $(x_i)_{1 \leq i \leq n}, (x'_i)_{1 \leq i \leq n}$ be two sequences of n elements of A and suppose that there exists a square matrix of order n, $M = (m_{ij})$, with coefficients in K, such that $x_i = \sum_{j=1}^n m_{ij} x'_j$ for $1 \leq i \leq n$. We write
$$
T = (\operatorname{Tr}_{A/\mathbf{K}}(x_i x_j))_{1 \leq i \leq n, 1 \leq j \leq n}, \qquad T' = (\operatorname{Tr}_{A/\mathbf{K}}(x'_i x'_j))_{1 \leq i \leq n, 1 \leq j \leq n}.
$$
Then $\operatorname{Tr}_{A/\mathbf{K}}(x_i x_j) = \sum_{p,q} m_{ip} m_{jq} \operatorname{Tr}_{A/\mathbf{K}}(x'_p x'_q)$, whence $T = M \cdot T' \cdot {}^t M$; the rule of multiplication of determinants therefore gives
$$
\det T = \det M \cdot \det T' \cdot \det {}^t M = (\det M)^2 \det T'
$$
whence finally
$$
D_{A/\mathbf{K}}(x_1, \ldots, x_n) = (\det M)^2 D_{A/\mathbf{K}}(x'_1, \ldots, x'_n).
$$

The above formula shows in particular that the discriminants of two bases of A over K differ by the square of an invertible element of K and therefore generate the same (principal) ideal of K. This ideal $\Delta_{A/K}$ is called the discriminant ideal of A over K; by formula (32) the discriminant of every sequence of n elements of A which differ only in the order of the terms have the same discriminant, for the determinant of a permutation matrix is equal to $\pm 1$.

#### Example {#alg-iii-s9-n5-exa-1 .statement}

(1) If A is a quadratic algebra of type $(\alpha, \beta)$ over K, then (in the notation of § 2, no. 3) $\operatorname{Tr}(e_1) = 2, \operatorname{Tr}(e_2) = \beta$,

$$
\operatorname{Tr}(e_2^2) = \alpha \operatorname{Tr}(e_1) + \beta \operatorname{Tr}(e_2) = 2\alpha + \beta^2,
$$

whence $D_{A/K}(e_1, e_2) = \beta^2 + 4\alpha$.

(2) Let $A = K[X]/K[X]P$, where $P(X) = X^3 + pX + q$, so that if x is the image of X in A, 1, x, $x^2$ form a basis of A over K and $x^3 = -px - q$. It is seen immediately that $\operatorname{Tr}(1) = 3, \operatorname{Tr}(x) = 0, \operatorname{Tr}(x^2) = -2p$, taking account of the relation $x^3 = -px - q, \operatorname{Tr}(x^3) = -3q$ and $\operatorname{Tr}(x^4) = 2p^2$, whence easily $D_{A/K}(1, x, x^2) = -4p^3 - 27q^2$.

(3) Let A be a quaternion algebra of type $(\alpha, \beta, \gamma)$ over K and $(1, i, j, k)$ a basis of A of type $(\alpha, \beta, \gamma)$; taking account of § 3, no. 5, formula (30), it is easily found that $\operatorname{Tr}(1) = 4, \operatorname{Tr}(i) = 2\beta, \operatorname{Tr}(j) = \operatorname{Tr}(k) = 0$, then

$$
D_{A/K}(1, i, j, k) = -16\gamma^2(\beta^2 + 4\alpha)^2.
$$

(4) Let $A = M_n(K)$ and consider the canonical basis $(E_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}$ of A over K (II, § 10, no. 3). It is immediate that $\operatorname{Tr}_{A/K}(E_{ij}) = 0$ if $j \neq i$ and $\operatorname{Tr}_{A/K}(E_{ii}) = n$ for all i; it follows without difficulty that the matrix $(\operatorname{Tr}(E_{ij}E_{hk}))$ of order $n^2$ is of the form $n.P$, where P is a permutation matrix, whence $D_{A/K}((E_{ij})) = \pm n^{n^2}$.

### Exercises {#alg-iii-s9-exercises}

See the [exercises for § 9](exercises/s9/).
