---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 1
section_title: FIRST DERIVATIVE
lang: en
source: fvr-i-vii
pdf_pages: 0018-0027, 0050-0052
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVE OF A VECTOR FUNCTION
      page: 0
      pdf_page: 18
    - "no": 2
      title: LINEARITY OF DIFFERENTIATION
      page: 0
      pdf_page: 20
    - "no": 3
      title: DERIVATIVE OF A PRODUCT
      page: 0
      pdf_page: 21
    - "no": 4
      title: DERIVATIVE OF THE INVERSE OF A FUNCTION
      page: 0
      pdf_page: 23
    - "no": 5
      title: DERIVATIVE OF A COMPOSITE FUNCTION
      page: 0
      pdf_page: 24
    - "no": 6
      title: DERIVATIVE OF AN INVERSE FUNCTION
      page: 0
      pdf_page: 24
    - "no": 7
      title: DERIVATIVES OF REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 25
statements: 31
exercises: 9
content_sha256: 9e452a8a87bd744096308ba376bdee0283bca25aeb29ff2316660fa2697ceaa1
---

## § 1. FIRST DERIVATIVE

As was said in the Introduction, in this chapter and the next we shall study the infinitesimal properties of functions which are defined on a subset of the real field $ \mathbf{R} $ and take their values in a *Hausdorff topological vector space* E over the field $ \mathbf{R} $; for brevity we shall say that such a function is a *vector function of a real variable*. The most important case is that where $ E = \mathbf{R} $ (real-valued functions of a real variable). When $ E = \mathbf{R}^n $, consideration of a vector function with values in E reduces to the simultaneous consideration of $ n $ finite real functions.

Many of the definitions and properties stated in chapter I extend to functions which are defined on a subset of the field $ \mathbf{C} $ of complex numbers and take their values in a topological vector space over $ \mathbf{C} $ (vector functions of a complex variable). Some of these definitions and properties extend even to functions which are defined on a subset of an arbitrary commutative *topological field* K and take their values in a topological vector space over K.

We shall indicate these generalizations in passing (see in particular I, p. 10, *Remark 2*), emphasising above all the case of functions of a complex variable, which are by far the most important, together with functions of a real variable, and will be studied in greater depth in a later Book.

### 1. DERIVATIVE OF A VECTOR FUNCTION

#### Definition 1 {#fvr-i-s1-def-1 .statement}

*Let $ f $ be a vector function defined on an interval $ I \subset \mathbf{R} $ which does not reduce to a single point. We say that $ f $ is differentiable at a point $ x_0 \in I $ if*
$$
\lim_{x \to x_0, x \in I, x \neq x_0} \frac{f(x) - f(x_0)}{x - x_0}
$$
*exists (in the vector space where $ f $ takes its values); the value of this limit is called the first derivative (or simply the derivative) of $ f $ at the point $ x_0 $, and it is denoted by $ f'(x_0) $ or $ Df(x_0) $.*

If $ f $ is differentiable at the point $ x_0 $, so is the *restriction* of $ f $ to any interval $ J \subset I $ which does not reduce to a single point and such that $ x_0 \in J $; and the derivative of this restriction is equal to $ f'(x_0) $. Conversely, let $ J $ be an interval contained in $ I $ and containing a neighbourhood of $ x_0 $ relative to $ I $; if the restriction of $ f $ to $ J $ admits a derivative at the point $ x_0 $, then so does $ f $.

We summarise these properties by saying that the concept of derivative is a local concept.

#### Remark 1 {#fvr-i-s1-n1-rem-1 .statement}

In Kinematics, if the point $ \mathbf{f}(t) $ is the position of a moving point in the space $ \mathbf{R}^3 $ at time $ t $, then $ \frac{\mathbf{f}(t) - \mathbf{f}(t_0)}{t - t_0} $ is termed the average velocity between the instants $ t_0 $ and $ t $, and its limit $ \mathbf{f}'(t_0) $ is the instantaneous velocity (or simply velocity) at the time $ t_0 $ (when this limit exists).*
2) If a function $ \mathbf{f} $, defined on $ I $, is differentiable at a point $ x_0 \in I $, it is necessarily continuous relative to $ I $ at this point.

#### Definition 2 {#fvr-i-s1-def-2 .statement}

*Let $ \mathbf{f} $ be a vector function defined on an interval $ I \subset \mathbf{R} $, and let $ x_0 $ be a point of $ I $ such that the interval $ I \cap [x_0, +\infty[ $ (resp. $ I \cap ]-\infty, x_0] $) does not reduce to a single point. We say that $ \mathbf{f} $ is differentiable on the right (resp. on the left) at the point $ x_0 $ if the restriction of $ \mathbf{f} $ to the interval $ I \cap [x_0, +\infty[ $ (resp. $ I \cap ]-\infty, x_0] $) is differentiable at the point $ x_0 $; the value of the derivative of this restriction at the point $ x_0 $ is called the right (resp. left) derivative of $ \mathbf{f} $ at the point $ x_0 $ and is denoted by $ \mathbf{f}'_d(x_0) $ (resp. $ \mathbf{f}'_g(x_0) $).*

