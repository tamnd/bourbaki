---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 11
section_title: Connectedness
lang: zh
source: top-i-iv
book_pages: 107-116, 155-161
pdf_pages: 0113-0122, 0161-0167
extraction: ocr
subsections:
    - "no": 1
      title: CONNECTED SPACES AND CONNECTED SETS
      page: 107
      pdf_page: 113
    - "no": 2
      title: IMAGE OF A CONNECTED SET UNDER A CONTINUOUS MAPPING
      page: 109
      pdf_page: 115
    - "no": 3
      title: QUOTIENT SPACES OF A CONNECTED SPACE
      page: 110
      pdf_page: 116
    - "no": 4
      title: PRODUCT OF CONNECTED SPACES
      page: 110
      pdf_page: 116
    - "no": 5
      title: COMPONENTS
      page: 110
      pdf_page: 116
    - "no": 6
      title: LOCALLY CONNECTED SPACES
      page: 112
      pdf_page: 118
    - "no": 7
      title: 'APPLICATION : THE POINCARÉ-VOLTERRA THEOREM'
      page: 114
      pdf_page: 120
statements: 29
exercises: 25
content_sha256: 58d96f933557885ba10f80a54cb8cb784b839a606b2fd219fe020ad8fe15d3d5
translated_from: content/en/top/I/11_s11_connectedness.md
translation_method: google
source_content_sha256: 602e72b63986cd10033d70d8a3dec1b9d5fcf55f8050a8e3d312d439a7a17d9f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 94628235c99687c88e5e00d8d12ae37b785987a5a3eff6104fbca259e6870592
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 11. 连通性

### 1. 连接空间和连接集合

#### 定义 1 {#top-i-s11-def-1 .statement tag=0BBG}

如果拓扑空间X不是两个不相交的非空开集合中的并，则称其是连通的。

通过替换字“打开集合”通过“关闭集合”获得等效的定义。 X连通当且仅当X中唯一开闭的子集是空集以及整个空间X。

如果 X 已连通，并且 A、B 是两个非空开（或闭）子集，使得 A \cup B = X，则 A \cap B \neq \emptyset。

#### 例 1 {#top-i-s11-n1-exa-1 .statement tag=0BBH}

我们将在章IV, § 2, no. 5中看到实直线是连通的，而有理线则不是。 \*

#### 例 2 {#top-i-s11-n1-exa-2 .statement tag=0BBI}

具有多个点的离散空间未连接。

观察如果$(U_i)_{i \in I}$是开集合的拓扑空间$X$由……组成的划分[必然非空，从划分的定义（集合理论，R，， no. 4)]则每个$U_i$在$X$中既开又闭，因为$U_i$的补集是$U_x$的并，其中$x \neq i$。 $X$的开子集为子集$A$，使得$A \cap U_i$对于每个$i \in I$在$U_i$中开开，这样$X$可以与$U_i$的和识别（$\S 2$， no. 4, 例 3) 并且如果$I$有多个元素则不连接

#### 定义 2 {#top-i-s11-def-2 .statement tag=0BBJ}

*如果 $X$ 的子空间 $A$ 是连通的，则拓扑空间 $X$ 的子集 $A$ 被称为连通的集合。*

为了使$A$成为$X$的连通子集，对于$A$的每个覆盖，$X$的两个开（或闭）子集$B, C$，使得$A \cap B$和$A \cap C$非空，我们有$A \cap B \cap C \neq \emptyset$。

#### 例 {#top-i-s11-n1-exa-3 .statement tag=0BBK}

在任何拓扑中空间、空集以及单个点的每个集合由……组成都是相连的。在 Hausdorff 空间 $X$ 中，超过 1 个点的每个有限集合由……组成均不相连，更一般地，$X$ 的每个子集具有多个点并且至少有一个孤立的点未连接。

如果密集的子集$A$相连，则整个空间$X$相连；否则，将存在$X$的两个非空开不相交的开子集$M, N$，使得$M \cup N = X$和$M \cap A, N \cap A$将是$A$的两个不相交的非空开子集，其并是 $A$。因此我们有

