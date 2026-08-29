---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 1
section_title: Upper integral of a positive function
lang: en
source: int-i-vi
pdf_pages: 0108-0118, 0225-0227
extraction: ocr
subsections:
    - "no": 1
      title: Upper integral of a lower semi-continuous positive function
      page: 0
      pdf_page: 108
    - "no": 2
      title: Outer measure of an open set
      page: 4
      pdf_page: 111
    - "no": 3
      title: Upper integral of a positive function
      page: 6
      pdf_page: 113
    - "no": 4
      title: Outer measure of an arbitrary set
      page: 10
      pdf_page: 117
statements: 34
exercises: 8
content_sha256: 4efc1f3cfe523060663c90bb9b64343469cc31d0bbbed2b5f147d96fa86f496e
---

## § 1. UPPER INTEGRAL OF A POSITIVE FUNCTION

### 1. Upper integral of a lower semi-continuous positive function

Let X be a locally compact space, $\mu$ a positive measure on X; we know that $\mu$ is an increasing function on the lattice $\mathcal{K}_+(X)$ (which will also be denoted $\mathcal{K}_+$).

We denote by $\mathcal{I}_+(X)$ (or simply $\mathcal{I}_+$) the set of numerical functions on X, finite or not, that are positive and lower semi-continuous on X.\footnote{1} Recall that the sum of any family of functions in $\mathcal{I}_+$ belongs to $\mathcal{I}_+$; the product of a function in $\mathcal{I}_+$ by a finite number $\alpha > 0$ belongs to $\mathcal{I}_+$; the upper envelope of *any* family of functions in $\mathcal{I}_+$ and the lower envelope of a *finite* family of functions in $\mathcal{I}_+$ also belong to $\mathcal{I}_+$ (GT, IV, §6, No. 2, Prop. 2 and Th. 4). We shall also make use of the following lemma:

#### Lemma {#int-iv-s1-n1-lem-1 .statement}

— *Every function* $f \in \mathcal{I}_+$ *is the upper envelope of the set* (directed for the relation $\leq$) *of all functions* $g \in \mathcal{K}_+$ *such that* $g \leq f$.

For every $x \in X$ such that $f(x) > 0$, and for every real number $a$ such that $0 < a < f(x)$, there exists by hypothesis a compact neighborhood V of $x$ such that $f(y) \geq a$ on V; on the other hand, there exists a function $g \in \mathcal{K}_+$, with support contained in V, equal to $a$ at the point $x$ and $\leq a$

\footnotetext{1 'I' as in 'inferior'; the letter $\mathcal{L}$ (as in 'lower') is preempted for other function spaces, to be discussed in §3.}

on V (GT, IX, §1, No. 5, Th. 2); therefore $0 \leq g \leq f$ and $g(x) \geq a$, which proves the lemma.

#### Definition 1 {#int-iv-s1-def-1 .statement}

*Given a positive measure $\mu$ on $X$, one calls upper integral of a function $f \in \mathcal{J}_+$ (with respect to $\mu$) the positive number (finite or equal to $+\infty$)*

$$
\mu^*(f) = \sup_{g \in \mathcal{H}_+, g \leq f} \mu(g).
$$

For every function $f \in \mathcal{H}_+$, it is clear that $\mu^*(f) = \mu(f)$, in other words $\mu^*$ is an *extension* of $\mu$ to $\mathcal{J}_+$.

#### Example {#int-iv-s1-n1-exa-1 .statement}

