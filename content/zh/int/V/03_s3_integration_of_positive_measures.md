---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 3
section_title: Integration of positive measures
lang: zh
source: int-i-vi
book_pages: INT V.96-INT V.98
pdf_pages: 0270-0286, 0351-0353
extraction: ocr
subsections:
    - "no": 1
      title: Functions with values in a space of measures
      page: 0
      pdf_page: 270
    - "no": 2
      title: Superimposed integrals of positive functions
      page: 20
      pdf_page: 275
    - "no": 3
      title: Superimposed integrals of functions with values in a Banach space
      page: 24
      pdf_page: 279
    - "no": 4
      title: Universally measurable functions
      page: 25
      pdf_page: 280
    - "no": 5
      title: Diffusions
      page: 26
      pdf_page: 281
    - "no": 6
      title: Composition of bounded diffusions
      page: 29
      pdf_page: 284
statements: 30
exercises: 11
content_sha256: c8806ca9b801b20df35b5fbfaddc146844005a950aa31d3bad240743baa781c2
translated_from: content/en/int/V/03_s3_integration_of_positive_measures.md
translation_method: google
source_content_sha256: 4363fec5ea39b1d12c9673dd8324ba6983ab374b2f5f144cb72fb7d26d6dfd8e
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: dced6682959ef3596947ebf7c25448482fd79eacc96d0f9c54d94566f9e634b1
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。整合积极措施

### 1. 函数与值在空间措施中

令 $X$ 为局部紧致空间，$\mathscr{M}_+(X)$ $X$ 上的正测度凸锥。在章的其余部分中，$\mathscr{M}_+(X)$将配备由$\mathscr{M}(X)$上模糊的拓扑引起的拓扑（第III, §1, No. 9）；因此，说局部紧致空间$T$到$\mathscr{M}_+(X)$的映射$\Lambda : t \mapsto \lambda_t$是连续的意味着，对于每个函数$f \in \mathscr{K}(X)$，数值函数$t \mapsto \lambda_t(f)$是连续的。在这种情况下，我们还可以说$\Lambda$在$T$上是模糊连续的。说映射$\Lambda : t \mapsto \lambda_t$是$\mu$可测意味着$T$的紧凑子集$K$的集合，使得$\Lambda$到$K$的限制模糊连续，是

令$\Lambda : t \mapsto \lambda_t$为T的映射进入$\mathscr{M}_+(X)$；如果对于每个函数 $f \in \mathscr{K}(X)$，函数 $t \mapsto \lambda_t(f)$ 本质上是 μ 可积的，我们可以说 Λ 对于测度 μ 本质上是标量可积的。如果集合 $\nu(f) = \int \lambda_t(f)\, d\mu(t)$，很明显 ν 是 $\mathscr{K}(X)$ 上的正线性形式，因此是 X 上的测度（Ch. III, §1, No. 5，Th. 1）。我们会说ν是函数Λ与值在$\mathscr{M}_+(X)$中的积分，我们会写成$\nu = \int \lambda_t\, d\mu(t)$。

前面的定义是弱积分概念的一个特例，在第1章中会以一般的方式处理。 VI。

如果$f$表示$\mathscr{K}(X)$的一个元素，则积分$\int \lambda_t(f)\, d\mu(t)$也将通过滥用符号表示为$\int d\mu(t) \int f(x)\, d\lambda_t(x)$；整的$\nu = \int \lambda_t\, d\mu(t)$的定义可以写成

$$
\int f(x)\, d\nu(x) = \int d\mu(t) \int f(x)\, d\lambda_t(x).
$$

我们将在续集中对记号进行类似的滥用，对于上积分、本质上积分以及巴纳赫空间中函数与值的积分。

#### 例 1 {#int-v-s3-n1-exa-1 .statement tag=090W}

假设 T 是离散的空间，μ 是通过在 T 的每个点处放置质量 +1 来定义的 T 的度量（Ch. III, §1, No. 3）。设h为T上定义的函数$\geqslant 0$；因为函数 h 在 T 上是下半连续（甚至连续），$\mu^*(h) = \mu^\bullet(h) = \sum_{t \in T} h(t)$（Ch. IV, §1, No. 1，例）。

对于测量 μ，可积函数的概念和可积函数本质上是相同的。既然如此，如果说 T 到 $\mathscr{M}_+(X)$ 的映射 $t \mapsto \lambda_t$ 本质上是 μ 可积的，则等于说，即族 $(\lambda_t)_{t \in T}$ 是可求和的 (§2, No. 1)，然后就有 $\int \lambda_t\, d\mu(t) = \sum_{t \in T} \lambda_t$。请注意，映射 $t \mapsto \lambda_t$ 是模糊连续的。

#### 例 2 {#int-v-s3-n1-exa-2 .statement tag=090X}

T 到 $\mathscr{M}_+(T)$ 的映射 $t \mapsto \varepsilon_t$ 是模糊连续的，对于 T 上的每个正测度 μ 而言，本质上是标量 μ 可积的，并且有 $\int \varepsilon_t\, d\mu(t) = \mu$。

#### 命题 1 {#int-v-s3-prop-1 .statement tag=090Y}

假设μ是T上正测度递增有向族$(\mu_i)_{i \in I}$的至高；在阶中，$\Lambda : t \mapsto \lambda_t$ 本质上是 μ 可标量可积的，对于所有 $i \in I$，Λ 基本上是 $\mu_i$ 标量可积是必要且充分的，并且族 $(\int \lambda_t\, d\mu_i(t))_{i \in I}$ 的边界在 $\mathscr{M}(X)$ 中。那么一个人有，

$$
\int \lambda_t\, d\mu(t) = \sup_{i \in I} \int \lambda_t\, d\mu_i(t).
$$

因为，验证$\Lambda$对于$T$上的正测度$\eta$在标量上本质上可积，归结为验证$t \mapsto \lambda_t(g)$是$\eta$可测的，并且对于每个函数$g \in \mathscr{H}_+(X)$，对于$\eta$，承认有限本质上积分。因此，命题立即源自§1, No. 4的第11条命题及其推论2。

#### 推论 {#int-v-s3-n1-cor-1 .statement tag=090Z}

— *假设 $\mu$ 是 $T$ 上积极措施的可和族 $(\mu_\alpha)_{\alpha \in A}$ 的和；在阶中，$\Lambda : t \mapsto \lambda_t$本质上是$\mu$标量可积，对于每个$\alpha \in A$，$\Lambda$本质上$\mu_\alpha$标量可积是必要且充分的，并且测度族$\int \lambda_t d\mu_\alpha(t)$是可求和的。然后一个有*

