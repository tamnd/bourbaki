---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 8
section_title: Products of measures
lang: zh
source: int-i-vi
book_pages: INT V.114-INT V.122
pdf_pages: 0334-0349, 0369-0377
extraction: ocr
subsections:
    - "no": 1
      title: Interpretation of the product measure as an integral of measures
      page: 79
      pdf_page: 334
    - "no": 2
      title: Functions measurable with respect to a product of two measures
      page: 81
      pdf_page: 336
    - "no": 3
      title: Integration of positive functions
      page: 83
      pdf_page: 338
    - "no": 4
      title: Integration of functions with values in a Banach space
      page: 87
      pdf_page: 342
    - "no": 5
      title: Operations on the product of two measures
      page: 89
      pdf_page: 344
    - "no": 6
      title: Integration with respect to a finite product of measures
      page: 91
      pdf_page: 346
    - "no": 7
      title: 'Application: Measure of the Euclidean ball in $\mathbf{R}^n$'
      page: 93
      pdf_page: 348
statements: 31
exercises: 21
content_sha256: f7f892266db82026deb02c389c56ed3c0958a563c614994b9879ebb425ca5186
translated_from: content/en/int/V/08_s8_products_of_measures.md
translation_method: google
source_content_sha256: 80b705b3f9f0e254836af8cc36405c37a16c85755c16c07cdd40f1fdbc7ea3e4
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 891ef951d6a1cbcf8179860ea5bc0cb857a7930cc80dc3d7e072854f45fb6d65
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 8。 乘积措施

### 1. 将乘积措施解释为措施的整体

在整个截面中，T 和 T' 表示两个局部紧凑空间，$\mu$ T 上的正测度，$\mu'$ T' 上的正测度，$\nu = \mu \otimes \mu'$ 乘积 $X = T \times T'$ 上的测度（第 III, §4, No. 1 章）。

对于每个$t \in T$，T'到X的映射$t' \mapsto (t, t')$是连续且正确的。令$\lambda'_t$在此映射下为$\mu'$的像； $\lambda'_t$是X的正测度，如果$f \in \mathscr{K}(X)$那么，用$f_t$表示部分映射$t' \mapsto f(t, t')$，我们有

$$
\int f \, d\lambda'_t = \int f_t \, d\mu',
$$

也可以用关系$\lambda'_t = \varepsilon_t \otimes \mu'$来表示。

此外，映射$t \mapsto \lambda'_t(f)$是连续的，具有紧凑的支持（第III, §4, No. 1，引理2），因此T到$\mathscr{M}(X)$的映射$t \mapsto \lambda'_t$是模糊连续的（并且，*更不必说*，模糊$\mu$-可测量）；因而，措施族$t \mapsto \lambda'_t$是$\mu$-充分的（$§ 3$，No. 1，提案2a））。 $f$相对于测量$\int \lambda'_t \, d\mu(t)$的积分是定义

$$
\int \langle f, \lambda'_t \rangle \, d\mu(t) = \int d\mu(t) \int f_t(t') \, d\mu'(t') = \int f(t, t') \, d\nu(t, t')
$$

（第 III, §4, No. 1，第 2 章）；因而$\nu = \int \lambda'_t \, d\mu(t)$。

类似地，对于每个元素$t' \in T'$，令$\lambda_{t'}$为T的映射$t \mapsto (t, t')$下的$\mu$的像到X。 映射$t' \mapsto \lambda_{t'}$是$\mu'$-足够且模糊连续的，以及$\nu = \int \lambda_{t'} \, d\mu'(t')$。我们需要以下引理：

#### 引理 1 {#int-v-s8-lem-1 .statement tag=096Y}

*对于 X 上定义的每个数字函数 $f \geqslant 0$，*

$$
\int^* f_t \, d\mu' = \int^* f \, d\lambda'_t.
$$

由于 $t' \mapsto (t, t')$ 是连续且正确的映射，因此可以从 §4, No. 2 的命题 2 得出。

#### 引理 2 {#int-v-s8-lem-2 .statement tag=096Z}

设$f$为$X$的映射，形成拓扑空间。为了使 $f$ $\lambda'_t$ 可测，$f_t$ $\mu'$ 可测是充分必要的。
这是§6, No. 2第3号提案的推论。

#### 引理 3 {#int-v-s8-lem-3 .statement tag=0970}

令$f$为$X$上定义的函数，值在$\overline{\mathbf{R}}$或Banach空间中。对于 $f$ $\lambda'_t$ 可积，$f_t$ $\mu'$ 可积是必要且充分的，在这种情况下

$$
\int f_t \, d\mu' = \int f \, d\lambda'_t .
$$

这是从 Th 得出的。 §4, No. 4的2，考虑到$t' \mapsto (t, t')$是连续且正确的。

#### 注 {#int-v-s8-n1-rem-1 .statement tag=0971}

引理 1,2,3 可以通过直接论证非常简单地证明，而无需使用 §§4 和 6 的结果。对于例，如果$f \in \mathscr{K}(T \times T')$，则关系 (2) 由定义是明显的。如果$f$在$X = T \times T'$上是下半连续，则足以观察到$t' \mapsto f_t(t')$是函数$t' \mapsto g_t(t') = g(t, t')$的上包络，其中$g$在$\mathscr{K}(X)$中超过函数的集合，使得$0 \leq g \leq f$。最后，对于任意$f$，有一个注，如果$h \geq f$在$X$上是下半连续，那么$t' \mapsto h(t, t')$在$T'$上是下半连续；反之，如果 $t' \mapsto u(t')$ 在 $T'$ 上是下半连续，且对于所有 $t' \in T'$ 都具有 $u(t') \geq f(t, t')$，则函数 $h$ 使得 $h(t, t') = u(t')$、$h(t_1, t') = +\infty$ 对于 $t_1 \neq t'$ 是下半连续$X$且满足$h \geq f$。一旦证明了引理 1，就可以从中推出集合 $(T - \{t\}) \times T'$ $\lambda'_t$可以忽略不计，然后很容易证明引理 2和3。

