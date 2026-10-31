---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 9
section_title: Norms and traces
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 541-550, 644
pdf_pages: 0565-0574, 0668-0668
extraction: ocr
subsections:
    - "no": 1
      title: NORMS AND TRACES RELATIVE TO A MODULE
      page: 541
      pdf_page: 565
    - "no": 2
      title: PROPERTIES OF NORMS AND TRACES RELATIVE TO A MODULE
      page: 542
      pdf_page: 566
    - "no": 3
      title: NORM AND TRACE IN AN ALGEBRA
      page: 543
      pdf_page: 567
    - "no": 4
      title: PROPERTIES OF NORMS AND TRACES IN AN ALGEBRA
      page: 545
      pdf_page: 569
    - "no": 5
      title: DISCRIMINANT OF AN ALGEBRA
      page: 549
      pdf_page: 573
statements: 13
exercises: 1
content_sha256: 4074dd703287061157ff204e9bfae0c05cb78b68b5c8c6f9ddd9e86f244feb60
translated_from: content/en/alg/III/09_s9_norms_and_traces.md
translation_method: google
source_content_sha256: 35d7c75abeb9436ab650b86c4903e3125e8d6a5b2a7afd81b6be25b654009b6d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 02295e618b36bcdfdf21c33a01a5ff9185815fd1ce92289702e2a0da31fa923e
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 9。 范数和痕迹

在本段中，$K$将表示交换环，$A$表示单位结合代数$K$代数。每个$A$-模块将被假定为通过将标量限制为$K$而获得的$K$-模块结构。

### 1. 范数以及与模相关的痕迹

#### 定义 1 {#alg-iii-s9-def-1 .statement tag=065S}

设 $M$ 为 $A$ 模，承认有限基作为 $K$ 模。对于所有$a \in A$，令$a_M$为$K$模块$M$的自同态$x \mapsto ax$。 $a_M$的迹、行列式和特征多项式分别称为$z$相对于$M$的迹、范数和特征多项式。

因此$a$的迹和范数是$K$的元素，分别用$\operatorname{Tr}_{M/K}(a)$和$N_{M/K}(a)$表示； $a$的特征多项式为$K[X]$的元素，记为$\mathrm{Pc}_{M/K}(a; X)$。为了避免混淆，我们在上面的记号中省略了$K$。

根据自同态（II, § 4, no. 3和§ 8, no. 1）的迹和行列式的性质，我们得到关系

$$
\operatorname{Tr}_M(a + a') = \operatorname{Tr}_M(a) + \operatorname{Tr}_M(a')
$$

(2) $\mathrm{Tr}_M(aa') = \mathrm{Tr}_M(a'a)$
(3) $N_M(aa') = N_M(a)N_M(a')$

对于$A$中的所有$a, a'$。

就该基而言，令$(e_i)_{1 \leq i \leq n}$为$K$模块$M$的基以及自同态$a_M$的$(m_{ij}(a))$矩阵。 函数 $m_{ij}$ 是 $K$ 模块 $A$ 上的线性形式并且

(4) $\mathrm{Tr}_M(a) = \sum_{i=1}^n m_{ii}(a)$
(5) $N_M(a) = \det(m_{ij}(a))$
(6) $\mathrm{Pc}(a; X) = \det(\delta_{ij}X - m_{ij}(a)).$

由计算行列式 (§ 8, no. 11, 公式 (50)) 的方法得出：

(7) $\mathrm{Pc}_M(a; X) = X^n + c_1 X^{n-1} + \cdots + c_n$

哪里

(8) $c_1 = -\mathrm{Tr}_M(a), \quad c_n = (-1)^n N_M(a).$

对于$\lambda \in K$，

(9) $\mathrm{Tr}_M(\lambda) = n.\lambda, \quad N_M(\lambda) = \lambda^n, \quad \mathrm{Pc}_M(\lambda; X) = (X - \lambda)^n.$

