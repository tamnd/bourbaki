---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 1
section_title: Complex numbers, quaternions
lang: en
source: top-v-x
pdf_pages: 0106-0111, 0129-0131
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF COMPLEX NUMBERS
      page: 0
      pdf_page: 106
    - "no": 2
      title: THE TOPOLOGY OF $ \mathbf{C} $
      page: 0
      pdf_page: 108
    - "no": 3
      title: THE MULTIPLICATIVE GROUP $ \mathbf{C}^* $
      page: 0
      pdf_page: 109
    - "no": 4
      title: THE DIVISION RING OF QUATERNIONS
      page: 0
      pdf_page: 110
statements: 8
exercises: 5
content_sha256: 4f76f1968946b21c15bf121fd31c7fe9e3dcf0257a9b139060673abddd129427
---

## 1. COMPLEX NUMBERS, QUATERNIONS

### 1. DEFINITION OF COMPLEX NUMBERS

The polynomial $ X^2 + 1 $ has no root in $ \mathbf{R} $, because $ x^2 + 1 \geq 1 $ for all $ x \in \mathbf{R} $; it is therefore irreducible over $ \mathbf{R} $. [This is a particular case of the analogous result which applies to any ordered field.]

#### Definition 1 {#top-viii-s1-def-1 .statement}

*The field* $ \mathbf{R}[X]/(X^2 + 1) $ *is called the field of complex numbers and is denoted by* $ \mathbf{C} $. *The canonical image of* $ X $ *in* $ \mathbf{C} $ *is denoted by* $ i $, *so that* $ \mathbf{C} $ *is obtained from the field* $ \mathbf{R} $ *by algebraic adjunction of the root* $ i $ *of the polynomial* $ X^2 + 1 $. *The elements of* $ \mathbf{C} $ *are called complex numbers*.

From an algebraic point of view the importance of the field $ \mathbf{C} $ is due to the following fundamental theorem:

#### Theorem 1 {#top-viii-s1-thm-1 .statement}

(d'Alembert-Gauss). *The field* $ \mathbf{C} $ *of complex numbers is algebraically closed*.

For the proof it is enough to establish that (i) every element $ \geq 0 $ in $ \mathbf{R} $ has a *square root*, and (ii) every polynomial of *odd* degree with coefficients in $ \mathbf{R} $ has *at least one root* in $ \mathbf{R} $. The first of these assertions has already been proved in Chapter IV, § 3, no. 3. As to the second, if $ f(X) = a_0 X^n + a_1 X^{n-1} + \cdots + a_n $ is a polynomial of odd degree $ n $ ($ a_0 \neq 0 $) with real coefficients, we may write $ f(x) = a_0 x^n g(x) $ for $ x \neq 0 $, where

$$
g(x) = 1 + \frac{a_1}{a_0 x} + \cdots + \frac{a_n}{a_0 x^n}
$$

tends to $ +1 $ as $ x $ tends to $ +\infty $ or $ -\infty $. Hence there is a number $ a > 0 $ such that $ f(a) $ has the sign of $ a_0 $ and $ f(-a) $ the sign of $ -a_0 $;

and so by Bolzano’s theorem (Chapter IV, § 6, no. 1, Theorem 2), $ f $ has at least one root in $[—a, a]$.

#### Remark 1 {#top-viii-s1-n1-rem-1 .statement}

Theorem 1 can be proved without invoking the theory of ordered fields by using properties of the topology of the field $ \mathbf{C} $, which will be defined below (no. 2); see § 2, Exercise 2 and also the part of this series devoted to algebraic topology, where the theorem of d’Alembert-Gauss will appear as a consequence of results on the degree of a mapping.
2) Since $ \mathbf{C} $ is of degree 2 over $ \mathbf{R} $, it follows that $ \mathbf{C} $ is, up to isomorphism, the only algebraic extension of $ \mathbf{R} $ other than $ \mathbf{R} $ itself, and that there is no field contained in $ \mathbf{C} $ which contains $ \mathbf{R} $, other than $ \mathbf{R} $ and $ \mathbf{C} $.

We know that $ \mathbf{R} $ may be identified with a subfield of $ \mathbf{C} $, and that every $ z \in \mathbf{C} $ can be written uniquely in the form $ x + iy $, where $ x $ and $ y $ are real; $ x $ is called the real part of $ z $ and is denoted by $ \Re(z) $; $ y $ the imaginary part of $ z $, denoted by $ \Im(z) $. Complex numbers of the form $ iy $ ($ y $ real) are called pure imaginary. The relation $ x + iy = 0 $ ($ x, y $ real) is equivalent to $ x = 0 $ and $ y = 0 $.

