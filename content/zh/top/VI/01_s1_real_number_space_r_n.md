---
book: top
book_title: General Topology
chapter: VI
chapter_title: Real number spaces and projective spaces
section: 1
section_title: Real number space R^n
lang: zh
source: top-v-x
pdf_pages: 0037-0044, 0061-0064
extraction: ocr
subsections:
    - "no": 1
      title: THE TOPOLOGY OF $\mathbf{R}^n$
      page: 0
      pdf_page: 37
    - "no": 2
      title: THE ADDITIVE GROUP $\mathbf{R}^n$
      page: 0
      pdf_page: 38
    - "no": 3
      title: THE VECTOR SPACE $\mathbf{R}^n$
      page: 0
      pdf_page: 39
    - "no": 4
      title: AFFINE LINEAR VARIETIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 40
    - "no": 5
      title: TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $\mathbf{R}$
      page: 0
      pdf_page: 42
    - "no": 6
      title: TOPOLOGY OF MATRIX SPACES OVER $\mathbf{R}$
      page: 0
      pdf_page: 43
statements: 11
exercises: 13
content_sha256: a4bda3f1310d1eb14f714cc535c2951c34ab39c29180a5609e2cf04fe9312c02
translated_from: content/en/top/VI/01_s1_real_number_space_r_n.md
translation_method: google
source_content_sha256: 32d87d11d82f3f26afa123ebedc5e4a3d3bf1c06362cc553b78907c825a45e4c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 66706333968c414c1902c48e7e8b8157808dd23b14f105183a90ccd64e35a8ad
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 1. REAL NUMBER SPACE $\mathbf{R}^n$

### 1. $\mathbf{R}^n$ 的拓扑

#### 定义 1 {#top-vi-s1-def-1 .statement tag=0BW3}

*n 空间的拓扑乘积与实直线相同，称为n 维数的实数空间，记为$\mathbf{R}^n$。*

#### 注 {#top-vi-s1-n1-rem-1 .statement tag=0BW4}

空间 $\mathbf{R}^0$ 由单个点组成。

从*集合理论*、章III, § 6, no. 3、定理2、推论I，我们知道，如果E为无限集合，则$E^n$对于所有整数$n > 0$与E等价；因此，如果$n > 0$、$\mathbf{R}^n$与$\mathbf{R}$等价，即$\mathbf{R}^n$*具有连续统*的幂（cf.习题1和2）。

#### 定义 2 {#top-vi-s1-def-2 .statement tag=0BW5}

*$\mathbf{R}^n$的任何子集是$\mathbf{R}$的n个开（或闭）区间的乘积，称为$\mathbf{R}^n$中的开（或闭）盒子。 [对于 $n = 2$，它被称为开放（或闭合）矩形。]*

The open boxes in $\mathbf{R}^n$ form a *base* of the topology of $\mathbf{R}^n$ (Chapter I, § 4, no. 1); the open boxes which contain a point $x = (x_i)_{1 \leq i \leq n}$ of $\mathbf{R}^n$ form a fundamental system of neighbourhoods of $x$, and so do the closed boxes of $\mathbf{R}^n$ for which $x$ is an interior point.

$\mathbf{R}^n$ 中的每个非空开箱都与 $\mathbf{R}^n$ *同构*（章 IV, § 4, no. 1，命题 1）。

由此可见，当$n \geq 1$时，$\mathbf{R}^n$中的每个非空开集合都有连续统的幂。

$\mathbf{R}^n$的*开*（或*闭*）*立方体*是一个开（或闭）盒子，它是$n$的乘积*相等长度*的有界间隔[对于$n = 2$，它被称为开（或闭）平方]；这些间隔的公共的长度称为立方体的边（或边长）。开放的立方体

$$
K_m = \prod_{1 \leq i \leq n} \left[ x_i - \frac{1}{m}, x_i + \frac{1}{m} \right]
$$

形式点 $x = (x_i)$ 邻域的可数基本系统，因为 $m$ 穿过所有整数 $> 0$ 的集合或穿过整数递增的任何序列到无穷大。

$\mathbf{R}^n$中的每个开（或闭）盒子都是相连的（章I, § 11, no. 4，命题8）；特别地，$\mathbf{R}^n$是连通的并且是局部连通的。

如果$A$是$\mathbf{R}^n$中的非空开集合，则其分量因此是开集合（章I, § 11, no. 6，命题11）；这些分量中的集合是可数的，因为$\mathbf{R}^n$具有可数稠密子集（对于例$\mathbf{Q}^n$）。

