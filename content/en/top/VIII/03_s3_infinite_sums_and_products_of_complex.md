---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 3
section_title: Infinite sums and products of complex numbers
lang: en
source: top-v-x
pdf_pages: 0121-0124, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: INFINITE SUMS OF COMPLEX NUMBERS
      page: 0
      pdf_page: 121
    - "no": 2
      title: MULTIPLIABLE FAMILIES IN $\mathbf{C}^*$
      page: 0
      pdf_page: 121
    - "no": 3
      title: INFINITE PRODUCTS OF COMPLEX NUMBERS
      page: 0
      pdf_page: 123
statements: 9
exercises: 5
content_sha256: ae4b4fbbeeb49bd4c4110407841c8096fb7aa47e7ae95f9f57dd94c73c707730
---

## 3. INFINITE SUMS AND PRODUCTS OF COMPLEX NUMBERS

### 1. INFINITE SUMS OF COMPLEX NUMBERS

Since the additive group of the field $\mathbf{C}$ is the same as the additive group $\mathbf{R}^2$, it is not necessary to make a special study of summable families and series in $\mathbf{C}$, since this is included in the general theory of Chapter VII, § 3; we leave to the reader the exercise of translating the results of this theory into the language of the theory of complex numbers. We state only the following proposition, which is a corollary to Proposition 3 of Chapter VII, § 3, no. 1:

#### Proposition 1 {#top-viii-s3-prop-1 .statement}

*If* $(u_\lambda)_{\lambda \in L}$ *and* $(v_\mu)_{\mu \in M}$ *are two summable families of complex numbers, then the family* $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M}$ *is summable and we have*

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right).
$$

We leave it to the reader to state the corresponding result for quaternions.

### 2. MULTIPLIABLE FAMILIES IN $\mathbf{C}^*$

In the multiplicative group $\mathbf{C}^*$ of non-zero complex numbers a family $(z_i)_{i \in I}$ cannot be multipliable unless $\lim z_i = 1$ with respect to the filter of complements of finite subsets of $I$ (Chapter III, § 5, no. 2, Proposition 1); furthermore, since every point of $\mathbf{C}^*$ has a countable fundamental system of neighbourhoods, the set of indices $i$ such that $z_i \neq 1$ is countable if the family $(z_i)$ is multipliable (Chapter III, § 5, no. 2, Corollary to Proposition 1).

#### Proposition 2 {#top-viii-s3-prop-2 .statement}

*A family* $(z_i)$ *of complex numbers* $z_i = r_i (\cos \theta_i + i \sin \theta_i)$ *is multipliable if and only if the family* $(r_i)$ *of absolute values of the* $z_i$ *is multipliable in* $\mathbf{R}_+^*$ *and the family* $(\theta_i)$ *of amplitudes of the* $z_i$ *is summable in the group of angles* $\mathfrak{A}$.

In view of the structure of the group $\mathbf{C}^*$ ($\S$ 1, no. 3, Proposition 1), the proposition is an immediate consequence of Proposition 4 of Chapter III, $\S$ 5, no. 4.

If we map each angle $\theta$ to that one of its measures (to any given base $a$) which belongs to the interval $] - \frac{1}{2} a, \frac{1}{2} a ]$, we have a *local isomorphism* of $\mathfrak{A}$ with $\mathbf{R}$ ($\S$ 2, no. 2); since $\lim \theta_i = 0$ with respect to the filter of complements of finite subsets of $I$, we may replace the condition (in the statement of Proposition 2) that the family $\theta_i$ should be summable in $\mathfrak{A}$ by the condition that the family $(t_i)$ of *measures* of the angles $\theta_i$ which belong to $] - \frac{1}{2} a, \frac{1}{2} a ]$ should be summable in $\mathbf{R}$.

The following theorem gives another criterion for a family of complex numbers, put in the form $(1 + u_i)$, to be multipliable in $\mathbf{C}^*$. (It generalizes Theorem 4 of Chapter IV, $\S$ 7, no. 4; see also Chapter IX, Appendix, no. 2, Proposition 1):

#### Theorem 1 {#top-viii-s3-thm-1 .statement}

*The family* $(1 + u_i)_{i \in I}$ *is multipliable in* $\mathbf{C}^*$ *if and only if the family* $(|u_i|)$ *is summable in* $\mathbf{R}$.

For each finite subset $J$ of $I$, put

$$
p_J = \prod_{i \in J} (1 + a_i), \quad s_J = \sum_{i \in J} a_i, \quad \sigma_J = \sum_{i \in J} |a_i|.
$$

#### Lemma 1 {#top-viii-s3-lem-1 .statement}

*For each finite subset* $J$ *of* $I$, *let* $\varphi(J) = \sup_{L \subset J} (p_L - 1)$. *Then for each subset* $L$ *of* $J$ *we have*

$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_L.
$$

