---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 6
section_title: Images of a measure
lang: zh
source: int-i-vi
book_pages: INT V.62-INT V.74, INT V.107-INT V.112
pdf_pages: 0317-0329, 0362-0367
extraction: ocr
subsections:
    - "no": 1
      title: Image of a positive measure
      page: 62
      pdf_page: 317
    - "no": 2
      title: Integration with respect to the image of a positive measure
      page: 64
      pdf_page: 319
    - "no": 3
      title: Properties of the image of a positive measure
      page: 65
      pdf_page: 320
    - "no": 4
      title: Image of a complex measure
      page: 68
      pdf_page: 323
    - "no": 5
      title: 'Application: change of variable in the Lebesgue integral'
      page: 69
      pdf_page: 324
    - "no": 6
      title: Decomposition into slices. Inverse image of a measure under a local homeomorphism
      page: 71
      pdf_page: 326
statements: 29
exercises: 22
content_sha256: 9d18c87e86a3c8de0389a187ca79e7ffe8994c93101dd9704c935885df78e5f6
translated_from: content/en/int/V/06_s6_images_of_a_measure.md
translation_method: google
source_content_sha256: b4ee00e28c0ad5363315a73bf228d2a58c397d50dececefce928f935c44c92bb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 194b570541e1f83280f18924d787775028256f9b4ab92f10b65917c9ef1d9e62
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 6。 像尺寸

### 1. 像积极措施

令$X$为空间的局部紧凑空间，$\pi$将$T$的$\mu$可测映射放入$X$。说对$(\pi, 1)$是*$\mu$适应*（§4, No. 1）相当于说，对于每个函数$f \in \mathscr{K}(X)$，函数$f \circ \pi$*本质上是$\mu$可积*。

#### 命题 1 {#int-v-s6-prop-1 .statement tag=094O}

*令 $\pi$ 为 $T$ 的 $\mu$ 可测量映射为局部紧致空间 $X$。以下两个属性是等效的：*

a) *对于每个函数* $f \in \mathscr{K}(X)$，$f \circ \pi$ *本质上是* $\mu$-*可积*。

b) *对于每个紧集* $K \subset X$，$\overline{\pi}^{-1}(K)$ *本质上是* $\mu$-*可积*。

我们刚刚观察到 a) 意味着对 $(\pi, 1)$ 是 $\mu$ 适应的。因而（§ 4, No. 4，Th.2），对于每个紧集$K \subset X$，函数$\varphi_K \circ \pi = \varphi_A$，其中$A = \overline{\pi}^{-1}(K)$本质上是$\mu$可积，在其他字中，a）意味着b）。

相反，假设对于$X$的每个紧致子集$K$，$\overline{\pi}^{-1}(K)$本质上是$\mu$可积，并且让我们证明a）已被验证。事实上，让$S$成为$f$的支撑；由于 $S$ 是紧致的，设定 $A = \overline{\pi}^{-1}(S)$ 我们有假设，

$$
\int^\bullet |f(\pi(t))| \, d\mu(t) \leq \|f\| \int^\bullet \varphi_S(\pi(t)) \, d\mu(t) = \|f\| \int^\bullet \varphi_A(t) \, d\mu(t) < +\infty.
$$

由于 $f \circ \pi$ 是 $\mu$ 可测（第 IV, § 5, No. 3，第 1 章），我们看到 $f \circ \pi$ 本质上是 $\mu$ 可积（§ 1, No. 3，第 9 条）。

性质 b) 显然等价于以下内容（因此也等价于 a)）：

c) *对于* $X$的每个点* $x$ *，*存在一个* $V$ *的邻域* $x$ *使得* $\overline{\pi}^{-1}(V)$ *本质上是* $\mu$-*可积*。

#### 定义 1 {#int-v-s6-def-1 .statement tag=094P}

*让*$\mu$*成为局部紧凑空间*$T$的正测度。 *映射* $\pi$ *of* $T$ *转化为局部紧凑的空间* $X$ *据说是* $\mu$*-适当*（*或适当的度量* $\mu$）*如果对* $(\pi, 1)$ *是* $\mu$*-适应*，*即* (§ 4, No. 1)，*如果* $\pi$ *是* $\mu$*-可测量并满足命题 1* 的（等效）条件。 *测量* $\int \varepsilon_{\pi(t)} \, d\mu(t)$ *在* $X$ *然后称为* $\mu$ *下* $\pi$ *的像，并表示为* $\pi(\mu)$。

因此，如果 $\nu = \pi(\mu)$ 那么，通过定义，对于 $f \in \mathscr{K}(X)$ 有

$$
\int f(x) \, d\nu(x) = \int f(\pi(t)) \, d\mu(t).
$$

#### 注{#int-v-s6-n1-rem-1 .statement tag=094Q}

— 1) 如果 $\mu$ 是*有界*（特别是，如果 $\mu$ 具有紧凑支持），则 $T$ 到 $X$ 的每个 $\mu$-可测量映射都是 $\mu$-本征（Ch. IV, § 5, No. 3、Th. 1 和No. 6，第 5)。

