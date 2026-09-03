---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 10
section_title: Matrices
lang: en
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 338-363, 417-424
pdf_pages: 0362-0387, 0441-0448
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF MATRICES
      page: 338
      pdf_page: 362
    - "no": 2
      title: MATRICES OVER A COMMUTATIVE GROUP
      page: 339
      pdf_page: 363
    - "no": 3
      title: MATRICES OVER A RING
      page: 341
      pdf_page: 365
    - "no": 4
      title: MATRICES AND LINEAR MAPPINGS
      page: 342
      pdf_page: 366
    - "no": 5
      title: BLOCK PRODUCTS
      page: 346
      pdf_page: 370
    - "no": 6
      title: MATRIX OF A SEMI-LINEAR MAPPING
      page: 347
      pdf_page: 371
    - "no": 7
      title: SQUARE MATRICES
      page: 349
      pdf_page: 373
    - "no": 8
      title: CHANGE OF BASES
      page: 352
      pdf_page: 376
    - "no": 9
      title: EQUIVALENT MATRICES; SIMILAR MATRICES
      page: 354
      pdf_page: 378
    - "no": 10
      title: TENSOR PRODUCT OF MATRICES OVER A COMMUTATIVE RING
      page: 356
      pdf_page: 380
    - "no": 11
      title: TRACE OF A MATRIX
      page: 358
      pdf_page: 382
    - "no": 12
      title: MATRICES OVER A FIELD
      page: 359
      pdf_page: 383
    - "no": 13
      title: EQUIVALENCE OF MATRICES OVER A FIELD
      page: 360
      pdf_page: 384
statements: 35
exercises: 17
content_sha256: a47679ba1ab8c0e078a09ebdfca77031eefe61db8ddab4faffc08a0fa8c19aa5
---

## § 10. MATRICES

### 1. DEFINITION OF MATRICES

#### Definition 1 {#alg-ii-s10-def-1 .statement}

Let $I, K, H$ be three sets; a matrix of type $(I, K)$ with elements in $H$ (or a matrix of type $(I, K)$ over $H$) is any family $M = (m_{i\kappa})_{(i, \kappa) \in I \times K}$ of elements of $H$ whose indexing set is the product $I \times K$. For all $i \in I$, the family $(m_{i\kappa})_{\kappa \in K}$ is called the row of $M$ of index $i$; for all $\kappa \in K$, the family $(m_{i\kappa})_{i \in I}$ is called the column of $M$ of index $\kappa$.

If $I$ (resp. $K$) is finite, $M$ is said to be a matrix with a finite number of rows (resp. columns). The set of matrices of type $(I, K)$ over $H$ is identified with the product $HI^{I \times K}$.

The names "row" and "column" arise from the fact that, in the case where $I$ and $K$ are intervals $[1, p], [1, q]$ of $\mathbf{N}$, the elements of the matrix are envisaged as set out in a rectangular array with $p$ rows (arranged horizontally) and $q$ columns (arranged vertically):

$$
\begin{pmatrix}
m_{11} & m_{12} & \cdots & m_{1q} \\
m_{21} & m_{22} & \cdots & m_{2q} \\
\cdots & \cdots & \cdots & \cdots \\
m_{p1} & m_{p2} & \cdots & m_{pq}
\end{pmatrix}
$$

When $p$ and $q$ are explicit integers sufficiently small for it to be practicable, it is a convention that the above array is a symbol effectively denoting the matrix in question; this notation enables us to dispense with the use of indices, it being understood that the indices of an element are determined by its place in the array; for example, when we speak of the matrix

$$
\begin{pmatrix}
a & b & c \\
d & e & f
\end{pmatrix}
$$

we mean the matrix $(m_{ij})_{1 \leq i < 2, 1 \leq j < 3}$ such that

$$
m_{11} = a,\ m_{12} = b,\ m_{13} = c,\ m_{21} = d,\ m_{22} = e,\ m_{23} = f.
$$

Instead of matrix of type $([1, p], [1, q])$, we also say matrix of type $(p, q)$, or matrix with $p$ rows and $q$ columns, if no confusion arises; the set of matrices of type $(p, q)$ over $H$ is sometimes denoted by $\mathbf{M}_{p, q}(H)$.

Every matrix over $H$ for which one of the indexing sets $I, K$ is empty is identical with the empty family of elements of $H$; it is also called the empty matrix. When $I = \{i_0\}$ (resp. $K = \{k_0\}$) is a set consisting of a single element, $M$ is called a row matrix (resp. column matrix) and the row (resp. column) index can then be suppressed in the notation; when $I$ and $K$ are both sets with one element, a matrix of type $(I, K)$ is often identified with the unique element in this matrix.

A subfamily $M' = (m_{\iota \kappa})_{(\iota, \kappa) \in J \times L}$ of a matrix $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$, whose indexing set is the product of a subset $J$ of $I$ and a subset $L$ of $K$, is called a *submatrix* of the matrix $M$; it is said to be obtained by *suppressing* in $M$ the rows of index $\iota \notin J$ and the columns of index $\kappa \notin L$; conversely, $M$ is said to be obtained by *bordering* $M'$ with the rows of index $\iota \notin J$ and the columns of index $\kappa \notin L$.

#### Definition 2 {#alg-ii-s10-def-2 .statement}

*The transpose of a matrix* $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$, *denoted by* $^tM$, *is the matrix* $(m'_{\kappa \iota})_{(\kappa, \iota) \in K \times I}$ *over* $H$ *given by* $m'_{\kappa \iota} = m_{\iota \kappa}$ *for all* $(\iota, \kappa) \in K \times L$.

It follows from this definition that the transpose of a matrix of type $(I, K)$ is a matrix of type $(K, I)$ and that

(1)
$$
^t(^tM) = M.
$$

### 2. MATRICES OVER A COMMUTATIVE GROUP

Let $G$ be a commutative group (written additively). The set of matrices over $G$, with the given indexing sets $I, K$, has a *commutative group* structure since it is the set of mappings from $I \times K$ to $G$; this group is written additively, so that if $M = (m_{\iota \kappa})$ and $M' = (m'_{\iota \kappa})$ are two of its elements, then
$$
M + M' = (m_{\iota \kappa} + m'_{\iota \kappa});
$$
the identity element of this group is therefore the matrix all of whose elements are *zero* (called the *zero matrix*). Clearly
(2)
$$
^t(M + M') = ^tM + ^tM'.
$$

The sum of two matrices is thus only defined if the indexing sets of the rows and the columns are the *same* for the two matrices.

Let $H', H''$ be two sets, $G$ a commutative group (written additively) and $f : (h', h'') \mapsto h'h''$ a mapping from $H' \times H''$ to $G$. Given two matrices
$$
M' = (m'_{ik})_{(i, k) \in I \times K}, \quad M'' = (m''_{kl})_{(k, l) \in K \times L}
$$
over $H'$ and $H''$ respectively such that the indexing set $K$ of the columns of $M'$ is *finite* and equal to the indexing set of the rows of $M''$, the *product of* $M'$ and $M''$ *via* $f$, denoted by $M'M''$ or $f(M', M'')$, is the matrix
(3)
$$
\left( \sum_{k \in K} m'_{ik} m''_{kl} \right)_{(i, l) \in I \times L}
$$
over $G$.

The above definition supposes that the indexing set of the columns of $M'$ is equal to the indexing set of the rows of $M''$; in particular the product $M''M'$ *has no meaning if* $I \neq L$. In formula (3) the elements of the *same* row of $M'$ figure multiplied on the right by the elements of the *same* column of $M''$; the multiplication is said to be made "rows by columns".

Let $f^0$ be the mapping $(h'', h') \mapsto h'h''$ of $H'' \times H'$ to $G$; it follows immediately from the definitions that
$$
t(M'M'') = tM''.tM'
$$
where the product on the left (resp. right) hand side is calculated via $f$ (resp. via $f^0$).

When $H'$ and $H''$ are themselves commutative groups (written additively) and $f$ is $\mathbf{Z}$-*bilinear* (§ 3, no. 1), the distributivity formulae
$$
\begin{cases}
(M' + N')M'' = M'M'' + N'M'' \\
M'(M'' + N'') = M'M'' + M'N''
\end{cases}
$$
are immediately verified, the indexing sets being such that the sums and products appearing are defined.

Now let $H_1, H_2, H_3, H_{12}, H_{23}$ and $H$ be commutative groups (written additively), $f_{12}:H_1 \times H_2 \to H_{12}, f_{23}:H_2 \times H_3 \to H_{23}$ mappings and
$$
f_3:H_{12} \times H_3 \to H, \quad f_1:H_1 \times H_{23} \to H
$$
$\mathbf{Z}$-bilinear mappings; suppose further that, for all $x_i \in H_i \ (i = 1, 2, 3)$
$$
f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))
$$
(which may also be written as above $(x_1 x_2)x_3 = x_1(x_2 x_3)$); then, if $M' = (m'_{rs}), M'' = (m''_{st}), M''' = (m'''_{tu})$ are matrices over $H_1, H_2, H_3$ respectively,
$$
(M'M'')M''' = M'(M''M'''')
$$
when the products on the two sides (calculated respectively via $f_{12}, f_3, f_{23}$ and $f_1$) are defined; for
$$
\sum_t \left( \sum_s m'_{rs} m''_{st} \right) m'''_{tu} = \sum_t \sum_s (m'_{rs} m''_{st}) m'''_{tu} = \sum_s \sum_t m'_{rs} (m''_{st} m'''_{tu})
$$
$$
= \sum_s m'_{rs} \left( \sum_t m''_{st} m'''_{tu} \right)
$$
by virtue of the hypotheses made.

The two sides of (6) are also denoted by $M'M''M'''$. Analogous conventions are made for products of more than three factors.

#### Remark {#alg-ii-s10-n2-rem-1 .statement}

The above formulae extend to a more general situation. To be precise:

(a) Suppose $H = \bigcup_{(\iota, \kappa) \in I \times K} G_{\iota \kappa}$ where each $G_{\iota \kappa}$ is a commutative group written additively; then the sum $M + M'$ may be defined when, for each ordered pair $(\iota, \kappa)$, $m_{\iota \kappa} \in G_{\iota \kappa}$ and $m'_{\iota \kappa} \in G_{\iota \kappa}$.

