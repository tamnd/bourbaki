---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 3
section_title: Subspaces, quotient spaces
lang: zh
source: top-i-iv
book_pages: 35-43, 122-125
pdf_pages: 0041-0049, 0128-0131
extraction: ocr
subsections:
    - "no": 1
      title: SUBSPACES OF A TOPOLOGICAL SPACE
      page: 35
      pdf_page: 41
    - "no": 2
      title: CONTINUITY WITH RESPECT TO A SUBSPACE
      page: 37
      pdf_page: 43
    - "no": 3
      title: LOCALLY CLOSED SUBSPACES
      page: 38
      pdf_page: 44
    - "no": 4
      title: QUOTIENT SPACES
      page: 39
      pdf_page: 45
    - "no": 5
      title: CANONICAL DECOMPOSITION OF A CONTINUOUS MAPPING
      page: 40
      pdf_page: 46
    - "no": 6
      title: QUOTIENT SPACE OF A SUBSPACE
      page: 42
      pdf_page: 48
statements: 24
exercises: 16
content_sha256: dd7c5276a1d204abaa9d254a75d36fd046a2818e5cff0818330a8fceadb5984e
translated_from: content/en/top/I/03_s3_subspaces_quotient_spaces.md
translation_method: google
source_content_sha256: 49505713ae8eafd390ab9e7460fda1c5af09d0a5526d97705cb0bdc2a371a4da
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: a6413408ab87a315e27b616ad9c8e25963be4a5aaa96f5c3f737404275ee7bf1
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 3. 子空间； 商空间

### 1. 拓扑空间的子空间

设$A$为拓扑空间$X$的子集。我们将$X$的拓扑在$A$上的*拓扑诱导*定义为后者在典范嵌入$A \to X$下的逆像（§ 2, no. 3，例1）。等效的定义如下：

#### 定义 1 {#top-i-s3-def-1 .statement tag=0B13}

设$A$为拓扑空间$X$的子集。 $X$的拓扑在$A$上诱导拓扑是其中集合的开交和$X$的开集合的$A$。 集合$A$与此拓扑称为$X$的子空间。

#### 例 {#top-i-s3-n1-exa-1 .statement tag=0B14}

