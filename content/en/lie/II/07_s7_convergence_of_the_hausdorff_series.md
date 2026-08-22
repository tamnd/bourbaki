---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 7
section_title: Convergence of the Hausdorff series (real or complex case)
lang: en
source: lie-i-iii
pdf_pages: 0182-0188, 0222-0222
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS-POLYNOMIALS WITH VALUES IN $ g $
      page: 0
      pdf_page: 182
    - "no": 2
      title: GROUP GERM DEFINED BY A COMPLETE NORMED LIE ALGEBRA
      page: 0
      pdf_page: 183
    - "no": 3
      title: Exponential in Complete Normed Associative Algebras
      page: 0
      pdf_page: 187
statements: 4
exercises: 1
content_sha256: 5da45aeabf8166b0333b151ccda2df4e0070f0333ee675c1305d7ea8d515cb86
---

## § 7. CONVERGENCE OF THE HAUSDORFF SERIES (REAL OR COMPLEX CASE)

In this paragraph we assume that $ K $ is one of the fields $ \mathbf{R} $ or $ \mathbf{C} $ with its usual absolute value. Recall that a normable algebra over $ K $ is a (not necessarily associative) algebra over $ K $ with a topology $ \mathcal{T} $ with the following properties:
(1) $ \mathcal{T} $ can be defined by a norm:
(2) the mapping $ (x, y) \mapsto xy $ of $ A \times A $ into $ A $ is continuous.
A normed algebra over $ K $ is an algebra $ A $ over $ K $ with a norm such that $ \|xy\| \leq \|x\|\ \|y\| $ for all $ x, y $ in $ A $.
We denote by $ g $ a complete normable Lie algebra over $ K $. We choose a norm on $ g $ and a number $ M > 0 $ such that
$$
\|[x, y]\| \leq M \|x\|\ \|y\| \quad \text{for } x, y \text{ in } g.
$$

### 1. CONTINUOUS-POLYNOMIALS WITH VALUES IN $ g $

Let $ I $ be a finite set and let $ P(g^I; g) $ (resp. $ \hat{P}(g^I; g) $) be the vector space of *continuous-polynomials* (resp. *formal power series with continuous components*) on $ g^I $ with values in $ g $. Recall (*Differentiable and Analytic Manifolds*, R, Appendix) that $ P(g^I; g) $ has a graduation of type $ \mathbf{N}^I $ and that $ \hat{P}(g^I; g) $ is identified with the completion of the vector space $ P(g^I; g) $ with the topology defined by the filtration associated with the graduation of $ P(g^I; g) $. Moreover, $ P(g^I; g) $ is a graded Lie algebra with the bracket defined by $ [f, g](x) = [f(x), g(x)] $ for f, g in P(g^I; g), x \in g^I; this Lie algebra structure can be extended by continuity to $ \hat{P}(g^I; g) $ and makes it into a complete Hausdorff filtered Lie algebra.

By proposition 2 of § 6, no. 3, there exists one and only one continuous Lie algebra homomorphism $ \phi_I : u \mapsto \tilde{u} $ of $ \hat{L}(I) $ into $ \hat{P}(g^I; g) $ mapping the indeterminate of index i to $ \mathrm{pr}_i $ for all $ i \in I $, since $ \mathrm{pr}_i \in P(g^I; g) $. It follows that $ \tilde{u} \in P(g^I; g) $ for $ u \in L(I) $; more precisely, when $ u \in L(I) $, $ \tilde{u} $ is just the polynomial mapping $ (t_i) \mapsto u((t_i)) $ of § 2, no. 4. On the other hand, clearly $ \phi_I $ is compatible with the multigraduations of $ L(I) $ and $ P(g^I; g) $. If $ u = \sum_{v \in \mathbf{N}^I} u_v $, where $ u_v \in L^v(I) $ for $ v \in \mathbf{N}^I $, then

$$
\tilde{u} = \sum_{v \in \mathbf{N}^I} \tilde{u}_v, \quad \text{where } \tilde{u}_v \in P_v(g^I; g).
$$

