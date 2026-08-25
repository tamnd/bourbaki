---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 3
section_title: LP spaces
lang: en
source: int-i-vi
book_pages: INT IV.18-INT IV.32, INT IV.120
pdf_pages: 0125-0139, 0227-0227
extraction: ocr
subsections:
    - "no": 1
      title: Minkowski’s inequality
      page: 18
      pdf_page: 125
    - "no": 2
      title: The semi-norms $N_p$
      page: 19
      pdf_page: 126
    - "no": 3
      title: The spaces $\mathcal{F}_F^p$
      page: 20
      pdf_page: 127
    - "no": 4
      title: $p$-th power integrable functions
      page: 23
      pdf_page: 130
    - "no": 5
      title: Properties of $p$-th power integrable functions
      page: 25
      pdf_page: 132
    - "no": 6
      title: Directed sets in $L^p$ and increasing sequences in $\mathcal{L}^p$
      page: 27
      pdf_page: 134
    - "no": 7
      title: Lebesgue’s theorem
      page: 30
      pdf_page: 137
    - "no": 8
      title: Relations between the spaces $\mathcal{L}_F^p$ ($1 \leq p < +\infty$)
      page: 31
      pdf_page: 138
statements: 43
exercises: 3
content_sha256: 16b427b4ea1d3b84287755988b90eee74953fb89281b59156d8259d8da9fed05
---

## § 3. L$^p$ SPACES

### 1. Minkowski’s inequality

Let X be a locally compact space, $\mu$ a measure on X. In the set of positive numerical functions (finite or not) defined on X, the function $|\mu|^*(f)$ is positive, positively homogeneous, increasing and convex ($\S 1$, No. 3, Props. 10, 11 and 12).

#### Proposition 1 {#int-iv-s3-prop-1 .statement}

— For every real number $p \geqslant 1$ and every pair of positive functions $f, g$ (finite or not) defined on X,

$$
(|\mu|^*((f + g)^p))^{1/p} \leqslant (|\mu|^*(f^p))^{1/p} + (|\mu|^*(g^p))^{1/p}
$$

(Minkowski’s inequality).

The inequality (1) is obvious when one of the terms of the second member is equal to $+\infty$. In the contrary case, $f$ and $g$ are finite almost everywhere ($\S 2$, No. 3, Prop. 7). If $f_1$ and $g_1$ are finite positive functions equivalent to $f$ and $g$, respectively, then $f_1^p, g_1^p$ and $(f_1 + g_1)^p$ are equivalent to $f^p, g^p$ and $(f + g)^p$, respectively, and since equivalent positive functions have the same upper integral ($\S 2$, No. 3, Prop. 6), we are reduced to proving the inequality (1) in the case that $f$ and $g$ are everywhere finite; but in this case the inequality is a special case of the general Minkowski inequality proved in Ch. I, No. 2, Prop. 3.

We shall also have occasion to make use of the following elementary inequality: if $p \geqslant 1$ then, for any numbers $a \geqslant 0,\ b \geqslant 0$,

$$
a^p + b^p \leqslant (a + b)^p .
$$

The inequality is obvious if $a = b = 0$ or if one of the numbers $a, b$ is $+\infty$; if $a, b$ are finite and $a + b > 0$, it may be written

$$
\left( \frac{a}{a + b} \right)^p + \left( \frac{b}{a + b} \right)^p \leqslant 1 ,
$$

which follows from the fact that

$$
\left( \frac{a}{a + b} \right)^p \leqslant \frac{a}{a + b} , \quad \left( \frac{b}{a + b} \right)^p \leqslant \frac{b}{a + b} \quad \text{and} \quad \frac{a}{a + b} + \frac{b}{a + b} = 1 .
$$

### 2. The semi-norms $N_p$

In all that follows, $F$ denotes a *complete normed* vector space (that is, a Banach space) over the field $\mathbf{R}$ or the field $\mathbf{C}$; the *norm* of an element $z \in F$ will be denoted $|z|$. Given a mapping $f$ of a set $A$ into $F$, we write $|f|$ for the mapping $x \mapsto |f(x)|$ of $A$ into $\mathbf{R}_+$ (one must take care to note that $|f|$ is a *numerical function*, and not a *number*).

#### Definition 1 {#int-iv-s3-def-1 .statement}

*Let $X$ be a locally compact space, $\mu$ a measure on $X$. For every mapping $f$ of $X$ into a Banach space $F$, and for every number $p$ such that $1 \leq p < +\infty$, we denote by $N_p(f, \mu)$, or simply $N_p(f)$, the positive number* $(\int^* |f|^p d|\mu|)^{1/p}$.

Note that the number $N_p(f)$ may be equal to $+\infty$.

#### Proposition 2 {#int-iv-s3-prop-2 .statement}

*If $f$ and $g$ are two mappings of $X$ into $F$, and $\alpha$ is any scalar $\neq 0$, then, for $1 \leq p < +\infty$,

(3) $$
N_p(\alpha f) = |\alpha| N_p(f)
$$
(4) $$
N_p(f + g) \leq N_p(f) + N_p(g).
$$

For, the relation (3) follows at once from Def. 1 and the fact that $|\mu|^*$ is positively homogeneous; on the other hand, since $|f + g| \leq |f| + |g|$, the inequality (4) follows from Minkowski’s inequality (1) and the fact that $|\mu|^*$ is increasing.

We extend Def. 1 to the case of numerical functions, *finite or not*, defined on $X$, by again setting

$$
N_p(f) = \left( \int^* |f|^p d|\mu| \right)^{1/p}
$$

for such a function $f$. One sees immediately that the relations (3) and (4) also hold for these functions when $f + g$ is defined on $X$ and $\alpha \neq 0$. Moreover:

#### Theorem 1 (countable convexity theorem) {#int-iv-s3-thm-1 .statement}

— *Let $(f_n)$ be a sequence of functions $\geq 0$ (finite or not) defined on $X$. For $1 \leq p < +\infty$,

(5) $$
N_p \left( \sum_{n=1}^\infty f_n \right) \leq \sum_{n=1}^\infty N_p(f_n).
$$

