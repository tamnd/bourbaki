---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 3
section_title: The field of real numbers
lang: en
source: top-i-iv
book_pages: 339-342, 387-388
pdf_pages: 0345-0348, 0393-0394
extraction: ocr
subsections:
    - "no": 1
      title: MULTIPLICATION IN $\mathbf{R}$
      page: 339
      pdf_page: 345
    - "no": 2
      title: THE MULTIPLICATIVE GROUP $\mathbf{R}^*$
      page: 340
      pdf_page: 346
    - "no": 3
      title: '*n*TH ROOTS'
      page: 341
      pdf_page: 347
statements: 2
exercises: 3
content_sha256: 09a06def0cc19a2ce6d07eac5e95043aaf4755cf250d11490f88581170d128d1
---

## 3. THE FIELD OF REAL NUMBERS

### 1. MULTIPLICATION IN $\mathbf{R}$

The topology of the rational line $\mathbf{Q}$ is compatible not only with the *additive group* structure, but also with the *field* structure of $\mathbf{Q}$. For the function $xy$ is continuous at $(0, 0) \in \mathbf{Q} \times \mathbf{Q}$, since for each integer $n > 0$ the relations $|x| \leq 1/n$ and $|y| \leq 1/n$ together imply that $|xy| \leq 1/n^2 \leq 1/n$; on the other hand, if $a$ is any non-zero rational number, the function $ax$ is continuous at $x = 0$, since for each integer $n > 0$ the relation $|x| \leq 1/|n|a|$ implies that $|ax| \leq 1/n$. This shows that $xy$ is continuous at every point of $\mathbf{Q} \times \mathbf{Q}$ (Chapter III, § 6, no. 3).

To show that $1/x$ is continuous on $\mathbf{Q}^*$ we shall establish more precisely that $1/x$ is *uniformly continuous* (with respect to the additive structure) in the complement of any neighbourhood V of 0. Namely we have $$
\left| \frac{1}{x} - \frac{1}{y} \right| = \frac{|x-y|}{xy}
$$; there exists an integer $m > 0$ such that $|x| \geq 1/m$ for each $x \in \mathcal{G}_V$; if $x$ and $y$ are any two points of $\mathcal{G}_V$ such that $|x-y| \leq 1/m^2 n$, we shall then have $$
\left| \frac{1}{x} - \frac{1}{y} \right| \leq \frac{1}{n}.
$$

#### Proposition 1 {#top-iv-s3-prop-1 .statement}

*The functions xy and $1/x$, defined respectively on $\mathbf{Q} \times \mathbf{Q}$ and $\mathbf{Q}^*$, can be extended by continuity to $\mathbf{R} \times \mathbf{R}$ and $\mathbf{R}^*$ respectively, and define a field structure on $\mathbf{R}$. Endowed with this structure, $\mathbf{R}$ is called the field of real numbers.*

All the properties of topological fields established in § 6 of Chapter III are of course applicable; in particular, every *rational function* of $n$ real variables, with real coefficients, is *continuous* at every point of $\mathbf{R}^n$ where its denominator does not vanish.

### 2. THE MULTIPLICATIVE GROUP $\mathbf{R}^*$

We know from Chapter III, § 6, no. 7, that the topology induced on $\mathbf{R}^*$ by the topology of the real line is *compatible* with the multiplicative group structure of $\mathbf{R}^*$; since $\mathbf{R}^*$ is an *open* subset of the locally compact space $\mathbf{R}$, it follows that $\mathbf{R}^*$ is a *locally compact* topological group (Chapter I, § 9, no. 7, Proposition 13) and is therefore *complete* (Chapter III, § 3, no. 3, Corollary 1 to Proposition 4; this follows also from Chapter III, § 6, no. 8, Proposition 8); of course, this latter property relates to the *multiplicative* uniformity on $\mathbf{R}^*$ and not to the uniformity induced on $\mathbf{R}^*$ by the additive uniformity of $\mathbf{R}$.

The function $xy$ maps the set $\mathbf{Q}_+ \times \mathbf{Q}_+$ into $\mathbf{Q}_+$, and therefore it maps $\mathbf{R}_+ \times \mathbf{R}_+$ into $\mathbf{R}_+$ (Chapter I, § 2, no. 1, Theorem 1); in other words, *the product of two real numbers $\geqslant 0$ is $\geqslant 0$*. The formulae $(-x)y = -xy$ and $(-x)(-y) = xy$ then show that the product of a number $\geqslant 0$ and a number $\leqslant 0$ is $\leqslant 0$, and that the product of two numbers $\leqslant 0$ is $\geqslant 0$; from this it follows that

$$(1)$$
$$|xy| = |x| \cdot |y|$$

(which might also have been obtained by extension of the corresponding relation on $\mathbf{Q} \times \mathbf{Q}$).

If $x > 0$ and $y > 0$ we have $xy \neq 0$, and therefore $xy > 0$; likewise, if $x < 0$ and $y > 0$, then $xy < 0$; and if $x < 0$ and $y < 0$, then $xy > 0$. In particular, if $x \neq 0$ we have $x^2 > 0$, so that a *sum of squares* of real numbers cannot be zero unless each of the numbers is zero.

