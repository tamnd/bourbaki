---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 5
section_title: Formal calculations in Lie groups
lang: en
source: lie-i-iii
pdf_pages: 0315-0322, 0400-0401
extraction: ocr
subsections:
    - "no": 1
      title: THE COEFFICIENTS $ c_{\alpha \beta \gamma} $
      page: 0
      pdf_page: 315
    - "no": 2
      title: BRACKET IN THE LIE ALGEBRA
      page: 0
      pdf_page: 316
    - "no": 3
      title: POWERS
      page: 0
      pdf_page: 318
    - "no": 4
      title: EXPONENTIAL
      page: 0
      pdf_page: 321
statements: 5
exercises: 2
content_sha256: 3be8a17f6cc0964c47197ceb7a5dc79874139b28c957259aef32433c6ca556fd
---

## § 5. FORMAL CALCULATIONS IN LIE GROUPS

Let $ f, g $ be two formal power series with coefficients in $ K $ in the same indeterminates, let $ f_i $ (resp. $ g_i $) be the homogeneous component of $ f $ (resp. $ g $) of degree $ i $. We shall write
$$
f \equiv g \mod \deg p
$$
if $ f_i = g_i $ for $ i < p $.

In this §, G denotes a Lie group germ of finite dimension $ n $; the base field $ K $ is assumed to be of characteristic zero. We identify once and for all, by means of a chart, an open neighbourhood of $ e $ in G with an open neighbourhood U of 0 in $ K^n $, so that $ e $ is identified with 0. For $ x, y $ in U and $ n \in \mathbf{Z} $, $ x.y $ denotes the product of $ x $ and $ y $ and $ x^{[m]} $ the m-th power of $ x $ in G (when they are defined). The coordinates of $ x \in U $ are denoted by $ x_1, x_2, \ldots, x_n $.

### 1. THE COEFFICIENTS $ c_{\alpha \beta \gamma} $

Let $ \Omega $ be the set of $ (x, y) \in U \times U $ such that $ x.y $ is defined and belongs to U. Then $ \Omega $ is open in $ U \times U $ and the mapping $ (x, y) \mapsto x.y $ of $ \Omega $ into U is analytic. The coordinates $ z_1, \ldots, z_n $ of $ z = x.y $ therefore admit expansions as integral series about the origin in the powers of $ x_1, \ldots, x_n, y_1, \ldots, y_n $. Therefore, there exist well defined constants $ c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} \in K $, such that
$$
z_1^{\gamma_1} \cdots z_n^{\gamma_n} = \sum_{\alpha_1, \ldots, \beta_n \in \mathbf{N}} c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} x_1^{\alpha_1} \cdots x_n^{\alpha_n} y_1^{\beta_1} \cdots y_n^{\beta_n}
$$
for $ \gamma_1, \ldots, \gamma_n $ in $ \mathbf{N} $. Adopting the conventions of Differentiable and Analytic Manifolds, R, we shall write these formulae more briefly:
$$
(x.y)^{\gamma} = \sum_{\alpha, \beta \in \mathbf{N}^n} c_{\alpha, \beta, \gamma} x^{\alpha} y^{\beta} \quad (\gamma \in \mathbf{N}^n).
$$
Since $ x.0 = 0.x = x $ for $ x \in U $,
$$
c_{\alpha, 0, \gamma} = c_{0, \alpha, \gamma} = \delta_{\alpha \gamma}
$$
where $ \delta_{\alpha \gamma} $ is the Kronecker index. In particular, writing henceforth $ k $ instead of $ \varepsilon_k $ for $ k = 1, \ldots, n $,
$$
(x.y)_k = x_k + y_k + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha, \beta, k} x^{\alpha} y^{\beta}.
$$
Writing $ c_{\alpha \beta} = (c_{\alpha \beta 1}, c_{\alpha \beta 2}, \ldots, c_{\alpha \beta n}) \in K^n $, it then follows that
$$
x.y = x + y + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta} x^{\alpha} y^{\beta}.
$$

On the right hand side of (5), we consider the homogeneous component of degree 2:

$$
B(x, y) = \sum_{i,j=1}^n c_{ij} x_i y_j
$$

so that $(x, y) \mapsto B(x, y)$ is a bilinear mapping of $K^n \times K^n$ into $K^n$. Then

(6)
$$
x.y \equiv x + y + B(x, y) \mod \deg 3.
$$

Formula (4) implies on the other hand that

