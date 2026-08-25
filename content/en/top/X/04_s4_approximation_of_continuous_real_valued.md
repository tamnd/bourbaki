---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 4
section_title: Approximation of continuous real-valued functions
lang: en
source: top-v-x
pdf_pages: 0314-0323, 0343-0352
extraction: ocr
subsections:
    - "no": 1
      title: APPROXIMATION OF CONTINUOUS FUNCTIONS BY FUNCTIONS BELONGING TO A LATTICE
      page: 0
      pdf_page: 314
    - "no": 2
      title: APPROXIMATION OF CONTINUOUS FUNCTIONS BY POLYNOMIALS
      page: 0
      pdf_page: 317
    - "no": 3
      title: 'APPLICATION : APPROXIMATION OF CONTINUOUS REAL-VALUED FUNCTIONS DEFINED ON A PRODUCT OF COMPACT SPACES'
      page: 0
      pdf_page: 320
    - "no": 4
      title: APPROXIMATION OF CONTINUOUS MAPPINGS OF A COMPACT SPACE INTO A NORMED SPACE
      page: 0
      pdf_page: 320
statements: 18
exercises: 5
content_sha256: e1f48f0eea3cb2695064b08242793cda7fbea618354ff2ab03b050d4fdbb35fc
---

## 4. APPROXIMATION OF CONTINUOUS REAL-VALUED FUNCTIONS

### 1. APPROXIMATION OF CONTINUOUS FUNCTIONS BY FUNCTIONS BELONGING TO A LATTICE

In this section we shall study the set $\mathcal{C} = C(X; \mathbf{R})$ of continuous real-valued functions (*) defined on a *compact* space $X$, and we shall always suppose that $\mathcal{C}$ is endowed with the topology of *uniform convergence*. From § 3, no. 2 we know that this topology is defined by the norm

$$
||f|| = \sup_{x \in X} |f(x)|
$$

and that this norm is compatible with the $\mathbf{R}$-algebra structure of $\mathcal{C}$. With this norm and this algebra structure, $\mathcal{C}$ is a *complete normed algebra* over $\mathbf{R}$ ($\S 1$, no. 6, Theorem 2, Corollary 1).

(*) The real-valued functions under consideration in this section are assumed always to be *finite*.

If $H$ is a subset of $\mathcal{C}$, we shall say that a continuous real-valued function $f$ on $X$ can be uniformly approximated by functions of $H$ if $f$ lies in the closure of $H$ in the space $\mathcal{C}$, i.e. if, for each $\varepsilon > 0$, there exists a function $g \in H$ such that $|f(x) - g(x)| \leq \varepsilon$ for all $x \in X$. To say that every continuous real-valued function on $X$ can be uniformly approximated by functions of $H$ therefore means that $H$ is dense in $\mathcal{C}$.

On the set $\mathcal{C}$, the relation $f \leq g$ [which means that $f(x) \leq g(x)$ for all $x \in X$] is an order relation, with respect to which $\mathcal{C}$ is a lattice. Clearly we have $|||u| - |v||| \leq ||u - v||$, and therefore $u \to |u|$ is a uniformly continuous mapping of $\mathcal{C}$ into itself. It follows that

$$
(u, v) \to \sup (u, v) = \frac{1}{2}(u + v + |u - v|)
$$

and

$$
(u, v) \to \inf (u, v) = \frac{1}{2}(u + v - |u - v|)
$$

are uniformly continuous on $\mathcal{C} \times \mathcal{C}$.

PROPOSITION I. Let $X$ be a compact space and let $H$ be a set of continuous real-valued functions defined on $X$. Let $f$ be a continuous real-valued function on $X$ such that for each $x \in X$ there exists a function $u_x \in H$ such that $u_x(x) > f(x)$ [resp. $u_x(x) < f(x)$]. Then there exists a finite number of functions $u_{x_i} = f_i \in H$ ($1 \leq i \leq n$) such that, if $v = \sup(f_1, f_2, \ldots, f_n)$ [resp. $w = \inf(f_1, f_2, \ldots, f_n)$], we have $v(x) > f(x)$ [resp. $w(x) < f(x)$] for all $x \in X$.

