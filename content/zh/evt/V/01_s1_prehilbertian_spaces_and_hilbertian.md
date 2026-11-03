---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 1
section_title: Prehilbertian spaces and hilbertian spaces
lang: zh
source: evt-i-v
pdf_pages: 0259-0275, 0318-0328
extraction: ocr
subsections:
    - "no": 1
      title: Hermitian forms
      page: 0
      pdf_page: 259
    - "no": 2
      title: Positive hermitian forms
      page: 2
      pdf_page: 260
    - "no": 3
      title: Prehilbertian spaces
      page: 4
      pdf_page: 262
    - "no": 4
      title: Hilbertian spaces
      page: 6
      pdf_page: 264
    - "no": 5
      title: Convex subsets of a prehilbertian space
      page: 9
      pdf_page: 267
    - "no": 6
      title: Vector subspaces and orthoprojectors
      page: 12
      pdf_page: 270
    - "no": 7
      title: Dual of a hilbertian space
      page: 15
      pdf_page: 273
statements: 41
exercises: 37
content_sha256: 656fda7bfc2e72a064c7422e9525f3be317cdd4d9126046990b5831db4aa9aa5
translated_from: content/en/evt/V/01_s1_prehilbertian_spaces_and_hilbertian.md
translation_method: google
source_content_sha256: a3c6df7442ce70b3c022a53d8c8d5c5898d4f54434a40fd2c9ae5e5be4f6a2de
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 7597229cda5a6621362f218f717c7f1263de61d72f0df86f422b160998086ae5
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 1。前希尔伯特空间和希尔伯特空间

### 1. 厄米特形式

我们回想一下代数 (A, IX, § 3, No. 1) 中给出的定义：

#### 定义 1 {#evt-v-s1-def-1 .statement tag=07X0}

令 E 为域 K 上的向量空间。E 上的厄米特形式（左侧）是映射 f，从 E × E 到 K 满足以下条件（对于 E 中的 $x_1, x_2, x, y_1, y_2, y$ 和 K 中的 $\lambda, \mu$）：

(1)
$$
\begin{cases}
f(x_1 + x_2, y) = f(x_1, y) + f(x_2, y) \\
f(x, y_1 + y_2) = f(x, y_1) + f(x, y_2)
\end{cases}
$$

(2)
$$
\begin{cases}
f(\lambda x, y) = \overline{\lambda} f(x, y) \\
f(x, \mu y) = \mu f(x, y)
\end{cases}
$$

(3)
$$
f(x, y) = \overline{f(y, x)} .
$$

当域 K 为 R 时，E 约化上厄米特形式的概念与 E × E (A, III, § 6, No. 3) 上对称双线性形式的概念相同。

我们注意到第二个条件 (1) 和第二个条件 (2) 紧随其他三个。

1 对于对希尔伯特空间特别感兴趣的读者，我们点指出，只有§ 1的No. 7和§ 4的No. 8依赖于章III和IV的结果。为此，读者可以查阅本卷末尾的《巴拿赫空间一些重要性质的总结》。对章、I和II的唯一引用涉及凸集合和半范数（II、p. 1和p. 7）的定义、拓扑直和（I、 p. 4），一个总族和一个拓扑独立族（I，p. 12）。

从（1）和（2）我们立即推断出

$$
f(\sum_j \lambda_j x_j, \sum_k \mu_k y_k) = \sum_{j,k} \overline{\lambda}_j \mu_k f(x_j, y_k).
$$

特别是，如果 E 是有限维的，并且如果 $(e_j)_{1 \leq j \leq n}$ 是 E 的基，则对于 $x = \sum_{j=1}^n \xi_j e_j$ 和 $y = \sum_{j=1}^n \eta_j e_j$，我们有，

$$
f(x, y) = \sum_{j,k} \alpha_{jk} \overline{\xi}_j \eta_k
$$

与记号 $\alpha_{jk} = f(e_j, e_k)$；此外，对于指标$j, k$的每对，关系 (3) 等于$\alpha_{jk} = \overline{\alpha}_{kj}$；这特别意味着数 $\alpha_{jj}$ 是真实的。

从(3)可知，数$Q(x) = f(x, x)$对于所有$x \in E$都是真实的。此外，我们立即建立以下公式，称为*极化*公式

(5)
$$
4f(x, y) = \sum_{\varepsilon^2 = 1} \varepsilon Q(x + \varepsilon y) \quad \text{if } K \text{ is } \mathbf{R},
$$
(6)
$$
4f(x, y) = \sum_{\varepsilon^4 = 1, \varepsilon \in \mathbf{C}} \varepsilon Q(x + \overline{\varepsilon} y) \quad \text{if } K \text{ is } \mathbf{C}.
$$

#### 注 {#evt-v-s1-n1-rem-1 .statement tag=07X1}

— 我们观察到，公式 (6) 对于 $E \times E$ 上的每个 *sesquilinear* 形式都有效（也就是说，对于每个函数 $f$ 满足 (1) 和 (2)，但不一定是 (3)）。这个注表明，当$K = \mathbf{C}$时，一个倍半线性形式$f$使得$f(x, x)$对于所有$x \in E$都是真实的必然是*厄米特*：关系（6）然后给出$\overline{f(y, x)} = f(x, y)$，因为我们有$y + \varepsilon x = \varepsilon(x + \overline{\varepsilon} y)$并且每当$\varepsilon^4 = 1$时$Q(\varepsilon z) = Q(z)$。

从极化公式，我们特别有，

#### 命题 1 {#evt-v-s1-prop-1 .statement tag=07X2}

*如果$f$是$E$上的埃尔米特形式，并且$M$是$E$的向量子空间，使得$f(x, x) = 0$适用于所有$x \in M$，那么对于$M$中的每对点$x, y$，我们也有$f(x, y) = 0$。*

令$f$在$E$上为厄米特形式；所有$x \in E$的集合$N$，使得所有$y \in E$的$f(x, y) = 0$是$E$的向量子空间。从 (3) 可以得出，如果 $x_1 \equiv x_2$ (mod. $N$) 和 $y_1 \equiv y_2$ (mod. $N$)，我们有 $f(x_1, y_1) = f(x_2, y_2)$；因此，在商空间$E/N$，我们定义通过将$f(\dot{x}, \dot{y}) = f(x, y)$放入所有$x \in \dot{x}$和所有$y \in \dot{y}$，得到一个倍半线性的形式$f$；很明显，$f$是厄米特，并且关系“$f(\dot{x}, \dot{y}) = 0$对于所有$\dot{y} \in E/N$”意味着$E/N$中的$\dot{x} = 0$，在其他字（A，IX）$f$正在分离。我们说 $f$ 是与 $f$ *分离* 厄米特形式 *关联*。

### 2. 正厄米特形式

#### 定义 2 {#evt-v-s1-def-2 .statement tag=07X3}

*令 $E$ 为向量空间超过域 $K$。如果 $f(x, x) \geq 0$ 对于所有 $x \in E$，则 $E$ 上的厄米特形式 $f$ 被认为是正数。*

很明显，向量空间$E$上的厄米形式形成了一个向量空间*在场*$\mathbf{R}$上（但不是在场$\mathbf{C}$上，当$K$是$\mathbf{C}$时）：在这个空间中，正厄米形式构成*尖凸真锥*（II，p. 10）作为def的结果。 2 和支柱。 1.

#### 命题 2 {#evt-v-s1-prop-2 .statement tag=07X4}

— *如果 f 是正数厄米特形式，我们有*

$$
|f(x, y)|^2 \leq f(x, x) \ f(y, y)
$$

*对于 E 中的每个 x 和 y* (Cauchy-Schwarz 不等式)。

首先假设我们有$f(y, y) \neq 0$。对于每个$\xi \in \mathbf{K}$，我们有

$$
f(y, y) \ f(x + \xi y, x + \xi y) \geq 0
$$

可以写成

