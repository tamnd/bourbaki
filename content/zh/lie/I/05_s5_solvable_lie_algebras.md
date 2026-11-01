---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 5
section_title: Solvable Lie algebras
lang: zh
source: lie-i-iii
book_pages: 43-50, 99-101
pdf_pages: 0061-0068, 0117-0119
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF SOLVABLE LIE ALGEBRAS
      page: 43
      pdf_page: 61
    - "no": 2
      title: RADICAL OF A LIE ALGEBRA
      page: 44
      pdf_page: 62
    - "no": 3
      title: NILPOTENT RADICAL OF A LIE ALGEBRA
      page: 44
      pdf_page: 62
    - "no": 4
      title: A CRITERION FOR SOLVABILITY
      page: 47
      pdf_page: 65
    - "no": 5
      title: FURTHER PROPERTIES OF THE RADICAL
      page: 48
      pdf_page: 66
    - "no": 6
      title: EXTENSION OF THE BASE FIELD
      page: 49
      pdf_page: 67
statements: 27
exercises: 17
content_sha256: 0dd234ea04980598fba7e0e892c74940f930a7cf322f7c8c96dc64c50bb7f2b7
translated_from: content/en/lie/I/05_s5_solvable_lie_algebras.md
translation_method: google
source_content_sha256: 17ded9a5fe0c8a2a7818b8d120cc2777d7e553298aff0352151f7762860f3aac
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 30150f086398d787f400fa5d8c756f53baf9b7c240e1a97d24303c8dcd669c89
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。 可解李代数

回想一下，$K$ 从此表示特征 0 的域，并且所有李代数都假设为 $K$ 上的有限维。†

### 1. 定义 / 可解李代数

#### 定义 1 {#lie-i-s5-def-1 .statement tag=09Y1}

*如果李代数$g$的第k个派生代数$D^k g$对于足够大$k$来说是零，则称为可解。*

幂零李代数是可解的。

#### 命题 1 {#lie-i-s5-prop-1 .statement tag=09Y2}

*子代数和可解李代数的商代数是可解的。可解代数与可解代数的每个扩张都是可解的。可解代数的每个有限乘积都是可解的。*

令 $g$ 为李代数、$g'$ 子代数、$h$ $g$、$t = g/h$ 和$\phi$ 典范映射 $g$ 到 $t$ 的理想。如果 $g$ 可解，则 $D^k g = \{0\}$ 对于某些整数 $k$，因此 $D^k g' \subset D^k g = \{0\}$、$D^k t = \phi(D^k g) = \{0\}$ 以及$g'$ 和 $t$ 是可解的。如果 $h$ 和 $t$ 可解，则存在整数 $s, t$ 使得

$$
D^s h = D^t t = \{0\};
$$

那么$D^t g \subset h$，因此$D^{s+t} g = D^s(D^t g) \subset D^s h = \{0\}$和$g$是可解的。 最后一个断言从第二个开始，接着是因子的数上的归纳。

#### 命题 2 {#lie-i-s5-prop-2 .statement tag=09Y3}

*令$g$为李代数。以下条件是等效的：*

(a) $g$ 是可解的；
(b) *存在 $g$ 的理想递减序列 $g = g_0 \supset g_1 \supset \cdots \supset g_n = \{0\}$，使得代数 $g_i/g_{i+1}$ 是可交换的 ($i = 0, 1, \ldots, n-1$)；*
(c) *存在$g$的子代数的递减序列$g = g'_0 \supset g'_1 \supset \cdots \supset g'_p = \{0\}$，使得$g'_{i+1}$是$g'_i$的理想且$g'_i/g'_{i+1}$是可交换的($i = 0, 1, \ldots, p-1$)；*
(d) *存在$g$的子代数的递减序列$g = g''_0 \supset g''_1 \supset \cdots \supset g''_q = \{0\}$，使得$g''_{i+1}$是余维1 ($i = 0, 1, \ldots, q-1$)的$g''_i$的理想。*