For each $x \in X$, let $G_x$ be the open set consisting of all $z \in X$ such that $u_x(z) > f(z)$ [resp. $u_x(z) < f(z)$]. Since $x \in G_x$ by hypothesis, $X$ is the union of the sets $G_x$ as $x$ runs through $X$. Since $X$ is compact there exists a finite number of points $x_i$ ($1 \leq i \leq n$) such that the $G_{x_i}$ cover $X$, and it is clear that the functions $f_i = u_{x_i}$ satisfy the conditions of the proposition.

THEOREM I (Dini). Let $X$ be a compact space, and let $H$ be a set of continuous real-valued functions on $X$ which is directed with respect to the relation $\leq$ (resp. $\geq$). If the upper (resp. lower) envelope $f$ of $H$ is finite and continuous on $X$, then $f$ can be uniformly approximated by functions belonging to $H$ (or, equivalently, the section filter of $H$ converges uniformly to $f$ in $X$).

Given any $\varepsilon > 0$, for each $x \in X$ there exists a function $u_x \in H$ such that $u_x(x) > f(x) - \varepsilon$. By Proposition I and the fact that $H$ is directed with respect to the relation $\leq$, there exists $g \in H$ such that $g(x) > f(x) - \varepsilon$ for all $x \in X$; on the other hand, we have $g(x) \leq f(x)$ by definition, and therefore the theorem is proved.

#### Corollary {#top-x-s4-n1-cor-1 .statement}

Let $(u_n)$ be an increasing (resp. decreasing) sequence of continuous real-valued functions on $X$. If the upper (resp. lower) envelope $f$ of the sequence $(u_n)$ is finite and continuous on $X$, then the sequence $(u_n)$ converges uniformly to $f$ in $X$.

It is clear that the conclusion of Theorem 1 is no longer necessarily valid if $X$ is no longer assumed to be compact, as is shown by the example of the decreasing sequence of functions $x/(n + x)$ in $\mathbf{R}_+$.

#### Proposition 2 {#top-x-s4-prop-2 .statement}

Let $X$ be a compact space, and let $H$ be a set of continuous real-valued functions on $X$ such that, given any two functions $u \in H, v \in H$, the functions $\sup(u, v)$ and $\inf(u, v)$ are in $H$. Then a continuous real-valued function $f$ on $X$ can be uniformly approximated by functions belonging to $H$ if and only if, for each real number $\varepsilon > 0$ and each pair $x, y$ of points of $X$, there is a function $u_{x, y} \in H$ such that $|f(x) - u_{x, y}(x)| < \varepsilon$ and $|f(y) - u_{x, y}(y)| < \varepsilon$.

The condition is clearly necessary; let us show that it is sufficient. For each $\varepsilon > 0$, we shall show that there is a function $g \in H$ such that $|f(z) - g(z)| < \varepsilon$ for all $z \in X$. Let $x$ be any point of $X$, and let $H_x$ be the set of all functions $u \in H$ such that $u(x) < f(x) + \varepsilon$. By hypothesis, for each $y \in X$, the function $u_{x, y}$ belongs to $H_x$ and we have $u_{x, y}(y) > f(y) - \varepsilon$. Hence, by Proposition 1, there is a finite number of functions of $H_x$ whose upper envelope $v_x$ is such that $v_x(z) > f(z) - \varepsilon$ for all $z \in X$; on the other hand, we have $v_x(x) < f(x) + \varepsilon$ by the definition of $H_x$; finally, $v_x \in H$ by hypothesis. Proposition 1 therefore shows that there exists a finite number of functions $v_{x_i}$ whose lower envelope $g$ is such that $g(z) < f(z) + \varepsilon$ for all $z \in X$; but since we have $v_{x_i}(z) > f(z) - \varepsilon$ for all $z \in X$ and for every index $i$, we have also $g(z) > f(z) - \varepsilon$ for all $z \in X$. Since $g \in H$ by hypothesis, the proof is complete.

