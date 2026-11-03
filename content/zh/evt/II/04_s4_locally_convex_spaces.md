---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 4
section_title: Locally convex spaces
lang: zh
source: evt-i-v
book_pages: TVS II.23-TVS II.36, TVS II.74-TVS II.76
pdf_pages: 0060-0073, 0111-0113
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a locally convex space
      page: 23
      pdf_page: 60
    - "no": 2
      title: Examples of locally convex spaces
      page: 25
      pdf_page: 62
    - "no": 3
      title: Locally convex initial topologies
      page: 26
      pdf_page: 63
    - "no": 4
      title: Locally convex final topologies
      page: 27
      pdf_page: 64
    - "no": 5
      title: The direct topological sum of a family of locally convex spaces
      page: 29
      pdf_page: 66
    - "no": 6
      title: Inductive limits of sequences of locally convex spaces
      page: 31
      pdf_page: 68
    - "no": 7
      title: Remarks on Fréchet spaces
      page: 34
      pdf_page: 71
statements: 33
exercises: 17
content_sha256: 76f78091a571cef494c36959f042ea37c272fe827bd6a60282e9504362c12018
translated_from: content/en/evt/II/04_s4_locally_convex_spaces.md
translation_method: google
source_content_sha256: 739b1018258c46c62f41370f616639ef1cdd404280e387353dc0a0e48e83ef94
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 454038bd9c73a64575f4b4b1b18865ad8c7b359af82bf16267ba9be3bce684c2
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 4。局部凸空间

### 1. 局部凸空间的定义

#### 定义 1 {#evt-ii-s4-def-1 .statement tag=07E4}

— *如果存在 0 的邻域的基本系统是凸集合，则拓扑向量空间是局部凸（实数）。*

这样的空间被称为*局部凸空间*。它的拓扑被称为*局部凸拓扑*。

我们在本书其余部分中研究的 $\mathbf{R}$ 上的拓扑向量空间几乎都是局部凸的。

如果 $V$ 是局部凸空间 $E$ 中 0 的凸邻域，则 $V \cap (-V)$ 是 0 的对称凸邻域。 由于凸集合的闭包是凸的（II，p. 13，命题 14），因此来自I，p. 7，道具。 4 $E$ 中 0 的邻域是*闭、对称和凸*，形式邻域的基本系统在中心 0 和比率$\neq 0$ 的同位下不变。

#### 命题 1 {#evt-ii-s4-prop-1 .statement tag=07E5}

— *令$\mathfrak{S}$为由集合形成的向量空间$E$上的过滤器基，具有吸收性、对称且凸面。则 $\mathfrak{S}$ 集合变换集合 $\mathfrak{B}$ 通过比率 $> 0$ 的同位性是 0 的邻域的基本系统对于局部凸拓扑 $E$.*

显然 $\mathfrak{B}$ 是 I、p. 7 的过滤器基满足 (EV_I) 和 (EV_{II})。 4；它也满足 (EV_{III})，因为如果 $V \in \mathfrak{S}$ 那么 $\frac{1}{2}V + \frac{1}{2}V = V$。

请注意，如果 $\mathscr{T}$ 是 E 上的局部凸拓扑，且 $\mathfrak{B}$ 邻域的基本系统为 0，则集合 $(1/n) \ V$，其中 $n$ 在整数中变化$> 0$和V在$\mathfrak{S}$、形式变化，对于拓扑$\mathscr{T}$，邻域的基本系统为0。那么$\mathscr{T}$是Hausdorff，当且仅当对于E中的每个$x \neq 0$，存在整数$n$和集合$V \in \mathfrak{S}$，使得$nx \notin V$；此外，如果$\mathfrak{S}$是可枚举的，则拓扑$\mathscr{T}$是可度量的局部凸拓扑。相反，很明显，如果$\mathscr{T}$是可度量局部凸拓扑，则对于$\mathscr{T}$，存在闭对称凸邻域的可枚举基本系统为0。

#### 推论 {#evt-ii-s4-n1-cor-1 .statement tag=07E6}

— 拓扑向量空间 E 的 *拓扑 $\mathscr{T}$，由半范数的集合定义* (II, p. 3) *当且仅当 $\mathscr{T}$ 是局部凸的*。

条件是必要的，因为 E 上的每个半范数都是凸函数，因此，对于 $\alpha > 0$，$x \in E$ 的集合其中 $p(x) \leq \alpha$ 是凸的（II、p. 17、推论）。相反，如果 V 是 E 中 0 的对称、闭合、凸邻域，则 V 的*规范* $p$ 是 E 上的半范数，使得 V 是 E 的点 $x$ 的集合满足 $p(x) \leq 1$（II、p. 20，第 23 条）。

这进一步表明，局部凸拓扑 $\mathscr{T}$ 由 *所有对于 $\mathscr{T}$* 连续的半范数的集合定义。此外，如果 $\mathscr{T}$ 是可度量的，那么它是由半范数的*可枚举* 集合定义的。

从推论到道具。 1，半范数集合定义的拓扑上§ 1的所有结果特别适用于实数向量空间上的局部凸拓扑。局部凸 Hausdorff 空间 E 具有局部凸的完成$\hat{E}$。完整的、可度量的局部凸空间称为 *Fréchet 空间*；每个 Banach 空间都是 Fréchet 空间。

#### 命题 2 {#evt-ii-s4-prop-2 .statement tag=07E7}

— *令 f 为在向量子空间 M 上定义的连续线性形式，具有局部凸空间 E；则存在在 E 上定义的连续线性形式 h，并且是 f* 的扩张。

从上面的推论和II，p. 7，cor。 2、E 上存在连续半范数$p$，使得所有$y \in M$都有$|f(y)| \leq p(y)$。由哈恩-巴纳赫 th。 (II, p. 23, cor. 1) 在 E 上存在线性形式 $h$，扩展 $f$ 并且对于所有 $x \in E$ $|h(x)| \leq p(x)$，这意味着 $h$ 是连续的（II，p. 6，道具 5）。

#### 注 {#evt-ii-s4-n1-rem-1 .statement tag=07E8}

— 如果$g$是M在乘积空间$\mathbf{R}^I$中的连续线性映射，则$\mathbf{R}^I$中存在E的连续线性映射$h$，即$g$的扩张；对于写$g = (g_i)$，其中$g_i$是在M上定义的连续线性形式，对于每个$i \in I$，$g_i$有扩张$h_i$，这样$h_i$是E上的连续线性形式。连续线性映射 $h = (h_i)$ 具有所需的属性。

请注意，如果 F 是局部凸 Hausdorff 空间且 $g$ F 中 M 的连续线性映射，则 F 中不一定存在 E 的连续线性映射，即 $g$ 的扩张 (IV, p. 55, 练习 16, c))。然而，当 M 是有限维时，确实存在这样的扩张（*cf.* cor. 2，见下文）。

