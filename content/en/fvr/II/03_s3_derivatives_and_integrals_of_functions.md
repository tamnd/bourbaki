---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 3
section_title: DERIVATIVES AND INTEGRALS OF FUNCTIONS DEPENDING ON A PARAMETER
lang: en
source: fvr-i-vii
pdf_pages: 0083-0093, 0101-0105
extraction: ocr
subsections:
    - "no": 1
      title: INTEGRAL OF A LIMIT OF FUNCTIONS ON A COMPACT INTERVAL
      page: 0
      pdf_page: 83
    - "no": 2
      title: INTEGRAL OF A LIMIT OF FUNCTIONS ON A NON-COMPACT INTERVAL
      page: 0
      pdf_page: 84
    - "no": 3
      title: NORMALLY CONVERGENT INTEGRALS
      page: 0
      pdf_page: 87
    - "no": 4
      title: DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A COMPACT INTERVAL
      page: 0
      pdf_page: 88
    - "no": 5
      title: DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A NON-COMPACT INTERVAL
      page: 0
      pdf_page: 90
    - "no": 6
      title: CHANGE OF ORDER OF INTEGRATION
      page: 0
      pdf_page: 91
statements: 17
exercises: 10
content_sha256: 62bb6cd48dfc0b7f2b01d57475721e621137ba34388ad9ae689438f7ab394731
---

## § 3. DERIVATIVES AND INTEGRALS OF FUNCTIONS DEPENDING ON A PARAMETER

### 1. INTEGRAL OF A LIMIT OF FUNCTIONS ON A COMPACT INTERVAL

Th. 1 of II, p. 52, applied to the particular case of regulated functions on a compact interval, translates as follows into the notation appropriate to integrals:

#### Proposition 1 {#fvr-ii-s3-prop-1 .statement}

Let A be a set filtered by a filter $\mathfrak{F}$, and $(f_\alpha)_{\alpha \in A}$ a family of regulated functions on a compact interval $I = [a, b]$; if the functions $f_\alpha$ converge uniformly on I to a (regulated) function f with respect to the filter $\mathfrak{F}$, then

$$
\lim_{\mathfrak{F}} \int_a^b f_\alpha(t) \, dt = \int_a^b f(t) \, dt.
$$

Two corollaries to this proposition are important in applications:

#### Corollary 1 {#fvr-ii-s3-prop-1-cor-1 .statement}

Let $(f_n)$ be a sequence of regulated functions on a compact interval $I = [a, b]$. If the sequence $(f_n)$ converges uniformly on I to a (regulated) function f, one has

$$
\lim_{n \to \infty} \int_a^b f_n(t) \, dt = \int_a^b f(t) \, dt.
$$

In particular, if a series whose general term $u_n$ is a regulated function on I, converges uniformly to f on I, then the series with general term $\int_a^b u_n(t) \, dt$ is convergent and its sum is $\int_a^b f(t) \, dt$ ("term-by-term integration of a uniformly convergent series").

#### Corollary 2 {#fvr-ii-s3-prop-1-cor-2 .statement}

Let $A$ be a subset of a topological space $F$, and $f$ a map from $I \times A$ into a complete normed space $E$ over $\mathbf{R}$, such that, for each $\alpha \in A$, the function $x \mapsto f(x, \alpha)$ is regulated on $I$. If the functions $x \mapsto f(x, \alpha)$ converge uniformly on $I$ to a (regulated) function $x \mapsto g(x)$, as $\alpha$ tends to a point $\alpha_0 \in \overline{A}$ while remaining in $A$, then one has

$$
\lim_{\alpha \to \alpha_0,\ \alpha \in A} \int_a^b f(x, \alpha)\, dx = \int_a^b g(x)\, dx.
$$

In particular:

#### Proposition 2 ("continuity of an integral with respect to a parameter") {#fvr-ii-s3-prop-2 .statement}

Let $F$ be a compact space, let $I = [a,\ b]$ be a compact interval in $\mathbf{R}$, and let $f$ be a continuous map of $I \times F$ into a complete normed space $E$ over $\mathbf{R}$; then the function $h(\alpha) = \int_a^b f(x, \alpha)\, dx$ is continuous on $F$.

Indeed, since $f$ is uniformly continuous on the compact space $I \times F$, the functions $f(x, \alpha)$ converge uniformly to $f(x, \alpha_0)$ on $I$, when $\alpha$ tends to an arbitrary point $\alpha_0 \in F$.

