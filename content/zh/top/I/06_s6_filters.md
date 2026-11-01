---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 6
section_title: Filters
lang: zh
source: top-i-iv
book_pages: 57-68
pdf_pages: 0063-0074, 0135-0138
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A FILTER
      page: 57
      pdf_page: 63
    - "no": 2
      title: COMPARISON OF FILTERS
      page: 58
      pdf_page: 64
    - "no": 3
      title: BASES OF A FILTER
      page: 59
      pdf_page: 65
    - "no": 4
      title: ULTRAFILTERS
      page: 60
      pdf_page: 66
    - "no": 5
      title: INDUCED FILTER
      page: 61
      pdf_page: 67
    - "no": 6
      title: DIRECT IMAGE AND INVERSE IMAGE OF A FILTER BASE
      page: 62
      pdf_page: 68
    - "no": 7
      title: PRODUCT OF FILTERS
      page: 63
      pdf_page: 69
    - "no": 8
      title: ELEMENTARY FILTERS
      page: 64
      pdf_page: 70
    - "no": 9
      title: GERMS WITH RESPECT TO A FILTER
      page: 65
      pdf_page: 71
    - "no": 10
      title: GERMS AT A POINT
      page: 68
      pdf_page: 74
statements: 30
exercises: 20
content_sha256: 4b1f60f8b0afbb8b98fdf750a2f395aa389f66075713fe31f00c3dc8af708fab
translated_from: content/en/top/I/06_s6_filters.md
translation_method: google
source_content_sha256: a165a0f76eeee4bd4e5a4290b8617a33d4316a02017e4b95b814435276231fc9
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 541fa4b96a15d6f458c1730119b24c94daa1b20c716123d6fb3448623cc6b056
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 6. 过滤器

### 1. 定义过滤器

#### 定义 1 {#top-i-s6-def-1 .statement tag=0B3X}

*对集合 $X$ 进行过滤是 $X$ 的子集的集合 $\mathfrak{F}$，其具有以下属性：*

$(\mathrm{F}_1)$ *$X$的每子集，其中$\mathfrak{F}$属于至$\mathfrak{F}$的包含集合。*
$(\mathrm{F}_\mathrm{II})$ *$\mathfrak{F}$ 属于到 $\mathfrak{F}$ 的集合的每个有限交。*
$(\mathrm{F}_\mathrm{III})$ *空集不在 $\mathfrak{F}$ 中。*

从$(\mathrm{F}_\mathrm{II})$和$(\mathrm{F}_\mathrm{III})$得出，$\mathfrak{F}$的集合的每个有限交都是*非空*。

$X$ 定义结构 $X$、公理上的过滤器$\mathfrak{F}$，其中$(\mathrm{F}_1)$、$(\mathrm{F}_\mathrm{II})$ 和$(\mathrm{F}_\mathrm{III})$；这个结构被称为过滤后的集合*的*结构，而赋予这个结构的集合$X$被称为通过*$\mathfrak{F}$过滤的*集合。

公理$(\mathrm{F}_\mathrm{II})$等价于以下两个公理的合取：
$\mathfrak{F}$ 属于至$\mathfrak{F}$ 的两个集合 $(\mathrm{F}_{\mathrm{II}\,\mathrm{a}})$ *交。*
$(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ *$X$ 属于至 $\mathfrak{F}$。*

公理$(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$和$(\mathrm{F}_\mathrm{III})$表明*空集*上没有过滤器。

在子集的集合的阶中，满足$(\mathrm{F}_1)$也满足满足$(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$，它是*非空*是充分必要的。满足$(\mathrm{F}_1)$的子集中的集合也满足$(\mathrm{F}_\mathrm{III})$当且仅当它与$\mathfrak{P}(X)$不同时。

*过滤器的例。* 1) 如果单独的$X \neq \varnothing$、$X$的子集由……组成集合是$X$上的过滤器。更一般地，$X$的所有子集中的集合，其中包含给定的$X$的非空子集$A$是$X$上的过滤器。

2) 在拓扑空间$X$中，$X$的任意非空子集$A$的所有邻域*的*集合（特别是邻域的所有集合） $X$的点）是一个过滤器，称为$A$的*邻域过滤器*。

3) 如果$X$是*无限*集合，则$X$的*有限子集*的补码是过滤器的元素。 有限子集集合 $\mathbf{N}$ 整数 $\geqslant 0$ 的补集滤波器称为 *Fréchet 滤波器*。

### 2. 滤波器比较

#### 定义 2 {#top-i-s6-def-2 .statement tag=0B3Y}

给定相同集合 $X$ 上的两个滤波器 $\mathfrak{F}, \mathfrak{F}'$，$\mathfrak{F}'$ 被认为是更细比 $\mathfrak{F}$，或者 $\mathfrak{F}$ 比 $\mathfrak{F}'$ 更粗糙，如果 $\mathfrak{F} \subset \mathfrak{F}'$。如果也是 $\mathfrak{F} \neq \mathfrak{F}'$，则 $\mathfrak{F}'$ 被称为严格比 $\mathfrak{F}$ 更细，或 $\mathfrak{F}$ 严格比 $\mathfrak{F}'$ 更粗糙。

如果一个滤波器比另一个滤波器更细，则称两个滤波器具有可比性。 $X$上所有过滤器的集合按关系排序“$\mathfrak{F}$比$\mathfrak{F}'$更粗糙”；这个关系是由$\mathfrak{P}(\mathfrak{P}(X))$中包含关系引起的。

令 $(\mathfrak{F}_i)_{i \in I}$ 为集合 $X$ 上的任何非空过滤器系列（因此必须非空）；然后集合

