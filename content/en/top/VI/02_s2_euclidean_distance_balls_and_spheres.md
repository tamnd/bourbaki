---
book: top
book_title: General Topology
chapter: VI
chapter_title: Real number spaces and projective spaces
section: 2
section_title: Euclidean distance, balls and spheres
lang: en
source: top-v-x
pdf_pages: 0044-0050, 0064-0067
extraction: ocr
subsections:
    - "no": 1
      title: EUCLIDEAN DISTANCE IN $ \mathbf{R}^n $
      page: 0
      pdf_page: 44
    - "no": 2
      title: DISPLACEMENTS
      page: 0
      pdf_page: 45
    - "no": 3
      title: EUCLIDEAN BALLS AND SPHERES
      page: 0
      pdf_page: 46
    - "no": 4
      title: STEREOPHIC PROJECTION
      page: 0
      pdf_page: 48
statements: 12
exercises: 13
content_sha256: c079d162d43af341a9f2928c20803b7b5597940eb20b9c983f7ce0bcd9e63c46
---

## 2. EUCLIDEAN DISTANCE; BALLS AND SPHERES

### 1. EUCLIDEAN DISTANCE IN $ \mathbf{R}^n $

In conformity with the general definitions the *Euclidean distance* between two points $ x = (x_i) $ and $ y = (y_i) $ is the number

$$
d(x, y) = \sqrt{\sum_{i=1}^n (x_i - y_i)^2} \geq 0.
$$

We recall its principal properties. The relation $ d(x, y) = 0 $ is equivalent to $ x = y $. We have $ d(x, y) = d(y, x) $; for all scalars $ t \in \mathbf{R} $, $ d(tx, ty) = |t| d(x, y) $; for all $ z \in \mathbf{R}^n $, $ d(x + z, y + z) = d(x, y) $; in other words, the distance between two points is *invariant under translation*. The distance $ d(o, x) $ from the origin $ o $ to a point $ x $ is denoted also by $ \|x\| $ and is called the *Euclidean norm* of $ x $ (or simply the *norm* of $ x $, when there is no likelihood of confusion; cf. Chapter IX, § 3, no. 3). Then $ d(x, y) = \|y - x\| $.

For $ n = 1 $, the Euclidean distance between the points $ x, y $ of $ \mathbf{R} $ reduces to the length $ |y - x| $ of the intervals with $ x $ and $ y $ as end-points. For any $ n $, we say that $ d(x, y) = \|y - x\| $ is the *length* of the segments with $ x $ and $ y $ as end-points.

The Euclidean distance satisfies the *triangle inequality*

(I)
$$
d(x, y) \leq d(x, z) + d(z, y)
$$
for all $ x, y, z $ in $ \mathbf{R}^n $.

We recall that the proof of (I) reduces to that of the inequality

$$
\left( \sum_{i=1}^n (x_i + y_i)^2 \right)^{1/2} \leq \left( \sum_{i=1}^n x_i^2 \right)^{1/2} + \left( \sum_{i=1}^n y_i^2 \right)^{1/2};
$$

this in turn is equivalent to the Cauchy-Schwarz inequality

$$
\left( \sum_{i=1}^n x_i y_i \right)^2 \leq \left( \sum_{i=1}^n x_i^2 \right) \left( \sum_{i=1}^n y_i^2 \right),
$$

which is an immediate consequence of Lagrange’s identity

$$
\left( \sum_{i=1}^n x_i^2 \right) \left( \sum_{i=1}^n y_i^2 \right) - \left( \sum_{i=1}^n x_i y_i \right)^2 = \frac{1}{2} \sum_{i,j} (x_i y_j - x_j y_i)^2.
$$

This proof shows at the same time that the two sides of (1) can be equal only if $ z $ is a point of the segment with $ x $ and $ y $ as end-points.

From (1) we deduce the inequality

$$
d(x, y) \geq |d(x, z) - d(y, z)|.
$$

Finally, if $ x = (x_i), y = (y_i) $, we have

$$
\sup_{1 \leq i \leq n} |x_i - y_i| \leq d(x, y) \leq \sqrt{n} \cdot \sup_{1 \leq i \leq n} |x_i - y_i|.
$$

Hence a subset $ A $ of $ \mathbf{R}^n $ is *bounded* (\S 1, no. 1) if and only if

$$
\sup_{x \in A} \|x\| < +\infty.
$$

### 2. DISPLACEMENTS

