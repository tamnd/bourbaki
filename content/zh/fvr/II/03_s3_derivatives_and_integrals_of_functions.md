---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 3
section_title: DERIVATIVES AND INTEGRALS OF FUNCTIONS DEPENDING ON A PARAMETER
lang: zh
source: fvr-i-vii
book_pages: 68-78, 86-90
pdf_pages: 0083-0093, 0101-0105
extraction: ocr
subsections:
    - "no": 1
      title: INTEGRAL OF A LIMIT OF FUNCTIONS ON A COMPACT INTERVAL
      page: 68
      pdf_page: 83
    - "no": 2
      title: INTEGRAL OF A LIMIT OF FUNCTIONS ON A NON-COMPACT INTERVAL
      page: 69
      pdf_page: 84
    - "no": 3
      title: NORMALLY CONVERGENT INTEGRALS
      page: 72
      pdf_page: 87
    - "no": 4
      title: DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A COMPACT INTERVAL
      page: 73
      pdf_page: 88
    - "no": 5
      title: DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A NON-COMPACT INTERVAL
      page: 75
      pdf_page: 90
    - "no": 6
      title: CHANGE OF ORDER OF INTEGRATION
      page: 76
      pdf_page: 91
statements: 18
exercises: 10
content_sha256: 1ab5d1e4cc20e39664adc52734241ee1ab3405ef6931026a59789b91f425c3b4
translated_from: content/en/fvr/II/03_s3_derivatives_and_integrals_of_functions.md
translation_method: google
source_content_sha256: 35c740d0a30b3f3ffd2d5f08cde90f87df1496bb44cbc74f5b2898276d078665
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: e2ba436173504c1d11b3e6edb81748507d4f387f006b2b0987380143570b72f0
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 3。 函数的导数和积分取决于参数

### 1. 极限函数在紧区间上的积分

Th。 II、p. 52 中的 1，应用于紧凑区间上调节的函数的特殊情况，可按如下方式转换为适合积分的记号：

#### 命题 1 {#fvr-ii-s3-prop-1 .statement tag=088Y}

Let A be a set filtered by a filter $\mathfrak{F}$, and $(f_\alpha)_{\alpha \in A}$ a family of regulated functions on a compact interval $I = [a, b]$; if the functions $f_\alpha$ converge uniformly on I to a (regulated) function f with respect to the filter $\mathfrak{F}$, then

$$
\lim_{\mathfrak{F}} \int_a^b f_\alpha(t) \, dt = \int_a^b f(t) \, dt.
$$

命题的两个推论在应用中很重要：

#### 推论 1 {#fvr-ii-s3-prop-1-cor-1 .statement tag=088Z}

令 $(f_n)$ 为紧凑区间 $I = [a, b]$ 上调节的函数的序列。如果序列 $(f_n)$ 在 I 上一致收敛到（调节的）函数 f，则有

$$
\lim_{n \to \infty} \int_a^b f_n(t) \, dt = \int_a^b f(t) \, dt.
$$

特别地，如果级数其广义项$u_n$是I上的调节函数，一致收敛于I上的f，则级数与广义项$\int_a^b u_n(t) \, dt$收敛，其和为$\int_a^b f(t) \, dt$（“一致收敛的级数的逐项积分”）。

#### 推论 2 {#fvr-ii-s3-prop-1-cor-2 .statement tag=0890}

令$A$为拓扑空间$F$的子集，并将$f$映射从$I \times A$变为空间$E$超过$\mathbf{R}$，这样，对于每个$\alpha \in A$， 函数 $x \mapsto f(x, \alpha)$受$I$监管。如果函数 $x \mapsto f(x, \alpha)$ 在 $I$ 上均匀收敛到（调节的）函数 $x \mapsto g(x)$，因为 $\alpha$ 趋于点 $\alpha_0 \in \overline{A}$，同时保持在 $A$，则有

$$
\lim_{\alpha \to \alpha_0,\ \alpha \in A} \int_a^b f(x, \alpha)\, dx = \int_a^b g(x)\, dx.
$$

尤其：

#### 命题 2（“积分相对于参数的连续性”）{#fvr-ii-s3-prop-2 .statement tag=0891}

令$F$为紧致空间，令$I = [a,\ b]$为$\mathbf{R}$中的紧致区间，令$f$为$I \times F$的连续映射到空间$E$超过$\mathbf{R}$；那么函数$h(\alpha) = \int_a^b f(x, \alpha)\, dx$在$F$上连续。

