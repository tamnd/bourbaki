---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 4
section_title: Products of measures
lang: en
source: int-i-vi
book_pages: INT III.60-INT III.62
pdf_pages: 0085-0100, 0105-0107
extraction: ocr
subsections:
    - "no": 1
      title: The product of two measures
      page: 40
      pdf_page: 85
    - "no": 2
      title: Properties of product measures
      page: 44
      pdf_page: 89
    - "no": 3
      title: Continuity of product measures
      page: 47
      pdf_page: 92
    - "no": 4
      title: Product of a finite number of measures
      page: 48
      pdf_page: 93
    - "no": 5
      title: Inverse limits of measures
      page: 50
      pdf_page: 95
    - "no": 6
      title: Infinite products of measures
      page: 53
      pdf_page: 98
statements: 22
exercises: 8
content_sha256: 6cce27b93cc8eb2432ea6f68fe801fc213586fdca8c9bffffb15f6d695b84b75
---

## § 4. PRODUCTS OF MEASURES

### 1. The product of two measures

#### Theorem 1 {#int-iii-s4-thm-1 .statement}

— *Let X and Y be two locally compact spaces, $\lambda$ a measure on X, $\mu$ a measure on Y; there exists one and only one measure $\nu$ on $X \times Y$ such that, for every function* $g \in \mathcal{K}(X; \mathbf{C})$ *and every function* $h \in \mathcal{K}(Y; \mathbf{C})$,

$$
\int g(x)h(y)\, d\nu(x, y) = \left( \int g(x)\, d\lambda(x) \right) \left( \int h(y)\, d\mu(y) \right).
$$

#### Lemma {#int-iii-s4-n1-lem-1 .statement}

1— *Let X and Y be two locally compact spaces, K (resp. L) a compact subset of X (resp. Y).*

(i) *The restriction to* $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ *of the canonical bijection*

$$
\omega : \mathcal{F}(X \times Y; \mathbf{C}) \to \mathcal{F}(X; \mathcal{F}(Y; \mathbf{C}))
$$

(S, R, §4, No. 14) *is an isometry of the Banach space* $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ *onto the Banach space* $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$.

(ii) *The vector space* $\mathcal{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y, L; \mathbf{C})$, *identified canonically with a subspace of* $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ *(A, II, §7, No. 7, comments following the Cor. of Prop. 15), is dense in this Banach space*.

It is immediate that the image under $\omega$ of $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ is contained in $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$. Conversely, if $u$ is a continuous mapping of $X$ into $\mathcal{K}(Y, L; \mathbf{C})$, with support contained in $K$, then the mapping $(x, y) \mapsto u(x)(y)$ of $X \times Y$ into $\mathbf{C}$ is continuous and has support contained in $K \times L$, therefore the restriction of $\omega$ to $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ is a bijection of this space onto $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$; the fact that this restriction is a Banach space isometry follows from the relation

$$
\sup_{(x, y) \in K \times L} |f(x, y)| = \sup_{x \in K} \left( \sup_{y \in L} |f(x, y)| \right).
$$

This proves (i); on the other hand the image under $\omega$, of

$$
\mathcal{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y, L; \mathbf{C})
$$

identified with a subspace of $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$, is again the space $\mathcal{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y, L; \mathbf{C})$ but this time identified canonically with a space of mappings of $X$ into $\mathcal{K}(Y, L; \mathbf{C})$ (A, II, §7, No. 7, Cor. of Prop. 15); but this subspace of $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$ is known to be *dense* in the latter space (§ 1, No. 2, Prop. 5), thus the conclusion of (ii) follows from the fact that the restriction of $\omega$ is a topological isomorphism.

Having proved the lemma, we now observe that every compact subset of $X \times Y$ is contained in a product $K \times L$, where $K$ (resp. $L$) is a compact subset of $X$ (resp. $Y$). It therefore follows from Lemma 1, (ii) that the subspace $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ is *dense* in $\mathcal{K}(X \times Y; \mathbf{C})$; since the relation (1) may also be written as $\nu(g \otimes h) = \lambda(g)\mu(h)$ for $g \in \mathcal{K}(X; \mathbf{C})$, $h \in \mathcal{K}(Y; \mathbf{C})$, the *uniqueness* of $\nu$ follows at once. To prove the existence of $\nu$, we shall make use of the following lemma:

#### Lemma 2 {#int-iii-s4-lem-2 .statement}

*With notations as in Lemma 1, for every function* $f \in \mathcal{K}(X \times Y, K \times L; \mathbf{C})$ *the function*

$$
y \mapsto h(y) = \int f(x, y) \, d\lambda(x)
$$

*belongs to* $\mathcal{K}(Y, L; \mathbf{C})$.

For every function $u \in \mathcal{K}(X; \mathcal{K}(Y, L; \mathbf{C}))$, the integral $\int u(x) d\lambda(x)$ belongs to $\mathcal{K}(Y, L; \mathbf{C})$ since the latter is a Banach space (§ 3, No. 3, Cor. 1 of Prop. 7); but for $u = \omega(f)$ and for every $y \in Y$,

$$
\left\langle \int u(x) d\lambda(x), \varepsilon_y \right\rangle = \int u(x)(y) d\lambda(x) = \int f(x, y) d\lambda(x),
$$

whence the lemma.

Consider, then, for every function $f \in \mathcal{K}(X \times Y; \mathbf{C})$, the number $\nu(f) = \mu(\int f(x, y) d\lambda(x))$ (which we shall also write $\int d\mu(y) \int f(x, y) d\lambda(x)$ by an abuse of notation); if K (resp. L) is a compact subset of X (resp. Y), then there exists a number $a_K$ (resp. $b_L$) such that, for every function $g \in \mathcal{K}(X, K; \mathbf{C})$ (resp. $h \in \mathcal{K}(Y, L; \mathbf{C})$), we have $|\lambda(g)| \leq a_K \|g\|$ (resp. $|\mu(h)| \leq b_L \|h\|$). It follows that for every function $f \in \mathcal{K}(X \times Y, K \times L; \mathbf{C})$,

