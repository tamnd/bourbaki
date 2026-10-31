---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 10
section_title: Matrices
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 338-363, 417-424
pdf_pages: 0362-0387, 0441-0448
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF MATRICES
      page: 338
      pdf_page: 362
    - "no": 2
      title: MATRICES OVER A COMMUTATIVE GROUP
      page: 339
      pdf_page: 363
    - "no": 3
      title: MATRICES OVER A RING
      page: 341
      pdf_page: 365
    - "no": 4
      title: MATRICES AND LINEAR MAPPINGS
      page: 342
      pdf_page: 366
    - "no": 5
      title: BLOCK PRODUCTS
      page: 346
      pdf_page: 370
    - "no": 6
      title: MATRIX OF A SEMI-LINEAR MAPPING
      page: 347
      pdf_page: 371
    - "no": 7
      title: SQUARE MATRICES
      page: 349
      pdf_page: 373
    - "no": 8
      title: CHANGE OF BASES
      page: 352
      pdf_page: 376
    - "no": 9
      title: EQUIVALENT MATRICES; SIMILAR MATRICES
      page: 354
      pdf_page: 378
    - "no": 10
      title: TENSOR PRODUCT OF MATRICES OVER A COMMUTATIVE RING
      page: 356
      pdf_page: 380
    - "no": 11
      title: TRACE OF A MATRIX
      page: 358
      pdf_page: 382
    - "no": 12
      title: MATRICES OVER A FIELD
      page: 359
      pdf_page: 383
    - "no": 13
      title: EQUIVALENCE OF MATRICES OVER A FIELD
      page: 360
      pdf_page: 384
statements: 35
exercises: 17
content_sha256: 676aa5f0238251bccc540aa94541ed6101e617753286f42b7bb25c84fdbcdde7
translated_from: content/en/alg/II/10_s10_matrices.md
translation_method: google
source_content_sha256: 9f20d99617c7f5aad6362a5f7207c5eb84fe7bf5906f6a9107df6de45c2d511a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 9fed53bb226638760514ebeee60aa688de5c92f36ce6d7d224b91c0fddff0005
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 10。 矩阵

### 1. 定义的矩阵

#### 定义 1 {#alg-ii-s10-def-1 .statement tag=05WH}

令$I, K, H$为三集合； 型 $(I, K)$ 矩阵且$H$ 中元素（或型 $(I, K)$ 矩阵超过$H$）是$H$ 元素 $M = (m_{i\kappa})_{(i, \kappa) \in I \times K}$ 的任何家庭，其索引集合为乘积 $I \times K$。对于所有$i \in I$，族$(m_{i\kappa})_{\kappa \in K}$称为指标$i$的$M$行；对于所有$\kappa \in K$，$(m_{i\kappa})_{i \in I}$家族称为指标$\kappa$$M$列。

如果 $I$（或 $K$）是有限的，则 $M$ 被称为矩阵，且行数有限数（或列）。 $H$以上的型$(I, K)$矩阵的集合被识别为乘积$HI^{I \times K}$。

名称“row”和“列”源自以下事实：在$I$和$K$是$\mathbf{N}$的间隔$[1, p], [1, q]$的情况下，矩阵的元素被设想为具有$p$行的矩形阵列中的集合 （水平排列）和 $q$ 列（垂直排列）：

$$
\begin{pmatrix}
m_{11} & m_{12} & \cdots & m_{1q} \\
m_{21} & m_{22} & \cdots & m_{2q} \\
\cdots & \cdots & \cdots & \cdots \\
m_{p1} & m_{p2} & \cdots & m_{pq}
\end{pmatrix}
$$

当 $p$ 和 $q$ 明确整数足够小以使其可行时，按照惯例，上述数组是有效表示所讨论的矩阵的符号；这个记号使我们能够免除使用指标，可以理解，元素的指标是由它在数组中的位置决定的；对于例，当我们谈到矩阵时

$$
\begin{pmatrix}
a & b & c \\
d & e & f
\end{pmatrix}
$$

我们的意思是矩阵 $(m_{ij})_{1 \leq i < 2, 1 \leq j < 3}$ 这样

$$
m_{11} = a,\ m_{12} = b,\ m_{13} = c,\ m_{21} = d,\ m_{22} = e,\ m_{23} = f.
$$

如果不引起混淆，我们也可以说型 $(p, q)$ 的矩阵，或者矩阵 $p$ 行和$q$ 列，而不是型 $([1, p], [1, q])$ 的矩阵； 型$(p, q)$的矩阵超过$H$的集合是有时，用$\mathbf{M}_{p, q}(H)$表示。

$H$上的每个矩阵，其索引集合$I, K$之一为空，与$H$的元素的空族相同；又名空矩阵。当$I = \{i_0\}$（或$K = \{k_0\}$）是单个元素的集合由……组成时，$M$称为行矩阵（或列矩阵）和行（或矩阵）。 列)指标可以在记号中被抑制；当$I$和$K$都是集合且有一个元素时，型$(I, K)$中的矩阵常常被识别为这个矩阵中的唯一元素。

矩阵 $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$的子族$M' = (m_{\iota \kappa})_{(\iota, \kappa) \in J \times L}$，其索引集合为$I$的子集$J$和子集$L$的乘积，称为$K$的*子矩阵* 矩阵$M$；据说是通过在$M$中*抑制*指标$\iota \notin J$和列的指标$\kappa \notin L$的行来获得；相反，$M$据说是通过将指标$\iota \notin J$和列的指标$\kappa \notin L$的行*接壤*$M'$获得的。

#### 定义 2 {#alg-ii-s10-def-2 .statement tag=05WI}

*矩阵* $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$的转置，*表示为* $^tM$，*是矩阵* $(m'_{\kappa \iota})_{(\kappa, \iota) \in K \times I}$ *超过* $H$ *由* $m'_{\kappa \iota} = m_{\iota \kappa}$ *所有* $(\iota, \kappa) \in K \times L$给出。

由此定义得出型$(I, K)$矩阵转置是型$(K, I)$矩阵并且

(1)
$$
^t(^tM) = M.
$$

### 2. 矩阵超过可交换群

令 $G$ 为交换律群（加法写）。 $G$ 上的矩阵的集合，给定索引集合 $I, K$，具有*可交换的群* 结构，因为它是从 $I \times K$ 到映射的集合 $G$；这个群是相加写的，所以如果$M = (m_{\iota \kappa})$和$M' = (m'_{\iota \kappa})$是它的元素中的两个，那么
$$
M + M' = (m_{\iota \kappa} + m'_{\iota \kappa});
$$
因此，这个群中的单位元素是矩阵，其所有元素都是*零*（称为*零矩阵*）。显然
(2)
$$
^t(M + M') = ^tM + ^tM'.
$$

因此，仅当行的索引集合和列对于两个矩阵 *相同*时，才定义两个矩阵的和。

令$H', H''$是两个集合，$G$是可交换的群（相加）和从$H' \times H''$到$G$的$f : (h', h'') \mapsto h'h''$映射。给定两个矩阵
$$
M' = (m'_{ik})_{(i, k) \in I \times K}, \quad M'' = (m''_{kl})_{(k, l) \in K \times L}
$$
分别超过$H'$和$H''$，使得$M'$的列的索引集合$K$是*有限*并且等于$M''$的行的索引集合，*的*乘积* $M'$和$M''$*通过*$f$，用$M'M''$或$f(M', M'')$表示，是矩阵
(3)
$$
\left( \sum_{k \in K} m'_{ik} m''_{kl} \right)_{(i, l) \in I \times L}
$$
超过$G$。

上述定义假设$M'$的列的索引集合等于$M''$的行的索引集合；特别是乘积 $M''M'$ *如果* $I \neq L$ 则没有任何意义。在 $M'$ 数字的公式 (3) 元素右边乘以$M''$ 的*同* 列的元素；据说乘法是“按列排列”。

令$f^0$为$H'' \times H'$至$G$中的映射$(h'', h') \mapsto h'h''$；从定义可以立即得出
$$
t(M'M'') = tM''.tM'
$$
其中左侧（或右侧）的乘积是通过$f$（或通过$f^0$）计算的。

当 $H'$ 和 $H''$ 本身是可交换的群（相加）且 $f$ 是 $\mathbf{Z}$-*双线性* (§ 3, no. 1) 时，分配律公式
$$
\begin{cases}
(M' + N')M'' = M'M'' + N'M'' \\
M'(M'' + N'') = M'M'' + M'N''
\end{cases}
$$
立即验证，索引集合使得和和乘积出现被定义。

现在让 $H_1, H_2, H_3, H_{12}, H_{23}$ 和 $H$ 可交换群 （相加），$f_{12}:H_1 \times H_2 \to H_{12}, f_{23}:H_2 \times H_3 \to H_{23}$ 映射和
$$
f_3:H_{12} \times H_3 \to H, \quad f_1:H_1 \times H_{23} \to H
$$
$\mathbf{Z}$-双线性映射；进一步假设，对于所有 $x_i \in H_i \ (i = 1, 2, 3)$
$$
f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))
$$
（也可以写成上面$(x_1 x_2)x_3 = x_1(x_2 x_3)$）；那么，如果 $M' = (m'_{rs}), M'' = (m''_{st}), M''' = (m'''_{tu})$ 分别大于 $H_1, H_2, H_3$ 矩阵，
$$
(M'M'')M''' = M'(M''M'''')
$$
当定义了两侧的乘积（分别通过$f_{12}, f_3, f_{23}$和$f_1$计算）时；为了
$$
\sum_t \left( \sum_s m'_{rs} m''_{st} \right) m'''_{tu} = \sum_t \sum_s (m'_{rs} m''_{st}) m'''_{tu} = \sum_s \sum_t m'_{rs} (m''_{st} m'''_{tu})
$$
$$
= \sum_s m'_{rs} \left( \sum_t m''_{st} m'''_{tu} \right)
$$
凭借所做的假设。

(6)的两边也用$M'M''M'''$表示。对于三个以上因子中的乘积也有类似的约定。

#### 注 {#alg-ii-s10-n2-rem-1 .statement tag=05WJ}

以上公式扩展为更一般的情况。准确地说：

(a) 假设$H = \bigcup_{(\iota, \kappa) \in I \times K} G_{\iota \kappa}$，其中每个$G_{\iota \kappa}$是可加写的交换律群；那么对于每个有序对$(\iota, \kappa)$、$m_{\iota \kappa} \in G_{\iota \kappa}$和$m'_{\iota \kappa} \in G_{\iota \kappa}$，可以定义和$M + M'$。