#### Remark {#top-x-s4-n1-rem-1 .statement}

When the set $H$ satisfies the conditions of Proposition 2, it is a lattice with respect to the ordering $f \leq g$. But it should be remarked that a subset $H$ of $C$ can be a lattice with respect to this ordering without it being necessarily the case that the least upper bound (resp. greatest lower bound) in $H$ of two functions $u, v$ of $H$ is the same as their least upper bound (resp. greatest lower bound) in $C$. \* An example is provided by the convex mappings of a compact interval of $\mathbf{R}$ into $\mathbf{R}$. \*

#### Corollary {#top-x-s4-n1-cor-2 .statement}

Suppose that $H$ is such that, whenever $u \in H$ and $v \in H$, we have $\sup(u, v) \in H$ and $\inf(u, v) \in H$; and is such that, given any two distinct points $x, y$ of $X$ and any two real numbers $\alpha, \beta$, there is a function $g \in H$ such that $g(x) = \alpha$ and $g(y) = \beta$. Then every continuous real-valued function on $X$ can be uniformly approximated by functions belonging to $H$.

#### Definition 1 {#top-x-s4-def-1 .statement}

*If X is any set, a set H of mappings of X into a set Y is said to separate the elements of a subset A of X (or to be a separating set for the elements of A) if, given any two distinct elements x, y of A, there is a function f ∈ H such that f(x) ≠ f(y).*

For example, if X is a completely regular space (Chapter IX, § 1, no. 5) then the set of all continuous mappings of X into [0, 1] separates the points of X.

#### Theorem 2 (Stone) {#top-x-s4-thm-2 .statement}

*Let X be a compact space, and let H be a vector subspace of $\mathcal{C}(X; \mathbf{R})$ such that 1) the constant functions belong to H; 2) if $u \in H$, then $|u| \in H$; 3) H separates the points of X. Then every continuous real-valued function on X can be uniformly approximated by functions of H.*

It is enough to show that H satisfies the conditions of the Corollary to Proposition 2. By hypothesis, if $u \in H$ and $v \in H$, we have

$$
\sup (u, v) = \frac{1}{2} (u + v + |u - v|) \in H
$$
and
$$
\inf (u, v) = \frac{1}{2} (u + v - |u - v|) \in H.
$$

On the other hand, let x and y be any two distinct points of X, and let α, β be any two real numbers. By hypothesis, there is a function $h \in H$ such that $h(x) \neq h(y)$: say $h(x) = \gamma$ and $h(y) = \delta$. Since the constants belong to H, the function
$$
g(z) = \alpha + (\beta - \alpha) \frac{h(z) - \gamma}{\delta - \gamma}
$$
belongs to H and is such that $g(x) = \alpha$ and $g(y) = \beta$.

### 2. APPROXIMATION OF CONTINUOUS FUNCTIONS BY POLYNOMIALS

Given a set H of real-valued functions defined on a set X, we say that a real-valued function defined on X is a polynomial (resp. a polynomial with no constant term) with real coefficients, in the functions of H, if it is of the form $x \to g(f_1(x), f_2(x), \ldots, f_n(x))$ where g is a polynomial (resp. a polynomial with no constant term) in n indeterminates (n arbitrary) with real coefficients, and the $f_i$ ($1 \leq i \leq n$) belong to H.

#### Theorem 3 (Weierstrass-Stone) {#top-x-s4-thm-3 .statement}

*Let X be a compact space and let H be a set of continuous real-valued functions on X which separates the points of X. Then every continuous real-valued function on X can be uniformly approximated by polynomials (with real coefficients) in the functions of H.*

An equivalent statement of the theorem is that *any subalgebra of $\mathcal{C}(X; \mathbf{R})$ which contains the constant functions and separates the points of X is dense in $\mathcal{C}(X; \mathbf{R})$*.