We recall again that the affine transformations $ f $ of $ \mathbf{R}^n $ onto itself which leave *invariant* the distance between any two points [that is to say, such that $ d(f(x), f(y)) = d(x, y) $ for all $ x, y $] are called *Euclidean displacements* (or simply *displacements*) (*); they form a group, called the *group of displacements* of $ \mathbf{R}^n $. This group operates transitively on $ \mathbf{R}^n $; more generally, if $ V $ and $ V' $ are any two affine linear varieties of the same dimension in $ \mathbf{R}^n $, there exists a displacement which transforms $ V $ into $ V' $. The displacements which leave the origin fixed, called *orthogonal transformations*, form a subgroup of the group of all displacements. This subgroup is called the *orthogonal group* on $ n $ real variables; the linear mappings which belong to this group are characterized by the fact that they leave invariant the *norm* $ \|x\| $ of every point $ x \in \mathbf{R}^n $, or, equivalently, the *quadratic*

(*) If $ f $ is subjected only to the condition $ d(f(x), f(y)) = d(x, y) $ for all $ x, y $, then in fact $ f $ must be affine and linear, and therefore a displacement.

form $ \|x\|^2 = \sum_{i=1}^n x_i^2 $. The scalar product of two vectors $ x = (x_i) $ and $ y = (y_i) $ of $ \mathbf{R}^n $ is the value $ \sum_{i=1}^n x_i y_i $ of the bilinear form associated with the quadratic form $ \sum_{i=1}^n x_i^2 $; it is denoted by $ (x|y) $, or simply by $ xy $ if there is no likelihood of confusion. Every orthogonal transformation leaves invariant the scalar product of any two vectors. Two vectors $ x, y $ are said to be orthogonal if $ (x|y) = 0 $; two vector subspaces $ V, V' $ of $ \mathbf{R}^n $ are said to be orthogonal if each $ x \in V $ is orthogonal to each $ y \in V' $; and two affine linear varieties $ P, P' $ are said to be orthogonal if the vector subspaces parallel respectively to $ P $ and $ P' $ are orthogonal.

### 3. EUCLIDEAN BALLS AND SPHERES

For each integer $ p > 0 $, let $ U_p $ denote the set of all pairs $ (x, y) $ of points of $ \mathbf{R}^n $ such that $ d(x, y) < 1/p $; the inequalities (3) show that the sets $ U_p $ form a fundamental system of entourages of the uniformity of $ \mathbf{R}^n $ (cf. Chapter IX, § 2).

From this fact and from the inequality
$$
|d(x, y) - d(x', y')| \leq d(x, x') + d(y, y'),
$$
which is a consequence of (1), we infer that $ d(x, y) $ is uniformly continuous on $ \mathbf{R}^n \times \mathbf{R}^n $; consequently the norm $ \|x\| = d(0, x) $ is uniformly continuous on $ \mathbf{R}^n $.

#### Definition 1 {#top-vi-s2-def-1 .statement}

Given a point $ x_0 \in \mathbf{R}^n $ and a real number $ r > 0 $, the open (resp. closed) Euclidean ball of $ n $ dimensions with centre $ x_0 $ and radius $ r $ is the set of all points $ x \in \mathbf{R}^n $ such that $ d(x_0, x) < r $ [resp. $ d(x_0, x) \leq r $]; the Euclidean sphere of $ n - 1 $ dimensions with centre $ x_0 $ and radius $ r $ is the set of all $ x \in \mathbf{R}^n $ such that $ d(x_0, x) = r $.

When there is no risk of confusion we say simply "ball" (resp. "sphere") for "Euclidean ball" (resp. "Euclidean sphere"). When $ n = 2 $, a ball of two dimensions is called a disc, and a sphere of one dimension is called a circle. When $ n = 1 $, the open (resp. closed) ball with centre $ x_0 $ and radius $ r $ is the interval $ ]x_0 - r, x_0 + r[ $ (resp. $ [x_0 - r, x_0 + r] $); the sphere with centre $ x_0 $ and radius $ r $ is the set consisting of the two end-points $ x_0 - r, x_0 + r $ of these intervals.

From what has been said, the balls (open or closed) with centre $ x_0 $ (or just those with radii $ 1/p $, where $ p $ runs through the set of integers $ > 0 $) form a fundamental system of neighbourhoods of the point $ x_0 $.

#### Proposition 1 {#top-vi-s2-prop-1 .statement}

Every open (resp. closed) ball of $ \mathbf{R}^n $ is an open (resp. compact) set. The closure of an open ball is the closed ball with the same centre and the same radius; the interior of a closed ball is the open ball with the same centre and the same radius.

The open (resp. closed) ball with centre $ x_0 $ and radius $ r $ is the inverse image of the interval ]$-\infty, r[$ (resp. ]$-\infty, r]$) under the continuous function $ d(x_0, x) $; it is therefore open (resp. closed and bounded, hence compact). If $ d(x_0, x) = r $, and if $ y = x_0 + t(x - x_0) $ ($ 0 < t < 1 $) is a point of the open segment with end-points $ x_0 $ and $ x $, we have $ d(x_0, y) = tr < r $, and $ d(x, y) = (1 - t)r $ is as small as we please; hence $ x $ lies in the closure of the open ball with centre $ x_0 $ and radius $ r $. Again, if $ z = x + t(x - x_0) $ ($ t > 0 $) is a point of the open ray with origin $ x $ and direction vector $ x - x_0 $, we have
$$
d(x_0, z) = (1 + t)r > r,
$$
and $ d(x, z) = tr $ is as small as we please; hence $ x $ is not an interior point of the closed ball with centre $ x_0 $ and radius $ r $.

