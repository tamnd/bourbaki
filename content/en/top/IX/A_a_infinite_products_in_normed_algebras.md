---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 0
section_title: Infinite products in normed algebras
appendix: true
lang: en
source: top-v-x
book_pages: 268-270
pdf_pages: 0217-0223, 0274-0276
extraction: ocr
subsections:
    - "no": 1
      title: MULTIPLIABLE SEQUENCES IN A NORMED ALGEBRA
      page: 0
      pdf_page: 217
    - "no": 2
      title: MULTIPLIABILITY CRITERIA
      page: 0
      pdf_page: 218
    - "no": 3
      title: INFINITE PRODUCTS
      page: 0
      pdf_page: 221
statements: 16
exercises: 8
content_sha256: 8ac8a39858022c80b0d394946d918655525055ba0ae1ab6a174d3924458ebb1b
---

## APPENDIX

# INFINITE PRODUCTS IN NORMED ALGEBRAS

### 1. MULTIPLIABLE SEQUENCES IN A NORMED ALGEBRA

Let $A$ be a normed algebra over a non-discrete valued field $K$ (Chapter IX, § 3, no. 7, Definition 9); we shall denote by $||x||$ the norm of an element $x \in A$, and we shall assume that this norm satisfies the inequality $||xy|| \leq ||x|| \cdot ||y||$; also we shall assume that $A$ has an identity element $e$.

Let $(x_n)_{n \in \mathbf{N}}$ be an infinite sequence of points of $A$. Every finite subset $J$ of $\mathbf{N}$, linearly ordered by the ordering of $\mathbf{N}$, defines a sequence $(x_n)_{n \in J}$ of points of $A$, and we define the product

$$
p_J = \prod_{n \in J} x_n
$$

of this sequence; this product is called the finite partial product of the sequence $(x_n)_{n \in \mathbf{N}}$, corresponding to the finite subset $J$ of $\mathbf{N}$ (recall that if $J = \varnothing$ we put $\prod_{n \in \varnothing} x_n = e$).

#### Definition 1 {#top-ix-a0-def-1 .statement}

*The sequence* $(x_n)_{n \in \mathbf{N}}$ *is said to be multipliable in the normed algebra* $A$ *if the mapping* $J \to p_J$ *has a limit with respect to the filter of sections of the set* $\mathfrak{F}(\mathbf{N})$ *of finite subsets of* $\mathbf{N}$, *ordered by the relation* $\subset$; *this limit is called the product of the sequence* $(x_n)_{n \in \mathbf{N}}$, *and is denoted by* $\prod_{n \in \mathbf{N}} x_n$ *(or simply* $\prod_n x_n$); *the* $x_n$ *are called the factors of this product.*

Definition 1 is equivalent to the following: *the sequence* $(x_n)$ *is multipliable and its product is* $p$ *if for each* $\varepsilon > 0$ *there exists a finite subset* $J_0$ *of* $\mathbf{N}$ *such that, for every finite subset* $J \supset J_0$ *of* $\mathbf{N}$, *we have* $||p_J - p|| \leq \varepsilon$.

#### Remark 1 {#top-ix-a0-n1-rem-1 .statement}

When $A$ is a commutative algebra, Definition 1 is identical with that given in Chapter III, § 5, no. 1, Remark 3; but when $A$ is not commutative, the order structure of the index set $\mathbf{N}$ is essentially involved in Definition 1. If $\sigma$ is an arbitrary permutation of $\mathbf{N}$, we cannot in general assert that the sequence $(x_{\sigma(n)})$ is multipliable if the sequence (x_n) is multipliable; and if both sequences are multipliable, their products will in general be different.

#### Remark 2 {#top-ix-a0-n1-rem-2 .statement}

Definition 1 can be immediately generalized to the case of a family (x_n)_{n \in I} whose index set I is a subset of \mathbf{Z} (linearly ordered by the order induced by that of \mathbf{Z}). We leave it to the reader to extend to this case the results below (cf. Exercises 1 and 2).

