---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 1
section_title: Polynomials
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0010-0023, 0095-0096
extraction: ocr
subsections:
    - "no": 1
      title: Definition of polynomials
      page: 0
      pdf_page: 10
    - "no": 2
      title: Degrees
      page: 2
      pdf_page: 11
    - "no": 3
      title: Substitutions
      page: 4
      pdf_page: 13
    - "no": 4
      title: Differentials and derivations
      page: 6
      pdf_page: 15
    - "no": 5
      title: Divisors of zero in a polynomial ring
      page: 9
      pdf_page: 18
    - "no": 6
      title: Euclidean division of polynomials in one indeterminate
      page: 10
      pdf_page: 19
    - "no": 7
      title: Divisibility of polynomials in one indeterminate [^1]
      page: 11
      pdf_page: 20
    - "no": 8
      title: Irreducible polynomials
      page: 13
      pdf_page: 22
statements: 30
exercises: 5
content_sha256: 680d2b1dc0057e134cacc841defea4521163184e80d9745b8d469153561a213f
---

## § 1. POLYNOMIALS

### 1. Definition of polynomials

Let $ I $ be a set. We recall (III, p. 452) that the free commutative algebra on $ I $ over $ \mathbf{A} $ is denoted by $ \mathbf{A}[(X_i)_{i \in I}] $ or $ \mathbf{A}[X_i]_{i \in I} $. The elements of this algebra are called *polynomials* with respect to the indeterminates $ X_i $ (or in the indeterminates $ X_i $) with coefficients in $ \mathbf{A} $. Let us recall that the indeterminate $ X_i $ is the canonical image of $ i $ in the free commutative algebra on $ I $ over $ \mathbf{A} $; sometimes it is convenient to denote this image by another symbol such as $ X'_i, Y_i, T_i $, etc. This convention is often introduced by a phrase such as: « Let $ Y = (Y_i)_{i \in I} $ be a family of indeterminates »; in this case the algebra of polynomials in question is denoted by $ \mathbf{A}[Y] $. When $ I = \{1, 2, \ldots, n\} $, one writes $ \mathbf{A}[X_1, X_2, \ldots, X_n] $ in place of $ \mathbf{A}[(X_i)_{i \in I}] $.

For $ \nu \in \mathbf{N}^{(I)} $ we put

$$
X^\nu = \prod_{i \in I} X_i^{\nu_i}.
$$

Then $ (X^\nu)_{\nu \in \mathbf{N}^{(I)}} $ is a basis of the $ \mathbf{A} $-module $ \mathbf{A}[(X_i)_{i \in I}] $. The $ X^\nu $ are called *monomials* in the indeterminates $ X_i $. For $ \nu = 0 $ we obtain the unit element of $ \mathbf{A}[(X_i)_{i \in I}] $. Every polynomial $ u \in \mathbf{A}[(X_i)_{i \in I}] $ can be written in exactly one way in the form

$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$

where $ a_\nu \in \mathbf{A} $ and the $ \alpha_\nu $ are zero except for a finite number; the $ a_\nu $ are called the *coefficients* of $ u $; the $ \alpha_\nu X^\nu $ are called the *terms* of $ u $ (often the element $ \alpha_\nu X^\nu $ is called the term in $ X^\nu $), in particular the term of $ \alpha_0 X^0 $, identified with $ a_0 $, is called the *constant term* of $ u $. When $ \alpha_\nu = 0 $, we say by abuse of language that $ u $ *contains no element* in $ X^\nu $; in particular when $ \alpha_0 = 0 $, we say that $ u $ is a polynomial *without constant term* (III, p. 453). Any scalar multiple of 1 is called a *constant polynomial*.

Let B be a commutative ring and $ \rho : A \to B $ a ring homomorphism. We consider $ B[(X_i)_{i \in I}] $ as an A-algebra by means of $ \rho $. Thus the mapping $ \sigma $ of $ A[(X_i)_{i \in I}] $ into $ B[(X_i)_{i \in I}] $ which transforms $ \sum \alpha_v X^\nu $ into $ \sum \rho(\alpha_v) X^\nu $ is a homomorphism of A-algebras; if $ u \in A[(X_i)_{i \in I}] $, we sometimes denote by $ ^\rho u $ the image of $ u $ by this homomorphism. The homomorphism of $ B \otimes_A A[(X_i)_{i \in I}] $ into $ B[(X_i)_{i \in I}] $ canonically defined by $ \sigma $ transforms, for every $ i \in I $, $ 1 \otimes X_i $ into $ X_i $; this is an isomorphism of B-algebras (III, p. 449).

Let M be a free A-module with basis $ (e_i)_{i \in I} $. There exists precisely one unital homomorphism $ \varphi $ of the symmetric algebra $ S(M) $ into the algebra $ A[(X_i)_{i \in I}] $ such that $ \varphi(e_i) = X_i $ for each $ i \in I $, and this homomorphism is an isomorphism (III, p. 506). This isomorphism is said to be canonical. It allows us to apply to polynomial algebras certain properties of symmetric algebras. For example, let $ (I_1), \ldots, L $ be a partition of I. Let $ \varphi_\lambda $ be the homomorphism of $ P_\lambda = A[(X_i)_{i \in I_\lambda}] $ into $ P = A[(X_i)_{i \in I}] $ which transforms $ X_i $ (qua element of $ P_\lambda $) into $ X_i $ (qua element of P). Then the $ \varphi_\lambda $ define a homomorphism of the algebra $ \bigotimes_{h \in L} P_\lambda $ into the algebra P,
and this homomorphism is an isomorphism (III, p. 503, Prop. 9).

Let E be an A-module, and put $ E \otimes_A A[(X_i)_{i \in I}] = E[(X_i)_{i \in I}] $. The elements of the A-module $ E[(X_i)_{i \in I}] $ are called polynomials in the indeterminates $ X_i $ with coefficients in E. Such a polynomial can be written in just one way as $ \sum_{v \in \mathbf{N}^{(I)}} e_v \otimes X^\nu $, where $ e_v \in E $ and the $ e_v $ are zero for all but a finite number of suffixes; we frequently write $ e_v X^\nu $ instead of $ e_v \otimes X^\nu $.

