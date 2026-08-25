---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 1
section_title: Subgroups and quotient groups of R
lang: en
source: top-v-x
pdf_pages: 0013-0017, 0030-0031
extraction: ocr
subsections:
    - "no": 1
      title: CLOSED SUBGROUPS OF $ \mathbf{R} $
      page: 0
      pdf_page: 13
    - "no": 2
      title: QUOTIENT GROUPS OF $ \mathbf{R} $
      page: 0
      pdf_page: 13
    - "no": 3
      title: CONTINUOUS HOMOMORPHISMS OF $ \mathbf{R} $ INTO ITSELF
      page: 0
      pdf_page: 15
    - "no": 4
      title: LOCAL DEFINITION OF A CONTINUOUS HOMOMORPHISM OF $ \mathbf{R} $ INTO A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 15
statements: 13
exercises: 3
content_sha256: 0513ba6a9bc41e90886babf7d0b0e14690c3eae643b9d00e406e9fd2dc2956f4
---

## 1. SUBGROUPS AND QUOTIENT GROUPS OF $ \mathbf{R} $

### 1. CLOSED SUBGROUPS OF $ \mathbf{R} $

#### Proposition 1 {#top-v-s1-prop-1 .statement}

*Every closed subgroup of the additive group $ \mathbf{R} $, other than $ \mathbf{R} $ and $ \{0\} $, is a discrete group of the form $ a.\mathbf{Z} $, where $ a > 0 $* (in other words, it consists of the integer multiples of $ a $).

We begin by showing that every non-discrete subgroup of $ \mathbf{R} $ is dense in $ \mathbf{R} $. If a subgroup $ G $ of $ \mathbf{R} $ is not discrete, then for every $ \varepsilon > 0 $ there is a point $ x \neq 0 $ in $ G $ which belongs to the interval $[-\varepsilon, +\varepsilon]$; since all integer multiples of $ x $ belong to $ G $, every interval of length $ > \varepsilon $ contains an element of $ G $, and therefore $ G $ is dense in $ \mathbf{R} $.

Every closed subgroup of $ \mathbf{R} $ other than $ \mathbf{R} $ itself is therefore discrete. It remains to show that every discrete subgroup $ G $ of $ \mathbf{R} $ other than $ \{0\} $ is of the form $ a.\mathbf{Z} $, where $ a > 0 $. Now the relation $ -G = G $ shows that the set $ H $ of elements $ > 0 $ in $ G $ is not empty; if $ b \in H $, the intersection of the interval $[0, b]$ and $ G $ is *compact and discrete*, and is therefore *finite*. Let $ a $ be the smallest element of $ H $ contained in $[0, b]$, and for every $ x \in G $ put $ m = [x/a] $, the integer part of $ x/a $; then we have $ x - ma \in G $ and $ 0 \leq x - ma < a $. By the definition of $ a $ it follows that $ x - ma = 0 $ and therefore $ G = a.\mathbf{Z} $.

### 2. QUOTIENT GROUPS OF $ \mathbf{R} $

Every *Hausdorff* quotient group of $ \mathbf{R} $ is of the form $ \mathbf{R}/H $, where $ H $ is a *closed* subgroup of $ \mathbf{R} $ (Chapter III, § 2, no. 6, Proposition 18); hence, by Proposition 1 of no. 1:

#### Proposition 2 {#top-v-s1-prop-2 .statement}

*The Hausdorff quotient groups of* $ \mathbf{R} $, *other than* $ \{0\} $, *are the groups* $ \mathbf{R}/a\mathbf{Z} $ ($ a \geqslant 0 $).
*If* $ a $ *and* $ b $ *are* $ > 0 $, *the automorphism* $ x \to b/a\,x $ *of* $ \mathbf{R} $ *transforms* $ a\mathbf{Z} $ *into* $ b\mathbf{Z} $, *and therefore* (Chapter III, § 2, no. 8, Remark 3) *the quotient groups* $ \mathbf{R}/a\mathbf{Z} $ *and* $ \mathbf{R}/b\mathbf{Z} $ *are isomorphic; in other words*:

#### Proposition 3 {#top-v-s1-prop-3 .statement}

*Every Hausdorff quotient group of* $ \mathbf{R} $, *other than* $ \mathbf{R} $ *and* $ \{0\} $, *is isomorphic to the group* $ \mathbf{R}/\mathbf{Z} $.

#### Definition 1 {#top-v-s1-def-1 .statement}

