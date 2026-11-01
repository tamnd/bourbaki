---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 5
section_title: Endomorphisms of vector spaces
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.70-A VII.72
pdf_pages: 0387-0407, 0429-0431
extraction: ocr
subsections:
    - "no": 1
      title: The module associated to an endomorphism
      page: 28
      pdf_page: 387
    - "no": 2
      title: Eigenvalues and eigenvectors
      page: 30
      pdf_page: 389
    - "no": 3
      title: Similarity invariants of an endomorphism
      page: 31
      pdf_page: 390
    - "no": 4
      title: Triangularisable endomorphisms
      page: 34
      pdf_page: 393
    - "no": 5
      title: 'Properties of the characteristic polynomial : trace and determinant'
      page: 36
      pdf_page: 395
    - "no": 6
      title: Characteristic polynomial of the tensor product of two endomorphisms
      page: 39
      pdf_page: 398
    - "no": 7
      title: Diagonalisable endomorphisms
      page: 40
      pdf_page: 399
    - "no": 8
      title: Semi-simple and absolutely semi-simple endomorphisms
      page: 41
      pdf_page: 400
    - "no": 9
      title: Jordan decomposition
      page: 43
      pdf_page: 402
statements: 66
exercises: 14
content_sha256: 16d70c8e43a530acd88980d634caacfd61e2e40e9549a5b78c5edc8dc64ccd9b
translated_from: content/en/alg/VII/05_s5_endomorphisms_of_vector_spaces.md
translation_method: google
source_content_sha256: b9e185d13ebac7827bb1a35037e89aed5a271cfe0bbc0b2b0fb72b7a265e5960
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: dc66771315ab163c8a55f75e2d39559ef22a02f9fd9f78bce1a18045bcf5e004
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。 自同态 / 向量空间

记号。 — 给定 $M$ 的模 $M$、元素 $x$，以及 $M$ 的两个自同态 $u$ 和 $v$，我们将写 $u.x$、$uv.x$ 和 $uv$ 来代替分别为$u(x)$、$(u \circ v)(x)$和$u \circ v$；当不会引起混淆时，我们将用 1 来表示从 $M$ 到自身的恒等式映射。

### 1. 模与自同态关联

令$A$为交换环，令$M$为$A$模，令$u$为$M$的$A$自同态。回想一下（III，p. 538），映射$(p(X), x) \mapsto p(u).x$从$A[X] \times M$到$M$使$M$成为$A[X]$模块，写作$M_u$。还记得（III，第 538 和 539 页），如果 $M[X]$ 表示从 $M$ 通过扩张从 $\mathbf{A}$ 到 $\mathbf{A}[X]$ 的标量获得的 $A[X]$ 模块，并且如果 $\bar{u}$ 表示由$u$诱发$\mathbf{A}[X]$-$M[X]$的自同态，则$\mathbf{A}[XI]$-模块$^1$有正合序列

$$
(1) \quad 0 \to M[X] \xrightarrow{\psi} M[X] \xrightarrow{\varphi} M_u \to 0 ,
$$

其中 $\varphi(p(X) \otimes x) = p(u).x$ 和 $\psi = X - \bar{u}$。

自同态 $u$ of an $\mathbf{A}$-module $M$ and 自同态 $u'$ of an $\mathbf{A}$-module $M'$ are said to be similar if there exists 同构 $g$ from $M$ onto $M'$使得$u' \circ g = g \circ u$，即（III，p. 540，命题19）同构$g$从$M_u$到$M_{u'}$。 If $M$ (resp. $M'$) is free on the finite 基 $B$ (resp. $B'$), and if $M(u)$ (resp. $M(u')$) is 矩阵 of $u$ (resp. $u'$) with respect to $B$ (resp. $B'$), then $u$ and $u'$ are similar if and only if $M(u)$ and $M(u')$ are similar 矩阵 (II, p. 356, Def. 6). The characteristic polynomials (III, p. 541, Def. 3) of two similar 自同态 of finitely generated 自由模 are equal (III, p. 540, Prop. 19).

令$K$为交换域；然后将 $K$ 上的向量空间 $E$ 中的任意对 $(E, u)$ 由……组成和 $E$ 对应中的自同态 $u$ 转换为 $K[X]$ 模块$E_{,,}$。由于环$K[X]$是主理想整环（IV，p. 11，命题11），所以前面截面的结果可以应用到$E_{,,}$。

首先让我们展示如何将某些概念从模的语言翻译为向量空间的自同态的语言：

« V 是 $E$ 的子模，» 意思是： « V 是 $E$ 的向量子空间在 $u$ 下关闭 »。

« V is a cyclic 子模 of $E$, » means : « there exists $x \in V$ such that 向量子空间 $V$ is spanned by 元素 $u^i . x \ (i \in \mathbf{N})$ ».那么 $V$ 被称为循环（相对于 $u$），$x$ 被称为生成元。

« V is an indecomposable 子模 of $E$, » means : « V is 非零的 and is not 直和 of two 非零的子空间 each closed under $u$ ».

« a is 湮没子 of 子模 $V$ » means : « a is the ideal 由……组成 of those polynomials $p(X) \in K[X]$ such that $p(u).x = 0$ for all $x \in V$ ».

The monic polynomial $g$ such that $a$ is equal to the principal ideal $(g)$ is then called the minimal polynomial of 限制 of $u$ to $V$.

« $E_{,,}$ 与湮没子 $a = (g)$ 循环 »

$$
\text{(with } g(X) = X^n + \alpha_{n-1} X^{n-1} + \cdots + \alpha_0 )
$$

$^1$$\psi$的单射性，在III、p. 539第18条命题中未提及，证明如下：在loc的记号中。如上所述，我们有

$$
\psi(\sum (X^k \otimes x_k)) = \sum X^k \otimes (x_{k-1} - u(x_k)) .
$$

如果$\psi$的$\sum X^k \otimes x_k$属于到核，那么$x_k , = u(x_k)$对于所有$k$，$x_k$都是零，因为$(x_k)$家族有有限支撑。

意思是：«存在$x \in E$使得$(u^i . x)$（$0 \leq i \leq n - 1$）是向量空间$E$的基和$g(u).x = 0$»。在其他字中，我们可以找到$E$的基，使得$u$的矩阵$U$相对于此基为

$$
U = \begin{pmatrix}
0 & 0 & 0 \ldots 0 & -\alpha_0 \\
1 & 0 & 0 \ldots 0 & -\alpha_1 \\
0 & 1 & 0 \ldots 0 & -\alpha_2 \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & 0 \ldots 0 & -\alpha_{n-2} \\
0 & 0 & 0 \ldots 1 & -\alpha_{n-1}
\end{pmatrix}.
$$

« $E$，是挠元模 » 意味着，根据上面给出的循环挠元模的特征： « $E$ 的每个循环子模，在 $K$ 上都是有限维的 »。尤其 ：

« $E_u$ 是有限生成的挠元模 » 意味着： « $E$ 是 $K$ 上的有限维 »。

### 2. 特征值和特征向量

#### 定义 1 {#alg-vii-s5-def-1 .statement tag=075G}

*设$E$为向量空间大于交换域$K$，且$u$自同态大于$E$。 如果存在$a \in K$使得$u . x = \alpha x$，则称$E$的元素$x$为$u$的特征向量；如果 $x \neq 0$ 则标量 $a$ 被称为 $u$ 相应的的特征值到特征向量 $x$。 对于$x \in E$的每个标量$a$，向量子空间$V_a$由……组成，使得$u . x = \alpha x$称为$E$相应的到$a$的特征空间。

特征值$a$的几何重数是基数$\dim V_a$。

假设 $E$ 是有限维的。 $u$的特征值是$K$的元素$a$，使得$E$的自同态$a . 1 - u$不是单射的，在其他字（III，p. 524，命题3）中，这样那个$\det(a . 1 - u) = 0$。但是，通过 $u$ (III, p.541, Def. 3) 的特征多项式 $\chi_u$ 的定义，我们有 $\det(a . 1 - u) = \chi_u(\alpha)$。最后 ：

#### 命题 1 {#alg-vii-s5-prop-1 .statement tag=075H}