Here is an application of this proposition: the function $(x, \alpha) \mapsto x^\alpha$ is continuous on the product $I \times J$, where $I = [a,\ b]$ is a compact interval such that $0 < a < b$, and $J$ is any compact interval in $\mathbf{R}$; one concludes that $\int_a^b x^\alpha\, dx$ is a continuous function of $\alpha$ on $\mathbf{R}$; now, for $\alpha$ rational and $\neq -1$, this function is equal to $\frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$, and the function $\alpha \mapsto \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ is continuous on every interval of $\mathbf{R}$ not containing $-1$; one thus has (extension of identities) $\int_a^b x^\alpha\, dx = \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ for all real $\alpha \neq -1$; this again means that, for all real $\alpha$, the derivative of $x^\alpha$ is $\alpha x^{\alpha-1}$ (cf. III, p. 94).

### 2. INTEGRAL OF A LIMIT OF FUNCTIONS ON A NON-COMPACT INTERVAL

Th. 1 of II, p. 52 applies to functions more general than regulated functions, since there one merely assumes that the functions admit primitives. In particular one sees that prop. 1 of II, p. 68 still applies when, on an interval $I \subset \mathbf{R}$, the functions $f_\alpha$ are only assumed to be *piecewise regulated* and to admit an *integral* over $I$; however this result presupposes that the other two hypotheses of prop. 1 are satisfied, namely:
1. $I$ is a *bounded* interval; 2' the $f_\alpha$ converge *uniformly on* $I$ to $f$. Formula (1) of II, p. 68 *may fail* when one of these conditions is no longer satisfied: it can happen that one or the other of these two terms does not exist, or that both exist but have different values.

For example, if $f_n$ is the regulated function on $]0,\ 1[$, defined by $f_n(x) = n$ for $0 < x < 1/n$ and $f_n(x) = 0$ for $1/n \leq x \leq 1$, then the sequence $(f_n)$ converges to 0 uniformly on every compact interval contained in ]0, 1[, but not uniformly on [0, 1], and one has $\int_0^1 f_n(t) \, dt = 1$ for each $n$. One has an example where $\int_0^1 f_n(t) \, dt$ does not tend to any limit on replacing the preceding sequence $(f_n)$ by the sequence $((-1)^n f_n)$ which again converges uniformly to 0 on every compact interval contained in ]0, 1].

