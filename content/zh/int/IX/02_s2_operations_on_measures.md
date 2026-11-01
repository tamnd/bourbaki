---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 2
section_title: Operations on measures
lang: zh
source: int-vii-ix
book_pages: INT IX.22-INT IX.41, INT IX.108
pdf_pages: 0204-0223, 0290-0290
extraction: ocr
subsections:
    - "no": 1
      title: Induced measure on a measurable subspace
      page: 22
      pdf_page: 204
    - "no": 2
      title: Measures defined by numerical densities
      page: 24
      pdf_page: 206
    - "no": 3
      title: Image of a measure
      page: 26
      pdf_page: 208
    - "no": 4
      title: Lifting of measures
      page: 29
      pdf_page: 211
    - "no": 5
      title: Product of two measures
      page: 31
      pdf_page: 213
    - "no": 6
      title: Integration with respect to the product of two measures
      page: 33
      pdf_page: 215
    - "no": 7
      title: A result on the disintegration of measures
      page: 37
      pdf_page: 219
statements: 41
exercises: 3
content_sha256: 695fe573b09be6dab5072f74826a2cf590131bc7ab07ae50e2a342fe6506bdca
translated_from: content/en/int/IX/02_s2_operations_on_measures.md
translation_method: google
source_content_sha256: d7699f39ec1644b116484ef30c5ca9df84de13c33a79612bcf054973c062c5c9
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 417c7d1fc7f5d1243244e723902547cc43b02b941e30fe79b031cdee6c945a76
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。 运算采取措施

与前面的截面一样，$T$表示豪斯多夫拓扑空间，$\mu$表示$T$的测度。请记住，所有措施均假定为积极的，没有提及相反的情况。

### 1. 对可测量的子空间进行诱导测量

令$X$为$T$的子集，令$\nu$为$X$的紧凑子集的映射$\mu : K \mapsto \mu_K$限制至集合；显然$\nu$是$X$的预测值。另一方面，令$x \in X$和$V$是$x$在$T$中的开邻域，使得$\mu^\bullet(V) < +\infty$；然后

$$
\nu^\bullet(X \cap V) = \sup_{\substack{K \text{ compact} \\ K \subset X \cap V}} \mu^\bullet(K) \leq \mu^\bullet(V) < +\infty
$$

通过 §1, No. 2 的 *注 3*，因此 $\nu$ 是一个度量。

当$X$不是$\mu$可测量时，产权负担$\nu^\bullet$和$(\mu^\bullet)_X$不一定相等，并且测量$\nu$没有利息。

#### 定义 1 {#int-ix-s2-def-1 .statement tag=09OF}

*令 $X$ 为 $T$ 的 $\mu$ 可测量子集。 $\mu : K \mapsto \mu_K$的限制到$X$的紧凑子集的集合称为$\mu$在子空间$X$上引发的测度，并用$\mu_X$或$\mu|X$表示。*

#### 命题 1 {#int-ix-s2-prop-1 .statement tag=09OG}

*令 $X$ 为 $T$ 的 $\mu$ 可测量子集。负担$(\mu_X)^\bullet$等于$\mu^\bullet$在$X$（§1, No. 1）上引起的负担$(\mu^\bullet)_X$。在其他字，每函数$g \in \mathscr{F}_+(X)$对应$(\mu_X)^\bullet(g) = \mu^\bullet(g^0)$。

令$f \in \mathscr{F}_+(X)$且$f^0$为扩张除$f$至$T$中的0。一个有 $(\mu^\bullet)_X(f) = \mu^\bullet(f^0) = \sup_L \mu^\bullet(f^0 \varphi_L)$，其中 $L$ 超过 $T$ 的紧致子集的集合（§1, No. 2，命题 2）；类似地$(\mu_X)^\bullet(f) = \sup_K \mu_K^\bullet(f_K) = \sup_K \mu^\bullet(f^0 \varphi_K)$，其中$K$运行超过$X$的紧凑子集的集合。因此，这一切都归结为表明对于$T$的每个紧凑子集$L$，$\mu^\bullet(f^0 \varphi_L) = \sup_K \mu^\bullet(f^0 \varphi_K)$，其中$K$超过$L \cap X$的紧凑子集的集合。现在，令$(K_n)$为$L \cap X$中包含的紧集的递增序列，使得$(L \cap X) - \bigcup_n K_n$局部$\mu$可忽略不计（§1, No. 8，命题11）； $f^0$在$X$之外是零，$f^0 \varphi_L$在$L \cap X$之外是零，因此几乎处处都等于序列$(f^0 \varphi_{K_n})$的上包络线。这意味着 $\mu^\bullet(f^0 \varphi_L) = \sup_n \mu^\bullet(f^0 \varphi_{K_n})$, 从而是期望的结果。*

#### 注 1 {#int-ix-s2-n1-rem-1 .statement tag=09OH}

关系 $(\mu_X)^\bullet = (\mu^\bullet)_X$ 允许毫无歧义地使用记号 $\mu_X^\bullet$；今后我们将这样做。前面§1, No. 2的命题1和命题2表明，迄今为止$\mu_K$表示的措施，对于$K$紧凑来说，确实是Def意义上的诱导措施。 1. 类似地，如果$T$是局部紧的，并且如果$X$是$T$的局部紧的子空间，则上述第1章的命题1和命题1。 V, §7, No. 1 表明 Def. 1 第 1 章重合与定义 IV, §5, No. 7。

#### 注 2 {#int-ix-s2-n1-rem-2 .statement tag=09OI}

定义。 1可以扩展到$\mu$是$T$的复测度的情况。为了在这种情况下证明预测值 $\mu_X$ 是一个测度，只需观察 $|\mu_K| = |\mu|_K$ 对于 $X$ (§1, No. 2) 的每个紧凑子集 $K$ 即可。

根据命题 1，当且仅当 $X$ 的子集 $Y$ 是$\mu_X$ 可测量的（分别是本地 $\mu_X$ 可忽略的），当且仅当它是 $\mu$ 可测量的（分别是本地 $\mu$ 可忽略的）。如果 $Y$ 是 $\mu_X$ 可测，因此 $\mu$ 可测，则根据命题 1，诱导测度 $(\mu_X)_Y$ 和 $\mu_Y$ 显然相等（*诱导测度的传递性*）。

