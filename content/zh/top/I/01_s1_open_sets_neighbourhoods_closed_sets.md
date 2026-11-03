---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 1
section_title: Open sets, neighbourhoods, closed sets
lang: zh
source: top-i-iv
book_pages: 17-25, 117-119
pdf_pages: 0023-0031, 0123-0125
extraction: ocr
subsections:
    - "no": 1
      title: OPEN SETS
      page: 17
      pdf_page: 23
    - "no": 2
      title: NEIGHBOURHOODS
      page: 18
      pdf_page: 24
    - "no": 3
      title: FUNDAMENTAL SYSTEMS OF NEIGHBOURHOODS; BASES OF A TOPOLOGY
      page: 21
      pdf_page: 27
    - "no": 4
      title: CLOSED SETS
      page: 21
      pdf_page: 27
    - "no": 5
      title: LOCALLY FINITE FAMILIES
      page: 22
      pdf_page: 28
    - "no": 6
      title: INTERIOR, CLOSURE, FRONTIER OF A SET; DENSE SETS
      page: 23
      pdf_page: 29
statements: 24
exercises: 9
content_sha256: 3d9af4b03b92b9160bc6cd4609a517bc375cb7096622c8759d8e3b3351ef9fd5
translated_from: content/en/top/I/01_s1_open_sets_neighbourhoods_closed_sets.md
translation_method: google
source_content_sha256: 70913d7a2aa52b144a991fde157d2311e959bf9873a82740f1d49300682f0fef
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 64c42c79ee105d6e6723fce88a5bdfb6a2e696c3d6af7f51941903a95adfcd75
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 1. 营业集合、邻域、休息集合

### 1. 开集合

#### 定义 1 {#top-i-s1-def-1 .statement tag=0AZ1}

*拓扑结构*（或更简单地说，*拓扑*）*在集合*$X$*是结构由集合*$\mathscr{D}$*的子集的*$X$，*具有以下属性*（称为*公理拓扑结构*)：

(O_I) ** $\mathscr{D}$ *的集合的每个并是* $\mathscr{D}$ 的集合。

(O_{II}) ** $\mathscr{D}$ * 的集合的每个有限交是 * $\mathscr{D}$ 的集合。

* $\mathscr{D}$的*集合 *被称为由* $\mathscr{D}$ *在* $X$定义的拓扑结构的开集合。

#### 定义 2 {#top-i-s1-def-2 .statement tag=0AZ2}

*拓扑空间是集合赋予拓扑结构*。

拓扑空间的元素通常称为*点*。当在集合 $X$ 上定义拓扑时，集合被称为集合*底层*拓扑空间$X$。

公理 (O_I) 特别意味着 $\mathscr{D}$ 的空子集的并，即 *空集* 属于到 $\mathscr{D}$。公理(O_{II})意味着$\mathscr{D}$的空子集的交，即*集合*$X$、属于到$\mathscr{D}$。

为了证明$X$的子集的集合$\mathscr{D}$满足(O_{II})，通常可以方便地分别证明它满足以下两个公理，其中合取等价于(O_{II})：
(O_{II\a})*$\mathscr{D}$*属于到*$\mathscr{D}$的两个集合*交。
(O_{II\ b})$X$*属于到*$\mathscr{D}$。

例拓扑。给定 $X$ 和 $\varnothing$ 的任何集合 $X$，$X$ 由……组成的子集集合满足公理 $(O_1)$ 和 $(O_{II})$，因此定义拓扑于$X$。 $X$的所有子集中的集合$\mathfrak{P}(X)$也是如此：拓扑它定义是$X$上的离散拓扑，并且集合$X$与此拓扑称为离散空间。

如果拓扑空间 $X$ 的子集 $A$ 的覆盖$(U_i)_{i \in I}$ 被称为开路，则如果所有 $U_i$ 在$X$ 中都开路。

#### 定义 3 {#top-i-s1-def-3 .statement tag=0AZ3}

