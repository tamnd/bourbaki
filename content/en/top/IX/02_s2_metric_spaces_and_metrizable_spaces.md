---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 2
section_title: Metric spaces and metrizable spaces
lang: en
source: top-v-x
pdf_pages: 0153-0166, 0232-0241
extraction: ocr
subsections:
    - "no": 1
      title: METRICS AND METRIC SPACES
      page: 0
      pdf_page: 153
    - "no": 2
      title: STRUCTURE OF A METRIC SPACE
      page: 0
      pdf_page: 154
    - "no": 3
      title: OSCILLATION OF A FUNCTION
      page: 0
      pdf_page: 157
    - "no": 4
      title: METRIZABLE UNIFORM SPACES
      page: 0
      pdf_page: 157
    - "no": 5
      title: METRIZABLE TOPOLOGICAL SPACES
      page: 0
      pdf_page: 158
    - "no": 6
      title: USE OF COUNTABLE SEQUENCES
      page: 0
      pdf_page: 159
    - "no": 7
      title: SEMI-CONTINUOUS FUNCTIONS ON A METRIZABLE SPACE
      page: 0
      pdf_page: 161
    - "no": 8
      title: METRIZABLE SPACES OF COUNTABLE TYPE
      page: 0
      pdf_page: 161
    - "no": 9
      title: COMPACT METRIC SPACES; COMPACT METRIZABLE SPACES
      page: 0
      pdf_page: 163
    - "no": 10
      title: QUOTIENT SPACES OF METRIZABLE SPACES
      page: 0
      pdf_page: 165
statements: 33
exercises: 9
content_sha256: 6e7b44504b54feee5f0b3d6af73ef51f9efcd47254e6b60be3532a4009721713
---

## 2. METRIC SPACES AND METRIZABLE SPACES

### 1. METRICS AND METRIC SPACES

#### Definition 1 {#top-ix-s2-def-1 .statement}

*A metric on a set* $X$ *is a finite pseudometric* $d$ *on* $X$ *such that the relation* $d(x, y) = 0$ *implies* $x = y$. *A metric space is a set* $X$ *endowed with the structure defined by a given metric on* $X$.

A metric space $X$ is always considered as carrying the uniformity and the topology defined by the given metric on $X$.

#### Example 1 {#top-ix-s2-n1-exa-1 .statement}

The Euclidean distance $d(x, y)$ (Chapter VI, § 2, no. 1) is a metric on real $n$-dimensional number space $\mathbf{R}^n$; so are the functions

$$
\sup_{1 \leq i \leq n} |x_i - y_i| \quad \text{and} \quad \sum_{i=1}^n |x_i - y_i|.
$$

All these metrics are *equivalent* ($\S$ 1, no. 2).

#### Example 2 {#top-ix-s2-n1-exa-2 .statement}

On any set $X$ the pseudometric $d$, defined by the relations $d(x, x) = 0$ and $d(x, y) = 1$ if $x \neq y$, is a metric. The uniformity it defines on $X$ is the *discrete* uniformity.

We have a definition equivalent to Definition 1 if we say that a metric is a *finite* pseudometric such that the uniformity defined by this pseudometric is *Hausdorff*; a finite pseudometric which is equivalent to a metric is therefore a metric.

Uniform spaces defined by a *single pseudometric* (which we may assume to be *finite*) can be reduced to metric spaces when the pseudometric is not a metric. Let $f$ be such a pseudometric on a set $X$, and let $\mathcal{U}$ be the uniformity defined by $f$; $\mathcal{U}$ is not Hausdorff, and the intersection of the entourages of $\mathcal{U}$ is the subset of $X \times X$ defined by the equivalence relation $f(x, y) = 0$. Let $R$ denote this relation. If $x \equiv x' \pmod{R}$, then by the triangle inequality we have