(a) $\Rightarrow$ (b)：考虑 $g$ 的派生理想中的序列就足够了。
(b) $\Rightarrow$ (c)：这是显而易见的。
(c)$\Rightarrow$(d)：假设条件(c)成立； $g'_i$ 包含 $g'_{i+1}$ 的每一个向量子空间都是$g'_i$、从而的理想立即 (d)。
(d) $\Rightarrow$ (a)：这直接源于以下事实：可解的代数与可解的代数的扩张是可解的。

† 读者会发现注 $K$ 的特性中的假设并未在第 1 条中使用。本段 1 和 2。

例 / 可解李代数

I。令 $g$ 为 $K$ 和 $(e_1, e_2)$ 基的二维向量空间 $g$。在$g$上存在且仅有一个交错的双线性乘法$(x, y) \mapsto [x, y]$使得$[e_1, e_2] = e_2$。很容易验证$g$由此给出可解李代数结构。现在让$h$是维数2超过$K$的非交换李代数。我们证明$h$与$g$同构的。令 $(f_1, f_2)$ 为 $h$ 的基。 元素$[f_1, f_2]$非零（否则$h$将是可交换的），因此它生成是$h$的一维子空间$t$。然后$[h, h] = t$。令$(e'_1, e'_2)$为$h$的基，使得$e'_2 \in t$。然后 $[e'_1, e'_2] = \lambda e'_2$ 与 $\lambda \neq 0$。 替换$e'_1$乘$\lambda^{-1} e_1$，可以假设$\lambda = 1$，从而我们的断言。

II。 § 1的公式(5)证明$\mathscr{D}t(n, K) = n(n, K)$。由于 $n(n, K)$ 是幂零的，因此是可解的，因此 $t(n, K)$ 是可解的。因此$st(n, K)$是可解的。特别地，$st(2, K)$同构于例I的代数。

### 2. 李代数的根式

令 $a, b$ 为李代数 $g$ 的两个可解理想。 代数 $(a + b)/b$ 与 $a/(a \cap b)$ 同构的，因此可解，而 $a + b$（$(a + b)/b$ 的扩张除以 $b$）也是可解的 (命题 1)。由此可见，$g$包含的最大可解理想，$g$的每个可解理想，因此$g$有最大的可解理想。这使我们能够做出以下定义：

#### 定义 2 {#lie-i-s5-def-2 .statement tag=09Y4}

*李代数的根式是它的最大的可解理想。*

#### 命题 3 {#lie-i-s5-prop-3 .statement tag=09Y5}

*李代数$g$的根式$r$是$g$的最小的理想，使得$g/r$有根式$\{0\}$。*

令$a$为$g$和$\phi$典范映射的$g$到$g/a$的理想。如果$g/a$的根式是零，那么$g/a$的可解理想$\phi(r)$就是零；因此$r \subset a$。

另一方面，$g/r$的部首$r'$的逆像$\phi^{-1}(r')$是$g$的理想，它可由命题1解出，因此等于$r$；因此$r' = \{0\}$。

#### 命题 4 {#lie-i-s5-prop-4 .statement tag=09Y6}

*令$g_1, \ldots, g_n$为李代数。 $g_i$的乘积的部首$r$是$g_i$的部首$r_i$的乘积。*

$r_i$ 的乘积 $r'$ 是可解理想 (命题 1)，因此是 $r' \subset r$。 $g_i$中$r$的典范像是$g_i$的可解理想，因此包含在$r_i$中；因此$r \subset r'$。

### 3. 李代数的幂幂

#### 定义 3 {#lie-i-s5-def-3 .statement tag=09Y7}

*令$g$为李代数。 $g$的幂零根式是$g$的有限维简单表示的核的交。*

#### 注 {#lie-i-s5-n3-rem-1 .statement tag=09Y8}

(1) 设$s$为$g$的幂零根。由于$g$的向量子空间的每个递减序列都是平稳的，因此存在$g$的有限维简单表示的有限数，其核有交$s$。

其中表示中的直和是半单并且有核 s。由此可见，g的有限维半单表示的集合或核有至少元素，即s。