On the other hand, on the *unbounded* interval $I = [0, +\infty[$, let $f_n$ be the regulated function such that $f_n(x) = 1/n$ for $n^2 \leq x \leq (n+1)^2$ and $f_n(x) = 0$ for every other value of $x$ in $I$ ($n \geq 1$); the sequence $(f_n)$ converges uniformly to 0 on $I$, but the integral $\int_0^{+\infty} f_n(t) \, dt = (2n+1)/n$ tends to 2 as $n$ increases indefinitely.

In other words, when $I$ is not bounded, if one denotes by $\mathcal{I}$ the vector space formed by the regulated functions $\mathbf{f}$ on $I$, with values in $E$, and admitting an integral over $I$, then the map $\mathbf{f} \mapsto \int_I \mathbf{f}(t) \, dt$ *is not continuous* when one endows $\mathcal{I}$ with the topology of uniform convergence on $I$ (*cf.* II, p. 53, cor. 2)

We shall seek *sufficient* conditions to assure the validity of prop. 1, under the following hypotheses:

1. $I$ is an arbitrary interval in $\mathbf{R}$, the function $\mathbf{f}_\alpha$ is regulated on $I$, and admits an integral over $I$;
2. the family $(\mathbf{f}_\alpha)$ converges uniformly to $\mathbf{f}$ with respect to the filter $\mathfrak{F}$ on every compact interval contained in $I$.

Writing $\mathfrak{K}(I)$ for the directed set of compact intervals contained in $I$ (II, p. 64), the left-hand side of formula (1) of II, p. 68 can be written as $\lim_{\delta} \left( \lim_{J \in \mathfrak{K}(I)} \int_J \mathbf{f}_\alpha(t) \, dt \right)$; on the other hand, taking account of prop. 1 (II. p. 68), and also the fact that the family $(\mathbf{f}_\alpha)$ is uniformly convergent on every compact interval $J \subset I$, the right-hand side of (1) (II, p. 68) can be written as $\lim_{J \in \mathfrak{K}(I)} \left( \lim_{\delta} \int_J \mathbf{f}_\alpha(t) \, dt \right)$. One thus sees that prop. 1 of II, p. 19 extends when one can *interchange the limits* of the map$(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ with respect to the filter $\mathfrak{F}$ and with respect to the filter $\Phi$ of sections of the directed set $\mathfrak{K}(I)$. Now, we know a *sufficient* condition for this interchange to be justified, namely the existence of the limit of the map $(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ with respect to the *product filter* $\Phi \times \mathfrak{F}$ (*Gen. Top.*, I, p. 81, cor. to th. 1). We shall transform this condition into an equivalent, more manageable, condition.

In the first place, since $E$ is complete, in order that $(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ should have a limit with respect to $\Phi \times \mathfrak{F}$ it is necessary and sufficient that, for every $\varepsilon > 0$, there should exist a compact interval $J_0 \subset I$ and a set $M \in \mathfrak{F}$ such that, for any elements $\alpha, \beta$ of $M$ and compact interval $J \supset J_0$ contained in $I$, one has

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t) \, dt - \int_J \mathbf{f}_\beta(t) \, dt \right| \leq \varepsilon.
$$

We shall show on the other hand that this condition is itself equivalent to the following condition: for every $\varepsilon > 0$ there exists a compact interval $J_0 \subset I$ and a set $M \in \mathfrak{F}$ such that, for any $\alpha$ of $M$ and any compact interval $J \supset J_0$ contained in $I$, one has

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t) \, dt - \int_J \mathbf{f}_\alpha(t) \, dt \right| \leq \varepsilon.
$$

It is indeed clear that this last condition is necessary; conversely, if it is satisfied, there exists (by the uniform convergence of $(\mathbf{f}_\alpha )$ on every compact interval) a set $N \in \mathfrak{F}$ such that, for any $\alpha,\ \beta$ in $N$ one has

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t)\,dt - \int_{J_0} \mathbf{f}_\beta(t)\,dt \right| \leq \varepsilon;
$$

and therefore $\left| \int_{J_0} \mathbf{f}_\alpha(t)\,dt - \int_J \mathbf{f}_\beta(t)\,dt \right| \leq 2\varepsilon$ for any $\alpha$ and $\beta$ in $M \cap N \in \mathfrak{F}$ and for any compact interval $J \supset J_0$.

Finally, the lemma of II, p. 65 allows us to put this last condition in the following equivalent form: *for every $\varepsilon > 0$ there exist a compact interval $J_0 \subset I$ and a set $M \in \mathfrak{F}$ (depending on $\varepsilon$) such that, for every compact interval $K \subset I$ having no interior point in common with $J_0$, and every $\alpha \in M$, one has* $\left| \int_K \mathbf{f}_\alpha(t)\,dt \right| \leq \varepsilon$.

Most often, one uses a more restrictive condition obtained by supposing that, in the last statement, the set $M$ *does not depend on $\varepsilon$*:

#### Definition 1 {#fvr-ii-s3-def-1 .statement}

*One says that the integral $\int_I \mathbf{f}_\alpha(t)\,dt$ is uniformly convergent for $\alpha \in A$ (or uniformly convergent over $A$) if, for every $\varepsilon > 0$ there exists a compact interval $J_0 \subset J$ such that, for every compact interval $K \subset I$ with no interior point in common with $J_0$, and every $\alpha \in A$, one has*

$$
\left| \int_K \mathbf{f}_\alpha(t)\,dt \right| \leq \varepsilon.
$$

This definition is equivalent to saying that the family of maps $\alpha \mapsto \int_I \mathbf{f}_\alpha(t)\,dt$ is *uniformly convergent on $A$* (towards the map $\alpha \mapsto \int_I \mathbf{f}_\alpha(t)\,dt$) with respect to the filter of sections $\Phi$ of $\mathcal{K}(I)$; each of the integrals $\int_I \mathbf{f}_\alpha(t)\,dt$ is *a fortiori* convergent (the converse being false). Further, from what we have just seen (or from *Gen. Top.*, X, p. 281, cor. 2):

#### Proposition 3 {#fvr-ii-s3-prop-3 .statement}

*Let* $(\mathbf{f}_\alpha )$ *be a family of regulated functions on an interval* $I$ *such that: 1* with respect to the filter $\mathfrak{F}$ *the family* $(\mathbf{f}_\alpha )$ *converges uniformly to a function* $f$ *(regulated on* $I$) *on every compact interval contained in* $I$; *2* the integral $\int_I \mathbf{f}_\alpha(t)\,dt$ *is uniformly convergent for every* $\alpha \in A$. *Under these hypotheses the integral* $\int_I f(t)\,dt$ *is convergent, and one has*

$$
\lim_{\mathfrak{F}} \int_I \mathbf{f}_\alpha(t)\,dt = \int_I f(t)\,dt.
$$

The hypotheses of prop. 3 are fulfilled when for example $I$ is a *bounded* interval, the $\mathbf{f}_\alpha$ are *uniformly bounded* on $I$, and converge uniformly to $f$ on every compact interval contained in $I$; indeed, if $\| \mathbf{f}_\alpha(x) \| \leq h$ for all $x \in I$ and all $\alpha$, and if $J_0$ is such that the difference between the lengths of $I$ and $J_0$ is $\leq \varepsilon / h$, then condition (7) is satisfied for every interval $K \subset I$ with no interior point in common with $J_0$.

As with prop. 1 of II, p. 68, two corollaries to prop. 3 are important in applications:

#### Corollary 1 {#fvr-ii-s3-prop-3-cor-1 .statement}

*Let* $(f_n)$ *be a sequence of regulated functions on an arbitrary interval* $I$, *converging uniformly to a function* $f$ *on each compact interval contained in* $I$; *if the integral* $\int_I f_n(t)\,dt$ *is uniformly convergent, then the integral* $\int_I f(t)\,dt$ *is convergent, and*
$$
\lim_{n \to \infty} \int_I f_n(t)\,dt = \int_I f(t)\,dt.
$$
(9)

#### Remark {#fvr-ii-s3-n2-rem-1 .statement}

The hypotheses imposed in this corollary are sufficient, but not necessary, for the validity of formula (9); we shall generalize this formula later, at the same time as the concept of integral (see INT, IV), and obtain much less restrictive conditions.

#### Corollary 2 {#fvr-ii-s3-prop-3-cor-2 .statement}

*Let* $A$ *be a subset of a topological space* $F$, *and* $f$ *a map of* $I \times A$ *into a complete normed space* $E$ *over* $\mathbf{R}$, *such that, for every* $\alpha \in A$, *the function* $x \mapsto f(x, \alpha)$ *is regulated on* $I$. *If, on the one hand, the functions* $x \mapsto f(x, \alpha)$ *converge uniformly on every compact interval contained in* $I$ *to a function* $x \mapsto f(x)$ *as* $\alpha$ *tends to* $\alpha_0 \in \overline{A}$ *while remaining in* $A$; *if, on the other hand, the integral* $\int_I f(x, \alpha)\,dx$ *is uniformly convergent on* $A$, *then the integral* $\int_I f(x)\,dx$ *is convergent, and one has*
$$
\lim_{\alpha \to \alpha_0,\ \alpha \in A} \int_I f(x, \alpha)\,dx = \int_I f(x)\,dx.
$$
(10)

In particular:

#### Proposition 4 ("continuity of an improper integral with respect to a parameter") {#fvr-ii-s3-prop-4 .statement}

*Let* $F$ *be a compact space, let* $I$ *be any interval in* $\mathbf{R}$, *and* $f$ *a continuous map from* $I \times F$ *into a complete normed space* $E$ *over* $\mathbf{R}$; *if the integral* $h(\alpha) = \int_I f(x, \alpha)\,dx$ *is uniformly convergent on* $F$, *it is a continuous function of* $\alpha$ *on* $F$.

In view of prop. 2 of II, p. 69, this proposition also follows from the continuity of a uniform limit of continuous functions (*Gen. Top.*, X, p. 282, th. 2).

### 3. NORMALLY CONVERGENT INTEGRALS

Let $(f_\alpha)_{\alpha \in A}$ be a family of regulated functions on an arbitrary interval $I \subset \mathbf{R}$, with values in a complete normed space $E$ over $\mathbf{R}$. Suppose that there exists a finite real regulated function $g$ on $I$ such that, for every $x \in I$ and every $\alpha \in A$, $\|f_\alpha(x)\| \leq g(x)$ and also the integral $\int_I g(t)\,dt$ is convergent. Under these conditions the integral $\int_I f_\alpha(t)\,dt$ is *absolutely and uniformly convergent* on $A$; in fact, for every compact interval $K$ contained in $I$,
$$
\left\| \int_K f_\alpha(t)\,dt \right\| \leq \int_K g(t)\,dt
$$

and the convergence of the integral $\int_I g(t) \, dt$ implies that for every $\varepsilon > 0$ there exists a compact interval $J \subset I$ such that for every compact interval $K \subset I$ disjoint from $J$ one has $\int_K g(t) \, dt \leq \varepsilon$. When there exists a real function $g$ having the preceding properties one says that the integral $\int_I f_\alpha(t) \, dt$ is normally convergent on $A$ (cf. Gen. Top., X, p. 296).

An integral can be uniformly convergent on $A$ without being normally convergent. *This happens for the sequence $(f_n)$ of real functions defined by the conditions $f_n(x) = 1/x$ for $n \leq x \leq n+1$, and $f_n(x) = 0$ for the other values of $x$ in $I = [0, +\infty[$. It is immediate that the integral $\int_1^\infty f_n(t) \, dt$ is uniformly convergent, but not normally convergent, since the relation $g(x) \geq f_n(x)$ for each $x \in I$ and all $n$ entails that $g(x) \geq 1/x$, and consequently that the integral of $g$ over $I$ is not convergent..

In particular, let us consider a series whose general term $u_n$ is a regulated function on an interval $I$, and suppose that the series with general term $\|u_n(x)\|$ (which is a regulated function on $I$) converges uniformly on every compact interval contained in $I$, and such that the series with general term $\int_I \|u_n(t)\| \, dt$ is convergent; then (II, p. 66, prop. 2) the (regulated) function $g(x)$, the sum of the series with general term $\|u_n(x)\|$, is such that the integral $\int_I g(t) \, dt$ is convergent. If one puts $f_n = \sum_{p=1}^n u_p$, then the integral $\int_I f_n(t) \, dt$ is normally convergent, for one has

$$
\|f_n(x)\| \leq \sum_{p=1}^n \|u_p(x)\| \leq g(x)
$$

for all $x \in I$ and all $n$; in consequence, the sum $f$ of the series with general term $u_n$ is a regulated function on $I$ such that the integral $\int_I f(t) \, dt$ is convergent, and one has

$$
\int_I f(t) \, dt = \sum_{n=1}^\infty \int_I u_n(t) \, dt
$$

("term-by-term integration of a series on a non-compact interval").

### 4. DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A COMPACT INTERVAL

Let $A$ be a compact neighbourhood of a point $\alpha_0$ in the field $\mathbf{R}$ (resp. the field $\mathbf{C}$), let $I = [a, b]$ be a compact interval in $\mathbf{R}$, and $f$ a continuous map of $I \times A$ into a complete normed space $E$ over $\mathbf{R}$ (resp. $\mathbf{C}$). We have seen (II, p. 69, prop. 2) that under these conditions $g(\alpha) = \int_a^b f(t, \alpha) \, dt$ is a continuous function on $A$. Let us seek sufficient conditions for $g$ to admit a derivative at the point $\alpha_0$. One has, for $\alpha \neq \alpha_0$,

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_a^b \frac{f(t, \alpha) - f(t, \alpha_0)}{\alpha - \alpha_0} \, dt
$$

so (II, p. 69, cor. 2), if the functions $x \mapsto \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ converge uniformly on I to a (necessarily continuous) function $x \mapsto \mathbf{h}(x)$ as $\alpha$ tends to $\alpha_0$ (while remaining $\neq \alpha_0$), then $g$ admits a derivative equal to $\int_a^b \mathbf{h}(t)\,dt$ at the point $\alpha_0$; moreover, for each $x \in I$, $\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ tends to $\mathbf{h}(x)$, so $\mathbf{h}(x)$ is the derivative at the point $\alpha_0$ of the map $\alpha \mapsto \mathbf{f}(x, \alpha)$; we denote this derivative (called the *partial derivative of* $\mathbf{f}$ *with respect to* $\alpha$) by the notation $\mathbf{f}'_{\alpha}(x, \alpha_0)$; the hypotheses we have made imply that

$$
g'(\alpha_0) = \int_a^b \mathbf{f}'_{\alpha}(t, \alpha_0)\,dt.
$$

(12)

The following proposition gives a very simple sufficient condition for the validity of formula (12):

#### Proposition 5 {#fvr-ii-s3-prop-5 .statement}

*Suppose that the partial derivative* $\mathbf{f}'_{\alpha}(x, \alpha)$ *exists for all* $x \in I$ *and all* $\alpha$ *in an open neighbourhood* $V$ *of* $\alpha_0$, *and that, for all* $\alpha \in V$, *the map* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ *is regulated on* $I$. *Under these conditions, if* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ *converges uniformly on* $I$ *to* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha_0)$ *as* $\alpha$ *tends to* $\alpha_0$, *then the function* $g(\alpha) = \int_a^b \mathbf{f}(t, \alpha)\,dt$ *admits a derivative, given by the formula* (12), *at the point* $\alpha_0$.

Indeed, for every $\varepsilon > 0$ there exists by hypothesis an $r > 0$ such that $|\alpha - \alpha_0| \leq r$ implies $\| \mathbf{f}'_{\alpha}(x, \alpha) - \mathbf{f}'_{\alpha}(x, \alpha_0) \| \leq \varepsilon$ *for any* $x \in I$. By props. 3 and 5 of I, p. 17 one has, for $|\alpha - \alpha_0| \leq r$ ($\alpha \neq \alpha_0$) and for all $x \in I$

$$
\left\| \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0} - \mathbf{f}'_{\alpha}(x, \alpha_0) \right\| \leq \varepsilon
$$

which proves the uniform convergence of $\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ to $\mathbf{f}'_{\alpha}(x, \alpha_0)$ on I as $\alpha$ tends to $\alpha_0$ (remaining $\neq \alpha_0$), and so establishes formula (12).

#### Corollary {#fvr-ii-s3-n4-cor-1 .statement}

*If the partial derivative* $\mathbf{f}'_{\alpha}(x, \alpha)$ *exists on* $I \times V$ *and is a continuous function of* $(x, \alpha)$ *on this set, then the function* $g$ *admits a derivative given by the formula* (12) *at the point* $\alpha_0$.

Indeed, if W is a compact neighbourhood of $\alpha_0$ contained in V, then the map $(x, \alpha) \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ is *uniformly continuous* on the compact set $I \times W$, so $\mathbf{f}'_{\alpha}(x, \alpha)$ tends to $\mathbf{f}'_{\alpha}(x, \alpha_0)$ uniformly on I as $\alpha$ tends to $\alpha_0$.

From prop. 5 one deduces a more general proposition which allows one to evaluate the derivative of an integral when, not only the integrand $\mathbf{f}$, but also the limits of integration, depend on a parameter $\alpha$:

#### Proposition 6 {#fvr-ii-s3-prop-6 .statement}

*Supposing that the hypotheses of prop. 5 are satisfied, let* $a(\alpha)$, $b(\alpha)$ *be two functions defined on* $V$, *with values in* $I$; *if the derivatives* $a'(\alpha_0),\ b'(\alpha_0)$ exist and are finite then the function $g(\alpha) = \int_{a(\alpha)}^{b(\alpha)} f(t, \alpha)\, dt$ admits at $\alpha_0$ a derivative given by the formula

$$
g'(\alpha_0) = \int_{a(\alpha_0)}^{b(\alpha_0)} f'_\alpha(t, \alpha_0)\, dt + b'(\alpha_0)f(b(\alpha_0), \alpha_0) - a'(\alpha_0)f(a(\alpha_0), \alpha_0).
$$

Indeed, for all $\alpha \in V$ distinct from $\alpha_0$ one can write

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_{a(\alpha_0)}^{b(\alpha_0)} \frac{f(t, \alpha) - f(t, \alpha_0)}{\alpha - \alpha_0}\, dt + \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt
$$
$$
- \frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} f(t, \alpha)\, dt.
$$

By prop. 5 of II, p. 74, the first integral on the right-hand side tends to $\int_{a(\alpha_0)}^{b(\alpha_0)} f'_\alpha(t, \alpha_0)\, dt$ as $\alpha$ tends to $\alpha_0$. In the second integral we replace $f(t, \alpha)$ by $f(b(\alpha_0), \alpha_0)$ and show that the difference tends to 0. We put $M = \max (\|f(b(\alpha_0), \alpha_0)\|, |b'(\alpha_0)| + 1)$; the function $b(\alpha)$ being continuous at the point $\alpha_0$ and the function $f$ continuous at the point $(b(\alpha_0), \alpha_0)$, for every $\varepsilon$ such that $0 < \varepsilon < 1$ there exists an $r > 0$ such that the relation $|\alpha - \alpha_0| \leq r$ entails that $\|f(t, \alpha) - f(b(\alpha_0), \alpha_0)\| \leq \varepsilon$ for all $t$ belonging to the interval with endpoints $b(\alpha_0)$ and $b(\alpha)$; thus one may also suppose that the relation $|\alpha - \alpha_0| \leq r$ entails $\left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} - b'(\alpha_0) \right| \leq \varepsilon$.