*假设$E$是有限维的。那么$K$的元素$a$是自同态$u$的特征值当且仅当它是$u$的特征多项式的根。

如果$L$是域$K$的扩张，则$L$中$\chi_u$的根是$L$向量空间$L \otimes_K E$的自同态$1, \otimes u$的特征值。它们通常被称为 $L$* 中的 $u$ *特征值。通过滥用语言，我们说$u$属于到$L$的所有特征值，如果这适用于$L$的代数闭扩张中的$u$的所有特征值；这意味着$\chi_u$分解为$L[X]$中的线性因子。

令$U$为阶$n$的平方矩阵，系数为$K$。则由定义 $U$ 的特征多项式为

$$
\chi_U(X) = \det(X . I, -U);
$$

$U$的特征值（$K$的扩张$L$）是多项式$\chi_U$的根（$L$）；这些也是标量$a$（在$L$中），使得存在线性方程$UX = \alpha X$的非零的解到系统，其中$X$是阶的列矩阵 $n$； 列矩阵 $X$ 满足该方程称为 $U$ 相应的至 $a$ 的特征向量。

如果$U$相对于基$B$是n维向量空间的自同态$u$的矩阵，则$U$的$\chi_U = \chi_u$、特征值是特征值 $u$，$U$的特征向量是$u$的特征向量相对于基$B$的矩阵。

#### 命题 2 {#alg-vii-s5-prop-2 .statement tag=075I}

*令$u$为向量空间$E$之自同态超过交换域$K$；对于每个标量 $a$，令 $V_a$ 为特征空间相应的到 $a$。那么子空间$V_a$在$u$下闭合，$V_a$的和是直接的。*

第一个断言是清楚的。 定义子空间$V_a$被$K[X]$的元素$X - a$湮灭； $X - a, a \in K$ 是不可约且成对非关联的；因此，第二个断言是从VII、p. 8、Th得出的。 1.

### 3. 自同态的相似不变量

If we translate the decomposition of a finitely generated torsion module in VII, p. 8, Th. 1 and p. 9, Prop. 2, then we obtain:

#### 命题 3 {#alg-vii-s5-prop-3 .statement tag=075J}

*令$E$为有限维$n$之向量空间超过交换域$K$，令$u$为$E$之自同态；对于每个莫尼克不可约多项式$p(X)$，令$M_p$为$E$的元素$x$的向量子空间由……组成，使得$(p(u))^k \cdot x = 0$对于某些整数$k$。那么$M_p$在$u$下闭，向量空间$E$是$M_p$的直和，并且存在多项式$s_p$，使得对于所有$x \in E$，$x$在$M_p$的分量是等于 $s_p(u) \cdot x$.*

#### 注 1 {#alg-vii-s5-n3-rem-1 .statement tag=075K}

显然，$u$到$M_p$的限制的最小多项式是$p$的最大的幂，其中除是$u$的最小多项式。此外，对于$x \in M_p$，我们有$s_p(u) \cdot x = x$，从中可以立即得出，如果$M_p \neq 0$，则$s_p$与$p$互质。

同样，Th. VII、p. 19、模$E_u$的2同构于循环模$F_j = K[X]/a_j \ (1 \leq j \leq r)$的直和，其中理想$a_j$不同于$K[X]$和$a_j \subset a_{j+1}$；而$a_j$是由这些条件决定的。此外，由于$E$，是挠元模，所以我们有$a_1 \neq (0)$；因为$E$有维数$n$，所以我们有$r \leq n$。将$a_j = (h_j) \ (1 \leq j \leq r)$和$h_j$作为一元多项式，并考虑由以下定义的多项式的序列$(q_i) \ (1 \leq i \leq n)$：

$$
\begin{cases}
q_i(X) = 1 & \text{if } i \leq n - r \\
q_i(X) = h_{n-i+1}(X) & \text{if } n - r < i \leq n .
\end{cases}
$$

很明显，首一多项式 $q_i$ 确定多项式 $h_j$ ，反之，$E$ 与 $n$ 模 $K[X]/(q_i)$ 的直和同构，其中第一个 $n - r$ 是$0$。

其他字：

#### 命题 4 {#alg-vii-s5-prop-4 .statement tag=075L}

— 令 E 为有限维 n 的交换域 K 的向量空间，令 u 为 E 的自同态。则存在 n 个一元多项式 $q_i(X) \in K[X]$ ($1 \leq i \leq n$)，使得 $q_i$ 除 $q_{i+1}$ 对于 $1 \leq i \leq n-1$，并且E 是 n 子空间 $V_i$ ($1 \leq i \leq n$) 的直和，在 u 下闭合，循环（相对于 u），并且使得 u 到 $V_i$ 的限制的最小多项式等于 $q_i$ ($1 \leq i \leq n$)。首一多项式$q_i$由这些条件唯一确定，$q_n$是u的最小多项式q。

#### 注 2 {#alg-vii-s5-n3-rem-2 .statement tag=075M}

由上述命题，存在E的基相对于u的矩阵U有形式

$$
\begin{pmatrix}
A_{n-r+1} & 0 & \ldots & 0 & 0 \\
0 & A_{n-r+2} & \ldots & 0 & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \ldots & A_{n-1} & 0 \\
0 & 0 & \ldots & 0 & A_n
\end{pmatrix}
$$

其中每个矩阵$A_i$都有形式(2)（取$g(X) = q_i(X)$）（cf.VII，第29-30页）。

#### 定义 2 {#alg-vii-s5-def-2 .statement tag=075N}

— 在命题 4 的记号中，n 个调多项式 $q_i(X)$ ($1 \leq i \leq n$) 称为自同态 u 的相似不变量。

因此，第 n 个相似不变量 $q_n$ 是 u 的最小多项式（命题 4）；在其他字中，对于多项式$p(X) \in K[X]$到满足$p(u) = 0$，$p$是$q_n$的倍数是充分必要的。

#### 推论 1 {#alg-vii-s5-def-2-cor-1 .statement tag=075O}

— 令 K 为域，令 E 和 $E'$ 为 K 上的两个有限维向量空间，并令 u（分别为 $u'$）为 E（分别为 $E'$）的自同态。那么 u 和 $u'$ 是相似的 (VII, p. 29) 当且仅当它们具有相同的相似不变量。

事实上，当且仅当$K[X]$-模E和$E'_u$同构时，$u$和$u'$是相似的。

#### 推论 2 {#alg-vii-s5-def-2-cor-2 .statement tag=075P}

— 令 u 为域 K 上有限维向量空间 E 的自同态，令 $(q_1, \ldots, q_n)$ 为 u 的相似不变量族，令 L 为 K 的扩张，令 $E_{(L)} = L \otimes_K E$ 为由扩张从 E 导出的 L 向量空间标量，并令 $u_{(L)} = 1_L \otimes u$ 为由 u 引发的 $E_{(L)}$ 的自同态。那么$u_{(L)}$的相似不变量就是$L[X]$中$q_1, \ldots, q_n$的像$\bar{q}_1, \ldots, \bar{q}_n$。

这直接从命题 4 以及$L[X]$模块$E_{(L)u_{(L)}}$和$(K[X]/(q_i))_{(L)}$分别同构于$L[X] \otimes_{K[X]} E_u$和$L[X]/(\bar{q}_i)$的事实出发。

设U为阶 n 的平方矩阵，系数为交换域 K。则由U定义的$K^n$的自同态的相似不变量称为$U$的相似不变量。接下来是 Cor 的结论。上面的1中，两个方阵相似当且仅当它们具有相同的相似不变量，并且如果$u$是$K$上有限维向量空间$E$的自同态，并且$U$是$u$的矩阵关于某些$E$的基$B$，然后是$U$和$u$重合的相似不变量。由科.上面1和2，我们有：

#### 推论 3 {#alg-vii-s5-def-2-cor-3 .statement tag=075Q}

— 令$U$和$V$为阶$n$中的两个方阵，系数为交换域$K$。如果在 $K$ 的某些扩张 $K'$ 上存在可逆平方矩阵 $P$ 使得 $V = P^{-1}UP$，则在 $K$ 上存在可逆平方矩阵 $Q$ 使得$V = Q^{-1}UQ$。