(2) 由§ 4, no. 3的命题4(c)，s也是g的有限维表示的最大的幂零理想交。特别是，s 包含在 g 的最大的幂零理想中，因此是 g 的幂零理想。

(3) g 上的每个线性形式 $\lambda$（即 $\mathscr{D}g$ 上的零）都是 g 的简单表示（带有空间 K），从而 $\lambda(s) = \{0\}$。由此可见$s \subset \mathscr{D}g$。另一方面，s 由注 2 包含在g 的根r r 中。我们将证明$s = r \cap \mathscr{D}g$。

#### 引理 1 {#lie-i-s5-lem-1 .statement tag=09Y9}

令 V 为 K 上的有限维向量空间，gl(V) 的 g 子代数，使得 V 是一个简单的 g 模，并且是 g 的交换理想。然后$a \cap \mathscr{D}g = \{0\}$。令 S 为由 1 和 a 生成的 $\mathscr{L}(V)$ 的子代数。

如果 b 是 a 中包含的 g 的理想，使得 $\operatorname{Tr} bs = 0$ 对于所有 $b \in b$ 和所有 $s \in S$，则特别是，通过 S 的定义，对于每个整数 $n > 0$ $\operatorname{Tr}(b^n) = 0$，因此 b 是幂零的（代数， 章VII, § 5, no. 5，推论4至命题13)；因为 b 的元素都是幂零的，$b = \{0\}$ (§ 4, no. 3, 引理 2)。我们首先将其应用于 g 的理想 $[g, a]$。如果$x \in g, a \in a, s \in S$，则从$as = sa$起$\operatorname{Tr}[x, a]s = \operatorname{Tr}(xas - axs) = \operatorname{Tr} x(as - sa) = 0$；因此$[g, a] = \{0\}$。因此 g 的元素与 a 的交换，因此也与 S 的交换。如果 $x, y$ 属于到 g 和 $s \in S$，则

$$
\operatorname{Tr}[x, y]s = \operatorname{Tr}(xys - yxs) = \operatorname{Tr} x(ys - sy) = 0
$$

从 $ys = sy$ 开始；则取b为理想的$\mathscr{D}g \cap a$，则可得出$\mathscr{D}g \cap a = \{0\}$。

#### 定理 1 {#lie-i-s5-thm-1 .statement tag=09YA}

设 g 为李代数，r 为其根式，s 为幂零根式。然后$s = \mathscr{D}g \cap r$。

我们已经知道$s \subset \mathscr{D}g \cap r$。因此，只要证明如果 $\rho$ 是 g 的有限维简单表示，则 $\rho(\mathscr{D}g \cap r) = \{0\}$ 就足够了。令 k 为最小整数 $\geq 0$，使得 $\rho(\mathscr{D}^{k+1}r) = \{0\}$；我们写$g' = \rho(g)$，$a' = \rho(D^k r)$；由于$\mathscr{D}^k r$是g的理想，$a'$是$g'$的理想；这个理想从 $\rho(\mathscr{D}^{k+1}r) = \{0\}$ 开始是可交换的。如果V是$\rho$的空间，则$g' \subset \operatorname{gl}(V)$和V是一个简单的$g'$模块。然后$\rho(\mathscr{D}g \cap \mathscr{D}^k r) \subset \mathscr{D}g' \cap a' = \{0\}$。如果$k > 0$，则$\mathscr{D}^k r \subset \mathscr{D}g$和$\rho(\mathscr{D}^k r) = \{0\}$，与k的定义相反。因此$k = 0$，即

$$
\rho(\mathscr{D}g \cap r) = \{0\}.
$$

#### 推论 1 {#lie-i-s5-thm-1-cor-1 .statement tag=09YB}

设g为可解李代数。 g 的幂零根是$\mathscr{D}g$。如果$\rho$是g的有限维简单表示，$\rho(g)$是可交换的，并且由1和$\rho(g)$生成的结合律代数L是K上有限次数的域。