事实上，由于$f$在紧空间$I \times F$上一致连续，当$\alpha$趋于任意点$\alpha_0 \in F$时，函数$f(x, \alpha)$一致收敛到$I$上的$f(x, \alpha_0)$。

这是命题的一个应用：函数$(x, \alpha) \mapsto x^\alpha$在乘积$I \times J$上连续，其中$I = [a,\ b]$是紧致区间，使得$0 < a < b$，$J$是$\mathbf{R}$中的任何紧致区间；一个结论，$\int_a^b x^\alpha\, dx$是$\mathbf{R}$上$\alpha$的连续函数；现在，对于$\alpha$有理数和$\neq -1$，这个函数等于$\frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$，并且函数$\alpha \mapsto \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$在$\mathbf{R}$的每个区间上连续，而不是包含$-1$；因此，对于所有真实的$\alpha \neq -1$，一个人拥有（扩张个身份）$\int_a^b x^\alpha\, dx = \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$；这再次意味着，对于所有实数$\alpha$，$x^\alpha$的导数是$\alpha x^{\alpha-1}$（cf.III，p. 94）。

### 2. 极限函数在非紧区间上的积分

Th。 II、p. 52 中的第 1 个适用于函数，比规定的函数更通用，因为仅假设函数接受原语。特别是人们会看到那个道具。当仅假设在间隔 $I \subset \mathbf{R}$、函数 $f_\alpha$ 是“分段调节”并承认 $I$ 上的“整的”时，II、p. 68 中的 1 仍然适用；然而，这个结果以其他两个假设为前提。 1 满足，即：
1. $I$ 是一个*有界*区间； 2' $f_\alpha$*均匀地**$I$ 收敛到$f$。当不再满足这些条件之一时，II、p. 68的公式 (1) *可能会失败*：可能会发生这两个项中的一个或另一个不存在，或者两者都存在但具有不同的值。

对于例，如果$f_n$是$]0,\ 1[$上的调节函数，由$0 < x < 1/n$的$f_n(x) = n$和$1/n \leq x \leq 1$的$f_n(x) = 0$定义，则序列$(f_n)$在]0中包含的每个紧凑区间上均匀收敛于0， 1[，但在 [0, 1] 上并不统一，每个 $n$ 都有 $\int_0^1 f_n(t) \, dt = 1$。一个有例，其中 $\int_0^1 f_n(t) \, dt$ 不趋向于替换上的任何极限，而序列 $(f_n)$ 到序列 $((-1)^n f_n)$ 又在 ]0, 1] 中包含的每个紧凑区间上均匀收敛到 0。

