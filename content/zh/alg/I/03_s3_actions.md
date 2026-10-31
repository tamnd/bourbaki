---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 3
section_title: Actions
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 24-29, 129-132
pdf_pages: 0048-0053, 0153-0156
extraction: ocr
subsections:
    - "no": 1
      title: ACTIONS
      page: 24
      pdf_page: 48
    - "no": 2
      title: SUBSETS STABLE UNDER AN ACTION. INDUCED ACTION
      page: 26
      pdf_page: 50
    - "no": 3
      title: QUOTIENT ACTION
      page: 26
      pdf_page: 50
    - "no": 4
      title: DISTRIBUTIVITY
      page: 27
      pdf_page: 51
    - "no": 5
      title: DISTRIBUTIVITY OF ONE INTERNAL LAW WITH RESPECT TO ANOTHER
      page: 29
      pdf_page: 53
statements: 14
exercises: 10
content_sha256: db487de2f3a584ed67375d2cb44db5800ad1a6358d10221851447a23c6c93159
translated_from: content/en/alg/I/03_s3_actions.md
translation_method: google
source_content_sha256: 7e8fbe4c81b4a012c8fdf0810f23488766fe66b340393425e3d9b307319fe67d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 5cc4d21303bb3640435f5f4a877080e9a2256ca792981d8f02aba9e30e3e2465
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。 作用

### 1.作用

#### 定义 1 {#alg-i-s3-def-1 .statement tag=057T}

*令$\Omega$和E为两个集合。将$\Omega$的映射放入集合，将E的映射$E^E$放入自身，称为E上的$\Omega$作用。*

令 $\alpha \mapsto f_\alpha$ 为 E 上 $\Omega$ 的作用。映射 $(\alpha, x) \mapsto f_\alpha(x)$（分别为 $(x, \alpha) \mapsto f_\alpha(x)$）被称为左*（分别为*右*）的 *律 *作用为 E*† 上的 $\Omega$ *与给定关联E* 上的作用共 $\Omega$。给定 E 中 $\Omega \times E$（或 $E \times \Omega$）的映射 $g$，E 上存在且仅有一个 $\Omega$ 的作用 $\alpha \mapsto f_\alpha$，使得左（或右）作用的关联律为$g$（*集合理论*、II, § 5, no. 2、命题3）。

在这个章中，为了缩写，我们应该说“律 of 作用”

† 或 E 上合成* 的有时 *外法则，其中 $\Omega$ 作为集合操作。

而不是“左律作用”。 E 的元素$f_\alpha(x)$（对于$\alpha \in \Omega$和$x \in E$）有时称为$\alpha$下$x$的*变换*或$\alpha$和$x$的*合成*。通常用左（或右）乘法记号$\alpha . x$（或$x . \alpha$）表示，点可以省略； $\alpha$和$x$的合成则称为$\alpha$和$x$的*乘积*（分别为$x$和$\alpha$）。还使用指数记号 $x^\alpha$。在下面各段的论证中，我们一般使用记号$\alpha \perp x$。 元素或 $\Omega$ 通常被称为*运算符*。

#### 例 {#alg-i-s3-n1-exa-1 .statement tag=057U}

(1) 令 E 为乘法写成的结合岩浆。与 E 的严格正整数 $n$ 映射 $x \mapsto x^n$ 关联到自身的映射是 E 上 $\mathbf{N}^*$ 的作用。 如果 E 是群，则与有理数关联的映射 E 的整数 $a$ 映射 $x \mapsto x^a$ 到 E 上等于 E 上的 $\mathbf{Z}$ 作用。

(2) 令E为律的岩浆，用$\top$表示。与 E 的子集集合的 $x \in E$ 映射 $A \mapsto x \top A$ 关联到自身的映射是 $\mathscr{P}(E)$ 上的 E 的作用。

(3) 设E为集合。 E 上$E^E$ 的恒等映射是$E^E$ 的作用，称为*规范的作用*。 作用的相应的律等于$E^E \times E$的映射$(f, x) \mapsto f(x)$到E中。