(b) Let I, K, L be three sets with K assumed finite and let $H' = \bigcup_{(i, k) \in I \times K} H'_{ik}$, $H'' = \bigcup_{(k, l) \in K \times L} H''_{kl}$, $H = \bigcup_{(i, l) \in I \times L} H_{il}$ be three sets; suppose that each $H_{il}$ is a commutative group written additively and for each triple $(i, k, l)$ let
$$
f_{ikl}: H'_{ik} \times H''_{kl} \to H_{il}
$$
be a mapping. Then if $M' = (m'_{ik})_{(i, k) \in I \times K}$, $M'' = (m''_{kl})_{(k, l) \in K \times L}$ are matrices such that $m'_{ik} \in H'_{ik}$ and $m''_{kl} \in H''_{kl}$ for all $i, k, l$ we can define the product $M'M''$ via the $f_{ikl}$. We leave to the reader the task of writing down and proving the formulae analogous to (4), (5) and (6).

### 3. MATRICES OVER A RING

The most important matrices in Mathematics are matrices over a ring A. The set $A^{I \times K}$ of matrices over A corresponding to indexing sets I, K then has canonically an (A, A)-bimodule structure (§ 1, no. 14).

For every ordered pair $(i, k) \in I \times K$, let $E_{ik}$ be the matrix $(a_{jl})$ such that $a_{ik} = 1$ and $a_{jl} = 0$ for $(j, l) \neq (i, k)$; the $E_{ik}$ are called the matrix units in the set of matrices $A^{I \times K}$; if I and K are finite, they form the canonical basis of this set for its left or right A-module structure (§ 1, no. 11). Clearly
$$
tE_{ik} = E_{ki}.
$$

Unless otherwise mentioned, the product $M'M''$ of two matrices over A (assumed to be defined) will always be understood to be relative to the multiplication $(x, y) \mapsto xy$ in A (or, as is also said, will be "calculated in A"). Then we have (no. 2) the associativity and distributivity formulae

(7)
$$(XY)Z = X(YZ)$$

(8)
$$
\begin{cases}
X(Y + Z) = XY + XZ \\
(X + Y)Z = XZ + YZ
\end{cases}
$$
for three matrices X, Y, Z over A, whenever the sums and products appearing in these formulae are defined.

In particular, if $E_{ik}$ (resp. $E'_{kl}, E''_{il}$) are the matrix units in $A^{I \times K}$ (resp. $A^{K \times L}, A^{I \times L}$) respectively, with $I = \{1, p\}, K = \{1, q\}, L = \{1, r\}$, we obtain the formulae
$$
\begin{cases}
E_{ik}E'_{jl} = 0 & \text{if } k \neq j \\
E_{ik}E'_{kl} = E''_{il}.
\end{cases}
$$

Let $A^0$ be the opposite ring of A and let $a * b \ (= ba)$ denote the product of a and b in $A^0$; then, for two matrices X, Y over A whose product is defined,
$$(10)$$
$$
t(XX) = tY * tX
$$

where on the right hand side $^tY$ and $^tX$ are considered as matrices with elements in $\mathbf{A}^0$; when $\mathbf{A}$ is *commutative*, then

$$(11)$$
$$
^t(XY) = ^tY.^tX
$$

#### Proposition 1 {#alg-ii-s10-prop-1 .statement}

*Let $\mathbf{A}, \mathbf{B}$ be two rings and $M = (m_{ik})_{(i,k) \in I \times K}$ and*
$$
M' = (m'_{ik})_{(i,k) \in I \times K}
$$
*two matrices with finite indexing sets over an* $(\mathbf{A}, \mathbf{B})$*-bimodule* $G$. *Suppose that for every matrix unit* $L = (a_i)_{i \in I}$ *with one row and elements in* $\mathbf{A}$ *and every matrix unit* $C = (b_k)_{k \in K}$ *with one column and elements in* $\mathbf{B}$, $L.M.C = L.M'.C$ (*the products being calculated via the external laws of the* $(\mathbf{A}, \mathbf{B})$*-module* $G$); then* $M = M'$.

If $L$ is taken to be the matrix unit $(a_s)$ with $a_i = 1, a_s = 0$ for $s \neq i$, and $C$ the matrix unit $(b_t)$ with $b_k = 1, b_t = 0$ for $t \neq k$, the products $L.M.C$ and $L.M'.C$ are matrices with a single element respectively equal to $m_{ik}$ and $m'_{ik}$.

Let $\mathbf{A}, \mathbf{B}$ be two rings and $\sigma : \mathbf{A} \to \mathbf{B}$ a homomorphism.

For every matrix $M = (m_{ik})$ over $\mathbf{A}$, we shall denote by $\sigma(M)$ the matrix $(\sigma(m_{ik}))$ over $\mathbf{B}$; clearly $\sigma(aM) = \sigma(a)\sigma(M)$, $\sigma(Ma) = \sigma(M)\sigma(a)$ for $a \in \mathbf{A}$, also $\sigma(^tM) = (^t(\sigma(M)))$ and

$$(12)$$
$$
\begin{cases}
\sigma(M + M') = \sigma(M) + \sigma(M') \\
\sigma(MM') = \sigma(M)\sigma(M')
\end{cases}
$$
*when the operations considered are defined, the products on the left and right hand sides of (12) being calculated in* $\mathbf{A}$ *and* $\mathbf{B}$ *respectively.* When $\sigma$ is denoted by $x \mapsto x^\sigma$, we write $M^\sigma$ instead of $\sigma(M)$.

Consider in particular an *anti-endomorphism* $\sigma$ of $\mathbf{A}$, that is a homomorphism of $\mathbf{A}$ to the opposite ring $\mathbf{A}^0$, or a mapping of $\mathbf{A}$ into itself such that
$$
\sigma(a + a') = \sigma(a) + \sigma(a'), \qquad \sigma(aa') = \sigma(a')\sigma(a)
$$
*for all* $a, a'$ *in* $\mathbf{A}$; then, for two matrices $M, M'$ over $\mathbf{A}$ whose product $MM'$ is defined,
$$(13)$$
$$
\sigma(MM') = (^t(\sigma(^tM')).\sigma(^tM))
$$
*where the products on the two sides are calculated in* $\mathbf{A}$; *this follows immediately from (10) and (12).*

### 4. MATRICES AND LINEAR MAPPINGS

Let $\mathbf{A}$ be a ring and $E$ a *(right or left)* $\mathbf{A}$*-module* admitting a basis $(e_i)_{i \in I}$. For every element $x \in E$, the *matrix of* $x$ *with respect to the basis* $(e_i)$, denoted by $M(x)$ or $\mathbf{x}$ (or sometimes simply $x$ when no confusion can arise), is the *column matrix* consisting of the components $x_i \ (i \in I)$ of $x$ with respect to $(e_i)$ (§ 1, no. 11); in calculations it will sometimes be convenient, in order to remember that the index $i$ is a row index, to adjoin to it a column index taking only one value and write the matrix $M(x)$ as $(x_{i0})$.

We now consider two (left or right) A-modules E and F with bases $(e_i)_{i \in I}$ and $(f_k)_{k \in K}$ respectively; let $(f_k^*)$ be the family of coordinate forms corresponding to $(f_k)$. For a linear mapping $u$ of E into F, we shall define *the matrix of u with respect to the bases* $(e_i), (f_k)$ in each of the following cases:

(D) E and F are right A-modules, $u$ is A-linear.
(G) E and F are left A-modules, $u$ is A-linear.

In what follows, we shall attach the letter (D) (resp. (G)) to formulae applying to right (resp. left) modules.

#### Definition 3 {#alg-ii-s10-def-3 .statement}

*In each of the above two cases, the matrix of u with respect to the bases* $(e_i), (f_k)$ *is the matrix* $M(u) = (u_{ki})_{(k, i) \in K \times I}$ *such that*

$$
u_{ki} = f_k^*(u(e_i))
$$

*which is written respectively as*

(14 D)
$$
u_{ki} = \langle f_k^*, u(e_i) \rangle
$$
(14 G)
$$
u_{ki} = \langle u(e_i), f_k^* \rangle.
$$

The *column* of $M(u)$ of index $i$ is therefore equal to $M(u(e_i))$.

Clearly if $u, v$ are two linear mappings of E into F and $M(u), M(v)$ their matrices with respect to the same bases, then

$$
M(u + v) = M(u) + M(v)
$$
and
$$
M(\gamma u) = \gamma M(u)
$$
for every element $\gamma$ of the *centre* $\Gamma$ of A. In other words, once the bases $(e_i), (f_k)$ are fixed, the mapping $u \mapsto M(u)$ is a *$\Gamma$-module isomorphism* of $\mathrm{Hom}_A(E, F)$ onto a subset of the set $A^{K \times I}$, equal to $A^{K \times I}$ if K is *finite*.

#### Proposition 2 {#alg-ii-s10-prop-2 .statement}

*Suppose I and K are finite. For every element* $x \in E$, *the matrix* $M(u(x))$ *with respect to the basis* $(f_k)$ *is given by the formula*

(17 D)
$$
M(u(x)) = M(u) . M(x)
$$
(17 G)
$$
{}^t M(u(x)) = {}^t M(x) . {}^t M(u).
$$