关系 (3) 允许用 $\int f(t, t') \, d\mu'(t')$ 表示其两个成员，而不存在混淆的风险。类似的结果显然适用于措施$\lambda_{t'} = \mu \otimes \varepsilon_{t'}$。

而不是记号

$$
\int^* f(t, t') \, d\nu(t, t'), \quad \int^\bullet f(t, t') \, d\nu(t, t'), \quad \int f(t, t') \, d\nu(t, t'),
$$

我们将雇用记号

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t'), \quad \iint^\bullet f(t, t') \, d\mu(t) \, d\mu'(t'), \quad \iint f(t, t') \, d\mu(t) \, d\mu'(t'),
$$

与第 1 章中采用的记号一致。 III, §4, No. 1。

将措施$\nu$解释为积分$\int \lambda'_t \, d\mu(t)$将使我们能够将§3的结果翻译成乘积措施的语言。另一方面，度量$\lambda'_t$由$\{t\} \times T' = \overline{\mathrm{pr}}_1^{-1}(t)$承载，因此将$\nu$的定义分解积分为切片，相对于$T \times T'$的投影$\mathrm{pr}_1$到$T$（§6, No. 6）。 之前给出了如此获得的结果的列表，这里是一个有用的性质：

#### 命题 1 {#int-v-s8-prop-1 .statement tag=0972}

— 令$(\mu_\alpha)_{\alpha \in A}$（或$(\mu'_\beta)_{\beta \in B}$）为T（或T'）上的正测度的可求和族，其中和表示为$\mu$（或$\mu'$）。然后，族 $(\mu_\alpha \otimes \mu'_\beta)_{(\alpha, \beta) \in A \times B}$ 可在 $T \times T'$ 上求和，并且

$$
\mu \times \mu' = \sum_{(\alpha, \beta) \in A \times B} \mu_\alpha \otimes \mu'_\beta.
$$

当 A 和 B 有限时，这些性质是显而易见的。由此可见，如果 A（或 B）的 $A'$（或 $B'$）是有限子集，则

$$
\sum_{(\alpha, \beta) \in A' \times B'} \mu_\alpha \otimes \mu'_\beta \leq \mu \otimes \mu'.
$$

因此，族$(\mu_\alpha \otimes \mu'_\beta)$是可求和的。为了证明（4）的两个成员相等，只需证明第二个成员满足乘积措施（Ch.III, §4, No. 1，Th.1）的特征性质即可，这由以下计算得出。

令$f$为$\mathscr{K}_+(T)$的元素，$\mathscr{K}_+(T')$的$f'$元素；回想一下，$f \otimes f'$表示$T \times T'$上的函数$(t, t') \mapsto f(t)f'(t')$，其中属于到$\mathscr{K}_+(T \times T')$（A，II, §7, No. 7）。然后，通过乘积措施中的定义，

$$
\sum_{(\alpha, \beta) \in A \times B} \langle \mu_\alpha \otimes \mu'_\beta, f \otimes f' \rangle = \sum_{(\alpha, \beta) \in A \times B} (\langle \mu_\alpha, f \rangle \langle \mu'_\beta, f' \rangle)
= \left( \sum_{\alpha \in A} \langle \mu_\alpha, f \rangle \right) \left( \sum_{\beta \in B} \langle \mu'_\beta, f' \rangle \right)
= \langle \mu, f \rangle \langle \mu', f' \rangle
= \langle \mu \otimes \mu', f \otimes f' \rangle.
$$

### 2. 函数可相对于乘积的两个度量进行测量

#### 命题 2 {#int-v-s8-prop-2 .statement tag=0973}

— 令$f$为$T \times T'$上定义的$\nu$可测函数，其中值位于拓扑空间 G中，并令M为$t \in T$的集合，使得映射$t' \mapsto f(t, t')$不是$\mu'$-可测量。

a) 如果 $f$ 对于 $\nu$ 调节的子集的 $T \times T'$ 的补集是常数，则 M $\mu$ 可忽略不计。

b) 如果 $\mu'$ 受到调节，则 M $\mu$ 可忽略不计。

断言 a) 源自§3, No. 2 的命题 4b) 和No. 1 的注。对待b)、$\mu'$为有界测度序列$\mu'_n$和的注（§2, No. 3，命题4）； $f$可以相对于$\mu \otimes \mu'_n \leq \nu$进行测量，并且集合$M$是与测量$\mu'_n$相关的集合$M_n$的并（§ 2, No. 2，命题2）。因此，可以简化为 $\mu'$ 有界的情况，这是从 § 3, No. 2 的命题 4c) 得出的。

这叙述扩展立即转向复杂的措施（第 III, § 4, No. 2 章，第 3 条）。

#### 推论{#int-v-s8-n2-cor-1 .statement tag=0974}

— *令 A 为 $T \times T'$ 的 $\nu$ 可测子集，并令 M 为 $t \in T$ 的集合，使得 A 在 t 时的截面 $A(t)$ 不可测 $\mu'$。*

a) *如果 A 是 $\nu$-调节的，则 M 是 $\mu$-可忽略不计的。*

b) *如果 A 在 $T'$ 上的投影是 $\mu'$ 调节的，则 M 局部 $\mu$ 可以忽略不计。*

断言 a) 紧随命题 2 而来。 To establish b), denote by B a set, the union of a sequence of $\mu'$-integrable open sets in $T'$, that contains the projection of A on $T'$, and denote by $\mu'_1$ the moderated measure $\varphi_B \cdot \mu'$; since A is measurable with respect to $\mu \otimes \mu'_1 \leq \mu \otimes \mu'$, Prop. 2 implies that $A(t)$ is $\mu'_1$-measurable, except for $t$ forming a locally $\mu$-negligible set. 但从$A(t) \subset B$开始，说$A(t)$是$\mu'_1$可测就相当于说$A(t)$是$\mu'$可测（§ 5, No. 3，Prop.4的Cor.）。

#### 命题 3 {#int-v-s8-prop-3 .statement tag=0975}