— Let $X$ be a *discrete* space, $\mu$ a positive measure on $X$, and set $\alpha(x) = \mu(\varphi_{\{x\}})$ for all $x \in X$. Every numerical function $f$ defined on $X$ is then continuous; for such a function $f \geq 0$, $\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$, where we agree to set $\alpha(x)f(x) = 0$ whenever $\alpha(x) = 0$ and $f(x) = +\infty$. For,
$$
\sum_{x \in X} \alpha(x)f(x) = \sup_M \left( \sum_{x \in M} \alpha(x)f(x) \right),
$$
where $M$ runs over the set of all finite subsets of $X$. If there exists an $x_0 \in X$ such that $f(x_0) = +\infty$ and $\alpha(x_0) > 0$, then $\sum_{x \in M} \alpha(x)f(x) = +\infty$ whenever $x_0 \in M$, and, on the other hand, $f \geq n \cdot \varphi_{\{x_0\}}$ for every integer $n > 0$, therefore $\mu^*(f) \geq n \alpha(x_0)$ and so $\mu^*(f) = +\infty$. If, on the contrary, $\alpha(x) = 0$ at all the points where $f(x) = +\infty$, then the function $g$ equal to $f$ at the points $x \in M$ where $\alpha(x) > 0$ and to 0 elsewhere belongs to $\mathcal{H}_+$, and so, by virtue of the conventions made, $\mu(g) = \sum_{x \in M} \alpha(x)f(x)$, which again proves the relation $\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$.

#### Proposition 1 {#int-iv-s1-prop-1 .statement}

*For every finite real number $\alpha > 0$ and every function $f \in \mathcal{J}_+$,*
$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### Proposition 2 {#int-iv-s1-prop-2 .statement}

*On the set $\mathcal{J}_+$, the function $\mu^*$ is increasing.*
The proofs are immediate from Def. 1.

#### Theorem 1 {#int-iv-s1-thm-1 .statement}

*Let $H$ be a nonempty set of functions in $\mathcal{J}_+$, directed for the relation $\leq$. For every positive measure $\mu$ on $X$,*
$$
\mu^*\left( \sup_{g \in H} g \right) = \sup_{g \in H} \mu^*(g) = \lim_{g \in H} \mu^*(g).
$$

Let $f = \sup_{g \in H} g$. We shall first prove the theorem for the special case that the functions $g \in H$ and their upper envelope $f$ *belong to* $\mathcal{H}_+$. It then follows from Dini’s theorem (GT, X, §4, No. 1, Th. 1) that the section filter of $H$ converges *uniformly* to $f$ on every compact subset of $X$, and in particular on the support K of $f$. Since $0 \leq g \leq f$ for every function $g \in \mathbf{H}$, the support of every function in $\mathbf{H}$ is contained in $K$; but by definition $\mu$ is continuous on the vector space $\mathcal{K}(X, K; \mathbf{C})$ of continuous functions with support contained in $K$, for the topology of uniform convergence; whence the relation (2) in this case.

Let us pass to the general case. It is clear that $\mu^*(g) \leq \mu^*(f)$ for every function $g \in \mathbf{H}$. By Def. 1, it all comes down to showing that, for every function $\psi \in \mathcal{K}_+$ such that $\psi \leq f$,

$$
\mu(\psi) \leq \sup_{g \in \mathbf{H}} \mu^*(g).
$$

For every function $g \in \mathbf{H}$, let $\Phi_g$ be the set of functions $\varphi \in \mathcal{K}_+$ such that $\varphi \leq g$, and let $\Phi$ be the union of the sets $\Phi_g$ as $g$ runs over $\mathbf{H}$; since $\mathbf{H}$ is directed, so is $\Phi$, and $f = \sup_{\varphi \in \Phi} \varphi$. Since $\psi \leq f$, $\psi$ is the upper envelope of the set of functions $\inf(\psi, \varphi)$ as $\varphi$ runs over $\Phi$; but since $\psi$ and the functions $\inf(\psi, \varphi)$ belong to $\mathcal{K}_+$, the first part of the proof shows that $\mu(\psi) = \sup_{\varphi \in \Phi} \mu(\inf(\psi, \varphi))$. Now, each $\varphi \in \Phi$ belongs to a set $\Phi_g$, therefore

$$
\mu(\inf(\psi, \varphi)) \leq \mu(\varphi) \leq \mu^*(g) \leq \sup_{g \in \mathbf{H}} \mu^*(g),
$$

