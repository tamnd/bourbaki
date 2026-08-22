---
book: int
book_title: Integration
chapter: I
chapter_title: INEQUALITIES OF CONVEXITY
section: 0
section_title: INEQUALITIES OF CONVEXITY
kind: front
lang: en
source: int-i-vi
pdf_pages: 0016-0022
extraction: ocr
statements: 0
exercises: 0
content_sha256: e54d6fbe9e90c62a28ec6f6ba87e334e73d7ce4098ca837039ce5c3f52732531
---

## CHAPTER I

# Inequalities of convexity

1. The fundamental inequality of convexity

Let X be a set; in the vector space $ \mathbf{R}^X $ of all finite numerical functions$^1$ defined on X, let P be the set of all positive real-valued functions on X. On the other hand, let $ M $ be a numerical function,$^2$ finite or not, with values $ \geqslant 0 $, defined on P, such that:

$ 1^\circ $ $ M(0) = 0 $, and $ M $ is positively homogeneous, that is, $ M(\lambda f) = \lambda M(f) $ for every real number $ \lambda > 0 $.$^3$

$ 2^\circ $ $ M $ is increasing in P, in other words the relation $ f \leqslant g $ implies $ M(f) \leqslant M(g) $.

$ 3^\circ $ $ M $ is convex in P, in other words (TVS, II, §2, No. 8) satisfies the relation $ M(f + g) \leqslant M(f) + M(g) $.

*Example.* — Suppose X is a finite set, for example the interval $[1, n]$ of $ \mathbf{N} $; denoting by $ x_i $ ($ 1 \leqslant i \leqslant n $) the coordinates of a vector $ \mathbf{x} \in \mathbf{R}^n $, the functions
$$
M_1(\mathbf{x}) = \sum_{i=1}^n x_i \quad \text{and} \quad M_\infty(\mathbf{x}) = \sup_{1 \leqslant i \leqslant n} x_i
$$
satisfy the preceding conditions in the set P of vectors $ \mathbf{x} $ with coordinates $ \geqslant 0 $.

*Remark.* — Let S be a pointed convex cone contained in P (that is, a set such that $ S + S \subset S $ and $ \lambda S \subset S $ for $ \lambda \geqslant 0 $; cf. TVS, II, §2, No. 4); let $ M $ be a numerical function (finite or not) with values $ \geqslant 0 $, defined on S and satisfying in S the above conditions $ 1^\circ, 2^\circ $ and $ 3^\circ $. Then $ M $ can be extended to the entire set P, in such a way that the extended function (which we denote again by $ M $) satisfies the same conditions: it suffices, for every function $ f \in P $, to set $ M(f) = +\infty $ if there does not exist any function $ g \in S $ such that $ f \leqslant g $, and $ M(f) = \inf_{g \in S, f \leqslant g} M(g) $ in the contrary case. This procedure will be applied in Ch. IV, §1 to define the *upper integral* of a positive function.

\footnotetext{
$ ^1 $ Fonction numérique finie—a function with values in $ \mathbf{R} $—may also be translated as "real-valued function" (cf. GT, IV, §5, No. 1).
$ ^2 $ Fonction numérique—"numerical function"—signifies a function with values in $ \overline{\mathbf{R}} $ (TG, IV, §5, No. 1). The phrase "finite or not" is sometimes added as a reminder that the function may take on infinite values.
$ ^3 $ Recall that in $ \overline{\mathbf{R}} $, products such as $ 0 \cdot (+\infty) $ are not defined (GT, IV, §4, No. 3).
}

PROPOSITION 1. — Let $ \varphi(t_1, t_2, \ldots, t_n) $ be a finite numerical function, defined and continuous for $ t_i \geq 0 $ ($ 1 \leq i \leq n $), such that:
$ 1^\circ $ the relations $ t_i > 0 $ ($ 1 \leq i \leq n $) imply $ \varphi(t_1, t_2, \ldots, t_n) > 0 $;
$ 2^\circ $ the function $ \varphi $ is positively homogeneous;
$ 3^\circ $ the set $ K \subset \mathbf{R}^n $ defined by the relations $ t_i \geq 0 $ ($ 1 \leq i \leq n $), $ \varphi(t_1, t_2, \ldots, t_n) \geq 1 $ is convex.
Under these conditions, if $ f_1, f_2, \ldots, f_n $ are $ n $ finite functions $ \geq 0 $ defined on $ X $, such that $ M(f_i) < +\infty $ for $ 1 \leq i \leq n $, then

$$
M(\varphi(f_1, f_2, \ldots, f_n)) \leq \varphi(M(f_1), M(f_2), \ldots, M(f_n)).
$$

