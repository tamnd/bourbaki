---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 3
section_title: Complete spaces
lang: zh
source: top-i-iv
book_pages: 181-198, 208-209
pdf_pages: 0187-0204, 0214-0215
extraction: ocr
subsections:
    - "no": 1
      title: CAUCHY FILTERS
      page: 181
      pdf_page: 187
    - "no": 2
      title: MINIMAL CAUCHY FILTERS
      page: 183
      pdf_page: 189
    - "no": 3
      title: COMPLETE SPACES
      page: 184
      pdf_page: 190
    - "no": 4
      title: SUBSPACES OF COMPLETE SPACES
      page: 186
      pdf_page: 192
    - "no": 5
      title: PRODUCTS AND INVERSE LIMITS OF COMPLETE SPACES
      page: 186
      pdf_page: 192
    - "no": 6
      title: EXTENSION OF UNIFORMLY CONTINUOUS FUNCTIONS
      page: 190
      pdf_page: 196
    - "no": 7
      title: THE COMPLETION OF A UNIFORM SPACE
      page: 191
      pdf_page: 197
    - "no": 8
      title: THE HAUSDORFF UNIFORM SPACE ASSOCIATED WITH A UNIFORM SPACE
      page: 196
      pdf_page: 202
    - "no": 9
      title: COMPLETION OF SUBSPACES AND PRODUCT SPACES
      page: 197
      pdf_page: 203
statements: 48
exercises: 7
content_sha256: 0e6316f3ac8281d9e8abe0ede787d1548ce0c028c7483cf70f0781191ec06571
translated_from: content/en/top/II/03_s3_complete_spaces.md
translation_method: google
source_content_sha256: 4fff5edd8ba62b0c67040f4aad9934e1ca08a8f7749a27d75004f56f99335c47
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: b6a4557b3eb0a0836aa687a2958cb6405d4db1c3ae9bb48915e5eaf26c0131e3
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 3. 完成空间

### 1.柯西滤波器

一旦集合$X$被赋予了制服结构，我们就可以定义什么是$X$的“小”子集（相对于这个结构）：$X$的“小”子集是其中所有点都是的一个彼此“非常接近”。恰恰：

#### 定义 1 {#top-ii-s3-def-1 .statement tag=0BEE}

如果$X$是制服空间且$V$是$X$的随从，则$X$的子集$A$被称为$V$-小，如果$A$的点的每个对都是$V$-关闭（在其他字，如果$A \times A \subset V$）。

#### 命题 1 {#top-ii-s3-prop-1 .statement tag=0BEF}

在统一的空间$X$中，如果两个集合$A$和$B$是$V$小并且相交，那么它们的并$A \cup B$是$\vec{V}$小。

令$x$和$y$为$A \cup B$中的任意两个点，并令$Z \in A \cap B$。然后$(x, z) \in V$和$(z, y) \in V$，所以$(x, y) \in \overline{V}$。

#### 定义 2 {#top-ii-s3-def-2 .statement tag=0BEG}

*制服空间$X$上的过滤器$\mathfrak{F}$是柯西过滤器，如果对于$X$的每个随行人员$V$，$X$有子集，$V$小，属于到$\mathfrak{F}$。*

在这里，我们可以再次通过使用“足够小集合”和“a 集合尽可能小”这样的表达方式来使我们的语言更具表现力；因此定义 2 可以通过说重述，柯西滤波器是一个包含 *任意小集合*。

如果与序列关联的基本滤波器是柯西滤波器，则均匀空间 $X$ 的点的无限序列 $(u_n)$ 被称为 *Cauchy 序列*。对于$X$的每个随行人员$V$，都有整数$n_0$，这样对于所有整数$m \geq n_0$和$n \geq n_0$，我们就有$(u_m, u_n) \in V$，这也是同样的道理。

#### 命题 2 {#top-ii-s3-prop-2 .statement tag=0BEH}

*在统一的空间$X$上，每个收敛滤波器都是柯西滤波器。*

如果$x$是$X$的任意点且$V$是$X$的任意对称周边，则$x$的邻域$V(x)$是$\overline{V}$小。如果$\mathfrak{F}$是收敛到$x$的滤波器，则$V(x)$中包含$\mathfrak{F}$的集合，因此$V$小。

显然，每个比柯西滤波器 *更细* 的滤波器都是柯西滤波器。

#### 命题 3 {#top-ii-s3-prop-3 .statement tag=0BEI}

*令$f : X \to X'$为均匀连续的映射。那么$X$上的柯西滤波器基的$f$下的像是$X'$上的柯西滤波器基。*

让$g = f \times f$。如果$V'$是$X'$的随从，则$\overline{g^{-1}(V')}$是$X$的随从，$\overline{g^{-1}(V')}$-小集合的$f$下的像是$V'$-小；因此结果。

特别是，如果均匀空间 $X$ 的均匀性被*粗糙*均匀性替换，则相对于原始均匀性的每个柯西滤波器仍然是相对于新均匀性的柯西滤波器。

这个事实可以在下面的形式中轻松记住：*更细均匀性，柯西滤波器越少*。

#### 命题 4 {#top-ii-s3-prop-4 .statement tag=0BEJ}

*令$X$为集合，令$(Y_i)_{i \in I}$为制服空间的族，对于每个$i \in I$，让$f_i$为$X$到$Y_i$的映射。令 $X$ 具有最粗糙的均匀性 $U$，其中 $f_i$ 是均匀连续的。那么在阶中，$X$上的滤波器基$\mathfrak{B}$应该是柯西滤波器基，对于每个$i \in I$，$f_i(\mathfrak{B})$应该是$Y_i$上的柯西滤波器基是必要且充分的。*

