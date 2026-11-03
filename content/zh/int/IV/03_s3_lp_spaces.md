---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 3
section_title: LP spaces
lang: zh
source: int-i-vi
book_pages: INT IV.18-INT IV.32, INT IV.120
pdf_pages: 0125-0139, 0227-0227
extraction: ocr
subsections:
    - "no": 1
      title: Minkowski’s inequality
      page: 18
      pdf_page: 125
    - "no": 2
      title: The semi-norms $N_p$
      page: 19
      pdf_page: 126
    - "no": 3
      title: The spaces $\mathscr{F}_F^p$
      page: 20
      pdf_page: 127
    - "no": 4
      title: $p$-th power integrable functions
      page: 23
      pdf_page: 130
    - "no": 5
      title: Properties of $p$-th power integrable functions
      page: 25
      pdf_page: 132
    - "no": 6
      title: Directed sets in $L^p$ and increasing sequences in $\mathscr{L}^p$
      page: 27
      pdf_page: 134
    - "no": 7
      title: Lebesgue’s theorem
      page: 30
      pdf_page: 137
    - "no": 8
      title: Relations between the spaces $\mathscr{L}_F^p$ ($1 \leq p < +\infty$)
      page: 31
      pdf_page: 138
statements: 44
exercises: 3
content_sha256: bb71f2e3bd963c6cd48f96b639e739eeaf544a1cabd8ea3cc9fd71913f389476
translated_from: content/en/int/IV/03_s3_lp_spaces.md
translation_method: google
source_content_sha256: 7e23198285dc5cb4353370685c3d59fc0442a1a826f792dd80d1ab78eaae10e8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 30f4f026ba44ccaf76159f8ee8d543cf54a38e8d396f4ccd558b7d4a0c7171f7
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。 L$^p$空间

### 1. 闵可夫斯基的不等式

令 X 为局部紧致空间，$\mu$ 为X 的测度。在 X 上定义的正数值函数（有限或非有限）的集合中，函数 $|\mu|^*(f)$ 为正、正齐次、递增且凸（$§ 1$、No. 3，命题 10、11 和 12）。

#### 命题 1 {#int-iv-s3-prop-1 .statement tag=08QN}

— 对于X上定义的每个实数$p \geqslant 1$和每个对正函数$f, g$（有限或不有限），

$$
(|\mu|^*((f + g)^p))^{1/p} \leqslant (|\mu|^*(f^p))^{1/p} + (|\mu|^*(g^p))^{1/p}
$$

（闵可夫斯基的不等式）。

当第二个成员的项之一等于$+\infty$时，不等式(1)是明显的。相反的情况下，$f$和$g$几乎在任何地方都是有限的（$§ 2$，No. 3，命题7）。如果$f_1$和$g_1$是有限正数函数分别等价于$f$和$g$，则$f_1^p, g_1^p$和$(f_1 + g_1)^p$分别等价于$f^p, g^p$和$(f + g)^p$，并且因为等价正数函数具有相同的上积分（$§ 2$，No. 3，命题 6），在 $f$ 和 $g$ 处处有限的情况下，我们被简化为证明不等式 (1)；但在这种情况下不等式是第1章中证明的一般明可夫斯基不等式的特例。 I，No. 2，提案 3。

我们还将有机会利用以下初等不等式：如果$p \geqslant 1$那么，对于任何数$a \geqslant 0,\ b \geqslant 0$，

$$
a^p + b^p \leqslant (a + b)^p .
$$

如果$a = b = 0$或者数$a, b$之一是$+\infty$，则不等式是明显的；如果$a, b$是有限的且$a + b > 0$，则可以写成

$$
\left( \frac{a}{a + b} \right)^p + \left( \frac{b}{a + b} \right)^p \leqslant 1 ,
$$

由此可见

$$
\left( \frac{a}{a + b} \right)^p \leqslant \frac{a}{a + b} , \quad \left( \frac{b}{a + b} \right)^p \leqslant \frac{b}{a + b} \quad \text{and} \quad \frac{a}{a + b} + \frac{b}{a + b} = 1 .
$$

### 2. 半范数$N_p$

在接下来的所有内容中，$F$表示*完全规范*向量空间（即，Banach空间）超过域$\mathbf{R}$或域$\mathbf{C}$； 元素 $z \in F$ 的 *范数* 将表示为 $|z|$。 给定集合 $A$ 的映射 $f$ 到 $F$，我们将 $A$ 的映射 $x \mapsto |f(x)|$ 写成 $|f|$ 到$\mathbf{R}_+$（必须注意，$|f|$ 是一个*数字） 函数*，而不是 *数*）。

#### 定义 1 {#int-iv-s3-def-1 .statement tag=08QO}

*令$X$为局部紧凑空间，$\mu$为$X$的测度。对于$X$的每个映射$f$转化为Banach空间$F$，对于每个数$p$，这样$1 \leq p < +\infty$，我们用$N_p(f, \mu)$或简称$N_p(f)$表示，正数* $(\int^* |f|^p d|\mu|)^{1/p}$。

请注意，数$N_p(f)$可能等于$+\infty$。

#### 命题 2 {#int-iv-s3-prop-2 .statement tag=08QP}

*如果$f$和$g$是$X$到$F$的两个映射，并且$\alpha$是任意标量$\neq 0$，那么，对于$1 \leq p < +\infty$，

(3) $$
N_p(\alpha f) = |\alpha| N_p(f)
$$
(4) $$
N_p(f + g) \leq N_p(f) + N_p(g).
$$

因为，关系 (3) 立即从 Def 得出。 1 并且 $|\mu|^*$ 是正齐次的；另一方面，由于 $|f + g| \leq |f| + |g|$，不等式 (4) 由 Minkowski 的不等式 (1) 和 $|\mu|^*$ 是递增的事实得出。

我们扩展 Def。 1 到数值函数的情况，*有限与否*，在 $X$ 上定义，再次由设定定义

$$
N_p(f) = \left( \int^* |f|^p d|\mu| \right)^{1/p}
$$

对于这样的函数$f$。人们立即看出，当在 $X$ 和 $\alpha \neq 0$ 上定义 $f + g$ 时，关系 (3) 和 (4) 也适用于这些函数。而且：

#### 定理 1（可数凸性定理）{#int-iv-s3-thm-1 .statement tag=08QQ}

— *令 $(f_n)$ 为 $X$ 上定义的函数 $\geq 0$（有限或非有限）的序列。对于$1 \leq p < +\infty$，

