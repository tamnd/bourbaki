---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 3
section_title: Measures and additive set functions
lang: zh
source: int-vii-ix
book_pages: INT IX.41-INT IX.49, INT IX.108-INT IX.112
pdf_pages: 0223-0231, 0290-0294
extraction: ocr
subsections:
    - "no": 1
      title: Measures and additive set functions of compact sets
      page: 41
      pdf_page: 223
    - "no": 2
      title: Inner regular set functions
      page: 44
      pdf_page: 226
    - "no": 3
      title: Radon spaces
      page: 46
      pdf_page: 228
statements: 17
exercises: 18
content_sha256: 9ab1a2dbbc3ef7984fa0f363c005015b133b79411e552907e0ea812b8d5eb031
translated_from: content/en/int/IX/03_s3_measures_and_additive_set_functions.md
translation_method: google
source_content_sha256: b7143e1dccb4a50f4c6430b942b6320cab29a534320ec6405180a553d32e45d9
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 6c167e22c1c6e6747868ff3110974dc12f1ade0ed2485c1f5d1b1ae356c502cb
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。措施和加法集合函数

在这个截面中，我们将分别用$\mathscr{K}(T)$和$\mathscr{B}(T)$表示Hausdorff拓扑空间T的紧致子集和T的Borel族的集合。

### 1. 紧集的措施和加法集合函数

#### 定理 1 {#int-ix-s3-thm-1 .statement tag=09PN}

— 令 T 为拓扑空间，且 $\mathscr{K}(T)$ 的 I 映射进入$\mathbf{R}_+$。在阶中，T上存在一个测度$\mu$使得$I(K) = \mu^\bullet(K)$对于所有$K \in \mathscr{K}(T)$来说，I满足以下条件是充分必要的：

1) 如果 K 和 L 是 T 的紧凑子集，使得 $K \subset L$，则 $I(K) \leq I(L)$（“I 是递增”）。

2) 如果 K 和 L 是 T 的紧子集，则$I(K \cup L) \leq I(K) + I(L)$。

3) 如果K和L是T的不相交的紧子集，则$I(K \cup L) = I(K) + I(L)$（“I是可加的”）。

4) 对于T的紧凑子集的每个递减有向家庭$(K_\alpha)_{\alpha \in A}$，一个有$I(\bigcap_{\alpha \in A} K_\alpha) = \inf_{\alpha \in A} I(K_\alpha)$。

5) 对于每个 $x \in T$，存在 x 的邻域 V，使得
$$
\sup_{\substack{K \in \mathscr{K}(T) \\ K \subset V}} I(K) < +\infty
$$
（“I 是局部有界的”）。

那么度量 $\mu$ 是唯一的。

$\mu$ 的唯一性源自 Cor。 § 1, No. 2 的第 2 号提案。上面的条件是必要的，前三个是明显的方式，最后一个是因为$\mu^\bullet$是一个局部有界的负担，而条件4）是由Cor. § 1, No. 6 的第 5 号提案。

为了证明这些条件是足够的，我们首先处理 T 是紧的情况。

#### 引理 1 {#int-ix-s3-lem-1 .statement tag=09PO}

假设 T 是紧的，并且集合 l = I(T)。每$A \subset T$，集合

$$
J(A) = \sup_{\substack{K \in \mathscr{K}(T) \\ K \subset A}} I(K)
$$

并令 $\Phi$ 为 $A \subset T$ 的集合，使得 $J(A) + J(\mathbf{C}A) = l$。 集合 $\Phi$ 是包含 $\mathscr{K}(T)$ 的氏族，$\Phi$ 上的函数 $J$ 是递增和相加。

很明显，$J$是递增集合函数，延伸$I$，并且每$A \subset T$延伸$J(A) + J(\mathbf{C}A) \leq l$。

令$K$和$S$为$T$中的两个紧集；我们首先要证明

$$
J(K \cap S) + J(\mathbf{C}K \cap S) = J(S).
$$

