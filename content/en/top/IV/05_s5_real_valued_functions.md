---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 5
section_title: Real-valued functions
lang: en
source: top-i-iv
pdf_pages: 0353-0365, 0395-0399
extraction: ocr
subsections:
    - "no": 1
      title: REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 353
    - "no": 2
      title: REAL-VALUED FUNCTIONS DEFINED ON A FILTERED SET
      page: 0
      pdf_page: 354
    - "no": 3
      title: LIMITS ON THE RIGHT AND ON THE LEFT OF A FUNCTION OF A REAL VARIABLE
      page: 0
      pdf_page: 355
    - "no": 4
      title: BOUNDS OF A REAL-VALUED FUNCTION
      page: 0
      pdf_page: 356
    - "no": 5
      title: ENVELOPES OF A FAMILY OF REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 358
    - "no": 6
      title: UPPER LIMIT AND LOWER LIMIT OF A REAL-VALUED FUNCTION WITH RESPECT TO A FILTER
      page: 0
      pdf_page: 359
    - "no": 7
      title: ALGEBRAIC OPERATIONS ON REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 362
statements: 30
exercises: 6
content_sha256: 3619523eedec18461c8156e453fc7b714426edb1b942c26194e2855e6d24b459
---

## 5. REAL-VALUED FUNCTIONS

### 1. REAL-VALUED FUNCTIONS

#### Definition 1 {#top-iv-s5-def-1 .statement}

A mapping of a set $ X $ into the real line is called a real-valued function (or real function) defined on $ X $.

By an abuse of language analogous to that mentioned in § 4, no. 2, mappings of $ X $ into $ \overline{\mathbf{R}} $ will also be called real-valued functions defined on $ X $ in this and the following section. Mappings of $ X $ into $ \mathbf{R} $ will be called finite real-valued functions.

If $ f $ and $ g $ are two real-valued functions defined on $ X $, the relation $ f \leq g $ is by definition equivalent to "$ f(x) \leq g(x) $ for all $ x \in X $;” this relation is an ordering on the set $ \overline{\mathbf{R}}^X $ of all real-valued functions on $ X $. The set $ \overline{\mathbf{R}},^X $ ordered by this relation, is a lattice; for if $ f $ and $ g $ are any two real-valued functions, the function $ h $ defined by $ h(x) = \sup (f(x), g(x)) $ for all $ x \in X $ is the smallest of the real-valued functions on $ X $ which are both $ \geq f $ and $ \geq g $; in accordance with general notation, we denote this function (which is the least upper bound of $ f $ and $ g $ in $ \overline{\mathbf{R}}^X $) by $ \sup (f, g) $. Similarly, the function whose value at each $ x \in X $ is $ \inf (f(x), g(x)) $ is denoted by $ \inf (f, g) $.

Note that $ \sup (f, g) $ is the composition of the mapping
$$
(u, v) \to \sup (u, v)
$$
of $ \overline{\mathbf{R}} \times \overline{\mathbf{R}} $ into $ \overline{\mathbf{R}} $ and the mapping $ x \to (f(x), g(x)) $ of $ X $ into $ \overline{\mathbf{R}} \times \overline{\mathbf{R}} $. Similarly for $ \inf (f, g) $.

A real-valued function $ f $ defined on a set $ X $ is said to be *bounded above* (resp. *bounded below*) in $ X $, if $ f(X) $ is a subset of $ A'' = [-\infty, +\infty] $ and is bounded above (resp. if $ f(X) $ is a subset of $ A' = ]-\infty, +\infty] $ and is bounded below). $ f $ is said to be *bounded* in $ X $ if it is bounded both above and below, that is if $ f(X) $ is a bounded subset of $ \mathbf{R} $.

Every bounded function is therefore *finite*. The converse is false, as is shown by the function $ 1/x $ on $ \mathbf{R}_+^* = ]0, +\infty[ $.

### 2. REAL-VALUED FUNCTIONS DEFINED ON A FILTERED SET

#### Proposition 1 {#top-iv-s5-prop-1 .statement}

*Let $ f $ and $ g $ be two real-valued functions defined on a set $ X $ filtered by a filter $ \mathfrak{F} $. If $ \lim_{\mathfrak{F}} f $ and $ \lim_{\mathfrak{F}} g $ exist, and if, for each subset $ A \in \mathfrak{F} $, there exists $ x \in A $ such that $ f(x) \leq g(x) $, then we have $ \lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g $.*

To prove this result we shall prove the following equivalent statement:

#### Proposition 2 {#top-iv-s5-prop-2 .statement}

*Let $ f $ and $ g $ be two real-valued functions defined on a set $ X $ filtered by a filter $ \mathfrak{F} $. If $ \lim_{\mathfrak{F}} f $ and $ \lim_{\mathfrak{F}} g $ exist, and if $ \lim_{\mathfrak{F}} f > \lim_{\mathfrak{F}} g $, then there is a set $ A \in \mathfrak{F} $ such that $ f(x) > g(x) $ for all $ x \in A $.*

Let $ a = \lim_{\mathfrak{F}} f $, let $ b = \lim_{\mathfrak{F}} g $ and let $ c $ be such that $ b < c < a $. The interval $ ]c, +\infty] $ of $ \overline{\mathbf{R}} $ (resp. $ ]-\infty, c[ $) is a neighbourhood of $ a $ (resp. $ b $); hence there is a set $ M \in \mathfrak{F} $ (resp. a set $ N \in \mathfrak{F} $) such that $ f(x) > c $ for all $ x \in M $ [resp. $ g(x) < c $ for all $ x \in N $]. The set $ A = M \cap N $ belongs to $ \mathfrak{F} $, and we have $ f(x) > c > g(x) $ for all $ x \in A $.

