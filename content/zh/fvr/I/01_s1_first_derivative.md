---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 1
section_title: FIRST DERIVATIVE
lang: zh
source: fvr-i-vii
book_pages: 3-12, 35-37
pdf_pages: 0018-0027, 0050-0052
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVE OF A VECTOR FUNCTION
      page: 3
      pdf_page: 18
    - "no": 2
      title: LINEARITY OF DIFFERENTIATION
      page: 5
      pdf_page: 20
    - "no": 3
      title: DERIVATIVE OF A PRODUCT
      page: 6
      pdf_page: 21
    - "no": 4
      title: DERIVATIVE OF THE INVERSE OF A FUNCTION
      page: 8
      pdf_page: 23
    - "no": 5
      title: DERIVATIVE OF A COMPOSITE FUNCTION
      page: 9
      pdf_page: 24
    - "no": 6
      title: DERIVATIVE OF AN INVERSE FUNCTION
      page: 9
      pdf_page: 24
    - "no": 7
      title: DERIVATIVES OF REAL-VALUED FUNCTIONS
      page: 10
      pdf_page: 25
statements: 36
exercises: 9
content_sha256: dc573a3c77b0529596715cfdc922c9f1e3a77b6d1b01c79042e8ae04813f7678
translated_from: content/en/fvr/I/01_s1_first_derivative.md
translation_method: google
source_content_sha256: 5dea356d12e98a054923f53371a9f84b313b2a5f5dd6646107d466573ef4a73f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: b7a3178ad5f6cb8dcd05a39d759fcda958ef1eeb93b3c5b4b2cb87a997365f9c
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 1。一阶导数

正如引言中所说，在这个章和接下来的函数中，我们将研究函数的无穷小属性，这些属性定义在实域$\mathbf{R}$的子集上，并在域上的*豪斯多夫拓扑向量空间* E中获取它们的值 $\mathbf{R}$；为了简洁起见，我们可以说这样的函数是一个实数变量*的 *向量函数。最重要的情况是其中 $E = \mathbf{R}$（实变量的实值函数）。当$E = \mathbf{R}^n$时，考虑E约化中的向量函数和值，同时考虑$n$有限实数函数。

许多定义和章I扩展到函数中所述的属性定义在域$\mathbf{C}$复数的子集上，并在拓扑向量空间上取它们的值 $\mathbf{C}$（复变量的向量函数）。其中一些定义和属性扩展甚至到函数是在任意交换*拓扑域* K的子集上定义的，并在K上的拓扑向量空间中取它们的值。

我们将在经过中指出这些推广（特别参见I，p. 10，*注2*），首先强调复变量的函数的情况，这是迄今为止最重要的，与实变量的函数一起，并将在后面的书中进行更深入的研究。

### 1. 向量函数的导数

#### 定义 1 {#fvr-i-s1-def-1 .statement tag=082P}

*令 $f$ 为区间 $I \subset \mathbf{R}$ 上定义的向量函数，它不会将约化定义为单个点。我们说 $f$ 在点 $x_0 \in I$ if* 处可微
$$
\lim_{x \to x_0, x \in I, x \neq x_0} \frac{f(x) - f(x_0)}{x - x_0}
$$
*存在（在向量空间中，其中$f$取其值）；这个极限的值称为$f$在点$x_0$的一阶导数（或简称导数），用$f'(x_0)$或$Df(x_0)$表示。*

If $f$ is differentiable at the point $x_0$, so is the *restriction* of $f$ to any interval $J \subset I$ which does not reduce to a single point and such that $x_0 \in J$; and the derivative of this restriction is equal to $f'(x_0)$. 相反，令$J$为包含在$I$中且包含相对于$I$的$x_0$邻域的区间；如果$f$到$J$的限制允许在点$x_0$处导数，那么$f$也是如此。

我们用说总结这些性质，即导数的概念是一个局部概念。

#### 注 1 {#fvr-i-s1-n1-rem-1 .statement tag=082Q}

在运动学中，如果点 $\mathbf{f}(t)$ 是移动的点在空间 $\mathbf{R}^3$ 在时间 $t$ 的位置，则 $\frac{\mathbf{f}(t) - \mathbf{f}(t_0)}{t - t_0}$ 称为瞬时 $t_0$ 和 $t$ 之间的平均速度，其极限 $\mathbf{f}'(t_0)$是$t_0$时刻的瞬时速度（或简称速度）（当极限存在时）。*

#### 注 2 {#fvr-i-s1-n1-rem-2 .statement tag=082R}

如果在$I$上定义的函数$\mathbf{f}$在点$x_0 \in I$处可微，则它在点处相对于$I$必然是连续的。

#### 定义 2 {#fvr-i-s1-def-2 .statement tag=082S}