(5) $$
N_p \left( \sum_{n=1}^\infty f_n \right) \leq \sum_{n=1}^\infty N_p(f_n).
$$

集合$f = \sum_{n=1}^\infty f_n$； $f$是函数$g_n = \sum_{k=1}^n f_k$的递增序列的上包络线； $N_p(f)$ 中的定义，以及 Th。 §1, No. 3中的3个，表明$N_p(f) = \sup_n N_p(g_n)$。 但是根据命题 1 $N_p(g_n) \leq \sum_{k=1}^n N_p(f_k)$，从而不等式 (5)。

#### 命题 3 {#int-iv-s3-prop-3 .statement tag=08QR}

*如果 f 和 g 是 X 的两个等价映射到 Banach 空间 F，则 $N_p(f - g) = 0$ 为 $1 \leq p < +\infty$；相反，如果 $N_p(f - g) = 0$ 对于 $p \geq 1$ 的值，则 f 和 g 是等价的。*

命题立即从 Th 开始。 1 个§2, No. 3。

如果 f 和 g 是 X 到 F 中的两个等价映射，则$N_p(f) = N_p(g)$ 对于所有 $p \geq 1$（§ 2, No. 3，命题 6）；因此，$N_p(f)$仅取决于f的类$\tilde{f}$，以及一个集合，由定义、$N_p(\tilde{f}) = N_p(f)$决定。由于X的映射的类代入F形式向量空间(§ 2, No. 4)，关系(3)和(4)也可写成

$$
(6) \quad N_p(\alpha \tilde{f}) = |\alpha| N_p(\tilde{f})
$$
$$
(7) \quad N_p(\tilde{f} + \tilde{g}) \leq N_p(\tilde{f}) + N_p(\tilde{g}).
$$

类似地，对于等效数值函数（有限或非有限）的每一个类，都有一个定义 $N_p(\tilde{f})$。

然后，我们可以将定义$N_p(f)$用于函数，而F中的值（分别在$\overline{\mathbf{R}}$中）几乎在X中的任何地方都定义为设定$N_p(f) = N_p(\tilde{f})$；那么很明显，关系（3）和（4）再次成立（假设$\alpha \neq 0$和$f + g$几乎到处定义，在数值函数的情况下，无论是否有限）。

如果 $0 < p < 1$，则再次集合 $N_p(f) = (\int^* |f|^p d|\mu|)^{1/p}$，但不等式 (4) 和 (5) 不再有效（cf. Ch. I，Exer. 6 和 Ch. IV, §6，Exer. 13）。

### 3. 空间 $\mathscr{F}_F^p$

设 F 是 X 的所有映射到 F 中的 Banach 空间、$\mathscr{F}(X; F)$（或简称 $\mathscr{F}_F$）向量空间。对于 $1 \leq p < +\infty$，我们将用 $\mathscr{F}^p(X, \mu; F)$ 或 $\mathscr{F}_F^p(X, \mu)$ 表示，或简称 $\mathscr{F}_F^p(\mu)$，或$\mathscr{F}_F^p$（如果不会造成混淆），将X的映射 f 的集合代入F，使得$N_p(f) < +\infty$（我们写为$\mathscr{F}^p$而不是$\mathscr{F}_R^p$）。显然$\mathscr{F}_F^p(|\mu|) = \mathscr{F}_F^p(\mu)$。从No. 2的命题2可以立即得出，$\mathscr{F}_F^p$是$\mathscr{F}_F$的*线性子空间*，而$N_p(f)$是空间的*半范数*。我们将始终假设（没有明确提及相反）$\mathscr{F}_F^p$配备有由该半范数定义的拓扑；我们可以说，这个拓扑是阶p*的均值收敛的*拓扑（对于$p = 1$，我们简称它为均值收敛的*拓扑*；对于$p = 2$，也称“二次均值收敛的拓扑”）。我们可以说，$\mathscr{F}_F^p$上的过滤器$\mathscr{G}$（分别是元素或$\mathscr{F}_\mathbf{F}^p$的序列$(f_n)$）收敛到$f$，对于这个拓扑*收敛于阶*的平均值$p$ 至 $f$；因此，这意味着 $N_p(g - f)$ 相对于 $\mathscr{G}$ 趋于 0（即 $N_p(f_n - f)$ 趋于 0，因为 $n$ 趋于无穷大）。

这个术语扩展立即适用于函数$f_n$和函数$f$几乎到处都有定义（或者在$\overline{\mathbf{R}}$中有值，并且几乎到处都有定义和有限）。

请注意，局部凸空间 $\mathscr{F}_\mathbf{F}^p$ 通常*不是 Hausdorff*；这个空间中0的闭包是X的*可忽略*映射到F的线性子空间$\mathscr{N}_\mathbf{F}$（No. 2，命题3）。

#### 注{#int-iv-s3-n3-rem-1 .statement tag=08QS}

— 令 F 为 Banach 空间 *超过域* $\mathbf{C}$ 或复数；然后，对于每个函数$f \in \mathscr{F}_\mathbf{F}^p$和每个复数$\alpha$，$\alpha f$属于到$\mathscr{F}_\mathbf{F}^p$和$N_p(\alpha f) = |\alpha| N_p(f)$；在其他字中，$\mathscr{F}_\mathbf{F}^p$也是向量空间超过$\mathbf{C}$，并且$N_p(f)$是这个复合体向量空间（TVS，II, §1）的半范数。

#### 命题 4 {#int-iv-s3-prop-4 .statement tag=08QT}

*让$\mathscr{B}$成为$\mathscr{F}_\mathbf{F}^p$上的过滤器基。假设存在紧集$K \subset X$，使得对于每个集合$M \in \mathscr{B}$，所有映射$f \in M$的支持都包含在K中。在这些条件下，如果$\mathscr{B}$在X一致收敛到$f_0$，然后 $f_0$ 属于到 $\mathscr{F}_\mathbf{F}^p$ 和 $\mathscr{B}$ 收敛于阶 $p$ 到 $f_0$。*

同样的道理，在映射$f \in \mathscr{F}_\mathbf{F}^p$的集合上，其支撑包含在固定的紧集中，拓扑的一致收敛性比阶的均值收敛性拓扑*更细**更细* $p$。