在考虑$I$至$\mathscr{K}(S)$和$J$至$\mathfrak{P}(S)$的限制时，立即将约化对应于$S = T$的情况。由于$T$是正规的，$K$是递减有向邻域的交，并且条件4)意味着对于每个$\varepsilon > 0$，存在$K$的紧凑邻域$H$使得$I(H) \leq I(K) + \varepsilon$。设$L$为$T - H$的闭包； $L$ 是紧凑的，$L \cap K = \varnothing$ 和 $H \cup L = T$，因此 $l = I(H \cup L) \leq I(H) + I(L) \leq I(K) + I(L) + \varepsilon$ (条件 2))、从而关系 $J(K) + J(\mathbf{C}K) \geq I(K) + I(L) \geq l - \varepsilon$。由于 $\varepsilon$ 是任意的，$J(K) + J(\mathbf{C}K) = l$。这就证明了公式(2)，以及包含$\mathscr{K}(T) \subset \Phi$。

现在让我们证明$\Phi$是一个氏族。由于$\Phi$在通向补体的过程中显然是稳定的，因此足以证明如果$A_1$和$A_2$表示$\Phi$的元素，则$A_1 \cup A_2 \in \Phi$，或者再次

$$
J(A_1 \cup A_2) + J(\mathbf{C}(A_1 \cup A_2)) \geq l.
$$

用$\varepsilon$数$> 0$表示，对于$i = 1, 2$，令$K_i$为包含在$A_i$中的紧集，以及包含在$\mathbf{C}A_i$中的$L_i$紧集，使得

$$
I(K_i) \geq J(A_i) - \varepsilon, \quad I(L_i) \geq J(\mathbf{C}A_i) - \varepsilon.
$$

集合$M_1 = K_1 \cup L_1$； 关系$l = J(M_1) + J(\mathbf{C}M_1)$ 和

$$
J(M_1) = I(K_1) + I(L_1) \geq J(A_1) + J(\mathbf{C}A_1) - 2\varepsilon = l - 2\varepsilon
$$

暗示$J(\mathbf{C}M_1) \leq 2\varepsilon$。那么如果$S$是$T$的紧致子集，关系 (2)（应用于$K = M_1$）意味着$J(S) \leq J(M_1 \cap S) + 2\varepsilon$，从而

$$
J(S) \leq J(K_1 \cap S) + J(L_1 \cap S) + 2\varepsilon.
$$

让我们添加通过制作$S = K_2$和$S = L_2$获得的不等式，并考虑到不等式$J(K_2) + J(L_2) \geq l - 2\varepsilon$以及$K_1 \cap K_2$，$L_1 \cap K_2$和$K_1 \cap L_2$是三个不相交的紧集包含在$A_1 \cup A_2$。用这三个紧集中的$C$并表示，可以得出：

$$
l - 2\varepsilon \leq J(K_2) + J(L_2) \leq J(C) + J(L_1 \cap L_2) + 4\varepsilon \\
\leq J(A_1 \cup A_2) + J(\mathscr{C}(A_1 \cup A_2)) + 4\varepsilon,
$$

鉴于$\varepsilon$的任意性，从而立即得到所需的公式（3）。成立后，前面的不等式意味着 $J(C) \geq J(A_1 \cup A_2) - 6\varepsilon$；如果$A_1$和$A_2$是不相交的，则$C$是$K_1 \cap L_2 \subset A_1$和$K_2 \cap L_1 \subset A_2$的并，由此推导出$J(A_1 \cup A_2) \leq J(A_1) + J(A_2)$。反之不等式显而易见，$J$确实是$\Phi$的相加，引理成立。