*令$\mathbf{f}$为区间$I \subset \mathbf{R}$上定义的向量函数，并令$x_0$为$I$的点，使得区间$I \cap [x_0, +\infty[$（或$I \cap ]-\infty, x_0]$）不约化至单个点。如果$\mathbf{f}$到区间$I \cap [x_0, +\infty[$（或$I \cap ]-\infty, x_0]$）的限制在点可微，我们说$\mathbf{f}$在点$x_0$在右侧（或在左侧）可微。 $x_0$； 限制在点$x_0$的导数的值称为$\mathbf{f}$在点$x_0$的右（或左）导数，并表示为$\mathbf{f}'_d(x_0)$（或$\mathbf{f}'_g(x_0)$）。*

令$\mathbf{f}$为$I$上定义的向量函数，$x_0$为$I$的内部点，使得$\mathbf{f}$在点处连续；它来自 defs。 1 和 2 对于 $\mathbf{f}$ 在 $x_0$ 可微分，$\mathbf{f}$ 在此点承认右导数和左导数是必要且充分的，并且这些导数相等；然后

$$
\mathbf{f}'(x_0) = \mathbf{f}'_d(x_0) = \mathbf{f}'_g(x_0).
$$

#### 例 1 {#fvr-i-s1-n1-exa-1 .statement tag=082T}

常数函数在每个点处都有零导数。

#### 例 2 {#fvr-i-s1-n1-exa-2 .statement tag=082U}

仿射线性函数 $x \mapsto ax + b$ 在每个点处的导数等于 $a$。

#### 例 3 {#fvr-i-s1-n1-exa-3 .statement tag=082V}

实数函数$1/x$（为$x \neq 0$定义）在每个点$x_0 \neq 0$处是可微的，因为我们有$\left( \frac{1}{x} - \frac{1}{x_0} \right) / (x - x_0) = -\frac{1}{x x_0}$，并且由于$1/x$在$x_0$处连续，因此前面表达式的极限为$-1/x_0^2$。

#### 例 4 {#fvr-i-s1-n1-exa-4 .statement tag=082W}

在 $\mathbf{R}$ 上定义的标量函数 $|x|$，在 $x = 0$ 具有右导数 $+1$ 和左导数 $-1$；在这个点处不可微分。

#### 例 5 {#fvr-i-s1-n1-exa-5 .statement tag=082X}

实数函数对于$x = 0$等于0，对于$x \neq 0$等于$x \sin 1/x$，在$\mathbf{R}$上定义且连续，但在点$x \neq 0$处既没有右导数也没有左导数。*可以给出函数的例，它在函数上连续区间并且无法在区间的每个点处求导数（I、p. 35，练习 2 和 3）。

#### 定义 3 {#fvr-i-s1-def-3 .statement tag=082Y}

*我们说定义在区间$I \subset \mathbf{R}$上的向量函数$\mathbf{f}$在$I$上是可微的（分别是右可微、左可微），如果它在每个点是可微的（分别是右可微、左可微） $I$；在$I$上定义的函数$x \mapsto \mathbf{f}'(x)$（分别为$x \mapsto \mathbf{f}'_d(x)$、$x \mapsto \mathbf{f}'_g(x)$），称为派生的函数，或（滥用语言）$\mathbf{f}$的导数（分别为右导数、左导数），并表示为$\mathbf{f}'$或$\mathrm{Df}$ 或 $d\mathbf{f}/dx$（分别为 $\mathbf{f}'_d, \mathbf{f}'_g$）。*

#### 注 {#fvr-i-s1-n1-rem-3 .statement tag=082Z}

函数可以在区间上可微，但其导数在区间的每个点连续（*cf.*I，p. 36，练习5）； *这由函数的例等于0（对于$x = 0$）和$x^2 \sin 1/x$（对于$x \neq 0$）来表示；它到处都有导数，但这个导数在点 $x = 0$ 处不连续。

### 2. 微分线性

#### 命题 1 {#fvr-i-s1-prop-1 .statement tag=0830}

*在区间$I \subset \mathbf{R}$上定义向量函数的集合，在给定拓扑向量空间$E$中取值，并在点$x_0$可微，为向量空间超过$\mathbf{R}$，而映射$f \mapsto Df(x_0)$是空间的线性映射变成$E$。*

在其他字中，如果$f$和$g$在$I$上定义并且在点$x_0$可微，则$f + g$和$fa$（$a$任意标量）在$x_0$可微，它们的导数为分别为$f'(x_0) + g'(x_0)$和$f'(x_0)a$。这紧随$x + y$和$xa$分别在$E \times E$和$E$上的连续性而来。

#### 推论 {#fvr-i-s1-n2-cor-1 .statement tag=0831}

