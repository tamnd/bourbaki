---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 2
section_title: Uniformly continuous functions
lang: zh
source: top-i-iv
book_pages: 174-181, 207-208
pdf_pages: 0180-0187, 0213-0214
extraction: ocr
subsections:
    - "no": 1
      title: UNIFORMLY CONTINUOUS FUNCTIONS
      page: 174
      pdf_page: 180
    - "no": 2
      title: COMPARISON OF UNIFORMITIES
      page: 175
      pdf_page: 181
    - "no": 3
      title: INITIAL UNIFORMITIES
      page: 176
      pdf_page: 182
    - "no": 4
      title: INVERSE IMAGE OF A UNIFORMITY; UNIFORM SUBSPACES
      page: 177
      pdf_page: 183
    - "no": 5
      title: LEAST UPPER BOUND OF A SET OF UNIFORMITIES
      page: 178
      pdf_page: 184
    - "no": 6
      title: PRODUCT OF UNIFORM SPACES
      page: 179
      pdf_page: 185
    - "no": 7
      title: INVERSE LIMITS OF UNIFORM SPACES
      page: 180
      pdf_page: 186
statements: 27
exercises: 6
content_sha256: 99c5d44dc8cbadd2c900be1d8584ae263854c8ef8e8d28aa8dc3c76c9cafeb5e
translated_from: content/en/top/II/02_s2_uniformly_continuous_functions.md
translation_method: google
source_content_sha256: 92b674d0f20d1a67ab0b8298e6f5a7fe7434487139d32666270aa426c8d22f2f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 70128667984cf28708867ad56aeb6870a804248efb6e197118036374282aba07
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 2. 均匀连续函数

### 1. 均匀连续函数

#### 定义 1 {#top-ii-s2-def-1 .statement tag=0BDH}

*将制服空间 $X$ 到制服空间 $X'$ 的映射 $f$ 称为均匀连续，如果对于 $X'$ 的每个随行人员 $V'$，存在 $X$ 的随行人员 $V$，使得关系 $(x, y) \in V$ 意味着$(f(x), f(y)) \in V'$。*

在更具表现力的项中，如果$f(x)$和$f(y)$彼此尽可能接近，只要$x$和$y$足够接近，我们可以说$f$是一致连续的。