对于 $T$ 是紧致的情况，让我们完成定理的证明。令$\mathscr{E}(\Phi)$为$T$上$\Phi$步函数的向量空间，配备一致收敛的拓扑（Ch.IV, §4, No. 9，Def.4）；我们将再次用$J$表示与加性函数$J$相关的$\mathscr{E}(\Phi)$上的正值线性形式（参见第18号提案）。由于$J(T) = l$，$J$是连续的并且有范数$l$。令$\mathscr{H}$为$\mathscr{E}(\Phi)$对于拓扑一致收敛的闭包；我们立即验证$J$可以通过连续性扩展到$\mathscr{H}$上的*正*线性形式，再次表示为$J$。由于 $\mathscr{H}$ 包含于 $\mathscr{C}(T)$（前述，No. 10，第 19 号提案），$J$ 至 $\mathscr{C}(T)$ 中的限制是积极措施 $\mu$。还需要证明对于 $T$ 的每个紧凑子集 $K$，$\mu^\bullet(K) = I(K)$。现在，我们有$\mu^\bullet(K) = \inf_{f \in S_K} \mu^\bullet(f)$，其中$S_K$表示$\mathscr{C}(T)$的元素中的集合，即$\geq \varphi_K$（§ 1, No. 6，命题5）。由于$J(f) = \mu^\bullet(f)$对应$f \in \mathscr{C}(T)$，显然足以证明$J(K) \geq \inf_{f \in S_K} J(f)$。如引理 1 的证明，令$H$ 为$K$ 的紧邻域，使得$J(H) \leq J(K) + \varepsilon$，并让$f$ 为$T$ 上的连续函数，介于0 和1 之间，等于$K$ 上的1，并且0 在 $H$ 之外（GT，IX, §4, No. 1，提案 1）。然后

$$
J(f) \leq J(H) \leq J(K) + \varepsilon;
$$

$\varepsilon$是任意的，需要的不等式得证，当$T$紧致时，定理成立。

现在让我们讨论一般情况。对于$T$中的每个紧集$L$，令$I_L$为$I$到$\mathfrak{K}(L)$的限制。通过刚刚处理的特殊情况，$L$上存在唯一的测度$\mu_L$，使得每个紧集$K \subset L$都有$\mu_L(K) = I_L(K)$。令$L'$ 为紧集包含在$L$ 中；对于每个紧集$K \subset L'$，我们有$(\mu_L)_{L'}^\bullet(K) = \mu_{L'}^\bullet(K) = \mu_{L'}^\bullet(K)$，因此$\mu_{L'} = (\mu_L)_{L'}$； 映射 $\mu : L \mapsto \mu_L$ 是预测值。 条件 5) 表示$\mu$是一个测度，关系$I(K) = \mu^*(K)$对于所有紧致$K \subset T$是显而易见的。

#### 注 1 {#int-ix-s3-n1-rem-1 .statement tag=09PP}

在定理 1 的陈述中，条件 4) 可以用以下条件（“右连续性”）代替：
$4')$ 对于每个$K \in \mathscr{K}(T)$ 和每个$\varepsilon > 0$，都存在一个包含$K$ 的开集$U$，这样对于每个紧集$H \subset U$ 都有$I(H) \leq I(K) + \varepsilon$。
因为，如果 $\mu$ 是一个测度，则函数 $I : K \mapsto \mu^*(K)$ 满足 $4'$（§ 1, No. 9，命题 13）。 反之，假设$I$满足1)和$4'$；让我们证明 $I$ 则满足 4)。 对于记号，如定理 1 的叙述、选择、$\varepsilon > 0$ 和开集合 $U$ 包含紧集 $K = \bigcap_{\alpha \in A} K_\alpha$，并且满足$4'$）。 那么存在指标$\beta \in A$使得$K_\beta \subset U$，这意味着
$$
\inf_{\alpha \in A} I(K_\alpha) \leq I(K_\beta) \leq I(K) + \varepsilon
$$
4) 确实得到验证。

#### 注 2 {#int-ix-s3-n1-rem-2 .statement tag=09PQ}

条件 2)和3)中的集合可以在定理 1的叙述中用以下条件代替：
如果$K$和$L$是$T$的紧子集，那么
$$
I(K \cup L) + I(K \cap L) = I(K) + I(L).
$$
事实上，这个条件意味着2)和3)，另一方面
$$
\mu^*(K \cup L) = \mu^*(K \cap L) = \mu^*(K) + \mu^*(L)
$$
对于每个措施$\mu$，凭借关系$\varphi_{K \cup L} + \varphi_{K \cap L} = \varphi_K + \varphi_L$之间的特征函数。

### 2. 内部常规集合函数

