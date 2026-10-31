---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 1
section_title: Polynomials
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0010-0023, 0095-0096
extraction: ocr
subsections:
    - "no": 1
      title: Definition of polynomials
      page: 0
      pdf_page: 10
    - "no": 2
      title: Degrees
      page: 2
      pdf_page: 11
    - "no": 3
      title: Substitutions
      page: 4
      pdf_page: 13
    - "no": 4
      title: Differentials and derivations
      page: 6
      pdf_page: 15
    - "no": 5
      title: Divisors of zero in a polynomial ring
      page: 9
      pdf_page: 18
    - "no": 6
      title: Euclidean division of polynomials in one indeterminate
      page: 10
      pdf_page: 19
    - "no": 7
      title: Divisibility of polynomials in one indeterminate [^1]
      page: 11
      pdf_page: 20
    - "no": 8
      title: Irreducible polynomials
      page: 13
      pdf_page: 22
statements: 30
exercises: 6
content_sha256: bf24df7812c2a1b2557ce22c619d5c9ab7f80dcd91f7c9ccbde5ebd17e040ce9
translated_from: content/en/alg/IV/01_s1_polynomials.md
translation_method: google
source_content_sha256: f94b9470c6da2e74358afdf52f506465ae49993b41748514c1bc1d675c01f9e6
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: e37b47200fee62418d00255b67a0fff6be3349006f80e83b9302f6be42f2de6a
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 1。多项式

### 1. 定义多项式

令$I$为集合。我们记得（III，p. 452）$I$超过$\mathbf{A}$的免费交换代数由$\mathbf{A}[(X_i)_{i \in I}]$或$\mathbf{A}[X_i]_{i \in I}$表示。这个代数的元素被称为关于不定式$X_i$（或不定式$X_i$）的*多项式*，系数在$\mathbf{A}$中。让我们回想一下，不确定的$X_i$是$i$在$I$上的自由交换代数超过$\mathbf{A}$的典范像； 有时用另一个符号（如 $X'_i, Y_i, T_i$ 等）来表示此像是很方便的。此约定通常由诸如以下的短语引入：“让 $Y = (Y_i)_{i \in I}$ 成为一个不定族”；在这种情况下，相关多项式的代数由$\mathbf{A}[Y]$表示。当$I = \{1, 2, \ldots, n\}$时，写$\mathbf{A}[X_1, X_2, \ldots, X_n]$代替$\mathbf{A}[(X_i)_{i \in I}]$。

对于$\nu \in \mathbf{N}^{(I)}$，我们把

$$
X^\nu = \prod_{i \in I} X_i^{\nu_i}.
$$

那么$(X^\nu)_{\nu \in \mathbf{N}^{(I)}}$就是$\mathbf{A}$模块$\mathbf{A}[(X_i)_{i \in I}]$的基。 $X^\nu$ 在不定式$X_i$ 中称为*单项式*。对于$\nu = 0$，我们获得$\mathbf{A}[(X_i)_{i \in I}]$的单位元。每个多项式 $u \in \mathbf{A}[(X_i)_{i \in I}]$ 都可以用一种方式写成形式

$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$

其中$a_\nu \in \mathbf{A}$和$\alpha_\nu$是零，除了有限的数； $a_\nu$ 称为 $u$ 的*系数*； $\alpha_\nu X^\nu$ 称为 $u$ 的 *项*（通常元素 $\alpha_\nu X^\nu$ 在 $X^\nu$ 中称为项），特别是 $\alpha_0 X^0$ 的项，以 $a_0$ 标识，称为*$u$ 的常数项*。当$\alpha_\nu = 0$时，我们滥用语言说$u$*包含在$X^\nu$中没有元素*；特别是当$\alpha_0 = 0$时，我们说$u$是一个多项式*没有常数项*（III，p. 453）。任何 1 的标量倍数称为*常数多项式*。

设 B 为交换环和 $\rho : A \to B$ 环同态。 我们通过$\rho$将$B[(X_i)_{i \in I}]$视为A-代数。 因此，$A[(X_i)_{i \in I}]$的映射$\sigma$转化为$B[(X_i)_{i \in I}]$，其中变换$\sum \alpha_\nu X^\nu$转化为$\sum \rho(\alpha_\nu) X^\nu$是A-代数的同态；如果$u \in A[(X_i)_{i \in I}]$，我们用$u$的$^\rho u$像来表示有时，这个同态。 将 $B \otimes_A A[(X_i)_{i \in I}]$ 的同态转换为由 $\sigma$ 变换规范定义的 $B[(X_i)_{i \in I}]$，对于每个 $i \in I$、$1 \otimes X_i$ 转换为 $X_i$；这是 B 代数 (III, p. 449) 的同构。

