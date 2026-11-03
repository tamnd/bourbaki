---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 5
section_title: Infinite sums in commutative groups
lang: zh
source: top-i-iv
book_pages: 261-270
pdf_pages: 0267-0276, 0320-0321
extraction: ocr
subsections:
    - "no": 1
      title: SUMMABLE FAMILIES IN A COMMUTATIVE GROUP
      page: 261
      pdf_page: 267
    - "no": 2
      title: CAUCHY'S CRITERION
      page: 262
      pdf_page: 268
    - "no": 3
      title: PARTIAL SUMS ; ASSOCIATIVITY
      page: 264
      pdf_page: 270
    - "no": 4
      title: SUMMABLE FAMILIES IN A PRODUCT OF GROUPS
      page: 266
      pdf_page: 272
    - "no": 5
      title: IMAGE OF A SUMMABLE FAMILY UNDER A CONTINUOUS HOMOMORPHISM
      page: 267
      pdf_page: 273
    - "no": 6
      title: SERIES
      page: 267
      pdf_page: 273
    - "no": 7
      title: COMMUTATIVELY CONVERGENT SERIES
      page: 269
      pdf_page: 275
statements: 19
exercises: 7
content_sha256: 0e79455419f28a2340e1dbf96e3695c1b65eaffdfb0f31320db627e20e3fea6f
translated_from: content/en/top/III/05_s5_infinite_sums_in_commutative_groups.md
translation_method: google
source_content_sha256: 91048f1fa3704dfbdf345b8175de3a71f69a6c736f07b39c3b412650ede3cf78
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: e15b53a80bd2e2ac916462bca88c100c8b4c9d8840fe546c40267886996ff575
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 5. 可交换群中的无限和

### 1. 可交换族群

在这个截面中，我们只关心*豪斯多夫交换拓扑群*，其合成的律被写成*加法*。只有最重要的结果才会被转换为乘法记号。

令$G$为Hausdorff交换律群，令$I$为任意指标集合，并令$(x_i)_{i \in I}$为$G$的点族，索引为$I$。对于$I$的每个*有限*子集$J$，我们将$G$的元素$s_J = \sum_{i \in J} x_i$关联起来，我们称之为族的*有限部分和*$(x_i)_{i \in I}$、相应的到集合 $J$。如果$\mathfrak{F}(I)$表示$I$的有限子集*的*集合，那么我们就有$\mathfrak{F}(I)$的映射$J \to s_J$到$G$。现在$\mathfrak{F}(I)$是一个关于关系$\subset$的*定向*集合；因为如果$J$和$J'$是$\mathfrak{F}(I)$的两个元素，那么$J \subset J \cup J'$和$J' \subset J \cup J'$，并且$J \cup J'$是$I$的有限子集。令$\Phi$为有向集合$\mathfrak{F}(I)$（章I, § 6, no. 3）的*截面过滤器*。

#### 定义 1 {#top-iii-s5-def-1 .statement tag=0BMB}

设$(x_i)_{i \in I}$是Hausdorff交换律群$G$的点族；令$\mathfrak{F}(I)$为指标集合$I$有限子集集合，并且对于$I$的每个有限子集$J$，令$s_J$为其中的和 $x_i$使得$i \in J$。如果映射$J \to s_J$对于关系$\subset$定向的集合$\mathfrak{F}(I)$的截面过滤器$\Phi$有极限，则称族$(x_i)_{i \in I}$是可求和的；然后，这个极限被称为$(x_i)_{i \in I}$家族的和，并用$\sum_{i \in I} x_i$表示（或者简称为$\sum_i x_i$，甚至$\sum x_i$，当没有歧义的风险时）。

定义 1 等价于： *family* $(x_i)$ *可求和，其和为* $s$ *如果，对于每个邻域* $V$ *原点在* $G$，*有有限子集* $J_0$*of*$I$*这样对于每个有限子集*$J \supset J_0$*of*$I$*我们有*$s_J \in s + V$。

如果$G$被写成“乘法”，并且如果我们为$I$的每个有限子集$J$放置$p_J = \prod_{i \in J} x_i$，则如果映射$J \to p_J$相对于过滤器具有极限，则$(x_i)$族将被称为“可乘” $\Phi$；这个极限称为$(x_i)$家族的*乘积*，用$\prod_{i \in I} x_i$表示。

