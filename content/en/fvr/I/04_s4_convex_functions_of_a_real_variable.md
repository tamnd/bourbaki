---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 4
section_title: CONVEX FUNCTIONS OF A REAL VARIABLE
lang: en
source: fvr-i-vii
pdf_pages: 0038-0048, 0060-0064
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A CONVEX FUNCTION
      page: 0
      pdf_page: 39
    - "no": 2
      title: FAMILIES OF CONVEX FUNCTIONS
      page: 0
      pdf_page: 42
    - "no": 3
      title: CONTINUITY AND DIFFERENTIABILITY OF CONVEX FUNCTIONS
      page: 0
      pdf_page: 42
    - "no": 4
      title: CRITERIA FOR CONVEXITY
      page: 0
      pdf_page: 45
statements: 21
exercises: 10
content_sha256: 7ce62adb175e316461e0076f49e0da867be5dc77b36f37f3c179a2545bb96dd9
---

## § 4. CONVEX FUNCTIONS OF A REAL VARIABLE

Let $H$ be a subset of $\mathbf{R}$. $f$ a finite real function defined on $H$, and let $G$ be the *graph* or representative set of the function $f$ in $\mathbf{R} \times \mathbf{R} = \mathbf{R}^2$, the set of points $M_x = (x, f(x))$, where $x$ runs through $H$. It is convenient to say that a point $(a, b)$ of $\mathbf{R}^2$ such that $a \in H$ lies *above* (resp. *strictly above*, *below*, *strictly below*) $G$ if one has $b \geq f(a)$ (resp. $b > f(a)$, $b \leq f(a)$, $b < f(a)$). If $A = (a, a')$ and $B = (b, b')$ are two points of $\mathbf{R}^2$ we denote by $AB$ the closed segment with endpoints $A$ and $B$; if $a < b$ then $AB$ is the graph of the linear function $a' + \frac{b' - a'}{b - a} (x - a)$ defined on $[a, b]$; we denote the slope $\frac{b' - a'}{b - a}$ of this segment by $p(AB)$, and will make use of the following lemma, whose verification is immediate:

#### Lemma {#fvr-i-s4-n0-lem-1 .statement}

*Let $A = (a, a')$, $B = (b, b')$, $C = (c, c')$ be three points in $\mathbf{R}^2$ such that $a < b < c$. The following statements are equivalent:*

a) *B is below AC;*
b) *C lies above the line passing through A and B;*
c) *A is above the line passing through B and C;*
d) $p(AB) \leq p(AC)$;
e) $p(AC) \leq p(BC)$.

The lemma still holds when one replaces "above" (resp. "below") by "strictly above" (resp. "strictly below") and the sign $\leq$ by < (fig. 1).

![Graph showing points A, B, C, and segments labeled with x values a, b, c](../images/fig_1.png)

Fig. 1

### 1. DEFINITION OF A CONVEX FUNCTION

#### Definition 1 {#fvr-i-s4-def-1 .statement}

We say that a finite numerical function $f$, defined on an interval $I \subset \mathbf{R}$, is convex on $I$ if, no matter what the points $x, x'$ of $I$, ($x < x'$), every point $M_z$ of the graph $G$ of $f$ such that $x \leq z \leq x'$ lies below the segment $M_xM_{x'}$ (or, what comes to the same, if every point of this segment lies above $G$) (fig. 2).

![Graph showing points M_x, M_z, M_{x'}, and curve G](../images/fig_2.png)

Fig. 2

Taking account of the parametric representation of a segment (Gen. Top., VI, p. 35), the condition for $f$ to be convex on I is that one has the inequality

$$
f(\lambda x + (1 - \lambda)x') \leq \lambda f(x) + (1 - \lambda)f(x')
$$

for each pair of points $(x, x')$ of I and every $\lambda \in [0, 1]$.

Definition 1 is equivalent to the following: *the set of points in $\mathbf{R}^2$ lying above the graph G of $f$ is convex*. Indeed, this condition is clearly sufficient for $f$ to be convex on I; it is also necessary, for if $f$ is convex on I, and if $(x, y), (x', y')$ are two points lying above G, then one has $y \geq f(x),\ y' \geq f(x')$, from which, for $0 \leq \lambda \leq 1$,

$$
\lambda y + (1 - \lambda)y' \geq \lambda f(x) + (1 - \lambda)f(x') \geq f(\lambda x + (1 - \lambda)x')
$$

by (1), which shows that every point of the segment with endpoints $(x, y)$ and $(x', y')$ lies above G.

#### Remark {#fvr-i-s4-n1-rem-1 .statement}

On sees in the same way that the set of points lying *strictly above* G is convex. Conversely, if this set is convex one has

$$
\lambda y + (1 - \lambda)y' > f(\lambda x + (1 - \lambda)x')
$$

for $0 \leq \lambda \leq 1$ and $y > f(x),\ y' > f(x')$; on letting y tend to $f(x)$ and $y'$ approach $f(x')$ in this formula it follows that $f$ is convex.

