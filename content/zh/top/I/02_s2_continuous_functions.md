---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 2
section_title: Continuous functions
lang: zh
source: top-i-iv
book_pages: 25-35, 119-122
pdf_pages: 0031-0041, 0125-0128
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS FUNCTIONS
      page: 25
      pdf_page: 31
    - "no": 2
      title: COMPARISON OF TOPOLOGIES
      page: 28
      pdf_page: 34
    - "no": 3
      title: INITIAL TOPOLOGIES
      page: 30
      pdf_page: 36
    - "no": 4
      title: FINAL TOPOLOGIES
      page: 32
      pdf_page: 38
    - "no": 5
      title: PASTING TOGETHER OF TOPOLOGICAL SPACES
      page: 34
      pdf_page: 40
statements: 30
exercises: 11
content_sha256: 29977b43cc1f150f5106a03484aac56adba575b19d946f3ca187f53a6203996c
translated_from: content/en/top/I/02_s2_continuous_functions.md
translation_method: google
source_content_sha256: 1967343889fcc981f4c5cd14526701e2a3a3c66ffbc62c0729eebd3c4a84398d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: aaf971328986bd374e46a7faf2c2b89afe8ab73b91c3593be534d173647a0cef
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 2.连续函数

### 1.连续函数

#### 定义 1 {#top-i-s2-def-1 .statement tag=0AZY}

A mapping $f$ of a topological space $X$ into a topological space $X'$ is said to be continuous at a point $x_0 \in X$ if, given any neighbourhood $V'$ of $f(x_0)$ in $X'$, there is a neighbourhood $V$ of $x_0$ in $X$ such that the relation $x \in V$ implies $f(x) \in V'$.

定义 1 可以在下面更直观的形式中重述：说$f$在点连续$x_0$意味着只要$x$足够接近$x_0$，$f(x)$就尽可能接近$f(x_0)$。

关系“对于每个$x \in V, f(x) \in V'$”相当于$f(V) \subset V'$或再次相当于$V \subset \overline{f}^{-1}(V')$；鉴于邻域公理 ($V_I$)，我们看到定义 1 等价于以下内容： $f : X \to X'$ 被称为在点 $x_0$ 处连续 如果对于 $X'$ 中 $f(x_0)$ 的每个邻域 $V'$， $\overline{f}^{-1}(V')$ 是$X$ 中$x_0$ 的邻域。另外，对于$X'$中的$f(x_0)$的邻域的基本系统，对于每个邻域$V'$属于，$\overline{f}^{-1}(V')$是$x_0$的邻域就足够了($§ 1$， no. 3）。

#### 命题 1 {#top-i-s2-prop-1 .statement tag=0AZZ}

设$f$是拓扑空间$X$的映射到拓扑空间$X'$。如果$f$在$x$连续，且$x$位于$X$的子集$A$的闭包内，则$f(x)$位于$f(A)$的闭包内。

令$V'$为$X'$中$f(x)$的邻域。由于$f$在$x$连续，因此$\overline{f}^{-1}(V')$是$X$中$x$的邻域。因此$\overline{f}^{-1}(V')$满足$A$，由此得出$V'$满足$f(A)$，因此$f(x)$位于$f(A)$的闭包中。

#### 命题 2 {#top-i-s2-prop-2 .statement tag=0B00}

令$X, X', X''$为三个拓扑空间；设$f$为$X$的映射入$X'$，在$x \in X$连续；设$g$为$X'$的映射入$X''$，在$f(x)$连续。那么合成$h = g \circ f : X \to X''$在$x$处连续。

令$V''$为$X''$中$h(x) = g(f(x))$的邻域。由于$g$在$f(x)$连续，因此$\overline{g}^{-1}(V'')$是$X'$中$f(x)$的邻域。但$f$在$x$连续，因此$\overline{f}^{-1}(\overline{g}^{-1}(V'')) = \overline{h}^{-1}(V'')$是$X$中$x$的邻域，因此$h$在$x$连续。

#### 定义 2 {#top-i-s2-def-2 .statement tag=0B01}

如果拓扑空间$X$到拓扑空间$X'$的映射在$X$上连续（或者只是连续），如果它在$X$的每个点连续。

#### 例 1 {#top-i-s2-n1-exa-1 .statement tag=0B02}

拓扑空间$X$自身的恒等映射是连续的。

#### 例 2 {#top-i-s2-n1-exa-2 .statement tag=0B03}

拓扑空间到拓扑空间的常数映射是连续的。

#### 例 3 {#top-i-s2-n1-exa-3 .statement tag=0B04}

离散空间到拓扑空间的每个映射都是连续的。

#### 定理 1 {#top-i-s2-thm-1 .statement tag=0B05}

设$f$是拓扑空间$X$到拓扑空间$X'$的映射。那么下面的叙述是等价的：

a) $f$ 在$X$ 中连续。

b) 对于$X$中的每子集$A$，$f(\overline{A}) \subset \overline{f(A)}$。

