---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 5
section_title: Real-valued functions
lang: zh
source: top-i-iv
book_pages: 347-359, 389-393
pdf_pages: 0353-0365, 0395-0399
extraction: ocr
subsections:
    - "no": 1
      title: REAL-VALUED FUNCTIONS
      page: 347
      pdf_page: 353
    - "no": 2
      title: REAL-VALUED FUNCTIONS DEFINED ON A FILTERED SET
      page: 348
      pdf_page: 354
    - "no": 3
      title: LIMITS ON THE RIGHT AND ON THE LEFT OF A FUNCTION OF A REAL VARIABLE
      page: 349
      pdf_page: 355
    - "no": 4
      title: BOUNDS OF A REAL-VALUED FUNCTION
      page: 350
      pdf_page: 356
    - "no": 5
      title: ENVELOPES OF A FAMILY OF REAL-VALUED FUNCTIONS
      page: 352
      pdf_page: 358
    - "no": 6
      title: UPPER LIMIT AND LOWER LIMIT OF A REAL-VALUED FUNCTION WITH RESPECT TO A FILTER
      page: 353
      pdf_page: 359
    - "no": 7
      title: ALGEBRAIC OPERATIONS ON REAL-VALUED FUNCTIONS
      page: 356
      pdf_page: 362
statements: 31
exercises: 18
content_sha256: b9b92302ea9b79242bc457ad1a913e534fa457603664294d097197439470c778
translated_from: content/en/top/IV/05_s5_real_valued_functions.md
translation_method: google
source_content_sha256: 621e60dc8288e6ddcbaf7c1e586598f735828021aa542b362efd2af2f9c86a93
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: c01750e9f1ec761c8fcc0d4764add183cc125456b2a1f396b74b4d0ea7d0150c
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 5. 实值函数

### 1. 实值函数

#### 定义 1 {#top-iv-s5-def-1 .statement tag=0BR2}

集合 $X$到实直线的映射称为定义在$X$上的实值函数（或实数函数）。

通过滥用与§ 4, no. 2中提到的类似的语言，$X$到$\overline{\mathbf{R}}$的映射也将被称为在此和下面的截面中定义在$X$上的实值函数。 $X$到$\mathbf{R}$的映射将被称为有限实值函数。

如果$f$和$g$是在$X$上定义的两个实值函数，则关系$f \leq g$乘以定义相当于“对于所有$x \in X$来说$f(x) \leq g(x)$；”这个关系是$X$上所有实值函数在集合$\overline{\mathbf{R}}^X$上的排序。按此关系排序集合$\overline{\mathbf{R}},^X$，是一个格子；因为如果$f$和$g$是由$h(x) = \sup (f(x), g(x))$定义的任意两个实值函数、函数$h$，则所有$x \in X$是$X$上的实值函数的最小的，它们都是$\geq f$和$\geq g$；根据一般记号，我们用$\sup (f, g)$表示这个函数（$f$和$\overline{\mathbf{R}}^X$中的$g$中最小的上界）。类似地，每个$x \in X$处的值为$\inf (f(x), g(x))$的函数用$\inf (f, g)$表示。

$\sup (f, g)$是映射的合成的注
$$
(u, v) \to \sup (u, v)
$$
将 $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ 转换为 $\overline{\mathbf{R}}$，并将映射 $x \to (f(x), g(x))$ 将 $X$ 转换为 $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$。对于 $\inf (f, g)$ 也是如此。

A real-valued function $f$ defined on a set $X$ is said to be *bounded above* (resp. *bounded below*) in $X$, if $f(X)$ is a subset of $A'' = [-\infty, +\infty]$ and is bounded above (resp. if $f(X)$ is a subset of $A' = ]-\infty, +\infty]$ and is bounded below). $f$ is said to be *bounded* in $X$ if it is bounded both above and below, that is if $f(X)$ is a bounded subset of $\mathbf{R}$.

因此，每个有界函数都是*有限*。 逆命题为假，如$\mathbf{R}_+^* = ]0, +\infty[$上的函数$1/x$所示。

### 2. 在过滤的集合上定义实值函数

#### 命题 1 {#top-iv-s5-prop-1 .statement tag=0BR3}

*令$f$和$g$为在集合$X$上定义的两个实值函数，并通过过滤器$\mathfrak{F}$过滤。如果$\lim_{\mathfrak{F}} f$和$\lim_{\mathfrak{F}} g$存在，并且对于每个子集$A \in \mathfrak{F}$，存在$x \in A$使得$f(x) \leq g(x)$，那么我们有$\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$。*

为了证明这个结果，我们将证明以下等价叙述：

#### 命题 2 {#top-iv-s5-prop-2 .statement tag=0BR4}

*令$f$和$g$为在集合$X$上定义的两个实值函数，并通过过滤器$\mathfrak{F}$过滤。如果$\lim_{\mathfrak{F}} f$和$\lim_{\mathfrak{F}} g$存在，并且如果$\lim_{\mathfrak{F}} f > \lim_{\mathfrak{F}} g$，则存在集合$A \in \mathfrak{F}$，使得$f(x) > g(x)$对于所有$x \in A$。*

令$a = \lim_{\mathfrak{F}} f$、$b = \lim_{\mathfrak{F}} g$和$c$使得$b < c < a$。 The interval $]c, +\infty]$ of $\overline{\mathbf{R}}$ (resp. $]-\infty, c[$) is a neighbourhood of $a$ (resp. $b$); hence there is a set $M \in \mathfrak{F}$ (resp. a set $N \in \mathfrak{F}$) such that $f(x) > c$ for all $x \in M$ [resp. $g(x) < c$ for all $x \in N$]. 集合$A = M \cap N$属于到$\mathfrak{F}$，对于所有$x \in A$我们都有$f(x) > c > g(x)$。

