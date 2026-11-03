---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 3
section_title: Dual of a Fréchet space
lang: zh
source: evt-i-v
book_pages: TVS IV.21-TVS IV.26, TVS IV.57-TVS IV.61
pdf_pages: 0203-0208, 0239-0243
extraction: ocr
subsections:
    - "no": 1
      title: Semi-barrelled spaces
      page: 21
      pdf_page: 203
    - "no": 2
      title: Dual of a locally convex metrizable space
      page: 22
      pdf_page: 204
    - "no": 3
      title: Bidual of a locally convex metrizable space
      page: 23
      pdf_page: 205
    - "no": 4
      title: Dual of a reflexive Fréchet space
      page: 23
      pdf_page: 205
    - "no": 5
      title: The topology of compact convergence on the dual of a Fréchet space
      page: 24
      pdf_page: 206
    - "no": 6
      title: Separately continuous bilinear mappings
      page: 26
      pdf_page: 208
statements: 15
exercises: 18
content_sha256: 2f09c9c9e86b840a795fd70d81ff40a703ec70ce9bfd5dcf352341bd62cfc76c
translated_from: content/en/evt/IV/03_s3_dual_of_a_frechet_space.md
translation_method: google
source_content_sha256: bb0b04778ba87067d91908af5a1b8236b1f89fcb725229b0b2dd6d0e99a65350
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 3818caa69627161f93a137d63eb6af8cdfa7c5d336b423ddb9a6097ecc6874da
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。双FrÉchet 空间

### 1. 半桶装空间

#### 命题 1 {#evt-iv-s3-prop-1 .statement tag=07TU}

— 令 E 为局部凸空间。以下条件是等效的：

(i) 令 U 为 E 的子集，它吸收 E 的每个有界子集，并且是 E 中 0 的凸、平衡、闭邻域的序列的交。则 U 是 E 中 0 的邻域。

(ii) 对于每个局部凸空间 F，$\mathscr{L}_b(E; F)$ 的每个有界子集（即等连续子集可数族的并）是等连续的。

(iii) 在 E 的强对偶$E'_b$中，等连续子集的可数族的每个有界子集（即并）是等连续的。

显然，(iii) 是(ii) 的特例。

(i) $\Rightarrow$ (ii) ：令 H 为 $\mathscr{L}_b(E; F)$ 的有界子集，并令 $(H_n)$ 为 $\mathscr{L}_b(E; F)$ 的等连续子集的序列，使得 $H = \bigcup H_n$。令 V 为 F 中 0 的凸、平衡且封闭的邻域。对于每个 $n$，集合 $W_n = \bigcap_{u \in H_n} u^{-1}(V)$ 是 E 中 0 的凸、平衡且封闭的邻域，因为 $H_n$ 是等连续的。 集合$W = \bigcap_{u \in H} u^{-1}(V)$吸收E的每个有界子集，因为H有界于$\mathscr{L}_b(E; F)$（III，p. 22），并且我们有$W = \bigcap_n W_n$。如果E满足(i)，则集合W是E中0的邻域，因此H是等连续的。

(iii) $\Rightarrow$ (i) ：令 $(U_n)$ 为 E 中 0 的凸、平衡且闭邻域的序列。我们假设集合 $U = \bigcap_n U_n$ 吸收 E 的每个有界子集，因此其极$U^\circ$ 有界$E'_b$。那么集合$B = \bigcup_n U_n^\circ$包含在$U^\circ$中，因此有界于$E'_b$。若E满足(iii)，集合B在$E'$等连续；因而，E 中 B 的极$B^\circ = \bigcap_n (U_n^\circ)^\circ = \bigcap_n U_n = U$ 是 E 中 0 的邻域。

#### 定义 1 {#evt-iv-s3-def-1 .statement tag=07TV}

— 如果局部凸空间 E 满足等价的 prop 条件，则称其为半桶状。 1.

每个桶装空间都是半桶装。这对于每个出生的空间（III，p. 22，道具10）也是如此。

### 2. 局部凸可度量的对偶空间

