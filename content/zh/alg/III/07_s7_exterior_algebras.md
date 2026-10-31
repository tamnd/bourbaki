---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 7
section_title: Exterior algebras
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 507-522, 633-637
pdf_pages: 0531-0546, 0657-0661
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE EXTERIOR ALGEBRA OF A MODULE
      page: 507
      pdf_page: 531
    - "no": 2
      title: Functorial properties of the exterior algebra
      page: 508
      pdf_page: 532
    - "no": 3
      title: ANTICOMMUTATIVITY OF THE EXTERIOR ALGEBRA
      page: 510
      pdf_page: 534
    - "no": 4
      title: '*n*-th EXTERIOR POWER OF A MODULE AND ALTERNATING MULTILINEAR MAPPINGS'
      page: 511
      pdf_page: 535
    - "no": 5
      title: EXTENSION OF THE RING OF SCALARS
      page: 513
      pdf_page: 537
    - "no": 6
      title: DIRECT LIMITS OF EXTERIOR ALGEBRAS
      page: 514
      pdf_page: 538
    - "no": 7
      title: EXTERIOR ALGEBRA OF A DIRECT SUM. EXTERIOR ALGEBRA OF A GRADED MODULE
      page: 515
      pdf_page: 539
    - "no": 8
      title: EXTERIOR ALGEBRA OF A FREE MODULE
      page: 517
      pdf_page: 541
    - "no": 9
      title: CRITERIA FOR LINEAR INDEPENDENCE
      page: 519
      pdf_page: 543
statements: 31
exercises: 15
content_sha256: 624ccb97d206577c8f9e7780f1c5a44bbe86762771787463ef4a1354dae87b9c
translated_from: content/en/alg/III/07_s7_exterior_algebras.md
translation_method: google
source_content_sha256: 2ecded72dc27d27759b8e68470e35ec8930215e63753cc4598f26151e19c86fa
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 9c66253dbbe646a4afff61b956000e68687b868cc1a688d9b339bfdc9b431c5b
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 7。外观代数

### 1. 外部定义代数模

#### 定义 1 {#alg-iii-s7-def-1 .statement tag=062S}

设$A$为交换环，$M$为$A$模。 $M$的外代数，用$\bigwedge(M)$或$\mathrm{Alt}(M)$或$\bigwedge_A(M)$表示，是代数除以$A$张量代数$T(M)$与两侧理想$\mathfrak{J}''$的商（也用$\mathfrak{J}_{M}''$表示）由元素$x \otimes x$生成，其中$x$贯穿$M$。

由于理想$\mathfrak{J}''$是由次数2的齐次元素生成的，因此它是一个分级理想（II, § 11, no. 3，命题2）；我们写$\mathfrak{J}_n'' = \mathfrak{J}'' \cap T^n(M)$；因此，代数 $\bigwedge(M)$ 按 $\bigwedge^n(M) = T^n(M)/\mathfrak{J}_n''$ 的毕业（称为规范）由……组成进行评分。然后$\mathfrak{J}_0'' = \mathfrak{J}_1'' = \{0\}$，因此$\bigwedge^0(M)$与$A$识别，$\bigwedge^1(M)$与$T^1(M) = M$识别；接下来我们将始终进行这些识别，并且典范嵌入$M \to \bigwedge(M)$将由$\phi''$或$\phi_M''$表示。

#### 命题 1 {#alg-iii-s7-prop-1 .statement tag=062T}

令 $E$ 为 $A$ 代数，$f : M \to E$ 为 $A$ 线性映射，使得
$$
(f(x))^2 = 0 \quad \text{for all } x \in M.
$$
存在且仅有一个$A$-代数同态$g : \bigwedge(M) \to E$使得$f = g \circ \phi''$。

在其他字中，$(\bigwedge(M), \phi'')$是普遍映射问题的解（集合理论，IV, § 3, no. 1），其中$\Sigma$是$A$-代数结构的类， $\alpha$-映射是线性映射从$A$-模块$M$到$A$-代数满足 (1)。

$g$的唯一性源自$\phi''(M) = M$生成$\bigwedge(M)$。为了证明$g$的存在性，我们注由§ 5, no. 1，命题1存在$A$代数同态$g_1 : T(M) \to E$使得$f = g_1 \circ \phi$；我们需要证明$g_1$在理想的$\mathfrak{J}''$上是零，因为如果
$$
p : T(M) \to \bigwedge(M) = T(M)/\mathfrak{J}''
$$
是典范同态，我们可以写成$g_1 = g \circ p$，其中$g : \bigwedge(M) \to E$是代数同态，结论由$p \circ \phi = \phi''$得出。现在，$g_1$的核是一个双面理想，根据（1）和关系$g_1 \circ \phi = f$，包含元素$x \otimes x$对于$x \in M$。这样就完成了证明。

#### 注 {#alg-iii-s7-n1-rem-1 .statement tag=062U}

(1) 假设 E 是 $(E_n)$ 等级型 $\mathbf{Z}$ 的A-代数，并且还假设线性映射 $f$（假设满足 (1)）是这样的：
$$
f(M) \subset E_1.
$$
然后关系 $g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p)$ 与 $x_i \in M$ 表明 $g(\bigwedge^p(M)) \subset E_p$ 对于所有 $p \geq 0$，因此 $g$ 是分级的代数同态。

(2) 为了避免混淆，外部代数$\bigwedge(M)$的两个元素$u, v$中的乘积通常用$u \wedge v$表示，并用$v$称为$u$的*外部乘积*。因此，$\bigwedge^n(M)$ 的元素是形式 $x_1 \wedge x_2 \wedge \cdots \wedge x_n$ 的元素的和，$x_i \in M$ $1 \leq i \leq n$，通常称为*n 向量*。

### 2. 外部的函数性质代数

#### 命题 2 {#alg-iii-s7-prop-2 .statement tag=062V}