*在区间$I$上定义向量函数的集合，在给定拓扑向量空间$E$中取值，并且在$I$上可微，则向量空间超过$\mathbf{R}$，而映射$f \mapsto Df$是从$I$到$E$的空间的线性映射到映射的向量空间。*

#### 注 {#fvr-i-s1-n2-rem-1 .statement tag=0832}

如果将映射的向量空间从$I$赋予$E$，并且将其可微的映射（*cf. Gen. Top.*，X，p. 277）的子空间与简单收敛的拓扑赋予（或一致收敛的拓扑），线性映射$f \mapsto Df$*不连续*（一般情况下）*例如，函数*的序列*$f_n(x) = \sin n^2 x / n$*一致收敛到*0*在*$\mathbf{R}$，*但是导数的序列* $f'_n(x) = n \cos n^2 x$ *甚至不收敛到* 0。

#### 命题 2 {#fvr-i-s1-prop-2 .statement tag=0833}

*令$E$和$F$为$\mathbf{R}$上的两个拓扑向量空间，以及$u$从$E$到$F$的连续线性映射。如果$f$是在区间$I \subset \mathbf{R}$上定义的向量函数，在$E$中取值，并在点$x_0 \in I$可微，则复合函数$u \circ f$有等于 $u(f'(x_0))$ 在 $x_0$ 处的导数。*

事实上，从$\frac{u(f(x)) - u(f(x_0))}{x - x_0} = u \left( \frac{f(x) - f(x_0)}{x - x_0} \right)$开始，这是$u$的连续性。

#### 推论 {#fvr-i-s1-n2-cor-2 .statement tag=0834}

*如果$\varphi$是$E$上的连续线性形式，则实数函数$\varphi \circ f$在点$x_0$处的导数等于$\varphi(f'(x_0))$。*

#### 例 1 {#fvr-i-s1-n2-exa-1 .statement tag=0835}

设$f = (f_i)_{1 \leq i \leq n}$为函数，$\mathbf{R}^n$中有值，定义于区间$I \subset \mathbf{R}$；每个实数函数$f_i$都是复合函数$\mathrm{pr}_i \circ f$，因此如果$f$是可微的，那么在点$x_0$是可微的，如果是，则$f'(x_0) = (f'_i(x_0))_{1 \leq i \leq n}$是可微的。

#### 例 2 {#fvr-i-s1-n2-exa-2 .statement tag=0836}

在运动学中，如果 $f(t)$ 是移动点 $M$ 在时间 $t$ 的位置，如果 $g(t)$ 是 $M$ 到平面 $P$（或直线 $D$）上的投影 $M'$ 同一时刻的位置，且内核不平行于直线（或平面） $P$（分别$D$），则$g$是$\mathbf{R}^3$到$P$（分别$D$）和$f$的投影$u$的合成；由于 $u$ 是一个（连续）线性映射，我们可以看到移动点在平面（分别是直线）上的投影速度等于移动点在平面（分别是直线）上的投影速度。*

#### 例 3 {#fvr-i-s1-n2-exa-3 .statement tag=0837}

令$f$为在区间$I \subset \mathbf{R}$上定义的复值函数，并令$a$为任意复数；支柱。图2表明，如果$f$在点$x_0$处可微，那么$af$也是可微的，并且该函数在$x_0$处的导数等于$af'(x_0)$。

### 3. 乘积的导数

现在让我们考虑$\mathbf{R}$上的$p$拓扑向量空间$E_i$($1 \leq i \leq p$)，以及连续多线性$^1$映射（我们将表示为

$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1.x_2 \ldots x_p])
$$

$E_1 \times E_2 \times \cdots \times E_p$ 转换为$\mathbf{R}$ 上的拓扑向量空间 F。

#### 命题 3 {#fvr-i-s1-prop-3 .statement tag=0838}

*对于每个指标 $i$ ($1 \leq i \leq p$) 令 $f_i$ 为区间 $I \subset \mathbf{R}$ 上定义的函数，在 $E_i$ 中取值，并在点 $x_0 \in I$ 处可微。然后函数

$$
x \mapsto [f_1(x).f_2(x) \ldots f_p(x)]
$$

定义在 $I$ 上，$F$ 中的值的导数等于

$$
\sum_{i=1}^p [f_1(x_0) \ldots f_{i-1}(x_0).f'_i(x_0).f_{i+1}(x_0) \ldots f_p(x_0)]
$$

在$x_0$。

让我们把$h(x) = [f_1(x).f_2(x) \ldots f_p(x)]$；那么，根据身份

$$
[b_1.b_2 \ldots b_p] - [a_1.a_2 \ldots a_p] = \sum_{i=1}^p [b_1 \ldots b_{i-1}.(b_i - a_i).a_{i+1} \ldots a_p],
$$

我们可以写

$$
h(x) - h(x_0) = \sum_{i=1}^p [f_1(x) \ldots f_{i-1}(x).(f_i(x) - f_i(x_0)).f_{i+1}(x_0) \ldots f_p(x_0)].
$$

将两边同时乘以$\frac{1}{x - x_0}$并让$x$在$I$中逼近$x_0$，我们得到表达式(1)，因为映射都

$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1.x_2 \ldots x_p]
$$

