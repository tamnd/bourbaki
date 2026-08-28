---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 2
section_title: Support of a measure
lang: en
source: int-i-vi
book_pages: INT III.23-INT III.32, INT III.59
pdf_pages: 0068-0077, 0104-0104
extraction: ocr
subsections:
    - "no": 1
      title: Restriction of a measure to an open set. Definition of a measure by means of local data
      page: 23
      pdf_page: 68
    - "no": 2
      title: Support of a measure
      page: 25
      pdf_page: 70
    - "no": 3
      title: Characterization of the support of a measure
      page: 27
      pdf_page: 72
    - "no": 4
      title: Point measures. Measures with finite support
      page: 29
      pdf_page: 74
    - "no": 5
      title: Discrete measures
      page: 31
      pdf_page: 76
statements: 26
exercises: 5
content_sha256: 7734d12336d925e72881f81d6d32fad0063a3ed5a19a0cac962d4a91f9de9a67
---

## § 2. SUPPORT OF A MEASURE

### 1. Restriction of a measure to an open set. Definition of a measure by means of local data

Let X be a locally compact space, Y an open set in X. The subspace Y of X is locally compact, and every continuous function with values in a topological vector space E, defined on Y and with compact support, may be extended by continuity to all of X, by giving it the value 0 on $\mathbf{C}Y$; one can therefore identify in this way the space $\mathcal{K}(Y;E)$ with the linear subspace of $\mathcal{K}(X;E)$ formed by the continuous functions with compact support *contained in* Y. If $\mu$ is a measure on X, it is clear that the restriction of $\mu$ to $\mathcal{K}(Y;\mathbf{C})$ is a measure on Y, which is called the *restriction* of $\mu$ to the open subspace Y, or the measure *induced* on Y by $\mu$, and is denoted $\mu|Y$. The restrictions to Y of $|\mu|$, $\mathcal{R}\mu$ and $\mathcal{I}\mu$ are, respectively, $|\mu|Y|$, $\mathcal{R}(\mu|Y)$ and $\mathcal{I}(\mu|Y)$, by virtue of §1, Nos. 5 and 6. If $\mu$ is real then the restrictions of $\mu^+$ and $\mu^-$ to Y are, respectively, $(\mu|Y)^+$ and $(\mu|Y)^-$, by virtue of formula (8) of §1, No. 5.

One sees immediately that if Y and Z are two open sets in X such that $Y \supset Z$, and if $\mu|Y$ and $\mu|Z$ are the restrictions of $\mu$ to Y and Z, then $\mu|Z$ is also the restriction of $\mu|Y$ to the open subspace Z of the locally compact space Y.

In Ch. IV, §5, No. 7 we shall generalize this definition to the case that Y is a locally compact subspace of X.

Note that a measure on Y *is not necessarily* the restriction of some measure on X (cf. Ch. V, §7, No. 2, Prop. 3).

