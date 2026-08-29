---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 6
section_title: Convexity inequalities
lang: en
source: int-i-vi
book_pages: INT IV.89-INT IV.100, INT IV.134-INT IV.142
pdf_pages: 0196-0207, 0241-0249
extraction: ocr
subsections:
    - "no": 1
      title: The convexity theorem
      page: 89
      pdf_page: 196
    - "no": 2
      title: Inequality of the mean
      page: 90
      pdf_page: 197
    - "no": 3
      title: The spaces $L^\infty_F$
      page: 91
      pdf_page: 198
    - "no": 4
      title: Hölder’s inequality
      page: 93
      pdf_page: 200
    - "no": 5
      title: 'Application: relations between the spaces $L^p_F$ ($1 \leq p \leq +\infty$)'
      page: 98
      pdf_page: 205
statements: 22
exercises: 20
content_sha256: 620a678b6145f9aecb2d7fa10cb1189bf44b0c751811b2152d367e638c2e239d
---

## § 6. CONVEXITY INEQUALITIES

### 1. The convexity theorem

#### Theorem 1 {#int-iv-s6-thm-1 .statement}

— Let $X$ be a locally compact space, $\mu$ a positive measure on $X$, $F$ a real Banach space, $D$ a closed convex set in $F$, and $f$ a function on $X$ such that $f(X) \subset D$. For every non-negligible integrable numerical function $g \geqslant 0$ such that $fg$ is integrable, the point $\frac{\int fg\, d\mu}{\int g\, d\mu}$ belongs to $D$.

For, let $F'$ be the dual of $F$ and let $\langle z, a' \rangle \leqslant \alpha$ ($a' \in F', \alpha \in \mathbf{R}$) be a relation defining a closed half-space containing $D$. Since $fg$ is integrable, so is the numerical function $\langle fg, a' \rangle = \langle f, a' \rangle g$, and

$$
\int \langle fg, a' \rangle\, d\mu = \left\langle \int fg\, d\mu, a' \right\rangle
$$

(§ 4, No. 2, Cor. 1 of Th. 1); but, by hypothesis, $\langle f(x), a' \rangle \leqslant \alpha$ for all $x \in X$, therefore $\langle f(x)g(x), a' \rangle \leqslant \alpha g(x)$; on integrating, we have

$$
\left\langle \int fg\, d\mu, a' \right\rangle \leqslant \alpha \int g\, d\mu .
$$

This proves that the point $\frac{\int fg\, d\mu}{\int g\, d\mu}$ belongs to every closed half-space containing $D$; but, by the Hahn–Banach theorem, $D$ is the intersection of the closed half-spaces containing it (TVS, II, §5, No. 3, Cor. 1 of Prop. 4), whence the theorem.

#### Corollary {#int-iv-s6-n1-cor-1 .statement}

— *If the positive measure $\mu$ has total mass equal to 1 and if $f$ is integrable, then $\int f\, d\mu$ belongs to the closed convex envelope of $f(X)$ in $F$*.

It suffices to take for $g$ the constant function 1.

### 2. Inequality of the mean

We are going to sharpen Th. 1 for numerical measurable functions (finite or not).

#### Definition 1 {#int-iv-s6-def-1 .statement}

— Let X be a locally compact space, $\mu$ a measure on X. Given a numerical function f (finite or not), defined locally almost everywhere in X, we call maximum in measure, or $\mu$-maximum (resp. minimum in measure, or $\mu$-minimum) of the function f, and denote by $M_\infty(f)$ (resp. $m_\infty(f)$), the infimum (resp. supremum) of the set of numbers $\alpha$ such that $f(x) \leq \alpha$ (resp. $f(x) \geq \alpha$) locally almost everywhere (for $\mu$).

It follows at once from the definition that $m_\infty(f) = -M_\infty(-f)$, thus from every property of the maximum in measure one deduces a corresponding property of the minimum in measure.

For every $\alpha > M_\infty(f)$, the set of $x \in X$ such that $f(x) > \alpha$ is locally negligible; now, the set of $x \in X$ such that $f(x) > M_\infty(f)$ is the union of the sets where $f(x) > r_n$, with $r_n$ running over the set of rational numbers $> M_\infty(f)$; therefore $f(x) \leq M_\infty(f)$ locally almost everywhere (§ 5, No. 2). Similarly $f(x) \geq m_\infty(f)$ locally almost everywhere; it follows that $m_\infty(f) \leq M_\infty(f)$ if the measure $\mu$ is nonzero; moreover, the relation $m_\infty(f) = M_\infty(f)$ is equivalent to saying that $f$ is equal to a constant locally almost everywhere. It is clear that if the measure $\mu$ is nonzero, then

$$
\inf_{x \in X} f(x) \leq m_\infty(f) \leq M_\infty(f) \leq \sup_{x \in X} f(x).
$$