As a particular case of Proposition 1 we have the following theorem:

#### Theorem 1 (Principle of extension of inequalities) {#top-iv-s5-thm-1 .statement}

*Let $ f $ and $ g $ be two real-valued functions, defined on a set $ X $ filtered by a filter $ \mathfrak{F} $. If $ \lim_{\mathfrak{F}} f $ and $ \lim_{\mathfrak{F}} g $ exist, and if $ f \leq g $, then $ \lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g $.*

#### Remark {#top-iv-s5-n2-rem-1 .statement}

If in particular we have $ f(x) < g(x) $ for all $ x \in X $ (or only for all points of a set of the filter $ \overline{\mathbf{R}} $) we can infer, by Theorem 1, that $ \lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g $; *but we cannot infer the strong inequality* $ \lim_{\mathfrak{F}} f < \lim_{\mathfrak{F}} g $. For example, if we take $ X $ to be the set $ \mathbf{N} $ of natural numbers, filtered by the Fréchet filter, and if $ f(n) = 0 $ and $ g(n) = 1/n $, then $ f(n) < g(n) $ for all $ n $, but $ \lim_{n \to \infty} f(n) = \lim_{n \to \infty} f(n) = 0 $. Thus we *lose strictness* when we pass to the limit in a *strict* inequality.

Suppose for example that $ f $ is increasing, and let $ a = \sup f(A) $. If $ a = -\infty $, the theorem is trivial. If $ a > -\infty $, then for each $ b < a $ there exists $ x \in A $ such that $ b < f(x) \leq a $; hence, if $ S_x $ is the section of $ A $ relative to $ x $ (i.e. the set of all $ y \geq x $, cf. Chapter I, § 6, no. 3), $ f(S_x) $ is contained in the neighbourhood $ ]b, +\infty] $ of $ a $, and the theorem follows. The proof is analogous if $ f $ is decreasing.

#### Corollary {#top-iv-s5-n2-cor-1 .statement}

An increasing (resp. decreasing) real-valued function, defined on a directed subset $ A $ of an ordered set $ X $, has a finite limit with respect to $ A $ if and only if it is bounded above (resp. bounded below) in $ A $.

If we apply Theorem 2 to the case where $ A = X = \mathbf{N} $ (ordered by the relation $ \leq $), we have the following proposition:

#### Proposition 3 {#top-iv-s5-prop-3 .statement}

Every monotonic sequence of real numbers has a limit in $ \overline{\mathbf{R}} $.
In particular, every increasing (resp. decreasing) sequence of finite numbers converges to a finite real number if it is bounded above (resp. bounded below) and to $ +\infty $ (resp. $ -\infty $) otherwise. For example, the sequence of positive integers converges to $ +\infty $.

This fact is the origin of the notation $ \lim_{n \to \infty} u_n $ to denote the limit of a sequence (Chapter I, § 7, no. 3).

Likewise, every strictly increasing sequence of integers $ (p_n) $ converges to $ +\infty $; for we see by induction that $ p_n \geq p_0 + n $ for all $ n $.

### 3. LIMITS ON THE RIGHT AND ON THE LEFT OF A FUNCTION OF A REAL VARIABLE