For example, let Y be the open interval ]0,1[ of $X = \mathbf{R}$; the mapping

$$
f \mapsto \int_0^1 \frac{f(x)}{x} dx
$$

is a measure on $Y$, because every function in $\mathcal{K}(Y; \mathbf{C})$ is zero on a neighborhood of 0 in $\mathbf{R}$. However, this measure cannot be extended to a measure on $\mathbf{R}$ because, in the contrary case, its restriction to the set of functions $f \in \mathcal{K}(Y; \mathbf{C})$ such that $\|f\| \leq 1$ would be bounded; but this is false.

However, we have the following proposition:

#### Proposition 1 {#int-iii-s2-prop-1 .statement}

*Let* $(Y_\alpha)_{\alpha \in A}$ *be an open covering of* $X$ *and suppose given, on each subspace* $Y_\alpha$, *a measure* $\mu_\alpha$, *in such a way that for every pair* $(\alpha, \beta)$, *the restrictions of* $\mu_\alpha$ *and* $\mu_\beta$ *to* $Y_\alpha \cap Y_\beta$ *are identical. Under these conditions, there exists one and only one measure* $\mu$ *on* $X$ *whose restriction to* $Y_\alpha$ *is equal to* $\mu_\alpha$ *for every index* $\alpha$.

Let us first show that every function $f \in \mathcal{K}(X; \mathbf{C})$ may be written in the form of a finite sum $f = \sum_i f_i$ where, for each of the functions $f_i \in \mathcal{K}(X; \mathbf{C})$, there exists an index $\alpha_i$ such that $\operatorname{Supp}(f_i) \subset Y_{\alpha_i}$. If $K = \operatorname{Supp}(f)$, there exists a finite number of indices $\alpha_i$ ($1 \leq i \leq n$) such that the $Y_{\alpha_i}$ form a covering of $K$; let $h_i$ ($1 \leq i \leq n$) be continuous mappings of $X$ into $[0, 1]$ such that the support of $h_i$ is compact and is contained in $Y_{\alpha_i}$ for $1 \leq i \leq n$, and such that $\sum_{i=1}^n h_i(x) = 1$ on $K$ (§ 1, No. 2, Lemma 1); the functions $f_i = f h_i$ meet the requirements. This shows in the first place that if there exists a measure $\mu$ meeting the requirements then it is *unique*, because for every finite sum $f = \sum_{i=1}^n f_i$, where $f_i \in \mathcal{K}(Y_{\alpha_i}; \mathbf{C})$, necessarily $\mu(f) = \sum_{i=1}^n \mu_{\alpha_i}(f_i)$. Moreover, we will have shown the existence of a linear form $\mu$ on $\mathcal{K}(X; \mathbf{C})$ whose restriction to each subspace $\mathcal{K}(Y_\alpha; \mathbf{C})$ is $\mu_\alpha$, provided we demonstrate the following property: if $(g_i)_{1 \leq i \leq m}$ and $(h_j)_{1 \leq j \leq n}$ are two finite sequences of functions in $\mathcal{K}(X; \mathbf{C})$ such that $g_i \in \mathcal{K}(Y_{\alpha_i}; \mathbf{C})$ for $1 \leq i \leq m$, $h_j \in \mathcal{K}(Y_{\beta_j}; \mathbf{C})$ for $1 \leq j \leq n$ and
$$
\sum_{i=1}^m g_i(x) = \sum_{j=1}^n h_j(x) = 1
$$
on $K$, then
$$
\sum_{i=1}^m \mu_{\alpha_i}(f g_i) = \sum_{j=1}^n \mu_{\beta_j}(f h_j).
$$
Now,
$$
f g_i = \sum_{j=1}^n f g_i h_j,
$$

whence
$$
\sum_{i=1}^{m} \mu_{\alpha_i}(f g_i) = \sum_{i=1}^{m} \sum_{j=1}^{n} \mu_{\alpha_i}(f g_i h_j).
$$
Similarly,
$$
\sum_{j=1}^{n} \mu_{\beta_j}(f h_j) = \sum_{j=1}^{n} \sum_{i=1}^{m} \mu_{\beta_j}(f g_i h_j).
$$
But since the support of $f g_i h_j$ is contained in $Y_{\alpha_i} \cap Y_{\beta_j}$, we have $\mu_{\alpha_i}(f g_i h_j) = \mu_{\beta_j}(f g_i h_j)$, which establishes our assertion.

It remains to see that $\mu$ is a measure on $X$; now, every point of $X$ admits a compact neighborhood contained in one of the $Y_\alpha$; the conclusion therefore follows at once from the definition of $\mu$ and from Prop. 6 of §1, No. 3.

**Corollary (Principle of localization).** — *Let $\mu$ and $\nu$ be two measures on $X$, and let $(Y_\alpha)$ be a family of open sets of $X$ such that, for every $\alpha$, the restrictions to $Y_\alpha$ of $\mu$ and $\nu$ are equal; then the restrictions of $\mu$ and $\nu$ to $Y = \bigcup_\alpha Y_\alpha$ are equal.*

### 2. Support of a measure

Let $\mu$ be a measure on a locally compact space $X$, and let $\mathcal{G}$ be the set of open sets $U \subset X$ such that the restriction of $\mu$ to $U$ is zero; it follows at once from the principle of localization (No. 1, Cor. of Prop. 1) that if $U_0$ is the union of the sets $U \in \mathcal{G}$, then $U_0$ itself belongs to $\mathcal{G}$ and is therefore the largest of the sets of $\mathcal{G}$.

#### Definition 1 {#int-iii-s2-def-1 .statement}

*If $\mu$ is a measure on a locally compact space $X$, one defines the support of $\mu$, denoted $\operatorname{Supp}(\mu)$, to be the closed set complementary to the largest of the open sets in $X$ on which the restriction of $\mu$ is zero.*

To say that a point $x \in X$ does not belong to the support of $\mu$ means that there exists an open neighborhood $V$ of $x$ such that the restriction of $\mu$ to $V$ is zero; to say that $x$ belongs to the support of $\mu$ therefore means that for *every* neighborhood $V$ of $x$, there exists a function $f \in \mathcal{K}(X; \mathbf{C})$, whose support is contained in $V$, such that $\mu(f) \neq 0$.

#### Example {#int-iii-s2-n2-exa-1 .statement}

— 1) For a measure on $X$ to be *zero*, it is necessary and sufficient that its support be *empty*.
2) The support of Lebesgue measure on $\mathbf{R}$ is the entire line $\mathbf{R}$; for, it is nonempty and is invariant under every translation.