注3）。 — 令 X 为 T 的 $\mu$ 可测量子集。根据 §1, No. 8 的第 10 条命题，应用于 $g = \varphi_X$，存在 T 的压碎 $(K_\alpha)_{\alpha \in A}$，使得对于每个 $\alpha \in A$，要么有 $K_\alpha \subset X$，要么有$K_\alpha \subset \mathbf{C}X$。如果通过§1, No. 8的Scholium程序修改T的拓扑，则将X配备由$T'$引发的拓扑而获得的空间$X'$是局部紧致的，并且知道如何与$\mu$（分别与$\mu_X$）相关联$T'$（或$X'$）上的测度$\mu'$（或$\nu$），承认与$\mu$（或$\mu_X$）相同的基本上积分：这意味着$\mu'_{X'} = \nu$。由于局部可忽略的集合、可测量的映射以及本质上可积函数和 Banach 空间中的值，对于 $\mu$ 和 $\mu'$，以及对于 $\mu_X$ 和 $(\mu_X)' = \nu = \mu'_{X'}$，积分理论相对于第 1 章中处理的诱导措施约化。 V, §7在局部紧致空间的特殊情况下。我们将抄写结果的任务留给读者。

### 2. 由数值密度定义的度量

#### 定义 2 {#int-ix-s2-def-2 .statement tag=09OJ}

*函数 f 在 T 上定义，值在 $\overline{\mathbf{R}}$ 或 Banach 空间中，如果 f 是 $\mu$ 可测的，并且每个点 $x \in T$ 承认一个邻域 V，则称其为局部 $\mu$ 可积$\mu^\bullet(|f|\varphi_V) < +\infty$.*

这个定义重合与第 1 章中给出的定义重合相同。 V, §5, No. 1，如果 T 是局部紧致的。

设$f$为局部$\mu$可积正函数； 映射 $K \mapsto f_K \cdot \mu_K$ 是预测措施（第 V, §7, No. 1 章，第 1 章 Cor.2），将表示为 $f \cdot \mu$。

#### 命题 2 {#int-ix-s2-prop-2 .statement tag=09OK}

*如果 f 是正局部 $\mu$ 可积函数，则对于每个函数 $g \in \mathscr{F}_+(T)$，有关系*

$$
(f \cdot \mu)^\bullet(g) = \mu^\bullet(fg).
$$

事实上，对于 T 中的每个紧集 K，

$$
(f \cdot \mu)_K^\bullet(g_K) = (f_K \cdot \mu_K)^\bullet(g_K) = \mu_K^\bullet(f_K g_K) = \mu_K^\bullet((fg)_K),
$$

关于使用 $f \cdot \mu$ 的定义和第 3 章的提案 3。 V, §5, No. 3。命题 2 由此在经过上得出 K 上的上界。

现在让$x \in T$和V是x的邻域，使得$\mu^\bullet(f \varphi_V) < +\infty$（定义2）；那么$(f \cdot \mu)^\bullet(V) = \mu^\bullet(f \varphi_V) < +\infty$，因此$f \cdot \mu$是一个测度。

#### 定义 3 {#int-ix-s2-def-3 .statement tag=09OL}

*设 f 为局部 $\mu$ 可积正函数。测度$f \cdot \mu : K \mapsto f_K \cdot \mu_K$被称为密度f关于*对$\mu$的测度，或乘积对$\mu$的测度函数$f$。 形式 $f \cdot \mu$ 的每个测度（其中 $f$ 为正且局部 $\mu$ 可积）称为具有基 $\mu$ 的测度。

#### 注 1 {#int-ix-s2-n2-rem-1 .statement tag=09OM}

$f \cdot \mu$扩展的定义对于$f$是局部复数可积函数的情况；那么就有 $|f \cdot \mu| = |f| \cdot \mu$，这立即意味着 $f \cdot \mu$ 是一种测度，而不仅仅是一个预测值。我们保留表达“使用基$\mu$的度量”来指定如此定义的复杂度量。

#### 注 2 {#int-ix-s2-n2-rem-2 .statement tag=09ON}

Similarly, if $\theta$ is a complex measure, $f$ is said to be locally $\theta$-integrable if it is locally $|\theta|$-integrable, and one defines the measure $f \cdot \theta : K \mapsto f_K \cdot \theta_K$. 一个有$|f \cdot \theta| = |f| \cdot |\theta|$（第 1 章） V, §5, No. 2，命题 2)。 在本期中，我们将抛开所有有关非积极措施的内容。

#### 命题 3 {#int-ix-s2-prop-3 .statement tag=09OO}

— 设 $\nu$ 为 T 上的测度。对于 $\nu$ 为形式 $f \cdot \mu$，其中 $f$ 是局部 $\mu$ 可积正值函数，则每个 $\mu$ 可忽略不计的紧集是充分必要的$\nu$-可以忽略不计。如果$f'$是第二个局部$\mu$可积函数，使得$\nu = f' \cdot \mu$，则$f = f'$局部$\mu$-几乎无处不在。

条件显然是必要的（命题 2）。相反，假设每个$\mu$可忽略不计紧集都是$\nu$可忽略不计。让我们为度量 $\mu + \nu$ 引入 T 的压榨 $(K_\alpha)_{\alpha \in A}$，并让我们集合 $N = T - \bigcup_{\alpha \in A} K_\alpha$。很明显，$(K_\alpha)_{\alpha \in A}$是对$\mu$和$\nu$的碾压，因此§1, No. 8的第9条命题意味着每个$g \in \mathscr{F}_+$有以下关系：

$$
\mu^\bullet(g) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(g_{K_\alpha}), \quad \nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}).
$$

考虑紧集$C \subset K_\alpha$即$\mu_{K_\alpha}$-可以忽略不计；那么 $C$ 局部 $\mu$ 可以忽略，因此局部 $\nu$ 可以忽略，最后 $\nu_{K_\alpha}$ 可以忽略 $\nu$ 的定义。然后从 Lebesgue-Nikodym 定理 (Ch. V, §5, No. 5, Th. 2) 可以得出，$\nu_{K_\alpha}$ 相对于 $\mu_{K_\alpha}$ 承认密度 $f_\alpha$。设$f$为函数即重合，其中集合$K_\alpha$各为$f_\alpha$，$N$为0； 函数 $f$ 是 $\mu$ 可测量的（第 IV, §5, No. 10，第 16 章），并且对于每一个函数 $g \in \mathscr{F}_+$，根据上述关系和第 16 章第 3 章，可测量。 V, §5, No. 3,

$$
\nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_\alpha g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet((f g)_{K_\alpha}) = \mu^\bullet(f g).
$$

那么首先，$f$是局部$\mu$可积的：如果$x$是T的点，并且如果$V$是$x$的邻域，使得$\nu^\bullet(V) < +\infty$，则$\mu^\bullet(f \varphi_V) < +\infty$。接下来，命题 2 表明测度$\nu$ 和$f \cdot \mu$ 具有相同的本质上积分。因此它们是相等的（§1, No. 2，Prop. 2 的 Cor.）。基于紧凑空间的情况，$f$的唯一性是明显的，命题成立。

注3)。 — 关于测量 $\nu = f \cdot \mu$ 约化的积分理论立即与第 1 章中处理的理论相关。 V。例如，令 $(K_\alpha)_{\alpha \in A}$ 为 T 对 $\mu$ 的压榨，因此也适用于 $\nu$，并令 $T'$ 为§1, No. 8 Scholium 中定义的局部紧致空间；我们可以将$\mu$（分别与$\nu$）与$T'$上的测量$\mu'$（分别与$\nu'$）相关联，这样，可测量的函数，本质上的可积函数和Banach空间中的值，以及基本的函数正函数的上积分对于$\mu$和$\mu'$（分别对于$\nu$和$\nu'$）是相同的。因此函数$f$是$\mu'$可测量的；它是局部$\mu'$可积的，因为$T'$是局部紧致的，并且$T'$的紧致子集仅与紧集$K_\alpha$（$\alpha \in A$）的有限数相交。最后，关系${\nu'}^\bullet(g) = \nu^\bullet(g) = \mu^\bullet(fg) = {\mu'}^\bullet(fg)$证明了$\nu' = f \cdot \mu'$（第V, §5, No. 3章，第3条命题）。我们将抄写第 1 章结果的任务留给读者。 V, §5。

### 3. 像一个小节

#### 定义 4 {#int-ix-s2-def-4 .statement tag=09OP}

设$\pi$为T的映射，形成拓扑空间X。有人说，如果$\pi$是$\mu$可测的，并且如果X的每个点 x 承认一个邻域V使得$\mu^\bullet(\overline{\pi}(V)) < +\infty$，那么$\pi$是$\mu$-适当的。

#### 注 1 {#int-ix-s2-n3-rem-1 .statement tag=09OQ}

当T和X局部紧致时，这个定义等价于Ch. V, §6, No. 1。

#### 注 2 {#int-ix-s2-n3-rem-2 .statement tag=09OR}

T 到 X 的真连续映射（GT，I, §10, No. 1，定义 1）是 $\mu$ - 对于每个小节 $\mu$ 都是正确的。对于，设 $x \in X$；由于 $\overline{\pi}(x)$ 是紧致的（前述，No. 2，Th.1），集合 $\overline{\pi}(x)$ 有一个开邻域 H，使得 $\mu^\bullet(H) < +\infty$。 集合$V = X - \pi(T - H)$；由于$\pi$闭，V在X、包含x开，并且满足$\overline{\pi}(V) \subset H$、从而$\mu^\bullet(\overline{\pi}(V)) \leq \mu^\bullet(H) < +\infty$。

#### 注 3 {#int-ix-s2-n3-rem-3 .statement tag=09OS}

如果$\mu$有界，则T到X的每个$\mu$可测映射都是$\mu$-本征。

#### 注 4 {#int-ix-s2-n3-rem-4 .statement tag=09OT}

如果 $\theta$ 是 T 上的复测度，如果 $\pi$ 对于正测度 $|\theta|$ 是正确的，则 $\pi$ 被称为 $\theta$-正确的。

#### 命题 4 {#int-ix-s2-prop-4 .statement tag=09OU}

令 $\pi$ 为 T 的 $\mu$-固有映射到拓扑空间 X。在X上存在且仅有一个测度$\nu$，使得$\nu^\bullet$等于像负担$\pi(\mu^\bullet)$（§1, No. 1），在其他字中，使得$\nu^\bullet(g) = \mu^\bullet(g \circ \pi)$对于所有$g \in \mathscr{F}_+(X)$。

唯一性是显而易见的（§1, No. 2，Prop. 2 的 Cor.）。为了证明存在性，我们首先要处理$\mu$被紧集 K携带的情况，使得$\pi$到K的限制是连续的。那么 $L = \pi(K)$ 是紧致的；令$\pi'$为由$\pi$诱导的K到L的连续映射，令$\nu'$为像在L上的测度$\pi'(\mu_K)$，$\nu$为由$\nu'$定义的X上的测度（§1, No. 3，例2）。对于每$g \in \mathscr{F}_+(X)$，

