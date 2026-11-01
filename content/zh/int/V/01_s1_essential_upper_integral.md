---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 1
section_title: Essential upper integral
lang: zh
source: int-i-vi
book_pages: INT V.2-INT V.11
pdf_pages: 0257-0266, 0349-0350
extraction: ocr
subsections:
    - "no": 1
      title: Definition of the essential upper integral
      page: 2
      pdf_page: 257
    - "no": 2
      title: Moderated functions and measures
      page: 4
      pdf_page: 259
    - "no": 3
      title: Essentially integrable functions
      page: 7
      pdf_page: 262
    - "no": 4
      title: A property special to the essential upper integral
      page: 10
      pdf_page: 265
statements: 22
exercises: 6
content_sha256: 6af9b01a833452cd0bcfe5b768172b376fbbb9fee958cf73a1fbc6c7a4cf88c6
translated_from: content/en/int/V/01_s1_essential_upper_integral.md
translation_method: google
source_content_sha256: d19dbe1131a1bb0064d0db8332b6983acb2090fbcf25d4ea5abb63e1585fb1b0
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 8bd09ecd58a57e5e4890eb536e598cbf224a76f7383514d4fdc39a75447f70a9
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。基本上衣整体

### 1. 本质上积分的定义

#### 定义 1 {#int-v-s1-def-1 .statement tag=08ZO}

对于每个函数 $f \in \mathscr{F}_+(T)$，我们调用 $f$ 关于 $\mu$ 的本质上积分，并用 $\mu^\bullet(f)$ 表示，即数 $\mu^*(f \varphi_K)$ 集合的上界，无论是否有限，其中 $K$ 超出$T$紧凑子集集合。对于$T$中的每子集$A$，有一个集合$\mu^\bullet(A) = \mu^\bullet(\varphi_A)$。

还使用记号$\int^\bullet f d\mu$、$\int^\bullet f(t) d\mu(t)$、$\int^\bullet f \mu$。
由于 $f \varphi_K \leq f$ 对于 $T$ 的每个紧凑子集 $K$，有

$$
\int^\bullet f d\mu \leq \int^* f d\mu .
$$

有可能发生$\mu^\bullet(f) \neq \mu^*(f)$；其中，条件$\mu^*(f) = 0$表示$f$可以忽略，而条件$\mu^\bullet(f) = 0$表示$f$局部可忽略（第IV, §5, No. 2，命题5），并且可能存在局部可忽略但不可忽略的集合（第1章）。 IV, §1，Exer 5）。

将$\mathscr{F}_+(T)$的映射$\mu^\bullet$放入$\overline{\mathbf{R}}$重合，将$\mu$放入$\mathscr{K}_+(T)$。由此可见，两个度量 $\mu_1$ 和 $\mu_2$ 使得 $\mu_1^\bullet = \mu_2^\bullet$ 相等。

#### 命题 1 {#int-v-s1-prop-1 .statement tag=08ZP}

a) 如果$f$和$g$是两个几乎处处局部相等的数值函数$\geq 0$，则$\mu^\bullet(f) = \mu^\bullet(g)$。
b) 如果$f$和$g$是两个数值函数$\geq 0$使得$f \leq g$，则$\mu^\bullet(f) \leq \mu^\bullet(g)$。
c) 如果 $f$ 是数字函数 $\geq 0$，且 $\alpha$ 是数 $\geq 0$，则$\mu^\bullet(\alpha f) = \alpha \mu^\bullet(f)$。
d) 如果$f$和$g$是两个数字函数$\geq 0$，则$\mu^\bullet(f + g) \leq \mu^\bullet(f) + \mu^\bullet(g)$。
e) 如果$(f_n)_{n \in \mathbf{N}}$是数值函数$\geq 0$的递增序列，并且如果$f = \lim_{n \to \infty} f_n$，则$\mu^\bullet(f) = \lim_{n \to \infty} \mu^\bullet(f_n)$。