3) On the interval $X = [0,1]$ of $\mathbf{R}$ consider a countable dense subset, arranged into a sequence $(a_n)$, and let $\mu$ be the measure defined by placing the mass $2^{-n}$ at the point $a_n$ for every $n \geq 0$ (§ 1, No. 3, Example I). The support of $\mu$ is all of $X$; for, let $x$ be any point of $X$, $V$ a neighborhood of $x$, and $f$ a continuous real-valued function $\geq 0$ on $X$, equal to 1 at the point $x$, whose support is contained in $V$ (§ 1, No. 2, Lemma 1); the set of $y \in V$ such that $f(y) > 0$ is open in $X$, therefore contains a point $a_n$, consequently $\mu(f) \geq f(a_n)2^{-n} > 0$.

#### Proposition 2 {#int-iii-s2-prop-2 .statement}

*The support of a measure $\mu$ is identical to the support of the measure $|\mu|$; if $\mu$ is real, its support is the union of the supports of the measures $\mu^+$ and $\mu^-$.*

For, if the restriction of $\mu$ to an open set $U$ is zero, then so is that of $|\mu|$ (resp. of $\mu^+$ and $\mu^-$ when $\mu$ is real), and conversely.

Note that the supports of $\mu^+$ and $\mu^-$ can be nonempty and *identical* (cf. Ch. V, § 5, Exer. 5).

#### Proposition 3 {#int-iii-s2-prop-3 .statement}

*If $\mu$ and $\nu$ are two measures on a locally compact space $X$ such that $|\mu| \leq |\nu|$, then $\mathrm{Supp}(\mu) \subset \mathrm{Supp}(\nu)$.*

For, if the restriction of $\nu$ to an open set is zero, then so is that of $\mu$.

#### Proposition 4 {#int-iii-s2-prop-4 .statement}

*The support of the sum of two measures is contained in the union of their supports.*

For, if the restrictions of two measures to an open set are zero, then the same is true of the restriction of their sum.

If $\mu$ and $\nu$ are two *positive* measures, then the support of $\lambda = \mu + \nu$ is *equal* to the union of the supports of $\mu$ and $\nu$; for, if $x_0$ is a point of the union and $V$ is any neighborhood of $x_0$, then there exists a continuous function $f \geq 0$ with support contained in $V$ and such that one of the numbers $\mu(f)$, $\nu(f)$ is $> 0$; *a fortiori*, $\lambda(f) = \mu(f) + \nu(f) > 0$.

#### Proposition 5 {#int-iii-s2-prop-5 .statement}

*The support of the restriction of a measure $\mu$ to an open set $U$ is the trace on $U$ of the support of $\mu$.*

The proposition is obvious from the definitions.

#### Proposition 6 {#int-iii-s2-prop-6 .statement}

*The set of measures on a locally compact space $X$, whose support is contained in a closed set $F$, is a vaguely closed linear subspace of $\mathcal{M}(X; \mathbf{C})$.*