One knows, by the Hahn-Banach theorem (TVS, II, §5), that $ K $ is the intersection of the $ n $ half-spaces $ t_i \geq 0 $ ($ 1 \leq i \leq n $) and a family of closed half-spaces $ (U_\iota)_{\iota \in I} $, $ U_\iota $ being defined by a relation of the form

$$
\alpha_{\iota 1} t_1 + \alpha_{\iota 2} t_2 + \cdots + \alpha_{\iota n} t_n - \beta_\iota \geq 0,
$$

where the $ \alpha_{\iota k} $ are not all zero. By hypothesis, if $ t = (t_i) $ is such that $ t_i > 0 $ for $ 1 \leq i \leq n $, then $ \varphi(t_1, \ldots, t_n) > 0 $, therefore there exists a $ \lambda_0 > 0 $ such that the relation $ \lambda \geq \lambda_0 $ implies $ \lambda t \in K $; this shows that, for each $ \iota \in I $, the relations $ t_i \geq 0 $ ($ 1 \leq i \leq n $) imply $ \alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \geq 0 $ and therefore $ \alpha_{\iota k} \geq 0 $ for $ 1 \leq k \leq n $; it is then clear that $ K $ is also the intersection of the half-spaces $ t_i \geq 0 $ ($ 1 \leq i \leq n $) and the $ U_\iota $ such that $ \beta_\iota \geq 0 $; moreover, since the origin does not belong to $ K $, there exists at least one index $ \iota $ such that $ \beta_\iota > 0 $.

Now let $ C $ be the convex cone in $ \mathbf{R}^{n+1} $ defined by the relations $ t_i \geq 0 $ ($ 1 \leq i \leq n+1 $), $ t_{n+1} \leq \varphi(t_1, t_2, \ldots, t_n) $ (the closure of the convex cone generated in $ \mathbf{R}^{n+1} $ by the convex set $ K \times \{1\} $); it is immediate that $ C $ is also defined by the relations $ t_i \geq 0 $ ($ 1 \leq i \leq n+1 $) and

$$
\beta_\iota t_{n+1} \leq \alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \quad (\iota \in I, \ \beta_\iota \geq 0).
$$

For every $ x \in X $, we therefore have

$$
\beta_\iota \varphi(f_1(x), \ldots, f_n(x)) \leq \alpha_{\iota 1} f_1(x) + \cdots + \alpha_{\iota n} f_n(x)
$$

for all $ \iota \in I $. For every index $ \iota $ such that $ \beta_\iota > 0 $, it follows from (4) and the hypotheses on $ M $ that $ M(\varphi(f_1, f_2, \ldots, f_n)) $ is finite and

$$
\beta_\iota M(\varphi(f_1, f_2, \ldots, f_n)) \leq \alpha_{\iota 1} M(f_1) + \alpha_{\iota 2} M(f_2) + \cdots + \alpha_{\iota n} M(f_n),
$$

and this relation is also verified in an obvious manner if $ \beta_\iota = 0 $. We thus see that the point with coordinates

$$
M(f_1), M(f_2), \ldots, M(f_n), \quad M(\varphi(f_1, f_2, \ldots, f_n))
$$

belongs to $ C $, which proves the proposition.

2. The inequalities of Hölder and Minkowski

In this No. and in the following one, $ X $ and $ P $ have the same meaning as in No. 1, and $ M $ denotes a function defined on $ P $ that satisfies the conditions listed in No. 1.

PROPOSITION 2. — *Let $ \alpha $ and $ \beta $ be two numbers such that $ 0 < \alpha < 1 $, $ 0 < \beta < 1 $, $ \alpha + \beta = 1 $. If $ f $ and $ g $ are two finite functions $ \geq 0 $ defined on $ X $, and if $ M(f) $ and $ M(g) $ are finite, then*

$$
M(f^\alpha g^\beta) \leq (M(f))^\alpha (M(g))^\beta
$$

(*Hölder’s inequality*).

By Prop. 1, it all comes down to proving that, in $ \mathbf{R}^2 $, the set defined by the relations $ t_1 \geq 0 $, $ t_2 \geq 0 $, $ t_1^\alpha t_2^\beta \geq 1 $ is convex, or again (FRV, I, §4, No. 1, Def. 1) that the function $ u(t) = t^{-\alpha/\beta} $ is convex for $ 0 < t < +\infty $. Now, setting $ r = \alpha/\beta $, we have $ D^2 u(t) = r(r+1)t^{-r-2} $ and, since $ r > 0 $, $ D^2 u(t) > 0 $ on $ ]0, +\infty[ $, which proves the proposition (FRV, I, §4, No. 4, Cor. of Prop. 8).

COROLLARY. — *Let $ \alpha_i $ ($ 1 \leq i \leq n $) be $ n $ numbers $ \geq 0 $ such that*
$$
\sum_{i=1}^n \alpha_i = 1,
$$
*and let $ f_i $ ($ 1 \leq i \leq n $) be $ n $ functions $ \geq 0 $ defined on $ X $, such that $ M(f_i) $ is finite for $ 1 \leq i \leq n $. Under these conditions,*

$$
M(f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}) \leq (M(f_1))^{\alpha_1} (M(f_2))^{\alpha_2} \cdots (M(f_n))^{\alpha_n}.
$$