如果我们放入$g = f \times f$，那么定义 1 意味着*当$V'$是$X'$的随从时，$\overline{g^{-1}}(V')$是$X$的随从*。

#### 例 1 {#top-ii-s2-n1-exa-1 .statement tag=0BDI}

均匀连续的空间的恒等映射是均匀连续的。

#### 例 2 {#top-ii-s2-n1-exa-2 .statement tag=0BDJ}

均匀连续的空间到均匀空间的常数映射是均匀连续的。

#### 例 3 {#top-ii-s2-n1-exa-3 .statement tag=0BDK}

离散均匀空间到均匀空间的每个映射都是均匀连续的。

#### 命题 1 {#top-ii-s2-prop-1 .statement tag=0BDL}

每个一致连续映射都是连续的。

这是定义中的直接的推论。

另一方面，从一致空间X到一致空间X'的连续映射不需要一致连续，\*如例$x \to x^3$所示，$\mathbf{R}$自身同胚，这不是就添加剂的均匀性而言是均匀连续的。 \* （参见§ 4, no. 1、定理 2。）

#### 命题 2 {#top-ii-s2-prop-2 .statement tag=0BDM}

(a) 如果$f : X \to X'$和$g : X' \to X''$是两个一致连续的映射，则$g \circ f : X \to X''$是一致连续的。

(b) 当且仅当$f$和$f$的逆一致连续时，均匀空间X到均匀空间X的双射$f$是同构。

这直接来自于乘积映射 $f \times f$ 项中定义 1 的解释。

### 2. 均匀性比较

no. 1的命题 2表明我们可以将结构均匀连续映射视为态射（集合理论，章IV, § 2, no. 1）；我们将来总是假设态射是这样选择的。根据一般的定义（集合理论，章IV, § 2, no. 2），这允许我们在给定的集合X上对集合均匀性进行定义序关系：

#### 定义 2 {#top-ii-s2-def-2 .statement tag=0BDN}

如果$\mathfrak{U}_1$和$\mathfrak{U}_2$是同一个集合X上的两个均匀结构，则$\mathfrak{U}_1$被称为更细比$\mathfrak{U}_2$（并且$\mathfrak{U}_2$比$\mathfrak{U}_1$更粗糙）如果，用 $X_i$ 集合 X 表示，且一致结构 $\mathfrak{U}_i$ ($i = 1,2$)，恒等映射 $X_1 \to X_2$ 是一致连续的。

如果$\mathfrak{U}_1$比$\mathfrak{U}_2$是更细并且与$\mathfrak{U}_2$不同，我们说$\mathfrak{U}_1$严格比更细比$\mathfrak{U}_2$（并且$\mathfrak{U}_2$严格比$\mathfrak{U}_1$更粗糙）。

如果一个均匀度比另一个均匀度更细，则称两个均匀度具有可比性。

#### 例 {#top-ii-s2-n2-exa-1 .statement tag=0BDO}

在集合X上有序的集合均匀度中，离散均匀度最好，最粗的均匀度是集合随行体由单个元素$X \times X$组成。

下面的命题是直接的推论定义1 no. 1：

#### 命题 3 {#top-ii-s2-prop-3 .statement tag=0BDP}

如果 $\mathfrak{U}_1$ 和 $\mathfrak{U}_2$ 是集合 X 上的两个一致，则当且仅当 $\mathfrak{U}_2$ 的每个随行人员都是 $\mathfrak{U}_1$ 的随行人员时，$\mathfrak{U}_1$ 比 $\mathfrak{U}_2$ 更细。

#### 推论{#top-ii-s2-n2-cor-1 .statement tag=0BDQ}

设$\mathfrak{U}_1$和$\mathfrak{U}_2$为集合X上的两个一致度，并假设$\mathfrak{U}_1$比$\mathfrak{U}_2$为更细；那么$\mathfrak{U}_1$诱发的拓扑比$\mathfrak{U}_2$诱发的拓扑为更细。

这是直接从项和邻域中的拓扑比较得出的（章 I, , no. 2, 命题 3）

#### 注 1 {#top-ii-s2-n2-rem-1 .statement tag=0BDR}

可能会出现均匀性 $\mathfrak{U}_1$ 比均匀性 $\mathfrak{U}_2$ 严格为更细，但两个导出的拓扑是相同的。下面的例展示了这一点：

令 $X$ 为非空集合。对于 $X$ 的每个有限划分 $\varpi = (A_i)_{1 \leq i \leq n}$，令 $V_{\overline{\varpi}}$ 表示
$$
\bigcup_i A_i \times A_i.
$$
集合$V_{\overline{\varpi}}$然后形式基本的系统随行人员在$X$上均匀$\mathfrak{U}$。因为如果$\varpi$是$X$的任何有限划分，我们有$\Delta \subset V_{\overline{\varpi}}$和$V_{\overline{\varpi}} \circ V_{\overline{\varpi}} = \overline{V_{\overline{\varpi}}} = V_{\overline{\varpi}}$（§ 1, no. 1，例2）；如果$\varpi' = (B_j)$和$\varpi'' = (C_k)$是$X$的两个有限划分，那么集合$B_j \cap C_k$不为空的形式是$X$的有限划分$\varpi$，我们有$V_{\overline{\varpi}} \subset V_{\overline{\varpi'}} \cap V_{\overline{\varpi''}}$。 $\mathfrak{U}$称为有限划分在$X$上的均匀性。由 $\mathfrak{U}$ 引发的拓扑是离散的拓扑，因为对于每个 $x \in X$ 集合 $\{x\}$ 和 $C\{x\}$ 形式 ，划分为 $X$。然而，如果 $X$ 是无限的，则显然 $\mathfrak{U}$ 严格比离散均匀性更粗糙。

#### 注 2 {#top-ii-s2-n2-rem-2 .statement tag=0BDS}