Let $H_0$ be the set of all polynomials in the functions of H, and let $\overline{H}_0$ be the closure of $H_0$ in $\mathcal{C}$. If g is any polynomial in n variables with real coefficients, then $(u_1, u_2, \ldots, u_n) \to g(u_1, u_2, \ldots, u_n)$ is a continuous mapping of $\mathcal{C}^n$ into $\mathcal{C}$, which maps $H_0^n$ into $H_0$, and therefore maps $\overline{H}_0^n$ into $\overline{H}_0$ (Chapter I, § 2, no. 1, Theorem 1). In particular, $\overline{H}_0$ is a vector subspace of $\mathcal{C}$ and evidently satisfies the first and third conditions of Theorem 2; we shall show that it also satisfies the second condition, and this will prove that $\overline{H}_0 = \mathcal{C}$.

Since every function $u \in \overline{H}_0$ is bounded in $X$, it is enough to prove the following lemma:

#### Lemma 1 {#top-x-s4-lem-1 .statement}

*For each real number $\varepsilon > 0$ and each compact interval $I \subset \mathbf{R}$ there exists a polynomial $p(t)$ with no constant term such that $|p(t) - |t|| \leq \varepsilon$ for all $t \in I$.*

It is enough to prove the lemma for an interval of the form $I = [-a, +a]$ and hence, replacing $t$ by $at$, for the interval $I = [-1, +1]$. Since $|t| = \sqrt{t^2}$, Lemma 1 is a consequence of the following result:

#### Lemma 2 {#top-x-s4-lem-2 .statement}

*Let $(P_n)$ be the sequence of polynomials without constant terms defined by*
$$
(1) \quad p_0(t) = 0, \quad p_{n+1}(t) = p_n(t) + \frac{1}{2} (t - (p_n(t))^2), \qquad n \geq 0.
$$
*In the interval $[0, 1]$ the sequence $(p_n)$ is increasing and converges uniformly to $\sqrt{t}$.*

To prove Lemma 2 it is enough to show that, for all $t \in [0, 1]$, we have
$$
(2) \qquad 0 \leq \sqrt{t} - p_n(t) \leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}},
$$
for (2) implies that $0 \leq \sqrt{t} - p_n(t) \leq 2/n$.

We prove (2) by induction on $n$. It is true for $n = 0$. If $n \geq 0$ it follows from the inductive hypothesis (2) that $0 \leq \sqrt{t} - p_n(t) \leq \sqrt{t}$, hence $0 \leq p_n(t) \leq \sqrt{t}$, and therefore from (1) we have
$$
\sqrt{t} - p_{n+1}(t) = (\sqrt{t} - p_n(t)) (1 - \frac{1}{2} (\sqrt{t} + p_n(t))),
$$
so that $\sqrt{t} - p_{n+1}(t) \geq 0$, and from (2)
$$
\begin{align*}
\sqrt{t} - p_{n+1}(t) &\leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2} \right) \\
&\leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2 + (n+1) \sqrt{t}} \right) \\
&= \frac{2 \sqrt{t}}{2 + (n+1) \sqrt{t}}.
\end{align*}
$$
Q.E.D.

If $X$ is not compact, the conclusion of Theorem 3 is not necessarily valid. For example, a continuous real-valued function on $\mathbf{R}$ which is bounded and not constant cannot be uniformly approximated in $\mathbf{R}$ by polynomials (cf. Exercise 6).

#### Proposition 3 {#top-x-s4-prop-3 .statement}

*Let* $(K_i)_{i \in I}$ *be a family of compact intervals of* $\mathbf{R}$, $K = \prod_{i \in I} K_i$ *their product*, and let $X$ *be a compact subspace of* $K$. *Then every continuous real-valued function on* $X$ *can be uniformly approximated by polynomials in the coordinates* $x_i = \mathrm{pr}_i x$.

For if $x = (x_i)$ and $y = (y_i)$ are two distinct points of $X$, there is at least one index $i$ such that $x_i \neq y_i$; hence the family of continuous functions $\mathrm{pr}_i$ satisfies the conditions of Theorem 3.

