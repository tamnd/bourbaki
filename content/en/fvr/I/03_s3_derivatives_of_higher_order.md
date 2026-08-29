---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 3
section_title: DERIVATIVES OF HIGHER ORDER
lang: en
source: fvr-i-vii
book_pages: 20-23, 39-45
pdf_pages: 0035-0038, 0054-0060
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVES OF ORDER $n$
      page: 20
      pdf_page: 35
    - "no": 2
      title: TAYLOR'S FORMULA
      page: 21
      pdf_page: 36
statements: 8
exercises: 18
content_sha256: df6c54970741a00f1b9a62ec3e7836c5591326bb5afa29b74fdcfa268de3aadc
---

## § 3. DERIVATIVES OF HIGHER ORDER

### 1. DERIVATIVES OF ORDER $n$

Let $f$ be a vector function of a real variable, defined, continuous and differentiable on an interval $I$. If the derivative $f'$ exists on a neighbourhood (with respect to $I$) of a point $x_0 \in I$, and is differentiable at the point $x_0$, then its derivative is called the *second derivative* of $f$ at the point $x_0$, and is denoted by $f''(x_0)$ or $D^2f(x_0)$. If this second derivative exists at every point of $I$ (which implies that $f'$ exists and is continuous on $I$), then $x \mapsto f''(x)$ is a vector function which one denotes by $f''$ or $D^2f$. We define, in the same way, recursively, the $n^{th}$ *derivative* (or *derivative of order* $n$) of $f$, and denote it by $f^{(n)}$ or $D^n f$; by definition, its value at the point $x_0 \in I$ is the derivative of the function $f^{(n-1)}$ at the point $x_0$: this definition presupposes the existence of *all* the derivatives $f^{(k)}$ of order $k \leq n - 1$ on a *neighbourhood* of $x_0$ relative to $I$, and the differentiability of $f^{(n-1)}$ at the point $x_0$.

We will say that $f$ is *n times differentiable* at the point $x_0$ (resp. in an interval) if it admits an $n^{th}$ derivative at this point (resp. in this interval). One says that $f$ is *indefinitely differentiable* on $I$ if for each integer $n > 0$ it admits a derivative of order $n$ on $I$.

By induction on $m$ one sees that

$$
D^m(D^n f) = D^{m+n} f.
$$

More precisely, when one of the two terms in (1) is defined, then so is the other, and is equal to it.

#### Proposition 1 {#fvr-i-s3-prop-1 .statement}

*The set of vector functions defined on an interval* $I \subset \mathbf{R}$, *taking values in a given topological vector space* $E$, *and having an* $n^{th}$ *derivative on* $I$, *is a vector space over* $\mathbf{R}$, *and* $f \mapsto D^n f$ *is a linear mapping of this space into the vector space of linear mappings from* $I$ *into* $E$.

One proves the formulae

$$
D^n(f + g) = D^n f + D^n g \tag{2}
$$
$$
D^n(fa) = D^n f . a \tag{3}
$$

by induction on $n$ when $f$ and $g$ have an $n^{th}$ derivative on $I$ ($a$ being constant).

#### Proposition 2 ("Leibniz' formula") {#fvr-i-s3-prop-2 .statement}

*Let* $E, F, G$ *be three topological vector spaces over* $\mathbf{R}$, *and* $(x, y) \mapsto [x.y]$ *a continuous bilinear mapping of* $E \times F$ *into* $G$. *If* $f$ *(resp.* $g$) *is defined on an interval* $I \subset \mathbf{R}$, *takes its values in* $E$ *(resp.* $F$) *and has an* $n^{th}$ *derivative on* $I$, *then* $[f.g]$ *has an* $n^{th}$ *derivative on* $I$, *given by the formula*

$$
D^n[f.g] = [f^{(n)}.g] + \binom{n}{1}[f^{(n-1)}.g'] + \cdots + \binom{n}{p}[f^{(n-p)}.g^{(p)}] + \cdots + [f.g^{(n)}]. \tag{4}
$$

Formula (4) is proved by induction on $n$ (using the relation $\binom{n}{p} = \binom{n-1}{p} + \binom{n-1}{p-1}$ for the binomial coefficients).

In the same way one can verify the following formula (where the hypotheses are the same as in prop. 2):

$$
[f^{(n)} . g] + (-1)^{n-1} [f . g^{(n)}] = D([f^{(n-1)} . g] - [f^{(n-2)} . g'] + \cdots + (-1)^{n-1} [f . g^{(n-1)}]).
$$

The preceding propositions have been stated for functions that are $n$ times differentiable on an interval; we leave it to the reader to formulate the analogous propositions for functions that are $n$ times differentiable at a point.

### 2. TAYLOR'S FORMULA

Let $f$ be a vector function defined on an interval $I \subset \mathbf{R}$, with values in a *normed* space $E$ over $\mathbf{R}$; to say that $f$ has a derivative at a point $a \in I$ signifies that

$$
\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)(x-a)}{x-a} = 0;
$$

or, otherwise, that $f$ is "approximately equal" to the *linear* function $f(a) + f'(a)(x-a)$ on a neighbourhood of $a$ (*cf.* chap. V, where this concept is developed in a general manner). We shall see that the existence of the $n^{th}$ order derivative of $f$ at the point $a$ entails in the same way that $f$ is "approximately equal" to a *polynomial of degree $n$ in $x$*, with coefficients in $E$ (*Gen. Top.*, X, p. 315) on a neighbourhood of $a$. To be precise:

#### Theorem 1 {#fvr-i-s3-thm-1 .statement}

*If the function $f$ has an $n^{th}$ derivative at the point $a$ then*

$$
\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - \cdots - f^{(n)}(a)\frac{(x-a)^n}{n!}}{(x-a)^n} = 0.
$$

