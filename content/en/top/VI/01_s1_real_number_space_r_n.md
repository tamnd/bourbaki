---
book: top
book_title: General Topology
chapter: VI
chapter_title: Real number spaces and projective spaces
section: 1
section_title: Real number space R^n
lang: en
source: top-v-x
pdf_pages: 0037-0044, 0061-0064
extraction: ocr
subsections:
    - "no": 1
      title: THE TOPOLOGY OF $ \mathbf{R}^n $
      page: 0
      pdf_page: 37
    - "no": 2
      title: THE ADDITIVE GROUP $ \mathbf{R}^n $
      page: 0
      pdf_page: 38
    - "no": 3
      title: THE VECTOR SPACE $ \mathbf{R}^n $
      page: 0
      pdf_page: 39
    - "no": 4
      title: AFFINE LINEAR VARIETIES IN $ \mathbf{R}^n $
      page: 0
      pdf_page: 40
    - "no": 5
      title: TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $ \mathbf{R} $
      page: 0
      pdf_page: 42
    - "no": 6
      title: TOPOLOGY OF MATRIX SPACES OVER $ \mathbf{R} $
      page: 0
      pdf_page: 43
statements: 11
exercises: 13
content_sha256: 5bba573e293af8b560db22f347efd7b4b37736326fa655b3237cc560cc32b87f
---

## 1. REAL NUMBER SPACE $ \mathbf{R}^n $

### 1. THE TOPOLOGY OF $ \mathbf{R}^n $

#### Definition 1 {#top-vi-s1-def-1 .statement}

*The topological product of n spaces identical with the real line is called real number space of n dimensions, and is denoted by $ \mathbf{R}^n $.*

#### Remark {#top-vi-s1-n1-rem-1 .statement}

The space $ \mathbf{R}^0 $ consists of a single point.

From *Set Theory*, Chapter III, § 6, no. 3, Theorem 2, Corollary I, we know that, if E is an infinite set, $ E^n $ is equipotent with E for all integers $ n > 0 $; hence, if $ n > 0 $, $ \mathbf{R}^n $ is equipotent with $ \mathbf{R} $, that is, $ \mathbf{R}^n $ *has the power of the continuum* (cf. Exercises 1 and 2).

#### Definition 2 {#top-vi-s1-def-2 .statement}

*Any subset of $ \mathbf{R}^n $ which is the product of n open (resp. closed) intervals of $ \mathbf{R} $ is called an open (resp. closed) box in $ \mathbf{R}^n $. [For $ n = 2 $ it is called an open (resp. closed) rectangle.]*

The open boxes in $ \mathbf{R}^n $ form a *base* of the topology of $ \mathbf{R}^n $ (Chapter I, § 4, no. 1); the open boxes which contain a point $ x = (x_i)_{1 \leq i \leq n} $ of $ \mathbf{R}^n $ form a fundamental system of neighbourhoods of $ x $, and so do the closed boxes of $ \mathbf{R}^n $ for which $ x $ is an interior point.

Every non-empty open box in $ \mathbf{R}^n $ is *homeomorphic* to $ \mathbf{R}^n $ (Chapter IV, § 4, no. 1, Proposition 1).

It follows that, when $ n \geq 1 $, every non-empty open set in $ \mathbf{R}^n $ has the power of the continuum.

An *open* (resp. *closed*) *cube* of $ \mathbf{R}^n $ is an open (resp. closed) box which is the product of $ n $ *bounded intervals of equal length* [for $ n = 2 $, it is called an open (resp. closed) square]; the common length of these intervals is called the side (or side-length) of the cube. The open cubes

$$
K_m = \prod_{1 \leq i \leq n} \left[ x_i - \frac{1}{m}, x_i + \frac{1}{m} \right]
$$

form a countable fundamental system of neighbourhoods of the point $ x = (x_i) $, as $ m $ runs through the set of all integers $ > 0 $ or through any sequence of integers increasing to infinity.