### 2. Degrees

Let $ P = A[(X_i)_{i \in I}] $ be a polynomial algebra. For each integer $ n \in \mathbf{N} $ let $ P_n $ be the submodule of P generated by the monomials $ X^\nu $ such that $ |\nu| = \sum_{i \in I} \nu_i $ equals n. Then $ (P_n), \ldots $ is a graduation which turns $ A[(X_i)_{i \in I}] $ into a graded algebra of type $ \mathbf{N} $ (III, p. 459). The homogeneous elements of degree $ n $ in $ A[(X_i)_{i \in I}] $ are sometimes called forms of degree $ n $ with respect to the indeterminates $ X_i $.

When we are dealing with the degree of inhomogeneous polynomials, we shall agree to adjoin to the set $ \mathbf{N} $ of natural numbers, an element written $ -\infty $ and to extend the order relation and the addition of $ \mathbf{N} $ to $ \mathbf{N} \cup \{-\infty\} $ by the following conventions, where $ n \in \mathbf{N} $,

$$
-\infty < n , \quad (-\infty) + n = n + (-\infty) = -\infty , \quad (-\infty) + (-\infty) = -\infty .
$$

Let $ u = \sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^\nu $ be a polynomial. The homogeneous component $ u_n $ of degree n of $ u $ (for the graduation of type N defined above) is equal to $ \sum_{|\nu|=n} \alpha_\nu X^\nu $, and we clearly have $ u = \sum_{n \in \mathbf{N}} u_n $. If $ u \neq 0 $, the $ u_n $ are not all zero, and we define the *degree* (or *total degree*) of $ u $, written $ \deg u $, as the greatest of the numbers $ n $ such that $ u_n \neq 0 $; in other words (III, p. 453), the degree of $ u $ is the largest of the integers $ |\nu| $ for the multi-indices $ \nu $ such that $ a_\nu \neq 0 $. When $ u = 0 $, the degree of $ u $ is $ -\infty $ by convention. For every integer $ p \in \mathbf{N} $, the relation $ \deg u \leq p $ is thus equivalent to « $ a_\nu = 0 $ for every multi-index $ \nu $ with $ |\nu| > p $ »; the set of polynomials $ u $ such that $ \deg u \leq p $ is thus an A-submodule of $ A[(X_i)_{i \in I}] $, equal to $ P_0 + P_1 + \ldots + P_p $ with the above notations.

Let E be an A-module. The family $ (E \otimes P_n)_{n \in \mathbf{N}} $ is a graduation of type N of the module $ E[(X_i)_{i \in I}] = E \otimes_A A[(X_i)_{i \in I}] $ of polynomials with coefficients in E. We extend the conventions adopted above for the degree of inhomogeneous polynomials to this case.

#### Proposition 1 {#alg-iv-s1-prop-1 .statement}

*Let $ u $ and $ v $ be two polynomials.*

(i) If $ \deg u \neq \deg v $, *we have*
$$
u + v \neq 0 \quad \text{and} \quad \deg(u + v) = \sup(\deg u, \deg v).
$$
If $ \deg u = \deg v $ *we have* $ \deg(u + v) \leq \deg u $.

(ii) *We have* $ \deg(uv) \leq \deg u + \deg v $.
The proof is immediate.

Let $ J \subset I $ and $ B = A[(X_i)_{i \in I - J}] $; we shall identify $ A[(X_i)_{i \in I}] $ with $ B[(X_i)_{i \in J}] $ (III, p. 453 f.). The degree of $ u \in A[(X_i)_{i \in I}] $, qua element of $ B[(X_i)_{i \in J}] $, is called the degree of $ u $ with respect to the $ X_i $ of index $ i \in J $ (III, p. 454).

Let $ u = \sum_{k=0}^n a_k X^k \in A[X] $ be a non-zero polynomial of degree $ n $ in a single indeterminate. The coefficient $ a_n $, which is $ \neq 0 $ by hypothesis, is called the *leading coefficient* of $ u $. *A* polynomial $ u \neq 0 $ whose leading coefficient is equal to 1 is called a *monic polynomial*.

In $ A[X_1, X_2, \ldots, X_q] $ the number of monomials of total degree $ p $ is equal to the number of elements $ (n_k)_{1 \leq k \leq q} $ of $ \mathbf{N}^q $ such that $ \sum_{k=1}^q n_k = p $, that is $ \binom{q+p-1}{p} $
(Sets III, Prop. 15, p. 182)

More generally, let A be a commutative monoid and $ (\delta_i)_{i \in I} $, a family of elements of A. There exists a unique graduation of type A of the algebra $ A[(X_i)_{i \in I}] $ such that each monomial $ X^\nu $ is of degree $ \sum_{i \in I} \nu_i \delta_i $ (III, p. 458, example 3). The case considered above is that where $ A = \mathbf{N} $ and $ \delta_i = 1 $. In the general case, to avoid confusion, we shall use the word « weight » instead of « degree » and « isobaric » instead of « homogeneous ». For example, there exists a unique graduation of type N of the algebra $ A[(X_i)_{i \geq 1}] $ such that $ X_i $ is of weight $ i $ for each integer $ i \geq 1 $. The isobaric elements of weight $ n $ are the polynomials of the form $ \sum a_{\nu} X^{\nu} $, where $ a_{\nu} = 0 $ for $ \sum_{i \geq 1} i \cdot \nu_i \neq n $.

### 3. Substitutions