Let $ \mathbf{f} $ be a vector function defined on $ I $, and $ x_0 $ an interior point of $ I $ such that $ \mathbf{f} $ is continuous at this point; it follows from defs. 1 and 2 that for $ \mathbf{f} $ to be differentiable at $ x_0 $ it is necessary and sufficient that $ \mathbf{f} $ admit both a right and a left derivative at this point, and that these derivatives be equal; and then

$$
\mathbf{f}'(x_0) = \mathbf{f}'_d(x_0) = \mathbf{f}'_g(x_0).
$$

#### Example 1 {#fvr-i-s1-n1-exa-1 .statement}

A constant function has zero derivative at every point.
2) An affine linear function $ x \mapsto ax + b $ has derivative equal to $ a $ at every point.
3) The real function $ 1/x $ (defined for $ x \neq 0 $) is differentiable at each point $ x_0 \neq 0 $, for we have $ \left( \frac{1}{x} - \frac{1}{x_0} \right) / (x - x_0) = -\frac{1}{x x_0} $, and, since $ 1/x $ is continuous at $ x_0 $, the limit of the preceding expression is $ -1/x_0^2 $.
4) The scalar function $ |x| $, defined on $ \mathbf{R} $, has right derivative $ +1 $ and left derivative $ -1 $ at $ x = 0 $; it is not differentiable at this point.
*5) The real function equal to 0 for $ x = 0 $, and to $ x \sin 1/x $ for $ x \neq 0 $, is defined and continuous on $ \mathbf{R} $, but has neither right nor left derivative at the point $ x \neq 0 $.* One can give examples of functions which are continuous on an interval and fail to have a derivative at every point of the interval (I, p. 35, exerc. 2 and 3).

#### Definition 3 {#fvr-i-s1-def-3 .statement}

*We say that a vector function $ \mathbf{f} $ defined on an interval $ I \subset \mathbf{R} $ is differentiable (resp. right differentiable, left differentiable) on $ I $ if it is differentiable (resp. right differentiable, left differentiable) at each point of $ I $; the function $ x \mapsto \mathbf{f}'(x) $ (resp. $ x \mapsto \mathbf{f}'_d(x) $, $ x \mapsto \mathbf{f}'_g(x) $) defined on $ I $, is called the derived function, or (by abuse of language) the derivative (resp. right derivative, left derivative) of $ \mathbf{f} $, and is denoted by $ \mathbf{f}' $ or $ \mathrm{Df} $ or $ d\mathbf{f}/dx $ (resp. $ \mathbf{f}'_d, \mathbf{f}'_g $).*

#### Remark {#fvr-i-s1-n1-rem-2 .statement}

A function may be differentiable on an interval without its derivative being continuous at every point of the interval (*cf.* I, p. 36, exerc. 5); *this is shown by the example of the function equal to 0 for $ x = 0 $ and to $ x^2 \sin 1/x $ for $ x \neq 0 $; it has a derivative everywhere, but this derivative is discontinuous at the point $ x = 0 $.

### 2. LINEARITY OF DIFFERENTIATION

#### Proposition 1 {#fvr-i-s1-prop-1 .statement}

*The set of vector functions defined on an interval $ I \subset \mathbf{R} $, taking values in a given topological vector space $ E $, and differentiable at the point $ x_0 $, is a vector space over $ \mathbf{R} $, and the map $ f \mapsto Df(x_0) $ is a linear mapping of this space into $ E $.*

In other words, if $ f $ and $ g $ are defined on $ I $ and differentiable at the point $ x_0 $, then $ f + g $ and $ fa $ ($ a $ an arbitrary scalar) are differentiable at $ x_0 $ and their derivatives there are $ f'(x_0) + g'(x_0) $ and $ f'(x_0)a $ respectively. This follows immediately from the continuity of $ x + y $ and of $ xa $ on $ E \times E $ and $ E $ respectively.

#### Corollary {#fvr-i-s1-n2-cor-1 .statement}

*The set of vector functions defined on an interval $ I $, taking values in a given topological vector space $ E $, and differentiable on $ I $, is a vector space over $ \mathbf{R} $, and the map $ f \mapsto Df $ is a linear mapping of this space into the vector space of mappings from $ I $ into $ E $.*

#### Remark {#fvr-i-s1-n2-rem-1 .statement}

If one endows the vector space of mappings from $ I $ into $ E $ and its subspace of differentiable mappings (*cf. Gen. Top.*, X, p. 277) with the topology of simple convergence (or the topology of uniform convergence), the linear mapping $ f \mapsto Df $ *is not continuous* (in general) *for example, the sequence of functions* $ f_n(x) = \sin n^2 x / n $ *converges uniformly to* 0 *on* $ \mathbf{R} $, *but the sequence of derivatives* $ f'_n(x) = n \cos n^2 x $ *does not converge even simply to* 0.

