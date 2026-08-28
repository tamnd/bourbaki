---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 4
section_title: Convolution of measures and functions
lang: en
source: int-vii-ix
book_pages: INT VIII.24-INT VIII.45, INT VIII.65-INT VIII.73
pdf_pages: 0124-0145, 0165-0173
extraction: ocr
subsections:
    - "no": 1
      title: Convolution of a measure and a function
      page: 24
      pdf_page: 124
    - "no": 2
      title: Examples of convolvable measures and functions
      page: 28
      pdf_page: 128
    - "no": 3
      title: Convolution and transposition
      page: 34
      pdf_page: 134
    - "no": 4
      title: Convolution of a measure and a function on a group
      page: 37
      pdf_page: 137
    - "no": 5
      title: Convolution of functions on a group
      page: 38
      pdf_page: 138
    - "no": 6
      title: Applications
      page: 42
      pdf_page: 142
    - "no": 7
      title: Regularization
      page: 44
      pdf_page: 144
statements: 38
exercises: 28
content_sha256: 49dae28e635f264996aa83405996b598158ace98510497220a4478b7bfbd1885
---

## § 4. CONVOLUTION OF MEASURES AND FUNCTIONS

### 1. Convolution of a measure and a function

Let X be a locally compact space on which a locally compact group G operates on the left continuously. Let $\beta$ be a positive measure on X, quasi-invariant under G. Let $\chi$ be a function $> 0$ on $G \times X$, measurable for every measure on $G \times X$, and such that, for every $s \in G$, $\chi(s^{-1}, \cdot)$ is a density of $\gamma(s)\beta$ with respect to $\beta$:

$$
(1) \qquad \gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta,
$$

which, with the conventions of Ch. VII, §1, No. 1, may be written:

$$
(1') \qquad d\beta(sx) = \chi(s, x) \, d\beta(x).
$$

These data will remain fixed in Nos. 1, 2, 3 (an exception being made in Remark 2 of No. 2).

Recall (§2, No. 5) that if $\chi$ is continuous and $\beta$ has support $X$, then $\chi$ is a multiplier.

Let $f$ be a locally $\beta$-integrable complex function on $X$, and let $\mu$ be a measure on $G$. For every $s \in G$, the measure $\gamma(s)(f \cdot \beta)$ has base $\beta$ since $\beta$ is quasi-invariant. Therefore, if $\mu$ and $f \cdot \beta$ are convolvable, then $\mu * (f \cdot \beta)$ has base $\beta$ (§3, No. 2, Prop. 10).

#### Definition 1 {#int-viii-s4-def-1 .statement}

*If $\mu$ and $f \cdot \beta$ are convolvable, $\mu$ and $f$ are said to be convolvable relative to $\beta$. Every density of $\mu * (f \cdot \beta)$ with respect to $\beta$ is called a convolution product of $\mu$ and $f$ relative to $\beta$ and is denoted $\mu *_{\beta} f$.*

One omits $\beta$ when no confusion is possible. Convolution for several measures on $G$ and a function on $X$ is defined in an analogous manner.

The various convolution products of $\mu$ and $f$ are equal locally $\beta$-almost everywhere. If $\beta$ has support $X$ and if there exists a convolution product of $\mu$ and $f$ that is continuous, then the latter is uniquely determined; it is then called *the* convolution product of $\mu$ and $f$ relative to $\beta$.

Let $s \in G$ and let $f$ be a locally $\beta$-integrable complex function on $X$. Then $\varepsilon_s$ and $f$ are convolvable, and

$$
\varepsilon_s * (f \cdot \beta) = \gamma(s)(f \cdot \beta) = (\gamma(s)f) \cdot (\gamma(s)\beta) = (\gamma(s)f) \cdot \chi(s^{-1}, \cdot) \cdot \beta,
$$

therefore

$$
(2) \qquad (\varepsilon_s * f)(x) = \chi(s^{-1}, x) f(s^{-1}x) = (\gamma_{\chi}(s)f)(x)
$$

locally $\beta$-almost everywhere.

#### Lemma 1 {#int-viii-s4-lem-1 .statement}

*Let $\mu$ be a measure on $G$. Then $\chi$ is locally $(\mu \otimes \beta)$-integrable, and the image of $\mu \otimes \beta$ under the homeomorphism $(s, x) \mapsto (s, s^{-1}x)$ of $G \times X$ onto $G \times X$ is $\chi \cdot (\mu \otimes \beta)$.*

We may suppose that $\mu \geqslant 0$. Let $F \in \mathcal{K}_+(\mathbf{G} \times \mathbf{X})$. Then
$$
\iint F(s, s^{-1}x) d\mu(s) d\beta(x) = \int d\mu(s) \int F(s, s^{-1}x) d\beta(x)
$$
$$
= \int d\mu(s) \int F(s, x) d(\gamma(s^{-1})\beta)(x) = \int d\mu(s) \int F(s, x)\chi(s, x) d\beta(x).
$$

Now, the function $(s, x) \mapsto F(s, x)\chi(s, x)$ has compact support and is $(\mu \otimes \beta)$-measurable. By Ch. V, §8, No. 3, Prop. 7, the preceding equality proves that this function is $(\mu \otimes \beta)$-integrable and that
$$
\iint F(s, s^{-1}x) d\mu(s) d\beta(x) = \iint F(s, x)\chi(s, x) d\mu(s) d\beta(x).
$$
This proves at the same time both assertions of Lemma 1.

#### Proposition 1 {#int-viii-s4-prop-1 .statement}

*Let $\mu$ be a measure on $\mathbf{G}$, $f$ a locally $\beta$-integrable complex function on $\mathbf{X}$. Suppose that the function $s \mapsto f(s^{-1}x)\chi(s^{-1}, x)$ is essentially $\mu$-integrable except for a locally $\beta$-negligible set of values of $x$, and that the function $x \mapsto \int |f(s^{-1}x)|\chi(s^{-1}, x) d|\mu|(s)$, defined locally almost everywhere for $\beta$, is locally $\beta$-integrable. Then $\mu$ and $f$ are convolvable.*

We may assume that $f \geqslant 0$ and $\mu \geqslant 0$. Let $h \in \mathcal{K}_+(\mathbf{X})$. We are to prove that the function $(s, x) \mapsto h(sx)$ is essentially integrable for $\mu \otimes (f \cdot \beta) = (1 \otimes f) \cdot (\mu \otimes \beta)$ (Ch. V, §8, No. 5, Prop. 10), that is, that $\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x) < +\infty$ (Ch. V, §5, No. 3, Prop. 3); it will clearly suffice to prove that there exists an $a > 0$ such that for every compact subset $K$ of $\mathbf{G}$,
$$
\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x) \leqslant a.
$$
By Lemma 1,
$$
\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x)
$$
$$
= \iint^* h(x)f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x) d\mu(s) d\beta(x).
$$
Now, the function $(s, x) \mapsto h(x)f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x)$ is $(\mu \otimes \beta)$-measurable (Lemma 1) and has compact support. The preceding expression is therefore equal (Ch. V, §8, No. 3, Prop. 7) to
$$
\int^* h(x) d\beta(x) \int^* f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x) d\mu(s)
$$
$$
\leqslant (\sup h) \int^* d\beta(x) \int^* f(s^{-1}x)\chi(s^{-1}, x) d\mu(s),
$$

where S denotes the support of h. Whence the proposition.

#### Proposition 2 {#int-viii-s4-prop-2 .statement}

— Let $\mu$ be a measure on G, f a locally $\beta$-integrable complex function on X. Assume that one of the following conditions is satisfied:
(i) f and $\chi$ are continuous;
(ii) G operates properly in X and f is zero on the complement of a countable union of compact sets;
(iii) $\mu$ is carried by a countable union of compact sets.
If $\mu$ and f are convolvable, then the function $s \mapsto f(s^{-1}x)\chi(s^{-1}, x)$ is essentially $\mu$-integrable except for a locally $\beta$-negligible set of values of x, and one has, locally almost $\beta$-everywhere,

$$
(\mu *_{\beta} f)(x) = \int_G f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) = \int_G (\gamma_{\chi}(s)f)(x)\, d\mu(s).
$$