$$
f(x, x) \ f(y, y) - |f(x, y)|^2 + (\xi f(y, y) + \overline{f(x, y)}) (\overline{\xi} f(y, y) + f(x, y)) \geq 0 .
$$

替换$\xi$乘以$-\overline{f(x, y)}/f(y, y)$，在这个不等式中，我们得到(7)。如果$f(x, x) \neq 0$，我们也有类似的论证。

最后，如果$f(x, x) = f(y, y) = 0$，对于所有$\xi \in \mathbf{K}$，我们有$f(x + \xi y, x + \xi y) \geq 0$，可以写为

$$
\xi f(x, y) + \overline{\xi} f(x, y) \geq 0 .
$$

替换$\xi$乘以$-\overline{f(x, y)}$，在这个不等式中，我们得到$-2 \ |f(x, y)|^2 \geq 0$，因此$f(x, y) = 0$；在这种情况下我们再次得到（7）。

#### 推论 1 {#evt-v-s1-prop-2-cor-1 .statement tag=07X5}

— *如果 f 是 E 中所有 x \in 的正数厄米特形式、集合 N，则 f(x, x) = 0 重合，且 E 中所有 x \in 的向量子空间，使得 E 中所有 y f(x, y) = 0。*

#### 推论 2 {#evt-v-s1-prop-2-cor-2 .statement tag=07X6}

— *对于正厄米特形式来说，关系 x \neq 0 意味着 f(x, x) > 0 是必要且充分的。*

这立即来自 cor。 1.

对于 E 上的每个正厄米特形式 f，与 f (V, p. 2) 相关的分隔厄米特形式显然是 E/N 上的正厄米特形式。

#### 命题 3 {#evt-v-s1-prop-3 .statement tag=07X7}

— *令 f 为 E 上的正厄米特形式。Put*

$$
p(x) = f(x, x)^{1/2}
$$

*对于 E 中的所有 x \in。则 p 是 E 上的半范数，并且当且仅当 f 分离时才是范数。*

证明不等式$p(x + y) \leq p(x) + p(y)$就足够了。但我们有

$$
f(x + y, x + y) = f(x, x) + f(y, y) + f(x, y) + \overline{f(x, y)}
$$

以及，柯西-施瓦茨不等式

$$
f(x + y, x + y) \leq f(x, x) + f(y, y) + 2(f(x, x) f(y, y))^{1/2}
$$
$$
= (f(x, x)^{1/2} + f(y, y)^{1/2})^2 .
$$

#### 注 {#evt-v-s1-n2-rem-1 .statement tag=07X8}

— 1) 假设 f 为正且可分离，令 x, y 为两个向量 $\neq 0$。 Cauchy-Schwarz 不等式的证明表明，如果(7)的两个成员相等，则存在标量$\xi$使得$f(x + \xi y, x + \xi y) = 0$，因此$x + \xi y = 0$，在其他字，$x$和$y$是*线性相关的*； 逆命题是直接的。 不等式 (8) 的证明表明，仅当 $x$ 和 $y$ 线性相关时，等式 $p(x + y) = p(x) + p(y)$ 才可能；如果$y = \lambda x$，则前面的等式可以写成$|1 + \lambda| = 1 + |\lambda|$，并且暗示$\lambda$是*实且正的*。

2) 令$f$为$E$上的正厄米特形式，并让$E$被赋予半范数$x \mapsto f(x, x)^{1/2}$；如果 $f$ 为正，则将$E/N$上定义的厄米特形式与$f$相关联，则将范数 $x \mapsto f(\dot{x}, \dot{x})^{1/2}$赋值给$E/N$得到的赋范空间就是与空间相关联的赋范空间 $E$（II、p. 5）。

#### 定义 3 {#evt-v-s1-def-3 .statement tag=07X9}

*令 $E$ 为向量空间超过域 $K$。如果 $E$ 上存在正的厄米特形式 $f$，使得 $p(x) = f(x, x)^{1/2}$ 对于所有 $x \in E$* 来说，$E$ 上的半范数 $p$ 被称为前希尔伯特式。

观察对于 $E$ 的半范数 $p$，至多存在一个正厄米特形式 $f$，使得 $p(x) = f(x, x)^{1/2}$ 对于所有 $x \in E$；这是由极化公式（V，p. 2）得出的。

### 3. 前希尔伯特空间

#### 定义 4 {#evt-v-s1-def-4 .statement tag=07XA}

*前希尔伯特空间为集合$E$，结构为向量空间超过$K$，并且厄米特形式为正。当$K$是$\mathbf{R}$（或$K$是$\mathbf{C}$）时，我们说$E$是实数（或复数）前希尔伯特空间。

#### 例 1 {#evt-v-s1-n3-exa-1 .statement tag=07XB}

形式 $(\lambda, \mu) \mapsto \overline{\lambda} \mu$ 定义 $K$ 上的前希尔伯特结构，据说是*规范*。当$K$被认为是前希尔伯特空间时，我们总是意味着除非，否则提到它有这个结构。

#### 例 2 {#evt-v-s1-n3-exa-2 .statement tag=07XC}

令$I$为$\mathbf{R}$中的区间（有界或无界），并令$E$为在$I$上定义的受管制函数（FVR，II，p. 4）的集合，其中值 $\mathbf{C}$，具有紧凑的支撑。显然，$E$比$\mathbf{C}$弱于向量空间；设 $f$ 为倍半线性形式 $(x, y) \mapsto \int_1^1 \overline{x(t)}\ y(t)\ dt$； 直接的$f$是$E$上的正厄米特形式，因此定义在空间上是前希尔伯特结构。

#### 例 3 {#evt-v-s1-n3-exa-3 .statement tag=07XD}

设$n \geqslant 0$为整数。我们定义前希尔伯特空间结构在空间$K^n$，通过厄米特形式

$$
(x, y) \mapsto \sum_{j=1}^n \overline{x_j} y_j
$$

（对于 $x = (x_1, ..., x_n)$ 和 $y = (y_1, ..., y_n)$）。当$K$为$\mathbf{R}$时，我们看到这只是$\mathbf{R}^n$的两个向量的标量乘积（GT，VI, § 2, No. 2）。

#### 例 4 {#evt-v-s1-n3-exa-4 .statement tag=07XE}

令$\ell^2$（或$\ell^2(\mathbf{N})$）为$K$的序列$x = (x_n)_{n \in \mathbf{N}}$或元素的集合，使得$\sum_{n=0}^\infty |x_n|^2$是有限的。通过厄米特形式 $(x, y) \mapsto \sum_{n=0}^\infty \overline{x_n} y_n$，可以证明$\ell^2$是$K^\mathbf{N}$的向量子空间，定义是$\ell^2$上的前希尔伯特空间结构 （cf.V、p. 18）。

#### 例 5 {#evt-v-s1-n3-exa-5 .statement tag=07XF}

令 $E$ 为真正的前希尔伯特空间，$f$ 相应的在$E$ 上对称双线性形式。令$E_{(c)}$为$E$的向量空间复化；我们将认同$E$和$E_{(c)}$的子集乘以映射$x \mapsto 1 \otimes x$，这样$E_{(c)}$的每个元素都可以唯一地写成$x_1 + ix_2$和$x_1, x_2$ $E$。 映射 $f$ 扩展 $E_{(c)}$ 上的厄米特形式 $f_{(c)}$ 独有；我们有，

$$
f_{(c)}(x_1 + ix_2, y_1 + iy_2) = f(x_1, y_1) + f(x_2, y_2) + i(f(x_1, y_2) - f(x_2, y_1)) .
$$

特别是，我们有
$$
f_{(\mathbf{C})}(x_1 + ix_2, x_1 + ix_2) = f(x_1, x_1) + f(x_2, x_2) \geqslant 0,
$$
因而 $f_{(\mathbf{C})}$ 为正。我们说 $E_{(\mathbf{C})}$ 和 $f_{(\mathbf{C})}$ 是 $E$ 的*前希尔伯特空间复化*。

