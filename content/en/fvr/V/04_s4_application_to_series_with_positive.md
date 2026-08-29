---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 4
section_title: APPLICATION TO SERIES WITH POSITIVE TERMS
lang: en
source: fvr-i-vii
book_pages: 236-246, 261-263
pdf_pages: 0251-0261, 0276-0278
extraction: ocr
subsections:
    - "no": 1
      title: CONVERGENCE CRITERIA FOR SERIES WITH POSITIVE TERMS
      page: 236
      pdf_page: 251
    - "no": 2
      title: ASYMPTOTIC EXPANSION OF THE PARTIAL SUMS OF A SERIES
      page: 238
      pdf_page: 253
    - "no": 3
      title: ASYMPTOTIC EXPANSION OF THE PARTIAL PRODUCTS OF AN INFINITE PRODUCT
      page: 243
      pdf_page: 258
    - "no": 4
      title: 'APPLICATION: CONVERGENCE CRITERIA OF THE SECOND KIND FOR SERIES WITH POSITIVE TERMS'
      page: 244
      pdf_page: 259
statements: 13
exercises: 3
content_sha256: 5de68e31a6f00483c82e1c1ae6441d8b63cc5a1acbdf825ba174f4e30753e569
---

## § 4. APPLICATION TO SERIES WITH POSITIVE TERMS

### 1. CONVERGENCE CRITERIA FOR SERIES WITH POSITIVE TERMS

