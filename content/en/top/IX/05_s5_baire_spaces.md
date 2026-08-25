---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 5
section_title: Baire spaces
lang: en
source: top-v-x
pdf_pages: 0196-0201, 0256-0264
extraction: ocr
subsections:
    - "no": 1
      title: NOWHERE DENSE SETS
      page: 0
      pdf_page: 196
    - "no": 2
      title: MEAGRE SETS
      page: 0
      pdf_page: 198
    - "no": 3
      title: BAIRE SPACES
      page: 0
      pdf_page: 198
    - "no": 4
      title: SEMI-CONTINUOUS FUNCTIONS ON A BAIRE SPACE
      page: 0
      pdf_page: 200
statements: 16
exercises: 4
content_sha256: 6ff94456cd858603fde2c77c69631bf89eb86771a095a8ba19828965838d440b
---

## 5. BAIRE SPACES

### 1. NOWHERE DENSE SETS

#### Definition 1 {#top-ix-s5-def-1 .statement}

*A subset $ A $ of a topological space $ X $ is said to be nowhere dense if its closure has no interior points.*

Equivalently, $ A $ is nowhere dense in $ X $ if and only if the exterior of $ A $ is dense in $ X $.

A closed set $ A $ is nowhere dense if and only if it has no interior points; that is, if and only if it coincides with its frontier. An arbitrary subset $ A $ is nowhere dense if and only if the closure of $ A $ is nowhere dense. Every subset of a nowhere dense set is nowhere dense.

#### Example 1 {#top-ix-s5-n1-exa-1 .statement}

The empty subset of $ X $ is nowhere dense. In a Hausdorff space $ X $, a set consisting of a single point is nowhere dense if and only if the point is not isolated in $ X $. A dense subset is never nowhere dense (unless $ X = \emptyset $).

#### Example 2 {#top-ix-s5-n1-exa-2 .statement}

The frontier of an open or of a closed set is always nowhere dense.

#### Example 3 {#top-ix-s5-n1-exa-3 .statement}

In the space $ \mathbf{R}^n $, every linear subspace of dimension $ p < n $ is a nowhere dense set (Chapter VI, § 1, no. 4, Proposition 2).

#### Remark {#top-ix-s5-n1-rem-1 .statement}

The frontier of an arbitrary subset need not be nowhere dense: for example, if $ A $ and $ \overline{C}A $ are both dense sets, then the frontier of $ A $ is the whole space.

#### Proposition 1 {#top-ix-s5-prop-1 .statement}

*The union of a finite number of nowhere dense sets is nowhere dense.*

It is enough to show that the union of two nowhere dense sets $ A, B $ is nowhere dense, and without loss of generality we may assume that $ A $ and $ B $ are closed. The proposition is then equivalent to saying that the intersection of two dense open sets $ \overline{C}A, \overline{C}B $ is dense. Now if $ U $ is a non-empty open set, then $ U \cap \overline{C}A $ is open and non-empty, hence

$$
(U \cap \overline{C}A) \cap \overline{C}B = U \cap (\overline{C}A \cap \overline{C}B)
$$

is open and non-empty.

Let $ Y $ be a subspace of a topological space $ X $. A subspace $ A $ of $ Y $ is said to be *nowhere dense relative to* $ Y $ if $ A $ is nowhere dense when considered as a subset of the topological space $ Y $.

#### Proposition 2 {#top-ix-s5-prop-2 .statement}

*Let $ Y $ be a subspace of a topological space $ X $, and let $ A $ be a subset of $ Y $. If $ A $ is nowhere dense relative to $ Y $, then $ A $ is nowhere dense relative to $ X $. Conversely, if $ Y $ is open in $ X $ and $ A $ is nowhere dense relative to $ X $, then $ A $ is nowhere dense relative to $ Y $.*

Suppose that $ A $ is nowhere dense relative to $ Y $. If the closure $ \overline{A} $ of $ A $ in $ X $ contains a non-empty open set $ U $, then $ U \cap A $ is not empty (by the definition of closure); hence $ U \cap Y $ is a non-empty open set relative to $ Y $, and is contained in the closure $ \overline{A} \cap Y $ of $ A $ with respect to $ Y $, which is contrary to the hypothesis.