$$
\int \lambda_t d\mu(t) = \sum_{\alpha \in A} \int \lambda_t d\mu_\alpha(t).
$$

紧接着，对于每个测度 $\mu' \leq \mu$，每个标量本质上 $\mu$ 可积的映射也是标量本质上 $\mu'$ 可积的。

在这个截面中，我们将极限自己研究$T$的标量本质上可积的映射到$\mathscr{M}_+(X)$，在下面的定义中考虑了性质：

#### 定义 1 {#int-v-s3-def-1 .statement tag=0910}

— *令$X$为局部紧凑空间，$\Lambda : t \mapsto \lambda_t$为$T$的标量本质上$\mu$可积映射到$\mathscr{M}_+(X)$，以及$\nu$$\Lambda$的积分。

我们说$\Lambda$是$\mu$-预充分的，如果对于$X$上定义的每个下半连续函数$f \geq 0$，函数$t \mapsto \int^\bullet f d\lambda_t$是$\mu$-可在$T$上测量并且*

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

*如果$\Lambda$是$\mu'$-对于每个积极措施$\mu' \leq \mu$来说是预充分的，那么我们说$\Lambda$是$\mu$-充分的(*)。*

可以证明，如果$\Lambda$是$\mu$-预充分的，并且如果$\nu = \int \lambda_t d\mu(t)$的测量是适度的——特别是如果$X$在无穷大时可数——那么$\Lambda$是$\mu$-充分的（Exer.7）；然而，尚不清楚这些概念是否大体相同。在下面第 2 条和第 3 条中的叙述中，断言前面加了 a) 或 b) 扩展，以预先充足映射，而前面加 c) 的则仅对充足的映射有效。

(*) 在第一版中，“$\mu$-足够”映射被定义为标量本质上$\mu$可积和模糊的$\mu$-可测量映射。这里给出的定义更为一般（下面的命题2）。

下面的命题通常允许人们验证给定的映射是否足够$\mu$。

#### 命题 2 {#int-v-s3-prop-2 .statement tag=0911}

— 设 $\Lambda : t \mapsto \lambda_t$ 是 $T$ 到 $\mathscr{M}_+(X)$ 的标量本质上 $\mu$ 可积映射，并设 $\nu = \int \lambda_t \, d\mu(t)$。

a) *如果$\Lambda$是模糊连续的，那么映射$t \mapsto \lambda_t^\bullet(f)$对于$X$上定义的每个下半连续函数$f \geqslant 0$来说是下半连续的，$\Lambda$是$\mu$-充分的，并且我们有关系*

$$
\int^* f(x) \, d\nu(x) = \int^* d\mu(t) \int^* f(x) \, d\lambda_t(x).
$$

b) *如果 $\Lambda$ 模糊地 $\mu$ 可测量，则 $\Lambda$ $\mu$ 足够。*

c) *如果 $X$ 的拓扑承认可数基，则 $\Lambda$ 隐约是 $\mu$ 可测量的（因此 $\mu$ 也是足够的）。*

设$f$是定义在$X$上的下半连续函数$\geqslant 0$。设$F$为集合，针对关系$\leqslant$，函数$g \in \mathscr{K}(X)$，使得$0 \leqslant g \leqslant f$。对于$g \in F$，用$h_g$表示，函数在$T$上定义为$h_g(t) = \lambda_t(g)$。同样，集合

$$
h_f(t) = \lambda_t^*(f) = \lambda_t^\bullet(f) = \sup_{g \in F} h_g(t)
$$

（§1, No. 1，提案 4）。让我们制作以下假设，比a)弱：仅假设$\Lambda$到$S$的限制是模糊连续的，其中$S$是$T$的闭子集，包含是$\mu$的支持。对于$g \in F$，用$\overline{h}_g$表示数字函数，重合在$S$上有$h_g$并且在$C_S$上有值$+\infty$。 集合$\overline{h}_f = \sup_{g \in F} \overline{h}_g$；然后$\overline{h}_f = h_f$上$S$。对于每个 $g \in F$，函数 $\overline{h}_g$ 是下半连续；因此$\overline{h}_f$是下半连续的，并且由于族$(\overline{h}_g)_{g \in F}$是有向的，

$$
\mu^*(\overline{h}_f) = \sup_{g \in F} \mu^*(\overline{h}_g) = \sup_{g \in F} \mu^*(h_g) = \sup_{g \in F} \nu(g) = \nu^*(f)
$$

（第 IV, §1, No. 1、第 1 章和§2, No. 3、第 6 条提案）。由于$h_f = \overline{h}_f$在$S$上，因此几乎在任何地方，这也可以写成$\mu^*(h_f) = \nu^*(f)$，等式，与(5)相同。类似地，$f$和$\overline{h}_f$是下半连续的，前面的关系产生等式$\mu^\bullet(\overline{h}_f) = \nu^\bullet(f)$（§1, No. 1，命题4）；由于$\overline{h}_f = h_f$在$S$上，因此$\mu^\bullet(h_f) = \nu^\bullet(f)$（§1, No. 1，命题1），等式与（4）相同。因此映射 $\Lambda$ 是 $\mu$-预充足；但我们可以用$\mu' \leqslant \mu$替换$\mu$，用$\nu' = \int \lambda_t \, d\mu'(t)$替换$\nu$，因为$\Lambda$本质上也是$\mu'$可积的，并且$S$包含是$\mu'$的支持。由此可见，$\Lambda$ $\mu$ 是足够的。

假设$\Lambda$是模糊连续的；我们可以取$S = T$；那么$h_f = \overline{h}_f$是下半连续，它完成了叙述的部分a)的证明。

假设 $\Lambda$ 模糊地 $\mu$ 可测，让我们证明 b)。 T 的紧致子集 K 的集合 $\mathscr{K}$，使得 $\Lambda$ 到 K 的限制是连续的 $\mu$ 稠密（第 IV, §5, No. 10，第 15 章），存在 T 上测度的可和族 $(\mu_\alpha)_{\alpha \in A}$ 使得 $\mu = \sum_{\alpha \in A} \mu_\alpha$以及对$\mu_\alpha$属于至$\mathscr{K}$每项措施的支持（§2, No. 3，提案4）。对于每个 $\alpha \in A$，映射 $\Lambda$ 本质上是 $\mu_\alpha$ 标量可积，并且我们集合 $\nu_\alpha = \int \lambda_t d\mu_\alpha(t)$；族$(\nu_\alpha)$是可求和的，其和等于$\nu$（命题1的Cor.）。如果$f$是在X上定义的正下半连续函数，则将证明的第一个部分应用于度量$\mu_\alpha$和封闭的集合$S_\alpha$，表明：