Let $ A $ be a non-empty subset of $ \overline{\mathbf{R}} $ and let $ a \neq -\infty $ be a point of $ \overline{\mathbf{R}} $ lying in the closure of the set $ B = A \cap [-\infty, a[ $. The set $ B $ is directed with respect to the relation $ \leq $, and its section filter $ \mathfrak{F} $ is the same as the trace on $ B $ of the neighbourhood filter of $ a $ in $ \overline{\mathbf{R}} $.

(*) This statement assumes implicitly that the ordering in $ X $ is written $ x \leq y $. If this relation is written $ x(\sigma) y $, where $ (\sigma) $ is a certain sign or group of signs characteristic of the relation envisaged, then the word "directed" in the statement must be replaced by "directed with respect to $ (\sigma) $".

#### Definition 2 {#top-iv-s5-def-2 .statement}

*Let f be a function defined on a non-empty subset A of $ \overline{\mathbf{R}} $, with values in a topological space X. A limit of f with respect to the filter $ \mathfrak{F} $, if it exists, is called a limit of f on the left at the point a, relative to A, and is denoted by*
$$
\lim_{x \to a,\ x < a,\ x \in A} f(x),
$$
*or $ f(a-) $, if X is Hausdorff.*

Likewise, if $ a $ is in the closure of the set $ A \cap ]a, + \infty] $, we define a *limit on the right* (if it exists) of $ f $ at the point $ a $, and denote it by
$$
\lim_{x \to a,\ x > a,\ x \in A} f(x),
$$
*or $ f(a+) $, if X is Hausdorff.*

The following proposition is an immediate consequence of Theorem 2:

#### Proposition 4 {#top-iv-s5-prop-4 .statement}