#### 命题 1 {#top-i-s11-prop-1 .statement tag=0BBL}

*如果$A$是一个连通的集合，那么每个集合$B$使得$A \subset B \subset \overline{A}$是连通的。*

#### 命题 2 {#top-i-s11-prop-2 .statement tag=0BBM}

* 集合的并交非空是相连的。*

令$(A_i)_{i \in I}$为$X$相连的子集族，所有包含与点$x$相同；我们必须证明

$$
A = \bigcup_i A_i
$$

已连接。如果不是，则存在两个开集合、$B$和$C$，使得$B \cap A$和$C \cap A$非空，以及$A \subset B \cup C$和$A \cap B \cap C = \emptyset$。 $x$ 属于到集合 $B, C$ 之一，比如 $x \in B$；另一方面，集合$A_i$中的一个，比如$A_x$，满足$C$；因此，$A_x \subset B \cup C$、$A_x \cap B \cap C = \emptyset$、$B \cap A_x$和$C \cap A_x$非空。因此$A_x$不连通，这是一个矛盾。

#### 推论{#top-i-s11-n1-cor-1 .statement tag=0BBN}

*让$(A_n)_{n \geq 0}$是连接的集合的无限序列，使得$A_{n+1} \cap A_n \neq \emptyset$对于所有$n \geq 0$。然后并$\bigcup_{n=0}^\infty A_n$已连接。*

通过$n$上的归纳，我们立即看到集合$B_n = \bigcup_{i=0}^n A_i$通过命题2连接到所有$n$。集合$B_n$有一个非空交；因此，它们的并等于 $\bigcup_{n=0}^\infty A_n$，由命题 2 连接。

#### 命题 3 {#top-i-s11-prop-3 .statement tag=0BBO}

*设$A$为拓扑空间$X$的子集。如果$B$是$X$的连通子集，并且满足$A$和$\complement A$，则$B$满足$A$的边界。*

否则，$B$的交与$A$的内部和外部将是$B$的两个开放的子集，其中$B$的形式、划分和$B$不会连接。

#### 推论 {#top-i-s11-n1-cor-2 .statement tag=0BBP}

*在连通的空间$X$中，除了$X$本身之外的每个非空集合都至少有一个边界点。*

### 2. 连续映射下连接的集合的像

#### 命题 4 {#top-i-s11-prop-4 .statement tag=0BBQ}

*令$A$为拓扑空间$X$的连通子集，并令$f$为$X$到拓扑空间$X'$的连续映射。然后$f(A)$已连接。*

假设 $f(A)$ 未连接。则存在两个$f^{-1}(A)$开路的集合$M', N'$，以及$f(A)$的形式划分；因此$A \cap f^{-1}(M')$和$A \cap f^{-1}(N')$在$A$的$A$和形式划分开放；这个与……矛盾假设与$A$相连。

连续映射下相连的集合的*逆像*不需要相连；考虑将离散的空间的例映射转换为一个点的空间由……组成。

从命题 4 我们推导出 *非连接空间* 的另一个刻画：

#### 命题 5 {#top-i-s11-prop-5 .statement tag=0BBR}

*要使拓扑空间 $X$ 不连通，存在 $X$ 的满射连续映射到离散空间包含多个点上是必要且充分的。*

条件满足命题 4。反之，如果$X$不连通，则存在两个非空不相交的开子集$A, B$，其并为$X$，且映射$f$ $X$到由$f(A) = \{a\}$和$f(B) = \{b\}$定义的两个元素$\{a, b\}$的离散空间是连续的。

### 3. 连接空间的商空间

#### 命题 6 {#top-i-s11-prop-6 .statement tag=0BBS}

连通的空间的每个商空间都是连通的。

这是直接的推论命题 4 no. 2。

#### 命题 7 {#top-i-s11-prop-7 .statement tag=0BBT}