### 2. MULTIPLIABILITY CRITERIA

From now on we shall assume that the normed algebra A is complete.

#### Theorem 1 {#top-ix-a0-thm-1 .statement}

Let (x_n)_{n \in \mathbf{N}} be a sequence of points in a complete normed algebra A.
a) If (x_n) is multipliable and if its product is a unit of A, then for each $\varepsilon > 0$ there exists a finite subset J_0 of \mathbf{N} such that, for every finite subset L of \mathbf{N} which does not meet J_0, we have $\|e - p_L\| \leq \varepsilon$.
b) Conversely, if the sequence (x_n) satisfies this condition, it is multipliable. Moreover, if each x_n is a unit, then $\prod_{n \in \mathbf{N}} x_n$ is a unit.

a) Let p be the product of the multipliable sequence (x_n), and suppose that p is a unit in A; then (Chapter IX, § 3, no. 7, Proposition 13) there exist $\alpha > 0$ and $a > 0$ such that, for all $y \in A$ for which we have
$$
\|y - p\| \leq \alpha,
$$
y is a unit and $\|y^{-1}\| \leq a$. By hypothesis, for every $\varepsilon$ such that $0 < \varepsilon < \alpha$, there is a finite subset H_0 of \mathbf{N} such that, for every finite subset H of \mathbf{N} containing H_0, we have $\|p_H - p\| \leq \varepsilon$. Let $J_0 = [0, m]$ be an interval of \mathbf{N} which contains H_0; for each finite subset L of \mathbf{N} which does not meet J_0, the integers belonging to L are all greater than those belonging to H_0; hence, if $H = H_0 \cup L$, we have $p_H = p_{H_0} p_L$. Now, since $\|p_{H_0} - p\| \leq \varepsilon \leq \alpha$, $p_{H_0}$ is a unit, and
$$
\|e - p_{H_0}^{-1} p\| \leq \varepsilon \|p_{H_0}^{-1} p\| \leq a \varepsilon;
$$
since $\|p_{H_0} p_L - p\| \leq \varepsilon$, we deduce
$$
\|p_L - p_{H_0}^{-1} p\| \leq \varepsilon \|p_{H_0}^{-1}\| \leq a \varepsilon,
$$
and finally $\|e - p_L\| \leq 2a \varepsilon$.

b) Suppose that, for each $\varepsilon > 0$, there exists a finite subset J_0 of \mathbf{N} such that, for every finite subset L of \mathbf{N} which does not meet J_0, we have $\|e - p_L\| \leq \varepsilon$. Let $H_0 = [0, p]$ be an interval of \mathbf{N} which contains J_0; then every finite subset H of \mathbf{N} which contains H_0 can be written in the form $H_0 \cup L$, where the integers in L are all greater than those in H_0; hence we have $p_H = p_{H_0} p_L$, and since L does not meet $J_0$, $\|p_H - p_{H_0}\| \leq \varepsilon \|p_{H_0}\|$, and consequently $\|p_H\| = (1 + \varepsilon)\|p_{H_0}\|$. If $p_{H_0} = 0$, the sequence $(x_n)$ is evidently multipliable and its product is 0; excluding this trivial case, there is an interval $H_1 = [0, q]$ containing $H_0$ and such that, for every finite subset $L$ of $\mathbf{N}$ which does not meet $H_1$, we have $\|e - p_L\| \leq \varepsilon (\|p_{H_0}\|)^{-1}$. As above, it follows that, for each finite subset $H \supset H_1$,

$$
\|p_H - p_{H_1}\| \leq (\|p_{H_0}\|)^{-1}\|p_{H_1}\|\varepsilon \leq \varepsilon (1 + \varepsilon).
$$

Cauchy’s criterion therefore shows that $J \to p_J$ has a limit in $A$ with respect to the directed set $\mathfrak{F}(\mathbf{N})$.

