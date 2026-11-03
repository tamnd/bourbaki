---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 1
section_title: Topologies on groups
lang: zh
source: top-i-iv
book_pages: 219-225, 296-298
pdf_pages: 0225-0231, 0302-0304
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGICAL GROUPS
      page: 219
      pdf_page: 225
    - "no": 2
      title: NEIGHBOURHOODS OF A POINT IN A TOPOLOGICAL GROUP
      page: 221
      pdf_page: 227
    - "no": 3
      title: ISOMORPHISMS AND LOCAL ISOMORPHISMS
      page: 224
      pdf_page: 230
statements: 11
exercises: 9
content_sha256: fb3e6f943539f479636ff4a6a45d7081359969f9993dac0df54a0e52ac3b732b
translated_from: content/en/top/III/01_s1_topologies_on_groups.md
translation_method: google
source_content_sha256: f983e9d3b98ec2684f1a28bb47c3f0112d4c5196bbdba56270d17585e82bcb5b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: af645d61ae44436e48fc6b9beb4800774bc190d3c6cd5cdeef00e2a7b19f3c81
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 1. 群上的拓扑

### 1. 拓扑群

群的章、律、合成的前四个截面一般写成乘法，e表示单位元素；将结果翻译成加法记号（我们记得，这是专门为交换群保留的）通常留给读者。

#### 定义 1 {#top-iii-s1-def-1 .statement tag=0BH8}

拓扑群是集合G，它带有群结构和拓扑并且满足以下两个公理：

（GT_I）。 $G \times G$到$G$的映射$(x, y) \to xy$是连续的。

（GT_{II}）。 $G$到$G$的映射$x \to x^{-1}$（群G的对称性）是连续的。

如果集合 G 上的群结构和拓扑满足 (GT_I) 和 (GT_{II})，则称它们是兼容的。

#### 例 1 {#top-iii-s1-n1-exa-1 .statement tag=0BH9}

群 G 上的离散拓扑与群结构兼容。 拓扑是离散的拓扑群称为离散群。

同样，G 上最粗糙的拓扑 (章 I, § 2, no. 2) 与 G 的群结构兼容。

#### 例 2 {#top-iii-s1-n1-exa-2 .statement tag=0BHA}

\* 在章IV中，我们将看到有理线Q（或实直线R）的拓扑与Q（或R）的加法群结构兼容。

#### 例 3 {#top-iii-s1-n1-exa-3 .statement tag=0BHB}

如果G是拓扑群，则其拓扑与群$G^0$的结构兼容，与G相反； $G^0$，加上拓扑，据说是与 G 相反的拓扑群。

公理 $(\mathrm{GT}_\mathrm{I})$ 和 $(\mathrm{GT}_\mathrm{II})$ 等价于以下内容：

（GT'）。 *映射* $(x, y) \to xy^{-1}$ *从* $G \times G$ *进入* $G$ *是连续的*。

