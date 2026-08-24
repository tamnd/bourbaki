---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 8
section_title: Norms and traces
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.47-A V.51, A V.153
pdf_pages: 0161-0165, 0267-0267
extraction: ocr
subsections:
    - "no": 1
      title: Recall
      page: 47
      pdf_page: 161
    - "no": 2
      title: Norms and traces in etale algebras
      page: 47
      pdf_page: 161
    - "no": 3
      title: Norms and traces in extensions of finite degree
      page: 50
      pdf_page: 164
statements: 9
exercises: 2
content_sha256: ecf695e74a6f72139dba063988cb43aedaa2286d094bf1ceb5de0b1f88085933
---

## § 8. NORMS AND TRACES

Throughout this paragraph K denotes a field.

### 1. Recall

Let A be an algebra of finite degree $ n $ over K. For each $ x \in A $ we denote by $ L_x $ the linear mapping $ a \mapsto xa $ of A into itself. We recall (III, p. 543) that the trace of $ L_x $ is called the trace of x relative to A and is written $ \mathrm{Tr}_{A/K}(x) $; likewise the determinant of $ L_x $ is called the norm of x relative to A and is denoted by $ N_{A/K}(x) $. The discriminant of a sequence $ (x_1, ..., x_n) $ of n elements of A is by definition the determinant $ D_{A/K}(x_1, ..., x_n) $ of the matrix $ (\mathrm{Tr}_{A/K}(x_i x_j))_{1 \leq i,j \leq n} $ (III, p. 549).

Let K' be an extension of K and let $ A' = A_{(K')} $ be the K'-algebra derived from A by extension of scalars. We have the formulae

(1) $$
\mathrm{Tr}_{A'/K'}(1 \otimes x) = \mathrm{Tr}_{A/K}(x) . 1 , \quad N_{A'/K'}(1 \otimes x) = N_{A/K}(x) . 1
$$
for all $ x \in A $ (III, p. 544). For every sequence $ (x_1, ..., x_n) $ of elements of A we have

(2) $$
D_{A'/K'}(1 \otimes x_1, ..., 1 \otimes x_n) = D_{A/K}(x_1, ..., x_n) . 1 ,
$$
as follows from the first formula (1).

### 2. Norms and traces in etale algebras

Let A be an etale algebra of (finite) degree $ n $ over K. By definition there exist then an extension L of K and distinct homomorphisms $ u_1, ..., u_n $ of A into L with the following properties.

a) every homomorphism of $ A $ into $ L $ is equal to one of the $ u_i $ (V, p. 29, Cor.);
b) there exists an $ L $-algebra isomorphism $ u : A_{(L)} \to L^n $ such that

$$
u(1 \otimes x) = (u_1(x), \ldots, u_n(x)) \quad \text{for all } x \in A .
$$

Moreover, every algebraically closed extension $ L $ of $ K $ has the above properties (V, p. 30, Prop. 2).

We fix $ L, u_1, \ldots, u_n $ in what follows. Let $ x \in A $; we shall prove the formulae

$$
\text{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) , \quad \text{N}_{A/K}(x) \cdot 1 = \prod_{i=1}^n u_i(x) .
$$

Let $ v $ be multiplication by $ l \otimes x $ in $ A_{(L)} $; with respect to the basis of $ A_{(L)} $ which is the image under $ u^{-1} $ of the canonical basis of $ L^n $, the matrix of the linear mapping $ v $ is diagonal, with diagonal elements $ u_1(x), \ldots, u_n(x) $. We conclude that

$$
Tr_{A_{(L)}/L}(1 \circ x) \cdot 1 = \sum_{r=1}^n u_i(x) , \quad \text{whence} \quad \text{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) \text{ by (1)} ;
$$

the case of norms is treated similarly.

Further let $ (x,, \ldots, x,) $ be a sequence of elements of $ A $, let U be the matrix

$$
(u_i(x_j))_{1 \leq i,j \leq n}
$$

