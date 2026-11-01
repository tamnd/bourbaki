---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 9
section_title: Compact spaces and locally compact spaces
lang: zh
source: top-i-iv
book_pages: 83-97, 141-150
pdf_pages: 0089-0103, 0147-0156
extraction: ocr
subsections:
    - "no": 1
      title: QUASI-COMPACT SPACES AND COMPACT SPACES
      page: 83
      pdf_page: 89
    - "no": 2
      title: REGULARITY OF A COMPACT SPACE
      page: 85
      pdf_page: 91
    - "no": 3
      title: QUASI-COMPACTS SETS; COMPACT SETS; RELATIVELY COMPACT SETS
      page: 85
      pdf_page: 91
    - "no": 4
      title: IMAGE OF A COMPACT SPACE UNDER A CONTINUOUS MAPPING
      page: 87
      pdf_page: 93
    - "no": 5
      title: PRODUCT OF COMPACT SPACES
      page: 88
      pdf_page: 94
    - "no": 6
      title: INVERSE LIMITS OF COMPACT SPACES
      page: 89
      pdf_page: 95
    - "no": 7
      title: LOCALLY COMPACT SPACES
      page: 90
      pdf_page: 96
    - "no": 8
      title: EMBEDDING OF A LOCALLY COMPACT SPACE IN A COMPACT SPACE
      page: 92
      pdf_page: 98
    - "no": 9
      title: LOCALLY COMPACT $\sigma$-COMPACT SPACES
      page: 93
      pdf_page: 99
    - "no": 10
      title: PARACOMPACT SPACES
      page: 94
      pdf_page: 100
statements: 52
exercises: 29
content_sha256: d7f708c8d6ab185dcdb67c3e03d85ca6afe354e2d9b90b0e864c00aeecfbe483
translated_from: content/en/top/I/09_s9_compact_spaces_and_locally_compact.md
translation_method: google
source_content_sha256: 5bd050717f2292378262b65271babbb584eca08fd5d5c1237ffed7a2b1b60829
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 91f3e8b78472390f17cd993f3c4c61458879f3efb9af53ba7e7b3169e506e548
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 9. 紧凑空间和局部紧凑空间

### 1. 准紧凑型空间和紧凑型空间

#### 定义 1 {#top-i-s9-def-1 .statement tag=0B7S}

*拓扑空间* $X$ *如果满足以下公理，则称其为拟紧的*：

(C)*$X$*上的每个过滤器至少有一个簇点*。

*如果拓扑空间是拟紧且Hausdorff*，则称它是紧的。

从这个公理可以立即得出，如果$f$是集合$Z$的映射到准紧凑空间$X$，并且$\mathfrak{F}$是$Z$上的任何过滤器，那么$f$至少有一个簇点关于$\mathfrak{F}$。特别是，准紧空间的点的每一个序列都至少有一个簇点；但是这个条件不等于(C)(习题11)。

我们给出三个公理，每个公理*等价于公理* (C)：