条件是命题 3 所必需的。反之，假设满足，令$U(V_{i_1}, \ldots, V_{i_n})$ 为均匀性$\mathfrak{U}$ [§ 2, no. 3, 公式 (1)] 的随从。到假设，对于每个指标$k$，都有集合$M_k \in \mathfrak{B}$，这样$f_{i_k}(M_k)$是$V_{i_k}$小（$1 \leq k \leq n$）。令$M$为$1 \leq k \leq n$包含在$M_k$中的$\mathfrak{B}$的集合；那么对于点 $x, x'$ $M$ 的每一个对，我们都有 $[f_{i_k}(x), f_{i_k}(x')] \in V_{i_k}$ 对应 $1 \leq k \leq n$，这样
$$
(x, x') \in U(V_{i_1}, \ldots, V_{i_n}).
$$
这样就完成了证明。

#### 推论 1 {#top-ii-s3-prop-4-cor-1 .statement tag=0BEK}

*如果均匀空间 $X$ 诱导上的柯西滤波器在 $X$ 的子集 $A$ 上的滤波器，则该滤波器是均匀子空间 $A$ 上的柯西滤波器。*

#### 推论 2 {#top-ii-s3-prop-4-cor-2 .statement tag=0BEL}

*均匀空间的乘积$\prod_{i \in I} X_i$上的滤波器基$\mathfrak{B}$是柯西滤波器基当且仅当，对于每个$i \in I$，$\operatorname{pr}_i(\mathfrak{B})$是柯西滤波器基 $X_i$.*

### 2. 最小柯西滤波器

均匀空间 $X$ 上柯西滤波器的集合的最小元素（相对于包含）称为 $X$ 上的*最小柯西滤波器*。

#### 命题 5 {#top-ii-s3-prop-5 .statement tag=0BEM}

*令$X$为制服空间。对于$X$上的每个柯西滤波器$\mathfrak{F}$，都有一个比$\mathfrak{F}$更粗糙的独特的最小柯西滤波器$\mathfrak{F}_0$。如果$\mathfrak{B}$是$\mathfrak{F}$的基且$\mathfrak{G}$是$X$的对称周边的基本系统，则集合$V(M)$($M \in \mathfrak{B}, V \in \mathfrak{G}$)形式基 $\mathfrak{F}_0$。

如果$M, M'$在$\mathfrak{B}$中且$V, V'$在$\mathfrak{G}$中，则存在集合$M'' \in \mathfrak{B}$（或$V'' \in \mathfrak{G}$）使得$M'' \subset M \cap M'$（或$V'' \subset V \cap V'$）；因此$V''(M'') \subset V(M) \cap V'(M')$，因此集合$V(M)$（$M \in \mathfrak{B}, V \in \mathfrak{G}$）实际上是$X$上的过滤器$\mathfrak{F}_0$的形式基。进一步，如果$M$是$V$-小，则$V(M)$是$V$-小；因此 $\mathfrak{F}_0$ 是柯西滤波器，并且明显比 $\mathfrak{F}$ 更粗糙。为了完成证明，只要证明如果$\mathfrak{G}$是比$\mathfrak{F}$更粗糙的柯西滤波器，那么$\mathfrak{G}$比$\mathfrak{F}_0$是更细。对于每个$M \in \mathfrak{B}$和每个$V \in \mathfrak{G}$，都有集合$N \in \mathfrak{G}$，即$V$小；从$N \in \mathfrak{F}$开始，$N$满足$M$；因此$N \subset V(M)$，所以$V(M) \in \mathfrak{G}$。

#### 推论 1 {#top-ii-s3-prop-5-cor-1 .statement tag=0BEN}

*对于每个$x \in X$，$X$中$x$的邻域滤波器$\mathfrak{B}(x)$是最小柯西滤波器。*

取命题 5中的$\mathfrak{F}$作为$X$中所有子集的过滤器，其中包含$x$，并取$\mathfrak{B}$由单个元素$\{x\}$组成。

#### 推论 2 {#top-ii-s3-prop-5-cor-2 .statement tag=0BEO}

*柯西滤波器* $\mathfrak{F}$ *的每个簇点* $x$ *是* $\mathfrak{F}$的极限点。

有一个过滤器$\mathfrak{G}$，它比$\mathfrak{F}$和$\mathfrak{B}(x)$都更细（章I, § 7, no. 2，命题4）；由于 $\mathfrak{F}$ 是柯西滤波器，因此 $\mathfrak{G}$ 也是。如果$\mathfrak{F}_0$是比$\mathfrak{F}$粗的唯一最小柯西滤波器，则$\mathfrak{F}_0$和$\mathfrak{B}(x)$都是比$\mathfrak{G}$粗的最小柯西滤波器。因此$\mathfrak{F}_0 = \mathfrak{B}(x)$，这表明$\mathfrak{F}$收敛于$x$。

#### 推论 3 {#top-ii-s3-prop-5-cor-3 .statement tag=0BEP}

*每个柯西滤波器比收敛到点* $x$ 的滤波器更粗糙，*也收敛到* $x$。

这是推论 2 的推论。

#### 推论 4 {#top-ii-s3-prop-5-cor-4 .statement tag=0BEQ}

*如果* $\mathfrak{F}$ *是一个最小柯西滤波器，那么* $\mathfrak{F}$ *的每个集合都有一个非空内部，其中也有属于到* $\mathfrak{F}$ *（在其他字，$\mathfrak{F}$有基由……组成）打开集合)*。

设$V$为$X$的任意随从；那么就有一个开放的随从$U \subset V$（$\S$1，no. 2，推论2到命题2）。对于$X$中的每个子集$M$，$U(M)$是开集并且包含在$V(M)$中；鉴于命题 5，因此得出结果。

### 3. 完成空间

在统一的空间$X$中，*柯西滤波器不需要有极限点*。

#### 例 1 {#top-ii-s3-n3-exa-1 .statement tag=0BER}

考虑$u_n = \sum_{p=0}^n 2^{-p(p+1)/2}$定义的有理线$\mathbf{Q}$上的序列$(u_n)$。如果 $m > n$ 我们有
$$
|u_m - u_n| \leq 2^{-n(n+3)/2}
$$
因此$(u_n)$是*柯西序列*。但是这个序列在$\mathbf{Q}$中没有极限；因为如果有理数数 $a/b$ 是 $(u_n)$ 的极限，那么通过 (1) 我们应该有所有 $n$
$$
|a/b - h_n/2^{n(n+1)/2}| \leq 1/2^{n(n+3)/2}
$$
其中$h_n$是整数（取决于$n$）；也就是说，
$$
|a \cdot 2^{n(n+1)/2} - b h_n| \leq b \cdot 2^{-n}
$$
对于所有$n$。现在，对于所有 $n$，此不等式的左侧为整数，因此只要 $n$ 大于整数 $n_0$，使得 $b < 2^{n_0}$ ，则必须为零；因此，我们应该为所有 $n > n_0$ 提供 $a/b = u_n$，这是荒谬的。

#### 例 2 {#top-ii-s3-n3-exa-2 .statement tag=0BES}

令$X$为无限集合，并考虑有限划分在$X$（$\S$2，no. 2，注1）上的均匀性。 $X$ 上的每个*超滤* $\mathfrak{F}$ 都是一个

柯西滤波器关于这种均匀性。因为如果 $(A_i)$ 是 $X$ 的有限划分并且
$$
V = \bigcup_i (A_i \times A_i)
$$
相应的随行人员，则$A_i$属于至$\mathfrak{F}$中至少之一（章I, § 6, no. 4，推论命题5），并且$A_i$是V-小。另一方面，$X$是无限离散的空间，因此不是紧致的，因而$X$上存在不收敛的超滤波器。

#### 定义 3 {#top-ii-s3-def-3 .statement tag=0BET}

*完整的空间是一个均匀的空间，其中每个柯西滤波器都收敛。*

因而，在完备的空间中，每个 *Cauchy 序列* (no. 1) 都是收敛的。

#### 例{#top-ii-s3-n3-exa-3 .statement tag=0BEU}

在“离散”均匀空间 $X$ 上，柯西滤波器是一个平凡的超滤波器（章 I, § 6, no. 4），因此是收敛的；因而，$X$是完整的。

从no. 1的定义2和3以及no. 1的命题2，我们推导出以下命题，称为*柯西准则*：

#### 命题 6 {#top-ii-s3-prop-6 .statement tag=0BEV}

*令$\mathfrak{F}$为集合$X$的过滤器，并令$f$为$X$的映射成为完整的均匀空间$X'$。那么$f$相对于$\mathfrak{F}$有极限当且仅当$f$下$\mathfrak{F}$的像是柯西滤波器基。*

