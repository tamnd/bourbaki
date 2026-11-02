---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 3
section_title: BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA
lang: ja
source: fvr-i-vii
book_pages: 288-290, 296-297
pdf_pages: 0303-0305, 0311-0312
extraction: ocr
subsections:
    - "no": 1
      title: BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA
      page: 288
      pdf_page: 303
    - "no": 2
      title: APPLICATION TO ASYMPTOTIC EXPANSIONS
      page: 289
      pdf_page: 304
statements: 0
exercises: 3
content_sha256: b9271defb112d0998857ccf7dac6526cf859634bf01dbaf425dcec2ab30679ce
translated_from: content/en/fvr/VI/03_s3_bounds_for_the_remainder_in_the_euler.md
translation_method: google
source_content_sha256: 0df8d05b12ca6ce3b68cbd660e6b590830aa5e44eda3d489241375154aaa1723
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 54dd293b1d7a75ea7f775f9bae1292ce88091bbd14a132889252198ed00bd4de
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。オイラー-マクローリン和の剰余の範囲公式

### 1. オイラー-マクローリン和の剰余の範囲公式

区間 $[0, 1]$ のベルヌーイ多項式について (16) で得られた推定により、オイラー・マクローリン和公式 (VI, p. 282, 公式 (39)) の剰余 $T_p(x, n)$ を簡単に推定できます。

$$
\left\{
\begin{array}{l}
f(x) + f(x+1) + \cdots + f(x+n) \\
\phantom{=} = \int_x^{x+n+1} f(t)\,dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
\phantom{=} \phantom{=} + \sum_{k=1}^p \frac{b_{2k}}{(2k)!} (f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x)) + T_p(x, n).
\end{array}
\right.
$$

確かに、(VI, p. 283, 公式 (41)) があります。

$$
T_p(x, n) = -\frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1-s) f^{(2p+1)}(x+s)\,ds
$$

ここで、$\overline{B}_{2p+1}(t)$ は、区間 $[0, 1[$ の $B_{2p+1}(t)$ に等しい期間 1 の周期写像です。 VI、p. 288 の公式 (16) は、次のことを示しています。

$$
|\overline{B}_{2p+1}(t)| \leq 4e^{2\pi} \frac{(2p+1)!}{(2\pi)^{2p+1}}
$$
(3)

すべての $t \in \mathbf{R}$ と適用の平均値公式が推定値を与えます

$$
|T_p(x, n)| \leq \frac{4e^{2\pi}}{(2\pi)^{2p+1}} \int_x^{x+n+1} |f^{(2p+1)}(t)| \, dt
$$
(4)

$T_p(x, n)$の場合。

### 2. 漸近展開への応用

オイラー・マクローリン公式を使用すると、V、p. 238 から 242 で扱われる、より完全な解 (最も重要な場合) から問題を与えることができ、部分的な和 $s_n = \sum_{m=0}^n g(m)$ (それぞれの剰余の漸近展開) を得ることができます。 $r_n = \sum_{m=n+1}^\infty g(m)$)、ここで、$g$ は、$[0, +\infty[$ で定義されたスカラー 写像、$> 0$、単調です。

$g$ が $e^x$ に対する位数 0 の (H) 写像 (V, p. 252) である場合に限定します。他の語には関係 $g' \ll g$ があります。この関係から、整数 $k > 0$ ごとに $g^{(k+1)} \ll g^{(k)}$ が推定され、位数 $h \leq k$ の導関数 $g^{(h)}$ は定数 (V、p. 232、定数 7) に等価ではありません。 $p$ を整数とし、位数 $h \leq 2p$ の導関数 $g^{(h)}$ が定数に等しくないようにします。 まず、系列と一般的な項 $g(n)$ が無限の和を持つと仮定し、いくつかのケースを区別します。

1. $|g^{(2p-1)}(n)|$ は $n$ では $+\infty$ になる傾向があります。 仮定までに、$|g^{(2k-1)}(n)|$、$1 \leq k \leq p$までに同じものがあります。さらに、$g^{(2p+1)}$は$+\infty$の近傍で単調なので、VI、p. 289の公式の(4)は$T_p(0, n) = O(g^{(2p)}(n+1)) = o(g^{(2p-1)}(n+1))$を与えます。 $x = 0$ に適用されたオイラー・マクローリン公式は、次のことを示しています。

$$
s_n = \sum_{m=0}^n g(m) = \int_0^{n+1} g(t) \, dt - \frac{1}{2} g(n+1)
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} g^{(2k-1)}(n+1) + o(g^{(2p-1)}(n+1))
$$

この和のそれぞれの項は、前の和に比べて無視できます。比較スケール $\mathscr{E}$ に対してそれぞれを拡張すると、$s_n$ の漸近拡張が得られます。

2) 次に、$1 \leq q \leq p$ のような添字 $q$ について、$n$ では $|g^{(2q-1)}(n)|$ が $+\infty$ になる傾向があるが、$k > q$ では $g^{(2k-1)}(n)$ が 0 になる傾向があるとします。 $g^{(2p+1)}$ は $+\infty$ の近傍で単調であるため、積分 $\int_0^\infty |g^{(2p+1)}(u)| \, du$ は収束し、次のように書くことができます。

$$
s_n = \sum_{m=0}^{n} g(m) = \int_0^{n+1} g(t)\,dt - \frac{1}{2}g(n+1) + \sum_{k=1}^{q} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + C
$$
$$
+ \sum_{k=q+1}^{p} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + o\left(g^{(2p-1)}(n+1)\right)
$$

ここで、C は定数です: 確かに

$$
\int_{n+1}^{\infty} |g^{(2p+1)}(u)|\,du = O\left(g^{(2p)}(n+1)\right) = o\left(g^{(2p-1)}(n+1)\right).
$$

$g(n)$ 自体が 0 になる傾向がある場合にも、同じ公式が有効です。最後に、系列と一般的な項 $g(n)$ が収束すると、残りの $r_n = \sum_{m=n+1}^{\infty} g(m)$ について、次の展開が得られます。

$$
r_n = \sum_{m=n+1}^{\infty} g(m) = \int_{n+1}^{\infty} g(t)\,dt + \frac{1}{2}\,g(n+1)
$$
$$
- \sum_{k=1}^{p} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + o\left(g^{(2p-1)}(n+1)\right).
$$

### 練習問題 {#fvr-vi-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
