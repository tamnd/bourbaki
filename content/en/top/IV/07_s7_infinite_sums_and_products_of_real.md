---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 7
section_title: Infinite sums and products of real numbers
lang: en
source: top-i-iv
pdf_pages: 0369-0378, 0403-0407
extraction: ocr
subsections:
    - "no": 1
      title: FAMILIES OF POSITIVE FINITE NUMBERS SUMMABLE IN $ \mathbf{R} $
      page: 0
      pdf_page: 370
    - "no": 2
      title: FAMILIES OF FINITE NUMBERS OF ARBITRARY SIGN SUMMABLE IN $ \mathbf{R} $
      page: 0
      pdf_page: 372
    - "no": 3
      title: PRODUCT OF TWO INFINITE SUMS
      page: 0
      pdf_page: 373
    - "no": 4
      title: FAMILIES MULTIPLIABLE IN $ \mathbf{R}^* $
      page: 0
      pdf_page: 373
    - "no": 5
      title: SUMMABLE FAMILIES AND MULTIPLIABLE FAMILIES IN $ \overline{\mathbf{R}} $
      page: 0
      pdf_page: 375
    - "no": 6
      title: INFINITE SERIES AND INFINITE PRODUCTS OF REAL NUMBERS
      page: 0
      pdf_page: 376
statements: 20
exercises: 11
content_sha256: 2663d8c219d754cff4afb607087a87f701e934fe8051cc66b900cf47a8e1cea4
---

## 7. INFINITE SUMS AND PRODUCTS OF REAL NUMBERS

Since every point of $ \mathbf{R} $ has a *countable* fundamental system of neighbourhoods (§ 1, no. 4, Corollary to Proposition 3), it follows that a family $ (x_t) $ of *finite* real numbers is summable in $ \mathbf{R} $ only if the set of indices t such that $ x_t \neq 0 $ is *countable* (Chapter III, § 5, no. 2, Corollary to Proposition 1). The study of summable families in $ \mathbf{R} $ thus reduces essentially to the study of summable *sequences*. However, we shall later have to consider uncountable families $ (x_t) $ of finite real numbers, whose terms are functions of a parameter $ t $; it can happen that this family is summable for all $ t $, but that the (countable) set of indices $ i $ such that $ x_i \neq 0 $ depends on $ t $. For this reason we shall not impose any hypothesis on the power of the index set in what follows.

### 1. FAMILIES OF POSITIVE FINITE NUMBERS SUMMABLE IN $ \mathbf{R} $

#### Theorem 1 {#top-iv-s7-thm-1 .statement}

*A family* $ (x_i) $ *of finite real numbers* $ \geqslant 0 $ *is summable in* $ \mathbf{R} $ *if and only if the set of partial finite sums of the family is bounded above in* $ \mathbf{R} $. *If so, the least upper bound of this set is the sum of the family* $ (x_i) $.

For each finite subset $ H $ of the index set $ I $, let $ s_H = \sum_{i \in H} x_i $; since the $ x_i $ are $ \geqslant 0 $, the relation $ H \subset H' $ implies $ s_H \leqslant s_{H'} $. In other words, the mapping $ H \to s_H $ is an *increasing* function on the directed set $ \mathfrak{F}(I) $ of finite subsets of $ I $; therefore (\$ 5, no. 2, Corollary to Theorem 2) it has a finite limit if and only if it is *bounded above*.

#### Remark {#top-iv-s7-n1-rem-1 .statement}

Let $ (H_\lambda) $ be a family of finite subsets of $ I $ such that, for each finite subset $ H $ of $ I $, there is an index $ \lambda $ such that $ H \subset H_\lambda $; then $ (x_i) $ is summable if and only if the family of the $ s_{H_\lambda} $ is *bounded above* in $ \mathbf{R} $. In particular, let $ (x_n) $ be a sequence of finite real numbers $ \geqslant 0 $, and for each integer $ n $ let $ s_n = \sum_{p=0}^n x_p $; then the sequence $ (x_n) $ is summable in $ \mathbf{R} $ if and only if, for *one sequence* of strictly increasing integers $ (n_k) $, the partial sequence $ (s_{n_k}) $ is *bounded above* in $ \mathbf{R} $.