Every open (or closed) box in $ \mathbf{R}^n $ is connected (Chapter I, § 11, no. 4, Proposition 8); in particular, $ \mathbf{R}^n $ is connected and locally connected.

If $ A $ is a non-empty open set in $ \mathbf{R}^n $, its components are therefore open sets (Chapter I, § 11, no. 6, Proposition 11); and the set of these components is countable, for $ \mathbf{R}^n $ has a countable dense subset (for example $ \mathbf{Q}^n $).

Consider under what conditions a subset $ A $ of $ \mathbf{R}^n $ will be relatively compact. By Tychonoff’s theorem (Chapter I, § 9, no. 5, Theorem 3) it is necessary and sufficient that the projections of $ A $ on the factors of $ \mathbf{R}^n $ should be relatively compact; by the Borel-Lebesgue theorem (Chapter IV, § 2, no. 2, Theorem 2) this is equivalent to saying that these projections are bounded subsets of $ \mathbf{R} $. We say that a subset $ A $ of $ \mathbf{R}^n $ is bounded if all its projections are bounded subsets of $ \mathbf{R} $; thus we have proved:

#### Proposition 1 {#top-vi-s1-prop-1 .statement}

A subset $ A $ of $ \mathbf{R}^n $ is relatively compact if and only if it is bounded.

#### Corollary {#top-vi-s1-n1-cor-1 .statement}

The space $ \mathbf{R}^n $ is locally compact, but is not compact if $ n \geq 1 $.

### 2. THE ADDITIVE GROUP $ \mathbf{R}^n $

The set $ \mathbf{R}^n $, endowed with the group structure which is the product of the additive group structures of the $ n $ factors of $ \mathbf{R}^n $, is an abelian group; we use the additive notation, the sum of $ x = (x_i) $ and $ y = (y_i) $ being therefore $ x + y = (x_i + y_i) $. The topology of the number space is compatible with this group structure; endowed with these two structures, $ \mathbf{R}^n $ is a topological group called the *additive group of n-dimensional real number space*. If $ n = 0 $, we make the convention that $ \mathbf{R}^0 $ denotes a group consisting only of the identity element.

The uniform structure of this group, called the *additive uniformity* of $ \mathbf{R}^n $, is the product of the uniformities of the factors of $ \mathbf{R}^n $ (Chapter III, § 3, no. 2). If, for each integer $ p > 0 $, $ V_p $ denotes the set of pairs $ (x, y) $ of $ \mathbf{R}^n $ such that $ \max_{1 \leq i \leq n} |x_i - y_i| \leq 1/p $, the sets $ V_p $ form a *fundamental*

### 3. THE VECTOR SPACE $ \mathbf{R}^n $

Since $ \mathbf{R} $ is a field, we can define on $ \mathbf{R}^n $ a vector space structure over the field $ \mathbf{R} $, the product $ t x $ of a scalar $ t \in \mathbf{R} $ and a point (or vector) $ x = (x_i) $ of $ \mathbf{R}^n $ being the point $ (t x_i) $. Note that the homothety $ (t, x) \to t x $ is continuous on $ \mathbf{R} \times \mathbf{R}^n $. If $ e_i $ denotes the vector of $ \mathbf{R}^n $ all of whose coordinates are zero, except for that of index $ i $, which is equal to 1, then the $ e_i $ form a basis of the vector space $ \mathbf{R}^n $, called the canonical basis of this space. Every vector $ x = (x_i) \in \mathbf{R}^n $ can be written as $ x = \sum_{i=1}^n x_i e_i $, and the relation $ \sum_{i=1}^n t_i e_i = 0 $ implies that $ t_i = 0 $ for $ 1 \leq i \leq n $.

The vector space $ \mathbf{R}^n $ is therefore of dimension $ n $ over the field $ \mathbf{R} $, in the sense of algebra (Algebra, Chapter II, § 7, no. 2); hence its name of $ n $-dimensional real number space.

