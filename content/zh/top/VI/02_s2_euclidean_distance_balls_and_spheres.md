---
book: top
book_title: General Topology
chapter: VI
chapter_title: Real number spaces and projective spaces
section: 2
section_title: Euclidean distance, balls and spheres
lang: zh
source: top-v-x
pdf_pages: 0044-0050, 0064-0067
extraction: ocr
subsections:
    - "no": 1
      title: EUCLIDEAN DISTANCE IN $\mathbf{R}^n$
      page: 0
      pdf_page: 44
    - "no": 2
      title: DISPLACEMENTS
      page: 0
      pdf_page: 45
    - "no": 3
      title: EUCLIDEAN BALLS AND SPHERES
      page: 0
      pdf_page: 46
    - "no": 4
      title: STEREOPHIC PROJECTION
      page: 0
      pdf_page: 48
statements: 12
exercises: 13
content_sha256: 8231bc9229a93b2d5c461d31065179c7472a2a66efa0623ee871c4ce19a5ef62
translated_from: content/en/top/VI/02_s2_euclidean_distance_balls_and_spheres.md
translation_method: google
source_content_sha256: a782e1c3f639976183f49d786a4ce82493366e142659214046bd4d37a7e18f82
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 9a2b75e11e98e795f29251a57f50ce6dbc699b8d0f7af6083726a992daceec39
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 2. 欧氏距离；球和球体

### 1. 欧氏距离$\mathbf{R}^n$

根据一般的定义，两个点$x = (x_i)$和$y = (y_i)$之间的*欧氏距离*为数

$$
d(x, y) = \sqrt{\sum_{i=1}^n (x_i - y_i)^2} \geq 0.
$$

我们回顾一下它的主要特性。 关系 $d(x, y) = 0$ 相当于$x = y$。我们有$d(x, y) = d(y, x)$；对于所有标量 $t \in \mathbf{R}$、$d(tx, ty) = |t| d(x, y)$；对于所有$z \in \mathbf{R}^n$、$d(x + z, y + z) = d(x, y)$；在其他字中，两个点之间的距离*在平移下不变*。从原点 $o$ 到点 $x$ 的距离 $d(o, x)$ 也用 $\|x\|$ 表示，称为 $x$ 的 *欧氏范数*（或简称为 $x$ 的 *范数*，当不可能发生混淆；cf.章IX, § 3, no. 3）。然后$d(x, y) = \|y - x\|$。

对于 $n = 1$，$\mathbf{R}$ 约化的点 $x, y$ 到区间的长度 $|y - x|$ 之间的距离为欧氏，以 $x$ 和 $y$ 作为端点。对于任何$n$，我们说$d(x, y) = \|y - x\|$是以$x$和$y$为端点的段的*长度*。

欧氏距离满足*三角形不等式*

(I)
$$
d(x, y) \leq d(x, z) + d(z, y)
$$
对于$\mathbf{R}^n$中的所有$x, y, z$。

我们记得（I）约化的证明到不等式的证明

$$
\left( \sum_{i=1}^n (x_i + y_i)^2 \right)^{1/2} \leq \left( \sum_{i=1}^n x_i^2 \right)^{1/2} + \left( \sum_{i=1}^n y_i^2 \right)^{1/2};
$$

这又相当于 Cauchy-Schwarz 不等式

$$
\left( \sum_{i=1}^n x_i y_i \right)^2 \leq \left( \sum_{i=1}^n x_i^2 \right) \left( \sum_{i=1}^n y_i^2 \right),
$$

这是拉格朗日恒等式的直接的推论

$$
\left( \sum_{i=1}^n x_i^2 \right) \left( \sum_{i=1}^n y_i^2 \right) - \left( \sum_{i=1}^n x_i y_i \right)^2 = \frac{1}{2} \sum_{i,j} (x_i y_j - x_j y_i)^2.
$$

这个证明同时表明，只有当$z$是以$x$和$y$为端点的线段的点时，(1)的两侧才可以相等。

从（1）我们推导出不等式

$$
d(x, y) \geq |d(x, z) - d(y, z)|.
$$

最后，如果$x = (x_i), y = (y_i)$，我们有

$$
\sup_{1 \leq i \leq n} |x_i - y_i| \leq d(x, y) \leq \sqrt{n} \cdot \sup_{1 \leq i \leq n} |x_i - y_i|.
$$

因此，$\mathbf{R}^n$的子集$A$是*有界*（§ 1, no. 1）当且仅当

$$
\sup_{x \in A} \|x\| < +\infty.
$$

