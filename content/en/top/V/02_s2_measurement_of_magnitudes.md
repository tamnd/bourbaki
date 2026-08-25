---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 2
section_title: Measurement of magnitudes
lang: en
source: top-v-x
pdf_pages: 0018-0023, 0031-0031
extraction: ocr
statements: 5
exercises: 2
content_sha256: 80ce56e645cdb24e359494fc910508a3b3a5858b7f204089f807d881480ea6a7
---

## 2. MEASUREMENT OF MAGNITUDES

We have seen (cf. the historical note to Chapter IV) that the problem of the measurement of magnitudes is at the origin of the concept of real number; more precisely, the various types of magnitudes which gradually came to be studied, for practical or theoretical purposes, were first considered separately from each other, and the possibility of measuring all types by the same number system had appeared as an experimental fact well before the Greeks had conceived the bold idea of giving a rigorous demonstration. In the axiomatic theory they established, the idea of magnitude was related to a law of composition ("addition" of magnitudes of the same type) and an order-relation (the relation "A is smaller than B", called the relation of comparison of magnitudes). In what follows we shall examine the same problem, that is to say we shall investigate the conditions that must be imposed on an internal law of composition and an order-relation on a set E in order that it should be isomorphic to a subset E' of R, endowed with the structure induced by addition and the relation $ \leq $ in R. As we shall not assume a priori that the given law of composition on E is commutative, we shall use the multiplicative notation; but apart from this we shall scarcely depart from the classical arguments.

Let E be a set linearly ordered by an order relation written $ x \leq y $, and suppose that E has a smallest element $ \omega $. Let I be a subset of E such that $ \omega \in I $, and such that the relations $ x \in I $ and $ y \leq x $ imply $ y \in I $; suppose also that we are given a law of composition $ (x, y) \to xy $ on E, the product $ xy $ being defined for all pairs of elements of I ($ xy $ belongs to E, but not necessarily to I). Furthermore, we make the following assumptions:

(GR_I) $ \omega $ is the identity element [$ \omega x = x \omega = x $ for all $ x \in I $] and the law of composition is associative [in the following sense: whenever $ x \in I, y \in I, z \in I, xy \in I $ and $ yz \in I $, then $ x(yz) = (xy)z $].

(GR_{II}) The relation $ x < y $ between elements of I implies, for all $ z \in I $, the relations $ xz < yz $ and $ zx < zy $.

(GR_{III}) The set of elements $ > \omega $ in I is not empty and has no smallest element; and given any elements $ x, y $ of I such that $ x < y $, there exists $ z > \omega $ such that $ xz \leq y $.

The condition (GR_{II}) implies that inequalities between elements of I may be multiplied term by term: $ x < y $ and $ x' < y' $ imply $ xx' < yy' $ (for $ xx' < yx' $ and $ yx' < yy' $). In particular we have $ y < yx $ for all $ x > \omega $ ($ x \in I, y \in I $).

Given a finite sequence $ (x_i)_{1 \leq i \leq p} $ of elements of I, we may define by induction on $ p $ the product of this sequence $ \prod_{i=1}^p x_i $ as being equal to $\left( \prod_{i=1}^{p-1} x_i \right) x_p$, provided that the product $\prod_{i=1}^{p-1} x_i$ is defined and belongs to I: thus if $\prod_{i=1}^p x_i$ is defined, each of the products $\prod_{i=1}^q x_i$ is defined and belongs to I, for $2 \leq q \leq p - 1$. By taking all the $x_i$ equal to the same element $x \in I$, we see in particular that if $x^p$ is defined, then $x^q$ is defined and belongs to I for $2 \leq q \leq p - 1$. Conventionally we define $x^0$ to be equal to $\omega$, for all $x \in I$. By (GR$_\text{II}$), if $x > \omega$, we have $\omega < x^q < x^p$ for $1 \leq q \leq p - 1$ if $x^p$ is defined; if $x < y$ and if $y^p$ is defined, then we see (by induction on $p$) that $x^p$ is defined and $x^p < y^p$. On the other hand, the associativity condition (GR$_\text{I}$) implies by induction on $n$ that, if $x^{m+n}$ is defined, then so is $x^m x^n$, and that $x^{m+n} = x^m x^n$. Conversely, by virtue of (GR$_\text{I}$) and (GR$_\text{II}$), if $x^m x^n$ is defined and belongs to I, then $x^{m+n}$ is defined and we have $x^{m+n} = x^m x^n$; again this is proved by induction on $n$, for we have $x^{n-1} \leq x^n$, therefore $x^m x^{n-1}$ is defined and belongs to I; by hypothesis, $x^m x^{n-1} = x^{m+n-1} \in I$, hence $(x^{m+n-1})x = x^{m+n}$ is defined and equal to $x^m x^n$ by the previous result. One shows likewise by induction on $n$ that, if $x^{mn}$ is defined, then $(x^m)^n$ is defined and that $x^{mn} = (x^m)^n$; and that conversely if $(x^m)^n$ is defined and belongs to I, then $x^{mn}$ is defined and equal to $(x^m)^n$.

