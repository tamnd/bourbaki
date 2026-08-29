---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 2
section_title: THE MEAN VALUE THEOREM
lang: en
source: fvr-i-vii
book_pages: 12-19, 37-39
pdf_pages: 0027-0034, 0052-0054
extraction: ocr
subsections:
    - "no": 1
      title: ROLLE'S THEOREM
      page: 12
      pdf_page: 27
    - "no": 2
      title: THE MEAN VALUE THEOREM FOR REAL-VALUED FUNCTIONS
      page: 13
      pdf_page: 28
    - "no": 3
      title: THE MEAN VALUE THEOREM FOR VECTOR FUNCTIONS
      page: 15
      pdf_page: 30
    - "no": 4
      title: CONTINUITY OF DERIVATIVES
      page: 18
      pdf_page: 33
statements: 21
exercises: 14
content_sha256: b3b7f9d38f4a2886f4332338a1ca2047871b449272d4a73cbe30a131219c1587
---

## § 2. THE MEAN VALUE THEOREM

The hypotheses and conclusions demonstrated in § 1 are local in character: they concern the properties of the functions under consideration only on an arbitrarily small neighbourhood of a fixed point. In contrast, the questions which we treat in this section involve the properties of a function on all of an interval.

### 1. ROLLE'S THEOREM

#### Proposition 1 ("Rolle's theorem") {#fvr-i-s2-prop-1 .statement}