设 M 为自由A-模和基 $(e_i)_{i \in I}$。 代数 $A[(X_i)_{i \in I}]$ 的对称代数 $S(M)$ 恰好存在一个单位同态 $\varphi$，使得每个$i \in I$有$\varphi(e_i) = X_i$，并且这个同态是同构 (III, p. 506）。这个同构据说是规范的。它允许我们将对称代数的某些属性应用于多项式代数。对于例，令$(I_1), \ldots, L$为I的划分。令$\varphi_\lambda$为$P_\lambda = A[(X_i)_{i \in I_\lambda}]$的同态入$P = A[(X_i)_{i \in I}]$，其中变换$X_i$（$P_\lambda$的元素）入$X_i$（P 的元素）。然后将代数$\bigotimes_{h \in L} P_\lambda$的$\varphi_\lambda$定义同态转化为代数P，
而这个同态就是同构（III，p. 503，第9条命题）。

设E为A-模，并放入$E \otimes_A A[(X_i)_{i \in I}] = E[(X_i)_{i \in I}]$。 A-模 $E[(X_i)_{i \in I}]$ 的元素被称为不定式 $X_i$ 中的多项式，其系数在 E 中。 这样的多项式只能以一种方式写为 $\sum_{\nu \in \mathbf{N}^{(I)}} e_\nu \otimes X^\nu$，其中 $e_\nu \in E$ 和 $e_\nu$ 对于除了有限数之外的所有情况都是零后缀；我们经常写$e_\nu X^\nu$而不是$e_\nu \otimes X^\nu$。

### 2.次数

令$P = A[(X_i)_{i \in I}]$为多项式代数。 对于每个整数$n \in \mathbf{N}$，令$P_n$为由单项式$X^\nu$生成的P的子模，使得$|\nu| = \sum_{i \in I} \nu_i$等于n。 那么$(P_n), \ldots$是一个分级，它将$A[(X_i)_{i \in I}]$变成型$\mathbf{N}$的分级代数（III，p. 459）。 The homogeneous elements of degree $n$ in $A[(X_i)_{i \in I}]$ are sometimes called forms of degree $n$ with respect to the indeterminates $X_i$.

当我们处理非齐次多项式次数时，我们同意将自然数的集合$\mathbf{N}$、元素写成$-\infty$以及扩展序关系和$\mathbf{N}$的加法 $\mathbf{N} \cup \{-\infty\}$ 按照以下约定，其中 $n \in \mathbf{N}$，

$$
-\infty < n , \quad (-\infty) + n = n + (-\infty) = -\infty , \quad (-\infty) + (-\infty) = -\infty .
$$

令 $u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu$ 为多项式。 $u$（对于上面定义的型 N 的分级）的次数 n 的齐次分量$u_n$等于$\sum_{|\nu|=n} \alpha_\nu X^\nu$，并且我们显然有$u = \sum_{n \in \mathbf{N}} u_n$。如果$u \neq 0$，$u_n$不都是零，我们将定义$u$的*次数*（或*总计次数*），写成$\deg u$，如数的最大的 $n$使得$u_n \neq 0$；在其他字（III，p. 453）中，对于多索引$\nu$，$u$的次数是整数$|\nu|$的最大的，使得$a_\nu \neq 0$。当$u = 0$时，$u$的次数按照约定为$-\infty$。对于每个整数 $p \in \mathbf{N}$，关系 $\deg u \leq p$ 因此相当于 « $a_\nu = 0$ 对于每个多索引 $\nu$ 和 $|\nu| > p$ »；首一多项式 $u$ 的集合使得 $\deg u \leq p$ 是 $A[(X_i)_{i \in I}]$ 的 A-子模，等于 $P_0 + P_1 + \ldots + P_p$ 和上面的记号。

令 E 为 A-模。族 $(E \otimes P_n)_{n \in \mathbf{N}}$ 是系数为 E 的多项式的模 $E[(X_i)_{i \in I}] = E \otimes_A A[(X_i)_{i \in I}]$ 型 N 的毕业。对于这种情况，我们将上面针对非齐次多项式次数采用的扩展约定。

#### 命题 1 {#alg-iv-s1-prop-1 .statement tag=069O}

*令$u$和$v$为两个多项式。*

(i) 如果 $\deg u \neq \deg v$，*我们有*
$$
u + v \neq 0 \quad \text{and} \quad \deg(u + v) = \sup(\deg u, \deg v).
$$
如果 $\deg u = \deg v$ *我们有* $\deg(u + v) \leq \deg u$。

(ii) *我们有* $\deg(uv) \leq \deg u + \deg v$。
证明是直接的。

设$J \subset I$和$B = A[(X_i)_{i \in I - J}]$；我们将认同$A[(X_i)_{i \in I}]$与$B[(X_i)_{i \in J}]$（III，p. 453f.）。 $u \in A[(X_i)_{i \in I}]$的次数，$B[(X_i)_{i \in J}]$的元素，相对于指标$i \in J$的$X_i$被称为$u$的次数(III，p. 454)。

令 $u = \sum_{k=0}^n a_k X^k \in A[X]$ 为次数 $n$ 的一个不定式的非零多项式。系数$a_n$，即$\neq 0$乘以假设，被称为$u$的*主导系数*。 *A* 首一多项式 $u \neq 0$ 其首项系数等于 1 称为 *monic 首一多项式*。

在次数$p$的单项式的$A[X_1, X_2, \ldots, X_q]$数中，等于$\mathbf{N}^q$的元素$(n_k)_{1 \leq k \leq q}$的数，使得$\sum_{k=1}^q n_k = p$，即$\binom{q+p-1}{p}$
（集合 III，第 15 号提案，p. 182）

更一般地，令 A 为交换幺半群，$(\delta_i)_{i \in I}$，A 的元素族。型 A 存在代数$A[(X_i)_{i \in I}]$的唯一分级，使得每个单项式$X^\nu$为次数$\sum_{i \in I} \nu_i \delta_i$（III，p. 458， 例3)。上面考虑的情况是$A = \mathbf{N}$和$\delta_i = 1$。在一般情况下，为了避免混淆，我们将使用字 « 权 » 代替 « 次数 » 并使用 « isobaric » 代替 « 均质 »。对于例，代数 $A[(X_i)_{i \geq 1}]$ 存在唯一的型 N 分级，使得对于每个整数 $i \geq 1$，$X_i$ 为权 $i$。 权 $n$ 的同量异位元素是形式 $\sum a_{\nu} X^{\nu}$ 的多项式，其中$a_{\nu} = 0$ 代表$\sum_{i \geq 1} i \cdot \nu_i \neq n$。

### 3.代换