这个标准显示了完整的空间在涉及极限的概念的所有问题中的重要性：如果函数在完整的空间中取其值，我们可以证明极限的*存在*无需提前知道值共极限*；如果极限中的定义是我们可以使用的唯一收敛标准，那么这是不可能的。

*更细* 比完整空间均匀度的均匀度不必是完整空间 (习题 2) 的均匀度。然而，我们有以下命题：

#### 命题 7 {#top-ii-s3-prop-7 .statement tag=0BEW}

*令$\mathfrak{U}_1, \mathfrak{U}_2$为集合$X$上的两个均匀性，并令$\mathfrak{T}_1, \mathfrak{T}_2$分别为由这些均匀性引起的拓扑。假设$\mathfrak{U}_1$比$\mathfrak{U}_2$是更细，并且$\mathfrak{U}_1$有一个基本的系统随行人员，这些随行人员在拓扑$\mathfrak{T}_2 \times \mathfrak{T}_2$的$X \times X$关闭。那么$X$上的滤波器$\mathfrak{F}$收敛于拓扑$\mathfrak{T}_1$当且仅当它是均匀性$\mathfrak{U}_1$中的柯西滤波器并且收敛于拓扑$\mathfrak{T}_2$。*

条件显然是必要的，因为 $\mathfrak{T}_2$ 比 $\mathfrak{T}_1$ 更粗糙。反之，假设满足条件，则令$x$相对于$\mathfrak{T}_2$为$\mathfrak{F}$的极限点；我们将证明$x$是$\mathfrak{F}$相对于$\mathfrak{T}_1$的极限。令 $V$ 为 $\mathfrak{U}_1$ 的对称周边，在拓扑 $\mathfrak{T}_2 \times \mathfrak{T}_2$ 中闭合。 假设、$\mathfrak{F}$ 包含集合 $M$，其中V小；因而，如果$x' \in M$我们有$M \subset V(x')$。但$V(x')$于拓扑$\mathfrak{T}_2$关闭；因而$x$位于$M$相对于$\mathfrak{T}_2$的闭包，必须属于到$V(x')$。由此可见$M \subset \hat{V}(x)$、命题得证。

#### 推出 {#top-ii-s3-n3-cor-1 .statement tag=0BEX}

在命题7的条件中，如果$U_2$是完整的空间的一致，那么$U_1$也是。

对于每个关于$U_1$的柯西滤波器都是关于$U_2$的柯西滤波器，因此收敛于拓扑$\mathfrak{T}_2$。

注当$\mathfrak{T}_1 = \mathfrak{T}_2$（§ 1, no. 2，推论2至命题2）时，满足命题7的推论假设。

### 4. 子空间完整空间

#### 命题 8 {#top-ii-s3-prop-8 .statement tag=0BEY}

完整的空间的每个闭合的子空间都是完整的。 Hausdorff 制服空间的每个完整子空间（完整或不完整）都是封闭的。

令$X$为完整的空间，并令$A$为$X$的闭子空间。如果$\mathfrak{F}$是$A$上的柯西滤波器，那么它是$X$（no. 1，命题3）上的柯西滤波器基，因此收敛到点$x \in X$；但由于$A$是封闭的，我们有$x \in A$，因此$\mathfrak{F}$收敛于子空间$A$。

现在令$\overline{A}$为Hausdorff制服空间$X$的非闭子集，并令$b \in \overline{A} - A$。 $X$中$b$的邻域滤波器$\mathfrak{B}$在$A$上的迹$\mathfrak{B}_A$是$A$上的柯西滤波器；但它不能收敛于点$c \in A$，否则$c$将是$\mathfrak{B}$的极限点（no. 2，命题5，推论3），这是荒谬的，因为$b \neq c$和$X$ 是豪斯多夫。

#### 命题 9 {#top-ii-s3-prop-9 .statement tag=0BEZ}

令$X$为均匀空间，并令$A$为$X$的密集子集，使得$A$上的每个柯西滤波器基收敛于$X$。那么$X$就完成了。

足以证明$X$上的每个最小柯西滤波器$\mathfrak{F}$是收敛的。由于$A$是稠密的，并且$\mathfrak{F}$的每个集合都有一个非空内部（no. 2，推论4到命题5），$\mathfrak{F}$在$A$上的迹$\mathfrak{F}_A$是一个柯西滤波器$A$，因此收敛到点$x_0 \in X$。由于$\mathfrak{F}$比$\mathfrak{F}_A$生成的$X$上的过滤器更粗糙，因此$\mathfrak{F}$收敛到$x_0$（no. 2，推论3到命题5）。

### 5. 完整的空间的乘积和逆极限

#### 命题 10 {#top-ii-s3-prop-10 .statement tag=0BF0}

完整制服空间的每乘积都已完成。反之，如果非空制服空间的乘积是完整的，那么每个因子都是完整的制服空间。

第一个断言是乘积空间上柯西滤波器和收敛滤波器刻画的推论（no. 1，推论2到命题4和章I, § 7, no. 6，推论） 1 至命题 10)。相反，假设

$$
X = \prod_{i \in I} X_i
$$

是完整的（$X_i$非空），并让$\mathfrak{F}_x$是$X_x$上的柯西滤波器。对于每个$i \neq x$，令$\mathfrak{F}_i$为$X_i$上的柯西滤波器，并考虑乘积滤波器（章I, § 6, no. 7）

$$
\mathfrak{F} = \prod_{i \in I} \mathfrak{F}_i \text{ on } X;
$$

$\mathfrak{F}$ 是柯西滤波器（no. 1，推论 2 到命题 4），因此是收敛的，因此每个 $\operatorname{pr}_x \mathfrak{F} = \mathfrak{F}_x$ 也是收敛的（章 I, § 7, no. 6，推论 1 到命题 10）。

#### 推论{#top-ii-s3-n5-cor-1 .statement tag=0BF1}

*设*$(X_\alpha, f_{\alpha\beta})$*为统一空间的逆系。**如果*$X_\alpha$*是豪斯多夫且完备，那么*$X = \varprojlim X_\alpha$也是。

对于 $X$ 是 Hausdorff，可以用 $\prod_{i \in I} X_\alpha$ 的 *封闭* 子空间来识别（章 I, § 8, no. 2，推论 2 到命题 7）；因此，从命题 10 和命题 8 (no. 4) 可以得出推论。

完整豪斯多夫均匀空间$X_\alpha$的逆极限可以是*空*，即使所有$X_\alpha$非空并且所有$f_{\alpha\beta}$都是满射，如离散空间的情况所示（*集合理论*，章） III, § 1，习题32）。然而，我们有以下定理：

#### 定理 1（米塔格-莱弗勒）{#top-ii-s3-thm-1 .statement tag=0BF2}

*令* $(X_\alpha, f_{\alpha\beta})$ *为完整Hausdorff制服空间的逆系，由有向集合* $I$ *索引，其具有可数的共尾子集；还假设，对于每个* $\alpha \in I$，$X_\alpha$ *都有可数的基本随行人员系统* (*)。 *最后，假设对于每个* $\alpha \in I$ *有指标* $\beta \geq \alpha$ *满足以下条件*：

(ML$_{\alpha\beta}$) *对于每个* $\gamma \geq \beta$，$f_{\alpha\gamma}(X_\gamma)$ *密集于* $f_{\alpha\beta}(X_\beta)$。