— *设 f 是 T 的映射到拓扑空间 F。如果 f 是 $\mu$ 可测，则映射 $(t, t') \mapsto f(t)$ 是 $\nu$ 可测。相反，如果$\mu' \neq 0$，并且如果这个映射是$\nu$可测的，那么函数 f是$\mu$可测的。*

第一个断言来自Cor。 § 6, No. 6 第 10 号提案 1。假设 $\mu' \neq 0$，由 $\mu'_1$ 非零的表示具有紧支撑的测度，其上方由 $\mu'$ 界定，由 $\nu_1$ 表示测度 $\mu \otimes \mu'_1$，以及集合 $a = \| \mu'_1 \|$。 $T \times T'$ 到 T 的投影 $\mathrm{pr}_1$ 则为 $\nu_1$-本征，像测度 $\mathrm{pr}_1(\nu_1)$ 等于 $a \mu$（§ 6, No. 6，命题 10）。如果$(t, t') \mapsto f(t)$是$\nu$可测的，那么它也是$\nu_1$可测的，因此$f$相对于测度$a \mu$是可测的（§ 6, No. 2，命题3），从而是自$a \neq 0$以来的结果。

前面的叙述扩展立即到复杂的测量（第 III, § 4, No. 2 章，第 3 条），下面的推论也是如此。

#### 推论 1 {#int-v-s8-prop-3-cor-1 .statement tag=0976}

— *设 F、F' 和 G 为三个拓扑空间，并设 u 为 $F \times F'$ 到 G 中的连续映射。设 f（分别为 $f'$）为函数，在 T（分别为 $T'$）上定义，值在 F（分别为 $F'$）中定义，并且可测量$\mu$（或$\mu'$）。那么函数 $(t, t') \mapsto u(f(t), f'(t'))$ 可测量 $\mu \otimes \mu'$。*

映射 $(t, t') \mapsto f(t)$，$(t, t') \mapsto f'(t')$ 是 $\nu$ - 可通过命题 3 测量，这是从 Th 得出的。第 1 章。 IV, § 5, No. 3。

#### 推论 2 {#int-v-s8-prop-3-cor-2 .statement tag=0977}

— *如果 $A \subset T$ 和 $A' \subset T'$ 可测量（分别对于 $\mu$ 和 $\mu'$），则 $A \times A'$ 对于 $\mu \otimes \mu'$ 可测量。*
这是从 Cor 立即得出的结论。 1.

#### 推论 3 {#int-v-s8-prop-3-cor-3 .statement tag=0978}

— *考虑在 $T$ 上定义的两个正数值（分别为复数值）函数 $f$ 和在$T'$ 上定义的$f'$。如果这些函数分别可测量 $\mu$ 和 $\mu'$，则函数*

$$
f \otimes f' : (t, t') \mapsto f(t)f'(t')
$$

*可测量$\mu \otimes \mu'$。*

复数函数或有限实数函数的情况是 Cor 的直接的推论。 1. 处理正数函数的情况，对于每个整数$n \geqslant 0$，我们集合$f_n = \inf(f, n)$，$f'_n = \inf(f', n)$，我们有（按照通常的约定$0 \cdot (+\infty) = 0$）$f \otimes f' = \sup_n (f_n \otimes f'_n)$，从而结果。

#### 命题 4 {#int-v-s8-prop-4 .statement tag=0979}

— *令$A$为$T$的子集。如果$A$局部$\mu$可忽略，则$A \times T'$局部$\nu$可忽略。相反，如果 $A \times T'$ 局部 $\nu$ 可忽略不计，并且如果 $\mu' \neq 0$，则 $A$ 局部 $\mu$ 可忽略。*

第一个断言源自 Cor。 §6, No. 6 第 10 号提案 1。为了建立第二个断言，让我们再次讨论命题3的证明中的记号； $A \times T' = \mathrm{pr}_1^{-1}(A)$ 对于测量 $\nu_1$ 来说是局部可忽略的，因此 $A$ 对于 $a\mu$ 来说是局部可以忽略不计的（§ 6, No. 2，第 2 条命题），从而自 $a \neq 0$ 以来的结果。

前面的叙述扩展立即到乘积两个复杂的措施（第 III, §4, No. 2，第 3 章），以下推论也是如此。

#### 推论{#int-v-s8-n2-cor-2 .statement tag=097A}

— *如果措施$\mu$（或$\mu'$）集中于$M$（或$M'$），则$\mu \otimes \mu'$集中于$M \times M'$。*

因为，$(T \times T') - (M \times M')$是集合、$(T - M) \times T'$和$T \times (T' - M')$的并，根据命题4，$\mu \times \mu'$在局部可以忽略不计。

### 3.整合积极函数

回想一下，我们已经同意定义乘积 $0 \cdot (+\infty)$ 等于 0。该约定特别具有以下推论：如果 $f$ 是一个数字函数 $\geqslant 0$ 定义在配备有正测度的局部紧凑空间上$\lambda$，然后对于每个常数 $a$ $\lambda^*(af) = a \cdot \lambda^*(f)$，使得 $0 \leqslant a \leqslant +\infty$。如果$a = 0$，这是显而易见的；如果$a = +\infty$，则$\lambda^*(af) = a \cdot \lambda^*(f) = 0$或$\lambda^*(af) = a \cdot \lambda^*(f) = +\infty$根据$f$是$\lambda$-可忽略或不可忽略；最后，如果$0 < a < +\infty$，就知道$\lambda^*(af) = a \cdot \lambda^*(f)$。

#### 命题 5 {#int-v-s8-prop-5 .statement tag=097B}

— 令 $f$ 为数值函数 $\geqslant 0$，在 $T \times T'$ 上下半连续。然后，函数

$$
t \mapsto \int^* f(t, t') \, d\mu'(t')
$$

在 $T$ 上是下半连续的，并且

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') \, d\mu'(t').
$$

这是§3, No. 1第2号提案的推论，考虑到No. 1的引理1。

#### 推论 1 {#int-v-s8-prop-5-cor-1 .statement tag=097C}

— 令$f$（或$f'$）为在$T$（或$T'$）上定义的下半连续函数$\geqslant 0$；那么函数$f \otimes f' : (t, t') \mapsto f(t)f'(t')$是$T \times T'$上的下半连续，并且

$$
\iint^* f(t)f'(t') \, d\mu(t) \, d\mu'(t') = \left( \int^* f(t) \, d\mu(t) \right) \left( \int^* f'(t') \, d\mu'(t') \right).
$$

