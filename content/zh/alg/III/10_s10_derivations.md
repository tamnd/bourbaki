---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 10
section_title: Derivations
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 550-574, 645-646
pdf_pages: 0574-0598, 0669-0670
extraction: ocr
subsections:
    - "no": 1
      title: COMMUTATION FACTORS
      page: 550
      pdf_page: 574
    - "no": 2
      title: GENERAL DEFINITION OF DERIVATIONS
      page: 551
      pdf_page: 575
    - "no": 3
      title: EXAMPLES OF DERIVATIONS
      page: 553
      pdf_page: 577
    - "no": 4
      title: COMPOSITION OF DERIVATIONS
      page: 554
      pdf_page: 578
    - "no": 5
      title: DERIVATIONS OF AN ALGEBRA A INTO AN A-MODULE
      page: 557
      pdf_page: 581
    - "no": 6
      title: DERIVATIONS OF AN ALGEBRA
      page: 559
      pdf_page: 583
    - "no": 7
      title: Functorial Properties
      page: 560
      pdf_page: 584
    - "no": 8
      title: RELATIONS BETWEEN DERIVATIONS AND ALGEBRA HOMOMORPHISMS
      page: 561
      pdf_page: 585
    - "no": 9
      title: EXTENSION OF DERIVATIONS
      page: 562
      pdf_page: 586
    - "no": 10
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; NON-COMMUTATIVE CASE
      page: 567
      pdf_page: 591
    - "no": 11
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; COMMUTATIVE CASE
      page: 568
      pdf_page: 592
    - "no": 12
      title: FUNCTIORIAL PROPERTIES OF K-DIFFERENTIALS
      page: 570
      pdf_page: 594
statements: 41
exercises: 5
content_sha256: 45c7c7255aaf46779d7e2fb7461299079d77d6ee2185bf54a8a0d7277a0f5ff6
translated_from: content/en/alg/III/10_s10_derivations.md
translation_method: google
source_content_sha256: aaeacce850abcb26b3dc2f0a2b6232e064f49c1f74a413c96833e391ff1f75f3
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: a33304f0f6180dfc7d85eb137994eed1d5f7129e9692f68cd8db9c3e64194dd2
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 10。 推导

在本段中，以及另外提到的除非，代数不被认为是结合的，也不一定具有单位元； K 表示交换环。

### 1.交换因子

当在本段中我们谈论毕业但没有指定它们时，我们总是指型$\Delta$的毕业，其中$\Delta$是可加写的交换律群。在本段中，$\Delta$上的交换因子和$\mathbf{Z}$中的值称为交换因子超过$\Delta$（§ 4, no. 7，定义6）。因此，$\Delta$上的交换因子被识别为$\Delta \times \Delta$的映射$\varepsilon : (\alpha, \beta) \mapsto \varepsilon_{\alpha \beta} = \varepsilon(\alpha, \beta)$到乘法群$\{-1, 1\}$，这样对于$\Delta$中的$\alpha, \alpha', \beta, \beta'$，

$$
\begin{cases}
\varepsilon(\alpha + \alpha', \beta) = \varepsilon(\alpha, \beta)\varepsilon(\alpha', \beta) \\
\varepsilon(\alpha, \beta + \beta') = \varepsilon(\alpha, \beta)\varepsilon(\alpha, \beta') \\
\varepsilon(\beta, \alpha) = \varepsilon(\alpha, \beta).
\end{cases}
$$

(1)

由此可见$\varepsilon(2\alpha, \beta) = \varepsilon(\alpha, 2\beta) = 1$。

当$\Delta = \mathbf{Z}$时，每交换因子$\varepsilon$由给$\varepsilon(1, 1)$确定；因此只有*两个*这样的因子，第一个由

(2)
$$
\varepsilon(p, q) = 1 \quad \text{for } p, q \text{ in } \mathbf{Z}
$$
第二个由
(3)
$$
\varepsilon(p, q) = (-1)^{pq} \quad \text{for } p, q \text{ in } \mathbf{Z}.
$$

### 2. 定义推导将军