属性 a)、b)、c)、d) 可以立即从上积分的相应的属性中推导出来：a) 从 Ch 的命题 6 中推导出来。 Ch. IV, §2, No. 3 和命题 5 IV, §5, No. 2； b), c), d) 来自第 10, 11, 12 章的命题 10, 11, 12 IV, §1, No. 3。 为建立e)，用$T$的紧致子集的$\mathfrak{K}$集合表示；由 Ch. 定理 3 IV, §1, No. 3，我们有

$$
\lim_{n \to \infty} \mu^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{K \in \mathfrak{K}} \mu^*(f_n \varphi_K) = \sup_{K \in \mathfrak{K}} \sup_{n \in \mathbf{N}} \mu^*(f_n \varphi_K)
= \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K) = \mu^\bullet(f) .
$$

等式在关系 d) 中成立，如果 $f$ 和 $g$ 可测量，由 Cor. 4 Th。 5，CH。 IV, §5, No. 6。更一般地，我们得到以下结果：

#### 命题 2 {#int-v-s1-prop-2 .statement tag=08ZQ}

*令$f, g, h$为$\mathscr{F}_+$中的三个元素；如果 $g$ 和 $h$ 可测量，则*

$$
\int^\bullet f(g + h)\, d\mu = \int^\bullet fg\, d\mu + \int^\bullet fh\, d\mu.
$$

对于上积分，一立即减少到类似公式的证明。从$f(g + h) = fg + fh$开始（按照$0 \cdot (+\infty) = 0$的约定），我们有

$$
\int^* f(g + h)\, d\mu \leq \int^* fg\, d\mu + \int^* fh\, d\mu;
$$

剩下的就是建立相反的不等式。令$u$为下半连续函数，使得$u \geq f(g + h)$。 集合$v = \frac{u}{g + h}$在集合，其中$g + h > 0$，以及$v = +\infty$在集合，其中$g + h = 0$；然后$v \geq f$和$u \geq v(g + h)$，从而

$$
\int^* v(g + h)\, d\mu \leq \int^* u\, d\mu
$$

因而， $v$ 是可测量的（第 IV, §5, No. 6 章，第 5 章第 4 章），

$$
\int^* fg\, d\mu + \int^* fh\, d\mu \leq \int^* vg\, d\mu + \int^* vh\, d\mu \\
= \int^* v(g + h)\, d\mu \leq \int^* u\, d\mu,
$$

这意味着所需的不等式，因为$u$是任意的。

#### 推论 {#int-v-s1-n1-cor-1 .statement tag=08ZR}

*令$f$为可测函数$\geq 0$的函数$\geq 0$、$(g_n)$序列；然后$\int^\bullet f \left( \sum_n g_n \right) d\mu = \sum_n \left( \int^\bullet f g_n\, d\mu \right)$。

对于有限序列的情况，这是命题2的直接的推论。无限序列的情况可以由此通过命题1，e）推导出来。

#### 命题 3 {#int-v-s1-prop-3 .statement tag=08ZS}

*对于每个有限的数$\alpha \geq 0$和$\mathbf{T}$上的每个对措施$\mu, \nu$，

$$
(\alpha \mu)^\bullet = \alpha \mu^\bullet \\
(\mu + \nu)^\bullet = \mu^\bullet + \nu^\bullet.
$$

此外，关系$\mu \leq \nu$意味着$\mu^\bullet \leq \nu^\bullet$。*

证明是直接的，来自第 1 章中类似的叙述。 IV（§1, No. 3，提案 15）。

#### 命题 4 {#int-v-s1-prop-4 .statement tag=08ZT}

— *对于每个数值函数* $f \geqslant 0$ *在* $T$、$\mu^\bullet(f) = \mu^*(f)$ 上是下半连续的。

例如，令$g$为$\mathscr{K}_+(T)$中的函数，使得$g \leqslant f$。如果$K$是$g$的（紧）支持，则$\mu(g) \leqslant \mu^*(f \varphi_K) \leqslant \mu^\bullet(f)$。根据上积分的定义，得出 $\mu^*(f) \leqslant \mu^\bullet(f)$，因而 $\mu^*(f) = \mu^\bullet(f)$ (公式 (1))。

