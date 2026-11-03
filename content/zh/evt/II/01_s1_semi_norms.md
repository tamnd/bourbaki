---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 1
section_title: Semi-norms
lang: zh
source: evt-i-v
pdf_pages: 0038-0044
extraction: ocr
subsections:
    - "no": 1
      title: Definition of semi-norms
      page: 0
      pdf_page: 38
    - "no": 2
      title: Topologies defined by semi-norms
      page: 2
      pdf_page: 39
    - "no": 3
      title: Semi-norms in quotient spaces and in product spaces
      page: 4
      pdf_page: 41
    - "no": 4
      title: Equicontinuity criteria of multilinear mappings for topologies defined by semi-norms
      page: 5
      pdf_page: 42
statements: 15
exercises: 0
content_sha256: 61df56095df14fa074a4f3cfd430fa2b4cdbf1cbaa36c31c81f5657bcaf048ff
translated_from: content/en/evt/II/01_s1_semi_norms.md
translation_method: google
source_content_sha256: 99701b6427e2fc51eea6f3f407ebff4fb20d627e99dfd31c75d611b17f9e8d84
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 2a818d469f9cb2ecd32c9c94938859bf49cdd2370d37e906c81abdb4fea3ae9c
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 1。半范数

在本段中，$\mathbf{K}$表示非离散值除法环。

### 1. 半范数定义

#### 定义 1 {#evt-ii-s1-def-1 .statement tag=07AP}

令 E 为左向量空间超过 $\mathbf{K}$。 $\mathbf{R}_+ = \{ 0, + \infty \}$ 中 E 的映射 $p$，如果满足以下公理，则称为 E 上的半范数：
(SN_I) 如果$x \in \mathrm{E}$和$\lambda \in \mathbf{K}$则$p(\lambda x) = |\lambda| \, p(x)$。
(SN_II) 如果 $x \in \mathrm{E}$ 和 $y \in \mathrm{E}$ 那么 $p(x + y) \leq p(x) + p(y)$。

由于$p(x) \leq p(y) + p(x - y)$和$p(y) \leq p(x) + p(y - x)$，从$p(y - x) = p(x - y)$，我们推出
$$
|p(x) - p(y)| \leq p(x - y) .
$$

#### 例 1 {#evt-ii-s1-n1-exa-1 .statement tag=07AQ}

E 上的范数是半范数 $p$，因此关系 $p(x) = 0$ 意味着 $x = 0$ (I, p. 3)。

#### 例 2 {#evt-ii-s1-n1-exa-2 .statement tag=07AR}

对于 E 上的每个线性形式 $f$，函数 $x \mapsto |f(x)|$ 是 E 上的半范数。

#### 例 3 {#evt-ii-s1-n1-exa-3 .statement tag=07AS}

如果 $p_i (1 \leq i \leq n)$ 是 E 上半范数的有限集合，则显然 $p'(x) = \sup_{1 \leq i \leq n} p_i(x)$
和$p''(x) = \sum_{i=1}^n \alpha_i p_i(x)$（其中$\alpha_i$是$\geq 0$）都是E上的半范数。

如果满足 (SN$_I$) 和以下公理，则 $\mathbf{R}_+$ 中 E 的映射 $p$ 被称为*超半范数*：

(SN$_{II}'$) *如果$x \in E$和$y \in E$，则$p(x + y) \leq \sup(p(x), p(y))$。*

显然，超半范数就是半范数。

说 K 上的绝对值是*超度量*（CA，VI, § 6.2）意味着它是左向量空间 $K_s$ 上的超半范数，与零不同。

#### 命题 1 {#evt-ii-s1-prop-1 .statement tag=07AT}

*设 E 为 K 上的左拓扑向量空间，并令 p 为 E 上的半范数。以下条件是等价的：*
  *a)* *p 在 E 中连续。*
  *b)* *p 在点 0 处连续。*
  *c)* *p 是一致连续的。*
  *d)* *对于每个实数 $\alpha > 0$、集合 W(p, $\alpha$)，其中 $x \in E$ 的 $p(x) < \alpha$ 在 E 中打开。*
  *e)* *存在实数$\alpha > 0$，使得W(p, $\alpha$)在E中为0的邻域。*
  *f)* *对于每个实数 $\alpha > 0$、集合 V(p, $\alpha$)，其中 $x \in E$ 的$p(x) \leq \alpha$，在 E 中邻域为 0。*

