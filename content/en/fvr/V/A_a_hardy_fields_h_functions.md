---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 0
section_title: Hardy Fields. (H) Functions
appendix: true
lang: en
source: fvr-i-vii
book_pages: 247-258, 263-267
pdf_pages: 0262-0273, 0278-0282
extraction: ocr
subsections:
    - "no": 1
      title: HARDY FIELDS
      page: 247
      pdf_page: 262
    - "no": 2
      title: EXTENSION OF A HARDY FIELD
      page: 248
      pdf_page: 263
    - "no": 3
      title: COMPARISON OF FUNCTIONS IN A HARDY FIELD
      page: 250
      pdf_page: 265
    - "no": 4
      title: (H) FUNCTIONS
      page: 252
      pdf_page: 267
    - "no": 5
      title: EXPONENTIALS AND ITERATED LOGARITHMS
      page: 253
      pdf_page: 268
    - "no": 6
      title: INVERSE FUNCTION OF AN (H) FUNCTION
      page: 255
      pdf_page: 270
statements: 21
exercises: 15
content_sha256: 2b7ece85b767af5816191cdddb2a46c6ea11aaccc68f65d9ac9a41b8c196aa46
---

## APPENDIX

# Hardy Fields. (H) Functions

### 1. HARDY FIELDS