显然$(\mathrm{GT}_\mathrm{I})$和$(\mathrm{GT}_\mathrm{II})$一起意味着（GT'）。相反，(GT') 意味着$(\mathrm{GT}_\mathrm{II})$，因为$x \to ex^{-1} = x^{-1}$ 是连续的； (GT') 和$(\mathrm{GT}_\mathrm{II})$一起意味着$(\mathrm{GT}_\mathrm{I})$，因为$(x, y) \to x(y^{-1})^{-1} = xy$是连续的。

如果$a$是$G$的任何元素，则*左平移*$x \to ax$（分别是*右平移*$x \to xa$）是连续的，通过$(\mathrm{GT}_\mathrm{I})$，因此是$G$到$G$的*同胚*。 映射$x \to axb$，因为$a$和$b$贯穿$G$，因此形式是$G$的同胚*群； 映射 $x \to axa^{-1}$（分别为$x \to ax, x \to xa$），其中$a$贯穿同胚的群的$G$、形式子群。同样，由于对称性$x \to x^{-1}$是$G$的对合置换，公理$(\mathrm{GT}_\mathrm{II})$表明这个映射是$G$到$G$的*同胚*。

如果$A$是$G$的开（或闭）子集，并且如果$x$是$G$的任何点，则集合、$x.A, A.x$和$A^{-1} (*)$是开（或闭），因为它们是变换 $A$ 在前述同胚之一下。如果$A$是*开*并且$B$是$G$中的任何子集，那么$AB$和$BA$是*开*，因为它们是开集合的并[公理$(\mathrm{O}_\mathrm{I})$]。如果$G$中$V$是$e$的邻域，则$VA$和$AV$是$A$的*邻域*；因为如果$W$是包含在$V$中的$e$的开邻域，则$WA$和$AW$是开的并且包含$A$。

另一方面，当$A$闭合时，$AB$不需要闭合，即使$B$也闭合（cf.§ 4, no. 1、推论1到命题1）。

\* 例如，在实直线$\mathbf{R}$的加法群中，有理数整数的子群$\mathbf{Z}$是闭集，所有整数的子群$\theta \mathbf{Z}$由……组成也是闭集*非理性* 倍数 $n\theta$ 数 $\theta$；但是$\mathbf{R}$的子群$\mathbf{Z} + \theta \mathbf{Z}$，即所有实数$m + n\theta$中的集合（其中$m$和$n$占所有整数值）在$\mathbf{R}$中并未关闭，正如我们将在章V, § 1。

再次，令$A$为$\mathbf{R} \times \mathbf{R}$的加法群的子集，其中包含所有$(x, y)$对，使得$x \geqslant 0$和$0 \leqslant y \leqslant 1 - \frac{1}{x+1}$；并令$B$为所有对$(x, 0)$中的集合，因为$x$贯穿$\mathbf{R}$。 $A$和$B$是封闭的，但是$A + B$是所有对$(x, y)$中的集合，使得$0 \leqslant y < 1$，并且在$\mathbf{R} \times \mathbf{R}$中不封闭。 \*

令$X$为拓扑空间，并令$f$和$g$为$X$的两个映射，形成拓扑群$G$。如果 $f$ 和 $g$ 在点 $x_0$ 连续

(*) 我们记得，如果$A$和$B$是群$G$中的两个子集，则$A.B$或$AB$表示所有乘积$xy$中的集合，其中$x \in A$和$y \in B$； $A^{-1}$ 表示所有元素 $x^{-1}$ 中的集合，其中 $x \in A$。如果$B$由单个元素$x$组成，我们写$x.A$或$xA$（分别为$A.x$或$Ax$）来代替$\{ x \}.A$（分别为$A.\{ x \}$）。

X，则$f^{-1}$和$fg$(*)，乘以章I, § 2, no. 1的定理 2。特别是，X的连续映射进入G，X的所有映射进入G的群$G^X$的形式子群。

再次，让$f$和$g$是集合X的两个映射，通过过滤器$\mathfrak{F}$过滤，成为豪斯多夫拓扑群G。如果$\lim_{\mathfrak{F}} f$和$\lim_{\mathfrak{F}} g$存在，那么也存在$\lim_{\mathfrak{F}} f^{-1}$ 和 $\lim_{\mathfrak{F}} fg$，我们有 (章 I, § 7, no. 4、命题 9、推论 1)

(1) $$
\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1},
$$
(2) $$
\lim_{\mathfrak{F}} fg = (\lim_{\mathfrak{F}} f) (\lim_{\mathfrak{F}} g).
$$

