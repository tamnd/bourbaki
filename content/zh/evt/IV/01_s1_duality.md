---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 1
section_title: Duality
lang: zh
source: evt-i-v
pdf_pages: 0183-0196, 0229-0234
extraction: ocr
subsections:
    - "no": 1
      title: Topologies compatible with a duality
      page: 0
      pdf_page: 183
    - "no": 2
      title: Mackey topology and weakened topology on a locally convex space
      page: 4
      pdf_page: 186
    - "no": 3
      title: Transpose of a continuous linear mapping
      page: 6
      pdf_page: 188
    - "no": 4
      title: Dual of a quotient space and of a subspace
      page: 8
      pdf_page: 190
    - "no": 5
      title: Dual of a direct sum and of a product
      page: 11
      pdf_page: 193
statements: 36
exercises: 25
content_sha256: a9f3debc9c7b903bf33bc732f75c62a94cd08e8c166efdeb9eb5ac4f99eedb88
translated_from: content/en/evt/IV/01_s1_duality.md
translation_method: google
source_content_sha256: b7f26d454273886007de38188e9c263540c6eccc68705afe146cbdcbcc0c7806
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 5d11a435a5b5d0cdf7402fee74413ba4d4de1db0694931e4dba6dc8006bd285c
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 1。二元性

### 1. 与对偶性兼容的拓扑

在这个截面中，E和F表示两个被双线性形式B（II，p. 40）对偶的向量空间。我们记得 (II, p. 41) 我们定义了两个线性映射

$$
d_B : F \to E^*, \quad s_B : E \to F^*
$$

其特征为关系

(1)
$$
B(x, y) = \langle x, d_B(y) \rangle = \langle y, s_B(x) \rangle
$$

对于$x \in E, \ y \in F$。

#### 定义 1 {#evt-iv-s1-def-1 .statement tag=07QI}

*如果 $d_B$ 是双射从 F 到通过将拓扑 $\mathscr{T}$ 分配给 E 获得的局部凸空间的对偶，则 E 上的局部凸拓扑 $\mathscr{T}$ 被认为与 E 和 F 之间的对偶性兼容。*

如果存在这样一个拓扑$\mathscr{T}$，则映射$d_B$是单射的，也就是说E和F的对偶性在F(II，p. 41)中分离。

#### 命题 1 {#evt-iv-s1-prop-1 .statement tag=07QJ}

(i) *E 中的闭凸子集对于 E 上的所有局部凸拓扑都是相同的，并且与 E 和 F 之间的对偶性兼容。*
(ii) *E 的有界子集对于 E 上的所有局部凸拓扑都是相同的，并且与 E 和 F 之间的对偶性兼容。*

令E上的$\mathscr{T}$为拓扑，与E和F之间的对偶性兼容，因此更细大于$\sigma(E, F)$。如果 E 的凸子集对于 $\mathscr{T}$ 是闭的，则它是闭实半空间（II，p. 38，cor. 1）的交，因此它对于 $\sigma(E, F)$ 是闭的。这就证明了(i)。 断言 (ii) 在 cor 中得到证明。 III、p. 27 中的 3 个。

让$F_\sigma$表示向量空间F，赋予弱拓扑$\sigma(F, E)$。然后线性映射 $s_B$ 映射 E 到 $F_\sigma$ 的对偶 $(F_\sigma)'$（II，p. 43，道具 3）。设$\mathfrak{S}$是$F_\sigma$的有界子集族。滥用语言，$(F_\sigma)'$上$\mathfrak{S}$拓扑的$s_B$下的逆像被称为$\mathfrak{S}\text{-topology on } E$。它由半范数族定义

$$
p_A(x) = \sup_{y \in A} |B(x, y)|,
$$

其中 A 穿过 $\mathfrak{S}$。特别是，当$\mathfrak{S}$是F的有限子集族时，$\mathfrak{S}$拓扑恰好是弱拓扑$\sigma(E, F)$。

#### 定义 2 {#evt-iv-s1-def-2 .statement tag=07QK}

*设E和F是对偶性中的两个空间。 E 上的 Mackey 拓扑，由 $\tau(E, F)$ 表示，被定义为 E 上的 $\mathfrak{S}$ 拓扑，其中 $\mathfrak{S}$ 是 F 的所有子集的族，其中 $E^*$ 中的像（$d_B$ 下）对于 $\sigma(E^*, E)$ 是凸的、平衡的和紧致的。*

当E和F之间的对偶性在F中分离时，$d_B$是单射的，F上的拓扑$\sigma(F, E)$是$E^*$上拓扑$\sigma(E^*, E)$的$d_B$下的逆像。在这种情况下，$\mathfrak{S}$由F的所有那些子集组成，这些子集对于$\sigma(F, E)$来说是凸的、平衡的和紧致的。

一般来说，如果$F_1 = d_B(F) \subset E^*$，并且如果我们用规范双线性形式$(x, x^*) \mapsto \langle x, x^* \rangle$到$E \times F_1$的$(x, y_1) \mapsto B_1(x, y_1)$限制表示，则E和$F_1$通过$B_1$置于对偶性中，并且这种对偶性在$F_1$中分离，因为定义我们有 $B(x, y) = B_1(x, d_B(y))$，def。 2表明$\tau(E, F) = \tau(E, F_1)$。

#### 注 1 {#evt-iv-s1-n1-rem-1 .statement tag=07QL}

— 设 A 为 Hausdorff 局部凸空间 G 的紧凸子集，$\tilde{A}$ 为 A 的闭凸平衡包络。当域 K 为 $\mathbf{R}$ 时，集合 $\tilde{A}$ 为$A \cup (-A)$ 的闭凸包络；当K为$\mathbf{C}$时，集合$\tilde{A}$包含在$2A \cup (-2A) \cup (2iA) \cup (-2iA)$的闭凸包络内。因而（II，p. 14，命题 15），$\tilde{A}$ 是紧致的。

我们特别推论，当 E 和 F 之间的对偶性在 F 中分离时，*Mackey 拓扑 $\tau(E, F)$ 也是 $\mathfrak{S}'$ 拓扑，其中 $\mathfrak{S}'$ 是 F 的所有凸子集的集合，对于 $\sigma(F, E)$* 是紧致的。以类似的方式，我们在 F 上定义 Mackey 拓扑 $\tau(F, E)$。

#### 定理 1（麦基）{#evt-iv-s1-thm-1 .statement tag=07QM}