*令$A$为交换环、$M$和$N$两个$A$模块和$u : M \to N$一个$A$线性映射。存在且仅有一个$A$-代数同态*
$$
u'' : \bigwedge(M) \to \bigwedge(N)
$$
*这样图表*

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M'' & & \downarrow \phi_N'' \\
\bigwedge(M) & \xrightarrow{u''} & \bigwedge(N)
\end{array}
$$

* 是可交换的。此外，$u''$是分级的代数同态。*

$u'$的存在性和唯一性由no. 1、命题1适用于代数、$\bigwedge(N)$和$f = \phi_N'' \circ u : M \to \bigwedge(N)$；对于$f(M) \subset N$，因此$f$通过$\mathfrak{g}_N''$的定义满足条件（1）：与$f(M) \subset \bigwedge^1(N) = N$一样，$u''$是分级代数同态的事实来自*注* 1 no. 1。

命题 2 中的同态 $u''$ 今后将用$\bigwedge(u)$ 表示。如果 $P$ 是$A$-模且 $v : N \to P$ 是$A$-线性映射，则
$$
\bigwedge(v \circ u) = \bigwedge(v) \circ \bigwedge(u)
$$
对于 $\bigwedge(v) \circ \bigwedge(u)$ 是代数同态，它呈现可交换的图表

$$
\begin{array}{ccc}
M & \xrightarrow{v \quad u} & P \\
\downarrow \phi_M' & & \downarrow \phi_P' \\
\bigwedge(M) & \xrightarrow{\bigwedge(v) \circ \bigwedge(u)} & \bigwedge(P)
\end{array}
$$

由于$\Lambda(M)$包含$M = \Lambda^1(M)$，$\Lambda(u)$是有时，称为$u$到$\Lambda(M)$的规范扩张。 限制 $\Lambda^n(u): \Lambda^n(M) \to \Lambda^n(N)$ 是这样的
$$
\Lambda^n(u)(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n)
$$
与$x_i \in M$，因为$\Lambda(u)$是代数同态和$\Lambda^1(u) = u$； 限制$\Lambda^0(u)$到$A$是恒等映射。 注 $\Lambda^n(u)$ 是由 $T^n(u): T^n(M) \to T^n(N)$ 除以经过的商得到的。

#### 命题 3 {#alg-iii-s7-prop-3 .statement tag=062W}

*如果$u: M \to N$是满射$A$线性映射，则同态$\Lambda(u): \Lambda(M) \to \Lambda(N)$是满射，其核是$u$的核$P \subset M \subset \Lambda(M)$生成的$\Lambda(M)$的两侧理想。

证明是由§ 6, no. 2、命题 4、替换 $S$ 和$\Lambda$ 以及$\mathfrak{g}'$ 和$\mathfrak{g}''$ 衍生而来。

如果 $u: M \to N$ 是单射线性映射，则 $\Lambda(u)$ 并不总是单射映射 (§ 6, 习题 3)（但请参见下面的no. 9，命题 12 的推论）。然而，当$u$是单射时，$u(M)$是$N$的直因子，然后$\Lambda(u)$的像（与$\Lambda(M)$同构的）是$\Lambda(N)$的直因子； 证明与 $T(u)$ (§ 5, no. 2) 替换 $T$ by $\Lambda$ 的类似断言相同。

#### 命题 4 {#alg-iii-s7-prop-4 .statement tag=062X}

*令$N$和$P$为$A$模块$M$的两个子模，使得它们的和$N + P$是$M$中的直因子，并且它们的交$N \cap P$是直因子在$N$和$P$。那么同态$\Lambda(N) \to \Lambda(M)$、$\Lambda(P) \to \Lambda(M)$和$\Lambda(N \cap P) \to \Lambda(M)$、典范嵌入的典范扩张是单射的；如果通过这些同态将$\Lambda(N)$、$\Lambda(P)$和$\Lambda(N \cap P)$与$\Lambda(M)$的子代数进行识别，则*
$$
\Lambda(N \cap P) = \Lambda(N) \cap \Lambda(P).
$$
证明始终由 § 5, no. 2、命题 4 替换 $T$ 衍生自 $\Lambda$。当$A$为域时，$M$的任意子模$N, P$总是满足命题4的假设。

#### 推论{#alg-iii-s7-n2-cor-1 .statement tag=062Y}

*令$K$为交换域且$M$向量空间大于$K$。对于每个元素$z \in \Lambda(M)$，都存在$M$的最小的向量子空间$N$，使得$z \in \Lambda(N)$和$N$是有限维的。*

证明是从§ 5, no. 2推导出来的，推论到命题4替换$T$乘以$\Lambda$。

$N$称为$M$的向量子空间，与$\Lambda(M)$的元素$z$相关联。

### 3.外部的反交换性代数

#### 命题 5 {#alg-iii-s7-prop-5 .statement tag=062Z}

(i) 令$(x_i)_{1 \leq i \leq n}$为模$M$中的元素中的有限序列；对于对称群 $S_n$ 中的每个置换 $\sigma$，

$$
x_{\sigma(1)} \wedge x_{\sigma(2)} \wedge \cdots \wedge x_{\sigma(n)} = \varepsilon_\sigma \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

其中$\varepsilon_\sigma$表示置换$\sigma$的签名。

(ii) 如果存在两个不同的指标 $i, j$ 使得 $x_i = x_j$, 乘积

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

是零。

(i) 首先，由于 $x \wedge x = 0$ 对于所有 $x \in M$ 乘以理想 $\mathfrak{g}'$ 的定义，同样，对于 $M$ 中的 $x, y$，

$$
x \wedge y + y \wedge x = (x + y) \wedge (x + y) - x \wedge x - y \wedge y = 0.
$$

这在$n = 2$情况下成立(6)。一般情况由§ 4, no. 6、引理 3 得出。

(ii) 在(ii)的假设下，存在置换$\sigma \in S_n$使得$\sigma(1) = i$和$\sigma(2) = j$；那么对于这个置换，(6) 的左侧是零，因此右侧也是零。

#### 推论 1 {#alg-iii-s7-prop-5-cor-1 .statement tag=0630}