这里$r = g$，从而$s = \mathscr{D}g$。因此$\varphi(\mathscr{D}g) = \{0\}$，它表明$g' = \rho(g)$是可交换的。 $L$ 的每个元素 $\neq 0$ 都可以通过 Schur 的引理可逆；因此$L$是域。

#### 推论2（谎言的定理）{#lie-i-s5-thm-1-cor-2 .statement tag=09YC}

*设$g$为可解李代数；假设 $K$ 是代数封闭的。令$M$为有限维在$K$上的$g$模，并令$(M_i)_{0 \leq i \leq r}$为$M$的Jordan-Hölder级数。那么，对于$1 \leq i \leq r$，$M_{i-1}/M_i$ 是$K$ 上的维数 1，对于所有$x \in g$，$x_{M_{i-1}/M_i} = \lambda_i(x) \cdot 1$，其中$\lambda_i$ 是$g$ 上的线性形式，$\mathscr{D}g$ 上是零。特别是，有限维超过$K$的每个简单$g$模实际上是维数 1。*

令$\rho_i$为$M_{i-1}/M_i$上$g$的表示。 1 和 $\rho_i(g)$ 生成的结合律代数 $L_i$ 是域，是 $K$ 的有限扩张，因此等于 $K$； $M_{i-1}/M_i$是一个简单的$L_i$模块，从而$\dim M_{i-1}/M_i = 1$。其余的推论是显而易见的。

#### 注 {#lie-i-s5-n3-rem-2 .statement tag=09YD}

(1) 如果将$(M_i)_{0 \leq i \leq r}$替换为$M$的另一个Jordan-Hölder级数，序列$(\lambda_1, \ldots, \lambda_r)$替换为形式$(\lambda_{\pi(1)}, \ldots, \lambda_{\pi(r)})$的序列，其中$\pi$为置换 $\{1, \ldots, r\}$，如下来自 Jordan-Hölder 定理。

(2) 设$(e_1, \ldots, e_r)$为$M$的基，使得$e_i \in M_{i-1}, e_i \notin M_i$($1 \leq i \leq r$)。如果$M$相应的到$x$的$x \in g$自同态关于这个基由一个三角形矩阵表示，其对角线系数为

$$
\lambda_1(x), \ldots, \lambda_r(x).
$$

#### 推论 3 {#lie-i-s5-thm-1-cor-3 .statement tag=09YE}

*假设 $K$ 是代数闭的。如果$g$是$r$维可解李代数，则$g$的每个理想都是维数$r, r-1, \ldots, 0$的理想的递减序列中的项。*

每个理想都是 $g$ 的 Jordan-Hölder 级数的部分，被视为伴随表示的空间（*代数*，章 I, § 6, no. 14，定理 8 的推论）；那么应用推论2就足够了。

#### 推论 4 {#lie-i-s5-thm-1-cor-4 .statement tag=09YF}

*假设$K = \mathbf{R}$。设$g$为可解李代数。 $g$ 的每个简单表示都是维数 $\leq 2$。 $g$ 的每个理想都是递减序列 $(g_i)_{0 \leq i \leq m}$ 理想中的项，使得 $g_0 = g, g_m = \{0\}, \dim g_{i-1}/g_i \leq 2$ ($1 \leq i \leq m$)。

这与推论 2 和推论 3 的证明方式类似，使用 $\mathbf{R}$ 的每个代数扩张都是次数 $\leq 2$。*

#### 推论 5 {#lie-i-s5-thm-1-cor-5 .statement tag=09YG}

*要使李代数 $g$ 可解，$\mathscr{D}g$ 幂零是充分必要的。*

根据推论 1，条件是必要的。它是充分的，因为$g/\mathscr{D}g$ 是可交换的。

#### 推论 6 {#lie-i-s5-thm-1-cor-6 .statement tag=09YH}

*令$\varphi$为李代数$g$中的有限维表示。令* r 为g 的根式。每个元素$x \in r$使得$\rho(x)$是幂零属于到最大的$\rho$的幂零理想$n$。