对于每个 $\alpha \in A$，$1^\circ$ $h_f$ 是 $\mu_\alpha$ 可测量的，因此 $\mu$ 可测量（§2, No. 2，命题 2），并且

$2^\circ$$\int^* f(x) d\nu_\alpha(x) = \int^* d\mu_\alpha(t) \int^* f(x) d\lambda_t(x)$。

公式 (4) 是对$\alpha$（§2, No. 2，命题 1）求和的结果。 应用前面对任意测度$\mu' \leq \mu$的论证（这是合法的，因为$\Lambda$本质上是$\mu'$可积且模糊地$\mu'$可测量，cf.§2, No. 2，命题2），我们结论 $\Lambda$是$\mu'$-预充分，并且b)被证明。

最后，假设 X 的拓扑承认可数基，让我们证明 T 的每个标量本质上 $\mu$ 可积到 $\mathscr{M}_+(X)$ 的映射 $\Lambda : t \mapsto \lambda_t$ 都是模糊地 $\mu$ 可测的。这将由以下引理产生：

#### 引理 {#int-v-s3-n1-lem-1 .statement tag=0912}

*令 X 为具有可数基的局部紧凑空间。那么，在$\mathscr{K}(X)$中存在可数子集 S，具有以下性质：对于每个函数$f \in \mathscr{K}(X)$，存在S的元素的序列$(f_n)$和正函数$\varphi \in S$，使得，对于每个数 $\varepsilon > 0$，$|f_n - f| \leq \varepsilon \varphi$，前提是 n 为足够大。*

令 $X'$ 为 X 的 Alexandroff 紧致化，这是一个可度量的紧致空间（GT、IX, §2, No. 9、Prop. 16 和 Cor.）；我们认同$\mathscr{K}(X)$与子集$\mathscr{C}(X')$。令 $S'$ 为 Banach 空间 $\mathscr{C}(X')$ (GT, X, §3, No. 3, Th. 1) 的可数稠密子集；我们可以假设对于每个 $n \in \mathbf{N}$，$S'$ 包含都是常数函数 $n$。令$(U_n)$为X中相对紧开集合的序列，且并X，使得$\overline{U}_n \subset U_{n+1}$对于所有n（GT，I, §9, No. 9，命题15），并令$\varphi_n$为$\mathscr{K}_+(X)$中的函数等于$\overline{U}_n$中的1。我们用 S 表示形式 $\varphi_n g$ ($n \in \mathbf{N}, g \in S'$) 的$\mathscr{K}(X)$ 元素可数集合。如果$f \in \mathscr{K}(X)$，令$(g_n)$为$S'$的元素的序列一致收敛于$f$，并令k为整数，使得$f$的支持度包含在$U_k$中。最后，令 m 为整数，即范数函数 $g_n$ 的上界。 函数 $f_n = \varphi_k g_n$ 属于至 S 和满足叙述，以及 $\varphi = m \varphi_k$。

引理已成立，并且映射 $t \mapsto \lambda_t(g)$ 对于 T 的每个 $g \in S$、映射 $t \mapsto (\lambda_t(g))_{g \in S}$ 本质上是 $\mu$ 可积为 $\mathbf{R}^S$ 的 $\mu$ 可测（第 IV, §5, No. 3、Th.1）。 T 的紧致子集 K 的集合 $\mathscr{K}$，使得该映射到 K 的限制是连续的，因此是 $\mu$ 稠密的，并且足以证明 $\Lambda$ 到每个 $K \in \mathscr{K}$ 的限制是连续的。现在，令$f$为引理的S满足叙述的$\mathscr{K}(X)$、$f_n$和$\varphi$元素中的任意元素； 函数$t \mapsto \lambda_t(f)$则为连续函数$t \mapsto \lambda_t(f_n)$在K上的一致极限；因此它在 K 上连续，命题得证。

### 2. 正函数的叠加积分

对于截面的其余部分，如果没有明确指出相反的情况，我们将用X表示局部紧凑的空间，用$\Lambda : t \mapsto \lambda_t$将T的$\mu$充分映射表示为$\mathscr{M}_+(X)$，并用$\nu$表示$\Lambda$的积分。

#### 命题 3 {#int-v-s3-prop-3 .statement tag=0913}

— 令 f 为在 X 上定义的数值函数 $\geqslant 0$。
a) 下列不等式成立：

$$
\int^* f(x)\, d\nu(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

b) 如果 $\Lambda$ 是模糊连续的，那么

$$
\int^* f(x)\, d\nu(x) \geqslant \int^* d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

c) 如果$\lambda_t^\bullet(1) < +\infty$局部$\mu$-几乎无处不在，那么

$$
\int^\bullet f(x)\, d\nu(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) = \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

令 g 为 X 上的下半连续函数，使得 $f \leqslant g$。对于每个$t \in T$，

$$
\int^* f(x)\, d\lambda_t(x) \leqslant \int^* g(x)\, d\lambda_t(x),
$$

因此，根据(4)和§1的命题4，

$$
\int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) \leqslant \int^\bullet d\mu(t) \int^* g(x)\, d\lambda_t(x) = \int^* g(x)\, d\nu(x).
$$

然后，第一个不等式 (6) 从 $\int^* f(x)\, d\nu(x)$ 的定义得出（Ch. IV, §1, No. 3，定义 3），第二个不等式立即从它得出。如果$\Lambda$是模糊连续的，则使用（5）而不是（4）来以类似的方式证明不等式（7）。

让我们转到 (8) 的证明。 映射 $t \mapsto \lambda_t^*(1)$ 是可测量的，并且局部有限 $\mu$ - 几乎无处不在。 $T$的紧致子集的集合$\mathscr{K}$，$t \mapsto \lambda_t^*(1)$到$K$的限制是有限且连续的，因此是$\mu$稠密，§2, No. 3的第4条意味着存在一个可和族$(\mu_\alpha)_{\alpha \in A}$积极措施，支持属于到$\mathscr{K}$，这样$\mu = \sum_{\alpha \in A} \mu_\alpha$。 映射 $\Lambda$ 是 $\mu_\alpha$ - 对于每个 $\alpha \in A$ 来说足够了； 集合$\nu_\alpha = \int \lambda_t d\mu_\alpha(t)$。命题 1 表明，将 $\nu = \sum_{\alpha \in A} \nu_\alpha$ 和关系 (4) 应用于测度 $\mu_\alpha$ 和函数 1，表明 $\nu_\alpha$ 是有界测度（因为 $\lambda_t^*(1)$ 在 $\operatorname{Supp}(\mu_\alpha)$ 上有界）。然后让我们将$\mu_\alpha$测度写成公式(6)，替换通过$\int^\bullet$第一个成员中的符号$\int^*$，这根据§1的第7条命题是合法的；然后

