---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 1
section_title: PRIMITIVES AND INTEGRALS
lang: en
source: fvr-i-vii
pdf_pages: 0066-0077, 0094-0099
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF PRIMITIVES
      page: 0
      pdf_page: 66
    - "no": 2
      title: EXISTENCE OF PRIMITIVES
      page: 0
      pdf_page: 67
    - "no": 3
      title: REGULATED FUNCTIONS
      page: 0
      pdf_page: 68
    - "no": 4
      title: INTEGRALS
      page: 0
      pdf_page: 71
    - "no": 5
      title: PROPERTIES OF INTEGRALS
      page: 0
      pdf_page: 74
    - "no": 6
      title: INTEGRAL FORMULA FOR THE REMAINDER IN TAYLOR'S FORMULA; PRIMITIVES OF HIGHER ORDER
      page: 0
      pdf_page: 77
statements: 28
exercises: 10
content_sha256: ff30f9508044e05296fa35eac9891d983060ac6f9e5e128e409343cc51396165
---

## § 1. PRIMITIVES AND INTEGRALS

Unless expressly mentioned to the contrary, in this chapter we shall only consider vector functions of a real variable which take their values in a complete normed space over $\mathbf{R}$. When we deal in particular with real-valued functions it will always be understood that these functions are finite unless stated to the contrary.

### 1. DEFINITION OF PRIMITIVES