(b) 设I、K、L为三个集合，假设K是有限的，并令$H' = \bigcup_{(i, k) \in I \times K} H'_{ik}$、$H'' = \bigcup_{(k, l) \in K \times L} H''_{kl}$、$H = \bigcup_{(i, l) \in I \times L} H_{il}$为三个集合；假设每个 $H_{il}$ 都是一个可加的交换律群，并且对于每个三元组 $(i, k, l)$ 让
$$
f_{ikl}: H'_{ik} \times H''_{kl} \to H_{il}
$$
是映射。然后，如果$M' = (m'_{ik})_{(i, k) \in I \times K}$，$M'' = (m''_{kl})_{(k, l) \in K \times L}$是矩阵，使得$m'_{ik} \in H'_{ik}$和$m''_{kl} \in H''_{kl}$对于所有$i, k, l$，我们可以通过$f_{ikl}$得到定义乘积$M'M''$。我们留给读者写下类似于（4）、（5）和（6）的证明公式的任务。

### 3.矩阵超过环

数学中最重要的矩阵是矩阵超过环A。矩阵超过相应的的集合$A^{I \times K}$到索引集合I，K则具有规范的（A，A）双模结构（§ 1, no. 14）。

对于每个有序对$(i, k) \in I \times K$，令$E_{ik}$为矩阵$(a_{jl})$，使得$a_{ik} = 1$和$a_{jl} = 0$对应$(j, l) \neq (i, k)$； $E_{ik}$在矩阵$A^{I \times K}$的集合中称为矩阵单位；如果 I 和 K 是有限的，则它们集合的左侧为形式典范基或右A-模结构 (§ 1, no. 11)。显然
$$
tE_{ik} = E_{ki}.
$$

除非另外提到，A上的两个矩阵的乘积$M'M''$（假设已定义）将始终被理解为相对于A中的乘法$(x, y) \mapsto xy$（或者，也如所说，将“在A中计算”）。那么我们有 (no. 2) 结合性和分配律公式

(7)
$$(XY)Z = X(YZ)$$

(8)
$$
\begin{cases}
X(Y + Z) = XY + XZ \\
(X + Y)Z = XZ + YZ
\end{cases}
$$
对于三个矩阵X，Y，Z在A上，每当和和乘积出现在这些公式中被定义。

特别是，如果$E_{ik}$（分别$E'_{kl}, E''_{il}$）在$A^{I \times K}$（分别$A^{K \times L}, A^{I \times L}$）中分别为矩阵单位，以及$I = \{1, p\}, K = \{1, q\}, L = \{1, r\}$，我们得到公式
$$
\begin{cases}
E_{ik}E'_{jl} = 0 & \text{if } k \neq j \\
E_{ik}E'_{kl} = E''_{il}.
\end{cases}
$$

令$A^0$为A的逆环，令$a * b \ (= ba)$表示$A^0$中a和b的乘积；那么，对于两个矩阵 X，Y 在定义了乘积的 A 上，
$$(10)$$
$$
t(XX) = tY * tX
$$

其中，在右侧，$^tY$ 和 $^tX$ 被视为矩阵，元素在 $\mathbf{A}^0$ 中；当 $\mathbf{A}$ 是*可交换的*，那么

$$(11)$$
$$
^t(XY) = ^tY.^tX
$$

#### 命题 1 {#alg-ii-s10-prop-1 .statement tag=05WK}

*令$\mathbf{A}, \mathbf{B}$为两个环和$M = (m_{ik})_{(i,k) \in I \times K}$并且*
$$
M' = (m'_{ik})_{(i,k) \in I \times K}
$$
*两个矩阵，在一个* $(\mathbf{A}, \mathbf{B})$*-双模块* $G$上具有有限索引集合。 *假设对于每个矩阵单位* $L = (a_i)_{i \in I}$ *有一行和元素在* $\mathbf{A}$ *和每个矩阵单位* $C = (b_k)_{k \in K}$ *有一个列和元素在* $\mathbf{B}$, $L.M.C = L.M'.C$ （*乘积通过*$(\mathbf{A}, \mathbf{B})$*-模块*$G$的外法则计算）；然后* $M = M'$。

如果 $L$ 被视为矩阵单位 $(a_s)$，$s \neq i$ 为 $a_i = 1, a_s = 0$，$C$ 矩阵单位 $(b_t)$，$t \neq k$ 为 $b_k = 1, b_t = 0$，乘积 $L.M.C$和$L.M'.C$是矩阵，单个元素分别等于$m_{ik}$和$m'_{ik}$。

令$\mathbf{A}, \mathbf{B}$为两个环和$\sigma : \mathbf{A} \to \mathbf{B}$同态。

对于$\mathbf{A}$上的每个矩阵$M = (m_{ik})$，我们将用$\mathbf{B}$上的$\sigma(M)$矩阵$(\sigma(m_{ik}))$来表示；显然$\sigma(aM) = \sigma(a)\sigma(M)$，$\sigma(Ma) = \sigma(M)\sigma(a)$代表$a \in \mathbf{A}$，还有$\sigma(^tM) = (^t(\sigma(M)))$和

$$(12)$$
$$
\begin{cases}
\sigma(M + M') = \sigma(M) + \sigma(M') \\
\sigma(MM') = \sigma(M)\sigma(M')
\end{cases}
$$
*当定义运算时，(12)左边和右边的乘积分别在*$\mathbf{A}$*和*$\mathbf{B}$*中计算。*当$\sigma$用$x \mapsto x^\sigma$表示时，我们写成$M^\sigma$而不是$\sigma(M)$。

特别考虑$\mathbf{A}$的*反自同态*$\sigma$，即$\mathbf{A}$的同态到逆环$\mathbf{A}^0$，或$\mathbf{A}$的映射自身，这样
$$
\sigma(a + a') = \sigma(a) + \sigma(a'), \qquad \sigma(aa') = \sigma(a')\sigma(a)
$$
*对于所有* $a, a'$ *在* $\mathbf{A}$；那么，对于$\mathbf{A}$上的两个矩阵$M, M'$，其乘积$MM'$已定义，
$$(13)$$
$$
\sigma(MM') = (^t(\sigma(^tM')).\sigma(^tM))
$$
*其中两侧乘积的计算公式为*$\mathbf{A}$； *这紧随 (10) 和 (12) 而来。*

### 4.矩阵和线性映射

令$\mathbf{A}$为环且$E$一个*（右或左）*$\mathbf{A}$*-模块*承认基$(e_i)_{i \in I}$。对于每个元素$x \in E$，*$x$*相对于基*$(e_i)$的*矩阵，用$M(x)$或$\mathbf{x}$表示（或者在不会引起混淆的情况下，有时简单地用$x$表示），是 $x$ 的分量 $x_i \ (i \in I)$ 相对于 $(e_i)$ (§ 1, no. 11) 的 *列矩阵* 由……组成；在计算中，有时会很方便，在阶中记住指标$i$是一行指标，与它相邻的列指标只取一个值并将矩阵$M(x)$写为$(x_{i0})$。

我们现在考虑两个（左或右）A-模 E 和 F，分别为基 $(e_i)_{i \in I}$ 和 $(f_k)_{k \in K}$；设$(f_k^*)$为形式相应的到$(f_k)$的坐标系。对于 E 的线性映射 $u$ 到 F 中，在以下每种情况下，我们应将 u 的定义 *矩阵相对于基* $(e_i), (f_k)$：

(D) E 和 F 是右A-模，$u$ 是 A 线性。
(G) E 和 F 是左A-模，$u$ 是 A 线性。

接下来，我们将字母 (D)（分别为 (G)）附加到公式应用右侧（分别为左侧）模。

#### 定义 3 {#alg-ii-s10-def-3 .statement tag=05WL}

*在上述两种情况中，u 的矩阵相对于基* $(e_i), (f_k)$ *是矩阵* $M(u) = (u_{ki})_{(k, i) \in K \times I}$ *这样*

$$
u_{ki} = f_k^*(u(e_i))
$$

*分别写为*

(14D)
$$
u_{ki} = \langle f_k^*, u(e_i) \rangle
$$
（14克）
$$
u_{ki} = \langle u(e_i), f_k^* \rangle.
$$

因此，指标$i$的$M(u)$的*列*等于$M(u(e_i))$。

显然，如果$u, v$是E到F中的两个线性映射，并且$M(u), M(v)$它们的矩阵相对于相同的基，那么

$$
M(u + v) = M(u) + M(v)
$$
和
$$
M(\gamma u) = \gamma M(u)
$$
对于A的*中心* $\Gamma$的每个元素$\gamma$。在其他字中，一旦基$(e_i), (f_k)$固定，映射$u \mapsto M(u)$是一个*$\Gamma$模同构* $\mathrm{Hom}_A(E, F)$ 到集合 $A^{K \times I}$ 的子集，如果 K 是*有限*，则等于 $A^{K \times I}$。

#### 命题 2 {#alg-ii-s10-prop-2 .statement tag=05WM}

*假设I和K是有限的。对于每个元素* $x \in E$，*矩阵* $M(u(x))$ *相对于基* $(f_k)$ *由公式* 给出

(17D)
$$
M(u(x)) = M(u) . M(x)
$$
（17克）
$$
{}^t M(u(x)) = {}^t M(x) . {}^t M(u).
$$