Let $h \in \mathcal{H}(X)$. Since $\mu$ and f are convolvable, the function $(s, x) \mapsto h(sx)f(x)$ is essentially $(\mu \otimes \beta)$-integrable. By Lemma 1, the function $(s, x) \mapsto h(x)f(s^{-1}x)\chi(s^{-1}, x)$ is essentially $(\mu \otimes \beta)$-integrable. Under hypothesis (i) or (ii) of the statement, one then deduces that this function is $(\mu \otimes \beta)$-integrable; for, in the first case it is continuous and one applies Prop. 3 of Ch. V, §1, No. 1, and in the second case it is zero outside a countable union of compact sets, and one applies Prop. 7, 2) of No. 2, loc. cit. By the Lebesgue–Fubini theorem,

$$
\iint h(sx)\, d\mu(s)\, d(f \cdot \beta)(x) = \iint h(x)f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)\, d\beta(x)
= \int h(x)\, d\beta(x) \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s),
$$

the function $x \mapsto g(x) = \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)$ being moreover locally $\beta$-integrable. One thus sees that

$$
\langle h, \mu * (f \cdot \beta) \rangle = \langle h, g \cdot \beta \rangle,
$$

whence $g = \mu *_{\beta} f$.

Suppose now that $\mu$ is carried by the union S of a sequence of compact sets. The function

$$
(s, x) \mapsto h(x)f(s^{-1}x)\chi(s^{-1}, x)\varphi_S(s)
$$

is essentially $(\mu \otimes \beta)$-integrable, and zero outside a countable union of compact sets, hence $(\mu \otimes \beta)$-integrable. Since $\mu = \varphi_S \cdot \mu$, the argument concludes as before.

#### Remark {#int-viii-s4-n1-rem-1 .statement}

The hypothesis (iii) of Prop. 2 is satisfied notably when $\mu$ is bounded. For, for every $n > 0$, there then exists a compact subset $K_n$ of $G$ such that
$$
|\mu|(G - K_n) \leq \frac{1}{n}
$$
(Ch. IV, §4, No. 7), and $\mu$ is carried by the union of the $K_n$. More generally, let $\rho$ be a lower semi-continuous finite function $> 0$ on $G$ such that $\rho(st) \leq \rho(s)\rho(t)$; if $\mu \in \mathcal{M}^\rho$, the hypothesis (iii) is satisfied; for, $\rho \cdot \mu$ is bounded, and $\mu$ is carried by the same subsets as $\rho \cdot \mu$ since, on every compact subset of $G$, $\rho$ is bounded below by a constant $> 0$.

### 2. Examples of convolvable measures and functions

In Props. 3 and 4, $\mathcal{C}'(G)$ and $\mathcal{M}(G)$ are equipped with the topology of compact convergence in $\mathcal{C}(G)$ and $\mathcal{K}(G)$, respectively.

#### Proposition 3 {#int-viii-s4-prop-3 .statement}

— Assume $\chi$ continuous. Let $\mu \in \mathcal{C}'(G)$, $f \in \mathcal{C}(X)$. Then:
(i) $\mu$ and $f$ are convolvable relative to $\beta$.
(ii) Formula (3) of No. 1 defines for every $x \in X$ a convolution product $\mu *_{\beta} f$ that is continuous and is none other than the element $\gamma_\chi(\mu)f$ defined by the continuous representation $\gamma_\chi$ of $G$ in $\mathcal{C}(X)$; moreover, the mapping $(\mu, f) \mapsto \mu *_{\beta} f$ is hypocontinuous relative to the equicontinuous subsets of $\mathcal{C}'(G)$ and the compact subsets of $\mathcal{C}(X)$.
(iii) If in addition $f \in \mathcal{K}(X)$, then the product $\mu *_{\beta} f$ of (ii) belongs to $\mathcal{K}(X)$ and the mapping $(\mu, f) \mapsto \mu *_{\beta} f$ is hypocontinuous relative to the equicontinuous subsets of $\mathcal{C}'(G)$ and the compact subsets of $\mathcal{K}(X)$.

We know that $\mu$ and $f$ are convolvable (§3, No. 2, Prop. 8 (i)). On the other hand, with the notations of §2, we have
$$
\gamma_\chi(\mu)f = \int (\gamma_\chi(s)f)d\mu(s) \in \mathcal{C}(X)
$$
since $\mathcal{C}(X)$ is complete. In particular, for every $x \in X$,
$$
(\gamma_\chi(\mu)f)(x) = \int (\gamma_\chi(s)f)(x)\,d\mu(s).
$$
This, combined with Prop. 2 (i), and §2, No. 6, proves (ii). Finally, if $f \in \mathcal{K}(X)$ then $\mu * (f \cdot \beta)$ has compact support (§3, No. 2, Prop. 9), therefore $\mu *_{\beta} f \in \mathcal{K}(X)$. For, let us consider the continuous representation $U$ of $G$ in the completion $\mathcal{K}(X)^{\sim}$ obtained by extending by continuity the continuous operators $\gamma_\chi(s)$ in $\mathcal{K}(X)$ (§ 2, No. 1, *Remark 3*). Let $S$ be the support of $\mu$. The functions $\gamma_\chi(s)f$, for $s \in S$, have their support contained in a fixed compact set $K$. The set $\mathcal{K}(X, K)$ is a complete linear subspace of $\mathcal{K}(X)$. Therefore $U(\mu)f \in \mathcal{K}(X)$. One sees as before that $U(\mu)f = \mu *^\beta f$, and (iii) again follows from § 2, No. 6.

#### Proposition 4 {#int-viii-s4-prop-4 .statement}

*Assume that G operates properly in X and that $\chi$ is continuous. Let $\mu \in \mathcal{M}(G)$ and $f \in \mathcal{K}(X)$.*

(i) $\mu$ and $f$ are convolvable relative to $\beta$.

(ii) *Formula (3) of No. 1 defines for every $x \in X$ a convolution product $\mu *^\beta f$ that is continuous.*

(iii) *The mapping $(\mu, f) \mapsto \mu *^\beta f$ of $\mathcal{M}(G) \times \mathcal{K}(X)$ into $\mathcal{C}(X)$ is hypocontinuous relative to the bounded subsets of $\mathcal{M}(G)$ and the compact subsets of $\mathcal{K}(X)$ that are contained in some subspace $\mathcal{K}(X, L)$ (where $L$ is a variable compact subset of $X$).*

We know that $\mu$ and $f$ are convolvable (§ 3, No. 2, Prop. 8 (ii)), and it is clear that the integrals occurring in (3) exist for every $x \in X$. Let $K$ and $L$ be two compact subsets of $X$. There exists a compact subset $H$ of $G$ such that the relations $x \in K$ and $s^{-1}x \in L$ imply $s \in H$; let $\varphi \in \mathcal{K}_+(G)$ with $\varphi(s) = 1$ for $s \in H$. Then, for $f \in \mathcal{K}(X, L)$ and $x \in K$,

$$
\int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) = \int f(s^{-1}x)\chi(s^{-1}, x)\varphi(s)\, d\mu(s)
= ((\varphi \cdot \mu) *^\beta f)(x).
$$

Consequently $\int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)$ is a continuous function of $x$ and defines a convolution product $\mu *^\beta f \in \mathcal{C}(X)$. Moreover, the mapping $\mu \mapsto \varphi \cdot \mu$ of $\mathcal{M}(G)$ into $\mathcal{C}'(G)$ is continuous for the topologies of compact convergence. Prop. 3 (iii) therefore implies that the mapping $(\mu, f) \mapsto \mu *^\beta f$ of $\mathcal{M}(G) \times \mathcal{K}(X, L)$ into $\mathcal{C}(X)$ is, for every compact subset $L$ of $X$, hypocontinuous relative to the compact subsets of $\mathcal{K}(X, L)$. In particular, the mapping $(\mu, f) \mapsto \mu *^\beta f$ of $\mathcal{M}(G) \times \mathcal{K}(X)$ into $\mathcal{C}(X)$ is separately continuous. Since $\mathcal{K}(X)$ is barreled, this mapping is hypocontinuous relative to the bounded subsets of $\mathcal{M}(G)$ (TVS, III, § 5, No. 3, Prop. 6).

#### Remark 1 {#int-viii-s4-n2-rem-1 .statement}

