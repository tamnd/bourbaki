---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 3
section_title: Spaces of continuous linear mappings
lang: zh
source: evt-i-v
book_pages: TVS III.13-TVS III.23, TVS III.41-TVS III.43
pdf_pages: 0145-0155, 0173-0175
extraction: ocr
subsections:
    - "no": 1
      title: The spaces $\mathscr{L}_\mathfrak{S}(E; F)$
      page: 13
      pdf_page: 145
    - "no": 2
      title: Condition for $\mathscr{L}_\mathfrak{S}(E; F)$ to be Hausdorff
      page: 15
      pdf_page: 147
    - "no": 3
      title: Relations between $\mathscr{L}(E; F)$ and $\mathscr{L}(\hat{E}; F)$
      page: 15
      pdf_page: 147
    - "no": 4
      title: Equicontinuous subsets of $\mathscr{L}(E; F)$
      page: 16
      pdf_page: 148
    - "no": 5
      title: Equicontinuous subsets of $E'$
      page: 19
      pdf_page: 151
    - "no": 6
      title: The completion of a locally convex space
      page: 20
      pdf_page: 152
    - "no": 7
      title: $\mathscr{S}$-bornologies on $\mathscr{L}(E; F)$
      page: 21
      pdf_page: 153
    - "no": 8
      title: Complete subsets of $\mathscr{L}_{\mathscr{S}}(E; F)$
      page: 22
      pdf_page: 154
statements: 39
exercises: 13
content_sha256: dfc25c3c6e0ba67365f5c1f3b8b981fd39fb7e5552b4f141645414bac46b7a17
translated_from: content/en/evt/III/03_s3_spaces_of_continuous_linear_mappings.md
translation_method: google
source_content_sha256: cf2d3140178ddd9a073d777e8eb5efd04f0920704426c6cc3aa6359b95506798
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 91b1eeb0a681e121c6bdb89a2ecf41104a373be1960359ead4d5b72f34e7416e
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 3。连续空间线性映射

### 1. The spaces $\mathscr{L}_\mathfrak{S}(E; F)$

设 F 为拓扑向量空间，E 为任意集合，$\mathfrak{S}$ E 的子集系列。考虑向量空间 $F^E$ 与 $\mathfrak{S}$ 收敛性的一致结构（GT，X, § 1, No. 2）。我们知道这个结构与$F^E$的交换律群结构兼容（GT，X, § 1, No. 4，cor.2）。这样推导出来的拓扑称为$\mathfrak{S}$*-拓扑*。如果X是$F^E$的子集，或更一般地，集合与映射$j : X \to F^E$，则$F^E$上$\mathfrak{S}$*-拓扑*的j下的宇宙像称为$\mathfrak{S}$*-拓扑* X。

#### 注 {#evt-iii-s3-n1-rem-1 .statement tag=07MJ}

— 1) $\mathfrak{S}$*-拓扑*与$\mathfrak{S}'$*-拓扑*相同，其中$\mathfrak{S}'$表示$\mathfrak{S}$（III，p. 1）生成的出生学。

2) 令F中的$M \in \mathfrak{S}$且V为0的邻域；让$T(M, V)$表示所有$f \in F^E$中的集合，这样对于每个$x \in M$都有$f(x) \in V$。如果 $\mathfrak{S}$ 在有限并下稳定，则对于$F^E$ 的 $\mathfrak{S}$*-拓扑*，邻域的基本系统为 0，集合 $T(M, V)$ 形式 。

#### 命题 1 {#evt-iii-s3-prop-1 .statement tag=07MK}

*设 E 为集合，$\mathfrak{S}$ E 的子集系列，F 为拓扑向量空间，H 向量子空间 $F^E$。在阶中，$\mathfrak{S}$*-拓扑*与H的向量空间结构兼容，对于每个$u \in H$和每个$M \in \mathfrak{S}$，$u(M)$在F中有界是充分必要的。此外，如果 F 是局部凸的，则 H 上的 $\mathfrak{S}$*-拓扑* 是局部凸的。*

考虑到上面的注 1) 和 2)，我们看到$\mathfrak{S}$*-拓扑*与H的向量空间结构兼容的必要且充分的条件是集合$H \cap T(M, V)$在H中*吸收*（I， p. 7，道具 4)；但这意味着对于 F 中的每个 $u \in H$、每个子集 $M \in \mathfrak{S}$ 以及每个平衡 0 的邻域 V，都存在 $\lambda \neq 0$ 使得 $u(M) \subset \lambda V$；也就是说 (III, p. 2) $u(M)$ 有界于 F。最后，命题的最后一个断言由以下事实得出：如果 V 是凸的，则 $T(M, V)$ 也是凸的。

#### 推论{#evt-iii-s3-n1-cor-1 .statement tag=07ML}

*设E和F是两个局部凸空间，$\mathfrak{S}$E的有界子集族，以及从E到F的连续线性映射的$\mathscr{L}(E; F)$向量空间。则$\mathfrak{S}$*-拓扑*与向量空间结构兼容$\mathscr{L}(E; F)$ 并且是局部凸的。*

如果$u$是从E到F的连续线性映射并且M是E的有界子集，则$u(M)$在F中有界（III，p. 4，cor.1），注就足够了。

给定两个局部凸向量空间 E 和 F，以及 E 的有界子集的族 $\mathfrak{S}$，令 $\mathscr{L}_\mathfrak{S}(E; F)$ 表示通过将 $\mathfrak{S}$*-topology* 分配给 $\mathscr{L}(E; F)$ 获得的局部凸空间。

#### 例 1 {#evt-iii-s3-n1-exa-1 .statement tag=07MM}