我们验证例（17 G）。让 $x = \sum_i x_{i0} e_i, \quad u(x) = \sum_k y_{k0} f_k$ 与 $x_{i0} \in A, \ y_{k0} \in A$；然后$u(x) = u\left( \sum_i x_{i0} e_i \right) = \sum_i x_{i0} u(e_i) = \sum_{i, k} x_{i0} u_{ki} f_k$； 从而 y_{k0} = \和_i x_{i0} u_{ki}。在阶中，将两个指标$i$沿着一个另一个并排，我们考虑转置矩阵${}^t M(x) = (x'_{0i})$，其中$x'_{0i} = x_{i0}$和
$$
{}^t M(u) = (u'_{ik}),
$$
其中$u'_{ik} = u_{ki}$；那么$y_{k0} = \sum_i x'_{0i} u'_{ik}$，右手边是指标$k$的矩阵的元素，其中一行${}^t M(x) \cdot {}^t M(u)$，从而（17G）。

当 A 是可交换的时，(17 G) 约化通过 no. 2 的公式 (4) 到 (17 D)。

#### 推论{#alg-ii-s10-n4-cor-1 .statement tag=05WN}

*设 E、F、G 为环 A、$(e_i)_{i \in I}$、$(f_k)_{k \in K}$、$(g_l)_{l \in L}$ 上的三个右（左）模分别为 E、F、G、$u : E \to F$、$v : F \to G$ 两个线性映射的有限基， u 的 $M(u)$ 矩阵相对于 v 的基 $(e_i)$、$(f_k)$、$M(v)$ 矩阵相对于 的基 $(f_k)$、$(g_l)$ 和 $M(v \circ u)$ 矩阵 $v \circ u$相对于基$(e_i)$、$(g_l)$；然后*

(18D)
$$
M(v \circ u) = M(v) M(u)
$$
(18克)
$$
{}^t M(v \circ u) = {}^t M(u) {}^t M(v).
$$

我们证明例 (18 G)。对于所有 $x \in E$，通过 (17 G)：
$$
{}^t M(x) \cdot {}^t M(v \circ u) = {}^t M(v(u(x))) = {}^t M(u(x)) \cdot {}^t M(v) = {}^t M(x) \cdot {}^t M(u) \cdot {}^t M(v)
$$
结合性；然后从 no. 3、命题 1 得出推论，因为矩阵 ${}^t M(x)$ 中的一行是任意的。

*注(1)*。 公式 (17 D) 可以被认为是 (18 D) 的特例。 对于每个$x \in E$线性映射$\theta_x : A_d \to E$映射，每个$\alpha \in A$到$x \alpha$（§ 2, no. 1），对应规范地存在。 It is immediate that the matrix $M(\theta_x)$ with respect to the basis 1 of $A_d$ and the basis $(e_i)$ of E is just the matrix $M(x)$; similarly $M(\theta_{u(x)}) = M(u(x))$ and formula (17 D) can therefore be considered as a translation of the relation
$$
\theta_{u(x)} = u \circ \theta_x.
$$

#### 命题 3 {#alg-ii-s10-prop-3 .statement tag=05WO}

*设E、F分别是E和F的两个右（左）A-模和$(e_i)_{i \in I}$、$(f_k)_{k \in K}$有限基。对于 E 到 F 中的每个线性映射 u，令 $M(u)$ 为 u 相对于基 $(e_i)$ 和 $(f_k)$ 的矩阵。那么${}^t u : F^* \to E^*$相对于对偶基$(f_k^*)$和$(e_i^*)$的矩阵等于${}^t M(u)$。*

E 被规范地标识为其双数 $E^{**}$ 和 $(e_i)$，其中对偶基为 $(e_i^*)$；那么（假设例，E和F是正确的模）
$$
\langle {}^t u(f_k^*), e_i \rangle = \langle f_k^*, u(e_i) \rangle,
$$
从而命题。

#### 注 {#alg-ii-s10-n4-rem-1 .statement tag=05WP}

(2) 令E和F分别为两个左A-模，其中基、$(e_i)_{i \in I}$和$(f_k)_{k \in K}$。对于每 A-线性映射 $u : E \to F$，通过 (14 G)，$u(e_i) = \sum_k u_{ki} f_k$；这些关系也可以被说解释为列矩阵$(u(e_i))_{i \in I}$与元素在F中等于乘积$^tM(u) \cdot (f_k)$，其中$(f_k)_{k \in K}$被视为列矩阵 F 中的元素和乘积是针对映射 $A \times F \to F$ 计算的，定义 A-模 F (no. 2) 上的作用的律。

(3) 令A、B为两个交换环和$\sigma : A \to B$环同态。在命题 3 的记号中，$(e_i \otimes 1)$和$(f_k \otimes 1)$分别是$E_{(B)} = E \otimes_A B$和$F_{(B)} = F \otimes_A B$的基（§ 5, no. 1、命题 4）；此外，如果$(e_i^*)$和$(f_k^*)$分别是$(e_i)$和$(f_k)$的对偶基，则$(e_i^* \otimes 1)$和$(f_k^* \otimes 1)$分别是$(e_i \otimes 1)$和$(f_k \otimes 1)$的对偶基 （§ 5, no. 4）。对于每个A-线性映射$u : E \to F$，令$M(u)$和$M(u \otimes 1)$相对于$(e_i)$为$u$的矩阵，相对于B-线性映射$u \otimes 1$为$(f_k)$和矩阵 $(e_i \otimes 1)$ 和 $(f_k \otimes 1)$。由 § 5, no. 4, 公式 (20) 得出
$$
M(u \otimes 1) = \sigma(M(u)).
$$

考虑有限数未知数中有限数右标量线性方程的系统
$$
\sum_{i \in I} a_{kt} x_i = b_k \quad (k \in K)
$$
A 中有 $a_{kt}, x_i, b_k$。

令$(e_i)_{i \in I}, (f_k)_{k \in K}$为$E = A_d^I$和$F = A_d^K$的规范基； 系统 (19) 等价于方程 $u(x) = b$，其中 $x = \sum_i e_i x_i$、$b = \sum_k f_k b_k$ 和 $u : E \to F$ 为线性映射，使得矩阵 $M(u)$ 相对于基 $(e_i)$ 和 $(f_k)$ 等于$A = (a_{kt})_{(k, i) \in K \times L}$。该矩阵称为线性方程组(19)的系统的矩阵。回想一下 (§ 2, no. 8, 注 2 和 3)，写出 $c_i = \sum_k f_k a_{kt}$, 系统 (19) 等价于唯一的向量方程
$$
\sum_i c_i x_i = b,
$$
由于$c_i$是矩阵$A$中指标$i$的列，我们看到说系统（19）承认解等于说即矩阵 $b = (b_{k0})$和一个列是矩阵$A$列线性组合。

我们留给读者为左线性方程的系统制定类似的定义和注的任务。

### 5.块乘积

no. 4的定义可以概括如下。设E是子模族$(E_i)_{i \in I}$的（右或左）A-模、直和。对于所有$x \in E$，让$x = \sum_{i \in I} x_i$和$x_i \in E_i$对于所有$i \in I$；我们可以说，E 中的列矩阵 $M(x) = (x_i)_{i \in I}$ 和元素是 x 的 *矩阵，而 E 的分解 $(E_i)_{i \in I}$ 是直和*。

设F为另一个A-模（E和F都是右A-模或都是左A-模），并假设F是子模的$(F_k)_{k \in K}$族的直和。对于所有$u \in \mathrm{Hom}(E, F)$和所有$x_i \in E_i$，让$u(x_i) = \sum_k u_{ki}(x_i)$和$u_{ki}(x_i) \in F_k$对于所有$k \in K$；然后$u_{ki} \in \mathrm{Hom}(E_i, F_k)$；我们可以说，型$(K, I)$的矩阵$M(u) = (u_{ki})_{(k, i) \in K \times I}$和$\mathrm{Hom}(E_i, F_k)$的集合H和中的元素是u相对于分解的*矩阵 E和F的$(E_i)$和$(F_k)$为直和*。

有了这些定义，很明显，如果$u, v$是E到F中的两个A-线性映射，那么对于矩阵来说，对于与直和相同的分解

$$
M(u + v) = M(u) + M(v), \qquad M(\gamma u) = \gamma M(u)
$$

对于 A 的中心的每个元素 $\gamma$（no. 2，*注*）。

此外，$u_{ki}$的定义表明，如果K是有限的，我们可以写

$$
M(u(x)) = M(u) . M(x)
$$

其中，$M(u(x))$是$u(x)$的矩阵，相对于分解$(F_k)$，(22)右侧的乘积将$\mathrm{Hom}(E_i, F_k) \times E_i$的映射$(t, z) \mapsto t(z)$计算为$F_k$ （no. 2，*注*）。

令 G 为子模中$(G_l)_{l \in L}$ 的第三个A-模、直和，因此对于分解，每个 A-线性映射 $v : F \to G$ 矩阵 $M(v) = (v_{lk})$ 都有对应 $(F_k)$ 和 $(G_l)$。如果 I、K 和 L 是*有限*，那么

$$
M(v \circ u) = M(v) . M(u)
$$

其中，左手边是 $w = v \circ u$ 的矩阵 $(w_{li})$ 相对于分解 $(E_i)$ 和 $(G_l)$，左手边的乘积将 $\mathrm{Hom}(F_k, G_l) \times \mathrm{Hom}(E_i, F_k)$ 的映射 $(t, s) \mapsto t \circ s$ 计算为 $\mathrm{Hom}(E_i, G_l)$ （no. 2，*注*）。这只是§ 1, no. 8的公式(32)，以矩阵的项来表示。

最后，如果假设 I 和 K 是有限的，则 $E^*$（分别为 $F^*$）被规范地标识为模 $E_i^*$（分别为 $F_k^*$）（§ 2, no. 6、命题 10）的直和。那么立即验证$^t u$相对于分解$(F_k^*)$和$(E_i^*)$的矩阵正好是$(^t u_{ki})_{(k, i) \in K \times I}$。

现在假设I和K是有限的，并且每个E_i（分别是F_k）都承认有限的基。这相当于说 E（分别为 F）承认基 (e_r)_{r \in R}（分别为 (f_s)_{s \in S}），并且 R（分别为 S）承认划分 (R_i)_{i \in I}（分别为 (S_k)_{k \in K}），这样对于所有 i \in I（分别为 k \in K），(e_r)_{r \in R_i} 为 E_i 的基（分别为 (f_s)_{s \in S_k} 为 F_k 的基）。那么，如果 X = M(u) 是 u 相对于基 (e_r)_{r \in R} 和 (f_s)_{s \in S} 的矩阵，则矩阵 X_{kt} = M(u_{kt}) 相对于基 (e_r)_{r \in R_i} (f_s)_{s \in S_k} 只是通过抑制指标 s \notin S_k 和列的指标 r \notin R_i 的行而获得的 X 的子矩阵。因此我们定义一对一对应

$$
X \mapsto (X_{kt})_{(k, t) \in K \times I}
$$

型 (S, R) 的矩阵集合与 A 中的元素和矩阵矩阵集合型 K 的 $(X_{kt})_{(k, t) \in K \times I}$ \times I，其中每个 X_{kt} 为矩阵超过型 (S_k, R_i) 的 A。 假设进一步 G 承认有限基 (g_t)_{t \in T} 并且 T = (T_l)_{l \in L} 是 T 的划分，这样，对于每个 l \in L，(g_t)_{t \in T_l} 是 G_l 的基；令 Y = M(v) 为 v 相对于基 (f_s)_{s \in S} 和 (g_t)_{t \in T} 的矩阵，Y_{lk} = M(v_{lk}) 为 v_{lk} 相对于基 (f_s)_{s \in S_k} 和 (g_t)_{t \in T_l}， w = v \circ u 的 Z = M(w) 矩阵相对于基 (e_r)_{r \in R} 和 (g_t)_{t \in T} 和 Z_{li} = M(w_{li}) w_{li} 相对于基 (e_r)_{r \in R_i} 和 (g_t)_{t \in T_l}；那么从 (23) 可以得出，Z = YX 的子矩阵 Z_{li} 由下式给出

$$
Z_{li} = \sum_k Y_{lk} X_{kt}
$$

在其他字中，当定义了所有相关乘积时，一对一的对应（24）变换乘积进入乘积（矩阵的矩阵的乘积在no. 2的意义上定义， 注);当乘积YX的子矩阵Z_{li}被这样计算时，这个乘积被称为“在块中”执行。

这个名称的由来是，当 I = {1, p} 且 K = {1, q} 时，表示矩阵 X 的表被设想分为“块”，形成“矩阵的数组”

$$
\begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
X_{21} & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
X_{q1} & X_{q2} & \ldots & X_{qp}
\end{pmatrix}
$$

which is considered as a symbol denoting X when p and q are specific integers sufficiently small for this to be practicable.

### 6. 半线性映射的矩阵

设A，B为两个环，\sigma：A \to B 同态，A进入B，E为右（左）A-模与基（e_i）_{i \in I}，F为右（左）B-模与基 $(f_k)_{k \in K}$。令 $u : E \to F$ 为相对于 $\sigma$ 和 $u(e_i) = \sum_{k \in K} f_k u_{ki}$（分别为 $u(e_i) = \sum_{k \in K} u_{ki} f_k$）的*半线性* 映射，其中 $u_{ki}$ 因此是 B 的元素；由定义、型$K \times I$的矩阵$M(u) = (u_{ki})$相对于基*$(e_i)$和$(f_k)$也称为u的*矩阵。通过与no. 4的命题2相同的计算，立即验证对于所有$x \in E$，如果I和K是*有限*，

(26D)
$$
M(u(x)) = M(u) \cdot \sigma(M(x))
$$
（分别。

(26克)
$$
{}^t M(u(x)) = \sigma({}^t M(x)) \cdot {}^t M(u)).
$$

