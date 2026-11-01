---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 3
section_title: DERIVATIVES OF HIGHER ORDER
lang: zh
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
content_sha256: 59e86e5eabf944f58579cf0fa3cf103487a37052eeee2555615052e4617c1751
translated_from: content/en/fvr/I/03_s3_derivatives_of_higher_order.md
translation_method: google
source_content_sha256: 699d9104f5cbf89e2acd64f1b847b3d92cb37baff716a8c7f28471e185a92054
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 465578c1f400db2decb7ec6d6473a3279340d8f014e6382925148893e5337bff
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 3。高阶阶的衍生物

### 1. 阶 $n$ 的衍生物

令 $f$ 为实数变量的向量函数，定义、连续且在区间 $I$ 上可微。如果导数$f'$存在于点$x_0 \in I$的邻域（相对于$I$），并且在点$x_0$可微，则其导数称为$f$在点$x_0$的*二阶导数*，并且用$f''(x_0)$或$D^2f(x_0)$表示。如果这个二阶导数存在于$I$的每一个点处（这意味着$f'$存在并且在$I$上连续），那么$x \mapsto f''(x)$就是向量函数，用$f''$或$D^2f$表示。我们定义，以同样的方式，递归地得到$f$的$n^{th}$*导数*（或*阶*$n$的导数），并用$f^{(n)}$或$D^n f$表示；由定义，它在点$x_0 \in I$的值是函数$f^{(n-1)}$在点$x_0$的导数：这个定义预设*所有*导数$f^{(k)}$的存在阶$k \leq n - 1$在$x_0$相对于$I$的*邻域*上，以及$f^{(n-1)}$在点$x_0$的可微性。

We will say that $f$ is *n times differentiable* at the point $x_0$ (resp. in an interval) if it admits an $n^{th}$ derivative at this point (resp. in this interval). 有人说，如果对于每个整数$n > 0$，它承认阶$n$在$I$上的导数，那么$f$在$I$上“无限可微”。

在 $m$ 归纳时，人们看到了这一点

$$
D^m(D^n f) = D^{m+n} f.
$$

更准确地说，当(1)中的两个项之一被定义时，另一个也被定义，并且等于它。

#### 命题 1 {#fvr-i-s3-prop-1 .statement tag=084Y}

*The set of vector functions defined on an interval* $I \subset \mathbf{R}$, *taking values in a given topological vector space* $E$, *and having an* $n^{th}$ *derivative on* $I$, *is a vector space over* $\mathbf{R}$, *and* $f \mapsto D^n f$ *is a linear mapping of this space into the vector space of linear mappings from* $I$ *into* $E$.

证明公式

$$
D^n(f + g) = D^n f + D^n g \tag{2}
$$
$$
D^n(fa) = D^n f . a \tag{3}
$$

当$f$和$g$在$I$上有$n^{th}$导数（$a$为常数）时，在$n$上乘以归纳。

#### 命题 2（“莱布尼兹”公式”）{#fvr-i-s3-prop-2 .statement tag=084Z}

*设*$E, F, G$*是*$\mathbf{R}$、*和*$(x, y) \mapsto [x.y]$*的三个拓扑向量空间*$E \times F$*的连续双线性映射*到*$G$。 *如果* $f$ *(分别* $g$) *在区间* $I \subset \mathbf{R}$上定义，*将其值放入* $E$ *(分别* $F$) *并且有一个* $n^{th}$ *右* $I$求导，*那么* $[f.g]$ *有一个* $n^{th}$ *右* $I$的导数，*由公式*给出

$$
D^n[f.g] = [f^{(n)}.g] + \binom{n}{1}[f^{(n-1)}.g'] + \cdots + \binom{n}{p}[f^{(n-p)}.g^{(p)}] + \cdots + [f.g^{(n)}]. \tag{4}
$$

公式 (4) 由归纳在 $n$ 上证明（使用关系 $\binom{n}{p} = \binom{n-1}{p} + \binom{n-1}{p-1}$ 作为二项式系数）。

以同样的方式可以验证以下公式（其中假设与命题2相同）：

$$
[f^{(n)} . g] + (-1)^{n-1} [f . g^{(n)}] = D([f^{(n-1)} . g] - [f^{(n-2)} . g'] + \cdots + (-1)^{n-1} [f . g^{(n-1)}]).
$$

前面的命题已经被表述为函数在一个区间上可微 $n$ 倍；我们留给读者来制定函数的类似命题，其在点处可微 $n$ 倍。

### 2. 泰勒公式

令 $f$ 为向量函数，定义在区间 $I \subset \mathbf{R}$ 上，值位于$\mathbf{R}$ 的 *范数* 空间 $E$ 内；说 $f$ 在点 $a \in I$ 处有导数表示

$$
\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)(x-a)}{x-a} = 0;
$$

或者，否则，$f$“大约等于”$a$的邻域上的*线性*函数$f(a) + f'(a)(x-a)$（*cf.*章节V，其中这个概念是以一般方式发展的）。我们将看到，$f$在点$a$的$n^{th}$阶导数的存在同样意味着$f$“约等于”次数$n$的*多项式$x$*，系数位于 $a$ 邻域上的$E$（*Gen.Top.*、X、p. 315）。准确地说：

#### 定理 1 {#fvr-i-s3-thm-1 .statement tag=0850}

*如果函数$f$在点$a$有$n^{th}$导数，那么*

$$
\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - \cdots - f^{(n)}(a)\frac{(x-a)^n}{n!}}{(x-a)^n} = 0.
$$