$$
\left| \int f(x, y) d\lambda(x) \right| \leq a_K \|f\|
$$

for every $y \in Y$, whence $|\nu(f)| \leq a_K b_L \|f\|$. The linear form $\nu$ on $\mathcal{K}(X \times Y; \mathbf{C})$ is thus a measure on $X \times Y$ that obviously satisfies (1), which completes the proof of Th. 1.

#### Definition 1 {#int-iii-s4-def-1 .statement}

*Given two measures $\lambda, \mu$ defined, respectively, on two locally compact spaces $X, Y$, the product measure of $\lambda$ by $\mu$ is defined to be the unique measure $\nu$ on $X \times Y$ satisfying the relation (1) for every function $g \in \mathcal{K}(X; \mathbf{C})$ and every function $h \in \mathcal{K}(Y; \mathbf{C})$.*

In the proof of Th. 1, the roles of the spaces X and Y may be interchanged; canonically identifying $Y \times X$ and $X \times Y$, we thus define on $X \times Y$ a measure

$$
f \mapsto \int d\lambda(x) \int f(x, y) d\mu(y)
$$

that again satisfies condition (1). We have thus proved the following theorem:

#### Theorem 2 {#int-iii-s4-thm-2 .statement}

*Let $\lambda, \mu$ be two measures defined, respectively, on two locally compact spaces $X, Y$. For every function $f$ in $\mathcal{K}(X \times Y; \mathbf{C})$, the integral of $f$ with respect to the product measure $\nu$ of $\lambda$ by $\mu$ has the value*

$$
\int f(x, y) d\nu(x, y) = \int d\lambda(x) \int f(x, y) d\mu(y)
$$
$$(3)$$
$$
= \int d\mu(y) \int f(x, y) d\lambda(x).
$$

Because of the last formula, the integral of $f$ with respect to the product measure $\nu$ is usually denoted $\iint f\, d\lambda\, d\mu$, or $\iint f\, d\mu\, d\lambda$, or $\iint f\, \lambda\mu$, or $\iint f\, \mu\lambda$, or $\iint f(x, y)\, d\lambda(x)\, d\mu(y)$, or $\iint f(x, y)\, d\mu(y)\, d\lambda(x)$, or $\iint f(x, y)\, \lambda(x)\mu(y)$, or $\iint f(x, y)\, \mu(y)\lambda(x)$; it is said to be the double integral of $f$ with respect to $\lambda$ and $\mu$. With this notation, the formula (3) may be written

$$
\iint f(x, y)\, d\lambda(x)\, d\mu(y) = \int d\lambda(x) \int f(x, y)\, d\mu(y)
$$
$$
= \int d\mu(y) \int f(x, y)\, d\lambda(x).
$$

Formula (3) shows that if $\lambda$ and $\mu$ are real (resp. positive) measures, then the product measure $\nu$ is real (resp. positive).

#### Example 1 {#int-iii-s4-n1-exa-1 .statement}

The product measure of the Dirac measures $\varepsilon_x$ ($x \in X$) and $\varepsilon_y$ ($y \in Y$) is the Dirac measure $\varepsilon_{(x, y)}$.

#### Example 2 {#int-iii-s4-n1-exa-2 .statement}

Let us take $X = Y = \mathbf{R}$, and for $\lambda$ and $\mu$ the *Lebesgue measure* on $\mathbf{R}$ (§1, No. 3); their product is called *Lebesgue measure* on $\mathbf{R}^2$; the integral of a function $f \in \mathcal{K}(\mathbf{R}^2; \mathbf{C})$ with respect to this measure is denoted $\iint f(x, y)\, dx\, dy$ or $\iint f(x, y)\, dy\, dx$; formula (4), for a function that is zero outside a compact rectangle $[a, b] \times [c, d]$, yields the formula

$$
\int_c^d dy \int_a^b f(x, y)\, dx = \int_a^b dx \int_c^d f(x, y)\, dy
$$

proved in FRV, II, §3, No. 6.

Since Lebesgue measure on $\mathbf{R}$ is invariant under every translation (§1, No. 3), it follows at once that Lebesgue measure on $\mathbf{R}^2$ is *invariant under every translation of $\mathbf{R}^2$*.

#### Remark {#int-iii-s4-n1-rem-1 .statement}

Let $E$ be a Hausdorff locally convex space, and let $f$ be a mapping in $\mathcal{K}(X \times Y; E)$ such that $f(X \times Y)$ is contained in a *complete convex* subset $C$ of $E$. Then, for every $y \in Y$, the integral $h(y) = \int f(x, y)\, d\lambda(x)$ belongs to $E$ (§3, No. 3, Prop. 7); moreover, the function $h$ belongs to $\widetilde{\mathcal{K}}(Y; E)$: indeed, for every $z' \in E'$ we have

$$
\langle h(y), z' \rangle = \int \langle f(x, y), z' \rangle\, d\lambda(x),
$$

therefore $y \mapsto \langle h(y), z' \rangle$ belongs to $\mathcal{K}(Y; C)$ by Lemma 2. The integral $\int h\, d\mu$ is therefore defined (and *a priori* belongs to ${E'}^*$); let us show that

$$
\iint f(x, y)\, d\lambda(x)\, d\mu(y) = \int d\mu(y) \int f(x, y)\, d\lambda(x)
$$
$$
= \int d\lambda(x) \int f(x, y)\, d\mu(y),
$$

thus generalizing the formula (4). Indeed, for every $z' \in E'$ we have
$$
\left\langle \int \int f d\lambda d\mu, z' \right\rangle = \int \int \langle f, z' \rangle d\lambda d\mu = \int d\mu \int \langle f, z' \rangle d\lambda \\
= \int \left\langle \int f d\lambda, z' \right\rangle d\mu = \left\langle \int d\mu \int f d\lambda, z' \right\rangle
$$
by (4), whence (5).