事实上，c) $\Rightarrow$ a) $\Rightarrow$ b) $\Rightarrow$ d) $\Rightarrow$ e) $\Rightarrow$ f) $\Rightarrow$ c) 立即从 (SN$_I$) 和不等式 (1) 得出。

#### 推论{#evt-ii-s1-n1-cor-1 .statement tag=07AU}

*如果 p 是 E 上的连续半范数，q 是满足 $q \leq p$ 的半范数，则 q 在 E 上连续。*

当 p 是 E 上的*超半范数*时，则集合 W(p, $\alpha$) 和 V(p, $\alpha$) *既开又闭*。因为，我们已经看到 W(p, $\alpha$) 是开集；另一方面，如果 z 是 W(p, $\alpha$) 的簇点，则存在$y \in W(p, \alpha)$使得 $p(y - z) < \alpha$，并且从 (SN$_{II}'$) 我们有 $p(z) < \alpha$，因此 W(p, $\alpha$) 是闭集。另外，V(p, $\alpha$) 是闭集，因为 p 是连续的；进一步如果$p(x) \leq \alpha$和$p(y) \leq \alpha$，则$p(x + y) \leq \alpha$乘以(SN$_{II}'$)，这表明V(p, $\alpha$)是开放的。

### 2. 由半范数定义的拓扑

令 p 为 K 上向量空间 E 的半范数；对于每个 $\alpha > 0$ 令 V(p, $\alpha$) 为 E 中 $p(x) \leq \alpha$ 的那些 x 的子集。显然，如果$x \in V(p, \alpha)$和$\lambda \in K$使得$|\lambda| \leq 1$，那么$\lambda x \in V(p, \alpha)$，在其他字V（p，$\alpha$）中是*平衡的*。此外，对于每个$x_0 \in E$，都存在一个非零标量$\mu \in K$，使得$|\mu| \geq p(x_0) \alpha^{-1}$，因此$\mu^{-1} x_0 \in V(p, \alpha)$，也就是说V（p，$\alpha$）是*吸收性*。最后，从(SN$_{II}$)，我们有$V(p, \alpha/2) + V(p, \alpha/2) \subset V(p, \alpha)$，从(SN$_I$)，对于K中的每个非零标量$\lambda$，我们有$\lambda V(p, \alpha) = V(p, |\lambda| \alpha)$。我们从这些注、I、p. 7、道具中获得结论。 4、当$\alpha$在数$> 0$的集合内变化时（或仅在严格正数数的序列趋于0时），则集合V(p, $\alpha$)构成基本0 的邻域系统拓扑与 E 的向量空间结构兼容；我们说这个拓扑 *由半范数 p* 定义。具有这样的拓扑的向量空间E被称为*半范数空间*。请注意，如果 W(p, $\alpha$) 是 E 的 x 的子集，使得 $p(x) < \alpha$，则 W(p, $\alpha$) 构成（其中 $\alpha > 0$ 或 $\alpha$ 以数的严格正值序列变化，趋向于零) 对于由$p$定义的拓扑，邻域的基本系统为0。

如果$\Gamma$是$E$上半范数的集合，则半范数$p \in \Gamma$定义的拓扑的*上界*与向量空间结构兼容（I，p. 10，cor.4）。对于拓扑，邻域的基本系统为 0，由有限交 $\bigcap_i V(p_i, \alpha_i)$ 给出，其中 $p_i \in \Gamma$ 和 $\alpha_i > 0$。这个拓扑据说是*由半范数的集合定义的*$\Gamma$。它是 $E$ 上*粗略的* 拓扑，其中在所有翻译下都保持不变，并且半范数 $p \in \Gamma$ 是连续的。

