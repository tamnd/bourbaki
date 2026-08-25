---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 5
section_title: Tensor algebra. Tensors
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0508-0521, 0651-0656
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE TENSOR ALGEBRA OF A MODULE
      page: 0
      pdf_page: 508
    - "no": 2
      title: FUNCTORIAL PROPERTIES OF THE TENSOR ALGEBRA
      page: 0
      pdf_page: 509
    - "no": 3
      title: EXTENSION OF THE RING OF SCALARS
      page: 0
      pdf_page: 513
    - "no": 4
      title: DIRECT LIMIT OF TENSOR ALGEBRAS
      page: 0
      pdf_page: 514
    - "no": 5
      title: TENSOR ALGEBRA OF A DIRECT SUM. TENSOR ALGEBRA OF A FREE MODULE. TENSOR ALGEBRA OF A GRADED MODULE
      page: 0
      pdf_page: 515
    - "no": 6
      title: TENSORS AND TENSOR NOTATION
      page: 0
      pdf_page: 516
statements: 15
exercises: 10
content_sha256: b5d2c4d338f5f14e72a546cc28face151c0373270a46c913792640245344c1fc
---

## § 5. TENSOR ALGEBRA, TENSORS

### 1. DEFINITION OF THE TENSOR ALGEBRA OF A MODULE

Let A be a commutative ring and M an A-module. For every integer $ n \geqslant 0 $, the A-module the tensor product of $ n $ modules equal to M (also called the *n-th tensor power* of M) is denoted by $ \bigotimes^n M $, or $ M^{\otimes n} $, or $ T^n(M) $, or $ T^n_A(M) $, or $ \mathrm{Tens}^n(M) $; then $ T^1(M) = M $; also we write $ T^0(M) = A $. The A-module the *direct sum* $ \bigoplus_{n \geqslant 0} T^n(M) $ is denoted by $ T(M) $ or $ \mathrm{Tens}(M) $. We shall define a graded A-algebra structure of type $ \mathbf{N} $ on $ T(M) $, by defining for every ordered pair of integers $ p \geqslant 0, q \geqslant 0 $, an A-linear mapping
$$
m_{pq} : T^p(M) \otimes_A T^q(M) \to T^{p+q}(M)
$$
($ \S 3 $, no. 1, *Remark*). For $ p > 0 $ and $ q > 0 $, $ m_{pq} $ is the associativity isomorphism (II, $ \S 3 $, no. 9) and, when $ p = 0 $ (resp. $ q = 0 $), $ m_{0,q} $ is the canonical isomorphism of $ A \otimes_A T^q(M) $ onto $ T^q(M) $ (resp. $ m_{p,0} $ is the canonical isomorphism of $ T^p(M) \otimes_A A $ onto $ T^p(M) $ (II, $ \S 3 $, no. 4, Proposition 4)). Then, for $ x_i \in M $, $ \alpha \in A $,
$$
\begin{align}
(x_1 \otimes \cdots \otimes x_p) \cdot (x_{p+1} \otimes \cdots \otimes x_{p+q}) &= x_1 \otimes \cdots \otimes x_p \otimes x_{p+1} \otimes \cdots \otimes x_{p+q} \\
\alpha \cdot (x_1 \otimes \cdots \otimes x_p) &= \alpha(x_1 \otimes \cdots \otimes x_p).
\end{align}
$$
It is immediate that the multiplication thus defined on $ T(M) $ is *associative* and admits as unit element the unit element 1 of $ A = T^0(M) $.

#### Definition 1 {#alg-iii-s5-def-1 .statement}

For every module $ M $ over a commutative ring $ A $, the tensor algebra of $ M $, denoted by $ T(M) $, or $ \mathrm{Tens}(M) $, or $ T_A(M) $, is the algebra $ \bigoplus_{n \geq 0} T^n(M) $ with the multiplication defined in (1). The canonical injection $ \phi : T^1(M) \to T(M) $ (II, § 1, no. 12) (also denoted by $ \phi_M $) is called the canonical injection of $ M $ into $ T(M) $.

#### Proposition 1 {#alg-iii-s5-prop-1 .statement}

Let $ E $ be a (unital) $ A $-algebra and $ f : M \to E $ an $ A $-linear mapping. There exists one and only one $ A $-algebra homomorphism $ g : T(M) \to E $ such that $ f = g \circ \phi $.

In other words, $ (T(M), \phi) $ is a solution of the universal mapping problem (Set Theory, IV, § 3, no. 1), where $ \Sigma $ is the species of $ A $-algebra structure, the $ \alpha $-mappings being the $ A $-linear mappings from the module $ M $ to an $ A $-algebra. Observe that here there is no question of a graduation on $ T(M) $.

For every finite family $ (x_i)_{1 \leq i \leq n} $ of $ n $ elements of $ M $, by definition of the product in $ T(M) $, $ x_1 \otimes x_2 \otimes \cdots \otimes x_n = \phi(x_1)\phi(x_2)\ldots\phi(x_n) $; then necessarily $ g(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1)f(x_2)\ldots f(x_n) $ for $ n \geq 1 $ and $ g(\alpha) = \alpha e $ (if $ e $ is the unit element of $ E $) for $ \alpha \in A $, which proves the uniqueness of $ g $. Conversely, note that, for all $ n > 0 $, the mapping
$$
(x_1, \ldots, x_n) \mapsto f(x_1)f(x_2)\ldots f(x_n)
$$
of $ M^n $ into $ E $ is $ A $-multilinear; hence there corresponds to it an $ A $-linear mapping $ g_n : T^n(M) \to E $ such that
$$
g(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1)f(x_2)\ldots f(x_n).
$$
Also we define the mapping $ g_0 : T^0(M) \to E $ as equal to $ \eta_E $ ($ \S 1 $, no. 3), in other words $ g_0(\alpha) = \alpha e $ for $ \alpha \in A $. Let $ g $ be the unique $ A $-linear mapping of $ T(M) $ into $ E $ whose restriction to $ T^n(M) $ is $ g_n $ ($ n \geq 0 $); it is immediate that $ g \circ \phi = g_1 = f $ and it remains to verify that $ g $ is an $ A $-algebra homomorphism. By construction $ g(1) = e $ and it suffices by linearity to show that $ g(uv) = g(u)g(v) $ for $ u \in T^p(M) $ and $ v \in T^q(M) $ ($ p > 0, q > 0 $); now it follows from formulae (1) and (2) that this relation is true when $ u = x_1 \otimes x_2 \otimes \cdots \otimes x_p $ and $ v \in x_{p+1} \otimes \cdots \otimes x_{p+q} $ (where the $ x_i $ belong to $ E $). It is therefore true for $ u \in T^p(M) $ and $ v \in T^q(M) $ by linearity.