We verify for example (17 G). Let $x = \sum_i x_{i0} e_i, \quad u(x) = \sum_k y_{k0} f_k$ with $x_{i0} \in A, \ y_{k0} \in A$; then $u(x) = u\left( \sum_i x_{i0} e_i \right) = \sum_i x_{i0} u(e_i) = \sum_{i, k} x_{i0} u_{ki} f_k$; whence y_{k0} = \sum_i x_{i0} u_{ki}. In order to bring the two indices $i$ along side one another, we consider the transpose matrices ${}^t M(x) = (x'_{0i})$, where $x'_{0i} = x_{i0}$ and
$$
{}^t M(u) = (u'_{ik}),
$$
where $u'_{ik} = u_{ki}$; then $y_{k0} = \sum_i x'_{0i} u'_{ik}$ and the right hand side is the element of index $k$ of the matrix with one row ${}^t M(x) \cdot {}^t M(u)$, whence (17 G).

When A is commutative, (17 G) reduces to (17 D) by formula (4) of no. 2.

#### Corollary {#alg-ii-s10-n4-cor-1 .statement}

*Let E, F, G be three right (resp. left) modules over a ring A, $(e_i)_{i \in I}$, $(f_k)_{k \in K}$, $(g_l)_{l \in L}$ respective finite bases of E, F, G, $u : E \to F$, $v : F \to G$ two linear mappings, $M(u)$ the matrix of u relative to the bases $(e_i)$, $(f_k)$, $M(v)$ the matrix of v relative to the bases $(f_k)$, $(g_l)$ and $M(v \circ u)$ the matrix of $v \circ u$ relative to the bases $(e_i)$, $(g_l)$; then*

(18 D)
$$
M(v \circ u) = M(v) M(u)
$$
(18 G)
$$
{}^t M(v \circ u) = {}^t M(u) {}^t M(v).
$$

We prove for example (18 G). For all $x \in E$, by (17 G):
$$
{}^t M(x) \cdot {}^t M(v \circ u) = {}^t M(v(u(x))) = {}^t M(u(x)) \cdot {}^t M(v) = {}^t M(x) \cdot {}^t M(u) \cdot {}^t M(v)
$$
by associativity; the corollary then follows from no. 3, Proposition 1 since the matrix ${}^t M(x)$ with one row is arbitrary.

*Remark (1)*. Formula (17 D) can be considered as a special case of (18 D). For there corresponds canonically to every $x \in E$ the linear mapping $\theta_x : A_d \to E$ mapping every $\alpha \in A$ to $x \alpha$ (§ 2, no. 1). It is immediate that the matrix $M(\theta_x)$ with respect to the basis 1 of $A_d$ and the basis $(e_i)$ of E is just the matrix $M(x)$; similarly $M(\theta_{u(x)}) = M(u(x))$ and formula (17 D) can therefore be considered as a translation of the relation
$$
\theta_{u(x)} = u \circ \theta_x.
$$

#### Proposition 3 {#alg-ii-s10-prop-3 .statement}

*Let E, F be two right (resp. left) A-modules and $(e_i)_{i \in I}$, $(f_k)_{k \in K}$ finite bases of E and F respectively. For every linear mapping u of E into F, let $M(u)$ be the matrix of u with respect to the bases $(e_i)$ and $(f_k)$. Then the matrix of ${}^t u : F^* \to E^*$ with respect to the dual bases $(f_k^*)$ and $(e_i^*)$ is equal to ${}^t M(u)$.*

E is canonically identified with its bidual $E^{**}$ and $(e_i)$ with the dual basis of $(e_i^*)$; then (supposing for example that E and F are right modules)
$$
\langle {}^t u(f_k^*), e_i \rangle = \langle f_k^*, u(e_i) \rangle,
$$
whence the proposition.

#### Remark {#alg-ii-s10-n4-rem-1 .statement}

(2) Let E and F be two left A-modules with bases $(e_i)_{i \in I}$ and $(f_k)_{k \in K}$ respectively. For every A-linear mapping $u : E \to F$, by (14 G), $u(e_i) = \sum_k u_{ki} f_k$; these relations can also be interpreted by saying that the column matrix $(u(e_i))_{i \in I}$ with elements in F is equal to the product $^tM(u) \cdot (f_k)$, where $(f_k)_{k \in K}$ is considered as a column matrix with elements in F and the product is calculated for the mapping $A \times F \to F$ defining the law of action on the A-module F (no. 2).

(3) Let A, B be two commutative rings and $\sigma : A \to B$ a ring homomorphism. In the notation of Proposition 3, $(e_i \otimes 1)$ and $(f_k \otimes 1)$ are respective bases of $E_{(B)} = E \otimes_A B$ and $F_{(B)} = F \otimes_A B$ (§ 5, no. 1, Proposition 4); moreover, if $(e_i^*)$ and $(f_k^*)$ are respectively the dual bases of $(e_i)$ and $(f_k)$, then $(e_i^* \otimes 1)$ and $(f_k^* \otimes 1)$ are respectively the dual bases of $(e_i \otimes 1)$ and $(f_k \otimes 1)$ (§ 5, no. 4). For every A-linear mapping $u : E \to F$, let $M(u)$ and $M(u \otimes 1)$ be the matrix of $u$ with respect to $(e_i)$ and $(f_k)$ and the matrix of the B-linear mapping $u \otimes 1$ with respect to $(e_i \otimes 1)$ and $(f_k \otimes 1)$. It follows from § 5, no. 4, formula (20) that
$$
M(u \otimes 1) = \sigma(M(u)).
$$

Consider a system of a finite number of right scalar linear equations in a finite number of unknowns
$$
\sum_{i \in I} a_{kt} x_i = b_k \quad (k \in K)
$$
with $a_{kt}, x_i, b_k$ in A.

Let $(e_i)_{i \in I}, (f_k)_{k \in K}$ be the canonical bases of $E = A_d^I$ and $F = A_d^K$; the system (19) is equivalent to the equation $u(x) = b$, where $x = \sum_i e_i x_i$, $b = \sum_k f_k b_k$ and $u : E \to F$ is the linear mapping such that the matrix $M(u)$ with respect to the bases $(e_i)$ and $(f_k)$ are equal to $A = (a_{kt})_{(k, i) \in K \times L}$. This matrix is called the matrix of the system of linear equations (19). Recall (§ 2, no. 8, Remarks 2 and 3), that, writing $c_i = \sum_k f_k a_{kt}$, the system (19) is equivalent to the unique vector equation
$$
\sum_i c_i x_i = b,
$$
and as $c_i$ is the column of index $i$ in the matrix $A$, we see that to say that the system (19) admits a solution amounts to saying that the matrix $b = (b_{k0})$ with one column is a linear combination of the columns of the matrix $A$.

We leave to the reader the task of formulating the analogous definitions and remarks for systems of left linear equations.

### 5. BLOCK PRODUCTS

The definitions of no. 4 can be generalized as follows. Let E be a (right or left) A-module, the direct sum of a family $(E_i)_{i \in I}$ of submodules. For all $x \in E$, let $x = \sum_{i \in I} x_i$ with $x_i \in E_i$ for all $i \in I$; we shall say that the column matrix $M(x) = (x_i)_{i \in I}$ with elements in E is *the matrix of x with respect to the decomposition $(E_i)_{i \in I}$ of E as a direct sum*.

Let F be another A-module (E and F being both right A-modules or both left A-modules) and suppose that F is the direct sum of a family $(F_k)_{k \in K}$ of submodules. For all $u \in \mathrm{Hom}(E, F)$ and all $x_i \in E_i$, let $u(x_i) = \sum_k u_{ki}(x_i)$ with $u_{ki}(x_i) \in F_k$ for all $k \in K$; then $u_{ki} \in \mathrm{Hom}(E_i, F_k)$; we shall say that the matrix $M(u) = (u_{ki})_{(k, i) \in K \times I}$ of type $(K, I)$ with elements in the set H the sum of the $\mathrm{Hom}(E_i, F_k)$ is *the matrix of u with respect to the decompositions $(E_i)$ and $(F_k)$ of E and F as direct sums*.

With these definitions, it is obvious that if $u, v$ are two A-linear mappings of E into F then, for matrices with respect to the same decompositions as direct sums

$$
M(u + v) = M(u) + M(v), \qquad M(\gamma u) = \gamma M(u)
$$

for every element $\gamma$ of the centre of A (no. 2, *Remark*).

Moreover, the definition of the $u_{ki}$ shows that, if K is finite, we can write

$$
M(u(x)) = M(u) . M(x)
$$

where $M(u(x))$ is the matrix of $u(x)$ with respect to the decomposition $(F_k)$, the product on the right hand side of (22) being calculated for the mappings $(t, z) \mapsto t(z)$ of $\mathrm{Hom}(E_i, F_k) \times E_i$ into $F_k$ (no. 2, *Remark*).

Let G be a third A-module, the direct sum of a family $(G_l)_{l \in L}$ of submodules, so that there corresponds to every A-linear mapping $v : F \to G$ a matrix $M(v) = (v_{lk})$ with respect to the decompositions $(F_k)$ and $(G_l)$. If I, K and L are *finite*, then

$$
M(v \circ u) = M(v) . M(u)
$$

where the left hand side is the matrix $(w_{li})$ of $w = v \circ u$ with respect to the decomposition $(E_i)$ and $(G_l)$ and the product on the left hand side is calculated for the mappings $(t, s) \mapsto t \circ s$ of $\mathrm{Hom}(F_k, G_l) \times \mathrm{Hom}(E_i, F_k)$ into $\mathrm{Hom}(E_i, G_l)$ (no. 2, *Remark*). This is just formula (32) of § 1, no. 8, expressed in terms of matrices.

Finally, if I and K are assumed to be finite, $E^*$ (resp. $F^*$) is canonically identified with the direct sum of the modules $E_i^*$ (resp. $F_k^*$) (§ 2, no. 6, Proposition 10). Then it is immediately verified that the matrix of $^t u$ with respect to the decompositions $(F_k^*)$ and $(E_i^*)$ is just $(^t u_{ki})_{(k, i) \in K \times I}$.

Suppose now that I and K are finite and further that each of the E_i (resp. F_k) admits a finite basis. It amounts to the same to say that E (resp. F) admits a basis (e_r)_{r \in R} (resp. (f_s)_{s \in S}) and that R (resp. S) admits a partition (R_i)_{i \in I} (resp. (S_k)_{k \in K}) such that for all i \in I (resp. k \in K), (e_r)_{r \in R_i} is a basis of E_i (resp. (f_s)_{s \in S_k} is a basis of F_k). Then, if X = M(u) is the matrix of u with respect to the bases (e_r)_{r \in R} and (f_s)_{s \in S}, the matrix X_{kt} = M(u_{kt}) with respect to the bases (e_r)_{r \in R_i} and (f_s)_{s \in S_k} is just the submatrix of X obtained by suppressing the rows of index s \notin S_k and the columns of index r \notin R_i. Thus we define a one-to-one correspondence

$$
X \mapsto (X_{kt})_{(k, t) \in K \times I}
$$

between the set of matrices of type (S, R) with elements in A and the set of matrices of matrices $(X_{kt})_{(k, t) \in K \times I}$ of type K \times I, where each X_{kt} is a matrix over A of type (S_k, R_i). Suppose that further G admits a finite basis (g_t)_{t \in T} and that T = (T_l)_{l \in L} is a partition of T such that, for each l \in L, (g_t)_{t \in T_l} is a basis of G_l; let Y = M(v) be the matrix of v with respect to the bases (f_s)_{s \in S} and (g_t)_{t \in T}, Y_{lk} = M(v_{lk}) that of v_{lk} with respect to the bases (f_s)_{s \in S_k} and (g_t)_{t \in T_l}, Z = M(w) the matrix of w = v \circ u with respect to the bases (e_r)_{r \in R} and (g_t)_{t \in T} and Z_{li} = M(w_{li}) that of w_{li} with respect to the bases (e_r)_{r \in R_i} and (g_t)_{t \in T_l}; then it follows from (23) that the submatrices Z_{li} of Z = YX are given by

$$
Z_{li} = \sum_k Y_{lk} X_{kt}
$$

in other words, the one-to-one correspondence (24) transforms products into products when all the products in question are defined (products of matrices of matrices being defined in the sense of no. 2, Remark); when the submatrices Z_{li} of the product YX are calculated thus, this product is said to be carried out "in blocks".

This name arises from the fact that, when I = {1, p} and K = {1, q}, the table representing the matrix X is envisaged as divided into "blocks" forming an "array of matrices"

$$
\begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
X_{21} & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
X_{q1} & X_{q2} & \ldots & X_{qp}
\end{pmatrix}
$$

which is considered as a symbol denoting X when p and q are specific integers sufficiently small for this to be practicable.

### 6. MATRIX OF A SEMI-LINEAR MAPPING

Let A, B be two rings, \sigma : A \to B a homomorphism of A into B, E a right (resp. left) A-module with basis (e_i)_{i \in I} and F a right (resp. left) B-module with basis $(f_k)_{k \in K}$. Let $u : E \to F$ be a *semi-linear* mapping relative to $\sigma$ and $u(e_i) = \sum_{k \in K} f_k u_{ki}$ (resp. $u(e_i) = \sum_{k \in K} u_{ki} f_k$), where the $u_{ki}$ are therefore elements of B; by definition, the matrix $M(u) = (u_{ki})$ of type $K \times I$ is also called the *matrix of u with respect to the bases* $(e_i)$ and $(f_k)$. By the same calculation as in Proposition 2 of no. 4, it is immediately verified that for all $x \in E$, if I and K are *finite*,

(26 D)
$$
M(u(x)) = M(u) \cdot \sigma(M(x))
$$
(resp.

(26 G)
$$
{}^t M(u(x)) = \sigma({}^t M(x)) \cdot {}^t M(u)).
$$

Let C be a third ring, $\tau : B \to C$ a homomorphism, G a right (resp. left) C-module with basis $(g_l)_{l \in L}$ and $v$ a semi-linear mapping of F into G relative to $\tau$; if $M(v)$ is the matrix of $v$ with respect to $(f_k)$ and $(g_l)$ and $M(v \circ u)$ the matrix of $v \circ u$ relative to $(e_i)$ and $(g_l)$, then, if I, K and L are finite,

(27 D)
$$
M(v \circ u) = M(v) \cdot \tau(M(u))
$$
(resp.

(27 G)
$$
{}^t M(v \circ u) = \tau({}^t M(u)) \cdot {}^t M(v)).
$$

To show for example (27 D), note that for all $x \in E$, by (26 D),
$$
M(v \circ u) \cdot \tau(\sigma(M(x))) = M(v(u(x)))
$$
$$
= M(v) \cdot \tau(M(u(x))) = M(v) \cdot \tau(M(u)) \cdot \tau(\sigma(M(x))),
$$
whence (27 D) by Proposition 1 of no. 3.

Suppose finally that $\sigma : A \to B$ is an *isomorphism*; then recall that ${}^t u : F^* \to E^*$ is a semi-linear mapping relative to $\sigma^{-1}$ (§ 2, no. 5); when I and K are finite, the matrix ${}^t u$ with respect to the dual bases $(f_k^*)$ and $(e_i^*)$ is given by

(28)
$$
M({}^t u) = \sigma^{-1}({}^t M(u))
$$
for, by definition, supposing for example that E and F are right modules,
$$
\langle {}^t u(f_k^*), e_i \rangle^\sigma = \langle f_k^*, u(e_i) \rangle
$$
when $\sigma$ is denoted by $x \mapsto x^\sigma$.

#### Remark {#alg-ii-s10-n6-rem-1 .statement}

Let A be a ring and $\sigma$ an *anti-endomorphism* of A (no. 3); consider the two following situations:

(GD) E is a left A-module, F a right A-module and $u$ a $\mathbf{Z}$-linear mapping of E into F such that $u(ax) = u(x)\sigma(a)$ for $a \in A,\ x \in E$; in other words, $u$ is a *semi-linear* mapping relative to $\sigma$ of the right $A^0$-module E into the right A-module F.

(DG) E is a right A-module, F a left A-module and $u$ a $\mathbf{Z}$-linear mapping of E into F such that $u(xa) = \sigma(a)u(x)$ for $a \in A,\ x \in E$; in other words, $u$ is a *semi-linear* mapping relative to $\sigma$ of the left $A^0$-module E into the left A-module F.

In the two cases, the matrix $M(u)$ of $u$ relative to bases of E and F has its elements in A; if these bases are finite, then, for all $x \in E$, we have the respective formulae

(17 GD) $$
M(u(x)) = M(u) . \sigma(M(x))
$$
(17 DG) $$
{}^t M(u(x)) = \sigma({}^t M(x)) . {}^t M(u),
$$
the products on the two sides being calculated *in* A. This follows immediately from (26 D) and (26 G) respectively.

### 7. SQUARE MATRICES

#### Definition 4 {#alg-ii-s10-def-4 .statement}

*A matrix whose rows and columns have the same indexing set is called a square matrix.*

A square matrix with $n$ rows and $n$ columns is called a *matrix of order* $n$.

#### Remark {#alg-ii-s10-n7-rem-1 .statement}

It should be noted that a matrix for which the indexing sets of the rows and columns have the *same cardinal* but *are not identical*, must not be considered as a square matrix; in particular, the product of two such matrices over a ring *is not defined*.

Clearly addition and multiplication of square matrices over A with a finite set as indexing set of the rows and columns, define on the set of these matrices a *ring* structure because of formulae (7), (8) and (9) (no. 3); the matrix $(\delta_{ij})$, where $\delta_{ij}$ is the Kronecker index (for $i \in I, j \in I$), is the unit element of this ring and is denoted by $I_n$ or $l_n$ when I has $n$ elements. When $I = \{1, n\}$, the ring of matrices thus defined is denoted simply by $\mathbf{M}_n(A)$; the group of invertible elements of $\mathbf{M}_n(A)$ is denoted by $\mathbf{GL}_n(A)$ or $\mathbf{GL}(n, A)$.

For a square matrix $U = (a_{ij})$ of order $n$ over A to be right (resp. left) invertible, it is necessary and sufficient that, for every system $(b_i)_{1 \leq i \leq n}$ of elements of A, the system of $n$ equations in $n$ unknowns

$$
\sum_{j=1}^n a_{ij} x_j = b_i \quad (1 \leq i \leq n)
$$

(resp. $\sum_{j=1}^n x_j a_{ji} = b_i$)

have *one solution* $(x_i)$ in A.

Let I be a finite indexing set, A a ring and E a right (resp. left) A-module with basis $(e_i)_{i \in I}$. For every *endomorphism* $u$ of E, the matrix $M(u)$ of $u$ with respect to the *two bases identical with* $(e_i)$ is a square matrix; more briefly, it is called the matrix of $u$ *with respect to the basis* $(e_i)$.

Suppose that $I = \{1, n\}$. The mapping $u \mapsto M(u)$ (resp. $u \mapsto {}^t M(u)$) is an *isomorphism* of the ring $\mathrm{End}_A(E)$ onto $\mathbf{M}_n(A)$ (resp. onto the opposite ring of $\mathbf{M}_n(A)$, as follows from formulae (18 D) (resp. 18 G)) (no. 4). The invertible elements of the ring $\mathbf{M}_n(\mathbf{A})$ called *invertible matrices*, correspond under the mapping $u \mapsto M(u)$ (resp. $u \mapsto {}^t M(u)$) to the *automorphisms* of E; the group $\mathbf{GL}(n, \mathbf{A})$ is therefore canonically identified with the group $\mathbf{GL}(\mathbf{A}_d^n)$.

If $u$ is an automorphism of E, its *contragredient* $\check{u}$ is an automorphism of the left (resp. right) A-module $E^*$, such that $\check{u} = ({}^t u)^{-1} = {}^t (u^{-1})$ (§ 2, no. 5, Definition 6); if $M(\check{u})$ is the matrix of $\check{u}$ with respect to the dual basis $(e_i^*)$, then, by virtue of Proposition 3 (no. 4),

$$
M(\check{u}) = ({}^t M(u))^{-1} = {}^t M(u^{-1}).
$$

For every invertible matrix $X$, it therefore follows that ${}^t (X^{-1}) = ({}^t X)^{-1}$; this matrix is also denoted by ${}^t X^{-1}$ and called the *contragredient* of the matrix $X$.

Let $\sigma$ be an *automorphism* of the ring $\mathbf{A}$; for every *semi-linear* mapping $u : E \to E$ relative to $\sigma$, the matrix $M(u)$ of this mapping with respect to a basis $(e_i)$ of E is also a square matrix. It follows immediately from (27 D) (no. 6) that, if $u$ is bijective, then

$$
M(u^{-1}) = (\sigma^{-1}(M(u)))^{-1}.
$$

Let E be an A-module which is the *direct sum* of a finite family $(E_i)_{i \in I}$ of submodules; for every endomorphism $u$ of E, the matrix $M(u) = (u_{ki})$ of $u$ with respect to the two decompositions of E identical with $(E_i)$ (no. 5) is a *square matrix of linear mappings*. In order that $u(E_i) \subset E_i$ for all $i \in I$, it is necessary and sufficient that $u_{ki} = 0$ for $k \neq i$. When $I = \{1, n\}$, the relations

$$
u(E_i) \subset E_i + E_{i+1} + \cdots + E_n \qquad (1 \leq i \leq n)
$$

are equivalent to the relations $u_{ki} = 0$ for $k < i$.

*Examples of square matrices.* I. *Diagonal matrices*. In a square matrix

$$
M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times I},
$$

the elements both of whose indices are equal are called *diagonal elements* and the family $(m_{\iota \iota})_{\iota \in I}$ is called the *diagonal* of $M$; a square matrix $M = (m_{\iota \kappa})$ over a ring, whose elements other than the diagonal elements are zero, is called a *diagonal matrix*. For every family $(a_\iota)_{\iota \in I}$ of elements of a ring $\mathbf{A}$, the diagonal matrix $(m_{\iota \kappa})$ such that $m_{\iota \iota} = a_\iota$ for all $\iota \in I$ is denoted by $\operatorname{diag}(a_\iota)_{\iota \in I}$ (or $\operatorname{diag}(a_1, a_2, \ldots, a_n)$ when $I = \{1, n\}$). In the set $\mathbf{M}_n(\mathbf{A})$ of square matrices of order $n$ over $\mathbf{A}$, the unit matrix $I_n$ is a diagonal matrix and also every multiple $a I_n = I_n a$ of this matrix by a scalar $a$ (the diagonal matrix (called *scalar*) all of whose diagonal elements are equal to $a$).

For every family $(d_i)_{1 \leq i \leq n}$ of elements of $\mathbf{A}$ and every matrix $X = (x_{ij})$ of type $(n, q)$ (resp. $(p, n)$) over $\mathbf{A}$, writing $D = \operatorname{diag}(d_i)$,

$$
\begin{cases}
DX = (d_i x_{ij}) \\
XD = (x_{ij} d_j).
\end{cases}
$$

In particular, for two diagonal matrices of order $n$,

$$
\text{diag}(a_i) + \text{diag}(b_i) = \text{diag}(a_i + b_i)
$$
(31)
$$
\text{diag}(a_i) \cdot \text{diag}(b_i) = \text{diag}(a_i b_i).
$$

The diagonal matrices therefore form a subring of $\mathbf{M}_n(\mathbf{A})$ isomorphic to the product ring $\mathbf{A}^n$; the scalar matrices form a subring isomorphic to $\mathbf{A}$.

II. *Permutation matrices; monomial matrices.* Let $\pi$ be any *permutation* of a finite set $\mathbf{I}$ and let $(e_i)_{i \in \mathbf{I}}$ be the canonical basis of the $\mathbf{A}$-module $\mathbf{E} = \mathbf{A}_d^\mathbf{I}$; there exists one and only one endomorphism $u_\pi$ of $\mathbf{E}$ such that, for all $i \in \mathbf{I}$, $u_\pi(e_i) = e_{\pi(i)}$ (§ 1, no. 11, Corollary 3 to Proposition 17). For all $i \in \mathbf{I}$, the column of index $i$ in the matrix $M(u_\pi)$ with respect to the basis $(e_i)$ has all its elements zero except the one in the row of index $\pi(i)$, which is equal to 1. By an abuse of language, $M(u_\pi)$ is called *the matrix of the permutation* $\pi$. It is immediate that for any two permutations $\sigma, \tau$ of $\mathbf{I}$, $u_{\sigma \tau} = u_\sigma \circ u_\tau$ and that for the identity permutation $\varepsilon$, $u_\varepsilon$ is the identity; the mapping $\pi \mapsto M(u_\pi)$ is therefore an *isomorphism* of the symmetric group $\mathfrak{S}_\mathbf{I}$ onto the group of permutation matrices.

Each row and each column of a permutation matrix contains only a single element $\neq 0$. A finite square matrix $R$ over a non-zero ring $\mathbf{A}$, with this property, is called a *monomial matrix*; let $r_i$ be the unique element $\neq 0$ in the column of $R$ of index $i$ and let $\pi(i)$ be the index of the row where this element is; clearly $\pi$ is a permutation of the indexing set $\mathbf{I}$ and $R = M(u_\pi)D$, where $D = \text{diag}(r_i)$.

III. *Triangular matrices.* In the ring $\mathbf{M}_n(\mathbf{A})$ of square matrices of order $n$ over a ring $\mathbf{A}$, any matrix $(a_{ij})$ such that $a_{ij} = 0$ for $i > j$ (resp. $i < j$) is called an *upper* (resp. *lower*) *triangular matrix*; it is also said that such a matrix *has only zeros below* (resp. *above*) *its diagonal*. It is immediately established that the upper (resp. lower) triangular matrices form a subring $S$ (resp. $T$) of $\mathbf{M}_n(\mathbf{A})$, $S \cap T$ being obviously the ring of diagonal matrices.

The set $S'$ (resp. $T'$) of matrices in $S$ (resp. $T$) whose diagonal elements are *invertible* is a multiplicative *group* of matrices called the *upper* (resp. *lower*) *total triangular group*, this follows immediately from § 1, no. 11, *Remark* 5. The set $S_1$ (resp. $T_1$) of matrices in $S$ (resp. $T$) whose diagonal elements are all equal to 1 is a *subgroup* of the above group, called the *upper* (resp. *lower*) *strict triangular group*, and every matrix $M \in S'$ (resp. $M \in T'$) whose diagonal is $(d_i)$, may be written as $M = DM_1 = M'_1D$, where $D = \text{diag}(d_i)$ and $M_1$ and $M'_1$ matrices belonging to $S_1$ (resp. $T_1$).