If two functions $f, g$ are equal locally almost everywhere, then $m_\infty(f) = m_\infty(g)$ and $M_\infty(f) = M_\infty(g)$.

Finally, if $f$ and $g$ are two functions such that $f + g$ is defined locally almost everywhere, then

(1)
$$
M_\infty(f + g) \leq M_\infty(f) + M_\infty(g)
$$
provided the second member is defined, as follows at once from Def. 1; similarly, if $f$ and $g$ are both $\geq 0$ and are such that $fg$ is defined locally almost everywhere, then

(2)
$$
M_\infty(fg) \leq M_\infty(f) M_\infty(g)
$$
provided the second member is defined.

If $M_\infty(f) < +\infty$, then $f(x) < +\infty$ locally almost everywhere, but not necessarily almost everywhere. A numerical function $f$ is said to be bounded in measure (for the measure $\mu$) if it is defined and finite almost everywhere and if, moreover, the numbers $m_\infty(f)$ and $M_\infty(f)$ are both finite (the latter condition amounts to saying that $M_\infty(|f|) < +\infty$).

#### Proposition 1 (Inequality of the mean) {#int-iv-s6-prop-1 .statement}

— *Let f be a measurable numerical function that is bounded in measure. For every integrable numerical function $g \geqslant 0$, the function $fg$ (defined almost everywhere) is integrable and*

$$
m_\infty(f) \int g d|\mu| \leqslant \int fg d|\mu| \leqslant M_\infty(f) \int g d|\mu|.
$$

Moreover, *two of the three members of the inequality (3) cannot be equal unless, in the set of $x \in X$ such that $g(x) \neq 0$, f is equal to $M_\infty(f)$ almost everywhere or equal to $m_\infty(f)$ almost everywhere*.

Indeed, $fg$ is measurable (§ 5, No. 3, Cor. 5 of Th. 1); moreover, the inequality $m_\infty(f)g(x) \leqslant f(x)g(x) \leqslant M_\infty(f)g(x)$ holds, not only locally almost everywhere, but even almost everywhere, because the set of points $x \in X$ where $g(x) \neq 0$ is a countable union of integrable sets (§ 5, No. 6, Lemma 1). It follows that $fg$ is integrable (§ 5, No. 6, Th. 5) and the inequality (3) holds. On the other hand, the function $M_\infty(f)g - fg$ is almost everywhere defined and equal to $(M_\infty(f) - f)g$; it is therefore $\geqslant 0$ almost everywhere in $X$; since the relation $M_\infty(f) \int g d|\mu| = \int fg d|\mu|$ is equivalent to $\int (M_\infty(f) - f)g d|\mu| = 0$, it can hold only if the function $(M_\infty(f) - f)g$ is negligible, which completes the proof.

Setting aside the trivial case that $\int g d|\mu| = 0$, the inequality (3) may be deduced from Th. 1 of No. 1 applied to the interval $D = [m_\infty(f), M_\infty(f)]$. One can bring to Th. 1 of No. 1 the complements analogous to those of Prop. 1, that specify the case in which the point $(\int fg d\mu)/(\int g d\mu)$ belongs to the boundary of D (Exer. 2).

### 3. The spaces $L^\infty_F$

#### Definition 2 {#int-iv-s6-def-2 .statement}

*For every mapping $f$ of $X$ into a Banach space $F$, one sets $N_\infty(f) = M_\infty(|f|)$; $f$ is said to be bounded in measure (for the measure $\mu$) if $N_\infty(f)$ is finite. The set of mappings of $X$ into $F$ that are measurable and bounded in measure is denoted $\mathcal{L}_F^\infty(X, \mu)$ (or $\mathcal{L}_F^\infty(\mu)$, or simply $\mathcal{L}_F^\infty$).*

A function $f$ in $\mathcal{L}_F^\infty$ may thus be characterized by the fact that there exists a *bounded measurable* function equal locally almost everywhere to $f$.

It follows immediately from (1) that

$$
N_\infty(f + g) \leqslant N_\infty(f) + N_\infty(g);
$$

on the other hand, $N_\infty(\alpha f) = |\alpha| N_\infty(f)$ for every scalar $\alpha$. The set $\mathcal{L}_F^\infty$ is therefore a *linear subspace* of the space of all mappings of $X$ into $F$, and $N_\infty(f)$ is a semi-norm on this vector space. Let $(f_n)$ be a sequence of functions in $\mathcal{L}_F^\infty$ that converges to $f \in \mathcal{L}_F^\infty$ for the topology defined by the semi-norm $N_\infty(f)$; for every integer $m$, there exist a locally negligible set $H_m$ and an integer $n_0$ such that $|f(x) - f_n(x)| \leq 1/m$ for every integer $n \geq n_0$ and every $x \notin H_m$ (every countable union of locally negligible sets being locally negligible); the union $H$ of the $H_m$ is locally negligible, and one sees that $f_n(x)$ tends *uniformly* to $f(x)$ on the complement of the locally negligible set $H$; the converse is immediate.

