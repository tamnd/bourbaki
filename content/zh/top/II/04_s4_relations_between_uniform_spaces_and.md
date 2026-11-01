---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 4
section_title: Relations between uniform spaces and compact spaces
lang: zh
source: top-i-iv
book_pages: 198-205, 209-215
pdf_pages: 0204-0211, 0215-0221
extraction: ocr
subsections:
    - "no": 1
      title: UNIFORMITY OF COMPACT SPACES
      page: 198
      pdf_page: 204
    - "no": 2
      title: COMPACTNESS OF UNIFORM SPACES
      page: 201
      pdf_page: 207
    - "no": 3
      title: COMPACT SETS IN A UNIFORM SPACE
      page: 203
      pdf_page: 209
    - "no": 4
      title: CONNECTED SETS IN A COMPACT SPACE
      page: 204
      pdf_page: 210
statements: 24
exercises: 23
content_sha256: f799853dd54f05ca9a42427240aa009f85e945cf1a171a9632e6e1ac4c00f961
translated_from: content/en/top/II/04_s4_relations_between_uniform_spaces_and.md
translation_method: google
source_content_sha256: 8fbe729c6ee10e2d495404ad78d874cc6e622625944438ceb687c0daa2ce0e9f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 14f021be944e01a68e96535cf45c11e1e3e8b88a7cc62cb4f5d0cbd0971c8454
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 4. 关系介于均匀空间和紧凑空间之间

### 1. 紧凑均匀度空间

#### 定义 1 {#top-ii-s4-def-1 .statement tag=0BFX}

*拓扑上的均匀性空间$X$据说与$X$的拓扑兼容，如果后者由均匀性引起重合与拓扑。*

如果空间上存在与其拓扑兼容的均匀性，则称拓扑空间是可一致的，并且其拓扑也称为可一致的。

存在不可统一的拓扑空间，对于例任何不满足公理$(O_{III})$的空间（$§ 1$，no. 2，命题2的推论3）；因而，问题是确定在什么条件下拓扑空间是可统一的。

这个问题要等到章IX、$§ 1$才能给出完整的答案。在这个截面中，我们将只检查一个重要的特殊情况，其中$X$是紧的。然后我们有以下定理：

#### 定理 1 {#top-ii-s4-thm-1 .statement tag=0BFY}

*在紧凑的空间 $X$ 上，恰好有一个与 $X$ 的拓扑兼容的一致性；这种均匀性的周边都是$X \times X$对角的$\Delta$的邻域。而且，赋予这种均匀性的$X$就是完整的制服空间。*

定理的最后一个部分很简单；对于 $X$ 上的每个柯西滤波器都有一个簇点 [公理 (C)]，因此是收敛的（$§ 3$、no. 2、命题 5，推论 2）。

接下来让我们证明，如果$X$上存在与$X$的拓扑兼容的均匀性，则该均匀性的随从的集合$U$是$\Delta$的所有邻域中的集合。我们已经知道每个随行人员都是$\Delta$的邻域（$§ 1$，no. 2，命题2），因此我们必须反过来证明$\Delta$属于到$U$的每个邻域。假设$\Delta$中有邻域$U$不在$U$中；然后集合$V \cap C_U$，因为$V$穿过紧凑型空间$X \times X$上的过滤器$G$的$U$、形式基；因而$G$有一个集群点$(a, b)$而不是属于到$\Delta$。由于$U$是比$G$更粗糙的过滤器，因而$(a, b)$也是$U$的集群点。但$U$定义的均匀性是假设的Hausdorff；因而$U$的集合关闭的交是$\Delta$（$§ 1$，no. 2，推论2至命题2和命题3）；这样我们就产生了矛盾。

因而，还需要证明$X \times X$中的$\Delta$邻域集合$B$是与$X$的拓扑兼容的一致性的集合。为此，足以证明 $B$ 是 $X$ 上 *Hausdorff* 均匀性的集合；因为由这种均匀性引起的拓扑将比$X$的拓扑*粗糙*（章I，$§ 2$，no. 2，命题3），因此必须重合与后者（章I、$§ 9$、no. 4、定理2、推论 3）。

