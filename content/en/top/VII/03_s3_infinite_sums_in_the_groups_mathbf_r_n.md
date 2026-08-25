---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 3
section_title: Infinite sums in the groups $\mathbf{R}^n$
lang: en
source: top-v-x
pdf_pages: 0089-0092, 0101-0102
extraction: ocr
subsections:
    - "no": 1
      title: SUMMABLE FAMILIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 89
    - "no": 2
      title: SERIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 92
statements: 9
exercises: 2
content_sha256: 63ba3a9e422d70448db18bbb1c82a9347f390a6d75ddb2e4e632006793a8a2bc
---

## 3. INFINITE SUMS IN THE GROUPS $\mathbf{R}^n$

### 1. SUMMABLE FAMILIES IN $\mathbf{R}^n$

Since every point of $\mathbf{R}^n$ has a *countable* fundamental system of neighbourhoods, a family $(x_t)$ of points of the additive group $\mathbf{R}^n$ is summable only if the set of indices $t$ such that $X_t \neq 0$ is *countable* (Chapter III, \S 5, no. 2, Corollary to Proposition 1); hence, essentially, the study of summable

#### Proposition 1 {#top-vii-s3-prop-1 .statement}

*A family* $(x_i)_{i \in I}$ *of points* $x_i = (x_{i,k})_{1 \leq k \leq n}$ *of* $\mathbf{R}^n$ *is summable if and only if each of the* $n$ *families* $(x_{i,k})_{i \in I}$ *of real numbers is summable in* $\mathbf{R}$.

This follows from Chapter III, § 5, no. 4, Proposition 4.

The condition of Proposition 1 may be transformed as follows:

#### Theorem 1 {#top-vii-s3-thm-1 .statement}

*A family* $(x_i)_{i \in I}$ *of points of* $\mathbf{R}^n$ *is summable if and only if the family* $(||x_i||)$ *of Euclidean norms of the* $x_i$ *is summable in* $\mathbf{R}$.

This follows without trouble from Proposition 1, the condition for summability of a family of real numbers (Chapter IV, § 7, no. 2, Theorem 3), the inequalities

$$
\sup_{1 \leq k \leq n} |x_{i,k}| \leq ||x_i|| \leq \sum_{i=1}^n |x_{i,i}|,
$$

and the comparison principle (Chapter IV, § 7, no. 1, Theorem 2).

One can also proceed somewhat differently, by first establishing the following proposition:

#### Proposition 2 {#top-vii-s3-prop-2 .statement}

*If* $(x_i)_{i \in I}$ *is any finite family of points in* $\mathbf{R}^n$, *then*

$$
\sum_{i \in I} ||x_i|| \leq 2n \cdot \sup_{J \subset I} \left| \sum_{i \in J} x_i \right|.
$$

For if $x_i = (x_{ij})_{1 \leq j \leq n}$, we have $||x_i|| \leq \sum_{j=1}^n |x_{ij}|$, hence

$$
\sum_{i \in I} ||x_i|| \leq \sum_{j=1}^n \left( \sum_{i \in I} |x_{ij}| \right).
$$

Now $\sum_{i \in I} |x_{ij}| = \sum_{i \in I} x_{ij}^+ + \sum_{i \in I} x_{ij}^-$, and since for every subset $J$ of $I$ we have

$$
-\sum_{i \in I} x_{ij}^- \leq -\sum_{i \in J} x_{ij}^- \leq \sum_{i \in J} x_{ij}^+ \leq \sum_{i \in I} x_{ij}^+
$$

it follows that

$$
\sum_{i \in I} |x_{ij}| \leq 2 \cdot \sup_{J \subset I} \left| \sum_{i \in J} x_{ij} \right|.
$$

But $\left| \sum_{i \in J} x_{ij} \right| \leq \left| \sum_{i \in J} x_{ij} \right|$, hence the inequality (1).

Now, Theorem 1 is equivalent to the following proposition (since $\mathbf{R}^n$ is a complete group): the family $(x_i)$ satisfies Cauchy’s criterion (Chapter III, § 5, no. 2, Theorem 1) if and only if the family $(||x_i||)$ also satisfies Cauchy’s criterion. Now the triangle inequality shows that this condition is sufficient, and the inequality (1) shows that it is necessary.

Furthermore we have the inequality

