---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 2
section_title: EULERIAN EXPANSIONS OF THE TRIGONOMETRIC FUNCTIONS AND BERNOULLI NUMBERS
lang: en
source: fvr-i-vii
book_pages: 283-288, 292-296
pdf_pages: 0298-0303, 0307-0311
extraction: ocr
subsections:
    - "no": 1
      title: EULERIAN EXPANSION OF $\cot z$
      page: 283
      pdf_page: 298
    - "no": 2
      title: EULERIAN EXPANSION OF $\sin z$
      page: 286
      pdf_page: 301
    - "no": 3
      title: APPLICATION TO THE BERNOULLI NUMBERS
      page: 287
      pdf_page: 302
statements: 5
exercises: 6
content_sha256: c5c7d446dee9ba1fe3d1c893187a3788356b0388489f1ea77fdf68ea2831727a
---

## § 2. EULERIAN EXPANSIONS OF THE TRIGONOMETRIC FUNCTIONS AND BERNOULLI NUMBERS

### 1. EULERIAN EXPANSION OF $\cot z$

By formula (20) of VI, p. 275, the numbers $b_n / n!$ are the coefficients in the expansion of $S/(e^S - 1)$ as a *formal* series; we shall show in this section that the function $z/(e^z - 1)$ is equal to the sum of an absolutely convergent entire series on a neighbourhood of 0 in $\mathbf{C}$; it will follow from the lemma of VI, p. 280, that the coefficients of this series are the numbers $b_n / n!$, from which we shall deduce estimates for the Bernoulli numbers $b_n$.

In the first place we note that

$$
\frac{z}{e^z - 1} = - \frac{z}{2} + \frac{z}{2} \frac{e^z + 1}{e^z - 1} = - \frac{z}{2} + \frac{iz}{2} \cot \frac{iz}{2}.
$$ (1)

We shall obtain below a series expansion for $\cot z$, valid for every $z$ not an integer multiple of $\pi$.

#### Proposition 1 {#fvr-vi-s2-prop-1 .statement}

*For every complex number* $z$ *and every integer* $n$ *one has*

$$
\sin nz = 2^{n-1} \sin z \sin \left(z + \frac{\pi}{n}\right) \sin \left(z + \frac{2\pi}{n}\right) \ldots \sin \left(z + \frac{(n-1)\pi}{n}\right).
$$ (2)

Indeed, one can write

$$
\sin nz = \frac{e^{niz} - e^{-niz}}{2i} = \frac{e^{-niz}(e^{2niz} - 1)}{2i}
= \frac{e^{-niz}(e^{2iz} - 1)(e^{2iz} - e^{-2i\pi/n}) \ldots (e^{2iz} - e^{-2(n-1)i\pi/n})}{2i}
= A \sin z \sin \left( z + \frac{\pi}{n} \right) \sin \left( z + \frac{2\pi}{n} \right) \ldots \sin \left( z + \frac{(n-1)\pi}{n} \right)
$$

where
$$
A = (2i)^{n-1} e^{-\frac{i\pi}{n}(1+2+\ldots+(n-1))} = (2i)^{n-1} e^{-i(n-1)\frac{\pi}{2}} = 2^{n-1}.
$$

#### Corollary 1 {#fvr-vi-s2-prop-1-cor-1 .statement}

*For every integer n one has*
$$
\sin \frac{\pi}{n} \sin \frac{2\pi}{n} \ldots \sin \frac{(n-1)\pi}{n} = \frac{n}{2^{n-1}}.
$$
(3)

It suffices to divide both sides of (2) by $\sin z$ and let $z$ tend to 0.

#### Corollary 2 {#fvr-vi-s2-prop-1-cor-2 .statement}

*For every odd integer $n = 2m + 1$, and every complex number $z$ such that $nz$ is not an integral multiple of $\pi$, one has*
$$
\cot nz = (-1)^m \cot z \cot \left( z + \frac{\pi}{n} \right) \ldots \cot \left( z + \frac{(n-1)\pi}{n} \right).
$$
(4)

Indeed, $\sin n \left( z + \frac{\pi}{2} \right) = \sin \left( nz + \frac{\pi}{2} + m\pi \right) = (-1)^m \cos nz$, whence, replacing $z$ by $z + \frac{\pi}{2}$ in (2),

$$
\cos nz = (-1)^m 2^{n-1} \cos z \cos \left( z + \frac{\pi}{n} \right) \ldots \cos \left( z + \frac{(n-1)\pi}{n} \right)
$$
(5)

and the formulae (2) and (5) give (4) on division term-by-term when $\sin nz \neq 0$.

In all that follows we shall always assume that $n = 2m + 1$ is an odd integer; the formula (4) can also be written

$$
\cot nz = (-1)^m \prod_{k=-m}^{m} \cot \left( z - \frac{k\pi}{n} \right).
$$

or, one has