F 中的加法是连续的。

$^1$ 回想一下（算法，II，p. 265），如果每个部分映射 $E_1 \times E_2 \times \cdots \times E_p$ 的映射 $f$ 进入 F 则被称为*多重线性*

$$
x_i \mapsto f(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_p)
$$

从$E_i$到F($1 \leq i \leq p$)是一个*线性*映射，指标$j \neq i$的$a_j$在$E_j$中是任意的。我们注意到，如果 $E_i$ 在 $\mathbf{R}$ 上是*有限*维的，那么 $E_1 \times E_2 \times \cdots \times E_p$ 到 F 中的每个多重线性映射必然是*连续的*；如果其中一些空间是无限维数的拓扑向量空间，则不必如此。

当函数$f_i$中的一些为常数时，式(1)包含中的项其导数$f'_i(x_0)$为零。

让我们详细考虑应用中最重要的特殊情况$p = 2$：如果$(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}.\mathbf{y}]$是$E \times F$到$G$的连续双线性映射，（E、F、G是$\mathbf{R}$上的拓扑向量空间），并且$\mathbf{f}$和$\mathbf{g}$ 是两个向量函数，在 $x_0$ 处可微，值分别在 E 和 F 中，则向量函数 $x \mapsto [\mathbf{f}(x).\mathbf{g}(x)]$（我们用 $[\mathbf{f}.\mathbf{g}]$ 表示）的导数等于 $[\mathbf{f}'(x_0).\mathbf{g}(x_0)] + [\mathbf{f}(x_0).\mathbf{g}'(x_0)]$ $x_0$。特别是，如果 $\mathbf{a}$ 是常数向量，则 $[\mathbf{a}.\mathbf{f}]$（分别为 $[\mathbf{f}.\mathbf{a}]$）在 $x_0$ 处的导数等于 $[\mathbf{a}.\mathbf{f}'(x_0)]$（分别为 $[\mathbf{f}'(x_0).\mathbf{a}]$）。

如果 $\mathbf{f}$ 和 $\mathbf{g}$ 在 I 上可微，那么 $[\mathbf{f}.\mathbf{g}]$ 也可微，并且我们有