and let $ (t_{ij}) = 'U . U $. By the first formula (3) we have

$$
\text{Tr}_{A/K}(x_i x_j) \cdot 1 = \sum_{k=1}^n u_k(x_i x_j) = \sum_{k=1}^n u_k(x_i) u_k(x_j) = t_{ij} ;
$$

passing to determinants, we obtain

$$
D_{A/K}(x_1, \ldots, x_r) \cdot 1 = [\det u_i(x_j)]^2 .
$$

#### Proposition 1 {#alg-v-s8-prop-1 .statement}

— *Let $ A $ be a commutative algebra of finite degree over $ K $. Then the following conditions are equivalent*:
a) *The algebra $ A $ is etale.*
b) *There exists a basis of $ A $ whose discriminant is non-zero.*
c) *For each $ x \neq 0 $ in $ A $ there exists $ y $ in $ A $ such that $ \text{Tr}_{A/K}(xy) \neq 0 $.*
*Further, when these conditions are satisfied, the discriminant of any basis of $ A $ is non-zero.*

We shall show that when $ A $ is assumed etale, the discriminant of $ A $ with respect to any basis $ (x,, \ldots, x,) $ of $ A $ over $ K $ is non-zero; this will in particular establish the implication $ a) \Rightarrow b) $. By (4), with the above notation, it suffices to show that the matrix U is invertible, or equivalently, that the system of linear equations

$$
\sum_{i=1}^n \lambda_i u_i(x_j) = 0 \quad (\text{for } 1 \leq j \leq n)
$$

has only the solution $ \lambda_1 = \cdots = A, = 0 $ in L. Now the relation (5) implies $ \sum_{i=1}^n \lambda_i u_i(x) = 0 $ for all $ x \in A $, whence $ \lambda_i = 0 $ for $ 1 \leq i \leq n $, by the theorem on the linear independence of homomorphisms (V, p. 27, Th. 1).

The equivalence of b) and c) is a consequence of the following general lemma:

#### Lemma 1 {#alg-v-s8-lem-1 .statement}

Let V be a vector space of finite dimension over K and B a bilinear *form on* V x V. Let $(v_1, \ldots, v_n)$ *be a basis of* V *over* K *and* $ \Delta = \det B(v_i, v_j) $. Then $ A \neq 0 $ if and only *if*, for each $ x \neq 0 $ in V there exists y in V such that $ B(x, y) \neq 0 $.

We have $ A \neq 0 $ if and only if the system of linear equations

$$
\sum_{i=1}^n \lambda_i B(v_i, v_j) = 0 \quad (1 \leq j \leq n)
$$

has only the solution $ A, = \cdots = A, = 0 $ in K. If we put $ x = \sum_{i=1}^n \lambda_i v_i $, the above system is equivalent to $ B(x, v_j) = 0 $ for $ 1 \leq j \leq n $, or also, since $(v_1, \ldots, v_n)$ is a basis of V over K, to $ B(x, y) = 0 $ for all $ y \in V $, whence the lemma.

Let us show that condition c) implies that A is reduced. Let x be a nilpotent element of A : for any $ y \in A $ the element xy is nilpotent, and so the endomorphism $ L_{xy} $ of the vector space A is nilpotent. Now the following lemma implies that $ \mathrm{Tr}(xy) = 0 $ for all $ y \in A $, whence $ x = 0 $ under hypothesis c).

#### Lemma 2 {#alg-v-s8-lem-2 .statement}

Let V be a vector space of finite dimension over K and $ u $ a nilpotent endomorphism of V, then $ \mathrm{Tr}(u) = 0 $.