$$
\cot \left( z - \frac{k\pi}{n} \right) = \frac{1 + \tan z \tan \frac{k\pi}{n}}{\tan z - \tan \frac{k\pi}{n}}
$$

for tan z finite; cot $nz$ is thus a rational function in $u = \tan z$, whose numerator is of degree $n - 1$, and whose denominator, of degree $n$, has the $n$ simple roots $\tan k\pi / n$; decomposing this into simple fractions yields

$$
\cot nz = \sum_{k=-m}^{m} \frac{A_k}{u - \tan \frac{k\pi}{n}}
$$

where

$$
A_k = \lim_{z \to k\pi/n} \cot nz \left( \tan z - \tan \frac{k\pi}{n} \right) = \lim_{z \to k\pi/n} \frac{\cos nz}{\sin nz} \frac{\sin \left( z - \frac{k\pi}{n} \right)}{\cos z \cos \frac{k\pi}{n}}
$$
$$
= \lim_{h \to 0} \frac{\cos nh}{\cos \frac{k\pi}{n} \cos \left( h + \frac{k\pi}{n} \right)} \frac{\sin h}{\sin nh} = \frac{1}{n \cos^2 \frac{k\pi}{n}}
$$

whence, on isolating the term in (6) corresponding to $k = 0$ and combining the terms corresponding to opposite values of $k$, and replacing $z$ by $z/n$,

$$
\cot z = \frac{1}{n \tan \frac{z}{n}} + \sum_{k=1}^{m} \frac{2n \tan \frac{z}{n}}{\cos^2 \frac{k\pi}{n} \left( n \tan \frac{z}{n} \right)^2 - \left( n \sin \frac{k\pi}{n} \right)^2}
$$

valid for every complex number $z$ not an integral multiple of $\pi/2$. One can write this formula in the form

$$
\cot z = \frac{1}{n \tan \frac{z}{n}} + \sum_{k=1}^{\infty} v_k(n, z)
$$

with $v_k(n, z) = 0$ for $k > m$ and

$$
v_k(n, z) = \frac{2n \tan \frac{z}{n}}{\cos^2 \frac{k\pi}{n} \left( n \tan \frac{z}{n} \right)^2 - \left( n \sin \frac{k\pi}{n} \right)^2}
$$

for $1 \leq k \leq m$. We shall see that for every $z$ contained in a compact subset K of $\mathbf{C}$, not containing any integral multiple of $\pi$, and for every sufficiently large odd $n$, the series with general term $v_k(n, z)$ is normally convergent. Indeed, as $n$ tends to $+\infty$, $\tan \frac{z}{n}$ tends to $\frac{z}{n}$ uniformly on K, so there exists a number $M > 0$ such that $\left| n \tan \frac{z}{n} \right| \leq M$ for every sufficiently large $m$ and every $z \in K$. On the other hand, for $0 \leq x \leq \pi/2$ one has $\sin x / x \geq 1 - \frac{x^2}{6} \geq \frac{1}{2}$, so for $1 \leq k \leq m$ one has $n \sin \frac{k\pi}{n} \geq k\pi/2$; consequently, when $m$ is sufficiently large, for every integer $k$ such t $k\pi /2 > M$ one has $|v_k(n, z)| \leq \frac{8M}{k^2 \pi^2 - 4M^2}$, which proves our assertion. For $k$ odd, $v_k(n, z)$ tends (uniformly on K) to $\frac{2z}{z^2 - k^2 \pi^2}$ as $n$ tends to $+\infty$. Consequently:

#### Theorem 1 {#fvr-vi-s2-thm-1 .statement}

*For every complex number $z$ not an integral multiple of $\pi$ one has*

$$
\cot z = \frac{1}{z} + \sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}
$$

*(series on the right being normally convergent on every compact subset $K \subset \mathbf{C}$ containing any integer multiple of $\pi$ (Eulerian expansion of $\cot z$).)*

### 2. EULERIAN EXPANSION OF $\sin z$

For every *odd* integer $n = 2m + 1$ and complex $z$ the formula (2) of VI, p. 283, can be written

$$
\sin nz = (-1)^m 2^{n-1} \prod_{k=-m}^{m} \sin \left( z - \frac{k\pi}{n} \right)
$$
$$
= (-1)^m 2^{n-1} \sin z \prod_{k=1}^{m} \sin \left( z - \frac{k\pi}{n} \right) \sin \left( z + \frac{k\pi}{n} \right).
$$

Now, one has $\sin \left( z - \frac{k\pi}{n} \right) \sin \left( z + \frac{k\pi}{n} \right) = \sin^2 z - \sin^2 \frac{k\pi}{n}$, and, by (3) (VI, 284), $\prod_{k=1}^{m} \sin^2 \frac{k\pi}{n} = \frac{n}{2^{n-1}}$, whence, on replacing $z$ by $z/n$,

$$
\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} \left( 1 - \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}} \right).
$$