c) $X'$的每个闭子集的$f$下的逆像是$X$的闭子集。

d) $X'$的每个开子集的$f$下的逆像是$X$的开子集。

我们已经看到 a) 蕴涵 b) (命题 1)。为了证明 b) 蕴含 c)，令 $F'$ 为 $X'$ 的闭子集，并令 $F = \overline{f^{-1}(F')}$；然后假设$f(\overline{F}) \subset \overline{f(F)} \subset \overline{F'} = F'$，因此$\overline{F} \subset \overline{f^{-1}(F')} = F \subset \overline{F}$，从而$F = \overline{F}$和$F$是闭合的。凭借关系$\overline{f^{-1}(A')} = \overline{f^{-1}(CA')}$对于$X'$的每一个子集$A'$，c）意味着d）。最后，假设d)得到满足。令$x$为$X$中的任意点，并令$V'$为$X'$中$f(x)$的任意邻域；那么$X'$中有一个开集合$A'$，其中

$$
f(x) \in A' \subset V'
$$

因此$x \in \overline{f^{-1}(A')} \subset \overline{f^{-1}(V')}$。到假设，$\overline{f^{-1}(A')}$在$X$开放，因此$\overline{f^{-1}(V')}$是$X$中$x$的邻域。因此 d) 意味着 a)。

#### 注 {#top-i-s2-n1-rem-4 .statement tag=0E95}

1) 设$\mathfrak{B}$为$X'$的拓扑中的基(§ 1, no. 3)；那么要使$f : X \to X'$连续，对于每一个$U' \in \mathfrak{B}$，$\overline{f^{-1}(U')}$在$X$中开路是充分必要的。

#### 例 {#top-i-s2-n1-exa-4 .statement tag=0B06}

令 $a$ 为任何有理数数。有理线$\mathbf{Q}$自身的映射$x \to a + x$在$\mathbf{Q}$上连续，因为逆像在开区间的映射下$]b, c[$是开区间

$$
]b - a, c - a[.
$$

同样，映射$x \to ax$在$\mathbf{Q}$上连续；这是很清楚的，如果$a = 0$，则$ax = 0$，对于所有$x$；如果$a \neq 0$，则开区间$]b, c[$的这个映射下的逆像是端点为$b/a$和$c/a$的开区间。

2) 在连续映射 $f : X \to X'$ 下，$X$ 的开（或闭）集合的直接像不一定在 $X'$ (cf. § 5) 中开（或闭）。

#### 例 {#top-i-s2-n1-exa-5 .statement tag=0B07}

\* $\mathbf{R}$的映射$f : x \to 1/(1 + x^2)$自身是连续的，但$f(\mathbf{R})$是半开区间$]0, 1]$，在$\mathbf{R}$中既不开也不闭。 \*

#### 定理 2 {#top-i-s2-thm-2 .statement tag=0B08}

1) 如果$f : X \to X'$和$g : X' \to X''$是两个连续的映射，则$g \circ f : X \to X''$是连续的。

2) 为了使拓扑空间$X$到拓扑空间$X'$的双射$f$成为同胚，$f$和$f$的逆是连续的（或者，也可以说，$f$是双连续）。

第一个断言是命题2的直接的推论；第二个来自同胚 (§ 1, no. 1) 的定理 1, d) 和定义。

#### 注 1 {#top-i-s2-n1-rem-1 .statement tag=0B09}

拓扑空间 $X$ 的连续双射可以在非双连续的拓扑空间 $X'$ 上存在：对于例，取 $X'$ 为有理线 $\mathbf{Q}$，$X$ 为集合 $\mathbf{Q}$ 与离散拓扑；那么恒等式映射 $X \to X'$ 是连续的，但不是同胚。

#### 注 2 {#top-i-s2-n1-rem-2 .statement tag=0B0A}

要验证连续双射 $f : X \to X'$ 是同胚，只需证明对于 $x$ 的每个 $x \in X$ 和每个邻域 $V$，$f(V)$ 是 $X'$ 中$f(x)$ 的邻域。

#### 注 3 {#top-i-s2-n1-rem-3 .statement tag=0B0B}