#### Proposition 2 {#fvr-i-s1-prop-2 .statement}

*Let $ E $ and $ F $ be two topological vector spaces over $ \mathbf{R} $, and $ u $ a continuous linear map from $ E $ into $ F $. If $ f $ is a vector function defined on an interval $ I \subset \mathbf{R} $, taking values in $ E $, and differentiable at the point $ x_0 \in I $, then the composite function $ u \circ f $ has a derivative equal to $ u(f'(x_0)) $ at $ x_0 $.*

Indeed, since $ \frac{u(f(x)) - u(f(x_0))}{x - x_0} = u \left( \frac{f(x) - f(x_0)}{x - x_0} \right) $, this follows from the continuity of $ u $.

#### Corollary {#fvr-i-s1-n2-cor-2 .statement}

*If $ \varphi $ is a continuous linear form on $ E $, then the real function $ \varphi \circ f $ has a derivative equal to $ \varphi(f'(x_0)) $ at the point $ x_0 $.*

#### Example 1 {#fvr-i-s1-n2-exa-1 .statement}

Let $ f = (f_i)_{1 \leq i \leq n} $ be a function with values in $ \mathbf{R}^n $, defined on an interval $ I \subset \mathbf{R} $; each real function $ f_i $ is none other than the composite function $ \mathrm{pr}_i \circ f $, so is differentiable at the point $ x_0 $ if $ f $ is, and, if so, $ f'(x_0) = (f'_i(x_0))_{1 \leq i \leq n} $.

#### Example 2 {#fvr-i-s1-n2-exa-2 .statement}

In Kinematics, if $ f(t) $ is the position of a moving point $ M $ at time $ t $, if $ g(t) $ is the position at the same instant of the projection $ M' $ of $ M $ onto a plane $ P $ (resp. a line $ D $) with kernel a line (resp. a plane) not parallel to $ P $ (resp. $ D $), then $ g $ is the composition of the projection $ u $ of $ \mathbf{R}^3 $ onto $ P $ (resp. $ D $) and of $ f $; since $ u $ is a (continuous) linear mapping one sees that the projection of the velocity of a moving point onto a plane (resp. a line) is equal to the velocity of the projection of the moving point onto the plane (resp. line).*

#### Example 3 {#fvr-i-s1-n2-exa-3 .statement}

Let $ f $ be a complex-valued function defined on an interval $ I \subset \mathbf{R} $, and let $ a $ be an arbitrary complex number; prop. 2 shows that if $ f $ is differentiable at a point $ x_0 $ then so is $ af $, and the derivative of this function at $ x_0 $ is equal to $ af'(x_0) $.

### 3. DERIVATIVE OF A PRODUCT

Let us now consider $ p $ topological vector spaces $ E_i $ ($ 1 \leq i \leq p $) over $ \mathbf{R} $, and a continuous multilinear $ ^1 $ map (which we shall denote by

$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1.x_2 \ldots x_p])
$$

of $ E_1 \times E_2 \times \cdots \times E_p $ into a topological vector space F over $ \mathbf{R} $.

PROPOSITION 3 . *For each index $ i $ ($ 1 \leq i \leq p $) let $ f_i $ be a function defined on an interval $ I \subset \mathbf{R} $, taking values in $ E_i $, and differentiable at the point $ x_0 \in I $. Then the function

$$
x \mapsto [f_1(x).f_2(x) \ldots f_p(x)]
$$

defined on $ I $ with values in $ F $ has a derivative equal to

$$
\sum_{i=1}^p [f_1(x_0) \ldots f_{i-1}(x_0).f'_i(x_0).f_{i+1}(x_0) \ldots f_p(x_0)]
$$

at $ x_0 $.

Let us put $ h(x) = [f_1(x).f_2(x) \ldots f_p(x)] $; then, by the identity

$$
[b_1.b_2 \ldots b_p] - [a_1.a_2 \ldots a_p] = \sum_{i=1}^p [b_1 \ldots b_{i-1}.(b_i - a_i).a_{i+1} \ldots a_p],
$$

we can write

$$
h(x) - h(x_0) = \sum_{i=1}^p [f_1(x) \ldots f_{i-1}(x).(f_i(x) - f_i(x_0)).f_{i+1}(x_0) \ldots f_p(x_0)].
$$

On multiplying both sides by $ \frac{1}{x - x_0} $ and letting $ x $ approach $ x_0 $ in $ I $, we obtain the expression (1), since both the map

$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1.x_2 \ldots x_p]
$$

and addition in F are continuous.

$ ^1 $ Recall (Alg., II, p. 265) that a map $ f $ of $ E_1 \times E_2 \times \cdots \times E_p $ into F is said to be *multilinear* if each partial mapping

$$
x_i \mapsto f(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_p)
$$