— *设 E 和 F 为对偶性中的两个空间；假设对偶性在 F 中分离。在阶中，E 上的局部凸拓扑 $\mathscr{T}$ 与 E 和 F 之间的对偶性兼容，$\mathscr{T}$ 比拓扑 $\sigma(E, F)$ 更细且比 Mackey 拓扑 $\tau(E, F)$ 更粗糙是充分必要的。*

认同 F 及其像在 $E^*$ 下$d_B$。令 $\mathfrak{S}_0$ 表示 F 的所有子集中的集合，对于 $\sigma(F, E)$ 是凸的、平衡的且紧致的。通过定义，$\tau(E, F)$是E上的$\mathfrak{S}_0$拓扑，因此更细比$\sigma(E, F)$。

#### 引理 1 {#evt-iv-s1-lem-1 .statement tag=07QN}

*E* 的子空间 F 由 E 上的所有线性形式组成，这些线性形式对于$\tau(E, F)$ 是连续的。

F 的每个元素对于$\sigma(E, F)$来说都是连续的映射，因此对于$\tau(E, F)$来说。

相反，令 $f \in E^*$ 对于 $\tau(E, F)$ 是连续的。 E 中存在 0 的邻域 U（对于 $\tau(E, F)$），使得 U 上有 $|f| \leq 1$；我们可以假设存在集合$A \in \mathscr{S}_0$使得$U = A^\circ$。在其他字中，$f$属于到A的双极性$A^{\circ\circ}$，对于$E^*$和E之间的对偶性。但是F上的拓扑$\sigma(F, E)$是由$\sigma(E^*, E)$诱导的；因而，对于 $\sigma(E^*, E)$，A 是凸的、平衡的且紧致的，并且双极子（II、p. 44、第 1）的定理意味着等式 $A = A^{\circ\circ}$。因此我们有 $f \in F$，由此得出引理。

#### 引理 2 {#evt-iv-s1-lem-2 .statement tag=07QO}

*令$\mathscr{T}$为E上的局部凸拓扑，使得E上的每个线性形式对于$\mathscr{T}$属于到F都是连续的。那么$\mathscr{T}$比$\tau(E, F)$更粗糙。*

*令$\mathscr{U}$为凸的集合，对于$\mathscr{T}$平衡邻域为0。令$\mathscr{S}$为$\mathscr{U}$的元素F中极点的集合。由科。 III、p. 17 中的 2 个，我们有 $\mathscr{S} \subset \mathscr{S}_0$，据我所知。 1 道具。 III、p. 19、$\mathscr{T}$的7与$\mathscr{S}'$拓扑相同，其中$\mathscr{S}'$是E的对偶$E'$中$\mathscr{U}$的集合极地的集合。但是$E' \subset F$，由假设，因而$\mathscr{S}'$的每个集合都包含在$\mathscr{S}$的集合中；和引理如下。*

令E上的$\mathscr{T}$为拓扑，并兼容E和F之间的对偶性。则$\mathscr{T}$比$\tau(E, F)$粗引理2，显然$\mathscr{T}$比$\sigma(E, F)$粗更细。相反，对于拓扑 $\tau(E, F)$ (引理 1) 和拓扑 $\sigma(E, F)$ (II, p. 43，命题 3)，F 是 E 的对偶，因此对于$\tau(E, F)$ 和 $\sigma(E, F)$ 之间的每个拓扑也是如此。

#### 推出 {#evt-iv-s1-n1-cor-1 .statement tag=07QP}

*设 p 为 E 上的半范数。以下条件是等价的：*

(i) *p 对于拓扑 $\tau(E, F)$ 是连续的；*
(ii) *E 上的每个线性形式 f，使得 $|f| \leq p$ 来自 F 的元素。*

(i) $\Rightarrow$ (ii) : 如果 p 对于 $\tau(E, F)$ 连续，则 E 上的每个线性形式 f 使得 $|f| \leq p$ 对于 $\tau(E, F)$ 连续，因此来自 F 的元素引理 1。

(ii) $\Rightarrow$ (i) ：令 $\mathscr{T}$ 为由半范数 p 定义的 E 上的拓扑。如果满足条件 (ii)，则 E 上的线性形式对于 $\mathscr{T}$ 属于到 F 是连续的。通过引理 2 $\mathscr{T}$ 比 $\tau(E, F)$ 更粗糙，因而 p 对于 $\tau(E, F)$ 是连续的。

#### 注 2 {#evt-iv-s1-n1-rem-2 .statement tag=07QQ}

*设 K 是 F 的凸子集，对于弱拓扑 $\sigma(F, E)$ 是紧致的，$\mu$ 是 K 的正测度。 Put*

$$
p(x) = \int_K |B(x, y)| \, d\mu(y)
$$

对于所有$x \in E$。 p 是半范数是直接的。此外，对于每个 $x \in E$，关系 « $|B(x, y)| \leq 1$ 对于所有 $y \in K$ » 意味着$p(x) \leq \mu(K)$。这证明了 E 上的半范数 p 对于 Mackey 拓扑 $\tau(E, F)$ 是连续的。 \*

#### 例 {#evt-iv-s1-n1-exa-1 .statement tag=07QR}

设 G 是局部凸空间，G' 是其对偶。在 G' 上，凸紧收敛的弱拓扑 $\sigma(G', G)$ 和拓扑 (III, p. 14) 与 G' 和 G 之间的对偶性相容。一般来说，G' 上紧致收敛的强拓扑和拓扑与 G' 和 G 之间的对偶性不相容。 然而回想一下，当 G 是 Hausdorff 时且 G' 重合上的紧致收敛的准完备性拓扑与凸紧致收敛 (III, p. 8) 的准完备性，因此与 G' 和 G 之间的对偶性兼容。

#### 定义 3 {#evt-iv-s1-def-3 .statement tag=07QS}

*设E和F是对偶性中的两个向量空间，并且$\mathscr{T}$是F的子集族，其边界为$\sigma(F, E)$。那么 F 上的 $\mathscr{T}$ 拓扑表示为 $\beta(E, F)$。*

类似地，我们对F进行定义拓扑$\beta(F, E)$。很容易看出拓扑$\beta(E, F)$与$\beta(E, F/E^\circ)$相同，并且我们可以约化到E和F之间的对偶性在F中分离的情况。

*注。 —* 3) 令 $E_\sigma$ 表示空间 E，赋予拓扑 $\sigma(E, F)$。 $E_\sigma$中的桶（III、p. 24）是E的子集，对于$\sigma(E, F)$来说是凸面、平衡封闭且吸水的。这些正是 F 的子集极点，它们是凸的、平衡的并且以 $\sigma(F, E)$ 为界。因而，对于 E 中的拓扑 $\beta(E, F)$，$E_\sigma$ 中所有桶的族是邻域的 0 的基本系统。在其他字中，E 上的半范数对于 $\beta(E, F)$ 是连续的当且仅当它对于 $\sigma(E, F)$ 是下半连续时（*cf.* III、p. 24，道具 1）。

