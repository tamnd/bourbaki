---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 0
section_title: Möbius function
appendix: true
lang: zh
source: lie-i-iii
book_pages: 176-177, 207
pdf_pages: 0194-0195, 0225-0225
extraction: ocr
statements: 1
exercises: 2
content_sha256: b10df09d6e54ef52981129817d465f52176bd3bc06a679e855c4d7cf835be503
translated_from: content/en/lie/II/A_a_mobius_function.md
translation_method: google
source_content_sha256: c54ffb7970e587f4343ab39ca3824bf23f6f7cf1e3a847c72dd475d033916502
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 338b57e4f57385e17e37d7cd6b715298277321127c803cf39cec7d7898d9f7da
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 附录

# 莫比乌斯函数

令 n 为整数 $\geq 1$。如果 n 能被素数数的平方整除，我们就写成 $\mu(n) = 0$。如果 n 不能被素数数的平方整除，则写为 $\mu(n) = (-1)^k$，其中 k 是 n 的素数除子的数。这样定义的函数$\mu : \mathbf{N}^* \to \{-1, 0, 1\}$称为莫比乌斯函数。

回想一下，给定两个整数 $n_1 \geq 1, n_2 \geq 1$，如果 $n_1$ 除 $n_2$，我们就写 $n_1 | n_2$。

#### 命题 {#lie-ii-a0-n0-prop-1 .statement tag=0A73}

(i) *函数 $\mu$ 是 $\mathbf{N}^*$ 的唯一映射到 $\mathbf{Z}$，使得 $\mu(1) = 1$ 并且*
$$
\sum_{d|n} \mu(d) = 0
$$
*每整数$n > 1$。*

(ii) *令 s 和 t 为 $\mathbf{N}^*$ 中的两个映射成为可加的交换律群。在阶*
$$
s(n) = \sum_{d|n} t(d) \quad \text{for every integer } n \geq 1,
$$
*这是必要且充分的*
$$
t(n) = \sum_{d|n} \mu(d) s\left(\frac{n}{d}\right) \quad \text{for every integer } n \geq 1.
$$

(i) 中的唯一性断言是显而易见的，因为 (1) 允许我们在 n 上通过归纳确定 $\mu(n)$。我们证明函数 $\mu$ 满足 (1)。令 n 为整数 $> 1$。设P为n的素数除子的集合，并令$n = \prod_{p \in P} p^{\nu_p(n)}$为n的分解到素数因子。如果 d 是 n 的除子，则 $\mu(d) = 0$ 除非 d 是形式 $\prod_{p \in H} p$，其中 H 是 P 的子集。则
$$
\sum_{d|n} \mu(d) = \sum_{H \subset P} (-1)^{\mathrm{Card}\ H}
= \sum_{k=0}^{\mathrm{Card}\ P} \binom{n}{k} (-1)^k = (1 - 1)^{\mathrm{Card}\ P} = 0.
$$

设 s 和 t 是 $\mathbf{N}^*$ 的两个映射到可加写的交换式群中。让$n \in \mathbf{N}^*$。如果(2)成立，则
$$
\sum_{d|n} \mu(d)s\left(\frac{n}{d}\right) = \sum_{d|n} \mu(d) \sum_{\delta|(n/d)} t(\delta) = \sum_{d|n} \mu(d)t(\delta)
$$
$$
= \sum_{\delta|n} t(\delta) \sum_{d|(n/\delta)} \mu(d) = t(n).
$$
反之，如果(3)成立，则
$$
\sum_{d|n} t(d) = \sum_{d|n} \sum_{\delta|d} \mu(\delta)s\left(\frac{d}{\delta}\right) = \sum_{d|n} s(d) \sum_{\delta|(n/d)} \mu(\delta) = s(n),
$$
完成证明。

公式 (3) 称为莫比乌斯反演公式。

### 习题 {#lie-ii-a0-exercises}

参见[习题附录 0](exercises/a0/)。