令$E$为交换域$K$上的有限维向量空间，令$(e_i)_{1 \leq i \leq n}$为$E$的基，并令$u$为$E$的自同态。然后通过VII、p. 29的正合序列(1)，与$u$伴随的$K[X]$模块$E$同构于自由$K[X]$模块$E[X]$与基的商$(1 \otimes e_i)$，在$K[X]$线性映射$X - \bar{u}$下乘$E[X]$的像。因此，$u$（VII，p. 32，Def.2）的相似不变量$q_i(X)$是$X - \bar{u}$（VII，p. 22）的不变量因子。因此VII、p. 22的第6号提案意味着：

#### 命题 5 {#alg-vii-s5-prop-5 .statement tag=075R}

— 令$E$为有限维$n$的向量空间超过交换域$K$，令$u$为$E$的自同态，并令$U$为关于某些的矩阵基 / $E$。然后对于每个整数 $m$ 和 $1 \leq m \leq n$，乘积
$$
d_m(X) = q_1(X) q_2(X) \ldots q_m(X)
$$
$u$的第一个$m$相似不变量的最大公约数等于$m$-第阶未成年人矩阵$XI, - U$的gcd。

#### 推论 1 {#alg-vii-s5-prop-5-cor-1 .statement tag=075S}

— 令 $u$ 为有限维 $n$ 向量空间的自同态在交换域 $K$ 上，特征多项式 $\chi_u(X)$ 和相似不变量 $q_i(X)$ ($1 \leq i \leq n$)。然后
$$
\chi_u(X) = q_1(X) q_2(X) \ldots q_n(X)
$$

#### 推论 2 {#alg-vii-s5-prop-5-cor-2 .statement tag=075T}

— 在 Cor 的记号中。 1、令$q(X)$为$u$的最小多项式；然后$q(X)$除$\chi_u(X)$和$\chi_u(X)$除$q(X)^n$。特别是$u$的最小多项式和特征多项式具有相同的根，即$u$的特征值。

从$q(X) = q_n(X)$开始，显然$q(X)$除$\chi_u(X)$。另一方面，由于每个$q_i$除$q$，他们的乘积$\chi_u$除$q^n$。

#### 推论 3 {#alg-vii-s5-prop-5-cor-3 .statement tag=075U}

— 自同态 $u$ 是幂零的当且仅当其特征多项式具有形式 $X^n$。

这立即来自Cor。 2.

现在让我们重写VII、p. 24的第9条命题，它将模的分解给出为不可分解的子模的直和。

#### 命题 6 {#alg-vii-s5-prop-6 .statement tag=075V}

— 令$E$为有限维$n$之向量空间超过交换域$K$，并令$u$为$E$之自同态。那么$E$是子空间$E_k$的直和，在$u$下闭集并且相对于$u$循环，使得$u$到$E_k$的限制的最小多项式有形式 $p_k^{n(k)}$，其中$p_k$是不可约多项式，$E_k$不能表示为两个非零的子空间的直和，每个非零的子空间在$u$下闭合。对于任何此类分解中的子空间 $E_k$ 的每个单调不可约多项式 $p \in K[X]$ 和每个整数 $n \geq 1$、数 $m(p^n)$，使得 $p^n$ 是限制的最小多项式$u$到$E_k$，是唯一确定的。

$p_k^{n(k)}$ 确定 $u$ 的相似不变量，反之亦然；我们可以通过VII，p. 25，注2和3中解释的过程从一个到另一个。此外，我们可以立即从第6条中考虑的分解到第3和4条中考虑的那些。

注 $p \in K[X]$ 使得 $m(p^n) > 0$ 对于某些整数 $n \geq 1$ 恰好是 $u$ 的最小多项式的因子。因此，与相似不变量相比，这些多项式通常取决于我们正在研究的域 $K$。

### 4. 可三角形自同态

在这个截面中，我们将感兴趣的是$u$分裂的的最小多项式$p(X)$到$K[X]$中线性因子的乘积，在其他字（VII，p. 33，Cor. 2) $u$属于至$K$中所有特征值的情况。当 $K$ 是代数闭时，这一点尤其成立。 VII、p. 31 的第 3 条命题立即给出：

#### 命题 7 {#alg-vii-s5-prop-7 .statement tag=075W}

— 令$E$为交换域$K$上的有限维向量空间，并令$u$为$E$的自同态，其特征值全部为属于至$K$。对于$u$的每个特征值$a$，令$M_a$为$E$由……组成中的向量子空间，其中元素$x$存在整数$k \geq 1$这样的那个$(u - a)^k \cdot x = 0$。那么$M_a$在$u$下闭，向量空间$E$是$M_a$的和，并且存在多项式$s_a \in K[X]$，使得对于所有$x \in E$，$x$在$M_a$的分量为等于$s_a(u) \cdot x$。

子模$M_a$，作为$K[X]$模块有限生成，则湮没子为形式$(X - a)'$；在其他字中，存在整数$r \geq 1$使得
$$
(u - a)^r \cdot x = 0
$$
对于所有$x \in M_a$； $u - a$到$M_a$的限制是幂零自同态。

仍然假设$u$属于到$K$的特征值，我们现在应用VII、p. 34到$u$的第6条建议。多项式$p_k$只不过是$X - a$（因为$a$穿过$u$的特征值的集合），我们看到$E$是子空间$E_i$的直和闭于$u$，循环（相对于$u$），并且使得$u$到$E_i$的限制的最小多项式具有形式$(X - a)^m$。令 $E_i'$ 为与 $E_i$ 伴随的 $K[X]$ 模块；则 $E_i'$ 同构于模 $K[X]/((X - a)^m)$ 之一。现在元素 $(X - \alpha)^k$ ($0 \leq k \leq m - 1$) 形式剩余类类 mod $(X - a)^m$ $K[X]/((X - a)^m)$ 的 $K$ 基础（IV，p. 11，Cor.），以及

$$
X(X - \alpha)^k = \alpha (X - \alpha)^k + (X - \alpha)^{k+1}
$$

对于$0 \leq k \leq m - 1$；由此可见，$E_i$有维数$m$，如果$a$是$u$到$E_i$的限制$u_i$唯一的特征值，则存在$E_i$的基，相对于$u_i$中的矩阵是$m \times m$矩阵

$$
U_{m,\alpha} = \begin{pmatrix}
\alpha & 0 & 0 & \ldots & 0 & 0 \\
1 & \alpha & 0 & \ldots & 0 & 0 \\
0 & 1 & \alpha & \ldots & 0 & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & 0 & \ldots & \alpha & 0 \\
0 & 0 & 0 & \ldots & 1 & \alpha
\end{pmatrix}
$$

#### 定义 3 {#alg-vii-s5-def-3 .statement tag=075X}

*对于每个域$K$，每个整数$m \geq 1$，每个$a \in K$，矩阵$U_{m,\alpha}$被称为阶$m$和特征值的乔丹矩阵 $a$.*

#### 命题 8 {#alg-vii-s5-prop-8 .statement tag=075Y}

*令$E$为交换域$K$的有限维向量空间，并令$u$为$E$的自同态。那么下面的条件是等价的*：

(i) *$u$中的特征值（在$K$中的某些代数闭扩张）属于至$K$*；

(ii) *存在$E$的基相对于$u$的矩阵是下（或上）三角形*；

(iii) *存在$E$的基，相对于$u$的矩阵是约旦矩阵的对角线块*。

根据第 7 号提案，我们有 (i) $\Rightarrow$ (iii) 和上面的注，并且断言 (iii) $\Rightarrow$ (ii) 和 (ii) $\Rightarrow$ (i) 是微不足道的。

#### 定义 4 {#alg-vii-s5-def-4 .statement tag=075Z}

*第 8 条中的自同态满足条件 (i)、(ii) 和 (iii) 称为可三角化*。

特别是，如果 $K$ 是代数闭的，则 $K$ 向量空间的每个自同态都是可三角化的。

对于矩阵，第 8 条命题意味着：

