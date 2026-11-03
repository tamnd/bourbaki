---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 0
section_title: Fixed points of groups of affine transformations
appendix: true
lang: zh
source: evt-i-v
pdf_pages: 0221-0229, 0254-0258
extraction: ocr
subsections:
    - "no": 1
      title: The case of solvable groups
      page: 0
      pdf_page: 221
    - "no": 2
      title: Invariant means
      page: 40
      pdf_page: 222
    - "no": 3
      title: Ryll-Nardzewski theorem
      page: 41
      pdf_page: 223
    - "no": 4
      title: Applications.
      page: 44
      pdf_page: 226
statements: 10
exercises: 8
content_sha256: 6d94423c653492ce19544bd0748c8155d95810b997d308b4fbe8c00d88a4771e
translated_from: content/en/evt/IV/A_a_fixed_points_of_groups_of_affine.md
translation_method: google
source_content_sha256: a3148232ea5c844b272b5847081786d07ced849332b19697c848a4c2a2b6e871
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: ec0ac385c45f5f8b3f11231592a431d1aa650c98f8dfbfbf4bd4d2ceb610be9d
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 附录
# 修复了仿射变换的点或群

### 1. 可解群的情况

设 E 为实数向量空间，K 为 E 的凸子集。映射 $u : K \to K$，这样对于 K 中的 $x, y$ 以及 $[0, 1]$ 中的每个实数 $t$，我们有

$$
u(t x + (1 - t) y) = t u(x) + (1 - t) u(y)
$$

被称为仿射变换。从关系 (1) 我们推出

$$
u \left( \sum_{i \in I} t_i x_i \right) = \sum_{i \in I} t_i u(x_i)
$$

对于 K 中的每个有限集合 I、点 $x_i$ 以及正实数 $t_i$，使得 $\sum_{i \in I} t_i = 1$。

令$u$和$v$为K上的两个仿射变换，则映射$u \circ v$为K上的仿射变换。如果$v : E \to E$为线性映射，则$v(K) \subset K$、映射$u : K \to K$其中重合 K 上的 $v$ 是仿射变换。

#### 定理 1（马尔科夫-角谷）{#evt-iv-a0-thm-1 .statement tag=07WI}

— *令 E 为在域 $\mathbf{R}$ 上的 Hausdorff 局部凸向量空间，K 为 E 的非空紧凸子集。令 $\Gamma$ 为 K 上连续仿射变换的集合，成对可置换。那么 K 中存在点 a，使得 $u(a) = a$ 对于所有 $u \in \Gamma$。*

对于每个$u \in \Gamma$，令$K_u$为所有$x \in K$中的集合，使得$u(x) = x$。我们将证明$K_u$非空。设$x$为K的点；对于每个整数$n \geq 1$，令$x_n$为E的元素$\frac{1}{n} \sum_{i=0}^{n-1} u^i(x)$。由于K在$u$、点$x_n$属于下是凸且稳定的，并且由于K是紧的，因此存在极限点$a$共序列$(x_n)_{n \geq 1}$。从K到E的映射$y \mapsto u(y) - y$是连续的，因而$u(a) - a$是序列$(u(x_n) - x_n)_{n \geq 1}$的极限点。但我们有$u(x_n) - x_n = \frac{1}{n} (u^n(x) - x)$。

由于 K 是紧致的，因此也是有界的（III，p. 3，道具 2），序列 $(u^n(x) - x)_{n \geq 1}$ 是有界的；因而，序列$\left( \frac{1}{n}(u^n(x) - x) \right)_{n \geq 1}$趋于0（III，p. 4，命题3），并且由于E是Hausdorff，所以我们有$u(a) - a = 0$。因而$a \in K_u$。

每个集合$K_u$都是紧空间K的闭凸子集，我们将证明交$\bigcap_{u \in \Gamma} K_u$非空。为此，只需证明，对于$n \geq 1$和$\Gamma$中的$u_1, ..., u_n$，集合$K_{u_1} \cap ... \cap K_{u_n}$非空即可。 $n = 1$的情况已经考虑完毕，我们通过归纳对$n$进行辩论。假设 $n \geq 2$ 并放入 $L = K_{u_1} \cap ... \cap K_{u_{n-1}}$。通过归纳的假设，L是E的非空紧凸子集。由于$u_n$与$u_1, ..., u_{n-1}$可交换，我们有$u_n(L) \subset L$。 应用证明的第一个部分到$u_n$在L上引起的仿射变换，我们结论在L中存在点$a$使得$u_n(a) = a$；然后$a$属于到$K_{u_1} \cap ... \cap K_{u_n}$，那么它是非空的。