— Under the hypotheses of Prop. 4, the mapping $\mu \mapsto \mu *^\beta f$ of $\mathcal{M}_+(G)$ into $\mathcal{C}(X)$ is continuous when $\mathcal{M}_+(G)$ is equipped with the *vague* topology, for every $f \in \mathcal{K}(X)$. For, let $K$ be a compact subset of $X$, $S$ the (compact) support of $f$; since $G$ operates properly in $X$, the set of $s \in G$ for which there exists an $x \in K$ with $s^{-1}x \in S$ is a compact subset $L$ of $G$ (GT, III, § 4, No. 5, Th. 1). Let $\varepsilon$ be a number $> 0$, $\varphi$ a function in $\mathcal{K}_+(G)$ equal to 1 on the compact set $L$, $\mu_0$ an element of $\mathcal{M}_+(G)$; the set $W_0$ of measures $\mu \in \mathcal{M}_+(G)$ such that
$$
\left| \int \varphi(s)\, d\mu(s) - \int \varphi(s)\, d\mu_0(s) \right| \leq \varepsilon
$$
is a neighborhood of $\mu_0$ in $\mathcal{M}_+(G)$. On the other hand, the function $(s, x) \mapsto f(s^{-1}x)\chi(s^{-1}, x)$ is uniformly continuous on $L \times K$, therefore there exists a finite number of points $x_i \in K$ ($1 \leq i \leq n$) such that for every $x \in K$, there is an $i$ for which
$$
|f(s^{-1}x)\chi(s^{-1}, x) - f(s^{-1}x_i)\chi(s^{-1}, x_i)| \leq \varepsilon
$$
for all $s \in L$. Since $\mu(L) \leq \int \varphi(s)\, d\mu_0(s) + \varepsilon$ for all $\mu \in W_0$, also
$$
\begin{align*}
\left| \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) - \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu(s) \right| \\
\leq \varepsilon \left( \int \varphi(s)\, d\mu_0(s) + \varepsilon \right)
\end{align*}
$$
for every $x$ satisfying the preceding inequality and every $\mu \in W_0$. Now let $W$ be the neighborhood of $\mu_0$ in $\mathcal{M}_+(G)$ formed by the measures $\mu \in W_0$ such that
$$
\left| \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu(s) - \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu_0(s) \right| \leq \varepsilon
$$
for $1 \leq i \leq n$. It is clear that for every measure $\mu \in W$ and every $x \in K$,
$$
\begin{align*}
\left| \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) - \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu_0(s) \right| \\
\leq \varepsilon \left( 2 \int \varphi(s)\, d\mu_0(s) + 2\varepsilon + 1 \right),
\end{align*}
$$
and since $\varepsilon$ is arbitrary, this proves our assertion.

#### Proposition 5 {#int-viii-s4-prop-5 .statement}

*Assume $\chi$ a continuous multiplier and each function $\chi(s, \cdot)$ bounded.*
(i) *The function $s \mapsto \rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$ on $G$ is lower semi-continuous $> 0$ and satisfies $\rho(st) \leq \rho(s)\rho(t)$ for all $s, t$ in $G$.*
(ii) *Let $\mu \in \mathcal{M}^\rho(G)$ and $f \in L^\infty(X, \beta)$.*¹ *Then $\mu$ and $f$ are convolvable and $\mu *^\beta f$ is given locally almost everywhere by the formula (3) of No. 1. One has $\mu *^\beta f \in L^\infty(X, \beta)$, and $\| \mu *^\beta f \|_\infty \leq \| \mu \|_\rho \| f \|_\infty$.*

¹For a function $f$, the expression "$f \in L^\infty(X, \beta)$" is an abuse of notation signifying that, depending on the context, the symbol $f$ is to be interpreted either as a function or the equivalence class of a function. In particular, the symbol $\mu *^\beta f$ can stand for either a function defined locally $\beta$-almost everywhere, or the equivalence class of such a function for the relation of equality locally $\beta$-almost everywhere.

(iii) *If, moreover, $f \in \mathcal{C}^\infty(X)$ (resp. $\overline{\mathcal{K}(X)}$), then formula (3) of No. 1 defines for every $x$ a convolution product $\mu *^\beta f$ that belongs to $\mathcal{C}^\infty(X)$ (resp. $\mathcal{K}(X)$).

(iv) *If $f \in \mathcal{K}(X)$, then the convolution product $\mu *^\beta f$ defined by (3) is none other than the element $\gamma_\chi(\mu)f$ defined by the continuous representation $\gamma_\chi$ of $G$ in $\overline{\mathcal{K}(X)}$.

The identity $\chi(st, x) = \chi(s, tx)\chi(t, x)$ implies at once that $\rho(st) \leq \rho(s)\rho(t)$. On the other hand, $\rho$ is lower semi-continuous, being the upper envelope of continuous functions.

Let $\mu \in \mathcal{M}^\rho(G)$. By Prop. 1 of No. 1, $\mu$ and 1 are convolvable; Prop. 2 (i) shows that $(|\mu| *^\beta 1)(x) \leq \int_G \rho(s) d|\mu|(s)$ locally $\beta$-almost everywhere. Therefore, if $f$ is $\beta$-measurable and $|f| \leq 1$, then $\mu$ and $f$ are convolvable and $N_\infty(\mu *^\beta f) \leq \int \rho(s) d|\mu|(s)$. Moreover, $\mu *^\beta f$ is given locally almost everywhere by formula (3) of No. 1, because condition (iii) of Prop. 2 of No. 1 is satisfied. This implies (ii).

Suppose $f$ continuous and bounded by 1 in absolute value. It is clear that the integrals occurring in (3) exist for all $x \in X$. Let us show that they depend continuously on $x$. We can suppose $\mu \geq 0$. Let $x_0 \in X$ and $\varepsilon > 0$. Let $K$ be a compact subset of $G$ such that $\int_{G - K} \rho(s) d\mu(s) \leq \varepsilon$. There exists a neighborhood $V$ of $x_0$ in $X$ such that $x \in V$ implies

$$
|f(s^{-1}x)\chi(s^{-1}, x) - f(s^{-1}x_0)\chi(s^{-1}, x_0)| \leq \varepsilon / \mu(K)
$$

for $s \in K$. Then, for $x \in V$,

$$
\left| \int f(s^{-1}x)\chi(s^{-1}, x) d\mu(s) - \int f(s^{-1}x_0)\chi(s^{-1}, x_0) d\mu(s) \right|
$$
$$
\leq 2 \int_{G - K} \rho(s) d\mu(s) + \int_K \frac{\varepsilon}{\mu(K)} d\mu(s) \leq 3\varepsilon,
$$

whence our assertion. Suppose that in addition $f \in \overline{\mathcal{K}(X)}$. Let $H$ be a compact subset of $X$ such that $|f(y)| \leq \varepsilon$ for $y \notin H$. Let $x \notin KH$. Then $s^{-1}x \notin H$ for $s \in K$, therefore

$$
\left| \int_G f(s^{-1}x)\chi(s^{-1}, x) d\mu(s) \right| \leq \int_{G - K} \rho(s) d\mu(s) + \int_K \varepsilon \rho(s) d\mu(s)
$$
$$
\leq \varepsilon \left( 1 + \int_G \rho(s) d\mu(s) \right),
$$

which completes the proof of (iii).

Finally, if $f \in \mathcal{K}(X)$ then, since $\varepsilon_x \in \mathcal{M}^1(X)$ for all $x \in X$, we have

$$
(\gamma_\chi(\mu)f)(x) = \int (\gamma_\chi(s)f)(x) d\mu(s),
$$

thus $\gamma_\chi(\mu)f$ is the convolution product $\mu *^\beta f$ defined by (3).

#### Proposition 6 {#int-viii-s4-prop-6 .statement}

*Assume $\chi$ a continuous multiplier and each function $\chi(s, \cdot)$ bounded. Let $\rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$. Let $p$ and $q$ be two conjugate exponents ($1 \leq p < +\infty$). Let $\mu \in \mathcal{M}^{\rho^{1/q}}(G)$ and $f \in L^p(X, \beta)^2$ Then:
(i) $\mu$ and $f$ are convolvable;
(ii) the convolution product $\mu *^\beta f$ is given locally $\beta$-almost everywhere by the formula (3), and is equal locally $\beta$-almost everywhere to a function $g \in L^p(X, \beta)$ such that $\|g\|_p \leq \|\mu\|_{\rho^{1/q}} \|f\|_p$;
(iii) $g$ is equal to the element $\gamma_\chi(\mu)f$ defined by the continuous representation $\gamma_\chi$ of $G$ in $L^p(X, \beta)$.