*Let A be a subset of $ \overline{\mathbf{R}} $ and let $ a \neq -\infty $ be a point in the closure of the intersection $ A \cap [-\infty, a[ $. If f is a monotonic real-valued function defined on A, then f has a limit $ f(a-) $ on the left at a, relative to A.*

### 4. BOUNDS OF A REAL-VALUED FUNCTION

#### Definition 3 {#top-iv-s5-def-3 .statement}

*Let f be a real-valued function defined on a set X, and let A be a non-empty subset of X. Then the least upper bound (resp. greatest lower bound) of the set $ f(A) $ in $ \overline{\mathbf{R}} $ is called the least upper bound (resp. greatest lower bound) of f in A, and is denoted by*
$$
\sup_{x \in A} f(x) \quad \text{[resp. } \inf_{x \in A} f(x) \text{]}.
$$

In particular, if A is a non-empty subset of $ \overline{\mathbf{R}} $, then
$$(1)$$
$$
\sup A = \sup_{x \in A} x.
$$
It is often more convenient to use the notation on the right-hand side to denote the least upper bound of A.

The number $ a = \sup_{x \in A} f(x) $ is characterized by the following two properties:
(i) For all $ x \in A, f(x) \leq a $.
(ii) For every $ b < a $, there exists $ x \in A $ such that $ b < f(x) \leq a $.

The numbers $ \sup_{x \in A} f(x) $ and $ \inf_{x \in A} f(x) $ belong to the *closure* of $ f(A) $ in $ \overline{\mathbf{R}} $. We have $ \inf_{x \in A} f(x) \leq \sup_{x \in A} f(x) $; and these two numbers are *equal* if and only if $ f $ is *constant* on A.

A real-valued function, defined on a set X, is *bounded above* (resp. *bounded below*) in a non-empty subset A of X if and only if $ \sup_{x \in A} f(x) < + \infty $ [resp. $ \inf_{x \in A} f(x) > -\infty $]. $ f $ is *bounded* in A if and only if $ |f| $ is bounded above in A, hence if and only if $ \sup_{x \in A} |f(x)| < + \infty $.

We have

$$
\inf_{x \in A} f(x) = -\sup_{x \in A} (-f(x)).
$$

This relation reduces all properties of the greatest lower bound to those of the least upper bound; hence in general we shall speak only of the latter.

#### Proposition 5 {#top-iv-s5-prop-5 .statement}

*Let $ f $ be a real-valued function defined on a set $ X $. On the set $ \mathcal{F}(X) $ of all finite subsets of $ X $, directed with respect to the relation $ \subset $, the real-valued function $ H \to \sup_{x \in H} f(x) $ is increasing, the real-valued function $ H \to \inf_{x \in H} f(x) $ is decreasing, and we have*

$$
\begin{cases}
\sup_{x \in A} f(x) = \lim_{H \in \mathcal{F}(X)} (\sup_{x \in H} f(x)), \\
\inf_{x \in A} f(x) = \lim_{H \in \mathcal{F}(X)} (\inf_{x \in H} f(x)).
\end{cases}
$$

Let $ \varphi(H) = \sup_{x \in H} f(x) $. Clearly $ \varphi $ is increasing, and therefore has a limit $ a $ (no. 2, Theorem 2); and since $ \varphi(H) \leq \sup_{x \in A} f(x) $ for all $ H $, we have $ a \leq \sup_{x \in A} f(x) $ (no. 2, Theorem 1). If we had $ a < \sup_{x \in A} f(x) $, then there would exist $ x_0 \in X $ such that $ a < f(x_0) $; but this is a contradiction since $ \varphi(H) \geq f(x_0) $ whenever $ x_0 \in H $.

In particular, by (1), if $ A $ is any non-empty subset of $ \overline{\mathbf{R}} $, we have

$$
\sup A = \lim_{H \in \mathcal{F}(A)} (\sup_{x \in H} x).
$$

#### Proposition 6 {#top-iv-s5-prop-6 .statement}

*Let $ f $ and $ g $ be two real-valued functions defined on $ X $. If $ f(x) \leq g(x) $ at every point $ x $ of a non-empty subset $ A $ of $ X $, then we have*

$$
\begin{cases}
\sup_{x \in A} f(x) \leq \sup_{x \in A} g(x), \\
\inf_{x \in A} f(x) \leq \inf_{x \in A} g(x).
\end{cases}
$$

#### Proposition 7 {#top-iv-s5-prop-7 .statement}

*Let $ f $ be a real-valued function defined on $ X $. If $ A $ and $ B $ are two non-empty subsets of $ X $ such that $ A \subset B $, then*

$$
\sup_{x \in A} f(x) \leq \sup_{x \in B} f(x).
$$

#### Proposition 8 {#top-iv-s5-prop-8 .statement}

*Let $ f $ be a real-valued function defined on $ X $, and let $ (A_i)_{i \in I} $ be a non-empty family of non-empty subsets of $ X $; then*

$$
\sup_{x \in \bigcup_{i \in I} A_i} f(x) = \sup_{i \in I} (\sup_{x \in A_i} f(x)).
$$

Let $ f $ be a real-valued function defined on a product set $ X_1 \times X_2 $. If $ A_2 $ is a non-empty subset of $ X_2 $ we shall denote by $ \sup_{x_1 \in A_2} f(x_1, x_2) $ the least upper bound in $ A_2 $ of the real-valued function $ x_2 \to f(x_1, x_2) $ defined on $ X_2 $. From Proposition 8 we deduce in particular:

#### Proposition 9 {#top-iv-s5-prop-9 .statement}

*Let $ f $ be a real-valued function defined on a product set $ X_1 \times X_2 $. If $ A_1, A_2 $ are any non-empty subsets of $ X_1, X_2 $ respectively, then*

$$
\sup_{(x_1, x_2) \in A_1 \times A_2} f(x_1, x_2) = \sup_{x_1 \in A_1} (\sup_{x_2 \in A_2} f(x_1, x_2)) = \sup_{x_2 \in A_2} (\sup_{x_1 \in A_1} f(x_1, x_2)).
$$

### 5. ENVELOPES OF A FAMILY OF REAL-VALUED FUNCTIONS

#### Definition 4 {#top-iv-s5-def-4 .statement}

*Let $ (f_i)_{i \in I} $ be a family of real-valued functions defined on a set $ X $. The real-valued function on $ X $ whose value at each point $ x \in X $ is $ \sup_{i \in I} (f_i(x)) $ [resp. $ \inf_{i \in I} (f_i(x)) $] is called the upper (resp. lower) envelope of the family $ (f_i) $, and is denoted by $ \sup_{i \in I} f_i $ or $ \sup_i f_i $ (resp. $ \inf_{i \in I} f_i $ or $ \inf_i f_i $).

The upper envelope of the family $ (f_i) $ is thus the least upper bound of this family in the lattice $ \overline{\mathbf{R}} $ of real-valued functions defined on $ X $, and this justifies the notation $ \sup_{i \in I} f_i $.

Furthermore, if we endow $ \overline{\mathbf{R}}^X $ with the topology which is the product of the topologies of its factors (all identical with $ \overline{\mathbf{R}} $), we have the following proposition:

#### Proposition 10 {#top-iv-s5-prop-10 .statement}

*In the product space $ \overline{\mathbf{R}}^X $ the upper envelope $ \sup_{i \in I} f_i $ of a family of real-valued functions $ (f_i)_{i \in I} $ is the limit, with respect to the directed set $ \mathcal{F}(I) $ of finite subsets of $ I $, of the mapping $ H \to \sup_{i \in H} f_i $ [which maps each finite subset $ H $ of $ I $ to the upper envelope of the finite subfamily $ (f_i)_{i \in H} $].

This follows immediately from Proposition 5 of no. 4 and from Chapter I, § 7, no. 6, Corollary 1 to Proposition 10.

We may therefore write

$$
\sup_{i \in I} f_i = \lim_{H \in \mathcal{F}(I)} (\sup_{i \in H} f_i).
$$

#### Definition 5 {#top-iv-s5-def-5 .statement}

*A family $ (f_i)_{i \in I} $ of real-valued functions defined on a set $ X $ is said to be uniformly bounded above (resp. uniformly bounded below) in $ X $, if there exists a finite number $ a $ such that $ f_i(x) \leq a $ [resp. $ f_i(x) \geq a $] for all $ x \in X $ and all $ i \in I $. The family $ (f_i) $ is said to be uniformly bounded in $ X $ if it is uniformly bounded above and below in $ X $.

Thus $ (f_i) $ is uniformly bounded above in $ X $ if and only if the upper envelope of this family is bounded above in $ X $. $ (f_i) $ is uniformly bounded in $ X $ if and only if the upper envelope of the family $ (|f_i|) $ is bounded above in $ X $ [i.e. if and only if there is a finite real number $ a \geq 0 $ such that $ |f_i(x)| \leq a $ for all $ x \in X $ and all $ i \in I $].

### 6. UPPER LIMIT AND LOWER LIMIT OF A REAL-VALUED FUNCTION WITH RESPECT TO A FILTER

Let $ f $ be a real-valued function defined on a set $ X $ filtered by a filter $ \mathcal{G} $. $ \mathcal{G} $ is a directed set with respect to the relation $ \supseteq $ (Chapter I, § 6). For each $ M \in \mathcal{G} $ consider the real number $ \sup_{x \in M} f(x) $: we have a function $ M \to \sup_{x \in M} f(x) $ of $ \mathcal{G} $ into $ \overline{\mathbf{R}} $, which is a decreasing function on $ \mathcal{G} $, by Proposition 7 of no. 4. Hence, by Theorem 2 of no. 2, it has a limit with respect to the directed set $ \mathcal{G} $.

#### Definition 6 {#top-iv-s5-def-6 .statement}

*The limit of the real-valued function* $ M \to \sup_{x \in M} f(x) $ *with respect to the directed set* $ \mathcal{G} $ *is called the upper limit of* $ f $ *with respect to the filter* $ \mathcal{G} $, *and is denoted by* $ \lim \sup_{\mathcal{G}} f $, *or by* $ \lim \sup_{x, \mathcal{G}} f(x) $.

The *lower limit* of $ f $ with respect to the filter $ \mathcal{G} $ is defined similarly, and is denoted by $ \lim \inf_{\mathcal{G}} f $ or $ \lim \inf_{x, \mathcal{G}} f(x) $. Thus we have

$$
\begin{cases}
\lim \sup_{\mathcal{G}} f = \lim_{M \in \mathcal{G}} (\sup_{x \in M} f(x)), \\
\lim \inf_{\mathcal{G}} f = \lim_{M \in \mathcal{G}} (\inf_{x \in M} f(x)).
\end{cases}
$$

(10)

Often the filter $ \mathcal{G} $ is suppressed from the notation, and we write simply $ \lim \sup f $ or $ \lim \sup_{x} f(x) $, or $ \lim \sup f(x) $ when there is no risk of confusion.

From formulae (10) and Theorem 1 we have

$$
\inf_{x \in X} f(x) \leq \lim \inf_{\mathcal{G}} f \leq \lim \sup_{\mathcal{G}} f \leq \sup_{x \in X} f(x).
$$

(11)

By Theorem 2 of no. 2 we may also write

$$
\begin{cases}
\lim \sup_{\mathcal{G}} f = \inf_{M \in \mathcal{G}} (\sup_{x \in M} f(x)), \\
\lim \inf_{\mathcal{G}} f = \sup_{M \in \mathcal{G}} (\inf_{x \in M} f(x)).
\end{cases}
$$

(12)

Also we may replace the filter $ \mathcal{G} $, on the right-hand sides of formulae (10) and (12), by any *base* $ \mathcal{B} $ of $ \mathcal{G} $.

From (2) and (10),

$$
\lim \inf_{\mathcal{G}} f = -\lim \sup_{\mathcal{G}} (-f)
$$

and therefore we need consider only the upper limit.

#### Theorem 3 {#top-iv-s5-thm-3 .statement}

*The upper limit of a real-valued function $ f $ with respect to a filter $ \mathcal{G} $ is equal to the largest cluster value of $ f $ with respect to $ \mathcal{G} $.*

Let $ b $ be a cluster point of $ f $ with respect to $ \mathcal{G} $. For each $ M \in \mathcal{G} $, $ b $ lies in the closure of $ f(M) $, hence $ b \leq \sup_{x \in M} f(x) $, and therefore, by (12),
$ b \leq \lim \sup_{\mathcal{G}} f = a. $

On the other hand, let $ V $ be any open neighbourhood of $ a $ in $ \overline{\mathbf{R}} $. Then there exists a set $ M_0 $ in $ \mathcal{G} $ such that, for each $ M \in \mathcal{G} $ contained in $ M_0 $, we have $ \sup_{x \in M} f(x) \in V $; since $ V $ is open it follows that $ f(M) $ meets $ V $, and therefore $ a $ is a *cluster point* of $ f $ with respect to $ \mathcal{G} $, and the proof is complete.

#### Corollary 1 {#top-iv-s5-thm-3-cor-1 .statement}

*In order that $ \lim \sup_{\mathcal{G}} f = \lim \inf_{\mathcal{G}} f $, it is necessary and sufficient that $ f $ has a limit with respect to the filter $ \mathcal{G} $, and then*
$$
\lim_{\mathcal{G}} f = \lim \sup_{\mathcal{G}} f = \lim \inf_{\mathcal{G}} f.
$$
For since $ \overline{\mathbf{R}} $ is compact, the filter base $ f(\mathcal{G}) $ has a limit point if and only if it has only one cluster point (Chapter I, § 9, no. 1, Corollary to Theorem 1).

#### Corollary 2 {#top-iv-s5-thm-3-cor-2 .statement}

*If $ \mathcal{H} $ is a filter finer than $ \mathcal{G} $, we have*
$$
\lim \inf_{\mathcal{G}} f \leq \lim \inf_{\mathcal{H}} f \leq \lim \sup_{\mathcal{H}} f \leq \lim \sup_{\mathcal{G}} f.
$$
For every cluster point of $ f $ with respect to $ \mathcal{H} $ is also a cluster point of $ f $ with respect to $ \mathcal{G} $ (Chapter I, § 7, no. 3).
In particular, if $ \lim_{\mathcal{G}} f $ exists, then
$$
\lim \inf_{\mathcal{G}} f \leq \lim_{\mathcal{G}} f \leq \lim \sup_{\mathcal{G}} f.
$$

#### Corollary 3 {#top-iv-s5-thm-3-cor-3 .statement}

*Let $ A $ be a set of the filter $ \mathcal{G} $, let $ \mathcal{G}_A $ be the filter induced on $ A $ by $ \mathcal{G} $, and let $ f_A $ be the restriction of $ f $ to $ A $; then*
$$
\lim \sup_{\mathcal{G}_A} f_A = \lim \sup_{\mathcal{G}} f.
$$
For every cluster point of the filter base $ f(\mathcal{G}) $ is a cluster point of the filter base $ f_A(\mathcal{G}_A) $, and conversely.

For this reason, if $ f $ is defined only on a subset $ A $ of $ X $ belonging to $ \mathcal{G} $, we shall often write $ \limsup_{\mathcal{G}} f $ instead of $ \limsup_{\mathcal{G}_A} f_A $, by abuse of language.

#### Proposition 11 {#top-iv-s5-prop-11 .statement}

Let $ f $ and $ g $ be two real-valued functions defined on a filtered set $ X $. Then the relation $ f \leq g $ implies

$$
\begin{cases}
\limsup f \leq \limsup g, \\
\liminf f \leq \liminf g.
\end{cases}
$$

This is an immediate consequence of the relations (12).

When $ X $ is a topological space and $ \mathcal{G} $ is the neighbourhood filter of a point $ a $ of $ X $, we write $ \limsup_{x \to a} f(x) $ [resp. $ \liminf_{x \to a} f(x) $] in place of $ \limsup_{\mathcal{G}} f $ [resp. $ \liminf_{\mathcal{G}} f $]; clearly we have

$$
\liminf_{x \to a} f(x) \leq f(a) \leq \limsup_{x \to a} f(x).
$$

More generally, if $ X $ is a subspace of a topological space $ Y $, and if $ \mathcal{G} $ is the trace on $ X $ of the neighbourhood filter of a point $ a \in \overline{X} $, we write $ \limsup_{x \to a, x \in X} f(x) $ [resp. $ \liminf_{x \to a, x \in X} f(x) $] instead of $ \limsup_{\mathcal{G}} f $ [resp. $ \liminf_{\mathcal{G}} f $] ; $ \limsup $ is called the upper limit of $ f(x) $ as $ x $ tends to $ a $ while remaining in $ X $. If $ X $ is the complement of $ \{a\} $ we write "x \neq a" in place of "x \in X" in these notations.

If $ A $ is a subset of $ X $ such that $ a \in \overline{A} $, then (Corollary 2 to Theorem 3)

$$
\liminf_{x \to a, x \in X} f(x) \leq \liminf_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in X} f(x).
$$

If $ V $ is a neighbourhood of $ a $ in $ Y $, we have (Corollary 3 to Theorem 3)

$$
\limsup_{x \to a, x \in V \cap X} f(x) = \limsup_{x \to a, x \in X} f(x).
$$

Hence the notions of upper and lower limits at a point of a topological space are, like the notion of limit, of local character.

Finally, if $ \mathcal{G} $ is the Fréchet filter on $ \mathbf{N} $, the upper (resp. lower) limit, with respect to $ \mathcal{G} $, of the mapping $ n \to u_n $ of $ \mathbf{N} $ into $ \overline{\mathbf{R}} $ is denoted by $ \limsup_{n \to \infty} u_n $ (resp. $ \liminf_{n \to \infty} u_n $) and is called the upper (resp. lower) limit of the sequence of real numbers $ u_n $.

The relation $ \limsup_{n \to \infty} u_n = a \in \mathbf{R} $ is therefore equivalent to the following : given any $ \varepsilon > 0 $ there exists an integer $ n_0 $ such that, for each $ n \geq n_0 $ we have $ u_n \leq a + \varepsilon $, and for an infinity of values of $ n $ we have $ u_n \geq a - \varepsilon $. The definition of the upper limit of a sequence may be translated similarly when its value is $ +\infty $ or $ -\infty $.

Given a sequence $(f_n)$ of real-valued functions defined on a set $X$, we denote by $\limsup_{n \to \infty} f_n$ (resp. $\liminf_{n \to \infty} f_n$) the real-valued function whose value at any point $x \in X$ is $\limsup_{n \to \infty} f_n(x)$ [resp. $\liminf_{n \to \infty} f_n(x)$]. From (10) and (12) we deduce
$$
\begin{cases}
\limsup_{n \to \infty} f_n = \inf_{n \in \mathbf{N}} (\sup_{m \geq n} f_m) = \lim_{n \to \infty} (\sup_{m \geq n} f_m), \\
\liminf_{n \to \infty} f_n = \sup_{n \in \mathbf{N}} (\inf_{m \geq n} f_m) = \lim_{n \to \infty} (\inf_{m \geq n} f_m),
\end{cases}
$$
the limits being taken in the *product space* $\overline{\mathbf{R}}^X$. The sequence $(f_n)$ has a *limit* in $\overline{\mathbf{R}}^X$ if and only if $\limsup_{n \to \infty} f_n = \liminf_{n \to \infty} f_n$ (Corollary 1 to Theorem 3, and Chapter I, § 7, no. 6, Corollary 1 to Proposition 10).

### 7. ALGEBRAIC OPERATIONS ON REAL-VALUED FUNCTIONS

Let $f$ and $g$ be two real-valued functions defined on a set $X$; if the sum $f(x) + g(x)$ [resp. the product $f(x)g(x)$] is defined for all $x \in X$, then we denote by $f + g$ (resp. $fg$) the real-valued function
$$
x \mapsto f(x) + g(x) \quad \text{[resp. } x \mapsto f(x)g(x)].
$$
Again, if $1/f(x)$ is defined for all $x \in X$, then $1/f$ denotes the function $x \mapsto 1/f(x)$.

This last function is therefore defined provided $f$ does not take the value 0; when $f$ takes its values in the interval $[0, +\infty]$ (resp. in $[-\infty, 0]$) $1/f(x)$ as everywhere defined by putting $1/0 = +\infty$ (resp. $1/0 = -\infty$); in this case the function $1/f$ is defined.

Suppose that $X$ is filtered by a filter $\mathcal{F}$, and that $\lim_{\mathcal{F}} f$ and $\lim_{\mathcal{F}} g$ exist. If on the one hand the function $f + g$ (resp. $fg$, $1/g$) is defined, and if on the other hand the expression $\lim_{\mathcal{F}} f + \lim_{\mathcal{F}} g$ (resp. $\lim_{\mathcal{F}} f \cdot \lim_{\mathcal{F}} g$, $1/\lim_{\mathcal{F}} f$) has a sense, then $\lim_{\mathcal{F}} (f + g)$ [resp. $\lim_{\mathcal{F}} fg$, $\lim_{\mathcal{F}} (1/f)$] exists and is equal to this expression by reason of the continuity of the function $x + y$ (resp. $xy$, $1/x$) at points where it is defined.

#### Proposition 12 {#top-iv-s5-prop-12 .statement}

*Let $f$ and $g$ be two real-valued functions defined on a set $X$, and let $A$ be a non-empty subset of $X$.*

(i) *We have*
$$
\begin{align*}
&\sup_{x \in A} (f(x) + g(x)) \leq \sup_{x \in A} f(x) + \sup_{x \in A} g(x), \\
&\sup_{x \in A} f(x) + \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x) + g(x)),
\end{align*}
$$
*whenever both sides of these inequalities are defined.*