令$X$为拓扑空间，对于每个$x \in X$，令$\mathfrak{B}(x)$为$x$的所有邻域的集合。 设$x_0$为$X$的点；对于$X$的子集的每个$x \in X$，定义集合$\mathfrak{B}_0(x)$如下：$\mathfrak{B}_0(x_0) = \mathfrak{B}(x_0)$，如果$x \neq x_0$则$\mathfrak{B}_0(x)$将是所有子集的集合 $X$ 其中包含 $x$。 It is immediately verified (§ 1, no. 2, Proposition 2) that the sets $\mathfrak{B}_0(x)$ are sets of neighbourhoods of points of $X$ for a topology on $X$; let $X_0$ denote the topological space thus obtained, and let $j : X_0 \to X$ denote the identity map, which is continuous but not in general bicontinuous. $X$的映射$f$进入拓扑空间$X'$在点$x_0$连续当且仅当合成$X_0 \xrightarrow{j} X \xrightarrow{f} X'$在$X_0$连续；这立即从定义开始。

### 2. 拓扑比较

no. 1的定理 2表明我们可以将连续映射视为拓扑结构的态射（集合理论，章IV, § 2, no. 1）；从现在开始，我们假设我们已经制作了态射的选择。根据一般的定义（集合理论，章IV, § 2, no. 2），这允许我们在给定的集合$X$上对集合拓扑进行定义排序：

#### 定义 3 {#top-i-s2-def-3 .statement tag=0B0C}

给定相同集合$X$上的两个拓扑$\mathfrak{T}_1, \mathfrak{T}_2$，我们说$\mathfrak{T}_1$比$\mathfrak{T}_2$更更细（并且$\mathfrak{T}_2$比$\mathfrak{T}_1$更粗糙）如果用$X_i$集合表示$X$ 与拓扑 $\mathfrak{T}_i$ ($i = 1, 2$)，恒等映射 $X_1 \to X_2$ 是连续的。如果在加法$\mathfrak{T}_1 \neq \mathfrak{T}_2$中，我们说$\mathfrak{T}_1$严格地更细比$\mathfrak{T}_2$（并且$\mathfrak{T}_2$严格地比$\mathfrak{T}_1$更粗糙）。

据说两种拓扑具有可比性，其中一种拓扑比另一种拓扑更细。

判据对于映射是连续的（no. 1、定义 1 和定理 1），给出以下命题：

#### 命题 3 {#top-i-s2-prop-3 .statement tag=0B0D}

给定集合 $X$ 上的两个拓扑 $\mathfrak{T}_1, \mathfrak{T}_2$，以下叙述是等效的：
a) $\mathfrak{T}_1$ 比 $\mathfrak{T}_2$ 更细。
b) 对于每个$x \in X$，$\mathfrak{T}_2$的$x$的每个邻域是$\mathfrak{T}_1$的$x$的邻域。
c) 对于$X$的每个子集$A$，拓扑$\mathfrak{T}_1$中$A$的闭包包含在拓扑$\mathfrak{T}_2$中$A$的闭包中。
d) $X$ 中每一个子集在 $\mathfrak{T}_2$ 关闭，在 $\mathfrak{T}_1$ 关闭。
e) 在$\mathfrak{T}_2$开放的$X$中的每个子集在$\mathfrak{T}_1$开放。

#### 例 {#top-i-s2-n2-exa-1 .statement tag=0B0E}

\* 在希尔伯特空间 $H$ 由……组成序列 $x = (x_n)$ 实数这样
$$
\|x\|^2 = \sum_{n=0}^\infty x_n^2 < +\infty,
$$
$H$上的强拓扑中的点$x_0$中的邻域是集合，其中包含以$x_0$为中心的开球$\|x - x_0\| < \alpha$； $H$上的弱拓扑中的$x_0$的邻域是由形式$\sup_{1 \leq i \leq n} |(x - x_0|a_i)| \leq 1$的关系定义的集合包含集合，其中$a_i$是$H$ 中的点以及
$$
(x|y) = \sum_{n=0}^\infty x_n y_n
$$
如果$x = (x_n)$和$y = (y_n)$。现在如果$\beta = \sup_{1 \leq i \leq n} \|a_i\|$，关系$\|x - x_0\| \leq 1 / \beta$意味着$|(x - x_0|a_i)| \leq \|x - x_0\| \cdot \|a_i\| \leq 1$对应$1 \leq i \leq n$；因此，$H$上的强拓扑比弱拓扑是更细。另一方面，给定$H$的点的任何有限族$(a_i)_{1 \leq i \leq n}$，$H$中存在点$x$，使得$(x - x_0|a_i) = 0$对于$1 \leq i \leq n$并且$\|x - x_0\|$是任意大；这表明强拓扑严格地更细比弱拓扑。 \*

#### 注 1 {#top-i-s2-n2-rem-1 .statement tag=0B0F}

在集合$X$上所有拓扑的有序集合中，拓扑中，唯一开放的集合是$\varnothing$，$X$最粗，离散的拓扑最细。