$$
\nu^\bullet(g) = {\nu'}^\bullet(g_L) = \mu_K^\bullet(g_L \circ \pi') = \mu_K^\bullet((g \circ \pi)_K) = \mu^\bullet((g \circ \pi)_K^0) = \mu^\bullet(g \circ \pi)
$$

（我们相继使用了§1, No. 3的公式（3）；V, §6, No. 2章的第2条；$\mu_K^\bullet$的定义；以及$\mu$由K携带的事实）。其他字、$\nu^\bullet = \pi(\mu^\bullet)$。

现在让我们讨论一般情况；通过道具。 §1, No. 8、$\mu$的10和9是紧支持度测度可求和族$(\mu_\alpha)_{\alpha \in A}$的和，使得$\pi$的限制到$\mu_\alpha$的支持$K_\alpha$对于每个$\alpha \in A$是连续的。上面处理的特殊情况允许将 T 上的每个度量 $\mu_\alpha$ 与 X 上的度量 $\nu_\alpha$ 关联，使得$\nu_\alpha^\bullet = \pi(\mu_\alpha^\bullet)$。那么，对于 $g \in \mathscr{F}_+(X)$，

$$
\sum_{\alpha \in A} \nu_\alpha^\bullet(g) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g \circ \pi) = \mu^\bullet(g \circ \pi).
$$

负担$\pi(\mu^\bullet)$是局部有界的，因为$\pi$是$\mu$-本征；因此，族$(\nu_\alpha)_{\alpha \in A}$是可求和的（§1, No. 7，命题7），并且它的和$\nu$满足叙述。

#### 定义 5 {#int-ix-s2-def-5 .statement tag=09OV}

*如果$\pi$是T的$\mu$-固有映射到拓扑空间X，X上的唯一测度$\nu$，使得所有$g \in \mathscr{F}_+(X)$的$\nu^\bullet(g) = \mu^\bullet(g \circ \pi)$被称为像测度$\mu$位于$\pi$之下，并表示为$\pi(\mu)$.*。

#### 例 {#int-ix-s2-n3-exa-1 .statement tag=09OW}

— 令 K 为 T 的紧凑子空间，将 K 的 i 典范嵌入引入 T，以及 $\lambda$ 对 K 的度量；因为 i 是连续的并且 $\lambda$ 有界，所以 i 是 $\lambda$-固有的。 §1, No. 3的公式(3)表明“由$\lambda$定义的T上的测度”是像测度$i(\lambda)$。

*注 5).* — 如果 $\theta$ 是实测度且 $\pi$ 是 $\theta$-真测度，则 $\pi$ 对于测度 $\theta^+$ 和 $\theta^-$ 是真测度；然后集合 $\pi(\theta) = \pi(\theta^+) - \pi(\theta^-)$。如果$\theta$是复测度并且$\pi$是$\theta$-真测度，则$\pi$对于实际测度$\Re(\theta)$和$\Im(\theta)$是真测度；一然后集合

$$
\pi(\theta) = \pi(\Re(\theta)) + i \pi(\Im(\theta)).
$$

#### 命题 5 {#int-ix-s2-prop-5 .statement tag=09OX}

*设 $\pi$ 为 T 的 $\mu$-固有映射 ，形成拓扑空间 X，并设 f 为 X 的映射 ，形成拓扑空间 F（是否为 Hausdorff）。为了使 f $\pi(\mu)$ 可测，$f \circ \pi$ $\mu$ 可测是充分必要的。*

让我们再次讨论第4条命题的证明，并从开头处理的特殊情况开始，同样的记号； g 对于测量 $\pi(\mu) = \nu$ 是可测量的，当且仅当 $g_L$ 是 $\nu'$ 可测量时（§1, No. 5，*例*）；现在，这相当于$g_L \circ \pi' = (g \circ \pi)_K$是$\mu_K$可测量的说（第V, §6, No. 2，第3章），最后，$g \circ \pi$是$\mu$可测量（§1, No. 5，*例*）。现在让我们讨论一般情况，与第 4 条的证明相同的记号； f 是 $\nu$ 可测当且仅当 f 对于每个 $\alpha \in A$ 是 $\nu_\alpha$ 可测（§1, No. 7，命题 8），因此当且仅当 $f \circ \pi$ 对于每个 $\alpha \in A$ 是 $\mu_\alpha$ 可测（前面的特殊情况），最后当且仅当$f \circ \pi$ 是 $\mu$ 可测量的（$§ 1$、No. 7，第 8 条）。

#### 推论{#int-ix-s2-n3-cor-1 .statement tag=09OY}

— *令X和Y为两个拓扑空间，$\pi$将T的$\mu$-固有映射引入X，并将$\pi'$将X的$\pi(\mu)$-固有映射引入Y. 映射 $\pi'' = \pi' \circ \pi$ 则为 $\mu$ 正值，以及 $\pi''(\mu) = \pi'(\pi(\mu))$（“措施像的传递性”）。

因为，$\pi''$ 是 $\mu$ 可测量的（命题 5）。 集合$\mu' = \pi(\mu)$； 像负担$\pi'({\mu'}^\bullet) = \pi'(\pi(\mu^\bullet))$显然等于$\pi''(\mu^\bullet)$。由于它是局部有界的，所以$\pi''$是$\mu$-固有的。度量$\pi''(\mu)$和$\pi'(\mu')$则具有相同的基本上积分，因此是相等的。

#### 命题 6 {#int-ix-s2-prop-6 .statement tag=09OZ}

— *令$\pi$为T的$\mu$-固有映射到拓扑空间X，并令B为X的$\pi(\mu)$可测子集。 集合 $A = \overline{\pi^{-1}(B)}$，并用 A 到 B 的 $\pi'$ 映射表示重合和 A 上的 $\pi$。集合 A 则$\mu$ 可测，$\pi_A$ 和 $\pi'$ 为$\mu_A$-正确，并且*

$$
(\pi(\mu))_B = (\pi_A(\mu_A))_B = \pi'(\mu_A).
$$

集合 A 是 $\mu$-可通过应用于 $\varphi_B$ 的第 5 条命题进行测量； 映射 $\pi_A$ 显然可以通过定义诱导测度 (No. 1) 进行$\mu_A$ 测量，因此$\pi'$ 是可测量的。设$f$为$\mathscr{F}_+(B)$中的元素；在 X 和 T 中用零指数扩张表示 0，我们有

$$
(\pi(\mu)_B)^\bullet(f) = \pi(\mu)^\bullet(f^0) = \mu^\bullet(f^0 \circ \pi) = \mu^\bullet((f \circ \pi')^0) = \mu_A^\bullet(f \circ \pi'),
$$

从而$(\pi(\mu)_B)^\bullet = \pi'(\mu_A^\bullet)$。由于负担$(\pi(\mu)_B)^\bullet$是局部有界的，$\pi'(\mu_A^\bullet)$也是如此，因此$\pi'$是$\mu_A$-本征。度量$\pi'(\mu_A)$和$(\pi(\mu))_B$具有相同的基本上积分，因此相等。其它关系可以类似的方式建立。

#### 命题 7 {#int-ix-s2-prop-7 .statement tag=09P0}

— *令 T 为拓扑空间 X 的子空间，并令 i 为 T 到 X 的单射。

a) *如果$\mu$是T上的一个测度，并且如果i是$\mu$-真值，那么测度$i(\mu)$集中在T上，并且一个有$(i(\mu))_T = \mu$。

b) *如果$\lambda$是X的测度，使得T是$\lambda$可测的，那么i是$\lambda_T$-真值，且$i(\lambda_T) = \varphi_T \cdot \lambda$。

a）集合$\nu = i(\mu)$； 关系$\nu^\bullet(A) = \mu^\bullet(A \cap T)$应用于$A = X - T$，表明$\nu$集中在T上。关系$\nu_T = \mu$是关系（2）在取$B = T = A$时的特例。

b) 令$f$为定义在X上的正函数； 设定 $\mu = \lambda_T$，一个有 $\mu^\bullet(f \circ i) = \lambda_T^\bullet(f_T) = \lambda^\bullet(f \varphi_T) \leq \lambda^\bullet(f)$（命题 1）；由此可见 i 是 $\mu$ 正确的。另一方面，$\mu^\bullet(f \circ i)$（或$\lambda^\bullet(f \varphi_T)$）是$f$相对于$i(\mu)$（或$\varphi_T \cdot \lambda$）的本质上积分。因此，这两个措施是相等的。