如果$\mathfrak{S}$是E的所有有限子集中的集合，则$\mathfrak{S}$拓扑是*简单收敛*的拓扑，并且空间$\mathscr{L}_{\mathfrak{S}}(E; F)$也由$\mathscr{L}_s(E; F)$表示。 $\mathscr{L}_s(E; F)$ 有界子集称为 $\mathscr{L}(E; F)$ 简单有界子集。

#### 例 2 {#evt-iii-s3-n1-exa-2 .statement tag=07MN}

如果$\mathfrak{S}$是*compact*（分别是*预紧*、*紧凸*）子集的集合，则$\mathfrak{S}$拓扑称为*compact*（分别是*预紧*、*紧凸*）收敛的拓扑，并且空间$\mathscr{L}_{\mathfrak{S}}(E; F)$也是由$\mathscr{L}_c(E; F)$（分别为$\mathscr{L}_{pc}(E; F)$、$\mathscr{L}_{cc}(E; F)$）表示。 （*参见* IV、p. 48、练习 7。）

#### 例 3 {#evt-iii-s3-n1-exa-3 .statement tag=07MO}

如果$\mathfrak{S}$是E的所有*有界*子集的集合，我们说$\mathfrak{S}$拓扑是*有界收敛*的拓扑，并且空间$\mathscr{L}_{\mathfrak{S}}(E; F)$由$\mathscr{L}_b(E; F)$表示。

#### 例 4 {#evt-iii-s3-n1-exa-4 .statement tag=07MP}

当$F = \mathbf{K}$、空间$\mathscr{L}(E; F)$是E的*对偶*$E'$时。我们用$E'_\mathfrak{S}$、$E'_s$等表示。空间$\mathscr{L}_{\mathfrak{S}}(E; \mathbf{K})$、$\mathscr{L}_s(E; \mathbf{K})$等空间 $E'_s$（或$E'_b$）称为E 的弱对偶（或强对偶）。$E'_s$（或$E'_b$）的有界子集被称为弱（或强）有界。我们观察到$E'$上的弱拓扑不是别人，正是$\sigma(E', E)$（II，p. 42）。

当$E = F$时，我们用$\mathscr{L}(E)$、$\mathscr{L}_{\mathfrak{S}}(E)$等表示。空间、$\mathscr{L}(E; F)$、$\mathscr{L}_{\mathfrak{S}}(E; F)$等。

令 $p$ 为 F 和 M 上的连续半范数，且以 E 的子集为界。令

$$
p_M(u) = \sup_{x \in M} p(u(x)) .
$$

$p_M$是$\mathscr{L}(E; F)$上的半范数直接的，如果$\Gamma$是F上半范数的基本系统，则半范数族$p_M$，其中$p$范围超过$\Gamma$，M范围超过基对于$\mathfrak{S}$生成的出生学来说，是$\mathscr{L}_{\mathfrak{S}}(E; F)$半范数的基本系统。

特别是，如果 E 和 F 是半范数空间，并且如果 $p$（分别为 $q$）表示 E（分别为 F）的半范数，则 $\mathscr{L}(E; F)$ 上有界收敛的拓扑由半范数定义

$$
r(u) = \sup_{p(x) \leq 1} q(u(x))
$$

（*cf.* GT，X, § 3, No. 2）。当我们将$\mathscr{L}_b(E; F)$视为半范数空间时，我们始终将除非（反之亦然）表示半范数（2）。如果 F 是赋范空间，则半范数 (2) 是范数。

#### 注 {#evt-iii-s3-n1-rem-2 .statement tag=07MQ}

— 3) 设 A 为 E 的单位稠密子集球。鉴于$u$的连续性，我们也有

$$
r(u) = \sup_{x \in A} q(u(x)) .
$$

例

$$
r(u) = \sup_{p(x) < 1} q(u(x)) .
$$

因为我们有 $u(tx) = tu(x)$ 对应 $t \in \mathbf{R}$，所以我们还有，

$$
r(u) = \sup_{p(x) = 1} q(u(x)) = \sup_{p(x) \neq 0} \frac{q(u(x))}{p(x)} .
$$

每当$p \neq 0$。

4) 公式 (2) 表明映射 $u \mapsto r(u)$ 是$\mathscr{L}_s(E; F)$ 上的下半连续。

#### 命题 2 {#evt-iii-s3-prop-2 .statement tag=07MR}

— 令 E 和 F 为两个局部凸空间，并令 $\mathfrak{S}$ 为 E 的有界子集的集合。

1) $\mathscr{L}(E; F)$上的$\mathfrak{S}$-拓扑与$\tilde{\mathfrak{S}}$-拓扑相同，其中$\tilde{\mathfrak{S}}$表示最小的改编，E上的出生学（III，p. 3），其中包含$\mathfrak{S}$。

2) 假设$\{0\}$在F中不稠密，并令$\mathfrak{S}'$为E的有界子集的另一个集合。则当且仅当$\mathfrak{S}' \subset \tilde{\mathfrak{S}}$时，$\mathfrak{S}'$拓扑比$\mathfrak{S}$拓扑更粗糙。

令$u \in \mathscr{L}(E; F)$、$M \in \mathfrak{S}$并令$p$为F上的连续半范数。由于$p \circ u$是E上的连续半范数，这与说相同，$p \circ u$在M上或在M的封闭凸平衡包络$\tilde{M}$上以1为界；在其他字中，我们有$p_M = p_{\tilde{M}}$。此外，很明显，对于所有$\lambda > 0$和$p_{M \cup M'} = \sup(p_M, p_{M'})$，我们有$p_{\lambda M} = \lambda p_M$，第一个断言随之而来，因为$\tilde{\mathfrak{S}}$具有$\mathfrak{S}$的集合的有限并的闭凸平衡包络的相似性集合为基。

