---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 2
section_title: Enveloping algebra of a Lie algebra
lang: zh
source: lie-i-iii
book_pages: 12-25, 83-85
pdf_pages: 0030-0043, 0101-0103
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE ENVELOPING ALGEBRA
      page: 12
      pdf_page: 30
    - "no": 2
      title: ENVELOPING ALGEBRA OF A PRODUCT OF LIE ALGEBRAS
      page: 13
      pdf_page: 31
    - "no": 3
      title: ENVELOPING ALGEBRA OF A LIE SUBALGEBRA
      page: 14
      pdf_page: 32
    - "no": 4
      title: ENVELOPING ALGEBRA OF THE OPPOSITE LIE ALGEBRA
      page: 15
      pdf_page: 33
    - "no": 5
      title: SYMMETRIC ALGEBRA OF A MODULE
      page: 16
      pdf_page: 34
    - "no": 6
      title: FILTRATION OF THE ENVELOPING ALGEBRA
      page: 17
      pdf_page: 35
    - "no": 7
      title: THE POINCARÉ–BIRKHOFF–WITT THEOREM
      page: 18
      pdf_page: 36
    - "no": 8
      title: EXTENSION OF DERIVATIONS
      page: 23
      pdf_page: 41
    - "no": 9
      title: EXTENSION OF THE BASE RING
      page: 25
      pdf_page: 43
statements: 22
exercises: 10
content_sha256: f98dffda3be7e72d6c5585f5d6bae9c00d33fdb5ce6cecd1907e15ae657360cd
translated_from: content/en/lie/I/02_s2_enveloping_algebra_of_a_lie_algebra.md
translation_method: google
source_content_sha256: 0efee89afffa5507d5ac319dd9602df1317a1ebd3ab29f31c8942d8c7c2a2199
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 6e8926325fa490717bc39d0b00a4a6fb718e25901f3796d67a5b685bba4b9ad2
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。包络代数的李代数

### 1. 定义封套代数

令 $g$ 为李代数超过 $K$。对于 $K$ 上的任何关联代数与单位元 $L$，$g$ 到 $L$ 的 $\alpha$ 映射是 $g$ 到 $L$ 的 $K$ 线性映射 $\sigma$，使得
$$
\sigma([x, y]) = \sigma(x)\sigma(y) - \sigma(y)\sigma(x) \quad (x, y \text{ in } g)
$$
（在 $g$ 的其他字同态中转换为与 $L$ 相关的李代数）。

如果$L'$与另一个结合代数与单位元超过$K$以及$L$的$\tau$同态入$L'$映射1比1，则$\tau \circ \sigma$是 $g$ 到 $L'$ 的 $\alpha$ 映射。我们将寻找与单位元相关联的代数以及 $g$ 到此代数的 $\alpha$ 映射，它们是通用的（集合理论，章 IV, § 3, no. 1）。

#### 定义 1 {#lie-i-s2-def-1 .statement tag=09UW}

*令$g$为$K$之上的李代数，$K$模$g$的$T$张量代数和$J$生成的$T$的两侧理想张量$x \otimes y - y \otimes x - [x, y]$其中$x \in g, y \in g$。结合律代数 $U = T/J$ 称为 $g$ 的包络代数。 $T$的典范映射到限制到$g$到$U$称为$g$到典范映射到$U$。*

令$T_+$为$T$由……组成的张量的双面理想，其阶0的分量为零。令$T_0 = K.1$为阶0的$T$元素集合。令$U$中的$U_+$和$U_0$为$T_+$和$T_0$的典范像。由于$J \subset T_+$、分解进入直和$T = T_0 + T_+$意味着分解进入直和$U = U_0 + U_+$。因此，代数 $U$ 单位元不同于 0 和 $U_0 = K.1$。对于所有$x \in U$，$U_0$中$x$的分量称为$x$的*常数项*。 元素与常数项零形式$U$的双边理想，即$U$中$g$的典范像生成的双边理想$U^+$。

结合律代数$U$由$U$中$g$的1和典范像生成。

如果$x \in g$和$y \in g$，$x \otimes y - y \otimes x$和$[x, y]$在$T$模$J$全等；因此，如果 $\sigma_0$ 表示 $g$ 的典范映射到 $U$，

$$
\sigma_0(x)\sigma_0(y) - \sigma_0(y)\sigma_0(x) = \sigma_0([x, y])
$$

在$U$。在其他字中，$\sigma_0$是$g$到$U$的$\alpha$映射。

#### 命题 1 {#lie-i-s2-prop-1 .statement tag=09UX}

*令 $\sigma$ 为 $g$ 到代数 $L$ 与单位元的$\alpha$ 映射。存在且仅有一个 $U$ 的同态 $\tau$ 到 $L$，映射 1 比 1，这样 $\sigma = \tau \circ \sigma_0$，其中 $\sigma_0$ 表示 $g$ 的典范映射到 $U$。*

设$\tau'$为$T$的唯一同态到$L$，其中扩展$\sigma$和映射1比1。然后，对于$g$中的$x, y$，

$$
\tau'(x \otimes y - y \otimes x - [x, y]) = \sigma(x)\sigma(y) - \sigma(y)\sigma(x) - \sigma([x, x]) = 0;
$$

因此$\tau'$是$J$上的零和经过上的定义与$U$的商同态$\tau$除以$L$，映射1比1，这样$\sigma = \tau \circ \sigma_0$。从 $\sigma_0(g)$ 开始，$\tau$ 的唯一性是直接的，并且 1 生成代数 $U$。

令$g'$为$K$之上的另一个李代数，$U'$将代数和$\sigma'_0$典范映射包络于$g'$到$U'$。设$\phi$为$g$到$g'$的同态。那么$\sigma'_0 \circ \phi$是$g$到$U'$的$\alpha$映射；因此，存在且仅有一个 $U$ 到 $U'$ 映射 1 比 1 的同态 $\tilde{\phi}$ 且图表

$$
\begin{array}{ccc}
g & \xrightarrow{\phi} & g' \\
\downarrow \sigma_0 & & \downarrow \sigma'_0 \\
U & \xleftarrow{\tilde{\phi}} & U'
\end{array}
$$