#### Example 1 {#fvr-i-s4-n1-exa-1 .statement}

Every (real) affine linear function $ax + b$ is convex on $\mathbf{R}$.
2) The function $x^2$ is convex on $\mathbf{R}$, since one has

$$
\lambda x^2 + (1 - \lambda)(x')^2 - \left( \lambda x + (1 - \lambda)x' \right)^2 = \lambda(1 - \lambda)(x - x')^2 \geq 0
$$

for $0 \leq \lambda \leq 1$.
3) The function $|x|$ is convex on $\mathbf{R}$, since

$$
|\lambda x + (1 - \lambda)x'| \leq \lambda |x| + (1 - \lambda)|x'|
$$

for $0 \leq \lambda \leq 1$.

It is clear that if $f$ is convex on I, then its restriction to any interval $J \subset I$ is convex on J.

Let $f$ be a convex function on I, and $x, x'$ two points of I such that $x < x'$; if $z \in I$ is *exterior* to $[x, x']$ then $M_z$ lies *above* the line D joining $M_x$ and $M_{x'}$; this is an immediate consequence of the lemma.

One deduces from this that if $z$ is a point such that $x < z < x'$ and such that $M_z$ lies *on* the segment $M_x M_{x'}$, then, for *every other point* $z'$ such that $x < z' < x'$ the point $M_{z'}$ also lies *on* the segment $M_x M_{x'}$, for it follows from the above that $M_{z'}$ is at the same time both above and below this segment; in other words, $f$ is then equal to an *affine linear* function on $[x, x']$.

#### Definition 2 {#fvr-i-s4-def-2 .statement}

*We say that a finite real function $f$ defined on an interval $I \subset \mathbf{R}$ is strictly convex on I if, for any points $x, x'$ of I ($x < x'$), every point $M_z$ of the graph G of $f$ such that $x < z < x'$ lies strictly below the segment $M_x M_{x'}$ (or, what comes to the same, if every point of the segment, apart from the endpoints, lies strictly above G).*

In other words, we must have the inequality

$$
f(\lambda x + (1 - \lambda)x') < \lambda f(x) + (1 - \lambda)f(x')
$$

for every pair of distinct points $(x, x')$ of $I$ and every $\lambda$ such that $0 < \lambda < 1$.

The remarks that precede def. 2 show that for a convex function $f$ to be strictly convex on $I$ it is necessary and sufficient that there be no interval contained in $I$ (not reducing to a single point) such that the restriction of $f$ to this interval is *affine linear*.

Of the examples above, the first and third are not strictly convex; on the other hand, $x^2$ is strictly convex on $\mathbf{R}$; a similar calculation shows that $1/x$ is strictly convex on $[0, +\infty[$.

#### Proposition 1 {#fvr-i-s4-prop-1 .statement}

*Let $f$ be a finite real function, convex (resp. strictly convex) on an interval $I \subset \mathbf{R}$. For every family $(x_i)_{1 \leq i \leq p}$ of $p \geq 2$ distinct points of $I$, and every family $(\lambda_i)_{1 \leq i \leq p}$ of $p$ real numbers such that $0 < \lambda_i < 1$ and $\sum_{i=1}^p \lambda_i = 1$, we have*

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i)
$$

(resp.

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i)).
$$

Since the proposition (for convex functions) reduces to the inequality (1) for $p = 2$ we argue by induction for $p > 2$. The number $\mu = \sum_{i=1}^{p-1} \lambda_i$ is $> 0$; it is immediate that if $a$ and $b$ are the smallest and largest of the $x_i$ then $a \leq \frac{\sum_{i=1}^{p-1} \lambda_i x_i}{\sum_{i=1}^{p-1} \lambda_i} \leq b$; in other words, the point $x = \frac{1}{\mu} \sum_{i=1}^{p-1} \lambda_i x_i$ belongs to $I$, and the induction hypothesis implies that $\mu f(x) \leq \sum_{i=1}^{p-1} \lambda_i f(x_i)$; moreover we have, from (1), that

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) = f(\mu x + (1 - \mu)x_p) \leq \mu f(x) + (1 - \mu)f(x_p) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