$B$显然满足公理$(F_I)$和$(F_{II})$。让我们证明公理$(U_{II})$和$(U_{III})$也满足，并且$\Delta$是$B$的集合的交。首先取最后一个点：单个点$(x, y) \in X \times X$的每个集合由……组成都是闭的，因为$X$是Hausdorff；因此，如果$x \neq y$，$X \times X$中$(x, y)$的补集是$\Delta$的邻域。由于对称性$(x, y) \to (y, x)$是$X \times X$自身的同胚，因此$V \in \mathfrak{B}$蕴涵$\overline{V}^1 \in \mathfrak{B}$、从而$(\mathbf{U}_{\mathrm{II}})$。最后，假设$(\mathbf{U}_{\mathrm{III}})$不满足；那么有集合 $V \in \mathfrak{B}$ 使得对于所有 $W \in \mathfrak{B}$ 集合 $\hat{W} \cap \mathscr{C}V$ 不为空； 集合$\hat{W} \cap \mathscr{C}V$，因为$W$贯穿$\mathfrak{B}$，因此形式在$X \times X$上有一个过滤器基，并且这个过滤器基有一个集群点$(x, y)$不在$\Delta$。现在，由于$X$是*常规*（章I、no. 2，命题1的推论），$x$有不相交的开放邻域$U_1$和$U_2$ $y$，还有$x$和$y$的*关闭*邻域、$V_1 \subset U_1$、$V_2 \subset U_2$。令$U_3 = \mathscr{C}(V_1 \cup V_2)$，并考虑邻域

$$
W = \bigcup_{i=1,2,3} (U_i \times U_i) \text{ of } \Delta \text{ in } X \times X.
$$

从这些定义可以立即得出，如果$(u, v) \in W$和$u \in V_1$（或$u \in U_1$），那么我们必须有$v \in U_1$（或$v \in U_1 \cup U_3 = \mathscr{C}V_2$）；因此$X \times X$中$(x, y)$的邻域$V_1 \times V_2$不满足$\hat{W}$，我们就有了矛盾。这样就完成了证明。

#### 注 1 {#top-ii-s4-n1-rem-1 .statement tag=0BFZ}

对于每个*有限的开放覆盖* $\mathscr{R} = (U_i)_{1 \leq i \leq n}$ of $X$, 集合

$$
V_{\mathscr{R}} = \bigcup_{i=1}^n (U_i \times U_i)
$$

is a neighbourhood of $\Delta$ in $X \times X$, and these sets $V_{\mathscr{R}}$ form a *fundamental system of neighbourhoods* of $\Delta$ (and therefore a *fundamental system of entourages* of the unique uniformity on $X$). 令$W$为$X \times X$中$\Delta$的任意邻域；那么对于每个$x \in X$，$X$中有一个$x$的开邻域$U_x$，使得$U_x \times U_x \subset W$。 由于 $U_x$ ($x \in X$) 形式是 $X$ 的开覆盖，因此存在点 $x_i$ ($1 \leq i \leq n$) 的有限数，使得$U_{x_i}$ ($1 \leq i \leq n$) 形式是一个覆盖$\mathscr{R}$ 共 $X$。 然后我们有$V_{\mathscr{R}} \subset W$，它证明了断言。

因此，$X$ 上的唯一均匀性通常称为“有限开覆盖​​的均匀性”（cf. 章 IX, § 4、习题 17）。

#### 推论 1 {#top-ii-s4-thm-1-cor-1 .statement tag=0BG0}

*紧致空间的每个子空间都是可均匀化的。*

#### 推论 2 {#top-ii-s4-thm-1-cor-2 .statement tag=0BG1}

*每个局部紧凑空间都是可统一的。*

对于 Alexandroff 的定理 (章 I, § 9, no. 8, 定理 4)，局部紧致空间同胚于紧致空间的子空间。

#### 注 2 {#top-ii-s4-n1-rem-2 .statement tag=0BG2}

可能存在与局部紧凑空间的拓扑兼容的几种不同的一致性。

对于例，我们已经看到，在无限离散的空间上，存在多个与离散的拓扑（§ 2, no. 2，注）兼容的明显均匀性。

然而，与可均匀化空间的拓扑兼容的均匀性的唯一性不是表征紧凑空间的性质；存在局部紧致空间，它们不是紧致的，但其均匀性是唯一的（习题4）。

#### 定理 2 {#top-ii-s4-thm-2 .statement tag=0BG3}

将紧致空间 $X$ 变为均匀空间 $X'$ 的每个连续映射 $f$ 都是均匀连续的。