#### 注 1 {#top-iii-s5-n1-rem-1 .statement tag=0BMC}

当$I$是*有限*时，定义1约化到有限族的和的普通定义。更一般地，如果 $I$ 是任意的，并且 $x_i = 0$ 除外，当指标 $i$ 属于到 $I$ 的*有限* 子集 $J$ 时，则和 $\sum_{i \in I} x_i$ 等于$\sum_{i \in J} x_i$。

#### 注 2 {#top-iii-s5-n1-rem-2 .statement tag=0BMD}

可求和族的定义不涉及指标集合$I$的任何*排序*，因此我们可以说由此定义的和的概念是*可交换的*。更准确地说，我们有以下性质：令$(x_i)_{i \in I}$为可求和族，并令$\varphi$为指标集合$K$到集合$I$的双射映射；那么如果我们放入 $y_x = x_{\varphi(x)}$，则族 $(y_x)_{x \in K}$ 是可求和的并且具有与 $(x_i)$ 相同的和。因为如果$s = \sum_{i \in I} x_i$，并且如果每个有限子集$J$包含有限子集$J_0$都有$\sum_{i \in J} x_i \in s + V$，那么对于$K$的每个有限子集$L$我们将有$\sum_{x \in L} y_x \in s + V$ 包含$\overline{\varphi}(J_0)$。

#### 注 3 {#top-iii-s5-n1-rem-3 .statement tag=0BME}

更一般地，定义 1 适用于 *Hausdorff 拓扑空间* $X$ 中的点的每个族，其上已定义了合成* 的*结合和交换律，可加法书写；因为它没有利用拓扑群的公理。

### 2. 柯西准则

设$(x_i)_{i \in I}$是$G$中的可求和族。那么对于$G$中原点的每个邻域$V$，$I$都有有限子集$J_0$，这样，对于$I$的每个有限子集$K$*不满足*$J_0$，我们有$s_K \in V$。因为 $J = J_0 \cup K$ 是任意有限子集包含 $J_0$；令 $s = \sum_{i \in J} x_i$ 且令 $W$ 为 $o$ 的对称邻域，使得 $W + W \subset V$；那么，到定义 1，我们可以选择$J_0$，这样$s_J \in s + W$和$s_{J_0} \in S + W$，这意味着$s_K = s_J - s_{J_0} \in W + W \subset V$。

相反，假设家庭$(x_i)$有这个性质。那么滤波器$\Phi$的像，在映射$J \to s_J$下，是$G$中的*柯西滤波器基*。因为如果$J$是有限子集包含$J_0$，并且如果$K$表示$J \cap C J_0$，那么$K \cap J_0 = \varnothing$和$s_K = s_J - s_{J_0}$，所以$s_J \in s_{J_0} + V$。如果 $J'$ 是另一个有限子集包含 $J_0$，则$s_J - s_{J'} \in V + V$，结果如下。因而：

#### 定理 1（柯西准则）{#top-iii-s5-thm-1 .statement tag=0BMF}

*在 Hausdorff 交换律群* $G$ 中，*在阶中，一个家庭* $(x_i)_{i \in I}$ *应该是可求和的，对于每个邻域* $V$ *原点在* $G$，*有有限子集* $J_0$ *of* $I$ *使得* $\sum_{i \in K} x_i \in V$ *对于所有有限子集* $K$ *of* $I$ *不满足* $J_0$。 *如果* $G$ *完整*，则这个必要的条件也足够了。

因而，通过从$(x_i)$家族中去掉项的（足够大）有限数，幸存亚家族的每个*有限部分和*必须*接近*$o$*如我们所愿*。

定理 1 的第一个部分的直接的推论是以下命题：

#### 命题 1 {#top-iii-s5-prop-1 .statement tag=0BMG}

*如果族* $(x_i)$ *是可求和的，那么* $o$ *包含的每个邻域所有* $x_i$ *除了有限子族*（在其他字中，如果$I$是无限的，我们对于补集过滤器有$\lim x_i = o$ 有限子集*$I$）。