$$
\int^\bullet f(x) d\nu_\alpha(x) \geq \int^\bullet d\mu_\alpha(t) \int^* f(x) d\lambda_t(x) = \int^\bullet d\mu_\alpha(t) \int^\bullet f(x) d\lambda_t(x)
$$

（最后一个等式是因为$\lambda_t$几乎在任何地方都有局部有界，以及§ 1的第7条命）。然后通过对$\alpha$求和得到(8)中的不等式（§2, No. 2，命题1）。

如果没有生成类似于 c) 的假设，则不等式 (8) 可能会失败（例 2）。

#### 推论 1 {#int-v-s3-prop-3-cor-1 .statement tag=0914}

— *令$f$为$X$上定义的函数$\geq 0$，并令$H$为$t \in T$的集合，使得$f$不是$\lambda_t$可忽略不计。*
a) *如果 $f$ $\nu$-可忽略，则 $H$ 局部 $\mu$-可忽略。*
b) *如果 $f$ 是 $\nu$-可忽略且 $\Lambda$ 是模糊连续的，则 $H$ 是 $\mu$-可忽略。*
c) *如果 $f$ 局部 $\nu$ 可忽略不计，且 $\lambda_t^\bullet(1) < +\infty$ 局部 $\mu$ 几乎无处不在，则 $H$ 局部 $\mu$ 可忽略不计。*

#### 推论 2 {#int-v-s3-prop-3-cor-2 .statement tag=0915}

— *令$f$为函数$\geq 0$，定义在$X$、$\nu$可测量且$\nu$可调节。 $t \in T$的集合使得$f$不是$\lambda_t$调节，则局部$\mu$可以忽略不计（如果$\Lambda$模糊地连续，甚至$\mu$可以忽略不计）。*

对于，$f$是函数$f_n \geq 0$序列的和，使得$f_n$对于$n \geq 1$来说在紧集$K_n$之外是零，并且$f_0$是$\nu$-可忽略不计（§1, No. 2，第 6 条）；那么$f_0$是$\lambda_t$-可以忽略的，除了$t$形成集合是局部$\mu$-可以忽略的（甚至$\mu$-可以忽略，如果$\Lambda$是模糊连续的）。 1，然后紧接着是叙述。

#### 命题 4 {#int-v-s3-prop-4 .statement tag=0916}

— *令$f$为$X$上定义的$\nu$可测函数，其中值位于拓扑空间$G$中，并令$M$为$t \in T$的集合，使得$f$ 不可测量 $\lambda_t$。*
a) *假设$f$在$\nu$调节的子集对$X$的补集上恒定；那么$M$在本地是$\mu$-可以忽略不计。*

b) *假设 f 在 ν 调节的子集 X 的补集上是常数，并且 Λ 是模糊连续的；那么 M 可以忽略不计。*

c) *假设$\lambda_t^\bullet(1) < +\infty$局部μ-几乎无处不在；那么 M 局部 μ 可以忽略不计。*

让我们首先证明a）（分别b））。由于每个 ν 可积集合都包含在 ν 可积开集合中，因此函数 f 在 ν 可积开集合的可数并的补 B 上是常数。存在由 ν 可忽略的集合 N 和紧集的序列 $(K_n)$ 形成的 X − B 的划分，使得 f 的限制对于每个 $K_n$ 都是连续的。令 S 为集合的集合或 $t \in T$，使得 N $\lambda_t$ 不可忽略：S 通过 Cor 局部可忽略（或可忽略）。命题 3 的 1. 集合 $K_n, B, N$ 对于 X 上的每一个测度都是可测的，而 f 的限制对于每个 $t \notin S$ 都是 $\lambda_t$ 可测的。因此，对于每个 $t \notin S$，函数 f 都是 $\lambda_t$ 可测量的（第 IV, §5, No. 10 章，第 16 条命题）。

为了成立c)，让我们再次讨论命题3的证明中的记号；由于 f 是 ν 可测的，因此它对于每个测度 $\nu_\alpha \leq \nu$ 都是可测的。现在，这些措施是有界的，因此是缓和的，并且从 a) 可以得出，对于每个 $\alpha \in A$，M 是局部$\mu_\alpha$-可忽略不计的。这意味着 M 局部 μ 可以忽略不计（§2, No. 2，命题 1 的 Cor.2）。

#### 命题 5 {#int-v-s3-prop-5 .statement tag=0917}

*设 f 为 X 上定义的 ν 可测量正数值函数，并令 N 为 $t \in T$ 的集合，使得 f 不能同时为 $\lambda_t$ 可测量和 $\lambda_t$ 调节。*

a) *假设 f 是 ν 调节的。 集合 N 局部 μ 可以忽略不计，函数 $t \mapsto \int^\bullet f(x) d\lambda_t(x)$ 是 μ 可测的，并且*

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

b) *假设 f 是 ν 调节的，并且 Λ 是模糊连续的。 集合 N 是 μ 可忽略不计的，函数 $t \mapsto \int^* f(x) d\lambda_t(x)$ 是 μ 可测量和 μ 调节的，并且*

$$
\int^* f(x) d\nu(x) = \int^* d\mu(t) \int^* f(x) d\lambda_t(x).
$$

c) *假设 $\lambda_t^\bullet(1) < +\infty$ 局部 μ-几乎无处不在。 集合 N 局部 μ 可忽略，函数 $t \mapsto \int^\bullet f(x) d\lambda_t(x)$ μ 可测，且 (9) 成立。*

让我们首先证明 a) (b))，假设 f 是 ν 调节的。关于集合 N 的断言已经成立（提案4，以及提案3的Cor.2）。根据§1, No. 2的第6号提案，在以下每种特殊情况下，我们可以将极限自己证明a）（或b））：

1) 函数 $f$ 是$\nu$-可以忽略不计。
2) 存在紧集$K$，使得$f$在$K$之外是零，并且$f$到$K$的限制是连续的。

