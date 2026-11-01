---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 4
section_title: CONVEX FUNCTIONS OF A REAL VARIABLE
lang: zh
source: fvr-i-vii
book_pages: 23-33, 45-49
pdf_pages: 0038-0048, 0060-0064
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A CONVEX FUNCTION
      page: 24
      pdf_page: 39
    - "no": 2
      title: FAMILIES OF CONVEX FUNCTIONS
      page: 27
      pdf_page: 42
    - "no": 3
      title: CONTINUITY AND DIFFERENTIABILITY OF CONVEX FUNCTIONS
      page: 27
      pdf_page: 42
    - "no": 4
      title: CRITERIA FOR CONVEXITY
      page: 30
      pdf_page: 45
statements: 23
exercises: 25
content_sha256: 505f7f1fb1065a86a1bb8ec6895319008a189042f312d65ffbd261ffdd5c4c4c
translated_from: content/en/fvr/I/04_s4_convex_functions_of_a_real_variable.md
translation_method: google
source_content_sha256: f3bb356dcd01c2f124b6edbcb7551016f358669cd0b6cfe2c6628e4d9303177e
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 758f10a23eac38a355b2d46b5f13fd2b9e9190b95e026593d0d03e81f29567ea
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。实变量的凸函数

设$H$为$\mathbf{R}$的子集。 $f$定义在$H$上的有限实数函数，令$G$为点$M_x = (x, f(x))$的$\mathbf{R} \times \mathbf{R} = \mathbf{R}^2$、集合中函数$f$的*图*或代表集合，其中$x$贯穿$H$。可以方便地说，$\mathbf{R}^2$的点$(a, b)$使得$a \in H$位于*上方*（分别为*严格上方*、*下方*、*严格下方*）$G$，如果有$b \geq f(a)$（分别为$b > f(a)$、$b \leq f(a)$、 $b < f(a)$）。如果$A = (a, a')$和$B = (b, b')$是$\mathbf{R}^2$的两个点，我们用$AB$表示端点为$A$和$B$的封闭线段；如果$a < b$，则$AB$是在$[a, b]$上定义的线性函数$a' + \frac{b' - a'}{b - a} (x - a)$的图；我们用$p(AB)$表示该段的斜率$\frac{b' - a'}{b - a}$，并将使用以下引理，其验证为直接的：

#### 引理 {#fvr-i-s4-n0-lem-1 .statement tag=085O}

*令$A = (a, a')$、$B = (b, b')$、$C = (c, c')$为$\mathbf{R}^2$中的三个点，使得$a < b < c$。以下叙述是等效的：*

a) *B 低于 AC；*
b) *C位于通过A和B的线经过之上；*
c) *位于通过 B 和 C 的线经过之上；*
d) $p(AB) \leq p(AC)$；
e) $p(AC) \leq p(BC)$。

当替换“之上”（或“之下”）乘以“严格之上”（或“严格之下”）且符号 $\leq$ 乘以 < 时，引理仍然成立（图 1）。

![图表显示点 A、B、C 和段标记为 x 值 a、b、c](../images/fig_1.png)

图1

### 1.凸面的定义函数

#### 定义 1 {#fvr-i-s4-def-1 .statement tag=085P}

我们说，在区间 $I \subset \mathbf{R}$ 上定义的有限数值函数 $f$，在 $I$ 上是凸的，如果，无论 $I$ 的点 $x, x'$，($x < x'$)，每点 $M_z$ $f$的图$G$，使得$x \leq z \leq x'$位于线段$M_xM_{x'}$下方（或者，如果该线段的每个点位于$G$上方，结果相同）（图2）。