By the mean value formula (II, p 62, formula (17)) one thus has

$$
\left| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt - \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} f(b(\alpha_0), \alpha_0) \right| \leq \left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} \right| \varepsilon
$$

and consequently

$$
\left| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt - b'(\alpha_0) f(b(\alpha_0), \alpha_0) \right| \leq 2M \varepsilon
$$

which shows that $\frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt$ tends to $b'(\alpha_0) f(b(\alpha_0), \alpha_0)$. In the same way one shows that $\frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} f(t, \alpha)\, dt$ tends to $a'(\alpha_0) f(a(\alpha_0), \alpha_0)$.

### 5. DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A NON-COMPACT INTERVAL

The set $V$ having the same meaning as in prop. 5 of II, p. 74, suppose now that I is *any* interval in $\mathbf{R}$, and that $f$ is a *continuous* map from $I \times V$ into E; if the integral $g(\alpha) = \int_I f(t, \alpha)\, dt$ exists for all $\alpha \in V$ and is a continuous function of $\alpha$, the function $g$ *need not have a derivative equal to* $\int_I f'_\alpha(t, \alpha_0)\, dt$ *at the point* $\alpha_0$, even if $f'_\alpha(x, \alpha)$ converges uniformly to $f'_\alpha(x, \alpha_0)$ on every compact interval contained in I, and if the integral $\int_I f'_\alpha(t, \alpha) \, dt$ exists for all $\alpha \in V$ (cf. II, p. 87, exerc. 3).