#### 命题 2 {#evt-iv-s3-prop-2 .statement tag=07TW}

— 设 E 为局部凸可度量空间，F 为强对偶。 空间 F 是完整的、半桶状的并且满足以下条件 ：
(DB) 存在 F 的有界子集的序列 $(A_n)_{n \in \mathbf{N}}$，使得 F 的每个有界子集都包含在 $A_n$ 之一中。

空间 E 是天生的 (III, p. 12, 命题 2)，因此它的强对偶是完备的 (III, p. 23, 命题 1)。

令$(V_n)_{n \in \mathbf{N}}$为E中0的邻域的递减序列，使得E中0的每个邻域都是包含中的$V_n$之一。令 $A_n$ 为 F 中 $V_n$ 的极坐标。由于 E 是天生的，F 的每个有界子集都是等连续的（III，p. 22，命题 10），因此包含在 $A_n$ 之一中。在其他字中，空间F满足条件(DB)。

现在我们证明 F 是半桶状的。令$(U_n)_{n \in \mathbf{N}}$为F中0的凸、平衡、闭邻域的序列。我们假设集合$U = \bigcap_n U_n$吸收F的每个有界子集。我们将证明U是F中0的邻域。为此，我们将构造、整数 $n \geqslant 0$、实数 $\lambda_n > 0$ 上的归纳以及 F 中 0 的凸平衡邻域 $W_n$，其对于 $\sigma(F, E)$ 和满足是闭合的关系

(1)
$$
\lambda_n A_n \subset \frac{1}{2} U \cap \left( \bigcap_{0 \leq i < n} W_i \right)
$$

(2)
$$
\bigcup_{0 \leq i \leq n} \lambda_i A_i \subset W_n \subset U_n .
$$

假设已为 $0 \leq i < n$ 构建了数 $\lambda_i$ 和集合 $W_i$。通过假设，集合 U 吸收 F 的有界子集；此外，对于$0 \leq i < n$，$W_i$是F中0的邻域，因此吸收了F的有界子集。因此我们可以找到数$\lambda_n > 0$满足（1）。令 C 表示 $\bigcup_{0 \leq i \leq n} \lambda_i A_i$ 的闭凸平衡包络线，对于 $\sigma(F, E)$； 集合 C 是等连续的，因此对于 $\sigma(F, E)$ 是紧凑的（III，p. 17，cor.2）。由于 F 中 $U_n$ 是 0 的邻域，因此存在 E 的有界子集 B，使得 $B^\circ \subset \frac{1}{2} U_n$。把$W_n = C + B^\circ$。由于F中$B^\circ$是0的邻域，我们看到$W_n$是F中0的凸且平衡的邻域。在加法中，C是紧的，$B^\circ$对于$\sigma(F, E)$是封闭的；由科。 GT 1 号、III, § 4, No. 1、$W_n$ $\sigma(F, E)$ 关闭。最后，我们有$C \subset \frac{1}{2} U \subset \frac{1}{2} U_n$和$B^\circ \subset \frac{1}{2} U_n$，因而$W_n \subset U_n$，因为$U_n$是凸的。这样我们就成立了(2)。

先放$W = \bigcap_n W_n$，然​​后放$W \subset U$。根据（1）和（2），我们对$\mathbf{N}$中的所有$i$和$j$有$\lambda_i A_i \subset W_j$，因此对所有$i \in \mathbf{N}$有$\lambda_i A_i \subset W$。特别是，W具有吸收性，因此是$\sigma(F, E)$的桶。由IV、p. 4的注3，W为F中0的邻域。更不必说，U为F中0的邻域，F为半筒状。

以下推论扩展 Banach-Steinhaus 定理与 Fréchet 空间的对偶（*cf.* III、p. 25，cor.2）。

#### 推论 {#evt-iv-s3-n2-cor-1 .statement tag=07TX}

— 令 G 为 Hausdorff 局部凸空间，并令 $(u_n)$ 为从 F 到 G 的线性映射的序列，从 F 到 G 简单收敛到映射 u。然后 u 是连续的，并且序列 $(u_n)$ 在每个预紧上均匀收敛到 u F 的子集。