(C') ** $X$ *上的每个超滤器都会收敛*。

(C') $\Longrightarrow$ (C)：如果$\mathfrak{F}$是$X$上的过滤器，则存在比$\mathfrak{F}$（§ 6, no. 4，定理 1）超过滤器更细。由于该超滤器收敛于点$x$，因此$x$是$\mathfrak{F}$的集群点。

(C) $\Longrightarrow$ (C')：如果超滤器有一个簇点，那么它会收敛到点（§ 7, no. 2，命题 4 的推论）。

如果$f$是集合$Z$的映射转化为准紧凑空间$X$，并且$\mathfrak{U}$是$Z$上的超滤器，则$f$至少有一个极限点相对于 $\mathfrak{U}$ (§ 6, no. 6, 命题 10)。

(C'') *每个闭族子集* $X$ *其交为空包含一个有限子族，其交为空*。

(C) $\Longrightarrow$ (C''): 设$\mathfrak{G}$是$X$的封闭子集和空交的族。如果 $\mathfrak{G}$ 的每个有限子族都有一个非空交，则 $\mathfrak{G}$ 生成是一个过滤器（§ 6, no. 2，命题 1），其集群为点 × 假设。这点属于至 $\mathfrak{G}$ 的所有集合（因为它们已关闭）；所以我们有矛盾。

$(C'') \implies (C)$：如果$(C)$为假，则$X$上有一个过滤器$\mathfrak{F}$，它没有集群点；因此，$\mathfrak{F}$形式的集合闭包，$X$的闭子集族与公理$(C'')$相矛盾。

$(C''')$（Borel-Lebesgue 公理） *每个开覆盖* $X$ *包含的有限开覆盖​​ $X$。

$(C''') \iff (C'')$ 通过服用补品。

如果 $X$ 是拟紧的，那么覆盖 $X$ 的 $\mathfrak{R}$ 的每个“局部有限”都是“有限”。对于$X$的每个点都有一个开邻域，它仅满足$\mathfrak{R}$的集合的有限数，并且由$(C''')$覆盖这些邻域的有限数 $X$。

#### 例 1 {#top-i-s9-n1-exa-1 .statement tag=0B7T}

每个*有限* 空间都是*拟紧的*，更一般地，每个空间其中只有有限个数的开集合都是准紧的。有限空间是紧致的，当且仅当它是离散的，因为有限 Hausdorff 空间是离散的（$§ 8$，no. 1，命题 3 的推论）。相反，*每个紧离散空间都是有限的*，因为单个点的空间集合由……组成是开路；因此空间由$(C''')$有限。

#### 例 2 {#top-i-s9-n1-exa-2 .statement tag=0B7U}

设$X$为集合，并给出$X$拓扑，其中闭集合为$X$，并且$X$的所有有限子集[子集的这个集合显然满足公理$§ 1$、no. 4的$(O'_1)$和$(O'_{II})$]。这样定义的拓扑空间是*准紧*。因为如果$(F_i)_{i \in I}$是$X$的闭族子集且交为空，那么$F_\alpha$对于某些$\alpha \in I$是有限的。令 $a_k$ ($1 \leq k \leq n$) 为 $F_\alpha$ 中的元素；那么通过假设，对于每个指标$k$，有指标$i_k \in I$，使得$a_k \notin F_{i_k}$；因此$F_{i_k}$（$1 \leq k \leq n$）和$F_\alpha$的交是空的，从而公理$(C'')$满足。如果 $X$ 是无限的，则它不是豪斯多夫。

#### 注 {#top-i-s9-n1-rem-1 .statement tag=0B7V}

拟紧（非豪斯多夫）空间主要用于拓扑在代数几何中的应用，很少在其他数学理论中出现，相反紧空间发挥着重要作用。

#### 定理 1 {#top-i-s9-thm-1 .statement tag=0B7W}

*设* $\mathfrak{F}$ *为准紧致空间* $X$ *上的滤波器，并让* $A$ *为* $\mathfrak{F}$的集群点的集合。 *然后每邻域*$A$*属于到*$\mathfrak{F}$。

令$V$为$A$的邻域，并假设$\mathfrak{F}$的每个集合都可能满足$\complement V$。 $\mathfrak{F}$ 集合交和 $\complement V$ 然后 $X$ 上的一个过滤器 $\mathfrak{G}$ 形式基； $X$是拟紧的，因此$\mathfrak{G}$至少有一个簇点$y$，而不是属于到$A$，因为$A$的邻域$V$不满足集合的一些$\mathfrak{G}$。但由于$\mathfrak{G}$比$\mathfrak{F}$*更细*，$y$也是$\mathfrak{F}$的簇点，这与假设相反。

#### 推论{#top-i-s9-n1-cor-1 .statement tag=0B7X}

为了使紧凑空间上的滤波器收敛，它具有单个集群点是必要且充分的。

必要性按§ 8, no. 1、命题 1；以上定理 1 就足够了。

### 2. 紧凑的规则性空间

#### 命题 1 {#top-i-s9-prop-1 .statement tag=0B7Y}

令 X 为 X 的紧凑空间、x 点。在阶中，由x的闭邻域形成的滤波器基B应该是x的邻域的基本系统，B的集合的交仅由x组成是充分必要的。

条件是必要的，因为 X 是 Hausdorff (§ 8, no. 1, 命题 1)。这是足够的，因为它表示 x 是 B 的唯一簇点；因此 B 通过 no. 1 的定理 1 的推论收敛到 x。

#### 推论{#top-i-s9-n2-cor-1 .statement tag=0B7Z}

每个紧凑空间都是正则。

因为根据公理 (Hi) (§ 8, no. 1, 命题 1) 可以得出，空间的任意点的所有闭邻域形成的滤波器基满足命题 1 的条件。

下面的命题将推论放大为命题1：

#### 命题 2 {#top-i-s9-prop-2 .statement tag=0B80}

令X为紧致空间，并令A、B为X的两个不相交的闭子集。则存在两个开集合 U、V，使得U ∩ V = ∅ 且A ⊂ U 和B ⊂ V。

假设结论是错误的。如果 A 的每个邻域 U 都满足 B 的每个邻域 V，则集合 U ∩ V 形式 X 上的过滤器基 B，因此有一个簇点 x ∈ X。现在x必须位于A中，因为如果y是X的任何点不在A中，则y的邻域和A的邻域不相交，因为X是规则的，因此y不能是B的簇点。类似地，x必须位于B中并且我们有矛盾。

这个命题有重要的推论，将在章IX, § 4中进行检查。

no. 1 的例 2 的非豪斯多夫拟紧空间 X 既不是满足公理 (O_{III})，也不是命题 2 中所述的更不必说性质，因为任意两个非空开这个空间的集合总是相交。

### 3. 准紧凑型集合； 紧集；相对紧集

#### 定义 2 {#top-i-s9-def-2 .statement tag=0B81}

如果子空间 A 是拟紧致（或紧致），则拓扑空间 X 的子集 A 被称为拟紧致（或紧致）集合。

拓扑空间$X$的子集$A$是拟紧集当且仅当$A$的每个覆盖$X$包含的*开集合是$A$的有限覆盖；这是从公理 $(C''')$ 得出的。在 Hausdorff 空间中，准紧的概念和紧集是相同的，因为每个子空间都是 Hausdorff。

#### 例 1 {#top-i-s9-n3-exa-1 .statement tag=0B82}

在拓扑空间$X$中，每个有限子集都是拟紧的； 空集和点中的每一个集合由……组成都是紧致的。

#### 例 2 {#top-i-s9-n3-exa-2 .statement tag=0B83}

在拓扑空间$X$中，令$(x_n)_{n \in \mathbf{N}}$为点的无限序列，收敛于点$a$；那么点$x_n$($n \in \mathbf{N}$)和$a$的集合$A$由……组成是拟紧的。因为如果$(U_i)$是$A$被$X$的开集合覆盖，那么$a \in U_x$对于一些指标$x$。 $U_x$是$a$的邻域，因此只有指标$n_k$的有限数使得$x_{n_k} \notin U_x$。对于每个指标$k$，令$i_k$为指标，使得$x_{n_k} \in U_{i_k}$；那么$U_x$和$U_{i_k}$形式是$A$的有限开覆盖​​。

#### 命题 3 {#top-i-s9-prop-3 .statement tag=0B84}

*拟紧致*（或*紧*）的每个闭子集 *空间都是拟紧*（或*紧*）。

这是公理$(C'')$的直接的推论，如果我们注，如果$A$在$X$中闭合，那么在$A$中闭合的每个集合在$X$中闭合。

#### 命题 4 {#top-i-s9-prop-4 .statement tag=0B85}

*Hausdorff 空间的每个紧凑子集都是封闭的。*

令$A$为Hausdorff空间$X$的紧子集，并令$x$为$\overline{A}$的任意点；我们必须证明$x \in A$。到假设，$x$的每个邻域都满足$A$，因此邻域在$X$诱导中过滤$x$的$\mathfrak{B}$，在$A$上过滤$\mathfrak{B}_A$； $A$ 是紧凑的从而 $\mathfrak{B}_A$ 有一个簇点 $y \in A$。由于过滤器$\mathfrak{B}$比$\mathfrak{B}_A$生成的$X$上的过滤器更粗糙（被视为$X$上的过滤器基），$y$也是$\mathfrak{B}$的集群点；因此$y = x$，因为$\mathfrak{B}$在$X$中收敛到$x$，并且$X$是豪斯多夫（§ 8, no. 1，命题1）。

#### 推论{#top-i-s9-n3-cor-1 .statement tag=0B86}

*在紧致空间* $X$ *子集* $A$ *是紧致当且仅当它闭于* $X$。

#### 命题 5 {#top-i-s9-prop-5 .statement tag=0B87}

*拓扑空间的有限拟紧族子集的并是拟紧的。*

足以证明，如果$A$和$B$是拓扑空间$X$的两个拟紧子集，则$A \cup B$是拟紧的。让$\mathscr{R}$覆盖$A \cup B$；那么$\mathscr{R}$是$A$的覆盖和$B$的覆盖；因此 $\mathscr{R}$ 包含于 $A$ 的有限覆盖 $\mathscr{R}_1$ 和 $B$ 的有限覆盖 $\mathscr{R}_2$；因此，$\mathscr{R}_1 \cup \mathscr{R}_2$ 是$\mathscr{R}$ 中包含的$A \cup B$ 的有限覆盖。

#### 定义 3 {#top-i-s9-def-3 .statement tag=0B88}

*子集* $A$ *拓扑空间* $X$ *据说是相对拟紧*（分别为*相对紧*）*在* $X$ *如果* $A$ *包含在准紧*（分别为*紧*）*子集*中$X$。

简而言之，当$X$没有歧义时，我们还说$A$是“相对拟紧集”（分别是“相对紧集”）。在*Hausdorff* 相对拟紧集的空间概念和相对紧集是相同的。

#### 命题 6 {#top-i-s9-prop-6 .statement tag=0B89}

*如果$X$是豪斯多夫空间，$X$的子集$A$是相对紧的当且仅当$\overline{A}$是紧的。*

如果$A$是相对紧致的，那么$\overline{A}$是由命题 4及其推论紧致的；反过来的含义是不言而喻的。

#### 命题 7 {#top-i-s9-prop-7 .statement tag=0B8A}

*如果$A$是拓扑空间$X$的相对准紧子集，则$A$上的每个过滤器基在$X$中都有一个簇点。*

对于如果$A \subset K$，其中$K$是$X$的拟紧子集，则$A$上的每个过滤器基在$K$中都有一个集群点。

如果没有 $X$ (习题 22) 上的限制，则此命题的逆命题无效。

#### 注 {#top-i-s9-n3-rem-1 .statement tag=0B8B}

在非 Hausdorff 空间中，紧集不需要闭集，并且它的闭包不需要是拟紧的 (习题 5)；两个紧集中的交不必是拟紧的 (习题 5)；两个紧集的并不必是紧凑的 (习题 5)。

### 4. 紧致空间下连续映射的像

#### 定理 2 {#top-i-s9-thm-2 .statement tag=0B8C}

*如果$f$是拟紧空间$X$到拓扑空间$X'$的连续映射，则集合$f(X)$是拟紧的。*

设$\mathscr{R}$是$X'$中开集合对$f(X)$的覆盖；那么 $\overline{f}^{-1}(\mathscr{R})$ 是 $X$ (§ 2, no. 1, 定理 1) 的开覆盖；因此，$\mathscr{R}$有有限子集$\mathscr{S}$，使得$(\mathscr{S} \overline{f})$覆盖$X$；但$\mathscr{S}$是$f(X)$的覆盖并且定理被证明。

#### 推论 1 {#top-i-s9-thm-2-cor-1 .statement tag=0B8D}

*设$f$是拓扑空间$X$到豪斯多夫空间$X'$的连续映射。那么 $X$ 中任意拟紧（或相对准紧）集合 $f$ 下的像是 $X'$ 中的紧（或相对紧）集合。*

#### 推论 2 {#top-i-s9-thm-2-cor-2 .statement tag=0B8E}

*准紧空间 $X$ 到 Hausdorff 空间 $X'$ 的每个连续映射 $f$ 都是闭集。如果 $f$ 也是双射，那么 $f$ 是同胚。*

这直接从 no. 3 的推论 1 和命题 4 得出。

特别是：

#### 推论 3 {#top-i-s9-thm-2-cor-3 .statement tag=0B8F}

*Hausdorff 拓扑比准紧凑空间的拓扑更粗糙，必须与后者重合。*

#### 推论 4 {#top-i-s9-thm-2-cor-4 .statement tag=0B8G}

*设$X$为拓扑空间，$R$为$X$上的豪斯多夫等价关系。*

a) *如果$X$中有一个拟紧集$K$满足每个等价类模$R$，则$X/R$是紧集，并且$K/R_K$到$X/R$的典范映射是同胚。*

b) *如果$K$也仅在一个点中满足每个等价类，则$K$是$X$相对于关系$R$* (§ 3, no. 5)的连续截面。

令$f$为典范映射$X \to X/R$中的限制至$K$。由于 $X/R$ 是 Hausdorff，因此从推论 1 可以得出 $X/R$ 是紧的，并且从推论 2 可以得出 $f$ 是闭的；因此，双射的$K/R_K \to X/R$与$f$相关联是同胚（§ 5, no. 2，命题3）。这涉及到a）； b) 紧随其后，因为我们现在有 $K/R_K = K$。

### 5. 乘积紧凑型空间

#### 定理 3（吉洪诺夫）{#top-i-s9-thm-3 .statement tag=0B8H}

*准紧致（或紧致）空间的每个乘积都是准紧致（或紧致）。相反，如果非空空间的乘积是准紧致（或紧致），则每个因子都是拟紧致（或紧致）。*

鉴于§ 8, no. 2、命题 7 中给出的 Hausdorff 乘积空间的刻画，足以证明断言对于准紧空间。如果 $X = \prod_{i \in I} X_i$ 是拟紧且非空，则 $X_i = \operatorname{pr}_i(X)$ 是准紧，因为定理 2 of no. 4。相反，假设$X_i$是准紧致的，并让$\mathfrak{U}$是$X$上的超滤器；那么对于每个$i \in I$，$\operatorname{pr}_i(\mathfrak{U})$是$X_i$（§ 6, no. 6，命题10）上的超滤波器基，因此根据公理（C'）收敛；因此$\mathfrak{U}$是收敛的（§ 7, no. 6，命题10的推论1），因此$X$是拟紧的。

#### 推论{#top-i-s9-n5-cor-1 .statement tag=0B8I}

*为了使拓扑空间的乘积的子集相对拟紧，其每个投影在相应的因子中相对拟紧是必要且充分的。*

必然性来自定理 2 of § 4。为了证明充分性，令$A$为$\prod_i X_i$的子集，这样，对于每个指标$i$，$\operatorname{pr}_i(A)$都包含在$X_i$的准紧子集$K_i$中；那么$A$包含在$\prod_i X_i$的准紧子集$\prod_i K_i$中。

### 6. 逆极限紧凑型空间

#### 命题 8 {#top-i-s9-prop-8 .statement tag=0B8J}

令$(X_\alpha, f_{\alpha\beta})$为由有向集合$I$索引的紧凑空间的逆系，使得对于每个$\alpha \in I$，$f_{\alpha\alpha}$为恒等映射。令 $X = \varprojlim X_\alpha$ 为逆极限且 $f_\alpha : X \to X_\alpha$ 典范映射 (§ 4, no. 4)。然后
a) $X$ 是紧凑的，对于每个 $\alpha \in I$ 我们有
$$
f_\alpha(X) = \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(X_\beta).
$$
b) *如果* $X_\alpha$ *都非空，则* $X$ *非空*。

$X$是$\prod_\alpha X_\alpha$的闭子空间（§ 8, no. 2，命题7，推论2），它由no. 5的定理3和no. 3的命题3压缩。其他断言是*集合理论*的推论，第1章。 III, § 7, no. 4，第。 1. 我们通过将$\mathscr{S}_\alpha$取为$X_\alpha$的闭合子集的集合来应用此定理。 条件 (i) 和 (ii) 分别是公理 $(O'_1)$ 和 $(C'')$；由于$\{x_\alpha\}$是闭集且$f_{\alpha\beta}$连续（§ 2, no. 1，定理1），因此条件（iii）得到满足，最后，由于no. 4的定理2的推论2，条件（iv）得到满足。

#### 推论 1 {#top-i-s9-prop-8-cor-1 .statement tag=0B8K}

*令* $(X_\alpha, f_{\alpha\beta})$ *为由有向集合索引的拓扑空间的逆系，使得对于指标*$\alpha, \beta$的每个对*对于其中*$\alpha \leq \beta$*以及对于每个*$x_\alpha \in X_\alpha$， $\overline{f}_{\alpha\beta}^{-1}(x_\alpha)$ *紧凑*。 *则方程 (1) 有效，并且* $\overline{f}_{\alpha}^{-1}(x_\alpha)$ *对于每个指标* $\alpha$ *和每个* $x_\alpha \in X_\alpha$ 都是紧凑的。

对于每个$x_\alpha \in \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(X_\beta)$和每个$\beta \geq \alpha$，让$L_\beta$表示$\overline{f}_{\alpha\beta}^{-1}(x_\alpha)$。如果$\alpha \leq \beta \leq \gamma$，那么我们有$f_{\beta\gamma}(L_\gamma) \subset L_\beta$，并且所有指标$\beta \geq \alpha$中的集合在指标集合中是共尾的。紧接着拓扑空间的$L_\beta$ ($\beta \geq \alpha$) 形式逆系（$f_{\beta\gamma}$的限制为映射），其逆极限$L$同胚于$\overline{f}_{\alpha}^{-1}(x_\alpha)$。由于到假设时，$L_\beta$ 是紧致的且不为空，因此推论由命题 8 得出。

#### 推论 2 {#top-i-s9-prop-8-cor-2 .statement tag=0B8L}

*设*$(X_\alpha, f_{\alpha\beta})$*和*$(X'_\alpha, f'_{\alpha\beta})$*为由相同有向集合*$I$索引的拓扑空间的两个逆系，*并让*$(u_\alpha)$*为映射*的逆系 $u_\alpha : X_\alpha \to X'_\alpha$。 *让*$X = \varprojlim X_\alpha$，$X' = \varprojlim X'_\alpha$，$u = \varprojlim u_\alpha$。 *然后*：
a) *如果* $x' = (x'_\alpha) \in X'$ *使得* $\overline{u'}_{\alpha}^{-1}(x'_\alpha)$ *对于每个* $\alpha \in I$ *是紧凑且非空的，*则* $\overline{u}^{-1}(x')$ *是紧凑且非空*。

b) *如果 $X_\alpha$ 是紧致的，$X'_\alpha$ Hausdorff 和 $u_\alpha$ 满射且连续，则 $u$ 是满射。*

设$L_\alpha$表示$\overline{u}_\alpha^{-1}(x'_\alpha)$；那么显然拓扑空间的$L_\alpha$形式逆系（$f_{\alpha\beta}$的限制为映射），$\overline{u}^{-1}(x' = L)$是$L_\alpha$的逆极限；因此，断言 a) 由命题 8 得出。鉴于no. 3 的命题 3，断言 b) 为直接的推论。

### 7. 局部紧空间

#### 定义 4 {#top-i-s9-def-4 .statement tag=0B8M}

*拓扑空间$X$如果是豪斯多夫且$X$的每个点都有一个紧邻域，则称其为局部紧致。*

显然，紧致空间是局部紧致的，但逆命题是假的；对于例，每个*离散* 空间都是局部紧致的，但如果*无限*则不是紧致的。

\* 正如我们将在章 IV, § 2 中看到的，实直线 $\mathbf{R}$ 是局部紧致的，但不是紧致的。 \*

#### 命题 9 {#top-i-s9-prop-9 .statement tag=0B8N}

*每个局部紧凑空间都是正则的。*

令$X$为局部紧致空间，则每个点$x \in X$都有一个紧致邻域$V$；由于 $X$ 是 Hausdorff，$V$ 是闭集（no. 3，命题 4）。另一方面，$V$是$X$的正则子空间（no. 2，命题1的推论），因此$X$是正则（§ 8, no. 4，命题13）。

#### 推论{#top-i-s9-n7-cor-1 .statement tag=0B8O}

*在局部紧致空间中，每个点都有紧致邻域的基本系统。*

对于$x$的闭邻域和$x$的紧致邻域的交，是$x$的紧致邻域（no. 3，命题 3）。

存在*非豪斯多夫*拓扑空间，其中每个点都有紧致邻域（习题5）的基本系统。

命题 9 的推论可概括如下：

#### 命题 10 {#top-i-s9-prop-10 .statement tag=0B8P}

*在局部紧致空间$X$中，每个紧集$K$都有紧致邻域的基本系统。*

令$U$为$K$中的任意邻域。对于每个 $x \in K$，$U$ 中都有一个包含 $x$ 的紧凑邻域 $W(x)$。 集合的内饰

W(x) 形式当 x 穿过 K 时 K 的开覆盖；因此，存在点 $x_i \in K$ ($1 \leq i \leq n$) 的有限数，使得 W(x_i) 的内部覆盖 K。因此，W(x_i) 的并 V 是包含在 U (no. 3, 命题 5) 中的 K 的紧凑邻域。

#### 命题 11 {#top-i-s9-prop-11 .statement tag=0B8Q}

*令X为X的局部紧致空间和F子集，使得只要K是X的紧致子集，F \cap K就是紧致的。那么 F 在 X 中闭合。*

鉴于no. 3的命题4，这是从§ 3, no. 1的命题3a)得出的。

#### 命题 12 {#top-i-s9-prop-12 .statement tag=0B8R}

*在 Hausdorff 空间 X 中，每个局部紧致子空间 A 都是局部闭的。*

到假设，对于每个$x \in A$，X中存在x的邻域V，使得$V \cap A$是紧致的，因此在V（no. 3，命题4）中闭合。

#### 命题 13 {#top-i-s9-prop-13 .statement tag=0B8S}

*局部紧致空间X的每个局部闭子空间都是局部紧致的。*

设 A 为 X 的局部闭子空间；那么对于每个$x \in A$，X中的x有邻域 U，使得$U \cap A$在U中闭。令$V \subset U$是X中x的紧凑邻域； $V \cap A = V \cap (U \cap A)$ 在 V 中闭合，因此是紧凑的（no. 3，命题 3）。由于$V \cap A$是A中x的邻域，所以结果得证（显然A是Hausdorff）。

定理 1 (no. 1) 和定理 2 (no. 4) 的推论 2 *不要扩展* 到局部紧凑的空间，因为空间不是紧凑的。

对于例，在无限离散空间X中，那些集合的滤波器由……组成，其中包含给定点$x \in X$并且具有有限补集，将x作为其唯一簇点，但不收敛于x。由于 X 的任何映射 f 进入 Hausdorff 空间 X' 都是连续的，因此 X 的任意子集的 f 下的像（在 X 中是闭集，因为 X 是离散的）通常不会是闭集子集共 X'。

no. 5中的命题相应的到定理3如下：

#### 命题 14 {#top-i-s9-prop-14 .statement tag=0B8T}

a) *令 $(X_i)_{i \in I}$ 为局部紧致空间族，使得 $X_i$ 对于除了指标的有限数以外的所有成员都是紧致的。那么乘积空间 $X = \prod_{i \in I} X_i$ 是局部紧致的。*

b) *相反，如果非空拓扑空间的族 $(X_i)_{i \in I}$ 的乘积是局部紧致的，则因子 $X_i$ 对于除指标的有限数之外的所有元素都是紧致的，并且非紧致的因子是局部紧致的。*

a) 设$x = (x_i)$为$X$的点。对于每个指标$i \in I$，使得$X_i$是局部紧致但不是紧致的，让$V_i$是$X_i$中$x_i$的紧致邻域，并且对于所有其他指标$i$放置$V_i = X_i$。那么$\prod_{i \in I} V_i$是$X$中$x$的紧邻域（no. 5，定理3）。另外 $X$ 是 Hausdorff by , no. 2, 命题 7，因此是局部紧致的

b) 如果$X = \prod_{i \in I} X_i$是局部紧致的且$X_i$非空，则每个$X_i$同胚于$X$的闭子空间（$§ 4$、no. 2、命题 4和$§ 4$、no. 3，推论命题 7)，因此局部压缩命题 13。 令$a = (a_i)$为$X$的点，并令$V$为$a$的紧致邻域；因为除了指标 ($§ 4$, no. 1) 的有限数之外，我们都有 $\operatorname{pr}_i V = X_i$，所以从no. 4，推论 1 到定理 2，$X_i$ 都是紧的，除了有限的数之外指标。

### 8. 将局部紧致空间嵌入紧致空间

#### 定理 4（亚历山德罗夫）{#top-i-s9-thm-4 .statement tag=0B8U}

*如果$X$是任意局部紧致空间，则存在紧致空间$X'$和$X$的同态$f$到$X'$中点的补集。此外，如果$X'_1$是另一个紧空间，使得$X$的同态$f_1$到$X'_1$中点的补集，那么$X'$到$X'_1$有唯一的同态$g$这样 $f_1 = g \circ f$.*

让我们从证明定理的第二个断言开始。 让
$$
f(X) = X' - \{ \omega \} \quad \text{and} \quad f_1(X) = X'_1 - \{ \omega_1 \}.
$$
如果同态$g$存在，它一定是唯一的，因为到定义，如果$x' \neq \omega$，我们有$g(x') = f_1(\overline{f}(x'))$，因此有$g(\omega) = \omega_1$。 仍有待证明由此定义的双射 $g : X' \to X'_1$ 是双连续的；由于$X'$和$X'_1$可以互换，我们只需证明点$x' \in X'$的邻域$g$下的像是$X'_1$中$g(x')$的邻域。 这从 $g$ if $x' \neq \omega$ 的定义可以明显看出。 如果$x' = \omega$，则令$V'$为$\omega$在$X'$的开邻域；那么 $X' - V' = K$ 在 $X'$ 中闭合，因此是紧凑的 (no. 3, 命题 3) 并且包含在 $f(X)$ 中；因此 $g(K) = f_1(\overline{f}(K))$ 是紧致的（no. 4，定理 2，推论 1）。 由此可知 $g(V') = X'_1 - g(K)$ 是 $\omega_1$ (no. 3, 命题 4) 的开邻域。 因此 $g$ 是同胚。

为了证明定理的第一个部分，令$X'$为集合，即$X$的和和单个点$\omega$的集合由……组成。我们在$X'$上进行定义拓扑，取$X'$的开放子集的集合$\mathscr{O}$，由$X$的所有开放子集和形式的所有子集组成$(X - K) \cup \{ \omega \}$，其中$K$是$X$的紧致子集。由于 $X$ 的紧致子集的任何交都是紧致的（no. 3、命题 3 和 4），并且由于紧集的任何闭闭子集都是紧致的（no. 3、命题 3），因此有$\mathfrak{D}$满足公理$(O_I)$；并且由于 $X$ 的紧致子集的任何有限并都是紧致的 (no. 3, 命题 5)，因此 $\mathfrak{D}$ 也满足 $(O_{II})$。 $X$ 的每个紧凑子集在$X$（no. 3，命题 4）中闭合，因此由 $X'$ 在$X$ 诱导的拓扑是$X$ 上的原始拓扑。因此，仍然需要证明 $X'$ 是紧的。首先，$X'$ 是 *Hausdorff*。因为如果$x, y$是$X$中任意两个不同的点，则它们分别在$X$中开不相交的、邻域、$V, W$，并且在$X'$中开$V, W$；另一方面，每个$x \in X$在$X$中有一个紧凑的邻域$K$，它也是$X'$中$x$的邻域，而

$$
(X - K) \cup \{ \omega \}
$$

是$X'$中$\omega$的邻域，显然不满足$K$。最后，$X'$是*准紧*。设$(U_\lambda)_{\lambda \in L}$是$X'$的开覆盖；那么对于至少一个指标$\mu \in L$，我们有$U_\mu = (X - K_\mu) \cup \{ \omega \}$，其中$K_\mu$是$X$的紧凑子集。因此，$L$有有限子集$H$，使得集合$U_\lambda$（对于$\lambda \in H$）覆盖$K_\mu$；如果$J = H \cup \{ \mu \}$，则$(U_\lambda)_{\lambda \in J}$是$X'$的有限开覆盖​​，并且证明是完备的。

请注意，如果 $X$ 已经是*紧致*，则 $\omega$ 是紧致空间 $X'$ 的*孤立* 点；因此$X'$是空间$X$和空间$\{ \omega \}$的*和*（$\S$2，no. 4，例3）。

当按上述方式从局部紧致空间 $X$ 通过邻接元素 $\omega$ 构建紧致空间 $X'$ 时，通常会说 $\omega$ 是 $X'$ 的“无穷远处的点”，并且 $X'$由 $X$ 通过在无穷远处邻接点获得。 $X'$ 也称为局部紧致空间 $X$ 的 *Alexandroff 紧致化* 或 *单点紧致化*。

\* 例。如果我们将 Alexandroff 的定理应用于实平面 $\mathbf{R}^2$，我们会得到一个紧致的空间同胚于球体 $S_2$，其方程为 $\mathbf{R}^3$ 中的 $x_1^2 + x_2^2 + x_3^2 = 1$。这两个空间的同胚可以描述如下：与$\mathbf{R}^2$邻接的点$\omega$（无穷远点）映射到$(0, 0, 1) \in S_2$，$\mathbf{R}^2$的每个点$(x_1, x_2)$映射到点，$\mathbf{R}^3$中连接点、$(0, 1, 1)$和$(x_1, x_2, 0)$的线再次与$S_2$相交。这种同胚被称为*立体投影*。

### 9. 局部紧凑 $\sigma$-紧凑空间

#### 定义 5 {#top-i-s9-def-5 .statement tag=0B8V}

*局部紧致空间 $X$ 被称为 $\sigma$ 紧致或无穷大可数，如果它是紧致子集的可数并。*

#### 例 1 {#top-i-s9-n9-exa-1 .statement tag=0B8W}

离散空间是 $\sigma$ 紧的当且仅当它是可数的。

#### 例 2 {#top-i-s9-n9-exa-2 .statement tag=0B8X}

\* 实直线 $\mathbf{R}$ 是局部紧致和 $\sigma$-紧致，因为它是 $n \in \mathbf{N}$ 的紧致区间 $[ -n, +n ]$ 的并。 \*

#### 注 {#top-i-s9-n9-rem-1 .statement tag=0B8Y}

Hausdorff 空间可以是紧致子空间的可数并，而不是局部紧致。 \* 例是希尔伯特空间与弱拓扑，我们将在后面的卷中展示。

#### 命题 15 {#top-i-s9-prop-15 .statement tag=0B8Z}

*如果$X$是局部紧致$\sigma$紧致空间，则$X$的相对紧致开子集有序列$(U_n)$覆盖$X$，使得每个$\overline{U}_n \subset U_{n+1}$ $n$。

令 $X$ 为序列 $(K_n)$ 紧集中的并。令$U_1$为$K_1$（no. 7，命题10）的相对紧开邻域，并归纳定义$U_n$，使$n > 1$为邻域的相对紧紧开邻域 $\overline{U}_{n-1} \in K_n$（no. 3、命题 5；no. 7、命题 10）。 序列 $(U_n)$ 显然具有所需的属性。

#### 推论 1 {#top-i-s9-prop-15-cor-1 .statement tag=0B90}

*对于命题 15 的记号，$X$ 的每个紧凑型子集 $K$ 都包含在一些$U_n$ 中。

对于 $K$ 可以由 $U_k$ 的有限数覆盖，根据公理 (C''')。

#### 推论 2 {#top-i-s9-prop-15-cor-2 .statement tag=0B91}

*令$X$为局部紧致空间，并令$X'$为通过在无穷远$\omega$与$X$（no. 8）处邻接点而获得的紧致空间。那么$X$是$\sigma$紧的当且仅当点$\omega$在$X'$中具有邻域的可数基本系统。

If $X$ is $\sigma$-compact we can construct a sequence of subsets $U_n$ of $X$ as in Proposition 15, and the neighbourhoods $X' - \overline{U}_n$ of $\omega$ in $X'$ form a fundamental system of neighbourhoods of $\omega$ by reason of Corollary 1. 逆命题源自以下事实：$\omega$的开邻域的补集是$X$的紧子集。

显然，局部紧致$\sigma$紧致空间的每个闭子空间都是局部紧致和$\sigma$紧致。同样，局部紧致 $\sigma$-紧致空间的任何有限乘积都是局部紧致和 $\sigma$-紧致。

但请注意，紧致空间的开子空间不必是 $\sigma$ 紧致，如 Alexandroff 的定理 (no. 8, 定理 4) 所示。

### 10. 超紧凑型空间

#### 定义 6 {#top-i-s9-def-6 .statement tag=0B92}

*如果拓扑空间是 Hausdorff 并且满足以下公理，则称其为仿紧：

(PC) *$X$的每个开覆盖$\mathscr{R}$都有一个局部有限的开优化$\mathscr{R}'$。*
（集合理论，章II, § 4, no. 6，定义5）。

每个*紧* 空间显然都是仿紧的。每个*离散*空间$X$都是仿紧的，因为$X$的单个点的所有集合由……组成形成的开覆盖是局部有限的，并且比$X$的每个开覆盖都更细。

#### 命题 16 {#top-i-s9-prop-16 .statement tag=0B93}

*准紧致空间* $X$ *的每个闭子空间* $F$ *都是准紧致*。

当然$F$是豪斯多夫。另一方面，如果$(V_i)$是子空间$F$中的开覆盖，则每个$V_i$都是形式$V_i = U_i \cap F$，其中$U_i$在$X$中开。考虑$CF$和$U_i$形成的$X$的开覆盖$\mathscr{R}$；由于 $X$ 是仿紧的，$\mathscr{R}$ 具有局部有限细化 $\mathscr{R}'$，而交的 $F$ 为集合属于到 $\mathscr{R}'$ 形式 $F$ 的局部有限开覆盖，即更细比给定的覆盖$(V_i)$。

另一方面，紧致空间的开子空间不必是仿紧致 (习题 11)。

#### 命题 17 {#top-i-s9-prop-17 .statement tag=0B94}

*副紧致空间和紧致空间的乘积是副紧致*。

令$X$为仿紧致空间，$Y$为紧致空间，$\mathscr{R}$为$X \times Y$的开覆盖。对于每个$(x, y) \in X \times Y$，$X$中存在$x$的开邻域$V(x, y)$和$Y$中$y$的开邻域$W(x, y)$，使得$V(x, y) \times W(x, y)$包含在某些集合中属于至 $\mathscr{R}$。对于每个$x \in X$，集合$W(x, y)$，因为$y$穿过$Y$形式一个$Y$的开放覆盖；因此存在有限数点
$$
y_i \in Y \quad (1 \leq i \leq n(x))
$$
这样$W(x, y_i)$覆盖$Y$。让 $U(x)$ 表示
$$
\bigcap_{i=1}^{n(x)} V(x, y_i);
$$
那么每个开集合$U(x) \times W(x, y_i)$都包含在$\mathscr{R}$的集合中。现在让$(T_i)_{i \in I}$是$X$的局部有限开覆盖​​，它细化了$(U(x))_{x \in X}$的覆盖。对于每个$i \in I$，令$x_i$为$X$的点，使得$T_i \subset U(x_i)$，并让我们用$S_{i, k}$集合$W(x_i, y_k)$相应的来表示点$x_i$ （$1 \leq k \leq n(x_i)$）。明显集合
$$
T_i \times S_{i, k} \quad (i \in I, \ 1 \leq k \leq n(x_i) \text{ for each } i \in I)
$$
形式 $X \times Y$ 的开覆盖，它细化了 $\mathscr{R}$，如果我们证明这个覆盖是局部有限的，证明将是完整的。令$(x, y)$为$X \times Y$中的任意点； $x$的邻域$Q$只满足集合$T_i$的有限数，因此$(x, y)$的邻域$Q \times Y$只满足集合的有限数 $T_i \times S_{i, k}$。

另一方面，两个仿紧式空间的乘积不必是仿紧式（参见章 IX, , 习题 16）

#### 命题 18 {#top-i-s9-prop-18 .statement tag=0B95}

*和* (§ 2, no. 4, 例 3) *一个家族的* $(X_i)_{i \in I}$ *超紧致空间是超紧致*。

令$X$为$X_i$的和，并令$(V_\lambda)_{\lambda \in L}$为$X$的开覆盖。开口集合$X_i \cap Y_\lambda$形成的覆盖物是更细比$(V_\lambda)$。对于每个$i \in I$，令$(U_{i,\mu})_{\mu \in M_i}$是覆盖$(V_\lambda \cap X_i)_{\lambda \in L}$的局部有限开放细化；然后由 $X$ 形成的开口覆盖物

$$
U_{i,\mu} \quad (i \in I, \ \mu \in M_i \text{ for each } i \in I)
$$

是局部有限的并且细化了原始覆盖$(V_\lambda)$。

#### 定理 5 {#top-i-s9-thm-5 .statement tag=0B96}

*局部紧致空间* $X$ *是仿紧致当且仅当* $X$ *是局部紧致$\sigma$-紧致空间*族中的和。

假设$X$是仿紧的，对于每个$x \in X$，令$V_x$是$X$中$x$的相对紧开邻域。那么到假设时，存在$X$的局部有限开覆盖​​$(U(\alpha))_{\alpha \in A}$，它细化了$(V_x)_{x \in X}$。因此$U(\alpha)$相对紧凑。 $X$的每个紧致子集$K$仅满足集合$U(\alpha)$的有限数，对于非空集$U(\alpha) \cap K$形式，紧致空间$X$的局部有限开覆盖​​；因此它们在数 (no. 1) 中必定是有限的。现在让$R$是$X$的两个点$x, y$之间的关系：“$A$中存在指标的有限序列$(\alpha_i)_{1 \leq i \leq n}$，使得$x \in U(\alpha_1), \ y \in U(\alpha_n)$和$U(\alpha_i)$满足$U(\alpha_{i+1})$ 为 $1 \leq i \leq n - 1$”。

立即验证$R$是等价关系，并且每个等价类模$R$是$X$的*开*子集[因为$U(\alpha)$是开集合]。因此，$X$ 是由等价类 mod $R$ 形成的局部紧凑子空间（no. 7，命题 13）的 *和*，并且仍然需要证明这些子空间中的每一个都是 *可数* 子族的并家庭$(U(\alpha))$。

令$x$为$X$的任意点，以及$X$的相对紧开子集与$n$上的归纳的定义序列$(C_n)$如下； $C_1$是集合$U(\alpha)$中的并，其中包含$x$，并且对于每个$n > 1$，$C_n$是满足$C_{n-1}$的集合$U(\alpha)$中的并。 归纳在$n$上立即验证，每个$C_n$都相对紧凑，并且是集合$U(\alpha)$的*有限*数的并。此外，$x$相对于$R$的等价类是$C_n$的*并*：因为如果$(\alpha_i)_{1 \leq i \leq n}$是指标的序列，使得$x \in U(\alpha_1)$和$U(\alpha_i)$满足$U(\alpha_{i+1})$代表$1 \leq i \leq n - 1$，然后通过归纳在$i$看到$U(\alpha_i) \subset C_i$代表$1 \leq i \leq n$。由此可见，等价类 mod $R$ 是 $\sigma$ 紧的，这完成了定理的第一个部分的证明。

为了证明逆命题，我们可以假设（通过命题 18）$X$是$\sigma$紧。令$\mathfrak{R} = (G_\lambda)_{\lambda \in L}$为$X$的任何开覆盖，并令$(U_n)$为$X$中相对紧凑的开集合的序列，其具有no. 9的命题15中所述的性质。让$K_n$表示紧集$\overline{U}_n - U_{n-1}$（如果$n \leq 0$则为$U_n = \emptyset$）。开集合$U_{n+1} - \overline{U}_{n-2}$是$K_n$乘邻域乘构造；因此，对于每个$x \in K_n$，$x$中的邻域$W_x$包含在集合$G_\lambda$之一中，也包含在$U_{n+1} - \overline{U}_{n-2}$中。由于$K_n$是紧致的，集合$W_x$的有限数覆盖了$K_n$；让$H_{ni} (1 \leq i \leq p_n)$成为这些集合。那么集合$H_{ni} (n \geq 1, 1 \leq i \leq p_n \text{ for each } n)$的族$\mathfrak{R}'$是$X$的开放覆盖，它细化了$\mathfrak{R}$，因此要完成证明，我们必须证明$\mathfrak{R}'$是*局部有限的*。令$z$为$X$、$n$最小的整数中的任意点，使得$z \in U_n$；那么从$z \notin U_{n-1}$开始，$z$就有邻域$T$包含在$U_n$中且不满足$U_{n-2}$。由此可见，$T$仅满足那些集合$H_{mi}$，其中$n - 2 \leq m \leq n + 1$，即$T$仅满足$\mathfrak{R}'$的集合的有限数。

在证明的过程中，我们还得出了以下结果：

#### 推论 {#top-i-s9-n10-cor-1 .statement tag=0B97}

*令 $X$ 为局部紧致准紧致空间。那么$X$的每个开覆盖$\mathfrak{R}$都有一个由相对紧集组成的局部有限开细化$\mathfrak{R}'$。如果 $X$ 是 $\sigma$-紧，那么 $\mathfrak{R}'$ 可以被认为是可数的。*

### 习题 {#top-i-s9-exercises}

参见[习题为 § 9](exercises/s9/)。
