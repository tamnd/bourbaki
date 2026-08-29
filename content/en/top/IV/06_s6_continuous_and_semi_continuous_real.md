---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 6
section_title: Continuous and semi-continuous real-valued functions
lang: en
source: top-i-iv
book_pages: 359-363, 393-397
pdf_pages: 0365-0369, 0399-0403
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS REAL-VALUED FUNCTIONS
      page: 359
      pdf_page: 365
    - "no": 2
      title: SEMI-CONTINUOUS FUNCTIONS
      page: 360
      pdf_page: 366
statements: 15
exercises: 15
content_sha256: 0d6d141948776b1a291d462628bde3942045e93557e66f550ce887f528af49e5
---

## 6. CONTINUOUS AND SEMI-CONTINUOUS REAL-VALUED FUNCTIONS

### 1. CONTINUOUS REAL-VALUED FUNCTIONS

Besides the general properties of continuous functions with values in an arbitrary topological space (Chapter I, § 2), continuous real-valued functions have the following two fundamental properties:

#### Theorem 1 (Weierstrass) {#top-iv-s6-thm-1 .statement}

Let $f$ be a continuous real-valued function defined on a non-empty quasi-compact space $X$. Then there is at least one point $a \in X$ such that $f(a) = \sup_{x \in X} (f(x))$, and at least one point $b \in X$ such that $f(b) = \inf_{x \in X} f(x)$. For $f(X)$ is compact (Chapter I, § 9, no. 4, Theorem 2) and therefore closed in $\overline{\mathbf{R}}$; hence $f(X)$ contains its bounds.

This theorem is often stated in the form that a continuous real-valued function on a non-empty quasi-compact space attains its bounds.

#### Corollary {#top-iv-s6-n1-cor-1 .statement}

If a real-valued function defined on a non-empty quasi-compact space $X$ is continuous and finite on $X$, then it is bounded in $X$.

#### Theorem 2 (Bolzano) {#top-iv-s6-thm-2 .statement}

Let $f$ be a continuous real-valued function defined on a connected space $X$. If $a$ and $b$ are any two points of $X$, and if $\alpha$ is a real number belonging to the closed interval whose end-points are $f(a)$ and $f(b)$, then there is at least one point $x \in X$ such that $f(x) = \alpha$.

For $f(X)$ is connected (Chapter I, § 11, no. 2, Proposition 4) and is therefore an interval of $\overline{\mathbf{R}}$ (§ 4, no. 2, Proposition 5); hence it contains the closed interval with end-points $f(a)$ and $f(b)$.

This theorem is often expressed in the form that *a continuous real-valued function on a connected space cannot pass from one value to another without passing through all intermediate values*.

This property is by no means characteristic of continuous functions; there are examples of functions defined on a connected space and *discontinuous at every point* which have this property (Exercise 2).

### 2. SEMI-CONTINUOUS FUNCTIONS

Let $f$ be a real-valued function defined on a topological space $X$. For $f$ to be continuous at a point $a \in X$ it is necessary and sufficient that:
(i) given any real number $h < f(a)$, there exists a neighbourhood $V$ of $a$ such that at each point $x \in V$ we have $h < f(x)$;
(ii) given any real number $k > f(a)$, there exists a neighbourhood $W$ of $a$ such that at each point $x \in W$ we have $k > f(x)$.

Functions which satisfy *only one* of these conditions play an important part in analysis. To be precise, we make the following definition:

#### Definition 1 {#top-iv-s6-def-1 .statement}

*A real-valued function $f$, defined on a topological space $X$, is said to be lower semi-continuous* (resp. *upper semi-continuous*) *at a point $a \in X$, if for each $h < f(a)$ [resp. each $k > f(a)$] there is a neighbourhood $V$ of $a$ such that $h < f(x)$ [resp. $k > f(x)$] *for each* $x \in V$.

*A real-valued function is said to be lower semi-continuous* (resp. *upper semi-continuous*) *on $X$ if it is lower semi-continuous* (resp. *upper semi-continuous*) *at every point of $X$*.

A real-valued function $f$ is therefore *continuous* at a point $a$ if and only if it is *both upper and lower semi-continuous* at $a$.

If $f$ is lower semi-continuous at a point, then $-f$ is upper semi-continuous at this point, and conversely; hence we may restrict ourselves in what follows, to considering properties of *lower semi-continuous* functions.

It is clear that a function which is lower semi-continuous on $X$ is also lower semi-continuous on every *subspace* of $X$.

#### Example 1 {#top-iv-s6-n2-exa-1 .statement}