令$G$（分别$G'$）为函数$g \in \mathscr{K}_+(T)$（分别$g' \in \mathscr{K}_+(T')$）的集合，使得$g \leqslant f$（分别$g' \leqslant f'$）；然后

$$
f \otimes f' = \sup_{g \in G,\ g' \in G'} g \otimes g'.
$$

由于函数$g \otimes g'$属于到$\mathscr{K}_+(T \times T')$，$f \otimes f'$确实是下半连续，并且（6）立即从命题5得出（或者直接通过前面的公式中的极限）。

#### 推论 2 {#int-v-s8-prop-5-cor-2 .statement tag=097D}

— 设$A$为$T$的$\mu$调节的子集，$A'$为$T'$的$\mu'$调节的子集；那么 $A \times A'$ 是 $T \times T'$ 中的 $\nu$ 调节的。

鉴于集合的定义（§1, No. 2，命题5），只要证明$B$是$T$中的可积开集合，并且$B'$是集合中的可积开集合 $T'$，则开集合$B \times B'$可积。这是从 Cor 立即得出的结论。 1.

#### 推论 3 {#int-v-s8-prop-5-cor-3 .statement tag=097E}

— 令$A$为$T$的$\mu$可忽略的子集，令$B'$为$T'$的$\mu'$调节的子集；那么 $A \times B'$ 是 $\nu$-可以忽略不计。

因为，$A \times B'$在局部$\nu$可忽略不计（第4条）和$\nu$可调节（修正2），因此$\nu$可忽略不计（§1, No. 2，修正第7条的修正1）。

科斯。 2和3可以扩展到两个复杂措施的乘积，在应用叙述上扩展到其绝对值（第III, §4, No. 2，第3条）。

#### 命题 6 {#int-v-s8-prop-6 .statement tag=097F}

— 令 $f$ 为在 $T \times T'$ 上定义的数值函数 $\geqslant 0$。然后

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') \geqslant \int^* d\mu(t) \int^* f(t, t') d\mu'(t').
$$

这是根据 §3, No. 2 的第 3 条命题得出的，考虑到了 (2)。

#### 命题 7 {#int-v-s8-prop-7 .statement tag=097G}

— 令 $f$ 为定义在 $T \times T'$ 上的 $\nu$ 可测量正数值函数。

a) *如果 $f$ 是 $\nu$ 调节的，则函数* $t \mapsto \int^* f(t, t') d\mu'(t')$、$t' \mapsto \int^* f(t, t') d\mu(t)$ *可分别针对 $\mu$ 和 $\mu'$ 进行测量和调节，并且*

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'(t')
$$
(7)
$$
= \int^* d\mu'(t') \int^* f(t, t') d\mu(t).
$$

b) *如果措施 $\mu'$ 得到调节，则函数* $t \mapsto \int^* f(t, t') d\mu'(t')$ *是 $\mu$ 可测量的，并且*

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'(t').
$$
(8)

断言 a) 以及 $\mu'$ 有界时的断言 b) 是 §3, No. 2 命题 5 的推论。为了处理$\mu'$受到调节的情况，让我们将$\mu'$表示为有界测度序列的和$\sum_{n \in \mathbf{N}} \mu'_n$（§ 2, No. 3，命题4）。 函数 $t \mapsto \int^* f(t, t') d\mu'_n(t')$ 则 $\mu$ 可测量，并且
$$
\iint^* f(t, t') d\mu(t) d\mu'_n(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'_n(t').
$$
但是$\mu \otimes \mu' = \sum_{n \in \mathbf{N}} (\mu \otimes \mu'_n)$（命题1）；然后通过对 $n$（§ 2, No. 2，命题 1）求和获得断言 b)。

#### 推论 1 {#int-v-s8-prop-7-cor-1 .statement tag=097H}

— 令$H$为$T \times T'$的子集，并令$A$为$t \in T$的集合，使得$t$处$H$的截面$H(t)$不是$\mu'$可忽略不计。

a) *如果 $H$ 是 $\nu$ - 可以忽略不计，则 $A$ 是 $\mu$ - 可以忽略不计。*

b) *如果$H$局部$\nu$可忽略不计且$\mu'$受到调节，则$A$局部$\mu$可忽略不计。*

性质 a) 立即来自第 7 号提案（或第 6 号提案）。在b)的假设下，说$H(t)$是局部μ′-可忽略的或者它是μ′-可忽略的，因为μ′是调节的（§1, No. 2，命题7）。因此性质 b) 由公式 (8) 得出。

这个推论立即扩展，通过两个复杂措施的绝对值，到乘积。对于以下推论也是如此：

#### 推论 2 {#int-v-s8-prop-7-cor-2 .statement tag=097I}

— *如果集合* $A \subset T \times T'$ * 是 ν 可积的，则截面* $A(t)$ *of* $A$ *在* $t$ *对于几乎所有* $t \in T$、*函数* $t \mapsto \mu'(A(t))$ * 都是 μ′ 可积μ 可积，并且*

$$
\nu(A) = \int \mu'(A(t))\, d\mu(t).
$$

#### 命题 8 {#int-v-s8-prop-8 .statement tag=097J}

— *对于每个对的数值函数* $f \geq 0$、$f' \geq 0$ *分别定义在* $T$ *和* $T'$，*上，

$$
\iint^\bullet f(t)f'(t')\, d\mu(t)\, d\mu'(t') = \left( \int^\bullet f(t)\, d\mu(t) \right) \left( \int^\bullet f'(t')\, d\mu'(t') \right).
$$

我们首先处理$\mu$和$\mu'$是*具有紧凑支持*的措施； $\mu \otimes \mu'$也是如此，所有符号$\int^\bullet$、$\iint^\bullet$都可以用上积分代替。根据第 6 号提案，