设$g = f \times f$，则$g$在$X \times X$上连续（章I, § 4, no. 1，命题1，推论1）；因此，对于$X'$的每个开环$V'$，$\overline{g^{-1}}(V')$是$X \times X$的开子集，显然是包含对角线。因此，定理源自定理1，因为$X'$形式的开放随从是随从的基本系统（§ 1, no. 2，命题2，推论2）。

在定理2假设下，$f$的限制到$X$的任意子空间$A$一致连续；因此（§ 3, no. 6，定理2）：

#### 推论{#top-ii-s4-n1-cor-1 .statement tag=0BG4}

令$A$为紧凑空间$X$的稠密子空间，并令$f$为$A$的映射，形成完整的豪斯多夫均匀空间$X'$。那么$f$可以通过连续性扩展到整个$X$当且仅当$f$一致连续。

### 2. 均匀的紧凑性空间

#### 定义 2 {#top-ii-s4-def-2 .statement tag=0BG5}

如果一致的空间 $X$ 是预紧的，如果它的 Hausdorff 完备的$\hat{X}$ 是紧的。如果 $X$ 的制服子空间 $A$ 是预紧的，则制服空间 $X$ 的子集 $A$ 被称为预紧子集。

因此，均匀空间 $X$ 的子集 $A$ 是预紧的，当且仅当 $\hat{X}$ 中的 $i(A)$ 的闭包是紧的（$i : X \to \hat{X}$ 是规范的映射）（§ 3, no. 9，命题 18，推论 1）。

#### 例 {#top-ii-s4-n2-exa-1 .statement tag=0BG6}

在任何制服空间$X$中，柯西序列$(x_n)$的点的集合是预紧的。由于$\hat{X}$中$x_n$的像再次形式是柯西序列，我们可以假设$X$是Hausdorff； 点 $x_n$ 集合的$\hat{X}$ 中的闭包则由点 $x_n$ 和 $\lim_{n \to \infty} x_n$ 组成，因此是紧凑的 (章 I, § 9, no. 3, 例 2)。

#### 定理 3 {#top-ii-s4-thm-3 .statement tag=0BG7}

统一的空间$X$是预紧的当且仅当对于$X$的每个随行人员$V$，$X$被$V$小集合有限覆盖。

我们可以用说更直观地表达条件，$X$可以被集合的有限数覆盖，它尽可能小。

令$i : X \to \hat{X}$为典范映射，则$X$的随从是$\hat{X}$随从的$i \times i$下的逆像（§ 3, no. 7，命题12）。 假设$X$是预紧的，并令$U$是$\hat{X}$的任意随行；那么存在 $\hat{X}$ 的对称周边$U'$，使得 $\hat{U}' \subset U$。 由于$\hat{X}$是紧致的，因此存在点$x_j \in \hat{X}$的有限数，使得$U'(x_j)$（$U$小）覆盖$\hat{X}$。 如果$V$是$U$的逆像乘以$i \times i$，则集合$i^{-1}(U'(x_j))$是$V$小并覆盖$X$。 相反，假设对于$X$的每个随行人员$V$，$V$-小集合有限地覆盖$X$。 我们必须证明$\hat{X}$上的每个超滤器$\mathfrak{F}$都是收敛的；由于$\hat{X}$是完整的，因此足以证明$\mathfrak{F}$是一个*柯西滤波器*，即对于$\hat{X}$的每个*封闭*随行$U$，$\mathfrak{F}$中有一个$U$-小集合（§ 1, no. 2，命题2，推论2）。 令$V$为$i \times i$下$U$的逆像，令$(B_j)$为$V$-小集合对$X$的有限覆盖；那么集合$C_j = i(B_j)$是$U$小并覆盖$i(X)$，这样
$$
\hat{X} = \bigcup_j \overline{C}_j.
$$
另一方面，由于$C_j \times C_j \subset U$和$U$在$\hat{X} \times \hat{X}$中闭合，我们有$\overline{C}_j \times \overline{C}_j \subset U$，因此$\overline{C}_j$也是$U$小。 由于$\mathfrak{F}$是超滤器，$\overline{C}_j$属于到$\mathfrak{F}$之一（章I, § 6, no. 4，命题5的推论）。

Q.E.D.

#### 推论{#top-ii-s4-n2-cor-1 .statement tag=0BG8}

*一致的空间$X$是紧的当且仅当它是豪斯多夫且完整的并且可以被$V$-小集合的有限数覆盖，其中$V$是$X$的任何随行。*

这是从 no. 1 的定理 3 和定理 1 得出的。

#### 注 1 {#top-ii-s4-n2-rem-1 .statement tag=0BG9}

非豪斯多夫 *拟紧* 空间不一定是可一致的，因为它不需要满足公理 $(O_{III})$ (cf. 章 I, § 9, no. 2)；对于例，代数几何中出现的大多数非豪斯多夫拟紧空间不存在满足公理$(O_{III})$（cf.习题2）。