(7)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{if } |\alpha| + |\beta| < |\gamma|
$$

and that the terms of total degree $|\gamma|$ in the expansion of $z^\gamma$ are also those of $(x_1 + y_1)^{\gamma_1}(x_2 + y_2)^{\gamma_2} \ldots (x_n + y_n)^{\gamma_n} = \sum_{\alpha + \beta = \gamma} ((\alpha, \beta)) x^\alpha y^\beta$ (cf. *Differentiable and Analytic Manifolds*, R, Notation and conventions). Hence:

(8)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{if } |\alpha| + |\beta| = |\gamma| \quad \text{but } \alpha + \beta \neq \gamma
$$
(9)
$$
c_{\alpha, \beta, \alpha + \beta} = ((\alpha, \beta)).
$$

The associativity of the product implies the relation
$$
\sum_{\xi} c_{\alpha \xi n} x^\alpha \left( \sum_{\beta, \gamma} c_{\beta \gamma \xi} y^\beta z^\gamma \right) = \sum_{\xi, \gamma} c_{\xi \gamma n} \left( \sum_{\alpha, \beta} c_{\alpha \beta \xi} x^\alpha y^\beta \right) z^\gamma
$$
for all $x, y, z$ sufficiently close to 0, whence

(10)
$$
\sum_{\xi} c_{\alpha \xi n} c_{\beta \gamma \xi} = \sum_{\xi} c_{\xi \gamma n} c_{\alpha \beta \xi} \quad (\alpha, \beta, \gamma, \eta \text{ in } \mathbf{N}^n).
$$

The group germ G admits a commutative open subgroup germ if and only if $c_{\alpha \beta \gamma} = c_{\beta \alpha \gamma}$ for all $\alpha, \beta, \gamma$ in $\mathbf{N}^n$.

### 2. BRACKET IN THE LIE ALGEBRA

For $\alpha \in \mathbf{N}^n$, let $e_\alpha$ be the point distribution $\frac{1}{\alpha!} \frac{\partial^\alpha}{\partial x^\alpha}$ at the origin. In particular,
$$
e_k = e_{e_k} = \frac{\partial}{\partial x_k}.
$$
The $e_\alpha$ form a basis of the vector space $U(G)$. If $f$ is an analytic function on an open neighbourhood of 0 in G and $f(x) = \sum \lambda_\alpha x^\alpha$ is its expansion as an integral series about the origin, then
$$
\langle e_\alpha, f \rangle = \lambda_\alpha.
$$
In particular,
$$
\langle e_\alpha, x^\gamma \rangle = \delta_{\alpha \gamma}.
$$

Hence
$$
\langle e_\alpha * e_\beta, x^\gamma \rangle = \langle e_\alpha \otimes e_\beta, (x.y)^\gamma \rangle \\
= \langle e_\alpha \otimes e_\beta, \sum_{\alpha', \beta'} c_{\alpha'\beta'\gamma} x^{\alpha'} y^{\beta'} \rangle \\
= \sum_{\alpha', \beta'} c_{\alpha'\beta'\gamma} \langle e_\alpha, x^{\alpha'} \rangle \langle e_\beta, y^{\beta'} \rangle = c_{\alpha\beta\gamma}
$$
and hence
$$
e_\alpha * e_\beta = \sum_\gamma c_{\alpha\beta\gamma} e_\gamma.
$$
(Formula (10) then expresses associativity on $ U(G) $.)
In particular, since $ L(G) $ is stable under the bracket.
$$
[e_i, e_j] = \sum_k (c_{ijk} - c_{jik}) e_k.
$$
The constants of structure of $ L(G) $ relative to the basis $ (e_1, \ldots, e_n) $ are therefore the $ c_{ijk} - c_{jik} $. In other words, canonically identifying $ L(G) $ with $ K^n $, we obtain:
$$
[x, y] = B(x, y) - B(y, x).
$$

#### Proposition 1 {#lie-iii-s5-prop-1 .statement}