Set $f = \sum_{n=1}^\infty f_n$; $f$ is the upper envelope of the increasing sequence of functions $g_n = \sum_{k=1}^n f_k$; the definition of $N_p(f)$, and Th. 3 of §1, No. 3, show that $N_p(f) = \sup_n N_p(g_n)$. But $N_p(g_n) \leq \sum_{k=1}^n N_p(f_k)$ by Prop. 1, whence the inequality (5).

#### Proposition 3 {#int-iv-s3-prop-3 .statement}

*If f and g are two equivalent mappings of X into a Banach space F, then $N_p(f - g) = 0$ for $1 \leq p < +\infty$; conversely, if $N_p(f - g) = 0$ for a value of $p \geq 1$ then f and g are equivalent.*

The proposition follows at once from Th. 1 of §2, No. 3.

If f and g are two equivalent mappings of X into F, then $N_p(f) = N_p(g)$ for all $p \geq 1$ (\S2, No. 3, Prop. 6); thus, $N_p(f)$ depends only on the class $\tilde{f}$ of f, and one sets, by definition, $N_p(\tilde{f}) = N_p(f)$. Since the classes of mappings of X into F form a vector space (\S2, No. 4), the relations (3) and (4) may also be written

$$
(6) \quad N_p(\alpha \tilde{f}) = |\alpha| N_p(\tilde{f})
$$
$$
(7) \quad N_p(\tilde{f} + \tilde{g}) \leq N_p(\tilde{f}) + N_p(\tilde{g}).
$$

One defines similarly $N_p(\tilde{f})$ for every class of equivalent numerical functions (finite or not).

One can then define $N_p(f)$ for a function with values in F (resp. in $\overline{\mathbf{R}}$) defined almost everywhere in X, by setting $N_p(f) = N_p(\tilde{f})$; it is then clear that the relations (3) and (4) again hold (assuming $\alpha \neq 0$ and $f + g$ defined almost everywhere, in the case of numerical functions, finite or not).

If $0 < p < 1$, one again sets $N_p(f) = (\int^* |f|^p d|\mu|)^{1/p}$, but the inequalities (4) and (5) are no longer valid (cf. Ch. I, Exer. 6 and Ch. IV, §6, Exer. 13).

### 3. The spaces $\mathcal{F}_F^p$

Let F be a Banach space, $\mathcal{F}(X; F)$ (or simply $\mathcal{F}_F$) the vector space of all mappings of X into F. For $1 \leq p < +\infty$ we will denote by $\mathcal{F}^p(X, \mu; F)$ or $\mathcal{F}_F^p(X, \mu)$, or simply $\mathcal{F}_F^p(\mu)$, or $\mathcal{F}_F^p$ (if no confusion can result), the set of mappings f of X into F such that $N_p(f) < +\infty$ (we write $\mathcal{F}^p$ instead of $\mathcal{F}_R^p$). It is clear that $\mathcal{F}_F^p(|\mu|) = \mathcal{F}_F^p(\mu)$. It follows at once from Prop. 2 of No. 2 that $\mathcal{F}_F^p$ is a *linear subspace* of $\mathcal{F}_F$ and that $N_p(f)$ is a *semi-norm* on this space. We shall always assume (absent express mention to the contrary) that $\mathcal{F}_F^p$ is equipped with the topology defined by this semi-norm; we shall say that this topology is the *topology of convergence in mean of order p* (for $p = 1$, we call it simply the *topology of convergence in mean*; for $p = 2$, one also says «topology of convergence in the quadratic mean»). We shall say that a filter $\mathcal{G}$ on $\mathcal{F}_F^p$ (resp. a sequence $(f_n)$ of elements of $\mathcal{F}_\mathbf{F}^p$) that converges to $f$ for this topology *converges in mean of order* $p$ to $f$; this means, therefore, that $N_p(g - f)$ tends to 0 with respect to $\mathcal{G}$ (resp. that $N_p(f_n - f)$ tends to 0 as $n$ tends to infinity).

This terminology extends at once to the case that the functions $f_n$ and the function $f$ are only defined almost everywhere (or have values in $\overline{\mathbf{R}}$, and are defined and finite almost everywhere).

Note that the locally convex space $\mathcal{F}_\mathbf{F}^p$ is in general *not Hausdorff*; the closure of 0 in this space is the linear subspace $\mathcal{N}_\mathbf{F}$ of *negligible* mappings of X into F (No. 2, Prop. 3).

#### Remark {#int-iv-s3-n3-rem-1 .statement}

— Let F be a Banach space *over the field* $\mathbf{C}$ of complex numbers; then, for every function $f \in \mathcal{F}_\mathbf{F}^p$ and every complex number $\alpha$, $\alpha f$ belongs to $\mathcal{F}_\mathbf{F}^p$ and $N_p(\alpha f) = |\alpha| N_p(f)$; in other words, $\mathcal{F}_\mathbf{F}^p$ is also a vector space over $\mathbf{C}$, and $N_p(f)$ is a semi-norm on this complex vector space (TVS, II, §1).

#### Proposition 4 {#int-iv-s3-prop-4 .statement}

*Let $\mathcal{B}$ be a filter base on $\mathcal{F}_\mathbf{F}^p$. Assume that there exists a compact set $K \subset X$ such that, for every set $M \in \mathcal{B}$, all of the mappings $f \in M$ have their support contained in K. Under these conditions, if $\mathcal{B}$ converges uniformly in X to $f_0$, then $f_0$ belongs to $\mathcal{F}_\mathbf{F}^p$ and $\mathcal{B}$ converges in mean of order $p$ to $f_0$.*

It comes to the same thing to say that, on the set of mappings $f \in \mathcal{F}_\mathbf{F}^p$ whose support is contained in a fixed compact set, the topology of uniform convergence is *finer* than the topology of convergence in mean of order $p$.

For, let $h$ be a continuous mapping of X into $[0,1]$, with compact support, equal to 1 on K (Ch. III, §1, No. 2, Lemma 1). For every $\varepsilon > 0$, there exists an $M \in \mathcal{B}$ such that, for every mapping $f \in M$, $|f(x) - f_0(x)| \leq \varepsilon h(x)$ for all $x \in X$. From this, it follows that $N_p(f - f_0) \leq \varepsilon N_p(h)$, whence the proposition.

#### Proposition 5 {#int-iv-s3-prop-5 .statement}

*The locally convex space $\mathcal{F}_\mathbf{F}^p$ is complete.*