对于一个家庭$(x_i)$来说，这个*必要的*条件一般来说是*远远不够的*，即使$G$是完整的；稍后我们会看到很多例（参见章IV, § 7）。

#### 推论 {#top-iii-s5-n2-cor-1 .statement tag=0BMH}

*设* $(x_i)_{i \in I}$ *是可交换族群，其单位元素具有邻域的可数基数系统。那么指标* $i$ *的集合 *使得* $x_i \neq o$ *是可数的*。

令 $(V_n)$ 为邻域 $o$ 的可数基本系统。如果$H_n$是所有指标$i$中的集合，使得$x_i \notin V_n$，则指标$i$中的集合$H$使得$x_i \neq o$是并集合 $H_n$，并且每个 $H_n$ 都是由命题 1 *有限*的。

如果我们不假设原点具有可数基数系统邻域，则这个推论不再必然有效。 \* 例如，考虑乘积群 $\mathbf{R}^\mathbf{R}$ [实变量的所有有限实值函数的加法群，其中拓扑逐点收敛 (cf. 章 X, , no. 3)]，并令$f_a$为$\mathbf{R}$的元素，使得$f_a(a) = 1$和$f_a(x) = 0$，如果$x \neq a$；那么$(f_a)_{a \in \mathbf{R}}$是可求和的，它的和是函数，其值在$\mathbf{R}$的每个点处都是1。\*

#### 注 {#top-iii-s5-n2-rem-1 .statement tag=0BMI}

当 G 被写成乘法时，柯西准则采用以下形式 ：为了使族 $(x_i)_{i \in I}$ 可乘，必须对于单位元素的每个邻域 V，都应该存在 I 的有限子集 $J_0$，使得对于每个I的有限子集 K 不满足$J_0$，有$\prod_{i \in K} x_i \in V$；只要 G 是完备的，这个条件就足够了。我们推断，如果I是无限的并且$(x_i)$是可乘的，那么$\lim x_i = 1$相对于I的有限子集的补集过滤器；如果加法单位元素中的可数基数系统为邻域，则集合为指标 i，使得 $x_i \neq 1$ 是可数的。

### 3. 部分和； 结合性

#### 命题 2 {#top-iii-s5-prop-2 .statement tag=0BMJ}

在完整的群 G 中，可求和族的每个子族都是可求和的。

因为如果一个族$(x_i)_{i \in I}$满足柯西准则，那么每个亚族都满足它。

如果$(x_i)_{i \in I}$是可求和的，则和$\sum_{i \in J} x_i$是为I的每个子集J定义的，无论是否有限：它再次被称为族$(x_i)$、相应的到子集J的部分和指标集合。可求和族的分部和的集合显然包含在有限分部和的闭包集合中。

#### 定理 2（结合性 / 和）{#top-iii-s5-thm-2 .statement tag=0BMK}

令$(x_i)_{i \in I}$为完整群G中的可求族，并令$(I_\lambda)_{\lambda \in L}$为I中的任意划分。如果 $s_\lambda$ 表示 $\sum_{i \in I_\lambda} x_i$，则族 $(s_\lambda)_{\lambda \in L}$ 可求和，并且与族 $(x_i)_{i \in I}$ 具有相同的和。

因此，如果我们在完整的群中有一个可求和族，我们可以将其项任意关联到子族中，并由此获得每个子族的形式和；这些部分和的族再次可求和，并且其和等于给定族的族。

令$s = \sum_{i \in I} x_i$，并令$V$是$G$中任何0的*封闭*邻域。然后有$I$的有限子集$J_0$，这样，对于$I$的每个有限子集$J$，其中包含$J_0$，我们有$\sum_{i \in J} x_i \in s + V$。令 $K_0$ 为 $L$ 由……组成或指标 $\lambda$ 的子集，使得 $J_\lambda = I_\lambda \cap J_0$ *不为空*：$K_0$ 显然是有限的。令$K$为$L$中的任意有限子集，其中包含$K_0$；我们将证明$\sum_{\lambda \in K} s_\lambda \in s + V$，这将建立定理。