令$X$为空间和$R$等价关系在$X$上。如果商空间 $X/R$ 相连，并且每个等价类 mod $R$ 相连，则 $X$ 相连。

假设 $X$ 未连接。然后还有$X$的划分分成两个开的集合$A, B$。 集合 $A, B$相对于$R$饱和；因为如果$x \in A$则$x$不能的等价类$M$满足$B$，否则集合$A \cap M, B \cap M$会将$M$的形式划分分成两部分集合在$M$打开，这是不可能的，因为$M$已连接。因此，$A$和$B$的典范像在$X/R$和形式划分开放集合和$X/R$；这个与……矛盾假设与$X/R$相连。

### 4. 乘积已连接空间

#### 命题 8 {#top-i-s11-prop-8 .statement tag=0BBU}

连接的空间中的每个乘积都是相连的。相反，如果非空空间中的乘积是连通的，则因子中的每一个都是连通的。

设$X = \prod_{i \in I} X_i$为拓扑空间的乘积。 如果$X_i$非空，则每个$i \in I$都有$X_i = \operatorname{pr}_i X$；因此，如果 $X$ 连接，则 $X_i$（no. 2，命题 4）也连接。 相反，假设每个 $X_i$ 已连接，而 $X$ 未连接。 通过no. 2的命题 5，存在连续的满射映射$f : X \to X'$，其中$X'$是离散的空间，其中包含多于一个点。 令$a = (a_i)$为$X$中的任意点，且$x$为任意指标；部分映射$f_x : X_x \to X'$，由$f_x(x) = f((y_i))$定义，其中$y_x = x$和$y_i = a_i$（如果$i \neq x$）在$X_x$上连续；由于$X_x$已连接，$f_x$在$X_x$上必须恒定。 It follows immediately by induction that $f(x) = f(a)$ for all points $x = (x_i)$ such that $x_i = a_i$ for all but a finite number of indices $i \in I$. 但是这些点$x$形式是$X$的密集子集（§ 4, no. 3，命题8）。 因此，$f$在$X$上连续，并且在$X$的密集子集上恒定，因此在$X$上恒定（§ 8, no. 1，命题2，推论1）。 但是$f$的这个与……矛盾定义。

### 5. 成分

Given a point $x$ of a topological space $X$, the union of the connected subsets of $X$ which contain $x$ is connected (no. 1, Proposition 2); it is therefore the largest connected subset of $X$ which contains $x$.

#### 定义 3 {#top-i-s11-def-3 .statement tag=0BBV}

拓扑空间$X$的点的分量（或连通分量）是最大的连接到$X$的子集，其中包含这个点。 $X$的子集$A$的分量是$A$的点的分量，相对于$X$的子空间$A$。

如果空间是连通的，则每个点的分量就是整个空间。如果空间$X$使得对于$X$的点的每个对$(x, y)$都有一个相连的集合包含$x$和$y$，则$X$是相连的。

如果$X$的每个点的分量仅由点组成，则空间$X$被称为“完全断开”。如果$X$的子空间$A$完全断开，则$X$的子集$A$是*完全断开的集合*。

一个*离散* 空间是完全不相连的，但是应该注意不要混淆这两个概念；对于例，我们将在章IV, § 2, no. 5中看到，有理线（不是离散的空间）是完全断开的。

集合 *既开又闭* 包含每个点、从而的分量 *点的分量包含在集合的交中，集合既开又闭，并且包含这个点*。然而，点的分量不一定等于这个交（cf.习题9和章II, § 4, no. 4、命题6）。

#### 命题 9 {#top-i-s11-prop-9 .statement tag=0BBW}

*拓扑空间$X$中任何点的分量都是闭集合。 关系“y 属于到x的分量”是$X$上的等价关系$R \{ x, y \}$，等价类是$X$的分量。商空间 $X/R$ 完全不相连。*