#### Proposition 4 {#top-x-s4-prop-4 .statement}

*Let* $X$ *be a compact space, let* $A$ *be a closed subspace of* $X$, *and let* $H$ *be a set of continuous real-valued functions on* $X$ *which separates the points of* $C_A$ *and is such that* $A$ *is the intersection of the sets* $\overline{u}^{-1}(0)$ *as* $u$ *runs through* $H$. *Then every continuous real-valued function on* $X$ *which is zero on* $A$ *can be uniformly approximated by polynomials without constant terms in the functions of* $H$.

Consider first the particular case in which $A$ consists of a single point $x_0$. The hypotheses then imply that $H$ separates the points of $X$; for, if $x \neq x_0$, then by hypothesis there is a function $u \in H$ such that $u(x) \neq 0 = u(x_0)$. Hence, for each $\varepsilon > 0$ and each continuous real-valued function $f$ on $X$ such that $f(x_0) = 0$, there exists (Theorem 3) a polynomial $g$ in the functions of $H$ such that $|f(x) - g(x)| \leq \varepsilon$ for all $x \in X$. In particular $|g(x_0)| \leq \varepsilon$, so that

$$
|f(x) - (g(x) - g(x_0))| \leq 2\varepsilon
$$

for all $x \in X$; and since $g(x) - g(x_0)$ is a polynomial in the functions of $H$ with no constant term, the result is established in this case.

In the general case, consider the equivalence relation $R$ on $X$ whose classes are the set $A$ and the sets $\{x\}$ for $x \notin A$. The quotient space $X/R$ is Hausdorff (Chapter I, § 8, no. 6, Proposition 15) and therefore compact. Let $\varphi : X \to X/R$ be the canonical mapping. Every continuous real-valued function $f$ on $X$ which vanishes on $A$ can be written in the form $f = f_1 \circ \varphi$, where $f_1$ is a continuous real-valued function on $X/R$ which vanishes at the point $x_0' = \varphi(A)$. Applying the result already proved to the space $X/R$ and the point $x_0'$, we obtain the final result.

### 3. APPLICATION : APPROXIMATION OF CONTINUOUS REAL-VALUED FUNCTIONS DEFINED ON A PRODUCT OF COMPACT SPACES

#### Theorem 4 {#top-x-s4-thm-4 .statement}

Let $(X_i)_{i \in I}$ be a family of compact spaces, and let
$$
X = \prod_{i \in I} X_i.
$$
Then every continuous real-valued function on $X$ can be uniformly approximated by sums of a finite number of functions of the form
$$
(x_i) \to \prod_{\alpha \in J} u_\alpha(x_\alpha),
$$
where $J$ is an (arbitrary) finite subset of $I$ and $u_\alpha$ is a continuous real-valued function on $X_\alpha$ for each $\alpha \in J$.

Consider the set $H$ of "functions of one variable" $(x_i) \to u_\alpha(x_\alpha)$ (any $\alpha \in I$) which are continuous on $X$. This set separates the points of $X$, for if $x = (x_i)$ and $y = (y_i)$ are any two distinct points of $X$, there exists $\alpha \in I$ such that $x_\alpha \neq y_\alpha$ and there exists a continuous real-valued function $h_\alpha$ on $X_\alpha$ such that $h_\alpha(x_\alpha) \neq h_\alpha(y_\alpha)$. The function $x \to h_\alpha(\operatorname{pr}_\alpha x)$ then belongs to $H$ and takes distinct values at $x$ and $y$. Since every polynomial in the functions of $H$ is of the form stated in the theorem, the result follows from Theorem 3.

If not all the $X_i$ are compact, the conclusion of Theorem 4 is not necessarily valid (cf. Exercise 9).

### 4. APPROXIMATION OF CONTINUOUS MAPPINGS OF A COMPACT SPACE INTO A NORMED SPACE