#### 注 2 {#top-i-s2-n2-rem-2 .statement tag=0B0G}

更细拓扑，较开集合，闭门集合和邻域； 更细拓扑，集合的封闭（或内部）较小（或较大）； 更细拓扑，密度较小的集合。

#### 注 3 {#top-i-s2-n2-rem-3 .statement tag=0B0H}

如果 $f : X \to X'$ 是连续的映射，则如果 $X$ 的拓扑被更细拓扑替换，并且 $X'$ 的拓扑被更粗糙的拓扑替换（no. 1， 定理2)。在其他字、$X$的更细拓扑和$X'$较粗的拓扑中，$X$到$X'$有更连续的映射。

### 3. 初始拓扑

#### 命题 4 {#top-i-s2-prop-4 .statement tag=0B0I}

令$X$为集合，令$(Y_i)_{i \in I}$为空间的拓扑族，对于每个$i \in I$，令$f_i$为$X$到$Y_i$的映射。 Let $\mathscr{S}$ be the set of subsets of $X$ of the form $\overline{f}_i^{-1}(U_i)$ ($i \in I$, $U_i$ open in $Y_i$), and let $\mathfrak{B}$ be the set of finite intersections of sets of $\mathscr{S}$. 那么$\mathfrak{B}$是$X$上拓扑$\mathfrak{T}$的基，这是族$(f_i)$在$X$上的初始拓扑结构（集合理论，章IV, § 2, no. 3），特别是最粗糙的拓扑在 $X$ 上，映射 $f_i$ 是连续的。 更准确地说，如果$g$是拓扑空间$Z$到$X$的映射，那么$g$在点$z \in Z$处连续（X携带拓扑$\mathfrak{T}$）当且仅当函数 $f_i \circ g$ 在 $z$ 连续。

令$\mathscr{D}$为集合属于到$\mathfrak{B}$的所有并中的集合；显然$\mathscr{D}$满足公理$(O_1)$，因为并的形成是结合的；并且$\mathscr{D}$由于$\mathfrak{B}$的定义以及有限交在任意并上可分配的事实而满足公理$(O_{II})$[集合理论，R § 4，公式(37)]。因此，对于拓扑$\mathfrak{T}$，集合$\mathscr{D}$是$X$的开子集的集合，其中$\mathfrak{B}$是基。我们将证明命题的最后一个断言，这通过初始结构的一般性质隐含了其他的（集合理论，章IV, § 2, no. 3，标准CST 9）。首先，$\mathscr{S}$的定义表明$f_i$在$X$上连续（no. 1，定理1）；因此，如果 $g$ 在 $z$ 连续，则映射 $f_i \circ g$ (no. 1, 命题 2) 也连续。反之，假设所有映射$f_i \circ g$在$z$处连续，并令$V$为$X$中$g(z)$的邻域；到定义，$I$有有限子集$J$，并且对于每个$i \in J$，$Y_i$有一个开放的子集$U_i$，使得$V$包含集合 $\bigcap_{i \in J} \overline{f}_i^{-1}(U_i)$和$g(z)$属于到这个集合。由此可见
$$
\overline{g}^{-1}(V) \supset \bigcap_{i \in J} \overline{g}^{-1}(\overline{f}_i^{-1}(U_i)),
$$
假设意味着集合 $\overline{g}^{-1}(\overline{f}_i^{-1}(U_i))$ 中的每一个都是$Z$ 中$z$ 的邻域；因此$\overline{g}^{-1}(V)$也是$Z$中$z$的邻域。这样就完成了证明。

设$\mathfrak{B}_i$为$Y_i (i \in I)$拓扑基；令$\mathscr{S}'$对于$i \in I$表示形式$\overline{f}_i^{-1}(U_i)$$X$子集集合，对于每个$i \in I$表示$U_i \in \mathfrak{B}_i$；如果$\mathfrak{B}'$是$\mathscr{S}'$的集合有限的交集合，显然$\mathfrak{B}'$是拓扑$\mathfrak{T}$的基。

初始结构（集合理论，章IV, § 2, no. 3，标准 CST 10）的一般属性特别意味着以下传递性性质（其直接证明非常简单）：

#### 命题 5 {#top-i-s2-prop-5 .statement tag=0B0J}

