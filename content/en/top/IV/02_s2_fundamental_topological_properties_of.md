---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 2
section_title: Fundamental topological properties of the real line
lang: en
source: top-i-iv
pdf_pages: 0340-0345, 0387-0393
extraction: ocr
subsections:
    - "no": 1
      title: ARCHIMEDES' AXIOM
      page: 0
      pdf_page: 340
    - "no": 2
      title: COMPACT SUBSETS OF $ \mathbf{R} $
      page: 0
      pdf_page: 341
    - "no": 3
      title: LEAST UPPER BOUND OF A SUBSET OF $ \mathbf{R} $
      page: 0
      pdf_page: 341
    - "no": 4
      title: CHARACTERIZATION OF INTERVALS
      page: 0
      pdf_page: 342
    - "no": 5
      title: CONNECTED SUBSETS OF $ \mathbf{R} $
      page: 0
      pdf_page: 342
    - "no": 6
      title: HOMEOMORPHISMS OF AN INTERVAL ONTO AN INTERVAL
      page: 0
      pdf_page: 344
statements: 10
exercises: 5
content_sha256: dca95919ad00007573bfd19893426aad9a8925afb87ee65f63ef2ddd5c547808
---

## 2. FUNDAMENTAL TOPOLOGICAL PROPERTIES OF THE REAL LINE

### 1. ARCHIMEDES' AXIOM

The topological properties of the real line which are the subject of this section are all consequences of the following theorem:

#### Theorem 1 {#top-iv-s2-thm-1 .statement}

*If $x$ and $y$ are any two real numbers > 0, then there is an integer $n > 0$ such that $y < nx$.*

There exist two rational numbers $ p/q $ and $ r/s $ such that $ 0 < p/q < x $ and $ y < r/s $, since the open intervals ]$ 0, x $ and ]$ y, \to $ are not empty ($ \S $ I, no. 4, Proposition 4); take $ n $ such that $ nps > qr $, and we have $ y < nx $.

#### Remark {#top-iv-s2-n1-rem-1 .statement}

An axiomatic construction of the theory of real numbers will be found in Chapter V, $ \S $ 2, in which Theorem 1 appears as an axiom; for more details about this axiom, see the Historical Note to Chapter IV.

### 2. COMPACT SUBSETS OF $ \mathbf{R} $

Theorem 2 (Borel-Lebesgue). For a subset of the real line $ \mathbf{R} $ to be compact it is necessary and sufficient that it be closed and bounded.

1) The condition is necessary. Let $ A $ be a compact subset of $ \mathbf{R} $ and let $ a $ be a real number $ > 0 $. The set $ A $ is closed (Chapter I, $ \S $ 9, no. 3, Proposition 4) and there exists a finite number of points $ x_i $ ($ 1 \leq i \leq n $) of $ \mathbf{R} $ such that $ A $ is contained in the union of the neighbourhoods $[x_i - a, x_i + a]$ (Chapter I, $ \S $ 9, no. 3). Let $ b $ be the maximum of the numbers $ |x_i| $; then we have $ A \subset [-b - a, b + a] $.

2) The condition is sufficient. It is enough to show that every interval $[ -a, +a ]$ ($ a > 0 $) is compact, and since this interval is a closed subset of a complete uniform space, it is enough to show that, for each $ b > 0 $, we can cover $[ -a, +a ]$ by a finite number of intervals of the form $[x - b, x + b]$ (Chapter II, $ \S $ 4, no. 2, Corollary to Theorem 3). Now, let $ n $ be an integer $ > 0 $ such that $ a < nb $; if $ x \in [ -a, +a ] $ and if $ m $ is the largest integer (positive or negative) such that $ mb \leq x $, then we have $ -n \leq m \leq n $ and $ mb \leq x \leq (m + 1)b $. Hence the $ 2n + 1 $ intervals $[ (k - 1)b, (k + 1)b ]$ ($ -n \leq k \leq n $) form a covering of the required type.

Corollary 1. A subset of the real line $ \mathbf{R} $ is relatively compact if and only if it is bounded.

Corollary 2. The real line is a locally compact space and is not compact.

#### Remark {#top-iv-s2-n2-rem-1 .statement}

Theorem 2 is often referred to as the "Heine-Borel Theorem"; see the Historical Notes to Chapters II and IV.

### 3. LEAST UPPER BOUND OF A SUBSET OF $ \mathbf{R} $

Theorem 3. Every non-empty subset of the real line which is bounded above (resp. bounded below) has a least upper bound (resp. greatest lower bound).