$$
\mathfrak{F} = \bigcap_{i \in I} \mathfrak{F}_i
$$

满足公理$(F_I), (F_{II})$和$(F_{III})$，因此是一个过滤器； $\mathfrak{F}$被称为过滤器家族$(\mathfrak{F}_i)_{i \in I}$的交，显然是$X$上所有过滤器的有序集合中$\mathfrak{F}_i$的集合的下确界。

由单个集合$X$形成的滤波器是$X$上所有滤波器的有序集合中的最小的元素。我们将在no. 4中看到，如果$X$有多个元素，则$X$上的所有过滤器中的集合没有最大元素。

给定集合$X$的子集的集合$\mathfrak{G}$，让我们考虑在$X$和包含$\mathfrak{G}$上是否存在过滤器。如果这样的过滤器存在，则由$\mathfrak{G}$的集合有限交的$(F_{II})$它包含还有集合$\mathfrak{G}'$（包括$X$，即空子集的交） $\mathfrak{G}$);因此，这样一个过滤器存在的必要的条件是$X$的空子集不在$\mathfrak{G}'$中。这个条件也足够了，对于$(F_I)$任何过滤器，其中包含$\mathfrak{G}'$还有$X$的子集包含集合$\mathfrak{G}''$其中包含集合 $\mathfrak{G}'$。现在$\mathfrak{G}''$显然满足$(F_I)$；由于$\mathfrak{G}'$的定义，它满足$(F_{II})$；最后它满足$(F_{III})$，因为$X$的空子集不会属于到$\mathfrak{G}'$。因此$\mathfrak{G}''$是包含$\mathfrak{G}$最粗的过滤器，我们已经证明：

#### 命题 1 {#top-i-s6-prop-1 .statement tag=0B3Z}

$X$的子集、$X$、包含、集合、$\mathfrak{G}$上应存在过滤器的充分充分条件是，$\mathfrak{G}$的有限子集不存在空的交。

上面定义的过滤器$\mathfrak{G}''$被认为是由$\mathfrak{G}$生成的，$\mathfrak{G}$被认为是$\mathfrak{G}''$的子基。

#### 例 {#top-i-s6-n2-exa-1 .statement tag=0B40}

令$\mathscr{S}$为集合$X$的子集中的任意集合，并令$\mathfrak{T}$为$\mathscr{S}$生成的$X$上的拓扑（$\S$2，no. 3， 例II）。由于$\mathscr{S}$的集合有限交集合是$\mathfrak{T}$的基，因此从上面的命题1的证明和$\S$1的命题3得出， no. 3，对于$\mathfrak{T}$的$x$的每个$x \in X$邻域过滤器是由$\mathscr{S}$的集合的集合$\mathfrak{G}(x)$生成，其中包含$x$。

#### 推论 1 {#top-i-s6-prop-1-cor-1 .statement tag=0B41}

令$\mathfrak{F}$为集合$X$的过滤器，以及$A$子集为$X$的过滤器。然后有一个过滤器$\mathfrak{F}'$，它比更细大于$\mathfrak{F}$，并且使得$A \in \mathfrak{F}'$，当且仅当$A$满足$\mathfrak{F}$的所有集合。

#### 推论 2 {#top-i-s6-prop-1-cor-2 .statement tag=0B42}

非空集$X$上的所有过滤器中的集合$\Phi$在$X$上的所有过滤器的集合中至少有上界当且仅当，对于$\Phi$的元素的所有有限序列$(\mathfrak{F}_i)_{1 \leq i \leq n}$且所有 $A_i \in \mathfrak{F}_i$ ($1 \leq i \leq n$), 交 $A_1 \cap \cdots \cap A_n$ 不为空。

对此，条件表示滤波器$\mathfrak{F} \in \Phi$的并$\mathfrak{G}$满足命题1的条件。

#### 推论 3 {#top-i-s6-prop-1-cor-3 .statement tag=0B43}

非空集合 $X$ 上所有滤波器的有序集合是归纳性的。

对于$X$上的每个线性排序的过滤器集合$\Phi$满足命题1的推论2的条件，因为集合$A_i$所有属于到相同的$\mathfrak{F}_j$ 假设，我们可以申请$(\mathrm{F}_{\mathrm{II}})$。

### 3. 基过滤器

如果 $\mathfrak{G}$ 是 $X$ (no. 2) 上过滤器 $\mathfrak{F}$ 的子基，则 $\mathfrak{F}$ 通常不是 $X$ 的子集的集合，其中包含集合 $\mathfrak{G}$；为了使$\mathfrak{G}$具有这个性质，$\mathfrak{G}$的集合的每个有限交应该是包含集合或$\mathfrak{G}$。因此有以下命题：

#### 命题 2 {#top-i-s6-prop-2 .statement tag=0B44}

设$\mathfrak{B}$为集合$X$的子集集合。那么$X$的子集的集合，其中$\mathfrak{B}$的包含集合是过滤器当且仅当$\mathfrak{B}$具有以下两个属性：
(B_I)$\mathfrak{B}$$\mathfrak{B}$包含集合两个集合交。
(B_{II})$\mathfrak{B}$不为空，$X$的空子集不在$\mathfrak{B}$中。

#### 定义 3 {#top-i-s6-def-3 .statement tag=0B45}

满足公理(B_I)和(B_{II})的集合$X$子集集合$\mathfrak{B}$被称为滤波器生成的基。如果两个过滤器基生成相同的过滤器，则称它们是等效的。