例如，令$h$是X到$[0,1]$的连续映射，有紧支撑，等于K上的1（第III, §1, No. 2，引理1）。对于每个$\varepsilon > 0$，都存在一个$M \in \mathscr{B}$，这样，对于每个映射$f \in M$，对于所有$x \in X$，都存在$|f(x) - f_0(x)| \leq \varepsilon h(x)$。由此可知$N_p(f - f_0) \leq \varepsilon N_p(h)$，从而命题。

#### 命题 5 {#int-iv-s3-prop-5 .statement tag=08QU}

*局部凸空间$\mathscr{F}_\mathbf{F}^p$已完成。*

由于与 $\mathscr{F}_\mathbf{F}^p$ 伴随的 Hausdorff 空间是一个规范的空间，因此足以证明 $\mathscr{F}_\mathbf{F}^p$ 中的每个 *Cauchy 序列* $(f_n)$ 对于拓扑的收敛均值阶具有极限 $p$（GT，IX, §2, No. 6，提案 9）。到假设，对于每个$\varepsilon > 0$，都存在整数$m_0$，使得关系$m \geq m_0,\ n \geq m_0$暗示$N_p(f_n - f_m) \leq \varepsilon$。因此，可以在$k$、严格递增的序列$(n_k)$定义、归纳、整数$\geq 0$这样$N_p(f_{n_{k+1}} - f_{n_k}) \leq 2^{-k}$。如果我们证明级数与一般项 $g_k = f_{n_{k+1}} - f_{n_k}$ ($k \geq 1$) *收敛于阶* $p$，那么它将有和 $g \in \mathscr{F}_\mathbf{F}^p$，并且 $f = g + f_{n_1}$ 将是极限序列$(f_{n_k})$在$\mathscr{F}_\mathbf{F}^p$；那么$f$将是序列$(f_n)$的集群点；因为这个序列是柯西序列，所以它将有$f$作为极限，并且第5条命题将被证明（GT，II, §3, No. 2，第5条命题的Cor.2）。

因此，第 5 条命题是以下命题中的推论：

#### 命题 6 {#int-iv-s3-prop-6 .statement tag=08QV}

*令$(f_n)$为$\mathscr{F}_\mathbf{F}^p$中函数的序列，使得$\sum_{n=1}^\infty N_p(f_n) < +\infty$。在这些条件下，级数与一般的项$f_n(x) \in \mathbf{F}$在$X$中几乎处处绝对收敛。 设定 $f(x) = \sum_{n=1}^\infty f_n(x)$ 在点处，其中级数收敛，而 $f(x) = 0$ 在其他地方，函数 $f$ 属于到 $\mathscr{F}_\mathbf{F}^p$ 并且是和级数与一般项$f_n$（对于拓扑收敛于阶$p$的平均值）；更准确地说，对于每个 $n \geqslant 0$，

$$
N_p \left( f - \sum_{k=1}^n f_k \right) \leqslant \sum_{k=n+1}^\infty N_p(f_k).
$$

考虑正函数（有限或无限）$g(x) = \sum_{n=1}^\infty |f_n(x)|$。由可数凸性定理 (No. 2, Th. 1)，

$$
N_p(g) \leqslant \sum_{n=1}^\infty N_p(f_n) < +\infty;
$$

因此$g$几乎处处是有限的（§ 2, No. 3，命题7），这意味着级数与一般的项$f_n(x)$几乎处处绝对收敛。由于$\mathbf{F}$是完备的，因此级数几乎处处收敛，并且对于每个$x \in X$、$|f(x)| \leqslant \sum_{n=1}^\infty |f_n(x)| = g(x)$、从而

$$
N_p(f) \leqslant N_p(g) \leqslant \sum_{n=1}^\infty N_p(f_n) < +\infty,
$$

这就证明了$f$属于到$\mathscr{F}_\mathbf{F}^p$。另一方面，对于每个整数 $n$，

$$
|f(x) - \sum_{k=1}^n f_k(x)| \leqslant \sum_{k=n+1}^\infty |f_k(x)|
$$

几乎无处不在，从而$N_p \left( f - \sum_{k=1}^n f_k \right) \leqslant \sum_{k=n+1}^\infty N_p(f_k)$。由假设，级数与一般项$N_p(f_n)$收敛；因此，对于每个$\varepsilon > 0$，都存在整数$n$使得$\sum_{k=n+1}^{\infty} N_p(f_k) \leq \varepsilon$，并且不等式(8)证明$f$是级数的和，对于项$f_n$，对于拓扑收敛的平均值为阶 $p$。

命题5和6由此被完全证明。

### 4. $p$-第幂可积函数

向量空间 $\mathscr{H}(X; F)$（如果不怕混淆，我们简单地用$\mathscr{H}_F$来表示），$X$连续的函数到$F$的紧凑支撑下的由……组成，显然是向量空间每个的子空间 $\mathscr{F}_F^p$。

#### 定义 2 {#int-iv-s3-def-2 .statement tag=08QW}

*给定一个局部紧凑的空间* $X$，*测量* $\mu$ *在* $X$，*和 Banach 空间* $F$，*我们表示为* $\mathscr{L}_F^p(X, \mu)$ *（或简单地* $\mathscr{L}_F^p(\mu)$，*或* $\mathscr{L}_F^p$) *闭包，在局部凸空间* $\mathscr{F}_F^p(X, \mu)$，*的向量空间* $\mathscr{H}(X; F)$ *的连续映射的* $X$ *进入* $F$ *具有紧支撑。* *我们用* $L_F^p(X, \mu)$表示*（或* $L_F^p(\mu)$，*或* $L_F^p$）*（标准化）* Hausdorff *空间与* $\mathscr{L}_F^p(X, \mu)$ 相关。 *函数属于到*$\mathscr{L}_F^p$*称为*$p$*-第幂可积函数* (*)。

显然是$\mathscr{L}_F^p(X, |\mu|) = \mathscr{L}_F^p(X, \mu)$和$L_F^p(X, |\mu|) = L_F^p(X, \mu)$。

我们应该写 $\mathscr{L}^p$ 和 $L^p$ 而不是 $\mathscr{L}_R^p$ 和 $L_R^p$（或者写 $\mathscr{L}_C^p$ 和 $L_C^p$，以免造成混淆）。如果$F$是一个*复数*Banach空间，$\mathscr{L}_F^p$和$L_F^p$配备了结构拓扑向量空间超过域$\mathbf{C}$（No. 3，*注*）。