from $ E_i $ into F ($ 1 \leq i \leq p $) is a *linear* map, the $ a_j $ for indices $ j \neq i $ being arbitrary in $ E_j $. We note that if the $ E_i $ are *finite* dimensional over $ \mathbf{R} $ then every multilinear map of $ E_1 \times E_2 \times \cdots \times E_p $ into F is necessarily *continuous*; this need not be so if some of these spaces are topological vector spaces of infinite dimension.

When some of the functions $ f_i $ are constant, the terms in the expression (1) containing their derivatives $ f'_i(x_0) $ are zero.

Let us consider in detail the particular case $ p = 2 $, the most important in applications: if $ (\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}.\mathbf{y}] $ is a continuous bilinear map of $ E \times F $ into $ G $, (E, F, G being topological vector spaces over $ \mathbf{R} $), and $ \mathbf{f} $ and $ \mathbf{g} $ are two vector functions, differentiable at $ x_0 $, with values in E and F respectively, then the vector function $ x \mapsto [\mathbf{f}(x).\mathbf{g}(x)] $ (which we denote by $ [\mathbf{f}.\mathbf{g}] $) has a derivative equal to $ [\mathbf{f}'(x_0).\mathbf{g}(x_0)] + [\mathbf{f}(x_0).\mathbf{g}'(x_0)] $ at $ x_0 $. In particular, if $ \mathbf{a} $ is a constant vector, then $ [\mathbf{a}.\mathbf{f}] $ (resp. $ [\mathbf{f}.\mathbf{a}] $) has a derivative equal to $ [\mathbf{a}.\mathbf{f}'(x_0)] $ (resp. $ [\mathbf{f}'(x_0).\mathbf{a}] $) at $ x_0 $.

If $ \mathbf{f} $ and $ \mathbf{g} $ are both differentiable on I then so is $ [\mathbf{f}.\mathbf{g}] $, and we have

$$
[\mathbf{f}.\mathbf{g}]' = [\mathbf{f}'.\mathbf{g}] + [\mathbf{f}.\mathbf{g}'].
$$

(2)

#### Example 1 {#fvr-i-s1-n3-exa-1 .statement}

Let $ f $ be a real function, $ \mathbf{g} $ a vector function, both differentiable at a point $ x_0 $; the function $ \mathbf{g}f $ has a derivative equal to $ \mathbf{g}'(x_0)f(x_0) + \mathbf{g}(x_0)f'(x_0) $ at $ x_0 $. In particular, if $ \mathbf{a} $ is constant, then $ \mathbf{a}f $ has derivative $ \mathbf{a}f'(x_0) $. This last remark, in conjunction with example 1 of I, p. 5, proves that if $ \mathbf{f} = (f_i)_{1 \leq i \leq n} $ is a vector function with values in $ \mathbf{R}^n $, then for $ \mathbf{f} $ to be differentiable at the point $ x_0 $ it is necessary and sufficient that each of the real functions $ f_i $ ($ 1 \leq i \leq n $) be differentiable there: for, if $ (\mathbf{e}_i)_{1 \leq i \leq n} $ is the canonical basis of $ \mathbf{R}^n $, we can write $ \mathbf{f} = \sum_{i=1}^n \mathbf{e}_i f_i $.

#### Example 2 {#fvr-i-s1-n3-exa-2 .statement}

The real function $ x^n $ arises from the multilinear function

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n
$$

defined on $ \mathbf{R}^n $, by substituting $ x $ for each of the $ x_i $; so prop. 3 shows that $ x^n $ is differentiable on $ \mathbf{R} $ and has derivative $ nx^{n-1} $. As a result the polynomial function $ \mathbf{a}_0 x^n + \mathbf{a}_1 x^{n-1} + \cdots + \mathbf{a}_{n-1} x + \mathbf{a}_n $ (the $ \mathbf{a}_i $ being constant vectors) has derivative

$$
n \mathbf{a}_0 x^{n-1} + (n-1) \mathbf{a}_1 x^{n-2} + \cdots + \mathbf{a}_{n-1};
$$

when the $ \mathbf{a}_i $ are real numbers this function coincides with the derivative of a polynomial function as defined in Algebra (A, IV).

#### Example 3 {#fvr-i-s1-n3-exa-3 .statement}

The euclidean scalar product $ (\mathbf{x}| \mathbf{y}) $ (Gen. Top , VI, p. 40) is a bilinear map (necessarily continuous) of $ \mathbf{R}^n \times \mathbf{R}^n $ into $ \mathbf{R} $. If $ \mathbf{f} $ and $ \mathbf{g} $ are two vector functions with values in $ \mathbf{R}^n $, and differentiable at the point $ x_0 $, then the real function $ x \mapsto (\mathbf{f}(x)|\mathbf{g}(x)) $ has a derivative equal to $ (\mathbf{f}'(x_0)|\mathbf{g}(x_0)) + (\mathbf{f}(x_0)|\mathbf{g}'(x_0)) $ at the point $ x_0 $. There is an analogous result for the hermitian scalar product on $ \mathbf{C}^n $, this space being considered as a vector space over $ \mathbf{R} $.

Let us consider in particular the case where the euclidean norm $ \| \mathbf{f}(x) \| $ is constant, so that $ (\mathbf{f}(x)|\mathbf{f}(x)) = \| \mathbf{f}(x) \|^2 $ is also constant; on writing that the derivative of $ (\mathbf{f}(x)|\mathbf{f}(x)) $ vanishes at $ x_0 $ we obtain $ (\mathbf{f}(x_0)|\mathbf{f}'(x_0)) = 0 $; in other words, $ \mathbf{f}'(x_0) $ is orthogonal to $ \mathbf{f}(x_0) $.

#### Example 4 {#fvr-i-s1-n3-exa-4 .statement}

If $ E $ is a topological algebra over $ \mathbf{R} $ (cf. Introduction), the product $ xy $ of two elements of $ E $ is a continuous bilinear function of $ (x, y) $; if $ \mathbf{f} $ and $ \mathbf{g} $ have their values in $ E $ and are differentiable at the point $ x_0 $, then the function $ x \mapsto \mathbf{f}(x)\mathbf{g}(x) $ has a derivative equal to $ \mathbf{f}'(x_0)\mathbf{g}(x_0) + \mathbf{f}(x_0)\mathbf{g}'(x_0) $ at $ x_0 $. In particular, if $ U(x) = (\alpha_{ij}(x)) $ and $ V(x) = (\beta_{ij}(x)) $ are two square matrices of order $ n $, differentiable at $ x_0 $, their product $ UV $ has a derivative equal to $ U'(x_0)V(x_0) + U(x_0)V'(x_0) $ at $ x_0 $ (where $ U'(x) = (\alpha'_{ij}(x)) $ and $ V'(x) = (\beta'_{ij}(x)) $).