Let $\mathfrak{F}$ be the filter base on $\mathbf{R}$ formed by the intervals of the form $[x_0, +\infty[$. Recall that we have defined an equivalence relation $R_\infty$: on the set $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ of real functions defined on sets belonging to $\mathfrak{F}$ “there exists a set $M \in \mathfrak{F}$ such that $f(x) = g(x)$ on $M$” (V, p. 211), and that the quotient set $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$ is endowed with the structure of a *ring* with unit element.

#### Definition 1 {#fvr-v-a0-def-1 .statement}

*Given a subset $\mathfrak{K}$ of $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ one says that $\mathfrak{K}/R_\infty$ (the canonical image of $\mathfrak{K}$ in $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$) is a Hardy field, if $\mathfrak{K}$ satisfies the following conditions:

1. $\mathfrak{K}/R_\infty$ is a subfield of the ring $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$.
2. *Every function in $\mathfrak{K}$ is continuous and differentiable on an interval $[a, +\infty[$ (depending on the function), and the class with respect to $R_\infty$ of its derivative belongs to $\mathfrak{K}/R_\infty$.*

The hypothesis that $\mathfrak{K}/R_\infty$ is a *field* is equivalent to the following conditions: if $f \in \mathfrak{K}$ and $g \in \mathfrak{K}$ then $f + g$ and $fg$ are equal to functions in $\mathfrak{K}$ on some set in $\mathfrak{F}$; further, if $f$ is not identically zero on a set in $\mathfrak{F}$ then there exists a set $M$ in $\mathfrak{F}$ on which $f$ *does not vanish*, and $1/f$ is equal to a function from $\mathfrak{K}$ on $M$; by condition 2' one can always assume that $M$ is taken so that $f$ is *continuous* on $M$, and consequently *has constant sign* on this interval.

By an abuse of language, if $\mathfrak{K}$ is such that $\mathfrak{K}/R_\infty$ is a Hardy field we shall say in what follows that $\mathfrak{K}$ is itself a *Hardy field*.

#### Example 1 {#fvr-v-a0-n1-exa-1 .statement}

Every Hardy field contains the field of *rational constants* (the smallest field of characteristic 0, *cf. Alg.*, V, §1), which one can identify with the field $\mathbf{Q}$; moreover, since two constants cannot be congruent modulo $R_\infty$ unless they are equal, $\mathbf{Q}/R_\infty$ is identical to $\mathbf{Q}$. The *real constants* also form a Hardy field, which one can identify with $\mathbf{R}$.

#### Example 2 {#fvr-v-a0-n1-exa-2 .statement}

A very important example of a Hardy field is the *set of rational functions with real coefficients*, which we shall denote by $\mathbf{R}(x)$, by an abuse of language; if $f(x) = p(x)/q(x)$ is a rational function with real coefficients, not identically zero, it is continuous, differentiable, and $\neq 0$ on an interval $[a, +\infty[$, where $a$ is strictly greater than the largest of the real roots of the polynomials $p(x)$ and $q(x)$; thus every element of $\mathbf{R}(x)/R_\infty$ other than 0 is invertible. We note again that two rational functions cannot be congruent modulo $\mathbf{R}_\infty$ unless they are equal, so $\mathbf{R}(x)/\mathbf{R}_\infty$ can again be identified with $\mathbf{R}(x)$.

### 2. EXTENSION OF A HARDY FIELD

Given a Hardy field $\mathfrak{K}$ we shall see how one can form new Hardy fields $\mathfrak{K}' \supset \mathfrak{K}$ such that $\mathfrak{K}'/\mathbf{R}_\infty$ is obtained by *adjoining* (in the algebraic sense of the term, *cf. Alg.*, V. §2) new elements, of a form which we shall make precise, to $\mathfrak{K}/\mathbf{R}_\infty$.

#### Lemma 1 {#fvr-v-a0-lem-1 .statement}

*Let* $a(x), b(x)$ *be two continuous real functions that do not change sign on an interval* $[x_0, +\infty[$. *If, on this interval, the function* $y(x)$ *is continuous and differentiable, and satisfies the identity*

$$
y' = ay + b
$$

(1)

*then there exists an interval* $[x_1, +\infty[$ *on which* $y$ *does not change sign.*

Indeed, let us put $z(x) = y(x) \exp \left( - \int_{x_0}^x a(t) \, dt \right)$ (*cf. IV*, p. 183); then, by (1), $z'(x) = b(x) \exp \left( - \int_{x_0}^x a(t) \, dt \right)$. If $b(x) \geqslant 0$ for $x \geqslant x_0$ then $z$ is increasing on this interval, so either is $< 0$ on all this interval, or is zero on an interval $[x_1, +\infty[$, or else is $> 0$ on an interval $[x_1, +\infty[$; since $y$ has the same sign as $z$ the proposition is proved in this case. The argument is similar if $b(x) \leqslant 0$ for $x \geqslant x_0$.

#### Remark {#fvr-v-a0-n2-rem-1 .statement}

This very elementary property does not extend to linear differential equations of order $> 1$; for example, the function $y = \sin x$ satisfies $y'' + y = 0$, but changes sign on every neighbourhood of $+\infty$.

#### Lemma 2 {#fvr-v-a0-lem-2 .statement}

*Let* $a(x)$ *and* $b(x)$ *be two functions belonging to a given Hardy field* $\mathfrak{K}$ *and* $y(x)$ *a function satisfying the identity* (1) *on an interval* $[x_0, +\infty[$ *where* $a$ *and* $b$ *are defined and continuous*. *If* $p(u)$ *is a polynomial in* $u$ *whose coefficients are functions of* $x$ *belonging to* $\mathfrak{K}$, *defined and differentiable on* $[x_0, +\infty[$, *then there exists an interval* $[x_1, +\infty[$ *on which the function* $p(y)$ *does not change sign*.

The proposition is trivial if $p(u)$ has coefficients which are identically zero on $[x_0, +\infty[$, or if $p(u)$ is of degree 0 in $u$, since any function in $\mathfrak{K}$ is of constant sign on an interval $[x_1, +\infty[$. Suppose that $p(u)$ is of degree $n > 0$; the leading coefficient $c$ of $p(u)$ is then $\neq 0$ on an interval $[\alpha, +\infty[$; one can thus write $p(u) = c(u^n + c_1 u^{n-1} + \cdots + c_n)$ where $c, c_1, c_2, \ldots, c_n$ are *functions* belonging to $\mathfrak{K}$ and differentiable on $[\alpha, +\infty[$; so it is enough to prove the lemma for $c = 1$. We argue by induction on $n$; one has

$$
\frac{d}{dx} (p(y)) = (ay + b)(ny^{n-1} + (n-1)c_1 y^{n-2} + \cdots + c_{n-1})
$$
$$
+ c'_1 y^{n-1} + \cdots + c'_n = na\ p(y) + q(y)
$$

where $q(u)$ is a polynomial of degree $\leq n - 1$, with coefficients in $\mathfrak{K}$. By hypothesis the functions $na(x)$ and $q(y(x))$ do not change sign on an interval $[ \beta, +\infty[$; the lemma is thus a consequence of lemma 1.

#### Theorem 1 {#fvr-v-a0-thm-1 .statement}

*Let $a(x)$ and $b(x)$ be two functions belonging to a given Hardy field $\mathfrak{K}$ and $y(x)$ a function satisfying (1) on an interval $[ x_0, +\infty[$. When $r(u) = p(u)/q(u)$ runs through the set of rational fractions in $u$ with coefficients in $\mathfrak{K}$ such that $q(y)$ is not identically zero on a neighbourhood of $+\infty$ the set $\mathfrak{K}(y)$ of functions $r(y)$ forms a Hardy field.*

Indeed, by lemma 2, there exists an interval $[ x_1, +\infty[$ on which $r(y)$ is defined, continuous, and does not change sign, from which it follows immediately that $\mathfrak{K}(y)/\mathbf{R}_\infty$ is a field; moreover, since

$$
\frac{d}{dx}(r(y)) = r'(y)y' = r'(y)(ay + b)
$$

(where $r'(y) = (p'(y)q(y) - p(y)q'(y))/(q(y))^2$ is defined by hypothesis on a neighbourhood of $+\infty$), the derivative of every function in $\mathfrak{K}(y)$ belongs to $\mathfrak{K}(y)$, which proves that $\mathfrak{K}(y)$ satisfies the conditions of def. 1 of V, p. 247.

It is clear that $\mathfrak{K}(y)/\mathbf{R}_\infty$ is obtained by the algebraic *adjunction* to $\mathfrak{K}/\mathbf{R}_\infty$ of the class of $y$ modulo $\mathbf{R}_\infty$. Again one says that $\mathfrak{K}(y)$ is obtained by *adjoining* $y$ to $\mathfrak{K}$.

#### Corollary 1 {#fvr-v-a0-thm-1-cor-1 .statement}

*If $y$ is a function in $\mathfrak{K}$, not identically zero on a neighbourhood of $+\infty$, then $\mathfrak{K}(\log|y|)$ is a Hardy field.*

Indeed, $(\log|y|)' = y'/y$ is equal to a function in $\mathfrak{K}$ on an interval $[ x_0, +\infty[$.

COROLLARY 2 *If $y$ is any function in $\mathfrak{K}$, then $\mathfrak{K}(e^y)$ is a Hardy field.*

Indeed, $(e^y)' = e^y y'$, and $y'$ is equal to a function in $\mathfrak{K}$ on an interval $[ x_0, +\infty[$.

COROLLARY 3 *If $\mathfrak{K}$ contains the real constants, and if $y$ is a function in $\mathfrak{K}$, not identically zero on a neighbourhood of $+\infty$, then $\mathfrak{K}(|y|^{\alpha})$ is a Hardy field for every real number $\alpha$.*

Indeed, $\frac{d}{dx}(|y|^{\alpha}) = |y|^{\alpha} (\alpha y'/y)$, and $\alpha y'/y$ is equal to a function in $\mathfrak{K}$ on an interval $[ x_0, +\infty[$.

Finally, we note that if $y$ is the *primitive* of any function in $\mathfrak{K}$ then $\mathfrak{K}(y)$ is again a Hardy field.

### 3. COMPARISON OF FUNCTIONS IN A HARDY FIELD

#### Proposition 1 {#fvr-v-a0-prop-1 .statement}

*Two functions in the same Hardy field are comparable to any order* (V, p. 232).

Indeed, if $f$ belongs to a Hardy field $\mathcal{K}$, then for every integer $n > 0$ there exists an interval $[x_0, +\infty[$ on which $f$ is $n$ times differentiable, its $n^{th}$ derivative being equal to a function in $\mathcal{K}$ on this interval. It is therefore enough to show that any two functions $f, g$ of $\mathcal{K}$ are *comparable*. This is evident if one of the functions is identically zero on a neighbourhood of $+\infty$; one may therefore restrict oneself to the case where they are both strictly positive on a neighbourhood of $+\infty$. But then, for every real number $t$, $f - tg$ is equal to a function in $\mathcal{K}$ on a neighbourhood of $+\infty$, so has constant sign on a neighbourhood of $+\infty$, which proves the proposition (V, p. 217, prop. 9).

One deduces immediately from this proposition that, if a Hardy field $\mathcal{K}$ contains the real constants (as we shall always assume in what follows), and if $f$ and $g$ are any two functions in $\mathcal{K}$ then any two of the functions $e^f, e^g, \log |f|, \log |g|, |f|^{\alpha}, |g|^{\alpha}$ ($\alpha$ an arbitrary real), $\int_a f, \int_a g$ ($a$ being any real number in an interval $[x_0, +\infty[$ where $f$ and $g$ are regulated) are *comparable* (when they are defined); indeed, any two of these functions belong to a given Hardy field obtained by adjoining them successively to $\mathcal{K}$.

Similarly, every function $f(x)$ in a Hardy field $\mathcal{K}$ is comparable to $x$, since $x$ and $f(x)$ belong to the Hardy field obtained by adjoining $x$ to $\mathcal{K}$. One thus concludes (in particular) that $f$ is comparable to any order to every power $x^{\alpha}$, as well as to $\log x$ and to $e^x$.

One also sees that if $f$ and $g$ belong to the same Hardy field $\mathcal{K}$, if $g(x) > 0$ on an interval $[x_0, +\infty[$, and if $g(x)$ tends to 0 or to $+\infty$ as $x$ tends to $+\infty$, then the *order* of $f$ relative to $g$ (V, p. 219) is always defined.

Prop. 8 of V, p. 233, is therefore applicable to every function $f$ in a Hardy field, and proves that:

1) if $f$ is of order $+\infty$ relative to $x$ then $\int_a^x f(t)\,dt \sim (f(x))^2/f'(x)$.

2) if $f$ is of order $\mu > -1$ relative to $x$ then $\int_a^x f(t)\,dt \sim \frac{1}{\mu+1} x f(x)$.

3) if $f$ is of order $\mu < -1$ relative to $x$ then $\int_a^{+\infty} f(t)\,dt \sim -\frac{1}{\mu+1} x f(x)$.

4) if $f$ is of order $-\infty$ relative to $x$ then $\int_a^{+\infty} f(t)\,dt \sim -(f(x))^2/f'(x)$.

Further, we have the following proposition:

#### Proposition 2 {#fvr-v-a0-prop-2 .statement}

Let $f$ be a function belonging to a Hardy field $\mathcal{K}$.

1 If $f$ is of infinite order relative to $x$, then, for every integer $n > 0$,
$$
f^{(n)}(x) \sim \frac{(f'(x))^n}{(f(x))^{n-1}}.
$$
(2)

2° If $f$ is of finite order $\mu$ relative to $x$ then, for every $n > 0$,
$$
f^{(n)}(x) \sim \mu(\mu - 1) \ldots (\mu - n + 1) \frac{f(x)}{x^n}
$$
$$
\sim \frac{(\mu - 1) \ldots (\mu - n + 1)}{\mu^{n-1}} \frac{(f'(x))^n}{(f(x))^{n-1}}
$$
(3)
except if $\mu$ is an integer $\geqslant 0$ and $n > \mu$.

1 If $f$ is of infinite order relative to $x$ one has $\log |f| \gg \log x$, so, since $\log |f|$ and $\log x$ are comparable to any order, $f'/f \gg 1/x$. Put $g = f'/f$; since $g$ is equal to a function in $\mathcal{K}$ on a neighbourhood of $+\infty$ one deduces from $1/g \ll x$, that $g'/g^2 \ll 1$, and so $g'/g \ll g = f'/f$, or again $fg' \ll gf'$. From the relation $f' = fg$ one deduces by differentiating that
$$
f'' = fg' + gf' \sim gf'
$$
or again $f''/f' \sim f'/f$. The same argument, applied to $f^{(n)}$ instead of $f$, shows, by induction on $n$, that $f^{(n)}/f^{(n-1)} \sim f'/f$; whence relation (2).

2 If $f$ is of finite order $\mu$ relative to $x$, and if $\mu \neq 0$, one has $\log |f| \sim \mu \log x$, whence, on differentiating, $f'(x) \sim \mu \frac{f(x)}{x}$; one deduces that $f'$ is of order $\mu - 1$ relative to $x$, which allows one to apply the same argument by induction on $n$ so long as $\mu \neq n$, whence formula (3) when $\mu$ is not an integer $\geqslant 0$ and $< n$.

When $f$ is of integral order $p \geqslant 0$ relative to $x$ one can write $f(x) = x^p f_1(x)$, where $f_1$ is of order 0 relative to $x$. By prop. 2 one has
$$
f^{(p)} \sim p! f_1.
$$
To evaluate the derivatives of order $n > p$ one may restrict oneself to the case $p = 0$. Then one has $\log |f| \ll \log x$, whence $f'(x)/f(x) \ll 1/x$, in other words $x f'(x) \ll f(x)$; if $f$ is not equivalent to a constant $k \neq 0$ one has, on differentiating this relation (V, p. 232, prop. 7), $x f''(x) + f'(x) \ll f'(x)$, which implies that $x f''(x) \sim -f'(x)$. Taking account of this formula, one sees by induction on $n$ that $f^{(n)}$ is of order $\leqslant -n$ relative to $x$, and that
$$
f^{(n)} \sim (-1)^{n+1} (n-1)! \frac{f'(x)}{x^{n-1}}.
$$
(4)

If $f$ is equivalent to a constant $k \neq 0$ one has $f(x) = k + f_2(x)$ with $f_2 \ll 1$, and it reduces to studying the derivatives of $f_2$.

### 4. (H) FUNCTIONS

#### Proposition 3 {#fvr-v-a0-prop-3 .statement}

*If $\mathcal{K}_0$ is a Hardy field there exists a Hardy field $\mathcal{K}$ containing $\mathcal{K}_0$ and such that, for every function $z \in \mathcal{K}$, not identically zero on a neighbourhood of $+\infty$, both $e^z$ and $\log |z|$ belong to $\mathcal{K}$.*

Denote by $\mathcal{K}$ the set of functions $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$ having the following properties: for each function $f \in \mathcal{K}$ there is a finite number of Hardy fields $\mathcal{K}_1, \mathcal{K}_2, \ldots, \mathcal{K}_n$ (the number $n$ and the fields $\mathcal{K}_i$ depending on $f$) such that $f \in \mathcal{K}_n$ and, for $0 \leq i \leq n-1$, one has $\mathcal{K}_{i+1} = \mathcal{K}_i(u_{i+1})$ where $u_{i+1}$ is equal either to $e^{z_i}$ or to $\log |z_i|$ with $z_i$ belonging to $\mathcal{K}_i$ and not vanishing identically on a neighbourhood of $+\infty$. One says that $u_1, u_2, \ldots, u_n$ form a *definition sequence* for the field $\mathcal{K}_n$ and of the function $f$; the same function can naturally admit several definition sequences.

By def. 1 of V, p. 247, every function $f \in \mathcal{K}$, not identically zero on a neighbourhood of $+\infty$, has constant sign and is differentiable on an interval $[x_0, +\infty[$; if $f \in \mathcal{K}_n$, then $1/f$ and $f'$ are equal to functions in $\mathcal{K}_n$, thus to functions in $\mathcal{K}$, on a neighbourhood of $+\infty$. To see that $\mathcal{K}$ is a Hardy field it is enough to prove that if $f$ and $g$ are two functions in $\mathcal{K}$ then $f - g$ and $fg$ are equal to functions in $\mathcal{K}$ on a neighbourhood of $+\infty$. Now let $u_1, u_2, \ldots, u_m$ be a definition sequence for $f$, and $v_1, v_2, \ldots, v_n$ a definition sequence for $g$. The sequence $u_1, u_2, \ldots, u_m, v_1, v_2, \ldots, v_n$ obtained by concatenating the sequences $(u_i)$ and $(v_i)$ is again a definition sequence of a Hardy field $\mathcal{K}_{m+n}$ and this field contains $f$ and $g$, so $f - g$ and $fg$ are equal to functions in $\mathcal{K}_{m+n}$ on a neighbourhood of $+\infty$.

One says that the Hardy field $\mathcal{K}$ defined in the proof of prop. 3 is the (H) *extension* of the Hardy field $\mathcal{K}_0$.

If $\mathcal{K}'$ is another Hardy field possessing the properties stated in prop. 3, it follows from the construction of $\mathcal{K}$ that $\mathcal{K}/\mathbf{R}_\sim$ is *contained* in $\mathcal{K}'/\mathbf{R}_\sim$. By abuse of language, one says that the (H) extension of the Hardy field $\mathcal{K}_0$ is the *smallest* Hardy field $\mathcal{K}$ having these properties.

#### Definition 2 {#fvr-v-a0-def-2 .statement}

*The field of (H) functions is called the (H) extension of the Hardy field $\mathbf{R}(x)$ of rational functions with real coefficients. Any function belonging to this extension is called an (H) function.*

Following this definition, if $f$ is an (H) function, not identically zero on a neighbourhood of $+\infty$, then $e^f$ and $\log |f|$ are also (H) functions. More generally, if $g$ is a second (H) function, and $u_1, u_2, \ldots, u_n$ a definition sequence for $g$, and if $f(x)$ tends to $+\infty$ with $x$, one sees by induction on $n$ that the composite functions $u_1 \circ f, u_2 \circ f, \ldots, u_n \circ f$ and $g \circ f$ are (H) functions.

### 5. EXPONENTIALS AND ITERATED LOGARITHMS

We have already (V, p. 229) defined the *iterated logarithms* $l_n(x)$ by the conditions $l_0(x) = x, l_n(x) = \log(l_{n-1}(x))$ for $n \geq 1$. In the same way one defines the *iterated exponentials* $e_n(x)$ by the conditions $e_0(x) = x, e_n(x) = \exp(e_{n-1}(x))$ for $n \geq 1$. It is immediate, by induction on $n$, that $l_n(x)$ is the inverse function of $e_n(x)$, defined for $x > e_{n-1}(0)$, and that $e_m(e_n(x)) = e_{m+n}(x), l_m(l_n(x)) = l_{m+n}(x)$. By the relations $\log x \ll x^\mu \ll e^x$ for every $\mu > 0$, one has, for $n \geq 1$,

$$
l_n(x) \ll (l_{n-1}(x))^\mu \quad \text{for every } \mu > 0 \tag{5}
$$

$$
e_{n-1}(x^{1+\beta}) \ll e_n(x^{1+\delta}) \ll e_n((1-\gamma)x) \ll (e_n(x))^\mu
$$
$$
\ll e_n((1+\alpha)x) \ll e_n(x^{1+\beta}) \tag{6}
$$

for all $\mu > 0, \alpha > 0, \beta > 0, 0 < \gamma < 1, 0 < \delta < 1$, these numbers being otherwise arbitrary (*cf.* V, p. 218, prop. 11).

We have already seen (V, p. 229) that, for $n \geq 1$, one has

$$
\frac{d}{dx}(l_n(x)) = \prod_{i=0}^{n-1} \frac{1}{l_i(x)}. \tag{7}
$$

Similarly for $n \geq 1$

$$
\frac{d}{dx}(e_n(x)) = \prod_{i=1}^n e_i(x). \tag{8}
$$

whence, by prop. 8 of V, p. 233, for every $\mu > 0$

$$
\int_a^x e_n(t^\mu) \, dt \sim \frac{x}{\mu} e_n(x^\mu) \prod_{i=0}^{n-1} \frac{1}{e_i(x^\mu)} \tag{9}
$$

$$
\int_x^{+\infty} \frac{dt}{e_n(t^\mu)} \sim \frac{x}{\mu} \prod_{i=0}^n \frac{1}{e_i(x^\mu)}. \tag{10}
$$

One can show that if $f$ is *any* (H) function such that $f \gg 1$ then there exist two integers $m$ and $n$ such that

$$
l_m(x) \ll f(x) \ll e_n(x)
$$

(V, p. 263, exerc. 1 and p. 264, exerc. 5) On the other hand, one can define increasing functions $g(x)$ (which are no longer (H) functions) such that $g(x) \gg e_n(x)$ for *every* $n > 0$, or $1 \ll g(x) \ll l_m(x)$ for *every* $m > 0$ (V, p. 265, exerc. 8, 9 and 10).

With the help of the iterated logarithms we shall show that one can define a *comparison scale* $\mathcal{E}$ (for $x$ tending to $+\infty$) of (H) functions, which are $> 0$ on a neighbourhood of $+\infty$ and satisfy the following conditions:

a) the product of any two functions in $\mathcal{E}$ belongs to $\mathcal{E}$;
b) $f^\mu \in \mathcal{E}$ for every function $f \in \mathcal{E}$ and every real number $\mu$;

c) for every function $f \in \mathcal{E}$, $\log f$ is a linear combination of a finite number of functions in $\mathcal{E}$;
d) for every function $f \in \mathcal{E}$, apart from the constant 1, $e^f$ is equivalent to a function in $\mathcal{E}$.

First we consider the set $\mathcal{E}_0$ of functions of the form $\prod_{m=0}^{\infty} (l_m(x))^{\alpha_m}$, where the $\alpha_m$ are real numbers, zero apart from for a finite number of indices $m$; it is immediate, from (5) (V, p. 253) that these functions form a *comparison scale* which satisfies conditions $a), b)$ and c). Now we define, by recursion on $n$, the set $\mathcal{E}_n$ (for $n \geqslant 1$) formed by the constant 1 and by the functions of the form $\exp \left( \sum_{k=1}^p a_k f_k \right)$, where $p$ is an arbitrary integer $> 0$, the functions $f_k$ ($1 \leqslant k \leqslant p$) are functions in $\mathcal{E}_{n-1}$ such that $f_1 \gg f_2 \gg \cdots \gg f_p \gg 1$, and the $a_k$ are real numbers $\neq 0$; we show by induction that $\mathcal{E}_n$ is a *comparison scale* satisfying $a), b)$ and c) and containing $\mathcal{E}_{n-1}$. In the first place, the relation $\mathcal{E}_{n-1} \subset \mathcal{E}_n$ holds for $n = 1$, since the logarithm of any nonconstant function in $\mathcal{E}_0$ is of the form $\sum_{k=1}^p a_k f_k$, where the $f_k$ are iterated logarithms, and so $\gg 1$; on the other hand, if $\mathcal{E}_{n-2} \subset \mathcal{E}_{n-1}$ one deduces from the definition of $\mathcal{E}_n$ that $\mathcal{E}_{n-1} \subset \mathcal{E}_n$; this definition furthermore shows that $\mathcal{E}_n$ satisfies $a), b)$ and c). It remains to see that $\mathcal{E}_n$ is a comparison scale: since the quotient of two functions in $\mathcal{E}_n$ again belongs to $\mathcal{E}_n$ it suffices to prove that every function $f$ of $\mathcal{E}_n$, apart from the constant 1, cannot be equivalent to a constant $\neq 0$. Now one has $\log f = \sum_{k=1}^p a_k f_k \sim a_1 f_1$ by construction, and since $f_1 \gg 1$, $\log f$ tends to $\pm \infty$, so $f$ tends to 0 or to $+\infty$ as $x$ tends to $+\infty$.

This being so, if $\mathcal{E}$ is the *union* of the $\mathcal{E}_n$ for $n \geqslant 0$, then $\mathcal{E}$ is a comparison scale, for two functions in $\mathcal{E}$ belong to the same scale $\mathcal{E}_n$; for the same reason, $\mathcal{E}$ satisfies a), and it is clear that it also satisfies b) and c). Finally, if $f \in \mathcal{E}$ there exists an $n$ such that $f \in \mathcal{E}_n$; if $f$ is not the constant 1 then $f(x)$ tends to 0 or to $+\infty$ as $x$ tends to $+\infty$; in the first case $e^f \sim 1$ and in the second, $e^f$ belongs to $\mathcal{E}_{n+1}$ by definition, and so to $\mathcal{E}$.

#### Remark {#fvr-v-a0-n5-rem-1 .statement}

Despite the practical usefulness of the scale $\mathcal{E}$ which we have just defined, it is easy to give examples of (H) functions which *have no principal part* with respect to $\mathcal{E}$. Indeed, if $f$ is an (H) function such that $f \sim a g$, where $a$ is a constant $> 0$ and $g \in \mathcal{E}$, then $\log f - \log g - \log a$ tends to 0 with $1/x$, so $\log f$ admits, relative to $\mathcal{E}$, an asymptotic expansion whose *remainder tends to 0*, by property c). Now, if one considers for example the (H) function $f(x) = e_2 \left( x + \frac{1}{x} \right)$ one has $\log f(x) = \exp \left( x + \frac{1}{x} \right)$, so the asymptotic expansions of $\log f$ relative to $\mathcal{E}$ are of the form

$$
\log f(x) = e^x + \frac{e^x}{x} + \frac{1}{2!} \frac{e^x}{x^2} + \cdots + \frac{1}{n!} \frac{e^x}{x^n} + o \left( \frac{e^x}{x^n} \right) \quad (n \text{ an integer } > 0).
$$

It is clear that the remainder in this expansion is equivalent to $\frac{1}{(n+1)!} \frac{e^x}{x^{n+1}}$, so does not tend to 0. Hence $f$ does not have a principal part relative to $\mathcal{E}$.

### 6. INVERSE FUNCTION OF AN (H) FUNCTION

If $f$ is an (H) function, then $f$ is monotone and continuous on an interval $[x_0, +\infty[$, so the inverse function $\varphi$ of the restriction of $f$ to this interval is monotone and continuous on a neighbourhood of the point $a = \lim_{x \to +\infty} f(x)$; but, if $a$ is equal to $+\infty$ (resp. $-\infty$, finite), one can show that $\varphi(y)$ (resp. $\varphi(-y)$, $\varphi \left( a + \frac{1}{y} \right)$ or $\varphi \left( a - \frac{1}{y} \right)$) is not in general equal to an (H) function on a neighbourhood of $+\infty$. Nevertheless we shall see that in certain important cases one can obtain an (H) function equivalent to $\varphi(y)$ (resp. $\varphi(-y)$, $\varphi \left( a + \frac{1}{y} \right)$, $\varphi \left( a - \frac{1}{y} \right)$) and sometimes even an asymptotic expansion of this function relative to the scale $\mathcal{E}$ defined in V, p. 254.

We shall use the following proposition:

#### Proposition 4 {#fvr-v-a0-prop-4 .statement}

Let $p$ and $q$ be two (H) functions which are strictly positive on an interval $[x_0, +\infty[$.

1° If $q \ll p/p'$ one has $p(x + q(x)) \sim p(x)$.
2° If both $q \ll p/p'$ and $q(x) \ll x$ then $p(x - q(x)) \sim p(x)$.

The two parts of this proposition are clear if $p \sim k$ (constant $\neq 0$); one may therefore suppose that $p(x) \ll 1$ (otherwise one applies the argument to $1/p$). One then deduces $p'(x) \ll 1$.

1° One can write $p(x + q(x)) = p(x) + q(x)p'(x + \theta q(x))$ with $0 \leq \theta \leq 1$ (I, p. 14, corollary). Since $|p'(x)|$ tends to 0 as $x$ tends to $+\infty$, and is equal to an (H) function on a neighbourhood of $+\infty$, it is decreasing on an interval $[x_1, +\infty[$, so, for $x \geq x_1$, one has $|p'(x + \theta q(x))| \leq |p'(x)|$; since $qp' \ll p$ one has $p(x + q(x)) \sim p(x)$.

2° The condition $q(x) \ll x$ ensures that $x - q(x)$ tends to $+\infty$ with $x$. Again one has $p(x - q(x)) = p(x) - q(x)p'(x - \theta p(x))$ with $0 \leq \theta \leq 1$. The same argument as in the first part of the proof shows that, for $x$ sufficiently large, $|p'(x - \theta q(x))| \leq |p'(x - q(x))|$. It reduces to showing that $q(x) \frac{p'(x - q(x))}{p(x - q(x))}$ tends to 0 as $x$ tends to $+\infty$. The proposition is true if $p'/p \gg 1$ since then $|p'/p|$ is an (H) function, increasing for $x$ large enough; thus $q(x) \frac{|p'(x - q(x))|}{|p(x - q(x))|} \leq q(x) \frac{|p'(x)|}{|p(x)|}$, and $qp' \ll p$ by hypothesis. It is also true if $p'/p \sim k$ ($k$ constant $\neq 0$), for then

$$
\frac{p'(x - q(x))}{p(x - q(x))} \sim \frac{p'(x)}{p(x)}
$$

since $x - q(x)$ tends to $+\infty$. It only remains to examine the case where $p'/p \ll 1$. First suppose that $p(x)$ is of *finite* order relative to $x$, and so (V, p. 232, prop. 7) $p'(x)/p(x) \ll 1/x$. Then one has
$$
\frac{p'(x-q(x))}{p(x-q(x))} = \frac{1}{x-q(x)} O_1(1),
$$
so
$$
q(x) \frac{p'(x-q(x))}{p(x-q(x))} = \frac{q(x)}{x} \left( 1 - \frac{q(x)}{x} \right)^{-1} O_1(1) = \frac{q(x)}{x} O_2(1),
$$
and one sees in this case that the proposition is true subject *only* to the hypothesis that $q(x) \ll x$. Finally we examine the case where $1/x \ll p'(x)/p(x) \ll 1$; the function $r = p'/p$ is then of finite order relative to $x$; since, by the preceding remark, prop. 4 of V, p. 255, is applicable to such a function, one has $p'(x-q(x))/p(x-q(x)) \sim p'(x)/p(x)$, and the hypothesis $qp' \ll p$ allows us to complete the proof.

#### Remark {#fvr-v-a0-n6-rem-3 .statement}

The conditions imposed on $q(x)$ may not be improved, as the following examples show:

a)
$$
p(x) = e^x, \quad q(x) = 1 = \frac{p(x)}{p'(x)}, \quad p(x+q(x)) = ep(x)
$$

b)
$$
p(x) = \log x, \quad q(x) = x - \log x \ll \frac{p(x)}{p'(x)} = x \log x,
$$
$$
p(x-q(x)) = \log \log x \ll p(x).
$$

We shall first study the inverses of (H) functions of a particular sort:

#### Proposition 5 {#fvr-v-a0-prop-5 .statement}

*Let g be an* (H) *function not equivalent to a constant $\neq 0$, and such that* $g(x) \ll x$, *and let* $u(x)$ *be the inverse function of* $x - g(x)$, *defined on a neighbourhood of* $+\infty$. *Let* $(u_n)$ *be the sequence of functions defined, by recursion on* $n$, *by the conditions* $u_0(x) = x$, $u_n(x) = x + g(u_{n-1}(x))$ *for* $n \geqslant 1$; *then* $u_n \gg 1$ *and*
$$
u(x) - u_n(x) \sim g(x)(g'(x))^n.
$$ (11)

Let us put $y = u(x)$, $y_n = u_n(x)$; then $x = y - g(y)$, $y_0 = x$ and $y_n = x + g(y_{n+1})$. One first deduces that $x/y = 1 - \frac{g(y)}{y}$; since $y$ tends to $+\infty$ with $x$, the hypothesis $g(x) \ll x$ shows that $y = u(x) \sim x = y_0$; further,
$$
y - x = g(y) = g(x) + (y - x)g'(z)
$$
where $z$ belongs to the interval with endpoints $x, y$; when $x$ tends to $+\infty$ so does $z$, and since $g(x) \ll x$, $g' \ll 1$, thus $g'(z)$ tends to 0, and consequently
$$
y - x = g(x) + o(y - x)
$$

whence
$$
u(x) - x \sim g(x).
$$
(12)

In the second place we show, by recursion on $n$, that when $x$ tends to $+\infty$ one has $u_n \gg 1$, and
$$
u(x) - u_n(x) \ll u(x) - u_{n-1}(x).
$$
(13)

Indeed, $y - y_n = g(y) - g(y_{n-1}) = (y - y_{n-1})g'(z_{n-1})$, where $z_{n-1}$ belongs to the interval with endpoints $y$ and $y_{n-1}$; by the induction hypothesis $z_{n-1}$ tends to $+\infty$ with $x$, and so $g'(z_{n-1})$ tends to 0, which proves (13). One deduces from this relation and from (12) that $u(x) - u_n(x) \ll u(x) - x \sim g(x) \ll x \sim u(x)$, whence $u_n(x) \sim u(x)$ and consequently $u_n \gg 1$. Finally, the relation $u(x) - u_n(x) \ll u(x) - x$ can also be written $(u(x) - x) - (u_n(x) - x) \ll u(x) - x$, whence
$$
u_n(x) - x \sim u(x) - x \sim g(x).
$$
(14)

To prove (11), first remark that if $t(x)$ is a function such that $t(x) - x \sim g(x)$, then one has $g'(t(x)) \sim g'(x)$. Indeed, for any $\varepsilon > 0$, for $x$ sufficiently large $g'$ is monotone, so $g'(t(x))$ lies between $g'(x + (1 + \varepsilon)g(x))$ and $g'(x + (1 - \varepsilon)g(x))$. Prop. 4 of V, p. 255, shows that $g'(t(x)) \sim g'(x)$, provided one has established the relation $g \ll g'/g''$. Now, if $g$ is of infinite order relative to $x$ one has (V, p. 251, prop. 2) $g''/g' \sim g'/g$, and, since $g' \ll 1, g \ll g/g' \sim g'/g''$; if $g$ is of finite order $\mu$ relative to $x$ one necessarily has $\mu \leq 1$; if $\mu < 1$, since $g$ is not equivalent to a constant $\neq 0$, formulae (3) and (4) (V, p. 251) show that $g''/g' \sim k/x$ ($k$ constant $\neq 0$), whence again $g \ll g'/g''$; finally, if $\mu = 1$ then $g'$ is of order 0 relative to $x$, so $g''/g' \ll 1/x$, and so again $g \ll g'/g''$.

This being so, since $z_{n-1}$ lies between $y$ and $y_n$, it follows from (14) that $z_{n-1} - x \sim g(x)$, whence $g'(z_{n-1}) \sim g'(x)$ by the above; thus
$$
y - y_n \sim (y - y_{n-1})g'(x),
$$
whence we obtain (11) by induction on $n$.

#### Remark 1 {#fvr-v-a0-n6-rem-1 .statement}

If $g$ is of order $< 1$ relative to $x$, the function $u(x) - u_n(x)$ tends to 0 with $x$ once $n$ is sufficiently large. Indeed, in the opposite case one would have $g{g''}^n \gg 1$ for every $n$, so $g$ would be of infinite order relative to $1/g'$; in other words, one would have $\log|g| \gg \log|g'|$, whence, on differentiating, $g'/g \gg g''/g'$. But if $g$ is of order $\mu < 1$ relative to $x$ one has $g'/g \sim g''/g'$ when $\mu = -\infty, \frac{g'}{g} \sim \frac{\mu}{\mu - 1} \frac{g''}{g'}$ when $\mu \neq 0$, and finally $g'/g \ll g''/g'$ when $\mu = 0$ (V, p. 251, n 3).

In contrast, if $g$ is of order 1 relative to $x$ one can have $g{g''}^n \gg 1$ for every integer $n > 0$, as the example $g(x) = x/\log x$ shows.

#### Remark 2 {#fvr-v-a0-n6-rem-2 .statement}

When $g(x)$ is an (H) function equivalent to a constant $k \neq 0$ one has $g(x) = k + g_1(x)$, with $g_1 \ll 1$; the function $u_1(x) = u(x) - k$ is the inverse of the function $x - g_1(x + k)$, and one is brought back to the case treated in prop. 5 of V, p. 256.

To have an asymptotic expansion for the function $u$ it thus suffices to have such an expansion for the function $u_n$: if $g$ admits an asymptotic expansion relative to the scale under consideration one is thus led (by the definition of (H) functions) to the problems examined in V, p. 223 to 227.

The most general case, as follows, reduces to the case treated in prop. 5 of V, p. 256: the function $y = u(x)$ is assumed to satisfy the relation
$$
\varphi(x) = \psi(y) - g(y)
$$
where $\varphi$ is an (H) function, $\psi$ is an (H) function such that $\psi \gg 1$ and such that the inverse function $\theta$ of $\psi$ is also an (H) function, and $g$ is an (H) function such that $g \ll \psi$. Let now $v(x)$ be the inverse function of $x - g(\theta(x))$; one has $u = \theta \circ v \circ \varphi$, and $g(\theta(x)) \ll x$; if one knows an asymptotic expansion for $v$ thanks to prop. 5 of V, p. 256, one can then deduce an asymptotic expansion for $u$ as in V, p. 223 to 227.

#### Example 1 {#fvr-v-a0-n6-exa-1 .statement}

Let us seek an asymptotic expansion for the inverse function $v(x)$ of $x^5 + x$ (for $x$ tending to $+\infty$); putting $x^5 = t$ one is led to seek an expansion of the inverse function $u(t)$ of $t + t^{1/5}$ (for $t$ tending to $+\infty$), that is, to apply prop. 5 of V, p. 256, to the case where $g(t) = -t^{1/5}$. Let us, for example, calculate, $u_2(t)$; one has
$$
u_2(t) = t - \left( t - t^{1/5} \right)^{1/5} = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{2}{25} t^{-7/5} + o_1\left( t^{-7/5} \right).
$$
Moreover, by (11) (V, p. 256)
$$
u(t) - u_2(t) \sim -\frac{1}{25} t^{-7/5}
$$
whence
$$
u(t) = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{1}{25} t^{-7/5} + o_2\left( t^{-7/5} \right)
$$
and one deduces the expansion
$$
v(x) = u(x)^{1/5} = x^{1/5} - \frac{1}{5} x^{-3/5} - \frac{1}{25} x^{-7/5} + o_3\left( x^{-7/5} \right)
$$
sought.

#### Example 2 {#fvr-v-a0-n6-exa-2 .statement}

Let us seek an asymptotic expansion for the inverse function of the function $x / \log x$; from the identity $x = y / \log y$, where $y = v(x)$, one deduces $\log x = \log y - \log \log y$; on putting $z = \log y, t = \log x$, one has $t = z - \log z$, and one is led to expand the inverse function $u(t)$ of $t - \log t$; for example, one has
$$
u_2(t) = t + \log(t + \log t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + o_1\left( \frac{\log t}{t^2} \right)
$$
and moreover, by (11) (V, p. 256)
$$
u(t) - u_2(t) \sim \frac{\log t}{t^2}
$$
whence
$$
u(t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + \frac{\log t}{t^2} + o_2\left( \frac{\log t}{t^2} \right)
$$
and on returning to the original problem one obtains the asymptotic expansion
$$
v(x) = x \log x + x \log \log x + x \frac{\log \log x}{\log x} + o\left( x \frac{\log \log x}{\log x} \right).
$$

#### Remark {#fvr-v-a0-n6-rem-4 .statement}

Note that two equivalent (H) functions can have non-equivalent inverses, as the example of the two functions $\log x$ and $1 + \log x$ shows.

### Exercises {#fvr-v-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