Let E be a unital associative algebra over $ \mathcal{A} $ and $ x = (x_i)_{i \in I} $ a family of pairwise permutable elements of E. Let $ X = (X_i)_{i \in I} $ be a family of indeterminates. By III, Prop. 7, p. 449, there exists a unique unital homomorphism $ f $ of $ \mathcal{A}[X] $ into $ E $ such that $ f(X_i) = x_i $ for every $ i \in I $. The image of an element $ u $ of $ \mathcal{A}[X] $ under $ f $ is written $ u(x) $ and is called *the element of E obtained by substituting $ x_i $ for $ X_i $ in $ u $*, or also *the value of $ u $ for $ X_i = x_i $*. In particular, $ u = u((X_i)_{i \in I}) $. If $ I = \{1, \ldots, n\} $ we write $ u(x_1, \ldots, x_n) $ in place of $ u((x_i)_{i \in I}) $. More generally, if M is an A-module and if o is an element of

$$
M[(X_i)_{i \in I}] = M \otimes_A \mathcal{A}[(X_i)_{i \in I}],
$$

we denote the image of $ v $ in $ M \otimes_A E = M_{(E)} $ under the mapping $ 1_M \otimes f $ by $ v(x) $.

If the homomorphism $ u \mapsto u(x) $ of $ \mathcal{A}[X] $ into E is injective, we say that the family $ x $ is *algebraically free* over $ \mathcal{A} $, or that the $ x_i $ are *algebraically independent* over $ \mathcal{A} $. This also means that the monomials $ x^{\nu} $ ($ \nu \in \mathbf{N}^{(I)} $) are linearly independent over $ \mathcal{A} $.

If $ \lambda $ is a unital homomorphism of E into a unital associative A-algebra E', we have

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i)_{i \in I})) ,
$$

because $ \lambda \circ f $ is a homomorphism of $ \mathcal{A}[X] $ into E' which maps $ X_i $ to $ \lambda(x_i) $.

Let $ u \in \mathcal{A}[X] $. If $ E $ is commutative, the mapping $ x \mapsto u(x) $ of $ E^1 $ into E is called the *polynomial function* defined by $ u $ (and the algebra $ E $) ; we shall sometimes denote it by $ \tilde{u} $ (or even just $ u $).

Let $ Y = (Y_j)_{j \in J} $ be another family of indeterminates, and let us take for E the polynomial algebra $ \mathcal{A}[Y] $. Given $ u \in \mathcal{A}[X] $, take $ g_i \in \mathcal{A}[Y] $ for $ i \in I $ and put $ g = (g_i)_{i \in I} $; let $ u(g) \in \mathcal{A}/[Y] $ be the polynomial obtained by substituting the polynomials $ g_i $ for $ X_i $ in $ u $. Let $ y = (y_j)_{j \in J} $ be a family of pairwise permutable elements of a unital associative A-algebra E' ; applying (1) and taking for $ \mathcal{A} $ the homomorphism $ g \mapsto g(y) $ of $ E $ into $ E' $, we obtain

$$
(u(g))(y) = u((g_i(y))) .
$$