(ii) *If $ f(x) $ and $ g(x) $ are $ \geq 0 $ for each $ x \in A $, then*

(19)
$$
\sup_{x \in A} (f(x)g(x)) \leq \sup_{x \in A} f(x) \sup_{x \in A} g(x),
$$
(20)
$$
\sup_{x \in A} f(x) \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x)g(x))
$$
*whenever both sides of these inequalities are defined.*

(iii) *If $ f(x) \geq 0 $ for all $ x \in A $, then*
(21)
$$
\sup_{x \in A} (1/f(x)) = 1/\inf_{x \in A} f(x)
$$
*(putting $ 1/0 = +\infty $).*

Let $ H $ be any *finite* subset of $ A $. If $ x_0 $ is one of the points of $ H $ where $ f + g $ takes its greatest value, then we have
$$
f(x_0) + g(x_0) \leq \sup_{x \in H} f(x) + \sup_{x \in H} g(x);
$$
on the other hand, if $ x_1 $ is one of the points of $ H $ where $ f $ takes its greatest value, then
$$
f(x_1) + g(x_1) \geq \sup_{x \in H} f(x) + \inf_{x \in H} g(x);
$$
therefore
$$
\sup_{x \in H} f(x) + \inf_{x \in H} g(x) \leq \sup_{x \in H} (f(x) + g(x)) \leq \sup_{x \in H} f(x) + \sup_{x \in H} g(x).
$$
The inequalities (17) and (18) follow from this by applying Proposition 5 of no. 4 and Theorem 1 of no. 2. The proofs of the other inequalities are analogous.