### 2. 位移

我们再次回忆一下，$\mathbf{R}^n$对其自身进行仿射变换$f$，这使得任意两个点之间的距离保持*不变*[也就是说，对于所有$x, y$来说，$d(f(x), f(y)) = d(x, y)$]被称为*欧氏位移*（或简称为*位移*）（*）；它们形式群，称为$\mathbf{R}^n$的*群位移*。这个群在$\mathbf{R}^n$上传递操作；更一般地，如果$V$和$V'$是相同维数在$\mathbf{R}^n$中的任意两个仿射线性簇，则存在变换$V$到$V'$的位移。保持原点固定的位移，称为*正交变换*，所有位移的群中的形式子群。这个子群称为$n$实变量的*正交群*； 线性映射其中属于到此群的特征在于，它们使每个点 $x \in \mathbf{R}^n$ 的 *范数* $\|x\|$ 保持不变，或者等效地，*二次*

(*) 如果对于所有 $x, y$，$f$ 仅受条件 $d(f(x), f(y)) = d(x, y)$ 影响，则实际上 $f$ 必须是仿射且线性的，因此是位移。

形式$\|x\|^2 = \sum_{i=1}^n x_i^2$。 $\mathbf{R}^n$的两个向量$x = (x_i)$和$y = (y_i)$的标量乘积是与二次形式$\sum_{i=1}^n x_i^2$相关的双线性形式的值$\sum_{i=1}^n x_i y_i$；它用 $(x|y)$ 表示，或者如果不存在混淆的可能性，则简单地用 $xy$ 表示。每个正交变换都会使任意两个向量的标量乘积保持不变。如果 $(x|y) = 0$，则两个向量 $x, y$ 被称为正交；如果每个 $x \in V$ 都与每个 $y \in V'$ 正交，则 $\mathbf{R}^n$ 中的两个向量子空间 $V, V'$ 被称为正交；如果分别与 $P$ 和 $P'$ 平行的向量子空间是正交的，则两个仿射线性簇 $P, P'$ 被称为正交。

### 3. 欧氏球体和球体

对于每个整数$p > 0$，令$U_p$表示$\mathbf{R}^n$的点的所有对$(x, y)$中的集合，使得$d(x, y) < 1/p$；不等式(3)表明集合$U_p$形式是$\mathbf{R}^n$均匀性的基本系统(cf.章IX, § 2)。

从这个事实和不等式
$$
|d(x, y) - d(x', y')| \leq d(x, x') + d(y, y'),
$$
即(1)的推论，我们推断$d(x, y)$在$\mathbf{R}^n \times \mathbf{R}^n$上一致连续；因此范数$\|x\| = d(0, x)$在$\mathbf{R}^n$上一致连续。

#### 定义 1 {#top-vi-s2-def-1 .statement tag=0BWR}

给定点 $x_0 \in \mathbf{R}^n$ 和实数 $r > 0$，$n$ 维数的开（或闭）欧氏球，其中心 $x_0$ 和半径 $r$ 为集合所有点$x \in \mathbf{R}^n$使得$d(x_0, x) < r$[分别。 $d(x_0, x) \leq r$]； $n - 1$ 维数的欧氏球体，其中中心 $x_0$，半径为 $r$，是所有 $x \in \mathbf{R}^n$ 的集合，使得 $d(x_0, x) = r$。

在不存在混淆风险的情况下，我们简单地用“ball”（分别为“sphere”）来表示“欧氏 ball”（分别为“欧氏 sphere”）。当$n = 2$时，两个维数的球称为圆盘，一个维数的球体称为圆。当 $n = 1$ 时，具有中心 $x_0$ 和半径 $r$ 的开（或闭）球为区间 $]x_0 - r, x_0 + r[$（或 $[x_0 - r, x_0 + r]$）； 中心 $x_0$、半径为$r$的球体是这些区间的两个端点$x_0 - r, x_0 + r$的集合由……组成。

根据上述内容，具有中心 $x_0$ 的球（开式或闭式）（或者只是半径为 $1/p$ 的球，其中 $p$ 穿过整数 $> 0$ 的集合）形式是基本系统邻域点 $x_0$。

#### 命题 1 {#top-vi-s2-prop-1 .statement tag=0BWS}

$\mathbf{R}^n$ 的每个开（或闭）球都是开（或紧）集合。开球的闭合是具有相同中心和相同半径的闭球；闭球的内部是具有相同中心和相同半径的开球。

中心 $x_0$ 和半径 $r$ 的开（或闭）球在连续函数 $d(x_0, x)$ 下为逆像或区间]$-\infty, r[$（或]$-\infty, r]$）；因此它是开放的（分别是封闭的和有界的，因此是紧凑的）。如果$d(x_0, x) = r$，并且如果$y = x_0 + t(x - x_0)$ ($0 < t < 1$)是端点为$x_0$和$x$的开路段的点，我们有$d(x_0, y) = tr < r$，并且$d(x, y) = (1 - t)r$尽可能小；因此 $x$ 位于中心 $x_0$ 和半径 $r$ 的开球闭合处。同样，如果 $z = x + t(x - x_0)$ ($t > 0$) 是原点为 $x$、方向为向量 $x - x_0$ 的开射线的点，我们有
$$
d(x_0, z) = (1 + t)r > r,
$$
$d(x, z) = tr$ 尽可能小；因此 $x$ 不是具有中心 $x_0$ 和半径 $r$ 的封闭球的内部点。