![图表显示点 M_x、M_z、M_{x'} 和曲线 G](../images/fig_2.png)

图2

考虑到线段的参数表示（Gen.Top.、VI、p. 35），$f$在I上凸的条件意味着有不等式

$$
f(\lambda x + (1 - \lambda)x') \leq \lambda f(x) + (1 - \lambda)f(x')
$$

对于点中的每对、I中的$(x, x')$以及每$\lambda \in [0, 1]$。

定义 1 等价于：*位于$f$的图G之上的$\mathbf{R}^2$中的点的集合是凸的*。事实上，这个条件显然足以让$f$在I上凸；这也是必要的，因为如果$f$在I上凸，并且$(x, y), (x', y')$是位于G上方的两个点，则其中一个有$y \geq f(x),\ y' \geq f(x')$，从中，对于$0 \leq \lambda \leq 1$，

$$
\lambda y + (1 - \lambda)y' \geq \lambda f(x) + (1 - \lambda)f(x') \geq f(\lambda x + (1 - \lambda)x')
$$

由(1)可知，端点为$(x, y)$和$(x', y')$的线段的每个点都位于G之上。

#### 注 {#fvr-i-s4-n1-rem-1 .statement tag=085Q}

以同样的方式，点的集合位于*严格上方*G 是凸的。相反，如果这个集合是凸的，则有

$$
\lambda y + (1 - \lambda)y' > f(\lambda x + (1 - \lambda)x')
$$

对于 $0 \leq \lambda \leq 1$ 和 $y > f(x),\ y' > f(x')$；在这个公式中，让y趋向$f(x)$并且$y'$接近$f(x')$，可以得出$f$是凸的。

#### 例 1 {#fvr-i-s4-n1-exa-1 .statement tag=085R}

每个（实数）仿射线性函数 $ax + b$ 在 $\mathbf{R}$ 上都是凸的。

#### 例 2 {#fvr-i-s4-n1-exa-2 .statement tag=085S}

函数 $x^2$ 在 $\mathbf{R}$ 上是凸的，因为有

$$
\lambda x^2 + (1 - \lambda)(x')^2 - \left( \lambda x + (1 - \lambda)x' \right)^2 = \lambda(1 - \lambda)(x - x')^2 \geq 0
$$

$0 \leq \lambda \leq 1$。

#### 例 3 {#fvr-i-s4-n1-exa-3 .statement tag=085T}

函数 $|x|$ 在 $\mathbf{R}$ 上是凸的，因为

$$
|\lambda x + (1 - \lambda)x'| \leq \lambda |x| + (1 - \lambda)|x'|
$$

$0 \leq \lambda \leq 1$。

很明显，如果$f$在I上凸，那么它的限制到任何区间$J \subset I$在J上都是凸的。

令$f$是I上的凸函数，并且$x, x'$是I的两个点，使得$x < x'$；如果$z \in I$是$[x, x']$的*外部*，则$M_z$位于连接$M_x$和$M_{x'}$的线D*之上；这是引理中的直接的推论。

由此推断，如果$z$是点，使得$x < z < x'$并且使得$M_z$位于线段$M_x M_{x'}$*上，那么，对于*所有其他点*$z'$使得$x < z' < x'$点 $M_{z'}$ 也位于*线段 $M_x M_{x'}$ 上，因为从上面可以得出，$M_{z'}$ 同时位于该线段的上方和下方；在其他字中，$f$等于$[x, x']$上的*仿射线性*函数。

#### 定义 2 {#fvr-i-s4-def-2 .statement tag=085U}

*我们说，在区间$I \subset \mathbf{R}$上定义的有限实数函数$f$在I上严格凸，如果对于I（$x < x'$）的任何点$x, x'$，图的每个点$M_z$ $f$ 的 G，使得 $x < z < x'$ 严格位于线段 $M_x M_{x'}$ 之下（或者，如果除了端点之外，线段的每个点都严格位于 G 之上）。*

在其他字，我们必须有不等式

$$
f(\lambda x + (1 - \lambda)x') < \lambda f(x) + (1 - \lambda)f(x')
$$