#### 推论 1 {#evt-ii-s4-prop-2-cor-1 .statement tag=07E9}

— *令 E 为局部凸空间。如果$x_0 \in E$不在$\{0\}$的闭包中，则存在在E上用$f(x_0) \neq 0$*定义的连续线性形式 f。

应用道具。 2 到由 $x_0$ 生成的一维向量空间 M 和在 M 上定义的线性形式 $\xi x_0 \mapsto \xi$，其中由 I、p. 12 支撑。 2、是连续的。

#### 推论 2 {#evt-ii-s4-prop-2-cor-2 .statement tag=07EA}

— 令 M 为 E 的有限维向量子空间，局部凸 Hausdorff 空间。则存在E的闭向量子空间N，它是E中M的拓扑补。

E 中存在 M 的拓扑补集当且仅当 M 的恒等映射本身可以扩展到 M 上的 E 的连续线性映射，则映射必然是连续的投影算子 (GT, III, § 6.2, 推论)。现在，这是从上面的注得出的，因为 M 与空间 $\mathbf{R}^n$ (I, p. 13, th. 2) 同构的。

#### 命题 3 {#evt-ii-s4-prop-3 .statement tag=07EB}

— 在局部凸空间 E 中，预紧集的平衡凸包络本身就是预紧集。

设A是E中的预紧集。给定V，E中0的平衡凸邻域，存在有限多个点$a_i \in A$($1 \leq i \leq n$)使得A包含在S中，邻域$a_i + V$($1 \leq i \leq n$)的并。因此，A 的平衡凸包络C 包含在 S 的平衡凸包络 T 中；但 T 包含在 B + V 中，其中 B 表示点 $a_i, -a_i$ ($1 \leq i \leq n$) 的有限集合的凸包络。现在 B 是预紧的（II，p. 14，cor.2）；因此，存在有限多个点$b_k \in B$（$1 \leq k \leq m$），使得$B_k$包含在邻域$b_k + V$的并中。则C包含在邻域$b_k + 2V$的并中，命题得证。

请注意，在无限维局部凸 Hausdorff 空间中，紧集的凸包络不一定是封闭的（II，p. 74，练习 3）。

#### 推论 {#evt-ii-s4-n1-cor-2 .statement tag=07EC}

— 如果在局部凸 Hausdorff 空间 E 中，紧集 X 包含在完全凸集合中（完全在由 E 引起的均匀结构中），则 X 的凸闭包络是紧的。

因为这个信封是一个完整的空间的封闭的子集，因此它是完整的，但它也是预紧的和豪斯多夫的。

然而，在非完全局部凸 Hausdorff 空间中，紧集的凸封闭包络不需要是紧致的（II，p. 87，练习 2）。

### 2. 局部凸空间的例

1) 空间 $\mathbf{R}^n$ 是局部凸的，因为中心 0 的开立方体是凸的（II，p. 9，道具 6）。因此，对于有限维的所有实拓扑向量空间也是如此；事实上，它是从上面和I, § 2.3，th 得出的。 2 假设E是Hausdorff；如果不是，则与 E 相关的 Hausdorff 空间 F 为有限维，因此局部凸，并且 F 中 0 的凸邻域的逆像在典范映射 $E \to F$ 下是凸的，形式 0 的邻域的基本系统 E.

2) 令E为$\mathbf{R}$中的向量空间，$\mathfrak{B}$为E的所有子集的族，这些子集是吸收的、对称的和凸的。通过道具。 1 of II, p. 23 我们看到$\mathfrak{B}$是0的邻域的基本系统，对于E上的局部凸拓扑$\mathscr{T}_\omega$，这是E上所有局部凸拓扑中最好的。这个拓扑是Hausdorff；让 $x \neq 0$ 为 E 的任意点；存在 E 的基 $(i_i)_{i \in I}$，其中 $\alpha \in I$ 使得 $e_\alpha = x$； 点 $y = \sum_i y_i e_i$ 的集合使得$|y_\alpha| < 1$ 具有吸收性、对称性和凸性。它不是包含 $x$。从II、p. 24、推论，可以得出$\mathscr{T}_\omega$也是由E上*所有*半范数的集合定义的拓扑，因此每个半范数在$\mathscr{T}_\omega$中都是连续的。

特别是，如果$u$是任何局部凸空间F中E的线性映射，逆像，在$u$下，F中0的每个凸邻域是E中的*吸收性*凸集合；因此，对于$\mathscr{T}_\omega$来说，邻域为0，因此对于$\mathscr{T}_\omega$来说，$u$是*连续的*。

给定E中的凸集合C，我们说点$a \in C$是C的*内部点*，如果对于每条线D包含$a$，交$D \cap C$ 包含于 an open segment which 包含于 $a$;在其他字 - $a + C$ 是*吸收性*。 E 中集合 A 的点 $a$ 对于* $\mathscr{T}_\omega$ 是 A 的*内部，当且仅当存在一个凸集合 C 与 $a \in C \subset A$，并且使得 $a$ 是以下的内点 C。

更一般地，令 V 为 E 中的仿射线性簇，C 为V 中包含的凸集合； 点 $a \in C$ 是 C 相对于* V 的*内部点，如果在向量子空间 $V_0 = -a + V$ 中，点 0 是集合的内部点 $C_0 = -a + C$。

当E为有限维时，拓扑$\mathscr{T}_\omega$恰好是E上的规范拓扑（I，p. 13，第2）；这表明，E 中凸集合 C 的每个内部点都位于规范拓扑的 C 的内部（*cf.* II，p. 74，练习 5）。

3) 设 A 是 $\mathbf{R}$ 上向量空间 E 中的对称凸集合。由 A *生成*的向量子空间 F 也是由 A 生成的凸锥体，因为 $-A = A$；这个集合是$\lambda x$的集合，其中$x \in A$和$\lambda \in \mathbf{R}$； 集合 A 在* F 和集合 $\lambda A$ 中*吸收，其中 $\lambda > 0$、形式邻域的基本系统为 0，对于* F 上的局部凸拓扑 *（据说由 A *定义*），即由半范数$p_A$定义，A的*规范*（II，p. 20，道具22）；我们将 $E_A$ 写为通过给 F 半范数而获得的局部凸空间。 空间 $E_A$ 是 *Hausdorff* 当且仅当 $p_A$ 是 *范数* 或者 A 不包含 *任何行*。如果 B 是 E 中的第二个对称凸集合，并且如果$A \subset B$，则显然$E_A \subset E_B$，并且$E_B$中$E_A$的典范嵌入对于由 A 和 B 分别定义的拓扑是*连续的。此外，如果 $f$ 是 E 的线性映射在实向量空间 $E'$ 中，$f(A)$ 在 $E'$ 中是凸且对称的，$f$ 是$E_A$ *在* $E'_{f(A)}$ 上的*连续* 线性映射。