A sufficient condition for formula (12) (II, p. 74) to remain valid is given by the following proposition:

#### Proposition 7 {#fvr-ii-s3-prop-7 .statement}

Let I be an arbitrary interval in $\mathbf{R}$, and $f$ a continuous function on $I \times V$. Suppose that:
1. the partial derivative $f'_\alpha(x, \alpha)$ exists for all $x \in I$ and all $\alpha \in V$, and, for all $\alpha \in V$, the map $x \mapsto f'_\alpha(x, \alpha)$ is regulated on I;
2. for all $\alpha \in V$, $f'_\alpha(x, \beta)$ converges uniformly to $f'_\alpha(x, \alpha)$ on every compact interval contained in I, as $\beta$ tends to $\alpha$;
3. the integral $\int_I f'_\alpha(t, \alpha) \, dt$ is uniformly convergent on $V$;
4. the integral $\int_I f(t, \alpha_0) \, dt$ is convergent.

In these circumstances the integral $g(\alpha) = \int_I f(t, \alpha) \, dt$ is uniformly convergent on $V$, and the function $g$ admits at every point of $V$ a derivative given by the formula

$$
g'(\alpha) = \int_I f'_\alpha(t, \alpha) \, dt.
$$

The uniform convergence of $\int_I f'_\alpha(t, \alpha) \, dt$ on $V$ means that the function $\alpha \mapsto \int_J f'_\alpha(t, \alpha) \, dt$ converges uniformly on $V$ with respect to the filter of sections $\Phi$ of the directed set $\mathfrak{K}(I)$ of compact intervals $J$ contained in I. Let us put $u_J(\alpha) = \int_J f(t, \alpha) \, dt$; the hypotheses show that on the one hand $u_J(\alpha_0)$ has a limit with respect to $\Phi$, and on the other hand, by virtue of prop. 5 of II, p. 74, that $u'_J(\alpha) = \int_J f'_\alpha(t, \alpha) \, dt$ for all $\alpha \in V$. We can therefore apply th. 1 of II, p. 52 to the functions $u_J$, the rôle of the set of indices being taken here by $\mathfrak{K}(I)$, and that of the filter on this set by the filter $\Phi$; the proposition follows immediately.