如果$\mathfrak{G}$是过滤器$\mathfrak{F}$的子基，则$\mathfrak{G}$的集合的有限交的集合$\mathfrak{G}'$是$\mathfrak{F}$（no. 2）的基。

#### 命题 3 {#top-i-s6-prop-3 .statement tag=0B46}

$X$上的过滤器$\mathfrak{F}$的子集$\mathfrak{B}$是$\mathfrak{F}$的基当且仅当$\mathfrak{F}$包含集合的$\mathfrak{B}$的每个集合。

如果$\mathfrak{B}$是$\mathfrak{F}$的基，那么显然$\mathfrak{F}$包含集合的集合是$\mathfrak{B}$；反之，如果$\mathfrak{F}$包含集合每集合$\mathfrak{B}$，则$X$包含集合$\mathfrak{B}$重合子集集合由于$(\mathrm{F}_1)$而有$\mathfrak{F}$。

#### 命题 4 {#top-i-s6-prop-4 .statement tag=0B47}

在集合$X$上，具有基$\mathfrak{B}'$的过滤器$\mathfrak{F}'$比具有基$\mathfrak{B}$的过滤器$\mathfrak{F}$更细当且仅当$\mathfrak{B}$包含的每个集合集合共$\mathfrak{B}'$。

这是定义 2 和 3 的直接的推论。

#### 推论{#top-i-s6-n3-cor-1 .statement tag=0B48}

集合 $X$ 上的两个滤波器基 $\mathfrak{B}, \mathfrak{B}'$ 等效当且仅当$\mathfrak{B}$ 包含集合 $\mathfrak{B}'$ 的每个集合以及$\mathfrak{B}'$ 包含的每个集合集合共$\mathfrak{B}$。

过滤器基的例。 1) 设$X$为拓扑空间。 命题3表明，点$x \in X$的邻域滤波器基正是$x$(§ 1, no. 3，定义5)的邻域的基数系统。

2) 令$X$是关于关系$(\sigma)$的非空有向集合（集合理论，章III, § 1, no. 10）。对于所有$x \in X$中的每个$a \in X$、集合$S(a)$，使得相对于元素$a$，$a(\sigma)x$将被称为$X$的截面。那么$X$的截面的集合$\mathscr{S}$是一个过滤器基，因为它显然满足$(\mathrm{B}_{\mathrm{II}})$，并且如果$a, b$是$X$的任意两个元素，则有假设元素$c \in X$使得$a(\sigma)c$和$b(\sigma)c$，因此
$$
S(c) \subset S(a) \cap S(b),
$$
从而满足$(\mathrm{B}_1)$。 $\mathscr{S}$生成的滤波器称为有向集合$X$的截面滤波器。

对于例，Fréchet 滤波器 (no. 1) 是有序集合 $\mathbf{N}$ 的截面滤波器，被视为由关系 $\leqslant$ 指示。
让$\mathfrak{F}$作为集合$Z$的过滤器。由于$\mathfrak{F}$相对于关系$\supset$有向[根据公理$(\mathrm{F}_{\mathrm{II}})$]，我们可以对$\mathfrak{F}$进行定义截面过滤；这里，$\mathfrak{F}$相对于集合$A \in \mathfrak{F}$的截面是所有$M \in \mathfrak{F}$的集合$S(A)$，使得$M \subset A$。该滤波器称为滤波器$\mathfrak{F}$的截面滤波器。

### 4. 超滤器

#### 定义 4 {#top-i-s6-def-4 .statement tag=0B49}

An ultrafilter on a set $X$ is a filter $\mathfrak{F}$ such that there is no filter on $X$ which is strictly finer than $\mathfrak{F}$ (in other words, a maximal element in the ordered set of all filters on $X$).

由于$X$上所有滤波器的有序集合是归纳式的（no. 2，命题1，推论3），Zorn的引理（集合理论，R，§ 6, no. 10）表明：

#### 定理 1 {#top-i-s6-thm-1 .statement tag=0B4A}

如果$\mathfrak{F}$是集合$X$上的任意滤波器，则存在比$\mathfrak{F}$超滤器更细。

#### 命题 5 {#top-i-s6-prop-5 .statement tag=0B4B}

令$\mathfrak{F}$为集合$X$上的超滤器。如果$A$和$B$是$X$的两个子集，使得$A \cup B \in \mathfrak{F}$，则$A \in \mathfrak{F}$或$B \in \mathfrak{F}$。

如果命题为假，则存在$X$的子集、$A$和$B$，使得$A \notin \mathfrak{F}$、$B \notin \mathfrak{F}$和$A \cup B \in \mathfrak{F}$。令 $\mathfrak{G}$ 为子集 $M$ $X$ 的集合，使得 $A \cup M \in \mathfrak{F}$。很容易检查$\mathfrak{G}$是$X$上的过滤器，并且$\mathfrak{G}$严格地更细比$\mathfrak{F}$，因为$B \in \mathfrak{G}$；但这与……矛盾假设那个$\mathfrak{F}$是超滤器。

#### 推论{#top-i-s6-n4-cor-1 .statement tag=0B4C}

*如果将并或有限序列*$(A_i)_{1 \leq i \leq n}$*将子集或*$X$*属于连接至超滤器*$\mathfrak{F}$，*则*$A_i$*属于至*$\mathfrak{F}$中的至少一个。

证明于 $n$ 归纳发布。
特别地，如果$(A_i)_{1 \leq i \leq n}$是$X$的*覆盖*，则$A_i$、属于到$\mathfrak{F}$中的至少一个。
命题 5 *表征*超滤器；更一般地说，我们有：

#### 命题 6 {#top-i-s6-prop-6 .statement tag=0B4D}