$$
[\mathbf{f}.\mathbf{g}]' = [\mathbf{f}'.\mathbf{g}] + [\mathbf{f}.\mathbf{g}'].
$$

(2)

#### 例 1 {#fvr-i-s1-n3-exa-1 .statement tag=0839}

设$f$为实数函数，$\mathbf{g}$向量函数，两者在点$x_0$可微； 函数 $\mathbf{g}f$ 在 $x_0$ 的导数等于 $\mathbf{g}'(x_0)f(x_0) + \mathbf{g}(x_0)f'(x_0)$。特别是，如果 $\mathbf{a}$ 是常数，则 $\mathbf{a}f$ 具有导数 $\mathbf{a}f'(x_0)$。最后的注，在合取，例 1 of I，p. 5，证明如果$\mathbf{f} = (f_i)_{1 \leq i \leq n}$是向量函数，值在$\mathbf{R}^n$，那么对于$\mathbf{f}$ 在点 $x_0$ 处可微，实数函数 $f_i$ ($1 \leq i \leq n$) 在那里可微是必要且充分的：因为，如果 $(\mathbf{e}_i)_{1 \leq i \leq n}$ 是 $\mathbf{R}^n$ 的典范基，我们可以写$\mathbf{f} = \sum_{i=1}^n \mathbf{e}_i f_i$。

#### 例 2 {#fvr-i-s1-n3-exa-2 .statement tag=083A}

真正的函数 $x^n$ 来自多重线性函数

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n
$$

在$\mathbf{R}^n$上定义，用$x$替换每个$x_i$；所以支持。图 3 表明 $x^n$ 在 $\mathbf{R}$ 上可微，并且具有导数 $nx^{n-1}$。结果多项式函数$\mathbf{a}_0 x^n + \mathbf{a}_1 x^{n-1} + \cdots + \mathbf{a}_{n-1} x + \mathbf{a}_n$（$\mathbf{a}_i$为常数向量）有导数

$$
n \mathbf{a}_0 x^{n-1} + (n-1) \mathbf{a}_1 x^{n-2} + \cdots + \mathbf{a}_{n-1};
$$

当$\mathbf{a}_i$是实数时，函数重合具有多项式函数的导数，如代数（A，IV）中所定义。

#### 例 3 {#fvr-i-s1-n3-exa-3 .statement tag=083B}

欧氏标量乘积$(\mathbf{x}| \mathbf{y})$（Gen.Top，VI，p. 40）是$\mathbf{R}^n \times \mathbf{R}^n$到$\mathbf{R}$的双线性映射（必须连续）。如果 $\mathbf{f}$ 和 $\mathbf{g}$ 是两个向量函数，其中值在 $\mathbf{R}^n$ 中，且在点 $x_0$ 处可微，则实数函数 $x \mapsto (\mathbf{f}(x)|\mathbf{g}(x))$ 在 处的导数等于 $(\mathbf{f}'(x_0)|\mathbf{g}(x_0)) + (\mathbf{f}(x_0)|\mathbf{g}'(x_0))$ 点$x_0$。 $\mathbf{C}^n$ 上的厄米特标量乘积也有类似的结果，这个空间被视为 $\mathbf{R}$ 上的向量空间。

让我们特别考虑欧氏范数$\| \mathbf{f}(x) \|$恒定的情况，因此$(\mathbf{f}(x)|\mathbf{f}(x)) = \| \mathbf{f}(x) \|^2$也是恒定的；当$(\mathbf{f}(x)|\mathbf{f}(x))$的导数在$x_0$处消失时，我们得到$(\mathbf{f}(x_0)|\mathbf{f}'(x_0)) = 0$；在其他字中，$\mathbf{f}'(x_0)$与$\mathbf{f}(x_0)$正交。

#### 例 4 {#fvr-i-s1-n3-exa-4 .statement tag=083C}

如果$E$是$\mathbf{R}$上的拓扑代数（cf.介绍），则$E$的两个元素的乘积$xy$是$(x, y)$的连续双线性函数；如果$\mathbf{f}$和$\mathbf{g}$在$E$有值并且在点$x_0$可微，那么函数$x \mapsto \mathbf{f}(x)\mathbf{g}(x)$在$x_0$有等于$\mathbf{f}'(x_0)\mathbf{g}(x_0) + \mathbf{f}(x_0)\mathbf{g}'(x_0)$的导数。特别是，如果$U(x) = (\alpha_{ij}(x))$和$V(x) = (\beta_{ij}(x))$是阶$n$的两个方阵，在$x_0$可微，那么它们的乘积$UV$在$x_0$的导数等于$U'(x_0)V(x_0) + U(x_0)V'(x_0)$（其中$U'(x) = (\alpha'_{ij}(x))$ 和 $V'(x) = (\beta'_{ij}(x))$）。

#### 例 5 {#fvr-i-s1-n3-exa-5 .statement tag=083D}

来自空间 $\mathbf{R}^n$ (Alg., III, p. 522) 的 $n$ 向量 $\mathbf{x}_i = (x_{ij})_{1 \leq i \leq n}$ 的行列式 $\det(\mathbf{x}_1, \mathbf{x}_2, \ldots, \mathbf{x}_n)$ 是 $\mathbf{x}_i$ 的（连续）多线性函数，可以看出，如果 $n^2$ 实数函数 $f_{ij}$ 可微分于$x_0$，那么它们的行列式$g(x) = \det(f_{ij}(x))$的导数等于
$$
\sum_{i=1}^n \left[ \mathbf{f}_1(x_0), \ldots, \mathbf{f}_{i-1}(x_0), \mathbf{f}_i'(x_0), \mathbf{f}_{i+1}(x_0), \ldots, \mathbf{f}_n(x_0) \right]
$$
在$x_0$，其中$\mathbf{f}_i(x) = (f_{ij}(x))_{1 \leq j \leq n}$；换句话说，通过对每个$i$将$i^{th}$列的项替换为其导数而形成的$n$行列式之和，获得$n$阶行列式的导数。

#### 注 {#fvr-i-s1-n3-rem-1 .statement tag=083E}

如果$U(x)$是平方矩阵，在点$x_0$可微且可逆，则其行列式$\Delta(x) = \det(U(x))$的导数可以通过$U(x)$对公式的导数来表示
$$
\Delta'(x_0) = \Delta(x_0) \cdot \operatorname{Tr}(U'(x_0) U^{-1}(x_0)).
$$
事实上，让我们输入 $U(x_0 + h) = U(x_0) + h V$；那么，到定义时，当$h$趋于0时，$V$趋于$U'(x_0)$。可以写
$$
\Delta(x_0 + h) = \Delta(x_0) \cdot \det(I + h V U^{-1}(x_0)).
$$
现在$\det(I + h X) = 1 + h \operatorname{Tr}(X) + \sum_{k=2}^n \lambda_k h^k$，$\lambda_k$（$k \geq 2$）是矩阵$X$的元素多项式；由于当$h$趋于0时，$V U^{-1}(x_0)$的元素有极限，所以我们确实得到了公式（3）。