### 2. Properties of product measures

If $\lambda$ (resp. $\mu$) is a measure on X (resp. Y) and $\nu$ is the product measure of $\lambda$ by $\mu$, then the restriction of $\nu$ to $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ is none other than the *tensor product* $\lambda \otimes \mu$ of the two linear forms $\lambda$ and $\mu$ (A, II, §3, No. 2), because the relation (1) of No. 1 may be written
$$
\langle g \otimes h, \nu \rangle = \langle g, \lambda \rangle \langle h, \mu \rangle = \langle g \otimes h, \lambda \otimes \mu \rangle
$$
for all $g \in \mathcal{K}(X; \mathbf{C})$ and $h \in \mathcal{K}(Y; \mathbf{C})$. By an abuse of notation, we shall also denote by $\lambda \otimes \mu$ the product measure $\nu$ (and not just its restriction to the dense subspace $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ of $\mathcal{K}(X \times Y; \mathbf{C})$).

The mapping $(\lambda, \mu) \mapsto \lambda \otimes \mu$ of $\mathcal{M}(X; \mathbf{C}) \times \mathcal{M}(Y; \mathbf{C})$ into $\mathcal{M}(X \times Y; \mathbf{C})$ is obviously *bilinear*, by virtue of formula (3) of No. 1.

#### Proposition 1 {#int-iii-s4-prop-1 .statement}

*Let $\lambda$ be a measure on X, $\mu$ a measure on Y; if $g \in \mathcal{C}(X; \mathbf{C}),\ h \in \mathcal{C}(Y; \mathbf{C}),$ then*
$$
(g \cdot \lambda) \otimes (h \cdot \mu) = (g \otimes h) \cdot (\lambda \otimes \mu).
$$

For every function $f \in \mathcal{K}(X \times Y; \mathbf{C})$, we have, by virtue of formula (3) of No. 1,
$$
\langle f, (g \otimes h) \cdot (\lambda \otimes \mu) \rangle = \int d\lambda(x) \int f(x, y) g(x) h(y) d\mu(y) \\
= \int g(x) d\lambda(x) \int f(x, y) h(y) d\mu(y),
$$
which proves formula (6).

#### Proposition 2 {#int-iii-s4-prop-2 .statement}

*The support of the product $\lambda \otimes \mu$ is equal to the product of the support of $\lambda$ and the support of $\mu$.*

We first observe that the relation $\lambda \otimes \mu = 0$ implies that one of the measures $\lambda, \mu$ is zero (A, II, §7, No. 7, Prop. 16, (ii)). On the other hand, if U (resp. V) is an open set in X (resp. Y), then the restriction of $\lambda \otimes \mu$ to the product $U \times V$ is the product of the restrictions of $\lambda$ to U and of $\mu$ to V, as follows from Th. 1 of No. 1 and the definition of the restriction of a measure to an open set (§ 2, No. 1). It therefore follows that, for the restriction of $\lambda \otimes \mu$ to $U \times V$ to be zero, it is necessary and sufficient that either the restriction of $\lambda$ to U or the restriction of $\mu$ to V be zero, which proves the proposition, on taking into account the definition of the support of a measure (§ 2, No. 2).

#### Proposition 3 {#int-iii-s4-prop-3 .statement}

*Let $\lambda \in \mathcal{M}(X; \mathbf{C}),\ \mu \in \mathcal{M}(Y; \mathbf{C})$. Then*

$$
|\lambda \otimes \mu| = |\lambda| \otimes |\mu|.
$$

Let $f \in \mathcal{K}_+(X \times Y),\ g \in \mathcal{K}(X \times Y; \mathbf{C})$ be such that $|g| \leq f$; we have (§ 1, No. 6, formula (13))

$$
\begin{align*}
|\langle g, \lambda \otimes \mu \rangle| &= \left| \int d\lambda(x) \int g(x, y) d\mu(y) \right| \\
&\leq \int d|\lambda|(x) \int |g(x, y)|\ d|\mu|(y) \\
&= \langle |g|, |\lambda| \otimes |\mu| \rangle \leq \langle f, |\lambda| \otimes |\mu| \rangle.
\end{align*}
$$

It follows that $\langle f, |\lambda \otimes \mu| \rangle \leq \langle f, |\lambda| \otimes |\mu| \rangle$, and so

$$
|\lambda \otimes \mu| \leq |\lambda| \otimes |\mu|.
$$

On the other hand, let $u \in \mathcal{K}_+(X),\ v \in \mathcal{K}_+(Y)$. For every $\varepsilon > 0$, there exist $u_1 \in \mathcal{K}(X; \mathbf{C}),\ v_1 \in \mathcal{K}(Y; \mathbf{C})$ such that $|u_1| \leq u,\ |v_1| \leq v$ and

$$
|\langle u_1, \lambda \rangle| \geq \langle u, |\lambda| \rangle - \varepsilon,\quad |\langle v_1, \mu \rangle| \geq \langle v, |\mu| \rangle - \varepsilon
$$
(§ 1, No. 6). It follows that $|u_1 \otimes v_1| \leq u \otimes v$ and

$$
\begin{align*}
\langle u \otimes v, |\lambda \otimes \mu| \rangle &\geq |\langle u_1 \otimes v_1, \lambda \otimes \mu \rangle| = |\langle u_1, \lambda \rangle \langle v_1, \mu \rangle| \\
&\geq ((\langle u, |\lambda| \rangle - \varepsilon)(\langle v, |\mu| \rangle - \varepsilon)).
\end{align*}
$$

Since $\varepsilon$ is arbitrary, we infer that

$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle \geq \langle u, |\lambda| \rangle \langle v, |\mu| \rangle = \langle u \otimes v, |\lambda| \otimes |\mu| \rangle.
$$

Taking (8) into account, we see that

$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle = \langle u \otimes v, |\lambda| \otimes |\mu| \rangle.
$$