有理线拓扑在有理整数的集合$\mathbf{Z}$上感应拓扑是离散的拓扑，对于$\mathbf{Z}$的交且开区间$]n - 1/2, n + 1/2[$是集合 $\{ n \}$。

通过§ 2, no. 3的命题 5（或直接从定义 1）我们看到，如果$B \subset A \subset X$，$X$的子空间$B$与子空间$A$的子空间$B$相同$X$（诱导拓扑的传递性）。如果 $\mathfrak{G}$ 是 $X$ ($§ 2$, no. 3, 例 3) 的拓扑的子底（分别为基），则 $A$ 上的踪迹 $\mathfrak{G}_A$ 是以下子底（分别为基） 拓扑于$A$诱发。

在所有涉及$A$的元素或子集的问题中，必须仔细区分它们作为$X$的点（分别为子集）的属性，以及它们作为子空间$A$的点（分别为子集）的属性。 我们将通过使用短语“在$A$中”、“相对于$A$”或“相对于$A$”来表示后一类中的属性（可能与短语“在$X$中”、“相对于$X$”、“相对于$X$”进行对比）来进行区分。

子空间 $A$ 的开集合不必在 $X$ 中开；在阶中，在$A$中打开的每个集合应该在$X$中打开，$A$在$X$中打开是必要且充分的。 条件是必要的，因为$A$在$A$中是开放的，并且凭借$(O_{II})$和定义1就足够了。

在$A$关闭的集合是交，以及在$X$关闭的集合的$A$（$§ 2$，no. 3，例1）；如上所述，我们看到每个在$A$中闭合的集合在$X$中闭合当且仅当$A$在$X$中闭合。

点 $x \in A$相对于$A$的邻域相对于交，以及$x$的邻域相对于$X$的$A$。 $x$相对于$A$的每个邻域是$x$相对于$X$的邻域，当且仅当$A$是$X$中$x$的邻域。

#### 命题 1 {#top-i-s3-prop-1 .statement tag=0B15}

如果$A$和$B$是拓扑空间$X$的两个子集和$B \subset A$，则子空间$A$中的$B$闭包是交和$A$闭包$X$ 中的$B$ $\overline{B}$。

如果$x \in A$，则$A$中$x$的每个邻域都是形式$V \cap A$，其中$V$是$X$中$x$的邻域。从$V \cap B = (V \cap A) \cap B$开始，当且仅当$x$位于$B$关于$X$的闭包时，$x$位于$B$相对于$A$的闭包。

#### 推论 {#top-i-s3-n1-cor-1 .statement tag=0B16}

$A$的子集$B$在$A$中是稠密的当且仅当$\overline{B} = \overline{A}$在$X$中（即当且仅当$A \subset \overline{B}$）。

由此可知，如果 $A, B, C$ 是 $X$ 的三个子集，使得 $A \supset B \supset C$，并且如果 $B$ 在 $A$ 中稠密，并且 $C$ 在 $B$ 中稠密，则 $C$ 在 $A$ 中稠密 (*传递性* 密度），因为$X$中有$\overline{A} = \overline{B} = \overline{C}$。

#### 命题 2 {#top-i-s3-prop-2 .statement tag=0B17}

*设$A$为拓扑空间$X$的稠密子集；那么对于$x$相对于$A$的每个$x \in A$和每个邻域$V$，$X$中$V$的闭包$\overline{V}$是$X$中$x$的邻域。*

对于$V$包含$U \cap A$，其中$U$是$X$的开子集，其中包含$x$，因此$\overline{V}$包含$U \cap \overline{A} = U$（§ 1, no. 6， 命题5)。

#### 命题 3 {#top-i-s3-prop-3 .statement tag=0B18}

*令$(A_i)_{i \in I}$为拓扑空间$X$的子集族，使得以下性质成立之一：
a) $A_i$ 盖$X$ 的内部。
b) $(A_i)_{i \in I}$ 是$X$ (§ 1, no. 5) 的局部有限闭覆盖。*

*在这些条件下，$X$的子集$B$在$X$中打开（或关闭）当且仅当每个集合$B \cap A_i$在$A_i$中打开（或关闭）。*

显然，如果 $B$ 在 $X$ 中开（或闭），则 $B \cap A_i$ 在 $A_i$ 中开（或闭）。反之，首先假设满足条件a)；由于$(\complement B) \cap A_i = A_i - (B \cap A_i)$，根据对偶性，考虑每个$B \cap A_i$相对于$A_i$都是“开”的情况就足够了。在这种情况下，对于每个$i \in I$，$B \cap \dot{A}_i$在$\dot{A}_i$中开，因此在$X$中开；从$B = \bigcup_i (B \cap \dot{A}_i)$到假设，$B$在$X$开放。

现在假设 b) 得到满足；再次通过对偶性，我们只需要考虑每个$B \cap A_i$在$A_i$中“闭合”，因此在$X$中闭合的情况。由于族$(B \cap A_i)$是局部有限的并且$B = \bigcup_i (B \cap A_i)$，因此从§ 1, no. 5，命题4可以得出$B$在$X$中是封闭的。

#### 注 {#top-i-s3-n1-rem-1 .statement tag=0B19}

令$(U_i)_{i \in I}$为拓扑空间$X$的*开放*覆盖，对于每个$i \in I$，令$\mathfrak{B}_i$为子空间$U_i$的拓扑的*基*，$X$；那么很明显$\mathfrak{B} = \bigcup_{i \in I} \mathfrak{B}_i$是$X$的拓扑的*基*。

### 2. 子空间的连续性

令$X$和$Y$为两个拓扑空间，$f$为$X$到$Y$的映射，$B$为$Y$的子集，其中包含$f(X)$。 诱导的拓扑的定义作为初始拓扑（§ 2, no. 3，命题4）表明$f$在$x \in X$连续当且仅当$X$的映射进入*子空间*$B$ $Y$与$f$具有相同的图，在$x$处连续。