令$X$为集合，$(Z_i)_{i \in I}$为空间的拓扑族，$I$的$(J_\lambda)_{\lambda \in L}$划分，以及$(Y_\lambda)_{\lambda \in L}$由$L$索引的集合族。同样对于每个$\lambda \in L$，让$h_\lambda$是$X$到$Y_\lambda$的映射；对于每个$\lambda \in L$和每个$i \in J_\lambda$，让$g_{i\lambda}$为$Y_\lambda$的映射放入$Z_i$，并放入$f_i = g_{i\lambda} \circ h_\lambda$。如果每个 $Y_\lambda$ 都带有映射 $g_{i\lambda} (i \in J_\lambda)$ 连续的最粗糙拓扑，则 $X$ 上 $f_i$ 连续的最粗糙拓扑与 $h_\lambda$ 连续的最粗糙拓扑相同。

#### 例 1 {#top-i-s2-n3-exa-1 .statement tag=0B0K}

逆像共拓扑。令$X$为集合，$Y$为$X$的拓扑空间，$f$映射到$Y$； $f$连续的$X$上最粗的拓扑$\mathfrak{T}$称为$Y$的拓扑的$f$下的逆像。从命题 4 和公式得出并和交的逆像 [集合理论，R，§ 4，公式 (34) 和 (46)]，开（或闭）集合在拓扑 $\mathfrak{T}$ 是 $Y$ 的$f$ 集合下的逆像；因而，对于每个$x \in X$，集合$f^{-1}(W)$，其中$W$穿过$f(x)$的基本系统的邻域在$Y$，形式基本系统的邻域拓扑$\mathfrak{T}$中的$x$。在§ 3中，我们将以诱导拓扑的名义研究$X$是$Y$中的子集且$f$是典范嵌入$X \to Y$的特殊情况； $X$，加上诱导的拓扑，则称为$Y$的子空间。

为了使拓扑空间$X$的映射$f$到拓扑空间$X'$连续，$X$的拓扑比$f$下的逆像是更细是必要且充分的拓扑共 $X'$。

#### 例 2 {#top-i-s2-n3-exa-2 .statement tag=0B0L}

集合拓扑中至少上界。 集合 $X$上的拓扑族$(\mathfrak{T}_i)_{i \in I}$在$X$上所有拓扑的有序集合中至少有上界$\mathfrak{T}$，即$X$上存在拓扑，这是所有拓扑中最粗的$X$ 比每个 $\mathfrak{T}_i$ 更细。为了看到这一点，我们可以将应用命题 4，将$Y_i$视为集合$X$，其中拓扑$\mathfrak{T}_i$，以及$f_i$作为恒等式映射$X \to Y_i$； $\mathfrak{T}$ 是最粗糙的拓扑，其中所有映射 $f_i$ 都是连续的。

令$\mathfrak{S}$为集合$X$中子集的任意集合；在$X$上的集合或$\mathfrak{S}$开放的拓扑$\mathfrak{T}$中，有拓扑$\mathfrak{T}_0$比所有其他拓扑都更粗糙，称为由$\mathfrak{S}$生成的拓扑。对于每个集合$U \in \mathfrak{S}$，令$\mathfrak{T}_U$为拓扑，其开集合为$\varnothing, U$和$X$[很明显，$X$的子集的集合满足(O_I)并且(O_{II})];那么$\mathfrak{T}_0$只是拓扑$\mathfrak{T}_U$中最小的上界。由命题 4，若$\mathfrak{B}$为集合属于有限交至$\mathfrak{S}$集合，则$\mathfrak{B}$为拓扑$\mathfrak{T}_0$基。我们说$\mathfrak{S}$是$\mathfrak{T}_0$的子底。

#### 例 3 {#top-i-s2-n3-exa-3 .statement tag=0B0M}

乘积拓扑。设$(X_i)_{i \in I}$是拓扑空间的族。 乘积集合 $X = \prod_{i \in I} X_i$ 上的最粗拓扑，其中投影 $\mathrm{pr}_i : X \to X_i$ 是连续的映射称为$X_i$ 拓扑的*乘积*；我们将更详细地研究它

### 4. 最终拓扑

#### 命题 6 {#top-i-s2-prop-6 .statement tag=0B0N}

*令$X$为集合，让$(Y_i)_{i \in I}$为空间的拓扑族，对于每个$i \in I$，令$f_i$为$Y_i$到$X$的映射。令$\mathscr{D}$为子集$U$或$X$的集合，使得对于每个$i \in I$，$\overline{f}_i^{-1}(U)$在$Y_i$中开；那么$\mathscr{D}$就是$X$上拓扑$\mathfrak{T}$中$X$开子集集合，对于家庭$(f_i)$来说就是$X$最后的结构（集合理论， 章 IV, § 2, no. 5），特别是$\mathfrak{T}$是$X$上最好的拓扑，其中映射$f_i$是连续的。在其他字中，如果$g$是$X$的映射进入拓扑空间$Z$，则$g$是连续的（$X$携带拓扑$\mathfrak{T}$）当且仅当映射 $g \circ f_i$ 是连续的。*