(4) 设$(\Omega_i)_{i \in I}$为集合的一个家庭。对于所有$i \in I$，令$f_i : \Omega_i \to E^E$为E上$\Omega_i$的作用。令$\Omega$为$\Omega_i$的和（*集合理论*，II, § 4, no. 8）。将$\Omega$的映射$f$延伸到$E^E$，延伸$f_i$，就是E上$\Omega$的作用。这使我们能够将约化对作用的家庭的研究转化为对单个家庭的研究作用。

(5) 给定E上$\Omega$的作用，$\perp$表示律，$\Omega$的子集$\Xi$和E的子集X，$\Xi \perp X$表示E的集合 $\alpha \perp x$ 与 $\alpha \in \Xi$ 和 $x \in X$；当$\Xi$由单个元素$\alpha$组成时，我们通常写$\alpha \perp X$而不是$\{\alpha\} \perp X$。与 $\alpha \in \Omega$ 映射 $X \mapsto \alpha \perp X$ 关联的映射是$\mathscr{P}(E)$上$\Omega$的作用，据说它是从给定的作用通过扩张到集合*导出的子集。

(6) 设$\alpha \mapsto f_\alpha$为E上$\Omega$的作用。设g为$\Omega$中$\Omega'$的映射。那么映射$\beta \mapsto f_{g(\beta)}$就是E上$\Omega'$的作用。

(7) 设$f : E \times E \to E$为集合E上合成的律。映射$\gamma : x \mapsto \gamma_x$（分别$\delta : x \mapsto \delta_x$）（§ 2, no. 2），与元素$x \in E$左（右）翻译相关联$x$ 是 E 对自身的作用；它被称为 E 的*左*（或*右*）*作用*，它本身*源自*给定的律。当$f$可交换时，这两个作用重合。

左（右）作用与$\gamma$相关的律是$f$（分别是律与$f$相反）。右（或左）作用与$\delta$相关的律是$f$（分别是律与$f$相反）。

设E上的$\Omega, E, F$为集合，$\alpha \mapsto f_\alpha$作用为$\Omega$，F上的$\Omega$为$\alpha \mapsto g_\alpha$作用。 E 到 F* 的 $\Omega$-*态射，或 E 到 F 的 *映射与 $\Omega$* 的作用兼容，是 E 到 F 的映射 $h$，使得

$$
g_\alpha(h(x)) = h(f_\alpha(x))
$$

对于所有$\alpha \in \Omega$和$x \in E$。两个$\Omega$态射中的合成是一个$\Omega$态射。

设$\Omega, \Xi, E, F$为集合，$E$上$\Omega$的$\alpha \mapsto f_\alpha$作用，$F$上$\Xi$的$\beta \mapsto g_\beta$作用和$\phi$映射 $\Omega$ 变成$\Omega'$。 $E$到$F$的$\phi$态射是$E$到$F$的映射$h$，使得
$$
g_{\phi(\alpha)}(h(x)) = h(f_\alpha(x))
$$
对于所有 $\alpha \in \Omega$ 和 $x \in E$。

### 2. 子集在作用下稳定。诱导作用

#### 定义 2 {#alg-i-s3-def-2 .statement tag=057V}

*如果$f_\alpha(A) \subset A$对于所有$\alpha \in \Omega$来说，集合$E$的子集$A$在$E$上$\Omega$的作用$\alpha \mapsto f_\alpha$下被称为稳定。如果$f_\alpha(x) = x$，则$E$的元素$x$在$\Omega$的元素$\alpha$下称为不变式。*

$E$的稳定子集族的交在给定作用下是稳定的。因此，对于给定的子集 $X$ $E$，存在$E$ 包含的最小的稳定子集；据说它是由$X$“生成”的；它由元素 $(f_{\alpha_1} \circ f_{\alpha_2} \circ \cdots \circ f_{\alpha_n})(x)$ 组成，其中 $x \in X, n \geq 0, \alpha_i \in \Omega$ 代表所有 $i$。

#### 注 {#alg-i-s3-n2-rem-1 .statement tag=057W}