#### 命题 1 {#top-ii-s4-prop-1 .statement tag=0BGA}

*在统一空间中，预紧式集合的每个子集，预紧式集合的每个有限并以及每个预紧式集合的闭包都是预紧式。*

前两个断言是定理3的直接的推论。令$X$为均匀空间，$A$为$X$的预紧子集，令$i : X \to \hat{X}$为典范映射。 $i(\overline{A})$包含在$\hat{X}$中$i(A)$的闭包中（章I, § 2, no. 1，定理1），因此$\hat{X}$中的$i(\overline{A})$闭包包含在紧集中，因此是紧凑的。

#### 注 2 {#top-ii-s4-n2-rem-2 .statement tag=0BGB}

在统一的空间$X$中，*相对紧凑*集合$A$是*预紧凑*，因为$A$包含在紧集中。另一方面，即使$X$是Hausdorff，$X$中的预紧集*不需要相对紧*，如$X$本身是预紧但不紧的情况所示。

#### 命题 2 {#top-ii-s4-prop-2 .statement tag=0BGC}

*令$f : X \to Y$为均匀连续的映射。如果 $A$ 是 $X$ 的任何预紧式子集，则 $f(A)$ 是 $Y$ 的预紧式子集。*

因为如果$i : X \to \hat{X}$和$j : Y \to \hat{Y}$是典范映射，我们有$j(f(A)) = \hat{f}(i(A))$（§ 3, no. 7，命题15），因此$j(f(A))$在$\hat{Y}$中相对紧凑（章I, § 9, no. 4， 定理 2，推论 1)。

#### 命题 3 {#top-ii-s4-prop-3 .statement tag=0BGD}

*令$X$为集合，令$(Y_\lambda)_{\lambda \in L}$为制服空间的族，对于每个$\lambda \in L$，让$f_\lambda$为$X$到$Y_\lambda$的映射。令 $X$ 具有最粗糙的均匀性，使得 $f_\lambda$ 均匀连续。那么 $X$ 的子集 $A$ 是预紧的，当且仅当对于每个 $\lambda \in L$，$f_\lambda(A)$ 是 $Y_\lambda$ 的预紧子集。*

由于命题 2，条件是必要的。充分性源自 § 3, no. 9、命题 18 中给出的 $X$ 的 Hausdorff 完成的刻画，以及吉洪诺夫的定理 (章) I, § 9，定理 3，推论）。

### 3. 紧集制服空间

对于任意均匀的空间，以下命题是紧凑空间的章I, § 9, no. 2的命题2的更锐利的形式。

#### 命题 4 {#top-ii-s4-prop-4 .statement tag=0BGE}

*在统一的空间$X$中，令$A$为紧集，并且$B$是一个封闭的集合，使得$A \cap B = \varnothing$。然后存在 $X$ 的随行人员 $V$，使得 $V(A)$ 和 $V(B)$ 不相交。*

如果命题为假，则集合$A \cap \overline{V}(B)$（其中$V$贯穿$X$的对称周边的集合）都不会是空的；因此，这些集合将形式过滤器基在$A$上，其中将有一个集群点$x_0 \in A$。因此，对于$X$的每个对称周边$V$，$\overline{V}(x_0)$将满足$B$，因此，当$B$闭合时，我们应该有$x_0 \in B$，与假设相反。

#### 推论{#top-ii-s4-n3-cor-1 .statement tag=0BGF}

*令$A$为紧集，穿着制服空间$X$；那么当$V$穿过$X$随行人员的集合时，集合$V(A)$形式$A$的邻域的基本系统。*

设$U$为$A$的任意开邻域，则$B = \complement U$闭且不满足$A$；因此，到命题 4 时，有一个随从 $V$ 使得 $V(A) \cap V(B) = \varnothing$，因此有 $V(A) \subset U$。

### 4. 连接集合，紧凑空间

#### 定义 3 {#top-ii-s4-def-3 .statement tag=0BGG}

*令$V$为制服空间$X$的对称随行人员。如果$x_i$和$x_{i+1}$对于$0 \leq i < n$来说是$V$闭，则$X$的点有限序列$(x_i)_{0 \leq i \leq n}$被称为$V$链。 点 $x_0$ 和 $x_n$ 被称为 $V$ 链的末端，据说它们由 $V$ 链连接。*

给定一个对称的周边$V$，关系“有一个$V$链连接$x$和$y$”是$X$中$x$和$y$之间的等价关系。对于这个关系，令$A_{x, v}$为$x$的等价类，即所有$y \in X$的集合，可以通过$V$链连接到$x$。显然，如果$y \in A_{x, v}$则$V(y) \subset A_{x, v}$；因此$A_{x, v}$在$X$开放；并且$A_{x, v}$的补集，即等价类的并，也是开的。因此：