Since $ i^2 = -1 $, the elements of $ \mathbf{C} $ (when given by their real and imaginary parts) satisfy the following rules of calculation:

$$
(x + iy) + (x' + iy') = (x + x') + i(y + y')
$$
$$
(x + iy)(x' + iy') = (xx' - yy') + i(xy' + x'y').
$$

In particular, $ (x + iy)(x - iy) = x^2 + y^2 \in \mathbf{R} $, so that, if $ x + iy \neq 0 $,

$$
\frac{1}{x + iy} = \frac{x}{x^2 + y^2} - i \frac{y}{x^2 + y^2}.
$$

The second root of the polynomial $ X^2 + 1 $ in $ \mathbf{C} $ is $ -i $; consequently the only automorphism of $ \mathbf{C} $, other than the identity mapping, which leaves all real numbers invariant, is that which maps $ z = x + iy $ to $ x - iy $; the latter is denoted by $ \overline{z} $ and (in agreement with the general definitions) is called the complex number conjugate to $ z $. We have

$$
\Re(z) = \frac{1}{2}(z + \overline{z}) \quad \text{and} \quad \Im(z) = \frac{1}{2i}(z - \overline{z}).
$$

By reason of this automorphism, if $ f(z) $ is a polynomial with real coefficients, we have $ f(\overline{z}) = \overline{f(z)} $ for all $ z \in \mathbf{C} $.

The real number $ z \overline{z} = x^2 + y^2 $ is called the algebraic norm of $ z $, or simply the norm whenever there is no risk of confusion; it is a real number $ \geq 0 $, which vanishes only if $ z = 0 $. The real number $ \sqrt{z \overline{z}} = \sqrt{x^2 + y^2} \geq 0 $ reduces to the absolute value of $ z $ when $ z $ is real, and we still call it the absolute value of $ z $, and denote it by $ |z| $, when $ z $ is any complex number. The relation $ |z| = 0 $ is equivalent to $ z = 0 $. If $ z $ and $ z' $ are two complex numbers, the conjugate of $ zz' $ is $ \overline{zz'} $, hence $ |zz'|^2 = zz'\overline{zz'} = |z|^2|z'|^2 $ and therefore $ |zz'| = |z|\cdot|z'| $: *the absolute value of a product is the product of the absolute values of the factors.* In particular, if $ z \neq 0 $ and $ z' = 1/z $, we have $ |1/z| = |1/z| $.

Finally, for all complex numbers $ z, z' $, we have the *triangle inequality*
$$
|z + z'| \leq |z| + |z'|.
$$

### 2. THE TOPOLOGY OF $ \mathbf{C} $

The mapping $ (x, y) \to x + iy $ of the real plane $ \mathbf{R}^2 $ onto $ \mathbf{C} $ is *bijective*; by means of this bijection we can *transport* to $ \mathbf{C} $ the topology of $ \mathbf{R}^2 $ (cf. Chapter VI, § 1, no. 5). The topology thus defined on $ \mathbf{C} $ is *compatible* with the field structure of $ \mathbf{C} $ (Chapter III, § 6, no. 7), because it is compatible with the ring structure of $ \mathbf{C} $ (Chapter VI, § 1, no. 5) and, by (3), $ 1/z $ is continuous on the complement $ \mathbf{C}^* $ of 0 in $ \mathbf{C} $.

If we endow the set $ \mathbf{C} $ with this topology and with the field structure defined earlier (no. 1, Definition 1), we have defined on $ \mathbf{C} $ the structure of a *topological field* (Chapter III, § 6, no. 7); whenever we speak of the topology of $ \mathbf{C} $ it will always be the above topology that is meant.

In the future we shall generally *identify* the sets $ \mathbf{C} $ and $ \mathbf{R}^2 $ considered as topological spaces; the subfield $ \mathbf{R} $ of $ \mathbf{C} $ is then identified with the abscissa of $ \mathbf{R}^2 $, which for this reason is called the *real axis*; likewise the ordinate is called the *imaginary axis* (note that this is *not* a subfield of $ \mathbf{C} $). The ray with origin 0 and direction ratios $ (1, 0) $ (identified with $ \mathbf{R}_+ $) is called the *positive real semi-axis*; the opposite ray, with the same origin and direction ratios $ (-1, 0) $, is called the *negative real semi-axis*.

For the purposes of graphical illustration we use the representation of $ \mathbf{R}^2 $ (well known in elementary analytic geometry) by the points of a plane in which have been drawn two perpendicular coordinate axes, representing respectively the real axis and the imaginary axis of $ \mathbf{C} $ (Fig. 7).

As in every topological field, every *rational function* of $ n $ complex variables with complex coefficients is *continuous* at every point of $ \mathbf{C}^n $ at which the denominator does not vanish.

![A diagram showing the complex plane with axes labeled x and y, and a point labeled z = x + iy](https://i.imgur.com/3Q5z5QG.png)

Figure 7.

The permutation $ z \to \overline{z} $ of $ \mathbf{C} $ is continuous, and is therefore an automorphism of the topological field $ \mathbf{C} $.

In fact it is the only automorphism of the topological field $ \mathbf{C} $ other than the identity automorphism (see Exercise 4).

The functions $ \Re(z), \Im(z) $ are just the projections of $ \mathbf{R}^2 $ onto its factors, and are therefore continuous; the same is true of the absolute value $ |z| $, since it is the Euclidean norm (Chapter VI, § 2, no. 1) of the point $ (x, y) $ in $ \mathbf{R}^2 $.

The properties of the absolute value lead to another proof of the fact that the topology of $ \mathbf{C} $ is compatible with its field structure (cf. Chapter IX, § 3, no. 2); the continuity of $ z + z' $ follows from the triangle inequality $ |z + z'| \leq |z| + |z'| $; that of $ zz' $ follows from the relation
$$
|zz' - z_0z'_0| = |z_0(z' - z'_0) + (z - z_0)z'_0 + (z - z_0)(z' - z'_0)| \\
\leq |z_0| \cdot |z' - z'_0| + |z'_0| \cdot |z - z_0| + |z - z_0| \cdot |z' - z'_0|;
$$
lastly, the continuity of $ z^{-1} $ follows from the relation
$$
|z_0^{-1} - z^{-1}| = |z|^{-1} \cdot |z - z_0| \cdot |z_0|^{-1}.
$$

### 3. THE MULTIPLICATIVE GROUP $ \mathbf{C}^* $

We know from Chapter III, § 6, no. 7 that the topology induced on the multiplicative group $ \mathbf{C}^* $ of non-zero complex numbers is compatible with the group structure of $ \mathbf{C}^* $. Since $ \mathbf{C}^* $ is open in $ \mathbf{C} $, it follows that $ \mathbf{C}^* $ is a locally compact topological group (Chapter I, § 9, no. 7, Proposition 13) and therefore complete (with respect to the multiplicative uniformity; cf. Chapter III, § 6, no. 8, Proposition 8). The multiplicative group $ \mathbf{R}_+^* $ of real numbers $ > 0 $ is a closed subgroup of $ \mathbf{C}^* $. Another subgroup is the set $ \mathbf{U} $ of complex numbers of absolute value 1, which is identified with the unit circle $ S_1 $ of $ \mathbf{R}^2 $, and is therefore a compact group. Moreover:

#### Proposition 1 {#top-viii-s1-prop-1 .statement}

*The topological group $ \mathbf{C}^* $ is isomorphic to the product of the topological groups $ \mathbf{R}^* $ and $ \mathbf{U} $.*

For the mapping $ z \to \left( |z|, \frac{z}{|z|} \right) $ is a homeomorphism of $ \mathbf{C}^* $ onto $ \mathbf{R}_+^* \times \mathbf{U} $ (Chapter VI, § 2, no. 3, Proposition 3); and it follows immediately that it is an isomorphism of the group structures.

The topological group $ \mathbf{R}_+^* $ is already known to be isomorphic to the additive group $ \mathbf{R} $ (Chapter V, § 4, Theorem 1); the study of the topological group $ \mathbf{C}^* $ is therefore reduced to that of $ \mathbf{U} $, which we shall consider in § 2.

### 4. THE DIVISION RING OF QUATERNIONS

It follows from Theorem 1 that the field $ \mathbf{R} $ is a maximal ordered field, and therefore the only non-commutative division ring of finite rank over $ \mathbf{R} $ is (up to isomorphism) the division ring of quaternions over $ \mathbf{R} $; it is denoted by $ \mathbf{H} $ and is called the division ring of real quaternions (or simply the division ring of quaternions, when there is no fear of confusion). Since $ \mathbf{H} $ is of rank 4 over the field $ \mathbf{R} $, we can define a topology on $ \mathbf{H} $ homeomorphic to that of $ \mathbf{R}^4 $ (Chapter VI, § 1, no. 5). To be precise, we shall usually identify $ \mathbf{H} $ with $ \mathbf{R}^4 $, the elements $ i, i, j, k $ of the canonical basis of $ \mathbf{H} $ being identified respectively with the vectors $ e_0, e_1, e_2, e_3 $ of the canonical basis of $ \mathbf{R}^4 $.

We recall that the multiplication table of the canonical basis of $ \mathbf{H} $ is given by the formulae

$$
i^2 = j^2 = k^2 = -1, \quad ij = -ji = k,
jk = -kj = i, \quad ki = -ik = j.
$$

The topology of $ \mathbf{H} $ is compatible not only with the ring structure of $ \mathbf{H} $ (Chapter VI, § 1, no. 5) but also with its division ring structure; for if $ x $ is a non-zero quaternion, the coordinates of $ x^{-1} $ are rational functions of those of $ x $, whose denominators do not vanish. The division ring $ \mathbf{H} $, endowed with this topology, is therefore a non-commutative topological division ring. The quaternions $ a + bi $ ($ a, b $ real) form a (topological) subfield of $ \mathbf{H} $, isomorphic to the field $ \mathbf{C} $, with which it is often identified.

We have thus a third example of a locally compact, connected topological division ring, the others being $ \mathbf{R} $ and $ \mathbf{C} $. In fact these are the only topological division rings with these two properties.

We know from algebra that the reduced norm of a quaternion $ x = x_0 + x_1 i + x_2 j + x_3 k $ is

$$
N(x) = x_0^2 + x_1^2 + x_2^2 + x_3^2 = ||x||^2
$$

(it is therefore the square of the Euclidean norm of $ x $). Since

$$
N(xy) = N(x)N(y),
$$

it follows that the set of all quaternions of norm 1, which is identical with the sphere $ S_3 $, forms a compact subgroup of the multiplicative group $ \mathbf{H}^* $ of non-zero quaternions.

#### Proposition 2 {#top-viii-s1-prop-2 .statement}

The multiplicative group $ \mathbf{H}^* $ of non-zero quaternions is a topological group isomorphic to the product of its subgroups $ \mathbf{R}_+^* $ and $ S_3 $.

Every quaternion $ x / o $ can be written as $ x \cdot z $ where $ z $ is a quaternion with norm 1; since $ \|xx'\| = \|x\|\cdot\|x'\| $, the mapping $ x \to (\|x\|, x_1, x_2) $ of $ H^* $ onto $ \mathbf{R}_+^* \times S_2 $ is an isomorphism of the group structures, and from Chapter VI, § 2, no. 2, Proposition 2, it is a homomorphism of $ H^* $ onto $ \mathbf{R}_+^* \times S_2 $.

#### Remark 1 {#top-viii-s1-n4-rem-1 .statement}

With the use of the relations $ \|x + y\| = \|x\| + \|y\| $ and $ \|xy\| = \|x\|\cdot\|y\| $ it can be proved directly, as with the field of complex numbers in no. 2, that the topology of $ \mathbf{R}^4 $ is compatible with the division ring structure of $ H $ (cf. Chapter IX, § 3, no. 2).

#### Remark 2 {#top-viii-s1-n4-rem-2 .statement}

From what has been proved it follows that the spheres $ S_1 $ and $ S_n $ can carry a group structure compatible with their topology. We shall see later that, for each integer $ n $ other than 1 and 3, there exists no group structure on $ S_n $ compatible with the topology of $ S_n $.

#### Remark 3 {#top-viii-s1-n4-rem-3 .statement}

Every point of the group $ S_2 $ has a neighbourhood homeomorphic to $ \mathbf{R}^3 $ (Chapter VI, § 2, no. 4, Proposition 5) but $ S_4 $ is not locally isomorphic to $ \mathbf{R}^3 $; for if it were it would be abelian, since it is connected (Chapter VII, § 2, no. 2, Theorem 1), and this is not the case, since $ i $ and $ j $ belong to $ S_3 $ and $ ij \neq ji $ (cf. Chapter V, § 3).

### Exercises {#top-viii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