Now suppose that $ Y $ is open in $ X $ and that $ A \subset Y $ is nowhere dense relative to $ X $. If $ U $ is open in $ Y $ and is not empty, then $ U $ is open in $ X $ and therefore contains a non-empty set $ V $ which is open in $ X $ (and *a fortiori* in $ Y $) and does not meet $ A $; hence $ A $ is nowhere dense relative to $ Y $.

The second part of Proposition 2 is clearly not valid if $ Y $ is not open in $ X $; consider, e.g., the situation where $ Y \neq \emptyset $ is nowhere dense in $ X $, and $ A = Y $.

### 2. MEAGRE SETS

#### Definition 2 {#top-ix-s5-def-2 .statement}

*A subset* $ A $ *of a topological space* $ X $ *is said to be meagre if it is the union of a countable family of nowhere dense sets.*

Equivalently, $ A $ is meagre if it is contained in a countable union of closed sets each of which has no interior points.

A meagre set can perfectly well be *dense* in $ X $; even the whole space $ X $ can itself be a meagre set.

An example of the latter possibility is provided by any *countable* Hausdorff space with no isolated points, e.g., the rational line $ \mathbf{Q} $. But a topological space $ X $ which is a meagre set in $ X $ need not be countable (see Exercise 9).

Every subset of a meagre set in a space $ X $ is meagre, and the union of a *countable* family of meagre sets is meagre.

Let $ Y $ be a subspace of $ X $. A subset $ A $ of $ Y $ is said to be *meagre relative to* $ Y $ if $ A $ is meagre when considered as a subset of the topological space $ Y $. It follows from Proposition 2 of no. 1 that if $ A $ is a subset of $ Y $ which is meagre relative to $ Y $, then $ A $ is meagre relative to $ X $; and that if also $ Y $ is *open* in $ X $, every subset $ A $ of $ Y $ which is meagre relative to $ X $ is meagre relative to $ Y $.

### 3. BAIRE SPACES

#### Definition 3 {#top-ix-s5-def-3 .statement}

*A topological space* $ X $ *is said to be a Baire space if it satisfies one or the other of the following two equivalent conditions:*