如果 $f : X \to X'$ 是均匀连续的映射，那么如果我们通过更细均匀性对 $X$ 进行替换的均匀性，并通过更粗略的均匀性（no. 1、命题 2）对 $X'$ 进行均匀连续处理，则 $f$ 保持均匀连续。在其他字、更细中，$X$的均匀度和$X'$的均匀度越粗糙，$X$到$X'$的映射越均匀连续。

### 3. 初始均匀性

#### 命题 4 {#top-ii-s2-prop-4 .statement tag=0BDT}

令$X$为集合，令$(Y_i)_{i \in I}$为统一空间的族，对于每个$i \in I$，令$f_i$为$X$到$Y_i$的映射。对于每个$i \in I$，让$g_i$表示$f_i \times f_i$。令$\mathfrak{S}$为形式$\overline{g_i}(V_i)$$X \times X$子集集合，其中$i \in I$和$V_i$为$Y_i$的随从，并令$\mathfrak{B}$为集合全部有限交

$$
\text{(1)} \quad U(V_{i_1}, \ldots, V_{i_n}) = \overline{g_{i_1}}(V_{i_1}) \cap \cdots \cap \overline{g_{i_n}}(V_{i_n})
$$

集合 $\mathfrak{S}$。那么$\mathfrak{B}$是$X$上均匀性$\mathfrak{U}$的基本系统，这是$X$上关于家庭$(f_i)$的初始均匀性结构（集合理论，章IV, § 2, no. 3），特别是$\mathfrak{U}$ 是 $X$ 上的最粗糙均匀性，其中所有映射 $f_i$ 都是均匀连续的。但除此之外，令 $h$ 为空间 $Z$ 到 $X$ 的映射；则 $h$ 是一致连续的（当 $X$ 具有均匀性 $\mathfrak{U}$ 时）当且仅当映射 $f_i \circ h$ 中的每一个都是一致连续的。