每当仅考虑向量空间 $E$ 上的一个前希尔伯特空间结构时，值，对 $(x, y)$，点，$E$，厄米特形式，其中定义，所述结构表示为$\langle x|y \rangle_E$或简称为$\langle x|y \rangle$，如果不会引起混淆的话。这个数称为$x$和$y$的*标量乘积* $^1$（如果$y = x$则为$x$的*标量平方*）。如果 $\langle x|y \rangle = 0$，则两个向量 $x, y$ 被称为“正交”。 函数 $x \mapsto \|x\| = \langle x|x \rangle^{1/2}$ 是向量空间 $E$ (V, p. 3) 上的*半范数*；前希尔伯特空间始终被认为具有分配给它的半范数（因此也具有相应的拓扑和均匀结构）。

有了这些记号，在前希尔伯特空间$E$中，柯西-施瓦茨不等式可以写成
$$
|\langle x|y \rangle| \leqslant \|x\| \cdot \|y\|.
$$

因而，标量乘积是$E \times E$上的*连续倍半线性形式*（II，p. 5，道具4）。

在阶中，$E$是Hausdorff，$x \mapsto \|x\|$是$E$上的*范数*是充分必要的；在其他字中，厄米特形式 $(x, y) \mapsto \langle x|y \rangle$ *为正且分离*；这相当于说，*$0$是$E$中唯一的向量，它与自身正交*。

根据一般定义（S，IV, § 1, No. 5），同构从前希尔伯特空间$E$到前希尔伯特空间$F$是双射线性映射$u$从$E$到$F$ 这样
$$
\langle u(x)|u(y) \rangle = \langle x|y \rangle
$$
对于$E$中的每个$x$和$y$。由此我们推断，对于所有$x \in E$，$\|u(x)\| = \|x\|$，对于$E$和$F$的拓扑向量空间结构，$u$显然是同构；如果$E$和$F$是Hausdorff，则$u$是从$E$到$F$的*等距*。相反，如果$u$是从$E$到$F$的双射线性映射，使得$\|u(x)\| = \|x\|$对于所有$x \in E$，则极化公式（V，p. 2）表明$u$是前希尔伯特空间同构从$E$到$F$。

令$E$为*复*前希尔伯特空间，而$\langle x|y \rangle$为$E$中的标量乘积。在集合$E$，我们可以定义相对于$\mathbf{C}$第二个向量空间结构，采用与加法群相同的律以及外部合成$(\lambda, x) \mapsto \overline{\lambda} x$的律 （A，II, § 1, No. 13）对于这个向量空间结构，$(x, y) \mapsto \langle y|x \rangle$是*正厄米特*

1 可能会发生有时，我们将$(x|y)$写成$\langle y|x \rangle$。观察V、p. 2的公式 (4)，取以下等价的形式：
$$
\begin{align*}
\langle \sum_i \lambda_i x_i | \sum_j \mu_j y_j \rangle &= \sum_{i,j} \overline{\lambda}_i \mu_j \langle x_i|y_j \rangle. \\
(\sum_i \lambda_i x_i | \sum_j \mu_j y_j) &= \sum_{i,j} \lambda_i \overline{\mu}_j (x_i|y_j).
\end{align*}
$$

形式。通过将新的向量空间结构和新的厄米特形式分配给 E 获得的前希尔伯特空间 $\overline{E}$ 被认为是共轭到 E。 同构 $u$ 从 E 到$\overline{E}$是从E到自身的半线性映射（相对于$\mathbf{C}$的自同构$\xi \mapsto \overline{\xi}$），使得$\langle u(y)|u(x) \rangle = \langle x|y \rangle$或$\langle u(x)|u(y) \rangle = \overline{\langle x|y \rangle}$（对于E中的$x, y$）；这样的映射被认为是前希尔伯特空间 E 的半自同构。

如果 E 是预希尔伯特空间，E 的 M 向量子空间，标量乘积 $\langle x|y \rangle$ 到 $M \times M$ 的限制是 M 上的正厄米特形式，则M 上的定义前希尔伯特空间结构；我们说这个结构是由E的结构诱导的，或者说M是E的前希尔伯特子空间。

### 4. 希尔伯特空间

#### 定义 5 {#evt-v-s1-def-5 .statement tag=07XG}

*希尔伯特空间*（或*希尔伯特空间*）*是前希尔伯特空间，它是Hausdorff且完整的*。 *如果向量空间 E（在 K 上）上的范数是前希尔伯特式的，并且赋范的空间 E 是完备的，我们就说它是希尔伯特式的*。

如果 E 是希尔伯特空间并且 M 是 E 的闭向量子空间，则在 M 上导出的前希尔伯特空间结构实际上是希尔伯特空间结构。在这种情况下，我们说 M 以及诱导的结构是 E 的 *希尔伯特子空间*。

#### 例 1 {#evt-v-s1-n4-exa-1 .statement tag=07XH}

V、p. 4 的例 1、3、4 中定义的前希尔伯特空间是希尔伯特空间。另一方面，例 2 中定义的前希尔伯特空间既​​不是豪斯多夫，也不完整。希尔伯特空间的*复化*是希尔伯特空间。

#### 例 2 {#evt-v-s1-n4-exa-2 .statement tag=07XI}

\* 令X为豪斯多夫拓扑空间，并令$\mu$为X的正测度。令$L^2(X, \mu)$为等价类的空间由……组成，对于$\mu$，X上的所有平方$\mu$可积函数与$\mathbf{C}$中的值可积函数。这是一个复希尔伯特空间，其标量乘积由下式给出

$$
\langle f|g \rangle = \int_X \overline{f(x)}\ g(x)\ d\mu(x) .
$$

#### 例 3 {#evt-v-s1-n4-exa-3 .statement tag=07XJ}

\* 令 $n \geqslant 1$ 为整数，并令 U 为 $\mathbf{R}^n$ 中的开集合。令 $\mu$ 为由 $\mathbf{R}^n$ 上的勒贝格测度导出的 U 测度，并放入 $\mathscr{H}^0 = L^2(U, \mu)$。让 $\mathscr{H}^1$ 表示所有函数 $f \in \mathscr{H}^0$ 中的空间以及以下性质；对于 $1 \leqslant i \leqslant n$，存在函数 $g_i \in \mathscr{H}^\circ$ 使得

$$
\int_U g_i(x)\ h(x)\ d\mu(x) = - \int_U f(x)\ D_i h(x)\ d\mu(x)
$$

对于类 $C^1$ 的每个函数 $h$，在 U 中具有紧凑支持。函数 $g_i$ 相对于 $\mu$ 唯一定义到等价，并由 $D_i f$ 或 $\partial f / \partial x_i$ 表示（i 偏导数）。在整数$s \geqslant 1$上的归纳，我们将定义$\mathscr{H}^s$作为所有函数$f \in \mathscr{H}^1$中的集合，这样$D_i f \in \mathscr{H}^{s-1}$对于$1 \leqslant i \leqslant n$。我们通过公式在$\mathscr{H}^s$上得到定义标量乘积

$$
\langle f|g \rangle = \sum_{k=0}^s \sum_{1 \leqslant i_1 \leqslant \ldots \leqslant i_k \leqslant n} \int \overline{D_{i_1} \ldots D_{i_k} f} \cdot D_{i_1} \ldots D_{i_k} g\ d\mu .
$$

那么 $\mathscr{H}^s$ 是一个复希尔伯特空间，称为指标 s 的 *Sobolev 空间*。

#### 例 4 {#evt-v-s1-n4-exa-4 .statement tag=07XK}

\* 设X是类$C^r$（与$r \geqslant 1$）的纯有限维$n$的微分变体。

在向量纤维空间$\Lambda^n T(X)$中，令L为零截面的补集。对于每个实数$\lambda \neq 0$，从$\Lambda^n T(X)$到自身的映射$u \mapsto \lambda u$，L都是稳定的。