令V为$\rho$中的空间；令$(V_i)_{0 \leq i \leq r}$为V上r模块结构的Jordan-Hölder级数，并让$\rho_i$为r的表示，其中空间$V_i / V_{i-1}$（$1 \leq i \leq r$）。如果$\rho(x)$是幂零的，那么$\rho_i(x)$也是幂零的；至于$\rho_i(x)$生成的所有$i$代数是域，$\rho_i(x) = 0$。相反，如果 $\rho_i(x) = 0$ 对于所有 $i$，则$\rho(x) = 0$。这表明$x \in r$的集合$a$使得$\rho(x)$幂零是r的理想。另一方面，$[g, a] \subset \mathscr{D}g \cap r \subset n \cap r \subset a$ 因此$a$ 是 g 的理想。这就证明了$a \subset n$。

#### 推论 7 {#lie-i-s5-thm-1-cor-7 .statement tag=09YI}

设 g 为李代数，r 为其根式。以下四个集合是相同的： (a) g 的最大的幂零理想； (b) r 最大的幂零理想； (c) $x \in r$的集合使得$\mathrm{ad}_g x$幂零； (d) $x \in r$ 的集合使得 $\mathrm{ad}_r x$ 幂零。

让这些集合表示为$a, b, c, d$。内含物$a \subset b \subset d \subset c$清晰。 $c \subset a$ 由推论 6 应用于 g 的伴随表示。

### 4. 可解性的标准

#### 引理 2 {#lie-i-s5-lem-2 .statement tag=09YJ}

令$x$为有限维向量空间V的自同态，并且s（分别为n）其半单（分别为幂零）分量（cf.代数、章VIII, § 9, no. 4、定义4）。令$\mathrm{ad}\, x, \mathrm{ad}\, s, \mathrm{ad}\, n$为$x, s, n$在$\mathfrak{gl}(V)$的伴随表示中各自的像。那么$\mathrm{ad}\, s$（或$\mathrm{ad}\, n$）是$\mathrm{ad}\, x$的半单（或幂幂）分量，并且等于$\mathrm{ad}\, x$中的多项式，系数为K且没有常数项。

我们知道$\mathrm{ad}\, x = \mathrm{ad}\, s + \mathrm{ad}\, n, [\mathrm{ad}\, s, \mathrm{ad}\, n] = 0$和$\mathrm{ad}\, n$是幂零的（$§ 4$，引理1）。我们证明$\mathrm{ad}\, s$是半单。当 K 是代数闭集 (cf. 代数, 章 VIII, § 9, no. 2, 命题 3) 时就足够了。然后令 $(e_i)_{1 \leq i \leq n}$ 为 V 的基，使得 $s(e_i) = \lambda_i e_i$ ($\lambda_i \in K$)。令$(E_{ij})$为$M_n(K) = \mathfrak{gl}(V)$中的典范基。到 $§ 1$ 公式 (5) 为止，

$$
(\mathrm{ad}\, s)\cdot E_{ij} = (\lambda_i - \lambda_j)E_{ij}
$$

因此 $\mathrm{ad}\, s$ 是半单。 引理中的最后一个断言源自代数、章VIII, § 9, no. 4、命题8。

#### 引理 3 {#lie-i-s5-lem-3 .statement tag=09YK}

设M为有限维向量空间，A和B为$\mathfrak{gl}(M)$的两个向量子空间，使得$B \subset A$，并且T为$t \in \mathfrak{gl}(M)$的集合，使得$[t, A] \subset B$。如果$z \in T$对于所有$u \in T$来说$\mathrm{Tr}(zu) = 0$是这样的，那么$z$是幂零的。

当 K 是代数封闭时就足以证明这一点，我们将在以后假设这一点。令 s 和 n 为半单和 z 的幂零分量，并令 $(e_i)$ 为 M 的基，使得 $s(e_i) = \lambda_i e_i$ ($\lambda_i \in K$)。令 $V \subset K$ 为向量空间超过由 $\lambda_i$ 生成的 $\mathbf{Q}$。我们需要证明$V = \{0\}$。令 f 为 V 上的 $\mathbf{Q}$ 线性形式，令 t 为 M 的自同态，使得

