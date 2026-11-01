---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 4
section_title: Products of measures
lang: zh
source: int-i-vi
book_pages: INT III.60-INT III.62
pdf_pages: 0085-0100, 0105-0107
extraction: ocr
subsections:
    - "no": 1
      title: The product of two measures
      page: 40
      pdf_page: 85
    - "no": 2
      title: Properties of product measures
      page: 44
      pdf_page: 89
    - "no": 3
      title: Continuity of product measures
      page: 47
      pdf_page: 92
    - "no": 4
      title: Product of a finite number of measures
      page: 48
      pdf_page: 93
    - "no": 5
      title: Inverse limits of measures
      page: 50
      pdf_page: 95
    - "no": 6
      title: Infinite products of measures
      page: 53
      pdf_page: 98
statements: 22
exercises: 8
content_sha256: 0cfc74a26f9a45a056c9bc654e4ba445c70ddfb3f7a6fb67c3a8c73900530d01
translated_from: content/en/int/III/04_s4_products_of_measures.md
translation_method: google
source_content_sha256: 375b3e9104624766e0c67616cc70666473c13c687b42ef6fceaaffeead1b1903
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 69dc1ff869455b7e6e06942cb898619aa24611963e24029bfdb5318e0e1b14d3
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 乘积措施

### 1. 乘积两个小节

#### 定理 1 {#int-iii-s4-thm-1 .statement tag=08O8}

— *令X和Y为两个局部紧致空间，$\lambda$对X的测度，$\mu$对Y的测度；在$X \times Y$上存在且仅有一个测度$\nu$，使得对于每一个函数* $g \in \mathscr{K}(X; \mathbf{C})$ *和每一个函数* $h \in \mathscr{K}(Y; \mathbf{C})$，

$$
\int g(x)h(y)\, d\nu(x, y) = \left( \int g(x)\, d\lambda(x) \right) \left( \int h(y)\, d\mu(y) \right).
$$

#### 引理 {#int-iii-s4-n1-lem-1 .statement tag=08O9}

1— *令 X 和 Y 为两个局部紧致空间，K（分别为 L）和 X（分别为 Y）的紧致子集。*

(i) *限制到* $\mathscr{K}(X \times Y, K \times L; \mathbf{C})$ *规范的双射*

$$
\omega : \mathscr{F}(X \times Y; \mathbf{C}) \to \mathscr{F}(X; \mathscr{F}(Y; \mathbf{C}))
$$

(S, R, §4, No. 14) *是 Banach 空间* $\mathscr{K}(X \times Y, K \times L; \mathbf{C})$ *到 Banach 空间* $\mathscr{K}(X, K; \mathscr{K}(Y, L; \mathbf{C}))$ 的等距。