*The topological group* $ \mathbf{R}/a\mathbf{Z} $ ($ a > 0 $) *is called the additive group of real numbers modulo* $ a $. *The topological group* $ \mathbf{R}/\mathbf{Z} $ *is denoted by* $ \mathbf{T} $. *As a topological space,* $ \mathbf{T} $ *is called the one-dimensional torus* (by abuse of language, the topological group $ \mathbf{T} $ is also called the one-dimensional torus).

#### Remark 1 {#top-v-s1-n2-rem-1 .statement}

*The relation* $ x \equiv y \pmod{a\mathbf{Z}} $ *is usually written* $ x \equiv y \pmod{a} $, *or simply* $ x \equiv y (a) $, *and is read* "x and y are congruent modulo a"; *it means that* $ x - y $ *is an integer multiple of* $ a $. *When* $ a $ *is an integer, the relation induced on* $ \mathbf{Z} $ *by this relation is precisely congruence modulo* $ a $; *this justifies the notation*.

#### Remark 2 {#top-v-s1-n2-rem-2 .statement}

*As we shall see in Chapter VI, § 2, no. 4, the topological space* $ \mathbf{T} $ *is homeomorphic to the circle* $ x^2 + y^2 = 1 $ *in the real number plane* $ \mathbf{R}^2 $; *the product space* $ \mathbf{T}^2 $ *is homeomorphic to a* torus of revolution *in* $ \mathbf{R}^3 $ *(Chapter VII, § 1, Exercise 15)*. *This is the origin of the name* "one-dimensional torus" *for* $ \mathbf{T} $ *(in Chapter VII, § 1, we shall call* $ \mathbf{T}^n $ *the n-dimensional torus)* *.

#### Proposition 4 {#top-v-s1-prop-4 .statement}

*The torus* $ \mathbf{T} $ *is homoeomorphic to the quotient space of any closed interval of* $ \mathbf{R} $ *of the form* $ [a, a+1] $ *obtained by identifying the end-points of this interval; it is compact, connected and locally connected*.

Every $ x \in \mathbf{R} $ *is congruent* $ (\bmod\,1) $ *to some number in the interval* $ [a, a+1] $, *namely to* $ x - [x-a] $; *hence* $ \mathbf{T} $ *is the image of this interval under the canonical mapping* $ \varphi $ *of* $ \mathbf{R} $ *onto* $ \mathbf{R}/\mathbf{Z} $, *and is therefore compact and connected* (Chapter I, § 9, no. 4, Theorem 2, and § 11, no. 2, Proposition 4). *On the other hand, two distinct elements of the interval* $ [a, a+1] $ *are congruent* $ (\bmod\,1) $ *only if they are the end-points of the interval; from the compactness of* $ \mathbf{T} $ *it therefore follows that* $ \mathbf{T} $ *is homeomorphic to the quotient space of* $ [a, a+1] $ *obtained by identifying the end-points* (Chapter I, § 9, no. 4, Theorem 2, Corollary 4, and § 10, no. 4, Proposition 8). *Finally,* $ \mathbf{Z} $ *being a discrete subgroup of* $ \mathbf{R} $, $ \mathbf{T} = \mathbf{R}/\mathbf{Z} $ *is* locally isomorphic *to* $ \mathbf{R} $ *(Chapter III, § 2, no. 6, Proposition 19)* and in particular is locally connected (this last fact is also a consequence of Chapter I, § 11, no. 6, Proposition 12).

#### Remark {#top-v-s1-n2-rem-3 .statement}