In this section by a *series with positive terms* we shall understand (by an abuse of language) a series $(u_n)$ of real terms such that $u_n \geq 0$ *starting from some particular* value of n. Everything we shall say about such series will extend immediately by a change of sign to series all of whose terms are $\leq 0$ starting from some particular value of n. We have seen (II, p. 64, Example 3) that to every sequence $(\mathbf{u}_n)_{n \geq 1}$ of points in a normed space E one can associate a step function $\mathbf{u}$ defined on $[1, +\infty[$ by the conditions $\mathbf{u}(x) = \mathbf{u}_n$ for $n \leq x < n+1$: then the series $(\mathbf{u}_n)$ converges if and only if the integral $\int_1^{+\infty} \mathbf{u}(t)\,dt$ converges.

Let $(u_n)$ and $(v_n)$ be two series with positive terms, and $u$ and $v$ the associated step functions: the relation $u_n \leq v_n$ for $n \geq n_0$ is equivalent to $u(x) \leq v(x)$ for $x \geq n_0$. Thus each of the relations $u_n \preccurlyeq v_n, u_n \ll v_n, u_n \sim v_n$ is equivalent to $u(x) \preccurlyeq v(x), u(x) \ll v(x)$ and $u(x) \sim v(x)$ respectively; this remark allows us to translate propositions 1 (V, p. 228) and 6 (V, p. 230) as follows:

#### Proposition 1 {#fvr-v-s4-prop-1 .statement}

*Let* $(u_n)$ *and* $(v_n)$ *be two series with positive terms. If* $u_n \preccurlyeq v_n$ *and if the series* $(v_n)$ *converges, then* $(u_n)$ *converges; if* $u_n \succ v_n$ *and if* $\sum_{n=1}^{\infty} v_n = +\infty$, *then* $\sum_{n=1}^{\infty} u_n = +\infty$.

#### Proposition 2 {#fvr-v-s4-prop-2 .statement}

*Let* $(u_n)$ *and* $(v_n)$ *be two series with positive terms*:
1. *If the series* $(v_n)$ *converges then the relation* $u_n \ll v_n$ *(resp.* $u_n \sim v_n$) *implies* $\sum_{p=n}^{\infty} u_p \ll \sum_{p=n}^{\infty} v_p$ *(resp.* $\sum_{p=n}^{\infty} u_p \sim \sum_{p=n}^{\infty} v_p$).
2. *If* $\sum_{n=1}^{\infty} v_n = +\infty$ *then the relation* $u_n \ll v_n$ *(resp.* $u_n \sim v_n$) *implies* $\sum_{p=1}^{n} u_p \ll \sum_{p=1}^{n} v_p$ *(resp.* $\sum_{p=1}^{n} u_p \sim \sum_{p=1}^{n} v_p$).

One obtains convenient convergence criteria by taking for the comparison series $(v_n)$ in prop. 1 a series whose terms are of the form $v_n = f(n)$, where $f$ is a function $\geq 0$ defined for every real number $x > x_0$ and decreasing on the interval $[x_0, +\infty[$; indeed:

#### Proposition 3 (Cauchy-Maclaurin criterion) {#fvr-v-s4-prop-3 .statement}

*If* $f$ *is a function* $\geq 0$ *and decreasing on* $[x_0, +\infty[$, *then the series with general term* $v_n = f(n)$ *converges if and only if the integral* $\int_{x_0}^{+\infty} f(t)\,dt$ *converges*.

To prove this it is sufficient to note that if $v$ is the step function associated with the series $(v_n)$ then $v(x+1) \leq f(x) \leq v(x)$ for every $x \geq x_0$ since $f$ is decreasing; the proposition is thus a consequence of the comparison principle (II, p. 66, prop. 3).

Since the functions which feature in the logarithmic convergence criteria for integrals (V, p. 229, prop. 2, 3 and 4) are decreasing on an interval $[x_0, +\infty[$, applying prop. 1 and 3 of V, p. 237, gives the following criteria:

#### Proposition 4 ("logarithmic criterion of order 0") {#fvr-v-s4-prop-4 .statement}

Let $(u_n)$ be a series with positive terms; if $u_n \preccurlyeq n^\mu$ for some $\mu < -1$ then the series $(u_n)$ converges; if $u_n \succcurlyeq n^\mu$ for some $\mu \geq -1$ then the series $(u_n)$ has an infinite sum.

#### Proposition 5 ("logarithmic criterion of order $p$") {#fvr-v-s4-prop-5 .statement}

Let $(u_n)$ be a series with positive terms. If $u_n \preccurlyeq \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)(l_p(n))^\mu}$ for some $\mu > 1$ then the series $(u_n)$ converges; if $u_n \succcurlyeq \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)(l_p(n))^\mu}$ for some $\mu \leq 1$ then the series $(u_n)$ has an infinite sum.

If $0 \leq q < 1$ one has $q^n \preccurlyeq n^{-\mu}$ for any $\mu > 0$; applying the logarithmic criterion of order 0 again proves the convergence of the geometric series $\sum_{n=0}^\infty q^n$ for $|q| < 1$ (Gen. Top., IV, p. 364). If one applies prop. 1 with $v_n = q^n$ one obtains a criterion which may be put in the following form ("Cauchy's criterion"): *Let $(u_n)$ be a series with positive terms; if $\limsup_{n \to \infty}(u_n)^{1/n} < 1$ then the series $(u_n)$ converges; if $\limsup_{n \to \infty}(u_n)^{1/n} > 1$ then the series $(u_n)$ has infinite sum.* Indeed, if $\limsup_{n \to \infty}(u_n)^{1/n} = a < 1$ then $u_n \preccurlyeq q^n$ for every $q$ such that $a < q < 1$. If, on the other hand, $\limsup_{n \to \infty}(u_n)^{1/n} = a > 1$ then $u_n \succcurlyeq q^n > 1$ for infinitely many values of $n$, for any $q$ such that $1 < q < a$; since $u_n$ does not tend to 0 one has $\sum_{n=1}^\infty u_n = +\infty$.

This criterion is very useful in the theory of *entire series*, which we shall study later; but it even so it does not permit one to decide the convergence of the series $(1/n^\alpha)$, in other words, its field of application is much more restricted than that of the logarithmic criteria.

### 2. ASYMPTOTIC EXPANSION OF THE PARTIAL SUMS OF A SERIES

For $x$ real tending to $+\infty$ let $\mathcal{E}$ be a comparison scale formed by functions each of which is defined on a *whole interval* $[x_0, +\infty[$ (depending on the function) and is $\geq 0$ on this interval. Let $(\mathbf{u}_n)$ be a series whose terms belong to a complete normed space $\mathbf{E}$, such that $\mathbf{u}_n$ admits an asymptotic expansion to precision $g_\alpha$ with respect to the scale $\mathcal{E}'$ of restrictions to $\mathbf{N}$ of the functions in $\mathcal{E}$:

$$
\mathbf{u}_n = \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda g_\lambda(n) + \mathbf{r}_\alpha(n).
$$

Suppose that every partial sum $\sum_{m=1}^n g(m)$, where $g \in \mathcal{E}$, admits an asymptotic expansion relative to $\mathcal{E}'$. One can then obtain an asymptotic expansion of the $s_n = \sum_{m=1}^n \mathbf{u}_m$ with respect to $\mathcal{E}'$; again we distinguish two cases:

1° $\sum_{n=1}^{\infty} g_{\alpha}(n) = +\infty$. Then (V, p. 237, prop. 2) one has $\sum_{m=1}^{n} r_{\alpha}(m) \ll \sum_{m=1}^{n} g_{\alpha}(m)$:
by hypothesis one can obtain an asymptotic expansion of
$$
\sum_{\lambda \leq \alpha} a_{\lambda} \left( \sum_{m=1}^{n} g(m) \right)
$$
(V, p. 222) to a certain precision $g_{\sigma}$; if $c g_{\sigma}(n)$ is the principal part of $\sum_{m=1}^{n} g_{\alpha}(m)$, one will have an asymptotic expansion of $s_{n}$ to precision $g_{\min(\rho,\sigma)}$.

2° $\sum_{n=1}^{\infty} g_{\alpha}(n)$ converges; then let $\beta$ be the smallest of the indices $\lambda \leq \alpha$ such that $a_{\lambda} \neq 0$ and such that $\sum_{n=1}^{\infty} g_{\lambda}(n)$ converges; the series
$$
C = \sum_{n=1}^{\infty} \left( u_{n} - \sum_{\lambda < \beta} a_{\lambda} g_{\lambda}(n) \right)
$$
then converges absolutely, and one can write
$$
s_{n} = \sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right) - \sum_{m=n+1}^{\infty} r_{\alpha}(m).
$$
Further, $\sum_{m=n+1}^{\infty} r_{\alpha}(m) \ll \sum_{m=n+1}^{\infty} g_{\alpha}(m)$; if $c g_{\sigma}(n)$ is the principal part of $\sum_{m=n+1}^{\infty} g_{\alpha}(m)$,
and if one has an asymptotic expansion of
$$
\sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right)
$$
to precision $g_{\rho}$ one thus obtains an asymptotic expansion of $s_{n}$ to precision $g_{\min(\rho,\sigma)}$.

One is thus led to the particular case of series $(g(n))$ where $g \in \mathcal{E}$. We shall see how, subject to certain conditions, one can straight away obtain a principal part of $s_{n} = \sum_{m=1}^{n} g(m)$ (when $\sum_{n=1}^{\infty} g(n) = +\infty$) or of $r_{n} = \sum_{m=n+1}^{\infty} g(m)$ (when $\sum_{n=1}^{n} g(n) < +\infty$).

#### Proposition 6 {#fvr-v-s4-prop-6 .statement}

*Let g be a real function, > 0 and monotone, defined on an interval [x_0, +\infty[ (where x_0 \leq 1 ), and such that log g and x are comparable to order 1.*

1° *If g is of infinite order relative to e*, one has

$$
s_n = \sum_{m=1}^n g(m) \sim g(n) \qquad \text{if} \quad \sum_{n=1}^\infty g(n) = +\infty; \tag{1}
$$

$$
r_n = \sum_{m=n+1}^\infty g(m) \sim g(n+1) \qquad \text{if} \quad \sum_{n=1}^\infty g(n) < +\infty. \tag{2}
$$

2° *If g is of finite order $\mu$ with respect to $e^x$ one has*

$$
s_n = \sum_{m=1}^n g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_{\lambda_0}^n g(t) \, dt \qquad \text{if} \quad \sum_{n=1}^\infty g(n) = +\infty; \tag{3}
$$

$$
r_n = \sum_{m=n+1}^\infty g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_n^\infty g(t) \, dt \qquad \text{if} \quad \sum_{n=1}^\infty g(n) < +\infty \tag{4}
$$

(the number $\frac{\mu}{1 - e^{-\mu}}$ is to be replaced by 1 in (3) and (4) when $\mu = 0$).

1° If g is of order $+\infty$ relative to $e^x$ one has $\log g \gg x$ whence $g'/g \gg 1$, or $g' \gg g$, by the hypothesis; g is therefore increasing and tends to $+\infty$ with $x$, whence $\sum_{n=1}^\infty g(n) = +\infty$. If $u$ is the step function associated with the series $(g(n))$ (V, p. 237), one has $u(x) \leq g(x)$ starting from a certain value of $x$, so $u \ll g$ and consequently

$$
s_{n-1} = \int_1^n u(t) \, dt \ll \int_1^n g(t) \, dt \ll \int_1^n g'(t) \, dt \sim g(n);
$$

since $s_n = s_{n-1} + g(n)$ one has $s_n \sim g(n)$. The proof is similar when g is of order $-\infty$ relative to $e^x$; we thus obtain formula (2).

2° If g is of finite order $\mu$ relative to $e^x$ one can write $g(x) = e^{\mu x} h(x)$ where h is of order 0 relative to $e^x$; further, by hypothesis, $\log g \sim \mu x$ for $\mu \neq 0$ ($\log g \ll x$ for $\mu = 0$) implies $h' \ll h$. Suppose first that $\sum_{n=1}^\infty g(n) = +\infty$ (which implies that $\mu \geq 0$; the converse always holds if $\mu > 0$, since then $g(x)$ tends to $+\infty$ with $x$); let us evaluate the principal part of $\int_{n-1}^n g(t) \, dt$. One can write

$$
\int_{n-1}^n g(t) \, dt = \int_{n-1}^n e^{\mu t} h(t) \, dt
$$
$$
= h(n) \int_{n-1}^n e^{\mu t} \, dt + \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt
$$
$$
= \frac{1 - e^{-\mu}}{\mu} g(n) + \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt.
$$

Now, the relation $h' \ll h$ implies that for every $\varepsilon > 0$ there is an $n_0$ such that the relation $x \geq n_0$ implies that $|h'(x)/h(x)| \leq \varepsilon$; one deduces from the mean value theorem that $-\varepsilon \leq \log |h(t)/h(n)| \leq \varepsilon$, for $n-1 \leq t \leq n$, if $n \geq n_0$, whence

$$
|h(t) - h(n)| \leq (e^\varepsilon - 1)h(n)
$$

and consequently

$$
\left| \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt \right| \leq (e^\varepsilon - 1)e^{\mu n}h(n) = (e^\varepsilon - 1)g(n)
$$

since $e^{\mu t}$ is increasing. Since $e^\varepsilon - 1$ becomes arbitrarily small with $\varepsilon$ one sees that one can write

$$
\int_{n-1}^n g(t) \, dt = \frac{1 - e^{-\mu}}{\mu} g(n) + o(g(n))
$$

$\left( \frac{1 - e^{-\mu}}{\mu} \text{ being replaced by } 1 \text{ when } \mu = 0 \right)$. The proposition is then a consequence of prop. 2 of V, p. 237. One argues similarly when $\sum_{n=1}^\infty g(n)$ is finite.

By applying prop. 6 of V, p. 239, repeatedly one can then sometimes obtain an *asymptotic expansion* for $s_n = \sum_{m=1}^n g(m)$. First suppose that $g$ is of order $+\infty$ relative to $e^\lambda$; for every *fixed* value of $p$ one can write, by prop. 6,

$$
s_n = g(n) + g(n-1) + \cdots + g(n-p) + o(g(n-p))
$$

and it suffices to expand (relative to $\mathcal{E}'$) each of the functions $g(n-k)$ ($0 \leq k \leq p$), limiting the precision of the expansions to the principal part of $g(n-p)$, to obtain an expansion for the $s_n$.

#### Example {#fvr-v-s4-n2-exa-1 .statement}

Let $g(x) = x^\lambda = \exp(\lambda \log x)$, of order $+\infty$ relative to $e^\lambda$. Taking $p = 2$ one has

$$
(n-1)\log(n-1) = (n-1)\log n - 1 + \frac{1}{2n} + o\left( \frac{1}{n} \right)
$$

whence (V, p. 225)

$$
(n-1)^{n-1} = \frac{1}{e} n^{n-1} + \frac{1}{2e} n^{n-2} + o_1\left( n^{n-2} \right)
$$

and similarly

$$
(n-2)^{n-2} = \frac{1}{e^2} n^{n-2} + o_2\left( n^{n-2} \right);
$$

consequently

$$
s_n = n^n + \frac{1}{e} n^{n-1} + \left( \frac{1}{2e} + \frac{1}{e^2} \right) n^{n-2} + o_3\left( n^{n-2} \right).
$$

One proceeds similarly (for $r_n$) when $g$ is of order $-\infty$ relative to $e^\lambda$.

Now if $g$ is of finite order $\mu$ relative to $e^x$, and if, for example, $\sum_{n=1}^\infty g(n) = +\infty$, one can write
$$
s_n = \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t)\, dt + \sum_{m=1}^n f_1(m)
$$
where $f_1(n) = g(n) - \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t)\, dt \ll g(n)$ by prop. 6 of V, p. 239. If one has a principal part $c g_1(n)$ of $f_1(n)$ relative to $\mathcal{E}'$, and if one can again apply prop. 6 to the function $g_1$ one will obtain a primitive equivalent to $\sum_{m=1}^n f_1(m)$ if $\sum_{n=1}^\infty g_1(n) = +\infty$, and equivalent to $\sum_{m=n+1}^\infty f_1(m)$ in the opposite case (in the latter case one writes $\sum_{m=1}^n f_1(m) = C - \sum_{m=n+1}^\infty f_1(m)$, with $C = \sum_{n=1}^\infty f_1(n)$).

Step by step one can thus eventually obtain an expression for $s_n$ as the sum of a certain number of primitives each of which is negligible with respect to the previous, of a term remaining negligible relative to the last primitive written, and finally a constant (the case where the remainder term tends to 0). It then remains to expand each of the primitives obtained with respect to $\mathcal{E}'$ (cf. V, p. 235).

#### Example {#fvr-v-s4-n2-exa-2 .statement}

Let $g(n) = \frac{1}{n}$; then
$$
s_n = \sum_{m=1}^n \frac{1}{m} \sim \int_1^n \frac{dt}{t} = \log n
$$
then
$$
\frac{1}{n} - (\log n - \log(n-1)) \sim -\frac{1}{2n^2}
$$
whence
$$
s_n = \log n + \gamma + \frac{1}{2n} + o\left(\frac{1}{n}\right).
$$
The constant $\gamma$ which appears in this formula plays an important rôle in Analysis (cf. chap. VI and VII); it is known as *Euler's constant*; one has
$$
\gamma = 0.577\,215\,664\ldots
$$
to within $1/10^9$.

We shall see in VI, p. 288, how the *Euler-Maclaurin summation formula* gives an asymptotic expansion of *arbitrary* order for $s_n$ (or for $r_n$) in the most important cases.

### 3. ASYMPTOTIC EXPANSION OF THE PARTIAL PRODUCTS OF AN INFINITE PRODUCT

One knows (Gen. Top., V. p. 22 and 23) that for the infinite product with general factor $1 + u_n$ ($u_n > -1$) to be convergent (resp. commutatively convergent) it is necessary and sufficient that the series with general term $\log(1 + u_n)$ should be convergent (resp. commutatively convergent), and that one then has the relation

$$
\log \prod_{n=1}^{\infty} (1 + u_n) = \sum_{n=1}^{\infty} \log(1 + u_n).
$$

When the infinite product converges one knows that $u_n$ tends to 0; thus $\log(1 + u_n) \sim u_n$; now one knows that for a series of real numbers to be commutatively convergent it is necessary and sufficient that it should be absolutely convergent (Gen. Top., IV, p. 372, prop. 5); by prop. 1 one thus recovers the fact that the product with general factor $1 + u_n$ is commutatively convergent if and only if the series with general term $u_n$ is absolutely convergent (Gen. Top., IV, p. 368, th. 4).

A similar argument applies to an infinite product whose general factor is a complex number $1 + u_n$ ($u_n \neq -1$). Indeed, for such a product to be commutatively convergent it is necessary and sufficient (Gen. Top., VIII, p. 115, prop. 2) that the infinite product with general factor $|1 + u_n|$ should be so, and further, if $\theta_n$ is the amplitude of $1 + u_n$ (taken between $-\pi$ and $+\pi$), that the series of the $\theta_n$ should be commutatively convergent. Since $u_n$ tends to 0, $\log(1 + u_n)$ is defined starting from some particular value of $n$ (III, p. 100) and one has

$$
\log(1 + u_n) = \log |1 + u_n| + i \theta_n;
$$

thus, for the product with general factor $1 + u_n$ to be commutatively convergent it is necessary and sufficient that the series with general term $|\log(1 + u_n)|$ be absolutely convergent (Gen Top., VII, p. 84, th. 1); now $\log(1 + u_n) \sim u_n$ (I, p. 18, prop. 5), so one again obtains the condition that the series with general term $u_n$ should be absolutely convergent (Gen. Top., VIII, p. 116, th. 1).

The relation between infinite products and series of real numbers sometimes allows one to obtain an asymptotic expansion for the partial product $p_n = \prod_{k=1}^{n} (1 + u_k)$; it suffices to have an asymptotic expansion for the partial sum $s_n = \sum_{k=1}^{n} \log(1 + u_k)$, then to expand $p_n = \exp(s_n)$; one is thus brought back to the two problems examined earlier (V, p. 238 and p. 226).

*Example: Stirling’s formula.* Let us seek an asymptotic expansion for $n!$; this leads us to expand $s_n = \sum_{p=1}^{n} \log p$, and then $\exp(s_n)$. The method of n 2 gives successively

$$
s_n = \sum_{p=1}^{n} \log p \sim \int_{1}^{n} \log t \, dt = n \log n - n + 1
$$

then
$$
\log n - \int_{n-1}^{n} \log t \, dt = \log n - (n \log n - (n-1) \log(n-1) - 1) \sim \frac{1}{2n}
$$
whence
$$
s_n = n \log n - n + \frac{1}{2} \log n + o(\log n).
$$
Then
$$
\log n - \int_{n-1}^{n} \log t \, dt - \frac{1}{2} (\log n - \log(n-1)) \sim -\frac{1}{12n^2}
$$
whence
$$
s_n = n \log n - n + \frac{1}{2} \log n + k + \frac{1}{12n} + o_1 \left( \frac{1}{n} \right) \quad (k \text{ constant})
$$
and one finally deduces (V, p. 226)
$$
n! = e^k \, n^{n+1/2} \, e^{-n} \left( 1 + \frac{1}{12n} + o_2 \left( \frac{1}{n} \right) \right). \tag{5}
$$
We shall show in VII, p. 322, that $e^k = \sqrt{2\pi}$. The formula (5) (with this value of $k$) is called *Stirling's formula*. In the same way, for every real number $a$ not an integer $> 0$, one shows that
$$
(a+1)(a+2)\ldots(a+n) \sim K(a) \, n^{n+a+\frac{1}{2}} \, e^{-n}. \tag{6}
$$
We shall determine the function $K(a)$ too (VII, p. 18). From formulae (5) and (6) one derives in particular that
$$
\binom{a}{n} \sim (-1)^n \varphi(a) \, n^{-a-1} \tag{7}
$$
for every real number $a$ not an integer $> 0$, where $\varphi(a)$ is a function of $a$ which will be specified in VII, p. 322.

### 4. APPLICATION: CONVERGENCE CRITERIA OF THE SECOND KIND FOR SERIES WITH POSITIVE TERMS

Quite often one meets series $(u_n)$ for which $u_n > 0$ from a certain point on, and $u_{n+1}/u_n$ has an asymptotic expansion which is easy to determine. It is convenient, for such series, to have criteria (called *criteria of the second kind*) allowing one to determine whether the series is convergent from the form of $u_{n+1}/u_n$ alone. The following is such a criterion:

#### Proposition 7 ("Raabe's test") {#fvr-v-s4-prop-7 .statement}

*Let $(u_n)$ be a series with terms $> 0$ from some point on. If, from a certain stage, $u_{n+1}/u_n \leqslant 1 - \frac{\alpha}{n}$ for some $\alpha > 1$, then the series $(u_n)$ converges; if, from a certain point on, $u_{n+1}/u_n \geqslant 1 - \frac{1}{n}$, then the series $(u_n)$ has infinite sum.*

Indeed, if $u_{n+1}/u_n \leqslant 1 - \frac{\alpha}{n}$ with $\alpha > 1$, for all $n \geqslant n_0$, then one has $u_n \preccurlyeq p_n = \prod_{k=n_0}^{n} \left( 1 - \frac{\alpha}{k} \right)$. Now, $\log \left( 1 - \frac{\alpha}{n} \right) = -\frac{\alpha}{n} - \frac{\alpha^2}{2n^2} + o \left( \frac{1}{n^2} \right)$, whence $\log p_n =$ $-\alpha \log n + k + o(1/n)$ ($k$ constant), and $p_n \sim e^k \frac{1}{n^\alpha}$; since $\alpha > 1$ the logarithmic criterion of order 0 allows one to finish.

If, on the other hand, $u_{n+1}/u_n \geq 1 - \frac{1}{n}$ from a certain point, then the same calculation proves that $u_n \geq \frac{1}{n}$, whence the proposition.

One can prove in the same way, using the logarithmic criteria of order $> 0$, the following criterion of the second kind:

#### Proposition 8 {#fvr-v-s4-prop-8 .statement}

*Let $(u_n)$ be a series with terms $> 0$ from a certain point on. If, from a certain point, one has*

$$
\frac{u_{n+1}}{u_n} \leq 1 - \frac{1}{n} - \frac{1}{nl_1(n)} - \ldots - \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)} - \frac{\alpha}{nl_1(n)l_2(n)\ldots l_p(n)}
$$

*for some $\alpha > 1$, then the series $(u_n)$ converges; if, from some point on, one has*

$$
\frac{u_{n+1}}{u_n} \geq 1 - \frac{1}{n} - \frac{1}{nl_1(n)} - \ldots - \frac{1}{nl_1(n)l_2(n)\ldots l_p(n)}
$$

*then the series $(u_n)$ has an infinite sum.*

#### Example {#fvr-v-s4-n4-exa-1 .statement}

Consider the *hypergeometric series*, with general term

$$
u_n = \frac{\alpha(\alpha+1)\ldots(\alpha+n-1)\,\beta(\beta+1)\ldots(\beta+n-1)}{1.2\ldots n.\gamma(\gamma+1)\ldots(\gamma+n-1)}
$$

where $\alpha, \beta, \gamma$ are arbitrary real numbers, not integers $\leq 0$: it is clear that $u_n$ is $> 0$ from a certain stage, or $< 0$ from a certain stage on. One has

$$
\begin{align*}
\frac{u_{n+1}}{u_n} &= \frac{(\alpha+n)(\beta+n)}{(n+1)(\gamma+n)} \\
&= \left(1 + \frac{\alpha+\beta}{n} + \frac{\alpha\beta}{n^2}\right) \left(1 + \frac{\gamma+1}{n} + \frac{\gamma}{n^2}\right)^{-1} \\
&= 1 + \frac{\alpha+\beta-\gamma-1}{n} \\
&\quad + \frac{\alpha\beta-(\alpha+\beta)(\gamma+1)+\gamma^2+\gamma+1}{n^2} + o\left(\frac{1}{n^2}\right).
\end{align*}
$$

Raabe's test shows that the series converges for $\alpha + \beta < \gamma$, and has infinite sum for $\alpha + \beta > \gamma$; when $\alpha + \beta = \gamma$ the series also has an infinite sum, as is shown by prop. 8.

#### Remark 1 {#fvr-v-s4-n4-rem-1 .statement}

As a particular instance of Raabe's test one sees that if $\limsup_{n \to \infty} u_{n+1}/u_n < 1$ the series $(u_n)$ converges; if, on the other hand, $\liminf_{n \to \infty} u_{n+1}/u_n > 1$, the series $(u_n)$ has an infinite sum (*d'Alembert's test*).

#### Remark 2 {#fvr-v-s4-n4-rem-2 .statement}

The criteria of the second kind can be applied only to series whose general term behaves in a very regular way as $n$ tends to $+\infty$; in other words, their scope is much more restricted than those of the logarithmic criteria, and it would be a blunder to try to use them beyond the special cases to which they are particularly suited. For example, for the series $(u_n)$ defined by $u_{2m} = 2^{-m}$, $u_{2m+1} = 3^{-m}$ one has $u_{2m+1}/u_{2m} = \left(\frac{2}{3}\right)^m$, $u_{2m+2}/u_{2m+1} = \frac{1}{2} \left(\frac{3}{2}\right)^m$; the first of these ratios tends to 0 and the second to $+\infty$ as $m$ increases indefinitely, so no criterion of the second kind is applicable; nevertheless, since $u_n \preccurlyeq 2^{-n/2}$, it is immediate that the series converges.

Even when $u_{n+1}/u_n$ has a simple expression, a direct evaluation of a principal part for $u_n$ often leads to a result as quickly as the criteria of the second kind. For example, for the hypergeometric series, Stirling’s formula shows immediately that $u_n \sim a n^{\alpha + \beta - \gamma - 1}$, where $a$ is a constant $\neq 0$, and the logarithmic criterion of order 0 is then applicable.

### Exercises {#fvr-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