2) 如果 $\pi$ 是 $\mu$-可测的，并且对于 $X$ 的每个紧致子集 $K$，$\overline{\pi}^{-1}(K)$ 是相对紧致的，那么 $\pi$ 是 $\mu$-真（第 IV, § 5, No. 5 章，第 7 条）和No. 6，Th 5）；特别是，$T$到$X$（GT，I, § 10, No. 2，Th.1）的每个“适当”连续映射对于$T$上的每个积极措施$\mu$来说都是$\mu$。更具体地说，对于$T$到X的每个“同胚”$\pi$都是如此；那么，措施$\nu = \pi(\mu)$就是X上的措施，即$\mu$乘$\pi$的迁移（第III, §1, No. 3）。

3) 假设X中的拓扑承认可数的基；那么满足命题 1 的条件 b) 的每个 T 的映射 $\pi$ 到 X 都是 $\mu$ 可测的，因此是 $\mu$ 正确的。应用Th就足够了。第 4 章。 IV, §5, No. 5，在注意到上，X 是可度量的（GT，IX, §2, No. 9，Prop. 16 的 Cor.），并且，对于与 X 的拓扑兼容的任何度量，每个闭球都是可数的并紧集。

### 2. 关于积极措施像的积分

设$\pi$是T到X的$\mu$真映射，并设$\nu = \pi(\mu)$。 应用 §4的结果，得到如下叙述：

#### 命题 2 {#int-v-s6-prop-2 .statement tag=094R}

— *对于每个数字函数* $f \geqslant 0$ *定义于* X，
$$
\int^\bullet f(x)\, d\nu(x) = \int^\bullet f(\pi(t))\, d\mu(t).
$$
(2)

这是从 Th 得出的。 §4, No. 2 中的 1 个。

#### 推论 1 {#int-v-s6-prop-2-cor-1 .statement tag=094S}

— *对于每个子集* A *of* X，
$$
\nu^\bullet(A) = \mu^\bullet(\pi^{-1}(A)).
$$

#### 推论 2 {#int-v-s6-prop-2-cor-2 .statement tag=094T}

— *对于* 子集* A ** X *对于* $\nu$ *局部可忽略不计，*对于* $\pi^{-1}(A)$ *局部可忽略* $\mu$ 是必要且充分的。

#### 推论 3 {#int-v-s6-prop-2-cor-3 .statement tag=094U}

— *如果测量* $\mu$ *集中在集合* M，*则* $\pi(\mu)$ *集中在* $\pi(M)$。

因为，如果$N = X - \pi(M)$则$\pi^{-1}(N)$不与M相交，因此局部$\mu$可忽略不计，因而（Cor.2）N局部$\nu$可忽略不计。

#### 推论 4 {#int-v-s6-prop-2-cor-4 .statement tag=094V}

— *让* S *成为* $\mu$ 的支持。 *如果*$\pi$*连续，则*$\pi(\mu)$*的支持度为*$\pi(S)$。

因为，它是从 Cor 得出的。 3 $\pi(\mu)$集中于$\pi(S)$，因此如果$S'$是$\pi(\mu)$的支撑，则$S' \subset \pi(S)$。另一方面，$\pi^{-1}(X - S')$是局部$\mu$可忽略的开集合（Cor.2），因而$\mu$可忽略不计（第5章第IV, §5, No. 2，Cor.2）。因而$\pi^{-1}(X - S') \subset T - S$，因而$\pi(S) \subset S'$，这证明了推论。

#### 命题 3 {#int-v-s6-prop-3 .statement tag=094W}

— *对于 * X *的映射* f * 到拓扑空间* G * 为* $\nu$* 可测量，* $f \circ \pi$ * 为* $\mu$* 可测量是必要且充分的。*

这是§4, No. 3第3条命题的直接的推论。

#### 推论{#int-v-s6-n2-cor-1 .statement tag=094X}

— 对于 X 的子集 A 为 $\nu$ 可测，$\pi^{-1}(A)$ 为 $\mu$ 可测是充分必要的。

然而，T 的 $\mu$ 可测量子集 M 的 $\pi$ 下的像不一定是 $\nu$ 可测量，即使 $\pi$ 是连续的且 M $\mu$ 可忽略不计（Exer. 7 和 §8，Exer. 1）。

#### 定理 1 {#int-v-s6-thm-1 .statement tag=094Y}

— 设 f 是在 X 上定义的函数，其中值在 $\overline{\mathbf{R}}$ 或 Banach 空间 F 中。 为了使 f 本质上 $\nu$ 可积，$f \circ \pi$ 本质上 $\mu$ 可积是必要且充分的，在这种情况下

$$
\int f(x)\, d\nu(x) = \int f(\pi(t))\, d\mu(t).
$$

此外，假设 $\pi$ 是连续且正确的。那么，要使 f $\nu$ 可积，$f \circ \pi$ $\mu$ 可积是充分必要的。

应用Th就足够了。 2 个§4, No. 4。

#### 推论{#int-v-s6-n2-cor-2 .statement tag=094Z}

— 为了使X的子集 A本质上$\nu$可积，$\pi^{-1}(A)$本质上$\mu$可积是必要且充分的，在这种情况下是$\nu(A) = \mu(\pi^{-1}(A))$。