If $f$ has a *relative minimum* at a point $a$, that is to say if there is a neighbourhood $V$ of $a$ such that, for each $x \in V$, we have $f(a) \leq f(x)$, then $f$ is lower semi-continuous at $a$. In particular, if $f(a) = -\infty$, $f$ is lower semi-continuous at $a$.

#### Example 2 {#top-iv-s6-n2-exa-2 .statement}

Define a real-valued function $f$ on $\mathbf{R}$ by putting $f(x) = 0$ if $x$ is irrational, and $f(x) = 1/q$ if $x$ is rational and equal to the irreducible fraction $p/q$ ($q > 0$). For each integer $n > 0$, the set of rational numbers $p/q$ such that $q < n$ is closed, and its points are isolated; hence for every irrational $x$ there is a neighbourhood $V$ of $x$ such that $f(y) \leq 1/n$ for all $y \in V$, which shows that $f$ is continuous at $x$; and on the other hand, $f$ has a *relative maximum* at every rational point $x$. Hence $f$ is upper semi-continuous on $\mathbf{R}$.

The condition for $f$ to be lower semi-continuous at $a$ may be expressed by saying that, for each $h < f(a)$, the set $\overline{f}([h, +\infty])$ must be a neighbourhood of $a$.

It is enough that this condition should be satisfied for an increasing sequence $(h_n)$ of real numbers $< f(a)$ which tend to $f(a)$.

Endow $\overline{\mathbf{R}}$ with the topology in which the open sets are $\varnothing$ and all open intervals of $\overline{\mathbf{R}}$ unbounded on the right (that is, all intervals $]a, +\infty[$ for finite $a$, and the interval $[--\infty, +\infty] = ]\leftarrow, \rightarrow[]$). Then the real-valued function $f$ is lower semi-continuous at $a$ if and only if it is continuous at $a$ when considered as a mapping into $\overline{\mathbf{R}}$ endowed with this topology.

#### Proposition 1 {#top-iv-s6-prop-1 .statement}

*A real-valued function $f$ on a topological space $X$ is lower semi-continuous if and only if, for each finite real number $k$, $\overline{f}([k, +\infty])$ [the set of all $x \in X$ such that $f(x) > k$] is an open set in $X$ [or, equivalently, $\overline{f}([-\infty, k])$ is a closed set in $X$].*

For this condition shows that $\overline{f}([k, +\infty])$ is a neighbourhood of each of its points.

For $f$ to be lower semi-continuous on $X$ it is sufficient that $f^{-1}([k, +\infty])$ is open in $X$ for all real numbers $k$ belonging to a dense subset of $\mathbf{R}$.

#### Corollary {#top-iv-s6-n2-cor-1 .statement}

*A subset $A$ of a topological space $X$ is open (resp. closed) in $X$ if and only if its characteristic function (*) $\varphi_A$ is lower (resp. upper) semi-continuous on $X$.*

For $\overline{f}_A([k, +\infty])$ is empty for $k \geq 1$, is equal to $A$ for $0 \leq k < 1$ and is equal to $X$ for $k < 0$.

#### Theorem 3 {#top-iv-s6-thm-3 .statement}

*Let $f$ be a lower semi-continuous function on a non-empty quasi-compact space $X$. Then there is at least one point $a \in E$ such that $f(a) = \inf_{x \in X} f(x)$ (in other words, $f$ attains its greatest lower bound in $X$).*

For each $k \in f(X)$, consider the set $A_k = \overline{f}([-\infty, k])$. These sets are non-empty and form a filter base on $X$; since they are closed by Proposition 1, they have at least one common point $a$ [axiom (C'') for quasi-compact spaces]. For each $x \in X$ we have therefore $f(a) \leq f(x)$, and the theorem follows.

(*) We recall (Set Theory, Chapter III, § 5, no. 5) that the characteristic function $\varphi_A$ of a subset $A$ of a set $X$ is the function defined on $X$ such that $\varphi_A(x) = 1$ for all $x \in A$, and $\varphi_A(x) = 0$ for all $x \in \complement_A$.

#### Corollary {#top-iv-s6-n2-cor-2 .statement}

Let $f$ be a lower semi-continuous function on a non-empty quasi-compact space $X$. If $f(x) > -\infty$ for all $x \in X$, then $f$ is bounded below in $X$.

Note that this theorem and the corresponding theorem for upper semi-continuous functions include Weierstrass's theorem as a particular case (no. 1, Theorem 1).

#### Proposition 2 {#top-iv-s6-prop-2 .statement}