现在$s_\lambda$非常接近$(x_i)$的有限部分和，其指标全部为属于到$I_\lambda$；更准确地说，给定 0 的任何对称邻域 $W$，对于 $I_\lambda$ 的每个 $\lambda \in K$ 有限子集 $H_\lambda$，*包含于* $J_\lambda$ 都存在$s_\lambda - \sum_{i \in H_\lambda} x_i \in W$。让$J = \sum_{\lambda \in K} H_\lambda$；那么$J$是$I$包含于$J_0$的有限子集，我们有

$$
\sum_{i \in J} x_i = \sum_{i \in \bigcup_{\lambda \in K} H_\lambda} x_i = \sum_{\lambda \in K} (\sum_{i \in H_\lambda} x_i)
$$

乘以有限和的结合性。因此，根据$J_0$和$H_\lambda$的选择，我们有

$$
\sum_{\lambda \in K} s_\lambda \in s + V + nW
$$

其中$n$是$K$中元素的数；这个关系对于每个$W$成立，因此也适用于$\sum_{\lambda \in K} s_\lambda \in s + V$，因为$V$（正在关闭）是邻域$V + nW$的交[§ 3, no. 1，公式（1）]。

因此，我们可以将和写为 *结合性公式*：

(I)

$$
\sum_{\lambda \in L} (\sum_{i \in I_\lambda} x_i) = \sum_{i \in \bigcup_{\lambda \in L} I_\lambda} x_i,
$$

只要族 $(I_\lambda)$ 是其并的 *划分* 并且定义了右侧，它就有效。特别地，如果指标集合是*乘积*$I = L \times M$，并且如果“双”族$(x_{\lambda \mu})_{(\lambda, \mu) \in L \times M}$是*可求和的*，我们就有阶的变换的求和*公式*

(2)

$$
\sum_{(\lambda, \mu) \in L \times M} x_{\lambda \mu} = \sum_{\lambda \in L} (\sum_{\mu \in M} x_{\lambda \mu}) = \sum_{\mu \in M} (\sum_{\lambda \in L} x_{\lambda \mu}).
$$

应该注意的是，(1) 的*左侧*可以具有含义，而无需定义右侧。例如，考虑$I = LX \{1, 2\}$和$L$是无限的情况，$I_\lambda$由两个元素、$(\lambda, 1)$和$(\lambda, 2)$组成；如果我们采用$x_{\lambda, 1} = a,\ x_{\lambda, 2} = -a$，其中$a$是$G$的任何非零元素，那么$I_\lambda$的所有部分和相应的都是零，因此（1）的左侧被定义并等于0，而（1）的右侧没有任何意义，如命题 1 所示。

同样，(2) 的左边可能没有定义，但 (2) 中的两个“双和”都有一个含义；它们所代表的$G$的元素不必相等（参见章IV, § 7、习题17）。

因此，虽然总是可以“关联”和的项，但另一方面，不可能将和的项“分离”到它们的元素中，这些项本身表现为和。然而，只要这些“可分离的”项中的数是有限的，这个运算就是合法的。

#### 命题 3 {#top-iii-s5-prop-3 .statement tag=0BML}

令$(x_i)_{i \in I}$为群$G$的点族，令$(I_\lambda)_{\lambda \in L}$为$I$的有限划分。如果每个子族 $(x_i)_{i \in I_\lambda}$ 可求和，则族 $(x_i)_{i \in I}$ 可求和，并且公式 (1) 有效。

当$L = (1,2)$时证明命题就足够了；完成此操作后，我们将在 $L$ 的元素的数上经过归纳。设$s_1 = \sum_{i \in I_1} x_i$和$s_2 = \sum_{i \in I_2} x_i$。对于原点的每个邻域 $V$，有 $I_1$（或 $I_2$）的有限子集 $J_1$（或$J_2$），这样，对于每个有限子集 $H_1$（或$H_2$） $I_1$（分别$I_2$）包含$J_1$（分别$J_2$），我们有$\sum_{i \in H_1} x_i \in S_1 + V$（分别$\sum_{i \in H_2} x_i \in s_2 + V$）。如果我们输入$J_0 = J_1 \cup J_2$，则对于$I$中的每个有限子集$H$（其中包含$J_0$），我们有$\sum_{i \in H} x_i \in S_1 + s_2 + V + V$，结果如下。