Since every function in $\mathcal{K}(X; \mathbf{C})$ (resp. $\mathcal{K}(Y; \mathbf{C})$) is a linear combination of functions in $\mathcal{K}_+(X)$ (resp. $\mathcal{K}_+(Y)$), the preceding formula remains true for $u \in \mathcal{K}(X; \mathbf{C})$ and $v \in \mathcal{K}(Y; \mathbf{C})$; the proposition therefore follows from the fact that $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ is dense in $\mathcal{K}(X \times Y; \mathbf{C})$.

#### Corollary {#int-iii-s4-n2-cor-1 .statement}

— *Let* $\lambda \in \mathcal{M}(X; \mathbf{R}), \ \mu \in \mathcal{M}(Y; \mathbf{R})$. *Then*

$$
\begin{cases}
(\lambda \otimes \mu)^+ = \lambda^+ \otimes \mu^+ + \lambda^- \otimes \mu^- , \\
(\lambda \otimes \mu)^- = \lambda^+ \otimes \mu^- + \lambda^- \otimes \mu^+ .
\end{cases}
$$

For, by virtue of Prop. 3,

$$
\begin{align*}
(\lambda \otimes \mu)^+ &= \frac{1}{2} (\lambda \otimes \mu + |\lambda| \otimes |\mu|) \\
&= \frac{1}{2} ((\lambda^+ - \lambda^-) \otimes (\mu^+ - \mu^-) + (\lambda^+ + \lambda^-) \otimes (\mu^+ + \mu^-)) \\
&= \lambda^+ \otimes \mu^+ + \lambda^- \otimes \mu^- .
\end{align*}
$$

The argument for $(\lambda \otimes \mu)^-$ is similar.

#### Proposition 4 {#int-iii-s4-prop-4 .statement}

— *Let* $\lambda \in \mathcal{M}(X; \mathbf{C}), \ \mu \in \mathcal{M}(Y; \mathbf{C})$. *Then*

$$
\|\lambda \otimes \mu\| = \|\lambda\| \cdot \|\mu\|,
$$

*with the convention that the second member is to be replaced by 0 whenever one of the factors is 0 and the other is $+\infty$*. *In particular, if* $\lambda$ *and* $\mu$ *are bounded then* $\lambda \otimes \mu$ *is bounded*.

By the above Proposition 3, and §1, No. 8, Cor. 1 of Prop. 10, we may limit ourselves to the case that $\lambda$ and $\mu$ are positive measures. If $\lambda = 0$ or $\mu = 0$, the result is trivial; let us therefore assume that $\lambda \neq 0$ and $\mu \neq 0$. Let us first prove that $\|\lambda \otimes \mu\| \leq \|\lambda\| \cdot \|\mu\|$. We may suppose $\lambda$ and $\mu$ to be bounded. For every $f \in \mathcal{K}_+(X \times Y)$,

$$
\langle f, \lambda \otimes \mu \rangle = \int d\lambda(x) \int f(x, y) d\mu(y)
$$

and

$$
\int f(x, y) d\mu(y) \leq \|f\| \cdot \|\mu\|
$$

for every $x \in X$, therefore

$$
\langle f, \lambda \otimes \mu \rangle \leq \|f\| \cdot \|\lambda\| \cdot \|\mu\|,
$$

which proves our assertion. On the other hand, let

$$
\alpha < \| \lambda \| , \quad \beta < \| \mu \|
$$

be two real numbers $\geqslant 0$. There exist $g \in \mathcal{K}_+(X) , \ h \in \mathcal{K}_+(Y)$ such that

$$
\| g \| \leqslant 1 , \ \| h \| \leqslant 1 , \quad \lambda(g) \geqslant \alpha , \ \mu(h) \geqslant \beta .
$$

Then $g \otimes h \in \mathcal{K}_+(X \times Y) , \ \| g \otimes h \| \leqslant 1$ and $\langle g \otimes h , \lambda \otimes \mu \rangle \geqslant \alpha \beta ;$ therefore $\| \lambda \otimes \mu \| \geqslant \alpha \beta$ and finally $\| \lambda \otimes \mu \| \geqslant \| \lambda \| \cdot \| \mu \|$, which completes the proof.

### 3. Continuity of product measures

#### Proposition 5 {#int-iii-s4-prop-5 .statement}

*For every measure* $\lambda_0 \in \mathcal{M}(X; \mathbf{C})$, *the mapping* $\mu \mapsto \lambda_0 \otimes \mu$ *of* $\mathcal{M}(Y; \mathbf{C})$ *into* $\mathcal{M}(X \times Y; \mathbf{C})$ *is vaguely continuous*.

For every function $f \in \mathcal{K}(X \times Y; \mathbf{C})$, we know that the function $h(y) = \int f(x, y) d\lambda_0(x)$ belongs to $\mathcal{K}(Y; \mathbf{C})$ (No. 1, Lemma 2), and $\langle f , \lambda_0 \otimes \mu \rangle = \langle h , \mu \rangle$, whence the proposition.

#### Proposition 6 {#int-iii-s4-prop-6 .statement}

*When* $\mathcal{M}(X; \mathbf{C}) , \ \mathcal{M}(Y; \mathbf{C})$ *and* $\mathcal{M}(X \times Y; \mathbf{C})$ *are equipped with the topology of strictly compact convergence* (§ 1, No. 10), *the bilinear mapping* $(\lambda, \mu) \mapsto \lambda \otimes \mu$ *of* $\mathcal{M}(X; \mathbf{C}) \times \mathcal{M}(Y; \mathbf{C})$ *into* $\mathcal{M}(X \times Y; \mathbf{C})$ *is hypocontinuous for the set of vaguely bounded subsets of* $\mathcal{M}(X; \mathbf{C})$ *and* $\mathcal{M}(Y; \mathbf{C})$ *(TVS, III, § 5, No. 3)*.