Finally, the axiom (GR$_\text{III}$) implies that, for all $x \in I$ such that $x > \omega$, there exists $y > \omega$ such that $y^2 \leq x$. For if $x > \omega$ there exists $z > \omega$ such that $z < x$, and then $t > \omega$ such that $zt \leq x$; take $y$ to be the smaller of the two elements $z, t$. By induction on $n$, we deduce that there exists $u > \omega$ such that $u^{2^n} \leq x$.

Let us now introduce the following assumption:

(GR$_\text{IV}$) ("Archimedes' axiom"). *For all* $x \in I$ *and* $y \in I$ *such that* $x > \omega$, *there exists an integer* $n > 0$ *such that* $x^n$ *is defined and* $x^n > y$.

If we take E to be a set of real numbers $\geq 0$ which contains 0 and arbitrarily small numbers $> 0$, I to be the intersection of E with an interval of R which has 0 as its left-hand end-point and contains at least one other number, the law of composition to be addition of elements of I, and if we suppose that $x + y \in E$ whenever $x \in I$ and $y \in I$ then it is clear that the axioms (GR$_\text{I}$), (GR$_\text{II}$), (GR$_\text{III}$) and (GR$_\text{IV}$) are satisfied (*).

(*) In the sets of "magnitudes" which arise in the experimental sciences, the axioms (GR$_\text{I}$) and (GR$_\text{II}$) are in general capable of experimental verification, at any rate approximately. On the other hand, axiom (GR$_\text{III}$), which postulates the existence of magnitudes "as small as we please", clearly cannot be established in the same way; it is a purely *a priori* assumption. As to axiom (GR$_\text{IV}$), it can be considered as an "extrapolation" of a fact which can be verified by experiment for magnitudes which are not "too small".

Conversely:

#### Proposition 1 {#top-v-s2-prop-1 .statement}

Let E be a linearly ordered set with a smallest element ω; let I be a subset of E such that ω ∈ I and such that the relations x ∈ I, y ≤ x imply y ∈ I; let (x, y) → xy be a law of composition on E, defined for x ∈ I and y ∈ I. Then, if the axioms (GR_I), (GR_{II}), (GR_{III}) and (GR_{IV}) are satisfied, there exists a strictly increasing mapping f of I into the set R_+ of real numbers ≥ 0, such that

$$
f(xy) = f(x) + f(y)
$$

whenever x ∈ I, y ∈ I and xy ∈ I; moreover, the intersection of f(I) with every interval [0, f(b)] of R is dense in this interval, where b denotes any element of I.

Given any two elements x, y of I such that y ≠ ω, let us denote by (x : y) the largest integer n ≥ 0 such that y^n is defined and ≤ x (*); this integer exists by (GR_{IV}); if (x : y) = p, then y^{p+1} is defined and > x. If x ∈ I, y ∈ I and xy ∈ I, we have

(I)
$$
(x : z) + (y : z) \leq (xy : z) \leq (x : z) + (y : z) + 1.
$$

For let (x : z) = p, (y : z) = q; then we have z^p ≤ x, z^q ≤ y; since xy ∈ I, z^p z^q is defined and belongs to I, therefore z^{p+q} is defined and z^{p+q} = z^p z^q ≤ xy; moreover, if z^{p+q+2} is defined, we have z^{p+q+2} > xy because z^{p+1} > x and z^{q+1} > y.

Next we establish the inequalities

(2)
$$
\begin{cases}
(x : y) (y : z) \leq (x : z), \\
((x : y) + 1) ((y : z) + 1) \geq (x : z) + 1.
\end{cases}
$$

Let (x : y) = p and (y : z) = q; then y^p ≤ x and z^q ≤ y, so that (z^q)^p is defined and ≤ x; it belongs therefore to I; consequently z^{pq} is defined and we have z^{pq} = (z^q)^p ≤ x, from which the first inequality follows. On the other hand, if z^{(p+1)(q+1)} is defined, we have z^{(p+1)(q+1)} > x, because y^{p+1} > x and z^{q+1} > y; hence the second inequality.