*令*$X = \varprojlim X_\alpha$*并令*$f_\alpha$*为典范映射*$X \to X_\alpha$。 *然后对于每个* $\alpha \in I$ *和每个* $\beta \geq \alpha$ *满足* (ML$_{\alpha\beta}$)，$f_\alpha(X)$ *稠密于* $f_{\alpha\beta}(X_\beta)$ *（因而，如果* $X_\alpha$ *都非空，则* $X$ *非空）*。

设$(\lambda_n)$为$I$中指标共尾的序列。从指标 $\alpha_0 \in I$ 和定义开始，递归递增序列 $(\alpha_n)$，使得 $\alpha_n \geq \lambda_n$ 且 (ML$_{\alpha_n, \alpha_{n+1}}$) 为真。显然序列

(*) *这个条件表示 Hausdorff 制服空间* $X_\alpha$ *是可度量的； cf.章IX, § 2, no. 4、定理1.*

(α_n) 在 I 中是共尾的。当 m ≤ n 时，我们将写 f_{mn} 代替 f_{α_mα_n}，并且我们将 f_{n, n+1}(X_{α_{n+1}}) = Y_n。那么，如果 m ≤ n，则 f_{mn}(Y_n) 在 Y_m 中是稠密的；对于定义 f_{m, n+1}(X_{α_{n+1}}) 来说是稠密的

f_{m, m+1}(X_{α_{m+1}}) = Y_m，f_{m, n+1}(X_{α_{n+1}}) = f_{mn}[f_{n, n+1}(X_{α_{n+1}})] = f_{mn}(Y_n)。

通过 n 和 k 上的归纳，我们可以为每个 n 定义一个 X_{α_n} 的封闭对称周边的基本系统 (V_{kn})_{k∈\mathbf{N}} 使得

(2)
$\overset{2}{V}_{k+1, n} \subset V_{kn}$,

(3)
$(f_{n, n+1} \times f_{n, n+1})(V_{k, n+1}) \subset V_{kn}$。

实际上，令 (U_{kn})_{k∈\mathbf{N}} 为 X_{α_n} 随从的基本系统。如果我们假设 V_{kn} 已经为给定的 n 和所有 k ∈ \mathbf{N} 定义，那么由于 f_{n, n+1} 是一致连续的，我们可以通过 k 上的归纳定义周围环境 V_{k, n+1} 来满足 (3) 且

$\overset{2}{V}_{k+1, n+1} \subset V_{k, n+1} \cap U_{k+1, n+1}$

接下来是断言。

现在令 x_0 ∈ Y_0。我们将证明，对于每个整数 k > 0，都有点 z ∈ X，使得 [x_0, f_{α_0}(z)] ∈ V_{k-1, 0}；这将证明定理。由于 f_{n, n+1} (Y_{n+1}) 在 Y_n 中是稠密的，因此我们可以通过点 x_n ∈ Y_n 的归纳序列定义使得

(4)
$$ [x_n, f_{n, n+1}(x_{n+1})] \in V_{k+n, n} $$

根据 (3) 可知，如果 m ≤ n 则

(5)
$$ [f_{mn}(x_n), f_{m, n+1}(x_{n+1})] \in V_{k+n, m} $$

由此我们结论对于固定的m序列(f_{mn}(x_n))_{n≥m}是X_{α_m}中的柯西序列，因此收敛到点z_m；对于归纳，从 (5) 可以得出，对于整数的每个对 p ≥ m, q > 0，我们有

(6)
$$ [f_{mp}(x_p), f_{m, p+q}(x_{p+q})] \in V_{k+p+q-1, m} \circ V_{k+p+q-2, m} \circ ... \circ V_{k+p, m} $$

且根据(2) 显然，(6) 的右侧包含在V_{k+p-1, m} 中。令q无限增加；我们特别推断，对于 m = p = 0，我们有 (x_0, z_0) ∈ V_{k-1, 0}，因为 V_{k-1, 0} 是封闭的。另一方面，根据关系 z_m = \lim_{n→∞} f_{mn}(x_n) 以及 f_{m, m+1} 的连续性，我们推导出对于每个 m ≥ 0，f_{m, m+1}(z_{m+1}) = z_m。对于每个 γ ∈ I，至少有一个整数 n 使得 α_n ≥ γ；放入$z_\gamma = f_{\gamma, \alpha_n}(z_n)$，我们立即验证$z_\gamma$不依赖于$n$的值，从而导致$\alpha_n \geq \gamma$，并且如此定义的族$(z_\alpha)_{\alpha \in I}$是$X = \varprojlim X_\alpha$的点$z$。从 $f_{\alpha_0}(z) = z_0$ 开始，证明已完成。

#### 推出 1 {#top-ii-s3-thm-1-cor-1 .statement tag=0BF3}

*令* $(X_\alpha, f_{\alpha \beta})$ *为由有向集合* $I$ *索引的集合的逆系，其具有可数共尾子集，并假设* $f_{\alpha \beta}$ *是满射的。那么如果*$X = \varprojlim X_\alpha$，*典范映射*$f_\alpha : X \to X_\alpha$*对于每个*$\alpha \in I$都是满射。

让每个$X_\alpha$具有离散均匀性，并且应用定理为1。

#### 推出 2 {#top-ii-s3-thm-1-cor-2 .statement tag=0BF4}

*设* $I$ *为有向集合，它有一个可数的共尾子集。设* $(X_\alpha, f_{\alpha \beta})$ *和* $(X'_\alpha, f'_{\alpha \beta})$ *为集合中的两个逆系，由* $I$索引，*并且对于每个* $\alpha \in I$ *让* $u_\alpha : X_\alpha \to X'_\alpha$ *为映射，使得* $u_\alpha$ *形式逆系共映射。让*$u = \varprojlim u_\alpha$。 *设*$x = (x'_\alpha)$*为*的元素

$$
X' = \varprojlim X'_\alpha
$$