### 4. 函数的倒数的导数

#### 命题 4 {#fvr-i-s1-prop-4 .statement tag=083F}

*设 E 为完全范数代数，单位元超过$\mathbf{R}$，并令$\mathbf{f}$为区间$I \subset \mathbf{R}$上定义的函数，在E中取值，并在点$x_0 \in I$可微。如果$y_0 = \mathbf{f}(x_0)$在E中可逆$^2$，则函数$x \mapsto (\mathbf{f}(x))^{-1}$定义在$x_0$的邻域上（相对于I），并且在$x_0$处具有等于$-(\mathbf{f}(x_0))^{-1} \mathbf{f}'(x_0) (\mathbf{f}(x_0))^{-1}$的导数。*

事实上，E 中可逆元的集合是一个开集合，其中函数 $y \mapsto y^{-1}$ 是连续的（*Gen.Top.*、IX、p. 178）；由于$\mathbf{f}$在$x_0$处是连续的（相对于I），$(\mathbf{f}(x))^{-1}$定义在$x_0$的邻域上，并且我们有
$$
(\mathbf{f}(x))^{-1} - (\mathbf{f}(x_0))^{-1} = (\mathbf{f}(x))^{-1} \left( \mathbf{f}(x_0) - \mathbf{f}(x) \right) (\mathbf{f}(x_0))^{-1}.
$$
因此，命题由$y_0$的邻域上的$y^{-1}$的连续性以及$xy$在$E \times E$上的连续性得出。

$^2$ 回想一下 (*Alg.*, I, p. 15)，如果存在 $E$ 的元素（用 $z^{-1}$ 表示），使得 $zz^{-1} = z^{-1}z = e$ （e 是 $E$ 的单位元素），则元素 $z \in E$ 被称为“可逆”。

#### 例 1 {#fvr-i-s1-n4-exa-1 .statement tag=083G}

最重要的特殊情况是，其中 E 是域 $\mathbf{R}$ 或 $\mathbf{C}$ 之一：如果 $f$ 是函数，实数或复数值，可在点 $x_0$ 微分，并且使得 $f(x_0) \neq 0$，则 $1/f$ 的导数等于$-f'(x_0)/(f(x_0))^2$ $x_0$。

#### 例 2 {#fvr-i-s1-n4-exa-2 .statement tag=083H}

如果$U = (\alpha_{ij}(x))$是阶$n$的平方矩阵，在$x_0$可微且在点可逆，则$U^{-1}$在$x_0$的导数等于$-U^{-1} U' U^{-1}$。

### 5. 复合函数的导数

#### 命题 5 {#fvr-i-s1-prop-5 .statement tag=083I}

*设$f$为定义在区间$I \subset \mathbf{R}$上的实数函数，$g$向量函数定义在$\mathbf{R}$包含$f(I)$的区间上。如果 $f$ 在点 $x_0$ 可微，并且 $g$ 在点 $f(x_0)$ 可微，则复合函数 $g \circ f$ 在 $x_0$ 的导数等于 $g'(f(x_0)) f'(x_0)$。*

让我们输入$h = g \circ f$；对于 $x \neq x_0$ 我们可以写
$$
\frac{h(x) - h(x_0)}{x - x_0} = u(x) \frac{f(x) - f(x_0)}{x - x_0}
$$
如果$f(x) \neq f(x_0)$，我们集合$u(x) = \frac{g(f(x)) - g(f(x_0))}{f(x) - f(x_0)}$，否则$u(x) = g'(f(x_0))$。现在，当$x$趋于$x_0$时，$f(x)$有极限$f(x_0)$，因此$u(x)$有极限$g'(f(x_0))$，鉴于函数$yx$的连续性，命题随之而来$E \times \mathbf{R}$。

### 6. 逆函数的导数

#### 命题 6 {#fvr-i-s1-prop-6 .statement tag=083J}

*设$f$为区间$I \subset \mathbf{R}$到区间$J = f(I) \subset \mathbf{R}$的同态，并令$g$为逆同态$^3$。如果 $f$ 在点 $x_0 \in I$ 可微，并且如果 $f'(x_0) \neq 0$，则 $g$ 在 $y_0 = f(x_0)$ 具有等于 $1/f'(x_0)$ 的导数。*

对于每个$y \in J$，我们有$g(y) \in I$和$u = f(g(y))$；我们因此可以写
$$
\frac{g(y) - g(y_0)}{y - y_0} = \frac{g(y) - x_0}{f(g(y)) - f(x_0)}
$$
$y \neq y_0$。当$y$趋向于$y_0$，同时保留在$J$和$\neq y_0$时，$g(y)$趋向于$x_0$，保留在$I$和$\neq x_0$，因此前面公式的右侧有极限 $1/f'(x_0)$，自假设 $f'(x_0) \neq 0$ 起。

