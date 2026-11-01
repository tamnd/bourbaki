---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 1
section_title: Definition of Lie algebras
lang: zh
source: lie-i-iii
book_pages: 1-12, 73-83
pdf_pages: 0019-0030, 0091-0101
extraction: ocr
subsections:
    - "no": 1
      title: ALGEBRAS
      page: 1
      pdf_page: 19
    - "no": 2
      title: LIE ALGEBRAS
      page: 3
      pdf_page: 21
    - "no": 3
      title: COMMUTATIVE LIE ALGEBRAS
      page: 5
      pdf_page: 23
    - "no": 4
      title: IDEALS
      page: 5
      pdf_page: 23
    - "no": 5
      title: DERIVED SERIES, LOWER CENTRAL SERIES
      page: 6
      pdf_page: 24
    - "no": 6
      title: UPPER CENTRAL SERIES
      page: 6
      pdf_page: 24
    - "no": 7
      title: EXTENSIONS
      page: 7
      pdf_page: 25
    - "no": 8
      title: SEMI-DIRECT PRODUCTS
      page: 8
      pdf_page: 26
    - "no": 9
      title: CHANGE OF BASE RING
      page: 11
      pdf_page: 29
statements: 20
exercises: 27
content_sha256: 236ba0fd04e241df39f4197dd45170ea01d0dbe912d665cd2cf484dd5644c7cf
translated_from: content/en/lie/I/01_s1_definition_of_lie_algebras.md
translation_method: google
source_content_sha256: 58f1eb6f89ce2afeeacfc62b6731300e79cd58a2c1821a7f29f1c6e2d9168f15
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: af68a7621dd62b37a7cf06729399e84d6b2acc62a8b0c221c3d04dbd7bba2a2b
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。 定义李代数

### 1.代数

设 M 是 K 上的酉模，其中 $M \times M$ 的双线性映射 $(x, y) \mapsto xy$ 进入 M。代数的所有公理均满足，除了乘法的结合性之外。通过滥用语言，M 被称为不一定与 K 相关的代数，或有时，当不会产生混淆时，称为代数在 K 上。我们将使用后者记号。

如果给定K-模 M，则得到乘法 $(x, y) \mapsto yx$ 代数，称为上述代数的相反。

M 的子 K 模 N 在乘法下稳定，在 K 上以明显的方式给出代数的结构。 N 称为 M 的子代数。如果条件 $x \in N, y \in M$ 蕴含 $yx \in N$（或 $xy \in N$），则 N 称为 M 的左（或右）理想。如果 N 既是 M 的左理想又是右理想，N 称为 M 的双边理想。在这种情况下，M 上的乘法使我们能够在经过上对商进行定义，在商模 $M/N$ 上进行双线性乘法，使得 $M/N$ 有代数结构。 $M/N$ 称为 M 除以 N 的商代数。

† 在章中证明的命题仅依赖于书I至VI中建立的性质以及交换代数、章III, § 2的某些结果。

令$M_1$和$M_2$是$M_1$的$K$和$\phi$映射到$M_2$的两个代数。如果 $\phi$ 是 $K$ 线性的，$\phi$ 被称为 *同态*，并且 $\phi(xy) = \phi(x)\phi(y)$ 是 $x \in M_1, y \in M_1$。 $\phi$的核$N$是$M_1$的双面理想，$\phi$的像是$M_2$的子代数。在经过上对代数 $M_1/N$ 进行$\phi$ 定义同构的商到代数 $\phi(M_1)$。

令 $M$ 为代数超过 $K$。 $M$的映射$D$进入$M$，如果它是$K$线性，则称为$M$的*推导*，对于所有$x \in M$和$y \in M$，称为$D(xy) = (Dx)y + x(Dy)$。这个定义概括了*代数*、章IV, § 4, no. 3中的定义 3。 $M$推导核是$M$子代数。如果$D_1$和$D_2$是$M$的推导，则$D_1D_2 - D_2D_1$是$M$的推导（cf. *代数*，章IV, § 4, no. 3， 命题5：这个命题的证明不使用代数的结合性）。

令$M_1$和$M_2$等于代数除以$K$。在乘积 $K$-模块 $M = M_1 \times M_2$ 上，我们通过编写定义乘法

$$
(x_1, x_2)(y_1, y_2) = (x_1y_1, x_2y_2),
$$

