---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 4
section_title: Complex number spaces and projective spaces
lang: en
source: top-v-x
pdf_pages: 0124-0128, 0133-0136
extraction: ocr
subsections:
    - "no": 1
      title: THE VECTOR SPACE $ \mathbf{C}^n $
      page: 0
      pdf_page: 124
    - "no": 2
      title: TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $ \mathbf{C} $
      page: 0
      pdf_page: 125
    - "no": 3
      title: COMPLEX PROJECTIVE SPACES
      page: 0
      pdf_page: 125
    - "no": 4
      title: SPACES OF COMPLEX PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 127
statements: 3
exercises: 8
content_sha256: e60e8c760ae416a6a77f510d4973229c4cc0480122fbf43d4dcc8047d3c7b3bf
---

## 4. COMPLEX NUMBER SPACES AND PROJECTIVE SPACES

### 1. THE VECTOR SPACE $ \mathbf{C}^n $

Since the topological space $ \mathbf{C} $ can be identified with $ \mathbf{R}^2 $, the topological product $ \mathbf{C}^n $ of $ n $ spaces identical with $ \mathbf{C} $ can be identified with $ \mathbf{R}^{2n} $ quâ topological space; likewise, the topological group structure of $ \mathbf{C}^n $, the product of the additive (topological) group structures of the $ n $ factors, can be identified with that of the additive group $ \mathbf{R}^{2n} $. But since $ \mathbf{C} $ is a field, we may define on $ \mathbf{C}^n $ the structure of an $ n $-dimensional vector space over $ \mathbf{C} $, the product $ az $ of a complex number $ a $ and a point $ z = (z_i) $ of $ \mathbf{C}^n $ being the point $ (az_i) $; this vector space structure should be carefully distinguished from the structure of a $ 2n $-dimensional vector space over $ \mathbf{R} $, defined on $ \mathbf{R}^{2n} $ (Chapter VI, § 1, no. 3). We shall reserve the notation $ \mathbf{C}^n $ for the topological space which is the product of $ n $ spaces identical with $ \mathbf{C} $, endowed in addition with the vector space structure over $ \mathbf{C} $ which has just been defined; $ \mathbf{C}^n $ is called complex number space of $ n $ dimensions. Note that the mapping $ (t, z) \to tz $ is continuous on $ \mathbf{C} \times \mathbf{C}^n $.

An affine linear mapping of $ \mathbf{C}^n $ into $ \mathbf{C}^m $ is also an affine linear mapping of $ \mathbf{R}^{2n} $ into $ \mathbf{R}^{2m} $, but the converse is false.

For example, the mapping $ z \to \overline{z} $ is a linear mapping of the vector space $ \mathbf{R}^2 $ onto itself but is not a linear mapping of the vector space $ \mathbf{C} $ onto itself.

Every affine linear mapping of $ \mathbf{C}^n $ into $ \mathbf{C}^m $ is therefore uniformly continuous; in particular, every affine linear mapping of $ \mathbf{C}^n $ onto itself is a homeomorphism.

Every affine linear variety of $ p $ dimensions ($ p \leq n $) in the vector space $ \mathbf{C}^n $ is also an affine linear variety of $ 2p $ dimensions in the vector space $ \mathbf{R}^{2n} $; here again, the converse is false. To avoid all confusion, (affine) linear varieties of $ p $ dimensions in $ \mathbf{C}^n $ will be called complex linear varieties of $ p $ dimensions (the linear varieties of $ \mathbf{R}^{2n} $ being called real linear varieties when necessary to prevent misunderstanding). In particular, complex linear varieties of one dimension (resp. two dimensions) are called complex lines (resp. complex planes), and complex linear varieties of $ n - 1 $ dimensions are called complex hyperplanes.

It is often convenient to regard real number space $ \mathbf{R}^n $ as embedded in complex number space $ \mathbf{C}^n $, by identifying $ \mathbf{R}^n $ with the subset of $ \mathbf{C}^n $ defined by the relations $ J(z_k) = 0 $ ($ 1 \leq k \leq n $). The topological group structure induced on this subset by the topological group structure of $ \mathbf{C}^n $ coincides with that of $ \mathbf{R}^n $.

Note that $ \mathbf{R}^n $, thus embedded in $ \mathbf{C}^n $, is not a complex linear variety in $ \mathbf{C}^n $.