特别是，对于每个紧集 $K \subset X$，$\nu(K) = \mu(\pi^{-1}(K))$。由此可见，Cor.命题 2 的第 3 条指出，如果 $\mu$ 是原子的 (§ 5, No. 10)，那么 $\pi(\mu) = \nu$ 也是原子的。对于，令 M 为 $t \in T$ 的集合，使得 $\mu(\{t\}) \neq 0$；由于$\mu$由M携带，$\nu$由$\pi(M)$携带；此外，对于每一个$x \in \pi(M)$，我们都有$\nu(\{x\}) = \mu(\pi^{-1}(x)) > 0$，因为$\pi^{-1}(x)$包含至少有M的一个点。因而$\nu$是原子的（§ 5, No. 10，命题15）。

### 3. 正测度像的性质

#### 命题 4 {#int-v-s6-prop-4 .statement tag=0950}

— 令 T、T'、T'' 为三个局部紧凑空间、$\mu$ T 的正测度、$\pi$ 将 T 的 $\mu$ 可测量映射放入 T'、将 T' 的 $\pi'$ 映射放入 T'' 以及 $\pi'' = \pi' \circ \pi$。

a) 假设$\pi$是$\mu$-真值，令$\mu' = \pi(\mu)$。为了使$\pi'$成为$\mu'$-本征，$\pi''$是$\mu$-本征是必要且充分的，在这种情况下$\pi''(\mu) = \pi'(\pi(\mu))$（“度量的像的传递性”）。

b) 假设$\pi'$是连续的，且$\pi''$是$\mu$-本征；那么$\pi$是$\mu$-本征，$\pi'$是$\pi(\mu)$-本征以及$\pi''(\mu) = \pi'(\pi(\mu))$。