If $ f = (f_i)_{i \in I} \in (\mathcal{A}[(X_j)_{j \in J}])^I $ and $ g = (g_j)_{j \in J} \in (\mathcal{A}[(Y_k)_{k \in K}])^J $, we denote by $ f \circ g $ or $ f(g) $, the family of polynomials $ (f_i(g))_{i \in I} \in (\mathcal{A}[(Y_k)_{k \in K}])^I $. If we denote by $ \tilde{f} $ the mapping $ x \mapsto (f_i(x))_{i \in I} $ of $ E'^J $ into $ E'^I $ (where $ E' $ is a unital associative and commutative $ A $-algebra), then the relation (2) implies

$$(3)$$
$$(\mathrm{fog})'' = \tilde{f} \circ \tilde{g}.$$

If $ h = (h_k)_{k \in K} \in (A[(Z_l)_l \bullet_L])^K $, it follows from (2) that :

$$(4)$$
$$f \circ (g \circ h) = (f \circ g) \circ h.$$

#### Proposition 2 {#alg-iv-s1-prop-2 .statement}

*Let $ a = (a_i)_{i \in I} $, be a family of elements of $ A $ and let $ u \in A[X] $. If $ v $ is the polynomial obtained by substituting $ X_i + a_i $ for $ X_i $ for each $ i \in I $, then the constant term of $ v $ is equal to $ u(a) $.*

The constant term of $ v $ is obtained by substituting 0 for $ X_i $ in $ v $ for each $ i \in I $. The result therefore follows by (2).

#### Corollary 1 {#alg-iv-s1-prop-2-cor-1 .statement}

*Let $ m $ be the ideal of polynomials $ u \in A[X] $ such that $ u(a) = 0 $. Then $ m $ is generated by the polynomials $ X_i - a_i $ (for $ i \in I $).*

It is clear that $ X_i - a_i \in m $ for each $ i \in I $. Let $ u \in m $ and let $ v $ be as in Prop. 2. Since $ v $ has no constant term, there exists a family $ (P_i)_{i \in I} $, of polynomials in $ A[X] $ with finite support such that

$$
v(X) = \sum_{i \in I} X_i \cdot P_i(X).
$$

If we replace $ X_i $ by $ X_i - a_i $ for each $ i \in I $ in the above equation, we obtain a relation of the form $ u(X) = \sum_{i \in I} (X_i - a_i) \cdot P'_i(X) $, whence the corollary.

#### Corollary 2 {#alg-iv-s1-prop-2-cor-2 .statement}

*Let $ X = (X_i)_{i \in I} $ and $ Y = (Y_i)_{i \in I} $ be two families of indeterminates. The set of polynomials $ u \in A[X,Y] $ such that $ u(X,X) = 0 $ is the ideal of $ A[X,Y] $ generated by the polynomials $ X_i - Y_i $ (for $ i \in I $).*

This corollary results directly from Cor. 1 on replacing $ A $ by $ A[Y] $ and $ a_i $ by $ Y_i $, interpreting $ A[X,Y] $ as polynomial ring in the $ X_i $ with coefficients in $ A[Y] $.

#### Proposition 3 {#alg-iv-s1-prop-3 .statement}

*Let $ u \in A[X] $ and let $ X.Z $ be the family $ (X_iZ)_{i \in I} $, of elements of the polynomial ring $ A[X][Z] $. The coefficient of $ Z^k $ in $ u(X.Z) $ is the homogeneous component of degree $ k $ of $ u $, for every positive integer $ k $.*

It suffices to prove this Prop. in the case where $ u $ is a monomial, and in this case the result is clear.

#### Corollary {#alg-iv-s1-n3-cor-1 .statement}

*For a polynomial $ u \in A[X] $ to be homogeneous of degree $ k $ it is necessary and sufficient that :*

$$
u(X.Z) = u(X) \cdot Z^k.
$$

#### Remark {#alg-iv-s1-n3-rem-1 .statement}

— Let $ x \in A^I $ and let $ f $ be the mapping $ u \mapsto u(x) $ of $ A[X] $ into $ A $. Given an $ A $-module $ M $, we consider the homomorphism $ 1 \otimes f $ of $ M[X] = M \otimes_A A[X] $ into $ M \otimes_A A = M $. For each $ v \in M[X] $ we have $ (1 \otimes f)(v) = v(x) $. If $ v = \sum_{\nu \in \mathbf{N}^{(l)}} e_\nu X^\nu $, then $ v(x) = \sum_{\nu \in \mathbf{N}^{(l)}} x^\nu e_\nu $.

### 4. Differentials and derivations

Let $ B = A[(X_i)_{i \in I}] $, then by III, p. 569 there exists for each $ i \in I $ one and only one A-derivation $ D_i $ of B such that
$$
D_i X_i = 1 , \quad D_i X_j = 0 \quad \text{for} \quad j \neq i
$$
The polynomial $ D_i P $ is called the *partial derivative* of $ P $ *with respect to* $ X_i $; we shall also denote it by $ D_{X_i} P $ or $ \frac{\partial P}{\partial X_i} $ or $ P'_{X_i} $. By III, p. 558, formula (21), we have, for $ \nu = (\nu,) \in \mathbf{N}^{(l)} $,
$$
D_i (X^\nu) = \begin{cases}
\nu_i X_i^{\nu_i - 1} \prod_{j \in I - \{i\}} X_j^{\nu_j} & \text{if } \nu_i > 0 \\
0 & \text{if } \nu_i = 0
\end{cases}
$$
It follows from (6) that $ D_i D_j = D_j D_i $ for any $ i, j \in I $. For $ \nu = (\nu_i)_{i \in I} \in \mathbf{N}^{(l)} $ we shall put $ D^\nu = \prod_{i \in I} D_i^{\nu_i} $ and $ \nu! = \prod_{i \in I} (\nu_i!) $. With the product ordering on $ \mathbf{N}^{(l)} $ we have
$$
D^\nu(X^\mu) = \begin{cases}
\frac{\mu!}{(\mu - \nu)!} X^{\mu - \nu} & \text{if } \nu \leq \mu , \\
0 & \text{if not .}
\end{cases}
$$
When $ P $ is a polynomial in a single indeterminate $ X $, the unique partial derivative of $ P $ is written $ DP $ or $ \frac{dP}{dX} $ or $ P' $ and is called simply the *derivative* of $ P $.

Again let $ B = A[(X_i)_{i \in I}] $; by III, p. 569 the B-module of A-differentials of $ B $, $ \Omega_A(B) $, has the family $ (dX_i)_{i,} $, of differentials of the $ X_i $ as basis. Let $ \partial_i $ be the coordinate form of index $ i $ relative to this basis over $ \Omega_A(B) $. Then the mapping $ u \mapsto (\partial_i, du) $ of B into itself is a derivation of B which maps $ X_i $ to 1 and $ X_j $ to 0 for $ j \neq i $, and hence is $ D_i $; in other words, we have
$$
du = \sum_{i \in I} (D_i u) dX_i
$$
for each $ u \in B $. If I is finite, $ (D_i)_{i \in I} $ is a basis of the B-module of derivations of B.

#### Proposition 4 {#alg-iv-s1-prop-4 .statement}

*Let E be an associative, commutative and unital A-algebra, $ x = (x_i)_{i \in I} $ a family of elements of E, u an element of $ A[(X_i)_{i,}] $ and $ y = u(x) $. Then for every derivation D of E into an E-module we have*
$$
Dy = \sum_{i \in I} (D_i u)(x) \cdot Dx_i .
$$

It suffices to prove the proposition when $ u $ is a monomial, and in that case it follows from III, p. 558, Prop. 6.

#### Corollary {#alg-iv-s1-n4-cor-1 .statement}

— *Let $ f \in A[X_1, ..., X_p] $ and $ g_i \in A[Y_1, ..., Y_q] $ for $ 1 \leq i \leq p $, and write $ h = f(g_1, ..., g_p) $, then for $ 1 \leq j \leq q $ we have*

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j}.
$$

This is the special case $ E = A[Y_1, ..., Y_r] $, $ x_i = g_i $ and $ D = \partial / \partial Y_j $ of Prop. 4.

Let $ X = (X_i)_{i \in I} $, $ Y = (Y_i)_{i \in I} $ be two disjoint families of indeterminates, and write $ X + Y $ for the family $ (X_i + Y_i)_{i \in I} $. Given $ u \in A[X] $, consider the element $ u(X + Y) $ of $ A[X, Y] $. For $ \nu \in \mathbf{N}^{(I)} $ we denote by $ A^\nu u $ the coefficient of $ Y_\nu $ in $ u(X + Y) $, considered as polynomial in the $ Y_i $ with coefficients in $ A[X] $. By definition we have $ A^\nu u \in A[X] $ and

$$
u(X + Y) = \sum_\nu (\Delta^\nu u)(X) Y^\nu.
$$