Let $ u = (u_j)_{j \in J} $ be a finite family of elements of $ \hat{L}(I) $, let $ v \in \hat{L}(J) $ and let $ w = v \circ u $ (\S 6, no. 3). We write $ \tilde{u} = (\tilde{u}_j)_{j \in J} \in \mathfrak{g} $. Then

(2)
$$
\tilde{v} \circ \tilde{u} = (v \circ u)^{\sim}.
$$

This follows by extending by continuity formula (7) of § 6, no. 3 and from Differentiable and Analytic Manifolds, R, Appendix, no. 6.

### 2. GROUP GERM DEFINED BY A COMPLETE NORMED LIE ALGEBRA

Let $ H = \sum_{r,s \geq 0} H_{r,s} \in \hat{L}(U, V) $ be the Hausdorff series (\S 6, no. 4, Definition 1). We shall show that the corresponding formal power series

(3)
$$
\tilde{H} = \sum_{r,s \geq 0} \tilde{H}_{r,s} \in \hat{P}(g \times g, g)
$$

is convergent (Differentiable and Analytic Manifolds, R, 3.1.1).

We introduce the following formal power series $ \eta \in \mathbf{Q}[[U, V]] $

(4)
$$
\eta(U, V) = -\log(2 - \exp(U + V))
$$
(5)
$$
= \sum_{m \geq 1} \frac{1}{m} (\exp(U + V) - 1)^m
$$
(6)
$$
= \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1, \ldots, r_m \\ s_1, \ldots, s_m}} \frac{U^{r_1} V^{s_1}}{r_1!} \frac{U^{r_2} V^{s_2}}{r_2!} \cdots \frac{U^{r_m} V^{s_m}}{s_m!}.
$$

Hence

(7)
$$
\eta(U, V) = \sum_{r,s \geq 0} \eta_{r,s} U^r V^s,
$$

where
$$
\eta_{r,s} = \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_i + s_i \geq 1}} \frac{1}{r_1! \ldots r_m! s_1! \ldots s_m!}.
$$
Now let $ u $ and $ v $ be two positive real numbers such that $ u + v < \log 2 $; then $ 0 \leq \exp(u + v) - 1 < 1 $; the series derived from (5) and (6) by substituting $ u $ for $ U $ and $ v $ for $ V $ are convergent and the above calculations imply that
$$
\sum_{r, s \geq 0} \eta_{r,s} u^r v^s = -\log(2 - \exp(u + v)) < +\infty.
$$
Let $ r, s \geq 0 $ and let $ \| \tilde{H}_{r,s} \| $ be the norm of the continuous-polynomial $ \tilde{H}_{r,s} $ (Differentiable and Analytic Manifolds, R, Appendix, no. 2).

#### Lemma 1 {#lie-ii-s7-lem-1 .statement}

$$
\| \tilde{H}_{r,s} \| \leq M^{r+s-1} \eta_{r,s}.
$$
Let $ r_i, s_i $ be in $ \mathbf{N} $ for $ 1 \leq i \leq m $, with $ s_m = 1 $; we write $ r = \sum_i r_i, s = \sum_i s_i $ and consider the following element of $ L(\{U, V\}) $:
$$
Z = \left( \left( \sum_{i=1}^{m-1} (\mathrm{ad}\ U)^{r_i} (\mathrm{ad}\ V)^{s_i} \right) (\mathrm{ad}\ U)^{r_m} \right)(V).
$$
Then $ \tilde{Z} = f \circ p $, where $ f $ is the following $ (r+s) $-linear mapping of $ g^{r+s} $ into $ g $:
$$
(x_1, \ldots, x_r, y_1, \ldots, y_s) \mapsto (\mathrm{ad}(x_1) \circ \cdots \circ \mathrm{ad}(x_r) \circ \mathrm{ad}(y_1) \circ \cdots \circ \mathrm{ad}(y_s))(y_s)
$$
and where $ p $ is the following mapping of $ g^2 $ into $ g^{r+s} $:
$$
(x, y) \mapsto (\underbrace{x, \ldots, x}_{r}, \underbrace{y, \ldots, y}_{s});
$$
hence $ \| \tilde{Z} \| \leq \| f \| \leq M^{r+s-1} $ (Differentiable and Analytic Manifolds, R, Appendix). Applying these inequalities to the various terms on the right hand side of formula (9) of § 6, no. 4, we obtain:
$$
\|(H'_{r,s})\sim\|
\leq \frac{M^{r+s-1}}{r+s} \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}} \frac{1}{r_1! \ldots r_m! s_1! \ldots s_m!}.
$$
A similar argument gives
$$
\|(H''_{r,s})\sim\|
\leq \frac{M^{r+s-1}}{r+s} \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_{m-1} = r-1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}} \frac{1}{r_1! \ldots r_{m-1}! s_1! \ldots s_{m-1}!}
$$