令C为第三个环，$\tau : B \to C$同态，G为右（或左）C-模，其中基$(g_l)_{l \in L}$和$v$为F到G相对于$\tau$的半线性映射；如果$M(v)$相对于$(f_k)$和$(g_l)$是$v$的矩阵，并且相对于$(e_i)$和$(g_l)$是$v \circ u$的$M(v \circ u)$矩阵，那么，如果I，K和L 是有限的，

(27D)
$$
M(v \circ u) = M(v) \cdot \tau(M(u))
$$
（分别。

（27克）
$$
{}^t M(v \circ u) = \tau({}^t M(u)) \cdot {}^t M(v)).
$$

要显示例 (27 D)、注，对于所有 $x \in E$，通过 (26 D)，
$$
M(v \circ u) \cdot \tau(\sigma(M(x))) = M(v(u(x)))
$$
$$
= M(v) \cdot \tau(M(u(x))) = M(v) \cdot \tau(M(u)) \cdot \tau(\sigma(M(x))),
$$
从而（27 天）由命题 1 个no. 3 完成。

最后假设$\sigma : A \to B$是*同构*；然后回想一下${}^t u : F^* \to E^*$是相对于$\sigma^{-1}$（§ 2, no. 5）的半线性映射；当I和K是有限的时，矩阵${}^t u$相对于对偶基$(f_k^*)$和$(e_i^*)$由下式给出

(28)
$$
M({}^t u) = \sigma^{-1}({}^t M(u))
$$
因为，根据定义，假设例 E 和 F 是正确的模，
$$
\langle {}^t u(f_k^*), e_i \rangle^\sigma = \langle f_k^*, u(e_i) \rangle
$$
当$\sigma$用$x \mapsto x^\sigma$表示时。

#### 注 {#alg-ii-s10-n6-rem-1 .statement tag=05WQ}

设 A 为环且 $\sigma$ A 的*反自同态* (no. 3)；考虑以下两种情况：

(GD) E 是左A-模、F 右A-模和 $u$ E 到 F 的 $\mathbf{Z}$ 线性映射，使得 $u(ax) = u(x)\sigma(a)$ 对于 $a \in A,\ x \in E$；在其他字中，$u$是相对于右侧$A^0$-模E到右A-模F的$\sigma$的*半线性*映射。

(DG) E 是右A-模、F 左A-模和 $u$ E 到 F 的 $\mathbf{Z}$ 线性映射，使得 $u(xa) = \sigma(a)u(x)$ 对于 $a \in A,\ x \in E$；在其他字中，$u$是相对于左侧$A^0$-模E到左A-模F的$\sigma$的*半线性*映射。

在这两种情况下，$u$相对于E和F的基的矩阵$M(u)$在A中具有元素；如果这些基是有限的，那么对于所有$x \in E$，我们有各自的公式

(17 GD) $$
M(u(x)) = M(u) . \sigma(M(x))
$$
(17 副总) $$
{}^t M(u(x)) = \sigma({}^t M(x)) . {}^t M(u),
$$
*在* A 中计算两侧的乘积。这分别紧随 (26 D) 和 (26 G) 得出。

### 7.方阵

#### 定义 4 {#alg-ii-s10-def-4 .statement tag=05WR}

*与列具有相同索引集合的行称为矩阵平方矩阵。*

具有 $n$ 行和 $n$ 列的平方矩阵称为阶* $n$ 的 *矩阵。

#### 注 {#alg-ii-s10-n7-rem-1 .statement tag=05WS}

应该注意的是，矩阵的行索引集合和列具有*相同的基数*但*不相同*，不能被视为平方矩阵；特别是，两个这样的矩阵超过环的乘积*未定义*。

显然，A 上的方阵的加法和乘法具有有限的集合作为行的索引集合，以及这些矩阵的集合上的列、定义 *环* 结构，因为公式 (7)、(8) 和 (9) (no. 3)； 矩阵$(\delta_{ij})$，其中$\delta_{ij}$是克罗内克指标（对于$i \in I, j \in I$），是环的单位元，当I时用$I_n$或$l_n$表示有 $n$ 元素。当$I = \{1, n\}$时，如此定义的矩阵中的环简称为$\mathbf{M}_n(A)$； $\mathbf{M}_n(A)$的可逆元的群用$\mathbf{GL}_n(A)$或$\mathbf{GL}(n, A)$表示。

为了使 A 上的阶 $n$ 的平方矩阵 $U = (a_{ij})$ 是右（或左）可逆的，有必要且充分的是，对于 A 的元素的每个系统 $(b_i)_{1 \leq i \leq n}$，系统 $n$ 未知数中的 $n$ 方程组

$$
\sum_{j=1}^n a_{ij} x_j = b_i \quad (1 \leq i \leq n)
$$

（分别$\sum_{j=1}^n x_j a_{ji} = b_i$）

A 中有*一个解* $(x_i)$。

令 I 为有限索引集合，A 环和 E 为右（左）A-模和基 $(e_i)_{i \in I}$。对于E的每个*自同态*$u$，$u$的矩阵$M(u)$相对于*$(e_i)$相同的两个基为平方矩阵；更简单地说，它被称为$u$*相对于基*$(e_i)$的矩阵。

假设$I = \{1, n\}$。 映射$u \mapsto M(u)$（分别$u \mapsto {}^t M(u)$）是环$\mathrm{End}_A(E)$到$\mathbf{M}_n(A)$（分别到$\mathbf{M}_n(A)$的逆环的*同构*，如下来自公式 （18 D）（分别为 18 G））（no. 4）。 环 $\mathbf{M}_n(\mathbf{A})$ 的可逆元称为*可逆矩阵*、对应在映射 $u \mapsto M(u)$（或$u \mapsto {}^t M(u)$）下到 E 的 *自同构*；因此，群 $\mathbf{GL}(n, \mathbf{A})$ 被规范地标识为群 $\mathbf{GL}(\mathbf{A}_d^n)$。

如果 $u$ 是 E 的自同构，则其*相反* $\check{u}$ 是左（右）A-模 $E^*$ 的自同构，使得 $\check{u} = ({}^t u)^{-1} = {}^t (u^{-1})$ (§ 2, no. 5, 定义 6)；如果$M(\check{u})$相对于对偶基$(e_i^*)$是$\check{u}$的矩阵，那么，凭借命题3（no. 4），

$$
M(\check{u}) = ({}^t M(u))^{-1} = {}^t M(u^{-1}).
$$

对于每个可逆矩阵 $X$，因此得出 ${}^t (X^{-1}) = ({}^t X)^{-1}$；这个矩阵也用${}^t X^{-1}$表示，称为矩阵$X$的*矛盾*。

令$\sigma$为环$\mathbf{A}$的*自同构*；对于相对于$\sigma$的每个*半线性*映射$u : E \to E$，此映射的矩阵$M(u)$相对于E的基$(e_i)$也是平方矩阵。从 (27 D) (no. 6) 可以立即得出，如果 $u$ 是双射的，那么

$$
M(u^{-1}) = (\sigma^{-1}(M(u)))^{-1}.
$$

设E为A-模，它是子模的有限族$(E_i)_{i \in I}$的*直和*；对于E的每一个自同态$u$，$u$的矩阵$M(u) = (u_{ki})$，对于E中与$(E_i)$（no. 5）相同的两个分解来说，是一个*平方矩阵线性映射*。在阶中，$u(E_i) \subset E_i$对于所有$i \in I$，$u_{ki} = 0$对于$k \neq i$是必要且充分的。当$I = \{1, n\}$、关系时

$$
u(E_i) \subset E_i + E_{i+1} + \cdots + E_n \qquad (1 \leq i \leq n)
$$

相当于$k < i$的关系$u_{ki} = 0$。

*例共方阵。*I。 *对角线矩阵*。在平方矩阵

$$
M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times I},
$$