令$\alpha$为复数。 L 上的复数值为函数 $\omega$，使得 $u \in L$ 的 $\omega(\lambda u) = |\lambda|^{\alpha} \omega(u)$ 和任何非零实数 $\lambda$ 称为阶 $\alpha$ 的密度 X。如果存在X的开盖$(U_i)_{i \in I}$，并且对于$U_i$上坐标$\xi_i = (\xi_i^1, ..., \xi_i^n)$的每个$i \in I$系统和复数值，我们说阶1的密度$\omega$是局部可积的函数$f_i$关于$\xi_i(U_i)$满足以下条件：

a) 函数 $f_i$ 对于勒贝格测度 $\mu$ 在$\mathbf{R}^n$ 的开集合 $\xi_i(U_i)$ 上是局部可积的；

b) 设 $x \in U_i$；如果$(\partial_{1,i,x}, ..., \partial_{n,i,x})$是$T_x X$的基与$U_i$中坐标$(\xi_i', ..., \xi_i^n)$的系统相关联，我们有
$$
\omega(\partial_{1,i,x} \wedge ... \wedge \partial_{n,i,x}) = f_i(\xi_i^1(x), ..., \xi_i^n(x)) .
$$

那么，X上存在且仅有一个测度$\tilde{\omega}$，使得对于$i \in I$，$\tilde{\omega}$到$U_i$的限制的$\xi_i$下的像等于测度$f_i \cdot \mu$（cf.） VAR，R，10.4.3）。

令$\mathscr{V}$（或$\mathscr{N}$）为可测量密度$\omega$为阶1/2的向量空间，使得与阶1的密度$|\omega|^2$相关的测量是有界的（或空）。设$\omega_1$和$\omega_2$在$\mathscr{V}$中；那么$\omega = \overline{\omega_1} \omega_2$是阶1的密度，并且与$\omega$相关的测度$\tilde{\omega}$是有界的； 数$\int_X \tilde{\omega}$仅取决于$\omega_1$和$\omega_2$模$\mathscr{N}$的类、$\dot{\omega}_1$和$\dot{\omega}_2$，并用$\langle \omega_1 | \omega_2 \rangle$或$\langle \dot{\omega}_1 | \dot{\omega}_2 \rangle$表示。然后映射$(\dot{\omega}_1, \dot{\omega}_2) \mapsto \langle \dot{\omega}_1 | \dot{\omega}_2 \rangle$将复希尔伯特空间结构分配给向量空间$\Omega_{1/2}(X) = \mathscr{V}/\mathscr{N}$。

#### 例 5 {#evt-v-s1-n4-exa-5 .statement tag=07XL}

\* 设 D 为 $\mathbf{C}$ 中中心 0、半径为 1 的开圆盘。 *Hardy 空间* $H^2(D)$ 由所有全纯函数 $f : D \to \mathbf{C}$ 组成，其中
$$
\sup_{0 < R < 1} \int_0^1 |f(R \cdot e(\theta))|^2 d\theta < + \infty .
$$
如果 $f_1$ 和 $f_2$ 属于到 $H^2(D)$，极限
$$
\langle f_1 | f_2 \rangle = \lim_{R \to 1} \int_0^1 \overline{f_1(R \cdot e(\theta))} \cdot f_2(R \cdot e(\theta)) \, d\theta
$$
存在； 映射 $(f_1, f_2) \mapsto \langle f_1 | f_2 \rangle$ 将复希尔伯特空间结构分配给向量空间 $H^2(D)$。

对于函数$f : D \to \mathbf{C}$到属于到$H^2(D)$，存在复数的序列$(a_n)_{n \in \mathbf{N}}$使得$\sum_{n=0}^\infty |a_n|^2 < + \infty$是必要且充分的
$$
f(z) = \sum_{n=0}^\infty a_n z^n
$$
对于所有$z \in D$。然后我们有 $\|f\|^2 = \sum_{n=0}^\infty |a_n|^2$，它将 $H^2(D)$ 的同构转换为希尔伯特空间 $\ell^2$（V，p. 4）。

每个 Hausdorff prehilbertian 空间都同构于直到同构的希尔伯特空间的处处稠密子空间。准确地说：

#### 命题 4 {#evt-v-s1-prop-4 .statement tag=07XM}

— *令 E 为 Hausdorff prehilbertian 空间、$\hat{E}$ E*(GT、IX, § 3, No. 3) 的规范空间完成。标量乘积* $(x, y) \mapsto \langle x|y \rangle$ *扩展通过连续性到正值并在* $\hat{E}$ 上分离厄米特形式，*和定义希尔伯特空间结构在* $\hat{E}$。

$(x, y) \mapsto \langle x|y \rangle$到$\hat{E} \times \hat{E}$的扩张的存在源自于这个半线性的形式和$E \times E$的连续性（GT，III, § 6, No. 5，第1）。此外，这个扩张也将被$(x, y) \mapsto \langle x|y \rangle$表示为厄米特形式并且满足关系$\langle x|x \rangle = \|x\|^2$，凭借扩张的原理恒等式（$\|x\|$是$\hat{E}$上的范数是通过在E上连续扩展范数获得的）；这证明关系$\langle x|x \rangle = 0$蕴含$x = 0$在$\hat{E}$中，因此形式$(x, y) \mapsto \langle x|y \rangle$是正的且分离的，因此定义是希尔伯特空间结构 $\hat{E}$。 Q.E.D.

这个希尔伯特空间据说是豪斯多夫前希尔伯特空间E的“完成”。

\* *例 6*。 — 令 U 为 $\mathbf{R}^n$ ($n \geqslant 1$) 的开子集。令 $\mathscr{C}_0^1(\mathrm{U})$ 为类 $\mathrm{C}^1$ 的所有函数的向量空间，且具有 U 的紧凑支持。我们定义 $\mathscr{C}_0^1(\mathrm{U})$ 上的豪斯多夫前希尔伯特空间结构，其标量乘积由下式给出

$$
\langle f|g \rangle = \sum_{i=1}^{n} \int_{\mathrm{U}} \overline{\mathrm{D}_i f(x)} . \mathrm{D}_i g(x) \, dx .
$$

这个前希尔伯特空间并不完整。它的补全称为与 U 相关的 *Dirichlet 空间*。 \*

#### 推论 {#evt-v-s1-n4-cor-1 .statement tag=07XN}

— *令 V 在 K 上为向量空间，并且 f 在 V 上为正厄米特形式。*
a) *对于 V 中的 x、y，存在希尔伯特空间 E 和线性映射* $u : V \to E$ *使得* $f(x, y) = \langle u(x)|u(y) \rangle$ *，并且使得 u(V) 在 E 中稠密。*
b) *如果两个对* $(E_i, u_i)$ *满足条件类似于a)，则存在唯一的同构* $\phi$ *从希尔伯特空间* $E_1$ *到希尔伯特空间* $E_2$ *这样* $u_2 = \phi \circ u_1$。

令 N 为所有 $x \in V$ 中的集合，使得 $f(x, x) = 0$。我们将定义正数并在空间V/N上将厄米特形式分开，通过$\langle \dot{x}|\dot{y} \rangle = f(x, y)$为$x \in \dot{x}$和$y \in \dot{y}$。令E为从V到E的V/N和$u$映射$x \mapsto x + N$的希尔伯特空间补全。则满足*a*)的条件。

在*b*)的假设下，N等于$u_1$的核和$u_2$。因此，存在从$u_1(V)$到$u_2(V)$的双射线性映射$\phi_0$，使得$u_2(x) = \phi_0(u_1(x))$对于所有$x \in V$。我们立即验证$\phi_0$是前希尔伯特空间的同构，因此是等距的。由于对于 $i = 1, 2$，$u_i(V)$ 在 $E_i$ 中是稠密的，因此 $\phi_0$ 扩展唯一地对应于从 $E_1$ 到 $E_2$ 的等距$\phi$，并且 *b*) 如下。