命题的第一个部分是定义3的直接的推论，并且连通的集合的闭包是连通的（no. 1，命题1）。由于集合的并在公共的中有点是相连的（no. 1，命题2），关系$R$是传递的，因此是等价关系（因为它显然是自反和对称的）并且$x$相对于$R$的等价类是$x$的分量。仍有待证明 $X/R$ 完全断开。令$f : X \to X/R$为典范映射，并令$F$为$X/R$*包含中至少两个不同的点*中的闭集合； $F$的逆像$f^{-1}(F)$在$X$中闭合，相对于$R$饱和，并且包含至少有$X$的两个不同分量，因而*不连接*。因而$X$中存在两个非空闭集合$B, C$，使得$B \cap C = \varnothing$和$B \cup C = f^{-1}(F)$。 $f^{-1}(F)$ *in* $f^{-1}(F)$ 的任何点 $x$ 的分量与 $x$ *in* $X$ 的分量相同（通过 $R$ 的定义），因而 $B$ 和 $C$，其中*在* $f^{-1}(F)$ 中都是开和闭的，相对于 $R$ 是饱和的。因而，$f(B)$和$f(C)$在$X/R$、$f(B) \cup f(C) = F$和$f(B) \cap f(C) = \varnothing$关闭；这表明 $F$ *未连接*，因而 $X/R$ 完全断开连接。

#### 命题 10 {#top-i-s11-prop-10 .statement tag=0BBX}

在乘积空间$X = \prod_{i \in J} X_i$中，$X$中$x = (x_i)$的分量是因子$X_i$中$x_i$的分量的乘积。

此乘积集合已连接（no. 4，命题8）。相反，如果$A$是$X$的连通的子集，其中包含$x$，则$\operatorname{pr}_i(A)$是集合（no. 2，命题4）的连通，其中包含 $x$；从$A \subset \prod_i \operatorname{pr}_i(A)$开始，$A$包含在$x_i$的组件的乘积中。

### 6. 本地连接空间

#### 定义 4 {#top-i-s11-def-4 .statement tag=0BBY}

如果 $X$ 的每个点都具有连通的邻域的基本系统，则称拓扑空间 $X$ 是局部连通的。

\* 我们将在章IV, § 2, no. 5中看到，实直线是本地连接的空间。 \*
在空间$X$的每个点$x$处，$x$的一个连接的邻域的存在绝不意味着$X$是本地连接的。特别是，$X$可以连接，但不能本地连接（习题2和13）。相反，空间可以局部连接但不连接（例如，离散的空间其中包含多于一个点）。

#### 命题 11 {#top-i-s11-prop-11 .statement tag=0BBZ}

空间 $X$本地连接的必要且充分的条件是$X$中开放的集合的每个组件在$X$中开放。

条件就足够了，因为$x$相对于$x$的开邻域的分量就是$X$中$x$的邻域。

相反，令 $A$ 为本地连接的空间 $X$ 的开子集，令$B$ 为$A$ 的组件，并令$x \in B$。令$V$为$A$中包含的$x$的连通邻域；由定义个分量，$V$包含在$B$中；因而$B$在$X$开放（§ 1, no. 2，命题1）。

因而，$X$的本地连接空间$X$的组件形式划分进入开放集合，因而$X$是其组件的和（§ 2, no. 4，例3）。

#### 推论{#top-i-s11-n6-cor-1 .statement tag=0BC0}

令$U$为本地连接的空间$X$的开放子集，并令$V$为$U$的组件。那么$V$的边界（相对于$X$）包含在$U$的边界中。

因为$V$在$U$中开闭，因而$V$的边界点（相对于$X$）不能属于到$U$，因为它也是相对于$V$的边界点 $U$，没有。

#### 命题 12 {#top-i-s11-prop-12 .statement tag=0BC1}

局部连通的空间的每个商空间都是局部连通的。

令 $X$ 为$X$、$\varphi : X \to X/R$ 典范映射上的本地连接空间、$R$ 等价关系。设 $A$ 为开子集