对于$I$的不同点$(x, x')$的每个对以及每个$\lambda$使得$0 < \lambda < 1$。

注位于 def 之前。图 2 显示，对于凸函数 $f$ 在 $I$ 上严格凸，$I$ 中不包含任何区间（不减少到单个点）是必要且充分的，使得 $f$ 的限制与该区间是*仿射线性*。

上述例中，第一个和第三个不是严格凸的；另一方面，$x^2$在$\mathbf{R}$上严格凸；类似的计算表明 $1/x$ 在 $[0, +\infty[$ 上严格凸。

#### 命题 1 {#fvr-i-s4-prop-1 .statement tag=085V}

*令 $f$ 为区间 $I \subset \mathbf{R}$ 上的凸（或严格凸）有限实数函数。对于$p \geq 2$的每个家庭$(x_i)_{1 \leq i \leq p}$与$I$不同的点，以及$p$实数的每个家庭$(\lambda_i)_{1 \leq i \leq p}$，这样$0 < \lambda_i < 1$和$\sum_{i=1}^p \lambda_i = 1$，我们有*

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i)
$$

（分别。

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i)).
$$

由于命题（对于凸函数）约化到不等式（1）对于$p = 2$，我们用归纳来论证$p > 2$。 数$\mu = \sum_{i=1}^{p-1} \lambda_i$为$> 0$；如果$a$和$b$分别是$x_i$的最小的和最大的，那么$a \leq \frac{\sum_{i=1}^{p-1} \lambda_i x_i}{\sum_{i=1}^{p-1} \lambda_i} \leq b$就是直接的；在其他字，点$x = \frac{1}{\mu} \sum_{i=1}^{p-1} \lambda_i x_i$属于到$I$，归纳假设暗示$\mu f(x) \leq \sum_{i=1}^{p-1} \lambda_i f(x_i)$；此外，从（1）我们有

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) = f(\mu x + (1 - \mu)x_p) \leq \mu f(x) + (1 - \mu)f(x_p) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

人们以同样的方式论证严格凸函数，从不等式 (2) 开始。