*拓扑空间$X$到拓扑空间$X'$的同胚是$X$的拓扑结构到$X'$的拓扑同构；*也就是说，根据一般$X$的定义*双射到$X'$，其中$X$的开子集的变换集合进入$X'$*的开子集的集合。

如果 $X$ 与 $X'$ 同态，则$X$ 和 $X'$ 被称为“同胚”。

#### 例 {#top-i-s1-n1-exa-1 .statement tag=0AZ4}

如果$X$和$X'$是两个离散的空间，则$X$到$X'$的任何双射都是同胚。

以下标准紧接着同胚的定义：*对于拓扑空间$X$的双射$f$到拓扑空间$X'$的同态，有必要且充分的是每个$f$下的像 $X$中的开集合是$X'$中的开集合，并且$X'$中的每个开集合的$f$下的逆像是$X$中的开集合*。

### 2. 邻域

#### 定义 4 {#top-i-s1-def-4 .statement tag=0AZ5}

*令$X$为拓扑空间和$A$$X$的任意子集。 $A$的邻域是$X$的任意子集，其中包含是开集合包含$A$。单个点的子集$\{ x \}$由……组成中的邻域也称为点$x$*中的邻域。

显然，$X$的子集$A$的每一个邻域也是子集$B \subset A$的每一个邻域；特别地，它是$A$中每个点的邻域。相反，假设$A$是集合$B$中每个点的邻域，并且令$U$是$A$中包含的开集合的并；然后$U \subset A$，并且由于$B$属于的每个点到包含在$A$中的开集合，我们有$B \subset U$；但$U$凭借$(O_1)$而开放，因此$A$是$B$的邻域。特别是：

#### 命题 1 {#top-i-s1-prop-1 .statement tag=0AZ6}

*当且仅当它打开时，集合是其每个点的邻域。*

字“邻域”的日常意义是这样的，涉及邻域数学思想的许多属性都表现为直观属性的数学表达； 项的选择因此具有使语言更具表现力的优点。为此目的，也允许在某些叙述中使用“足够接近”和“尽可能接近”的表达方式。例如，命题 1 可以用以下形式来表示： 集合 $A$ 是开放的，当且仅当对于每个 $x \in A$，所有点 *充分接近* $x$ 属于至$A$。更一般地说，如果$x$的某些邻域的点全部成立，那么性质对所有点*足够接近*点$x$成立。

让我们用$x$的所有邻域中的$\mathfrak{B}(x)$集合来表示。 集合 $\mathfrak{B}(x)$ 具有以下属性：

(V_I) *$X$中的每个子集，其中包含集合属于到$\mathfrak{B}(x)$本身属于到$\mathfrak{B}(x)$。*

(V_{II}) *$\mathfrak{B}(x)$属于到$\mathfrak{B}(x)$的集合的每个有限交。*

(V_{III}) *元素$x$位于$\mathfrak{B}(x)$的每集合中。*

事实上，这三个属性是定义 4 的直接的推论和公理 (O_{II})。

(V_{IV}) *如果$V$属于到$\mathfrak{B}(x)$，则有集合$W$属于到$\mathfrak{B}(x)$，这样，对于每个$y \in W$，$V$ 属于至 $\mathfrak{B}(y)$。*

到命题 1，我们可以将$W$视为任何开集合，其中包含$x$并且包含在$V$中。

这个性质可以用形式来表达，$x$的*邻域也是所有点的邻域，充分接近$x$*。

集合$\mathfrak{B}(x)$的这四个属性是*特征*。准确地说，我们有：

#### 命题 2 {#top-i-s1-prop-2 .statement tag=0AZ7}

*如果对于集合$X$的每个元素$x$，存在$X$的子集的对应集合$\mathfrak{B}(x)$，使得属性(V_I)，(V_{II})， (V_{III}) 和 (V_{IV}) 满足，则$X$上存在唯一的拓扑结构，使得对于每个$x \in X$，$\mathfrak{B}(x)$是$x$的邻域的集合拓扑.*