*Examples.* 1) For each number $ q $ such that $ 0 \leqslant q < 1 $, the sequence $ (q^n) $ ("geometric progression of ratio $ q $") is summable in $ \mathbf{R} $, since
$$
s_n = \frac{1 - q^{n+1}}{1 - q} \leqslant \frac{1}{1 - q}
$$
the sum of this sequence is $ \lim_{n \to \infty} s_n = \frac{1}{1 - q} $.

2) Let $ a $ and $ b $ be two numbers such that $ 0 \leqslant a < 1 $ and $ 0 \leqslant b < 1 $; then the family $ (a^m b^n)_{(m, n) \in \mathbf{N} \times \mathbf{N}} $ is summable in $ \mathbf{R} $. For each finite subset of $ \mathbf{N} \times \mathbf{N} $ is contained in a subset of the form $ [0, p] \times [0, p] $, and we have
$$
\sum_{m=0}^p \sum_{n=0}^p a^m b^n = \left( \sum_{m=0}^p a^m \right) \left( \sum_{n=0}^p b^n \right) = \frac{1 - a^{p+1}}{1 - a} \cdot \frac{1 - b^{p+1}}{1 - b} \leqslant \frac{1}{(1 - a)(1 - b)}.
$$

3) For each integer $ p > 1 $, the sequence $ (n^{-p}) $ ($ n > 0 $) is summable, since
$$
s_{2^n + 1} - s_{2^n} = \sum_{k=1}^{2^n} (2^n + k)^{-p} < 2^n \cdot (2^n)^{-p}
$$
and therefore, adding these inequalities together,
$$
s_{2^n} < \frac{1}{1 - 2^{1-p}}.
$$

4) The sequence $ (1/n) $ ($ n > 0 $) is not summable in $ \mathbf{R} $, since
$$
s_{2^{n+1}} - s_{2^n} = \sum_{k=1}^{2^n} \frac{1}{2^n + k} > \frac{2^n}{2^{n+1}} = \frac{1}{2}
$$
and therefore, adding these inequalities together,
$$
s_{2^n} > n/2
$$
so that the criterion of Theorem 1 is not satisfied.

5) Let $ (I_n) $ be a sequence of mutually disjoint non-empty open intervals, all contained in an interval of finite length $ l $. The sum of the lengths of a finite number of intervals of this family is $ \leq l $ ($ \S 1 $, no. 5) and therefore the family of lengths of the $ I_n $ is summable in $ \mathbf{R} $, and its sum is $ \leq l $.

#### Theorem 2 (Principle of comparison) {#top-iv-s7-thm-2 .statement}

*Let* $ (x_i)_{i \in I} $ *and* $ (y_i)_{i \in I} $ *be two families of finite real numbers* $ \geq 0 $, *such that* $ x_i \leq y_i $ *for all* $ i $. *If* $ (y_i) $ *is summable in* $ \mathbf{R} $ *then so is* $ (x_i) $, *and we have* $ \sum_i x_i \leq \sum_i y_i $; *if in addition there is an index* $ x $ *such that* $ x_x < y_x $, *then* $ \sum_i x_i < \sum_i y_i $.

The hypothesis implies that,
$$
\sum_{i \in H} x_i \leq \sum_{i \in H} y_i,
$$
for every finite subset $ H $ of $ I $ and the first part of the theorem follows from this; the inequality relating the sums follows from the principle of extension of inequalities ($ \S 5 $, no. 2, Theorem 1). If $ x_x < y_x $, then
$$
\sum_i x_i = x_x + \sum_{i \neq x} x_i < y_x + \sum_{i \neq x} y_i = \sum_i y_i.
$$

This theorem provides the most commonly used criterion for deciding whether or not a sequence $ (x_n) $ of real numbers $ \geq 0 $ is summable in $ \mathbf{R} $: we try to *compare* the given sequence with a simpler sequence $ (y_n) $ of which we already know whether it is summable or not. If there exists a finite number $ a > 0 $ such that $ x_n \leq a y_n $ for all $ n $ from a certain point onwards, and if $ (y_n) $ is summable, then $ (x_n) $ is summable; if on the other hand there is a finite number $ b > 0 $ such that $ x_n \geq b y_n $ for all $ n $ from a certain point onwards, and if $ (y_n) $ is not summable in $ \mathbf{R} $, then $ (x_n) $ is not summable in $ \mathbf{R} $. We shall see in a later volume how such comparison sequences may be obtained in the cases which arise most frequently.