现在我们证明第二个断言：首先，如果F是基域，则从定义得出，$E' = \mathscr{L}(E; F)$上的$\tilde{\mathfrak{S}}$拓扑具有0的邻域的基本系统，集合的极点集合 $\tilde{\mathfrak{S}}$。令 A 为 E 的有界子集，对于 $\tilde{\mathfrak{S}}$ 拓扑，其极$A^\circ$ 为 0 的邻域；那么存在一个闭凸平衡集合$B \in \tilde{\mathfrak{S}}$使得$A^\circ \supset B^\circ$，所以$A \subset B^{\circ \circ}$；但由科。 II、p. 45 中的 3 个，我们有 $B^{\circ \circ} = B$，因此有 $A \subset B$ 和 $A \in \tilde{\mathfrak{S}}$。因此，如果$\mathfrak{S}'$是E的有界子集的集合，当且仅当$\mathfrak{S}' \subset \tilde{\mathfrak{S}}$时，$\mathfrak{S}'$拓扑比$E'$上的$\mathfrak{S}$拓扑更粗糙。一般情况立即如下，因为如果 $y \in F$ 不在 0 的闭包中，我们可以验证映射使得 $f \in E'$ 对应到映射 $x \mapsto f(x)\ y$ 是局部凸空间 $E'_\mathfrak{S}$ 的同构到其上$\mathscr{L}_{\tilde{\mathfrak{S}}}(E; F)$ 中的像。

### 2. 条件 $\mathscr{L}_\mathfrak{S}(E; F)$ 为 Hausdorff

#### 命题 3 {#evt-iii-s3-prop-3 .statement tag=07MS}

— 令 E 和 F 为两个局部凸空间，F 假设为 Hausdorff，并令 $\mathfrak{S}$ 为 E 的有界子集族。如果 $\mathfrak{S}$ 的集合的并 A 在 E 中总计，则空间 $\mathscr{L}_\mathfrak{S}(E; F)$ 为 Hausdorff。

令$u_0$为$\mathscr{L}(E; F)$的非零元素；由于 $u_0$ 是连续的，并且 A 在 E 中是全的，因此 A 中存在$x_0$，使得$u_0(x_0) \neq 0$。由于 F 是 Hausdorff，因此 F 中存在 0 的邻域 V，使得 $u_0(x_0) \notin V$。令$M \in \mathfrak{S}$ 使得$x_0 \in M$。然后所有$u \in \mathscr{L}(E; F)$的集合U，使得$u(M) \subset V$是$\mathscr{L}(E; F)$中0的邻域，并且我们有$u_0 \notin U$，因此$\mathscr{L}(E; F)$是Hausdorff。

特别是，只要 F 是 Hausdorff ，$\mathscr{L}(E; F)$ 上的以下拓扑都是 Hausdorff：简单收敛、紧致收敛、预紧紧凸或有界收敛。

### 3. 关系 $\mathscr{L}(E; F)$ 和 $\mathscr{L}(\hat{E}; F)$ 之间

令E和F为两个Hausdorff局部凸空间，并假设F是完备的；令 $\hat{E}$ 为 E 的补全。由于从 E 到 F 扩展的每个连续线性映射 $u$ 唯一地到从 $\hat{E}$ 到 F 的连续线性映射 $\bar{u}$，我们可以确定空间 $\mathscr{L}(E; F)$ 并且$\mathscr{L}(\hat{E}; F)$由映射$u \mapsto \bar{u}$。在加法中，令$\mathfrak{S}$是E的有界子集族； $\mathscr{L}(E; F)$ 重合上的$\mathfrak{S}$拓扑与$\mathscr{L}(\hat{E}; F)$上的$\mathfrak{S}$拓扑以及$\hat{\mathfrak{S}}$拓扑，其中$\hat{\mathfrak{S}}$表示集合的$\hat{E}$中的闭包族$\mathfrak{S}$。

对于例，如果 E 是 *normed*，$\mathscr{L}(E; F)$ 上有界收敛的拓扑与 $\mathscr{L}(\hat{E}; F)$ 上有界收敛的拓扑相同：因为，$\hat{E}$ 的每个有界子集都包含在 E 的有界子集的闭包中。 $\hat{E}$的单位球是E的单位球的闭包，由公式 (3) (III, p. 14)得出，如果F是Banach空间，映射$u \mapsto \bar{u}$是等距$\mathscr{L}(E; F)$ 到$\mathscr{L}(\hat{E}; F)$。

我们观察到，如果 E 不是规范的空间，则可能存在 $\hat{E}$ 的有界子集，它们不包含在 E 的任何有界子集的闭包中（对于例，如果 E 是无限维 Banach 空间的弱对偶）；然而，如果 E 是可度量的并且满足可数性第一公理（III，p. 39，练习 16），情况就会如此。

### 4. $\mathscr{L}(E; F)$ 等连续子集

设E和F是两个局部凸空间。为了使 $\mathscr{L}(E; F)$ 的子集 H 等连续，它在 E 中的点 0 处等连续是必要且充分的（I，p. 9，命题 6）；这意味着对于 F 中的每个邻域 V 0，集合 $\bigcap_{u \in H} u^{-1}(V)$ 是 E 中的 0 邻域；或者对于 F 上的每个连续半范数 $p$，函数 $\sup_{u \in H} (p \circ u)$ 是 E 上的连续半范数。此外，(I，p. 5)，H 是一致等连续的。我们注等连续子集的凸平衡包络线是等连续的，因为如果$p$是F上的连续半范数并且$\tilde{H}$H的凸平衡包络线，对于H中的$u_i$，我们有不等式$p \circ (\sum_i \lambda_i u_i) \leq \sum_i |\lambda_i| \cdot (p \circ u_i)$，因而$\sup_{u \in H} (p \circ u) = \sup_{u \in \tilde{H}} (p \circ u)$。