我们说，如果 $-f$ 在 $I$ 上是凸（或严格凸），则有限实数函数 $f$ 在 $I$ 上是*凹*（或*严格凹*）。同样的说法，对于$I$的不同点的每个对$(x, x')$和每个$\lambda$，使得$0 < \lambda < 1$有一个

$$
f(\lambda x + (1 - \lambda)x') \geq \lambda f(x) + (1 - \lambda)f(x')
$$

（分别$f(\lambda x + (1 - \lambda)x') > \lambda f(x) + (1 - \lambda)f(x')$）。

### 2.凸家族函数

#### 命题 2 {#fvr-i-s4-prop-2 .statement tag=085W}

令 $f_i$ ($1 \leq i \leq p$) 为 $p$ 在区间 $I \subset \mathbf{R}$ 上凸函数，且 $c_i$ ($1 \leq i \leq p$) 为 $p$ 任意正数；那么函数$f = \sum_{i=1}^p c_i f_i$在$I$上是凸的。此外，如果对于至少一个指标$j$函数$f_j$在$I$和$c_j > 0$上严格凸，则$f$在$I$上严格凸。

接下来紧接着将应用不等式 (1) （或 (2)） 与每个 $f_i$ 相乘，将 $f_i$ 的不等式乘以 $c_i$，然后逐项相加。

#### 命题 3 {#fvr-i-s4-prop-3 .statement tag=085X}

令 $(f_\alpha)$ 为区间 $I \subset \mathbf{R}$ 上的凸函数族；如果该族的上包络$g$在$I$的每个点处是有限的，则$g$在$I$上是凸的。

事实上，位于$g$图上方的点$(x, y) \in \mathbf{R}^2$的集合是位于函数$f_\alpha$图上方的点形成的凸集合的交；所以它是凸的。

#### 命题 4 {#fvr-i-s4-prop-4 .statement tag=085Y}

设$H$是凸函数在区间$I \subset \mathbf{R}$上的集合；如果$\mathfrak{F}$是$H$上的一个滤波器，它在$I$上逐点收敛到有限实数函数$f_0$，那么这个函数在$I$上是凸的。

要看到这一点，只需在不等式 (1) 中沿着 $\mathfrak{F}$ 传递到极限即可。

### 3.凸函数的连续性和可微性

#### 命题 5 {#fvr-i-s4-prop-5 .statement tag=085Z}

对于实数有限函数$f$在区间$I$上凸（或严格凸），对于所有$a \in I$梯度是必要且充分的

$$
p(M_a M_x) = \frac{f(x) - f(a)}{x - a}
$$

$I \cap \mathbf{C}\{a\}$ 上的$x$ 为递增（分别为严格递增的）函数。

这个命题是定义1和2的直接的推论以及I、p. 23的引理。

#### 命题 6 {#fvr-i-s4-prop-6 .statement tag=0860}

令 $f$ 为区间 $I \subset \mathbf{R}$ 上的有限实数函数凸。那么在 $I$ 函数 $f$ 的每个内部点 $a$ 都是连续的，具有有限的右导数和左导数，以及 $f'_g(a) \leq f'_d(a)$。

事实上，对于 $x \in I$ 和 $x > a$ 函数 $x \mapsto \frac{f(x) - f(a)}{x - a}$ 是递增 （命题 5）并且有界如下，因为如果 $y < a$ 和 $y \in I$ 我们有

$$
\frac{f(y) - f(a)}{y - a} \leq \frac{f(x) - f(a)}{x - a}
$$
(5)

通过道具。 5；因此，这个函数在点$a$拥有有限的权利极限；在其他字中，$f'_d(a)$存在并且是有限的；进一步，令(5)中$x$逼近$a$($x > a$)，可得

$$
\frac{f(y) - f(a)}{y - a} \leq f'_d(a)
$$
(6)

适用于所有 $y < a$ 属于至 I。以同样的方式证明 $f'_g(a)$ 存在且

$$
f'_d(a) \leq \frac{f(x) - f(a)}{x - a}
$$
(7)

对于 $x \in I$ 和 $x > a$。在最后一个不等式中让$x$逼近$a$（$x > a$），我们得到$f'_g(a) \leq f'_d(a)$。 点$a$处左右导数的存在显然保证了$f$在此点的连续性。

#### 推论 1 {#fvr-i-s4-prop-6-cor-1 .statement tag=0861}

*令 $f$ 为 I 上的凸（或严格凸）函数；如果$a$和$b$是I的两个内部点，使得$a < b$其中一个有*（图3）

![显示凸函数的图，其切线位于点 a 和 b，分别标记为 M_a 和 M_b。](../images/fig_3.png)

图3

$$
f'_d(a) \leq \frac{f(b) - f(a)}{b - a} \leq f'_g(b)
$$
(8)

（分别。

$$
f'_d(a) < \frac{f(b) - f(a)}{b - a} < f'_g(b)
$$
(9)

双不等式 (8) 由 (6) 和 (7) 通过简单的变换记号得到。另一方面，如果 $f$ 是严格凸的并且 $c$ 使得 $a < c < b$ 有，从 (8) 和 prop. 5、

$$
f'_d(a) \leq \frac{f(c) - f(a)}{c - a} < \frac{f(b) - f(a)}{b - a} < \frac{f(b) - f(c)}{b - c} \leq f'_g(b)
$$

从中（9）。

#### 推论 2 {#fvr-i-s4-prop-6-cor-2 .statement tag=0862}

*如果$f$在I上凸（或严格凸），则$f'_d$和$f'_g$在I的内部是递增（或严格递增的）； $f$不可微分的I中的点的集合是可数的，$f'_d$和$f'_g$在点处连续，其中$f$可微分。*

第一个部分紧接着 (8)（分别是 (9)）和不等式

$$
f'_g(a) \leq f'_d(a).
$$

另一方面，令 E 为 I 内部点 $x$ 的集合，其中 $f$ 不可微（即 $f'_g(x) < f'_d(x)$）。对于每个 $x \in E$ 令 $J_x$ 为开区间 $]f'_g(x), f'_d(x)[$；由(8)得出，如果$x$和$y$是E的两个点，使得$x < y$，则$u < v$对于所有$u \in J_x$和所有$v \in J_y$；在其他字中，由于$x$穿过E，开非空间隔$J_x$是成对的不相交的；因此，这样的间隔中的集合是可数的，因此E也是可数的。最后，$f'_d$（分别为$f'_g$）为递增，它在I的每个内部点$x$处都有一个右极限和一个左极限；支柱。 I、p. 18 的 6 现在显示$f'_d$（或$f'_g$）的右侧极限在点 $x$ 等于$f'_d(x)$，而其左侧极限为$f'_g(x)$，由此我们得到了推论的最后一个部分。

设$f$是I上的凸函数，$a$是I的内部点，并且D是经过穿过点$M_a$的直线，方程为$y - f(a) = \alpha(x - a)$。从不等式 (8) 可以得出，如果 $f'_g(a) \leq \alpha \leq f'_d(a)$，则图 G 的每个点都位于 D *之上*，并且，如果 $f$ 严格凸，则 $M_a$ 是 D 和 G 的唯一点公共的；有人说 D 是 G 的一条*支撑线*，位于点 $M_a$。相反，如果 G 位于 D 之上，则每个 $x \in I$ 都有 $f(x) - f(a) \geq \alpha(x - a)$，其中 $x > a$ 为 $\frac{f(x) - f(a)}{x - a} \geq \alpha$，$\frac{f(x) - f(a)}{x - a} \leq \alpha$ 为 $x < a$；在这些不等式中，让 $x$ 趋向于 $a$，可以得出 $f'_g(a) \leq \alpha \leq f'_d(a)$。

特别是，如果 $f$ 在点 $a$ 处可微，则在点 $M_a$ 处*只有一条*支持 G 线，即 G 在 $M_a$ 处的*切线*。

#### 注 {#fvr-i-s4-n3-rem-1 .statement tag=0863}

如果$f$是开区间I上的严格凸函数，则$f'_d$是I上的严格递增的，因此根据prop，存在三种可能的情况。 I、p. 13 中的 2 个：
1. $f$ 是 I 上的严格递减；
2. $f$在I上是严格递增的；
3. 存在一个$a \in I$，使得$f$对于$x \leq a$来说是严格递减，对于$x \geq a$来说是严格递增的。

当$f$在I上凸，但不是严格凸时，$f$可以在I所包含的区间上恒定；设$J = ]a, b[$为最大的开区间，其中$f$为常数（即$f'_d(x) = 0$所在区间的内部）；那么$f$在点$x \in I$形成的区间上是严格递减使得$x \leq a$（如果存在），严格递增的在点$x \in I$形成的区间上使得$x \geq b$（如果存在）。

在所有情况下，我们都可以看到$f$在$I$（在$\overline{\mathbf{R}}$）的左端点拥有*右极限*，并且在右端点拥有*左极限*；这些极限可能是有限的或无限的（*cf.* I、p. 46、练习 5、6 和 7）。通过滥用语言，有时说，连续函数（$\overline{\mathbf{R}}$中的值）等于$I$内部的$f$，并通过连续性延伸到$I$的端点，是*$\overline{I}$上的*凸。

### 4. 判据凸性

#### 命题 7 {#fvr-i-s4-prop-7 .statement tag=0864}

*令 $f$ 为定义在区间 $I \subset \mathbf{R}$ 上的有限实数函数。为了使$f$在$I$上凸，对于数$a, b$的$I$的每个对，使得$a < b$，并且对于每个实数$\mu$，函数是必要和充分的$f(x) + \mu x$ 在 $[a, b]$ 点 $a, b$ 之一达到其最高值。*

条件是*必要的*；事实上，由于$\mu x$在$\mathbf{R}$上凸，所以函数$f(x) + \mu x$在$I$上凸；因此，我们可以将自己局限于案例$\mu = 0$。那么，对于
$$
x = \lambda a + (1 - \lambda) b \quad (0 \leq \lambda \leq 1),
$$
一个有
$$
f(x) \leq \lambda f(a) + (1 - \lambda) f(b) \leq \operatorname{Max}(f(a), f(b)).
$$

条件*足够*。让我们取 $\mu = -\frac{f(b) - f(a)}{b - a}$ 并令 $g(x) = f(x) + \mu x$；一个人有 $g(a) = g(b)$，因此对于所有 $x \in [a, b]$ 都有 $g(x) \leq g(a)$，并且可以立即检查该不等式是否等于不等式 (1)，其中一个替换 $z$ 由 $a$ 和 $x'$ 组成$b$。

#### 命题 8 {#fvr-i-s4-prop-8 .statement tag=0865}

*对于开区间$I \subset \mathbf{R}$上的有限实数函数$f$来说，它是凸（或严格凸）的，它在$I$上连续是必要且充分的，在补集$B$相对于可数的$I$的每个点都有一个导数该区间的子集，并且在 $B$ 上的导数为递增（分别为严格递增的）。*

条件是必要的，来自 prop。 6及其推论2（I，p. 27）；让我们证明这已经足够了。因此，假设$f'$是$B$上的递增，并且$f$不是凸的；那么存在（I，p. 27，道具5）$I$的三个点$a, b, c$，使得$a < c < b$和$\frac{f(c) - f(a)}{c - a} > \frac{f(b) - f(c)}{b - c}$；但从平均值定理 (I, p. 14, th. 1) 来看，有
$$
\frac{f(c) - f(a)}{c - a} \leq \sup_{x \in B,\ a < x < c} f'(x) \quad \text{and} \quad \frac{f(b) - f(c)}{b - c} \geq \inf_{x \in B,\ c < x < b} f'(x).
$$

因此，一个人有$\sup_{\lambda \in B,\ a < \lambda < c} f'(\lambda) > \inf_{\lambda \in B,\ c < \lambda < b} f'(\lambda)$，与假设相反，$f'$是$B$上的递增。

如果现在我们假设$f'$在$B$上是严格递增的，那么$f$是凸的，并且不能等于$I$中包含的任何开区间上的仿射线性函数，因为$f'$在这个区间上将是常数，与假设相反。

#### 推论{#fvr-i-s4-n4-cor-1 .statement tag=0866}

*令$f$为有限实数函数，连续且在区间$I \subset \mathbf{R}$上可微分；对于$f$在$I$上凸，$f''(x) \geqslant 0$对于所有$x \in I$是必要且充分的；为了使$f$在$I$上严格凸，满足前面的条件是必要且充分的，并且进一步满足点$x \in I$的集合，其中$f''(x) > 0$在$I$中稠密。*

这紧接着前面的命题，以及I、p. 14的推论。

#### 例 {#fvr-i-s4-n4-exa-1 .statement tag=0867}

在区间 ]$0, +\infty$ [ 函数 $x^r$ ($r$ 任意实数) 上，二阶导数等于 $r(r-1)x^{-2}$；因此，如果$r > 1$或$r < 0$，它是严格凸的，如果$0 < r < 1$，它是严格凹的。 \*

In order to be able to formulate another criterion for convexity we make the following definition: given the graph $G$ of a finite real function defined on an interval $I \subset \mathbf{R}$ and an interior point $a$ of $I$, we shall say that a line $D$ passing through $M_a = (a, f(a))$ is *locally above* (resp. *locally below*) $G$ if there exists a neighbourhood $V \subset I$ of $a$ such that every point of $D$ contained in $V \times \mathbf{R}$ is above (resp. below) $G$; we shall say that $D$ is *locally on* $G$ at the point $M_a$ if there is a neighbourhood $V \subset I$ of $a$ such that the intersection of $D$ and $V \times \mathbf{R}$ is identical to that of $G$ and $V \times \mathbf{R}$ (in other words, if $D$ is simultaneously locally above and locally below $G$).

#### 命题 9 {#fvr-i-s4-prop-9 .statement tag=0868}

*设$f$为实有限函数，它是开区间$I \subset \mathbf{R}$上的上半连续。 为了使$f$在$I$上凸出，对于$f$的图$G$的每个点$M_x$来说，$G$上的每条线局部在点上都应该局部在$G$上（在点处）是必要且充分的$M_x$).*