考虑在什么情况下$\mathbf{R}^n$的条件子集$A$会相对紧凑。 根据吉洪诺夫的定理（章I, § 9, no. 5，定理3），$A$的投影在$\mathbf{R}^n$的因子上相对紧凑是充分必要的；根据 Borel-Lebesgue 定理 (章 IV, § 2, no. 2, 定理 2)，这相当于说，这些投影以 $\mathbf{R}$ 的子集为界。 We say that a subset $A$ of $\mathbf{R}^n$ is bounded if all its projections are bounded subsets of $\mathbf{R}$; thus we have proved:

#### 命题 1 {#top-vi-s1-prop-1 .statement tag=0BW6}

$\mathbf{R}^n$ 的子集 $A$ 是相对紧的当且仅当它是有界的。

#### 推论{#top-vi-s1-n1-cor-1 .statement tag=0BW7}

空间 $\mathbf{R}^n$ 是局部紧致的，但如果 $n \geq 1$ 则不是紧致的。

### 2. 加法群$\mathbf{R}^n$

集合$\mathbf{R}^n$，赋予群结构即$\mathbf{R}^n$的$n$因子的加法群结构的乘积，为阿贝尔的群；我们使用$x = (x_i)$和$y = (y_i)$的添加剂记号、和，因此$x + y = (x_i + y_i)$。 数空间的拓扑与此群结构兼容；赋予这两个结构，$\mathbf{R}^n$是一个拓扑群，称为n维实数空间*的*加法群。 如果$n = 0$，我们约定$\mathbf{R}^0$仅表示单位元素中的群由……组成。

这个群的均匀度结构，称为$\mathbf{R}^n$的*加性均匀度*，是$\mathbf{R}^n$的因子均匀度的乘积（章III, § 3, no. 2）。如果，对于每个整数$p > 0$，$V_p$表示对$(x, y)$或$\mathbf{R}^n$的集合，使得$\max_{1 \leq i \leq n} |x_i - y_i| \leq 1/p$，集合$V_p$形式一个*基本* 系统这种一致性的随从。每当我们将 $\mathbf{R}^n$ 视为均匀性空间时，我们将始终牢记刚刚定义的加法均匀性，除非明确指出了相反的情况。有了这套制服结构，$\mathbf{R}^n$就是一套完整的制服空间（章II、、no. 5、命题10）

### 3. 向量空间$\mathbf{R}^n$

由于$\mathbf{R}$是域，我们可以在标量$t \in \mathbf{R}$的域$\mathbf{R}$、乘积$t x$上对$\mathbf{R}^n$向量空间结构进行定义并且点（或向量）$x = (x_i)$ / $\mathbf{R}^n$ 为点 $(t x_i)$。 注位似 $(t, x) \to t x$ 在 $\mathbf{R} \times \mathbf{R}^n$ 上连续。如果$e_i$表示$\mathbf{R}^n$中的向量，除了指标$i$的坐标等于1外，所有坐标均为零，则向量空间的$e_i$形式基 $\mathbf{R}^n$，称为这个空间的典范基。每个向量$x = (x_i) \in \mathbf{R}^n$都可以写成$x = \sum_{i=1}^n x_i e_i$，关系$\sum_{i=1}^n t_i e_i = 0$意味着$t_i = 0$对应$1 \leq i \leq n$。

因此，向量空间$\mathbf{R}^n$是维数$n$超过域$\mathbf{R}$，在代数（代数，章II, § 7, no. 2）的意义上；因此它的名称为$n$维实数空间。

令 $f$ 为向量空间 $\mathbf{R}^n$ 到向量空间 $\mathbf{R}^m$ 的仿射映射（$m$ 和 $n$ 整数 > 0）。如果我们把$g(x) = f(x) - f(0)$，$g$就是$\mathbf{R}^n$的线性映射放入$\mathbf{R}^m$。设$a_{ij}$($1 \leq j \leq m$)为$g(e_i)$在$\mathbf{R}^m$中的坐标，令$b_j$($1 \leq j \leq m$)为$f(0)$的坐标；如果 $x_i$ ($1 \leq i \leq n$) 是 $x \in \mathbf{R}^n$ 的第 $i$ 坐标，并且如果 $y_j$ 是 $y = f(x)$ 的第 $j$ 坐标，我们有

$$
y_j = \sum_{i=1}^n a_{ij} x_i + b_j \quad (1 \leq j \leq m).
$$