(i) $$ x^{[-1]} \equiv -x + B(x, x) \mod \deg 3 $$
(ii) $$ x.y.x^{[-1]} \equiv y + [x, y] \mod \deg 3 $$
(iii) $$ y^{[-1]}.x.y \equiv x + [x, y] \mod \deg 3 $$
(iv) $$ x^{[-1]}.y^{[-1]}.x.y \equiv [x, y] \mod \deg 3 $$
(v) $$ x.y.x^{[-1]}.y^{[-1]} \equiv [x, y] \mod \deg 3. $$
(In (i), $ x^{[-1]} $ of course represents the expansion of the function $ x \mapsto x^{[-1]} $ as an integral series about the origin; the other formulae can be interpreted analogously.)
Let $ g_1 $ and $ g_2 $ be the homogeneous components of $ x^{[-1]} $ of degrees 1 and 2. Then
$$
0 = x.x^{[-1]} \\
\equiv x + g_1(x) + B(x, g_1(x)) \mod \deg 2 \quad \text{(by (6))} \\
\equiv x + g_1(x) \mod \deg 2
$$
and hence $ g_1(x) = -x $. Then
$$
0 = x.x^{[-1]} \\
\equiv x + (-x + g_2(x)) + B(x, -x + g_2(x)) \mod \deg 3 \\
\equiv g_2(x) - B(x, x) \mod \deg 3
$$

and hence $ g_2(x) = B(x, x) $. This proves (i). Then, using (i),
$$
x.y.x^{[-1]} \equiv (x + y + B(x, y)).(-x + B(x, x)) \quad \text{mod deg 3}
$$
$$
\equiv x + y + B(x, y) + (-x + B(x, x)) + B(x + y, -x) \quad \text{mod deg 3}
$$
$$
\equiv y + B(x, y) - B(y, x) \quad \text{mod deg 3}
$$
$$
\equiv y + [x, y] \quad \text{mod deg 3 (by (13))}
$$
whence (ii). The proof of (iii) is analogous. Combining (i) and (iii), we obtain
$$
x^{[-1]},y^{[-1]}.x.y \equiv (-x + B(x, x)).(x + [x, y]) \quad \text{mod deg 3}
$$
$$
\equiv -x + B(x, x) + x + [x, y] + B(-x, x) \quad \text{mod deg 3}
$$
$$
\equiv [x, y] \quad \text{mod deg 3}
$$
whence (iv). The proof of (v) is analogous.

### 3. POWERS

Consider j points of G:
$$
x(1) = (x(1)_1, x(1)_2, \ldots, x(1)_n)
$$
$$
x(2) = (x(2)_1, x(2)_2, \ldots, x(2)_n)
$$
$$
\ldots \ldots \ldots \ldots \ldots \ldots \ldots
$$
$$
x(j) = (x(j)_1, x(j)_2, \ldots, x(j)_n).
$$
The mapping $(x(1), x(2), \ldots, x(j)) \mapsto x(1).x(2)\ldots x(j)$ admits an expansion as an integral series about the origin:

$$
x(1).x(2)\ldots x(j) = \sum_{\alpha(1), \alpha(2), \ldots, \alpha(j) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(j)} x(1)^{\alpha(1)} \ldots x(j)^{\alpha(j)}
$$

where the $a_{\alpha(1), \ldots, \alpha(j)}$ are elements of $\mathbf{K}^n$. We write, for $j = 0, 1, 2, \ldots$,

$$
\psi_j(x) = \sum_{\alpha(1) \neq 0, \ldots, \alpha(j) \neq 0} a_{\alpha(1), \ldots, \alpha(j)} x^{\alpha(1) + \ldots + \alpha(j)}
$$

where the right hand side is a convergent integral series in the variable $x \in \mathbf{K}^n$. This series is obtained by suppressing in (14) the terms in which one of the variables $x(1), \ldots, x(j)$ does not occur explicitly and then writing $x(1) = x(2) = \cdots = x(j) = x$.

If $t \in \mathbf{K}$, all the t-th power mappings of G have the same expansion as an integral series about the origin, since any two of them coincide on a neighbourhood of 0. We denote this expansion as an integral series by $x^{[t]}$.

#### Proposition 2 {#lie-iii-s5-prop-2 .statement}

(i) $\psi_j \equiv 0 \mod \deg j$.
(ii) *If $t \in \mathbf{K}$, then*
$$
x^{[t]} = \sum_{i=1}^8 \binom{t}{i} \psi_i(x)
$$
*where the formal power series on the right is meaningful because of (i).*

(We write

$$
\binom{t}{i} = \frac{t(t-1)\ldots(t-i+1)}{i!}
$$

for all $ t \in \mathbf{K} $.)

Assertion (i) is obvious from the definition of the $ \psi_j $.

We prove (ii) for $ t $ an integer $ \geq 0 $. By (14),