Let $X$ be a compact space and let $Y$ be a normed vector space over the field $\mathbf{R}$ (Chapter IX, § 3); the space $C(X; Y)$ will always be assumed to carry the topology of uniform convergence defined by the norm $\|u\| = \sup_{x \in X} \|u(x)\|$ ($\S 3$, no. 2).

Given a set $H$ of continuous real-valued functions defined on $X$, a finite family $(u_i)_{1 \leq i \leq n}$ of functions belonging to $H$, and a finite family $(a_i)_{1 \leq i \leq n}$ of points of $Y$: the mapping $x \to \sum_{i=1}^n a_i u_i(x)$ of $X$ into $Y$ is then continuous; we denote it by $\sum_{i=1}^n a_i u_i$, and we say that it is a linear combination of functions of $H$ with coefficients in $Y$. We say that a continuous mapping $f : X \to Y$ can be uniformly approximated by linear combinations of functions of $H$ (with coefficients in $Y$), if $f$ lies in the closure of the vector subspace of $C(X; Y)$ formed by these linear combinations.

#### Proposition 5 {#top-x-s4-prop-5 .statement}

Let $X$ be a compact space, $Y$ a normed space over $\mathbf{R}$ and $H$ a subset of $\mathcal{C}(X; \mathbf{R})$. If every continuous real-valued function on $X$ can be uniformly approximated by functions of $H$, then every continuous mapping $f$ of $X$ into $Y$ can be uniformly approximated by linear combinations of functions of $H$ with coefficients in $Y$.

Given any real number $\varepsilon > 0$, for each $x \in X$ there exists an open neighbourhood of $x$ in which the oscillation of $f$ is $\leq \varepsilon$. Hence there is a finite open covering $(A_i)_{1 \leq i \leq n}$ of $X$ such that the oscillation of $f$ in each $A_i$ is $\leq \varepsilon$. Let $a_i$ be a value of $f$ in $A_i$ ($1 \leq i \leq n$), and let $(u_i)_{1 \leq i \leq n}$ be a continuous partition of unity subordinate to the covering $(A_i)$ (Chapter IX, § 4, no. 4, Corollary to Proposition 4). Let $x$ be any point of $X$. For each index $i$ such that $x \notin A_i$, we have $u_i(x) = 0$, and for each index $i$ such that $x \in A_i$ we have $\|f(x) - a_i\| \leq \varepsilon$; it follows that

$$
\left\| f(x) - \sum_{i=1}^n a_i u_i(x) \right\| = \left\| \sum_{i=1}^n (f(x) - a_i) u_i(x) \right\| \leq \varepsilon \sum_{i=1}^n u_i(x) = \varepsilon.
$$

On the other hand, by hypothesis there is a function $v_i \in H$ such that

$$
|u_i(x) - v_i(x)| \leq \frac{\varepsilon}{\sum_{j=1}^n \|a_j\|}
$$

for all $x \in X$ ($1 \leq i \leq n$); hence we have

$$
\left\| f(x) - \sum_{i=1}^n a_i v_i(x) \right\| \leq 2\varepsilon \quad \text{for all } x \in X,
$$

and the proof is complete.

From Proposition 5 it follows that, to each of the propositions in which we have proved that a certain subset $H$ of $\mathcal{C}(X; \mathbf{R})$ is dense, there corresponds an analogous proposition for continuous mappings of $X$ into an arbitrary normed space $Y$. We shall write down explicitly only the proposition which corresponds in this way to Theorem 3. Given a set $H$ of real-valued functions on $X$, a polynomial in the functions of $H$, with coefficients in $Y$, is defined to be any linear combination, with coefficients in $Y$, of products of a finite (possibly empty) family of functions belonging to $H$. Then:

#### Proposition 6 {#top-x-s4-prop-6 .statement}

Let $X$ be a compact space and let $H$ be a set of continuous real-valued functions on $X$ which separates the points of $X$. Then every continuous mapping of $X$ into a normed space $Y$ over $\mathbf{R}$ can be uniformly approximated by polynomials in the functions of $H$ with coefficients in $Y$.