### 4. 群乘积中的可求和族

#### 命题 4 {#top-iii-s5-prop-4 .statement tag=0BMM}

令 $G = \prod_{\lambda \in L} G_\lambda$ 为 Hausdorff 交换族群的乘积。那么$G$的点的族$(x_i)_{i \in I}$是可求和的当且仅当对于每个$\lambda \in L$，族$(\mathrm{pr}_\lambda x_i)_{i \in I}$是可求和的；如果$s_\lambda$是这个家族的和，那么$s = (s_\lambda)$就是$(x_i)$家族的和。

这紧随条件的收敛，相对于函数的滤波器，它在乘积空间中取其值（章I, § 1, no. 6，推论1到命题10）；实际上，对于 $I$ 的每个有限子集 $J$，我们有

$$
\mathrm{pr}_\lambda \left( \sum_{i \in J} x_i \right) = \sum_{i \in J} \mathrm{pr}_\lambda x_i.
$$

### 5. 连续同态下可求和族的像

#### 命题 5 {#top-iii-s5-prop-5 .statement tag=0BMN}

令 $f$ 为交换律群 $G$ 到交换律群 $G'$ 的连续同态。如果$(x_i)$是$G$中的可求和族，则$(f(x_i))$是$G'$中的可求和族，并且我们有

$$
\Sigma f(x_i) = f(\Sigma x_i).
$$

如果$J$是索引集的任意有限子集，则$f \left( \sum_{i \in J} x_i \right) = \sum_{i \in J} f(x_i)$，并且收敛滤波器基的$f$下的图像是收敛滤波器基（第I, § 7, no. 4章，推论1到命题9）。

#### 命题 6 {#top-iii-s5-prop-6 .statement tag=0BMO}

令 $(x_i), (y_i)$ 为两个可求和族，在群 $G$ 中具有相同的指标集合。那么族 $(-x_i), (nx_i)$ ($n \in \mathbf{Z}$), $(x_i + y_i)$ 是可求和的，我们有

$$
\begin{align*}
\Sigma(-x_i) &= -\Sigma x_i, \\
\Sigma(nx_i) &= n\Sigma x_i, \\
\Sigma(x_i + y_i) &= \Sigma x_i + \Sigma y_i.
\end{align*}
$$

对于$x \to -x$和$x \to nx$来说，$G$的同态连续到$G$；另一方面，如果$(x_i)$和$(y_i)$可求和，那么$(x_i, y_i)$族在$G \times G$中可求和，并且由于$(x, y) \to x + y$是$G \times G$到$G$的连续同态，我们推导出(6)。

#### 注 {#top-iii-s5-n5-rem-1 .statement tag=0BMP}

命题 4 和 5 再次适用于前面提到的拓扑空间 $X$ 中的可求和族的情况，其具有合成的结合律和交换律律；如果我们假设在加法中$x + y$在$X \times X$上连续，则同样适用于命题 3和公式 (6)。

### 6. 级数

考虑 Hausdorff 交换式群中点 $(x_n)_{n \in \mathbf{N}}$ 的序列，以及 *部分和* $s_n = \sum_{p=0}^n x_p$ ($n \in \mathbf{N}$) 的形式序列。 映射$(x_n) \to (s_n)$是$G$的点序列$(x_n)$的集合$G^\mathbf{N}$的*双射*，在其自身上；因为如果给定序列 $(s_n)$，序列 $(x_n)$ 由关系 $x_0 = s_0, x_n = s_n - s_{n-1}$ ($n \geq 1$) 确定。

由序列* $(x_n)$ 定义的 *级数，或一般项* 为 $x_n$ 的 *级数 [或简单地称为 *级数* $(x_n)$]，通过滥用语言，如果没有混淆的风险]被定义为 *右* 序列$(x_n)$和$(s_n)$因此相关联。如果序列 $(s_n)$ 收敛，则由序列 $(x_n)$ 定义的级数被称为“收敛”；这个序列的极限称为级数*的*和，写成$\sum_{n=0}^\infty x_n$（或$\sum_{n=0}^\infty x_n$，滥用记号）。