4) 令E上的$\mathscr{T}$为拓扑，并与E和F之间的对偶性兼容。 1、(ii) F 上的IV、p. 1、拓扑$\beta(F, E)$ 正是 F 上的强拓扑，当 F 等同于 E 的对偶时（与拓扑 $\mathscr{T}$）。

5) E 上的拓扑 $\beta(E, F)$ 比 $\tau(E, F)$ 更细。一般来说，它与 E 和 F 之间的对偶性不兼容（*cf.* 然而 § 2）。特别是，E 的子集以 $\sigma(E, F)$ 为界，但不一定以 $\beta(E, F)$ 为界。

### 2. Mackey 拓扑和弱化拓扑在局部凸空间上

设 E 为局部凸空间，E' 为对偶。我们通过$E \times E'$上的规范双线性形式$(x, x') \mapsto \langle x, x' \rangle$将E和E'置于对偶性中。这种二元性在E'中分离。我们将考虑 E 上与 E 和 E' 之间的对偶性兼容的三种拓扑：

a) E 上给定的拓扑，每当可能出现任何混淆时，我们将其称为*初始拓扑*；

b) 拓扑 $\sigma(E, E')$，称为 E 上*弱化的拓扑*；

c) 拓扑 $\tau(E, E')$，称为 E 上的 *Mackey 拓扑*。

初始拓扑比弱化的拓扑更细，比Mackey拓扑更粗糙；此外，这三种拓扑可以是不同的（IV，p. 49，练习8）。

通过道具。 IV、p. 1中的第1个，这三种拓扑具有相同的闭凸集合、相同的桶、相同的有界集合和相同的适应出生学。尤其 ：

#### 命题 2 {#evt-iv-s1-prop-2 .statement tag=07QT}

*令 E 为局部凸空间，并令 A 为 E 的凸子集（例如，E 的向量子空间）。 A 的闭包对于 E 的初始拓扑和弱化的拓扑是相同的。*

#### 注 1 {#evt-iv-s1-n2-rem-1 .statement tag=07QU}

对于 E 的元素的族 $(x_i)_{i \in I}$ 对于初始拓扑而言是完全的（即拓扑独立），对于弱化的拓扑来说也是充分的；这是从道具得出的。 2. 因此我们可以应用II、p. 43中的判据。

#### 注 2 {#evt-iv-s1-n2-rem-2 .statement tag=07QV}

令$\mathscr{T}_1$和$\mathscr{T}_2$是E上的两个局部凸拓扑，与E和$E'$之间的对偶性兼容，$\mathscr{T}_1$是更细比$\mathscr{T}_2$。然后 $\mathscr{T}_1$ 的每个邻域为 0，对于 $\mathscr{T}_1$ 来说是凸且封闭的，通过 prop，对于 $\mathscr{T}_2$ 来说也是封闭的。 1 个IV、p. 1。因而，(GT, II, § 3, No. 3, 推论) E 的每个子集对于 $\mathscr{T}_2$ 来说都是完整的，对于 $\mathscr{T}_1$ 也是如此。

特别是，对于弱化的拓扑来说，E的每个子集对于初始拓扑来说是完整的，对于初始拓扑来说，E的每个子集对于Mackey拓扑来说也是如此。如果 E 对于弱化的拓扑是准完备的，那么对于每个与 ​​E 和 $E'$ 之间的对偶性兼容的拓扑也是如此。如果说初始拓扑是准完整的，那么Mackey拓扑也是如此。

#### 注 3 {#evt-iv-s1-n2-rem-3 .statement tag=07QW}

假设 E 是 Hausdorff（对于初始拓扑）。设 A 为 E 的子集，它对于 $\sigma(E, E')$ 是闭集且有界的，因此对于每个拓扑也与 E 和 $E'$ 之间的对偶性兼容。由于 A 对于 $\sigma(E, E')$ (III、p. 3、注 5) 是预紧的，因此假设 A 对于 $\sigma(E, E')$ 是*紧*，则相当于 A 对于 $\sigma(E, E')$ 是*完全*。

因此，由于注 2，我们看到：

#### 命题 3 {#evt-iv-s1-prop-3 .statement tag=07QX}

*假设 E 是 Hausdorff，$E'$ 是它的对偶。 E 的每个子集对于初始拓扑是预紧的，对于 $\sigma(E, E')$ 是紧的，对于初始拓扑是紧的。*

#### 注 4 {#evt-iv-s1-n2-rem-4 .statement tag=07QY}

拓扑 $\beta(E, E')$（IV、p. 4，定义 3）比 Mackey 拓扑更细。如果$\beta(E, E')$与$\tau(E, E')$不同，则它与E和$E'$之间的对偶性不兼容。当且仅当初始拓扑等于 $\beta(E, E')$（III，p. 24）时，空间 E 才被桶装。

#### 命题 4 {#evt-iv-s1-prop-4 .statement tag=07QZ}

*设 E 为局部凸空间。在以下每种情况下，E 上的 Mackey 拓扑与初始拓扑相同：*

a) E 是桶装的；
b) E 是出生学的；
c) E 是可度量的。

我们首先注意到，E 上的 Mackey 拓扑与初始拓扑相同，当且仅当 $E'$ 的每个凸子集（对于 $\sigma(E', E)$ 来说是紧致的）是等连续的。如果 E 是桶装的（III、p. 24、推论），情况肯定是这样。

假设E是天生的；令 V 为 E 中拓扑 $\tau(E, E')$ 的凸且平衡的邻域为 0。设 B 为 E 的子集，以初始拓扑为界。由于 B 以 Mackey 拓扑为界，V 吸收 B，并且由于 E 是出生学的，因此对于初始拓扑，V 是 0 的邻域。

在情况 c) 中，空间 E 是出生学的（III，p. 12，道具 2）。

### 3. 连续线性映射的转置

在此截面、$E_1$和$E_2$表示两个局部凸的空间，分别具有对偶$E'_1$和$E'_2$。