#### Example 5 {#fvr-i-s1-n3-exa-5 .statement}

The determinant $ \det(\mathbf{x}_1, \mathbf{x}_2, \ldots, \mathbf{x}_n) $ of $ n $ vectors $ \mathbf{x}_i = (x_{ij})_{1 \leq i \leq n} $ from the space $ \mathbf{R}^n $ (Alg., III, p. 522) being a (continuous) multilinear function of the $ \mathbf{x}_i $, one sees that if the $n^2$ real functions $ f_{ij} $ are differentiable at $ x_0 $, then their determinant $ g(x) = \det(f_{ij}(x)) $ has a derivative equal to
$$
\sum_{i=1}^n \left[ \mathbf{f}_1(x_0), \ldots, \mathbf{f}_{i-1}(x_0), \mathbf{f}_i'(x_0), \mathbf{f}_{i+1}(x_0), \ldots, \mathbf{f}_n(x_0) \right]
$$
at $ x_0 $, where $ \mathbf{f}_i(x) = (f_{ij}(x))_{1 \leq j \leq n} $; in other words, one obtains the derivative of a determinant of order $ n $ by taking the sum of the $ n $ determinants formed by replacing, for each $ i $, the terms of the $ i^{th} $ column by their derivatives.

#### Remark {#fvr-i-s1-n3-rem-1 .statement}

If $ U(x) $ is a square matrix which is differentiable and invertible at the point $ x_0 $, then the derivative of its determinant $ \Delta(x) = \det(U(x)) $ can be expressed through the derivative of $ U(x) $ by the formula
$$
\Delta'(x_0) = \Delta(x_0) \cdot \operatorname{Tr}(U'(x_0) U^{-1}(x_0)).
$$
Indeed, let us put $ U(x_0 + h) = U(x_0) + h V $; then, by definition, $ V $ tends to $ U'(x_0) $ when $ h $ tends to 0. One can write
$$
\Delta(x_0 + h) = \Delta(x_0) \cdot \det(I + h V U^{-1}(x_0)).
$$
Now $ \det(I + h X) = 1 + h \operatorname{Tr}(X) + \sum_{k=2}^n \lambda_k h^k $, the $ \lambda_k $ ($ k \geq 2 $) being polynomials in the elements of the matrix $ X $; since the elements of $ V U^{-1}(x_0) $ have a limit when $ h $ tends to 0, we indeed obtain the formula (3).

### 4. DERIVATIVE OF THE INVERSE OF A FUNCTION

#### Proposition 4 {#fvr-i-s1-prop-4 .statement}

*Let E be a complete normed algebra with a unit element over $ \mathbf{R} $ and let $ \mathbf{f} $ be a function defined on an interval $ I \subset \mathbf{R} $, taking values in E, and differentiable at the point $ x_0 \in I $. If $ y_0 = \mathbf{f}(x_0) $ is invertible $ ^2 $ in E, then the function $ x \mapsto (\mathbf{f}(x))^{-1} $ is defined on a neighbourhood of $ x_0 $ (relative to I), and has a derivative equal to $ -(\mathbf{f}(x_0))^{-1} \mathbf{f}'(x_0) (\mathbf{f}(x_0))^{-1} $ at $ x_0 $.*