Since the Hausdorff space associated with $\mathcal{F}_\mathbf{F}^p$ is a normed space, it suffices to prove that every *Cauchy sequence* $(f_n)$ in $\mathcal{F}_\mathbf{F}^p$ has a limit for the topology of convergence in mean of order $p$ (GT, IX, §2, No. 6, Prop. 9). By hypothesis, for every $\varepsilon > 0$ there exists an integer $m_0$ such that the relations $m \geq m_0,\ n \geq m_0$ imply $N_p(f_n - f_m) \leq \varepsilon$. One may therefore define, by induction on $k$, a strictly increasing sequence $(n_k)$ of integers $\geq 0$ such that $N_p(f_{n_{k+1}} - f_{n_k}) \leq 2^{-k}$. If we show that the series with general term $g_k = f_{n_{k+1}} - f_{n_k}$ ($k \geq 1$) is *convergent in mean of order* $p$, then it will have a sum $g \in \mathcal{F}_\mathbf{F}^p$, and $f = g + f_{n_1}$ will be the limit of the sequence $(f_{n_k})$ in $\mathcal{F}_\mathbf{F}^p$; $f$ will then be a cluster point of the sequence $(f_n)$; since this sequence is a Cauchy sequence, it will have $f$ as limit, and Prop. 5 will have been proved (GT, II, §3, No. 2, Cor. 2 of Prop. 5).

Prop. 5 is thus a consequence of the following proposition:

#### Proposition 6 {#int-iv-s3-prop-6 .statement}

*Let $(f_n)$ be a sequence of functions in $\mathcal{F}_\mathbf{F}^p$ such that $\sum_{n=1}^\infty N_p(f_n) < +\infty$. Under these conditions, the series with general term $f_n(x) \in \mathbf{F}$ is absolutely convergent almost everywhere in $X$. Setting $f(x) = \sum_{n=1}^\infty f_n(x)$ at the points where the series converges, and $f(x) = 0$ elsewhere, the function $f$ belongs to $\mathcal{F}_\mathbf{F}^p$ and is the sum of the series with general term $f_n$ (for the topology of convergence in mean of order $p$); more precisely, for every $n \geqslant 0$,

$$
N_p \left( f - \sum_{k=1}^n f_k \right) \leqslant \sum_{k=n+1}^\infty N_p(f_k).
$$

Consider the positive function (finite or not) $g(x) = \sum_{n=1}^\infty |f_n(x)|$. By the countable convexity theorem (No. 2, Th. 1),

$$
N_p(g) \leqslant \sum_{n=1}^\infty N_p(f_n) < +\infty;
$$

thus $g$ is finite almost everywhere (\S2, No. 3, Prop. 7), which means that the series with general term $f_n(x)$ is absolutely convergent almost everywhere. Since $\mathbf{F}$ is complete, this series is convergent almost everywhere and, for every $x \in X$, $|f(x)| \leqslant \sum_{n=1}^\infty |f_n(x)| = g(x)$, whence

$$
N_p(f) \leqslant N_p(g) \leqslant \sum_{n=1}^\infty N_p(f_n) < +\infty,
$$

which proves that $f$ belongs to $\mathcal{F}_\mathbf{F}^p$. On the other hand, for every integer $n$,

$$
|f(x) - \sum_{k=1}^n f_k(x)| \leqslant \sum_{k=n+1}^\infty |f_k(x)|
$$

almost everywhere, whence $N_p \left( f - \sum_{k=1}^n f_k \right) \leqslant \sum_{k=n+1}^\infty N_p(f_k)$. By hypothesis, the series with general term $N_p(f_n)$ is convergent; therefore, for every $\varepsilon > 0$, there exists an integer $n$ such that $\sum_{k=n+1}^{\infty} N_p(f_k) \leq \varepsilon$, and the inequality (8) proves that $f$ is the sum of the series with general term $f_n$, for the topology of convergence in mean of order $p$.

Propositions 5 and 6 are thus completely proved.

### 4. $p$-th power integrable functions

The vector space $\mathcal{H}(X; F)$ (which we shall denote simply by $\mathcal{H}_F$ if there is no fear of confusion), consisting of the continuous functions of $X$ into $F$ with compact support, is obviously a subspace of each of the vector spaces $\mathcal{F}_F^p$.

#### Definition 2 {#int-iv-s3-def-2 .statement}

*Given a locally compact space* $X$, *a measure* $\mu$ *on* $X$, *and a Banach space* $F$, *we denote by* $\mathcal{L}_F^p(X, \mu)$ *(or simply* $\mathcal{L}_F^p(\mu)$, *or* $\mathcal{L}_F^p$) *the closure, in the locally convex space* $\mathcal{F}_F^p(X, \mu)$, *of the vector space* $\mathcal{H}(X; F)$ *of continuous mappings of* $X$ *into* $F$ *with compact support.* *We denote by* $L_F^p(X, \mu)$ *(or* $L_F^p(\mu)$, *or* $L_F^p$) *the (normed)* Hausdorff *space associated with* $\mathcal{L}_F^p(X, \mu)$. *The functions belonging to* $\mathcal{L}_F^p$ *are called the* $p$*-th power integrable functions* (*).

Obviously $\mathcal{L}_F^p(X, |\mu|) = \mathcal{L}_F^p(X, \mu)$ and $L_F^p(X, |\mu|) = L_F^p(X, \mu)$.

We shall write $\mathcal{L}^p$ and $L^p$ instead of $\mathcal{L}_R^p$ and $L_R^p$ (or of $\mathcal{L}_C^p$ and $L_C^p$ when this causes no confusion). If $F$ is a *complex* Banach space, $\mathcal{L}_F^p$ and $L_F^p$ are equipped with the structure of a topological vector space over the field $\mathbf{C}$ (No. 3, *Remark*).

It is clear that every function in $\mathcal{F}_F^p$ that is equivalent to a function in $\mathcal{L}_F^p$, belongs to $\mathcal{L}_F^p$. A function with values in $F$ and *defined almost everywhere* in $X$ is again said to be *$p$*-*th power integrable* if it is equivalent to a function in $\mathcal{L}_F^p$; similarly a function with values in $\overline{\mathbf{R}}$, defined and finite almost everywhere in $X$, is said to be *$p$*-*th power integrable* if it is equivalent to a function in $\mathcal{L}^p$.