Let $K \subset X , \ L \subset Y$ be two compact sets, $A$ a compact subset of $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$, and $B$ a vaguely bounded and closed subset of $\mathcal{M}(X; \mathbf{C})$; it is known that $B$ is vaguely compact (§ 1, No. 9, Prop. 15), hence also compact for the topology of strictly compact convergence (§ 1, No. 10, Prop. 17). On the other hand, the Banach space $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ is isometric to $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$ (No. 1, Lemma 1); the mapping $\varphi$ of $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C})) \times \mathcal{M}(X; \mathbf{C})$ into $\mathcal{K}(Y, L; \mathbf{C})$, such that $\varphi(g, \lambda)$ is the function $h$ defined by $h(y) = \int g(x, y) d\lambda(x)$, is *separately continuous* by virtue of § 3, No. 4, Props. 8 and 9. Since $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$ is barreled, it follows that the mapping $\varphi$ is *hypocontinuous* relative to the vaguely bounded subsets of $\mathcal{M}(X; \mathbf{C})$ (TVS, III, § 5, No. 3, Prop. 6); the restriction of this mapping to $A \times B$ is therefore *continuous* (*loc. cit.*, Prop. 4). The image $C$ of $A \times B$ under this mapping is consequently a compact subset of the Banach space $\mathcal{K}(Y, L; \mathbf{C})$. Now, $C$ is none other than the set of functions $h(y) = \int f(x, y) d\lambda(x)$ as $f$ runs over $A$ and $\lambda$ runs over $B$; by virtue of formula (3) of No. 1, the conditions $\lambda \in B$ and $\mu \in C^\circ$ therefore imply $\lambda \otimes \mu \in A^\circ$. In view of the definition of the topology of strictly compact convergence, this proves the proposition (TVS, III, § 5, No. 3, Def. 2).

The conclusion of Prop. 6 is no longer valid when the topology of strictly compact convergence is replaced by the vague topology (Exer. 2 c)). However, if B (resp. C) is a vaguely bounded subset of $\mathcal{M}(X; \mathbf{C})$ (resp. $\mathcal{M}(Y; \mathbf{C})$), then the image of $B \times C$ under the mapping $(\lambda, \mu) \mapsto \lambda \otimes \mu$ is vaguely bounded in $\mathcal{M}(X \times Y; \mathbf{C})$ and therefore the restriction of this mapping to $B \times C$ is vaguely continuous, by virtue of Prop. 6, of §1, No. 10, Prop. 17, and of Prop. 4 of TVS, III, §5, No. 3 (cf. Exer. 3).

### 4. Product of a finite number of measures

Let $X_i$ ($1 \leq i \leq n$) be $n$ locally compact spaces, $X = \prod_{i=1}^n X_i$ their product. The set of linear combinations of complex functions of the form
$$
(x_1, x_2, \ldots, x_n) \mapsto f_1(x_1)f_2(x_2)\cdots f_n(x_n),
$$
where $f_i \in \mathcal{K}(X_i; \mathbf{C})$ ($1 \leq i \leq n$), may be identified canonically with the tensor product $\bigotimes_{i=1}^n \mathcal{K}(X_i; \mathbf{C})$, and it follows from Lemma 1 of No. 1, by induction on $n$, that this tensor product is *dense* in $\mathcal{K}(X; \mathbf{C})$.

Now let $\mu_i$ be a measure on $X_i$ ($1 \leq i \leq n$); there exists on $X$ one and only one measure $\nu$ such that, for $f_i \in \mathcal{K}(X_i; \mathbf{C})$ ($1 \leq i \leq n$),
$$
\langle f_1 \otimes f_2 \otimes \cdots \otimes f_n, \nu \rangle = \prod_{i=1}^n \langle f_i, \mu_i \rangle.
$$
For, if this measure exists, it is unique by the foregoing. On the other hand, let $\nu = \mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n$ be the measure on $X$ defined by the recursion relation
$$
\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n = (\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_{n-1}) \otimes \mu_n.
$$
It follows from No. 1, formula (1) and this definition (by induction on $n$) that $\nu$ verifies (11); it is said to be the *product measure* of the measures $\mu_i$ ($1 \leq i \leq n$) and it is denoted again by $\bigotimes_{i=1}^n \mu_i$. The relation (11) may also be written
$$
\langle f_1 \otimes f_2 \otimes \cdots \otimes f_n, \mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n \rangle = \prod_{i=1}^n \langle f_i, \mu_i \rangle.
$$

#### Proposition 7 ('associativity of the product of measures') {#int-iii-s4-prop-7 .statement}

—
*Let* $(I_k)_{1 \leq k \leq r}$ *be a partition of the interval* $[1, n]$ *of* $\mathbf{N}$; *then*
$$
\bigotimes_{k=1}^r \left( \bigotimes_{i \in I_k} \mu_i \right) = \bigotimes_{i=1}^n \mu_i
$$

For, these two measures coincide, by (12), for every function in $\bigotimes_{i=1}^n \mathcal{K}(X_i; \mathbf{C})$.

The integral of a function $f \in \mathcal{K}(X; \mathbf{C})$ with respect to the product measure is denoted
$$
\int f d\mu_1 d\mu_2 \ldots d\mu_n,
$$
or
$$
\iiint \ldots \int f d\mu_1 d\mu_2 \ldots d\mu_n
$$
or
$$
\int f(\mu_1 \otimes \cdots \otimes \mu_n)
$$
or also
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) d\mu_1(x_1) d\mu_2(x_2) \ldots d\mu_n(x_n)
$$
or
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) \mu_1(x_1) \mu_2(x_2) \ldots \mu_n(x_n)
$$
with $n$ signs $\int$; it is said to be a *multiple integral of order* $n$, or an *$n$-tuple integral*. By virtue of the associativity of the product of measures and the theorem on inverting the order of integration (No. 1, Th. 2), we have, for every permutation $\sigma$ of $[1, n]$,
$$
\iiint \ldots \int f d\mu_1 d\mu_2 \ldots d\mu_n = \int d\mu_{\sigma(1)} \int d\mu_{\sigma(2)} \ldots \int fd\mu_{\sigma(n)}.
$$
(14)