This is clear if $L$ is empty. We proceed by induction on card $(L)$. Let $L = K \cup \{ \lambda \}$, where $\lambda \notin K$; then $p_L = p_K (1 + a_\lambda)$ and $s_L = s_K + a_\lambda$, so that $p_L - 1 - s_L = (p_K - 1 - s_K) + (p_K - 1)a_\lambda$; hence, by the inductive hypothesis and the definition of $\varphi(J)$, we have

$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_K + \varphi(J)|a_\lambda| = \varphi(J) \sigma_L,
$$

which proves the lemma.

#### Lemma 2 {#top-viii-s3-lem-2 .statement}

*If* $J$ *is a finite subset of* $I$ *such that* $\varphi(J) < 1/4$, *then*

$$
|\sigma_J| \leq 4 \varphi(J)/(1 - 4 \varphi(J)).
$$

For since $\sigma_L \leq \sigma_J$ for all subsets $L$ of $J$, it follows from (2) that $|s_L| \leq \varphi(J) \sigma_J + |p_L - 1| \leq (1 + \sigma_J)\varphi(J)$; but by virtue of Chapter VII, $\S$ 3, no. 1, Proposition 2, we have $|\sigma_J| \leq 4 \sup_{L \subset J} |s_L|$, hence $\sigma_J \leq 4 \varphi(J)(1 + \sigma_J)$, and the result follows.

Now let us show that the condition stated in Theorem 1 is sufficient. The hypothesis that the family $(|u_i|)$ is summable in $\mathbf{R}$ implies that the family $(1 + |u_i|)$ is multipliable in $\mathbf{R}_+^*$ (Chapter IV, § 7, no. 4, Theorem 4); hence, for each $\varepsilon > 0$, there is a finite subset $J_0$ of $I$ such that, for each finite subset $L$ of $I$ which does not meet $J_0$, we have $\prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon$. But we can write $\prod_{i \in L} (1 + u_i) - 1$ in the form $\sum_M \left( \prod_{i \in M} u_i \right)$ where $M$ runs through all non-empty subsets of $L$; and since $\left| \prod_{i \in M} u_i \right| = \prod_{i \in M} |u_i|$, we have

$$
\left| \prod_{i \in L} (1 + u_i) - 1 \right| \leq \sum_M \left( \prod_{i \in M} |u_i| \right) = \prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon.
$$

This proves our assertion, by virtue of Cauchy’s criterion, since $\mathbf{C}^*$ is a complete group.

We still have to show that the condition of Theorem 1 is necessary. If $(1 + u_i)_{i \in I}$ is a multipliable family in $\mathbf{C}^*$, there exists a finite subset $J$ of $I$ such that, for every finite subset $H$ of $I$ which does not meet $J$, we have $\left| \prod_{i \in H} (1 + u_i) - 1 \right| \leq 1/8$. By Lemma 2, it follows that $\sum_{i \in H} |u_i| \leq 1$ for every finite subset $H$ of $I$ which does not meet $J$, and hence the family $(|u_i|)$ is summable in $\mathbf{R}$ (Chapter IV, § 7, no. 1, Theorem 1).

The proof above applies also, mutatis mutandis, to (ordered) infinite products in certain non-commutative division rings and algebras (see Exercise 6, and Chapter IX, Appendix).

### 3. INFINITE PRODUCTS OF COMPLEX NUMBERS

For an infinite product of non-zero complex numbers with general factor $z_n = r_n (\cos \theta_n + i \sin \theta_n)$ to be convergent in $\mathbf{C}^*$, it is necessary and sufficient, from the structure of the group $\mathbf{C}^*$, that the product with general factor $r_n$ converge in $\mathbf{R}_+^*$ and the series with general term $t_n$ (the measure of $\theta_n$ which lies in ]$-\frac{1}{2}a$, $\frac{1}{2}a$]) converge in $\mathbf{R}$.

#### Definition 1 {#top-viii-s3-def-1 .statement}

*An infinite product of complex numbers, with general factor* $1 + u_n$, *is said to be absolutely convergent if the product with general factor* $1 + |u_n|$ *is convergent* (or, equivalently, if the series with general term $|u_n|$ is convergent).

#### Proposition 3 {#top-viii-s3-prop-3 .statement}

*An infinite product of complex numbers is commutatively convergent if and only if it is absolutely convergent.*

#### Remark 1 {#top-viii-s3-n3-rem-1 .statement}

The product with general factor $|1 + u_n|$ can be convergent, and indeed absolutely convergent in $\mathbf{R}_i^*$, without the convergence of the product with general factor $1 + |u_n|$ (see Exercise 4); of course, this cannot happen if all the $u_n$ are real and $> 0$ from a certain index onwards.

#### Remark 2 {#top-viii-s3-n3-rem-2 .statement}

As already remarked for products of factors $> 0$, the convergence of the series with general term $u_n$ is neither necessary nor sufficient for the convergence of the product with general factor $1 + u_n$.

### Exercises {#top-viii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