由于 F 是完备的，所有 $u_n$ 的集合（以简单收敛的拓扑为界），都以 $\mathscr{L}_b(F; G)$ 为界（III，p. 27，cor. 1）。由于空间 F 是半桶状的（命题 2），$\mathscr{L}_b(F; G)$ 的每个可数且有界的子集都通过命题等连续。 1 个IV、p. 21。因此，$u_n$的集合是等连续的，推论由III、p. 18、推论推出。

### 3. 局部凸可度量化空间的对偶

#### 命题 3 {#evt-iv-s3-prop-3 .statement tag=07TY}

— 令 E 为局部凸可度量空间，$E'_b$ 其强对偶，G 为 Fréchet 空间。 空间 $\mathscr{L}_b(E'_b ; G)$ 是 Fréchet 空间。

通过道具。 2（IV，p. 22），$E'_b$的有界子集存在序列$(A_n)$，使得$E'_b$的每个有界子集都包含在$A_n$之一中。令$(V_n)$为G中0的邻域的可数基数系统。令$H_{mn}$为线性映射$u$的集合，从$E'_b$进入G，使得$u(A_m) \subset V_n$。那么$(H_{mn})$就是$\mathscr{L}_b(E'_b ; G)$中0的邻域的基本系统，而后者空间则可度量化。

要证明$\mathscr{L}_b(E'_b ; G)$是完备的，只要证明这个空间中的每一个柯西序列$(u_n)$都是收敛的即可；由于 G 是完备的，因此存在线性映射 $u : E'_b \to G$，使得 $(u_n)$ 简单收敛于 u。到IV、p. 23、推论，我们有$u \in \mathscr{L}_b(E'_b ; G)$。然后从 prop 得出。 GT 的 5，X, § 1, No. 5，$(u_n)$ 在$\mathscr{L}_b(E'_b ; G)$ 收敛于 u。

#### 推论 {#evt-iv-s3-n3-cor-1 .statement tag=07TZ}

— 局部凸可度量空间的双对偶是 Fréchet 空间。

### 4. 自反 Fréchet 的双重空间

#### 命题 4 {#evt-iv-s3-prop-4 .statement tag=07U0}

— 令 E 为自反 Fréchet 空间。 E 的强对偶 $E'_b$ 是 Banach 空间序列的归纳极限。

令$(V_n)_{n \in \mathbf{N}}$为E中0的凸、平衡且封闭的邻域的递减序列，使得E中0的每个邻域都是包含中的一个$V_n$。设$A_n$为$E'$中$V_n$的极坐标。那么$A_n$对于$\sigma(E', E)$来说是凸的、平衡的、紧致的；由 III、p. 8、推论空间 $E'_{A_n}$ 是 Banach 空间。我们要证明$E'_b$是空间$E'_{A_n}$的归纳极限；在其他字中，吸收每个$A_n$的$E'$的每个凸且平衡的子集U是$E'_b$中0的邻域。对于每个$n \in \mathbf{N}$，选择实数$\lambda_n > 0$，使得$\lambda_n A_n \subset U$。令$B_n$为集合$\bigcup_{0 \leq i \leq n} \lambda_i A_i$的凸包络；输入$V = \bigcup_n B_n$，然后输入$V \subset U$。对于每个 $n \in \mathbf{N}$，集合 $B_n$ 对于 $\sigma(E', E)$ 都是凸的、平衡的和紧凑的（II，p. 14，道具 15）。