最后，请注意，如果 E 携带与其向量空间结构兼容的拓扑 $\mathscr{T}$，并且如果 V 是 $\mathscr{T}$ 的 0 对称 *凸* 邻域，则由 V 生成的向量空间是相同的与 E，因为 V 是吸收性的，并且 $E_V$ 中 E 的恒等映射是*连续*。

### 3. 局部凸初始拓扑

#### 命题 4 {#evt-ii-s4-prop-4 .statement tag=07ED}

*设 E 为向量空间，并令 $(E_i)_{i \in I}$ 为局部凸空间族。对于每个$i \in I$，令$f_i$为$E_i$中E的线性映射；那么 E 上的拓扑* $\mathscr{T}$ 是使每个映射 $f_i$ 连续的最粗糙的，是局部凸的拓扑。

使用 II、p. 24、推论，这是由半范数 (II、p. 5) 定义的拓扑的相应的性质的特殊情况。

特别是，局部凸空间的每个向量子空间以及局部凸空间的每个乘积空间都是局部凸的。局部凸空间的每个射影极限都是局部凸的。

Fréchet 空间的每个*可枚举乘积*（特别是 Banach 空间的每个可枚举乘积）都是 Fréchet 空间。

每个局部凸 Hausdorff 空间 E 都同构于 Banach 空间的乘积的子空间，并且如果 E 是完备的，则该子空间是封闭的（II，p. 5，道具 3）。每个 Fréchet 空间都同构于 Banach 空间的可枚举乘积的闭子空间（*loc.cit.*）。

### 4. 局部凸最终拓扑

#### 命题 5 {#evt-ii-s4-prop-5 .statement tag=07EE}

*设E为向量空间，$(F_\alpha)_{\alpha \in A}$为向量空间的拓扑族，对于每个$\alpha \in A$，令$g_\alpha$为E中$F_\alpha$的线性映射。*

(i) *用$\mathfrak{B}$表示E的吸收性、对称凸子集V族，使得对于每个$\alpha$，$g_\alpha^{-1}(V)$是$F_\alpha$中0的邻域； $\mathfrak{B}$族是拓扑$\mathscr{T}$的E中0的邻域的基本系统，与向量空间结构兼容。*

(ii) E 的 *线性映射 f 在局部凸空间 G（或 E 上的半范数 p）中对于 $\mathscr{T}$ 连续，当且仅当对于每个指标 $\alpha$，$f \circ g_\alpha$（或 $p \circ g_\alpha$）在$F_\alpha$.*

(iii) *拓扑$\mathscr{T}$是E上最好的局部凸拓扑，其中$g_\alpha$是连续的。*

*此外，拓扑 $\mathscr{T}$ 是 E 上唯一满足条件 (ii) 对于线性映射（分别针对半范数）的局部凸拓扑。*

由于$\mathfrak{B}$是一个过滤器基在比率> 0的相似性下不变，断言（i）立即从II，p. 23，道具。 1. 通过$\mathfrak{B}$的定义，拓扑$\mathscr{T}$是E上最好的局部凸拓扑，使得$g_\alpha$连续； 从而（三）。最后很清楚，如果$f$连续，则$f \circ g_\alpha$也连续；相反，如果$f \circ g_\alpha$对于每个$\alpha$都是连续的，则对于G中每个0的对称凸邻域W，对于每个$\alpha$，集合$g_\alpha^{-1}(f^{-1}(W))$是$F_\alpha$中0的邻域。现在$f^{-1}(W)$是吸收性的、对称的、凸的，因此$f^{-1}(W)$是$\mathscr{T}$中0的邻域，并且$f$是连续的。类似地，如果$p$是E上的半范数，使得$p \circ g_\alpha$对于每个$\alpha$都是连续的，并且如果U是点$x \in E$的集合使得$p(x) < 1$，那么对于每个$\alpha$，集合 $g_\alpha^{-1}(U)$ 是 $E_\alpha$ 中 0 的凸邻域，对称且具有吸收性；因此，U 是 E 中 0 的邻域，并且 $p$ 是连续的（II，p. 2，道具 1）。

最后一个叙述源自S，IV, § 2.5，标准CST 18。

我们说$\mathscr{T}$是$F_\alpha$拓扑族$\mathscr{T}_\alpha$的*局部凸最终拓扑*，对于线性映射$g_\alpha$族。

$\mathscr{T}$ 可能不是 E 上与其向量空间结构兼容且使 $f_\alpha$ 连续的拓扑中最好的（II、p. 75、执行 15；另请参阅II、p. 75、执行 14）。

在最重要的情况$E = \sum_{\alpha \in A} g_\alpha(F_\alpha)$中，对于$\mathscr{T}$，我们得到邻域的基本系统为0，如下所示；对于每个$\alpha \in A$，令$V_\alpha$为$\mathscr{T}_\alpha$的对称邻域，$\alpha \in A$的$g_\alpha(V_\alpha)$的形式并，并用$\Gamma((g_\alpha(V_\alpha)))$表示该并的E中的凸包络；因为E的每个元素都是形式$\sum_{\alpha \in J} x_\alpha$，其中J是I和$x_\alpha \in g_\alpha(F_\alpha)$的有限子集，所以直接的$\Gamma((g_\alpha(V_\alpha)))$是E中的*吸收性*对称凸集合（每个$V_\alpha$在$F_\alpha$中具有吸水性）；如$\Gamma((g_\alpha(V_\alpha)))$包含所有$g_\alpha(V_\alpha)$，$\mathscr{T}$为0的邻域。另一方面，很明显，对于$\mathscr{T}$的每个对称凸邻域V为0，我们有$V \supset \Gamma((V \cap g_\alpha(F_\alpha)))$，从中我们可以得出断言。

#### 推论 1 {#evt-ii-s4-prop-5-cor-1 .statement tag=07EF}

*带有记号的支柱。 5、令H为局部凸空间G中E的线性映射的集合。假设E为其子空间$g_\alpha(F_\alpha)$的和；则 H 对于 $\mathscr{T}$ 等连续，当且仅当对于每个 $\alpha$、集合 $f \circ g_\alpha$，其中 $f$ 在 H 中变化，在 $F_\alpha$ 中等连续。*