from which it follows at once that $\mu(\psi) \leq \sup_{g \in \mathbf{H}} \mu^*(g)$. We have thus proved that $\mu^*(f) = \sup_{g \in \mathbf{H}} \mu^*(g)$; the relation $\mu^*(f) = \lim_{g \in \mathbf{H}} \mu^*(g)$ is then a consequence of the monotone limit theorem (GT, IV, §5, No. 2, Th. 2).

#### Theorem 2 {#int-iv-s1-thm-2 .statement}

*If $f_1$ and $f_2$ are two functions in $\mathcal{I}_+$ then*

$$
\mu^*(f_1 + f_2) = \mu^*(f_1) + \mu^*(f_2).
$$

As $\varphi_1$ (resp. $\varphi_2$) runs over the set of functions in $\mathcal{K}_+$ such that $\varphi_1 \leq f_1$ (resp. $\varphi_2 \leq f_2$), the functions $\varphi_1 + \varphi_2$ form a directed set (for $\leq$) whose upper envelope is $f_1 + f_2$. Therefore, by Th. 1,

$$
\mu^*(f_1 + f_2) = \sup \mu(\varphi_1 + \varphi_2) = \sup (\mu(\varphi_1) + \mu(\varphi_2)),
$$

where $(\varphi_1, \varphi_2)$ runs over the set of pairs of functions in $\mathcal{K}_+$ such that $\varphi_1 \leq f_1$ and $\varphi_2 \leq f_2$; since

$$
\sup (\mu(\varphi_1) + \mu(\varphi_2)) = \sup \mu(\varphi_1) + \sup \mu(\varphi_2)
$$

(GT, IV, §5, No. 7, Cor. 2 of Prop. 12), the theorem is proved.

#### Proposition 3 {#int-iv-s1-prop-3 .statement}

— *For every family* $(f_\iota)_{\iota \in I}$ *of functions in* $J_+$,

$$
\mu^*\left( \sum_{\iota \in I} f_\iota \right) = \sum_{\iota \in I} \mu^*(f_\iota).
$$

For every finite subset $J$ of $I$, it follows from Th. 2 (by induction on the number of elements of $J$) that $\mu^*\left( \sum_{\iota \in J} f_\iota \right) = \sum_{\iota \in J} \mu^*(f_\iota)$; as $J$ runs over the set of finite subsets of $I$, the functions $g_J = \sum_{\iota \in J} f_\iota$ belong to $J_+$ and form a directed set for the relation $\leq$, whose upper envelope is the function $\sum_{\iota \in I} f_\iota$; the proposition therefore follows from Th. 1.

#### Proposition 4 {#int-iv-s1-prop-4 .statement}

— *Let* $f$ *be a function in* $J_+$. *The mapping* $\mu \mapsto \mu^*(f)$ *of the set* $\mathcal{M}_+(X)$ *of positive measures on* $X$, *into the extended real line* $\overline{\mathbf{R}}$, *is lower semi-continuous for the vague topology on* $\mathcal{M}_+(X)$ *(Ch. III, §1, No. 9)*.

For, this mapping is by definition the upper envelope of the mappings $\mu \mapsto \mu(g)$, where $g$ runs over the set of functions in $\mathcal{K}_+$ such that $g \leq f$; and by definition of the vague topology, the mappings $\mu \mapsto \mu(g)$ are continuous on $\mathcal{M}(X)$.

### 2. Outer measure of an open set

Given an *open* set $G \subset X$, its characteristic function $\varphi_G$ is *lower semi-continuous* on $X$ (GT, IV, §6, No. 2, Cor. of Prop. 1). We may therefore make the following definition:

#### Definition 2 {#int-iv-s1-def-2 .statement}

— *Given a positive measure* $\mu$ *on* $X$, *for every open set* $G \subset X$ *the upper integral* $\mu^*(\varphi_G)$ *is called the outer measure of* $G$ *and is denoted* $\mu^*(G)$.

The outer measure of an open set $G$ is thus a number $\geq 0$, finite or equal to $+\infty$. Clearly $\mu^*(\varnothing) = 0$. Moreover, $\mu^*(X) = \| \mu \|,$ as is shown by formula (22) of Ch. III, §1, No. 8.

