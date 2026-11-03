---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 8
section_title: Hausdorff spaces and regular spaces
lang: zh
source: top-i-iv
book_pages: 75-83, 134-141
pdf_pages: 0081-0089, 0140-0147
extraction: ocr
subsections:
    - "no": 1
      title: HAUSDORFF SPACES
      page: 75
      pdf_page: 81
    - "no": 2
      title: SUBSPACES AND PRODUCTS OF HAUSDORFF SPACES
      page: 77
      pdf_page: 83
    - "no": 3
      title: HAUSDORFF QUOTIENT SPACES
      page: 78
      pdf_page: 84
    - "no": 4
      title: REGULAR SPACES
      page: 80
      pdf_page: 86
    - "no": 5
      title: EXTENSION BY CONTINUITY; DOUBLE LIMIT
      page: 81
      pdf_page: 87
    - "no": 6
      title: EQUIVALENCE RELATIONS ON A REGULAR SPACE
      page: 82
      pdf_page: 88
statements: 30
exercises: 29
content_sha256: f29d623a107167ff3e68f8ec7201a949a0c33dfcf7f8e68c8cb363d4334b9256
translated_from: content/en/top/I/08_s8_hausdorff_spaces_and_regular_spaces.md
translation_method: google
source_content_sha256: daafa83709f77ca8c5f24c854acb749ef62cc4f8fd95a86660a5a0aa731a2fec
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 7fb80677d38f3ff49835dadeb9cce34e9e0d84d2318c6144f8d5b90f676f576c
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 8. Hausdorff 空间和常规空间

### 1. 豪斯多夫空间

#### 命题 1 {#top-i-s8-prop-1 .statement tag=0B65}

设$X$为拓扑空间。那么下面的叙述是等价的：

(H) $X$ 中任意两个不同的点都有不相交的邻域。
（嗨）$X$的任何点的封闭邻域的交仅由点组成。
(嗨)乘积空间$X \times X$的对角线是闭集合。
(Hiii) 对于每个集合 $I$，乘积空间 $Y = X^I$ 的对角线在 $Y$ 内闭合。
(HIV) $X$ 上没有一个过滤器具有多个极限点。
(Hv) 如果$X$上的过滤器$\mathfrak{F}$收敛到$x$，则$x$是$\mathfrak{F}$的唯一簇点。

我们将证明其含义

$$
\begin{array}{cccccc}
(H) & \Longrightarrow & (Hi) & \Longrightarrow & (Hv) & \Longrightarrow (Hiv) \Longrightarrow (H)
\\
(H) & \Longrightarrow & (Hiii) & \Longrightarrow & (Hii) & \Longrightarrow (H).
\end{array}
$$

和

(H) $\Longrightarrow$ (Hi)：如果$x \neq y$存在$x$的开路邻域$U$和$y$的开路邻域$V$，使得$U \cap V = \varnothing$；因此$y \notin \overline{U}$。

（嗨）$\Longrightarrow$（Hv）：设$y \neq x$；那么存在$x$的闭邻域$V$使得$y \notin V$，并且到假设存在$M \in \mathfrak{F}$使得$M \subset V$；因此$M \cap C_V = \varnothing$。但$C_V$是$y$的邻域；因此$y$不是$\mathfrak{F}$的簇点。

(Hv) $\Longrightarrow$ (Hiv)：清楚，因为过滤器的每个极限点也是一个簇点。

(Hiv) $\Longrightarrow$ (H)：假设 $x \neq y$ 并且 $x$ 中的每一个邻域 $V$ 都满足 $y$ 中的每一个邻域 $W$。那么同时具有$x$和$y$的滤波器的集合$V \cap W$形式基为极限点，这与假设相反。

(H) $\Longrightarrow$ (Hiii)：设$(x) = (x_i)$为$X^I$的点，它不属于到对角线$\Delta$。那么至少有两个指标$\lambda, \mu$使得$x_\lambda \neq x_\mu$。令$V_\lambda$（或$V_\mu$）为$X$中$x_\lambda$（或$x_\mu$）的邻域，使得$V_\lambda \cap V_\mu = \varnothing$；那么集合 $W = V_\lambda \times V_\mu \times \prod_{i \neq \lambda, \mu} X_i$（其中 $X_i = X$ 如果 $i \neq \lambda, \mu$）是 $X^I$ (§ 4, no. 1) 中 $x$ 的邻域，且不满足 $\Delta$。因此$\Delta$于$X^I$关闭。