现在让$A$是$X$的子集；如果$f$在$x \in A$连续（分别在$X$上连续），则其限制$f|A$是子空间$A$到$Y$的映射，根据§ 2, no. 1的命题2，它在$x$连续（分别在$A$上连续）。 我们有时会说，如果映射$f|A$在$x$连续（或在$A$连续），则映射$f : X \to Y$在$x \in A$**相对于$A$连续（相对于$A$*连续）。

需要注意的是，在$X$的任意一个点处，$f|A$可以连续而不需要$f$连续；这种现象的例是由$X$的子集$A$的特征函数$\varphi_A$提供的，$A$及其补集在$X$中都是稠密的（$§ 2$，习题11），将$\varphi_A$视为$X$的映射转化为离散的空间$\{0, 1\}$。 $\varphi_A$在$X$的任意一个点都不连续，但它的限制到$A$是常数，因此是连续的。

如果$A$在点$x \in A$的$X$中为邻域，并且如果$f : X \to Y$使得$f|A$在$x$连续，则$f$在$x$连续；对于$A$中$x$的每个邻域是$X$中$x$的邻域（*局部*连续性特征标）。

#### 命题 4 {#top-i-s3-prop-4 .statement tag=0B1A}

*设* $(A_i)_{i \in I}$ *是拓扑空间* $X$ *其内部覆盖* $X$的子集族，*或者是* $X$的局部有限封闭覆盖。 *让*$f$*成为*$X$*的映射*进入拓扑空间*$X'$。 *如果* $f$ *中的限制 *对每个子空间* $A_i$ *是连续的，则* $f$ *是连续的。*

因为如果$F'$是$X'$的闭子集并且如果$F = \overline{f}(F')$，那么对于每个$i \in I$（$§ 2$，no. 1，定理1），$F \cap A_i$在$A_i$中是闭的，因此$F$于$X$截止至命题 3 / no. 1；现在的结果来自定理 1 of $§ 2$, no. 1。

### 3. 本地关闭子空间

#### 定义 2 {#top-i-s3-def-2 .statement tag=0B1B}

*子集* $L$ *拓扑空间* $X$ *据说在点* $x \in L$ *如果存在邻域* $V$ *of* $x$ *in* $X$ *使得*$L \cap V$*是子空间*$V$的闭子集。 *L 据说在* $X$ 局部闭合 *如果它在每个* $x \in L$ 局部闭合。

#### 注 {#top-i-s3-n3-rem-1 .statement tag=0B1C}

令 $F$ 为 $X$ 的子集，使得*对于每个点* $x$ *of* $X$ *有邻域* $V$ *of* $x$ *使得* $V \cap F$ *闭于子空间*$V$； *然后从命题 3 of no. 1 得出* $F$ *在* $X$ 结束。 *另一方面，下面的命题5表明，一般情况下，存在局​​部封闭的集合，而在*$X$中并未封闭。

#### 命题 5 {#top-i-s3-prop-5 .statement tag=0B1D}

*对于子集* $L$ *拓扑空间* $X$，*以下属性是等效的*：

a) $L$ *在* $X$ 局部关闭。

b) $L$ 是开子集的交和$X$ 的闭子集。

c) $L$ 在 $X$ 中的闭包 $\overline{L}$ 中打开。

如果$L$是局部闭的，那么对于每个$x \in L$，$X$中存在$x$的开邻域$V_x$，使得$L \cap V_x$在$V_x$中闭； $U = \bigcup_{x \in L} V_x$在$X$打开，no. 1的命题 3表明$L$在$U$关闭；因此a) 意味着b)。如果$L = U \cap F$，其中$U$在$X$打开且$F$关闭，我们有$L \subset F$；因此$L \subset U \cap L \subset U \cap F = L$，这表明$L = U \cap L$在$L$中开，因此b）蕴含c）。最后，如果$L = U \cap L$，其中$U$在$X$中开，$L$在$U$中闭，因此是局部闭的，因此c）意味着a）。