立即可见$\mathfrak{B}$满足公理$(B_1)$和$(U'_1)$。如果$W_i = \overline{g}_i^{-1}(V_i)$，则$\overline{W}_i = \overline{g}_i^{-1}(\overline{V}_i)$和$\dot{W}_i = \dot{g}_i^{-1}(\dot{V}_i)$；因此$\mathfrak{B}$也满足公理$(U'_{II})$和$(U'_{III})$，因此是$X$上一致性$\mathfrak{U}$的基本系统。此外，从$\mathfrak{U}$和定义1和no. 1的定义可以立即得出，对于每个指标$i \in I$，$f_i$是一致连续的；因此，如果 $h$ 是，则 (no. 1, 命题 2) $f_i \circ h$ 对于每个 $i \in I$ 是均匀连续的。相反，假设$f_i \circ h$对于每个$i \in I$是一致连续的，并考虑集合$U(V_{i_1}, \ldots, V_{i_n})$；通过假设，对于每个$k$使得$1 \leq k \leq n$，有一个$Z$的随从$W_k$使得关系$(z, z') \in W_k$意味着$[f_{i_k}(h(z)), f_{i_k}(h(z'))] \in V_k$；如果
$$
W = \bigcap_k W_k,
$$
每当 $z$ 和 $z'$ $W$ 接近时，这些 $n$ 关系同时满足，这样我们就有 $(h(z), h(z')) \in U(V_{i_1}, \ldots, V_{i_n})$，证明是完整的。

#### 推论{#top-ii-s2-n3-cor-1 .statement tag=0BDU}

*$X$上的拓扑由最粗糙均匀性$\mathfrak{U}$引起，其中$f_i$均匀连续，也是最粗糙拓扑，其中$f_i$连续。*

这后者中的拓扑是点邻域定义直接的推论（章I, § 2, no. 3、命题4）。

初始结构（*集合理论*，章IV, § 2, no. 3，标准 CST 10）的一般属性特别意味着以下*传递性* 性质：

#### 命题 5 {#top-ii-s2-prop-5 .statement tag=0BDV}

*令$X$为集合，令$(Z_i)_{i \in I}$为制服空间的族，令$(J_\lambda)_{\lambda \in L}$为$I$的划分，令$(Y_\lambda)_{\lambda \in L}$为由$L$索引的集合族。对于每个$\lambda \in L$，令$h_\lambda$为$X$到$Y_\lambda$的映射；对于每个$\lambda \in L$和每个$i \in J_\lambda$，让$g_{i\lambda}$是$Y_\lambda$的映射到$Z_i$；让$f_i = g_{i\lambda} \circ h_\lambda$。让每个$Y_\lambda$携带最粗糙的均匀结构，其中映射$g_{i\lambda}$（$i \in J_\lambda$）是均匀连续的。那么 $X$ 上 $f_i$ 均匀连续的最粗均匀结构与 $X$ 上 $h_\lambda$ 均匀连续的最粗均匀结构相同。*

### 4. 逆像统一性；制服子空间

令$X$为集合，$Y$将$X$统一为空间，$f$映射到$Y$。 $X$ 上的最粗均匀性$\mathfrak{U}$（其中$f$ 均匀连续）称为$Y$ 的均匀结构 $f$ 下的*逆像*。从no. 3的命题 4，以及从公式得出交的逆像，$Y$形式的随从的$g = f \times f$下的逆像是随从的基本系统 $\mathfrak{U}$。由$\mathfrak{U}$诱发的拓扑是$Y$的拓扑在$f$下的*逆像*（no. 3，命题4的推论）。

#### 注 {#top-ii-s2-n4-rem-1 .statement tag=0BDW}

如果$f : X \to Y$是满射，则$Y$的随从是$X$的随从的$g$下的直接像。

当且仅当$X'$均匀度的$f$下的逆像比$X$均匀度更粗糙时，均匀连续空间$X$到均匀空间$X'$的映射$f$是均匀连续的。

令$A$为均匀空间$X$的子集。由$X$的均匀性在$A$上引起的均匀性是后者在典范嵌入$A \to X$下的逆像。通过 no. 3 的命题 4，这相当于以下定义：

#### 定义 3 {#top-ii-s2-def-3 .statement tag=0BDX}

令$A$为均匀空间$X$的子集。 $A$上的均匀性，其周围的集合是$X$的周围的集合在$A \times A$上的迹，称为$X$的均匀性在$A$上引起的均匀性。

由$A$上的均匀性诱发的拓扑与$X$的拓扑在$A$上诱发的拓扑相同； 集合$A$，与$X$的均匀性和拓扑一起，称为$X$的均匀性子空间。

如果 $A$ 是均匀连续空间 $X$ 的子集并且 $f : X \to X'$ 是均匀连续映射，则限制 $f|A$ 是 $A$ 均匀连续映射 $X'$。如果$A' \subset X'$使得$f(X) \subset A'$，则$X$的映射进入$X'$的均匀子空间$A'$，与$f$具有相同的图，再次一致连续（no. 3，命题 4).

如果$B \subset A \subset X$，则$X$的制服子空间$B$与$X$的制服子空间$A$的制服子空间$B$相同（诱导制服的传递性） 结构；no. 3，命题5)。

#### 命题 6 {#top-ii-s2-prop-6 .statement tag=0BDY}

令 $A$ 为均匀空间 $X$ 的密集子集。然后，在$X \times X$，制服子空间$A$形式的随行人员关闭，这是$X$随行人员的基本系统。

$A \times A$ 在 $X \times X$ 中稠密（章 I, § 4, no. 3、命题 7）。令$V$为$A$的开放随从；它是交 $A \times A$ 以及开放的随从$U$ $X$。我们有$U \subset \overline{V}$（章I, § 1, no. 6，命题5），鉴于§ 1, no. 2，命题2的推论2，这个关系与$\overline{V} \subset \overline{U}$一起建立了命题。

### 5. 集合中最少上界的均匀性

集合$X$上的每个$(\mathfrak{U}_i)_{i \in I}$制服系列在$X$上所有制服的有序集合中至少有上界$\mathfrak{U}$；我们只需要no. 3中的应用命题 4，将$Y_i$视为集合$X$，均匀性为$\mathfrak{U}_i$，将$f_i$视为恒等映射$X \to Y_i$。由$\mathfrak{U}$引起的拓扑只是由$\mathfrak{U}_i$引起的拓扑中最小的上界。