#### 定义 1 {#int-ix-s3-def-1 .statement tag=09PR}

令$T$为拓扑空间，令$\mathscr{B}(T)$为$T$的Borel族；设$I$为$\mathscr{B}(T)$的映射到$\overline{\mathbf{R}}_+$。
a) $I$ 被认为是可数可加的，如果对于 $\mathscr{B}(T)$ 的成对不相交的元素中的每个序列 $(A_n)$，
$$
I\left( \bigcup_n A_n \right) = \sum_n I(A_n).
$$
b) $I$ 被称为内部常规，如果对于每个集合 $A \in \mathscr{B}(T)$，
$$
I(A) = \sup_K I(K),
$$
其中 $K$ 超过 $A$ 的紧凑子集的集合。

c) 如果$I(T) < +\infty$（或者每个点$x \in T$承认一个开邻域$V$使得$I(V) < +\infty$），则I被称为有界（或局部有界）。

#### 注 1 {#int-ix-s3-n2-rem-1 .statement tag=09PS}

条件 a) 清楚地暗示I 是$\mathscr{B}(T)$（按包含排序）到$\overline{\mathbf{R}}_+$ 的递增映射。

#### 注 2 {#int-ix-s3-n2-rem-2 .statement tag=09PT}

假设I是可数可加的；令$(A_n)_{n \in \mathbf{N}}$为Borel集合的递增序列，并令$A = \bigcup_{n \in \mathbf{N}} A_n$。 集合$D_0 = A_0$，$D_n = A_n - A_{n-1}$成对不相交的，它们的并是A，我们有$I(A) = \sum_n I(D_n) = \lim_{n \to \infty} I(A_n)$。类似地，如果$(B_n)$是Borel集合的递减序列，并且如果$I(B_0) < +\infty$，则$I(\bigcap_n B_n) = \lim_{n \to \infty} I(B_n)$：将前述应用于集合$A_n = B_0 - B_n$就足够了。

#### 注 3 {#int-ix-s3-n2-rem-3 .statement tag=09PU}

令 $(A_n)$ 为 T 的 Borel 集合的任意序列。如果 I 可数可加，则$I(\bigcup_n A_n) \leq \sum_n I(A_n)$。通过前面的注，足以为有限序列建立这个不等式。一个立即约化到两个集合$A_1$和$A_2$的情况；但关系 (4) 意味着

$$
I(A_1 \cup A_2) = I(A_1) + I(A_2 - (A_1 \cap A_2)) \leq I(A_1) + I(A_2).
$$

然后立即出现所需的不等式。

#### 注 4 {#int-ix-s3-n2-rem-4 .statement tag=09PV}

如果I是可数加法且局部有界函数，则前面的注立即意味着对于每个紧集$K \subset T$都有$I(K) < +\infty$。

#### 注 5 {#int-ix-s3-n2-rem-5 .statement tag=09PW}

可以证明，如果 I 是可加性的，即有限序列满足 (4)，并且如果 I 是内部正则，则 I 是可数可加性的（例 7）。读者还可以确定，Th 的证明中仅使用了可加性和内部正则性。 2 下面。

#### 定理 2 {#int-ix-s3-thm-2 .statement tag=09PX}

— 令 T 为拓扑空间，并令 I 为在 $\mathscr{B}(T)$ 上定义的函数，值在 $\overline{\mathbf{R}}_+$ 中。在阶中，T上存在一个测度$\mu$，使得$\mu^*(A) = I(A)$对于每一个$A \in \mathscr{B}(T)$，I是可数可加的、局部有界的且内部正则是充分必要的。那么度量$\mu$是唯一的。

这三个条件是必要的：因为，$\mathscr{B}(T)$上的映射$A \mapsto \mu^*(A)$是可数累加的（§ 1, No. 5，Prop.4的Cor.），局部以定义的度量为界（§ 1, No. 2，Def.5），并且内部正则注 3 个，共 § 1, No. 2。