*注 6).* — 设$\pi$是$T$的$\mu$真映射到拓扑空间$X$。一个约化关于像测量$\nu = \pi(\mu)$的积分理论在第1章中处理的理论。 V, §6，按以下方式。令$(K_\alpha)_{\alpha \in A}$（或$(L_\beta)_{\beta \in B}$）是$T$（或$X$）对$\mu$（或$\nu$）和集合$N = T - \bigcup_{\alpha \in A} K_\alpha,\ P = X - \bigcup_{\beta \in B} L_\beta$的压榨。我们可以假设$\pi$到每个$K_\alpha$的限制是连续的（§1, No. 8，命题10）。令$T', X'$为在§1, No. 8的Scholium中构造的局部紧凑空间，并令$\mu'$和$\nu'$为与$\mu$和$\nu$相关的这些空间的度量。 $T'$的拓扑是子空间$K_\alpha$拓扑的和和$N$上的离散拓扑，$\pi$是$T'$到$X$的连续映射并且关系 ${\mu'}^\bullet(g \circ \pi) = \mu^\bullet(g \circ \pi) = \nu^\bullet(g)$（对于 $g \in \mathscr{F}_+(X)$）表明 $\pi$ 是 $\mu'$ 正确且 $\pi(\mu') = \nu$。另一方面，$X$到$X'$的恒等映射$i$是$\nu$-本征，并且$i(\nu) = \nu'$。由此可见，$\pi$是$T'$到$X'$的$\mu'$固有映射，$\pi$下的$\mu'$的像是$\nu'$（第5条的Cor.）。我们将抄写第 1 章结果的任务留给读者。 V, §6。

### 4. 解除措施

#### 命题 8 {#int-ix-s2-prop-8 .statement tag=09P1}

*设$T$和$X$为$T$到$X$的两个拓扑空间、$\pi$映射。

a) 令 $\nu$ 为 $X$ 上的有界测度。在阶中，存在$T$上的测度$\mu$使得$\pi$是$\mu$-适当且$\pi(\mu) = \nu$，对于每个数$\varepsilon > 0$，存在紧集$K_\varepsilon \subset T$是充分必要的这样$\pi$到$K_\varepsilon$的限制是连续的并且$\nu^\bullet(X - \pi(K_\varepsilon)) < \varepsilon$。

b) 假设$\pi$是单射的；令$\mu$和$\mu'$是$T$的两个度量，使得$\pi$适合$\mu$和$\mu'$，并且$\pi(\mu) = \pi(\mu')$。然后$\mu = \mu'$。

*a)* 中所述的条件是必要的。因为，如果 $\pi$ 是$\mu$-真值且$\pi(\mu) = \nu$，则关系 $\mu^\bullet(1) = \nu^\bullet(1) < +\infty$ 意味着$\mu$ 有界。 §1, No. 2的命题2应用于函数1，意味着存在$T$的紧致子集$K$，使得$\mu^\bullet(T - K) < \varepsilon/2$。由于$\pi$是$\mu$可测的，因此存在紧集$K_\varepsilon \subset K$，使得$\pi$到$K_\varepsilon$的限制是连续的，并且使得$\mu^\bullet(K - K_\varepsilon) < \varepsilon/2$。那么（No. 3，命题 4）

$$
\nu^\bullet(X - \pi(K_\varepsilon)) = \mu^\bullet(T - \overline{\pi}^{-1}(\pi(K_\varepsilon))) < \varepsilon.
$$

为了证明条件是足够的，我们首先处理一个特殊情况。

#### 引理 1 {#int-ix-s2-lem-1 .statement tag=09P2}

令U和V是两个紧凑的空间，h是U在V上的连续映射。 $\mathscr{M}_+(U)$到$\mathscr{M}_+(V)$的映射$\lambda \mapsto h(\lambda)$则为满射。

对于，设a为$\mathscr{C}(V)$的线性映射$f \mapsto f \circ h$入$\mathscr{C}(U)$；由于 h 是满射，a 是 $\mathscr{C}(V)$ 到 $\mathscr{C}(U)$ 的子空间 H 的等距。令$\theta$为V的正测度；那么 $\theta \circ a^{-1}$ 是 H 上的连续线性形式，凭借 Hahn–Banach 定理（TVS，II, §3, No. 2，Th. 1 的 Cor. 3），它可以扩展到 $\mathscr{C}(U)$ 上的线性形式 $\eta$，具有相同的范数； $\eta$ 是对 U 的度量，$\theta(f) = \eta(f \circ h)$ 是所有 $f \in \mathscr{C}(V)$ 的度量，因此 $\theta = h(\eta)$。最后，$\theta(1) = \| \theta \| = \| \eta \|$和$\theta(1) = \eta(1)$，因此$\eta$为正（第V, §5, No. 5章，第9条命题）。

现在让我们证明a)中所述条件的充分性。 条件意味着T的紧凑子集存在序列$(K_n)_{n \geq 1}$，使得$\pi$的限制对于每个$K_n$是连续的，并且对于每个$n$，$\nu^\bullet(X - \pi(K_n)) < 1/n$。 序列 $(K_n)$ 可以假设为递增。 集合 $L_n = \pi(K_n)$ 并用 $\nu'_n$ 表示$L_n$ 上的测量$\varphi_{L_n - L_{n-1}} \cdot \nu_{L_n}$，并遵循惯例 $L_0 = \varnothing$。

限制 $\pi_{K_n}$ 是连续的，$K_n$ 上存在测度 $\mu'_n$ 使得 $\pi_{K_n}(\mu'_n) = \nu'_n$ (引理 1)。令T中$K_n$的典范嵌入下的$\mu_n$为$\mu'_n$的像，并令g为$\mathscr{F}_+(X)$的元素。相继利用$\nu$集中于$\bigcup L_n$的事实，§1, No. 5的命题4； §1, No. 2第2号提案； No. 3的第4条命题，最后是No. 3的第7条命题，我们有

$$
\nu^\bullet(g) = \sum_n \nu^\bullet(\varphi_{L_n - L_{n-1}} g) = \sum_n \nu'_n \bullet (g_{L_n}) = \sum_n \mu'_n \bullet (g_{L_n} \circ \pi_{K_n})
$$
$$
= \sum_n \mu'_n \bullet ((g \circ \pi)_{K_n}) = \sum_n \mu_n^\bullet (g \circ \pi).
$$

在这个公式中取$g = 1$，我们可以看到族$(\mu_n)$是可求和的，并且它的和是一个有界测度$\mu$（§1, No. 7，命题7）。根据No. 3的命题5，映射$\pi$对于所有$n$来说是$\mu_n$可测的，因为$\pi_{K_n}$是连续的，因此$\mu'_n$是可测的；由此可见 $\pi$ 是 $\mu$ 可测的（§1, No. 7，命题 8），因此 $\mu$ 是正确的，因为 $\mu$ 是有界的。上述关系则证明测度$\pi(\mu)$和$\nu$具有相同的本质上积分，因此是相等的（§1, No. 2，命题2的​​Cor.）。

最后，假设$\pi$是单射的，并证明b)。令 f 为 $\mathscr{F}_+(T)$ 的元素；由于$\pi$是单射的，因此存在函数$g \in \mathscr{F}_+(X)$使得$f = g \circ \pi$和设定$\nu = \pi(\mu) = \pi(\mu')$，根据No. 3的第4条命题我们有

$$
\mu^\bullet(f) = \mu^\bullet(g \circ \pi) = \nu^\bullet(g) = {\mu'}^\bullet(g \circ \pi) = {\mu'}^\bullet(f).
$$

因此，两个测度$\mu$和$\mu'$具有相同的基本上积分，这意味着它们的等式（§ 1, No. 2，Prop.2的Cor.）。

#### 注 {#int-ix-s2-n4-rem-1 .statement tag=09P3}

假设 $\pi$ 是单射的。令$\theta$为复测度，使得$\pi$为$\theta$真值且为$\pi(\theta) = 0$；然后$\theta = 0$。事实上，通过将$\theta$分为实数和虚数部分，我们可以将约化转化为$\theta$是实数的情况。然后我们有$\pi(\theta^+) = \pi(\theta^-)$，因此有$\theta^+ = \theta^-$（命题8），最后是$\theta = 0$。

这是一个重要的情况，其中第 8 条的条件 a) 总是满足的。

#### 命题 9 {#int-ix-s2-prop-9 .statement tag=09P4}

— *设 T 为 Souslin 空间* (GT, IX, §6, No. 2, Def. 2), *X Hausdorff 空间*, $\pi$ *T 到 X* 上的连续映射，以及 $\nu$ *上的有界测度X*。 *那么 T 上存在有界测度 $\mu$ 使得 $\pi(\mu) = \nu$*。

