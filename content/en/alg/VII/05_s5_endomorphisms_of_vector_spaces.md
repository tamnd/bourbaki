---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 5
section_title: Endomorphisms of vector spaces
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.70-A VII.72
pdf_pages: 0387-0407, 0429-0431
extraction: ocr
subsections:
    - "no": 1
      title: The module associated to an endomorphism
      page: 28
      pdf_page: 387
    - "no": 2
      title: Eigenvalues and eigenvectors
      page: 30
      pdf_page: 389
    - "no": 3
      title: Similarity invariants of an endomorphism
      page: 31
      pdf_page: 390
    - "no": 4
      title: Triangularisable endomorphisms
      page: 34
      pdf_page: 393
    - "no": 5
      title: 'Properties of the characteristic polynomial : trace and determinant'
      page: 36
      pdf_page: 395
    - "no": 6
      title: Characteristic polynomial of the tensor product of two endomorphisms
      page: 39
      pdf_page: 398
    - "no": 7
      title: Diagonalisable endomorphisms
      page: 40
      pdf_page: 399
    - "no": 8
      title: Semi-simple and absolutely semi-simple endomorphisms
      page: 41
      pdf_page: 400
    - "no": 9
      title: '**Jordan decomposition'
      page: 43
      pdf_page: 402
statements: 63
exercises: 14
content_sha256: ba0e2d8669622429c1f2d930977c5c10b6081cff6153171d88654f4c54a82a7d
---

## § 5. ENDOMORPHISMS OF VECTOR SPACES

Notation. — Given a module $ M $, an element $ x $ of $ M $, and two endomorphisms $ u $ and $ v $ of $ M $, we will write $ u.x $, $ uv.x $ and $ uv $ in place of $ u(x) $, $ (u \circ v)(x) $ and $ u \circ v $ respectively ; we will denote the identity map from $ M $ to itself by 1 when no confusion can arise.

### 1. The module associated to an endomorphism

Let $ A $ be a commutative ring, let $ M $ be an $ A $-module, and let $ u $ be an $ A $-endomorphism of $ M $. Recall (III, p. 538) that the map $ (p(X), x) \mapsto p(u).x $ from $ A[X] \times M $ into $ M $ makes $ M $ an $ A[X] $-module, written $ M_u $. Recall also (III, pp. 538 and 539) that if $ M[X] $ denotes the $ A[X] $-module obtained from $ M $ by extension of scalars from $ \mathbf{A} $ to $ \mathbf{A}[X] $, and if $ \bar{u} $ denotes the $ \mathbf{A}[X] $-endomorphism of $ M[X] $ induced by $ u $, then there is an exact sequence of $ \mathbf{A}[XI]$-modules $ ^1 $

$$
(1) \quad 0 \to M[X] \xrightarrow{\psi} M[X] \xrightarrow{\varphi} M_u \to 0 ,
$$

where $ \varphi(p(X) \otimes x) = p(u).x $ and $ \psi = X - \bar{u} $.

An endomorphism $ u $ of an $ \mathbf{A}$-module $ M $ and an endomorphism $ u' $ of an $ \mathbf{A}$-module $ M' $ are said to be similar if there exists an isomorphism $ g $ from $ M $ onto $ M' $ such that $ u' \circ g = g \circ u $, that is (III, p. 540, Prop. 19) an isomorphism $ g $ from $ M_u $ onto $ M_{u'} $. If $ M $ (resp. $ M' $) is free on the finite basis $ B $ (resp. $ B' $), and if $ M(u) $ (resp. $ M(u') $) is the matrix of $ u $ (resp. $ u' $) with respect to $ B $ (resp. $ B' $), then $ u $ and $ u' $ are similar if and only if $ M(u) $ and $ M(u') $ are similar matrices (II, p. 356, Def. 6). The characteristic polynomials (III, p. 541, Def. 3) of two similar endomorphisms of finitely generated free modules are equal (III, p. 540, Prop. 19).

Let $ K $ be a commutative field ; then any pair $ (E, u) $ consisting of a vector space $ E $ over $ K $ and an endomorphism $ u $ of $ E $ corresponds to a $ K[X] $-module $ E_{,,} $. Since the ring $ K[X] $ is a principal ideal domain (IV, p. 11, Prop. 11), the results of the preceding sections can be applied to $ E_{,,} $.

Let us first show how to translate certain notions from the language of modules to that of endomorphisms of vector spaces :

« V is a submodule of $ E $, » means : « V is a vector subspace of $ E $ closed under $ u $ ».

« V is a cyclic submodule of $ E $, » means : « there exists $ x \in V $ such that the vector subspace $ V $ is spanned by the elements $ u^i . x \ (i \in \mathbf{N}) $ ». Then $ V $ is said to be cyclic (with respect to $ u $) and $ x $ is called a generator.

« V is an indecomposable submodule of $ E $, » means : « V is nonzero and is not the direct sum of two nonzero subspaces each closed under $ u $ ».

« a is the annihilator of the submodule $ V $ » means : « a is the ideal consisting of those polynomials $ p(X) \in K[X] $ such that $ p(u).x = 0 $ for all $ x \in V $ ».

The monic polynomial $ g $ such that $ a $ is equal to the principal ideal $ (g) $ is then called the minimal polynomial of the restriction of $ u $ to $ V $.

« $ E_{,,} $ is cyclic with annihilator $ a = (g) $ »

$$
\text{(with } g(X) = X^n + \alpha_{n-1} X^{n-1} + \cdots + \alpha_0 )
$$

$ ^1 $ The injectivity of $ \psi $, which is not stated in Prop. 18 of III, p. 539, is proved as follows : in the notation of loc. cit., we have

$$
\psi(\sum (X^k \otimes x_k)) = \sum X^k \otimes (x_{k-1} - u(x_k)) .
$$

If $ \sum X^k \otimes x_k $ belongs to the kernel of $ \psi $, then it follows that $ x_k , = u(x_k) $ for all $ k $, and the $ x_k $ are all zero, since the family $ (x_k) $ has finite support.

means : « there exists $ x \in E $ such that $ (u^i . x) $ ($ 0 \leq i \leq n - 1 $) is a basis of the vector space $ E $, and $ g(u).x = 0 $ ». In other words, we can find a basis of $ E $ such that the matrix $ U $ of $ u $ with respect to this basis is

$$
U = \begin{pmatrix}
0 & 0 & 0 \ldots 0 & -\alpha_0 \\
1 & 0 & 0 \ldots 0 & -\alpha_1 \\
0 & 1 & 0 \ldots 0 & -\alpha_2 \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & 0 \ldots 0 & -\alpha_{n-2} \\
0 & 0 & 0 \ldots 1 & -\alpha_{n-1}
\end{pmatrix}.
$$

« $ E $, is a torsion module » means, by the characterisation of cyclic torsion modules given above : « every cyclic submodule of $ E $, is finite dimensional over $ K $ ». In particular :

« $ E_u $ is a finitely generated torsion module » means : « $ E $ is finite dimensional over $ K $ ».

### 2. Eigenvalues and eigenvectors

#### Definition 1 {#alg-vii-s5-def-1 .statement}

*Let $ E $ be a vector space over a commutative field $ K $, and $ u $ an endomorphism of $ E $. An element $ x $ of $ E $ is said to be an eigenvector of $ u $ if there exists $ a \in K $ such that $ u . x = \alpha x $; if $ x \neq 0 $ then the scalar $ a $ is called the eigenvalue of $ u $ corresponding to the eigenvector $ x $. For every scalar $ a $, the vector subspace $ V_a $ consisting of $ x \in E $ such that $ u . x = \alpha x $ is called the eigenspace of $ E $ corresponding to $ a $.

The geometric multiplicity of the eigenvalue $ a $ is the cardinal $ \dim V_a $.

Suppose $ E $ is finite dimensional. The eigenvalues of $ u $ are those elements $ a $ of $ K $ such that the endomorphism $ a . 1 - u $ of $ E $ is not injective, in other words (III, p. 524, Prop. 3) such that $ \det(a . 1 - u) = 0 $. But, by the definition of the characteristic polynomial $ \chi_u $ of $ u $ (III, p.541, Def. 3), we have $ \det(a . 1 - u) = \chi_u(\alpha) $. Consequently :

#### Proposition 1 {#alg-vii-s5-prop-1 .statement}

*Suppose $ E $ is finite dimensional. Then an element $ a $ of $ K $ is an eigenvalue of the endomorphism $ u $ if and only if it is a root of the characteristic polynomial of $ u $.