A vector function $f$ defined on an interval $I \subset \mathbf{R}$ cannot be the derivative at every point of this interval of a vector function $g$ (defined and continuous on $I$) unless it satisfies quite stringent conditions: for example, if $f$ admits a right limit and a left limit at a point $x_0$ interior to $I$ then $f$ must be continuous at the point $x_0$, as follows from prop. 6 of I, p. 18; it follows, that if one takes the interval $[ -1 , 1 ]$ for $I$, and for $f$ the real function equal to $-1$ on $[ -1 , 0[$, and to $+1$ on $[0 , 1]$, then $f$ is not the derivative of any continuous function on $I$; all the same, the function $|x|$ has $f(x)$ as its derivative at every point $\neq 0$; one is thus led to make the following definition:

#### Definition 1 {#fvr-ii-s1-def-1 .statement}

*Given a vector function $f$ defined on an interval $I \subset \mathbf{R}$ we say that a function $g$ defined on $I$ is a primitive of $f$ if $g$ is continuous on $I$ and has a derivative equal to $f(x)$ at every point $x$ of the complement (with respect to $I$) of a countable subset of $I$.*

If also $g$ admits a derivative equal to $f(x)$ at every point $x$ of $I$, one says that $g$ is a strict primitive of $f$.

With this definition, one sees that the real function $f$ considered above admits a primitive equal to $|x|$.

It is clear that if $f$ admits a primitive on $I$ then every primitive of $f$ is also a primitive of every function which is equal to $f$ except at the points of a countable subset of $I$. By an abuse of language one speaks of a primitive on $I$ of a function $f_0$ defined only on the complement (with respect to $I$) of a countable subset of $I$: this will be the primitive of every function $f$ defined on $I$ and equal to $f_0$ at the points where $f_0$ is defined.

#### Proposition 1 {#fvr-ii-s1-prop-1 .statement}

*Let $f$ be a vector function defined on $I$ with values in $E$; if $f$ admits a primitive $g$ on $I$ then the set of primitives of $f$ on $I$ is identical to the set of functions $g + a$, where $a$ is a constant function with its values in $E$.*

Indeed, it is clear that $g + a$ is a primitive of $f$ for any $a \in E$; on the other hand, if $g_1$ is a primitive of $f$ then $g_1 - g$ admits a derivative equal to 0 except at the points of a countable subset of $I$, and thus is constant (I, p. 17, corollary).

One says that the primitives of a function $f$ (when they exist) are defined “up to an additive constant”. To define a primitive of $f$ unambiguously it is enough to assign it (arbitrarily) a value at a point $x_0 \in I$; in particular, there exists one and only one primitive $g$ of $f$ such that $g(x_0) = 0$; for every primitive $h$ of $f$ one has $g(x) = h(x) - h(x_0)$.

### 2. EXISTENCE OF PRIMITIVES

Let $f$ be a function defined on an arbitrary interval $I \subset \mathbf{R}$; for a function $g$ defined on $I$ to be a primitive of $f$, it is necessary and sufficient that the restriction of $g$ to every compact interval $J \subset I$ be a primitive of the restriction of $f$ to $J$.

#### Theorem 1 {#fvr-ii-s1-thm-1 .statement}

*Let $A$ be a set filtered by a filter $\mathfrak{F}$, and $(f_\alpha)_{\alpha \in A}$ a family of vector functions with values in a complete normed space $E$ over $\mathbf{R}$, defined on an interval $I \subset \mathbf{R}$: for each $\alpha \in A$ let $g_\alpha$ be a primitive of $f_\alpha$. We suppose that:
1. with respect to the filter $\mathfrak{F}$ the functions $f_\alpha$ converge uniformly on every compact subset of $I$ to a function $f$;
2. there is a point $a \in I$ such that, with respect to the filter $\mathfrak{F}$, the family $(g_\alpha(a))$ has a limit in $E$.
Under these hypotheses the functions $g_\alpha$ converge uniformly (with respect to $\mathfrak{F}$) on every compact subset of $I$ to a primitive $g$ of $f$.*

By the remark at the beginning of this subsection we can restrict ourselves to the case where $I$ is a *compact* interval.

First let us show that the $g_\alpha$ converge uniformly on $I$ to a continuous function $g$. By hypothesis, for every $\varepsilon > 0$ there is a set $M \in \mathfrak{F}$ such that, for any two indices $\alpha, \beta$ belonging to $M$, one has $\|f_\alpha(x) - f_\beta(x)\| \leq \varepsilon$ for each $x \in I$; in consequence one has (I, p. 15, th. 2)

$$
\|g_\alpha(x) - g_\beta(x) - (g_\alpha(a) - g_\beta(a))\| \leq \varepsilon |x - a| \leq \varepsilon l
$$

where $l$ denotes the length of $I$; since by hypothesis $g_\alpha(a)$ approaches a limit with respect to $\mathfrak{F}$, it follows from the Cauchy criterion that the $g_\alpha$ converge uniformly on $I$. It remains to show that the limit $g$ of the $g_\alpha$ is a primitive of $f$.

For each integer $n > 0$ let $\alpha_n$ be an index such that $\|f(x) - f_{\alpha_n}(x)\| \leq 1/n$ on $I$; it is clear that the sequence $(f_{\alpha_n})$ converges uniformly to $f$ and that the sequence $(g_{\alpha_n})$ converges uniformly to $g$ on $I$. Let $H_n$ be the countable subset of $I$ where $f_{\alpha_n}$ is not the derivative of $g_{\alpha_n}$, and let $H$ be the union of the $H_n$, which is thus a countable subset of I; we shall see that at every point $x \in I$ not belonging to H the function g has a derivative equal to $f(x)$. Indeed, one sees as above that for every $m \geq n$ and every $y \in I$ one has

$$
\| g_{\alpha_m}(y) - g_{\alpha_m}(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|.
$$

Letting $m$ increase indefinitely one also has

$$
\| g(y) - g(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|
$$

for every $y \in I$; now, there exists an $h > 0$ such that, for $|y - x| \leq h$ and $y \in I$, one has $\| g_\alpha(y) - g_{\alpha_n}(x) - f_{\alpha_n}(x)(y - x) \| \leq |y - x| / n$; since, on the other hand, we have $\| f(x) - f_{\alpha_n}(x) \| \leq 1 / n$, we finally obtain

$$
\| g(y) - g(x) - f(x)(y - x) \| \leq \frac{4}{n} |y - x|
$$

for $y \in I$ and $|y - x| \leq h$, which completes the proof.

#### Corollary 1 {#fvr-ii-s1-thm-1-cor-1 .statement}

*The set $\mathcal{H}$ of maps from I into E which admit a primitive on an interval I is a closed (and so complete) vector subspace of the complete vector space $\mathcal{F}_c(I; E)$ of maps from I into E, endowed with the topology of uniform convergence on every compact subset of I* (*Gen. Top.*, X, p. 277).

#### Corollary 2 {#fvr-ii-s1-thm-1-cor-2 .statement}

*Let $x_0$ be a point of I, and for each function $f \in \mathcal{H}$ let $P(f)$ be the primitive of $f$ which vanishes at the point $x_0$; the map $f \mapsto P(f)$ of $\mathcal{H}$ into $\mathcal{F}_c(I; E)$ is a continuous linear mapping.*

Cor. 1 to th. 1 allows us to establish the existence of primitives for certain categories of functions by the following procedure: if one knows that the functions belonging to a subset $\mathcal{A}$ of $\mathcal{F}_c(I; E)$ admit a primitive, so will the functions belonging to the *closure* in $\mathcal{F}_c(I; E)$ of the vector subspace generated by $\mathcal{A}$. We shall apply this method in the next subsection.

### 3. REGULATED FUNCTIONS

#### Definition 2 {#fvr-ii-s1-def-2 .statement}

*One says that a map $f$ of an interval $I \subset \mathbf{R}$ into a set E is a step function if there is a partition of I into a finite number of intervals $J_k$ such that $f$ is constant on each of the $J_k$.*

Let $(a_i)_{0 \leq i \leq n}$ be the strictly increasing sequence formed by the distinct endpoints of the $J_k$; since the $J_k$ are pairwise disjoint each of them either reduces to a singleton $a_i$ or is an interval with two consecutive points $a_i, a_{i+1}$ as endpoints; moreover, since I is the union of the $J_k$, the point $a_0$ is the left-hand endpoint, and $a_n$ is the right-hand endpoint of I. Every step function on I can thus be characterised as a function which is constant on each of the open intervals ]$a_i,\ a_{i+1}[\ (0 \leq i \leq n - 1)$, where $(a_i)_{0 \leq i \leq n}$ is a strictly increasing sequence of points of $I$ with $a_0$ being the left-hand endpoint and $a_n$ the right-hand endpoint of $I$.

#### Proposition 2 {#fvr-ii-s1-prop-2 .statement}

*The set of step functions defined on $I$, with values in a vector space $E$ over $\mathbf{R}$, is a vector subspace $\mathcal{E}$ of the vector space $\mathcal{F}(I; E)$ of all maps of $I$ into $E$.*

Indeed, let $f$ and $g$ be two step functions, and $(A_i)$ and $(B_j)$ two partitions of $I$ into a finite number of intervals such that $f$ (resp. $g$) is constant on each of the $A_i$ (resp. $B_j$); whatever the real numbers $\lambda, \mu$, it is clear that $\lambda f + \mu g$ is constant on each of the nonempty intervals $A_i \cap B_j$, and that these intervals form a partition of $I$.

#### Corollary {#fvr-ii-s1-n3-cor-1 .statement}

*The vector subspace $\mathcal{E}$ is generated by the characteristic functions of intervals.*

Now let us consider the case where $E$ is a normed space over $\mathbf{R}$; it is then immediate that the characteristic function of an interval $J$ with endpoints $a, b$ ($a < b$) admits a primitive, namely the function equal to $a$ for $x \leq a$, to $x$ for $a \leq x \leq b$, and to $b$ for $x \geq b$. The cor. to prop. 2 thus shows that *every step function with values in $E$ admits a primitive*.

We can now apply the method set out in n' 2.

#### Definition 3 {#fvr-ii-s1-def-3 .statement}

*One says that a vector function, defined on an interval $I$, with values in a complete normed space $E$ over $\mathbf{R}$, is a regulated function, if it is the uniform limit of step functions on every compact subset of $I$.*

In other words, the regulated functions are the elements of the closure in $\mathcal{F}_c(I; E)$ of the subspace $\mathcal{E}$ of step functions; $\overline{\mathcal{E}}$ is a vector subspace of $\mathcal{F}_c(I; E)$ and since $\mathcal{F}_c(I; E)$ is complete, so is $\overline{\mathcal{E}}$; in other words, if a function is the uniform limit of regulated functions on every compact subset of $I$, then it is regulated on $I$. For $f$ to be regulated on an interval $I$ it is necessary and sufficient that its restriction to every compact interval contained in $I$ be regulated.

Cor. I to II, p. 53 shows:

#### Theorem 2 {#fvr-ii-s1-thm-2 .statement}

*Every regulated function on an interval $I$ admits a primitive on $I$.*

We shall transform def. 3 of II, p. 4 to another equivalent one:

#### Theorem 3 {#fvr-ii-s1-thm-3 .statement}

*For a vector function $f$ defined on an interval $I$, with values in a complete normed space $E$ over $\mathbf{R}$, to be regulated, it is necessary and sufficient that it have a right limit and a left limit at every interior point of $I$, and a right limit at the left-hand endpoint of $I$ and a left limit at the right-hand endpoint of $I$, when these points belong to $I$. The set of points of discontinuity of $f$ in $I$ is thus countable.*

Since every interval is a countable union of compact intervals, one can restrict oneself to proving th. 3 when I is compact, say I = [a, b].

1 The condition is necessary. Suppose that f is regulated and let x be a point of I different from b. By hypothesis, for every ε > 0 there is a step function g such that \|f(z) - g(z)\| \leq \varepsilon for every z \in I; since g has a right limit at the point x there exists a y such that x < y \leq b and such that, for every pair of points z, z' in the interval ]x, y] one has \|g(z) - g(z')\| \leq \varepsilon, and in consequence \|f(z) - f(z')\| \leq 3\varepsilon; this proves (by Cauchy’s criterion) that f has a right limit at the point x. In the same way one proves that f has a left limit at every point of I different from a.

2° The condition is sufficient. Suppose it is satisfied; for each x \in I there is an open interval V_x = ]c_x, d_x[ containing x and such that on the intersection of I with each of the open intervals ]c_x, x[, ]x, d_x[ (when the intersection is not empty) the oscillation of f is \leq \varepsilon. Since I is compact there is a finite number of points x_i in I such that the V_{x_i} form a cover of I; let (a_k)_{0 \leq k \leq n} be the sequence obtained by arranging in increasing order the points of the finite set formed by the points a, b and those points x_i, c_{x_i} and d_{x_i} which belong to I; each of the intervals ]a_k, a_{k+1}[ (0 \leq k \leq n - 1) being contained in an interval ]c_{x_i}, x_i[ or ]x_i, d_{x_i}[, the oscillation of f there is \leq \varepsilon; let c_k be one of the values of f on ]a_k, a_{k+1}[; on putting g(a_k) = f(a_k) for 0 \leq k \leq n, and g(x) = c_k for all x \in ]a_k, a_{k+1}[ (0 \leq k \leq n - 1), one defines a step function g such that \|f(z) - g(z)\| \leq \varepsilon on I; so f is regulated on I.

Finally, let us show that if f is regulated on I then its set of points of discontinuity is countable. For every n > 0 there exists a step function g_n such that \|f(x) - g_n(x)\| \leq 1/n on I; since the sequence (g_n) converges uniformly to f on I, we see that f is continuous at every point where the g_n are all continuous (Gen. Top., X, p. 281, cor. 1); but since g_n is continuous except at the points of a finite set H_n it follows that f is continuous at the points of the complement of the set H = \bigcup_{n} H_n, which is countable.

#### Corollary 1 {#fvr-ii-s1-thm-3-cor-1 .statement}

Let f be a regulated function on I; at every point of I, apart from the right-hand endpoint (resp. the left-hand endpoint) of I, every primitive of f has a right derivative equal to f(x+) (resp. a left derivative equal to f(x-)); in particular, at every point x where f is continuous, f(x) is the derivative of one of its primitives.

This is an immediate consequence of th. 3 of II, p. 54 and of prop. 6 of I, p. 18.

#### Corollary 2 {#fvr-ii-s1-thm-3-cor-2 .statement}

Let f_i (1 \leq i \leq n) be n regulated functions on an interval I, each f_i having its values in a complete normed space E_i over \mathbf{R} (1 \leq i \leq n). If g is a continuous map of the subspace \prod_{i=1}^{n} \overline{f_i(I)} of \prod_{i=1}^{n} E_i into a complete normed space F over \mathbf{R}, then the composite function x \mapsto g(f_1(x), f_2(x), \ldots, f_n(x)) is regulated on I.

Indeed, it clearly satisfies the conditions of th. 3 of II, p. 54.

Thus one sees that if f is a regulated vector function on I, then the real function x \mapsto \|f(x)\| is also regulated. Further, the real regulated functions on I form a ring;

moreover, if $f$ and $g$ are two real regulated functions, then $\sup(f, g)$ and $\inf(f, g)$ are regulated.

#### Remark 1 {#fvr-ii-s1-n3-rem-1 .statement}

If $f$ is a real regulated function on $I$, and $g$ is a regulated vector function on an interval containing $f(I)$, then the composite function $g \circ f$ is not necessarily regulated ($cf.$ II, p. 79, exerc. 4).

Two particular cases of th. 3 of II, p. 54 are especially important:

#### Proposition 3 {#fvr-ii-s1-prop-3 .statement}

*Every continuous vector function on an interval $I \subset \mathbf{R}$ taking its values in a complete normed space $E$ over $\mathbf{R}$ is regulated, and admits a primitive on $I$, of which it is the derivative at every point.*

#### Remark 2 {#fvr-ii-s1-n3-rem-2 .statement}

To show that a continuous function admits a primitive, one can use the fact that every *polynomial function* of a real variable (with coefficients in $E$) admits a primitive; since from the theorem of Weierstrass (*Gen. Top.*, X, p. 313, prop. 3) every continuous function is the uniform limit of polynomials on every compact interval, th. 1 of II, p. 52 shows that every continuous function admits a primitive.

#### Remark 3 {#fvr-ii-s1-n3-rem-3 .statement}

The principle of the preceding remark extends without significant modification to vector functions of a *complex* variable taking values in a complete normed space over $\mathbf{C}$. If $U$ is an open set in $\mathbf{C}$, homeomorphic to $\mathbf{C}$, a *primitive* of such a vector function $f$ defined on $U$ is by definition a continuous function on $U$, having derivative equal to $f$ at every point of $U$. With this definition, th. 1 of II, p. 52 extends without modification (one proves, using the connectedness of $U$, that $(g_\alpha)$ is uniformly convergent with respect to $\mathcal{F}$ on a neighbourhood of each point of $U$, from which it follows that $(g_\alpha)$ is uniformly convergent with respect to $\mathcal{F}$ on every compact subset of $U$; the proof is completed using prop. 4 of I, p. 18). Consequently, every function which is a *uniform limit of polynomials* on every compact subset of $U$, admits a primitive on $U$; these functions are no other than the functions called *holomorphic* on $U$, which we shall study further in detail in a later Book.

#### Proposition 4 {#fvr-ii-s1-prop-4 .statement}

*Every monotone real function $f$ on an interval $I \subset \mathbf{R}$ is regulated, and every primitive of $f$ is convex on $I$.*

Indeed, $f$ satisfies the criterion of th. 3 of *Gen. Top.*, IV, p. 350, prop. 4; the second part of the proposition follows from cor. 1, from II, p. 55, and from prop. 5 of I, p. 27.

#### Remark 4 {#fvr-ii-s1-n3-rem-4 .statement}

One must not think that the regulated functions on an interval $I$ are the only functions having a primitive on $I$ ($cf.$ II, p. 80, exercises 7 and 8).

### 4. INTEGRALS

We have obtained (II, p. 54, th. 2) a primitive of a regulated function on an interval $I$ as the uniform limit of primitives of step functions. This procedure can be expressed in a slightly different way: let $x_0, x$ be two arbitrary points of $I$ such that $x_0 < x$; we call a *subdivision* of the interval $[x_0, x]$ any sequence of intervals $[x_i, x_{i+1}]$ with union $[x_0, x]$, where $(x_i)_{0 \leq i \leq n}$ is a strictly increasing sequence of points of $[x_0, x]$ such that $x_n = x$. We shall call a *Riemann sum*, relative to a vector function $f$ defined on I and to the subdivision formed by the $[x_i,\ x_{i+1}]$, any expression of the form
$$
\sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i)
$$
where the $t_i$ belong to $[x_i,\ x_{i+1}]$ for $0 \leq i \leq n-1$. One then has the following proposition:

#### Proposition 5 {#fvr-ii-s1-prop-5 .statement}

*Let $f$ be a regulated function on an interval I, let $g$ be a primitive of $f$ on I, and $[x_0,\ x]$ a compact interval contained in I. For every $\varepsilon > 0$ there exists a number $\rho > 0$ such that for every subdivision of $[x_0,\ x]$ into intervals of length $\leq \rho$ one has*
$$
\left| g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) \right| \leq \varepsilon
$$
*(1)*
*for every Riemann sum relative to this subdivision.*

Indeed, let $f_1$ be a step function such that $\|f(y) - f_1(y)\| \leq \varepsilon$ for every $y \in [x_0,\ x]$; one has, denoting a primitive of $f_1$ on I by $g_1$,
$$
\|g(x) - g(x_0) - (g_1(x) - g_1(x_0))\| \leq \varepsilon(x - x_0)
$$
by the mean value theorem, and on the other hand
$$
\left| \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) - \sum_{i=0}^{n-1} f_1(t_i)(x_{i+1} - x_i) \right| \leq \varepsilon(x - x_0).
$$

It thus suffices to prove the proposition when $f$ is a *step function*. Let $(y_k)_{1 \leq k \leq m}$ be the strictly increasing finite sequence of points of discontinuity of $f$ in $[x_0,\ x]$. For every subdivision of $[x_0,\ x]$ into intervals of length $\leq \rho$ each of the points $y_k$ belongs to at most two of these intervals; there can therefore be no more than $2m$ intervals on which $f$ is not constant; but, on such an interval $[x_i,\ x_{i+1}]$ one has
$$
\|g(x_{i+1}) - g(x_i) - f(t_i)(x_{i+1} - x_i)\| \leq 2M (x_{i+1} - x_i)
$$
on denoting by $M$ the least upper bound of $\|f\|$ on $[x_0,\ x]$; on the other hand, when $f$ is constant on $[x_i,\ x_{i+1}]$ one has
$$
g(x_{i+1}) - g(x_i) - f(t_i)(x_{i+1} - x_i) = 0.
$$
One thus sees that the difference
$$
\left| g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) \right|
$$
cannot exceed $4Mm\rho$; it therefore suffices to take $\rho \leq \varepsilon / 4Mm$ to obtain (1).