立即验证$\mathscr{D}$满足公理$(O_I)$和$(O_{II})$。 [集合理论，R，§ 4，公式（34）和（46）]。我们将证明命题的最后一个断言，由于最终结构的一般性质，这意味着另一个断言（集合理论，章IV, § 2, no. 5，标准CST 18）。显然，$f_i$在拓扑$\mathfrak{T}$中连续，通过$\mathscr{D}$的定义（no. 1，定理1）；因此，如果 $g$ 是连续的，则每个映射 $g \circ f_i$ (no. 1, 定理 2) 也是连续的。反之，假设每个$g \circ f_i$是连续的，令$V$为$Z$中的开集合； 假设之前，$\overline{f}_i^{-1}(\overline{g}^{-1}(V))$在$Y_i$开放，每$i \in I$开放；因此 $\overline{g}^{-1}(V) \in \mathscr{D}$ 和证明是完整的。

#### 推论{#top-i-s2-n4-cor-1 .statement tag=0B0O}

*在命题 6 的假设下，$X$ 的子集 $F$ 在拓扑 $\mathfrak{T}$ 中闭合，当且仅当对于每个$i \in I$，$\overline{f}_i^{-1}(F)$ 在$Y_i$ 中闭合。*

This follows from the definition of the open sets in the topology $\mathfrak{T}$ by taking complements.

最终结构（集合理论，章IV, § 2, no. 5，标准CST 19）的一般属性意味着以下*传递性*性质（其直接证明也很简单）：

#### 命题 7 {#top-i-s2-prop-7 .statement tag=0B0P}

*令$X$为集合，$(Z_i)_{i \in I}$为空间的拓扑族，$I$的$(J_\lambda)_{\lambda \in L}$划分，以及$(Y_\lambda)_{\lambda \in L}$由$L$索引的集合族。另外，对于每个$\lambda \in L$，令$h_\lambda$为$Y_\lambda$到$X$的映射；对于每个$\lambda \in L$和每个$i \in J_\lambda$，让$g_{\lambda i}$为$Z_i$的映射放入$Y_\lambda$，并放入$f_i = h_\lambda \circ g_{\lambda i}$。如果每个 $Y_\lambda$ 都包含最细的拓扑，其中映射 $g_{\lambda i} (i \in J_\lambda)$ 是连续的，则 $X$ 上的 $f_i$ 是连续的最细的拓扑与 $h_\lambda$ 是连续的最细的拓扑相同。*

Examples

1) 商拓扑。 令$X$为$X$的$X$、$Y = X/R$商集关于关系$R$、$\varphi : X \to Y$典范映射的拓扑空间、$R$等价关系。 The finest topology on $Y$ for which $\varphi$ is continuous is called the quotient of the topology of $X$ by the relation $R$; we shall study it in more detail in § 3.

2) 拓扑结构的集合中的下确界。 集合 $X$ 上的每个拓扑族 $(\mathfrak{T}_i)_{i \in I}$ 在 $X$ 上的所有拓扑的集合中都有下确界 $\mathfrak{T}$，即 $\mathfrak{T}$ 是 $X$ 上所有拓扑中最精细的，它比每个拓扑都更粗糙$\mathfrak{T}_i$。为了看到这一点，我们可以将应用命题 6，将$Y_i$视为集合$X$，其中拓扑$\mathfrak{T}_i$，并将$f_i$视为恒等映射$Y_i \to X$。如果$\mathscr{D}_i$是拓扑$\mathfrak{T}_i$开放的$X$子集的集合，那么集合$\bigcap_{i \in I} \mathscr{D}_i$就是$X$开放的子集的集合 $\mathfrak{T}$。 $\mathfrak{T}$也称为拓扑$\mathfrak{T}_i$的交。

3) 拓扑空间的和。令$(X_i)_{i \in I}$为空间、$X$集合的拓扑族，即$X_i$的和（集合理论、章II, § 4, no. 8、定义8）；对于每个$i \in I$，令$j_i$为$X_i$到$X$的规范（内射）映射。 $X$上最精细的拓扑$\mathfrak{T}$（其中映射$j_i$是连续的）被称为$X_i$拓扑的和，并且$X$与此拓扑被称为拓扑的和空间$X_i$。让我们通过$j_i$来计算$X$中的$X_i$和子集中的每一个认同；那么集合$A \subset X$在拓扑$\mathfrak{T}$中打开（或关闭）当且仅当集合$A \cap X_i$中的每一个在$X_i$中打开（或关闭）。特别地，每个$X_i$既是开放的又是封闭的。

下面的命题概括了例3的情况：

#### 命题 8 {#top-i-s2-prop-8 .statement tag=0B0Q}