我们说希尔伯特空间 E 是 V 的*分离完成*（对于形式 *f*）。

#### 例 7 {#evt-v-s1-n4-exa-7 .statement tag=07XO}

令 G 为群（其中单位元 1）和 $\pi$ 同态，从 G 到复数希尔伯特空间 E 的自同构的群；我们说 $\pi$ 是 G 在 E 中的 *酉表示*。令 $a \in E$ ；我们把

$$
\phi(x) = \langle a|\pi(x).a \rangle
$$

对于所有$x \in G$。那么$\phi : G \to \mathbf{C}$是*正定*，另外字满足关系：

(PD) 对于$\mathbf{C}$中的每个$\lambda_1, ..., \lambda_n$和$G$中的$x_1, ..., x_n$，我们有

$$
\sum_{i,j=1}^n \overline{\lambda_i} \lambda_j \phi(x_i^{-1} x_j) \geqslant 0 .
$$

事实上，(11)的第一个成员正是$\| \sum_{i=1}^n \lambda_i \pi(x_i) . a \| ^2$。

相反，令$\phi$为$G$上的正定函数。令$C^{(G)}$为所有函数中的向量空间，其中有限支撑位于$G$上。我们定义厄米特形式$\Phi$于$G$

$$
\Phi(u, v) = \sum_{x,y \in G} \overline{u(x)} \ v(y) \ \phi(x^{-1} y)
$$

关系(PD)表示$\Phi$为正。通过推论的道具。 4、存在希尔伯特空间$E$和线性映射$\rho : C^{(G)} \to E$，以及稠密的像，使得

$$
\Phi(u, v) = \langle \rho(u)|\rho(v) \rangle \quad \text{for} \quad u, v \quad \text{in} \quad C^{(G)} .
$$

对于每个$x \in G$，令$\gamma_x$为$C^{(G)}$中$x$的左平移，由$\gamma_x u(y) = u(x^{-1} y)$为$u \in C^{(G)}$和$y \in G$定义。我们有$\Phi(\gamma_x u, \gamma_x v) = \Phi(u, v)$。现在应用推论的断言 b) 道具。 4到$\rho$和$\rho \circ \gamma_x$：希尔伯特空间$E$存在唯一的自同构$\pi(x)$，使得$\rho \circ \gamma_x = \pi(x) \circ \rho$。我们立即看到，$\pi$是从$G$到自同构的群到$E$的同态。

令 $\delta$ 为$G$ 中$x \neq 1$ 的$\delta(1) = 1, \delta(x) = 0$ 所定义的$C^{(G)}$ 的元素。我们对所有 $u \in C^{(G)}$ 都有 $u = \sum_{x \in G} u(x) . \gamma_x \delta$，因此通过放入 $a = \rho(\delta)$ 可以得到 $\rho(u) = \sum_{x \in G} u(x) \ \pi(x) . a$。

公式 (12) 和 (13) 意味着$\phi(x) = \langle a|\pi(x).a \rangle$ 对于所有 $x \in G$。我们注意到，对于所有 $x \in G$，向量 $\pi(x).a$ 中的集合总计为 $E$。

### 5. 前希尔伯特空间的凸子集

如果我们对前希尔伯特空间$E$的任意两个点$x, y$进行计算$\| x - y \| ^2 = \langle x - y|x - y \rangle$和$\| x + y \| ^2 = \langle x + y|x + y \rangle$，我们立即得到“中位数的恒等式”

$$
\| \frac{1}{2}(x + y) \| ^2 + \| \frac{1}{2}(x - y) \| ^2 = \frac{1}{2} (\| x \| ^2 + \| y \| ^2 ) .
$$

从这个恒等式我们推导出以下命题：