记住I，p. 9，道具。 6 该论证与(ii) 命题类似。 5. 令 W 为 G 中 0 的对称凸邻域，并注意，如果集合 $f \circ g_\alpha$，其中 $f \in H$ 等连续，则交 $\bigcap_{f \in H} g_\alpha^{-1}(f^{-1}(W))$ 为 $F_\alpha$ 中 0 的对称凸邻域。由于这个交与 $g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W))$ 相同，并且集合 $\bigcap_{f \in H} f^{-1}(W)$ 是对称且凸的，所以一切都取决于证明它也是*吸收性的*。现在，到假设，每个$x \in E$都可以写成$\sum_{i=1}^n g_{\alpha_i}(z_{\alpha_i})$，其中$z_{\alpha_i} \in F_{\alpha_i}$。为了证明对于所有$f \in H$存在$\lambda > 0$使得$f(\lambda x) \in W$，考虑$x = g_\alpha(z_\alpha)$和$z_\alpha \in F_\alpha$的情况就足够了（因为我们可以通过替换W通过$W/n$传递到一般情况）。但这种情况是因为$g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W))$是$F_\alpha$中0的邻域。

#### 推论 2 {#evt-ii-s4-prop-5-cor-2 .statement tag=07EG}

*令$(J_\lambda)_{\lambda \in L}$为指标集合A的划分。令$(G_\alpha)_{\alpha \in A}$为局部凸空间族，$(F_\lambda)_{\lambda \in L}$为向量空间族。对于每个$\lambda \in L$，令$h_\lambda$为向量空间E中$F_\lambda$的线性映射；对于每个$\lambda \in L$和$\alpha \in J_\lambda$，令$g_{\lambda \alpha}$为$F_\lambda$中$G_\alpha$的线性映射。写$f_\alpha = h_\lambda \circ g_{\lambda \alpha}$。假设每个$F_\lambda$都带有最细的局部凸拓扑，使得$g_{\lambda \alpha}$（$\alpha \in J_\lambda$）连续。那么，E 上使 $f_\alpha$ 连续的最细局部凸拓扑与使 $h_\lambda$ 连续的最细局部凸拓扑相同。*

这是 S，IV, § 2.5 准则 CST 19 的特例，也可以直接使用 prop 来证明。 5.

局部凸最终拓扑的例。

I。 商空间。

令 M 为局部凸空间 F 的子空间，并且 φ 为 F/M 上 F 的典范映射。由于 F/M 上的商拓扑是局部凸的，并且是使 φ 连续的所有拓扑（局部凸或非局部凸）中最好的，因此它也是单个映射 φ 族由……组成的局部凸最终拓扑。

II。局部凸空间的归纳极限。

设 A 为向右有序的集合，并令 $(E_\alpha, f_{\beta\alpha})$ 为向量空间相对于集合 A 的归纳系统 (A, II, § 6.2)；让$E = \varinjlim E_\alpha$和$f_\alpha : E_\alpha \to E$成为每个$\alpha \in A$的规范线性映射。 假设每个$E_\alpha$带有一个局部凸拓扑$\mathscr{T}_\alpha$，并进一步假设对于$\alpha \leq \beta$，映射$f_{\beta\alpha} : E_\alpha \to E_\beta$是*连续的*。 然后我们说族$(\mathscr{T}_\alpha)$相对于线性映射$f_\alpha$（分别是承载拓扑$\mathscr{T}$的空间E）的局部凸最终拓扑$\mathscr{T}$是族$(\mathscr{T}_\alpha)$的*归纳极限*（分别是系统$(E_\alpha, f_{\beta\alpha})$的*归纳极限*空间，或者简单地是局部凸空间$E_\alpha$）。 回想一下，E 是向量子空间 $f_\alpha(E_\alpha)$ 的并，当 $\alpha \leq \beta$ 时，我们有 $f_\alpha(E_\alpha) \subset f_\beta(E_\beta)$；如果我们将映射$f_\alpha$赋予$f_\alpha(E_\alpha)$最终的拓扑（这与用商空间$E_\alpha/f_\alpha^{-1}(0)$识别$f_\alpha(E_\alpha)$相同），拓扑$\mathscr{T}$也是最终的拓扑 $f_\alpha(E_\alpha)$拓扑系列，相对于典范嵌入（II，上面的相关2）。 此外，$f_{\beta\alpha}$对于$\alpha \leq \beta$的连续性意味着典范嵌入$j_{\beta\alpha} : f_\alpha(E_\alpha) \to f_\beta(E_\beta)$是连续的，因此E也是$f_\alpha(E_\alpha)$相对于单射$j_{\beta\alpha}$的归纳极限，带有前面的拓扑。

#### 例 {#evt-ii-s4-n4-exa-1 .statement tag=07EH}

— 令 X 为有限连续实值函数的局部紧致空间和 $E = \mathscr{K}(X; \mathbf{R})$ 向量空间，在 X 上定义，具有紧致支持。对于 X 的每个紧凑子集 K，令 $E_K$ 为由函数 $f \in E$ 构成的 E 的向量子空间，这些$x \notin K \Rightarrow f(x) = 0$ 是这样的。用$E_K$上诱导的$\mathscr{T}_K$拓扑和X上*均匀收敛*的$\mathscr{T}_u$拓扑表示。拓扑$\mathscr{T}_K$的电感极限$\mathscr{T}$比$\mathscr{T}_u$小更细；我们可以证明，如果 X 是仿紧且不是紧的，那么 $\mathscr{T}$ 严格来说更细比 $\mathscr{T}_u$ (*cf.* INT, III, 2nd ed., § 1.8)。 $\mathscr{T}$的重要性在于，在$\mathscr{T}$中连续的E上的线性形式正是X上的真实*测量*（INT，III，2nd.，§ 1.3）。

#### 注 {#evt-ii-s4-n4-rem-1 .statement tag=07EI}

— 在最后一个例子中，$\mathscr{T}$在$E_K$上引起的拓扑与$\mathscr{T}_K$相同，因为根据定义它比$\mathscr{T}_K$更粗糙，并且由于$\mathscr{T}$比$\mathscr{T}_u$更精细，所以$\mathscr{T}$在$E_K$上引起的拓扑比$\mathscr{T}_u$更精细，就是说$\mathscr{T}_K$。

当 E 上存在局部凸拓扑 $\mathscr{T}'$ 使得 $\mathscr{T}_\alpha$ 是由 $\mathscr{T}'$ 在 $E_\alpha$ 上诱导出拓扑时，推理立即推广到局部凸拓扑 $(\mathscr{T}_\alpha)$ 的归纳极限。

更一般地，人们可以问，当我们假设$E_\beta \subset E_\alpha$和$\mathscr{T}_\beta$是由$\mathscr{T}_\alpha$诱发拓扑时，在什么情况下$\mathscr{T}$诱导$\mathscr{T}_\alpha$在每个$E_\alpha$上。一般来说，情况并非如此（II，p. 80，练习26）；但我们将在以下两种重要情况中看到这种情况确实发生。

### 5. 局部凸空间族的直接拓扑和

#### 定义 2 {#evt-ii-s4-def-2 .statement tag=07EJ}