$$
f(x, y) \leq f(x, x') + f(x', y) = f(x', y)
$$

and similarly $f(x', y) \leq f(x, y)$, so that $f(x, y) = f(x', y)$; in other words, $f$ is a function *compatible* (in $x$ and $y$) with the equivalence relation $R$ (*Set Theory*, R, § 5, no. 7). Let $\overline{f}$ be the function induced by $f$ on the quotient set; $\overline{f}$ is defined on $(X/R) \times (X/R)$, and if $x$ and $y$ are any two points of $X$ and if $\dot{x}$ and $\dot{y}$ denote the equivalence classes (mod $R$) of $x$ and $y$ respectively, then we have $\overline{f}(\dot{x}, \dot{y}) = f(x, y)$. It follows immediately that $\overline{f}$ is a *metric* on $X/R$; it is called the metric *associated* with the pseudometric $f$; furthermore, the uniformity it defines on $X/R$ is precisely the Hausdorff uniformity *associated* with $\mathcal{U}$ by the definition of this uniformity (Chapter II, § 3, no. 8, Remark). Thus, by passing to a suitable quotient space, the uniform structure defined by a single pseudometric can be reduced to the structure of a metric space.

Proposition 1 of § 1, no. 3 determines the structure of the *completion* of a metric space:

#### Proposition 1 {#top-ix-s2-prop-1 .statement}

*Let $X$ be a metric space and let $d$ be its metric. If $\hat{X}$ is the completion of $X$ (with respect to the uniformity defined by $d$), the function $d$ can be extended by continuity to $\hat{X} \times \hat{X}$; the extended function $\overline{d}$ is a metric on $\hat{X}$, and the uniformity of $\hat{X}$ coincides with that defined by the metric $\overline{d}$.*

Proposition 1 of § 1, no. 3 shows that $\overline{d}$ is a finite pseudometric on $\hat{X}$, and that the uniformity defined by $\overline{d}$ on $\hat{X}$ is the uniformity obtained by completion; since this latter uniformity is Hausdorff, $\overline{d}$ is a *metric*. Whenever we consider the completion of a metric space $X$ as a metric space, it is always to be understood that the metric on $\hat{X}$ is that obtained by extending the metric on $X$ by continuity.

### 2. STRUCTURE OF A METRIC SPACE

Let $X$ and $X'$ be two metric spaces, $d$ the metric on $X$, $d'$ the metric on $X'$. In accordance with the general definitions (*Set Theory*, R, § 8, no. 5) a one-to-one mapping $f$ of $X$ onto $X'$ is an *isomorphism* of the metric space structure of $X$ onto that of $X'$ if

$$(1)$$
$$
d(x, y) = d'(f(x), f(y))
$$

for all $x \in X$ and all $y \in X$.

Note that if $f$ is a mapping of $X$ onto $X'$ which satisfies the identity (1), then $f$ must be *bijective* and therefore an isomorphism of $X$ onto $X'$; such an isomorphism is also called an *isometry* (or an *isometric* mapping) of $X$ onto $X'$.

An isometry of X onto X' is of course an isomorphism of the uniformity (resp. topology) of X onto the uniformity (resp. topology) of X'; the converses of these statements are false, as is shown by the existence of distinct equivalent metrics (§ 1, no. 2).

Let X be a metric space, d the metric on X. For each a > 0 let V_a denote the subset of X × X consisting of all pairs (x, y) such that d(x, y) < a, and let W_a denote the subset of X × X consisting of all pairs (x, y) such that d(x, y) ≤ a. As a runs through the set of all real numbers > 0 (or merely a sequence of numbers > 0 which tends to 0), the sets V_a (resp. W_a) form a fundamental system of open (resp. closed) entourages of the uniformity of X, because of the continuity of d (§ 1, no. 3). We have $\overline{V}_a \subset W_a$, but these two sets are not necessarily the same.

By analogy with the case of the Euclidean distance on $\mathbf{R}^n$, the set $V_a(x)$ [resp. $W_a(x)$] is called the open (resp. closed) ball with centre x and radius a; it is an open (resp. closed) set in X. Again, the set of all $y \in X$ such that $d(x, y) = a$ is called the sphere with centre x and radius a; it is a closed set. From what has been said, the open (resp. closed) balls with centre x and radius a form a fundamental system of neighbourhoods of x as a runs through the set of all real numbers > 0, or a sequence of numbers > 0 which tends to 0.

The reader should beware of assuming that balls and spheres in an arbitrary metric space enjoy the same properties as the Euclidean balls and spheres studied in Chapter VI, § 2. Thus the closure of an open ball need not be the closed ball of the same centre and radius; the frontier of a closed ball need not be the sphere of the same centre and radius; an open (or closed) ball need not be connected; and a sphere can be empty (cf. Exercise 4).

Let A and B be any two non-empty subsets of a metric space X. The number
$$
d(A, B) = \inf_{x \in A, y \in B} d(x, y)
$$
is called the distance between the sets A and B. In particular we denote by $d(x, A)$ the distance between the set $\{x\}$ and the set A; this is called the distance from the point x to the set A. Thus
$$
d(x, A) = \inf_{y \in A} d(x, y)
$$
whence
$$
d(A, B) = \inf_{x \in A} d(x, B)
$$
(Chapter IV, § 5, no. 4, Proposition 9).

#### Remark {#top-ix-s2-n2-rem-1 .statement}

If $d(x, A) = a$, it can happen that there is no point of A whose distance from x is equal to a. However, this situation can never arise if A is compact, for then Weierstrass's theorem (Chapter IV, § 6, no. 1, Theorem 1) shows that there exists $y \in A$ such that $d(x, A) = d(x, y)$.

#### Proposition 2 {#top-ix-s2-prop-2 .statement}

*The statements* $d(x, A) = 0$ *and* $x \in \overline{A}$ *are equivalent*.

For $d(x, A) = 0$ expresses the fact that the ball $V_a(x)$ meets $A$ whatever the value of $a > 0$; and this is equivalent to $x \in \overline{A}$.

#### Proposition 3 {#top-ix-s2-prop-3 .statement}

*The function* $d(x, A)$ *is uniformly continuous on* $X$.

Let $x$ and $y$ be any two points of $X$; then given any $\varepsilon > 0$ there exists $z \in A$ such that $d(y, z) \leq d(y, A) + \varepsilon$, and therefore
$$
d(x, z) \leq d(x, y) + d(y, z) \leq d(x, y) + d(y, A) + \varepsilon
$$
by the triangle inequality.

*A fortiori* $d(x, A) \leq d(x, y) + d(y, A) + \varepsilon$, and since $\varepsilon$ is arbitrary it follows that $d(x, A) \leq d(x, y) + d(y, A)$. Similarly we have
$$
d(y, A) \leq d(x, y) + d(x, A),
$$
so that
$$
|d(x, A) - d(y, A)| \leq d(x, y),
$$
whence the result follows.

#### Remark {#top-ix-s2-n2-rem-2 .statement}

We can have $d(A, B) = 0$ for two subsets $A, B$ of $X$ such that $\overline{A} \cap \overline{B} = \varnothing$, provided that neither subset consists of a single point. For example, on the real line $\mathbf{R}$, the set of integers $> 0$ and the set of points of the sequence $(n + 1/2^n)_{n \geq 1}$ are two disjoint closed sets whose distance a part is zero.

However, if $A$ is *compact* and $B$ is *closed*, the relation $d(A, B) = 0$ implies $A \cap B \neq \varnothing$, for by virtue of the relation
$$
d(A, B) = \inf_{x \in A} d(x, B)
$$
it follows from Proposition 3 and Weierstrass's theorem that there exists $x_0 \in A$ such that $d(x_0, B) = d(A, B) = 0$ and hence (Proposition 2) $x_0 \in B$.

The *diameter* of a non-empty subset $A$ of $X$ is the number (finite or equal to $+\infty$)
$$
\delta(A) = \sup_{x \in A, y \in A} d(x, y).
$$

The notion of a "W_a-small set" (Chapter II, § 3, no. 1) is identical with that of a set of diameter $\leq a$. A non-empty set $A$ consists of a single point if and only if $\delta(A) = 0$.

A subset $A$ of $X$ is *bounded* (with respect to the metric $d$) if its diameter is *finite*; equivalently, if for each point $x_0 \in X$, $A$ is contained in a ball with centre $x_0$. Every subset of a bounded set is bounded, and the union of a finite family of bounded sets is a bounded set.

Note that a subset of $X$ can be bounded with respect to a metric $d$ but unbounded with respect to a metric equivalent to $d$ (cf. § 1, no. 2).

### 3. OSCILLATION OF A FUNCTION

Related to the notion of diameter is that of the oscillation of a function $f$, defined on an arbitrary set $X$ and taking its values in a metric space $X'$; if $A$ is any non-empty subset of $X$, the diameter $\delta(f(A))$ is called the oscillation of $f$ in $A$.

If moreover $X$ is a subset of a topological space $Y$, and if $x \in \overline{X}$, the number
$$
\omega(x; f) = \inf \delta(f(V \cap X))
$$
(as $V$ runs through the neighbourhood filter of $x$ in $Y$) is called the oscillation of $f$ at $x \in \overline{X}$.

#### Proposition 4 {#top-ix-s2-prop-4 .statement}

*The oscillation $\omega(x; f)$ of an arbitrary function $f$, defined on a subset $X$ of a topological space $Y$ and taking its values in a metric space $X'$, is upper semi-continuous on $\overline{X}$.*

Let $a$ be any point of $\overline{X}$; then for each $k > \omega(a; f)$ there exists an open neighbourhood $V$ of $a$ such that $\delta(f(V \cap X)) \leq k$; for each $x \in V \cap \overline{X}$, $V$ is a neighbourhood of $x$ and therefore
$$
\omega(x; f) \leq \delta(f(V \cap X)) \leq k,
$$
which shows that $\omega$ is upper semi-continuous at the point $a$.

In order that $\omega(x; f) = 0$ at a point $x \in \overline{X}$ it is necessary and sufficient that for each $\varepsilon > 0$ there should exist a neighbourhood $V$ of $x$ such that $f(V \cap X)$ is contained in a ball of radius $\varepsilon$; if $x \in X$, this condition expresses the fact that $f$ is continuous at the point $x$ (with respect to $X$); if $x \in \overline{X} \cap \mathbf{C}X$, the image under $f$ of the trace on $X$ of the neighbourhood filter of $x$ in $Y$ is a Cauchy filter base on $X'$; in particular:

#### Proposition 5 {#top-ix-s2-prop-5 .statement}

*Let $f$ be a function defined on a subset $X$ of a topological space $Y$, taking its values in a complete metric space $X'$. Then $f$ has a limit relative to $X$ at a point $x \in \overline{X}$ if and only if the oscillation of $f$ at $x$ is zero.*

### 4. METRIZABLE UNIFORM SPACES

#### Definition 2 {#top-ix-s2-def-2 .statement}

*A metric on a set $X$ is said to be compatible with a uniformity $U$ on $X$ if the uniformity defined by the metric coincides with $U$.
A uniformity on a set $X$ is said to be metrizable if there is a metric on $X$ compatible with this uniformity. A uniform space is said to be metrizable if its uniformity is metrizable.*

Distinct metrics can be compatible with the same uniformity; they are then *equivalent* (§ 1, no. 2, Definition 2).

#### Theorem 1 {#top-ix-s2-thm-1 .statement}

*A uniformity is metrizable if and only if it is Hausdorff and the filter of entourages of the uniformity has a countable base.*

The condition is *necessary*, for (with the notation of no. 2) the entourages $V_{1/n} (n \geq 1)$ form a base of the filter of entourages of the uniformity of a metric space.

The condition is *sufficient*, for, if it is satisfied, the uniformity under consideration is defined by a single pseudometric, by Proposition 2 of § 1, no. 4; since the uniformity is Hausdorff, this pseudometric is a metric.

#### Corollary 1 {#top-ix-s2-thm-1-cor-1 .statement}

*A Hausdorff uniformity defined by a countable family of pseudometrics is metrizable.*

For if $(f_n)$ is a sequence of pseudometrics defining such a structure, the filter of entourages is generated by the countable family of sets $\overline{f}_n^1([0, 1/m])$, where $m$ and $n$ each run through the set of integers $> 0$.

#### Corollary 2 {#top-ix-s2-thm-1-cor-2 .statement}

*Every countable product of metrizable uniform spaces is metrizable.*

For such a space is Hausdorff and its uniformity has a countable fundamental system of entourages (Chapter II, § 2, no. 6).

### 5. METRIZABLE TOPOLOGICAL SPACES

#### Definition 3 {#top-ix-s2-def-3 .statement}

*A metric on a set $X$ is said to be compatible with a topology $\mathcal{T}$ on $X$ if the topology defined by this metric coincides with $\mathcal{T}$. A topological space is said to be metrizable if there exists a metric on $X$ compatible with the topology of $X$.*

Two metrics on a set $X$ which are both compatible with the same topology $\mathcal{T}$ can be *inequivalent*.

The subspace $\mathbf{R}_+^*$ of $\mathbf{R}$ provides an example of this. Both the uniformity induced by the additive uniformity of $\mathbf{R}$ and the uniformity induced by the multiplicative uniformity of $\mathbf{R}_+^*$ are metrizable and are compatible with the topology of $\mathbf{R}_+^*$; but they are not comparable.

We remark also that there can exist *non-metrizable* uniformities compatible with the topology of a *metrizable* topological space (Exercise 7).

We shall content ourselves here with *necessary* conditions for the metrizability of a topological space (for a necessary and sufficient condition, cf. § 4, Exercise 22). In the first place, a space cannot be metrizable unless it is completely regular (indeed we shall see, in § 4, no. 1, Proposition 2, that a metrizable space is necessarily "normal", which is a stronger condition). On the other hand, Theorem 1 shows that:

#### Proposition 6 {#top-ix-s2-prop-6 .statement}

Every point of a metrizable space has a countable fundamental system of neighbourhoods.

More generally:

#### Proposition 7 {#top-ix-s2-prop-7 .statement}

In a metrizable space, every closed set is the intersection of a countable family of open sets, and every open set is the union of a countable family of closed sets.

Let $d$ be a metric compatible with the topology of a metrizable space $X$. If $A$ is a closed subset of $X$, it is the intersection of the open sets $V_{1/n}(A)$ [the set of all $x \in X$ such that $d(x, A) < 1/n$; cf. Proposition 2]. The second part of the proposition follows by taking complements.

#### Remark 1 {#top-ix-s2-n5-rem-1 .statement}

These necessary conditions are not sufficient (cf. Exercise 13).

#### Remark 2 {#top-ix-s2-n5-rem-2 .statement}

There are spaces in which every point has a countable fundamental system of neighbourhoods but in which there exist closed sets which are not countable intersections of open sets (Exercise 15); such spaces are not metrizable.

Corollary 2 of Theorem 1, no. 4, shows that a countable product of metrizable topological spaces is metrizable. Also the sum $X$ (Chapter I, § 2, no. 4) of an arbitrary family $(X_i)_{i \in I}$ of metrizable spaces is metrizable. For if $d_i$ is a metric compatible with the topology of $X_i$ for each $i \in I$, we may assume that $d_i$ is bounded and that the diameter of $X_i$ is $\leq 1$; we can then define a distance $d$ compatible with the topology of $X$ by putting $d(x, y) = d_i(x, y)$ if $x$ and $y$ both belong to the same $X_i$, and $d(x, y) = 1$ otherwise.

### 6. USE OF COUNTABLE SEQUENCES

Proposition 6 is the origin of the part played by countable sequences of points in the theory of metrizable spaces; for many problems, they can be used to advantage in place of filters. This is because the neighbourhood filters of points of a metrizable space (and therefore also convergent filters) are determined by convergent sequences of points of the space: for since the neighbourhood filter of a point has a countable base, it is the intersection of the elementary filters finer than itself (Chapter I, § 6, no. 8, Proposition 11), i.e., of the elementary filters associated with sequences which converge to the point in question.

On the other hand, the notion of a convergent sequence is not adapted to the study of topological spaces in which there are points whose neighbourhood filter has no countable base. In particular, Hausdorff non-discrete topological spaces can be constructed in which, at every point $x$, the intersection of any countable family of neighbourhoods of $x$ is again a neighbourhood of $x$(*); in such a space the only convergent sequences are those in which all the terms are equal from a certain index onwards.

As examples of the use of countable sequences we give the following propositions:

#### Proposition 8 {#top-ix-s2-prop-8 .statement}

*In a metrizable space* $X$, *a point* $x$ *lies in the closure of a non-empty subset* $A$ *of* $X$ *if and only if there is a sequence of points of* $A$ *which converges to* $x$.

We know already, from Chapter I, § 7, no. 3, that the condition is *sufficient*. To see that it is *necessary*, consider a countable fundamental system $(V_n)$ of neighbourhoods of $x$ such that $V_{n+1} \subset V_n$ for each $n$. If $x$ lies in the closure of $A$ then each $V_n$ meets $A$, and if $x_n$ lies in $V_n \cap A$, the sequence $(x_n)$ converges to $x$(**).

From Proposition 8 we deduce:

#### Proposition 9 {#top-ix-s2-prop-9 .statement}

*A metric space* $X$ *is complete if and only if every Cauchy sequence in* $X$ *is convergent*.

Let $\hat{X}$ be the completion of $X$. If there is a point $x \in \hat{X}$ which does not belong to $X$, then there is a sequence $(x_n)$ of points of $X$ which converges to $x$, and this is a non-convergent Cauchy sequence in $X$.

#### Proposition 10 {#top-ix-s2-prop-10 .statement}

*Let* $X$ *be a metrizable space and let* $f$ *be a mapping of* $X$ *into a topological space* $X'$. *Then* $f$ *is continuous at a point* $x \in X$ *if and only if, whenever* $(x_n)$ *is a sequence of points of* $X$ *which converges to* $x$, *the sequence* $(f(x_n))$ *converges to* $f(x)$ *in* $X'$.

The condition is necessary, from Chapter I, § 7, no. 4, Proposition 9, Corollary 1. To show that it is sufficient, consider the filter $\mathcal{B}'$ of neighbourhoods of $f(a)$ in $X'$; the hypothesis implies that $\overline{f}^{-1}(\mathcal{B}')$ is coarser than every elementary filter associated with a sequence which converges to $a$, that is to say every elementary filter which converges to $a$; but

(*) See e.g., J. Dieudonné, Notes de Tératopologie (I), Revue scientifique (Revue rose), 1939, p. 39.
(**) This proposition can still be valid in certain spaces in which at least one point does not have any countable fundamental system of neighbourhoods; for example, the space obtained by compactifying an uncountable discrete space by adjoining a point at infinity (Chapter I, § 9, no. 8, Theorem 4).

the intersection of these filters is the neighbourhood filter of $a$ (Chapter I, § 6, no. 8, Proposition 11). Hence the result.

Note that Propositions 8 and 10 are valid in any space $X$ in which every point has a countable fundamental system of neighbourhoods.

### 7. SEMI-CONTINUOUS FUNCTIONS ON A METRIZABLE SPACE

#### Proposition 11 {#top-ix-s2-prop-11 .statement}

*Let $X$ be a metrizable space and let $f$ be a lower semi-continuous function on $X$ which takes its values in a closed interval $[a, b]$ of $\overline{\mathbf{R}}$. Then $f$ is the upper envelope of an increasing sequence of continuous functions on $X$ which take their values in $[a, b]$.*

By transfer of structure we may assume that $a = 0$ and $b = 1$.

(i) Suppose first that $f = \varphi_A$, where $A$ is an open subset of $X$. Then the function $g_n$ defined by $g_n(x) = n \inf (d(x, X - A), 1/n)$ is continuous and $\geq 0$ on $X$; also $g_n(x) = f(x)$ when $x \in X - A$ and when
$$
d(x, X - A) \geq 1/n.
$$
It follows immediately that $f = \sup_n (g_n)$.

(ii) In the general case consider, for each integer $n \geq 1$, the finite decreasing sequence of open sets
$$
A_k = f^{-1}\left( \left[ \frac{k}{n}, +\infty \right[ \right) \quad (0 \leq k \leq n - 1);
$$
the function $g_n = \frac{1}{n} \sum_{k=1}^{n-1} \varphi_{A_k}$ is lower semi-continuous, and we have $0 \leq f(x) - g_n(x) \leq 1/n$ for all $n$; hence $f$ is the upper envelope of the sequence $(g_n)$. On the other hand, $g_n$ is a linear combination with positive coefficients of a finite number of characteristic functions of open sets and is therefore the upper envelope of a countable sequence $(h_{mn})_{m \geq 0}$ of continuous functions $\geq 0$, by (i); hence $f = \sup_{m,n} h_{mn}$. If we put
$$
f_n = \sup_{p \leq n, q \leq n} h_{pq},
$$
we see that the sequence $(f_n)$ is an increasing sequence of continuous functions $\geq 0$, with $f$ as upper envelope, and which do not take the value 1, since $g_n \leq n - 1/n$.

### 8. METRIZABLE SPACES OF COUNTABLE TYPE

#### Definition 4 {#top-ix-s2-def-4 .statement}

*A metrizable space is said to be of countable type (or separable) if its topology has a countable base.*

Clearly every subspace of a metrizable space of countable type is again of countable type. The definition of the base of the topology of a product space (Chapter I, § 4, no. 1) and Corollary 2 to Theorem 1 of no. 4 show that the product of a countable family of metrizable spaces of countable type is a metrizable space of countable type. Again, the sum of a countable family of metrizable spaces of countable type is a metrizable space of countable type (no. 5).

#### Proposition 12 {#top-ix-s2-prop-12 .statement}

*If X is a metrizable topological space, the following statements are equivalent*:

a) *X is of countable type*.
b) *X has a countable dense subset*.
c) *X is homeomorphic to a subspace of the cube $\mathbf{I}^{\mathbf{N}}$, where $\mathbf{I}$ is the interval $[0, 1]$ in $\mathbf{R}$.

From the preceding remarks it is clear that c) implies a); a) implies b), for if $(U_n)$ is a countable base of the topology of X and $a_n$ is a point of $U_n$, the $a_n$ form a dense subset of X. Finally let us show that b) implies c). Let $(a_n)$ be a dense sequence of points of X, and for each $x \in X$ let $\varphi(x)$ be the point $(d(x, a_n))_{n \in \mathbf{N}}$ of $\mathbf{I}^{\mathbf{N}}$ ($d$ being a metric compatible with the topology of X, with respect to which the diameter of X is $\leq 1$). We shall show that $\varphi$ is a homeomorphism of X onto a subspace of $\mathbf{I}^{\mathbf{N}}$. Indeed, $\varphi$ is continuous, because each of the functions $x \to d(x, a_n)$ is continuous; and $\varphi$ is injective, because each point of X is the limit of some subsequence of $(a_n)$ (Proposition 8). Let B be a ball with centre $x_0$ and radius $r$ in X, and let $n$ be an integer such that