因而，等连续子集族是$\mathscr{L}(E; F)$上的凸出生学（III，p. 2，def.2）。

#### 命题 4 {#evt-iii-s3-prop-4 .statement tag=07MT}

*设E、F为两个局部凸空间，F为Hausdorff。令从E到F的所有映射中的空间$F^E$被分配为简单收敛的拓扑。然后*

(i) *从 E 到 F 的线性映射的集合在 $F^E$ 内闭合。*

(ii) *如果 H 是 $\mathscr{L}(E; F)$ 的等连续子集，则 $F^E$ 中 H 的闭包 $\overline{H}$ 包含在 $\mathscr{L}(E; F)$ 中并且是等连续的。*

我们知道 $\overline{H}$ 是等连续的（GT，X, § 2, No. 3，第 6 条）。尚需证明断言(i)。令x、y在E中，$\lambda, \mu$在K中，并令$A(x, y, \lambda, \mu)$为所有$u \in F^E$中的集合，使得

$$
u(\lambda x + \mu y) - \lambda u(x) - \mu u(y) = 0 .
$$

这个集合在$F^E$是封闭的，因为从$F^E$到F的映射$u \mapsto u(x)$对于每个$x \in E$都是连续的，并且因为F是Hausdorff。但从 E 到 F 的线性映射的集合等于

$$
\bigcap_{x,y,\lambda,\mu} A(x, y, \lambda, \mu) .
$$

因而，这个集合在$F^E$中关闭。

#### 推论 1 {#evt-iii-s3-prop-4-cor-1 .statement tag=07MU}

— *对于 $\mathscr{L}(E; F)$ 的等连续子集 H 在 $\mathscr{L}_s(E; F)$ 中相对紧致，对于所有 $x \in E$、所有 $u(x)$ 的集合 $H(x)$，当 $u$ 范围超过 H 时，在 F 中相对紧致是必要和充分的。*

事实上，这个条件对于$\overline{H}$在$F^E$中是紧致的是充分必要的（GT，I, § 9, No. 5，cor.）。

#### 推论 2 {#evt-iii-s3-prop-4-cor-2 .statement tag=07MV}

— *E 的对偶 $E'$ 的每个等连续子集对于 $E'$* 上的弱拓扑 $\sigma(E', E)$ 来说是相对紧的（III、p. 14、例 4）。

因为，如果H是$E'$的等连续子集，则$\sup_{u \in H} |u|$是E上的连续半范数；特别是，对于每个 $x \in E$，集合 $H(x)$ 都是有界的，因此在域标量中相对紧凑。

#### 推出 3 {#evt-iii-s3-prop-4-cor-3 .statement tag=07MW}

— *在半规范空间 E 的强对偶 $E'_b$ 中，每个闭球对于弱拓扑 $\sigma(E', E)$ 来说都是紧凑的。*

此球也因 $\sigma(E', E)$ 关闭。

#### 命题 5 {#evt-iii-s3-prop-5 .statement tag=07MX}

— *令 E 和 F 为两个局部凸空间，并令 T 为 E 的总子集。在 $\mathscr{L}(E; F)$ 的每个等连续子集 H 上，以下一致结构重合：*

1) *T中简单收敛的一致结构；*
2) *E中简单收敛的一致结构；*
3) *E 的预紧子集中均匀收敛结构。*

我们回想起（III，p. 15，道具2）$\mathscr{L}(E; F)$重合上的$\mathfrak{S}$拓扑与$\tilde{\mathfrak{S}}$拓扑，其中$\tilde{\mathfrak{S}}$是适应E的最小的出生学和包含$\mathfrak{S}$。

在道具的叙述中。 5，因此我们可以通过“处处密集”来实现替换字“总计”。然后从等连续集合 (GT, X, § 2, No. 4, th. 1) 的一般性质得出命题。

#### 例 {#evt-iii-s3-n4-exa-1 .statement tag=07MY}

— *1) 令$\mu$为$\mathbf{R}$的勒贝格测度，令E为半范数空间$\mathscr{L}^p(\mu)$ ($1 \leq p < \infty$) (INT, IV)。对于每个数字函数$f$和每个实数$h$，令$f_h$为函数$x \mapsto f(x - h)$。显然映射 $f \mapsto f_h$ 定义从 E 到自身的线性等距。如果 $f$ 是连续的并且具有紧支撑，则 $f_h$ 均匀收敛于 $f$，因此也是阶 $p$ 的均值，因为 $h$ 趋于 0。由于具有紧支撑的所有连续函数的集合 $\mathscr{K}(\mathbf{R})$ 是稠密的在 E 中，E 的线性等距的集合是等连续的，由命题得出。 5 对于每个 $f \in E$，$f_h$ 收敛于阶 $p$ 到 $f$，因为 $h$ 趋于 0。

对于 $p = 1$，考虑傅里叶变换，它与 $\mathbf{R}$ 上的每个 $f \in \mathscr{L}^1(\mu)$ 函数 $\hat{f}$ 相关联，定义为

$$
\hat{f}(y) = \int e^{-2i\pi xy} f(x) \, d\mu(x) .
$$

线性形式 $f \mapsto \hat{f}(y)$的集合是$\mathscr{L}^1(\mu)$的对偶的等连续子集。

另一方面，我们知道所有特征函数闭有界区间的集合 T 是$\mathscr{L}^1(\mu)$的总子集；我们很容易验证，对于所有$f \in T$，傅里叶变换$\hat{f}$是一个连续的函数趋于无穷大零。我们推断这对于所有$f \in \mathscr{L}^1(\mu)$都成立（“黎曼-勒贝格定理”）。