#### Proposition 5 {#int-iv-s1-prop-5 .statement}

— *The outer measure of a relatively compact open set* $G$ *is finite*.

For, there exists in this case a function $f \in \mathcal{K}_+$ such that $\varphi_G \leq f$ (Ch. III, §1, No. 2, Lemma 1), whence

$$
\mu^*(G) = \mu^*(\varphi_G) \leq \mu^*(f) = \mu(f) < +\infty.
$$

An open set of finite outer measure is not always relatively compact (Exer. 3).

#### Proposition 6 {#int-iv-s1-prop-6 .statement}

— *If* G₁ and G₂ *are two open sets such that* G₁ ⊂ G₂, *then* μ*(G₁) ≤ μ*(G₂).
For, the relation G₁ ⊂ G₂ is equivalent to φG₁ ≤ φG₂.

#### Proposition 7 {#int-iv-s1-prop-7 .statement}

— *Let* 𝔅 *be a set of open subsets of* X *that is directed for the relation* ⊂; *then*

$$
\mu^*\left(\bigcup_{G \in \mathfrak{B}} G\right) = \sup_{G \in \mathfrak{B}} \mu^*(G).
$$

The functions φ_G form a directed set (for ≤) in $\mathcal{I}_+$ and their upper envelope is the characteristic function of the union of the sets G ∈ 𝔅; the proposition is thus a consequence of Th. 1.

#### Proposition 8 {#int-iv-s1-prop-8 .statement}

— *Let* (G_ι)_{ι \in I} *be any family of open sets; then*

$$
\mu^*\left(\bigcup_{ι \in I} G_ι\right) \leq \sum_{ι \in I} \mu^*(G_ι).
$$

*Moreover, if the* G_ι *are pairwise disjoint then*

$$
\mu^*\left(\bigcup_{ι \in I} G_ι\right) = \sum_{ι \in I} \mu^*(G_ι).
$$

For, if G = $\bigcup_{ι \in I} G_ι$ then φ_G = sup_{ι \in I} φ_{G_ι} ≤ $\sum_{ι \in I} \varphi_{G_ι}$; when the G_ι are pairwise disjoint, φ_G = $\sum_{ι \in I} \varphi_{G_ι}$; the proposition is therefore a consequence of Props. 2 and 3.

#### Example {#int-iv-s1-n2-exa-1 .statement}