If all the $x_n$ are units, then so are all the finite partial products $p_J$; hence for each finite subset $H$ containing $H_0$ we have

$$
\|e - p_{H_0}^{-1}p_H\| \leq \varepsilon,
$$

and this shows that, in the multiplicative group $G$ of units of $A$, the image under the mapping $J \to p_J$ of the section filter of $\mathfrak{F}(\mathbf{N})$ is a Cauchy filter base with respect to the left uniformity of $G$; but since $G$ is *complete* (Chapter IX, § 3, no. 7, Proposition 13), the limit of the mapping $J \to p_J$ belongs to $G$.

#### Remark {#top-ix-a0-n2-rem-1 .statement}

If $(x_n)$ is multipliable and its product is not a unit, the condition of Theorem 1 is not necessarily satisfied: for example, if all the $x_n$ are equal to the same element $x$, where $\|x\| < 1$, the sequence $(x_n)$ is multipliable and its product is 0, and for each non-empty finite subset $H$ of $\mathbf{N}$, we have $\|p_H\| \leq \|x\| < 1 \leq \|e\|$.

#### Corollary 1 {#top-ix-a0-thm-1-cor-1 .statement}

*If* $(x_n)$ *is a multipliable sequence whose product is a unit of* $A$, *then* $\lim_{n \to \infty} x_n = e$.

#### Corollary 2 {#top-ix-a0-thm-1-cor-2 .statement}

*If* $(x_n)$ *is a multipliable sequence whose product is a unit of* $A$, *then every subsequence* $(x_{n_k})_{k \in \mathbf{N}}$ *of* $(x_n)$ *[$(n_k)$ being a strictly increasing sequence of integers]* *is multipliable*.

This follows immediately from the criterion of Theorem 1.

#### Theorem 2 {#top-ix-a0-thm-2 .statement}

*Let* $A$ *be a complete normed algebra*. *If* $(u_n)$ *is an absolutely convergent series of elements of* $A$, *then the sequence* $(e + u_n)$ *is multipliable in* $A$; *and if all the elements* $e + u_n$ *are units in* $A$, *then so is* $\prod_{n \in \mathbf{N}} (e + u_n)$.

Let us apply the criterion of Theorem 1. For every finite subset $L$ of $\mathbf{N}$, we have $p_L - e = \prod_{n \in L} (e + u_n) - e = \sum_M \left( \prod_{n \in M} u_n \right)$, where $M$ runs through the set of all non-empty subsets of $L$ (linearly ordered by the induced ordering). Since $\prod_{n \in M} u_n \leq \prod_{n \in M} |u_n|$, we may write

$$
||p_1 - e|| = \sum_M (\prod_{n \in M} u_n) \cdot \prod_{i \in I} (1 + |u_i|) - 1.
$$

Now since the series whose general term is $|u_n|$ is convergent by hypothesis, the sequence $1 - |u_n|$ is multipliable in $\mathbf{R}_+^*$ (Chapter IV, § 7, no. 4, Theorem 4). Hence for each $\varepsilon > 0$ there exists a finite subset $J_0$ of $\mathbf{N}$ such that, for every finite subset $L$ of $\mathbf{N}$ which does not meet $J_0$, we have $\left| \prod_{n \in L} (1 + ||u_n||) - 1 \right| \leq \varepsilon$; hence the result.

#### Corollary {#top-ix-a0-n2-cor-1 .statement}

*If the series whose general term is $u_n$ is absolutely convergent, and if none of the elements $e - u_n$ is a zero divisor in $A$, then the product $\prod_{n \in \mathbf{N}} (e + u_n)$ is not a zero divisor in $A$.*

There is only a finite number of integers $n$ such that $|u_n| > 1$. Let $J = [a, m]$ be an interval of $\mathbf{N}$ containing all these integers. The product of the sequence $(e + u_n)$ is the product of $p_J$ and the element $\prod_{n \notin J} (e - u_n)$, all of whose factors are units (Chapter IX, § 3, no. 7, Corollary to Proposition 12), and is therefore itself a unit; since $p_J$ is the product of a finite number of non-zero divisors, it is not a zero divisor, and hence $\prod_{n \in \mathbf{N}} (e + u_n)$ is not a zero divisor.