设$H, K$为$\mathbf{N}$的区间$[1, n]$的两个互补子集，并令$(i_h)_{1 \leq h \leq p}, (j_k)_{1 \leq k \leq n-p}$分别为$H$和$K$的元素的序列，排列在递增阶；我们写

$$
x_H = x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}, \quad x_K = x_{j_1} \wedge x_{j_2} \wedge \cdots \wedge x_{j_{n-p}};
$$

然后

$$
x_H \wedge x_K = (-1)^{\nu} x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

其中$\nu$是有序对$(i, j) \in H \times K$的数，使得$i > j$。

命题 5 约化至证明

#### 引理 1 {#alg-iii-s7-lem-1 .statement tag=0631}

如果$\sigma \in S_n$是置换，使得$\sigma(h) = i_h$对应$1 \leq h \leq p$，$\sigma(h) = j_{n-p}$对应$p + 1 \leq h \leq n$，则$\varepsilon_\sigma = (-1)^\nu$。

对于$1 \leq h < h' \leq p$或$p + 1 \leq h < h' \leq n$、$\sigma(h') > \sigma(h)$和数或有序对$(h, h')$，使得$1 \leq h \leq p < h' \leq n$和$\sigma(h) > \sigma(h')$等于$\nu$。

#### 推论 2 {#alg-iii-s7-lem-1-cor-2 .statement tag=0632}

代数 $\bigwedge(M)$ 的分级为交错的（$§ 4$、no. 9）。

$§ 4$、no. 9到$\bigwedge(M)$中的应用命题 13就足够了，取生成的系统集合$M$并使用命题5。

#### 命题 6 {#alg-iii-s7-prop-6 .statement tag=0633}

*如果M为有限生成A-模，则$\bigwedge(M)$为有限生成A-模；另外，如果 M 承认生成的系统且 n 元素，则 $\bigwedge^p(M) = \{0\}$ 对应 $p > n$。*

令$(x_i)_{1 \leq i \leq n}$为M的生成的系统。$\bigwedge^p(M)$的每元素为形式的元素线性组合
$$
x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}
$$
其中指标 $i_k$ 属于至 $\{1, n\}$；到命题 5，这些指标可以被认为是不同的（否则相应的元素是零）。如果$p > n$，则不存在指标这样的序列，因此不存在$\bigwedge^p(M) = \{0\}$。如果$p \leq n$，这些序列在数中是有限的，从而完成证明。

### 4. *n* 个外部幂模和交错的多线性映射

给定交换环 A 上的两个模 M, N，$M^n$ 到 N 的 *交错的 n-线性* 映射是任意 *n*-线性映射 $f : M^n \to N$，使得对于所有 $p \leq n - 2$，
$$
f(u_1, \ldots, u_p, x, x, v_1, \ldots, v_{n-p-2}) = 0
$$
对于所有 x，M 中的 $u_i$ ($1 \leq i \leq p$) 和 $v_j$ ($1 \leq j \leq n - p - 2$)。

#### 命题 7 {#alg-iii-s7-prop-7 .statement tag=0634}

*设A为交换环，M和N为A-模。如果与每个 A-线性映射 $g : \bigwedge^n(M) \to N$ ($n \geq 2$) 相关联，则 n 线性映射*
$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 \wedge x_2 \wedge \cdots \wedge x_n)
$$
*双射A-线性映射是从A-模$\operatorname{Hom}_A(\bigwedge^n(M), N)$到交错的的A-模获得$M^n$到N的n线性映射。*

我们考虑A-模$\operatorname{Hom}_A(T^n(M), N)$到A-模$\mathscr{L}_n(M, \ldots, M; N)$的规范双射到$M^n$到N的*所有*n线性映射，通过与每个A-线性映射$f : T^n(M) \to N$关联n线性映射获得
$$
\tilde{f} : (x_1, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n)
$$
（II, § 3, no. 9）。另一方面，A-线性映射 $g : \bigwedge^n(M) \to N$ 与 A-线性映射 $f : T^n(M) \to N$ 是一对一的对应，使得 *f 是 $\mathfrak{g}_n''$* 上的零，通过与 g 映射 $f = g \circ p_n$ 关联，其中
$$
p_n : T^n(M) \to \bigwedge^n(M) = T^n(M)/\mathfrak{g}_n''
$$