$te_i = f(\lambda_i)e_i$。如果$(E_{ij})$是由$E_{ij}e_k = \delta_{jk}e_i$定义的$\mathfrak{gl}(M)$的典范基，则
$$
\begin{align*}
(\mathrm{ad}\ s)E_{ij} &= (\lambda_i - \lambda_j)E_{ij} \\
(\mathrm{ad}\ t)E_{ij} &= (f(\lambda_i) - f(\lambda_j))E_{ij}.
\end{align*}
$$

存在一个没有常数项且 K 中的系数使得对于所有 i 和 j 为 $P(\lambda_i - \lambda_j) = f(\lambda_i) - f(\lambda_j)$ 的多项式 P（如果$\lambda_i - \lambda_j = \lambda_h - \lambda_k$，则$f(\lambda_i) - f(\lambda_j) = f(\lambda_h) - f(\lambda_k)$，如果$\lambda_i - \lambda_j = 0$，$f(\lambda_i) - f(\lambda_j) = 0$）。然后$\mathrm{ad}\ t = P(\mathrm{ad}\ s)$。另一方面，$\mathrm{ad}\ s$ 是一个多项式，$\mathrm{ad}\ z$ 中没有常数项。现在$(\mathrm{ad}\ z)(A) \subset B$，从而还有$(\mathrm{ad}\ t)(A) \subset B$。 假设$0 = \mathrm{Tr}(zt) = \sum \lambda_i f(\lambda_i)$、从而$0 = f(\mathrm{Tr}(zt)) = \sum f(\lambda_i)^2$。由于$f(\lambda_i)$是有理数数、$f = 0$，从而完成证明。

#### 定理 2（嘉当准则）{#lie-i-s5-thm-2 .statement tag=09YL}

*设 g 为 M 上 g 的李代数、M 有限维向量空间、ρ 表示，以及与 ρ 相关的 g 上的 β 双线性形式。那么 ρ(g) 是可解的当且仅当 $\mathscr{D}$g 相对于 β 与 g 正交。*

显然可以简化为g是$\mathfrak{gl}(M)$的李子代数且ρ是恒等映射的情况。如果 g 可解，则 $\mathscr{D}$g 包含在 g (定理 1) 的恒等式表示的最大的幂零理想中，因此相对于 β (§ 4, 命题 4 (d)) 与 g 正交。假设 $\mathscr{D}$g 与 g 关于 β 正交。我们证明g是可解的。令 T 为 $t \in \mathfrak{gl}(M)$ 的集合，使得 $[t, g] \subset \mathscr{D}g$。如果 $t \in T$ 和 x, y 属于到 g，则 $[t, x] \in \mathscr{D}g$ 因此
$$
\mathrm{Tr}(t[x, y]) = \beta([t, x], y) = 0
$$
对于所有$u \in \mathscr{D}g$，从而按线性$\mathrm{Tr}(tu) = 0$计算。另外，显然$\mathscr{D}g \subset T$。因此，(引理 3) $\mathscr{D}$g 中的每一个元素都是幂零的。由此可知 $\mathscr{D}$g 是幂零的（§ 4，推论 3 到定理 1），因此 g 是可解的（no. 3，推论 5 到定理 1）。

### 5. 激进派的更多特性

#### 命题 5 {#lie-i-s5-prop-5 .statement tag=09YM}

*设 g 为李代数，r 为根式。*
(a) *如果 ρ 是 g 的有限维表示，且 β 是关联的双线性形式，则 r 和 $\mathscr{D}$g 相对于 β 正交。*
(b) *r 是 $\mathscr{D}$g 相对于 Killing 形式的正交。*
设 x, y 为 g，$z \in r$。然后$[y, z] \in \mathscr{D}g \cap r$，因此
$$
\beta([x, y], z) = \beta(x, [y, z]) = 0
$$
（定理1）。因此(a)。
令 r' 为 $\mathscr{D}$g 相对于 Killing 形式的正交。由上可知，是g(§ 3, no. 6,命题7(a))的理想，其中包含r。另一方面，g 的伴随表示下 r' 的像 s 是可解的 (定理 2)，因此 r' 作为 s 的中心扩张是可解的。因此 r' ⊂ r。