作为命题 1 的特例，我们有以下定理：

#### 定理 1（扩张不等式中的原理）{#top-iv-s5-thm-1 .statement tag=0BR5}

*令$f$和$g$为两个实值函数，定义在由过滤器$\mathfrak{F}$过滤的集合$X$上。如果$\lim_{\mathfrak{F}} f$和$\lim_{\mathfrak{F}} g$存在，并且如果$f \leq g$，则$\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$。*

#### 注 {#top-iv-s5-n2-rem-1 .statement tag=0BR6}

特别是，如果我们对所有$x \in X$（或仅对过滤器$\overline{\mathbf{R}}$的集合的所有点）都有$f(x) < g(x)$，我们可以通过定理1推断出$\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$； *但我们不能推断强不等式*$\lim_{\mathfrak{F}} f < \lim_{\mathfrak{F}} g$。对于例，如果我们将 $X$ 设为自然数的集合 $\mathbf{N}$（经 Fréchet 过滤器过滤），并且如果 $f(n) = 0$ 和 $g(n) = 1/n$，则对于所有 $n$，但$\lim_{n \to \infty} f(n) = \lim_{n \to \infty} f(n) = 0$，$f(n) < g(n)$。因此，当我们在*严格*不等式中传递到极限时，我们*失去了严格性*。

#### 定理 2（单调极限的定理）{#top-iv-s5-thm-2 .statement tag=0BR7}

令 $X$ 为有序集合，令 $A$ 为 $X$ (*) 的有向子集。 $A$ 上定义的每个单调实值函数 $f$ 相对于 $A$ 都有极限 (章 I, , no. 3);如果 $f$ 为递增（分别为递减），则该极限等于集合 $f(A) \subset \overline{\mathbf{R}}$ 中的最小上界（分别为下确界）

假设对于例，$f$ 是递增，并设$a = \sup f(A)$。如果$a = -\infty$，定理是微不足道的。如果$a > -\infty$，则对于每个$b < a$，存在$x \in A$使得$b < f(x) \leq a$；因此，如果$S_x$相对于$x$是$A$的截面（即所有$y \geq x$、cf.章I, § 6, no. 3的集合），$f(S_x)$包含在邻域中$a$中的$]b, +\infty]$，以及定理紧随其后。如果 $f$ 是递减，证明是类似的。

#### 推论{#top-iv-s5-n2-cor-1 .statement tag=0BR8}

递增（或递减）实值函数，定义在有序集合$X$的有向子集$A$上，相对于$A$具有有限的极限当且仅当它在上界（或下界）时$A$。

如果我们将应用定理 2 转换为$A = X = \mathbf{N}$（按关系$\leq$排序），我们有以下命题：

#### 命题 3 {#top-iv-s5-prop-3 .statement tag=0BR9}

实数的每个单调序列在$\overline{\mathbf{R}}$ 中都有极限。
特别是，有限数的每个递增（或递减）序列，如果其上界（或下界），则收敛到有限的实数，否则收敛到$+\infty$（或$-\infty$）。对于例，正整数的序列收敛于$+\infty$。

这个事实是记号$\lim_{n \to \infty} u_n$表示序列的极限（章I, § 7, no. 3）的起源。

同样，整数$(p_n)$的每个严格递增的序列都收敛到$+\infty$；因为我们通过归纳看到$p_n \geq p_0 + n$对于所有$n$。

### 3. 极限位于实数变量函数的右侧和左侧