#### Remark 1 {#fvr-ii-s3-n5-rem-1 .statement}

Conditions 1 and 2 of prop. 7 are satisfied a fortiori when $f'_\alpha(x, \alpha)$ is a continuous function of $(x, \alpha)$ on $I \times V$.
2) When, in an integral $\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt$, the endpoints of the interval are finite functions of the parameter, the study of this integral as a function of $\alpha$ can be related to that of an integral over $[0, 1]$; indeed, by the change of variable $t = a(\alpha)(1 - u) + b(\alpha)u$, one has

$$
\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt = \int_0^1 f(a(\alpha)(1 - u) + b(\alpha)u, \alpha) (b(\alpha) - a(\alpha)) \, du.
$$

### 6. CHANGE OF ORDER OF INTEGRATION

Let $I = [a, b]$ and $A = [c, d]$ be two compact intervals in $\mathbf{R}$; let $f$ be a continuous function on $I \times A$ with values in a complete normed space E over $\mathbf{R}$; by prop. 2 of II, p. 69, $\int_a^b f(x, \alpha) \, dx$ is a continuous function of $\alpha$ on $A$; its integral $\int_c^d \left( \int_a^b f(x, \alpha) \, dx \right) d\alpha$ is also denoted, for simplicity, by $\int_c^d d\alpha \int_a^b f(x, \alpha) \, dx$.

