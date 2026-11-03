---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 2
section_title: THE MEAN VALUE THEOREM
lang: zh
source: fvr-i-vii
book_pages: 12-19, 37-39
pdf_pages: 0027-0034, 0052-0054
extraction: ocr
subsections:
    - "no": 1
      title: ROLLE'S THEOREM
      page: 12
      pdf_page: 27
    - "no": 2
      title: THE MEAN VALUE THEOREM FOR REAL-VALUED FUNCTIONS
      page: 13
      pdf_page: 28
    - "no": 3
      title: THE MEAN VALUE THEOREM FOR VECTOR FUNCTIONS
      page: 15
      pdf_page: 30
    - "no": 4
      title: CONTINUITY OF DERIVATIVES
      page: 18
      pdf_page: 33
statements: 21
exercises: 14
content_sha256: c0cf082d74fc691a4f87e5f04c406d28ee6c70e260376f75cf41fc989d3e52ce
translated_from: content/en/fvr/I/02_s2_the_mean_value_theorem.md
translation_method: google
source_content_sha256: cd3afa585ab839f9102101bc5e9f950b6b2590f43edbec61f3394622431f01ca
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: b4e87c76f59896a9b5fa8a12583f1745f14a18c1ca9780bd681fd63bbaff670c
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 2。平均值定理

§ 1 中证明的假设和结论在特征标中是局部的：它们只涉及在固定点的任意小邻域上考虑的函数的性质。相反，我们在截面中处理的问题涉及函数在所有区间上的属性。

### 1. 罗尔的定理

#### 命题 1（“罗尔的定理”）{#fvr-i-s2-prop-1 .statement tag=083Z}