#### Remark 1 {#fvr-ii-s1-n4-rem-1 .statement}

When $f$ is *continuous* prop. 5 can be proved more simply: since $f$ is uniformly continuous on $[x_0,\ x]$ there exists a $\rho > 0$ such that on every interval of length $\leq \rho$ contained in $[x_0,\ x]$ the oscillation of $f$ is $\leq \frac{\varepsilon}{x - x_0}$; for every subdivision of $[x_0,\ x]$ into intervals $[x_i,\ x_{i+1}]$ of length $\leq \rho$ and every choice of $t_i$ in $[x_i,\ x_{i+1}]$ for $0 \leq i \leq n-1$ the step function $f_1$ equal to $f(t_i)$ on $[x_i,\ x_{i+1}]$ ($0 \leq i \leq n-1$), and to $f(x)$ at the point x, is such that $\| f(y) - f_1(y) \| \leq \frac{\varepsilon}{x - x_0}$ on $[x_0, x]$; if $g_1$ is a primitive of $f_1$ one has
$$
g_1(x) - g_1(x_0) = \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i),
$$
so the relation (1) follows immediately from the mean value theorem.

In the rest of this chapter we shall confine ourselves to the study of primitives of *regulated* functions on an interval I. For such a function $f$, with values in E, a primitive $g$ of $f$, and for two arbitrary points $x_0, x$ of I, the element $g(x) - g(x_0)$ of E (which is clearly the same, no matter which primitive $g$ of $f$ one considers) is called the *integral of the function* $f$ *from* $x_0$ *to* $x$ (or *over the compact interval* $[x_0, x]$) and is denoted by $\int_{x_0}^x f(t) dt$ or $\int_{x_0}^x f$. This name and notation have their origin in prop. 5 of II, p. 57, which shows that an integral can be approximated arbitrarily closely by a Riemann sum; more particularly, one can write, taking subdivisions of $[x_0, x]$ into equal intervals,