如果级数（其通项为$x_n$）*收敛*，我们将有时允许自己滥用语言，将其称为“级数$\sum_{n=0}^\infty x_n$”或“级数$x_0 + x_1 + \cdots + x_n + \cdots$”。

级数收敛的*必要*条件（其一般项为$x_n$）是序列$(s_n)$应该是*柯西序列*，也就是说，对于原点的每个邻域$V$ $G$ 存在整数 $n_0$，因此对于整数 $n \geq n_0,\ p > 0$ 中的每一个对，我们有
$$
s_{n+p} - s_n = \sum_{i=n+1}^{n+p} x_i \in V.
$$
如果$G$是*完整的*，那么这个条件也是*充分的*（*柯西的级数标准*）。

如果级数（其通项为$x_n$）收敛，则我们特有$\lim_{n \to \infty} (s_n - s_{n-1}) = \lim_{n \to \infty} x_n = 0$；但是，即使 $G$ 是完整的（参见章 IV, § 7），收敛所需的条件一般情况下也远远不够。

#### 命题 7 {#top-iii-s5-prop-7 .statement tag=0BMQ}

*如果由序列* $(x_n)$ *和* $(y_n)$ *定义的级数收敛，那么由序列* $(-x_n)$ *和* $(x_n + y_n)$定义的级数也收敛，*我们有*
(7)
$$
\sum_{n=0}^\infty (-x_n) = -\sum_{n=0}^\infty x_n,
$$
(8)
$$
\sum_{n=0}^\infty (x_n + y_n) = \sum_{n=0}^\infty x_n + \sum_{n=0}^\infty y_n.
$$
这是$-x$在$G$上的连续性和$x + y$在$G \times G$上的连续性的明显推论。

#### 推论 {#top-iii-s5-n6-cor-1 .statement tag=0BMR}

*如果*$(x_n), (y_n)$*是*$G$*的点的两个序列，使得*$x_n = y_n$*除了指标的有限数，并且如果级数其一般项是*$x_n$ *收敛，那么级数也收敛，其通式项是*$y_n$。

对于级数，其总项为$x_n - y_n$，从某个指标开始，具有所有项零。

这个推论可以放入形式中，*我们可以任意改变收敛级数的项的有限数，而不会停止收敛*。
特别是，如果$y_n = 0$对于$n < m$，$y_n = x_n$对于$n \geq m$，我们看到，其一般项为$y_n$的级数收敛，当且仅当其一般项为$x_n$的级数收敛；其和记为$\sum_{n=m}^{\infty} x_n$，称为级数$(x_n)$的指标$m$的*剩余类*。自从
$$
\sum_{n=m}^{\infty} x_n = \sum_{n=0}^{\infty} x_n - s_{m-1},
$$
收敛级数的指标$m$的剩余类*趋向于*0，因为$m$趋向于$+\infty$。

如果序列 $(x_n)_{n \in I}$ 具有指标集合 $\mathbf{N}$ 的无限子集 $I$，并且如果 $\varphi$ 表示$\mathbf{N}$ 的*严格保序* 双射到$I$，那么序列$(x_{\varphi(n)})_{n \in \mathbf{N}}$定义的级数就被滥用语言，称为序列$(x_n)_{n \in I}$定义的*级数*；如果这个级数收敛，则它的和记为$\sum_{n \in I}^{\infty} x_n$。立即验证，当且仅当一般项为 $(z_n)$ 的级数收敛时，级数才收敛，其中，如果$n \in I$则为$z_n = x_n$，如果$n \in \mathbf{C} I$则为$z_n = 0$。

值得注意的是，如果由序列 $(x_n)_{n \in \mathbf{N}}$ 定义的级数收敛，则可能存在 $\mathbf{N}$ 的无限子集 $I$，使得由子序列 $(x_n)_{n \in I}$ 定义的级数 *不收敛*（参见习题 5 和章 IV, § 7）。

命题 4 和 5 扩展立即到级数，我们将在这种情况下的公式留给读者。

#### 命题 8（限制结合性 / 级数）{#top-iii-s5-prop-8 .statement tag=0BMS}