*设 E 为向量空间，即直和* (A, II, § 1.6) *属于局部凸空间* $(E_i)_{i \in I}$族。 *对于每个*$i \in I$，*让*$f_i$*成为$E$中$E_i$的典范嵌入*。 *通过族的拓扑直和* $(E_i)$ *我们的意思是空间* $E$ *具有最精细的局部凸拓扑，这使得每个* $f_i$ *连续（这个拓扑被称为*拓扑的直和） $E_i$）。

在这个编号的其余部分中，我们保留与 def 中相同的记号。 2（明确说明了除非相反），我们认同，典范地，每个$E_i$与$E$的子空间，通过$f_i$。

通过II，p. 28中给出的局部凸最终拓扑的一般描述和邻域，我们可以在这里获得$E$中0的邻域的基本系统，对于直和拓扑，以下方式；对于*每个*族$(V_i)_{i \in I}$，其中$V_i$是$E_i$中0的对称凸邻域，考虑$V_i$的并的凸包络$\Gamma((V_i))$；所有家庭$(V_i)$的$\Gamma((V_i))$（或仅对每个$i$取$V_i$，使$E_i$中邻域的基本系统为0）形式为系统的基本系统 $E$ 中的邻域为 0。

#### 例 {#evt-ii-s4-n5-exa-1 .statement tag=07EK}

— 令$(a_i)_{i \in I}$为向量空间$E$的基，并考虑每行$Ra_i$上的规范拓扑（I，p. 2，*例5*）；这些拓扑中的直和是$E$（II，p. 26）上*最好的*局部凸拓扑；事实上，如果$V$是$E$中的吸水、对称、凸集合，则$V_i = V \cap Ra_i$是$Ra_i$和$V$中0的邻域，显然包含凸包络$\Gamma((V_i))$。

#### 命题 6 {#evt-ii-s4-prop-6 .statement tag=07EL}

*局部凸拓扑* $\mathscr{T}$ *在* $E$ *是* $E_i$的拓扑的直和，*当且仅当，以下性质成立：线性映射 of* $E$ *在局部凸中空间* $G$ *（或半范数* $p$ *在* $E$）*是连续的，当且仅当对于每个* $i \in I$，*映射* $g \circ f_i$ *（或$p \circ f_i$）在*中连续$E_i$。

这是 prop 的一个特例。 5、II、p. 27。

回想一下向量空间家庭的直和的定义（A，II，p. 12，道具6），我们可以说拓扑$\mathscr{T}$是唯一一个典范映射$g \mapsto (g \circ f_i)$是*双射*

$$
\mathscr{L}(E; G) \to \prod_{i \in I} \mathscr{L}(E_i; G)
$$

对于每个局部凸空间$G$。

#### 推论 {#evt-ii-s4-n5-cor-1 .statement tag=07EM}

*带有记号的支柱。 5、II、p. 27，假设*$E$*是*$g_\alpha(F_\alpha)$的和。 *设* $F$ *为族* $(F_\alpha)_{\alpha \in A}$的拓扑直和，*并让* $j_\alpha : F_\alpha \to F$ *为典范嵌入；假设*$g : F \to E$*是线性映射使得*$g \circ j_\alpha = g_\alpha$*对于所有*$\alpha \in A$。 *如果* $N$ *是* $g$的核，*则规范的双射* $F/N \to E$ *与* $g$ *关联，是* $F/N$ *上的拓扑同构 * $E$ *与拓扑* $\mathscr{T}$。

这是 II、p. 28 的特例。 2 记住II、p. 29、*例I*。

#### 命题 7 {#evt-ii-s4-prop-7 .statement tag=07EN}

*典范嵌入* $j : E \to \prod_{i \in I} E_i$ *在* $E$ *携带* $E_i$ *和* $\prod_{i \in I} E_i$ *携带乘积拓扑的直和拓扑时连续。当* $I$ *有限时，这个映射是拓扑向量空间的同构。*

第一个断言源自以下事实：典范嵌入$E_\kappa \to \prod_{\iota \in I} E_\iota$对于每个$\kappa \in I$都是连续的。如果$I$是有限的，则$j$是恒等映射，并且足以证明乘积拓扑$\mathscr{T}'$比直和拓扑$\mathscr{T}$是更细。现在，令 $V$ 为 $\mathscr{T}$ 的 0 凸邻域；每个集合$V \cap E_\iota$都是$E_\iota$中0的凸邻域；如果$n$是$I$的元素的数，那么集合$V$包含集合$\frac{1}{n} \sum_n (V \cap E_\iota)$，对于$\mathscr{T}'$来说邻域是0，并且命题得证。

当$I$无穷大时，如果对于$I$的每个有限子集$J$，我们为空间$\prod_{\iota \in J} E_\iota$写出$E_J$，以及乘积拓扑，那么$E$就是极限*的归纳极限* $E_J$（标识为$E$ 的子空间）。

#### 命题 8 {#evt-ii-s4-prop-8 .statement tag=07EO}

*对于每个$\iota \in I$，令$N_\iota$为$E_\iota$的子空间，*

(i) *在$E$上由直和拓扑$\mathscr{T}$在$N = \sum_\iota N_\iota$上感应的拓扑与$N_\iota$拓扑的直和相同。*

(ii) *$E/N$ (A, II, § 1.6, 公式 (26)) 上的$E_\iota / N_\iota$的拓扑直和空间的典范映射$h$是拓扑向量空间之间的同构。*

(i) 通过上面介绍的记号，我们考虑$x = \sum_\iota \lambda_\iota x_\iota$属于到$N \cap \Gamma((V_\iota))$（$(\lambda_\iota)$是数$\geqslant 0$的族，其中最多有限多个非零，使得$\sum_\iota \lambda_\iota = 1$和$x_\iota \in V_\iota$，对于所有$\iota \in I$）。由于$N_\iota$的和是直接的，所以我们对所有$\iota \in I$有$\lambda_\iota x_\iota \in N_\iota$；因此，对于所有$\iota$使得$\lambda_\iota > 0$我们也有$x_\iota \in N_\iota \cap V_\iota$，以及$x$属于到凸包络$\Gamma((N_\iota \cap V_\iota))$，从而证明（i）。

(ii) 将典范映射表示如下：$f_\iota : E_\iota \to E, h_\iota : E_\iota / N_\iota \to E/N, p_\iota : E_\iota \to E_\iota / N_\iota$和$p : E \to E/N$。对于每个 $\iota \in I$、$h_\iota \circ p_\iota = p \circ f_\iota$ 和命题，都可以从 II、p. 28 得出。 2 和 p. 29 *例 I*。

#### 推论 1 {#evt-ii-s4-prop-8-cor-1 .statement tag=07EP}

*如果每$\iota \in I$在$E_\iota$关闭$N_\iota$，则$N = \sum_\iota N_\iota$在$E$关闭。*