It is clear that every function equal locally almost everywhere to a function in $\mathcal{L}_F^\infty$ belongs to $\mathcal{L}_F^\infty$. In particular, the *locally negligible* functions defined on $X$ with values in $F$ form a linear subspace $\mathcal{N}_F^\infty$ of $\mathcal{L}_F^\infty$, characterized by the relation $N_\infty(f) = 0$ (the closure of 0 for the topology defined by $N_\infty(f)$). The Hausdorff space associated with $\mathcal{L}_F^\infty$, that is, the quotient space $\mathcal{L}_F^\infty / \mathcal{N}_F^\infty$, is denoted $L_F^\infty(X, \mu)$ (or $L_F^\infty(\mu)$ or $L_F^\infty$); its topology is defined by the *norm* deduced from $N_\infty$ by passage to the quotient; the norm of a class $\dot{f} \in L_F^\infty$ is denoted $N_\infty(\dot{f})$, or also $\| \dot{f} \|_\infty$. When $F = \mathbf{R}$ (resp. $\mathbf{C}$), we write $\mathcal{L}^\infty$ and $L^\infty$ in place of $\mathcal{L}_\mathbf{R}^\infty$ and $L_\mathbf{R}^\infty$ (resp. $\mathcal{L}_\mathbf{C}^\infty$ and $L_\mathbf{C}^\infty$) if this can cause no confusion.

#### Proposition 2 {#int-iv-s6-prop-2 .statement}

*The space* $\mathcal{L}_F^\infty$ *is complete; the space* $L_F^\infty$ *is a Banach space*.

For, let $(f_n)$ be a Cauchy sequence in $\mathcal{L}_F^\infty$; for every integer $n$, there exists an integer $k_n$ such that $N_\infty(f_r - f_s) \leq 1/n$ for $r \geq k_n$ and $s \geq k_n$; thus, there exists a locally negligible set $A_{rs}$ such that $|f_r(x) - f_s(x)| \leq 1/n$ for all $x \notin A_{rs}$. If $A_n$ is the union of the sets $A_{rs}$ (for $r \geq k_n$ and $s \geq k_n$), then $A_n$ is locally negligible and, for every $x \notin A_n$, $|f_r(x) - f_s(x)| \leq 1/n$ for all indices $r \geq k_n, s \geq k_n$. Let $A$ be the locally negligible set formed by the union of the $A_n$, and set $g_n(x) = f_n(x)$ for $x \notin A$, $g_n(x) = 0$ for $x \in A$; then $g_n$ belongs to $\mathcal{L}_F^\infty$ and, by the definition of $A$, the sequence $(g_n)$ converges *uniformly* on $X$ to a function $g$. It follows that the function $g$ is measurable (§ 5, No. 4, Th. 2); moreover, $g$ is bounded on the set of $x \in X$ where $|g_{k_1}(x)| \leq N_\infty(g_{k_1})$ and, since the complement of this set is locally negligible, $g$ belongs to $\mathcal{L}_F^\infty$. It is clear that in $\mathcal{L}_F^\infty$, the sequence $(g_n)$ has limit $g$, and the same is therefore true of the sequence $(f_n)$, since $N_\infty(f_n - g_n) = 0$ for all $n$. The second part of the proposition may be deduced immediately from this.

#### Remark {#int-iv-s6-n3-rem-1 .statement}

— 1) Every *bounded continuous* function $f$ on $X$ with values in $F$ belongs to $\mathcal{L}_F^\infty$, and

$$
N_\infty(f) \leq \| f \| = \sup_{x \in X} |f(x)| .
$$

In order that $N_\infty(f) = \|f\|$ for every bounded continuous function $f$, it is necessary and sufficient that the support of the measure $\mu$ be equal to $X$. For, if there exists a continuous function $f$ with negligible compact support and not identically zero, then $N_\infty(f) = 0$ and $\|f\| > 0$. Conversely, if the support of $\mu$ is equal to $X$ then, for every bounded continuous function $f$ and every number $\alpha < \|f\|$, the set of $x \in X$ such that $|f(x)| > \alpha$ is open and nonempty, hence has outer measure $> 0$, which shows that $N_\infty(f) = \|f\|$.

When the support of $\mu$ is equal to $X$, we may therefore identify the normed space $C^b(X; F)$, of bounded continuous functions on $X$ with values in $F$, with a subspace of the space $L_F^\infty$. Since $L_F^\infty$ is not in general Hausdorff, the subspace $C^b(X; F)$ is not in general closed in $L_F^\infty$, but its canonical image in $L_F^\infty$ is a closed subspace of $L_F^\infty$ (which can moreover be identified with $C^b(X; F)$ in the case contemplated). In general, $C^b(X; F)$ is distinct from $L_F^\infty$, that is, for an arbitrary bounded measurable function $f$, there does not in general exist a continuous function $g$ equal to $f$ locally almost everywhere (§ 5, Exer. 12). This implies that the space $\mathcal{H}(X; F)$ of mappings of $X$ into $F$, continuous with compact support, is in general not dense in $L_F^\infty$, whereas it is dense in each of the spaces $L_F^p$ for $1 \leq p < +\infty$ (§ 3, No. 4. Def. 2).