*设*$(k_n)$*为严格递增的序列/整数*$\geqslant 0$。 *如果级数的一般项是* $x_n$ *收敛，如果我们把* $u_n = \sum_{p=k_{n-1}}^{k_n-1} x_p$，*那么级数的一般项是* $u_n$ *收敛，我们有* $\sum_{n=0}^{\infty} u_n = \sum_{n=0}^{\infty} x_n$。

对于级数$(u_n)$的部分和的序列来说，是级数$(x_n)$的部分和的序列$(s_n)$的*子序列*$(s_{k_n-1})$。

### 7. 交换收敛级数

令$(x_n)$为$G$中的*可求和*序列，并令$s = \sum_{n \in \mathbf{N}} x_n$为其和。那么对于每个 0 的邻域 $V$，都存在 $J_0 \in \mathfrak{F}(\mathbf{N})$，使得每当 $J \in \mathfrak{F}(\mathbf{N})$ 和 $J_0 \subset J$ 时就有 $s_J \in s + V$。令$J_0$中的$m$为最大的整数；那么如果 $n \geqslant m$ 我们有 $s_n \in s + V$，因此 *级数* $(x_n)$ 是收敛的，并且它的和是 $s$。但逆命题是*假*：

收敛级数的项的序列很可能无法求和（参见章 IV，）

此外，收敛级数的定义本质上涉及$\mathbf{N}$的阶结构。如果级数$(x_n)$收敛，并且$\sigma$是$\mathbf{N}$的置换，则级数$(x_{\sigma(n)})$不一定收敛（cf.章IV, § 7，习题） 15）。

#### 定义 2 {#top-iii-s5-def-2 .statement tag=0BMT}

*由序列* $(x_n)$ *定义的级数 *被认为是可交换收敛的，如果对于* $\mathbf{N}$的每个置换* $\sigma$ *，由序列* $(x_{\varphi(n)})$ *定义的级数是收敛的。*

#### 命题 9 {#top-iii-s5-prop-9 .statement tag=0BMU}

*由序列* $(x_n)$ *定义的级数 *可交换收敛当且仅当序列* $(x_n)$ *可求和；然后，对于每个置换* $\sigma$ *of* $\mathbf{N}$，*我们有*

$$
\sum_{n=0}^{\infty} x_{\sigma} = \sum_{n \in \mathbf{N}} x_n.
$$

如果序列可求和，那么显然级数是可交换收敛的。为了证明相反的含义，我们将通过*归谬法*进行论证，并假设级数 $(x_n)$ 是交换收敛的，但序列 $(x_n)$ 不可求和。滤波器$\Phi$在映射$H \to s_H$下的像因此不能是$G$中的柯西滤波器基，否则该滤波器基将收敛，因为到假设它有一个集群点（章II, § 3, no. 2、命题5、推论2）。因此，$G$中存在0的邻域$V$，这样，对于$\mathbf{N}$的每个有限子集$J$，$\mathbf{N}$中存在有限子集$H$，不满足$J$，因此那个$\sum_{n \in H} x_n \notin V$。因此，通过归纳，我们可以将$\mathbf{N}$的定义划分转化为*有限*子集$H_k$（$k \in \mathbf{N}$），使得$\sum_{n \in H_k} x_n \notin V$对于指标的无限数 $k$。显然，$\mathbf{N}$有置换$\sigma$，因此对于每个$k$，$n$的值其中$\sigma(n) \in H_k$是连续的。如果$\sigma$是这样的置换，那么级数其通项是$x_{\sigma(n)}$不能收敛，我们就有矛盾了。

如果群$G$被写成*乘法*，则由$G$的点的序列* $(x_n)$定义的*无限乘积（或*无限乘积，其通式项为* $x_n$，甚至 *乘积* $x_n$（如果不存在混淆的可能性）被定义为由序列 $(x_n)$ 和部分积的序列组成的对

$$
p_n = \prod_{k=0}^{n} x_k.
$$

如果序列 $(p_n)$ 收敛，则无限的乘积被称为“收敛”，并且该序列的极限由 $\prod_{n=0}^{\infty} x_n$ 表示（或通过滥用记号表示 $\prod_{n=0}^{\infty} x_n$）。我们留给读者的任务是将我们已经建立的级数的属性转录成乘法记号。

### 习题 {#top-iii-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