由于$x_1, x_2, \ldots, x_n$中的每个线性多项式在$\mathbf{R}^n$上一致连续，因此$\mathbf{R}^n$到$\mathbf{R}^m$的每个仿射映射在$\mathbf{R}^n$上一致连续（章II, § 2, no. 6，命题7）。

特别是，我们知道 $\mathbf{R}^n$ 对自身的每个仿射映射都是双射的，并且它的逆也是仿射映射；因此，$\mathbf{R}^n$对自身的每个仿射映射都是同胚（以及$\mathbf{R}^n$的一致结构的自同构）。

设$(a_i)_{1 \leq i \leq n}$为$\mathbf{R}^n$的$n$向量的自由系统[在向量空间$\mathbf{R}^n$的其他字基]；如果$b$是$\mathbf{R}^n$的任何点，点$x = b + \sum_{i=1}^{n} u_i a_i$的集合 P，使得$1 \leq i \leq n$的$-1 \leq u_i \leq 1$是$b$的紧凑邻域；因为存在 $\mathbf{R}^n$ 自身的双射仿射映射 $f$，使得 $f(b) = 0, f(b + a_i) = e_i$ 对于 $1 \leq i \leq n$； $f(P)$是$n$因子空间中$n$区间$[ -1, +1 ]$的立方乘积。 $P$ 与中心 $b$ 和基向量 $a_i$ 称为闭平行同位素。 $P$的内部由点$b + \sum_{i=1}^{n} u_i a_i$组成，使得$-1 < u_i < 1$代表$1 \leq i \leq n$；它被称为开放平行空间，具有中心$b$和基向量$a_i$。

### 4. $\mathbf{R}^n$ 中的仿射线性簇

给定$\mathbf{R}^n$中的$p$维仿射线性簇$V$，存在$\mathbf{R}^n$自身的仿射映射$f$，将变换$V$转换为$p$维坐标簇，即向量子空间$V'$由典范基$(e_i)$$\mathbf{R}^n$向量$p$生成。存在$V'$到$\mathbf{R}^p$的映射，即向量空间结构的同构和$V'$的拓扑到$\mathbf{R}^p$的相应的结构（而且通常很方便）到认同$\mathbf{R}^p$，具有这样的坐标变化$V'$，例如，具有由$e_1, e_2, \ldots, e_p$生成的向量子空间）。在加法中，$V'$是$\mathbf{R}^n$的闭子集（章I, § 4, no. 3，命题7的推论）；因此：

#### 命题 2 {#top-vi-s1-prop-2 .statement tag=0BW8}

*$\mathbf{R}^n$中的每个$p$维线性仿射簇都是$\mathbf{R}^n$的闭子集，与$\mathbf{R}^p$同胚。*

正是这个结果是在任意除法环上向量空间中的仿射线性变体 *one* 和 *two* 维数的名称 *line* 和 *plane* 的起源。我们还记得，对于$n \geq 1$，$\mathbf{R}^n$的$n - 1$维数的仿射线性簇称为*超平面*（*loc.cit.*）。

$n$ 一维坐标品种，即 $n$ 线经过到 $0$ 以及$n$ 点 $e_i$ 分别称为*坐标轴*。对于$n = 2$，通过$e_1$的轴是有时，称为*横坐标轴*，通过$e_2$的轴称为*纵坐标轴*； 点 $x \in \mathbf{R}^2$ 的第一个坐标称为其*横坐标*，第二个坐标称为其*纵坐标*。

每条线$D$经过到点$a$都有一个参数表示$t \to a + tb$，其中$t$贯穿$\mathbf{R}$和$b \neq 0$；这个映射是$\mathbf{R}$到$D$的同胚。 向量 $b$ 称为 D 的*方向* 向量，其分量 $b_i (1 \leq i \leq n)$ 称为 D 的方向比。如果 $b'$ 是 D 的另一个方向向量，则 $\mathbf{R}$ 中存在 $h \neq 0$，使得$b' = hb$。