$$
d(x_0, a_n) < \frac{1}{3} r.
$$

The image under $\varphi$ of the set W of points $x \in X$ such that

$$
|d(x_0, a_n) - d(x, a_n)| < \frac{1}{3} r
$$

is by definition a neighbourhood of $\varphi(x_0)$ in $\varphi(X)$. But for each $x \in W$ we have $d(x, a_n) < d(x_0, a_n) + \frac{1}{3} r < \frac{2}{3} r$, whence

$$
d(x, x_0) \leq d(x_0, a_n) + d(x, a_n) < r,
$$

which shows that W is a neighbourhood of $x_0$ contained in B, and therefore that $\varphi$ is a homeomorphism of X onto $\varphi(X)$.

Note that for an arbitrary topological space X, property b) does not necessarily imply the existence of a countable base, even if X is compact and every point of X has a countable fundamental system of neighbourhoods (Exercise 13; cf. Chapter I, § 1, Exercise 7).

#### Proposition 13 {#top-ix-s2-prop-13 .statement}

*Let X be a topological space which has a countable base $(U_n)$; then for each open covering $(V_i)_{i \in I}$ of X there exists a countable subset J of I such that $(V_i)_{i \in J}$ is a covering of X.*

Let H be the subset of N consisting of indices n such that U_n is contained in at least one of the V_i; the sequence (U_n)_{n \in H} is a covering of X, because every point x \in X belongs to some V_i, and since V_i is open, there is an index n such that x \in U_n \subset V_i. Hence there is a mapping $\psi$ of H into I such that U_n \subset V_{\psi(n)} for each n \in H; taking J = $\psi(H)$, which is countable, the proposition is proved.