Let $ f $ be an affine mapping of the vector space $ \mathbf{R}^n $ into the vector space $ \mathbf{R}^m $ ($ m $ and $ n $ being integers > 0). If we put $ g(x) = f(x) - f(0) $, $ g $ is a linear mapping of $ \mathbf{R}^n $ into $ \mathbf{R}^m $. Let $ a_{ij} $ ($ 1 \leq j \leq m $) be the coordinates of $ g(e_i) $ in $ \mathbf{R}^m $ and let $ b_j $ ($ 1 \leq j \leq m $) be those of $ f(0) $; if $ x_i $ ($ 1 \leq i \leq n $) is the $ i $th coordinate of $ x \in \mathbf{R}^n $ and if $ y_j $ is the $ j $th coordinate of $ y = f(x) $, we have

$$
y_j = \sum_{i=1}^n a_{ij} x_i + b_j \quad (1 \leq j \leq m).
$$

Since every linear polynomial in $ x_1, x_2, \ldots, x_n $ is uniformly continuous on $ \mathbf{R}^n $, it follows that every affine mapping of $ \mathbf{R}^n $ into $ \mathbf{R}^m $ is uniformly continuous on $ \mathbf{R}^n $ (Chapter II, § 2, no. 6, Proposition 7).

In particular, we know that every affine mapping of $ \mathbf{R}^n $ onto itself is bijective and that its inverse is again an affine mapping; hence every affine mapping of $ \mathbf{R}^n $ onto itself is a homeomorphism (and an automorphism of the uniform structure of $ \mathbf{R}^n $).

Let $ (a_i)_{1 \leq i \leq n} $ be a free system of $ n $ vectors of $ \mathbf{R}^n $ [in other words a basis of the vector space $ \mathbf{R}^n $]; if $ b $ is any point of $ \mathbf{R}^n $, the set P of points $ x = b + \sum_{i=1}^{n} u_i a_i $ such that $ -1 \leq u_i \leq 1 $ for $ 1 \leq i \leq n $ is a compact neighbourhood of $ b $; for there exists a bijective affine mapping $ f $ of $ \mathbf{R}^n $ onto itself such that $ f(b) = 0, f(b + a_i) = e_i $ for $ 1 \leq i \leq n $; and $ f(P) $ is the cube which is the product of the $ n $ intervals $[ -1, +1 ]$ in the $ n $ factor spaces. $ P $ is called the closed parallelootope with centre $ b $ and basis vectors $ a_i $. The interior of $ P $ consists of the points $ b + \sum_{i=1}^{n} u_i a_i $ such that $ -1 < u_i < 1 $ for $ 1 \leq i \leq n $; it is called the open parallelootope with centre $ b $ and basis vectors $ a_i $.

### 4. AFFINE LINEAR VARIETIES IN $ \mathbf{R}^n $

Given a $ p $-dimensional affine linear variety $ V $ in $ \mathbf{R}^n $, there exists an affine mapping $ f $ of $ \mathbf{R}^n $ onto itself which transforms $ V $ into a $ p $-dimensional coordinate variety, that is to say a vector subspace $ V' $ generated by $ p $ of the vectors of the canonical basis $ (e_i) $ of $ \mathbf{R}^n $. There exists a mapping of $ V' $ onto $ \mathbf{R}^p $ which is an isomorphism of the vector space structure and the topology of $ V' $ onto the corresponding structures of $ \mathbf{R}^p $ (it is moreover often convenient to identify $ \mathbf{R}^p $ with such a coordinate variety $ V' $, e.g., with the vector subspace generated by $ e_1, e_2, \ldots, e_p $). In addition, $ V' $ is a closed subset of $ \mathbf{R}^n $ (Chapter I, § 4, no. 3, Corollary to Proposition 7); hence:

#### Proposition 2 {#top-vi-s1-prop-2 .statement}

*Every $ p $-dimensional linear affine variety in $ \mathbf{R}^n $ is a closed subset of $ \mathbf{R}^n $, homeomorphic to $ \mathbf{R}^p $.*