$$
\left| \sum_i x_i \right| \leq \sum_i ||x_i||
$$

which comes by passing to the limit from the analogous inequality for finite partial sums.

#### Corollary {#top-vii-s3-n1-cor-1 .statement}

*A family* $(x_i)$ *of points of* $\mathbf{R}^n$ *is summable if and only if the set of finite partial sums of the family is bounded in* $\mathbf{R}^n$.

By Theorem 1 and the triangle inequality, this condition is necessary; it is sufficient by the inequality (1) and Theorem 1.

#### Proposition 3 {#top-vii-s3-prop-3 .statement}

*Let* $(x_\lambda)_{\lambda \in L}$ *be a summable family of points of* $\mathbf{R}^m$, $(y_\mu)_{\mu \in M}$ *a summable family of points of* $\mathbf{R}^n$, *and let* $f$ *be a bilinear mapping of* $\mathbf{R}^m \times \mathbf{R}^n$ *into* $\mathbf{R}^p$. *Then the family* $(f(x_\lambda, y_\mu))_{(\lambda, \mu) \in L \times M}$ *is summable and we have*

$$
\sum_{(\lambda, \mu) \in L \times M} f(x_\lambda, y_\mu) = f \left( \sum_{\lambda \in \mu} x_\lambda, \sum_{\mu \in M} y_\mu \right).
$$

To show that the family $(f(x_\lambda, y_\mu))$ is summable, it is sufficient by Proposition 1 to establish that each of the $p$ families formed by the coordinates of the points $f(x_\lambda, y_\mu)$ in $\mathbf{R}^n$ is summable: in other words, we can restrict ourselves to the case where $f$ is a bilinear *form*; but for such a form $f$ we have

$$
f(x, y) = \sum_{i, j} a_{ij} x_i y_j,
$$

and therefore we are brought back to the case $f(x, y) = x_i y_j$, and in this case the result has already been proved (Chapter IV, § 7, no. 3, Proposition 1).

By specializing the function $f$ we obtain in particular the following corollaries:

#### Corollary 1 {#top-vii-s3-prop-3-cor-1 .statement}

*If* $(a_\lambda)_{\lambda \in L}$ *is a summable family of real numbers and if* $(x_\mu)_{\mu \in M}$ *is a summable family of points of* $\mathbf{R}^n$, *then the family* $(a_\lambda x_\mu)_{(\lambda, \mu) \in L \times M}$ *is summable and we have*

$$
\sum_{(\lambda, \mu) \in L \times M} a_\lambda x_\mu = \left( \sum_{\lambda \in L} a_\lambda \right) \left( \sum_{\mu \in M} x_\mu \right).
$$

#### Corollary 2 {#top-vii-s3-prop-3-cor-2 .statement}

*If* $(x_\lambda)_{\lambda \in L}$ *and* $(y_\mu)_{\mu \in M}$ *are two summable families of points of* $\mathbf{R}^n$, *then the family* $(x_\lambda | y_\mu)$ *(cf. Chapter VI, § 2, no. 2)* *is summable in* $\mathbf{R}$, *and we have*

$$
\sum_{(\lambda, \mu) \in L \times M} (x_\lambda | y_\mu) = \left( \sum_{\lambda \in L} x_\lambda \middle| \sum_{\mu \in M} y_\mu \right).
$$

### 2. SERIES IN $\mathbf{R}^n$

A series whose general term is $x_m = (x_{mi})_{1 \leq i \leq n}$ converges in $\mathbf{R}^n$ if and only if each of the $n$ series $(x_{mi})_{m \in \mathbf{N}}$ converges in $\mathbf{R}$.

#### Definition 1 {#top-vii-s3-def-1 .statement}

*A series of points of* $\mathbf{R}^n$ *is said to be absolutely convergent if the series of Euclidean norms of its terms is convergent.*

#### Proposition 4 {#top-vii-s3-prop-4 .statement}

*A series of points of* $\mathbf{R}^n$ *is commutatively convergent if and only if it is absolutely convergent.*

This is a consequence of Proposition 9 of Chapter III, § 5, no. 7 and Theorem 1 above.

The examples given in Chapter IV, § 7 show that a series in $\mathbf{R}^n$ can be *convergent* without being *absolutely convergent*.

### Exercises {#top-vii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