令$E$为岩浆，律记为$\tau$。需要注意的是，$E$的子集$A$在$E$的左侧作用下稳定，在$E$的右作用下不一定稳定； $E$的子集$A$在左（或右）下稳定，$E$的作用本身在$E$上的律下稳定，但逆命题一般情况下并不正确。更准确地说，当且仅当$A \tau A \subset A$时，$A$在$E$上的律下稳定，而当且仅当$E \tau A \subset A$（或$A \tau E \subset A$）时，$A$在左（或右）作用在$E$上稳定。

#### 例 {#alg-i-s3-n2-exa-1 .statement tag=057X}

取岩浆$E$为集合$\mathbf{N}$和乘法。 集合$\{1\}$在$\mathbf{N}$的内部律下是稳定的，而$\{1\}$自身生成的$\mathbf{N}$的作用下稳定的子集是$\mathbf{N}$的整体。

#### 定义 3 {#alg-i-s3-def-3 .statement tag=057Y}

*令$\alpha \mapsto f_\alpha$为$E$上$\Omega$的作用，并且$A$为$E$的稳定子集。与 $f_\alpha$ 至 $A$ 的元素 $\alpha \in \Omega$ 限制相关联的映射（视为 $A$ 的映射自身）是 $A$ 上的 $\Omega$ 的作用，据说是由给定的作用.*

### 3.商作用

#### 定义 4 {#alg-i-s3-def-4 .statement tag=057Z}

*令$\alpha \mapsto f_\alpha$为集合$E$上集合$\Omega$的作用。 $E$上的等价关系$R$据说与给定的作用兼容，如果对于$E$的所有元素$x$和$y$，使得$x \equiv y \pmod{R}$和所有$\alpha \in \Omega, f_\alpha(x) \equiv f_\alpha(y) \pmod{R}$。 映射与 $E/R$ 的元素 $\alpha \in \Omega$ 映射相关联，由 $f_\alpha$ 通过经过得到的商是 $\Omega$ 在 $E/R$ 上的作用，称为 的商$E$ $\Omega$ 作用。*

令$E$为岩浆，$R$等价关系为$E$。 $R$ 据说是*左*（分别是。 *右*) *相容的* 与 $E$ 上的律如果它与左兼容（分别为。

右）E 本身的作用源自E上的律。为了使R与E上的律兼容，它与E上的律左右兼容是必要且充分的。

我们将§ 1, no. 6的命题 6、7和8的类似物留给读者叙述和证明。

### 4.分配律

#### 定义 5 {#alg-i-s3-def-5 .statement tag=0580}

设 $E_1, \ldots, E_n$ 和 F 为集合，并将 $E_1 \times \cdots \times E_n$ 的 u 映射代入 F。设 $i \in \{1, n\}$。假设 $E_i$ 和 F 被赋予结构岩浆。如果部分映射则表示 u 相对于指标变量 i 具有分布性

$$
x_i \mapsto u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n)
$$

对于$E_j$和$j \neq i$中所有固定的$a_j$，$E_i$的同态进入F。

如果 $\top$ 表示 $E_i$ 和 F 上的内部律，则 u 的分配律由以下方程给出