令 E 为 $\mathscr{A}$ 上的单位结合律代数和 $x = (x_i)_{i \in I}$ E 的成对可置换元素族。令 $X = (X_i)_{i \in I}$ 为不定式族。根据III，第7条，p. 449，$\mathscr{A}[X]$到$E$存在一个唯一的单位同态$f$，这样每个$i \in I$就有$f(X_i) = x_i$。将$f$下的$\mathscr{A}[X]$的元素$u$像记作$u(x)$，称为将$u$*中的$x_i$替换为$X_i$而得到的E的*元素，或者也可以*值 $u$ $X_i = x_i$*。特别是$u = u((X_i)_{i \in I})$。如果$I = \{1, \ldots, n\}$我们写$u(x_1, \ldots, x_n)$代替$u((x_i)_{i \in I})$。更一般地，如果 M 是 A-模并且 o 是元素

$$
M[(X_i)_{i \in I}] = M \otimes_A \mathscr{A}[(X_i)_{i \in I}],
$$

我们用$v(x)$表示映射$1_M \otimes f$下的$M \otimes_A E = M_{(E)}$中$v$的像。

如果 $\mathscr{A}[X]$ 的同态 $u \mapsto u(x)$ 进入 E 是单射的，我们说族 $x$ 在 $\mathscr{A}$ 上“代数上自由”，或者说 $x_i$ 在 $\mathscr{A}$ 上“代数上独立”。这也意味着单项式 $x^{\nu}$ ($\nu \in \mathbf{N}^{(I)}$) 在 $\mathscr{A}$ 上线性无关。

如果 $\lambda$ 是 E 的单位同态到单位结合词 A-代数 E'，我们有

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i)_{i \in I})) ,
$$

因为$\lambda \circ f$是$\mathscr{A}[X]$的同态进入E'，其中映射$X_i$到$\lambda(x_i)$。

让$u \in \mathscr{A}[X]$。如果$E$是可交换的，$E^1$到E的映射$x \mapsto u(x)$称为$u$（和代数$E$）定义的*多项式函数*；我们将有时表示为$\tilde{u}$（甚至只是$u$）。

令$Y = (Y_j)_{j \in J}$为另一个不定族，并让我们将多项式代数$\mathscr{A}[Y]$视为E。给定$u \in \mathscr{A}[X]$，将$g_i \in \mathscr{A}[Y]$换成$i \in I$，然后放入$g = (g_i)_{i \in I}$；设$u(g) \in \mathscr{A}/[Y]$为将$u$中的多项式$g_i$代入$X_i$得到的多项式。令 $y = (y_j)_{j \in J}$ 为单位结合词 A-代数 E' 的成对可置换元素族； 应用 (1) 将$E$中的$\mathscr{A}$同态$g \mapsto g(y)$代入$E'$，我们得到

$$
(u(g))(y) = u((g_i(y))) .
$$

如果$f = (f_i)_{i \in I} \in (\mathscr{A}[(X_j)_{j \in J}])^I$和$g = (g_j)_{j \in J} \in (\mathscr{A}[(Y_k)_{k \in K}])^J$，我们用$f \circ g$或$f(g)$表示多项式族$(f_i(g))_{i \in I} \in (\mathscr{A}[(Y_k)_{k \in K}])^I$。如果我们将 ${E'}^J$ 的 $\tilde{f}$ 映射 $x \mapsto (f_i(x))_{i \in I}$ 表示为 ${E'}^I$（其中 $E'$ 是单位结合律和可交换的 $A$-代数），则关系 (2) 意味着

$$(3)$$
$$(\mathrm{fog})'' = \tilde{f} \circ \tilde{g}.$$

如果 $h = (h_k)_{k \in K} \in (A[(Z_l)_l \bullet_L])^K$，则由 (2) 得出：

$$(4)$$
$$f \circ (g \circ h) = (f \circ g) \circ h.$$

#### 命题 2 {#alg-iv-s1-prop-2 .statement tag=069P}

*设$a = (a_i)_{i \in I}$，是元素和$A$的家庭，并设$u \in A[X]$。如果$v$是每个$i \in I$用$X_i + a_i$代替$X_i$得到的多项式，则$v$的常数项等于$u(a)$。*

$v$的常数项是通过将$v$中的$X_i$替换为0而得到的，对于每个$i \in I$。因此结果如下（2）。

#### 推论 1 {#alg-iv-s1-prop-2-cor-1 .statement tag=069Q}

*令$m$为多项式$u \in A[X]$的理想，使得$u(a) = 0$。然后 $m$ 由多项式 $X_i - a_i$ 生成（对于 $i \in I$）。*

很明显，每个$i \in I$都有$X_i - a_i \in m$。令$u \in m$和$v$如命题2中那样。由于$v$没有常数项，因此存在$A[X]$和有限支撑中的多项式族$(P_i)_{i \in I}$，使得

$$
v(X) = \sum_{i \in I} X_i \cdot P_i(X).
$$

如果我们对上式中的每个 $i \in I$ 替换 $X_i$ $X_i - a_i$，我们就得到关系形式 $u(X) = \sum_{i \in I} (X_i - a_i) \cdot P'_i(X)$，从而的推论。

#### 推论 2 {#alg-iv-s1-prop-2-cor-2 .statement tag=069R}

*令 $X = (X_i)_{i \in I}$ 和 $Y = (Y_i)_{i \in I}$ 为两个不定族。多项式 $u \in A[X,Y]$ 的集合使得 $u(X,X) = 0$ 是由多项式 $X_i - Y_i$ 生成的 $A[X,Y]$ 的理想值（对于 $i \in I$）。*

这个推论直接来自Cor。 1 在替换 $A$ 与 $A[Y]$ 和 $a_i$ 与 $Y_i$ 上，将 $A[X,Y]$ 解释为 $X_i$ 中的多项式环，系数在 $A[Y]$ 中。