令$A$为$\overline{\mathbf{R}}$的非空子集，令$a \neq -\infty$为$\overline{\mathbf{R}}$的点，位于集合$B = A \cap [-\infty, a[$的闭包中。 集合$B$相对于关系$\leq$有向，其截面滤波器$\mathfrak{F}$与$\overline{\mathbf{R}}$中$a$的邻域滤波器在$B$上的踪迹相同。

(*) 这个叙述隐含地假设$X$中的排序被写成$x \leq y$。 如果将这个关系写成$x(\sigma) y$，其中$(\sigma)$是关系所设想的某个符号或群特征符号，则叙述中的字“定向”必须替换为“相对于$(\sigma)$定向”。

#### 定义 2 {#top-iv-s5-def-2 .statement tag=0BRA}

*设 f 为函数，定义在 $\overline{\mathbf{R}}$ 的非空子集 A 上，值位于拓扑空间 X 中。 f 相对于过滤器 $\mathfrak{F}$ 的极限（如果存在）称为 f 的极限，位于点 a 左侧，相对于 A，并表示为*
$$
\lim_{x \to a,\ x < a,\ x \in A} f(x),
$$
*或 $f(a-)$，如果 X 是 Hausdorff。*

同样，如果$a$在集合$A \cap ]a, + \infty]$的闭包中，我们在点$a$处$f$右侧*（如果存在）定义一个*极限，并将其表示为
$$
\lim_{x \to a,\ x > a,\ x \in A} f(x),
$$
*或 $f(a+)$，如果 X 是 Hausdorff。*

下面的命题是定理2的直接的推论：

#### 命题 4 {#top-iv-s5-prop-4 .statement tag=0BRB}

*在交$A \cap [-\infty, a[$的闭包中，令A为$\overline{\mathbf{R}}$的子集，并令$a \neq -\infty$为点。如果 f 是 A 上定义的单调实值函数，则 f 在 a 左侧相对于 A 具有极限 $f(a-)$。*

### 4. 实值函数的界限

#### 定义 3 {#top-iv-s5-def-3 .statement tag=0BRC}

*设f为定义在集合X上的实值函数，并设A为X的非空子集。那么$\overline{\mathbf{R}}$中集合$f(A)$的最小上界（或下确界）称为A中f的最小上界（或下确界），记为*
$$
\sup_{x \in A} f(x) \quad \text{[resp. } \inf_{x \in A} f(x) \text{]}.
$$

特别是，如果 A 是 $\overline{\mathbf{R}}$ 的非空子集，则
$$(1)$$
$$
\sup A = \sup_{x \in A} x.
$$
通常更方便的是在右侧使用记号来表示 A 的最小上界。

数 $a = \sup_{x \in A} f(x)$ 具有以下两个性质：
(i) 对于所有$x \in A, f(x) \leq a$。
(ii) 对于每个$b < a$，都存在$x \in A$使得$b < f(x) \leq a$。

数$\sup_{x \in A} f(x)$和$\inf_{x \in A} f(x)$属于到$\overline{\mathbf{R}}$*关闭*$f(A)$。我们有$\inf_{x \in A} f(x) \leq \sup_{x \in A} f(x)$；当且仅当 $f$ 在 A 上是*常数*时，这两个数*相等*。

定义在集合 X 上的实值函数，在 X 的非空子集 A 中*上界*（分别*下界*）当且仅当 $\sup_{x \in A} f(x) < + \infty$ [分别*下界*]。 $\inf_{x \in A} f(x) > -\infty$]。 $f$ 在 A 中是有界的当且仅当$|f|$ 在 A 中有界，因此当且仅当$\sup_{x \in A} |f(x)| < + \infty$。

我们有

$$
\inf_{x \in A} f(x) = -\sup_{x \in A} (-f(x)).
$$

这关系约化下确界的所有属性到最小上界的属性；因此，一般来说我们只讨论后者。

#### 命题 5 {#top-iv-s5-prop-5 .statement tag=0BRD}

*令$f$为定义在集合$X$上的实值函数。在$X$的所有有限子集中的集合$\mathfrak{F}(X)$上，相对于关系$\subset$，实值函数$H \to \sup_{x \in H} f(x)$为递增，实值函数 $H \to \inf_{x \in H} f(x)$ 是递减，我们有*

$$
\begin{cases}
\sup_{x \in A} f(x) = \lim_{H \in \mathfrak{F}(X)} (\sup_{x \in H} f(x)), \\
\inf_{x \in A} f(x) = \lim_{H \in \mathfrak{F}(X)} (\inf_{x \in H} f(x)).
\end{cases}
$$

让$\varphi(H) = \sup_{x \in H} f(x)$。显然 $\varphi$ 是递增，因此有极限 $a$ (no. 2, 定理 2)；由于 $\varphi(H) \leq \sup_{x \in A} f(x)$ 对于所有 $H$，我们有 $a \leq \sup_{x \in A} f(x)$（no. 2，定理 1）。如果我们有$a < \sup_{x \in A} f(x)$，那么就会存在$x_0 \in X$，使得$a < f(x_0)$；但这是一个矛盾，因为 $\varphi(H) \geq f(x_0)$ 每当 $x_0 \in H$ 时。

特别是，根据（1），如果$A$是$\overline{\mathbf{R}}$的任何非空子集，我们有

$$
\sup A = \lim_{H \in \mathfrak{F}(A)} (\sup_{x \in H} x).
$$

#### 命题 6 {#top-iv-s5-prop-6 .statement tag=0BRE}

*令$f$和$g$为$X$上定义的两个实值函数。如果$f(x) \leq g(x)$位于$X$的非空子集$A$的每个点$x$，那么我们有*

$$
\begin{cases}
\sup_{x \in A} f(x) \leq \sup_{x \in A} g(x), \\
\inf_{x \in A} f(x) \leq \inf_{x \in A} g(x).
\end{cases}
$$

#### 命题 7 {#top-iv-s5-prop-7 .statement tag=0BRF}

*令$f$为定义在$X$上的实值函数。如果$A$和$B$是$X$的两个非空子集，使得$A \subset B$，那么*

$$
\sup_{x \in A} f(x) \leq \sup_{x \in B} f(x).
$$

#### 命题 8 {#top-iv-s5-prop-8 .statement tag=0BRG}

*设$f$为$X$上定义的实值函数，并令$(A_i)_{i \in I}$为$X$的非空子集的非空族；那么*

$$
\sup_{x \in \bigcup_{i \in I} A_i} f(x) = \sup_{i \in I} (\sup_{x \in A_i} f(x)).
$$

令$f$为定义在乘积集合$X_1 \times X_2$上的实值函数。如果$A_2$是$X_2$的非空子集，我们将用$\sup_{x_1 \in A_2} f(x_1, x_2)$表示$X_2$上定义的实值函数$x_2 \to f(x_1, x_2)$中$A_2$中最小的上界。从命题 8 我们特别推出：

#### 命题 9 {#top-iv-s5-prop-9 .statement tag=0BRH}

*令$f$为定义在乘积集合$X_1 \times X_2$上的实值函数。如果$A_1, A_2$分别是$X_1, X_2$的任何非空子集，则*

$$
\sup_{(x_1, x_2) \in A_1 \times A_2} f(x_1, x_2) = \sup_{x_1 \in A_1} (\sup_{x_2 \in A_2} f(x_1, x_2)) = \sup_{x_2 \in A_2} (\sup_{x_1 \in A_1} f(x_1, x_2)).
$$

### 5. 真正有价值的家庭信封函数

#### 定义 4 {#top-iv-s5-def-4 .statement tag=0BRI}

*设$(f_i)_{i \in I}$是在集合$X$上定义的实值函数族。 $X$ 上的实值函数，其值在每个点 $x \in X$ 处为 $\sup_{i \in I} (f_i(x))$ [resp]。 $\inf_{i \in I} (f_i(x))$]称为$(f_i)$族的上（或下）信封，并用$\sup_{i \in I} f_i$或$\sup_i f_i$（或$\inf_{i \in I} f_i$或$\inf_i f_i$）表示。