For each integer $ n \geq 0 $ let $ V_n $ be the image of $ u^n $. Since $ u $ is nilpotent, there exists an integer $ r \geq 0 $ such that $ V_0 = V, V_r = 0 $ and $ V_i \neq V_{i+1} $ for $ 0 \leq i < r - 1 $. Let d, be the dimension of $ V_{i-1} $ (for $ 1 \leq i \leq r $). There exists a basis $(x,, \ldots, x_d)$ of V such that the vectors $ x_j $ with $ d - d_i < j \leq d $ form a basis of $ V_{i-1} $ (for $ 1 \leq i \leq r $). We have $ u(V_{i-1}) \subset V_i $ and so the diagonal elements of the matrix of $ u $ for the basis $(x,, \ldots, x,) $ are zero. Thus we have $ \mathrm{Tr}(u) = 0 $ and the lemma follows.

Finally let us show that b) implies a). Let $(x,, \ldots, x_n)$ be a basis of A over K such that $ D_{A/K}(x_1, \ldots, x_n) \neq 0 $. Let K' be an extension of K, A' the K'-algebra derived from A by extension of scalars and $ x'_i = 1 \otimes x_i $ for $ 1 \leq i \leq n $. By Formula (2) (V, p. 47) we have $ D_{A'/K'}(x'_1, \ldots, x'_n) \neq 0 $. Applying the preceding result to A' we see that A' is reduced, hence the algebra A is etale (V, p. 34, Th. 4).

#### Corollary {#alg-v-s8-n2-cor-1 .statement}

— Let E be an extension *of finite* degree of K. For E to be separable it is necessary and sufficient that there exist a in E such that $ \mathrm{Tr}_{E/K}(a) \neq 0 $.

The condition is necessary by Prop. 1. Conversely, assume that there exists $ a \in E $ such that $ \mathrm{Tr}_{E/K}(a) \neq 0 $. Given $ x \neq 0 $ in E, if we put $ y = a x' $, then $ \mathrm{Tr}_{E/K}(xy) \neq 0 $. Now Prop. 1 shows that E is an etale algebra over K, hence a separable extension of K.

### 3. Norms and traces in extensions of finite degree

The transitivity formulae in algebras (III, p. 548) imply the following proposition in the case of extensions of finite degree.

#### Proposition 2 {#alg-v-s8-prop-2 .statement}

— Let F be an extension of finite degree of K and E a subextension of F. Then for every $ x \in F $ we have
$$
\text{Tr}_{F/K}(x) = \text{Tr}_{E/K}(\text{Tr}_{F/E}(x)) \\
\text{N}_{F/K}(x) = \text{N}_{E/K}(\text{N}_{F/E}(x)) .
$$

#### Corollary {#alg-v-s8-n3-cor-1 .statement}

— Put $ m = [F : E] $; then for every $ x \in E $ we have
$$
\text{Tr}_{F/K}(x) = m \cdot \text{Tr}_{E/K}(x) \\
\text{N}_{F/K}(x) = \text{N}_{E/K}(x)^m .
$$

#### Proposition 3 {#alg-v-s8-prop-3 .statement}