与指标相等的元素称为*对角线元素*，$(m_{\iota \iota})_{\iota \in I}$族称为$M$的*对角的*； 平方矩阵 $M = (m_{\iota \kappa})$超过环，其元素除对角线元素外均为零，称为*对角矩阵*。对于环$\mathbf{A}$、对角矩阵$(m_{\iota \kappa})$的元素的每个家庭$(a_\iota)_{\iota \in I}$，使得所有$\iota \in I$的$m_{\iota \iota} = a_\iota$由$\operatorname{diag}(a_\iota)_{\iota \in I}$表示（或$\operatorname{diag}(a_1, a_2, \ldots, a_n)$，当$I = \{1, n\}$）。 $\mathbf{A}$以上阶$n$方阵集合$\mathbf{M}_n(\mathbf{A})$，单位矩阵$I_n$为对角矩阵以及每倍数这个矩阵的$a I_n = I_n a$由标量$a$（对角矩阵（称为*标量*），其所有对角线元素等于$a$）。

对于$\mathbf{A}$的元素的每个家庭$(d_i)_{1 \leq i \leq n}$和型$(n, q)$（分别为$(p, n)$）超过$\mathbf{A}$的每个矩阵$X = (x_{ij})$，写下$D = \operatorname{diag}(d_i)$，

$$
\begin{cases}
DX = (d_i x_{ij}) \\
XD = (x_{ij} d_j).
\end{cases}
$$

特别是，对于阶 $n$ 的两个对角线矩阵，

$$
\text{diag}(a_i) + \text{diag}(b_i) = \text{diag}(a_i + b_i)
$$
(31)
$$
\text{diag}(a_i) \cdot \text{diag}(b_i) = \text{diag}(a_i b_i).
$$

The diagonal matrices therefore form a subring of $\mathbf{M}_n(\mathbf{A})$ isomorphic to the product ring $\mathbf{A}^n$; the scalar matrices form a subring isomorphic to $\mathbf{A}$.

II。 *置换矩阵；单项式矩阵。*令$\pi$为有限集合$\mathbf{I}$的任意*置换*，并令$(e_i)_{i \in \mathbf{I}}$为$\mathbf{A}$模$\mathbf{E} = \mathbf{A}_d^\mathbf{I}$的典范基； $\mathbf{E}$中存在且仅有一个自同态$u_\pi$，使得对于所有$i \in \mathbf{I}$，$u_\pi(e_i) = e_{\pi(i)}$（§ 1, no. 11，推论3到命题17）。对于所有$i \in \mathbf{I}$，矩阵$M(u_\pi)$中的指标$i$的列相对于基$(e_i)$拥有除指标行中的所有元素零之外的所有元素零 $\pi(i)$，等于 1。通过滥用语言，$M(u_\pi)$ 被称为置换* $\pi$ 的 *矩阵。 直接的，对于$\mathbf{I}$，$u_{\sigma \tau} = u_\sigma \circ u_\tau$中的任意两个置换$\sigma, \tau$，对于恒等式置换$\varepsilon$，$u_\varepsilon$是恒等式；因此，映射$\pi \mapsto M(u_\pi)$是群$\mathfrak{S}_\mathbf{I}$到置换矩阵的对称群的*同构的*。

每行和置换矩阵包含中的每个列只有一个元素$\neq 0$。非零环 $\mathbf{A}$ 上的有限平方矩阵 $R$，以及性质，称为*单项式矩阵*；令指标$i$的$R$列中的$r_i$为唯一元素$\neq 0$，并令$\pi(i)$为该元素所在行的指标；显然，$\pi$是索引集合$\mathbf{I}$和$R = M(u_\pi)D$的置换，其中$D = \text{diag}(r_i)$。

III。 *三角形矩阵。*在阶$n$的方阵的环$\mathbf{M}_n(\mathbf{A})$超过环$\mathbf{A}$，任何矩阵$(a_{ij})$使得$a_{ij} = 0$对于$i > j$ （分别$i < j$）被称为*上*（分别*下*）*三角形矩阵*；也有人说这样的矩阵*只有零低于*（或*以上*）*其对角线*。立即确定，$\mathbf{M}_n(\mathbf{A})$的上（或下）三角形矩阵形式子环$S$（或$T$），$S \cap T$显然是对角线矩阵的环。