令$f$为实数函数，它在闭区间$I = [a, b]$（其中$a < b$）上是有限且连续的，在]$a, b$[的每个点有一个导数（有限或非），并且使得$f(a) = f(b)$。那么存在]$a, b$[的点$c$使得$f'(c) = 0$。

如果 $f$ 是常数，命题是明显的：如果不是，$f$ 采用，例如值 $> f(a)$，因此在点 $c$ 内部到 I 处达到其最小上界（Gen.1）。 上、IV、p. 359、第。 1）。 由于$f$在点处有相对最大值，我们有$f'(c) = 0$（I，p. 20，道具7）。

#### 推论 {#fvr-i-s2-n1-cor-1 .statement tag=0840}

令$f$为实数函数，它在$[a, b]$（其中$a < b$）上是有限且连续的，并且在每个点有一个导数（有限或非）。那么存在]$a, b$[的点$c$使得$f(b) - f(a) = f'(c)(b - a)$。

我们只需要应用道具。 1 至函数 $f(x) - \frac{f(b) - f(a)}{b - a}(x - a)$。

这个推论表示在$f$的图$C$上存在点$M_c = (c, f(c))$使得$a < c < b$并且$C$在这个点处的切线平行于连接点$M_a = (a, f(a))$的线并且$M_b = (b, f(b))$。

### 2. 实值函数的平均值值定理

下面的重要结果是推论到推论的支撑。 1：如果]$a, b$[上有$m \leq f'(x) \leq M$，那么也有$m \leq \frac{f(b) - f(a)}{b - a} \leq M$。在其他字中，$f'$ 的导数在整个区间上与端点 $a, b$ 的*界限意味着 $\frac{f(b) - f(a)}{b - a}$ 的*相同界限*（函数的“增量”与区间上变量的“增量”之比）。我们将在下文中使这个基本结果更加精确并概括它。

#### 命题 2 {#fvr-i-s2-prop-2 .statement tag=0841}

*设* $f$ *是一个实数函数，它在闭界区间* $I = [a, b]$ *（其中* $a < b$*）上是有限且连续的，并且具有右导数*（有限或非）*在可数的* $[a, b)$ *中的相对补数的点子集* $A$ *其中区间。如果*$f'_d(x) \geq 0$*在*$[a, b[$的每点*不是属于到*$A$，*则有*$f(b) \geq f(a)$； *如果进一步，*$f'_d(x) > 0$*对于*$[a, b[$中的至少一个点，*则*$f(b) > f(a)$。

令$\varepsilon > 0$任意，并用列出可数集合$A$得到的$(a_n)_{n \geq 1}$序列表示。令 $J$ 为点 $y \in I$ 的集合，使得有

$$
f(x) - f(a) \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$

(1)

对于所有$x$和$a \leq x \leq y$，右侧第二个项中的和将取代所有指标$n$，其中$a_n < x$。我们将证明，如果$f'_d(x) \geq 0$在$[a, b[$的每个点与$a_n$不同，则$J = I$。

显然$J$不为空，因为$a \in J$；此外，这个集合的定义表明，如果$y \in J$一个对于$a \leq x \leq y$有$x \in J$，那么$J$是一个*区间*，左端点为$a$（*Gen.Top.*，IV，p. 336，prop. 1）；令 $c$ 为其右侧端点。一个有$c \in J$；如果$c = a$，这很清楚；如果不是，对于每个 $x < c$，我们有不等式 (1)，并且 *更不必说*

$$
f(x) - f(a) \geq -\varepsilon(c - a) - \varepsilon \sum_{a_n < c} \frac{1}{2^n}
$$

由此可见，在这个不等式中让$x$趋于$c$（因为$f$是连续的），$c$满足（1）。

既然如此，我们将看到我们必须有$c = b$。事实上，如果一个人有$c < b$，那么肯定会有$c \notin A$；现在$f'_d(c)$存在，并且由于$f'_d(c) \geq 0$到假设，存在一个$y$使得$c < y \leq b$并且对于$c \leq x \leq y$有一个

$$
f(x) - f(c) \geq -\varepsilon(x - c)
$$

其中，考虑到 (1)，其中 $x$ 被 $c$ 替代，

$$
f(x) - f(a) \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < c} \frac{1}{2^n} \geq -\varepsilon(x - a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$

这表示$y \in J$，与$c$的定义矛盾。因此，对于某些指标 $k$，我们有 $c = a_k$；因为 $f$ 在点 $a_k$ 处连续，所以存在一个 $y$ 使得 $c < y \leq b$ 并且对于 $c < x \leq y$ 有一个
$$
f(x) - f(c) \geq -\frac{\varepsilon}{2^k}
$$
其中，考虑到 (1)，其中 $x$ 被 $c$ 替代，
$$
f(x) - f(a) \geq -\varepsilon(c-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n} \geq -\varepsilon(x-a) - \varepsilon \sum_{a_n < x} \frac{1}{2^n}
$$
这又导致了矛盾；因此我们有$c = b$，并且在推论
$$
f(b) - f(a) \geq -\varepsilon(b-a) - \varepsilon \sum_{a_n < b} \frac{1}{2^n} \geq -\varepsilon(b-a) - \varepsilon. \tag{2}
$$
由于$\varepsilon > 0$是任意的，我们从(2)推导出$f(b) \geq f(a)$，它演示了命题的第一个部分。

我们现在注意到这个结果适用于区间$[x, y]$，其中$a \leq x < y \leq b$证明$f$是I上的*递增*；如果有$f(b) = f(a)$，可以推断出$f$在I上是“常数”，然后在$[a, b[$的每点处都有$f'_d(x) = 0$；第二个部分由此而来。

#### 推出 {#fvr-i-s2-n2-cor-1 .statement tag=0842}

*设$f$是$[a, b]$（其中$a < b$）上的有限连续实数函数，并且对这个区间的可数子集$A$的$[a, b[$中的补集有一个右导数点。为了使$f$在I上成为递增，$f'_d(x) \geq 0$在$[a, b[$的每个点处是必要且充分的，而不是属于到$A$；为了使$f$成为严格递增的，前面的条件成立是必要且充分的，并且点$x$的集合成立，其中$f'_d(x) > 0$在$[a, b]$中稠密。*

#### 注 1 {#fvr-i-s2-n2-rem-1 .statement tag=0843}

当替换区间 $[a, b[$ 通过 ]$a, b$ 和字 “右导数”通过“左导数”时，命题 2 仍然成立。

#### 注 2 {#fvr-i-s2-n2-rem-2 .statement tag=0844}

区间 I 上$f$ 上的*连续性* 假设（而不仅仅是$[a, b[$ 的每个点上的*正确连续性* $^4$）对于道具的有效性至关重要。 2（*cf.* I、p. 36、练习 8）。

#### 注 3 {#fvr-i-s2-n2-rem-3 .statement tag=0845}

道具的结论。如果仅仅假设“例外”点的集合$A$在I中不密集，但不可数（*cf.*I，p. 37，练习3），则不能保证2。

命题 2 包含以下基本原理定理（这似乎更一般）：

**定理 1**（指值定理）。 *设$f$和$g$是两个有限连续实值函数，定义在闭有界区间$I = [a, b]$上，并且具有

如果限制到区间$I \cap [x_0, +\infty[$相对于此在点$x_0$连续，则在区间$I \subset \mathbf{R}$上定义的$^4$函数被称为在点$x_0 \in I$*右连续* 区间；同样的，这个函数的右极限存在于这个点，并且等于函数的值在这个点。

该区间的可数子集 $[a,\ b[$ 中相对补集的所有点的右导数（有限或非有限）。 进一步假设 $f'_d(x)$ 和 $g'_r(x)$ 不同时无限，除了 I 的可数子集的点处，并且存在有限数 $m$、$M$，使得

$$
mg'_r(x) \leq f'_d(x) \leq Mg'_r(x)
$$

除了 I (替换 $Mg'_r(x)$ (分别为 $mg'_r(x)$) 的可数子集的点处，如果 $M = 0$ (分别为 $m = 0$) 和 $g'_r(x) = \pm \infty$。在这些条件下，有一个

$$
m(g(b) - g(a)) < f(b) - f(a) < M(g(b) - f(a))
$$

除非对于所有 $x \in I$ 都有 $f(x) = Mg(x) + k$ 或 $f(x) = mg(x) + k$（$k$ 常数）。

应用 prop 就足够了。 2 到函数 $Mg - f$ 和 $f - mg$，根据我们的假设，除了 I 的可数子集的点之外，它们具有正的右导数。

#### 注 {#fvr-i-s2-n2-rem-4 .statement tag=0846}

Th。如果允许 $f'_d$ 和 $g'$ 在I 的不可数子集上同时无限（cf. I，p. 37，执行 3），则 1 失败。

#### 推论 {#fvr-i-s2-n2-cor-2 .statement tag=0847}

设$f$是$[a,\ b]$（其中$a < b$）上的有限连续函数，并且在该区间的可数子集的$[a,\ b[$中具有相对补B的右导数（有限或非）点。如果 $m$ 和 $M$ 比最大的低，并且 B 上的 $f'_d$ 至少有上界，则有

$$
m(b - a) < f(b) - f(a) < M(b - a)
$$

如果 $f$ 不是仿射线性函数；如果 $f$ 是仿射线性的，则有

$$
m = M = \frac{f(b) - f(a)}{b - a}.
$$

当$m$和$M$有限时，不等式(5)是(4)的推论；当这些数中的一个或另一个是无限时的情况是微不足道的。

#### 注 {#fvr-i-s2-n2-rem-5 .statement tag=0848}

不等式(5)证明连续函数不能在区间的所有点处具有等于$+\infty$的右导数（cf.I，p. 38，练习6）。

### 3. 向量函数的平均值值定理

#### 定理 2 {#fvr-i-s2-thm-2 .statement tag=0849}

令 $f$ 定义为向量函数，并在 $\mathbf{R}$（其中 $a < b$）的闭有界区间 $I = [a,\ b]$ 上定义且连续，并在 $\mathbf{R}$ 上的规范化空间 E 中取值；设$g$是I上连续的递增实数函数。假设$f$和$g$在区间的可数子集A的$[a,\ b[$中的相对补集点有右导数（允许$g'_r(x)$在点$x \notin A$的某些处无限），并假设在每一个点我们有

$$
\| f'_d(x) \| \leq g'_r(x).
$$

在这些假设下，人们有

$$
\| f(b) - f(a) \| \leq g(b) - g(a).
$$

证明的处理方式与 prop 类似。 2. 令$\varepsilon > 0$任意，并通过枚举某个阶中的A得到$(a_n)$序列。令 J 为点 $y \in I$ 的集合，使得对于所有 $x$ 使得 $a \leq x \leq y$ 有

$$
\| f(x) - f(a) \| \leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n};
$$

我们将证明$J = I$。人们立即看到，就像在道具中一样。 2、J 为区间，左端点为$a$；如果 c 是其右侧端点，则 $c \in J$；事实上，对于所有 $x < c$ 都有 (8)，并且 *更不必说*

$$
\| f(x) - f(a) \| \leq g(c) - g(a) + \varepsilon (c - a) + \varepsilon \sum_{a_n < c} \frac{1}{2^n}
$$

由此，在不等式中让$x$趋向于$c$，则根据$f$的连续性，$c$满足(8)。

让我们证明我们必须有 $c = b$。因此，假设$c < b$和$c \notin A$：则$f'_d(c)$和$g'_r(c)$存在且满足 (6)；首先假设$g'_r(c)$（必然是$\geq 0$）是有限的；那么我们总是可以写 $f'_d(c) = u g'_r(c)$，与 $\| u \| \leq 1$；由于函数$f(x) - u g(x)$在点$c$有零右导数，因此必须存在$y$使得$c < y \leq b$并且对于$c \leq x \leq y$有一个

$$
\| f(x) - f(c) - u(g(x) - g(c)) \| \leq \varepsilon (x - c)
$$

从中

$$
\| f(x) - f(c) \| \leq g(x) - g(c) + \varepsilon (x - c)
$$

并且，考虑到 (8)，其中 $x$ 被 $c$ 替代，

$$
\begin{align*}
\| f(x) - f(a) \| &\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < c} \frac{1}{2^n} \\
&\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}.
\end{align*}
$$

因此有$y \in J$，这是一个矛盾。接下来假设$c \notin A$和$g'_r(c) = +\infty$；那么有一个$y$使得$c < y \leq b$并且对于$c \leq x \leq y$一方面有

$$
\| f(x) - f(c) \| \leq (\| f'_d(c) \| + 1) (x - c)
$$

另一方面

$$
g(x) - g(c) \geq (\| f'_d(c) \| + 1) (x - c)
$$

从中

$$
\| f(x) - f(c) \| \leq g(x) - g(c)
$$

和一个如上所述的结论。最后，如果有 $c = a_k$，则存在 $y$，使得 $c < y \leq b$，并且对于 $c < x \leq y$，有

$$
\| f(x) - f(c) \| \leq \frac{\varepsilon}{2^k}
$$

由此，考虑(8)，用$x$替换为$c$，

$$
\begin{align*}
\| f(x) - f(a) \| &\leq g(c) - g(a) + \varepsilon (c - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n} \\
&\leq g(x) - g(a) + \varepsilon (x - a) + \varepsilon \sum_{a_n < x} \frac{1}{2^n}
\end{align*}
$$

这又产生了矛盾。 证明与道具相同。 2.

Q.E.D.

#### 注 1 {#fvr-i-s2-n3-rem-1 .statement tag=084A}

再次，在第叙述中。 2 可以通过 ]$a, b]$ 计算替换区间 $[a, b[$，并通过“左导数”计算“右导数”。

#### 注 2 {#fvr-i-s2-n3-rem-2 .statement tag=084B}

稍后我们将展示如何识别（7）中的相等情况，以及如何推广它。 2 到 E 是任意局部凸空间的情况，借助另一种证明方法可以推导出 th。 2 从 th. 1.

#### 推出 {#fvr-i-s2-n3-cor-1 .statement tag=084C}

对于区间 $I \subset \mathbf{R}$上的连续向量函数，其中值位于$\mathbf{R}$上的范数空间E中，要在I上保持不变，只要它在补集的所有点上具有零右导数就足够了（相对于I）I的可数子集。

#### 注 {#fvr-i-s2-n3-rem-3 .statement tag=084D}

其中证明。 1和2本质上依赖于域$\mathbf{R}$的特殊拓扑性质；可以给出值域 K 的例，其中 K 对其自身存在非常数线性映射，并且在每点具有零导数（cf. I、p. 37，练习 2）。

#### 命题 3 {#fvr-i-s2-prop-3 .statement tag=084E}

令$f$为向量函数，其中值位于$\mathbf{R}$上的范数空间E中，在区间$I \subset \mathbf{R}$上定义且连续，并且在可数子集的补集B（相对于I）上右可微I；那么对于所有点 $x_0 \in B, x \in I, y \in I$，有一个（例如假设 $x < y$）

$$
\| f(y) - f(x) - f'_d(x_0)(y - x) \| \leq (y - x) \sup_{z \in B, x < z < y} \| f'_d(z) - f'_d(x_0) \|.
$$ (9)

事实上，应用 th 就足够了。 2、替换$f$乘函数

$$
f(z) - f'_d(x_0)z,
$$

$g$ 由线性函数求导，其导数为 $\sup_{z \in B, x < z < y} \| f'_d(z) - f'_d(x_0) \|$。

复变量的定理 2 扩展到向量函数：

#### 命题 4 {#fvr-i-s2-prop-4 .statement tag=084F}

*令$f$为定义在域$\mathbf{C}$的凸开子集$A$上的复变量的连续可微函数，其中值位于域上的赋范空间$E$中$\mathbf{C}$。如果一个人对所有 $z \in A$ 都有 $\|f'(z)\| \leq m$，那么对点 $a, b$ $A$ 的每一个对都有 $\|f(b) - f(a)\| \leq m |b - a|$。*

我们用$g(t) = \frac{1}{b - a} f(a + t(b - a))$代替$0 \leq t \leq 1$；从$g'(t) = f'(a + t(b - a))$、应用日起。 2 到函数 $g$ 立即产生命题。

#### 推出 {#fvr-i-s2-n3-cor-2 .statement tag=084G}

*对于复数变量的向量函数$f$，在开集合$A \subset \mathbf{C}$上定义且连续，并且值在$\mathbf{C}$上的规范化空间中，要保持不变，只要它在每个零导数就足够了点共 $A$。*

事实上，让$a$是$A$的任意点； 集合 $B$ 点 $z$ $A$ 其中$f(z) = f(a)$ *封闭*，因为$f$ 是连续的；它也是*开放的*，如应用属性所示。 4（与$m = 0$）到凸开邻域，包含在$A$中，具有$B$的任意点；所以与 $A$ 相同。

#### 命题 5 {#fvr-i-s2-prop-5 .statement tag=084H}

*设$f$为复变量的向量函数，在凸开集合$A \subset \mathbf{C}$上定义、连续且可微，在域$\mathbf{C}$上将值取为范数空间；那么，无论 $A$ 中的点 $x_0, x$ 和 $y$ 是什么，都有*
$$
\|f(y) - f(x) - f'_d(x_0)(y - x)\| \leq |y - x| \sup_{z \in A} \|f'(z) - f'(x_0)\|.
$$
(10)

应用th就足够了。 2至函数
$$
g(t) = f(x + t(y - x)) - f'(x_0)(y - x)t
$$
在区间$[0, 1]$。

### 4. 衍生品的连续性

#### 命题 6 {#fvr-i-s2-prop-6 .statement tag=084I}

*设$I$为$\mathbf{R}$中的开区间，令$x_0$为$I$的端点之一，$f$向量函数在$I$上定义且连续，值为完全范数空间$E$超过$\mathbf{R}$；假设$f$在点处有$I$的可数子集的$I$补集$B$的右导数。那么对于$f'_d(x)$有极限，因为$x$趋向于$x_0$，同时保持在$B$和$\neq x_0$，$\frac{f(y) - f(x)}{y - x}$有极限$c$是充分必要的，因为$(x, y)$趋向于$(x_0, x_0)$ 受$x \in I, y \in I, x \neq x_0, y \neq x_0$ 和$x \neq y$ 约束。在这些条件$f$扩展下，通过连续到点$x_0$，右导数$f'_d(x)$趋于$c$，因为$x$趋于$x_0$（同时保留在B中）和函数 $f$扩展（在$I \cup \{x_0\}$上定义）在$x_0$处的导数等于$c$。

例如，假设 $x_0$ 是 I 的右侧端点。让我们首先证明，如果$f'_d(x)$趋向于$c$，就像$x$趋于$x_0$一样，同时保留在B和$\neq x_0$中，那么$\frac{f(y) - f(x)}{y - x}$趋向于$c$；这紧随 th 而来。 2 应用于函数 $f(z) - cz$，得出

$$
\| f(y) - f(x) - c(y - x) \| \leq (y - x) \sup_{z \in B,\ x < z < y} \| f'_d(z) - c \|
$$

$x < y < x_0$。相反，如果 $\frac{f(y) - f(x)}{y - x}$ 趋于 $c$，则对于每个 $\varepsilon > 0$ 都存在一个 $h > 0$，使得条件 $|x - x_0| < h,\ |y - x_0| < h\ (x \neq x_0,\ y \neq x_0)$ 意味着

$$
\| f(y) - f(x) - c(y - x) \| \leq \varepsilon |y - x|.
$$

但对于所有$x \in B$和$\neq x_0$，使得$|x - x_0| < h$存在$k > 0$（取决于$x$），使得关系$x < y < x + k$需要

$$
\| f(y) - f(x) - f'_d(x)(y - x) \| \leq \varepsilon |y - x|
$$

由此，考虑 (11)：

$$
\| f'_d(x) - c \| \leq 2\varepsilon
$$

对于 $|x - x_0| < h,\ x \in B$ 和 $x \neq x_0$。这就证明了$f'_d(x)$趋于$c$。此外，从关系 (11) 可以立即得知

$$
\| f(y) - f(x) \| \leq (\|c\| + \varepsilon) |y - x|,
$$

这证明（根据柯西准则）$f$在点$x_0$处具有极限$d$，因为$x$趋向于点，同时保持在I和$\neq x_0$；现在，让$x$逼近(11)中的$x_0$，对于$y \in I,\ y \neq x_0$和$|y - x_0| \leq h$，我们有

$$
\left\| \frac{f(y) - d}{y - x_0} - c \right\| \leq \varepsilon
$$

这就证明了$c$是函数$f$在点$x_0$处的导数通过连续性延伸到$I \cup \{x_0\}$。

#### 注 {#fvr-i-s2-n4-rem-1 .statement tag=084J}

类似的论点，基于 th。 1，表明如果 $f$ 是实数函数，使得 $f'_d(x)$ 在点 $x_0$ 趋向于 $+\infty$，则比率

$$
(f(y) - f(x))/(y - x)
$$

也趋于$+\infty$，反之亦然；此外，如果$f$在点$x_0$处有一个有限的极限（不是当前假设的推论），则函数$f$通过连续性扩展到$x_0$，在以下位置有等于$+\infty$的导数这个点。

### 习题 {#fvr-i-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