We can write this formula as $\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} (1 - w_k(n, z))$, with $w_k(n, z) = 0$ if $k > m$ and $w_k(n, z) = \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}}$ for $1 \leq k \leq m$. We shall see that for every $z$ contained in a compact subset $K$ of $\mathbf{C}$, and for $n$ odd, the series with general term $(n, z)$ is *normally convergent*. Indeed, as $n$ tends to $+\infty$, $n \sin \frac{z}{n}$ tends uniformly on $K$, so there exists a number $M > 0$ such that $\left| n \sin \frac{z}{n} \right| \leq M$ for every integer $n$ and every $z \in K$. We saw, moreover, in the proof of th. 1 of VI, p. 286, that for $1 \leq k \leq m$ one has $n \sin \frac{k \pi}{n} \geq \frac{k \pi}{2}$; thus for every integer $k$ such that $k \pi / 2 \geq M$ one has $|w_k(n, z)| \leq 4M^2 / k^2 \pi^2$, which proves our assertion. Since, for every fixed $k$, $w_k(n, z)$ tends (uniformly on K) to $z^2 / k^2 \pi^2$ as $n$ tends to $+\infty$, one sees that:

#### Theorem 2 {#fvr-vi-s2-thm-2 .statement}

For every complex number $z$ one has

$$
\sin z = z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2 \pi^2} \right)
$$

the infinite product on the right being absolutely and uniformly convergent on every compact subset of $\mathbf{C}$ (Eulerian expansion of $\sin z$).

### 3. APPLICATION TO THE BERNOULLI NUMBERS

Theorem 1 of VI, p. 286, shows that, for $0 \leq x < \pi$, the series with general term

$$
\frac{2x}{n^2 \pi^2 - x^2} \geq 0
$$

converges. On the other hand, one can write, for every complex number $z$ such that $|z| < \pi$,

$$
\frac{2z}{n^2 \pi^2 - z^2} = \frac{2z}{n^2 \pi^2} \sum_{k=0}^{\infty} \frac{z^{2k}}{n^{2k} \pi^{2k}}
$$

the series on the right being absolutely convergent. We shall deduce from this that the "double" series

$$
\sum_{n=1}^{\infty} \sum_{k=1}^{\infty} \frac{-2z^{2k-1}}{n^{2k} \pi^{2k}}
$$

is absolutely convergent in the open disc $|z| < \pi$, normally convergent on every compact set contained in this disc, and has sum $\cot z - \frac{1}{z}$. Indeed, for $|z| \leq a < \pi$ the absolute value of the general term of (11) is at most equal to $2a^{2k-1} / n^{2k} \pi^{2k}$, and the sum of any finite number of the terms $2a^{2k-1} / n^{2k} \pi^{2k}$ is less than the finite number $\sum_{n=1}^{\infty} \frac{2a}{n^2 \pi^2 - a^2}$; on summing first over $k$, then over $n$, one sees that the sum of the series (11) is equal to $\sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}$, which proves our statement.

If now one sums the series (11) first over $n$ and then over $k$ one obtains the identity (for $|z| < \pi$)

$$
\cot z - \frac{1}{z} = -2 \sum_{k=1}^{\infty} \frac{S_{2k}}{\pi^{2k}} z^{2k-1}
$$

where we have put $S_k = \sum_{n=1}^{\infty} \frac{1}{n^k}$. By (1) (VI, p. 283) one thus has, for $|z| < 2\pi$ whence we obtain the formula

$$
b_{2n} = (-1)^{n-1} (2n)! \frac{2 S_{2n}}{(2\pi)^{2n}} \quad \text{for } n \geq 1,
$$

a formula which shows in particular that the numbers $S_{2n}/\pi^{2n}$ are *rational*. Clearly $S_{k+1} \leq S_k$ so, for every integer $k \geq 2$, we have $S_k \leq S_2 = \pi^2/6 \leq 2$; from (14) one deduces the following inequalities for the Bernoulli numbers

$$
\frac{2 (2n)!}{(2\pi)^{2n}} \leq |b_{2n}| \leq 4 \frac{(2n)!}{(2\pi)^{2n}} \quad \text{for } n \geq 1.
$$

From these inequalities one can deduce an estimate for the Bernoulli polynomial

$$
B_n(x) = \sum_{k=0}^n \binom{n}{k} b_k x^{n-k}; \text{ in particular, for } 0 \leq x \leq 1 \text{ one has}
$$

$$
|B_n(x)| \leq 4 \sum_{k=0}^n \binom{n}{k} \frac{k!}{(2\pi)^k} = 4 \frac{n!}{(2\pi)^n} \sum_{k=0}^n \frac{(2\pi)^k}{k!} \leq 4 e^{2\pi} \frac{n!}{(2\pi)^n}.
$$

### Exercises {#fvr-vi-s2-exercises}

See the [exercises for § 2](exercises/s2/).