— Let E be an extension of finite degree n of K and x an element of E, of degree d over K. Write $ f(X) = X^d + \sum_{i=1}^d a_i X^{d-i} $ for the minimal polynomial of X over K. Then we have
$$
\text{Tr}_{E/K}(x) = - \frac{n}{d} a_1 \\
\text{N}_{E/K}(x) = (((-1)^d a_d)^{n/d} = (-1)^n a_d^{n/d} .
$$

Prop. 3 follows directly from the Cor. of Prop. 2 and the lemma:

#### Lemma 3 {#alg-v-s8-lem-3 .statement}

Let R be a commutative ring, $ f(X) = X^d + \sum_{i=1}^d a_i X^{d-i} $ a monic polynomial of $ \mathbf{R}[X] $, A the R-algebra $ \mathbf{R}[X]/(f) $ and x the residue class of X in A. Then $ \text{Tr}_{A/R}(x) = -a_1 $ and $ \text{N}_{A/R}(x) = (-1)^d a_d $.

By the Cor. (IV, p. 11) the sequence $ (1, x, ..., x^{d-1}) $ is a basis of A ; further we have
$$
x \cdot 1 = x , \quad x \cdot x = x^2 , \ldots , x \cdot x^{d-2} = x^{d-1} ,
$$
$$
x \cdot x^{d-1} = -a_d \cdot 1 - a_{d-1} \cdot x - \ldots - a_1 \cdot x^{d-1}
$$

The matrix which expresses the multiplication by x with respect to the basis $ (1, x, ..., x^{d-1}) $ of $ A $ is thus of the following form (we have taken $ d = 5 $ to fix the ideas):

$$
\begin{pmatrix}
0 & 0 & 0 & 0 & -a \\
1 & 0 & 0 & 0 & -a \\
0 & 1 & 0 & 0 & -a_3 \\
0 & 0 & 1 & 0 & -a_2 \\
0 & 0 & 0 & 1 & -a_1
\end{pmatrix}
$$

The trace of this matrix is clearly $ -a $; the determinant may be calculated by expanding by the first row, and we then find

$$
(-1)^{d-1} (-a_d) = (-1)^d a_d .
$$

For the rest of this No. we denote by E an extension of finite degree of K and by $ x $ an element of E. We shall indicate how to calculate the norm and trace of $ x $ in various cases.

$ a) $ *Case of a separable extension*: suppose that E is separable of degree $ n $ over K, denote by $ \Omega $ an algebraic closure of K and by $ \sigma_1, \ldots, \sigma_n $ the $ n $ distinct $ K $-homomorphisms of E into R. By Formula (3) ($ V $, p. 48) we have in R

$$
\text{Tr}_{E/K}(x) = \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = \prod_{i=1}^n \sigma_i(x) .
$$

$ b) $ *Case of a p-radical extension*: suppose that K is of characteristic $ p > 0 $ and that the extension E is p-radical; there exists an integer $ e \geq 0 $ such that $[E:K] = p^e$ ($ V $, p. 26, Prop. 4). If $ f $ is the height of $ x $ over K, the minimal polynomial of $ x $ over K is $ X^{p^f} - x^{p^f} $ ($ V $, p. 24, Prop. 1). By Prop. 3 we have $ N_{E/K}(x) = (x^{p^f})^{p^e/p^f} $, whence

$$
N_{E/K}(x) = x^{p^e} = x^{[E:K]}
$$

For the trace we find $ \text{Tr}_{E/K}(x) = -p^{e-f} a $, where $ a $ is the coefficient of $ X^{p^f-1} $ in the polynomial $ X^{p^f} - x^{p^f} $; in other words, we have

$$
\text{Tr}_{E/K}(x) = p^e \cdot x = [E:K] x = \begin{cases} x & \text{if } [E:K] = 1 \\ 0 & \text{if } [E:K] > 1 . \end{cases}
$$

$ c) $ *General case*: we can summarize the calculation of norm and trace in the following proposition:

#### Proposition 4 {#alg-v-s8-prop-4 .statement}

*Let p be the characteristic exponent of K and E an extension of finite degree of K. Let $ \sigma_1, \ldots, \sigma_n $ be the distinct K-homomorphisms of E into an algebraic closure $ \Omega $ of K, and let $ p^e = [E:K]_i $. For each $ x \in E $ we have in $ \Omega $*

$$
\text{Tr}_{E/K}(x) = p^e \cdot \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = \left( \prod_{i=1}^n \sigma_i(x) \right)^{p^e} .
$$

Let E, be the relative separable closure of K in E; then $ E_s $ is a separable extension of degree $ n $ of K and $ \sigma_1, \ldots, \sigma_n $ induce distinct K-homomorphisms of E, into R; further, E is ap-radical extension of E, of degreep$^e$ ($ V $, p. 44, Prop. 13 and p. 46). So Prop. 4 follows from the Formulae (6), (7), (13), (14) and (12).

### Exercises {#alg-v-s8-exercises}

See the [exercises for § 8](exercises/s8/).