#### 推出 {#top-vi-s2-n3-cor-1 .statement tag=0BWT}

每个欧氏球体的紧集是具有相同中心和相同半径的开球和闭球的边界。

将映射 $x \to \frac{1}{r}(x - x_0)$ 变换中心 $x_0$ 和半径 $r$ 的球体（分别为开球、闭球）放入中心 $o$ 和半径 $1$ 的球体（分别为开球、闭球）；这个球体用$S_{n-1}$表示，在$\mathbf{R}^n$中称为单位球体。同样，半径为$1$、中心$o$的闭球记为$B_n$，在$\mathbf{R}^n$中称为单位球。因此，$(n - 1)$ 维数球体（分别为 $n$ 维数的闭球）的拓扑研究被简化为 $S_{n-1}$（分别为 $B_n$）的拓扑研究。对于开球，我们有以下命题：

#### 命题 2 {#top-vi-s2-prop-2 .statement tag=0BWU}

每个$n$维开球都同胚于$\mathbf{R}^n$。

对于映射$x \to \frac{x}{1 + ||x||}$，在$\mathbf{R}^n$和映射$\mathbf{R}^n$上连续到中心$o$和半径$1$的开球上；此外，从$y = \frac{x}{1 + ||x||}$我们推导出$x = \frac{y}{1 - ||y||}$，因此映射是双射且双连续的。

让$\mathbf{R}_n^*$表示$\mathbf{R}^n$中$o$的补集。

#### 命题 3 {#top-vi-s2-prop-3 .statement tag=0BWV}

空间$\mathbf{R}_n^*$同胚于$S_{n-1}$的乘积和实数$> 0$的空间$\mathbf{R}_+^*$。

对于每个点$x \neq o$都可以唯一地写成形式$tz$，其中$t > 0$和$||z|| = 1$，因为$x = tz$意味着$t = ||x||$和$z = x/||x||$。由于$tz$在乘积$\mathbf{R} \times \mathbf{R}^n$上连续，因此*更不必说*在$\mathbf{R}_+^* \times S_{n-1}$上连续，并且由于$||x||$和$\frac{1}{||x||}$在$\mathbf{R}_n^*$上连续，因此证明了命题。

映射 $x \to x/||x||$ 被称为$\mathbf{R}_n^*$ 到$S_{n-1}$ 的*中心投影*。一个定义以同样的方式将点$a$的补集的*中心投影*放到具有中心$a$的球面上。

#### 推论 1 {#top-vi-s2-prop-3-cor-1 .statement tag=0BWW}

*球体* $S_{n-1}$ *与* $\mathbf{R}_n^*$ *的商同胚于等价关系，其类是原点* $o$的开光线。

这些类也可以被定义为比$> 0$的同位性群除了$\{ o \}$之外的不及物性**类。

#### 推论 2 {#top-vi-s2-prop-3-cor-2 .statement tag=0BWX}

*空间* $\mathbf{R}_n^*$ *同构于* $\mathbf{R} \times S_{n-1}$。