对于$M_1$中的所有$x_1, y_1$，$M_2$中的$x_2, y_2$。 这样定义的代数称为$M_1$和$M_2$的*乘积代数*。 映射 $x_1 \mapsto (x_1, 0)$（或$x_2 \mapsto (0, x_2)$）是$M_1$（或$M_2$）的同构到$M$的双面理想。 在这些下，同构、$M_1$和$M_2$被视为$M$的双面理想。 那么$K$-模$M$就是$M_1$和$M_2$的直和。 Conversely, let $M$ be an algebra over $K$ and $M_1, M_2$ two two-sided ideals of $M$ such that $M$ is the direct sum of $M_1$ and $M_2$. 然后$M_1M_2 \subset M_1 \cap M_2 = \{0\}$；那么，如果$x_1, y_1$属于到$M_1$并且$x_2, y_2$到$M_2$，那么$(x_1 + x_2)(y_1 + y_2) = x_1y_1 + x_2y_2$，这样$M$就被识别为乘积代数$M_1 \times M_2$。 $M_1$ 的每个左（或右、两侧）理想都是 $M$ 的左（或右、两侧）理想。 我们将在任意有限族代数的情况下制定类似结果的任务留给读者。

令$M$为代数超过$K$，并假设$K$模块$M$承认基$(a_\lambda)_{\lambda \in L}$。 $K$ 存在唯一的系统 $(\gamma_{\lambda \mu \nu})_{(\lambda, \mu, \nu) \in L \times L \times L}$ 元素，使得$a_\lambda a_\mu = \sum_v \gamma_{\lambda \mu v} a_v$ 对于$L$ 中的所有$\lambda, \mu$。 $\gamma_{\lambda \mu \nu}$ 被称为$M$ 的结构相对于基* $(a_\lambda)$ 的*常数。

设$M$为代数超过$K$，$K_0$交换环，其中单位元和$\rho$同态为$K_0$到$K$映射单位元到单位元。然后通过将$\alpha \in K_0, x \in M$写为$\alpha.x = \rho(\alpha).x$，$M$可以被认为是代数超过$K_0$。特别是当$K_0$是$K$包含单位元中的子环并且$\rho$被视为$K_0$的映射包含在$K$中时。

设$M$为代数超过$K$，$K_1$交换环，其中$K$的单位元和$\sigma$同态进入$K_1$映射单位元到单位元。令 $M_{(K_1, \sigma)} = M_{(K_1)}$ 为从 $M$ 派生的 $K_1$ 模块，通过将标量的环扩展到 $K_1$ (*代数*, 章 II, § 5)。 $M$ 定义上的乘积典型地将 $M_{(K_1)} \times M_{(K_1)}$ 的 $K_1$ 双线性映射转换为 $M_{(K_1)}$ (*代数*, 章 IX, § 1, no. 4)，使得给出 $M_{(K_1)}$ 代数的结构超过$K_1$（据说是*源自*$M$*通过将标量的环扩展到*$K_1$）。特别是当$K$是$K_1$包含单位元的子环以及$\sigma$将$K$的映射包含到$K_1$时。

### 2.李代数

#### 定义 1 {#lie-i-s1-def-1 .statement tag=09TJ}

*如果乘法（用$(x, y) \mapsto [x, y]$表示）满足以下恒等式，则 K 上的代数 g 称为 K 上的李代数：*

(1) $$ [x, x] = 0 $$

(2) $$ [x, [y, z]] + [y, [z, x]] + [z, [x, y]] = 0 $$

*对于所有人* $x, y, z$ *以克为单位*。

乘积$[x, y]$称为$x$和$y$的*括号*。恒等式 (2) 称为*雅可比恒等式*。

括号$[x, y]$是$x$和$y$的交错的双线性函数。我们有身份：

(3) $$ [x, y] = -[y, x] $$

这样雅可比恒等式就可以写成：

(4) $$ [x, [y, z]] = [[x, y], z] + [y, [x, z]]. $$

每个子代数和李代数的每个代数商都是李代数。 李代数的每个乘积都是李代数。如果$g$是李代数，反代数$g^0$是李代数，并且根据恒等式(3)，$g$的映射$x \mapsto -x$同构到$g^0$。

#### 例 1 {#lie-i-s1-n2-exa-1 .statement tag=09TK}

设$L$是代数在$K$上的结合律。括号$[x, y] = xy - yx$是$x$和$y$的双线性函数。很容易验证，$K$-模块$L$上的合成$(x, y) \mapsto [x, y]$的律在$K$上使$L$变成李代数。

#### 例 2 {#lie-i-s1-n2-exa-2 .statement tag=09TL}

在例 1 选择 $L$ 中，是$K$-模 $E$ 的自同态的关联代数。我们得到*$E$的自同态的*李代数，记为$gl(E)$。 （如果$E = K^n$，则李代数$gl(E)$表示为$gl(n, K)$。）

