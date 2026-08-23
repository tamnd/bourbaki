---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: DIFFERENTIAL EQUATIONS
section: 1
section_title: EXISTENCE THEOREMS
lang: en
source: fvr-i-vii
pdf_pages: 0178-0192, 0214-0219
extraction: ocr
subsections:
    - "no": 1
      title: THE CONCEPT OF A DIFFERENTIAL EQUATION
      page: 0
      pdf_page: 178
    - "no": 2
      title: DIFFERENTIAL EQUATIONS ADMITTING SOLUTIONS THAT ARE PRIMITIVES OF REGULATED FUNCTIONS
      page: 0
      pdf_page: 179
    - "no": 3
      title: EXISTENCE OF APPROXIMATE SOLUTIONS
      page: 0
      pdf_page: 181
    - "no": 4
      title: COMPARISON OF APPROXIMATE SOLUTIONS
      page: 0
      pdf_page: 183
    - "no": 5
      title: EXISTENCE AND UNIQUENESS OF SOLUTIONS OF LIPSCHITZ AND LOCALLY LIPSCHITZ EQUATIONS
      page: 0
      pdf_page: 186
    - "no": 6
      title: CONTINUITY OF INTEGRALS AS FUNCTIONS OF A PARAMETER
      page: 0
      pdf_page: 189
    - "no": 7
      title: DEPENDENCE ON INITIAL CONDITIONS
      page: 0
      pdf_page: 191
statements: 29
exercises: 18
content_sha256: 2a0ebfd7467ee48420642d2462fb0e4209b34c54a99b6fdf811e56e594cacd20
---

## § 1. EXISTENCE THEOREMS

### 1. THE CONCEPT OF A DIFFERENTIAL EQUATION

Let I be an interval contained in $ \mathbf{R} $, not reducing to a single point, E a *topological vector space* over $ \mathbf{R} $, and A and B two open subsets of E. Let $ (x, y, t) \mapsto g(x, y, t) $ be a continuous map of $ A \times B \times I $ into E; to every *differentiable* map u of I into A whose derivative takes its values in B we associate the map $ t \mapsto g(u(t), u'(t), t) $ of I into E, and denote it by $ \tilde{g}(u) $; so $ \tilde{g} $ is defined on the set $ \mathcal{D}(A, B) $ of differentiable functions of I into B whose derivatives have their values in B. We shall say that the equation $ \tilde{g}(u) = 0 $ is a *differential equation* in u (relative to the *real* variable t); a *solution* of this equation is also called an *integral* of the differential equation (on the interval I); it is a differentiable map of I into A, whose derivative takes values in B, such that $ g(u(t), u'(t), t) = 0 $ for *every* $ t \in I $. By abuse of language we shall write the differential equation $ \tilde{g}(u) = 0 $ in the form