For, it is the intersection of the vaguely closed hyperplanes with equation $\mu(f) = 0$, where $f$ runs over the set of functions in $\mathcal{H}(X; \mathbf{C})$ whose support does not intersect $F$.

Suppose $X$ is *not compact*: given a filter $\Phi$ on the space $\mathcal{M}(X; \mathbf{C})$ of measures on $X$, we shall say that the support of a measure $\mu$ *recedes indefinitely along* $\Phi$ if, for every compact subset $K$ of $X$, there exists a set $M \in \Phi$ such that $\mathrm{Supp}(\mu) \cap K = \varnothing$ for every measure $\mu \in M$.

#### Proposition 7 {#int-iii-s2-prop-7 .statement}

— *If $\Phi$ is a filter on $\mathcal{M}(X; \mathbf{C})$ such that the support of $\mu$ recedes indefinitely along $\Phi$, then $\mu$ converges vaguely to 0 with respect to $\Phi$.*

Let $f$ be any function in $\mathcal{K}(X; \mathbf{C})$ and let $K$ be its support. By hypothesis, there exists a set $M \in \Phi$ such that for every measure $\mu \in M$, $\operatorname{Supp}(\mu) \cap K = \varnothing$; it follows that $\mu(f) = 0$ for all $\mu \in M$, which proves the proposition.

### 3. Characterization of the support of a measure

By definition, if the support of a function $f \in \mathcal{K}(X; \mathbf{C})$ *does not intersect* the support of a measure $\mu$, then $\mu(f) = 0$; but the following more precise result is true:

#### Proposition 8 {#int-iii-s2-prop-8 .statement}

— *Let $\mu$ be a measure on a locally compact space $X$. For every function $f \in \mathcal{K}(X; \mathbf{C})$ that is zero on $\operatorname{Supp}(\mu)$, $\mu(f) = 0$.*

Set $K = \operatorname{Supp}(f)$, $S = \operatorname{Supp}(\mu)$. Given a number $\varepsilon > 0$, let $V$ be the set of $x \in X$ such that $|f(x)| < \varepsilon$; $V$ is an open set containing $S$ by hypothesis, therefore $CS$ is a neighborhood of the compact set $CV$. It follows that there exists a continuous mapping $h$ of $X$ into $[0, 1]$, equal to 1 on $CV$ and with support contained in $CS$ (§ 1, No. 2, Lemma 1). Since the support of $fh$ does not intersect $S$, $\mu(fh) = 0$. On the other hand, $f = fh$ on $K \cap CV$, and $|fh| \leq |f|$ on $X$, therefore $|f - fh| \leq 2\varepsilon$ on $X$, by the choice of $V$. Observe finally that there exists a number $M_K$ such that $|\mu(g)| \leq M_K \|g\|$ for every function $g \in \mathcal{K}(X; \mathbf{C})$ whose support is contained in $K$; since the support of $f - fh$ is contained in $K$, $|\mu(f - fh)| \leq 2M_K \varepsilon$ and consequently $|\mu(f)| = |\mu(f - fh)| \leq 2M_K \varepsilon$; since $\varepsilon$ is arbitrary, $\mu(f) = 0$.

#### Corollary 1 {#int-iii-s2-prop-8-cor-1 .statement}

— *If two functions $f, g$ in $\mathcal{K}(X; \mathbf{C})$ are equal on $\operatorname{Supp}(\mu)$, then $\mu(f) = \mu(g)$.*

#### Corollary 2 {#int-iii-s2-prop-8-cor-2 .statement}

— *Let $\mu$ be a positive measure on $X$; if $f \in \mathcal{K}(X; \mathbf{C})$ is such that $f(x) \geq 0$ on $\operatorname{Supp}(\mu)$, then $\mu(f) \geq 0$.*

For, $f = |f|$ on $\operatorname{Supp}(\mu)$, therefore $\mu(f) = \mu(|f|) \geq 0$ by Corollary 1.

#### Corollary 3 {#int-iii-s2-prop-8-cor-3 .statement}