X/R 和C A 的一个分量。则$\overline{\varphi}^1(C)$ 是$\overline{\varphi}^1(A)$ 的分量中的并；对于如果 $x \in \overline{\varphi}^1(C)$ 且 K 是 $\overline{\varphi}^1(A)$ 中 x 的分量，则 $\varphi(K)$ 连接 (no. 2, 命题 4)，包含在 A 中，且包含 $\varphi(x)$；因而$\varphi(K) \subset C$乘以C的定义，因而$K \subset \overline{\varphi}^1(C)$。由于X是本地连接的，并且$\overline{\varphi}^1(A)$在X中打开，因此从命题11可以得出$\overline{\varphi}^1(C)$在X中打开；因而，C在X/R中打开，因而，再次到命题11时，X/R本地连接。

#### 命题 13 {#top-i-s11-prop-13 .statement tag=0BC2}

a) 令 $(X_i)_{i \in I}$ 为一系列局部连接的空间，使得 $X_i$ 与除指标 $i \in I$ 的有限数之外的所有元素相连。 那么乘积空间$X = \prod_{i \in I} X_i$是本地连接的。

b) 相反，如果非空拓扑空间的族$(X_i)$的乘积是局部连通的，则每个$X_i$都是局部连通的，并且除了指标的有限数之外的所有$X_i$都是连通的。

a) 令 J 为 I 的有限子集，使得当且仅当 $i \in J$ 时，$X_i$ 不连通。让
$$
U = \prod_{i \in I} U_i
$$
是 X 的初等集合包含点 $x = (x_i)$，并令 K 为 I 的有限子集，使得 $U_i \neq X_i$ 当且仅当 $i \in K$。对于$i \notin J \cup K$，令$V_i$为$X_i$，对于$i \in J \cup K$，令$V_i$为包含在$U_i$中的$x_i$的连通邻域；那么
$$
V = \prod_{i \in I} V_i
$$
已连接（通过 no. 4 的命题 8），且 U 中包含 $x$ 的邻域。因此 X 是本地连接的。

b) 令$a = (a_i)$为X的点，并令V为X中$a$的连通邻域。由于除了指标 (§ 4, no. 1) 的有限数之外，我们还有 $\mathrm{pr}_i V = X_i$，因此从 no. 2、命题 4 可以得出，$X_i$ 是相连的，除了指标的有限数之外。另一方面，对于$X_x$中$a_x$的每个$x \in I$、每个$a_x \in X_x$和每个邻域$V_x$，存在X的点$x$使得$\mathrm{pr}_x x = a_x$，并且
$$
V = V_x \times \prod_{i \neq x} X_i
$$
X 中的 $x$ 为邻域； V 因此包含 $x$ 的连通邻域 W，其投影 $\mathrm{pr}_x W$ 是 $V_x$ 中包含的$a_x$ 的连通邻域 (no. 2, 命题 4 和§ 4, no. 2，命题5)。因此每个$X_x$都是本地连接的。

### 7. 应用：POINCARÉ-VOLTERRA 定理

#### 定理 1 {#top-i-s11-thm-1 .statement tag=0BC3}

设$X$是拓扑空间满足公理$(O_{III})$（但不一定是豪斯多夫），并假设$X$是连通的且是局部连通的。令$Y$为拓扑空间，其拓扑具有可数基，并令$p : X \to Y$为连续映射，使得对于每个$y \in Y$，$\overline{p}^{-1}(y)$是离散的子空间 $X$。最后让 $\mathfrak{B}$ 为子集的 $X$ 的集合，其内部覆盖$X$，这样：
(i)*$p$*的限制*对于每个*$V \in \mathfrak{B}$*是*$V$*到*$Y$的闭映射。
(ii) *每个* $V \in \mathfrak{B}$ *都有一个可数的子集，它密集于* $V$。

*那么空间* $X$ *是开集合的可数族中的并，每个开族集合都包含在* $\mathfrak{B}$的集合中。