We can restrict attention to the case that $ \alpha_i > 0 $ for every $ i $. It suffices to argue by induction on $ n $, by applying the inequality (5) to the numbers $ \alpha = \alpha_1 $ and $ \beta = \sum_{i=2}^n \alpha_i $, and to the functions $ f = f_1 $, $ g = (f_2^{\alpha_2} f_3^{\alpha_3} \cdots f_n^{\alpha_n})^{1/\beta} $.

PROPOSITION 3. — *Let $ p $ be a real number $ \geq 1 $. If $ f $ and $ g $ are two finite functions $ \geq 0 $ defined on $ X $, then*

$$
\left( M((f+g)^p) \right)^{1/p} \leq \left( M(f^p) \right)^{1/p} + \left( M(g^p) \right)^{1/p}
$$

(*Minkowski’s inequality*).

We can restrict attention to the case that $ M(f^p) $ and $ M(g^p) $ are finite. By Prop. 1, we are reduced to proving that the set in $ \mathbf{R}^2 $ defined by the relations $ t_1 \geq 0,\ t_2 \geq 0,\ t_1^{1/p} + t_2^{1/p} \geq 1 $ is convex, or again that the function $ u(t) = (1 - t^{1/p})^p $ is convex for $ 0 \leq t \leq 1 $. Now,

$$
D^2 u(t) = \left(1 - \frac{1}{p}\right)t^{1/p-2}(1-t^{1/p})^{p-2} \geq 0
$$

for $ 0 < t \leq 1 $, whence the proposition.

3. The semi-norms $ N_p $

Let $ p $ be a real number $ \geq 1 $ and let $ \mathcal{F}^p(X, M) $ be the set of finite numerical functions $ f $ defined on $ X $ such that $ M(|f|^p) $ is *finite*. It is obvious that if $ g $ is a function belonging to $ \mathcal{F}^p(X, M) $ and if $ |f| \leq |g| $, then $ f $ also belongs to $ \mathcal{F}^p(X, M) $; this remark and Minkowski’s inequality show that the sum of two functions in $ \mathcal{F}^p(X, M) $ also belongs to this set; taking into account the fact that $ M $ is positively homogeneous, we thus see that $ \mathcal{F}^p(X, M) $ is a *linear subspace* of the space $ \mathbf{R}^X $ of all finite numerical functions defined on $ X $.

For every number $ p > 0 $ and every finite numerical function $ f $ defined on $ X $, set

$$
N_p(f) = \left(M(|f|^p)\right)^{1/p};
$$

then $ N_p(\lambda f) = |\lambda| N_p(f) $ for every scalar $ \lambda $; moreover, if $ p \geq 1 $ then, by (7),

$$
N_p(f+g) \leq N_p(f) + N_p(g),
$$

which proves that $ N_p $ is a *semi-norm* on the vector space $ \mathcal{F}^p(X, M) $ (TVS, II, §1).

**Proposition 4.** — *Let $ p $ and $ q $ be two real numbers $ > 0 $ and set $ 1/r = 1/p + 1/q $. For any finite numerical functions $ f, g $ defined on $ X $,*

$$
N_r(fg) \leq N_p(f) N_q(g)
$$

*provided that $ N_p(f) $ and $ N_q(g) $ are finite.*

For, the relation (9) may be written

$$
M(|f|^r |g|^r) \leq (M(|f|^p))^{r/p} (M(|g|^q))^{r/q},
$$

which is none other than Hölder’s inequality (5) applied to the numbers $ \alpha = r/p $ and $ \beta = r/q $ and to the functions $ |f|^p $ and $ |g|^q $.