当 G 是可交换的群（加法书写）时，公理 (GT') 表明 $(x, y) \to x - y$ 是连续的映射。如果$f$和$g$是G中拓扑空间X的映射，在点$x_0$连续，则$f - g$在点连续。 公式 (1) 和 (2) 可以类似地转录。

### 2. 拓扑群中点的邻域

令$\mathfrak{B}$为拓扑群G中单位元素$e$的邻域滤波器，并令$a$为G的任意点。由于$x \to ax$和$x \to xa$是同胚，因此$a$的邻域过滤器是集合$a.V$的$a.\mathfrak{B}$族，其中V贯穿$\mathfrak{B}$，也是集合$V.a$的$\mathfrak{B}.a$族。因此，只要我们知道群的单位元素$e$的邻域过滤器，我们就知道拓扑群的任何点的邻域过滤器。

如果我们说$xy$和$x^{-1}$在$x = y = e$连续，我们得到(章I, § 2, no. 1)：

(GV_I)。 *给定任何*$U \in \mathfrak{B}$，*存在*$V \in \mathfrak{B}$*使得*$V.V \subset U$。

（GV_{II}）。 *给定任何*$U \in \mathfrak{B}$，*我们有*$\overline{U} \in \mathfrak{B}$。

G 上满足 (GV_I) 和 (GV_{II}) 的每个滤波器 $\mathfrak{B}$ 也满足 (GV_a)。 *给定任何*$U \in \mathfrak{B}$，*存在*$V \in \mathfrak{B}$*使得*$V.V^{-1} \subset U$。对于(GV_I)，存在$W \in \mathfrak{B}$使得$W.W \subset U$，并且通过(GV_{II})存在$V \in \mathfrak{B}$使得$V \subset W \cap W^{-1}$；因此$V^{-1} \subset W$，因此$V.V^{-1} \subset W.W \subset U$。

相反，如果 G 上的过滤器 $\mathfrak{B}$ 满足 (GV_a)，则它首先遵循 $e$ 属于到每个集合 $U \in \mathfrak{B}$；因为如果 $V \in \mathfrak{B}$ 使得 $V.V^{-1} \subset U$，

(*) 我们记得$f^{-1}$是映射$x \to (f(x))^{-1}$和$fg$映射$x \to f(x)g(x)$；它们不应与 $f^{-1}$ 和 $f \circ g$（定义时）混淆（*集合理论*，R，§ 2，第 6 和 11 号）。

那么，由于 $V$ 不为空，因此每个 $x \in V$ 都有 $x.x^{-1} = e \in U$。因此，条件$(GV_a)$意味着$V^{-1} \subset V.V^{-1} \subset U$，因此每当$U \in \mathfrak{B}$时，$U^{-1} \in \mathfrak{B}$。最后，如果 $V \in \mathfrak{B}$ 满足 $V.V^{-1} \subset U$，且 $W \in \mathfrak{B}$ 满足 $W \subset V \cap V^{-1}$，则我们有 $W.W \subset U$。因此，我们看到$(GV_a)$*等于*$(GV_1)$和$(GV_{II})$的合取。

最后，由于 $x \to axa^{-1}$ 是同胚，使得 $e$ 固定，因此 $\mathfrak{B}$ 有以下性质：

$(GV_{III}).$ *对于所有* $a \in G$ *和所有* $V \in \mathfrak{B}$，*我们有* $a.Va^{-1} \in \mathfrak{B}$。

过滤器$\mathfrak{B}$的这三个属性是*特征*：

#### 命题 1 {#top-iii-s1-prop-1 .statement tag=0BHC}

*让* $G$ *成为群，让* $\mathfrak{B}$ *成为* $G$ *满足公理* $(GV_1)$、$(GV_{II})$ *和* $(GV_{III})$的过滤器。 *然后在* $G$上有一个独特的拓扑，*与* $G$的群结构兼容，*其中* $\mathfrak{B}$ *是单位元素* $e$的邻域过滤器。 *对于任何点* $a \in G$ 的此拓扑邻域过滤器 *与两个过滤器中的每个过滤器相同* $a.\mathfrak{B}$ *和* $\mathfrak{B}.a$。

如果存在具有所需属性的拓扑，则通过上面所说的邻域过滤器$a$重合以及每个过滤器$a.\mathfrak{B}$和$\mathfrak{B}.a$；因此拓扑是唯一的（如果存在的话）。如果我们证明 1) 过滤器$a.\mathfrak{B}$ 是$G$ 上拓扑的邻域过滤器，以及 2) 这个拓扑与$G$ 的群结构兼容，则它的存在成立。

1) 正如我们已经看到的，由于$(GV_1)$和$(GV_{II})$，滤波器$a.\mathfrak{B}$满足公理$(V_{III})$（参见章I § 1, no. 2）；因此，为了证明$a.\mathfrak{B}$是$G$上拓扑中$a$的邻域过滤器，我们必须验证公理$(V_{IV})$。令$V$为$\mathfrak{B}$的任意集合，以及$\mathfrak{B}$的$W$集合，使得$W.W \subset V$；那么对于任何$x \in a.W$，我们有$x.W \subset a.W.W \subset a.V$，因此$a.V$属于到过滤器$x.\mathfrak{B}$；因此$(V_{IV})$是满足的。