#### 命题 3 {#alg-iv-s1-prop-3 .statement tag=069S}

*令$u \in A[X]$和$X.Z$为多项式环$A[X][Z]$的元素的家庭$(X_iZ)_{i \in I}$。对于每个正整数 $k$，$u(X.Z)$ 中$Z^k$ 的系数是 $u$ 次数 $k$ 的齐次分量。*

在$u$是单项式的情况下证明这个命题就足够了，这样结果就很清楚了。

#### 推论{#alg-iv-s1-n3-cor-1 .statement tag=069T}

*对于次数 $k$ 齐次的多项式 $u \in A[X]$ ，满足以下条件是充分必要的：*

$$
u(X.Z) = u(X) \cdot Z^k.
$$

#### 注 {#alg-iv-s1-n3-rem-1 .statement tag=069U}

— 令 $x \in A^I$ 并令 $f$ 为 $A[X]$ 的映射 $u \mapsto u(x)$ 到 $A$。给定一个$A$-模块$M$，我们将$M[X] = M \otimes_A A[X]$的同态$1 \otimes f$考虑到$M \otimes_A A = M$。对于每个$v \in M[X]$，我们有$(1 \otimes f)(v) = v(x)$。如果$v = \sum_{\nu \in \mathbf{N}^{(I)}} e_\nu X^\nu$，则$v(x) = \sum_{\nu \in \mathbf{N}^{(I)}} x^\nu e_\nu$。

### 4. 微分和推导

设 $B = A[(X_i)_{i \in I}]$，则由 III，p. 569 对于每个 $i \in I$ 存在且仅有一个 B 的 A 导数 $D_i$，使得
$$
D_i X_i = 1 , \quad D_i X_j = 0 \quad \text{for} \quad j \neq i
$$
多项式$D_i P$称为$P$*相对于*$X_i$的*偏导数*；我们也用$D_{X_i} P$或$\frac{\partial P}{\partial X_i}$或$P'_{X_i}$来表示它。通过 III, p. 558, 公式 (21)，对于$\nu = (\nu,) \in \mathbf{N}^{(I)}$，我们有，
$$
D_i (X^\nu) = \begin{cases}
\nu_i X_i^{\nu_i - 1} \prod_{j \in I - \{i\}} X_j^{\nu_j} & \text{if } \nu_i > 0 \\
0 & \text{if } \nu_i = 0
\end{cases}
$$
从 (6) 可以得出，对于任何 $i, j \in I$ 都有 $D_i D_j = D_j D_i$。对于$\nu = (\nu_i)_{i \in I} \in \mathbf{N}^{(I)}$，我们将放置$D^\nu = \prod_{i \in I} D_i^{\nu_i}$和$\nu! = \prod_{i \in I} (\nu_i!)$。在$\mathbf{N}^{(I)}$订购乘积，我们有
$$
D^\nu(X^\mu) = \begin{cases}
\frac{\mu!}{(\mu - \nu)!} X^{\mu - \nu} & \text{if } \nu \leq \mu , \\
0 & \text{if not .}
\end{cases}
$$
当$P$是单个不定$X$中的多项式时，$P$的唯一偏导数写作$DP$或$\frac{dP}{dX}$或$P'$，简称为$P$的*导数*。

再次令$B = A[(X_i)_{i \in I}]$；由III，$B$、$\Omega_A(B)$的A-微分的p. 569 B-模，具有$X_i$的微分家族$(dX_i)_{i \in I}$为基。令$\partial_i$为指标$i$相对于基在$\Omega_A(B)$上的坐标形式。那么 B 的映射 $u \mapsto (\partial_i, du)$ 到自身就是 B 的推导，对于 $j \neq i$，映射 $X_i$ 为 1，$X_j$ 为 0，因此是 $D_i$；在其他字中，我们有
$$
du = \sum_{i \in I} (D_i u) dX_i
$$
每$u \in B$。如果 I 是有限的，$(D_i)_{i \in I}$ 就是 B 的推导 B-模基。

#### 命题 4 {#alg-iv-s1-prop-4 .statement tag=069V}

*设E是结合律、交换律和单位A-代数，$x = (x_i)_{i \in I}$E的元素族，$A[(X_i)_{i \in I}]$和$y = u(x)$的u元素。然后，对于 E 的每个推导 D 到 E 模块，我们有*
$$
Dy = \sum_{i \in I} (D_i u)(x) \cdot Dx_i .
$$

当$u$是单项式时，只要证明命题就足够了，在这种情况下，它可以从III，p. 558，命题6得出。

#### 推论{#alg-iv-s1-n4-cor-1 .statement tag=069W}

— *让$f \in A[X_1, ..., X_p]$和$g_i \in A[Y_1, ..., Y_q]$代表$1 \leq i \leq p$，并写出$h = f(g_1, ..., g_p)$，那么对于$1 \leq j \leq q$我们有*

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j}.
$$

这是第 4 条的特殊情况 $E = A[Y_1, ..., Y_r]$、$x_i = g_i$ 和 $D = \partial / \partial Y_j$。

令$X = (X_i)_{i \in I}$、$Y = (Y_i)_{i \in I}$为两个不相交的不定族，并为$(X_i + Y_i)_{i \in I}$族写出$X + Y$。给定 $u \in A[X]$，考虑 $A[X, Y]$ 的元素 $u(X + Y)$。对于$\nu \in \mathbf{N}^{(I)}$，我们用$A^\nu u$表示$u(X + Y)$中$Y_\nu$的系数，将其视为$Y_i$中的多项式，系数在$A[X]$中。到定义我们有$A^\nu u \in A[X]$并且

$$
u(X + Y) = \sum_\nu (\Delta^\nu u)(X) Y^\nu.
$$