COROLLARY. — *Suppose that* $ M(1) = 1 $; *then, for every finite numerical function* $ f $ *defined on* $ X $, *the mapping* $ p \mapsto N_p(f) $ *is increasing in* $ ]0, +\infty[ $.

Applying the inequality (9) to the case that $ g = 1 $, we see that $ N_r(f) \leq N_p(f) $ for all $ q > 0 $; since the number $ r $ defined by $ 1/r = 1/p + 1/q $ runs over the set of numbers such that $ 0 < r < p $ when $ q $ runs over the set of numbers $ > 0 $, the corollary is proved.

PROPOSITION 5. — *For every finite numerical function* $ f $ *defined on* $ X $, *the set* $ I $ *of values of* $ 1/p $ ($ p > 0 $) *such that* $ N_p(f) $ *is finite is either empty or is an interval; if* $ I $ *is not reduced to a point, then the mapping* $ \alpha \mapsto \log N_{1/\alpha}(f) $ *is either convex on* $ I $ *or is equal to* $ -\infty $ *on the interior of* $ I $.

Let $ r $ and $ s $ be two distinct numbers $ > 0 $ such that $ 1/r $ and $ 1/s $ belong to $ I $; it all comes down to proving that if

$$
\frac{1}{p} = \frac{t}{r} + \frac{1-t}{s},
$$

with $ 0 < t < 1 $, then

$$
\log N_p(f) \leq t \cdot \log N_r(f) + (1-t) \log N_s(f),
$$

or, what comes to the same,

$$
N_p(f) \leq (N_r(f))^t (N_s(f))^{1-t},
$$

a relation that may, by the definition of $ N_p $, be written

$$
M(|f|^p) \leq (M(|f|^r))^{tp/r} (M(|f|^s))^{(1-t)p/s}.
$$

Setting $ \alpha = tp/r $, we have $ 1-\alpha = (1-t)p/s $ by the relation that defines $ p $ as a function of $ t, r, s $; whence $ p = \alpha r + (1-\alpha)s $. Hölder’s inequality now yields

$$
M(|f|^{r\alpha}|f|^{s(1-\alpha)}) \leq (M(|f|^r))^{\alpha} (M(|f|^s))^{1-\alpha},
$$

which is none other than the inequality (12).

Exercises

1) With the hypotheses of No. 1, show that the set of bounded functions on X such that $ M(|f|) $ is finite is a subalgebra A of $ \mathbf{R}^X $, and that the set of bounded functions on X such that $ M(|f|) = 0 $ is an ideal in A. If, moreover, $ M(1) $ is finite, show that the mapping $ f \mapsto M(f) $ is continuous when A is equipped with the topology of uniform convergence in X.

2) Let X be the interval $[0, +\infty[$ of $ \mathbf{R} $, S the convex cone formed by the functions defined on X such that $ 0 \leq f(x) \leq kx $ on X (for a finite number $ k > 0 $ depending on $ f $). Set $ M(f) = 0 $ for $ f \in S $, and $ M(f) = +\infty $ for every positive function $ f $ defined on X and not belonging to S. Show that $ M $ satisfies the conditions of No. 1, and that $ M(x) = 0 $, and $ M(x^r) = +\infty $ for every number $ r > 0 $ not equal to 1.

3) Give an example where X is a set with two elements, $ N_p(\mathbf{x}) $ is finite for every $ p > 0 $ and every $ \mathbf{x} \in \mathbf{R}^2 $, but where there exist values of $ p $ such that the mapping $ p \mapsto N_p(\mathbf{x}) $ is not differentiable at these points.

4) Deduce the inequality (6) from the inequality of the geometric mean

$$
z_1^{\alpha_1} z_2^{\alpha_2} \cdots z_n^{\alpha_n} \leq \alpha_1 z_1 + \cdots + \alpha_n z_n \quad \text{(where } \sum_{i=1}^n \alpha_i = 1 \text{)}
$$

(FRV, III, §1, No. 1, Prop. 2). (Reduce to the case that $ M(f_i) = 1 $ for $ 1 \leq i \leq n $.)

5) Let $ \alpha $ be a real number $ > 1 $ and let $ \beta = 1 - \alpha < 0 $. Let $ g $ be a finite function, defined on X, such that $ g(x) > 0 $ for all $ x \in X $ and such that $ M(g) > 0 $; show that for every finite function $ f \geq 0 $ defined on X such that $ M(f) $ is finite,

$$
M(f^\alpha g^\beta) \geq (M(f))^\alpha (M(g))^\beta
$$

(apply Hölder’s inequality suitably).

6) Deduce Minkowski’s inequality from Hölder’s inequality (find an upper bound for $ M((f+g)^{p-1}) $ with the help of Hölder’s inequality). If one assumes that $ M(f+g) = M(f) + M(g) $ for every pair of functions $ f, g $ defined and $ \geq 0 $ on $ X $, deduce similarly from Exer. 5 the inequality

$$
(M((f+g)^p))^{1/p} \geq (M(f^p))^{1/p} + (M(g^p))^{1/p}
$$

in the following cases:

a) $ 0 < p < 1 $, $ f $ and $ g $ finite functions $ \geq 0 $ defined on $ X $, such that $ f(x) + g(x) > 0 $ for all $ x \in X $ and such that $ M(f^p) $ and $ M(g^p) $ are finite;

b) $ p < 0 $, $ f $ and $ g $ finite functions defined on $ X $, such that $ f(x) > 0 $ and $ g(x) > 0 $ for all $ x \in X $, $ M(f^p) $ and $ M(g^p) $ are finite, and $ M((f+g)^p) > 0 $.