$$
\frac{1}{x - x_0} \int_{x_0}^x f(t) dt = \lim_{n \to \infty} \frac{1}{n} \sum_{k=0}^{n-1} f \left( x_0 + k \frac{x - x_0}{n} \right).
$$

In other words, the element $\frac{1}{x - x_0} \int_{x_0}^x f(t) dt$ is the limit of the *arithmetic means* of the values of $f$ at the left-hand endpoints of the intervals of a subdivision of $[x_0, x]$ into equal intervals; one also calls it the *mean* (or *mean value*) of the function $f$ on the interval $[x_0, x]$.

By definition, the function $x \mapsto \int_{x_0}^x f(t) dt$ is none other than the primitive of $f$ which vanishes at the point $x_0 \in I$; one also denotes it by $\int_{x_0}^x f(t) dt$ or $\int_{x_0}^x f$.

#### Remark 2 {#fvr-ii-s1-n4-rem-2 .statement}

For an arbitrary function $h$ defined on I, with values in E, the element $h(x) - h(x_0)$ is also written as $h(t)\Big|_{x_0}^x$; with this notation one sees that if $g$ is any primitive of a regulated function $f$ on I, one has

$$
\int_{x_0}^x f(t) dt = g(t)\Big|_{x_0}^x.
$$

#### Remark 3 {#fvr-ii-s1-n4-rem-3 .statement}