#### 命题 5 {#top-ii-s4-prop-5 .statement tag=0BGH}

*在统一的空间$X$、点的集合$A_{x, v}$中，可以通过$V$链连接到给定的点$x$，在$X$中既开又闭。*

For each $x \in X$, let $A_x$ denote the intersection of the sets $A_{x, v}$ as $V$ runs through the set of symmetric entourages of $X$; $A_x$ is the equivalence class of $x$ for the equivalence relation "for all symmetric entourages $V$, there is a $V$-chain joining $x$ and $y$".

#### 命题 6 {#top-ii-s4-prop-6 .statement tag=0BGI}

*在紧凑的空间$X$中，$x$、集合$A_x$和$x$的邻域的交都是开闭的，这三个部分都是相同的。*

足以证明$A_x$是*连通的*：因为在任何制服空间$X$中，$x$的分量包含在$x$的邻域的交中，它们都是开闭的，并且这个交包含在$A_x$中命题5。

假设 $A_x$ 未连接。由于$A_x$是*闭*的，因此有两个非空不相交的闭集合$B$和$C$，使得$B \cup C = A_x$。到§ 3的命题 4时，有$X$的随行人员$U$，因此$U(B) \cap U(C)$为空。

令$W$是一个*开放*随行人员，使得$\hat{W} \subset U$，并让$H$是*封闭*集合，它是$X$中$W(B) \cup W(C)$的补集。假设例为$x \in B$，并令$y$为点除以$C$。然后，对于每个对称的随从$V \subset W$，我们可以立即看到，通过$i$上的归纳，每个连接$X$中的$x$和$y$的$V$链$(x_i)_{0 \leq i \leq n}$必须有点 $H$，由 $W$ 的选择。由于假设$x$和$y$可以通过每个对称周边$V$的$V$链连接，我们看到如果$V \subset W$则$H \cap A_{x, v}$不为空。另一方面，如果 $V' \subset V$ 则显然 $A_{x, v'} \subset A_{x, v}$；因此，当$V$穿过$X$对称周边的集合时，集合$H \cap A_{x, v}$形式在紧凑空间中*封闭*集合的过滤器基 $H$。因此，所有这些集合都有公共的点，因此$H$满足$A_x$；但这$H$的与……矛盾定义。

#### 推论 {#top-ii-s4-n4-cor-1 .statement tag=0BGJ}

*设 X 为局部紧致空间，令 K 为 X 的紧致分量。那么 K 的邻域既开又闭形式 K 的邻域的基本系统。*

令V为K在X（章I, § 9, no. 7，命题10）中的相对紧开邻域，并令F为其边界。令 U ⊂ \overline{V} 为集合，*相对于* \overline{V} 既开又闭。那么 U 在 X 中闭，如果在加法中 U 不满足 F，则 U 在 X 中开（因为此时 U ⊂ V 并且 U 在 V 中开）。因此，只要证明\overline{V}存在子集，其中包含K不满足F，并且相对于\overline{V}既开又闭。

假设情况并非如此：那么 F 的交和 \overline{V} 的子集其中包含 K 和 在 \overline{V} 中开闭形式 F 中闭集合的过滤器基； F 是紧的，所以这些集合有公共的点 y ∈ F。 但这是荒谬的；由于\overline{V}是紧的，K是\overline{V}的一个分量，并且凭借命题6，集合的交，其中包含K和在\overline{V}中都是开闭的。推论是证明了。

#### 命题 7 {#top-ii-s4-prop-7 .statement tag=0BGK}

*令X为紧致空间，令R为X上的等价关系，其中类是X的分量。那么商空间 X/R 是紧致的并且完全不连通。*

由章I、§II、no. 5、命题9可知X/R完全断开；因此我们必须证明 X/R 是 *Hausdorff* (章 I, § 10, no. 4, 命题 8.) 令 A 和 B 是 X 的两个不同分量。到命题 6 时，存在X 的对称周边 U，使得 A 的点不能通过 U 链连接到 B 的任何点。 X 的点的集合 V（分别为 W），可以通过 U 链连接到点 x ∈ A（分别为 y ∈ B），在 X (命题 5) 中既开又闭包含 A（分别为 B）；因此，这些集合分别是 A 和 B 的开邻域，相对于 R 饱和并且不相交。这样就完成了证明。

### 习题 {#top-ii-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