令 $\mathfrak{B}$ 为拓扑 $Y$ 的可数基。如果 (i) $U \in \mathfrak{B}$ 和 (ii) $W$ 是 $\mathfrak{B}$ 的集合中包含的 $\overline{p}^{-1}(U)$ 的组成部分，我们可以说对 $(W, U)$ 是“可区分的”。

#### 引理 1 {#top-i-s11-lem-1 .statement tag=0BC4}

*如果*$x$*是*$X$中的任何点，*有一个杰出的对*$(W, U)$*使得*$x \in W$。

逆像$\overline{p}^{-1}(p(x))$是离散的，因此$X$中存在$x$的邻域，其除$x$之外的所有点$x'$都有像$p(x') \neq p(x)$；由于$X$满足$(O_{III})$，因此$x$与此性质存在一个*封闭*邻域$V$，并且我们还可以假设$V$包含在$\mathfrak{B}$的集合中。设$F$为$V$在$X$的边界。到定理的条件(i)，$p(F)$于$Y$关闭；由于$p(F)$不满足包含$p(x)$，因此存在集合$U \in \mathfrak{B}$，其中包含$p(x)$且不满足$p(F)$。设$W$为$\overline{p}^{-1}(U)$中$x$的分量；那么只要证明$W \subset A$就足够了。如果不是这样，则$W$将满足$F$（no. 1，命题3），因此$p(F)$将满足$U$，与$U$的定义相反。

#### 引理 2 {#top-i-s11-lem-2 .statement tag=0BC5}

*如果*$(W, U)$*是一个杰出的对，那么所有杰出的对*$(W', U')$*中的集合*使得*$W'$*满足*$W$*是可数的*。

由于$\mathfrak{B}$是可数的，因此足以证明，给定$U' \in \mathfrak{B}$，杰出的对$(W', U')$的集合使得$W'$满足$W$是可数的。现在这些集合$W'$是开放的，因为$X$是本地连接的（no. 6，命题11）并且相互不相交的，因为它们是$\overline{p}^{-1}(U')$的组件；因此集合 $W' \cap W$ 开且互不相交的。但是 $W$ 包含是一个可数子集，它在 $W$ 中是稠密的；因此$W'$的集合使得$W' \cap W$不为空也是可数的。

To prove Theorem 1, consider the following relation R between two points x, x' of X: "There exists a finite sequence of distinguished pairs (W_i, U_i) (1 \leq i \leq n) such that x \in W_1 and x' \in W_n and that W_i \cap W_{i+1} \neq \emptyset for \leq 1 i \leq n — 1."

引理 1 表明 R 是自反的，并且很容易验证 R 是对称且传递的，因此 R 是等价关系；另外，由于 W_i 是开路的，因此每个等价类 mod R 在X 中都是开路的。但X是连通的；因此只能有一个等价类，即X中的任意两个点全等mod R。由此我们可以推断，X是杰出对的第一个元素的可数族中的并，这将证明定理 1. 为此，令 x 为 X 中的任意点，并且在 X 的开子集的 n 序列 (C_n) 上通过归纳定义，如下： 引理 1 存在一个可区分的对 (W_1, U_1) 使得 x \in W_1，并且我们取 C_1 = W_1；如果 n > 1，则 C_n 为可区分的对 (W, U) 中所有第一个元素 W 的并，使得 W 满足 C_{n-1}。由n上的归纳立即表明，凭借引理2，C_n是可数的并可区分的对的第一个元素。最后，每个 x' \in X 属于到某个 C_n；因为有有限序列

$$(W'_i, U'_i)_{1 \leq i \leq m}$$

的对使得 x \in W'_1、x' \in W'_m 和 W'_i \cap W'_{i+1} \neq \emptyset for 1 \leq i \leq m — 1，并且通过 i 上的归纳，我们看到 W'_i \子集 C_{i+1} 对于所有 i，因此 x' \in C_{m+1}。

Q.E.D.

#### 推出 1 {#top-i-s11-lem-2-cor-1 .statement tag=0BC6}