— *Let $\mu$ be a bounded measure on $X$; if $f \in \mathcal{K}(X; \mathbf{C})$ is such that $|f(x)| \leq a$ on $\operatorname{Supp}(\mu)$, then $|\mu(f)| \leq a \|\mu\|$.*

For, $\operatorname{Supp}(|\mu|) = \operatorname{Supp}(\mu)$, and if $h$ is a continuous mapping of $X$ into $[0, 1]$, equal to 1 on $\operatorname{Supp}(f)$ and with compact support, then $|f(x)| \leq ah(x)$ on $\operatorname{Supp}(\mu)$, therefore

$$
|\mu|(|f|) \leq a|\mu|(h) \leq a\|\mu\|
$$

by Corollary 2; the conclusion then follows from formula (13) of § 1, No. 6.

#### Proposition 9 {#int-iii-s2-prop-9 .statement}

— Let $\mu$ be a positive measure on $X$; if $f$ is a function in $\mathcal{K}_+(X)$ such that $\mu(f) = 0$, then $f$ is zero on $\mathrm{Supp}(\mu)$.

Let $x$ be a point of $X$ such that $f(x) > 0$; let us show that $x$ does not belong to $\mathrm{Supp}(\mu)$. For, there exist a compact neighborhood $V$ of $x$ and a number $a > 0$ such that $f(y) \geq a$ on $V$. If $g$ is any continuous function $\geq 0$ with support contained in $V$, let us show that $\mu(g) = 0$; indeed, if one sets $b = \|g\|$ then $g \leq bf/a$, whence $\mu(g) \leq b\mu(f)/a = 0$.

#### Proposition 10 {#int-iii-s2-prop-10 .statement}

— Let $\mu$ be a measure on a locally compact space $X$; for every function $g \in \mathcal{C}(X; \mathbf{C})$, the support of the measure $g \cdot \mu$ is the closure $T$ of the set of points $x \in \mathrm{Supp}(\mu)$ such that $g(x) \neq 0$.

Set $S = \mathrm{Supp}(\mu)$; let $x_0$ be a point not belonging to $T$; there exists an open neighborhood $V$ of $x_0$ such that at every point of $V \cap S$, $g$ is zero; if $f \in \mathcal{K}(X; \mathbf{C})$ has support contained in $V$, then $fg$ is zero on $S$, therefore (Prop. 8) $\mu(gf) = 0$; in other words, the restriction of $g \cdot \mu$ to $V$ is zero.

Conversely, assuming that the restriction of $g \cdot \mu$ to an open neighborhood $W$ of a point $x_0 \in X$ is zero, let us show that there does not exist a point of $W \cap S$ at which $g$ is $\neq 0$. Indeed, if there were such a point $y$, there would exist a compact neighborhood $U$ of $y$, contained in $W$, at every point $x$ of which $g(x) \neq 0$; but then every function $f \in \mathcal{K}(X; \mathbf{C})$ with support contained in $U$ could be written $f = gh$, where $h \in \mathcal{K}(X; \mathbf{C})$ has support contained in $U \subset W$; it would then follow that $\mu(f) = \mu(gh) = 0$, contrary to the hypothesis $y \in S$.

Note that $T$ is contained in the intersection of the support $S$ of $\mu$ and the support of $g$, but it is not necessarily equal to this intersection. For example, if $X = \mathbf{R}$, $\mu$ is the Dirac measure at the point 0, and $g(x) = x$, then $g \cdot \mu = 0$ even though the intersection of the supports of $g$ and $\mu$ reduces to the point 0, thus is nonempty.

#### Corollary {#int-iii-s2-n3-cor-1 .statement}

— In order that the measure $g \cdot \mu$ be zero, it is necessary and sufficient that $g$ be zero on the support of $\mu$.

#### Proposition 11 {#int-iii-s2-prop-11 .statement}

— Every measure with compact support is bounded.

For, $|\mu|$ is also a measure with compact support, thus we can restrict attention to the case that $\mu \geq 0$; if $h$ is a continuous mapping of $X$ into $[0, 1]$, with compact support and equal to 1 on $\mathrm{Supp}(\mu)$, then for every function $f \in \mathcal{K}(X; \mathbf{C})$ one has $|f(x)| \leq \|f\| h(x)$ on $\mathrm{Supp}(\mu)$, therefore (Cor. 2 of Prop. 8) $\mu(|f|) \leq \mu(h)\|f\|$, which proves the proposition (§ 1, No. 8).