Let $f$ be a real function which is finite and continuous on a closed interval $I = [a, b]$ (where $a < b$), has a derivative (finite or not) at every point of ]$a, b$[, and is such that $f(a) = f(b)$. Then there exists a point $c$ of ]$a, b$[ such that $f'(c) = 0$.

The proposition is evident if $f$ is constant: if not, $f$ takes, for example, values $> f(a)$, and so attains its least upper bound at a point $c$ interior to I (Gen. Top., IV, p. 359, th. 1). Since $f$ has a relative maximum at this point we have $f'(c) = 0$ (I, p. 20, prop. 7).

#### Corollary {#fvr-i-s2-n1-cor-1 .statement}

Let $f$ be a real function which is finite and continuous on $[a, b]$ (where $a < b$), and has a derivative (finite or not) at every point. Then there exists a point $c$ of ]$a, b$[ such that $f(b) - f(a) = f'(c)(b - a)$.

We need only apply prop. 1 to the function $f(x) - \frac{f(b) - f(a)}{b - a}(x - a)$.

This corollary signifies that there is a point $M_c = (c, f(c))$ on the graph $C$ of $f$ such that $a < c < b$ and such that the tangent to $C$ at this point is parallel to the line joining the points $M_a = (a, f(a))$ and $M_b = (b, f(b))$.

### 2. THE MEAN VALUE THEOREM FOR REAL-VALUED FUNCTIONS

The following important result is a consequence of the corollary to prop. 1: if one has $m \leq f'(x) \leq M$ on ]$a, b$[, then also $m \leq \frac{f(b) - f(a)}{b - a} \leq M$. In other words, a *bound for the derivative of* $f'$ on the whole interval with endpoints $a, b$ implies the *same bound* for $\frac{f(b) - f(a)}{b - a}$ (the ratio of the "increment" of the function to the "increment" of the variable on the interval). We shall make this fundamental result more precise, and generalize it, in the sequel.

#### Proposition 2 {#fvr-i-s2-prop-2 .statement}

*Let* $f$ *be a real function which is finite and continuous on the closed bounded interval* $I = [a, b]$ *(where* $a < b$*) and has a right derivative* (finite or not) *at all the points of the relative complement in* $[a, b)$ *of a countable subset* $A$ *of this interval. If* $f'_d(x) \geq 0$ *at every point of* $[a, b[$ *not belonging to* $A$, *then one has* $f(b) \geq f(a)$; *if, further,* $f'_d(x) > 0$ *for at least one point of* $[a, b[$, *then* $f(b) > f(a)$.

Let $\varepsilon > 0$ be arbitrary, and denote by $(a_n)_{n \geq 1}$ a sequence obtained by listing the countable set $A$. Let $J$ be the set of points $y \in I$ such that one has

$$
f(x) - f(a) \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$

(1)

for all $x$ with $a \leq x \leq y$, the sum in the second term of the right-hand side being taken over all indices $n$ for which $a_n < x$. We shall show that if $f'_d(x) \geq 0$ at every point of $[a, b[$ distinct from the $a_n$, then $J = I$.

It is clear that $J$ is not empty, since $a \in J$; moreover the definition of this set shows that if $y \in J$ one has $x \in J$ for $a \leq x \leq y$, so $J$ is an *interval* with left-hand endpoint $a$ (*Gen. Top.*, IV, p. 336, prop. 1); let $c$ be its right-hand endpoint. One has $c \in J$; this is clear if $c = a$; if not, for every $x < c$ we have the inequality (1), and *a fortiori*

$$
f(x) - f(a) \geq -\varepsilon(c - a) - \varepsilon \sum_{a_n < c} \frac{1}{2^n}
$$

from which it follows, on letting $x$ tend to $c$ in this inequality (since $f$ is continuous), that $c$ satisfies (1).

This being so, we shall see that we must have $c = b$. Indeed, if one had $c < b$, then certainly one would have $c \notin A$; now $f'_d(c)$ exists, and since $f'_d(c) \geq 0$ by hypothesis, there exists a $y$ such that $c < y \leq b$ and such that for $c \leq x \leq y$ one has

$$
f(x) - f(c) \geq -\varepsilon(x - c)
$$

from which, taking account of (1), where $x$ is replaced by $c$,

$$
f(x) - f(a) \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < c} \frac{1}{2^n} \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$

which signifies that $y \in J$, contradicting the definition of $c$. Thus we have $c = a_k$ for some index $k$; since $f$ is continuous at the point $a_k$ there is a $y$ such that $c < y \leq b$ and such that for $c < x \leq y$ one has
$$
f(x) - f(c) \geq -\frac{\varepsilon}{2^k}
$$
from which, taking account of (1), where $x$ is replaced by $c$,
$$
f(x) - f(a) \geq -\varepsilon(c-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n} \geq -\varepsilon(x-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$
which again leads to a contradiction; we thus have $c = b$, and in consequence
$$
f(b) - f(a) \geq -\varepsilon(b-a) - \varepsilon \sum_{a_n < b} \frac{1}{2^n} \geq -\varepsilon(b-a) - \varepsilon. \tag{2}
$$
Since $\varepsilon > 0$ is arbitrary we deduce from (2) that $f(b) \geq f(a)$, which demonstrates the first part of the proposition.

We remark now that this result applied to an interval $[x, y]$ where $a \leq x < y \leq b$ proves that $f$ is *increasing* on I; if one had $f(b) = f(a)$ one could deduce that $f$ is *constant* on I, and then that $f'_d(x) = 0$ at every point of $[a, b[$; the second part follows from this.

#### Corollary {#fvr-i-s2-n2-cor-1 .statement}

*Let $f$ be a finite continuous real function on $[a, b]$ (where $a < b$) and have a right derivative at all points of the complement in $[a, b[$ of a countable subset $A$ of this interval. For $f$ to be increasing on I it is necessary and sufficient that $f'_d(x) \geq 0$ at every point of $[a, b[$ that does not belong to $A$; for $f$ to be strictly increasing it is necessary and sufficient that that the preceding condition holds, and further that the set of points $x$ where $f'_d(x) > 0$ be dense in $[a, b]$.*

#### Remark 1 {#fvr-i-s2-n2-rem-1 .statement}

Prop. 2 remains true when one replaces the interval $[a, b[$ by ]$a, b$ and the words "right derivative" by "left derivative".

#### Remark 2 {#fvr-i-s2-n2-rem-2 .statement}

The hypothesis of *continuity* on $f$ on the closed interval I (and not just *right continuity* $^4$ at every point of $[a, b[$) is essential for the validity of prop. 2 (*cf.* I, p. 36, exerc. 8 ).

#### Remark 3 {#fvr-i-s2-n2-rem-3 .statement}

The conclusion of prop. 2 is not guaranteed if one merely supposes that the set $A$ of "exceptional" points is nowhere dense in I, but not countable (*cf.* I, p. 37, exerc. 3).

Prop. 2 entails the following fundamental theorem (which appears to be more general):

**THEOREM 1** (mean value theorem). *Let $f$ and $g$ be two finite continuous real-valued functions defined on a closed bounded interval $I = [a, b]$ and having a

$^4$ A function defined on an interval $I \subset \mathbf{R}$ is said to be *right continuous* at a point $x_0 \in I$ if its restriction to the interval $I \cap [x_0, +\infty[$ is continuous at the point $x_0$ relative to this interval; it comes to the same to say that the right limit of this function exists at this point and is equal to the value of the function at this point.

right derivative (finite or not) at all points of the relative complement in $[a,\ b[$ of a countable subset of this interval. Suppose further that $f'_d(x)$ and $g'_r(x)$ are not simultaneously infinite except at the points of a countable subset of I and that there are finite numbers $m$, $M$ such that

$$
mg'_r(x) \leq f'_d(x) \leq Mg'_r(x)
$$

except at the points of a countable subset of I (replacing $Mg'_r(x)$ (resp. $mg'_r(x)$) by 0 if $M = 0$ (resp. $m = 0$) and $g'_r(x) = \pm \infty$. Under these conditions one has

$$
m(g(b) - g(a)) < f(b) - f(a) < M(g(b) - f(a))
$$

except when one has $f(x) = Mg(x) + k$, or $f(x) = mg(x) + k$ ($k$ constant) for all $x \in I$.

It suffices to apply prop. 2 to the functions $Mg - f$ and $f - mg$, which, under our hypotheses, have a positive right derivative except at the points of a countable subset of I.

#### Remark {#fvr-i-s2-n2-rem-4 .statement}

Th. 1 fails if one allows $f'_d$ and $g'$ to be simultaneously infinite on an uncountable subset of I (cf. I, p. 37, exerc. 3).

#### Corollary {#fvr-i-s2-n2-cor-2 .statement}

Let $f$ be a finite continuous function on $[a,\ b]$ (where $a < b$) and have a right derivative (finite or not) at all points of the relative complement B in $[a,\ b[$ of a countable subset of this interval. If $m$ and $M$ are the greatest lower and least upper bounds of $f'_d$ on B then one has

$$
m(b - a) < f(b) - f(a) < M(b - a)
$$

if $f$ is not an affine linear function; if $f$ is affine linear one has

$$
m = M = \frac{f(b) - f(a)}{b - a}.
$$

The inequalities (5) are consequences of (4) when $m$ and $M$ are finite; the case when one or the other of these numbers is infinite is trivial.

#### Remark {#fvr-i-s2-n2-rem-5 .statement}

The inequalities (5) prove that a continuous function cannot have right derivative equal to $+\infty$ at all points of an interval (cf. I, p. 38, exerc. 6).

### 3. THE MEAN VALUE THEOREM FOR VECTOR FUNCTIONS

#### Theorem 2 {#fvr-i-s2-thm-2 .statement}

Let $f$ be a vector function defined and continuous on a closed bounded interval $I = [a,\ b]$ of $\mathbf{R}$ (where $a < b$) and taking values in a normed space E over $\mathbf{R}$; let $g$ be a continuous increasing real function on I. Suppose that $f$ and $g$ have right derivatives at all points of the relative complement in $[a,\ b[$ of a countable subset A of this interval (allowing $g'_r(x)$ to be infinite at some of the points $x \notin A$), and suppose that at each of these points we have

$$
\| f'_d(x) \| \leq g'_r(x).
$$

Under these hypotheses one has

$$
\| f(b) - f(a) \| \leq g(b) - g(a).
$$

The proof proceeds similarly to that of prop. 2. Let $\varepsilon > 0$ be arbitrary, and $(a_n)$ the sequence obtained by enumerating A in some order. Let J be the set of points $y \in I$ such that, for all $x$ such that $a \leq x \leq y$ one has

$$
\| f(x) - f(a) \| \leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n};
$$

we shall show that $J = I$. One sees immediately, as in prop. 2, that J is an interval with left-hand endpoint $a$; if c is its right-hand endpoint then $c \in J$; indeed, for all $x < c$ one has (8), and *a fortiori*

$$
\| f(x) - f(a) \| \leq g(c) - g(a) + \varepsilon (c - a) + \varepsilon \sum_{a_n < c} \frac{1}{2^n}
$$

from which, letting $x$ tend to $c$ in this inequality, it follows from the continuity of $f$ that $c$ satisfies (8).

Let us show that we must have $c = b$. So suppose that $c < b$ and that moreover $c \notin A$: then $f'_d(c)$ and $g'_r(c)$ exist and satisfy (6); suppose in the first place that $g'_r(c)$ (which is necessarily $\geq 0$) is finite; then one can always write $f'_d(c) = u g'_r(c)$, with $\| u \| \leq 1$; since the function $f(x) - u g(x)$ has zero right derivative at the point $c$ there must exist a $y$ such that $c < y \leq b$ and such that for $c \leq x \leq y$ one has

$$
\| f(x) - f(c) - u(g(x) - g(c)) \| \leq \varepsilon (x - c)
$$

from which

$$
\| f(x) - f(c) \| \leq g(x) - g(c) + \varepsilon (x - c)
$$

and, taking account of (8), in which $x$ is replaced by $c$,

$$
\begin{align*}
\| f(x) - f(a) \| &\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < c} \frac{1}{2^n} \\
&\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}.
\end{align*}
$$

Thus one has $y \in J$, which is a contradiction. Suppose next that $c \notin A$ and that $g'_r(c) = +\infty$; then there is a $y$ such that $c < y \leq b$ and such that for $c \leq x \leq y$ one has on the one hand

$$
\| f(x) - f(c) \| \leq (\| f'_d(c) \| + 1) (x - c)
$$

while on the other hand

$$
g(x) - g(c) \geq (\| f'_d(c) \| + 1) (x - c)
$$

from which

$$
\| f(x) - f(c) \| \leq g(x) - g(c)
$$

and one concludes as above. Finally, if one has $c = a_k$, then there is a $y$ such that $c < y \leq b$, and such that for $c < x \leq y$ one has

$$
\| f(x) - f(c) \| \leq \frac{\varepsilon}{2^k}
$$

from which, taking account of (8), with $x$ replaced by $c$,

$$
\begin{align*}
\| f(x) - f(a) \| &\leq g(c) - g(a) + \varepsilon (c - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n} \\
&\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}
\end{align*}
$$

which again entails a contradiction. The proof finishes as that of prop. 2.

Q.E.D.

#### Remark 1 {#fvr-i-s2-n3-rem-1 .statement}

Here again, in the statement of th. 2 one can replace the interval $[a, b[$ by ]$a, b]$ and "right derivative" by "left derivative".

#### Remark 2 {#fvr-i-s2-n3-rem-2 .statement}

We shall show later how to identify the case of equality in (7), and also how to generalize th. 2 to the case where E is an arbitrary locally convex space, with the help of another method of proof which allows one to deduce th. 2 from th. 1.

#### Corollary {#fvr-i-s2-n3-cor-1 .statement}

For a continuous vector function on an interval $I \subset \mathbf{R}$, with values in a normed space E over $\mathbf{R}$, to be constant on I it suffices that it have zero right derivative at all points of the complement (relative to I) of a countable subset of I.

#### Remark {#fvr-i-s2-n3-rem-3 .statement}

The proofs of ths. 1 and 2 rely in an essential manner on the special topological properties of the field $\mathbf{R}$; one can give examples of valued fields K for which there are nonconstant linear maps of K to itself with zero derivative at every point (cf. I, p. 37, exerc. 2).

#### Proposition 3 {#fvr-i-s2-prop-3 .statement}

Let $f$ be a vector function with values in a normed space E over $\mathbf{R}$, defined and continuous on an interval $I \subset \mathbf{R}$, and right differentiable on the complement B (relative to I) of a countable subset of I; then for all points $x_0 \in B, x \in I, y \in I$, one has (supposing that $x < y$, for example)

$$
\| f(y) - f(x) - f'_d(x_0)(y - x) \| \leq (y - x) \sup_{z \in B, x < z < y} \| f'_d(z) - f'_d(x_0) \|.
$$ (9)

Indeed it suffices to apply th. 2, replacing $f$ by the function

$$
f(z) - f'_d(x_0)z,
$$

and $g$ by the linear function whose derivative is $\sup_{z \in B, x < z < y} \| f'_d(z) - f'_d(x_0) \|$.

Theorem 2 extends to vector functions of a complex variable:

#### Proposition 4 {#fvr-i-s2-prop-4 .statement}

*Let $f$ be a continuous differentiable function of a complex variable defined on a convex open subset $A$ of the field $\mathbf{C}$, with values in a normed space $E$ over the field $\mathbf{C}$. If one has $\|f'(z)\| \leq m$ for all $z \in A$, then one has $\|f(b) - f(a)\| \leq m |b - a|$ for every pair of points $a, b$ of $A$.*

We put $g(t) = \frac{1}{b - a} f(a + t(b - a))$ for $0 \leq t \leq 1$; since $g'(t) = f'(a + t(b - a))$, applying th. 2 to the function $g$ yields the proposition immediately.

#### Corollary {#fvr-i-s2-n3-cor-2 .statement}

*For a vector function $f$ of a complex variable, defined and continuous on an open set $A \subset \mathbf{C}$, and with values in a normed space over $\mathbf{C}$, to be constant, it suffices that it have zero derivative at every point of $A$.*

Indeed, let $a$ be an arbitrary point of $A$; the set $B$ of points $z$ of $A$ where $f(z) = f(a)$ is *closed* because $f$ is continuous; it is also *open*, as is shown by applying prop. 4 (with $m = 0$) to a convex open neighbourhood, contained in $A$, of an arbitrary point of $B$; so is identical to $A$.

#### Proposition 5 {#fvr-i-s2-prop-5 .statement}

*Let $f$ be a vector function of a complex variable, defined, continuous and differentiable on a convex open set $A \subset \mathbf{C}$, taking values in a normed space over the field $\mathbf{C}$; then, no matter what the points $x_0, x$ and $y$ in $A$, one has*
$$
\|f(y) - f(x) - f'_d(x_0)(y - x)\| \leq |y - x| \sup_{z \in A} \|f'(z) - f'(x_0)\|.
$$
(10)

It suffices to apply th. 2 to the function
$$
g(t) = f(x + t(y - x)) - f'(x_0)(y - x)t
$$
on the interval $[0, 1]$.

### 4. CONTINUITY OF DERIVATIVES

#### Proposition 6 {#fvr-i-s2-prop-6 .statement}

*Let $I$ be an open interval in $\mathbf{R}$, let $x_0$ be one of the endpoints of $I$, and $f$ a vector function defined and continuous on $I$, with values in a complete normed space $E$ over $\mathbf{R}$; suppose that $f$ has a right derivative at the points of the complement $B$ in $I$ of a countable subset of $I$. Then for $f'_d(x)$ to have a limit as $x$ tends to $x_0$ while remaining in $B$ and $\neq x_0$ it is necessary and sufficient that $\frac{f(y) - f(x)}{y - x}$ have a limit $c$ as $(x, y)$ tends to $(x_0, x_0)$ subject to $x \in I, y \in I, x \neq x_0, y \neq x_0$ and $x \neq y$. Under these conditions $f$ extends by continuity to the point $x_0$, the right derivative $f'_d(x)$ tends to $c$ as $x$ tends to $x_0$ (while remaining in B) and the function $f$ extended (defined on $I \cup \{x_0\}$) has derivative at $x_0$ equal to $c$.

Suppose for example that $x_0$ is the right-hand endpoint of I. Let us first show that if $f'_d(x)$ tends to $c$ as $x$ tends to $x_0$ while remaining in B and $\neq x_0$, then $\frac{f(y) - f(x)}{y - x}$ tends to $c$; this follows immediately from th. 2 applied to the function $f(z) - cz$, which yields

$$
\| f(y) - f(x) - c(y - x) \| \leq (y - x) \sup_{z \in B,\ x < z < y} \| f'_d(z) - c \|
$$

for $x < y < x_0$. Conversely, if $\frac{f(y) - f(x)}{y - x}$ tends to $c$, then for every $\varepsilon > 0$ there exists an $h > 0$ such that the conditions $|x - x_0| < h,\ |y - x_0| < h\ (x \neq x_0,\ y \neq x_0)$ imply

$$
\| f(y) - f(x) - c(y - x) \| \leq \varepsilon |y - x|.
$$

But for all $x \in B$ and $\neq x_0$ such that $|x - x_0| < h$ there exists a $k > 0$ (depending on $x$) such that the relation $x < y < x + k$ entails

$$
\| f(y) - f(x) - f'_d(x)(y - x) \| \leq \varepsilon |y - x|
$$

from which, considering (11):

$$
\| f'_d(x) - c \| \leq 2\varepsilon
$$

for $|x - x_0| < h,\ x \in B$ and $x \neq x_0$. which proves that $f'_d(x)$ tends to $c$. Moreover, from the relation (11) one has immediately that

$$
\| f(y) - f(x) \| \leq (\|c\| + \varepsilon) |y - x|,
$$

which proves (by Cauchy's criterion) that $f$ has a limit $d$ at the point $x_0$ as $x$ tends to this point while remaining in I and $\neq x_0$; now, letting $x$ approach $x_0$ in (11), for $y \in I,\ y \neq x_0$ and $|y - x_0| \leq h$, we have

$$
\left\| \frac{f(y) - d}{y - x_0} - c \right\| \leq \varepsilon
$$

which proves that $c$ is the derivative at the point $x_0$ of the function $f$ extended by continuity to $I \cup \{x_0\}$.

#### Remark {#fvr-i-s2-n4-rem-1 .statement}

A similar argument, based on th. 1, shows that if $f$ is a real function such that $f'_d(x)$ tends to $+\infty$ at the point $x_0$ then the ratio

$$
(f(y) - f(x))/(y - x)
$$

also tends to $+\infty$, and conversely; if moreover $f$ has a finite limit at the point $x_0$ (which is not a consequence of the present hypothesis), then the function $f$ extended by continuity to $x_0$ has a derivative equal to $+\infty$ at this point.

### Exercises {#fvr-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