Indeed, the set of invertible elements in E is an open set on which the function $ y \mapsto y^{-1} $ is continuous (*Gen. Top.*, IX, p. 178); since $ \mathbf{f} $ is continuous (relative to I) at $ x_0 $, $ (\mathbf{f}(x))^{-1} $ is defined on a neighbourhood of $ x_0 $, and we have
$$
(\mathbf{f}(x))^{-1} - (\mathbf{f}(x_0))^{-1} = (\mathbf{f}(x))^{-1} \left( \mathbf{f}(x_0) - \mathbf{f}(x) \right) (\mathbf{f}(x_0))^{-1}.
$$
The proposition thus follows from the continuity of $ y^{-1} $ on a neighbourhood of $ y_0 $ and the continuity of $ xy $ on $ E \times E $.

$ ^2 $ Recall from (*Alg.*, I, p. 15) that an element $ z \in E $ is said to be *invertible* if there exists an element of $ E $, denoted by $ z^{-1} $, such that $ zz^{-1} = z^{-1}z = e $ (e being the unit element of $ E $).

#### Example 1 {#fvr-i-s1-n4-exa-1 .statement}

The most important particular case is that where E is one of the fields $ \mathbf{R} $ or $ \mathbf{C} $: if $ f $ is a function with real or complex values, differentiable at the point $ x_0 $, and such that $ f(x_0) \neq 0 $, then $ 1/f $ has derivative equal to $ -f'(x_0)/(f(x_0))^2 $ at $ x_0 $.

#### Example 2 {#fvr-i-s1-n4-exa-2 .statement}

If $ U = (\alpha_{ij}(x)) $ is a square matrix of order $ n $, differentiable at $ x_0 $ and invertible at this point, then $ U^{-1} $ has derivative equal to $ -U^{-1} U' U^{-1} $ at $ x_0 $.

### 5. DERIVATIVE OF A COMPOSITE FUNCTION

#### Proposition 5 {#fvr-i-s1-prop-5 .statement}

*Let $ f $ be a real function defined on an interval $ I \subset \mathbf{R} $, and $ g $ a vector function defined on an interval of $ \mathbf{R} $ containing $ f(I) $. If $ f $ is differentiable at the point $ x_0 $ and $ g $ is differentiable at the point $ f(x_0) $ then the composite function $ g \circ f $ has a derivative equal to $ g'(f(x_0)) f'(x_0) $ at $ x_0 $.*

Let us put $ h = g \circ f $; for $ x \neq x_0 $ we can write
$$
\frac{h(x) - h(x_0)}{x - x_0} = u(x) \frac{f(x) - f(x_0)}{x - x_0}
$$
where we set $ u(x) = \frac{g(f(x)) - g(f(x_0))}{f(x) - f(x_0)} $ if $ f(x) \neq f(x_0) $, and $ u(x) = g'(f(x_0)) $ otherwise. Now $ f(x) $ has limit $ f(x_0) $ when $ x $ tends to $ x_0 $, so $ u(x) $ has limit $ g'(f(x_0)) $, from which the proposition follows in view of the continuity of the function $ yx $ on $ E \times \mathbf{R} $.

### 6. DERIVATIVE OF AN INVERSE FUNCTION

#### Proposition 6 {#fvr-i-s1-prop-6 .statement}

*Let $ f $ be a homeomorphism of an interval $ I \subset \mathbf{R} $ onto an interval $ J = f(I) \subset \mathbf{R} $, and let $ g $ be the inverse homeomorphism$ ^3 $. If $ f $ is differentiable at the point $ x_0 \in I $, and if $ f'(x_0) \neq 0 $, then $ g $ has a derivative equal to $ 1/f'(x_0) $ at $ y_0 = f(x_0) $.*

For each $ y \in J $ we have $ g(y) \in I $ and $ u = f(g(y)) $; we thus can write
$$
\frac{g(y) - g(y_0)}{y - y_0} = \frac{g(y) - x_0}{f(g(y)) - f(x_0)}
$$
for $ y \neq y_0 $. When $ y $ tends to $ y_0 $ while remaining in $ J $ and $ \neq y_0 $, then $ g(y) $ tends to $ x_0 $ remaining in $ I $ and $ \neq x_0 $, and the right-hand side in the preceding formula thus has limit $ 1/f'(x_0) $, since by hypothesis $ f'(x_0) \neq 0 $.

#### Corollary {#fvr-i-s1-n6-cor-1 .statement}

*If $ f $ is differentiable on $ I $ and if $ f'(x) \neq 0 $ on $ I $, then $ g $ is differentiable on $ J $ and its derivative at each point $ y \in J $ is $ 1/f'(g(y)) $.*