### 4. Point measures. Measures with finite support

#### Proposition 12 {#int-iii-s2-prop-12 .statement}

— Let $a_i$ ($1 \leq i \leq n$) be distinct points in a locally compact space $X$. Every measure on $X$ whose support is contained in the set of the $a_i$ is a linear combination of the measures $\varepsilon_{a_i}$ ($1 \leq i \leq n$).

For, such a measure $\mu$ is zero for every function $f \in \mathcal{K}(X; \mathbf{C})$ satisfying the $n$ relations $f(a_i) = 0$ (No. 3, Prop. 8); since these relations may be written $\varepsilon_{a_i}(f) = 0$, $\mu$ is a linear combination of the $\varepsilon_{a_i}$ (A, II, §7, No. 5, Cor. 1 of Th. 7).

In particular, every measure whose support is either empty or reduced to a single point $x$ is of the form $\alpha \varepsilon_x$, where $\alpha$ is a complex number; such a measure is said to be a *point measure*; thus every measure whose support is finite is a sum of point measures.

#### Theorem 1 {#int-iii-s2-thm-1 .statement}

— *Every measure* $\mu$ *on a locally compact space* $X$ *is in the vague closure of the vector space* $V$ *of measures whose support is finite and contained in* $\mathrm{Supp}(\mu)$.

It suffices to prove that $\mu$ is orthogonal to the subspace $V^\circ$ of $\mathcal{K}(X; \mathbf{C})$ orthogonal to $V$ (TVS, II, §6, No. 3, Cor. 2 of Th. 1), that is, that the relations $\langle f, \varepsilon_a \rangle = 0$, where $a$ runs over the support of $\mu$, imply $\langle f, \mu \rangle = 0$; but this is just Prop. 8 of No. 3.

#### Corollary 1 {#int-iii-s2-thm-1-cor-1 .statement}

— *Every bounded measure* $\mu$ *on* $X$ *is in the vague closure of the convex set* $A$ *of measures whose support is finite and is contained in that of* $\mu$, *and whose norm is* $\leq \| \mu \|$. *Moreover, if* $\nu$ *tends vaguely to* $\mu$ *while remaining in* $A$, *then* $\| \nu \|$ *tends to* $\| \mu \|$.

To prove the first assertion, it suffices to establish that the measure $\mu$ belongs to the polar set of the polar set $A^\circ$ of $A$ in $\mathcal{K}(X; \mathbf{C})$ (TVS, II, §6, No. 3, Th. 1 and §8, No. 4); this means that for $f \in \mathcal{K}(X; \mathbf{C})$, the relations $|\langle f, \varepsilon_a \rangle| \leq 1/\| \mu \|$ for all $a \in \mathrm{Supp}(\mu)$ imply that $|\langle f, \mu \rangle| \leq 1$; but this is a consequence of Cor. 3 of Prop. 8 of No. 3.

To prove the second assertion, we note that

$$
\liminf_{\nu \to \mu, \nu \in A} \| \nu \| \geq \| \mu \|
$$

since the function $\nu \mapsto \| \nu \|$ is lower semi-continuous for the vague topology (§1, No. 9, Cor. 4 of Prop. 15), and the conclusion follows from the fact that $\| \nu \| \leq \| \mu \|$ for $\nu \in A$ by definition.

#### Corollary 2 {#int-iii-s2-thm-1-cor-2 .statement}

— *Every bounded measure* $\mu$ *on* $X$ *is in the vague closure of the set of measures whose support is finite and contained in that of* $\mu$ *and whose norm is equal to* $\| \mu \|$.