#### Example 1 {#top-iv-s7-n1-exa-1 .statement}

Let $ a $ be a finite real number $ > 0 $, and consider the sequence $ \left( \frac{a^n}{n!} \right) $; let $ n_0 $ be the smallest integer such that $ a < n_0 $. Then for each $ n \geq n_0 $ we have
$$
\frac{a^n}{n!} \leq \frac{a^{n_0}}{n_0!} \cdot \left( \frac{a}{n_0} \right)^{n-n_0};
$$
since $ q = \frac{a}{n_0} < 1 $, the sequence $ (q^{n-n_0}) $ is summable, and therefore so is the sequence $ \left( \frac{a^n}{n!} \right) $.

#### Example 2 {#top-iv-s7-n1-exa-2 .statement}

Let $ (a_n) $ be a summable sequence of positive numbers. Since
$$
\lim_{n \to \infty} a_n = 0,
$$
there exists an integer $ n_0 $ such that $ a_n \leq 1 $ whenever $ n \geq n_0 $. Consequently, for each $ n \geq n_0 $ we have $ a_n^2 \leq a_n $, and therefore the sequence $ (a_n^2) $ is summable in $ \mathbf{R} $. So is the sequence $ (a_n^p) $ for each integer $ p > 1 $.

#### Example 3 {#top-iv-s7-n1-exa-3 .statement}

Let $ a $ and $ b $ be two numbers $ < 1 $; then
$$
\frac{1}{a^m + b^n} \leq \frac{1}{2(\sqrt{a})^m (\sqrt{b})^n}
$$
and hence the family $ \left( \frac{1}{a^m + b^n} \right) $ is summable in $ \mathbf{R} $.

#### Corollary {#top-iv-s7-n1-cor-1 .statement}

*Let* $ (x_i)_{i \in I} $ *be a summable family of finite numbers* $ \geq 0 $ *in* $ \mathbf{R} $. *If* $ H $ *is any subset of* $ I $, *we have*
$$
\sum_{i \in H} x_i \leq \sum_{i \in I} x_i,
$$
*and equality holds only if* $ x_i = 0 $ *for all* $ i \in \complement H $.

### 2. FAMILIES OF FINITE NUMBERS OF ARBITRARY SIGN SUMMABLE IN $ \mathbf{R} $

#### Theorem 3 {#top-iv-s7-thm-3 .statement}

*Let* $ (x_i)_{i \in I} $ *be a family of finite real numbers; then the following statements are equivalent*:

a) *The family* $ (x_i) $ *is summable in* $ \mathbf{R} $.
b) *The family* $ (|x_i|) $ *is summable in* $ \mathbf{R} $.
c) *The set of finite partial sums of the family* $ (x_i) $ *is bounded in* $ \mathbf{R} $.

Let $ I_1 $ *be the set of all* $ i \in I $ *such that* $ x_i \geq 0 $, *and* $ I_2 $ *the set of all* $ i \in I $ *such that* $ x_i < 0 $. *The family* $ (x_i)_{i \in I} $ *[resp. $ (|x_i|)_{i \in I} $] *is summable if and only if each of the families* $ (x_i)_{i \in I_1} $ *and* $ (x_i)_{i \in I_2} $ *[resp. $ (|x_i|)_{i \in I_1} $ and $ (|x_i|)_{i \in I_2} $] *is summable* (Chapter III, § 5, no. 3, Propositions 2 and 3). *Now it comes to the same thing to say that* $ (x_i)_{i \in I_1} $ *is summable, or that* $ (|x_i|)_{i \in I_1} $ *is summable, or that the set of finite partial sums of the* family $ (x_i)_{i \in I_1} $ is bounded (no. 1, Theorem 1); and the same is true with $ I_1 $ replaced by $ I_2 $. The theorem follows immediately.

Theorem 3 shows that the summability in $ \mathbf{R} $ of a family of finite real numbers depends only on the summability of the family of their absolute values.