We have
$$
\int^* \|\gamma_\chi(s)f\|_p d|\mu|(s) \leq \left( \int^* \rho(s)^{1/q} d|\mu|(s) \right) \|f\|_p < +\infty
$$
by §2, No. 5, formula (5). On the other hand, the mapping $s \mapsto \gamma_\chi(s)f$ of $G$ into $L^p(X, \beta)$ is continuous (§2, No. 5, Prop. 9). Therefore this mapping is $\mu$-integrable. Let
$$
g = \int_G (\gamma_\chi(s)f) d\mu(s) \in L^p(X, \beta).
$$
We have $\|g\|_p \leq (\int \rho^{1/q}(s) d|\mu|(s)) \|f\|_p$. Applying the preceding remarks to $|f|$, one sees that the mapping $s \mapsto \varepsilon_s * |f|$ of $G$ into $L^p(X, \beta)$ is $\mu$-integrable, therefore that, for every $h \in \mathcal{H}(X)$, the mapping $s \mapsto \langle h, \varepsilon_s * (|f| \cdot \beta) \rangle$ is $\mu$-integrable. Prop. 7 of §1, No. 5 then proves that $\mu$ and $f \cdot \beta$ are convolvable. Moreover,
$$
\int_X g(x)h(x) d\beta(x) = \int_G d\mu(s) \int_X (\gamma_\chi(s)f)(x)h(x) d\beta(x)
= \int_G \langle h, \varepsilon_s * (f \cdot \beta) \rangle d\mu(s),
$$
and this last integral is equal to $\langle h, \mu * (f \cdot \beta) \rangle$ by Prop. 7 of §1, No. 5. One therefore sees that $g$ is a convolution product of $\mu$ and $f$. This convolution product is given locally $\beta$-almost everywhere by (3), by Prop. 2 and the *Remark* that follows it.

2For a function $f$, the expression " $f \in L^p(X, \beta)$ " is an abuse of notation signifying that, depending on the context, the symbol $f$ is to be interpreted either as a function defined $\beta$-almost everywhere, or as the equivalence class of such a function for the relation of equality $\beta$-almost everywhere. Thus $f \in L^p$ can symbolize either $f \in \mathcal{L}^p$ or $\dot{f} \in L^p$.

By an abuse of notation, it is often one of the functions $g$ of the statement that is denoted $\mu *^\beta f$, which permits writing

$$
\| \mu *^\beta f \|_p \leq \| \mu \|_{\rho^{1/q}} \| f \|_p .
$$

If $X$ is countable at infinity, this style of notation is, moreover, entirely justified.

#### Corollary {#int-viii-s4-n2-cor-1 .statement}

*Under the hypotheses of Prop. 6, the mapping* $(\mu, f) \mapsto \mu *^\beta f$ *defines on* $L^p(X, \beta)$ *the structure of a left module over* $\mathcal{M}^{\rho^{1/q}}(G)$ $(1 \leq p \leq +\infty)$.

This follows from Props. 5 and 6 and the associativity of the convolution product.

#### Remark 2 {#int-viii-s4-n2-rem-2 .statement}

— Let $X$ be a locally compact space on which a locally compact group $G$ operates continuously on the right by $(x, s) \mapsto xs$. Let $\beta$ be a positive measure on $X$. Let $\chi$ be a function $> 0$ on $G \times X$, measurable for every measure on $G \times X$, such that $\delta(s)\beta = \chi(s, \cdot) \cdot \beta$ for every $s \in G$. Let $f$ be a locally $\beta$-integrable function on $X$ and let $\mu$ be a measure on $G$. If $f \cdot \beta$ and $\mu$ are convolvable (for the mapping $(x, s) \mapsto xs$ of $X \times G$ into $X$), then $(f \cdot \beta) * \mu$ has base $\beta$. We then say that $f$ and $\mu$ are convolvable relative to $\beta$; every density of $(f \cdot \beta) * \mu$ with respect to $\beta$ is called a convolution product of $f$ and $\mu$ relative to $\beta$, and is denoted $f *^\beta \mu$ or simply $f * \mu$.

Let $G^0$ be the group opposite to $G$. By $(s, x) \mapsto xs$, $G^0$ operates continuously on the left in $X$. To say that $f$ and $\mu$ are convolvable in the foregoing sense is equivalent to saying that $\mu$ and $f$ are convolvable for $G^0$ operating on the left in $X$; and the convolution products $f *^\beta \mu$ are none other than the convolution products $\mu *^\beta f$ for $G^0$ operating on the left in $X$. On the other hand, for $s \in G^0$ one has $\gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta$. The results of Nos. 1 and 2 may then be translated immediately into results concerning the products $f *^\beta \mu$. In particular:

1) If $s \in G$ and $f$ is locally $\beta$-integrable, then $f$ and $\varepsilon_s$ are convolvable and

$$
(f * \varepsilon_s)(x) = \chi(s^{-1}, x)f(xs^{-1}) .
$$

2) If $f$ and $\mu$ are convolvable and if one of the conditions (i), (ii), (iii) of Prop. 2 is fulfilled, then $f *^\beta \mu$ is given locally $\beta$-almost everywhere by

$$
(f *^\beta \mu)(x) = \int_G f(xs^{-1})\chi(s^{-1}, x)\, d\mu(s) .
$$

We leave to the reader the task of translating the other statements. Note that if $\chi$ is continuous and $\beta$ has support $X$, then

$$
\chi(ts, x) = \chi(s, xt)\chi(t, x) \quad (x \in X; \ s, t \text{ in } G) .
$$

### 3. Convolution and transposition

Let us return to the hypotheses and notations of the beginning of No. 1, but let us assume in addition that $\beta$ is *relatively invariant with multiplier* $\chi$; $\chi$ is therefore a continuous function on $G$.

#### Proposition 7 {#int-viii-s4-prop-7 .statement}

*Let $f$ be a locally $\beta$-integrable function on $X$, $\nu$ a measure on $X$, and $\mu$ a measure on $G$. Assume that:
(i) $\mu$ and $f$ are convolvable and formula (3) of No. 1 defines locally $\beta$-almost everywhere a convolution product $\mu *_{\beta} f$.
(ii) $\chi \cdot \check{\mu}$ and $\nu$ are convolvable.
(iii) *The function* $g(s, x) = f(s^{-1}x)\chi(s^{-1})$ *is* $(\mu \otimes \nu)$*-integrable.
*Then* $f$ *is essentially integrable for* $(\chi \cdot \check{\mu}) * \nu$, *the function* $\mu *_{\beta} f$ *defined by (3) is* $\nu$*-integrable, and*

$$
\nu(\mu *_{\beta} f) = ((\chi \cdot \check{\mu}) * \nu)(f).
$$

Since $g(s, x)$ is integrable for $\mu \otimes \nu$, the function $f(sx)$ is essentially integrable for $(\chi \cdot \check{\mu}) \otimes \nu$ and $f$ is essentially integrable for $(\chi \cdot \check{\mu}) * \nu$. By the Lebesgue–Fubini theorem, $\mu *_{\beta} f = \int g(s, x) d\mu(s)$ is $\nu$-integrable and

$$
\begin{align*}
\nu(\mu *_{\beta} f) &= \iint f(s^{-1}x)\chi(s^{-1}) d\mu(s) d\nu(x) \\
&= \iint f(sx)\chi(s) d\check{\mu}(s) d\nu(x) = ((\chi \cdot \check{\mu}) * \nu)(f).
\end{align*}
$$

#### Example {#int-viii-s4-n3-exa-1 .statement}

— 1) One can take $f \in \mathcal{C}(X)$, $\nu \in \mathcal{C}'(X)$ and $\mu \in \mathcal{C}'(G)$ by Prop. 3, and the Cor. of Prop. 5 of §1, No. 4. The formula (7) then means that the endomorphism $\nu \mapsto (\chi \cdot \check{\mu}) * \nu$ of $\mathcal{C}'(X)$ is the *transpose* of the endomorphism $f \mapsto \mu * f$ of $\mathcal{C}(X)$.

2) One can take $f \in \mathcal{K}(X)$, $\nu \in \mathcal{M}(X)$ and $\mu \in \mathcal{C}'(G)$ by Prop. 3, Prop. 8 of §3, No. 2, and the remark that the support of the continuous function $g(s, x)$ intersects the support of $\mu \otimes \nu$ in a compact set. The formula (7) then means that the endomorphism $\nu \mapsto (\chi \cdot \check{\mu}) * \nu$ of $\mathcal{M}(X)$ is the *transpose* of the endomorphism $f \mapsto \mu * f$ of $\mathcal{K}(X)$.

3) If $G$ operates properly on $X$, one can take $f \in \mathcal{K}(X)$, $\nu \in \mathcal{C}'(X)$ and $\mu \in \mathcal{M}(G)$ by Prop. 4, Prop. 8 of §3, No. 2, and the same remark as in *Example 2*.

#### Proposition 8 {#int-viii-s4-prop-8 .statement}