现在我们将证明$\frac{1}{2} V^{oo} \subset V$。设 $x \in E'_b - V$；对于每个$n \in \mathbf{N}$，我们有$x \notin B_n$，并且由于$B_n$对于$\sigma(E', E)$是闭合的，所以$B_n^\circ$中存在元素$y_n$，使得 \langle y_n, x \rangle = 1 (\text{II, p. 38, prop. 4}）。由于 E 是自反的，因而 E 的每个有界子集对于 $\sigma(E, E')$ 来说都是相对紧凑的（IV，p. 16，第 2 个）。到$B_n$的定义，我们有
$$
\lambda_i y_n \in V_i \quad \text{for all } n \geq i,
$$
因此序列 $(y_n)$ 是有界的。对于拓扑 $\sigma(E, E')$，令 $y$ 为 $(y_n)$ 的极限点。我们有$y \in V^\circ = \bigcap_n B_n^\circ$和$\langle y, x \rangle = 1$。因而$x \notin \frac{1}{2}V^{\circ\circ}$，所以我们有包含$\frac{1}{2}V^{\circ\circ} \subset V$和*更不必说*，$\frac{1}{2}V^{\circ\circ} \subset U$。

由于$E'_b$的每个有界子集都包含在集合$A_n$之一中，因此集合$V = \bigcup_n B_n$吸收$E'_b$的每个有界子集。因而，$V^\circ$有界于E，因而$\frac{1}{2}V^{\circ\circ}$是$E'_b$中0的邻域。 *更不必说*，U是$E'_b$中的邻域。

#### 推论 {#evt-iv-s3-n4-cor-1 .statement tag=07U1}

*反身 Fréchet 空间的强对偶是天生的和桶装的。*

Banach 空间的归纳极限由定义产生。此外，Banach空间是桶装的（III，p. 25，推论），桶装空间的每个感应极限都是桶装空间（III，p. 25，cor.3）。

### 5. Fréchet 的对偶空间的紧凑收敛性拓扑

#### 定理 1（巴拿赫-迪厄多内）{#evt-iv-s3-thm-1 .statement tag=07U2}

— *令 E 为局部凸可度量空间。以下拓扑重合在 E 的对偶 $E'$ 上：*

a) *$\mathfrak{N}$的拓扑$\mathscr{T}_\mathfrak{N}$收敛，其中$\mathfrak{N}$是E的子集族，序列的点的每个由……组成收敛到0；*
b) *E 的紧子集上一致收敛的拓扑 $\mathscr{T}_c$；*
c) *E 的预紧式子集一致收敛的拓扑$\mathscr{T}_{pc}$；*
d) *拓扑$\mathscr{T}_f$，这是最好的拓扑，在$E'$的每个等连续子集上诱导出与$\sigma(E', E)$相同的拓扑。*