#### 推论 {#alg-vii-s5-n4-cor-1 .statement tag=0760}

*令$U$为平方矩阵超过交换域$K$，使得$U$的所有特征值都在$K$中；那么存在类似于$U$的矩阵，它是乔丹矩阵*的对角线块。

#### 注 {#alg-vii-s5-n4-rem-1 .statement tag=0761}

— 1) 由VII、p. 34的命题6可知，如果$U$与约旦矩阵$(J_k)$的对角线块相似，则形式的$J_k$的数 $U_{m,\alpha}$（对于给定的$m$和$\alpha$）由$U$唯一确定。

2) 更一般地，如果 $U$ 类似于 Jordan 矩阵 $U_{m_i, \alpha_i}$ 的对角线块，则 $U$ 的相似不变量可以通过以VII、p. 25 中提出的模型为模型的方法轻松计算， 注 3 ：将递减阶指数中所有与$\alpha$相同的$(X - \alpha_i)^{m_i}$写在同一行，并以1补全，使长度等于$U$的阶；完成此操作后，通过在相同的列中形成项的乘积，在指标的递减阶中获得$U$的相似不变量。 例，矩阵

$$
\begin{pmatrix}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 1 & 3
\end{pmatrix}
$$

我们写

$$
(X - 2), 1, 1 \\
(X - 3)^2, 1, 1
$$

相似性不变量为 1、1 和 $(X - 2)\ (X - 3)'$

通过注意到 Jordan 矩阵 $U_{m, \alpha}$ 的最小多项式为 $(X - a)''$，并且它等于其特征多项式，我们得到以下结果：

#### 命题 9 {#alg-vii-s5-prop-9 .statement tag=0762}

