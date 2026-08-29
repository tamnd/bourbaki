---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 0
section_title: Möbius function
appendix: true
lang: en
source: lie-i-iii
book_pages: 176-177, 207
pdf_pages: 0194-0195, 0225-0225
extraction: ocr
statements: 1
exercises: 2
content_sha256: 035e755d266fe3a54e74dc905de768808e16a07832a5d5f8c3e45b46b8b2c762
---

## APPENDIX

# MÖBIUS FUNCTION

Let n be an integer $\geq 1$. If n is divisible by the square of a prime number, we write $\mu(n) = 0$. If n is not divisible by the square of a prime number, we write $\mu(n) = (-1)^k$, where k is the number of prime divisors of n. The function $\mu : \mathbf{N}^* \to \{-1, 0, 1\}$ thus defined is called the Möbius function.

Recall that given two integers $n_1 \geq 1, n_2 \geq 1$, we write $n_1 | n_2$ if $n_1$ divides $n_2$.

#### Proposition {#lie-ii-a0-n0-prop-1 .statement}

(i) *The function $\mu$ is the unique mapping of $\mathbf{N}^*$ into $\mathbf{Z}$ such that $\mu(1) = 1$ and*
$$
\sum_{d|n} \mu(d) = 0
$$
*for every integer $n > 1$.*

(ii) *Let s and t be two mappings of $\mathbf{N}^*$ into a commutative group written additively. In order that*
$$
s(n) = \sum_{d|n} t(d) \quad \text{for every integer } n \geq 1,
$$
*it is necessary and sufficient that*
$$
t(n) = \sum_{d|n} \mu(d) s\left(\frac{n}{d}\right) \quad \text{for every integer } n \geq 1.
$$

The uniqueness assertion in (i) is obvious, for (1) allows us to determine $\mu(n)$ by induction on n. We show that the function $\mu$ satisfies (1). Let n be an integer $> 1$. Let P be the set of prime divisors of n and let $n = \prod_{p \in P} p^{\nu_p(n)}$ be the decomposition of n into prime factors. If d is a divisor of n, then $\mu(d) = 0$ unless d is of the form $\prod_{p \in H} p$, where H is a subset of P. Then
$$
\sum_{d|n} \mu(d) = \sum_{H \subset P} (-1)^{\mathrm{Card}\ H}
= \sum_{k=0}^{\mathrm{Card}\ P} \binom{n}{k} (-1)^k = (1 - 1)^{\mathrm{Card}\ P} = 0.
$$

Let s and t be two mapping of $\mathbf{N}^*$ into a commutative group written additively. Let $n \in \mathbf{N}^*$. If (2) holds, then
$$
\sum_{d|n} \mu(d)s\left(\frac{n}{d}\right) = \sum_{d|n} \mu(d) \sum_{\delta|(n/d)} t(\delta) = \sum_{d|n} \mu(d)t(\delta)
$$
$$
= \sum_{\delta|n} t(\delta) \sum_{d|(n/\delta)} \mu(d) = t(n).
$$
Conversely, if (3) holds, then
$$
\sum_{d|n} t(d) = \sum_{d|n} \sum_{\delta|d} \mu(\delta)s\left(\frac{d}{\delta}\right) = \sum_{d|n} s(d) \sum_{\delta|(n/d)} \mu(\delta) = s(n),
$$
which completes the proof.

Formula (3) is called the Möbius inversion formula.

### Exercises {#lie-ii-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
