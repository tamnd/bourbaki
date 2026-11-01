---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 6
section_title: Polish spaces, Souslin spaces, Borel sets
lang: zh
source: top-v-x
pdf_pages: 0201-0216, 0264-0273
extraction: ocr
subsections:
    - "no": 1
      title: POLISH SPACES
      page: 0
      pdf_page: 201
    - "no": 2
      title: SOUSLIN SPACES
      page: 0
      pdf_page: 203
    - "no": 3
      title: BOREL SETS
      page: 0
      pdf_page: 205
    - "no": 4
      title: ZERO-DIMENSIONAL SPACES AND LUSIN SPACES
      page: 0
      pdf_page: 206
    - "no": 5
      title: SIEVES
      page: 0
      pdf_page: 208
    - "no": 6
      title: SEPARATION OF SOUSLIN SETS
      page: 0
      pdf_page: 210
    - "no": 7
      title: LUSIN SPACES AND BOREL SETS
      page: 0
      pdf_page: 211
    - "no": 8
      title: BOREL SECTIONS
      page: 0
      pdf_page: 212
    - "no": 9
      title: CAPACITABILITY OF SOUSLIN SETS
      page: 0
      pdf_page: 214
statements: 48
exercises: 19
content_sha256: 52e2051e1e37d6d5dc9efdb3f9d9e963ba5308d89fae81216da392952ad877e8
translated_from: content/en/top/IX/06_s6_polish_spaces_souslin_spaces_borel_sets.md
translation_method: google
source_content_sha256: 29c13eb3d7cf0721a55e24e7530e1acd68312f601ca3f6f347a6bce38b4c8832
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: e661fa132b63cfeb277ef1335760527018e9c047e0a436291df86659be2f923e
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 6. 抛光空间、苏兰空间、波雷尔集合

### 1. 波兰语空间

#### 定义 1 {#top-ix-s6-def-1 .statement tag=0C88}

*拓扑空间* $X$ *如果它是可数的型* ($§ 2$, no. 8) *并且如果有一个度量，与* $X$的拓扑兼容，*就其而言* $X$ *是完整的*，则称其为波兰式。

#### 命题 1 {#top-ix-s6-prop-1 .statement tag=0C89}

a) *波兰语空间的每个闭合子空间都是波兰语*。
b) *波兰可数家族的乘积空间是波兰人*。
c) *波兰可数家族的和空间是波兰人*。

可数型的可度量空间的每个子空间都是可数型的可度量，并且完整的空间的每个闭子空间都是完整的； （章II, § 3, no. 4、命题8）。可数型可度量空间的每个可数乘积又可数型可度量：($§ 2$，no. 8)，并且完整度量空间的每个可数乘积是一个完整度量空间到与其拓扑兼容的度量（章 II, § 3, no. 5、命题 10 和章 IX, § 2, no. 4、定理 1，推论 2）。最后，令$(X_n)$为非空波兰语空间的序列，并考虑乘积空间$Y = \mathbf{N} \times \prod_n X_n$，其中$\mathbf{N}$携带离散拓扑；已经证明，$Y$是波兰语空间。另一方面，对于每个$n$，令$a_n$为$X_n$的点，并令$f_n$为$X_n$的映射到$Y$，这样对于每个$x \in X_n$，我们有

$$
f_n(x) = (n, (y_p)),
$$

其中 $y_p = a_p$ 如果 $p \neq n$ 和 $y_n = x$。如果$X$是$X_n$的拓扑和，很明显，$X$的映射$f$进入$Y$，与$X_n$上的$f_n$一致，因为每个$n$都是一个$X$同胚到$f(X)$；此外，对于每个 $n$，$f_n(X_n)$ 在 $Y$ 中闭合，并且族 $(f_n(X_n))$ 是局部有限的，因为 $\mathbf{N}$ 是离散的；因此 $f(X) = \bigcup_n f_n(X_n)$ 在 $Y$ 中闭合（章 I, § 1, no. 5，命题 4），因此 $f(X)$ 是波兰语空间，由 a) 得到。

#### 命题 2 {#top-ix-s6-prop-2 .statement tag=0C8A}

波兰语空间的每个空位子空间都是波兰语。

令$X$为波兰空间，令$d$为$X$与其拓扑兼容的度量，并令$U \neq X$为$X$的开子集。令 $V$ 为所有点 $(t, x)$ 中 $\mathbf{R} \times X$ 由……组成的子集，使得
$$
t \cdot d(x, X - U) = 1;
$$
$V$ 由 § 2, no. 2 的命题 3 闭合，因此是波兰语 (命题 1)。由于投影 $\mathrm{pr}_2 : \mathbf{R} \setminus X \to X$ 的限制到 $V$ 是 $V$ 到 $U$ 的同胚（$§ 2,$ no. 2，命题 3），$U$ 是波兰语子空间共 $X$。

#### 推论{#top-ix-s6-n1-cor-1 .statement tag=0C8B}

每个局部紧凑、可度量的空间 $X$ 都是波兰语。

设 $X$ 为将点无限邻接于 $X$ 所获得的紧空间； $X'$ 是可计量且可数的型（$§ 2,$ no. 9，命题 16 的推论），$X$ 就其独特的均匀性而言是完整的（章 II、$§ 4,$ no. 1， 定理1)。因此 $X$ 是波兰语空间；由于$X$在$X'$中开放，因此$X$是波兰语。

#### 命题 3 {#top-ix-s6-prop-3 .statement tag=0C8C}

令 $X$ 为 Hausdorff 拓扑空间。那么$X$波兰语子空间序列$(A_n)$交就是波兰语子空间。

设$f$为$X$到$X^\mathbf{N}$的对角线映射（[集合理论，章II，$§ 5,$no. 3；回想一下$f(x) = (x, x, \ldots)$，其中$x_n = x$对于所有$n \in \mathbf{N}$]。我们将使用以下引理：

#### 引理 1 {#top-ix-s6-lem-1 .statement tag=0C8D}

令$(A_n)$为豪斯多夫拓扑空间$X$的子集的序列。那么$X$的对角线映射$f : X \to X^\mathbf{N}$到子空间$\bigcap_n A_n$的限制是$\bigcap_n A_n$同胚到$\prod_n A_n$的闭子空间。