For example, for each integer $ n > 0 $, the function $ x^{1/n} $ is a homeomorphism of $ \mathbf{R}_+ $ onto itself, is the inverse of $ x^n $, and has derivative $ \frac{1}{n} x^{\frac{1}{n} - 1} $ at each $ x > 0 $.

One deduces easily, from prop. 5, that for every rational number $ r = p/q > 0 $ the function $ x^r = (x^{1/q})^p $ has derivative $ rx'^{-1} $ at every $ x > 0 $.

$ ^3 $ For $ f $ to be a homeomorphism of $ I $ onto a subset of $ \mathbf{R} $ we know that it is necessary and sufficient that $ f $ be continuous and strictly monotone on $ I $ (*Gen. Top.*, IV, p. 338, th. 5).

#### Remark 1 {#fvr-i-s1-n6-rem-1 .statement}

All the preceding propositions, stated for functions differentiable at a point $ x_0 $, immediately yield propositions for functions which are right (resp. left) differentiable at $ x_0 $, when, instead of the functions themselves, one considers their restrictions to the intersection of their intervals of definition with the interval $[x_0, +\infty[$ (resp. ]$ -\infty, x_0 $]); we leave it to the reader to state them.

#### Remark 2 {#fvr-i-s1-n6-rem-2 .statement}

The preceding definitions and propositions (except for those concerning right and left derivatives) extend easily to the case where one replaces $ \mathbf{R} $ by an arbitrary *commutative non-discrete topological field* $ K $, and the topological vector spaces (resp. topological algebras) over $ \mathbf{R} $ by topological vector spaces (resp. topological algebras) over $ K $. In def. 1 and props. 1, 2 and 3 it is enough to replace I by a *neighbourhood* of $ x_0 $ in $ K $; in prop. 4 one must assume further that the map $ y \mapsto y' $ is defined and continuous on a neighbourhood of $ f(x_0) $ in E. Prop. 5 generalizes in the following manner: let $ K' $ be a non-discrete subfield of the topological field $ K $, let E be a topological vector space *over* $ K $; let $ f $ be a function defined on a neighbourhood $ V \subset K' $ of $ x_0 \in K' $, with values in $ K $ (considered as a topological vector space over $ K' $), differentiable at $ x_0 $, and let g be a function defined on a neighbourhood of $ f(x_0) \in K $, with values in E, and differentiable at the point $ f(x_0) $; then the map $ g \circ f $ is differentiable at $ x_0 $ and has derivative $ g'(f(x_0))f'(x_0) $ there (E being then considered as a topological vector space *over* $ K' $).

With the same notation, let $ f $ be a function defined on a neighbourhood V of $ a \in K $, with values in E, and differentiable at the point $ a $; if $ a \in K' $, then the *restriction* of $ f $ to $ V \cap K' $ is differentiable at $ a $, and has derivative $ f'(a) $ there. These considerations apply above all, in practice, to the case where $ K = \mathbf{C} $ and $ K' = \mathbf{R} $.

Finally, prop. 6 extends to the case where one replaces I by a neighbourhood of $ x_0 \in K $, and $ f $ by a homeomorphism of I onto a neighbourhood $ J = f(I) $ of $ y_0 = f(x_0) $ in $ K $.

### 7. DERIVATIVES OF REAL-VALUED FUNCTIONS

The preceding definitions and propositions may be augmented in several respects when we deal with *real-valued* functions of a real variable.

In the first place, if $ f $ is such a function, defined on an interval $ I \subset \mathbf{R} $, and continuous relative to I at a point $ x_0 \in I $, it can happen that when $ x $ tends to $ x_0 $ while remaining in I and $ \neq x_0 $, that $ \frac{f(x) - f(x_0)}{x - x_0} $ has a limit equal to $ +\infty $ or to $ -\infty $; one then says that $ f $ is differentiable at $ x_0 $ and has derivative $ +\infty $ (resp. $ -\infty $) there; if the function $ f $ has a derivative $ f'(x) $ (finite or infinite) at every point $ x $ of I, then the function $ f' $ (with values in $ \overline{\mathbf{R}} $) is again called the derived function (or simply the derivative) of $ f $. One generalizes the definitions of right and left derivative similarly.

#### Example {#fvr-i-s1-n7-exa-1 .statement}

At the point $ x = 0 $ the function $ x^{1/3} $ (the inverse function of $ x^3 $, a homeomorphism of $ \mathbf{R} $ onto itself) has a derivative, equal to $ +\infty $; at $ x = 0 $ the function $ |x|^{1/3} $ has right derivative $ +\infty $ and left derivative $ -\infty $.