### 2. 审核函数和措施

#### 命题 5 {#int-v-s1-prop-5 .statement tag=08ZU}

— *设* $A$ *为* $T$ 的子集； *以下属性是等效的*：
a) *集合*$A$*包含在*$\mu$*的序列并-可积开集合*。
b) *集合*$A$*包含在*$\mu$*的序列并-可积集合*。
c) *集合* $A$ *包含在紧集的序列并和a*$\mu$*-可忽略的集合*。

很明显，属性 a) 和 c) 都隐含 b)。相反，b) 意味着 a)，因为有限外部测度的每个集合都包含在可积开集合（第 IV, §1, No. 4，命题 19）中，并且 b) 意味着 c)，因为每个可积集合是序列的并紧集和可忽略不计的集合（第 IV, §4, No. 6 章，第 4 章第 2 章）。

#### 定义 2 {#int-v-s1-def-2 .statement tag=08ZV}

—*$T$*的*子集*如果满足命题5*的等价条件，则称为*$\mu$*-调节。 *函数定义在* $T$上，*与向量空间或* $\overline{\mathbf{R}}$中的值，*如果它是零在a* $\mu$*-调节的补码上，则被认为是* $\mu$*-调节子集*$T$。 *测量* $\mu$ *如果* $T$ *是* $\mu$*-调节的集合*，则据说是经过调节的。

如果$\mu$是调节措施，则$T$上的每个函数都是$\mu$调节，$T$的每个子集都是$\mu$调节。

#### 注 {#int-v-s1-n2-rem-1 .statement tag=08ZW}

— 1) 如果 $\theta$ 是 $T$ 的复杂测度，如果 $f$ 是 $|\theta|$ 调节（或者 $|\theta|$ 调节），则可以说函数 $f$ 是 $\theta$ 调节（或 $\theta$ 调节）。
2) 每个有界措施都经过调节；如果$T$是紧集的可数并，则$T$上的每个度量都会被调节。
3) 令$(f_n)$为$\mu$调节的函数的序列，其中值在$\overline{\mathbf{R}}$中。对于每个$n$，令$U_n$是一个开集合，它是有限外部测度的开集合的可数并，使得$f_n$是$U_n$之外的零。 函数 $s = \sum_{n \in \mathbf{N}} |f_n|$ 那么零在 $\bigcup_{n \in \mathbf{N}} U_n$ 之外；因此它是 $\mu$ 调节的，对于所有函数 $f$ 也是如此，这样 $|f| \leq s$ 。这尤其适用于函数 $\liminf_{n \to \infty} f_n$、$\limsup_{n \to \infty} f_n$ 和 $\sum_{n \in \mathbf{N}} f_n$（如果定义了和）。

4) 函数几乎在任何地方都等于经过调节的函数被调节。

#### 命题 6 {#int-v-s1-prop-6 .statement tag=08ZX}

— *令$f$为在$T$上定义的正数值函数，即$\mu$可测量且$\mu$可调节。则存在$\mathscr{F}_+(T)$的元素的序列$(h_n)_{n \in \mathbf{N}}$，其中和等于$f$，具有以下性质：*

1) *函数 $h_0$ 是$\mu$-可以忽略不计。*
2) *对于每个$n \geq 1$，都存在紧集$K_n$，使得$h_n$在$K_n$之外是零，并且$h_n$到$K_n$的限制是有限且连续的。*

假设$f$是正可测函数的序列$(f_n)$中的和，其中叙述中各有性质；显然$f$也有。 集合
$$
f_n = \inf(f, n+1) - \inf(f, n)
$$
每$n \in \mathbf{N}$；由于 $f$ 等于序列 $(f_n)$ 的和，因此假设 $f$ 受到调节且“有界”，则足以建立命题。然后用$t \in T$的$A$集合表示，使得$f(t) > 0$； $A$是可测量和调节的，因此存在序列$(A_n)$成对的不相交的可积集合使得$A = \bigcup_n A_n$。我们将函数$f \varphi_{A_n}$减少为证明叙述；在其他字中，我们可以假设$f$是有界的并且零位于可积集合$I$之外。但$I$是可忽略不计的集合$N$的并和成对不相交的紧集的序列$(L_n)$（第IV, §4, No. 6章，第4章的Cor.2）。因此，我们只能处理 $f$ 有界且零在紧集 $L$ 之外的情况。