We recall (Chapter III, § 5, no. 5, Proposition 6) that if $ (x_i) $ and $ (y_i) $ are two summable families of finite real numbers, then the family $ (x_i + y_i) $ is summable and $ \sum (x_i + y_i) = \sum x_i + \sum y_i $. Moreover, if $ (x_i) $ is a summable family of finite real numbers and $ a $ is any finite real number, then the family $ (ax_i) $ is summable in $ \mathbf{R} $, and we have $ \sum ax_i = a \cdot \sum x_i $.

### 3. PRODUCT OF TWO INFINITE SUMS

#### Proposition 1 {#top-iv-s7-prop-1 .statement}

*If the families* $ (x_\lambda)_{\lambda \in L} $ *and* $ (y_\mu)_{\mu \in M} $ *of finite real numbers are summable in* $ \mathbf{R} $, *then so is the family* $ (x_\lambda y_\mu)_{(\lambda, \mu) \in L \times M} $ *and we have*

(1)
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = (\sum_{\lambda \in L} x_\lambda) (\sum_{\mu \in M} y_\mu).
$$

Every finite subset of $ L \times M $ is contained in a finite subset of the form $ H \times K $, where $ H $ is a finite subset of $ L $ and $ K $ is a finite subset of $ M $. By hypothesis, there exists a number $ a > 0 $ such that $ \sum_{\lambda \in H} |x_\lambda| \leq a $ and $ \sum_{\mu \in K} |y_\mu| \leq a $ for all finite subsets $ H $ and $ K $ of $ L $ and $ M $ respectively; therefore
$$
\sum_{(\lambda, \mu) \in H \times K} |x_\lambda y_\mu| = (\sum_{\lambda \in H} |x_\lambda|) (\sum_{\mu \in K} |y_\mu|) \leq a^2,
$$
and this shows that the family $ (x_\lambda y_\mu) $ is summable in $ \mathbf{R} $, by Theorems 1 and 3. By associativity we can write [Chapter III, § 5, no. 3, formula (2)]
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = \sum_{\lambda \in L} (\sum_{\mu \in M} x_\lambda y_\mu) = \sum_{\lambda \in L} x_\lambda (\sum_{\mu \in M} y_\mu) = (\sum_{\lambda \in L} x_\lambda) (\sum_{\mu \in M} y_\mu);
$$
hence the result.

### 4. FAMILIES MULTIPLIABLE IN $ \mathbf{R}^* $

In the multiplicative group $ \mathbf{R}^* $ of finite non-zero real numbers, a family $ (x_i)_{i \in I} $ can be multipliable only if $ \lim x_i = 1 $ with respect to the filter of complements of finite subsets of $ I $ (Chapter III, § 5, no. 2, Proposition 1). In particular there can be only a *finite* number of indices $ i $ such that $ x_i < 0 $. We may therefore limit ourselves to considering only families $ x_i $ all of whose terms are strictly positive; it is then convenient to put $ x_i = 1 + u_i $, where the $ u_i $ are subject to the inequalities $ -1 < u_i < +\infty $ for all $ i $. Since each point of $ \mathbf{R}^* $ has a countable fundamental system of neighbourhoods, the set of indices $ i $ such that $ u_i \neq 0 $ is countable, if the family $ (1 + u_i) $ is multipliable in $ \mathbf{R}^* $.

#### Theorem 4 {#top-iv-s7-thm-4 .statement}

*The family* $ (1 + u_i) $ *is multipliable in* $ \mathbf{R}^* $ *if and only if the family* $ (u_i) $ *is summable in* $ \mathbf{R} $.
**Lemma.** (i) *If* $ (a_i)_{1 \leq i \leq p} $ *is a finite sequence of numbers* $ > 0 $, *then*
$$
\prod_{i=1}^p (1 + a_i) \geq 1 + \sum_{i=1}^p a_i.
$$
(ii) *If also* $ a_i < 1 $ *for each* $ i $, *then*
$$
\prod_{i=1}^p (1 - a_i) \geq 1 - \sum_{i=1}^p a_i.
$$