A system of $ p $ vectors of $ \mathbf{R}^n $ which is free over $ \mathbf{R} $ is also free over $ \mathbf{C} $. Every real linear variety $ V $ of $ p $ dimensions in $ \mathbf{R}^n $ generates a complex linear variety $ V' $ of $ p $ dimensions in $ \mathbf{C}^n $ such that $ V $ is the trace of $ V' $ on $ \mathbf{R}^n $; if $ V $ is defined by a system of $ n - p $ linear equations $ f_k(x) = a_k $, where the $ f_k $ are linear forms on $ \mathbf{R}^n $ (with real coefficients, and linearly independent over $ \mathbf{R} $) and the $ a_k $ are real numbers, then the same equations define $ V' $, but now the coordinates of $ x $ take complex values.

Conversely, if a complex linear variety of $ p $ dimensions has a non-empty intersection with $ \mathbf{R}^n $, this intersection is a real linear variety, but its dimension may be $ < p $.

### 2. TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $ \mathbf{C} $

All the definitions and all the results of nos. 5 and 6 of Chapter VI, § 1, relative to topologies on vector spaces and algebras over the field $ \mathbf{R} $, and in particular spaces and algebras of matrices with elements in $ \mathbf{R} $, remain valid with no modifications when we replace $ \mathbf{R} $ by $ \mathbf{C} $ throughout.

### 3. COMPLEX PROJECTIVE SPACES

With the notation recalled in Chapter VI, § 3, no. 1, we make the following definition, analogous to the definition of real projective spaces:

#### Definition 1 {#top-viii-s4-def-1 .statement}

*The projective space* $ \mathbf{P}_n(\mathbf{C}) $, *endowed with the topology which is the quotient of that of* $ \mathbf{C}_{n+1}^* $ *by the equivalence relation* $ \Delta_n(\mathbf{C}) $, *is called complex projective space of* $ n $ *dimensions.*

The projective space $ \mathbf{P}_1(\mathbf{C}) $ is called the *complex projective line*, and $ \mathbf{P}_2(\mathbf{C}) $ is called the *complex projective plane*.

Most of the arguments relating to real projective spaces extend with very slight modifications to complex projective spaces.

In the first place we see that the topological space $ P_n(\mathbf{C}) $ is *Hausdorff* by the argument of Proposition 1 of Chapter VI, § 3. no. 1, which applies word for word simply by replacing $ \mathbf{R} $ by $ \mathbf{C} $. Again, the proof of Proposition 2 of Chapter VI, § 3. no. 1 shows that $ P_n(\mathbf{C}) $ is *compact and connected*, and homeomorphic to the quotient of the sphere $ S_{2n-1} $ (considered as embedded in the space $ C_{n-1}^* $, identified with $ R_{2n-2}^* $) by the equivalence relation induced on this sphere by $ \Delta_n(\mathbf{C}) $; the only point of difference is that now, if $ n \geqslant 0 $, the equivalence classes for this relation are homeomorphic to the circle $ S_1 $.

For this reason, Proposition 3 of Chapter VI. § 3, no. 1 has no analogue for complex projective spaces.

Next one shows, as in Chapter VI, § 3, no. 2, that every $ p $-dimensional projective linear variety in the space $ P_n(\mathbf{C}) $ is a closed set, homeomorphic to $ P_r \mathbf{C} $, and that its complement is dense in $ P_n(\mathbf{C}) $ if $ p < n $. The proof of Proposition 5 of Chapter VI, § 3, no. 2 can be transposed as it stands, simply by substituting $ \mathbf{C} $ for $ \mathbf{R} $, and shows that (if $ n \geqslant 0 $) the complement of a projective hyperplane in $ P_n(\mathbf{C}) $ is homeomorphic to $ \mathbf{C}^* $, and therefore that every point has a neighbourhood homeomorphic to $ \mathbf{C}^* $. This result allows us to *embed* complex number space $ \mathbf{C}^n $ in complex projective space $ P_n(\mathbf{C}) $, by identifying $ \mathbf{C}^* $ with the complement of a projective hyperplane, called the "hyperplane at infinity" (usually the hyperplane whose equation is $ x_0 = 0 $). In the particular case $ n = 1 $, the hyperplane at infinity is a *point*, and Alexandroff's theorem shows that $ P_1 \mathbf{C} $ is homeomorphic to the space $ \tilde{\mathbf{C}} $ obtained by compactifying the locally compact space $ \mathbf{C} $ by adjoining a "point at infinity", denoted by $ \infty $. Proposition 4 of Chapter VI. § 2, no. 4 then shows that *the complex projective line* $ P_1(\mathbf{C}) $ *is homeomorphic to the sphere* $ S_2 $.

We leave to the reader the task of enunciating the results analogous to those of Chapter VI. § 3. no. 4, for functions which take their values in $ \mathbf{C} $.