首先观察到，$E'$ 的 *子集 A 对 $\mathscr{T}_f$ 是封闭的，当且仅当 $A \cap H$ 对 $\sigma(E', E)$ 封闭，对于 $E'$ 的每个子集 H，它是等连续的并且对 $\sigma(E', E)$ 封闭。* 弱拓扑 $\sigma(E', E)$ 和 $\mathscr{T}_{pc}$ 诱导在 $E'$ 的每个等连续子集上，拓扑相同（III、p. 17，第 5 条）。因而，每个拓扑$\mathscr{T}_\mathfrak{N}$、$\mathscr{T}_c$、$\mathscr{T}_{pc}$、$\mathscr{T}_f$ 都比其后面的拓扑更粗糙。因而，只要证明 $\mathscr{T}_\mathfrak{N}$ 比 $\mathscr{T}_f$ 更等于更细。此外，$E'$中的每个翻译都是$\mathscr{T}_f$的同胚。因而，只要证明，如果 F 是 $E'$ 的子集，且对 $\mathscr{T}_f$ 是闭集，并且不包含 0，则存在集合 $S \in \mathfrak{N}$ 使得 $S^\circ \cap F = \varnothing$。

令 $(U_n)_{n \geq 0}$ 为 E 中 0 的邻域的递减序列，形成 0 的邻域的基数系统。 我们将通过 $n \geq 0$ 上的归纳构造，*有限* 集合 $X_n$，使得我们有
$$
X_n \subset U_n
$$
$$
\left( \bigcup_{0 \leq p \leq n} X_p \right)^\circ \cap U_{n+1}^\circ \cap F = \varnothing
$$

每整数$n \geqslant 0$。令$m \geqslant 0$为整数，使得$X_n$已针对$0 \leqslant n < m$构建，并且对于$0 \leqslant n < m$满足(4)和(5)。对于每 $x \in U_m$，放入
$$
F_x = (\bigcup_{0 \leqslant p < m} X_p)^{\circ} \cap \{x\}^{\circ} \cap U_{m+1}^{\circ} \cap F.
$$
公式 (5) 与$n = m - 1$ 意味着$\bigcap_{x \in U_m} F_x = \varnothing$。此外，集合$U_{m+1}^{\circ}$是等连续的，并且对于$\sigma(E', E)$是紧致的。鉴于$\mathscr{T}_f$的定义，集合$F_x$每一个对于$\sigma(E', E)$都是紧致的；因而，存在$U_m$的有限子集$X_m$使得$\bigcap_{x \in X_m} F_x = \varnothing$，*即*关系(5)满足$n = m$。

输入$S = \bigcup_{n \geqslant 0} X_n$。 $n \geqslant p$有$X_n \subset U_p$，因而$S$是序列的点的集合，在$E$收敛到0。从(5)我们推导出$S^{\circ} \cap U_{n+1}^{\circ} \cap F = \varnothing$，由于$E'$是集合$U_{n+1}^{\circ}$的序列的并，所以我们得到$S^{\circ} \cap F = \varnothing$。

#### 推出 1 {#evt-iv-s3-thm-1-cor-1 .statement tag=07U3}

*令 $E$ 为局部凸可度量空间。 $E$的每个预紧式子集都包含在序列的点的集合收敛于0的封闭凸平衡包络中。*

这是由于拓扑$\mathscr{T}_{pc}$和$\mathscr{T}_{\mathfrak{H}}$是相同的这一事实得出的。 2 个III、p. 15。

#### 推出 2 {#evt-iv-s3-thm-1-cor-2 .statement tag=07U4}

*令 $E$ 为 Fréchet 空间。在阶中，$E$的对偶$E'$的凸子集$A$对于$\sigma(E', E)$封闭，对于每个邻域$U$，$A \cap U^{\circ}$对于$\sigma(E', E)$封闭是必要且充分的0 在 $E$.*

由于$E$是完备的，$E'$上的拓扑$\mathscr{T}_c$相容的$E'$和$E$之间的对偶性（IV，p. 3，*例*）；因而，$E'$中的闭凸子集对于$\mathscr{T}_c$和$\sigma(E', E)$是相同的（IV，p. 1，道具1）。然后根据拓扑$\mathscr{T}_c$和$\mathscr{T}_f$的恒等式得出推论。

回想一下（I，p. 13），$E'$中的超平面在$\sigma(E', E)$关闭，是与$E$中的元素相关的$E'$上的线性形式中的核。科。因而 2 给出 cor 的另一个证明（对于 Fréchet 空间）。 1 个III、p. 21。

#### 推出 3 {#evt-iv-s3-thm-1-cor-3 .statement tag=07U5}

*令$E$为$E$的对偶$E'$的Banach空间和$M$向量子空间。在阶中，$M$对弱拓扑$\sigma(E', E)$关闭，其交与$E'$中的单位球（关闭）对$\sigma(E', E)$关闭是必要和充分的。

#### 例 {#evt-iv-s3-n5-exa-1 .statement tag=07U6}

— *令 $H$ 为希尔伯特空间满足可数性第一公理；让 $H_{\sigma}$ 表示空间 $H$，并将弱化的拓扑分配给它。令$\mathscr{L}^1(H)$为$H$的核自同态的Banach空间（V，p. 51，以及TS，V）； $\mathscr{L}^1(H)$中的范数由$\|u\|_1 = \operatorname{Tr}((u^*u)^{1/2})$定义。我们通过将$\mathscr{L}^1(H)$上的线性形式$\phi_u : v \mapsto \operatorname{Tr}(uv)$与每个$u \in \mathscr{L}(H)$相关联，将可以确定$\mathscr{L}(H)$与Banach空间$\mathscr{L}^1(H)$的对偶进行关联。设$A$为$\mathscr{L}(H)$、包含1的子代数且在$u \mapsto u^*$下稳定；这是冯诺依曼代数当且仅当它对于弱拓扑$\sigma(\mathscr{L}(H), \mathscr{L}^1(H))$而言在$\mathscr{L}(H)$内闭合。来自科。 3，我们推导出以下标准：*对于$A$是冯诺依曼代数，如果$(u_n)$是$A$的元素中的任何序列且范数$\leqslant 1$具有极限，则其充分必要$u$→空间$\mathscr{L}_s(H ; H_{\sigma})$，然后$u$属于至$A$。*