These inequalities are clear if $ p = 1 $, and are proved by induction on $ p $. If
$$
\prod_{i=1}^{p-1} (1 + a_i) \geq 1 + \sum_{i=1}^{p-1} a_i,
$$
we have
$$
\prod_{i=1}^p (1 + a_i) \geq (1 + a_p) \left( 1 + \sum_{i=1}^{p-1} a_i \right) = 1 + \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 + \sum_{i=1}^p a_i.
$$
Again, if
$$
\prod_{i=1}^{p-1} (1 - a_i) \geq 1 - \sum_{i=1}^{p-1} a_i,
$$
we have
$$
\prod_{i=1}^p (1 - a_i) \geq (1 - a_p) \left( 1 - \sum_{i=1}^{p-1} a_i \right) = 1 - \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 - \sum_{i=1}^p a_i.
$$

Having proved the lemma, we note that if the family $ (1 + u_i) $ is multipliable then so are the families $ (1 + u_i^+) $ and $ (1 - u_i^-) $, since $ \mathbf{R}^* $ is a complete group (Chapter III, § 5, no. 3, Proposition 2); and conversely, if the families $ (1 + u_i^+) $ and $ (1 - u_i^-) $ are multipliable, then so is $ (1 + u_i) $ (Chapter III, § 5, no. 3, Proposition 3). We need therefore consider only the cases in which all the $ u_i $ are $ \geq 0 $ and in which they are all $ \geq 0 $.

Suppose first that $ u_i \geq 0 $ for all $ i $. If the family $ (1 + u_i) $ is multipliable, then for each $ \varepsilon > 0 $ there is a finite subset $ J $ of the index set in $ I $ such that, for each finite subset $ H $ of $ I $ disjoint from $ J $, we have $ 1 \leq \prod_{i \in H} (1 + u_i) \leq 1 + \varepsilon $; by (2) it follows that $ \sum_{i \in H} u_i \leq \varepsilon $, which shows that $ (u_i) $ is summable in $ \mathbf{R} $ by virtue of Cauchy’s criterion (Chapter III, § 5, no. 2, Theorem 1).

Conversely, suppose that $ (u_i) $ is summable in $ \mathbf{R} $. For each $ \varepsilon $ such that $ 0 < \varepsilon < 1 $, there is a finite subset $ J $ of $ I $ such that, for each finite subset $ H $ of $ I $ disjoint from $ J $, we have $ 0 \leq \sum_{i \in H} u_i \leq \varepsilon $. By (3), we have therefore $ \prod_{i \in H} (1 - u_i) \geq 1 - \varepsilon $; but since $ 1 + u \leq \frac{1}{1 - u} $ for every number $ u $ such that $ 0 \leq u < 1 $, it follows that

$$
1 \leq \prod_{i \in H} (1 + u_i) \leq \frac{1}{1 - \varepsilon},
$$

and this shows that $ (1 + u_i) $ is multipliable (Cauchy’s criterion).

The proof is similar when all the $ u_i $ are $ \leq 0 $. To show that $ (u_i) $ is summable if $ (1 + u_i) $ is multipliable, use formula (2) and the inequality $ 1 - u \leq \frac{1}{1 + u} $ ($ 0 \leq u < 1 $); to show that $ (1 + u_i) $ is multipliable if $ (u_i) $ is summable, use formula (3).

In Chapter V (§ 4), the topological study of the group $ \mathbf{R}^* $ will enable us to give another criterion for multipliability of a family in $ \mathbf{R}^* $ with the help of the logarithmic function; in a later volume we shall establish the equivalence of this criterion with the one above, using the differential properties of the logarithm.

### 5. SUMMABLE FAMILIES AND MULTIPLIABLE FAMILIES IN $ \overline{\mathbf{R}} $

On the interval $[0, + \infty]$ of $ \overline{\mathbf{R}} $, addition is an associative and commutative law of composition (§ 4, no. 3); hence the notion of a *summable* family of numbers in this interval is defined (Chapter III, § 5, no. 1, Remark 3).

#### Proposition 2 {#top-iv-s7-prop-2 .statement}

*Every family* $ (x_i) $ *of real numbers* $ \geq 0 $ *is summable in* $ \overline{\mathbf{R}} $.

For the mapping $ H \to s_H $ of the directed set $ \mathfrak{F}(I) $ into $ \overline{\mathbf{R}} $ is *increasing*; hence (§ 5, no. 2, Theorem 2) has a limit.