#### 推论 {#evt-iv-a0-n1-cor-1 .statement tag=07WJ}

— *令 G 为 K 上连续仿射变换的可解群。则 K 中存在点，其在 G 下不变。*

通过可解群 (A, I, § 6, No. 4) 的定义，存在 G 的不同子群的有限递减序列 $(G_i)_{0 \leq i \leq n}$，使得 $G_0 = G$、$G_n = \{e\}$ 且群 $G_{i-1}/G_i$ 是*可交换的* $1 \leq i \leq n$。令$K_i$表示K中$G_i$的固定点的集合。然后是$K_n = K$。此外，对于$1 \leq i \leq n$，$G_i$诱导的每元素在$K_i$上进行恒等变换；因而，如果 $K_i$ 非空，我们就可以在 K 上推出阿贝尔的群 $G_{i-1}/G_i$ 的作用；由此可见。 1 $K_i$中$G_{i-1}/G_i$固定点的集合$K_{i-1}$非空。通过在 $i$ 上下降归纳，我们结论 $K_0$ 非空，因此推论。

### 2. 不变意味着

设X为拓扑空间。让$\mathscr{B}(X; \mathbf{R})$表示从X到$\mathbf{R}$的连续有界映射的实数向量空间由……组成。赋予范数$\|f\| = \sup_{x \in X} |f(x)|$，这是巴纳赫空间（GT，X, § 3, No. 1）；它也是一个有序的向量空间，其中关系$f \geq g$表示“$f(x) \geq g(x)$对于所有$x \in X$”。

#### 定义 1 {#evt-iv-a0-def-1 .statement tag=07WK}

*空间$\mathscr{B}(X; \mathbf{R})$上的正线性形式$\mu$，其中X是拓扑空间，其中$\|\mu\| = 1$称为X上的均值。*

\* 当 X 是紧致的时，X 上的均值是 X 上的正测度，使得 $\mu(X) = 1$。 \*

#### 引理 1 {#evt-iv-a0-lem-1 .statement tag=07WL}

*X上的平均值集合K是Banach空间$E = \mathscr{B}(X; \mathbf{R})$的对偶的单位球的子集，其元素是线性形式$\mu$使得$\mu(1) = 1$。它是 $E'$ 的子集，对于 $\sigma(E', E)$ 是凸且紧的。*

令 E 上的 $\mu$ 为线性形式，使得 $\mu(1) = 1$。对于每函数 $f \in E$，我们定义函数 $f' \in E$ $f'(x) = \|f\| - f(x)$ ($x \in X$)。首先假设$\mu$是均值；对于每个$f \in E$，我们有$f' \geq 0$，因而$\mu(f') \geq 0$，*即*$\mu(f) \leq \|f\|$；因而$\|\mu\| \leq 1$。

相反，假设$\mu$属于到$E'$，则$\| \mu \| \leq 1$；对于每个正数函数$f \in E$，我们有$\mu(f') \leq \| f' \|$，因而