*Let $f$ and $g$ be two locally $\beta$-integrable functions on $X$ and let $\mu \in \mathcal{M}(G)$. Assume that:*

(i) $\mu$ and $f$ are convolvable and the formula (3) of No. 1 defines locally $\beta$-almost everywhere a convolution product $\mu *_{\beta} f$.

(ii) $\chi \cdot \check{\mu}$ and $g$ are convolvable and the formula (3) of No. 1 (with $\mu$ replaced by $\chi \cdot \check{\mu}$ and $f$ by $g$) defines locally $\beta$-almost everywhere a convolution product $(\chi \cdot \check{\mu}) *_{\beta} g$.

(iii) There exists a function $\psi$ on $G$, equal locally $\mu$-almost everywhere to 1, such that the function

$$
h(s, x) = g(x) f(s^{-1} x) \chi(s^{-1}) \psi(s)
$$

is $(\mu \otimes \beta)$-integrable.

Then the functions $g(x)((\mu *_{\beta} f)(x))$ and $f(x)(((\chi \cdot \check{\mu}) *_{\beta} g)(x))$ are essentially $\beta$-integrable, and

$$
(8) \quad \int f(x)(((\chi \cdot \check{\mu}) *_{\beta} g)(x)) d\beta(x) = \int g(x)((\mu *_{\beta} f)(x)) d\beta(x).
$$

For, by (iii) and the Lebesgue–Fubini theorem, the function

$$
x \mapsto g(x) \int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s)
$$

is $\beta$-integrable, and

$$
\begin{align*}
\mathrm{I} &= \iint f(s^{-1} x) g(x) \chi(s^{-1}) \psi(s) d\mu(s) d\beta(x) \\
&= \int g(x) d\beta(x) \int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s).
\end{align*}
$$

But $\psi \cdot \mu = \mu$, consequently

$$
\int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s) = (\mu *_{\beta} f)(x)
$$

locally $\beta$-almost everywhere. This shows that the function

$$
x \mapsto g(x)((\mu *_{\beta} f)(x))
$$

is essentially $\beta$-integrable and that

$$
\mathrm{I} = \int g(x)((\mu *_{\beta} f)(x)) d\beta(x).
$$

On the other hand, Lemma 1 shows that the function

$$(s, x) \mapsto g(sx)f(x)\chi(s^{-1})\psi(s)$$

is integrable for $(\chi \cdot \mu) \otimes \beta$. Therefore the function $(s, x) \mapsto g(s^{-1}x)f(x)\psi(s^{-1})$ is integrable for $\check{\mu} \otimes \check{\beta}$, and

$$
\begin{align*}
\mathrm{I} &= \iint g(s^{-1}x)f(x)\psi(s^{-1})\, d\check{\mu}(s)\, d\beta(x) \\
&= \int f(x)\, d\beta(x) \int g(s^{-1}x)\psi(s^{-1})\, d\check{\mu}(s).
\end{align*}
$$

But $\check{\psi} \cdot \check{\mu} = \check{\mu}$ and so $\int g(s^{-1}x)\psi(s^{-1})\, d\check{\mu}(s) = ((\chi \cdot \check{\mu}) *^\beta g)(x)$ locally $\beta$-almost everywhere. This shows that the function

$$x \mapsto f(x)(((\chi \cdot \check{\mu}) *^\beta g)(x))$$

is essentially $\beta$-integrable and that

$$\mathrm{I} = \int f(x)(((\chi \cdot \check{\mu}) *^\beta g)(x))\, d\beta(x).$$

This proves the proposition.

#### Example {#int-viii-s4-n3-exa-2 .statement}

— 4) One can take $f \in \mathcal{C}(X)$, $g \in \mathcal{K}(X)$ and $\mu \in \mathcal{C}'(G)$ (with $\psi = 1$).

5) If G operates properly on X, one can take $f \in \mathcal{K}(X)$, $g \in \mathcal{K}(X)$ and $\mu \in \mathcal{M}(G)$ (with $\psi = 1$).

6) One can take $f \in \mathbf{L}^p(X, \beta)$, $g \in \mathbf{L}^q(X, \beta)$ and $\mu \in \mathcal{M}^\rho(G)$, where $1 \leq p < +\infty$, $\frac{1}{p} + \frac{1}{q} = 1$, $\rho = \chi^{-1/q}$. The conditions (i) and (ii) are satisfied by Props. 5 and 6. Let us prove (iii). We have seen that $\mu$ is carried by a set S that is a countable union of compact sets. Let us take for $\psi$ the characteristic function of S. The function $h$ is $(\mu \otimes \beta)$-measurable: for, the function $(s, x) \mapsto g(x)\chi(s^{-1})\psi(s)$ is so, as is the function $(s, x) \mapsto f(s^{-1}x)$ by Lemma 1. Moreover, $g$ being zero outside a countable union of $\beta$-integrable sets, $h$ is zero outside a countable union of $(\mu \otimes \beta)$-integrable sets. We then have (Ch. V, §8, No. 3, Prop. 7):

$$
\begin{align*}
\mathrm{J} &= \iint^* |g(x)f(s^{-1}x)|\chi(s^{-1})\psi(s)\, d|\mu|(s)\, d\beta(x) \\
&= \int^* |g(x)|\, d\beta(x) \int^* |f(s^{-1}x)|\chi(s^{-1})\psi(s)\, d|\mu|(s).
\end{align*}
$$

But since $g$ (resp. $\psi$) is zero outside a countable union of integrable sets, the upper integrals of the second member of (9) are equal to the essential upper integrals (Ch. V, §1, No. 2, Prop. 7). Now (Ch. V, §5, No. 3, Prop. 3)

$$
\int^\bullet |f(s^{-1}x)| \chi(s^{-1}) \psi(s) d|\mu|(s) = \int^\bullet |f(s^{-1}x)| \chi(s^{-1}) d|\mu|(s)
$$

since $\mu = \psi \cdot \mu$. By Prop. 6, this last integral is finite and is equal to $(|\mu| *^\beta |f|)(x)$ locally $\beta$-almost everywhere. Therefore

$$
J = \int^\bullet |g(x)|(|\mu| *^\beta |f|)(x) d\beta(x),
$$

and J is finite since $g \in L^q$ and $|\mu| *^\beta |f| \in L^p$ (Prop. 6). Therefore h is $(\mu \otimes \beta)$-integrable.

The formula (8) then means that the endomorphism $g \mapsto (\chi \cdot \check{\mu}) * g$ of $L^q(X, \beta)$ is, for $\mu \in \mathcal{M}^\rho(G)$, the transpose of the endomorphism $f \mapsto \mu * f$ of $L^p(X, \beta)$.

### 4. Convolution of a measure and a function on a group

Let G be a locally compact group. Throughout Nos. 4 and 5, we fix a relatively invariant positive measure $\beta \neq 0$ on G; let $\chi$ and $\chi'$ be its left and right multipliers (recall that $\chi' = \chi \Delta_G$). If $\mu$ is a measure on G and $f$ is a locally $\beta$-integrable function on G, the convolvability of $\mu$ and $f$ and the products $\mu * f$ (resp. the convolvability of $f$ and $\mu$ and the products $f * \mu$) may be defined by regarding G as operating on itself on the left (resp. on the right) by translations. Let us make explicit in this situation some of the preceding results:

1) Let $\mu$ be a measure on G, $f$ a locally $\beta$-integrable complex function on G. Assume verified one of the following conditions:
   (i) $f$ is continuous;
   (ii) $f$ is zero on the complement of a countable union of compact sets;
   (iii) $\mu$ is carried by a countable union of compact sets.
If $\mu$ and $f$ are convolvable then, locally $\beta$-almost everywhere,

$$
(\mu * f)(x) = \int_G f(s^{-1}x) \chi(s^{-1}) d\mu(s).
$$

If $f$ and $\mu$ are convolvable then, locally $\beta$-almost everywhere,

$$
(f * \mu)(x) = \int_G f(xs^{-1}) \chi'(s^{-1}) d\mu(s).
$$

2) Let $p$ and $q$ be two conjugate exponents ($1 \leq p \leq +\infty$). If $\mu \in \mathcal{M}^{\chi^{-1/q}}(G)$ and $f \in L^p(G, \beta)$, then $\mu$ and $f$ are convolvable, and $\mu * f$ is equal locally $\beta$-almost everywhere to a function in $L^p(G, \beta)$; one has (with an abuse of notations already noted)

$$
\| \mu * f \|_p \leq \| \mu \|_{\chi^{-1/q}} \| f \|_p .
$$