The same reasoning shows that every family of real numbers $ \leq 0 $ is summable in $ \overline{\mathbf{R}} $.

Similarly, multiplication is an associative and commutative law of composition on each of the intervals $[0, 1]$ and $[1, + \infty]$ of $ \overline{\mathbf{R}} $, and therefore the notion of a multipliable family is defined on each of these intervals.

#### Proposition 3 {#top-iv-s7-prop-3 .statement}

Every family $ (1 + u_i) $ [resp. $ (1 - u_i) $] of numbers $ \geq 1 $ (resp. $ \geq 0 $ and $ \leq 1 $) is multipliable in $ \overline{\mathbf{R}} $.

Same proof as for Proposition 2.

#### Corollary {#top-iv-s7-n5-cor-1 .statement}

The product $ \prod (1 + u_i) $ [resp. $ \prod (1 - u_i) $] of numbers $ \geq 1 $ (resp. $ > 0 $ and $ \leq 1 $) is equal to $ + \infty $ (resp. 0) if and only if $ \sum u_i = + \infty $.

For if $ \sum u_i $ is finite then $ \prod (1 + u_i) $ and $ \prod (1 - u_i) $ are in $ \mathbf{R}^* $, and conversely (no. 4, Theorem 4).

#### Remark {#top-iv-s7-n5-rem-1 .statement}

The theorem of associativity (Chapter III, § 5, no. 3, Theorem 2) remains valid when G is replaced by $ \overline{\mathbf{R}} $ and the $ x_i $ are assumed to be $ \geq 0 $. This is clear if $ \sum_{i \in I} x_i $ is finite. Suppose, on the contrary, that $ \sum_{i \in I} x_i = + \infty $. Then for each finite $ a > 0 $ there is a finite subset H of I such that $ \sum_{i \in H} x_i \geq a $. Let K be a finite subset of L such that $ H \subset \bigcup_{\lambda \in K} I_\lambda $; then since $ s_\lambda \geq \sum_{i \in I_\lambda \cap H} x_i $ for all $ \lambda \in K $, we have
$$
\sum_{\lambda \in K} s_\lambda \geq \sum_{i \in H} x_i \geq a,
$$
which shows that $ \sum_{\lambda \in L} s_\lambda = + \infty $. We leave to the reader the task of formulating the analogous proposition for multipliable families of numbers in $[0, 1]$ or in $[1, + \infty]$.

### 6. INFINITE SERIES AND INFINITE PRODUCTS OF REAL NUMBERS

A series of finite real numbers is simply said to be convergent if it is convergent in $ \mathbf{R} $.

#### Definition 1 {#top-iv-s7-def-1 .statement}

A series of finite real numbers is said to be absolutely convergent if the series of absolute values of its terms is convergent.

#### Proposition 4 {#top-iv-s7-prop-4 .statement}

A series of finite real numbers is commutatively convergent if and only if it is absolutely convergent.

This follows from Chapter III, § 5, no. 7, Proposition 9 and from Theorem 3 of no. 2.

In other words, if $ (u_n) $ is a sequence of finite real numbers, it comes to the same thing to say that the series whose general term is $ u_n $ is commutatively convergent, or that it is absolutely convergent, or that the sequence $ (u_n) $ is summable in $ \mathbf{R} $. All the properties of summable families proved in Chapter III, § 5 therefore apply to absolutely convergent series. In particular, if the series whose general term is $ u_n $ is absolutely convergent, then the sum $ \sum_{n \in H} u_n $ exists for all subsets $ H $ of $ \mathbf{N} $; and, if $ (H_p) $ is a partition of $ \mathbf{N} $, we have
$$
\sum_{n=0}^{\infty} u_n = \sum_p \left( \sum_{n \in H_p} u_n \right)
$$
*(associativity* of absolutely convergent series).

As we have already remarked in Chapter III, § 5, a series of real numbers can be convergent without being commutatively convergent, that is, without being absolutely convergent.

#### Example {#top-iv-s7-n6-exa-1 .statement}