The expressions $\int_{x_0}^x f(t) dt$ and $g(t)\Big|_{x_0}^x$ are abbreviating symbols representing assemblies in which the letters $x, x_0, f, g$, but *not* the letter $t$, appear (*cf. Set Theory*, I, p. 15); one says that among these symbols $t$ is a "*dummy variable*": one can thus replace $t$ by any other variable distinct from $x, x_0, f$ and $g$ (and from variables which may possibly enter into the proof where these symbols appear) without changing the sense of the symbol so obtained (the reader may compare these symbols with symbols such as $\sum_{i=1}^n x_i$, or $\bigcup X_i$, where $i$ is likewise a dummy variable).

#### Remark 4 {#fvr-ii-s1-n4-rem-4 .statement}

The approximation of an integral by Riemann sums is closely connected to one of the historical origins of the concept of an integral, the problem of the *measure* of areas. We shall come back to this point in the Book on Integration which is devoted to generalizations of the concept of integral to which this problem leads; in these generalizations the functions to be "*integrated*" are not necessarily defined on a subset of $\mathbf{R}$; moreover, even when one deals with (not necessarily regulated) real functions $f$ of a real variable for which one can define an integral $\int_{x_0}^x f(t)\,dt$, the function $x \mapsto \int_{x_0}^x f(t)\,dt$ is not always a primitive of $f$, and there exist functions which have a primitive but are not "integrable" in the sense to which we allude.