条件是*必要的*：事实上，如果$f$在$I$上凸，那么在$f$的图$G$的每个点$M_a$，存在一条*支撑线*$\Delta$到$G$：现在$\Delta$在下面$G$，因而*更不必说*局部低于$G$（I，p. 29）；如果线$D$在点$M_a$处局部位于$G$上方，则它局部在$\Delta$上方，因此重合必须与$\Delta$一起，因此局部在$G$处点$M_a$。

条件*足够*。事实上，假设它是满足的，并且假设$f$在$I$上不是凸的；那么 $I$ ($a < b$) 中有两个点 $a, b$，因而 $G$ 的点 $M_x$ 严格位于线段 $M_aM_b$ 之上（图 4）。在其他字中，函数$g(x) = f(x) - f(a) - \frac{f(b) - f(a)}{b - a}(x - a)$在$[a, b]$上占用值$> 0$；由于 $g$ 是有限且上半连续的，因而 $[a, b]$ 上的最小上界 $k$ 是有限且 $> 0$，且集合 $g^{-1}(k)$ 是闭且非空的 (\emph{Gen. Top.}, IV, p. 361，第 3 条和第 1 条）。设$c$为$g^{-1}(k)$的下确界；我们有$a < c < b$。并且在点 $M_c$ 处，具有方程 $y = f(c) + \frac{f(b) - f(a)}{b - a}(x - c)$ 的线 D 局部位于 G 上方；但不能在这个点处位于G上，因为对于$a < x < c$，有$g(x) < k$，这意味着$M_x$严格低于D。这导致了一个矛盾，从而建立了命题。

#### 推论 1 {#fvr-i-s4-prop-9-cor-1 .statement tag=0869}

*对于实数有限函数* $f$ *定义在开区间* $I \subset \mathbf{R}$ *上半连续在* $I$ *凸在* $I$ *对于所有* $x \in I$ *应该存在一个* $\varepsilon > 0$ *使得关系* $|h| \leq \varepsilon$ *需要*

$$
f(x) \leq \frac{1}{2} \left( f(x + h) + f(x - h) \right).
$$

我们只需证明条件 *足够*。事实上，如果在$f$的图G的点$M_a$处，线D局部位于G之上，那么它在这个点处局部位于G上；因为，在相反的情况下，对于例，点$M_{a+h}$将严格低于D，而点$M_{a-h}$将低于D：因此，线段$M_{a-h}M_{a+h}$的中点将严格高于D（图5），并且，由于假设，$M_a$将*更不必说* 严格低于 D，这是荒谬的。

![显示凸函数与点 M_{a-h}、M_a、M_{a+h} 和标记为 D 的切线的图。](https://i.imgur.com/3Q5z5QG.png)

图5

#### 推论 2 {#fvr-i-s4-prop-9-cor-2 .statement tag=086A}

*令 $f$ 为在开区间 $I \subset \mathbf{R}$ 上定义的有限实数函数。如果对于每个点 $x \in I$ 都有一个开区间 $J_x \subset I$ 包含 $x$ 并且使得 $f$ 到 $J_x$ 的限制在 $J_x$ 上凸，那么 $f$ 在$I$.*

显然$f$满足prop的标准。 9.

### 习题 {#fvr-i-s4-exercises}

§ 4](exercises/s4/)参见[习题。