设$K'$是可交换的$K$代数。令$M' = K' \otimes_K M$和$A' = K' \otimes_K A$，使得$M'$具有$A'$模块结构（§ 4，例2）。作为$K'$-模块$M'$承认$1 \otimes e_i$（$1 \leq i \leq n$）的基由……组成和$a_M$的矩阵相对于$(e_i)$等于$(1 \otimes a)_M'$的矩阵关于$(e'_i)$。然后

(12) $\mathrm{Tr}_{M'}(1 \otimes a) = \mathrm{Tr}_M(a).1, \quad N_{M'}(1 \otimes a) = N_M(a).1$
        $\mathrm{Pc}_{M'}(1 \otimes a; X) = \mathrm{Pc}_M(a; X).1$

对于所有 $a \in A$，其中 1 表示 $K'$ 的单位元。如果特别我们取 $K' = K[X]$，那么

(13) $\mathrm{Pc}_{M/K}(a; X) = N_{M[X]/K[X]}(X - a).$

### 2. 范数的性质以及相对于模的迹线

如果$M$和$M'$是两个*同构的*$A$模，且在$K$上具有有限基，那么，对于所有$a \in A$，

(14) $\mathrm{Tr}_{M'}(a) = \mathrm{Tr}_M(a), \quad N_{M'}(a) = N_M(a), \quad \mathrm{Pc}_{M'}(a; X) = \mathrm{Pc}_M(a; X)$

因为如果$f$是$M$的同构到$M'$，则$a_M$的矩阵相对于$M$的基$B$在$K$上与$a_{M'}$的矩阵相同相对于$M'$的基$f(B)$。

#### 命题 1 {#alg-iii-s9-prop-1 .statement tag=065T}

令$M = M_0 \supset M_1 \supset \ldots \supset M_r = \{0\}$为$A$模块$M$的子模的递减序列，使得每个$K$模块$P_i = M_{i-1}/M_i$（$1 \leq i \leq r$）承认有限的基。那么$K$-模$M$承认有限的基并且

$$
\operatorname{Tr}_M(a) = \sum_{i=1}^r \operatorname{Tr}_{P_i}(a), \qquad N_M(a) = \prod_{i=1}^r N_{P_i}(a)
$$
(15)

$$
P_{C_M}(a; X) = \prod_{i=1}^r P_{C_{P_i}}(a; X).
$$

令$B'_i$为$P_i$除$K$的基；那么$B'_i$（模$M_i$）的代表$B_i$的系统就是$K$-模块$M_{i-1}$中$K$-模块$M_i$的补子模的基（II, § 1, no. 11， 命题21）。 $B_i$($1 \leq i \leq r$)的并$B$比$K$是$M$的基。令$X_{tt}$为自同态$a_{P_i}$相对于基$B'_i$的矩阵。 $a_M$的矩阵相对于$B$是形式的直接的

$$
\begin{pmatrix}
X_{rr} & X_{r,r-1} & \cdots & X_{r,1} \\
0 & X_{r-1,r-1} & \cdots & X_{r-1,1} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & X_{11}
\end{pmatrix}
$$

命题由no. 1的公式(4)、(5)和(6)以及§ 8, no. 6的公式(31)得出。

#### 命题 2 {#alg-iii-s9-prop-2 .statement tag=065U}

令$A, A'$为两个$K$代数，$M$为$A$模，$M'$为$A'$模。假设$M$和$M'$分别是维数、$n$和$n'$的自由$K$模块，并将$M \otimes_K M'$视为$(A \otimes_K A')$模块（$§ 4$、no. 3、例） 2）。然后，对于$a \in A$和$a' \in A'$，

$$
\operatorname{Tr}_{M \otimes M'}(a \otimes a') = \operatorname{Tr}_M(a) \operatorname{Tr}_{M'}(a')
$$
(16)

$$
N_{M \otimes M'}(a \otimes a') = (N_M(a))^{n'} (N_{M'}(a'))^n.
$$
(17)

公式 (16) 源自II, § 4, no. 4、公式 (26)，公式 (17) 源自§ 8, no. 6、公式 (33)。

### 3. 范数并在代数中追踪

#### 定义 2 {#alg-iii-s9-def-2 .statement tag=065V}

令 $A$ 为 $K$ 代数，它是有限维自由 $K$ 模。对于每个元素$a \in A$，跟踪（分别为范数，\脚注{†这个概念不应与概念相混淆，因为代数中的范数超过了值域（\emph{一般拓扑}）， $a$相对于$A$和$K$的IX, § 3, no. 7.}分别是特征多项式）是$K$模$A$的自同态$x \mapsto ax$的迹（分别是行列式、特征多项式）。

$a \in A$相对于$A$和$K$的迹、范数和特征多项式分别用$\mathrm{Tr}_{A/K}(a)$、$N_{A/K}(a)$和$\mathrm{Pc}_{A/K}(a; X)$表示；当不存在混淆风险时，我们会从记号中省略 $K$ 甚至 $A$。 注 $a \in A$ 的迹（分别为范数，特征多项式）正是$a$ 相对于$A$-模$A_s$ 的迹（分别为范数，特征多项式）。

假设 $A$ 是 $K$ 上的有限数有限维代数的乘积 $A_1 \times A_2 \times \cdots \times A_m$，它们是自由的 $K$ 模块。使用上面的注和命题 1 of no. 2，我们有，对于每个元素

$$
a = (a_1, \ldots, a_m) \in A,
$$

$$
\mathrm{Tr}_{A/K}(a) = \sum_{i=1}^m \mathrm{Tr}_{A_i/K}(a_i), \qquad N_{A/K}(a) = \prod_{i=1}^m N_{A_i/K}(a_i)
$$
(18)

$$
\mathrm{Pc}_{A/K}(a; X) = \prod_{i=1}^m \mathrm{Pc}_{A_i/K}(a_i; X).
$$

类似地，no. 2的命题 2表明，如果$A$和$A'$分别是$K$上的有限维和$n, n'$的两个代数（它们是免费的$K$模块），则对于$a \in A, a' \in A'$。

$$
\mathrm{Tr}_{A \otimes A'}(a \otimes a') = \mathrm{Tr}_A(a) \, \mathrm{Tr}_{A'}(a')
$$
(19)

$$
N_{A \otimes A'}(a \otimes a') = (N_A(a))^{n'} (N_{A'}(a'))^n.
$$
(20)

Finally let $A$ be a finite-dimensional algebra over $K$ which is a free $K$-module, $h$ a homomorphism of $K$ into a commutative ring $K'$ and $A' = A_{(K')}$ the $K'$-algebra derived from $A$ by extending the scalars by means of $h$. 从 no. 1 的公式 (12) 可以得出，对于所有 $a \in A$，

$$
\mathrm{Tr}_{A'/K'}(1 \otimes a) = h(\mathrm{Tr}_{A/K}(a)), \qquad N_{A'/K'}(1 \otimes a) = h(N_{A/K}(a))
$$
(21)

$$
\mathrm{Pc}_{A'/K'}(1 \otimes a; X) = \bar{h}(\mathrm{Pc}_{A/K}(a; X))
$$

其中$\bar{h}$是同态$K[X] \to K'[X]$源自$h$。特别是，对于$K' = K[X]$，我们得到，写成$A[X] = A \otimes_K K[X]$，

$$
\mathrm{Pc}_{A/K}(a; X) = N_{A[X]/K[X]}(X - a).
$$
(22)

更一般地，如果 $K'$ 是可交换的 $K$ 代数和 $A' = A \otimes_K K'$，那么，对于所有 $x \in A'$，

$$
\mathrm{Pc}_{A/K}(a; x) = N_{A'/K'}(x - a).
$$

#### 例 {#alg-iii-s9-n3-exa-1 .statement tag=065W}

(1) Let $A$ be a quadratic algebra over $K$ of type $(\alpha, \beta)$ and $(e_1, e_2)$ a basis of type $(\alpha, \beta)$ (§ 2, no. 3). 对于 $x = \xi e_1 + \eta e_2$、$\mathrm{Tr}_{A/K}(x) = 2\xi + \beta \eta$ 和 $N_{A/K}(x) = \xi^2 + \beta \xi \eta - \alpha \eta^2$；因此，这些函数与 $x$ (§ 2, no. 24) 的凯莱迹和范数相同。

(2) 设 $A$ 为四元数代数大于 $K$。直接计算使我们能够验证 $\mathrm{Tr}_{A/\mathbf{K}}(x) = 2T(x)$ 和 $N_{A/\mathbf{K}}(x) = (N(x))^2$，其中 T 和 N 是凯莱迹和范数 (§ 2, no. 4)。

(3) 令A(II, § 10, no. 3)的$A = \mathbf{M}_n(\mathbf{K})$和典范基$(E_{ij})$按字典顺序排列阶。 然后立即看出，对于自同态$Y \mapsto XY$的每个矩阵$X = \sum_{i,j} \xi_{ij} E_{ij}$矩阵（阶$n^2$）来说，形式

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

从而$\mathrm{Tr}_{A/\mathbf{K}}(X) = n \cdot \mathrm{Tr}(X)$和$N_{A/\mathbf{K}}(X) = (\det(X))^n$。

### 4. 范数的性质以及代数中的迹线

#### 命题 3 {#alg-iii-s9-prop-3 .statement tag=065X}

*设 A 为 K-代数，承认有限的基。为了使元素 $a \in A$ 可逆，其 $N_{A/\mathbf{K}}(a)$ 在 $\mathbf{K}$ 中可逆是充分必要的。*

如果$a$在$A$中承认逆$a'$，那么

$$
N_{A/\mathbf{K}}(a) N_{A/\mathbf{K}}(a') = N_{A/\mathbf{K}}(aa') = N_{A/\mathbf{K}}(1) = 1
$$

由 no. 1 的公式 (3) 获得。相反，如果 $N_{A/\mathbf{K}}(a)$ 可逆，则自同态 $h : x \mapsto ax$ 是双射 (§ 8, no. 2, 定理 1)。那么存在$a' \in A$使得$aa' = 1$；那么 $h(a'a - 1) = aa'a - a = (aa' - 1)a = 0$, 从而 $aa' = 1$ 因为 $h$ 是单射的。因此$a'$是$a$的倒数。

#### 命题 4 {#alg-iii-s9-prop-4 .statement tag=065Y}

*设 A 为 K-代数，承认有限的基。对于所有 $a \in A$、$\mathrm{Pc}_{A/\mathbf{K}}(a; a) = 0$。*

这紧随 Cayley-Hamilton 定理（§ 8, no. 11、命题 20）而来。

#### 命题 5 {#alg-iii-s9-prop-5 .statement tag=065Z}

*设A为K-代数，m为A的双向理想。假设$A_0 = A/m$是有限维n的自由K-模，存在整数$r > 0$，使得$m^r = \{0\}$且$m^{i-1}/m^i$是$A_0$的自由模有限维$s_i$对应$1 \leq i \leq r$。让$s = s_1 + \cdots + s_r$和所有$a \in A$让$a_0$表示类对$a$模。米。那么 A 是维数 $ns$ 中的自由K-模，并且对于所有 $a \in A$，

$$
\mathrm{Tr}_A(a) = s \cdot \mathrm{Tr}_{A_0}(a_0), \qquad N_A(a) = (N_{A_0}(a_0))^s
$$
$$
\mathrm{Pc}_A(a; X) = (\mathrm{Pc}_{A_0}(a_0; X))^s.
$$

由于II, § 1, no. 13、命题25，$m^{i-1}/m^i$是维数$ns_i$中的自由K-模。因此，no. 2中的命题 1可以与$P_i = m^{i-1}/m^i$一起应用；

这首先表明 $A$ 是维数 $n(s_1 + \cdots + s_r) = ns$ 的免费 $K$ 模块。此外，假设意味着$A$-模块$P_i$同构于$s_i$的直和，子模同构于$A$-模块$A_0$； 命题 1 / no. 2，因此 $N_{P_i}(a) = N_{A_0}(a)^{s_i}$；最终因此
$$
N_A(a) = N_{A_0}(a)^s.
$$
在此，通过将$A_0$视为左$A$模来定义公式$N_{A_0}(a)$，并且它等于$A_0$的$K$线性映射$x \mapsto ax$到自身的行列式；但是，如$ax = a_0x$代表$x \in A_0$，$N_{A_0}(a) = N_{A_0}(a_0)$，它完成证明或公式（23）的范数。其他两个的显示方式类似。

#### 命题 6 {#alg-iii-s9-prop-6 .statement tag=0660}

*设$A$是一个可交换的$K$-代数，在$K$上承认有限的基，而$V$是在$A$上承认有限的基的$A$模。那么$V$在$K$上承认有限的基，并且对于$V$的每个$A$-自同态$u$，如果$u_K$是映射，$u$被视为$K$-自同态$V$,*
$$
\begin{align*}
\operatorname{Tr}(u_K) &= \operatorname{Tr}_{A/K}(\operatorname{Tr}(u)), \qquad \det(u_K) = N_{A/K}(\det(u)) \\
\operatorname{Pc}(u_K; X) &= N_{A[X]/K[X]}(\operatorname{Pc}(u; X)).
\end{align*}
$$
(24)

设$(a_i)_{1 \leq i \leq m}$为$A$之基超过$K$且$(e_j)_{1 \leq j \leq n}$基超过$V$超过$A$；那么 $(a_i e_j)$ 是 $V$ 的基超过 $K$（II, § 1, no. 13，命题 25）。另一方面，公式 (24) 的第三个可以从应用于$A[X]$-模$A[X] \otimes_A V$ (§ 8, no. 10) 的自同态 $X - \bar{u}$ 的第二个推导出来。因此，只需显示 (24) 中的前两个公式即可。我们首先建立以下引理：

#### 引理 1 {#alg-iii-s9-lem-1 .statement tag=0661}

*令 $X_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq n$) 为 $n^2$ 不定式，$X$ 平方矩阵 $(X_{ij})$ 为阶 $n$，$D(X_{11}, \ldots, X_{nn}) \in \mathbf{Z}[X_{11}, \ldots, X_{nn}]$ 为行列式 $\det(X)$。另一方面，令 $A$ 为交换环，$M_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq n$) $n^2$ 矩阵 of 阶 $m$ over $A$，它们是成对可置换的，并且 $M$ 阶 $mn$超过$A$的平方矩阵可以表示为矩阵的平方矩阵（II, § 10, no. 7）
$$
M = \begin{pmatrix}
M_{11} & M_{12} & \cdots & M_{1n} \\
M_{21} & M_{22} & \cdots & M_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
M_{n1} & M_{n2} & \cdots & M_{nn}
\end{pmatrix}
$$
那么$M$的行列式等于平方矩阵的行列式
$$
D(M_{11}, \ldots, M_{nn})
$$
阶$m$。

我们在$n$上按归纳继续，$n = 0$和$n = 1$的情况很简单。

设 $Z$ 为新的不定式，$N_{ij}$ 矩阵 $M_{ij} + \delta_{ij} Z I_m$（$\delta_{ij}$ Kronecker 指标）。如果 $D^{ij}(X_{11}, \ldots, X_{nn})$ 是矩阵 $X$ (§ 8, no. 6) 中$X_{ij}$的*辅因子*，则

$$
\text{(25)} \quad X_{ji} D^{ki}(X_{11}, \ldots, X_{nn}) = \delta_{jk} D(X_{11}, \ldots, X_{nn})
$$

（§ 8, no. 6，公式（28））。我们写 $N'_{ij} = D^{ij}(N_{11}, \ldots, N_{nn})$，即阶 $m$ 与 $\mathbf{A}[Z]$ 的平方矩阵，并考虑乘积 $N . U$，其中

$$
U = \begin{pmatrix}
N'_{11} & 0 & \cdots & 0 \\
N'_{12} & I_m & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots \\
N'_{1n} & 0 & \cdots & I_m
\end{pmatrix},
$$
$$
N = \begin{pmatrix}
N_{11} & N_{12} & \cdots & N_{1n} \\
N_{21} & N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
N_{n1} & N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

在块 (II, § 10, no. 5) 中执行乘积并使用公式 (25)，我们得到

$$
N . U = \begin{pmatrix}
P & N_{12} & \cdots & N_{1n} \\
0 & N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots & \cdots \\
0 & N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

我们写了$P = D(N_{11}, \ldots, N_{nn})$。让

$$
Q = \begin{pmatrix}
N_{22} & \cdots & N_{2n} \\
\cdots & \cdots & \cdots \\
N_{n2} & \cdots & N_{nn}
\end{pmatrix}
$$

即矩阵 / 阶 $m(n-1)$；那么 (§ 8, no. 6, 公式 (31)) (det $N$) (det $U$) = (det $P$)(det $Q$) 和 det $U = \det N'_{11}$。但由归纳假设、$Q = \det(D^{11}(N_{11}, \ldots, N_{nn})) = \det N'_{11}$并凭借$N_{ij}$的定义，显然$Q$是次数$m(n-1)$的$\mathbf{A}[Z]$中的多项式，其项在$Z^{m(n-1)}$中具有系数1 ;紧接着，在分级的代数 $\mathbf{A}[Z]$ 中，det $Q$ 不是零的除子。因此，我们结论在$\mathbf{A}[Z]$中得到了$N = \det(D(N_{11}, \ldots, N_{nn}))$；如果我们用 0 代替这些多项式中的$Z$，则得到$M = \det(D(M_{11}, \ldots, M_{nn}))$。

示出了这个引理，K-模V是K-模$Ae_j$($1 \leq j \leq n$)的直和；我们写$u(e_j) = \sum_{k=1}^n c_{jk} e_k$。对于每个元素$xe_j \in Ae_j$，对于$x \in A$，$u(xe_j)$在$Ae_k$中的分量是$xc_{jk} e_k$；由此可见，$u_k$的矩阵相对于K-模V的基$(a_i e_j)$可以用矩阵$(M_{jk})$的平方矩阵的形式来表示，其中$M_{jk}$是相对于这两个K-模（II, § 10, no. 5）的基$(a_i e_j)_{1 \leq i \leq m}$和$(a_i e_k)_{1 \leq i \leq m}$，将$Ae_j$的K-线性映射$xe_j \mapsto xc_{jk} e_k$的矩阵转换为$Ae_k$。如果对于所有$t \in A$，$M(t)$表示矩阵，相对于A在K上的基$(a_i)_{1 \leq i \leq m}$，A的自同态$x \mapsto xt$，则$M_{jk} = M(c_{jk})$；因为 $t \mapsto M(t)$ 是环同态矩阵 $M_{jk}$ *可与 1 个另一个* 置换。然后
$$
\det u_K = \det(D(M_{11}, \ldots, M_{nn}))
$$
引理 1。但由于$t \mapsto M(t)$是环同态，$D(M_{11}, \ldots, M_{nn})$是A相对于基$(a_i)$的K-自同态$x \mapsto x.\det(c_{jk})$的矩阵；因此，通过定义，它的行列式是$N_{A/K}(\det(u))$，这证明了（24）的第二个公式。另一方面，
$$
\operatorname{Tr}(u_K) = \sum_{j=1}^n \operatorname{Tr}(M_{jj}) = \sum_{j=1}^n \operatorname{Tr}_{A/K}(c_{jj}) = \operatorname{Tr}_{A/K}\left( \sum_{j=1}^n c_{jj} \right) = \operatorname{Tr}_{A/K}(\operatorname{Tr}(u))
$$
命题 6 中的证明已完成。

#### 推论{#alg-iii-s9-n4-cor-1 .statement tag=0662}

*设 A 交换K-代数在 K 上承认有限基，并且 B A-代数在 A 上承认有限基。然后 B 在 K 上承认有限基，并且，对于所有 $b \in B$ (“传递性公式”)*
$$
\begin{align*}
\operatorname{Tr}_{B/K}(b) &= \operatorname{Tr}_{A/K}(\operatorname{Tr}_{B/A}(b)), \quad N_{B/K}(b) = N_{A/K}(N_{B/A}(b)) \\
P_{C_{B/K}}(b; X) &= N_{A[X]/K[X]}(P_{C_{B/A}}(b; X)).
\end{align*}
$$
(26)
这紧接着命题 6、设定 $V = B$ 和 $u(x) = bx$。

#### 注 {#alg-iii-s9-n4-rem-1 .statement tag=0663}

假设K到A中的同态$\lambda \mapsto \lambda . 1$是单射的，并让K与其在A中的像等同；假设 A 承认有限的基 $(e_i)_{1 \leq i \leq n}$ 为 K-模。令 s 为 A 的自同构，使得 $s(K) = K$。设a为A的元素；然后，通过运输结构
$$
\begin{align*}
\operatorname{Tr}_{A/K}(s(a)) &= s(\operatorname{Tr}_{A/K}(a)) \\
N_{A/K}(s(a)) &= s(N_{A/K}(a)).
\end{align*}
$$
(27) (28)
*还考虑 A 的推导 D ($§ 10$, no. 2)，使得 $D(K) \subset K$ 并在 $\mu_{ji} \in K$ 处写出 $D(e_i) = \sum_{j=1}^n e_j \mu_{ji}$；写*
$$
ae_i = \sum_{j=1}^n e_j \lambda_{ji} \quad \text{with} \quad \lambda_{ji} \in K.
$$

然后
$$
D(a)e_i + aD(e_i) = D(ae_i) = \sum_{j=1}^n (D(e_j)\lambda_{ji} + e_j D(\lambda_{ji})).
$$
由此可见
$$
D(a)e_i = \sum_{j=1}^n e_j v_{ji}
$$
$v_{ji} = D(\lambda_{ji}) + \sum_{k=1}^n (\mu_{jk}\lambda_{ki} - \lambda_{jk}\mu_{ki})$。由于$\sum_{i,k} (\mu_{ik}\lambda_{ki} - \lambda_{ik}\mu_{ki}) = 0$，因此$\operatorname{Tr}_{A/\mathbf{K}}(D(a)) = \sum_{i=1}^n D(\lambda_{ii})$，在其他字
$$
\operatorname{Tr}_{A/\mathbf{K}}(D(a)) = D(\operatorname{Tr}_{A/\mathbf{K}}(a)). *
$$

### 5. 代数的判别式

#### 定义 3 {#alg-iii-s9-def-3 .statement tag=0664}

*设 A 为 K-代数，承认 n 元素的有限基。 A 的 n 元素的序列 $(x_1, \ldots, x_n)$ 对于 K 的判别式，用 $D_{A/\mathbf{K}}(x_1, \ldots, x_n)$ 表示，是平方矩阵* 的判别式
$$
(\operatorname{Tr}_{A/\mathbf{K}}(x_i x_j))_{1 \leq i \leq n, 1 \leq j \leq n}.
$$
首先考虑 A 右 K 的基 $(e_i)_{1 \leq i \leq n}$ 并写
$$
e_i e_j = \sum_{k=1}^n c_{ij k} e_k \quad \text{with} \quad c_{ij k} \in \mathbf{K}.
$$
然后 $\operatorname{Tr}_{A/\mathbf{K}}(e_i) = \sum_{s=1}^n c_{iss}$, 从而 $\operatorname{Tr}_{A/\mathbf{K}}(e_i e_j) = \sum_{k,s} c_{ij k} c_{kss}$ 因此
$$
D_{A/\mathbf{K}}(e_1, \ldots, e_n) = \det \left( \left( \sum_{k,s} c_{ij k} c_{kss} \right)_{1 \leq i \leq n, 1 \leq j \leq n} \right).
$$
现在令$(x_i)_{1 \leq i \leq n}, (x'_i)_{1 \leq i \leq n}$为A的n元素的两个序列，并假设存在阶n、$M = (m_{ij})$的平方矩阵，系数为K，使得$x_i = \sum_{j=1}^n m_{ij} x'_j$对应于$1 \leq i \leq n$。我们写
$$
T = (\operatorname{Tr}_{A/\mathbf{K}}(x_i x_j))_{1 \leq i \leq n, 1 \leq j \leq n}, \qquad T' = (\operatorname{Tr}_{A/\mathbf{K}}(x'_i x'_j))_{1 \leq i \leq n, 1 \leq j \leq n}.
$$
然后$\operatorname{Tr}_{A/\mathbf{K}}(x_i x_j) = \sum_{p,q} m_{ip} m_{jq} \operatorname{Tr}_{A/\mathbf{K}}(x'_p x'_q)$、从而$T = M \cdot T' \cdot {}^t M$；因此，行列式乘法规则给出
$$
\det T = \det M \cdot \det T' \cdot \det {}^t M = (\det M)^2 \det T'
$$
终于从而
$$
D_{A/\mathbf{K}}(x_1, \ldots, x_n) = (\det M)^2 D_{A/\mathbf{K}}(x'_1, \ldots, x'_n).
$$

上述公式特别表明，A的两个基对K的判别式相差K的可逆元的平方，因此生成是K的相同（主要）理想。这个理想$\Delta_{A/K}$称为A对K的判别式理想；由公式 (32) A 的 n 个元素中的每个序列的判别式仅在项的阶不同，具有相同的判别式，因为置换矩阵的行列式等于$\pm 1$。

#### 例{#alg-iii-s9-n5-exa-1 .statement tag=0665}

(1) 如果 A 在 K 上是型 $(\alpha, \beta)$ 的二次代数，则（在 § 2, no. 3 的记号中）$\operatorname{Tr}(e_1) = 2, \operatorname{Tr}(e_2) = \beta$，

$$
\operatorname{Tr}(e_2^2) = \alpha \operatorname{Tr}(e_1) + \beta \operatorname{Tr}(e_2) = 2\alpha + \beta^2,
$$

从而$D_{A/K}(e_1, e_2) = \beta^2 + 4\alpha$。

(2) 令$A = K[X]/K[X]P$，其中$P(X) = X^3 + pX + q$，使得如果x是A中X的像，1，x，A在K上的$x^2$形式基和$x^3 = -px - q$。立即可以看出，$\operatorname{Tr}(1) = 3, \operatorname{Tr}(x) = 0, \operatorname{Tr}(x^2) = -2p$，考虑到关系$x^3 = -px - q, \operatorname{Tr}(x^3) = -3q$和$\operatorname{Tr}(x^4) = 2p^2$，从而很容易$D_{A/K}(1, x, x^2) = -4p^3 - 27q^2$。

(3) 令A为K上的型$(\alpha, \beta, \gamma)$的四元数代数和型$(\alpha, \beta, \gamma)$的A的$(1, i, j, k)$基；考虑§ 3, no. 5，公式(30)，很容易发现$\operatorname{Tr}(1) = 4, \operatorname{Tr}(i) = 2\beta, \operatorname{Tr}(j) = \operatorname{Tr}(k) = 0$，则

$$
D_{A/K}(1, i, j, k) = -16\gamma^2(\beta^2 + 4\alpha)^2.
$$

(4) 令 $A = M_n(K)$ 并考虑 A 对 K (II, § 10, no. 3) 的典范基 $(E_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}$。如果对于所有 i 都有 $j \neq i$ 和 $\operatorname{Tr}_{A/K}(E_{ii}) = n$，那么 $\operatorname{Tr}_{A/K}(E_{ij}) = 0$ 就是直接的；毫无疑问，阶$n^2$的矩阵$(\operatorname{Tr}(E_{ij}E_{hk}))$是形式$n.P$，其中P是置换矩阵，从而$D_{A/K}((E_{ij})) = \pm n^{n^2}$。

### 习题 {#alg-iii-s9-exercises}

§ 9](exercises/s9/)参见[习题。