whence, by (8)

$$
\|\tilde{H}_{r,s}\| < \eta_{r,s} \frac{M^{r+s-1}}{r+s} \leq \eta_{r,s} M^{r+s-1},
$$

which proves the lemma.

#### Proposition 1 {#lie-ii-s7-prop-1 .statement}

*The formal power series* $ \tilde{H} $ *is a convergent series* (*Differentiable and Analytic Manifolds*, R, 3.1.1); *its domain of absolute convergence* (*Differentiable and Analytic Manifolds*, R, 3.1.4) *contains the open set*

$$
\Omega = \left\{ (x, y) \in g \times g \mid \|x\| + \|y\| < \frac{1}{M} \log 2 \right\}.
$$

Let $ u, v $ be two real numbers $ > 0 $ such that $ u + v < \frac{1}{M} \log 2 $; then (Lemma 1)

$$
\text{(12)} \quad M \sum_{r,s \geq 0} \|\tilde{H}_{r,s}\| u^r v^s \\
\leq \sum_{r,s \geq 0} \eta_{r,s} M^{r+s} u^r v^s = -\log(2 - \exp M(u + v)) < +\infty
$$
by (9).

Let $ h : \Omega \to g $ denote the *analytic function* (*Differentiable and Analytic Manifolds*, R, 3.2.9) defined by $ \tilde{H} $, that is by the formula

$$
\text{(13)} \quad h(x, y) = \sum_{r,s \geq 0} \tilde{H}_{r,s}(x, y) = \sum_{r,s \geq 0} H_{r,s}(x, y) \quad \text{for } (x, y) \in \Omega.
$$

This function is called the *Hausdorff function* of $ g $ relative to $ M $ (or simply the Hausdorff function of $ g $ if no confusion can arise). Note that $ H_{r,s}(U, -U) = 0 $ if $ r + s \geq 2 $ and hence

$$
\text{(14)} \quad h(x, -x) = 0 \quad \text{for } \|x\| < \frac{1}{2M} \log 2.
$$

Similarly

$$
\text{(15)} \quad h(0, x) = h(x, 0) = x \quad \text{for } \|x\| < \frac{1}{M} \log 2.
$$

#### Proposition 2 {#lie-ii-s7-prop-2 .statement}

*Let*

$$
\Omega' = \left\{ (x, y, z) \in g \times g \times g \mid \|x\| + \|y\| + \|z\| < \frac{1}{M} \log \frac{3}{2} \right\}.
$$

*If* $ (x, y, z) \in \Omega' $, *then*

$$
\text{(16)} \quad (x, y) \in \Omega, \quad (h(x, y), z) \in \Omega, \quad (y, z) \in \Omega, \quad (x, h(y, z)) \in \Omega
$$
*and*
$$
\text{(17)} \quad h(h(x, y), z) = h(x, h(y, z)).
$$

Let $(x, y, z) \in \Omega'$; clearly $(x, y) \in \Omega$ and $(y, z) \in \Omega$. Moreover:

$$
\|h(x, y)\| \leq \sum_{r, s} \|H_{r,s}\| \|x|r\|y|s,
$$

and hence by (13)

$$
\|h(x, y)\| \leq -\frac{1}{M} \log(2 - \exp M(\|x\| + \|y\|)).
$$

Now $M(\|x\| + \|y\|) < \log \frac{3}{2} - M\|z\|$; we write $u = \exp(M\|z\|)$; then $1 \leq u \leq \frac{3}{2}$ and