![图表显示集合 B'、B 和 A，其中 x 和 y 标记在 A 内](https://i.imgur.com/3Q5z5QG.png)

图 1.

#### 命题 5 {#evt-v-s1-prop-5 .statement tag=07XP}

— 设 $E$ 为前希尔伯特空间。令$d$为实数$> 0$，$\delta$实数，使得$0 \leqslant \delta \leqslant d$。令$B$和$B'$为由$\| x \| < d$定义的$E$中的子集，

$$
\|x\| \leq d + \delta \text{ respectively, and let } A \text{ be a convex set contained in } B' - B. \text{ Then for every pair of points } x, y \text{ of } A, \text{ we have } \|x - y\| \leq \sqrt{12d\delta} \text{ (fig. 1).}
$$
事实上，我们有$\frac{1}{2}(x + y) \in A$，因此$\left\| \frac{1}{2}(x + y) \right\| \geq d$；因此从 (14) 我们得到不等式
$$
\left\| \frac{1}{2}(x - y) \right\|^2 = \frac{1}{2}(\|x\|^2 + \|y\|^2) - \left\| \frac{1}{2}(x + y) \right\|^2 \leq (d + \delta)^2 - d^2 \leq 3d\delta
$$
由此得出命题。

#### 定理 1 {#evt-v-s1-thm-1 .statement tag=07XQ}

*设 E 为前希尔伯特空间，H 为 E 的非空凸子集，使得 H 为 Hausdorff 且 E 的完全一致子空间。对于每个 $x \in E$，H 中存在唯一的点 $p_H(x)$，使得 $\|x - p_H(x)\| = \inf_{y \in H} \|x - y\|$。 H 的元素 $p_H(x)$ 也是 H 满足关系* 的唯一元素 a
$$
\Re \langle x - a | y - a \rangle \leq 0
$$
*对于所有人*$y \in H$。

![图表显示点 x、点 y 和标记为 a + λ(y − a) 的线段](https://i.imgur.com/3Q5z5QG.png)

图 2.

放置$d = \inf_{y \in H} \|x - y\|$，对于每个整数$n > 0$，令$H_n$为H的点$y$的集合，使得$\|x - y\| \leq d + n^{-1}$。 集合 $H_n$ 在 H 中封闭，是凸且非空的，对于所有足够大的 $n$，其直径以 $\sqrt{12 \frac{d}{n}}$ 为界，由 prop. 5. 序列$(H_n)_{n \geq 1}$为递减，集合H为豪斯多夫并完成，柯西滤波器$(H_n)_{n \geq 1}$的基收敛于H的点$p_H(x)$；我们有$\{ p_H(x) \} = \bigcap_{n \geq 1} H_n$，因此$p_H(x)$是H的唯一点$a$，使得$\|x - a\| = d$。

1 我们记得（GT，VIII, § 1, No. 1）$\Re(z)$表示复数z的实部分；如果 z 是实数，我们有 $\Re(z) = z$。

设 $y \in \mathbf{H}$；由于$\mathbf{H}$是凸的，对于每个实数$\lambda$，E属于到$\mathbf{H}$的点$z(\lambda) = p_{\mathbf{H}}(x) + \lambda(y - p_{\mathbf{H}}(x))$使得$0 < \lambda < 1$。因此我们有
$$
\| x - z(\lambda) \|^{2} \geq \| x - p_{\mathbf{H}}(x) \|^{2} \quad \text{for} \quad 0 < \lambda < 1 ,
$$
这给出了
$$
\mathscr{R} \langle x - p_{\mathbf{H}}(x)|y - p_{\mathbf{H}}(x) \rangle = \lim_{\lambda \to 0} \frac{1}{2\lambda} \left\{ \| x - p_{\mathbf{H}}(x) \|^{2} - \| x - z(\lambda) \|^{2} \right\} \leq 0 .
$$
相反，令 $a$ 为 $\mathbf{H}$ 的点，使得 $\mathscr{R} \langle x - a|y - a \rangle \leq 0$ 对于所有 $y \in \mathbf{H}$。对于每个 $y \in \mathbf{H}$，我们有
$$
\| x - y \|^{2} = \| x - a \|^{2} + \| y - a \|^{2} - 2 \mathscr{R} \langle x - a|y - a \rangle \geq \| x - a \|^{2} ,
$$
所以$\| x - a \| = d$，最后$a = p_{\mathbf{H}}(x)$是从证明的第一个部分得出的。 Q.E.D.

下文中$\mathbf{H}$中E的映射$p_{\mathbf{H}}$将被称为从E到$\mathbf{H}$的*投影*。我们注意到，$p_{\mathbf{H}}(x) = x$适用于所有$x \in \mathbf{H}$。

第一个部分。 1 在空间 E（V，p. 67，练习 31）的更一般假设下有效。

第证明。 1 除其他外，还建立了以下性质 ：

#### 推论 1 {#evt-v-s1-thm-1-cor-1 .statement tag=07XR}

*令I为由过滤器$\mathfrak{F}$引导的集合，并令$(y_{i})_{i \in I}$为$\mathbf{H}$的点族。让$x \in \mathbf{E}$。假设我们有*
$$
\lim_{i, \mathfrak{F}} \| x - y_{i} \| = \inf_{z \in \mathbf{H}} \| x - z \| .
$$
*然后相对于过滤器$\mathfrak{F}$，$y_{i}$趋向于$p_{\mathbf{H}}(x)$。*

#### 推论 2 {#evt-v-s1-thm-1-cor-2 .statement tag=07XS}

*对于$\mathbf{E}$中的每个$x, y$，我们有*
$$
\| p_{\mathbf{H}}(x) - p_{\mathbf{H}}(y) \| \leq \| x - y \| .
$$
*特别是，映射$p_{\mathbf{H}}$从$\mathbf{E}$到$\mathbf{H}$是连续的。*

令$x, y$为$\mathbf{E}$的两个点。把$a = p_{\mathbf{H}}(x) - x, b = p_{\mathbf{H}}(y) - p_{\mathbf{H}}(x), c = y - p_{\mathbf{H}}(y)$。到公式 (15) (V, p. 10) 我们有 $\mathscr{R} \langle a|b \rangle \geq 0$ 和 $\mathscr{R} \langle c|b \rangle \geq 0$。我们还有 $a + b + c = y - x$，它给出，
$$
\| x - y \|^{2} = \| a + b + c \|^{2} = \| b \|^{2} + \| a + c \|^{2} + 2 \mathscr{R} \langle a|b \rangle + 2 \mathscr{R} \langle c|b \rangle
$$
$$
\geq \| b \|^{2} = \| p_{\mathbf{H}}(x) - p_{\mathbf{H}}(y) \|^{2} .
$$
这就证明了推论2。

#### 命题 6 {#evt-v-s1-prop-6 .statement tag=07XT}

*令$\mathbf{E}$为前希尔伯特空间，并令$\Phi$为非空Hausdorff的非空有向递减集合和$\mathbf{E}$的完全凸子集。对于$\mathbf{E}$的每个$x \in \mathbf{E}$和每个子集$\mathbf{H}$，放入$d(x, \mathbf{H}) = \inf_{z \in \mathbf{H}} \| x - z \|$。在阶中，集合H属于到$\Phi$的交M非空，E中存在$x_0$使得$\sup_{H \in \Phi} d(x_0, H)$有限是充分必要的。对于每 $x \in E$ 我们有
$$
p_M(x) = \lim_{H \in \Phi} p_H(x)
$$
（极限相对于有向集合$\Phi$）。

如果 M 非空，则 $d(x, H) \leq d(x, M)$ 对于所有 $H \in \Phi$ 和所有 $x \in E$。

相反，假设E中存在点$x_0$和实数$C \geq 0$，使得$d(x_0, H) \leq C$对于所有$H \in \Phi$。 设 $x \in E$；那么
$$
d(x, H) \leq \|x - x_0\| + C \quad \text{for all } H \in \Phi,
$$
因此数 $d = \sup_{H \in \Phi} d(x, H)$ 是有限的。 令 B 为所有 $z \in E$ 中的集合，使得 $\|x - z\| \leq d$。 由于 B 是凸的并且在 E 中是闭的，因此集合 $H \cap B$，对于范围超过 $\Phi$ 的 H，是凸的、豪斯多夫且完备的。 设 $\varepsilon > 0$；存在集合$H \in \Phi$使得$d(x, H) \geq d - \varepsilon$，并且如果$\varepsilon < d/2$，则$H \cap B$的直径由prop以$\sqrt{12 \varepsilon (d - \varepsilon)}$为界。 5（V，p. 9）。 在其他字中，对于所有$H_0 \in \Phi$，对于$H \in \Phi$和$H \subset H_0$，封闭的集合$H \cap B$，对于豪斯多夫上的柯西滤波器的形式基以及完整的空间$H_0$。 因而，集合$H \cap B$（对于$H \in \Phi$）约化到点y的交。 我们得到$y \in M$和$\|x - y\| = d = d(x, M)$。 由于 M 在 $H_0$ 中是闭集，因此它是 E 中凸且完备的 Hausdorff 集合，因而 $y = p_M(x)$。 对于每个$H \in \Phi$，我们有$p_H(x) \in H \cap B$，从中我们得到$p_M(x) = \lim_{H \in \Phi} p_H(x)$。

#### 命题 7 {#evt-v-s1-prop-7 .statement tag=07XU}

*设 E 为 Hausdorff prehilbertian 空间，并令 $\Psi$ 为 E 的非空、凸、完备子集的非空有向递增集合。放置 $A = \bigcup_{H \in \Psi} H$ 并假设 A 的闭包 N 是完备的。那么 N 是凸的，我们有*
$$
p_N(x) = \lim_{H \in \Psi} p_H(x) \text{ for all } x \in E.
$$

很明显，A 是凸的，因此它的闭包 N 是凸的（II，p. 13）。具有记号的支撑。 6、$d(x, N) = \inf_{H \in \Psi} d(x, H)$，因此相对于$\Psi$的截面滤波器，$d(x, N)$是$d(x, H)$的极限。从 $p_H(x) \in H$ 开始
$$
\lim_{H \in \Psi} \|x - p_H(x)\| = \lim_{H \in \Psi} d(x, H) = d(x, N),
$$
它来自cor。相对于$\Psi$的截面过滤器，$p_H(x)$倾向于$x$的投影$p_N(x)$到N上的V、p. 11的1。

### 6. 向量子空间和正投影仪

令 E 为前希尔伯特空间。回想一下，如果 $\langle x | y \rangle = 0$，则 E 的两个向量 $x$ 和 $y$ 被称为“正交”；然后
$$
\|x + y\|^2 = \|x\|^2 + \|y\|^2
$$
（《毕达哥拉斯》定理»）。

设A为E的子集。如果E中的向量x与A的每个向量正交，则我们说E中的向量x与A正交。与A正交的所有向量中的集合是A的闭向量子空间，记为$A^\circ$并称为（由滥用语言）A 的正交。

设A和B是E的两个子集。如果A的每个向量与B的每个向量正交，我们说A和B是正交的。这相当于$A \subset B^\circ$或$B \subset A^\circ$的说。如果 E 是豪斯多夫且 A 和 B 正交，则 $A \cap B$ 为空或约化为 0，因为 0 是 E 中唯一与其自身正交的向量。

#### 定理 2 {#evt-v-s1-thm-2 .statement tag=07XV}

*设 E 为 E 的前希尔伯特空间和 M 向量子空间，这是 Hausdorff 且完备的。那么 E 是 M 和与 M 正交的 $M^\circ$ 子空间的拓扑直和。从 E 到 M 与分解 $E = M \oplus M^\circ$ 关联的投影算子是 th 中定义的从 E 到 M 的投影 $p_M$。 1（V，p. 10）。

我们首先证明对于所有$x \in E$，$x - p_M(x)$属于到$M^\circ$。让$y \in M$。对于每个标量 $\lambda \in K$、向量 $p_M(x) + \lambda y$ 属于到 M；因而，到公式 15 (V, p. 10) 我们有，

$$
\mathscr{R}(\lambda \langle x - p_M(x)|y \rangle) \leq 0
$$

对于所有$\lambda \in K$。如果，特别是我们取$\lambda = \overline{\langle x - p_M(x)|y \rangle}$，我们就结论，$\langle x - p_M(x)|y \rangle = 0$，因此我们的断言。

由于 M 是 Hausdorff，所以 0 是 M 的唯一向量，与其自身正交，因此是 $M \cap M^\circ = \{0\}$。对于每个$x \in E$，我们有$p_M(x) \in M$和$x - p_M(x) \in M^\circ$。因而，E 是 M 和 $M^\circ$ 的直和，$p_M$ 是从 E 到 M 的投影算子，其中核 $M^\circ$。由于$p_M$是从E到M的连续映射（V，p. 11，cor.2），如果从GT得出III, § 6, No. 2，则E是M和$M^\circ$的拓扑直和。

#### 推论 {#evt-v-s1-n6-cor-1 .statement tag=07XW}

*设 E 为豪斯多夫预希尔伯特空间，M 为 E 的有限维向量子空间。则 E 为 M 和 $M^\circ$ 的直和。

由于E是豪斯多夫，所以M也是豪斯多夫；由于 M 是有限维的，因此它是完备的 (I, p. 13)。因而，应用 th 就足够了。 2.

与第记号。 2，我们说$M^\circ$是M的正交补集，$p_M$是从E到M的正交投影（或正交投影算子，或者滥用语言，投影算子）；如果x是E的向量，M的向量$p_M(x)$也称为x在M上的正交投影。注意$p_M$是从E到M的连续线性映射，并且我们有$\|p_M\| = 1$。 V、p. 11 中的 2 个，但$M = \{0\}$ 的情况除外，在这种情况下$p_M = 0$。

直接从毕达哥拉斯定理可以看出，如果将 E (II, p. 4) 的商半范数赋予 $E/M$，则从直接和分解 $E = M \oplus M^\circ$ 推导出来的从 $E/M$ 到 $M^\circ$ 的规范映射 $\psi$ 是等距的。 我们总是将前希尔伯特结构分配给$E/M$，其中$\psi$是前希尔伯特空间的同构；然后从这个前希尔伯特结构推导出 $E/M$ 的商半范数。

当E是希尔伯特空间且M是E的闭向量子空间时，我们经常会使用前面的结果。在这种情况下，$M^\circ$是E的闭向量子空间，以及$p_{M^\circ} = 1 - p_M$和$(M^\circ)^\circ = M$。

#### 命题 8 {#evt-v-s1-prop-8 .statement tag=07XX}

— 令 E 为希尔伯特空间，M 为 E 的闭向量子空间，I 为非空有序有向集合，$(M_i)_{i \in I}$ E 的闭向量子空间系列。我们假设映射 $i \mapsto M_i$是递增，M是$\bigcup_{i \in I} M_i$的闭包，或者映射$i \mapsto M_i$是递减，并且$M = \bigcap_{i \in I} M_i$。然后对所有 $x \in E$ 进行$p_M(x) = \lim_{i \in I} p_{M_i}(x)$。

提案 8 紧随提案之后。 6（V，p. 11）和 7（V，p. 12）。

#### 命题 9 {#evt-v-s1-prop-9 .statement tag=07XY}

— 令 E 为希尔伯特空间，M、N 为 E 的两个闭向量子空间。

a) 以下条件是等效的：
(i) $p_M p_N = p_N p_M$；
(ii) 如果 $x \in M$ 与 $M \cap N$ 正交，且 $y \in N$ 与 $M \cap N$ 正交，则 x 和 y 正交；
(iii) 与$M \cap N$正交的M的每个向量都与N正交；
（四）$M = (M \cap N) + (M \cap N^\circ)$。

b) 如果满足a)的等价条件，我们有$p_{M \cap N} = p_M p_N$，向量子空间$M + N$，E是封闭的，我们有$p_{M+N} = p_M + p_N - p_M p_N$。