因为，对于每个 $\iota \in I$，典范映射 $p_\iota : E \to E_\iota$ 都是连续的（II, § 4.5，道具 6），因此 $p_\iota^{-1}(N_\iota)$ 在 $E$ 中闭合，因此交 $N = \bigcap_{\iota \in I} p_\iota^{-1}(N_\iota)$ 也是如此。

#### 推论 2 {#evt-ii-s4-prop-8-cor-2 .statement tag=07EQ}

*如果每个$E_\iota$都是Hausdorff，那么$E$也是Hausdorff，并且每个$E_\iota$在$E$中闭合。*

要证明第一个叙述，请应用cor。 1 为所有 $\iota \in I$ 取 $N_\iota = \{0\}$；第二个应用 cor。 1 每个 $\kappa \neq \iota$ 对应 $N_\iota = E_\iota$ 和 $N_\kappa = \{0\}$。

我们将在 III、p. 21 中展示。 2 如果 $E_\iota$ 是 Hausdorff 并且*完整*，那么它们的拓扑直和 $E$ 也是。

### 6. 局部凸空间序列电感极限

在这个数中，我们将考虑向量空间$E$的向量子空间的*递增序列*$(E_n)$，使得$E$是$E_n$的*并*；我们假设每个$E_n$带有一个局部凸拓扑$\mathscr{T}_n$，这样，对于每个$n$，$\mathscr{T}_{n+1}$在$E_n$上诱导的拓扑比$\mathscr{T}_n$*粗糙*，并且我们给$E$局部凸拓扑$\mathscr{T}$即序列$(\mathscr{T}_n)$的*感应极限*（II，p. 29，*例II*）；这些假设和记号将在本编号的其余部分中使用，无需重述。

可能会出现每个$\mathscr{T}_n$是豪斯多夫但$\mathscr{T}$不是的情况；也可能发生这样的情况：对于整数$n, m$的每个对，$n \leq m$、子空间$E_n$在$E_m$中闭合（使用拓扑$\mathscr{T}_m$），但$E_n$在$E$中不闭合，使用$\mathscr{T}$（II，p. 80，练习 26）。

#### 引理 1 {#evt-ii-s4-lem-1 .statement tag=07ER}

— *令$\mathfrak{F}$为$E$上的柯西滤波器（对于$\mathscr{T}$）；那么存在整数$k$，这样对于所有$N \in \mathfrak{F}$以及$E$中$0$的每一个邻域$V$，子空间$E_k$都满足$N + V$。*

我们假设相反并得出矛盾。假设对于每个 $k$ 都存在邻域 $V_k$ $0$ 和集合 $M_k \in \mathfrak{F}$ 使得
$$
(E_k + V_k) \cap M_k = \varnothing.
$$
显然，我们可以假设 $V_{k+1} \subset V_k$ 对于所有 $k$。令$V$为$\bigcup_k (E_k \cap V_k)$的凸包络，这显然是$\mathscr{T}$的$0$的邻域。对于所有 $n$，我们有 $V \subset V_n + E_n$；事实上，每个$x \in V$都可以写成$\sum_i \lambda_i x_i$，其中$\lambda_i \geq 0$、$\sum_i \lambda_i = 1$和$x_i \in V_i \cap E_i$对于所有$i$；现在对于$i < n$，我们有$x_i \in E_n$，因此$\sum_{i < n} \lambda_i x_i \in E_n$；对于$i \geq n$，我们有$x_i \in V_n$，因此$\sum_{i \geq n} \lambda_i x_i \in V_n$，因为$V_n$是凸的，包含$0$和$\sum_{i \geq n} \lambda_i \leq 1$。因此，对于所有 $n$ 来说，$V + E_n \subset V_n + E_n$。既然如此，令$M \in \mathfrak{F}$为集合，即$V$小。对于某些整数 $m$，$E_m \cap M$不为空；我们结论
$$
M \subset E_m + V \subset E_m + V_m;
$$
由于$\mathfrak{F}$是一个过滤器，集合$M_m$满足$M$，因此$E_m + V_m$；我们有一个矛盾，它成立引理。

#### 命题 9 {#evt-ii-s4-prop-9 .statement tag=07ES}

*假设对于每个整数$n$，$\mathscr{T}_{n+1}$在$E_n$上诱导的拓扑与$\mathscr{T}_n$相同。然后
(i) $\mathscr{T}$在$E_n$上引起的拓扑与每个$n$的$\mathscr{T}_n$相同；如果 $\mathscr{T}_n$ 是 Hausdorff，则 $\mathscr{T}$ 是 Hausdorff。
(ii) 如果对于每个$n$，$E_n$ 在$E_{n+1}$（对于$\mathscr{T}_{n+1}$）闭合，那么对于每个$n$，$E_n$ 在$E$（使用$\mathscr{T}$）闭合。
(iii) 如果每个 $E_n$ 都是完整的（使用 $\mathscr{T}_n$），那么 $E$ 使用 $\mathscr{T}$ 是完整的。*

(i) 为了证明第一个断言，只要证明$\mathscr{T}$在$E_n$上诱发拓扑$\mathscr{T}'_n$比$\mathscr{T}_n$更细就足够了。为此，令$V_n$为$0$在$E_n$中对于拓扑$\mathscr{T}_n$的凸邻域；我们将$E_{n+p}$中$0$的凸邻域的构造递增序列对于$\mathscr{T}_{n+p}$，比如说$(V_{n+p})_{p \geq 1}$，这样对于每个指标$p \geq 1$来说$V_{n+p} \cap E_n = V_n$。那么递增序列 $(V_{n+p})$ 的并 $V$ 将是凸集合，使得 $V \cap E_k$ 是 $E_k$ 中 $0$ 的邻域（使用 $\mathscr{T}_k$），对于每个指标$k$；因此，对于$\mathscr{T}$，$V$将是$E$中$0$的邻域，并且作为$V \cap E_n = V_n$，我们已经证明$\mathscr{T}'_n$比$\mathscr{T}_n$是更细。

到定义到$V_{n+p}$，我们使用以下引理，在$p$上经过归纳：

#### 引理 2 {#evt-ii-s4-lem-2 .statement tag=07ET}

*令$V$为局部凸空间$F$的$M$、向量子空间中0的凸邻域。那么在 $F$ 中存在 0 的凸邻域 $W$，使得 $W \cap M = V$。此外，如果 $M$ 在 $F$ 中闭合，则对于每个点 $x_0 \in \complement M$，$F$ 中存在 0 的凸邻域 $W_0$，使得 $W_0 \cap M = V$ 和 $x_0 \notin W_0$。*

