---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 2
section_title: Quotient of a space by a group; homogeneous spaces
lang: en
source: int-vii-ix
book_pages: INT VII.27-INT VII.53, INT VII.87-INT VII.91
pdf_pages: 0033-0059, 0093-0097
extraction: ocr
subsections:
    - "no": 1
      title: General results
      page: 27
      pdf_page: 33
    - "no": 2
      title: The case $\chi = 1$
      page: 29
      pdf_page: 35
    - "no": 3
      title: Another interpretation of $\lambda^\#$
      page: 32
      pdf_page: 38
    - "no": 4
      title: The case that $X/H$ is paracompact
      page: 36
      pdf_page: 42
    - "no": 5
      title: Quasi-invariant measures on a homogeneous space
      page: 38
      pdf_page: 44
    - "no": 6
      title: Relatively invariant measures on a homogeneous space
      page: 43
      pdf_page: 49
    - "no": 7
      title: Haar measure on a quotient group
      page: 44
      pdf_page: 50
    - "no": 8
      title: A transitivity property
      page: 45
      pdf_page: 51
    - "no": 9
      title: Construction of the Haar measure of a group from the Haar measures of certain subgroups
      page: 48
      pdf_page: 54
    - "no": 10
      title: Integration on a fundamental domain
      page: 50
      pdf_page: 56
statements: 53
exercises: 13
content_sha256: 99ba561aafca40f963d3f96797899f8fc83f5e667a8708612f7fd51b6fd36471
---

## § 2. QUOTIENT OF A SPACE BY A GROUP; HOMOGENEOUS SPACES

### 1. General results

Let X be a locally compact space in which a locally compact group H operates on the right, continuously and properly, by $(x, \xi) \mapsto x\xi$ ($x \in X, \xi \in H$). The equivalence relation in X defined by H is open (GT, III, §2, No. 4, Lemma 2) and X/H is Hausdorff (*loc. cit.*, §4, No. 2, Prop. 3) hence locally compact (GT, I, §10, No. 4, Prop. 10). We denote by $\pi$ the canonical mapping of X onto X/H. The saturation of a subset Y of X is $YH = \pi^{-1}(\pi(Y))$. If K is a compact subset of X, then $\pi(K)$ is compact and the saturation $\pi^{-1}(\pi(K))$ of K is closed in X. Every compact subset of X/H is the image under $\pi$ of a compact subset of X (GT, I, §10, No. 4, Prop. 10). *We assume given once and for all a left Haar measure $\beta$ on H*.

Let $\chi$ be a continuous representation of H in $\mathbf{R}_+^*$. If a function g on X satisfies $g(x\xi) = \chi(\xi)g(x)$ for all $x \in X$ and $\xi \in H$, its support S is invariant under H hence may be written $\pi^{-1}(\pi(S))$. We shall denote by $\mathcal{K}^\chi(X)$ the Riesz space formed by the continuous real-valued functions g on X that satisfy $g(x\xi) = \chi(\xi)g(x)$ ($x \in X, \xi \in H$) and whose support is the saturation of a compact subset of X; we denote by $\mathcal{K}_+^\chi(X)$ the set of elements $\geqslant 0$ of $\mathcal{K}^\chi(X)$. In particular, $\mathcal{K}^1(X)$ is none other than the set of continuous functions on X, constant on the orbits, whose support is the saturation of a compact subset.

#### Proposition 1 {#int-vii-s2-prop-1 .statement}

*Let f be a continuous real-valued function on X whose support S has compact intersection with the saturation of every compact subset of X.*

a) *For every $x \in X$, the function $\xi \mapsto f(x\xi)$ on H belongs to $\mathcal{K}(H)$; one sets*

$$
f^\chi(x) = \int_H f(x\xi)\chi(\xi)^{-1}\, d\beta(\xi).
$$

b) *The function $f^\chi$ is continuous, is zero outside SH, and satisfies $f^\chi(x\xi) = \chi(\xi)f^\chi(x)$.*

c) *If g is a continuous real-valued function on X and satisfies $g(x\xi) = \chi(\xi)g(x)$, then $(fg)^\chi = f^1g$ ($f^1$ being given by the formula (1) with $\chi$ replaced by the representation $\xi \mapsto 1$ of H in $\mathbf{R}_+^*$).*

d) *If* $\eta \in \mathbf{H}$, *then* $(\delta(\eta)f)^{\chi} = \chi(\eta)\Delta_{\mathbf{H}}(\eta)^{-1}f^{\chi}$.

Let $x_0 \in X$ and let $V$ be a compact neighborhood of $x_0$ in $X$. The set of $\xi \in \mathbf{H}$ such that $V\xi$ intersects $S$ is also the set of $\xi \in \mathbf{H}$ such that $V\xi$ intersects $S \cap VH$, hence is compact in $\mathbf{H}$ since $S \cap VH$ is compact and $\mathbf{H}$ operates properly in $X$ (GT, III, §4, No. 5, Th. 1); then Lemma 1 of §1, No. 1 proves a) and the continuity of $f^{\chi}$. The rest of b) is obvious. Finally, c) and d) result from the following calculations:

$$
(fg)^{\chi}(x) = \int_{\mathbf{H}} f(x\xi)g(x\xi)\chi(\xi)^{-1}\,d\beta(\xi) = \int_{\mathbf{H}} f(x\xi)g(x)\chi(\xi)\chi(\xi)^{-1}\,d\beta(\xi)
$$
$$
= g(x) \int_{\mathbf{H}} f(x\xi)\,d\beta(\xi) = g(x)f^{1}(x)
$$

$$
(\delta(\eta)f)^{\chi}(x) = \int_{\mathbf{H}} f(x\xi\eta)\chi(\xi)^{-1}\,d\beta(\xi)
$$
$$
= \Delta_{\mathbf{H}}(\eta)^{-1} \int_{\mathbf{H}} f(x\xi)\chi(\xi\eta^{-1})^{-1}\,d\beta(\xi)
$$
$$
= \chi(\eta)\Delta_{\mathbf{H}}(\eta)^{-1} \int_{\mathbf{H}} f(x\xi)\chi(\xi)^{-1}\,d\beta(\xi).
$$

#### Proposition 2 {#int-vii-s2-prop-2 .statement}

*The mapping* $f \mapsto f^{\chi}$ *of* $\mathcal{K}(X)$ *into* $\mathcal{K}^{\chi}(X)$ *is linear, and the image of* $\mathcal{K}(X)$ *(resp. $\mathcal{K}_{+}(X)$) is* $\mathcal{K}^{\chi}(X)$ *(resp. $\mathcal{K}_{+}^{\chi}(X)$).*

Linearity is immediate. It is clear that $f^{\chi} \geqslant 0$ for $f \geqslant 0$. It then suffices to apply the following lemma:

#### Lemma 1 {#int-vii-s2-lem-1 .statement}

— *Let* $K$ *be a compact subset of* $X$, *u a function of* $\mathcal{K}_{+}(X)$ *with* $u(x) > 0$ *for* $x \in K$. *Let* $g \in \mathcal{K}^{\chi}(X)$ *be such that* $\operatorname{Supp} g \subset KH$.
a) *One has* $\inf_{x \in KH} u^{1}(x) > 0$.
b) *The function* $h$ *equal to* $g/u^{1}$ *on* $KH$, *and to* $0$ *on* $X - KH$, *belongs to* $\mathcal{K}^{\chi}(X)$.
c) $g = (uh)^{\chi}$.
One has $u^{1}(x) > 0$ for $x \in K$, therefore $\inf_{x \in KH} u^{1}(x) = \inf_{x \in K} u^{1}(x) > 0$.
Assertion b) follows from this at once. Finally, $(uh)^{\chi} = u^{1}h$ by Prop. 1 c), and it is clear that $u^{1}h = g$.

Let I be a relatively bounded linear form (Ch. II, §2, No. 2) on $\mathcal{K}^{\chi}(X)$. Then $f \mapsto I(f^{\chi})$ is a relatively bounded linear form on $\mathcal{K}(X)$, that is, a *measure* $\mu_{I}$ on $X$. The mapping $I \mapsto \mu_{I}$ is injective by Prop. 2. The measures $\mu_{I}$ on $X$ so obtained may be characterized as follows:

#### Proposition 3 {#int-vii-s2-prop-3 .statement}

*Let* $\mu$ *be a measure on* $X$. *The following conditions are equivalent:*

a) There exists a relatively bounded linear form I on $\mathcal{K}^\chi(X)$ such that $I(f^\chi) = \mu(f)$ for all $f \in \mathcal{K}(X)$.
b) $\delta(\xi)\mu = \chi(\xi)^{-1} \Delta_H(\xi)\mu$ for all $\xi \in H$.
c) For all $f, g$ in $\mathcal{K}(X)$,

(2)
$$
\mu(f \cdot g^1) = \mu(f^\chi \cdot g) .
$$

d) If $f \in \mathcal{K}(X)$ is such that $f^\chi = 0$, then $\mu(f) = 0$.

a) $\Rightarrow$ b): If $\mu(f) = I(f^\chi)$ then, taking into account Prop. 1 d),

$$
\langle \delta(\xi)\mu, f \rangle = \langle \mu, \delta(\xi^{-1})f \rangle = I\left( (\delta(\xi^{-1})f)^\chi \right)
= I(\chi(\xi)^{-1} \Delta_H(\xi)f^\chi)
= \chi(\xi)^{-1} \Delta_H(\xi) \langle \mu, f \rangle ,
$$

whence $\delta(\xi)\mu = \chi(\xi)^{-1} \Delta_H(\xi)\mu$.

b) $\Rightarrow$ c): Suppose hypothesis b) is satisfied. Note that the functions $(x, \xi) \mapsto f(x)g(x\xi)$ and $(x, \xi) \mapsto f(x\xi)g(x)$ on $X \times H$ are continuous with compact support (because $H$ operates properly in $X$); this established, Th. 2 of Ch. III, §4, No. 1 permits us to write:

$$
\int_X f(x) d\mu(x) \int_H g(x\xi) d\beta(\xi) = \int_H d\beta(\xi) \int_X f(x)g(x\xi) d\mu(x)
= \int_H d\beta(\xi) \int_X f(x\xi^{-1})g(x)\chi(\xi)\Delta_H(\xi)^{-1} d\mu(x)
= \int_X g(x) d\mu(x) \int_H f(x\xi^{-1})\chi(\xi)\Delta_H(\xi)^{-1} d\beta(\xi)
= \int_X g(x) d\mu(x) \int_H f(x\xi)\chi(\xi)^{-1} d\beta(\xi),
$$

which proves c).

c) $\Rightarrow$ d): If c) is verified and if $f^\chi = 0$, then $\mu(f \cdot g^1) = 0$ for all $g \in \mathcal{K}(X)$, thus $\mu(f) = 0$ on choosing $g \in \mathcal{K}(X)$ such that $g^1 = 1$ on $\mathrm{Supp}\, f$ (which is possible by Prop. 2 applied with $\chi = 1$).