*让*$\mathfrak{G}$*成为集合*$X$上的过滤器的子基。 *如果对于* $X$的每个子集* $Y$ *我们有* $Y \in \mathfrak{G}$ *或* $\complement Y \in \mathfrak{G}$，*那么* $\mathfrak{G}$ *是* $X$上的超滤器。

设$\mathfrak{F}$为过滤器包含$\mathfrak{G}$（有一个，通过假设）；然后 $\mathfrak{F}$ 重合与 $\mathfrak{G}$；如果$Y \in \mathfrak{F}$则$\complement Y \notin \mathfrak{F}$；因此$\complement Y \notin \mathfrak{G}$，因此$Y \in \mathfrak{G}$。

*超滤器的例。*非空集合$X$的所有子集中的集合，其中包含给定的元素$a \in X$是超滤器；因为它是一个过滤器，如果$Y$是$X$中的任何子集，那么$a \in Y$或$a \in \complement Y$。这种超滤器被称为“平凡的”。

除了这个例之外，我们永远不会证明超滤器的存在（即使是在可数的无限集合上），除非使用定理1（因此选择公理）。

#### 注 {#top-i-s6-n4-rem-1 .statement tag=0B4E}

如果$X$包含至少有两个元素，则$X$上至少有两个不同的超滤器，因此$X$上的有序过滤器集合没有最大元素。

#### 命题 7 {#top-i-s6-prop-7 .statement tag=0B4F}

*每个过滤器* $\mathfrak{F}$ *在集合* $X$ *超滤器更细中的交比* $\mathfrak{F}$。

显然这个交包含$\mathfrak{F}$。反之，令$A$为$X$的子集，不包括属于至$\mathfrak{F}$，并令$A'$表示$\complement A$； $A$ 包含无 $\mathfrak{F}$ 的集合；因此，每个$M \in \mathfrak{F}$都满足$A'$，因此（no. 2，命题1，推论1）存在一个过滤器$\mathfrak{F}'$，它比$\mathfrak{F}$和包含$A'$更更细。如果$\mathfrak{U}$是超滤器更细，而不是$\mathfrak{F}'$（定理 1），则$A \notin \mathfrak{U}$。这样就完成了证明。

### 5.感应过滤器

#### 命题 8 {#top-i-s6-prop-8 .statement tag=0B4G}

*让*$\mathfrak{F}$*成为*集合*$X$*和*$A$*子集的过滤器*$X$。 *那么当且仅当* $\mathfrak{F}$ *的每个集合满足* $A$时，跟踪* $\mathfrak{F}_A$ *of* $\mathfrak{F}$ *在* $A$ *是一个过滤器。

从$(M \cap N) \cap A = (M \cap A) \cap (N \cap A)$我们看到$\mathfrak{F}_A$满足$(\mathrm{F}_{\mathrm{II}})$；再次，如果$M \cap A \subset P \subset A$则$P = (M \cup P) \cap A$，从而$\mathfrak{F}_A$满足$(\mathrm{F}_1)$。 Hence $\mathfrak{F}_A$ is a filter if and only if it satisfies $(\mathrm{F}_{\mathrm{III}})$, i.e. if and only if each set of $\mathfrak{F}$ meets $A$.

特别是，如果$A \in \mathfrak{F}$，则$\mathfrak{F}_A$是$A$上的过滤器，通过$(\mathrm{F}_{\mathrm{II}})$和$(\mathrm{F}_{\mathrm{III}})$。

#### 定义 5 {#top-i-s6-def-5 .statement tag=0B4H}

*令$A$为集合$X$的子集和$\mathfrak{F}$$X$上的过滤器。如果$\mathfrak{F}$在$A$上的迹是$A$上的滤波器，则称该滤波器是由$A$上的$\mathfrak{F}$诱导的。*

如果$X$ 诱导上的过滤器$\mathfrak{F}$ $A \subset X$ 上的过滤器，则由于no. 3 的命题 3，$\mathfrak{F}$ 基 $A$ 上的轨迹为$\mathfrak{F}_A$ 基。

#### 例 {#top-i-s6-n5-exa-1 .statement tag=0B4I}

令$X$为空间、$X$的$A$子集、$X$的$x$点。在阶中，$x$的*邻域滤波器*$\mathfrak{B}$在$A$上的迹应该是$A$上的滤波器，$x$的每个邻域满足$A$是充分必要的，即$x$位于在$A$（§ 1, no. 6，定义10）的*闭包*中。

诱导滤波器的例之所以令人感兴趣，有两个原因：首先是因为它在极限 (§ 7, no. 5) 的理论中发挥着重要作用，其次是因为*每个滤波器都可以用这种方式定义*。事实上，让$\mathfrak{F}$成为集合$X$上的过滤器，并让$X'$成为集合，通过将新的元素$\omega$*邻接*到$X$，$X$被识别为$\{ \omega \}$的补集在$X'$（*集合理论*，R，§ 4, no. 5）；令$\mathfrak{F}'$为集合$M \cup \{ \omega \}$的$X'$由……组成上的过滤器，其中$M$穿过$\mathfrak{F}$。对于$X'$的每个点$x \neq \omega$，令$\mathfrak{B}(x)$为$X'$的所有子集其中包含$x$的集合，并令$\mathfrak{B}(\omega)$为$\mathfrak{F}'$；那么$x \in X'$的$\mathfrak{B}(x)$显然是满足公理$(\mathrm{V}_1), (\mathrm{V}_{\mathrm{II}}), (\mathrm{V}_{\mathrm{III}})$和$(\mathrm{V}_{\mathrm{IV}})$，因此$X'$上的定义拓扑，它们是点的邻域过滤器。最后，$\omega$位于拓扑中$X$的*闭包*中，$\mathfrak{F}$由$\mathfrak{F}' = \mathfrak{B}(\omega)$在$X$上诱导。因此在 $X'$（分别是集合 $X'$ 和这个拓扑）上定义的拓扑被称为 *拓扑* （分别是 *拓扑空间*）*与* $\mathfrak{F}$ 相关联。