令 Y 为正则空间，其拓扑具有可数基 (*)。令 X 为连通且局部连通的空间，并令 p : X \to Y 为连续映射，并具有以下性质：对于 X 中的每个 x \，在 X 中存在 x 的闭邻域 V，使得p 的限制到 V 是 V 到 Y 的闭子空间的同胚。那么 X 是正则，X 的拓扑具有可数基。

首先，假设意味着X是正则的（§ 8, no. 4，命题13）。让我们证明，如果我们取 \mathfrak{B} 为 X 的所有闭子集 V 的集合，则满足定理 1 的条件，使得 p 到 V 的限制是 V 在 a 上的同胚Y 的子空间闭合。到假设，\mathfrak{B} 的集合的内部覆盖 Y，并且凭借 Y 上的假设，\mathfrak{B} 中的每个 V \in 有一个可数基，因此包含是一个可数稠密子集（§ 1, no. 6，命题6）。此外，如果 x \in p^{-1}(y)，则 X 中 x 的 \mathfrak{B} 存在邻域 V \in \mathfrak{B}，使得 V con-

(*) \* 可以证明，这些条件意味着Y的拓扑是可度量的（章IX, § 4，习题22）。 \* 除了 $x$ 之外，$\overline{p}^{-1}(y)$ 不包含点，因此 $\overline{p}^{-1}(y)$ 是一个离散的空间。因此，我们可以得到应用定理 1，这表明$X$是开放集合的可数族$(T_n)_{n \geq 0}$的并，这样每个子空间$T_n$都有一个可数基$(U_{mn})_{m \geq 0}$。然后是$X$（$§ 3$，no. 1，注）的拓扑的$U_{mn}$（$m \geq 0, n \geq 0$）形式基。

#### 推论 2 {#top-i-s11-lem-2-cor-2 .statement tag=0BC7}

*令$X$局部紧致、连通且局部连通，并假设$X$的每个点都有邻域，邻域有可数的基。令 $Y$ 为 Hausdorff 空间，其拓扑具有可数基，并令 $p : X \to Y$ 为连续映射，使得对于每个 $y \in Y$，$\overline{p}^{-1}(y)$ 为离散子空间 $X$。那么$X$的拓扑有一个可数的基。*

对于每个$x \in X$，令$V_x$是$X$中$x$的紧凑邻域，其中基可数。由$§ 9$、no. 4、定理 2、推论2得出，$V_x$的集合$\mathfrak{B}$满足定理1的条件，并且我们完成证明，如推论1。

请注意，在这个推论中，$p$的限制到$X$的点的任意小邻域$V$*不是$V$到$p(V)$*的同胚。

#### 推论 3（庞加莱-沃尔泰拉定理）{#top-i-s11-lem-2-cor-3 .statement tag=0BC8}

*令$Y$为局部紧致、局部连通的空间，其拓扑有可数基。令$X$为连通豪斯多夫空间，并令$p : X \to Y$为连续映射，其具有以下性质：对于每个$x \in X$，存在$x$的开邻域$U$ $X$使得$p$到$U$的限制是$U$到$Y$的开子空间的同胚。那么$X$是局部紧致且局部连通的，$X$的拓扑有一个可数的基。*

显然 $X$ 是本地连接的。此外，每个$x \in X$在$X$中都有一个开邻域$U$，使得$p$的限制到$U$映射$U$同构到开子空间$p(U)$ $Y$。由于$p(U)$是$Y$的局部紧子空间（$§ 9$，no. 7，命题13），$p(U)$中包含$p(x)$的紧邻域$W$， 从而 $U \cap \overline{p}^{-1}(W)$ 是 $U$ 中包含的 $x$ 的紧致邻域；因此$X$是局部紧的，因为假设$X$是Hausdorff。 $U \cap \overline{p}^{-1}(W)$是紧致的，在$X$（$§ 9$，no. 3，命题4）中是封闭的，因此满足推论1的条件；因此$X$的拓扑有一个可数的基。

### 习题 {#top-i-s11-exercises}

请参阅[习题为 § 11](exercises/s11/)。