我们走向存在。可知，I～$\mathscr{K}(T)$的限制满足Th的叙述的条件1)、2)、3)、5)。 1;让我们证明 4) 也满足。令K为T的紧子集，递减的有向族$(K_\alpha)_{\alpha \in A}$的紧集的交，并令$\varepsilon$为数$> 0$； I 是局部有界的，存在 K 的开邻域 V，使得 $I(V) < +\infty$，然后存在指标 $\alpha$，使得 $K_\alpha \subset V$；如有必要，更改记号，我们可以假设$K_\alpha \subset V$适用于所有$\alpha \in A$。根据I的内部正则，存在紧集$L \subset V - K$使得$I(L) \geq I(V - K) - \varepsilon$；由于L不与K相交，因此存在指标$\alpha$使得$L \cap K_\alpha = \varnothing$，然后有$I(V - K_\alpha) \geq I(L) \geq I(V - K) - \varepsilon$。从$K_\alpha \subset V$开始，$I(K_\alpha) \leq I(K) + \varepsilon$和条件4)得到验证。

由 Th. 1，存在一个测度$\mu$，使得$\mu^\bullet(K) = I(K)$对于所有$K \in \mathscr{K}(T)$。 内部集合函数$\mu^\bullet$和$I$在$\mathscr{B}(T)$上的正则性意味着$\mu^\bullet(A) = I(A)$对于所有$A \in \mathscr{B}(T)$，并且存在性被证明。 $\mu$的唯一性源自Th的唯一性断言。 1.

### 3. 氡气空间

#### 定义 2 {#int-ix-s3-def-2 .statement tag=09PY}

*设 T 为拓扑空间。有人说 T 是氡气（或强氡气）空间，如果 T 是 Hausdorff，并且如果在 T 的 Borel 族$\mathscr{B}(T)$ 上定义的每个函数，其中值在 $\overline{\mathbf{R}}_+$，则可数加性且有界（或局部有界）是内部正则。

例如，我们稍后将看到（命题 3），每个波兰语空间都是强氡气。特别是，每个具有可数基的局部紧致空间都是强氡气。

存在非强氡气的氡气空间。

#### 命题 1 {#int-ix-s3-prop-1 .statement tag=09PZ}

*每个 Lindelöf*$^{(1)}$* 氡气空间是强氡气。*

令 T 为 Lindelöf 空间，即氡气，并令 I 为部落 $\mathscr{B}(T)$ 上的集合函数，该族为正数、可加性且局部有界。开集合V使得$I(V) < +\infty$形式T的覆盖，从中可以提取可数覆盖$(V_n)_{n \in \mathbf{N}}$。每 $n \in \mathbf{N}$ 集合 $G_n = V_0 \cup V_1 \cup \cdots \cup V_n$； 集合 $H_0 = G_0$ 和 $H_n = G_n - G_{n-1}$ $n \geq 1$；最后，在$\mathscr{B}(T)$上用$I_n$集合函数$A \mapsto I(A \cap H_n)$表示，这显然是可数可加且有界的。从 T 的集合 $H_n$ 形式划分开始，我们有 $I = \sum_n I_n$。 空间 T 是氡气，对于每个$n \in \mathbf{N}$，T 上存在一个有界测度$\mu_n$，使得$\mu_n^\bullet(A) = I_n(A)$ 对于所有 $A \in \mathscr{B}(T)$；因此也$\sum_n \mu_n^\bullet(A) = I(A)$。由于 I 是局部有界的，所以$(\mu_n)$族是可求和的（§ 1, No. 7，命题 7）；如果 $\mu$ 表示 $\sum_n \mu_n$，则对于所有 $A \in \mathscr{B}(T)$，我们都有 $\mu^\bullet(A) = I(A)$，因此 I 是内部正则。在其他字中，T是强氡气。

回想一下，拓扑空间 T 的子集 A 被称为“通用可测”，如果 A 对于 T 上的每个测度 $\mu$ 都是 $\mu$ 可测的。这相当于说，A 对于 T 上的每个测度 $\mu$ 都是 $\mu$ 可测的，且有*紧凑支持* （§ 1, No. 8，提案 9）。