#### Corollary 1 {#top-iv-s5-prop-12-cor-1 .statement}

*Let $ f $ be a real-valued function defined on $ X $, and let $ k $ be a real number. Then*
(22)
$$
\sup_{x \in A} (f(x) + k) = k + \sup_{x \in A} f(x)
$$
*whenever both sides are defined, and, if $ k \geq 0,$*
(23)
$$
\sup_{x \in A} (kf(x)) = k \cdot \sup_{x \in A} f(x)
$$
*whenever both sides are defined.*

#### Corollary 2 {#top-iv-s5-prop-12-cor-2 .statement}

*Let $ f_1 $ and $ f_2 $ be two real-valued functions defined on sets $ X_1, X_2 $ respectively; then if $ A_1, A_2 $ are any non-empty subsets of $ X_1, X_2 $ respectively, we have*
(24)
$$
\sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1) + f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) + \sup_{x_2 \in A_2} f_2(x_2)
$$

whenever both sides are defined; and if $ f_1, f_2 $ are $ \geq 0 $ in $ A_1, A_2 $ respectively we have

$$
(25) \quad \sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1)f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) \sup_{x_2 \in A_2} f_2(x_2),
$$

whenever both sides are defined.

This is an immediate consequence of the preceding corollary and Proposition 9 of no. 4.