关系$\sup_{y \in \mathbf{R}} |\hat{f}(y)| \leq \|f\|_1$表明映射$f \mapsto \hat{f}$是$\mathbf{R}$上所有有界函数从$\mathscr{L}^1(\mu)$到空间$\mathscr{B}(\mathbf{R})$的连续映射，且结构一致收敛。由于$\hat{f}$对于所有$f \in T$都是连续的，因此$\hat{f}$对于所有$f \in L^1(\mu)$都是连续的。 $\hat{f}$趋于无穷远零的事实源于以下事实：所有连续函数趋于无穷远零的子空间$C_0(\mathbf{R})$在$\mathscr{B}(\mathbf{R})$处闭合。

2) 令E为$\mathbf{R}$上所有连续数值函数的空间，赋予拓扑紧致收敛性。令 K 为 $\mathbf{R}$ 的紧致子集，令 $(\mu_n)$ 为 $\mathbf{R}$ 上测度的序列，并有 K 的支持。假设所有 n 都为 $\|\mu_n\| \leq 1$。那么 $\mu_n$ 的集合就是 E' 的等连续子集。因此，如果对于每个函数$f \in E$，我们有$\lim_{n \to \infty} \mu_n(f) = 0$，函数$x \mapsto \int e^{itx} d\mu_n(t)$的序列收敛于0，均匀地在$\mathbf{R}$的每个紧凑子集上（从函数的集合开始） $t \mapsto e^{itx}$，因为 x 的范围超过 $\mathbf{R}$ 的紧致子集，因此在 E) 中是紧致的。 \*

#### 推论{#evt-iii-s3-n4-cor-1 .statement tag=07MZ}

— *假设 F 是豪斯多夫。设 H 是 $\mathscr{L}(E; F)$ 的等连续子集。如果 H 上的滤波器 $\Phi$ 从 E 到 F 简单地收敛到映射 $u_0$，则 $u_0$ 是从 E 到 F 的连续线性映射，并且 $\Phi$ 在 E 的每个预紧子集上均匀收敛到 $u_0$。*

第一个断言来自 prop. 4 (III, p. 16) 和 prop 中的第二个。 5（III，p. 17）。

#### 命题 6 {#evt-iii-s3-prop-6 .statement tag=07N0}

— *令 H 为 $\mathscr{L}(E; F)$ 的等连续子集。如果F是可度量的，并且E中存在可数总集合，则E中简单收敛的H上的一致结构是可度量的。如果在加法中，F中存在可数总集合，则H中存在可数处处稠密集合（对于E的紧子集一致收敛的拓扑）。

令$(a_n)$为E中的总序列。则映射$u \mapsto (u(a_n))$是$\mathscr{L}(E; F)$的同构，其中$\mathscr{L}(E; F)$具有$a_n$的集合简单收敛的一致结构，穿上子空间 $F^\mathbf{N}$ 的制服。如果 F 是可度量的（分别是可度量的并且满足可数性的第一个公理），那么对于 $F^\mathbf{N}$ 也是如此（GT，IX, § 2, No. 4，cor.2 和§ 2, No. 8，推论），并且命题由命题得出。 5（III，p. 17）。

#### 推论 1 {#evt-iii-s3-prop-6-cor-1 .statement tag=07N1}

— *令 E 为局部凸可度量空间，F 为标准化空间。假设 E 和 F 都是满足可数性第一公理。那么$\mathscr{L}(E; F)$是等连续子集的可数族的并，并且$\mathscr{L}(E; F)$中存在可数集合，对于E的预紧子集一致收敛的拓扑来说是稠密的。

设 B 为 F 的单位球，$(V_n)$ E 中 0 的邻域的可数基本系统。对于每个整数 n，所有 $u \in \mathscr{L}(E; F)$ 的集合 $H_n$，使得 $u(V_n) \subset B$ 等连续且$\mathscr{L}(E; F)$ 是$H_n$ 的并。然后从命题得出推论。 6.*

#### 推论 2 {#evt-iii-s3-prop-6-cor-2 .statement tag=07N2}

— *第一个可数公理赋范空间满足的对偶E'中的每个闭球，对于弱拓扑σ(E', E)来说都是一个紧凑可度量空间，并且对于这个拓扑，在E'*中存在一个可数稠密子集。

这是从道具得出的。 6 以及从 III、p. 17 开始，cor。 3.

### 5. $E'$ 等连续子集

在这个截面中，E表示局部凸的空间，$E'$是它的对偶。每当我们谈论 E 中集合 M 的极坐标 $M^\circ$（或 $E'$）时，我们总是指的是，除非，否则，M 的极坐标相对于 E 和 $E'$ 之间的对偶性。回想一下，如果V是E中0的闭凸平衡邻域，我们有$V^{\circ\circ} = V$（II，p. 45，cor.3）。

#### 命题 7 {#evt-iii-s3-prop-7 .statement tag=07N3}

— *令 M 为子集 / $E'$。以下条件是等效的：*

(i) $M$ *等连续* ;
(ii) $M$ *包含在 E* 中 0 的邻域极坐标中；
(iii) *M 的极坐标是 E* 中 0 的邻域。

如果 M 是等连续的，则存在 0 的凸平衡邻域 V，使得对于所有 $x \in V$ 和所有 $u \in M$ 都有 $|u(x)| \leq 1$；那么我们就有了 $M \subset V^\circ$ 并且 (i) 蕴涵 (ii)。对于相同的记号，如果$M \subset V^\circ$则$V \subset V^{\circ\circ} \subset M^\circ$并且(ii)意味着(iii)。最后，如果$M^\circ$包含凸平衡邻域V为0，则$M \subset M^{\circ\circ} \subset V^\circ$和关系$x \in \varepsilon V,\ u \in M$对于所有$\varepsilon > 0$意味着$|u(x)| \leq \varepsilon$，这证明(iii)蕴涵(i)。