#### 命题 9 {#top-i-s6-prop-9 .statement tag=0B4J}

* 集合 $X$ 诱导上的超滤$U$ $X$ 子集 $A$ 上的过滤器当且仅当$A \in U$；如果满足这个条件，那么$U_A$就是$A$上的超级过滤器。*

这是命题 5 中的直接的推论和no. 4 中的6。

### 6. 过滤器直接像和逆像基

令$\mathfrak{B}$为集合$X$上的过滤器基，并令$f$为$X$的映射进入集合$X'$；那么$f(\mathfrak{B})$是$X'$上的*过滤器基*，因为关系$M \neq \emptyset$意味着$f(M) \neq \emptyset$，我们有$f(M \cap N) \subset f(M) \cap f(N)$。如果$\mathfrak{B}_1$是比基$\mathfrak{B}$的过滤器*更细*的过滤器的基，则$f(\mathfrak{B}_1)$是比基$f(\mathfrak{B})$的过滤器*更细*的基 （no. 3，命题4）。

#### 命题 10 {#top-i-s6-prop-10 .statement tag=0B4K}

*如果$\mathfrak{B}$是集合$X$上的超滤器基，并且如果$f$是集合$X'$中$X$的映射，则$f(\mathfrak{B})$是超滤器基 $X'$.*

令 $M'$ 为 $X'$ 的子集。如果 $\mathfrak{B}$ 中的 $\overline{f}^{-1}(M')$ 包含集合 $M$，则 $M'$ 包含 $f(M)$；如果不是，则 $\mathscr{C}_{\overline{f}}^{-1}(M') = \overline{f}^{-1}\mathscr{C}(M')$ 包含集合 $N$ $\mathfrak{B}$ (no. 4, 命题 5)，因此$\mathscr{C}M'$ 包含 $f(N)$。因此，结果来自命题 6 of no. 4。

特别考虑$f$是集合$X$的子集$A$的典范嵌入$A \to X$的情况。如果$\mathfrak{B}$是$A$上的过滤器基，则$f(\mathfrak{B})$是$X$上的过滤器基。当$\mathfrak{B}$被视为$X$上的过滤器基*时，由$f(\mathfrak{B})$生成的$X$上的过滤器$\mathfrak{F}$称为*由$\mathfrak{B}$生成的过滤器。如果$\mathfrak{B}$是$A$上的*超滤基*，那么由于命题10，它也是$X$上的*超滤基*。

接下来让我们检查过滤器基的*逆像*是否是过滤器基。令$\mathfrak{B}'$为集合$X'$上的过滤器基，令$f$为集合$X$到$X'$的映射；那么 $\overline{f}^{-1}(\mathfrak{B}')$ 是 $X$ *当且仅当* $\overline{f}^{-1}(M') \neq \varnothing$ *对于每个* $M' \in \mathfrak{B}'$ 的过滤器基。这是关系$\overline{f}^{-1}(M' \cap N') = \overline{f}^{-1}(M') \cap \overline{f}^{-1}(N')$的直接的推论和no. 3的定义3。这个条件也可以用说来表示：$\mathfrak{B}'$的每一个集合都满足$f(X)$*[或者$\mathfrak{B}'$在$f(X)$上的迹是一个过滤器基]。如果满足这个条件，则$f(\overline{f}^{-1}(\mathfrak{B}'))$是过滤器*更细*的基，而不是基$\mathfrak{B}$的过滤器。

如果$\mathfrak{B}$是$X$上的过滤器基，很明显，上面的条件由$\mathfrak{B}' = f(\mathfrak{B}); \; \overline{f}^{-1}(f(\mathfrak{B}))$满足，那么基的过滤器*比基$\mathfrak{B}$的过滤器*粗糙。

设$A$为集合$X$、$\varphi$典范嵌入$A \to X$中的子集；如果$\mathfrak{B}$是$X$上的过滤器基，则$\overline{\varphi}^{-1}(\mathfrak{B})$与$\mathfrak{B}_A$相同。如果我们通过上面的条件将其表达为$A$的过滤器基，我们将恢复no. 5的命题8的部分。

### 7. 乘积过滤器

令$(X_i)_{i \in I}$为集合的族，对于每个$i \in I$，令$\mathfrak{B}_i$为$X_i$上的*过滤器基*。令$\mathfrak{B}$为乘积集合$X = \prod_{i \in I} X_i$的子集的集合，其中形式$\prod_{i \in I} M_i$，其中$M_i = X_i$除了指标的*有限*数并且其中$M_i \in \mathfrak{B}_i$ 对于每个 $i$ 使得 $M_i \neq X_i$。 公式 $\left( \prod_{i \in I} M_i \right) \cap \left( \prod_{i \in I} N_i \right) = \prod_{i \in I} (M_i \cap N_i)$ 显示$\mathfrak{B}$ 是$X$ 上的*过滤器基*。 注基 $\mathfrak{B}$ 的过滤器也是由

集合 $\overline{\mathrm{pr}}_x^{-1}(M_x)$，其中$M_x \in \mathfrak{B}_x$和$x$贯穿$I$，因为
$$
\overline{\mathrm{pr}}_x^{-1}(M_x) = M_x \times \prod_{i \neq x} X_i.
$$