这个像是$\prod_n A_n$的交和对角线$\Delta = f(X)$，它在$X^\mathbf{N}$闭合，因为$X$是豪斯多夫（章I，$§ 8,$no. 1）； $f$ 是 $X$ 到 $\Delta$ 的同胚。

根据命题 3 的假设，$\prod_n A_n$ 是波兰语空间 (命题 1)，因此$\bigcap_n A_n$ 是引理 1 和命题 1 的波兰语。

#### 推论 {#top-ix-s6-n1-cor-2 .statement tag=0C8E}

非理性数的集合，由于实直线$\mathbf{R}$而被赋予了拓扑，是波兰语空间。

它是$\mathbf{R}$中可数开集合族的交，即单个有理数数的集合由……组成的补集。

#### 定理 1 {#top-ix-s6-thm-1 .statement tag=0C8F}

*子空间* $Y$ *波兰人空间* $X$ *是波兰人当且仅当* $Y$ *是* $X$中可数开集合族的交。

条件的充分性紧随命题 2和3。为了证明必要性，令$d$是与$Y$的拓扑兼容的度量，并且$Y$是完备的。设$\overline{Y}$为$X$中$Y$的闭包。对于每个整数 $n > 0$，令 $Y_n$ 为具有开放邻域 $U$ 的所有 $x \in \overline{Y}$ 的集合，使得 $U \cap Y$ 的直径（相对于公制 $d$）为 $\leq 1/n$。显然 $Y_n$ 在 $\overline{Y}$ 和包含 $Y$ 中开放。令 $x \in \bigcap_n Y_n$；则$x \in \overline{Y}$，$X$中$x$的邻域滤波器在$Y$上的迹是柯西滤波器（相对于$d$）；因此这个滤波器收敛到$Y$的点，从而收敛到$x \in Y$。因此$Y = \bigcap_n Y_n$。

对于每个$n$，令$H_n$为$X$的开子集，使得$H_n \cap \overline{Y} = Y_n$，并令$(U_m)$为$X$的开子集的序列，使得$\overline{Y} = \bigcap_m U_m$ （§ 2, no. 5，命题7）；那么$Y$是开集合$(H_n \cap U_m)$可数族的交。

#### 推论 1 {#top-ix-s6-thm-1-cor-1 .statement tag=0C8G}

*空间* $X$ *是波兰式当且仅当它同胚于立方体* $\mathbf{I}^{\mathbf{N}}$ 中开集合的可数交，*其中* $\mathbf{I}$ *是间隔* $[0, 1]$ *属于* $\mathbf{R}$。

条件显然是充分的，而且是必要的，因为可数型的每个可度量空间都同胚于$\mathbf{I}^{\mathbf{N}}$的子空间（§ 2, no. 8，命题12）。

#### 推论 2 {#top-ix-s6-thm-1-cor-2 .statement tag=0C8H}

*令* $X$ *和* $Y$ *为两个波兰语空间，并令* $f : X \to Y$ *为连续的映射。如果* $Z$ *是* $Y$ 的波兰语子空间，*则* $\overline{f}^{-1}(Z)$ *是* $X$ 的波兰语子空间。

对于$Z = \bigcap_n Z_n$，其中$Z_n$开放$Y$的子集；因此
$$
\overline{f}^{-1}(Z) = \bigcap_n \overline{f}^{-1}(Z_n),
$$
和集合$\overline{f}^{-1}(Z_n)$在$X$开放。

### 2. 苏林空间

#### 定义 2 {#top-ix-s6-def-2 .statement tag=0C8I}

*拓扑空间* $X$ *如果可度量并且存在波兰语空间* $P$ *和* $P$ *在* $X$上的连续映射，则称其为苏斯林空间。 *子集* $A$ *拓扑空间* $X$ *称为苏斯林集合如果子空间* $A$ *是苏斯林空间。*

显然，每个波兰语空间都是苏斯林，并且将 $X$ 的连续映射下的苏斯林空间 $X$ 的像转换为可度量的空间 $Y$ 是苏斯林空间。

#### 命题 4 {#top-ix-s6-prop-4 .statement tag=0C8J}

*每个 Souslin 空间 $X$ 都是可数的型。*

令$P$是波兰语空间，$f$是$P$到$X$的连续映射。那么$P$的可数稠密子集在$f$下的像就是$X$的可数稠密子集。

#### 命题 5 {#top-ix-s6-prop-5 .statement tag=0C8K}

*Souslin 空间 $X$ 的每个关闭（或打开）子空间都是 Souslin。*

因为如果$f$是波兰语空间$P$到$X$的连续映射，那么逆像在闭（或开）的$f$下，$X$的子集是闭（或开） 子集等于 $P$，因此是波兰语子空间等于 $P$（no. 1、命题 1 和 2）。

#### 命题 6 {#top-ix-s6-prop-6 .statement tag=0C8L}

*令$X$为Souslin空间，令$Y$为Hausdorff空间，令$f : X \to Y$为连续映射。那么$Y$的苏斯林子空间$A$在$f$下的逆像是$X$的苏斯林子空间。*

令$P, Q$为波兰语空间，令$g$为$P$在$X$上的连续映射，并令$h$为$Q$在$A$上的连续映射。令$R$为所有$(x, y) \in P \times Q$中的集合，使得$f(g(x)) = h(y)$； $R$ 在 $P \times Q$ 关闭，因此是 $P \times Q$ 的波兰子空间（no. 1、命题 1）。令$\varphi$为投影$pr_1$中的限制至$R$。那么$X$的子空间$\overline{f}^{-1}(A)$是连续映射$g \circ \varphi$下的$R$的像，因此是苏斯林空间。

#### 命题 7 {#top-ix-s6-prop-7 .statement tag=0C8M}

*苏斯林空间家族的乘积和和是苏斯林空间。*

对于每个整数$n$，让$X_n$是可度量的空间，$P_n$是波兰空间，$f_n$是$P_n$到$X_n$的连续映射。 空间 $P_n$ 的乘积（或和）是波兰语（no. 1、命题 1），而空间的像在映射下，即乘积 $f_n$（或映射，对于所有$n$，与$P_n$上的$f_n$一致）是空间$X_n$的乘积（或和）；后者是可度量的，因此是 Souslin 空间。