令$\mathscr{K}$为$T$的紧凑子集$K$的集合，使得$f|K$是连续的；由于 $\mathscr{K}$ 是 $\mu$ 稠密（第 IV, §5, No. 10 章，第 15 条），$L$ 是可忽略不计的集合 $N$ 和序列 $(K_n)_{n \geq 1}$ 的并成对不相交的元素，共 $\mathscr{K}$（第 IV, §5, No. 8 章，定义 6）。 函数 $h_0 = f \varphi_N$、$h_n = f \varphi_{K_n}$ $n \geq 1$ 然后满足条件叙述。

下面的命题使得约化将上积分的研究变成本质上积分的研究成为可能。

#### 命题 7 {#int-v-s1-prop-7 .statement tag=08ZY}

— *令 $f$ 为 $\mathscr{F}_+(T)$ 的元素。*
1) *如果函数 $f$ 不是 $\mu$ 调节，则 $\mu^*(f) = +\infty$。*
2) *如果函数 $f$ 是 $\mu$ 调节，则 $\mu^*(f) = \mu^*(f)$。*
3) *如果$\mu^*(f) < +\infty$，则存在$\mu$调节的子集$A$、序列的并，以及$T$的紧凑子集，使得$f = f \varphi_A$局部几乎无处不在。

第一个断言紧接着第 1 章的引理 1。 IV, §5, No. 6。为了建立第二个，用 $A$ 表示一个经过调节的子集，使得 f 是 A 之外的零； A 是可忽略不计的集合 $A_0$ 的并和紧集的序列 $(A_n)_{n \geq 1}$，我们可以假设是递增。 函数 $f$ 几乎处处都等于函数 $f \varphi_{A_n}$ ($n \geq 1$) 的上包络线，因此（第 IV, §1, No. 3、第 3 章和§2, No. 3、第 6 条命题）

$$
\mu^*(f) = \lim_{n \to \infty} \mu^*(f \varphi_{A_n}) \leq \mu^\bullet(f),
$$

从而等式 $\mu^*(f) = \mu^\bullet(f)$ 凭借公式 (1)。最后，假设$\mu^\bullet(f) < +\infty$；存在紧集的递增序列 $(A_n)$ 使得

$$
\mu^\bullet(f) = \sup_n \mu^*(f \varphi_{A_n}).
$$

集合$A = \bigcup_n A_n$；第二个成员等于$\mu^*(f \varphi_A)$（第IV, §1, No. 3，Th.3），即$\mu^\bullet(f \varphi_A)$（根据上述第1条或第2条）。由于$\mu^\bullet(f) = \mu^\bullet(f \varphi_A) + \mu^\bullet(f \varphi_{\mathbf{C}_A})$（命题2），我们有$\mu^\bullet(f \varphi_{\mathbf{C}_A}) = 0$，由此得出3）。

#### 推论 1 {#int-v-s1-prop-7-cor-1 .statement tag=08ZZ}

*要使 f 可以忽略不计，其局部可忽略且可调节是必要且充分的。*

#### 推论 2 {#int-v-s1-prop-7-cor-2 .statement tag=0900}

*如果 $\mu$ 是一个调节测度（特别是如果 $\mu$ 有界，或者如果 T 在无穷大处可数），则 $\mu^* = \mu^\bullet$。*

#### 命题 8 {#int-v-s1-prop-8 .statement tag=0901}

a) *设H为函数$\geq 0$的集合，下半连续，指向关系$\leq$；那么*