The sufficient condition for multipliability given by Theorem 2 is not in general necessary (cf. Exercise 6). However, it is necessary in the important case where $A$ is an algebra of finite rank over the field $\mathbf{R}$ (i.e., $A$ is finite-dimensional as a vector space over $\mathbf{R}$); in particular this is the case if $A$ is the division ring of quaternions $\mathbf{H}$, or a matrix algebra $\mathbf{M}_n(\mathbf{R})$:

#### Proposition 1 {#top-ix-a0-prop-1 .statement}

*Let $A$ be a normed algebra of finite rank over $\mathbf{R}$. If $(e + u_n)$ is a multipliable sequence in $A$, whose product is a unit of $A$, then the series whose general term is $u_n$ is absolutely convergent.*

From Chapter VII, § 3, no. 1, Proposition 2, there exists a number $c > 0$ such that, for every finite family $(x_i)_{i \in I}$ of points of $A$, we have

$$
\sum_{i \in I} \|x_i\| \leq c \sup_{J \subset I} \left| \sum_{i \in J} x_i \right|.
$$

Let $(a_i)_{i \in \mathbf{N}}$ be an arbitrary sequence of elements of $A$. For each finite subset $I$ of $\mathbf{N}$, put

$$
p_I = \prod_{i \in I} (e + a_i), \quad s_I = \sum_{i \in I} a_i, \quad \sigma_I = \sum_{i \in I} \|a_i\|.
$$

#### Lemma 1 {#top-ix-a0-lem-1 .statement}

For each finite subset $I$ of $\mathbf{N}$, let $\varphi(I) = \sup_{J \subset I} ||p_J - e||$. Then for each subset $J$ of $I$ we have

$$
||p_J - e - s_J|| \leq \varphi(I)\sigma_J.
$$

The lemma is obvious if $J$ is empty; we shall prove it by induction on the number of elements in $J$. Let $J = K \cup \{j\}$, where $\{j\}$ is strictly larger than every $i \in K$. Then $p_J = p_K(e + a_j)$ and

$$
s_J = s_K + a_j,
$$

so that

$$
p_J - e - s_J = p_K - e - s_K + (p_K - e)a_j,
$$

and by the inductive hypothesis and the definition of $\varphi(I)$, we have

$$
||p_J - e - s_J|| \leq \varphi(I)\sigma_K + \varphi(I)||a_j|| = \varphi(I)\sigma_J,
$$

which proves the lemma.

#### Lemma 2 {#top-ix-a0-lem-2 .statement}

If $I$ is a finite subset of $\mathbf{N}$ such that $\varphi(I) < 1/c$, then

$$
\sigma_I \leq c\varphi(I)/(1 - c\varphi(I)).
$$

For since $\sigma_J \leq \sigma_I$ for every subset $J$ of $I$, we have from (2)

$$
||s_J|| \leq \varphi(I)\sigma_I + ||p_J - e|| \leq (1 + \sigma_I)\varphi(I);
$$

and since also $\sigma_I \leq c \cdot \sup_{J \subset I} ||s_J||$, from (1), it follows that

$$
\sigma_I \leq c\varphi(I)(1 + \sigma_I),
$$

which leads to the result.

Now let $(e + u_n)$ be a multipliable sequence in $A$, whose product is a unit; by Theorem 1 there exists a finite subset $J_0$ of $\mathbf{N}$ such that, for each finite subset $H$ of $\mathbf{N}$ which does not meet $J_0$, we have

$$
\left| \prod_{i \in H} (e + u_i) - e \right| \leq 1/2c.
$$

By Lemma 2, it follows that $\sum_{i \in H} ||u_i|| - 1$ for every finite subset $H$ of $\mathbf{N}$ which does not meet $J_0$, and hence (Chapter IV, § 7, no. 1, Theorem 1) the family $(||u_n||)$ is summable in $\mathbf{R}$.