From this we deduce:

#### Proposition 7 {#top-x-s4-prop-7 .statement}

Let $X$ be a compact space and let $H$ be a set of continuous complex-valued functions on $X$ which separates the points of $X$. Then every continuous mapping of $X$ into a normed space $Y$ over $\mathbf{C}$ can be uniformly approximated by polynomials in the functions $f \in H$ and their conjugates $\overline{f}$ with coefficients in $Y$.

We have only to note that $Y$ is also a normed space over $\mathbf{R}$ and to apply Proposition 6 to the set of real parts and imaginary parts of the functions $f \in H$, using the formulas

$$
\Re f = \frac{1}{2} (f + \overline{f}), \quad \Im f = \frac{1}{2i} (f - \overline{f}).
$$

#### Corollary 1 {#top-x-s4-prop-7-cor-1 .statement}

If $X$ is a compact subset of the space $\mathbf{C}^n$, then every continuous mapping $(z_1, z_2, \ldots, z_n) \to f(z_1, z_2, \ldots, z_n)$ of $X$ into a normed space $Y$ over the field $\mathbf{C}$ can be uniformly approximated by polynomials in the $z_k$ and $\overline{z}_k$ with coefficients in $Y$.

We shall see later that in general it is not possible to approximate $f$ uniformly by polynomials (with coefficients in $Y$) in the variables $z_k$ alone, even if $Y = \mathbf{C}$.

#### Corollary 2 {#top-x-s4-prop-7-cor-2 .statement}

Let $X$ be a locally compact space and let $C_0(X)$ be the normed $\mathbf{C}$-algebra of continuous mappings of $X$ into $\mathbf{C}$ which tend to 0 at infinity. Let $A$ be a subalgebra of $C_0(X)$ which separates the points of $X$ and is such that (i) $\overline{f} \in A$ whenever $f \in A$, (ii) for each $x \in X$, there is an $f \in A$ such that $f(x) \neq 0$. Then $A$ is dense in $C_0(X)$.

If $X'$ is the compact space obtained by adjoining a point at infinity $\omega$ to $X$, then $C_0(X)$ can be identified with the subspace of $C(X; \mathbf{C})$ consisting of continuous mappings which vanish at $\omega$, the norm on $C_0(X)$ being defined by

$$
\|f\| = \sup_{x \in X} |f(x)| = \sup_{x \in X} |f(x)|.
$$

By virtue of Proposition 7, every $f \in C_0(X)$ can be uniformly approximated by polynomials with complex coefficients in the functions belonging to $A$; moreover, since $f(\omega) = 0$, the argument of no. 2, Proposition 4 shows that we may suppose these polynomials to have no constant term, and then they belong to $A$.

Another application of Proposition 7 is the following:

#### Proposition 8 {#top-x-s4-prop-8 .statement}

Let P be the set of all periodic continuous mappings of $\mathbf{R}^m$ into $\mathbf{C}$ whose group of periods contains $\mathbf{Z}^m$. Then every function belonging to P can be uniformly approximated in $\mathbf{R}^m$ by linear combinations, with complex coefficients, of functions of the form

$$
(x_1, x_2, \ldots, x_m) \to e(h_1 x_1 + h_2 x_2 + \cdots + h_m x_m),
$$

where the $h_i$ are rational integers (such linear combinations are called trigonometric polynomials in m variables).

We have only to observe that P (endowed with the topology of uniform convergence) is canonically isomorphic to the space of all continuous mappings of the compact space $\mathbf{T}^m$ into $\mathbf{C}$ (Chapter VII, § 1, no. 6), and apply Proposition 7 to the set of mappings of $\mathbf{T}^m$ into $\mathbf{C}$ which correspond to the m mappings $(x_1, x_2, \ldots, x_m) \to e(x_i) \quad (1 \leq i \leq m)$ of $\mathbf{R}^m$ into $\mathbf{C}$.

### Exercises {#top-x-s4-exercises}

See the [exercises for § 4](exercises/s4/).