另一方面，在*无界*区间$I = [0, +\infty[$上，令$f_n$为受管制的函数，使得$n^2 \leq x \leq (n+1)^2$有$f_n(x) = 1/n$，$I$（$n \geq 1$）中$x$的每隔一个值有$f_n(x) = 0$； 序列$(f_n)$在$I$上均匀收敛于0，但随着$n$无限增加，整的$\int_0^{+\infty} f_n(t) \, dt = (2n+1)/n$趋于2。

在其他字中，当$I$无界时，如果用函数$\mathbf{f}$在$I$上所形成的$\mathscr{I}$向量空间表示，值在$E$上，并且承认$I$上的积分，则当赋予 $\mathscr{I}$ $I$ 上均匀收敛的拓扑时，映射 $\mathbf{f} \mapsto \int_I \mathbf{f}(t) \, dt$ *不连续* (*cf.* II, p. 53, cor. 2)

我们将寻求*足够*条件来确保道具的有效性。 1、在以下假设下：

1. $I$是$\mathbf{R}$中的任意区间，函数$\mathbf{f}_\alpha$在$I$上有规定，并且允许$I$上的积分；
2. 在$I$中包含的每个紧区间上，族$(\mathbf{f}_\alpha)$相对于滤波器$\mathfrak{F}$均匀收敛到$\mathbf{f}$。

将$I$(II,p. 64)中包含的紧区间有向集合写成$\mathfrak{K}(I)$，II、p. 68的公式(1)左边可写为$\lim_{\delta} \left( \lim_{J \in \mathfrak{K}(I)} \int_J \mathbf{f}_\alpha(t) \, dt \right)$；另一方面，考虑到道具。 1 (II.p. 68)，并且族$(\mathbf{f}_\alpha)$在每个紧区间$J \subset I$上一致收敛，(1)的右侧(II，p. 68)可以写成$\lim_{J \in \mathfrak{K}(I)} \left( \lim_{\delta} \int_J \mathbf{f}_\alpha(t) \, dt \right)$。 人们因此看到了这个道具。 II、p. 19扩展中的1，当可以相对于过滤器$\mathfrak{F}$和相对于有向集合$\mathfrak{K}(I)$的截面的过滤器$\Phi$*互换映射$(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$的极限*时。 现在，我们知道一个*足够* 条件来证明此交换是合理的，即映射 $(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ 的极限相对于*乘积过滤器* $\Phi \times \mathfrak{F}$ 的存在（*Gen. 顶部。*、I、p. 81、cor。到 th。 1）。 我们将把变换这个条件变成一个等价的、更易于管理的条件。

首先，由于$E$是完备的，在阶中，$(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$相对于$\Phi \times \mathfrak{F}$应该有极限，对于每个$\varepsilon > 0$，应该存在一个紧区间$J_0 \subset I$和集合$M \in \mathfrak{F}$，这样，对于任何$M$的元素$\alpha, \beta$和$I$包含的紧区间$J \supset J_0$，有一个

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t) \, dt - \int_J \mathbf{f}_\beta(t) \, dt \right| \leq \varepsilon.
$$

另一方面，我们将证明这个条件本身等价于以下条件：对于每个$\varepsilon > 0$，都存在一个紧凑区间$J_0 \subset I$和集合$M \in \mathfrak{F}$，这样，对于$M$的任何$\alpha$和$I$中包含的任何紧凑区间$J \supset J_0$，一个有

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t) \, dt - \int_J \mathbf{f}_\alpha(t) \, dt \right| \leq \varepsilon.
$$

确实很明显，最后这个条件是必要的；相反，如果满足，则存在（通过$(\mathbf{f}_\alpha )$在每个紧区间上的一致收敛）集合$N \in \mathfrak{F}$，使得对于$N$中的任何$\alpha,\ \beta$有一个

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t)\,dt - \int_{J_0} \mathbf{f}_\beta(t)\,dt \right| \leq \varepsilon;
$$

因此对于 $M \cap N \in \mathfrak{F}$ 中的任何 $\alpha$ 和 $\beta$ 以及任何紧凑区间 $J \supset J_0$，$\left| \int_{J_0} \mathbf{f}_\alpha(t)\,dt - \int_J \mathbf{f}_\beta(t)\,dt \right| \leq 2\varepsilon$。

最后，II、p. 65的引理允许我们将最后一个条件放入以下等价的形式中：*对于每个$\varepsilon > 0$，存在一个紧凑区间$J_0 \subset I$和集合$M \in \mathfrak{F}$（取决于$\varepsilon$），这样，对于每个紧区间 $K \subset I$ 在公共的中没有内部点且有 $J_0$，并且每个 $\alpha \in M$ 有一个* $\left| \int_K \mathbf{f}_\alpha(t)\,dt \right| \leq \varepsilon$。

最常见的是，人们使用更严格的条件，通过假设在最后一个叙述、集合$M$*不依赖于$\varepsilon$*获得：

#### 定义 1 {#fvr-ii-s3-def-1 .statement tag=0892}

*有人说积分$\int_I \mathbf{f}_\alpha(t)\,dt$对于$\alpha \in A$一致收敛（或在$A$上一致收敛），如果对于每个$\varepsilon > 0$存在一个紧致区间$J_0 \subset J$，使得对于公共的和$J_0$中没有内部点的每个紧致区间$K \subset I$，并且每$\alpha \in A$，就有一个*

$$
\left| \int_K \mathbf{f}_\alpha(t)\,dt \right| \leq \varepsilon.
$$

这个定义相当于说，映射$\alpha \mapsto \int_I \mathbf{f}_\alpha(t)\,dt$的族*一致收敛于$A$*（朝向映射$\alpha \mapsto \int_I \mathbf{f}_\alpha(t)\,dt$）关于截面$\Phi$的过滤器$\mathscr{K}(I)$；每个积分 $\int_I \mathbf{f}_\alpha(t)\,dt$ 都 *更不必说* 收敛（逆命题为假）。此外，根据我们刚刚看到的内容（或来自*Gen.Top.*，X，p. 281，cor.2）：

#### 命题 3 {#fvr-ii-s3-prop-3 .statement tag=0893}

*设* $(\mathbf{f}_\alpha )$ *是一个在间隔* $I$ *上受调节的函数族，使得： 1* 相对于滤波器$\mathfrak{F}$ *族* $(\mathbf{f}_\alpha )$ *均匀收敛到函数* $f$ *（调节于* $I$） *在*$I$中包含的每个紧凑区间上； *2*整的$\int_I \mathbf{f}_\alpha(t)\,dt$*对于每个*$\alpha \in A$一致收敛。 *在这些假设下，整的* $\int_I f(t)\,dt$ *收敛，并且有*

$$
\lim_{\mathfrak{F}} \int_I \mathbf{f}_\alpha(t)\,dt = \int_I f(t)\,dt.
$$

道具的假设。当例$I$是一个*有界*区间时，$\mathbf{f}_\alpha$在$I$上*一致有界*，并且在$I$中包含的每个紧凑区间上一致收敛到$f$；事实上，如果$\| \mathbf{f}_\alpha(x) \| \leq h$对于所有$x \in I$和所有$\alpha$，并且如果$J_0$使得$I$和$J_0$之间的长度之差为$\leq \varepsilon / h$，则每个区间都满足条件（7） $K \subset I$ 无内饰点位于公共的与 $J_0$。

与道具一样。 II、p. 68 中的 1 个，支持两个推论。 3 在应用中很重要：

#### 推论 1 {#fvr-ii-s3-prop-3-cor-1 .statement tag=0894}

*设* $(f_n)$ *是在任意区间* $I$ 上调节的函数的序列，*在* $I$ 中包含的每个紧凑区间上均匀收敛到函数* $f$； *如果积分* $\int_I f_n(t)\,dt$ *一致收敛，则积分* $\int_I f(t)\,dt$ *收敛，并且*
$$
\lim_{n \to \infty} \int_I f_n(t)\,dt = \int_I f(t)\,dt.
$$
(9)

#### 注 {#fvr-ii-s3-n2-rem-1 .statement tag=0895}

对于公式 (9) 的有效性，该推论中提出的假设是充分的，但不是必要的；稍后我们将推广这个公式，同时推广积分的概念（参见INT，IV），并获得限制性小得多的条件。

#### 推论 2 {#fvr-ii-s3-prop-3-cor-2 .statement tag=0896}

*让* $A$ *成为拓扑空间* $F$的子集，*和* $f$ *映射的* $I \times A$ *变成完全规范的空间* $E$ *超过* $\mathbf{R}$，*这样，对于每个* $\alpha \in A$，*函数* $x \mapsto f(x, \alpha)$ *受* $I$ 监管。 *如果，一方面，函数* $x \mapsto f(x, \alpha)$ *均匀地收敛于* $I$ *到函数* $x \mapsto f(x)$ *作为* $\alpha$ *趋于* $\alpha_0 \in \overline{A}$ *同时保持在* $A$； *另一方面，如果积分* $\int_I f(x, \alpha)\,dx$ *一致收敛于* $A$，*则积分* $\int_I f(x)\,dx$ *收敛，并且有*
$$
\lim_{\alpha \to \alpha_0,\ \alpha \in A} \int_I f(x, \alpha)\,dx = \int_I f(x)\,dx.
$$
(10)

特别是：

#### 命题 4（“关于参数的不正确积分的连续性”）{#fvr-ii-s3-prop-4 .statement tag=0897}

*设* $F$ *为紧致空间，让* $I$ *为* $\mathbf{R}$中的任意区间，*和* $f$ *从* $I \times F$ *连续的映射变成完全规范的空间* $E$ *超过* $\mathbf{R}$； *如果积分* $h(\alpha) = \int_I f(x, \alpha)\,dx$ *一致收敛于* $F$，*它是* $\alpha$ *在* $F$ 上的连续函数。

鉴于道具。 II、p. 69中的第2个，这个命题也是从连续函数的均匀极限的连续性得出的（*Gen.Top.*、X、p. 282，第2个）。

### 3. 通常收敛的积分

令 $(f_\alpha)_{\alpha \in A}$ 成为任意间隔 $I \subset \mathbf{R}$ 上的受规管函数族，其中值处于$\mathbf{R}$ 上的完整规范空间 $E$ 中。假设$I$上存在有限实数调节函数$g$，使得对于每个$x \in I$和每个$\alpha \in A$，$\|f_\alpha(x)\| \leq g(x)$以及积分$\int_I g(t)\,dt$收敛。在这些条件下，整的 $\int_I f_\alpha(t)\,dt$ *绝对一致收敛*在 $A$ 上；事实上，对于 $I$ 中包含的每个紧区间 $K$，
$$
\left\| \int_K f_\alpha(t)\,dt \right\| \leq \int_K g(t)\,dt
$$

整的$\int_I g(t) \, dt$的收敛意味着对于每个$\varepsilon > 0$都存在一个紧致区间$J \subset I$，这样对于$J$中的每个紧致区间$K \subset I$不相交的都有一个$\int_K g(t) \, dt \leq \varepsilon$。当存在具有上述性质的实函数$g$时，我们说积分$\int_I f_\alpha(t) \, dt$通常收敛于$A$（cf.Gen.Top.，X，p. 296）。

积分可以一致收敛于$A$，而不是正常收敛。 *对于 $n \leq x \leq n+1$ 的条件 $f_n(x) = 1/x$ 定义的实函数的序列 $(f_n)$，以及$I = [0, +\infty[$ 中$x$ 的其他值，会发生$f_n(x) = 0$。整的$\int_1^\infty f_n(t) \, dt$一致收敛的是直接的，但不是通常收敛，因为关系$g(x) \geq f_n(x)$对于每个$x \in I$和所有$n$都蕴含$g(x) \geq 1/x$，因而$g$在$I$上的积分不收敛。

特别地，让我们考虑级数，其广义项$u_n$是区间$I$上的调节函数，并假设级数与广义项$\|u_n(x)\|$（它是$I$上的调节函数）收敛均匀地分布在 $I$ 中包含的每个紧区间上，并且使得级数与一般项 $\int_I \|u_n(t)\| \, dt$ 收敛；则 (II, p. 66, 命题 2) 级数的（规定的）函数 $g(x)$, 和与一般项 $\|u_n(x)\|$，使得积分 $\int_I g(t) \, dt$ 收敛。如果输入 $f_n = \sum_{p=1}^n u_p$，则积分 $\int_I f_n(t) \, dt$ 通常是收敛的，因为有

$$
\|f_n(x)\| \leq \sum_{p=1}^n \|u_p(x)\| \leq g(x)
$$

对于所有$x \in I$和所有$n$；在推论中，级数的和$f$与一般项$u_n$是$I$上的调节函数，使得积分$\int_I f(t) \, dt$收敛，并且有

$$
\int_I f(t) \, dt = \sum_{n=1}^\infty \int_I u_n(t) \, dt
$$

（“在非紧区间上逐项积分级数”）。

### 4. 紧区间上积分参数的导数

令$A$为域$\mathbf{R}$（或域$\mathbf{C}$）中点$\alpha_0$的紧邻域，令$I = [a, b]$为$\mathbf{R}$中的紧致区间，$f$为连续将$I \times A$的映射转化为完整规范的空间$E$超过$\mathbf{R}$（或$\mathbf{C}$）。我们已经看到（II，p. 69，道具2），在这些条件$g(\alpha) = \int_a^b f(t, \alpha) \, dt$之下是$A$上的连续函数。让我们为 $g$ 寻找足够的条件来承认点 $\alpha_0$ 处的导数。一个有，对于 $\alpha \neq \alpha_0$，

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_a^b \frac{f(t, \alpha) - f(t, \alpha_0)}{\alpha - \alpha_0} \, dt
$$

所以（II，p. 69，cor.2），如果函数$x \mapsto \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$在I上均匀收敛到（必然连续的）函数$x \mapsto \mathbf{h}(x)$，而$\alpha$趋于$\alpha_0$（同时保持$\neq \alpha_0$），那么$g$ 在点 $\alpha_0$ 处承认等于 $\int_a^b \mathbf{h}(t)\,dt$ 的导数；此外，对于每个$x \in I$，$\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$趋向于$\mathbf{h}(x)$，因此$\mathbf{h}(x)$是映射$\alpha \mapsto \mathbf{f}(x, \alpha)$在点$\alpha_0$的导数；我们用记号$\mathbf{f}'_{\alpha}(x, \alpha_0)$表示这个导数（称为*$\mathbf{f}$*相对于*$\alpha$的偏导数）；我们所做的假设意味着

$$
g'(\alpha_0) = \int_a^b \mathbf{f}'_{\alpha}(t, \alpha_0)\,dt.
$$

(12)

下面的命题给出了一个非常简单的充分的条件来证明公式（12）的有效性：

#### 命题 5 {#fvr-ii-s3-prop-5 .statement tag=0898}

*假设偏导数* $\mathbf{f}'_{\alpha}(x, \alpha)$ *对于所有* $x \in I$ *和所有* $\alpha$ *存在于* 邻域* $V$ ** $\alpha_0$，*并且对于所有* $\alpha \in V$，*映射* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ *受* $I$ 监管。 *在这些条件下，如果* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ *一致收敛于* $I$ *到* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha_0)$ *作为* $\alpha$ *趋于* $\alpha_0$，*则函数* $g(\alpha) = \int_a^b \mathbf{f}(t, \alpha)\,dt$ *承认导数，由下式给出公式* (12)，*在点* $\alpha_0$。

事实上，对于每个$\varepsilon > 0$，都存在假设一个$r > 0$，使得$|\alpha - \alpha_0| \leq r$意味着$\| \mathbf{f}'_{\alpha}(x, \alpha) - \mathbf{f}'_{\alpha}(x, \alpha_0) \| \leq \varepsilon$*对于任何*$x \in I$。通过道具。 I、p. 17 中的 3 和 5 个有，适用于 $|\alpha - \alpha_0| \leq r$ ($\alpha \neq \alpha_0$) 以及所有 $x \in I$

$$
\left\| \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0} - \mathbf{f}'_{\alpha}(x, \alpha_0) \right\| \leq \varepsilon
$$

证明当$\alpha$趋于$\alpha_0$（剩余$\neq \alpha_0$）时$\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$到$\mathbf{f}'_{\alpha}(x, \alpha_0)$在I上一致收敛，从而建立公式 (12)。

#### 推论 {#fvr-ii-s3-n4-cor-1 .statement tag=0899}

*如果偏导数* $\mathbf{f}'_{\alpha}(x, \alpha)$ *存在于* $I \times V$ *并且是* $(x, \alpha)$ *在此集合上的连续函数，则函数* $g$ *承认由公式* (12) *给出的导数点*$\alpha_0$。

事实上，如果 W 是包含在 V 中的 $\alpha_0$ 的紧凑邻域，那么映射 $(x, \alpha) \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ 在紧集 $I \times W$ 上“均匀连续”，因此 $\mathbf{f}'_{\alpha}(x, \alpha)$ 倾向于在 I 上均匀地趋于 $\mathbf{f}'_{\alpha}(x, \alpha_0)$因为$\alpha$趋向于$\alpha_0$。

来自道具。 5 推导出更通用的命题，当积分的被积数 $\mathbf{f}$ 和积分的极限都依赖于参数 $\alpha$ 时，它允许人们计算积分的导数：

#### 命题 6 {#fvr-ii-s3-prop-6 .statement tag=089A}

*假设道具的假设。 5满足，令*$a(\alpha)$、$b(\alpha)$*为两个函数定义在*$V$、*和值在*$I$； *如果导数* $a'(\alpha_0),\ b'(\alpha_0)$ 存在且有限，则函数 $g(\alpha) = \int_{a(\alpha)}^{b(\alpha)} f(t, \alpha)\, dt$ 在 $\alpha_0$ 承认由公式给出的导数

$$
g'(\alpha_0) = \int_{a(\alpha_0)}^{b(\alpha_0)} f'_\alpha(t, \alpha_0)\, dt + b'(\alpha_0)f(b(\alpha_0), \alpha_0) - a'(\alpha_0)f(a(\alpha_0), \alpha_0).
$$

事实上，对于所有与$\alpha_0$不同的$\alpha \in V$，我们都可以写

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_{a(\alpha_0)}^{b(\alpha_0)} \frac{f(t, \alpha) - f(t, \alpha_0)}{\alpha - \alpha_0}\, dt + \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt
$$
$$
- \frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} f(t, \alpha)\, dt.
$$

通过道具。 II、p. 74的5，右边第一个积分趋于$\int_{a(\alpha_0)}^{b(\alpha_0)} f'_\alpha(t, \alpha_0)\, dt$，因为$\alpha$趋于$\alpha_0$。在第二个积分中，我们将替换 $f(t, \alpha)$ 除以 $f(b(\alpha_0), \alpha_0)$，并表明差值趋于 0。我们输入 $M = \max (\|f(b(\alpha_0), \alpha_0)\|, |b'(\alpha_0)| + 1)$； 函数 $b(\alpha)$ 在点 $\alpha_0$ 处连续，函数 $f$ 在点 $(b(\alpha_0), \alpha_0)$ 连续，对于每个$\varepsilon$，使得$0 < \varepsilon < 1$ 存在一个$r > 0$，使得关系 $|\alpha - \alpha_0| \leq r$ 意味着 $\|f(t, \alpha) - f(b(\alpha_0), \alpha_0)\| \leq \varepsilon$ 对于所有 $t$ 属于到端点为 $b(\alpha_0)$ 和 $b(\alpha)$ 的区间；因而，我们也可以假设关系 $|\alpha - \alpha_0| \leq r$ 必然包含 $\left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} - b'(\alpha_0) \right| \leq \varepsilon$。