We can suppose that $\mu \neq 0$. Let $V$ be an open neighborhood of 0 for the vague topology; for every $\varepsilon$ such that $0 < \varepsilon < 1$, there exists, by virtue of Cor. 1, a measure $\nu_0$ whose support is finite and contained in $\mathrm{Supp}(\mu)$ and for which $\nu_0 - \mu \in V$ and $\| \mu \| \geq \| \nu_0 \| \geq (1 - \varepsilon) \| \mu \|$. Setting $\nu = (\| \mu \| / \| \nu_0 \|) \nu_0$, we have $\| \nu \| = \| \mu \|$ and $\| \nu - \nu_0 \| \leq \| \mu \|$; for $\varepsilon$ sufficiently small we therefore have $\nu - \mu \in V + V$, whence the conclusion.

#### Corollary 3 {#int-iii-s2-thm-1-cor-3 .statement}

*Every bounded positive measure $\mu$ on $X$ is in the vague closure of the convex set of positive measures whose support is finite and contained in that of $\mu$ and whose norm is equal to $\| \mu \|$.*

The same reasoning as in Cor. 2 shows that we can limit ourselves to proving that $\mu$ is in the vague closure of the convex set $B$ formed by the positive measures with finite support contained in $\mathrm{Supp}(\mu)$ and with norm $\leq \| \mu \|$. Again, it suffices to establish that $\mu$ belongs to the polar set of $B^\circ$, the polar set of $B$ *in the space* $\mathcal{K}(X; \mathbf{R})$ (TVS, II, §6, No. 3, Th. 1); but this means that for $f \in \mathcal{K}(X; \mathbf{R})$ the relations $\langle f, \varepsilon_a \rangle \geq -1 / \| \mu \|$ for all $a \in \mathrm{Supp}(\mu)$ imply $\langle f, \mu \rangle \geq -1$, which is a consequence of No. 3, Cor. 2 of Prop. 8.

#### Corollary 4 {#int-iii-s2-thm-1-cor-4 .statement}

*In the space $\mathcal{M}(X; \mathbf{C})$, the set of point measures is total for the topology of strictly compact convergence* (§1, No. 10).

On the cone $\mathcal{M}_+(X)$, the topology of strictly compact convergence is identical to the vague topology (§1, No. 10, Prop. 18), and every measure on $X$ may be written $\mu_1 - \mu_2 + i \mu_3 - i \mu_4$, where the $\mu_j$ ($1 \leq j \leq 4$) are positive measures; the conclusion therefore follows from Th. 1.

#### Proposition 13 {#int-iii-s2-prop-13 .statement}

*Let $\mu$ be a measure on a locally compact space $X$. For a point $x_0$ to belong to $\mathrm{Supp}(\mu)$, it is necessary and sufficient that the point measure $\varepsilon_{x_0}$ be in the vague closure of the set of measures $g \cdot \mu$, where $g$ runs over the set of continuous functions with compact support such that $\| g \cdot \mu \| \leq 1$.*

The condition is obviously sufficient by virtue of Prop. 6 of No. 2. To see that it is necessary, suppose $x_0 \in \mathrm{Supp}(\mu)$; consider a finite number of functions $f_k$ ($1 \leq k \leq n$) in $\mathcal{K}(X; \mathbf{C})$, and an arbitrary number $\delta > 0$; we are to prove that there exists a function $g \in \mathcal{K}(X; \mathbf{C})$ such that $\| g \cdot \mu \| \leq 1$ and such that
$$
|f_k(x_0) - \mu(g f_k)| \leq \delta
$$
for $1 \leq k \leq n$. Let $U$ be a relatively compact open neighborhood of $x_0$ such that the oscillation of each of the $f_k$ ($1 \leq k \leq n$) on $U$ is $\leq \delta / 2$. By hypothesis, since $x_0 \in \mathrm{Supp}(\mu)$, there exists a function $g_0 \in \mathcal{K}(X; \mathbf{C})$ whose support is contained in $U$ and such that $\mu(g_0) \neq 0$; the measure $\nu = g_0 \cdot \mu$ is not zero, since for every function $f \in \mathcal{K}(X; \mathbf{C})$ equal to 1 on $U$, $\nu(f) = \mu(g_0) \neq 0$. Moreover, $\nu$ is bounded (No. 3, Prop. 11);

multiplying $g_0$ by a scalar, we can suppose that $\| \nu \| = 1$. This being so, setting $\alpha_k = f_k(x_0)$ we can write, for $1 \leq k \leq n$ and for every function $h \in \mathcal{K}(X; \mathbf{C})$,