到命题 1 时，如果$X$ 满足上有拓扑这条件，为此集合集合拓扑必然是子集集合 $\mathscr{D}$ $X$的$A$使得*对于每个$x \in A$我们有$A \in \mathfrak{B}(x)$*；因此，如果存在的话，这个拓扑的*唯一性*。

集合 $\mathscr{D}$ 当然满足公理 (O_I) 和 (O_{II})：对于 (O_I)，这直接从 (V_I) 得出，对于 (O_{II})，从 (V_{II}) 得出。它

![图表显示集合 V、U、W 和点 x、y、z](https://i.imgur.com/3Q5z5QG.png)

图 1.

仍有待证明，在$\mathscr{D}$定义的拓扑中，对于每个$x \in X$，$\mathfrak{B}(x)$是$x$的邻域的集合。从(V_I)可以得出，$x$属于到$\mathfrak{B}(x)$的每一个邻域。相反，令$V$为集合属于至$\mathfrak{B}(x)$，并令$U$为点$y \in X$中的集合，使得$V \in \mathfrak{B}(y)$；如果我们能证明$x \in U, U \subset V$和$U \in \mathscr{D}$，那么证明就完整了。从 $V \in \mathfrak{B}(x)$ 开始，我们就有了 $x \in U$；还有 $U \subset V$，对于每个点 $y \in U$ 属于到 $V$，由于 (V_III) 和假设 $V \in \mathfrak{B}(y)$。还需要证明$U \in \mathscr{D}$，即每个$y \in U$对应$U \in \mathfrak{B}(y)$；现在（图1）如果$y \in U$，那么通过（V_IV）有集合$W$，这样对于每个$z \in W$，我们有$V \in \mathfrak{B}(z)$；因为$V \in \mathfrak{B}(z)$意味着$z \in U$，所以可以得出$W \subset U$，因此，根据(V_I)，$U \in \mathfrak{B}(y)$。

Q.E.D.

命题 2 表明$X$上的拓扑可以通过$X$的点的邻域的集合$\mathfrak{B}(x)$来定义，仅受限于公理 (V_I), (V_II)， （V_III）和（V_IV）。

#### 例 {#top-i-s1-n2-exa-1 .statement tag=0AZ8}

我们可以将有理数的集合$Q$上的定义拓扑取为有界开区间的开集合所有并；这些子集中的集合当然满足（O_I），并且要看到它满足（O_II）就足以说明如果两个开区间$]a, b[$和$]c, d[$中的交不为空，则它是区间$]\alpha, \beta[$，其中$\alpha = \sup(a, c)$和$\beta = \inf(b, d)$。通过将$x$的邻域的每个$x \in Q$集合$\mathfrak{B}(x)$定义为子集包含的集合，我们得到相同的拓扑，一个开区间到$x$ 属于。将这个拓扑代入$Q$得到的拓扑空间称为有理线（cf.章IV, § 1, no. 2）。请注意，在这个空间中，每个开区间都是一个开集合。 \* 我们可以用同样的方式对实数的集合$R$进行定义拓扑； $R$与拓扑称为实直线（cf.§ 2、习题5和章IV, § 1, no. 3）。 \*

### 3. 邻域的基本系统； 基 / 拓扑

#### 定义 5 {#top-i-s1-def-5 .statement tag=0AZ9}

在拓扑空间$X$中，点$x$的邻域的基本系统（分别是$X$的子集$A$）是以下任意集合$\mathfrak{G}$ $x$（或$A$）的邻域，使得对于$x$（或$A$）的每个邻域$V$，有邻域$W \in \mathfrak{G}$，使得$W \subset V$。

如果$\mathfrak{G}$是$X$的子集$A$的邻域的基本系统，则$\mathfrak{G}$的$\mathfrak{G}$包含集合的集合的每个有限交。

例。 1) 在离散的空间 (no. 1) 集合 $\{ x \}$ 中，单独构成邻域点 $x$ 的基本系统。
2) 在所有开区间包含点$x$的有理线上$\mathbf{Q}$集合是这个点的邻域的基本系统。开区间$]x - 1/n, x + 1/n[$的集合和闭区间$[x - 1/n, x + 1/n]$的集合也是如此，其中$n$贯穿所有整数$> 0$，或贯穿严格递增的序列的任何无限严格递增的序列整数$> 0$。
\* 实直线也有类似的结果。 \*

#### 定义 6 {#top-i-s1-def-6 .statement tag=0AZA}

一个拓扑空间$X$的拓扑基是$X$的开子集的任何集合$\mathfrak{B}$使得$X$的每个开子集是集合的并属于至$\mathfrak{B}$。

#### 命题 3 {#top-i-s1-prop-3 .statement tag=0AZB}

如果$X$是拓扑空间，则对于$X$的开子集的集合$\mathfrak{B}$为$X$的拓扑的基来说，对于每个$x \in X$集合是充分必要的$V \in \mathfrak{B}$使得$x \in V$是$x$的邻域的基本系统。

显然条件是必要的。相反，如果满足，则给定任何开集合$U$和任何$x \in U$，都存在一个开集合$V_x \in \mathfrak{B}$使得$x \in V_x \subset U$。因此，$x \in U$ 的集合 $V_x$ 的并等于$U$。这样就完成了证明。

#### 例 1 {#top-i-s1-n3-exa-1 .statement tag=0AZC}

离散的拓扑具有基集合、子集、$X$，由单个点组成。

#### 例 2 {#top-i-s1-n3-exa-2 .statement tag=0AZD}

有界开区间的集合是由有理线(no. 2)的拓扑的定义基。 \* 同样，有界开区间的集合是实直线的拓扑的基。 \*

### 4. 已关闭集合

#### 定义 7 {#top-i-s1-def-7 .statement tag=0AZE}

在拓扑空间$X$中，$X$的开集合的补集称为闭集合。

取补，我们发现公理$(O_I)$和$(O_{II})$取以下形式：

$(O'_I)$ *闭集合的每个交都是一个闭集合。*

$(O'_{II})$ *闭集合的每个有限并都是闭集合。*

空集和整个空间 $X$ 都是闭合的（因此*既开又闭合*；cf. § 11）。

在有理线上，形式$[a, \rightarrow[$的每个区间都是一个闭集合，对于它的补码]\leftarrow，a[是开的；同样，形式]\leftarrow, a] 的每个区间都是一个闭集合；因此，每个有界闭区间$[a, b]$也是如此，因为它是区间$[a, \rightarrow[$和]\leftarrow, b]的交。

有理数整数的集合$Z$在有理数线上是闭的，因为它的补数$\bigcup_{n \in Z} ]n, n+1[$是开路的。

如果每个 $F_i$ 都在 $X$ 中闭合，则拓扑空间 $X$ 的子集 $A$ *覆盖* $(F_i)_{i \in I}$ 被称为“闭”。

拓扑空间$X$到拓扑空间$X'$（no. 1）的*同胚*$f$可以表征为$X$到$X'$的双射*使得像在$X$的每个闭子集的$f$是$X'$的闭子集，并且$X'$的每个闭子集的$f$下的逆像是子集的闭子集 $X$*。

### 5. 局部有限家庭

#### 定义 8 {#top-i-s1-def-8 .statement tag=0AZF}

*拓扑空间$X$的子集的族$(A_i)_{i \in I}$被认为是局部有限的，如果对于每个$x \in X$，$x$有邻域$V$，使得除了有限的数之外的所有$V \cap A_i = \varnothing$ 指标$i \in I$。如果由 $\mathscr{S}$ 的恒等式映射定义的子集族是局部有限的，则 $X$ 的子集的集合 $\mathscr{S}$ 被认为是局部有限的。*

很明显，如果$(A_i)_{i \in I}$是子集的局部有限族，并且如果每个$i \in I$都有$B_i \subset A_i$，则$(B_i)_{i \in I}$族是局部有限的。

拓扑空间 $X$ 的子集的每个“有限”族显然是局部有限的； 逆命题一般来说是不正确的。

\* 例如，在$\mathbf{R}$中，对于每个整数$n \geqslant 0$，由区间]\leftarrow、1[和区间]$n, \rightarrow[$形成的开覆盖是局部有限的；并且每个区间]$n, \rightarrow[$都满足该覆盖层的集合的无限数。 \*

#### 命题 4 {#top-i-s1-prop-4 .statement tag=0AZG}

*拓扑空间$X$的局部有限闭族子集的并在$X$中封闭。*

设$(F_i)_{i \in I}$是$X$的闭子集的局部有限族，并假设$x \in X$不属于到$F = \bigcup_{i \in I} F_i$；那么$x$有邻域$V$，它只满足那些$F_i$，其指标属于到$I$的*有限*子集$J$。对于每个 $i \in J$ 令 $U_i$ 为 $F_i$ 的补集；然后$\complement F$包含集合$V \cap \bigcap_{i \in J} U_i$，这是$x$的邻域，因为每个$U_i$都是开放的，包含于$x$。因而，到 no. 2 的命题 1 时，$\complement F$ 打开，因而 $F$ 在 $X$ 关闭。

我们注意到，$X$的封闭子集的*任意*族中的并不一定是封闭的；例如，在有理线$\mathbf{Q}$上，集合$]2, 1[$是闭集合的并
$$
\left[ \frac{1}{n}, 1 - \frac{1}{n} \right] \quad \text{for } n > 2,
$$
但并未关闭。

### 6. 集合的内部、封闭、边界；浓密集合

#### 定义 9 {#top-i-s1-def-9 .statement tag=0AZH}

*在拓扑空间$X$中，如果$A$是$x$的邻域，点$x$被认为是子集$A$的点内部$X$。 $A$的内部点的集合称为$A$的内部，记为$\dot{A}$。*

根据定义 9和4，如果$A$中存在一个开集合，其中包含 $x$，则点$x$是$A$的内点；由此可见，$\dot{A}$是$A$中包含的所有开集合的并，因而*最大的开集合包含在*$A$：在其他字中，如果$B$是一个*开* 集合包含在$A$中，然后是$B \subset \dot{A}$。因而，如果$A$和$B$是$X$的两个子集，使得$B \subset A$，则$\dot{B} \subset \dot{A}$；并且$A$是$B$的邻域当且仅当$B \subset \dot{A}$。

#### 注 {#top-i-s1-n6-rem-1 .statement tag=0AZI}

非空集合的内部可以为空；这是单个点的集合由……组成的情况，该点未开，例如在有理线 \* （或实直线）* 上。

命题 1 of no. 2 可以重述如下：

*集合打开当且仅当重合及其内部。*

no. 2的性质$(V_{II})$意味着每个点是两个子集$A$和$B$中每一个的内部点是$A \cap B$的内部点；因而
$$(1)$$$$
\dot{A} \cap \dot{B} = \dot{A} \cap \dot{B}.
$$

每个集合$A$补集的内部点被称为$A$的*外部*点，并且这些点中的集合被称为$X$中$A$的*外部*；因此，作为$A$的外部点的点$x \in X$的特征在于性质，即*$x$具有不满足*$A$的邻域。

#### 定义 10 {#top-i-s1-def-10 .statement tag=0AZJ}

*拓扑空间* $X$ *的子集* $A$ *的闭包是所有点* $x \in X$的集合 *使得* $x$的每个邻域 *满足* $A$，*并且是用*$\overline{A}$表示。

这个定义可以通过说重新表述，点$x$位于集合$A$的闭包中，如果$A$有点*尽可能接近*$x$*如我们所愿*。

不在$A$闭包内的每个点都是$A$的外部，反之亦然；因此我们有公式 （它们是彼此的对偶）

$$(2)$$
$$
\mathscr{C}\overline{A} = \widehat{\mathscr{C}}A,\qquad \mathscr{C}\dot{A} = \overline{\mathscr{C}}A.
$$

因此，对于集合内部的任何命题，闭包上的*对偶性*命题存在对应，反之亦然。特别地，集合$A$的闭包是*最小的闭集合，其中包含*$A$；在其他字中，如果$B$是闭集合，使得$A \subset B$，则$\overline{A} \subset B$。如果$A$和$B$是$X$的两个子集，使得$A \subset B$，则$\overline{A} \subset \overline{B}$。

*集合是封闭的当且仅当重合及其闭包*。

公式 (1) 的对偶是

$$(3)$$
$$
\overline{A \cup B} = \overline{A} \cup \overline{B}.
$$

#### 命题 5 {#top-i-s1-prop-5 .statement tag=0AZK}

*设*$A$*为*$X$中的开集合； *然后对于每个子集* $B$ *of* $X$ *我们有*

$$(4)$$
$$
A \cap \overline{B} \subset \overline{A \cap B}.
$$

假设$x \in A \cap \overline{B}$；那么如果$V$是$x$中的任意邻域，则$V \cap A$是$x$中的邻域，因为$A$是开放的；因此$V \cap A \cap B$不为空，因此$x$位于$A \cap B$的闭包中。

如果$x$位于$A$的闭包中但不在$A$中，则$A$的$x$包含点的每个邻域*除了*$x$；但如果$x \in A$，则可能发生$x$有邻域，其中包含没有$A$的点，除了$x$。那么我们说$x$是$A$的*孤立的点*。特别地，当且仅当$\{x\}$是开集合时，$x$在整个空间$X$中是孤立的。

没有孤立的点的封闭集合称为*完美* 集合。

#### 定义 11 {#top-i-s1-def-11 .statement tag=0AZL}

在拓扑空间$X$中，如果$x$位于$A$的闭包和$\overline{CA}$的闭包中，则点$x$被称为集合$A$的边界点。 $A$的边界点的集合称为$A$的边界。

因此，$A$的边界是集合$\overline{A} \cap \overline{\overline{CA}}$，它是封闭的。 $A$的边界点$x$的特征在于性质，$x$包含的每邻域至少有一个点在$A$和至少一个点 $\overline{CA}$； $x$ 可能会也可能不会属于至 $A$。 $A$的边界与$\overline{CA}$的边界相同。 $A$的内部、$A$的外部和$A$的边界互为不相交的，并且它们的并是整个空间$X$。

#### 定义 12 {#top-i-s1-def-12 .statement tag=0AZM}

如果$\overline{A} = X$，即如果每个非空开集合，则拓扑空间$X$的子集$A$被认为在$X$是稠密的（或者简单地稠密，如果$X$没有歧义） $X$中的$U$满足$A$。

#### 例 {#top-i-s1-n6-exa-1 .statement tag=0AZN}

\* 我们将在章IV, § 1中看到有理数的集合及其补集在实直线上稠密。 \*
在离散空间 $X$ 中，$X$ 的唯一稠密子集是 $X$ 本身。另一方面，$X$的每个非空子集都密集在$X$上的拓扑，其中唯一的开集合是$\varnothing$和$X$。

#### 命题 6 {#top-i-s1-prop-6 .statement tag=0AZO}

如果$\mathfrak{B}$是拓扑空间$X$的拓扑的基，则在$X$中存在稠密的集合$D$使得$\mathrm{Card}(D) \leq \mathrm{Card}(\mathfrak{B})$。

我们可以将自己限制在$\mathfrak{B}$的集合都不为空的情况（$\mathfrak{B}$的非空集已经是$X$的拓扑的形式基）。对于每个$U \in \mathfrak{B}$，令$x_V$为$U$的点；从 no. 3 的命题 3 可以得出，点 $x_U$ 的集合 $D$ 密集在 $X$ 中，我们有 $\mathrm{Card}(D) \leq \mathrm{Card}(\mathfrak{B})$ (集合理论, 章) III, § 3, no. 2、命题 3)。

### 习题 {#top-i-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