这些假设显然暗示X是苏斯林空间。

让我们考虑$\mathfrak{P}(T)$上的集合函数$c : A \mapsto \nu^\bullet(\pi(A))$。 关系 $A \subset B$ 意味着 $c(A) \leq c(B)$；如果$(A_n)$是T的子集的递增序列，并且如果$A = \bigcup_{n \in \mathbf{N}} A_n$，则$c(A) = \sup_n c(A_n)$来自$\nu^\bullet$是负担。最后，令$A \subset T$、$\varepsilon$为数$> 0$； 选择 X 包含 $\pi(A)$ 的开子集 G，使得 $\nu^\bullet(G) \leq \nu^\bullet(\pi(A)) + \varepsilon$（§ 1, No. 9，命题 13）； T 包含 A 的开路子集 $H = \overline{\pi^{-1}(G)}$ 和 $c(H) \leq c(A) + \varepsilon$。因而，函数 c 是 T (TG, IX, §6, No. 10, Def. 9)(1) 上的右连续容量，而定理的容量 (*loc. cit.*, Th. 6) 意味着等式 $c(T) = \sup_K c(K)$，其中 K 超过紧凑子集的集合 T. 命题 8 则暗示了所需测度 $\mu$ 的存在。

### 5. 乘积两小节

设S和T为两个拓扑空间，分别配备两个（正）预测$\lambda$和$\mu$，并令X为乘积空间$S \times T$。令 K 为 X 的紧凑子集；让我们分别用A和B表示K在S和T上的投影，以及集合

$$
\nu_K = (\lambda_A \otimes \mu_B)_K .
$$

因而，我们将定义作为X的预测。例如，令L为X包含K的紧子集，并令C和D为其两个投影；然后$A \subset C$，$B \subset D$，

(1) 如果对于 T 中的每个紧集 K，当 U 越过开路集合 $U \supset K$ 时，$f(K) = \inf_U f(U)$，则称 T 上的容量 $f$ 是右连续的。 GT 中没有定义这个概念，翻译自 Ch 的早期版本。 IX。

因而，使用传递性诱导措施，以及第 12 章的 Prop. 12。 V, §8, No. 5，我们有

$$
(\nu_L)_K = ((\lambda_C \otimes \mu_D)_L)_K = (\lambda_C \otimes \mu_D)_K \\
= ((\lambda_C \otimes \mu_D)_{A \times B})_K = (\lambda_A \otimes \mu_B)_K = \nu_K .
$$

#### 定义 6 {#int-ix-s2-def-6 .statement tag=09P5}

*式(3)定义的预测值$\nu$称为$\lambda$和$\mu$的乘积预测值，记作$\lambda \otimes \mu$。*

对于$\lambda$和$\mu$是复杂预测措施的情况，定义显然是扩展，然后有$|\lambda \otimes \mu| = |\lambda| \otimes |\mu|$（第III, §4, No. 2，第3章和第IV, §5, No. 7，引理3）。

我们保留 Ch 的记号。 III, §4 和章。 V, §8 相对于乘积测量和迭代积分。特别地，如果$f$和$g$是分别定义在$S$和$T$上的两个函数，且值在$\overline{\mathbf{R}}_+$或$\mathbf{C}$中，则函数$(s, t) \mapsto f(s)g(t)$在$S \times T$ 将表示为 $f \otimes g$。

#### 命题 10 {#int-ix-s2-prop-10 .statement tag=09P6}

*令$\nu$为$\lambda$和$\mu$的乘积预量度；对于每个函数 $f \in \mathscr{F}_+(S)$ 和每个函数 $g \in \mathscr{F}_+(T)$，*

$$
\nu^\bullet(f \otimes g) = \lambda^\bullet(f)\mu^\bullet(g) .
$$

*预测值 $\nu$ 是 $S \times T$ 上唯一满足 (4) 的预测值。*

由于$K$（或$L$）超过$S$（或$T$）的紧致子集的集合，我们有

$$
\begin{align*}
\nu^\bullet(f \otimes g) &= \sup_{K,L} \nu^\bullet_{K \times L}((f \otimes g)_{K \times L}) = \sup_{K,L} (\lambda_K \otimes \mu_L)^\bullet(f_K \otimes g_L) \\
&= \sup_{K,L} \lambda_K^\bullet(f_K) \cdot \mu_L^\bullet(g_L) = (\sup_K \lambda_K^\bullet(f_K)) (\sup_L \mu_L^\bullet(g_L)) \\
&= \lambda^\bullet(f)\mu^\bullet(g)
\end{align*}
$$

由第 8 章第 8 条提案V, §8, No. 3。

设$\eta$为$S \times T$满足 (4) 上的第二个预测值，并令$K$和$L$分别为$S$和$T$的紧子集，$f$和$g$元素分别为$\mathscr{F}_+(K)$和$\mathscr{F}_+(L)$。 关系 $(f \otimes g)^0 = f^0 \otimes g^0$ 在扩张之间除 0，因此（§1, No. 2，命题 2）

$$
\eta^\bullet_{K \times L}(f \otimes g) = \eta^\bullet((f \otimes g)^0) = \eta^\bullet(f^0 \otimes g^0) \\
= \lambda^\bullet(f^0)\mu^\bullet(g^0) = \lambda_K^\bullet(f)\mu_L^\bullet(g) .
$$

特别是，如果取$f \in \mathscr{K}_+(K)$、$g \in \mathscr{K}_+(L)$，则可以看到$\eta_{K \times L}$具有乘积度量$\lambda_K \otimes \mu_L$的特征性质（第III, §4, No. 1，Th.1）。因此$\eta_{K \times L} = \nu_{K \times L}$；由于$S \times T$的每个紧凑子集都包含在形式$K \times L$的集合中，因此诱导措施的传递性意味着$\eta = \nu$。

#### 推论 1 {#int-ix-s2-prop-10-cor-1 .statement tag=09P7}

— *如果 $\lambda$ 和 $\mu$ 是度量，则 $\nu$ 是一个度量。*

例如，令$x = (s, t)$为$X$的点，并令$U$和$V$分别为$s, t$的邻域，使得$\lambda^\bullet(U) < +\infty$、$\mu^\bullet(V) < +\infty$； 集合$U \times V$是$x$和$\nu^\bullet(U \times V) = \lambda^\bullet(U)\mu^\bullet(V) < +\infty$的邻域（4）；因此，负担$\nu^\bullet$是局部有界的，而预测措施$\nu$是一个测度。

对于复杂的措施来说，这个结果立即扩展。

#### 推论 2 {#int-ix-s2-prop-10-cor-2 .statement tag=09P8}

— *如果 $A$ 是 $S$ 的子集对于 $\lambda$ 局部可忽略不计，则 $A \times T$ 局部 $\nu$ 可忽略不计。*

#### 推论 3 {#int-ix-s2-prop-10-cor-3 .statement tag=09P9}

— *假设$\lambda$（或$\mu$）是$S$（或$T$）上的可求和族$(\lambda_\alpha)_{\alpha \in A}$（或$(\mu_\beta)_{\beta \in B}$）的和。然后族 $(\lambda_\alpha \otimes \mu_\beta)_{(\alpha, \beta) \in A \times B}$ 可求和，其和为 $\lambda \otimes \mu$。*

例如，令 $p$ 为负担$\sum_{\alpha, \beta} (\lambda_\alpha \otimes \mu_\beta)^\bullet$；如果$f \in \mathscr{F}_+(S)$和$g \in \mathscr{F}_+(T)$，那么显然是$p(f \otimes g) = \lambda^\bullet(f)\mu^\bullet(g)$。 Cor 的证明。然后，1 表明 $p$ 是局部有界的，因此族 $(\lambda_\alpha \otimes \mu_\beta)$ 是可求和的（§ 1, No. 7，命题 7）。它的和$\eta$则满足$\eta^\bullet = p$（§ 1, No. 7，第7条命题），而第10条命题意味着$\eta = \nu$。

### 6. 两个度量关于乘积的积分

*在本编号中，$\lambda$和$\mu$分别表示$S$和$T$的措施，$\nu$表示乘积对$S \times T$的措施$\lambda \otimes \mu$。在加法中，如果$f$在$S \times T$上是正函数，则对于每个$s \in S$，我们在$T$上用$f_s$函数$t \mapsto f(s, t)$表示，并用$I_f$函数表示$s \mapsto \mu^\bullet(f_s)$ $S$。*

#### 引理 2 {#int-ix-s2-lem-2 .statement tag=09PA}