#### 定义 6 {#top-i-s6-def-6 .statement tag=0B4L}

*Given a filter $\mathfrak{F}_i$ on each set $X_i$ of a family of sets $(X_i)_{i \in I}$, the product of the filters $\mathfrak{F}_i$ is the filter on $X = \prod_{i \in I} X_i$ which has as a base the set of subsets of $X$ of the form $\prod_{i \in I} M_i$, where $M_i \in \mathfrak{F}_i$ for each $i \in I$ and $M_i = X_i$ for all but a finite number of indices. 乘积过滤器由$\prod_{i \in I} \mathfrak{F}_i$表示。*

读者可以轻松验证过滤器$\mathfrak{F}_i$的乘积也可以定义为$X$上的*粗略*过滤器$\mathfrak{G}$，使得每个$i \in I$都有$\mathrm{pr}_i(\mathfrak{G}) = \mathfrak{F}_i$。

前面的注表明，如果对于每个$i \in I$，$\mathfrak{B}_i$是$\mathfrak{F}_i$的基，则$\mathfrak{B}$是乘积过滤器$\prod_{i \in I} \mathfrak{F}_i$的*基*（no. 3，命题3）。

在拓扑空间的乘积$X = \prod_{i \in I} X_i$上，任何点$x = (x_i)$的邻域过滤器都是$x_i$（§ 4, no. 1）的邻域过滤器的*乘积*。

当指标集合 $I$ 是*有限*时，乘积过滤器 $\mathfrak{F} = \prod_{i \in I} \mathfrak{F}_i$ 构造更简单：$\mathfrak{F}$ 的基则由 *all* 乘积 $\prod_{i \in I} M_i$ 形成，其中每个$M_i \in \mathfrak{F}_i$ $i \in I$。 如果 $I = \{ 1, 2, \ldots, n \}$ 我们写
$$
\mathfrak{F}_1 \times \mathfrak{F}_2 \times \cdots \times \mathfrak{F}_n
$$
而不是 $\prod_{i \in I} \mathfrak{F}_i$。

### 8. 基本过滤器

#### 定义 7 {#top-i-s6-def-7 .statement tag=0B4M}

*令$(x_n)_{n \in \mathbf{N}}$为集合$X$的元素的无限序列。与序列 $(x_n)$ 关联的基本滤波器是由 Fréchet 滤波器 (no. 1) 的像通过 $\mathbf{N}$ 的映射 $n \to x_n$ 生成$X$ 的滤波器。*

与$(x_n)$相关的基本过滤器是$X$的子集$M$的集合，使得$x_n \in M$除了$n$的值的*有限*数，这也是同样的道理。如果$S_n$表示所有$x_p$中的集合使得$p \geq n$，则集合$S_n$形式与序列$(x_n)$相关联的基本滤波器的*基*。

与序列 $(x_n)$ 的无限*子序列*关联的基本滤波器比与 $(x_n)$ (cf. 习题 15) 关联的基本滤波器 *更细*。

到定义，每个基本过滤器都有一个可数的基。反过来：

#### 命题 11 {#top-i-s6-prop-11 .statement tag=0B4N}

*如果过滤器$\mathfrak{F}$有可数的基，则它是基本过滤器中更细比$\mathfrak{F}$的交。*

我们将$\mathfrak{F}$的可数基排列为序列$(A_n)_{n \in \mathbf{N}}$；如果我们把

$$
B_n = \bigcap_{p=0}^n A_p,
$$

然后$B_n$又是$\mathfrak{F}$的形式基（no. 3，命题3），每个$n$都有$B_{n+1} \subset B_n$。对于每个$n \in \mathbf{N}$，令$a_n$为$B_n$中的任意元素；那么很明显$\mathfrak{F}$比与$(a_n)$相关的基本滤波器更粗糙。因此存在更细大于$\mathfrak{F}$且更细大于$\mathfrak{F}$的基本滤波器交$\mathfrak{J}$；如果$\mathfrak{J}$*严格更细*大于$\mathfrak{F}$，则存在集合$M \in \mathfrak{J}$，使得每个$n$都有$B_n \cap \complement M \neq \varnothing$；如果$b_n \in B_n \cap \complement M$，则与序列$(b_n)$相关联的基本滤波器更细大于$\mathfrak{F}$，并且不包含$M$。这$\mathfrak{J}$的与……矛盾定义。

#### 注 {#top-i-s6-n8-rem-1 .statement tag=0B4O}

比具有可数基的过滤器“更粗糙”的过滤器不需要拥有可数基；对于例，如果$X$是不可数无限集合，则$X$的有限子集的补集的过滤器由……组成没有可数的基（否则$X$的有限子集的集合）是可数的，与假设相反）；然而，这个过滤器比与无限序列的不同元素或 $X$ 相关联的每个基本过滤器都要粗糙。

### 9. 与过滤器相关的细菌

让$\mathfrak{F}$作为集合$X$的过滤器。 $X$全部子集、关系中的集合$\mathfrak{P}(X)$

“存在$V \in \mathfrak{F}$使得$M \cap V = N \cap V$”

$M$和$N$之间是一个*等价关系*$R$，因为$R$显然是自反且对称的，并且如果$M, N, P$是$X$的三个子集，使得$M \cap V = N \cap V$和$N \cap W = P \cap W$，其中$V$ 和 $W$ 属于到 $\mathfrak{F}$，可得出 $M \cap (V \cap W) = N \cap (V \cap W) = P \cap (V \cap W)$ 和 $V \cap W \in \mathfrak{F}$，因此 $R$ 是及物性的。 $X$的子集$M$等价类模$R$相对于$\mathfrak{F}$*称为$M$的*胚芽； 商集$\mathfrak{P}(X)/R$称为$X$（相对于$\mathfrak{F}$）*的子集菌*集合。 映射 $(M, N) \to M \cap N$ 和 $(M, N) \to M \cup N$