If $ L $ is an extension of the field $ K $, then the roots of $ \chi_u $ in $ L $ are eigenvalues of the endomorphism $ 1, \otimes u $ of the $ L $-vector space $ L \otimes_K E $. They are often referred to as *eigenvalues of $ u $ in $ L $*. By abuse of language, we say that all the eigenvalues of $ u $ belong to $ L $ if this holds for all the eigenvalues of $ u $ in an algebraically closed extension of $ L $; this means that $ \chi_u $ decomposes into linear factors in $ L[X] $.

Let $ U $ be a square matrix of order $ n $ with coefficients in $ K $. Then by definition the characteristic polynomial of $ U $ is

$$
\chi_U(X) = \det(X . I, -U);
$$

the eigenvalues of $ U $ (in an extension $ L $ of $ K $) are the roots (in $ L $) of the polynomial $ \chi_U $; these are also the scalars $ a $ (in $ L $) such that there exists a nonzero solution to the system of linear equations $ UX = \alpha X $, where $ X $ is a column matrix of order $ n $; a column matrix $ X $ satisfying this equation is called an eigenvector of $ U $ corresponding to $ a $.

If $ U $ is the matrix of an endomorphism $ u $ of an n-dimensional vector space with respect to a basis $ B $, then $ \chi_U = \chi_u $, the eigenvalues of $ U $ are the eigenvalues of $ u $, and the eigenvectors of $ U $ are the matrices of the eigenvectors of $ u $ with respect to the basis $ B $.

#### Proposition 2 {#alg-vii-s5-prop-2 .statement}

*Let $ u $ be an endomorphism of a vector space $ E $ over a commutative field $ K $; for each scalar $ a $, let $ V_a $ be the eigenspace corresponding to $ a $. Then the subspaces $ V_a $ are closed under $ u $ and the sum of the $ V_a $ is direct.*

The first assertion is clear. By definition the subspace $ V_a $ is annihilated by the element $ X - a $ of $ K[X] $; the $ X - a, a \in K $, are irreducible and pairwise non-associate; the second assertion thus follows from VII, p. 8, Th. 1.

### 3. Similarity invariants of an endomorphism

If we translate the decomposition of a finitely generated torsion module in VII, p. 8, Th. 1 and p. 9, Prop. 2, then we obtain:

#### Proposition 3 {#alg-vii-s5-prop-3 .statement}

*Let $ E $ be a vector space of finite dimension $ n $ over a commutative field $ K $, and let $ u $ be an endomorphism of $ E $; for every monic irreducible polynomial $ p(X) $, let $ M_p $ be the vector subspace consisting of elements $ x $ of $ E $ such that $ (p(u))^k \cdot x = 0 $ for some integer $ k $. Then $ M_p $ is closed under $ u $, the vector space $ E $ is the direct sum of the $ M_p $, and there exist polynomials $ s_p $ such that, for all $ x \in E $, the component of $ x $ in $ M_p $ is equal to $ s_p(u) \cdot x $.*

#### Remark 1 {#alg-vii-s5-n3-rem-1 .statement}

— Clearly the minimal polynomial of the restriction of $ u $ to $ M_p $ is the greatest power of $ p $ which divides the minimal polynomial of $ u $. Moreover we have $ s_p(u) \cdot x = x $ for $ x \in M_p $, from which it follows immediately that, if $ M_p \neq 0 $, then $ s_p $ is coprime to $ p $.

Similarly, by Th. 2 of VII, p. 19, the module $ E_u $ is isomorphic to a direct sum of cyclic modules $ F_j = K[X]/a_j \ (1 \leq j \leq r) $, where the ideals $ a_j $ are distinct from $ K[X] $ and $ a_j \subset a_{j+1} $; and the $ a_j $ are determined by these conditions. Moreover, since $ E $, is a torsion module, we have $ a_1 \neq (0) $; since $ E $ has dimension $ n $, we have $ r \leq n $. Put $ a_j = (h_j) \ (1 \leq j \leq r) $, with $ h_j $ a monic polynomial, and consider the sequence $ (q_i) \ (1 \leq i \leq n) $ of polynomials defined by:

$$
\begin{cases}
q_i(X) = 1 & \text{if } i \leq n - r \\
q_i(X) = h_{n-i+1}(X) & \text{if } n - r < i \leq n .
\end{cases}
$$

It is clear that the polynomials $ q_i $ determine the polynomials $ h_j $ and conversely, and that $ E $, is isomorphic to the direct sum of the $ n $ modules $ K[X]/(q_i) $, the first $ n - r $ of which are $ 0 $.

In other words:

#### Proposition 4 {#alg-vii-s5-prop-4 .statement}

— Let E be a vector space of finite dimension n over a commutative field K, and let u be an endomorphism of E. Then there exist n monic polynomials $ q_i(X) \in K[X] $ ($ 1 \leq i \leq n $) such that $ q_i $ divides $ q_{i+1} $ for $ 1 \leq i \leq n-1 $, and E is the direct sum of n subspaces $ V_i $ ($ 1 \leq i \leq n $) closed under u, cyclic (with respect to u), and such that the minimal polynomial of the restriction of u to $ V_i $ is equal to $ q_i $ ($ 1 \leq i \leq n $). The polynomials $ q_i $ are uniquely determined by these conditions, and $ q_n $ is the minimal polynomial q of u.

#### Remark 2 {#alg-vii-s5-n3-rem-2 .statement}

— By the above proposition, there exists a basis of E with respect to which the matrix U of u has the form

$$
\begin{pmatrix}
A_{n-r+1} & 0 & \ldots & 0 & 0 \\
0 & A_{n-r+2} & \ldots & 0 & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \ldots & A_{n-1} & 0 \\
0 & 0 & \ldots & 0 & A_n
\end{pmatrix}
$$

where each matrix $ A_i $ has the form (2) (taking $ g(X) = q_i(X) $) (cf. VII, pp. 29-30).

#### Definition 2 {#alg-vii-s5-def-2 .statement}

— In the notation of Prop. 4, the n monic polynomials $ q_i(X) $ ($ 1 \leq i \leq n $) are called the similarity invariants of the endomorphism u.

Thus the n-th similarity invariant $ q_n $ is the minimal polynomial of u (Prop. 4); in other words, for a polynomial $ p(X) \in K[X] $ to satisfy $ p(u) = 0 $, it is necessary and sufficient that $ p $ be a multiple of $ q_n $.

#### Corollary 1 {#alg-vii-s5-def-2-cor-1 .statement}