(1) 回忆一下 (GT, I, §9, Exer. 14; TG, IX, 附录 I) *Lindelöf 空间* 是一个拓扑空间 T，使得 T 包含的每个开覆盖都是可数覆盖。

#### 命题 2 {#int-ix-s3-prop-2 .statement tag=09Q0}

— 令 X 为 X 的拓扑空间和 T 子空间。

a) 假设 T 是氡气空间。然后，对于在 $\mathscr{B}(X)$ 上定义的每个函数 I ，它是正的、可数可加的且有界的，有

$$
\sup_{\substack{K \text{ compact} \\ K \subset T}} I(K) = \inf_{\substack{B \in \mathscr{B}(X) \\ B \supset T}} I(B).
$$

此外，T 在 X 中普遍可测。

b) 相反，假设X是氡空间并且T在X中普遍可测；那么 T 是氡气空间。

让我们证明a）。我们用$\alpha$表示(6)的右侧；对于每个$n \in \mathbf{N}$，都存在集合 $C_n \in \mathscr{B}(X)$ 包含于 T，因此$I(C_n) \leq \alpha + 2^{-n}$。 设定$C = \bigcap_n C_n$，然后我们有$T \subset C$，$I(C) = \alpha$。如果$A \in \mathscr{B}(T)$，让我们选择一个X的Borel集合B，这样$A = B \cap T$（GT，IX, §6, No. 3）和集合$J(A) = I(B \cap C)$。这个数不依赖于B的选择，因为如果$B'$是X中的第二个Borel集合，使得$A = B' \cap T$，那么$B \cap C$和$B' \cap C$的区别仅在于包含在集合M中的Borel集合M $C - T$，以及$I(M) = 0$乘构造乘C。显然，每紧集 $K \subset T$ 就有 $J(K) = I(K)$。令$(A_n)$为T的Borel集合的序列，成对不相交的，并且对于每个$n$，令$B_n$为X的Borel集合，使得$B_n \cap T = A_n$。 替换$B_n$乘以$B_n - \left( \bigcup_{k < n} B_k \right)$，如果有必要，我们可以假设集合$B_n$是成对的不相交的。 集合$A = \bigcup_n A_n$和$B = \bigcup_n B_n$；然后

$$
J(A) = I(B \cap C) = \sum_n I(B_n \cap C) = \sum_n J(A_n);
$$

因而，J 是可数加法，且以 $\mathscr{B}(T)$ 为界函数。由于 T 由假设一个氡空间构成，因而 T 上存在有界测度 $\mu$，使得对于每个 $A \in \mathscr{B}(T)$ 都有 $J(A) = \mu^\bullet(A)$；因而

$$
\alpha = J(T) = \mu^\bullet(T) = \sup_K \mu^\bullet(K) = \sup_K J(K),
$$

定义共 $\mu^\bullet$。 公式(6)由此成立。

现在让我们证明 T 是普遍可测的。令 $\lambda$ 为 X 上的有界测度；前面的论点可以应用于$\mathscr{B}(X)$上的集合函数$I : A \mapsto \lambda^\bullet(A)$，因此存在T的紧凑子集的序列$(K_n)$，使得（与上面的记号）

$$
\sup_n \lambda^\bullet(K_n) = J(T) = \lambda^\bullet(C).
$$

集合$K' = \bigcup_{n \in \mathbf{N}} K_n$； $K'$ 是 $X$、$K' \subset T \subset C$、$\lambda^*(K') = \lambda^*(C)$ 中的 Borel，因此这三个集合仅相差 $\lambda$（可忽略不计）集合，因而 $T$ 是 $\lambda$ 可测的。这样就完成了 a) 的证明。