2) It is immediate that the topology defined by the semi-norm $N_\infty$ is finer than the topology induced on $L_F^\infty$ by the topology of convergence in measure (§ 5, No. 11).

### 4. Hölder’s inequality

In this No., $p$ and $q$ will denote two real numbers such that $1 \leq p \leq +\infty$, $1 \leq q \leq +\infty$, bound by the relation $1/p + 1/q = 1$; thus $q = p/(p-1)$ if $1 < p < +\infty$, $q = +\infty$ if $p = 1$, and $q = 1$ if $p = +\infty$; $p$ and $q$ will be called conjugate exponents. Note that the relation $1 \leq p \leq 2$ is equivalent to $2 \leq q \leq +\infty$; $p = q$ only when $p$ and $q$ are equal to 2.

#### Theorem 2 (Hölder’s inequality) {#int-iv-s6-thm-2 .statement}

— Let $f$ and $g$ be two numerical functions that are finite almost everywhere and are such that $f$ is equal almost everywhere to a function in $L^p$ and $g$ to a function in $L^q$. Then, the function $fg$ (defined almost everywhere) is integrable, and

$$
N_1(fg) \leq N_p(f) N_q(g).
$$

Let $f_1$ (resp. $g_1$) be a function in $L^p$ (resp. $L^q$) to which $f$ (resp. $g$) is equal almost everywhere; $fg$ is equal almost everywhere to the function $f_1 g_1$, which is everywhere defined and finite, and which is measurable, being the product of two measurable functions (§ 5, No. 3, Cor. 5 of Th. 1). If $1 < p < +\infty$, Hölder’s inequality for the upper integral (Ch. I, No. 3, Prop. 4) yields the inequality (4), and the relation $N_1(fg) < +\infty$ then shows that $fg$ is integrable (§ 5, No. 6, Th. 5). If $p = 1$, $q = +\infty$, the inequality (4) and the fact that $fg$ is integrable are immediate consequences of the inequality of the mean (No. 2, Prop. 1); thus the theorem is proved in all cases.

#### Corollary 1 {#int-iv-s6-thm-2-cor-1 .statement}

— Let $F, G, H$ be three Banach spaces, and let $(u, v) \mapsto \Phi(u, v)$ be a continuous bilinear mapping of $F \times G$ into $H$ such that $|\Phi(u, v)| \leq |u| \cdot |v|$. If $f \in \mathcal{L}_F^p$ and $g \in \mathcal{L}_G^q$, then the function $\Phi(f, g)$ is integrable and

$$
\left| \int \Phi(f, g)\, d\mu \right| \leq \int |\Phi(f, g)|\, d|\mu| \leq N_p(f) N_q(g).
$$

For, $\Phi(f, g)$ is measurable (§ 5, No. 3, Cor. 5 of Th. 1); since $|\Phi(f, g)| \leq |f| \cdot |g|$, the corollary follows from Th. 2 and the integrability criterion of § 5, No. 6, Th. 5.

Two special cases of Cor. 1 are important in applications:

#### Corollary 2 {#int-iv-s6-thm-2-cor-2 .statement}

— Let $F$ be a real (resp. complex) Banach space, $F'$ its strong dual (TVS, III, § 3, No. 1), and let $(z, z') \mapsto \langle z, z' \rangle$ be the canonical bilinear form on $F \times F'$. If $f \in \mathcal{L}_F^p$ and $g \in \mathcal{L}_{F'}^q$, then the real (resp. complex) function $\langle f, g \rangle$ is integrable and

$$
\left| \int \langle f, g \rangle\, d\mu \right| \leq \int |\langle f, g \rangle|\, d|\mu| \leq N_p(f) N_q(g).
$$

For, $|\langle z, z' \rangle| \leq |z| \cdot |z'|$.

When $F$ is a real or complex Hilbert space, one knows that it can be canonically identified with its dual $F'$ (TVS, V, § 1, No. 7). Since the space $L_F^2$ is complete, we have the following result:

#### Corollary 3 {#int-iv-s6-thm-2-cor-3 .statement}

— Let $\mu$ be a positive measure on $X$, $F$ a real (resp. complex) Hilbert space. On the space $L_F^2$, the symmetric (resp. Hermitian) form

$$
(\widetilde{f}, \widetilde{g}) \mapsto \int \langle f, g \rangle\, d\mu
$$

defines a Hilbert space structure, for which the norm is equal to $\| \widetilde{f} \|_2$.

#### Corollary 4 {#int-iv-s6-thm-2-cor-4 .statement}

— Let $F$ be a Banach space, $f$ a function in $\mathcal{L}_F^p$, and $g$ a numerical function belonging to $\mathcal{L}^q$; then, the function $fg$ is integrable and

$$
\left| \int fg\, d\mu \right| \leq \int |fg|\, d|\mu| \leq N_p(f) N_q(g).
$$

#### Corollary 5 {#int-iv-s6-thm-2-cor-5 .statement}

— Let $f_1, f_2, \ldots, f_n$ be n positive integrable functions, and let $\alpha_1, \alpha_2, \ldots, \alpha_n$ be n numbers $> 0$ such that $\sum_{i=1}^n \alpha_i = 1$; under these conditions, the function $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ is integrable and

$$
\int f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n} d|\mu| \leqslant
\left( \int f_1 d|\mu| \right)^{\alpha_1} \left( \int f_2 d|\mu| \right)^{\alpha_2} \cdots \left( \int f_n d|\mu| \right)^{\alpha_n}.
$$