c) 当且仅当 M 与 N 正交时，我们才有 $p_M p_N = 0$。如果是这样，则 E 的向量子空间 $M + N$ 是闭集，并且$p_{M+N} = p_M + p_N$。

输入 $L = M \cap N$、$M_1 = M \cap L^\circ$ 和 $N_1 = N \cap L^\circ$。 条件 (ii) 意味着$M_1$ 和$N_1$ 是正交的，并且(iii) 意味着$M_1$ 和N 是正交的。由于我们有$N = N_1 + L$并且$M_1$与L正交，我们已经证明了(ii)和(iii)的等价。如果条件 (iii) 满足，我们就有$M_1 = M \cap N^\circ$，并且由于$M = L + M_1$，条件 (iv) 也满足。相反，从(iv)我们结论得知$M_1 = M \cap N^\circ$，因为M的子空间$M \cap N$和$M \cap N^\circ$是正交的，所以$M_1 \subset N^\circ$，即关系(iii)。

假设满足条件(iv)。对于所有 $y \in M$ 来说，直接的是 $p_N(y) = p_L(y)$，因此对于所有 $x \in E$ 来说，$p_N p_M(x) = p_L p_M(x)$。但是，对于每个 $x \in E$、向量 $p_L p_M(x)$ 属于到 L 和向量
$$
x - p_L p_M(x) = (x - p_M(x)) + (p_M(x) - p_L(p_M(x)))
$$
属于至 $M^\circ + L^\circ = L^\circ$；因此我们有 $p_L p_M(x) = p_L(x)$。最后$p_N p_M = p_L p_M = p_L$。由于条件 (ii) 等价于 (iv) 并且在 M 和 N 上对称，因此我们也有 $p_M p_N = p_L$。最后我们得到$p_M p_N = p_N p_M = p_{M \cap N}$，给出(i)。

相反，假设满足条件(i)。让$x \in M$；我们有
$$
p_M(p_N(x)) = p_N(p_M(x)) = p_N(x)
$$
所以$p_N(x) \in M$。我们结论$x - p_N(x) \in M$，因此$x$是$M \cap N$的元素$p_N(x)$的和和$M \cap N^\circ$的元素$x - p_N(x)$，得到(iv)。

我们已经证明了a)和b)的第一个部分。现在假设$p_M$和$p_N$通勤并放入$q = p_M + p_N - p_M p_N$；由于 $p_M$ 和 $p_N$ 在代数 $\mathscr{L}(E)$ 中是幂等的，因此 q 也是幂等的；因此 q 的 (GT, III, § 6, No. 2) 像是 E 的闭向量子空间。

显然，$q$的像包含在$M + N$中；然而，我们有 $p_N(x) = x$，因此对于所有 $x \in N$ 都有 $q(x) = x$；因为我们还有 $q = p_M + p_N - p_N p_M$，所以对于所有 $x \in M$，我们得到 $q(x) = x$。我们结论认为$q$的像等于$M + N$。 $M + N$的正交等于$M^\circ \cap N^\circ$，$q$的核显然是包含$M^\circ \cap N^\circ$，因此$q = p_{M+N}$。这证明了b)。

我们有$p_M p_N = 0$当且仅当$p_N$的像$N$包含在$p_M$的核$M^\circ$中，也就是说，当且仅当$M$与$N$正交。 断言 c) 的其余部分就是 b) 的特例。

#### 注 {#evt-v-s1-n6-rem-1 .statement tag=07XZ}

— 令 $E$ 为希尔伯特空间和$M, N$ $E$ 的两个闭向量子空间。 关系 $M \subset N$ 等价于 $M$ 和 $N^\circ$ 的正交性，即通过 prop 与关系 $p_M p_{N^\circ} = 0$ 正交。 9、c)。因为我们有 $p_{N^\circ} = 1 - p_N$，所以结论 *关系* $M \subset N$ *和* $p_M = p_M p_N$ *是等价的*（《三个垂直线定理》，*cf.* 图 3）。