d) $\Rightarrow$ a): If condition d) is satisfied, there exists a linear form I on $\mathcal{K}^\chi(X)$ such that $\mu(f) = I(f^\chi)$ for $f \in \mathcal{K}(X)$, and this form is relatively bounded by virtue of Prop. 2.

### 2. The case $\chi = 1$

If $f$ is a function on $X/H$, then $f \circ \pi$ is a function on $X$ constant on the orbits, continuous if and only if $f$ is continuous. The mapping $f \mapsto f \circ \pi$ defines in particular a bijection of $\mathcal{K}(X/H)$ onto $\mathcal{K}^1(X)$.

We can then, in the case that $\chi = 1$, reformulate certain results of No. 1 in the following way:

Let $f$ be a continuous numerical function on $X$ whose support has compact intersection with the saturation of every compact subset of $X$. The formula

$$
f^b(\pi(x)) = \int_H f(x\xi)\, d\beta(\xi)
$$

defines a continuous function $f^b$ on $X/H$. If $g$ is a continuous function on $X/H$, then

$$
(f \cdot g \circ \pi)^b = f^b \cdot g .
$$

If $\eta \in H$, then

$$
(\delta(\eta)f)^b = \Delta_H(\eta)^{-1} f^b .
$$

One must not forget that the definition of $f^b$ depends on the choice of $\beta$. If $H$ is compact and $\beta$ is normalized, the function $f^b$ is sometimes called the *orbital mean* of $f$.

If $f \in \mathcal{K}(X)$, then $f^b \in \mathcal{K}(X/H)$. The mapping $f \mapsto f^b$ of $\mathcal{K}(X)$ into $\mathcal{K}(X/H)$ is linear, and the image of $\mathcal{K}(X)$ (resp. $\mathcal{K}_+(X)$) is $\mathcal{K}(X/H)$ (resp. $\mathcal{K}_+(X/H)$).

#### Remark 1 {#int-vii-s2-n2-rem-1 .statement}

— We are going to show that the mapping $f \mapsto f^b$ is a *strict morphism* (GT, III, §2, No. 8) of $\mathcal{K}(X)$ onto $\mathcal{K}(X/H)$.

a) The mapping is continuous: it suffices to prove that, for every compact subset $K$ of $X$, the restriction of $f \mapsto f^b$ to $\mathcal{K}(X, K)$ is a continuous mapping of $\mathcal{K}(X, K)$ into $\mathcal{K}(X/H, \pi(K))$ (TVS, II, §4, No. 4, Prop. 5); since $H$ operates properly in $X$, the set $P$ of $\xi \in H$ such that $K\xi$ intersects $K$ is compact; one concludes from (3) that $\sup_{x \in K} |f^b(\pi(x))| \leq \beta(P) \sup_{x \in K} |f(x)|$, and this proves our assertion.

b) Let $K'$ be a compact subset of $X/H$. Let us choose a compact subset $K$ of $X$ such that $\pi(K) = K'$, and let us show that the restriction of $f \mapsto f^b$ to $\mathcal{K}(X, K)$ is a strict morphism of $\mathcal{K}(X, K)$ onto $\mathcal{K}(X/H, K')$. It suffices to construct a right inverse for this restriction (GT, III, §6, No. 2, Prop. 3). Now, by Lemma 1 of No. 1 (whose notations we adopt), one obtains such an inverse by composing the following mappings:
$\alpha)$ the mapping $f' \mapsto f' \circ \pi$ of $\mathcal{K}(X/H, K')$ into the set $E$ of functions of $\mathcal{K}^1(X)$ whose support is contained in $KH$;
$\beta)$ the mapping of $E$ into $E$ that, to every $g \in E$, makes correspond the function equal to $g/u^1$ on $KH$, and to 0 on $X - KH$;
$\gamma)$ the mapping of $E$ into $\mathcal{K}(X)$ that, to every function $h \in E$, makes correspond $uh$.

c) This established, if $V$ is a convex neighborhood of 0 in $\mathcal{K}(X)$, then $V \cap \mathcal{K}(X, K)$ is a convex neighborhood of 0 in $\mathcal{K}(X, K)$, therefore $V^b \cap \mathcal{K}(X/H, K')$ is a convex neighborhood of 0 in $\mathcal{K}(X/H, K')$ by b), therefore $V^b$ is a neighborhood of 0 in $\mathcal{K}(X/H)$ (TVS, II, §4, No. 4). This completes the proof.

#### Proposition 4 {#int-vii-s2-prop-4 .statement}

a) *Let $\lambda$ be a measure on $X/H$. There exists one and only one measure $\lambda^\#$ on $X$ such that*
$$
\int_{X/H} f^b d\lambda = \int_X f d\lambda^\#
$$
*for all $f \in \mathcal{K}(X)$. One has $\delta(\xi)\lambda^\# = \Delta_H(\xi)\lambda^\#$ for all $\xi \in H$.*

b) *Conversely, let $\mu$ be a measure on $X$ such that $\delta(\xi)\mu = \Delta_H(\xi)\mu$ for all $\xi \in H$. There exists one and only one measure $\lambda$ on $X/H$ such that $\mu = \lambda^\#$.*

This is a special case of No. 1, Prop. 3.

#### Definition 1 {#int-vii-s2-def-1 .statement}

*With hypotheses and notations as in Prop. 4, $\lambda$ is called the quotient of $\mu$ by $\beta$ and is denoted $\frac{\mu}{\beta}$ or $\mu/\beta$.*

The mapping $\lambda \mapsto \lambda^\#$ of $\mathcal{M}(X/H)$ into $\mathcal{M}(X)$ is none other than the transpose of the mapping $f \mapsto f^b$ of $\mathcal{K}(X)$ into $\mathcal{K}(X/H)$. Let $\mathfrak{F}$ be a filter on $\mathcal{M}(X/H)$; to say that $\lim_{\lambda,\mathfrak{F}} \lambda^\#(f) = 0$ for all $f \in \mathcal{K}(X)$ is equivalent to saying that $\lim_{\lambda,\mathfrak{F}} \lambda(f') = 0$ for all $f' \in \mathcal{K}(X/H)$; therefore the mapping $\lambda \mapsto \lambda^\#$ is, for the vague topologies, an *isomorphism* of $\mathcal{M}(X/H)$ onto a linear subspace of $\mathcal{M}(X)$. This subspace is *vaguely closed*, since it is the set of $\mu \in \mathcal{M}(X)$ such that $\delta(\xi)\mu = \Delta_H(\xi)\mu$ for all $\xi \in H$. It is clear that the conditions $\lambda \geqslant 0$ and $\lambda^\# \geqslant 0$ are equivalent.

The formula (6) may, by analogy with the usual notation for double integrals, be written
$$
\int_X f(x) d\lambda^\#(x) = \int_{X/H} d\lambda(\dot{x}) \int_H f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$
This involves an abuse of notation, the integral $\int_H f(x\xi) d\beta(\xi)$ being regarded as a function of $\dot{x}$ and not of $x$; this manner of writing will be used frequently in what follows provided no confusion can arise.

#### Remark 2 {#int-vii-s2-n2-rem-2 .statement}

— Let E be a locally convex vector space and let m be a vectorial measure on $X/H$ with values in E. The mapping $f \mapsto m(f^b)$ of $\mathcal{K}(X)$ into E is then a vectorial measure on X, with values in E, which we shall again denote by $m^\#$. The mapping $m \mapsto m^\#$ is again an *isomorphism* of $\mathcal{L}(\mathcal{K}(X/H); E)$ onto a linear subspace A of $\mathcal{L}(\mathcal{K}(X); E)$ (when these spaces are equipped with the topology of pointwise convergence). Moreover, since the mapping $f \mapsto f^b$ is a surjective strict morphism, the subspace A consists precisely of the vectorial measures n on X that are zero on the kernel N of the mapping $f \mapsto f^b$. In order that $n \in A$, it is therefore necessary and sufficient that the scalar measures $z' \circ n$ be zero on N for every $z' \in E'$. One then deduces from Prop. 3 that $n \in A$ if and only if $\delta(\xi)n = \Delta_H(\xi)n$ for all $\xi \in H$.

### 3. Another interpretation of $\lambda^\#$

For every $x \in X$, the mapping $\xi \mapsto x\xi$ of H into X is proper (GT, III, §4, No. 2, Prop. 4), therefore $\beta$ admits an image measure on X under this mapping, which image is concentrated on the orbit $xH$ (Ch. V, §6, No. 2, Cor. 3 of Prop. 2); since $\beta$ is left-invariant, this image measure depends only on the class $u = \pi(x)$ of $x$ in $X/H$, and will be denoted $\beta_u$. By definition, for $f \in \mathcal{K}(X)$,

$$
\int_X f(y)\, d\beta_u(y) = \int_H f(x\xi)\, d\beta(\xi) = f^\flat(u).
$$

We thus see that

$$
(\varepsilon_u)^\# = \beta_u.
$$

#### Lemma 2 {#int-vii-s2-lem-2 .statement}

*Let f be a function on X, with values in a topological space.*

a) *If f is a numerical function $\geq 0$ then, for $x \in X$,*

$$
\int_X^* f(y)\, d\beta_{\dot{x}}(y) = \int_H^* f(x\xi)\, d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

b) *For f to be $\beta_{\dot{x}}$-measurable, it is necessary and sufficient that the function $\xi \mapsto f(x\xi)$ on H be $\beta$-measurable.*

c) *Suppose that f is a function on X, with values in a Banach space or in $\overline{\mathbf{R}}$; then, for f to be $\beta_{\dot{x}}$-integrable (resp. essentially $\beta_{\dot{x}}$-integrable), it is necessary and sufficient that the function $\xi \mapsto f(x\xi)$ on H be $\beta$-integrable (resp. essentially $\beta$-integrable), in which case $\int_X f(y)\, d\beta_{\dot{x}}(y) = \int_H f(x\xi)\, d\beta(\xi)$.*

This follows from Ch. V, §4, Prop. 2, Prop. 3 and Th. 2.

Since $f^\flat \in \mathcal{K}(X/H)$ for $f \in \mathcal{K}(X)$, formula (8) proves that the mapping $u \mapsto \beta_u$ of $X/H$ into $\mathcal{M}(X)$ is vaguely continuous, that the family $(\beta_u)$ is $\lambda$-adequate$^1$ for any positive measure $\lambda$ on $X/H$, and that

$$
\lambda^\# = \int_{X/H} \beta_u\, d\lambda(u),
$$

which furnishes a new interpretation of $\lambda^\#$.

$^1$ In the sense of the first edition of Ch. V, hence *a fortiori* in the sense of the second (cf. the footnote to the Example of Ch. VI, §1, No. 1).

#### Proposition 5 {#int-vii-s2-prop-5 .statement}