在 a) 的假设下，对于 $\pi''$ $\mu$ 可测，$\pi'$ $\mu'$ 可测是充分必要的（No. 2，命题 3）。另一方面，如果$K$是$T''$的紧子集，则$\pi''(K) = \pi^{-1}(\pi'(K))$；对于$\pi''(K)$本质上$\mu$可积，$\pi'(K)$本质上$\mu'$可积是必要且充分的，由Cor.的 Th。 1. 最后，如果 $\pi''$ 是 $\mu$，那么，设定 $\mu'' = \pi''(\mu)$，对于每个函数 $f \in \mathscr{H}(T'')$，我们有，

$$
\int f(t'')\, d\mu''(t'') = \int f(\pi''(t))\, d\mu(t)
$$
$$
= \int f\left(\pi'\left(\pi(t)\right)\right)\, d\mu(t) = \int f(\pi'(t'))\, d\mu'(t')
$$

通过 Th。 No. 2 的 1，完备的 a) 的证明。

在b)的假设下，令$K'$是$T'$的紧子集。那么$K'' = \pi'(K')$是紧的，因此$\pi''(K'')$本质上是$\mu$可积，因此$\pi^{-1}(K') \subset \pi''(K'')$本质上是$\mu$可积（第IV, §5, No. 5，第7章），因此$\pi$是$\mu$-固有的。 证明然后由叙述的应用部分 a) 得出结论。

#### 推论{#int-v-s6-n3-cor-1 .statement tag=0951}

*令$T$和$T'$为两个局部紧致空间，$\mu$为$T$的正测度，$\pi$为$T$的双射映射到$T'$，以及$\pi^{-1}$的逆测度映射。假设$\pi$是$\mu$真值，并令$\mu' = \pi(\mu)$。那么 $\pi^{-1}$ 就是 $\mu'$-proper 和 $\pi^{-1}(\pi(\mu)) = \mu$。*

#### 命题 5 {#int-v-s6-prop-5 .statement tag=0952}

*Let $T$ and $X$ be two locally compact spaces, $\mu$ a positive measure on $T$, $\pi$ a $\mu$-proper mapping of $T$ into $X$, $g$ a finite numerical function $\geqslant 0$, defined on $X$ and such that $g \circ \pi$ is locally integrable for $\mu$. 在阶中，$g$ 对于 $\pi(\mu)$ 是局部可积的，$\pi$ 对于测度 $(g \circ \pi) \cdot \mu$ 是适当的，这是必要且充分的，在这种情况下*

$$
\pi((g \circ \pi) \cdot \mu) = g \cdot \pi(\mu).
$$

集合$\nu = \pi(\mu)$。对于$g$局部$\nu$可积，$gf$对于每个函数$f \in \mathscr{H}(X)$是$\nu$可积是必要且充分的；由于 $gf$ 具有紧凑支持，因此可以说 $gf$ 本质上是 $\nu$ 可积，这相当于说 $(g \circ \pi)(f \circ \pi)$ 本质上是 $\mu$ 可积（Th. 1）。但是，Th. §5, No. 3的1，这意味着$f \circ \pi$本质上对于$\rho = (g \circ \pi) \cdot \mu$是可积的，并且，到定义，这表明$\pi$是$\rho$-适当的（因为$\pi$显然是$\rho$可测的）。而且，

$$
\int fg\, d\nu = \int f(\pi(t))g(\pi(t))\, d\mu(t) = \int f(\pi(t))\, d\rho(t)
$$

(No. 2, Th. 1 和§5, Th. 1)，从而证明关系 (4)。

#### 命题 6 {#int-v-s6-prop-6 .statement tag=0953}

— 令 T 和 X 为两个局部紧致空间，$(\lambda_\alpha)_{\alpha \in A}$ T 上的一系列正测度，针对关系 $\leq$，在 $\mathscr{M}(T)$ 中承认一个上等$\mu$。在阶中，T到X的映射$\pi$是$\mu$-适当的，它对于所有$\alpha \in A$是$\lambda_\alpha$-适当的是必要和充分的，并且家庭$(\pi(\lambda_\alpha))_{\alpha \in A}$在$\mathscr{M}(X)$中被限制在上面。在这种情况下，

$$
\pi(\mu) = \sup_\alpha \pi(\lambda_\alpha).
$$

为了使 $\pi$ $\mu$ 可测，$\pi$ 对于所有 $\alpha \in A$ $\lambda_\alpha$ 可测是充分必要的（§ 1, No. 4，第 11 条命题的 Cor. 2）。假设满足这个条件；说 $\pi$ 是 $\mu$-proper 则相当于说，对于每个函数 $f \in \mathscr{K}_+(X)$，

$$
\mu^\bullet(f \circ \pi) < +\infty.
$$

现在，

$$
\int^\bullet (f \circ \pi)\, d\mu = \sup_\alpha \int^\bullet (f \circ \pi)\, d\lambda_\alpha = \sup_\alpha \int^\bullet f\, d(\pi(\lambda_\alpha))
$$

（§ 1, No. 4，提案 11）；因此，当且仅当族 $(\pi(\lambda_\alpha))$ 在 $\mathscr{M}(X)$ 中承认一个上等$\theta$时，第一个成员对于每个 $f \in \mathscr{K}_+(X)$ 都是有限的，在这种情况下，$\int (f \circ \pi)\, d\mu = \int f\, d\theta$、关系等价于 (5)。

#### 推论 1 {#int-v-s6-prop-6-cor-1 .statement tag=0954}

— 令 $(\mu_\alpha)_{\alpha \in A}$ 为 T 上的正测度的可求和族，使得 $\mu = \sum_{\alpha \in A} \mu_\alpha$；为了使 T 的映射 $\pi$ 成为局部紧致空间 X 成为 $\mu$-真值，它对于每个 $\alpha \in A$ 都是$\mu_\alpha$-真值，并且族 $(\pi(\mu_\alpha))_{\alpha \in A}$ 可求和是充分必要的。在这种情况下，

$$
\pi(\mu) = \sum_{\alpha \in A} \pi(\mu_\alpha).
$$

#### 推论 2 {#int-v-s6-prop-6-cor-2 .statement tag=0955}

— 令 T 和 X 为 T 上正测度的两个局部紧致空间、$(\lambda_i)_{1 \leq i \leq n}$ 有限序列，并令 $\mu = \sum_{i=1}^n \lambda_i$。为了使 T 到 X 的映射 $\pi$ 成为 $\mu$-真值，对于每个指标 i 来说，它是 $\lambda_i$-真值是充分必要的，在这种情况下

$$
\sum_{i=1}^n \pi(\lambda_i) = \pi\left( \sum_{i=1}^n \lambda_i \right).
$$

### 4. 复杂测度的像

令$\theta$为$T$的复测度，并令$\pi$为$T$的映射，成为局部紧凑的空间$X$；假设$\pi$是$\theta$可测的，并且对于每个$f \in \mathscr{K}(X; \mathbf{C})$，$f \circ \pi$本质上是$\theta$可积的。因为相当于说函数对于 $\theta$ 或$|\theta|$ 是可测的（或者本质上可积），这意味着 $\pi$ 是 $|\theta|$ 正确的。如果$f \in \mathscr{K}(X; \mathbf{C})$，

$$
\left| \int (f \circ \pi) \, d\theta \right| \leq \int (|f| \circ \pi) \, d|\theta| ;
$$

由此可见，$\mathscr{K}(X; \mathbf{C})$上的线性形式$f \mapsto \int (f \circ \pi) \, d\theta$是$X$上的“复杂措施”（第III, §1, No. 3，第6章），并且可以做出以下定义：

#### 定义 2 {#int-v-s6-def-2 .statement tag=0956}

*令 $\theta$ 为局部紧凑空间 $T$ 上的复杂测度。将 $T$ 的映射 $\pi$ 转换成局部紧致的空间 $X$，如果它是 $|\theta|$-本征，则被认为是 $\theta$-本征。然后，度量$f \mapsto \int (f \circ \pi) \, d\theta$ 称为$\pi$ 下$\theta$ 的像，并表示为$\pi(\theta)$.*。

然后关系 (7) 可以代入以下形式：

$$
|\pi(\theta)| \leq \pi(|\theta|) .
$$

度量$\pi(\theta)$可以是零，而$\theta$不是零，正如人们所看到的，对于$T$空间，立即减少到两个点$a, b$，对于$\theta$度量$\varepsilon_a - \varepsilon_b$，对于$\pi$是一个常数映射。

令$\theta$和$\theta'$为$T$上的两个复测度；如果 $\pi$ 是 $\theta$-proper 和 $\theta'$-proper，则可从 Cor 得出。命题 6 的第 2 条指出，自 $|\theta + \theta'| \leq |\theta| + |\theta'|$ 以来，$\pi$ 是 $(\theta + \theta')$ 真值，显然是 $\pi(\theta + \theta') = \pi(\theta) + \pi(\theta')$。

特别是，如果 $\theta$ 是实测度并且 $\pi$ 是 $\theta$-本征，那么

$$
\pi(\theta) = \pi(\theta^+) - \pi(\theta^-) .
$$

早期扩展同时建立了多项结果以进行复杂的测量；我们列举其中最重要的一些。

#### 命题 7 {#int-v-s6-prop-7 .statement tag=0957}

*令 $\theta$ 为 $T$、$\pi$ $T$ 的 $\theta$ 映射的复杂测度，转换为局部紧凑的空间 $X$、$\nu$ 像测度$\pi(\theta)$。

a) 设$A$为$X$中的子集；如果 $\overline{\pi^{-1}}(A)$ 局部 $\theta$ 可以忽略不计，则 $A$ 局部 $\nu$ 可以忽略不计。

b) 设$f$为$X$的映射为拓扑空间；如果 $f \circ \pi$ 是 $\theta$ 可测量，则 $f$ 是 $\nu$ 可测量。*

c) 设$f$为$X$上定义的函数，其中值在Banach空间$F$中；如果$f \circ \pi$本质上是$\theta$可积，那么$f$本质上是$\nu$可积，并且