### 5. PROPERTIES OF INTEGRALS

The properties of the integrals of regulated functions are simply a translation, into the appropriate notation, of the properties of derivatives demonstrated in chap. I.

In the first place, the formula (3) shows that no matter what the points $x,\ y,\ z$ of I, one has

$$
\int_x^x f(t)\,dt = 0 \tag{4}
$$

$$
\int_x^y f(t)\,dt + \int_y^x f(t)\,dt = 0 \tag{5}
$$

$$
\int_x^y f(t)\,dt + \int_y^z f(t)\,dt + \int_z^x f(t)\,dt = 0 \tag{6}
$$

From prop. 1 of II, p. 52 one has

$$
\int_{x_0}^x (f + g) = \int_{x_0}^x f + \int_{x_0}^x g \tag{7}
$$

and for every scalar $k$

$$
\int_{x_0}^x k f = k \int_{x_0}^x f. \tag{8}
$$

Let E, F be two complete normed spaces over $\mathbf{R}$, and u a continuous linear map from E into F. If f is a regulated function on I with values in E, then $u \circ f$ is a regulated function on I with values in F (II, p. 6, cor. 2), and one has for $a, b \in I$ (I, p. 13, prop. 2)

$$
\int_a^b u(f(t))\,dt = u \left( \int_a^b f(t)\,dt \right). \tag{9}
$$