— Let $\lambda$ be a positive measure on $X/H$.

a) Let $f$ be a $\lambda^\#$-measurable function on $X$, with values in a topological space, constant outside a countable union of $\lambda^\#$-integrable sets. Then, the set of $\dot{x} \in X/H$ such that the function $\xi \mapsto f(x\xi)$ is not $\beta$-measurable is locally $\lambda$-negligible.

b) Let $f$ be a $\lambda^\#$-measurable function $\geq 0$ on $X$, zero outside a countable union of $\lambda^\#$-integrable sets. Then, the function $\dot{x} \mapsto \int^* f(x\xi) d\beta(\xi)$ on $X/H$ is $\lambda$-measurable, and

$$
\int_X^* f(x) d\lambda^\#(x) = \int_{X/H}^* d\lambda(\dot{x}) \int_H^* f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

c) Let $f$ be a $\lambda^\#$-integrable function on $X$, with values in a Banach space or in $\overline{\mathbf{R}}$. Then, the set of $\dot{x} \in X/H$ such that $\xi \mapsto f(x\xi)$ is not $\beta$-integrable is $\lambda$-negligible; the function $f^b$ on $X/H$ defined almost everywhere by the formula

$$
f^b(\dot{x}) = \int_H f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x))
$$

is $\lambda$-integrable, and

$$
\int_{X/H} f^b d\lambda = \int_X f d\lambda^\#
$$

and

$$
\int_{X/H} |f^b| d\lambda \leq \int_X |f| d\lambda^\#.
$$

d) Let $f$ be a $\lambda^\#$-measurable function on $X$, with values in a Banach space or in $\overline{\mathbf{R}}$, and zero outside a countable union of $\lambda^\#$-integrable sets. Then, for $f$ to be $\lambda^\#$-integrable, it is necessary and sufficient that

$$
\int_{X/H}^* d\lambda(\dot{x}) \int_H^* |f(x\xi)| d\beta(\xi) < +\infty \quad (\dot{x} = \pi(x)).
$$

Taking into account Lemma 2, the assertions a), b) and c) follow from Ch. V, §3, Prop. 4, Prop. 5 and Th. 1 (with the exception of (13), which follows from (12) because it is clear that $|f^b| \leq |f|^b$); d) follows from b).

#### Proposition 6 {#int-vii-s2-prop-6 .statement}

— Let $\lambda$ be a positive measure on $X/H$.

a) Let $N$ be a subset of $X/H$. For $N$ to be locally $\lambda$-negligible, it is necessary and sufficient that $\pi^{-1}(N)$ be locally $\lambda^\#$-negligible.

b) Let g be a function on X/H, with values in a topological space. For g to be $\lambda$-measurable, it is necessary and sufficient that $g \circ \pi$ be $\lambda^\#$-measurable.

c) Let h be a function on X/H, with values in a Banach space or in $\overline{\mathbf{R}}$. For h to be locally $\lambda$-integrable, it is necessary and sufficient that $h \circ \pi$ be locally $\lambda^\#$-integrable, in which case $(h \cdot \lambda)^\# = (h \circ \pi) \cdot \lambda^\#$.

Suppose $h \circ \pi$ is locally $\lambda^\#$-integrable. For every $f \in \mathcal{K}(X)$, $f \cdot (h \circ \pi)$ is $\lambda^\#$-integrable, therefore (Prop. 5) the function $(f \cdot (h \circ \pi))^b = f^b \cdot h$ is $\lambda$-integrable and

$$
\int_{X/H} f^b \cdot h \, d\lambda = \int_X f \cdot (h \circ \pi) \, d\lambda^\#.
$$

Since $f \mapsto f^b$ is a surjective mapping of $\mathcal{K}(X)$ onto $\mathcal{K}(X/H)$, this shows that h is locally $\lambda$-integrable and that

$$
(h \cdot \lambda)^\# = (h \circ \pi) \cdot \lambda^\#.
$$

In particular, if $\pi^{-1}(N)$ is locally $\lambda^\#$-negligible, then $\varphi_N \circ \pi$ is locally $\lambda^\#$-negligible, therefore $(\varphi_N \cdot \lambda)^\# = (\varphi_N \circ \pi) \cdot \lambda^\# = 0$, consequently $\varphi_N \cdot \lambda = 0$ and N is locally $\lambda$-negligible. Now suppose that $g \circ \pi$ is $\lambda^\#$-measurable. Let K' be a compact subset of X/H. Let $f \in \mathcal{K}_+(X)$ be such that $f^b = 1$ on K' (No. 1, Prop. 2), and let $K = \operatorname{Supp} f$; one has $\pi(K) \supset K'$. There exists a partition of K formed of a $\lambda^\#$-negligible set M and a sequence $(K_n)$ of compact sets such that $(g \circ \pi)|K_n$ is continuous for every n. Then $g|_{\pi(K_n)}$ is continuous. Let P be the set of points of K' not belonging to $\pi(K_1) \cup \pi(K_2) \cup \ldots$; then $\pi^{-1}(P) \cap K$ is contained in M, hence is $\lambda^\#$-negligible; therefore $f \cdot \varphi_{\pi^{-1}(P)}$ is $\lambda^\#$-negligible; it follows (Prop. 5) that

$$
0 = \int_X f \cdot \varphi_{\pi^{-1}(P)} \, d\lambda^\# = \int_{X/H} f^b \cdot \varphi_P \, d\lambda \geq \int_{X/H}^* \varphi_P \, d\lambda,
$$

therefore P is $\lambda$-negligible, and g is $\lambda$-measurable.

If N is locally $\lambda$-negligible, then $\pi^{-1}(N)$ is locally $\lambda^\#$-negligible (Ch. V, §6, No. 6, Cor. 1 of Prop. 10). If g is $\lambda$-measurable, then $g \circ \pi$ is $\lambda^\#$-measurable (*ibid.*). Finally, suppose h is locally $\lambda$-integrable. Then we already know that $h \circ \pi$ is $\lambda^\#$-measurable. For every $f \in \mathcal{K}_+(X)$ we have, by Prop. 5,

$$
\int_X^* f(x)|h|(\pi(x)) \, d\lambda^\#(x) = \int_{X/H}^* |h|(u)f^b(u) \, d\lambda(u) < +\infty,
$$

therefore $h \circ \pi$ is locally $\lambda^\#$-integrable.

#### Corollary 1 {#int-vii-s2-prop-6-cor-1 .statement}

— Let $\lambda, \lambda'$ be two positive measures on $X/H$. For $\lambda'$ to have base $\lambda$, it is necessary and sufficient that ${\lambda'}^\#$ have base $\lambda^\#$. For $\lambda$ and $\lambda'$ to be equivalent, it is necessary and sufficient that $\lambda^\#$ and ${\lambda'}^\#$ be equivalent.

The first assertion follows from Prop. 6, a) and c). The second follows from the first.

#### Corollary 2 {#int-vii-s2-prop-6-cor-2 .statement}

— Let $\lambda$ be a positive measure on $X/H$, and $f$ a $\lambda^\#$-measurable numerical function on $X$. Suppose that, for every $\xi \in H$, $\delta(\xi)f = f$ locally $\lambda^\#$-almost everywhere. Then, there exists a $\lambda$-measurable function $g$ on $X/H$ such that $f = g \circ \pi$ locally $\lambda^\#$-almost everywhere.

Replacing $f$ by $f/(1+|f|)$, one reduces to the case that $f$ is bounded, hence locally $\lambda^\#$-integrable. Let $\mu = f \cdot \lambda^\#$. The hypothesis on $f$ implies that $\delta(\xi)\mu = f \cdot \delta(\xi)\lambda^\# = \Delta_H(\xi)\mu$ for all $\xi \in H$. There then exists (Prop. 4) a measure $\lambda'$ on $X/H$ such that $\mu = {\lambda'}^\#$. By Cor. 1, there exists a locally $\lambda$-integrable function $g$ on $X/H$ such that $\lambda' = g \cdot \lambda$. By Prop. 6, $f \cdot \lambda^\# = {\lambda'}^\# = (g \circ \pi) \cdot \lambda^\#$, whence $f = g \circ \pi$ locally $\lambda^\#$-almost everywhere.

#### Corollary 3 {#int-vii-s2-prop-6-cor-3 .statement}

— a) Let $(\lambda_\iota)_{\iota \in I}$ be a family of real measures on $X/H$. For the family $(\lambda_\iota)$ to be bounded above in $\mathcal{M}(X/H)$, it is necessary and sufficient that the family $(\lambda_\iota^\#)$ be bounded above in $\mathcal{M}(X)$, in which case

$$
\sup(\lambda_\iota^\#) = (\sup \lambda_\iota)^\#.
$$

b) Let $\lambda$ be a real measure on $X/H$. Then $(\lambda^+)^\# = (\lambda^\#)^+$ and $(\lambda^-)^\# = (\lambda^\#)^-$.

c) Let $\lambda$ be a complex measure on $X/H$. Then $|\lambda|^\# = |\lambda^\#|$.

Assume the family $(\lambda_\iota)$ to be bounded above and let $\mu = \sup \lambda_\iota$. Since $\lambda \geq 0$ implies $\lambda^\# \geq 0$, we have $\mu^\# \geq \lambda_\iota^\#$ for all $\iota$, which shows that the family $(\lambda_\iota^\#)$ is bounded above and that

$$
(\sup \lambda_\iota)^\# \geq \sup(\lambda_\iota^\#).
$$

Conversely, assume the family $(\lambda_\iota^\#)$ to be bounded above and let $\nu = \sup(\lambda_\iota^\#)$. Since $\delta(\xi)\lambda_\iota^\# = \Delta_H(\xi)\lambda_\iota^\#$ for all $\xi \in H$, obviously $\delta(\xi)\nu = \Delta_H(\xi)\nu$, therefore there exists a measure $\mu' \in \mathcal{M}(X/H)$ such that $\nu = {\mu'}^\#$. Since $\lambda^\# \geq 0$ implies $\lambda \geq 0$, we have $\mu' \geq \lambda_\iota$ for all $\iota$, which shows that the family $(\lambda_\iota)$ is bounded above and that $\nu = {\mu'}^\# \geq (\sup \lambda_\iota)^\#$, whence

$$
\sup(\lambda_\iota^\#) \geq (\sup \lambda_\iota)^\#,
$$

which completes the proof of a). The assertion b) then follows at once since, for example, $\lambda^+$ is none other than $\sup(\lambda, 0)$. To prove c), it suffices to note that $|\lambda| = \sup \mathcal{R}(\alpha \lambda)$ over the complex numbers $\alpha$ of absolute value 1, and on the other hand that $\mathcal{R}(\mu^\#) = (\mathcal{R}\mu)^\#$ for every $\mu \in \mathcal{M}(X/H)$.

#### Remark 1 {#int-vii-s2-n3-rem-1 .statement}

Prop. 6 a) may be expressed by saying that $\lambda$ is a *pseudo-image* measure of $\lambda^\#$ under $\pi$ (Ch. VI, §3, No. 2, Def. 1).

