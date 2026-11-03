---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 3
section_title: BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA
lang: zh
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
content_sha256: ab6a93ee740e4b12cc5d278beaa1b902ad87e6edd56914de2ec1509c367f19d3
translated_from: content/en/fvr/VI/03_s3_bounds_for_the_remainder_in_the_euler.md
translation_method: google
source_content_sha256: 0df8d05b12ca6ce3b68cbd660e6b590830aa5e44eda3d489241375154aaa1723
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 93fdb5a4c483a9289a83df8c8f061b213407d5bf942d9a9a853ea5815fe8c84c
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。欧拉-麦克劳林求和公式中余数的界限

### 1. 欧拉-麦克劳林求和公式中余数的界限

(16) 中对区间 $[0, 1]$ 的伯努利多项式获得的估计允许人们轻松估计欧拉-麦克劳林求和公式 (VI, p. 282, 公式 (39)) 中的余数 $T_p(x, n)$：

$$
\left\{
\begin{array}{l}
f(x) + f(x+1) + \cdots + f(x+n) \\
\phantom{=} = \int_x^{x+n+1} f(t)\,dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
\phantom{=} \phantom{=} + \sum_{k=1}^p \frac{b_{2k}}{(2k)!} (f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x)) + T_p(x, n).
\end{array}
\right.
$$

事实上，有 (VI, p. 283, 公式 (41))

$$
T_p(x, n) = -\frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1-s) f^{(2p+1)}(x+s)\,ds
$$

其中$\overline{B}_{2p+1}(t)$是周期1的周期函数等于区间$[0, 1[$上的$B_{2p+1}(t)$。 VI、p. 288 的公式 (16) 表明

$$
|\overline{B}_{2p+1}(t)| \leq 4e^{2\pi} \frac{(2p+1)!}{(2\pi)^{2p+1}}
$$
(3)

对于所有 $t \in \mathbf{R}$ 和应用，平均值公式给出估计值

$$
|T_p(x, n)| \leq \frac{4e^{2\pi}}{(2\pi)^{2p+1}} \int_x^{x+n+1} |f^{(2p+1)}(t)| \, dt
$$
(4)

对于$T_p(x, n)$。

### 2. 应用于渐近展开

欧拉-麦克劳林公式允许人们给出更完整的解（在最重要的情况下）到V，p. 238到242中处理的问题，即获得部分和$s_n = \sum_{m=0}^n g(m)$（分别是余数）的渐近展开 $r_n = \sum_{m=n+1}^\infty g(m)$)，其中$g$是标量函数、$> 0$，单调，在$[0, +\infty[$上定义。

我们将仅限于$g$是阶0相对于$e^x$的(H)函数(V,p. 252)；在其他字中，有一个有关系$g' \ll g$；由此关系可以为每个整数 $k > 0$ 推出 $g^{(k+1)} \ll g^{(k)}$，使得阶 $h \leq k$ 的导数 $g^{(h)}$ 都不等于常数（V、p. 232，命题 7）。令$p$为整数，使得阶$h \leq 2p$的导数$g^{(h)}$都不等于常数。首先我们假设级数与一般的项$g(n)$有无穷大的和，并区分几种情况：

1. $|g^{(2p-1)}(n)|$与$n$趋于$+\infty$；我们有相同的，到假设，对于$|g^{(2k-1)}(n)|$对于$1 \leq k \leq p$；进一步，由于$g^{(2p+1)}$在$+\infty$的邻域上单调，VI、p. 289的公式 (4)，给出$T_p(0, n) = O(g^{(2p)}(n+1)) = o(g^{(2p-1)}(n+1))$；欧拉-麦克劳林公式，应用于$x = 0$，表明

$$
s_n = \sum_{m=0}^n g(m) = \int_0^{n+1} g(t) \, dt - \frac{1}{2} g(n+1)
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} g^{(2k-1)}(n+1) + o(g^{(2p-1)}(n+1))
$$

该和中的每一个项相对于前一个都可以忽略不计；将它们中的每一个相对于比较尺度 $\mathscr{E}$ 进行扩展，就会得到 $s_n$ 的渐近展开。

2) 现在假设对于指标$q$，使得$1 \leq q \leq p$我们有$|g^{(2q-1)}(n)|$趋向于$+\infty$和$n$，但对于$k > q$$g^{(2k-1)}(n)$趋于0。由于$g^{(2p+1)}$在$+\infty$的邻域上是单调的，因此积分$\int_0^\infty |g^{(2p+1)}(u)| \, du$收敛，然后可以写出

$$
s_n = \sum_{m=0}^{n} g(m) = \int_0^{n+1} g(t)\,dt - \frac{1}{2}g(n+1) + \sum_{k=1}^{q} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + C
$$
$$
+ \sum_{k=q+1}^{p} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + o\left(g^{(2p-1)}(n+1)\right)
$$

其中 C 是一个常数：确实

$$
\int_{n+1}^{\infty} |g^{(2p+1)}(u)|\,du = O\left(g^{(2p)}(n+1)\right) = o\left(g^{(2p-1)}(n+1)\right).
$$

同样，当$g(n)$自身趋于0时，公式有效。最后，当级数与一般项$g(n)$收敛时，对于余数$r_n = \sum_{m=n+1}^{\infty} g(m)$，展开

$$
r_n = \sum_{m=n+1}^{\infty} g(m) = \int_{n+1}^{\infty} g(t)\,dt + \frac{1}{2}\,g(n+1)
$$
$$
- \sum_{k=1}^{p} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + o\left(g^{(2p-1)}(n+1)\right).
$$

### 习题{#fvr-vi-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