#### 命题 8 {#top-ix-s6-prop-8 .statement tag=0C8N}

*令$X$为可度量的空间，并令$(A_n)$为$X$的苏斯林子空间的序列。那么$A_n$的并和交就是Souslin 空间。*

这些子空间当然是可度量的。 $A_n$的和的规范映射到$X$的子空间$\bigcup_n A_n$的存在表明后者是苏斯林空间；并且$\bigcap_n A_n$凭借命题 5和7以及no. 1的引理 1而成为Souslin。

一般来说，即使在波兰语空间中，Souslin子空间的补语也不一定是Souslin（cf.习题6）；然而，参见no. 6、定理 2，推论。

#### 命题 9 {#top-ix-s6-prop-9 .statement tag=0C8O}

*令X为可度量的空间，并令A为X的相对紧凑的苏斯林子空间。那么存在 K 的空间 K、子集的紧凑可度量空间 K、递减序列 $(B_n)$，其中每一个都是紧集的可数并，以及连续的映射 $f : K \to X$，使得 $A = f\left(\bigcap_n B_n\right)$。*

替换 X by $\overline{A}$ 如果有必要，我们可以假设 X 是紧的，并且 A 在 X 中是稠密的。由于 A 是苏斯林空间，因此存在波兰语空间 P 和连续映射 $g : P \to X$，使得 $g(P) = A$。根据no. 1，定理 1，推论1，我们可以假设P是立方体$I^\mathbf{N}$的开子集的递减序列$(U_n)$的交。令 K 为空间 $I^\mathbf{N} \times X$，它是紧凑且可度量的（§ 2, no. 4，定理 1，推论 2）。令$G \subset P \times X$为g的图，令$\overline{G}$为K中G的闭包，令f表示$K = I^\mathbf{N} \times X$到X的投影；那么显然我们有$f(G) = A$。由于g是连续的，所以G在$P \times X$（章I, § 8, no. 1，命题2，推论2）和$G = \overline{G} \cap (P \times X)$中是闭的；因此$G = \bigcap_n B_n$，其中

$$
B_n = \overline{G} \cap (U_n \times X).
$$

由于每个$U_n$是$I^\mathbf{N}$（§ 2, no. 5，命题7）中闭集合的可数并，因此每个$B_n$是紧集和证明的可数并已完成。

### 3. 依波路集合

#### 定义 3 {#top-ix-s6-def-3 .statement tag=0C8P}

*令X为集合，令$\mathfrak{L}$为X的子集集合。如果满足以下条件，则称$\mathfrak{L}$是X上的$\sigma$代数：

a) *右 $\mathfrak{L}$ 属于到 $\mathfrak{L}$ 中每个集合的补集*。

b) *$\mathfrak{L}$属于到$\mathfrak{L}$的每个可数交/集合*。

如果$\mathfrak{L}$是X上的$\sigma$代数，$\mathfrak{L}$属于到$\mathfrak{L}$的集合的每个*可数并*（对于这个并的补集是交集合 $\mathfrak{L}$）。

X的所有子集中的集合$\mathfrak{B}(X)$显然是$\sigma$代数。 X上的$\sigma$代数的每个交都是X上的$\sigma$代数。对于 $\mathfrak{B}(X)$ 的任意子集，因此存在 *最小的* $\sigma$-代数包含 $\mathfrak{F}$；它被称为$\sigma$代数*由*$\mathfrak{F}$生成。

#### 定义 4 {#top-ix-s6-def-4 .statement tag=0C8Q}

在拓扑空间$X$中，$X$的所有闭子集的集合生成的$\sigma$代数的元素在$X$中称为Borel集合。

#### 命题 10 {#top-ix-s6-prop-10 .statement tag=0C8R}

令$f$是拓扑空间$X$到拓扑空间$Y$的连续映射。那么$Y$中的每个Borel集合在$f$下的逆像是$X$中的一个Borel集合。

令$\mathfrak{I}$为$Y$的所有子集$A$中的集合，使得$f^{-1}(A)$是$X$中的Borel集合。紧接着，$\mathfrak{I}$是$\sigma$代数，其中包含是$Y$的所有闭子集；因此 $\mathfrak{I}$ 包含于 $Y$ 中的所有 Borel 集合。

#### 命题 11 {#top-ix-s6-prop-11 .statement tag=0C8S}

在 Souslin 空间 $X$ 中，每个 Borel 集合都是 Souslin 集合。

令$\mathfrak{I}$为$X$的所有子集$A$中的集合，使得$A$和$\overline{A}$都是Souslin集合。通过 no. 2 的命题 8，$\mathfrak{I}$ 是$\sigma$ 代数。 $X$ 属于至 $\mathfrak{I}$ 的每个关闭子集 $F$，$F$ 和 $\overline{F}$ 均为 Souslin 集合（no. 2，命题 5）；因此$\mathfrak{I}$包含于$X$的所有Borel集合（cf.no. 6，定理2，推论）。

#### 推论{#top-ix-s6-n3-cor-1 .statement tag=0C8T}

令 $f$ 为苏斯林空间 $X$ 到可度量空间 $Y$ 的连续映射。如果$B$是$X$中的任何Borel集合，则$f(B)$是$Y$中的Souslin集合。

因为$B$是苏斯林空间，因此$f(B)$乘注跟随定义2（no. 2）也是如此。

#### 注 1 {#top-ix-s6-n3-rem-1 .statement tag=0C8U}

即使$X$和$Y$是波兰语空间，一般情况下，$X$中的Borel集合的像在$X$到$Y$的连续映射下也不是Borel 集合 in $Y$（cf. 习题 6；以及 no. 7、定理 3 推论）。

#### 注 2 {#top-ix-s6-n3-rem-2 .statement tag=0C8V}

令$X$为拓扑空间，并令$Y$为$X$的Borel子集。那么空间$Y$的Borel集合正好是$Y$中包含的$X$的Borel集合。对于 (i) $X$ 中的 Borel 集合包含在 $Y$ 形式 $Y$ 上的$\sigma$-代数，其中包含 $Y$ 中的闭集合，因此包含 $Y$ 的所有 Borel 集合； (ii) $X$的子集$A$使得$A \cap Y$是$Y$形式的Borel集合$X$上的$\sigma$代数，其中包含所有闭$X$ 的集合，因此包含 $X$ 的所有 Borel 集合。