For, the product $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ is measurable, being the product of measurable functions (§ 5, No. 3, Th. 1 and its Cor. 5); since the inequality (8) is true for upper integrals (Ch. I, No. 2, Cor. of Prop. 2), the function $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ is integrable (§ 5, No. 6, Th. 5), whence the corollary.

Cor. 2 of Th. 2 is sharpened by the following proposition:

#### Proposition 3 {#int-iv-s6-prop-3 .statement}

— Let $\mu$ be a positive measure on X, F a real or complex Banach space, F' its strong dual, and $(z, z') \mapsto \langle z, z' \rangle$ the canonical bilinear form on $F \times F'$.

1° For every function $f \in \mathcal{L}_F^p$ ($1 \leq p \leq +\infty$),

$$
N_p(f) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$

as g runs over the set of functions in $\mathcal{L}_{F'}^q$, such that $N_q(g) \leq 1$.

2° For every function $g \in \mathcal{L}_{F'}^q$ ($1 \leq q \leq +\infty$),

$$
N_q(g) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$

as f runs over the set of functions in $\mathcal{L}_F^p$ such that $N_p(f) \leq 1$.

Let us first prove the relation (9); we distinguish between two cases.

(i) $1 \leq p < +\infty$. The relation (9) being trivial when $N_p(f) = 0$ (because f and $\langle f, g \rangle$ are then negligible), we can always suppose, on multiplying f by a scalar, that $N_p(f) = 1$. Suppose first that f is an integrable step function, $f = \sum_{k=1}^n a_k \varphi_{A_k}$, where the $A_k$ are pairwise disjoint (§ 4, No. 9, Lemma). Thus $\sum_{k=1}^n |a_k|^p \mu(A_k) = 1$ by hypothesis. For every $\varepsilon > 0$, there exists (for every index k) a vector $a'_k \in F'$ such that $|a'_k|^q = |a_k|^p$ if $p > 1$ (resp. $|a'_k| = 1$ if $p = 1$) and $\langle a_k, a'_k \rangle \geq (1 - \varepsilon)|a_k| \cdot |a'_k|$ (TVS, IV,

§1, No. 3, Prop. 8). Setting $g = \sum_{k=1}^n a_k' \varphi_{A_k}$, we have $\sum_{k=1}^n |a_k'|^q \mu(A_k) = 1$ if $p > 1$ (resp. $\sup_{1 \leq k \leq n} |a_k'| = 1$ if $p = 1$), thus $N_q(g) = 1$; on the other hand,

$$
\int \langle f, g \rangle d\mu = \sum_{k=1}^n \langle a_k, a_k' \rangle \mu(A_k) \geq (1 - \varepsilon) \sum_{k=1}^n |a_k| \cdot |a_k'| \mu(A_k)
$$

and, since $|a_k'| = |a_k|^{p/q} = |a_k|^{p-1}$ if $p > 1$ (resp. $|a_k'| = 1$ if $p = 1$), we have

$$
\int \langle f, g \rangle d\mu \geq (1 - \varepsilon) \sum_{k=1}^n |a_k|^p \mu(A_k) = (1 - \varepsilon) N_p(f) = 1 - \varepsilon,
$$

which proves the relation (9) in this case.

Let us pass to the case that $f$ is any element of $\mathcal{L}_F^p$ such that $N_p(f) = 1$. For every $\varepsilon > 0$, there exists a step function $f_1 \in \mathcal{L}_F^p$ such that $N_p(f - f_1) \leq \varepsilon$ (§ 4, No. 10, Cor. 1 of Prop. 19). By what we have just seen, there exists a function $g \in \mathcal{L}_F^q$, such that $N_q(g) = 1$ and

$$
\int \langle f_1, g \rangle d\mu \geq N_p(f_1) - \varepsilon \geq 1 - 2\varepsilon.
$$

Now,

$$
\int \langle f, g \rangle d\mu = \int \langle f_1, g \rangle d\mu + \int \langle f - f_1, g \rangle d\mu
$$

and, by (6),

$$
\left| \int \langle f - f_1, g \rangle d\mu \right| \leq N_p(f - f_1) N_q(g),
$$

whence

$$
\left| \int \langle f, g \rangle d\mu \right| \geq 1 - 3\varepsilon,
$$

which proves (9).

(ii) $p = +\infty$. We may again restrict ourselves to the case that $N_\infty(f) > 0$. Let $\alpha$ be any number such that $0 < \alpha < N_\infty(f)$; by hypothesis, the set of $x \in X$ such that $|f(x)| > \alpha$ is measurable and is not locally negligible, therefore it contains a compact set $K$ of measure $> 0$. Since $f$ is measurable, there exists a compact set $K_1 \subset K$ of measure $> 0$, such that the restriction of $f$ to $K_1$ is continuous. It follows that, for every $\varepsilon > 0$, there exists a partition of $K_1$ into a finite number of integrable sets, in each of which the oscillation of $f$ is $\leq \varepsilon$; at least one of these sets $A$ has measure > 0. Let $a$ be one of the values of $f$ in $A$; then $|a| > \alpha$ and $|f(x) - a| \leq \varepsilon$ for all $x \in A$. There exists a vector $a' \in F'$ such that $|a'| = 1$ and $|\langle a, a' \rangle| \geq |a| - \varepsilon$; the function $g = \varphi_A \cdot a'/\mu(A)$ is integrable and $N_1(g) = 1$; on the other hand,

$$
\int \langle f, g \rangle d\mu = \frac{1}{\mu(A)} \int \langle f, a' \rangle \varphi_A d\mu.
$$

Now, one can write

$$
\int \langle f, a' \rangle \varphi_A d\mu = \langle a, a' \rangle \mu(A) + \int \langle f - a, a' \rangle \varphi_A d\mu,
$$

and since

$$
|\langle f - a, a' \rangle \varphi_A| \leq \varepsilon \varphi_A,
$$

we see that

$$
\left| \int \langle f, g \rangle d\mu \right| \geq |\langle a, a' \rangle| - \varepsilon \geq |a| - 2\varepsilon > \alpha - 2\varepsilon;
$$

since $\varepsilon$ is arbitrary and $\alpha$ is any number < $N_\infty(f)$, the relation (9) is also verified in this case.

One argues in exactly the same manner to prove the relation (10), on considering separately the case $1 \leq q < +\infty$ and the case $q = +\infty$, and using the fact that for every $z' \in F'$, $|z'| = \sup_{|z| \leq 1} |\langle z, z' \rangle|$ by the definition of the norm in $F'$.

#### Remark {#int-iv-s6-n4-rem-1 .statement}

— 1) Let $\mathcal{E}$ be a dense linear subspace of $\mathcal{L}_{F'}^q$; then the formula (9) holds when $g$ runs over the intersection of $\mathcal{E}$ with the set $B$ of functions in $\mathcal{L}_{F'}^q$ such that $N_q(g) \leq 1$. For, it suffices to observe that the interior $\overset{\circ}{B}$ of $B$ is dense in $B$ and that $\overset{\circ}{B} \cap \mathcal{E}$ is dense in $\overset{\circ}{B}$, since $\overset{\circ}{B}$ is open. This remark applies in particular to the set $\mathcal{E} = \mathcal{K}(X; F')$ of continuous functions with compact support (with values in $F'$) when $1 \leq q < +\infty$, that is, $1 < p \leq +\infty$. But in this case, the formula (9) is true as $g$ runs over $B \cap \mathcal{K}(X; F')$, even for $p = 1$. For, we may, as above, restrict ourselves to the case that $f$ is a step function. We saw then that if $N_1(f) = 1$, then for every $\varepsilon > 0$ there exists a step function $g \in \mathcal{L}_{F'}^\infty$ such that $|g(x)| \leq 1$ for all $x \in X$ and $|\int \langle f, g \rangle d\mu| \geq 1 - \varepsilon$. There exists a finite number of pairwise disjoint compact sets $K_i$ such that $g$ has a constant value $a'_i$ on each $K_i$ and such that, if $K$ is the union of the $K_i$, then $\int |f| \varphi_{\mathcal{C}_K} d\mu \leq \varepsilon$. Let $U_i$ be a neighborhood of $K_i$ such that the sets $U_i$ are pairwise disjoint, and let $h_i$ be a continuous mapping of $X$ into $[0, 1]$ with support contained in $U_i$ and equal to 1 on $K_i$. Setting $h = \sum a'_i h_i$, we have $h(x) = g(x)$ on $K$ and $|h(x)| \leq 1$ on $X$, therefore