因此，族$(f_i)$的上包络线是在$X$上定义的实值函数的格子$\overline{\mathbf{R}}$中该族的最小上界，并且这证明记号$\sup_{i \in I} f_i$是合理的。

此外，如果我们赋予$\overline{\mathbf{R}}^X$以拓扑，即其因子拓扑的乘积（与$\overline{\mathbf{R}}$相同），我们有以下命题：

#### 命题 10 {#top-iv-s5-prop-10 .statement tag=0BRJ}

*在乘积空间$\overline{\mathbf{R}}^X$实值函数$(f_i)_{i \in I}$族的上包络线$\sup_{i \in I} f_i$是极限，相对于有限子集的有向集合$\mathfrak{F}(I)$ $I$，映射$H \to \sup_{i \in H} f_i$[其中映射每个有限子集$H$共$I$到有限子族$(f_i)_{i \in H}$的上包络]。

这紧接着从no. 4的命题5和章I, § 7, no. 6，推论1到命题10。

因此我们可以写

$$
\sup_{i \in I} f_i = \lim_{H \in \mathfrak{F}(I)} (\sup_{i \in H} f_i).
$$

#### 定义 5 {#top-iv-s5-def-5 .statement tag=0BRK}

*在集合 $X$ 上定义的实值函数的族 $(f_i)_{i \in I}$ 据说在 $X$ 中均匀上界（或下界均匀），如果存在有限数 $a$ 使得 $f_i(x) \leq a$ [或。 $f_i(x) \geq a$] 对于所有 $x \in X$ 和所有 $i \in I$。如果族 $(f_i)$ 在 $X$ 的上方和下方均匀有界，则称其在 $X$ 中均匀有界。