是典范同态 (II, § 2, no. 1, 定理 1)。但由于$\mathfrak{J}_n''$是形式元素线性组合
$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$
$M$中的$(x, u_i, v_j$），说$f$是形式$g \circ p_n$意味着相应的$n$-线性函数$\bar{f}$满足（8），在其他字中是*交错的*。

A-模 $\bigwedge^n(M)$ 被称为 M 的第 n 个外部幂*。对于每个 A-模同态 $u : M \to N$，映射
$$
\bigwedge^n(u) : \bigwedge^n(M) \to \bigwedge^n(N)
$$
其中重合与$\bigwedge^n(M)$上的$\bigwedge(u)$称为u*的第n个外部幂。

#### 推论 1 {#alg-iii-s7-prop-7-cor-1 .statement tag=0635}

*对于每个交错的 n 线性映射* $g : M^n \to N$，*对于每个置换* $\sigma \in \mathfrak{S}_n$，
$$
g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = \varepsilon_\sigma \cdot g(x_1, x_2, \ldots, x_n)
$$
*对于所有人*$x_i \in M$； *此外，如果* $x_i = x_j$ *对于两个不同的指标* $i, j$，*则*
$$
g(x_1, x_2, \ldots, x_n) = 0.
$$
这是命题 7 和no. 3、命题 5 的明显推论。

#### 推论 2 {#alg-iii-s7-prop-7-cor-2 .statement tag=0636}

*设* $(x_i)_{1 \leq i \leq n}$ *为 M 的 n 元素中的序列，使得*
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0;
$$
*然后，对于每个交错的 n 线性映射* $g : M^n \to N$，$g(x_1, \ldots, x_n) = 0$。

#### 推论 3 {#alg-iii-s7-prop-7-cor-3 .statement tag=0637}

*设* $f : M^{n-1} \to A$ *为交错的* $(n-1)$*-线性形式*。 *如果* $(x_i)_{1 \leq i \leq n}$ *是 M 的 n 元素中的序列，使得* $x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$，*则*
$$
\sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i = 0
$$
*（我们写* $f(x_1, \ldots, \hat{x}_i, \ldots, x_n) = f(x_1, \ldots, x_{i-1}, x_{i+1}, \ldots, x_n)$ *为* $1 \leq i \leq n$。

足以证明$n$-线性映射
$$
(x_1, \ldots, x_n) \mapsto \sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i
$$
$M^n$到$M$是*交错的*。现在，如果$x_i = x_{i+1}$，则右侧和中的所有项都有零系数，除了$x_i$和$x_{i+1}$之外，因为$f$是交错的；另一方面，$x_i$的系数为
$$
(-1)^i f(x_1, \ldots, x_{i-1}, x_{i+1}, x_{i+2}, \ldots, x_n)
$$

$x_{i+1}$ 是$(-1)^{i+1} f(x_1, \ldots, x_i, x_{i+2}, \ldots, x_n)$，它们是假设的倒数。

#### 注 {#alg-iii-s7-n4-rem-1 .statement tag=0638}

$T^n(M)$ 的元素 $z$ 被称为阶* $n$ 的（逆变）*斜对称张量，如果 $\sigma.z = \varepsilon_\sigma z$ 对于每个置换 $\sigma \in S_n$ (cf.) § 6, no. 3、注）；这些元素形式是$T^n(M)$的子A模块$A'_n(M)$。对于所有$z \in T^n(M)$，我们写成$a.z = \sum_{\sigma \in S_n} \varepsilon_\sigma(\sigma.z)$，并称$a.z$为$z$的*倾斜对称化*；作为$\varepsilon_{\sigma\tau} = \varepsilon_\sigma \varepsilon_\tau$，立即看出$a.z$是斜对称的张量，因此$z \mapsto a.z$是$T^n(M)$的自同态，其中像$A''_n(M)$包含在$A'_n(M)$中；一般来说$A''_n(M) \neq A'_n(M)$（习题8）。如果$z$是斜对称张量，则$a.z = n!z$；因此，*当* $n!$ *可逆于* $A$时，自同态 $z \mapsto (n!)^{-1}a.z$ 是 $T^n(M)$ 的 *投影算子*，其像为

$$
A'_n(M) = A''_n(M).
$$

而且这个投影算子的*核*正好是$\mathfrak{J}_n''$；因为注意显然可能仅限于$n \geqslant 2$的情况，因此2（$n!$的除子）在$A$和$x \otimes x = 2^{-1}(x \otimes x + x \otimes x)$中是可逆的；因此$\mathfrak{J}_n''$由元素$z + \rho.z$生成，其中$\rho$是$\{1, n\}$中两个连续数的转置；此外，对于$S_n$中的两个置换$\sigma, \tau$，我们可以写

$$
z - \varepsilon_{\sigma\tau}((\sigma\tau).z) = z - \varepsilon_\tau(\tau.z) + \varepsilon_\tau(\tau.z - \varepsilon_\sigma \sigma.(\tau.z))
$$

从而由此可见，$z - \varepsilon_\sigma(\sigma.z) \in \mathfrak{J}_n''$ 对于所有 $z \in T^n(M)$ 和 $\sigma \in S_n$。因此（始终假设$n!$在$A$中可逆），可以看出

$$
z - (n!)^{-1}a.z = \sum_{\sigma \in S_n} (n!)^{-1}(z - \varepsilon_\sigma(\sigma.z)) \in \mathfrak{J}_n''
$$

对于所有$z \in T^n(M)$，这建立了我们的断言。

当$n!$在$A$中可逆时，$T^n(M)$的子模、$A'_n(M)$和$\mathfrak{J}_n''$因此是*补充*并且典范同态$T^n(M) \to \bigwedge^n(M) = T^n(M)/\mathfrak{J}_n''$的限制到$A'_n(M)$是A-模 *同构*，这允许我们在所讨论的情况下将阶$n$的认同倾斜对称张量与$M$的第$n$外部幂的元素。 注这里还表明，该标识与两个斜对称张量的$T(M)$中的乘法、乘积不兼容，一般情况下不是斜对称的。

### 5. 标量的环中的扩张

令$A, A'$为两个交换环、$\rho : A \to A'$环同态、$M$一个$A$模、$M'$一个$A'$模以及$f : M \to M'$一个*A同态*（相对于$\rho$）的$M$变成$M'$。复合映射 $M \xrightarrow{f} M' \xrightarrow{\phi_{M'}} \bigwedge_{A'}(M')$ 是 $M$ 的 A-线性映射到 A-代数 $\bigwedge_{A'}(M')$，并且，由于 f(M) ⊂ M' 的元素是 $\bigwedge_{A'}(M')$ 中的零平方，因此存在(no. 1, 命题 1) 唯一一个 $A$-代数 $f'' : \bigwedge_A(M) \to \bigwedge_{A'}(M')$ 呈现可交换图表

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\downarrow \phi_M'' & & \downarrow \phi_{M'}'' \\
\bigwedge_A(M) & \xrightarrow{f''} & \bigwedge_{A'}(M')
\end{array}
$$

$f''$ 是分级的代数同态。立即推断出，如果$\sigma : A' \to A''$是另一个环同态，$M''$是$A''$模，$g : M' \to M''$是$A'$同态（相对于$\sigma$）和$g'' : \bigwedge_{A'}(M') \to \bigwedge_{A''}(M'')$ 相应的 $A''$-代数的同态，则复合$A$-代数的同态

$$
\bigwedge_A(M) \xrightarrow{f''} \bigwedge_{A'}(M') \xrightarrow{g''} \bigwedge_{A''}(M'')
$$

对应到复合$A$-同态$g \circ f : M \to M''$（相对于$\sigma \circ \rho$）。

#### 命题 8 {#alg-iii-s7-prop-8 .statement tag=0639}

*令$A, B$为两个交换环、$\rho : A \to B$环同态和$M$一个$A$模块。规范的扩张*

$$
\psi : \bigwedge_B(B \otimes_A M) \to B \otimes_A \bigwedge_A(M)
$$

*$B$-线性映射* $1_B \otimes \phi_M'' : B \otimes_A M \to B \otimes_A \bigwedge_A(M)$ *是分级的$B$-代数同构。*

证明是由 § 5, no. 4 衍生而来，命题 5 替换 $T$ 由 $\bigwedge$ 衍生而来，$\phi_M$ 由 $\phi_M''$ 衍生而来。

### 6. 外部直极限代数

令$(A_\alpha, \phi_{\beta \alpha})$为交换环、$(M_\alpha, f_{\beta \alpha})$直接系统的有向直接系统、$A_\alpha$模块、$A = \lim \to A_\alpha$和$M = \lim \to M_\alpha$。对于 $\alpha \leq \beta$，我们从 $A_\alpha$ 同态 $f_{\beta \alpha} : M_\alpha \to M_\beta$ 和 $A_\alpha$ 代数同态 (no. 5, 公式 (12)) $f_{\beta \alpha}' : \bigwedge_{A_\alpha}(M_\alpha) \to \bigwedge_{A_\beta}(M_\beta)$ 推导出来，并从 (13) 得出$(\bigwedge_{A_\alpha}(M_\alpha), f_{\beta \alpha}')$ 是 *直接系统已分级* $A_\alpha$*-模块*。另一方面，令 $f_\alpha : M_\alpha \to M$ 为规范的 $A_\alpha$ 同态；我们推导出 (no. 5, 公式 (12)) 分级$A_\alpha$-代数同态$f_\alpha'' : \bigwedge_{A_\alpha}(M_\alpha) \to \bigwedge_A(M)$，并且从 (13) 还可以得出，$f_\alpha''$ 构成$A_\alpha$-同态的直接系统。

#### 命题 9 {#alg-iii-s7-prop-9 .statement tag=063A}

*A-同态* $f'' = \varprojlim f''_\alpha : \varprojlim \Lambda_{A_\alpha}(M_\alpha) \to \Lambda_A(M)$ *是分级的代数同构*。

证明与 § 5, no. 4 相同，命题 6 替换在整个 T 中由 $\Lambda$ 和 $\phi$ 与 $\phi''$ 相同，并且考虑到交错的代数的直极限是交错的。

### 7. 外观代数直和。外观代数等级模

设A为A-模家庭的交换环、$M = \bigoplus_{\lambda \in L} M_\lambda$直和和$j_\lambda : M_\lambda \to M$典范嵌入；推导出分级代数 $\Lambda(j_\lambda) : \Lambda(M_\lambda) \to \Lambda(M)$ 的 A-同态。由于$\Lambda(M)$是反交换的，§ 4, no. 7的命题 10（或者如果需要推广到L无限的情况，cf.§ 4, no. 8，*Reamrk* 1）可以应用于同态$\Lambda(j_\lambda)$；那么存在唯一代数同态

$$
g : \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda) \to \Lambda(M)
$$