从no. 3的命题4也可以得出，如果$X$不为空且$\mathfrak{U}_i$是$\mathfrak{U}_i$的随从过滤器，则$\mathfrak{U}$的随从过滤器是过滤器$\mathfrak{U}_i$中最小的上界（章） I, § 6, no. 2）。

#### 例 {#top-ii-s2-n5-exa-1 .statement tag=0BDZ}

如果$\varpi$是非空集合$X$的任何有限划分$(A_i)_{1 \leq i \leq n}$，则集合$V_\varpi = \bigcup_i (A_i \times A_i)$本身就构成$X$上均匀性$\mathfrak{U}_\varpi$的基本随从系统（§ 1, no. 1， 例2); $X$ (no. 2, 注 1) 上的有限划分的均匀性是均匀性 $\mathfrak{U}_\varpi$ 中最小的上界。

#### 注 {#top-ii-s2-n5-rem-1 .statement tag=0BE0}

$X$上的均匀度族$(\mathfrak{U}_i)$在$X$上所有均匀度的有序集合中也有下确界，即$X$上所有均匀度的集合中最小的上界，它们比每个$\mathfrak{U}_i$更粗糙（例如存在均匀性，因为 $X$ 上的所有均匀性中的集合至少有元素）。但是（假设$X$不为空）这种一致性的随行过滤器不一定是$\mathfrak{U}_i$的随行过滤器的交，因为后者过滤器不需要满足公理$(U_{III})$（习题4）。

### 6. 制服乘积空间

#### 定义 4 {#top-ii-s2-def-4 .statement tag=0BE1}

*如果*$(X_i)_{i \in I}$ *是一个制服空间的家族，那么这个家族的乘积制服空间就是乘积集合*
$$
X = \prod_{i \in I} X_i
$$
*具有最粗的均匀度，投影* $pr_i : X \to X_i$
* 是均匀连续的。这个均匀度被称为* $X_i$的均匀度的乘积，*和均匀度空间* $X_i$ *被称为* $X$的因子。

由$X$上的乘积均匀性引起的拓扑与$X_i$拓扑的乘积相同（no. 3，命题4的推论）。

#### 命题 7 {#top-ii-s2-prop-7 .statement tag=0BE2}

*让*$f = (f_i)$*成为制服空间*$Y$*的映射*变成乘积制服空间*$X = \prod_{i \in I} X_i$。 *则* $f$ *一致连续当且仅当每个* $f_i$ *一致连续*。

从$f_i = pr_i \circ f$开始，这是命题 4 of no. 3的特例。

#### 推论{#top-ii-s2-n6-cor-1 .statement tag=0BE3}

*令* $(X_i)_{i \in I}, (Y_i)_{i \in I}$ *为制服空间的两个系列，由相同的集合* $I$索引。 *对于每个*$i \in I$，*让*$f_i$*成为*$X_i$*的映射*进入*$Y_i$。 *如果* $f_i$ *中的每一个都是均匀连续的，那么乘积映射*
$$
f : (x_i) \to (f_i(x_i)).
$$
*相反，如果* $X_i$ *非空且* $f$ *一致连续，则每个* $f_i$ *一致连续。*

f 可以写成$x \to (f_i(\mathrm{pr}_i x))$，因此推论的第一个部分是从命题7得出的。第二个部分是通过考虑$\prod_{i \in I} X_i$的点$a = (a_i)$并重复章的论证来证明的I、no. 1、推论 1 到命题 1，其中短语“在$a$（分别$a_\kappa$）处连续”替换为“均匀连续”

初始均匀性传递性（no. 3，命题 5）的一般准则表明，对于拓扑空间（章I, § 4, no. 1）的乘积，均匀空间的乘积是结合律并且以下内容正确：

#### 命题 8 {#top-ii-s2-prop-8 .statement tag=0BE4}