If $\mu \in \mathcal{M}^{{\chi'}^{-1/q}}(G)$ and $f \in L^p(G, \beta)$, then $f$ and $\mu$ are convolvable, and $f * \mu$ is equal locally $\beta$-almost everywhere to a function in $L^p(G, \beta)$; one has $\| f * \mu \|_p \leq \| \mu \|_{{\chi'}^{-1/q}} \| f \|_p$.

3) The mappings $(\mu, f) \mapsto \mu * f , (f, \mu) \mapsto f * \mu$ define on $L^p(G, \beta)$ the structures of a left module over $\mathcal{M}^{\chi^{-1/q}}(G)$ and a right module over $\mathcal{M}^{{\chi'}^{-1/q}}(G)$. The two external laws on $L^p(G, \beta)$ are permutable by the associativity of convolution.

4) If $\mu * f$ is continuous and is given at every point by (10), then

$$
(\mu * f)(e) = \int f(s^{-1}) \chi(s^{-1}) d\mu(s) .
$$

If $f * \mu$ is continuous and is given at every point by (11), then

$$
(f * \mu)(e) = \int f(s^{-1}) \chi'(s^{-1}) d\mu(s) .
$$

### 5. Convolution of functions on a group

We conserve the notations $G, \beta, \chi, \chi'$ of No. 4.

Recall that if $f$ is a complex function on $G$, the property of being locally $\beta$-integrable is independent of the choice of $\beta$. Let $\mathcal{L}(G)$ be the set of functions having this property. If $f \in \mathcal{L}(G) , g \in \mathcal{L}(G)$, the relation

« $f \cdot \beta$ and $g \cdot \beta$ are convolvable »

is independent of the choice of $\beta$ (§ 3, No. 1, Prop. 6). We shall then say that $f$ and $g$ are *convolvable*. By No. 1, $(f \cdot \beta) * (g \cdot \beta)$ is of the form $h \cdot \beta$ with $h \in \mathcal{L}(G)$, $h$ being determined up to locally $\beta$-negligible sets. We shall write $h = f *^{\beta} g$ and we shall say that $h$ is a *convolution product* of $f$ and $g$ relative to $\beta$. (One omits $\beta$ when no confusion is possible.) If $\beta$ is replaced by $\psi \cdot \beta$, $\psi$ being a continuous representation of $G$ in $\mathbf{R}_+^*$, $h$ does not change (§ 3, No. 1, Prop. 6); if $\beta$ is replaced by $a \beta$ ($a \in \mathbf{R}_+^*$), then $h$ is replaced by $ah$. The convolution product of several functions on $G$ is defined in an analogous manner.

If one of the convolutions of $f$ and $g$ is continuous, it is uniquely determined since the support of $\beta$ is $G$. It is then called *the* convolution product of $f$ and $g$ relative to $\beta$.

It is clear that

$$
f *_{\beta}^{\beta} g = (f \cdot \beta) *_{\beta}^{\beta} g = f *_{\beta}^{\beta} (g \cdot \beta).
$$

#### Proposition 9 {#int-viii-s4-prop-9 .statement}

*Let $f, g$ be in $\mathcal{L}(G)$. Assume that the function $s \mapsto g(s^{-1}x)f(s)\chi(s^{-1})$ is essentially $\beta$-integrable except for a locally $\beta$-negligible set of values of $x$, and that the function*

$$
x \mapsto \int |g(s^{-1}x)f(s)|\chi(s^{-1})\, d\beta(s),
$$

*defined locally $\beta$-almost everywhere, is locally $\beta$-integrable. Then $f$ and $g$ are convolvable.*

This follows from Prop. 1 of No. 1.

#### Proposition 10 {#int-viii-s4-prop-10 .statement}

*Let $f, g$ be in $\mathcal{L}(G)$. Assume that one of these two functions is continuous or is zero on the complement of a countable union of compact sets. If $f$ and $g$ are convolvable, then the function $f * g$ is given locally $\beta$-almost everywhere by*

$$
(f * g)(x) = \int_G g(s^{-1}x)f(s)\chi(s^{-1})\, d\beta(s)
= \int_G f(xs^{-1})g(s)\chi'(s^{-1})\, d\beta(s).
$$

This follows from Prop. 2 of No. 1, and the remarks in No. 4.

In particular, if $f * g$ is continuous and is given at every point by (15), then

$$
(f * g)(e) = \int g(s^{-1})f(s)\chi(s^{-1})\, d\beta(s) = \int f(s^{-1})g(s)\chi'(s^{-1})\, d\beta(s).
$$

Still more particularly, if $\beta$ is a left and right Haar measure, and if $f * g$ and $g * f$ are continuous and are given at every point by (15) and the analogous formula for $g * f$, then

$$
(f * g)(e) = (g * f)(e) = \int f(s)g(s^{-1})\, d\beta(s).
$$

#### Proposition 11 {#int-viii-s4-prop-11 .statement}

— Let $f, g$ be in $\mathcal{L}(G)$. Assume that one of the functions $f, g$ is continuous, and that one of the functions $f, g$ has compact support. Then $f$ and $g$ are convolvable. The formula (15) defines for all $x \in G$ a product $f * g$ that is continuous. If $f \in \mathcal{K}(G)$ and $g \in \mathcal{K}(G)$, then $f * g \in \mathcal{K}(G)$.

This follows from Props. 3 and 4 of No. 2.

#### Proposition 12 {#int-viii-s4-prop-12 .statement}

— Let $p$ and $q$ be two conjugate exponents ($1 \leq p \leq +\infty$). If $f \chi^{-1/q} \in L^1(G, \beta)$ and $g \in L^p(G, \beta)$, then $f$ and $g$ are convolvable, $f * g$ is equal locally $\beta$-almost everywhere to a function in $L^p(G, \beta)$, and
$$
\|f * g\|_p \leq \|f \chi^{-1/q}\|_1 \|g\|_p.
$$
If $f \in L^p(G, \beta)$ and $g {\chi'}^{-1/q} \in L^1(G, \beta)$, then $f$ and $g$ are convolvable, $f * g$ is equal locally $\beta$-almost everywhere to a function in $L^p(G, \beta)$, and
$$
\|f * g\|_p \leq \|f\|_p \|g {\chi'}^{-1/q}\|_1.
$$
This follows from Props. 5 and 6 of No. 2 and the remarks in No. 4.

#### Proposition 13 {#int-viii-s4-prop-13 .statement}

— If $f \chi^{-1} \in L^1(G, \beta)$ and $g \in \overline{\mathcal{K}(G)}$, or if $f \in \mathcal{K}(G)$ and $g {\chi'}^{-1} \in L^1(G, \beta)$, then $f$ and $g$ are convolvable, and (15) defines for every $x \in G$ a product $f * g$ that belongs to $\mathcal{K}(G)$.

This follows from Prop. 5 of No. 2, and the remarks in No. 4.

#### Proposition 14 {#int-viii-s4-prop-14 .statement}

— If $f \chi^{-1} \in L^1(G, \beta)$ and $g \in L^\infty(G, \beta)$, then the formula (15) defines for every $x \in G$ a product $f * g$ that is bounded and is uniformly continuous for the right uniform structure of $G$.

We already know that $f * g$ belongs to $L^\infty(G, \beta)$ (No. 2, Prop. 5); moreover, $(f * g)(x) = \int f(xs^{-1})g(s)\, d\nu(s)$, on setting $\nu = {\chi'}^{-1} \cdot \beta$; $\nu$ is a right Haar measure. Therefore
$$
|(f * g)(x) - (f * g)(x')| \leq \|g\|_\infty \int |f(xs^{-1}) - f(x's^{-1})|\, d\nu(s)
$$
$$
= \|g\|_\infty \int |(f(s^{-1}) - f(x'x^{-1}s^{-1}))\, d\nu(s)
$$
and the latter integral is arbitrarily small provided $x'x^{-1}$ is in a suitable neighborhood of $e$ (§ 2, No. 5, Prop. 8).

#### Proposition 15 {#int-viii-s4-prop-15 .statement}

— Let $p$ and $q$ be two conjugate exponents ($1 < p < +\infty$). Assume that $\beta$ is left-invariant. Let $f \in L^p(G, \beta)$, $g \in L^q(G, \check{\beta})$. Then $f$ and $g$ are convolvable. The formula (15) defines, for every $x \in G$, a product $f * g$ that belongs to $\mathcal{K}(G)$ and is such that
$$
\|f * g\|_\infty \leq \|f\|_p \|g\|_q.
$$

For, we have $\dot{g} \in L^q(G, \beta)$, therefore the function $s \mapsto g(s^{-1}x)f(s)$ is $\beta$-integrable for every $x \in G$. Moreover,

$$
\int |g(s^{-1}x)f(s)| d\beta(s) \leq \left( \int |f(s)|^p d\beta(s) \right)^{1/p} \left( \int |g(s^{-1}x)|^q d\beta(s) \right)^{1/q}
= \|f\|_p \left( \int |\dot{g}(x^{-1}s)|^q d\beta(s) \right)^{1/q} = \|f\|_p \|\dot{g}\|_q,
$$

therefore $f$ and $g$ are convolvable (Prop. 9). One sees at the same time that (15) defines for every $x$ a product $f * g$ such that

$$
|(f * g)(x)| \leq \|f\|_p \|\dot{g}\|_q.
$$

For $f, g$ in $\mathcal{K}(G)$, we have $f * g \in \mathcal{K}(G)$ (Prop. 11); therefore, for $f \in L^p(G, \beta)$ and $g \in L^q(G, \dot{\beta})$, the product $f * g$ furnished by (15) is the uniform limit of functions in $\mathcal{K}(G)$, hence belongs to $\overline{\mathcal{K}(G)}$.

#### Corollary {#int-viii-s4-n5-cor-1 .statement}

— Let $f \in L^2(G, \beta)$, $g \in L^2(G, \beta)$. Then $f$ and $\dot{g}$ are convolvable. One of the convolutions $f * \dot{g}$ belongs to $\overline{\mathcal{K}(G)}$ and its value at $e$ is $\int_G f(s)g(s) d\beta(s)$.

It suffices to take $p = q = 2$ in Prop. 15 and to apply (16).

We no longer assume $\beta$ to be left-invariant. Let $\rho$ be a lower semi-continuous finite function $> 0$ on $G$, such that $\rho(st) \leq \rho(s)\rho(t)$ for all $s, t$ in $G$. We denote by $L^\rho(G, \beta)$ the set of equivalence classes of the complex functions on $G$ that are integrable for $\rho \cdot \beta$. By the mapping $f \mapsto f \cdot \beta$, $L^\rho(G, \beta)$ may be identified with the set of elements of $\mathcal{M}^\rho(G)$ that have base $\beta$ (a set that is independent of the choice of $\beta$). If one sets

$$
\|f\|_\rho = \int_G |f(s)| \rho(s) d\beta(s)
$$

for $f \in L^\rho(G, \beta)$, this identification is compatible with the norms, thus $L^\rho(G, \beta)$ appears as a complete normed subalgebra of $\mathcal{M}^\rho(G)$. It is even a two-sided ideal of $\mathcal{M}^\rho(G)$ by Prop. 10 of §3, No. 2. (For $\rho = 1$, one recovers one of the assertions of No. 4.) In particular, $L^1(G, \beta)$ may be identified with a closed two-sided ideal of $\mathcal{M}^1(G)$.

#### Proposition 16 {#int-viii-s4-prop-16 .statement}

— Let $U$ be a continuous representation of $G$ in a Banach space $E$. Set $\rho(s) = \|U(s)\|$ for all $s \in G$. For every $f \in L^\rho(G, \beta)$, set $U(f) = U(f \cdot \beta)$. Then $f \mapsto U(f)$ is a linear representation of the algebra $L^\rho(G, \beta)$ in $E$, such that $\|U(f)\| \leq \|f\|_\rho$.

This follows from §2, No. 6 and §3, No. 3, Prop. 11.

### 6. Applications

#### Proposition 17 {#int-viii-s4-prop-17 .statement}

— Let G be a locally compact group, A a subset of G, measurable and not locally negligible for a Haar measure. Then $A \cdot A^{-1}$ is a neighborhood of e.

Let $\beta$ be a left Haar measure. There exists a compact subset K of G such that $B = A \cap K$ is integrable with measure > 0 for $\beta$. Let us apply the Cor. of Prop. 15 with $f = g = \varphi_B$. The function $F = \varphi_B * \check{\varphi}_B$ is continuous and > 0 at e. Therefore there exists a neighborhood V of e such that $F(x) > 0$ for $x \in V$. Now,

$$
F(x) = \int \varphi_B(s) \varphi_B(x^{-1}s) d\beta(s) = \beta(B \cap xB).
$$

Therefore, for $x \in V$, one has $B \cap xB \neq \emptyset$, whence $x \in B \cdot B^{-1}$. Thus $V \subset B \cdot B^{-1} \subset A \cdot A^{-1}$.

#### Corollary 1 {#int-viii-s4-prop-17-cor-1 .statement}

— Let H be a subgroup of G measurable for a Haar measure $\beta$. Then H is either open or locally $\beta$-negligible.

For, $H = H \cdot H^{-1}$, therefore if H is not locally $\beta$-negligible, then H contains a neighborhood of e (Prop. 17) hence is open (GT, III, §2, No. 1, Cor. of Prop. 4).

#### Corollary 2 {#int-viii-s4-prop-17-cor-2 .statement}

— Let L be a subset of G stable for multiplication and whose complement is locally negligible for a Haar measure $\beta$. Then $L = G$.

For, $L^{-1}$ and $L \cap L^{-1}$ have locally $\beta$-negligible complements. Now, $L \cap L^{-1}$ is a subgroup, hence is open (Cor. 1) and therefore closed. Therefore $G - (L \cap L^{-1})$, which is open and locally $\beta$-negligible, is empty. Thus $G = L \cap L^{-1}$.

#### Proposition 18 {#int-viii-s4-prop-18 .statement}

— Let G be a locally compact group, $\Gamma$ a set equipped with a multiplication $(u, v) \mapsto uv$ and a Hausdorff topology such that:
1) the topology of $\Gamma$ is invariant under the translations;
2) the restriction of the multiplication to every compact subset of $\Gamma \times \Gamma$ is continuous.

Let $f : G \to \Gamma$ be a mapping of G into $\Gamma$ such that $f(xy) = f(x)f(y)$ for $x, y$ in G, and measurable for a Haar measure $\beta$ on G. Then $f$ is continuous.

Set $g(x) = f(x^{-1})$ for $x \in G$. Since $f$ and $g$ are $\beta$-measurable, there exists a non $\beta$-negligible compact subset K of G such that the restrictions of $f$ and $g$ to K are continuous. The mapping $(x, y) \mapsto f(xy^{-1}) = f(x)g(y)$ of $K \times K$ into $\Gamma$ is continuous because the multiplication of $\Gamma$ is continuous on $f(K) \times g(K)$; now, this mapping may be written as $\varphi \circ \psi$, where $\psi$ is the mapping $(x, y) \mapsto xy^{-1}$ of $K \times K$ onto $K \cdot K^{-1}$, and $\varphi$ is the restriction of $f$ to $K \cdot K^{-1}$. Let $R$ be the equivalence relation defined on $K \times K$ by $\psi$. The mapping $\psi'$ of $(K \times K)/R$ onto $K \cdot K^{-1}$ deduced from $\psi$ by passage to the quotient is continuous, therefore $(K \times K)/R$ is Hausdorff and $\psi'$ is a homeomorphism. Since $\varphi \circ \psi$ is continuous, one sees that the restriction of $f$ to $K \cdot K^{-1}$ is continuous. Now, $K \cdot K^{-1}$ is a neighborhood of $e$ (Prop. 17), therefore $f$ is continuous at $e$. For every $x_0 \in G$, $f(x_0x) = f(x_0)f(x)$, thus $f$ is continuous at $x_0$ because the topology of $\Gamma$ is invariant under translations.

#### Corollary 1 {#int-viii-s4-prop-18-cor-1 .statement}

*Let $G$ be a locally compact group, $\beta$ a Haar measure on $G$, $E$ a Hausdorff barreled locally convex space, $U$ a linear representation of $G$ in $E$, such that $U(s) \in \mathcal{L}(E;E)$ for all $s \in G$, $\beta$-measurable when $\mathcal{L}(E;E)$ is equipped with the topology of pointwise convergence. Then $U$ is a continuous linear representation.*

Let $\Gamma$ be the group of automorphisms of $E$, equipped with the topology of pointwise convergence. This topology is Hausdorff and is invariant under translations. Let $K$ be a compact subset of $\Gamma$. Then $K$ is bounded in $\mathcal{L}(E;E)$ equipped with the topology of pointwise convergence, hence is equicontinuous (TVS, III, §4, No. 2, Th. 1); therefore the mapping $(u,v) \mapsto v \circ u$ of $K \times K$ into $\mathcal{L}(E;E)$ is continuous (*loc. cit.*, §5, No. 5, Cor. 1 of Prop. 9). Therefore, for every $x \in E$, the mapping $s \mapsto U(s)x$ of $G$ into $E$ is continuous (Prop. 18). Since $E$ is barreled, $U$ is continuous (§2, No. 1, Prop. 1).

#### Corollary 2 {#int-viii-s4-prop-18-cor-2 .statement}

*Let $G$ be a locally compact group, $\beta$ a Haar measure on $G$, $E$ a separable Banach space, and $U$ a linear representation of $G$ in $E$ such that $U(s) \in \mathcal{L}(E;E)$ for all $s \in G$. Let $(a_m)$ be a total sequence in $E$, and let $(a'_n)$ be a dense sequence in the unit ball $B'$ of the dual $E'$ of $E$, equipped with the weak topology. Assume that the functions $s \mapsto \langle U(s)a_m, a'_n \rangle$ on $G$ are $\beta$-measurable. Then $U$ is a continuous linear representation.*

Let us first show that for every $z' \in E'$, the scalar functions

$$
s \mapsto \langle U(s)a_m, z' \rangle
$$

are $\beta$-measurable; we may restrict ourselves to the case that $\|z'\| \leq 1$, and, since $B'$ is metrizable for the weak topology (TVS, III, §3, No. 4, Cor. 2 of Prop. 6), there exists a subsequence $(a'_{n_k})$ of $(a'_n)$ that converges weakly to $z'$; the function

$$
s \mapsto \langle U(s)a_m, z' \rangle
$$

is thus the limit of a sequence of $\beta$-measurable functions, whence our assertion. It follows that the mapping $s \mapsto U(s)a_m$ of $G$ into $E$ is $\beta$-measurable for every $m$ (Ch. IV, §5, No. 5, Prop. 10). On the other hand, there exists a sequence $(b_m)$ of elements of $E$, linear combinations of the $a_i$, that is dense in the unit ball of $E$. For every $s \in G$, $\|U(s)\| = \sup_m \|U(s)b_m\|$, therefore $s \mapsto \|U(s)\|$ is measurable. Let $K$ be a compact subset of $G$ and let $\varepsilon > 0$. There exists a compact subset $K_0$ of $K$ such that $\beta(K - K_0) \leq \varepsilon$ and such that the restrictions to $K_0$ of the functions $s \mapsto U(s)a_m$ and $s \mapsto \|U(s)\|$ are continuous. Then the $U(s)$ for $s \in K_0$ are equicontinuous, and the topology of pointwise convergence induces on $U(K_0)$ the topology of pointwise convergence in the set of $a_m$ (TVS, III, §3, No. 4, Prop. 5). Consequently the mapping $s \mapsto U(s)$ of $K_0$ into $\mathcal{L}_s(E; E)$ is continuous. It then suffices to apply Cor. 1.

### 7. Regularization

#### Proposition 19 {#int-viii-s4-prop-19 .statement}

— *Let $G$ be a locally compact group, $\beta$ a relatively invariant positive measure $\neq 0$ on $G$, $\mathcal{B}$ a base for the filter of neighborhoods of $e$ in $G$, consisting of compact neighborhoods. For every $V \in \mathcal{B}$, let $f_V$ be a continuous function $\geq 0$ on $G$, with support contained in $V$, such that $\int f_V d\beta = 1$. If $\mu$ is a measure on $G$ then, in $\mathcal{M}(G)$ equipped with the topology of compact convergence in $\mathcal{H}(G)$,

$$
\mu = \lim_V (\mu * f_V) \cdot \beta = \lim_V (f_V * \mu) \cdot \beta,
$$

the limit being taken with respect to the section filter of $\mathcal{B}$.

For the topology of compact convergence in $\mathcal{C}(G)$, $f_V \cdot \beta$ tends to $\varepsilon_e$ with respect to the section filter of $\mathcal{B}$ (§ 2, No. 7, Cor. 1 of Lemma 4). Therefore $\mu = \lim_V \mu * (f_V \cdot \beta) = \lim_V (f_V \cdot \beta) * \mu$ in $\mathcal{M}(G)$ equipped with the topology of compact convergence in $\mathcal{H}(G)$ (§ 3, No. 3, Cor. of Prop. 12).

#### Remark 1 {#int-viii-s4-n7-rem-1 .statement}

We thus see that every measure on $G$ is the limit of measures admitting a *continuous density* with respect to every Haar measure (for the topology indicated in Prop. 19 and *a fortiori* for the vague topology).

#### Remark 2 {#int-viii-s4-n7-rem-2 .statement}

If $G$ is metrizable, $\mathcal{B}$ can be taken to be a sequence $(V_n)$ of neighborhoods. Then $\mu$ is the limit of the sequence of measures $(\mu * f_{V_n}) \cdot \beta$ with continuous densities. *If $G$ is a real Lie group, the $f_{V_n}$ can be taken to be infinitely differentiable; we shall see later on that the densities $\mu * f_{V_n}$ are then infinitely differentiable.*

#### Proposition 20 {#int-viii-s4-prop-20 .statement}

— *We conserve the hypotheses and notations of Prop. 19.* Let $p \in [1, +\infty[$ and $g \in L^p(G, \beta)$. Then

$$
g = \lim_V g *^\beta f_V = \lim_V f_V *^\beta g
$$

in the sense of the norm $N_p$, the limit being taken with respect to the section filter of $\mathcal{B}$.

It suffices to apply Prop. 6 (iii), and §2, No. 7, Cor. 3 of Lemma 4.

#### Remark 3 {#int-viii-s4-n7-rem-3 .statement}

By Prop. 15, the functions $g * f_V$, $f_V * g$ belong to $\mathcal{K}(G)$.

#### Corollary {#int-viii-s4-n7-cor-1 .statement}

— Let $W$ be a closed linear subspace of $L^1(G, \beta)$. For $W$ to be a left (resp. right) ideal of $L^1(G, \beta)$, it is necessary and sufficient that $W$ be invariant under the left (resp. right) translations of $G$.

Suppose that $W$ is a left ideal. Let $s \in G$ and $g \in W$. We have $\varepsilon_s * g = \lim_V f_V * (\varepsilon_s * g) = \lim_V (f_V * \varepsilon_s) * g$, and $(f_V * \varepsilon_s) * g \in W$, therefore $\varepsilon_s * g \in W$, thus $\gamma(s)g \in W$. Conversely, if $W$ is invariant under the left translations, then $\mu *^\beta g \in W$ for $\mu \in \mathcal{M}^1(G)$ and $g \in W$, therefore $W$ is a fortiori a left ideal of $L^1(G, \beta)$. One argues similarly for right ideals.

#### Example {#int-viii-s4-n7-exa-1 .statement}

We take $G = \mathbf{R}$. Let us define a function $F_n \in \mathcal{K}(\mathbf{R})$ by
$$
F_n(x) = (1 - x^2)^n \quad \text{if } x \in [-1, 1] \\
F_n(x) = 0 \qquad \text{if } x \notin [-1, 1].
$$
Let $A_n = \int_{-1}^{+1} F_n(x) dx$, and $G_n = A_n^{-1} F_n$. It is immediate that the measures $G_n(x) dx$ satisfy the conditions of §2, No. 7, Cor. 1 of Lemma 4. Let $\mu$ be a measure on $\mathbf{R}$ whose support is contained in $[-1/2, 1/2]$. Then
$$
(\mu * G_n)(x) = \int_{\mathbf{R}} G_n(x - y) d\mu(y)
= A_n^{-1} \int_{-1/2}^{1/2} F_n(x - y) d\mu(y).
$$
If $-1/2 \leq x \leq 1/2$, then
$$
(\mu * G_n)(x) = A_n^{-1} \int_{-1/2}^{1/2} [1 - (x - y)^2]^n d\mu(y),
$$
therefore $\mu * G_n$ coincides on $[-1/2, 1/2]$ with a polynomial. In particular, if $f$ is a continuous function with support contained in $[-1/2, 1/2]$, then $f * G_n$ coincides in $[-1/2, 1/2]$ with a polynomial; moreover, by Prop. 5 (iv), and §2, No. 7, Cor. 3 of Lemma 4, $f * G_n$ converges uniformly to $f$.
*If $f$ is of class $C^r$, the derivatives $D^s(f * G_n)$ tend uniformly to $D^s f$ for $0 \leq s \leq r$.*

### Exercises {#int-viii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