$$
\mu^\bullet \left( \sup_{h \in H} h \right) = \sup_{h \in H} \mu^\bullet(h).
$$

b) *设H为函数$\geq 0$的集合，上半连续，指向关系$\geq$；如果 H 函数 $h_0$ 中存在$\mu^\bullet(h_0) < +\infty$，则*

$$
\mu^\bullet \left( \inf_{h \in H} h \right) = \inf_{h \in H} \mu^\bullet(h).
$$

根据命题 4，断言 a) 是第 1 章定理 1 的重复。 IV, §1, No. 1。建立b)，集合$\eta = \inf_{h \in H} h$，令$a$为数$> 0$。存在紧集 K 使得（第 IV, §4, No. 4 章，第 5 条命题第 1 条）：

$$
\mu^\bullet(h_0) - a \leq \mu^*(h_0 \varphi_K) = \mu(h_0 \varphi_K) \leq \mu^\bullet(h_0).
$$

函数$h\varphi_K$，其中$h$运行于上半连续函数的$H$、形式集合，指向关系$\geqslant$，其中包含可积函数。因此（第 IV, §4, No. 4 章，第 5 号提案第 2 条）：

$$
\mu^*(\eta\varphi_K) = \inf_{h \in H} \mu^*(h\varphi_K).
$$

但是（第 IV, §4, No. 4 章，第 5 条命题第 1 条）对于每个函数 $h \in H$，$\mu^\bullet(h_0\varphi_{C_K}) \leqslant a$、从而 $\mu^\bullet(h\varphi_{C_K}) \leqslant a$ 使得 $h \leqslant h_0$。因此，最后：

$$
\mu^\bullet(\eta) \geqslant \mu^*(\eta\varphi_K) = \inf_{h \in H} \mu^*(h\varphi_K) \geqslant \inf_{h \in H} \mu^\bullet(h) - a.
$$

不等式$\mu^\bullet(\eta) \leqslant \inf_{h \in H} \mu^\bullet(h)$是明显的，$a$是任意的，命题成立。

### 3.本质上可积函数

让$F$成为真正的巴纳赫空间；请记住，空间 $\mathscr{F}_F^p$（第 IV, §3, No. 3 章）和 $\mathscr{L}_F^p$（第 IV, §3, No. 4，定义 2）中的元素是 $\mu$ 调节的函数（第 IV, §5, No. 6、引理） 1）；由于$\mathscr{N}_F$仍将$T$的可忽略的映射的空间表示为$F$，我们将把$T$的局部可忽略的映射的空间$\mathscr{N}_F^\infty$引入$F$。

#### 引理 {#int-v-s1-n3-lem-1 .statement tag=0902}

*设$g$和$g'$是两个$\mu$调节的映射，其中值在$F$中；如果 $g$ 和 $g'$ 几乎在任何地方都等于相同的函数 $f$，则 $g = g'$ 几乎在任何地方都相等。*

例如，令$D$为$t \in T$的集合，使得$g(t) \neq g'(t)$； $D$ 局部可以忽略不计并且经过调节，因此可以忽略不计（第 7 号提案的第 1 条）。

我们将用$\overline{\mathscr{F}}_F^p(T, \mu)$（或简称为$\overline{\mathscr{F}}_F^p(\mu)$，$\overline{\mathscr{F}}_F^p$，如果不会造成混淆）将$T$的映射$f$的集合表示为$F$，使得存在函数$g \in \mathscr{F}_F^p$等于$f$当地几乎到处都是。由于数$N_p(g)$仅依赖于$f$乘以引理，我们将写成$\overline{N}_p(f) = N_p(g)$。 函数$\overline{N}_p$显然是$\overline{\mathscr{F}}_F^p$的半范数，我们总是假设$\overline{\mathscr{F}}_F^p$配备有$\overline{N}_p$定义的拓扑。这个拓扑的0的闭包是空间$\mathscr{N}_F^\infty$； 关系 $\overline{\mathscr{F}}_F^p = \mathscr{F}_F^p + \mathscr{N}_F^\infty$、$\mathscr{N}_F^\infty \cap \mathscr{F}_F^p = \mathscr{N}_F$ (引理) 表明规范化的空间 $\overline{\mathscr{F}}_F^p / \mathscr{N}_F^\infty$ 可以与 $\mathscr{F}_F^p / \mathscr{N}_F$ 规范地一致，这是完整的（第 IV, §3, No. 3 章，第 5 条）；因此$\overline{\mathscr{F}}_F^p$本身是完整的。