*令$f$为$S \times T$上的$\nu$可测量正函数；对于$T$的每个紧凑子集$L$，令$I_f^L$为$S$上的函数$s \mapsto \mu^\bullet(f_s \varphi_L)$。那么函数$I_f^L$是$\lambda$可测的，并且*

$$
(5) \quad I_f = \sup_L I_f^L
$$
$$
(6) \quad \nu^\bullet(f) = \sup_L \lambda^\bullet(I_f^L),
$$

*其中 $L$ 超过集合的紧凑型子集或 $T$。*

我们首先注包含$L \subset L'$意味着$I_f^L \leq I_f^{L'}$；另一方面，$I_f^L(s) = \mu_L^\bullet((f_s)_L)$适用于所有$s \in S$。因此，公式 (5) 是 $\mu^\bullet$ 的定义的直接的推论，如下所示

§1, No. 2。如果 K 是 S 的紧致子集，且 L T 的紧致子集，则 $\nu_{K \times L} = \lambda_K \otimes \mu_L$ 乘以构造，且第 7 章的命题 7。 V, §8, No. 3 意味着关系

$$
\nu^\bullet(f \varphi_{K \times L}) = \lambda_K^\bullet((I_f^L)_K).
$$

而且，$S \times T$的每个紧凑子集都包含在形式$K \times L$的紧集中； 经过到前面公式中所有 K 和 L 的上包络线，因此我们得到

$$
\nu^\bullet(f) = \sup_L \sup_K \lambda_K^\bullet((I_f^L)_K) = \sup_L \lambda^\bullet(I_f^L),
$$

即(6)。

最后，第 7 章的提案 7。 V, §8, No. 3意味着$I_f^L$的限制对于S的每个紧致子集K都是$\lambda_K$可测的；这相当于说 $I_f^L$ 是 $\lambda$ 可测量的。

#### 命题 11 {#int-ix-s2-prop-11 .statement tag=09PB}

*设f是定义在$X = S \times T$上的下半连续函数$\geqslant 0$。*

a) *对于每个 $s \in S$，函数 $f_s : t \mapsto f(s, t)$ 在 T 上是下半连续的。*

b) *函数 $I_f : s \mapsto \int^\bullet f(s, t) d\mu(t)$ 在 S 上是下半连续，并且*

$$
\iint_X^\bullet f(s, t) d\nu(s, t) = \int_S^\bullet d\lambda(s) \int_T^\bullet f(s, t) d\mu(t).
$$

性质 *a)* 是显而易见的，因为 T 到 $\overline{\mathbf{R}}$ 的映射 $t \mapsto f(s, t)$ 是 $f$ 的合成，并且 T 到 X 的连续映射 $t \mapsto (s, t)$。为了建立 *b)*，我们将利用引理：

#### 引理 3 {#int-ix-s2-lem-3 .statement tag=09PC}

— *令 X 为拓扑空间（或非豪斯多夫），f 定义于 X 的下半连续函数 $\geqslant 0$；那么 f 是X上下半连续函数的递增序列$(f_n)_{n \in \mathbf{N}}$的极限，使得每个函数$f_n$都是线性组合，具有正系数， 特征函数开放集合.*

给定两个整数$k \geqslant 1$和$n \geqslant 1$，让我们用$J_{kn}$表示$\overline{\mathbf{R}}$的区间$]k/2^n, +\infty]$的特征函数。每$x \in \overline{\mathbf{R}}_+$、集合

$$
u_n(x) = 2^{-n} \sum_{k=1}^{n \cdot 2^n} J_{kn}(x);
$$

直接的序列 $(u_n(x))_{n \geqslant 1}$ 是递增并且承认 x 为极限。因而，函数$f_n = u_n \circ f$的序列是递增，并且收敛到$f$，并且有$f_n = 2^{-n} \sum_{k=1}^{n \cdot 2^n} \varphi_{U(k,n)}$，
其中$U(k,n)$是$X$的开集合$f^{-1}([k/2^n, +\infty])$。

让我们转到 b) 的证明。 函数$I_f$是函数$I_f^L$递增定向族的上层信封，其中$L$运行在$T$（引理2）的紧凑子集的集合之上，足以证明函数 $I_f^L$ 是下半连续；然后可以从 (6) 通过经过将公式 (9) 推导出到 $L$ 上的上包络线（§ 1, No. 6，命题 5）。

因而，令$\mathscr{H}$为$S \times T$上的正下半连续函数$f$的集合，使得$I_f^L$对于$T$的每个紧致子集$L$都是下半连续。根据§ 1, No. 6第5条，$\mathscr{H}$属于到$\mathscr{H}$的元素每递增有向集合的上界。因而，到引理 3，就足以证明$S \times T$属于到$\mathscr{H}$的开集合$W$的特性函数。另外，$S \times T$乘积拓扑定义，集合$W$为递增定向家庭并形式开放集合$(W_\alpha)_{\alpha \in A}$
$$
W = \bigcup_{1 \leq i \leq n} (U_i \times V_i),
$$
其中$U_i$在$S$开放，$V_i$在$T$开放；通过上面的注，足以表明这样一个开集合属于到$\mathscr{H}$的特征函数。设$s \in S$，并令$U$为由开集合$U_i$包含$s$形成的族（可能为空）的交；人们立即看到，$\varphi_W(s,t) \leq \varphi_W(s',t)$对于所有$s' \in U$和$t \in T$，从而，通过积分，$I_{\varphi_W}^L(s) \leq I_{\varphi_W}^L(s')$对于所有$s' \in U$。因而$I_{\varphi_W}^L$是下半连续的，命题成立。

#### 推论 1 {#int-ix-s2-lem-3-cor-1 .statement tag=09PD}

*设$f$为$X = S \times T$上定义的正数函数；那么*
$$
\iint_X^* f(s,t)\, d\nu(s,t) \geq \int_S^* d\lambda(s) \int_T^* f(s,t)\, d\mu(t).
$$

对于，令$g$是$X$上的下半连续函数，使得$g \geq f$；根据第 11 号提案，
$$
\iint_X^* g(s,t)\, d\nu(s,t) = \iint^* g(s,t)\, d\nu(s,t) = \int^* d\lambda(s) \int^* g(s,t)\, d\mu(t)
$$
$$
= \int^* d\lambda(s) \int^* g(s,t)\, d\mu(t) \geq \int^* d\lambda(s) \int^* f(s,t)\, d\mu(t).
$$
不等式 (10) 是通过经过到$g$ 的下包络线获得的。

#### 推论 2 {#int-ix-s2-lem-3-cor-2 .statement tag=09PE}

— 令 $f$ 为在 $S \times T$ 和 $\nu$ 上定义的数值函数，可忽略不计。那么函数$f_s : t \mapsto f(s, t)$是$\mu$——对于$\lambda$来说可以忽略不计——几乎每一个$s \in S$。

#### 命题 12 {#int-ix-s2-prop-12 .statement tag=09PF}

— 令 $f$ 为在 $X = S \times T$ 上定义的$\nu$可测量正函数。假设 $f$ 是 $\nu$ 调节的（分别是 $\mu$ 调节的）。然后：
a) $s \in S$的集合$N$使得函数$f_s : t \mapsto f(s, t)$不是$\mu$可测量，对于$\lambda$来说是可忽略的（或局部可忽略的）。
b) 映射 $s \mapsto \int^\bullet f(s, t) \, d\mu(t)$ 是 $\lambda$ 可测量的，并且

$$
\iint_X^\bullet f(s, t) \, d\nu(s, t) = \int_S^\bullet d\lambda(s) \int_T^\bullet f(s, t) \, d\mu(t).
$$

我们首先建立 b)，当 $f$ 是 $\nu$ 时。到引理 2，当存在$T$的紧子集$L$使得$f$在$S \times L$之外是零时，叙述的部分有效；对于，在这种情况下，$I_f = I_f^{L'}$对于$T$包含$L$的每个紧凑子集$L'$，以及公式（11）约化到（6）。特别是，b) 是针对函数 $f$ 建立的，即零在$S \times T$ 的紧凑子集之外。另一方面，科。命题 11 的 1 意味着当 $f$ $\nu$ 可以忽略不计时，b) 为真。由于每个$\nu$-调节的函数都是$\nu$-可忽略不计的函数的和和带有紧凑支持的函数的序列（§ 1, No. 9，第14号提案的Cor.3），断言b）为真当 $f$ 是 $\nu$ 时。