（这里和本号的其余部分，求和扩展到指标集合$\mathbf{N}^{(I)}$除非相反。）

设$a \in A'$，然后在(9)中用$a$代替$X$，用$X - a$代替$Y$，我们得到

$$
u(X) = \sum_\nu (\Delta^\nu u)(a)(X - a)^\nu.
$$

特别是我们有

$$
u(X) = \sum_\nu (\Delta^\nu u)(0) X^\nu.
$$

如果$u, v \in A[X]$，我们有

$$
(uv)(X + Y) = \left( \sum_\nu (\Delta^\nu u)(X) Y^\nu \right) \left( \sum_\rho (\Delta^\rho v)(X) Y^\rho \right)
= \sum_\sigma \left[ \sum_{\nu + \rho = \sigma} (\Delta^\nu u)(X)(\Delta^\rho v)(X) \right] Y^\sigma
$$

因此

$$
\Delta^\sigma(uv) = \sum_{\nu + \rho = \sigma} (\Delta^\nu u)(\Delta^\rho v).
$$

令 $Z = (Z_i)_{i \in I}$ 为另一个不定族。

我们有：

$$
\sum_{\nu} (\Delta^\nu u)(\mathbf{X})(\mathbf{Y} + \mathbf{Z})^\nu = u(\mathbf{X} + \mathbf{Y} + \mathbf{Z})
$$
$$
= \sum_{\sigma} (Au u)(\mathbf{X} + \mathbf{Y})Zu
$$
$$
= \sum_{\rho, \sigma} (\Delta^\rho \Delta^\sigma u)(\mathbf{X}) Y^\rho Z^\sigma u,
$$

因此，我，p. 99，Cor。 2：

(13)
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \; \sigma!} \Delta^{\rho + \sigma} u.
$$

#### 命题 5 {#alg-iv-s1-prop-5 .statement tag=069X}

— *对于任何* $u \in \mathbf{A}[\mathbf{X}]$ *和* $\nu \in \mathbf{N}^{(I)}$ *我们有*

$$
D^\nu u = \nu! \; \Delta^\nu u
$$

首先假设 $\nu$ 有长度 1 ；则 I 存在元素 $i$，使得 I 中所有 $j \neq i$ 存在 $\nu = \varepsilon_i$，即 $\nu_i = 1$ 和 $\nu_j = 0$。 公式 (12) 表明 $A''$ 是 A-代数的推导 $\mathbf{A}[\mathbf{X}]$显然在$X_j$上有值零对于$j \neq i$和值1在$X_i$上。因此，对于每个$i \in I$，我们有$\Delta^{\varepsilon_i} = D_i$。

由(13)我们有

(14)
$$
(\rho! \; \Delta^\rho) \cdot (\sigma! \; \Delta^\sigma) = (\rho + \sigma)! \; \Delta^{\rho + \sigma}
$$

在内同态代数/A-模$\mathbf{A}[\mathbf{X}]$。现在，$\nu$ 的长度上的归纳紧随$\nu! \; A'' = D^\nu$。

如果 $\mathbf{A}$ 是 Q 代数，公式 (9), (10), (11) 可以写成