— Let K be a field, let E and $ E' $ be two finite dimensional vector spaces over K, and let u (resp. $ u' $) be an endomorphism of E (resp. $ E' $). Then u and $ u' $ are similar (VII, p. 29) if and only if they have the same similarity invariants.

Indeed $ u $ and $ u' $ are similar if and only if the $ K[X] $-modules E, and $ E'_u $ are isomorphic.

#### Corollary 2 {#alg-vii-s5-def-2-cor-2 .statement}

— Let u be an endomorphism of a finite dimensional vector space E over a field K, let $ (q_1, \ldots, q_n) $ be the family of similarity invariants of u, let L be an extension of K, let $ E_{(L)} = L \otimes_K E $ be the L-vector space induced from E by extension of scalars and let $ u_{(L)} = 1_L \otimes u $ be the endomorphism of $ E_{(L)} $ induced by u. Then the similarity invariants of $ u_{(L)} $ are the images $ \bar{q}_1, \ldots, \bar{q}_n $ of $ q_1, \ldots, q_n $ in $ L[X] $.

This follows immediately from Prop. 4 and the fact that the $ L[X] $-modules $ E_{(L)u_{(L)}} $ and $ (K[X]/(q_i))_{(L)} $ are isomorphic to $ L[X] \otimes_{K[X]} E_u $ and $ L[X]/(\bar{q}_i) $ respectively.

Let U be a square matrix of order n with coefficients in a commutative field K. Then the similarity invariants of the endomorphism of $ K^n $ defined by U are called the similarity invariants of $ U $. It then follows from Cor. 1 above that two square matrices are similar if and only if they have the same similarity invariants, and that if $ u $ is an endomorphism of a finite dimensional vector space $ E $ over $ K $, and $ U $ is the matrix of $ u $ with respect to some basis $ B $ of $ E $, then the similarity invariants of $ U $ and $ u $ coincide. By Cor. 1 and 2 above, we have:

#### Corollary 3 {#alg-vii-s5-def-2-cor-3 .statement}

— Let $ U $ and $ V $ be two square matrices of order $ n $ with coefficients in a commutative field $ K $. If there exists an invertible square matrix $ P $ over some extension $ K' $ of $ K $ such that $ V = P^{-1}UP $, then there exists an invertible square matrix $ Q $ over $ K $ such that $ V = Q^{-1}UQ $.

Let $ E $ be a finite dimensional vector space over a commutative field $ K $, let $ (e_i)_{1 \leq i \leq n} $ be a basis of $ E $ and let $ u $ be an endomorphism of $ E $. Then by the exact sequence (1) of VII, p. 29, the $ K[X] $-module $ E $, associated to $ u $ is isomorphic to the quotient of the free $ K[X] $-module $ E[X] $, with basis $ (1 \otimes e_i) $, by the image of $ E[X] $ under the $ K[X] $-linear map $ X - \bar{u} $. The similarity invariants $ q_i(X) $ of $ u $ (VII, p. 32, Def. 2) are thus the invariant factors of $ X - \bar{u} $ (VII, p. 22). Thus Prop. 6 of VII, p. 22, implies:

#### Proposition 5 {#alg-vii-s5-prop-5 .statement}

— Let $ E $ be a vector space of finite dimension $ n $ over a commutative field $ K $, let $ u $ be an endomorphism of $ E $, and let $ U $ be its matrix with respect to some basis of $ E $. Then for each integer $ m $ with $ 1 \leq m \leq n $, the product
$$
d_m(X) = q_1(X) q_2(X) \ldots q_m(X)
$$
of the first $ m $ similarity invariants of $ u $ is equal to the gcd of the $ m $-th order minors of the matrix $ XI, - U $.

#### Corollary 1 {#alg-vii-s5-prop-5-cor-1 .statement}

— Let $ u $ be an endomorphism of a vector space of finite dimension $ n $ over a commutative field $ K $, with characteristic polynomial $ \chi_u(X) $ and similarity invariants $ q_i(X) $ ($ 1 \leq i \leq n $). Then
$$
\chi_u(X) = q_1(X) q_2(X) \ldots q_n(X)
$$

#### Corollary 2 {#alg-vii-s5-prop-5-cor-2 .statement}

— In the notation of Cor. 1, let $ q(X) $ be the minimal polynomial of $ u $; then $ q(X) $ divides $ \chi_u(X) $ and $ \chi_u(X) $ divides $ q(X)^n $. In particular the minimal polynomial and the characteristic polynomial of $ u $ have the same roots, and these are the eigenvalues of $ u $.

Since $ q(X) = q_n(X) $, it is clear that $ q(X) $ divides $ \chi_u(X) $. On the other hand, since each $ q_i $ divides $ q $, their product $ \chi_u $ divides $ q^n $.

#### Corollary 3 {#alg-vii-s5-prop-5-cor-3 .statement}

— An endomorphism $ u $ is nilpotent if and only if its characteristic polynomial has the form $ X^n $.

This follows immediately from Cor. 2.

Let us now rewrite Prop. 9 of VII, p. 24, which gives the decomposition of a module as a direct sum of indecomposable submodules.

#### Proposition 6 {#alg-vii-s5-prop-6 .statement}

— Let $ E $ be a vector space of finite dimension $ n $ over a commutative field $ K $, and let $ u $ be an endomorphism of $ E $. Then $ E $ is the direct sum of subspaces $ E_k $, closed under $ u $ and cyclic with respect to $ u $, such that the minimal polynomial of the restriction of $ u $ to $ E_k $ has the form $ p_k^{n(k)} $, where $ p_k $ is an irreducible polynomial, and $ E_k $ cannot be expressed as a direct sum of two nonzero subspaces each closed under $ u $. For every monic irreducible polynomial $ p \in K[X] $ and every integer $ n \geq 1 $, the number $ m(p^n) $ of subspaces $ E_k $ in any such decomposition, such that $ p^n $ is the minimal polynomial of the restriction of $ u $ to $ E_k $, is uniquely determined.

The $ p_k^{n(k)} $ determine the similarity invariants of $ u $ and vice versa; we can get from one to the other by the procedure explained in VII, p. 25, Remarks 2 and 3. Furthermore, we can immediately get from the decomposition considered in Prop. 6 to those considered in Prop. 3 and 4.

Note that the monic irreducible polynomials $ p \in K[X] $ such that $ m(p^n) > 0 $ for some integer $ n \geq 1 $ are precisely the monic irreducible factors of the minimal polynomial of $ u $. Thus, in contrast to the similarity invariants, these polynomials depend in general on the field $ K $ in which we are working.

### 4. Triangularisable endomorphisms

In this section we will be interested in the case where the minimal polynomial $ p(X) $ of $ u $ splits into a product of linear factors in $ K[X] $, in other words (VII, p. 33, Cor. 2) in the case where all the eigenvalues of $ u $ belong to $ K $. This will hold in particular when $ K $ is algebraically closed. Prop. 3 of VII, p. 31 gives immediately:

#### Proposition 7 {#alg-vii-s5-prop-7 .statement}

— Let $ E $ be a finite dimensional vector space over a commutative field $ K $, and let $ u $ be an endomorphism of $ E $ whose eigenvalues all belong to $ K $. For each eigenvalue $ a $ of $ u $, let $ M_a $ be the vector subspace of $ E $ consisting of those elements $ x $ for which there exists an integer $ k \geq 1 $ such that $ (u - a)^k \cdot x = 0 $. Then $ M_a $ is closed under $ u $, the vector space $ E $ is the sum of the $ M_a $, and there exist polynomials $ s_a \in K[X] $ such that, for all $ x \in E $, the component of $ x $ in $ M_a $ is equal to $ s_a(u) \cdot x $.

The submodule $ M_a $, being finitely generated as a $ K[X] $-module, then has an annihilator of the form $ (X - a)' $; in other words, there exists an integer $ r \geq 1 $ such that
$$
(u - a)^r \cdot x = 0
$$
for all $ x \in M_a $; the restriction of $ u - a $ to $ M_a $ is a nilpotent endomorphism.

Still assuming that the eigenvalues of $ u $ belong to $ K $, we now apply Prop. 6 of VII, p. 34 to $ u $. The polynomials $ p_k $ are nothing other than the $ X - a $ (as $ a $ runs through the set of eigenvalues of $ u $), and we see that $ E $ is the direct sum of subspaces $ E_i $ closed under $ u $, cyclic (with respect to $ u $), and such that the minimal polynomial of the restriction of $ u $ to $ E_i $ has the form $ (X - a)^m $. Let $ E_i' $ be the $ K[X] $-module associated to $ E_i $; then $ E_i' $ is isomorphic to one of the modules $ K[X]/((X - a)^m) $. Now the residue classes mod $ (X - a)^m $ of the elements $ (X - \alpha)^k $ ($ 0 \leq k \leq m - 1 $) form a $ K $-basis of $ K[X]/((X - a)^m) $ (IV, p. 11, Cor.), and

$$
X(X - \alpha)^k = \alpha (X - \alpha)^k + (X - \alpha)^{k+1}
$$

for $ 0 \leq k \leq m - 1 $; it follows that $ E_i $ has dimension $ m $, and if $ a $ is the unique eigenvalue of the restriction $ u_i $ of $ u $ to $ E_i $, then there exists a basis of $ E_i $ with respect to which the matrix of $ u_i $ is the $ m \times m $ matrix

$$
U_{m,\alpha} = \begin{pmatrix}
\alpha & 0 & 0 & \ldots & 0 & 0 \\
1 & \alpha & 0 & \ldots & 0 & 0 \\
0 & 1 & \alpha & \ldots & 0 & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & 0 & \ldots & \alpha & 0 \\
0 & 0 & 0 & \ldots & 1 & \alpha
\end{pmatrix}
$$

#### Definition 3 {#alg-vii-s5-def-3 .statement}

*For every field $ K $, every integer $ m \geq 1 $, and every $ a \in K $, the matrix $ U_{m,\alpha} $ is called the Jordan matrix of order $ m $ and eigenvalue $ a $.*

#### Proposition 8 {#alg-vii-s5-prop-8 .statement}

*Let $ E $ be a finite dimensional vector space over a commutative field $ K $, and let $ u $ be an endomorphism of $ E $. Then the following conditions are equivalent*:

(i) *the eigenvalues of $ u $ (in some algebraically closed extension of $ K $) belong to $ K $*;

(ii) *there exists a basis of $ E $ with respect to which the matrix of $ u $ is lower (resp. upper) triangular*;

(iii) *there exists a basis of $ E $ with respect to which the matrix of $ u $ is a diagonal block of Jordan matrices*.

We have (i) $ \Rightarrow $ (iii) by Prop. 7 and the above remarks, and the assertions (iii) $ \Rightarrow $ (ii) and (ii) $ \Rightarrow $ (i) are trivial.

#### Definition 4 {#alg-vii-s5-def-4 .statement}

*An endomorphism satisfying conditions (i), (ii) and (iii) of Prop. 8 is called triangularisable*.

In particular if $ K $ is algebraically closed, then every endomorphism of a $ K $-vector space is triangularisable.

For matrices, Prop. 8 implies :

#### Corollary {#alg-vii-s5-n4-cor-1 .statement}

*Let $ U $ be a square matrix over a commutative field $ K $ such that all the eigenvalues of $ U $ are in $ K $; then there exists a matrix similar to $ U $ which is a diagonal block of Jordan matrices*.

#### Remark {#alg-vii-s5-n4-rem-1 .statement}

— 1) It follows from Prop. 6 of VII, p. 34, that, if $ U $ is similar to a diagonal block of Jordan matrices $ (J_k) $, then the number of $ J_k $ of the form $ U_{m,\alpha} $ (for given $ m $ and $ \alpha $) is uniquely determined by $ U $.