If $x > 0$ and $y \leqslant z$ (resp. $y < z$) we have $xy \leqslant xz$ (resp. $xy < xz$) in other words, *a homothety of ratio* $> 0$ *preserves order on* $\mathbf{R}$. Since $(-x)y = -xy$, a homothety of ratio $< 0$ changes the ordering on $\mathbf{R}$ into the opposite ordering.

If $x > 0$ we have $1/x > 0$, since $x.(1/x) = 1 > 0$. If $0 < x < y$ we have $xy > 0$, hence $x.(1/xy) < y.(1/xy)$, that is $1/y < 1/x$. Hence the mapping $x \to 1/x$ of the set $\mathbf{R}_+^*$ of real numbers $> 0$ onto itself is strictly decreasing.

We see in the same way that the function $1/x$ is strictly decreasing in ]$\leftarrow, 0[$, and therefore the function $\frac{1}{x-a}$ is strictly decreasing in each of the intervals ]$\leftarrow, a[$ and $]a, \to[$.

It follows from what precedes that $\mathbf{R}_+^*$ is a subgroup of the multiplicative group $\mathbf{R}^*$; moreover, the order relation $x \leq y$ is compatible with the multiplicative, group structure of $\mathbf{R}_+^*$; in other words, $\mathbf{R}_+^*$ is a linearly ordered group.

The fact that the product of two real numbers $\geq 0$ is $\geq 0$ can be expressed by saying that $\mathbf{R}$ is an ordered field: all the above properties are common to all ordered fields.

#### Proposition 2 {#top-iv-s3-prop-2 .statement}

*The multiplicative group $\mathbf{R}^*$ of real numbers $\neq 0$ is a topological group isomorphic to the product of its subgroups $\mathbf{R}_+^*$ and $\mathbf{U}_0$, where*

$$
\mathbf{U}_0 = \{ -1, +1 \}.
$$

For each $x \neq 0$ let $\operatorname{sgn} x$ denote $\frac{x}{|x|}$ (*sign of* $x$). The function $\operatorname{sgn}$ is a homomorphism of $\mathbf{R}^*$ onto $\mathbf{U}_0$. We have $x = |x|\operatorname{sgn} x$, and this decomposition of $x$ as the product of an element of $\mathbf{R}_+^*$ and an element of $\mathbf{U}_0$ is unique; hence the group structure of $\mathbf{R}^*$ is the product of the group structures of $\mathbf{R}_+^*$ and $\mathbf{U}_0$. On the other hand, the mapping $x \to |x|$ is continuous, and so is $x \to \operatorname{sgn} x = \frac{x}{|x|}$, since $x \neq 0$. Hence the result.
We extend the function $\operatorname{sgn}$ to the whole of $\mathbf{R}$ by putting $\operatorname{sgn} 0 = 0$.

We shall see in Chapter V (§ 4, no. 1, Theorem 1) that the topological group $\mathbf{R}_+^*$ is *isomorphic* to the *additive* group $\mathbf{R}$; this will complete the determination of the structure of the topological group $\mathbf{R}_*$.

### 3. *n*TH ROOTS

Let $n$ be any integer $> 0$. From the relation $0 < x < y$ we deduce, by induction on $n$, that $0 < x^n < y^n$. In other words, the function $x \to x^n$ is *strictly increasing* for $x \geq 0$; it is clearly continuous at every point and therefore (§ 2, no. 6, Theorem 5) it is a homeomorphism of $\mathbf{R}_+$ onto an interval $I$. On the other hand, since $x \geqslant 1$ implies $x^{n-1} \geqslant 1$ and therefore $x^n \geqslant x$, it follows that $I$ is not bounded and hence $I = \mathbf{R}_+$. The value, for $x \geqslant 0$, of the inverse of the mapping $x \to x^n$ is denoted by $x^{1/n}$ or $\sqrt[n]{x}$ and is called $x$ to the power $1/n$ or the nth root of $x$ (for $n = 2, 3$ we say square root, cube root; for $n = 2$ we write $\sqrt{x}$ in place of $\sqrt[2]{x}$). The positive number $x^{1/n}$ is thus defined as the unique positive solution of the equation

$$
y^n = x \quad (x \geqslant 0).
$$

In particular we see that there is a real number $x$ such that $x^2 = 2$, whereas no rational number has this property; thus we recover the fact that the rational line $\mathbf{Q}$ is not a complete space.

The mapping $x \to x^{1/n}$ of $\mathbf{R}_+$ onto itself is strictly increasing and continuous. By (2) we have $0^{1/n} = 0, 1^{1/n} = 1$, also

$$
(xy)^{1/n} = x^{1/n} y^{1/n};
$$

hence $x \to x^{1/n}$ is an automorphism of the topological group $\mathbf{R}_+^*$.

In Chapter V, § 4, no. 1, we shall generalize this result by finding all the automorphisms of the multiplicative group $\mathbf{R}_+^*$.

### Exercises {#top-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