考虑交换环$K$，型$\Delta : A, A', A'', B, B', B''$的六个分级$K$模块，以及三个$K$线性映射
$$
\mu : A \times A' \to A'', \qquad \lambda_1 : B \times A' \to B'', \qquad \lambda_2 : A \times B' \to B''
$$
这样相应的 $K$-线性映射
$$
A \otimes_K A' \to A'', \qquad B \otimes_K A' \to B'', \qquad A \otimes_K B' \to B''
$$
*分级为次数* 0。$a \in A, a' \in A'$的像$\mu(a, a')$简单地表示为$a.a'$甚至$aa'$，对于其他两个双线性映射也类似。因此，$a.a'$的*次数*是$a$和$a'$的次数的*和*。

#### 定义 1 {#alg-iii-s10-def-1 .statement tag=0667}

*鉴于上述和$\Delta \times \Delta$上的交换因子$\varepsilon$，$(A, A', A'')$的次数$\delta \in \Delta$到$(B, B', B'')$的$\varepsilon$衍生（或$(K, \varepsilon)$衍生）是一个三元组次数 $\delta$ 的分级$K$线性映射：*
$$
d : A \to B, \qquad d' : A' \to B', \qquad d'' : A'' \to B''
$$
*这样，对于每个同质元素$a \in A$和每个元素$a' \in A'$*
(4)
$$
d''(a.a') = (da).a' + \varepsilon_{\delta, \deg(a)}a.(d'a').
$$

当$a$和$a'$分别穿过$A$和$A'$的生成的和系统时，显然用线性足以验证关系(4)。

用同一个字母 $d$ 表示三个映射 $d, d', d''$ 通常很方便（可以通过用 $d$ 同等地表示次数 $\delta$ 的分级 $K$ 线性映射来证明其合理性）

$$
(a, a', a'') \mapsto (da, d'a', d''a'')
$$

$A \oplus A' \oplus A''$ 变为$B \oplus B' \oplus B''$）。 关系 (4) 可以写得更简单
$$
d(a.a') = (da).a' + \varepsilon_{\delta,\deg(a)} a.(da').
$$
*给定* 次数形式 $(A, A', A'')$ 到 $(B, B', B'')$ 的 $\varepsilon$ 推导，分级线性映射的K-模的子 K 模块
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
当$\varepsilon(\alpha, \beta) = 1$对于$\Delta$中的所有$\alpha, \beta$时，我们简单地说*推导*（或*K-导数*）而不是$\varepsilon$-导数。 推导形式的子 K 模块
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
当$\Delta = \mathbf{Z}$和$\varepsilon(p.q) = (-1)^{pq}$时，*偶数*次数的每个$\varepsilon$-导数都是推导； *奇数* 次数的每个$\varepsilon$-导数通常称为*反导数*（或*K-反导数*）；因此反导数 $d$ 满足
$$
d(a.a') = (da).a' + (-1)^{\deg(a)} a.(da')
$$
对于*同质* 元素 $a \in A$。

#### 注 {#alg-iii-s10-n2-rem-1 .statement tag=0668}

(1) *推导* 的概念可以通过同意给予这些模简单的毕业来定义为非分级模。

(2) 如果只考虑给定次数$\delta$的$\varepsilon$-导数，交换因子$\varepsilon$可以如下处理：双线性映射$\lambda_2 : A \times B' \to B''$由替换通过双线性映射$\lambda'_2 : A \times B' \to B''$修改，这样对于$A$和所有$b' \in B'$中的每个*同质*$a$，
$$
\lambda'_2(a, b') = \varepsilon_{\delta, \deg(a)} \lambda_2(a, b').
$$
那么相对于双线性映射$\mu, \lambda_1, \lambda'_2$，$d$ 是推导。

上面给出的 $\varepsilon$ 的一般定义推导特别适用于两种情况：

*情况 (I)*：$A = B, A' = B', A'' = B''$ 和三个双线性映射$\mu, \lambda_1, \lambda_2$ 等于*相同* 映射。

*情况 (II)*：$A = A' = A'', B = B' = B''$，因此（对于$\mu$）$A$ 是一个*分级的代数* 和两个 K 双线性映射。
$$
\lambda_1 : B \times A \to B, \quad \lambda_2 : A \times B \to B
$$
相应的 K-线性映射 $B \otimes_K A \to B, A \otimes_K B \to B$ 的分级为次数 0。 $A$ 的次数 $\delta$ 到 $B$ 的 $\varepsilon$ 推导则为分级 K-线性映射次数 $\delta$的$d : A \to B$，这样对于$A$中的每个齐次$x$和每个$y \in A$，我们有关系
$$
d(xy) = (dx)y + \varepsilon_{\delta, \deg(a)} x(dy).
$$

特别考虑在 (II) 情况下，A 是单位结合律 K-代数并且 $\lambda_1$ 和 $\lambda_2$ 是 (A, A) 双模 (§ 4, no. 3, 定义 3) 的外法则。当 A 和 B 是两个单位关联 K-代数时，这一点尤其成立，给出分级 K-代数 $\rho : A \to B$ 的单位同态，并且在由两个外法则定义的 B 上考虑 (A, A)-双模结构

$$
\lambda_1 : (b, a) \mapsto b \rho(a), \qquad \lambda_2 : (a, b) \mapsto \rho(a)b
$$

$a \in A, b \in B$。

情况 (I) 和 (II) 在公共的中具有以下情况：考虑分级 K-代数 A，取 $B = A$、映射 (7) 均为 A 上的乘法。然后我们讨论$\varepsilon$ 推导（或 (K,分级代数 A 的$\varepsilon$）-推导）：对于 A 中的每个齐次 $x$ 和所有$y \in A$，它是 A 自身的分级 K-线性映射，次数 $\delta$、满足 (8)。特别是，如果 A 是分级环，被视为（结合）$\mathbf{Z}$-代数，我们说的是环 A 的 $\varepsilon$ 推导。

设 A 为单位交换结合律 K-代数且 B A-模；当我们谈到 A 的推导进入 B 时，我们总是会理解我们的意思是 B 上的 A 双模结构源自其 A-模结构；然后公式

$$
d(xy) = x(dy) + y(dx) \quad \text{for} \quad x \in A, y \in A
$$

对于这样的推导 $d : A \to B$ 成立。

### 3.例推导

#### 例 1 {#alg-iii-s10-n3-exa-1 .statement tag=0669}

设A是$\mathbf{R}$的映射可微分到$\mathbf{R}$的$\mathbf{R}$代数，并令$x_0$是$\mathbf{R}$的点； $\mathbf{R}$可以被认为是A-模与外法则$(f, a) \mapsto f(x_0)a$。那么映射 $f \mapsto Df(x_0)$ 就是推导，因为（实数变量的函数，I, § 1, no. 3）

$$
(D(fg))(x_0) = (Df(x_0))g(x_0) + f(x_0)(Dg(x_0)).*
$$

#### 例 2 {#alg-iii-s10-n3-exa-2 .statement tag=066A}

令X为类$C^\infty$的可微流形，并令A为X上微分形式的分级$\mathbf{R}$代数。 映射与X上的每个微分形式$\omega$相关联，其外部微分$d\omega$是次数+1的反推导（可微分和解析流形，R，§ 8）。*

#### 例 3 {#alg-iii-s10-n3-exa-3 .statement tag=066B}

设 A 是结合律 K-代数。对于所有 $a \in A$，映射 $x \mapsto ax - xa$ 是代数 A (cf. no. 6) 中的推导。

#### 例 4 {#alg-iii-s10-n3-exa-4 .statement tag=066C}

令 M 为 K-模，A 为外部代数 $\bigwedge(M^*)$ 及其通常的刻度 (§ 7, no. 1)。 *在§ 11, no. 9中可以看出，对于所有$x \in M$，右内部乘积$i(x)$是次数$-1$的A的反导数。*

#### 例 5 {#alg-iii-s10-n3-exa-5 .statement tag=066D}

回到no. 2的定义1的一般情况，令$\overline{K}$为另一个交换环和$\rho : K \to \overline{K}$环同态；让$\overline{A}, \overline{A}', \overline{A}'', \overline{B}, \overline{B}', \overline{B}''$表示通过将标量的环扩展到$\overline{K}$（II, § 11, no. 5）分别从$A, A', A'', B, B', B''$获得的分级$\overline{K}$模块；我们从 $\mu, \lambda_1$ 和 $\lambda_2$ $\overline{K}$ 双线性映射导出
$$
\bar{\mu} : \overline{A} \times \overline{A}' \to \overline{A}'', \quad \bar{\lambda}_1 : \overline{B} \times \overline{A}' \to \overline{B}'', \quad \bar{\lambda}_2 : \overline{A} \times \overline{B}' \to \overline{B}''
$$
通过考虑张量积乘$l_{\overline{K}}$的相应的$K$-线性映射到$\mu, \lambda_1$和$\lambda_2$（II, § 5, no. 1）。那么，如果 $d$ 是 $(A, A', A'')$ 的次数 $\delta$ 到 $(B, B', B'')$ 的 $\varepsilon$ 推导，则 $\overline{A} \oplus \overline{A}' \oplus \overline{A}''$ 的映射 $\bar{d} = d \otimes l_{\overline{K}}$ 到 $\overline{B} \oplus \overline{B}' \oplus \overline{B}''$ 是$\varepsilon$-将$(\overline{A}, \overline{A}', \overline{A}'')$的次数$\delta$推导为$(\overline{B}, \overline{B}', \overline{B}'')$。

#### 例 6 {#alg-iii-s10-n3-exa-6 .statement tag=066E}

令$A$为型$\mathbf{Z}$的分级$K$代数； 次数 0、$d : A \to A$的分级线性$K$映射是通过取$x_n \in A_n (n \in \mathbf{Z})$、$d(x_n) = nx_n$来定义的。这个映射是$A$的推导，因为对于$x_p \in A_p, x_q \in A_q$，
$$
d(x_p x_q) = (p + q)x_p x_q = d(x_p)x_q + x_p d(x_q).
$$

### 4.合成推导

我们假设在这个没有。 no. 2的情况(I)成立，即$A, A', A''$是型$\Delta$的三个分级$K$模块，并且我们被给予$K$双线性映射$\mu : A \times A' \to A''$相应的到分级$K$-次数 0、$A \otimes_K A' \to A''$ 的线性映射。 $A \oplus A' \oplus A''$的分级自同态$f$使得$f(A) \subset A, f(A') \subset A'$和$f(A'') \subset A''$形式分级关联代数$\mathrm{Endgr}_K(A \oplus A' \oplus A'')$的分级子代数（§ 3, no. 1， 例2)。特别是，可以组合 $(A, A', A'')$ 的两个 $\varepsilon$ 导数，但不应认为两个 $\varepsilon$ 导数中的合成是 $\varepsilon$ 导数。

在型 $\Delta$ 的每个分级代数 $B$ 上，定义了两个同质元素 $u, v$ 的 $\varepsilon$ 括号（或在 $\varepsilon = 1$ 时简单地括号），由公式 (10)
$$
[u, v]_\varepsilon = uv - \varepsilon_{\deg u, \deg v} vu \text{ (denoted simply by } [u, v] \text{ if } \varepsilon = 1).
$$
通过线性扩展该映射，获得$B \times B$到$B$的$K$双线性映射$(u, v) \mapsto [u, v]_\varepsilon$。然后，对于 $B$ 中的齐次 $u$ 和 $v$
$$
[v, u]_\varepsilon = -\varepsilon_{\deg u, \deg v}[u, v]_\varepsilon.
$$
应用这个定义到分级的代数$\mathrm{Endgr}_K(A \oplus A' \oplus A'')$，两个分级的自同态的$\varepsilon$括号就这样定义了。

#### 命题 1 {#alg-iii-s10-prop-1 .statement tag=066F}

*令$d_1, d_2$为次数$\delta_1, \delta_2$的$(A, A', A'')$的两个$\varepsilon$派生。然后是$\varepsilon$-括号*
$$
[d_1, d_2]_\varepsilon = d_1 \circ d_2 - \varepsilon_{\delta_1, \delta_2} d_2 \circ d_1
$$
*是次数 $\delta_1 + \delta_2$ 的 $\varepsilon$ 派生。此外，如果$d$是次数$\delta$的$(A, A', A'')$的$\varepsilon$衍生，并且如果$\varepsilon_{\delta, \delta} = -1$，则$d^2 = d \circ d$是推导。*

假设$x \in A$齐次于次数$\xi$；对于所有$y \in A'$，
$$
d_1(d_2(xy)) = ((d_1 d_2)(x))y + \varepsilon_{\delta_1, \delta_2 + \xi}(d_2 x)(d_1 y)
+ \varepsilon_{\delta_2, \xi}(d_1 x)(d_2 y) + \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
$$
考虑no. 1的公式(1)。交换$d_1$和$d_2$的角色，我们再次使用（1）（no. 1）得到之后简化，
$$
(d_1 d_2)(xy) - \varepsilon_{\delta_1, \delta_2}(d_2 d_1)(xy) = ((d_1 d_2)(x))y - \varepsilon_{\delta_1, \delta_2}((d_2 d_1)(x))y
+ \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
- \varepsilon_{\delta_1, \delta_2} \varepsilon_{\delta_1 + \delta_2, \xi} x((d_2 d_1)(y))
$$
即写$d = [d_1, d_2]_\varepsilon$和$\delta = \delta_1 + \delta_2$，
$$
d(xy) = (dx)y + \varepsilon_{\delta, \xi} x(dy)
$$
这证明了$d$是$\varepsilon$的导数。

另一方面，如果在 (11) 中，我们令 $d_1 = d_2 = d$、$\delta_1 = \delta_2 = \delta$ 和 $\varepsilon_{\delta, \delta} = -1$，则通过 (1) 得到 $\varepsilon_{\delta, \delta + \xi} = -\varepsilon_{\delta, \xi}$，
$$
d^2(xy) = (d^2 x)y + \varepsilon_{2\delta, \xi} x(d^2 y)
$$
而作为$\varepsilon_{2\delta, \xi} = 1$，可以看出$d^2$是推导。

#### 推论 {#alg-iii-s10-n4-cor-1 .statement tag=066G}

*假设$\Delta = \mathbf{Z}$。然后：*
(i) *反推导的平方是推导。*
(ii) *两个推导的括号是推导。*
(iii) *反推导的括号和偶数次数的推导是反推导。*
(iv) *如果$d_1$和$d_2$是反导数，则$d_1 d_2 + d_2 d_1$是推导。*

在这个数开头的假设下，现在考虑$(A, A', A'')$的*成对可置换推导*的有限序列$D = (d_i)_{1 \leq i \leq n}$。对于代数 $K[X_1, \ldots, X_n]$ 中的每个多项式 $P(X_1, \ldots, X_n)$，然后定义 $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ 的元素 $P(d_1, \ldots, d_n)$ (§ 2, no. 9)； 记号缩写为$P(D)$。

#### 命题 2 {#alg-iii-s10-prop-2 .statement tag=066H}

*根据上述假设和记号，考虑 2n 个不定式 $T_1, \ldots, T_n, T'_1, \ldots, T'_n$，对于每个多项式 $F \in K[X_1, \ldots, X_n]$ 写出 $F(T) = F(T_1, \ldots, T_n), F(T') = F(T'_1, \ldots, T'_n)$ 和*
$$
F(T + T') = F(T_1 + T'_1, \ldots, T_n + T'_n).
$$
*假设*
$$
P(T + T') = \sum_i Q_i(T) R_i(T')
$$
*其中 $Q_i$ 和 $R_i$ 属于至 $K[X_1, \ldots, X_n]$。然后，对于所有 $x \in A$ 和 $y \in A'$，*
$$
P(D)(xy) = \sum_i (Q_i(D)x)(R_i(D)y).
$$

我们引入$n$其他不定式$T_1'', \ldots, T_n''$并考虑多项式代数$K[T_1, \ldots, T_n, T_1', \ldots, T_n', T_1'', \ldots, T_n''] = B$；另一方面，我们将$A \times A'$的双线性映射的$K$模$M$考虑为$A''$；对于每个$K$双线性映射$f \in M$和$1 \leq i \leq n$，通过编写在$M$上定义$B$-模块结构，

$$
\begin{cases}
(T_i f)(a, a') = f(d_i a, a') \\
(T_i' f)(a, a') = f(a, d_i a') \\
(T_i'' f)(a, a') = d_i(f(a, a'))
\end{cases}
$$

由于 $d_i$ 可以用一个另一个置换，因此可以看出，对于每个多项式 $F \in K[X_1, \ldots, X_n]$、$(F(T)f)(a, a') = f(F(D)a, a')$，

$$
(F(T')f)(a, a') = f(a, F(D)a')
$$

和$(F(T'')f) = F(D)(f(a, a'))$。因此，要证明(12)，只需证明

$$
(P(T'') - \sum_i Q_i(T)R_i(T')).\mu = 0
$$

或$B$模块$M$中的$(P(T'') - P(T + T')).\mu = 0$。现在，$d_i$是推导的假设也可以用说来表示，对于$1 \leq i \leq n$，

$$
(T_i'' - T_i - T_i').\mu = 0
$$

在$B$模块$M$中。通过连续考虑多项式

$P(T_1'', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2'', \ldots, T_n'')$
$P(T_1 + T_1', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2 + T_2', \ldots, T_n'')$
$\ldots$
$P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n'') - P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n + T_n')$

可见差$P(T'') - P(T + T')$可以写成形式

$$
\sum_{i=1}^n (T_i'' - T_i - T_i') G_i(T, T', T'')
$$

其中$G_i$是$B$的元素。因此，关系 (14) 是关系 (15) 的直接的推论。

#### 推论（莱布尼兹公式）{#alg-iii-s10-n4-cor-2 .statement tag=066I}

*设 $d_i$ ($1 \leq i \leq n$) 为 $(A, A', A'')$ 的 $n$ 推导，可用 1 另一个置换。对于所有 $\alpha = (\alpha_1, \ldots, \alpha_n) \in \mathbf{N}^n$，我们写*

$$
d^\alpha = d_1^{\alpha_1} d_2^{\alpha_2} \ldots d_n^{\alpha_n}.
$$

然后，对于$x \in \mathbf{A}$和$y \in \mathbf{A}'$，

$$
d^\alpha(xy) = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) d^\beta(x)d^\gamma(y)
$$

我们所写的地方（在记号在章开头引入）

$$
((\beta, \gamma)) = (\beta + \gamma)!/(\beta! \gamma!).
$$

这立即由多项式公式 (I, § 8, no. 2) 得出

$$
(T + T')^\alpha = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) T^\beta {T'}^\gamma
$$

和命题2。

### 5. 推导将代数 A 转换为 A-模

我们假设在这个没有。 no. 2 的情况 (II) 成立。然后有一个分级的 K-代数 A 和一个分级的 K-模 E，还有两个 K-线性映射次数 0

$$
E \otimes_K A \to E, \quad A \otimes_K E \to E
$$

表示为

$$
x \otimes a \mapsto x.a \quad \text{and} \quad a \otimes x \mapsto a.x \quad \text{for } a \in A \text{ and } x \in E.
$$

#### 命题 3 {#alg-iii-s10-prop-3 .statement tag=066J}

令 $d : A \to E$ 为次数 $\delta$ 的 $\varepsilon$ 导数。那么$\mathrm{Ker}(d)$就是A级的子代数；如果A承认单位元，则它属于到$\mathrm{Ker}(d)$。

显然$\mathrm{Ker}(d)$是A的分级子K模块；此外，no. 2的关系(8)表明，如果$x$和$y$是两个齐次的元素属于到$\mathrm{Ker}(d)$，则$d(xy) = 0$，因此$xy \in \mathrm{Ker}(d)$。最后，如果 A 承认单位元 1（次数 0、cf. § 3, no. 1），no. 2 的关系 (8)，其中 $x$ 和 $y$ 被 1 替代，则给出 $d(1) = d(1) + d(1)$，因此$d(1) = 0$。

#### 推论{#alg-iii-s10-n5-cor-1 .statement tag=066K}

令$d_1$和$d_2$是同一次数$\delta$从A到E的两个$\varepsilon$派生。如果$d_1$和$d_2$在代数A的生成的系统的每个元素取相同的值，则$d_1 = d_2$。

$d_1 - d_2$是次数$\delta$的$\varepsilon$派生，因此$\mathrm{Ker}(d_1 - d_2)$是A的子代数，其中A的包含生成的系统因此等于A。

#### 命题 4 {#alg-iii-s10-prop-4 .statement tag=066L}

令 $d : A \to E$ 为次数 $\delta$ 的 $\varepsilon$ 派生。假设 A 具有单位元 1，并令 $x$ 为 A 的齐次元素，且 A 中有逆$x^{-1}$。则

$$
d(x^{-1}) = -\varepsilon_{\delta, \deg(x)} x^{-1}((dx)x^{-1}) = -\varepsilon_{\delta, \deg(x)} (x^{-1}(dx))x^{-1}.
$$

我们有 $d(xx^{-1}) = d(1) = 0$ (命题 3), 从而
$$
(dx)x^{-1} + \varepsilon_{\delta, \deg(x)} x(d(x^{-1})) = 0
$$
这就证明了(19)的第一个公式。另一方面，$x^{-1}$是次数$-\deg(x)$和$\varepsilon_{\delta, \deg(x)} = \varepsilon_{\delta, -\deg(x)}$齐次于no. 1的公式(1)；代入$d(x^{-1}x) = 0$，类似地得到(19)的第二个公式。

#### 命题 5 {#alg-iii-s10-prop-5 .statement tag=066M}

*假设$\mathbf{A}$为整环，令$\mathbf{L}$为分数的域。 $\mathbf{A}$ 的每个推导到向量空间 $\mathbf{E}$ 超过 $\mathbf{L}$（视为 $\mathbf{A}$ 模块）都可以唯一地扩展到 $\mathbf{L}$ 到 $\mathbf{E}$ 的推导。*

令$d$为$\mathbf{A}$的推导入$\mathbf{E}$，并将$\mathbf{L}$的$\bar{d}$推导入$\mathbf{E}$延伸$d$；那么，对于 $u \in \mathbf{A}, v \in \mathbf{A}, v \neq 0$，必然根据 (19)，
$$
\bar{d}(u/v) = v^{-1}du - uv^{-2}dv
$$
这就证明了$\bar{d}$的唯一性。相反，我们证明$\bar{d}$可以由公式(20)定义；首先必须验证当$u$被$u'$替代，$v$被$v'$替代时，(20)右边的$u/v = u'/v'$值是否不是变换。现在，$uv' = vu'$，因此$v'(du) + u(dv') = v(du') + u'(dv)$，因此$v'(du - uv^{-1}dv) = v(du' - u'{v'}^{-1}dv')$，因为$uv'v^{-1} = u'$和$u'{v'}^{-1}v = u$。因此映射 $\bar{d}: \mathbf{L} \to \mathbf{E}$ 被定义为扩展 $d$；立即验证它是$\mathbf{K}$-线性和推导。

#### 命题 6 {#alg-iii-s10-prop-6 .statement tag=066N}

*假设 $\mathbf{A}$ 是单位关联分级 $\mathbf{K}$-代数，$\mathbf{E}$ 是分级 $(\mathbf{A}, \mathbf{A})$ 双模。如果 $d : \mathbf{A} \to \mathbf{E}$ 是次数 $\delta$ 的 $\varepsilon$ 导数，则对于 $\mathbf{A}$ 的齐次元素的每个有限序列 $(x_i)_{1 \leq i \leq n}$，分别对应次数 $\xi_i$ ($1 \leq i \leq n$),
$$
d(x_1 x_2 \ldots x_n) = \sum_{i=1}^n \varepsilon_{\delta, \xi_1 + \cdots + \xi_{i-1}} x_1 \cdots x_{i-1} (dx_i) x_{i+1} \cdots x_n.
$$
公式 (21) 对于 $n = 0$ 来说是微不足道的，并由归纳在 $n$ 上证明，考虑到 (4) (no. 2)。

#### 推论{#alg-iii-s10-n5-cor-2 .statement tag=066O}

*假设$\mathbf{A}$是单位交换结合律代数，$\mathbf{E}$是$\mathbf{A}$模。如果 $d : \mathbf{A} \to \mathbf{E}$ 是推导，那么对于每个整数 $n \geq 0$，
$$
d(x^n) = nx^{n-1}(dx) \quad \text{for all } x \in \mathbf{A}.
$$
给予 $\mathbf{A}$ 简单的毕业并应用 (21) 就足够了，所有 $x_i$ 等于 $x$。

我们回到次数$\delta$的$\varepsilon$推导$d : \mathbf{A} \to \mathbf{E}$的一般情况。令$Z_\delta$为$a \in \mathbf{A}$的集合，使得对于次数$\alpha$的$a$的每个齐次分量$a_\alpha$，对于$\mathbf{E}$中的每个齐次$x$，
$$
xa_\alpha = \varepsilon_{\alpha, \deg(x)} a_\alpha x.
$$

如果 $A$ 是分级代数的单位结合律，而 $E$ 是分级的 $(A, A)$ 双模，则直接从定义得出 $Z_\varepsilon$ 是 $A$ 包含的*分级子代数* 单位元。

#### 命题 7 {#alg-iii-s10-prop-7 .statement tag=066P}

*假设 $A$ 是分级的单位结合律代数，而 $E$ 是分级的 $(A, A)$ 双模。令$d : A \to E$是次数$\delta$的$\varepsilon$衍生，$a$是次数$\alpha$的$Z_\varepsilon$的齐次元素。那么映射 $x \mapsto a(dx)$ 是次数 $\delta + \alpha$ 的 $\varepsilon$ 派生。*

我们写$d'(x) = a(dx)$；对于 $A$ 和 $y \in A$ 中次数 $\xi$ 的$x$齐次，根据 (23) 和 (1) (no. 1)，

$$
d'(xy) = a((dx)y) + \varepsilon_{\delta, \xi} a(x(dy)) = (a(dx))y + \varepsilon_{\delta+\alpha, \xi}(xa)(dy)
= (d'x)y + \varepsilon_{\delta+\alpha, \xi} x(d'y).
$$

命题 7 表示$\varepsilon$的K-模-从$A$到$E$的派生是型$\Delta$的*分级$Z_\varepsilon$*-模块。

### 6. 推导的代数

设$A$为分级的K-代数；对于每个*同质*元素$a \in A$，让$\mathrm{ad}_\varepsilon(a)$，或者简单地$\mathrm{ad}(a)$（如果不会引起混淆），将$A$的K-线性映射表示为$A$

$$
x \mapsto [a, x]_\varepsilon
$$
(no. 4, 公式 (10))，*分级为次数* $\deg a$。

#### 命题 8 {#alg-iii-s10-prop-8 .statement tag=066Q}

*让 $A$ 成为分级的 K-代数。*

(i) *对于$\varepsilon$*-导数$d : A \to A$和$A$的每个齐次元素$a$，

$$(24)$$
$$
[d, \mathrm{ad}_\varepsilon(a)]_\varepsilon = \mathrm{ad}_\varepsilon(da).
$$

(ii) *如果代数 $A$ 是结合律，$\mathrm{ad}_\varepsilon(a)$ 是次数 $\deg(a)$ 的 $A$ 的 $\varepsilon$* 导数。

(i) 假设$d$等于次数$\delta$，设$\alpha = \deg a$并写出$f = [d, \mathrm{ad}_\varepsilon(a)]_\varepsilon$。对于次数 $\xi$ 的每个齐次元素 $x \in A$，通过 (1) (no. 1)，我们有，

$$
f(x) = d(ax - \varepsilon(\alpha, \xi) xa) - \varepsilon_{\delta, \alpha}(a(dx)) - \varepsilon_{\alpha, \delta+\xi}(dx)a \\
= (da)x + \varepsilon_{\delta, \alpha} a(dx) - \varepsilon_{\alpha, \xi}(dx)a - \varepsilon_{\delta+\alpha, \xi} x(da) \\
- \varepsilon_{\delta, \alpha} a(dx) + \varepsilon_{\alpha, \xi}(dx)a \\
= (da)x - \varepsilon_{\delta+\alpha, \xi} x(da) = [da, x]_\varepsilon.
$$

(ii) 对于$A$中次数$\xi$的所有$x$齐次和次数$\eta$的所有$y$齐次，

$$
\mathrm{ad}_\varepsilon(a)(xy) = a(xy) - \varepsilon_{\alpha, \xi+\eta}(xy)a \\
= (ax - \varepsilon_{\alpha, \xi} xa)y + \varepsilon_{\alpha, \xi} x(ay - \varepsilon_{\alpha, \eta} ya) \\
= \mathrm{ad}_\varepsilon(a)(x).y + \varepsilon_{\alpha, \xi} x.\mathrm{ad}_\varepsilon(a)(y)
$$
考虑 (1) 和 $A$ 的结合性。

当$A$结合时，$\mathrm{ad}_\varepsilon(a)$称为$a$定义的$A$的*内部$\varepsilon$推导*。

#### 推论{#alg-iii-s10-n6-cor-1 .statement tag=066R}

*令 $A$ 为关联分级代数。对于两个齐次元素, $a, b$ 或 $A$,*
$$
[\mathrm{ad}_\varepsilon(a), \mathrm{ad}_\varepsilon(b)]_\varepsilon = \mathrm{ad}_\varepsilon([a, b]_\varepsilon).
$$
(25)

在(24)中，足以满足替换$d$乘以$\mathrm{ad}_\varepsilon(a)$和$\mathrm{ad}_\varepsilon(a)$乘$\mathrm{ad}_\varepsilon(b)$。

如果$\deg a = \alpha, \deg b = \beta$，公式(25)对于次数$\gamma$的每个齐次元素$c \in A$等价于以下关系
$$
\varepsilon_{\alpha, \gamma}[a, [b, c]_\varepsilon]_\varepsilon + \varepsilon_{\beta, \alpha}[b, [c, a]_\varepsilon]_\varepsilon + \varepsilon_{\gamma, \beta}[c, [a, b]_\varepsilon]_\varepsilon = 0
$$
称为*雅可比恒等式*。

### 7. 函数性质

*在这个数中，所有代数都被假定为结合且单位的，并且每个代数同态被假定为单位的。*

#### 命题 9 {#alg-iii-s10-prop-9 .statement tag=066S}

*令$A, B$为两个分级的$K$-代数，$E$为$(A, A)$-双模，$F$为分级的$(B, B)$-双模；设$\rho : A \to B$为代数同态的分级代数同态，$\theta : E \to F$为$A$双模的分级$A$同态（相对于$\rho$），次数0。则：*

*(i)* *对于每个 $\varepsilon$ 派生 $d' : B \to F$，$d' \circ \rho : A \to \rho^*(F)$ 是相同次数的 $\varepsilon$ 派生。*
*(ii)* *对于每个 $\varepsilon$ 派生 $d : A \to E$，$\theta \circ d : A \to \rho^*(F)$ 是相同次数的 $\varepsilon$ 派生。*

两个断言紧随关系而来
$$
d'(\rho(xy)) = d'(\rho(x)\rho(y)) = d'(\rho(x))\rho(y) + \varepsilon_{\delta', \xi}\rho(x)d'(\rho(y))
$$
$$
\theta(d(xy)) = \theta((dx)y + \varepsilon_{\delta, \xi}x(dy)) = \theta(dx)\rho(y) + \varepsilon_{\delta, \xi}\rho(x)\theta(dy)
$$
对于次数、$\xi$和$y \in A$的$x \in A$齐次，$\delta$和$\delta'$分别表示$d$和$d'$的次数。

#### 推论{#alg-iii-s10-n7-cor-1 .statement tag=066T}

*设$S$为代数$A$中的生成的系统。在阶和$d' \circ \rho = \theta \circ d$中，$d'(\rho(x)) = \theta(d(x))$对于所有$x \in S$来说是必要且充分的。*

这是命题 9 和 no. 5 的直接的推论，命题 3 的推论。

在命题 9 的条件下，我们知道$B$（通过$\rho$）有一个$(A, A)$双模结构（II, § 1, no. 14，*例 1*）。

#### 命题 10 {#alg-iii-s10-prop-10 .statement tag=066U}

*在命题 9 的条件下，对于$B$和$\rho^*(F)$上的左（右）$A$模块结构，$\varepsilon$-导数$d' : B \to F$为$A$线性，有必要且充分$d'$ 是零，位于 $B$ 的子代数 $\rho(A)$。*

我们为左A-模结构表演证明。对于$a \in A, b \in B$，
$$
d'(\rho(a)b) = d'(\rho(a))b + \rho(a)d'b
$$
因此，如果 $d' \circ \rho = 0$，$d'$ 对于 B 和 $\rho^*(F)$ 上的左A-模结构是线性的。相反，如果是这样的话，特别是
$$
d'(\rho(a)) = d'(\rho(a).1) = \rho(a)d'(1) = 0
$$
（no. 5，命题3）。

特别地，让$D_K(B, F)$表示B的推导到F中的K-模（no. 2）；其中推导是A线性的，在其他字中是$\rho(A)$上的零，形式是$D_K(B, F)$的子K模，用$D_{A,\rho}(B, F)$或简单地表示为$D_A(B, F)$（显然$D_K(B, F) = D_{K,\phi}(B, F)$，其中$\phi : K \to B$是同态，定义B)上的K-代数结构。

现在让A，B，C为三级K-代数，$\rho : A \to B, \sigma : B \to C$为二级代数同态，G为一个分级（C，C）双模；如果$D_A(B, G)$、$D_B(C, G)$和$D_A(C, G)$分别表示K-模、$D_{A,\rho}(B, \sigma_*(G))$、$D_{B,\sigma}(C, G)$和$D_{A,\sigma \circ \rho}(C, G)$，则$D_B(C, G)$显然是$D_A(C, G)$自$\sigma(\rho(A)) \subset \sigma(B)$以来的子K模。

#### 命题 11 {#alg-iii-s10-prop-11 .statement tag=066V}

*在上面的条件下，有正合序列个K-同态*
$$
0 \to D_B(C, G) \xrightarrow{u} D_A(C, G) \xrightarrow{v} D_A(B, G)
$$
*其中 u 为典范嵌入，v 同态 $d \mapsto d \circ \sigma$* (命题 9)。

v 的核是推导 $d : C \to G$ 的集合，使得所有 $b \in B$ 都有 $d(\sigma(b)) = 0$，这恰好是 u 的像。

### 8. 关系推导和代数同态之间

我们再次假设这个没有。 no. 2 的 *情况 (II)* 成立，且分级 K-代数 A 不假定为结合律。给定元素 $\delta \in \Delta$，考虑分级 K-模 E($\delta$) (II, § 11, no. 2)，使得
$$
(E(\delta))_\mu = E_{\mu+\delta}
$$
对于所有$\mu \in \Delta$。我们对K-模$A \oplus E(\delta)$进行定义*分级K-代数*结构按设定，对于$E(\delta)$中的每个同质元素$a \in A$和任意元素$a' \in A, x, x'$
$$
(a, x)(a', x') = (aa', x.a' + \varepsilon_{\delta, \deg(a)} a.x');
$$
验证这个乘法定义分级环结构是直接的。

投影$p : (a, x) \mapsto a$称为代数$A \oplus E(\delta)$的增强，是分级的代数同态。 次数 0 的分级 K-线性映射 $g : A \to A \oplus E(\delta)$ 使得合成

$$
A \xrightarrow{g} A \oplus E(\delta) \xrightarrow{p} A
$$

是身份$1_A$是形式$x \mapsto (x, f(x))$的映射，其中$f : A \to E$是次数$\delta$的分级K-线性映射。

#### 命题 12 {#alg-iii-s10-prop-12 .statement tag=066W}

*对于次数$\delta$的分级K-线性映射$f : A \to E$作为$\varepsilon$推导，A到$A \oplus E(\delta)$的映射$x \mapsto (x, f(x))$是分级的K-代数同态是必要且充分的。*

利用以下事实：对于 $A$ 和 $y \in A$ 中的 $x$ 齐次

$$
(xy, f(xy)) = (x, f(x)).(y, f(y)),
$$

考虑到 (28)，我们得到等价的关系

$$
f(xy) = f(x).y + \varepsilon_{\delta, \deg(x)} x.f(y),
$$

从而命题。

#### 命题 13 {#alg-iii-s10-prop-13 .statement tag=066X}

*为了使代数 $A \oplus E(\delta)$ 结合且单位，$A$ 结合且单位，并且 $E$ $(A, A)$ 双模结构上的映射 $(a, x) \mapsto a.x$ 和 $(a, x) \mapsto x.a$ 定义是充分必要的； $A \oplus E(\delta)$ 的单位元则为 $(1, 0)$。*

如果把元素$(u, m) \in A \oplus E(\delta)$写成这个代数的单位元，立刻发现$u$一定是$A$的单位元；写$(u, m).(0, x) = (0, x).(u, m) = (0, x)$，我们得到$x \in E$的$u.x = x.u = x$，写$(u, m).(u, 0) = (u, 0).(u, m) = (u, 0)$，我们得到$m = 0$。当$A \oplus E(\delta)$时$A$是结合律的事实是从增广为满同态的事实得出的。 条件 $(x.a').a'' = x.(a'.a'')$ 等价于 $((0, x)(a', 0))(a'', 0) = (0, x)((a', 0)(a'', 0))$，类似地条件 $a.(a'.x) = (a.a').x$ 等价于

$$
(a, 0)((a', 0)(0, x)) = ((a, 0)(a', 0))(0, x);
$$

最后条件 $a.(x.a') = (a.x).a'$ 相当于

$$
(a, 0)((0, x)(a', 0)) = ((a, 0)(0, x))(a', 0).
$$

### 9. 扩张的推导

#### 命题 14 {#alg-iii-s10-prop-14 .statement tag=066Y}

*令$A$为交换环，$M$为$A$模，$B$为$A$代数$T(M)$（分别为$S(M)$，分别为$\Lambda(M)$）和$E$ $(B, B)$-双模。令$d_0 : A \to E$为环$\mathbf{A}$的推导进入$\mathbf{A}$-模块$\mathbf{E}$和$d_1 : M \to \mathbf{E}$加法群同态，这样，对于所有$a \in \mathbf{A}$和所有$x \in M$，

$$
(29) \quad d_1(ax) = ad_1(x) + d_0(a) \cdot x,
$$

进一步，当$B = S(M)$时，

$$
(30) \quad x \cdot d_1(y) + d_1(x) \cdot y = y \cdot d_1(x) + d_1(y) \cdot x
$$

对于$M$中的所有$x, y$，并且当$B = \bigwedge(M)$时，

$$
(31) \quad x \cdot d_1(x) + d_1(x) \cdot x = 0
$$

对于所有$x \in M$。那么在$(B, B)$-双模$\mathbf{E}$中存在且仅有一个$B$（被视为$\mathbf{Z}$代数）的推导$d$，使得$d|_{\mathbf{A}} = d_0$和$d|_{M} = d_1$。

我们采用 $\mathbf{Z}$-模 $B \oplus \mathbf{E}$ 关联 $\mathbf{Z}$-代数结构定义为

$$
(b, t)(b', t') = (bb', bt' + tb')
$$

其中 $(1, 0)$ 为单位元 (no. 8, 命题 13)。 在典范嵌入 $t \mapsto (0, t)$ 下，$\mathbf{E}$ 被识别为$B \oplus \mathbf{E}$ 的双面理想，使得 $\mathbf{E}^2 = \{0\}$。 另一方面，$h_0(a) = (a, d_0(a))$定义的映射$h_0 : B \oplus \mathbf{E}$是单位环同态（no. 8，命题12）；在这个映射下，$B \oplus \mathbf{E}$就变成了$\mathbf{A}$代数。 此外，如果对于所有$x \in M$，我们写为$h_1(x) = (x, d_1(x))$，则从$h_0$的定义和(29)得出$h_1(ax) = h_0(a)h_1(x)$；在其他字$h_1$是$M$到$B \oplus \mathbf{E}$的$\mathbf{A}$线性映射。 那么存在一个且仅有一个$\mathbf{A}$-代数同态，$h : B \to B \oplus \mathbf{E}$使得$h|_M = h_1$（并且必然$h|_{\mathbf{A}} = h_0$）：对于，如果$B = T(M)$，则从$§ 5$，no. 1，命题1得出；如果 $B = S(M)$, 条件 (30) 表明$h(x)h(y) = h(y)h(x)$ 对于 $M$ 中的所有$x, y$ 且结论由 $§ 6$, no. 1, 命题 2 得出；最后，如果$B = \bigwedge(M)$，条件（31）表明，从$x \wedge x = 0$开始，对于所有$x \in M$，$(h(x))^2 = 0$，结论来自$§ 7$，no. 1，命题1。 同态$h$使得合成$p \circ h : B \to B$加上增强$\rho : B \oplus \mathbf{E} \to B$是身份$l_B$，对于$p \circ h$和$l_B$重合通过定义对于$\mathbf{A}$的元素和这些元素中的$M$和集合是$B$的生成的系统。 We can therefore write $h(b) = (b, d(b))$ for all $b \in B$ and the mapping $b \mapsto d(b)$ of $B$ into $\mathbf{E}$ is a derivation with the required properties, by virtue of Proposition 12 of no. 8.

#### 推论{#alg-iii-s10-n9-cor-1 .statement tag=066Z}

*令$M$为型$\Delta$的分级$K$模； $K$-代数$T(M)$、$S(M)$和$\bigwedge(M)$的相应的分度为型$\Delta' = \Delta \times \mathbf{Z}$（$§ 5$、no. 5、命题7、$§ 6$、 no. 6、命题 10 和 $§ 7$、no. 7、命题 11）。另一方面，$M$ 的分级为型 $\Delta'$，使得所有 $\alpha \in \Delta$ 为 $M_{\alpha, 1} = M_{\alpha}$，$\alpha \in \Delta$ 和 $n \neq 1$ 为 $M_{\alpha, n} = \{0\}$。令 $\varepsilon'$ 为交换因子超过 $\Delta'$。*

(i) 令 E 为型 $\Delta'$ 的分级（左和右）$\mathbf{T}(M)$-双模；对于所有$\delta \in \Delta$和每个整数$n \in \mathbf{Z}$，次数$\delta_1' = (\delta, n)$的每个分级K-线性映射$f : M \to E$都可以唯一地扩展到次数的$\varepsilon'$衍生$d : \mathbf{T}(M) \to E$ $\delta'$。

(ii) 令 E 为型 $\Delta'$ 的分级 $S(M)$ 模块；对于次数$\delta'$的分级K-线性映射$f : M \to E$可扩展到次数$\delta'$的$\varepsilon'$衍生$d : S(M) \to E$，有充分必要，对于每个有序对$(x, y)$ M 的齐次元素，

$$
x . f(y) + \varepsilon_{\delta', (\deg(y), 1)} y . f(x) = y . f(x) + \varepsilon_{\delta', (\deg(x), 1)} x . f(y).
$$

那么$\varepsilon'$-导数 d 是唯一的。

(iii) 令 E 为型 $\Delta'$ 的分级（左和右）$\Lambda(M)$-双模；对于次数$\delta'$的分级K-线性映射$f : M \to E$可扩展到$\varepsilon'$衍生

$$
d : \Lambda(M) \to E
$$

次数 $\delta'$，对于 M 的每个齐次元素 x，这是充分必要的，

$$
x . f(x) + \varepsilon_{\delta', (\deg(x), 1)} f(x) . x = 0.
$$

那么$\varepsilon'$-导数 d 是唯一的。

no. 2 的注 2 应用于 E 上的外部B-模律之一（B 等于$\mathbf{T}(M)$、$S(M)$ 或$\Lambda(M)$）修改；这样修改后的外法则仍然是，通过(1)(no. 1)，在E上得到的B-模律和B-模律仍然与其他B-模结构兼容。那么它就足以满足应用命题 14 与 $A = K$ 和 $d_0 = 0$ 的要求。

例 (1)。在命题 14 注的应用中，如果 $d_0 = 0$ 条件 (29) 只是意味着 $d_1$ 是 A 线性的。如果我们特别采用$E = B$和从B上的环结构导出的(B，B)双模结构，当$d_1$被取为M的自同态s的合成和典范嵌入$M \to B$时，条件(30)和(31)自动满足；这对于 (30) 来说是显而易见的，因为 $S(M)$ 是可交换的，而对于 (31) 来说，这是根据 x 和 $s(x)$ 在 $\Lambda(M)$ 中等于次数 1 的事实得出的。因此可以看出，M 的每个自同态 s 都可以唯一地扩展到 $\mathbf{T}(M)$ 的推导 $D_s$（分别为 $S(M)$、$\Lambda(M)$），即次数 0。此外，对于 M 的两个自同态 s，t，

$$
[D_s, D_t] = D_{[s, t]}
$$

两边都是 $\mathbf{T}(M)$ 的推导（分别为 $S(M)$，分别为 $\Lambda(M)$），等于 M 上的 $[s, t]$。

$D_s$ 的表达式是使用 no. 5 的公式 (21) 得到的，它分别给出，对于 $M$ 中的 $x_1, x_2, \ldots, x_n$，

$$
\begin{cases}
D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n) \\
\phantom{D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n)} = \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes s(x_i) \otimes x_{i+1} \otimes \cdots \otimes x_n \\
D_s(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 \ldots x_{i-1} s(x_i) x_{i+1} \ldots x_n \\
D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \\
\phantom{D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n)} = \sum_{i=1}^n x_1 \wedge \cdots \wedge x_{i-1} \wedge s(x_i) \wedge x_{i+1} \wedge \cdots \wedge x_n.
\end{cases}
$$

以代数$\Lambda(M)$为例，$D_s$有如下解释：

#### 命题 15 {#alg-iii-s10-prop-15 .statement tag=0670}

*如果$M$是有限秩$n$的自由$K$模块，那么，对于$M$的每个自同态$s$，推导$D_s$的限制到$\Lambda^n(M)$是位似比率 $\operatorname{Tr}(s)$.*

令$(e_j)_{1 \leq j \leq n}$为$M$的基并写成$e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$。如果
$$
s(e_j) = \sum_{k=1}^n \alpha_{jk} e_k,
$$
(36) 中的第三个公式给出
$$
D_s(e) = \sum_{i=1}^n e_1 \wedge \cdots \wedge e_{i-1} \wedge s(e_i) \wedge e_{i+1} \wedge \cdots \wedge e_n = \left( \sum_{j=1}^n \alpha_{jj} \right) e.
$$

*例 (2).* 在命题 14、部分 (iii) 的推论中，设$\Delta = \{0\}$，$\Lambda(M)$ 的毕业则为型 $\mathbf{Z}$ 的通常毕业；另一方面取$\varepsilon(p, q) = (-1)^{pq}$。然后，对于$M$上的每个线性形式$x^* \in M^*$，$x \mapsto \langle x, x^* \rangle$是$M$的次数$-1$到$\Lambda(M)$满足关系的分级$K$线性映射(34);那么存在$\Lambda(M)$、次数$-1$的*反导数*$i(x^*)$，使得（凭借no. 5的公式(21)）
$$
i(x^*)(x_1 \wedge \cdots \wedge x_n)
= \sum_{i=1}^n (-1)^{i-1} \langle x_i, x^* \rangle x_1 \wedge \cdots \wedge x_{i-1} \wedge x_{i+1} \wedge \cdots \wedge x_n
$$
这是内部乘积的特殊情况，在§ 11, no. 9，公式（68）中定义。

#### 命题 16 {#alg-iii-s10-prop-16 .statement tag=0671}

*令$A$为可交换的$K$-代数，$M_i$ ($1 \leq i \leq n$)和$P$$A$-模，以及$H$$A$的$A$-模-$M_1 \times M_2 \times \cdots \times M_n$*到P的多线性映射。假设有给定代数 A 的 K 导数 $d_0 : A \to A$，对于每个 i，K-线性映射 $d_i : M_i \to M_i$ 和 K-线性映射 $D : P \to P$，因此，对于 $1 \leq i \leq n$，$(d_0, d_i, d_i)$ 是 $(A, M_i, M_i)$ 自身的 K 导数，并且$(d_0, D, D)$ 是 $(A, P, P)$ 自身的 K 导数。那么存在 K-线性映射 $D' : H \to H$ 使得 $(d_0, D', D')$ 是 $(A, H, H)$ 自身的 K 导数，并且

(37) $D(f(x_1, \ldots, x_n))$

$$
= (D'f)(x_1, \ldots, x_n) + \sum_{i=1}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

对于所有$x_i \in M_i$，对于$1 \leq i \leq n$和$f \in H$。

我们证明，对于 $f \in H$，$M_1 \times M_2 \times \cdots \times M_n$ 的映射 $D'f$ 进入由 (37) 定义的 P 是 A-多重线性。对于$a \in A$，

$$
(D'f)(ax_1, x_2, \ldots, x_n) = D(af(x_1, \ldots, x_n)) - f(d_1(ax_1), x_2, \ldots, x_n)
$$
$$
-a \sum_{i=2}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

到假设

$$
D(af(x_1, \ldots, x_n)) = (d_0a)f(x_1, \ldots, x_n) + aD(f(x_1, \ldots, x_n))
$$

和 $d_1(ax_1) = (d_0a)x_1 + a.d_1x_1$，这给出

$$
(D'f)(ax_1, x_2, \ldots, x_n) = a.(D'f)(x_1, \ldots, x_n)
$$

并且类似地证明了每个$x_i$的线性。另一方面，

$$
(D'(af))(x_1, \ldots, x_n) = D(af(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^n af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n)) + aD(f(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^n af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n) + a(D'f)(x_1, \ldots, x_n)
$$

其他字

$$
D'(af) = (d_0a)f + a(D'f)
$$

从而建立命题。

#### 例 {#alg-iii-s10-n9-exa-1 .statement tag=0672}

(3) 应用命题 16 到情况$n = 1$、$M_1 = M$、$P = A$，然后是$H = M^*$，M 的对偶，可以看出，对于$(A, M, M)$ 的 K 导数$(d_0, d, d')$ 可以导出以下的 K 导数$(d_0, d^*, d^*)$ $(A, M^*, M^*)$ 这样

(38) $d_0\langle m, m^*\rangle = \langle dm, m^*\rangle + \langle m, d^*m^*\rangle$

对于 $m \in M$ 和 $m^* \in M^*$。 $M \oplus M^*$的K-线性映射自身等于$M$上的$d$和$M^*$上的$d^*$则满足条件(29)，因此存在$A$代数的$K$推导$D$ $T(M \oplus M^*)$，其中$A$约化至$d_0$，$M$至$d$，$M^*$至$d^*$。 $D$的限制$d_J^I$到$T(M \oplus M^*)$的子$A$模块$T_J^I(M)$（$§ 5$，no. 6）是$T_J^I(M)$的$K$自同态，使得$(d_0, d_J^I, d_J^I)$ 是 $(A, T_J^I(M), T_J^I(M))$ 的 $K$ 派生。此外，对于$i \in I, j \in J$，如果我们写$I' = I - \{i\}, J' = J - \{j\}$，立即验证对于收缩$c_j^i$（$§ 5$，no. 6）

$$
c_j^i(d_J^I(z)) = d_{J'}^{I'}(c_j^i(z)) \quad \text{for all } z \in T_J^I(M).
$$

(4) 设$M_i$($1 \leq i \leq 3$)为三个$A$模块，对于每个$i$，假设$(d_0, d_i, d_i)$是$(A, M_i, M_i)$的推导； $n = 1$、推导$(d_0, d_{ij}, d_{ij})$再次为应用命题16，$(A, H_{ij}, H_{ij})$，其中$H_{ij} = \operatorname{Hom}_A(M_i, M_j)$是为每个有序对$(i, j)$导出的。有了这个记号，对于$u \in \operatorname{Hom}_A(M_1, M_2)$和$v \in \operatorname{Hom}_A(M_2, M_3)$，

$$
d_{13}(v \circ u) = (d_{23}v) \circ u + v \circ (d_{12}u)
$$
定义立即验证了这一点。

### 10.通用问题适用于推导；非交换情况

在 $§ 10$ 的其余部分中，所有代数均假定为结合且单位的，并且所有代数同态均假定为单位的。

令 $A$ 为$K$-代数； 张量积 $A \otimes_K A$ 具有规范的 $(A, A)$ 双模块结构，在该结构下

$$
x . (u \otimes v) . y = (xu) \otimes (vy)
$$
对于 $A$ 中的所有$x, y, u, v$（$§ 4$、no. 3、例 2）。 $A$中$K$-线性映射$m : A \otimes_K A \to A$相应的到乘法（因此$m(x \otimes y) = xy$）是$(A, A)$-双模同态；因此，它的核 $I$ 是 $A \otimes_K A$ 的子双模。

#### 引理 1 {#alg-iii-s10-lem-1 .statement tag=0673}

*映射$\delta_A : x \mapsto x \otimes 1 - 1 \otimes x$是$A$到$I$的$K$衍生，并且$I$是由像生成$\delta_A$作为左$A$模块。*

第一个断言源自以下事实：

$$
(xy) \otimes 1 - 1 \otimes (xy) = (x \otimes 1 - 1 \otimes x) . y + x . (y \otimes 1 - 1 \otimes y)
$$
由（40）。另一方面，如果元素$\sum_i x_i \otimes y_i$（$A$中的$x_i, y_i$）属于到$I$，则定义$\sum_i x_i y_i = 0$，因此

$$
\sum_i (x_i \otimes y_i) = \sum_i x_i (1 \otimes y_i - y_i \otimes 1)
$$
通过 (40)，完成引理的证明。

#### 命题 17 {#alg-iii-s10-prop-17 .statement tag=0674}

*推导* $\delta_A$ *具有以下泛性质*：对于每个$(A, A)$-双模$E$和每个$K$-推导$d : A \to E$，存在且仅有一个$(A, A)$-双模同态 $f : I \to E$使得$d = f \circ \delta_A$。

注首先，对于每个$(A, A)$-双模同态 $f : I \to E$，$f \circ \delta_A$ 是推导（no. 7，命题 9）。相反，令 $d : A \to E$ 为 K 导数；那么我们首先证明，如果存在一个$(A, A)$-双模同态$f : I \to E$，使得$d = f \circ \delta_A$，$f$*由这个条件*唯一确定*，对于$\delta_A$的定义给出

$$
f(x \otimes 1 - 1 \otimes x) = dx
$$

而我们的断言是从$\delta_A$的像已经生成I作为左A-模（引理1）得出的：因此必然

$$
f\left( \sum_i x_i \otimes y_i \right) = \sum_i x_i \cdot f(1 \otimes y_i - y_i \otimes 1) = -\sum_i x_i \cdot dy_i.
$$

相反，由于$A \times A$到$E$的映射$(x, y) \mapsto -x \cdot dy$是$K$双线性，因此存在一个且仅有一个$K$线性映射$g : A \otimes_K A \to E$使得$g(x \otimes y) = -x \cdot dy$；只需验证 $g$ 到 $I$ 的限制 $f$ 是左 A 线性且右A-模结构即可。第一个断言从$(xx') \cdot dy = x \cdot (x' \cdot dy)$开始就很明显；证明第二个注，如果$\sum_i x_i \otimes y_i \in I$和$x \in A$，那么

$$
\sum_i x_i \cdot d(y_i x) = \sum_i x_i \cdot dy_i \cdot x + \sum_i (x_i y_i) \cdot dx
$$

但从$\sum_i x_i y_i = 0$到$I$的定义，这就完成了证明。

因此，我们定义了一个 *规范* $K$-模块 *同构的* $f \mapsto f \circ \delta_A$

$$
\operatorname{Hom}_{(A, A)}(I, E) \to D_K(A, E)
$$

左侧是$(A, A)$的$K$模，$A$的双模同态进入$E$。

### 11.通用问题适用于推导；交换案例

现在假设 $A$ 是一个*可交换的* $K$-代数，而 $E$ 是一个 $A$-*模*； $E$可以被认为是一个$(A, A)$双模，其两个外法则与给定的$A$-模律相同。另一方面，$A \otimes_K A$上的$(A, A)$双模结构与$A \otimes_K A$上的*交换环*结构产生的$(A \otimes_K A)$模结构相同，因为在这种情况下，对于$A$中的$x, y, u, v$，

$$
x \cdot (u \otimes v) \cdot y = (xu) \otimes (vy) = (xu) \otimes (yv) = (x \otimes y)(u \otimes v).
$$

因此，在这种情况下，$m$的核$\mathfrak{J}$是环$A \otimes_K A$的*理想*，并且由于$m : A \otimes_K A \to A$是满射，$(A \otimes_K A)/\mathfrak{J}$与$A$同构的；如果$E$也通过$m$被视为$(A \otimes_K A)$模块（在其他字中，$(A \otimes_K A)$模块$m_*(E)$），则$(A, A)$-*双模* 同态$\mathfrak{J} \to E$被识别为$(A \otimes_K A)$-*模* 同态 $\mathfrak{J} \to E$ (§ 4, no. 3)，在其他字中有一个规范的$K$-模块同构。

$$
\operatorname{Hom}_{(A, A)}(\mathfrak{J}, E) \to \operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E).
$$

另一方面，$\mathfrak{J}E = \{0\}$，对于元素 $1 \otimes x - x \otimes 1$ 生成 $\mathfrak{J}$ 作为 $(A \otimes_K A)$ 模块（no. 10，引理 1），并且对于所有 $z \in E$，

$$
(1 \otimes x - x \otimes 1)z = 0
$$

凭借$E$上的$(A \otimes_K A)$模块结构的定义。由于 $\mathfrak{J}$ 包含在 $(A \otimes_K A)$ 模块 $E$ 的湮没子中，并且 $E$ 上的 $((A \otimes_K A)/\mathfrak{J})$ 模块结构由定义构成，只是 $E$ 上给出的初始 $A$ 模块结构，因此，考虑到典范同构

$$
\mathfrak{J} \otimes_K ((A \otimes_K A)/\mathfrak{J})
$$

到$\mathfrak{J}/\mathfrak{J}^2$（§ 4, no. 1，推论1到命题1），一个规范的$K$-模块同构

$$
\operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E) \to \operatorname{Hom}_A(\mathfrak{J}/\mathfrak{J}^2, E).
$$

考虑到no. 10的命题 17，可以看出我们已经证明了以下命题：

#### 命题 18 {#alg-iii-s10-prop-18 .statement tag=0675}

*令 $A$ 为可交换的 $K$ 代数，而 $\mathfrak{J}$ 是满射典范同态 $m : A \otimes_K A \to A$ 的理想核，因此 $A$ 同构于 $(A \otimes_K A)/\mathfrak{J}$ 并且 $\mathfrak{J}/\mathfrak{J}^2$ 具有规范的$A$-模块结构。令$d_{A/K} : A \to I/I^2$为$K$线性映射，与$x \otimes 1 - 1 \otimes x$模$\mathfrak{J}^2$的每个$x \in A$类相关联。 映射 $d_{A/K}$ 是$K$-导数，并且对于每个$A$-模块$E$ 和每个$K$-导数$D : A \to E$，存在且仅有一个$A$-线性映射$g : \mathfrak{J}/\mathfrak{J}^2 \to E$，使得$D = g \circ d_{A/K}$.*

#### 例 {#alg-iii-s10-n11-exa-1 .statement tag=0676}

设M为K-模；从 no. 9 的命题 14 可以得出，对于每个 S(M)-模 E，映射 D ↦ D | M 定义 D_K(S(M), E) 到 Hom_K(M, E) 的 S(M) 模同构；另一方面，由于 E 是 S(M) 模，因此 Hom_K(M, E) 规范地同构于

$$
\operatorname{Hom}_{S(M)}(M \otimes_K S(M), E),
$$

M 到 E 的每个 K 同态都可以在形式 $x \mapsto h(x \otimes 1)$ 中唯一表达，其中

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E)
$$

（II, § 5, no. 1）。令D_0为K-导数$S(M) \to M \otimes_K S(M)$，其限制到M为典范同态$x \mapsto x \otimes 1$；因此，每个 K 导数 D : S(M) → E 都可以唯一地写为 $h \circ D_0$ ，其中

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E).
$$

由普遍映射问题的解唯一性可知，存在唯一的S(M)模同构

$$
\omega : M \otimes_K S(M) \to \Omega_K(S(M))
$$

使得 $D_0 \circ \omega = d_{S(M)/K}$；其他字，对于所有$x \in M$，$\omega(x \otimes 1) = dx$。

特别是，*如果 M 是自由K-模且基* $(e_\lambda)_{\lambda \in L}$，则 $\Omega_K(S(M))$ *是一个自由 S(M) 模，具有基集合的微分* $de_\lambda$。特别考虑$L = \{1, n\}$的情况，因此S(M)可以用多项式代数$K[X_1, \ldots, X_n]$(§ 6, no. 6)来识别；对于每个多项式$P \in K[X_1, \ldots, X_n]$，我们可以唯一地写出

$$
dP = \sum_{i=1}^n D_i P . dX_i
$$

与$D_i P \in K[X_1, \ldots, X_n]$，并且根据上述，映射$P \mapsto D_i P$是$K[X_1, \ldots, X_n]$相应的到$\Omega_K(S(M))$上的坐标形式对于基$(dX_i)$的*K-导数*；我们还写 $\frac{\partial P}{\partial X_i}$ 而不是 $D_i P$，这称为 P 相对于 $X_i$ 的*偏导数*。

### 12. K-微分的功能特性

#### 命题 19 {#alg-iii-s10-prop-19 .statement tag=0677}

*让*

$$
\begin{array}{ccc}
K & \xrightarrow{\rho} & K' \\
\downarrow \eta & & \downarrow \eta' \\
A & \xrightarrow{u} & A'
\end{array}
$$

*是交换环同态*、$\eta$（分别$\eta'$）的交换图表*制作*

A（分别为$A'$）转换为$K$-代数（分别为$K'$-代数）。存在且仅有一个$A$线性映射$v : \Omega_K(A) \to \Omega_{K'}(A')$渲染交换图表

$$
\begin{array}{ccc}
A & \xrightarrow{u} & A' \\
d_{A/K} \downarrow & & d_{A'/K'} \downarrow \\
\Omega_K(A) & \xrightarrow{v} & \Omega_{K'}(A')
\end{array}
$$

$d_{A'/K'} \circ u$ 是$A$-模块$\Omega_{K'}(A')$ 中$A$ 与值的$K$ 派生； $v$的存在性和唯一性则由no. 11的命题18得出。

命题 19 中的映射 $v$ 将表示为$\Omega(u)$；如果存在交换环同态的交换律图表

$$
\begin{array}{cccccc}
K & \xrightarrow{\sigma} & K' & \xrightarrow{\sigma'} & K'' \\
\eta \downarrow & & \eta' \downarrow & & \eta'' \downarrow \\
A & \xrightarrow{u} & A' & \xrightarrow{u'} & A''
\end{array}
$$

从命题 19 的唯一性性质立即得出

$$
\Omega(u' \circ u) = \Omega(u') \circ \Omega(u).
$$

由于 $\Omega_{K'}(A')$ 是 $A'$ 模块，因此我们从 $\Omega(u)$ 推导出规范的 $A'$ 线性映射

$$(41)$$
$$
\Omega_0(u) : \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

这样$\Omega(u)$是$\Omega_0(u)$和典范同态$i_A : \Omega_K(A) \to \Omega_K(A) \otimes_A A'$的合成。对于每个$A'$模$E'$，都有一个可交换的图表

$$
\begin{array}{ccc}
\operatorname{Hom}_{A'}(\Omega_{K'}(A'), E') & \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_{E'})} & \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \\
\phi_{A'} \downarrow & & \phi_A \circ r_A \downarrow \\
D_{K'}(A', E') & \xrightarrow{C(u)} & D_K(A, E)
\end{array}
$$

其中 $C(u)$ 为映射 $D \mapsto D \circ u$ (no. 7, 命题 9)，$r_A$ 为典范同构

$$
\operatorname{Hom}(i_A, 1_{E'}) : \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \to \operatorname{Hom}_A(\Omega_K(A), E');
$$

这紧接着命题 19 和定义的同构 $\phi_A$ 和 $\phi_{A'}$。

#### 命题 20 {#alg-iii-s10-prop-20 .statement tag=0678}

*假设 $A' = A \otimes_K K'$、$\eta': K' \to A'$ 和 $u: A \to A'$ 典范同态。然后是$A'$-线性映射*

$$
\Omega_0(u): \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

*是同构。*

由于图表 (42) 中的垂直箭头是双射的，约化到证明，对于每个 $A'$-模 $E'$，图表 (42) 中的同态 $C(u): D \mapsto D \circ u$ 是双射的（II, § 2, no. 1，定理1）。现在$\mathrm{Hom}(u, 1_{E'}): \mathrm{Hom}_{K'}(A \otimes_K K', E') \to \mathrm{Hom}_K(A, E')$是同构（II, § 5, no. 1，命题1），$C(u)$是它的限制到$D_{K'}(A', E')$，因此是单射的；此外，如果 $f: A' \to E'$ 是 $K'$ 线性映射，使得

$$
f \circ u: A \to E'
$$

是 $K$ 推导，它直接从以下事实得出：$f$ 是 $K'$ 线性的，并且 $f((x \otimes 1)(y \otimes 1)) = (y \otimes 1)f(x \otimes 1) + (x \otimes 1)f(y \otimes 1)$ 对于 $A$ 中的 $x, y$，$f$ 是$K'$-*推导*， 元素$x \otimes 1$用于$x \in A$形成$K'$模块$A'$的生成的系统；这完成了证明，$C(u)$是双射的。

从现在开始，我们将注意力集中在$\rho: K \to K'$是$K$的*恒等映射*的情况；因此，每个$K$-代数同态$u: A \to B$都映射到$B$-线性映射

$$
\Omega_0(u): \Omega_K(A) \otimes_K B \to \Omega_K(B).
$$

另一方面，我们可以考虑 $A$-*微分* $\Omega_A(B)$ 的 $B$ 模，因为 $B$ 是通过 $u$ 实现的 $A$ 代数；规范的推导 $d_{B/A}: B \to \Omega_A(B)$ 是 *更不必说* $K$ 的推导，它唯一分解为

$$
B \xrightarrow{d_{B/K}} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B)
$$

其中$\Omega_u$是$B$线性映射（no. 11，命题18）。对于每个$B$模$E$，都有一个可交换的图表

$$
\begin{array}{ccc}
\mathrm{Hom}_B(\Omega_A(B), E) & \xrightarrow{\mathrm{Hom}(\Omega_u, 1_E)} & \mathrm{Hom}_B(\Omega_K(B), E) \\
\downarrow \phi_{A,B} & & \downarrow \phi_{K,B} \\
D_A(B, E) & \xrightarrow{j_u} & D_K(B, E)
\end{array}
$$

其中 $j_u$ 是典范嵌入 (no. 7)；这紧随 no. 11 的命题 18 而来。

#### 命题 21 {#alg-iii-s10-prop-21 .statement tag=0679}

*$B$-线性映射的序列*

$$
\Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B) \to 0
$$

*准确。*

约化验证，对于每个 B-模 E，序列

$$
0 \to \operatorname{Hom}_B(\Omega_A(B), E) \xrightarrow{\operatorname{Hom}(\Omega_u, 1_E)} \operatorname{Hom}_B(\Omega_K(B), E) \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_E)} \operatorname{Hom}_B(\Omega_K(A) \otimes_A B, E)
$$

是精确的 (II, § 2, no. 1, 定理 1)；但由于在交换图表 (42) 和 (44) 中垂直箭头是同构，足以证明序列

$$
0 \longrightarrow D_A(B, E) \xrightarrow{j_u} D_K(B, E) \xrightarrow{C(u)} D_K(A, E)
$$

是准确的，正好是 no. 7 的命题 11。

我们现在考虑K-代数同态$u : A \to B$是满射的情况；如果$\mathfrak{J}$是它的核，则B与$A/\mathfrak{J}$同构的。我们考虑规范推导 $d = d_{A/K}$ 的限制 $d|_{\mathfrak{J}} : \mathfrak{J} \to \Omega_K(A)$ 和复合A-线性映射

$$
d' : \mathfrak{J} \xrightarrow{d|_{\mathfrak{J}}} \Omega_K(A) \xrightarrow{i_A} \Omega_K(A) \otimes_A B.
$$

然后$d'(\mathfrak{J}^2) = 0$，因为，对于$\mathfrak{J}$中的$x, y$，

$$
d'(xy) = d(xy) \otimes 1 = (x.dy + y.dx) \otimes 1 = dy \otimes u(x) + dx \otimes u(y) = 0
$$

从$u(x) = u(y) = 0$开始。因此，我们从 $d'$ 乘以经过得出商 A-线性映射

$$
\bar{d} : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_K(A) \otimes_A B
$$

当$\mathfrak{J}$消灭A-模$\mathfrak{J}/\mathfrak{J}^2$时，$\bar{d}$等于B-线性映射。

#### 命题 22 {#alg-iii-s10-prop-22 .statement tag=067A}

*令$\mathfrak{J}$为交换K-代数A、$B = A/\mathfrak{J}$和$u : A \to B$典范同态的理想。 序列 / B-线性映射*

$$
\mathfrak{J}/\mathfrak{J}^2 \xrightarrow{\bar{d}} \Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \to 0
$$

*那么准确。*

注，$\Omega_K(A) \otimes_A B$与$\Omega_K(A)/\mathfrak{J}\Omega_K(A)$相同，并且在该商模中，$\bar{d}$的像是$d(\mathfrak{J})$的像；因此，$\Omega_K(A) \otimes_A B$除以$\operatorname{Im}(\bar{d})$的商等于商$\Omega_K(A)/N$，其中N是由$\mathfrak{J}\Omega_K(A)$和$d(\mathfrak{J})$生成的子A模块。此外，复合映射

$$
A \xrightarrow{d_{A/K}} \Omega_K(A) \longrightarrow \Omega_K(A)/N
$$

是 K 导数 (no. 7, 命题 9)，并且由于它是 $\mathfrak{J}$ 上的零除以 N 的定义，因此它是定义，当经过为商时，K 导数$D_0 : B \to \Omega_K(A)/N$。

考虑到普遍映射问题的解的唯一性，约化到证明，对于每个 B-模 E 和每个 K 导数 D: B → E，存在唯一的 B-线性映射 g: Ω_K(A)/N → E 使得 D = g ∘ D_0。但是，复合映射 D ∘ u: A → E 是 K 导数 (no. 7, 命题 9)，因此存在且仅有一个 A-线性映射 f: Ω_K(A) → E 使得 f ∘ d_{A/K} = D ∘ u。这个关系已经表明 f 是 d(Σ) 上的零；同样 ΣE = {0}，因为 E 为 B-模，f 在 ΣΩ_K(A) 上为零；因此，f 在 N 和定义上为零，当经过为商时，B-线性映射 g: Ω_K(A)/N → E 使得 g ∘ D_0 = D； g 的唯一性由 f 的唯一性推出。

千万不要认为，即使 u: A → B 是单同态，Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) 是单射的 (习题 5)。然而我们有以下命题：

#### 命题 23 {#alg-iii-s10-prop-23 .statement tag=067B}

设 A 为 K-代数的积分，B 为分数的域，u：A → B 典范嵌入。则 Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) 为同构。

利用图表 (42) 中垂直箭头是双射的事实，约化到证明，对于 B 上的每个向量空间 E，映射 C(u)： D_K(B, E) → D_K(A, E) 是双射的。但这源于以下事实：A 到 E 的每个 K 推导都可以唯一地扩展到 B 到 E 的 K 推导（no. 5，命题 5）。

### 习题{#alg-iii-s10-exercises}

§ 10](exercises/s10/)参见[习题。