$$
\int f(\pi(t))\ d\theta(t) = \int f(x)\ d\nu(x).
$$

考虑到公式 (8)，这些结果可以从 Cor 中推出。提案 2 的 2、提案 3 和 Th。 No. 2 中的 1 个。

### 5. 应用：勒贝格积分中变量的变换

令I为$\mathbf{R}$的区间（有界或无界），$a$其左端点和$b$在$\overline{\mathbf{R}}$中的右端点，以及$\mu$在I上的勒贝格测度。对于每个$\mu$可积函数$f$和每个区间$H \subset I$，左端点$\alpha$和右端点$\beta$，我们写$\int_{\alpha}^{\beta} f(t)\ dt$而不是$\int_H f(t)\ dt = \int_H f\ d\mu$，并且我们集合$\int_{\beta}^{\alpha} f(t)\ dt = -\int_{\alpha}^{\beta} f(t)\ dt$；因此赋予这些符号重合的含义与FRV、II, §§1和2中赋予它们的含义相同，当$f$是具有紧凑支持的受监管函数时（第IV, §4, No. 4、例）。

设$g$是定义在I上的数值函数并且*局部$\mu$*可积，I的$x_0$点；每$x \in I$、集合

$$
G(x) = c + \int_{x_0}^{x} g(t)\ dt \quad (c \text{ a constant}).
$$

数值函数 G 在 I 上*连续*；这立即来自勒贝格的定理（第IV, §4, No. 3，第2章的Cor.1），因为$g$的乘积以及端点$x$和$x+h$的区间特征函数趋向于可忽略不计的函数因为 $h$ 趋于 0。因此 G(I) 是 $\mathbf{R}$ 的*区间*。在这整篇文章中，我们将 G 视为 I 的映射到局部紧致空间 G(I) 上。我们用$\lambda$表示I上的度量$g \cdot \mu$。

首先假设 $g$ 是 $\mu$*-可积*。那么，与上面相同的推理表明极限$G(a+)$和$G(b-)$存在并且是*有限*；此外，测度$|\lambda|$是*有界*（§5, No. 3，Th.1的Cor.），并且I到G(I)的映射G是*$\lambda$*-本征。

#### 命题 8 {#int-v-s6-prop-8 .statement tag=0958}

*假设 g 是 $\mu$* 可积。如果 J 表示 $\mathbf{R}$ 中的开区间，端点为 $G(a+)$ 和 $G(b-)$，则测度 $g \cdot \mu$ 的 G 下的像是测度 $\varphi_J \cdot \nu$（如果 $G(a+) \leq G(b-)$）和测度 $-\varphi_J \cdot \nu$（如果 $G(a+) \geq G(b-)$）（其中$\nu$ 表示 G(I)) 上的勒贝格测度。*

足以证明，对于每个函数 $f \in \mathscr{K}(G(I))$，

$$
\int_{G(a+)}^{G(b-)} f(\xi) d\xi = \int_a^b f(G(t))g(t)\,dt.
$$

现在，这个公式已经被证明适用于$g \in \mathscr{K}(I)$（FRV，II, §2, No. 1，公式（1））。让我们转向一般情况；在 $\mathscr{K}(I)$ 中存在函数的序列 $(g_n)$，使得： $1^\circ$ 序列 $(g_n(t))$ 几乎在 $I$ 中的所有地方都趋向于 $g(t)$； $2^\circ$ 存在一个$\mu$可积函数$h \geq 0$，使得$|g_n| \leq h$对于所有$n$（第IV, §3, No. 4，第3章）。从勒贝格的定理立即可以得出，设定$G_n(x) = c + \int_{x_0}^x g_n(t)\,dt$、序列$(G_n)$在$I$上一致收敛到$G$，并且数、$G_n(a+)$和$G_n(b-)$分别倾向于$G(a+)$ 和 $G(b-)$。令$f'$为$\mathscr{K}(\mathbf{R})$中的函数，即扩展$f$；上述证明对于所有$t \in I$，$f'(G_n(t))$趋向于$f'(G(t)) = f(G(t))$； 应用勒贝格的定理，可以看出公式(12)是由公式得出的