— *如果平方矩阵 $U$ 类似于Jordan 矩阵 $(U_{m_i, \alpha_i})$的对角线块，那么$U$的最小多项式就是$(X - \alpha_i)^{m_i}$的lcm，特征多项式就是乘积的乘积 $(X - a_i)'''$.*

#### 推论{#alg-vii-s5-n4-cor-2 .statement tag=0763}

— *在第7条的记号中，子空间$M_\alpha$的维数是特征值$\alpha$的重数作为$u$的特征多项式的根。*

### 5. 特征多项式的性质：迹和行列式

令E为交换域K上有限维$n$的向量空间，并令$u$为E的自同态。由III，p. 541，$u$的特征多项式有形式：

(5)
$$
\chi_u(X) = X^n - \mathrm{Tr}(u)\ X^{n-1} + \cdots + (-1)^n \det(u)\ .
$$

#### 命题 10 {#alg-vii-s5-prop-10 .statement tag=0764}

— *令$E$为有限维$n$的向量空间超过交换域$K$，令$u$为$E$的自同态，令$\chi_u(X) = \prod_{i=1}^n (X - \alpha_i)$为分解为线性其特征多项式的因子（$K$，cf.V，p. 21的合适扩张）。如果 $q$ 是系数为 $K$ 的多项式，则 $q(u)$ 的特征多项式由下式给出：

(6)
$$
\chi_{q(u)}(X) = \prod_{i=1}^n (X - q(\alpha_i))\ ,
$$

它的迹和行列式由下式给出

(7) $$
\operatorname{Tr}(q(u)) = \sum_{i=1}^n q(\alpha_i),
$$
(8) $$
\det(q(u)) = \prod_{i=1}^n q(\alpha_i).
$$

显然，根据（5）可以从（6）推导出（7）和（8）。为了证明公式 (6)，我们可以假设 K 是代数封闭的。然后我们取基作为E，相对于$u$的矩阵$U$是下三角（$VII$，p. 35，对应命题8）；我们将利用以下简单的引理：

#### 引理 1 {#alg-vii-s5-lem-1 .statement tag=0765}

*如果B和C是阶n的下三角形矩阵，对角线为$(\beta_i)$和$(\gamma_i)$，则矩阵$B + C$和$BC$是对角线为$(\beta_i + \gamma_i)$和$(\beta_i \gamma_i)$.*

由于$u$的矩阵$U$是对角线$(\alpha_i)$的下三角形，因此从引理1可以得出$q(U)$是对角线$(q(\alpha_i))$的下三角形矩阵。那么$X . I, -q(U)$是一个对角线为$(X - q(a;))$的下三角形矩阵，这就证明了(6)。

#### 推论 1 {#alg-vii-s5-lem-1-cor-1 .statement tag=0766}

*要使$q(u)$可逆，$q$与$\chi_u$互质是必要且充分的。*

事实上，说$q$和$\chi_u$互质就相当于说，它们在K的代数闭扩张中没有公共的根，而在其他字(8)中$\det(q(u)) \neq 0$。

#### 注 1 {#alg-vii-s5-n5-rem-1 .statement tag=0767}

— 多项式与 $\chi_u$ 互质当且仅当它与 $u$ 的最小多项式互质（VII，p. 33，Cor.2）。

#### 推论 2 {#alg-vii-s5-lem-1-cor-2 .statement tag=0768}

*设$r \in K(X)$是K上的有理数函数。则$u$在$r$中可替换（IV，p. 21）当且仅当其每个特征值是。在这种情况下，以下公式成立：*

$$
\chi_{r(u)}(X) = \prod_{i=1}^n (X - r(\alpha_i)), \quad \operatorname{Tr}(r(u)) = \sum_{i=1}^n r(\alpha_i), \quad \det(r(u)) = \prod_{i=1}^n r(\alpha_i).
$$

写出 $r = p/q$，其中 $p$ 和 $q$ 是互质多项式。那么当且仅当$\det(q(u)) \neq 0$时$u$可在$r$中替换，因此第一个断言由(8)得出。由科. 1，我们可以假设$q$与$\chi_u$互质，因此根据Bezout恒等式，存在多项式$g$和$h$使得$qg + h\chi_u = 1$。然后由 Cayley-Hamilton 定理（III、p. 541）乘坐 $q(\alpha_i)g(\alpha_i) = 1$ 和 $q(u)g(u) = 1$。然后可以通过应用公式(6)、(7)和(8)到$p(u)\ g(u) = r(u)$获得所述公式。

#### 推论 3 {#alg-vii-s5-lem-1-cor-3 .statement tag=0769}

*对于每个整数$s \geq 0$，我们有$\operatorname{Tr}(u^s) = \sum_{i=1}^n \alpha_i^s$。如果 $u$ 是可逆的，则此公式对于 $s < 0$ 也有效。*

这是前一个推论的一个特例。

#### 推论 4 {#alg-vii-s5-lem-1-cor-4 .statement tag=076A}

— *假设域 K 为特征零；那么自同态 u 是幂零的当且仅当* $\operatorname{Tr}(u^s) = 0$ *对于* $1 \leq s \leq n$。

如果$u$是幂零的，那么$a_i$都是零，$\operatorname{Tr}(u^s) = 0$对于所有$s > 0$（Cor.3）。相反，如果$\operatorname{Tr}(u^s) = 0$代表$1 \leq s \leq n$，则$a_i$都是零，因为$K$是特征零（IV，p. 72，Cor.），并且$u$是幂零的（VII， p. 33）。

#### 推论 5 {#alg-vii-s5-lem-1-cor-5 .statement tag=076B}

— *令 Y 为不定数，并令 $\tilde{u}$ 表示 $K(Y)$ 向量空间 $K(Y) \otimes_K E$ 的自同态，由有理函数的$K$ 到域 $K(Y)$ 的标量扩张从 $u$ 导出$Y$，系数来自$K$。那么自同态 $Y \cdot 1 - \tilde{u}$ 可逆。此外，如果$\chi_u'$表示多项式$\chi_u$的导数，则*

$$
\operatorname{Tr}((Y \cdot 1 - \tilde{u})^{-1}) = \chi_u'(Y)/\chi_u(Y) .
$$

自同态 $Y \cdot 1 - \tilde{u}$ 是可逆的，因为它的行列式是 $K(Y)$ 的非零元素 $\chi_u(Y)$。由此可见，$\tilde{u}$可以用有理数函数$r(X) = (Y - X)^{-1}$替代$K(Y)(X)$。第二个断言现在来自Cor。 2、关系

$$
\chi_u'(Y)/\chi_u(Y) = \sum_i (Y - \alpha_i)^{-1} = \sum_i r(\alpha_i) .
$$

#### 推论 6 {#alg-vii-s5-lem-1-cor-6 .statement tag=076C}

— *假设域 K 为特征零。然后，在正式幂级数的环$K[[T]]$中，我们有*

$$
- T \frac{d}{dT} \log \det(1 - Tu) = \sum_{m \geq 1} \operatorname{Tr}(u^m) T^m
$$

让我们首先处理有理函数的域$K(T)$，并放入$P(T) = \det(I, -T \cdot U)$，其中$U$是$u$的矩阵相对于$E$的某些基。然后

$$
P(T) = \det(T(T^{-1} \cdot I, -U)) = T^n \chi_U(T^{-1}) ,
$$

所以$P'(T)/P(T) = n/T - \chi_u'(T^{-1})/T^2 \chi_u(T^{-1})$。此外，通过 Cor. 5 我们有

$$
\chi_u'(T^{-1})/T \chi_U(T^{-1}) = \operatorname{Tr}((T^{-1} \cdot I_n - U)^{-1})/T = \operatorname{Tr}((I_n - T \cdot U)^{-1}) .
$$

由此可知$-TP'(T)/P(T) = -n + \operatorname{Tr}((I_n - TU)')$。现在通过将该方程的每一边展开为形式幂级数来获得推论。

#### 注 2 {#alg-vii-s5-n5-rem-2 .statement tag=076D}

— 作者：IV、p. 80，Cor。 1 和公式 (8)，对于每个多项式 $q \in K[X]$，我们有

$$
\det q(u) = \operatorname{res}(\chi_u, q) ,
$$

其中 $\operatorname{res}(\chi_u, q)$ 是多项式 $\chi_u$ 和 $q$ 的结果。 *特别是如果我们取 $q = \chi_u'$ 我们得到

$$
\det \chi_u'(u) = (-1)^{n(n-1)/2} \operatorname{dis}(\chi_u),
$$

其中 $\operatorname{dis}(\chi_u)$ 是多项式 $\chi_u$ (*IV*, p. 82, 公式 (47)) 的判别式。此外：

#### 推论 7 {#alg-vii-s5-lem-1-cor-7 .statement tag=076E}

我们有$\det(\operatorname{Tr}(u^{i+j})_{0 \leq i,j \leq n}) = \operatorname{dis}(\chi_u)$。

令 D 为 Vandermonde 矩阵 $(\alpha_i^j)_{1 \leq i,j \leq n}$。那么 (**III**, p. 532, 公式 (29)):

$$
\det(D)^2 = \prod_{i < j} (a_j - \alpha_i)^2 = \operatorname{dis}(\chi_u).
$$

此外，$D \cdot 'D$的第$(i, j)$条目是$\sum_k \alpha_k^{i+j-2} = \operatorname{Tr}(u^{i+j-2})$，推论如下。

### 6. 两个自同态的张量积特征多项式

#### 命题 11 {#alg-vii-s5-prop-11 .statement tag=076F}

*设 E*（分别为 $E'$）*为交换域 K 上的有限维向量空间，并令 u*（分别为 $u'$）*为 E*（分别为 $E'$）的自同态。让*

$$
\chi_u(X) = \prod_i (X - \alpha_i), \quad \chi_{u'}(X) = \prod_j (X - \beta_j)
$$

*将分解转化为u和$u'$*的特征多项式的线性因子在$K$的某些合适的扩张中。 *则向量空间$E \otimes_K E'$的自同态$u \otimes u'$的特征多项式由公式给出*

$$
\chi_u \otimes u'(X) = \prod_{i,j} (X - \alpha_i \beta_j).
$$

按照*VII*、p. 36第10条命题证明的论证，我们发现只要证明以下引理就足够了：

#### 引理 2 {#alg-vii-s5-lem-2 .statement tag=076G}

*设B和C分别为阶 m和n的两个下三角形矩阵，对角线为$(\beta_i)_{1 \leq i \leq n}$和$(\gamma_j)_{1 \leq j \leq n}$。让我们认同有序集 $\{1, 2, \ldots, m\}$ 和 $\{1, 2, \ldots, n\}$ 的字典顺序乘积 ，间隔为 $\{1, 2, \ldots, mn\}$。那么张量积矩阵* (**II**, p. 357) *B $\otimes$ C 是对角线* $(\beta_i \gamma_j)$ 的下三角形。

这紧接着两个矩阵（*loc.cit.*）和词典乘积（*集合理论*，III，p. 157）的张量积的定义。

### 7. 可对角化自同态

#### 定义 5 {#alg-vii-s5-def-5 .statement tag=076H}

— Let E be a finite dimensional 向量空间 over 交换域 K and let $\mathfrak{F}$ be 集合 of 自同态 of E. Then $\mathfrak{F}$ is said to be diagonal with respect to 基 $(e_i)$ of E if 矩阵 of each $u \in \mathfrak{F}$ with respect to $(e_i)$ 是对角线。如果存在 E 的基相对于 $\mathfrak{F}$ 是对角的，则称集合 $\mathfrak{F}$ 是可对角化的。

这个定义特别适用于$\mathfrak{F}$包含只有一个元素$u$的情况；然后我们说 $u$ 是对角线的（可对角线化）。 注还表明 $\mathfrak{F}$ 相对于基 $(e_i)$ 是对角的，当且仅当 $(e_i)$ 是 $\mathfrak{F}$ 的所有元素的公共的特征向量；由此可见，当且仅当 E 由 $\mathfrak{F}$ 的所有元素的特征向量公共的生成时，$\mathfrak{F}$ 是可对角化的。

设 A 为 $\mathrm{End}_K(E)$ 包含 Id 中的子代数。那么 A 是可对角化的当且仅当它与代数 $K^r$ 同构的（在其他情况下字在 V、p. 28、Def. 1 的意义上是可对角化的）；事实上，如果 A 同构于 $K^r$，则 A 可通过 V、p. 29、命题 1 对角化；相反，如果 A 可对角化，则它与对角线矩阵的代数的子代数同构，即代数与 $K^n$、$n = \dim(E)$ 同构的，因此 A 同构于某个代数 $K^r$ （V，p. 30，提案 3）。

#### 命题 12 {#alg-vii-s5-prop-12 .statement tag=076I}

— 令 E 为交换域 K 上的有限维向量空间，并令 u 为 E 的自同态。则以下条件是等价的：

(i) u 是可对角化的。
(ii) E 是 u 特征空间的直和。
(iii) u 的最小多项式的所有根都在K中，并且这些根都是简单的。

此外，如果满足这些条件，则在u下闭合的E的每个子空间都是其具有u的特征空间的交的直和。

(i) 和 (ii) 的等价由前面的注和VII、p. 31、命题2得出。假设u是可对角化的，并令$(\alpha_i)$为其特征值族，以及$(V_i)$相应的族特征空间；由于u到$V_i$的限制是由$\alpha_i$定义的位似，因此它消除了多项式$X - \alpha_i$；由此可见，u 消除了多项式 $\prod (X - \alpha_i)$，因此它是 u 的最小多项式的倍数，因此也有重合，这证明了 (iii)。相反，如果满足(iii)，则存在E的基，相对于u的矩阵U是Jordan矩阵$U_{m,\alpha}$的对角线块（VII，p. 35，命题8）；那么根据命题 9 整数 m 都等于 1，所以 U 是对角线。最后，最后一个断言源自以下事实：如果 u 可对角化，则其特征空间是 $E_u$ 的主要组成部分，并且来自 VII、p. 9、Cor。 1.

#### 推论{#alg-vii-s5-n7-cor-1 .statement tag=076J}

— 如果 u 的特征多项式的所有根都在 K 中，并且它们都是简单的，则 u 可对角化。

实际上最小多项式除是特征多项式。

#### 命题 13 {#alg-vii-s5-prop-13 .statement tag=076K}

— 令 E 为交换域 K 上的有限维向量空间，令 $\mathscr{S}$ 为 E 的自同态的集合，并令 A 为由 $\mathscr{S}$ 和 $\mathrm{Id}_E$ 生成的 $\mathrm{End}_K(E)$ 的子代数。那么下面的条件是等价的：
(i) $\mathscr{S}$ 可对角化。
(ii) K-代数 A 是可对角化的。
(iii) $\mathscr{S}$ 中的元素可对角化并可与 1 个另一个交换。

如果$(e_i)$是E的基，$\mathscr{S}$是对角的，那么A包含在自同态的代数中，它们相对于这个基是对角的，所以也是可对角化的；如果 A 是可对角化的，那么同样的论证表明 $\mathscr{S}$ 是可对角化的。这显示了 (i) 和 (ii) 的等价。由于任意两条对角线矩阵通勤，我们有 (i) $\rightarrow$ (iii)，并且还有待证明逆命题。假设 $\mathscr{S}$ 的元素可对角化并且彼此交换。我们将利用以下引理：

#### 引理 3 {#alg-vii-s5-lem-3 .statement tag=076L}

设g和h是向量空间E的两个对易自同态。那么g的每个特征空间在h下都是封闭的。

事实上，如果 $W_\lambda$ 是 g 相应的到特征值 $\lambda$ 的特征空间，那么对于所有 $x \in W$，我们有
$$
gh \cdot x = hg \cdot x = h \cdot \lambda x = \lambda h \cdot x ,
$$
这表示$h \cdot x \in W_\lambda$。

现在让我们回到第13条命题的证明。E的所有分解中，非零的子空间的直和每个都在$\mathscr{S}$的所有元素、选择下封闭，其中最大的数的最大的数分量（E 的维数对于这个数来说是上界），比如 $E = \sum_{i \in I} E_i$。令 $u \in \mathscr{S}$ 且令 $E = \sum V_\alpha$ 为 E 的分解作为 $u$ 特征空间的直和。到引理 3，每个$V_\alpha$都在$\mathscr{S}$下闭合，因此每个$V_i \cap E_i$也是如此；根据第 12 条命题，每个 $E_i$ 都是 $V_i \cap E_i$ 的直和。因此，$E_i$的选择迫使每个$E_i$包含在$V_\alpha$之一中；因此，$u$的限制对于每个$E_i$来说是位似。由于这对于 $\mathscr{S}$ 的所有元素都是成立的，因此$\mathscr{S}$ 是可对角化的。

#### 推论{#alg-vii-s5-n7-cor-2 .statement tag=076M}

— 和以及 E 的两个对角可对角化自同态的复合是可对角化的。

### 8. 半单绝对半单自同态

#### 定义 6 {#alg-vii-s5-def-6 .statement tag=076N}

— 令 E 为交换域 K 上的有限维向量空间。如果在 u 下封闭的 E 的每个子空间都有一个在 u 下封闭的补集，则 E 的自同态 u 被称为半单。

这意味着$K[X]$-模块E的每个子模是直因子，在其他字中，$K[X]$-模块$E_u$是半单（VII，p. 9）。

#### 命题 14 {#alg-vii-s5-prop-14 .statement tag=076O}

— *当且仅当 u 的最小多项式没有倍数因子时，有限维向量空间在交换域上的自同态 u 是半单。*

这紧接着来自 VII、p. 9、Cor。 4 和 p. 31、注 1。

令 E 为交换域 K 上的向量空间，令 L 为 K 的扩张，且为 E 的 $u$ 自同态；令 $u_{(L)}$ 表示由标量扩张从 E 导出的 L-向量空间 $E_{(l.)} = L \otimes_K E$ 的 L-自同态 $l_L \otimes u$。同样，如果$\mathfrak{F}$是E的自同态的集合，则令$\mathfrak{F}_{(L)}$表示'8中$u$的$u_{(L)}$的集合。

#### 推论{#alg-vii-s5-n8-cor-1 .statement tag=076P}

— *令 u 为交换域 K 上有限维向量空间的自同态，并令 L 为 K 的扩张。如果 $u_{(L)}$ 为半单，则 u 为半单。如果 u 是半单并且 L 在 K 上可分，则 $u_{(L)}$ 是半单。*

这紧随第 14 号提案和 V、p. 120、Cor. 1（注表示$u$和$u_{(L)}$重合的最小多项式）。

#### 命题 15 {#alg-vii-s5-prop-15 .statement tag=076Q}

— *令 E 为交换域 K 上的有限维向量空间，令 u 为 E 的自同态，令 q(X) 为其最小多项式。那么下面的条件是等价的：*

(i) *对于 K 的每个扩张 L，自同态 $u_{(L)}$ 为半单。*
(ii) *存在 K 的扩张 L，使得自同态 $u_{(L)}$ 可对角化。*
(iii) *多项式 q(X) 在 K 上可分离。*

事实上，条件(i)意味着$L[X]$中的多项式$1 \otimes q(X)$不存在倍数因子，对于K的任意扩张L（命题14），条件(ii)意味着存在扩张 K 的L使得$q(X)$属于到L的所有根并且这些根都是简单的（VII，p. 40，命题12），并且这些条件每个都等价于（iii）乘以定义 （V，p. 38）。

#### 定义 7 {#alg-vii-s5-def-7 .statement tag=076R}

— *第 15 号提案的自同态 u 满足条件 (i)、(ii) 和 (iii) 据说绝对是半单。*

#### 推论{#alg-vii-s5-n8-cor-2 .statement tag=076S}

— *u绝对半单的充分必要条件是存在K的扩张L，使得L完美且$u_{(L)}$是半单。*

推论中的条件意味着K存在扩张L使得L是完美的并且$q(X)$在$L[X]$中没有倍数因子（命题14）；这个条件相当于V、p. 38、Cor的(iii)。 2.

#### 命题 16 {#alg-vii-s5-prop-16 .statement tag=076T}

— *令 E 为交换域 K 上的有限维向量空间，令 $\mathfrak{F}$ 为 E 的自同态的集合，令 A 为由 $\mathfrak{F}$ 和 Id 生成的 $\mathrm{End}_K(E)$ 的子代数。那么下面的条件是等价的：*

(i) *存在 K 的扩张 L，使得 $\mathfrak{F}_{(l.)}$ 可对角化。*

(ii) *K-代数* $A$ *是étale*（V，p. 28，默认1）。

(iii)*$\mathfrak{F}$*中的*元素*绝对是半单，并且与一个另一个*通勤。

注首先，对于$K$的每个扩张$L$，由$\mathfrak{F}_{(L)}$和$\mathrm{Id}_{E_{(L)}}$重合与$L \otimes_K A$生成的$L$代数；因此，根据命题 13，$\mathfrak{F}_{(L)}$ 是可对角化的，当且仅当 $L$-代数 $L \otimes_K A$ 是可对角化的。因此，条件 (i) 和 (ii) 的等价是从 V、p. 28、Def 得出的。 1. 另一方面，(i) $\Rightarrow$ (iii) 是直接的。最后假设(iii)成立，令$L$为$K$的代数闭包；那么 $\mathfrak{F}_{(L)}$ 中的元素是可对角化的（VII、p. 40，命题 12）并且可以与 1 个另一个通勤；因此 $\mathfrak{F}_{(L)}$ 可以通过 VII、p. 41、命题 13 对角化。

#### 推论{#alg-vii-s5-n8-cor-3 .statement tag=076U}

*两个通勤的和和乘积，绝对半单自同态绝对半单*。

#### 注 {#alg-vii-s5-n8-rem-1 .statement tag=076V}

— 假设满足第16条命题的条件，并令$L$为$K$的扩张。根据命题 13，当且仅当代数 $L \otimes_K A$ 可对角化时，集合 $\mathfrak{F}_{(L)}$ 可对角化。根据V、p. 30、命题 2，存在 $K$ 的有限扩张 $L$，使得 $\mathfrak{F}_{(L)}$ 可对角化。事实上 $L$ 可以被视为 *Galois*；事实上，取$\mathfrak{F}$的有限子集$\mathfrak{F}'$，其中生成$A$，对于$\mathfrak{F}'$的元素的最小多项式，我们可以取$L$为分裂域（命题12和13）。

### 9. 乔丹分解

#### 定义 8 {#alg-vii-s5-def-8 .statement tag=076W}

*令$E$为交换域上的有限维向量空间，令$u$为$E$的自同态。那么 $u$ 的 Jordan 分解就是对* $(u_s, u_n)$，*其中 $u_s$ 是 $E$ 的半单自同态，$u_n$ 是幂零自同态 $E$，这样*$u_s u_n = u_n u_s$*和*$u = u_s + u_n$。

#### 定理 1 {#alg-vii-s5-thm-1 .statement tag=076X}

*令$E$为交换域$K$的有限维向量空间，并令$u$为$E$的自同态。那么$u$有乔丹分解*$(u_s, u_n)$*当且仅当$u$的特征值在$K$上可分。而且分解是唯一的，$u$和$u_s$重合的特征多项式，并且存在多项式*$P, Q \in K[X]$，*没有常数项，使得*$u_s = P(u)$*和*$u_n = Q(u)$。

A）我们首先证明以下特殊情况

#### 引理 4 {#alg-vii-s5-lem-4 .statement tag=076Y}

*令$E$为交换域$K$上的有限维向量空间，并令$u$为$E$的可三角化自同态。那么存在 $E$ 的唯一可对角化自同态 $v$，它与 $u$ 交换，并且使得 * $u - v$ * 幂零的。而且，在这些条件$u$和$v$重合的特征多项式下，存在一个多项式*$P \in K[X]$*使得*$v = P(u)$。

令$v$为$E$的可对角化自同态，使得$uv = vu$和$v - u$幂零的；令$\alpha$为$v$的特征值，并令$V_\alpha$为相应的特征空间。到引理 3 (VII, p. 41)，$V_\alpha$在$u$下闭，u - α的限制到V，也是u - v的限制，所以幂幂；因此V，包含在被u - a的一些幂湮没的那些x ∈ E的子空间M，由……组成中。由于E是V的直和，也是M的直和，（VII，p. 34，命题7），这表明对于所有a，V，= M。根据命题 9 (VII, p. 36) 的推论，得出 χ_u = χ_v ；还可以得出 v 由 u 唯一确定；它对每个M_α的限制是由α定义的位似。

相反，让我们通过上面的条件来定义 v；显然 v 是可对角化的，并且 u - v 是幂零的。根据VII、p. 34的命题7，存在多项式q，使得对于所有x ∈ E，x在M中的分量为q_α(u).x。则 v = Σ αq_α(u)；这意味着 u 和 v 交换并完成证明。

B) 现在让我们回到 Th 的证明。 1.

首先，假设 u 可以写成形式 s + n，其中 s 绝对半单，n 幂零，并且 s 和 n 可交换。设 Ω 为 K 的代数闭包；那么 u_{(Ω)} = s_{(Ω)} + n_{(Ω)}，其中 s_{(Ω)} 可对角化，n_{(Ω)} 幂零，并且其中 s_{(Ω)} 和 n_{(Ω)} 可交换；由引理 4 可知 s_{(Ω)} 以及 s 都是唯一的，Ω[X] 重合中的多项式 χ_{u_{(Ω)}} 和 χ_{s_{(Ω)}} 是唯一的，因此多项式 χ_u 和 χ_s 也是唯一的，并且 s 可以表示为 u 中的多项式系数以 Ω 为单位。这首先表明 u 的特征值与 s 的特征值相同，因此在 K 上可分离（VII，p. 42，命题 15）；在加法中，由于 s 是 u 幂的 0 线性组合，因此它也是这些相同幂（II，p. 311，命题 19）的 K 线性组合，并且存在多项式 P ∈ K[X]，使得 s = P(u)，因此 n = Q(u)其中 Q(X) = X - P(X)。现在让我们证明 Q（以及 P）可以在没有常数项的情况下选择。如果 u 可逆，则其特征多项式具有非零的常数项，并且凯利-汉密尔顿定理（III，p. 541，命题 20）表明 1 可以表示为 u 中的多项式，没有常数项，因此断言成立案例。如果 u 不可逆，则其核 W 为非零的，且在 n (VII, p. 41, 引理 3) 下闭；由于n到W的限制是幂零的，所以W中存在向量 x ≠ 0，使得u(x) = n(x) = 0，这表明Q 不能有一个常数项。

相反，假设 u 的特征值在 K 上是可分的，并令 L 为 K 包含这些特征值的有限伽罗瓦扩张。到引理 4，我们可以写出 u_{(L)} = v + w，其中 v 可对角化，w 幂零，且 vw = wv。令B为E的基，令B'为L⊗_K E的相应的基，并令U、V、W为关于B'的u_{(L)}、v、w的矩阵； 注 U 也是 u 相对于 B 的矩阵，因此在 K 中有条目。对于 L 的每个 K 自同构 σ，以及每个在 L 中有条目的矩阵 A，令 A" 表示通过应用 σ 对 A 的条目获得的矩阵。令 a 为 a L 的 K 自同构；则 U = U^σ = (V + W)^σ = V^σ + W^σ, V^σW^σ = (VW)^σ = (WV)^σ = W^σV^σ；因为 Vu 是可对角化的矩阵自同态和 W" 是幂零的，从引理 4 可以得出 Vu = V 且 W^σ = W。由于这对于所有 σ 都有效，因此 V 和 W 的条目在 K 中；如果$u_s$和$u_n$是E与矩阵V和W相对于B的自同态，则$(u_s)_{(L)} = v$和$(u_n)_{(L)} = w$。由此可见，$u_s$绝对是半单，$u_n$幂零，$u_s$和$u_n$可交换，$u = u_s + u_n$。这样就完成了证明。

每当自同态f承认Jordan分解时，我们将其写为$(f_s, f_n)$，自同态、$f_s$和$f_n$分别称为绝对*半单*分量和幂零分量。当K完美时，每个自同态都有一个乔丹分解；在这种情况下，绝对半单自同态和半单自同态之间也没有区别，我们有时说“半单分量”为“绝对半单分量”。

#### 推论 1 {#alg-vii-s5-lem-4-cor-1 .statement tag=076Z}

假设$u$有一个乔丹分解，并让L是K的扩张。那么$u_{(L)}$有一个乔丹分解，还有$(u_{(L)})_s = (u_s)_{(L)}$和$(u_{(L)})_n = (u_n)_{(L)}$。

#### 推论 2 {#alg-vii-s5-lem-4-cor-2 .statement tag=0770}

假设你有一双 Jordan 分解。那么与 u *通勤*的 E 的每个 *自同态* 也与 $u_s$ 和 $u_n$ 通勤。

#### 推论 3 {#alg-vii-s5-lem-4-cor-3 .statement tag=0771}

设$u$和$v$为E的两个通勤自同态，其中有乔丹分解。
a) 自同态 $u, v, u_s, v_s, u_n, v_n, v,$ 全部通勤。
b) 自同态 $u + v$ 和 $uv$ 有乔丹分解与
$$
(u + v)_s = u_s + v_s , \quad (u + v)_n = u_n + v_n , \quad (uv)_s = u_s v_s ,
$$
$$
(uv)_n = u_s v_n + u_n v_s + u_n v_n .
$$
部分 a) 源自 Cor. 2. 为了证明部分 b)，只要注意$u_s + v_s$和$u_s v_s$绝对是半单（VII，p. 43，Cor.）并且$u_n + v_n$和$u_s v_n + u_n v_s + u_n v_n$是幂零的（如通勤的和） 幂零自同态）。

#### 推论 4 {#alg-vii-s5-lem-4-cor-4 .statement tag=0772}

假设$u$有一个Jordan分解，并令R为$\mathbf{K}[X]$中的多项式。然后自同态$R(u)$有乔丹分解和$R(u)_s = R(u_s)$。

#### 注 1 {#alg-vii-s5-n9-rem-1 .statement tag=0773}

我们有$\det(u_s) = \det(u)$和$\operatorname{Tr}(u_s) = \operatorname{Tr}(u)$。

#### 注 2 {#alg-vii-s5-n9-rem-2 .statement tag=0774}

$u$ 可三角化的必要且充分的条件是 $u$ 具有可对角化的 Jordan 分解，且 $u_s$ 可对角化。 Then there exists a basis of E with respect to which the matrix of $u$ is lower triangular, and that of $u_s$ is diagonal, with the same diagonal as the matrix of $u$ (cf. Lemma 4 and Prop. 19 below).
Note however that if the matrix of $u$ with respect to some basis is triangular, it does not in general follow that the matrix of $u_s$ with respect to the same basis is diagonal.

#### 注 3 {#alg-vii-s5-n9-rem-3 .statement tag=0775}

约旦分解的概念对于平方矩阵可以用类似的方式定义。对于例，对于 Jordan 矩阵 $U_{m,\alpha}$，我们有
$$
(U_{m,\alpha})_s = \alpha \cdot I_m , \quad (U_{m,\alpha})_n = U_{m,0} .
$$

#### 注 4 {#alg-vii-s5-n9-rem-4 .statement tag=0776}

如果$u$是半单但不是绝对半单，那么它就没有乔丹分解。

向量空间 $V$超过交换域的自同态$u$被认为是单能的，如果自同态$u - \mathrm{Id}$是幂零的，即如果存在整数$r$使得$(u - \mathrm{Id},)' = 0$；那么$u$是$V$的自同构，因为如果$u = \mathrm{Id}, - n$和$n' = 0$，那么
$$
(\mathrm{Id}, + n + \ldots + n^{r-1})\ u = u (\mathrm{Id}_V + n + \ldots + n^{r-1}) = \mathrm{Id}_V .
$$
如果$V$有有限维$m$，那么$u$是单能的当且仅当$\chi_u(X) = (X - 1)^m$（VII，p. 33，Cor.3到Prop.5）。

#### 命题 17 {#alg-vii-s5-prop-17 .statement tag=0777}

— 令$E$为交换域上的有限维向量空间，并令$f$为$E$的自同态。那么下面的条件是等价的：
(i) $f$ 有 Jordan 分解并且是自同构 ；
(ii) $f$ 有 Jordan 分解并且 $f_s$ 是自同构 ；
(iii) 存在$E$的绝对半单自同构$a$和$E$的单能自同态$u$，使得$f = ua = au$。
而且，在这些条件下，在(iii)的记号中，我们必须有$a = f_s$和$u = 1 + f_s^{-1}f_n$。
(i) $\Rightarrow$ (ii)：这是从注 1 得出的。
(ii) $\Rightarrow$ (iii)：取$a = f_s$和$u = 1 + f_s^{-1}f_n$；那么$f = ua = au$，而$a$绝对是半单自同构，$u$是单能的。
(iii) $\Rightarrow$ (i)：在(iii)的记号中，取$n = a(u - 1) = (u - 1)a$。那么$an = na$和$f = a + n$，并且$n$是幂零的。由此可见，$(a, n)$是$f$的乔丹分解。这意味着 (i) 以及关系 $a = f_s$ 和 $u = 1 + f_s^{-1}f_n$。

放入$f_r = f_s^{-1}f = ff_s^{-1} = 1 + f_s^{-1}f_n$，并称其为$f$的单能分量。 对 $(f_s, f_r)$ 通常被称为自同构 $f$ 的乘法 Jordan 分解。

#### 命题 18 {#alg-vii-s5-prop-18 .statement tag=0778}

— 令$E$为交换域$K$上的有限维向量空间，令$u$为$E$的自同态，令$E'$为$u$下封闭的$E$的子空间。令 $u'$（分别为 $u''$）为由 $u$ 诱发的 $E'$（分别为 $E/E'$）的自同态。然后$\chi_u = \chi_{u'} \cdot \chi_{u''}$。

对于$u$来说，要拥有乔丹分解，$u'$和$u''$有是充分必要的；此外，如果这成立，则$u'$和$u''$的绝对半单（或幂零）分量是由$u$的绝对半单（或幂零）分量引起的$E'$和$E/E'$的自同态。

令 $B$ 为$E$ 包含基 $B'$ $E'$ 的基，并令$B''$ 为基

$E'' = E/E'$ 是 $B - B'$ 中的像。令$U, U', U''$分别为$u, u', u''$相对于$B, B', B''$的矩阵。那么$U$有形式

$$
\begin{pmatrix}
U' & Z \\
0 & U''
\end{pmatrix}
$$

和 $\chi_u = \chi_U = \chi_{U'}\chi_{U''} = \chi_{u'}\chi_{u''}$（cf. III、p. 533，例 2）。我们推导出$u$的特征值集合是$u'$和$u''$的特征值集合并。如果$u'$和$u''$有乔丹分解，那么$u'$和$u''$的特征值在K上是可分离的，因此$u$的特征值也是可分离的，$u$有乔丹分解（VII， p. 43，第 1)。相反，如果 $u$ 有 Jordan 分解 $(s, n)$，则 $s$ 和 $n$ 使 $E'$ 保持不变，因为它们是 $u$ 中的多项式；让$s', n', s'', n''$分别表示由$s, n, s, n$引起的$E', E', E'', E''$的自同态。那么$s'$和$s''$绝对是半单，因为它们的最小多项式除是$s$的（VII，p. 42，命题15）； $n'$ 和 $n''$ 也是幂零的。最后$u' = s' + n', u'' = s'' + n'', s'n' = n's', \text{ and } s''n'' = n''s''$，完成证明。

#### 命题 19 {#alg-vii-s5-prop-19 .statement tag=0779}

— *令 E 为交换域 K 上的有限维向量空间，并令 $\mathscr{S}$ 为 E 的可交换三角化自同态的集合。则存在 E 的基，相对于每个元素 u 的矩阵 $\mathscr{S}$是下三角，$u_s$的矩阵是对角线，与u的对角线元素相同。*

由科. $\mathfrak{T}$ 元素的绝对半单分量中的 VII、p. 4.5、集合 $\mathfrak{T}_s$ 中的 3 个由可对角化的元素组成，它与 1 个另一个交换，因此是可对角化的（VII，p. 41，第 13 条命题），$\mathscr{S}$ 元素幂零分量的集合 $\mathfrak{T}_n$ 由幂零元组成，幂零元可与一个另一个交换，$\mathfrak{T}_n$ 的每个元素每元素 $\mathfrak{T}_s$ 通勤。根据第 13 条命题的证明（VII，p. 41），我们发现存在 E 的分解作为子空间 $E_i$ 的直和，它们在 $\mathfrak{T}_s$ 和 $\mathfrak{T}_n$ 下是不变的，因此$\mathscr{S}$的每个元素中的限制，对于每个$E$，是位似。 替换 $E$ 除以$E$，反过来，我们可以假设 $\mathscr{S}$ 的元素是同位；足以证明存在E的基，相对于$\mathfrak{T}_n$的元素，由对角线为零的下三角形矩阵表示；因此，我们被简化为 $\mathscr{S}$ 由幂零元组成的情况。

现在假设$E \neq 0$，并令F为$E$的非零的子空间，在$\mathfrak{T}$下不变，最小为维数。那么对于每个$u \in \mathfrak{T}$，$u$到F的限制核为非零的且在$\mathfrak{T}$下不变（VII，p. 41，引理3）；通过 $u$ 的 F 限制到 F 的选择因此对于所有 $u \in \mathfrak{T}$ 来说是零。令 $x \in F,\ x \neq 0$；那么 $u(x) = 0$ 对于所有 $u \in \mathscr{S}$；通过归纳对E的维数进行论证，我们可以假设存在商$E' = E/Kx$的基$(\bar{e}_1, ..., \bar{e}_{n-1})$，这样，对于所有$u \in \mathfrak{T}$，$E'$的自同态$\bar{u}$由$u$ 相对于基有矩阵，它是对角线为零的下三角形；如果$e_i \in E$投影到a上，对于$i = 1, ..., n-1$，则基$(e_1, ..., e_{n-1}, x)$满足所需的条件。

习题

### 习题 {#alg-vii-s5-exercises}

这个截面中的所有域都是可交换的除非，否则明确说明。

参见[习题为 § 5](exercises/s5/)。