#### Remark 2 {#int-vii-s2-n3-rem-2 .statement}

Suppose $H$ is *compact* and $\beta$ is normalized. The saturation of every compact subset of $X$ is compact. Therefore, if $f \in \mathcal{K}(X/H)$ then $f \circ \pi \in \mathcal{K}(X)$; and, for every positive measure $\lambda$ on $X/H$, Prop. 5 c) gives

$$
\int_X (f \circ \pi)(x)\, d\lambda^\#(x) = \int_{X/H} f(u)\, d\lambda(u).
$$

In other words, $\lambda$ is the *image* of $\lambda^\#$ under $\pi$.

#### Remark 3 {#int-vii-s2-n3-rem-3 .statement}

Cor. 3 c) of Prop. 6 shows at once that the results of this subsection remain valid in the case of complex measures (except for those that involve the upper integral).

#### Remark 4 {#int-vii-s2-n3-rem-4 .statement}

Let $m$ be a vectorial measure on $X/H$ with values in $E$, and let $q$ be a lower semi-continuous semi-norm on $E$. For $m$ to be $q$-majorizable (Ch. VI, §2, No. 3, Def. 3), it is necessary and sufficient that $m^\#$ be so, in which case $q(m^\#) = q(m)^\#$. This follows at once from the definitions and Cor. 3 a).

On the other hand, let $\mu$ be a positive measure on $X/H$. For $m$ to be scalarly of base $\mu$, it is necessary and sufficient that $m^\#$ be scalarly of base $\mu^\#$: this follows from Cor. 1.

Finally, if $m$ has base $\mu$, with density $f$ with respect to $\mu$ (Ch. VI, §2, No. 4, Def. 4), then $m^\#$ has base $\mu^\#$, with density $f \circ \pi$: this follows from Prop. 6 c).

### 4. The case that $X/H$ is paracompact

If $X/H$ is paracompact, we shall first see that the vector spaces $\mathcal{K}^\chi(X)$, for variable $\chi$, are all *isomorphic* to each other, and in particular isomorphic to $\mathcal{K}^1(X)$.

#### Proposition 7 {#int-vii-s2-prop-7 .statement}

*Assume $X/H$ paracompact. Let $\chi$ be a continuous representation of $H$ in $\mathbf{R}_+^*$.*

a) *There exists on $X$ a continuous function $r$, with values $> 0$, such that $r(x\xi) = \chi(\xi)r(x)$ for all $x \in X$ and $\xi \in H$.*

b) *The mapping $g \mapsto g/r$ is an isomorphism of the vector space $\mathcal{K}^\chi(X)$ onto the vector space $\mathcal{K}^1(X)$.*

Let us apply Prop. 1 of No. 1 on taking $f$ to be a function $\geqslant 0$ that is not identically zero on any orbit (this is possible by Lemma 1 of Appendix 1); then $r = f^\chi$ satisfies the properties of a). The assertion b) is obvious.

#### Proposition 8 {#int-vii-s2-prop-8 .statement}

*Assume $X/H$ paracompact. There exists a continuous function $h \geqslant 0$ on $X$, whose support has compact intersection with* the saturation of every compact subset of X, and is such that $h^b = 1$. For such a function, one has $g = (h \cdot (g \circ \pi))^b$ for every continuous function $g$ on $X/H$.

Let us apply Prop. 1 of No. 1, with $\chi = 1$, on taking for $f$ a function $\geqslant 0$ that is not identically zero on any orbit. We have $f^1(x) > 0$ at every point $x$ of $X$. Set $h = f/f^1$. Then $h^1 = f^1/f^1 = 1$, therefore $h^b = 1$. It follows that if $g$ is a continuous function on $X/H$, then $(h \cdot (g \circ \pi))^b = h^b \cdot g = g$.

#### Remark 1 {#int-vii-s2-n4-rem-1 .statement}

In particular, let $X$ be a locally compact space on which a discrete group $D$ operates continuously and properly on the right; suppose $X/D$ is paracompact. Then, there exists a continuous function $h \geqslant 0$ on $X$ whose support has compact intersection with the saturation of every compact subset of $X$, and is such that $\sum_{d \in D} h(xd) = 1$ for every $x \in X$ (all terms of the sum being zero except for a finite number of them).

#### Remark 2 {#int-vii-s2-n4-rem-2 .statement}

Let us conserve the hypotheses and notations of Prop. 8. The mapping $g \mapsto h \cdot (g \circ \pi)$ is a continuous mapping of $\mathcal{K}(X/H)$ into $\mathcal{K}(X)$ that is a right inverse of the mapping $f \mapsto f^b$. Consequently, every bounded (resp. compact) subset of $\mathcal{K}(X/H)$ is the image of a bounded (resp. compact) subset of $\mathcal{K}(X)$. From this, one deduces immediately that the mapping $\lambda \mapsto \lambda^\#$ is again an isomorphism of $\mathcal{M}(X/H)$ onto a closed linear subspace of $\mathcal{M}(X)$ when these spaces are equipped with the topology of bounded (resp. compact) convergence.

#### Proposition 9 {#int-vii-s2-prop-9 .statement}

— *We conserve the hypotheses and notations of Prop. 8.* Let $\lambda$ be a positive measure on $X/H$.

a) *The pair* $(\pi, h)$ *is $\lambda^\#$-adapted, and* $\int_X h(x) \varepsilon_{\pi(x)} d\lambda^\#(x) = \lambda$.

b) *The mapping* $\pi$ *is proper for the measure* $h \cdot \lambda^\#$, *and* $\pi(h \cdot \lambda^\#) = \lambda$.

c) *Let* $k$ *be a function on* $X/H$, *with values in a Banach space or in* $\overline{\mathbf{R}}$. *For* $k$ *to be measurable (resp. locally integrable, essentially integrable, integrable) for* $\lambda$, *it is necessary and sufficient that* $h \cdot (k \circ \pi)$ *be so for* $\lambda^\#$; *and, if* $k$ *is essentially integrable for* $\lambda$, *then*

$$
\int_{X/H} k \, d\lambda = \int_X h \cdot (k \circ \pi) \, d\lambda^\#.
$$

Let $f \in \mathcal{K}(X/H)$. Then $h \cdot (f \circ \pi) \in \mathcal{K}(X)$ and

$$
\int_X h(x) f(\pi(x)) d\lambda^\#(x) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}) \int_H h(x\xi) d\beta(\xi) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}),
$$

whence a). The assertion b) is proved similarly. The assertions of c) concerning measurability, essential integrability and formula (14) may then be obtained by applying the results of Ch. V (\S4, Prop. 3, \S5, Th. 1, \S4, Th. 2). If $k$ is $\lambda$-integrable, then $h \cdot (k \circ \pi)$ is $\lambda^\#$-integrable (Ch. V, \S3, No. 3, Th. 1). If $h \cdot (k \circ \pi)$ is $\lambda^\#$-integrable, Prop. 5 proves that $(h \cdot (k \circ \pi))^b = h^b \cdot k = k$ is $\lambda$-integrable. If $k$ is locally $\lambda$-integrable, then $h \cdot (k \circ \pi)$ is locally $\lambda^\#$-integrable (Prop. 6). Finally, suppose $h \cdot (k \circ \pi)$ locally $\lambda^\#$-integrable; for every $f \in \mathcal{H}(X/H)$, $h \cdot (k \circ \pi) \cdot (f \circ \pi)$ has compact support, and
$$
|h \cdot (k \circ \pi) \cdot (f \circ \pi)| \leq M |h \cdot (k \circ \pi)|,
$$
where $M = \sup |f|$; therefore $h \cdot ((kf) \circ \pi)$ is $\lambda^\#$-integrable, consequently $kf$ is $\lambda$-integrable, by what has already been proved; this proves that $k$ is indeed locally $\lambda$-integrable.

#### Corollary {#int-vii-s2-n4-cor-1 .statement}