$$
\int |\langle f, h \rangle| \varphi_{\mathcal{C}_K} d\mu \leq \varepsilon
$$

and consequently $|\int \langle f, h \rangle d\mu| \geq 1 - 3\varepsilon$, which proves our assertion. Analogous remarks can be made for the formula (10).

2) Let $\mu$ be a positive measure on $X$, $f$ a measurable function $\geq 0$ (finite or not) whose support is contained in a countable union of compact sets $K_n$. Then, for every $p$ such that $1 \leq p \leq +\infty$,

$$
(11) \quad N_p(f) = \sup \int^* |fg| d\mu,
$$

as $g$ runs over the set of functions in $\mathcal{H}(X; \mathbf{R})$ such that $N_q(g) \leq 1$. For, the formula (11) is a special case of (9) when $N_p(f) < +\infty$, since $f$ is then equivalent to a function in $\mathcal{L}^p$ (§ 5, No. 6, Th. 5). If $N_p(f) = +\infty$, for every integer $n > 0$ set $f_n = \inf(n, f \varphi_{K_n})$. Then

$$
N_p(f_n) = \sup \int^* |f_n g| d\mu \leq \sup \int^* |f g| d\mu,
$$

whence, on passing to the limit (assuming, as we may, that the sequence $(K_n)$ is increasing), we have $\sup \int^* |f g| d\mu = +\infty$ (§ 1, No. 3, Th. 3).