$$
\int_{G_n(a+)}^{G_n(b-)} f'(\xi)\,d\xi = \int_a^b f'(G_n(t))g_n(t)\,dt
$$

通过极限。

#### 推论{#int-v-s6-n5-cor-1 .statement tag=0959}

*如果在 $G(I)$ 上定义函数 $\mathbf{f}$，且值在 $\overline{\mathbf{R}}$ 或 Banach 空间中，对于勒贝格测度，函数 $t \mapsto \mathbf{f}(G(t))g(t)$ 可在 $I$ 上积分，则对于勒贝格测度，$\mathbf{f}$ 可积在 $J$ 上并且*

$$
\int_{G(a+)}^{G(b-)} \mathbf{f}(\xi)\,d\xi = \int_a^b \mathbf{f}(G(t))g(t)\,dt
$$

（公式代表勒贝格积分中变量的变换）。

因为，$\mathbf{f}(G(t))$对于测度$|g|\cdot\mu$是可积的，因此对于测度$g^+\cdot\mu$和$g^-\cdot\mu$也是可积的；这是从 Th 得出的。 1 (No. 2) $\mathbf{f}$对于像测度$G(g^+\cdot\mu)$和$G(g^-\cdot\mu)$是可积的，因此对于测度$\varphi_J \cdot \nu$也是可积的，并且在考虑到第8条和公式(9)的情况下，(13)成立。

对于勒贝格测度，$\mathbf{f}$ 可在 $J$ 上积，但对于勒贝格测度，$t \mapsto \mathbf{f}(G(t))g(t)$ 不可在 $I$ 上积（Exer. 10）。

现在假设 $g$ 几乎在任何地方都保持一个*常数符号*（并且是局部 $\mu$ 可积）；人们可能会认为，对于例，$g(t) \geq 0$几乎在$I$中无处不在。那么$G$在$I$上是递增连续的函数，因此$G(a+)$和$G(b-)$存在（但可能是无限的）。此外，$G$是$I$到$G(I)$的*$\lambda$-适当*映射：因为，如果$G(b-) \in G(I)$，则存在$x_1 \geq x_0$，使得$G$对于$x \geq x_1$是常数，然后逆像在紧区间$[G(x_0), G(b-)]$的$G$是$\lambda$可积；相反，如果$G(b-) \notin G(I)$，则$G(I)$中包含的左端点为$G(x_0)$的每个紧致区间的$G$下的逆像与紧致区间至多相差$\lambda$可忽略不计的区间。对于具有右端点 $G(x_0)$、从而我们的断言的紧凑区间，人们也有类似的争论。而且：

#### 命题 9 {#int-v-s6-prop-9 .statement tag=095A}

*假设 $g \geq 0$ 和局部 $\mu$ 可积。 那么，正测度$g \cdot \mu$的$G$下的像就是$G(I)$上的勒贝格测度。 对于在 $G(I)$ 上定义的函数 $f$，以及 $\overline{\mathbf{R}}$ 或 Banach 空间中的值，要在勒贝格测度的 $G(I)$ 上可积，函数 $t \mapsto f(G(t))g(t)$ 在 $I$ 上可积是必要且充分的对于勒贝格测度，在这种情况下关系 (13) 成立。*

The first part of the statement follows from the fact that the formula (12) is valid for every function $f \in \mathscr{K}(G(I))$; for, the support of the function $t \mapsto f(G(t))$ is contained in an interval $K \subset I$ on which $g$ is integrable, by virtue of the above remarks, and it suffices to apply Prop. 8 to $K$. 第二个部分是Th的推论。 1 个No. 2。

### 6. 分解切成片。局部同胚下测度的逆像

令 $X$ 为 $X$ 的局部紧致空间、$\pi$ 映射为局部紧致空间 $T$、$\mu$ $T$ 的正测度，$\Lambda : t \mapsto \lambda_t$ 本质上为 $\mu$ 可积的标量$\mu$-可测量映射的 $T$ 到 $\mathscr{M}_+(X)$。让$\nu = \int \lambda_t d\mu(t)$。如果对于每个$t \in T$，$\lambda_t$被*$\overline{\pi}^{-1}(t)$*携带，则等式$\nu = \int \lambda_t d\mu(t)$被认为是相对于$\pi$的$\nu$的*分解切片*（或*分解*）。这个概念将在第 1 章中详细研究。 VI。

#### 命题 10 {#int-v-s6-prop-10 .statement tag=095B}

*有了上面的记号，假设$\pi$是$\nu$可测的。令 $g$ 为 $T$ 上的函数 $t \mapsto \lambda_t^*(1)$。为了使 $\pi$ 成为$\nu$-适当的，$g$ 是局部 $\mu$ 可积的充分必要，在这种情况下*

$$
\pi(\nu) = g \cdot \mu.
$$