因此，当且仅当该族的上包络线在 $X$ 中上界时，$(f_i)$ 统一在 $X$ 中上界。 $(f_i)$ 统一有界于 $X$ 当且仅当族 $(|f_i|)$ 的上包络线在 $X$ 中上界 [即当且仅当存在有限实数 $a \geq 0$，使得 $|f_i(x)| \leq a$ 对于所有 $x \in X$ 和所有 $i \in I$]。

### 6. 相对于过滤器的实值函数的上部极限和下部极限

令 $f$ 为在集合 $X$ 上定义的实值函数，并由过滤器 $\mathfrak{G}$ 过滤。 $\mathfrak{G}$ 相对于关系 $\supseteq$ (章 I, § 6) 而言是有向集合。对于每个$M \in \mathfrak{G}$考虑实数$\sup_{x \in M} f(x)$：我们将$\mathfrak{G}$的函数$M \to \sup_{x \in M} f(x)$放入$\overline{\mathbf{R}}$，即$\mathfrak{G}$上的递减函数，乘以命题7 no. 4。因此，通过no. 2的定理2，它相对于有向集合$\mathfrak{G}$有极限。

#### 定义 6 {#top-iv-s5-def-6 .statement tag=0BRL}

*The limit of the real-valued function* $M \to \sup_{x \in M} f(x)$ *with respect to the directed set* $\mathfrak{G}$ *is called the upper limit of* $f$ *with respect to the filter* $\mathfrak{G}$, *and is denoted by* $\lim \sup_{\mathfrak{G}} f$, *or by* $\lim \sup_{x, \mathfrak{G}} f(x)$.

$f$相对于滤波器$\mathfrak{G}$的*下极限*的定义类似，并用$\lim \inf_{\mathfrak{G}} f$或$\lim \inf_{x, \mathfrak{G}} f(x)$表示。因此我们有

$$
\begin{cases}
\lim \sup_{\mathfrak{G}} f = \lim_{M \in \mathfrak{G}} (\sup_{x \in M} f(x)), \\
\lim \inf_{\mathfrak{G}} f = \lim_{M \in \mathfrak{G}} (\inf_{x \in M} f(x)).
\end{cases}
$$

(10)

通常，过滤器$\mathfrak{G}$会被记号抑制，并且在不存在混淆风险的情况下，我们简单地写为$\lim \sup f$或$\lim \sup_{x} f(x)$或$\lim \sup f(x)$。

从公式 (10) 和定理 1 我们有

$$
\inf_{x \in X} f(x) \leq \lim \inf_{\mathfrak{G}} f \leq \lim \sup_{\mathfrak{G}} f \leq \sup_{x \in X} f(x).
$$

(11)

通过定理 2 of no. 2 我们也可以写

$$
\begin{cases}
\lim \sup_{\mathfrak{G}} f = \inf_{M \in \mathfrak{G}} (\sup_{x \in M} f(x)), \\
\lim \inf_{\mathfrak{G}} f = \sup_{M \in \mathfrak{G}} (\inf_{x \in M} f(x)).
\end{cases}
$$

(12)

我们也可以通过 $\mathfrak{G}$ 的任何 *基* $\mathfrak{B}$，在公式 (10) 和 (12) 的右侧进行替换过滤器 $\mathfrak{G}$。

由(2)和(10)可知，

$$
\lim \inf_{\mathfrak{G}} f = -\lim \sup_{\mathfrak{G}} (-f)
$$

因此我们只需要考虑上面的极限。

#### 定理 3 {#top-iv-s5-thm-3 .statement tag=0BRM}

*相对于过滤器$\mathfrak{G}$的实值函数$f$的上部极限等于相对于$\mathfrak{G}$的$f$的最大的簇值。*

令$b$为$f$相对于$\mathfrak{G}$的簇点。对于每个$M \in \mathfrak{G}$，$b$位于$f(M)$的闭包中，因此$b \leq \sup_{x \in M} f(x)$，因此，根据（12），
$b \leq \lim \sup_{\mathfrak{G}} f = a.$

另一方面，令$V$为$\overline{\mathbf{R}}$中$a$的任意开邻域。那么$\mathfrak{G}$中存在集合$M_0$，这样，对于$M_0$中包含的每个$M \in \mathfrak{G}$，我们有$\sup_{x \in M} f(x) \in V$；由于$V$是开放的，因此$f(M)$满足$V$，因此$a$是$f$相对于$\mathfrak{G}$的*簇点*，并且证明是完整的。