类似地，当 $\mu$ 由 $T$ (引理 2) 的紧凑型子集 $L$ 承载时，断言 b) 是显而易见的。假设 $\mu$ 已被审核；则在 $T$ 上存在序列 $(\mu_n)_{n \in \mathbf{N}}$ 具有紧凑支持的测度，例如 $\mu = \sum_n \mu_n$（§ 1, No. 9，第 14 号提案的 Cor. 5），从而 $\nu = \sum_n \lambda \otimes \mu_n$（No. 5，第 10 号提案的 Cor. 3）。 断言 b) 对$\nu_n = \lambda \otimes \mu_n$ 的每项措施都有效，也对$\nu = \sum_n \nu_n$ 有效。

让我们证明a）；用$s \in S$的$N$集合表示，使得$f_s$不可测$\mu$；对于$T$的每个紧凑子集$L$，类似地用$s \in S$的$N_L$集合表示，使得$f_s \varphi_L$不是$\mu$可测的。如果$K$和$L$分别在$S$和$T$中为紧集，则$f_{K \times L}$相对于测量$\nu_{K \times L} = \lambda_K \otimes \mu_L$是可测量的，并且第2章的命题2。 V, § 8, No. 2表明集合$N_L$对于$\lambda_K$来说局部可以忽略不计；由于$K$是任意的，$N_L$局部$\lambda$可以忽略不计。

假设$f$是零在形式$K \times L$的紧集之外；则$N = N_L$，且$N$包含在$K$中；由此可见 $N$ $\lambda$ 可以忽略不计。类似地，如果 $f$ 是 $\nu$-可以忽略不计，Cor.第 11 条命题第 2 条暗示 $N$ $\lambda$ 可以忽略不计。结合前面的两种情况，$f$ 是 $\nu$ 调节的情况可以如上所述进行处理。

假设$\mu$由$T$的紧致子集$L$承载；然后再次$N = N_L$，因此$N$在本地$\lambda$可以忽略不计。由于每个经过调节的措施都是具有紧凑支持的措施的序列中的和（$§ 1$，No. 9，第14号提案的Cor.5），因此在使用$§ 1$的第8号提案时，对于$\mu$经过调节的情况，这个结果立即扩展， No. 7。

#### 注 {#int-ix-s2-n6-rem-1 .statement tag=09PG}

— 令 $(K_\alpha)_{\alpha \in A}$ 为 $S$ 对 $\lambda$ 的压榨，并令 $M = S - \bigcup_{\alpha \in A} K_\alpha$； 定义以类似的方式$(L_\beta)_{\beta \in B}$和$N$用于$T$上的措施$\mu$。我们用$S'$表示局部紧致空间，即子空间$K_\alpha$或$S$的和和*离散*空间$M$； 空间$T'$的定义类似，我们集合$X' = S' \times T'$。局部紧凑空间$X'$是$X$的紧凑子空间族$(K_\alpha \times L_\beta)_{(\alpha, \beta) \in A \times B}$的和和子空间$P = (M \times T) \cup (S \times N)$，这是局部$\nu$可忽略的子集 $X$（观察到$P$通常不是离散的空间）。我们在$§ 1$、No. 8的*Scholium*中看到，在$S'$上存在一个测度$\lambda'$，使得可测函数、正函数的本质上积分、本质可积函数及其积分对于$\lambda$和$\lambda'$。我们将$T'$上的措施$\mu'$与$\mu$相关联，将$X'$上的$\nu'$与$\nu$相关联，与引用的Scholium一致；人们立即看到${\nu'}^\bullet(f \otimes g) = {\lambda'}^\bullet(f) {\mu'}^\bullet(g)$代表$f \in \mathscr{F}_+(S)$和$g \in \mathscr{F}_+(T)$；因此，根据No. 5第10号提案，$\nu' = \lambda' \otimes \mu'$。由于$X'$的拓扑比$X$的更细大，因此每个$\nu$调节的函数都是$\nu'$调节的。该程序允许在没有新的证明 Lebesgue–Fubini 定理（第V、$§ 8$、No. 4、Th.1）的情况下扩展到目前的情况。

### 7. 措施分解的结果

#### 命题 13 {#int-ix-s2-prop-13 .statement tag=09PH}

*令$X$为拓扑空间，$\nu$为$X$、$p$将$X$的$\nu$-固有映射调整为拓扑空间$T$，并且$\mu = p(\nu)$。假设 $X$ 的每个紧凑子空间都是可度量的。那么$T$到$\mathscr{M}_+(X)$中存在映射$t \mapsto \lambda_t$，具有以下性质：

a) 对于每个$t \in T$，测量$\lambda_t$由$\overline{p}^{-1}(t)$携带；
b) 对于$X$上的每个普遍可测$^{(1)}$正函数$f$，函数$t \mapsto \lambda_t^\bullet(f)$在$T$上普遍可测并且*

$$
\int_X f(x)\, d\nu(x) = \int_T d\mu(t) \int_X f(x)\, d\lambda_t(x);
$$

(1) 如果拓扑空间 $X$ 到拓扑空间 $Y$ 的映射被称为“普遍可测”，如果对于 $X$ 上的每个测度 $\mu$ $\mu$ 可测（cf. Ch. 1）。 V、$§ 3$、No. 4）。

c) $t \in T$的集合使得$\lambda_t(1) \neq 1$局部$\mu$可以忽略不计。
此外，如果$t \mapsto \lambda'_t$是$T$的映射进入$\mathscr{M}_+(X)$满足条件a)和b)，集合$t \in T$，使得$\lambda_t \neq \lambda'_t$局部$\mu$可以忽略不计。
我们需要一个辅助结果：

#### 引理 4 {#int-ix-s2-lem-4 .statement tag=09PI}

令$X$为拓扑空间，$\nu$为$X$的测度，$f$将$X$的$\nu$可测量映射转换为拓扑空间$F$（豪斯多夫或非豪斯多夫）。存在一个普遍可测量的映射 $f'$，即 $X$ 到 $F$，局部等于 $f$ $\nu$——几乎在任何地方。

证明与第 7 章的命题 7 相同。 V, §3, No. 4，考虑到§1, No. 8的第10号提案。

让我们讨论第 13 条命题的证明。
A) 假设 $X$ 是紧致且可度量的，并且 $p$ 是连续且满射的：
空间 $T$ 是紧凑且可度量的（GT，IX, §2, No. 10）。由 Th.第 1 章。 VI, §3, No. 1，存在$T$的映射$H : t \mapsto \eta_t$进入$\mathscr{M}_+(X)$，模糊地$\mu$可测量并且基本上标量$\mu$可积，使得$\nu = \int_T \eta_t \, d\mu(t)$并且使得$\eta_t$的总质量为1并且由每 $t \in T$ $\overline{p}(t)$。令$(S_n)_{n \in \mathbf{N}}$为$T$对$\mu$的压榨，使得$H$的限制对于集合$S_n$中的每一个都是连续的（§1, No. 8，命题10和11）；我们将$T$的$\Lambda : t \mapsto \lambda_t$映射表示为$\mathscr{M}_+(X)$，在$S = \bigcup_{n \in \mathbf{N}} S_n$上等于$H$，在$T - S$上等于0。显然，$\nu = \int_T \lambda_t \, d\mu(t)$和$\Lambda$满足叙述的条件a)。
令 $\theta$ 为 $T$ 的测度； 映射 $\Lambda$ 模糊地是$\theta$-可测量的，并且基本上是$\theta$-可积的，因此$\theta$-是足够的（第V, §3, No. 1，提案2 b））。令$f$为$X$上普遍可测的正值函数；由第 5 章第 5 条提案V, §3, No. 2应用于$\int \lambda_t \, d\theta(t)$，映射$t \mapsto \lambda_t^\bullet(f)$是$\theta$可测的，因此考虑到$\theta$的任意性，是普遍可测的。
公式 (12) 来自第 5 章命题 5 的结果V, §3, No. 2。
B) 假设存在 $X$ 的紧致子集 $X'$，携带测度$\nu$，且$p_{X'}$ 是连续的：
集合$T' = p(X')$和$p' = p_{X'}$；让我们用$\nu'$表示测量$\nu_{X'}$，用$\mu'$像测量$p'(\nu')$对$T'$。由于 $p'$ 是连续且满射的，并且由于 $X'$ 是紧致且可度量的，因此由 A) 存在 $T'$ 的映射 $\Lambda' : t' \mapsto \lambda'_{t'}$ 进入 $\mathscr{M}_+(X')$ 满足以下条件：
a') 对于每个 $t' \in T'$，$\lambda'_{t'}$ 的度量由 $X' \cap \overline{p}'(t')$ 承载；
b') 对于$X'$上的每个普遍可测量的正函数$f'$，函数$t' \mapsto {\lambda'_{t'}}^\bullet(f')$在$T'$上普遍可测量并且
$$
\int_{X'} f'(x') \, d\nu'(x') = \int_{T'} d\mu'(t') \int_{X'} f'(x') \, d\lambda'_{t'}(x').
$$

设 $t \in T$；如果$t$属于到$T'$，让我们用$\lambda'_t$的$\lambda_t$像在$X'$的典范嵌入到$X$表示，如果$t$属于到$T - T'$我们集合$\lambda_t = 0$。读者将毫无困难地验证映射$t \mapsto \lambda_t$满足叙述的条件a）和b）。

C) *一般情况下存在*:

$\nu$对$X$的措施正在缓和，我们可以选择覆盖$\nu$的$X$由……组成的$(U_m)_{m \in \mathbf{N}}$-可积开放集合。令加法$(X_n)_{n \in \mathbf{N}}$为$X$的$\nu$压榨，使得$p$的限制对于每个集合$X_n$是连续的（§ 1, No. 8，道具10和11）；用$\nu_n$表示$X$上的测量$\varphi_{X_n} \cdot \nu$，用$\mu_n$表示$p$下的像。 B) 对于每个整数$n \in \mathbf{N}$，$T$的映射$t \mapsto \alpha^n_t$到$\mathscr{M}_+(X)$满足，存在以下条件：

$a'')$ 措施$\alpha^n_t$ 由$\overline{p}(t)$ 承担所有$t \in T$。

$b'')$ 如果 $f$ 是 $X$ 上的普遍可测正值函数，则 $T$ 上的正值函数 $t \mapsto (\alpha^n_t)^*(f)$ 是普遍可测的，并且