$gl(E)$ 的每个谎言子代数都是李代数超过 $K$。特别是：
(1) 如果$E$在$K$上被赋予（不一定结合）代数结构、$E$形式李代数的推导。
(2) 如果$E$承认零的$E$的有限基、自同态，则在$K$上追踪形式李代数，用$sl(E)$表示（或$sl(n, K)$，如果$E = K^n$）。

#### 例 3 {#lie-i-s1-n2-exa-3 .statement tag=09TM}

阶 $n$ 方阵集合 $M_n(K)$ 可以认为是 K 上的李代数与 gl(n, K) 自然同构。令$(E_{ij})$为$\mathbf{M}_n(K)$的典范基（代数，章II, § 10, no. 3）。很容易得出：

$$
\begin{cases}
[E_{ij}, E_{kl}] = 0 & \text{if } j \neq k \text{ and } i \neq l \\
[E_{ij}, E_{jl}] = E_{il} & \text{if } i \neq l \\
[E_{ij}, E_{kt}] = -E_{kj} & \text{if } j \neq k \\
[E_{ij}, E_{ji}] = E_{ii} - E_{jj}
\end{cases}
$$

(5)

The Lie subalgebra of $\mathbf{M}_n(K)$ consisting of the triangular matrices (resp. triangular matrices of zero trace, resp. triangular matrices of zero diagonal) is denoted by $t(n, K)$ (resp. st(n, K), resp. n(n, K)) (Algebra, Chapter II, § 10; no. 7).

*例 3. 令V为无限可微实数流形。具有无限可微实系数的微分算子在 $\mathbf{R}$ 上构成结合律代数，因此，通过例 1，在 $\mathbf{R}$ 上构成李代数 $\Delta$。 V上的两个无限可微的向量域的括号是无限可微的向量域，因此V上的无限可微的向量域构成谎言子代数 $\mathfrak{f}$ / $\Delta$。如果V是实数*李群*，则左不变量向量域构成$\mathfrak{f}$的谎言子代数$g$，称为V的*李代数*。 向量空间 $g$ 与空间到 V 在 $e$ 处的切线（V 的单位元素）进行识别。令V'为另一个实李群，$e'$为单位元素，$g'$为李代数。将V的同态解析为V'定义线性映射，将$e$处空间到V的切线解析为空间到V'的切线$e'$；这个映射是李代数$g$到李代数$g'$的同态。如果V是有限维实数向量空间E的线性群，则存在$gl(E)$的典范同构到V的李代数$g$，其中$g$被识别为$gl(E)$。*

#### 定义 2 {#lie-i-s1-def-2 .statement tag=09TN}

*设 g 为 g 的李代数和 x 元素。 g 到 g 的线性映射 $y \mapsto [x, y]$ 称为 x 的伴随线性映射，用 $\operatorname{ad}_g x$ 或 $\operatorname{ad} x$ 表示。*

#### 命题 1 {#lie-i-s1-prop-1 .statement tag=09TO}

*设g为李代数。对于所有 $x \in g$，$\operatorname{ad} x$ 是推导。 映射$x \mapsto \operatorname{ad} x$是将李代数g同态转化为g的推导李代数$\mathfrak{d}$。如果$D \in \mathfrak{d}$和$x \in g$，则$[D, \operatorname{ad} x] = \operatorname{ad}(Dx)$。

恒等式(4)可以写成：

$$
(\operatorname{ad} x) \cdot [y, z] = [(\operatorname{ad} x) \cdot y, z] + [y, (\operatorname{ad} x) \cdot z]
$$

或者：

$$
(\operatorname{ad}[x, y]) \cdot z = (\operatorname{ad} x) \cdot ((\operatorname{ad} y) \cdot z) - (\operatorname{ad} y) \cdot ((\operatorname{ad} x) \cdot z)
$$

从而前两个断言。另一方面，如果$D \in \mathfrak{d}$，$x \in g$，$y \in g$，则$[D, \operatorname{ad} x] \cdot y = D([x, y]) - [x, Dy] = [Dx, y] = (\operatorname{ad} Dx) \cdot y$，从而最后一个断言。

映射$\operatorname{ad} x$也称为$x$定义的*内部推导*。

### 3.可交换李代数

#### 定义 3 {#lie-i-s1-def-3 .statement tag=09TP}

*如果 [x, y] = 0，则李代数的两个元素 x, y 被称为可交换的。如果元素中的任何两个是可交换的，则 g 被称为可交换的。*

#### 例 1 {#lie-i-s1-n3-exa-1 .statement tag=09TQ}

令 L 为结合律代数和由它定义的 g 李代数 (no. 2, 例 1)。当且仅当 L 中 xy = yx 时，两个元素 x, y 在 g 中可置换。