Now let E, F, G be three complete normed spaces over $\mathbf{R}$, and $(x, y) \mapsto |x.y|$ a continuous bilinear map of $E \times F$ into G. Let f and g be two vector functions defined and continuous on I, taking their values in E and F respectively; suppose moreover that f and g are two primitives of *regulated* functions, which we denote by $f'$ and $g'$ by abuse of language (these functions are not actually guaranteed to be equal to the derivatives of f and g respectively except on the complement of a countable set). By prop. 3 of I, p. 6, the function $h(x) = [f(x).g(x)]$ has, at every point of the complement of a countable subset of I, a derivative equal to $[f(x).g'(x)] + [f'(x).g(x)]$. Now, by the continuity of $[x.y]$ and cor. 2 of II, p. 55, each of the functions $[f.g']$ and $[f'.g]$ is a regulated function on I; so one has the formula

$$
\int_a^b [f'(t).g(t)]\,dt = [f(t).g(t)]\Big|_a^b - \int_a^b |f(t).g'(t)|\,dt \tag{10}
$$

called the *formula for integration by parts*, which allows one to evaluate many primitives.

For example, the formula for integration by parts yields the following formula

$$
\int_{x_0}^{x} t f'(t) \, dt = t f(t) \Big|_{x_0}^{x} - \int_{x_0}^{x} f(t) \, dt
$$

so reducing the evaluation of primitives of one of the two functions $f(x)$ and $x f'(x)$ to the other.

Likewise, if $f$ and $g$ are $n$ times differentiable on an interval $I$, and if $f^{(n)}$ and $g^{(n)}$ are regulated functions on $I$, then formula (5) of I, p. 21 is equivalent to the following:

$$
\int_a^b [f^{(n)}(t) \cdot g(t)] \, dt
$$
$$
= \left( \sum_{p=0}^{n-1} (-1)^p [f^{(n-p-1)}(t) \cdot g^{(p)}(t)] \right) \Bigg|_a^b + (-1)^n \int_a^b [f(t) \cdot g^{(n)}(t)] \, dt
$$
(11)

which one calls the *formula for integration by parts of order n*.

Let us now translate the formula for differentiation of composite functions (I, p. 9, prop. 5). Let $f$ be a real function defined and continuous on $I$, which is the primitive of a *regulated* function on $I$ (which we again write as $f'$ by abuse of language); let, moreover, $g$ be a *continuous* vector function (with values in a complete normed space) on an open interval $J$ containing $f(I)$; if $h$ denotes an arbitrary primitive of $g$ on $J$, then $h$ admits a derivative equal to $g$ at each point of $J$ (II, p. 56, prop 3); thus the composite function $h \circ f$ admits a derivative equal to $g(f(x)) f'(x)$ at all the points of the complement (with respect to $I$) of a countable subset of $I$ (I, p. 9, prop. 5); since the function $g(f(x)) f'(x)$ is regulated (II, p. 55, cor. 2), one can write the formula

$$
\int_a^b g(f(t)) f'(t) \, dt = \int_{f(a)}^{f(b)} g(u) \, du
$$
(12)

called the *formula for change of variables*, which also facilitates the evaluation of primitives.

If, for example, one takes $f(x) = x^2$, one sees that the formula (12) reduces from one to the other the evaluation of the primitives of the functions $g(x)$ and $x g(x^2)$.

To translate the mean value theorem (I, p. 14, th. 1) for primitives of real regulated functions, we first remark that a real regulated function $f$ on a compact interval $I$ is bounded on $I$; let $J$ be the set of points of $I$ where $f$ is *continuous*, and put $m = \inf_{x \in J} f(x)$, $M = \sup_{x \in J} f(x)$; one knows (II, p. 54, th. 3) that $I \cap \mathbf{C}J$ is countable; further, if $B$ is the complement, with respect to $I$, of any countable subset of $I$, and $m' = \inf_{x \in B} f(x)$, $M' = \sup_{x \in B} f(x)$, then one has $m' \leq m \leq M \leq M'$: indeed, for every point $x \in J$, there are points $y$ of B arbitrarily close to $x$, whence $m' \leq f(y) \leq M'$; since $f$ is continuous at the point $x$ one sees, making $y$ approach $x$ ($y$ remaining in B) that $m' \leq f(x) \leq M'$, which proves our assertion. This being so, translating the mean value theorem gives the following proposition:

#### Proposition 6 (theorem of the mean) {#fvr-ii-s1-prop-6 .statement}

*Let $f$ be a real regulated function on a compact interval $l = [a, b]$; if $J$ is the set of points of I where $f$ is continuous, and $m = \inf_{x \in J} f(x)$, $M = \sup_{x \in J} f(x)$, then*

$$
m < \frac{1}{b-a} \int_a^b f(t)\,dt < M
$$

*(13)*

*except when $f$ is constant on J, in which case the three members of (13) are equal.*

In other words, the *mean* of the regulated function $f$ in I lies between the bounds of $f$ over the subset of I where $f$ is continuous.

#### Corollary 1 {#fvr-ii-s1-prop-6-cor-1 .statement}

*If a real regulated function $f$ on I is such that $f(x) \geq 0$ at the points where $f$ is continuous, then* $\frac{1}{b-a} \int_a^b f(t)\,dt > 0$ *unless* $f(x) = 0$ *at the points where* $f$ *is continuous.*

#### Corollary 2 {#fvr-ii-s1-prop-6-cor-2 .statement}

*Let $f$ and $g$ be two real regulated functions on I, such that $g(x) \geq 0$ *at the points where* $g$ *is continuous; if* $m$ *and* $M$ *are the greatest lower bound and least upper bound of* $f$ *over the set of points where* $f$ *is continuous, then*

$$
\frac{m}{b-a} \int_a^b g(t)\,dt \leq \frac{1}{b-a} \int_a^b f(t)g(t)\,dt \leq \frac{M}{b-a} \int_a^b g(t)\,dt.
$$

*(14)*

*The first two terms (resp. the two last) are unequal unless* $g(x)(f(x) - m) = 0$ *(resp. $g(x)(f(x) - M) = 0$) at every point where* $f$ *and* $g$ *are continuous.*

For vector functions the mean value theorem (I, p. 15, th. 2) yields the following proposition:

#### Proposition 7 {#fvr-ii-s1-prop-7 .statement}

*Let* $\mathbf{f}$ *be a regulated vector function on a compact interval* $I = [a, b]$, *with values in a complete normed space* $E$, *and let* $g$ *be a real regulated function on* $I$, *such that* $g(x) \geq 0$ *at the points where* $g$ *is continuous; in these circumstances*

$$
\left\| \int_a^b \mathbf{f}(t)g(t)\,dt \right\| \leq \int_a^b \| \mathbf{f}(t) \| g(t)\,dt.
$$

*(15)*

*In particular,*

$$
\left\| \int_a^b \mathbf{f}(t)\,dt \right\| \leq \int_a^b \| \mathbf{f}(t) \| \,dt.
$$

*(16)*

### 6. INTEGRAL FORMULA FOR THE REMAINDER IN TAYLOR'S FORMULA; PRIMITIVES OF HIGHER ORDER

The formula for integration by parts of order $n$ (II, p. 60, formula (11)) allows one to express in terms of an integral the remainder $r_n(x)$ in the Taylor expansion of order $n$ of a function which admits a regulated $(n+1)^{th}$ derivative on an interval I (I, p. 22); indeed, on replacing, in (12), $f$ by $f'$, $b$ by $x$, and $g(t)$ by the function $(t-x)^n/n!$, it follows that

$$
f(x) = f(a) + f'(a) \frac{(x-a)}{1!} + f''(a) \frac{(x-a)^2}{2!} + \cdots \\
+ f^{(n)}(a) \frac{(x-a)^n}{n!} + \int_a^x f^{(n+1)}(t) \frac{(x-t)^n}{n!} \, dt
$$

in other words

$$
r_n(x) = \int_a^x f^{(n+1)}(t) \frac{(x-t)^n}{n!} \, dt,
$$

which formula often permits one to obtain simple bounds for the remainder.

Given a regulated function $f$ on an interval I, an arbitrary primitive $g$ of $f$, being continuous in I, admits a primitive in its turn; an arbitrary primitive of an arbitrary primitive of $f$ is called a *second primitive* of $f$. More generally, a primitive of a primitive of order $n-1$ of $f$ is termed a *primitive of order* $n$ of $f$. One sees immediately, by induction on $n$, that the difference of two primitives of order $n$ of $f$ is a *polynomial of degree at most equal to* $n-1$ (with coefficients in E). A primitive of order $n$ of $f$ is entirely determined if one specifies its value and those of its first $n-1$ derivatives at a point $a \in I$.

In particular, $\int_a^{(n)} f$ denotes that primitive of order $n$ of $f$ which vanishes, together with its first $n-1$ derivatives, at the point $a$. The Taylor formula of order $n-1$, applied to this primitive, shows that if $g = \int_a^{(n)} f$, then

$$
g(x) = \int_a^x f(t) \frac{(x-t)^{n-1}}{(n-1)!} \, dt
$$

so reducing the determination of a primitive of order $n$ to one single integral.

### Exercises {#fvr-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