平均而言值公式 (II, p 62, 公式 (17)) 因此有

$$
\left| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt - \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} f(b(\alpha_0), \alpha_0) \right| \leq \left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} \right| \varepsilon
$$

因而

$$
\left| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt - b'(\alpha_0) f(b(\alpha_0), \alpha_0) \right| \leq 2M \varepsilon
$$

这表明$\frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt$趋于$b'(\alpha_0) f(b(\alpha_0), \alpha_0)$。以同样的方式表明 $\frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} f(t, \alpha)\, dt$ 趋于 $a'(\alpha_0) f(a(\alpha_0), \alpha_0)$。

### 5. 非紧区间上积分参数的导数

集合 $V$ 与道具中的含义相同。 II、p. 74的 5 个，现在假设I是$\mathbf{R}$中的*任意*区间，并且$f$是从$I \times V$到E的*连续*映射；如果所有 $\alpha \in V$ 都存在积分 $g(\alpha) = \int_I f(t, \alpha)\, dt$ 并且是 $\alpha$ 的连续函数，则函数 $g$ *不需要有等于* $\int_I f'_\alpha(t, \alpha_0)\, dt$ *在点* $\alpha_0$ 的导数，即使$f'_\alpha(x, \alpha)$ 在 I 中包含的每个紧凑区间上一致收敛于 $f'_\alpha(x, \alpha_0)$，并且如果所有 $\alpha \in V$ 都存在积分 $\int_I f'_\alpha(t, \alpha) \, dt$（cf. II，p. 87，执行 3）。