设$E$是$K$上的拓扑向量空间：$E$上半范数的系统，比如说$\Gamma$，被称为半范数的*基本系统*，如果拓扑在$E$上与$\Gamma$定义的拓扑相同。

令$E$为向量空间超过$K$，拓扑由半范数$\Gamma$的集合定义。对于每个半范数$p$，我们有$p(x - z) \leq p(x - y) + p(y - z)$，这表明函数$(x, y) \mapsto p(x - y)$是$E$（GT，IX, § 1.1）上的*伪计量*：从定义得出，当$p$在$\Gamma$变化时，这些伪度量的集合定义拓扑向量空间$E$的统一结构。

#### 注 {#evt-ii-s1-n2-rem-1 .statement tag=07AV}

— 1) 拓扑由 $E$ 上半范数 $p_i$ ($1 \leq i \leq n$) 的*有限* 集合定义，可以由*单个*半范数 $p = \sup_{1 \leq i \leq n} p_i$ 定义。但拓扑由半范数不能的无限集合定义，通常由单个半范数定义（III，p. 37，练习2）。

2) 设$(\mathscr{T}_i)_{i \in I}$为向量空间$E$超过$K$的拓扑族，每个拓扑族都由半范数族$\Gamma_i$定义。那么半范数$\Gamma = \bigcup_{i \in I} \Gamma_i$的集合定义的拓扑就是拓扑$\mathscr{T}_i$的上界。

3) 如果$\Gamma_0$是半范数的集合*由递增*序关系定义，定义在$E$上的两个半范数$p, q$之间，通过«存在$\lambda > 0$使得$p \leq \lambda q$»，那么基本的系统为对于由 $\Gamma_0$ 定义的拓扑，0 的邻域是通过取集合 $V(p, \alpha)$ 获得的，其中 $p \in \Gamma_0$ 和 $\alpha > 0$。如果$\Gamma$是$E$上的任何半范数集合，则半范数的过滤集合（定义与$\Gamma$相同的拓扑）是所有有限半范数族的上包络的集合$\Gamma_0$ 属于至 $\Gamma$。