$$
\mathfrak{P}(X) \times \mathfrak{P}(X)
$$

$\mathfrak{P}(X)$ 与等价关系 $R \times R$ 和 $R$ 相容的

（集合理论，R，，no. 8）。对于如果 $M \equiv M' \pmod{R}$ 和 $N \equiv N' \pmod{R}$ 则在 $\mathfrak{F}$ 中存在 $V$ 和 $W$ 使得

$$
M \cap V = M' \cap V \quad \text{and} \quad N \cap W = N' \cap W,
$$
这样
$$
(M \cap N) \cap (V \cap W) = (M' \cap N') \cap (V \cap W)
$$
和
$$
\begin{align*}
(M \cup N) \cap (V \cap W) &= (M \cap (V \cap W)) \cup (N \cap (V \cap W)) \\
&= (M' \cap (V \cap W)) \cup (N' \cap (V \cap W)) \\
&= (M' \cup N') \cap (V \cap W).
\end{align*}
$$

经过到商，这些映射诱导将$(\mathfrak{P}(X)/R) \times (\mathfrak{P}(X)/R)$的两个映射化为$\mathfrak{P}(X)/R$，我们分别用$(\xi, \eta) \to \xi \cap \eta$和$(\xi, \eta) \to \xi \cup \eta$表示（滥用语言）。这是一个简单的习题来验证对于合成的这些律[在$\mathfrak{P}(X)/R$中定义]，每个元素都是幂等的，并且每个律相对于另一个律是可交换的、关联的和分配的。进一步地，关系$\xi = \xi \cap \eta$与$\eta = \xi \cup \eta$等价；如果我们用$\xi \subset \eta$来表示它们（滥用语言），很容易验证这个关系是$\mathfrak{P}(X)/R$的一个排序，相对于它$\mathfrak{P}(X)/R$是一个格子，其中$\varnothing$的胚芽至少为元素，$X$的胚芽为最大元素。 注、关系$\xi \subset \eta$意味着存在$M \in \xi$、$N \in \eta$和$V \in \mathfrak{F}$使得$M \cap V \subset N \cap V$。

现在令$X'$为另一个集合，并令$\Phi$为$\mathfrak{F}$的集合所有映射到$X'$的集合。 关系 $\Phi$

“存在$V \in \mathfrak{F}$使得$f$和$g$被定义并同意$V$”

$f$和$g$之间是等价关系$S$；显然，$S$是自反且对称的，如果$f, g, h$是$\Phi$的三个元素，使得$f$和$g$在$V \in \mathfrak{F}$上定义，$g$和$h$在$W \in \mathfrak{F}$上定义并一致，那么$f$ 和 $h$ 已定义且一致于 $V \cap W \in \mathfrak{F}$，因此 $S$ 具有传递性。将集合 $V \in \mathfrak{F}$ 映射 $f$ 等价类 mod $S$ 成 $X'$ 称为 $f$ (相对于$\mathfrak{F}$)的胚芽，商集 $\tilde{\Phi} = \Phi/S$ 称为$X$的映射细菌的集合变成$X'$（相对于$\mathfrak{F}$）。

#### 注 1 {#top-i-s6-n9-rem-1 .statement tag=0B4P}

将$X$的子集$M$的每个映射$f$化为$X'$，其中$M$属于到$\mathfrak{F}$，相当于$S$对映射$f_1$的mod $X$ 变为 $X'$（这证明了上述术语）：扩展 $f$ 到 $X$ 就足够了，例如通过在 $X - M$ 上给它一个常数值。

#### 注 2 {#top-i-s6-n9-rem-2 .statement tag=0B4Q}

两个子集$M$的特征函数$\varphi_M$和$\varphi_N$以及$X$的$N$相对于$\mathfrak{F}$具有相同的胚芽当且仅当$M$和$N$相对于$\mathfrak{F}$具有相同的胚芽。

令$X''$为$X'$的第三个集合、$\varphi$映射到$X''$、$\Phi'$集合到$\mathfrak{F}$的集合的所有映射到$X''$。对于每个 $f \in \Phi$、$\varphi \circ f$ 属于至 $\Phi'$；此外，立即看出，如果$g \in \Phi$与$f$对于$\mathfrak{F}$具有相同的胚芽，则$\varphi \circ f$和$\varphi \circ g$对于$\mathfrak{F}$具有相同的胚芽。

因此，该胚芽仅依赖于$f$相对于$\mathfrak{F}$的胚芽$\tilde{f}$，并用$\varphi(\tilde{f})$表示。 因此，我们将$X$的映射细菌的定义映射（通过滥用语言表示为$\varphi$）集合$\tilde{\Phi}$转化为$X'$，映射的细菌集合$\tilde{\Phi}'$ $X$ 变为$X''$。