The functions in $\mathcal{L}_F^p$ (resp. in $\mathcal{L}^p$) are thus the *$p$*-*th power integrable functions* that are *defined on all of* $X$ (resp. defined and finite on all of $X$). In this section and the following one, most of the propositions proved for the functions in $\mathcal{L}_F^p$ (resp. $\mathcal{L}^p$) may immediately be extended to *$p$*-*th power integrable functions* that are not everywhere defined (resp. that are not everywhere defined and finite); we shall usually leave to the reader the task of formulating and proving these results.

(*) The justification for this terminology will be given in §4, No. 2.

#### Remark 1 {#int-iv-s3-n4-rem-1 .statement}

As has already been signalled (§2, No. 5) the $p$-th power integrable functions with values in $\mathbf{F}$ in general do not form a vector space.
2) In general, the space $\mathcal{F}_\mathbf{F}^p$ is distinct from its subspace $\mathcal{L}_\mathbf{F}^p$ (§4, Exer. 8).

Def. 2 immediately yields the following criterion:

#### Proposition 7 {#int-iv-s3-prop-7 .statement}

For a function $\mathbf{f}$ to belong to $\mathcal{L}_\mathbf{F}^p$, it is necessary and sufficient that, for every $\varepsilon > 0$, there exist a continuous function $g$ with compact support such that $N_p(\mathbf{f} - g) \leq \varepsilon$.

In other words, the functions in $\mathcal{L}_\mathbf{F}^p$ are the limits of sequences of continuous functions with compact support, for the topology of convergence in mean of order $p$.

#### Proposition 8 {#int-iv-s3-prop-8 .statement}

Let $f$ be a numerical function (finite or not) defined almost everywhere; if, for every $\varepsilon > 0$, there exists two $p$-th power integrable functions $g, h$ such that $g \leq f \leq h$ almost everywhere and $N_p(h - g) \leq \varepsilon$, then $f$ is $p$-th power integrable.

For, $f$ is finite almost everywhere and $N_p(f - g) \leq N_p(h - g) \leq \varepsilon$; Prop. 7 therefore shows that $f$ is $p$-th power integrable.

Since, by definition, $\mathcal{L}_\mathbf{F}^p$ is a closed subspace of $\mathcal{F}_\mathbf{F}^p$, and since the latter space is complete (No. 3, Prop. 5), we have the following result (GT, II, §3, No. 4, Prop. 8):

#### Theorem 2 {#int-iv-s3-thm-2 .statement}

The space $\mathcal{L}_\mathbf{F}^p$ is complete; the space $L_\mathbf{F}^p$ is a Banach space.

In the space $L_\mathbf{F}^p$, the norm $N_p(\tilde{\mathbf{f}})$ of a class is again denoted $\| \tilde{\mathbf{f}} \|_p$.

Th. 2 can be sharpened as follows:

#### Theorem 3 {#int-iv-s3-thm-3 .statement}

Let $(\mathbf{f}_n)$ be a Cauchy sequence in the space $\mathcal{L}_\mathbf{F}^p$; there exists a subsequence $(\mathbf{f}_{n_k})$ of $(\mathbf{f}_n)$ having the following properties:
1° the series with general term $N_p(\mathbf{f}_{n_{k+1}} - \mathbf{f}_{n_k})$ is convergent;
2° the series with general term $\mathbf{f}_{n_{k+1}}(x) - \mathbf{f}_{n_k}(x)$ is absolutely convergent almost everywhere;
3° if $\mathbf{f}$ is a function defined on $X$ and equal almost everywhere to the limit of the sequence $(\mathbf{f}_{n_k}(x))$, then $\mathbf{f}$ belongs to $\mathcal{L}_\mathbf{F}^p$ and the sequence $(\mathbf{f}_n)$ converges in mean of order $p$ to $\mathbf{f}$;
4° there exists a lower semi-continuous function $g \geq 0$ such that $N_p(g) < +\infty$ and such that, for every $k$, $|\mathbf{f}_{n_k}(x)| \leq g(x)$ for all $x \in X$.

As in the proof of Prop. 5 of No. 3, it suffices to define the sequence $(n_k)$ by induction, in such a way that $N_p(\mathbf{f}_{n_{k+1}} - \mathbf{f}_{n_k}) \leq 2^{-k}$; parts 2° and 3° then follow from Prop. 6 of No. 3 and the fact that $\mathcal{L}_\mathbf{F}^p$ is closed in $\mathcal{F}_\mathbf{F}^p$. On the other hand, if $h(x)$ is the sum of the series with general term $|\mathbf{f}_{n_{k+1}}(x) - \mathbf{f}_{n_k}(x)|$, Th. 1 of No. 2 shows that $N_p(h) < +\infty$; therefore, by the definition of $|\mu|^*$, there exists a lower semi-continuous function $g \geq h + |\mathbf{f}_{n_1}|$ such that $N_p(g) < +\infty$, which completes the proof.

#### Corollary 1 {#int-iv-s3-thm-3-cor-1 .statement}

— *If a Cauchy sequence* $(f_n)$ *in the space* $\mathcal{L}_F^p$ *is such that the sequence* $(f_n(x))$ *converges almost everywhere to* $f(x)$*, then* $f$ *is p-th power integrable and the sequence* $(f_n)$ *converges in mean of order* $p$ *to* $f$.

For, there exists a subsequence $(f_{n_k})$ of $(f_n)$ such that $(f_{n_k}(x))$ converges almost everywhere to $g(x)$, where $g$ is a function in $\mathcal{L}_F^p$ such that $(f_n)$ converges in mean of order $p$ to $g$. The hypotheses therefore imply that $f(x) = g(x)$ almost everywhere, whence the corollary.

#### Corollary 2 {#int-iv-s3-thm-3-cor-2 .statement}

— *Let* $\mathcal{E}$ *be a dense subset of* $\mathcal{L}_F^p$. *For every function* $f \in \mathcal{L}_F^p$, *there exists a sequence* $(g_n)$ *of functions in* $\mathcal{E}$ *having the following properties*:

1° *the sequence* $(g_n)$ *converges in mean of order* $p$ *to* $f$;
2° *for almost every* $x \in X$, *the sequence* $(g_n(x))$ *converges to* $f(x)$.