$$
\| f \| - \mu(f) = \mu(f') \leq \| f' \| \leq \| f \|,
$$

最后$\mu(f) \geq 0$；因而，$\mu$是一个平均值。

显然$K$是凸的；从 cor 可以看出，$\sigma(E', E)$ 是紧致的。 3 个III、p. 17。

Q.E.D.

令$\Gamma$为从$X$到$X$的连续映射的集合，成对通勤。让$\gamma \in \Gamma$。对于每个函数 $f \in E$，我们有 $f \circ \gamma \in E$；因此我们可以对$X$上的均值集合$K$进行定义仿射变换$u_{\gamma}$，通过

$$
u_{\gamma} \mu(f) = \mu(f \circ \gamma) \quad (\mu \in K, f \in E).
$$

如果$K$由$\sigma(E', E)$诱导分配拓扑，映射$u_{\gamma}$是连续的。如果$\gamma$是同胚，$u_{\gamma} \mu$可以由$\mu$通过迁移或结构推出。最后，我们对$\Gamma$中的所有$\gamma, \gamma'$有$u_{\gamma} u_{\gamma'} = u_{\gamma' \gamma} u_{\gamma}$。由马尔科夫-卡库塔尼 th。 (IV, p. 39, th.1), *在$X$上存在一个均值$\mu$，使得$u_{\gamma} \mu = \mu$对于所有$\gamma \in \Gamma$；在其他字*中，对于$f \in E$和$\gamma \in \Gamma$，$\mu$满足关系$\mu(f) = \mu(f \circ \gamma)$。

类似地，th 的推论。 1 (IV, p. 40) 意味着以下结果：

#### 命题 1 {#evt-iv-a0-prop-1 .statement tag=07WM}

*设$X$为拓扑空间，$G$为可解群。我们假设$G$对左侧的$X$进行运算，这样对于所有$g \in G$，从$X$到$X$的映射$x \mapsto g.x$都是连续的。那么 $X$ 上存在一个均值，该均值在 $G$ 下不变。*

#### 推论 {#evt-iv-a0-n2-cor-1 .statement tag=07WN}

*设$G$为可解拓扑群。那么 $G$ 上存在一个均值，它在左平移和右平移下保持不变。*

应用 prop 就足够了。 1 到可解的群 $G \times G$ 通过 $(g.g').x = {gxg'}^{-1}$ 作用于 $G$。

### 3. 里尔-纳尔泽夫斯基定理

在本节中，$E$表示域$\mathbf{R}$和$\mathscr{T}$上的赋范*空间*，$E$上的Hausdorff局部凸拓扑，其中$E$的范数是*下半连续*。 这些假设在以下情况下尤其得到满足：

a) $\mathscr{T}$ 是由范数空间 $E$ 的范数引发的拓扑。
b) $\mathscr{T}$ 是规范化空间 $E$ 的弱化拓扑 $\sigma(E, E')$。
c) $E$ 是规范的空间 $F$ 和 $\mathscr{T} = \sigma(F', F)$ 的对偶。
d) 存在两个范数空间、$F_1$和$F_2$，使得$E = \mathscr{L}(F_1 ; F_2)$和$\mathscr{T}$是简单收敛的拓扑。

*除非另有明确说明，拓扑概念指拓扑$\mathscr{T}$。*

令 $K$ 为 $E$ 的凸子集。假设 $K$ 是紧致的（对于拓扑 $\mathscr{T}$），并且 $K$ 满足 $E$ 的范数定义的距离的第一个可数公理。

#### 引理 2 {#evt-iv-a0-lem-2 .statement tag=07WO}

假设$K$包含至少有两个点。对于每个$\varepsilon > 0$，存在$K$的划分分为两个非空子集$K_1$和$K_2$，具有以下性质：

a) $K_1$ 是凸且紧的；
b) $K_2$ 中的每个 $x_1$ 和 $x_2$ 都有 $\| x_1 - x_2 \| < \varepsilon$。

令$L$ 为$K$ 的所有极值点的集合的闭包。由克赖因-米尔曼 th。 (II,p. 55,第1),$K$是$L$的闭凸包络。由于$K$包含至少有两个点，$L$也是如此。对于每个$x \in L$，令$A_x$为所有$y \in L$中的集合，使得$\| x - y \| \leq \varepsilon / 4$。到假设，在$K$，存在$L$的可数子集$D$，使得$L = \bigcup_{x \in D} A_x$。由于范数是下半连续的，因此集合$A_x$都是闭集。 应用贝尔的第 3 次。 (GT, IX, § 5, No. 3, th. 1) 到紧空间 $L$，我们看到$D$中存在点$a$，$E$中存在开子集$U$，使得$L \cap U$为非空且包含在 $A_a$ 中。由于$L$包含至少有两个点，并且由于$E$是Hausdorff，因此我们可以通过$L \notin U$这样的方式来选择$U$。