*令$X$为集合，让$(Y_i)_{i \in I}$为制服空间的族，对于每个$i \in I$，让$f_i$为$X$到$Y_i$的映射。令$f$为$X$到$Y = \prod_{i \in I} Y_i$的映射$x \to (f_i(x))$，并令$U$为$X$上的最粗糙均匀度，其中$f_i$是均匀连续的。那么 $U$ 是逆像在 $f(X)$ 上由乘积均匀性在 $Y$ 上引起的均匀性的 $f$ 下。*

#### 推论{#top-ii-s2-n6-cor-2 .statement tag=0BE5}

*对于每个$i \in I$，令$A_i$为$Y_i$的子空间。那么$\prod_{i \in I} Y_i$上的乘积均匀度在$A = \prod_{i \in I} A_i$上引起的均匀度与子空间$A_i$均匀度的乘积相同。*

在加法中，我们立即看到，如果$X_1, X_2$是两个统一的空间并且$a_1$是$X_1$中的任何点，则映射$x_2 \to (a_1, x_2)$是$X_2$的同构到子空间$\{a_1\} \times X_2$ $X_1 \times X_2$；因此：

#### 命题 9 {#top-ii-s2-prop-9 .statement tag=0BE6}

*令$f$为乘积均匀连续空间$X_1 \times X_2$到均匀空间$Y$的均匀连续映射；然后每个部分映射*

$$
x_2 \to f(x_1, x_2)
$$

*$X_2$到$Y$是均匀连续的。*

在其他字中，两个参数的一致连续函数分别相对于它们中的每一个来说是一致连续的。

\* 章 I, § 4, no. 2、注 2 中给出的例，表明此命题的逆命题为假。 \*

### 7. 制服逆极限空间

令$I$为偏序集合，其中偏序写为$\alpha \leq \beta$。对于每个$\alpha \in I$，令$X_\alpha$为统一的空间，对于指标$\alpha, \beta$的每个对，使得$\alpha \leq \beta$令$f_{\alpha \beta}$为$X_\beta$到$X_\alpha$的映射。

我们可以说，$(X_\alpha, f_{\alpha\beta})$是均匀空间的逆系，如果（i）$(X_\alpha, f_{\alpha\beta})$是集合的逆系（cf.章I，附录，no. 1）并且（ii）每当 $\alpha \leq \beta$ 时，$f_{\alpha\beta}$ 一致连续。在 $X = \varprojlim X_\alpha$ 上，典范映射 $f_\alpha : X \to X_\alpha$ 均匀连续的最粗糙均匀度称为 $X_\alpha$ 均匀度的逆极限（相对于 $f_{\alpha\beta}$），而赋予这种最粗糙均匀度的集合 $X$ 称为逆极限制服逆系空间$(X_\alpha, f_{\alpha\beta})$。如果我们通过“均匀性”和“连续的映射”来计算替换“拓扑”，则在章、I、no. 4（命题 9 除外）中建立的拓扑空间的逆极限的所有属性仍然有效通过“均匀连续映射”。 加法

#### 命题 10 {#top-ii-s2-prop-10 .statement tag=0BE7}

令$I$为有向集合，令$(X_\alpha, f_{\alpha\beta})$为由$I$索引的均匀空间的逆系，并令$J$为$I$的共尾子集。对于每个$\alpha \in I$，令$f_\alpha$为$X = \varprojlim X_\alpha$到$X_\alpha$的典范映射，并令$g_\alpha$表示$f_\alpha \times f_\alpha$。那么集合$\overline{g}_\alpha^{-1}(V_\alpha)$的家庭，其中$\alpha$贯穿$J$，并且对于每个$\alpha \in J$，$V_\alpha$贯穿$X_\alpha$随行人员的基本系统，是随行人员的基本系统 $X$。

我们把证明留给读者；它是证明 of 命题 9 of 章 I, § 4, no. 4 的直接改编。

最后，由$X_\alpha$均匀性的逆极限在$X = \varprojlim X_\alpha$上导出的拓扑是$X_\alpha$拓扑的逆极限。

### 习题{#top-ii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