For, since the space $\mathcal{L}_F^p$ is metrizable, there exists a Cauchy sequence $(f_n)$ in $\mathcal{L}_F^p$ consisting of functions in $\mathcal{E}$ and convergent in mean of order $p$ to $f$ (GT, IX, §2, No. 6, Prop. 8); it suffices to apply Th. 3 to this sequence.

Cor. 2 is applicable in particular to the case where $\mathcal{E}$ is taken to be the space $\mathcal{K}_F$ of *continuous functions with compact support*.

#### Remark 2 {#int-iv-s3-n4-rem-2 .statement}

A Cauchy sequence $(f_n)$ in $\mathcal{L}_F^p$ can be such that the sequence $(f_n(x))$ is not convergent *at any point of* $X$ (Exer. 1).

#### Remark 3 {#int-iv-s3-n4-rem-3 .statement}

If $f$ belongs to $\mathcal{L}_F^p$, it is not always possible to find a sequence $(f_n)$ of continuous functions with compact support such that the sequence $(f_n(x))$ converges *everywhere* in $X$ to a function equal to $f(x)$ almost everywhere (§4, Exer. 4 c)).

### 5. Properties of $p$-th power integrable functions

#### Theorem 4 {#int-iv-s3-thm-4 .statement}

— *Let* $F$ *and* $G$ *be two Banach spaces,* $u$ *a continuous linear mapping of* $F$ *into* $G$. *For every function* $f \in \mathcal{L}_F^p$, *the composite function* $u \circ f$ *belongs to* $\mathcal{L}_G^p$.

Let $f \in \mathcal{L}_F^p$; for every $\varepsilon > 0$, there exists a function $g \in \mathcal{K}_F$ such that $N_p(f - g) \leq \varepsilon$; since $|u \circ f - u \circ g| \leq \|u\| \cdot |f - g|$, we have

$$
N_p(u \circ f - u \circ g) \leq \|u\| \cdot N_p(f - g) \leq \varepsilon \|u\|,
$$

and since $u \circ g$ is continuous with compact support, the theorem is proved.

#### Corollary 1 {#int-iv-s3-thm-4-cor-1 .statement}