### 9. COMPACT METRIC SPACES; COMPACT METRIZABLE SPACES

The criterion for precompactness of a uniform space (Chapter II, § 4, no. 2, Theorem 3) gives rise to the following proposition for metric spaces:

#### Proposition 14 {#top-ix-s2-prop-14 .statement}

*A metric space X is precompact if and only if, for each $\varepsilon > 0$, there is a finite covering of X by sets of diameter $\leq \varepsilon$.*

If we adjoin the hypothesis that X is *complete* we have a criterion for *compactness* of metric spaces.

From Proposition 14 we get a *topological* criterion for compactness, applicable to metrizable spaces:

#### Proposition 15 {#top-ix-s2-prop-15 .statement}

*A metrizable topological space X is compact if and only if every infinite sequence of points of X has a cluster point in X.*

Axiom (C) of Chapter I, § 9, no. 1 shows that the condition is *necessary*. To show *sufficiency*, let d be a metric compatible with the topology of X. We show first that the metric space X so defined is *complete*: every Cauchy sequence in X has a cluster point and is therefore convergent (Chapter II, § 3, no. 2, Proposition 5, Corollary 2); hence X is complete, by Proposition 9. Next we shall show that X is *precompact*; if this were not so, then by Proposition 14 there would exist a real number $\alpha > 0$ such that X could not be covered by any finite number of subsets of X of diameter $\leq \alpha$. We could then define by induction on n an infinite sequence $(x_n)$ of points of X by the condition $d(x_p, x_n) > \frac{1}{2} \alpha$ for all $p < n$; and such a sequence can have no cluster point, since every ball of radius $< \frac{1}{2} \alpha$ contains at most one point of the sequence.