Consider the space $ \mathbf{R}^{n+1} $ as *embedded* in $ \mathbf{C}^{n+1} $ (no. 1). Let $ f $ be the canonical mapping of $ C_{n-1}^* $ onto its quotient space $ P_n(\mathbf{C}) $. The subspace $ f(\mathbf{R}_{n-1}^*) $ consists of the points of $ P_n(\mathbf{C}) $ which have at least one system of *real* homogeneous coordinates; let us show that $ f(\mathbf{R}_{n-1}^*) $ is homeomorphic to real projective space $ P_n(\mathbf{R}) $, which will allow us to consider the space $ P_n(\mathbf{R}) $ as *embedded* in $ P_n(\mathbf{C}) $. Now the relation induced by $ \Delta_n(\mathbf{C}) $ on $ \mathbf{R}_{n+1}^* $ is $ \Delta_n(\mathbf{R}) $; the canonical mapping $ \varphi $ of

$$
\mathbf{R}_{n+1}^*/\Delta_n(\mathbf{R}) = P_n(\mathbf{R})
$$

onto $ f(\mathbf{R}_{n-1}^*) $ is *continuous* (Chapter I, § 3, no. 6, Proposition 10); since

$ P_n(\mathbf{R}) $ is compact, $ \varphi $ must be a homeomorphism (Chapter I, § 9, no. 4, Theorem 2, Corollary 2).

We can also prove that $ \varphi $ is bicontinuous without using the compactness of $ P_n(\mathbf{R}) $, by invoking the criterion of Proposition 10 of Chapter I, § 3, no. 6 (see Exercise 3).

Since every vector subspace of $ p + 1 $ dimensions of $ \mathbf{R}^{n+1} $ generates a complex vector subspace of $ p + 1 $ dimensions in $ \mathbf{C}^{n+1} $, we see that every projective linear variety $ V $ of $ p $ dimensions in $ P_n(\mathbf{R}) $ ($ V $ is called a *real* projective linear variety) generates a projective linear variety $ V' $ of $ p $ dimensions in $ P_n(\mathbf{C}) $ ($ V' $ is called a *complex* projective linear variety), such that $ V $ is the trace of $ V' $ on $ P_n(\mathbf{R}) $. Moreover, every system of (homogeneous) equations of $ V $ is also a system of (homogeneous) equations of $ V' $ when we allow the variables to take complex values.

### 4. SPACES OF COMPLEX PROJECTIVE LINEAR VARIETIES

With the notation recalled in Chapter VI, § 3, no. 5, we define similarly the spaces of projective linear varieties in a complex projective space:

#### Definition 2 {#top-viii-s4-def-2 .statement}

*The quotient space* $ P_{n,p}(\mathbf{C}) $ *of the topological space* $ L_{n+1,\ p+1}(\mathbf{C}) $ *by the equivalence relation* $ \Delta_{n,p}(\mathbf{C}) $ *is called the space of projective linear varieties of* $ p \geqslant 0 $ *dimensions in the projective space* $ P_n(\mathbf{C}) $.

By the argument of Proposition 6 of Chapter VI, § 3, no. 5, we see first of all that $ P_{n,p}(\mathbf{C}) $ is *Hausdorff*. Next we prove that it is *compact* by replacing the subspace $ V_{n+1,\ p+1} $ (in the proof of Proposition 7 of Chapter VI, § 3, no. 5) by the subspace $ W_{n+1,\ p+1} $ of $ L_{n+1,\ p+1}(\mathbf{C}) $ consisting of systems of $ p + 1 $ vectors which form an *orthonormal Hermitian basis* of the vector subspace they generate; that is to say, $ W_{n+1,\ p+1} $ consists of the matrices $ X = (x_{ij}) $ which satisfy the conditions

$$
\sum_{j=0}^n x_{ij} \overline{x}_{ij} = 1 \quad (1 \leq i \leq p + 1),
$$
$$
\sum_{j=0}^n x_{ij} \overline{x}_{kj} = 0 \quad (i \neq k).
$$

The proof of Proposition 8 of Chapter VI, § 3, no. 5 extends unaltered for the space $ P_{n,p}(\mathbf{C}) $ and shows that this space is *connected* and *locally connected* and that each of its points has a neighbourhood homeomorphic to $ \mathbf{C}^{p+1,(n-p)} $. Finally the proof of Proposition 9 of Chapter VI, § 3, no. 6 applies without change, and therefore the Grassmannian $ G_{n,p}(\mathbf{C}) $ is homeomorphic to $ \mathbf{P}_{n,p}(\mathbf{C}) $.

#### Remark {#top-viii-s4-n4-rem-1 .statement}

Most of the properties common to the real and complex number spaces (resp. projective spaces) are also valid for number spaces (resp. projective spaces) defined in the same way over the division ring of quaternions $ \mathbf{H} $; indeed, they are capable of extension to many other topological fields and division rings (cf. Exercises 2 and 6).

### Exercises {#top-viii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