令 $M$ 为$L \cap \complement U$ 的封闭凸包络。对于每个实数$t$使得$0 < t < 1$，令$M_t$为形式$tx_1 + (1 - t) x_2$的所有向量以及$x_1 \in M$和$x_2 \in K$的集合；这是一个非空、紧凑凸子集 $K$。我们将通过反证法证明$M_t \neq K$。假设$M_t = K$；那么$K$属于到$M_t$中的每个极值点$x$，因此可以用$x_1 \in M$和$x_2 \in K$写成形式$x = tx_1 + (1 - t) x_2$。这意味着$x = x_1 = x_2$，所以$x \in M$。作者：Krein-Milman th。 （II，p. 55，第1），我们有$K = M$，$K$是$L \cap \complement U$的封闭凸包络。通过II、p. 56、推论，这意味着$L \subset L \cap \complement U$，即与……矛盾关系$L \cap U \neq \varnothing$。

将 $d = \sup_{x \in K, y \in K} \| x - y \|$ 和选择实数 $t$ 使得 $0 < t < 1$ 和 $t < \varepsilon / 4d$。输入$K_1 = M_t$和$K_2 = K - M_t$。根据前面的论证，集合、$K_1$和$K_2$非空，$K_1$是凸紧的。令 $M'$ 为 $L \cap U$ 的封闭凸包络。由于$K$是集合$L = (L \cap \complement U) \cup (L \cap U)$的闭凸包络，因此它也是$M \cup M'$的闭凸包络。设$x_1$和$x_2$为$K_2$中的两个点；对于$i = 1, 2$，存在$y_i \in M$、$z_i \in M'$和实数$\alpha_i$，使得$0 \leq \alpha_i \leq 1$和$x_i = \alpha_i y_i + (1 - \alpha_i) z_i$。如果$\alpha_i \geq t$，那么
$$
x_i = t y_i + (1 - t) \left\{ \frac{\alpha_i - t}{1 - t} y_i + \frac{1 - \alpha_i}{1 - t} z_i \right\}
$$
;这个与……矛盾假设那个$x_i \notin M_i$。因此$\alpha_i < t$，对于$i = 1, 2$，等等
$$
\| x_i - z_i \| = \| \alpha_i (y_i - z_i) \| = \alpha_i \| y_i - z_i \| \leq \alpha_i d < dt < \varepsilon / 4 .
$$
对于$M'$中的每个点$z$，我们有$\| z - a \| \leq \varepsilon / 4$，从$L \cap U \subset A_a$开始，所以，特别是$\| z_i - a \| \leq \varepsilon / 4$。因此
$$
\| x_1 - x_2 \| \leq \sum_{i=1}^2 (\| x_i - z_i \| + \| z_i - a \|) < \varepsilon .
$$
这样就完成了证明。

#### 引理 3 {#evt-iv-a0-lem-3 .statement tag=07WP}

设 G 为 K 上连续（对于 $\mathscr{T}$）仿射变换的群。假设 K 非空，并且对于 K 中的所有 x、y 和 G 中的所有 g 都有 $\|gx - gy\| = \|x - y\|$。则 K 中存在点，它在 G 下是不变的。

令$\mathfrak{J}$为K的非空子集族，对于G来说是闭凸且稳定的。如果$(L_\alpha)_{\alpha \in I}$是$\mathfrak{J}$的元素族，且按包含全序，则集合$L = \bigcap_{\alpha \in I} L_\alpha$属于到$\mathfrak{J}$。因而（S，III, § 3, No. 4，th.2），$\mathfrak{J}$中存在元素L，这对于包含关系来说是最小的。我们将证明L约化到点。

我们通过反证法进行论证，假设L包含至少有两个不同的点$x_1$和$x_2$，放入$x = (x_1 + x_2)/2$和$\varepsilon = \|x_1 - x_2\|/2$。凸和紧集 L 满足由范数 (GT, IX, § 2, No. 8) 定义的距离的第一可数公理。因而，我们可以应用引理 2 并找到L的紧凑且凸的子集$L_1$，与$\varnothing$和L不同，具有以下性质：

(A) *对于$L - L_1$中的每个$y_1$和$y_2$，我们有$\|y_1 - y_2\| < \varepsilon$。*