显然，$\mathscr{F}_F^p$中的每个函数都相当于$\mathscr{L}_F^p$中的函数，属于到$\mathscr{L}_F^p$。 函数与 $F$ 中的值以及 $X$ 中的*几乎处处定义*，再次被称为*$p$*-*第幂可积*，如果它等价于 $\mathscr{L}_F^p$ 中的函数；类似地，函数与$\overline{\mathbf{R}}$中的值，在$X$中几乎处处定义且有限，如果等价于$\mathscr{L}^p$中的函数，则据说是*$p$*-*第幂可积*。

因此，$\mathscr{L}_F^p$中的函数（分别在$\mathscr{L}^p$中）是在所有*$X$上*定义的*$p$*-*第幂可积函数*（分别在所有$X$上定义和有限）。在这个截面和下一个中，$\mathscr{L}_F^p$（或$\mathscr{L}^p$）中证明函数的大部分命题可以立即扩展到*$p$*-*第幂可积函数*，这些幂可积函数*不是处处定义的（或者不是处处定义和有限的）；我们通常会将制定这些结果和证明的任务留给读者。

(*) 术语的理由将在§4, No. 2 中给出。

#### 注 1 {#int-iv-s3-n4-rem-1 .statement tag=08QX}

正如已经发出的信号（§2, No. 5），$p$第幂可积函数和$\mathbf{F}$中的值一般不会形式向量空间。

#### 注 2 {#int-iv-s3-n4-rem-2 .statement tag=08QY}

一般来说，空间$\mathscr{F}_\mathbf{F}^p$与其子空间$\mathscr{L}_\mathbf{F}^p$不同（§4，Exer.8）。

定义。 2 立即得出以下标准：

#### 命题 7 {#int-iv-s3-prop-7 .statement tag=08QZ}

对于函数$\mathbf{f}$到属于到$\mathscr{L}_\mathbf{F}^p$，对于每个$\varepsilon > 0$，存在一个连续的函数$g$，并且具有紧支持使得$N_p(\mathbf{f} - g) \leq \varepsilon$是充分必要的。

在其他$\mathscr{L}_\mathbf{F}^p$中的字、函数是连续函数的序列的极限，具有紧支撑，对于阶$p$的均值收敛的拓扑。

#### 命题 8 {#int-iv-s3-prop-8 .statement tag=08R0}

令 $f$ 为几乎处处定义的数值函数（有限或无限）；如果对于每个 $\varepsilon > 0$，存在两个$p$-第幂可积函数 $g, h$，使得 $g \leq f \leq h$ 几乎处处且 $N_p(h - g) \leq \varepsilon$，则 $f$ 是 $p$-第幂可积。

因为，$f$几乎处处都是有限的，而$N_p(f - g) \leq N_p(h - g) \leq \varepsilon$；因此，命题 7 表明 $f$ 是$p$-第幂可积。

因为，到定义，$\mathscr{L}_\mathbf{F}^p$是$\mathscr{F}_\mathbf{F}^p$的闭子空间，并且由于后者空间是完整的（No. 3，命题5），我们有以下结果（GT，II, §3, No. 4，命题8）：

#### 定理 2 {#int-iv-s3-thm-2 .statement tag=08R1}

空间$\mathscr{L}_\mathbf{F}^p$已完成； 空间$L_\mathbf{F}^p$是巴拿赫空间。

在空间$L_\mathbf{F}^p$中，类的范数$N_p(\tilde{\mathbf{f}})$再次表示为$\| \tilde{\mathbf{f}} \|_p$。

Th。 2 可以如下锐化：

#### 定理 3 {#int-iv-s3-thm-3 .statement tag=08R2}

设$(\mathbf{f}_n)$为空间$\mathscr{L}_\mathbf{F}^p$中的柯西序列； $(\mathbf{f}_n)$ 存在一个子序列 $(\mathbf{f}_{n_k})$，具有以下属性：
1° 级数与一般项 $N_p(\mathbf{f}_{n_{k+1}} - \mathbf{f}_{n_k})$ 收敛；
2° 级数与一般项 $\mathbf{f}_{n_{k+1}}(x) - \mathbf{f}_{n_k}(x)$ 几乎处处绝对收敛；
3° 如果 $\mathbf{f}$ 是在 $X$ 上定义的函数并且几乎处处都等于序列 $(\mathbf{f}_{n_k}(x))$ 的极限，则 $\mathbf{f}$ 属于到 $\mathscr{L}_\mathbf{F}^p$ 和序列 $(\mathbf{f}_n)$以阶$p$的平均值收敛到$\mathbf{f}$；
4° 存在下半连续函数$g \geq 0$，使得$N_p(g) < +\infty$，并且对于每个$k$，对于所有$x \in X$，$|\mathbf{f}_{n_k}(x)| \leq g(x)$。

正如No. 3第5条命题证明，定义序列$(n_k)$乘以归纳就足够了，这样$N_p(\mathbf{f}_{n_{k+1}} - \mathbf{f}_{n_k}) \leq 2^{-k}$； 部分 2° 和 3° 然后根据No. 3 的第 6 条命题以及$\mathscr{L}_\mathbf{F}^p$ 在$\mathscr{F}_\mathbf{F}^p$ 中闭合的事实得出。另一方面，如果$h(x)$是级数的和和一般的项$|\mathbf{f}_{n_{k+1}}(x) - \mathbf{f}_{n_k}(x)|$，则Th。 No. 2中的1表示$N_p(h) < +\infty$；因此，通过$|\mu|^*$的定义，存在下半连续函数$g \geq h + |\mathbf{f}_{n_1}|$，使得$N_p(g) < +\infty$完整，从而完成证明。

#### 推论 1 {#int-iv-s3-thm-3-cor-1 .statement tag=08R3}

— *如果柯西序列* $(f_n)$ *在空间* $\mathscr{L}_F^p$ *使得序列* $(f_n(x))$ *几乎处处收敛到* $f(x)$*，则* $f$ *是第 p 个幂可积和序列* $(f_n)$ *收敛于阶* $p$ *到* $f$。

因为，存在$(f_n)$的子序列$(f_{n_k})$，使得$(f_{n_k}(x))$几乎处处收敛到$g(x)$，其中$g$是$\mathscr{L}_F^p$中的函数，使得$(f_n)$收敛于阶的均值$p$ 至 $g$。因此，假设意味着 $f(x) = g(x)$ 几乎无处不在，从而推论。

#### 推论 2 {#int-iv-s3-thm-3-cor-2 .statement tag=08R4}