（也用 $g_M$ 表示）使得 $\Lambda(j_\lambda) = g \circ f_\lambda$，其中

$$
f_\lambda : \Lambda(M_\lambda) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)
$$

表示典范同态。

#### 命题 10 {#alg-iii-s7-prop-10 .statement tag=063B}

*典范同态* g (*公式 (14)*) *是分级的代数同构*。

为了证明 g 是双射的，我们定义分级代数同态

$$
h : \Lambda(M) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)
$$

这样$g \circ h$和$h \circ g$分别是$\Lambda(M)$和$\bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$上的恒等映射。对于每个$\lambda \in L$，考虑复合线性映射

$$
u_\lambda : M_\lambda \xrightarrow{\phi''_{M_\lambda}} \Lambda(M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda).
$$

存在且仅有一个A-线性映射$u : M \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$，使得$u \circ j_\lambda = u_\lambda$适用于所有$\lambda \in L$。偏斜张量积 $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$ 是 *交错的* 代数：对于 L 有限，这从 § 4, no. 9、命题 14 得出，对于 L 任意，这从给出的乘积的定义得出§ 4, no. 8、*注* 1 并且交错的中的直极限分级为代数为交错的。由于$u(M)$也包含在分级代数$\bigotimes_{\lambda \in L} \Lambda(M_\lambda)$中的次数1的元素的子模中，因此从no. 1、命题1和*注*1可以得出，存在唯一的评分代数同态。

$$
h : \Lambda(M) \to \bigotimes_{\lambda \in L} \Lambda(M_\lambda)
$$

这样$h \circ \phi''_M = u$。然后，如§ 6, no. 6、命题 9 替换$S$那样通过$\Lambda$和$\phi'$通过$\phi''$来验证$g \circ h$和$h \circ g$是恒等映射。

#### 注 {#alg-iii-s7-n7-rem-1 .statement tag=063C}

令$N = \bigoplus_{\lambda \in L} N_\lambda$为另一个系列$A$模块中的直和，并以$L$作为索引集合，并且对于所有$\lambda \in L$，令$v_\lambda : M_\lambda \to N_\lambda$为$A$线性映射， 从而存在$A$线性映射$v = \bigoplus_\lambda v_\lambda : M \to N$（II, § 1, no. 6，命题 7）。然后图表

$$
\begin{array}{ccc}
\bigotimes_{\lambda \in L} \Lambda(M_\lambda) & \xrightarrow{g_M} & \Lambda(M) \\
\downarrow & & \downarrow \\
\bigotimes_{\lambda \in L} \Lambda(v_\lambda) & & \Lambda(v) \\
\downarrow & & \downarrow \\
\bigotimes_{\lambda \in L} \Lambda(N_\lambda) & \xrightarrow{g_N} & \Lambda(N)
\end{array}
$$