$$
\iint^* f(t)f'(t')\, d\mu(t)\, d\mu'(t') \geq \int^* d\mu(t) \int^* f(t)f'(t')\, d\mu'(t')
$$
$$
= \left( \int^* f(t)\, d\mu(t) \right) \left( \int^* f'(t')\, d\mu'(t') \right).
$$

为了建立反向不等式，让我们选择函数$h \geq f$（分别$h' \geq f'$），即下半连续函数的序列$(h_n)$（分别$(h'_n)$）的下包络线，这样

$$
\int^* h(t)\, d\mu(t) = \int^* f(t)\, d\mu(t)
$$

（分别$\int^* h'(t')\, d\mu'(t') = \int^* f'(t')\, d\mu'(t')$）；这种函数的存在紧随上积分（第IV, §1, No. 3，定义3）的定义和勒贝格的定理而来。 应用提案 7 对于可测量的函数 $h \otimes h'$，我们有

$$
\iint^* f(t)f'(t')\, d\mu(t)\, d\mu'(t') \leq \iint^* h(t)h'(t')\, d\mu(t)\, d\mu'(t')
$$
$$
= \left( \int^* h(t)\, d\mu(t) \right) \left( \int^* h'(t')\, d\mu'(t') \right)
$$
$$
= \left( \int^* f(t)\, d\mu(t) \right) \left( \int^* f'(t')\, d\mu'(t') \right),
$$

这就是人们所寻求的不等式。因此，当$\mu$和$\mu'$是具有紧支撑的测度时，命题成立。为了处理一般情况，只需将$\mu$（或$\mu'$）表示为具有紧凑支持的测度系列$(\mu_\alpha)_{\alpha \in A}$（或$(\mu'_\beta)_{\beta \in B}$）的和（§ 2, No. 3，命题4），为每个测度写入公式（10） $\mu_\alpha \otimes \mu'_\beta$，以及 $(\alpha, \beta)$ 上的和，考虑到提案 1（§ 2, No. 2，提案 1）。

#### 推论 1 {#int-v-s8-prop-8-cor-1 .statement tag=097K}

*使用第 8 条中的记号，

$$
\iint^* f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int^* f(t)\,d\mu(t) \right) \left( \int^* f'(t')\,d\mu'(t') \right)
$$

除非第二个成员的因子之一等于0而另一个等于$+\infty$。

当第二个成员的两个因子有限时，函数$f$和$f'$受到调节（§ 1, No. 2，提案7），因此函数$f \otimes f'$受到调节（提案5的Cor.2）；上述等式因此约化至公式 (10)（§ 1, No. 2，提案 7）。当第二个成员的因子之一具有值$+\infty$而另一个不是零时，则第二个成员具有值$+\infty$，则上述等式由命题6得出。

#### 推论 2 {#int-v-s8-prop-8-cor-2 .statement tag=097L}

*设$f$和$f'$是两个函数，其中值在$\mathbf{C}$或$\overline{\mathbf{R}}$中，分别定义在$T$和$T'$上，并且对于测度$\mu$和$\mu'$来说本质上可积（或可积），分别。 函数 $f \otimes f'$ 对于测度 $\mu \otimes \mu'$ 来说本质上是可积的（或可积的），并且*

$$
\iint f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int f(t)\,d\mu(t) \right) \left( \int f'(t')\,d\mu'(t') \right).
$$

当$f$和$f'$为正时，$f \otimes f'$可以通过Cor来测量。命题 3 的第 3 条和叙述源自公式 (10)（分别为 (11)）和基本可积性准则（§ 1, No. 3，命题 9）（分别为第 IV, § 5, No. 6、第 5 章的可积性准则）。接下来是一般情况。

推论 2 扩展一次到乘积两个复杂的措施。

### 4. 将函数与值整合到 Banach 空间中

#### 定理 1（勒贝格-富比尼）{#int-v-s8-thm-1 .statement tag=097M}

— *令 $f$ 为 $T \times T'$ 上定义的函数，其中值在 Banach 空间 $F$ 或$\overline{\mathbf{R}}$ 中；令$N$为$t \in T$的集合，使得函数$t' \mapsto f(t,t')$不可积$\mu'$。

a) 假设$f$是$\nu$可积；那么$N$是$\mu$可忽略不计，函数$t \mapsto \int f(t,t')\,d\mu'(t')$（为$t \notin N$定义）是$\mu$可积，并且*

$$
\iint f(t,t')\,d\mu(t)\,d\mu'(t') = \int d\mu(t) \int f(t,t')\,d\mu'(t').
$$

b) *假设$f$本质上是$\nu$可积，并且测度$\mu'$经过调节；那么$N$在局部$\mu$可忽略不计，函数$t \mapsto \int f(t, t')\, d\mu'(t')$（为$t \notin N$定义）本质上是$\mu$可积，并且（13）成立。*

断言 a) 立即从 Th 开始。 §3, No. 3 中的 1 个。为了建立 b)，让我们用 $g$ 表示几乎在任何地方都等于 $f$ 的 $\nu$ 可积函数，并用 $(t, t')$ 的 $H$ 集合表示，使得 $f(t, t') \neq g(t, t')$。由科.第 7 条命题 1 中，截面 $H(t)$ $\mu'$ 可忽略不计，除了 $t \in T$ 形成局部 $\mu$ 可忽略不计的集合。然后，可以从应用于 $g$ 的叙述 a) 推导出与 $f$ 相关的结果。

#### 学院{#int-v-s8-n4-sch-1 .statement tag=097N}

— *令$f$为$T \times T'$上定义的函数，值在$\overline{\mathbf{R}}$或Banach空间中，即$\nu$可测量且$\nu$可调节。对于三个积分*