令$X$为集合，$(X_\lambda)_{\lambda \in L}$是子集和$X$的一个家族。假设每个$X_\lambda$携带拓扑$\mathfrak{T}_\lambda$，这样，对于指标$(\lambda, \mu)$的每个对：
1) $X_\lambda \cap X_\mu$ 在每个拓扑 $\mathfrak{T}_\lambda, \mathfrak{T}_\mu$ 中都是开路（或闭路）。
2) 由$\mathfrak{T}_\lambda$和$\mathfrak{T}_\mu$重合在$X_\lambda \cap X_\mu$上导出的拓扑。令$\mathfrak{T}$为$X$上最好的拓扑，其中单射$j_\lambda : X_\lambda \to X$是连续的。然后，对于每个$\lambda \in L$，$X_\lambda$在拓扑$\mathfrak{T}$中的$X$中打开（或关闭），并且拓扑由$\mathfrak{T}$在$X_\lambda$重合上与$\mathfrak{T}_\lambda$诱导。

鉴于命题 6 及其推论，足以证明对于 $\lambda$ 和 $X_\lambda$ 的每个子集 $A_\lambda$，以下叙述是等价的：
(i) $A_\lambda$ 在拓扑 $\mathfrak{T}_\lambda$ 开放（或关闭）。
(ii) 对于每个 $\mu \in L$，$A_\lambda \cap X_\mu$ 在拓扑 $\mathfrak{T}_\mu$ 中打开（或关闭）。

很明显，(ii) 通过取 $\mu = \lambda$ 暗示 (i)。相反，如果满足 (i)，则 $A_\lambda \cap X_\mu$ 在 $X_\lambda \cap X_\mu$ 中开（或闭），对于拓扑 $\mathfrak{T}_{\lambda \mu}$，由 $\mathfrak{T}_{\lambda}$ 在 $X_{\lambda} \cap X_{\mu}$ 上诱发；但$\mathfrak{T}_{\lambda \mu}$也是由$\mathfrak{T}_{\mu}$在$X_{\lambda} \cap X_{\mu}$上诱发拓扑；因此$A_{\lambda} \cap X_{\mu}$也是$X_{\lambda} \cap X_{\mu}$的交，其中$X_{\mu}$的子集$B_{\mu}$在拓扑$\mathfrak{T}_{\mu}$中打开（或关闭）；由于 $X_{\lambda} \cap X_{\mu}$ 在 $\mathfrak{T}_{\mu}$ 中打开（或关闭），$A_{\lambda} \cap X_{\mu}$ 也是如此。这样就完成了证明。

我们注，如果$X_{\lambda}$的并与$X$不同，那么$\mathfrak{T}$在$X - \left( \bigcup_{\lambda \in L} X_{\lambda} \right)$上诱导的拓扑是*离散的*。因为如果 $x \in X$ 属于不存在 $X_{\lambda}$，则 $\{ x \} \cap X_{\lambda} = \varnothing$ 在每个拓扑 $\mathfrak{T}_{\lambda}$ 中开路，因此 $\{ x \}$ 在拓扑 $\mathfrak{T}$ 中开路。

### 5. 拓扑空间的粘贴在一起

令$(X_{\lambda})_{\lambda \in L}$为集合的族，令$X$为集合，即$X_{\lambda}$的*和*（*集合理论*，章II, § 4, no. 8，定义8）；我们将认同每个$X_{\lambda}$与$X$的子集通过典范嵌入$j_{\lambda} : X_{\lambda} \to X$。

令$R$为$X$上的等价关系，使得*$R$的*每个等价类*每个*$X_{\lambda}$中至多有一个元素；对于指标$(\lambda, \mu)$的每个对，令$A_{\lambda \mu}$为元素$x$的$X_{\lambda}$由……组成的子集，其中有元素$y \in X_{\mu}$，其中属于至等价类共 $X$。显然，每个 $x \in A_{\lambda \mu}$ 对应都有一个独特的 $y \in A_{\mu \lambda}$，它与 $x$ mod $R$ 全等； 映射$h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$如此定义满足以下条件：

(i) 对于每个 $\lambda \in L$，$h_{\lambda \lambda}$ 是 $A_{\lambda \lambda} = X_{\lambda}$ 中的恒等映射。

(ii) 对于$L$的每个指标$(\lambda, \mu, \nu)$和每个$x \in A_{\lambda \mu} \cap A_{\lambda \nu}$，我们有$h_{\mu \lambda}(x) \in A_{\mu \nu}$和

$$
h_{\nu \lambda}(x) = h_{\nu \mu}(h_{\mu \lambda}(x)).
$$