是可交换的（cf. § 4, no. 5，命题 8 的推论）。

可以更精确地描述$\bigotimes_{\lambda \in L} \Lambda(M_\lambda)$的子$A$模块，通过同构$g$来识别$\Lambda^n(M)$。对于$L$的每个有限子集$J$，我们写$E_J = \bigotimes_{\lambda \in J} \Lambda(M_\lambda)$，因此$\bigotimes_{\lambda \in L} \Lambda(M_\lambda) = \lim \to E_J$相对于$L$的有限子集的有向集合$\mathscr{F}(L)$，通过定义（$§ 4$， no. 8，*注* 1)。对于每个家庭$\nu = (n_\lambda) \in \mathbf{N}^{(L)}$（因此具有*有限*支持），使得$\sum_{\lambda \in L} n_\lambda = n$和$L$包含中的每个有限子集$J$家庭$\nu$的支持，我们写

$$
\Lambda^{J,\nu}(M) = \bigotimes_{\lambda \in J} \Lambda^{n_\lambda}(M_\lambda)
$$

因此，$E_J$中次数$n$的元素的子模$E_{J,n}$是$J$中包含的所有家庭$\nu$支持的$\Lambda^{J,\nu}(M)$的*直和*，并且这样

$$
\sum_{\lambda \in L} n_\lambda = n
$$

（$§ 4$、no. 7、命题 10 和 no. 8）。按照惯例，我们为$J$中没有包含赡养费的家庭$\nu$写为$\Lambda^{J,\nu}(M) = \{0\}$；然后

E_{J,n}也可以称为所有$\bigwedge^{J,\nu}(M)$的直和，其中$\nu$贯穿所有$\nu = (n_\lambda)_{\lambda \in L}$族的集合$H_n$，从而$\sum_{\lambda \in L} n_\lambda = n$。由于$\bigwedge^0(M_\lambda)$与$A$相同，显然也适用于$L$中的两个有限子集$J \subset J'$以及$J$、典范映射$\bigwedge^{J,\nu}(M) \to \bigwedge^{J',\nu}(M)$（典范映射中的限制）的支持家庭$\nu$ $E_J \to E_{J'}$ 到 $\bigwedge^{J,\nu}(M)$) 是双射的。如果我们写，对于所有 $\nu \in H_n$，

$$
\bigwedge^\nu(M) = \lim_{\longrightarrow} \bigwedge^{J,\nu}(M)
$$

然后可以看出，考虑到II, § 6, no. 2，命题 5，我们有：

#### 推论{#alg-iii-s7-n7-cor-1 .statement tag=063D}

*The A-module $\bigwedge^n(M)$ is the image under isomorphism (14) of the submodule of* $\bigotimes_{\lambda \in L} \bigwedge(M_\lambda)$* *the direct sum of the submodules* $\bigwedge^\nu(M)$* *for all families* $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$* *such that* $\sum_{\lambda \in L} n_\lambda = n$; *如果* $J$* 是* $\nu$、$\bigwedge^\nu(M)$* *的支持，则与* $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_\lambda)$ 自然同构。

一般来说，$\bigwedge^n(M)$中的$\bigwedge^\nu(M)$、$\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_\lambda)$及其像都被识别。有了这个约定：

#### 命题 11 {#alg-iii-s7-prop-11 .statement tag=063E}

*令$\Delta$为可交换幺半群，$M$为型$\Delta$的分级A-模和*$(M_\alpha)_{\alpha \in \Delta}$**其毕业。对于子模* $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_{\alpha_\lambda})$的每个有序对* $(\alpha, n) \in \Delta \times \mathbf{N}$，*令* $\bigwedge^{\alpha,n}(M)$* *为* $\bigwedge^n(M)$* *直和的子模，*其中* $(n_\lambda)_{\lambda \in L}$* *穿过以下家庭的集合整数* $\geq 0$* *使得* $\sum_{\lambda \in L} n_\lambda = n$、$J$* *是它的支持，并且对于每个* $(n_\lambda)$、$(\alpha_\lambda)_{\lambda \in J}$* *贯穿* $\Delta^J$* *的家庭的集合使得* $\sum_{\lambda \in J} \alpha_\lambda = \alpha$。 *然后* $(\bigwedge^{\alpha,n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$* *是型* $\Delta \times \mathbf{N}$* *与* $\bigwedge(M)$* 上的代数结构兼容，并且诱导在* $M = \bigwedge^1(M)$* *给出了毕业。*

事实上，$\bigwedge(M)$ 是 $\bigwedge^{\alpha,n}(M)$ 的直和，这是从命题 10 的推论得出的； 证明的其余部分与§ 5, no. 5、命题7的证明结尾相同。

### 8. 外观代数自由模

#### 定理 1 {#alg-iii-s7-thm-1 .statement tag=063F}

*设* $M$* *为A-模和基* $(e_\lambda)_{\lambda \in L}$。 *让* $L$* *被给予全序集*的结构（集合理论，III, § 2, no. 3，定理 1）* *并且对于每个有限子集* $J$* *的* $L$* *我们写*

$$
e_J = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}
$$

其中$(\lambda_k)_{1 \leq k \leq n}$是J的元素排列在递增阶中的序列（集合理论，III, § 5, no. 3，命题6）；我们写A的$e_\varnothing = 1$，单位元。然后是$e_J$，其中J穿过L的有限子集的集合$\mathscr{F}(L)$，外部代数$\bigwedge(M)$的形式基。

由于$e_\lambda$生成A-模M，$\bigwedge(M)$的每个元素都是元素$e_\lambda$的乘积的有限数的线性组合，因此（考虑到no. 3, 命题 5) 是$J \in \mathscr{F}(L)$ 的元素 $e_J$ 的有限数的线性组合。 约化到证明，$e_J$对A是线性无关的。否则，这些元素之间会存在一个线性关系，其系数不全是零； 子集 J 的并，其中对应到关系中的系数为$\neq 0$的$e_J$是L的有限子集 K（因为只有有限的数系数$\neq 0$）。令 N 为由 $e_\lambda$ 生成的 M 的子模，使得 $\lambda \in K$； N 是 M 中的直因子，因此 (no. 2) $\bigwedge(N)$ 与 $\bigwedge(M)$ 的子代数等同，如果我们证明 $e_J$ 与$J \subset K$ 形式基 $\bigwedge(N)$，我们将得到想要的矛盾。