$$
\iint f(t, t')\, d\mu(t)\, d\mu'(t'), \quad \int d\mu(t) \int f(t, t')\, d\mu'(t'), \quad \int d\mu'(t') \int f(t, t')\, d\mu(t)
$$

*要存在且平等，两个数之一是必要且充分的*

$$
\int^* d\mu(t) \int^* |f(t, t')|\, d\mu'(t'), \quad \int^* d\mu'(t') \int^* |f(t, t')|\, d\mu(t)
$$

*是有限的。*

这是Th的直接的推论。 1，第 7 条命题和可积性准则（第 IV, §5, No. 6 章，第 5 章）。

#### 注 {#int-v-s8-n4-rem-1 .statement tag=097O}

— 1) 当测度$\mu'$未经调节时，对于$t \in T$的任何值，可能会发生$f$本质上是$\nu$可积，而函数$t' \mapsto f(t, t')$本质上不是$\mu'$可积（§3，Exer.4）。

2) 令$\mu$和$\mu'$为两个复测度，并令$\nu = \mu \otimes \mu'$。如果$f$是$\nu$可积（在其他字，$|\nu|$可积），则将定理应用于措施$|\mu|$和$|\mu'|$，其乘积是$|\nu|$（第III, §4, No. 2，道具。 3)，意味着$t' \mapsto f(t, t')$是$\mu'$——对于$\mu$可积——几乎每一个$t$。由此推断，将措施$\mu$和$\mu'$分解为积极措施的线性组合，将a)扩展的叙述分解为复杂措施。人们可以对 b) 进行类似的论证。

#### 命题 9 {#int-v-s8-prop-9 .statement tag=097P}

*令$F$、$F'$和$G$为三个Banach空间，并令$(x, y) \mapsto [x \cdot y]$为$F \times F'$到$G$的连续双线性映射。 令$f$（或$f'$）是在$T$（或$T'$）上定义的函数，其中值在$F$（或$F'$）中定义，并且对于$\mu$（或$\mu'$）本质上可积。 设$g$为函数$(t, t') \mapsto [f(t) \cdot f'(t')]$；那么 $g$ 本质上可积为 $\mu \otimes \mu'$，并且*

$$
\iint [f(t) \cdot f'(t')] \, d\mu(t)\, d\mu'(t') = \left[ \left( \int f\, d\mu(t) \right) \cdot \left( \int f'(t')\, d\mu'(t') \right) \right].
$$

*此外，如果 $f$ 和 $f'$ 可积，则 $g$ 可积。*

函数 $(t, t') \mapsto [\mathbf{f}(t) \cdot \mathbf{f}'(t')]$ 是 $(\mu \otimes \mu')$ - 可通过 Cor 测量。命题 3 的 1. 另一方面，如果 $b$ 表示双线性映射 $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x} \cdot \mathbf{y}]$ 的范数，则

$$
\iint^\bullet |[\mathbf{f}(t) \cdot \mathbf{f}'(t')]| d\mu(t) d\mu'(t') \leq b \iint^\bullet |\mathbf{f}(t)| \cdot |\mathbf{f}'(t')| d\mu(t) d\mu'(t')
$$
$$
= b \left( \int^\bullet |\mathbf{f}(t)| d\mu(t) \right) \left( \int^\bullet |\mathbf{f}'(t')| d\mu'(t') \right)
$$

根据命题 8。这表明 $[\mathbf{f}(t) \cdot \mathbf{f}'(t')]$ 对于 $\mu \otimes \mu'$ 本质上是可积的（§ 1, No. 3，命题 9）。假设 $\mathbf{f}$ 和 $\mathbf{f}'$ 是可积的：那么 $\mathbf{f}$ 和 $\mathbf{f}'$ 是有调节的，并且 $\mathbf{g}$ 是有调节的（第 5 条的 Cor. 2），因此是可积的（§ 1, No. 3，第 9 条的 Cor.）。在这种情况下，公式 (14) 由 Lebesgue–Fubini 定理和积分的线性度得出（Ch. IV, § 4, No. 2，Th. 1）。为了完成对$\mathbf{f}$和$\mathbf{f}'$本质上可积的情况的处理，然后将（14）应用于两个可积函数$\mathbf{f}_1$和$\mathbf{f}_1'$，几乎处处都等于$\mathbf{f}$和$\mathbf{f}'$，在注意到上，$[\mathbf{f} \cdot \mathbf{f}'] = [\mathbf{f}_1 \cdot \mathbf{f}_1']$几乎处处处处相等$T \times T'$（提案 4）。

这是复杂措施的扩展到乘积的结果。

### 5. 运算共乘积两小节

#### 命题 10 {#int-v-s8-prop-10 .statement tag=097Q}

— 令$g$（或$g'$）为在$T$（或$T'$）上定义的复数函数（或函数，$\overline{\mathbf{R}}$中的值）。
a) 如果$g$（或$g'$）对于$\mu$（或$\mu'$）可局部可积，则函数 $g \otimes g': (t, t') \mapsto g(t)g'(t')$对于$\nu = \mu \otimes \mu'$可局部可积，并且

$$
(g \cdot \mu) \otimes (g' \cdot \mu') = (g \otimes g') \cdot (\mu \otimes \mu').
$$

b) 相反，如果 $g \otimes g'$ 局部 $\nu$ 可积，并且 $g'$ 局部 $\mu'$ 不可忽略，则 $g$ 局部 $\mu$ 可积。