Let $ A $ be a non-empty subset of $ \mathbf{R} $, bounded above, and let $ b $ be an upper bound of $ A $, so that $ A \subset ]\leftarrow, b] $. For each $ x \in A $ consider the set $ A_x $ of numbers $ \geqslant x $ which belong to $ A $; the sets $ A_x $ form a filter base $ \mathcal{B} $ on $ \mathbf{R} $, since $ A_y \subset A_x $ if $ y \geqslant x $. Let $ a $ be a point of $ A $. For each $ x \geqslant a $ belonging to $ A $, $ A_x $ is contained in the compact interval $[a, b]$ and thus the filter base $ \mathcal{B} $ has a cluster point $ c $. Since the intervals $[x, \rightarrow[$ are closed, $ c $ belongs to their intersection and therefore $ c $ is an upper bound of $ A $. But, on the other hand, every upper bound $ z $ of $ A $ is $ \geqslant c $, otherwise the neighbourhood $ ]z, \rightarrow[ $ of $ c $ would not contain any point of $ A $. Hence $ c $ is the least upper bound of $ A $.

We can argue similarly for a non-empty set $ B $ bounded below, or else simply remark that $-B$ is non-empty and bounded above, and that if $ c $ is the least upper bound of $-B$, then $-c$ is the greatest lower bound of $ B $.

The least upper bound $ c $ of $ A $ can be characterized by the following two properties:
(i) For each $ x \in A, x \leqslant c_* $.
(ii) For each $ a < c $, there exists $ x \in A $ such that $ a < x \leqslant c $.

The least upper bound of a closed set (non-empty and bounded above) belongs to the set and is its greatest element; and the least upper bound of any non-empty subset $ A $ of $ \mathbf{R} $ which is bounded above may be defined as the largest real number in the closure of $ A $.

### 4. CHARACTERIZATION OF INTERVALS

#### Proposition 1 {#top-iv-s2-prop-1 .statement}

*A non-empty subset $ A $ of $ \mathbf{R} $ is an interval if and only if, whenever $ a $ and $ b $ are any two points of $ A $ such that $ a < b $, the closed interval $[a, b]$ is contained in $ A $*.

The condition is clearly necessary. Conversely, suppose that it is satisfied. If $ A $ is neither bounded above nor below it must be the whole of $ \mathbf{R} $, for if $ x $ is any point of $ \mathbf{R} $ there are then two points $ a, b $ of $ A $ such that $ a < x < b $. If $ A $ is bounded above but not below, let $ k $ be its least upper bound; then for any $ x < k $ there exist $ a $ and $ b $ in $ A $ such that $ a < x < b \leqslant k $, hence $ x \in A $, and therefore $ A $ can only be one of the two intervals $ ]\leftarrow, k], ]\leftarrow, k[ $. The argument is similar in the other cases.

### 5. CONNECTED SUBSETS OF $ \mathbf{R} $

#### Theorem 4 {#top-iv-s2-thm-4 .statement}

*A subset $ A $ of $ \mathbf{R} $ is connected if and only if $ A $ is an interval.*

i) The condition is necessary. Suppose that $ A $ is connected: if $ A $ consists of a single point, it is an interval. If $ A $ has more than one point, let $ a $ and $ b $ be two points of $ A $ such that $ a < b $; by Proposition 1 of no. 4 it is enough to show that every $ x $ such that $ a < x < b $ belongs to $ A $. Now, if $ x \notin A $ we should have $ A \subset C\{x\} $; but $ C\{x\} $ is the union of two disjoint open sets ]$ \leftarrow, x[ $ and $ ]x, \rightarrow[ $, each of which meets $ A $, and therefore $ A $ would not be connected, contrary to hypothesis.

2) The condition is *sufficient*. Let us show first that every *compact* interval $[a, b]$ is connected. For each integer $ n > 0 $, let $ V_{1/n} $ be the entourage consisting of all pairs $(x, y)$ such that $ |x - y| \leq 1/n $; by Proposition 6 of Chapter II, § 4, no. 4, it is enough to show that every pair of points $ x, y $ of $[a, b]$ can be joined by a $ V_{1/n} $-chain. Let $ p $ be the greatest integer such that $ p/n \leq x $ and let $ q $ be the greatest integer such that $ q/n \leq y $ ($ p $ and $ q $ exist by reason of Theorem 1 of no. 1); then $ p \leq q $. If $ p = q $ then $ y - x < 1/n $ and the points $ x $ and $ y $ form a $ V_{1/n} $-chain. If $ q > p $, put $ x_i = (p + i)/n $ ($ i = 1, 2, \ldots, q - p $); we have $ x_1 - x \leq 1/n $, $ y - x_{q-p} \leq 1/n $ and $ x_{i+1} - x_i = 1/n $, hence the points $ x, x_1, x_2, \ldots, x_{q-p}, y $ form a $ V_{1/n} $-chain joining $ x $ and $ y $.

If now $ I $ is any interval not consisting of a single point, and if $ a $ and $ b $ are any two points of $ I $ such that $ a < b $, then the interval $[a, b]$ is contained in $ I $ and is connected, and hence $ I $ is connected.

#### Corollary 1 {#top-iv-s2-thm-4-cor-1 .statement}

*The real line is a connected and locally connected space.*

#### Corollary 2 {#top-iv-s2-thm-4-cor-2 .statement}

*The only compact connected subsets of $ \mathbf{R} $ are the bounded closed intervals.*

By Theorem 4, a subset of $ \mathbf{R} $ which does not contain any interval consisting of more than one point is *totally disconnected*; this is true, for example, of the set $ \mathbf{Q} $ of rational numbers, since the set $ C\mathbf{Q} $ of irrational numbers is dense in $ \mathbf{R} $.