### 3. INFINITE PRODUCTS

To each sequence $(x_n)$ of points in a normed algebra $A$, let us make correspond the sequence of *partial products* $p_n = \prod_{k=0}^n x_k$; then the *pair* of sequences $(x_n)$ and $(p_n)$ is called the infinite product whose general factor is $x_n$. The infinite product with general factor $x_n$ is said to be convergent if the sequence $(p_n)$ is convergent in $A$; the limit of this sequence is then called the product of the sequence $(x_n)$ and is denoted by $\prod_{n=0}^\infty x_n$.

#### Proposition 2 {#top-ix-a0-prop-2 .statement}

*Let* $(x_n)$ *be a sequence of points in a complete normed algebra* $A$.

a) *If the infinite product whose general factor is* $x_n$ *is convergent and if* $\prod_{n=0}^\infty x_n$ *is a unit in* $A$, *then for each* $\varepsilon > 0$ *there exists an integer* $n_0$ *such that*
$$
\left\| \prod_{k=m}^n x_k - e \right\| \leq \varepsilon
$$
*whenever* $n_0 \leq m \leq n$.

b) *Conversely, if the sequence* $(x_n)$ *satisfies this condition, the infinite product with general factor* $x_n$ *is convergent; and if each of the* $x_n$ *is a unit in* $A$, *then* $\prod_{n=0}^\infty x_n$ *is a unit*.

The proof of this proposition follows step by step the proof of Theorem 1, and is left to the reader (the finite subsets $L$ of $N$ in the proof of Theorem 1 are to be replaced by intervals).

#### Corollary 1 {#top-ix-a0-prop-2-cor-1 .statement}

*If the infinite product with general factor* $x_n$ *is convergent, and if* $\prod_{n=0}^\infty x_n$ *is a unit*, *then* $\lim_{n \to \infty} x_n = e$.

#### Corollary 2 {#top-ix-a0-prop-2-cor-2 .statement}

*If the infinite product with general factor* $x_n$ *is convergent, and if* $\prod_{n=0}^\infty x_n$ *is a unit*, *then the infinite product with general factor*
$$
y_n = x_{n+h} \quad (n \geq 0)
$$
*is convergent*.

The product of the sequence $(y_n)$ is denoted by $\prod_{n=h}^\infty x_n$, and is also called the residue of index $h$ of the infinite product with general factor $x_n$.

Still under the assumption that $\prod_{n=h}^\infty x_n$ is a unit, it follows from Proposition 2 that if $(z_n)$ is a sequence such that $z_n = x_n$ for all but a finite number of indices, then the product with general factor $z_n$ is convergent.

#### Proposition 3 {#top-ix-a0-prop-3 .statement}

*Let* $(k_n)$ *be a strictly increasing sequence of integers* $\geq 0$, *such that* $k_0 = 0$; *if the infinite product with general factor* $x_n$ *converges*, *and* if we put

$$
u_n = \prod_{p=k_n}^{k_{n+1}-1} x_p,
$$

then the infinite product whose general factor is $u_n$ is convergent and we have

$$
\prod_{n=0}^{\infty} u_n = \prod_{n=0}^{\infty} x_n.
$$

For the sequence of partial products of the sequence $(u_n)$ is a subsequence of the sequence of partial products of the sequence $(x_n)$.

Finally, the same argument as was used for abelian groups (Chapter III, § 5, no. 7) shows that if a sequence $(x_n)$ in a normed algebra $\mathbf{A}$ is *multiplicable*, then the product whose general factor is $x_n$ is convergent, and

$$
\prod_{n=0}^{\infty} x_n = \prod_{n \in \mathbf{N}} x_n
$$

(which is also written as $\prod_{n=0}^{\infty} x_n$); the converse is of course not true (cf. Exercise 7).

### Exercises {#top-ix-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