我们首先论证假设 $g$ 是局部有限的 $\mu$——几乎无处不在；我们将在证明结束时摆脱这个辅助假设。由于 $\pi$ 是通过假设 $\nu$ 可测量的，因此说 $\pi$ 是 $\nu$ 本身就相当于说，对于每个函数 $f \in \mathscr{K}_+(T)$，$\nu^*(f \circ \pi) < +\infty$； $g$几乎在任何地方都是局部有限的，对于应用断言c），我们处于§3, No. 2第5条命题的条件之下。因此

$$
\int^\bullet (f \circ \pi)\, d\nu = \int^\bullet d\mu(t) \int^\bullet (f \circ \pi)\, d\lambda_t = \int^\bullet f(t)g(t)\, d\mu(t),
$$

因为 $\lambda_t$ 集中在 $\overline{\pi}^{-1}(t)$ 上。我们知道 $g$ 是 $\mu$ 可测量的，因为 $\Lambda$ 是 $\mu$ 足够的（§ 3, No. 1，定义 1）。因此，说第一个成员对于每个 $f \in \mathscr{K}_+(T)$ 是有限的，就等价于说，$g$ 是局部 $\mu$ 可积的（§ 5，命题 1），在这种情况下，(14) 立即从上面的关系得出。

因此只剩下消除辅助假设。如果$g$局部$\mu$可积，则$g$局部有限$\mu$-几乎处处，并且假设确实满足。让我们假设 $\pi$ 是 $\nu$ 正确的，并且让我们证明 $g$ 几乎在任何地方都是局部有限的。令$\mathfrak{K}$为紧集$K$的$\mu$稠密集合，使得$\Lambda|K$模糊连续；由于$g$是可测量的，我们简化为表明每个紧集$K \in \mathfrak{K}$使得$g|K = +\infty$是$\mu$可以忽略不计。现在，令$\mathscr{H}$为函数$h \in \mathscr{K}_+(X)$中的集合，使得$h \leq 1$； 集合$g_h(t) = \lambda_t(h)$，用$\Lambda_h$表示$\mu$-足够的映射$t \mapsto h \cdot \lambda_t$，用$\nu_h$表示$\Lambda_h$的积分，用$f$元素表示$\mathscr{K}_+(T)$这样$f \geq \varphi_K$。 应用公式 (14) 到$\Lambda_h$，其中满足辅助假设，我们得到：

$$
\int (f \circ \pi)\, d\nu \geq \int (f \circ \pi)\, d\nu_h = \int fg_h\, d\mu.
$$

但$K$上连续的函数的函数$fg_h|K$形式递增有向集合，其上包络有值$+\infty$；根据Dini的定理（GT，X, §4, No. 1，Th.1），可以选择$h$，使得$fg_h|K$大于或等于任意正数数$n$，从而得出$\int (f \circ \pi)\, d\nu \geq n\, \mu(K)$。由于第一个成员是有限的，因为 $\pi$ 是 $\nu$-proper，因此它遵循 $\mu(K) = 0$。

#### 推论 1 {#int-v-s6-prop-10-cor-1 .statement tag=095C}

— *假设 $\pi$ 是 $\nu$ 可测量。*

a) *如果$N \subset T$局部$\mu$可忽略，则$\overline{\pi}^{-1}(N)$局部$\nu$可忽略。*
b) *如果 $f$ 是 $T$ 的 $\mu$ 可测映射到拓扑空间 $G$，则 $f \circ \pi$ 是 $\nu$ 可测。*