### 4. 零维空间和卢辛空间

#### 定义 5 {#top-ix-s6-def-5 .statement tag=0C8W}

如果拓扑空间是 Hausdorff 并且每个点都有一个邻域的基本系统（既开又闭），则称它是零维的。

每个零维空间$X$都是完全不连通的；因为点$x$的分量包含在所有开闭的集合包含$x$中（章I，§II，no. 5），并且这些集合中的交是如果 $X$ 是零维，则只是 $\{ x \}$。

相反，局部紧致完全断开空间是零维的（章 II, § 4, no. 4，命题 6）；但存在完全断开的可度量空间，它们不是零维的[习题 3 b)]。

零维空间的每个子空间都是零维，零维空间的拓扑和和乘积也是零维。

#### 定义 6 {#top-ix-s6-def-6 .statement tag=0C8X}

拓扑空间 $X$ 是 Lusin 空间，如果它是可度量的并且存在零维波兰语空间 $P$ 和 $P$ 到 $X$ 的连续双射映射。

每个 Lusin 空间显然都是 Souslin 空间。

#### 命题 12 {#top-ix-s6-prop-12 .statement tag=0C8Y}

可度量的空间是Lusin空间当且仅当它是连续双射映射下的波兰语空间的像。

条件显然是必要的；让我们证明这也是足够的。如果 $f$ 是 Lusin 空间 $X$ 在可度量空间 $Y$ 上的连续双射，则从定义 6 可以得出 $Y$ 是 Lusin 空间。因此，我们只需要证明波兰人空间是卢辛空间。

首先注意，如果$X$是Lusin空间，$X$的每个闭（或开）子空间$A$都是Lusin空间（cf.no. 7，定理3）；因为如果$f$是零维波兰语空间$P$在$X$上的连续双射，则$f^{-1}(A)$在$P$中闭（或开），因此是$P$的零维波兰语子空间（no. 1， 命题 1 和 2)。

Lusin 空间的每个可数乘积都是 Lusin 空间；这是从 no. 1 的命题 1 以及零维空间的每个乘积都是零维这一事实得出的。 Hausdorff 拓扑空间的 Lusin 子空间的每个可数交都是 Lusin 子空间；这是从前面的注和引理1 of no. 1得出的。此外：

#### 引理 2 {#top-ix-s6-lem-2 .statement tag=0C8Z}

如果一个可度量的空间$X$使得存在由Lusin子空间组成的$X$的可数划分$(A_n)$，则$X$是一个Lusin空间。

对于每个$n$，令$P_n$为零维波兰空间，并令$f_n$为$P_n$到$A_n$的连续双射。如果$P$是$P_n$的拓扑和，则$P$是波兰语（no. 1，命题1）且零维，并且映射$f : P \to X$与$f_n$在$P_n$上一致$n$是$P$到$X$的连续双射；因此结果。

现在让我们证明$\mathbf{R}$的区间$I = [0, 1]$是Lusin空间。令$J$为所有无理数数中$I$由……组成的子空间；那么 $J$ 是波兰语（no. 1，命题 3 的推论）； J 也是零维的，因为如果 x 是 J 的任意点，形式 ]r, s[ 的 R 区间在 J 上的迹，其中 r 和 s 是有理数且 r < x < s，形式 J 中 x 的开和闭邻域的基数系统（因为 ]r 在 J 上的迹， s[ 和 [r, s] 相同）。因此 J 是 I 的 Lusin 子空间。现在 J 和 I 的子空间分别由单个有理数点形式和 I 的可数划分组成，因此 I 是引理 2 的 Lusin 空间。

设 P 为任意波兰语空间。根据推论 1 到定理 1 (no. 1)，P 同胚于立方体 IN 的子空间，它是 IN 中开集合的可数交。由于I是Lusin空间，证明开头的注表明P是Lusin空间，命题12的证明因此是完整的。

### 5. 筛子

#### 定义 7 {#top-ix-s6-def-7 .statement tag=0C90}

筛子是序列 C = (C_n, p_n)_{n \geq 0} 这样，对于每个 n，C_n 是可数集合，p_n 是 C_{n+1} 到 C_n 的满射。

对于整数 m, n 的每个对，使得 0 \leq m \leq n，如果 m = n，则令 p_{mn} 表示 C_m 的恒等映射到其自身上，如果 m < n，则将 C_n 的满射 p_m \circ p_{m+1} \circ \cdots \circ p_{n-1} 表示到 C_m 上。显然，每当 m \leq n \leq q 时，p_{mq} = p_{mn} \circ p_{nq}，因此我们可以考虑族 (C_n) 的逆极限 L(C) 相对于映射 (p_{mn}) 族（集合理论，章 III, § 7）。如果每个C_n被赋予离散的拓扑，则L(C)是拓扑空间(章I, § 4, no. 4)的逆极限；因此，L(C) 称为与筛C 相关的拓扑空间。 L(C)是拓扑乘积$\prod_n C_n$的闭子空间，紧接着L(C)是零维波兰语空间(no. 4)。

公制空间 X 的筛分由筛子 C = (C_n, p_n) 组成，对于 C_n 的每个整数 n \geq 0 映射 \varphi_n 到直径为 X 的非空封闭子集的集合中\leq 2^{-n}，这样：

a) 当 c 穿过 C_0 时，X 是集合 \varphi_0(c) 的并；
b) 对于每个 n 和每个 c \in C_n，\varphi_n(c) 是集合 \varphi_{n+1}(c') 的并，其中 c' 贯穿 p_n^{-1}(c)。

如果在加法中，对于每个 n，集合 \varphi_n(c)（当 c 穿过 C_n）互为不相交的，则称筛选是严格的。

#### 引理 3 {#top-ix-s6-lem-3 .statement tag=0C91}

可数型的每个度量空间X都具有筛选。如果 X 也是零维的，则 X 具有严格的筛选。

注首先，如果$Y$是可数型的公制空间，并且如果$\varepsilon$是实数$> 0$，则存在直径为$\leq \varepsilon$的集合可数覆盖$Y$ （$§ 2$、no. 8、命题13）。此外，如果$Y$是零维的，则存在由集合构成的覆盖$(V_n)$，它既是开闭的；如果$W_n$是$V_n$和$\bigcap_{k < n} (Y - V_k)$的交，我们看到$W_n$是封闭的，直径为$\leq \varepsilon$，成对的不相交的和覆盖$X$。在任何情况下，覆盖形式的非空集合的闭包是$Y$的可数覆盖，其元素是直径为$\leq \varepsilon$的非空闭闭集合。

令 $X$ 为可数型的度量空间。令$C_0$为由直径为$\leq 1$的非空闭集合构成的$X$可数覆盖的集合或指标，如果$X$是零维的话，它们是成对的不相交的； $\varphi_0$应为映射，与覆盖物的每个指标$c \in C_0$相应的集合相关联。假设我们已经定义了$C_i$和$\varphi_i$以及$i \leq n$的满射映射$p_i : C_{i+1} \to C_i$，使得这些指标满足条件b)。如果 $c \in C_n$、空间 $\varphi_n(c)$ 具有由直径为 $\leq 1/2^{n+1}$ 的非空闭合集合构成的可数覆盖，如果 $X$ [因此 $\varphi_n(c)$] 为零维，则它们互为不相交的；如果$I(c)$表示该覆盖层的指标集合，则我们将$c_{n+1}$视为集合$I(c)$的和，因为$c$穿过$C_n$；对于每个$c' \in C_{n+1}$，让$p_n(c')$表示元素$c \in C_n$，使得$c' \in I(c)$，并让$\varphi_{n+1}(c')$表示集合，并在考虑的$\varphi_n(c)$的覆盖中使用指标$c'$。显然，我们通过定义乘以归纳对$X$进行筛选，如果$X$是零维的，那么这个筛选是严格的；因此引理 3。