#### 推论 1 {#top-iv-s5-thm-3-cor-1 .statement tag=0BRN}

*在阶、$\lim \sup_{\mathfrak{G}} f = \lim \inf_{\mathfrak{G}} f$中，$f$相对于过滤器$\mathfrak{G}$具有极限是充分必要的，然后*
$$
\lim_{\mathfrak{G}} f = \lim \sup_{\mathfrak{G}} f = \lim \inf_{\mathfrak{G}} f.
$$
因为由于$\overline{\mathbf{R}}$是紧凑的，所以当且仅当过滤器基$f(\mathfrak{G})$只有一个簇点时，它才具有极限点（章I, § 9, no. 1，定理1的推论）。

#### 推论 2 {#top-iv-s5-thm-3-cor-2 .statement tag=0BRO}

*如果$\mathfrak{H}$是更细比$\mathfrak{G}$的过滤器，我们有*
$$
\lim \inf_{\mathfrak{G}} f \leq \lim \inf_{\mathfrak{H}} f \leq \lim \sup_{\mathfrak{H}} f \leq \lim \sup_{\mathfrak{G}} f.
$$
对于$f$相对于$\mathfrak{H}$的每个集群点也是$f$相对于$\mathfrak{G}$的集群点（章I, § 7, no. 3）。
特别是，如果 $\lim_{\mathfrak{G}} f$ 存在，那么
$$
\lim \inf_{\mathfrak{G}} f \leq \lim_{\mathfrak{G}} f \leq \lim \sup_{\mathfrak{G}} f.
$$

#### 推论 3 {#top-iv-s5-thm-3-cor-3 .statement tag=0BRP}

*令$A$为滤波器$\mathfrak{G}$的集合，令$\mathfrak{G}_A$为$\mathfrak{G}$在$A$上诱导的滤波器，令$f_A$为$f$至$A$的限制；那么*
$$
\lim \sup_{\mathfrak{G}_A} f_A = \lim \sup_{\mathfrak{G}} f.
$$
对于过滤器基$f(\mathfrak{G})$的每个集群点都是过滤器基$f_A(\mathfrak{G}_A)$的集群点，反之亦然。

因此，如果仅在$X$、属于至$\mathfrak{G}$中的子集、$A$定义$f$，我们常常会写成$\limsup_{\mathfrak{G}} f$而不是$\limsup_{\mathfrak{G}_A} f_A$，这是语言滥用。

#### 命题 11 {#top-iv-s5-prop-11 .statement tag=0BRQ}

令$f$和$g$是在过滤后的集合$X$上定义的两个实值函数。那么关系 $f \leq g$ 意味着

$$
\begin{cases}
\limsup f \leq \limsup g, \\
\liminf f \leq \liminf g.
\end{cases}
$$

这是关系 (12) 中的直接的推论。

当$X$是拓扑空间并且$\mathfrak{G}$是$X$的点$a$的邻域过滤器时，我们写$\limsup_{x \to a} f(x)$[resp。 $\liminf_{x \to a} f(x)$] 代替 $\limsup_{\mathfrak{G}} f$ [分别。 $\liminf_{\mathfrak{G}} f$]；显然我们有

$$
\liminf_{x \to a} f(x) \leq f(a) \leq \limsup_{x \to a} f(x).
$$

更一般地，如果$X$是拓扑空间$Y$的子空间，并且如果$\mathfrak{G}$是点$a \in \overline{X}$的邻域滤波器在$X$上的踪迹，我们写$\limsup_{x \to a, x \in X} f(x)$[resp。 $\liminf_{x \to a, x \in X} f(x)$] 而不是$\limsup_{\mathfrak{G}} f$ [分别。 $\liminf_{\mathfrak{G}} f$]； $\limsup$被称为$f(x)$的上极限，因为$x$趋于$a$，同时保持在$X$。如果$X$是$\{a\}$的补集，我们在记号中写“x \neq a”来代替“x \in X”。

如果$A$是$X$的子集使得$a \in \overline{A}$，那么（推论2到定理3）

$$
\liminf_{x \to a, x \in X} f(x) \leq \liminf_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in X} f(x).
$$

如果$V$是$Y$中$a$的邻域，我们有（推论3到定理3）

$$
\limsup_{x \to a, x \in V \cap X} f(x) = \limsup_{x \to a, x \in X} f(x).
$$

因此，拓扑空间的点处的上极限和下极限的概念是局部特征标的概念，就像极限的概念一样。

Finally, if $\mathfrak{G}$ is the Fréchet filter on $\mathbf{N}$, the upper (resp. lower) limit, with respect to $\mathfrak{G}$, of the mapping $n \to u_n$ of $\mathbf{N}$ into $\overline{\mathbf{R}}$ is denoted by $\limsup_{n \to \infty} u_n$ (resp. $\liminf_{n \to \infty} u_n$) and is called the upper (resp. lower) limit of the sequence of real numbers $u_n$.