因此，当M的基有限时，约化提供定理1；因此我们可以假设$L = \{1, m\} \subset N$。对于每个$i \in L$，令$M_i$为M的自由子模$Ae_i$； M 是$M_i$ 的直和，$\bigwedge(M_i)$ 是$\bigwedge^0(M_i) = A$ 和$\bigwedge^1(M_i) = M_i$ 的直和（no. 3，命题 6）。让$\bigwedge(M)$与$\bigwedge(M_i)$的A-模张量积（no. 7，命题10）进行规范地标识；后者具有$\bigwedge(M_i)$的基$(1, e_i)$的基张量积（II, § 3, no. 7，推论2至命题7）；这样我们就得到了所有元素

$$
u_1 \otimes u_2 \otimes \cdots \otimes u_m
$$

其中$u_i = 1$或$u_i = e_i$；如果 J 是指标 i 的集合，使得 $u_i = e_i$、$u_1 \otimes u_2 \otimes \cdots \otimes u_m$ 与 $e_J$ 相同，从而完成证明。

#### 推论 1 {#alg-iii-s7-thm-1-cor-1 .statement tag=063G}

假设$L = \{1, m\}$；那么$\bigwedge(M)$的基$(e_J)_{J \in \mathscr{P}(L)}$有$2^m$元素。对于$p > m$、$\bigwedge^p(M) = \{0\}$； $\bigwedge^m(M)$ 有基由……组成单个元素 $e_L$；对于$e_J$的$\bigwedge^p(M)$由……组成的基$(e_J)$中元素的$0 \leq p \leq m$数，使得$\mathrm{Card}(J) = p$为

$$
\binom{m}{p} = \frac{m!}{p!(m-p)!}
$$

这是从集合理论、III, § 3, no. 5、命题12和集合理论、III, § 5, no. 8、推论1到命题11得出的。

我们回到定理 1 中集合 L 是任意的情况，并明确给出基 $(e_J)$ 的乘法表 (§ 1, no. 7)。给定全序集 $L$ 中的两个有限子集 $J, K$，我们写
$$
\begin{cases}
\rho_{J, K} = 0 & \text{if } J \cap K \neq \varnothing \\
\rho_{J, K} = (-1)^v & \text{if } J \cap K = \varnothing
\end{cases}
$$
其中$v$表示有序对$(\lambda, \mu) \in J \times K$中的数，使得$\lambda > \mu$。那么no. 2的推论1到命题4立即意味着关系
$$
e_J \wedge e_K = \rho_{J, K} e_{J \cup K}.
$$
注公式
$$
\rho_{J, K} \rho_{K, J} = (-1)^{jk}
$$
当$J \cap K = \varnothing, j = \mathrm{Card}(J), k = \mathrm{Card}(K)$（no. 3，推论2至命题5。）

#### 推论 2 {#alg-iii-s7-thm-1-cor-2 .statement tag=063H}

*如果 M 是射影 A-模，则 $\bigwedge(M)$ 是射影 A-模。*

证明与 § 5, no. 5 相同，推论定理 1 替换 T by $\bigwedge$。

#### 推论 3 {#alg-iii-s7-thm-1-cor-3 .statement tag=063I}

*设 M 为 M 的元素的射影 A-模和 $(x_i)_{1 \leq i \leq n}$ 有限序列。对于 M 交错的 n 线性形式 f 存在这样的*
$$
f(x_1, x_2, \ldots, x_n) \neq 0,
$$
*这是必要且充分的* $x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0$。

我们已经知道（M 上没有假设）条件是必要的（no. 4，命题 7）。现在假设 M 是射影的并且
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0.
$$
那么 $\bigwedge^n(M)$ 是投影（推论 2），因此典范映射
$$
\bigwedge^n(M) \to (\bigwedge^n(M))^{**}
$$
是单射的（II, § 2, no. 7，推论 4 到命题 13）；我们结论存在线性形式$g : \bigwedge^n(M) \to A$使得$g(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \neq 0$。如果$f$是交错的n-线性形式相应的到$g$（no. 4，命题7），则$f(x_1, \ldots, x_n) \neq 0$。

### 9. 判据线性无关

#### 命题 12 {#alg-iii-s7-prop-12 .statement tag=063J}

*设 M 为射影 A-模。为了使 M 的元素 $x_1, x_2, \ldots, x_n$ 线性相关，A 中存在 $\lambda \neq 0$ 是必要且充分的，使得*
$$
\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0.
$$

条件是必要的（M上没有假设），因为如果例$\lambda x_1$（有$\lambda \neq 0$）是$x_2, \ldots, x_n$的线性组合，关系（22）成立（no. 3，命题5）。我们通过$n$上的归纳证明条件是足够的；对于 $n = 1$ 来说，它是定义的微不足道的推论。因而，假设 $n > 1$ 和条件 (22) 对于某些 $\lambda \neq 0$ 成立。如果
$$
\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n = 0,
$$
那么归纳假设意味着 $x_2, \ldots, x_n$ 是线性相关的，因而 *更不必说* $x_1, x_2, \ldots, x_n$ 是线性相关的。如果$\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n \neq 0$，则从no. 8，推论3到定理1，存在交错的$(n - 1)$-线性形式$f$，使得$f(\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n) = \mu \neq 0$。自从
$$
x_1 \wedge (\lambda x_2) \wedge \cdots \wedge x_n = 0,
$$
由no. 8，推论3到定理1，$\mu x_1$是$\lambda x_2, x_3, \ldots, x_n$的线性组合；因而 $x_1, x_2, \ldots, x_n$ 是线性相关的。

#### 推论{#alg-iii-s7-n9-cor-1 .statement tag=063K}

*设 M 和 N 为两个射影 A-模和 $f : M \to N$ A-线性映射。如果 f 是单射，则 $\Lambda(f) : \Lambda(M) \to \Lambda(N)$ 是单射。*

我们首先在假设下证明 M 是*自由*；设$(e_\lambda)_{\lambda \in L}$为M的基，则$(e_J)_{J \in \mathfrak{B}(L)}$(公式(18))为$\Lambda(M)$的基。假设$\Lambda(f)$包含元素$u = \sum_J \alpha_J e_J \neq 0$中的核。令 K 为有限子集 J 中最小的元素，使得$\alpha_J \neq 0$，并令 H 为来自 K 的 L 不相交的的有限子集，并且使得 $K \cup H$ 包含所有 J（数中有限），使得 $\alpha_J \neq 0$；对于所有 $J \neq K$ 使得 $\alpha_J \neq 0$，我们因此有定义 $J \cap H \neq 0$，因而 (no. 8, 公式 (20))。
$$
u \wedge e_H = +\alpha_K e_{K \cup H}
$$
属于到$\Lambda(M)$的双面理想，核$\Lambda(f)$。我们写$e_{K \cup H} = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}$；然后$\alpha_K f(e_{\lambda_1}) \wedge f(e_{\lambda_2}) \wedge \cdots \wedge f(e_{\lambda_n}) = 0$；由于命题 12，N 的元素 $f(e_{\lambda_i})$ ($1 \leq i \leq n$) 是线性相关的。但是$f$是单射的与……矛盾假设（II, § 1, no. 11，推论3到命题17）。