足以使公式 (12) (II, p. 74) 保持有效的条件由以下命题给出：

#### 命题 7 {#fvr-ii-s3-prop-7 .statement tag=089B}

令I为$\mathbf{R}$上的任意区间，$f$为$I \times V$上的连续函数。假设：
1. 偏导数$f'_\alpha(x, \alpha)$对于所有$x \in I$和所有$\alpha \in V$都存在，并且对于所有$\alpha \in V$，映射$x \mapsto f'_\alpha(x, \alpha)$受I规管；
2. 对于所有$\alpha \in V$，$f'_\alpha(x, \beta)$在I中包含的每个紧区间一致收敛到$f'_\alpha(x, \alpha)$，因为$\beta$趋向于$\alpha$；
3. 整的$\int_I f'_\alpha(t, \alpha) \, dt$一致收敛于$V$；
4. 整的$\int_I f(t, \alpha_0) \, dt$收敛。

在这些情况下，整的$g(\alpha) = \int_I f(t, \alpha) \, dt$一致收敛于$V$，并且函数$g$在$V$的每个点处允许由公式给出的导数

$$
g'(\alpha) = \int_I f'_\alpha(t, \alpha) \, dt.
$$

$\int_I f'_\alpha(t, \alpha) \, dt$在$V$上一致收敛意味着，对于I中包含的紧区间$J$的有向集合$\mathfrak{K}(I)$的截面$\Phi$滤波器，函数$\alpha \mapsto \int_J f'_\alpha(t, \alpha) \, dt$在$V$上一致收敛。让我们输入 $u_J(\alpha) = \int_J f(t, \alpha) \, dt$；假设表明，一方面 $u_J(\alpha_0)$ 相对于 $\Phi$ 具有极限，另一方面，凭借 prop. II、p. 74 中的 5 个，即 $u'_J(\alpha) = \int_J f'_\alpha(t, \alpha) \, dt$ 代表所有 $\alpha \in V$。因此我们可以应用th。 II、p. 52到函数$u_J$，这里指标的集合的作用由$\mathfrak{K}(I)$承担，而这个集合上的过滤器的作用则由过滤器$\Phi$承担； 命题紧随其后。

