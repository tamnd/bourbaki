---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 0
section_title: Fonction de Möbius
appendix: true
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0069-0071, 0092-0092
extraction: ocr
statements: 1
exercises: 2
content_sha256: 50394ceb619d8b370d5388fb9364a8494f0bff50bd6fb54ee4604515552d338c
---

### APPENDICE Fonction de Möbius

Soit $n$ un entier $\geqslant 1$. Si $n$ est divisible par le carré d’un nombre premier, on pose $\mu(n) = 0$. Si $n$ n’est divisible par le carré d’aucun nombre premier, on pose $\mu(n) = (-1)^k$, où $k$ est le nombre de diviseurs premiers de $n$. La fonction $\mu : \mathbf{N}^* \to \{-1, 0, 1\}$ ainsi définie s’appelle fonction de Möbius.

Rappelons qu’étant donnés deux entiers $n_1 \geqslant 1, n_2 \geqslant 1$, on écrit $n_1 \mid n_2$ si $n_1$ divise $n_2$.

#### Proposition {#lie-ii-a0-n0-prop-1 .statement}

(i) La fonction $\mu$ est l’unique application de $\mathbf{N}^*$ dans $\mathbf{Z}$ telle que $\mu(1) = 1$ et que

$$
\sum_{d \mid n} \mu(d) = 0
$$

pour tout entier $n > 1$.

(ii) Soient $s$ et $t$ deux applications de $\mathbf{N}^*$ dans un groupe commutatif noté additivement. Pour que l’on ait

$$
s(n) = \sum_{d \mid n} t(d) \quad \text{pour tout entier } n \geqslant 1,
$$

il faut et il suffit que l’on ait

$$
t(n) = \sum_{d \mid n} \mu(d) s\left( \frac{n}{d} \right) \quad \text{pour tout entier } n \geqslant 1.
$$

L’assertion d’unicité dans (i) est évidente, car (1) permet de déterminer $\mu(n)$ par récurrence sur $n$. Montrons que la fonction $\mu$ satisfait bien à (1). En effet, soit $n$ un entier $> 1$. Soit $P$ l’ensemble des diviseurs premiers de $n$ et soit $n = \prod_{p \in P} p^{v_p(n)}$ la décomposition de $n$ en facteurs premiers. Si $d$ est un diviseur de $n$, on a $\mu(d) = 0$ sauf si $d$ est de la forme $\prod_{p \in \mathbf{H}} p$, où $\mathbf{H}$ est une partie de $\mathbf{P}$. On a donc

$$
\sum_{d|n} \mu(d) = \sum_{\mathbf{H} \subset \mathbf{P}} (-1)^{\mathrm{Card}\,\mathbf{H}}
$$
$$
= \sum_{k=0}^{\mathrm{Card}\,\mathbf{P}} \binom{n}{k}(-1)^k = (1 - 1)^{\mathrm{Card}\,\mathbf{P}} = 0.
$$

Soient $s$ et $t$ deux applications de $\mathbf{N}^*$ dans un groupe commutatif noté additivement. Soit $n \in \mathbf{N}^*$. Si (2) est vérifiée, on a

$$
\sum_{d|n} \mu(d)s\left(\frac{n}{d}\right) = \sum_{d|n} \mu(d) \sum_{\delta|\frac{n}{d}} t(\delta) = \sum_{d\delta|n} \mu(d)t(\delta)
$$
$$
= \sum_{\delta|n} t(\delta) \sum_{d|\frac{n}{\delta}} \mu(d) = t(n).
$$

Réciproquement, si (3) est vérifiée, on a

$$
\sum_{d|n} t(d) = \sum_{d|n} \sum_{\delta|d} \mu(\delta)s\left(\frac{d}{\delta}\right) = \sum_{d|n} s(d) \sum_{\delta|\frac{n}{d}} \mu(\delta) = s(n),
$$

ce qui achève la démonstration.

La formule (3) s'appelle *formule d'inversion de Möbius*.

Exercices

## EXERCICES {#lie-ii-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