特殊情况 1) 已被处理（Prop. 3 的 Cor. 1）。为了处理第二个，我们用$G$表示$\nu$可积开集合包含$K$，用$M$表示$f$的常数上界，用$h$表示下半连续函数 $M \varphi_G$，以及$g$函数$h - f$。由于函数$f$在$X$上是上半连续，$g$是下半连续且正。此外，$f, g, h$是$\nu$可积的。

然后，让我们将公式 (4)（或 (5)）应用于下半连续函数 $h$ 和 $g$。通过减法，我们看到函数

$$
t \mapsto \int^\bullet f(x)\, d\lambda_t(x) \quad (\text{resp. } \int^* f(x)\, d\lambda_t(x))
$$

是 $\mu$ 可测的，且公式 (9) (resp. (10)) 成立。最后，在b)的假设下，函数$t \mapsto \int^* f(x)\, d\lambda_t(x)$具有有限上积分，因此确实是$\mu$调节的。

为了证明c），让我们再次采用第3条第证明的措施$\mu_\alpha$和$\nu_\alpha$；由于 $f$ 是 $\nu_\alpha$ 可测量且 $\nu_\alpha$ 可调节，断言 a) 意味着 $t \mapsto \int^\bullet f(x)\, d\lambda_t(x)$ 是 $\mu_\alpha$ 可测量，并且

$$
\int^\bullet f(x)\, d\nu_\alpha(x) = \int^\bullet d\mu_\alpha(t) \int^\bullet f(x)\, d\lambda_t(x).
$$

它仅保留到 $\alpha$、应用道具上的和。 §2, No. 2 的 1 和 2。

如果 $f$ 不被假定为 $\nu$ 调节的，并且如果在 c) 中没有得到假设，则关系 (9) 可能不成立（例 3）。

#### 推论 {#int-v-s3-n2-cor-1 .statement tag=0918}

— *令$\mathbf{f}$为$X$上定义的函数，值位于Banach空间$F$或$\overline{\mathbf{R}}$中，即$\nu$可测量且$\nu$可调节。对于 $\mathbf{f}$ $\nu$ 可积，有充分必要*

$$
\int^\bullet d\mu(t) \int^\bullet |\mathbf{f}(x)|\, d\lambda_t(x) < +\infty.
$$

这立即来自第 5 条命题和可积性标准（第 IV, §5, No. 6 章，第 5 章）。

### 3. Banach 空间中函数与值的叠加积分

#### 定理 1 {#int-v-s3-thm-1 .statement tag=0919}

— 设 $f$ 为函数，其中值在 Banach 空间 $F$ 或 $\overline{\mathbf{R}}$ 中，并令 $H$ 为 $t \in T$ 的集合，其中 $f$ 不是$\lambda_t$-可积。

a) *如果 $f$ 是 $\nu$ 可积，则 $H$ 局部 $\mu$ 可忽略不计，函数 $t \mapsto \int f(x)\, d\lambda_t(x)$（为 $t \notin H$ 定义）本质上是 $\mu$ 可积，并且*

$$
\int f(x)\, d\nu(x) = \int d\mu(t) \int f(x)\, d\lambda_t(x).
$$

b) *如果$f$是$\nu$可积且$\Lambda$是模糊连续的，那么$H$此外$\mu$可忽略不计，函数$t \mapsto \int f(x)\, d\lambda_t(x)$（为$t \notin H$定义）是$\mu$可积。*

c) *如果 $\lambda_t^*(1) < +\infty$ 局部 $\mu$ - 几乎无处不在，那么 a) 的结论对于 $f$ 本质上 $\nu$ 可积函数仍然成立。*

我们首先要建立a）（分别b））。当$f$是正数函数时，叙述为真（命题5）；如果 $f$ 是可积函数，$\overline{\mathbf{R}}$ 中有值，则该结果可应用于正函数、$f^+$ 和 $f^-$，因此通过减法将扩展立即减至 $f$。剩下的就是用$F$中的值来处理函数的情况。令$\mathscr{H}$为线性组合形成的$\mathscr{L}_F^1(\nu)$的子空间，其中$F$为系数，$\mathscr{K}(X)$为函数；与实函数有关的结果立即意味着叙述对于$\mathscr{H}$的元素的有效性。现在，$\mathscr{H}$在$\mathscr{L}_F^1(\nu)$中是稠密的；因此，对于每个$f \in \mathscr{L}_F^1(\nu)$，都存在序列$(f_n)$ / 元素 / $\mathscr{H}$，它们具有以下属性：

1) 序列 $(f_n)$在$\mathscr{L}_F^1(\nu)$和$\nu$中均值收敛于$f$——几乎处处；
2) 函数 $g = |f_0| + \sum_{n \in \mathbf{N}} |f_{n+1} - f_n|$ 使得 $\nu^*(g) < +\infty$ (Ch. IV, §3, No. 4, Th. 3)。

令$N_1$为$t \in T$的集合，使得$\lambda_t^*(g) = +\infty$； $N_1$ 局部 $\mu$-可忽略（或 $\mu$-可忽略）乘以公式 (6)（或 (7)）。对于 $t \notin N_1$，$f_n$ 属于到 $\mathscr{L}_F^1(\lambda_t)$、序列 $(f_n)$ 几乎处处收敛于 $\lambda_t$，对于拓扑，$\mathscr{L}_F^1(\lambda_t)$ 中均值收敛（第 IV, §3, No. 3，提案 6）。令$M$为$x \in X$的集合，使得$f_n(x)$不会收敛到$f(x)$：因为$M$是$\nu$可忽略不计，集合$N_2$为$t \in T$，使得$M$ 不是 $\lambda_t$-可以忽略不计，是局部 $\mu$-可以忽略（或$\mu$-可以忽略）。提案 3 中的 1 条。

