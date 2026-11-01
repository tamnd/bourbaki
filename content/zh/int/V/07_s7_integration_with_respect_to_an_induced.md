---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 7
section_title: Integration with respect to an induced measure
lang: zh
source: int-i-vi
book_pages: INT V.74-INT V.78, INT V.112-INT V.114
pdf_pages: 0329-0333, 0367-0369
extraction: ocr
subsections:
    - "no": 1
      title: Integration with respect to an induced measure
      page: 74
      pdf_page: 329
    - "no": 2
      title: Properties of induced measures
      page: 77
      pdf_page: 332
statements: 20
exercises: 11
content_sha256: 3654f12fcfb1c9a39b2dd2789af42eb4b149cb4e34f34c186373b90e0993afa8
translated_from: content/en/int/V/07_s7_integration_with_respect_to_an_induced.md
translation_method: google
source_content_sha256: 0f5f27152d636e2b4a3f4de2fe99a74694ba33c12058af8b625950449ac3a190
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 0dc08149252c5e4aec0c2c19b01afaa8d0e67d3ee7eb133312bc9e9c7395cfff
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 7。与诱导措施相关的积分

### 1. 关于诱导测量的积分

令$X$为$T$的局部紧凑子空间，$\mu$为$T$的正测度，$\mu_X$为$\mu$在$X$上引发的测度（第IV, §5, No. 7）。对于每个$t \in T$，让我们按以下方式在$\lambda_t$*上*$X$测量定义：如果$t \in X$则$\lambda_t = \varepsilon_t$，如果$t \in \mathbf{C}X$则$\lambda_t = 0$。对于在$X$、$\int g(x) d\lambda_t(x) = g(t)$（如果$t \in X$）和$\int g(x) d\lambda_t(x) = 0$（如果$t \in \mathbf{C}X$）上定义的每个有限数值函数$g$。如果$g$在$\mathscr{K}(X)$中是函数，那么我们可以通过$\mu_X$的定义，

$$
\mu_X(g) = \int \langle g, \lambda_t \rangle d\mu(t) .
$$

这意味着人们可以写

$$
\mu_X = \int \lambda_t d\mu(t)
$$

（§3, No. 1）。

现在让我们将 T 的定义映射 $\pi$ 转换为 X，对于 $t \in X$，通过设定 $\pi(t) = t$，对于 $t \in \mathbf{C}X$，$\pi(t) = t_0$，$t_0$ 是任意点 X；每个$t \in T$可以写出$\lambda_t = \varphi_X(t)\varepsilon_{\pi(t)}$。 映射 $\pi$ 是 $\mu$ 可测的，因为它的限制到 X 和 $\mathbf{C}X$ 是（第 IV, §5, No. 10 章，第 16 条）；由此可见，对$(\pi, \varphi_X)$是$\mu$适合的（§4, No. 1）。因此我们得到以下结果：

#### 命题 1 {#int-v-s7-prop-1 .statement tag=0963}

— *对于每个数字函数* $g \geqslant 0$ *定义于* X，

$$
\int^\bullet g\,d\mu_X = \int_X g\,d\mu
$$

（cf.§5, No. 3，*例*，记号$\int_X^\bullet$）。

考虑到前面的注和(2)，关系(3)由Th推出。 1 个§4。

#### 推论 1 {#int-v-s7-prop-1-cor-1 .statement tag=0964}

— *对于每个子集* B *of* X, $\mu_X^\bullet(B) = \mu^\bullet(B)$； *对于*B *在本地*$\mu_X$*-可忽略不计，*B *在本地*$\mu$*-可忽略*是必要且充分的。

#### 推论 2 {#int-v-s7-prop-1-cor-2 .statement tag=0965}

— *设* M *为* T 的子集。*如果* $\mu$ *集中于* M，*则* $\mu_X$ *集中于* $M \cap X$。

#### 推论 3 {#int-v-s7-prop-1-cor-3 .statement tag=0966}

— *对于测量* $\mu_X$ *为零，* X *在本地* $\mu$*-可忽略不计*是必要且充分的。

#### 注 {#int-v-s7-n1-rem-1 .statement tag=0967}

— 如果 S 是 $\mu$ 的支持，则 $S \cap X$（在 X 中闭合）包含 Cor 的$\mu_X$ 的支持。 2，但可能与它不同。对于例，如果$\mu$是扩散测度并且X是子空间减少到点，那么诱导测度$\mu_X$是零，因此它的支撑是空的。然而，注，如果X在T中开放，$\mu_X$的支持度等于$S \cap X$。

#### 命题 2 {#int-v-s7-prop-2 .statement tag=0968}

— *对于 * X *的映射* g * 到拓扑空间为* $\mu_X$* 可测量，* g * 为* $\mu$* 可在* X *(§5, No. 3, *例*)*。

这是从§4 的第 3 号提案得出的。