In particular, if $ A $ and $ B $ are two subsets of $ \overline{\mathbf{R}} $ such that the set $ A + B $ of sums $ x + y \ (x \in A, y \in B) $ is defined, we have

$$
(26) \quad \sup (A + B) = \sup A + \sup B
$$

if the right-hand side is defined. Again, if $ A $ and $ B $ are two subsets of $[0, + \infty]$, we have

$$
(27) \quad \sup AB = \sup A \cdot \sup B
$$

whenever both sides are defined.

#### Proposition 13 {#top-iv-s5-prop-13 .statement}

*Let $ f $ and $ g $ be two real-valued functions defined on a filtered set $ X $.*

(i) *We have*

$$
(28) \quad \lim \sup (f + g) \leq \lim \sup f + \lim \sup g,
$$
$$
(29) \quad \lim \sup f + \lim \inf g \leq \lim \sup (f + g)
$$

*whenever both sides of these inequalities are defined.*

(ii) *If $ f $ and $ g $ are $ \geq 0 $ on $ X $, we have*

$$
(30) \quad \lim \sup fg \leq (\lim \sup f) (\lim \sup g),
$$
$$
(31) \quad (\lim \sup f) (\lim \inf g) \leq \lim \sup fg
$$

*whenever both sides of these inequalities are defined.*

(iii) *If $ f \geq 0 $ on $ X $, then*

$$
(32) \quad \lim \sup (1/f) = 1/(\lim \inf f)
$$

(putting $ 1/0 = + \infty $).

These relations are consequences of Proposition 12 and relations (10)

#### Corollary 1 {#top-iv-s5-prop-13-cor-1 .statement}

*Let $ f $ and $ g $ be two real-valued functions defined on a filtered set $ X $. If $ \lim g $ exists, then*

$$
(33) \quad \lim \sup (f + g) = \lim \sup f + \lim g
$$

whenever both sides are defined, and

(34) $$
\lim \sup fg = (\lim \sup f) (\lim g)
$$

whenever both sides are defined and $ f $ and $ g $ are $ \geqslant 0 $.

#### Corollary 2 {#top-iv-s5-prop-13-cor-2 .statement}

Let $ f $ and $ g $ be two real-valued functions defined on a filtered set $ X $. If $ \lim f = +\infty $ and $ \lim \inf g > -\infty $ and $ f + g $ is defined, then $ \lim (f + g) = +\infty $. If $ \lim f = +\infty $ and $ \lim \inf g > 0 $ and $ fg $ is defined, then $ \lim fg = +\infty $.

### Exercises {#top-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