假设$t$不属于到$N_1 \cup N_2$； 序列$(f_n)$均值收敛于$\mathscr{L}_F^1(\lambda_t)$，并且$\lambda_t$几乎处处收敛到$f$。因此$f \in \mathscr{L}_F^1(\lambda_t)$和$\int f\, d\lambda_t = \lim_{n \to \infty} \int f_n\, d\lambda_t$（第IV, §4, No. 1章）。因此，叙述中的集合$H$包含在$N_1 \cup N_2$中；因此，它在本地$\mu$可以忽略不计（分别为$\mu$可以忽略不计）。另一方面，函数$t \mapsto \int f\, d\lambda_t$局部等于$\mu$-几乎处处等于$\mu$的序列的极限-可测量的函数；因此它是$\mu$-可测量的。最后，对于每个$t \notin N_1 \cup N_2$和每个$n$，我们有
$$
\left| \int f_n(x)\, d\lambda_t(x) \right| \leq \int^* g(x)\, d\lambda_t(x)
$$
凭借不等式 $|f_n| \leq g$ 和第 2 章的 Prop. 2 IV, §4, No. 2。现在，函数$t \mapsto \int^* g(x)\, d\lambda_t(x)$本质上是$\mu$可积（或$\mu$可积），根据命题5。因此，我们可以应用勒贝格的定理，得出
$$
\int d\mu(t) \int f(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int d\mu(t) \int f_n(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int f_n(x)\, d\nu(x).
$$
由于$\int f_n(x)\, d\nu(x)$趋于$\int f(x)\, d\nu(x)$，而$n$趋于$\infty$，根据序列$(f_n)$的假设，关系(11)如下，我们证明了a)(b))。

现在假设$\lambda_t^\bullet(1) < +\infty$局部$\mu$几乎无处不在，并且$g$本质上是一个$\nu$可积函数。令$f$为$\nu$可积函数，使得$g = f$局部$\nu$-几乎处处（§ 1, No. 3）。那么 $g = f$ 几乎无处不在 $\lambda_t$，除了 $t$ 形成局部 $\mu$ 可忽略不计的集合 $P$（第 3 条的 Cor. 1 c）。因此 $\int g\, d\lambda_t = \int f\, d\lambda_t$ 对于所有 $t \notin P \cup H$，这完成了证明。

#### 注 {#int-v-s3-n3-rem-1 .statement tag=091A}

令$\Lambda : t \mapsto \lambda_t$是$T$到$\mathscr{M}_+(X)$的$\mu$充分的映射。如果$T$到$\mathscr{M}_+(X)$的映射$\Lambda' : t \mapsto \lambda'_t$在局部$\mu$几乎处处都等于$\Lambda$，那么从定义立即得出$\Lambda'$也是$\mu$-足够的，并且$\Lambda$和$\Lambda'$ 有相同的积分。如果现在$H : t \mapsto \eta_t$是函数，$\mathscr{M}_+(X)$中的值，本地定义$\mu$-几乎无处不在，我们将再次说$H$是$\mu$-足够，如果它在本地$\mu$-几乎所有地方都等于映射 $\Lambda : t \mapsto \lambda_t$ 随处定义且 $\mu$ 足够。然后我们使用不依赖于函数$\Lambda$的集合$\int \eta_t\, d\mu(t) = \int \lambda_t\, d\mu(t)$、定义。我们留给读者的任务是验证前面的扩展到$\mu$中证明的命题-足够的函数本地定义$\mu$-几乎无处不在。

### 4. 普遍可测量函数

#### 定义 2 {#int-v-s3-def-2 .statement tag=091B}

*将 T 的映射 f 转换成拓扑空间 F，如果对于 T 上的每个正测度 $\mu$ $\mu$ 可测，则称 F 是普遍可测的。*

T 的子集其特征函数是普适可测的，称为普适可测集合。 他们形式 T 上的一个部落（第 1 章） IV, §5, No. 4，科。 2 Th。 2) 包含 Borel 集合（相同参考文献，Cor. 3），以及 Souslin 集合（如果 T 可度量）（第 1 章） IV, §5, No. 1，科。提案 3 中的 2）。 为了将 T 的映射 $f$ 转化为可度量且可分离的拓扑空间 F，并且是普遍可测的，F 中每个闭球的 $f$ 下的逆像是 T 的普遍可测子集是充分必要的（第 1 章）。 IV, §5, No. 5，Th。 4).

#### 命题 6 {#int-v-s3-prop-6 .statement tag=091C}

*为了使 T 的映射 $f$ 成为拓扑空间 F 普遍可测，$f$ 对于具有紧支撑的 T 上的每个正测度都是可测的。*

条件显然是必要的；另一方面，它是足够的，因为每个正测度$\mu$都是具有紧凑支持的测度系列中的和（§2, No. 3，命题4）：叙述则由§2, No. 2的命题2得出。

#### 命题 7 {#int-v-s3-prop-7 .statement tag=091D}

*设$\mu$为T上的正测度，并设$f$为T到拓扑空间F的$\mu$可测映射。那么，存在T到F的普遍可测映射$f'$，使得局部$f = f'$ $\mu$-几乎无处不在。*

令$\mathscr{K}$为T中紧集的集合，使得$f$的限制到K是连续的；由于 $\mathscr{K}$ 是 $\mu$ 稠密（第 IV, §5, No. 10 章，第 15 章），因此存在 $\mathscr{K}$ 的成对不相交的元素的局部可数族 $(K_i)_{i \in I}$，使得集合 $N = T - \bigcup_{i \in I} K_i$ 是局部的$\mu$-可以忽略不计（第 IV, §5, No. 9 章，第 14 条提案）。令$x$为F的元素； 集合

$$
f'(t) = f(t) \quad \text{if } t \in \bigcup_{i \in I} K_i,
$$
$$
f'(t) = x \quad \text{if } t \in N.
$$

函数 $f$ 和 $f'$ 在局部 $\mu$ 上相等——几乎在任何地方。另一方面，对于 T 中的每个紧集 K，$N \cap K$ 是 K 的 Borel 子集，因为族 $(K_i)$ 是局部可数的。由此可见，N 是普遍可测的集合，$f'$ 是普遍可测的函数（第 IV, §5, No. 10 章，第 16 条命题）。

### 5. 扩散

#### 定义 3 {#int-v-s3-def-3 .statement tag=091E}

*令X为局部紧致空间，令$\Lambda : t \mapsto \lambda_t$为T到$\mathscr{M}_+(X)$的映射。 映射 $\Lambda$ 被认为是 T 在 X 中的扩散*，如果 Λ 对于具有紧凑支持的 T 上的每个正测度来说是足够的。如果所有测度 λ_t 都是有界且 $\sup_{t \in T} \| \lambda_t \| < +\infty$，则称扩散 Λ 是有界的；这个量称为 Λ 的范数，并表示为 $\| \Lambda \|$。

以下命题仅翻译定义：

#### 命题 8 {#int-v-s3-prop-8 .statement tag=091F}