#### 推论{#fvr-i-s1-n6-cor-1 .statement tag=083K}

*如果$f$在$I$上可微，并且$f'(x) \neq 0$在$I$上可微，则$g$在$J$上可微，并且其在每个点$y \in J$处的导数为$1/f'(g(y))$。*

For example, for each 整数 $n > 0$, 函数 $x^{1/n}$ is a homeomorphism of $\mathbf{R}_+$ onto itself, is the inverse of $x^n$, and has derivative $\frac{1}{n} x^{\frac{1}{n} - 1}$ at each $x > 0$.

从道具中可以很容易地推断出。 5, that for every rational 数 $r = p/q > 0$ 函数 $x^r = (x^{1/q})^p$ has derivative $r{x'}^{-1}$ at every $x > 0$.

$^3$ For $f$ to be a homeomorphism of $I$ onto 子集 of $\mathbf{R}$ we know that it is necessary and sufficient that $f$ be continuous and strictly monotone on $I$ (*Gen. Top.*, IV, p. 338，第5）。

#### 注 1 {#fvr-i-s1-n6-rem-1 .statement tag=083L}

All the preceding 命题, stated for 函数 differentiable at 点 $x_0$, immediately yield 命题 for 函数 which are right (resp. left) differentiable at $x_0$, when, instead of 函数 themselves, one considers their 限制 to 交 of their 区间 of 定义 with 区间 $[x_0, +\infty[$ (resp. ]$-\infty, x_0$]);我们让读者来陈述它们。

#### 注 2 {#fvr-i-s1-n6-rem-2 .statement tag=083M}

The preceding 定义 and 命题 (except for those concerning right and left derivatives) 扩展 easily to the case where one 替换 $\mathbf{R}$ by an arbitrary *commutative non-discrete topological 域* $K$, and the topological 向量空间 (resp. topological 代数) over $\mathbf{R}$ by topological 向量空间 (resp. topological 代数) over $K$.在定义中。 1、道具。 1、2、3 $K$ 中$x_0$的*邻域*足以替换I；在道具中。 4 one must assume further that 映射 $y \mapsto y'$ is defined and continuous on 邻域 of $f(x_0)$ in E. Prop. 5 generalizes in the following manner: let $K'$ be a non-discrete 子域 of the topological 域 $K$, let E be a拓扑向量空间 *超过* $K$； let $f$ be 函数 defined on 邻域 $V \subset K'$ of $x_0 \in K'$, with 值 in $K$ (considered as a topological 向量空间 over $K'$), differentiable at $x_0$，令g为函数定义在$f(x_0) \in K$的邻域上，值在E中，并且在点$f(x_0)$可微； then 映射 $g \circ f$ is differentiable at $x_0$ and has derivative $g'(f(x_0))f'(x_0)$ there (E being then considered as a topological 向量空间 *over* $K'$).

With the same 记号, let $f$ be 函数 defined on 邻域 V of $a \in K$, with 值 in E, and differentiable at 点 $a$; if $a \in K'$, then the *限制* of $f$ to $V \cap K'$ is differentiable at $a$, and has derivative $f'(a)$ there. These considerations apply above all, in practice, to the case where $K = \mathbf{C}$ and $K' = \mathbf{R}$.

最后，道具。 6 扩展 to the case where one 替换 I by 邻域 of $x_0 \in K$, and $f$ by a homeomorphism of I onto 邻域 $J = f(I)$ of $y_0 = f(x_0)$ in $K$。

### 7. 实值函数的衍生品

The preceding 定义 and 命题 may be augmented in several respects when we deal with *real-valued* 函数 of a real variable.

首先，如果$f$是这样的函数，定义在区间$I \subset \mathbf{R}$上，并且相对于I在点$x_0 \in I$连续，那么可能会发生当$x$趋向于$x_0$同时保持在I并且$\neq x_0$，$\frac{f(x) - f(x_0)}{x - x_0}$的极限等于$+\infty$或$-\infty$；然后可以说 $f$ 在 $x_0$ 处可微，并且在那里有导数 $+\infty$（或 $-\infty$）；如果函数$f$在I的每个点$x$有一个导数$f'(x)$（有限或无限），则函数$f'$（$\overline{\mathbf{R}}$中的值）再次称为导数函数（或简称为$f$的导数）。类似地推广右导数和左导数定义。

#### 例 {#fvr-i-s1-n7-exa-1 .statement tag=083N}

在点$x = 0$函数$x^{1/3}$（$x^3$的逆函数，$\mathbf{R}$自身同胚）有一个导数，等于$+\infty$；在$x = 0$函数$|x|^{1/3}$有右导数$+\infty$和左导数$-\infty$。

公式对于可微实数函数的和、乘积的导数，以及可微分函数的逆（命题1、3和4），以及（实值）合成对函数的导数（命题1）。 5) 当出现的导数是无限时仍然有效，只要这些公式中出现的所有表达式都有意义（*Gen Top.*、IV、p. 345–346）。事实上，如果在道具中。 6 假设 $f$ 为严格递增的（分别为严格递减）并且在 I 上连续，并且如果 $f'(x_0) = 0$，则逆函数 $g$ 的导数等于 $+\infty$（分别为 $-\infty$） 点$y_0 = f(x_0)$；如果$f'(x_0) = +\infty$（或$-\infty$），则$g$的导数为0。右导数和左导数有类似的结果，我们将其留给读者处理。

令C为由点$(x, f(x))$形成的平面$\mathbf{R}^2$的有限实数函数$f$、子集的图形或表示曲线，其中$x$穿过集合，其中定义了$f$。若函数$f$在点$x_0 \in I$有有限右导数，则C以点$M_{x_0} = (x_0, f(x_0))$为原点，方向为数$(1, f'_d(x_0))$的半直线称为曲线的右半切线C 点 $M_{x_0}$；当$f'_d(x_0) = +\infty$（或$f'_d(x_0) = -\infty$）时，我们对原点为$M_{x_0}$、方向为数$(0, 1)$（或$(0, -1)$）的半线使用相同的术语。同理，当$f'_g(x_0)$存在时，在$M_{x_0}$处求定义左半切线。通过这些定义，我们可以快速验证右（或左）半切线与横坐标所成的角度是该轴与从 $M_{x_0}$ 和经过到 C 的点 $M_1 = (x, f(x))$ 所成的角度的极限，如下$x$趋于$x_0$，同时保持$> x_0$（或$< x_0$）。

也可以说，右（或左）半切线是从 $M_{x_0}$ 经过到 $M_1$ 的半线的极限，赋予具有相同原点的半线的集合商空间拓扑 $C^*/\mathbf{R}_+^*$（Gen.Top.、VIII、p. 107）。

如果C的点$M_{x_0}$存在两条半切线，则仅当$f$在点$x_0$（假设在I内部）有导数（有限或非）时，它们方向相反；仅当 $f'_d(x_0)$ 和 $f'_g(x_0)$ 无穷大且符号相反时，它们才相同。在这两种情况下，我们说直线包含这两条半切线是 C 在点 $M_{x_0}$ 的切线。

当$M_{x_0}$处的切线存在时，它是经过穿过$M_{x_0}$和$M_1$的线的极限，因为$x$趋于$x_0$，剩余$\neq x_0$，拓扑在穿过给定固定的线的集合上点是商空间 $C^*/\mathbf{R}^*$（Gen. Top.、VIII、p. 114）。

图的正切和半相切的概念是一般概念的特例，这些概念将在致力于可微分簇的级数的部分中定义。

#### 定义 4 {#fvr-i-s1-def-4 .statement tag=083O}

我们说，在拓扑空间 E 的子集 A 上定义的实函数 $f$，如果存在邻域 $V$，则相对于 A 在点 $x_0 \in A$ 处具有相对最大值（严格相对最大值、相对最小值、严格相对最小值） E 中的$x_0$，使得在与$x_0$不同的每个点$x \in V \cap A$，有一个$f(x) \leq f(x_0)$（分别为$f(x) < f(x_0)$、$f(x) \geq f(x_0)$、$f(x) > f(x_0)$）。

很明显，如果$f$在A的点处达到A上的最小上界（或下确界），那么它在这个点处相对于A有一个相对最大值（或相对最小值）； 逆命题当然是不正确的。

请注意，如果 $B \subset A$ 和 $f$ 承认（例如）相对于 B 的点 $x_0 \in B$ 处存在相对最大值，则 $f$ 不一定在该点处相对于 A 具有相对最大值。

#### 命题 7 {#fvr-i-s1-prop-7 .statement tag=083P}

令 $f$ 为有限实数函数，定义于区间 $I \subset \mathbf{R}$。如果$f$在I内部的点$x_0$处承认相对最大值（或相对最小值），并且在该点处具有右导数和左导数，则有$f'_d(x_0) \leq 0$和$f'_g(x_0) \geq 0$（分别为$f'_d(x_0) \geq 0$和$f'_g(x_0) \leq 0$);特别是，如果 $f$ 在点 $x_0$ 可微，则 $f'(x_0) = 0$。

命题是从定义衍生出来的。

我们可以进一步说，如果在I函数$f$内部的点$x_0$是可微的并且允许相对最大值或最小值，则其图的切线平行于横坐标。 逆命题是不正确的，如函数 $x^3$ 的例所示，它在点 $x = 0$ 处具有零导数，但在该点处既没有相对最大值也没有相对最小值。

### 习题 {#fvr-i-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