#### Remark {#alg-iii-s5-n1-rem-1 .statement}

Suppose that $ E $ is a graded $ A $-algebra of type $ \mathbf{Z} $, with graduation $ (E_n) $, and suppose also that
$$
f(M) \subset E_1.
$$
Then it follows from (2) that $ g(T^p(M)) \subset E_p $ for all $ p \geq 0 $ and hence $ g $ is a graded algebra homomorphism.

### 2. FUNCTORIAL PROPERTIES OF THE TENSOR ALGEBRA

#### Proposition 2 {#alg-iii-s5-prop-2 .statement}

Let $ A $ be a commutative ring, $ M $ and $ N $ two $ A $-modules and
$$
u : M \to N
$$

an A-linear mapping. There exists one and only one A-algebra homomorphism

$$
u': \mathbf{T}(M) \to \mathbf{T}(N)
$$

such that the diagram

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M & & \downarrow \phi_N \\
\mathbf{T}(M) & \xrightarrow{u'} & \mathbf{T}(N)
\end{array}
$$

is commutative. Further, $ u' $ is a graded algebra homomorphism.

The existence and uniqueness of $ u' $ follow from no. 1, Proposition 1, applied to the algebra $ \mathbf{T}(N) $ and the linear mapping $ \phi_N \circ u : M \to \mathbf{T}(N) $; as

$$
u(M) \subset \mathbf{T}^1(N) = N,
$$

the fact that $ u' $ is a graded algebra homomorphism follows from the Remark of no. 1.

The homomorphism $ u' $ of Proposition 2 will henceforth be denoted by $ \mathbf{T}(u) $. If P is an A-module and $ v : N \to P $ an A-linear mapping, then

$$
\mathbf{T}(v \circ u) = \mathbf{T}(v) \circ \mathbf{T}(u)
$$

for $ \mathbf{T}(v) \circ \mathbf{T}(u) $ is an algebra homomorphism rendering commutative the diagram

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\downarrow \phi_M & & \downarrow \phi_P \\
\mathbf{T}(M) & \xrightarrow{\mathbf{T}(v) \circ \mathbf{T}(u)} & \mathbf{T}(P)
\end{array}
$$

$ \mathbf{T}(u) $ is sometimes called the canonical extension of $ u $ to $ \mathbf{T}(M) $ (which contains $ M = \mathbf{T}^1(M) $). Note that the restriction $ \mathbf{T}^n(u) : \mathbf{T}^n(M) \to \mathbf{T}^n(N) $ is just the linear mapping $ u^{\otimes n} = u \otimes u \otimes \cdots \otimes u $ (n times), for

$$
\mathbf{T}^n(u)(x_1 \otimes \cdots \otimes x_n) = u(x_1) \otimes \cdots \otimes u(x_n)
$$

since $ \mathbf{T}(u) $ is an algebra homomorphism and $ \mathbf{T}^1(u) = u $; the restriction $ \mathbf{T}^0(u) $ to A is the identity mapping. $ \mathbf{T}^n(u) $ is called the $ n $-th tensor power of $ u $.

#### Proposition 3 {#alg-iii-s5-prop-3 .statement}

*If $ u : M \to N $ is a surjective A-linear mapping, the homomorphism $ \mathbf{T}(u) : \mathbf{T}(M) \to \mathbf{T}(N) $ is surjective and its kernel is the two-sided ideal of $ \mathbf{T}(M) $ generated by the kernel $ P \subset M \subset \mathbf{T}(M) $ of $ u $.*

$ \mathbf{T}^0(u) : \mathbf{T}^0(M) \to \mathbf{T}^0(N) $ is bijective and for every integer $ n > 0 $,

$$
\mathbf{T}^n(u) : \mathbf{T}^n(M) \to \mathbf{T}^n(N)
$$

is surjective, as is seen by induction on $ n $ using II, § 3, no. 6, Proposition 6; the latter proposition also shows, by induction on $ n $, that the kernel $ \mathfrak{I}_n $ of $ T^n(u) $ is the submodule of $ T^n(M) $ generated by the products
$$
x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$
where at least one of the $ x_i $ belongs to $ P $. This shows that the kernel $ \mathfrak{I} = \bigoplus_{n \geq 1} \mathfrak{I}_n $ of $ T(u) $ is the two-sided ideal generated by $ P $ in $ T(M) $.

If $ u : M \to N $ is an *injective* linear mapping, it is not always true that $ T(u) $ is an injective mapping (Exercise 1). However, this is true when $ u $ is an injection such that $ u(M) $ is a *direct factor* of $ N $, for then there exists a linear mapping $ v : N \to M $ such that $ v \circ u $ is the identity mapping on $ M $ and therefore
$$
T(v \circ u) = T(v) \circ T(u)
$$
is the identity mapping on $ T(M) $, hence $ T(u) $ is injective and its image (isomorphic to $ T(M) $) is a *direct factor* of $ T(N) $ (II, § 1, no. 9, Proposition 15). More precisely:

#### Proposition 4 {#alg-iii-s5-prop-4 .statement}

*Let $ N $ and $ P $ be two submodules of an $ A $-module $ M $ such that their sum $ N + P $ is a direct factor in $ M $ and their intersection $ N \cap P $ is a direct factor in $ N $ and in $ P $. Then the homomorphisms $ T(N) \to T(M) $, $ T(P) \to T(M) $ and*
$$
T(N \cap P) \to T(M),
$$
*canonical extensions of the canonical injections, are injective; if $ T(N) $, $ T(P) $ and $ T(N \cap P) $ are identified with subalgebras of $ T(M) $ by means of these homomorphisms, then*
(5)
$$
T(N \cap P) = T(N) \cap T(P).
$$

By hypothesis, there exist submodules $ N' \subset N $ and $ P' \subset P $ such that $ N = N' \oplus (N \cap P) $, $ P = P' \oplus (N \cap P) $; then
$$
N + P = N' \oplus P' \oplus (N \cap P)
$$
and there exists by hypothesis a submodule $ M' $ of $ M $ such that
$$
M = M' \oplus (N + P) = M' \oplus N' \oplus P' \oplus (N \cap P) \\
= M' \oplus P' \oplus N = M' \oplus N' \oplus P.
$$

In particular, $ N + P $, $ N $, $ P $ and $ N \cap P $ are direct factors in $ M $, which implies, as has been seen above, that the canonical homomorphisms
$$
T(N + P) \to T(M), \quad T(N) \to T(M),
$$
$$
T(P) \to T(M), \quad T(N \cap P) \to T(M)
$$
are injective. The three algebras $ T(N) $, $ T(P) $ and $ T(N \cap P) $ are thus identified with subalgebras of $ T(N + P) $ and the latter with a subalgebra of $ T(M) $;

writing $ Q = N \cap P $, it remains to show that, if $ T(Q) $, $ T(N' \oplus Q) $ and $ T(P' \oplus Q) $ are identified with subalgebras of $ T(N' \oplus P' \oplus Q) $, then

$$
T(N' \oplus Q) \cap T(P' \oplus Q) = T(Q).
$$

Now, consider the commutative diagram

$$
\begin{array}{ccc}
N' \oplus Q & \longrightarrow & N' \oplus P' \oplus Q \\
\downarrow & & \downarrow \\
Q & \longrightarrow & P' \oplus Q
\end{array}
$$

where the horizontal arrows are the canonical injections and the vertical arrows the canonical projections. We derive a commutative diagram

$$
\begin{array}{ccc}
T(N' \oplus Q) & \overset{u}{\longrightarrow} & T(N' \oplus P' \oplus Q) \\
\downarrow r & & \downarrow s \\
T(Q) & \overset{v}{\longrightarrow} & T(P' \oplus Q)
\end{array}
$$

where $ r $ and $ s $ are surjective homomorphisms (Proposition 3) and $ u $ and $ v $ injective homomorphisms. Hence, to prove (6), note that the right hand side is obviously contained in the left; it therefore suffices to verify that if

$$
x \in T(N' \oplus Q) \cap T(P' \oplus Q),
$$

then $ x \in T(Q) $. Now the definition of the homomorphism $ s $ shows that its restriction to $ T(P' \oplus Q) $ (identified with a subalgebra of $ T(N' \oplus P' \oplus Q) $) is the identity mapping; the hypothesis on $ x $ therefore implies that $ s(u(x)) = x $. But then also $ v(r(x)) = x $, in other words $ x $ belongs to the image of $ T(Q) $ in $ T(P' \oplus Q) $, which was to be proved.

#### Remark {#alg-iii-s5-n2-rem-1 .statement}

Note in particular that the hypotheses of Proposition 4 always hold for arbitrary submodules $ N, P $ of $ M $ when $ A $ is a field (II, § 7, no. 3, Proposition 4). Moreover, if $ N \subset P $ and $ N \neq P $, then $ T^n(N) \neq T^n(P) $ for all $ n \geq 1 $, since if $ R $ is a complement of $ P $ in $ N $, then $ T^n(P) \cap T^n(R) = \{0\} $ by (4) and $ T^n(R) \neq \{0\} $.

#### Corollary {#alg-iii-s5-n2-cor-1 .statement}

*Let $ K $ be a commutative field and $ M $ a vector space over $ K $. For every element $ z \in T(M) $, there exists a smallest vector space $ N $ of $ M $ such that $ z \in T(N) $ and $ N $ is of finite rank over $ K $.*

It is understood in this statement that for every vector subspace $ P $ of $ M $, $ T(P) $ is canonically identified with a subalgebra of $ T(M) $. Let $ z \in T(M) $; $ z $ can be expressed as a linear combination of elements each of which is a finite product of elements of $ M = T^1(M) $; all the elements of $ M $ which occur in these products generate a vector subspace $ Q $ of finite rank and $ z \in T(Q) $.

Let $ \mathcal{F} $ be the (non-empty) set of vector subspaces $ P $ of finite rank such that $ z \in T(P) $. Every decreasing sequence of elements of $ \mathcal{F} $ is stationary, since they are vector spaces of finite rank. Hence $ \mathcal{F} $ has a minimal element $ N $ (Set Theory, III, § 6, no. 5). It remains to verify that every $ P \in \mathcal{F} $ contains $ N $; now, $ z \in T(P) \cap T(N) = T(P \cap N) $ (Proposition 4); in view of the definition of $ N $, this implies $ N \cap P = N $, that is $ P \supset N $.

The subspace $ N $ of $ M $ is said to be *associated* with $ z $.

### 3. EXTENSION OF THE RING OF SCALARS

Let $ A, A' $ be two commutative rings and $ \rho : A \to A' $ a ring homomorphism. Let $ M $ be an $ A $-module, $ M' $ an $ A' $-module and $ u : M \to M' $ an $ A $-homomorphism; as the canonical injection $ \phi_{M'} : M' \to T_{A'}(M') $ is also an $ A $-homomorphism (by restriction of scalars), so is the composition $ M \xrightarrow{u} M' \xrightarrow{\phi_{M'}} T_{A'}(M') $. An $ A $-algebra homomorphism $ T_A(M) \to \rho^*(T_{A'}(M')) $ is derived (no. 2), also denoted by $ T(u) : T_A(M) \to T_{A'}(M') $, which is the unique $ A $-homomorphism rendering commutative the diagram

$$
\begin{array}{ccc}
M & \xrightarrow{u} & M' \\
\downarrow \phi_M & & \downarrow \phi_{M'} \\
T_A(M) & \xrightarrow{T(u)} & T_{A'}(M')
\end{array}
$$

If $ \sigma : A' \to A'' $ is a commutative ring homomorphism, $ M'' $ an $ A'' $-module and $ v : M' \to M'' $ an $ A' $-homomorphism, the above uniqueness property shows that

$$
T(v \circ u) = T(v) \circ T(u).
$$

#### Proposition 5 {#alg-iii-s5-prop-5 .statement}

*Let $ A, B $ be two commutative rings, $ \rho : A \to B $ a ring homomorphism and $ M $ an $ A $-module. The canonical extension*

$$
\psi : T_B(B \otimes_A M) \to B \otimes_A T_A(M)
$$

*of the B-linear mapping* $ l_B \otimes \phi_M : B \otimes_A M \to B \otimes_A T_A(M) $ *is an isomorphism of graded B-algebras*.

Consider the two $ A $-algebra homomorphisms: the canonical injection $ j : B = T^0(B \otimes_A M) \to T(B \otimes_A M) $ and the homomorphism

$$
h = T(i) : T(M) \to T(B \otimes_A M)
$$

derived (cf. formula (8)) from the canonical $ A $-linear mapping

$$
i : M \to B \otimes_A M.
$$

As $ T^0(B \otimes_A M) $ is contained in the centre of $ T(B \otimes_A M) $, Proposition 5 of § 4, no. 2 can be applied and an A-algebra homomorphism

$$
\psi': B \otimes_A T(M) \to T(B \otimes_A M)
$$

is obtained such that, for $ \beta \in B, x_i \in M $ for $ 1 \leq i \leq n $,

$$
\psi'(\beta \otimes (x_1 \otimes x_2 \otimes \cdots \otimes x_n)) = \beta((1 \otimes x_1) \otimes (1 \otimes x_2) \otimes \cdots \otimes (1 \otimes x_n)),
$$

which shows immediately that $ \psi' $ is also a B-algebra homomorphism. It suffices to prove that $ \psi \circ \psi' $ and $ \psi' \circ \psi $ are the identity mappings on $ B \otimes_A T(M) $ and $ T(B \otimes_A M) $ respectively. Now, these two algebras are generated by $ B \otimes_A M $ and clearly $ \psi \circ \psi' $ and $ \psi' \circ \psi $ coincide with the identity mapping on $ B \otimes_A M $, whence the conclusion.

### 4. DIRECT LIMIT OF TENSOR ALGEBRAS

Let $ (A_\alpha, \phi_{\beta \alpha}) $ be a directed direct system of commutative rings and $ (M_\alpha, f_{\beta \alpha}) $ a direct system of $ A_\alpha $-modules (II, § 6, no. 2); let $ A = \lim \rightarrow A_\alpha $ and $ M = \lim \rightarrow M_\alpha $, which is an $ A $-module. For $ \alpha \leq \beta $ an $ A_\alpha $-algebra homomorphism (no. 3, formula (8)) $ f'_{\beta \alpha} = T(f_{\beta \alpha}): T_{A\alpha}(M_\alpha) \to T_{A\beta}(M_\beta) $ is derived canonically from the $ A_\alpha $-homomorphism $ f_{\beta \alpha}: M_\alpha \to M_\beta $ and it follows from (9) (no. 3) that $ (T_{A\alpha}(M_\alpha), f'_{\beta \alpha}) $ is a *direct system of $ A_\alpha $-algebras*. On the other hand let $ f'_\alpha: M_\alpha \to M $ be the canonical $ A_\alpha $-homomorphism; an $ A_\alpha $-algebra homomorphism $ f'_\alpha: T_{A\alpha}(M_\alpha) \to T_A(M) $ is derived (no. 3, formula (8)) and it also follows from (9) (no. 3) that the $ f'_\alpha $ constitute a direct system of $ A_\alpha $-homomorphisms.

#### Proposition 6 {#alg-iii-s5-prop-6 .statement}

*The A-homomorphism* $ f' = \lim \rightarrow f'_\alpha : \lim \rightarrow T_{A\alpha}(M_\alpha) \to T_A(M) $ *is a graded algebra isomorphism*.

To simplify we write $ E = T_A(M) $ and $ E' = \lim \rightarrow T_{A\alpha}(M_\alpha) $ and let

$$
g_\alpha: T_{A\alpha}(M_\alpha) \to E'
$$

be the canonical $ A_\alpha $-homomorphism. Clearly the composite $ A_\alpha $-linear mappings $ M_\alpha \xrightarrow{\phi_{M_\alpha}} T_{A\alpha}(M_\alpha) \xrightarrow{g_\alpha} E' $ form a direct system and there is therefore one and only one $ A $-linear mapping $ u = \lim \rightarrow (g_\alpha \circ \phi_{M_\alpha}): M \to E' $ such that

$$
u \circ f_\alpha = g_\alpha \circ \phi_{M_\alpha}
$$

for all $ \alpha $. This mapping itself factorizes uniquely (no. 1, Proposition 1) into $ M \xrightarrow{\phi_M} E \to E' $, where $ h $ is an $ A $-algebra homomorphism. It will suffice to prove that $ h \circ f' = 1_{E'} $ and $ f' \circ h = 1_E $.

To this end note that, for every index $ \alpha $, (no. 3, formula (8))

$$
h \circ f'_\alpha \circ \phi_{M_\alpha} = h \circ \phi_M \circ f_\alpha = u \circ f_\alpha = g_\alpha \circ \phi_{M_\alpha}
$$

whence, by the uniqueness assertion of no. 1, Proposition 1,

$$
h \circ f'_\alpha = g_\alpha
$$

for all $ \alpha $; it follows that $ (h \circ f') \circ g_\alpha = g_\alpha $ for all $ \alpha $ and hence $ h \circ f' = 1_{E'} $ by definition of a direct limit.

On the other hand, by virtue of no. 3, formula (8),

$$
f' \circ u \circ f_\alpha = f' \circ g_\alpha \circ \phi_{M_\alpha} = f'_\alpha \circ \phi_{M_\alpha} = \phi_M \circ f_\alpha,
$$

whence again $ f' \circ u = \phi_M $ by definition of a direct limit; we conclude that $ f' \circ h \circ \phi_M = \phi_M $ and the uniqueness property of no. 1, Proposition 1 gives $ f' \circ h = 1_E $.

Proposition 6 can also be shown by observing that, for every integer $ n \geq 1 $, there is a canonical $ A $-module isomorphism $ \lim \rightarrow T^n_{A_\alpha}(M_\alpha) \to T^n_A(M) $, as follows by induction on $ n $ from II, § 6, no. 3, Proposition 7. It is immediately verified that these isomorphisms are the restrictions of $ f' $.

### 5. TENSOR ALGEBRA OF A DIRECT SUM. TENSOR ALGEBRA OF A FREE MODULE. TENSOR ALGEBRA OF A GRADED MODULE

Let $ A $ be a commutative ring and $ M = \bigoplus_{\lambda \in L} M_\lambda $ the direct sum of a family of $ A $-modules. It follows from II, § 3, no. 7, Proposition 7, by induction on $ n $, that $ T^n(M) $ is the direct sum of the submodules the images of the canonical injections

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n} \to T^n(M) = M^{\otimes n}
$$

relative to *all* the sequences $ (\lambda_i) \in L^n $. Identifying $ M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n} $ with this image, it is seen that $ T(M) $ is the *direct sum of all the modules*

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n}
$$

where $ n $ runs through $ \mathbf{N} $ and, for each $ n $, $ (\lambda_i) $ runs through $ L^n $.

We first deduce the following consequence:

#### Theorem 1 {#alg-iii-s5-thm-1 .statement}

*Let $ A $ be a commutative ring, $ M $ a free $ A $-module and $ (e_\lambda)_{\lambda \in L} $ a basis of $ M $. Then the elements $ e_s = e_{\lambda_1} \otimes e_{\lambda_2} \otimes \cdots \otimes e_{\lambda_n} $, where $ s = (\lambda_1, \ldots, \lambda_n) $ runs through the set of all finite sequences of elements of $ L $ and $ e_\varnothing $ is used to denote the unit element of $ T(M) $, form a basis of the $ A $-module $ T(M) $.*

The elements of this basis are obviously homogeneous and the multiplication table is given by

$$
e_s e_t = e_{st}
$$

where $ st $ denotes the sequence of elements of $ L $ obtained by *juxtaposing* the sequences $ s $ and $ t $ (I, § 7, no. 2).

It is seen that the basis $(e_s)$ of $T(M)$, with the multiplicative law (10), is canonically isomorphic to the *free monoid* of the set $L$ (I, § 7, no. 2), the isomorphism being obtained by mapping each word $s$ of this monoid to the element $e_s$. It follows (\S 2, no. 7) that *the tensor algebra $T(M)$ of a free module $M$, with a basis of indexing set $L$, is canonically isomorphic to the free associative algebra of $L$ over $A$*. In particular (\S 2, no. 7, Proposition 7), for every mapping $f : L \to E$ from $L$ to an $A$-algebra $E$, there exists one and only one $A$-algebra homomorphism $\bar{f} : T(M) \to E$ such that $\bar{f}(e_\lambda) = f(\lambda)$.

#### Remark {#alg-iii-s5-n5-rem-1 .statement}

The above results can equally be obtained as a consequence of the universal properties of the free associative algebra of the tensor algebra, using II, § 3, no. 7, Corollary 2 to Proposition 7.

#### Corollary {#alg-iii-s5-n5-cor-1 .statement}

*If $M$ is a projective $A$-module, $T(M)$ is a projective $A$-module.*

$M$ is a direct factor of a free $A$-module $N$ (II, § 2, no. 2, Proposition 4) and hence $T(M)$ is a direct factor of $T(N)$ (no. 2); as $T(N)$ is free (Theorem 1), this shows that $T(M)$ is projective (II, § 2, no. 2).

#### Proposition 7 {#alg-iii-s5-prop-7 .statement}

*Let $\Delta$ be a commutative monoid, $M$ a graded $A$-module of type $\Delta$ and $(M_\alpha)_{\alpha \in \Delta}$ its graduation. For every ordered pair $(\alpha, n) \in \Delta \times \mathbf{N}$, let $T^{\alpha, n}(M)$ be the (direct) sum of the submodules $M_{\alpha_1} \otimes M_{\alpha_2} \otimes \cdots \otimes M_{\alpha_n}$ of $T^n(M)$ such that $\sum_{i=1}^n \alpha_i = \alpha$; then $(T^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ is the only graduation of type $\Delta \times \mathbf{N}$ compatible with the algebra structure on $T(M)$ and inducing on $M = T^1(M)$ the given gradation.*

It has been seen at the beginning of this no. that $T(M)$ is the direct sum of the $T^{\alpha, n}(M)$ and the fact that this is a graduation compatible with the algebra structure follows immediately from the definitions. If $({T'}^{\alpha, n})$ is another graduation of type $\Delta \times \mathbf{N}$ on $T(M)$ compatible with the algebra structure and such that ${T'}^{\alpha, 1}(M) = {T'}^{\alpha, 1}$ for $\alpha \in \Delta$, it follows immediately from the definitions that, for all $n \geq 1$ and all $\alpha \in \Delta$, $T^{\alpha, n}(M) \subset {T'}^{\alpha, n}$; but since $T(M)$ is also the direct sum of the $T^{\alpha, n}(M)$, this implies that ${T'}^{\alpha, n} = T^{\alpha, n}(M)$ (II, § 1, no. 8, *Remark*).

### 6. TENSORS AND TENSOR NOTATION

Let $A$ be a commutative ring, $M$ an $A$-module, $M^*$ the *dual* of $M$ (II, § 2, no. 3) and $I$ and $J$ two *disjoint finite* sets; the $A$-module $\bigotimes_{i \in I \cup J} E_i$, where $E_i = M$ if $i \in I$, $E_i = M^*$ if $i \in J$, is denoted by $T^I_J(M)$; the elements of $T^I_J(M)$ are called *tensors of type* $(I, J)$ over $M$. They are called *contravariant* if $J = \varnothing$, *covariant* if $I = \varnothing$ and *mixed* otherwise.

Let $I', I''$ be two subsets of $I$ and $J', J''$ two subsets of $J$ such that $I' \cup I'' = I$,

$ I' \cap I'' = \varnothing,\ J' \cup J'' = J,\ J' \cap J'' = \varnothing $; then there is a canonical associativity isomorphism (II, § 3, no. 9)

$$
T_J^I(M) \to T_{J'}^{I'}(M) \otimes_A T_{J''}^{I''}(M).
$$

Considering the tensor algebra $ T(M \oplus M^*) $, it follows from no. 5 that $ T^n(M \oplus M^*) $ is canonically identified with the direct sum of the $ T_J^I(M) $ where I runs through the set of subsets of the interval $ \{1, n\} $ of $ \mathbf{N} $ and $ J $ is the complement of I in $ \{1, n\} $.

When $ I = \{1, p\} $ and $ J = \{p + 1, p + q\} $ with integers $ p \geq 0,\ q \geq 0 $ (where we replace I (resp. J) by $ \varnothing $ when $ p = 0 $ (resp. $ q = 0 $)), the A-module $ T_J^I(M) $ is also denoted by $ T_q^p(M) $; the A-modules $ T_0^n(M) $ and $ T_n^0(M) $ are therefore by definition the A-modules $ T^n(M) $ and $ T^n(M^*) $ respectively. When I and J are arbitrary finite sets of cardinals $ p = \mathrm{Card}(I) $ and $ q = \mathrm{Card}(J) $, we give each of them a total ordering; then there exists an increasing bijection of I (resp. J) onto $ \{1, p\} $ (resp. $ \{p + 1, p + q\} $) and these bijections therefore define an isomorphism

$$
T_J^I(M) \to T_q^p(M).
$$

When M is a *finitely generated projective* A-module, it follows from II, § 2, no. 7, Corollary 4 to Proposition 13 and II, § 4, no. 4, Corollary 1 to Proposition 4 that there is a canonical isomorphism

$$
(T_J^I(M))^* \to T_I^J(M).
$$

Suppose now that M is a *finitely generated free* A-module and let $ (e_\lambda)_{\lambda \in L} $ be a basis of M (L therefore being a *finite* set). The basis of $ M^* $ *dual* to $ (e_\lambda) $ (II, § 2, no. 6) is denoted by $ (e^\lambda)_{\lambda \in L} $. The bases $ (e_\lambda) $ and $ (e^\lambda) $ of M and $ M^* $ respectively define (no. 5) a basis of $ T_J^I(M) $, which we give explicitly as follows: given two mappings $ f : I \to L $ and $ g : J \to L $, let $ e_f^g $ be the element $ \bigotimes_{i \in I \cup J} x_i $ of $ T_J^I(M) $ defined by

$$
x_i = e_{f(i)} \quad \text{if } i \in I, \qquad x_i = e_{g(i)} \quad \text{if } i \in J.
$$

When $ (f, g) $ runs through the set of ordered pairs of mappings $ f : I \to L $ and $ g : J \to L $, the $ e_f^g $ form a *basis* of the A-module $ T_J^I(M) $, said to be *associated* with the given basis $ (e_\lambda) $ of M. For $ z \in T_J^I(M) $, we can therefore write

$$
z = \sum_{(f, g)} \alpha_g^f(z) \cdot e_f^g
$$

where the $ \alpha_g^f $ are the coordinate forms relative to the basis $ (e_f^g) $; by an abuse of language, the $ \alpha_g^f(z) $ are called the coordinates of the tensor $ z $ *with respect to the basis* $ (e_\lambda) $ of the module M. The $ \alpha_g^f $ constitute the dual basis of $ (e_f^g) $, in other words they are identified with the elements of the basis of $ T_I^J(M) $, *associated* with $ (e_\lambda) $. When I and J are complementary subsets of an interval $ \{1, n\} $ of $ \mathbf{N} $, $ \alpha_g^f $ (or $ \alpha_g^f(z) $) is denoted as follows: each element $ f(i) $ for $ i \in I $ is written as an upper index in the i-th place with a dot in the i-th place for $ i \in J $; similarly, $ g(i) $ for $ i \in J $ is written as a lower index in the i-th place with a dot in the i-th place for $ i \in I $. For example, for $ I = \{1, 4\}, J = \{2, 3\} $, we write $ \alpha_{v\rho}^{\lambda\cdot\cdot\mu} $: if $ f(1) = \lambda, f(4) = \mu, g(2) = \nu, g(3) = \rho $.

Let $ (\tilde{e}_{\lambda})_{\lambda \in L} $ be another basis of M and P the matrix of passing from $ (e_{\lambda}) $ to $ (\tilde{e}_{\lambda}) $ (II, § 10, no. 8). Then the matrix of passing from $ (e^{\lambda}) $ to $ (\tilde{e}^{\lambda}) $ (dual basis of $ (\tilde{e}_{\lambda}) $) is the contragredient $ ^tP^{-1} $ of P (II, § 10, no. 8, Proposition 5). It follows (II, § 10, no. 10) that the matrix of passing from the basis $ (e^{g}_{f}) $ of $ T^{I}_{J}(M) $ to the basis $ (\tilde{e}^{g}_{f}) $ (where $ f $ (resp. $ g $) runs through the set of mappings of I into L (resp. of J into L)) is the matrix

$$
\bigotimes_{i \in I \cup J} Q_{i}, \quad \text{where } Q_{i} = P \text{ if } i \in I, Q_{i} = {}^{t}P^{-1} \text{ if } i \in J.
$$

The transpose of this matrix is therefore identified with

$$
\bigotimes_{i \in I \cup J} R_{i}, \quad \text{where } R_{i} = {}^{t}P^{-1} \text{ if } i \in I, R_{i} = P \text{ if } i \in J.
$$

Suppose now that M is an arbitrary module. Let $ i \in I, j \in J $ and write $ I' = I - \{i\}, J' = J - \{j\} $; we shall define a canonical A-linear mapping

$$
c^{i}_{j}: T^{I}_{J}(M) \to T^{I'}_{J'}(M),
$$

called contraction of the index i and the index j. For this, note that the mapping of $ M^{I} \times (M^{*})^{J} $, which associates with every family $ (x_{i})_{i \in I \cup J} $, where $ x_{i} \in M $ if $ i \in I $ and $ x_{i} \in M^{*} $ if $ i \in J $, the element

$$
\langle x_{i}, x_{j} \rangle_{k \in (I \cup J) - \{i, j\}} x_{k}
$$

of $ T^{I'}_{J'}(M) $, is A-multilinear; $ c^{i}_{j} $ is the corresponding A-linear mapping.

Suppose now that M is free and finitely generated and let $ (e_{\lambda})_{\lambda \in L} $ be a basis of M. Given two mappings $ f: I \to L, g: J \to L $, let $ f_{i} $ denote the restriction of $ f $ to $ I' = I - \{i\} $ and $ g_{j} $ the restriction of $ g $ to $ J' = J - \{j\} $; then by virtue of (12)

$$
c^{i}_{j}(e^{g}_{f}) = \begin{cases} 0 & \text{if } f(i) \neq g(j) \\ e^{g_{j}}_{f_{i}} & \text{if } f(i) = g(j) \end{cases}
$$

The expression for the coordinates of $ c^{i}_{j}(z) $ as a function of those of z is obtained; for every mapping $ f' $ (resp. $ g' $) of I' into L (resp. of J' into L) and every $ \lambda \in L $, let $ (f', \lambda) $ (resp. $ (g', \lambda) $) denote the mapping of I into L (resp. of J into L) whose restriction to I' (resp. J') is $ f' $ (resp. $ g' $) and which takes the value $ \lambda $ at the element i (resp. j). Then, if the coordinate forms relative to the basis $ (e^{g'}_{f'}) $ of $ T^{I'}_{J'}(M) $ are denoted by $ \beta^{f'}_{g'} $,

$$
\beta^{f'}_{g'}(c^{i}_{j}(z)) = \sum_{\lambda \in L} \alpha^{(f'; \lambda)}_{(g'; \lambda)}(z).
$$

Examples of tensors. (1) Let M be a finitely generated projective A-module. We know (II, § 4, no. 2, Corollary to Proposition 2), that there is a canonical A-module isomorphism

$$
\theta_M : M^* \otimes_A M \to \operatorname{End}_A(M)
$$

such that $ \theta_M(x^* \otimes x) $ (for $ x \in M, x^* \in M^* $) is the endomorphism

$$
y \mapsto \langle y, x^*\rangle x.
$$

Hence, by means of $ \theta_M $, $ T^{(2)}_{\{1\}}(M) $ (isomorphic to $ T^1_1(M) $) can be identified with the A-module $ \operatorname{End}_A(M) $. Suppose that M is a free module and let $ (e_\lambda)_{\lambda \in L} $ be a basis of M; then the coordinates of a tensor $ z \in M^* \otimes M $ relative to the basis $ (e^\mu \otimes e_\lambda) $ of this module are denoted by $ \zeta_{\mu \cdot \lambda} $. As $ \theta_M(e^\mu \otimes e_\lambda) $ is the endomorphism $ y \mapsto \langle y, e^\mu\rangle e_\lambda $, the endomorphism $ u = \theta_M(z) = \theta_M\left( \sum_{\lambda, \mu} \zeta_{\mu \cdot \lambda} e^\mu \otimes e_\lambda \right) $ maps $ y $ to $ \sum_{\lambda, \mu} \zeta_{\mu \cdot \lambda} \langle y, e^\mu\rangle e_\lambda $; writing $ y = e_\lambda $, we obtain the relation

$$
u(e_\lambda) = \sum_{\mu \in L} \zeta_{\lambda \cdot \mu} e_\mu
$$

in other words, *the matrix of the linear mapping* $ u = \theta_M(z) $ *is that whose element in the row of index* $ \mu $ *and column of index* $ \lambda $ *is* $ \zeta_{\lambda \cdot \mu} $.

The definition of the *trace* of $ u $ (II, § 4, no. 3) shows immediately that

$$
\operatorname{Tr}(\theta_M(z)) = c_1^2(z).
$$

Therefore the element $ z_0 = \sum_{\lambda \in L} e^\lambda \otimes e_\lambda $ (whose coordinates $ \zeta_{\mu \cdot \lambda} $ are zero for $ \lambda \neq \mu $ and equal to 1 for $ \lambda = \mu $), which is such that $ \theta_M(z_0) = 1_M $, is the image of the element $ 1 \in A = T^0_0(M) $ under the mapping the *transpose of the contraction*

$$
c_1^2 : T^{(2)}_{\{1\}}(M) \to A.
$$

(2) Suppose always that M is a finitely generated projective A-module; there is a canonical A-module isomorphism

$$
\mu : M^* \otimes_A M^* \to (M \otimes_A M)^*
$$

(II, § 4, no. 4, Corollary 1 to Proposition 2) and a canonical isomorphism

$$
\theta : (M \otimes_A M)^* \otimes_A M \to \operatorname{Hom}_A(M \otimes_A M, M)
$$

(II, § 4, no. 2, Corollary to Proposition 2); also $ \operatorname{Hom}_A(M \otimes_A M, M) $ is canonically isomorphic to the A-module $ \mathcal{L}_2(M, M; M) $ of A-*bilinear* mappings of $ M \times M $ into $ M $ (II, § 3, no. 9). Composing these isomorphisms, a canonical isomorphism is obtained

$$
\chi_M : T^{(3)}_{\{1, 2\}}(M) = M^* \otimes M^* \otimes M \to \mathcal{L}_2(M, M; M)
$$

such that, for $ x^*, y^* $ in $ M^* $, $ z \in M $, $ \chi_M(x^* \otimes y^* \otimes z) $ is the bilinear mapping
$$
(u, v) \mapsto \langle u, x^*\rangle \langle v, y^*\rangle z.
$$
Hence, by means of $ \chi_M $, $ T_{\{1, 2\}}^{(3)}(M) $ (isomorphic to $ T_2^1(M) $) can be identified with the A-module $ \mathcal{L}_2(M, M; M) $. Suppose that M is a free A-module and let $ (e_\lambda)_{\lambda \in L} $ be a basis of M; then the coordinates of a tensor $ z \in M^* \otimes M^* \otimes M $ relative to the basis $ (e^\lambda \otimes e^\mu \otimes e_\nu) $ of this module are denoted by $ \zeta_{\lambda \mu \nu} $. The bilinear mapping $ \chi_M(z) $ maps the ordered pair $ (e_\lambda, e_\mu) $ to
$$
\sum_{\nu \in L} \zeta_{\lambda \mu \nu} e_\nu
$$
and therefore the $ \zeta_{\lambda \mu \nu} $ are just the *constants of structure* of the (in general non-associative) algebra defined on M by the bilinear mapping $ \chi_M(z) $, with respect to the basis $ (e_\lambda) $ (\S 1, no. 7).

#### Remark 2 {#alg-iii-s5-n6-rem-2 .statement}

Let $ (e_\lambda)_{\lambda \in L} $, $ (\bar{e}_\lambda)_{\lambda \in L} $ be two bases of M and P the matrix of passage from $ (e_\lambda) $ to $ (\bar{e}_\lambda) $. On account of what was seen in *Example 1*, the element of P appearing in the row of index $ \lambda $ and the column of index $ \mu $ is denoted by $ \alpha_\mu^\lambda $ and the element of the contragredient $ {}^tP^{-1} $ appearing in the row of index $ \lambda $ and the column of index $ \mu $ is denoted by $ \beta_\lambda^\mu $. Then (in the notation introduced above)
$$
\begin{cases}
\bar{e}_\mu = \sum_\lambda \alpha_\mu^\lambda e_\lambda \\
\bar{e}^\mu = \sum_\lambda \beta_\lambda^\mu e_\lambda
\end{cases}
$$
$$
\bar{e}_{f'}^{g'} = \sum_{(f', g)} \left( \prod_{i \in I} \alpha_{f'(i)}^{f(i)} \right) \left( \prod_{j \in J} \beta_{g(j)}^{g'(j)} \right) e_f^g
$$
for all mappings $ f': I \to L $ and $ g': J \to L $. The coordinates $ \zeta_g^f $ of a tensor $ z \in T_J^I(M) $ with respect to the basis $ (e_\lambda) $ can therefore be expressed in terms of the coordinates $ \bar{\zeta}_{g'}^{f'} $ of z with respect to the basis $ (\bar{e}_\lambda) $ using the formulae
$$
\zeta_g^f = \sum_{(f', g')} \left( \prod_{i \in I} \alpha_{g'(i)}^{g(i)} \right) \left( \prod_{j \in J} \beta_{f'(j)}^{f(j)} \right) \bar{\zeta}_{g'}^{f'}
$$
The matrix $ P^{-1} $ of passage from the basis $ (\bar{e}_\lambda) $ to the basis $ (e_\lambda) $ is the transpose of $ {}^tP^{-1} $, so that $ \beta_\lambda^\mu $ is the element which appears in the column of index $ \lambda $ and the row of index $ \mu $ of $ P^{-1} $. The calculation of $ e_f^g $ in terms of the $ \bar{e}_{f'}^{g'} $ and that of the $ \bar{\zeta}_{g'}^{f'} $ in terms of the $ \zeta_g^f $ are therefore made by replacing $ \alpha_\mu^\lambda $ by $ \beta_\lambda^\mu $ and $ \beta_\lambda^\mu $ by $ \alpha_\mu^\lambda $ in the above calculations and exchanging the roles of $ f $ and $ f' $ and those of $ g $ and $ g' $. Then
$$
e_f^g = \sum_{(f', g')} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f'(i)}^{f(i)} \right) \bar{e}_{f'}^{g'}
$$

(23)
$$
\bar{\zeta}_{g'}^{f'} = \sum_{(f,g)} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f(i)}^{f'(i)} \right) \zeta_g^f.
$$

The above formulae are such that the summation is over indices which appear once as a lower index and once as an upper index. Certain authors allow themselves because of this circumstance to suppress the summation signs.

### Exercises {#alg-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