— 为了使 T 的映射 $\Lambda : t \mapsto \lambda_t$ 进入 $\mathscr{M}_+(X)$ 成为扩散，满足以下条件是必要且充分的：
1) 对于在 X 上定义的每个下半连续函数 $f \geqslant 0$，函数 $t \mapsto \lambda_t^\bullet(f)$ 在 T 上普遍可测。
2) 对于每个函数 $g \in \mathscr{K}_+(X)$，函数 $t \mapsto \lambda_t(g)$ 在 T 中局部有界。
3) 对于 X 上定义的每个下半连续函数 $f \geqslant 0$ 以及对于具有紧支撑的 T 上的每个正测度 $\mu$，以下关系成立，其中 $\nu$ 表示 $\int \lambda_t d\mu(t)$：

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

假设 $\Lambda$ 是扩散。 条件 1) 然后由足够的映射 (No. 1, Def. 1) 和 Prop. 6 的定义满足； 条件 3) 由公式 (4) 满足，因为$\Lambda$ $\mu$ 是足够的。令 $g \in \mathscr{K}_+(X)$ 且令 $u$ 为函数 $t \mapsto \lambda_t(g)$（普遍可测，乘以 1））；假设 $u$ 不是局部有界的。那么将存在紧集 K，使得$u$不受K约束，因此将存在K的元素的序列$(t_n)$，使得对于所有$n \geqslant 1$有$u(t_n) \geqslant n^2$；那么$u$对于紧支持下的测度$\mu = \sum_{n \geqslant 1} \frac{1}{n^2} \varepsilon_{t_n}$是不可积的，与$\Lambda$上的假设相反，这意味着$t \mapsto \lambda_t(g)$对于紧支持下的每个正测度都是可积的。因此，上述三个条件是必要的。相反，条件 1) 和 2) 意味着$\Lambda$本质上是$\mu$——在紧致支持下对于每个测度$\mu$可积。由于上面由具有紧支撑的测度 $\mu$ 限制的每个测度 $\mu' \geqslant 0$ 也具有紧支撑，条件 1) 和 3) 表示 $\Lambda$ 是 $\mu$ - 对于每个具有紧支撑的正测度来说是充分的，这确实是所寻求的结果。

#### 命题 9 {#int-v-s3-prop-9 .statement tag=091G}

— 令 $\Lambda : t \mapsto \lambda_t$ 为 T 到 $\mathscr{M}_+(X)$ 的映射，使得对于每个 $g \in \mathscr{K}_+(X)$，函数 $t \mapsto \lambda_t(g)$ 是普遍可测的且在 T 中局部有界。在以下每种情况下，可以肯定 $\Lambda$ 是扩散：

a) *X的拓扑承认可数基*；
b) *Λ 对于模糊拓扑* 是普遍可测的。

因为，令 $\mu$ 为具有紧支撑的$T$ 的正测度； 映射$\Lambda$本质上是$\mu$可积，因此如果满足a)或b)则$\mu$是充分的（No. 1，命题2）。

对于这个截面的其余部分，我们将采用以下记号：我们将用$⟨\eta, h⟩$表示对于正测量$\eta$，正$\eta$可测量函数$h$的上基本积分。 映射 $\Lambda : t \mapsto \lambda_t$ 将是 $T$ 在 $X$ 中的扩散。如果$f$是定义在$X$上的正的普遍可测函数，我们将用$\Lambda f$映射$t \mapsto \lambda_t^*(f)$表示。如果$\mu$是$T$的正测度，使得$\Lambda$本质上是$\mu$可标量可积，我们将用$\mu\Lambda$表示测度$\int \lambda_t d\mu(t)$。积分的定义则取形式

$$
⟨\mu\Lambda, f⟩ = ⟨\mu, \Lambda f⟩ \quad \text{for } f \in \mathscr{K}_+(X).
$$

我们可以说，如果$\Lambda$是$\mu$充分的话，$T$*属于对$\Lambda$*域的正测度$\mu$：这相当于说（根据第8条命题），$\Lambda$本质上是$\mu$可积的$⟨\mu'\Lambda, f⟩ = ⟨\mu', \Lambda f⟩$ 对于每个正测量$\mu' \leq \mu$ 和每个下半连续正函数 $f$。

#### 命题 10 {#int-v-s3-prop-10 .statement tag=091H}

*令$f, g$为$X$上的两个正普遍可测函数，让$a$为数$\geq 0$，并让$\mu$和$\nu$为$T$上的两个正测度。然后：*

a) $\Lambda(f + g) = \Lambda f + \Lambda g$、$\Lambda(af) = a\Lambda f$。
b) *如果$\mu$和$\nu$属于到$\Lambda$的域，那么$\mu + \nu$和$a\mu$也是如此，并且有*$(\mu + \nu)\Lambda = \mu\Lambda + \nu\Lambda$，$(a\mu)\Lambda = a(\mu\Lambda)$。

唯一不明显的点是$\mu + \nu$属于到$\Lambda$的域，通过注意到处理，上面由$\mu + \nu$界定的每个正测度都是形式$\mu' + \nu'$，其中$\mu' \leq \mu$， $\nu' \leq \nu$（“分解引理”，第II, §1, No. 1）。另请参阅下一个命题。

#### 命题 11 {#int-v-s3-prop-11 .statement tag=091I}

*对于$T$到属于到$\Lambda$域的正测度$\mu$，$\Lambda$基本上是$\mu$可标量可积是必要且充分的。*

这个条件显然是有必要的。相反，假设满足，令$f$为$X$上定义的下半连续正函数。 函数 $\Lambda f$ 是普遍可测的，因而 $\mu$ 可测。我们要证明$⟨\mu, \Lambda f⟩ = ⟨\mu\Lambda, f⟩$；因为这个等式对于每个正测度$\mu' \leq \mu$也有效，因为$\Lambda$本质上也是$\mu'$可积的，因而$\Lambda$是$\mu$足够的。

令 $(\mu_i)_{i\in I}$ 为具有紧支持的正测度的可求和族，使得$\mu = \sum_{i\in I} \mu_i$（§2, No. 3，命题 4）；然后，措施族 $\mu_i \Lambda$ 可求和，并且 $\mu \Lambda = \sum_{i \in I} \mu_i \Lambda$（No. 1，命题 1 的 Cor.）。因而$\langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle$（§ 2, No. 2，命题1）；但 $\Lambda$ $\mu_i$ 足够，因而$\langle \mu_i \Lambda, f \rangle = \langle \mu_i, \Lambda f \rangle$。再次根据§ 2的应用命题1，我们得到了所寻求的等式：

$$
\langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i, \Lambda f \rangle = \langle \mu, \Lambda f \rangle .
$$

#### 推论 1 {#int-v-s3-prop-11-cor-1 .statement tag=091J}