#### 推论 {#top-i-s3-n3-cor-1 .statement tag=0B1E}

*设$f : X \to X'$为连续映射，$L'$为$X'$的局部闭子集；那么$f^{-1}(L')$在$X$*中局部闭。

这紧接着上面的命题 5 和§ 2, no. 1 的定理 1。

### 4. 商空间

#### 定义 3 {#top-i-s3-def-3 .statement tag=0B1F}

*令$X$为空间、$R$等价关系在$X$上。 $X$ 商空间 $R$ 是商集 $X/R$ 和拓扑 $X$ 拓扑商关系 $R$ （§ 2, no. 4，例1）*。

除非恰恰相反，每当我们将$X/R$称为拓扑空间时，我们都可以理解为$R$是指$X$的商空间。我们经常说，这个拓扑空间是通过识别$X$的点而获得的空间，其中属于与相同的等价类模$R$。

令$\varphi$为典范映射$X \to X/R$。通过定义（§ 2, no. 4、命题 6 及其推论），$X/R$ 中的开（或闭）集合为集合 $A$，使得 $\varphi^{-1}(A)$ 开（或闭） $X$；在其他字中，$X/R$中的开路（或闭路）集合与$X$的开路（或闭路）子集是一对一的对应，它们相对于$R$饱和，并且是其中的典范像子集。

#### 命题 6 {#top-i-s3-prop-6 .statement tag=0B1G}

*设$X$为$X$的$X$、$\varphi$典范映射到$X/R$的拓扑空间、$R$等价关系；那么$X/R$的映射$f$到拓扑空间$Y$是连续的当且仅当$f \circ \varphi$在$X$*上连续。

这是§ 2, no. 4、命题 6 的特例；它表达了这样一个事实：商拓扑是映射$\varphi$的最终拓扑。

命题 6 表明$X/R$到$Y$的连续映射和$X$到$Y$的连续映射之间存在一对一的对应 *在每个等价类模上都是恒定的$R$*。

#### 例 {#top-i-s3-n4-exa-1 .statement tag=0B1H}

*考虑等价关系$x \equiv y \pmod{1}$对实直线$\mathbf{R}$； $\mathbf{R}$的商空间由此关系称为*一维环面*并用$T$表示。 点 $x \in \mathbf{R}$的等价类由所有点$x + n$组成，其中$n$贯穿有理数整数的集合$\mathbf{Z}$。到命题 6，$T$上的连续函数和$\mathbf{R}$上的连续函数之间存在一对一的对应，它们是周期为1的“周期性”。我们将在章中回到这个重要的例 V, § 1.*

#### 推论 {#top-i-s3-n4-cor-1 .statement tag=0B1I}

*设$X, Y$为$X$（或$Y$）上的两个拓扑空间、$R$（或$S$）等价关系，并令$f : X \to Y$为连续的映射，与等价关系$R$和$S$（集合理论R，§ 5, no. 8）；那么由 $f$ (集合理论 R, § 5, no. 8) 诱导的映射 $g : X/R \to Y/S$ 是连续的。*

这是一般性质商结构（集合理论、章 IV, § 2, no. 6，标准 CST 20）的特殊情况。

#### 命题 7（商空间中的传递性）{#top-i-s3-prop-7 .statement tag=0B1J}

*令$R$和$S$为拓扑空间$X$上的两个等价关系，使得$R$蕴含$S$，并令$S/R$为商等价关系商空间$X/R$（集合理论R，§ 5, no. 9）。那么规范的双射 $(X/R)/(S/R) \to X/S$ 是同胚。*

这是最终拓扑传递性的特例（§ 2, no. 4、命题7。参见集合理论、章IV, § 2, no. 3，标准 CST 21）。

### 5. 连续映射的规范分解

令$X$和$Y$为两个拓扑空间，$f : X \to Y$在$X$上连续的映射，$R$等价关系$f(x) = f(y)$。考虑*规范的分解*

$$
f : X \xrightarrow{\varphi} X/R \xrightarrow{g} f(X) \xrightarrow{\psi} Y
$$