是可交换的。常数项为零的$U$的同态映射元素到常数项为零的$U'$的元素。如果$g''$是$K$上的另一个李代数，并且$\phi'$是$g'$的同态到$g''$，则$(\phi' \circ \phi)^{\sim} = \tilde{\phi}' \circ \tilde{\phi}$。

### 2. 包络代数乘积李代数

令$g_1, g_2$是$K$上的两个李代数，$U_i$将$g_i$的代数和$g_i$的$\sigma_i$典范映射包络到$U_i$（$i = 1, 2$）中。令 $g = g_1 \times g_2, U$ 为代数和 $g$ 的 $\sigma$ 典范映射到 $U$ 的包络。 $g_1$和$g_2$的典范嵌入进入$g$ 定义 $U_1$和$U_2$的典范同态进入$U$，其像通勤，因此同态将代数 $U_1 \otimes_K U_2$ 中的$\phi$ 化为代数 $U$，映射 1 比 1。

#### 命题 2 {#lie-i-s2-prop-2 .statement tag=09UY}

*同态$\phi$为代数同构*

映射 $\sigma': (x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)$ ($x_1 \in g_1, x_2 \in g_2$) 是 $g$ 到 $U_1 \otimes_K U_2$ 的 $\alpha$ 映射，因此存在 $U$ 的 (no. 1, 命题 1) 唯一同态 $\tau$ $U_1 \otimes_K U_2$ 映射 1 比 1，使得：

$$(1)$$
$$
\sigma' = \tau \circ \sigma.
$$

现在$\phi \circ \tau \circ \sigma = \phi \circ \sigma' = \sigma$和$\tau \circ \phi \circ \sigma' = \tau \circ \sigma = \sigma'$，因此$\phi \circ \tau$和$\tau \circ \phi$分别是$U$和$U_1 \otimes_K U_2$的恒等映射。因此命题。

$U_1 \otimes_K U_2$ 与同构 $\phi$ 下的$U$ 进行识别。然后$g$到$U$的典范映射由(1)与映射识别：
$$
(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2).
$$

类似地，如果 $g_1, \ldots, g_n$ 是李代数超过 $K$，且包络代数 $U_1, \ldots, U_n$，则 $g_1 \times \cdots \times g_n$ 的包络代数 $U$ 被规范地识别为 $U_1 \otimes_K \cdots \otimes_K U_n$ 和典范映射 $g_1 \times \cdots \times g_n$ 到 $U$ 被识别为映射：
$$
(x_1, \ldots, x_n) \mapsto \sigma_1(x_1) \otimes 1 \otimes \cdots \otimes 1 + \cdots + 1 \otimes \cdots \otimes 1 \otimes \sigma_n(x_n)
$$
（$\sigma_i$ 表示 $g_i$ 中的典范映射到$U_i$）。

### 3. 谎言代数的包围子代数

令$g$为李代数超过$K$，$g$的$h$子代数和$g, h$的$\sigma, \sigma'$典范映射进入它们的包络线代数$U, V$。然后将$h$的典范嵌入$i$转换为$g$定义同态$\tilde{i}$，称为*规范*，将$V$转换为$U$，从而得到$\sigma \circ i = \tilde{i} \circ \sigma'$。 代数 $\tilde{i}(V)$ 由 1 和 $\sigma(h)$ 生成。我们将看到（no. 7，定理 5 的推论）$\tilde{i}$ 在重要情况下是单射的。