IV. *Diagonal and triangular matrices of matrices.* Let $(I_k)_{1 \leq k \leq p}$ be a partition of the finite set $\mathbf{I}$; every square matrix over a ring $\mathbf{A}$ with indexing set $\mathbf{I}$ can be written in the form of a *square matrix of matrices* corresponding to the same partition $(\mathbf{I}_k)$ of the indexing set of the rows and the indexing set of the columns (no. 5)

$$
(32)
\begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
X_{21} & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
X_{p1} & X_{p2} & \ldots & X_{pp}
\end{pmatrix}
$$

where each $X_{kk}$ is a square matrix with $\mathbf{I}_k$ as indexing set of the rows and columns.

With this notation, (32) will be called a diagonal (resp. upper triangular, resp. lower triangular) matrix of matrices if all the matrices $X_{ij}$ such that $i \neq j$ (resp. $i > j$, resp. $i < j$) are zero. The interpretation of endomorphisms $u$ whose matrix is a diagonal, resp. triangular, matrix of matrices has been seen earlier, by considering the corresponding matrix $M(u)$ of linear mappings. The lower triangular (resp. upper triangular, diagonal) matrices of matrices for a given partition $(\mathbf{I}_k)$ of I form subrings of the ring of matrices $\mathbf{A}^{I \times I}$. In particular, the ring of diagonal matrices of matrices relative to the partition $(\mathbf{I}_k)$ is isomorphic to the product $\prod_{k=1}^p \operatorname{End}_\mathbf{A}(E_k)$.