#### 推论 1 {#lie-i-s5-prop-5-cor-1 .statement tag=09YN}

设g为李代数。那么 g 是可解的当且仅当 $\mathscr{D}g$ 相对于 Killing 形式与 g 正交。

这是命题 5 (b) 中的直接的推论。

#### 推论 2 {#lie-i-s5-prop-5-cor-2 .statement tag=09YO}

李代数 g 的根式 r 是一个特征理想。

$\mathscr{D}g$ 是一个特征理想，而杀戮形式是完全不变的（§ 3, no. 6，命题 10）。因此，$\mathscr{D}g$相对于杀戮形式的正交是一个特征理想（§ 3, no. 6，命题 7 (b)）。

#### 推论 3 {#lie-i-s5-prop-5-cor-3 .statement tag=09YP}

设 g 为李代数，r 为 g 的根式，a 为 g 的理想。那么a的根式就等于$r \cap a$。

r ∩ a 是 a 的可解理想，因此包含在 a 的根式 r' 中。相反，r' 是 g 的理想（推论 2 和 § 1, no. 4、命题 2），因此 r' ⊂ r。

推论2可以更精确如下：

#### 命题 6 {#lie-i-s5-prop-6 .statement tag=09YQ}

设g为李代数，r为根式，n为最大的幂零理想。 g 映射 r 的每个推导转化为 n。

令 D 为 g 的推导。令 g' = g + Kx_0 为李代数，其中 g 是余维 1 的理想，使得对于所有 x ∈ g (§ 1, no. 8, 例 1)，Dx = [x_0, x]。根据推论3至命题5，r包含在g'的基团r'中。则 D(r) = [x_0, r] ⊂ [g', g'] ∩ r' = s'。对于所有 x ∈ s'，ad_{g'} x 是幂零的 (定理 1)。因此，对于所有 x ∈ s' ∩ g，ad_g x 是幂零的。因此 D(r) 包含在 g 的幂零理想 s' ∩ g 中。

#### 推论{#lie-i-s5-n5-cor-1 .statement tag=09YR}

最大的李代数的幂零理想是特征理想。

#### 注 {#lie-i-s5-n5-rem-1 .statement tag=09YS}

总结上面的一些结果，注，若r、n、s、t分别表示g的根、最大的g的幂零理想、g的幂零根以及g相对于Killing形式的正交，则

$$
r \supset t \supset n \supset s.
$$

包含于 r ⊃ t 由命题 5 (b) 得出。包含于 t ⊃ n 由 § 4, no. 4, 命题 6 (b) 得出。包含n ⊃ s 已在no. 3 的注 2 中指出。

### 6. 扩张基域

令 g 为 K 的李子 K-代数且 K_1 扩张。显然，当且仅当 g 可解时，g_{(K_1)} 才可解，因为 $\mathscr{D}^n(g_{(K_1)}) = (\mathscr{D}^n g)_{(K_1)}$。

设 r 为 g 的根式。那么$r_{(K_1)}$ *是* $g_{(K_1)}$的根式。让 $\beta$ 成为 g 的杀戮形式。由于r是$\mathscr{D}g$相对于$\beta$的正交(命题 5 (b))，$r_{(K_1)}$是$(\mathscr{D}g)_{(K_1)} = \mathscr{D}(g_{(K_1)})$相对于形式的正交，由$\beta$通过扩张从K到$K_1$导出，即杀戮形式共 $g_{(K_1)}$ (§ 3, no. 8)。我们的断言是从命题 5 (b) 的进一步应用得出的。

### 习题{#lie-i-s5-exercises}

§ 5 的约定仍然有效，除非另有提及。

参见[习题为 § 5](exercises/s5/)。