— *The continuous linear mapping* $f \mapsto f^b$ *of* $L^1(X, \lambda^\#)$ *into* $L^1(X/H, \lambda)$ *defined by Prop. 5 is surjective*.

Suppose first that $X/H$ is paracompact and let $h$ be a function on $X$ satisfying the conditions of Prop. 8. If $k$ is a $\lambda$-integrable numerical function on $X/H$, then $h \cdot (k \circ \pi)$ is $\lambda^\#$-integrable and $(h \cdot (k \circ \pi))^b = k$ (Prop. 9).

In the general case, let $u \in L^1(X/H, \lambda)$. There exists a function $f \in \mathcal{L}^1(X/H, \lambda)$ with class $u$ and zero outside a countable union of compact sets $K_n$. Let us define recursively a sequence of relatively compact open sets $U_n$ of $X/H$ such that $U_{n+1} \supset K_n \cup \overline{U}_n$, and let $V$ be the union of the $U_n$. Then $V$ is an open subset of $X/H$, a countable union of compact subsets $\overline{U}_n$, hence is paracompact (GT, I, \S9, No. 10, Th. 5). Set $Y = \overline{\pi}^{-1}(V)$ and let $\lambda_V$ (resp. $\lambda_Y^\#$) be the measure induced by $\lambda$ (resp. $\lambda^\#$) on $V$ (resp. $Y$). It is clear that $Y/H$ may be identified with $V$ (GT, I, \S3, Prop. 10) and that $\lambda_Y^\#$ may be identified with $(\lambda_V)^\#$. Moreover, $f$ is zero outside $V$ and belongs to $\mathcal{L}^1(V, \lambda_V)$. Therefore, there exists $g \in \mathcal{L}^1(Y, \lambda_Y^\#)$ such that $g^b = f$ almost everywhere in $V$. Extending $g$ by 0 on $X - Y$, one obtains a function $g_1 \in \mathcal{L}^1(X, \lambda^\#)$, and it is clear that the class of $g_1^b$ in $L^1(X/H, \lambda)$ is none other than $u$.

#### Remark 3 {#int-vii-s2-n4-rem-3 .statement}

— Suppose $X/H$ paracompact, and let us retain the notations of Proposition 9. The mapping $k \mapsto h \cdot (k \circ \pi)$ of $L^1(X/H, \lambda)$ into $L^1(X, \lambda^\#)$ is then *isometric* by (14) and is a *right inverse* of the mapping $f \mapsto f^b$ of $L^1(X, \lambda^\#)$ onto $L^1(X/H, \lambda)$.

### 5. Quasi-invariant measures on a homogeneous space

#### Lemma 3 {#int-vii-s2-lem-3 .statement}

— *Let G be a locally compact group, $\mu$ a left Haar measure on G, $\nu$ and $\nu'$ two nonzero quasi-invariant measures on G. If, for every $s \in G$, the densities of $\gamma(s)\nu$ with respect to $\nu$ and of $\gamma(s)\nu'$* with respect to $\nu'$ are equal locally $\mu$-almost everywhere, then $\nu$ and $\nu'$ are proportional.

Write $\nu = \rho \cdot \mu$, $\nu' = \rho' \cdot \mu$, where $\rho, \rho'$ are locally $\mu$-integrable functions on $G$ and are everywhere nonzero ($\S 1$, No. 9, Prop. 11). For every $s \in G$,

$$
\gamma(s)\nu = (\gamma(s)\rho) \cdot \mu, \qquad \gamma(s)\nu' = (\gamma(s)\rho') \cdot \mu,
$$

and the hypothesis implies that $\rho^{-1} \cdot \gamma(s)\rho = {\rho'}^{-1} \cdot \gamma(s)\rho'$ locally $\mu$-almost everywhere. Set $\sigma = \rho'/\rho$, which is a $\mu$-measurable function on $G$. For every $s \in G$, $\gamma(s)\sigma = \sigma$ locally $\mu$-almost everywhere. Therefore $\sigma$ is equal to a constant locally $\mu$-almost everywhere, by Cor. 2 of Prop. 6 applied with $X = H = G$.

Let $G$ be a locally compact group, $H$ a closed subgroup of $G$. Consider the homogeneous space $G/H$ of left cosets with respect to $H$, on which $G$ operates continuously on the left. We are going to show that there exists one and only one class of nonzero quasi-invariant measures on $G/H$.

Note that $H$ operates on $G$ continuously and properly by right translations; and the quotient space, which is none other than $G/H$, is paracompact (GT, III, $\S 4$, No. 6, Prop. 13). We may therefore apply the results of Nos. 1 to 4, with $X = G$. We thus have mappings $f \mapsto f^b$ of $\mathcal{K}(G)$ onto $\mathcal{K}(G/H)$, and $\lambda \mapsto \lambda^\#$ of $\mathcal{M}(G/H)$ into $\mathcal{M}(G)$ (once a left Haar measure $\beta$ on $H$ has been fixed). The fact that $G$ operates on the left in $G/H$ gives rise to a supplementary property:

$$
\begin{align*}
(15) \qquad & \gamma_{G/H}(s) \cdot f^b = (\gamma_G(s) \cdot f)^b \qquad (s \in G,\ f \in \mathcal{K}(G)) \\
(16) \qquad & (\gamma_{G/H}(s) \cdot \lambda)^\# = \gamma_G(s) \cdot \lambda^\# \qquad (s \in G,\ \lambda \in \mathcal{M}(G/H)).
\end{align*}
$$

Indeed, for every $x \in G$,

$$
(\gamma_{G/H}(s) \cdot f^b)(\pi(x)) = f^b(s^{-1}\pi(x)) = f^b(\pi(s^{-1}x))
= \int_H f(s^{-1}x\xi)\, d\beta(\xi) = \int_H (\gamma_G(s)f)(x\xi)\, d\beta(\xi) = (\gamma_G(s)f)^b(\pi(x)),
$$

whence formula (15), which implies formula (16).

#### Lemma 4 {#int-vii-s2-lem-4 .statement}

Let $\lambda$ be a measure $\neq 0$ on $G/H$, and $\mu$ a left Haar measure on $G$. The following properties are equivalent:
a) $\lambda$ is quasi-invariant under $G$;
b) for a subset $A$ of $G/H$ to be locally $\lambda$-negligible, it is necessary and sufficient that $\overline{\pi}^{-1}(A)$ be locally $\mu$-negligible;
c) the measure $\lambda^\#$ is equivalent to $\mu$.

Suppose this to be the case and let $\lambda^\# = \rho \cdot \mu$, where $\rho$ is a locally $\mu$-integrable function that is everywhere nonzero. Then, for every $s \in G$, the density $\theta_s$ of $\gamma_{G/H}(s)\lambda$ with respect to $\lambda$ is such that

$$
\theta_s(\pi(x)) = \frac{\rho(s^{-1}x)}{\rho(x)}
$$

locally $\mu$-almost everywhere on $G$.

c) $\Rightarrow$ b): This follows at once from Prop. 6 a).

b) $\Rightarrow$ a): If property b) holds, then the set of locally $\lambda$-negligible subsets of $G/H$ is invariant under $G$, thus $\lambda$ is quasi-invariant under $G$.

a) $\Rightarrow$ c): Assume $\lambda$ is quasi-invariant under $G$; for every $s \in G$, $\lambda$ and $\gamma_{G/H}(s)\lambda$ are equivalent, therefore $\lambda^\#$ and $\gamma_G(s) \cdot \lambda^\# = (\gamma_{G/H}(s) \cdot \lambda)^\#$ are equivalent (Cor. 1 of Prop. 6); since $\lambda^\# \neq 0$, $\lambda^\#$ is equivalent to $\mu$ (\S 1, No. 9, Prop. 11).

Moreover, for every $s \in G$,

$$
(\theta_s \circ \pi) \cdot \lambda^\# = (\theta_s \cdot \lambda)^\# = (\gamma_{G/H}(s)\lambda)^\# = \gamma_G(s)\lambda^\#
$$
$$
= (\gamma_G(s)\rho) \cdot \mu = \frac{\gamma_G(s)\rho}{\rho} \cdot \lambda^\#,
$$

whence (17).

The equivalence of a) and b) implies first the uniqueness result already announced, and even a more precise result:

#### Theorem 1 {#int-vii-s2-thm-1 .statement}

*Let $G$ be a locally compact group, $H$ a closed subgroup of $G$.*

a) *Any two nonzero quasi-invariant measures on $G/H$ are equivalent; the subsets of $G/H$ locally negligible for these measures are those whose inverse image in $G$ is locally negligible for a Haar measure.*

b) *Let $\lambda, \lambda'$ be two nonzero quasi-invariant measures on $G/H$. If, for every $s \in G$, the densities of $\gamma_{G/H}(s)\lambda$ with respect to $\lambda$ and of $\gamma_{G/H}(s)\lambda'$ with respect to $\lambda'$ are equal almost everywhere for $\lambda$ (or $\lambda'$), then $\lambda$ and $\lambda'$ are proportional.*

The assertion a) follows at once from Lemma 4. Let $\lambda$ and $\lambda'$ be two nonzero quasi-invariant measures satisfying the condition of b). Then, for every $s \in G$, the densities of $\gamma_G(s)\lambda^\#$ with respect to $\lambda^\#$ and of $\gamma_G(s){\lambda'}^\#$ with respect to ${\lambda'}^\#$ are equal locally $\mu$-almost everywhere, therefore (Lemma 3) $\lambda^\#$ and ${\lambda'}^\#$ are proportional, hence $\lambda$ and $\lambda'$ are proportional.

On the other hand, Lemma 4 reduces the search for nonzero quasi-invariant measures on $G/H$ to that for the measures on $G$ equivalent to

Haar measure and of the form $\lambda^\#$. On this subject we have the following lemma:

#### Lemma 5 {#int-vii-s2-lem-5 .statement}

*Let $\mu$ be a left Haar measure on $G$, and $\rho$ a locally $\mu$-integrable function. For $\rho \cdot \mu$ to be of the form $\lambda^\#$, it is necessary and sufficient that, for every $\xi \in H$,*

$$
\rho(x\xi) = \frac{\Delta_H(\xi)}{\Delta_G(\xi)} \rho(x)
$$

*locally $\mu$-almost everywhere on $G$.*

To say that $\rho \cdot \mu$ is of the form $\lambda^\#$ amounts to saying that, for every $\xi \in H$, $\delta(\xi)(\rho \cdot \mu) = \Delta_H(\xi)\rho \cdot \mu$ (Prop. 4). Now,

$$
\delta(\xi)(\rho \cdot \mu) = (\delta(\xi)\rho) \cdot (\delta(\xi)\mu) = \Delta_G(\xi)(\delta(\xi)\rho) \cdot \mu,
$$

whence the lemma.

We can now establish the announced existence result, and even a more precise result:

#### Theorem 2 {#int-vii-s2-thm-2 .statement}

*Let $G$ be a locally compact group, $H$ a closed subgroup of $G$, $\mu$ a left Haar measure on $G$, and $\beta$ a left Haar measure on $H$.

a) *There exist functions $\rho$ continuous and $> 0$ on $G$, such that*

$$
\rho(x\xi) = \frac{\Delta_H(\xi)}{\Delta_G(\xi)} \rho(x)
$$

*for all* $x \in G$ *and* $\xi \in H$.

b) *Given such a function $\rho$, one can form the measure* $\lambda = (\rho \cdot \mu)/\beta$ *on* $G/H$, *and* $\lambda$ *is a nonzero positive measure quasi-invariant under* $G$.

c) *For* $s, x$ *in* $G$, $\rho(sx)/\rho(x)$ *depends only on* $s$ *and* $\pi(x)$, *hence defines a function* $\chi$ *continuous and* $> 0$ *on* $G \times (G/H)$ *such that*

$$
\chi(s, \pi(x)) = \frac{\rho(sx)}{\rho(x)}.
$$

*Then*

$$
\gamma_{G/H}(s)\lambda = \chi(s^{-1}, .) \cdot \lambda \quad \text{for all } s \in G.
$$

a) follows from Prop. 7.
b) follows from Lemmas 5 and 4.
c) follows from (17).

#### Remark 1 {#int-vii-s2-n5-rem-1 .statement}

One deduces from Remark 1 of No. 3 that the nonzero quasi-invariant measures on G/H are none other than the pseudo-images under $\pi$ of a Haar measure on G.

#### Remark 2 {#int-vii-s2-n5-rem-2 .statement}

If G is a Lie group, we shall see later that the function $\rho$ of Th. 2 can be chosen to be infinitely differentiable.*

Under the conditions of Th. 2, certain results of Nos. 3 and 4 may be specialized as follows (on taking into account Ch. V, §4, Th. 2 and Prop. 2 for passing from properties relative to $\mu$ to properties relative to $\rho \cdot \mu$):

a) Let $f$ be a $\mu$-measurable function on G, with values in a topological space, constant outside a countable union of $\mu$-integrable sets; then, the set of $\dot{x} \in G/H$ such that the function $\xi \mapsto f(x\xi)$ is not $\beta$-measurable is locally $\lambda$-negligible.

b) Let $f$ be a $\mu$-measurable function $\geqslant 0$ on G, zero outside a countable union of $\mu$-integrable sets. Then, the function
$$
\dot{x} \mapsto \int_{H}^{*} f(x\xi) d\beta(\xi)
$$
on $G/H$ is $\lambda$-measurable and
$$
\int_{G}^{*} f(x)\rho(x) d\mu(x) = \int_{G/H}^{*} d\lambda(\dot{x}) \int_{H}^{*} f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