#### Corollary {#top-vi-s2-n3-cor-1 .statement}

Every Euclidean sphere is a compact set and is the frontier of the open and closed balls with the same centre and the same radius.

The mapping $ x \to \frac{1}{r}(x - x_0) $ transforms the sphere (resp. open ball, closed ball) with centre $ x_0 $ and radius $ r $ into the sphere (resp. open ball, closed ball) with centre $ o $ and radius $ 1 $; this sphere is denoted by $ S_{n-1} $ and is called the unit sphere in $ \mathbf{R}^n $. Likewise, the closed ball with centre $ o $ and radius $ 1 $ is denoted by $ B_n $ and is called the unit ball in $ \mathbf{R}^n $. The topological study of a sphere of $ (n - 1) $ dimensions (resp. a closed ball of $ n $ dimensions) is thus reduced to that of $ S_{n-1} $ (resp. $ B_n $). For the open balls, we have the following proposition:

#### Proposition 2 {#top-vi-s2-prop-2 .statement}

Every $ n $-dimensional open ball is homeomorphic to $ \mathbf{R}^n $.

For the mapping $ x \to \frac{x}{1 + ||x||} $ is continuous on $ \mathbf{R}^n $ and maps $ \mathbf{R}^n $ onto the open ball with centre $ o $ and radius $ 1 $; moreover, from $ y = \frac{x}{1 + ||x||} $ we deduce $ x = \frac{y}{1 - ||y||} $, so that the mapping is bijective and bicontinuous.

Let $ \mathbf{R}_n^* $ denote the complement of $ o $ in $ \mathbf{R}^n $.

#### Proposition 3 {#top-vi-s2-prop-3 .statement}

The space $ \mathbf{R}_n^* $ is homeomorphic to the product of $ S_{n-1} $ and the space $ \mathbf{R}_+^* $ of real numbers $ > 0 $.

For every point $ x \neq o $ can be written uniquely in the form $ tz $, where $ t > 0 $ and $ ||z|| = 1 $, since $ x = tz $ implies $ t = ||x|| $ and $ z = x/||x|| $. Since $ tz $ is continuous on the product $ \mathbf{R} \times \mathbf{R}^n $ and hence *a fortiori* on $ \mathbf{R}_+^* \times S_{n-1} $, and since $ ||x|| $ and $ \frac{1}{||x||} $ are continuous on $ \mathbf{R}_n^* $, the proposition is proved.

The mapping $ x \to x/||x|| $ is called the *central projection* of $ \mathbf{R}_n^* $ onto $ S_{n-1} $. One defines in the same way the *central projection* of the complement of a point $ a $ onto a sphere with centre $ a $.

#### Corollary 1 {#top-vi-s2-prop-3-cor-1 .statement}

*The sphere* $ S_{n-1} $ *is homeomorphic to the quotient of* $ \mathbf{R}_n^* $ *by the equivalence relation whose classes are the open rays with origin* $ o $.

These classes can also be defined as the *classes of intransitivity*, other than $ \{ o \} $, of the group of homotheties of ratio $ > 0 $.

#### Corollary 2 {#top-vi-s2-prop-3-cor-2 .statement}

*The space* $ \mathbf{R}_n^* $ *is homeomorphic to* $ \mathbf{R} \times S_{n-1} $.