— Let X = \mathbf{R} and let μ be Lebesgue measure on \mathbf{R} (Ch. III, §1, No. 3); we are going to determine the outer measure of an *open interval* G = ]a, b[ (−∞ ≤ a < b ≤ +∞). Suppose first that a and b are finite. For every function f in $\mathcal{K}_+$ such that f ≤ φ_G, we have, by the theorem of the mean (FRV, II, §1, No. 5, Prop. 6),

$$
\int_{-\infty}^{+\infty} f(x)\, dx = \int_a^b f(x)\, dx \leq b - a,
$$

whence $\mu^*(G) \leq b - a$. On the other hand, for every $\varepsilon > 0$ there exists a function $f \in \mathcal{K}_+$ such that $f \leq \varphi_G$ and $f(x) = 1$ for $a + \varepsilon \leq x \leq b - \varepsilon$, whence $\mu^*(G) \geq b - a - 2\varepsilon$; since $\varepsilon$ is arbitrary, $\mu^*(G) = b - a$; in other words, the outer measure of $G$ is equal to its *length*. This result extends at once to the case that $G$ is an unbounded open interval, since it then contains bounded open intervals of arbitrarily large length; thus $\mu^*(G) = +\infty$ in this case.

Now let $G$ be any open set in $\mathbf{R}$; $G$ is the union of a countable set (finite or infinite) of pairwise disjoint open intervals $]a_k, b_k[$ (GT, IV, §2, No. 5, Prop. 2), consequently

$$
\mu^*(G) = \sum_k (b_k - a_k)
$$

(Prop. 8); in other words:

#### Proposition 9 {#int-iv-s1-prop-9 .statement}

*For Lebesgue measure on $\mathbf{R}$, the outer measure of an open set in $\mathbf{R}$ is equal to the sum of the lengths of its connected components.*

Note in particular that if $G$ is an open set in $\mathbf{R}$ such that $\mu^*(G) = 0$, then $G$ is *empty*.

### 3. Upper integral of a positive function

For every numerical function $f \geq 0$ (finite or not) defined on $X$, there exist functions $h \in \mathcal{I}_+$ such that $f \leq h$, if none other then the constant $+\infty$.

#### Definition 3 {#int-iv-s1-def-3 .statement}

*Let $\mu$ be a positive measure on $X$; for every numerical function $f \geq 0$ (finite or not) defined on $X$, the positive number*

$$
\mu^*(f) = \inf_{h \geq f, h \in \mathcal{I}_+} \mu^*(h)
$$

(*finite or equal to $+\infty$) *is called the upper integral of $f$ (with respect to $\mu$).*

When $f \in \mathcal{I}_+$, the number $\mu^*(f)$ thus defined is equal to the upper integral defined in Def. 1, since $\mu^*$ is increasing in $\mathcal{I}_+$.

In place of the notation $\mu^*(f)$, we shall also employ the notations $\int^* f d\mu$, $\int^* f(x) d\mu(x)$, $\int^* f \mu$ and $\int^* f(x) \mu(x)$.

#### Example {#int-iv-s1-n3-exa-1 .statement}

— If $X$ is a *discrete* space, $\mu$ a positive measure on $X$, and if one sets $\alpha(x) = \mu(\varphi_{\{x\}})$, then $\mu^*(f) = \sum_{x \in X} \alpha(x) f(x)$ for every numerical function $f \geq 0$ defined on $X$, since such a function is continuous (No. 1, *Example*).

#### Proposition 10 {#int-iv-s1-prop-10 .statement}

— *If f and g are two numerical functions $\geqslant 0$ defined on X such that $f \leqslant g$, then $\mu^*(f) \leqslant \mu^*(g)$.*

#### Proposition 11 {#int-iv-s1-prop-11 .statement}

— *For every finite real number $\alpha > 0$ and every numerical function $f \geqslant 0$ defined on X,

$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### Proposition 12 {#int-iv-s1-prop-12 .statement}

— *If $f_1$ and $f_2$ are two numerical functions $\geqslant 0$ defined on X, then

$$
\mu^*(f_1 + f_2) \leqslant \mu^*(f_1) + \mu^*(f_2).
$$

For every function $h_1 \in \mathcal{I}_+$ such that $f_1 \leqslant h_1$ and every function $h_2 \in \mathcal{I}_+$ such that $f_2 \leqslant h_2$, we have, by Th. 2,

$$
\mu^*(f_1 + f_2) \leqslant \mu^*(h_1 + h_2) = \mu^*(h_1) + \mu^*(h_2),
$$
whence (GT, IV, §5, No. 7, Cor. 2 of Prop. 12)

$$
\mu^*(f_1 + f_2) \leqslant \inf_{h_1 \geqslant f_1, h_1 \in \mathcal{I}_+} \mu^*(h_1) + \inf_{h_2 \geqslant f_2, h_2 \in \mathcal{I}_+} \mu^*(h_2),
$$
which is none other than the inequality (9).

Props. 10, 11 and 12 express that $\mu^*$ is an *increasing, positively homogeneous* and *convex* function on the set of numerical functions $\geqslant 0$ defined on X (Ch. I, No. 1). Note that if $f_1$ and $f_2$ are any two positive functions, the two members of (9) are not necessarily equal (§ 4, Exer. 8 d)); in §5, No. 6 we shall give conditions under which equality holds.

#### Theorem 3 {#int-iv-s1-thm-3 .statement}

— *For every increasing sequence $(f_n)$ of numerical functions $\geqslant 0$ defined on X,

$$
\mu^*\left( \sup_n f_n \right) = \sup_n \mu^*(f_n).
$$