我们注从$E'$到K的每个$x \in E$定义映射$j(x): u \mapsto u(x)$到K。因此我们可以讨论E上的$\mathscr{S}$拓扑，其中$\mathscr{S}$是$E'$的子集的族：这是$K^{E'}$ 上$\mathscr{S}$ 拓扑的$j$ 下的逆像。我们立即验证，如果 $\mathscr{S}$ 是 $E'$ 上的凸出生学，那么对于 E 上的 $\mathscr{S}$ 拓扑，$\mathscr{S}$ 形式集合的极坐标是 0 的邻域的基本系统。 尤其是当$\mathscr{S}$是$E'$与螺旋等连续的子集族。 7 意味着：

#### 推论 1 {#evt-iii-s3-prop-7-cor-1 .statement tag=07N4}

— E 的 *拓扑与 $E'$* 的等连续子集一致收敛的拓扑相同。

更一般地，令 F 为局部凸空间；每$u \in \mathscr{L}(E; F)$定义映射$j(u):(x, f) \mapsto f(u(x))$从$E \times F'$进入K（*即*进入$\mathbf{R}$或$\mathbf{C}$）。这使得我们能够在定义、空间、$\mathscr{L}(E; F)$、拓扑、集合、子集、$E \times F'$上均匀收敛。尤其 ：

#### 推论 2 {#evt-iii-s3-prop-7-cor-2 .statement tag=07N5}

— *令$\mathscr{S}$为E的有界子集族。$\mathscr{L}(E; F)$上的$\mathscr{S}$拓扑是拓扑一致收敛于形式$A \times B \subset E \times F'$的集合，其中A在$\mathscr{S}$中，B属于在族中$F'$* 等连续子集。

对于F中每一个$u \in \mathscr{L}(E; F)$、每一个$A \in \mathscr{S}$以及每一个0的闭凸平衡邻域V，关系$u(A) \subset V$等价于“$j(u)(A \times V^\circ)$包含在K的单位球中”。

#### 命题 8 {#evt-iii-s3-prop-8 .statement tag=07N6}

— *设 H 是从 E 到局部凸空间 F 的线性映射族。要使 H 等连续，对于 F 的对偶 F' 中的每个等连续子集 X，线性形式 f \circ u 的集合，对于 f \in X 和 u \in H，是必要且充分的等连续。

显然条件是必要的。假设已验证，令V为F中0的闭凸平衡邻域。由于V^\circ等连续，因此E中存在0的邻域W使得|f(u(x))|对于所有 x \in W、u \in H 和 f \in V^\circ，\leq 1；在其他字中，对于所有 u \in H，u(W) \子集 V^{\circ\circ} = V，因而 H 是等连续的。

### 6. 局部凸空间的完成

#### 定理 1（格罗腾迪克）{#evt-iii-s3-thm-1 .statement tag=07N7}

— 令 E 为局部凸空间，令 \mathscr{S} 为 E 上的适应和覆盖出生学。令 F \子集 E^* 为 E 上那些线性形式的空间，其限制到每个集合属于到 \mathscr{S} 是连续的。如果 F 被分配为 \mathscr{S} 拓扑，则典范嵌入从 E'_\mathscr{S} 到 F 扩展到同构从 E'_\mathscr{S} 的补全 \hat{E}'_\mathscr{S} 到 F。

由于 E 上线性形式的每个简单极限都是线性形式（III，p. 16，道具 4），并且由于 E 上的出生学 \mathscr{S} 正在覆盖，因此它可以从 GT，X, § 1, No. 6，cor 得出。 2 具有 \mathscr{S} 拓扑的空间 F 是 Hausdorff 且完备的。显然 E'_\mathscr{S} 是 F 的拓扑向量子空间；因而，只要证明 E'_\mathscr{S} 在 F 中处处稠密即可。这由以下引理推出：

#### 引理 1 {#evt-iii-s3-lem-1 .statement tag=07N8}

设 A 为 E 的闭凸平衡子集，令 u 为 E 上的线性形式，其限制到 A 是连续的。那么对于每个 \varepsilon > 0，存在一个 x' \in E' 使得

$$ |u(x) - \langle x, x' \rangle| \leq \varepsilon \quad \text{for every} \quad x \in A . $$

设 \varepsilon > 0。E 中存在一个闭凸平衡邻域 U 为 0，使得 |u(x)| \leq \varepsilon 对于所有 x \in U \cap A。我们知道 E* 中 U 的极坐标 U^\circ 包含在 E' 中，并且对于拓扑 \sigma(E^*, E) (III, p. 17, cor. 2) 是紧致的。由于 E* 中 A 的极坐标 A^\circ 对 \sigma(E^*, E) 是封闭的，因而 A^\circ + U^\circ 是 E* 的封闭凸子集 (GT, III, § 4, No. 1, cor. 1)。

令 C 为 E 的闭凸平衡子集。则 C 对于 \sigma(E, E') (II, p. 45, cor. 3) 是封闭的，因此对于 \sigma(E, E^*) 也是如此，并且作为推论，我们有 C = C^{\circ\circ}（E 和 E* 之间的对偶性）。结果，我们有

$$ A \cap U = A^{\circ\circ} \cap U^{\circ\circ} = (A^\circ \cup U^\circ)^\circ \supset (A^\circ + U^\circ)^\circ $$

由此，我们得到

$$ (A \cap U)^\circ \subset (A^\circ + U^\circ)^{\circ\circ} = A^\circ + U^\circ . $$

从线性形式 \varepsilon^{-1}u 属于到 (A \cap U)^\circ，存在 v \in A^\circ 和 w \in U^\circ 使得 u = \varepsilon(v + w)。因而 x' = \varepsilon w 属于到 E' 且 u - x' = \varepsilon v 在绝对值中以 A 上的 \varepsilon 为界；因此引理。

现在设 E 为局部凸 Hausdorff 空间且 \hat{E} 它的完成。 E 扩展上的每个连续线性形式 f 到 \hat{E} 通过连续性；因此我们有 (\hat{E})' = E'

(III, p. 16) 以及 $E'$ $\hat{E}$ 定义线性形式的每元素；即 $E'$ 的代数对偶 ${E'}^*$ 的元素。在加法中，$E$（分别为$\hat{E}$）和$E'$之间的对偶性正在分离（II，p. 24，对应1）。因而$E$和$\hat{E}$可以用${E'}^*$的向量子空间来识别。

#### 定理 2 {#evt-iii-s3-thm-2 .statement tag=07N9}

*设 $E$ 为局部凸 Hausdorff 空间且 $\hat{E}$ 为它的完备集；我们认同$E$和$\hat{E}$以及向量子空间和${E'}^*$。那么对于元素$f \in {E'}^*$到属于到$\hat{E}$，$f$的限制到$E'$的每个等连续子集对于拓扑$\sigma(E', E)$是连续的。*

当$E'$被赋值为拓扑$\sigma(E', E)$时，空间$E$可以等同于$E'$的拓扑对偶（II，p. 43，第3条）；另一方面，如果$\mathscr{S}$是$E'$的等连续子集的集合，则$E$上给定的拓扑是$\mathscr{S}$拓扑（III，p. 19，cor.1）。然后从III，p. 13，道具得出。 1，$\mathscr{S}$的集合以$\sigma(E', E)$为界（*cf.*稍后，III，p. 22，道具9）；在其他字中，$\mathscr{S}$是对拓扑$\sigma(E', E)$的改编和涵盖的出生学。 定理 2 则为 th 的推论。 1 如果我们替换 $E$ 乘以 $E'$ 并且 $E'_\mathscr{S}$ 乘以 $E$。

#### 推论 1（巴纳赫）{#evt-iii-s3-thm-2-cor-1 .statement tag=07NA}

— *令 $E$ 为 Hausdorff 且完全局部凸空间。在阶中，$E'$上的线性形式对于弱拓扑$\sigma(E', E)$是连续的（即从$E$的元素产生），其限制对于每个等连续的子集就足够了$E'$ 对于 $\sigma(E', E)$ 是连续的。*