*我们将通过反证法证明$gx \in L_1$对于所有$g \in G$。*令$g \in G$使得$gx \in L - L_1$那么我们有

$$
\|gx_i - gx\| = \|x_i - x\| = \|x_1 - x_2\|/2 = \varepsilon ,
$$

$i = 1, 2$。到性质 (A)，我们有$gx_i \in L_1$。由于$L_1$是凸的，我们将结论从$gx = (gx_1 + gx_2)/2$属于到$L_1$，即与……矛盾假设。

令 $L'$ 为 x 的轨道 $Gx$ 的闭凸包络。 集合$L'$属于至$\mathfrak{J}$。根据前面的论证，我们有$L' \subset L_1$，因此有$L' \subset L, L' \neq L$。这样与……矛盾L和证明的最小特征标就完成了。

#### 定理 2（里尔-纳尔泽夫斯基）{#evt-iv-a0-thm-2 .statement tag=07WQ}

— *令 E 为赋范空间，K 为 E 的非空凸子集，对于弱化的拓扑 $\sigma(E, E')$ 是紧致的。设G为K的等距仿射变换的群，则K中存在点，其在G下不变。*

对于每个$g \in G$，令$K_g$表示K中所有点x中的集合，使得$gx = x$；令 K 被指定为弱化的拓扑；每个集合$K_g$在紧致空间K中都是凸且闭的。我们将证明交$\bigcap_{g \in G} K_g$非空；为此，只需证明对于G中的每个$g_1, ..., g_n$来说集合$K_{g_1} \cap ... \cap K_{g_n}$非空即可。固定$g_1, ..., g_n$并令H为$\{ g_1, ..., g_n \}$生成的G的子群。 K 中的选择点 a，令 L 表示 a 的轨道 Ha 的闭凸包络。令 D 为形式 $\lambda_1 h_1 a + \cdots + \lambda_m h_m a$ 的元素的可数集合，其中 $\lambda_1, ..., \lambda_m$ 是正有理数数，使得 $\lambda_1 + \cdots + \lambda_m = 1$ 和 $h_1, ..., h_m$ 是 H 中的元素。 D 的 $\overline{D}$ 对于强拓扑是凸的，因此它对于 $\sigma(E, E')$ 是封闭的（IV，p. 4，道具 2）；因而$\overline{D} = L$，这证明L是一个度量空间满足距离$(x, y) \mapsto \|x - y\|$的第一个可数公理。现在我们可以应用引理 2。L中存在点 b，它在H下是不变的，因而$b \in K_{g_1} \cap ... \cap K_{g_n}$。

#### 推论 {#evt-iv-a0-n3-cor-1 .statement tag=07WR}

— 令 E 为自反 Banach 空间，赋模空间 E 的自同构的 G 群，以及 E 的 K 子集。假设 K 在 G 下非空、凸、闭、有界且稳定。则 K 中存在点，其在 G 下不变。

由于 E 是自反的，因而 K 对于 $\sigma(E, E')$ (IV, p. 15, th. 1) 是紧致的。此外，G属于到$\mathscr{L}(E)$的每个元素。

### 4. 应用。

\* A) 表示群 ：
令 E 为复希尔伯特空间、G 群和 $\pi$ E 上 G 的酉表示，即同态从 G 到 E 的自同构的群。令 $E^G$ 为希尔伯特所有向量的E由……组成的子空间在$\pi(G)$下不变。对于每个 $x \in E$，令 $K_x$ 为 x 的轨道的闭凸包络。修复 E 中的点 x。

我们将证明$K_x$中存在唯一的点，它在$\pi(G)$下不变，即x在$E^G$上的投影。通过IV、p. 44、推论（应用于底层实数向量空间到E），$K_x$中存在点，在$\pi(G)$下不变；令 a 为点；然后$a \in E^G$。令 P 为所有 $y \in E$ 的集合，使得 $y - x$ 与 $E^G$ 正交；我们立即看到 P 在 $\pi(G)$ 下是闭的、凸的且不变的；因而$x \in P$，因而$K_x \subset P$，最后$a \in P$。在其他字中，$a - x$与$E^G$正交；因而 a 是 x 到 $E^G$ 的投影。 \*

\* B) 希尔伯特空间中运算符的踪迹：
假设表示$\pi$是不可约的，即不存在E的希尔伯特子空间，不同于$\{0\}$和E，它在$\pi(G)$下不变。令 $F = \mathscr{L}^2(E)$ 为 E 的所有 Hilbert-Schmidt 自同态的希尔伯特空间，标量为乘积 $\langle u|v \rangle = \operatorname{Tr}(u^*v)$。我们定义一个酉表示$\lambda$从G通过公式进入F

$$
\lambda(g).u = \pi(g)\ u\pi(g)^{-1} \quad (u \in F,\ g \in G)
$$

$\lambda(G)$ 下 E 不变量的所有元素的空间 $F^G$ 由 E 的希尔伯特-施密特自同态 $u$ 组成，对于所有 $g \in G$ 与 $\pi(g)$ 交换。根据 Schur 的引理，这样的 $u$ 就是位似。因此我们必须考虑两种情况：
1) 如果 E 是无限维的，则 $F^G = \{0\}$；
2) 如果 E 是有限维的，则 $F = \mathscr{L}(E)$ 和 $F^G = \mathbf{C}.1_E$。