#### Corollary {#int-iv-s6-n4-cor-1 .statement}

— *Let $\mu$ be a positive measure on $X$, $F$ a Banach space, $F'$ its strong dual, and $g$ any function in $\mathcal{L}^q_{F'}$. Then, the linear form on $L^p_F$, deduced from the linear form $f \mapsto \int \langle f, g \rangle d\mu$ on $\mathcal{L}^p_F$ by passage to the quotient, is continuous and has norm $N_q(g)$.*

### 5. Application: relations between the spaces $L^p_F$ ($1 \leq p \leq +\infty$)

#### Proposition 4 {#int-iv-s6-prop-4 .statement}

— *Let $f$ be a measurable function with values in a Banach space $F$; the set $I$ of numbers $p$, such that $1 \leq p \leq +\infty$ and $N_p(f)$ is finite, is either empty or is an interval of $\overline{\mathbf{R}}$. If $I$ is nonempty, the restriction to $I$ of the mapping $p \mapsto N_p(f)$ is continuous; moreover, if $f$ is not negligible, $\log N_p(f)$ is a convex function of $1/p$ on $\bar{I}$.

We already know (Ch. I, No. 3, Prop. 5) that the set $J$ of *finite* numbers $p \geq 1$ such that $N_p(f) < +\infty$ is either empty or is an interval, and that $\log N_p(f)$ is a convex function of $1/p$ on $J$ (when $f$ is not negligible); this of course implies the continuity of $p \mapsto N_p(f)$ on $J$.

If $J$ is empty then either $I = \varnothing$ or $I = \{+\infty\}$, and the proposition is obvious in this case; assume henceforth that $J$ is nonempty. The proposition is also obvious if $f$ is negligible; assume henceforth that $f$ is not negligible. If $s \in J$ then, for every finite number $p > s$, $|f|^p = |f|^s |f|^{p-s}$, and the inequality of the mean shows that

$$
(12) \quad N_p(f) \leq (N_s(f))^{s/p} (N_\infty(f))^{(p-s)/p}.
$$

Letting $p$ tend to $+\infty$, it follows that

$$
\limsup_{p \to +\infty} N_p(f) \leq N_\infty(f).
$$

This proves that if $+\infty \in I$ then $J$ contains arbitrarily large numbers; thus $I$ is indeed an interval of $\overline{\mathbf{R}}$, and $\overline{I} = \overline{J}$. The proposition will be proved if we show that $p \mapsto N_p(f)$ is continuous on $\overline{J}$, and it suffices to establish continuity at the end-points of $J$. We can suppose, moreover, that $J$ does not reduce to a point. Let $r$ and $s$ be the left and right end-points of $J$ ($r < s \leq +\infty$). Let $A$ be the (measurable) set of $x \in X$ such that $|f(x)| \geq 1$; then

$$
\int |f|^p d|\mu| = \int |f|^p \varphi_A d|\mu| + \int |f|^p \varphi_{C_A} d|\mu|.
$$

As $p \in J$ tends to $r$, $|f|^p \varphi_A$ tends to $|f|^r \varphi_A$ while decreasing, and $|f|^p \varphi_{C_A}$ tends to $|f|^r \varphi_{C_A}$ while increasing. Thus $\int |f|^p \varphi_{C_A} d|\mu|$ tends to $\int^* |f|^r \varphi_{C_A} d|\mu|$ (§ 1, No. 3, Th. 3). On the other hand, $|f|^p \varphi_A$ is integrable for $p \in J$, and $\int |f|^p \varphi_A d|\mu|$ tends to $\int |f|^r \varphi_A d|\mu|$ (§ 4, No. 3, Prop. 4). Therefore $\int |f|^p d|\mu|$ tends to $\int^* |f|^r d|\mu|$, which proves the continuity of $p \mapsto N_p(f)$ at $r$.