令$u$为从$E_1$到$E_2$的线性映射。当$E_1$和$E_2$被分配弱化拓扑时，为了使$u$连续，对于所有$f \in E'_2$，$f \circ u$属于到$E'_1$是必要且充分的；如果 $u$ 是连续的，就是这种情况。那么从$E'_2$到$E'_1$的线性映射$f \mapsto f \circ u$称为$u$的转置，记为$^t u$。

#### 命题 5 {#evt-iv-s1-prop-5 .statement tag=07R0}

*令$u$为从$E_1$到$E_2$的连续线性映射。*

(i) *如果 $E_1$ 和 $E_2$ 是 Hausdorff，则 $u$ 是单射当且仅当 $^t u$ 的像对于弱拓扑 $\sigma(E'_1 : E_1)$ 来说是密集于 $E'_1$ 的。*

(ii) *要使 $^t u$ 成为单射，$u$ 的像在 $E_2$ 中稠密是必要且充分的。*

$E_2$的向量子空间对于初始拓扑来说是稠密的，当且仅当它对于弱化的拓扑来说是稠密的（IV，p. 4，道具2）。然后，第 5 号提案是从 II、p. 47 得出的。 2.

#### 命题 6 {#evt-iv-s1-prop-6 .statement tag=07R1}

*令$u$为从$E_1$到$E_2$的线性映射，这对于弱化拓扑是连续的。对于$i = 1, 2$，令$\mathfrak{S}_i$是$E_i$的有界子集族。在阶中，$^t u$是从$(E'_2)_{\mathfrak{S}_2}$到$(E'_1)_{\mathfrak{S}_1}$的连续映射，对于每一个集合$A \in \mathfrak{S}_1$，在$\mathfrak{S}_2$和实数中存在集合$A_1, ..., A_n$是充分必要的$\lambda > 0$使得$\lambda \cdot u(A)$包含在$A_1 \cup ... \cup A_n$\脚注{在其他字中，$u(\mathfrak{S}_1)$包含在最小的改编的出生学中包含$\mathfrak{S}_2$（III， p. 3).}.*

这是道具的直接的推论。 2 个III、p. 15。

#### 推论 {#evt-iv-s1-n3-cor-1 .statement tag=07R2}

*令$u$为从$E_1$到$E_2$的连续线性映射。当对偶 $E'_i$ 被分配以下拓扑时，$^t u$ 是连续的：*
a) *弱拓扑$\sigma(E'_i, E_i)$;*
b) *强拓扑$\beta(E'_i, E_i)$;*
c) *麦基拓扑$\tau(E'_i, E_i)$;*
d) *预紧收敛的拓扑。*
*此外，如果 $E_2$ 是 Hausdorff，则当对偶 $E'_i$ 被赋值时，$^t u$ 是连续的：*
e) *紧致收敛拓扑*（分别为*紧凸*）。

唯一需要证明的点是情况c)，此时$E_1$和$E_2$的拓扑不一定是Hausdorff。那么对于每个线性形式$f \in E'_1*$，$f \circ ^t u$在$E'_2$上就是线性形式；因而，对于拓扑$\sigma(E'_1*, E'_1)$和$\sigma(E'_2*, E'_2)$，存在线性映射$v : E'_1* \to E'_2*$，并且$d_{B_2} \circ u = v \circ d_{B_1}$是连续的，其中$d_{B_i}$是从$E_i$到$E'_i*$（$i = 1, 2$）的典范映射。因而，如果 $A$ 是 $E_1$ 的子集，使得 $d_{B_1}(A)$ 对于 $\sigma(E'_1*, E'_1)$ 是凸的、平衡的和紧致的，那么 $d_{B_2}(u(A)) = v(d_{B_1}(A))$ 对于 $\sigma(E'_2*, E'_2)$ 是凸的、平衡的和紧致的，因为拓扑 $\sigma(E'_1*, E'_1)$ 和 $\sigma(E'_2*, E'_2)$ 是 Hausdorff。

#### 命题 7 {#evt-iv-s1-prop-7 .statement tag=07R3}

— 设 $u : E_1 \to E_2$ 为线性映射。我们假设$u$对于$E_1$和$E_2$的弱化拓扑是连续的。

(i) 如果 $E_1$ 和 $E_2$ 被分配了它们的 Mackey 拓扑，映射 $u$ 是连续的。

(ii) 如果$E_1$是天生的或桶状的，则$u$对于$E_1$和$E_2$的初始拓扑是连续的。

(iii) 在阶中，$u$对于$E_1$和$E_2$的初始拓扑是连续的，$E_2'$的每个等连续的子集的$'u$下的像在$E_1'$中是等连续的是充分必要的。

假设意味着$'u$对于弱拓扑$\sigma(E_2', E_2)$和$\sigma(E_1', E_1)$（II，p. 46，推论）是连续的，因此对于$\sigma(E_2', E_2)$，像在$'u$的凸、平衡和紧致子集下对于 $\sigma(E_1', E_1)$ 是凸、平衡且紧的，拓扑 $\sigma(E_2', E_2)$ 和 $\sigma(E_1', E_1)$ 是 Hausdorff。因此，断言 (i) 由 GT，X, § 1, No. 4，道具得出。 3、b）。 断言 (ii) 是 (i) 的推论 ：因为，如果 $E_1$ 是天生的或桶装的，则其初始拓扑是 Mackey 拓扑，并且 $E_2$ 的 Mackey 拓扑比拓扑的初始拓扑更细 $E_2$。最后，$E_i$的初始拓扑是$E_i'$的等连续子集的一致收敛（III，p. 19，第7条的相关1）。这就证明了(iii)。

#### 推论 {#evt-iv-s1-n3-cor-2 .statement tag=07R4}

— 假设 $E_1$ 是规范的空间。设$u$是从$E_1$到$E_2$的线性映射。以下属性是等效的：

a) $u$是连续的；

b) 对于弱化拓扑，$u$ 是连续的；

c) $u$下$E_1$中的单位球的像在$E_2$内；

d) 对于初始拓扑，$E_1$的点的序列$(x_n)$趋于0，序列$(u(x_n))$对于$E_2$的弱化拓扑有界。

由于 a) 和 b) 的 $E_1$ 是出生学的等价，因此可以从 prop 得出。 7； a)和c)的值是直接的。 a) 和 d) 的等价由命题得出。 1 of IV、p. 1，以及来自 prop。 III、p. 11 中的 1 个。

#### 命题 8 {#evt-iv-s1-prop-8 .statement tag=07R5}

— (i) 令 $E$ 为范数空间，具有对偶 $E'$。对于每个 $x \in E$，我们有