其中$\varphi$是$X$到商空间$X/R$的规范（满射）映射，$\psi$是子空间$f(X)$到$Y$的典范嵌入，并且$g$ 是双射与$f$ (集合理论 R, § 5, no. 3) 相关。立即可见$g$是连续的（通过no. 4的命题6）；这也是商结构上一般结果的特例。 （参见集合理论、章IV, § 2, no. 6）。但双射 $g$ *不一定是同胚*。

#### 命题 8 {#top-i-s3-prop-8 .statement tag=0B1K}

令$f = \psi \circ g \circ \varphi$为连续映射$f : X \to Y$的规范分解，并令$R$表示等价关系
$$
f(x) = f(y).
$$
那么下面三个条件是等价的：
a) $g$ 是$X/R$ 到$f(X)$ 的同胚。
b) 相对于$R$饱和的每个开路集合的$f$下的像是子空间$f(X)$中的开路集合。
c) 每个相对于$R$饱和的闭集合在$f$下的像是子空间$f(X)$中的闭集合。

对于条件 b) [分别。 c)]表示$X/R$中每个开（或闭）集合的$g$下的像是$f(X)$中的开（或闭）集合。

#### 例 {#top-i-s3-n5-exa-1 .statement tag=0B1L}

设$X$是拓扑空间，$(X_i)_{i \in I}$是$X$的覆盖，$Y$和对子空间$X_i$对$X$的覆盖；那么$Y$有划分$(Y_i)_{i \in I}$进入子空间，它们都是开闭的，并且对于每个$i \in I$都有一个同胚$f_i : Y_i \to X_i$。令$f : Y \to X$为每个$i \in I$在$Y_i$上与$f_i$一致的连续映射，并令$R$为等价关系$f(x) = f(y)$；因此，商空间$Y/R$是通过将$Y_i$（§ 2, no. 5）“粘贴在一起”获得的。考虑双射$g : Y/R \to X$与$f$相关；一般来说，$g$不是同胚，如例所示，其中每个$X_i$由单个点组成，而$X$不是离散的。然而，如果$X_i$的内部覆盖$X$，或者如果$(X_i)$是$X$的局部有限闭覆盖，那么$g$是同胚：因为如果$U$是$Y$的任何开子集，并且相对于饱和$R$，然后对于每个 $i \in I$ 集合
$$
f(U) \cap X_i = f_i(U \cap Y_i)
$$
$X_i$开放，断言从no. 1的命题3开始。

下面的命题给出了一个简单的足够的条件，使$g$成为同胚：

#### 命题 9 {#top-i-s3-prop-9 .statement tag=0B1M}

令$f : X \to Y$为连续射影，令$R$表示等价关系$f(x) = f(y)$。如果存在与$f$关联的连续截面$s : Y \to X$（集合理论、章II, § 3, no. 8、定义11），则与$f$关联的映射$g : X/R \to Y$是同态，$s$是$Y$到$X$的子空间$s(Y)$的同态。

因为如果$\varphi : X \to X/R$是典范映射，那么$g$和$\varphi \circ s$是双射、连续且互逆；同样，$f$到$s(Y)$的$s$和限制是双射、连续且互逆的。

如果在拓扑空间 $X$ 上$R$ 是等价关系并且
$$
\varphi : X \to X/R
$$
是典范映射，与$\varphi$相关的*连续截面*$s : X/R \to X$也称为$X$的*连续截面*相对于$R$（cf.*集合理论*， 章II, § 6, no. 2）；那么$X$的子空间$s(X/R)$同胚于$X/R$。如果给定$s(X/R)$，则$s$是唯一确定的； $s(X/R)$ 通常被滥用语言称为 $X$ 相对于 $R$ 的（连续）*截面*。

拓扑空间相对于等价关系的连续截面不一定存在 (习题 12)。

### 6. 商空间共子空间