Since each of the functions $f_n$ is less than or equal to $\sup_n f_n$, everything comes down to proving that $\mu^*(\sup_n f_n) \leqslant \sup_n \mu^*(f_n)$; this is obvious if the second member of the inequality is $+\infty$. In the contrary case, $\mu^*(f_n) < +\infty$ for all $n$; we are going to show that, for every $\varepsilon > 0$, there exists an *increasing* sequence $(g_n)$ of functions in $\mathcal{I}_+$ such that $f_n \leqslant g_n$ and $\mu^*(g_n) \leqslant \mu^*(f_n) + \varepsilon$. If $g$ is the upper envelope of the sequence $(g_n)$, we will then have $\mu^*(g) = \sup_n \mu^*(g_n)$ (No. 1, Th. 1), whence $\mu^*(g) \leqslant \sup \mu^*(f_n) + \varepsilon$; since $\sup f_n \leqslant g$ and $\varepsilon$ is arbitrary, the theorem will then have been proved.

By hypothesis, there exists a function $h_n \in \mathcal{J}_+$ such that $f_n \leq h_n$ and $\mu^*(f_n) \leq \mu^*(h_n) \leq \mu^*(f_n) + \varepsilon/2^n$; let us show that the functions $g_n = \sup(h_1, h_2, \ldots, h_n)$ meet the requirements. They belong to $\mathcal{J}_+$, form an increasing sequence, and satisfy $f_n \leq g_n$ for all $n$; we shall prove that

$$
\mu^*(g_n) \leq \mu^*(f_n) + \varepsilon \left( 1 - \frac{1}{2^n} \right).
$$

Let us argue by induction on $n$; the case $n = 1$ is trivial. On the other hand $g_{n+1} = \sup(g_n, h_{n+1})$, $g_n \geq f_n$ and $h_{n+1} \geq f_{n+1} \geq f_n$, whence $\inf(g_n, h_{n+1}) \geq f_n$; since

$$
\inf(g_n, h_{n+1}) + \sup(g_n, h_{n+1}) = g_n + h_{n+1},
$$

it follows from Th. 2 of No. 1 that

$$
\begin{align*}
\mu^*(g_{n+1}) &= \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(\inf(g_n, h_{n+1})) \\
&\leq \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(f_n) \\
&\leq \mu^*(f_{n+1}) + \varepsilon \left( 1 - \frac{1}{2^n} \right) + \frac{\varepsilon}{2^{n+1}} \\
&= \mu^*(f_{n+1}) + \varepsilon \left( 1 - \frac{1}{2^{n+1}} \right).
\end{align*}
$$

Q.E.D.

#### Corollary {#int-iv-s1-n3-cor-1 .statement}

— *Let $\mathfrak{F}$ be a set of numerical functions $\geq 0$, directed for the relation $\leq$, such that there exists a countable cofinal subset $\mathfrak{G}$ of $\mathfrak{F}$* (S, III, §1, No. 7); then

$$
\mu^*\left( \sup_{f \in \mathfrak{F}} f \right) = \sup_{f \in \mathfrak{F}} \mu^*(f).
$$

For, there exists an increasing sequence of functions in $\mathfrak{G}$ having the same upper envelope as $\mathfrak{F}$: if $(f_n)$ is the sequence of functions of $\mathfrak{G}$, arranged in any order, let $(f_{n_k})$ be a subsequence defined recursively by the conditions $n_1 = 1$, $f_{n_{k+1}} \geq \sup(f_{n_k}, f_k)$; it is clear that this subsequence has the indicated properties.

#### Remark {#int-iv-s1-n3-rem-1 .statement}

— 1) The relation (11) does not necessarily hold when $\mathfrak{F}$ is an *uncountable* directed set of functions $\geq 0$ that are not lower semi-continuous. Take for example $X = \mathbf{R}$, $\mu$ being Lebesgue measure on $\mathbf{R}$, and consider the directed (for $\leq$) set $\mathfrak{F}$ of characteristic functions $\varphi_M$ of all the *finite* subsets M of $\mathbf{R}$. Then $\mu^*(\varphi_M) = 0$ for every finite subset M, because a point is contained in an open interval of arbitrarily small length, and the characteristic function of a set reduced to a point therefore has upper integral zero by Def. 3 and Prop. 9 of No. 2. But the upper envelope of $\mathcal{F}$ is the constant function equal to 1, and $\mu^*(1) = +\infty$.