事实上，到假设时，$F$ 中存在 0 的凸邻域 $U$，使得$U \cap M \subset V$。显然，$F$中$U \cup V$的凸包络$W$是$F$中0的邻域；我们证明$W \cap M = V$。因为，每个点$z \in W$都是形式$\lambda x + (1-\lambda) y$与$x \in V, y \in U$和$0 \leq \lambda \leq 1$（II，p. 9，第8条）；如果$z \in M$和$\lambda \neq 1$那么必然是$y \in M$，因此$y \in U \cap M \subset V$，因此$z \in V$；如果$\lambda = 1$，结果显然为真。如果$M$在$F$内闭，空间$F/M$是Hausdorff，因此$F$中存在0的凸邻域$U_0 \subset U$，使得$U_0$不满足$x_0 + M$；那么$U_0 \cup V$的凸包络$W_0$满足要求的条件。

回到定理，为了证明(i)的第二个部分，请注意，如果$x \in E$，则对于某些$n$，$x \in E_n$；如果 $x \neq 0$ 和 $\mathscr{T}_n$ 是 Hausdorff，则 $\mathscr{T}_n$ 的邻域 $V_n$ 为 0，而包含 $x$ 则不存在。我们看到对于 $\mathscr{T}$ 存在邻域 $V$ 为 0，这样 $V \cap E_n = V_n$，因此$x \notin V$，并且由此可见 $\mathscr{T}$ 是 Hausdorff。

(ii) 设 $x \in E - E_n$；存在$m > n$使得$x \in E_m$，因此，因为对于$\mathscr{T}_m$，$E_n$在$E_m$中是封闭的（因为假设，对于每个$n$，在$E_n$上存在$\mathscr{T}_{n+1}$诱导$\mathscr{T}_n$） 拓扑 $\mathscr{T}_m$ $E_m$ 中 0 的凸邻域 $V_m$，使得 $(x + V_m) \cap E_n$ 为空。现在我们在 (i) 中看到，对于 $\mathscr{T}$ 存在 0 的凸邻域 $V$，使得 $V \cap E_m = V_m$；因此$(x + V) \cap E_m = x + V_m$，因此$(x + V) \cap E_n = \varnothing$，这证明了(ii)。

(iii) 从引理 1，如果$\mathfrak{F}$是$\mathscr{T}$（GT，II, § 3.2）的*最小*柯西滤波器，则存在$k$，使得$\mathfrak{F}$在$E_k$上的迹是滤波器$\mathfrak{F}_k$；从 (i) 这最后一个是 $\mathscr{T}_k$ 的柯西滤波器，因此 $\mathfrak{F}_k$ 通过假设收敛于 $E_k$；但是由于$\mathfrak{F}_k$生成的$E$上的过滤器是更细比$\mathfrak{F}$，我们看到$\mathfrak{F}$对于$\mathscr{T}$有一个集群点，因此对于$\mathscr{T}$是收敛的。

当$\mathscr{T}_{n+1}$在$E_n$上感应出的所有$n$拓扑只是$\mathscr{T}_n$时，我们说$\mathscr{T}$是序列$(\mathscr{T}_n)$的*严格归纳极限*，并且空间 $E$和拓扑$\mathscr{T}$是局部凸空间$E_n$的序列的*严格归纳极限*。

#### 注 {#evt-ii-s4-n6-rem-1 .statement tag=07EU}

— 1) 假设$E$是递增定向的并，子空间$(E_\alpha)_{\alpha \in I}$的*不可枚举*族，每个$E_\alpha$都有一个局部凸拓扑$\mathscr{T}_\alpha$，这样，对于$E_\alpha \subset E_\beta$， $\mathscr{T}_\beta$ 在$E_\alpha$ 上诱发的拓扑与$\mathscr{T}_\alpha$ 相同。可能的情况是，拓扑$\mathscr{T}$在每个$E_\alpha$上诱导的拓扑等于$\mathscr{T}_\alpha$，并且$E_\alpha$是*Hausdorff且完整的，但$E$对于$\mathscr{T}$*不完整（INT，III，第二版，§ 1，练习 2)。

2) 设$F$为局部凸空间，即向量子空间$(F_n)$的递增序列的并，对于每个指标$n$，令$\mathscr{T}_n$为拓扑由 $F$ 的拓扑 $\mathscr{T}$ 在 $F_n$ 诱发。应该注意的是，一般来说 $\mathscr{T}$ 并不是 $\mathscr{T}_n$ 的归纳极限。

3）假设$E$是序列$(E_n)$的严格归纳法极限；如果 $F$ 是 $E$ 的闭（在 $\mathscr{T}$ 中）向量子空间，则可能会出现这样的情况：$\mathscr{T}_n$ 在 $F \cap E_n$ 上诱导的拓扑的严格归纳极限 * 严格小于更细* 拓扑由 $\mathscr{T}$ 诱发（IV、p. 63、锻炼 10）。

#### 命题 10 {#evt-ii-s4-prop-10 .statement tag=07EV}

*设E、F为两个局部凸空间。假设：*

1) *存在一个Fréchet族空间* $(E_\alpha)$，*并且对于每个$\alpha$线性映射* $g_\alpha : E_\alpha \to E$，*使得E的拓扑是该族*$(g_\alpha)$的最终局部凸拓扑。

2) *存在 Fréchet 空间* $(F_n)$ *的序列 *并且对于每个 n 都有一个连续线性单射* $j_n : F_n \to F$ *使得* $F = \bigcup_n j_n(F_n)$。

*那么F中E的每一个线性映射u，其图封闭在*$E \times F$，*必然是连续的。*

为了证明 $u$ 是连续的，只需证明对于每个 $\alpha$，映射 $u \circ g_\alpha : E_\alpha \to F$ 是连续的（II，p. 27，命题 5）。现在$u \circ g_\alpha$的图是连续映射$g_\alpha \times 1_F : E_\alpha \times F \to E \times F$下$u$图的逆像，因此到假设，在$E_\alpha \times F$封闭。因此，我们可以将自己限制在 E 本身是 *Fréchet 空间* 的情况。但命题是I、p. 20的特例。 1.

#### 推论 {#evt-ii-s4-n6-cor-1 .statement tag=07EW}

*对 E 和 F 的假设与命题中相同。 10 并假设 E 是 Hausdorff，则 E 中 F 的每个连续满射映射 v 都是严格的态射。*

令N为$v$的核并写成$N_n = j_n^{-1}(N)$；那么映射$j'_n : F_n / N_n \to F / N$，从$j_n$通过取商推导出来，是单射且连续的，$F_n / N_n$也是Fréchet空间（因为$N_n$是封闭的）并且$F / N$是并像低于$j'_n$。通过假设，在规范因式分解$v : F \to F / N \xrightarrow{w} E$中，线性映射$w$是双射且连续的，因此它在$(F / N) \times E$中的图是*封闭的*（GT，I, § 8.1，第2项的cor.2）。通过注开始并通过 prop。 10、$w$的逆映射$u$因此是连续的，推论被证明。