*(EB)* *Every countable intersection of dense open sets in* $ X $ *is dense in* $ X $.
*(EB')* *Every countable union of closed sets with no interior points in* $ X $ *has no interior point in* $ X $.

Axiom (EB) can be stated in two other equivalent forms:

*(EB'')* *Every non-empty open set in* $ X $ *is non-meagre.*

Indeed a set is meagre if and only if it is contained in a countable union of closed sets with no interior points.

(EB'') *The complement of a meagre set in $ X $ is dense in $ X $.*

This signifies that a meagre set cannot contain a non-empty open set, and is therefore equivalent to (EB").

#### Proposition 3 {#top-ix-s5-prop-3 .statement}

*Every non-empty open subspace $ Y $ of a Baire space $ X $ is a Baire space.*

This follows from (EB"), for every open (resp. meagre) set in $ Y $ is open (resp. meagre) in $ X $.

It follows from Proposition 3 that every point of a Baire space has a fundamental system of neighbourhoods, each of which is a Baire space. Conversely:

#### Proposition 4 {#top-ix-s5-prop-4 .statement}

*If every point of a topological space $ X $ has a neighbourhood which is a Baire space, then $ X $ is a Baire space.*

Let $ A $ be a non-empty open set in $ X $, let $ x \in A $ and let $ V $ be an open neighbourhood of $ x $ which is a Baire space. If $ A $ were meagre in $ X $, then $ V \cap A $ would be meagre in $ V $ and open in $ V $, which is contrary to hypothesis.

#### Proposition 5 {#top-ix-s5-prop-5 .statement}

*In a Baire space $ X $, the complement of a meagre set is a Baire space.*

Let $ A $ be a meagre set in $ X $; then its complement $ Y = \complement_A $ in $ X $ is dense in $ X $. Let $ B $ be a meagre set relative to $ Y $; $ B $ is also meagre relative to $ X $, hence $ A \cup B $ is meagre relative to $ X $. Hence the complement of $ A \cup B $ in $ X $, which is also the complement of $ B $ in $ Y $, is dense in $ X $ and *a fortiori* dense in $ Y $. Hence $ Y $ is a Baire space.

#### Theorem 1 (Baire) {#top-ix-s5-thm-1 .statement}

(i) *Every locally compact space $ X $ is a Baire space.* (ii) *Every topological space $ X $ on which there exists a metric, compatible with the topology of $ X $ and which defines on $ X $ the structure of a complete metric space, is a Baire space.*

We shall show that axiom (EB) is satisfied in each case. Let $ (A_n) $ be a sequence of dense open sets in $ X $, and let $ G $ be any non-empty open set. We can then define inductively a sequence $ (G_n) $ of non-empty open sets such that $ G_1 = G $ and $ \overline{G}_{n+1} \subset G_n \cap A_n $: for since by hypothesis $ G_n $ is not empty, $ G_n \cap A_n $ is a non-empty open set; and since $ X $ is *regular* in both cases envisaged, there is a non-empty open set $ G_{n+1} $ such that $ \overline{G}_{n+1} \subset G_n \cap A_n $. Hence the set $ G \cap \bigcap_{n=1}^\infty A_n $ contains the intersection of the sets $ G_n $, which is equal to the intersection of the sets $ \overline{G}_n $; hence it is enough to show that $ \bigcap_{n=1}^\infty \overline{G}_n \neq \varnothing $. Now if $ X $ is locally compact, we may assume that $ \overline{G}_2 $ is compact; in the compact space $ \overline{G}_2 $, the $ \overline{G}_n (n \geq 2) $ form a decreasing sequence of non-empty closed sets, and their intersection is therefore not empty by axiom (C'') (cf. Chapter I, § 9, no. 1, Definition 1]. If $ X $ is a complete metric space (with respect to a metric compatible with its topology) we may suppose that $ \overline{G}_n $ has been chosen so that its diameter (with respect to this metric) tends to 0 as $ n $ tends to $ +\infty $; the $ \overline{G}_n $ therefore form a Cauchy filter base which converges to a point $ x $, and $ x $ necessarily belongs to the intersection of the sets $ \overline{G}_n $.

Q.E.D.

#### Remark {#top-ix-s5-n3-rem-1 .statement}

There are Baire spaces which belong to neither of these two categories, in particular Baire spaces which are neither metrizable nor locally compact (Exercise 16); there are also metrizable Baire spaces which possess no complete metric space structure compatible with their topology (Exercise 14).

### 4. SEMI-CONTINUOUS FUNCTIONS ON A BAIRE SPACE

#### Theorem 2 {#top-ix-s5-thm-2 .statement}

Let $ X $ be a Baire space and let $ (f_\alpha) $ be a family of lower semi-continuous real-valued functions on $ X $ such that, at every point $ x $ of $ X $, the upper envelope $ \sup_\alpha f_\alpha(x) $ is finite. Then every non-empty open set in $ X $ contains a non-empty open set on which the family $ (f_\alpha) $ is uniformly bounded above.

This theorem may also be stated in the form that the set of points in the neighbourhood of which the family $ (f_\alpha) $ is uniformly bounded above is a dense open set.

Let $ f = \sup_\alpha f_\alpha $ be the upper envelope of the family $ (f_\alpha) $. The function $ f $ is lower semi-continuous (Chapter IV, § 6, no. 2, Theorem 4) and finite at every point of $ X $. It is therefore enough to carry through the proof in the case where the family $ (f_\alpha) $ consists of a single function $ f $. Let $ A_n $ be the set of points $ x \in X $ such that $ f(x) \leq n $; $ A_n $ is closed (Chapter IV, § 6, no. 2, Proposition 1), and the assumptions imply that $ X $ is the union of the sets $ A_n $; hence at least one of the $ A_n $ has an interior point, and therefore there is a non-empty open set on which $ f $ is bounded above (by an integer $ n $). If we apply this result to any non-empty open subset of $ X $ (this subspace is also a Baire space by Proposition 3 of no. 3), we have the theorem.

In applications of this theorem it is generally the case that the $ f_\alpha $ are continuous on $ X $.

#### Remark {#top-ix-s5-n4-rem-1 .statement}

The theorem may be false if we do not suppose that $ X $ is a Baire space. For example if, for each rational number $ p/q $ ($ p, q $ being coprime integers, $ q > 0 $) we put $ f(p/q) = q $, we have a lower semi-continuous function $ f $ on the rational line $ Q $ which is finite at each point (cf. Chapter IV, § 6, no. 2); but there is no non-empty open set in $ Q $ on which $ f $ is bounded above.

### Exercises {#top-ix-s5-exercises}

See the [exercises for § 5](exercises/s5/).