2) Note that for a *decreasing* sequence $(f_n)$ of functions $\geqslant 0$, one does not necessarily have $\mu^*(\inf_n f_n) = \inf_n \mu^*(f_n)$, even if $\mu^*(f_n) < +\infty$ for all $n$ (cf. §4, Exer. 8 c)).

#### Proposition 13 {#int-iv-s1-prop-13 .statement}

*For every sequence* $(f_n)$ *of numerical functions* $\geqslant 0$ *defined on* $X$,

$$
\mu^*\left( \sum_{n=1}^\infty f_n \right) \leqslant \sum_{n=1}^\infty \mu^*(f_n).
$$

It suffices to apply the relation (10) to the increasing sequence of functions $g_n = \sum_{k=1}^n f_k$ while taking into account that, by (9),

$$
\mu^*(g_n) \leqslant \sum_{k=1}^n \mu^*(f_k).
$$

In §5, No. 6, we will give conditions under which the two members of (12) are equal.

#### Proposition 14 (Fatou’s lemma) {#int-iv-s1-prop-14 .statement}

— *For every sequence* $(f_n)$ *of numerical functions* $\geqslant 0$,

$$
\mu^*\left( \liminf_{n \to \infty} f_n \right) \leqslant \liminf_{n \to \infty} \mu^*(f_n).
$$

For every integer $n$, set $g_n = \inf_{p \geqslant 0} f_{n+p}$; the sequence $(g_n)$ is increasing and $\liminf_{n \to \infty} f_n = \sup_n g_n$, whence, by (10),

$$
\mu^*(\liminf_{n \to \infty} f_n) = \sup_n \mu^*(g_n);
$$

but since $g_n \leqslant f_{n+p}$ for $p \geqslant 0$, we have $\mu^*(g_n) \leqslant \mu^*(f_{n+p})$, whence $\mu^*(g_n) \leqslant \inf_{p \geqslant 0} \mu^*(f_{n+p})$ and finally

$$
\mu^*\left( \liminf_{n \to \infty} f_n \right) \leqslant \sup_n \left( \inf_{p \geqslant 0} \mu^*(f_{n+p}) \right) = \liminf_{n \to \infty} \mu^*(f_n).
$$

#### Corollary {#int-iv-s1-n3-cor-2 .statement}

*Let* $(f_n)$ *be a sequence of numerical functions* $\geqslant 0$ *such that, for every* $x \in X$, $\lim_{n \to \infty} f_n(x) = +\infty$. *If* $\mu$ *is not the zero measure, then* $\lim_{n \to \infty} \mu^*(f_n) = +\infty$.

If $f_0$ is the constant function equal to $+\infty$, then $f_0$ is the upper envelope of all the functions of $\mathcal{K}_+$, and, since $\mu \neq 0$, we have $\mu^*(f_0) > 0$; but since $f_0 = \alpha f_0$ for every $\alpha > 0$, necessarily $\mu^*(f_0) = +\infty$ (Prop. 11). The inequality (13) then shows that $\mu^*(f_n)$ tends to $+\infty$ with $n$.

#### Proposition 15 {#int-iv-s1-prop-15 .statement}

*For every scalar $\alpha > 0$ and every pair of positive measures $\mu, \nu$ on $X$,*

$$
(\alpha \mu)^* = \alpha \mu^*
$$
$$
(\mu + \nu)^* = \mu^* + \nu^*.
$$

*Moreover, the relation $\mu \leq \nu$ implies $\mu^* \leq \nu^*$.*