\* 命题 10 及其推论特别适用于当 E 是一个*完整的出生学空间*（III，p. 12）并且 F 是 Fréchet 空间的序列的归纳极限时。 \*

### 7. 注弗雷谢空间

我们将考虑道具。 GT 的 2，在局部凸空间的情况下，IX, § 3.1。

#### 命题 11 {#evt-ii-s4-prop-11 .statement tag=07EX}

*令 E 为可测量的局部凸空间。 E 的拓扑可以通过平移下不变的距离来定义，并且开球是凸的。*

令$(p_n)_{n \in \mathbf{N}}$为E的定义拓扑的半范数序列。令$d_n$为$d_n(x, y) = \inf(p_n(x - y), 1/n)$对E中的$x, y$定义的伪度量；它在翻译下是不变的。对于每个$n \geq 0$和每个实数$R \geq 0$，令$B_{n, R}$为$x \in E$的集合，其中$d_n(x, 0) < R$。如果$R \geq 1/n$，则$B_{n, R} = E$，而在其他情况下，$B_{n, R}$由$x \in E$形成，使得$p_n(x) < R$；在所有情况下 $B_{n, R}$ 都是凸的。

对于$E$定义$d(x, y) = \sup_{n \in \mathbf{N}} d_n(x, y)$中的$x, y$。我们立即看到 $d$ 是一个距离，在 $E$ 的平移和定义 $E$ 的拓扑下保持不变。对于$x_0 \in E$和$R \geq 0$，中心$x_0$和半径$R$（对于距离$d$）的开球等于$\bigcap_{n \in \mathbf{N}} (x_0 + B_{n, R})$，因此它是凸球。

#### 命题 12 {#evt-ii-s4-prop-12 .statement tag=07EY}

*设$E$和$F$是两个Fréchet空间和$u$，$F$上$E$的连续线性映射。那么存在$u$的截面是连续的虽然不一定是线性的。*

通过道具。 11 $E$中存在距离$d$，平移不变，定义拓扑或$E$，并且开球是凸的。 给定$F$中的$y$和$y'$，令$\delta(y, y')$为$E$中闭合的集合$u^{-1}(y)$和$u^{-1}(y')$之间的距离。 由于$u$是GT的严格态射（I，p. 17，第1）注，IX, § 3.1表明$\delta$是定义$F$的拓扑的$F$上的距离。 我们将归纳地构造$F$在$E$中的连续映射$(s_n)_{n \in \mathbf{N}}$，并且对于所有$y \in F$满足以下不等式：

$$
\delta(y, u(s_n(y))) < 2^{-n}
$$
$$
d(s_n(y), s_{n-1}(y)) < 2^{-n+1} \quad \text{(only if } n \geq 1 \text{)}.
$$

假设$n = 0$或$n \geq 1$以及$s_{n-1}$已被构造。设 $y_0 \in F$；由于$u$是满射，集合$u^{-1}(y_0)$非空，对于$n \geq 1$，我们有$d(u^{-1}(y_0), s_{n-1}(y_0)) < 2^{-n+1}$乘以归纳假设。因此，存在$E$的点$x_0$，使得$u(x_0) = y_0$，并且对于$n \geq 1$，$d(x_0, s_{n-1}(y_0)) < 2^{-n+1}$。由于映射 $s_{n-1}$ 是连续的，点 $y$ $F$ 的集合，其中满足不等式$\delta(y, y_0) < 2^{-n}$ 和$d(x_0, s_{n-1}(y)) < 2^{-n+1}$ 是$y_0$ 的开邻域。因此，在$E$中存在$F$的开覆盖$(V_i)_{i \in I}$和$F$的常数映射$s_{n,i}$，其中满足不等式（2）和（3）*在*$V_i$，其中一个替换 $s_n$ $s_{n,i}$。由于空间$F$是可度量的，因此存在单位元$(f_i)_{i \in I}$的连续划分，它是局部有限的并且从属于覆盖$(V_i)_{i \in I}$（GT，IX, § 4.5，th.4和§ 4.4，cor.1）。对于每个$y \in F$，放入$s_n(y) = \sum_{i \in I} f_i(y) \cdot s_{n,i}(y)$。 $E$中$F$的映射$s_n$是连续的；由于开球在 $E$ 和 $F$ 中是凸球，因此对于所有 $y \in F$，映射 $s_n$ 满足不等式 (2) 和 (3)。

从不等式 (3) 映射 $s_n : F \to E$ 形式到柯西序列，用于一致收敛。当$E$完备时，序列$(s_n)_{n \in \mathbf{N}}$均匀收敛到连续的映射$s : F \to E$（GT，X, § 1.6）； 公式(2)表明$u \circ s$是$F$的恒等映射，因此$s$是$u$的连续截面。

#### 推论 {#evt-ii-s4-n7-cor-1 .statement tag=07EZ}

*如果$F$中$L$是紧集，则$E$中存在紧集$K$，使得$u(K) = L$。*

放置$K = s(L)$就足够了，其中$s$是$u$的连续截面。

#### 注 {#evt-ii-s4-n7-rem-1 .statement tag=07F0}

— 1) 推论至支柱。也可以从 th 推出 12。 1 个 I、p. 17 和道具。 GT 18，IX, § 2.10。
2）我们保留道具的记号。 12. 令$p$为$E$的连续半范数；

对于所有$y \in F$，放入$q(y) = \inf_{u(x)=y} p(x)$，使得$q$是$F$（II，p. 4）上的连续半范数。令$\phi$为$\overline{\mathbf{R}}$的区间$]0, +\infty[$中$F$的下半连续映射。我们证明存在 u 的*连续截面 s，使得*$p \circ s < q + \phi$。

令$s_0$是$u$（命题12）的连续截面和$N$核的$u$。设$y_0 \in F$，则存在$z_0 \in N$使得$p(s_0(y_0) + z_0) < q(y_0) + \phi(y_0)$。 $F$ 中存在$y_0$ 的开邻域 $W$，使得$p(s_0(y) + z_0) < q(y) + \phi(y)$ 对于所有$y \in W$。因此，存在$F$的开覆盖$(W_i)_{i \in I}$和常数映射$t_i : F \to N$，使得$p(s_0(y) + t_i(y)) < q(y) + \phi(y)$适用于所有$y \in W_i$。由于$F$是可度量的，因此存在单位元的局部有限连续划分，它从属于覆盖$(W_i)_{i \in I}$，例如$(g_i)_{i \in I}$（GT，IX, § 4.5，th.4和§ 4.4，cor.1）。由$s(y) = s_0(y) + \sum_{i \in I} g_i(y) \cdot t_i(y)$定义的$E$中的$F$的映射$s$满足规定的条件。

### 习题 {#evt-ii-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