我们同样用$\overline{\mathscr{F}}_F^p$的$\overline{\mathscr{L}}_F^p(T, \mu)$（或$\overline{\mathscr{L}}_F^p(\mu)$，或$\overline{\mathscr{L}}_F^p$）子空间$\mathscr{L}_F^p + \mathscr{N}_F^\infty$来表示；也可以将$\overline{\mathscr{L}}_F^p$表征为$\overline{\mathscr{F}}_F^p$的子空间，由*可测量的*映射构成（第IV, §5, No. 6，第5章）。

规范化的空间$\overline{\mathscr{L}}_F^p / \mathscr{N}_F^\infty$可以与$L_F^p$规范地识别；因此$\overline{\mathscr{L}}_F^p$是完整的。 它的元素被称为 *p-th 幂本质上是可积函数*，这个术语由以下命题证明是合理的：

#### 命题 9 {#int-v-s1-prop-9 .statement tag=0903}

*对于T的映射 f到F到属于到$\overline{\mathscr{F}}_F^p$（分别到$\overline{\mathscr{L}}_F^p$），如果是必要和充分的*（分别是*f是可测量的并且*）

$$
\mu^\bullet(|f|^p) < +\infty .
$$

*则有*$\overline{N}_p(f) = (\mu^\bullet(|f|^p))^{1/p}$。

关于$\overline{\mathscr{F}}_F^p$，我们可以清楚地从极限自己到断言。如果 f 属于至 $\overline{\mathscr{F}}_F^p$，则令 g 为函数属于至 $\mathscr{F}_F^p$，几乎处处局部等于 f；那么 $|f|^p = |g|^p$ 几乎无处不在，因此

$$
\mu^\bullet(|f|^p) = \mu^\bullet(|g|^p) = \mu^*(|g|^p) < +\infty
$$

（命题 1，a）和命题 7），另一方面，通过 $\overline{N}_p$ 的定义，

$$
\overline{N}_p(f) = N_p(g) = (\mu^*(|g|^p))^{1/p} .
$$

相反，假设$\mu^\bullet(|f|^p) < +\infty$；则存在一个经过调节的集合 A，使得 f 在 T − A 中几乎所有地方都局部为零（命题 7）。 函数 $f \varphi_A$，几乎在任何地方都等于 f，使得 $N_p(f \varphi_A) = \overline{N}_p(f) < +\infty$，因此它属于到 $\mathscr{F}_F^p$，以及 $f \in \overline{\mathscr{F}}_F^p$。

#### 推论{#int-v-s1-n3-cor-1 .statement tag=0904}

*对于f到属于到$\mathscr{L}_F^p$，f属于到$\overline{\mathscr{L}}_F^p$是必要且充分的并且被调节。*

#### 定义 3 {#int-v-s1-def-3 .statement tag=0905}

* $\overline{\mathscr{L}}_F^1$ 的元素实质上被称为 F 中与值的 $\mu$ 可积函数。 将 $L_F^1$ 的映射 $\tilde{f} \mapsto \mu(f)$ 组合到 F 中，将 $\overline{\mathscr{L}}_F^1$ 的典范映射组合到 $L_F^1$ 上，得到连续将$\overline{\mathscr{L}}_F^1$的线性映射转化为F，将$\mathscr{L}_F^1$的扩展映射$f \mapsto \int f d\mu$转化为F。再将$f \in \overline{\mathscr{L}}_F^1$的映射的$\int f d\mu$或$\mu(f)$值表示，并且这元素称为 f 右 $\mu$ 的积分。*