2) More generally, if $ U $ is similar to a diagonal block of Jordan matrices $ U_{m_i, \alpha_i} $, then the similarity invariants of $ U $ can be readily calculated by a method modelled on that presented in VII, p. 25, Remark 3 : write all the $ (X - \alpha_i)^{m_i} $ with the same $ \alpha $ on the same line, in decreasing order of exponents, and complete with 1’s to have lines whose lengths are equal to the order of $ U $; this done, the similarity invariants of $ U $ are obtained, in decreasing order of indices, by forming the products of terms in the same column. For example, for the matrix

$$
\begin{pmatrix}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 1 & 3
\end{pmatrix}
$$

we write

$$
(X - 2), 1, 1 \\
(X - 3)^2, 1, 1
$$

and the similarity invariants are 1, 1 and $ (X - 2)\ (X - 3)' $

By noticing that the minimal polynomial of the Jordan matrix $ U_{m, \alpha} $ is $ (X - a)'' $, and that it is equal to its characteristic polynomial, we obtain the following result :

#### Proposition 9 {#alg-vii-s5-prop-9 .statement}

— *If the square matrix $ U $ is similar to a diagonal block of Jordan matrices $ (U_{m_i, \alpha_i}) $, then the minimal polynomial of $ U $ is the lcm of the $ (X - \alpha_i)^{m_i} $, and the characteristic polynomial is the product of the $ (X - a_i)''' $.*

#### Corollary {#alg-vii-s5-n4-cor-2 .statement}

— *In the notation of Prop. 7, the dimension of the subspace $ M_\alpha $ is the multiplicity of the eigenvalue $ \alpha $ as a root of the characteristic polynomial of $ u $.*

### 5. Properties of the characteristic polynomial : trace and determinant

Let E be a vector space of finite dimension $ n $ over a commutative field K, and let $ u $ be an endomorphism of E. By III, p. 541, the characteristic polynomial of $ u $ has the form :

(5)
$$
\chi_u(X) = X^n - \mathrm{Tr}(u)\ X^{n-1} + \cdots + (-1)^n \det(u)\ .
$$

#### Proposition 10 {#alg-vii-s5-prop-10 .statement}

— *Let $ E $ be a vector space of finite dimension $ n $ over a commutative field $ K $, let $ u $ be an endomorphism of $ E $, and let $ \chi_u(X) = \prod_{i=1}^n (X - \alpha_i) $ be a decomposition into linear factors of its characteristic polynomial (in a suitable extension of $ K $, cf. V, p. 21). If $ q $ is a polynomial with coefficients in $ K $, then the characteristic polynomial of $ q(u) $ is given by*

(6)
$$
\chi_{q(u)}(X) = \prod_{i=1}^n (X - q(\alpha_i))\ ,
$$

and its trace and determinant are given by

(7) $$
\operatorname{Tr}(q(u)) = \sum_{i=1}^n q(\alpha_i),
$$
(8) $$
\det(q(u)) = \prod_{i=1}^n q(\alpha_i).
$$

It is clear that (7) and (8) follow from (6) by virtue of (5). To prove the formula (6), we may assume that K is algebraically closed. We then take a basis for E with respect to which the matrix $ U $ of $ u $ is lower triangular ($ VII $, p. 35, Cor. to Prop. 8); we will make use of the following easy lemma:

#### Lemma 1 {#alg-vii-s5-lem-1 .statement}

*If B and C are lower triangular matrices of order n with diagonals $ (\beta_i) $ and $ (\gamma_i) $, then the matrices $ B + C $ and $ BC $ are lower triangular with diagonals $ (\beta_i + \gamma_i) $ and $ (\beta_i \gamma_i) $.*

Since the matrix $ U $ of $ u $ is lower triangular with diagonal $ (\alpha_i) $ say, it follows from Lemma 1 that $ q(U) $ is a lower triangular matrix with diagonal $ (q(\alpha_i)) $. Then $ X . I, -q(U) $ is a lower triangular matrix with diagonal $ (X - q(a;)) $, which proves (6).

#### Corollary 1 {#alg-vii-s5-lem-1-cor-1 .statement}

*For $ q(u) $ to be invertible, it is necessary and sufficient that $ q $ be coprime to $ \chi_u $.*

Indeed, to say that $ q $ and $ \chi_u $ are coprime is equivalent to saying that they have no common root in an algebraically closed extension of K, in other words (8) that $ \det(q(u)) \neq 0 $.

#### Remark 1 {#alg-vii-s5-n5-rem-1 .statement}

— A polynomial is coprime to $ \chi_u $ if and only if it is coprime to the minimal polynomial of $ u $ (VII, p. 33, Cor. 2).

#### Corollary 2 {#alg-vii-s5-lem-1-cor-2 .statement}

*Let $ r \in K(X) $ be a rational function over K. Then $ u $ is substitutable (IV, p. 21) in $ r $ if and only if each of its eigenvalues is. In this case the following formulae hold:*

$$
\chi_{r(u)}(X) = \prod_{i=1}^n (X - r(\alpha_i)), \quad \operatorname{Tr}(r(u)) = \sum_{i=1}^n r(\alpha_i), \quad \det(r(u)) = \prod_{i=1}^n r(\alpha_i).
$$

Write $ r = p/q $ where $ p $ and $ q $ are coprime polynomials. Then $ u $ is substitutable in $ r $ if and only if $ \det(q(u)) \neq 0 $, so the first assertion follows from (8). By Cor. 1, we may suppose $ q $ coprime to $ \chi_u $, so by the Bezout identity there exist polynomials $ g $ and $ h $ such that $ qg + h\chi_u = 1 $. Then $ q(\alpha_i)g(\alpha_i) = 1 $ and $ q(u)g(u) = 1 $ by the Cayley-Hamilton theorem (III, p. 541). The stated formulae can then be obtained by applying formulae (6), (7) and (8) to $ p(u)\ g(u) = r(u) $.

#### Corollary 3 {#alg-vii-s5-lem-1-cor-3 .statement}

*For each integer $ s \geq 0 $ we have $ \operatorname{Tr}(u^s) = \sum_{i=1}^n \alpha_i^s $. This formula is also valid for $ s < 0 $ provided $ u $ is invertible.*

This is a special case of the previous corollary.

#### Corollary 4 {#alg-vii-s5-lem-1-cor-4 .statement}

— *Suppose the field K is of characteristic zero; then the endomorphism u is nilpotent if and only if* $ \operatorname{Tr}(u^s) = 0 $ *for* $ 1 \leq s \leq n $.

If $ u $ is nilpotent then the $ a_i $ are all zero, and $ \operatorname{Tr}(u^s) = 0 $ for all $ s > 0 $ (Cor. 3). Conversely, if $ \operatorname{Tr}(u^s) = 0 $ for $ 1 \leq s \leq n $, then the $ a_i $ are all zero since $ K $ is of characteristic zero (IV, p. 72, Cor.), and $ u $ is nilpotent (VII, p. 33).

#### Corollary 5 {#alg-vii-s5-lem-1-cor-5 .statement}

— *Let Y be an indeterminate and let $ \tilde{u} $ denote the endomorphism of the $ K(Y) $-vector space $ K(Y) \otimes_K E $ induced from $ u $ by extension of scalars from $ K $ to the field $ K(Y) $ of rational functions in $ Y $ with coefficients from $ K $. Then the endomorphism $ Y \cdot 1 - \tilde{u} $ is invertible. Moreover, if $ \chi_u' $ denotes the derivative of the polynomial $ \chi_u $, then*

$$
\operatorname{Tr}((Y \cdot 1 - \tilde{u})^{-1}) = \chi_u'(Y)/\chi_u(Y) .
$$

The endomorphism $ Y \cdot 1 - \tilde{u} $ is invertible because its determinant is the nonzero element $ \chi_u(Y) $ of $ K(Y) $. It follows that $ \tilde{u} $ is substitutable in the rational function $ r(X) = (Y - X)^{-1} $ in $ K(Y)(X) $. The second assertion now follows from Cor. 2, by the relation

$$
\chi_u'(Y)/\chi_u(Y) = \sum_i (Y - \alpha_i)^{-1} = \sum_i r(\alpha_i) .
$$

#### Corollary 6 {#alg-vii-s5-lem-1-cor-6 .statement}

— *Suppose the field K is of characteristic zero. Then, in the ring $ K[[T]] $ of formal power series, we have*

$$
- T \frac{d}{dT} \log \det(1 - Tu) = \sum_{m \geq 1} \operatorname{Tr}(u^m) T^m
$$

Let us first of all work in the field $ K(T) $ of rational functions, and put $ P(T) = \det(I, -T \cdot U) $, where $ U $ is the matrix of $ u $ with respect to some basis of $ E $. Then

$$
P(T) = \det(T(T^{-1} \cdot I, -U)) = T^n \chi_U(T^{-1}) ,
$$

so $ P'(T)/P(T) = n/T - \chi_u'(T^{-1})/T^2 \chi_u(T^{-1}) $. Moreover, by Cor. 5 we have

$$
\chi_u'(T^{-1})/T \chi_U(T^{-1}) = \operatorname{Tr}((T^{-1} \cdot I_n - U)^{-1})/T = \operatorname{Tr}((I_n - T \cdot U)^{-1}) .
$$

It follows that $ -TP'(T)/P(T) = -n + \operatorname{Tr}((I_n - TU)') $. The corollary is now obtained by expanding each side of this equation as a formal power series.

#### Remark 2 {#alg-vii-s5-n5-rem-2 .statement}

— By IV, p. 80, Cor. 1 and formula (8), we have, for each polynomial $ q \in K[X] $, that

$$
\det q(u) = \operatorname{res}(\chi_u, q) ,
$$

where $ \operatorname{res}(\chi_u, q) $ is the resultant of the polynomials $ \chi_u $ and $ q $. *In* particular if we take $ q = \chi_u' $ we obtain

$$
\det \chi_u'(u) = (-1)^{n(n-1)/2} \operatorname{dis}(\chi_u),
$$

where $ \operatorname{dis}(\chi_u) $ is the discriminant of the polynomial $ \chi_u $ (*IV*, p. 82, formula (47)). Furthermore:

#### Corollary 7 {#alg-vii-s5-lem-1-cor-7 .statement}

We have $ \det(\operatorname{Tr}(u^{i+j})_{0 \leq i,j \leq n}) = \operatorname{dis}(\chi_u) $.

Let D be the Vandermonde matrix $ (\alpha_i^j)_{1 \leq i,j \leq n} $. Then (**III**, p. 532, formula (29)):

$$
\det(D)^2 = \prod_{i < j} (a_j - \alpha_i)^2 = \operatorname{dis}(\chi_u).
$$

Moreover, the $(i, j)$-th entry of $ D \cdot 'D $ is $ \sum_k \alpha_k^{i+j-2} = \operatorname{Tr}(u^{i+j-2}) $, and the corollary follows.

### 6. Characteristic polynomial of the tensor product of two endomorphisms

#### Proposition 11 {#alg-vii-s5-prop-11 .statement}

*Let E* (resp. $ E' $) *be a finite dimensional vector space over a commutative field K and let u* (resp. $ u' $) *be an endomorphism of E* (resp. $ E' $). Let*

$$
\chi_u(X) = \prod_i (X - \alpha_i), \quad \chi_{u'}(X) = \prod_j (X - \beta_j)
$$

*be decompositions into linear factors of the characteristic polynomials of u and $ u' $* in some suitable extension of $ K $. *Then the characteristic polynomial of the endomorphism $ u \otimes u' $ of the vector space $ E \otimes_K E' $ is given by the formula*

$$
\chi_u \otimes u'(X) = \prod_{i,j} (X - \alpha_i \beta_j).
$$

Arguing as in the proof of Prop. 10 of *VII*, p. 36, we see that it is sufficient to prove the following lemma:

#### Lemma 2 {#alg-vii-s5-lem-2 .statement}

*Let B and C be two lower triangular matrices of orders m and n respectively, with diagonals $ (\beta_i)_{1 \leq i \leq n} $ and $ (\gamma_j)_{1 \leq j \leq n} $. Let us identify the lexicographic product of the ordered sets $ \{1, 2, \ldots, m\} $ and $ \{1, 2, \ldots, n\} $ with the interval $ \{1, 2, \ldots, mn\} $. Then the tensor product matrix* (**II**, p. 357) *B $ \otimes $ C is lower triangular with diagonal* $ (\beta_i \gamma_j) $.

This follows immediately from the definition of the tensor product of two matrices (*loc. cit.*) and of the lexicographic product (*Set Theory*, III, p. 157).

### 7. Diagonalisable endomorphisms

#### Definition 5 {#alg-vii-s5-def-5 .statement}

— Let E be a finite dimensional vector space over a commutative field K and let $ \mathfrak{F} $ be a set of endomorphisms of E. Then $ \mathfrak{F} $ is said to be diagonal with respect to a basis $ (e_i) $ of E if the matrix of each $ u \in \mathfrak{F} $ with respect to $ (e_i) $ is diagonal. The set $ \mathfrak{F} $ is said to be diagonalisable if there exists a basis of E with respect to which $ \mathfrak{F} $ is diagonal.

This definition applies in particular to the case when $ \mathfrak{F} $ contains only one element $ u $; we then say that $ u $ is diagonal (diagonalisable). Note also that $ \mathfrak{F} $ is diagonal with respect to a basis $ (e_i) $ if and only if the $ (e_i) $ are common eigenvectors of all the elements of $ \mathfrak{F} $; it follows that $ \mathfrak{F} $ is diagonalisable if and only if E is generated by eigenvectors common to all the elements of $ \mathfrak{F} $.

Let A be a subalgebra of $ \mathrm{End}_K(E) $ containing Id. Then A is diagonalisable if and only if it is isomorphic to an algebra $ K^r $ (in other words is diagonalisable in the sense of V, p. 28, Def. 1); indeed, if A is isomorphic to $ K^r $, then A is diagonalisable by V, p. 29, Prop. 1; conversely, if A is diagonalisable, then it is isomorphic to a subalgebra of the algebra of diagonal matrices, which is isomorphic as an algebra to $ K^n $, $ n = \dim(E) $, hence A is isomorphic to some algebra $ K^r $ (V, p. 30, Prop. 3).

#### Proposition 12 {#alg-vii-s5-prop-12 .statement}

— Let E be a finite dimensional vector space over a commutative field K, and let u be an endomorphism of E. Then the following conditions are equivalent:

(i) u is diagonalisable.
(ii) E is the direct sum of the eigenspaces of u.
(iii) All the roots of the minimal polynomial of u are in K, and these roots are all simple.

Moreover, if these conditions are satisfied, then every subspace of E closed under u is the direct sum of its intersections with the eigenspaces of u.

The equivalence of (i) and (ii) follows from the preceding remarks and VII, p. 31, Prop. 2. Suppose u is diagonalisable, and let $ (\alpha_i) $ be its family of eigenvalues, and $ (V_i) $ the corresponding family of eigenspaces; since the restriction of u to $ V_i $ is the homothety defined by $ \alpha_i $, it annihilates the polynomial $ X - \alpha_i $; it follows that u annihilates the polynomial $ \prod (X - \alpha_i) $, which is therefore a multiple of the minimal polynomial of u, and hence coincides with it, which proves (iii). Conversely, if (iii) is satisfied then there exists a basis of E with respect to which the matrix U of u is a diagonal block of Jordan matrices $ U_{m,\alpha} $ (VII, p. 35, Prop. 8); then by Prop. 9 the integers m are all equal to 1 and so U is diagonal. Finally, the last assertion follows from the fact that if u is diagonalisable then its eigenspaces are the primary components of $ E_u $, and from VII, p. 9, Cor. 1.

#### Corollary {#alg-vii-s5-n7-cor-1 .statement}

— If all the roots of the characteristic polynomial of u are in K, and they are all simple, then u is diagonalisable.

Indeed the minimal polynomial divides the characteristic polynomial.

#### Proposition 13 {#alg-vii-s5-prop-13 .statement}

— Let E be a finite dimensional vector space over a commutative field K, let $ \mathcal{S} $ be a set of endomorphisms of E, and let A be the subalgebra of $ \mathrm{End}_K(E) $ generated by $ \mathcal{S} $ and $ \mathrm{Id}_E $. Then the following conditions are equivalent:
(i) $ \mathcal{S} $ is diagonalisable.
(ii) The K-algebra A is diagonalisable.
(iii) The elements of $ \mathcal{S} $ are diagonalisable and commute with one another.

If $ (e,) $ is a basis of E with respect to which $ \mathcal{S} $ is diagonal, then A is contained in the algebra of endomorphisms which are diagonal with respect to this basis, so is also diagonalisable; if A is diagonalisable, then the same argument shows that $ \mathcal{S} $ is diagonalisable. This shows the equivalence of (i) and (ii). Since any two diagonal matrices commute, we have (i) $ \rightarrow $ (iii), and it remains to prove the converse. Suppose then that the elements of $ \mathcal{S} $ are diagonalisable and commute with each other. We will make use of the following lemma:

#### Lemma 3 {#alg-vii-s5-lem-3 .statement}

— Let g and h be two commuting endomorphisms of a vector space E. Then each eigenspace of g is closed under h.

Indeed, if $ W_\lambda $ is the eigenspace of g corresponding to the eigenvalue $ \lambda $, then for all $ x \in W $, we have
$$
gh \cdot x = hg \cdot x = h \cdot \lambda x = \lambda h \cdot x ,
$$
which says that $ h \cdot x \in W_\lambda $.

Let us now return to the proof of Prop. 13. Among all decompositions of E as a direct sum of nonzero subspaces each closed under all the elements of $ \mathcal{S} $, choose one with the greatest number of components (the dimension of E is an upper bound for this number), say $ E = \sum_{i \in I} E_i $. Let $ u \in \mathcal{S} $ and let $ E = \sum V_\alpha $ be the decomposition of E as the direct sum of the eigenspaces of $ u $. By Lemma 3, each $ V_\alpha $ is closed under $ \mathcal{S} $, and hence so is each $ V_i \cap E_i $; by Prop. 12 each $ E_i $ is the direct sum of the $ V_i \cap E_i $. The choice of the $ E_i $ thus forces each $ E_i $ to be contained in one of the $ V_\alpha $; thus the restriction of $ u $ to each $ E_i $ is a homothety. Since this is true for all the elements of $ \mathcal{S} $, it follows that $ \mathcal{S} $ is diagonalisable.

#### Corollary {#alg-vii-s5-n7-cor-2 .statement}

— The sum and the composite of two commuting diagonalisable endomorphisms of E are diagonalisable.

### 8. Semi-simple and absolutely semi-simple endomorphisms

#### Definition 6 {#alg-vii-s5-def-6 .statement}

— Let E be a finite dimensional vector space over a commutative field K. Then an endomorphism u of E is said to be semi-simple if every subspace of E which is closed under u has a complement which is closed under u.

This means that every submodule of the $ K[X] $-module E, is a direct factor, in other words the $ K[X] $-module $ E_u $ is semi-simple (VII, p. 9).

#### Proposition 14 {#alg-vii-s5-prop-14 .statement}

— *An endomorphism u of a finite dimensional vector space over a commutative field is semi-simple if and only if the minimal polynomial of u has no multiple factors.*

This follows immediately from VII, p. 9, Cor. 4 and p. 31, Remark 1.

Let E be a vector space over a commutative field K, let L be an extension of K, and $ u $ an endomorphism of E ; let $ u_{(L)} $ denote the L-endomorphism $ l_L \otimes u $ of the L-vector space $ E_{(l.)} = L \otimes_K E $ induced from E by extension of scalars. In the same way, if $ \mathfrak{F} $ is a set of endomorphisms of E, let $ \mathfrak{F}_{(L)} $ denote the set of $ u_{(L)} $ for $ u $ in '8.

#### Corollary {#alg-vii-s5-n8-cor-1 .statement}

— *Let u be an endomorphism of a finite dimensional vector space over a commutative field K, and let L be an extension of K. If $ u_{(L)} $ is semi-simple then u is semi-simple. If u is semi-simple and L is separable over K, then $ u_{(L)} $ is semi-simple.*

This follows immediately from Prop. 14 and from V, p. 120, Cor. 1 (note that the minimal polynomials of $ u $ and $ u_{(L)} $ coincide).

#### Proposition 15 {#alg-vii-s5-prop-15 .statement}

— *Let E be a finite dimensional vector space over a commutative field K, let u be an endomorphism of E and let q(X) be its minimal polynomial. Then the following conditions are equivalent :*

(i) *For every extension L of K, the endomorphism $ u_{(L)} $ is semi-simple.*
(ii) *There exists an extension L of K such that the endomorphism $ u_{(L)} $ is diagonalisable.*
(iii) *The polynomial q(X) is separable over K.*

Indeed, condition (i) means that the polynomial $ 1 \otimes q(X) $ in $ L[X] $ has no multiple factors, for any extension L of K (Prop. 14), condition (ii) means that there exists an extension L of K such that all the roots of $ q(X) $ belong to L and that these roots are all simple (VII, p. 40, Prop. 12), and these conditions are each equivalent to (iii) by definition (V, p. 38).

#### Definition 7 {#alg-vii-s5-def-7 .statement}

— *An endomorphism u satisfying conditions (i), (ii) and (iii) of Prop. 15 is said to be absolutely semi-simple.*

#### Corollary {#alg-vii-s5-n8-cor-2 .statement}

— *A necessary and sufficient condition for u to be absolutely semi-simple is that there exist an extension L of K such that L is perfect and $ u_{(L)} $ is semi-simple.*

The condition in the corollary means that there exists an extension L of K such that L is perfect and $ q(X) $ has no multiple factors in $ L[X] $ (Prop. 14) ; this condition is equivalent to (iii) by V, p. 38, Cor. 2.

#### Proposition 16 {#alg-vii-s5-prop-16 .statement}

— *Let E be a finite dimensional vector space over a commutative field K, let $ \mathfrak{F} $ be a set of endomorphisms of E and let A be the subalgebra of $ \mathrm{End}_K(E) $ generated by $ \mathfrak{F} $ and Id. Then the following conditions are equivalent :*

(i) *There exists an extension L of K such that $ \mathfrak{F}_{(l.)} $ is diagonalisable.*

(ii) *The K-algebra* $ A $ *is étale* (V, p. 28, Def. 1).

(iii) *The elements of* $ \mathfrak{F} $ *are absolutely semi-simple and commute with one another*.

Note first that, for every extension $ L $ of $ K $, the $ L $-algebra generated by $ \mathfrak{F}_{(L)} $ and $ \mathrm{Id}_{E_{(L)}} $ coincides with $ L \otimes_K A $; hence by Prop. 13 $ \mathfrak{F}_{(L)} $ is diagonalisable if and only if the $ L $-algebra $ L \otimes_K A $ is diagonalisable. The equivalence of conditions (i) and (ii) thus follows from V, p. 28, Def. 1. On the other hand, it is immediate that (i) $ \Rightarrow $ (iii). Finally suppose (iii) holds, and let $ L $ be an algebraic closure of $ K $; then the elements of $ \mathfrak{F}_{(L)} $ are diagonalisable (VII, p. 40, Prop. 12) and commute with one another; hence $ \mathfrak{F}_{(L)} $ is diagonalisable by VII, p. 41, Prop. 13.

#### Corollary {#alg-vii-s5-n8-cor-3 .statement}

*The sum and product of two commuting, absolutely semi-simple endomorphisms are absolutely semi-simple*.

#### Remark {#alg-vii-s5-n8-rem-1 .statement}

— Suppose the conditions of Prop. 16 are satisfied and let $ L $ be an extension of $ K $. By Prop. 13 the set $ \mathfrak{F}_{(L)} $ is diagonalisable if and only if the algebra $ L \otimes_K A $ is diagonalisable. It follows from V, p. 30, Prop. 2 that there exists a finite extension $ L $ of $ K $ such that $ \mathfrak{F}_{(L)} $ is diagonalisable. In fact $ L $ may be taken to be *Galois*; indeed, taking a finite subset $ \mathfrak{F}' $ of $ \mathfrak{F} $ which generates $ A $, we may take $ L $ to be a splitting field for the minimal polynomials of the elements of $ \mathfrak{F}' $ (Prop. 12 and 13).

### 9. **Jordan decomposition

#### Definition 8 {#alg-vii-s5-def-8 .statement}

*Let $ E $ be a finite dimensional vector space over a commutative field and let $ u $ be an endomorphism of $ E $. Then a Jordan decomposition of $ u $ is a pair* $ (u_s, u_n) $, *where $ u_s $ is a semi-simple endomorphism of $ E $ and $ u_n $ is a nilpotent endomorphism of $ E $, such that* $ u_s u_n = u_n u_s $ *and* $ u = u_s + u_n $.

#### Theorem 1 {#alg-vii-s5-thm-1 .statement}

*Let $ E $ be a finite dimensional vector space over a commutative field $ K $ and let $ u $ be an endomorphism of $ E $. Then $ u $ has a Jordan decomposition* $ (u_s, u_n) $ *if and only if the eigenvalues of $ u $ are separable over $ K $. Moreover the decomposition is unique, the characteristic polynomials of $ u $ and $ u_s $ coincide, and there exist polynomials* $ P, Q \in K[X] $, *with no constant terms, such that* $ u_s = P(u) $ *and* $ u_n = Q(u) $.

A) Let us first of all prove the following special case

#### Lemma 4 {#alg-vii-s5-lem-4 .statement}

*Let $ E $ be a finite dimensional vector space over a commutative field $ K $ and let $ u $ be a triangularisable endomorphism of $ E $. Then there exists a unique diagonalisable endomorphism $ v $ of $ E $ which commutes with $ u $ and is such that* $ u - v $ *is nilpotent. Moreover, under these conditions the characteristic polynomials of $ u $ and $ v $ coincide, and there exists a polynomial* $ P \in K[X] $ *such that* $ v = P(u) $.

Let $ v $ be a diagonalisable endomorphism of $ E $ such that $ uv = vu $ and $ v - u $ is nilpotent; let $ \alpha $ be an eigenvalue of $ v $ and let $ V_\alpha $ be the corresponding eigenspace. By Lemma 3 (VII, p. 41), $ V_\alpha $ is closed under $ u $, and the restriction of u - α to V, is also the restriction of u - v, so is nilpotent; hence V, is contained in the subspace M, consisting of those x ∈ E which are annihilated by some power of u - a. Since E is the direct sum of the V, and also of the M, (VII, p. 34, Prop. 7), this shows that V, = M, for all a. By the corollary to Prop. 9 (VII, p. 36) it follows that χ_u = χ_v ; it also follows that v is uniquely determined by u ; its restriction to each M_α is the homothety defined by α.

Conversely, let us define v by the above condition; it is clear that v is diagonalisable and that u - v is nilpotent. By Prop. 7 of VII, p. 34 there exist polynomials q, such that, for all x ∈ E, the component of x in M, is q_α(u).x. Then v = ∑ αq_α(u); this implies that u and v commute and completes the proof.

B) Now let us return to the proof of Th. 1.

First of all, suppose that u can be written in the form s + n, where s is absolutely semi-simple and n is nilpotent, and where s and n commute. Let Ω be an algebraic closure of K; then u_{(Ω)} = s_{(Ω)} + n_{(Ω)}, where s_{(Ω)} is diagonalisable and n_{(Ω)} is nilpotent, and where s_{(Ω)} and n_{(Ω)} commute; by Lemma 4 it follows that s_{(Ω)}, and so also s, is unique, that the polynomials χ_{u_{(Ω)}} and χ_{s_{(Ω)}} in Ω[X] coincide, hence also the polynomials χ_u and χ_s, and that s can be expressed as a polynomial in u with coefficients in Ω. This shows first of all that the eigenvalues of u are the same as those of s, so are separable over K (VII, p. 42, Prop. 15); in addition, since s is an 0-linear combination of powers of u, it is also a K-linear combination of these same powers (II, p. 311, Prop. 19), and there exists a polynomial P ∈ K[X] such that s = P(u), hence n = Q(u) where Q(X) = X - P(X). Now let us show that Q (and hence P) may be chosen with no constant term. If u is invertible then its characteristic polynomial has a nonzero constant term, and the Cayley-Hamilton theorem (III, p. 541, Prop. 20) shows that 1 can be expressed as a polynomial in u with no constant term, so the assertion holds in this case. If u is not invertible, then its kernel W is nonzero and closed under n (VII, p. 41, Lemma 3); since the restriction of n to W is nilpotent, there exists a vector x ≠ 0 in W such that u(x) = n(x) = 0, which shows that Q cannot have a constant term.

Conversely, suppose that the eigenvalues of u are separable over K, and let L be a finite Galois extension of K containing these eigenvalues. By Lemma 4 we can write u_{(L)} = v + w, where v is diagonalisable and w is nilpotent, and where vw = wv. Let B be a basis of E, let B' be the corresponding basis of L ⊗_K E, and let U, V, W be the matrices of u_{(L)}, v, w with respect to B'; note that U is also the matrix of u with respect to B, so has entries in K. For every K-automorphism σ of L, and every matrix A with entries in L, let A" denote the matrix obtained by applying σ to the entries of A. Let a be a K-automorphism of L; then U = U^σ = (V + W)^σ = V^σ + W^σ, V^σW^σ = (VW)^σ = (WV)^σ = W^σV^σ; since Vu is the matrix of a diagonalisable endomorphism and W" is nilpotent, it follows from Lemma 4 that Vu = V and W^σ = W. Since this is valid for all σ, the entries of V and W are in K; if $ u_s $ and $ u_n $ are the endomorphisms of E with matrices V and W with respect to B, then $ (u_s)_{(L)} = v $ and $ (u_n)_{(L)} = w $. It follows that $ u_s $ is absolutely semi-simple, that $ u_n $ is nilpotent, that $ u_s $ and $ u_n $ commute, and that $ u = u_s + u_n $. This completes the proof.

Whenever an endomorphism f admits a Jordan decomposition, we write it (f,, f,), and the endomorphisms f, and f, are called the absolutely *semi-simple* component and the nilpotent component off respectively. When K is perfect, every endomorphism has a Jordan decomposition; in this case also there is no distinction between absolutely semi-simple endomorphisms and semi-simple endomorphisms, and we sometimes say « semi-simple component » for « absolutely semi-simple component ».

#### Corollary 1 {#alg-vii-s5-lem-4-cor-1 .statement}

Suppose $ u $ has a Jordan decomposition, and let L be an extension of K. Then $ u_{(L)} $ has a Jordan decomposition, with $ (u_{(L)})_s = (u_s)_{(L)} $ and $ (u_{(L)})_n = (u_n)_{(L)} $.

#### Corollary 2 {#alg-vii-s5-lem-4-cor-2 .statement}

Suppose u has a Jordan decomposition. Then every *endomorphism* of E which *commutes* with u also commutes with $ u_s $ and $ u_n $.

#### Corollary 3 {#alg-vii-s5-lem-4-cor-3 .statement}

Let $ u $ and $ v $ be two commuting endomorphisms of E which have Jordan decompositions.
a) The endomorphisms $ u, v, u_s, v_s, u_n, v_n, v, $ all commute.
b) The endomorphisms $ u + v $ and $ uv $ have Jordan decompositions with
$$
(u + v)_s = u_s + v_s , \quad (u + v)_n = u_n + v_n , \quad (uv)_s = u_s v_s ,
$$
$$
(uv)_n = u_s v_n + u_n v_s + u_n v_n .
$$
Part a) follows from Cor. 2. To prove part b) it is enough to notice that $ u_s + v_s $ and $ u_s v_s $ are absolutely semi-simple (VII, p. 43, Cor.) and that $ u_n + v_n $ and $ u_s v_n + u_n v_s + u_n v_n $ are nilpotent (as sums of commuting nilpotent endomorphisms).

#### Corollary 4 {#alg-vii-s5-lem-4-cor-4 .statement}

Suppose $ u $ has a Jordan decomposition, and let R be a polynomial in $ \mathbf{K}[X] $. Then the endomorphism $ R(u) $ has a Jordan decomposition with $ R(u)_s = R(u_s) $.

#### Remark {#alg-vii-s5-n9-rem-1 .statement}

— 1) We have $ \det(u_s) = \det(u) $ and $ \operatorname{Tr}(u_s) = \operatorname{Tr}(u) $.
2) A necessary and sufficient condition for $ u $ to be triangularisable is that $ u $ have a Jordan decomposition with $ u_s $ diagonalisable. Then there exists a basis of E with respect to which the matrix of $ u $ is lower triangular, and that of $ u_s $ is diagonal, with the same diagonal as the matrix of $ u $ (cf. Lemma 4 and Prop. 19 below).
Note however that if the matrix of $ u $ with respect to some basis is triangular, it does not in general follow that the matrix of $ u_s $ with respect to the same basis is diagonal.

3) The notion of Jordan decomposition for a square matrix can be defined in an analogous manner. For example, for the Jordan matrix $ U_{m,\alpha} $ we have
$$
(U_{m,\alpha})_s = \alpha \cdot I_m , \quad (U_{m,\alpha})_n = U_{m,0} .
$$
4) If $ u $ is semi-simple but not absolutely semi-simple, then it has no Jordan decomposition.

An endomorphism $ u $ of a vector space $ V $ over a commutative field is said to be unipotent if the endomorphism $ u - \mathrm{Id} $, is nilpotent, that is if there exists an integer $ r $ such that $ (u - \mathrm{Id},)' = 0 $; then $ u $ is an automorphism of $ V $, since if $ u = \mathrm{Id}, - n $ with $ n' = 0 $, then
$$
(\mathrm{Id}, + n + \ldots + n^{r-1})\ u = u (\mathrm{Id}_V + n + \ldots + n^{r-1}) = \mathrm{Id}_V .
$$
If $ V $ has finite dimension $ m $, then $ u $ is unipotent if and only if $ \chi_u(X) = (X - 1)^m $ (VII, p. 33, Cor. 3 to Prop. 5).

#### Proposition 17 {#alg-vii-s5-prop-17 .statement}

— Let $ E $ be a finite dimensional vector space over a commutative field, and let $ f $ be an endomorphism of $ E $. Then the following conditions are equivalent:
(i) $ f $ has a Jordan decomposition and is an automorphism ;
(ii) $ f $ has a Jordan decomposition and $ f_s $ is an automorphism ;
(iii) there exists an absolutely semi-simple automorphism $ a $ of $ E $ and a unipotent endomorphism $ u $ of $ E $ such that $ f = ua = au $.
Moreover, under these conditions, in the notation of (iii), we must have $ a = f_s $ and $ u = 1 + f_s^{-1}f_n $.
(i) $\Rightarrow$ (ii): this follows from Remark 1.
(ii) $\Rightarrow$ (iii): take $ a = f_s $ and $ u = 1 + f_s^{-1}f_n $; then $ f = ua = au $, while $ a $ is an absolutely semi-simple automorphism, and $ u $ is unipotent.
(iii) $\Rightarrow$ (i): in the notation of (iii), take $ n = a(u - 1) = (u - 1)a $. Then $ an = na $ and $ f = a + n $, and $ n $ is nilpotent. It follows that $ (a, n) $ is the Jordan decomposition of $ f $. This implies (i) as well as the relations $ a = f_s $ and $ u = 1 + f_s^{-1}f_n $.

Put $ f_r = f_s^{-1}f = ff_s^{-1} = 1 + f_s^{-1}f_n $, and call this the unipotent component of $ f $. The pair $ (f_s, f_r) $ is often called the multiplicative Jordan decomposition of the automorphism $ f $.

#### Proposition 18 {#alg-vii-s5-prop-18 .statement}

— Let $ E $ be a finite dimensional vector space over a commutative field $ K $, let $ u $ be an endomorphism of $ E $ and let $ E' $ be a subspace of $ E $ closed under $ u $. Let $ u' $ (resp. $ u'' $) be the endomorphism of $ E' $ (resp. $ E/E' $) induced by $ u $. Then $ \chi_u = \chi_{u'} \cdot \chi_{u''} $.

For $ u $ to have a Jordan decomposition, it is necessary and sufficient that $ u' $ and $ u'' $ have ; moreover, if this holds then the absolutely semi-simple (resp. nilpotent) components of $ u' $ and $ u'' $ are the endomorphisms of $ E' $ and $ E/E' $ induced by the absolutely semi-simple (resp. nilpotent) component of $ u $.

Let $ B $ be a basis of $ E $ containing a basis $ B' $ of $ E' $, and let $ B'' $ be the basis of

$E'' = E/E'$ which is the image of $B - B'$. Let $U, U', U''$ be the matrices of $u, u', u''$ with respect to $B, B', B''$ respectively. Then $U$ has the form

$$
\begin{pmatrix}
U' & Z \\
0 & U''
\end{pmatrix}
$$

and $\chi_u = \chi_U = \chi_{U'}\chi_{U''} = \chi_{u'}\chi_{u''}$ (cf. III, p. 533, Ex. 2). We deduce that the set of eigenvalues of $u$ is the union of the sets of eigenvalues of $u'$ and $u''$. If $u'$ and $u''$ have Jordan decompositions then the eigenvalues of $u'$ and $u''$ are separable over K, hence so are the eigenvalues of $u$, and $u$ has a Jordan decomposition (VII, p. 43, Th. 1). Conversely, if $u$ has a Jordan decomposition $(s, n)$ then $s$ and $n$ leave $E'$ invariant because they are polynomials in $u$; let $s', n', s'', n''$ denote the endomorphisms of $E', E', E'', E''$ induced by $s, n, s, n$ respectively. Then $s'$ and $s''$ are absolutely semi-simple, since their minimal polynomials divide that of $s$ (VII, p. 42, Prop. 15); also $n'$ and $n''$ are nilpotent. Finally $u' = s' + n', u'' = s'' + n'', s'n' = n's', \text{ and } s''n'' = n''s''$, which completes the proof.

#### Proposition 19 {#alg-vii-s5-prop-19 .statement}

— *Let E be a finite dimensional vector space over a commutative field K, and let $ \mathcal{S} $ be a set of commuting triangularisable endomorphisms of E. Then there exists a basis of E with respect to which the matrix of each element u of $ \mathcal{S} $ is lower triangular and the matrix of $ u_s $ is diagonal, with the same diagonal elements as that of u.*

By Cor. 3 of VII, p. 4.5, the set $ \mathfrak{T}_s $ of absolutely semi-simple components of elements of $ \mathfrak{T} $ consists of diagonalisable elements which commute with one another, so is diagonalisable (VII, p. 41, Prop. 13), the set $ \mathfrak{T}_n $ of nilpotent components of elements of $ \mathcal{S} $ consists of nilpotent elements which commute with one another, and each element of $ \mathfrak{T}_n $ commutes with each element of $ \mathfrak{T}_s $. Arguing as in the proof of Prop. 13 (VII, p. 41), we see that there exists a decomposition of E as a direct sum of subspaces $E_i$, which are invariant under $ \mathfrak{T}_s $ and $ \mathfrak{T}_n $, and such that the restriction of each element of $ \mathcal{S} $, to each $E$, is a homothety. Replacing $E$ by each $E$, in turn, we may assume that the elements of $ \mathcal{S} $, are homotheties; it is enough to prove that there exists a basis of E with respect to which the elements of $ \mathfrak{T}_n $ are represented by lower triangular matrices with zero diagonals; we are thus reduced to the case where $ \mathcal{S} $ consists of nilpotent elements.

Now suppose $E \neq 0$, and let F be a nonzero subspace of $E$, invariant under $ \mathfrak{T} $, of minimum dimension. Then for each $u \in \mathfrak{T}$, the kernel of the restriction of $u$ to F is nonzero and invariant under $ \mathfrak{T} $ (VII, p. 41, Lemma 3); by the choice of F the restriction of $u$ to F is thus zero for all $u \in \mathfrak{T}$. Let $x \in F,\ x \neq 0$; then $u(x) = 0$ for all $u \in \mathcal{S}$; arguing by induction on the dimension of E, we may suppose that there exists a basis $(\bar{e}_1, ..., \bar{e}_{n-1})$ of the quotient $E' = E/Kx$ such that, for all $u \in \mathfrak{T}$, the endomorphism $\bar{u}$ of $E'$ induced by $u$ has a matrix with respect to this basis which is lower triangular with zero diagonal; if $e_i \in E$ projects onto a, for $i = 1, ..., n-1$, then the basis $(e_1, ..., e_{n-1}, x)$ satisfies the required conditions.

Exercises

### Exercises {#alg-vii-s5-exercises}

All fields in this section are commutative unless explicitly stated otherwise.

See the [exercises for § 5](exercises/s5/).