将A)的结果应用代入酉表示$\lambda$，我们得到以下定理：

设$u \in \mathscr{L}^2(E)$，并令$A_u$为E的自同态$\pi(g)\ u\pi(g)^{-1}$的集合的$\mathscr{L}^2(E)$的闭凸包络，其中g穿过G。如果E是无限维的，则我们有$0 \in A_u$。如果E是维数d的有限维，则$A_u$中存在唯一的位似，即u的投影$\frac{1}{d}\ \operatorname{Tr}(u).\ 1_E$到$\mathscr{L}^2(E)$的子空间$\mathbf{C}.1_E$。 \*

C) 紧凑群的哈尔测度：

设 G 为紧群，并令 E = $\mathscr{C}(G, \mathbf{R})$ 为 G 上所有实值连续函数的 Banach 空间，赋予范数

$$
\| f \| = \sup_{x \in G} |f(x)| .
$$

对于所有 $x \in G$，我们将 E 的定义自同构 $\gamma_x$ 和 $\delta_x$ 乘以公式

$$
\gamma_x f(y) = f(x^{-1}y) , \quad \delta_x f(y) = f(yx)
$$

（$y \in G,\ f \in E$）。

*令$f \in E$、$\Gamma_f$（或$\Delta_f$）表示封闭凸包络i。当 x 范围大于 G 时，所有函数 $\gamma_x f$（或 $\delta_x f$）中的集合的 E。我们将证明存在唯一常数函数 $\mu(f)$ 属于到 $\Gamma_f$，唯一常数函数 $\mu'(f)$ 属于到 $\Delta_f$，并且这些常数相等。*