Let us prove the relation (15). Set $\lambda = \mu + \nu$; thus $\lambda(f) = \mu(f) + \nu(f)$ for $f \in \mathcal{K}_+$; for $f \in \mathcal{J}_+$, the value of $\lambda^*(f)$ (resp. $\mu^*(f)$, $\nu^*(f)$) is the limit of $\lambda(g)$ (resp. $\mu(g)$, $\nu(g)$) as $g$ runs over the directed set (for $\leq$) of all $g \in \mathcal{K}_+$ such that $g \leq f$; therefore $\lambda^*(f) = \mu^*(f) + \nu^*(f)$. Finally, if $f$ is any function $\geq 0$ defined on $X$, then $\lambda^*(f)$ (resp. $\mu^*(f)$, $\nu^*(f)$) is the limit of $\lambda^*(h)$ (resp. $\mu^*(h)$, $\nu^*(h)$) as $h$ runs over the directed set (for $\geq$) of all functions $h \in \mathcal{J}_+$ such that $h \geq f$; again, by passage to the limit, we therefore have $\lambda^*(f) = \mu^*(f) + \nu^*(f)$, which proves (15). The relation (14) is established similarly. Finally, if $\mu \leq \nu$ one can write $\nu = \mu + (\nu - \mu)$, where $\nu - \mu \geq 0$, therefore $\nu^* = \mu^* + (\nu - \mu)^*$, which shows that $\mu^* \leq \nu^*$.

### 4. Outer measure of an arbitrary set

#### Definition 4 {#int-iv-s1-def-4 .statement}

*Let $\mu$ be a positive measure on $X$; for every subset $A$ of $X$, the upper integral $\mu^*(\varphi_A)$ is called the outer measure of $A$ (with respect to the measure $\mu$) and is denoted $\mu^*(A)$.*

The outer measure of a set is thus a number $\geq 0$, finite or equal to $+\infty$, that, for an open set, coincides with the outer measure defined in Def. 2 of No. 2.

#### Proposition 16 {#int-iv-s1-prop-16 .statement}

*If $A$ and $B$ are two subsets of $X$ such that $A \subset B$, then $\mu^*(A) \leq \mu^*(B)$.*

#### Corollary {#int-iv-s1-n4-cor-1 .statement}

*Every relatively compact set in $X$ has finite outer measure.*

For, such a set is contained in a relatively compact open set (GT, I, §9, No. 7, Prop. 10), whose outer measure is finite (No. 2, Prop. 5).

#### Proposition 17 {#int-iv-s1-prop-17 .statement}

— *If* $(A_n)$ *is an increasing sequence of subsets of X*, then $\mu^*(\bigcup_n A_n) = \sup_n \mu^*(A_n)$.

#### Proposition 18 {#int-iv-s1-prop-18 .statement}

— *For every sequence* $(A_n)$ *of subsets of X*,

$$
\mu^*\left(\bigcup_n A_n\right) \leq \sum_n \mu^*(A_n).
$$

These propositions are the translations of Props. 10 and 13 and of Th. 3 of No. 3 for characteristic functions of sets.

#### Proposition 19 {#int-iv-s1-prop-19 .statement}

— *For every subset A of X*, $\mu^*(A)$ *is the infimum of the outer measures of the open sets containing A*.

The proposition is obvious if $\mu^*(A) = +\infty$. In the contrary case, for every $\varepsilon$ such that $0 < \varepsilon < 1$, there exists a function $f \in \mathcal{J}_+$ such that $\varphi_A \leq f$ and $\mu^*(A) \leq \mu^*(f) \leq \mu^*(A) + \varepsilon$. Let G be the set of $x \in X$ such that $f(x) > 1 - \varepsilon$. Since $f$ is lower semi-continuous, G is *open* (GT, IV, §6, No. 2, Prop. 1) and contains A; on the other hand $f \geq (1 - \varepsilon)\varphi_G$, whence

$$
\mu^*(G) \leq \frac{1}{1 - \varepsilon} \mu^*(f) \leq \frac{1}{1 - \varepsilon} (\mu^*(A) + \varepsilon);
$$

since $\varepsilon$ is arbitrary, we see that $\mu^*(G)$ differs as little as we please from $\mu^*(A)$, whence the proposition.

### Exercises {#int-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