### 8. CHANGE OF BASES

#### Proposition 4 {#alg-ii-s10-prop-4 .statement}

*Let E be a right A-module with finite basis $(e_i)_{1 \leq i \leq n}$ of n elements. For a family of n elements $e'_i = \sum_{j=1}^n e_j a_{ji} (1 \leq i \leq n)$ to be a basis of E, it is necessary and sufficient that the square matrix $P = (a_{ji})$ of order n be invertible.*

$P$ is just the matrix, with respect to the basis $(e_i)$ of the endomorphism $u$ of E defined by $u(e_i) = e'_i (1 \leq i \leq n)$. Now, for $u$ to be an automorphism of E, it is necessary and sufficient that $(u(e_i))$ be a basis of E (§ 1, no. 11, Corollary 3 to Proposition 17); whence the proposition.

The invertible matrix $P$ is called the *matrix of passage from the basis* $(e_i)$ *to the basis* $(e'_i)$. It can also be interpreted as the matrix of the identity mapping $l_E$ with respect to the bases $(e'_i)$ and $(e_i)$ (*in that order*); then clearly the matrix of passage *from the basis* $(e'_i)$ *to the basis* $(e_i)$ is the *inverse* $P^{-1}$ of $P$.

#### Proposition 5 {#alg-ii-s10-prop-5 .statement}

*Let $(e_i), (e'_i)$ be two bases of n elements of E and P the matrix of passage from $(e_i)$ to $(e'_i)$. If $(e_i^*)$ and $({e'_i}^*)$ are the respective dual bases of $(e_i)$ and $(e'_i)$, the matrix of passage from $(e_i^*)$ to $({e'_i}^*)$ is the contragredient $^tP^{-1}$ of P.*

The transpose of the identity mapping $l_E$ is the identity mapping $l_{E^*}$; by Proposition 3, no. 4, the matrix of $l_{E^*}$ with respect to the bases $({e'_i}^*)$ and $(e_i^*)$ (in that order) is the transpose of the matrix of $l_E$ with respect to the bases $(e_i)$ and $(e'_i)$ (in that order), that is the transpose of $P^{-1}$.

#### Proposition 6 {#alg-ii-s10-prop-6 .statement}

*Let E and F be two right A-modules, $(e_i)$ and $(e'_i)$ two bases of E* with $n$ elements, $(f_j)$ and $(f'_j)$ two bases of $F$ with $m$ elements, $P$ the matrix of passage from $(e_i)$ to $(e'_i)$ and $Q$ the matrix of passage from $(f_j)$ to $(f'_j)$. For every linear mapping $u$ of $E$ into $F$, let $M(u)$ be the matrix of $u$ with respect to the bases $(e_i)$ and $(f_j)$ and $M'(u)$ the matrix of $u$ with respect to the bases $(e'_i)$ and $(f'_j)$; then

$$
M'(u) = Q^{-1} M(u) P.
$$

We may write $u = l_F \circ u \circ l_E$. Formula (33) follows immediately from no. 4, Corollary to Proposition 2 when the matrix of $l_E$ is taken with respect to $(e'_i)$ and $(e_i)$, that of $u$ with respect to $(e_i)$ and $(f_i)$ and that of $l_F$ with respect to $(f_i)$ and $(f'_j)$.

#### Corollary 1 {#alg-ii-s10-prop-6-cor-1 .statement}

*If $u$ is an endomorphism of $E$ and $M(u)$ and $M'(u)$ its matrices with respect to the bases $(e_i)$ and $(e'_i)$ respectively, then*

$$
M'(u) = P^{-1} M(u) P.
$$

#### Corollary 2 {#alg-ii-s10-prop-6-cor-2 .statement}

*If $M(x)$ and $M'(x)$ are the matrices with one column of the same element $x \in E$ with respect to the bases $(e_i)$ and $(e'_i)$ respectively, then*

$$
M(x) = P . M'(x).
$$

This is a special case of Proposition 6, applied to the mapping $\theta_x : a \mapsto xa$ of $A_d$ to $E$ (no. 4, *Remark 1*).

Formula (35) is equivalent to

$$
x_i = \sum_{j=1}^n a_{ij} x'_j \quad (1 \leq i \leq n)
$$

for the elements $x_i$ and $x'_i$ of the matrices $M(x)$ and $M'(x)$ respectively. Formulae (36 D) are called *formulae of change of coordinates*. Observe that they express the components of $x$ relative to the "old" basis $(e_i)$ as functions of the components of $x$ relative to the "new" basis $(e'_i)$ and the elements of $P$, that is the components of the "new" basis relative to the "old" basis.

#### Remark {#alg-ii-s10-n8-rem-1 .statement}

(1) We now start with a *left* $A$-module $E$ with two bases $(e_i), (e'_i)$, each with $n$ elements; if we write $e'_i = \sum_{j=1}^n a_{ji} e_i$, $P = (a_{ji})$ is also called the *matrix of passing* from $(e_i)$ to $(e'_i)$; it is also the matrix of the automorphism of $E$ such that $u(e_i) = e'_i$, with respect to the basis $(e_i)$ and also the matrix of $l_E$ with respect to the bases $(e'_i)$ and $(e_i)$ *in that order*. The above results then hold with only the following modifications: formulae (33 D) to (36 D) are respectively replaced by

$$
\begin{align*}
(33\text{ G}) &\quad {}^t M'(u) = {}^t P . {}^t M(u) . {}^t Q^{-1} \\
(34\text{ G}) &\quad {}^t M'(u) = {}^t P . {}^t M(u) . {}^t P^{-1} \\
(35\text{ G}) &\quad {}^t M(u) = {}^t M'(u) . {}^t P.
\end{align*}
$$

LINEAR ALGEBRA

(36 G)
$$
x_i = \sum_{j=1}^n x_j' a_{ij} \quad (1 \leq i \leq n).
$$

(2) Under the hypotheses of Proposition 4, consider an element $x^* \in \mathbf{E}^*$; as the matrix of passage from $(e_i^*)$ to $(e_{i'}^*)$ is $tP^{-1}$ (Proposition 5), for the matrices $M(x^*)$ and $M'(x^*)$ of $x^*$ with respect to these two bases respectively,

$$
tM(x^*) = tM'(x^*) . P^{-1}
$$

or also

(37 D)
$$
tM'(x^*) = tM(x^*) . P
$$

which is equivalent to the system of equations

(38 D)
$$
x_{i'}^* = \sum_{j=1}^n x_j^* a_{ji} \quad (1 \leq i \leq n)
$$

for the elements $(x_i^*)$ and $(x_{i'}^*)$ of the matrices $M(x^*)$ and $M'(x^*)$. The corresponding formulae for a left A-module E are

(37 G)
$$
M'(x^*) = tP . M(x^*)
$$

(38 G)
$$
x_{i'}^* = \sum_{j=1}^n a_{ji} x_j^* \quad (1 \leq i \leq n).
$$

(3) Let A, B be two rings, $\sigma : A \to B$ a homomorphism of A into B, E a right (resp. left) A-module, $(e_i)$, $(e_i')$ two bases with $n$ elements of E, F a right (resp. left) B-module, $(f_j)$, $(f_j')$ two bases with $m$ elements of F and $P$ (resp. $Q$) the matrix of passage from $(e_i)$ to $(e_i')$ (resp. from $(f_j)$ to $(f_j')$).

For every semi-linear mapping $u : E \to F$, relative to $\sigma$, let $M(u)$ be the matrix of $u$ with respect to $(e_i)$ and $(f_j)$ and $M'(u)$ its matrix with respect to $(e_i')$ and $(f_j')$. Then

(39 D)
$$
M'(u) = Q^{-1} M(u) \sigma(P)
$$
(resp.
(39 G)
$$
tM'(u) = \sigma(tP) . tM(u) . tQ^{-1}.
$$

The proof is the same as that for (33 D) and (33 G), this time using formulae (27 D) and (27 G) (no. 6).

### 9. EQUIVALENT MATRICES; SIMILAR MATRICES

#### Definition 5 {#alg-ii-s10-def-5 .statement}

*Two matrices* $X, X'$ *with m rows and n columns over a ring are called equivalent if there exists an invertible square matrix* $P$ *of order m and an invertible square matrix* $Q$ *of order n such that*

(40)
$$
X' = PXQ.
$$

Clearly the relation "X and X' are equivalent" is an equivalence relation (Set Theory, II, § 6, no. 1) on the set $A^{mn}$ of matrices of type $(m, n)$ over A, which justifies the terminology.

With this definition, Proposition 6 of no. 8 can be stated by saying that when the bases are changed in two right A-modules E, F (with finite bases), the matrix of a linear mapping $u : E \to F$ with respect to the new bases is equivalent to the matrix of $u$ with respect to the old bases.

Conversely, if relation (40) holds and $u : A_d^n \to A_d^m$ is a linear mapping whose matrix is $X$ with respect to the respective canonical bases $(e_i)$ and $(f_j)$ of $A_d^n$ and $A_d^m$, then $X'$ is the matrix of $u$ with respect to the bases $(e'_i)$ and $(f'_j)$ such that $Q$ is the matrix of passage from $(e_i)$ to $(e'_i)$ and $P^{-1}$ the matrix of passage from $(f_j)$ to $(f'_j)$.

Examples of equivalent matrices. (1) Two matrices $X = (x_{ij})$ and $X' = (x'_{ij})$ with $m$ rows and $n$ columns "differ only in the order of their rows" if there exists a permutation $\sigma$ of the interval $[1, m]$ of $\mathbf{N}$, such that for every ordered pair of indices $(i, j)$, $x'_{ij} = x_{\sigma(i), j}$ (we also say that $X'$ is obtained by performing the permutation $\sigma^{-1}$ on the rows of $X$). The matrices $X$ and $X'$ are then equivalent, for $X' = PX$, where $P$ is the matrix of the permutation $\sigma^{-1}$ (cf. no. 7, Example II).

Similarly $X$ and $X'$ are said to differ only in the order of their columns if there exists a permutation $\tau$ of $[1, n]$ such that $x'_{ij} = x_{i, \tau(j)}$ for every ordered pair of indices $(i, j)$, $X$ and $X'$ are also equivalent, for $X' = XQ$ where $Q$ is the matrix of the permutation $\tau$.

Note that in the above notation $P$ is the matrix of passage from a basis $(f_j)_{1 \leq j \leq m}$ to the basis $(f_{\sigma^{-1}(j)})_{1 \leq j \leq m}$ and $Q$ the matrix of passage from a basis $(e_i)_{1 \leq i \leq n}$ to the basis $(e_{\tau(i)})_{1 \leq i \leq n}$.

(2) Let $j, k$ be distinct elements of $[1, n]$ and let $a \in A$.

Suppose that for $1 \leq i \leq m$, $x'_{ij} = x_{ij} + x_{ik}a$ and $x'_{il} = x_{il}$ for $j \neq l$ and $1 \leq i \leq m$; $X'$ is said to be derived from $X$ by adding to the column of $X$ of index $j$ the column of index $k$ multiplied on the right by $a$. In this case $X$ and $X'$ are also equivalent: for if $Q = I_n + aE_{kj}$ (an invertible triangular matrix, as seen in no. 7), then $X' = XQ$.

Similarly, let $h, i$ be two distinct elements of $[1, m]$ and $a$ an element of $A$; if $X'$ is derived from $X$ by adding to the row of $X$ of index $i$ the row of index $h$ multiplied on the left by $a$, $X$ and $X'$ are equivalent, for $X' = PX$, where $P = I_m + aE_{ih}$.

(3) Finally, if, for a given index $j$, $x'_{ij} = x_{ij}c$ for $1 \leq i \leq m$, where $c$ is invertible and $x'_{il} = x_{il}$ for $1 \leq i \leq m$ and $l \neq j$, $X$ and $X'$ are equivalent; for $X' = XQ$, where $Q$ is the matrix $\operatorname{diag}(a_k)$ with $a_j = c$, $a_k = 1$ for $k \neq j$. Then $X'$ is said to be derived from $X$ by multiplying the column of $X$ of index $j$ on the right by $a$.

Similarly, if $X'$ is derived from $X'$ by multiplying the row of $X$ of index $i$ on the left by an invertible element $c \in A$, $X'$ and $X$ are equivalent, for $X' = PX$ where $P$ is the matrix $\operatorname{diag}(b_h)$ with $b_i = c$, $b_h = 1$ for $h \neq i$.

#### Definition 6 {#alg-ii-s10-def-6 .statement}

*Two square matrices X, X' of order n over a ring A are called similar if there exists an invertible square matrix P of order n such that*

$$(41)$$
$$X' = PXP^{-1}$$

Clearly the relation "X and X' are similar" is an *equivalence relation* on $M_n(A)$ meaning that X and X' are transformed into one another by an *inner automorphism* of this ring.

With this definition, Corollary 1 to Proposition 6 of no. 8 can be stated by saying that when the basis of an A-module E (with a finite basis) is changed, the matrix of an endomorphism u with respect to the new basis is *similar* to the matrix of u with respect to the old basis.

#### Remark {#alg-ii-s10-n9-rem-1 .statement}

(1) Two square matrices which differ only in the order of their rows (or the order of their columns) are equivalent, but in general *not similar*. A matrix similar to a square matrix $X = (x_{ij})$ can be obtained by performing *the same permutation* $\sigma^{-1}$ on the rows and columns, that is by considering the matrix $X' = (x'_{ij})$, where $x'_{ij} = x_{\sigma(i), \sigma(j)}$ for every ordered pair of indices; for if X is the matrix of an endomorphism u of $A^n_d$ with respect to a basis $(e_i)_{1 \leq i \leq n}$, $X'$ is the matrix of u with respect to the basis $(e_{\sigma(i)})_{1 \leq i \leq n}$.

(2) Let X and $X'$ be two square matrices of order n which can be written in the form of diagonal matrices of square matrices (no. 7, Example IV):

$$
X = \begin{pmatrix}
X_1 & 0 & \ldots & 0 \\
0 & X_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X_p
\end{pmatrix}
\qquad
X' = \begin{pmatrix}
X'_1 & 0 & \ldots & 0 \\
0 & X'_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X'_p
\end{pmatrix}
$$

corresponding to the *same* partition of the indexing set $[1, n]$ for X and $X'$. If, for $1 \leq i \leq p$, $X_i$ and $X'_i$ are equivalent (resp. similar), then X and $X'$ are equivalent (resp. similar): for, if $X'_i = P_i X_i Q_i$ for $1 \leq i \leq p$, then $X' = PXQ$ where

$$
P = \begin{pmatrix}
P_1 & 0 & \ldots & 0 \\
0 & P_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & P_p
\end{pmatrix}
\qquad
Q = \begin{pmatrix}
Q_1 & 0 & \ldots & 0 \\
0 & Q_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Q_p
\end{pmatrix}
$$

as follows from calculating the "block" product (no. 6). Moreover, if $Q_i = P_i^{-1}$ for all i, then $Q = P^{-1}$.

### 10. TENSOR PRODUCT OF MATRICES OVER A COMMUTATIVE RING

Let C be a commutative ring, E, F, U, V four C-modules and $\phi : E \to U$, $\psi : F \to V$ two C-linear mappings. Suppose that E, F, U, V have respectively finite bases $(e_\lambda)_{\lambda \in L}, (f_\mu)_{\mu \in M}, (u_\rho)_{\rho \in R}, (v_\sigma)_{\sigma \in S}$; let $A = (a_{\rho \lambda})$ be the matrix of $\phi$ with respect to $(e_\lambda)$ and $(u_\rho)$, $B = (b_{\sigma \mu})$ that of $\psi$ with respect to $(f_\mu)$ and $(v_\sigma)$. For every ordered pair $(\lambda, \mu) \in L \times M = N$, let $g_{\lambda \mu} = e_\lambda \otimes f_\mu$; for every ordered pair $(\rho, \sigma) \in R \times S = T$ let $w_{\rho \sigma} = u_\rho \otimes v_\sigma$; the $g_{\lambda \mu}$ then form a basis of $E \otimes F$ and the $w_{\rho \sigma}$ a basis of $U \otimes V$ (§ 3, no. 6, Corollary 2 to Proposition 7). The *tensor product* of $A$ by $B$, denoted by $A \otimes B$, is the matrix $X = (x_{\tau v})_{(\tau, v) \in T \times N}$ whose elements are given by

$$
x_{(\rho, \sigma), (\lambda, \mu)} = a_{\rho \lambda} b_{\sigma \mu}.
$$

Then $A \otimes B$ is *the matrix of* $\phi \otimes \psi$ *with respect to the bases* $(g_{\lambda \mu})$ *and* $(w_{\rho \sigma})$. By definition (§ 3, no. 2, formula (3))

$$
\begin{align*}
(\phi \otimes \psi)(g_{\lambda \mu}) &= (\phi \otimes \psi)(e_\lambda \otimes f_\mu) = \phi(e_\lambda) \otimes \psi(f_\mu) \\
&= \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} (u_\rho \otimes v_\sigma) = \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} w_{\rho \sigma}.
\end{align*}
$$

Definition (42) of the elements of $A \otimes B$ shows that this matrix corresponds bijectively with the matrix of matrices $(a_{\rho \lambda} B)_{(\rho, \lambda) \in R \times L}$ and also the matrix $(A b_{\sigma \mu})_{(\sigma, \mu) \in S \times M}$ (no. 5).

The fact that $(\phi, \psi) \mapsto \phi \otimes \psi$ is a C-bilinear mapping and formula (9) of § 3, no. 5, can be expressed by the identities

$$
\begin{align*}
(A \otimes (B_1 + B_2)) &= A \otimes B_1 + A \otimes B_2 \\
((A_1 + A_2) \otimes B) &= A_1 \otimes B + A_2 \otimes B
\end{align*}
$$
(43)

$$(cA) \otimes B = A \otimes (cB) = c(A \otimes B) \quad \text{for } c \in \mathbf{C}$$
(44)

$$(A_1 \otimes B_1)(A_2 \otimes B_2) = (A_1 A_2) \otimes (B_1 B_2)$$
(45)

when the operations appearing are defined. The transpose of a tensor product of matrices is given by

$$(A \otimes B)^t = (A^t) \otimes (B^t).$$
(46)

If $A$ and $B$ are invertible square matrices over $\mathbf{C}$, $A \otimes B$ is invertible and

$$(A \otimes B)^{-1} = (A^{-1}) \otimes (B^{-1}).$$
(47)

Let $(e'_\lambda)_{\lambda \in L}$ be another basis of $E$ and $(f'_\mu)_{\mu \in M}$ another basis of $F$; if $P$ is the matrix of passage from the basis $(e_\lambda)$ to the basis $(e'_\lambda)$ and $Q$ the matrix of passage from the basis $(f_\mu)$ to the basis $(f'_\mu)$, the matrix of passage from the basis $(e_\lambda \otimes f_\mu)$ to the basis $(e'_\lambda \otimes f'_\mu)$ is $P \otimes Q$. If $A'$ is *equivalent* (resp. *similar*) to $A$ and $B'$ *equivalent* (resp. *similar*) to $B$, then $A' \otimes B'$ is *equivalent* (resp. *similar*) to $A \otimes B$.

The definition of tensor product of matrices can be generalized in an obvious way to an arbitrary finite number of matrices over $\mathbf{C}$; in particular we have the associativity formula

$$
\left( \bigotimes_{i \in I_1} X_i \right) \otimes \left( \bigotimes_{i \in I_2} X_i \right) = \bigotimes_{i \in I} X_i
$$

for every *partition* $(I_1, I_2)$ of the finite indexing set $I$.

### 11. TRACE OF A MATRIX

Let $C$ be a *commutative* ring; for every square matrix $X = (x_{ij})$ over $C$ corresponding to the finite indexing set $I$, the *trace* of $X$ is the element

$$
\operatorname{Tr}(X) = \sum_{i \in I} x_{ii}.
$$

Let $E$ be a $C$-module admitting a finite basis $(e_i)_{i \in I}$; for every endomorphism $u$ of $E$,

$$
\operatorname{Tr}(u) = \operatorname{Tr}(M(u))
$$

$M(u)$ being the matrix $u$ with respect to the basis $(e_i)$; this follows immediately from § 4, no. 3, formula (17), when this formula is applied to the endomorphism $x \mapsto \langle x, e_i^*\rangle e_j$ (where $e_i^*$) is the dual basis of $(e_i)$); from this we pass to the general case by linearity. Formula (49) shows that

$$
\operatorname{Tr}(u) = \sum_i \langle u(e_i), e_i^* \rangle
$$

for every basis $(e_i)$ of $E$ (cf. § 4, no. 3, formula (17)).

If $X$ is a matrix of type $(m, n)$ over $C$ and $Y$ a matrix of type $(n, m)$ over $C$, then

$$
\operatorname{Tr}(XY) = \operatorname{Tr}(YX)
$$

as follows from the above and Proposition 3 of § 4, no. 3; (52) can also be obtained directly, for if $X = (x_{ij}), Y = (y_{ji})$ ($1 \leq i \leq m, 1 \leq j \leq n$), then

$$
\operatorname{Tr}(XY) = \sum_{i,j} x_{ij} y_{ji}
$$

by (49). The latter formula proves moreover:

#### Proposition 7 {#alg-ii-s10-prop-7 .statement}

*Let $C$ be a commutative ring and for every matrix $P \in \mathbf{M}_n(C)$ let $f_P$ be the linear form $X \mapsto \operatorname{Tr}(PX)$ on $\mathbf{M}_n(C)$; the mapping $P \mapsto f_P$ is a $C$-linear bijection of $\mathbf{M}_n(C)$ onto its dual.*

#### Proposition 8 {#alg-ii-s10-prop-8 .statement}

*If $g$ is a linear form on the $C$-module $\mathbf{M}_n(C)$ such that $g(XY) = g(YX)$ for all matrices $X, Y$ in $\mathbf{M}_n(C)$, there exists one and only one scalar $c \in C$ such that $g(X) = c \cdot \operatorname{Tr}(X)$ for every matrix $X \in \mathbf{M}_n(C)$.*

Since the proposition is trivial for $n = 1$, attention may be confined to the case where $n \geqslant 2$. Taking $X = E_{ij},\ Y = E_{jk}$ with $i \neq k$, we obtain $g(E_{ik}) = 0$; then taking $X = E_{ij},\ Y = E_{ji}$ with $i \neq j$, we find $g(E_{ii}) = g(E_{jj})$; the proposition follows immediately since the $E_{ij}$ form a basis of $\mathbf{M}_n(\mathbf{C})$.

### 12. MATRICES OVER A FIELD

The finite matrices with $m$ rows and $n$ columns over a field $K$ are in one-to-one correspondence with the linear mappings of the right vector space $E = K_d^n$ into the right vector space $K_d^m$ when the matrices of these mappings are taken with respect to the canonical bases of $E$ and $F$. By definition, the *rank* of such a matrix $X$ is the rank of the linear mapping $u : E \to F$ corresponding to it; as this number is by definition the dimension of the subspace $u(E)$ of $F$, it amounts to the same (identifying the columns of $X$ with the images under $u$ of the canonical basis of $E$) to give the following definition:

#### Definition 7 {#alg-ii-s10-def-7 .statement}

*Given a matrix $X$ with $m$ rows and $n$ columns over a field $K$, the dimension of the subspace of $K_d^m$ generated by the $n$ columns of $X$ is called the rank of $X$ with respect to $K$ and denoted by $\operatorname{rg}(X)$.*

It can also be said that the rank of $X$ is the *maximum number of linearly independent columns of $X$* (as elements of $K_d^m$). Obviously $\operatorname{rg}(X) \leqslant \inf(m, n)$; for every submatrix $Y$ of $X$, $\operatorname{rg}(Y) \leqslant \operatorname{rg}(X)$.

If $E$ and $F$ are two finite-dimensional vector spaces over $K$ and $u$ a linear mapping of $E$ into $F$, the rank of the matrix $M(u)$ with respect to any two bases is equal to the rank of $u$.

#### Proposition 9 {#alg-ii-s10-prop-9 .statement}

*If the elements of a matrix $X$ with $m$ rows and $n$ columns belong to a subfield $K_0$ of a field $K$, the rank of $X$ with respect to $K_0$ is equal to the rank of $X$ with respect to $K$.*

Let $F_0$ be the right vector $K_0$-space generated by the canonical basis of the right vector $K$-space $E = K_d^m$; by hypothesis the columns of $X$ belong to $E_0$. Let $V_0$ (resp. $V$) be the vector sub-$K_0$-space of $F_0$ (resp. the vector sub-$K$-space of $E$) generated by these columns. Then $V = V_0 \otimes_{K_0} K$ (§ 8, no. 2, Proposition 2) and hence $\dim_K V = \dim_{K_0} V_0$.

#### Proposition 10 {#alg-ii-s10-prop-10 .statement}

*The rank of a matrix $X$ over a field $K$ is equal to the rank of its transpose ${}^t X$ over the opposite field $K^0$.*

In the notation introduced before Definition 7, the rank of $u$ is equal to that of ${}^t u$ (§ 7, no. 5, Proposition 10) and the proposition therefore follows from no. 4, Proposition 3.

It is thus seen that the rank of $X$ can also be defined as the *maximum number of linearly independent rows of $X$* (considering them as elements of the left vector $K$-space $K_s^n$).

The square matrices of order $n$ over a field $K$ correspond bijectively with the endomorphisms of $E = K_d^n$ and form a ring isomorphic to the ring

End$_{\mathbf{K}}$ (E) (no. 7); corresponding to the automorphisms of E are the invertible square matrices.

#### Proposition 11 {#alg-ii-s10-prop-11 .statement}

*Let X be a square matrix of order n over a field K. The following properties are equivalent:*

(a) *X is invertible in $\mathbf{M}_n(\mathbf{K})$.*
(b) *X is right invertible in $\mathbf{M}_n(\mathbf{K})$.*
(c) *X is left invertible in $\mathbf{M}_n(\mathbf{K})$.*
(d) *X is of rank n.*

This is just a translation of § 7, no. 4, Corollary to Proposition 9.

#### Proposition 12 {#alg-ii-s10-prop-12 .statement}

*For a system of m linear equations in n unknowns*

$$
\sum_{j=1}^n a_{ij} x_j = b_i \quad (1 \leq i \leq m)
$$

*over a field K to have at least one solution, it is necessary and sufficient that the matrix $A = (a_{ij})$ of the system and the matrix B, obtained by bordering A with an $(n+1)$-th column equal to $(b_i)$, be matrices of the same rank.*

It has been seen (no. 4) that the existence of a solution of (54) is equivalent to the fact that the column $(b_i)$ is a linear combination of the columns of $A$ and the proposition therefore follows from § 7, no. 3, Corollary 4 to Proposition 4.

Note that the condition of Proposition 12 is always fulfilled when $m = n$ and $A$ is invertible, that is of rank $n$ (Proposition 11). If $x$ and $b$ then denote the matrices with one column $(x_i)$ and $(b_i)$ respectively, system (54) is equivalent to $A.x = b$ and its unique solution is $x = A^{-1}.b$.

### 13. EQUIVALENCE OF MATRICES OVER A FIELD

#### Proposition 13 {#alg-ii-s10-prop-13 .statement}

*Let E, F be two finite-dimensional vector spaces over a field K. If $u : E \to F$ is a linear mapping of rank r, there exist bases of E and F such that, with respect to these bases,

$$
M(u) = \begin{pmatrix} I_r & 0 \\ 0 & 0 \end{pmatrix}.
$$

Every matrix of type $(m, n)$ over K and of rank r is equivalent to a matrix of the form (55).*

The second assertion is trivially equivalent to the first. To show the latter, let $\dim E = n$, $\dim F = m$. The kernel $N = u^{-1}(0)$ is of dimension $n - r$ (§ 7, no. 4, formula (11)); let V be a supplementary subspace of N in E and $(e_i)_{1 \leq i \leq n}$ a basis of E such that $(e_i)_{1 \leq i \leq r}$ is a basis of V and $(e_i)_{r+1 \leq i \leq n}$ a basis of N. Then the $u(e_j)$ $(1 \leq j \leq r)$ form a basis of $u(E)$; hence there exists a basis $(f_j)_{1 \leq j \leq m}$ of F such that $f_j = u(e_j)$ for $1 \leq j \leq r$ (§ 7, no. 1, Theorem 2) and clearly with respect to the bases $(e_i)$ and $(f_j)$ the matrix $M(u)$ is given by (55).

#### Corollary {#alg-ii-s10-n13-cor-1 .statement}

*For two matrices over a field, of type $(m, n)$, to be equivalent, it is necessary and sufficient that they have the same rank.*

We shall now recover Proposition 13 by another more explicit method. For every ring $A$, every $\lambda \in A$, every integer $m > 1$ and every ordered pair of *distinct* integers $i, j$ in $[1, m]$, we write

$$
B_{ij}(\lambda) = I_m + \lambda E_{ij}
$$

an invertible matrix of order $m$ by no. 8.

#### Lemma 1 {#alg-ii-s10-lem-1 .statement}

*Let $X = (\xi_{ij})$ be a matrix of type $(m, n)$ over a ring $A$. Suppose that $m \geqslant 2$ and that there exists an element $\xi_{i1}$ in the first column of $X$ which is invertible in $A$. Then there exist two invertible square matrices $P \in \mathbf{M}_m(A)$, $Q \in \mathbf{M}_n(A)$ and a matrix $Y$ of type $(m - 1, n - 1)$ over $A$ such that $P$ (resp. $Q$) is a product of matrices of the form $B_{ij}(\lambda)$ of order $m$ (resp. $n$) and*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 \\
0 & & & \\
\vdots & & Y & \\
0 & & &
\end{pmatrix}.
$$

The matrix $B_{ij}(\lambda)X$ is obtained by adding to the row of $X$ of index $i$ the row of index $j$ multiplied on the left by $\lambda$ (no. 9, *Example 2*); if $\xi_{i1}$ is invertible, then there exists $\lambda \in A$ such that, for the matrix $X' = B_{1i}(\lambda)X = (\xi'_{kl})$, $\xi'_{11} = 1$; multiplying $X'$ on the left by suitably chosen matrices $B_{k1}(\mu_k)$ of order $m$ (for $1 \leq k \leq m$), a matrix $X'' = (\xi''_{kl})$ is obtained such that $\xi''_{j1} = 1$, $\xi''_{k1} = 0$ for $k \neq 1$. Then the matrix obtained is multiplied successively *on the right* by suitable matrices $B_{1j}(v_j)$ of order $n$ $(2 \leq j \leq n)$ and a matrix is obtained of the form (57).

#### Proposition 14 {#alg-ii-s10-prop-14 .statement}

*Let $X$ be a matrix of type $(m, n)$ over a field $K$. If $X$ is of rank $r$, there exist two invertible square matrices $P \in \mathbf{M}_m(K)$, $Q \in M_n(K)$ such that $P$ (resp. $Q$) is a product of matrices of order $m$ (resp. $n$) of the form $B_{ij}(\lambda)$ and*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & \delta_r & 0 & \cdots & 0 \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0
\end{pmatrix}
$$

(a matrix $(\eta_{ij})$ all of whose terms are zero except the $\eta_{li}$ for $1 \leq i \leq r$, with $\eta_{li} = 1$ for $1 \leq i \leq r - 1$, $\eta_{rr} = \delta_r \neq 0$). *If $r \neq m$ or $r \neq n$, it may also be assumed that $\delta_r = 1$.

The proposition is obvious if $X = 0$; suppose therefore $X \neq 0$. If $m = n = 1$ the proposition is obvious (with $P = I_m$, $Q = I_n$, $\delta_1 \neq 0$ arbitrary). If $n = 1$, $m \geq 2$, we can apply Lemma 1 (since $X \neq 0$), which gives the desired form (58) with $r = 1$, $\delta_r = 1$. We argue by induction on $n > 1$; there exists an element $\xi_{ij} \neq 0$ in $X$; if $j = 1$, Lemma 1 can be applied and reduces the problem to the case where $X$ has the form (57). The induction hypothesis then applies to $Y$ and there are therefore invertible matrices

$$
P' \in \mathbf{M}_{m-1}(\mathbf{K}), \quad Q' \in \mathbf{M}_{n-1}(\mathbf{K})
$$

which are products of matrices of the form $B_{ij}(\lambda)$ of order $m - 1$ (resp. $n - 1$), such that $P'YQ'$ is of the form (58). But, if $B_{ij}(\lambda)$ belongs for example to $\mathbf{M}_{m-1}(\mathbf{K})$, then

$$
\begin{pmatrix}
1 & 0 \\
0 & B_{ij}(\lambda)
\end{pmatrix} = B_{i+1,\ j+1}(\lambda);
$$

formula (58) then follows from the formula for block products writing

$$
P = \begin{pmatrix} 1 & 0 \\ 0 & P' \end{pmatrix} \text{ and } Q = \begin{pmatrix} 1 & 0 \\ 0 & Q' \end{pmatrix}.
$$

If finally $j \neq 1$, it would be sufficient to consider the matrix $XB_{j1}(1)$ to reduce it to the above case.

Proposition 14 recovers Proposition 13 immediately.

#### Corollary 1 {#alg-ii-s10-prop-14-cor-1 .statement}

*If $X$ is an invertible square matrix of order $n$ over a field $\mathbf{K}$, there exist three invertible matrices $P, Q, D$ of order $n$ such that $X = PDQ$, $P$ and $Q$ being products of matrices of the form $B_{ij}(\lambda)$ and $D$ a diagonal matrix of the form*

$$
D = \operatorname{diag}(1, 1, \ldots, \delta),
$$

*where $\delta \neq 0$ (cf. Exercise 13).*

#### Corollary 2 {#alg-ii-s10-prop-14-cor-2 .statement}

*For every field $\mathbf{K}$, the group of invertible matrices $\mathbf{GL}(n, \mathbf{K})$ is generated by the permutation matrices (no. 7, Example 2), the diagonal matrices $\operatorname{diag}(a, 1, \ldots, 1)$ ($a \neq 0$ in $\mathbf{K}$) and the matrices $B_{12}(\lambda)$ ($\lambda \in \mathbf{K}$).*

It has been seen (no. 9) that the right (resp. left) product of a matrix by the matrix of a suitable transposition exchanges any two columns (resp. rows). Then the matrix $\operatorname{diag}(1, \ldots, 1, a)$ is equal to the product of $\operatorname{diag}(a, 1, \ldots, 1)$ and permutation matrices and every matrix $B_{ij}(\lambda)$ is equal to the product of $B_{12}(\lambda)$ and permutation matrices, whence the corollary.

#### Remark {#alg-ii-s10-n13-rem-1 .statement}

(1) In Chapter III, we shall see that, if $m = n = r$ and $K$ is *commutative*, then, for all choices of $P$ and $Q$ satisfying the conditions of Proposition 14, the element $\delta_r$ is always the same and equal to the *determinant* of $X$ (III, § 8, no. 6).

(2) The argument of Proposition 14, slightly modified, shows that there is a permutation matrix $R$ such that (with the same conditions on $P$)

$$
PX R = \begin{pmatrix} I_r & N \\ 0 & 0 \end{pmatrix}
$$

if $m = n = r$ does not hold, and

$$
PX R = \operatorname{diag}(1, \ldots, 1, \delta)
$$

otherwise. Observe also that the method of proof gives an explicit determination of the matrices $P, Q, R$ when $X$ is given explicitly.

### Exercises {#alg-ii-s10-exercises}

See the [exercises for § 10](exercises/s10/).