*Alternating series.* A series defined by a sequence $ (u_n) $ of finite real numbers is called *alternating* if $ u_n = (-1)^n v_n $, where $ v_n \geq 0 $ for all $ n $. Let us show that a *sufficient* condition for the convergence of such a series is that the *sequence* $ (v_n) $ *decreases and has* 0 *as its limit*. For if $ s_n $ denotes
$$
\sum_{p=0}^{n} u_p,
$$
the hypothesis that $ (v_n) $ is decreasing implies that
$$
s_{2n+1} \leq s_{2n+3} \leq s_{2n+2} \leq s_{2n}
$$
for all $ n \geq 0 $. The sequence $ (s_{2n}) $ [resp. $ (s_{2n+1}) $] is decreasing and bounded below (resp. increasing and bounded above) and therefore has a finite limit $ a $ (resp. $ b $), and $ b \leq a $; since
$$
a - b = \lim_{n \to \infty} (s_{2n} - s_{2n+1}) = \lim_{n \to \infty} v_{2n+1} = 0,
$$
the assertion is proved.

If we take for example $ v_n = 1/n $, the conditions above are satisfied, and therefore the series whose general term is $ (-1)^n / n $ (the "alternating harmonic series") is convergent. We have seen in no. 1 that the series whose general term is $ 1/n $ (the "harmonic series") is not convergent, and thus the alternating harmonic series is not absolutely convergent.

We recall (Chapter III, § 5, no. 6, Proposition 7) that, if $ (u_n) $ and $ (v_n) $ are two convergent series of finite real numbers, then the series $ (u_n + v_n) $ is convergent, and
$$
\sum_{n=0}^{\infty} (u_n + v_n) = \sum_{n=0}^{\infty} u_n + \sum_{n=0}^{\infty} v_n;
$$
also, if the series $ (u_n) $ is convergent then the series $ (au_n) $ is convergent for all finite real numbers $ a $, and $ \sum_{n=0}^{\infty} au_n = a \cdot \sum_{n=0}^{\infty} u_n $.

Finally, if the series $(u_n)$ and $(v_n)$ are convergent, and if $u_n \leq v_n$ for all $n$, we have $\sum_{n=0}^{\infty} u_n \leq \sum_{n=0}^{\infty} v_n$ by the principle of extension of inequalities (\S 5, no. 2, Theorem 1).

It should be noted that, if we suppose the series $(v_n)$ to be convergent but not absolutely convergent, and if $|u_n| \leq |v_n|$ for each $n$, we can by no means infer that the series $(u_n)$ is convergent, as is seen by taking $u_n = |v_n|$.

An infinite product of finite non-zero real numbers is said simply to be convergent if it is convergent in $\mathbf{R}^*$; its value is then a finite non-zero real number.

#### Definition 2 {#top-iv-s7-def-2 .statement}

*An infinite product whose general factor is $1 + u_n$ is said to be absolutely convergent if the product whose general factor is $1 + |u_n|$ is convergent.*

#### Proposition 5 {#top-iv-s7-prop-5 .statement}

*An infinite product of finite real numbers is commutatively convergent if and only if it is absolutely convergent.*

This follows from Chapter III, \S 5, no. 7, Proposition 9, and from Theorem 4 above.

Moreover, the product whose general factor is $1 + u_n$ is *absolutely convergent* if and only if the series whose general term is $u_n$ is *absolutely convergent*.

A product of non-zero real numbers can be convergent without being commutatively convergent, i.e. without being absolutely convergent.

#### Example {#top-iv-s7-n6-exa-2 .statement}

If we take $u_{2n-1} = -1/n$ and $u_{2n} = 1/n$ for $n \geq 2$, the product $(1 + u_n)$ is not absolutely convergent, since the series $(u_n)$ is not absolutely convergent; but since

$$
\prod_{p=3}^{n} (1 + u_p) = \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right),
$$
and
$$
\prod_{p=3}^{2n+1} (1 + u_p) = \left(1 - \frac{1}{n+1}\right) \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right),
$$
it follows from Theorem 4 that the product is convergent and that its value is
$$
\prod_{n=2}^{\infty} \left(1 - \frac{1}{n^2}\right).
$$

Moreover, it should be observed that the *convergence* of the series whose general term is $u_n$ *is neither necessary nor sufficient* for the *convergence* of the product whose general factor is $1 + u_n$ (see Exercises 21 and 22).

### Exercises {#top-iv-s7-exercises}

See the [exercises for § 7](exercises/s7/).