— *让*$\mathscr{E}$*成为*$\mathscr{L}_F^p$的密集子集。 *对于每个函数* $f \in \mathscr{L}_F^p$，*在* $\mathscr{E}$ *中存在序列* $(g_n)$ *中的函数 *具有以下属性*：

1° *序列* $(g_n)$ *收敛于阶* $p$ *到* $f$；
2° *几乎每个* $x \in X$、*序列* $(g_n(x))$ *收敛到* $f(x)$。

因为，由于空间$\mathscr{L}_F^p$是可度量的，$\mathscr{L}_F^p$由……组成中存在函数在$\mathscr{E}$中的柯西序列$(f_n)$并且收敛于阶$p$至 $f$（GT、IX, §2, No. 6、提案 8）；应用Th就足够了。 3 到此序列。

科。 2特别适用于将$\mathscr{E}$视为*具有紧凑支撑的连续函数*的空间$\mathscr{K}_F$的情况。

#### 注 3 {#int-iv-s3-n4-rem-3 .statement tag=08R5}

$\mathscr{L}_F^p$ 中的柯西序列 $(f_n)$ 可以使得序列 $(f_n(x))$ *在* $X$ 的任何点处不收敛（示例 1）。

#### 注 4 {#int-iv-s3-n4-rem-4 .statement tag=08R6}

如果 $f$ 属于到 $\mathscr{L}_F^p$，并不总是能够找到具有紧凑支持的连续函数的序列 $(f_n)$，使得序列 $(f_n(x))$ 在$X$*处处*收敛到函数几乎在任何地方都等于$f(x)$（§4，Exer.4 c））。

### 5. 第 $p$-第幂可积函数的性质

#### 定理 4 {#int-iv-s3-thm-4 .statement tag=08R7}

— *让* $F$ *和* $G$ *成为两个Banach 空间，* $u$ *连续的线性映射 of * $F$ *进入* $G$。 *For every 函数* $f \in \mathscr{L}_F^p$, *composite 函数* $u \circ f$ *属于 to* $\mathscr{L}_G^p$.

令 $f \in \mathscr{L}_F^p$；对于每个$\varepsilon > 0$，都存在函数$g \in \mathscr{K}_F$使得$N_p(f - g) \leq \varepsilon$；从$|u \circ f - u \circ g| \leq \|u\| \cdot |f - g|$开始，我们

$$
N_p(u \circ f - u \circ g) \leq \|u\| \cdot N_p(f - g) \leq \varepsilon \|u\|,
$$

由于$u \circ g$是连续的且有紧支撑，因此定理得证。

#### 推论 1 {#int-iv-s3-thm-4-cor-1 .statement tag=08R8}

— *Let* $a'$ *be a continuous 线性形式 on* $F$; *if* $f \in \mathscr{L}_F^p$, *numerical 函数* $x \mapsto \langle f(x), a' \rangle$ **(denoted by $\langle f, a' \rangle$)* 属于 to* $\mathscr{L}^p$.

#### 推论 2 {#int-iv-s3-thm-4-cor-2 .statement tag=08R9}

— 给定 F ($1 \leq k \leq n$) 的 n 点 $a_k$，以及 n 个数值函数 $f_k$ ($1 \leq k \leq n$) 属于至 $\mathscr{L}^p$，函数 $f = \sum_{k=1}^n a_k f_k$ 属于至$\mathscr{L}_F^p$。

这是因为 $\mathbf{R}$ 到 F 中的映射 $t \mapsto a t$ 是连续的。

#### 命题 9 {#int-iv-s3-prop-9 .statement tag=08RA}

— 令 F 为 $\mathbf{R}$ 上的 n 维向量空间，并令 $(e_k)_{1 \leq k \leq n}$ 为 F 的基。对于函数 $f = \sum_{k=1}^n e_k f_k$ 至属于至 $\mathscr{L}_F^p$，每个数值函数是充分必要的$f_k$属于至$\mathscr{L}^p$。

这是 Cors 的结论。 Th的1和2。 4.

#### 命题 10 {#int-iv-s3-prop-10 .statement tag=08RB}

— 在空间$\mathscr{L}_F^p$中，由（有限）线性组合$\sum_k a_k f_k$形成的线性子空间，其中$a_k \in F$和$f_k$是具有紧支撑的连续数值函数，是稠密的（对于拓扑的收敛意味着阶$p$）。

集合 $\mathscr{K}_F$ of continuous 映射 of X into F with compact support is by 定义 dense in $\mathscr{L}_F^p$.另一方面，每个函数$g \in \mathscr{K}_F$可以通过形式$\sum_k a_k f_k$的函数统一近似，其中$f_k$是连续的函数，且支撑包含在$g$支撑的固定紧邻域中（第1章）。 III, §1, No. 2、引理2)； it follows (No. 3, Prop. 4) that $g$ is in the closure in $\mathscr{L}_F^p$ of 集合 of $\sum_k a_k f_k$, 从而命题.

#### 命题 11 {#int-iv-s3-prop-11 .statement tag=08RC}

— 如果函数 $f$ 属于至 $\mathscr{L}_F^p$，则函数 $|f|$ 属于至 $\mathscr{L}^p$，以及映射 $f \mapsto |f|$ 至 $\mathscr{L}_F^p$ $\mathscr{L}^p$ 是一致连续的（对于拓扑来说，收敛于阶 $p$ 的平均值）。

对于每个$\varepsilon > 0$，都存在一个连续的函数$g$，具有紧支撑，使得$N_p(f - g) \leq \varepsilon$；从$||f| - |g|| \leq |f - g|$开始，我们有$N_p(|f| - |g|) \leq \varepsilon$，这证明了$|f| \in \mathscr{L}^p$。另一方面，如果$f_1, f_2$是$\mathscr{L}_F^p$中的两个函数，则$N_p(|f_1| - |f_2|) \leq N_p(f_1 - f_2)$，这表明$f \mapsto |f|$是均匀连续的映射。

#### 命题 12 {#int-iv-s3-prop-12 .statement tag=08RD}

— 对于数值函数$f$至属于至$\mathscr{L}^p$，函数$f^+$和$f^-$属于至$\mathscr{L}^p$中的每一个都是必要且充分的。

从 $f = f^+ - f^-$ 开始，条件就足够了；这是必要的，因为如果$f \in \mathscr{L}^p$则$|f| \in \mathscr{L}^p$（命题11）。

#### 推论 {#int-iv-s3-n5-cor-1 .statement tag=08RE}