(1) $$
u(a_1, \ldots, a_{i-1}, x_i \top x'_i, a_{i+1}, a_n) \\
= u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n) \top u(a_1, \ldots, a_{i-1}, x'_i, a_{i+1}, \ldots, a_n)
$$

对于$i = 1, 2, \ldots, n, a_1 \in E_1, \ldots, a_{i-1} \in E_{i-1}, x_i \in E_i, x'_i \in E_i, a_{i+1} \in E_{i+1}, \ldots, a_n \in E_n$。

#### 例 {#alg-i-s3-n4-exa-1 .statement tag=0581}

令 E 为乘法写成的幺半群（分别为群）。 $\mathbf{N} \times E$（或 $\mathbf{Z} \times E$）的映射 $(n, x) \mapsto x^n$ 进入 E，可通过方程 $x^{m+n} = x^m x^n$ 相对于第一个变量进行分配（加法与 $\mathbf{N}$ 上的律）。如果 E 是可交换的，则该映射对于第二个变量可通过方程 $(xy)^n = x^n y^n$ 进行分配。

#### 命题 1 {#alg-i-s3-prop-1 .statement tag=0582}

令 $E_1, E_2, \ldots, E_n$ 和 F 为可加写的交换幺半群，并令 u 为 F 中 $E_1 \times \cdots \times E_n$ 的映射，它对所有变量都是可分配的。对于$i = 1, 2, \ldots, n$，令$L_i$为非空有限集合，且$(x_{i,\lambda})_{\lambda \in L_i}$为$E_i$的元素族。让 $y_i = \sum_{\lambda \in L_i} x_{i,\lambda}$ 代表 $i = 1, 2, \ldots, n$。然后

(2) $$
u(y_1, \ldots, y_n) = \sum_\alpha u(x_1, \alpha_1, \ldots, x_n, \alpha_n)
$$

和被接管所有序列 $\alpha = (\alpha_1, \ldots, \alpha_n)$ 属于至 $L_1 \times \cdots \times L_n$。

我们通过归纳对n进行论证，案例$n = 1$源自§ 1, no. 2的公式(2)。来自同一参考文献

(3) $$
u(y_1, \ldots, y_{n-1}, y_n) = \sum_{\alpha_n \in L_n} u(y_1, \ldots, y_{n-1}, x_n, \alpha_n)
$$

对于$y_n = \sum_{\alpha_n \in L_n} x_{n,\alpha_n}$和映射$z \mapsto u(y_1, \ldots, y_{n-1}, z)$的$E_n$进入$F$是岩浆同态。将归纳假设应用于从 $E_1 \times \cdots \times E_{n-1}$ 到 $F$ 的分配律映射 $(z_1, \ldots, z_{n-1}) \mapsto u(z_1, \ldots, z_{n-1}, x_n, \alpha_n)$，

(4)
$$
u(y_1, \ldots, y_{n-1}, x_n, \alpha_n) = \sum_{\alpha_1, \ldots, \alpha_{n-1}} u(x_1, \alpha_1, \ldots, x_{n-1}, \alpha_{n-1}, x_n, \alpha_n),
$$
和被接管序列 $(\alpha_1, \ldots, \alpha_{n-1})$ 属于至$M = L_1 \times \cdots \times L_{n-1}$。现在$L_1 \times \cdots \times L_n = M \times L_n$；写作
$$
t_{\alpha_1, \ldots, \alpha_n} = u(x_1, \alpha_1, \ldots, x_n, \alpha_n),
$$
我们有
(5)
$$
\sum_{\alpha_1, \ldots, \alpha_n} t_{\alpha_1, \ldots, \alpha_n} = \sum_{\alpha_n} \left( \sum_{\alpha_1, \ldots, \alpha_{n-1}} t_{\alpha_1, \ldots, \alpha_{n-1}, \alpha_n} \right)
$$
由公式 (7) 共 § 1, no. 5。 (2) 紧接着(3)、(4) 和(5)。

#### 注 {#alg-i-s3-n4-rem-1 .statement tag=0583}

如果$u(a_1, \ldots, a_{i-1}, 0, a_{i+1}, \ldots, a_n) = 0$适用于$i = 1, 2, \ldots, n$和$a_j \in E_j$（$j \neq i$），则公式（2）对于有限支撑的家庭$(x_i, \lambda)_{\lambda \in L_i}$仍然成立。

定义 5 的一个特例是，$u$ 是作用的律，与岩浆 $E$ 上的集合 $\Omega$ 的作用相关联。如果$u$相对于第二个变量是可分配的，则也可以说$\Omega$在岩浆$E$上的作用是可分配的。其他字：

#### 定义 6 {#alg-i-s3-def-6 .statement tag=0584}

*作用* $\alpha \mapsto f_\alpha$ *属于集合* $\Omega$ *在岩浆上* $E$ *如果对于所有* $\alpha \in \Omega$，*映射* $f_\alpha$ *是岩浆的自同态，则称其具有分配性$E$。

如果$\top$表示岩浆$E$的律，并且作用的$\perp$律与$E$上$\Omega$的作用相关，则后者的分配律表示为公式
(6)
$$
\alpha \perp (x \top y) = (\alpha \perp x) \top (\alpha \perp y) \quad \text{(for } \alpha \in \Omega \text{ and } x, y \in E\text{)}.
$$

通过滥用语言，还可以说律 $\perp$ 相对于律 $\top$ 是可分配的（或右分配的）。

§ 1, no. 2的公式(2)表明，对于$E$的元素的每一个有序的序列$(x_\lambda)_{\lambda \in L}$和每一个$\alpha \in \Omega$，
(7)
$$
\alpha \perp \left( \bigwedge_{\lambda \in L} x_\lambda \right) = \bigwedge_{\lambda \in L} (\alpha \perp x_\lambda).
$$

如果作用 $\alpha \mapsto f_\alpha$ 具有分配性，且 $E$ 上的等价关系 $R$ 与 $E$ 的合成和作用 $\alpha \mapsto f_\alpha$ 的律兼容，则作用的商$E/R$ 是可分配的。

当$E$上的律写成乘法时，我们经常使用作用的律的指数记号$x^\alpha$，它相对于这个乘法是可分配的，因此分配律可以用恒等式$(xy)^\alpha = x^\alpha y^\alpha$来表示。如果E上的律是相加的，我们经常使用左（或右）乘法记号$\alpha . x$（或$x . \alpha$）来表示作用的律，这是关于由恒等式表示的加法，分配律的分配性

$$
\alpha(x + y) = \alpha x + \alpha y \quad (\text{resp. } (x + y)\alpha = x\alpha + y\alpha).
$$

我们还可以考虑$\Omega$有一个内部律，记为$\overline{T}$，作用的律相对于第一个变量是可分配的，这意味着

(8)
$$
(\alpha \overline{T} \beta) \perp x = (\alpha \perp x) T (\beta \perp x)
$$
对于所有 $\alpha, \beta \in \Omega$ 和 $x \in E$。然后，通过§ 1, no. 2的公式(2)

(9)
$$
\left( \overline{T}_{\lambda \in L} \alpha_{\lambda} \right) \perp x = \overline{T}_{\lambda \in L} (\alpha_{\lambda} \perp x)
$$
对于每个订购的序列 $(\alpha_{\lambda})_{\lambda \in L}$ 元素 $\Omega$ 以及所有 $x \in E$。

### 5. 一个内部律的分配律相对于另一个

#### 定义 7 {#alg-i-s3-def-7 .statement tag=0585}

设$T$和$\perp$是集合E上的两个内部律。律$\perp$被认为关于律$T$是可分配的如果

(10)
$$
x \perp (y T z) = (x \perp y) T (x \perp z)
$$
(11)
$$
(x T y) \perp z = (x \perp z) T (y \perp z)
$$
对于 E 中的所有 $x, y, z$。

注如果律 $\perp$ 是可交换的，则 (10) 和 (11) 是等价的。一般来说，律其中一个写为加法，另一个写为乘法；如果乘法对于加法是可分配的，则：

(12)
$$
x . (y + z) = x . y + x . z
$$
(13)
$$
(x + y) . z = x . z + y . z
$$

#### 例 {#alg-i-s3-n5-exa-1 .statement tag=0586}

(1) 在集合 E 的子集的集合 $\mathscr{P}(E)$ 中，内部律 $\cap$ 和 $\cup$ 各自相对于自身和对方具有分配性。这是从形式的公式得出的

$$
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$
$$
A \cup (B \cap C) = (A \cup B) \cap (A \cup C).
$$

(2) 在$\mathbf{Z}$（更一般地，在任何全序集）中，律sup 和 inf 相对于另一个和相对于自身都是可分配的。

(3) In $\mathbf{Z}$(*and more generally in any 环*) 乘法 is distributive with respect to 加法.

(4) 在$\mathbf{N}$中，加法和乘法对于律sup和inf是可分配的。

### 习题{#alg-i-s3-exercises}

§ 3](exercises/s3/)参见[习题。