a) 令$K$和$K'$分别为$T$和$T'$的两个紧致子集；科。命题 8 的 2 表明函数 $(t, t') \mapsto g(t)g'(t')\varphi_{K \times K'}(t, t')$ 等于 $(g\varphi_K) \otimes (g'\varphi_{K'})$，是 $\nu$ 可积的。因而，$g \otimes g'$ 是局部$\nu$可积的。然后立即验证（15）的第二个成员是否满足乘积措施的特征性质（Ch.III, § 4, No. 1，Th.1）。

b) 现在假设 $g \otimes g'$ 局部 $\nu$ 可积，并且 $g'$ 局部 $\mu'$ 不可忽略。令 $\mu_1$ 为具有紧凑支持的正测度，使得 $\mu_1 \leq \mu$； $g \otimes g'$是$(\mu_1 \otimes \mu')$可测量的，$t \mapsto g(t)g'(t')$是$\mu_1$可测量的，除了$t'$的值的局部$\mu'$可忽略不计的集合（命题2）。

由于$g'$不是零，$\mu'$几乎无处不在，由此我们推断$g$是$\mu_1$可测，然后$\mu$可测，将$\mu$分解为和一系列具有紧支持的测度（§ 2, No. 3，提案 4 和§ 2, No. 2，提案 2）。建立了这个点后，如有必要，我们可以将$g$和$g'$是$\geqslant 0$的情况，对替换$g$和$g'$按其绝对值进行约化。令$K$为$T$的任意紧致子集，并令$K'$为$T'$的紧致子集，使得$\int g' \varphi_{K'} d\mu' \neq 0$。根据第 8 号提案，

$$
\left( \int^\bullet g \varphi_K d\mu \right) \left( \int^\bullet g' \varphi_{K'} d\mu' \right) = \iiint^\bullet (g \otimes g') \varphi_{K \times K'} d\mu d\mu' < +\infty .
$$

因此，第一个成员的第一个因子是有限的，这完成了证明。

这命题扩展到复杂的措施，感谢第 3 章的提案。 III, § 4, No. 2。

#### 命题 11 {#int-v-s8-prop-11 .statement tag=097R}

*让$\pi$（或$\pi'$）是$T$（或$T'$）的映射成为局部紧凑的空间$T_1$（或$T'_1$）。*

a) *如果$\pi$（或$\pi'$）是$\mu$-本征（或$\mu'$-本征），则映射$\pi \times \pi'$是$(\mu \otimes \mu')$-本征和$(\pi \times \pi')(\mu \otimes \mu') = \pi(\mu) \otimes \pi'(\mu')$。*

b) *相反，如果$\pi \times \pi'$是$(\mu \otimes \mu')$-固有且$\mu' \neq 0$，则$\pi$是$\mu$-固有。*