#### 例 2 {#lie-i-s1-n3-exa-2 .statement tag=09TR}

*如果实李群 G 是可交换的，那么它的李代数也是可交换的。*

显然，每个 K-模都可以在 K 上被赋予唯一的可交换性李代数结构。

如果 g 是李代数，则 g 的每个单生子模都是 g 的交换李子代数。

### 4.理想

由恒等式(3)得出，在李代数g中，左理想和右理想之间没有区别，每个理想都是双面的。因此，我们只谈论理想。

#### 例 {#lie-i-s1-n4-exa-1 .statement tag=09TS}

*设 G 为李群，g 为李代数，H 为 G 的谎言子群。H 定义上的每个左不变量向量域规范地是 G 上的左不变量向量域，从而有典范嵌入李代数 h 的 H 换算成 g； h 在这个单射下被 g 的谎言子代数识别。如果 H 在 G 中是正规的，则 g 中 h 的典范像是 g 的理想。*

g 的理想值是 g 的子模，它在 g 的内部推导下是稳定的。

#### 定义 4 {#lie-i-s1-def-4 .statement tag=09TT}

*在g的每个推导下稳定的g的子模称为g的特征理想。*

#### 命题 2 {#lie-i-s1-prop-2 .statement tag=09TU}

*设g为李代数，a是g的理想（分别是特征理想），b是a的特征理想。那么 b 是 g 的理想（或特征理想）。*

g 的每内部推导（或每推导）都会留下一个稳定，诱导会留在推导上，因此也会留下 b 稳定。

设g为李代数。如果a和b是g的理想，则a + b和a ∩ b是g的理想。

设a和b是g的两个子模。通过滥用记号，由形式的元素生成的g的子模[x, y] (x ∈ a, y ∈ b)被表示为[a, b]。根据恒等式 (3)，我们有 [a, b] = [b, a]。如果 z ∈ g、[z, a] 或 [a, z]，则表示子模 [Kz, a] = (ad z)(a)。

#### 命题 3 {#lie-i-s1-prop-3 .statement tag=09TV}

*如果 a 和 b 是 g 的理想（或特征理想），则 [a, b] 是 g 的理想（或特征理想）。*

令 D 为 g 的内部推导（分别为推导）。若$x \in a$且$y \in b$，则
$$
D([x, y]) = [Dx, y] + [x, Dy] \in [a, b].
$$
因此命题。

如果a是g的子模，$x \in g$的集合，使得$(\mathrm{ad}\ x).a \subset a$是g的子代数n，称为g中a的*归一化器*。若进一步a为g的子代数，则$a \subset n$且a为n的理想。

### 5.导出级数，下中央级数

特征理想 $[g, g]$ 称为李代数 g 的*派生理想*，并用 $\mathscr{D}g$ 表示。

g 包含 $\mathscr{D}g$ 的每个子模都是 g 的一个理想。

g 的*导出级数*是g 的特征理想的递减序列$\mathscr{D}^0g, \mathscr{D}^1g, \ldots$，归纳定义如下： (1) $\mathscr{D}^0g = g$； (2) $\mathscr{D}^{p+1}g = [\mathscr{D}^pg, \mathscr{D}^pg]$。

g的*下中心级数*是g的特征理想的递减序列$\mathscr{C}^1g, \mathscr{C}^2g, \ldots$，归纳定义如下： (1) $\mathscr{C}^1g = g$； (2) $\mathscr{C}^{p+1}g = [g, \mathscr{C}^pg]$。然后对于所有$p$，$\mathscr{C}^2g = \mathscr{D}g$和$\mathscr{C}^{p+1}g \supset \mathscr{D}^pg$，正如归纳在$p$上立即看到的那样。

#### 命题 4 {#lie-i-s1-prop-4 .statement tag=09TW}

*设g和h为K上的两个李代数，且g为h上的f同态。然后$f(\mathscr{D}^pg) = \mathscr{D}^pf, f(\mathscr{C}^pg) = \mathscr{C}^ph$.*

如果 a 和 b 是 g 的子模，则立即得出
$$
f([a, b]) = [f(a), f(b)].
$$
那么命题就是$p$ 上的直接的和归纳。

#### 推论{#lie-i-s1-n5-cor-1 .statement tag=09TX}

*设 g 为李代数且 g 的一个理想。为了使李代数$g/a$可交换，$a \supset \mathscr{D}g$是充分必要的。*

说 $g/a$ 是可交换的，相当于说 $\mathscr{D}(g/a) = \{0\}$。
但是$\mathscr{D}(g/a)$是$g/a$中$\mathscr{D}g$的典范像乘以命题4。

### 6.上中部级数