#### Proposition 8 {#fvr-ii-s3-prop-8 .statement}

*If f is continuous on I × A one has*

$$
\int_c^d d\alpha \int_a^b f(x, \alpha) dx = \int_a^b dx \int_c^d f(x, \alpha) d\alpha
$$

("formula for interchanging the order of integration").

We shall show that, for all $y \in A$, one has

$$
\int_c^y d\alpha \int_a^b f(x, \alpha) dx = \int_a^b dx \int_c^y f(x, \alpha) d\alpha.
$$

Since the two sides of (16) are functions of $y$, and equal for $y = c$, it will suffice to prove that they are differentiable on $]c, d[$ and that their derivatives are equal at every point of this interval. If one puts $g(\alpha) = \int_a^b f(x, \alpha) dx$, and $h(x, y) = \int_c^y f(x, \alpha) dx$, the relation (16) can be written

$$
\int_c^y g(\alpha) d\alpha = \int_a^b h(x, y) dx.
$$

Now, the derivative of the first term with respect to $y$ is $g(y)$, while that of the second is $\int_a^b h_y'(x, y) dx$, by II, p. 74, corollary, since $h_y'(x, y) = f(x, y)$ is continuous on $I \times A$; the two expressions thus obtained are identical.

Suppose now that $A = [c, d]$ is a *compact* interval in $\mathbf{R}$, and I an *arbitrary* interval in $\mathbf{R}$; let $f$ be a continuous function on $I \times A$, with values in E, such that the integral $g(\alpha) = \int_I f(t, \alpha) dt$ is convergent for all $\alpha \in A$; even if $g(\alpha)$ is continuous on $A$ one cannot always interchange the order of integration in the integral $\int_c^d d\alpha \int_I f(t, \alpha) dt$, for the integral $\int_I dt \int_c^d f(t, \alpha) d\alpha$ may not exist, or it may be different from the integral $\int_c^d d\alpha \int_I f(t, \alpha) dt$ (*cf.* II, p. 87, exerc. 7). One has, however, the following result:

#### Proposition 9 {#fvr-ii-s3-prop-9 .statement}

*If the function f is continuous on I × A, and if the integral $\int_I f(t, \alpha) dt$ is uniformly convergent on A, then the integral $\int_I dt \int_c^d f(t, \alpha) d\alpha$ is convergent, and one has*

$$
\int_c^d d\alpha \int_I f(t, \alpha) dt = \int_I dt \int_c^d f(t, \alpha) d\alpha.
$$

For every compact interval J contained in I, put $u_J(\alpha) = \int_J f(t, \alpha) dt$. The hypothesis entails that with respect to the filter of sections $\Phi$ of the directed set $\mathcal{K}(I)$ the continuous function $u_J$ converges uniformly on A to $\int_I f(t, \alpha) dt$; thus (II, p. 68, prop. 1), $\int_c^d d\alpha \int_J f(t, \alpha) dt$ has limit $\int_c^d d\alpha \int_I f(t, \alpha) dt$ with respect to $\Phi$; but, by prop. 8 (II, p. 77), one has

$$
\int_c^d d\alpha \int_J f(t, \alpha) dt = \int_J dt \int_c^d f(t, \alpha) d\alpha.
$$

The preceding result thus means that the integral $\int_1 dt \int_c^{d} f(t, \alpha) d\alpha$ is convergent, and on passing to the limit with respect to $\Phi$ in the relation (18), one obtains (17).

### Exercises {#fvr-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