#### Proposition 2 {#top-iv-s2-prop-2 .statement}

*Every non-empty open set in $ \mathbf{R} $ is the union of a countable family of mutually disjoint open intervals.*

Let $ A $ be a non-empty open set in $ \mathbf{R} $. Since $ \mathbf{R} $ is locally connected, every *component* of $ A $ is a connected open set (Chapter I, § 11, no. 6, Proposition 11) and therefore an *open interval* by Theorem 4. Any two of these open intervals are disjoint; on the other hand, each of them contains a rational number; hence the set of these intervals has a power less than or equal to that of $ \mathbf{Q} $, i.e. is *countable*.

It follows that every closed set in $ \mathbf{R} $ is the complement of the union of a (finite or infinite) sequence $ (I_n) $ of mutually disjoint open intervals. These intervals are said to be *contiguous* to the closed set under consideration. Conversely, given such a sequence of intervals, the complement of their union is a closed set to which these intervals are contiguous.

#### Example {#top-iv-s2-n5-exa-1 .statement}

Let us define by induction a countable family $ (I_{n,p}) $ of mutually disjoint open intervals as follows:
The integer $ n $ takes all values $ \geqslant 0 $, and for each value of $ n $, $ p $ takes the values $ 1, 2, 3, \ldots, 2^n $. All the intervals $ I_{n,p} $ are contained in
$$
A = [0, 1],
$$
and we take $ I_{0,1} = ]1/3, 2/3[ $ (the "middle third" of $ ]0, 1[ $). Suppose now that the $ 2^{m+1} - 1 $ intervals $ I_{n,p} $ have been defined for $ 0 \leq n \leq m $ in such a way that, if $ J_m $ is their union, the set $ A \cap \complement J_m $ is the union of $ 2^{m+1} $ mutually disjoint closed intervals $ K_{m,p} $ ($ 1 \leq p \leq 2^{m+1} $) each of length $ \frac{1}{3^{m+1}} $. If $ K_{m,p} = [a, b] $ we then take $ I_{m+1,p} $ to be the open interval $ \left[ a + \frac{b-a}{3}, \frac{b-a}{3} \right] $ (the "middle third" of the interval $ ]a, b[ $), and it is immediately verified that the induction can continue in this way (Fig. 3).

![Diagram showing intervals I_{2,1}, I_{1,1}, I_{2,2}, I_{0,1}, I_{2,3}, I_{1,2}, I_{2,4} and corresponding intervals K_{2,1}, K_{2,2}, K_{2,3}, K_{2,4}, K_{1,1}, K_{1,2}, K_{1,3}, K_{1,4}, K_{0,1}, K_{0,2}](https://i.imgur.com/3Q5z5QG.png)

Figure 3.

If $ K' $ is the complement of the union of the $ I_{n,p} $, the closed set $ K = A \cap K' $ is called Cantor's triadic set. Clearly $ K $ is compact (no. 2, Theorem 2); also $ K $ is totally disconnected. For if $ K $ contained an interval $ I $ of length $ > 0 $, then $ I $ would be contained in some interval $ K_{m,p} $; hence its length would be $ \leq 1/3^{m+1} $ for each $ m $, which is absurd.

### 6. HOMEOMORPHISMS OF AN INTERVAL ONTO AN INTERVAL

Theorem 5. *Let I be an interval in R. Then a mapping f of I into R is a homeomorphism of I onto f(I) if and only if f is strictly monotonic and continuous on I; and f(I) is then an interval in R.*

1) The condition is necessary. Let $ a $ and $ b $ be two points of I such that $ a < b $, and suppose for example that $ f(a) < f(b) $. Let us show that $ f $ is strictly increasing on I. First, if $ a < c < b $ then we must have $ f(a) < f(c) < f(b) $; if, for example, we had $ f(a) < f(b) < f(c) $

It follows that if $x$ and $y$ are any two points of I such that $x < y$, then $f(x) < f(y)$; for we have $f(a) < f(x) < f(b)$ if $a < x < b$, $f(a) < f(b) < f(x)$ if $b < x$, and $f(x) < f(a) < f(b)$ if $x < a$; repeating the argument with $a, x, y$ in place of $a, b, x$ respectively, we see that $f(x) < f(y)$.

2) The condition is *sufficient*. Suppose that $f$ is continuous and strictly monotonic on I (say, strictly increasing): $f(I)$ is connected and is therefore an interval, and since $f$ is strictly increasing, $f$ is a bijective mapping of I onto $f(I)$. Moreover, the image under $f$ of an open interval *in* I is an open interval *in* $f(I)$, and therefore (\$1, no, 4, Proposition 5) $f$ is a homeomorphism of I onto $f(I)$.

#### Remark {#top-iv-s2-n6-rem-1 .statement}

The first part of the preceding proof shows in fact that a *continuous injective* mapping of I into $\mathbf{R}$ is strictly monotonic; from the second part of the proof it therefore follows that *every continuous injective mapping* $f$ *of an interval* I *into* $\mathbf{R}$ *is a homeomorphism of* I *onto* $f(I)$.

### Exercises {#top-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