因此，关系$\limsup_{n \to \infty} u_n = a \in \mathbf{R}$等价于：给定任何$\varepsilon > 0$，都存在整数$n_0$，这样，对于每个$n \geq n_0$，我们有$u_n \leq a + \varepsilon$，对于$n$的无穷大值，我们有$u_n \geq a - \varepsilon$。 序列的上极限的定义，当其值为$+\infty$或$-\infty$时，可以类似地翻译。

给定在集合$X$上定义的实值函数的序列$(f_n)$，我们用$\limsup_{n \to \infty} f_n$（或$\liminf_{n \to \infty} f_n$）表示实值函数，其值在任何点 $x \in X$ 是$\limsup_{n \to \infty} f_n(x)$ [分别。 $\liminf_{n \to \infty} f_n(x)$]。由(10)和(12)我们推导出
$$
\begin{cases}
\limsup_{n \to \infty} f_n = \inf_{n \in \mathbf{N}} (\sup_{m \geq n} f_m) = \lim_{n \to \infty} (\sup_{m \geq n} f_m), \\
\liminf_{n \to \infty} f_n = \sup_{n \in \mathbf{N}} (\inf_{m \geq n} f_m) = \lim_{n \to \infty} (\inf_{m \geq n} f_m),
\end{cases}
$$
极限拍摄于 *乘积空间* $\overline{\mathbf{R}}^X$。 序列$(f_n)$在$\overline{\mathbf{R}}^X$中有*极限*当且仅当$\limsup_{n \to \infty} f_n = \liminf_{n \to \infty} f_n$（推论1到定理3，以及章I, § 7, no. 6，推论1到命题10）。

### 7. 实值函数上的代数运算

令$f$和$g$为定义在集合$X$上的两个实值函数；如果和 $f(x) + g(x)$ [分别。 乘积 $f(x)g(x)$] 是为所有 $x \in X$ 定义的，那么我们用 $f + g$（或 $fg$）表示实值函数
$$
x \mapsto f(x) + g(x) \quad \text{[resp. } x \mapsto f(x)g(x)].
$$
同样，如果为所有$x \in X$定义了$1/f(x)$，则$1/f$表示函数$x \mapsto 1/f(x)$。

因此，如果 $f$ 不采用值 0，则定义最后一个函数；当$f$在区间$[0, +\infty]$（分别在$[-\infty, 0]$）$1/f(x)$中取其值时，如通过放置$1/0 = +\infty$（分别在$1/0 = -\infty$）定义的任何地方；在这种情况下，定义了函数$1/f$。

假设$X$被过滤器$\mathfrak{F}$过滤，并且存在$\lim_{\mathfrak{F}} f$和$\lim_{\mathfrak{F}} g$。 If on the one hand the function $f + g$ (resp. $fg$, $1/g$) is defined, and if on the other hand the expression $\lim_{\mathfrak{F}} f + \lim_{\mathfrak{F}} g$ (resp. $\lim_{\mathfrak{F}} f \cdot \lim_{\mathfrak{F}} g$, $1/\lim_{\mathfrak{F}} f$) has a sense, then $\lim_{\mathfrak{F}} (f + g)$ [resp. $\lim_{\mathfrak{F}} fg$, $\lim_{\mathfrak{F}} (1/f)$] exists and is equal to this expression by reason of the continuity of the function $x + y$ (resp. $xy$, $1/x$) at points where it is defined.

#### 命题 12 {#top-iv-s5-prop-12 .statement tag=0BRR}

*令$f$和$g$为集合$X$上定义的两个实值函数，并令$A$为$X$的非空子集。*

(i) *我们有*
$$
\begin{align*}
&\sup_{x \in A} (f(x) + g(x)) \leq \sup_{x \in A} f(x) + \sup_{x \in A} g(x), \\
&\sup_{x \in A} f(x) + \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x) + g(x)),
\end{align*}
$$
*只要定义了这些不等式的两边。*

(ii) *如果对于每个 $x \in A$，$f(x)$ 和 $g(x)$ 都是 $\geq 0$，则*

(19)
$$
\sup_{x \in A} (f(x)g(x)) \leq \sup_{x \in A} f(x) \sup_{x \in A} g(x),
$$
(20)
$$
\sup_{x \in A} f(x) \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x)g(x))
$$
*只要定义了这些不等式的两边。*

(iii) *如果 $f(x) \geq 0$ 对于所有 $x \in A$，则*
(21)
$$
\sup_{x \in A} (1/f(x)) = 1/\inf_{x \in A} f(x)
$$
*（放入$1/0 = +\infty$）。*