$$
\|x\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x, x' \rangle|.
$$

(ii) 设$E_1$和$E_2$是两个规范的空间和$u$，从$E_1$到$E_2$的连续线性映射。我们有

$$
\|u\| = \|t u\|.
$$

让$x \in E$。对于每个$x' \in E'$使得$\|x'\| \leq 1$，我们有

$$
|\langle x, x' \rangle| \leq \|x\| \cdot \|x'\| \leq \|x\|.
$$

根据Hahn-Banach 定理（II，p. 23，cor.2），$E'$中存在元素$x'$，使得$\|x'\| \leq 1$和$\langle x, x' \rangle = \|x\|$。这就证明了(i)。

现在让我们证明(ii)。通过公式 (3) 和转置的定义，我们有

$$
\|^{t}u\| = \sup_{\|y'\| \leq 1} \|^{t}u(y')\| = \sup_{\|y'\| \leq 1, \|x\| \leq 1} |\langle x, ^{t}u(y') \rangle|
= \sup_{\|x\| \leq 1, \|y'\| \leq 1} |\langle u(x), y' \rangle| = \sup_{\|x\| \leq 1} \|u(x)\| = \|u\|.
$$

#### 注 1 {#evt-iv-s1-n3-rem-1 .statement tag=07R6}

公式 (3) 是 (4) 的特例，从 K 到 E 的相应的到线性映射 $\lambda \mapsto \lambda x$。

#### 注 2 {#evt-iv-s1-n3-rem-2 .statement tag=07R7}

将 $B(x, y') = \langle u(x), y' \rangle = \langle x, ^{t}u(y') \rangle$ 替换为 $x \in E_1,\ y' \in E'_2$。上述证明表明B是$E_1 \times E'_2$上的连续双线性形式，其中范数（GT，X, § 3, No. 2）等于$\|u\|$。

#### 推论 {#evt-iv-s1-n3-cor-3 .statement tag=07R8}

— *令 $\dot{E}$ 为规范的空间满足第一个可数性公理。存在 $E' - \{0\}$ 的可数子集 D，这样我们有*

$$
\|x\| = \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\|
$$

*对于所有人*$x \in E$。

令 B' 为 E 的对偶 $E'$ 的单位球，并为其分配了弱拓扑 $\sigma(E', E)$。那么 B' 是一个紧凑的可度量空间 (III, p. 19, cor. 2)；因此 B' 中存在可数稠密子集 D'。输入$D = D' \cap (E' - \{0\})$。设 $x \in E$； 映射 $x' \mapsto \langle x, x' \rangle$ 从 B' 到 K 是连续的，因此

$$
\sup_{x' \in B'} |\langle x, x' \rangle| = \sup_{\xi \in D'} |\langle x, \xi \rangle| \leq \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\| \leq \|x\|.
$$

公式 (5) 现在由 (3) 得出。

### 4. 商空间和子空间的双重

在整个截面中，E表示局部凸空间，E的M向量子空间，以及$M^\circ$E的对偶$E'$中M的正交。令$p$为从E到$E/M$的典范映射；那么 $^{t}p$ 是单射的，有像 $M^\circ$，因此定义向量空间同构 （非拓扑）

$$
\pi : (E/M)' \to M^\circ .
$$

类似地，令 $i$ 为从 M 到 E 的典范嵌入。则 $^{t}i$ 是满射（II，p. 24，命题 2）；它的核等于$M^\circ$，我们得到向量空间同构（非拓扑）

$$
i : E'/M^\circ \to M'.
$$

#### 命题 9 {#evt-iv-s1-prop-9 .statement tag=07R9}

— (i) *为了使* $(E/M)'$ 的子集 A 等连续，* $\pi(A)$ *是* $E'$ 的等连续子集是充分必要的。

(ii) 设$\mathfrak{S}$为$E$的有界子集的集合，以及$E/M$中的子集$A \in \mathfrak{S}$的像的$\mathfrak{S}_1$集合。那么$\pi$是从$(E/M)'_{\mathfrak{S}_1}$到$M^\circ$的同构，其中$M^\circ$被分配为$E'_{\mathfrak{S}}$的拓扑。

(iii) 假设$E$是一个有范数的空间，那么$\pi$是从有范数的空间$(E/M)'$到$E'$的有范数子空间$M^\circ$的等距。

设$A$为$(E/M)'$和$B = {}^t p(A) \subset E'$的子集。放
$$
q(\xi) = \sup_{\xi' \in A} |\langle \xi, \xi' \rangle|
$$
对于所有$\xi \in E/M$。在阶中$A$等连续，从$E/M$到$\overline{\mathbf{R}}_+$的映射$q$是连续半范数是充分必要的。这意味着$q \circ p$是$E$的连续半范数（II，p. 27，第5条，（ii））。既然我们有
$$
(q \circ p)(x) = \sup_{x' \in B} |\langle x, x' \rangle|
$$
对于所有 $x \in E$，这又意味着 $B$ 在 $E'$ 中是等连续的，并且 (i) 如下。

令$A \in \mathfrak{S}$和$f$是$E/M$上的连续线性形式。对于每个$\lambda \in \mathbf{R}_+$，我们在$p(A)$上有$|f| \leq \lambda$当且仅当$|{}^t p(f)| \leq \lambda$在$A$上；因此(ii)。

最后我们证明(iii)。设$y'$在$(E/M)'$中。 $E/M$中的元素具有范数$< 1$当且仅当$E$中的范数$< 1$的元素$p$之下时像。因此
$$
\begin{align*}
\|y'\| &= \sup_{y \in E/M, \|y\| < 1} |\langle y, y' \rangle| = \sup_{x \in E, \|x\| < 1} |\langle p(x), y' \rangle| \\
&= \sup_{x \in E, \|x\| < 1} |\langle x, {}^t p(y') \rangle| = \|{}^t p(y')\|,
\end{align*}
$$
以及 ${}^t p$ 诱导从 $(E/M)'$ 到 $M^\circ$ 的等距。

#### 命题 10 {#evt-iv-s1-prop-10 .statement tag=07RA}

— (i) 为了使$M'$的子集$A$等连续，只要像位于$E'$的等连续子集的${}^t i$之下即可。

(ii) 假设 $M$ 在 $E$ 中闭合。令$\mathfrak{S}$为有界子集的$E$由……组成的覆盖，并令$\mathfrak{S}_1$为$A$为形式$M \cap A$$M$子集集合 $\mathfrak{S}$。从 $E'_{\mathfrak{S}}/M^\circ$ 到 $M'_{\mathfrak{S}_1}$ 的双射线性映射 $i$ 是连续的。如果关系 $\subset$ 的 $\mathfrak{S}$ 是有向集合，并且由闭凸和 $\sigma(E, E')$ 的紧集组成，则它是同胚。

(iii) 如果假设$E$是标准化的，则$i$是从$E'/M^\circ$到$M'$的等距。

$E'$的等连续子集在${}^t i$下的像是$M'$的等连续子集（IV，p. 7，道具7）。相反，令 $A$ 为 $M'$ 的等连续子集。 $M$的拓扑由$E$上的连续半范数的限制到$M$的集合定义。因此，在$E$上存在连续半范数$p$，使得$|f(x)| \leq p(x)$对于所有$f \in A$和所有$x \in M$。令$B$为$E$上所有线性形式$g$的集合，使得$|g| \leq p$且其限制至$M$属于至$A$。 集合 $B$ 在 $E'$ 等连续；由 Hahn-Banach 定理 (II, p. 23, cor. 1)，我们有 ${}^t i(B) = A$，因此 (i) 如下。

我们现在证明(ii)。通过道具。 IV，p. 6，线性映射${}^t i$从$E'_{\mathfrak{S}}$到$M'_{\mathfrak{S}_1}$是连续的，定义，由经过到商，从线性映射$\iota$连续$E'_\mathscr{S}/M^\circ$ 到$M'_{\mathscr{S}_1}$。令$\mathscr{T}$为$M'$上的拓扑，通过将$E'_\mathscr{S}/M^\circ$的$\iota$转移得到；这是更细比 $\mathscr{S}_1$ 拓扑。

现在假设$\mathscr{S}$对于$\subset$来说是有向集合，并且由闭、凸、平衡和紧集对于$\sigma(E, E')$组成。为了证明$\iota$是同胚，*即*$\mathscr{T}$比$M'$上的$\mathscr{S}_1$拓扑更粗糙，只需证明$\mathscr{T}$与$M'$和$M$之间的对偶性兼容，并且每个等连续$M$中的集合（被视为$M$与$\mathscr{T}$的对偶）包含在集合属于与$\mathscr{S}_1$的拟似中。由于$\mathscr{T}$比$\mathscr{S}_1$拓扑是更细，并且$\mathscr{S}_1$是$M$的覆盖，因此对于每个$y \in M$，$M'$上的线性形式$y' \mapsto \langle y, y' \rangle$对于$\mathscr{T}$是连续的。令$f$为$M'$上的线性形式，对于$\mathscr{T}$连续；那么$f \circ \iota$是$E'_\mathscr{S}$上的连续线性形式。 $E'$上的$\mathscr{S}$拓扑比Mackey拓扑$\tau(E', E)$更粗糙；因为，映射$d_B : E \to {E'}^*$对于拓扑$\sigma(E, E')$和$\sigma({E'}^*, E')$是连续的，并且由于后者是Hausdorff，因此集合的$d_B$下的像对于$\sigma(E, E')$是紧致的对于$\sigma({E'}^*, E')$是紧致的。通过IV、p. 3的引理 1，存在$x_0 \in E$，使得$f(\iota(x')) = \langle x_0, x' \rangle$对于所有$x' \in E'$。特别是，对于所有$x' \in M^\circ$，$\langle x_0, x' \rangle = 0$，并且由于$M$在$E$关闭，我们有$x_0 \in M$（II，p. 45，cor.2）；最后，为所有 $y' \in M'$ 提供 $f(y') = \langle x_0, y' \rangle$。这证明$\mathscr{T}$ *与* $M$ *和* $M'$之间的对偶性兼容。

现在令$A$为$M$的子集，对于$M'$上的拓扑$\mathscr{T}$等连续。根据$\mathscr{T}$的定义，并且考虑到$\mathscr{S}$有向假设，这意味着存在集合$B \in \mathscr{S}$包含0并且使得数$|\langle y, x' \rangle|$的上界$\lambda$为$y \in A$ 和 $x' \in B^\circ$ 是有限的（III、p. 19，第 7 条）。由于$B$在$E$闭合，双极的定理（II，p. 44，第1）表明我们有$A \subset \lambda(B \cap M)$；这样就完成了 (ii) 的证明。

现在我们要证明(iii)。让$y' \in M'$。我们将证明公式

$$
\|y'\| = \inf_{\iota(x') = y'} \|x'\|.
$$

通过道具。 8、(ii) IV、p. 7，我们有$\|\iota\| = \|i\|$，所以$\|\iota\| \leq 1$，以及

$$
\|y'\| \leq \inf_{\iota(x') = y'} \|x'\|.
$$

根据Hahn-Banach 定理（II，p. 23，cor.3），$E$上存在线性形式$x'_0$，其中扩展$y'$与范数相同；因此，由于$\iota(x'_0) = y'$，我们得到与(7)相反的不等式。

#### 注{#evt-iv-s1-n4-rem-1 .statement tag=07RB}

— 我们知道（II，p. 48，命题 7，(ii)）$\iota$ 是从 $E'_s/M^\circ$ 到$M'_s$ 的拓扑向量空间同构（弱对偶）。对于拓扑的紧致凸收敛，支柱。图10显示，当$E$是Hausdorff并且$M$在$E$闭合时，从$E'_{cc}/M^\circ$到$M'_{cc}$，$\iota$是同构。对于强拓扑，$\iota$是从$E'_b/M^\circ$到$M'_b$连续的映射；如果 $E$ 是 Banach 空间 \* 或者如果 $E$ 是半反身且 $M$ 闭于 $E$ (IV, p. 15) *，则它是同构，但如果 $E$ 是一个则情况并非总是如此Fréchet 空间（IV，p. 58，练习 5，*c*））。

#### 命题 11 {#evt-iv-s1-prop-11 .statement tag=07RC}

— (i) *在* $E/M$ 上削弱拓扑 *是在* $E$ 上的商； *在* $M$ 上减弱拓扑 *由* $E$ 引起。

(ii) *E/M 上的 Mackey 拓扑是 E 上的商； M 上的 Mackey 拓扑更细比 τ(E, E') 引起的拓扑更细。*

断言 (i) 由命题得出。 7 个II、p. 48。

对于弱化拓扑，典范嵌入$i : M \to E$是连续的，因此对于麦基拓扑$\tau(M, M')$和$\tau(E, E')$（IV，p. 7，第7条）。类似地，规范的投影 $p : E \to E/M$ 对于 Mackey 拓扑是连续的。我们立即看到，从$\tau(E, E')$获得的$E/M$上的商拓扑与$E/M$和$(E/M)'$之间的对偶性兼容，因此比Mackey的定理在$E/M$上的Mackey拓扑更粗糙（IV，p. 2，第 1）。这就证明了(ii)。

### 5. 直和和乘积的双重

对于每个$i \in I$，令$(E_i, F_i)$为向量空间、集合的对偶性双线性形式$B_i$的对。我们放置$E = \prod_{i \in I} E_i$和$F = \bigoplus_{i \in I} F_i$，我们将认同每个$F_i$和$F$的子空间。我们通过双线性形式将$E$和$F$置于对偶中

$$
B(x, y) = \sum_{i \in I} B_i(x_i, y_i) \quad \text{for} \quad x = (x_i) \quad \text{and} \quad y = (y_i)
$$

（家庭$(B_i(x_i, y_i))_{i \in I}$有有限支撑）。

我们记得（II，p. 50，命题8），弱拓扑$\sigma(E, F)$是弱拓扑$\sigma(E_i, F_i)$的乘积。

#### 引理 3 {#evt-iv-s1-lem-3 .statement tag=07RD}

— (i) *对于每个$i \in I$，令$\mathfrak{S}_i$是$F_i$的子集族，其边界为$\sigma(F_i, E_i)$；把$\mathfrak{S} = \bigcup_{i \in I} \mathfrak{S}_i$。那么$E$上的$\mathfrak{S}$拓扑就是$E_i$上$\mathfrak{S}_i$拓扑的乘积。*

(ii) *对于每个$i \in I$，让$\mathfrak{J}_i$是空间$E_i$上的适应出生学，赋予弱拓扑$\sigma(E_i, F_i)$，没有一个等于$\{ \varnothing \}$。 令$\mathfrak{J}$为$E = \prod_{i \in I} E_i$的子集$A$族，使得$\operatorname{pr}_i(A) \in \mathfrak{J}_i$适用于所有$i \in I$。 那么$F$上的$\mathfrak{J}$拓扑就是$F_i$上$\mathfrak{J}_i$拓扑的直和。*

令 $\mathscr{T}$ 为 $\mathfrak{S}_i$ 拓扑中的乘积。 集合 / 形式

$$
A = \prod_{i \in J} A_i^\circ \times \prod_{i \in I - J} E_i
$$

其中$J \subset I$是有限的，$A_i \in \mathfrak{S}_i$对于所有$i \in J$，形式对于$\mathscr{T}$来说邻域的基本系统为0。我们有$A = (\bigcup_{i \in J} A_i)^\circ$，因此$\mathscr{T}$与$\mathfrak{S}$拓扑相同。这就证明了(i)。

我们将$\mathfrak{J}$拓扑分配给$F$，将$\mathfrak{J}_i$拓扑分配给每个$F_i$。对于$E$的每一个子集$A$，我们都有$F_i \cap A^\circ = \operatorname{pr}_i(A)^\circ$，因此从$F_i$到$F$的单射是连续的。设$q$为$F$的半范数；我们假设$q$到$F_i$的限制$q_i$对于所有$i \in I$都是连续的。然后我们可以找到非空子集 $A_i \in \mathfrak{J}_i$ 这样我们有

$$
q_i(y_i) \leq \sup_{x_i \in A_i} |B_i(x_i, y_i)| \quad (y_i \in F_i) .
$$

把$A = \prod_{i \in I} A_i$；然后$A \in \mathfrak{J}$。对于$F$中的$y = (y_i)_{i \in I}$，我们有
$$
q(y) \leq \sum_{i \in I} q_i(y_i) \leq \sum_{i \in I} \sup_{x_i \in A_i} |B_i(x_i, y_i)| = \sup_{x \in A} |B(x, y)|,
$$
其中最后一个等式是从（8）得出的，因为族$(y_i)_{i \in I}$有有限支撑并且$A_i$非空并且可以假设是平衡的（GT，IV, § 5, No. 7，cor.2到prop.12）。这个不等式证明$q$在$F$上连续，因此(ii)。

#### 命题 12 {#evt-iv-s1-prop-12 .statement tag=07RE}

*拓扑$\beta(F, E)$是拓扑$\beta(F_i, E_i)$的直和。 拓扑 $\beta(E, F)$ 是拓扑$\beta(E_i, F_i)$ 的乘积。*

我们将申请引理 3，取$\mathfrak{S}_i$所有子集或$F_i$的家庭，其范围为$\sigma(F_i, E_i)$，而$\mathfrak{J}_i$则为$E_i$的所有子集的家庭，其范围为$\sigma(E_i, F_i)$。

由科。 III、p. 4、$\mathfrak{J}$中的2是$E_i$的所有子集的族，其边界为$\sigma(E_i, F_i)$的乘积拓扑，与$\sigma(E, F)$相同。因此我们的 $\beta(F, E)$ 上的断言如下。

我们赋予$F = \bigoplus_{i \in I} F_i$以拓扑$\mathscr{T}$，这是拓扑$\sigma(F_i, E_i)$的直和。那么$F$的对偶由线性形式$y \mapsto B(x, y)$组成，其中$x$穿过$E$（II，p. 30，道具6）。通过道具。 IV、p. 1 中的 1 个，拓扑$\mathscr{T}$ 和 $\sigma(F, E)$ 具有相同的有界集合。首先假设拓扑$\sigma(F_i, E_i)$是Hausdorff。通过道具。 III、p. 5中的 5 个，这些集合包含在形式 $\sum_{i \in J} B_i$ 的子集中，其中 $J \subset I$ 有限，$B_i$ 限制在 $F_i$（对于 $\sigma(F_i, E_i)$） $i \in J$。由于$\sum_{i \in J} B_i$包含在$\bigcup_{i \in J} nB_i$的凸包络中，其中$n = \mathrm{Card}(J)$，我们可以应用引理 3，在这种情况下证明断言在$\beta(E, F)$上。

对于一般情况，对于$\sigma(F_i, E_i)$，令$N_i$为0的所有邻域中的交，并令$N = \sum_{i \in I} N_i$；那么$F/N$是$F_i/N_i$的拓扑直和（II，p. 31，命题8）；由此我们推断，以$\mathscr{T}$为界的$F$的每个子集都包含在形式$N + \sum_{i \in J} B_i$的集合中，其中$J \subset I$有限，并且对于所有$i \in J$，$B_i$以$F_i$为界（III、p. 2、*注* 3）；由于$E$中这个集合的极坐标与$\sum_{i \in J} B_i$的极坐标相同，所以结果如上。

#### 命题 13 {#evt-iv-s1-prop-13 .statement tag=07RF}

*Mackey 拓扑 $\tau(F, E)$ 是 Mackey 拓扑 $\tau(F_i, E_i)$ 中的直和。 拓扑 $\tau(E, F)$ 是拓扑 $\tau(E_i, F_i)$ 的乘积。*

$\tau(F, E)$ 上的断言由引理 3 (ii) 和以下性质得出：对于$F^* = \prod_{i \in I} F_i^*$ 的封闭、凸且平衡的子集对于$\sigma(F^*, F)$ 而言是紧凑的，其在每个$F_i^*$ 上的投影是充分必要的紧凑型$\sigma(F_i^*, F_i)$。

为了证明$\tau(E, F)$上的断言，首先假设拓扑$\sigma(F_i, E_i)$是Hausdorff，则足以证明$F$的每个子集$A$对于$\sigma(F, E)$是凸的、平衡的和紧的，都包含在(引理 3 (i)) 形式 $\sum_{i \in J} A_i$的集合，其中$J \subset I$是有限的，而$A_i$对于$\sigma(F_i, E_i)$来说是凸的、平衡的和紧致的。但这样的子集是有界于$\sigma(F, E)$的。通过证明的道具。 12、存在$I$的有限子集$J$使得$A \subset \sum_{i \in J} F_i$，在$F_i$上取$A$的$A_i$投影就足够了。

在一般情况下，与 prop 的证明相同的记号 。 12，我们有$\tau(E_i, F_i) = \tau(E_i, F_i/N_i)$和$\tau(E, F) = \tau(E, F/N)$（IV，p. 2），并且由于$F/N$是$F_i/N_i$的拓扑直和，我们已经简化为前面的情况。

Q.E.D.

对于本段的其余部分，我们假设 $(E_i)_{i \in I}$ 是局部凸空间的族。让$S$表示$E_i$和$P$的拓扑直和，即它们的乘积。我们定义线性映射$\theta : S' \to \prod_{i \in I} E_i'$，据说是*规范*，由

$$
\theta(x') = (x'|E_i)_{i \in I} \quad (x' \in S')
$$

（其中$S'$表示$S$的对偶，$E_i'$表示$E_i$的对偶）。

#### 命题 14 {#evt-iv-s1-prop-14 .statement tag=07RG}

(i) *映射$\theta$是同构从$S = \bigoplus_{i \in I} E_i$的强（或弱）对偶到$E_i$的强（或弱）对偶的乘积：*

(ii) *为了使$S'$的子集$A$等连续，$\theta(A)$的投影到$E_i'$对于所有$i \in I$来说是等连续的。*

(iii) *Mackey 拓扑 $\tau(S, S')$ 是 Mackey 拓扑 $\tau(E_i, E_i')$ 的直和。*

(iv) *拓扑$\beta(S, S')$是拓扑$\beta(E_i, E_i')$的直和。*

$\theta$ 是双射，紧接着拓扑直和的定义（II，p. 30，命题 6）。 断言 (i) 然后从道具得出。 12 of IV、p. 12，对于强拓扑，来自 prop。 II、p. 50 中的 8 个，用于弱拓扑。类似地，(iii) 由命题得出。 13（IV，p. 12）和（iv）来自道具。 12（IV，p. 12）。

为了证明 (ii)，令 $A$ 为 $S'$ 的子集。放

$$
q(x) = \sup_{x' \in A} |\langle x, x' \rangle| \quad \text{for} \quad x \in S ;
$$

让$q_i$表示$q$到$E_i$、从而的限制

$$
q_i(x_i) = \sup_{x_i' \in A_i} |\langle x_i, x_i' \rangle| \quad \text{for} \quad x_i \in E_i ,
$$

其中$A_i$表示$E_i'$上$\theta(A)$的投影。为了使 $A$ 等连续，$q$ 是有限的（即每个 $q_i$ 是有限的）并且连续是充分必要的。鉴于拓扑直和上的连续半范数刻画（II，p. 27，命题5），这与假设每个$q_i$是连续的，或者事实上，每个集合$A_i$是等连续的。

令$\phi$为线性映射，据说是*规范*，从$\bigoplus_{i \in I} E_i'$到$P = \prod_{i \in I} E_i$的对偶$P'$，由公式定义

$$
\langle x, \phi(x') \rangle = \sum_{i \in I} \langle x_i, x'_i \rangle
$$

对于$P$中的$x = (x_i)$和$\bigoplus_{i \in I} E'_i$中的$x' = (x'_i)$。

#### 命题 15 {#evt-iv-s1-prop-15 .statement tag=07RH}

— (i) *映射 $\phi$ 是同构，从$E_i$ 强对偶的拓扑直和到$P = \prod_{i \in I} E_i$ 的强对偶。*

(ii) *要使$P'$的子集$A$等连续，它包含在有限的和$\sum_{i \in J} \phi(A_i)$中是必要且充分的，其中$J \subset I$是有限的，并且对于所有$i \in J$，$A_i$在$E'_i$中等连续。*

(iii) *Mackey 拓扑 $\tau(P, P')$ 是拓扑 $\tau(E_i, E'_i)$ 的乘积。*

(iv) *拓扑$\beta(P, P')$是拓扑$\beta(E_i, E'_i)$的乘积。*

$\phi$ 是单射的，直接的。 $P$ 中 0 的邻域的基本系统由形式 $V = \prod_{i \in J} V_i \times \prod_{i \in I - J} E_i$ 的集合组成，其中 $J \subset I$ 是有限的，$V_i$ 是 $E_i$ 中 0 的邻域， $i$在$J$。 $P'$中$V$的极坐标等于$\sum_{i \in J} \phi(V_i^0)$。

这证明了 $\phi$ 和断言 (ii) 的满射性。

断言 (i) 和 (iv) 由命题得出。 12 (IV, p. 12) 和 (iii) 来自道具。 13（IV，p. 12）。

#### 推论 {#evt-iv-s1-n5-cor-1 .statement tag=07RI}

— *每乘积桶装空间都是桶装。*

当且仅当初始拓扑与 $\beta(E, E')$ (IV, p. 4, *注 3*) 相同时，局部凸空间 $E$ 才是桶形的。因此应用 prop 就足够了。 15（四）。

### 习题 {#evt-iv-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