The formulae for the derivative of a sum, of a product of differentiable real functions, and for the inverse of a differentiable function (props. 1, 3 and 4), as well as for the derivative of a (real-valued) composition of functions (prop. 5) remain valid when the derivatives that occur are infinite, so long as all the expressions that occur in these formulae make sense (*Gen Top.*, IV, p. 345–346). In fact, if in prop. 6 one supposes that $ f $ is strictly increasing (resp. strictly decreasing) and continuous on I, and if $ f'(x_0) = 0 $, then the inverse function $ g $ has a derivative equal to $ +\infty $ (resp. $ -\infty $) at the point $ y_0 = f(x_0) $; if $ f'(x_0) = +\infty $ (resp. $ -\infty $), then $ g $ has derivative 0. There are similar results for right and left derivatives, which we leave to the care of the reader.

Let C be the graph or representing curve of a finite real function $ f $, the subset of the plane $ \mathbf{R}^2 $ formed by the points $ (x, f(x)) $ where $ x $ runs through the set where $ f $ is defined. If the function $ f $ has a finite right derivative at a point $ x_0 \in I $, then the half-line with origin at the point $ M_{x_0} = (x_0, f(x_0)) $ of C, and direction numbers $ (1, f'_d(x_0)) $ is called the right half-tangent to the curve C at the point $ M_{x_0} $; when $ f'_d(x_0) = +\infty $ (resp. $ f'_d(x_0) = -\infty $) we use the same terminology for the half-line with origin $ M_{x_0} $ and direction numbers $ (0, 1) $ (resp. $ (0, -1) $). In the same way one defines the left half-tangent at $ M_{x_0} $ when $ f'_g(x_0) $ exists. With these definitions one can verify quickly that the angle which the right (resp. left) half-tangent makes with the abscissa is the limit of the angle made by this axis with the half-line originating at $ M_{x_0} $ and passing through the point $ M_1 = (x, f(x)) $ of C, as $ x $ tends to $ x_0 $ while remaining $ > x_0 $ (resp. $ < x_0 $).

One can also say that the right (resp. left) half-tangent is the limit of the half-line originating at $ M_{x_0} $ passing through $ M_1 $, on endowing the set of half-lines having the same origin with the quotient space topology $ C^*/\mathbf{R}_+^* $ (Gen. Top., VIII, p. 107).

If the two half-tangents exist at a point $ M_{x_0} $ of C, they are in opposite directions only when $ f $ has a derivative (finite or not) at the point $ x_0 $ (assumed interior to I); they are identical only when $ f'_d(x_0) $ and $ f'_g(x_0) $ are infinite and of opposite sign. In these two cases we say that the line containing these two half-tangents is the tangent to C at the point $ M_{x_0} $.

When the tangent at $ M_{x_0} $ exists it is the limit of the line passing through $ M_{x_0} $ and $ M_1 $ as $ x $ tends to $ x_0 $ remaining $ \neq x_0 $, the topology on the set of lines which pass through a given fixed point being that of the quotient space $ C^*/\mathbf{R}^* $ (Gen. Top., VIII, p. 114).

The concepts of tangent and half-tangent to a graph are particular cases of general concepts which will be defined in the part of this Series devoted to differentiable varieties.

#### Definition 4 {#fvr-i-s1-def-4 .statement}

We say that a real function $ f $, defined on a subset A of a topological space E, has a relative maximum (resp. strict relative maximum, relative minimum, strict relative minimum) at a point $ x_0 \in A $, relative to A, if there is a neighbourhood $ V $ of $ x_0 $ in E such that at every point $ x \in V \cap A $ distinct from $ x_0 $ one has $ f(x) \leq f(x_0) $ (resp. $ f(x) < f(x_0) $, $ f(x) \geq f(x_0) $, $ f(x) > f(x_0) $).

It is clear that if $ f $ attains its least upper bound (resp. greatest lower bound) over A at a point of A, then it has a relative maximum (resp. relative minimum) relative to A at this point; the converse is of course incorrect.

Note that if $ B \subset A $, and if $ f $ admits (for example) a relative maximum at a point $ x_0 \in B $ relative to B, then $ f $ does not necessarily have a relative maximum relative to A at this point.

#### Proposition 7 {#fvr-i-s1-prop-7 .statement}

Let $ f $ be a finite real function, defined on an interval $ I \subset \mathbf{R} $. If $ f $ admits a relative maximum (resp. relative minimum) at a point $ x_0 $ interior to I, and has both right and left derivatives at this point, then one has $ f'_d(x_0) \leq 0 $ and $ f'_g(x_0) \geq 0 $ (resp. $ f'_d(x_0) \geq 0 $ and $ f'_g(x_0) \leq 0 $); in particular, if $ f $ is differentiable at the point $ x_0 $, then $ f'(x_0) = 0 $.

The proposition follows trivially from the definitions.

We can say further that if at a point $ x_0 $ interior to I the function $ f $ is differentiable and admits a relative maximum or minimum, then the tangent to its graph is parallel to the abscissa. The converse is incorrect, as is shown by the example of the function $ x^3 $ which has zero derivative at the point $ x = 0 $, but has neither relative maximum nor minimum at this point.

### Exercises {#fvr-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