点 $a + tb$的集合，其中$t$穿过实数$\geq 0$的集合，称为闭射线（或简称射线，或半线），原点为$a$，方向为向量 $b$（或方向比$b_i$）。它是 $\mathbf{R}^n$ 的闭子集，同胚于 $\mathbf{R}$ 的区间 $[0, +\infty[$，因此是连通的。直线D是原点为$a$、方向分别为向量、$b$、$-b$的两条射线的并；据说这些光线是相反的。

滥用语言，点$a + tb$的集合，其中$t$穿过实数$> 0$的集合，被称为原点$a$和方向向量$b$的开射线；它与区间]$0, +\infty[$同胚（因此与$\mathbf{R}$同胚），但如果$n > 1$则在$\mathbf{R}^n$不开，尽管它在包含的行中开。

通过两个不同的点 $x$ 和 $y$ 的线经过也有一个参数表示 $(u, v) \to ux + vy$，其中 $(u, v)$ 穿过实数的对的集合，使得$u + v = 1$。给定点 $ux + uy$ 的任意两个点 $x, y$（无论是否不同）集合，其中 $(u, v)$ 穿过实数的对的集合，使得 $u \geq 0, v \geq 0$ 和$u + v = 1$，称为端点为$x, y$的闭线段（或简称线段）。闭线段是紧致且连通的，因为如果其端点不同，则它同胚于区间 $[0, 1]$ 和 $\mathbf{R}$。

如果点$ux + vy$的$x \neq y$、集合使得$u > 0, v > 0$和$u + v = 1$被称为（滥用语言）端点为$x, y$的开段；它与开区间]$0, 1[$同胚（因此也与$\mathbf{R}$同胚）。最后$\{y\}$的并和端点为$x, y$的开线段为有时，称为在$x$开、在$y$闭的线段；它与区间$[0, 1[$同胚。所有以$x$和$y$为端点的段都是相连的，它们的闭包就是具有相同端点的闭线段。

#### 命题 3 {#top-vi-s1-prop-3 .statement tag=0BW9}

*令 $f(x) = f(x_1, x_2, \ldots, x_n)$ 为具有实数系数的多项式，与在 $\mathbf{R}^n$ 上定义的零不同。那么集合 $\overline{f}(0)$ 的补集在 $\mathbf{R}^n$ 中是稠密的。*

令$x$为$\mathbf{R}^n$中的任意点，并令$y \in \mathbf{R}^n$满足$f(y) \neq 0$； $\varphi(t) = f(x + t(y - x))$是实数变量$t$的多项式，与零不等；因此存在$t$的任意小值使得$\varphi(t) \neq 0$。这表明$x$位于$\overline{f}(0)$的补集的闭包中。

#### 推论{#top-vi-s1-n4-cor-1 .statement tag=0BWA}

*维数 $p < n$ 的仿射线性簇的补集在 $\mathbf{R}^n$ 中是稠密的。*

由于维数$p < n$的每一个仿射线性簇都包含在超平面中，因此足以证明超平面的推论；但超平面由方程 $g(x) = 0$ 定义，其中 $g$ 是与零不同的线性多项式。

#### 命题 4 {#top-vi-s1-prop-4 .statement tag=0BWB}

*在 $\mathbf{R}^n$ ($n \geq 1$) 中，每个超平面的补集都有两个连通分量。*

令$g(x) = 0$为$\mathbf{R}^n$中超平面$H$的方程，$g$为线性多项式。 集合$CH$是所有点$x$中的集合$E_1$中的并使得$g(x) > 0$和所有点$x$中的集合$E_2$使得$g(x) < 0$。 $E_1$和$E_2$是相连的，因为如果$g(x) > 0$和$g(y) > 0$，只要$u \geq 0, v \geq 0$和$u + v = 1$，我们就有$g(ux + vy) = ug(x) + vg(y) > 0$；在其他字中，端点为$x$和$y$的线段包含在$E_1$中。对于 $E_2$ 也是如此。另一方面，$CH$不连通，因为$g$下的$\mathbf{R}$中的像是区间]$0, +\infty$[和]$-\infty, 0$[的并。

超平面 $H$ 的补集的分量 $E_1, E_2$ 称为由 $H$ 确定的*开半空间*。

$E_1$和$E_2$的闭包分别为$E_1 \cup H$和$E_2 \cup H$，称为由$H$确定的*闭半空间*。

观察$\mathbf{R}^n$的仿射映射自身，其中变换$H$进入“坐标”超平面，例如，超平面，其方程为$x_n = 0$，还有变换由$H$确定的开半空间进入分别由关系、$x_n > 0$和$x_n < 0$定义的开放半空间；后者是开放的盒子，因此*同构*$\mathbf{R}^n$。

### 5. 拓扑向量空间和代数超过域 $\mathbf{R}$

设$E$为维数$n$除域$\mathbf{R}$之向量空间；如果$(a_i)_{1 \leq i \leq n}$是$E$的*基*，那么每个点$x \in E$都可以唯一地写成形式$x = \sum_{i=1}^n x_i a_i$，其中$x_i$是实数；因此，映射$(x_i) \to \sum_{i=1}^n x_i a_i$是$\mathbf{R}^n$到$E$的双射线性映射。

如果我们通过这个映射*迁移*到$\mathbf{R}^n$的$E$拓扑，则$E$被赋予与其加法群结构兼容的拓扑，以及映射$(t, x) \to tx$ $\mathbf{R} \times E$到$E$相对于此拓扑是连续的。这个拓扑*独立于$E$中选择的基*；因为如果$(a')$是$E$的另一个基，并且如果$x = \sum_{i=1}^n x'_i a'_i = \sum_{i=1}^n x_i a_i$，$\mathbf{R}^n$的映射$(x_i) \to (x'_i)$自身是线性的，因此是同胚。

这一事实使人们怀疑，在$E$上定义的拓扑应该能够在没有$E$的基帮助的情况下实现刻画。事实上，我们稍后会看到，这是$E$上*唯一的*Hausdorff 拓扑，其中函数$x - y$（在$E \times E$上）和$tx$（在$\mathbf{R} \times E$上）是连续的。

如果现在$A$是有限秩$n$超过域$\mathbf{R}$的*代数*，则$A$上的上述拓扑（被视为$\mathbf{R}$上的$n$维向量空间）不仅兼容$A$ 的加法群结构，还有它的 *环* 结构。这是以下更一般结果的推论：

#### 命题 5 {#top-vi-s1-prop-5 .statement tag=0BWC}

*令$E, F, G$是有限维向量空间除域$\mathbf{R}$的三倍。那么 $E \times F$ 到 $G$ 的每个双线性映射 (*) $f$ 都是连续的。*

我们可以假设$E = \mathbf{R}^m, F = \mathbf{R}^n, G = \mathbf{R}^p$；足以证明$f(x, y)$的$\mathbf{R}^p$中的坐标是$(x, y) \in E \times F$的连续函数（章I, § 4, no. 1，命题1）。在其他字中，足以证明每个*双线性形式*$g$在$E \times F$上连续；这是直接的，因为 $g(x, y)$ 是 $x$ 和 $y$ 坐标中的多项式。

### 6. 拓扑矩阵空间超过 $\mathbf{R}$

向量空间超过$\mathbf{R}$的重要例是*矩阵的空间$\mathbf{M}_{m,n}(\mathbf{R})$，有m行和n个列*，其元素属于到$\mathbf{R}$；这是维数$mn$超过$\mathbf{R}$的空间，因此与$\mathbf{R}^{mn}$同胚。 通过§ 5的命题5，两个矩阵$X \in \mathbf{M}_{m,n}(\mathbf{R}), Y \in \mathbf{M}_{n,p}(\mathbf{R})$的乘积$X.Y$是$(X, Y)$的连续函数。 In particular, the topology of the space $\mathbf{M}_n(\mathbf{R})$ of square matrices of order $n$ is compatible with the ring structure on $\mathbf{M}_n(\mathbf{R})$. 此外：

#### 命题 6 {#top-vi-s1-prop-6 .statement tag=0BWD}

*在环$\mathbf{M}_n(\mathbf{R})$中，非奇异矩阵的群$\mathbf{GL}_n(\mathbf{R})$是稠密开子集，在此集合上归纳出拓扑与其群结构兼容。*

(*) 如果$E, F, G$是域$K$上的三个向量空间，则$E \times F$到$G$的映射$f$被称为*双线性*，如果我们有相同的条件
$$
f(x + x', y) = f(x, y) + f(x', y), \quad f(x, y + y') = f(x, y) + f(x, y'),
$$
$$
f(\lambda x, y) = f(x, \lambda y) = \lambda f(x, y)
$$
对于所有 $x, x' \in E$、所有 $y, y' \in F$ 和所有 $\lambda \in K$。

如果$X$是非奇异平方矩阵，则$X^{-1}$的元素是$X$的元素函数；因此，这些函数在$X$的邻域中被定义和连续，因此这个邻域中的每个矩阵$Y$都是非奇异的，映射$Y \to Y^{-1}$在点$X$连续；因此，$\mathbf{GL}_n(\mathbf{R})$在$\mathbf{M}_n(\mathbf{R})$中开放，并且$\mathbf{GL}_n(\mathbf{R})$的拓扑与其群结构兼容。

最后，$\mathbf{GL}_n(\mathbf{R})$是方阵$X$的集合的补集，其行列式为零；由于$X$的行列式是$X$的元素中的多项式，no. 4的命题 3表明$\mathbf{GL}_n(\mathbf{R})$在$\mathbf{M}_n(\mathbf{R})$中是稠密的。

### 习题 {#top-vi-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