2) 现在让我们证明由邻域过滤器$a.\mathfrak{B}$定义的拓扑满足$(GT')$。令$a, b$为$G$中的任意两个点；如果我们放入$x = au$和$y = bv$，那么只要$u$和$v$足够接近$e$，我们就必须证明$xy^{-1}$尽可能接近$ab^{-1}$。现在$(ab^{-1})^{-1}(xy^{-1}) = buv^{-1}b^{-1}$；令$U$是$e$中的任意邻域，那么如果$uv^{-1} \in b^{-1}Ub = V$我们将有$buv^{-1}b^{-1} \in U$，并且由于$(GV_{III})$我们将有$V \in \mathfrak{B}$。但通过$(GV_1)$和$(GV_{II})$，存在$W \in \mathfrak{B}$使得$W.W^{-1} \subset V$；因此，在阶中取$u \in W$和$v \in W$就足以得到$xy^{-1} \in (ab^{-1})U$。这样就完成了证明。

定义与$G$上的群结构兼容的拓扑的常用方法包括给出满足公理$(GV_1)$、$(GV_{II})$和$(GV_{III})$的过滤器。 *过滤器基* $\mathfrak{B}$ 的相应的条件如下：

$(GV'_1).$ *给定任何* $U \in \mathfrak{B}$，*存在* $V \in \mathfrak{B}$ *使得* $V.V \subset U$。

（GV_{II}）。 *给定任何*$U \in \mathfrak{B}$，*存在*$V \in \mathfrak{B}$*使得*$V^{-1} \subset U$。

（GV'_{III}）。 *给定任何* $a \in G$ *和任何* $U \in \mathfrak{B}$，*存在* $V \in \mathfrak{B}$ *这样* $V \subset a . U . a^{-1}$。

$e$的邻域，其中重合及其像在对称性$x \to x^{-1}$下被称为*对称*。如果$V$是$e$中的任意邻域，则$V \cup V^{-1}$、$V \cap V^{-1}$和$V . V^{-1}$是对称的邻域。通过(GV_{II})，$e$的对称邻域形式a *基本系统的邻域*。另外，根据 (GV_{I})，当$V$穿过$e$的邻域的基本系统时，集合$V^n$（其中$n$是固定的整数$\neq 0$） 形式邻域 $e$ 的基本系统。

#### 注 {#top-iii-s1-n2-rem-1 .statement tag=0BHD}

如果$G$是*可交换的*，对于$G$的每个子集$A$和每个$x \in G$，我们都有$x . A . x^{-1} = A$，因此（GV_{III}）[resp。 (GV'_{III})] 自动满足$G$上的每个过滤器（分别是过滤器基）。另一方面，如果 $G$ 不是阿贝尔的，则 (GV_{III}) 不是 (GV_{I}) 和 (GV_{II}) 的推论 [参见习题 5]。

如果$G$是可交换的群，写为*加法*，公理表征了拓扑的原点邻域的过滤器$\mathfrak{B}$与$G$的群结构兼容，因此如下：

（GA_{I}）。 *给定任何*$U \in \mathfrak{B}$，*存在*$V \in \mathfrak{B}$*使得*$V + V \subset U$。

（GA_{II}）。 *给定任何*$U \in \mathfrak{B}$，*我们有*$-U \in \mathfrak{B}$。

#### 命题 2 {#top-iii-s1-prop-2 .statement tag=0BHE}

*拓扑群* $G$ *是 Hausdorff 当且仅当集合* $\{e\}$ *闭合*。

显然，如果 $G$ 是 Hausdorff，则 $\{e\}$ 是闭集。反之，如果$\{e\}$是闭的，那么$G \times G$的对角线$\Delta$也是闭的，因为它是连续映射$(x, y) \to xy^{-1}$下的$\{e\}$的逆像；因此 (章 I, § 8, no. 1, 命题 1) $G$ 是豪斯多夫。

#### 推论 {#top-iii-s1-n2-cor-1 .statement tag=0BHF}

*拓扑群* $G$ *是 Hausdorff 当且仅当* $e$ 的邻域交 *仅由点* $e$ 组成。

条件显然是必要的。相反，如果 $e$ 的所有邻域中的交只是 $\{e\}$，则给定任意 $x \neq e$，$e$ 中存在邻域 $V$，使得 $x^{-1} \notin V$ 进而$e \notin xV$。这说明$x$不在$\{e\}$的闭包内，因而$\{e\}$是闭包，所以$G$是Hausdorff。

#### 例 {#top-iii-s1-n2-exa-1 .statement tag=0BHG}

*通过一组子群定义群上的拓扑。* 如果$\mathfrak{B}$是群$G$上的*过滤基*，由$G$的*子群*组成，那么可以立即看出$\mathfrak{B}$满足公理 (GV_{I}) 和 (GV_{II})，因为$H . H^{-1} = H$ 对于$G$ 的任意子群$H$。 因此，集合$\mathfrak{B}$将是拓扑中$e$的邻域*的基本系统与$G$的群结构兼容，前提是$\mathfrak{B}$满足(GV_{III})；如果 $\mathfrak{B}$ 中的所有子群都是正规的，则尤其如此，因此如果 $G$ 是*可交换的*，则总是如此。 因此拓扑由命题2定义为*Hausdorff*，当且仅当$\mathfrak{B}$中所有子群的*交仅由*$e$组成。 最有趣的情况是子群 $\{ e \}$ *不在* $\mathfrak{B}$ 中（否则由 $\mathfrak{B}$ 定义的拓扑是*离散* 拓扑）：如果 $\{ e \} \notin \mathfrak{B}$，则仅当 $\mathfrak{B}$ 时，$\mathfrak{B}$ 定义的拓扑才是 Hausdorff是一个*无限*集合。

由于两个子群的交是子群，我们可以在$G$上定义拓扑，与其群结构兼容，从$G$的子群*任意*集合$\mathfrak{F}$开始：令$\mathfrak{G}$为所有子群$a.H.a^{-1}$的集合，其中$H \in \mathfrak{F}$和$a \in G$，并让$\mathfrak{B}$为子群属于的所有*有限*交的集合到$\mathfrak{G}$。那么$\mathfrak{B}$是一个过滤器基并且满足(GV$_{\text{III}}$)。

特别考虑 *环* $A$ 的加法群。 $A$定义拓扑的*理想*中的每个集合$\mathfrak{F}$都与此加法群结构兼容。如果$\mathfrak{F}$的所有理想中的交是零理想，则拓扑是Hausdorff；如果$\mathfrak{F}$的理想中没有有限的交是零理想，则该拓扑不是离散的。以这种方式定义的拓扑在数的理论中发挥大的部分（参见§§ 6的习题和章的7个）。

### 3. 同构和本地同构

根据一般的定义 (*集合理论*, 章 IV, § 1, no. 5) 拓扑群 $G$ *到* 拓扑群的 *同构* $f$ *群 $G'$是$G$到$G'$的双射映射，它同时是*$G$到$G'$的群结构的*同构，以及*$G$到$G'$的*同胚。在其他字中，$f$ 是 $G$ 的同构到 $G'$ 当且仅当： 1) $f$ 是双射； 2) $f(xy) = f(x)f(y)$ 对于所有$x, y \in G$； 3) $f$ 是双连续的。

例如，如果$a$是$G$的任意点，则映射$x \to axa^{-1}$是$G$到$G$的同构，即(*loc.cit.*)，拓扑群的*自同构* $G$。它被称为*内自同构*。

如果拓扑 $\mathscr{C}$ 与群 $G$ 的群结构兼容，则 $\mathscr{C}$ 也与群结构兼容，与 $G$ 的*相反*。如果$G^0$表示通过给予与$G$拓扑$\mathscr{C}$相反的群获得的拓扑群，则对称性$x \to x^{-1}$是拓扑群$G$在拓扑上的*同构* 群$G^0$。

#### 定义 2 {#top-iii-s1-def-2 .statement tag=0BHH}

*如果* $G$ *和* $G'$ *是两个拓扑群，* $G$ *的局部同构 *与* $G'$ *是同胚* $f$ *邻域* $V$ *单位元素 * $G$ *到邻域* $V'$ *of 单位元素 of* $G'$ *满足以下条件：*

1) *对于* $V$ *中的每个对* $x, y$ *点 *这样* $xy \in V$，
$$
f(xy) = f(x)f(y).
$$

2) 如果 g 是 f 的逆映射，那么对于 V' 的每对点 x', y' 使得 x'y' ∈ V'，我们有 g(x'y') = g(x') g(y')。
那么映射 g 就是 G' 与 G 的局部同构。
如果存在 G 与 G' 的局部同构，则称两个拓扑群 G、G' 是局部同构的。

同构拓扑群显然是局部同构的。 逆命题为假。

\* 例如，我们将在章V, § 1中看到，拓扑群R和T是局部同构的，但不是同构的。 \*

如果 f 是 G 与 G' 的局部同构，则 f 的每个限制到 G 的单位元素的邻域又是 G 与 G' 的局部同构。

G 与 G 的局部同构称为 G 的局部自同构。

一般来说，如果f是G的单位元素的邻域V到G'的单位元素的邻域V'的同胚，且满足定义2的条件1)，则f不一定是满足条件 2)（参见习题7）。然而，G 和 G' 实际上是局部同构的。

#### 命题 3 {#top-iii-s1-prop-3 .statement tag=0BHI}

设G和G'为两个拓扑群，设f为G的单位元素的邻域V到G'的单位元素的邻域V'的同态，满足定义2的条件1)，则f为G 与 G' 的局部同构的扩张。

因为不难看出，如果 W 是 G 的单位元素的邻域，使得 W.W ⊂ V，则 f 到 W 的限制是 G 与 G' 的局部同构。

### 习题{#top-iii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