c) Let $f$ be a $\rho \cdot \mu$-integrable function on G, with values in a Banach space or in $\overline{\mathbf{R}}$. Then, the set of $\dot{x} \in G/H$ such that $\xi \mapsto f(x\xi)$ is not $\beta$-integrable is $\lambda$-negligible; the function $\dot{x} \mapsto \int_{H} f(x\xi) d\beta(\xi)$ is $\lambda$-integrable, and
$$
\int_{G} f(x)\rho(x) d\mu(x) = \int_{G/H} d\lambda(\dot{x}) \int_{H} f(x\xi) d\beta(\xi).
$$

d) There exists a continuous function $h \geqslant 0$ on G, whose support has compact intersection with the saturation KH of every compact subset K of G, and such that $\int_{H} h(x\xi) d\beta(\xi) = 1$ for every $x \in G$. For a function g on G/H to be measurable (resp. locally integrable, essentially integrable, integrable) for $\lambda$, it is necessary and sufficient that $h \cdot (g \circ \pi)$ be so for $\rho \cdot \mu = \lambda^{\sharp}$; and, when g is essentially integrable for $\lambda$, one has
$$
\int_{G/H} g(u) d\lambda(u) = \int_{G} h(x)g(\pi(x)) \rho(x) d\mu(x).
$$

### 6. Relatively invariant measures on a homogeneous space

Let G again be a locally compact group, H a closed subgroup, $\beta$ a left Haar measure on H.

#### Lemma 6 {#int-vii-s2-lem-6 .statement}

Let $\lambda$ be a measure on $G/H$, $\chi$ a continuous representation of G in $\mathbf{C}^*$. The following properties are equivalent:
a) $\lambda$ is relatively invariant on $G/H$ with multiplier $\chi$;
b) $\lambda^\#$ is relatively invariant on G with left multiplier $\chi$;
c) $\lambda^\#$ is of the form $a \chi \cdot \mu$ ($a \in \mathbf{C}$).

The condition a) means that, for every $s \in G$,

$$
\gamma_{G/H}(s)\lambda = \chi(s)^{-1}\lambda;
$$

this is equivalent to $(\gamma_{G/H}(s)\lambda)^\# = \chi(s)^{-1}\lambda^\#$, that is, to

$$
\gamma_G(s)\lambda^\# = \chi(s)^{-1}\lambda^\#.
$$

Whence the equivalence of a) and b). The equivalence of b) and c) follows from §1, No. 8, Cor. 1 of Prop. 10.

#### Theorem 3 {#int-vii-s2-thm-3 .statement}

Let G be a locally compact group, H a closed subgroup of G, $\mu$ (resp. $\beta$) a left Haar measure on G (resp. H), $\chi$ a continuous representation of G in $\mathbf{C}^*$.

a) In order that there exist on $G/H$ a nonzero measure relatively invariant under G and with multiplier $\chi$, it is necessary and sufficient that $\chi(\xi) = \Delta_H(\xi)/\Delta_G(\xi)$ for all $\xi \in H$.

b) This measure is then unique up to a constant factor; more precisely, it is proportional to $(\chi \cdot \mu)/\beta$.

For there to exist on $G/H$ a nonzero measure relatively invariant under G with multiplier $\chi$, it is necessary and sufficient (Lemma 6) that $\chi \cdot \mu$ be of the form $\lambda^\#$, hence (No. 2, Prop. 4) that $\delta(\xi)(\chi \cdot \mu) = \Delta_H(\xi)(\chi \cdot \mu)$ for all $\xi \in H$. This condition may also be written $\chi(\xi)\chi \cdot \Delta_G(\xi)\mu = \Delta_H(\xi)\chi \cdot \mu$, that is,

$$
\chi(\xi) = \Delta_H(\xi)/\Delta_G(\xi)
$$

for all $\xi \in H$. Whence a). The assertion b) follows at once from Lemma 6 and the fact that the mapping $\lambda \mapsto \lambda^\#$ is injective.

We shall see in §3 (No. 3, Example 4) some very simple examples where the representation $\xi \mapsto \Delta_H(\xi)/\Delta_G(\xi)$ cannot be extended to a continuous representation of G in $\mathbf{C}^*$. In this case, there therefore does not exist any nonzero complex measure on $G/H$ relatively invariant under G.

#### Corollary 1 {#int-vii-s2-thm-3-cor-1 .statement}

For there to exist on $G/H$ a nonzero positive measure relatively invariant under G, it is necessary and sufficient that there exist a continuous representation of $G$ in $\mathbf{R}_+^*$ extending the representation $\xi \mapsto \Delta_H(\xi)/\Delta_G(\xi)$.

Note that this condition is fulfilled when $H$ is unimodular.

#### Corollary 2 {#int-vii-s2-thm-3-cor-2 .statement}

— For there to exist on $G/H$ a nonzero positive measure invariant under $G$, it is necessary and sufficient that $\Delta_G$ coincide with $\Delta_H$ on $H$.

#### Corollary 3 {#int-vii-s2-thm-3-cor-3 .statement}

— Suppose that $H$ is unimodular and that there exists on $G/H$ a nonzero bounded positive measure $\nu$ relatively invariant under $G$. Then $\nu$ is invariant, and $G$ is unimodular.

Let $\chi$ be the multiplier of $\nu$. For every $s \in G$, $\nu$ and $\gamma(s)\nu$ have the same finite total mass (\S 1, No. 1, formula (6)); since $\gamma(s)\nu = \chi(s)^{-1}\nu$, we have $\chi(s) = 1$. Thus $\nu$ is invariant. By Cor. 2, $\Delta_G(s) = 1$ for all $s \in H$. Let $G'$ be the set of $t \in G$ such that $\Delta_G(t) = 1$. This is a closed normal subgroup of $G$ containing $H$. Let $\pi$ be the canonical mapping of $G/H$ onto $G/G'$. Then $\pi(\nu)$ is a nonzero, bounded positive measure invariant under $G$. Therefore the left Haar measure of the group $G/G'$ is bounded, so that $G/G'$ is compact (\S 1, No. 2, Prop. 2). Consequently the image of $G$ under $\Delta_G$ is a compact subgroup of $\mathbf{R}_+^*$; this subgroup is reduced to $\{1\}$, thus $\Delta_G = 1$ on all of $G$.

### 7. Haar measure on a quotient group

#### Proposition 10 {#int-vii-s2-prop-10 .statement}

— Let $G$ be a locally compact group, $G'$ a closed normal subgroup, $G''$ the group $G/G'$, $\pi$ the canonical mapping of $G$ onto $G/G'$, and $\alpha, \alpha', \alpha''$ left Haar measures on $G, G', G''$.

a) Multiplying $\alpha$ by a constant factor if necessary, we can suppose that $\alpha'' = \alpha/\alpha'$. In particular, if $f \in \mathcal{K}(G)$ then

$$
\int_G f(x)\,d\alpha(x) = \int_{G''} d\alpha''(\dot{x}) \int_{G'} f(x\xi)\,d\alpha'(\xi) \quad (\dot{x} = \pi(x)).
$$

b) One has $\Delta_G(\xi) = \Delta_{G'}(\xi)$ for all $\xi \in G'$; in particular, if $G$ is unimodular then so is $G'$.

c) The kernel of the representation $\Delta_G$ of $G$ in $\mathbf{R}_+^*$ is the largest unimodular closed normal subgroup of $G$.