我们于 $n$ 乘归纳出发。 定理适用于 $n = 1$。对于任意$n$，我们可以通过归纳假设，将其应用于$f$的导数$f'$：对于任何$\varepsilon > 0$，都存在一个$h > 0$，这样，如果有人将

$$
g(x) = f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - f''(a)\frac{(x-a)^2}{2!} - \cdots - f^{(n)}(a)\frac{(x-a)^n}{n!}
$$

对于 $|y-a| \leq h$ 和 $y \in I$，

$$
\|g'(y)\| = \left\| f'(y) - f'(a) - f''(a)\frac{(y-a)}{1!} - \cdots - f^{(n)}(a)\frac{(y-a)^{n-1}}{(n-1)!} \right\|
$$
$$
\leq \varepsilon\ |y-a|^{n-1}.
$$

我们将平均值值定理 (I, p. 15, th.2) 应用到端点 $a,\ x$（$|x-a| \leq h$）到向量函数 $g$ 以及实数递增的区间上如果$x > a$则函数等于$\varepsilon |y - a|^n / n$，如果$x < a$则等于$-\varepsilon |y - a|^n / n$；由此可知$\|g(x)\| \leq \varepsilon |x - a|^n / n$，从而证明定理。

因此我们可以写
$$
f(x) = f(a) + f'(a) \frac{(x - a)}{1!} + f''(a) \frac{(x - a)^2}{2!} + \cdots \\
+ f^{(n)}(a) \frac{(x - a)^n}{n!} + u(x) \frac{(x - a)^n}{n!}
$$
其中当$x$接近$a$时，$u(x)$接近0，同时保持在I；这个公式在点$a$称为阶*$n$的*泰勒公式，而(8)的右边称为阶*$n$的*泰勒展开函数$f$在点$a$。最后一个项$r_n(x) = u(x)(x - a)^n / n!$称为阶$n$的泰勒公式中的*余数*。

当$f$在I上有阶* $n + 1$的*导数时，可以在所有I上，而不仅仅是在$a$的未指定的邻域上，估计该$n + 1^{th}$导数的项中的$\|r_n(x)\|$：

#### 命题 3 {#fvr-i-s3-prop-3 .statement tag=0851}

*如果$\|f^{(n+1)}(x)\| \leq M$在I上，那么我们有*
$$
\|r_n(x)\| \leq M \frac{|x - a|^{n+1}}{(n + 1)!}
$$
*在*I。

事实上，公式对于$n = 0$成立，乘以I，p. 15，th。 2. 让我们用归纳在$n$上证明：通过归纳假设应用于$f'$，有
$$
\|r'_n(y)\| \leq M \frac{|y - a|^n}{n!}
$$
其中公式 (9) 遵循平均值值定理 (I, p. 23, th. 2)。

#### 推论{#fvr-i-s3-n2-cor-1 .statement tag=0852}

*如果 $f$ 是有限实数函数，且具有阶* $n + 1$ *在* I 上的导数，*且如果* $m \leq f^{(n+1)}(x) \leq M$ *在* I 上，*则对于所有* $x \geq a$ *在* I *其中一个有*
$$
m \frac{(x - a)^{n+1}}{(n + 1)!} \leq r_n(x) \leq M \frac{(x - a)^{n+1}}{(n + 1)!}
$$
*并且第二个项不能等于第一个*（分别*第三个*）*除非*$f^{(n+1)}$*是常数并等于*$m$（分别$M$）*在区间*$[a, x]$。

证明以同样的方式进行，但应用 th。 1 个I、p. 14。

#### 注 1 {#fvr-i-s3-n2-rem-1 .statement tag=0853}

我们已经在第证明注意到了。 1 如果$f$在I上有阶$n$的导数，并且如果
$$
f(x) = a_0 + a_1(x - a) + a_2(x - a)^2 + \cdots + a_n(x - a)^n + r_n(x)
$$
是点 $a$ 处阶 $n$ 的泰勒展开，则点 $a$ 处 $f'$ 阶 $n - 1$ 的泰勒展开为
$$
f'(x) = a_1 + 2a_2(x - a) + \cdots + na_n(x - a)^{n-1} + r'_n(x).
$$

我们说它是通过*逐项微分*从$f$的展开(11)获得的。

#### 注 2 {#fvr-i-s3-n2-rem-2 .statement tag=0854}

同样的假设，(11)中的系数$a_i$由关系递归确定

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

在$a = 0$一个结论的情况下，特别是，如果$f(x^p)$（$p$整数> 0）在0的邻域上有阶$pn$的导数，则阶$pn$的泰勒展开函数简直就是

$$
f(x^p) = a_0 + a_1 x^p + a_2 x^{2p} + \cdots + a_n x^{np} + r_n(x^p)
$$

其中 $r_n(x^p)$ 是展开中的余数 (*cf.* V, p. 222)。

#### 注 3 {#fvr-i-s3-n2-rem-3 .statement tag=0855}

阶 $n$ 的导数的定义和前面的结果立即推广到复变量的函数；我们不会在这里进一步讨论这个话题；这将在本级数后面的书中详细讨论。

### 习题 {#fvr-i-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