(Here and in the rest of this No., the summations are extended over the index set $ \mathbf{N}^{(I)} $ unless the contrary is said.)

Let $ a \in A' $, then on substituting $ a $ for $ X $ and $ X - a $ for $ Y $ in (9) we obtain

$$
u(X) = \sum_\nu (\Delta^\nu u)(a)(X - a)^\nu.
$$

In particular we have

$$
u(X) = \sum_\nu (\Delta^\nu u)(0) X^\nu.
$$

If $ u, v \in A[X] $, we have

$$
(uv)(X + Y) = \left( \sum_\nu (\Delta^\nu u)(X) Y^\nu \right) \left( \sum_\rho (\Delta^\rho v)(X) Y^\rho \right)
= \sum_\sigma \left[ \sum_{\nu + \rho = \sigma} (\Delta^\nu u)(X)(\Delta^\rho v)(X) \right] Y^\sigma
$$

hence

$$
\Delta^\sigma(uv) = \sum_{\nu + \rho = \sigma} (\Delta^\nu u)(\Delta^\rho v).
$$

Let $ Z = (Z_i)_{i \in I} $ be another family of indeterminates.

We have:

$$
\sum_{\nu} (\Delta^\nu u)(\mathbf{X})(\mathbf{Y} + \mathbf{Z})^\nu = u(\mathbf{X} + \mathbf{Y} + \mathbf{Z})
$$
$$
= \sum_{\sigma} (Au u)(\mathbf{X} + \mathbf{Y})Zu
$$
$$
= \sum_{\rho, \sigma} (\Delta^\rho \Delta^\sigma u)(\mathbf{X}) Y^\rho Z^\sigma u,
$$

hence by I, p. 99, Cor. 2:

(13)
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \; \sigma!} \Delta^{\rho + \sigma} u.
$$

#### Proposition 5 {#alg-iv-s1-prop-5 .statement}

— *For any* $ u \in \mathbf{A}[\mathbf{X}] $ *and* $ \nu \in \mathbf{N}^{(I)} $ *we have*

$$
D^\nu u = \nu! \; \Delta^\nu u
$$

Suppose first that $ \nu $ has length 1 ; then there exists an element $ i $ of I such that $ \nu = \varepsilon_i $, that is, $ \nu_i = 1 $ and $ \nu_j = 0 $ for all $ j \neq i $ in I. Formula (12) shows that $ A'' $ is a derivation of the A-algebra $ \mathbf{A}[\mathbf{X}] $ which clearly has the value zero on $ X_j $ for $ j \neq i $ and the value 1 on $ X_i $. We thus have $ \Delta^{\varepsilon_i} = D_i $ for each $ i \in I $.

By (13) we have

(14)
$$
(\rho! \; \Delta^\rho) \cdot (\sigma! \; \Delta^\sigma) = (\rho + \sigma)! \; \Delta^{\rho + \sigma}
$$

in the endomorphism algebra of the A-module $ \mathbf{A}[\mathbf{X}] $. It now follows by induction on the length of $ \nu $ that $ \nu! \; A'' = D^\nu $.

If $ \mathbf{A} $ is a Q-algebra, the formulae (9), (10), (11) may thus be written