#### Corollary {#top-ix-s2-n9-cor-1 .statement}

*A subset A of a metrizable topological space X is relatively compact if and only if every infinite sequence of points of A has a cluster point in X.*

Let d be a metric compatible with the topology of X. We shall show that the space $\overline{A}$ is compact, by applying the criterion of Proposition 15. Let $(x_n)$ be a sequence of points of $\overline{A}$; then for each index n there exists $y_n \in A$ such that $d(x_n, y_n) < 1/n$; the sequence $(y_n)$ has, by hypothesis, a cluster point $a \in X$, and a is also a cluster point of the sequence $x_i$, for if $y_m$ lies in the ball with centre $a$ and radius $1/n$, for some $m > n$, then $x_m$ lies in the ball with centre $a$ and radius $2/n$.

It should be remarked that Proposition 15 is not a consequence of the existence of a countable fundamental system of neighbourhoods at each point of $X$; there are examples of non-metrizable, non-compact spaces in which every point has a countable fundamental system of neighbourhoods and every infinite sequence of points has a cluster point (Exercise 15).

#### Proposition 16 {#top-ix-s2-prop-16 .statement}

*A compact space $X$ is metrizable if and only if its topology has a countable base.*

The condition is *necessary*. By Proposition 14, for each integer $n \geq 1$ there is a finite subset $A_n$ of $X$ such that the distance of $A_n$ from every point of $X$ is $\leq 1/n$; the countable set $A = \bigcup_n A_n$ is therefore dense in $X$, and the result follows from Proposition 12 of no. 8.