我们现在考虑一般情况；令$M'$为A-模，使得$M \oplus M' = P$是免费的（II, § 2, no. 2，命题4）。考虑线性映射$g : M \oplus M' \to N \oplus M \oplus M'$使得$g(x, y) = (f(x), 0, y)$，因此存在可交换的图表
$$
\begin{array}{ccc}
M & \xrightarrow{f} & N \\
j \downarrow & & j' \downarrow \\
P & \xrightarrow{g} & N \oplus P
\end{array}
$$

其中垂直箭头是典范嵌入。由于$g$是单射的并且$P$是自由的，因而$\Lambda(g)$是单同态，如上所示。现在，$\Lambda(j): \Lambda(M) \to \Lambda(P)$ 是单同态，因为 $M$ 在 $P$ (no. 2) 中是直因子。复合同态

$$
\Lambda(M) \xrightarrow{\Lambda(j)} \Lambda(P) \xrightarrow{\Lambda(g)} \Lambda(N \oplus P)
$$

因此是单射的，并且它也等于复合同态

$$
\Lambda(M) \xrightarrow{\Lambda(f)} \Lambda(N) \xrightarrow{\Lambda(g')} \Lambda(N \oplus P)
$$

我们结论 $\Lambda(f)$ 是单射的。

#### 命题 13 {#alg-iii-s7-prop-13 .statement tag=063L}

*令$M$为$A$模块，$M$的$N$直因子子模不含维数$p$和$\Lambda^p(N)$的$\{u\}$基。对于元素$x \in M$到属于到$N$，$u \wedge x = 0$是充分必要的。*

令$P$为$M$的子模与$N$互补，并令$y \in N,\ z \in P$使得$x = y + z$。然后$u \wedge x = u \wedge z$。由于 $\Lambda^p(N)$ 不包含维数 1、映射 $\phi: P \to P \otimes \Lambda^p(N)$，因此 $\phi(p) = p \otimes u$ 是双射 (II, § 3, no. 4、命题 4)。另一方面 (no. 7, 命题 10), 合成 / 典范同态

$$
\psi: P \otimes \Lambda^p(N) \to \Lambda(P) \otimes \Lambda(N) \to \Lambda(M)
$$

是单射的。因此映射 $\psi \circ \phi$ 是单射的，从而命题。

#### 定理 2 {#alg-iii-s7-thm-2 .statement tag=063M}

*令 $M$ 为具有有限基 $(e_i)_{1 \leq i \leq n}$ 的 $A$ 模。对于$n$的序列$(x_i)_{1 \leq i \leq n}$、$M$的元素到$M$的形式基，元素$\lambda \in A$是充分必要的，使得

$$
x_1 \wedge x_2 \wedge \ldots \wedge x_n = \lambda \cdot e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

在$A$内可逆。*

回想一下，$e_1 \wedge e_2 \wedge \cdots \wedge e_n$是$\Lambda^n(M)$的基的唯一元素（no. 8，推论1到定理1），因此元素$\lambda \in A$满足（23）是唯一确定的。如果$(x_i)_{1 \leq i \leq n}$是$M$的基，$x_1 \wedge x_2 \wedge \cdots \wedge x_n$在$\Lambda^n(M)$的基（no. 8）中是唯一元素，则$\lambda$是可逆的。相反，假设$\lambda$是可逆的；然后交错的 $n$-线性形式 $f$ 相应的到线性映射 $g: \Lambda^n(M) \to A$ 使得

$$
g(e_1 \wedge e_2 \wedge \cdots \wedge e_n) = \lambda^{-1}
$$

是这样的$f(x_1, x_2, \ldots, x_n) = 1$。对于所有$x \in M$，显然

$$
x \wedge x_1 \wedge \cdots \wedge x_n = 0
$$

（no. 3，命题6）； 应用no. 8，推论3到定理1，我们得到

$$
f(x_1, x_2, \ldots, x_n) \cdot x = \sum_{i=1}^n (-1)^{i-1} f(x, x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i.
$$

作为$f(x_1, \ldots, x_n) = 1$，这表明每个$x \in M$都是$x_1, x_2, \ldots, x_n$的线性组合，并且后者是线性独立的（因为

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0),
$$

他们形式基共$M$。

### 习题{#alg-iii-s7-exercises}

§ 7](exercises/s7/)参见[习题。