It is this result which is the origin of the names *line* and *plane* given to affine linear varieties of *one* and *two* dimensions in a vector space over an arbitrary division ring. We recall also that, for $ n \geq 1 $, the affine linear varieties of $ n - 1 $ dimensions of $ \mathbf{R}^n $ are called *hyperplanes* (*loc. cit.*).

The $ n $ one-dimensional coordinate varieties, that is to say the $ n $ lines passing through $ 0 $ and the $ n $ points $ e_i $ respectively, are called the *coordinate axes*. For $ n = 2 $ the axis through $ e_1 $ is sometimes called the *axis of abscissas* and the axis through $ e_2 $ is called the *axis of ordinates*; the first coordinate of a point $ x \in \mathbf{R}^2 $ is called its *abscissa*, the second coordinate its *ordinate*.

Every line $ D $ passing through a point $ a $ has a parametric representation $ t \to a + tb $, where $ t $ runs through $ \mathbf{R} $ and $ b \neq 0 $; this mapping is a homeomorphism of $ \mathbf{R} $ onto $ D $. The vector $ b $ is called a *direction* vector of D, and its components $ b_i (1 \leq i \leq n) $ are called direction ratios of D. If $ b' $ is another direction vector of D, there exists $ h \neq 0 $ in $ \mathbf{R} $ such that $ b' = hb $.