One argues in the same way for strictly convex functions, starting from the inequality (2).

We say that a finite real function $f$ is *concave* (resp. *strictly concave*) on $I$ if $-f$ is convex (resp. strictly convex) on $I$. It comes to the same to say that for every pair $(x, x')$ of distinct points of $I$ and every $\lambda$ such that $0 < \lambda < 1$ one has

$$
f(\lambda x + (1 - \lambda)x') \geq \lambda f(x) + (1 - \lambda)f(x')
$$

(resp. $f(\lambda x + (1 - \lambda)x') > \lambda f(x) + (1 - \lambda)f(x')$).

### 2. FAMILIES OF CONVEX FUNCTIONS

#### Proposition 2 {#fvr-i-s4-prop-2 .statement}

Let $f_i$ ($1 \leq i \leq p$) be $p$ convex functions on an interval $I \subset \mathbf{R}$, and $c_i$ ($1 \leq i \leq p$) be $p$ arbitrary positive numbers; then the function $f = \sum_{i=1}^p c_i f_i$ is convex on $I$. Further, if for at least one index $j$ the function $f_j$ is strictly convex on $I$, and $c_j > 0$, then $f$ is strictly convex on $I$.

This follows immediately by applying the inequality (1) (resp. (2)) to each of the $f_i$, multiplying the inequality for $f_i$ by $c_i$, and then adding term-by-term.

#### Proposition 3 {#fvr-i-s4-prop-3 .statement}

Let $(f_\alpha)$ be a family of convex functions on an interval $I \subset \mathbf{R}$; if the upper envelope $g$ of this family is finite at every point of $I$ then $g$ is convex on $I$.

Indeed, the set of points $(x, y) \in \mathbf{R}^2$ lying above the graph of $g$ is the intersection of the convex sets formed by the points lying above the graph of each of the functions $f_\alpha$; so it is convex.

#### Proposition 4 {#fvr-i-s4-prop-4 .statement}

Let $H$ be a set of convex functions on an interval $I \subset \mathbf{R}$; if $\mathfrak{F}$ is a filter on $H$ which converges pointwise on $I$ to a finite real function $f_0$, then this function is convex on $I$.

To see this it suffices to pass to the limit along $\mathfrak{F}$ in the inequality (1).

### 3. CONTINUITY AND DIFFERENTIABILITY OF CONVEX FUNCTIONS

#### Proposition 5 {#fvr-i-s4-prop-5 .statement}

For a real finite function $f$ to be convex (resp. strictly convex) on an interval $I$ it is necessary and sufficient that for all $a \in I$ the gradient

$$
p(M_a M_x) = \frac{f(x) - f(a)}{x - a}
$$

be an increasing (resp. strictly increasing) function of $x$ on $I \cap \mathbf{C}\{a\}$.

This proposition is an immediate consequence of definitions 1 and 2 and of the lemma of I, p. 23.

#### Proposition 6 {#fvr-i-s4-prop-6 .statement}

Let $f$ be a finite real function convex on an interval $I \subset \mathbf{R}$. Then at every interior point $a$ of $I$ the function $f$ is continuous, has finite right and left derivatives, and $f'_g(a) \leq f'_d(a)$.

Indeed, for $x \in I$ and $x > a$ the function $x \mapsto \frac{f(x) - f(a)}{x - a}$ is increasing (prop. 5) and bounded below, since if $y < a$ and $y \in I$ we have

$$
\frac{f(y) - f(a)}{y - a} \leq \frac{f(x) - f(a)}{x - a}
$$
(5)

by prop. 5; this function therefore has a finite right limit at the point $a$; in other words, $f'_d(a)$ exists and is finite; further, letting $x$ approach $a$ ($x > a$) in (5), it follows that

$$
\frac{f(y) - f(a)}{y - a} \leq f'_d(a)
$$
(6)

for all $y < a$ belonging to I. In the same way one shows that $f'_g(a)$ exists and that

$$
f'_d(a) \leq \frac{f(x) - f(a)}{x - a}
$$
(7)

for $x \in I$ and $x > a$. On letting $x$ approach $a$ ($x > a$) in this last inequality we obtain $f'_g(a) \leq f'_d(a)$. The existence of the left and right derivatives at the point $a$ clearly ensures the continuity of $f$ at this point.

#### Corollary 1 {#fvr-i-s4-prop-6-cor-1 .statement}

*Let $f$ be a convex (resp. strictly convex) function on I; if $a$ and $b$ are two interior points of I such that $a < b$ one has* (fig. 3)

![A graph showing a convex function with tangents at points a and b, labeled M_a and M_b, respectively.](../images/fig_3.png)

Fig. 3

$$
f'_d(a) \leq \frac{f(b) - f(a)}{b - a} \leq f'_g(b)
$$
(8)

(resp.

$$
f'_d(a) < \frac{f(b) - f(a)}{b - a} < f'_g(b)
$$
(9)

The double inequality (8) results from (6) and (7) by a simple change of notation. On the other hand, if $f$ is strictly convex and $c$ is such that $a < c < b$ one has, from (8) and prop. 5,

$$
f'_d(a) \leq \frac{f(c) - f(a)}{c - a} < \frac{f(b) - f(a)}{b - a} < \frac{f(b) - f(c)}{b - c} \leq f'_g(b)
$$

from which (9).

#### Corollary 2 {#fvr-i-s4-prop-6-cor-2 .statement}

*If $f$ is convex (resp. strictly convex) on I then $f'_d$ and $f'_g$ are increasing (resp. strictly increasing) on the interior of I; the set of points in I at which $f$ is not differentiable is countable, and $f'_d$ and $f'_g$ are continuous at every point where $f$ is differentiable.*

The first part follows immediately from (8) (resp. (9)) and the inequality

$$
f'_g(a) \leq f'_d(a).
$$

On the other hand, let E be the set of interior points $x$ of I where $f$ is not differentiable (that is $f'_g(x) < f'_d(x)$). For each $x \in E$ let $J_x$ be the open interval $]f'_g(x), f'_d(x)[$; it follows from (8) that if $x$ and $y$ are two points of E such that $x < y$, then $u < v$ for all $u \in J_x$ and all $v \in J_y$; in other words, as $x$ runs through E the open nonempty intervals $J_x$ are pairwise disjoint; the set of such intervals is thus countable, and hence so is E. Finally, $f'_d$ (resp. $f'_g$) being increasing, it has a right limit and a left limit at every interior point $x$ of I; prop. 6 of I, p. 18 now shows that the right limit of $f'_d$ (resp. $f'_g$) at the point $x$ is equal to $f'_d(x)$, and its left limit is $f'_g(x)$, from which we have the last part of the corollary.