$$
f_k(x_0) - \nu(f_k h) = \alpha_k (1 - \nu(h)) + \nu((\alpha_k - f_k)h) .
$$

Since $\nu$ has its support in $U$, we may identify it with its restriction to $U$; the hypothesis $\| \nu \| = 1$ then implies that there exists a function $h \in \mathcal{K}(X; \mathbf{C})$, with support contained in $U$, such that $\| h \| \leq 1$ and such that $| \alpha_k (1 - \nu(h)) | \leq \delta / 2$ for $1 \leq k \leq n$. The definition of $U$ moreover shows that $| (\alpha_k - f_k(x)) h(x) | \leq \delta / 2$ for all $x \in U$; since $\| \nu \| = 1$ and $\operatorname{Supp}(\nu) \subset U$ we therefore have $| \nu((\alpha_k - f_k)h) | \leq \delta / 2$ and so, setting $g = g_0 h$,

$$
| f_k(x_0) - \mu(g f_k) | \leq \delta \quad \text{for } 1 \leq k \leq n .
$$

This proves the proposition, since $\| g \cdot \mu \| = \| (g_0 h) \cdot \mu \| \leq \| g_0 \cdot \mu \| = 1$.

#### Corollary {#int-iii-s2-n4-cor-1 .statement}

*Let $\mu$ be a measure on $X$. For a measure $\nu$ on $X$ to be in the vague closure of the set of measures $g \cdot \mu$, where $g$ runs over $\mathcal{K}(X; \mathbf{C})$, it is necessary and sufficient that $\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu)$.*

For, $\operatorname{Supp}(g \cdot \mu) \subset \operatorname{Supp}(\mu)$ by No. 3, Prop. 10; therefore the support of every vague limit of measures of the form $g \cdot \mu$ is also contained in $\operatorname{Supp}(\mu)$ (No. 2, Prop. 6). Conversely, if $\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu)$ then $\nu$ is the vague limit of measures with *finite* support contained in $\operatorname{Supp}(\mu)$ (Th. 1), hence is in the vague closure of the set of measures $g \cdot \mu$ by Prop. 13.

### 5. Discrete measures

#### Proposition 14 {#int-iii-s2-prop-14 .statement}

*For a measure $\mu$ on a locally compact space $X$ to be a discrete measure (§ 1, No. 3, Example I), it is necessary and sufficient that $\operatorname{Supp}(\mu)$ be a discrete closed subspace of $X$.*

Let $\mu$ be a discrete measure on $X$, defined by the masses $h(x) \neq 0$ placed at the points $x$ of a discrete closed subspace $N$ of $X$; let us show that $\operatorname{Supp}(\mu) = N$. For every $a \in N$ and every neighborhood $V$ of $a$, there exists a function $f \in \mathcal{K}(X; \mathbf{C})$ with support contained in $V$, equal to 1 at the point $a$ and to 0 at the other points of $N$, whence $\mu(f) = h(a) \neq 0$. On the other hand if $b \notin N$ then there exists a neighborhood $W$ of $b$ not intersecting $N$; for every function $g \in \mathcal{K}(X; \mathbf{C})$ with support contained in $W$, we therefore have $\mu(g) = 0$, which proves that $b \notin \operatorname{Supp}(\mu)$.

Conversely, let $\mu$ be a measure such that $\operatorname{Supp}(\mu)$ is a discrete closed subspace $N$ of $X$. For every $a \in N$, there exists an open neighborhood $V_a$ of $a$ that contains no point of $N$ distinct from $a$; the restriction of $\mu$ to $V_a$ is therefore a point measure with support $\{a\}$ (No. 2, Prop. 5), hence (No. 4, Prop. 12) is of the form $h(a)\varepsilon_a$, where $h(a) \neq 0$. Setting $h(x) = 0$ at the points of $\mathbf{C}\mathbf{N}$, and denoting by $\nu$ the measure defined by the masses $h(x)$, the principle of localization shows that $\nu = \mu$.

We thus see that on a *discrete* space $X$, every measure is *discrete*.

### Exercises {#int-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