The integral notation and formula (14) may be extended in an obvious way to functions $f \in \mathcal{K}(X; E)$ with values in a Hausdorff locally convex space $E$, such that $f(X)$ is contained in a complete convex subset of $E$. We leave to the reader the task of generalizing to the product of any finite number of measures the results of Nos. 2 and 3 concerning the product of two measures.

In particular, one calls *Lebesgue measure* on $\mathbf{R}^n$ the product of $n$ measures identical to the Lebesgue measure on $\mathbf{R}$; the integral of a function $f \in \mathcal{K}(\mathbf{R}^n; E)$, satisfying the preceding condition, is denoted
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) dx_1 dx_2 \ldots dx_n
$$
and is equal to
$$
\int_{-\infty}^{+\infty} dx_1 \int_{-\infty}^{+\infty} dx_2 \ldots \int_{-\infty}^{+\infty} f(x_1, x_2, \ldots, x_n) dx_n.
$$
Lebesgue measure on $\mathbf{R}^n$ is *invariant under every translation*.

### 5. Inverse limits of measures

Let $X, Y$ be two compact spaces, $p : X \to Y$ a continuous mapping; then $f \mapsto f \circ p$ is a continuous linear mapping of $\mathcal{C}(Y; \mathbf{C})$ into $\mathcal{C}(X; \mathbf{C})$, since $\|f \circ p\| \leq \|f\|$ for every function $f \in \mathcal{C}(Y; \mathbf{C})$; we denote this mapping by $p'$. Its transpose ${}^t p' : \mathcal{M}(X; \mathbf{C}) \to \mathcal{M}(Y; \mathbf{C})$ is therefore such that, for every measure $\mu$ on $X$, ${}^t p'(\mu)$ is the measure on $Y$ such that

$$
\langle {}^t p'(\mu), f \rangle = \langle \mu, f \circ p \rangle
$$

for every function $f \in \mathcal{C}(Y; \mathbf{C})$. Note that for every $x \in X$, ${}^t p'(\varepsilon_x) = \varepsilon_{p(x)}$; for this reason, we shall denote by $p_*(\mu)$ the measure ${}^t p'(\mu)$, which thus extends $p$ when $X$ (resp. $Y$) is canonically embedded in $\mathcal{M}(X; \mathbf{C})$ (resp. $\mathcal{M}(Y; \mathbf{C})$) (§ 1, No. 9, Prop. 13); for every measure $\mu$ on $X$, $p_*(\mu)$ is a special case of the general concept of *image of a measure*, which we shall study in Ch. V, §6. Since, as we saw above, $\|p'\| \leq 1$, we have also $\|{}^t p'\| \leq 1$ and so

$$
\|p_*(\mu)\| \leq \|\mu\|
$$

for every measure $\mu \in \mathcal{M}(X; \mathbf{C})$.

Let us now consider a directed pre-ordered set $I$, and an *inverse system* (or 'projective system') $(X_\alpha, p_{\alpha\beta})$ of *compact* spaces $X_\alpha$ (GT, I, §4, No. 4) having $I$ as set of indices; the *inverse limit* space $X = \lim_{\leftarrow} X_\alpha$ is known to be compact (GT, I, §9, No. 6, Prop. 8); we shall denote by $p_\alpha$ the canonical mapping of $X$ into $X_\alpha$.

It is clear that $(\mathcal{M}(X_\alpha; \mathbf{C}), (p_{\alpha\beta})_* )$ is an *inverse system* of vector spaces, and that $((p_\alpha)_*)$ is an *inverse system* of linear mappings, which justifies the following definition:

#### Definition 2 {#int-iii-s4-def-2 .statement}

*A family* $(\mu_\alpha)_{\alpha \in I}$, *where, for every* $\alpha \in I$, $\mu_\alpha$ *is a measure on* $X_\alpha$, *is said to be an inverse system of measures if, whenever* $\alpha \leq \beta$, $\mu_\alpha = (p_{\alpha\beta})_*(\mu_\beta)$. *A measure* $\mu$ *on* $X = \lim_{\leftarrow} X_\alpha$ *is said to be an inverse limit of the inverse system* $(\mu_\alpha)$ *if* $\mu_\alpha = (p_\alpha)_*(\mu)$ *for every* $\alpha \in I$.

#### Proposition 8 {#int-iii-s4-prop-8 .statement}

(i) *If an inverse system* $(\mu_\alpha)$ *of measures on the* $X_\alpha$ *has an inverse limit, then that limit is unique.*
(ii) *If an inverse system* $(\mu_\alpha)$ *has an inverse limit, then the family of norms* $(\|\mu_\alpha\|)$ *is bounded.*
(iii) *If the* $p_{\alpha\beta}$ *are surjective and the family* $(\|\mu_\alpha\|)$ *is bounded, then the inverse system of measures* $(\mu_\alpha)$ *has an inverse limit.*

(iv) *If the $p_{\alpha \beta}$ are surjective, then every inverse system $(\mu_\alpha)$ of positive measures has an inverse limit $\mu$, which is a positive measure on $X$, and $\| \mu \| = \| \mu_\alpha \|$ for all $\alpha$.

(i) We first prove the following lemma:

#### Lemma 3 {#int-iii-s4-lem-3 .statement}

— *Let F be the set of functions $f \in \mathcal{C}(X; \mathbf{C})$ having the following property: there exist an $\alpha \in I$ and a function $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$ such that $f = f_\alpha \circ p_\alpha$. Then F is a dense linear subspace of $\mathcal{C}(X; \mathbf{C})$.*