The set $S'$ (resp. $T'$) of matrices in $S$ (resp. $T$) whose diagonal elements are *invertible* is a multiplicative *group* of matrices called the *upper* (resp. *下*）*总三角形群*，紧随§ 1, no. 11，*注* 5。 The set $S_1$ (resp. $T_1$) of matrices in $S$ (resp. $T$) whose diagonal elements are all equal to 1 is a *subgroup* of the above group, called the *upper* (resp. *下*) *严格的三角形群*，以及每个对角线为$(d_i)$的矩阵$M \in S'$（分别为$M \in T'$），可以写成$M = DM_1 = M'_1D$，其中$D = \text{diag}(d_i)$和$M_1$和$M'_1$矩阵属于至 $S_1$（分别为 $T_1$）。

IV。 *矩阵的对角线和三角形矩阵。*令$(I_k)_{1 \leq k \leq p}$为有限集合$\mathbf{I}$的划分； 平方矩阵超过环 $\mathbf{A}$ 且具有索引集合 $\mathbf{I}$ 都可以写在矩阵* 相应的的 *平方矩阵的形式中行索引集合的划分 $(\mathbf{I}_k)$ 以及列 (no. 5) 的索引集合

$$
(32)
\begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
X_{21} & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
X_{p1} & X_{p2} & \ldots & X_{pp}
\end{pmatrix}
$$

其中每个$X_{kk}$是平方矩阵，其中$\mathbf{I}_k$作为行的索引集合和列。

有了这个记号，如果所有矩阵$X_{ij}$使得$i \neq j$（$i > j$，$i < j$）都是零，则（32）将被称为矩阵的对角线（分别是上三角，分别是下三角）矩阵。 自同态 $u$ 的解释，其矩阵分别是对角线。三角形，通过考虑线性映射的相应的矩阵 $M(u)$，之前已经看到了矩阵的矩阵。 The lower triangular (resp. upper triangular, diagonal) matrices of matrices for a given partition $(\mathbf{I}_k)$ of I form subrings of the ring of matrices $\mathbf{A}^{I \times I}$. 特别地，矩阵的对角线矩阵相对于划分$(\mathbf{I}_k)$的环与乘积$\prod_{k=1}^p \operatorname{End}_\mathbf{A}(E_k)$同构的。

### 8. 变换的基

#### 命题 4 {#alg-ii-s10-prop-4 .statement tag=05WT}

*设 E 为右A-模，且基 $(e_i)_{1 \leq i \leq n}$ 为 n 元素。对于 n 元素 $e'_i = \sum_{j=1}^n e_j a_{ji} (1 \leq i \leq n)$ 的族是 E 的基，阶 n 的平方矩阵 $P = (a_{ji})$ 可逆是必要且充分的。*

相对于$u(e_i) = e'_i (1 \leq i \leq n)$定义的E的自同态$u$的基$(e_i)$，$P$只是矩阵。现在，要使$u$成为E的自同构，$(u(e_i))$成为E的基是充分必要的（§ 1, no. 11，推论3到命题17）； 从而命题。

可逆的矩阵$P$称为从基*$(e_i)$*到基*$(e'_i)$的通道*矩阵。它也可以解释为恒等映射$l_E$相对于基$(e'_i)$和$(e_i)$的矩阵（*其中阶*）；那么显然，从基* $(e'_i)$ *到基* $(e_i)$的通道矩阵是$P$的*逆*$P^{-1}$。

#### 命题 5 {#alg-ii-s10-prop-5 .statement tag=05WU}

*设$(e_i), (e'_i)$为从$(e_i)$到$(e'_i)$的通道的E和P矩阵的n元素中的两个基。如果$(e_i^*)$和$({e'_i}^*)$分别是$(e_i)$和$(e'_i)$的对偶基，则从$(e_i^*)$到$({e'_i}^*)$的矩阵就是P的同余$^tP^{-1}$。

The transpose of the identity mapping $l_E$ is the identity mapping $l_{E^*}$; by Proposition 3, no. 4, the matrix of $l_{E^*}$ with respect to the bases $({e'_i}^*)$ and $(e_i^*)$ (in that order) is the transpose of the matrix of $l_E$ with respect to the bases $(e_i)$ and $(e'_i)$ (in that order), that is the transpose of $P^{-1}$.

#### 命题 6 {#alg-ii-s10-prop-6 .statement tag=05WV}

*Let E and F be two right A-modules, $(e_i)$ and $(e'_i)$ two bases of E* with $n$ elements, $(f_j)$ and $(f'_j)$ two bases of $F$ with $m$ elements, $P$ the matrix of passage from $(e_i)$ to $(e'_i)$ and $Q$ the matrix of passage from $(f_j)$ to $(f'_j)$. 对于$E$的每个线性映射$u$进入$F$，令$M(u)$是$u$的矩阵，相对于基$(e_i)$和$(f_j)$和$M'(u)$矩阵 $u$相对于基$(e'_i)$和$(f'_j)$；然后

$$
M'(u) = Q^{-1} M(u) P.
$$

我们可以写$u = l_F \circ u \circ l_E$。 Formula (33) follows immediately from no. 4, Corollary to Proposition 2 when the matrix of $l_E$ is taken with respect to $(e'_i)$ and $(e_i)$, that of $u$ with respect to $(e_i)$ and $(f_i)$ and that of $l_F$ with respect to $(f_i)$ and $(f'_j)$.

#### 推论 1 {#alg-ii-s10-prop-6-cor-1 .statement tag=05WW}

*如果$u$是$E$、$M(u)$和$M'(u)$的自同态，分别相对于基、$(e_i)$和$(e'_i)$，则矩阵，则*

$$
M'(u) = P^{-1} M(u) P.
$$

#### 推论 2 {#alg-ii-s10-prop-6-cor-2 .statement tag=05WX}

*如果$M(x)$和$M'(x)$分别相对于基$(e_i)$和$(e'_i)$为矩阵，其中一个列具有相同的元素$x \in E$，则*

$$
M(x) = P . M'(x).
$$

这是命题 6 的特例，应用于 $A_d$ 到 $E$ 的映射 $\theta_x : a \mapsto xa$（no. 4，*注 1*）。

公式 (35) 等价于

$$
x_i = \sum_{j=1}^n a_{ij} x'_j \quad (1 \leq i \leq n)
$$

分别为元素 $x_i$ 和 $x'_i$ 矩阵 $M(x)$ 和 $M'(x)$。 公式(36D)称为坐标*变换*公式。观察它们将$x$相对于“旧”基$(e_i)$的分量表示为$x$相对于“新”基的分量函数，$(e'_i)$和元素的$P$的分量，即“新”基相对于“旧”基。

#### 注 {#alg-ii-s10-n8-rem-1 .statement tag=05WY}

(1) 我们现在从一个*左* $A$-模块$E$开始，其中有两个基$(e_i), (e'_i)$，每个$n$元素；如果我们写$e'_i = \sum_{j=1}^n a_{ji} e_i$，$P = (a_{ji})$也称为经过*的*矩阵，从$(e_i)$到$(e'_i)$；它也是$E$的自同构的矩阵，使得对于基$(e_i)$而言$u(e_i) = e'_i$，对于基$(e'_i)$和$(e_i)$也是$l_E$的矩阵 *在那阶*。上述结果只需进行以下修改即可成立： 公式 (33 D) 至 (36 D) 分别替换为

$$
\begin{align*}
(33\text{ G}) &\quad {}^t M'(u) = {}^t P . {}^t M(u) . {}^t Q^{-1} \\
(34\text{ G}) &\quad {}^t M'(u) = {}^t P . {}^t M(u) . {}^t P^{-1} \\
(35\text{ G}) &\quad {}^t M(u) = {}^t M'(u) . {}^t P.
\end{align*}
$$

线性代数

(36克)
$$
x_i = \sum_{j=1}^n x_j' a_{ij} \quad (1 \leq i \leq n).
$$

（2）在命题4的假设下，考虑元素$x^* \in \mathbf{E}^*$；因为从$(e_i^*)$到$(e_{i'}^*)$的路径矩阵是$tP^{-1}$（命题5），对于这两个基，分别为$x^*$的矩阵、$M(x^*)$和$M'(x^*)$，

$$
tM(x^*) = tM'(x^*) . P^{-1}
$$

或者也

(37D)
$$
tM'(x^*) = tM(x^*) . P
$$

相当于方程的系统

(38D)
$$
x_{i'}^* = \sum_{j=1}^n x_j^* a_{ji} \quad (1 \leq i \leq n)
$$

对于元素$(x_i^*)$和$(x_{i'}^*)$共矩阵$M(x^*)$和$M'(x^*)$。 相应的公式左A-模 E 是

（37克）
$$
M'(x^*) = tP . M(x^*)
$$

(38克)
$$
x_{i'}^* = \sum_{j=1}^n a_{ji} x_j^* \quad (1 \leq i \leq n).
$$

(3) 设A、B为A的两个环、$\sigma : A \to B$同态到B、E的右（左）A-模、$(e_i)$、$(e_i')$两个基与E、F的右（左）$n$元素 B-模、$(f_j)$、$(f_j')$ 两个基以及 F 的 $m$ 元素和 $P$（分别为 $Q$）矩阵从 $(e_i)$ 到 $(e_i')$（分别从$(f_j)$至$(f_j')$）。

对于每个半线性映射$u : E \to F$，相对于$\sigma$，令$M(u)$为$u$相对于$(e_i)$和$(f_j)$的矩阵，$M'(u)$相对于$(e_i')$的矩阵和$(f_j')$。然后

（39D）
$$
M'(u) = Q^{-1} M(u) \sigma(P)
$$
（分别。
（39克）
$$
tM'(u) = \sigma(tP) . tM(u) . tQ^{-1}.
$$

证明与 (33 D) 和 (33 G) 相同，这次使用公式 (27 D) 和 (27 G) (no. 6)。

### 9. 相当于矩阵；类似矩阵

#### 定义 5 {#alg-ii-s10-def-5 .statement tag=05WZ}

*如果存在阶 m 的可逆平方矩阵* $P$ *和可逆平方，则两个矩阵* $X, X'$ *具有 m 行和 n 列超过环被称为等效矩阵* $Q$ *阶 n 这样*

(40)
$$
X' = PXQ.
$$

显然关系“X和X'是等价的”在A上型$(m, n)$的矩阵集合$A^{mn}$上等价关系（集合理论，II, § 6, no. 1），这证明术语是合理的。

由此，定义、no. 8的命题 6 可以用说来表示，当基改变为两个右A-模E、F（其中有限基）时，线性映射$u : E \to F$的矩阵新的基相当于$u$的矩阵相对于旧的基。

相反，如果关系 (40) 成立且 $u : A_d^n \to A_d^m$ 为线性映射，其中矩阵为 $X$，相对于 $A_d^n$ 和 $A_d^m$ 各自的规范基 $(e_i)$ 和 $(f_j)$，则$X'$是$u$相对于基$(e'_i)$和$(f'_j)$的矩阵，使得$Q$是从$(e_i)$到$(e'_i)$和$P^{-1}$的矩阵从 $(f_j)$ 到 $(f'_j)$ 的矩阵。

例相当于矩阵。 (1) 如果存在 $\mathbf{N}$ 的区间 $[1, m]$ 的置换 $\sigma$，则两个矩阵 $X = (x_{ij})$ 和 $X' = (x'_{ij})$ 具有 $m$ 行和 $n$ 列“仅在阶行中不同”，这样对于指标$(i, j)$的每个有序对，$x'_{ij} = x_{\sigma(i), j}$（我们也说$X'$是通过对$X$的行执行置换$\sigma^{-1}$获得的）。对于 $X' = PX$，矩阵 $X$ 和 $X'$ 是等价的，其中 $P$ 是置换 $\sigma^{-1}$ 的矩阵 (cf. no. 7, 例) II）。

类似地，如果存在$[1, n]$的置换$\tau$，使得$x'_{ij} = x_{i, \tau(j)}$对于指标的每个有序对，则据说$X$和$X'$仅在列的阶有所不同$(i, j)$、$X$ 和 $X'$ 也等效，对于 $X' = XQ$，其中 $Q$ 是置换 $\tau$ 的矩阵。

注上述中的记号 $P$ 是从基 $(f_j)_{1 \leq j \leq m}$ 到基 $(f_{\sigma^{-1}(j)})_{1 \leq j \leq m}$ 的通道矩阵以及从基的$Q$ 矩阵 $(e_i)_{1 \leq i \leq n}$ 至基 $(e_{\tau(i)})_{1 \leq i \leq n}$。

(2) 令$j, k$不同于元素与$[1, n]$，并令$a \in A$。

假设对于$1 \leq i \leq m$，$x'_{ij} = x_{ij} + x_{ik}a$和$x'_{il} = x_{il}$对于$j \neq l$和$1 \leq i \leq m$；据说$X'$是由$X$通过添加指标$j$列的$X$的列加上指标$k$的右侧乘以$a$而得。在这种情况下，$X$和$X'$也是等价的：因为如果$Q = I_n + aE_{kj}$（可倒三角形矩阵，如no. 7所示），则$X' = XQ$。

类似地，令$h, i$是$[1, m]$的两个不同的元素和$a$元素的$A$；如果 $X'$ 是从 $X$ 导出的，通过将指标 $i$ 的 $X$ 行添加到指标 $h$ 行左侧乘以 $a$，则 $X$ 和 $X'$ 是等价的，对于$X' = PX$，其中$P = I_m + aE_{ih}$。

(3) 最后，如果对于给定的指标$j$，$x'_{ij} = x_{ij}c$对应于$1 \leq i \leq m$，其中$c$是可逆的，$x'_{il} = x_{il}$对应于$1 \leq i \leq m$和$l \neq j$，$X$和$X'$是等价的；对于$X' = XQ$，其中$Q$是矩阵$\operatorname{diag}(a_k)$，$a_j = c$，$a_k = 1$对于$k \neq j$。那么$X'$据说是由$X$通过将右侧的指标$j$的$X$的列乘以$a$得出。

类似地，如果$X'$是由$X'$通过将左侧指标$i$的$X$行乘以可逆元$c \in A$得出，$X'$和$X$是等价的，对于$X' = PX$，其中$P$ 是矩阵 $\operatorname{diag}(b_h)$ 与 $b_i = c$，$b_h = 1$ $h \neq i$。

#### 定义 6 {#alg-ii-s10-def-6 .statement tag=05X0}

*如果存在阶 n 的可逆平方矩阵 P，则环 A 上的阶 n 的两个方阵 X、X' 被称为相似*

$$(41)$$
$$X' = PXP^{-1}$$

显然，关系“X和X'相似”是$M_n(A)$上的*等价关系*，这意味着X和X'通过这个环的*内自同构*转换为一个另一个。

有了这个定义，no. 8的推论1到命题6可以用说来表示，当A-模E（具有有限的基）的基改变时，自同态u的矩阵新的基与旧的基相比，与u的矩阵*相似。

#### 注 {#alg-ii-s10-n9-rem-1 .statement tag=05X1}

(1) 两个仅在阶行（或列的阶）不同的方阵是等价的，但一般来说*不相似*。 矩阵类似于平方矩阵 $X = (x_{ij})$ 可以通过对行和列执行*相同的置换* $\sigma^{-1}$ 来获得，即考虑矩阵 $X' = (x'_{ij})$，其中每有序对指标 $x'_{ij} = x_{\sigma(i), \sigma(j)}$；因为如果相对于基$(e_i)_{1 \leq i \leq n}$，X是$A^n_d$的自同态u的矩阵，$X'$相对于基$(e_{\sigma(i)})_{1 \leq i \leq n}$是u的矩阵。

(2) 设X和$X'$为阶n中的两个方阵，可写成方阵的对角线矩阵的形式(no. 7，例IV)：

$$
X = \begin{pmatrix}
X_1 & 0 & \ldots & 0 \\
0 & X_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X_p
\end{pmatrix}
\qquad
X' = \begin{pmatrix}
X'_1 & 0 & \ldots & 0 \\
0 & X'_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X'_p
\end{pmatrix}
$$

相应的与 X 和 $X'$ 的索引集合 $[1, n]$ *相同* 划分。如果，对于 $1 \leq i \leq p$，$X_i$ 和 $X'_i$ 等价（或类似），则 X 和 $X'$ 等价（或类似）： 对于，如果 $X'_i = P_i X_i Q_i$ 对于 $1 \leq i \leq p$，则 $X' = PXQ$ 其中

$$
P = \begin{pmatrix}
P_1 & 0 & \ldots & 0 \\
0 & P_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & P_p
\end{pmatrix}
\qquad
Q = \begin{pmatrix}
Q_1 & 0 & \ldots & 0 \\
0 & Q_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Q_p
\end{pmatrix}
$$

计算“块”乘积（no. 6）如下。此外，如果$Q_i = P_i^{-1}$对于所有i，则$Q = P^{-1}$。

### 10.张量积矩阵超过交换环

令C为交换环、E、F、U、V四个C-模块和$\phi : E \to U$、$\psi : F \to V$两个C-线性映射。假设E、F、U、V分别有有限基$(e_\lambda)_{\lambda \in L}, (f_\mu)_{\mu \in M}, (u_\rho)_{\rho \in R}, (v_\sigma)_{\sigma \in S}$；对于$(e_\lambda)$和$(u_\rho)$，令$A = (a_{\rho \lambda})$为$\phi$的矩阵，对于$(f_\mu)$和$(v_\sigma)$，$B = (b_{\sigma \mu})$为$\psi$。对于每个有序对 $(\lambda, \mu) \in L \times M = N$，令 $g_{\lambda \mu} = e_\lambda \otimes f_\mu$；对于每个有序对 $(\rho, \sigma) \in R \times S = T$ 让 $w_{\rho \sigma} = u_\rho \otimes v_\sigma$； $g_{\lambda \mu}$ 然后 $E \otimes F$ 的形式基以及 $U \otimes V$ 的 $w_{\rho \sigma}$ 基（§ 3, no. 6，推论 2 到命题 7）。 $A$ 与 $B$ 的 *张量积*（记为 $A \otimes B$）为矩阵 $X = (x_{\tau v})_{(\tau, v) \in T \times N}$，其中元素由下式给出

$$
x_{(\rho, \sigma), (\lambda, \mu)} = a_{\rho \lambda} b_{\sigma \mu}.
$$

那么$A \otimes B$是*$\phi \otimes \psi$*相对于基*$(g_{\lambda \mu})$*和*$(w_{\rho \sigma})$的*矩阵。 定义 (§ 3, no. 2, 公式 (3))

$$
\begin{align*}
(\phi \otimes \psi)(g_{\lambda \mu}) &= (\phi \otimes \psi)(e_\lambda \otimes f_\mu) = \phi(e_\lambda) \otimes \psi(f_\mu) \\
&= \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} (u_\rho \otimes v_\sigma) = \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} w_{\rho \sigma}.
\end{align*}
$$

$A \otimes B$的元素的定义(42)表明，该矩阵对应与矩阵$(a_{\rho \lambda} B)_{(\rho, \lambda) \in R \times L}$的矩阵以及矩阵$(A b_{\sigma \mu})_{(\sigma, \mu) \in S \times M}$(no. 5)双射。

事实上，$(\phi, \psi) \mapsto \phi \otimes \psi$是C双线性映射以及§ 3, no. 5的公式(9)，可以用恒等式来表示

$$
\begin{align*}
(A \otimes (B_1 + B_2)) &= A \otimes B_1 + A \otimes B_2 \\
((A_1 + A_2) \otimes B) &= A_1 \otimes B + A_2 \otimes B
\end{align*}
$$
(43)

$$(cA) \otimes B = A \otimes (cB) = c(A \otimes B) \quad \text{for } c \in \mathbf{C}$$
(44)

$$(A_1 \otimes B_1)(A_2 \otimes B_2) = (A_1 A_2) \otimes (B_1 B_2)$$
(45)

当运算出现时被定义。 矩阵张量积转置由下式给出

$$(A \otimes B)^t = (A^t) \otimes (B^t).$$
(46)

如果 $A$ 和 $B$ 可逆方阵超过 $\mathbf{C}$，则 $A \otimes B$ 可逆且

$$(A \otimes B)^{-1} = (A^{-1}) \otimes (B^{-1}).$$
(47)

设$(e'_\lambda)_{\lambda \in L}$为$E$的另一个基和$F$的$(f'_\mu)_{\mu \in M}$另一个基；如果$P$是从基$(e_\lambda)$到基$(e'_\lambda)$的通道的矩阵和从基$(f_\mu)$到基$(f'_\mu)$的通道$Q$矩阵，从基$(e_\lambda \otimes f_\mu)$到基$(e'_\lambda \otimes f'_\mu)$经过的矩阵是$P \otimes Q$。如果 $A'$ 与 $A$ *等价*（或 *相似*），并且 $B'$ *等价*（或 *相似*）至 $B$，则 $A' \otimes B'$ 与 $A \otimes B$ *等价*（或 *相似*）。

矩阵的张量积的定义可以以明显的方式推广到$\mathbf{C}$上矩阵的任意有限数；特别是我们有结合性公式

$$
\left( \bigotimes_{i \in I_1} X_i \right) \otimes \left( \bigotimes_{i \in I_2} X_i \right) = \bigotimes_{i \in I} X_i
$$

对于有限索引集合 $I$ 的每个 *划分* $(I_1, I_2)$。

### 11. 矩阵的踪迹

设 $C$ 是一个*可交换的* 环；对于每个平方矩阵$X = (x_{ij})$超过$C$相应的到有限索引集合$I$，$X$的*迹*是元素

$$
\operatorname{Tr}(X) = \sum_{i \in I} x_{ii}.
$$

设 $E$ 为 $C$ 模，承认有限基 $(e_i)_{i \in I}$；对于 $E$ 中的每自同态 $u$，

$$
\operatorname{Tr}(u) = \operatorname{Tr}(M(u))
$$

相对于基$(e_i)$，$M(u)$为矩阵$u$；当这个公式应用于自同态$x \mapsto \langle x, e_i^*\rangle e_j$（其中$e_i^*$）是$(e_i)$的对偶基时，这立即从§ 4, no. 3，公式（17）开始；由此我们通过线性传递到一般情况。 公式 (49) 表明

$$
\operatorname{Tr}(u) = \sum_i \langle u(e_i), e_i^* \rangle
$$

对于 $E$ 中的每个基 $(e_i)$ (cf. § 4, no. 3, 公式 (17))。

如果$X$是$C$上型$(m, n)$的矩阵，并且$C$上型$(n, m)$的$Y$矩阵，则

$$
\operatorname{Tr}(XY) = \operatorname{Tr}(YX)
$$

由上述和§ 4, no. 3中的命题3如下； (52) 也可以直接求得，若 $X = (x_{ij}), Y = (y_{ji})$ ($1 \leq i \leq m, 1 \leq j \leq n$)，则

$$
\operatorname{Tr}(XY) = \sum_{i,j} x_{ij} y_{ji}
$$

由（49）。后者公式还证明：

#### 命题 7 {#alg-ii-s10-prop-7 .statement tag=05X2}

*令$C$为交换环，对于每个矩阵$P \in \mathbf{M}_n(C)$，让$f_P$在$\mathbf{M}_n(C)$上为线性形式$X \mapsto \operatorname{Tr}(PX)$； 映射 $P \mapsto f_P$ 是 $\mathbf{M}_n(C)$ 的 $C$ 线性双射到其对偶上。*

#### 命题 8 {#alg-ii-s10-prop-8 .statement tag=05X3}

*如果$C$模块$\mathbf{M}_n(C)$上的$g$为线性形式，使得$g(XY) = g(YX)$对于$\mathbf{M}_n(C)$中的所有矩阵$X, Y$，则存在且仅有一个标量$c \in C$，使得$g(X) = c \cdot \operatorname{Tr}(X)$对于每个矩阵 $X \in \mathbf{M}_n(C)$.*

由于命题对于$n = 1$来说是微不足道的，因此注意力可能仅限于$n \geqslant 2$的情况。将$X = E_{ij},\ Y = E_{jk}$与$i \neq k$相乘，得到$g(E_{ik}) = 0$；然后用$X = E_{ij},\ Y = E_{ji}$和$i \neq j$，我们找到$g(E_{ii}) = g(E_{jj})$； 命题紧随$\mathbf{M}_n(\mathbf{C})$的$E_{ij}$形式基之后。

### 12.矩阵超过域

The finite matrices with $m$ rows and $n$ columns over a field $K$ are in one-to-one correspondence with the linear mappings of the right vector space $E = K_d^n$ into the right vector space $K_d^m$ when the matrices of these mappings are taken with respect to the canonical bases of $E$ and $F$. 由定义，这样的矩阵$X$的*秩*对其来说是线性映射$u : E \to F$相应的的秩；因为这个数是由$F$的子空间$u(E)$定义维数，所以它是相同的（识别$X$的列与典范基的$u$下的像） $E$）给出以下定义：

#### 定义 7 {#alg-ii-s10-def-7 .statement tag=05X4}

*Given a matrix $X$ with $m$ rows and $n$ columns over a field $K$, the dimension of the subspace of $K_d^m$ generated by the $n$ columns of $X$ is called the rank of $X$ with respect to $K$ and denoted by $\operatorname{rg}(X)$.*

也可以说，$X$的秩是$X$*线性无关的列的*最大值数（如$K_d^m$的元素）。显然$\operatorname{rg}(X) \leqslant \inf(m, n)$；对于 $X$、$\operatorname{rg}(Y) \leqslant \operatorname{rg}(X)$ 的每个子矩阵 $Y$。

如果$E$和$F$是$K$和$E$的$u$线性映射到$F$的两个有限维向量空间，则矩阵$M(u)$的秩相对于任意两个基等于秩共 $u$。

#### 命题 9 {#alg-ii-s10-prop-9 .statement tag=05X5}

*如果矩阵 $X$ 中的元素具有 $m$ 行以及 $n$ 列属于至子域 $K_0$ 域 $K$，秩的$X$相对于$K_0$等于$X$相对于$K$的秩。*

设$F_0$为右向量$K$-空间$E = K_d^m$的典范基生成的右向量$K_0$-空间；由假设列至 $X$ 属于至 $E_0$。令$V_0$（或$V$）为由这些列生成的$F_0$的向量子$K_0$空间（或向量$E$的子$K$空间）。然后是 $V = V_0 \otimes_{K_0} K$ (§ 8, no. 2, 命题 2)，因此是 $\dim_K V = \dim_{K_0} V_0$。

#### 命题 10 {#alg-ii-s10-prop-10 .statement tag=05X6}

*矩阵$X$超过域$K$的秩等于其转置${}^t X$的秩超过相反的域$K^0$。*

在记号引入之前定义7中，$u$的秩等于${}^t u$（§ 7, no. 5，命题10），命题因此从no. 4，命题3得出。

由此可见，$X$的秩也可以定义为$X$*的线性独立行的*最大数（将它们视为左侧向量$K$-空间$K_s^n$的元素）。

阶 $n$ 的方阵在域 $K$ 对应上双射，与 $E = K_d^n$ 的自同态和形式环同构于环

结束$_{\mathbf{K}}$ (E) (no. 7); E 的相应的到自同构是可逆的方阵。

#### 命题 11 {#alg-ii-s10-prop-11 .statement tag=05X7}

*设X为阶n除以域K的平方矩阵。以下属性是等效的：*

(a) *X 在 $\mathbf{M}_n(\mathbf{K})$ 中可逆。*
(b) *X 在 $\mathbf{M}_n(\mathbf{K})$ 中是右可逆的。*
(c) *X 在 $\mathbf{M}_n(\mathbf{K})$ 中可逆。*
(d) *X 属于秩 n.*

这只是 § 7, no. 4 的翻译，是命题 9 的推论。

#### 命题 12 {#alg-ii-s10-prop-12 .statement tag=05X8}

*对于 n 个未知数中 m 个线性方程的系统*

$$
\sum_{j=1}^n a_{ij} x_j = b_i \quad (1 \leq i \leq m)
$$

*在域 K 上至少有一个解，系统和矩阵 B 的矩阵 $A = (a_{ij})$ 是必要且充分的，通过将 A 与第 $(n+1)$ 列接壤而获得，等于 $(b_i)$，为相同的矩阵秩.*

可知(no. 4)，(54)中解的存在性等价于列$(b_i)$是$A$的列的线性组合和命题，因此从§ 7, no. 3推出推论4到命题4。

当$m = n$和$A$可逆时，注总是满足命题12的条件，即秩$n$（命题11）。如果$x$和$b$分别用1个列、$(x_i)$和$(b_i)$表示矩阵，则系统(54)等价于$A.x = b$，其唯一的解为$x = A^{-1}.b$。

### 13.等价矩阵超过域

#### 命题 13 {#alg-ii-s10-prop-13 .statement tag=05X9}

*设E、F为域K上的两个有限维向量空间。如果$u : E \to F$是秩r的线性映射，则存在E和F的基，使得对于这些基，

$$
M(u) = \begin{pmatrix} I_r & 0 \\ 0 & 0 \end{pmatrix}.
$$

K 上的型 $(m, n)$ 和秩 r 的每个矩阵相当于形式 (55) 的矩阵。*

第二个断言与第一个基本等价。为了显示后者，让$\dim E = n$，$\dim F = m$。 核 $N = u^{-1}(0)$ 是维数 $n - r$ (§ 7, no. 4, 公式 (11))；令V为E中N的子空间和E中的$(e_i)_{1 \leq i \leq n}$基的补充，使得$(e_i)_{1 \leq i \leq r}$是V的基和N的$(e_i)_{r+1 \leq i \leq n}$基。则$u(e_j)$ $(1 \leq j \leq r)$形式基共$u(E)$；因此，存在 F 的基 $(f_j)_{1 \leq j \leq m}$，使得 $1 \leq j \leq r$ (§ 7, no. 1, 定理 2) 具有 $f_j = u(e_j)$，并且显然关于基 $(e_i)$ 和 $(f_j)$ 矩阵 $M(u)$由 (55) 给出。

#### 推论{#alg-ii-s10-n13-cor-1 .statement tag=05XA}

*对于型$(m, n)$中的两个矩阵超过域，要等价，它们具有相同的秩是必要且充分的。*

我们现在将通过另一个更明确地方法恢复命题13。对于$[1, m]$中*不同*整数$i, j$的每个环$A$、每个$\lambda \in A$、每个整数$m > 1$和每个有序对，我们写

$$
B_{ij}(\lambda) = I_m + \lambda E_{ij}
$$

阶 $m$乘no. 8的可逆矩阵。

#### 引理 1 {#alg-ii-s10-lem-1 .statement tag=05XB}

*设$X = (\xi_{ij})$为型$(m, n)$除环$A$中的矩阵。假设$m \geqslant 2$，并且在$X$的第一个列中存在元素$\xi_{i1}$，它在$A$中可逆。那么在$A$上存在型$(m - 1, n - 1)$的两个可逆方阵$P \in \mathbf{M}_m(A)$、$Q \in \mathbf{M}_n(A)$和矩阵$Y$，使得$P$（分别为$Q$）为乘积矩阵形式 $B_{ij}(\lambda)$ 阶 $m$（或$n$）和*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 \\
0 & & & \\
\vdots & & Y & \\
0 & & &
\end{pmatrix}.
$$

The matrix $B_{ij}(\lambda)X$ is obtained by adding to the row of $X$ of index $i$ the row of index $j$ multiplied on the left by $\lambda$ (no. 9, *Example 2*); if $\xi_{i1}$ is invertible, then there exists $\lambda \in A$ such that, for the matrix $X' = B_{1i}(\lambda)X = (\xi'_{kl})$, $\xi'_{11} = 1$; multiplying $X'$ on the left by suitably chosen matrices $B_{k1}(\mu_k)$ of order $m$ (for $1 \leq k \leq m$), a matrix $X'' = (\xi''_{kl})$ is obtained such that $\xi''_{j1} = 1$, $\xi''_{k1} = 0$ for $k \neq 1$. 然后将得到的矩阵依次*在右边*乘以阶$n$$(2 \leq j \leq n)$的合适的矩阵$B_{1j}(v_j)$，得到形式(57)的矩阵。

#### 命题 14 {#alg-ii-s10-prop-14 .statement tag=05XC}

*设$X$为型$(m, n)$除域$K$中的矩阵。如果$X$是秩$r$，则存在两个可逆的方阵$P \in \mathbf{M}_m(K)$、$Q \in M_n(K)$，使得$P$（或$Q$）是阶的矩阵的乘积形式 $B_{ij}(\lambda)$ 中的$m$（分别为$n$）和*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & \delta_r & 0 & \cdots & 0 \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0
\end{pmatrix}
$$

（矩阵 $(\eta_{ij})$ 的所有项都是零，除了 $\eta_{li}$ 代表 $1 \leq i \leq r$，$\eta_{li} = 1$ 代表$1 \leq i \leq r - 1$、$\eta_{rr} = \delta_r \neq 0$）。 *如果$r \neq m$或$r \neq n$，也可以假设为$\delta_r = 1$。

如果$X = 0$，则命题是明显的；因此假设$X \neq 0$。如果$m = n = 1$命题是明显的（$P = I_m$，$Q = I_n$，$\delta_1 \neq 0$任意）。如果$n = 1$，$m \geq 2$，我们可以应用引理 1（从$X \neq 0$开始），这给出了所需的形式（58）和$r = 1$，$\delta_r = 1$。我们通过归纳对$n > 1$争论； $X$中存在元素$\xi_{ij} \neq 0$；如果$j = 1$，引理 1 可以应用，约化问题可以应用到$X$ 有形式 (57) 的情况。 归纳假设然后适用于$Y$，因此有可逆的矩阵

$$
P' \in \mathbf{M}_{m-1}(\mathbf{K}), \quad Q' \in \mathbf{M}_{n-1}(\mathbf{K})
$$

其中乘积 / 矩阵 / 形式 $B_{ij}(\lambda)$ / 阶 $m - 1$（分别为$n - 1$），使得$P'YQ'$为形式 (58)。但是，如果 $B_{ij}(\lambda)$ 属于对于例到 $\mathbf{M}_{m-1}(\mathbf{K})$，则

$$
\begin{pmatrix}
1 & 0 \\
0 & B_{ij}(\lambda)
\end{pmatrix} = B_{i+1,\ j+1}(\lambda);
$$

公式 (58) 然后从公式开始块乘积写作

$$
P = \begin{pmatrix} 1 & 0 \\ 0 & P' \end{pmatrix} \text{ and } Q = \begin{pmatrix} 1 & 0 \\ 0 & Q' \end{pmatrix}.
$$

如果最终$j \neq 1$，对于上述情况考虑矩阵$XB_{j1}(1)$到约化就足够了。

命题14立即恢复命题13。

#### 推论 1 {#alg-ii-s10-prop-14-cor-1 .statement tag=05XD}

*如果$X$是阶$n$的可逆平方矩阵超过域$\mathbf{K}$，则存在阶$n$的三个可逆矩阵$P, Q, D$这样$X = PDQ$、$P$ 和 $Q$ 分别为形式 $B_{ij}(\lambda)$ 矩阵乘积以及形式 $D$ 对角矩阵*

$$
D = \operatorname{diag}(1, 1, \ldots, \delta),
$$

*其中 $\delta \neq 0$ (cf. 习题 13).*

#### 推论 2 {#alg-ii-s10-prop-14-cor-2 .statement tag=05XE}

*对于每个域$\mathbf{K}$，可逆矩阵$\mathbf{GL}(n, \mathbf{K})$的群由置换矩阵（no. 7，例2）生成，对角线矩阵$\operatorname{diag}(a, 1, \ldots, 1)$ （$\mathbf{K}$中的$a \neq 0$）和矩阵$B_{12}(\lambda)$（$\lambda \in \mathbf{K}$）。*

已经看出(no. 9)，适当转置的矩阵的右(或左)乘积乘以矩阵交换任意两个列(或行)。那么矩阵$\operatorname{diag}(1, \ldots, 1, a)$等于$\operatorname{diag}(a, 1, \ldots, 1)$和置换矩阵的乘积，并且每个矩阵$B_{ij}(\lambda)$等于$B_{12}(\lambda)$和置换的乘积矩阵，从而推论。

#### 注 {#alg-ii-s10-n13-rem-1 .statement tag=05XF}

(1) 在章III中，我们将看到，如果$m = n = r$和$K$是*可交换的*，那么，对于$P$和$Q$满足条件的所有选择命题 14、元素 $\delta_r$ 始终相同且等于 $X$ (III, § 8, no. 6) 的*行列式*。

(2) 命题 14 的论证稍加修改，表明存在置换矩阵 $R$ 使得（与 $P$ 上的条件相同）

$$
PX R = \begin{pmatrix} I_r & N \\ 0 & 0 \end{pmatrix}
$$

如果 $m = n = r$ 不成立，并且

$$
PX R = \operatorname{diag}(1, \ldots, 1, \delta)
$$

否则。还观察到，当显式给出 $X$ 时，证明的方法给出了矩阵 $P, Q, R$ 的显式确定。

### 习题{#alg-ii-s10-exercises}

§ 10](exercises/s10/)参见[习题。