The set of points $ a + tb $, where $ t $ runs through the set of real numbers $ \geq 0 $, is called the closed ray (or simply ray, or half-line) with origin $ a $ and direction vector $ b $ (or with direction ratios $ b_i $). It is a closed subset of $ \mathbf{R}^n $, homeomorphic to the interval $[0, +\infty[$ of $ \mathbf{R} $, and therefore connected. The line D is the union of the two rays with origin $ a $ and direction vectors $ b $ and $ -b $ respectively; these rays are said to be opposite.

By abuse of language, the set of points $ a + tb $, where $ t $ runs through the set of real numbers $ > 0 $, is called the open ray with origin $ a $ and direction vector $ b $; it is homeomorphic to the interval ]$0, +\infty[$ (and therefore homeomorphic to $ \mathbf{R} $), but is not open in $ \mathbf{R}^n $ if $ n > 1 $, although it is open in the line which contains it.

A line passing through two distinct points $ x $ and $ y $ also has a parametric representation $(u, v) \to ux + vy$, where $(u, v)$ runs through the set of pairs of real numbers such that $ u + v = 1 $. Given any two points $ x, y $ (distinct or not) the set of points $ ux + uy $, where $(u, v)$ runs through the set of pairs of real numbers such that $ u \geq 0, v \geq 0 $ and $ u + v = 1 $, is called the closed segment (or simply segment) with end-points $ x, y $. A closed segment is compact and connected, for if its end-points are distinct it is homeomorphic to the interval $[0, 1]$ of $ \mathbf{R} $.

If $ x \neq y $, the set of points $ ux + vy $ such that $ u > 0, v > 0 $ and $ u + v = 1 $ is called (by abuse of language) the open segment with end-points $ x, y $; it is homeomorphic to the open interval ]$0, 1[$ (and hence also homeomorphic to $ \mathbf{R} $). Finally the union of $ \{y\} $ and the open segment with end-points $ x, y $ is sometimes called the segment open at $ x $ and closed at $ y $; it is homeomorphic to the interval $[0, 1[$. All the segments with $ x $ and $ y $ as end-points are connected, and the closure of each of them is the closed segment with the same end-points.

#### Proposition 3 {#top-vi-s1-prop-3 .statement}

*Let $ f(x) = f(x_1, x_2, \ldots, x_n) $ be a polynomial with real coefficients, not identically zero, defined on $ \mathbf{R}^n $. Then the complement of the set $ \overline{f}(0) $ is dense in $ \mathbf{R}^n $.*

Let $ x $ be any point of $ \mathbf{R}^n $ and let $ y \in \mathbf{R}^n $ be such that $ f(y) \neq 0 $; $ \varphi(t) = f(x + t(y - x)) $ is a polynomial in the real variable $ t $, not identically zero; hence there exist arbitrarily small values of $ t $ such that $ \varphi(t) \neq 0 $. This shows that $ x $ lies in the closure of the complement of $ \overline{f}(0) $.

#### Corollary {#top-vi-s1-n4-cor-1 .statement}

*The complement of an affine linear variety of dimension $ p < n $ is dense in $ \mathbf{R}^n $.*

Since every affine linear variety of dimension $ p < n $ is contained in a hyperplane, it is enough to prove the corollary for a hyperplane; but a hyperplane is defined by an equation $ g(x) = 0 $, where $ g $ is a linear polynomial not identically zero.

#### Proposition 4 {#top-vi-s1-prop-4 .statement}

*In $ \mathbf{R}^n $ ($ n \geq 1 $) the complement of every hyperplane has two connected components.*

Let $ g(x) = 0 $ be an equation of a hyperplane $ H $ in $ \mathbf{R}^n $, $ g $ being a linear polynomial. The set $ CH $ is the union of the set $ E_1 $ of all points $ x $ such that $ g(x) > 0 $ and the set $ E_2 $ of all points $ x $ such that $ g(x) < 0 $. $ E_1 $ and $ E_2 $ are connected, for if $ g(x) > 0 $ and $ g(y) > 0 $ we have $ g(ux + vy) = ug(x) + vg(y) > 0 $ whenever $ u \geq 0, v \geq 0 $ and $ u + v = 1 $; in other words, the segment with end-points $ x $ and $ y $ is contained in $ E_1 $. Similarly for $ E_2 $. On the other hand, $ CH $ is not connected, because its image in $ \mathbf{R} $ under $ g $ is the union of the intervals ]$ 0, +\infty $ [ and ]$ -\infty, 0 $ [.

The components $ E_1, E_2 $ of the complement of a hyperplane $ H $ are called the *open half-spaces* determined by $ H $.

The closures of $ E_1 $ and $ E_2 $, which are respectively $ E_1 \cup H $ and $ E_2 \cup H $, are called the *closed half-spaces* determined by $ H $.

Observe that an affine mapping of $ \mathbf{R}^n $ onto itself which transforms $ H $ into a "coordinate" hyperplane, e.g., the hyperplane whose equation is $ x_n = 0 $, also transforms the open half-spaces determined by $ H $ into the open half-spaces defined respectively by the relations $ x_n > 0 $ and $ x_n < 0 $; the latter are open boxes and therefore *homeomorphic to* $ \mathbf{R}^n $.

### 5. TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $ \mathbf{R} $

Let $ E $ be a vector space of dimension $ n $ over the field $ \mathbf{R} $; if $ (a_i)_{1 \leq i \leq n} $ is a *basis* of $ E $, then every point $ x \in E $ can be written uniquely in the form $ x = \sum_{i=1}^n x_i a_i $, where the $ x_i $ are real numbers; the mapping $ (x_i) \to \sum_{i=1}^n x_i a_i $ is therefore a bijective linear mapping of $ \mathbf{R}^n $ onto $ E $.

If we *transport* to $ E $ the topology of $ \mathbf{R}^n $ by this mapping, $ E $ is endowed with a topology compatible with its additive group structure, and the mapping $ (t, x) \to tx $ of $ \mathbf{R} \times E $ into $ E $ is continuous with respect to this topology. This topology is *independent of the basis* chosen in $ E $; for if $ (a') $ is another basis of $ E $, and if $ x = \sum_{i=1}^n x'_i a'_i = \sum_{i=1}^n x_i a_i $, the mapping $ (x_i) \to (x'_i) $ of $ \mathbf{R}^n $ onto itself is linear and therefore a homeomorphism.

This fact leads one to suspect that the topology so defined on $ E $ should be capable of characterization without the help of a basis of $ E $. In fact, we shall see later that this is the *only* Hausdorff topology on $ E $ for which the functions $ x - y $ (on $ E \times E $) and $ tx $ (on $ \mathbf{R} \times E $) are continuous.

If now $ A $ is an *algebra* of finite rank $ n $ over the field $ \mathbf{R} $, the above topology on $ A $ (considered as an $ n $-dimensional vector space over $ \mathbf{R} $) is compatible not only with the additive group structure of $ A $, but also with its *ring* structure. This is a consequence of the following more general result:

#### Proposition 5 {#top-vi-s1-prop-5 .statement}

*Let $ E, F, G $ be three finite-dimensional vector spaces over the field $ \mathbf{R} $. Then every bilinear mapping (*) $ f $ of $ E \times F $ into $ G $ is continuous.*

We may suppose that $ E = \mathbf{R}^m, F = \mathbf{R}^n, G = \mathbf{R}^p $; it is enough to show that the coordinates in $ \mathbf{R}^p $ of $ f(x, y) $ are continuous functions of $ (x, y) \in E \times F $ (Chapter I, § 4, no. 1, Proposition 1). In other words, it is enough to show that every *bilinear form* $ g $ is continuous on $ E \times F $; and this is immediate, since $ g(x, y) $ is a polynomial in the coordinates of $ x $ and $ y $.

### 6. TOPOLOGY OF MATRIX SPACES OVER $ \mathbf{R} $

An important example of a vector space over $ \mathbf{R} $ is the space $ \mathbf{M}_{m,n}(\mathbf{R}) $ of *matrices with m rows and n columns* whose elements belong to $ \mathbf{R} $; this is a space of dimension $ mn $ over $ \mathbf{R} $, hence is homeomorphic to $ \mathbf{R}^{mn} $. By Proposition 5 of § 5, the product $ X.Y $ of two matrices $ X \in \mathbf{M}_{m,n}(\mathbf{R}), Y \in \mathbf{M}_{n,p}(\mathbf{R}) $ is a continuous function of $ (X, Y) $. In particular, the topology of the space $ \mathbf{M}_n(\mathbf{R}) $ of square matrices of order $ n $ is compatible with the ring structure on $ \mathbf{M}_n(\mathbf{R}) $. Furthermore:

#### Proposition 6 {#top-vi-s1-prop-6 .statement}

*In the ring $ \mathbf{M}_n(\mathbf{R}) $, the group $ \mathbf{GL}_n(\mathbf{R}) $ of non-singular matrices is a dense open subset, and the topology induced on this set is compatible with its group structure.*

(*) If $ E, F, G $ are three vector spaces over a field $ K $, a mapping $ f $ of $ E \times F $ into $ G $ is said to be *bilinear* if we have identically
$$
f(x + x', y) = f(x, y) + f(x', y), \quad f(x, y + y') = f(x, y) + f(x, y'),
$$
$$
f(\lambda x, y) = f(x, \lambda y) = \lambda f(x, y)
$$
for all $ x, x' \in E $, all $ y, y' \in F $ and all $ \lambda \in K $.

If $ X $ is a nonsingular square matrix, the elements of $ X^{-1} $ are rational functions of the elements of $ X $; these functions are therefore defined and continuous in a neighbourhood of $ X $, so that every matrix $ Y $ in this neighbourhood is non-singular, and the mapping $ Y \to Y^{-1} $ is continuous at the point $ X $; hence $ \mathbf{GL}_n(\mathbf{R}) $ is open in $ \mathbf{M}_n(\mathbf{R}) $ and the topology of $ \mathbf{GL}_n(\mathbf{R}) $ is compatible with its group structure.

Finally, $ \mathbf{GL}_n(\mathbf{R}) $ is the complement of the set of square matrices $ X $ whose determinant is zero; since the determinant of $ X $ is a polynomial in the elements of $ X $, Proposition 3 of no. 4 shows that $ \mathbf{GL}_n(\mathbf{R}) $ is dense in $ \mathbf{M}_n(\mathbf{R}) $.

### Exercises {#top-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