(15)
$$
u(\mathbf{X} + \mathbf{Y}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(\mathbf{X}) \mathbf{Y}^\nu
$$
(16)
$$
u(\mathbf{X}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(a)(\mathbf{X} - a)^\nu
$$
(17)
$$
u(\mathbf{X}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(0) \; X^\nu
$$

公式 (15)、(16)、(17) 这三个都称为“泰勒的公式”。

#### 命题 6 (*《欧拉恒等式》*) {#alg-iv-s1-prop-6 .statement tag=069Y}

— *令* $u \in \mathbf{A}[\mathbf{X}]$ *为次数 r 的齐次多项式；我们有*

$$
\sum_{i \in I} X_i \cdot D_i u = ru.
$$

令 D 为 $A[X]$ 的 A-线性映射自身，使得当 v 是次数 s 的齐次时，$D(v) = sv$。我们知道 (III, p. 554, 例 6) D 是 $A[X]$ 的推导。因此，第 6 条命题是第 4 条命题的推论（IV，p. 6）。

### 5. 多项式环中的零除子

#### 命题 7 {#alg-iv-s1-prop-7 .statement tag=069Z}

— *令 $f \in A[X]$ 为不定的非零多项式，$a$ 为其首项系数。如果$a$在A中是可取消的（特别是当且仅当是单调的）那么我们对于$A[X]$的任何非零元素'g，*

$$
fg \neq 0 \quad \text{and} \quad \deg(fg) = \deg f + \deg g
$$

令 $g \in A[X]$ 为非零多项式，$\beta$ 为其首项系数，$n = \deg f$ 和 $p = \deg g$。那么$fg$中$X^{n+p}$的系数是不消失的$\alpha \beta$，从而命题。

#### 命题 8 {#alg-iv-s1-prop-8 .statement tag=06A0}

— *如果 A 是整环，那么$A[(X_i)_{i \in I}]$ 也是。*

令$u, v$为$A[(X_i)_{i \in I}]$的两个非零元素；我们必须证明$uv \neq 0$。现在$u$和$v$属于到环$A[(X_j)_{j \in J}]$，其中J是I的有限子集。因此，我们可以将极限变成I有限且等于$\{1, 2, ..., p\}$的情况。另一方面，环$A[X_1, ..., X_p]$同构于$X_p$中的多项式环，系数在$A[X_1, ..., X_{p-1}]$中。到$p$的归纳，我们就将$A[X]$减少到证明命题，现在应用第7条命题就足够了。

#### 推论 1 {#alg-iv-s1-prop-8-cor-1 .statement tag=06A1}

— *如果 A 为整环，且 $u, v$ 为 $A[(X_i)_{i \in I}]$ 的元素，则 $\deg(uv) = \deg u + \deg v$。*

我们可以将极限自己设置为 $u$ 和 $v$ 非零的情况。让$m = \deg u, n = \deg v$；我们有

$$
u = u_0 + u_1 + \cdots + u_m, \quad v = v_0 + v_1 + \cdots + v_n
$$

其中 $u_h$（分别为 $v_h$）是 $u$（分别为 v）的次数 $h$ 的齐次分量。从$u_m \neq 0$和$v_n \neq 0$开始，我们有$u_m v_n \neq 0$（命题8）。现在 $uv = u_m v_n + w$ 和 $\deg w < m + n$，从而结果。

#### 推论 2 {#alg-iv-s1-prop-8-cor-2 .statement tag=06A2}

— *如果 A 为整环，则 $A[(X_i)_{i \in I}]$ 的可逆元为 A 的可逆元。*

这立即来自Cor。 1.

#### 命题 9 {#alg-iv-s1-prop-9 .statement tag=06A3}

— *令$u \in A[(X_i)_{i \in I}]$；那么，要使 u 在环 $A[(X_i)_{i \in I}]$ 中幂零，其所有系数在环 A 中幂零是必要且充分的。*

正如在第 8 条的证明中，我们可以对一个变量 X 中多项式的情况进行约简。如果 $u$ 的所有系数都是幂零的，那么 $u$ 也是幂零的（I，p. 99，Cor.1）。假设$u$是幂零的，但零不是幂等的，并令$n$为其次数；我们将在$n$上争论归纳。令 $a$ 为 $u$ 的首项系数。存在整数$m > 0$使得$u^m = 0$。 $u^m$ 的首项系数为 $a^m$，因此为 $a^m = 0$。现在$u - \alpha X^n$是幂零的（I，loc.cit.）并且归纳假设显示$u - \alpha X^n$的所有系数都是幂零的。因此 $u$ 的所有系数都是幂零的。

#### 注 {#alg-iv-s1-n5-rem-1 .statement tag=06A4}

令$u$和$v$为$A[(X_i)_i \in ,]$的元素，并假设$A$为整环，$v$为$u$的非零倍数且$v$是齐次的；那么 $u$ 也是齐次的。让$u' \in A[(X_i)_i ,_1]$使得$v = uu'$；我们有 $u \neq 0$，$u' \neq 0$，如果
$$
u = u_h + u_{h+1} + \cdots + u_k \\
u' = u_{h'} + u_{h'+1} + \cdots + u_{k'}
$$
将$u$和$u'$的分解分解为齐次分量，其中$u_h \neq 0$、$u_k \neq 0$、$u_{h'} \neq 0$、$u_{k'} \neq 0$，则$v = u_h u_{h'} + u_h u_{h'+1} + \ldots + u_k u_{k'}$和$u_h u_{h'}$是次数的非零齐次$h + h'$ 而 $u_k u_{k'}$ 是次数 $k + k'$ 的非零齐次（命题 8）。由于$v$是齐次的，所以我们有$h + h' = k + k'$从而$h = k$，$h' = k'$。

### 6. 欧几里得除法一个不定多项式

#### 命题 10 {#alg-iv-s1-prop-10 .statement tag=06A5}

*令$f$和$g$分别为非零元素、次数、$m$和$n$的$A[X]$。设$\alpha_0$为$f$和$\mu = \sup(n - m + 1, 0)$的首项系数。存在 $u, v \in A[X]$ 这样*
$$
\alpha_0^\mu g = uf + v, \quad \deg v < m.
$$
*如果$\alpha_0$在$A$中可取消，则$u$和$v$由这些属性唯一确定。*

当$n < m$时，$u$和$v$的存在性是明确的，因为这样我们就可以取$u = 0$和$v = g$。对于$n \geq m$，我们将在$n$ 使用归纳法。设$\beta$为$g$的首项系数；如果$f = \sum_{k=0}^m \alpha_k X^{m-k}$，我们可以写成$\alpha_0^\mu g = \alpha_0^\mu \beta X^n \cdot f + \alpha_0^{\mu-1} g_1$，其中$g_1 \in A[X]$和$\deg g_1 < n$。到归纳假设，存在$u_1, v \in A[X]$，使得$\alpha_0^{\mu-1} g_1 = u_1 f + v$和$\deg v < m$。因此
$$
\alpha_0^\mu g = (\alpha_0^{\mu-1} \beta X^{n-m} + u_1) f + v
$$
输入$u = \alpha_0^{\mu-1} \beta X^{n-m} + u_1$就足够了。

假设$\alpha_0$在$A$中可以取消，现在让我们证明$u$和$v$的唯一性。令 $u, v, u_1, v_1 \in A[X]$ 为
$$
\alpha_0^\mu g = uf + v = u_1 f + v_1, \quad \deg v < m, \quad \deg v_1 < m
$$

我们有$(u - u_1) f = v_1 - v$和$\deg(v_1 - v) < m$，因此有$u - u_1 = 0$（IV，p. 9，提案7），因此有$v_1 - v = 0$。

#### 推论（《多项式的欧几里得除法》）{#alg-iv-s1-n6-cor-1 .statement tag=06A6}

— 令 $f$ 为 $A[X]$ 的非零元素，其前导*系数*可逆且$m = \deg f$。
(i) 对于每个 $g \in A[X]$ 都存在 $u,\ v \in A[X]$ 这样*那个*
$$
g = uf + v , \quad \deg v < m .
$$
而且，这些条件确定$u$和$v$是独一无二的。
(ii) $A[X]$的子A模块$A + AX + \ldots + AX^{m-1}$和$fA[X]$是$A[X]$的补充。
(iii) 假设$f$非常数，并将$A[X]$视为$A[T]$-*模*，通过将$A[T]$的同态$u(T) \mapsto u(f(X))$转化为$A[X]$。那么 $A[X]$ 就是一个免费的 $A[T]$-*模* 和基 $(1, X, \ldots, X^{m-1})$。
断言 (i) 和 (ii) 是提案 10 的直接的推论。
让我们证明(iii)。设$\psi$为$A[T, X]$的同态$v \mapsto v(f(X), X)$到$A[X]$。首先将$A[T, X]$视为$T$中的多项式环，系数在$A[X]$中；科。 IV的1，p. 5表明$\psi$的核$a$是$A[T, X]$的理想$(T - f(X))$。现在将$A[T, X]$视为$X$中的多项式环，系数在$A[T]$中；那么$\psi$是$A[T][X]$到$A[X]$的$A[T]$线性映射。上面的断言 (ii)（应用于$X$中的多项式$f(X) - T$，系数在$A[T]$中）表明$(1, X, \ldots, X^{m-1})$是$A[T, X]$的补充$a$的$A[T]$子模的基。由于$\psi(X^i) = X^i$对于每一个整数$i \geq 0$，(iii)立即随之而来。

对于(i)的记号，我们可以说$u$是商，$v$是$g$的欧几里得除法除以$f$的余数；为了使余数消失，$f$应该除$g$是必要且充分的。

### 7. 多项式在一个不定式 [^1] 中的整除性

#### 命题 11 {#alg-iv-s1-prop-11 .statement tag=06A7}

— 令 $K$ 为可交换的 *域*。
(i) 对于 $K[X]$ 的每个非零理想 $a$，在 $K[X]$ 中恰好存在一个*单调*首一多项式 $f$，使得 $a = (f )$。
(ii) 设$f_1$和$f_2$在$K[X]$中；对于 $(f_1) = (f_2)$ 来说，存在 $K$ 的非零元素 $\lambda$ 使得 $f_2 = \lambda f_1$ 成立是必要且充分的。
让我们证明(ii)，所述条件的充分性是明确的。 $f_1$ 和 $f_2$ 生成零理想的情况是微不足道的。因此假设非零多项式$f_1$和$f_2$生成与$K[X]$相同。则存在多项式$u_1$和$u_2$使得$f_1 = u_1 f_2$和$f_2 = u_2 f_1$；由此可见，u_1 u_2 = 1，从而 $\deg u_1 + \deg u_2 = 0$，所以$\deg u_2 = 0$。因此我们证明了$u_2$是$K$的非零元素。

为了证明 (i)，令 $f$ 为 $a$ 中最小可能的次数的一元多项式。给定$a$中的$g$，令$u$和$v$为$g$的欧几里得除法除以$f$的商和余数；然后$v = g - u f$属于到$a$，我们有$\deg v < \deg f$；如果$v$非零，则$K$将存在非零元素$A$，使得$\lambda v$是单调的，并且由于$\lambda v \in a$，这将与定义相矛盾。因此我们有 $a = (f)$； 唯一性的一元多项式 $f$ 使得 $a = (f)$ 现在由 (ii) 得出。

#### 命题 12 {#alg-iv-s1-prop-12 .statement tag=06A8}

*令$K$为交换域且$f, g$为$K[X]$的两个元素。对于 $K[X]$ 中的每个多项式 $d$，以下属性是等效的*：

(i) *多项式$d$除$f$和$g$以及除同时$f$和$g$除$d$*。

(ii) *多项式$d$除$f$和$g$并且存在两个多项式$u$和$v$使得$d = u f + v g$*。

(iii) *关系$(d) = (f) + (g)$在$K[X]$*的理想之间成立。

*多项式 $d$ 由这些属性的 $K$ 的非零元素确定至乘法。如果$f$和$g$不都是零，则$d$的$d \neq 0$和次数主要除以$f$和$g$*的每个多项式的次数。

当$f$和$g$为零时，仅对于$d = 0$满足(i)至(iii)的每个性质，因此它们是等价的。此后，我们假设$f, g$不都是0，并且我们用$a$表示$K[X]$的理想$(f) + (g)$。

我们注对于$K[X]$中的任何多项式$u$和$v$，属性$(u) \supset (v)$和«$u$除$v$»是等价的。因此，断言 (ii) 等价于 « $(d) \supset (f)$ 和 $(d) \supset (g)$ 和 $d \in (f) + (g)$ »，即 (iii)。显然，(ii) 暗示着(i)。最后假设 (i) 成立；我们有$(d) \supset (f)$和$(d) \supset (g)$，从而$(d) \supset a$；另一方面，根据命题11（IV，p. 12），存在一个多项式$d_1$使得$a = (d_1)$；由于$d_1$除既$f$和$g$，除$d$乘假设，从而$(d) \subset a$，最后我们有$(d) = a$，即(iii)。

第 12 条命题的其他断言是应用于理想$a = (f) + (g)$ 的第 11 条命题的直接的推论。

#### 定义 1 {#alg-iv-s1-def-1 .statement tag=06A9}

*根据第 12 条提案的记号，我们说 $d$ 是 $f$ 和 $g$ 的最大的公共的除子（简称 gcd）。我们说$f$和$g$互质，或者如果$1$是$f$和$g$*的gcd，则$f$与$g$互质。

说$f$和$g$互质，意味着在$K[X]$中存在多项式$u$和$v$，使得$u f + v g = 1$。

#### 推论 1 {#alg-iv-s1-def-1-cor-1 .statement tag=06AA}

*设$d$为$f$和$g$的gcd，并且$K'$交换域包含$K$为子域。那么$d$是$f$的gcd，$g$被视为$K'[X]$*的元素。

这是根据第 12 号提案 (iii) 得出的。

#### 推论 2 {#alg-iv-s1-def-1-cor-2 .statement tag=06AB}

— 设 d 为 gcd，g。
    (i) 如果$u \in K[X]$，du 是 fu 和 gu 的 gcd。
    (ii) 如果$v \in K[X]$是f和g的除子($\neq 0$)，则$d/v$是$f/v$和$g/v$的gcd。
    这是根据第 12 号提案 (ii) 得出的。

#### 推论 3 {#alg-iv-s1-def-1-cor-3 .statement tag=06AC}

— 令 w 为 f 和 g 的公共的因子。对于 w 是 gcd off 和 g，$f/w$ 和 $g/w$ 互质是充分必要的。
    这是从 Cor 得出的。 2.

#### 推论 4 {#alg-iv-s1-def-1-cor-4 .statement tag=06AD}

— 让$f, g, h \in K[X]$。如果 f 除 gh 且与 g 互质，则 f 除 h。
    对于 f 除 gh 和 fh，因此 f 除 gh 和 fh 的每个 gcd，特别是 h（Cor. 2, (i)）。

#### 推论 5 {#alg-iv-s1-def-1-cor-5 .statement tag=06AE}

— 让$f, g \in K[X]$。为了使 g 互质，$K[X]/(f)$ 中 g 的典范像可逆是必要且充分的。
    对于这个条件意味着存在$u, v \in K[X]$使得$uf + vg = 1$。

#### 推论 6 {#alg-iv-s1-def-1-cor-6 .statement tag=06AF}

— 让$f, g_1, g_2, ..., g_n \in K[X]$。如果 f 与 $g_1, g_2, ..., g_n$ 互质，则 f 与 $g_1g_2...g_n$ 互质。

\* 推论 7. — 要使 f 和 g 互质，它们在 K 的任何扩张中都没有公共的根是必要且充分的。
    因为如果 d 是 f、g 的 gcd，则 K 的扩张 K' 中 f 的根公共的和 g 是 K' 中 d 的根。现在推论来自 V，p. 21，命题 4。

### 8. 不可约多项式

#### 定义 2 {#alg-iv-s1-def-2 .statement tag=06AG}

— 令 K 为交换域。如果 $\deg f \geq 1$ 且 f 不能被任何多项式 g 整除，使得 $0 < \deg g < \deg f$ ，我们说 $f \in K[X]$ 是不可约的。
    同样，$\deg f \geq 1$ 和 $K[X]$ 中 f 的唯一除子是 f 的标量 $\neq 0$ 和乘积与标量 $\neq 0$。由于关系 $(f) \subset (g)$ 意味着 g 除 f，我们看到 $K[X]$ 的不可约多项式也可以定义为多项式 f，使得理想 $(f)$ 极大（I，p. 104）。

    让$f, g \in K[X]$。如果 ff 是不可约的，则显然 f 和 g 互质或者 f 除 g。如果 f 和 g 是不可约的，则 f 和 g 互质，或者每个都是另一个的乘积标量 $\neq 0$。特别是，两个不同的不可约单调多项式互质。

#### 命题 13 {#alg-iv-s1-prop-13 .statement tag=06AH}

— 令 $\mathscr{I}$ 为 $K[X]$ 中不可约单调多项式的集合。令 f 为 $K[X]$ 的非零元素及其首项系数；那么恰好存在正整数 $(v_p)_{p \in \mathscr{S}}$ 和有限支撑的族，这样我们就有分解

$$
f = \alpha \prod_{p \in \mathscr{S}} p^{v_p}.
$$

当$f$是单数时，即$\alpha = 1$时，只需证明命题即可。我们将以归纳对次数$n$进行争论，$n = 0$的情况微不足道。假设$n \geq 1$和命题对于次数$< n$的所有多项式都成立。

设$E$为一元多项式$\neq 1$的集合，其中除$f$；我们有$f \in E$，因此$E$不为空，并且$E$中存在一个至少为次数的多项式$g$。显然$g$是不可约的，并且存在次数$< n$的一元多项式$h$使得$f = gh$；通过归纳假设 $h$ 是不可约一族多项式的乘积，因此 $f$ 具有相同的性质。这就证明了分解(18)的存在。

现在让我们证明分解 (18) 的唯一性。令$(w_p)_{p \in \mathscr{S}}$是正整数与有限支撑的族，使得$f = \prod_{p \in \mathscr{S}} p^{w_p}$。由于$f$是次数$n \geq 1$，因此存在$p \in \mathscr{S}$使得$w_p > 0$；如果我们有$v_p = 0$，$f$将是$\mathscr{S}$的元素族中的乘积，与$p$不同，因此它将是$p$（IV，p. 13，Cor.6）的素数，与$p$的事实相反除$f$。到归纳假设，首一多项式$f/p$承认型的唯一分解 (18)；因此，每 $q \in \mathbf{4}$ 就有结论等式 $w_q = v_q$。

令 $f$ 为 $\mathbf{K}[X]$ 中的非零多项式。如果分解(18)中的指数$v_p$都是$\leq 1$，我们可以说$f$没有倍数因子；说$f$是成对不同不可约多项式的有限序列的乘积，或者说$f$不能被$\mathbf{K}[X]$的任何非常数多项式的平方整除，这也是同样的道理。

### 习题 {#alg-iv-s1-exercises}

§ 1](exercises/s1/)参见[习题。

[^1]: 读者将会注这个数与下一个数的结果与整数 (I, p. 112) 的环 $Z$ 的整除性质之间的类比。它们本质上取决于这样一个事实：在环$Z$和$K[X]$中，每个理想都是主要的，正如我们将在章VII, § 1中看到的那样。