We note first of all that if $g = g_\beta \circ p_\beta$ and $h = h_\gamma \circ p_\gamma$, where $g_\beta \in \mathcal{C}(X_\beta; \mathbf{C})$ and $h_\gamma \in \mathcal{C}(X_\gamma; \mathbf{C})$, then there exists an $\alpha \in I$ such that $\alpha \geq \beta$ and $\alpha \geq \gamma$, and therefore $p_\beta = p_{\beta \alpha} \circ p_\alpha$, $p_\gamma = p_{\gamma \alpha} \circ p_\alpha$, which shows that
$$
g + h = (g_\beta \circ p_{\beta \alpha} + h_\gamma \circ p_{\gamma \alpha}) \circ p_\alpha
$$
belongs to F; one sees similarly that $gh \in F$; F is thus a *C*-subalgebra of $\mathcal{C}(X; \mathbf{C})$, which contains the constants and is such that the relation $f \in F$ implies $\overline{f} \in F$. Finally, if $x \neq y$ are two points of X, there exists an $\alpha \in I$ such that $p_\alpha(x) \neq p_\alpha(y)$, therefore there is a function $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$ such that $f_\alpha(p_\alpha(x)) \neq f_\alpha(p_\alpha(y))$. The conclusion therefore follows from the Stone–Weierstrass theorem (GT, X, §4, No. 4, Prop. 7).