The condition is *sufficient*. Let $(U_n)$ be a countable base of the topology of $X$. Every neighbourhood of a point of the diagonal $\Delta$ of $X \times X$ therefore contains a neighbourhood of the form $U_n \times U_n$; applying the Borel-Lebesgue axiom to the compact subset $\Delta$ of $X \times X$, it follows that every neighbourhood of $\Delta$ contains a finite union of sets of the form $U_n \setminus U_n$, which is a neighbourhood of $\Delta$. Hence the neighbourhoods of $\Delta$ which are finite unions of sets of the form $U_n \times U_n$ form a fundamental system of entourages of the uniformity of $X$ (Chapter II, § 4, no. 1, Theorem 1), and the result therefore follows from Theorem 1 of no. 4.

#### Corollary {#top-ix-s2-n9-cor-2 .statement}

*Let $X$ be a locally compact space and let $X'$ be the compact space obtained by adjoining a point at infinity $\omega$ to $X$ (Chapter I, § 9, no. 8). Then the following statements are equivalent:*

a) *The topology of $X$ has a countable base.*
b) $X'$ *is metrizable.*
c) $X$ *is metrizable and $\sigma$-compact.*

$a \Longrightarrow b$: Let $U_n$ be a countable base of the topology of $X$. Each neighbourhood of a point $x \in X$ contains a compact neighbourhood of $x$, which in turn contains a neighbourhood of $x$ equal to some $U_n$. Hence the relatively compact $U_n$ form a base of the topology of $X$, and we may therefore suppose that all the $U_n$ are relatively compact. $X$ is therefore a countable union of compact sets $\overline{U}_n$, i.e. it is $\sigma$-compact; this implies that in $X'$ the point $\omega$ has a countable fundamental system $V_n$ of open neighbourhoods (Chapter I, § 9, no. 9, Proposition 15, Corollary 2). Hence each neighbourhood of a point $y \in X'$ contains either one of the $U_n$ or one of the $V_n$, which is a neighbourhood of $y$, and so the $U_n$ and the $V_n$ form a countable base of the topology of $X'$. Hence $X'$ is metrizable, by Proposition 16.