![图表显示子空间 M、N 和投影 p_M(x)、p_N(x)](https://i.imgur.com/3Q5z5QG.png)

图 3.

### 7. 希尔伯特的对偶空间

#### 定理 3 {#evt-v-s1-thm-3 .statement tag=07Y0}

*令 $E$ 为希尔伯特空间。对于每个$x \in E$，令$x^*$为$E$上的连续线性形式$y \mapsto \langle x | y \rangle$； 映射 $x \mapsto x^*$ 是一个双射半线性（对于自同构 $\xi \mapsto \bar{\xi}$）映射，从 $E$ 到其对偶 $E'$，以及从赋范空间 $E$ 到赋范的等距空间$E'$.*

映射 $x \mapsto x^*$ 通过 (2) (V, p. 1) 是半线性的，并且凭借柯西-施瓦茨不等式，我们有 $\|x^*\| = \sup_{\|y\| \leq 1} |\langle x | y \rangle| = \|x\|$，因此 $x \mapsto x^*$ 是从 $E$ 到 $E'$ 的等距，特别是单射。为了完成证明，我们需要证明对于$E'$中的所有$x' \neq 0$，存在$x \in E$使得$x' = x^*$。但超平面$H = \mathrm{Ker}\, x'$于$E$关闭；它的正交线是线$D$。令$b$为$D$的非零元素； 线性形式$b^*$的核等于$H$，因此存在标量$\lambda \neq 0$使得$x' = \lambda \cdot b^* = (\overline{\lambda} \cdot b)^*$。 Q.E.D.

映射$x \mapsto x^*$从$E$到其对偶$E'$据说是*规范*。从 $E'$ 到 $E$ 的逆映射也称为正则，用 $x' \mapsto {x'}^*$ 表示。我们有

$$
\langle x | y \rangle = \langle y, x^* \rangle, \quad \langle x, x' \rangle = \langle {x'}^* | x \rangle
$$

对于$E$中的$x, y$和$E'$中的$x'$。还有$(x^*)^* = x$换$x \in E$。

当K为$\mathbf{R}$时，映射$x \mapsto x^*$是线性的。我们将通过这个映射将E的标量乘积转移到E'。当$K = \mathbf{C}$时，我们可以将映射$x \mapsto x^*$视为同构，从E的向量空间$\overline{E}$、共轭到E'（V、p. 6）。我们将通过这个映射将$\overline{E}$的标量乘积转移到E'。

在考虑的两种情况下，E' 是希尔伯特空间，我们有公式

$$
\langle x^*|y^* \rangle = \overline{\langle x|y \rangle}, \quad \langle x'|x' \rangle = \|x'\|^2
$$

对于 E 中的 $x, y$ 和 E' 中的 $x'$。

说向量$x \in E$与向量$y \in E$正交，相当于说，线性形式$x^* \in E'$在II、p. 41中定义的意义上与$y$正交（这证明在这两种情况下使用字 « 正交 » 是合理的）。如果 M 是 E 的闭向量子空间，则 E' 中与 M 正交的子空间 $M^\circ$ (II, p. 44) 是 E 中 M 正交的 $x \mapsto x^*$ 下的像，定义为V、p. 13（这证明在这两种情况下使用记号$M^\circ$是合理的）。

#### 推论 1 {#evt-v-s1-thm-3-cor-1 .statement tag=07Y1}

*在阶中，希尔伯特空间E的点的家庭$(x_i)_{i \in I}$是完整的，关系$\langle x_i|y \rangle = 0$对于$y \in E$和所有指标$i \in I$来说是充分必要的$y = 0$.*

事实上，这表示 0 是 E' 中唯一与所有 $x_i$（II、p. 43 和 IV、p. 1）正交的向量。

#### 推论 2 {#evt-v-s1-thm-3-cor-2 .statement tag=07Y2}

*令 E 和 F 为两个希尔伯特空间。对于 $u \in \mathscr{L}(E; F)$、$x \in E$ 和 $y \in F$，输入*

$$
\Phi_u(y, x) = \langle y|u(x) \rangle .
$$

*映射$u \mapsto \Phi_u$是同构从Banach空间$\mathscr{L}(E; F)$到空间所有连续倍半线性$^1$形式在$F \times E$上，赋予范数*

$$
\|f\| = \sup_{\substack{x \in E, y \in F \\ \|x\| \leq 1, \|y\| \leq 1}} |f(y, x)| .
$$

很明显，对于所有$u \in \mathscr{L}(E; F)$，$\Phi_u$ 是倍半线性且连续的。相反，令 $f$ 为 $F \times E$ 上的连续倍半线性形式。对于每个 $x \in E$，映射 $y \mapsto f(y, x)$ 是希尔伯特空间 F 上的连续线性形式。 3、对于每个$x \in E$，F中都存在唯一元素$u(x)$，使得$f(y, x) = \langle u(x)|y \rangle$对于所有$y \in F$。从 E 到 F 的映射 $u : x \mapsto u(x)$ 是线性的，我们有

$$
\begin{align*}
\|f\| &= \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |f(y, x)| = \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |\langle y|u(x) \rangle| \\
&= \sup_{\|x\| \leq 1} \|u(x)\| ;
\end{align*}
$$

因此$u$属于到$\mathscr{L}(E; F)$、$f = \Phi_u$和$\|u\| = \|f\|$。这证明了cor。 2.

$^1$ 回想一下（A，IX, § 1, No. 5），$F \times E$上的倍半线性形式（左侧）$f$是从$F \times E$到K的映射，满足V的关系（1）和（2）， p. 1。

典范映射从E到其双数E''（IV，p. 14）映射E到E''，在其他字（IV，p. 16）中，E是自反Banach空间。事实上，如果 E 是实数（或复数）希尔伯特空间，则从 E' 到 E 的典范映射 φ 是从范数空间 E' 到 E 的同构（或到 E 的共轭空间 $\overline{E}$）； 应用th。从 3 到 E（分别为 E），我们看到范数空间 E' 上的每个连续线性形式都是形式 $x' \mapsto \langle \phi(x')|x \rangle = \langle x, x' \rangle$ 和 $x \in E$，因此我们的断言如下。

作为推论（IV，p. 17，第 6 条）：

#### 定理 4 {#evt-v-s1-thm-4 .statement tag=07Y3}

*在希尔伯特空间 E 中，单位球是弱紧致的。*

#### 命题 10 {#evt-v-s1-prop-10 .statement tag=07Y4}

*如果在希尔伯空间 E 中，滤波器 $\mathfrak{F}$ 弱收敛到 $x_0$，而且如果$\lim_{\mathfrak{F}} \|x\| = \|x_0\|$，则对于 E 的初始拓扑，$\mathfrak{F}$ 收敛到 $x_0$。*

事实上，$\|x - x_0\|^2 = \|x\|^2 - 2\Re \langle x|x_0 \rangle + \|x_0\|^2$。由于$\langle x|x_0 \rangle$相对于$\mathfrak{F}$趋向于$\|x_0\|^2$假设，并且$\|x\|$相对于$\mathfrak{F}$趋于$\|x_0\|$，$\|x - x_0\|$相对于$\mathfrak{F}$趋于0，因此命题。

#### 注 {#evt-v-s1-n7-rem-1 .statement tag=07Y5}

— 如果 E 是 Hausdorff prehilbertian 空间且$\hat{E}$ E 的希尔伯特空间补全，我们知道 (III, p. 16) E 的对偶 E' 可以与 $\hat{E}$ 的对偶识别；然后从 th 得出。 3 (V, p. 15) E 上的每个连续线性形式都可以以独特的方式写为 $x \mapsto \langle a|x \rangle$，其中 $a \in \hat{E}$。

### 习题 {#evt-v-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