Applying Th. 3 of No. 6 with $\chi = 1$ (and in the knowledge that here, there exists a measure on $G/G'$ invariant under $G$, namely $\alpha''$), we obtain a) and b); c) follows at once from b).

#### Proposition 11 {#int-vii-s2-prop-11 .statement}

— We maintain the notations of Prop. 10. Let $u$ be an automorphism of $G$ such that $u(G') = G'$. Let $u'$ be the restriction of $u$ to $G'$, and $u''$ the automorphism of $G''$ deduced from $u$ by passage to the quotients. Then

$$
\operatorname{mod}_G(u) = \operatorname{mod}_{G'}(u') \operatorname{mod}_{G''}(u'').
$$

For, if $\alpha'' = \alpha/\alpha'$ then $u''(\alpha'') = u(\alpha)/u'(\alpha')$, that is,
$$
\operatorname{mod}_{G''}(u'')^{-1}\alpha'' = \operatorname{mod}_G(u)^{-1}\alpha/\operatorname{mod}_{G'}(u')^{-1}\alpha'
$$
$$
= \frac{\operatorname{mod}_{G'}(u')}{\operatorname{mod}_G(u)} (\alpha/\alpha') = \frac{\operatorname{mod}_{G'}(u')}{\operatorname{mod}_G(u)} \alpha'',
$$
whence the proposition.

#### Corollary {#int-vii-s2-n7-cor-1 .statement}

— *For every* $x \in G$,
$$
\Delta_G(x) = \Delta_{G/G'}(\dot{x}) \operatorname{mod}(i_x),
$$
*where* $\dot{x}$ *denotes the canonical image of* $x$ *in* $G/G'$, *and* $i_x$ *the automorphism* $s \mapsto x^{-1}sx$ *of* $G'$.

This follows from Prop. 11, and formula (33) of §1, No. 4.

### 8. A transitivity property

Let $X$ be a locally compact space in which a locally compact group $H$ acts on the right, continuously and *properly*, by $(x, \xi) \mapsto x\xi$ ($x \in X,\ \xi \in H$). Let $H'$ be a closed subgroup of $H$; then $H'$ operates on the right in $X$, continuously and *properly*. We shall denote by $\pi, \pi', p$ the canonical mappings of $X$ onto $X/H$, of $X$ onto $X/H'$, and of $H$ onto $H/H'$.

Let $\beta, \beta'$ be left Haar measures on $H, H'$; suppose that $\Delta_H$ and $\Delta_{H'}$ *coincide on* $H'$; one can then form the measure $\beta/\beta'$ on $H/H'$, left-invariant under $H$ (No. 6, Th. 3). On the other hand, let $\mu$ be a positive measure on $X$ such that
$$
\delta(\xi)\mu = \Delta_H(\xi)\mu
$$
for $\xi \in H$; one can then form the measures $\mu/\beta$ on $X/H$ and $\mu/\beta'$ on $X/H'$ (No. 2, Prop. 4). We are going to write $\mu/\beta'$ as the *integral*, with respect to $\mu/\beta$, of a family of measures on $X/H'$ indexed by the points of $X/H$. When $H' = \{e\}$, we shall find ourselves again in the situation of No. 3.

The mapping $(x, \xi) \mapsto \pi'(x\xi)$ of $X \times H$ into $X/H'$ is continuous; since $\pi'(x\xi) = \pi'(x\xi\xi')$ for all $\xi' \in H'$ this mapping defines, by passage to the quotient, a *continuous* mapping of $X \times (H/H')$ into $X/H'$; whence, for each fixed $x$ in $X$, a partial mapping $\omega_x$ of $H/H'$ into $X/H'$, deduced by passage to the quotient from the mapping $\psi_x : \xi \mapsto x\xi$ of H into X. Note that $\psi_{x\xi} = \psi_x \circ \gamma_H(\xi)$, therefore that $\omega_{x\xi} = \omega_x \circ \gamma_{H/H'}(\xi)$ for all $\xi \in H$.

#### Lemma 7 {#int-vii-s2-lem-7 .statement}

*Let K be a compact subset of X/H', and L a compact subset of X. Then $\bigcup_{x \in L} \omega_x^{-1}(K)$ is relatively compact in H/H'._

Let $K_1$ be a compact subset of X such that $\pi'(K_1) = K$. Let $K_2$ be the set of $\xi \in H$ such that $L\xi$ intersects $K_1$. Then $K_2$ is compact (GT, III, §4, No. 5, Th. 1). Let $\xi \in H$ be such that $p(\xi) \in \bigcup_{x \in L} \omega_x^{-1}(K)$. Thus, there exists an $x \in L$ such that $\omega_x(p(\xi)) \in K$, in other words such that $\pi'(x\xi) \in K$. Since $\pi'(K_1) = K$, there exists $\xi' \in H'$ such that $x\xi\xi' \in K_1$. Then $\xi\xi' \in K_2$, therefore $p(\xi) = p(\xi\xi') \in p(K_2)$. We have thus shown that $\bigcup_{x \in L} \omega_x^{-1}(K) \subset p(K_2)$.

This lemma shows first of all that the mapping $\omega_x$ is *proper*. One can therefore form the measure $\omega_x(\beta/\beta')$ on $X/H'$, which is concentrated on $\omega_x(H/H') = \pi'(\psi_x(H)) = \pi'(xH)$. If $f \in \mathcal{K}(X/H')$, Lemma 7 and §1, No. 1, Lemma 1 show that the function $x \mapsto \langle f, \omega_x(\beta/\beta') \rangle$ is continuous on X; moreover, $\langle f, \omega_x(\beta/\beta') \rangle$ is zero when Supp $f$ does not intersect $\pi'(xH)$, in other words when $\pi(x)$ does not belong to the canonical image of Supp $f$ in $X/H$.

Moreover, if $x \in H$ then

$$
\omega_{x\xi}(\beta/\beta') = \omega_x(\gamma_{H/H'}(\xi)(\beta/\beta')) = \omega_x(\beta/\beta').
$$

The mapping $x \mapsto \omega_x(\beta/\beta')$ of X into $\mathcal{M}(X/H')$ therefore defines by passage to the quotient a mapping $u \mapsto (\beta/\beta')_u$ of $X/H$ into $\mathcal{M}(X/H')$. The foregoing shows that, for every $f \in \mathcal{K}(X/H')$, the mapping $u \mapsto \langle f, (\beta/\beta')_u \rangle$ is continuous with compact support. Consequently the mapping $u \mapsto (\beta/\beta')_u$ *is a vaguely continuous and* $(\mu/\beta)$*-adequate family of measures on* $X/H'$, *with* $X/H$ *as index set*.

Let $x \in X$, and $u = \pi(x) \in X/H$. Let $f$ be a function on $X/H'$, with values in a Banach space or in $\overline{\mathbf{R}}$. By Ch. V, §4, Th. 2, for $f$ to be $(\beta/\beta')_u$-integrable, it is necessary and sufficient that the function $p(\xi) \mapsto f(\omega_x(p(\xi))) = f(\pi'(x\xi))$ on $H/H'$ be $(\beta/\beta')$-integrable, in which case

$$
(21) \quad \int_{X/H'} f(u') d(\beta/\beta')_u(u') = \int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}) \qquad (\dot{\xi} = p(\xi)).
$$

One has analogous properties for measurability, the upper integral and the essential integral.

#### Proposition 12 {#int-vii-s2-prop-12 .statement}

— *With the foregoing notations*,

$$
\int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u) = \mu/\beta'.
$$

Let $f \in \mathcal{K}(X)$, and let $f^b \in \mathcal{K}(X/H')$, defined by

$$
f^b(\pi'(x)) = \int_{H'} f(x\xi') d\beta'(\xi').
$$

It suffices (cf. No. 2) to prove that $f^b$ has the same integral with respect to the two members of (22). Now, $\langle \mu/\beta', f^b \rangle = \langle \mu, f \rangle$. On the other hand,

$$
\left\langle \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u), f^b \right\rangle = \int_{X/H} \langle (\beta/\beta')_u, f^b \rangle d(\mu/\beta)(u).
$$

Now, let $x \in X$ and $u = \pi(x)$. We have

$$
\langle (\beta/\beta')_u, f^b \rangle = \langle \omega_x(\beta/\beta'), f^b \rangle = \int_{H/H'} f^b(\omega_x(\dot{\xi})) d(\beta/\beta')(\dot{\xi})
$$
$$
= \int_{H/H'} f^b(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})
$$
$$
= \int_{H/H'} d(\beta/\beta')(\dot{\xi}) \int_{H'} f(x\xi\xi') d\beta'(\xi')
$$
$$
= \int_H f(x\xi) d\beta(\xi).
$$

Therefore

$$
\left\langle \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u), f^b \right\rangle = \int_{X/H} d(\mu/\beta)(u) \int_H f(x\xi) d\beta(\xi) = \langle \mu, f \rangle,
$$

which proves the proposition.

#### Corollary 1 {#int-vii-s2-prop-12-cor-1 .statement}

— a) *Let f be a function on X/H', with values in a Banach space or in $\overline{\mathbf{R}}$, integrable for $\mu/\beta'$. There exists a $(\mu/\beta)$-negligible subset N of X/H having the following property: if $x \in X$ is such that $\pi(x) \notin N$, then the function $f \circ \omega_x$ on H/H', that is, the function $\dot{\xi} \mapsto f(\pi'(x\xi))$, is integrable for $\beta/\beta'$. The integral $\int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})$ depends only on $\dot{x} = \pi(x)$, and is a $(\mu/\beta)$-integrable function of $\dot{x}$; and*

$$
\int_{X/H'} f d(\mu/\beta') = \int_{X/H} d(\mu/\beta)(\dot{x}) \int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}).
$$

b) Let $f$ be a function $\geq 0$ on $X/H'$, measurable for $\mu/\beta'$ and zero outside a countable union of $(\mu/\beta')$-integrable sets. Then

$$
\pi(x) \mapsto \int_{H/H'}^* f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})
$$

is $(\mu/\beta)$-measurable, and

$$
\int_{X/H'}^* f d(\mu/\beta') = \int_{X/H}^* d(\mu/\beta)(\dot{x}) \int_{H/H'}^* f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}).
$$

c) Let $f$ be a function on $X/H'$ with values in a Banach space or in $\overline{\mathbf{R}}$, measurable for $\mu/\beta'$ and zero outside a countable union of $(\mu/\beta')$-integrable sets. Then, for $f$ to be $(\mu/\beta')$-integrable, it is sufficient that

$$
\int_{X/H}^* d(\mu/\beta)(\dot{x}) \int_{H/H'}^* |f(\pi'(x\xi))| d(\beta/\beta')(\dot{\xi}) < +\infty.
$$

#### Corollary 2 {#int-vii-s2-prop-12-cor-2 .statement}

— Let $G$ be a locally compact group, $A$ and $B$ closed subgroups of $G$ such that $A \supset B$. Suppose that there exists, on the homogeneous space $G/B$ of left cosets with respect to $B$, a nonzero positive measure $\alpha$ that is invariant under $G$ and is bounded.

a) The canonical image of $\alpha$ in $G/A$ is a nonzero positive measure, invariant under $G$, and bounded.

b) $\Delta_G$ coincides with $\Delta_A$ on $A$ and with $\Delta_B$ on $B$.

c) There exists, on the homogeneous space $A/B$ of left cosets of $A$ with respect to $B$, a nonzero positive measure invariant under $A$ and bounded.

The assertion a) is immediate. The assertion b) follows from a) and No. 6, Cor. 2 of Th. 3. By b), $\Delta_A$ coincides with $\Delta_B$ on $B$, and one can therefore apply the results of the present subsection, on taking $X = G$, $H = A$, $H' = B$. The function 1 on $G/B$ is $\alpha$-integrable. By a) of Cor. 1, the function 1 on $A/B$ is integrable for $\beta/\beta'$, where $\beta$ and $\beta'$ denote left Haar measures on $A$ and $B$; thus $\beta/\beta'$ is bounded.

### 9. Construction of the Haar measure of a group from the Haar measures of certain subgroups

Let $G$ be a locally compact group, $X$ and $Y$ two closed subgroups of $G$ such that $\Omega = XY$ contains a neighborhood $U$ of $e$. Then $\Omega$ is open in $G$; for, for any $x_0 \in X$ and $y_0 \in Y$, $XY = (x_0X)(Yy_0) \supset x_0Uy_0$, and $x_0 U y_0$ is a neighborhood of $x_0 y_0$; thus $\Omega$ is a neighborhood of each of its points.

*When G is a Lie group with Lie algebra $g$, the condition imposed on X and Y is satisfied if the subalgebras corresponding to X and Y have sum $g$.*

The group $X \times Y$ operates continuously in G on the left, by the law $(x, y) \cdot s = x s y^{-1}$ ($x \in X, y \in Y, s \in G$). Let $Z = X \cap Y$. The stabilizer of e in $X \times Y$ is the subgroup $Z_0$ of $X \times Y$ formed by the pairs $(z, z)$, where $z \in Z$, a subgroup canonically isomorphic to $Z$. Thus the set $\Omega$ may be identified with the homogeneous space $(X \times Y)/Z_0$ of left cosets; more precisely, the mapping $(x, y) \mapsto xy^{-1}$ of $X \times Y$ onto $\Omega$ defines, by passage to the quotient, a continuous bijection of $(X \times Y)/Z_0$ onto $\Omega$. We shall assume that this mapping *is a homeomorphism*. (This is notably the case if G is countable at infinity: cf. App. I.)

#### Proposition 13 {#int-vii-s2-prop-13 .statement}

— *Suppose in addition that Z is compact. Let $\mu_G, \mu_X, \mu_Y$ be left Haar measures on G, X, Y, and $\Lambda$ the restriction of $\Delta_G$ to Y. Then the restriction $\mu$ of $\mu_G$ to $\Omega$ is, up to a constant factor, the image of $\mu_X \otimes (\Lambda^{-1} \cdot \mu_Y)$ under the mapping $(x, y) \mapsto xy^{-1}$ of $X \times Y$ onto $\Omega$ (a mapping that is proper).

For $x \in X, y \in Y$,

$$
\gamma((x, y)) \mu = \delta(y) \gamma(x) \mu = \Delta_G(y) \mu .
$$