Note that the canonical mapping $ \varphi $ of $ \mathbf{R} $ onto $ T = \mathbf{R}/\mathbf{Z} $, restricted to the half-open interval $[a, a+1[$, is a continuous bijective mapping of this interval onto $ T $; the inverse mapping is continuous at every point of $ T $ other than $ \varphi(a) $, but discontinuous at $ \varphi(a) $. We shall sometimes identify the space $ T $ with the interval $[a, a+1[$, endowed with the topology which is the inverse image under $ \varphi $ of the topology of $ T $ (Chapter I, § 1, no. 3); this topology is of course not the same as that induced on $[a, a+1[$ by the topology of $ \mathbf{R} $.

### 3. CONTINUOUS HOMOMORPHISMS OF $ \mathbf{R} $ INTO ITSELF

#### Proposition 5 {#top-v-s1-prop-5 .statement}

Every continuous homomorphism $ f $ of the topological group $ \mathbf{R} $ into itself is of the form $ x \to ax $, where $ a \in \mathbf{R} $; it is an automorphism of $ \mathbf{R} $ if $ a \neq 0 $.

For every $ x \in \mathbf{R} $ and every integer $ p \in \mathbf{Z} $, we have $ f(px) = pf(x) $; replacing $ x $ by $ (1/p)x $, it follows that

$$
f\left(\frac{1}{p}x\right) = \frac{1}{p} f(x) \quad \text{if } p \neq 0;
$$

hence, for all integers $ p $ and $ q \neq 0 $, we have

$$
f\left(\frac{p}{q}x\right) = \frac{p}{q} f(x).
$$

In other words, $ f(rx) = rf(x) $ for all rational numbers $ r $. If now $ t $ is any real number, by reason of the continuity of $ f $ we have

$$
f(tx) = \lim_{r \to t, r \in \mathbf{Q}} f(rx) = \lim_{r \to t, r \in \mathbf{Q}} rf(x) = \left( \lim_{r \to t, r \in \mathbf{Q}} r \right) f(x) = tf(x).
$$

In particular, if $ a = f(1) $ we have $ f(t) = at $, and the proposition is proved.

The group of automorphisms of the topological group $ \mathbf{R} $ is therefore isomorphic to the multiplicative group $ \mathbf{R}^* $ of non-zero real numbers.

#### Corollary {#top-v-s1-n3-cor-1 .statement}

Let $ G $ be a topological group isomorphic to $ \mathbf{R} $. For each $ a \in G $ there is exactly one continuous homomorphism $ f_a $ of $ \mathbf{R} $ into $ G $ such that $ f_a(1) = a $, and this homomorphism is an isomorphism of $ \mathbf{R} $ onto $ G $ if $ a $ is not the zero element of $ G $.

### 4. LOCAL DEFINITION OF A CONTINUOUS HOMOMORPHISM OF $ \mathbf{R} $ INTO A TOPOLOGICAL GROUP

If we are given a group $ G $ and a subset $ A $ of $ G $ which generates $ G $, it is clear that two homomorphisms $ f, g $ of $ G $ into a group $ G' $ coincide if they take the same value at every point of $ A $. But the values on $ A $ of a homomorphism $ f $ of $ G $ into $ G' $ cannot in general be taken arbitrarily; if $ G $ and $ G' $ are written multiplicatively, these values must satisfy the condition $ f(xy) = f(x)f(y) $ for each pair $ (x, y) $ such that $ x \in A, y \in A $ and $ xy \in A $. Moreover, this necessary condition is not in general sufficient.

In particular, a *local isomorphism* of a topological group $ G $ with a topological group $ G' $ cannot always be extended to a homomorphism (continuous or not) of $ G $ into $ G' $. For example, a local isomorphism $ f $ of $ T $ with $ \mathbf{R} $ cannot be extended to a homomorphism of $ T $ into $ \mathbf{R} $; for if $ f $ is defined on a neighbourhood $ V $ of $ o $, there is an integer $ p > 0 $ such that the class $ x \pmod{\mathbf{Z}} $ of $ \frac{1}{p} $ belongs to $ V $; since $ x $ has order $ p $ in $ T $, its image under every homomorphism of $ T $ into $ \mathbf{R} $ is necessarily $ o $ and therefore distinct from $ f(x) $ by hypothesis.

In this respect the topological group $ \mathbf{R} $ enjoys the following property:

#### Proposition 6 {#top-v-s1-prop-6 .statement}

*Let $ I $ be an interval of $ \mathbf{R} $ which contains $ o $ and at least one other point; let $ f $ be a continuous mapping of $ I $ into a topological group $ G $ (written multiplicatively), such that $ f(x+y) = f(x)f(y) $ for each pair of points $ (x, y) $ such that $ x \in I, y \in I $ and $ x + y \in I $. Then there is a unique continuous homomorphism of $ \mathbf{R} $ into $ G $ which extends $ f $.*.

The uniqueness of the extension (if it exists) follows from the preceding remarks, because $ I $ generates the group $ \mathbf{R} $. We have to establish the existence of such an extension.

If $ n $ is an integer $ > 0 $ and if $ x \in I $ and $ nx \in I $, we have $ f(nx) = (f(x))^n $, by induction on $ n $ (since $ mx \in I $ for all integers $ m $ such that $ 1 \leq m \leq n $). Put $ J = \bigcup_{n \in \mathbf{N}} nI $; $ J $ is either the whole line $ \mathbf{R} $, or one of the intervals $[0, +\infty[$ or $[-\infty, 0]$, according as $ o $ is or is not an interior point of $ I $. If $ x \in J $ we have $ x/n \in I $ whenever $ n $ is a sufficiently large integer $ > 0 $. Let $ x \in J $, and let $ m, n $ be two integers $ > 0 $ such that $ x/n \in I $ and $ x/m \in I $; then $ x/mn \in I $, and therefore

$$
f\left( \frac{x}{m} \right) = \left( f\left( \frac{x}{mn} \right) \right)^n \quad \text{and} \quad f\left( \frac{x}{n} \right) = \left( f\left( \frac{x}{mn} \right) \right)^m;
$$

in other words, the element $ (f(x/n))^n $ of $ G $ is the same for all integers $ n > 0 $ such that $ x/n \in I $. Let us denote this element by $ f_1(x) $; $ f_1 $ is a mapping of $ J $ into $ G $, which agrees with $ f $ on $ I $ and is therefore continuous at the point $ o $ (with respect to $ J $). Let $ x, y $ be two elements of J and let n be a sufficiently large integer > 0 such that $ \frac{x}{n} \in I, \frac{y}{n} \in I $ and $ \frac{x+y}{n} \in I $; then

$$
f\left( \frac{x+y}{n} \right) = f\left( \frac{x}{n} \right) f\left( \frac{y}{n} \right) = f\left( \frac{y}{n} \right) f\left( \frac{x}{n} \right),
$$

which shows that $ f\left( \frac{x}{n} \right) $ and $ f\left( \frac{y}{n} \right) $ commute; by the definition of $ f_1 $, we have therefore $ f_1(x+y) = f_1(x) f_1(y) $. If $ J = \mathbf{R} $, the proof is complete; if not, say $ J = [0, +\infty[ $, and for each $ x < 0 $ define $ f_1(x) $ to be $ (f_1(-x))^{-1} $. Then the relation $ f_1(x+y) = f_1(x) f_1(y) $ remains valid for all $ x \in \mathbf{R} $ and all $ y \in \mathbf{R} $. This is clear if $ x < 0 $ and $ y < 0 $; if $ x \geqslant 0 $, $ y < 0 $ and $ x + y \geqslant 0 $ it follows from $ f_1(x) = f_1(x+y) f_1(-y) $; similarly if $ x \geqslant 0, y < 0 $ and $ x + y < 0 $, for then we have

$$
f_1(-y) = f_1(-x-y) f_1(x);
$$

analogous proofs for $ x < 0 $ and $ y \geqslant 0 $. We see therefore that $ f_1 $ is a homomorphism of $ \mathbf{R} $ into G, so that $ f_1(0) = e $, the identity element of G; and since $ f_1 $ is continuous with respect to J, it has a limit on the right at 0, equal to $ e $; since $ f_1(-x) = (f_1(x))^{-1} $, $ f_1 $ also has a limit at 0 on the left, equal to $ e $; thus $ f_1 $ is continuous at 0, and the proof is complete.

#### Corollary {#top-v-s1-n4-cor-1 .statement}

*Let f be a local isomorphism of $ \mathbf{R} $ with a topological group G. Then there is a unique strict morphism of $ \mathbf{R} $ onto an open subgroup of G which coincides with f at all points of some neighbourhood of 0.*

Let $ \overline{f} $ be the continuous homomorphism of $ \mathbf{R} $ into G which coincides with $ f $ at all points of an open interval I, which contains 0 and is contained in the set on which $ f $ is defined; $ \overline{f}(\mathbf{R}) $ by hypothesis contains a neighbourhood of the identity element of G, hence (Chapter III, § 2, no. 1, Corollary to Proposition 4) is an open subgroup of G; and $ \overline{f} $ is a strict morphism of $ \mathbf{R} $ onto $ \overline{f}(\mathbf{R}) $, by Chapter III, § 2, no. 8, Proposition 24.

#### Proposition 7 {#top-v-s1-prop-7 .statement}

*Every connected group G which is locally isomorphic to $ \mathbf{R} $ is isomorphic to either $ \mathbf{R} $ or $ \mathbf{T} $.*

For a local isomorphism of $ \mathbf{R} $ with G extends to a strict morphism of $ \mathbf{R} $ onto an open subgroup of G (Corollary to Proposition 6), hence onto G itself since G is connected. Hence G is isomorphic to a quotient group of $ \mathbf{R} $; since G is Hausdorff and does not consist of the identity element alone (because it is locally isomorphic to $ \mathbf{R} $), it is isomorphic to either $ \mathbf{R} $ or $ \mathbf{T} $ by Proposition 3 of no. 2.

### Exercises {#top-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