*满足以下条件：对于每个*$\alpha \in I$*有指标*$\beta \geq \alpha$*这样对于所有*$\gamma \geq \beta$*我们有*$f_{\alpha \gamma}(\overline{u}_\gamma^{-1}(x_\gamma)) = f_{\alpha \beta}(\overline{u}_\beta^{-1}(x'_\beta))$。 *然后有元素* $x \in X$ *这样* $u(x) = x'$。

集合$\overline{u}_\alpha^{-1}(x'_\alpha)$的应用定理1到逆系，每个都带有离散均匀性。

#### 例 {#top-ii-s3-n5-exa-1 .statement tag=0BF5}

假设我们在 $C$ 中给出： (i) 序列 $(a_n)$ 不同的点使得序列 $(|a_n|)$ 是递增并且趋于 $+\infty$； (ii) 对于每个$n$，在$C - \{a_n\}$中定义一个有理函数$z \to R_n(z)$，并且在$a_n$处有一个极点； (iii) 递增序列 $(B_n)$ 以 0 为中心的开盘，其并为 $C$，并且没有一个 $a_k$ 位于任何盘 $B_n$ 的边界上。对于每个$n$，令$B'_n$表示$\overline{B}_n$的交以及点$a_n$的集合$C$中的补集；并令 $X_n$ 表示所有映射中的集合

$$
z \to S(z) = P(z) + \sum_{a_k \in B'_n} R_k(z)
$$

$B'_n$到$C$，其中$P$是函数的限制到$B'_n$，在$\overline{B}_n$是连续的，在$B_n$是全纯的。我们将定义放入 $X_n$ 中，将

$$
d_n(S_1, S_2) = \sup_{z \in B'_n} |S_1(z) - S_2(z)|.
$$

很容易验证$X_n$对于这个指标来说是“完整的”。最后，对于$n \leq m$，我们定义映射$f_{nm} : X_m \to X_n$，这样如果$S \in X_m$则$f_{nm}(S)$是$S$到$B'_n$的*限制*。很明显，$f_{nm}$是*均匀连续的*并且$(X_n, f_{nm})$是均匀空间的逆系。既然如此，逆极限$X = \lim_{\leftarrow} X_n$的元素可以被规范地等同于$\mathbf{C}$中的亚态函数$F$，其唯一的极点是点$a_n$，并且对于每个$n$， $F(z) - R_n(z)$ 在 $a_n$ 是全纯的。 Mittag-Leffler 的经典定理断言 $X$ 不为空；凭借定理 1，我们只需验证所有$n$的条件（ML$_{nn}$）。让
$$
S_n = P_n + \sum_{a_k \in B_n} R_k
$$
是$X_n$的元素，其中$P_n$在$\overline{B}_n$中连续，在$B_n$中全纯；对于任意 $m \geq n$，令 $Q_{mn}$ 为限制
$$
\sum_{a_h \in B_m - B_n} R_h \text{ to } B'_n;
$$
后者和是$\overline{B}_n$的某些邻域中的全纯函数，因此（根据泰勒的定理）对于每个$\varepsilon > 0$，都有一个多项式$P_{mn}$，使得$B_n$中有$|Q_{mn}(z) - P_{mn}(z)| \leq \varepsilon$；如果$S_m$是$S_n + Q_{mn} - P_{mn}$到$B'_m$的限制，我们在$B'_n$中有$S_m \in X_m$和$|S_m(z) - S_n(z)| \leq \varepsilon$。这样就完成了证明。 \*

### 6. 扩张均匀连续函数

扩张的定理通过连续性（章I, § 8, no. 5，定理1）具有重要的加法，当有问题的函数将其值穿着完整的豪斯多夫制服空间时。

#### 命题 11 {#top-ii-s3-prop-11 .statement tag=0BF6}

*令$A$为拓扑空间$X$的稠密子集，并令$f$为$A$的映射，形成完整的豪斯多夫均匀空间$X'$。那么$f$可以通过连续性扩展到$X$当且仅当，对于$f$下的每个$x \in X$，像在邻域滤波器的$A$上的轨迹$X$中的$x$是柯西滤波器基 $X'$。

这是通过连续性从扩张的定理得出的（前述），因为 $X'$ 是正则的（§ 1, no. 2，命题 3），并且因为 $X'$ 上的收敛滤波器与柯西滤波器相同。

当$X$也是均匀空间时，有如下定理：

#### 定理 2 {#top-ii-s3-thm-2 .statement tag=0BF7}

*令 $f$ 为函数，定义在一致空间 $X$ 的稠密子空间 $A$ 上，将其值取为完整的 Hausdorff 一致空间 $X'$，并假设 $f$ 一致连续$A$。那么$f$可以通过连续性扩展到整个$X$，且扩展后的函数$\overline{f}$一致连续。*

$\overline{f}$的存在性是命题3的直接的推论和no. 1的11个。让我们证明 $\overline{f}$ 是一致连续的。令$V'$为$X'$的闭对称周边，并令$V$为$X$的周边，这样，当$x$和$y$在$A$中并且$V$闭时，则$f(x)$和$f(y)$ 与 $V'$ 接近。我们可以假设$V$是$A$的随行人员$W$在$X \times X$的闭包（$\S$2，no. 4，命题6）。当 $(x, y) \in W$ 时，我们有 $[ \bar{f}(x), \bar{f}(y) ] \in V'$；由于 $\bar{f} \times \bar{f}$ 在 $X \times X$ 中连续（章 I、$\S$ 4、no. 1、命题 1），当 $(x, y) \in V = \overline{W}$ 时，我们也有 $[ \bar{f}(x), \bar{f}(y) ] \in V'$，因为 $V'$ 是封闭的（章I、$\S$2、no. 1、定理1）。

Q.E.D.

#### 推论 {#top-ii-s3-n6-cor-1 .statement tag=0BF8}

*设$X_1, X_2$为两个完整的豪斯多夫均匀空间，并令$Y_1, Y_2$分别为$X_1, X_2$的稠密子空间。然后每$Y_1$的同构$f$到$Y_2$扩展到$X_1$的同构到$X_2$。*

$f$ 在 $Y_1$ 中均匀连续，因而 (定理 2) 扩展到均匀连续映射 $\bar{f} : X_1 \to X_2$。同样，$f$扩展的逆$g$到均匀连续的映射$\bar{g} : X_2 \to X_1$。因而，函数$\bar{g} \circ \bar{f}$是$X_1$自身的连续映射，其限制到$Y_1$是恒等映射；通过扩张的原理恒等式（章 I、$\S$ 8、no. 1、推论 1 到命题 2），$\bar{g} \circ \bar{f}$ 因此是 $X_1$ 的恒等映射；类似地，$\bar{f} \circ \bar{g}$是$X_2$的恒等式映射。因而 (*集合理论*, R, $\S$ 2, no. 12) $\bar{f}^{-1}$ 和 $\bar{g}$ 是双射并且互为倒数；它们也是一致连续的，因此是同构 ($\S$ 2, no. 1, 命题 2)。

应该注意的是，如果$f$是$Y_1$在$Y_2$上的*双射的*一致连续映射，则其连续性的扩张*不需要既不是单射也不是满射*（习题 3）。

### 7. 制服的完成空间

#### 定理 3 {#top-ii-s3-thm-3 .statement tag=0BF9}

*令$X$为制服空间。那么存在一个完整的豪斯多夫均匀空间$\hat{X}$和一个均匀连续的映射$i : X \to \hat{X}$，具有以下性质：*

(P) *将 $X$ 的任何均匀连续映射 $f$ 赋予完整的 Hausdorff 均匀空间 $Y$，则存在唯一的均匀连续映射 $g : \hat{X} \to Y$，使得 $f = g \circ i$。*

*如果$(i_1, X_1)$是完整Hausdorff均匀空间$X_1$的另一个对由……组成和具有性质（P）的均匀连续映射$i_1 : X \to X_1$，则有唯一同构$\varphi : \hat{X} \to X_1$使得$i_1 = \varphi \circ i$。*

定理的第一个叙述表示对$(i, \hat{X})$是普遍映射问题的解（集合理论，章IV，， no. 1），其中$\Sigma$-集合是完全豪斯多夫均匀空间，$\sigma$-态射是均匀连续映射，$\alpha$-映射是$X$均匀连续映射成完全豪斯多夫均匀空间。因而，从对 $(i, \hat{X})$ 到唯一的同构的唯一性可以从普遍映射问题的解的一般属性得出（前述）。还需要证明对$(i, \hat{X})$的存在

1) 定义 / $\hat{X}$。令 $\hat{X}$ 为 $X$ 上的最小柯西滤波器 (no. 2) 的集合。我们将在$\hat{X}$穿定义制服结构。为此，如果$V$是$X$的任何对称周边，则让$\tilde{V}$表示所有对$(\mathscr{K}, \mathfrak{Y})$最小柯西滤波器的集合，这些滤波器在公共的中具有$V$小集合。我们将证明集合 $\tilde{V}$ 形式 $\hat{X}$ 上制服结构的基本随从人员系统：

(i) 由于每个 $\mathscr{K} \in \hat{X}$ 都是柯西滤波器，因此对于 $X$ 的每个对称随行人员 $V$，我们有定义 $(\mathscr{K}, \mathscr{K}) \in \tilde{V}$；因此满足公理$(U'_1)$。

(ii) 如果$V$和$V'$是$X$的两个对称周边，则$W = V \cap V'$是对称周边，并且每个$W$小的集合也是$V$小和$V'$小；因此$\tilde{W} \subset \tilde{V} \cap \tilde{V}'$，证明$(B_1)$。

(iii) 集合 $\tilde{V}$ 与定义对称，因此满足 $(U''_1)$。

(iv) 给定 $X$ 的对称周边$V$，令$W$ 为对称周边$\tilde{V} \subset V$。考虑三个最小柯西滤波器$\mathscr{K}, \mathfrak{Y}, \mathfrak{B}$，使得$(\mathscr{K}, \mathfrak{Y}) \in \tilde{W}$和$(\mathfrak{Y}, \mathfrak{B}) \in \tilde{W}$；那么有两个$W$小集合$M, N$这样$M \in \mathscr{K} \cap \mathfrak{Y}$和$N \in \mathfrak{Y} \cap \mathfrak{B}$。由于 $M$ 和 $N$ 属于到 $\mathfrak{Y}$，$M \cap N$ 不为空，因此 (no. 1, 命题 1) $M \cup N$ 是 $\tilde{W}$-小，因此 $V$-小；从$M \cup N$属于到$\mathscr{K}$再到$\mathfrak{B}$，我们有$\tilde{W} \subset \tilde{V}$；因此$(U'''_1)$是满足的。

接下来我们证明制服空间 $\hat{X}$ 是 Hausdorff。令$\mathscr{K}, \mathfrak{Y}$为$X$上的两个最小柯西滤波器，使得$(\mathscr{K}, \mathfrak{Y}) \in \hat{X}$适用于$X$的所有对称随行人员$V$。紧接着是集合$M \cup N$，其中$M \in \mathscr{K}$和$N \in \mathfrak{Y}$、$\mathfrak{B}$过滤器的形式基比$\mathscr{K}$和$\mathfrak{Y}$更粗糙。现在$\mathfrak{B}$是一个柯西滤波器，因为对于$X$的每个对称周边$V$，对于$\mathscr{K}$和$\mathfrak{Y}$，都有假设一个$V$小集合$P$属于，并且因此属于至 $\mathfrak{B}$。通过最小柯西滤波器的定义，我们有$\mathscr{K} = \mathfrak{B} = \mathfrak{Y}$，这表明$\hat{X}$是Hausdorff。

2) $i$的定义； $X$的统一结构是$\hat{X}$的$i$之下的逆像。我们知道，对于$X$中$x$的每个$x \in X$邻域过滤器$\mathfrak{B}(x)$来说，都是最小柯西过滤器（no. 2，命题5，推论1）。所以我们定义$i(x) = \mathfrak{B}(x)$。设 $f = i \times i$；我们将证明，对于$X$的每个对称随行人员$V$，我们有$j^{-1}(\tilde{V}) \subset V \cup j^{-1}[(\tilde{V})^3]$，这将证明我们的断言（§ 2, no. 4）。现在，如果$[i(x), i(y)] \in \tilde{V}$，则有一个$V$小集合$M$，它是$x$和$y$中每一个的邻域，因此$(x, y) \in V$。相反，如果$(x, y) \in V$，则立即看出集合$V(x) \cup V(y)$比$V$小，并且是$x$和$y$中每一个的邻域。

3) $\hat{X}$是完备的，$i(X)$在$\hat{X}$中是稠密的。 点 $\mathfrak{X} \in X$ 邻域 $\tilde{V}(\mathfrak{X})$ 在 $i(X)$ 上的迹是所有 $i(x)$ 的集合，使得

$$
(\mathfrak{X}, i(x)) \in \tilde{V}.
$$

这个关系意味着$X$中有一个$x$的$V$-小邻域，其中属于到$\mathfrak{X}$，即$x$是$V$-小的内部点集合共 $\mathfrak{X}$。令$M$为$\mathfrak{X}$的所有$V$-小集合的内部的并；然后 $M$ 属于到 $\mathfrak{X}$（no. 2，命题 5，推论 4），根据上述内容，得出 $\tilde{V}(\mathfrak{X}) \cap i(X) = i(M)$。我们结论认为：

(i) $\tilde{V}(\mathfrak{X}) \cap i(X)$ 不为空，因此 $i(X)$ 在 $\hat{X}$ 中是稠密的。
(ii) $i(X)$ 属于上的$\tilde{V}(\mathfrak{X})$到$X$上的滤波器基$i(\mathfrak{X})$的踪迹；因此这个过滤器基在$\hat{X}$收敛到点$\mathfrak{X}$。

现在让 $\mathfrak{F}$ 成为 $i(X)$ 上的柯西滤波器；那么从上面的2)和no. 1的命题4，$\overline{i^1}(\mathfrak{F})$是$X$上的柯西滤波器$\mathfrak{G}$的基。令 $\mathfrak{X}$ 为比 $\mathfrak{G}$ 更粗糙的最小柯西滤波器（no. 2，命题 5）；那么$i(\mathfrak{X})$是$i(X)$（no. 1，命题3）上的柯西滤波器基，并且$\mathfrak{F} = i[\overline{i^1}(\mathfrak{F})]$比基是$i(\mathfrak{X})$的滤波器是更细。由于后者收敛于 $\hat{X}$，$\mathfrak{F}$ 也收敛，命题 9 of no. 4 因此表明 $\hat{X}$ 是完备的。

4) 性质(P)的验证。令 $f$ 为 $X$ 的一致连续映射成为完整的 Hausdorff 均匀空间 $Y$。让我们首先证明存在唯一一致连续的映射$g_0 : i(X) \to Y$使得$f = g_0 \circ i$。由于$f$是连续的，我们有

$$
f(x) = \lim f(\mathfrak{B}(x)),
$$

因此，如果我们输入$g_0(i(x)) = \lim f(\mathfrak{B}(x))$，我们就有$f = g_0 \circ i$；所以还需要证明$g_0$在$i(X)$中一致连续。令$U$为$Y$的周边，并令$V$为$X$的对称周边，使得关系$(x, x') \in V$蕴涵$(f(x), f(x')) \in U$；我们在 2) 中看到关系 $(i(x), i(x')) \in \tilde{V}$ 蕴含 $(x, x') \in V$，因此也蕴涵
$$
(g_0(i(x)), g_0(i(x'))) \in U,
$$
这证明了我们的断言。

通过连续到 $\hat{X}$ (no. 6, 定理 2)，令$g$为$g_0$的扩张；那么$f = g \circ i$，很明显，$g$是$\hat{X}$到$Y$满足这个关系的唯一连续映射，因为$i(X)$在$\hat{X}$中是稠密的（章） I, § 8, no. 1，命题 2，推论 1)。

Q.E.D.

#### 定义 4 {#top-ii-s3-def-4 .statement tag=0BFA}

*完成Hausdorff一致空间*$\hat{X}$*定义在定理3的证明称为*$X$的Hausdorff完成，*和映射*$i : X \to \hat{X}$*称为*$X$*的典范映射成它的豪斯多夫完成。*

我们注还有以下事实：

#### 命题 12 {#top-ii-s3-prop-12 .statement tag=0BFB}

(i) *The subspace* $i(X)$ *is dense in* $\hat{X}$.
(ii) *The graph of the equivalence relation* $i(x) = i(x')$ *is the intersection of the entourages of* $X$.
(iii) *The uniform structure of* $X$ *is the inverse image under* $i$ *of that of* $\hat{X}$ *[or of that of the subspace* $i(X)$].
(iv) *The entourages of* $i(X)$ *are the images under* $i \times i$ *of the entourages of* $X$, *and the closures in* $\hat{X} \times \hat{X}$ *of the entourages of* $i(X)$ *form a fundamental system of entourages of* $\hat{X}$.

(i)和(iii)已在定理3的证明过程中得到证明；凭借先前证明的一般结果（§ 2, no. 4、注和命题 6），(iv) 是 (i) 和 (iii) 的推论。 关系
$$
i(x) = i(x')
$$
定义表示 $x$ 和 $x'$ 具有相同的邻域过滤器。但这意味着，通过定义，$(x, x') \in V$对于$X$的每个随行人员$V$，并且逆命题是显而易见的。

#### 推论{#top-ii-s3-n7-cor-1 .statement tag=0BFC}

*如果* $X$ *是豪斯多夫均匀空间，则典范映射* $i : X \to \hat{X}$ *是* $X$ 的同构 *到* $\hat{X}$ 的密集子空间。

当$X$是Hausdorff时，$\hat{X}$被认为是$X$的*完备的*，并且我们通常通过$i$*认同*$X$与$\hat{X}$的稠密子集。

#### 注 {#top-ii-s3-n7-rem-1 .statement tag=0BFD}

如果这样识别，X上的最小柯西滤波器就是$\hat{X}$的点的邻域滤波器在X上的迹；这是从定理 3 的证明得出的。

命题 12 的推论描述了 Hausdorff 制服空间的完成：

#### 命题 13 {#top-ii-s3-prop-13 .statement tag=0BFE}

*如果Y是完整的豪斯多夫均匀空间和XY的稠密子空间，则典范嵌入$X \to Y$扩展到同构$\hat{X}$到Y上。*

对于X的每个均匀连续映射到完整的Hausdorff均匀空间Z扩展，唯一到Y的均匀连续映射通过no. 6的定理2到Z。

#### 命题 14 {#top-ii-s3-prop-14 .statement tag=0BFF}

*令X为完整的豪斯多夫均匀空间，$\mathfrak{U}$其均匀性，并令Z为X的稠密子空间。如果 $\mathfrak{U}'$ 是 X 上的均匀性，比 $\mathfrak{U}$ 更粗糙，并且诱导与 Z 上的 $\mathfrak{U}$ 具有相同的均匀性，则 $\mathfrak{U} = \mathfrak{U}'$。*

让X'表示集合X，均匀度为$\mathfrak{U}'$。 典范映射$X' \to \hat{X}'$和恒等映射$X \to X'$的合成是均匀连续的映射$\varphi : X \to \hat{X}'$。由于对于$\mathfrak{U}'$诱导的均匀结构，Z是Hausdorff，因此$\varphi$到Z的限制是通过Z的假设同构到$\hat{X}'$的稠密子空间$\varphi(Z)$； （no. 6，定理 2 的推论）$\varphi$ 本身是X 的同构到$\hat{X}'$，因此$X' = \hat{X}'$ 和$\mathfrak{U}' = \mathfrak{U}$。

#### 命题 15 {#top-ii-s3-prop-15 .statement tag=0BFG}

*令X和X'为两个统一的空间。对于每个均匀连续映射$f : X \to X'$，都有一个唯一的均匀连续映射$\hat{f} : \hat{X} \to \hat{X}'$，使得图表

$$
\begin{array}{ccc}
X & \xrightarrow{i'} & X' \\
i \downarrow & & \downarrow i' \\
\hat{X} & \xrightarrow{\hat{f}} & \hat{X}'
\end{array}
$$

是可交换的 (*)，其中 $i : X \to \hat{X}$ 和 $i' : X' \to \hat{X}'$ 是典范映射。

应用定理 3 至函数 $i' \circ f : X \to \hat{X}'$。

#### 推论{#top-ii-s3-n7-cor-2 .statement tag=0BFH}

*如果$f : X \to X'$和$g : X' \to X''$是两个均匀连续的映射和$h = g \circ f$，则$\hat{h} = \hat{g} \circ \hat{f}$。*

这是命题 15 中唯一性的直接的推论。

(*) 其他字、$i' \circ f = \hat{f} \circ i$。

### 8. HAUSDORFF 制服空间与制服空间相关

#### 命题 16 {#top-ii-s3-prop-16 .statement tag=0BFI}

令$X$为$X$的一致空间和$i$典范映射进入其Hausdorff完成$\hat{X}$。对于 $X$ 的每个均匀连续映射 $f$ 到 Hausdorff 均匀空间 $Y$，有一个唯一的均匀连续映射 $h : i(X) \to Y$，使得 $f = h \circ i$。

我们可以将认同 $Y$ 与子空间完成 $\hat{Y}$（no. 7，命题 12 的推论），然后 $f$ 可以被认为是 $X$ 的均匀连续映射到$\hat{Y}$。凭借定理 3，$f$ 就是形式 $f = g \circ i$，其中$g$ 是$\hat{X}$ 到$\hat{Y}$ 的均匀连续的映射。如果$h$是$g$到$i(X)$的限制，那么显然是$f = h \circ i$，并且$h$映射$i(X)$变成$Y$。 $h$的唯一性是微不足道的。

因此，对$(i, i(X))$是普遍映射问题的解（集合理论，章IV, § 3, no. 1），这次我们将$\Sigma$集合视为Hausdorff均匀集空间，并且$\sigma$-态射（或$\alpha$-映射）均匀连续映射（或$X$的均匀连续映射到Hausdorff均匀空间）。

#### 定义 5 {#top-ii-s3-def-5 .statement tag=0BFJ}

在定理 3 的证明中定义的豪斯多夫制服空间 $i(X)$ 称为与 $X$ 关联的豪斯多夫制服空间。

因此，$X$ 的豪斯多夫完备性是与 $X$ 相关的豪斯多夫制服空间的完备性。

#### 推论{#top-ii-s3-n8-cor-1 .statement tag=0BFK}

令 $X, Y$ 为两个一致的空间和 $X', Y'$ 伴随的 Hausdorff 空间。对于每个均匀连续映射$f : X \to Y$，都有一个唯一的均匀连续映射$f' : X' \to Y'$，其中图表

$$
\begin{array}{ccc}
X & \xrightarrow{f} & Y \\
i \downarrow & & \downarrow i' \\
X' & \xrightarrow{f'} & Y'
\end{array}
$$

是可交换的，其中 $i$ 和 $i'$ 是典范映射。

应用命题 16 至 $i' \circ f : X \to Y'$。

与制服空间相关的 Hausdorff 空间也可以用以下性质来表征：

#### 命题 17 {#top-ii-s3-prop-17 .statement tag=0BFL}

令$X$为均匀空间，$i(X)$其关联的豪斯多夫空间，并令$f$为$X$的映射到豪斯多夫均匀空间$X'$，这样的均匀性$X$在$X'$均匀度的$f$下是逆像。然后映射$g : i(X) \to X'$使得$f = g \circ i$是同构。

到命题 16 时，$g$ 均匀连续；而且 $g$ 显然是满射，并且也是单射，因为关系 $f(x) = f(y)$ 通过定义暗示 $(x, y)$ 属于到 $X$ 的所有随从，因此 $i(x) = i(y)$ (no. 7, 命题 12）。最后，$X'$的随从是$X$随从的$f \times f$之下像（$§ 2$、no. 4、注），因此他们也是$i(X)$的随从的$g \times g$之下像 （no. 7，命题12）；因此结果。

#### 注 {#top-ii-s3-n8-rem-1 .statement tag=0BFM}

令 $R$ 为 $X$ 上的等价关系 $i(x) = i(x')$。我们已经看到（no. 7，命题12），$R$的图$C$是$X$所有随从的交。很明显，$X$中的每个开集合（因此也是每个闭集合）相对于$R$来说是“饱和”的；考虑到拓扑的逆像的定义，我们结论认为由$i$引发的空间$X/R$到$i(X)$的商的规范双射是一个*同胚*。因此，与 $X$ 相关的 Hausdorff 空间可以被识别为，*qua* 拓扑空间与 $X/R$。 典范映射 $i : X \to i(X)$ 是开闭的，甚至是适当的（章 I、$§ 10$、no. 2、例）。

令$X'$为另一个统一空间，$X'$所有随从的$C'$交，以及$R'$等价关系，其图为$C'$。令 $f : X \to X'$ 为*连续* 映射。由于$f(x)$的任意邻域的$f$下的逆像是$x$的邻域，因此$C'(f(x))$包含$C(x)$的$f$下的逆像，因此$f$ 与 $R$ 和 $R'$ *相容的*，并且诱导是连续的映射 $X/R \to X'/R'$（章 I、$§ 3$、no. 4，命题的推论） 6).这将推论推广到命题 16。

### 9. 完成子空间和乘积空间

#### 命题 18 {#top-ii-s3-prop-18 .statement tag=0BFN}

*令$X$为集合，让$(Y_\lambda)_{\lambda \in L}$为制服空间的族，对于每个$\lambda \in L$，让$f_\lambda$为$X$到$Y_\lambda$的映射。让$X$带有最粗糙的均匀性$U$，这使得所有$f_\lambda$均匀连续。那么$X$的Hausdorff完成$\hat{X}$的均匀性是最粗糙的，其中所有映射$\hat{f}_\lambda : \hat{X} \to \hat{Y}_\lambda$（$\lambda \in L$）（no. 7，命题15）都是一致连续的。此外，如果$j_\lambda$是$Y_\lambda$的典范映射进入$\hat{Y}_\lambda$，并且如果$g_\lambda = j_\lambda \circ f_\lambda$，则$\hat{X}$可以被识别为映射下的$X$的像的$\prod_{\lambda \in L} \hat{Y}_\lambda$中的闭包$x \to (g_\lambda(x))$.*

令$X'$（分别$Y'_\lambda$）为与$X$（分别$Y_\lambda$）关联的豪斯多夫均匀空间，并令$f'_\lambda : X' \to Y'_\lambda$为均匀连续的映射，这使得图表

$$
\begin{array}{ccc}
X & \xrightarrow{f_\lambda} & Y_\lambda \\
i \downarrow & & \downarrow j_\lambda \\
X' & \xrightarrow{f'_\lambda} & Y'_\lambda
\end{array}
$$

可交换（*i* 为典范映射）。

初始均匀度（§ 2, no. 3，命题 5）的传递性一方面表明$\mathfrak{U}$是最粗糙的均匀度，其中映射$j_\lambda \circ f_\lambda : X \to Y'_\lambda$均匀连续，另一方面$\mathfrak{U}$在$i$下也是逆像集合 $X'$ 上最粗糙的均匀性$\mathfrak{U}'$，其中$f'_\lambda$ 是均匀连续的。现在$\mathfrak{U}'$是*Hausdorff*，因为如果$x_1, x_2$是$X$的两个点，那么$j_\lambda(f_\lambda(x_1)) = j_\lambda(f_\lambda(x_2))$对应于每个$\lambda \in L$，那么$(x_1, x_2)$属于对应于$\mathfrak{U}$的所有随从，因此$i(x_1) = i(x_2)$。因此，no. 8的命题 17表明$\mathfrak{U}'$是与$X$相关的豪斯多夫空间$X'$的均匀性。

既然如此，双射$x' \to (f'_\lambda(x'))$将$X$与统一的子空间标识为乘积$\prod_\lambda Y'_\lambda$（§ 2, no. 6，命题8）。由于$Y'_\lambda$是Hausdorff，每个$Y'_\lambda$可以用其完成$\hat{Y}_\lambda$的密集子空间来识别，因此$\prod_\lambda Y'_\lambda$可以用$\prod_\lambda \hat{Y}_\lambda$的密集子空间来识别（章I, § 4, no. 3，命题） 7).但$\prod_\lambda \hat{Y}_\lambda$是豪斯多夫且完备的（no. 5，命题10）；因此$\prod_\lambda \hat{Y}_\lambda$中$X'$的闭包$\overline{X'}$是一个完整的Hausdorff子空间（no. 4，命题8），可以用$X$的Hausdorff完成$\hat{X}$来识别；在此证明下，映射$\hat{f}_\lambda$变为投影到因子$\hat{Y}_\lambda$，并且命题被证明。

#### 推论 1 {#top-ii-s3-prop-18-cor-1 .statement tag=0BFO}

*令$X$为均匀空间，并让$i$为$X$的典范映射进入其Hausdorff完成$\hat{X}$；设$A$为$X$和$j : A \to X$典范嵌入中的子空间。那么$\hat{j} : \hat{A} \to \hat{X}$是$\hat{A}$的同构到$\hat{X}$中$i(A)$的闭包上。*

#### 推论 2 {#top-ii-s3-prop-18-cor-2 .statement tag=0BFP}

*令$(Y_\lambda)_{\lambda \in L}$为制服空间的家族。那么乘积空间 $\prod_{\lambda \in L} Y_\lambda$ 的 Hausdorff 补全与乘积 $\prod_{\lambda \in L} \hat{Y}_\lambda$ 自然同构。*

### 习题 {#top-ii-s3-exercises}

§ 3](exercises/s3/)参见[习题。