Let $ \tilde{\mathcal{X}} $ denote the filter of sections of the ordered set of elements > ω in I, with respect to the relation ≥; the intervals ]ω, z[, where z runs through the set of all elements > ω, form a base of $ \tilde{\mathcal{X}} $. Given two elements a and x of I such that a > ω, we shall show that the ratio $ \frac{(x : z)}{(a : z)} $, which is defined for z ≤ a and is a rational number > 0,

(*) When E = I is the set of natural integers, the law of composition being addition, (x : y) is the integral part of x/y.

is a function of $ z $ which has a *limit* with respect to $ \mathfrak{F} $. This is obvious if $ x = \omega $, for then $ (x : z) = 0 $ for all $ z $. If $ x > \omega $, we shall show that the image $ \mathcal{G} $ of $ \mathfrak{F} $ under the mapping $ z \to \frac{(x : z)}{(a : z)} $ (restricted to the set of those $ z > \omega $ which are $ \leq x $ and $ \leq a $) is a Cauchy filter base for the uniform structure of the *multiplicative* group $ \mathbf{R}_+^* $, and therefore converges to a real number $ > 0 $. Note first that, $ u > \omega $ being given, $ (u : z) $ has limit $ +\infty $ with respect to $ \mathfrak{F} $: for there exists $ z > \omega $ such that $ z^{2^n} \leq u $, so that $ (u : z) \geq 2^n > n $. Now take a number $ \varepsilon > 0 $ arbitrarily; there exists $ t > \omega $ such that $ (x : t) \geq 1 / \varepsilon $ and $ (a : t) \geq 1 / \varepsilon $. Consider the double inequality

$$
\frac{(x : t)}{(a : t) + 1} \cdot \frac{(t : z)}{(t : z) + 1} \leq \frac{(x : z)}{(a : z)} \leq \frac{(x : t) + 1}{(a : t)} \cdot \frac{(t : z) + 1}{(t : z)},
$$

which follows immediately from the inequalities (2). There exists $ z_0 > \omega $ such that $ z \leq z_0 $ implies $ (t : z) \geq 1 / \varepsilon $, so that

$$
\frac{1}{(1 + \varepsilon)^2} \frac{(x : t)}{(a : t)} \leq \frac{(x : z)}{(a : z)} \leq (1 + \varepsilon)^2 \frac{(x : t)}{(a : t)},
$$

which shows that $ \mathcal{G} $ is a Cauchy filter base for the multiplicative uniformity.

Fix once and for all the element $ a > \omega $ (the "unit of measure") and for each $ x \in I $ put

$$
f(x) = \lim_{z \in \mathfrak{F}} \frac{(x : z)}{(a : z)}.
$$

From what has already been proved, we have $ f(\omega) = 0 $, $ f(x) > 0 $ for $ x > \omega $, and $ f(a) = 1 $. If we divide the inequality (1) throughout by $ (a : z) $ and pass to the limit with respect to $ \mathfrak{F} $, we see that

$$
f(xy) = f(x) + f(y)
$$

whenever $ x \in I, y \in I $ and $ xy \in I $. Likewise, the relation $ x \leq y $ implies $ (x : z) \leq (y : z) $, whence by dividing by $ (a : z) $ and passing to the limit we have $ f(x) \leq f(y) $, so that $ f $ is *increasing* on $ I $. We deduce that $ f $ is *strictly increasing* on $ I $; for if $ x < y $, there exists $ z > \omega $ such that $ xz \leq y $, whence $ f(xz) \leq f(y) $; and since $ xz \in I $,

$$
f(x) + f(z) = f(xz) \leq f(y);
$$

but $ f(z) > 0 $, so that indeed $ f(x) < f(y) $.

Finally, if $ b \in I $, the intersection of $ f(I) $ and the interval $[0, f(b)]$ of $ \mathbf{R} $ is dense in this interval. For if $ n $ is any integer $ > 0 $, there exists $ x > \omega $ such that $ f(x) \leq 2^{-n} $ (take $ x $ such that $ x^{2^n} \leq a $); if $ p $ is the smallest integer such that $ x^{p+1} > b $, we have $ (p+1)f(x) > f(b) $ and $ qf(x) \leq f(b) $ for $ 1 \leq q \leq p $; therefore every interval contained in $[0, f(b)]$ and of length $ > 2^{-n} $ contains at least one point of the form $ qf(x) = f(x^q) \in f(I) $. The proof of Proposition 1 is therefore complete.

#### Remark 1 {#top-v-s2-rem-1 .statement}

The relations $ x \in I, y \in I, xy \in I, yx \in I $ imply
$$
f(xy) = f(x) + f(y) = f(yx),
$$
and hence $ yx = xy $ since $ f $ is strictly increasing; in other words, the law induced by the law of composition of $ E $ on an interval $[0, b]$ suitably chosen (e.g., such that $ b^2 \leq a $) is *commutative*.

#### Remark 2 {#top-v-s2-rem-2 .statement}

Every mapping $ g $ of $ I $ into $ \mathbf{R}_+ $ which satisfies the same conditions as $ f $ is of the form $ x \to \lambda f(x) $ where $ \lambda > 0 $. For if $ \lambda = g(a) > 0 $, the relations $ z^p \leq x \leq z^{p+1}, z^q \leq a \leq z^{q+1} $ imply, by hypothesis,
$$
pg(z) \leq g(x) \leq (p+1)g(z), \qquad qg(z) \leq g(a) \leq (q+1)g(z),
$$
whence
$$
\lambda \frac{(x : z)}{(q : z) + 1} \leq g(x) \leq \lambda \frac{(x : z) + 1}{(q : z)},
$$
and therefore, passing to the limit with respect to $ \tilde{x} $, we have $ g(x) = \lambda f(x) $.

Let us seek conditions under which $ f(I) $ is an *interval* of $ \mathbf{R}_+ $. Clearly the following two conditions are necessary:

(GR_{IIIa}) *The set of elements $ > \omega $ in $ I $ is not empty and has no smallest element, and given any two elements $ x, y $, of $ I $ such that $ x < y $, there exists $ z \in I $ such that $ xz = y $* ("subtraction" of magnitudes).

(GR_{IVa}) *Every increasing sequence of elements of $ I $, which is bounded above by an element of $ I $ has a least upper bound in $ I $*.

We shall show that these conditions are also sufficient, and moreover that they allow us to dispense with axiom (GR_{IV}) (Archimedes' axiom). To be precise, we shall prove the following proposition:

#### Proposition 2 {#top-v-s2-prop-2 .statement}

*If a linearly ordered set $ E $ and a subset $ I $ of $ E $ satisfy the axioms (GR_I), (GR_{II}), (GR_{IIIa}) and (GR_{IVa}), there exists a strictly increasing mapping $ f $ of $ I $ onto an interval of $ \mathbf{R} $, with $ 0 $ as its left-hand end-point, such that $ f(\omega) = 0 $ and $ f(xy) = f(x) + f(y) $ whenever $ x, y $ and $ xy $ belong to $ I $.*

Let us first show that axiom (GR_{IV}) is satisfied. We argue by contradiction: suppose that there exist $ x, y \in I $ such that $ x > \omega $, $ x^n $ is defined and $ x^n \leq y $ for all integers $ n > 0 $. The increasing sequence $ (x^n) $ has a least upper bound $ b \in I $ by (GR$_{\text{IV}_a}$). Since $ x < b $, there exists $ c \in I $ such that $ xc = b $ by (GR$_{\text{III}_a}$), and we have $ c < b $ since $ x > \omega $. Now, for every $ n $, we have $ x^{n+1} \leq b = xc $, whence $ x^n \leq c $ by (GR$_{\text{II}}$) : the upper bound $ b $ of the $ x^n $ is therefore $ \leq c $, which is a contradiction.

We are therefore in a position to apply Proposition 1. It remains to show that, if $ \gamma = f(c) $ ($ c > \omega $) is any element of $ f(I) $, and if $ \beta $ is any real number such that $ 0 < \beta < \gamma $, there exists $ b \in I $ such that $ f(b) = \beta $ (Chapter IV, § 2, no. 4, Proposition 1). Since the intersection of $ f(I) $ and $[0, \gamma]$ is dense in $[0, \gamma]$, there exists an increasing sequence $(x_n)$ of elements of $ I $ such that $ f(x_n) $ has $ \beta $ as limit. Let $ b $ be the least upper bound of the sequence $(x_n)$ in $ I $; we have $ f(b) \geq f(x_n) $ for all $ n $, hence $ f(b) \geq \beta $; but $ f(b) > \beta $ is impossible, otherwise there would exist $ y \in I $ such that $ \beta < f(y) < f(b) $, and since $ \beta $ is the least upper bound of the sequence $(f(x_n))$, we should have $ f(x_n) < f(y) < f(b) $ for all $ n $, whence $ x_n < y < b $ for all $ n $, which is absurd. Hence $ f(b) = \beta $, and Proposition 2 is therefore proved.

#### Remark {#top-v-s2-n0-rem-3 .statement}

When $ I = E $, the image $ f(I) = f(E) $ is the whole of $ \mathbf{R}_+ $, for if $ b > \omega $, then $ b^n $ is defined for all $ n $, and therefore $ n \cdot f(b) $ belongs to $ f(E) $ for all $ n $; this implies that $ f(E) $ is not bounded above, because $ f(b) > 0 $.

### Exercises {#top-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