We proceed by induction on $n$. The theorem holds for $n = 1$. For arbitrary $n$ one can, by the induction hypothesis, apply it to the derivative $f'$ of $f$: for any $\varepsilon > 0$ there is an $h > 0$ such that, if one puts

$$
g(x) = f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - f''(a)\frac{(x-a)^2}{2!} - \cdots - f^{(n)}(a)\frac{(x-a)^n}{n!}
$$

one has, for $|y-a| \leq h$ and $y \in I$,

$$
\|g'(y)\| = \left\| f'(y) - f'(a) - f''(a)\frac{(y-a)}{1!} - \cdots - f^{(n)}(a)\frac{(y-a)^{n-1}}{(n-1)!} \right\|
$$
$$
\leq \varepsilon\ |y-a|^{n-1}.
$$

We apply the mean value theorem (I, p. 15, th. 2) on the interval with endpoints $a,\ x$ (with $|x-a| \leq h$) to the vector function $g$ and to the real increasing function equal to $\varepsilon |y - a|^n / n$ if $x > a$, and to $-\varepsilon |y - a|^n / n$ if $x < a$; it follows that $\|g(x)\| \leq \varepsilon |x - a|^n / n$, which proves the theorem.

We thus can write
$$
f(x) = f(a) + f'(a) \frac{(x - a)}{1!} + f''(a) \frac{(x - a)^2}{2!} + \cdots \\
+ f^{(n)}(a) \frac{(x - a)^n}{n!} + u(x) \frac{(x - a)^n}{n!}
$$
where $u(x)$ approaches 0 as $x$ approaches $a$ while remaining in I; this formula is called *Taylor’s formula of order* $n$ at the point $a$, and the right-hand side of (8) is called the *Taylor expansion of order* $n$ of the function $f$ at the point $a$. The last term $r_n(x) = u(x)(x - a)^n / n!$ is called the *remainder* in the Taylor formula of order $n$.

When $f$ has a *derivative of order* $n + 1$ on I, one can estimate $\|r_n(x)\|$ in terms of this $n + 1^{th}$ derivative, on all of I, and not just on an unspecified neighbourhood of $a$:

#### Proposition 3 {#fvr-i-s3-prop-3 .statement}

*If $\|f^{(n+1)}(x)\| \leq M$ on I, then we have*
$$
\|r_n(x)\| \leq M \frac{|x - a|^{n+1}}{(n + 1)!}
$$
*on* I.

Indeed, the formula holds for $n = 0$, by I, p. 15, th. 2. Let us prove it by induction on $n$: by the induction hypothesis applied to $f'$, one has
$$
\|r'_n(y)\| \leq M \frac{|y - a|^n}{n!}
$$
from which the formula (9) follows by the mean value theorem (I, p. 23, th. 2).

#### Corollary {#fvr-i-s3-n2-cor-1 .statement}

*If $f$ is a finite real function with a derivative of order* $n + 1$ *on* I, *and if* $m \leq f^{(n+1)}(x) \leq M$ *on* I, *then for all* $x \geq a$ *in* I *one has*
$$
m \frac{(x - a)^{n+1}}{(n + 1)!} \leq r_n(x) \leq M \frac{(x - a)^{n+1}}{(n + 1)!}
$$
*and the second term cannot be equal to the first* (resp. *to the third*) *unless* $f^{(n+1)}$ *is constant and equal to* $m$ (resp. $M$) *on the interval* $[a, x]$.

The proof proceeds in the same way, but applying th. 1 of I, p. 14.

#### Remark 1 {#fvr-i-s3-n2-rem-1 .statement}

We have already noticed in the proof of th. 1 that if $f$ has a derivative of order $n$ on I, and if
$$
f(x) = a_0 + a_1(x - a) + a_2(x - a)^2 + \cdots + a_n(x - a)^n + r_n(x)
$$
is its Taylor expansion of order $n$ at the point $a$, then the Taylor expansion of order $n - 1$ for $f'$ at the point $a$ is
$$
f'(x) = a_1 + 2a_2(x - a) + \cdots + na_n(x - a)^{n-1} + r'_n(x).
$$

We say that it is obtained from the expansion (11) of $f$ by *differentiating term-by-term*.

#### Remark 2 {#fvr-i-s3-n2-rem-2 .statement}

With the same hypotheses, the coefficients $a_i$ in (11) are determined recursively by the relations

$$
a_0 = f(a)
$$
$$
a_1 = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}
$$
$$
a_2 = \lim_{x \to a} \frac{f(x) - f(a) - a_1(x - a)}{(x - a)^2}
$$
$$
\ldots
$$
$$
a_n = \lim_{x \to a} \frac{f(x) - f(a) - a_1(x - a) - \cdots - a_{n-1}(x - a)^{n-1}}{(x - a)^n}.
$$

In the case $a = 0$ one concludes, in particular, that if $f(x^p)$ ($p$ an integer > 0) has a derivative of order $pn$ on a neighbourhood of 0 then the Taylor expansion of order $pn$ of this function is simply

$$
f(x^p) = a_0 + a_1 x^p + a_2 x^{2p} + \cdots + a_n x^{np} + r_n(x^p)
$$

where $r_n(x^p)$ is the remainder in the expansion (*cf.* V, p. 222).

#### Remark 3 {#fvr-i-s3-n2-rem-3 .statement}

The definition of the derivative of order $n$ and the preceding results generalize immediately to functions of a complex variable; we shall not pursue this topic further here; it will be treated in detail in a later Book in this Series.

### Exercises {#fvr-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