Let $f$ be a convex function on I, $a$ an interior point of I, and D a line passing through the point $M_a$, with equation $y - f(a) = \alpha(x - a)$. It follows from the inequalities (8) that if $f'_g(a) \leq \alpha \leq f'_d(a)$ then every point of the graph G lies *above* D, and, if $f$ is strictly convex, $M_a$ is the only point common to D and G; one says that D is a *support line* to G at the point $M_a$. Conversely, if G lies above D, one has $f(x) - f(a) \geq \alpha(x - a)$ for every $x \in I$, from which $\frac{f(x) - f(a)}{x - a} \geq \alpha$ for $x > a$, and $\frac{f(x) - f(a)}{x - a} \leq \alpha$ for $x < a$; on letting $x$ tend to $a$ in these inequalities it follows that $f'_g(a) \leq \alpha \leq f'_d(a)$.

In particular, if $f$ is differentiable at the point $a$ there is *only one* supporting line to G at the point $M_a$, the *tangent* to G at $M_a$.

#### Remark {#fvr-i-s4-n3-rem-1 .statement}

If $f$ is a strictly convex function on an open interval I then $f'_d$ is strictly increasing on I, so there are three possible cases, according to prop. 2 of I, p. 13:
1. $f$ is strictly decreasing on I;
2. $f$ is strictly increasing on I;
3. there is an $a \in I$ such that $f$ is strictly decreasing for $x \leq a$, and is strictly increasing for $x \geq a$.