#### 注 1 {#fvr-ii-s3-n5-rem-1 .statement tag=089C}

条件 1 和 2 的支柱。当$f'_\alpha(x, \alpha)$是$(x, \alpha)$在$I \times V$上的连续函数时，7满足更不必说。

#### 注 2 {#fvr-ii-s3-n5-rem-2 .statement tag=089D}

在积分$\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt$中，当区间的端点是参数的有限函数时，将该积分作为$\alpha$的函数的研究可以与$[0, 1]$上的积分的研究相关联；事实上，通过变量$t = a(\alpha)(1 - u) + b(\alpha)u$的变换，我们有

$$
\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt = \int_0^1 f(a(\alpha)(1 - u) + b(\alpha)u, \alpha) (b(\alpha) - a(\alpha)) \, du.
$$

### 6. 变换阶整合

设$I = [a, b]$和$A = [c, d]$为$\mathbf{R}$中的两个紧区间；设$f$是$I \times A$上的连续函数，其中值在$\mathbf{R}$上的完整规范的空间E中；通过道具。 II、p. 69、$\int_a^b f(x, \alpha) \, dx$中的2个是$A$上$\alpha$的连续函数；为简单起见，其积分 $\int_c^d \left( \int_a^b f(x, \alpha) \, dx \right) d\alpha$ 也表示为 $\int_c^d d\alpha \int_a^b f(x, \alpha) \, dx$。