The lemma having been established, let $\mu, \mu'$ be two measures on X such that $(p_\alpha)_*(\mu) = (p_\alpha)_*(\mu')$ for all $\alpha \in I$; this means that, for every $\alpha \in I$ and every function $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$, we have
$$
\langle f_\alpha, (p_\alpha)_*(\mu) \rangle = \langle f_\alpha, (p_\alpha)_*(\mu') \rangle,
$$
that is, $\langle f_\alpha \circ p_\alpha, \mu \rangle = \langle f_\alpha \circ p_\alpha, \mu' \rangle$; in other words, $\mu$ and $\mu'$ coincide on the subspace F of $\mathcal{C}(X; \mathbf{C})$, which is dense by Lemma 3, therefore $\mu = \mu'$, which proves (i).

(ii) The relation (15) applied to $p_\alpha$ shows that if $\mu$ is the inverse limit of the inverse system $(\mu_\alpha)$, necessarily
$$
\| \mu \| \geq \| \mu_\alpha \|
$$
for all $\alpha \in I$.

(iii) Suppose the $p_{\alpha \beta}$ are surjective; one knows that the same is then true of the $p_\alpha$ (GT, I, §9, No. 6, Prop. 8). Consider an inverse system of measures $(\mu_\alpha)$ and let us first show that there exists a linear form $\lambda$ *on* F (in the notations of Lemma 3) such that, for every $\alpha \in I$ and every $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$, $\lambda(f_\alpha \circ p_\alpha) = \mu_\alpha(f_\alpha)$. To that end, let $\beta, \gamma$ be two indices in I, and $f_\beta \in \mathcal{C}(X_\beta; \mathbf{C})$, $f_\gamma \in \mathcal{C}(X_\gamma; \mathbf{C})$ two functions such that $f_\beta \circ p_\beta = f_\gamma \circ p_\gamma$; then there exists an index $\alpha \in I$ such that $\alpha \geq \beta$ and $\alpha \geq \gamma$, therefore
$$
p_\beta = p_{\beta \alpha} \circ p_\alpha ,\ p_\gamma = p_{\gamma \alpha} \circ p_\alpha \quad \text{and} \quad (f_\beta \circ p_{\beta \alpha}) \circ p_\alpha = (f_\gamma \circ p_{\gamma \alpha}) \circ p_\alpha ;
$$

since $p_\alpha$ is surjective, this implies $f_\beta \circ p_{\beta \alpha} = f_\gamma \circ p_{\gamma \alpha}$, therefore

$$
\mu_\alpha(f_\beta \circ p_{\beta \alpha}) = \mu_\alpha(f_\gamma \circ p_{\gamma \alpha});
$$

but by definition the last relation may also be written $\mu_\beta(f_\beta) = \mu_\gamma(f_\gamma)$, whence our assertion.

This being so, suppose that there exists a finite number $a > 0$ such that $\| \mu_\alpha \| \leq a$ for all $\alpha \in I$; then, for every function $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$,

$$
|\lambda(f_\alpha \circ p_\alpha)| = |\mu_\alpha(f_\alpha)| \leq a \| f_\alpha \| = a \| f_\alpha \circ p_\alpha \|
$$

since $p_\alpha$ is surjective. This shows that the linear form $\lambda$ is continuous on $F$, and it follows from Lemma 3 that $\lambda$ may be extended to a measure $\mu$ on $X$ such that $(p_\alpha)_*(\mu) = \mu_\alpha$ for all $\alpha \in I$, which proves (iii).

(iv) To prove the existence of $\mu$ it suffices, by (iii), to verify that the family of norms $(\| \mu_\alpha \|)$ is bounded. But $\| \mu_\alpha \| = \mu_\alpha(1)$ and, when $\alpha \leq \beta$, the relation $\mu_\alpha = (p_{\alpha \beta})_*(\mu_\beta)$ implies that $\mu_\alpha(1) = \mu_\beta(1)$; since $I$ is directed, the total masses of all the measures $\mu_\alpha$ are therefore equal, whence our assertion. Moreover, the subspace $F$ obviously satisfies the property (P) of §1, No. 7, Prop. 9, therefore the inverse limit measure $\mu$ of $(\mu_\alpha)$ is positive. Finally, the relation $\mu_\alpha = (p_\alpha)_*(\mu)$ shows as above that $\mu(1) = \mu_\alpha(1)$.

#### Example {#int-iii-s4-n5-exa-1 .statement}

— Let $(X_\lambda)_{\lambda \in L}$ be a family of compact spaces; set $X = \prod_{\lambda \in L} X_\lambda$ and, for every finite subset $J$ of $L$, set $X_J = \prod_{\lambda \in J} X_\lambda$; denote by $\mathrm{pr}_J : X \to X_J$ and $\mathrm{pr}_{J, K} : X_K \to X_J$ (for $J \subset K$) the canonical projections. We know that $(X_J, \mathrm{pr}_{JK})$ is an inverse system of compact spaces, and that the inverse limit of the system of continuous mappings $(\mathrm{pr}_J)$ is a *homomorphism* of $X$ onto the inverse limit space $\lim_{\leftarrow} X_J$, permitting one to identify these two spaces (GT, I, §4, No. 4 and S, III, §7, No. 2, *Remark* 3). Since the projections $\mathrm{pr}_{J, K}$ are surjective, it follows from Prop. 8 that the set $\mathcal{M}(X; \mathbf{C})$ (resp. $\mathcal{M}_+(X)$) may be identified with the set of inverse systems $(\mu_J)$ such that the family of norms $(\| \mu_J \|)$ is bounded (resp. such that the $\mu_J$ are all positive, and necessarily of the same total mass).

Let us consider in particular the case where, for each $\lambda \in L$, a measure $\mu_\lambda$ is given on $X_\lambda$ and one sets $\mu_J = \bigotimes_{\lambda \in J} \mu_\lambda$. If $J \subset K$ are two finite subsets of $I$ then, for every function $f_J \in \mathcal{C}(X_J; \mathbf{C})$ we have, by virtue of formula (14) of No. 4,

$$
\mu_K(f_J \circ \mathrm{pr}_{J, K}) = \mu_J(f_J) \cdot \prod_{\lambda \in K - J} \mu_\lambda(1).
$$

For $(\mu_J)$ to be an inverse system of measures, it is therefore necessary and sufficient that either $\mu_\lambda = 0$ for all $\lambda \in L$ or $\mu_\lambda(1) = 1$ for all $\lambda \in L$.

### 6. Infinite products of measures

Let $(X_\lambda)_{\lambda \in L}$ be a family of compact spaces, and for every $\lambda \in L$ let $\mu_\lambda$ be a measure on $X_\lambda$. We retain the notations of the Example of No. 5, so that in particular $\mu_J = \bigotimes_{\lambda \in J} \mu_\lambda$ for every finite subset $J$ of $L$.

#### Proposition 9 {#int-iii-s4-prop-9 .statement}

*Suppose that all of the measures $\mu_\lambda$ are positive and that the family $(\mu_\lambda(1))_{\lambda \in L}$ is multipliable in $\mathbf{R}_+$ (with product possibly 0). Then there exists one and only one measure $\mu$ on $X$ such that, for every finite subset $J$ of $L$ and every function $f_J \in \mathcal{C}(X_J; \mathbf{C})$,*

$$
\mu(f_J \circ \mathrm{pr}_J) = \mu_J(f_J) \prod_{\lambda \in L - J} \mu_\lambda(1).
$$

Moreover, the measure $\mu$ is positive and its total mass is given by

$$
\mu(1) = \prod_{\lambda \in L} \mu_\lambda(1).
$$

Let $F$ be the vector space consisting of the functions on $X$ of the form $f_J \circ \mathrm{pr}_J$, where $J$ runs over the directed set of finite subsets of $L$, and $f_J \in \mathcal{C}(X_J; \mathbf{C})$; we again say that $F$ is the space of continuous functions on $X$ that *depend only on a finite number of variables*. Lemma 3 of No. 5 shows that $F$ is dense in $\mathcal{C}(X; \mathbf{C})$, which proves the uniqueness assertion. If $\mu_{\lambda_0} = 0$ for some $\lambda_0 \in L$ then the measure $\mu = 0$ meets the requirements, since in the second member of (18) we have $\mu_J(f_J) = 0$ if $\lambda_0 \in J$ and $\prod_{\lambda \in L - J} \mu_\lambda(1) = 0$ if $\lambda_0 \notin J$. We can therefore suppose that $\mu_\lambda \neq 0$ for all $\lambda \in J$ and, since the measures $\mu_\lambda$ are positive, this implies that $\mu_\lambda(1) \neq 0$ for all $\lambda \in L$. Let us then set $\mu'_\lambda = \mu_\lambda / \mu_\lambda(1)$ for every $\lambda \in L$, so that $\mu'_\lambda$ is a positive measure on $X_\lambda$ such that $\mu'_\lambda(1) = 1$. It then follows from Prop. 8 of No. 5 that there exists a positive measure $\mu'$ on $X$ of total mass 1, such that $\mu'(f_J \circ \mathrm{pr}_J) = \mu'_J(f_J)$ for every finite subset $J$ of $L$ and every function $f_J \in \mathcal{C}(X_J; \mathbf{C})$. The positive measure

$$
\mu = \left( \prod_{\lambda \in L} \mu_\lambda(1) \right) \mu'
$$

then meets the requirements, since

$$
\mu_J(f_J) = \mu'_J(f_J) \cdot \prod_{\lambda \in J} \mu_\lambda(1),
$$
$$
\prod_{\lambda \in L} \mu_\lambda(1) = \prod_{\lambda \in J} \mu_\lambda(1) \cdot \prod_{\lambda \in L - J} \mu_\lambda(1).
$$

The measure $\mu$ defined in Prop. 9 is called the *product measure* of the family of positive measures $(\mu_\lambda)_{\lambda \in L}$ and is denoted by $\bigotimes_{\lambda \in L} \mu_\lambda$.

#### Corollary {#int-iii-s4-n6-cor-1 .statement}

*Assume that the conditions of Prop. 9 are verified, and let $(L_\rho)_{\rho \in R}$ be a partition of $L$. Then each of the families of measures $(\mu_\lambda)_{\lambda \in L_\rho}$ admits a product measure, the family of product measures $\left( \bigotimes_{\lambda \in L_\rho} \mu_\lambda \right)_{\rho \in R}$ admits a product measure, and*

$$
\bigotimes_{\rho \in R} \left( \bigotimes_{\lambda \in L_\rho} \mu_\lambda \right) = \bigotimes_{\lambda \in L} \mu_\lambda.
$$

This follows at once from the formulas (18) and (19) and the associativity of the product for multipliable families in $\mathbf{R}_+$ (GT, IV, §7, No. 5, *Remark*).

Exercises

### Exercises {#int-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