When $f$ is convex on I, but not strictly convex, $f$ can be constant on an interval contained in I; let $J = ]a, b[$ be the largest open interval on which $f$ is constant (that is to say, the interior of the interval where $f'_d(x) = 0$); then $f$ is strictly decreasing on the interval formed by the points $x \in I$ such that $x \leq a$ (if it exists), strictly increasing on the interval formed by the points $x \in I$ such that $x \geq b$ (if it exists).

In all cases one sees that $f$ possesses a *right limit* at the left-hand endpoint of $I$ (in $\overline{\mathbf{R}}$), and a *left limit* at the right-hand endpoint; these limits may be finite or infinite (*cf.* I, p. 46, exerc. 5, 6 and 7). By abuse of language one sometimes says that the continuous function (with values in $\overline{\mathbf{R}}$), equal to $f$ on the interior of $I$, and extended by continuity to the endpoints of $I$, is *convex on* $\overline{I}$.

### 4. CRITERIA FOR CONVEXITY

#### Proposition 7 {#fvr-i-s4-prop-7 .statement}

*Let $f$ be a finite real function defined on an interval $I \subset \mathbf{R}$. For $f$ to be convex on $I$ it is necessary and sufficient that for every pair of numbers $a, b$ of $I$ such that $a < b$, and for every real number $\mu$, the function $f(x) + \mu x$ attains its supremum on $[a, b]$ at one of the points $a, b$.*

The condition is *necessary*; indeed, since $\mu x$ is convex on $\mathbf{R}$, the function $f(x) + \mu x$ is convex on $I$; one can therefore restrict oneself to the case $\mu = 0$. Then, for
$$
x = \lambda a + (1 - \lambda) b \quad (0 \leq \lambda \leq 1),
$$
one has
$$
f(x) \leq \lambda f(a) + (1 - \lambda) f(b) \leq \operatorname{Max}(f(a), f(b)).
$$

The condition is *sufficient*. Let us take $\mu = -\frac{f(b) - f(a)}{b - a}$ and let $g(x) = f(x) + \mu x$; one has $g(a) = g(b)$ and therefore $g(x) \leq g(a)$ for all $x \in [a, b]$, and one can check immediately that this inequality is equivalent to the inequality (1) where one replaces $z$ by $a$ and $x'$ by $b$.

#### Proposition 8 {#fvr-i-s4-prop-8 .statement}

*For a finite real function $f$ to be convex (resp. strictly convex) on an open interval $I \subset \mathbf{R}$ it is necessary and sufficient that it be continuous on $I$, have a derivative at every point of the complement $B$ relative to $I$ of a countable subset of this interval, and that the derivative be increasing (resp. strictly increasing) on $B$.*

The condition is necessary, from prop. 6 and its corollary 2 (I, p. 27); let us show that it is sufficient. Suppose, therefore, that $f'$ is increasing on $B$, and that $f$ is not convex; there then exist (I, p. 27, prop. 5) three points $a, b, c$ of $I$, such that $a < c < b$, and $\frac{f(c) - f(a)}{c - a} > \frac{f(b) - f(c)}{b - c}$; but from the mean value theorem (I, p. 14, th. 1) one has
$$
\frac{f(c) - f(a)}{c - a} \leq \sup_{x \in B,\ a < x < c} f'(x) \quad \text{and} \quad \frac{f(b) - f(c)}{b - c} \geq \inf_{x \in B,\ c < x < b} f'(x).
$$

One thus has $\sup_{\lambda \in B,\ a < \lambda < c} f'(\lambda) > \inf_{\lambda \in B,\ c < \lambda < b} f'(\lambda)$, contrary to the hypothesis that $f'$ is increasing on $B$.

If now we assume that $f'$ is strictly increasing on $B$, then $f$ is convex and cannot be equal to an affine linear function on any open interval contained in $I$, for then $f'$ would be constant on this interval, contrary to the hypothesis.

#### Corollary {#fvr-i-s4-n4-cor-1 .statement}

*Let $f$ be a finite real function, continuous and twice differentiable on an interval $I \subset \mathbf{R}$; for $f$ to be convex on $I$ it is necessary and sufficient that $f''(x) \geqslant 0$ for all $x \in I$; for $f$ to be strictly convex on $I$ it is necessary and sufficient that the previous condition be satisfied and further that the set of points $x \in I$ where $f''(x) > 0$ be dense in $I$.*

This follows immediately from the preceding proposition, and from the corollary at I, p. 14.

#### Example {#fvr-i-s4-n4-exa-1 .statement}

On the interval ]$0, +\infty$ [ the function $x^r$ ($r$ any real number) has a second derivative equal to $r(r-1)x^{-2}$; thus it is strictly convex if $r > 1$ or $r < 0$, and strictly concave if $0 < r < 1$. \*

In order to be able to formulate another criterion for convexity we make the following definition: given the graph $G$ of a finite real function defined on an interval $I \subset \mathbf{R}$ and an interior point $a$ of $I$, we shall say that a line $D$ passing through $M_a = (a, f(a))$ is *locally above* (resp. *locally below*) $G$ if there exists a neighbourhood $V \subset I$ of $a$ such that every point of $D$ contained in $V \times \mathbf{R}$ is above (resp. below) $G$; we shall say that $D$ is *locally on* $G$ at the point $M_a$ if there is a neighbourhood $V \subset I$ of $a$ such that the intersection of $D$ and $V \times \mathbf{R}$ is identical to that of $G$ and $V \times \mathbf{R}$ (in other words, if $D$ is simultaneously locally above and locally below $G$).

#### Proposition 9 {#fvr-i-s4-prop-9 .statement}

*Let $f$ be a real finite function which is upper semi-continuous on an open interval $I \subset \mathbf{R}$. For $f$ to be convex on $I$ it is necessary and sufficient that for every point $M_x$ of the graph $G$ of $f$ every line locally above $G$ at this point should be locally on $G$ (at the point $M_x$).*

The condition is *necessary*: indeed, if $f$ is convex on $I$ then at every point $M_a$ of the graph $G$ of $f$ there exists a *support line* $\Delta$ to $G$: now $\Delta$ is below $G$, so *a fortiori* locally below $G$ (I, p. 29); if a line $D$ is locally above $G$ at the point $M_a$ it is locally above $\Delta$, so must coincide with $\Delta$, and consequently is locally on $G$ at the point $M_a$.

The condition is *sufficient*. Indeed, suppose it is satisfied, and suppose that $f$ is not convex on $I$; then there are two points $a, b$ of $I$ ($a < b$) such that there are points $M_x$ of $G$ strictly above the segment $M_aM_b$ (fig. 4). In other words, the function $g(x) = f(x) - f(a) - \frac{f(b) - f(a)}{b - a}(x - a)$ takes values $> 0$ on $[a, b]$; since $g$ is finite and upper semi-continuous on this compact interval its least upper bound $k$ on $[a, b]$ is finite and $> 0$, and the set $g^{-1}(k)$ is closed and not empty (\emph{Gen. Top.}, IV, p. 361, th. 3 and prop. 1). Let $c$ be the greatest lower bound of $g^{-1}(k)$; we have $a < c < b$. and at the point $M_c$ the line D with equation $y = f(c) + \frac{f(b) - f(a)}{b - a}(x - c)$ lies locally above G; but it cannot be locally on G at this point, since, for $a < x < c$, one has $g(x) < k$, which signifies that $M_x$ is strictly below D. This has led us to a contradiction, which establishes the proposition.

#### Corollary 1 {#fvr-i-s4-prop-9-cor-1 .statement}

*For a real finite function* $f$ *defined on an open interval* $I \subset \mathbf{R}$ *and upper semi-continuous on* $I$ *to be convex on* $I$ *it is necessary and sufficient that for all* $x \in I$ *there should exist an* $\varepsilon > 0$ *such that the relation* $|h| \leq \varepsilon$ *entails*

$$
f(x) \leq \frac{1}{2} \left( f(x + h) + f(x - h) \right).
$$

We have only to show that the condition is *sufficient*. Indeed, if at a point $M_a$ of the graph G of $f$ a line D is locally above G, then it is locally on G at this point; for, in the opposite case, for example, a point $M_{a+h}$ would be strictly below D, while a point $M_{a-h}$ would be below D: the mid-point of the segment $M_{a-h}M_{a+h}$ would thus be strictly above D (fig. 5), and, in virtue of the hypothesis, $M_a$ would *a fortiori* be strictly below D, which is absurd.

![A graph showing a convex function with points M_{a-h}, M_a, M_{a+h} and a tangent line labeled D.](https://i.imgur.com/3Q5z5QG.png)

Fig. 5

#### Corollary 2 {#fvr-i-s4-prop-9-cor-2 .statement}

*Let $f$ be a finite real function defined on an open interval $I \subset \mathbf{R}$. If for every point $x \in I$ there is an open interval $J_x \subset I$ containing $x$ and such that the restriction of $f$ to $J_x$ is convex on $J_x$, then $f$ is convex on $I$.*

It is clear that $f$ satisfies the criterion of prop. 9.

### Exercises {#fvr-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