### 6. 单独连续的双线性映射

#### 引理 1 {#evt-iv-s3-lem-1 .statement tag=07U7}

设E和F是两个局部凸可度量空间，u是从$E'_b$到F的连续线性映射。则$E'_b$中存在0的邻域U，其u下的像有界于F。

令$(U_n)_{n \in \mathbf{N}}$（或$(V_n)_{n \in \mathbf{N}}$）为E（或F）中0的邻域的基本系统。我们假设集合$U_n$是平衡的并且形式递减序列。由于 u 是连续的，因此对于每个 $n \in \mathbf{N}$，E 中存在有界集合 $B_n$，使得 $u(B_n^\circ) \subset V_n$。由于$B_n$有界，因此存在实数$\lambda_n > 0$使得$\lambda_n B_n \subset U_n$。把$B = \bigcup_{n \in \mathbf{N}} \lambda_n B_n$。

我们将证明集合 B 在 E 中有界，在其他字中，对于每个整数 $m \geqslant 0$，存在实数 $\mu > 0$ 使得 $\mu B \subset U_m$。由于集合$B_n$有界，因此存在实数$\mu$使得$0 < \mu \leqslant 1$并且对于$0 \leqslant n \leqslant m$存在$\mu (\lambda_n B_n) \subset U_m$；如果$n > m$，我们还有$\lambda_n B_n \subset U_n \subset U_m$；因此 $\mu B \subset U_m$ 因为 $U_m$ 是平衡的。

设 U 为 B 在 $E'_b$ 中的极坐标。这是$E'_b$中0的邻域，我们有$\lambda_n B^\circ \subset B_n^\circ$，因此所有$n \in \mathbf{N}$都有$\lambda_n u(U) \subset V_n$。因而 $u(U)$ 有界于 F。

#### 定理 2 {#evt-iv-s3-thm-2 .statement tag=07U8}

令 $E_1$ 和 $E_2$ 为两个自反 Fréchet 空间，G 为局部凸 Hausdorff 空间。对于$i = 1, 2$，令$F_i$为$E_i$的强对偶。那么每个单独连续的双线性映射$u : F_1 \times F_2 \to G$都是连续的。

空间 G 同构于 Banach 空间的乘积子空间（II，p. 5，命题 3）。因而，在附加假设下证明定理就足够了，G是Banach空间。但 $F_1$ 是桶装的，$F_2$ 天生的（IV、p. 24、推论），$\mathscr{L}_b(F_2 ; G)$ 是 Fréchet 空间（IV、p. 23，道具 3）。让v表示从$F_1$到$\mathscr{L}_b(F_2 , G)$的线性映射，与u通过关系相关联

$$
u(x_1, x_2) = v(x_1)(x_2) \quad (x_1 \in F_1, x_2 \in F_2).
$$

由于 $F_1$ 是桶状的且 u 单独连续，因而 v 是连续的（III，p. 31，道具 6）。

由于 v 是连续的，引理 1 意味着 $F_1$ 中存在 0 的邻域 $U_1$，而 v 下的像的边界在 $\mathscr{L}_b(F_2 ; G)$ 内。在其他字中，对于$F_2$中的每个有界子集$B_2$，集合$u(U_1 \times B_2)$在Banach空间G中都有界。令$U_2$为所有$x_2 \in F_2$中的集合，使得$\|u(x_1, x_2)\| \leqslant 1$ 对于所有$x_1 \in U_1$。 集合 $U_2$ 然后吸收所有有界的子集；由于$F_2$是天生的，$U_2$是$F_2$中0的邻域，这证明了u是连续的。

### 习题 {#evt-iv-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