(15)
$$
u(\mathbf{X} + \mathbf{Y}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(\mathbf{X}) \mathbf{Y}^\nu
$$
(16)
$$
u(\mathbf{X}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(a)(\mathbf{X} - a)^\nu
$$
(17)
$$
u(\mathbf{X}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(0) \; X^\nu
$$

The formulae (15), (16), (17) are all three called « Taylor's formula ».

#### Proposition 6 (*« Euler's identity »*) {#alg-iv-s1-prop-6 .statement}

— *Let* $ u \in \mathbf{A}[\mathbf{X}] $ *be a homogeneous polynomial of degree r ; we have*

$$
\sum_{i \in I} X_i \cdot D_i u = ru.
$$

Let D be the A-linear mapping of $ A[X] $ into itself such that $ D(v) = sv $ when v is homogeneous of degree s. We know (III, p. 554, Example 6) that D is a derivation of $ A[X] $. Thus Prop. 6 is a Corollary of Prop. 4 (IV, p. 6).

### 5. Divisors of zero in a polynomial ring

#### Proposition 7 {#alg-iv-s1-prop-7 .statement}

— *Let $ f \in A[X] $ be a non-zero polynomial in an indeterminate and $ a $ its leading coefficient. If $ a $ is cancellable in A (in particular iff is monic) then we have for any non-zero element'g of $ A[X] $,*

$$
fg \neq 0 \quad \text{and} \quad \deg(fg) = \deg f + \deg g
$$

Let $ g \in A[X] $ be a non-zero polynomial, $ \beta $ its leading coefficient, $ n = \deg f $ and $ p = \deg g $. Then the coefficient of $ X^{n+p} $ in $ fg $ is $ \alpha \beta $ which does not vanish, whence the proposition.

#### Proposition 8 {#alg-iv-s1-prop-8 .statement}

— *If A is an integral domain, then so is $ A[(X_i)_{i \in I}] $.*

Let $ u, v $ be two non-zero elements of $ A[(X_i)_{i \in I}] $; we have to show that $ uv \neq 0 $. Now $ u $ and $ v $ belong to a ring $ A[(X_j)_{j \in J}] $ where J is a finite subset of I. Thus we can limit ourselves to the case when I is finite and equal to $ \{1, 2, ..., p\} $. On the other hand, the ring $ A[X_1, ..., X_p] $ is isomorphic to the polynomial ring in $ X_p $ with coefficients in $ A[X_1, ..., X_{p-1}] $. By induction on $ p $ we are thus reduced to proving the proposition for $ A[X] $, and now it suffices to apply Prop. 7.

#### Corollary 1 {#alg-iv-s1-prop-8-cor-1 .statement}

— *If A is an integral domain, and $ u, v $ are elements of $ A[(X_i)_{i \in I}] $, then $ \deg(uv) = \deg u + \deg v $.*

We can limit ourselves to the case where $ u $ and $ v $ are non-zero. Let $ m = \deg u, n = \deg v $; we have

$$
u = u_0 + u_1 + \cdots + u_m, \quad v = v_0 + v_1 + \cdots + v_n
$$

where $ u_h $ (resp. $ v_h $) is the homogeneous component of degree $ h $ of $ u $ (resp. v). Since $ u_m \neq 0 $ and $ v_n \neq 0 $, we have $ u_m v_n \neq 0 $ (Prop. 8). Now $ uv = u_m v_n + w $ with $ \deg w < m + n $, whence the result.

#### Corollary 2 {#alg-iv-s1-prop-8-cor-2 .statement}

— *If A is an integral domain, the invertible elements of $ A[(X_i)_{i \in I}] $ are the invertible elements of A.*

This follows immediately from Cor. 1.

#### Proposition 9 {#alg-iv-s1-prop-9 .statement}

— *Let $ u \in A[(X_i)_{i \in I}] $; then for u to be nilpotent in the ring $ A[(X_i)_{i \in I}] $ it is necessary and sufficient for all its coefficients to be nilpotent in the ring A.*

As in the proof of Prop. 8 we can make a reduction to the case of polynomials in one variable X. If all the coefficients of $ u $ are nilpotent, then $ u $ is nilpotent (I, p. 99, Cor. 1). Suppose that $ u $ is nilpotent but not zero and let $ n $ be its degree; we shall argue by induction on $ n $. Let $ a $ be the leading coefficient of $ u $. There exists an integer $ m > 0 $ such that $ u^m = 0 $. The leading coefficient of $ u^m $ is $ a^m $, hence $ a^m = 0 $. Now $ u - \alpha X^n $ is nilpotent (I, loc. cit.) and the induction hypothesis shows all the coefficients of $ u - \alpha X^n $ to be nilpotent. Thus all the coefficients of $ u $ are nilpotent.

#### Remark {#alg-iv-s1-n5-rem-1 .statement}

Let $ u $ and $ v $ be elements of $ A[(X_i)_i \in ,] $, and suppose that $ A $ is an integral domain, $ v $ is a non-zero multiple of $ u $ and $ v $ is homogeneous; then $ u $ is also homogeneous. For let $ u' \in A[(X_i)_i ,_1] $ be such that $ v = uu' $; we have $ u \neq 0 $, $ u' \neq 0 $, and if
$$
u = u_h + u_{h+1} + \cdots + u_k \\
u' = u_{h'} + u_{h'+1} + \cdots + u_{k'}
$$
are the decompositions of $ u $ and $ u' $ into homogeneous components, with $ u_h \neq 0 $, $ u_k \neq 0 $, $ u_{h'} \neq 0 $, $ u_{k'} \neq 0 $, then $ v = u_h u_{h'} + u_h u_{h'+1} + \ldots + u_k u_{k'} $ and $ u_h u_{h'} $ is non-zero homogeneous of degree $ h + h' $ while $ u_k u_{k'} $ is non-zero homogeneous of degree $ k + k' $ (Prop. 8). Since $ v $ is homogeneous, we have $ h + h' = k + k' $ whence $ h = k $, $ h' = k' $.

### 6. Euclidean division of polynomials in one indeterminate

#### Proposition 10 {#alg-iv-s1-prop-10 .statement}

*Let $ f $ and $ g $ be non-zero elements of $ A[X] $ of degrees $ m $ and $ n $ respectively. Let $ \alpha_0 $ be the leading coefficient of $ f $ and $ \mu = \sup(n - m + 1, 0) $. There exist $ u, v \in A[X] $ such that*
$$
\alpha_0^\mu g = uf + v, \quad \deg v < m.
$$
*If $ \alpha_0 $ is cancellable in $ A $, then $ u $ and $ v $ are uniquely determined by these properties.*

The existence of $ u $ and $ v $ is clear when $ n < m $, because then we can take $ u = 0 $ and $ v = g $. For $ n \geq m $ we shall use induction on $ n $. Let $ \beta $ be the leading coefficient of $ g $; if $ f = \sum_{k=0}^m \alpha_k X^{m-k} $, we can write $ \alpha_0^\mu g = \alpha_0^\mu \beta X^n \cdot f + \alpha_0^{\mu-1} g_1 $, where $ g_1 \in A[X] $ and $ \deg g_1 < n $. By the induction hypothesis there exist $ u_1, v \in A[X] $ such that $ \alpha_0^{\mu-1} g_1 = u_1 f + v $ and $ \deg v < m $. Hence
$$
\alpha_0^\mu g = (\alpha_0^{\mu-1} \beta X^{n-m} + u_1) f + v
$$
and it suffices to put $ u = \alpha_0^{\mu-1} \beta X^{n-m} + u_1 $.

Assuming $ \alpha_0 $ to be cancellable in $ A $, let us now prove the uniqueness of $ u $ and $ v $. Let $ u, v, u_1, v_1 \in A[X] $ be such that
$$
\alpha_0^\mu g = uf + v = u_1 f + v_1, \quad \deg v < m, \quad \deg v_1 < m
$$

We have $(u - u_1) f = v_1 - v$ and $\deg(v_1 - v) < m$, hence $u - u_1 = 0$ (IV, p. 9, Prop. 7) and therefore $v_1 - v = 0$.

#### Corollary (« Euclidean division of polynomials ») {#alg-iv-s1-n6-cor-1 .statement}

— Let $f$ be a non-zero element of $A[X]$ whose leading *coefficient* is invertible and $m = \deg f$.
(i) For every $g \in A[X]$ there exist $u,\ v \in A[X]$ such *that*
$$
g = uf + v , \quad \deg v < m .
$$
Moreover, these conditions determine $u$ and $v$ uniquely.
(ii) The sub-A-modules $A + AX + \ldots + AX^{m-1}$ and $fA[X]$ of $A[X]$ are supplementary in $A[X]$.
(iii) Assume $f$ non-constant and consider $A[X]$ as an $A[T]$-*module* by means of the homomorphism $u(T) \mapsto u(f(X))$ of $A[T]$ into $A[X]$. Then $A[X]$ is a free $A[T]$-*module* with basis $(1, X, \ldots, X^{m-1})$.
Assertions (i) and (ii) are immediate consequences of Prop. 10.
Let us prove (iii). Let $\psi$ be the homomorphism $v \mapsto v(f(X), X)$ of $A[T, X]$ into $A[X]$. Consider $A[T, X]$ first as polynomial ring in $T$ with coefficients in $A[X]$; Cor. 1 of IV, p. 5 shows that the kernel $a$ of $\psi$ is the ideal $(T - f(X))$ of $A[T, X]$. Consider now $A[T, X]$ as polynomial ring in $X$ with coefficients in $A[T]$; then $\psi$ is an $A[T]$-linear mapping of $A[T][X]$ into $A[X]$. Assertion (ii) above (applied to the polynomial $f(X) - T$ in $X$ with coefficients in $A[T]$) shows that $(1, X, \ldots, X^{m-1})$ is a basis of an $A[T]$-submodule of $A[T, X]$ supplementary to $a$. Since $\psi(X^i) = X^i$ for every integer $i \geq 0$, (iii) follows at once.

With the notations of (i) we shall say that $u$ is the quotient and $v$ the remainder in the Euclidean division of $g$ by $f$; for the remainder to vanish it is necessary and sufficient that $f$ should divide $g$.

### 7. Divisibility of polynomials in one indeterminate [^1]

#### Proposition 11 {#alg-iv-s1-prop-11 .statement}

— Let $K$ be a commutative *field*.
(i) For every non-zero ideal $a$ of $K[X]$ there exists precisely one *monic* polynomial $f$ in $K[X]$ such that $a = (f )$.
(ii) Let $f_1$ and $f_2$ be in $K[X]$; for $(f,) = (f_2)$ to hold it is necessary and sufficient that there exist a non-zero element $\lambda$ of $K$ such that $f_2 = \lambda f_1$.
Let us prove (ii), the sufficiency of the stated condition being clear. The case where $f_1$ and $f_2$ generate the zero ideal is trivial. Thus assume that the non-zero polynomials $f_1$ and $f_2$ generate the same ideal of $K[X]$. Then there exist polynomials $u_1$ and $u_2$ such that $f_1 = u_1 f_2$ and $f_2 = u_2 f_1$; it follows that u_1 u_2 = 1, whence $ \deg u_1 + \deg u_2 = 0 $ and so $ \deg u_2 = 0 $. We have thus shown that $ u_2 $ is a non-zero element of $ K $.

To prove (i), let $ f $ be a monic polynomial in $ a $ of least possible degree. Given $ g $ in $ a $, let $ u $ and $ v $ be the quotient and remainder of the Euclidean division of $ g $ by $ f $; then $ v = g - u f $ belongs to $ a $ and we have $ \deg v < \deg f $; if $ v $ were non-zero, there would be a non-zero element $ A $ of $ K $ such that $ \lambda v $ is monic, and since $ \lambda v \in a $, this would contradict the definition off. We thus have $ a = (f) $; the uniqueness of the monic polynomial $ f $ such that $ a = (f) $ now follows from (ii).

#### Proposition 12 {#alg-iv-s1-prop-12 .statement}

*Let $ K $ be a commutative field and $ f, g $ two elements of $ K[X] $. For every polynomial $ d $ in $ K[X] $ the following properties are equivalent*:

(i) *The polynomial $ d $ divides $ f $ and $ g $ and every polynomial which divides both $ f $ and $ g $ divides $ d $*.

(ii) *The polynomial $ d $ divides $ f $ and $ g $ and there exist two polynomials $ u $ and $ v $ such that $ d = u f + v g $*.

(iii) *The relation $ (d) = (f) + (g) $ holds between ideals in $ K[X] $*.

*The polynomial $ d $ is determined up to multiplication by a non-zero element of $ K $ by these properties. If $ f $ and $ g $ are not both zero, then $ d \neq 0 $ and the degree of $ d $ majorizes the degree of every polynomial dividing both $ f $ and $ g $*.

When $ f $ and $ g $ are zero, each of the properties (i) to (iii) is satisfied only for $ d = 0 $, hence they are then equivalent. Henceforth we assume that $ f, g $ are not both 0 and we denote by $ a $ the ideal $ (f) + (g) $ of $ K[X] $.

We remark that for any polynomials $ u $ and $ v $ in $ K[X] $ the properties $ (u) \supset (v) $ and « $ u $ divides $ v $ » are equivalent. The assertion (ii) is thus equivalent to « $ (d) \supset (f) $ and $ (d) \supset (g) $ and $ d \in (f) + (g) $ », that is (iii). It is clear that (ii) implies (i). Finally suppose that (i) holds; we have $ (d) \supset (f) $ and $ (d) \supset (g) $, whence $ (d) \supset a $; on the other hand, by Prop. 11 (IV, p. 12) there exists a polynomial $ d_1 $ such that $ a = (d,) $; since $ d_1 $ divides both $ f $ and $ g $, it divides $ d $ by hypothesis, whence $ (d) \subset a $, and finally we have $ (d) = a $, that is, (iii).

The other assertions of Prop. 12 are immediate consequences of Prop. 11 applied to the ideal $ a = (f) + (g) $.

#### Definition 1 {#alg-iv-s1-def-1 .statement}

*With the notation of Prop. 12 we say that $ d $ is a greatest common divisor (gcd for short) of $ f $ and $ g $. We say that $ f $ and $ g $ are relatively prime or that $ f $ is prime to $ g $ if $ 1 $ is a gcd of $ f $ and $ g $*.

To say that $ f $ and $ g $ are relatively prime thus means that there exist polynomials $ u $ and $ v $ in $ K[X] $ such that $ u f + v g = 1 $.

#### Corollary 1 {#alg-iv-s1-def-1-cor-1 .statement}

*Let $ d $ be a gcd of $ f $ and $ g $ and $ K' $ a commutative field containing $ K $ as subfield. Then $ d $ is a gcd of $ f $ and $ g $ considered as elements of $ K'[X] $*.

This follows from Prop. 12, (iii).

#### Corollary 2 {#alg-iv-s1-def-1-cor-2 .statement}

— Let d be a gcd off and g.
    (i) If $ u \in K[X] $, du is a gcd of fu and gu.
    (ii) If $ v \in K[X] $ is a divisor ($ \neq 0 $) of f and g, then $ d/v $ is a gcd of $ f/v $ and $ g/v $.
    This follows from Prop. 12, (ii).

#### Corollary 3 {#alg-iv-s1-def-1-cor-3 .statement}

— Let w be a common factor of f and g. For w to be a gcd off and g it is necessary and sufficient that $ f/w $ and $ g/w $ are relatively prime.
    This follows from Cor. 2.

#### Corollary 4 {#alg-iv-s1-def-1-cor-4 .statement}

— Let $ f, g, h \in K[X] $. If f divides gh and is prime to g, then f divides h.
    For f divides gh and fh, hence f divides every gcd of gh and fh, in particular h (Cor. 2, (i)).

#### Corollary 5 {#alg-iv-s1-def-1-cor-5 .statement}

— Let $ f, g \in K[X] $. For fand g to be relatively prime it is necessary and sufficient that the canonical image of g in $ K[X]/(f) $ should be invertible.
    For this condition means that there exist $ u, v \in K[X] $ such that $ uf + vg = 1 $.

#### Corollary 6 {#alg-iv-s1-def-1-cor-6 .statement}

— Let $ f, g_1, g_2, ..., g_n \in K[X] $. If f is prime to $ g_1, g_2, ..., g_n $, then f is prime to $ g_1g_2...g_n $.

\* COROLLARY 7. — For f and g to be relatively prime it is necessary and sufficient that they have no common roots in any extension of K.
    For if d is a gcd of f, g then the roots common to f and g in an extension K' of K are the roots of d in K'. Now the corollary follows from V, p. 21, Prop. 4.

### 8. Irreducible polynomials

#### Definition 2 {#alg-iv-s1-def-2 .statement}

— Let K be a commutative field. We say that $ f \in K[X] $ is irreducible if $ \deg f \geq 1 $ and f is not divisible by any polynomial g such that $ 0 < \deg g < \deg f $.
    It comes to the same to say that $ \deg f \geq 1 $ and the only divisors of f in $ K[X] $ are the scalars $ \neq 0 $ and the products of f by scalars $ \neq 0 $. Since the relation $ (f) \subset (g) $ means that g divides f, we see that the irreducible polynomials of $ K[X] $ may also be defined as the polynomials f such that the ideal $ (f) $ is maximal (I, p. 104).

    Let $ f, g \in K[X] $. Iff is irreducible, it is clear that either f and g are relatively prime or that f divides g. If f and g are irreducible, either f and g are relatively prime or each is a product of the other by a scalar $ \neq 0 $. In particular, two distinct irreducible monic polynomials are relatively prime.

#### Proposition 13 {#alg-iv-s1-prop-13 .statement}

— Let $ \mathcal{I} $ be the set of irreducible monic polynomials in $ K[X] $. Let f be a non-zero element of $ K[X] $ and a its leading coefficient; then there exists precisely one family of positive integers $(v_p)_{p \in \mathcal{S}}$ with finite support, such that we have a decomposition

$$
f = \alpha \prod_{p \in \mathcal{S}} p^{v_p}.
$$

It suffices to prove the proposition when $f$ is monic, that is when $\alpha = 1$. We shall argue by induction on the degree $n$ off, the case $n = 0$ being trivial. Suppose then that $n \geq 1$ and that the proposition has been established for all polynomials of degree $< n$.

Let $E$ be the set of monic polynomials $\neq 1$ which divide $f$; we have $f \in E$ hence $E$ is not empty and there exists in $E$ a polynomial $g$ of least degree. It is clear that $g$ is irreducible and there exists a monic polynomial $h$ of degree $< n$ such that $f = gh$; by the induction hypothesis $h$ is the product of a finite family of irreducible monic polynomials, hence $f$ has the same property. This proves the existence of the decomposition (18).

Let us now prove the uniqueness of the decomposition (18). Let $(w_p)_{p \in \mathcal{S}}$ be a family of positive integers with finite support, such that $f = \prod_{p \in \mathcal{S}} p^{w_p}$. Since $f$ is of degree $n \geq 1$, there exists $p \in \mathcal{S}$ such that $w_p > 0$; if we had $v_p = 0$, $f$ would be the product of a family of elements of $\mathcal{S}$ distinct from $p$, hence it would be prime to $p$ (IV, p. 13, Cor. 6), contrary to the fact that $p$ divides $f$. By the induction hypothesis the polynomial $f/p$ admits a unique decomposition of type (18); hence we conclude the equality $w_q = v_q$ for every $q \in \mathbf{4}$.

Let $f$ be a non-zero polynomial in $\mathbf{K}[X]$. We shall say that $f$ has no multiple factors if the exponents $v_p$ in the decomposition (18) are all $\leq 1$; it comes to the same to say that $f$ is the product of a finite sequence of pairwise distinct irreducible polynomials, or also that $f$ is not divisible by the square of any non-constant polynomial of $\mathbf{K}[X]$.

### Exercises {#alg-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).

[^1]: The reader will note the analogy between the results of this No. and the next and the divisibility properties of the ring $Z$ of integers (I, p. 112). They depend essentially on the fact that in the rings $Z$ and $K[X]$ every ideal is principal, as we shall see in Chapter VII, § 1.