让我们转到b)。假设$X$是氡气空间，并且$T$在$X$中普遍可测。令 $I$ 为 $\mathscr{B}(T)$ 上的正函数，它是可数可加且有界的； 函数 $A \mapsto I(A \cap T)$ 在 $\mathscr{B}(X)$ 上则为正数、可数加法且有界，因此在 $X$ 上存在有界测度 $\nu$，使得 $I(A \cap T) = \nu^*(A)$ 对于所有 $A \in \mathscr{B}(X)$。现在，$T$是$\nu$可测量的；前面的关系表明，对于$X$的每个紧凑子集$K$，$\nu^*(K) = 0$是$T$的不相交的，因而$\nu$集中在$T$。因而，对于 $X$ 的每个 Borel 集合 $A$，我们都有 $I(A \cap T) = \nu^*(A \cap T) = \mu^*(A \cap T)$，其中 $\mu$ 是$\nu$ 在 $T$ 上引起的测度。最后，$I(B) = \mu^*(B)$对于每个集合$B \in \mathscr{B}(T)$（GT，IX, §6, No. 3，*注2*），并且$I$确实是内部正则。

#### 推论 {#int-ix-s3-n3-cor-1 .statement tag=09Q1}

— *如果 $X$ 是氡气空间，则 $X$ 的每个 Borel 子集 $T$ 都是氡气。*

因为，$T$在$X$中是普遍可测的。

#### 命题 3 {#int-ix-s3-prop-3 .statement tag=09Q2}

— *每个 Souslin 空间（特别是每个波兰或 Lusin 空间）都具有很强的氡气。*

令$T$为苏斯林空间；由于 $T$ 是 Lindelöf 空间（TG，IX，附录 I，命题 1 的 Cor.），(2) 足以证明 $T$ 是氡气（命题 1）。设 $I$ 是在 $\mathscr{B}(T)$ 上定义的函数，正数、可加性且有界。我们将扩展 $I$ $\mathscr{P}(T)$ 设定子集 $A$ $T$，

$$
I(A) = \inf_{\substack{B \in \mathscr{B}(T) \\ B \supseteq A}} I(B).
$$

让我们证明这个扩张是$T$（GT，IX, §6, No. 9）上的*容量*。显然，关系$A \subset A'$意味着$I(A) \leq I(A')$。令$(A_n)$为$T$的子集、递增、序列，并令$A = \bigcup_n A_n$。 Borel 集合的集合使得包含$A_n$对于可数交是稳定的，对于每个$n$都存在一个Borel集合$B_n$使得$A_n \subset B_n$和$I(A_n) = I(B_n)$ （提案 2 的cf. 证明）。 集合$C_n = \bigcap_{p \geq n} B_p$； $C_n$ 是 Borel，$A_n \subset C_n \subset B_n$，因而 $I(A_n) = I(C_n)$。另一方面，序列$(C_n)$是递增。让 $C = \bigcup_n C_n$: 关系 $A \subset C$ 意味着

$$
I(A) \leq I(C) = \lim_n I(C_n) = \lim_n I(A_n),
$$

(2) 每个 Souslin 空间对于开集合都有一个可数基 (GT, IX, §6, No. 2, 命题 4)，因此是 Lindelöf (GT, I, §9, Exer. 14)。

从而等式$I(A) = \lim_n I(A_n)$是直接的。因而，I是一个容量。

如果T中$(H_n)$是闭集合的递减序列，显然是$I\left( \bigcap_n H_n \right) = \inf_n I(H_n)$。由此可见，T 的每个 Souslin 子集 F 都能够实现 I（TG，IX, §6, No. 10，命题 15）。特别是，T 的每个 Borel 集合 A 都是有能力的（*loc.cit.*，§6, No. 3，提案 10）。(3) 在其他字中，

$$
I(A) = \sup_K I(K),
$$

其中 K 超过 A 中包含的紧集的集合；我们已经证明I是内部正则。

#### 注 {#int-ix-s3-n3-rem-1 .statement tag=09Q3}

— 令 X 为 Lusin 空间（特别是任何波兰语空间），并且将 X 的双射连续映射置于（Lusin）正则空间 Y 上。人们知道（TG，IX, §6, No. 7，命题 14） 映射 $B \mapsto f^{-1}(B)$ 是Y 的Borel 部落的双射到X 的Borel 部落。 空间 X 和 Y 是 Lusin，因此是强氡气（命题 3）。紧接着，映射$\mu \mapsto f(\mu)$是X上有界度量的集合的双射到Y上有界度量的集合。(4)

### 习题{#int-ix-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