$$
g(x, x', t) = 0,
$$

on the understanding that x belongs to the set $ \mathcal{D}(A, B) $.

For example, for $ I = E = \mathbf{R} $ the relations

$$
x' = 2t, \qquad tx' - 2x = 0, \qquad x'^2 - 4x = 0, \qquad x - t^2 = 0
$$

are differential equations, all four of which admit the function $ x(t) = t^2 $ as a solution

In this chapter we consider in principle only the case where E is a *complete normed space* over $ \mathbf{R} $, and where the differential equations are of the specific form

$$
x' = f(t, x)
$$

("explicit equations in $ x' $"), where f denotes a function defined on $ I \times H $ with values in E, and H is an *open* nonempty subset of E. We shall, moreover, widen a little the concept of a *solution* (or *integral*) of such an equation (on the interval I): we shall say that a function u, defined and continuous on I, with values in H, is a solution (or integral) of the equation (I) if there exists a *countable* subset A of I such that at every point t of the complement of A in I the function u admits a derivative $ u'(t) $ such that $ u'(t) = f(t, u(t)) $. If $ u $ is differentiable and satisfies the relation above for every point $ t \in I $ we shall say that it is a strict solution of the equation (1) on I.

In the particular case of a differential equation of the form $ x' = f(t) $, where $ f $ is a map of I into E, the solutions in the above sense are the primitives of the function $ f $ (II, p. 51), and the strict solutions are the strict primitives.

When E is a product of complete normed spaces $ E_i $ ($ 1 \leq i \leq n $), one can write $ x = (x_i)_{1 \leq i \leq n} $ and $ f = (f_i)_{1 \leq i \leq n} $, where $ x_i $ is a map from I into $ E_i $ and $ f_i $ is a map from $ I \times H $ into $ E_i $; the equation (1) is then equivalent to the system of differential equations
$$
x'_i = f_i(t, x_1, x_2, \ldots, x_n) \qquad (1 \leq i \leq n).
$$
(2)

The most important case is that where the $ E_i $ are equal to $ \mathbf{R} $ or to $ \mathbf{C} $; one then says that (2) is a system of scalar differential equations.

One may reduce the study of relations of the form
$$
x^{(n)} = f(t, x, x', \ldots, x^{(n-1)})
$$
to that of the system (2), where $ x $ is an $ n $ times differentiable vector function on I; for on putting $ x_1 = x $, and $ x_p = x^{(p-1)} $ for $ 2 \leq p \leq n $, the relation (3) is equivalent to the system
$$
\begin{cases}
x'_i = x_{i+1} & (1 \leq i \leq n-1) \\
x'_n = f(t, x_1, x_2, \ldots, x_n).
\end{cases}
$$
(4)

A relation of the form (3) is called a differential equation of order $ n $ (explicitly resolved for $ x^{(n)} $); in contrast, equations of the form (1) are called differential equations of first order.

Similarly one may reduce any "system of differential equations" of the form
$$
D^{n_i} x_i = f_i(t, x_1, Dx_1, \ldots, D^{n_1} x_1, \ldots, x_p, Dx_p, \ldots, D^{n_p-1} x_p)
$$
$(1 \leq i \leq p)$ to a system of the form (2), where $ x_i $ is function on I which is $ n_i $ times differentiable on I (for $ 1 \leq i \leq p $).

### 2. DIFFERENTIAL EQUATIONS ADMITTING SOLUTIONS THAT ARE PRIMITIVES OF REGULATED FUNCTIONS

Recall (II, p. 54, def. 3) that a vector function $ u $ defined on an interval $ I \subset \mathbf{R} $ is said to be regulated if it is the uniform limit of step functions on every compact subset of I; an equivalent condition is that at every interior point of I the function $ u $ has a right and a left limit, and also a right limit at the left-hand end point of I and a left limit at the right-hand endpoint of I, when these two points belong to I (II, p. 54, th. 3). In this chapter we shall restrict ourselves to differential equations (1) for which every solution is a primitive of a regulated function on I. This condition is clearly satisfied if, for every continuous map $ u $ of I into H, the function $ f(t, u(t)) $ is regulated on I; the following lemma gives a sufficient condition for this:

#### Lemma 1 {#fvr-iv-s1-lem-1 .statement}

Let $ f $ be a map from $ I \times H $ into $ E $ such that, on writing $ f_x $ (for every $ x \in H $) for the map $ t \mapsto f(t, x) $ of $ I $ into $ E $, the following conditions are satisfied: 1° $ f_x $ is regulated on $ I $ for every $ x \in H $; 2° the map $ x \mapsto f_x $ of $ H $ into the set $ \mathcal{F}(I, E) $ of maps from $ I $ into $ E $ is continuous when one endows $ \mathcal{F}(I, E) $ with the topology of compact convergence (Gen. Top., X, p. 278). Under these conditions:

1° For every continuous map $ u $ of $ I $ into $ H $ the function $ t \mapsto f(t, u(t)) $ is regulated on $ I $; more precisely, the right (resp. left) limit of this function at a point $ t_0 \in I $ is equal to the right (resp. left) limit of the function $ t \mapsto f(t, u(t_0)) $ at the point $ t_0 $.

2° If $ (u_n) $ is a sequence of maps of $ I $ into $ H $ which converges uniformly to a continuous function $ u $ of $ I $ into $ H $ on every compact subset of $ I $, then the sequence of functions $ t \mapsto f(t, u_n(t)) $ converges uniformly to $ f(t, u(t)) $ on every compact subset of $ I $.

1 Let $ c $ be the right limit of $ f(t, u(t_0)) $ at the point $ t_0 $; for every $ \varepsilon > 0 $ there is a compact neighbourhood $ V $ of $ t_0 $ in $ I $ such that $ \|f(t, u(t_0)) - c\| \leq \varepsilon $ for $ t \in V $ and $ t > t_0 $. On the other hand, there exists $ \delta > 0 $ such that the relations

$$
x \in H, \quad \|x - u(t_0)\| \leq \delta
$$

imply $ \|f(s, x) - f(s, u(t_0))\| \leq \varepsilon $ for all $ s \in V $; if $ W \subset V $ is a neighbourhood of $ t_0 $ in $ I $ such that $ \|u(t) - u(t_0)\| \leq \delta $ for every $ t \in W $, then $ \|f(t, u(t)) - c\| \leq 2\varepsilon $ for $ t \in W $ and $ t > t_0 $, which proves that $ c $ is the right limit of $ f(t, u(t)) $ at the point $ t_0 $.

2 Let $ K $ be a compact subset of $ I $; since $ u $ is continuous on $ I $, $ u(K) $ is a compact subset of $ H $; for every $ \varepsilon > 0 $ and $ x \in u(K) $ there exists a number $ \delta_x $ such that, for every $ y \in H, \|y - x\| \leq \delta_x $ and every $ t \in K $, one has $ \|f(t, y) - f(t, x)\| \leq \varepsilon $. There is a finite number of points $ x_i \in u(K) $ such that the closed balls with centre $ x_i $ and radius $ \frac{1}{2}\delta_{x_i} $ form a cover of $ u(K) $; let $ \delta = \operatorname{Min}(\delta_{x_i}) $. By hypothesis there exists an integer $ n_0 $ such that for $ n \geq n_0 $ one has $ \|u_n(t) - u(t)\| \leq \frac{1}{2}\delta $ for every $ t \in K $. Now, for every $ t \in K $ there exists an index $ i $ such that

$$
\|u(t) - x_i\| \leq \frac{1}{2}\delta_{x_i};
$$

consequently one has $ \|u_n(t) - x_i\| \leq \delta_x $, whence $ \|f(t, u_n(t)) - f(t, u(t))\| \leq 2\varepsilon $ for every $ t \in K $ and every $ n \geq n_0 $

For the rest of this section I will denote an interval contained in $ \mathbf{R} $, not reducing to a single point, $ H $ an open nonempty set contained in the normed space $ E $, and $ f $ a map from $ I \times H $ into $ E $ satisfying the hypotheses of lemma 1.

#### Proposition 1 {#fvr-iv-s1-prop-1 .statement}

Let $ t_0 $ be a point of $ I $ and $ x_0 $ a point of $ H $; for a continuous function $ u $ to be a solution of the equation (1) on $ I $ and take the value $ x_0 $ at the point $ t_0 $, it is necessary and sufficient that it satisfies the relation

$$
u(t) = x_0 + \int_{t_0}^t f(s, u(s))\, ds
$$

for every $ t \in I $.

Indeed, by lemma 1, if $ u $ is a solution of (1) on $ I $, then $ f(t, u(t)) $ is regulated, so the right-hand side of (6) is defined and equal to $ u(t) $ for every $ t \in I $. Conversely, if $ u $ is a continuous function that satisfies (6) then $ f(t, u(t)) $ is regulated, by lemma 1, so $ u $ has derivative equal to $ f(t, u(t)) $ except at the points of a countable subset of $ I $.

#### Corollary {#fvr-iv-s1-n2-cor-1 .statement}

*At every point of I distinct from the left (resp. right) endpoint of this interval, every solution u of (1) on I admits a left (resp. right) derivative equal to the left (right) limit of $ f(t, u(t)) $ at this point.*

#### Proposition 2 {#fvr-iv-s1-prop-2 .statement}

*If f is a continuous map from $ I \times H $ into E, then every solution of (1) on I is a strict solution.*

Indeed, such a solution $ u $ is a primitive of the continuous function $ f(t, u(t)) $ (II, p. 66, prop. 3).

Furthermore, we note that a continuous function $ f $ on $ I \times H $ satisfies the conditions of lemma 1 (*Gen. Top.*, X, p. 286, cor. 3).

In the sequel we shall choose $ t_0 \in I $ and $ x_0 \in H $ arbitrarily and investigate whether there exist solutions of (1) on $ I $ (or on a neighbourhood of $ t_0 $ in $ I $) taking the value $ x_0 $ at the point $ t_0 $ (or, what comes to the same, solutions of (6)).

### 3. EXISTENCE OF APPROXIMATE SOLUTIONS

Given a number $ \varepsilon > 0 $ we shall say that a continuous map $ u $ of $ I $ into $ H $ is an *approximate solution to within* $ \varepsilon $ of the differential equation

$$
x' = f(t, x)
$$

if, at all the points of the complement of a *countable* subset of $ I $, the function $ u $ admits a derivative which satisfies the condition

$$
\|u'(t) - f(t, u(t))\| \leq \varepsilon.
$$

Let $ (t_0, x_0) $ be a point of $ I \times H $; since $ f $ satisfies the hypotheses of lemma 1 (IV, p. 165) there exist a compact neighbourhood $ J $ of $ t_0 $ in $ I $ such that $ f(t, x_0) $ is bounded on $ J $, and an open ball $ S $ with centre $ x_0 $ contained in $ H $, such that $ f(t, x) - f(t, x_0) $ is bounded on $ J \times S $; it follows that $ f(t, x) $ is *bounded* on $ J \times S $. *Throughout this subsection J will denote a compact interval which is a neighbourhood of t_0 in I, S will be an open ball with centre x_0 and radius r contained in H, with J and S such that f is bounded on J × S; and M will denote the supremum of \|f(t, x)\| over J × S.*

#### Proposition 3 {#fvr-iv-s1-prop-3 .statement}

*On every compact interval with left (or right) endpoint t_0 contained in J, with length less than r/(M + ε), there exists an approximate solution to within ε of equation (1), with values in S, and equal to x_0 at t_0.*

We suppose that $ t_0 $ is not the right-hand endpoint of J, and prove the proposition for intervals with left-hand endpoint $ t_0 $. Let $ \mathcal{M} $ be the set of solutions of (1) to within $ \varepsilon $, each of which takes values in S, is equal to $ x_0 $ at $ t_0 $, and is defined on a half open interval $[t_0, b[$ contained in J (the interval depending on the approximate solution under consideration). First we show that $ \mathcal{M} $ is not empty. Let c be right limit of $ f(t, x_0) $ at $ t_0 $; by lemma 1 (IV, p. 165) the function $ f(t, x_0 + c(t - t_0)) $ has a right limit equal to c at $ t_0 $, so the restriction of the function $ x_0 + c(t - t_0) $ to a sufficiently small half open interval $[t_0, b[$ will belong to $ \mathcal{M} $.

We order the set $ \mathcal{M} $ by the relation "u is a restriction of v", and show that $ \mathcal{M} $ is inductive (Set Theory, III, p. 154). Let $ (u_\alpha) $ be a totally ordered subset of $ \mathcal{M} $ and $[t_0, b_\alpha[$ the interval where $ u_\alpha $ is defined: for $ b_\alpha \leq b_\beta $ the function $ u_\beta $ is thus an extension of $ u_\alpha $. The union of the intervals $[t_0, b_\alpha[$ is an interval $[t_0, b[$ contained in J, and there exists one and only one function u defined on $[t_0, b[$ that coincides with $ u_\alpha $ on $[t_0, b_\alpha[$ for each $ \alpha $; among the $ b_\alpha $ there is an increasing sequence $ (b_{\alpha_n}) $ tending to b; since u agrees with $ u_{\alpha_n} $ on $[t_0, b_{\alpha_n}[$ the function u admits a derivative satisfying (7) at all the points of the complement of a countable subset of $[t_0, b[$, and so is the supremum of the set $ (u_\alpha) $ in $ \mathcal{M} $.

By Zorn's lemma (Set Theory, III, p. 154, th. 2), $ \mathcal{M} $ admits a maximal element $ u_0 $; we shall show that if $[t_0, t_1[$ is the interval where $ u_0 $ is defined, then either $ t_1 $ is the right-hand endpoint of J, or else $ t_1 - t_0 \geq r/(M + \varepsilon) $. We argue by contradiction, supposing that neither of these conditions holds; first we show that one can extend $ u_0 $ by continuity at the point $ t_1 $; in fact, for any s and t in $[t_0, t_1[$,

$$
\|u_0(s) - u_0(t)\| \leq (M + \varepsilon)|s - t|
$$

by the mean value theorem; Cauchy's criterion shows that $ u_0 $ admits a left limit $ x_1 \in S $ at the point $ t_1 $. Now let $ c_1 $ be the right limit at $ t_1 $ of the function $ f(t, x_1) $; one has $ \|c_1\| \leq M $; the same argument as that at the beginning of the proof shows that one can extend $ u_0 $ to a half open interval with left-hand endpoint $ t_1 $ by the function $ x_1 + c_1(t - t_1) $, so that the extended function belongs to $ \mathcal{M} $, which is absurd. This proves the proposition.

When f is uniformly continuous on $ J \times S $ one can prove prop. 3 without using Zorn's lemma (IV, p. 199, exerc. 1a)).

#### Proposition 4 {#fvr-iv-s1-prop-4 .statement}

*The set of approximate solutions of (1) to within $ \varepsilon $, defined on the same interval $ K \subset J $ and taking values in S, is uniformly equicontinuous.*

Indeed, if u is any function in this set and s and t are two points of K, then by the mean value theorem

$$
\|u(s) - u(t)\| \leq (M + \varepsilon)|s - t|.
$$

#### Corollary (Peano's theorem) {#fvr-iv-s1-n3-cor-1 .statement}

*If E is of finite dimension over $ \mathbf{R} $ then there exists a solution of (1) with values in S and equal to $ x_0 $ at $ t_0 $, on every compact interval K with left (or right) endpoint $ t_0 $ contained in J and having length $ < r/M $.*

Indeed, by prop. 3, once $ n $ is large enough there is an approximate solution $ u_n $ of (1) to within $ 1/n $, defined on $ K $, with values in $ S $, and equal to $ x_0 $ at $ t_0 $. Further, from some value of $ n $ on, $ u_n(K) $ is contained in a *closed* ball with centre $ x_0 $ and radius $ < r $, independent of $ n $. The set of $ u_n $ is equicontinuous (prop. 4), and since $ E $ is finite dimensional the set $ S $ is relatively compact in $ E $; so for every $ t \in K $ the set of $ u_n(t) $ is relatively compact in $ E $. By Ascoli’s theorem (*Gen. Top.*, X, p. 290, th. 2) the set of $ u_n $ is relatively compact in the space $ \mathcal{F}(K; E) $ of maps from $ K $ into $ E $ endowed with the uniform norm. Thus there is a sequence extracted from $ (u_{n_k}) $ of $ (u_n) $ which converges uniformly on $ K $ to a continuous function $ u $. One has $ u(K) \subset S $, so $ t \mapsto f(t, u(t)) $ is defined on $ K $; by lemma 1 (IV, p. 165), $ f(t, u_{n_k}(t)) $ converges uniformly to $ f(t, u(t)) $ on $ K $; by (IV, p. 4, formula (7)), $ u_{n_k} $ is a primitive of a function which tends uniformly to $ f(t, u(t)) $ on $ K $, so (II, p. 52, th. 1) $ u $ is a solution of (1) on $ K $, and equal to $ x_0 $ at the point $ t_0 $.

#### Remark 1 {#fvr-iv-s1-n3-rem-1 .statement}

There can be *infinitely many* integrals of a differential equation (1) taking the same value at a given point. For example, the scalar differential equation $ x' = 2\sqrt{|x|} $ has all the functions defined by

$$
\begin{array}{ll}
u(t) = 0 & \text{for } -\beta \leq t \leq \alpha \\
u(t) = -(t + \beta)^2 & \text{for } t \leq -\beta \\
u(t) = (t - \alpha)^2 & \text{for } t \geq \alpha
\end{array}
$$

as integrals taking the value 0 at the point $ t = 0 $, for any positive numbers $ \alpha $ and $ \beta $.

#### Remark 2 {#fvr-iv-s1-n3-rem-2 .statement}

Peano’s theorem no longer holds when $ E $ is an arbitrary complete normed space of *infinite* dimension (IV, p. 204, exerc. 18).

### 4. COMPARISON OF APPROXIMATE SOLUTIONS

In what follows, I and $ H $ denote, as above, an interval contained in $ \mathbf{R} $ and an open set in the normed space $ E $, respectively; $ t_0 $ is a point of I.

#### Definition 1 {#fvr-iv-s1-def-1 .statement}

*Given a positive real function* $ t \mapsto k(t) $ *defined on* $ I $, *one says that a map* $ f $ *from* $ I \times H $ *into* $ E $ *is Lipschitz with respect to the function* $ k(t) $ *if, for every* $ x \in H $, *the function* $ t \mapsto f(t, x) $ *is regulated on* $ I $, *and if, for every* $ t \in I $ *and every pair of points* $ x_1, x_2 $ *of* $ H $, *one has (the "Lipschitz condition")*

$$
\| f(t, x_1) - f(t, x_2) \| \leq k(t) \| x_1 - x_2 \|.
$$

(8)

We shall say that $ f $ is *Lipschitz* (without being more specific) on $ I \times H $ if it is Lipschitz on this set for some *constant* $ k \geq 0 $. It is immediate that a Lipschitz function on $ I \times H $ satisfies the hypotheses of lemma 1 of IV, p. 165 (the converse being false); when $ f $ is Lipschitz (on $ I \times H $) one says that the differential equation

$$
x' = f(t, x)
$$

(1)

is *Lipschitz* (on $ I \times H $).

#### Example {#fvr-iv-s1-n4-exa-1 .statement}

When $ E = \mathbf{R} $ and $ H $ is an interval in $ \mathbf{R} $, if the function $ f(t, x) $ admits a *partial derivative* $ f'_x $ (II, p. 74) at every point $ (t, x) $ of $ I \times H $, such that $ |f'_x(t, x)| \leq k(t) $ on $ I \times H $, then condition (8) is satisfied, by the mean value theorem; we shall see later how this example generalizes to the case where $ E $ is an arbitrary normed space.

If $ f $ is Lipschitz on $ I \times H $ then $ f $ is *bounded* on $ J \times S $ for every compact subinterval $ J \subset I $ and every open ball $ S \subset H $. Thus prop. 3 (IV, p. 166) can be applied, and demonstrates the existence of approximate solutions of equation (1). But we also have the following proposition, which allows us to *compare* two approximate solutions:

#### Proposition 5 {#fvr-iv-s1-prop-5 .statement}

*Let $ k(t) $ be a real regulated function and $ > 0 $ on $ I $, and let $ f(t, x) $ be a function that is defined and Lipschitz with respect to $ k(t) $ on $ I \times H $. If $ u $ and $ v $ are two approximate solutions of (1), to within $ \varepsilon_1 $ and $ \varepsilon_2 $ respectively, defined on $ I $ with values in $ H $, then, for all $ t \in I $ such that $ t \geq t_0 $,

$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\| \Phi(t) + (\varepsilon_1 + \varepsilon_2)\Psi(t)
$$

where

$$
\begin{cases}
\Phi(t) = 1 + \int_{t_0}^t k(s) \exp \left( \int_s^t k(\tau) d\tau \right) ds \\
\Psi(t) = t - t_0 + \int_{t_0}^t (s - t_0)k(s) \exp \left( \int_s^t k(\tau) d\tau \right) ds.
\end{cases}
$$

From the relation $ \|u'(t) - f(t, u(t))\| \leq \varepsilon_1 $, valid on the complement of a countable set, one deduces, from the mean value theorem, that

$$
\left\| u(t) - u(t_0) - \int_{t_0}^t f(s, u(s))\, ds \right\| \leq \varepsilon_1 (t - t_0)
$$

and similarly

$$
\left\| v(t) - v(t_0) - \int_{t_0}^t f(s, v(s))\, ds \right\| \leq \varepsilon_2 (t - t_0)
$$

whence

$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\|
$$
$$
+ \left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\, ds \right\| + (\varepsilon_1 + \varepsilon_2)(t - t_0).
$$

By the Lipschitz condition (8) one has

$$
\left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\, ds \right\| \leq \int_{t_0}^t \|f(s, u(s)) - f(s, v(s))\|\, ds
$$
$$
\leq \int_{t_0}^t k(s) \|u(s) - v(s)\|\, ds
$$

whence, putting $ w(t) = \|u(t) - v(t)\| $,

$$
w(t) \leq w(t_0) + (\varepsilon_1 + \varepsilon_2)(t - t_0) + \int_{t_0}^t k(s)w(s)\, ds.
$$

The proposition is thus a consequence of the following lemma:

#### Lemma 2 {#fvr-iv-s1-lem-2 .statement}

*If w is a continuous real function on the interval [t_0, t_1] and satisfies the inequality*

$$
w(t) \leq \varphi(t) + \int_{t_0}^{t} k(s) w(s) \, ds
$$
(12)

*where $ \varphi $ is a regulated function $ \geq 0 $ on $[t_0, t_1]$, then, for $ t_0 \leq t \leq t_1 $,*

$$
w(t) \leq \varphi(t) + \int_{t_0}^{t} \varphi(s) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) \, ds.
$$
(13)

Put $ y(t) = \int_{t_0}^t k(s) w(s) \, ds $; the relation (12) implies that

$$
y'(t) - k(t) y(t) \leq \varphi(t) k(t)
$$
(14)

on the complement of a countable set.

Put $ z(t) = y(t) \exp \left( - \int_{t_0}^t k(s) \, ds \right) $; then (14) is equivalent to

$$
z'(t) \leq \varphi(t) k(t) \exp \left( - \int_{t_0}^t k(s) \, ds \right).
$$

On applying the mean value theorem (I, p. 15, th. 2) to this inequality, and noting that $ z(t_0) = 0 $, we obtain

$$
z(t) \leq \int_{t_0}^t \varphi(s) k(s) \exp \left( - \int_{t_0}^s k(\tau) \, d\tau \right) \, ds
$$

whence

$$
y(t) \leq \int_{t_0}^t \varphi(s) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) \, ds
$$

and since $ w(t) \leq \varphi(t) + y(t) $ one thus obtains (13).

#### Corollary {#fvr-iv-s1-n4-cor-1 .statement}

*Let $ \mathbf{f} $ be a Lipschitz function for the constant $ k > 0 $, defined on $ \mathbf{I} \times \mathbf{H} $. If $ \mathbf{u} $ and $ \mathbf{v} $ are two approximate solutions of (1) to within $ \varepsilon_1 $ and $ \varepsilon_2 $ respectively, defined on $ \mathbf{I} $ and taking their values in $ \mathbf{H} $, then, for all $ t \in \mathbf{I} $,*

$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k |t - t_0|} + (\varepsilon_1 + \varepsilon_2) \frac{e^{k |t - t_0|} - 1}{k}.
$$
(15)

This inequality is in fact an immediate consequence of (9) when $ t \geq t_0 $; to prove it for $ t \leq t_0 $ it suffices to apply it to the equation

$$
\frac{d \mathbf{x}}{ds} = -\mathbf{f}(-s, \mathbf{x})
$$

obtained from (1) by the change of variable $ t = -s $.

#### Remark 1 {#fvr-iv-s1-n4-rem-1 .statement}

When $ k = 0 $ the inequality (15) is replaced by the inequality
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| + (\varepsilon_1 + \varepsilon_2) |t - t_0|
$$
whose proof is immediate.

#### Remark 2 {#fvr-iv-s1-n4-rem-2 .statement}

When E is of finite dimension, and $ \mathbf{f} $ is Lipschitz on $ I \times H $, one can show the existence of approximate solutions of (1) (IV, p. 166, prop. 3) without using the axiom of choice (IV, p. 199, exerc. 1 b)).

#### Proposition 6 {#fvr-iv-s1-prop-6 .statement}

*Let $ \mathbf{f} $ and $ \mathbf{g} $ be two functions defined on $ I \times H $, satisfying the hypotheses of lemma 1 of IV, p. 165, and such that, on $ I \times H $,
$$
\| \mathbf{f}(t, \mathbf{x}) - \mathbf{g}(t, \mathbf{x}) \| \leq \alpha.
$$
(16)

Suppose further that $ \mathbf{g} $ is Lipschitz for the constant $ k > 0 $ on $ I \times H $. In these circumstances, if $ \mathbf{u} $ is an approximate solution of $ \mathbf{x}' = \mathbf{f}(t, \mathbf{x}) $ to within $ \varepsilon_1 $, defined on $ I $, with values in $ H $, and $ \mathbf{v} $ is an approximate solution of $ \mathbf{x}' = \mathbf{g}(t, \mathbf{x}) $ to within $ \varepsilon_2 $, defined on $ I $, with values in $ H $, then, for all $ t \in I $
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k|t-t_0|} + (\alpha + \varepsilon_1 + \varepsilon_2) \frac{e^{k|t-t_0|} - 1}{k}.
$$
(17)

Indeed
$$
\left\| \mathbf{u}'(t) - \mathbf{g}(t, \mathbf{u}(t)) \right\| \leq \alpha + \varepsilon_1
$$
for all $ t $ in the complement in $ I $ of a countable subset of $ I $; in other words, $ \mathbf{u} $ is an approximate solution of $ \mathbf{x}' = \mathbf{g}(t, \mathbf{x}) $ to within $ \alpha + \varepsilon_1 $, so the inequality (17) follows on applying prop. 5 of IV, p. 169.

### 5. EXISTENCE AND UNIQUENESS OF SOLUTIONS OF LIPSCHITZ AND LOCALLY LIPSCHITZ EQUATIONS

#### Theorem 1 (Cauchy) {#fvr-iv-s1-thm-1 .statement}

*Let $ \mathbf{f} $ be a Lipschitz function on $ I \times H $, let J be a compact subinterval of $ I $, not reducing to a single point, $ t_0 $ a point of J, S an open ball with centre $ \mathbf{x}_0 $ and radius r, contained in H, and M the least upper bound of $ \| \mathbf{f}(t, \mathbf{x}) \| $ on $ J \times S $. In these circumstances, for every compact interval K that does not reduce to a single point and is contained in the intersection of J with $ ]t_0 - r/M, t_0 + r/M[ $, and contains $ t_0 $, there exists one and only one solution of the differential equation $ \mathbf{x}' = \mathbf{f}(t, \mathbf{x}) $ defined on K, with values in S, and equal to $ \mathbf{x}_0 $ at the point $ t_0 $.

Indeed, for $ \varepsilon > 0 $ sufficiently small, the set $ F_\varepsilon $ of approximate solutions of (1) to within $ \varepsilon $, defined on K, with values in S, and equal to $ \mathbf{x}_0 $ at the point $ t_0 $, is not empty (IV, p. 166, prop. 3); further, if $ \mathbf{u} $ and $ \mathbf{v} $ belong to $ F_\varepsilon $ then, by (15) (IV. p. 170)
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq 2\varepsilon \frac{e^{k|t-t_0|} - 1}{k}
$$

for all $ t \in K $, so the sets $ F_\varepsilon $ form a filter base $ \mathcal{G} $ which converges uniformly on $ K $ to a continuous function $ w $, equal to $ x_0 $ at $ t_0 $; also $ w $ takes values in $ S $, since, for $ \varepsilon $ small enough, the functions $ u \in F_\varepsilon $ take their values in a closed ball contained in $ S $. Since $ f(t, u(t)) $ tends uniformly on $ K $ to $ f(t, w(t)) $ along $ \mathcal{G} $, $ w $ satisfies equation (6) of IV, p. 165, so is a solution of (1). The uniqueness of the solution follows immediately from inequality (15) of IV, p. 170 where one takes $ \varepsilon_1 = \varepsilon_2 = 0 $ and $ u(t_0) = v(t_0) $.

We shall say that a function $ f $ defined on $ I \times H $ is locally Lipschitz if, for every point $ (t, x) $ of $ I \times H $, there exists a neighbourhood $ V $ of $ t $ (with respect to $ I $) and a neighbourhood $ S $ of $ x $ such that $ f $ is Lipschitz on $ V \times S $ (for a constant $ k $ depending on $ V $ and $ S $). By the Borel-Lebesgue theorem, for every compact interval $ J \subset I $ and every point $ x_0 \in H $ there exists an open ball $ S $ with centre $ x_0 $, contained in $ H $, such that $ f $ is Lipschitz on $ J \times S $; thus $ f $ satisfies the hypotheses of lemma 1 of IV, p. 3. When $ f $ is locally Lipschitz on $ I \times H $ we shall say that the equation $ x' = f(t, x) $ is locally Lipschitz on $ I \times H $.

We shall generalize and clarify th. 1 of IV, p. 10 for locally Lipschitz equations; we restrict ourselves to the case where $ t_0 $ is the left endpoint of the interval $ I $; one can pass easily to the case where $ t_0 $ is an arbitrary point of $ I $ (cf. IV, §IV ??, p. 9, corollary).

#### Theorem 2 {#fvr-iv-s1-thm-2 .statement}

*Let $ I \subset \mathbf{R} $ be an interval (not reducing to a single point) with left-hand endpoint $ t_0 \in I $, let $ H $ be a nonempty open set in $ E $, and $ f $ a locally Lipschitz function on $ I \times H $.*

$ 1^\circ $ *For $ x_0 \in H $ there exists a largest interval $ J \subset I $, with left-hand endpoint $ t_0 \in J $, on which there exists an integral $ u $ of the equation $ x' = f(t, x) $ taking values in $ H $ and equal to $ x_0 $ at the point $ t_0 $; this integral is unique.*

$ 2^\circ $ *If $ J \neq I $ then $ J $ is a half-open interval $ [t_0, \beta[ $ of finite length; further, for every compact subset $ K \subset H $ the set $ \overline{u}(K) $ is a compact subset of $ \mathbf{R} $.*

$ 3^\circ $ *If $ J $ is bounded, and if $ f(t, u(t)) $ is bounded on $ J $, then $ u(t) $ has a left limit $ c $ at the right-hand endpoint of $ J $; further, if $ J \neq I $ then $ c $ is a boundary point of $ H $ in $ E $.*

$ 1^\circ $ Let $ \mathfrak{M} $ be the set of intervals $ L $ (not reducing to a single point) with left-hand endpoint $ t_0 \in L $ which are contained in $ I $ and are such that on $ L $ there is a solution of (1) (IV, p. 163) with values in $ H $ and equal to $ x_0 $ at $ t_0 $; by th. 1 (IV, p. 171) the set $ \mathfrak{M} $ is not empty. Let $ L $ and $ L' $ be two intervals belonging to $ \mathfrak{M} $, and suppose, for example, that $ L \subset L' $; if $ u $ and $ v $ are two integrals of (1) defined respectively on $ L $ and $ L' $, with values in $ H $, and equal to $ x_0 $ at $ t_0 $, we shall see that $ v $ is an extension of $ u $. Indeed, let $ t_1 $ be the supremum of the set of $ t \in L $ such that $ u(s) = v(s) $ for $ t_0 \leq s \leq t $; we shall show that $ t_1 $ is the right-hand endpoint of $ L $. If this were not so, we would have $ u(t_1) = v(t_1) $ by continuity, and $ x_1 = u(t_1) $ would belong to $ H $; since $ f $ is locally Lipschitz, th. 1 shows that there can exist only one integral of (1) defined on a neighbourhood of $ t_1 $ with values in $ H $ and equal to $ x_1 $ at $ t_1 $; it is therefore a contradiction to suppose that $ t_1 $ is not the right-hand endpoint of $ L $. We now see that if $ J $ is the union of the intervals $ L \in \mathfrak{M} $ there exists one and only one integral $ u $ of (1), defined on $ J $, with values in $ H $ and equal to $ x_0 $ at $ t_0 $.

2' Suppose that J ≠ I and let β be the right endpoint of J; if β is the right-hand endpoint of I then β ∈ I (so β is finite) and J = [t_0, β[ by hypothesis. Suppose then that β is not the right-hand endpoint of I; if β ∈ J then u(β) = c belongs to H; by th. 1 there exists an integral of (1) with values in H, defined on an interval

$$ [\beta, \beta_1[ \subset I $$

and equal to c at β; then J would not be the largest of the intervals in $ \mathfrak{M} $, which is absurd; so J = [t_0, β[.

If K is a compact subset of H then $ \bar{u}^{-1}(K) $ is closed in J; we shall see that there exists a γ ∈ J such that $ \bar{u}^{-1}(K) $ is contained in [t_0, γ ], which will prove that $ \bar{u}^{-1}(K) $ is compact. If not, there would be a point c ∈ K such that (β, c) is a cluster point of the set of points (t, u(t)) such that t < β and u(t) ∈ K. Since β ∈ I and c ∈ H there exists a neighbourhood V of β in I, and an open ball S with centre c and radius r contained in H, such that f is Lipschitz and bounded on V × S; let M be the supremum of $ \|f(t, x)\| $ over this set. By hypothesis there exists a t_1 ∈ J such that $ \beta - t_1 < r/2M $, $ t_1 \in V $ and $ \|u(t_1) - c\| \leq r/2 $; th. 1 shows that there exists one and only one integral of (1), with values in H, defined on an interval [t_1, t_2] containing β, and equal to u(t_1) at t_1; since this interval coincides with u on the interval [t_1, β[ it follows that J = [t_0, β[ is not the largest interval in $ \mathfrak{M} $, which is absurd.

3 Suppose that J is bounded and that $ \|f(t, u(t))\| \leq M $ on J; then $ \|u'(t)\| \leq M $ on the complement of a countable subset of J; then, by the mean value theorem, $ \|u(s) - u(t)\| \leq M |s - t| $ for any s and t in J; by the Cauchy criterion, u has a left limit c at the right endpoint β of J. If J ≠ I then c cannot belong to H, for on extending u by continuity at β, u would be an integral of (1) with values in H, defined on an interval [t_0, β] and equal to x_0 at t_0; then one would have J = [t_0, β], contradicting what we have seen in 2 .

#### Corollary 1 {#fvr-iv-s1-thm-2-cor-1 .statement}

*If H = E and J ≠ I then f(t, u(t)) is not bounded on J, if, further, E is finite dimensional, then $ \|u(t)\| $ has left limit $ +\infty $ at the right-hand endpoint of J.*

The first part is an immediate consequence of the third part of th. 2 If E is finite dimensional then every closed ball S ⊂ E is compact, so the second part of th. 2 shows that there exists a γ ∈ J such that u(t) ∉ S for t > γ.

If E is finite dimensional it can happen that J ≠ I but that $ \|u(t)\| $ remains *bounded* as t tends to the right-hand endpoint of J (IV, p. 200, exerc. 5).

#### Corollary 2 {#fvr-iv-s1-thm-2-cor-2 .statement}

*If, on I × H, the function f is Lipschitz with respect to a regulated function k(t), and if the right-hand endpoint β of J belongs to I, then u has a left limit at β; if H = E and if f is Lipschitz with respect to a regulated function k(t) on I × E, then J = I.*

Indeed, if β ∈ I, there exists a compact neighbourhood V of β in I, such that f(t, x_0) and k(t) are bounded on V; then $ \|f(t, x)\| \leq m \|x\| + h $ (m and h constant) on $ V \times H $, whence $ \|u'(t)\| \leq m \|u(t)\| + h $ on the complement of a countable subset of $ V \cap J $, so that $ \|u(t)\| \leq m \int_{t_0}^t \|u(s)\|\ ds + q $ ($ q $ constant) on $ V \cap J $; lemma 2 (IV, p. 170) shows that $ \|u(t)\| \leq c\ e^{mt} + d $ ($ c $ and $ d $ constant) on $ V \cap J $, and thus $ f(t, u(t)) $ remains *bounded* on $ J $, and the corollary results from th. 2 of IV, p. 172.

#### Example 1 {#fvr-iv-s1-n5-exa-1 .statement}

For a differential equation of the form $ x' = g(t) $, where $ g $ is regulated on $ I $, every integral $ u $ is clearly defined on all of $ I $. One should note that $ u $ can be bounded on $ I $ without $ g(t) $ being so.

#### Example 2 {#fvr-iv-s1-n5-exa-2 .statement}

For the scalar equation $ x' = \sqrt{1 - x^2} $ one has $ I = \mathbf{R},\ H = ] - 1, +1[ $. If one takes $ t_0 = x_0 = 0 $ the corresponding integral is $ \sin t $ *on the largest interval containing 0 where the derivative of $ \sin t $ is positive*, that is to say, on $ ] - \pi/2, +\pi/2[ $; at the endpoints of this interval the integral tends to an endpoint of $ H $.

#### Example 3 {#fvr-iv-s1-n5-exa-3 .statement}

For the scalar equation $ x' = 1 + x^2 $ one has $ I = H = \mathbf{R} $: the integral that vanishes at $ t = 0 $ is $ \tan t $, and the largest interval containing 0 where this function is continuous is $ J = ] - \pi/2, +\pi/2[ $; and $ |\tan t| $ tends to $ +\infty $ at the endpoints of $ J $ (*cf.* IV, p. 173, cor. 1).

#### Example 4 {#fvr-iv-s1-n5-exa-4 .statement}

For the scalar equation $ x' = \sin tx $ one has $ I = H = \mathbf{R} $ and the right-hand side is bounded on $ I \times H $, so (IV, p. 173, cor. 1) every integral is defined on all of $ \mathbf{R} $.

### 6. CONTINUITY OF INTEGRALS AS FUNCTIONS OF A PARAMETER

Prop. 6 (IV, p. 171) shows that when a differential equation

$$
x' = f(t, x)
$$

is "close" to a Lipschitz equation $ x' = g(t, x) $ and when one supposes that *both* equations have an approximate solution on the same interval, then these approximate solutions are "close"; we shall clarify this result by showing that the existence of solutions of the Lipschitz equation $ x' = g(t, x) $ on an interval *implies* that of approximate solutions of $ x' = f(t, x) $ on the same interval, so long as, on the latter, the values of the solution of $ x' = g(t, x) $ are not "too close" to the *boundary* of $ H $.

#### Proposition 7 {#fvr-iv-s1-prop-7 .statement}

*Let $ f $ and $ g $ be two functions defined on $ I \times H $, satisfying the hypotheses of lemma 1 of IV. p. 165, and such that, on $ I \times H $*

$$
\|f(t, x) - g(t, x)\| \leq \alpha .
$$
(16)

*Suppose further that $ g $ is Lipschitz with respect to a constant $ k > 0 $ on $ I \times H $ and that $ f $ is locally Lipschitz on $ I \times H $, or that $ E $ is finite dimensional. Let $ (t_0, x_0) $ be a point of $ I \times H $, $ \mu $ a number $ > 0 $, and*

$$
\varphi(t) = \mu\ e^{k(t-t_0)} + \alpha\ \frac{e^{k(t-t_0)} - 1}{k} .
$$

*Let $ u $ be an integral of the equation $ x' = g(t, x) $ defined on an interval $ K = [t_0, b[ $ contained in $ I $, equal to $ x_0 $ at the point $ t_0 $, and such that for all $ t \in K $ the closed ball with centre $ u(t) $ and radius $ \varphi(t) $ is contained in $ H $. Under these conditions, for every $ y \in H $ such that $ \|y - x_0\| \leq \mu $ there exists an integral $ v $ of $ x' = f(t, x) $, defined on $ K $, with values in $ H $, and equal to $ y $ at the point $ t_0 $; moreover, $ \|u(t) - v(t)\| \leq \varphi(t) $ on $ K $.*

Let $ \mathcal{M} $ be the family of integrals of $ x' = f(t, x) $ each of which takes its values in $ H $, is equal to $ y $ at $ t_0 $, and is defined on a half-open interval $[t_0, \tau[$ contained in $ I $ (depending on the interval considered). By th. 1 of IV, p. 171 (when $ f $ is locally Lipschitz) or IV, p. 167 corollary (when $ E $ is finite dimensional), $ \mathcal{M} $ is not empty, and the same reasoning as in prop. 3 of IV, p. 166 shows that $ \mathcal{M} $ is *inductive* for the order "v is a restriction of w". Let $ v_0 $ be a maximal element of $ \mathcal{M} $ and $[t_0, t_1[$ the interval of definition of $ v_0 $; by prop. 6 of IV, p. 171, it all comes down to proving that $ t_1 \geq b $. If not, one would have

$$
\| u(t) - v_0(t) \| \leq \varphi(t)
$$

on the interval $[t_0, t_1[$ by prop. 6; now on the compact interval $[t_0, t_1]$ the regulated function $ g(t, u(t)) $ is bounded, so the function $ g(t, v_0(t)) $ is bounded on the interval $[t_0, t_1[$, for $ \| g(t, v_0(t)) \| \leq \| g(t, u(t)) \| + k \varphi(t) $ on this interval. Since $ v_0 $ is an approximate solution of $ x' = g(t, x) $ to within $ \alpha $ on $[t_0, t_1[$ there exists a number $ M > 0 $ such that $ \| v_0'(t) \| \leq M $ on this interval, except at the points of a countable set; the mean value theorem now shows that $ \| v_0(s) - v_0(t) \| \leq M |s - t| $ for every pair of points $ s, t $ of $[t_0, t_1[$, so (by Cauchy's criterion) $ v_0(t) $ has a left limit $ c $ at the point $ t_1 $, and, by continuity, one has $ \| c - u(t_1) \| \leq \varphi(t_1) $, and so $ c \in H $. Now one sees, from IV, p. 171, th. 1 or IV, p. 167, corollary, that there exists an integral of $ x' = f(t, x) $ defined on an interval $[t_1, t_2[$ and equal to $ c $ at $ t_1 $, which contradicts the definition of $ v_0 $.

#### Theorem 3 {#fvr-iv-s1-thm-3 .statement}

*Let F be a topological space and let f be a map from I × H × F into E such that, for every $ \xi \in F $, the function $ (t, x) \mapsto f(t, x, \xi) $ is Lipschitz on I × H, and such that, when $ \xi $ tends to $ \xi_0 $, $ f(t, x, \xi) $ tends uniformly to $ f(t, x, \xi_0) $ on I × H. Let $ u_0(t) $ be an integral of $ x' = f(t, x, \xi_0) $ defined on an interval $ J = [t_0, b[ $ contained in I, with values in H, and equal to $ x_0 $ at $ t_0 $. For every compact interval $[t_0, t_1]$ contained in J there exists a neighbourhood V of $ \xi_0 $ in F such that, for every $ \xi \in V $, the equation $ x' = f(t, x, \xi) $ has an integral (and only one) $ u(t, \xi) $ defined on $[t_0, t_1]$, with values in H and equal to $ x_0 $ at $ t_0 $; moreover, when $ \xi $ tends to $ \xi_0 $ the solution $ u(t, \xi) $ tends uniformly to $ u_0(t) $ on $[t_0, t_1]$.*

Indeed, let $ r > 0 $ be such that for $ t_0 \leq t \leq t_1 $ the closed ball with centre $ u_0(t) $ and radius $ r $ is contained in $ H $; if $ f(t, x, \xi) $ is Lipschitz with respect to the constant $ k > 0 $ on $ I \times H $ we take $ \alpha $ small enough that $ \alpha \frac{e^{k(t_1-t_0)} - 1}{k} < r $; taking $ V $ such that, for every $ \xi \in V $, one has $ \| f(t, x, \xi) - f(t, x, \xi_0) \| \leq \alpha $ on $ I \times H $, one can apply prop. 7 of IV, p. 174; moreover,

$$
\| u(t, \xi) - u_0(t) \| \leq \alpha \frac{e^{k(t_1-t_0)} - 1}{k}
$$

on $[t_0, t_1]$, which completes the proof of the theorem.

#### Remark {#fvr-iv-s1-n6-rem-1 .statement}

When $ H = E $ and the condition (16) of IV, p. 174 is satisfied on $ I \times E $, prop. 7 of IV, p. 174 applies to *every* solution $ u $ of $ x' = g(t, x) $ on *any* interval where this solution is defined; one may even assume that $ g(t, x) $ is Lipschitz with respect to a regulated function $ k(t) $ though not necessarily bounded on this interval.

### 7. DEPENDENCE ON INITIAL CONDITIONS

Let $ x' = f(t, x) $ be a locally Lipschitz equation on $ I \times H $; by th. 2 (IV, p. 172), for every point $ (t_0, x_0) $ of $ I \times H $ there exists a *largest interval* $ J(t_0, x_0) \subset I $, not reducing to a single point, containing $ t_0 $, and on which there exists an integral (and only one) of this equation, equal to $ x_0 $ at $ t_0 $; we shall clarify the manner in which this integral, and the interval $ J(t_0, x_0) $ where it is defined, depend on the point $ (t_0, x_0) $.

#### Theorem 4 {#fvr-iv-s1-thm-4 .statement}

*Let $ f $ be a locally Lipschitz function on $ I \times H $ and $ (a, b) $ an arbitrary point of $ I \times H $.*

1 *There exist an interval $ K \subset I $, a neighbourhood of $ a $ in $ I $, and a neighbourhood $ V $ of $ b $ in $ H $ such that, for every point $ (t_0, x_0) $ of $ K \times V $, there exists an integral (and only one) $ u(t, t_0, x_0) $ defined on $ K $, with values in $ H $ and equal to $ x_0 $ at the point $ t_0 $ (in other words, $ J(t_0, x_0) \supset K $ for all $ (t_0, x_0) \in K \times V $).*

2 *The map $ (t, t_0, x_0) \mapsto u(t, t_0, x_0) $ of $ K \times K \times V $ into $ H $ is uniformly continuous.*

3 *There exists a neighbourhood $ W \subset V $ of $ b $ in $ H $ such that, for every point*
$$
(t, t_0, x_0) \in K \times K \times W,
$$
*the equation $ x_0 = u(t_0, t, x) $ has a unique solution $ x $ on $ V $ equal to $ u(t, t_0, x_0) $* ("resolution of the integral with respect to the constant of integration").

1 Let $ S $ be a ball with centre $ b $ and radius $ r $ contained in $ H $, and $ J_0 $ an interval contained in $ I $, a neighbourhood of $ a $ in $ I $, such that $ f $ is bounded and Lipschitz (with respect to some constant $ k $) on $ J_0 \times S $; denote by $ M $ the supremum of $ \|f(t, x)\| $ on $ J_0 \times S $. Then there exist (IV, p. 171, th. 1) an interval $ J \subset J_0 $, a neighbourhood of $ a $ in $ I $, and an integral $ v $ of $ x' = f(t, x) $ defined on $ J $, with values in $ S $ and equal to $ b $ at $ a $. We shall see that the open ball $ V $ with centre $ b $ and radius $ r/2 $, and the intersection $ K $ of $ J $ with an interval $ ]a - l, a + l[ $, where $ l $ is *small enough*, are as required. Indeed, prop. 7 of IV, p. 174 (applied to the set $ J_0 \times S $ and the case where $ \alpha = 0 $) shows that there exists an integral of $ x' = f(t, x) $ *defined on* $ K $, with values in $ S $, and equal to $ x_0 $ at a point $ t_0 \in K $, provided that
$$
\|v(t) - b\| + \|v(t_0) - x_0\| e^{k|t-t_0|} < r
$$
for every $ t \in K $. Now, by the mean value theorem, one has
$$
\|v(t) - b\| \leq M |t - a| \leq Ml
$$
for every $ t \in K $; since $ \|x_0 - b\| < r/2 $ one sees that it suffices to take $ l $ such that
$$
Ml + (Ml + r/2)e^{2kl} < r
$$
or the relation (18) to be satisfied for every $ (t, t_0, x_0) $ of $ K \times K \times V $.

2' By the mean value theorem we have

$$
\| \mathbf{u}(t_1, t_0, \mathbf{x}_0) - \mathbf{u}(t_2, t_0, \mathbf{x}_0) \| \leq M |t_2 - t_1|
$$

(20)

for all $ t_0, t_1, t_2 $ in K and $ \mathbf{x}_0 $ in V. Now prop. 5 (IV, p. 169) shows that

$$
\| \mathbf{u}(t, t_0, \mathbf{x}_1) - \mathbf{u}(t, t_0, \mathbf{x}_2) \| \leq e^{2kt} \ \| \mathbf{x}_2 - \mathbf{x}_1 \|
$$

(21)

for every $ t $ and $ t_0 $ in K, and $ \mathbf{x}_1 $ and $ \mathbf{x}_2 $ in V. Finally, if $ t_1 $ and $ t_2 $ are any two points in K,

$$
\| \mathbf{u}(t_1, t_2, \mathbf{x}_0) - \mathbf{u}(t_2, t_2, \mathbf{x}_0) \| \leq M |t_2 - t_1|
$$

by the mean value theorem, that is to say

$$
\| \mathbf{u}(t_1, t_2, \mathbf{x}_0) - \mathbf{x}_0 \| \leq M |t_2 - t_1| ;
$$

since $ \mathbf{u}(t, t_2, \mathbf{x}_0) $ is identical to the integral which takes the value $ \mathbf{u}(t_1, t_2, \mathbf{x}_0) $ at the point $ t_1 $, prop. 5 (IV, p. 169) shows that

$$
\| \mathbf{u}(t, t_1, \mathbf{x}_0) - \mathbf{u}(t, t_2, \mathbf{x}_0) \| \leq Me^{2kl} |t_2 - t_1|
$$

(22)

for all $ t, t_1, t_2 $ in K and $ \mathbf{x}_0 $ in V. The three inequalities (20), (21) and (22) thus prove the uniform continuity of the map $ (t, t_0, \mathbf{x}_0) \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0) $ on $ K \times K \times V $.

3 By (20), we have $ \| \mathbf{u}(t, t_0, \mathbf{x}_0) - \mathbf{x}_0 \| \leq M |t - t_0| \leq 2Ml $ on

$$
K \times K \times V.
$$

If $ l $ is taken small enough, so that $ 2Ml < r/4 $, one then sees that if $ \mathbf{x}_0 $ is any point of the open ball W with centre $ \mathbf{b} $ and radius $ r/4 $, that $ \mathbf{u}(t, t_0, \mathbf{x}_0) \in V $ for any $ t $ and $ t_0 $ in K. If $ \mathbf{x} = \mathbf{u}(t, t_0, \mathbf{x}_0) $, the function $ s \mapsto \mathbf{u}(s, t, \mathbf{x}) $ is then defined on K and is equal to the integral of (1) which takes the value $ \mathbf{x} $ at the point $ t $, that is, to $ \mathbf{u}(s, t_0, \mathbf{x}_0) $; in particular

$$
\mathbf{x}_0 = \mathbf{u}(t_0, t_0, \mathbf{x}_0) = \mathbf{u}(t_0, t, \mathbf{x}).
$$

Moreover, if $ y \in V $ is such that $ \mathbf{x}_0 = \mathbf{u}(t_0, t, y) $, then the integral $ s \mapsto \mathbf{u}(s, t, y) $ takes the value $ \mathbf{x}_0 $ at $ t_0 $ so is identical to $ s \mapsto \mathbf{u}(s, t_0, \mathbf{x}_0) $, which consequently takes the value $ \mathbf{x} $ at $ t $, which shows that $ y = \mathbf{x} $ and concludes the proof.

### Exercises {#fvr-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