*相反*，假设对于指标 $(\lambda, \mu)$ 中的每个对，我们给出了上述 (i) 和 (ii) $X_{\lambda}$ 和映射 $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ 满足条件的子集 $A_{\lambda \mu}$。首先，从应用于三元组$(\lambda, \mu, \lambda)$和$(\mu, \lambda, \mu)$的(ii)得出，$h_{\lambda \mu} \circ h_{\mu \lambda}$（分别$h_{\mu \lambda} \circ h_{\lambda \mu}$）是$h_{\lambda \lambda}$（分别$h_{\mu \mu}$）到$A_{\lambda \mu}$（分别$A_{\mu \lambda}$）的限制；因此，我们从 (i) 推断出 $h_{\lambda \mu}$ 和 $h_{\mu \lambda}$ 是 *双射*，它们互为倒数。现在令$R \{ x, y \}$为关系“存在$\lambda, \mu$使得$x \in A_{\lambda \mu}$、$y \in A_{\mu \lambda}$和$y = h_{\mu \lambda}(x)$”。从 (i) 和前面的内容可以得出，$R$ 是*自反*和*对称*；另一方面，如果 $x \in A_{\lambda \mu}$，

$$
y = h_{\mu \lambda}(x) \in A_{\mu \lambda} \cap A_{\mu \nu} \quad \text{and} \quad z = h_{\nu \mu}(y),
$$

然后还有 $x = h_{\lambda \mu}(y)$，因此，通过 (ii)，$x \in A_{\lambda \mu} \cap A_{\lambda \nu}$； 关系 (i) 因此表明 $R$ 是*传递*，因此 $R$ 是 $X$ 上的等价关系。从 (i) 和 $R$ 的定义还可以得出，每个等价类 mod $R$ 在集合 $X_\lambda$ 的每一个中至多有一个元素，并且 $A_{\lambda \mu}$ 是所有 $x \in X_\lambda$ 中的集合其中元素 $y \in X_\mu$ 与 $x$ mod $R$ 全等。我们说商集$X/R$是通过*$X_\lambda$*沿着*$A_{\lambda \mu}$*通过双射*$h_{\mu \lambda}$*粘贴在一起获得的。如果$\varphi : X \to X/R$是典范映射，则$\varphi$到每个$X_\lambda$的限制是$X_\lambda$的*双射*到$\varphi(X_\lambda)$。

现在假设每个$X_\lambda$是一个*拓扑空间*，并令$\mathfrak{T}_\lambda$为其拓扑。令$\mathfrak{T}$为集合$X/R$上最好的拓扑，其中映射$\varphi \circ j_\lambda$是连续的； $\mathfrak{T}$ 是$X$ 上拓扑与$R$ 的商，即拓扑$\mathfrak{T}_\lambda$ 的*和*。我们说拓扑空间$X/R$（与拓扑$\mathfrak{T}$）是通过*将拓扑空间*$X_\lambda$*沿着*$A_{\lambda \mu}$*通过双射*$h_{\mu \lambda}$粘贴在一起获得的。因此，$X/R$的*开*（或*闭*）子集是$X$的子集$B$的典范像，它们相对于$R$是*饱和*的，并且使得$B \cap X_\lambda$是*开*（或*闭*）每 $\lambda \in L$ $X_\lambda$。

由于$\varphi$的限制到每个$X_\lambda$都是双射到$X/R$的子集$X'_\lambda = \varphi(X_\lambda)$，我们可以通过这个方法将迁移拓扑$\mathfrak{T}_\lambda$到$X'_\lambda$ 双射，因此$X'_\lambda$携带拓扑$\mathfrak{T}'_\lambda$； $X/R$ 上的拓扑 $\mathfrak{T}$ 是典范嵌入 $X'_\lambda \to X/R$ 连续的*最佳*。一般来说，$\mathfrak{T}$在$X'_\lambda$上引起的拓扑比$\mathfrak{T}'_\lambda$“更粗糙”，但与后者不完全相同；即使$h_{\mu \lambda}$是同胚（§ 3，习题15）。然而，根据no. 4、命题 8，加上前面的记号：

#### 命题 9 {#top-i-s2-prop-9 .statement tag=0B0R}

*假设* $h_{\mu \lambda}$ *是同胚，并且每个* $A_{\lambda \mu}$ *都是开（或闭）* *在* $X_\lambda$中； *则每个* $\varphi(X_\lambda)$ *都是开（或闭）* *在* $X/R$ *和限制 of* $\varphi$ *到* $X_\lambda$ *是* $X_\lambda$ *到子空间* $\varphi(X_\lambda)$ *的同态$X/R$。

### 习题 {#top-i-s2-exercises}

§ 2](exercises/s2/)参见[习题。