b) $\Longrightarrow c)$: If $X'$ is metrizable, then $\omega$ has a countable fundamental system of neighbourhoods, and therefore $X$ is $\sigma$-compact by Chapter I, § 9, no. 9, Proposition 15, Corollary 2.

c) $\Longrightarrow a)$: By hypothesis, there is an increasing sequence $(V_n)$ of relatively compact open sets which cover $X$ and are such that $\overline{V}_n \subset V_{n+1}$ (Chapter I, § 9, no. 9, Proposition 15). The subspace $\overline{V}_n$ is compact and metrizable and therefore has a countable base (Proposition 16), and therefore so does $V_n$. Let $(U_{mn})_{m \geq 1}$ be a base of the topology of $V_n$. For each $x \in X$ and each neighbourhood $W$ of $x$, there exists $n$ such that $x \in V_n$, hence there exists $m$ such that $x \in U_{mn} \subset V_n \cap W$. Hence the sets $U_{mn}$ ($m \geq 1, n \geq 1$) form a base of the topology of $X$.

### 10. QUOTIENT SPACES OF METRIZABLE SPACES

If $X$ is a metrizable space and $R$ is an equivalence relation on $X$, the quotient space $X/R$ is not necessarily metrizable (even if $X$ is locally compact \* and $X/R$ is normal *). However:

#### Proposition 17 {#top-ix-s2-prop-17 .statement}

Every Hausdorff quotient space of a compact metrizable space is compact and metrizable.

Equivalently, if $f$ is a continuous mapping of a compact metrizable space $X$ into a Hausdorff space $X'$, then $f(X)$ is a metrizable subspace of $X'$ (Chapter I, § 9, no. 4, Theorem 2, Corollary 4).