$$
\begin{align*}
M(\|h(x, y)\| + \|z\|) &< -\log(2 - \exp(\log \frac{3}{2} - M\|z\|)) + M\|z\| \\
&= -\log\left(2 - \frac{3}{2u}\right) + \log u = \log \frac{2u^2}{4u - 3} \\
&= \log\left(2 + \frac{2(u - 1)(u - 3)}{4u - 3}\right) \leq \log 2.
\end{align*}
$$

We see similarly that $(x, h(y, z)) \in \Omega$.

We now prove (17). In the Lie algebra $\hat{L}(\{U, V, W\})$,

$$
H(H(U, V), W) = H(U, H(V, W))
$$

by Proposition 4 of § 6, no. 5. By no. 1, formula (2), we therefore have in $\hat{P}(g \times g \times g, g)$ the relation

$$
\tilde{H} \circ (\tilde{H} \times \mathrm{Id}_g) = \tilde{H} \circ (\mathrm{Id}_g \times \tilde{H}).
$$

By *Differentiable and Analytic Manifolds*, R, 3.1.9, there exists a number $\varepsilon > 0$ such that formula (17) is true when $\|x\|, \|y\|$ and $\|z\|$ are $\leq \varepsilon$. But the functions $(x, y, z) \mapsto h(h(x, y), z)$ and $(x, y, z) \mapsto h(x, h(y, z))$ are analytic functions on $\Omega'$ with values in $g$ (*Differentiable and Analytic Manifolds*, R, 3.2.7). As $\Omega'$ is connected and they coincide in a neighbourhood of 0, they are equal (*Differentiable and Analytic Manifolds*, R, 3.2.5).

The above results imply:

Let $\alpha$ be a real number such that $0 < \alpha \leq \frac{1}{3M} \log \frac{3}{2}$. Let

$$
G = \{x \in g \mid \|x\| < \alpha\},
$$

$
\Theta = \{(x, y) \in G \times G \mid h(x, y) \in G\}
$
and $m : \Theta \to G$ be the restriction of $h$ to $\Theta$. Then:
(1) $\Theta$ is open in $G \times G$ and $m$ is analytic.
(2) $x \in G$ implies $(0, x) \in \Theta$, $(x, 0) \in \Theta$ and $m(0, x) = m(x, 0) = x$.
(3) $x \in G$ implies $-x \in G$, $(x, -x) \in \Theta$, $(-x, x) \in \Theta$ and

$$
m(x, -x) = m(-x, x) = 0.
$$

(4) Let x, y, z be elements of G such that (x, y) ∈ Θ, (m(x, y), z) ∈ Θ, (y, z) ∈ Θ and (x, m(y, z)) ∈ Θ. Then m(m(x, y), z) = m(x, m(y, z)).

*In other words (Chapter III, § 1), if we write −x = σ(x), the quadruple (G, 0, σ, m) is a Lie group germ over K.*

### 3. Exponential in Complete Normed Associative Algebras

In this no. we denote by A a complete normed unital associative algebra (General Topology, Chapter IX, § 3, no. 7). Then \|x.y\| ≤ \|x\|. \|y\| for x, y in A.

Let I be a finite set and let $ \hat{P}(A^I; A) $ be the vector space of formal power series with continuous components on $ A^I $ with values in A (Differentiable and Analytic Manifolds, R, Appendix, no. 5) with the algebra structure obtained by writing

$$
f.g = m \circ (f, g) \quad \text{for } f, g \text{ in } \hat{P}(A^I; A),
$$

where $ m : A \times A \to A $ denotes multiplication on A. Arguing as in no. 1 and using Proposition 1 of § 5, no. 1, we define a continuous homomorphism of unital algebras $ u \mapsto \tilde{u} $ of $ \hat{A}(I) $ into $ \hat{P}(A^I; A) $ mapping the indeterminate of index i to $ pr_i $; this homomorphism extends the Lie algebra homomorphism of $ \hat{L}(I) $ into $ \hat{P}(A^I; A) $ defined in no. 1. If $ u = \sum_v u_v $ with $ u_v \in A^v(I) $ for $ v \in \mathbf{N}^I $, then $ \tilde{u} = \sum_v \tilde{u}_v $, where $ \tilde{u}_v $ is the polynomial mapping $ (t_i)_{i \in I} \mapsto u_v((t_i)) $.