(Hiii) $\Longrightarrow$ (Hii)：显而易见。

(Hii) $\Longrightarrow$ (H): 如果$x \neq y$则$(x, y) \in X \times X$不在对角线$\Delta$中，因此(§ 4, no. 1)存在$x$的邻域$V$和邻域$W$ $y$ in $X$ 使得$(V \times W) \cap \Delta = \varnothing$，这意味着
$$
V \cap W = \varnothing.
$$

#### 定义 1 {#top-i-s8-def-1 .statement tag=0B66}

* 命题 1 的拓扑空间满足条件称为 Hausdorff 或分离空间；这样的空间中的拓扑据说是豪斯多夫拓扑。*

公理 (H) 是*豪斯多夫公理*。

#### 例 {#top-i-s8-n1-exa-1 .statement tag=0B67}

任何离散空间都是 Hausdorff。有理线$Q$是Hausdorff，因为如果$x, y$是两个有理数数，使得$x < y$，则存在有理数$z$，使得$x < z < y$和邻域]$\leftarrow, z[$等于$x$与 $y$ 的 ]$z, \rightarrow[$ 不相交。

集合 $X$ 至少有两个点并带有最粗糙的拓扑 (§ 2, no. 2) 不是 Hausdorff 空间。

令 $f : X \to Y$ 为集合 $X$ 的映射变为 *Hausdorff* 空间 $Y$；那么从命题 1 可以立即得出，相对于 $X$ 上的过滤器 $\mathfrak{F}$，$f$ 最多可以有一个极限*，并且如果 $f$ 相对于 $\mathfrak{F}$ 具有 $y$ 和极限一样，那么$y$ *仅是$f$相对于$\mathfrak{F}$的集群点*。

#### 命题 2 {#top-i-s8-prop-2 .statement tag=0B68}

*令$f, g$为拓扑空间$X$的两个连续的映射变为豪斯多夫空间$Y$；那么所有$x \in X$中的集合使得$f(x) = g(x)$在$X$中闭合。*

对于这个集合是$Y \times Y$在映射$x \mapsto (f(x), g(x))$下的对角线的逆像，它是连续的（§ 4, no. 1，命题1）。因此，结果由 (Hii) 和§ 2, no. 1、定理 1 得出。

#### 推论 1（扩张个身份中的原理）{#top-i-s8-prop-2-cor-1 .statement tag=0B69}

*设$f, g$是拓扑空间$X$到Hausdorff空间$Y$的两个连续的映射。如果 $f(x) = g(x)$ 是 $X$ 的密集子集的点，则 $f = g$。*

在其他字中，$X$的连续映射进入$Y$（Hausdorff）由其值在点的密集子集唯一确定$X$。

#### 推论 2 {#top-i-s8-prop-2-cor-2 .statement tag=0B6A}

*如果$f$是拓扑空间$X$到Hausdorff空间$Y$的连续映射，则$f$的图在$X \times Y$中闭合。*

对于该图，是所有 $(x, y) \in X \times Y$ 中的集合使得 $f(x) = y$，并且两个映射 $(x, y) \to y$ 和 $(x, y) \to f(x)$ 是连续的。

#### 命题 3 {#top-i-s8-prop-3 .statement tag=0B6B}

*令 $(x_i)_{1 \leq i \leq n}$ 为 Hausdorff 空间 $X$ 的不同点的有限族；那么每个$x_i$在$X$中有邻域$V_i$，使得$V_i$（$1 \leq i \leq n$）互为不相交的。*

证明在 $n$ 上乘以归纳：情况 $n = 2$ 只是公理 (H)。设$W_i$ ($1 \leq i \leq n - 1$) 为$x_i$ 的邻域，使得$W_i$ 互为不相交的。另一方面，对于$1 \leq i \leq n - 1$，$x_i$有邻域$T_i$和$x_n$有邻域$U_i$不相交。如果我们将 $1 \leq i \leq n - 1$ 的$V_i$ 变为 $W_i \cap T_i$ 并且
$$
V_n = \bigcap_{i=1}^{n-1} U_i,
$$
命题中的条件满意。

#### 推论 {#top-i-s8-n1-cor-1 .statement tag=0B6C}

*每个有限 Hausdorff 空间都是离散的。*

#### 命题 4 {#top-i-s8-prop-4 .statement tag=0B6D}

*Hausdorff 空间的每个有限子集都关闭。*

对于单个点的每个子集由……组成由于公理 (H\textsuperscript{i}) 是封闭的。

#### 命题 5 {#top-i-s8-prop-5 .statement tag=0B6E}

*令$X$为拓扑空间，并假设对于$X$的不同点$x, y$的每个对，都有一个连续的$X$的映射$f$进入Hausdorff 空间$X'$使得$f(x) \neq f(y)$。那么 $X$ 就是 Hausdorff。*

令$V'$和$W'$分别为$X'$中$f(x)$和$f(y)$的不相交的和邻域；那么$\overline{f}^{-1}(V')$和$\overline{f}^{-1}(W')$分别是$X$中$x$和$y$的不相交的邻域。

#### 推论 {#top-i-s8-n1-cor-2 .statement tag=0B6F}

*每个拓扑比 Hausdorff 拓扑更细都是 Hausdorff。*

### 2. hausdorff 的子空间和乘积空间

*Hausdorff 空间 $X$ 的子空间 $A$ 是 Hausdorff*，正如我们通过 no. 1 到典范嵌入 $A \to X$ 的应用命题 5 看到的那样。相反，我们有

#### 命题 6 {#top-i-s8-prop-6 .statement tag=0B6G}

*如果拓扑空间$X$的每个点都有一个闭邻域，它是$X$的豪斯多夫子空间，则$X$是豪斯多夫。*

令 $x \in X$ 并令 $V$ 为 $x$ 在 $X$ 中的闭邻域，使得子空间 $V$ 为 Hausdorff。那么$V$中$x$的闭邻域有$\{x\}$作为它们的交（公理（H\textsuperscript{'}））；但它们在$X$ (§ 3, no. 1) 中也是闭$x$ 的邻域，因此$X$ 满足(H\textsuperscript{i})。

存在*非Hausdorff* 空间，其中每个点都有一个Hausdorff邻域（习题7）。

#### 命题 7 {#top-i-s8-prop-7 .statement tag=0B6H}

*Hausdorff 空间的每个乘积都是 Hausdorff。相反，如果非空空间的乘积是 Hausdorff，则每个因子都是 Hausdorff 空间。*

设$X = \prod_{i \in I} X_i$为拓扑空间的乘积。那么，如果$x, y$是$X$的两个不同的点，对于某些指标$i$，我们有$\operatorname{pr}_i x \neq \operatorname{pr}_i y$，并且no. 1的命题5表明，如果$X_i$是，则$X$是Hausdorff。相反，如果 $X$ 是 Hausdorff 并且 $X_i$ 非空，则每个 $X_i$ 同胚于 $X$ 的子空间 (§ 4, no. 2，命题 4)，因此是 Hausdorff。

#### 推论 1 {#top-i-s8-prop-7-cor-1 .statement tag=0B6I}

*令$X$为集合，让$(Y_i)_{i \in I}$为Hausdorff拓扑族空间，对于每个$i \in I$，令$f_i$为$X$到$Y_i$的映射。让$X$携带最粗糙的拓扑$\mathfrak{T}$，其中$f_i$是连续的。那么，对于$X$成为Hausdorff的必要且充分的条件是，对于$X$的不同点$x, y$的每个对，对于某些指标$i \in I$，我们有$f_i(x) \neq f_i(y)$。*

由于 no. 1 中的命题 5，条件就足够了。相反，假设 $X$ 是 Hausdorff；令 $Y = \prod_{i \in I} Y_i$ 并令 $f = (f_i)_{i \in I}$ 为映射 $x \to (f_i(x))$。 $Y$以上的命题7为Hausdorff，§ 4, no. 1的命题3，$\mathfrak{T}$为$Y$的拓扑$f$下的逆像。如果 $f(x) = f(y)$ 对于 $X$ 的两个不同的点 $x, y$，很明显，每个开集合（在拓扑 $\mathfrak{T}$）其中包含 $x$ 也包含 $y$，与假设相反，$X$是Hausdorff。

#### 推论 2 {#top-i-s8-prop-7-cor-2 .statement tag=0B6J}

*令$(X_\alpha, f_{\alpha \beta})$为拓扑空间的逆系。如果 $X_\alpha$ 是 Hausdorff，则 $X = \varprojlim X_\alpha$ 是 Hausdorff，并且是 $\prod_\alpha X_\alpha$ 的闭子空间。

第一个断言源自$X$是Hausdorff空间$\prod_\alpha X_\alpha$（命题7）的子空间。为了证明 $X$ 在乘积空间内闭合，令 $F_{\alpha \beta}$ ($\alpha \leq \beta$) 为 $\prod_\alpha X_\alpha$ 由……组成的子集点 $x$，其中 $\operatorname{pr}_\alpha x = f_{\alpha \beta}(\operatorname{pr}_\beta x)$； $F_{\alpha \beta}$ 在$\prod_\alpha X_\alpha$（no. 1、命题 2）关闭，因此交 $X$ 也关闭。

显然，Hausdorff 空间 (§ 2, no. 4, 例 3) 的任何 *和* 都是 Hausdorff 空间。

### 3. 豪斯多夫商空间

让我们查找条件，其中商空间 $X/R$ 是 *Hausdorff*（在这种情况下，等价关系 $R$ 被称为 *Hausdorff*）。首先，如果 $X/R$ 是 Hausdorff，则单个点的 $X/R$ 由……组成的子集是*闭*（no. 1，命题 4），因此*每个等价类* mod $R$ *闭于* $X$。但这个必要的条件还不够。

$X/R$中的开集合的定义产生以下必要且充分的条件：当且仅当$X$中的任何两个不同的等价类包含在$X$的不相交的饱和开子集中时，$X/R$是Hausdorff。我们会给其他更有用的条件。

#### 命题 8 {#top-i-s8-prop-8 .statement tag=0B6K}

*商空间$X/R$成为Hausdorff的必要条件是$R$的图$C$在$X \times X$内闭。 如果等价关系$R$打开，这个条件也足够了。*

设$\varphi : X \to X/R$为典范映射；那么$C$是$(X/R) \times (X/R)$的对角线$\Delta$的$\varphi \times \varphi : X \times X \to (X/R) \times (X/R)$下的逆像。因此，命题的第一个部分源自$\varphi \times \varphi$的连续性[公理（Hii）和§ 2, no. 1的定理1]。如果$R$开路，则$(X/R) \times (X/R)$可被识别为商、空间、$(X \times X)/(R \times R)$（$§ 5$、no. 3、推论至命题8），然后$\Delta$可被识别为典范像集合$C$的$(X \times X)/(R \times R)$，相对于$R \times R$饱和。因此 $\Delta$ 在 $X \times X$ 中闭合，因此 $X$ 是 Hausdorff。

如果 $R$ 不开，则有例，其中 $C$ 闭，但 $R$ 不是 Hausdorff（习题 10 和 28）。

为了证明$X/R$是Hausdorff，我们还可以no. 1的应用命题5：$M$和$N$是$R$的两个不同的等价类，只要有一个开子集的连续映射$f$就足够了$X$的$A$，相对于$R$和包含$M$和$N$饱和，变成Hausdorff空间$X'$，使得1)$f$在每个等价类模上是恒定的$A$中包含$R$，2) $f$在$M$和$N$上取不同的值。因为$A/R_A$可以用$X/R$的开子集来识别（$§ 3$，no. 6，命题10，推论1），我们可以将no. 1中的应用命题5到映射 $g : A/R_A \to X'$ 由 $f$ 引发，因为 $g$ 是连续的 ($§ 3$、no. 4、命题 6)。

特别是：

#### 命题 9 {#top-i-s8-prop-9 .statement tag=0B6L}

*如果$f$是拓扑空间$X$到Hausdorff空间$X'$的连续映射，并且$R$是等价关系$f(x) = f(y)$，则商空间 $X/R$ 是豪斯多夫。*

#### 命题 10 {#top-i-s8-prop-10 .statement tag=0B6M}

*如果 $X$ 是 Hausdorff 空间，并且如果 $X$ 对于等价关系 $R$ 具有连续的截面 $s$，则 $X/R$ 是 Hausdorff 并且 $s(X/R)$ 是闭的$X$.*

对于 ($§ 3$, no. 5) $X/R$ 同胚于 $X$ 的子空间 $s(X/R)$，即 Hausdorff。此外，$s(X/R)$是所有$x \in X$中的集合，使得$s(\varphi(x)) = x$，其中$\varphi : X \to X/R$是典范映射；因此，第二个断言源自no. 1、命题2。

### 4. 常规空间

#### 命题 11 {#top-i-s8-prop-11 .statement tag=0B6N}

拓扑空间 $X$ 的以下属性是等效的：

(O_{III}) $X$的任意点的闭邻域的集合是点的邻域的基本系统。

(O'_{III}) 给定 $X$ 的任何闭子集 $F$ 和任何点 $x \notin F$，则存在 $x$ 的邻域和 $F$ 的邻域，它们不存在相交。

(O_{III}) \Longrightarrow(O'_{III})：如果$F$闭且$x \notin F$，则$x$的邻域$C_F$中包含$x$的闭邻域$V$； $V$和$C_V$分别是$x$和$F$的邻域，公共的中没有点。

(O'_{III}) \Longrightarrow (O_{III})：如果$W$是$x \in X$的开邻域，则存在$x$和邻域的邻域$U$ $C_W$中的$V$，即不相交的，因此$\overline{U} \subset W$。

#### 定义 2 {#top-i-s8-def-2 .statement tag=0B6O}

如果拓扑空间是 Hausdorff 并且满足公理 (O_{III})，则称其为正则；那么它的拓扑就被称为是规则的。

离散的空间是规则的。 \* 我们将在 § 9 中看到，每个局部紧致空间 （特别是实直线 $\mathbf{R}$）都是正则的。 \*

#### 命题 12 {#top-i-s8-prop-12 .statement tag=0B6P}

常规空间中的每一个子空间都是常规的。

令$A$为常规空间$X$的子空间。由于 $X$ 是 Hausdorff，所以 $A$ (no. 2) 也是如此；另一方面，点$x \in A$相对于$A$的每个邻域都是形式$V \cap A$，其中$V$是$X$中$x$的邻域。由于$X$是正则，$X$中有$x$的邻域$W$，它在$X$中闭合并包含在$V$中； $W \cap A$ 则为$A$ 中$x$ 的邻域，在$A$ 中闭合并包含在$V \cap A$ 中。于是就有了这样的结果。反之：

#### 命题 13 {#top-i-s8-prop-13 .statement tag=0B6Q}

如果拓扑空间$X$的每个点$x$都有一个闭邻域，并且它是$X$的正则子空间，则$X$是正则的。

$X$ 是 no. 2 的命题 6 的 Hausdorff。 令$x$为$X$的任意点，并令$V$为$x$的闭正则邻域。 如果$U$是$V$中包含的$x$中的任意一个邻域，则$U$是$x$相对于$V$的邻域；因此，到假设时，$V$中有$x$的邻域$W$，它在$V$中闭合并包含在$U$中。 但$W$是$X$中$x$的邻域，因为$V$是$X$中$x$的邻域，并且$W$在$X$中关闭，因为$V$在$X$中关闭。

#### 注 1 {#top-i-s8-n4-rem-1 .statement tag=0B6R}

存在非 Hausdorff 空间的例，其中每个点都有一个正则邻域 (习题 7)。

#### 注 2 {#top-i-s8-n4-rem-2 .statement tag=0B6S}

有空间是 Hausdorff 但不是正则 (习题 20)。

#### 注 3 {#top-i-s8-n4-rem-3 .statement tag=0B6T}

比常规拓扑更细的拓扑不必是常规的 (习题 20)。

### 5. 扩张连续性； 双极限

#### 定理 1 {#top-i-s8-thm-1 .statement tag=0B6U}

设X是拓扑空间，A是X的稠密子集，f：A→Y映射将A变成正则空间Y。对于f到扩展到连续映射的充分必要条件 $\overline{f} : X \to Y$ 是，对于每个 $x \in X$，当 y 趋于 x 而保持在 A 中时，$f(y)$ 趋向于 Y 中的极限。则 f 到 X 的连续扩张 $\overline{f}$ 是唯一的。

$\overline{f}$ 的唯一性源自恒等式扩张的原理（no. 1、命题 2、推论 1）。很明显，条件是必要的，因为如果$\overline{f}$在X上连续，那么对于每个$x \in X$我们有
$$
\overline{f}(x) = \lim_{y \to x, y \in A} \overline{f}(y) = \lim_{y \to x, y \in A} f(y)
$$
（§ 7, no. 5）。相反，假设满足条件且定义
$$
\overline{f}(x) = \lim_{y \to x, y \in A} f(y)
$$
对于每个$x \in X$； $\overline{f}(x)$ 是 Y 的明确定义的元素，因为 Y 是 Hausdorff。我们必须证明$\overline{f}$在每个点$x \in X$处都是连续的。设 V' 为 Y 中 $\overline{f}(x)$ 的闭邻域；那么到假设时，X中存在x的开邻域V，使得$f(V \cap A) \subset V'$。由于 V 是其每个点的邻域，因此我们有
$$
\overline{f}(z) = \lim_{y \to z, y \in V \cap A} f(y)
$$
对于每个$z \in V$，由此得出$\overline{f}(z) \in \overline{f}(V \cap A) \subset V'$，因为V'是封闭的。现在的结果是基于 Y 中 $f(x)$ 形式的封闭邻域是 $f(x)$ 的邻域的基本系统。

映射$\overline{f}$据说是通过将f连续性扩展到X而获得的。

在定理 1 假设的叙述中，Y 是正则不能被削弱，而不对 X、A 或 f (习题 19) 施加额外的限制。

#### 推论 {#top-i-s8-n5-cor-1 .statement tag=0B6V}

设$\mathfrak{F}_1$为集合$X_1$上的过滤器，$\mathfrak{F}_2$为集合$X_2$上的过滤器；令$\mathfrak{F}_1 \times \mathfrak{F}_2$为乘积在$X = X_1 \times X_2$上过滤（§ 6, no. 7），并令f为X的映射转换为常规空间Y。假设
a) $\lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f$ 存在。

b) $\lim_{x_2, \mathfrak{F}_2} f(x_1, x_2) = g(x_1)$ 对于所有 $x_1 \in X_1$ 都存在。

那么$\lim_{x_1, \mathfrak{F}_1} g(x_1)$存在并且等于$\lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f$。

令$X'_1 = X_1 \cup \{\omega_1\}$（或$X'_2 = X_2 \cup \{\omega_2\}$）为拓扑空间 *与过滤器相关联* $\mathfrak{F}_1$（或$\mathfrak{F}_2$）（§ 6, no. 5，例）。在乘积空间$X' = X'_1 \times X'_2$中，令$X''$为子空间$X_1 \times X'_2$和$\{(\omega_1, \omega_2)\}$中的并。 $X$显然是$X''$的稠密子空间，并且假设暗示当$(y_1, y_2)$趋向于$X''$的任何点$(x_1, x_2)$同时保持在$X$时，$f(y_1, y_2)$趋向于极限。 $f$ 的扩张通过连续到 $X''$ 可以从定理 1 得出。由于 $(\omega_1, \omega_2)$ 也位于 $X_1 \times \{\omega_2\}$ 相对于 $X''$ 的闭包中，因此结果立即得出（§ 7, no. 5）。

### 6. 等价关系常规空间

#### 命题 14 {#top-i-s8-prop-14 .statement tag=0B6W}

*让*$X$*成为常规空间*，$R$*于*$X$关闭等价关系。 *然后* $C$ *的* $R$ *在* $X \times X$ *中的图形是闭合的*。

令$(a, b)$为$C$闭包中$X \times X$的点，并令$V$（或$W$）为$a$的*封闭*邻域（或$b$的邻域）在$X$；然后是点$(x, y) \in C \cap (V \times W)$。从$x \in V$、$y$属于到$V$相对于$R$的饱和度$S$；因此，$b$中的每个邻域$W$都满足$S$。到假设 $S$ *关闭*，因此$b \in S$。现在令$B$为$\{b\}$相对于$R$的饱和，则$a$的每个闭邻域$V$都满足$B$；由于假设$B$是*关闭的*并且$X$是*常规*，因此$a \in B$因此是$(a, b) \in C$。这样就完成了证明。

#### 推论 {#top-i-s8-n6-cor-1 .statement tag=0B6X}

*在常规空间上，每个打开和关闭的等价关系都是 Hausdorff*。

这是从 no. 3 的命题 14 和命题 8 得出的。

#### 命题 15 {#top-i-s8-prop-15 .statement tag=0B6Y}

*设* $X$ *为正则空间*，$F$ ** $X$、$R$ *的闭子集* $X$ *通过识别* $F$ *的所有点获得等价关系[换句话说，等价关系的等价类为* $F$ *(if* $F \neq \emptyset$*) 和集合* $\{x\}$ *其中* $x \in CF$*]。 *那么商空间*$X/R$*就是Hausdorff*。

令$M$和$N$是$X$中两个不同的等价类。如果它们每个都由$F$的补集中的单个点组成，则Hausdorff子空间$CF$中存在$M$和$N$的两个不相交的开邻域；这些是$X$中$M$和$N$的邻域，并且相对于$R$饱和。如果$M = F$（因此$F \neq \emptyset$）和$N = \{ b \}$，其中$b \notin F$，则由于$X$是正则，因此存在$b$的开邻域和$F$的开邻域，它们不相交；这些邻域相对于$R$是饱和的，并且命题被证明。

请注意，商空间 $X/R$ 不一定是正则（章 IX, § 4、习题 14）。

### 习题{#top-i-s8-exercises}

参见[习题为 § 8](exercises/s8/)。