Let $X$ be a compact metrizable space, and let $R$ be an equivalence relation on $X$ such that $X/R$ is Hausdorff. Then $X/R$ is compact (Chapter I, § 9, no. 4, Theorem 2), hence by Proposition 16 it is enough to show that the topology of $X/R$ has a countable base. To do this, we use the facts that $R$ is closed (Chapter I, § 10, no. 4, Proposition 8) and that the classes mod $R$ are compact. Let $\varphi$ be the canonical mapping of $X$ onto $X/R$, and let $(U_n)$ be a countable base of the topology of $X$. Let $z$ be any point of $X/R$ and let $V$ be a neighbourhood of $z$ in $X/R$; then $\overline{\varphi}^{-1}(V)$ is a neighbourhood in $X$ of the compact set $\overline{\varphi}^{-1}(z)$. If $x$ is any point of $\overline{\varphi}^{-1}(z)$, there is a set $U_n$ containing $x$ and contained in $\overline{\varphi}^{-1}(V)$, and therefore by the Borel-Lebesgue axiom there is a finite open covering $(U_{n_k})_{1 \leq k \leq r}$ of $\overline{\varphi}^{-1}(z)$ such that, if $W$ denotes $\bigcup_k U_{n_k}$, $W$ is a neighbourhood of $\overline{\varphi}^{-1}(z)$ contained in $\overline{\varphi}^{-1}(V)$. Since $R$ is closed, it follows that $\varphi(W)$ is a neighbourhood of $z$ in $X/R$, contained in $V$ (Chapter I, § 5, no. 4, Proposition 10). Let $\mathcal{B}$ denote the set of interiors of sets of the form $\varphi(W)$, where $W$ runs through the set $\mathcal{F}$ of all finite unions of sets of the form $U_n$; we have then shown that $\mathcal{B}$ is a base of the topology of $X/R$, and since $\mathfrak{F}$ is countable, so is $\mathcal{B}$.

#### Proposition 18 {#top-ix-s2-prop-18 .statement}

*Let $X$ be a complete metric space, let $R$ be an open equivalence relation on $X$ such that $X/R$ is Hausdorff, and let $\varphi : X \to X/R$ be the canonical mapping. Then if $K$ is any compact subset of $X/R$, there is a compact subset $K'$ of $X$ such that $\varphi(K') = K$.*

Let $\mathcal{B}_1$ be the set of all open balls of radius $1/2$ in $X$. As $B$ runs through $\mathcal{B}_1$, the sets $\varphi(B)$ form an open covering of $K$, and therefore there exists a finite number of points $x_1, \ldots, x_m$ of $X$ such that the images under $\varphi$ of the open balls with radius $1/2$ and centre $x_i$ ($1 \leq i \leq m$) form an open covering of $K$. Let $H_1 = \{ x_1, \ldots, x_m \}$ and suppose that we have defined a finite set $H_i$, for $1 < i \leq n$, such that:

(i) $H_i \subset H_{i+1}$ and each point of $H_{i+1}$ is at a distance $< 1/2^i$ from $H_i$, for $1 \leq i \leq n - 1$;

(ii) the images under $\varphi$ of the open balls of radius $1/2^i$, with centres at the points of $H_i$, form an open covering of $K$, for $1 \leq i \leq n$.

Let $\mathcal{B}_{n+1}$ be the set of all open balls of radius $1/2^{n+1}$ whose centre $x$ is such that $d(x, H_n) < 1/2^n$ ($d$ being the metric on $X$). The properties of $H_n$ show that the sets $\varphi(B)$, for $B \in \mathcal{B}_{n+1}$, form an open covering of $K$; hence there is a finite set $L_{n+1} \subset X$ such that the images under $\varphi$ of the open balls of radius $1/2^{n+1}$ whose centre belongs to $L_{n+1}$ form an open covering of $K$. Taking $H_{n+1} = H_n \cup L_{n+1}$, we see that we can define inductively an infinite sequence $(H_n)$ of finite subsets of $X$ with properties (i) and (ii) above. Let $H = \bigcup_n H_n$, and let us show that $H$ is *precompact*. For each $p > 0$ and each point $z_{n+p} \in H_{n+p}$, there exists a sequence of points $z_{n+i} \in H_{n+i}$ ($0 \leq i \leq p - 1$) such that

$$
d(z_{n+i}, z_{n+i+1}) < 1/2^{n+i} \quad \text{for } 0 \leq i \leq p - 1;
$$

it follows that $d(z_n, z_{n+p}) \leq \sum_{i=0}^{p-1} 1/2^{n+i} \leq 1/2^{n-1}$, and consequently $d(y, H_n) \leq 1/2^{n-1}$ for all $y \in H$, which proves our assertion. Since $X$ is complete, $\overline{H}$ is compact, hence $\varphi(\overline{H})$ is compact. Next, let us show that $K \subset \varphi(\overline{H})$. If $z \in K$, then by definition $d(\overline{H}_n, \overline{\varphi}(z)) \leq 1/2^n$ for all $n$, and therefore $d(\overline{H}, \overline{\varphi}(z)) = 0$; but $\overline{\varphi}(z)$ is closed and $\overline{H}$ is compact, so that this implies $\overline{H} \cap \overline{\varphi}(z) \neq \emptyset$ (no. 2, Remark following Proposition 3); hence the assertion. Thus if $K' = \overline{H} \cap \overline{\varphi}(K)$, then $K'$ is closed in $\overline{H}$ and therefore compact, and from what has been proved we have $\varphi(K') = K$.

Q.E.D.

### Exercises {#top-ix-s2-exercises}

See the [exercises for § 2](exercises/s2/).