几乎处处局部相等的两个本质上可积函数具有相同的积分。对于每个有限且本质上可积的函数$f \geq 0$，$\int^\bullet f d\mu = \int f d\mu$。如果 A 是集合，其特征函数本质上可积，则 A 被称为 *本质上 $\mu$ 可积集合*； $\int \varphi_A d\mu$ 也表示为 $\mu(A)$，再次称为 A 的*度量*。

If a function $f$, with values in $F$, is defined locally almost everywhere in $T$, we again say that $f$ is *essentially integrable* if it is equal, locally almost everywhere, to a function $f_1$ that is everywhere defined and integrable; we then set
$$
\int f\, d\mu = \int f_1\, d\mu,
$$
and this definition is independent of the integrable function $f_1$ everywhere defined and equal locally almost everywhere to $f$ (Lemma). One defines similarly the notion of essentially integrable function for functions with values in $\overline{\mathbf{R}}$ that are defined and finite locally almost everywhere.

读者将毫无困难地将第 1 章的结果扩展到本质上可积函数。 IV, §4 代表可积函数，替换叙述中的“几乎无处不在”，由“本地几乎无处不在”。我们注为了例不等式
$$
\left| \int f\, d\mu \right| \leq \int |f|\, d\mu,
$$
对于 Banach 空间中的每个可积函数 $f$ 和值都有效。

#### 命题 10 {#int-v-s1-prop-10 .statement tag=0906}

*令$\mathfrak{K}$为$T$的紧凑子集的$\mu$密集集合。*
a) *如果 $f$ 是数字函数 $\geq 0$，则*
$$
\mu^\bullet(f) = \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K).
$$
b) *如果 $f$ 实质上是可积函数且值位于 Banach 空间 $F$ 中，则*
$$
\int f\, d\mu = \lim_{\mathfrak{K}} \int f \varphi_K\, d\mu,
$$
*极限是相对于指示（对于$\subset$）集合$\mathfrak{K}$而言的。*

为了建立 a)，只需证明对于 $T$ 的每个紧凑子集 $L$，
$$
\int^* f \varphi_L\, d\mu = \sup_K \int^* f \varphi_K\, d\mu,
$$
其中$K$超过$L$属于到$\mathfrak{K}$的子集的集合。由于$L$是可忽略不计的集合的并和$\mathfrak{K}$的元素的递增序列$(K_n)$（第IV, §5, No. 8，第12章），这是从定理到上积分中的极限（第 IV, §1, No. 3 章，第 3 章）。

现在假设$f$属于到$\mathscr{L}_F^1$；令$\varepsilon$为数$> 0$，并令$K$为$\mathfrak{K}$的元素，使得
$$
\int |f| \varphi_K\, d\mu \geq \int |f|\, d\mu - \varepsilon
$$

（这样的 K 由 a) 存在。然后，对于每个紧集 H 包含 K，

$$
\left| \int f \, d\mu - \int f \varphi_H \, d\mu \right| \leq \int |f| \varphi_{\mathbf{C}_H} \, d\mu \leq \int |f| \varphi_{\mathbf{C}_K} \, d\mu \leq \varepsilon .
$$

扩张到复杂的 Banach 空间和措施。设 F 为复数 Banach 空间；通过滥用记号，F 下的真正的 Banach 空间也将被表示为 F。那么 Banach 空间 $\overline{\mathscr{L}}_F^p(T, \mu)$ 可能会配备一个自然复数 Banach 空间结构，并且有必要具体说明是使用该实数还是复数结构空间。在这个章中，如果没有明确提及相反的情况，它将始终被理解为真正的结构。

令 $\theta$ 为复测度；我们集合$\overline{\mathscr{L}}_F^p(T, \theta) = \overline{\mathscr{L}}_F^p(T, |\theta|)$；如果 F 是复数 Banach 空间，则可以得到与上面相同的注。特别是，如果函数 f 与 F 中的值对于 $\theta$ 本质上可积，则它对于 $|\theta|$ 本质上可积。第 10 号提案的断言 b)，然后立即扩展采取复杂措施。

