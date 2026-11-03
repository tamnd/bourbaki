---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 0
section_title: Möbius function
appendix: true
lang: ja
source: lie-i-iii
book_pages: 176-177, 207
pdf_pages: 0194-0195, 0225-0225
extraction: ocr
statements: 1
exercises: 2
content_sha256: 2d723bbb6381a6533a7323375e8d328152872276c8d13470abeadb08dc24aac1
translated_from: content/en/lie/II/A_a_mobius_function.md
translation_method: google
source_content_sha256: c54ffb7970e587f4343ab39ca3824bf23f6f7cf1e3a847c72dd475d033916502
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0987054d7eabb0f1853a8ce71fc3e9bb8c9e6a508a16d116f74f3af28bf1f52a
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録

# メビウス写像

n を整数 $\geq 1$ とします。 n が素数数の平方で割り切れる場合、$\mu(n) = 0$ と書きます。 n が素数数の平方で割り切れない場合は、 $\mu(n) = (-1)^k$ と書きます。ここで、k は n の素数因子の数です。このように定義された写像 $\mu : \mathbf{N}^* \to \{-1, 0, 1\}$ をメビウス写像と呼びます。

2 つの整数 $n_1 \geq 1, n_2 \geq 1$ が与えられた場合、$n_1$ 割る $n_2$ であれば $n_1 | n_2$ と書くことを思い出してください。

#### 命題 {#lie-ii-a0-n0-prop-1 .statement tag=0A73}

(i) *写像 $\mu$ は、$\mathbf{N}^*$ の一意な写像を $\mathbf{Z}$ に変換し、$\mu(1) = 1$ となり、*
$$
\sum_{d|n} \mu(d) = 0
$$
*整数 $n > 1$ごとに。*

(ii) *s と t を $\mathbf{N}^*$ の 2 つの写像を加法的に書いた可換群にします。 位数では*
$$
s(n) = \sum_{d|n} t(d) \quad \text{for every integer } n \geq 1,
$$
*それは必要かつ十分です*
$$
t(n) = \sum_{d|n} \mu(d) s\left(\frac{n}{d}\right) \quad \text{for every integer } n \geq 1.
$$

(i) の一意性主張は明らかです。(1) により、n 上の帰納法によって決定する $\mu(n)$ が可能になります。 写像 $\mu$ が (1) を満たすことを示します。 n を整数 $> 1$ とします。 P を n の素数因子の集合とし、$n = \prod_{p \in P} p^{\nu_p(n)}$ を n の素数因子の分解とします。 d が n の因子である場合、 $\mu(d) = 0$ 〜でない限り d は形 $\prod_{p \in H} p$ であり、H は P の部分集合です。
$$
\sum_{d|n} \mu(d) = \sum_{H \subset P} (-1)^{\mathrm{Card}\ H}
= \sum_{k=0}^{\mathrm{Card}\ P} \binom{n}{k} (-1)^k = (1 - 1)^{\mathrm{Card}\ P} = 0.
$$

s と t を $\mathbf{N}^*$ の 2 つの写像を加法的に書かれた可換群とします。 $n \in \mathbf{N}^*$ にしましょう。 (2) が成立する場合、
$$
\sum_{d|n} \mu(d)s\left(\frac{n}{d}\right) = \sum_{d|n} \mu(d) \sum_{\delta|(n/d)} t(\delta) = \sum_{d|n} \mu(d)t(\delta)
$$
$$
= \sum_{\delta|n} t(\delta) \sum_{d|(n/\delta)} \mu(d) = t(n).
$$
逆に、(3) が成り立つ場合は、
$$
\sum_{d|n} t(d) = \sum_{d|n} \sum_{\delta|d} \mu(\delta)s\left(\frac{d}{\delta}\right) = \sum_{d|n} s(d) \sum_{\delta|(n/d)} \mu(\delta) = s(n),
$$
これで証明が完了します。

公式 (3) はメビウス反転公式と呼ばれます。

### 練習問題 {#lie-ii-a0-exercises}

[練習問題付録 0](exercises/a0/)を参照してください。