— $\mathscr{L}^p$ 属于到 $\mathscr{L}^p$ 中函数有限族的上（或下）包络线。

### 6. $L^p$中的有向集合和$\mathscr{L}^p$中的递增序列

我们在$X$中几乎处处定义了数值函数的等价类的集合$\widetilde{\mathscr{F}}$中的(§ 2, No. 6)序关系$\tilde{f} \leq \tilde{g}$；配备此序关系及其向量空间结构，$\widetilde{\mathscr{F}}$是*Riesz空间*。 No. 5第12条命题推论表明，如果$\tilde{f}$和$\tilde{g}$是子空间的元素和$\widetilde{\mathscr{F}}$的$L^p$，则$\tilde{f}$的上等$\sup(\tilde{f}, \tilde{g})$和$\widetilde{\mathscr{F}}$中的$\tilde{g}$（即函数$\sup(f, g)$中每个类，其中$f \in \tilde{f}$和$g \in \tilde{g}$）属于至$L^p$；这特别证明了$L^p$，配备了由$\widetilde{\mathscr{F}}$诱导的序关系，是*Riesz空间*。

#### 命题 13 {#int-iv-s3-prop-13 .statement tag=08RF}

*在Riesz空间$L^p$中，配备范数$\| \tilde{f} \|_p$定义的拓扑，映射$\tilde{f} \mapsto | \tilde{f} |$均匀连续，元素$\tilde{f} \geq 0$的集合为已关闭。*

命题的第一个部分立即来自No. 5的第11条命题；因为$\tilde{f} \geq 0$的集合也是$\tilde{f}$的集合使得$| \tilde{f} | = f$，所以它是闭集，因为$\tilde{f} \mapsto | \tilde{f} |$是连续的映射而$L^p$是Hausdorff。

因此，我们看到范数$\| \tilde{f} \|_p$定义的$L^p$上的拓扑与$L^p$（TVS，II, § 2, No. 7）的有序向量空间结构“相容的”。

#### 命题 14 {#int-iv-s3-prop-14 .statement tag=08RG}

*令$H$为Riesz空间$L^p$的子集，类$\geq 0$的由……组成，并指向关系$\leq$。对于 $H$ 在 $L^p$ 有一个上界，有必要且充分*

$$
\sup_{\tilde{f} \in H} \| \tilde{f} \|_p < +\infty.
$$

*$L^p$中$H$的上界则为$H$*的截面滤波器的极限*（在Banach空间$L^p$中）*。

条件显然是必要的，因为$\tilde{f} \mapsto \| \tilde{f} \|_p$是递增函数在元素$\geq 0$的集合上，$L^p$。为了证明它是充分的，我们首先观察到它意味着映射$\tilde{f} \mapsto \| \tilde{f} \|_p$下的$H$的像在$\mathbf{R}$中有极限，通过单调极限定理；因此，在此映射下的截面滤波器的$\mathfrak{F}$，$H$的像因此是$\mathbf{R}$上的柯西滤波器的基。如果我们证明$\mathfrak{F}$本身是$L^p$上的柯西滤波器*基，证明将是完整的；因为，$\mathfrak{F}$ 将在 $L^p$ 收敛，因为 $L^p$ 已完成（No. 4，Th.2），命题将从 TVS，II, § 2, No. 7，第 18 条命题而来。

要查看柯西滤波器的$\mathfrak{F}$是基，我们将使用以下引理：

#### 引理 {#int-iv-s3-n6-lem-1 .statement tag=08RH}

如果$f$和$g$是$\mathscr{L}^p$中的两个函数，使得$0 \leq f \leq g$，那么

$$
(N_p(g - f))^p \leq (N_p(g))^p - (N_p(f))^p .
$$

当$f$和$g$在紧支撑下连续时，关系(9)可以写成

$$
\int (g - f)^p d|\mu| \leq \int g^p d|\mu| - \int f^p d|\mu|
$$

则 是初等不等式 $(g - f)^p \leq g^p - f^p$ (No. 1, 公式 (2)) 的推论。为了从这种情况过渡到一般情况，只需观察（9）的两个成员在$\mathscr{L}^p \times \mathscr{L}^p$上连续函数，并且$\mathscr{L}^p$中的每个函数$f \geq 0$都是极限（对于阶$p$的平均值收敛）连续函数 $\geq 0$ 的序列具有紧支撑，通过$\mathscr{L}^p$ 上映射 $g \mapsto |g|$ 的连续性（命题 11）。

引理成立后，对于每一个$\varepsilon > 0$，都存在假设一个$\tilde{f} \in \mathrm{H}$，这样，对于每一个$\tilde{g} \geq \tilde{f}$属于到$\mathrm{H}$，我们有$(\|\tilde{g}\|_p)^p - (\|\tilde{f}\|_p)^p \leq \varepsilon$；由此可知 $(\|\tilde{g} - \tilde{f}\|_p)^p \leq \varepsilon$；因此，如果$\tilde{g}_1$和$\tilde{g}_2$是$\mathrm{H}$中的两个元素，即$\geq \tilde{f}$，则$\|\tilde{g}_1 - \tilde{g}_2\|_p \leq 2\varepsilon^{1/p}$，这证明$\mathfrak{F}$是$L^p$上的柯西滤波器基并完成提案 14 的证明。

#### 推论 1 {#int-iv-s3-prop-14-cor-1 .statement tag=08RI}

如果$\tilde{g}$是$\mathrm{H}$在$L^p$中的上乘，那么

$$
\|\tilde{g}\|_p = \lim_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p = \sup_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p .
$$

这是由$L^p$中范数$\|\tilde{f}\|_p$的连续性以及极限定理的单调性得出的。

#### 推论 2 {#int-iv-s3-prop-14-cor-2 .statement tag=08RJ}

Riesz 空间 $L^p$ 是完全晶格有序的。

$L^p$中的每个有向集合$\mathrm{H}$（对于关系$\leq$）、类$\geq 0$的由……组成以及在$L^p$中的上界，都有一个上界：对于，如果$\tilde{h}$是上界对于$L^p$中的$\mathrm{H}$，则$\|\tilde{f}\|_p \leq \|\tilde{h}\|_p$对于所有$\tilde{f} \in \mathrm{H}$，并且第14条命题适用。这证明了推论（第II, §1, No. 3章，命题1）。