Let $f$ and $g$ be two real-valued functions, lower semi-continuous at a point $a \in X$. Then the functions $\inf(f, g)$ and $\sup(f, g)$ are lower semi-continuous at $a$; so is $f + g$ whenever it is defined, and so is $fg$ if $f$ and $g$ are $\geq 0$ and the product $fg$ is defined.

We give the proof for $f + g$; the argument is analogous in the other cases. The result is clear if either $f(a)$ or $g(a)$ is equal to $-\infty$; if not, then $f(a) + g(a) > -\infty$. Every finite number $h < f(a) + g(a)$ can be written as $h = r + s$, where $r < f(a)$ and $s < g(a)$ are finite [it is enough to take $s$ so that $h - f(a) < s < g(a)$]; by hypothesis, there is a neighbourhood $V$ of $a$ such that, for each $x \in V$, we have $r < f(x)$, and a neighbourhood $W$ such that for each $x \in W$ we have $s < g(x)$; therefore $h = r + s < f(x) + g(x)$ for all points $x$ of the neighbourhood $V \cap W$.

In the same way we see that, if $f$ is lower semi-continuous at a point $a$, and if $f \geq 0$, then $1/f$ is upper semi-continuous at $a$.

#### Theorem 4 {#top-iv-s6-thm-4 .statement}

The upper envelope of a family $(f_i)$ of functions which are lower semi-continuous at a point $a \in X$ is lower semi-continuous at $a$.

Let $g$ be the upper envelope. For each $h < g(a)$ there is an index $i$ such that $h < f_i(a) \leq g(a)$, and a neighbourhood $V$ of $a$ such that $h < f_i(x)$ for all $x \in V$; hence $a$ fortiori $h < g(x)$ for all $x \in V$.

It follows from Proposition 2 that the lower envelope of a finite number of lower semi-continuous functions is again lower semi-continuous; but this is not in general true for the lower envelope of an infinite family of lower semi-continuous functions. For example, if $r$ is any rational number, let $f_r$ denote the function which is equal to 0 at $r$ and equal to 1 for all real numbers $x \neq r$; the lower envelope of the $f_r$ is the function $g$ which is equal to 0 for every rational number and 1 for every irrational number ("Dirichlet's function"), and this function is not lower semi-continuous at irrational points.

#### Corollary {#top-iv-s6-n2-cor-3 .statement}

The upper envelope of a family of continuous real-valued functions on a space $X$ is lower semi-continuous on $X$.

In Chapter IX, § 1, no. 6, Proposition 5, we shall show that the converse of this proposition is true if $X$ is uniformizable (and only in this case): every lower semi-continuous function on a uniformizable space is the upper envelope of a family of continuous functions.

#### Proposition 3 {#top-iv-s6-prop-3 .statement}

*A real-valued function f, defined on a topological space X, is lower semi-continuous at a point $a \in X$ if and only if* $\liminf_{x \to a} f(x) = f(a)$ [or, equivalently, if and only if $\liminf_{x \to a} f(x) \geq f(a)$].

The condition is *necessary*. For, given any $h < f(a)$, there is a neighbourhood V of $a$ such that $h < f(x)$ for all $x \in V$; therefore
$$
h \leq \inf_{x \in V} f(x) \leq \liminf_{x \to a} f(x)
$$
(§ 5, no. 6, formulae (12)), and so $f(a) \leq \liminf_{x \to a} f(x)$. The condition is *sufficient*; for if it is satisfied, then for each $h < f(a)$ there is a neighbourhood V of $a$ such that $h \leq \inf_{x \in V} f(x)$, and therefore $f$ is lower semi-continuous at $a$.

#### Proposition 4 {#top-iv-s6-prop-4 .statement}

*Let f be any real-valued function defined on a dense subset A of a topological space X. If, for each $x \in X$, we put* $g(x) = \liminf_{y \to x, y \in A} f(y)$, *then g is lower semi-continuous on X*.

For, given any $h < g(x)$, there is an *open* neighbourhood V of $x$ such that, for all $z \in V \cap A$, we have $h < f(z)$; now V is a neighbourhood of each of its points $y$; thus we have $\liminf_{z \to y, z \in A} f(z) = g(y) \geq h$ for all $y \in V$, and the result follows.

The function $g$ is called the *lower semi-continuous regularization* of $f$. We define the *upper semi-continuous regularization* of $f$ similarly.

We may also define $g$ as the *greatest* of the lower semi-continuous functions $\varphi$ on X which are such that $\varphi(x) \leq f(x)$ for all $x \in A$. If $f$ is *lower semi-continuous* on A, then $g$ is an *extension* of $f$ to X, by Proposition 3.

### Exercises {#top-iv-s6-exercises}

See the [exercises for § 6](exercises/s6/).