$$
\int_X f(x)\, d\nu_n(x) = \int_T d\mu_n(t) \int_X f(x)\, d\alpha^n_t(x).
$$

一个有$\nu = \sum_{n \in \mathbf{N}} \nu_n$和$\mu = \sum_{n \in \mathbf{N}} \mu_n$；直接从No. 2的命题3和上面的引理4得出，在$T$上存在普遍可测的正函数的序列$(g_n)_{n \in \mathbf{N}}$，使得$\mu_n = g_n \cdot \mu$对于所有$n \in \mathbf{N}$以及$\sum_{n \in \mathbf{N}} g_n = 1$。对于每个$t \in T$，让我们用$\beta^n_t$表示$X$上的措施$g_n(t) \cdot \alpha^n_t$，用$q_t$表示$X$上的负担$\sum_{n \in \mathbf{N}} (\beta^n_t)^*$。令$f$为$X$上普遍可测的正值函数；利用No. 2的命题2并对(13)中的$n$求和，我们得到

$$
\int_X f(x)\, d\nu(x) = \int_T q_t(f)\, d\mu(t);
$$

而且很明显，$T$上的函数$t \mapsto q_t(f)$是普遍可测的。

对于每个$m \in \mathbf{N}$，令$E_m$为$t \in T$的集合，使得$q_t(U_m) = +\infty$； 集合 $E_m$ 是普遍可测的，因为映射 $t \mapsto q_t(U_m)$ 也是如此，并且 $E_m$ 局部 $\mu$ 可以通过应用于 $f = \varphi_{U_m}$ 的公式 (14) 忽略不计，因为 $\nu^*(U_m)$ 是有限的。因此，集合$E = \bigcup_{m \in \mathbf{N}} E_m$是普遍可测量的，而局部$\mu$可以忽略不计。我们集合$\lambda_t = 0$$t \in E$。此外，设 $t \in T - E$；由于开口集合 $U_m$ 覆盖$X$ 并且$q_t(U_m)$ 是有限的，因此负担$q_t$ 是局部有界的；根据§ 1, No. 7的第7条，在$X$上存在一个测度$\lambda_t$，使得$q_t = \lambda_t^*$和$\lambda_t = \sum_{n \in \mathbf{N}} \beta^n_t$。 映射$t \mapsto \lambda_t$满足叙述的条件a）和b）是直接的。

D) *c)*的证明：
令 $f$ 为 $X$ 上普遍可测的函数，且为正且有界；我们将证明，对于 $\mu = p(\nu)$ 的测度 $\mu_f = p(f \cdot \nu)$，$T$ 上的普遍可测函数 $h_f : t \mapsto \lambda_t^\bullet(f)$ 是密度。令$K$为$T$的紧致子集，并令$A = \overline{p}^{-1}(K)$。对于每个 $t \in T$，$\lambda_t$ 的度量由 $\overline{p}^{-1}(t)$ 承载；如果$t$属于到$K$则$\overline{p}^{-1}(t) \subset A$、从而$\lambda_t^\bullet(f \varphi_A) = \lambda_t^\bullet(f)$；另一方面，如果$t$属于到$T - K$则$\overline{p}^{-1}(t) \subset X - A$、从而$\lambda_t^\bullet(f \varphi_A) = 0$。 应用公式 (12) 到 $f \cdot \varphi_A$,$^{(1)}$ 我们得到

$$
\mu_f(K) = \int_A^\bullet f(x)\, d\nu(x) = \int_K^\bullet d\mu(t) \int_X^\bullet f(x)\, d\lambda_t(x) = \int_K^\bullet h_f(t)\, d\mu(t),
$$

从而建立关系 $\mu_f = h_f \cdot \mu$。

令 $f = 1$ 可知，函数 $h_1 : t \mapsto \| \lambda_t \|$ 是 $\mu_1 = \mu$ 相对于 $\mu$ 的度量的密度，因此在$\mu$ 中局部等于 1 - $T$ 中几乎所有地方。

E) *唯一性*:
让$t \mapsto \lambda_t^i$（对于$i = 1, 2$）是$T$的两个映射到$\mathscr{M}_+(X)$满足条件a）和b）叙述。如C），选择对$X$进行$\mu$压榨$(X_n)_{n \in \mathbf{N}}$，使得$p_{X_n}$对于每个$n \in \mathbf{N}$和集合$N = X - \bigcup_{n \in \mathbf{N}} X_n$都是连续的。对于每个整数 $n \in \mathbf{N}$、选择，$X$、零在 $X_n$ 之外，有一个可数的集合 $D_n$ 正函数，其限制到 $X_n$ 形式规范空间$\mathscr{C}(X_n)$中的稠密集合（将GT的Th.1，X, §3, No. 3应用于可度量紧凑空间$X_n$）。我们集合$D = \bigcup_{n \in \mathbf{N}} D_n$。

设 $f \in D$；通过 D)，函数 $t \mapsto (\lambda_t^1)^\bullet(f)$ 和 $t \mapsto (\lambda_t^2)^\bullet(f)$ 是测量$\mu_f$相对于$\mu$的密度，因此$T$中存在局部可忽略的$\mu$集合$E_f$，使得$(\lambda_t^1)^\bullet(f) = (\lambda_t^2)^\bullet(f)$为$t \in T - E_f$。此外，根据(12)，$t \in T$的集合$F_i$使得$(\lambda_t^i)^\bullet(N) \neq 0$局部$\mu$-对于$i = 1, 2$可以忽略不计。由于$D$是可数的，集合$G = (\bigcup_{f \in D} E_f) \cup F_1 \cup F_2$局部$\mu$可以忽略不计；对于$t \in T - G$，根据§1, No. 8第9号提案，我们有$(\lambda_t^1)^\bullet(N) = (\lambda_t^2)^\bullet(N) = 0$和$(\lambda_t^1)_{X_n} = (\lambda_t^2)_{X_n}$、从而$\lambda_t^1 = \lambda_t^2$。

Q.E.D.

#### 注 {#int-ix-s2-n7-rem-1 .statement tag=09PJ}

— 1) 如果$X$是苏斯林空间，则$X$的每个紧致子空间都是苏斯林空间，因此可度量（TG，IX，附录I，第3条的Cor.2），$^{(2)}$

(1) 如果 $f \cdot \varphi_A$ 不可普遍测量，请使用下面的 *注 2*)。
(2) 该结果未出现在 GT 中（cf. §1, No. 9 的 *注 1* 的脚注）。

并且 X 上的每项措施都经过调节（§ 1, No. 9，注 1）。因此，根据第 13 条命题，X 上的每个测度$\nu$ 都承认对每个$\nu$-固有映射的分解。

2) 根据命题13的记号，令$f$为正$\nu$可测函数。一个可以证明，如第 1 章中所示。 V, § 3, No. 2，命题5，$t \in T$的集合使得$f$不可测$\lambda_t$，局部$\mu$可忽略不计，$t \mapsto \lambda_t^\bullet(f)$是$\mu$可测，关系(12)再次成立。

### 习题{#int-ix-s2-exercises}

§ 2](exercises/s2/)参见[习题。