现在假设$X$是可数型的完整度量空间，并考虑通过筛子$C$和映射$\varphi_n$筛选$X$。如果$\gamma = (c_n)$是与$C$关联的空间$L(C)$的点，则序列$(\varphi_n(c_n))$是直径趋于0的$X$中封闭的集合的递减序列；因此，集合的序列中的交由单个点组成，我们用$f(\gamma)$表示。因此我们定义了映射$f : L(C) \to X$。如果$L(C)$的两个点$\gamma, \gamma'$对于$i \leq n$有相同的第$i$坐标，显然$f(\gamma)$和$f(\gamma')$之间的距离是$\leq 1/2^n$，因此$f$是连续的，因为定义拓扑$L(C)$。对于每个$x \in X$，从筛选的定义可以得出，我们可以在$n$序列$\gamma = (c_n)$上定义乘以归纳，这样每个$n \geq 0$和$c_n = p_n(c_{n+1})$都有$x \in \varphi_n(c_n)$；因此 $x = f(\gamma)$ 且 $f$ 是满射。此外，如果筛选严格，序列$\gamma = (c_n)$使得$x = f(\gamma)$是唯一的，因此在这种情况下$f$是双射的。据说$f$是由所考虑的筛选引起的映射。

#### 命题 13 {#top-ix-s6-prop-13 .statement tag=0C92}

*如果 $X$ 是任何 Lusin（或 Souslin）空间，则存在筛子 $C$ 和 $L(C)$ 到 $X$ 的连续双射（或满射）。*

参考 Lusin 空间（no. 4，定义 6）的定义 [resp。 a Souslin 空间 (no. 2, 定义 2)]，我们约化的情况

X 是波兰语和零维（或波兰语），然后前面的论证证明了结果。

### 6. 苏林的分离集合

#### 定理 2 {#top-ix-s6-thm-2 .statement tag=0C93}

令 X 为可度量的空间。如果我们给定X的互不相交的Souslin子空间的序列$(X_n)$，那么X中存在互不相交的Borel集合的序列$(B_n)$，这样每个 n $X_n \subset B_n$。

证明依赖于两个引理：

#### 引理 4 {#top-ix-s6-lem-4 .statement tag=0C94}

令$(A_n), (A'_m)$为拓扑空间X的子集中的两个序列。假设对于每个对$(A_n, A'_m)$，都有一个X的Borel集合$B_{nm}$，使得$B_{nm} \supset A_n$和$B_{nm} \cap A'_m = \emptyset$。然后存在X的Borel集合B，其包含$\bigcup_n A_n$且不满足$\bigcup_m A'_m$。

对于 Borel 集合 $B = \bigcup_n \left( \bigcap_m B_{nm} \right)$ 满足这些条件。

#### 引理 5 {#top-ix-s6-lem-5 .statement tag=0C95}

令X为Hausdorff空间，并令A、A'为X的两个不相交的Souslin子空间。然后存在 X 的 Borel 集合 B，使得 $B \supset A$ 和 $B \cap A' = \emptyset$。

通过no. 5的命题13，存在两个筛C，C'和L（C）的连续映射f到A，L（C'）的$f'$到A A'，由no. 5中描述的方法构造。对于每个$n \geq 0$和每个$c \in C_n$，让$q_n(c)$表示由所有序列$(c_k)_{k \geq 0}$组成的L（C）中的子空间，使得$c_n = c$； $q_n(c)$ 是 L(C) 的闭子空间。对于封闭的集合$q_n(c_n)$的每个$\gamma = (c_n) \in L(C)$序列是递减和形式一个过滤器基，其中$\gamma$为极限。此外，对于每个$c \in C_n$、集合$q_{n+1}(d)$，其中d在$q_n(c)$的$C_{n+1}$、形式划分中经过集合$p_n^{-1}(c)$。使筛子 $c'$ 与记号类似，定义。

我们将通过反证法论证并假设每个 Borel 集合其中包含 A 满足 A'。首先，从筛选的引理4和定义得出，存在$c_0 \in C_0$和$c'_0 \in C'_0$，使得每个Borel集合包含$f(q_0(c_0))$满足$f'(q'_0(c'_0))$。然后我们可以通过定义，乘以n上的归纳，