(ii) *向量空间* $\mathscr{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathscr{K}(Y, L; \mathbf{C})$，*与* $\mathscr{K}(X \times Y, K \times L; \mathbf{C})$ *（A，II, §7, No. 7，第 15 号提案之后的注释）的子空间进行规范识别，在这个 Banach 空间* 中是密集的。

$\mathscr{K}(X \times Y, K \times L; \mathbf{C})$的$\omega$下的像包含在$\mathscr{K}(X, K; \mathscr{K}(Y, L; \mathbf{C}))$中，是直接的。相反，如果$u$是$X$到$\mathscr{K}(Y, L; \mathbf{C})$的连续映射，支持度包含在$K$中，则$X \times Y$到$\mathbf{C}$的映射$(x, y) \mapsto u(x)(y)$是连续的，并且支持度包含在$K \times L$中，因此$\omega$到$\mathscr{K}(X \times Y, K \times L; \mathbf{C})$的限制是这个空间的双射到$\mathscr{K}(X, K; \mathscr{K}(Y, L; \mathbf{C}))$；事实上，这个限制是 Banach 空间等距，是从关系得出的

$$
\sup_{(x, y) \in K \times L} |f(x, y)| = \sup_{x \in K} \left( \sup_{y \in L} |f(x, y)| \right).
$$

这就证明了(i)；另一方面，$\omega$下的像，

$$
\mathscr{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathscr{K}(Y, L; \mathbf{C})
$$

用$\mathscr{K}(X \times Y, K \times L; \mathbf{C})$的子空间识别，又是空间$\mathscr{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathscr{K}(Y, L; \mathbf{C})$，但这次用$X$的映射的空间规范地识别为$\mathscr{K}(Y, L; \mathbf{C})$（A，II, §7, No. 7，Prop.15的Cor.）；但是$\mathscr{K}(X, K; \mathscr{K}(Y, L; \mathbf{C}))$的这个子空间在后者空间中被认为是“稠密”的（§ 1, No. 2，命题5），因此（ii）的结论是根据$\omega$的限制是拓扑同构这一事实得出的。

证明了引理后，我们现在观察到$X \times Y$的每个紧致子集都包含在乘积$K \times L$中，其中$K$（或$L$）是$X$（或$Y$）的紧致子集。因此，根据引理 1，(ii) 子空间 $\mathscr{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathscr{K}(Y; \mathbf{C})$ 在 $\mathscr{K}(X \times Y; \mathbf{C})$ 中是“稠密”的；由于对于$g \in \mathscr{K}(X; \mathbf{C})$、$h \in \mathscr{K}(Y; \mathbf{C})$，关系 (1) 也可以写成$\nu(g \otimes h) = \lambda(g)\mu(h)$，因此$\nu$的*唯一性*紧随其后。为了证明$\nu$的存在，我们将利用以下引理：

#### 引理 2 {#int-iii-s4-lem-2 .statement tag=08OA}

*对于记号，如引理 1，对于每个函数* $f \in \mathscr{K}(X \times Y, K \times L; \mathbf{C})$ *函数*

$$
y \mapsto h(y) = \int f(x, y) \, d\lambda(x)
$$

*属于到*$\mathscr{K}(Y, L; \mathbf{C})$。

对于每个函数 $u \in \mathscr{K}(X; \mathscr{K}(Y, L; \mathbf{C}))$，$\int u(x) d\lambda(x)$ 属于到 $\mathscr{K}(Y, L; \mathbf{C})$ 的积分，因为后者是 Banach 空间（§ 3, No. 3，第 7 条命题的 Cor. 1）；但对于 $u = \omega(f)$ 和每个 $y \in Y$，

$$
\left\langle \int u(x) d\lambda(x), \varepsilon_y \right\rangle = \int u(x)(y) d\lambda(x) = \int f(x, y) d\lambda(x),
$$

从而引理。

那么，考虑一下，对于每个函数$f \in \mathscr{K}(X \times Y; \mathbf{C})$，数$\nu(f) = \mu(\int f(x, y) d\lambda(x))$（我们也将通过滥用记号写成$\int d\mu(y) \int f(x, y) d\lambda(x)$）；如果 K（分别为 L）是 X（分别为 Y）的紧凑子集，则存在数 $a_K$（分别为 $b_L$），这样，对于每个函数 $g \in \mathscr{K}(X, K; \mathbf{C})$（分别为 $h \in \mathscr{K}(Y, L; \mathbf{C})$），我们有$|\lambda(g)| \leq a_K \|g\|$（分别为$|\mu(h)| \leq b_L \|h\|$）。由此可见，对于每个函数 $f \in \mathscr{K}(X \times Y, K \times L; \mathbf{C})$，

$$
\left| \int f(x, y) d\lambda(x) \right| \leq a_K \|f\|
$$

每 $y \in Y$、从而 $|\nu(f)| \leq a_K b_L \|f\|$。因此，$\mathscr{K}(X \times Y; \mathbf{C})$上的线性形式$\nu$是$X \times Y$上的测度，它显然满足(1)，从而完成了Th的证明。 1.

#### 定义 1 {#int-iii-s4-def-1 .statement tag=08OB}

*给定分别在两个局部紧凑空间$X, Y$上定义的两个测度$\lambda, \mu$，$\mu$右$\lambda$的测度乘积定义为$X \times Y$满足关系上的唯一测度$\nu$ (1) 对于每个函数 $g \in \mathscr{K}(X; \mathbf{C})$ 和每个函数 $h \in \mathscr{K}(Y; \mathbf{C})$。*

周四证明。 1、空间X和Y的角色可以互换；规范地识别$Y \times X$和$X \times Y$，因此我们对$X \times Y$进行定义测量

$$
f \mapsto \int d\lambda(x) \int f(x, y) d\mu(y)
$$

再次满足条件 (1)。由此我们证明了以下定理：

#### 定理 2 {#int-iii-s4-thm-2 .statement tag=08OC}

*令 $\lambda, \mu$ 为分别在两个局部紧凑空间 $X, Y$ 上定义的两个度量。对于$\mathscr{K}(X \times Y; \mathbf{C})$中的每个函数$f$，$f$相对于乘积测量$\lambda$的$\nu$除以$\mu$的积分有值*

$$
\int f(x, y) d\nu(x, y) = \int d\lambda(x) \int f(x, y) d\mu(y)
$$
$$(3)$$
$$
= \int d\mu(y) \int f(x, y) d\lambda(x).
$$

由于最后一个公式，$f$相对于乘积测量$\nu$的积分通常表示为$\iint f\, d\lambda\, d\mu$，或$\iint f\, d\mu\, d\lambda$，或$\iint f\, \lambda\mu$，或$\iint f\, \mu\lambda$，或$\iint f(x, y)\, d\lambda(x)\, d\mu(y)$，或$\iint f(x, y)\, d\mu(y)\, d\lambda(x)$、或$\iint f(x, y)\, \lambda(x)\mu(y)$、或$\iint f(x, y)\, \mu(y)\lambda(x)$；据说它是$f$关于$\lambda$和$\mu$的双积分。有了这个记号，公式 (3) 就可以写成

$$
\iint f(x, y)\, d\lambda(x)\, d\mu(y) = \int d\lambda(x) \int f(x, y)\, d\mu(y)
$$
$$
= \int d\mu(y) \int f(x, y)\, d\lambda(x).
$$

公式 (3) 表明，如果 $\lambda$ 和 $\mu$ 是实数（分别为正）测度，则乘积测度 $\nu$ 为实数（分别为正）。

#### 例 1 {#int-iii-s4-n1-exa-1 .statement tag=08OD}

狄拉克测度$\varepsilon_x$ ($x \in X$) 和$\varepsilon_y$ ($y \in Y$) 的乘积测度是狄拉克测度$\varepsilon_{(x, y)}$。

#### 例 2 {#int-iii-s4-n1-exa-2 .statement tag=08OE}

让我们采用$X = Y = \mathbf{R}$，对于$\lambda$和$\mu$，使用$\mathbf{R}$ (§1, No. 3) 上的*勒贝格测度*；他们的乘积被称为$\mathbf{R}^2$上的*勒贝格测度*； 函数 $f \in \mathscr{K}(\mathbf{R}^2; \mathbf{C})$ 对于该测量的积分表示为 $\iint f(x, y)\, dx\, dy$ 或 $\iint f(x, y)\, dy\, dx$； 公式 (4)，对于函数，即零在紧凑矩形 $[a, b] \times [c, d]$ 之外，产生公式

$$
\int_c^d dy \int_a^b f(x, y)\, dx = \int_a^b dx \int_c^d f(x, y)\, dy
$$

在 FRV 中证明，II, §3, No. 6。

由于$\mathbf{R}$上的勒贝格测度在每个翻译下（§1, No. 3）都是不变的，因此立即得出$\mathbf{R}^2$上的勒贝格测度在$\mathbf{R}^2$的每个翻译下都是不变的*。

#### 注 {#int-iii-s4-n1-rem-1 .statement tag=08OF}

令$E$为Hausdorff局部凸空间，并令$f$为$\mathscr{K}(X \times Y; E)$中的映射，使得$f(X \times Y)$包含在$E$的*完全凸*子集$C$中。然后，对于每个$y \in Y$，$h(y) = \int f(x, y)\, d\lambda(x)$属于到$E$的积分（§3, No. 3，命题7）；此外，函数$h$属于到$\widetilde{\mathscr{K}}(Y; E)$：确实，对于每个$z' \in E'$，我们有

$$
\langle h(y), z' \rangle = \int \langle f(x, y), z' \rangle\, d\lambda(x),
$$

因此 $y \mapsto \langle h(y), z' \rangle$ 属于到 $\mathscr{K}(Y; C)$ 引理 2。因此定义了积分 $\int h\, d\mu$（并且*先验* 属于到 ${E'}^*$）；让我们证明

$$
\iint f(x, y)\, d\lambda(x)\, d\mu(y) = \int d\mu(y) \int f(x, y)\, d\lambda(x)
$$
$$
= \int d\lambda(x) \int f(x, y)\, d\mu(y),
$$

从而推广公式 (4)。事实上，对于每 $z' \in E'$，我们有
$$
\left\langle \int \int f d\lambda d\mu, z' \right\rangle = \int \int \langle f, z' \rangle d\lambda d\mu = \int d\mu \int \langle f, z' \rangle d\lambda \\
= \int \left\langle \int f d\lambda, z' \right\rangle d\mu = \left\langle \int d\mu \int f d\lambda, z' \right\rangle
$$
由 (4), 从而 (5)。

### 2. 乘积测度的性质

如果 $\lambda$（或 $\mu$）是 X（或 Y）上的度量，且 $\nu$ 是 $\lambda$ 通过 $\mu$ 的乘积度量，则 $\nu$ 到 $\mathscr{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathscr{K}(Y; \mathbf{C})$ 的限制为无除了两个线性形式$\lambda$和$\mu$（A，II, §3, No. 2）中的*张量积*$\lambda \otimes \mu$之外，因为No. 1的关系（1）可以写成
$$
\langle g \otimes h, \nu \rangle = \langle g, \lambda \rangle \langle h, \mu \rangle = \langle g \otimes h, \lambda \otimes \mu \rangle
$$
对于所有 $g \in \mathscr{K}(X; \mathbf{C})$ 和 $h \in \mathscr{K}(Y; \mathbf{C})$。通过滥用记号，我们还可以用$\lambda \otimes \mu$乘积度量$\nu$来表示（而不仅仅是限制到$\mathscr{K}(X \times Y; \mathbf{C})$的密集子空间$\mathscr{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathscr{K}(Y; \mathbf{C})$）。

由于No. 1的公式(3)，$\mathscr{M}(X; \mathbf{C}) \times \mathscr{M}(Y; \mathbf{C})$的映射$(\lambda, \mu) \mapsto \lambda \otimes \mu$进入$\mathscr{M}(X \times Y; \mathbf{C})$显然是*双线性*。

#### 命题 1 {#int-iii-s4-prop-1 .statement tag=08OG}

*设$\lambda$为X的测度，$\mu$为Y的测度；如果 $g \in \mathscr{C}(X; \mathbf{C}),\ h \in \mathscr{C}(Y; \mathbf{C}),$ 那么*
$$
(g \cdot \lambda) \otimes (h \cdot \mu) = (g \otimes h) \cdot (\lambda \otimes \mu).
$$

对于每一个函数 $f \in \mathscr{K}(X \times Y; \mathbf{C})$，我们凭借 No. 1 的公式 (3)，
$$
\langle f, (g \otimes h) \cdot (\lambda \otimes \mu) \rangle = \int d\lambda(x) \int f(x, y) g(x) h(y) d\mu(y) \\
= \int g(x) d\lambda(x) \int f(x, y) h(y) d\mu(y),
$$
这就证明了公式 (6)。

#### 命题 2 {#int-iii-s4-prop-2 .statement tag=08OH}

*乘积$\lambda \otimes \mu$的支持度等于$\lambda$的支持度和$\mu$的支持度的乘积。*

我们首先观察到关系$\lambda \otimes \mu = 0$意味着其中一个措施$\lambda, \mu$是零（A，II, §7, No. 7，提案16，（ii））。另一方面，如果 U（分别V）是X（分别Y）中的开集合，则$\lambda \otimes \mu$到乘积$U \times V$的限制是限制的乘积 $\lambda$ 到 U 以及 $\mu$ 到 V，如下从 Th 开始。 1 的 No. 1 和定义的限制措施到开放的集合 (§ 2, No. 1)。因此，为了使$\lambda \otimes \mu$到$U \times V$的限制成为零，$\lambda$到U的限制或$\mu$到V的限制为零是充分必要的，证明命题，考虑到定义对措施的支持（§ 2, No. 2）。

#### 命题 3 {#int-iii-s4-prop-3 .statement tag=08OI}

*让$\lambda \in \mathscr{M}(X; \mathbf{C}),\ \mu \in \mathscr{M}(Y; \mathbf{C})$。然后*

$$
|\lambda \otimes \mu| = |\lambda| \otimes |\mu|.
$$

令 $f \in \mathscr{K}_+(X \times Y),\ g \in \mathscr{K}(X \times Y; \mathbf{C})$ 使得 $|g| \leq f$；我们有 (§ 1, No. 6, 公式 (13))

$$
\begin{align*}
|\langle g, \lambda \otimes \mu \rangle| &= \left| \int d\lambda(x) \int g(x, y) d\mu(y) \right| \\
&\leq \int d|\lambda|(x) \int |g(x, y)|\ d|\mu|(y) \\
&= \langle |g|, |\lambda| \otimes |\mu| \rangle \leq \langle f, |\lambda| \otimes |\mu| \rangle.
\end{align*}
$$

由此可见$\langle f, |\lambda \otimes \mu| \rangle \leq \langle f, |\lambda| \otimes |\mu| \rangle$，依此类推

$$
|\lambda \otimes \mu| \leq |\lambda| \otimes |\mu|.
$$

另一方面，让$u \in \mathscr{K}_+(X),\ v \in \mathscr{K}_+(Y)$。对于每个$\varepsilon > 0$，都存在$u_1 \in \mathscr{K}(X; \mathbf{C}),\ v_1 \in \mathscr{K}(Y; \mathbf{C})$使得$|u_1| \leq u,\ |v_1| \leq v$和

$$
|\langle u_1, \lambda \rangle| \geq \langle u, |\lambda| \rangle - \varepsilon,\quad |\langle v_1, \mu \rangle| \geq \langle v, |\mu| \rangle - \varepsilon
$$
（§ 1, No. 6）。由此可见 $|u_1 \otimes v_1| \leq u \otimes v$ 和

$$
\begin{align*}
\langle u \otimes v, |\lambda \otimes \mu| \rangle &\geq |\langle u_1 \otimes v_1, \lambda \otimes \mu \rangle| = |\langle u_1, \lambda \rangle \langle v_1, \mu \rangle| \\
&\geq ((\langle u, |\lambda| \rangle - \varepsilon)(\langle v, |\mu| \rangle - \varepsilon)).
\end{align*}
$$

由于 $\varepsilon$ 是任意的，我们推断

$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle \geq \langle u, |\lambda| \rangle \langle v, |\mu| \rangle = \langle u \otimes v, |\lambda| \otimes |\mu| \rangle.
$$

考虑(8)，我们看到

$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle = \langle u \otimes v, |\lambda| \otimes |\mu| \rangle.
$$

由于$\mathscr{K}(X; \mathbf{C})$（或$\mathscr{K}(Y; \mathbf{C})$）中的每个函数都是$\mathscr{K}_+(X)$（或$\mathscr{K}_+(Y)$）中函数的线性组合，因此前面的公式对于$u \in \mathscr{K}(X; \mathbf{C})$和$v \in \mathscr{K}(Y; \mathbf{C})$仍然成立；因此，命题是从$\mathscr{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathscr{K}(Y; \mathbf{C})$在$\mathscr{K}(X \times Y; \mathbf{C})$中稠密这一事实得出的。

#### 推论{#int-iii-s4-n2-cor-1 .statement tag=08OJ}

— *让* $\lambda \in \mathscr{M}(X; \mathbf{R}), \ \mu \in \mathscr{M}(Y; \mathbf{R})$。 *然后*

$$
\begin{cases}
(\lambda \otimes \mu)^+ = \lambda^+ \otimes \mu^+ + \lambda^- \otimes \mu^- , \\
(\lambda \otimes \mu)^- = \lambda^+ \otimes \mu^- + \lambda^- \otimes \mu^+ .
\end{cases}
$$

因为，根据第 3 条命题，

$$
\begin{align*}
(\lambda \otimes \mu)^+ &= \frac{1}{2} (\lambda \otimes \mu + |\lambda| \otimes |\mu|) \\
&= \frac{1}{2} ((\lambda^+ - \lambda^-) \otimes (\mu^+ - \mu^-) + (\lambda^+ + \lambda^-) \otimes (\mu^+ + \mu^-)) \\
&= \lambda^+ \otimes \mu^+ + \lambda^- \otimes \mu^- .
\end{align*}
$$

$(\lambda \otimes \mu)^-$ 的论证类似。

#### 命题 4 {#int-iii-s4-prop-4 .statement tag=08OK}

— *让* $\lambda \in \mathscr{M}(X; \mathbf{C}), \ \mu \in \mathscr{M}(Y; \mathbf{C})$。 *然后*

$$
\|\lambda \otimes \mu\| = \|\lambda\| \cdot \|\mu\|,
$$

*约定当因子之一为0且另一个为$+\infty$*时，第二个成员将被0替换。 *特别是，如果* $\lambda$ *和* $\mu$ *有界，则* $\lambda \otimes \mu$ *有界*。

由上述命题 3 和 §1, No. 8，Cor.根据第 10 条命题 1，我们可以将极限应用于$\lambda$ 和$\mu$ 是积极措施的情况。如果$\lambda = 0$或$\mu = 0$，结果是微不足道的；因此，让我们假设$\lambda \neq 0$和$\mu \neq 0$。我们首先证明$\|\lambda \otimes \mu\| \leq \|\lambda\| \cdot \|\mu\|$。我们可以假设$\lambda$和$\mu$是有界的。对于每$f \in \mathscr{K}_+(X \times Y)$，

$$
\langle f, \lambda \otimes \mu \rangle = \int d\lambda(x) \int f(x, y) d\mu(y)
$$

和

$$
\int f(x, y) d\mu(y) \leq \|f\| \cdot \|\mu\|
$$

对于每 $x \in X$，因此

$$
\langle f, \lambda \otimes \mu \rangle \leq \|f\| \cdot \|\lambda\| \cdot \|\mu\|,
$$

这证明了我们的断言。另一方面，让

$$
\alpha < \| \lambda \| , \quad \beta < \| \mu \|
$$

是两个实数$\geqslant 0$。存在 $g \in \mathscr{K}_+(X) , \ h \in \mathscr{K}_+(Y)$ 使得

$$
\| g \| \leqslant 1 , \ \| h \| \leqslant 1 , \quad \lambda(g) \geqslant \alpha , \ \mu(h) \geqslant \beta .
$$

然后$g \otimes h \in \mathscr{K}_+(X \times Y) , \ \| g \otimes h \| \leqslant 1$和$\langle g \otimes h , \lambda \otimes \mu \rangle \geqslant \alpha \beta ;$，因此$\| \lambda \otimes \mu \| \geqslant \alpha \beta$，最后$\| \lambda \otimes \mu \| \geqslant \| \lambda \| \cdot \| \mu \|$，从而完成证明。

### 3. 乘积措施的连续性

#### 命题 5 {#int-iii-s4-prop-5 .statement tag=08OL}

*对于每一个度量*$\lambda_0 \in \mathscr{M}(X; \mathbf{C})$，*映射*$\mu \mapsto \lambda_0 \otimes \mu$*的*$\mathscr{M}(Y; \mathbf{C})$*到*$\mathscr{M}(X \times Y; \mathbf{C})$*是模糊连续的*。

对于每个函数$f \in \mathscr{K}(X \times Y; \mathbf{C})$，我们知道函数$h(y) = \int f(x, y) d\lambda_0(x)$属于到$\mathscr{K}(Y; \mathbf{C})$（No. 1，引理2），以及$\langle f , \lambda_0 \otimes \mu \rangle = \langle h , \mu \rangle$，从而命题。

#### 命题 6 {#int-iii-s4-prop-6 .statement tag=08OM}

*当* $\mathscr{M}(X; \mathbf{C}) , \ \mathscr{M}(Y; \mathbf{C})$ *和* $\mathscr{M}(X \times Y; \mathbf{C})$ *配备严格紧致收敛的拓扑* (§ 1, No. 10)时，*双线性映射* $(\lambda, \mu) \mapsto \lambda \otimes \mu$ *of* $\mathscr{M}(X; \mathbf{C}) \times \mathscr{M}(Y; \mathbf{C})$ *进入* $\mathscr{M}(X \times Y; \mathbf{C})$ *对于集合是低连续的* $\mathscr{M}(X; \mathbf{C})$ *和* $\mathscr{M}(Y; \mathbf{C})$ *(TVS, III, § 5, No. 3)* 的子集有模糊界限。

令$K \subset X , \ L \subset Y$为两个紧集，$A$为$\mathscr{K}(X \times Y, K \times L; \mathbf{C})$的紧凑子集，$B$为$\mathscr{M}(X; \mathbf{C})$的模糊边界且封闭的子集；众所周知，$B$是模糊紧致的（§ 1, No. 9，命题15），因此对于严格紧致收敛的拓扑也是紧致的（§ 1, No. 10，命题17）。另一方面，Banach 空间 $\mathscr{K}(X \times Y, K \times L; \mathbf{C})$ 与 $\mathscr{K}(X, K; \mathscr{K}(Y, L; \mathbf{C}))$ 等距（No. 1，引理 1）；将$\mathscr{K}(X, K; \mathscr{K}(Y, L; \mathbf{C})) \times \mathscr{M}(X; \mathbf{C})$的映射$\varphi$转化为$\mathscr{K}(Y, L; \mathbf{C})$，使得$\varphi(g, \lambda)$是由$h(y) = \int g(x, y) d\lambda(x)$定义的函数$h$，凭借§ 3, No. 4，道具是“单独连续的”。 8 和 9. 由于 $\mathscr{K}(X, K; \mathscr{K}(Y, L; \mathbf{C}))$ 是桶状的，因此映射 $\varphi$ 相对于 $\mathscr{M}(X; \mathbf{C})$ 的模糊边界子集是“次连续的”（TVS，III, § 5, No. 3，第 6 条）；因而，映射到$A \times B$的限制是*连续的*（*loc.cit.*，Prop.4）。 映射之下的$A \times B$的像$C$因此是Banach空间$\mathscr{K}(Y, L; \mathbf{C})$的紧凑子集。现在，$C$正是函数$h(y) = \int f(x, y) d\lambda(x)$的集合，因为$f$超过$A$，$\lambda$超过$B$；根据No. 1的公式(3)，条件$\lambda \in B$和$\mu \in C^\circ$因此意味着$\lambda \otimes \mu \in A^\circ$。鉴于严格紧致收敛的定义或拓扑，这证明了命题（TVS，III, § 5, No. 3，Def.2）。

当严格紧致收敛的拓扑被模糊的拓扑取代时，命题6的结论就不再有效（Exer.2c））。但是，如果 B（分别为 C）是 $\mathscr{M}(X; \mathbf{C})$（分别为 $\mathscr{M}(Y; \mathbf{C})$）的模糊边界子集，则映射 $(\lambda, \mu) \mapsto \lambda \otimes \mu$ 下的 $B \times C$ 的像模糊地边界为 $\mathscr{M}(X \times Y; \mathbf{C})$，因此根据命题 6、§1, No. 10、命题 17 和 TVS 命题 4、III, §5, No. 3 (cf. Exer. 3)，映射到 $B \times C$ 的限制是模糊连续的。

### 4. 有限数措施中的乘积

令$X_i$ ($1 \leq i \leq n$) 为$n$ 局部紧凑空间，$X = \prod_{i=1}^n X_i$ 它们的乘积。 形式复合体函数线性组合集合
$$
(x_1, x_2, \ldots, x_n) \mapsto f_1(x_1)f_2(x_2)\cdots f_n(x_n),
$$
其中 $f_i \in \mathscr{K}(X_i; \mathbf{C})$ ($1 \leq i \leq n$)，可以用张量积 $\bigotimes_{i=1}^n \mathscr{K}(X_i; \mathbf{C})$ 来规范地识别，并且从 No. 1 的引理 1，通过 $n$ 上的归纳得出，这个张量积是*密集*的$\mathscr{K}(X; \mathbf{C})$。

现在让 $\mu_i$ 成为$X_i$ ($1 \leq i \leq n$) 的测度；在 $X$ 上存在且仅有一个测度 $\nu$，使得对于 $f_i \in \mathscr{K}(X_i; \mathbf{C})$ ($1 \leq i \leq n$)，
$$
\langle f_1 \otimes f_2 \otimes \cdots \otimes f_n, \nu \rangle = \prod_{i=1}^n \langle f_i, \mu_i \rangle.
$$
因为，如果这种措施存在，那么它是独一无二的。另一方面，令 $\nu = \mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n$ 为由递归关系定义的 $X$ 的度量
$$
\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n = (\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_{n-1}) \otimes \mu_n.
$$
从No. 1、公式 (1) 和这个定义（由$n$ 上的归纳）得出$\nu$ 验证 (11)；据说它是措施$\mu_i$（$1 \leq i \leq n$）的*乘积措施*，并且再次用$\bigotimes_{i=1}^n \mu_i$表示。 关系 (11) 也可以写成
$$
\langle f_1 \otimes f_2 \otimes \cdots \otimes f_n, \mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n \rangle = \prod_{i=1}^n \langle f_i, \mu_i \rangle.
$$

#### 命题 7（'措施乘积结合性'）{#int-iii-s4-prop-7 .statement tag=08ON}

—
*设*$(I_k)_{1 \leq k \leq r}$*为区间*$[1, n]$*的划分*$\mathbf{N}$； *然后*
$$
\bigotimes_{k=1}^r \left( \bigotimes_{i \in I_k} \mu_i \right) = \bigotimes_{i=1}^n \mu_i
$$

对于$\bigotimes_{i=1}^n \mathscr{K}(X_i; \mathbf{C})$中的每个函数，这两个测量重合，通过(12)。

函数 $f \in \mathscr{K}(X; \mathbf{C})$相对于乘积测量的积分表示为
$$
\int f d\mu_1 d\mu_2 \ldots d\mu_n,
$$
或
$$
\iiint \ldots \int f d\mu_1 d\mu_2 \ldots d\mu_n
$$
或
$$
\int f(\mu_1 \otimes \cdots \otimes \mu_n)
$$
或者也
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) d\mu_1(x_1) d\mu_2(x_2) \ldots d\mu_n(x_n)
$$
或
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) \mu_1(x_1) \mu_2(x_2) \ldots \mu_n(x_n)
$$
带有 $n$ 标志 $\int$；据说它是阶* $n$ 的 *倍数积分，或 *$n$ 元组积分*。凭借乘积的措施结合性和阶积分反转的定理（No. 1，Th.2），对于 $[1, n]$ 的每一个置换 $\sigma$，我们有，
$$
\iiint \ldots \int f d\mu_1 d\mu_2 \ldots d\mu_n = \int d\mu_{\sigma(1)} \int d\mu_{\sigma(2)} \ldots \int fd\mu_{\sigma(n)}.
$$
(14)

积分记号和公式 (14) 可以通过 Hausdorff 局部凸空间 $E$ 中的值以明显的方式扩展到函数 $f \in \mathscr{K}(X; E)$，使得 $f(X)$ 包含在 $E$ 的完全凸子集中。我们留给读者的任务是，将第 2 条和第 3 条关于两个措施的乘积的结果推广到任何有限数措施的乘积。

特别是，我们称$n$的$\mathbf{R}^n$乘积上的*勒贝格测度*与$\mathbf{R}$上的勒贝格测度相同； 函数 $f \in \mathscr{K}(\mathbf{R}^n; E)$、满足前面的条件的积分表示为
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) dx_1 dx_2 \ldots dx_n
$$
并且等于
$$
\int_{-\infty}^{+\infty} dx_1 \int_{-\infty}^{+\infty} dx_2 \ldots \int_{-\infty}^{+\infty} f(x_1, x_2, \ldots, x_n) dx_n.
$$
$\mathbf{R}^n$ 的勒贝格测度*在每个翻译下都是不变的*。

### 5. 逆极限措施

令$X, Y$为两个紧凑的空间，$p : X \to Y$为连续的映射；那么$f \mapsto f \circ p$是$\mathscr{C}(Y; \mathbf{C})$到$\mathscr{C}(X; \mathbf{C})$的连续线性映射，因为$\|f \circ p\| \leq \|f\|$对于每个函数$f \in \mathscr{C}(Y; \mathbf{C})$；我们用$p'$表示这个映射。因此，它的转置 ${}^t p' : \mathscr{M}(X; \mathbf{C}) \to \mathscr{M}(Y; \mathbf{C})$ 使得，对于 $X$ 上的每个测度 $\mu$，${}^t p'(\mu)$ 是 $Y$ 上的测度，使得

$$
\langle {}^t p'(\mu), f \rangle = \langle \mu, f \circ p \rangle
$$

对于每个函数 $f \in \mathscr{C}(Y; \mathbf{C})$。 注对于每个$x \in X$，${}^t p'(\varepsilon_x) = \varepsilon_{p(x)}$；因此，我们将用$p_*(\mu)$表示度量${}^t p'(\mu)$，因此当$X$（或$Y$）规范地嵌入$\mathscr{M}(X; \mathbf{C})$（或$\mathscr{M}(Y; \mathbf{C})$）时，扩展$p$（§ 1, No. 9，第13条）；对于$X$上的每个测度$\mu$，$p_*(\mu)$是测度*像一般概念的特例，我们将在第1章中研究它。 V, §6。因为，正如我们上面看到的，$\|p'\| \leq 1$，我们还有$\|{}^t p'\| \leq 1$，所以

$$
\|p_*(\mu)\| \leq \|\mu\|
$$

对于每一个度量$\mu \in \mathscr{M}(X; \mathbf{C})$。

现在让我们考虑一个有向预排序的集合 $I$，以及 *逆系*（或“投影系统”）$(X_\alpha, p_{\alpha\beta})$ 的 *compact* 空间 $X_\alpha$（GT，I, §4, No. 4），其中 $I$ 为集合共指标； *逆极限* 空间 $X = \lim_{\leftarrow} X_\alpha$ 已知是紧凑的（GT，I, §9, No. 6，提案 8）；我们用$X$的$p_\alpha$典范映射表示为$X_\alpha$。

很明显，$(\mathscr{M}(X_\alpha; \mathbf{C}), (p_{\alpha\beta})_* )$是向量空间的*逆系*，$((p_\alpha)_*)$是线性映射的*逆系*，这证明了以下定义的合理性：

#### 定义 2 {#int-iii-s4-def-2 .statement tag=08OO}

*家庭* $(\mu_\alpha)_{\alpha \in I}$，*其中，对于每个* $\alpha \in I$，$\mu_\alpha$ *是对*$X_\alpha$的测量，*据说是逆系测量，如果，每当*$\alpha \leq \beta$，$\mu_\alpha = (p_{\alpha\beta})_*(\mu_\beta)$。 *测量* $\mu$ *在* $X = \lim_{\leftarrow} X_\alpha$ *据说是逆系* $(\mu_\alpha)$ *如果* $\mu_\alpha = (p_\alpha)_*(\mu)$ *对于每个* $\alpha \in I$ 的逆极限。

#### 命题 8 {#int-iii-s4-prop-8 .statement tag=08OP}

(i) *如果逆系* $(\mu_\alpha)$ *在* $X_\alpha$ *上的度量有逆极限，则极限是唯一的。*
(ii) *如果逆系* $(\mu_\alpha)$ *有逆极限，则范数* $(\|\mu_\alpha\|)$ *的族是有界的。*
(iii) *如果* $p_{\alpha\beta}$ *是满射且族* $(\|\mu_\alpha\|)$ *有界，则逆系测度* $(\mu_\alpha)$ *有逆极限。*

(iv) *如果 $p_{\alpha \beta}$ 是满射的，则每个逆系 $(\mu_\alpha)$ 的正测度都有逆极限 $\mu$，这是对 $X$ 的正测度，并且对于所有 $\alpha$ 都有 $\| \mu \| = \| \mu_\alpha \|$。

(i) 我们首先证明以下引理：

#### 引理 3 {#int-iii-s4-lem-3 .statement tag=08OQ}

— *令 F 为函数 $f \in \mathscr{C}(X; \mathbf{C})$ 的集合，具有以下性质：存在 $\alpha \in I$ 和函数 $f_\alpha \in \mathscr{C}(X_\alpha; \mathbf{C})$，使得 $f = f_\alpha \circ p_\alpha$。那么 F 是 $\mathscr{C}(X; \mathbf{C})$ 的稠密线性子空间。*

我们注首先，如果$g = g_\beta \circ p_\beta$和$h = h_\gamma \circ p_\gamma$，其中$g_\beta \in \mathscr{C}(X_\beta; \mathbf{C})$和$h_\gamma \in \mathscr{C}(X_\gamma; \mathbf{C})$，则存在$\alpha \in I$使得$\alpha \geq \beta$和$\alpha \geq \gamma$，因此存在$p_\beta = p_{\beta \alpha} \circ p_\alpha$，$p_\gamma = p_{\gamma \alpha} \circ p_\alpha$，这表明
$$
g + h = (g_\beta \circ p_{\beta \alpha} + h_\gamma \circ p_{\gamma \alpha}) \circ p_\alpha
$$
属于至 F；类似地，$gh \in F$；因此，F 是 $\mathscr{C}(X; \mathbf{C})$ 的 *C*-子代数，其中包含为常量，且关系 $f \in F$ 蕴涵$\overline{f} \in F$。最后，如果$x \neq y$是X的两个点，则存在$\alpha \in I$使得$p_\alpha(x) \neq p_\alpha(y)$，因此存在函数$f_\alpha \in \mathscr{C}(X_\alpha; \mathbf{C})$使得$f_\alpha(p_\alpha(x)) \neq f_\alpha(p_\alpha(y))$。因此，结论来自 Stone–Weierstrass 定理（GT，X, §4, No. 4，Prop. 7）。

引理成立后，令$\mu, \mu'$为X的两个测度，使得$(p_\alpha)_*(\mu) = (p_\alpha)_*(\mu')$适用于所有$\alpha \in I$；这意味着，对于每个 $\alpha \in I$ 和每个函数 $f_\alpha \in \mathscr{C}(X_\alpha; \mathbf{C})$，我们有
$$
\langle f_\alpha, (p_\alpha)_*(\mu) \rangle = \langle f_\alpha, (p_\alpha)_*(\mu') \rangle,
$$
即$\langle f_\alpha \circ p_\alpha, \mu \rangle = \langle f_\alpha \circ p_\alpha, \mu' \rangle$；在其他字，$\mu$和$\mu'$重合上，$\mathscr{C}(X; \mathbf{C})$的子空间F，其稠密为引理3，因此$\mu = \mu'$，证明了(i)。

(ii) 关系 (15) 应用于$p_\alpha$表明，如果$\mu$是逆系$(\mu_\alpha)$的逆极限，必然
$$
\| \mu \| \geq \| \mu_\alpha \|
$$
对于所有$\alpha \in I$。

(iii) 假设 $p_{\alpha \beta}$ 是满射的；人们知道$p_\alpha$也是如此（GT，I, §9, No. 6，提案8）。考虑度量 $(\mu_\alpha)$ 的逆系，让我们首先证明在* F 上存在线性形式 $\lambda$（在引理 3 的记号中），这样，对于每个$\alpha \in I$ 和每个$f_\alpha \in \mathscr{C}(X_\alpha; \mathbf{C})$，都有$\lambda(f_\alpha \circ p_\alpha) = \mu_\alpha(f_\alpha)$。为此，令$\beta, \gamma$为I中的两个指标，且$f_\beta \in \mathscr{C}(X_\beta; \mathbf{C})$、$f_\gamma \in \mathscr{C}(X_\gamma; \mathbf{C})$为两个函数，使得$f_\beta \circ p_\beta = f_\gamma \circ p_\gamma$；则存在指标 $\alpha \in I$ 使得 $\alpha \geq \beta$ 和 $\alpha \geq \gamma$，因此
$$
p_\beta = p_{\beta \alpha} \circ p_\alpha ,\ p_\gamma = p_{\gamma \alpha} \circ p_\alpha \quad \text{and} \quad (f_\beta \circ p_{\beta \alpha}) \circ p_\alpha = (f_\gamma \circ p_{\gamma \alpha}) \circ p_\alpha ;
$$

由于$p_\alpha$是满射，这意味着$f_\beta \circ p_{\beta \alpha} = f_\gamma \circ p_{\gamma \alpha}$，因此

$$
\mu_\alpha(f_\beta \circ p_{\beta \alpha}) = \mu_\alpha(f_\gamma \circ p_{\gamma \alpha});
$$

但到了定义，最后一个关系也可能会写成$\mu_\beta(f_\beta) = \mu_\gamma(f_\gamma)$，从而我们的断言。

既然如此，假设存在有限的数$a > 0$，使得$\| \mu_\alpha \| \leq a$对于所有$\alpha \in I$；那么，对于每个函数 $f_\alpha \in \mathscr{C}(X_\alpha; \mathbf{C})$，

$$
|\lambda(f_\alpha \circ p_\alpha)| = |\mu_\alpha(f_\alpha)| \leq a \| f_\alpha \| = a \| f_\alpha \circ p_\alpha \|
$$

因为 $p_\alpha$ 是满射的。这表明线性形式$\lambda$在$F$上是连续的，并且从引理3得出$\lambda$可以扩展到$X$上的测度$\mu$，使得$(p_\alpha)_*(\mu) = \mu_\alpha$对于所有$\alpha \in I$，这证明了(iii)。

(iv) 为了证明$\mu$的存在，通过(iii)，验证范数$(\| \mu_\alpha \|)$族是有界的就足够了。但是$\| \mu_\alpha \| = \mu_\alpha(1)$，并且当$\alpha \leq \beta$时，关系$\mu_\alpha = (p_{\alpha \beta})_*(\mu_\beta)$意味着$\mu_\alpha(1) = \mu_\beta(1)$；由于$I$是有向的，因此所有措施$\mu_\alpha$的总质量相等，从而我们的断言。而且，子空间$F$显然满足命题9 §1, No. 7的性质(P)，因此逆极限测度$(\mu_\alpha)$的$\mu$为正。最后，关系$\mu_\alpha = (p_\alpha)_*(\mu)$如上所示，即$\mu(1) = \mu_\alpha(1)$。

#### 例 {#int-iii-s4-n5-exa-1 .statement tag=08OR}

— 令 $(X_\lambda)_{\lambda \in L}$ 为紧致空间族； 集合 $X = \prod_{\lambda \in L} X_\lambda$，并且对于 $L$ 中的每个有限子集 $J$，集合 $X_J = \prod_{\lambda \in J} X_\lambda$；用$\mathrm{pr}_J : X \to X_J$和$\mathrm{pr}_{J, K} : X_K \to X_J$（对于$J \subset K$）表示规范的投影。我们知道，$(X_J, \mathrm{pr}_{JK})$是紧凑空间的逆系，连续映射$(\mathrm{pr}_J)$的系统的逆极限是$X$的*同态*到逆极限空间 $\lim_{\leftarrow} X_J$，允许一到认同这两个空间（GT、I, §4, No. 4和S、III, §7, No. 2、*注* 3）。由于投影 $\mathrm{pr}_{J, K}$ 是满射，根据第 8 条命题，集合 $\mathscr{M}(X; \mathbf{C})$（分别为 $\mathscr{M}_+(X)$）可以与逆系 $(\mu_J)$ 的集合识别，这样范数的族$(\| \mu_J \|)$ 是有界的（分别使得 $\mu_J$ 都是正数，并且总质量必须相同）。

Let us consider in particular the case where, for each $\lambda \in L$, a measure $\mu_\lambda$ is given on $X_\lambda$ and one sets $\mu_J = \bigotimes_{\lambda \in J} \mu_\lambda$. 如果$J \subset K$是$I$的两个有限子集，那么对于每个函数$f_J \in \mathscr{C}(X_J; \mathbf{C})$，凭借No. 4的公式(14)，我们有，

$$
\mu_K(f_J \circ \mathrm{pr}_{J, K}) = \mu_J(f_J) \cdot \prod_{\lambda \in K - J} \mu_\lambda(1).
$$

因此，为了使$(\mu_J)$成为逆系措施，$\mu_\lambda = 0$适用于所有$\lambda \in L$或$\mu_\lambda(1) = 1$适用于所有$\lambda \in L$是必要且充分的。

### 6. 无限乘积测量

令$(X_\lambda)_{\lambda \in L}$为紧凑空间族，对于每个$\lambda \in L$，令$\mu_\lambda$为$X_\lambda$的测度。我们保留No. 5的例中的记号，因此对于$L$的每个有限子集$J$，特别是$\mu_J = \bigotimes_{\lambda \in J} \mu_\lambda$。

#### 命题 9 {#int-iii-s4-prop-9 .statement tag=08OS}

*假设所有度量 $\mu_\lambda$ 均为正数，并且族 $(\mu_\lambda(1))_{\lambda \in L}$ 可与 $\mathbf{R}_+$ 相乘（乘积可能为 0）。那么$X$上存在且仅有一个测度$\mu$，使得对于$L$的每一个有限子集$J$和每一个函数$f_J \in \mathscr{C}(X_J; \mathbf{C})$，*

$$
\mu(f_J \circ \mathrm{pr}_J) = \mu_J(f_J) \prod_{\lambda \in L - J} \mu_\lambda(1).
$$

此外，测量值 $\mu$ 为正，其总质量由下式给出

$$
\mu(1) = \prod_{\lambda \in L} \mu_\lambda(1).
$$

令$F$为形式$f_J \circ \mathrm{pr}_J$的$X$上函数的向量空间由……组成，其中$J$超过$L$的有限子集的有向集合，以及$f_J \in \mathscr{C}(X_J; \mathbf{C})$；我们再次说$F$是$X$上连续函数的空间，*仅依赖于有限的数变量*。 No. 5的引理3表明$F$在$\mathscr{C}(X; \mathbf{C})$中是稠密的，这就证明了唯一性断言。如果 $\mu_{\lambda_0} = 0$ 对于某些 $\lambda_0 \in L$，则测度 $\mu = 0$ 满足要求，因为在 (18) 的第二个成员中，如果 $\lambda_0 \in J$，我们有 $\mu_J(f_J) = 0$；如果 $\lambda_0 \notin J$，我们有 $\prod_{\lambda \in L - J} \mu_\lambda(1) = 0$。因此，我们可以假设 $\mu_\lambda \neq 0$ 对于所有 $\lambda \in J$，并且由于测量 $\mu_\lambda$ 是正数，这意味着 $\mu_\lambda(1) \neq 0$ 对于所有 $\lambda \in L$。然后让我们对每个 $\lambda \in L$ 集合 $\mu'_\lambda = \mu_\lambda / \mu_\lambda(1)$，这样 $\mu'_\lambda$ 是 $X_\lambda$ 的正测度，使得$\mu'_\lambda(1) = 1$。然后根据No. 5的第8条命题，总质量1的$X$上存在一个正测度$\mu'$，使得$\mu'(f_J \circ \mathrm{pr}_J) = \mu'_J(f_J)$对应于$L$的每个有限子集$J$和每个函数$f_J \in \mathscr{C}(X_J; \mathbf{C})$。积极措施

$$
\mu = \left( \prod_{\lambda \in L} \mu_\lambda(1) \right) \mu'
$$

那么满足要求，因为

$$
\mu_J(f_J) = \mu'_J(f_J) \cdot \prod_{\lambda \in J} \mu_\lambda(1),
$$
$$
\prod_{\lambda \in L} \mu_\lambda(1) = \prod_{\lambda \in J} \mu_\lambda(1) \cdot \prod_{\lambda \in L - J} \mu_\lambda(1).
$$

提案 9 中定义的措施$\mu$称为积极措施族$(\mu_\lambda)_{\lambda \in L}$的*乘积措施*，并用$\bigotimes_{\lambda \in L} \mu_\lambda$表示。

#### 推论{#int-iii-s4-n6-cor-1 .statement tag=08OT}

*假设9号命题的条件得到验证，令$(L_\rho)_{\rho \in R}$为$L$的划分。那么$(\mu_\lambda)_{\lambda \in L_\rho}$措施族中的每一个都承认乘积措施，乘积措施族$\left( \bigotimes_{\lambda \in L_\rho} \mu_\lambda \right)_{\rho \in R}$都承认乘积措施，并且*

$$
\bigotimes_{\rho \in R} \left( \bigotimes_{\lambda \in L_\rho} \mu_\lambda \right) = \bigotimes_{\lambda \in L} \mu_\lambda.
$$

对于$\mathbf{R}_+$（GT，IV, §7, No. 5，*注*）中的可乘族，这立即从公式（18）和（19）以及乘积的结合性得出。

Exercises

### 习题{#int-iii-s4-exercises}

§ 4](exercises/s4/)参见[习题。