如果$h$是$g$的理想，则$\sigma(h)$重合生成的$U$的左理想与$\sigma(h)$生成的右理想，在其他字中它是双面理想$R$。这是因为，对于 $x \in h$ 和 $x' \in g$，
$$
\sigma(x)\sigma(x') = \sigma(x')\sigma(x) + \sigma([x, x'])
$$
和$[x, x'] \in h$。

#### 命题 3 {#lie-i-s2-prop-3 .statement tag=09UZ}

*令$h$为$g$、$g$的$p$典范同态到$g/h$和$W$的理想，$g/h$的包络代数。 同态:*
$$
\tilde{p}: U \to W
$$
*规范地定义$p$是满射，其核是由$\sigma(h)$生成的$U$的理想$R$。*

令 $\sigma''$ 为 $g/\mathfrak{h}$ 的典范映射进入 W。交换律图表：

$$
\begin{array}{ccc}
\mathfrak{h} & \xrightarrow{i} & g \\
\downarrow \sigma' & & \downarrow \sigma \\
V & \xrightarrow{\iota} & U
\end{array}
$$
$$
\begin{array}{ccc}
g & \xrightarrow{p} & g/\mathfrak{h} \\
\downarrow \sigma & & \downarrow \sigma'' \\
U & \xrightarrow{\tilde{p}} & W
\end{array}
$$

证明$\tilde{p}$在$\sigma(\mathfrak{h})$上是零，因此在R上。令$\psi$是U在U/R上的典范同态。 U/R 存在同态 $\phi$

$$
\begin{array}{ccc}
g & \xrightarrow{p} & g/\mathfrak{h} \\
\downarrow \sigma & & \downarrow \sigma'' \\
U & \xrightarrow{\psi} & U/R
\end{array}
$$
$$
\begin{array}{ccc}
U/R & \xleftarrow{\phi'} & W \\
& \uparrow \theta & \\
& \uparrow \phi & \\
U/R & \xrightarrow{\phi} & W
\end{array}
$$

代入 W 使得$\tilde{p} = \phi \circ \psi$。 g 到 U/R 的映射 $\psi \circ \sigma$ 是 $\alpha$ 映射，并且是 $\mathfrak{h}$ 上的零，因此定义是 $g/\mathfrak{h}$ 到 U/R 的 $\alpha$ $\theta$ 映射，使得 $\theta \circ p = \psi \circ \sigma$。然后$\phi \circ \theta \circ p = \phi \circ \psi \circ \sigma = \sigma'' \circ p$。因此$\phi \circ \theta = \sigma''$。在 U/R 映射 1 比 1 中，存在 (no. 1, 命题 1) 个且仅有一个同态 $\phi'$，且$\theta = \phi' \circ \sigma''$。那么$\phi' \circ \phi \circ \theta = \phi' \circ \sigma'' = \theta$和$\phi \circ \phi' \circ \sigma'' = \phi \circ \theta = \sigma''$，因此$\phi' \circ \phi$和$\phi \circ \phi'$分别是U/R和W的恒等映射。这样就完成了证明。

U/R 在同构 $\phi$ 下用 W 标识。然后将$g/\mathfrak{h}$的典范映射$\sigma''$转化为W，用$\theta$来识别，即用$g/\mathfrak{h}$的映射转化为从$\sigma$取商得出的U/R。

### 4. 包络相反的李代数的代数

令$g$是K上的李代数，$g^0$与李代数和$\sigma$相反，以及$g$和$g^0$的$\sigma_0$典范映射进入它们的包络线代数U和V。那么 $\sigma$ 是 $g^0$ 到关联词代数 $U^0$ 的 $\alpha$ 映射，与关联词代数 U 相反。因此，存在且仅有一个 V 到 $U^0$ 的同态 $\phi$ 映射 1 比 1，使得 $\sigma = \phi \circ \sigma_0$。

#### 命题 4 {#lie-i-s2-prop-4 .statement tag=09V0}

*同态 $\phi$ 是 V 的同构到 $U^0$。*

U 存在同态 $\phi'$ 到 $V^0$ 映射 1 比 1 且$\sigma_0 = \phi' \circ \sigma$。 $\phi'$可以被认为是$U^0$的同态变成V。那么$\sigma_0 = \phi' \circ \phi \circ \sigma_0$和$\sigma = \phi \circ \phi' \circ \sigma$，因此$\phi' \circ \phi$和$\phi \circ \phi'$是V和U的恒等映射。因此命题。

V 与同构 $\phi$ 下的$U^0$ 进行标识。那么$\sigma_0$就被识别为$\sigma$。

通过此识别，$g$的同构$\theta : x \mapsto -x$到$g^0$定义同构$\tilde{\theta}$到$V = U^0$。这个同构可以被认为是U的反自同构，称为U的主反自同构。如果$x_1, \ldots, x_n$在$g$中，则：

$$
(2) \quad \tilde{\theta}(\sigma(x_1) \ldots \sigma(x_n)) = \tilde{\theta}(\sigma(x_n)) \ldots \tilde{\theta}(\sigma(x_1)) = (-\sigma(x_n)) \ldots (-\sigma(x_1))
$$
$$
= (-1)^n \sigma(x_n) \ldots \sigma(x_1).
$$

### 5. 对称代数模

设V为K-模。 V 可以以一种独特的方式被视为可交换的李代数。然后可以如下获得V的包络代数：令T为V的张量代数；令 I 为由张量 $x \otimes y - y \otimes x$ ($x \in V, y \in V$) 生成的 T 的两侧理想；然后形式代数$S = T/I$。

回想一下（*代数*，章III, § 6），S被称为V的对称代数，我们简单总结一下这个章，证明所需的性质，其中直接的。令$T^n$为T中阶n的齐次张量的集合。则$I = (I \cap T^2) + (I \cap T^3) + \cdots$，因此S为$T^n$的典范像$S^n$的直和。 $S^n$的元素称为次数n的齐次。 $S^0 = K.1, S^1$ 与V 和$S^n S^p \subset S^{n+p}$ 进行识别。 代数 S 由 1 和 $S^1 = V$ 生成。显然 $S^1$ 中的任意两个元素都是可置换的，因此 S 是可交换的。如果 V 是自由K-模，其中基 $(x_\lambda)_{\lambda \in \Lambda}$，则将多项式代数 $K[X_\lambda]_{\lambda \in \Lambda}$ 的典范同态 f 放到 S 上，其中映射 1 到 1 且 $X_\lambda$ 到 $x_\lambda$ 对于所有$\lambda \in \Lambda$ 是同构：对于 S 的泛性质 (no. 1，命题 1)，存在同态 g 的 S 进入$K[X_\lambda]_{\lambda \in \Lambda}$，其中映射 1 到 1，$x_\lambda$ 到$X_\lambda$ 对于所有 $\lambda \in \Lambda$ 且 f 和 g 是另一个的逆同态。

设${S'}^n \subset T^n$为阶n的齐次对称张量的集合(*代数*,章III, § 5, no. 1,定义2)。如果K是特征0的域，则${S'}^n$和$I \cap T^n$在$T^n$中互补。令 $(x_\lambda)_{\lambda \in \Lambda}$ 为 V 中的基。我们给$\Lambda$一个总排序（*集合理论*，章III, § 2, no. 3，定理1）。令$\Lambda_n$为$\Lambda$的n个元素中的递增序列中的集合。对于$M = (\lambda_1, \ldots, \lambda_n) \in \Lambda_n$，让

$$
y_M = \frac{1}{n!} \sum_{\sigma \in S_n} x_{\lambda_{\sigma(n)}} \otimes \cdots \otimes x_{\lambda_{\sigma(n)}}.
$$

向量K空间${S'}^n$的生成元的$M \in \Lambda_n$形式系统的$y_M$。现在，根据上一段，$S^n$中的典范像构成了$S^n$中的基。因此，$(y_M)_{M \in \Lambda_n}$是$T^n$中$I \cap T^n$的补充子空间的基（*代数*，章II, § 1, no. 6，命题4），从而建立了我们的断言。

因此，当K为特征0的域时，典范映射$T^n \to S^n$的限制到${S'}^n$是空间${S'}^n$到空间$S^n$的同构，因此有逆同构。因此，对于空间 S 的每个 n 定义典范同构到空间获得逆同构

$$
S' = \sum_{n \geq 0} {S'}^n \text{ of symmetric tensors}.
$$

### 6. 包络过滤代数

令$g$是$K$模块$g$的$K$和$T$张量代数的李代数。令$T^n$为阶$n$和$T_n = \sum_{i \leq n} T^i$的齐次张量的$T$由……组成的子模。然后是$T_n \subset T_{n+1}$、$T_0 = K.1$、$T_{-1} = \{0\}$和$T_n T_p \subset T_{n+p}$。

令$U_n$为$T_n$的典范像，并且在$g$的包络线代数$U$中。然后是$U_n \subset U_{n+1}$、$U_0 = K.1$、$U_{-1} = \{0\}$和$U_n U_p \subset U_{n+p}$；因此 $U$ 可以描述为代数 *由* $U_n$ (*交换代数*, 章 III, § 2, no. 1) 过滤； $U_n$的元素将被称为*过滤*$\leq n$。

令$G^n$为$K$-模块$U_n / U_{n-1}$，让$G$为$G^n$的$K$-模块直和。 $U$ 定义上的乘法，在取商时，$G^n \times G^m$到$G^{n+m}$的双线性映射，因此$G \times G$到$G$的双线性映射，这是结合的。因此 $G$ 被赋予关联性 $K$-代数结构。然后$G^n G^m \subset G^{n+m}$。 $G^n$的元素据说是*次数* $n$。由此获得的分级代数正是与过滤后的代数$U$相关联的分级代数（*交换代数*，章III, § 2, no. 3）。

令 $\phi_n$ 为规范 $K$ 线性映射的合成

$$
T^n \to U_n \to G^n.
$$

由于$T^n$是$T_n$中$T_{n-1}$的补充，$\phi_n$是满射。 $\sum_n T^n = T$ 的$\phi_n$ 定义 $K$-线性映射$\phi$ 到$\sum_n G^n = G$。

#### 命题 5 {#lie-i-s2-prop-5 .statement tag=09V1}

*$T$到$G$的映射$\phi$是代数同态映射1比1，并且是张量$x \otimes y - y \otimes x$（$x \in g, y \in g$）生成的双面理想上的零。*

如果$t \in T^n$和$t' \in T^p$，则$G$上$\phi(t)\phi(t') = \phi(tt')$乘定义除乘法。因此$\phi$是代数同态并且显然是$\phi(1) = 1$。如果$x, y$在$g$中，则$U_2$中该元素的$x \otimes y - y \otimes x \in T^2$和典范像等于$[x, y]$，因此属于到$U_1$。因此$\phi(x \otimes y - y \otimes x) = 0$，证明了命题。

令$S$为$K$模块$g$的对称代数和$T$的$\tau$典范同态到$S$的对称。 命题 5证明存在唯一同态$\omega$，称为*规范*，将代数$S$到代数$G$，映射1比1，使得$\phi = \omega \circ \tau$。我们有$\omega(S^n) = \phi(T^n) = G^n$。令$\tau_n$为$\tau$至$T^n$的限制、$\omega$至$S^n$的$\omega_n$限制、$T^n$的$\psi_n$典范映射代入$U_n$的$U_n$和$\theta_n$典范映射到$G^n$。 $\omega_n$的定义证明以下图表是可交换的：

$$
\begin{array}{ccccc}
T^n & \xrightarrow{\psi_n} & U_n & \xrightarrow{\theta_n} & G^n \\
& \searrow & & \swarrow & \\
& & S^n & \xrightarrow{\omega_n} &
\end{array}
$$

#### 命题 6 {#lie-i-s2-prop-6 .statement tag=09V2}

*如果K是诺特并且g是有限生成模，则环U是正确的并且左诺特的。*

S 是 K 上有限生成的代数，因此诺特环（*交换代数*，章 III, § 2, no. 10，推论 3 到定理 2）。因此，与 S 的商环同构的 G 是诺特。因此 U 是正确的且左诺特的 (*交换代数*, 章 III, § 2, no. 10, *注 2*)。

#### 推论{#lie-i-s2-n6-cor-1 .statement tag=09V3}

*假设 K 为域并且 g 是 K 上的有限维。令 I₁, ..., Iₘ 为 U 中有限余维的右（或左）理想。则乘积理想I₁I₂...Iₘ 等于有限余维。*

通过 m 上的归纳，足以考虑对于例两个正确理想的情况。右 U 模 I₁ 由元素 u₁, ..., uₚ (命题 6) 的有限数生成。令 v₁, ..., vₐ 为 U 的元素，其类模 I₂ 生成向量空间 U/I₂。然后 uᵢvⱼ 生成向量空间 I₁/I₁I₂ 的 I₁/I₁I₂ 中的典范像，因此是有限维的。因此，dim_K(U/I₁I?) = dim_K(U/I₁) + dim_K(I₁/I₁I?) < +∞。

#### 注 {#lie-i-s2-n6-rem-1 .statement tag=09V4}

设g'在环K上为另一个李代数，U'其包络代数，过滤$\leq n$U'元素U'_n集合和U^n(resp.U'^n)集合典范像在阶 n 的 g（分别为 g'）的齐次对称张量的 U（分别为 U'）中。令$\eta$为g到g'的同态，并令$\tilde{\eta}$为U到U'的相应的同态。然后

$$
\tilde{\eta}(U_n) \subset U'_n, \quad \tilde{\eta}(U^n) \subset {U'}^n.
$$

特别是，U 的主要反自同构使 U_n 和 U^n 保持稳定。 T^n 的 K-线性映射自身映射

$$
x_1 \otimes x_2 \otimes \cdots \otimes x_n \quad \text{to} \quad x_n \otimes x_{n-1} \otimes \cdots \otimes x_1
$$

因为 g 中的所有 $x_1, ..., x_n$ 都是对称算子，因此阶 n 的齐次对称张量是固定的。因此，U 诱导在比率 $(-1)^n$ 的每个 U^n 位似上存在主要反自同构。

### 7. 庞加莱-伯霍夫-威特定理

#### 定理 1 {#lie-i-s2-thm-1 .statement tag=09V5}

*令 g 为谎言 K-代数，U 为其包络代数，G 为与过滤后的代数 U 相关的分级代数，S 为 K-模 g 的对称代数。如果 g 为自由K-模，则典范同态 $\omega : S \to G$ 为同构。*

设$(x_\lambda)_{\lambda \in \Lambda}$为K-模g中的基；我们给$\Lambda$一个总排序（*集合理论*，章III, § 2, no. 3，定理1）。令 P 为对应与 $x_\lambda$ 一对一的不定式 $z_\lambda$ 中的多项式代数 $K[z_\lambda]_{\lambda \in \Lambda}$。对于$\Lambda$的元素的每个序列$M = (\lambda_1, \lambda_2, ..., \lambda_n)$，令$z_M$表示单项式$z_{\lambda_1}z_{\lambda_2}...z_{\lambda_n}$和$x_M$张量$x_{\lambda_1} \otimes x_{\lambda_2} \otimes \cdots \otimes x_{\lambda_n}$。

$z_M$，对于 M 递增，K-模 P 的形式基（我们约定$\varnothing$ 是递增序列以及$z_\varnothing = 1$）。令 $P_p$ 为次数 $\leq p$ 多项式的子模。我们首先要证明几个引理。 （为了简化，我们将序列 M 的每指标 $\mu$ 写成 $\lambda \leq M$ if $\lambda \leq \mu$。）

#### 引理 1 {#lie-i-s2-lem-1 .statement tag=09V6}

*对于每个整数$p \geq 0$，K-模$g \otimes_K P_p$中存在唯一同态$f_p$进入K-模P满足以下条件：*
$$
\begin{align*}
(A_p) \quad & f_p(x_\lambda \otimes z_M) = z_\lambda z_M \quad \text{for } \lambda \leq M, z_M \in P_p; \\
(B_p) \quad & f_p(x_\lambda \otimes z_M) - z_\lambda z_M \in P_q \quad \text{for } z_M \in P_q, q \leq p; \\
(C_p) \quad & f_p(x_\lambda \otimes f_p(x_\mu \otimes z_N)) = f_p(x_\mu \otimes f_p(x_\lambda \otimes z_N)) + f_p([x_\lambda, x_\mu] \otimes z_N)
\end{align*}
$$
*$z_N \in P_{p-1}$。 （（C_p）中出现的项对（B_p）来说是有意义的。）*

此外，$f_p$的限制到$g \otimes P_{p-1}$重合与$f_{p-1}$。

由于 $f_p$ 到 $g \otimes_K P_{p-1}$ 的限制满足条件 (A_{p-1})、(B_{p-1}) 和 (C_{p-1})，所以最后一个断言是其他的。我们将通过$p$上的归纳证明$f_p$的存在性和唯一性。对于$p = 0$，条件(A_0)给出$f_0(x_\lambda \otimes 1) = z_\lambda$，条件(B_0)和(C_0)显然是满足的。现在假设$f_{p-1}$的存在性和唯一性都被证明了。我们证明$f_{p-1}$承认唯一的扩张$f_p$到$g \otimes_K P_p$满足条件（A_p），（B_p）和（C_p）。

我们必须为 $p$ 元素的递增序列 M 定义 $f_p(x_\lambda \otimes z_M)$。

如果 $\lambda \leq M$，值由条件 (A_p) 给出。否则，M可以唯一地写成形式($\mu, N$)，其中$\mu < \lambda, \mu \leq N$。然后
$$
z_M = z_\mu z_N = f_{p-1}(x_\mu \otimes z_N)
$$
通过 (A_{p-1})，因此 (C_p) 的左侧为 $f_p(x_\lambda \otimes z_M)$。现在 (C_p) 的右侧已经定义：for (B_{p-1}) 允许我们写：
$$
f_p(x_\lambda \otimes z_N) = f_{p-1}(x_\lambda \otimes z_N) = z_\lambda z_N + w
$$
其中$w \in P_{p-1}$；因此 (C_p) 的右侧变为：
$$
z_\lambda z_\mu z_N + f_{p-1}(x_\mu \otimes w) + f_{p-1}([x_\lambda, x_\mu] \otimes z_N).
$$

因此$f_p$被唯一定义并且显然满足条件(A_p)和(B_p)。如果$\mu < \lambda, \mu \leq N$则满足条件(C_p)。由于$[x_\mu, x_\lambda] = -[x_\lambda, x_\mu]$，条件(C_p)也满足$\lambda < \mu, \lambda \leq N$。由于 (C_p) 对于 $\lambda = \mu$ 来说是简单满足的，因此如果 $\lambda \leq N$ 或 $\mu \leq N$ 则满足 (C_p)。如果这些不等式都不成立，则 $N = (\nu, Q)$，其中 $\nu \leq Q, \nu < \lambda, \nu < \mu$。从今以后将$f_p(x \otimes z) = xz$缩写为$x \in g$和$z \in P_p$，我们得到归纳假设：
$$
x_\mu z_N = x_\mu(x_\nu z_Q) = x_\nu(x_\mu z_Q) + [x_\mu, x_\nu]z_Q.
$$

现在$z_\mu z_Q$是形式$z_\mu z_Q + w$，其中$w \in P_{p-2}$。 (C_p) 可应用于 $x_\lambda(x_\nu(z_\mu z_Q))$，因为 $\nu \leq Q$ 和 $\nu < \mu$，并且可通过归纳假设应用于 $x_\lambda(x_\nu w)$，从而应用于 $x_\lambda(x_\nu(x_\mu z_Q))$。因此：
$$
x_\lambda(x_\mu z_N) = x_\nu(x_\lambda(x_\mu z_Q)) + [x_\lambda, x_\nu](x_\mu z_Q) + [x_\mu, x_\nu](x_\lambda z_Q)
+ [x_\lambda, [x_\mu, x_\nu]]z_Q.
$$

交换 $\lambda$ 和 $\mu$ 并相减：

$$
x_{\lambda}(x_{\mu}z_{N}) - x_{\mu}(x_{\lambda}z_{N}) = x_{v}(x_{\lambda}(x_{\mu}z_{Q}) - x_{\mu}(x_{\lambda}z_{Q}))
+ [x_{\lambda}, [x_{\mu}, x_{v}]]z_{Q} - [x_{\mu}, [x_{\lambda}, x_{v}]]z_{Q}
= x_{v}([x_{\lambda}, x_{\mu}]z_{Q}) + [x_{\lambda}, [x_{\mu}, x_{v}]]z_{Q} + [x_{\mu}, [x_{v}, x_{\lambda}]]z_{Q}
= [x_{\lambda}, x_{\mu}](x_{v}z_{Q}) + ([x_{v}, [x_{\lambda}, x_{\mu}]]
+ [x_{\lambda}, [x_{\mu}, x_{v}]] + [x_{\mu}, [x_{v}, x_{\lambda}]])z_{Q}
$$

因此由雅可比恒等式

$$
x_{\lambda}(x_{\mu}z_{N}) - x_{\mu}(x_{\lambda}z_{N}) = [x_{\lambda}, x_{\mu}]z_{N}
$$

完成引理 1 中的证明。

#### 引理 2 {#lie-i-s2-lem-2 .statement tag=09V7}

*存在$g$到$\mathscr{L}_{K}(P)$的$\alpha$映射$\sigma$，使得：*

(1) $\sigma(x_{\lambda})z_{M} = z_{\lambda}z_{M}$ 为 $\lambda \leq M$；
(2) $\sigma(x_{\lambda})z_{M} \equiv z_{\lambda}z_{M}$ (mod. $P_{p}$) 如果 $M$ 有 $p$ 元素。

到引理 1 时，K-模 $g \otimes_{K} P_{p}$ 中存在同态 $f$ 到 $P$ 满足，对于所有 $p$、条件 (A$_{p}$)、(B$_{p}$)， (C$_{p}$)（其中$f_{p}$替换为$f$）。 K-模 $g$ 到 K-模 $\mathscr{L}_{K}(P)$ 和 $\sigma$ 的同态定义同态 $\sigma$ 是$\alpha$ 映射，因为条件 （C$_{p}$）。最后，由于条件（A$_{p}$）和（B$_{p}$），$\sigma$满足引理的性质（1）和（2）。

#### 引理 3 {#lie-i-s2-lem-3 .statement tag=09V8}

*令$T_{n} \cap J$中的$t$为张量。 阶$n$$t$的齐次分量$t_{n}$在典范同态$T \to S$的核$I$中。*

我们将形式$\sum_{i=1}^{r} x_{M_{i}}$写成$t_{n}$，其中$M_{i}$是$n$的序列，$\Lambda$的元素。 映射$\sigma$扩展到代数$T$的同态变成代数$\mathscr{L}_{K}(P)$（我们也用$\sigma$表示），即$J$上的零。通过引理 2，$\sigma(t) . 1$ 是一个多项式，其最高次数中的项为 $\sum_{i=1}^{r} z_{M_{i}}$。作为$t \in J$、$\sigma(t) = 0$，因此在$P$中为$\sum_{i=1}^{r} z_{M_{i}} = 0$。现在 $P$ 被规范地标识为 $S$，因为 $g$ 具有基 $(x_{\lambda})$。因此$S$中$t_{n}$的典范像是零，即$t_{n} \in I$。

现在我们可以证明定理 1。需要证明$S$到$G$的典范同态是单射的。在其他字中，如果$t \in T^{n}$和$\psi$将$T$的典范同态表示到$U$上，则需要证明条件$\psi(t) \in U_{n-1}$隐含$t \in I$。现在$\psi(t) \in U_{n-1}$意味着存在张量$t' \in T_{n-1}$使得$t - t' \in J$。 张量 $t - t'$ 承认 $t$ 为阶 $n$ 的齐次分量，因此 $t \in I$ 为引理 3。

#### 推论 1 {#lie-i-s2-lem-3-cor-1 .statement tag=09V9}

*假设 $g$ 是一个免费的 $K$ 模块。令 $W$ 为 $T^{n}$ 的子 K 模。*

*如果，在图表*的记号(3)中，*$\tau_n$*到*$W$*的*限制是*$W$*到*$S^n$的同构，*则*$\psi_n$*到*的限制 $W$ *是* $W$ *的同构 *到* $U_{n-1}$ *的补充 *在* $U_n$。

$\omega_n \circ \tau_n$的限制到$W$是$W$的双射到$G^n$； 限制 $\theta_n \circ \psi_n$ 至 $W$ 也是如此。由此得出推论。

#### 推论 2 {#lie-i-s2-lem-3-cor-2 .statement tag=09VA}

*如果 $g$ 是自由K-模，则 $g$ 的典范映射进入其包络线代数是单射的。*

这是从取 $W = T^1$ 的推论 1 得出的。

当$g$为自由K-模时（特别是当K为域时），$g$与$g$的典范映射下的$U$的子模识别为$U$。本公约自以下推论起采用。

#### 推论 3 {#lie-i-s2-lem-3-cor-3 .statement tag=09VB}

*如果$g$承认包络代数$U$的全序基$(x_\lambda)_{\lambda \in \Lambda}$、元素$x_{\lambda_1} x_{\lambda_2} \ldots x_{\lambda_n}$，其中$(\lambda_1, \ldots, \lambda_n)$是元素的任意递增有限序列 $\Lambda$、形式基共 K-模 $U$。*

令$\Lambda_n$为$\Lambda$的$n$元素的递增序列中的集合。对于$M = (\lambda_1, \ldots, \lambda_n) \in \Lambda_n$，设$y_M = x_{\lambda_1} \otimes x_{\lambda_2} \otimes \cdots \otimes x_{\lambda_n}$。令$W$为$T^n$的子模和基$(y_M)_{M \in \Lambda_n}$。推论1表明，$\psi_n$到$W$的限制是$W$的同构到$U_n$中$U_{n-1}$的补充。但是

$$
\psi_n(y_M) = x_{\lambda_1} x_{\lambda_2} \ldots x_{\lambda_n},
$$

从而推论。

#### 推论 4 {#lie-i-s2-lem-3-cor-4 .statement tag=09VC}

*令 ${S'}^n \subset T^n$ 为阶 n 的齐次对称张量的集合。假设K是特征0的域，那么典范映射*的复合映射

$$
S^n \to {S'}^n \to U_n
$$

*是 $U_n$ 中向量空间 $S^n$ 的同构到$U_{n-1}$ 的补充。*

这是从采用 $W = {S'}^n$ 的推论 1 得出的。

假设此后 K 是特征 0 的域。令 $\eta_n$ 为刚刚定义的 $U_n$ 中 $S^n$ 的映射。让$U^n = \eta_n(S^n)$。 向量空间 $U$ 是 $U^n$ 的直和。 向量空间$S = \sum_n S^n$到向量空间$U = \sum_n U^n$的$\eta_n$定义同构$\eta$，称为S到U*的*典范同构；这*不是*代数同构。我们有交换律图表：

$$
\begin{array}{ccccc}
& & U^n & & \\
& \nearrow \psi_n & \uparrow \eta_n & \searrow \theta_n & \\
{S'}^n & & & & G^n \\
& \searrow \tau_n & & \nearrow \omega_n & \\
& & S^n & &
\end{array}
$$

其中每个箭头代表向量空间同构。如果$x_1, x_2, \ldots, x_n$在$g$、$\eta_n$ 映射乘积 $x_1 x_2 \ldots x_n$，则按$S$计算，到元素

$$
\frac{1}{n!} \sum_{\sigma \in S_n} x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)}
$$

按$U$计算。

#### 推论 5 {#lie-i-s2-lem-3-cor-5 .statement tag=09VD}

*令$h$为李代数$g$的子代数和$U'$其包络代数。假设$K$-模块$h$和$g/h$是免费的（对于例，如果$K$是域）。设$(x_\alpha)_{\alpha \in L}$为$h$的基，$(y_\beta)_{\beta \in M}$为$g$的元素的家庭，其典范像在$g/h$形式基为$g/h$。

(a) *$U'$到$U$的典范同态是单射的。*

(b) *如果$M$全序，元素$y_{\beta_1} \ldots y_{\beta_q}$，其中$U$中的$\beta_1 \leq \cdots \leq \beta_q$、形式基被视为$U'$上的左或右模。*

我们给$L \cup M$一个总排序，使得$L$的每个元素都小于$M$的每个元素。 元素 $x_{\alpha_1} x_{\alpha_2} \ldots x_{\alpha_p}$ 在 $U'$（其中 $\alpha_1 \leq \cdots \leq \alpha_p$）形式基中计算$U'$（推论 3）。 元素

$$
x_{\alpha_1} \ldots x_{\alpha_p} y_{\beta_1} \ldots y_{\beta_q}
$$

$U$（其中$\alpha_1 \leq \cdots \leq \alpha_p \leq \beta_1 \leq \cdots \leq \beta_q$）类似地计算$U$的形式基。因此，$U'$的典范同态转化为$U'$的基的$U$映射元素到$U$的线性无关的元素，因此是单射的。此外可以看出，$U$的$y_{\beta_1} \ldots y_{\beta_q}$（其中$\beta_1 \leq \cdots \leq \beta_q$）形式基被视为左$U'$模块。对$L \cup M$进行排序，使得$M$的每个元素小于$L$的每个元素，同样可以看出$y_{\beta_1} \ldots y_{\beta_q}$（其中$\beta_1 \leq \cdots \leq \beta_q$）形式基被视为$U$的右$U'$-模块。

在推论5的条件下，$U'$与$h$通过$U'$的典范同态进入$U$生成的$U$的子代数进行识别。

#### 推论 6 {#lie-i-s2-lem-3-cor-6 .statement tag=09VE}

*假设$K$-模块$g$是直和/子代数$g_1, g_2, \ldots, g_n$，并且每个$g_i$都是一个免费的$K$-模块。令 $U_i$ 为 $g_i$ ($1 \leq i \leq n$) 的包络代数。令$\phi$为$K$模块$U_1 \otimes_K \cdots \otimes_K U_n$到$U$的$K$线性映射，由$U_1 \times \cdots \times U_n$到$U$的多线性映射$(u_1, \ldots, u_n) \mapsto u_1 \ldots u_n$定义。那么$\phi$是一个$K$模块同构。*

令 $(x^i_{\lambda})_{\lambda \in L_i}$ 为 $g_i$ 中的基。我们总共阶$L_1 \cup \cdots \cup L_n$，这样$L_i$的每个元素就超过了$i \geq j$的$L_j$的每个元素。然后元素：

$$
(x^1_{\lambda_1} x^1_{\lambda_2} \ldots x^1_{\lambda_p}) \otimes \cdots \otimes (x^n_{v_1} x^n_{v_2} \ldots x^n_{v_q}),
$$

其中$\lambda_1 \leq \lambda_2 \leq \cdots \leq \lambda_p \leq \cdots \leq v_1 \leq v_2 \leq \cdots \leq v_q$，构成$U_1 \otimes_K \cdots \otimes_K U_n$的基。它们由 $\phi$ 映射到元素：

$$
x^1_{\lambda_1} x^1_{\lambda_2} \ldots x^1_{\lambda_p} \ldots x^n_{v_1} x^n_{v_2} \ldots x^n_{v_q}
$$

构成 $U$ 的基。由此得出推论。

#### 推论 7 {#lie-i-s2-lem-3-cor-7 .statement tag=09VF}

*如果 K 为整环并且 g 为自由K-模，则代数 U 没有零的除子。*

G 同构于 K (定理 1) 上的多项式代数，因此是整环 (*代数*, 章 IV, § 1, no. 4, 定理 1)。因此推论 (*交换代数*, 章 III, § 2, no. 3, 命题 1)。

### 8. 扩张推导

#### 引理 4 {#lie-i-s2-lem-4 .statement tag=09VG}

*设 V 为 K-模，T 张量代数为 V。让你成为V中的自同态。 T 中存在且仅有一个推导，其中扩展 u。这个推导与 T 上的对称算子交换。*

令 F = V × V × ... × V (n 因子)。 映射
$$
(x_1, \ldots, x_n) \mapsto ux_1 \otimes x_2 \otimes \cdots \otimes x_n \\
+ x_1 \otimes ux_2 \otimes \cdots \otimes x_n + \cdots + x_1 \otimes x_2 \otimes \cdots \otimes ux_n
$$
F 到 $\bigotimes^n V$ 是多重线性的。因此存在 $\bigotimes^n V$ 的自同态 $u_n$ 使得：
$$
u_n(x_1 \otimes \cdots \otimes x_n) = ux_1 \otimes \cdots \otimes x_n + \cdots + x_1 \otimes \cdots \otimes ux_n
$$
对于V中的所有$x_1, \ldots, x_n$。然后$u_1 = u$。令v为K-模T的自同态，其中重合在每个$T^n = \bigotimes^n V$上有$u_n$，并且在$T^0 = K.1$上有零。我们证明 v 是 T 的推导。如果 $x_1, \ldots, x_n, y_1, \ldots, y_p$ 是 V 的元素，那么
$$
v((x_1 \otimes \cdots \otimes x_n) \otimes (y_1 \otimes \cdots \otimes y_p)) \\
= \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes ux_i \otimes x_{i+1} \otimes \cdots \otimes x_n \otimes y_1 \otimes \cdots \otimes y_p \\
+ \sum_{j=1}^p x_1 \otimes \cdots \otimes x_n \otimes y_1 \otimes \cdots \otimes y_{j-1} \otimes uy_j \otimes y_{j+1} \otimes \cdots \otimes y_p \\
= v(x_1 \otimes \cdots \otimes x_n) \otimes (y_1 \otimes \cdots \otimes y_p) + (x_1 \otimes \cdots \otimes x_n) \otimes v(y_1 \otimes \cdots \otimes y_p).
$$
根据线性关系，v 为推导。 v 的唯一性是显而易见的。最后，显然 $u_n$ 与 $\bigotimes^n V$、从而最后一个断言上的所有对称算子都可交换。

#### 命题 7 {#lie-i-s2-prop-7 .statement tag=09VH}

*Let g be a Lie algebra, U its enveloping algebra, σ the canonical mapping of g into U and D a derivation of g.*
(a) *There exists one and only one derivation $D_U$ of U such that $\sigma \circ D = D_U \circ \sigma$ (that is such that $D_U$ extends D, when g can be identified with a submodule of U under σ).
(b) $D_U$ leaves stable $U_n$ and the set $U^n$ of images in U of the homogeneous symmetric tensors of order n over g.

(c) $D_U$ 与 $U$ 的主要反自同构可交换。

(d) *如果$D$是$g$的元素$x$定义的$g$的内部推导，则$D_U$是$\sigma(x)$定义的$U$的内部推导。*

令 $D_T$ 为张量代数 $T$ $g$ 的推导，其中扩展 $D$ (引理 4)。由 $T$ 生成的双边理想 $J$

$$
x \otimes y - y \otimes x - [x, y]
$$

$g$中的$(x, y$）在$D_T$下是稳定的。为了：

$$
D_T(x \otimes y - y \otimes x - [x, y]) = Dx \otimes y - y \otimes Dx - [Dx, y]
$$
$$
+ x \otimes Dy - Dy \otimes x - [x, Dy].
$$

在经过上对 $U$ 进行$D_T$ 定义推导 $D_U$ 的商，使得 $\sigma \circ D = D_U \circ \sigma$。 $D_U$的唯一性从1开始就是直接的，并且$\sigma(g)$生成代数$U$。 断言 (b) 是显而易见的。设$A$为$U$的主要反自同构。现在我们证明(c)。如果$x_1, \ldots, x_n$在$g$中，那么

$$
D_U A(\sigma(x_1) \ldots \sigma(x_n)) = D_U((-1)^n \sigma(x_n) \ldots \sigma(x_1))
$$
$$
= (-1)^n \sum_{i=1}^n \sigma(x_n) \ldots D_U(\sigma(x_i)) \ldots \sigma(x_1)
$$
$$
= (-1)^n \sum_{i=1}^n \sigma(x_n) \ldots \sigma(Dx_i) \ldots \sigma(x_1)
$$
$$
= A \left( \sum_{i=1}^n \sigma(x_1) \ldots \sigma(Dx_i) \ldots \sigma(x_n) \right)
$$
$$
= AD_U(\sigma(x_1) \ldots \sigma(x_n)).
$$

最后让$x \in g$。令 $\Delta$ 为 $U$ 的内部推导 $y \mapsto \sigma(x)y - y\sigma(x)$ (*代数*, 章 IV, § 4, no. 3, *例 2*)。那么，对于 $x' \in g$，

$$
(\Delta \circ \sigma)(x') = \sigma(x)\sigma(x') - \sigma(x')\sigma(x) = \sigma([x, x']) = (\sigma \circ \mathrm{ad}\, x)(x'),
$$

从而$\Delta \circ \sigma = \sigma \circ \mathrm{ad}\, x$。这样就完成了证明。

应用命题7对于可交换李代数的情况，可以看出$K$模的每个自同态$u$都可以唯一地扩展到该模的对称代数的推导；这个推导是在经过上导出推导与张量代数的商，其中扩展$u$。

我们再次取李代数$g$除以$K$，并令$D$为推导除以$g$。我们使用早期的记号$T, S, U, G$。令$D_T, D_S$为$T, S$的推导，其中扩展$D$，并令$D_U$为$U$的唯一推导，使得$\sigma \circ D = D_U \circ \sigma$。由于$D_U$使$U_n$保持稳定，因此$D_U$定义取$G$的商推导$D_G$。由于当经过为商时，$D_U$和$D_S$是从$D_T$导出的，因此交换性图表（3）证明$D_G$也可以由$D_S$通过同态$\omega$导出no. 6。若进一步$K$为特征0的域，则图表的同构 (4)映射一为$D_T, D_S, D_U, D_G$至${S'}^n, S^n, U^n, G^n$的另一个限制。因此，$S$的典范同构到$U$映射$D_S$到$D_U$。

### 9. 扩张基环

令$g$为李代数超过$K$，$T$其张量代数，$J$由$x \otimes y - y \otimes x - [x, y]$生成的$T$的两侧理想（$x, y$在$g$）和$U = T/J$。设$K_1$为交换环，其中$K$的单位元和$\sigma$同态化为$K_1$映射1比1。然后张量代数 $g_{(K_1)}$ 被规范地标识为 $T_{(K_1)}$。令 $J'$ 为由 $T_{(K_1)}$ 生成的两侧理想

$$
x' \otimes y' - y' \otimes x' - [x', y']
$$

（$g_{(K_1)}$中的$x', y'$）。显然$T_{(K_1)}$中的$J_{(K_1)}$的典范像包含在$J'$中。要看出它等于$J'$，只要证明，如果$x'$和$y'$表示$g_{(K_1)}$中的两个元素，则$x' \otimes y' - y' \otimes x' - [x', y']$属于等于这个像。现在

$$
x' = \sum_i x_i \otimes \lambda_i, y' = \sum_j y_j \otimes \mu_j \quad (x_i, y_j \text{ in } g, \lambda_i, \mu_j \text{ in } K_1);
$$

从而

$$
x' \otimes y' - y' \otimes x' - [x', y'] = \sum_{i,j} (x_i \otimes y_j - y_j \otimes x_i - [x_i, y_j]) \otimes \lambda_i \mu_j
$$

这证明了我们的断言。然后可以看出，$U_{(K_1)} = (T/J)_{(K_1)}$ 被规范地标识为 $T_{(K_1)}/J'$：*将 $g_{(K_1)}$ 的代数规范地标识为 $U_{(K_1)}$*，将 $g_{(K_1)}$ 的典范映射规范地标识为它的包络代数被标识为 $\sigma \otimes 1$ （其中$\sigma$表示$g$到$U$的典范映射）。

### 习题 {#lie-i-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