令$X$为$X$、$R$等价关系在$X$、$f$规范映射$X \to X/R$上的拓扑空间、$A$子空间， $g$限制共$f$至$A$。 $A$上的等价关系$g(x) = g(y)$只是由$A$上的$R$*诱发*的关系$R_A$（*集合理论*R，§ 5, no. 5）。令 $g = \psi \circ h \circ \varphi$ 为 $g$ 的规范分解，这样，如果 $j$ 是 $A$ 的典范嵌入到 $X$，我们就有一个可交换的图表 (*)

$$
\begin{array}{ccc}
A & \xrightarrow{\varphi} & A/R_A \xrightarrow{h} f(A) \xrightarrow{\psi} X/R. \\
& & \\
& \searrow_j & \nearrow_s \\
& & X
\end{array}
$$

#### 命题 10 {#top-i-s3-prop-10 .statement tag=0B1N}

*规范双射* $h : A/R_A \to f(A)$ *是连续的*。 *此外，以下三个叙述是等价的*：

a) $h$ *是同胚*。

b) * * $A$ * 的每个开路子集 * 相对于 * $R_A$ * 是交和 * $A$ * 的开路子集 * $X$ * 相对于* $R$ 饱和。

c) * * $A$ * 的每个闭子集 * 相对于 * $R_A$ * 是交和 * $A$ * 的闭子集的 * $X$ * 相对于 * $R$ 饱和。

命题的第一个部分是直接的 (no. 5)。第二个部分源自no. 5的命题8：如果$B$是$A$的开（或闭）子集，相对于$R_A$饱和，并且$g(B) = f(B)$是交， $f(A)$ 开（或闭）子集 $C$ 或 $X/R$，则 $B$ 为交，$A$ 开（或闭）子集 $f^{-1}(C)$

(*) 该表达式的意思是 $f \circ j = \psi \circ h \circ \varphi$。

X，其相对于 R 是饱和的；相反，如果 B 是交，A 是开（或闭）子集 D，且相对于 R 饱和，则 $f(B)$ 是 $f(A)$ 和 $f(D)$ 的交，其在 $X/R$ 中开（或闭）。

#### 推论 1 {#top-i-s3-prop-10-cor-1 .statement tag=0B1O}

*如果 A 是 X 的开（或闭）子集，且相对于 R 饱和，则典范映射 $h : A/R_A \to f(A)$ 是同胚。*

如果 A 在 X 中开路（或闭路）且相对于 R 饱和，且如果 $B \subset A$ 在 A 中开路（或闭路）且相对于 $R_A$ 饱和，则 B 在 X 中开路（或闭路）且相对于 R 饱和。

#### 推论 2 {#top-i-s3-prop-10-cor-2 .statement tag=0B1P}

*如果存在连续的映射$u : X \to A$，使得$u(x)$对于每个$x \in X$都与$x$ mod R一致，则$f(A) = X/R$和典范映射$h : A/R_A \to X/R$是同胚。*

由于每个等价类 mod R满足A，$X/R$中$A/R_A$的典范像是$X/R$的整体；另一方面，如果U在A中开路并且对于$R_A$饱和，则从假设得出$\bar{u}^1(U)$是通过使U关于R饱和而获得的集合；由于$u$是连续的，$\bar{u}^1(U)$在X（§ 2, no. 1，定理1）中开。 推论根据命题 10 从这个事实得出。

#### 例 {#top-i-s3-n6-exa-1 .statement tag=0B1Q}

设 R 表示实直线 $\mathbf{R}$ (no. 4, 例) 上的等价关系 $x \equiv y \pmod{1}$，并设 A 表示闭区间 $[0, 1]$；每个等价类 mod R 中的包含至少有一个点。$A/R_A$ 的典范映射到环面 T 上是同胚；因为如果 F 在 A 中闭（因此在 R 中），在阶中要使 F 相对于关系 R 饱和，我们必须取闭集合 $F + n$ 的并（对于所有$n \in \mathbf{Z}$），这显然形式是一个局部有限族，因此它们的并已关闭（§ 1, no. 5、命题4）；由此得出断言。我们注意到$A/R_A$是通过识别A中的点0和1得到的。\*

### 习题{#top-i-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