#### 推论{#int-v-s7-n1-cor-1 .statement tag=0969}

— *对于* X *的子集* B *为* $\mu_X$*可测量，* B *为* $\mu$*可测量*是必要且充分的。

#### 定理 1 {#int-v-s7-thm-1 .statement tag=096A}

— *Let* g *be a function defined on* X, *with values in* $\overline{\mathbf{R}}$ *or in a Banach space. 对于* g *本质上* $\mu_X$*可积，$g$本质上$\mu$可在$X$（§ 5, No. 3，例）中可积是必要*且充分的，在这种情况下

$$
\int g \, d\mu_X = \int_X g \, d\mu.
$$

这是从 Th 得出的。 2 个§ 4。

#### 推论 1 {#int-v-s7-thm-1-cor-1 .statement tag=096B}

*对于 X 的子集 B 本质上$\mu_X$可积，它本质上$\mu$可积是必要且充分的，在这种情况下$\mu_X(B) = \mu(B)$。*

#### 推论 2 {#int-v-s7-thm-1-cor-2 .statement tag=096C}

*设 g 为在 T 上定义且局部 $\mu$ 可积的复数函数； g 到 X 的限制 $g_X$ 则可局部 $\mu_X$ 可积，并且*

$$
(g \cdot \mu)_X = g_X \cdot \mu_X.
$$

这是从 Th 立即得出的。 1，应用于函数 $fg_X$ ($f \in \mathscr{K}(X; \mathbf{C})$)，以及由复杂测度（第 IV, § 5, No. 7）在 X 上引发的测度的定义。

#### 推论 3 {#int-v-s7-thm-1-cor-3 .statement tag=096D}

*令 $\theta$ 为 T 上的复测度；然后*

$$
|\theta|_X = |\theta_X|.
$$

集合 $|\theta| = \mu$ 并应用 Cor. 2 将 $g$ 视为绝对值 1 的复数函数，使得 $\theta = g \cdot \mu$（§ 5, No. 5，Th. 2 的 Cor. 3）；然后$\theta_X = g_X \cdot \mu_X$；但$g_X$是值1的绝对值函数，公式(6)由§ 5, No. 2的命题2得出。

#### 注 {#int-v-s7-n1-rem-2 .statement tag=096E}

— a) Cor. 3已经被另一个方法证明（第IV, § 5, No. 7，引理3）。
    b) 凭借 Cor. 3、命题1、命题2、定理1的推论1,2,3及其推论1,2扩展同时到一个复杂的测度。

#### 学院{#int-v-s7-n1-sch-1 .statement tag=096F}

— For every function $f$ (resp. $g$) defined on $X$ (resp. $T$) with values in the Banach space $F$ or in $\overline{\mathbf{R}}$, let us denote by $\zeta(f)$ (resp. $\rho(g)$) the extension by 0 of $f$ to $T$ (resp. the restriction of $g$ to $X$). 然后$\zeta(\rho(g)) = \varphi_X \cdot g$，$\rho(\zeta(f)) = f$。 我们用$\mu'$表示$T$上的$\varphi_X \cdot \mu$测度。 对于每个$p \in [1, +\infty]$，道具。 1和2意味着$\zeta$映射$\mathscr{L}_F^p(X, \mu_X)$进入$\mathscr{L}_F^p(T, \mu')$，以及$\rho$映射$\mathscr{L}_F^p(T, \mu')$进入$\mathscr{L}_F^p(X, \mu_X)$，在两种情况下都保留范数，以及$p = 1$（Th.1）时的积分；将经过代入关联的Hausdorff空间，我们得到两个互为逆的同构。 类似地，如果将$\zeta$和$\rho$应用于正数值函数，则保留基本的上积分（命题1）。 因此，如果我们同意 $X$ 上的 *认同* 函数以及 T 上的函数，即 X − T 上的零，并且措施 $\mu_X$ 和措施 $\mu'$，则有关诱导措施的问题会减少到有关由下式定义的措施的问题：密度，按§5处理。 这种推理也适用于复杂的度量，Cor. 3 Th。 1.

### 2. 诱导测度的属性

#### 命题 3 {#int-v-s7-prop-3 .statement tag=096G}

— 令 X 为 T 的局部紧凑子空间，而 $\lambda$ 为 X 的复测度。以下属性是等效的：
a) 典范嵌入 $i : X \to T$ 是 $\lambda$-本征；
b) 对于 T 的每个紧致子集 K，$K \cap X$ 本质上是 $\lambda$ 可积；
c) 每个点$t \in T$承认一个邻域V，使得$V \cap X$本质上是$\lambda$可积；
d) T 上存在一个测度$\theta$，使得$\theta_X = \lambda$。
如果这些等价的条件得到满足，我们就有 d) 中的记号，

$$
(i(\lambda))_X = \lambda \quad \text{and} \quad i(\lambda) = i(\theta_X) = \varphi_X \cdot \theta .
$$