#### 命题 8 {#fvr-ii-s3-prop-8 .statement tag=089E}

*如果 f 在 I × A 上连续，则有*

$$
\int_c^d d\alpha \int_a^b f(x, \alpha) dx = \int_a^b dx \int_c^d f(x, \alpha) d\alpha
$$

（“公式交换阶积分”）。

我们将证明，对于所有 $y \in A$，有一个

$$
\int_c^y d\alpha \int_a^b f(x, \alpha) dx = \int_a^b dx \int_c^y f(x, \alpha) d\alpha.
$$

由于(16)的两侧是$y$的函数，并且对于$y = c$相等，因此只需证明它们在$]c, d[$上可微，并且它们的导数在该区间的每个点处相等。如果把$g(\alpha) = \int_a^b f(x, \alpha) dx$和$h(x, y) = \int_c^y f(x, \alpha) dx$放在一起，关系(16)可以写成

$$
\int_c^y g(\alpha) d\alpha = \int_a^b h(x, y) dx.
$$

现在，第一个项相对于$y$的导数是$g(y)$，而第二个$\int_a^b h_y'(x, y) dx$，由II、p. 74推论，因为$h_y'(x, y) = f(x, y)$在$I \times A$上连续；由此获得的两个表达式是相同的。

现在假设$A = [c, d]$是$\mathbf{R}$中的*紧凑*区间，I是$\mathbf{R}$中的*任意*区间；设$f$是$I \times A$上的连续函数，值在E中，使得积分$g(\alpha) = \int_I f(t, \alpha) dt$对于所有$\alpha \in A$是收敛的；即使$g(\alpha)$在$A$上连续一个不能，也总是在积分$\int_c^d d\alpha \int_I f(t, \alpha) dt$中互换积分的阶，因为积分$\int_I dt \int_c^d f(t, \alpha) d\alpha$可能不存在，或者可能与积分$\int_c^d d\alpha \int_I f(t, \alpha) dt$不同（*cf.* II， p. 87，练习7）。然而，有以下结果：

#### 命题 9 {#fvr-ii-s3-prop-9 .statement tag=089F}

*如果函数 f 在I × A 上连续，并且如果积分 $\int_I f(t, \alpha) dt$ 在 A 上一致收敛，则积分 $\int_I dt \int_c^d f(t, \alpha) d\alpha$ 收敛，有*

$$
\int_c^d d\alpha \int_I f(t, \alpha) dt = \int_I dt \int_c^d f(t, \alpha) d\alpha.
$$

对于I中包含的每个紧区间J，放入$u_J(\alpha) = \int_J f(t, \alpha) dt$。 假设意味着对于有向集合 $\mathscr{K}(I)$ 的截面 $\Phi$ 滤波器，连续函数 $u_J$ 在 A 上一致收敛到$\int_I f(t, \alpha) dt$；因此（II，p. 68，道具1），$\int_c^d d\alpha \int_J f(t, \alpha) dt$相对于$\Phi$有极限$\int_c^d d\alpha \int_I f(t, \alpha) dt$；但是，通过道具。 8 个（II，p. 77），其中一个有

$$
\int_c^d d\alpha \int_J f(t, \alpha) dt = \int_J dt \int_c^d f(t, \alpha) d\alpha.
$$

因此，前面的结果意味着积分$\int_1 dt \int_c^{d} f(t, \alpha) d\alpha$是收敛的，并且在关系(18)中关于$\Phi$在经过到极限上，得到(17)。

### 习题 {#fvr-ii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