### 4. 性质本质上积分特殊

下面的结果将在后续中经常使用。在叙述中，一个不能替换由普通上积分得到的必要上积分（见例 4）。

#### 命题 11 {#int-v-s1-prop-11 .statement tag=0907}

— 令 $(\lambda_\alpha)_{\alpha \in A}$ 为 T 上的一系列正测度，针对关系 $\leq$，并在 $\mathscr{M}(T)$ 中具有至高$\lambda$。然后，对于每个数字函数 $f \geq 0$，

$$
\lambda^\bullet(f) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

当$f$属于到$\mathscr{K}(T)$时，$\mathscr{M}(T)$中有向集合的上等的关系约化到定义（II, §2, No. 2，引理）。接下来假设$f \leq g$对于某些函数$g \in \mathscr{K}_+$（在其他字中，$f$是有界的并且是零在紧集K之外）；令$\alpha$为指标，使得$\lambda_\alpha(g) \geq \lambda(g) - \varepsilon$，其中$\varepsilon$为数$> 0$；由于测量 $\nu = \lambda - \lambda_\alpha$ 是正数，因此我们有 $\nu^*(f) \leq \nu(g) \leq \varepsilon$ 或 $\lambda_\alpha^*(f) \geq \lambda^*(f) - \varepsilon$（第 IV, §1, No. 3 章，第 15 条命题）。由此可见（因为 $\varepsilon$ 是任意的）（5）的第二个成员是第一个成员 $\geq$；反之不等式是显而易见的，(5)是针对所考虑的特殊情况而成立的。接下来，假设$f$是K之外的零，但不一定有界，并且对于每个整数$n$，集合$f_n = \inf(f, n)$。然后

$$
\lambda^\bullet(f) = \sup_{n \in \mathbf{N}} \lambda^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \sup_{n \in \mathbf{N}} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

最后，在$f$上没有生成限制，用$T$的紧凑子集的$\mathscr{K}$集合表示，我们有
$$
\lambda^\bullet(f) = \sup_{K \in \mathscr{K}} \lambda^\bullet(f \varphi_K) = \sup_{K \in \mathscr{K}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f \varphi_K)
$$
$$
= \sup_{\alpha \in A} \sup_{K \in \mathscr{K}} \lambda_\alpha^\bullet(f \varphi_K) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

#### 推论 1 {#int-v-s1-prop-11-cor-1 .statement tag=0908}

*为了使 T 的子集 N 局部 $\lambda$ 可以忽略不计，对于每个 $\alpha \in A$，N 局部 $\lambda_\alpha$ 可以忽略是充分必要的。*

#### 推论 2 {#int-v-s1-prop-11-cor-2 .statement tag=0909}

*为了使 T 的映射 g 成为拓扑空间 G $\lambda$ 可测，它对于每个 $\alpha \in A$ $\lambda_\alpha$ 可测是充分必要的。*

条件显然是必要的，因为每个 $\alpha$ 都有 $\lambda_\alpha \leq \lambda$（第 IV, §1, No. 3 章，提案 15）。相反，假设$g$对于所有$\alpha$来说是$\lambda_\alpha$可测的，用T的紧致子集K的$\mathscr{K}$集合表示，使得$g|K$是连续的，并令L为紧集，使得$L \cap K$ 是 $\lambda$——对于每个 $K \in \mathscr{K}$ 来说，可以忽略不计。由于集合$\mathscr{K}$是$\lambda_\alpha$密集，L对于每个$\alpha$来说$\lambda_\alpha$可以忽略不计（第IV, §5, No. 8，第12章），因此$\lambda$可以忽略不计（Cor.1）。由此可知 $\mathscr{K}$ 是 $\lambda$ 稠密的，而 $g$ 是 $\lambda$ 可测的（第 IV, §5, No. 10 章，第 15 条命题）。

### 习题{#int-v-s1-exercises}

§ 1](exercises/s1/)参见[习题。