— *Let* $a'$ *be a continuous linear form on* $F$; *if* $f \in \mathcal{L}_F^p$, *the numerical function* $x \mapsto \langle f(x), a' \rangle$ **(denoted by $\langle f, a' \rangle$)* belongs to* $\mathcal{L}^p$.

#### Corollary 2 {#int-iv-s3-thm-4-cor-2 .statement}

— Given n points $a_k$ of F ($1 \leq k \leq n$), and n numerical functions $f_k$ ($1 \leq k \leq n$) belonging to $\mathcal{L}^p$, the function $f = \sum_{k=1}^n a_k f_k$ belongs to $\mathcal{L}_F^p$.

This follows from the fact that the mapping $t \mapsto a t$ of $\mathbf{R}$ into F is continuous.

#### Proposition 9 {#int-iv-s3-prop-9 .statement}

— Let F be an n-dimensional vector space over $\mathbf{R}$, and let $(e_k)_{1 \leq k \leq n}$ be a basis of F. For a function $f = \sum_{k=1}^n e_k f_k$ to belong to $\mathcal{L}_F^p$, it is necessary and sufficient that each of the numerical functions $f_k$ belong to $\mathcal{L}^p$.

This follows at once from Cors. 1 and 2 of Th. 4.

#### Proposition 10 {#int-iv-s3-prop-10 .statement}

— In the space $\mathcal{L}_F^p$, the linear subspace formed by the (finite) linear combinations $\sum_k a_k f_k$, where $a_k \in F$ and the $f_k$ are continuous numerical functions with compact support, is dense (for the topology of convergence in mean of order $p$).

The set $\mathcal{K}_F$ of continuous mappings of X into F with compact support is by definition dense in $\mathcal{L}_F^p$. On the other hand, every function $g \in \mathcal{K}_F$ may be uniformly approximated by functions of the form $\sum_k a_k f_k$, where the $f_k$ are continuous functions with support contained in a fixed compact neighborhood of the support of $g$ (Ch. III, §1, No. 2, Lemma 2); it follows (No. 3, Prop. 4) that $g$ is in the closure in $\mathcal{L}_F^p$ of the set of $\sum_k a_k f_k$, whence the proposition.

#### Proposition 11 {#int-iv-s3-prop-11 .statement}

— If a function $f$ belongs to $\mathcal{L}_F^p$, then the function $|f|$ belongs to $\mathcal{L}^p$, and the mapping $f \mapsto |f|$ of $\mathcal{L}_F^p$ into $\mathcal{L}^p$ is uniformly continuous (for the topology of convergence in mean of order $p$).

For every $\varepsilon > 0$ there exists a continuous function $g$ with compact support, such that $N_p(f - g) \leq \varepsilon$; since $||f| - |g|| \leq |f - g|$, we have $N_p(|f| - |g|) \leq \varepsilon$, which proves that $|f| \in \mathcal{L}^p$. On the other hand, if $f_1, f_2$ are two functions in $\mathcal{L}_F^p$ then $N_p(|f_1| - |f_2|) \leq N_p(f_1 - f_2)$, which shows that $f \mapsto |f|$ is a uniformly continuous mapping.

#### Proposition 12 {#int-iv-s3-prop-12 .statement}

— For a numerical function $f$ to belong to $\mathcal{L}^p$, it is necessary and sufficient that each of the functions $f^+$ and $f^-$ belong to $\mathcal{L}^p$.

The condition is sufficient since $f = f^+ - f^-$; it is necessary, because if $f \in \mathcal{L}^p$ then $|f| \in \mathcal{L}^p$ (Prop. 11).

#### Corollary {#int-iv-s3-n5-cor-1 .statement}

— The upper (resp. lower) envelope of a finite family of functions in $\mathcal{L}^p$ belongs to $\mathcal{L}^p$.

### 6. Directed sets in $L^p$ and increasing sequences in $\mathcal{L}^p$

We have defined (\S 2, No. 6) an order relation $\tilde{f} \leq \tilde{g}$ in the set $\widetilde{\mathcal{F}}$ of equivalence classes of numerical functions defined and finite almost everywhere in $X$; equipped with this order relation and with its vector space structure, $\widetilde{\mathcal{F}}$ is a *Riesz space*. The corollary of Prop. 12 of No. 5 shows that if $\tilde{f}$ and $\tilde{g}$ are two elements of the subspace $L^p$ of $\widetilde{\mathcal{F}}$, then the supremum $\sup(\tilde{f}, \tilde{g})$ of $\tilde{f}$ and $\tilde{g}$ in $\widetilde{\mathcal{F}}$ (which is the class of each of the functions $\sup(f, g)$, where $f \in \tilde{f}$ and $g \in \tilde{g}$) belongs to $L^p$; this proves in particular that $L^p$, equipped with the order relation induced by that of $\widetilde{\mathcal{F}}$, is a *Riesz space*.

#### Proposition 13 {#int-iv-s3-prop-13 .statement}

*In the Riesz space $L^p$, equipped with the topology defined by the norm $\| \tilde{f} \|_p$, the mapping $\tilde{f} \mapsto | \tilde{f} |$ is uniformly continuous, and the set of elements $\tilde{f} \geq 0$ is closed.*

The first part of the proposition follows at once from Prop. 11 of No. 5; since the set of $\tilde{f} \geq 0$ is also the set of $\tilde{f}$ such that $| \tilde{f} | = f$, it is closed, because $\tilde{f} \mapsto | \tilde{f} |$ is a continuous mapping and $L^p$ is Hausdorff.

We thus see that the topology on $L^p$ defined by the norm $\| \tilde{f} \|_p$ is *compatible* with the ordered vector space structure of $L^p$ (TVS, II, \S 2, No. 7).

#### Proposition 14 {#int-iv-s3-prop-14 .statement}

*Let $H$ be a subset of the Riesz space $L^p$, consisting of classes $\geq 0$ and directed for the relation $\leq$. For $H$ to have a supremum in $L^p$, it is necessary and sufficient that*

$$
\sup_{\tilde{f} \in H} \| \tilde{f} \|_p < +\infty.
$$

*The supremum of $H$ in $L^p$ is then the limit* (in the Banach space $L^p$) *of the section filter of $H$*.

The condition is clearly necessary, since $\tilde{f} \mapsto \| \tilde{f} \|_p$ is an increasing function on the set of elements $\geq 0$ of $L^p$. To see that it is sufficient, we first observe that it implies that the image of $H$ under the mapping $\tilde{f} \mapsto \| \tilde{f} \|_p$ has a limit in $\mathbf{R}$, by the monotone limit theorem; the image of the section filter $\mathfrak{F}$ of $H$ under this mapping is therefore a base of a Cauchy filter on $\mathbf{R}$. The proof will be complete if we show that $\mathfrak{F}$ itself is a *base of a Cauchy filter* on $L^p$; for, $\mathfrak{F}$ will then converge in $L^p$, since $L^p$ is complete (No. 4, Th. 2), and the proposition will follow from TVS, II, \S 2, No. 7, Prop. 18.

To see that $\mathfrak{F}$ is a base of a Cauchy filter, we shall make use of the following lemma:

#### Lemma {#int-iv-s3-n6-lem-1 .statement}

If $f$ and $g$ are two functions in $\mathcal{L}^p$ such that $0 \leq f \leq g$, then

$$
(N_p(g - f))^p \leq (N_p(g))^p - (N_p(f))^p .
$$

When $f$ and $g$ are continuous with compact support, the relation (9) may be written

$$
\int (g - f)^p d|\mu| \leq \int g^p d|\mu| - \int f^p d|\mu|
$$

and is then a consequence of the elementary inequality $(g - f)^p \leq g^p - f^p$ (No. 1, formula (2)). To pass from this to the general case, it suffices to observe that the two members of (9) are continuous functions on $\mathcal{L}^p \times \mathcal{L}^p$, and that every function $f \geq 0$ in $\mathcal{L}^p$ is the limit (for convergence in mean of order $p$) of a sequence of continuous functions $\geq 0$ with compact support, by the continuity of the mapping $g \mapsto |g|$ on $\mathcal{L}^p$ (Prop. 11).

The lemma having been established, for every $\varepsilon > 0$ there exists by hypothesis an $\tilde{f} \in \mathrm{H}$ such that, for every $\tilde{g} \geq \tilde{f}$ belonging to $\mathrm{H}$, we have $(\|\tilde{g}\|_p)^p - (\|\tilde{f}\|_p)^p \leq \varepsilon$; from this it follows that $(\|\tilde{g} - \tilde{f}\|_p)^p \leq \varepsilon$; thus, if $\tilde{g}_1$ and $\tilde{g}_2$ are two elements in $\mathrm{H}$ that are $\geq \tilde{f}$, then $\|\tilde{g}_1 - \tilde{g}_2\|_p \leq 2\varepsilon^{1/p}$, which proves that $\mathfrak{F}$ is a Cauchy filter base on $L^p$ and completes the proof of Prop. 14.

#### Corollary 1 {#int-iv-s3-prop-14-cor-1 .statement}

If $\tilde{g}$ is the supremum of $\mathrm{H}$ in $L^p$, then

$$
\|\tilde{g}\|_p = \lim_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p = \sup_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p .
$$

This follows from the continuity of the norm $\|\tilde{f}\|_p$ in $L^p$, and the monotone limit theorem.

#### Corollary 2 {#int-iv-s3-prop-14-cor-2 .statement}

The Riesz space $L^p$ is fully lattice-ordered.

Every directed set $\mathrm{H}$ in $L^p$ (for the relation $\leq$), consisting of classes $\geq 0$ and bounded above in $L^p$, has a supremum: for, if $\tilde{h}$ is an upper bound for $\mathrm{H}$ in $L^p$, then $\|\tilde{f}\|_p \leq \|\tilde{h}\|_p$ for all $\tilde{f} \in \mathrm{H}$, and Prop. 14 is applicable. This proves the corollary (Ch. II, §1, No. 3, Prop. 1).

The conclusions of Prop. 14 no longer hold when they are formulated for the functions in $\mathcal{L}^p$ instead of their classes. To be precise, if $M$ is a subset of $\mathcal{L}^p$, consisting of functions $\geq 0$, directed for the relation $\leq$, and such that $\sup_{f \in M} N_p(f) < +\infty$, *the class of the upper envelope* $g$ of $M$ *is not necessarily identical to the supremum in* $L^p$ *of the classes of the functions* f \in M ; in particular, g is not necessarily p-th power integrable, and even if $g \in \mathcal{L}^p$, $N_p(g)$ can be distinct from $\sup_{f \in M} N_p(f)$ (cf. §1, No. 3, Remark 1 following Th. 3).

Nevertheless, we have the following theorem:

#### Theorem 5 {#int-iv-s3-thm-5 .statement}

*Let $(f_n)$ be an increasing sequence of functions $\geqslant 0$ in $\mathcal{L}^p$. For the upper envelope $f$ of this sequence to be p-th power integrable, it is necessary and sufficient that $\sup_n N_p(f_n) < +\infty$. The sequence $(f_n)$ is then convergent in mean of order $p$ to $f$, and*

$$
N_p(f) = \sup_n N_p(f_n) = \lim_{n \to \infty} N_p(f_n).
$$

The condition being obviously necessary, we need only prove that it is sufficient. Now, if the condition is satisfied then Prop. 14 shows that the sequence $(\tilde{f}_n)$ is a Cauchy sequence in $L^p$, therefore the sequence $(f_n)$ is a Cauchy sequence in $\mathcal{L}^p$; since $f_n(x)$ tends to $f(x)$ for all $x \in X$, $f$ is p-th power integrable and is the limit of the sequence $(f_n)$ for the topology of convergence in mean of order $p$ (No. 4, Cor. 1 of Th. 3). Therefore $N_p(f_n)$ tends to $N_p(f)$ since $N_p$ is a continuous function on $\mathcal{L}^p$.

#### Corollary 1 {#int-iv-s3-thm-5-cor-1 .statement}

*Let $(f_n)$ be a decreasing sequence of functions $\geqslant 0$ in $\mathcal{L}^p$; then, the lower envelope $f$ of the sequence belongs to $\mathcal{L}^p$, the sequence $(f_n)$ converges in mean of order $p$ to $f$, and*

$$
N_p(f) = \lim_{n \to \infty} N_p(f_n) = \inf_n N_p(f_n).
$$

The first two assertions follow from Th. 5 applied to the sequence $g_n = f_1 - f_n$, which is increasing and bounded above; the rest is then obvious.

#### Corollary 2 {#int-iv-s3-thm-5-cor-2 .statement}

*Let $(f_n)$ be a sequence of functions in $\mathcal{L}^p$. For the upper envelope $f$ of the sequence $(f_n)$ to be p-th power integrable, it is necessary and sufficient that there exist a function $g \geqslant 0$ such that $\int^* g^p d|\mu| < +\infty$ and $f_n \leqslant g$ for all $n$.

The condition is obviously necessary, on taking $g = f^+$. Conversely, suppose it is verified, and set $g_n = \sup_{k \leqslant n} f_k$; the sequence $(g_n)$ is increasing and consists of p-th power integrable functions (No. 5, Cor. of Prop. 12). The increasing sequence of positive functions $h_n = g_n + g_1^-$ satisfies the conditions of Th. 5, since $N_p(h_n) \leqslant N_p(g + g_1^-) < +\infty$; its upper envelope $\sup_n h_n$ is therefore p-th power integrable, and the same is true of $f = \sup_n h_n - g_1^-$.

#### Corollary 3 {#int-iv-s3-thm-5-cor-3 .statement}

— Let $A$ be a countable set, $\mathfrak{F}$ a filter on $A$ having a countable base, $(f_\alpha)_{\alpha \in A}$ a family of functions $\geq 0$ in $\mathcal{L}^p$. Assume that there exists a function $g \geq 0$ such that $N_p(g) < +\infty$ and $f_\alpha \leq g$ for all $\alpha \in A$; then the function $\limsup_{\mathfrak{F}} f_\alpha$ is $p$-th power integrable and

$$
\limsup_{\mathfrak{F}} N_p(f_\alpha) \leq N_p(\limsup_{\mathfrak{F}} f_\alpha).
$$

Let $(A_n)$ be a decreasing base of $\mathfrak{F}$ and set $g_n = \sup_{\alpha \in A_n} f_\alpha$; since $A_n$ is a countable set, it follows from Cor. 2 that $g_n$ is $p$-th power integrable; on the other hand, $N_p(g_n) \geq \sup_{\alpha \in A_n} N_p(f_\alpha)$. This being so, $\limsup_{\mathfrak{F}} f_\alpha$ is the lower envelope of the decreasing sequence $(g_n)$; thus $\limsup_{\mathfrak{F}} f_\alpha$ is $p$-th power integrable by Cor. 1, and

$$
N_p(\limsup_{\mathfrak{F}} f_\alpha) = N_p \left( \inf_n g_n \right) = \lim_{n \to \infty} N_p(g_n)
$$
$$
\geq \lim_{n \to \infty} \left( \sup_{\alpha \in A_n} N_p(f_\alpha) \right) = \limsup_{\mathfrak{F}} N_p(f_\alpha).
$$

### 7. Lebesgue’s theorem

#### Theorem 6 (Lebesgue) {#int-iv-s3-thm-6 .statement}

— Let $F$ be a Banach space, $(f_n)$ a sequence of functions in $\mathcal{L}_F^p$ such that: $1^\circ$ the sequence $(f_n(x))$ converges almost everywhere to a limit $f(x) \in F$; $2^\circ$ there exists a numerical function $g \geq 0$ such that $\int^* g^p d|\mu| < +\infty$ and $|f_n(x)| \leq g(x)$ almost everywhere in $X$, for every integer $n$. Then, the function $f$ (defined almost everywhere) is $p$-th power integrable, and the sequence $(f_n)$ converges in mean of order $p$ to $f$.

Consider the ‘double’ sequence of numerical functions $g_{mn} = |f_m - f_n|$, which belong to $\mathcal{L}^p$ (No. 5, Prop. 11); by hypothesis, $\lim_{m \to \infty, n \to \infty} g_{mn}(x) = 0$ almost everywhere, and on the other hand $|g_{mn}(x)| \leq 2g(x)$ almost everywhere; applying Cor. 3 of Th. 5 of No. 6 to this double sequence,

$$
\limsup_{m \to \infty, n \to \infty} N_p(f_m - f_n) \leq N_p(0) = 0,
$$

and since $N_p(f_m - f_n) \geq 0$ this implies $\lim_{m \to \infty, n \to \infty} N_p(f_m - f_n) = 0$; in other words, the sequence $(f_n)$ is a Cauchy sequence in $\mathcal{L}_F^p$. The theorem therefore follows from Cor. 1 of Th. 3 of No. 4.

#### Corollary {#int-iv-s3-n7-cor-1 .statement}

— Let $A$ be a set of indices, filtered by a filter $\mathfrak{F}$ having a countable base. If $(f_\alpha)_{\alpha \in A}$ is a family of functions in $\mathcal{L}_F^p$ that, with respect to the filter $\mathfrak{F}$, converge pointwise almost everywhere to a function $f$, and if, moreover, there exists a numerical function $g \geq 0$ such that $\int^* g^p d|\mu| < +\infty$ and $|f_\alpha(x)| \leq g(x)$ almost everywhere in $X$ for each $\alpha \in A$, then the function $f$ is $p$-th power integrable and $f_\alpha$ tends in mean of order $p$ to $f$ with respect to the filter $\mathfrak{F}$.

For, let $(A_n)$ be a decreasing countable base of $\mathfrak{F}$, and let $\alpha_n$ be any element of $A_n$; the sequence $(f_{\alpha_n})$ converges pointwise to $f$ almost everywhere in $X$, thus Th. 6 shows that $f$ is $p$-th power integrable and that $\lim_{n \to \infty} N_p(f - f_{\alpha_n}) = 0$. Since $\mathfrak{F}$ is the intersection filter of the elementary filters associated with all such sequences $(\alpha_n)$ (GT, I, §6, No. 8, Prop. 11), $\lim_{\mathfrak{F}} N_p(f - f_\alpha)$ exists and is equal to the common limit 0 of all of the sequences $(N_p(f - f_{\alpha_n}))$.

#### Remark 1 {#int-iv-s3-n7-rem-1 .statement}

Th. 6 no longer holds if the hypothesis $|f_n| \leq g$ (with $N_p(g) < +\infty$) is replaced by the weaker hypothesis $\sup_n N_p(f_n) < +\infty$. Suppose, for example, that $\mu$ is Lebesgue measure on $\mathbf{R}$; define continuous functions $f_n$ in the following manner: $f_n(x) = 0$ for $x \leq 0$ and for $x \geq \frac{2}{n}$, $f_n(\frac{1}{n}) = n$, $f_n$ being linear on the intervals $[0, \frac{1}{n}]$ and $[\frac{1}{n}, \frac{2}{n}]$. Then $\lim_{n \to \infty} f_n(x) = 0$ for all $x \in \mathbf{R}$, but $N_1(f_n) = 1$ for every $n$ (cf. §5, Exer. 12).

#### Remark 2 {#int-iv-s3-n7-rem-2 .statement}

The Cor. of Th. 6 no longer holds if it is not assumed that the filter $\mathfrak{F}$ has a countable base (cf. §1, No. 3, Remark 1 following the Cor. of Th. 3).

### 8. Relations between the spaces $\mathcal{L}_F^p$ ($1 \leq p < +\infty$)

For every real number $\alpha > 0$, the mapping $z \mapsto |z|^{\alpha-1} \cdot z$ is defined and continuous on the complement of 0 in $F$; moreover, since $||z|^{\alpha-1} \cdot z| = |z|^{\alpha}$, this function tends to 0 with $z$ and may therefore be extended by continuity to the point 0 by giving it the value 0 at this point, even if $\alpha < 1$.

#### Theorem 7 {#int-iv-s3-thm-7 .statement}

— Let $p$ and $q$ be two real numbers such that $1 \leq p < +\infty$, $1 \leq q < +\infty$. If a function $f$ belongs to $\mathcal{L}_F^p$ then the function $|f|^{(p/q)-1} \cdot f$ belongs to $\mathcal{L}_F^q$, and conversely.

By hypothesis, there exists a sequence $(f_n)$ of continuous functions with compact support such that $\sum_{n=1}^\infty N_p(f_n) < +\infty$ and $f(x) = \sum_{n=1}^\infty f_n(x)$ almost everywhere (No. 4, Th. 3). Set

$$
g_n = |f_1 + f_2 + \cdots + f_n|^{(p/q)-1} \cdot (f_1 + f_2 + \cdots + f_n);
$$

the function $g_n$ is continuous with compact support; on the other hand,

$$
|g_n|^q = |f_1 + f_2 + \cdots + f_n|^p \leq \left( \sum_{n=1}^\infty |f_n| \right)^p = h^q,
$$

where the numerical function $h \geqslant 0$ (finite or not) satisfies the inequality

$$
(N_q(h))^q = \left( N_p \left( \sum_{n=1}^{\infty} |f_n| \right) \right)^p \leqslant \left( \sum_{n=1}^{\infty} N_p(f_n) \right)^p < +\infty
$$

by the countable convexity theorem. Moreover, $g_n(x)$ tends almost everywhere to $g(x) = |f(x)|^{(p/q)-1} \cdot f(x)$, therefore Lebesgue’s theorem shows that $g \in \mathcal{L}_F^q$. The converse is immediate, since $f = |g|^{(q/p)-1} \cdot g$.

It can be shown that the mapping $f \mapsto |f|^{\frac{p}{q}-1} \cdot f$ is a homeomorphism of $\mathcal{L}_F^p$ onto $\mathcal{L}_F^q$ (\S 6, Exer. 10).

#### Corollary 1 {#int-iv-s3-thm-7-cor-1 .statement}

— *For a function $f$ to belong to $\mathcal{L}_F^p$, it is necessary and sufficient that the function $|f|^{p-1} \cdot f$ belong to $\mathcal{L}_F^1$.*

#### Corollary 2 {#int-iv-s3-thm-7-cor-2 .statement}

— *For a positive numerical function $f$ to belong to $\mathcal{L}^p$, it is necessary and sufficient that $f^p$ belong to $\mathcal{L}^1$.*

Note that if $f$ is a numerical function of arbitrary sign, such that $|f|^p$ belongs to $\mathcal{L}^1$, $f$ does not necessarily belong to $\mathcal{L}^p$ (cf. \S 4, Exer. 8).

### Exercises {#int-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