因为 $\mathbf{R}_+^* = ]0, +\infty[$ 同胚于 $\mathbf{R}$ (章 IV, § 4, no. 1, 命题 1)。

#### 注 {#top-vi-s2-n3-rem-1 .statement tag=0BWY}

这些命题并不是欧氏球所特有的，而是可以扩展到$\mathbf{R}^n$中$o$的紧凑邻域的整个类别（参见习题12）。

集合 $S_{n-1}$ 和 $B_n$ 在所有正交变换下显然是不变的。如果$V$是$\mathbf{R}^n$中的$p$维向量子空间，则存在变换$V$到$p$维坐标系的正交变换；因此$V \cap S_{n-1}$（分别$V \cap B_n$）与$S_{p-1}$（分别$B_p$）同胚。

### 4. 立体投影

考虑 $S_{n-1}$ 的点 $e_n = (0, \ldots, 0, 1)$，以及超平面 $H$ 和方程 $x_n = 0$，与向量 $e_n$ 正交。对于$S_{n-1}$中的每个点$x = (x_i)$，除了$e_n$之外，让我们制作对应点$y$，其中通过$e_n$和$x$的线与超平面$H$相交（图3）。很容易验证我们有

$$
y = \frac{1}{1 - x_n} (x - x_n e_n)
$$

和

$$
x = \frac{||y||^2 - 1}{||y||^2 + 1} e_n + \frac{2}{||y||^2 + 1} y.
$$

![图表显示立体图投影](https://i.imgur.com/3Q5z5QG.png)

图 3.

如果我们用$A$表示$S_{n-1}$中$\{ e_n \}$的补集，那么这些公式表明我们已经定义了$A$到超平面$H$的同胚。这种同胚被称为$A$到$H$的立体投影投影，或者（滥用语言）$S_{n-1}$到$H$的立体投影投影； $e_n$是投影的顶点，$H$超平面是投影的顶点。更一般地，如果$H'$是超平面经过到$o$（$B_n$的直径超平面），并且如果$a$是$S_{n-1}$的交的点之一，并且直线通过$o$与$H'$经过正交，我们可以以同样的方式将定义顶点为$a$的立体投影放到投影$H'$的超平面上；在任何情况下，这个投影都可以通过正交变换返回到前一个变换$H'$到$H$和$a$到$e_n$。

#### 命题 4 {#top-vi-s2-prop-4 .statement tag=0BWZ}

*如果 $n > 1$、欧氏球体 $S_{n-1}$ 同胚于空间 $\mathbf{R}^{n-1}$，通过邻接“无穷远处的点”而变得紧致*（章 I, § 9, no. 8、定理 4）。

对于立体投影定义，$S_{n-1}$中点的补集到$\mathbf{R}^n$的超平面的同胚，它与$\mathbf{R}^{n-1}$同胚。

#### 推论 1 {#top-vi-s2-prop-4-cor-1 .statement tag=0BX0}

*球体$S_n$与通过识别球体$S_{n-1}$的所有点获得的球$B_n$的商空间同胚。

球$B_n$是常规空间（章I, § 8, no. 4）；因此，通过识别$S_{n-1}$的所有点得到的$B_n$的商空间$F$是*Hausdorff*（章I, § 8, no. 6，命题15）。由于 $B_n$ 是紧致的，$F$ 也是紧致的，并且 $F$ 因此同胚于 $n$ 维数的开球，通过在无穷远处邻接点使其紧致，由 Alexandroff 的定理 (章) I, § 9, no. 8、定理 4)。因此，结果由命题 2 和 4 得出。

#### 推论 2 {#top-vi-s2-prop-4-cor-2 .statement tag=0BX1}

*圆$S_1$同胚于环面$T$*。

在章VIII, § 2, no. 1，我们将再次获得这个结果，作为更精确的定理的推论。

#### 命题 5 {#top-vi-s2-prop-5 .statement tag=0BX2}

*如果$n > 1$、欧氏球体$S_{n-1}$是连通且局部连通的，并且它的每个点都有一个与$\mathbf{R}^{n-1}$同胚的开邻域。*

$S_{n-1}$ 中点的补集是连通稠密集合，因此 (章 I, § 11, no. 1, 命题 1) $S_{n-1}$ 是连通的。要看到每个点都有与$\mathbf{R}^{n-1}$同胚的邻域，我们只需从给定点以外的顶点进行立体投影。

从这个命题和no. 3的命题3可以得出，$\mathbf{R}_n^*$是两个相连的空间的乘积，是相连的（章I, § 11, no. 4，命题8； cf.§ 1、习题10)。

$S_{n-1}$的交和由$B_n$的直径超平面确定的闭（或开）半空间称为$S_{n-1}$的*闭*（或*开*）*半球*。通过将投影立体投影到超平面上，没有包含投影顶点的闭合（或开放）半球被映射到 $n - 1$ 维数的*闭合*（或*开放*）球上，因此它与该球是*同胚*的。

如果$n = 2$，我们说“半圆”而不是“半球”。

### 习题{#top-vi-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