现在令 $X'_i$ ($1 \leq i \leq n$) 为集合并且
$$
Y = \prod_{i=1}^n X'_i
$$
他们的乘积；让$\Phi_i$（或$\Phi$）表示$\mathfrak{F}$的集合的所有映射到$X'_i$（或$Y$）的集合。如果 $f_i \in \Phi_i$ 代表 $1 \leq i \leq n$ 并且 $M_i \in \mathfrak{F}$ 是定义域且 $f_i$，则映射 $t \to (f_1(t), \ldots, f_n(t))$ 定义为
$$
\bigcap_{i=1}^n M_i
$$
因此属于到 $\Phi$；我们将这个映射（通过滥用语言）表示为$(f_1, \ldots, f_n)$。此外，如果$f_i$和$g_i$属于到$\Phi_i$并且对于$\mathfrak{F}$（对于$1 \leq i \leq n$）具有相同的胚芽，那么立即可以看出$(f_1, \ldots, f_n)$和$(g_1, \ldots, g_n)$对于$\mathfrak{F}$具有相同的胚芽；因此，该细菌仅依赖于 $f_i$ 的细菌 $\tilde{f}_i$。如果我们用$\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$表示，那么$\Gamma$显然是乘积集合的双射
$$
\prod_{i=1}^n \tilde{\Phi}_i
$$
到集合$\tilde{\Phi}$，其中$\tilde{\Phi}_i$（分别$\tilde{\Phi}$）表示相对于$\mathfrak{F}$将$X$的映射的细菌的集合进入$X'_i$（分别$Y$）；因此，为了避免混淆，我们通常会滥用语言，写成$(\tilde{f}_1, \ldots, \tilde{f}_n)$而不是$\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$。

如上所述，每 $Y$ 映射 $\psi$ 变为集合 $X''$ 定义映射 $(\tilde{f}_1, \ldots, \tilde{f}_n) \to \psi(\tilde{f}_1, \ldots, \tilde{f}_n)$
$$
\prod_{i=1}^n \tilde{\Phi}_i
$$
将$X$的映射细菌转化为集合$\tilde{\Phi}'$转化为$X''$。

特别是，如果 $n = 2$ 且 $X'_1, X'_2$ 和 $X''$ 都等于相同的集合 $X'$（因此 $\psi$ 是在 $X'$ 中定义的合成的律），则 $\psi$ 诱导合成的律定义为$X$映射的细菌的集合$\tilde{\Phi}$到$X'$。很容易验证，如果在 $X'$ 上给出的律是结合律（或可交换的），那么在 $\tilde{\Phi}$ 上的相应的律也是结合律（或交换律）；如果$X'$上的律$\psi$有单位元素$e'$，则常数映射$x \to e'$相对于$\mathfrak{F}$的胚芽对于相应的律来说是单位元素 $\tilde{\Phi}$。最后，如果$X'$上的律具有单位元素$e'$，则$f \in \Phi$的胚芽$\tilde{f}$在$\tilde{\Phi}$中具有逆，当且仅当存在包含在$f$域中的$V \in \mathfrak{F}$，使得对于每个 $t \in V$，$f(t)$ 在 $X'$ 中是可逆的；如果对于每个$t \in V$，$g(t)$表示$f(t)$的逆，那么$g$的胚芽$\tilde{g}$就是$\tilde{\Phi}$中$\tilde{f}$的逆。特别是，如果$X'$相对于律$\psi$来说是群，则$\tilde{\Phi}$相对于相应的律来说是群；同样，如果$X'$是环（分别是代数超过环$A$），那么相对于相应的，$\tilde{\Phi}$是环（分别是代数超过$A$） 律共合成。

### 10. 细菌点

定义和no. 9的结果适用的最常见情况之一是$\mathfrak{F}$是拓扑空间$X$的点$a$的邻域过滤器；我们不再说“关于 $\mathfrak{F}$ 的细菌”，而是说“点 $a$ 的细菌”。请注意，$a$中只有一个邻域的胚芽，即整个空间$X$的胚芽。闭合集合的细菌与在点$a$处局部闭合的集合的细菌相同，因为如果$L$在$a$处局部闭合，则$L$和$\overline{\Gamma}$在$a$处的细菌是等于（§ 3, no. 1，命题1）。由此可见，如果$\xi, \eta$是$a$处局部封闭的集合的两个细菌，那么$\xi \cup \eta$和$\xi \cap \eta$也是。

由于$a$在每个$V \in \mathfrak{F}$中，因此为每个映射$f$定义了$f(a)$，其域为属于到$\mathfrak{F}$；此外，如果$f$和$g$在$a$处具有相同的胚芽，我们必须有$f(a) = g(a)$，因此$f(a)$仅依赖于$f$在$a$处的胚芽$\tilde{f}$，并且在$\tilde{f}$处被称为值 $a$ 并用$\tilde{f}(a)$ 表示。需要强调的是，关系$\tilde{f}(a) = \tilde{g}(a)$一般并不意味着$\tilde{f} = \tilde{g}$。

设$X', X''$为两个拓扑空间； $b$点共$X''$； $g, g'$ $X'$ 中的两个映射进入$X''$，在$b$ 具有相同的胚芽。如果$f, f'$是$X$的两个映射进入$X'$，它们在$a$处连续并且在$a$处具有相同的胚芽并且使得$f(a) = b$，则$g \circ f$和$g' \circ f'$在点处具有相同的胚芽$a$；因为如果$V'$是$X'$中$b$的邻域，使得$g(x') = g'(x')$对于所有$x' \in V'$，则存在$a$的邻域$V$使得$f(V) \subset V'$，$f'(V) \subset V'$并且$f(x) = f'(x')$ 对于所有 $x \in V$，然后是断言。 $a$处的$g \circ f$的胚芽则分别称为$g$和$f$的胚芽$\tilde{g}$和$\tilde{f}$的合成，并用$\tilde{g} \circ \tilde{f}$表示。

### 习题{#top-i-s6-exercises}

§ 6](exercises/s6/)参见[习题。