$$
x^{[t]} = \sum_{\alpha(1), \ldots, \alpha(t) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \ldots + \alpha(t)}.
$$

For $ \alpha = (\alpha(1), \ldots, \alpha(t)) \in (\mathbf{N}^n)^t $, let $ \sigma(\alpha) $ denote the set of $ j \in \{1, 2, \ldots, t\} $ such that $ \alpha(j) \neq 0 $. If, in the sum (17), we group together the terms for which $ \sigma(\alpha) $ is the same, then

$$
x^{[t]} = \sum_{\sigma \subset \{1, t\}} h_{t, \sigma}(x)
$$

where

$$
h_{t, \sigma}(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \ldots + \alpha(t)}.
$$

Let $ \sigma = \{j_1, j_2, \ldots, j_q\} $ with $ j_1 < j_2 < \ldots < j_q $. In (14) (where $ j $ is replaced by $ t $), we substitute 0 for $ x(k) $ for $ k \notin \sigma $; as 0 is the identity element of $ G $, we obtain the expansion of $ x(j_1) \cdot x(j_2) \ldots x(j_q) $ as an integral series about the origin:

$$
x(j_1) \cdot x(j_2) \ldots x(j_q) = \sum_{\sigma(\alpha) \subset \sigma} a_{\alpha(1), \ldots, \alpha(t)} x(j_1)^{\alpha(j_1)} x(j_2)^{\alpha(j_2)} \ldots x(j_q)^{\alpha(j_q)}
$$

and hence, by the definition of $ \psi_q $:

$$
\psi_q(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(j_1) + \ldots + \alpha(j_q)}.
$$

By (19) and (20), we see that $ h_{t, \sigma}(x) = \psi_{\mathrm{card}\,\sigma}(x) $. Then (18) implies

$$
x^{[t]} = \sum_{i=0}^t \binom{t}{i} \psi_i(x) = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x).
$$