$$
\gamma = (c_n) \in L(C) \quad \text{and} \quad \gamma' = (c'_n) \in L(C')
$$

如下：假设已经为$i < n$定义了$c_i$和$c'_i$，这样对于每个指标$i < n$，每个Borel集合包含$f(q_i(c_i))$都满足$f'(q'_i(c'_i))$； 应用引理4和定义筛选到集合$f(q_{n-1}(c_{n-1}))$和$f'(q'_{n-1}(c'_{n-1}))$，我们看到存在$c_n \in C_n$和$c'_n \in C'_n$使得$p_{n-1}(c_n) = c_{n-1}$和$p_{n-1}(c'_n) = c'_{n-1}$并且使得每个Borel 集合包含$f(q_n(c_n))$满足$f'(q'_n(c'_n))$。现在序列$f(q_n(c_n))$收敛到点$a = f(\gamma) \in A$，序列$f'(q'_n(c'_n))$收敛到点$a' = f'(\gamma') \in A'$。由于 $A \cap A' = \emptyset$ 和 $X$ 是 Hausdorff，因此存在 $a$ 的闭邻域 $V$，它不存在包含 $a'$，因此对于 $n$ 足够大、$V$ 包含$f(q_n(c_n))$且不满足$f'(q'_n(c'_n))$。这是一个矛盾，因为 $V$ 是 Borel 集合。