单射$i$是连续的，属性a)、b)和c)的等价来自§6的命题1，其后面的注应用于正测度$|\lambda|$。如果通过 T 上的测度 $\theta$ 在 X 上导出 $\lambda$，则$|\lambda| = |\theta|_X$ (公式 (6))，因此对于 T 的每个紧致子集 K 都有 $|\lambda|(K \cap X) = |\theta|(K \cap X) \leq |\theta|(K) < +\infty$（命题 1），因而 d) 蕴涵 b)。假设满足a)，让我们证明$(i(\lambda))_X = \lambda$，这将暗示d)。令g为$\mathscr{H}(X; \mathbf{C})$的元素；用 $g'$ 扩张用 g 到 T 的 0 表示，我们有，用诱导测度的定义，然后用 §6, No. 4 的命题 7，

$$
\int g \, d(i(\lambda))_X = \int g' \, d(i(\lambda)) = \int (g' \circ i) \, d\lambda = \int g \, d\lambda .
$$

这样就完成了四个属性中的等价中的证明。如果$\lambda = \theta_X$和$g \in \mathscr{H}(T; \mathbf{C})$，那么

$$
\int g \, d(i(\theta_X)) = \int (g \circ i) \, d(\theta_X) = \int g \varphi_X \, d\theta ,
$$

因为$g \varphi_X$是扩张除以0的$g \circ i$到T。这就证明了(7)的第二个公式。

#### 推论 1 {#int-v-s7-prop-3-cor-1 .statement tag=096H}

— 如果 X 是闭合的，则 X 上的每个复杂测度 $\lambda$ 都是由 T 上的测度引发的。

因为，如果 T 中的 K 为紧集，则 K ∩ X 是紧致的，因此是 λ 可积的。

#### 推论 2 {#int-v-s7-prop-3-cor-2 .statement tag=096I}

— 令 θ 为 T 上的复测度，π 将 T 的 θ-proper 映射转换为局部紧凑的空间 Y，并且 π_X 为限制到 X。那么 π_X 就是 θ_X-proper，并且 π_X(θ_X) = π(φ_X · θ)。

对于，π_X = π ∘ i，其中 i 为典范嵌入 X → T。当 θ 为正时，推论因此可以从命题 3 和像测量的传递性推导出来（§6, No. 3，命题 4）。非正复测度的情况则遵循线性。

#### 命题 4 {#int-v-s7-prop-4 .statement tag=096J}

— 令 X 和 Y 为 T 的两个局部紧凑子空间，使得 Y ⊂ X。如果 θ 是 T 上的复测度，则 θ_X 在 Y 上引发的测度 (θ_X)_Y 等于 θ_Y（“引发测度的传递性”）。

足以观察到，如果 g 是 $\mathscr{H}(Y; \mathbf{C})$ 的元素，则可以通过将 g 的 0 扩张扩展到 X 来获得扩张乘以 0 的 g 到 T，或者再次利用 Scholium 的标识，即 $\varphi_Y · \theta = \varphi_Y(\varphi_X · \theta)$ （§5, No. 4，提案 8）。

#### 命题 5 {#int-v-s7-prop-5 .statement tag=096K}

— 令 $(\lambda_\alpha)_{\alpha \in A}$ 为 T 上的递增有向测度族，承认上确值 λ，并令 X 为 T 的局部紧致子空间。诱导测度族 $\lambda_\alpha|X$ 的上界为 $\mathscr{M}(X)$，并且

$$
\sup_{\alpha \in A} (\lambda_\alpha|X) = \lambda|X.
$$

从学界的认定来看，这个命题是§5, No. 4第5号提案的特例。

#### 推论{#int-v-s7-n2-cor-1 .statement tag=096L}

— 令 $(\mu_i)_{i \in I}$ 为 T 上的正测度的可求和族，其中和 μ。然后可对诱导测度族$\mu_i|X$进行求和，并且

$$
\sum_{i \in I} (\mu_i|X) = \mu|X.
$$

#### 命题 6 {#int-v-s7-prop-6 .statement tag=096M}

— 令 $\Lambda : t \mapsto \lambda_t$ 为 T 到 $\mathscr{M}_+(X)$ 的 μ 充分映射，其中 X 为无穷大可数的局部紧致空间，并令 Y 为 X 的局部紧致子空间。 集合$\int \lambda_t d\mu(t) = \nu$。 T 的映射 $t \mapsto \lambda_t|Y$ 进入 $\mathscr{M}_+(Y)$ 那么 μ 是足够的，并且

$$
\int (\lambda_t|Y) d\mu(t) = \nu|Y.
$$

考虑到学院中的鉴定，这个命题是§5, No. 4第7号提案的特例。

### 习题{#int-v-s7-exercises}

§ 7](exercises/s7/)参见[习题。