Then we write $ x^{[t]'} = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x) $ for all $ t \in \mathbf{K} $. In the integral series $ x^{[t]} $ and $ x^{[t]'} $, each coefficient is a polynomial function of $ t $. For this is obvious for $ x^{[t]'} $. As far as $ x^{[t]} $ is concerned, it suffices to prove that, for all $ u \in \mathrm{U}(G) $, the image of $ u $ under $ x \mapsto x^{[t]} $ is a polynomial function of $ t $. Now, for $ u \in \mathrm{U}^m(G) $, this image is $ t^m u $ (\S 4, no. 3, Proposition 7 (iv)).

As $ x^{[t]} = x^{[t]'} $ for $ t $ an integer $ \geq 0 $, it then follows that $ x^{[t]} = x^{[t]'} $ for all $ t \in \mathbf{K} $.

#### Remark {#lie-iii-s5-n3-rem-1 .statement}

(1) We write condition (ii) of Proposition 2 for t an integer $ \geqslant 0 $:

$$
\begin{align*}
0 &= \psi_0(x) \\
x &= \psi_0(x) + \psi_1(x) \\
x^{[2]} &= \psi_0(x) + 2\psi_1(x) + \psi_2(x) \\
&\ldots \ldots \ldots \ldots \ldots \ldots \ldots
\end{align*}
$$

These formulae suffice to determine the $ \psi_i $.

(2) We see that $ \psi_0(x) = 0, \psi_1(x) = x, \psi_2(x) = x^{[2]} - 2x $,

$$
x^{[-1]} = \sum_{i=1}^\infty (-1)^i \psi_i(x).
$$

(3) The above expression for $ \psi_2 $ and formula (6) prove that

$$
\psi_2(x) \equiv \mathrm{B}(x, x) \mod \deg 3.
$$
Using Proposition 2, (i) and (ii), we see that

$$
x^{[t]} \equiv tx + \binom{t}{2} \mathrm{B}(x, x) \mod \deg 3.
$$

(4) Let $ \psi_{p,m}(x) $ and $ h_{t,m}(x) $ denote the homogeneous components of $ \psi_p(x) $ and $ x^{[t]} $ of degree m. Then $ \psi_{p,m} = 0 $ for $ m < p $. On the other hand, Proposition 2 (ii) gives

$$
h_{t,m}(x) = \sum_{p \leq m} \frac{t(t-1)\ldots(t-p+1)}{p!} \psi_{p,m}(x)
$$
that is

$$
h_{t,m}(x) = \sum_{1 \leq r \leq m} t^r \phi_{r,m}(x)
$$
where the $ \phi_{r,m} $ are homogeneous polynomial mappings of degree m of $ \mathbf{K}^n $ into $ \mathbf{K}^n $. In particular, by (23),

$$
\phi_{1,m}(x) = \sum_{p \leq m} \frac{(-1)^{p-1}}{p} \psi_{p,m}(x)
$$
$$
\phi_{m,m}(x) = \frac{1}{m!} \psi_{m,m}(x).
$$

(5) If $ \mathbf{K} $ is of characteristic $ > 0 $, the results of nos. 1 and 2 remain true, provided $ e_\alpha $, in no. 2, is defined by $ \langle e_\alpha, \sum_\beta \lambda_\beta x^\beta \rangle = \lambda_\alpha $. In no. 3, if the $ \psi_j $ are defined as above, the argument again proves that $ x^{[t]} = \sum_{i=1}^\infty \binom{t}{i} \psi_i(x) $ if $ t \in \mathbf{N} $.

### 4. EXPONENTIAL

Let $ E(x) $ be the expansion of an exponential mapping of $ G $ as an integral series about 0. Let $ L(x) $ be the expansion of the inverse mapping of an injective exponential mapping of $ G $ as an integral series about 0. Since the tangent mapping at 0 to any exponential mapping is the identity of $ L(G) $, $ E(x) \equiv x \mod \deg 2 $ and $ L(x) \equiv x \mod \deg 2 $. Since $ E(L(x)) = L(E(x)) $ for $ x $ sufficiently close to 0, the formal power series $ E $ and $ L $ are such that $ E(L(X)) = L(E(X)) = X $. An analogous argument shows that
$$
E(tX) = (E(X))^{[t]}, \quad L(X^{[t]}) = tL(X)
$$
for $ t \in K $.

#### Proposition 3 {#lie-iii-s5-prop-3 .statement}

(27)
$$
L = \sum_{p=1}^{\infty} \frac{(-1)^{p-1}}{p} \psi_p
$$
(28)
$$
E = \sum_{p=1}^{\infty} \frac{1}{p!} \psi_{p,p}
$$
(Recall that $ \psi_{p,p} $ is the homogeneous component of $ \psi_p $ of degree $ p $.)

or, by (24),
$$
E(tx) = (E(x))^{[t]}
$$

The two sides are formal power series in $ t $ and $ x $. Equating the terms of first degree in $ t $, we obtain
$$
x = \sum_{m \geq 0} \phi_{1,m}(E(x)).
$$
Now the inversion of a system of formal power series, when it is possible, is possible in only one way (Algebra, Chapter IV, § 6, Corollary to Proposition 8). Then
$$
L(x) = \sum_{m \geq 0} \phi_{1,m}(x) \quad \text{by (29)}
$$
$$
= \sum_{p,m} \frac{(-1)^p}{p} \psi_{p,m}(x) \quad \text{by (25)}
$$
$$
= \sum_p \frac{(-1)^p}{p} \psi_p(x),
$$
whence (i). Similarly, for $ t \neq 0 $,
$$
L(tx) = tL((tx)^{[t^{-1}]})
$$
$$
= tL\left( \sum_{m \geq 0} \sum_{1 \leq r \leq m} t^{m-r} \phi_{r,m}(x) \right) \quad \text{by (24)}.
$$

Equating the terms of first degree in t, we obtain

$$
x = L \left( \sum_{m \geq 0} \phi_{m,m}(x) \right)
$$

whence

$$
E(x) = \sum_{m \geq 0} \phi_{m,m}(x)
$$
$$
= \sum_{m \geq 0} \frac{1}{m!} \psi_{m,m}(x) \quad \text{by (26).}
$$

#### Proposition 4 {#lie-iii-s5-prop-4 .statement}

*For the chart of G used to be canonical, it is necessary and sufficient that $ \psi_j = 0 $ for $ j \geq 2 $.*

This is sufficient by Proposition 3. Suppose that the chart is canonical and that $ \psi_i = 0 $ for $ 2 \leq i < n $. Then $ nx = x^{[n]} = \sum_{i=0}^n \binom{n}{i} \psi_i(x) = nx + \psi_n(x) $, whence $ \psi_n = 0 $. Hence $ \psi_j = 0 $ for $ j \geq 2 $ by induction on $ j $.

### Exercises {#lie-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