我们再次考虑前一个证明末尾的记号$\Lambda_h$、$\nu_h$、$g_h$：$\nu_h$是每个$h \in \mathscr{H}$的有界测度，$\pi$是$\nu_h$真值，$g_h$是局部的$\mu$-可积，以及 $\pi(\nu_h) = g_h \cdot \mu$，与基 $\mu$ 的测度。 由此可见，对于测量 $\pi(\nu_h)$（§ 5, No. 3，第 3 条和第 4 条的 Cor. 1），$N$ 是局部可忽略的（即 $f$ 是可测量的）。 Consequently $\overline{\pi}^{-1}(N)$ is locally negligible (resp. $f \circ \pi$ is measurable) for the measure $\nu_h$ (Cor. 2 of

分别为 2 号提案和 2 号提案。命题 3）。最后，一个注，措施$\nu_h$形式递增指导一系列积极措施，其上限为$\nu$，并且一个适用于Cor。 §1, No. 4 提案 11 的 1（或 Cor.2）。

#### 推论 2 {#int-v-s6-prop-10-cor-2 .statement tag=095D}

*假设$\pi$是$\nu$-真；设$f$为$T$上定义的映射，值在Banach空间或$\overline{\mathbf{R}}$中。为了使$f \circ \pi$本质上$\nu$可积，$gf$本质上$\mu$可积是必要且充分的。*

考虑到第 10 号提案，这可以直接从 Th 推论出来。 §5, No. 3 和 Th 中的 1。 1 个No. 2。

#### 例 {#int-v-s6-n6-exa-1 .statement tag=095E}

— 令 $X$ 和 $T$ 为两个局部紧致空间，并令 $\pi$ 为$X$ 到 $T$* 的局部同胚。在其他字（GT，I, §11，Exer.25）中，我们假设每个点$x \in X$承认一个邻域$V$，使得$\pi|V$是$V$到$\pi(x)$邻域的同胚；如果需要替换$V$通过$x$的相对紧凑开邻域$W$使得$\overline{W} \subset V$，可以推导出$X$的相对紧凑开子集$U$的集合$\mathscr{U}$，使得$\pi|\overline{U}$ 是$\overline{U}$ 到像的同胚，是$X$ 的*开覆盖*。现在让$\mu$作为$T$的正测度；如果$U$是$\mathscr{U}$的元素，则$\pi(U)$是紧空间$\pi(\overline{U})$中的开集合，因此是$T$的局部紧子空间，并且知道如何测度定义 $\mu|\pi(U)$ 由 $\pi(U)$ 上的 $\mu$ 诱发（第 IV, §5, No. 7 章）。令$\nu_U$为$\mu|\pi(U)$在$\pi|U$逆同胚下的像；我们将证明，在 $X$ 上存在且仅有一个测度 $\nu$，即诱导在每个打开的集合 $U \in \mathscr{U}$ 上存在测度 $\nu_U$。该测度称为局部同胚$\pi$*下$\mu$的*逆像，记为$\pi^{-1}(\mu)$。

$\nu$的唯一性立即来自本地化的原理（第III, §2, No. 1章，Prop.1的Cor.）。为了建立存在性，我们注如果$t \in T$，那么每个点$x \in \pi^{-1}(t)$承认一个邻域仅在点$x$与$\pi^{-1}(t)$相交，因此$\pi^{-1}(t)$是一个*离散*子空间 $X$，并且家庭$(\varepsilon_x)_{x \in \pi^{-1}(t)}$是可求和的；我们用 $\lambda_t$ 表示它的和。接下来我们证明映射$t \mapsto \lambda_t$本质上是$\mu$可积的，并且它的积分$\nu = \int \lambda_t d\mu(t)$就是所寻求的逆像。这将立即由以下引理产生：

#### 引理 {#int-v-s6-n6-lem-1 .statement tag=095F}

— a) *令$f$为$\mathscr{K}_+(X)$中的元素； 函数$t \mapsto \lambda_t(f)$为正，上半连续，支撑紧凑，其限制至$\pi(X)$为连续。*

b) *令$U$为$\mathscr{U}$、$\nu$的元素，$\mu$可积函数$t \mapsto \lambda_t$的积分； $\pi|U$下措施$\nu|U$的像等于$\mu|\pi(U)$。*

为了建立a)，可以通过单位元的划分（第III, §1, No. 2，引理1）来实现约化到$f$的支撑$S$包含在开放的集合$U \in \mathscr{U}$中的情况。设$g$为映射$t \mapsto \lambda_t(f)$； $\pi|U$是同胚，$g|\pi(U)$属于到$\mathscr{K}_+(\pi(U))$，因而（$\pi(U)$是$\pi(X)$中的开集合）$g$到$\pi(X)$的限制是连续的。由于 $g$ 为正，并且 $g$ 到紧集 $\pi(S)$ 的限制是连续的，因此可以看出 $g$ 在 $T$ 上是上半连续的。由此可知 $g$ 是 $\mu$ 可积。

为了建立b)，用$\mathscr{K}(\pi(U))$的$g$元素，用$g^\circ$表示其扩张0到$T$，用$f$函数$g \circ (\pi|U)$，以及$f^\circ$ 扩张除$f$到$X$的0。 断言 b) 相当于等式 $\int g^\circ d\mu = \int f^\circ d\nu$。但是$f \in \mathscr{K}(U)$，因而$f^\circ \in \mathscr{K}(X)$，第二个积分因此等于$\int \lambda_t(f^\circ) d\mu(t)$。最后$\lambda_t(f^\circ) = g^\circ(t)$，完成证明。

我们现在观察到 $\pi(X)$ 在 $T$ 中是“开”的，因而$\mu$是可测的； 映射 $\Lambda : t \mapsto \lambda_t$ 是模糊的 $\mu$ 可测的，因为它的限制对于集合 $\pi(X)$ 和 $\mathbf{C}\pi(X)$ 都是模糊连续的。在这些条件下，公式 $\overline{\pi}^{-1}(\mu) = \int \lambda_t d\mu(t)$ 定义分解相对于$\pi$ 划分为 $\overline{\pi}^{-1}(\mu)$ 的切片，并且第 10 条命题产生以下结果：

#### 命题 11 {#int-v-s6-prop-11 .statement tag=095G}

*设$\pi$为局部紧致空间$X$到局部紧致空间$T$的局部同胚，并令$\mu$为$T$的正测度。如果该数是有限的，则令$n$为与$\overline{\pi}^{-1}(t)$的元素的每个$t \in T$数相关联的数值函数，反之则为$+\infty$。为了使 $\pi$ $\overline{\pi}^{-1}(\mu)$ 正确，$n$ 是$\mu$ 局部可积的充分必要，在这种情况下*

$$
\pi\left( \overline{\pi}^{-1}(\mu) \right) = n \cdot \mu .
$$

### 习题 {#int-v-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