为了证明定理 2，令$Y_n$表示集合$X_i$的并，使得$i \neq n$；那么 $Y_n$ 是 $X$ (no. 2, 命题 8) 的苏斯林子空间。对于每个指标 $n$，存在一个 Borel 集合 $B'_n$，其中包含 $X_n$ 且不满足 $Y_n$，通过引理 5。令 $B_n$ 为 $B'_n$ 的交且$\bigcap_{i < n} (X - B'_i)$。那么$B_n$是Borel集合，互为不相交的，并且对于每个$n$来说$B_n \supset X_n$。

#### 推论{#top-ix-s6-n6-cor-1 .statement tag=0C96}

*如果可度量空间的可数划分由Souslin 集合构成，那么这些集合就是Borel 集合。特别是，可度量空间中的每个 Souslin 集合（其补集是 Souslin 集合）都是 Borel 集合。*

### 7. 卢辛空间和波雷尔集合

#### 定理 3 {#top-ix-s6-thm-3 .statement tag=0C97}

*令$X$为Lusin空间。那么 $X$ 的子空间是 Lusin 空间当且仅当它是 Borel 集合。*

这个定理是以下两个引理中的推论：

#### 引理 6 {#top-ix-s6-lem-6 .statement tag=0C98}

*在 Lusin 空间 $X$ 中，每个 Borel 集合都是 $X$ 的 Lusin 子空间。*

令$\mathfrak{T}$为$X$的所有子集$A$中的集合，使得$A$和$\complement A$都是$X$的Lusin子空间。由于$X$中的每个闭集合和每个开集合都是$X$（no. 4）的Lusin子空间，$\mathfrak{T}$包含都闭$X$的子集，因此引理将如果我们能证明$\mathfrak{T}$是$X$上的$\sigma$代数，就可以证明。为此，只要证明如果$(A_n)$是$\mathfrak{T}$的集合的序列，那么$\bigcap_n A_n$和$\bigcup_n A_n$就是$X$的Lusin子空间。现在我们在no. 4中看到，Lusin子空间的每个可数交都是一个Lusin子空间。另一方面，如果$B_n$是$A_n$和$\bigcap_{i < n} \complement A_i$中的交，则从假设和前面的注可以得出，$B_n$是Lusin子空间；并且由于 $\bigcup_n A_n = \bigcup_n B_n$，子空间 $\bigcup_n A_n$ 是 no. 4 的引理 2 的 Lusin 子空间。

#### 引理 7 {#top-ix-s6-lem-7 .statement tag=0C99}

*可测量的空间 $X$ 的每个 Lusin 子空间 $A$ 都是 $X$ 中的 Borel 集合。*

通过no. 5的命题13，存在筛子C和L（C）的连续双射f到A上。对于no. 6的引理5的记号，对于每个整数n和每个c ε C_n，设 g_n(c) 表示 X 的子空间 f(q_n(c))；它是 Lusin 子空间，因此是 X 的 Souslin 子空间。当 c 穿过 C_n 时，集合 g_n(c) 是成对的不相交的，因为 f 是双射的；因此，通过 no. 6 的定理 2，X 中存在 Borel 集合的族 c → g'_n(c) (c ∈ C_n)，成对不相交的并且对于所有 c ∈ C_n 来说 g'_n(c) ⊃ g_n(c)。 替换 g'_n(c) 通过其交以及 X 中 g_n(c) 的闭包 g_n(c) 如有必要，我们可以假设 g'_n(c) ⊂ g_n(c)。令 c_{n-1}, c_{n-2}, ..., c_0 表示满射下 C_{n-1}, C_{n-2}, ..., C_0 中 c 的像

$$
p_{n-1,n} = p_{n-1},\ p_{n-2,n} = p_{n-2} \circ p_{n-1},\ ...,\ p_{0n} = p_0 \circ p_1 \circ ... \circ p_{n-1}
$$

分别;令 h_n(c) 表示集合的交

g'_n(c),\ g'_{n-1}(c_{n-1}),\ ...\ ,\ g'_0(c_0)。

由于 q_i(c_i) ⊃ q_n(c) 对于 0 ≤ i ≤ n − 1，h_n(c) 包含于 g_n(c)；还清楚的是，h_n(c) 是 Borel 集合并且包含在 g_n(c) 中，并且当 c 贯穿 C_n 时，h_n(c) 互为不相交的集合；最后，通过构造，对于每个 c' ∈ C_{n+1}，我们有 h_{n+1}(c') ⊂ h_n(p_n(c'))。当 c 穿过 C_n 时，令 B_n 为集合 h_n(c) 的并； B_n 是 Borel 集合，且 B_{n+1} ⊂ B_n；还有集合 g_n(c) 的 B_n 包含并 (c ∈ C_n)，即 A。设 B 为集合 B_n 的递减序列交； B 是 Borel 集合和包含 A。我们将证明 B = A，这将完成证明。

令x为B的点。那么，对于每个整数n，存在唯一的c ∈ C_n，使得x ∈ h_n(c)；让我们用 c_n(x) 来表示这个 c。 序列 (c_n(x))_{n≥0} 属于至 L(C)。 递减序列 (g_n(c_n(x))) 由定义收敛到点 a ∈ A；这些集合的闭包的序列也收敛于X中的a，因此更不必说也收敛于序列(h_n(c_n(x)))。现在 x 属于对所有集合 h_n(c_n(x))，因此 x = a ∈ A。由此证明了引理 7，并由此证明了定理 3。

#### 推论{#top-ix-s6-n7-cor-1 .statement tag=0C9A}

*如果 f 是 Lusin 空间（或者，特别是波兰语空间）X 到可度量空间 Y 的连续内射映射，则 f(X) 是 Y 中的 Borel 集合。*

### 8. 依波路截面

#### 定理 4 {#top-ix-s6-thm-4 .statement tag=0C9B}

*令X为波兰空间，令R为X上的等价关系，使得等价类 mod R在X中闭合，并且X中每个闭合集合的饱和度（相对于R）是Borel集合。然后，X 中存在一个 Borel 集合，它恰好满足一个点中的每个等价类。*

考虑 $X$ 上的一个度量与其拓扑兼容，并且 $X$ 是完整的。通过no. 5的引理3，存在$X$的筛分，由筛子$C = (C_n, p_n)$和映射$(\varphi_n)$的序列定义。对于每个$c \in C_n$，令$g_n(c)$为闭集合$\varphi_n(c)$相对于$R$的饱和度；通过假设，$g_n(c)$ 是 $X$ 中的 Borel 集合。

由于每个集合$C_n$都是可数的，我们可以线性地阶每个$C_n$，这样小于给定元素的元素的集合是有限的。对于每个$c \in C_n$，我们在$n$上按归纳计算定义集合$h_n(c)$，如下所示。首先，对于$c \in C_0$，$h_0(c)$是$\varphi_0(c)$和集合$X - g_0(c')$的交，其中$c' \in C_0$和$c' < c$。对于$c \in C_{n+1}$，$h_{n+1}(c)$ 是$\varphi_{n+1}(c), h_n(P_n(c))$ 的交，对于$c' \in C_{n+1}$、$p_n(c') = p_n(c)$ 和$c' < c$，集合 $X - g_{n+1}(c')$。 $h_n(c)$ 显然是 Borel 集合。

我们将证明以下断言：对于每个整数$n \geq 0$和每个等价类$H$ mod $R$，存在唯一元素$c \in C_n$使得$h_n(c)$满足$H$，并且我们有
$$
h(c_n) \cap H = \varphi_n(c) \cap H,
$$
因此这是一个*封闭*集合。对于$n = 0$，考虑最小的元素 $c \in C_0$，使得$\varphi_0(c)$满足$H$；那么$\varphi_0(c) \cap H$不满足任何集合$g_0(c')$，其中$c' \in C_0$和$c' < c$；因此它包含在$h_0(c) \cap H$中，因此等于这个集合；此外，我们有$H \subset g_0(c)$，因而$h_0(c') \cap H$对于$c' \in C_0$和$c' > c$来说是空的；因此断言被证明适用于$n = 0$。我们在$n$上继续归纳：如果存在$c \in C_{n+1}$使得$h_{n+1}(c)$满足$H$，那么从关系$h_{n+1}(c) \subset h_n(p_n(c))$和归纳假设得出$p_n(c)$是唯一元素 $d \in C_n$使得$h_n(d)$满足$H$。观察$\varphi_n(d)$中包含的$h_n(d)$包含在集合$\varphi_n(c)$的并中，其中$c \in p_n^{-1}(d)$经过定义筛选；因而，存在最小的元素$c \in p_n^{-1}(d)$使得$\varphi_{n+1}(c)$满足$H$。因此我们有
$$
\varphi_{n+1}(c) \cap H \subset \varphi_n(d) \cap H = h_n(d) \cap H
$$
由感应假设。因而
$$
\varphi_{n+1}(c) \cap H \subset \varphi_{n+1}(c) \cap h_n(d),
$$
并且由于到定义$\varphi_{n+1}(c) \cap H$都不满足集合$g_{n+1}(c')$（其中$c' \in p_n^{-1}(d)$和$c' < c$），因此从$h_{n+1}(c)$的定义得出$\varphi_{n+1}(c) \cap H = h_{n+1}(c) \cap H$。此外，我们有$H \subset g_{n+1}(c)$，因而，如果$c' \in p_n^{-1}(d)$使得$c' > c$，则$h_{n+1}(c') \cap H$为空。因此断言对于所有$n$都是证明的。

对于每个整数$n$，令$S_n$为集合$h_n(c)$的并，其中$c$贯穿$C_n$。 集合 $S_n$ 是 Borel 集合，我们有 $S_{n+1} \subset S_n$。

令S为集合 S_n的交，它也是X中的Borel集合；我们将证明 S 在一个点中正好满足每个等价类 H mod R。对于每个 n，令 c_n(H) 为唯一元素 c \in C_n，使得 h_{c_n(H)} 满足 H；那么 S_n \cap H = \varphi_n(c_n(H)) \cap H，并且 S \cap H 是集合 \varphi_n(c_n(H)) \cap H 的交。从序列 (c_n(H)) 属于到L.C.、闭集合 \varphi_n(c_n(H)) 的递减序列，其直径趋于0，收敛到点 x \in X，因为X 是完整的。因而，闭合的集合 \varphi_n(c_n(H)) \cap H 的交仅由点 x 组成，并且定理 4 的证明是完整的。

#### 注 {#top-ix-s6-n8-rem-1 .statement tag=0C9C}

特别是，闭等价关系 R 满足定理 4 的假设。当 X 是紧致可度量空间时，定理 4 因此适用于任何 Hausdorff 等价关系 R，因为 Hausdorff 等价关系位于紧致上空间已关闭（章I, § 10, no. 4、命题8）。

### 9. 苏林容量集合

#### 定义 8 {#top-ix-s6-def-8 .statement tag=0C9D}

令 X 为 Hausdorff 拓扑空间。 X 上的容量为 X 的所有子集的集合 \mathscr{P}(X) 的映射 f 进入扩展实直线 \overline{\mathbf{R}}、满足以下条件：

(CA_1) 如果 A \子集 B，则 f(A) \leq f(B)。

(CA_2) 如果 (A_n) 是 X 的子集中的任意递增序列，则
$$
f\left(\bigcup_n A_n\right) = \sup_n f(A_n).
$$

(CA_3) 如果 (K_n) 是 X 的紧凑子集中的任意递减序列，则
$$
f\left(\bigcap_n K_n\right) = \inf_n f(K_n).
$$

#### 例 {#top-ix-s6-n9-exa-1 .statement tag=0C9E}

\* 令 \mu 为局部紧致空间 X 的正测度；那么相应的外测度 \mu^* 就是 X 上的容量。
可以证明，在欧氏空间 \mathbf{R}^n (n \geq 3) 中，“牛顿外容量”是定义 8 意义上的容量。

#### 定义 9 {#top-ix-s6-def-9 .statement tag=0C9F}

令 f 为 X 上的容量；如果 $f(A) = \sup_k f(K)$，则X 的子集 A 被认为是有能力的（相对于 f），其中 K 穿过 A 的紧致子集的集合。

\* 对于例，如果 f 是外部测度 \mu^*，则每个开路集合都是可容的；可积集合 A 使得 \mu^*(A) < +\infty 恰好是 \mu 可积集合。 \*

#### 命题 14 {#top-ix-s6-prop-14 .statement tag=0C9G}

令 K 为紧致空间，令 f 为 K 上的容量。 If A is the intersection of a decreasing sequence $(A_n)$ of subsets of K, each of which is a countable union of closed sets, then A is capacitable.

足以证明，对于每个$a < f(A)$，都有一个闭合的集合$C \subset A$，使得$f(C) \geq a$。 让我们首先证明，存在闭集合的序列$(B_n)_{n \geq 1}$使得$B_n \subset A_n$并且这样，如果我们通过$n \geq 1$的条件$C_0 = A, C_n = C_{n-1} \cap B_n$归纳出定义序列$(C_n)$，那么对于每个$f(C_n) > a$ $n \geq 0$。 假设已经为$i < n$定义了$B_i$；到假设，我们有$C_{n-1} \subset A \subset A_n$和$f(C_{n-1}) > a$；因为$A_n$是闭集合$D_j$的递增序列的并，所以从(CAII)得出
$$
f(C_{n-1}) = \sup_j f(C_{n-1} \cap D_j).
$$
因此有指标$j$使得$f(C_{n-1} \cap D_j) > a$，我们可以取$B_n = D_j$。

现在让$C = \bigcap_n C_n$。从$A = \bigcap_n A_n$和$B_n \subset A_n$开始，我们有
$$
C = \bigcap_n B_n;
$$
因此集合 C 是紧致的并且包含在 A 中。

设 $B'_n = B_1 \cap B_2 \cap \cdots \cap B_n$； $(B'_n)$是K的紧子集的递减序列；正如$C_n \subset C_i \subset B_i$对应$i < n$，我们也有$C_n \subset B'_n$。通过（CAIII），$f(C) = \inf_n f(B'_n)$，从$C \subset C_n \subset B'_n$开始，我们还有$f(C) = \inf_n f(C_n) \geq a$。这样就完成了证明。

#### 定理 5 {#top-ix-s6-thm-5 .statement tag=0C9H}

令X为可度量的空间，并令Y为X的相对紧凑的苏斯林子空间。那么 Y 对于 X 上的每个容量 f 都是有容量的。

我们已经看到 (no. 2, 命题 9)，存在 K 的子集的紧凑空间 K、递减序列 $(A_n)$，其中每一个都是紧集的可数并，以及连续的映射 $\varphi : K \to X$，使得$Y = \varphi \left( \bigcap_n A_n \right)$。到命题 14 时，$\bigcap_n A_n$ 对于 K 上的每个容量都是有能力的。因此，定理 5 是以下命题中的推论：

#### 命题 15 {#top-ix-s6-prop-15 .statement tag=0C9I}

令 $\varphi$ 为 Hausdorff 空间 K 到 Hausdorff 空间 X 的连续映射，并令 f 为 X 上的容量。如果对于 K 的每个子集 A，我们放置 $g(A) = f(\varphi(A))$，则 g 是 K 上的容量；此外，如果 A 对于 g 有能力，则 $\varphi(A)$ 对于 f 有能力。

显然$g$满足公理$(\mathrm{CA}_I)$和$(\mathrm{CA}_{II})$。另一方面，令$(C_n)$为$K$的紧凑子集的递减序列，且令$C = \bigcap_n C_n$； 集合 $\varphi(C)$ 是紧的，它们的交是 $\varphi(C)$；对于这个交当然是包含$\varphi(C)$，并且如果$x \in \varphi(C_n)$对于所有$n$，那么$K$的非空紧凑子集的集合$\overline{\varphi^1}(x) \cap C_n$形式递减序列，因此他们的交不为空。因此我们有$f(\varphi(C)) = \inf_n f(\varphi(C_n))$，即$g(C) = \inf_n g(C_n)$；因此$g$满足公理$(\mathrm{CA}_{III})$，因此是$K$的容量。

现在令$A$为$K$的子集，它可以相对于$g$；如果$a < f(\varphi(A)) = g(A)$，则有紧集$C \subset A$使得$g(C) \geq a$；因而$\varphi(C)$是紧集包含在$\varphi(A)$和$f(\varphi(C)) \geq a$中。这表明$\varphi(A)$对于$f$是有能力的，并且完成命题15的证明，因此完成定理5。

#### 注 {#top-ix-s6-n9-rem-1 .statement tag=0C9J}

\* 如果$\mu$是局部紧凑可度量空间$X$的正测度，则$X$的每个Souslin子集$A$都是$\mu$可测的。因为如果$K$是$X$的任何紧致子集，则$K \cap A$是一个相对紧致的苏斯林集合，因此对于$\mu^*$是可积的，因而$\mu$可积。 注 $X$ 中 Souslin 集合的补集，虽然一般不是 Souslin 集合，但是 $\mu$ 可测*。

### 习题 {#top-ix-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