很明显，G 上的连续函数在 E 的自同构 $\gamma_x$（或 $\delta_x$）下是不变的当且仅当它是常数。现在，G 中 x 的所有函数 $\gamma_x f$（分别为 $\delta_x f$）中的集合在 E 中是紧致的，因为从 G 到 E 的映射 $x \mapsto \gamma_x f$（分别为 $x \mapsto \delta_x f$）是连续的（GT，X, § 3, No. 4，第 3 个）。由此可见（II，p. 25，命题 3），对于由范数定义的拓扑，$\Gamma_f$（分别为 $\Delta_f$）在 E 中为紧集，因此对于 $\sigma(E, E')$。作者：Ryll-Nardzewski。 （IV，p. 43，第2），$\Gamma_f$和$\Delta_f$存在常数函数。尚待证明，如果$c_1 \in \Gamma_f$和$c_2 \in \Delta_f$是常数，则$c_1 = c_2$。

让$\varepsilon > 0$。到假设时，G 中存在点 $x_1, ..., x_n,\ y_1, ..., y_n$ 且正实数 $\lambda_1, ..., \lambda_n,\ \mu_1, ..., \mu_m$ 使得

$$
\lambda_1 + \cdots + \lambda_n = \mu_1 + \cdots + \mu_m = 1 .
$$
$$
\sup_{x \in G} \left| \sum_{i=1}^n \lambda_i f(x_i x) - c_1 \right| \leq \varepsilon ,
$$
$$
\sup_{x \in G} \left| \sum_{j=1}^m \mu_j f(xy_j) - c_2 \right| \leq \varepsilon .
$$

输入$r = \sum_{i,j} \lambda_i \mu_j f(x_i y_j)$。然后$r - c_1 = \sum_{j=1}^m \mu_j a_j$与$a_j = \sum_{i=1}^n \lambda_i f(x_i y_j) - c_1$；根据 (7)，我们有 $|a_j| \leq \varepsilon$ 对应 $1 \leq j \leq m$，因此有 $|r - c_1| \leq \varepsilon$。同样，我们证明不等式$|r - c_2| \leq \varepsilon$，因此$|c_1 - c_2| \leq 2\varepsilon$。由于 $\varepsilon$ 是任意的，因此我们得到 $c_1 = c_2$，正如断言的那样。

通过$\mu(f)$的定义，对于每个$\varepsilon > 0$，我们可以在G中找到正的数$\lambda_1, ..., \lambda_n$，其中和1和元素$x_1, ..., x_n$，使得$\left| \sum_{i=1}^n \lambda_i f(x_i x) - \mu(f) \right| \leq \varepsilon$对于所有$x \in G$。

直接的对于E中的$f, g$和每个标量$\lambda$，我们有$\Gamma_{f+g} \subset \Gamma_f + \Gamma_g$和$\Gamma_{\gamma f} = \lambda \Gamma_f$，因此我们有关系$\mu(f+g) = \mu(f) + \mu(g)$和$\mu(\lambda f) = \lambda \mu(f)$。因此，从 E 到 $\mathbf{R}$ 的映射 $\mu : f \mapsto \mu(f)$ 是紧致空间 G (IV, p. 40) 上的平均值； *在其他情况下，字$\mu$是G上的正测度，使得$\mu(G) = 1$*。

$\mu$在$G$的左平移下不变是直接的，等式$\mu(f) = \mu'(f)$意味着$\mu$在右平移下也是不变的。 \* 在其他字中，$\mu$ 是 $G$ 上的左度量和右度量（INT，VII, § 1, No. 2，定义 2）。 \*

*D) 不变测度的存在：

令$X$为豪斯多夫拓扑空间，$\mu$为$X$的正有界测度，$G$群为$X$的同胚。假设对于所有$g \in G$，映射$g : X \to X$下$\mu$的测度$g.\mu$、像为基$\mu$。令$u_g$为$X$上的$\mu$可积正函数，使得$g.\mu = u_g.\mu$。还假设$X$上存在两个正的$\mu$、可积函数、$\phi$和$\psi$，它们不是$\mu$-空，并且使得$\phi \leq u_g \leq \psi$$\mu$-对于所有$g \in G$来说几乎无处不在。我们将证明$X$上存在正有界测度$\nu \neq 0$，其中基$\mu$，且在$G$下不变。

令 $P$ 为 Banach 空间 $E = L^1(X, \mu)$ 的子集，该空间由函数类 $f$ 组成，使得 $\phi \leq f \leq \psi$ $\mu$ 几乎无处不在。 那么$P$对于弱化的拓扑$\sigma(E, E')$来说是紧致的。 从$P$到$X$上有界实测度的巴拿赫空间$F = \mathscr{M}^b(X)$的映射$h \mapsto h.\mu$，是从$P$到$E$的子集$P_1$的双射，对于拓扑$\sigma(F, F')$来说是凸且紧的。 由假设，$g.\mu \in P_1$ 为所有 $g \in G$。 令$K$为所有测度$g.\mu$的集合的封闭凸包络。 对于所有$g \in G$，映射$\nu \mapsto g.\nu$是$K$的等距仿射变换。 作者：Ryll-Nardzewski。 (IV,p. 43,th.2)，存在一个测度$\nu \in K$，它在$G$下不变。 我们有$\phi.\mu \leq \nu$，因此有$\nu \neq 0$。 \*

习题

### 习题{#evt-iv-a0-exercises}

参见[习题附录 0](exercises/a0/)。