当第 14 条命题的结论在$\mathscr{L}^p$ 中针对函数而不是类时，它们就不再成立。准确地说，如果$M$是$\mathscr{L}^p$中的子集，函数$\geq 0$中的由……组成，指向关系$\leq$，并且使得上封套的$\sup_{f \in M} N_p(f) < +\infty$，*类* $M$ 的$g$ *不一定与函数* 的类* $L^p$ *中的上界相同 f \in M ；特别是，g 不一定是第 p 个幂可积，即使 $g \in \mathscr{L}^p$、$N_p(g)$ 也可以与 $\sup_{f \in M} N_p(f)$ 不同（Th. 3 之后的cf. §1, No. 3、注 1）。

尽管如此，我们还是有以下定理：

#### 定理 5 {#int-iv-s3-thm-5 .statement tag=08RK}

*令$(f_n)$为$\mathscr{L}^p$中的函数$\geqslant 0$中的递增序列。为了使序列的上包络$f$是第p次幂可积，$\sup_n N_p(f_n) < +\infty$是必要且充分的。 序列 $(f_n)$ 然后以阶 $p$ 的平均值收敛到 $f$，并且*

$$
N_p(f) = \sup_n N_p(f_n) = \lim_{n \to \infty} N_p(f_n).
$$

条件显然是必要的，我们只需证明它是充分的。现在，如果满足条件，则第14条命题表明序列$(\tilde{f}_n)$是$L^p$中的柯西序列，因此序列$(f_n)$是$\mathscr{L}^p$中的柯西序列；因为对于所有 $x \in X$，$f_n(x)$ 趋向于 $f(x)$，$f$ 是第 p 个幂可积，并且对于拓扑的收敛均值为序列 $(f_n)$ 的极限阶 $p$（No. 4，第 3 条第 1 条）。因此，$N_p(f_n)$趋向于$N_p(f)$，因为$N_p$是$\mathscr{L}^p$上的连续函数。

#### 推论 1 {#int-iv-s3-thm-5-cor-1 .statement tag=08RL}

*设$\mathscr{L}^p$中$(f_n)$为函数$\geqslant 0$中的递减序列；那么，序列属于到$\mathscr{L}^p$的下包络$f$、序列$(f_n)$收敛于阶$p$到$f$的平均值，并且*

$$
N_p(f) = \lim_{n \to \infty} N_p(f_n) = \inf_n N_p(f_n).
$$

前两个断言源自 Th。 5 应用于序列 $g_n = f_1 - f_n$，即递增且受其限制；剩下的就很明显了。

#### 推论 2 {#int-iv-s3-thm-5-cor-2 .statement tag=08RM}

*令$(f_n)$为$\mathscr{L}^p$中函数的序列。为了使序列 $(f_n)$ 的上包络$f$ 成为第 p 个幂可积，存在函数 $g \geqslant 0$ 使得对于所有 $n$ 存在 $\int^* g^p d|\mu| < +\infty$ 和 $f_n \leqslant g$ 是充分必要的。

服用$g = f^+$后，条件显然是必要的。反之，假设验证通过，集合$g_n = \sup_{k \leqslant n} f_k$； 序列 $(g_n)$ 是递增，由第 p 个幂可积函数组成（No. 5，第 12 号提案的 Cor.）。正函数$h_n = g_n + g_1^-$的递增序列满足Th的条件。 5、从$N_p(h_n) \leqslant N_p(g + g_1^-) < +\infty$开始；因此，它的上包络$\sup_n h_n$是第p次幂可积的，$f = \sup_n h_n - g_1^-$也是如此。

#### 推论 3 {#int-iv-s3-thm-5-cor-3 .statement tag=08RN}

— 令 $A$ 为可数集合，$\mathfrak{F}$ $A$ 上的过滤器，具有可数基，$(f_\alpha)_{\alpha \in A}$ $\mathscr{L}^p$ 中的函数 $\geq 0$ 族。假设存在函数 $g \geq 0$，使得所有$\alpha \in A$都有$N_p(g) < +\infty$和$f_\alpha \leq g$；那么函数 $\limsup_{\mathfrak{F}} f_\alpha$ 是 $p$-th 幂可积且

$$
\limsup_{\mathfrak{F}} N_p(f_\alpha) \leq N_p(\limsup_{\mathfrak{F}} f_\alpha).
$$

设$(A_n)$为$\mathfrak{F}$和集合$g_n = \sup_{\alpha \in A_n} f_\alpha$中的递减基；由于 $A_n$ 是可数集合，因此可以从 Cor 得出。 2 $g_n$ 是第 $p$ 个幂可积；另一方面，$N_p(g_n) \geq \sup_{\alpha \in A_n} N_p(f_\alpha)$。这样一来，$\limsup_{\mathfrak{F}} f_\alpha$就是递减序列$(g_n)$的下包络线；因此 $\limsup_{\mathfrak{F}} f_\alpha$ 是 $p$-th 幂可通过 Cor 积分。 1、和

$$
N_p(\limsup_{\mathfrak{F}} f_\alpha) = N_p \left( \inf_n g_n \right) = \lim_{n \to \infty} N_p(g_n)
$$
$$
\geq \lim_{n \to \infty} \left( \sup_{\alpha \in A_n} N_p(f_\alpha) \right) = \limsup_{\mathfrak{F}} N_p(f_\alpha).
$$

### 7. 勒贝格的定理

#### 定理 6（勒贝格）{#int-iv-s3-thm-6 .statement tag=08RO}

— 令$F$为$\mathscr{L}_F^p$中函数的Banach空间、$(f_n)$序列，这样：$1^\circ$序列$(f_n(x))$几乎处处收敛到极限$f(x) \in F$； $2^\circ$ 存在一个数字函数 $g \geq 0$，使得对于每个整数 $n$，$\int^* g^p d|\mu| < +\infty$ 和 $|f_n(x)| \leq g(x)$ 几乎在 $X$ 中无处不在。那么，函数$f$（几乎到处都有定义）是$p$-第幂可积，并且序列$(f_n)$以阶$p$的平均值收敛到$f$。

考虑数值函数$g_{mn} = |f_m - f_n|$的‘双’序列，其中属于到$\mathscr{L}^p$（No. 5，命题11）； 假设、$\lim_{m \to \infty, n \to \infty} g_{mn}(x) = 0$几乎无处不在，而另一方面$|g_{mn}(x)| \leq 2g(x)$几乎无处不在； 应用科。 3 Th。 No. 6中的5个到这个双序列，