The same reasoning may be applied at the point $s$ if $s < +\infty$. Finally, suppose that $s = +\infty$. In view of (13), it suffices to prove that

$$
\liminf_{p \to +\infty} N_p(f) \geq N_\infty(f).
$$

Now, let $a$ be a number such that $0 < a < N_\infty(f)$. Since, by hypothesis, there exist finite values of $p$ such that $N_p(f) < +\infty$, the set $A$ of $x \in X$ such that $|f(x)| \geq a$, which is measurable and non-negligible, is integrable by virtue of the inequality $\varphi_A \leq (|f|/a)^p$; moreover, we infer from this inequality that $N_p(f) \geq a \cdot (|\mu|(A))^{1/p}$; letting $p$ tend to $+\infty$, it follows that $\liminf_{p \to +\infty} N_p(f) \geq a$, which completes the proof.

#### Corollary {#int-iv-s6-n5-cor-1 .statement}

— *If* $r, s, p$ *are three numbers such that*

$$
1 \leq r < p < s \leq +\infty,
$$

*then the intersection* $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ *is contained in* $\mathcal{L}_F^p$.

Note that in general the topologies induced on the intersection $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ by the topologies of the $\mathcal{L}_F^p$ ($r < p < s$) are *distinct*. If no further hypothesis is made on $\mu$, the topologies induced on $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ by those of $\mathcal{L}_F^r$ and $\mathcal{L}_F^s$ are in general not comparable (in other words, the ratio $N_r(f)/N_s(f)$ can take arbitrarily large values and arbitrarily small values in $\mathcal{L}_F^r \cap \mathcal{L}_F^s$; cf. Exer. 8).

Prop. 4 may be sharpened when $\mu$ is a bounded measure:

#### Proposition 5 {#int-iv-s6-prop-5 .statement}

— Let $\mu$ be a bounded measure, and let $f$ be a $\mu$-measurable function with values in a Banach space $F$. The set I of numbers $p$ such that $1 \leq p \leq +\infty$ and $N_p(f)$ is finite, is either empty or is an interval with left end-point $p = 1$ and containing this point; moreover, $(|\mu|(X))^{-1/p} N_p(f)$ is an increasing function of $p$ on I.

This is an immediate consequence of Prop. 4 above and of the Cor. of Prop. 4 of Ch. I, No. 3.

#### Corollary {#int-iv-s6-n5-cor-2 .statement}

— If the measure $\mu$ is bounded, the relation $r < s$ implies $\mathcal{L}_F^s \subset \mathcal{L}_F^r$; moreover, the topology of convergence in mean of order $s$ is finer than the topology of convergence in mean of order $r$ (on $\mathcal{L}_F^s$).

One can show that in general the topology of convergence in mean of order $s$ is strictly finer than the topology of convergence in mean of order $r$ (Exer. 8).

#### Proposition 6 {#int-iv-s6-prop-6 .statement}

— Let $X$ be a discrete space, $\mu$ the measure on $X$ defined by placing a mass $+1$ at each point of $X$. If $f$ is a mapping of $X$ into the Banach space $F$, the set I of numbers $p$ such that $1 \leq p \leq +\infty$ and $N_p(f)$ is finite, is either empty or is an interval with right end-point $+\infty$ and containing this point; moreover, $N_p(f)$ is a decreasing function of $p$ on I.

For, $\mu^*(|f|) = \sum_{x \in X} |f(x)|$ for every function $f$ (§ 1, No. 1, Example), and $N_\infty(f) = \|f\| = \sup_{x \in X} |f(x)|$; if there exists a number $\alpha > 0$ such that $|f(x)| \geq \alpha$ for infinitely many values of $x \in X$, then $N_p(f) = +\infty$ for every finite $p$; in the contrary case, there exists an $x_0 \in X$ such that $|f(x_0)| = \|f\|$, whence

$$
N_\infty(f) = |f(x_0)| \leq N_p(f)
$$

for every finite $p$. Since the function $\log N_p(f)$ is convex with respect to $1/p$ and takes its smallest value at the point $+\infty$, it is necessarily a decreasing function of $p$ on I (FRV, I, § 4, No. 3, Prop. 5), which completes the proof.

#### Corollary {#int-iv-s6-n5-cor-3 .statement}

— If $X$ is discrete and the measure $\mu$ is defined by a mass $+1$ at each point of $X$, then the relation $r < s$ implies $\mathcal{L}_F^r \subset \mathcal{L}_F^s$; moreover, the topology of convergence in mean of order $r$ is finer than the topology of convergence in mean of order $s$ (on $\mathcal{L}_F^r$).

### Exercises {#int-iv-s6-exercises}

See the [exercises for § 6](exercises/s6/).