Identifying $\Omega$ with the homogeneous space $(X \times Y)/Z_0$ and choosing a suitable Haar measure on $Z_0$, one sees that $\mu^\#$ is the product of the left Haar measure of $X \times Y$, namely $\mu_X \otimes \mu_Y$, by the function $(x, y) \mapsto \Delta_G(y)^{-1}$ (No. 6, Lemma 6). On the other hand $\mu$ is, up to a constant factor, the image of $\mu^\#$ under the canonical mapping of $X \times Y$ onto $\Omega$ (No. 3, Remark 2).

#### Corollary {#int-vii-s2-n9-cor-1 .statement}

— *Let f be a function defined on $\Omega$, with values in a Banach space or in $\overline{\mathbf{R}}$. For f to be $\mu$-integrable, it is necessary and sufficient that the function $(x, y) \mapsto f(xy) \Delta_G(y) \Delta_Y(y)^{-1}$ be $(\mu_X \otimes \mu_Y)$-integrable, in which case*

$$
\int_\Omega f(\omega) d\mu(\omega) = a \iint_{X \times Y} f(xy) \Delta_G(y) \Delta_Y(y)^{-1} d\mu_X(x) d\mu_Y(y),
$$

where $a$ is a constant $> 0$ independent of f.

By Prop. 13, and Ch. V, §4, No. 4, Th. 2, for f to be $\mu$-integrable, it is necessary and sufficient that the function $(x, y) \mapsto f(xy^{-1})$ be integrable for $\mu_X \otimes (\Lambda^{-1} \cdot \mu_Y)$, or again that the function $(x, y) \mapsto f(xy^{-1}) \Delta_G(y)^{-1}$ be integrable for $\mu_X \otimes \mu_Y$, or again that the function $(x, y) \mapsto f(xy) \Delta_G(y) \Delta_Y(y)^{-1}$ be integrable for $\mu_X \otimes \mu_Y$. Formula (23) results from an analogous argument.

#### Proposition 14 {#int-vii-s2-prop-14 .statement}

— Suppose that the conditions of Prop. 13 are fulfilled and that, in addition, Y is normal.

a) The restriction of $\mu_G$ to $\Omega$ is, up to a constant factor, the image of $\mu_X \otimes \mu_Y$ under the mapping $(x, y) \mapsto xy$ of $X \times Y$ onto $\Omega$.

b) For $x \in X$ and $y \in Y$,

$$
\Delta_G(xy) = \Delta_X(x)\Delta_Y(y) \operatorname{mod}(i_x),
$$

where $i_x$ denotes the automorphism $v \mapsto x^{-1}vx$ of Y.

We have $\Delta_G = \Delta_Y$ on Y (Prop. 10 b)), therefore a) follows from (23). Let $x_0 \in X,\ y_0 \in Y$. Denote by $p$ the mapping $(x, y) \mapsto xy$ of $X \times Y$ onto $\Omega$. Since

$$
xy(x_0y_0)^{-1} = xx_0^{-1}(x_0yy_0^{-1}x_0^{-1}) = xx_0^{-1}i_{x_0^{-1}}(yy_0^{-1}),
$$

we have

$$
\begin{align*}
\Delta_G(x_0y_0)p(\mu_X \otimes \mu_Y) &= \delta(x_0y_0)p(\mu_X \otimes \mu_Y) \\
&= p(\delta(x_0)\mu_X \otimes i_{x_0^{-1}}\delta(y_0)\mu_Y) \\
&= p(\Delta_X(x_0)\mu_X \otimes \Delta_Y(y_0)(\operatorname{mod}\ i_{x_0})\mu_Y) \\
&= \Delta_X(x_0)\Delta_Y(y_0)(\operatorname{mod}\ i_{x_0})p(\mu_X \otimes \mu_Y),
\end{align*}
$$

whence b).

#### Remark {#int-vii-s2-n9-rem-1 .statement}

Prop. 14 applies in particular when G is the topological semi-direct product of X by Y (GT, III, §2, No. 10). In this case, $Z = \{e\}$ and $\Omega = G$. Since $yx = xi_x(y)$ for $x \in X,\ y \in Y$, the measure $\mu_G$ is also, up to a constant factor, the image of $(\operatorname{mod}\ i_x)\mu_X \otimes \mu_Y$ under the mapping $(x, y) \mapsto yx$ of $X \times Y$ into G.

### 10. Integration on a fundamental domain

Let X be a locally compact space, H a discrete group operating on the right continuously and properly in X. Let $\pi$ be the canonical mapping of X onto $X/H$. For every $x \in X$, we denote by $H_x$ the stabilizer of $x$ in H; this is a finite subgroup of H (GT, III, §4, No. 2, Prop. 4); its order will be denoted $n(x)$. For every $s \in H,\ H_{xs} = s^{-1}H_x s$, therefore $n(xs) = n(x)$. There exists an open neighborhood U of x such that $U \cap Us = \varnothing$ for $s \notin H_x$ (loc. cit., No. 4, proof of Prop. 8); for $y \in U$, one has $H_y \subset H_x$; thus the function $n$ on X is upper semi-continuous. When X is countable at infinity, H is countable; for, let $(K_1, K_2, \ldots)$ be a covering of X by a sequence of compact subsets, and let $x_0 \in X$; the set of $s \in H$ such that $x_0 s \in K_i$ is finite (*loc. cit.*, No. 5, Th. 1), whence our assertion.

#### Definition 2 {#int-vii-s2-def-2 .statement}

*Let $F \subset X$. One says that $F$ is a fundamental domain (for $H$) if the restriction of $\pi$ to $F$ is a bijection of $F$ onto $X/H$* (in other words, $F$ is a *system of representatives* for the equivalence relation defined by $H$).

#### Lemma 8 {#int-vii-s2-lem-8 .statement}

— *Let $F$ be a fundamental domain. For every $x \in X$,*
$$
\sum_{s \in H} \varphi_{Fs}(x) = n(x).
$$
(24)

Since $\varphi_{Fs}(xt) = \varphi_{Fst^{-1}}(x)$ for all $s$ and $t$ in $H$, the two members of (24) remain invariant when $x$ is replaced by $xt$. We can therefore suppose that $x \in F$. We then have the equivalences
$$
\varphi_{Fs}(x) = 1 \iff x \in Fs \iff xs^{-1} \in F \iff xs^{-1} = x \iff s \in H_x,
$$
whence (24).

#### Proposition 15 {#int-vii-s2-prop-15 .statement}

*Assume that $X$ is countable at infinity. Let $\mu$ be a measure $\geq 0$ on $X$. Let $F$ be a fundamental domain such that $Fs$ is $\mu$-measurable for every $s \in H$. Let $f$ be a $\mu$-integrable function on $X$, with values in a Banach space or in $\overline{\mathbf{R}}$. Then the family of the*
$$
\int_{Fs} n(x)^{-1} f(x) d\mu(x) \qquad (s \in H)
$$
*is summable, and*
$$
\int_X f(x) d\mu(x) = \sum_{s \in H} \int_{Fs} n(x)^{-1} f(x) d\mu(x).
$$

If $A$ is a finite subset of $H$, then
$$
\left| \sum_{s \in A} n^{-1} f \varphi_{Fs} \right| \leq n^{-1} |f| \sum_{s \in A} \varphi_{Fs} \leq |f|
$$
by Lemma 8. Lemma 8 also proves that $\sum_{s \in A} n^{-1} f \varphi_{Fs}$ converges pointwise to $f$ with respect to the increasing directed set of finite subsets of $H$. Prop. 15 then follows from Ch. IV, §4, No. 3, Th. 2.

#### Theorem 4 {#int-vii-s2-thm-4 .statement}

*Let $X$ be a locally compact space countable at infinity, $H$ a discrete group operating continuously and properly on the right in $X$, π the canonical mapping of X onto X/H, μ a positive measure on X invariant under H, β the normalized Haar measure of H, and λ = μ/β. Let F be a μ-measurable fundamental domain.

a) The pair $(\pi, n^{-1}\varphi_F)$ is μ-adapted, and

$$
\int_X n(x)^{-1} \varphi_F(x) \varepsilon_{\pi(x)} \, d\mu(x) = \lambda.
$$

b) The mapping π is proper for $n^{-1}\varphi_F \cdot \mu$, and $\pi(n^{-1}\varphi_F \cdot \mu) = \lambda$.

c) Let k be a function on X/H. For k to be λ-measurable (resp. λ-integrable), it is necessary and sufficient that $n^{-1}\varphi_F(k \circ \pi)$ be μ-measurable (resp. μ-integrable); and, if k is λ-integrable then

$$
\int_{X/H} k \, d\lambda = \int_F n^{-1}(k \circ \pi) \, d\mu.
$$

We have $\mu = \lambda^\sharp$. Let $f \in \mathcal{H}_+(X/H)$. Then $n^{-1}\varphi_F(f \circ \pi)$ is μ-measurable and $\geq 0$, and by Prop. 5 b) of No. 3 we have

$$
\int_X^* n(x)^{-1} \varphi_F(x) f(\pi(x)) d\mu(x) = \int_{X/H}^* f(\dot{x}) d\lambda(\dot{x}) \int_H^* n(x\xi)^{-1} \varphi_F(x\xi) d\beta(\xi)
$$

and $\int_H^* n(x\xi)^{-1} \varphi_F(x\xi) d\beta(\xi) = n(x)^{-1} \sum_{\xi \in H} \varphi_F(x\xi) = 1$ by Lemma 8. Thus $n^{-1}\varphi_F \cdot (f \circ \pi)$ is μ-integrable and

$$
\int_X n(x)^{-1} \varphi_F(x) f(\pi(x)) d\mu(x) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}).
$$

This proves a). The assertion b) is proved similarly. The assertion c) may be deduced from a) and from Ch. V, §4, Prop. 3 and Th. 2.

#### Corollary {#int-vii-s2-n10-cor-1 .statement}

— We maintain the hypotheses and notations of Th. 4. Let F' be a second μ-measurable fundamental domain. Let u be a function on X, with values in a Banach space or in $\overline{\mathbf{R}}$, invariant under H. Suppose that u is μ-integrable on F. Then u is μ-integrable on F' and

$$
\int_F u(x) d\mu(x) = \int_{F'} u(x) d\mu(x).
$$

Since u and n are invariant under H, there exists a function v on X/H such that v o π coincides with nu on F and on F'. Then $n^{-1} \varphi_F(v \circ \pi) = \varphi_{F'} u, \quad n^{-1} \varphi_{F'}(v \circ \pi) = \varphi_{F'} u.$ By hypothesis, $n^{-1} \varphi_F(v \circ \pi)$ is $\mu$-integrable. By Th. 4, $v$ is $\lambda$-integrable, $\varphi_{F'} \mu$ is $\mu$-integrable, and

$$
\int_F u d\mu = \int_{X/H} v d\lambda = \int_{F'} u d\mu.
$$

For the existence of $\mu$-measurable fundamental domains, see Exer. 12.

### Exercises {#int-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