$$
\limsup_{m \to \infty, n \to \infty} N_p(f_m - f_n) \leq N_p(0) = 0,
$$

并且由于 $N_p(f_m - f_n) \geq 0$ 这意味着 $\lim_{m \to \infty, n \to \infty} N_p(f_m - f_n) = 0$；在其他字中，序列$(f_n)$是$\mathscr{L}_F^p$中的柯西序列。因此定理由 Cor 得出。 1 Th。 No. 4 中的 3 个。

#### 推论 {#int-iv-s3-n7-cor-1 .statement tag=08RP}

— 令 $A$ 为指标的集合，由具有可数基的过滤器 $\mathfrak{F}$ 过滤。如果$(f_\alpha)_{\alpha \in A}$是$\mathscr{L}_F^p$中的函数族，相对于滤波器$\mathfrak{F}$，几乎处处逐点收敛到函数$f$，此外，如果存在一个数值函数$g \geq 0$，使得$\int^* g^p d|\mu| < +\infty$和$|f_\alpha(x)| \leq g(x)$对于每个 $\alpha \in A$，几乎在 $X$ 中的所有位置，则函数 $f$ 是 $p$-第幂可积，并且 $f_\alpha$ 相对于滤波器倾向于阶 $p$ 到 $f$ 的平均值$\mathfrak{F}$。

例如，令$(A_n)$为$\mathfrak{F}$的递减可数底数，并令$\alpha_n$为$A_n$的任意元素；序列 $(f_{\alpha_n})$ 几乎在 $X$ 中的所有位置逐点收敛到 $f$，因此 Th。图6显示$f$是$p$次方可积，并且$\lim_{n \to \infty} N_p(f - f_{\alpha_n}) = 0$。 由于$\mathfrak{F}$是与所有此类序列$(\alpha_n)$（GT，I, §6, No. 8，命题11）相关联的基本滤波器的交滤波器，$\lim_{\mathfrak{F}} N_p(f - f_\alpha)$存在并且等于所有序列$(N_p(f - f_{\alpha_n}))$中的公共的极限0。

#### 注 1 {#int-iv-s3-n7-rem-1 .statement tag=08RQ}

Th。如果假设$|f_n| \leq g$（与$N_p(g) < +\infty$）被较弱的假设$\sup_n N_p(f_n) < +\infty$取代，则6不再成立。例如，假设$\mu$是$\mathbf{R}$上的勒贝格测度； 定义连续函数$f_n$，按以下方式：$f_n(x) = 0$对于$x \leq 0$和$x \geq \frac{2}{n}$，$f_n(\frac{1}{n}) = n$，$f_n$在区间$[0, \frac{1}{n}]$和$[\frac{1}{n}, \frac{2}{n}]$上呈线性。然后对所有$x \in \mathbf{R}$使用$\lim_{n \to \infty} f_n(x) = 0$，但对每个$n$使用$N_1(f_n) = 1$（cf.§5，Exer.12）。

#### 注 2 {#int-iv-s3-n7-rem-2 .statement tag=08RR}

科。的 Th。如果不假设过滤器 $\mathfrak{F}$ 具有可数基（cf. §1, No. 3、注 1 遵循 Th. 3 的 Cor.），则 6 不再成立。

### 8. 关系空间 $\mathscr{L}_F^p$ ($1 \leq p < +\infty$) 之间

对于每个实数$\alpha > 0$，映射$z \mapsto |z|^{\alpha-1} \cdot z$都被定义并且在$F$中0的补码上连续；此外，由于$||z|^{\alpha-1} \cdot z| = |z|^{\alpha}$，这个函数随着$z$趋于0，因此可以通过在这个点处给它值0，通过连续性扩展到点0，即使$\alpha < 1$。

#### 定理 7 {#int-iv-s3-thm-7 .statement tag=08RS}

— 令$p$和$q$为两个实数，使得$1 \leq p < +\infty$、$1 \leq q < +\infty$。如果函数 $f$ 属于至 $\mathscr{L}_F^p$，则函数 $|f|^{(p/q)-1} \cdot f$ 属于至 $\mathscr{L}_F^q$，反之亦然。

到假设时，存在连续函数的序列 $(f_n)$，并且具有紧凑的支持，使得 $\sum_{n=1}^\infty N_p(f_n) < +\infty$ 和 $f(x) = \sum_{n=1}^\infty f_n(x)$ 几乎无处不在（No. 4，Th.3）。 集合

$$
g_n = |f_1 + f_2 + \cdots + f_n|^{(p/q)-1} \cdot (f_1 + f_2 + \cdots + f_n);
$$

函数$g_n$连续，支撑紧凑；另一方面，

$$
|g_n|^q = |f_1 + f_2 + \cdots + f_n|^p \leq \left( \sum_{n=1}^\infty |f_n| \right)^p = h^q,
$$

其中数值函数 $h \geqslant 0$（有限或非有限）满足不等式

$$
(N_q(h))^q = \left( N_p \left( \sum_{n=1}^{\infty} |f_n| \right) \right)^p \leqslant \left( \sum_{n=1}^{\infty} N_p(f_n) \right)^p < +\infty
$$

由可数凸性定理。此外，$g_n(x)$几乎到处都趋向于$g(x) = |f(x)|^{(p/q)-1} \cdot f(x)$，因此勒贝格的定理表明$g \in \mathscr{L}_F^q$。自 $f = |g|^{(q/p)-1} \cdot g$ 起，逆命题为直接的。

可以证明映射$f \mapsto |f|^{\frac{p}{q}-1} \cdot f$是$\mathscr{L}_F^p$到$\mathscr{L}_F^q$的同胚（§ 6，Exer.10）。

#### 推论 1 {#int-iv-s3-thm-7-cor-1 .statement tag=08RT}

— *对于函数$f$至属于至$\mathscr{L}_F^p$，函数$|f|^{p-1} \cdot f$属于至$\mathscr{L}_F^1$是必要且充分的。*

#### 推论 2 {#int-iv-s3-thm-7-cor-2 .statement tag=08RU}

— *对于正数函数 $f$ 至属于至 $\mathscr{L}^p$，$f^p$ 属于至 $\mathscr{L}^1$ 是充分必要的。*

请注意，如果$f$是任意符号的数字函数，则$|f|^p$属于到$\mathscr{L}^1$，$f$不一定是属于到$\mathscr{L}^p$（cf.§ 4，Exer.8）。

### 习题{#int-iv-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