令 g 为 g 的李代数且 P 子集。 g 中 P 的*集中器*是 g 的元素的集合，它们可与 P 的那些可置换。该集中器是 ad $y$ 的核的交，其中 $y$ 穿过 P；因此它是g的子代数。

#### 命题 5 {#lie-i-s1-prop-5 .statement tag=09TY}

*设 g 为李代数且为 g 的理想（或特征理想）。 g 中 a 的扶正器 $a'$ 是 g 的理想（或特征理想）。*

令 D 为 g 的内部推导（分别为推导）。若$x \in a'$且$y \in a$，则
$$
[Dx, y] = D([x, y]) - [x, Dy] = 0;
$$
因此$Dx \in a'$。因此命题。

设$g$为李代数。 $g$中$g$的扶正器称为$g$的中心，这是$x \in g$的特征理想，使得$[x, y] = 0$适用于所有$y \in g$。 $g$的中心是同态$x \mapsto \mathrm{ad}\, x$的核。

$g$的上中心级数是$g$特征理想的递增序列$\mathscr{C}_0 g, \mathscr{C}_1 g, \ldots$，归纳定义如下： (1) $\mathscr{C}_0 g = \{0\}$； (2) $\mathscr{C}_{p+1} g$是$g$典范映射下的逆像到$g / \mathscr{C}_p g$中心$g / \mathscr{C}_p g$
理想的 $\mathscr{C}_1 g$ 是 $g$ 的中心。

### 7.扩张

#### 定义 5 {#lie-i-s1-def-5 .statement tag=09TZ}

设$a$和$b$是李代数除以$K$。 $b$除以$a$的扩张为序列：

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

其中$g$是$K$上的李代数，$g$的$\mu$满同态到$b$，以及$a$的$\lambda$单同态到$\mu$的核。

$\mu$的核$n$称为扩张的核。 The homomorphism $\lambda$ is an isomorphism of $a$ onto $n$ and the homomorphism $\mu$ defines an isomorphism of $g / n$ onto $b$ when passing to the quotient.
By an abuse of language, $g$ is also called an extension of $b$ by $a$.