For $ \mathbf{R}_+^* = ]0, +\infty[ $ is homeomorphic to $ \mathbf{R} $ (Chapter IV, § 4, no. 1, Proposition 1).

#### Remark {#top-vi-s2-n3-rem-1 .statement}

These propositions are not peculiar to Euclidean balls, but can be extended to a whole category of compact neighbourhoods of $ o $ in $ \mathbf{R}^n $ (see Exercise 12).

The sets $ S_{n-1} $ and $ B_n $ are evidently invariant under all orthogonal transformations. If $ V $ is a $ p $-dimensional vector subspace in $ \mathbf{R}^n $, there exists an orthogonal transformation which transforms $ V $ into a $ p $-dimensional coordinate variety; hence $ V \cap S_{n-1} $ (resp. $ V \cap B_n $) is homeomorphic to $ S_{p-1} $ (resp. $ B_p $).

### 4. STEREOPHIC PROJECTION

Consider the point $ e_n = (0, \ldots, 0, 1) $ of $ S_{n-1} $, and the hyperplane $ H $ with equation $ x_n = 0 $, orthogonal to the vector $ e_n $. To every point $ x = (x_i) $ of $ S_{n-1} $, other than $ e_n $, let us make correspond the point $ y $ where the line through $ e_n $ and $ x $ meets the hyperplane $ H $ (Fig. 3). It is easily verified that we have

$$
y = \frac{1}{1 - x_n} (x - x_n e_n)
$$

and

$$
x = \frac{||y||^2 - 1}{||y||^2 + 1} e_n + \frac{2}{||y||^2 + 1} y.
$$

![Diagram showing stereographic projection](https://i.imgur.com/3Q5z5QG.png)

Figure 3.

If we denote by $ A $ the complement of $ \{ e_n \} $ in $ S_{n-1} $, these formulas show that we have thus defined a homeomorphism of $ A $ onto the hyperplane $ H $. This homeomorphism is called the stereographic projection of $ A $ onto $ H $, or (by abuse of language) the stereographic projection of $ S_{n-1} $ onto $ H $; $ e_n $ is the vertex of the projection, $ H $ the hyperplane of projection. More generally, if $ H' $ is any hyperplane passing through $ o $ (a diametral hyperplane of $ B_n $) and if $ a $ is one of the points of intersection of $ S_{n-1} $ and the line orthogonal to $ H' $ passing through $ o $, we can define in the same way the stereographic projection with vertex $ a $ onto the hyperplane of projection $ H' $; in any case this projection can be brought back to the preceding one by an orthogonal transformation which transforms $ H' $ into $ H $ and $ a $ into $ e_n $.

#### Proposition 4 {#top-vi-s2-prop-4 .statement}

*If $ n > 1 $, the Euclidean sphere $ S_{n-1} $ is homeomorphic to the space $ \mathbf{R}^{n-1} $ made compact by adjoining a "point at infinity"*(Chapter I, § 9, no. 8, Theorem 4).

For the stereographic projection defines a homeomorphism of the complement of a point in $ S_{n-1} $ onto a hyperplane of $ \mathbf{R}^n $, which is homeomorphic to $ \mathbf{R}^{n-1} $.

#### Corollary 1 {#top-vi-s2-prop-4-cor-1 .statement}

*The sphere $ S_n $ is homeomorphic to the quotient space of the ball $ B_n $ obtained by identifying all the points of the sphere $ S_{n-1} $*.

The ball $ B_n $ is a regular space (Chapter I, § 8, no. 4); hence the quotient space $ F $ of $ B_n $ obtained by identifying all the points of $ S_{n-1} $ is *Hausdorff* (Chapter I, § 8, no. 6, Proposition 15). Since $ B_n $ is compact, so is $ F $, and $ F $ is therefore homeomorphic to an open ball of $ n $ dimensions made compact by adjoining a point at infinity, by Alexandroff's theorem (Chapter I, § 9, no. 8, Theorem 4). The result therefore follows from Propositions 2 and 4.

#### Corollary 2 {#top-vi-s2-prop-4-cor-2 .statement}

*The circle $ S_1 $ is homeomorphic to the torus $ T $*.

In Chapter VIII, § 2, no. 1, we shall obtain this result again as a consequence of a more precise theorem.

#### Proposition 5 {#top-vi-s2-prop-5 .statement}

*If $ n > 1 $, the Euclidean sphere $ S_{n-1} $ is connected and locally connected, and every point of it has an open neighbourhood homeomorphic to $ \mathbf{R}^{n-1} $.*

The complement of a point in $ S_{n-1} $ is a connected dense set, and therefore (Chapter I, § 11, no. 1, Proposition 1) $ S_{n-1} $ is connected. To see that every point has a neighbourhood homeomorphic to $ \mathbf{R}^{n-1} $, we have only to project stereographically from a vertex other than the given point.

From this proposition and from Proposition 3 of no. 3 it follows that $ \mathbf{R}_n^* $, being the product of two connected spaces, is connected (Chapter I, § 11, no. 4, Proposition 8; cf. § 1, Exercise 10).

The intersection of $ S_{n-1} $ and a closed (resp. open) half-space determined by a diametral hyperplane of $ B_n $ is called a *closed* (resp. *open*) *hemisphere* of $ S_{n-1} $. By stereographic projection onto the diametral hyperplane, the closed (resp. open) hemisphere which does not contain the vertex of projection is mapped onto a *closed* (resp. *open*) ball of $ n - 1 $ dimensions, to which it is therefore *homeomorphic*.

If $ n = 2 $, we say "semicircle" instead of "hemisphere".

### Exercises {#top-vi-s2-exercises}

See the [exercises for § 2](exercises/s2/).