Let $ u = (u_j)_{j \in I} $ be a finite family of elements of $ \hat{A}(I) $, let $ v \in \hat{A}(J) $ and write $ w = v \circ u $ (\S 5, no. 1). Then

$$
(v \circ u)^{\sim} = \tilde{v} \circ \tilde{u}.
$$

This follows by extending by continuity formula (2) of § 5, no. 1 and from Differentiable and Analytic Manifolds, R, Appendix, no. 6.

In particular we take I = {U}, identify A and $ A^{(U)} $ and consider the images $ \tilde{e} $ and $ \tilde{l} $ of the series $ e(U) = \sum_{n \geq 1} U^n/n! $ and $ l(U) = \sum_{n \geq 1} (-1)^{n-1} U^n/n $ in $ \hat{P}(A; A) $. Then $ \|\tilde{U}^n\| \leq 1 $ for $ \|x_1 \ldots x_n\| \leq \|x_1\| \ldots \|x_n\| $ for $ x_1, \ldots, x_n $ in A. Therefore the radius of absolute convergence of $ \tilde{e} $ (resp. $ \tilde{l} $) is infinite (resp. $ \geq 1 $).

We shall denote by $ e_A $ (resp. $ l_A $) the analytic mapping of A into A (resp. of B into A, where B is the open unit ball of A) defined by the convergent series $ \tilde{e} $ (resp. $ \tilde{l} $) and we shall write $ \exp_A(x) = 1 + e_A(x) $ (for $ x \in A $) and

$$
\log_A(x) = l_A(x - 1)
$$

(for $ x \in A, \|x - 1\| < 1 $). Then

$$
\exp_A x = \sum_{n \geq 0} \frac{x^n}{n!} \quad (x \in A)
$$

(20)    $ \log_A x = \sum_{n \geq 1} (-1)^{n-1} \frac{(x-1)^n}{n} \quad (x \in A, \|x-1\| < 1). $

As $ (e \circ l)(U) = (l \circ e)(U) = U $ (cf. § 6, no. 1), by (18) $ \tilde{e} \circ \tilde{l} = \tilde{l} \circ \tilde{e} = \mathrm{Id}_A $.
Therefore (*Differentiable and Analytic Manifolds*, R, 3.1.9)
(21)    $ \exp_A(\log_A(x)) = x \quad (x \in A, \|x-1\| \leq 1) $
(22)    $ \log_A(\exp_A(x)) = x \quad (x \in A, \|x\| < \log 2) $
for $ \|x\| < \log 2 $ implies $ \|\exp_A(x) - 1\| \leq \exp \|x\| - 1 < 1 $.

Finally we consider A as a complete normed Lie algebra. Then
$$
\|[x, y]\| = \|xy - yx\| \leq 2\|x\|\cdot\|y\|.
$$
Proposition 1 of no. 2 implies that the domain of absolute convergence of the formal power series $ \tilde{H} $ contains the set
$$
\Omega = \{x, y) \in A \times A \mid \|x\| + \|y\| < \frac{1}{2} \log 2\}.
$$
Hence $ \tilde{H} $ defines an analytic function $ h : \Omega \to A $. Then $ h(x, y) = \sum_{r,s} H_{r,s}(x, y) $ (cf. § 3, no. 1, *Remark 4*).

#### Proposition 3 {#lie-ii-s7-prop-3 .statement}

*For $ \|x\| + \|y\| < \frac{1}{2} \log 2 $,*
(23)    $ \exp_A x \cdot \exp_A y = \exp_A h(x, y). $
It follows from (18) and the relation $ e^u e^v = e^{u+v} $ that
$$
m \circ (1 + \tilde{e}, 1 + \tilde{e}) = (1 + \tilde{e}) \circ \tilde{H}
$$
in $ \hat{P}(A \times A; A) $. We therefore deduce from *Differentiable and Analytic Manifolds*, R, 3.1.9 that (23) is true for $ (x, y) $ sufficiently close to $ (0, 0) $, whence the proposition follows by analytic continuation (*Differentiable and Analytic Manifolds*, R, 3.2.5).

### Exercises {#lie-ii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