令 $H$ 为 $A$ 的任何*有限* 子集。如果$x_0$是$H$的点之一，其中$f + g$取其最大的值，那么我们有
$$
f(x_0) + g(x_0) \leq \sup_{x \in H} f(x) + \sup_{x \in H} g(x);
$$
另一方面，如果 $x_1$ 是 $H$ 的点之一，其中 $f$ 取其最大的值，则
$$
f(x_1) + g(x_1) \geq \sup_{x \in H} f(x) + \inf_{x \in H} g(x);
$$
因此
$$
\sup_{x \in H} f(x) + \inf_{x \in H} g(x) \leq \sup_{x \in H} (f(x) + g(x)) \leq \sup_{x \in H} f(x) + \sup_{x \in H} g(x).
$$
由此得出不等式 (17) 和 (18) 应用命题 5 of no. 4 和定理 1 of no. 2。其他不等式证明类同。

#### 推论 1 {#top-iv-s5-prop-12-cor-1 .statement tag=0BRS}

*令$f$为定义在$X$上的实值函数，并令$k$为实数。然后*
(22)
$$
\sup_{x \in A} (f(x) + k) = k + \sup_{x \in A} f(x)
$$
*只要双方都被定义，并且，如果 $k \geq 0,$*
(23)
$$
\sup_{x \in A} (kf(x)) = k \cdot \sup_{x \in A} f(x)
$$
*每当双方都被定义时。*

#### 推论 2 {#top-iv-s5-prop-12-cor-2 .statement tag=0BRT}

*设$f_1$和$f_2$分别为定义在集合和$X_1, X_2$上的两个实值函数；那么如果 $A_1, A_2$ 分别是 $X_1, X_2$ 的任何非空子集，我们有*
(24)
$$
\sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1) + f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) + \sup_{x_2 \in A_2} f_2(x_2)
$$

每当双方都被定义时；如果 $f_1, f_2$ 分别是 $A_1, A_2$ 中的 $\geq 0$，我们有

$$
(25) \quad \sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1)f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) \sup_{x_2 \in A_2} f_2(x_2),
$$

每当双方都被定义时。

这是前面推论的直接的推论和no. 4的命题9。

特别地，如果$A$和$B$是$\overline{\mathbf{R}}$的两个子集，从而定义了和$x + y \ (x \in A, y \in B)$的集合$A + B$，我们有

$$
(26) \quad \sup (A + B) = \sup A + \sup B
$$

如果定义了右侧。同样，如果$A$和$B$是$[0, + \infty]$中的两个子集，我们有

$$
(27) \quad \sup AB = \sup A \cdot \sup B
$$

每当双方都被定义时。

#### 命题 13 {#top-iv-s5-prop-13 .statement tag=0BRU}

*让$f$和$g$是在过滤后的集合$X$上定义的两个实值函数。*

(i) *我们有*

$$
(28) \quad \lim \sup (f + g) \leq \lim \sup f + \lim \sup g,
$$
$$
(29) \quad \lim \sup f + \lim \inf g \leq \lim \sup (f + g)
$$

*只要定义了这些不等式的两边。*

(ii) *如果$f$和$g$在$X$上是$\geq 0$，我们有*

$$
(30) \quad \lim \sup fg \leq (\lim \sup f) (\lim \sup g),
$$
$$
(31) \quad (\lim \sup f) (\lim \inf g) \leq \lim \sup fg
$$

*只要定义了这些不等式的两边。*

(iii) *如果$f \geq 0$在$X$上，那么*

$$
(32) \quad \lim \sup (1/f) = 1/(\lim \inf f)
$$

（放入$1/0 = + \infty$）。

这些关系是命题 12 和关系 (10) 中的推论

#### 推论 1 {#top-iv-s5-prop-13-cor-1 .statement tag=0BRV}

*令$f$和$g$是在过滤后的集合$X$上定义的两个实值函数。如果 $\lim g$ 存在，则*

$$
(33) \quad \lim \sup (f + g) = \lim \sup f + \lim g
$$

每当双方都被定义时，并且

(34) $$
\lim \sup fg = (\lim \sup f) (\lim g)
$$

每当两边都被定义并且$f$和$g$是$\geqslant 0$时。

#### 推论 2 {#top-iv-s5-prop-13-cor-2 .statement tag=0BRW}

令$f$和$g$是在过滤后的集合$X$上定义的两个实值函数。如果定义了$\lim f = +\infty$、$\lim \inf g > -\infty$和$f + g$，则$\lim (f + g) = +\infty$。如果定义了$\lim f = +\infty$、$\lim \inf g > 0$和$fg$，则$\lim fg = +\infty$。

### 习题 {#top-iv-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