4) 即使超过$K$不能的拓扑向量空间的$K = \mathbf{R}$、拓扑始终由半范数的集合定义(*cf.* II、p. 24， 推论）。

#### 例 {#evt-ii-s1-n2-exa-1 .statement tag=07AW}

— 令 $\mathscr{C}^\infty(\mathbf{R})$ 为向量空间超过 $\mathbf{R}$ 的实值函数，其在 $\mathbf{R}$ 中无限可微。对于函数和整数$n \geq 0$、$m \geq 1$的每个对，将

$$
p_{n,m}(f) = \sup_{-m \leq t \leq m} |f^{(n)}(t)|
$$

与$f^{(0)} = f$。显然$p_{n,m}$是$\mathscr{C}^\infty(\mathbf{R})$的半范数。在阶中，函数$f_\alpha$趋于0（在指标的集合上过滤$\mathfrak{F}$），在$\mathscr{C}^\infty(\mathbf{R})$中，拓扑$\mathscr{T}$由半范数定义$p_{n,m}$，对于所有整数$n \geq 0$，函数$f_\alpha^{(n)}$趋于0（在$\mathfrak{F}$之后）*均匀地在*$\mathbf{R}$的每个紧凑子集上是必要且充分的。我们说$\mathscr{T}$是函数*$f \in \mathscr{C}^\infty(\mathbf{R})$*及其所有导数*（*cf.*III，p. 9）的紧致收敛*拓扑。

#### 命题 2 {#evt-ii-s1-prop-2 .statement tag=07AX}

*在向量空间* $E$，*令* $\mathscr{T}$ *由半范数* $\Gamma$ 的集合定义为拓扑。

(i) *E 中 {0} 的闭包，对于 $\mathscr{T}$，是 $x \in E$ 的子集，其中 $p(x) = 0$ 对于每个半范数 $p \in \Gamma$。*

(ii) *如果 $\mathscr{T}$ 是 Hausdorff 并且 $\Gamma$ 可枚举，则 $\mathscr{T}$ 是可度量的。*

命题紧随定义和 GT，IX, § 2 。 4，科尔。 1.

请注意，如果$\mathscr{T}$是可度量的，则$\mathscr{T}$不能可能由单个范数定义；上面给出的例就是这种情况（*cf.* IV、p. 18、*例 4*）。

令 E 为 K 上的向量空间，其中拓扑由半范数 $\Gamma$ 的集合定义。令 $\hat{E}$ 为 E (I, p. 6) 的豪斯多夫完成，$\hat{\Gamma}$ 为 $\mathbf{R}_+$ 中 $\hat{E}$ 的集合映射 $\hat{p}$，其中 $p$ 在 $\Gamma$ 中变化 (GT, II, § 3 7，道具 15）。通过扩展不等式的原理，函数$\hat{p} \in \hat{\Gamma}$是$\hat{E}$的半范数，以及定义$\hat{E}$的统一结构的伪度量的函数$\hat{p}(x - y)$形式集合（GT， IX, § 1 3，道具 1)。因此，我们看到$\hat{\Gamma}$是定义$\hat{E}$的拓扑的半范数的基本集合。

### 3. 商空间和乘积空间中的半范数

设E是K上的拓扑向量空间，其拓扑由半范数$\Gamma$、集合定义。显然，E 的 $\Gamma$ 到向量子空间 M 的半范数限制，由 E 的半范数在 M 上导出定义拓扑。

令 $\phi$ 为 E 在向量商空间 E/M 上的典范映射。我们证明，对于 E 上的每个半范数 $p$，函数

$$
\dot{p}(z) = \inf_{\phi(x) = z} p(x)
$$

是 E/M 的半范数。事实上，显然$\dot{p}$满足条件(SN$_1$)；另一方面，如果$z', z''$是E/M的两个向量，我们有：

$$
\begin{align*}
\inf_{\phi(x) = z' + z''} p(x) &\leq \inf_{\phi(x') = z', \phi(x'') = z''} p(x' + x'') \\
&\leq \inf_{\phi(x') = z', \phi(x'') = z''} (p(x') + p(x'')) \\
&= \inf_{\phi(x') = z'} p(x') + \inf_{\phi(x'') = z''} p(x'')
\end{align*}
$$

这表明$\dot{p}$验证了(SN$_2$)。我们说$\dot{p}$是M对$p$的*商半范数*。

同样的推理证明，如果$p$是*超半范数*，那么$\dot{p}$也是。

既然如此，我们有（在No. 2的记号）

$$
\phi(\mathrm{W}(p, \alpha)) = \mathrm{W}(\dot{p}, \alpha)
$$

对于每个$\alpha > 0$。事实上，说$\dot{p}(z) < \alpha$，意味着存在$x \in E$，使得$\phi(x) = z$和$p(x) < \alpha$，由此得出关系(4)。

由此我们推断，如果半范数$\Gamma$的集合是*有向*（II，p. 3，*注3*），那么$E/M$上的商拓扑由半范数集合定义$\dot{p}$，当$p$在$\Gamma$变化时。

如果$N$是$E$中$\{0\}$的闭包，$E/N$的拓扑由商半范数$\dot{p}$定义，其中$p$在$\Gamma$中变化（即使$\Gamma$没有被过滤）：这里每 $x$ 属于至类 $\dot{x} \mod N$ $\dot{p}(\dot{x}) = p(x)$。请注意，$E/N$正是与$E$（I，p. 4）关联的Hausdorff 空间。

令$E$是$K$上的向量空间，$(E_i)_{i \in I}$是向量空间在$K$上的族，其中$E_i$有拓扑$\mathscr{T}_i$由半范数集合定义$\Gamma_i$。对于每个$i \in I$，令$f_i$为$E_i$中$E$的线性映射；显然，当$p_i$在集合$\Gamma_i$变化时，$E$的半范数$p_i \circ f_i$形式集合$\Gamma'_i$。 $E$上的拓扑$\mathscr{T}$，定义为使所有映射$f_i$连续（I，p. 9）的最粗糙的，然后由半范数$\Gamma' = \bigcup_{i \in I} \Gamma'_i$的集合定义，这来自$\mathscr{T}$ 的定义或邻域为 0（GT，I, § 2.3，道具 4）。

如果$p_i$是超半范数，那么$p_i \circ f_i$也是超半范数。

令$E$为向量空间超过$K$，其中拓扑$\mathscr{T}$由半范数族$(p_i)_{i \in I}$定义；对于每个$i \in I$，让$\mathscr{T}_i$是由单个半范数$p_i$定义的拓扑，并用使用拓扑$\mathscr{T}_i$从$E$获得的$E_i$空间表示。那么拓扑 $\mathscr{T}$ 是逆像通过乘积拓扑在 $\prod_{i \in I} E_i$ 上的对角线映射 $\Delta : E \to \prod_{i \in I} E_i$（I，p. 9，道具 7）。对于每个$i \in I$，将$E_i$中$\{0\}$的闭包写成$N_i$，并通过$F_i = E_i / N_i$，由范数$p_i$相应的到$p_i$定义*范数*空间 (II、p. 4、公式(3))；如果$\phi_i : E_i \to F_i$是典范映射并且$\phi : (x_i) \mapsto (\phi_i(x_i))$乘积映射，我们知道$\prod_{i \in I} E_i$上的乘积拓扑是逆像乘以乘积的$\phi$ $\prod_{i \in I} F_i$ 上的拓扑（GT，II, § 3.9，道具 18）。因此，拓扑$\mathscr{T}$是逆像在$\prod_{i \in I} F_i$上的乘积拓扑的复合映射$\phi \circ \Delta$。特别是，如果 $\mathscr{T}$ 是 *Hausdorff* 那么它是从 II，p. 3，道具得出的。 2 映射 $\phi \circ \Delta$ 是*内射*，因此：

#### 命题 3 {#evt-ii-s1-prop-3 .statement tag=07AY}

*每个豪斯多夫拓扑向量空间* $E$ *超过* $K$，*其拓扑由半范数集合定义，同构于Banach 空间*的乘积子空间。

此外，如果 $E$ 的拓扑由半范数的*可枚举* 集合定义，则 $E$ 是*可度量*（I，p. 16）。

### 4. 对于由半范数定义的拓扑，多线性映射的等连续性判据

#### 命题 4 {#evt-ii-s1-prop-4 .statement tag=07AZ}

*设* $E_i$ ($1 \leq i \leq n$) *和* $F$ *拓扑向量空间超过* $K$； *我们假设，对于每个* $i$，* $E_i$ *的拓扑 *由半范数* $\Gamma_i$的有向集合定义，*并且* $F$ *的拓扑由半范数的集合定义* $\Gamma$。 *然后集合* $H$，*of* $\prod_{i=1}^n E_i$ 的多线性映射在 F 中是等连续的当且仅当，对于每个半范数 $q \in \Gamma$ 和每个指标 i，存在一个半范数 $p_i \in \Gamma_i$，并且数$a > 0$，这样对于每个函数$u \in \mathbf{H}$和点$(x_i) \in \prod_{i=1}^n E_i$，

$$
q(u(x_1, x_2, ..., x_n)) \leq a \cdot p_1(x_1)\ p_2(x_2) ... p_n(x_n) .
$$

条件是足够的，因为它意味着 H 在 (0, 0, ..., 0) 处等连续，因此在任何地方 (I, p. 9, 命题 6)。

我们证明条件是必要的。到假设，对于每个半范数$q \in \Gamma$和每个数$\beta > 0$，对于每个函数$u \in \mathbf{H}$，我们有$q(u(x_1, x_2, ..., x_n)) \leq \beta$，前提是$p_i(x_i) \leq \alpha_i$对于每个指标$i$、$1 \leq i \leq n$和某些适当选择数$\alpha_i > 0$和半范数$p_i \in \Gamma_i$。由于 K 是非离散的，我们还可以假设，对于每个 $i$，我们有 $\alpha_i = |\lambda_i| < 1$，其中 $\lambda_i \in \mathbf{K}$。然后令$(x_1, x_2, ..., x_n)$为$\prod_{i=1}^n E_i$中的任意点，对于每个指标$i$，令$m_i \in \mathbf{Z}$为整数，使得$p_i(x_i) \leq |\lambda_i|^{m_i + 1}$；这可以写成 $p_i(\lambda_i^{-m_i} x_i) \leq |\lambda_i|$ ($1 \leq i \leq n$)，因此，通过假设，我们有

$$
q(u(x_1, x_2, ..., x_n)) \leq \beta |\lambda_1|^{m_1} |\lambda_2|^{m_2} ... |\lambda_n|^{m_n} .
$$

首先假设$p_i(x_i)$中的一个是零，那么我们可以取任意大的$m_i \in \mathbf{N}$，因此$q(u(x_1, x_2, ..., x_n)) = 0$。相反，如果所有$p_i(x_i)$都是$\neq 0$，则取整数$m_i$，使得每个$i$都有$|\lambda_i|^{m_i + 2} < p_i(x_i) \leq |\lambda_i|^{m_i + 1}$；那么我们有 $|\lambda_i|^{m_i} < |\lambda_i|^{-2} p_i(x_i)$，根据 (6)，关系 (5) 如下

$$
a = \beta (|\lambda_1| \cdot |\lambda_2| ... |\lambda_n|)^{-2} .
$$

Q.E.D.

#### 推论 {#evt-ii-s1-n4-cor-1 .statement tag=07B0}

— *集合 H 是等连续的，当且仅当对于每个半范数 $q \in \Gamma$，$\prod_{i=1}^n E_i$ 中存在 0 的邻域，其中函数 $q \circ u$，对于 $u \in \mathbf{H}$，是一致有界的。*

条件显然是必要的，道具的演示。图 4 表明，对于所有 $u \in \mathbf{H}$，它意味着不等式或形式 (5)，因此 H 是等连续的。

我们明确说明 prop 的特殊情况。 4 个线性映射。

#### 命题 5 {#evt-ii-s1-prop-5 .statement tag=07B1}

— *令 E、F 为非离散值除法环 K 上的两个拓扑向量空间；假设 E（或 F）的拓扑由半范数 $\Gamma$（或 $\Gamma'$）的集合定义。设 H 为 F 中 E 的线性映射的集合。以下条件是等价的：*
    a) H 是等连续的。

b) 对于每个半范数$q \in \Gamma'$，都存在半范数属于到$\Gamma$和数$a > 0$的有限族$(p_i)_{1 \leq i \leq n}$，这样，对于所有$x \in E$和所有$u \in H$，

$$
q(u(x)) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x) .
$$

c) 对于每个半范数$q \in \Gamma'$，映射$\sup_{u \in H} (q \circ u)$是$E$上的连续半范数。

#### 推论 1 {#evt-ii-s1-prop-5-cor-1 .statement tag=07B2}

— 假设$\mathscr{T}, \mathscr{T}'$是向量空间$E$上的$K$上的两个拓扑，分别由半范数$\Gamma$和$\Gamma'$的两个集合定义。 $\mathscr{T}$比更细比$\mathscr{T}'$当且仅当，对于每个半范数$q \in \Gamma'$，存在半范数属于到$\Gamma$和数$a > 0$的有限族$(p_i)_{1 \leq i \leq n}$，使得对于所有$x \in E$，我们有$q(x) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x)$。

事实上，这表明$E$的恒等映射与拓扑$\mathscr{T}$，$E$与拓扑$\mathscr{T}'$，是连续的。

#### 推论 2 {#evt-ii-s1-prop-5-cor-2 .statement tag=07B3}

— 假设$K$上的拓扑向量空间$E$的拓扑$\mathscr{T}$由半范数$\Gamma$的有向集合定义；对于每个半范数$p \in \Gamma$，让$E_p$是使用$p$定义的拓扑从$E$获得的空间。 $E$上的线性形式的集合$E'$连续$\mathscr{T}$是集合$E'_p$的并，其中$E'_p$是连续线性形式的集合 $E_p$（$p \in \Gamma$）。