— *如果 $\Lambda$ 是有界扩散，则每个有界正测度 $\mu$ 属于到 $\Lambda$ 和 $\| \mu \Lambda \| \leq \| \mu \| \| \Lambda \|$ 的域。*

#### 推论 2 {#int-v-s3-prop-11-cor-2 .statement tag=091K}

— *假设$\mu$是$\Lambda$域的正测度属于的可和族$(\mu_\alpha)_{\alpha \in A}$的和。对于$\mu$到属于到$\Lambda$的域，测度族$\mu_\alpha \Lambda$可求和是必要且充分的，在这种情况下$\mu \Lambda = \sum_{\alpha \in A} \mu_\alpha \Lambda$。*

应用No. 1第1号提案推论即可。

命题 5，用扩散语言表达，取以下形式：

#### 命题 12 {#int-v-s3-prop-12 .statement tag=091L}

— *令$\mu$为$T$上属于对$\Lambda$域的正测度，并令$f$为在$X$上定义的通用可测函数$\geq 0$。如果$f$针对测度$\mu \Lambda$进行调节，或者如果测度$\lambda_t$有界，则函数$\Lambda f$是$\mu$可测且*

$$
\langle \mu \Lambda, f \rangle = \langle \mu, \Lambda f \rangle .
$$

#### 推论 {#int-v-s3-n5-cor-1 .statement tag=091M}

— *如果 $X$ 在无穷大处可数，或者如果测量 $\lambda_t$ 有界，则对于 $X$ 上定义的每个普遍可测的函数 $f \geq 0$，函数 $\Lambda f$ 在 $T$ 上普遍可测，并且 (13)成立。*

### 6. 有界扩散的合成

#### 命题 13 {#int-v-s3-prop-13 .statement tag=091N}

— *令$T, X, Y$为三个局部紧凑空间，$\Lambda : t \mapsto \lambda_t$为$T$在$X$中的有界扩散，$H : x \mapsto \eta_x$为$X$在$Y$中的有界扩散。那么映射$t \mapsto \lambda_t H$就是$T$在$Y$的有界扩散，用$\Lambda H$表示，并且*

$$
\| \Lambda H \| \leq \| \Lambda \| \| H \|.
$$

*设$f$为$Y$上定义的通用可测函数$\geq 0$，$\mu$为$T$上的测度。假设$\mu$属于到$\Lambda$的域，并且*μΛ属于到H的域；然后 μ 属于到 ΛH 的域，并且

$$
\langle \mu(\Lambda H), f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda Hf \rangle;
$$
(15)
$$
(\mu \Lambda)H = \mu(\Lambda H); \quad \Lambda(Hf) = (\Lambda H)f.
$$

集合$\gamma_t = \lambda_t H$；我们将用T的$\Gamma$映射$\Lambda H$表示为$\mathscr{M}_+(Y)$，并用$\Gamma f$函数$t \mapsto \langle \gamma_t, f \rangle$（滥用记号，因为我们还不知道$\Gamma$是否是扩散）。然后$\langle \gamma_t, f \rangle = \langle \lambda_t H, f \rangle = \langle \lambda_t, Hf \rangle$乘以(13)；由于函数 $Hf$ 是正数并且在 X（第 12 条命题的修正）上普遍可测，因此它首先遵循 $\Gamma f = \Lambda(Hf)$，然后 $\Gamma f$ 在 T 上普遍可测（相同的参考）。显然，所有$\gamma_t$的总质量最多等于$\| \Lambda \| \| H \|$。因而，$\Gamma g$ 是普遍可测的，并且对于每个函数 $g \in \mathscr{K}_+(Y)$ 都是有界的；因而，对于 T 上的每个有界测度，$\Gamma$ 本质上是可标量可积的，特别是对于具有紧凑支持的每个测度。更一般地，如果 $\mu$ 是 $\Lambda$ 域中的测度，使得 $\mu \Lambda$ 属于到 H 域，那么，对于 $g \in \mathscr{K}_+(Y)$，

$$
\langle \mu, \Gamma g \rangle = \langle \mu, \Lambda(Hg) \rangle = \langle \mu \Lambda, Hg \rangle = \langle (\mu \Lambda)H, g \rangle.
$$

由于最后一个数量是有限的，我们看到 $\Gamma$ 本质上是 $\mu$ 可积的。让我们用$\mu \Gamma$表示积分$\int \gamma_t d\mu(t)$（滥用记号，因为我们还不知道$\Gamma$是否是扩散）。前面的关系可以写成

$$
\langle \mu \Gamma, g \rangle = \langle (\mu \Lambda)H, g \rangle,
$$

或者也$\mu \Gamma = (\mu \Lambda)H$，因为$g$在$\mathscr{K}_+(Y)$中是任意的。

重新考虑普遍可测量的函数$f \geqslant 0$。我们有

$$
\langle \mu \Gamma, f \rangle = \langle (\mu \Lambda)H, f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda(Hf) \rangle = \langle \mu, \Gamma f \rangle.
$$

当$f$是下半连续且$\mu$运行在紧支持的正测度集合时，这些关系表示$\Gamma$是T在Y中的扩散。断言则只不过是明确在上述证明过程中获得的关系。

#### 定义 4 {#int-v-s3-def-4 .statement tag=091O}

*记号是命题13的那些，扩散$\Lambda H$称为有界扩散H和$\Lambda$的组合扩散（或合成）。*

令$X_1, X_2, X_3, X_4$分别为$X_2$中$X_1$、$X_3$中$X_2$、$X_4$中$X_3$的四个局部紧凑空间和$\Lambda_1, \Lambda_2, \Lambda_3$三个有界扩散。从第 13 条命题可以立即得出结论：

$$
(\Lambda_1 \Lambda_2) \Lambda_3 = \Lambda_1 (\Lambda_2 \Lambda_3).
$$

因而，我们将使用这些不带括号的记号来表示扩散的合成。

#### 例 {#int-v-s3-n6-exa-1 .statement tag=091P}

令$u$为T到X的普遍可测映射，以及$v$为X到Y的普遍可测映射；根据提案 2 b)，通过公式进行 1 个定义扩散 $\Lambda$ 和 $H$

$$
\lambda_t = \varepsilon_{u(t)}, \quad \eta_x = \varepsilon_{v(x)};
$$

扩散 $\Gamma = \Lambda H$ 则由下式给出

$$
\gamma_t = \varepsilon_{(vou)(t)}.
$$

因而，请注意扩散的合成的阶与通常的函数的阶或合成相反。

### 习题{#int-v-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