两个扩张：

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b, \quad a \xrightarrow{\lambda'} g' \xrightarrow{\mu'} b
$$

are said to be equivalent if there exists a homomorphism $f$ of $g$ into $g'$ such that the following diagram:

$$
\begin{array}{ccccc}
a & \xrightarrow{\lambda} & g & \xrightarrow{\mu} & b \\
& & f \downarrow & & \\
& & g' & \xrightarrow{\mu'} & b \\
a & \xrightarrow{\lambda'} & g' & \xrightarrow{\mu'} & b
\end{array}
$$

是可交换的（即 $f \circ \lambda = \lambda', \mu' \circ f = \mu$）。我们证明这样的同态必然是双射的。首先 $f$ 是单射的。因为如果$x \in g$使得$f(x) = 0$，那么$\mu(x) = \mu'(f(x)) = 0$，因此对于某些$y \in a$来说$x = \lambda(y)$；然后$\lambda'(y) = f(\lambda(y)) = f(x) = 0$，因此$y = 0$，因此$x = 0$。另一方面，$f$是满射的。因为 $\mu' \circ f = \mu$ 是满射，因此 $f(g) + \lambda'(a) = g'$；另一方面$f(g) \supset f(\lambda(a)) = \lambda'(a)$。

由此可见，刚刚在$b$的两个扩张与$a$之间定义的关系是等价关系。

#### 命题 6 {#lie-i-s1-prop-6 .statement tag=09U0}

让

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

是$b$除以$a$的扩张，并且$n$是核。

(a) *如果g中存在g的子代数m对n的补充，则μ对m的限制就是m对b的同构。如果 ν 表示此限制的逆同构，则 ν 是 b 到 g 中的同态，μ ∘ ν 是 b 的恒等式自同构。*

(b) *相反，如果 g 中存在 b 的同态 ν 且 μ ∘ ν 是 b 的恒等式自同构，则 ν(b) 是 g 中 n 的补子代数。*

(a)中的断言是直接的。另一方面，令 ν 为 b 到 g 中的同态，使得 μ ∘ ν 为 b 的恒等式自同构。那么 ν(b) 是 g 的子代数，g 是 ν(b) 的直和和 $\mu^{-1}(0) = n$ (*代数*, 章 VIII, § 1, no. 1)。

#### 定义 6 {#lie-i-s1-def-6 .statement tag=09U1}

*让*

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*a 等于 b 的扩张，n 等于核。如果存在 g 的子代数（或理想）补充 g 中的 n，则此扩张称为无关紧要（或琐碎）。如果 n 包含在 g 的中心中，则该扩张称为中心。*

如果扩张是平凡的，则令 m 为 g 中 n 的补充的理想。那么 (cf. no. 1) g 被规范地等同于李代数 m × n，因此也等同于李代数 a × b。反之，设a和b为两个李代数；那么 a × b 是 a 乘 b 的平凡扩张。

一个无关紧要的中心扩张是微不足道的。令g为李代数，n是g的中心中包含的g的理想，g的m子代数补充g中的n。则 [m, g] = [m, m] + [m, n] = [m, m] ⊂ m，因此 m 是 g 的理想。

### 8.半直接乘积

设a和b是K上的两个李代数。用a来构造所有b的扩张并不容易。但我们将非常简单地用 a 来描述 b 的所有*非必要* 扩张。

设 g 是 b 与 a 的非必要扩张。我们认同 a 的理想为 g，b 为子代数 g 的补充，模 g 为模 a × b。对于所有$b \in b$，令$\phi_b$为限制到$\mathrm{ad}_g\ b$的a；这是a的推导和映射$b \mapsto \phi_b$是b的同态到a的推导的李代数。另一方面，对于 a 中的 $a, a'$ 和 b 中的 $b, b'$，我们有：

$$
[(a, b), (a', b')] = [a + b, a' + b']
= [a, a'] + [a, b'] + [b, a'] + [b, b']
= ([a, a'] + \phi_b a' - \phi_{b'} a, [b, b']).
$$

相反，设a和b在K上是李代数，并且b的$b \mapsto \phi_b$同态变成a的推导的李代数。在 K-模* a 和 b 的乘积 *g 上，我们通过写来定义两个元素的括号：

$$
[(a, b), (a', b')] = ([a, a'] + \phi_b a' - \phi_{b'} a, [b, b'])
$$

对于$a$中的所有$a, a'$，$b$中的$b, b'$。 It is immediate that this bracket is an alternating bilinear function of $(a, b), (a', b')$; we show that, given 3 elements $(a, b), (a', b'), (a'', b'')$ of $a \times b$:

(7)
$$
[(a, b), [(a', b'), (a'', b'')]] + [(a', b'), [(a'', b''), (a, b)]] \\
+ [(a'', b''), [(a, b), (a', b')]] = 0.
$$

由于(7)的左边是$(a, b), (a', b'), (a'', b'')$的交错的三线性函数，因此当元素的系统取以下形式之一时即可进行验证：

(8) $(a, 0), (a', 0), (a'', 0)$

(9) $(a, 0), (a', 0), (0, b'')$

(10) $(a, 0), (0, b'), (0, b'')$

(11)$(0, b), (0, b'), (0, b'')$。

在情况(8)和(11)中，关系(7)是$a$和$b$中雅可比恒等式的直接的推论。对于情况（9），我们有

$$
[(a, 0), [(a', 0), (0, b'')]] = [(a, 0), (-\phi_{b''}a', 0)] = (-[a, \phi_{b''}a'], 0)
$$
$$
[(a', 0), [(0, b''), (a, 0)]] = [(a', 0), (\phi_{b''}a, 0)] = ([a', \phi_{b''}a], 0)
$$
$$
[(0, b''), [(a, 0), (a', 0)]] = [(0, b''), ([a, a'], 0)] = (\phi_{b''}([a, a']), 0)
$$

关系 (7) 由等式得出：
$$
\phi_{b''}([a, a']) = [\phi_{b''}a, a'] + [a, \phi_{b''}a'].
$$

对于情况（10），我们有：

$$
[(a, 0), [(0, b'), (0, b'')]] = [(a, 0), (0, [b', b''])] = (-\phi_{[b', b'']}a, 0)
$$
$$
[(0, b'), [(0, b''), (a, 0)]] = [(0, b'), (\phi_{b''}a, 0)] = (\phi_{b'}\phi_{b''}a, 0)
$$
$$
[(0, b''), [(a, 0), (0, b')]] = [(0, b''), (-\phi_{b'}a, 0)] = (-\phi_{b''}\phi_{b'}a, 0)
$$

关系 (7) 由等式得出：
$$
\phi_{[b', b'']} = \phi_{b'}\phi_{b''} - \phi_{b''}\phi_{b'}.
$$

因此李代数结构已定义在$g$上。 $g$的映射$(a, b) \mapsto b$到$b$是同态$\mu$，其中核$n$是形式$(a, 0)$的$g$元素的理想。 映射 $a \mapsto (a, 0)$ 是$a$ 的同构 $\lambda$ 到$n$。因此：

(12)
$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

是$b$的扩张乘以核$n$的$a$，据说这是由$a, b, \phi$*规范定义的。 映射$b \mapsto (0, b)$是$b$的同构$\nu$到$g$的子代数，对$g$中$n$的补充；因此扩张是无关紧要的。

如果$a$在$\lambda$下与$n$识别，并且$b$在$v$下与$v(b)$识别，则对于$a \in a$和$b \in b$：

$$
(\mathrm{ad}\ b).a = [(0, b), (a, 0)] = (\phi_b a, 0) = \phi_b a.
$$

当$\phi = 0$时，$g$是$b$和$a$中的乘积李代数。一般情况下，$g$被$a$*称为$b$的*半直接乘积（$b$的相应的到同态$b \mapsto \phi_b$到推导的李代数） $a$）。

因此，我们建立了以下命题：

#### 命题 7 {#lie-i-s1-prop-7 .statement tag=09U2}

*设$a$和$b$是李代数除以$K$，*

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*$b$的扩张通过$a$，$b$的$\nu$同构到$g$的子代数，使得$\mu \circ \nu$是$b$的身份自同构并且将 $b$ $\phi$ 相应的同态化为 $a$ 推导李代数。* 让

$$
a \xrightarrow{\lambda_0} g_0 \xrightarrow{\mu_0} b
$$

*是$b$的非必要扩张，由$\phi$规范定义的$a$。*则映射$(a, b) \mapsto \lambda(a) + \nu(b)$是$g_0$的同构$f$到$g$和以下图表

$$
\begin{array}{ccccc}
& & \\
a & \xrightarrow{\lambda_0} & g_0 & \xrightarrow{\mu_0} & b \\
& \searrow f & \downarrow & \nearrow \mu_0 \\
& & g & & \\
& \swarrow i & & \searrow \mu \\
& & & &
\end{array}
$$

*是可交换的，因此两个扩张是等价的。*

#### 例 1 {#lie-i-s1-n8-exa-1 .statement tag=09U3}

令$g$为李代数除以$K$，并且$D$推导除以$g$。令 $h$ 为*可交换* 李代数 $K$。 映射$\lambda \mapsto \lambda D (\lambda \in K)$是将$h$同态转化为$g$推导李代数。我们通过$g$半直接$h$形式相应的半直接乘积$t$。令 $x_0$ 为 $t$ 的元素 $(0, 1)$。对于所有 $x \in g$、$Dx = [x_0, x]$。

#### 例 2 {#lie-i-s1-n8-exa-2 .statement tag=09U4}

令$g$是$K$上的李代数，$M$是$K$模，$\rho$同态是$g$的$\mathfrak{gl}(M)$。 如果将$M$视为可交换的李代数，则$M$的推导的李代数为$\mathfrak{gl}(M)$。 因此，我们可以将$g$的形式半直接乘积$h$乘以$M$相应的到$\rho$。

特别地，令$g = \mathfrak{gl}(M)$和$\rho$为$\mathfrak{gl}(M)$的恒等映射。 $M$对$g$的半直接乘积则表示为$\mathfrak{af}(M)$（如果$M = K^n$则表示为$\mathfrak{af}(n, K)$）。 $\mathfrak{af}(M)$的元素为有序对$(m, u)$，其中$m \in M, u \in \mathfrak{gl}(M)$；括号定义为

$$
[(m, u), (m', u')] = (u(m') - u'(m), [u, u']).
$$

*当 M 是有限维向量空间大于 $\mathbf{R}$ 时，$\mathfrak{af}(M)$ 规范地与 M 的 *仿射群* 的李代数等同。*

设$t$为K上的李代数。$t$入$\mathfrak{af}(M)$的线性映射$\theta$可以写成$x \mapsto ((\zeta(x), \eta(x)))$，其中$\zeta$是$t$入$M$和$\eta$的线性映射将$t$中的线性映射转化为$gl(M)$。我们检查条件，$\zeta$和$\eta$必须满足，$\theta$才能成为同态。对于$x \in t, y \in t$，我们必须有

$$
\theta([x, y]) = [\theta(x), \theta(y)]
$$

那就是

$$
(\zeta([x, y]), \eta([x, y])) = [(\zeta(x), \eta(x)), (\zeta(y), \eta(y))] \\
= (\eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x), [\eta(x), \eta(y)]).
$$

因此，要使$\theta$成为$t$的同态进入$\mathfrak{af}(M)$，$\eta$成为$t$的同态进入$gl(M)$以及$\zeta$满足是充分必要的关系：

(13)
$$
\zeta([x, y]) = \eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x).
$$

令 N 为 K-模 $M \times K$。我们取$t$为$w \in gl(N)$的$gl(N)$由……组成中的子代数，这样$w(N) \subset M$。对于所有$w \in t$，令$\eta(w) \in gl(M)$为$w$至$M$中的限制，并令$\zeta(w) = w(0, 1) \in M$。对于$w_1 \in t, w_2 \in t$，

$$
\zeta([w_1, w_2]) = w_1(\zeta(w_2)) - w_2(\zeta(w_1)) = \eta(w_1) \cdot \zeta(w_2) - \eta(w_2) \cdot \zeta(w_1).
$$

因此，映射 $w \mapsto (\zeta(w)), \eta(w))$ 是 $t$ 的同态 $\theta$ 到 $\mathfrak{af}(M)$。显然 $\theta$ 是*双射的*。让$\phi = \theta^{-1}$。如果 $(m, u) \in \mathfrak{af}(M)$，$\phi(m, u)$ 是 $t$ 的元素 $w$，定义为

$$
w(m', \lambda) = (u(m') + \lambda m, 0).
$$

$\mathfrak{af}(M)$经常与同构$\phi$下的$gl(N)$的子代数$t$等同。

*当 M 为 $\mathbf{R}$ 有限维向量空间时，将 $\mathfrak{af}(M)$ 的同态 $\phi$ 转化为 $gl(N)$ 对应至典范同态 $\psi$ 将 M 的仿射群 A 转化为群 $\mathbf{GL}(N)$；如果$a \in A, \psi(a)$是$\mathbf{GL}(N)$的唯一元素$g$，那么$g(m, 1) = (a(m), 1)$对于所有$m \in M$。这个同态是单射的，$\psi(A)$ 是 N 的自同构的集合，这使得 N 平行于 M 的所有线性簇保持不变。*

### 9.变换基环

令$K_0$为交换环，其中单位元和$K_0$的$\rho$同态转化为K映射单位元至单位元。令 $g$ 为 K 上的李代数。 令 $g'$ 为代数，通过 $\rho$ (cf. no. 1) 将 $g$ 视为 $K_0$ 上的代数。那么$g'$就是李代数。 $g$的子代数（分别是理想）是$g'$的子代数（分别是理想）。如果$a$和$b$是$g$的子模，则$[a, b]$在$g$和$g'$中是相同的； $[a, b]$ 是形式元素集合

$$
\sum_{i=1}^n [x_i, y_i]
$$

其中$x_i \in a, y_i \in b$。由此可见，对于所有$p$，$\mathscr{D}^p g = \mathscr{D}^p g', \mathscr{C}^p g = \mathscr{C}^p g'$。

子集的扶正器在$g$和$g'$中是相同的。因此，对于所有$p$，$\mathscr{C}_p g = \mathscr{C}_p g'$。

设$K_1$为交换环，其中$K$的单位元和$\sigma$同态变为$K_1$映射单位元至单位元。令 $g$ 为李代数超过 $K$。令 $g_{(K_1)}$ 为代数，超过 $K_1$，通过扩展基环 (cf. no. 1) 从 $g$ 派生。那么$g_{(K_1)}$就是李代数。如果$a$是$g$的子代数（或理想），则$g_{(K_1)}$中$a_{(K_1)}$的典范像是$g_{(K_1)}$的子代数（或理想）。如果$a$和$b$是$g$的子模，则$[a, b]_{(K_1)}$的$g_{(K_1)}$中的典范像等于$a_{(K_1)}$和$b_{(K_1)}$的典范像的括号。由此可见，$\mathscr{D}^p(g_{(K_1)})$是$(\mathscr{D}^p g)_{(K_1)}$的典范像，$\mathscr{C}^p(g_{(K_1)})$是$\mathscr{C}^p(g_{(K_1)})$的典范像。

如果$K$是域，$K$的$K_1$扩张域和$K$的$\sigma$典范嵌入进入$K_1$，那么通过通常的识别我们有
$$
[a, b]_{(K_1)} = [a_{(K_1)}, b_{(K_1)}], \quad \mathscr{D}^p(g_{(K_1)}) = (\mathscr{D}^p g)_{(K_1)},
$$
$$
\mathscr{C}^p(g_{(K_1)}) = (\mathscr{C}^p g)_{(K_1)}.
$$

这些结果在§ 2, no. 9完成。

如果 $M$ 是有限维向量空间超过域 $K$，$M_{(K_1)}$ 是有限维向量空间超过 $K_1$，并且结合词代数 $\mathscr{L}(M_{(K_1)})$ 与结合词代数被规范地识别$\mathscr{L}(M)_{(K_1)}$。因此李代数 $gl(M_{(K_1)})$ 被规范地识别为李代数 $gl(M)_{(K_1)}$。

### 习题 {#lie-i-s1-exercises}

§ 1](exercises/s1/)参见[习题。