#### 注 {#evt-iii-s3-n6-rem-1 .statement tag=07NB}

— 假设在加法中，$E$中存在可数总数集合；那么 $E'$ 的每个等连续子集都可度量为拓扑 $\sigma(E', E)$（III，p. 18，道具 6）；因此，要验证$E'$上的线性形式$u$是弱连续的，只需验证$E'$中每个*等连续的序列*$(x'_n)$（对于$\sigma(E', E)$收敛到0），我们就有$\lim_{n \to \infty} u(x'_n) = 0$。

#### 推论 2 {#evt-iii-s3-thm-2-cor-2 .statement tag=07NC}

*令$(E_i)_{i \in I}$为Hausdorff局部凸空间族，并令$E$为其拓扑直和。那么从$\hat{E}_i$的直和到$\hat{E}$的典范映射就是同构。特别是，当且仅当所有 $E_i$ 都完整时，$E$ 才完整。*

我们知道$E$的对偶可以与$E_i$的对偶的乘积识别（II，p. 30，公式（1））。设$u \in \hat{E}$，并令$u_i \in {E_i'}^*$为$u$的限制（视为${E'}^*$的元素）到$E_i' \subset E'$。除了指标$i \in I$的有限数之外，直接的足以证明$u_i = 0$。相反，假设存在不同的指标使得$u_{i_n} \neq 0$存在序列$(i_n)_{n \in \mathbf{N}}$。那么存在$x_{i_n} \in E_{i_n}'$使得$u_{i_n}(x_{i_n}) = n$。所有$x_{i_n}$中的集合$H$在$E'$中等连续，并且$u$到$H$中的限制无界，这是不可能的。

### 7. $\mathscr{S}$-$\mathscr{L}(E; F)$上的出生学

令$E$和$F$是两个局部凸空间和$\mathscr{S}$，$E$的有界子集族。说$\mathscr{L}(E; F)$的子集$H$对于$\mathscr{S}$拓扑有界意味着*对于*每个$M \in \mathscr{S}$，F中0的每个邻域$V$吸收集合$H(M) = \bigcup_{u \in H} u(M)$；这与说相同，对于每个$M \in \mathscr{S}$，集合$H(M)$都以F为界。同样，这意味着对于F中0的每个邻域$V$，集合$\bigcap_{u \in H} u^{-1}(V)$吸收每个子集 $M$ 共 $\mathscr{S}$。

#### 命题 9 {#evt-iii-s3-prop-9 .statement tag=07ND}

*设E和F是两个局部凸空间和$\mathscr{S}$，E的有界子集族。那么$\mathscr{L}(E; F)$的每个等连续子集对于$\mathscr{S}$拓扑都是有界的。*

因为，如果 F 中 $H$ 是 $\mathscr{L}(E; F)$ 的等连续子集和 0 的 $V$ 邻域，则集合 $\bigcap_{u \in H} u^{-1}(V)$ 是 E 中 0 的邻域，因此吸收 E 的每个有界子集。

以 $\mathscr{S}$ 拓扑为界的 $\mathscr{L}(E; F)$ 的子集不一定是等连续的，即使 $\mathscr{S}$ 是覆盖的并且 $\mathscr{S}$ 是 E 上的规范出生学（IV，p. 50，练习 17）。在下面的段落中，我们将在 *barrelled* 空间、空间 E 的名称下研究，使得 $\mathscr{L}(E; F)$ 的每个简单有界子集都是等连续的。对于当前注，结果如下：

#### 命题 10 {#evt-iii-s3-prop-10 .statement tag=07NE}

*设 E 为出生学空间（特别是可度量的局部凸空间），F 为局部凸空间。以有界收敛的拓扑为界的$\mathscr{L}(E; F)$的每个子集 H 是等连续的。*

对于 F 中 0 的每个凸平衡邻域 $V$，集合 $\bigcap_{u \in H} u^{-1}(V)$ 吸收 E 的每个有界子集，因此 E 中 0 的邻域；这就证明H是等连续的。

### 8. 完成子集 / $\mathscr{L}_{\mathscr{S}}(E; F)$

#### 命题 11 {#evt-iii-s3-prop-11 .statement tag=07NF}

*设E和F是两个局部凸空间，$\mathscr{S}$有界子集的E由……组成的覆盖。如果 F 是 Hausdorff 且准完备 (III, p. 8)，则$\mathscr{L}(E; F)$ 的每个等连续子集 H（对于 $\mathscr{S}$ 拓扑是闭集）是 $\mathscr{L}_{\mathscr{S}}(E; F)$ 的完全一致子空间。*

由于对于 $\mathscr{S}$ 拓扑，H 的边界为 $\mathscr{L}_{\mathscr{S}}(E; F)$（III，p. 22，命题 9），并且在 $F^E$ 中封闭（III，p. 16，命题 4），因此可以从以下结论得出： GT 3，X, § 1, No. 5。

#### 注 1 {#evt-iii-s3-n8-rem-1 .statement tag=07NG}

— 令 M 为 $\mathscr{L}_{\mathscr{S}}(E; F)$ 的*完整*一致子空间。对于E的有界子集$\mathscr{S}' \supset \mathscr{S}$的每个集合，$\mathscr{S}'$拓扑比$\mathscr{L}(E; F)$上的$\mathscr{S}$拓扑更细；另一方面，对于$\mathscr{S}'$拓扑，存在系统为0的邻域，对于简单收敛的拓扑是封闭的（III，p. 13，*注2*），并且对于更不必说* $\mathscr{S}$-拓扑。我们结论（GT，III, § 3, No. 5，cor.1）M对于$\mathscr{S}'$拓扑来说是*完整的。

#### 推论{#evt-iii-s3-n8-cor-1 .statement tag=07NH}

*令 E 和 F 为两个局部凸空间，H 为 $\mathscr{L}(E; F)$ 的等连续子集。如果 F 是 Hausdorff 且准完备，并且 H 上的滤波器 $\Phi$ 简单地收敛于 E 的总子集 T 的点，则存在从 E 到 F 的连续线性映射 u，使得 $\Phi$ 在 E 的每个预紧子集上均匀收敛到 u。

因为，凭借道具。 5 (III, p. 17) $\Phi$ 是 E 中预紧收敛一致结构的柯西滤波器；通过道具。如图11所示，H在$\mathscr{L}_{pc}(E; F)$中的闭包$\overline{H}$是完全的，因此$\Phi$一致收敛于E到映射$u \in \overline{H}$的每个预紧子集。

#### 注 2 {#evt-iii-s3-n8-rem-2 .statement tag=07NI}

令 $(u_n)$ 为从 Banach 空间 E 到 Banach 空间 F 的连续线性映射的序列；可能会发生，$(u_n(x))$ 在 E 的处处密集向量子空间 T 的每个点处都有极限，而序列 $(u_n)$ 不受范数空间 $\mathscr{L}(E; F)$ 的限制。对于例，取E为$\mathbf{R}$上所有连续数值函数的空间，在无穷大处趋向于零，且范数$\|f\| = \sup_{x \in \mathbf{R}} |f(x)|$，令T为具有紧支撑的连续数值函数的子空间。对于所有$f \in T$，从E到$\mathbf{R}$的连续线性映射$f \mapsto nf(n)$的序列收敛于0，但不受$\mathscr{L}_b(E; \mathbf{R})$的限制。同样例表明，在空间$\mathscr{L}(T; \mathbf{R})$中，序列$(v_n)$对于有界收敛的拓扑可能是简单收敛且无界的。

另一方面，连续线性映射$f \mapsto \sum_{k=1}^n f(k)$的序列对于简单收敛的拓扑来说是$\mathscr{L}(T; \mathbf{R})$中的柯西序列，但对于这个拓扑并不倾向于$\mathscr{L}(T; \mathbf{R})$中的极限。

#### 命题 12 {#evt-iii-s3-prop-12 .statement tag=07NJ}

— *令 E 为出生学局部凸空间，F 为完全局部凸 Hausdorff 空间和 $\mathfrak{S}$ 一个由 E 包含像组成的有界子集族，其中每个序列收敛于 0。然后空间 $\mathscr{L}_{\mathfrak{S}}(E; F)$ 已完成。*

令 $\Phi$ 为 $\mathscr{L}_{\mathfrak{S}}(E; F)$ 中的柯西滤波器。那么$\Phi$是拓扑的简单收敛的柯西滤波器，因此收敛于$F^E$；此外，它的极限$u$是从E到F的线性映射，并且$\Phi$在$\mathfrak{S}$的每个集合均匀地收敛到$u$（GT，X, § 1, No. 5，道具5）。由此可见，序列收敛到零的$u$下的像是序列收敛到零，因此，$u$是*连续的*，因为E是天生的（III，p. 11，道具1， (三))。

#### 推论 1 {#evt-iii-s3-prop-12-cor-1 .statement tag=07NK}

— *出生学空间的强对偶已完成。*

#### 推论 2 {#evt-iii-s3-prop-12-cor-2 .statement tag=07NL}

— *令 E 为半范数空间，F 为 Banach（分别为 Fréchet）空间。 空间 $\mathscr{L}_b(E; F)$ 是 Banach（或 Fréchet）空间。特别是，半范数空间的对偶是 Banach 空间。*

### 习题{#evt-iii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