a) 对于，$\pi \times \pi'$ 是 $(\mu \times \mu')$-可通过 Cor 测量。 No. 2第 3 号提案 1。另一方面，如果$K$（或$K'$）是$T_1$（或$T'_1$）的紧子集，则$\pi^{-1}(K)$和${\pi'}^{-1}(K')$本质上分别对于$\mu$和$\mu'$可积，因此$\pi^{-1}(K) \times {\pi'}^{-1}(K')$是本质上可积 $\mu \otimes \mu'$（Prop. 8 的 Cor. 2）。这证明$\pi \times \pi'$是$(\mu \times \mu')$-正确的。现在让$\mu_1 = \pi(\mu)$，$\mu'_1 = \pi'(\mu')$，$\nu_1 = (\pi \times \pi')(\mu \otimes \mu')$；对于 $f \in \mathscr{K}(T_1)$ 和 $f' \in \mathscr{K}(T'_1)$，我们有

$$
\iint f(\pi(t)) f'(\pi'(t')) d\mu(t) d\mu'(t')
$$
$$
= \left( \int f(\pi(t)) d\mu(t) \right) \left( \int f'(\pi'(t')) d\mu'(t') \right)
$$

（Prop. 8 Cor. 2），证明 $\nu_1 = \mu_1 \otimes \mu'_1$（Ch. III, § 4, No. 1，Th. 1）。

b) 现在假设 $\pi \times \pi'$ 是 $\mu \otimes \mu'$ 真值，$\mu' \neq 0$。令 $\mu_1$ 为具有紧支撑的测度 $\leq \mu$。 函数$\pi \times \pi'$对于$\mu_1 \otimes \mu'$是可测量的，映射$t \mapsto (\pi(t), \pi'(t'))$是$\mu$可测量的，除了$t'$形成局部$\mu'$-可忽略的集合（No. 2，命题2）。由于$\mu' \neq 0$，$\pi$是$\mu_1$可测，最后$\pi$是$\mu$可测

（§2, No. 3，提案 4 和 §2, No. 2，提案 2）。 还需要证明对于每个函数 $f \in \mathscr{K}_+(\mathrm{T}_1)$ 都有 $\mu^\bullet(f \circ \pi) < +\infty$。 如果$\mu$是零，这个性质是显而易见的。 If $\mu$ is not zero, then neither is $\mu \otimes \mu'$, consequently $(\pi \times \pi')(\mu \otimes \mu') \neq 0$ (§6, No. 2, Cor. 1 of Prop. 2). 由 Ch. 引理 1 开始 III, §4, No. 1，存在两个函数$g \in \mathscr{K}_+(\mathrm{T}_1)$，$g' \in \mathscr{K}_+(\mathrm{T}'_1)$使得

$$
\langle (\pi \times \pi')(\mu \otimes \mu'), g \otimes g' \rangle \neq 0.
$$

该表达式等于$\langle \mu \otimes \mu', (g \circ \pi) \otimes (g' \circ \pi') \rangle$乘以像措施的定义，第8条命题意味着${\mu''}^\bullet(g' \circ \pi') \neq 0$。然后，根据 §6, No. 2 的第 8 条命题和第 2 条命题，我们有：

$$
\left( \int^\bullet (f \circ \pi) d\mu \right) \left( \int^\bullet (g' \circ \pi') d\mu' \right) = \iint^\bullet (f \circ \pi) \otimes (g' \circ \pi') d\mu d\mu'
$$
$$
= \iint^\bullet (f \otimes g') d((\pi \times \pi')(\mu \otimes \mu')) < +\infty.
$$

因而，第一个成员中的第一个积分是有限的，完成证明。

两个复杂度量的结果扩展立即变为乘积（将叙述应用于其绝对值值）。下面的命题也是如此。

#### 命题 12 {#int-v-s8-prop-12 .statement tag=097S}

— 令X（或X'）为T（或T'）的局部紧凑子空间。那么，$T \times T'$的局部紧致子空间$X \times X'$上导出的测度$(\mu \otimes \mu')_{X \times X'}$分别等于$\mu$和$\mu'$在X和X'上导出的测度乘积$\mu_X \otimes \mu'_{X'}$。

对于，如果$f \in \mathscr{K}(X)$和$f' \in \mathscr{K}(X')$，那么

$$
\iint_{X \times X'} f(t)f'(t') d\mu(t) d\mu'(t') = \left( \int_X f(t) d\mu(t) \right) \left( \int_{X'} f'(t') d\mu'(t') \right)
$$

由科.第 8 条命题 2，通过诱导措施的定义（第 IV, §5, No. 7 章）证明

$$
(\mu \otimes \mu')_{X \times X'} = \mu_X \otimes \mu'_{X'}
$$

（第 III, §4, No. 1 章，第 1 章）。

### 6. 对有限乘积测度的积分

前面的结果可以毫无困难地扩展到有限数措施中的乘积。对于例，令$T_1, T_2, T_3$为三个局部紧致空间，$\mu_i$为$T_i$（$i = 1, 2, 3$）的正测度，并令ν = μ₁⊗μ2⊗μ₃为乘积在T = T₁×T2×T₃上的测度。令 f 为 ν 可积函数，其中 $\overline{\mathbf{R}}$ 或 Banach 空间中的值； Lebesgue–Fubini 定理的首次应用表明，除了在点 $(t_1, t_2) \in T_1 \times T_2$ 处形成可忽略不计的集合（对于 $\mu_1 \otimes \mu_2$），函数 $t_3 \mapsto f(t_1, t_2, t_3)$ 是 $\mu_3$ 可积的，函数

$$
(t_1, t_2) \mapsto \int f(t_1, t_2, t_3) \, d\mu_3(t_3),
$$

几乎在 $T_1 \times T_2$ 中的任何位置都定义，是 $(\mu_1 \otimes \mu_2)$ 可积的，并且

$$
\iiint f(t_1, t_2, t_3) \, d\nu(t_1, t_2, t_3) = \iint d\mu_1(t_1) \, d\mu_2(t_2) \int f(t_1, t_2, t_3) \, d\mu_3(t_3).
$$

相同定理的第二个应用表明，对于几乎每个 $t_1 \in T_1$，函数 $t_2 \mapsto \int f(t_1, t_2, t_3) \, d\mu_3(t_3)$ 几乎在 $T_2$ 中的所有位置都有定义，并且是 $\mu_2$ 可积的；此外，函数

$$
t_1 \mapsto \int d\mu_2(t_2) \int f(t_1, t_2, t_3) \, d\mu_3(t_3),
$$

几乎在 $T_1$ 中的任何位置都定义，是 $\mu_1$ 可积的，并且

$$
\iiint f(t_1, t_2, t_3) \, d\nu(t_1, t_2, t_3) = \int d\mu_1(t_1) \int d\mu_2(t_2) \int f(t_1, t_2, t_3) \, d\mu_3(t_3).
$$

类似地证明，对于几乎每个 $t_1 \in T_1$，函数 $(t_2, t_3) \mapsto f(t_1, t_2, t_3)$ 是 $(\mu_2 \otimes \mu_3)$ 可积，函数

$$
t_1 \mapsto \iint f(t_1, t_2, t_3) \, d\mu_2(t_2) \, d\mu_3(t_3),
$$

几乎处处定义，是$\mu_1$可积，并且

$$
\iiint f(t_1, t_2, t_3) \, d\nu(t_1, t_2, t_3) = \int d\mu_1(t_1) \iint f(t_1, t_2, t_3) \, d\mu_2(t_2) \, d\mu_3(t_3).
$$

我们留给读者以同样的方式概括上面针对两个测量的乘积的其他结果的任务。

### 7. 应用：测量$\mathbf{R}^n$中的欧氏球

令$\mu$为$\mathbf{R}$上的勒贝格测度，$\mu_n$为$\mathbf{R}^n$上的勒贝格测度，$n$因子的乘积等于$\mu$。我们向计算提出欧氏单位球的措施$V_n = \mu_n(\mathbf{B}_n)$。由科.第 7 号提案第 2 条，

$$
V_n = \int_{-1}^{+1} \mu_{n-1}(\mathbf{B}_n(z_n)) dz_n .
$$

现在，截面$\mathbf{B}_n(z_n)$是由关系$\sum_{i=1}^{n-1} z_i^2 \leq 1 - z_n^2$定义的$\mathbf{R}^{n-1}$的子集，在其他字中，它是球$\mathbf{B}_{n-1}$的变换乘以位似的比例$\sqrt{1 - z_n^2}$。但它紧随第 11 号提案和公式而来

$$
\alpha \int_{-\infty}^{+\infty} f(\alpha x) dx = \int_{-\infty}^{+\infty} f(z) dz
$$

对于$f \in \mathscr{K}(\mathbf{R})$，位似$\mathbf{x} \mapsto \alpha \mathbf{x}$下的$\mu_{n-1}$的像是$\alpha^{1-n} \mu_{n-1}$。因此

$$
\mu_{n-1}(\mathbf{B}_n(z_n)) = \left( \sqrt{1 - z_n^2} \right)^{n-1} V_{n-1} .
$$

(16) 中的代换，并用变量$z_n = \sin \varphi$（与$-\frac{\pi}{2} \leq \varphi \leq \frac{\pi}{2}$）制作变换，得出

$$
V_n = V_{n-1} \int_{-\frac{\pi}{2}}^{+\frac{\pi}{2}} \cos^n \varphi d\varphi = 2 V_{n-1} \int_0^{\frac{\pi}{2}} \cos^n \varphi d\varphi .
$$

但是（FRV，第 VII, §1, No. 3，公式 (20)）

$$
\int_0^{\frac{\pi}{2}} \cos^m \varphi d\varphi = \frac{1}{2} \frac{\Gamma \left( \frac{1}{2} \right) \Gamma \left( \frac{m+1}{2} \right)}{\Gamma \left( \frac{m+2}{2} \right)}
$$

代入关系 (17) 并考虑$\Gamma \left( \frac{1}{2} \right)$ (FRV, VII, §1, No. 3, 公式 (21)) 的表达式，最终得到

$$
V_n = \frac{\pi^{n/2}}{\Gamma \left( \frac{n}{2} + 1 \right)} .
$$

习题

### 习题{#int-v-s8-exercises}

§ 8](exercises/s8/)参见[习题。
