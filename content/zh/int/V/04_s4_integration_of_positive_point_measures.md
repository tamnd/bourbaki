---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 4
section_title: Integration of positive point measures
lang: zh
source: int-i-vi
book_pages: INT V.31-INT V.38, INT V.99
pdf_pages: 0286-0293, 0354-0354
extraction: ocr
subsections:
    - "no": 1
      title: Families of point measures
      page: 31
      pdf_page: 286
    - "no": 2
      title: Upper integrals of positive functions with respect to an integral of point measures
      page: 33
      pdf_page: 288
    - "no": 3
      title: Measurability with respect to an integral of point measures
      page: 35
      pdf_page: 290
    - "no": 4
      title: Integration of functions with values in a Banach space, with respect to an integral of point measures
      page: 37
      pdf_page: 292
statements: 10
exercises: 2
content_sha256: 792a20115abbf9b42ada35187b1d6626f34c005a1b8f5f1884e2c2b3cc60c211
translated_from: content/en/int/V/04_s4_integration_of_positive_point_measures.md
translation_method: google
source_content_sha256: dd55e7fee706c3d9d06f24460ca7220536b2e52fe66b64ab093af515c9c25f41
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: ce435c6dce8bf0a134ce5a5bafc4ff223acfbe1fe9a83a1f699c58c4ee6f9960
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。积极点措施的整合

### 1. 点措施的家庭

令X和T为两个局部紧致空间，将T的$\pi$映射转化为X，以及$g$定义在T上的有限数值函数$\geqslant 0$； T 的这两个函数定义映射 $t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)}$ 进入 X 上的度量空间 $\mathscr{M}(X)$，这样对于每个 $t \in T$，$\lambda_t$ 要么是点度量（第 III, §2, No. 4），要么等于 0。如果 $f$ 是在 X 上定义的数值函数 $\geqslant 0$，则 $\int^* f(x) d\lambda_t(x) = \int^\bullet f(x) d\lambda_t(x) = f(\pi(t))g(t)$ （回想一下我们的惯例，当 $g(t) = 0$ 和 $f(\pi(t)) = +\infty$ 时，将这个乘积设为 0）。在X上定义的每个函数（拓扑空间中的值）对于每个$t \in T$来说都是$\lambda_t$可测的。 X的每个映射$f$到Banach空间F对于所有$t \in T$和$\int f(x) d\lambda_t(x) = f(\pi(t))g(t)$来说都是$\lambda_t$可积。最后，如果$f$是在X上定义的任意数值函数，则$f$要$\lambda_t$可积，$f(\pi(t))g(t)$是有限的是必要且充分的，在这种情况下$\int f(x) d\lambda_t(x) = f(\pi(t))g(t)$。

#### 定义 1 {#int-v-s4-def-1 .statement tag=0921}

令 $\mu$ 为 T 上的正测度。如果满足以下条件，则对 $(\pi, g)$ 被称为$\mu$ 适应：
1° 函数 $\pi$ 和 $g$ 是 $\mu$ 可测量的。
2° 对于每个函数 $f \in \mathscr{K}(X)$，映射 $t \mapsto f(\pi(t))g(t)$ 本质上是 $\mu$ 可积。

#### 命题 1 {#int-v-s4-prop-1 .statement tag=0922}

如果对$(\pi, g)$是$\mu$适应的，那么T到$\mathscr{M}_+(X)$的映射$\Lambda : t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)}$基本上是标量$\mu$可积，模糊地$\mu$可测量和$\mu$足够。相反，如果$\Lambda$本质上是$\mu$可标量可积且模糊地$\mu$可测量，则函数$g$是$\mu$可测量且$\pi$到集合的限制 $t \in T$的$S$使得$g(t) \neq 0$是$\mu$可测量的。

假设对$(\pi, g)$是$\mu$适配的；对于每个函数$f \in \mathscr{K}(X)$，函数$t \mapsto \langle f, \lambda_t \rangle = f(\pi(t))g(t)$本质上是$\mu$可积的。让我们证明 $t \mapsto \lambda_t$ 是模糊可测的 $\mu$。因为，我们首先注，如果$\pi$和$g$是连续的，那么映射$t \mapsto \lambda_t$是模糊连续的。在一般情况下，紧凑子集 $K$ $T$ 的集合使得 $\pi$ 的限制和 $g$ 到 $K$ 连续，是 $\mu$ 稠密（第 IV, §5, No. 10 章，提案 1）。 15);如果$K$是这样的集合，那么$t \mapsto \lambda_t$到$K$的限制是模糊连续的，从而是叙述的第一个断言。 §3, No. 1 的命题 2 表明$\Lambda$ $\mu$ 是足够的。

相反，假设 $\Lambda$ 本质上是 $\mu$ 可积且模糊地 $\mu$ 可测；那么 $\mu$ 就足够了（§3, No. 1，提案 2）。由于函数 1 在 $X$ 上是下半连续的，函数 $t \mapsto \lambda_t(1) = g(t)$ 是 $\mu$ 可测（§3，定义 1）。因此集合 $S$ 是可测量的（第 IV, §5, No. 5 章，第 7 条命题）。 紧集 $K \subset S$的集合$\mathfrak{K}$使得$g|K$是连续的并且$\Lambda|K$是模糊连续的，在$S$中是$\mu$密集（第IV, §5, No. 10章，第15条）；如果$K \in \mathfrak{K}$，那么映射$t \mapsto \varepsilon_{\pi(t)} = \frac{1}{g(t)} \lambda_t$的限制到$K$因此是模糊连续的，这意味着$\pi|K$的连续性（第III, §1, No. 9章，第13条命题）。由于$\mathfrak{K}$在$S$中是$\mu$密集，因此$\pi$到$S$的限制是$\mu$可测。

我们将利用以下引理：

#### 引理 {#int-v-s4-n1-lem-1 .statement tag=0923}

*设$T$和$X$为两个拓扑空间、$\pi$，$T$到$X$的真连续映射（GT，I, §10, No. 1，定义1）。令$g$为$T$上定义的下半连续数值函数。对于每个$x \in X$，令$f(x)$为集合$\overline{\pi}^{-1}(x)$中函数$g(t)$的下确界（如果$\overline{\pi}^{-1}(x) = \varnothing$则下确界等于$+\infty$；cf.S，III, §1, No. 9）。那么$f$在$X$上是下半连续的。*

对于每个（有限）实数$a$，用$x \in X$的$B_a$集合表示，使得$f(x) \leq a$，并用$t \in T$的$A_a$集合表示，使得$g(t) \leq a$；这一切都归结为表明 $B_a$ 是封闭的（GT，IV, §6, No. 2，提案 1）。现在，$A_a$是封闭的（相同的参考文献），并且正确的映射$\pi$是封闭的（GT，I, §10, No. 1，提案1）；因此，我们将证明减少为 $\pi(A_a) = B_a$。对于所有$t \in T$，明显的关系$f(\pi(t)) \leq g(t)$意味着$\pi(A_a) \subset B_a$。另一方面，令 $x \in B_a$； 集合 $\overline{\pi}^{-1}(x)$ 是拟紧的 (GT, I, §10, No. 2, Th. 1) 和非空，因此存在一个 $t \in \overline{\pi}^{-1}(x)$ 使得

$$
g(t) = \inf_{u \in \pi^{-1}(x)} g(u) = f(x) \quad (\text{GT, IV, } § 6, \text{ No. 2, Th. 3}); \text{ thus } t \in A_a \text{ and } \pi(t) = x.
$$

### 2. 正函数相对于点度量的积分的上积分

我们将看到，当$(\pi, g)$是$\mu$适应的对时，可以将$§ 3$的应用命题获得的结果锐化到$t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)},$族，根据第1条，$\mu$是足够的。

#### 定理 1 {#int-v-s4-thm-1 .statement tag=0924}

*让* $(\pi, g)$ *成为$\mu$适应的对，并且让*
$$
\nu = \int g(t)\varepsilon_{\pi(t)}\, d\mu(t).
$$
*对于每个数字函数* $f \geq 0$ *在 X 上定义，* (1)
$$
\int^\bullet f(x)\, d\nu(x) = \int^\bullet f(\pi(t))g(t)\, d\mu(t).
$$

A) 首先假设测度$\mu$具有紧支持K，并且函数、$g$和$\pi$的限制到K是连续的。通过 $§ 3$、No. 1、$\nu^\bullet(1) = \int_K g(t)\, d\mu(t) < +\infty,$ 的公式 (4)，以便公式 (1) 中的所有度量都有界。因此，我们可以在第一个成员中通过 $\int^*$ 替换 $\int^\bullet$。鉴于$§ 3$、No. 2的公式(6)，一切都归结为证明(2)
$$
\int^* f(x)\, d\nu(x) \leq \int^\bullet f(\pi(t))g(t)\, d\mu(t),
$$
其中第二个成员中的符号$\int^\bullet$又可以替换为$\int^*$。由上积分定义，即可验证不等式 (3)
$$
\int^* f(x)\, d\nu(x) \leq \int^* h(t)\, d\mu(t)
$$
对于 T 上的每个下半连续函数 $h$，即 $\geq$ 函数 $t \mapsto f(\pi(t))g(t)$。现在，令 $\varepsilon$ 为数 $> 0$，并令 $u$ 为函数 $(h + \varepsilon)/g,$，它在 K 中是下半连续的。如果 $t \in \pi^{-1}(\{x\}) \cap K,$ 则 $u(t) \geq f(x):$ 这是显而易见的 if $g(t) = 0,$ 因为那么 $u(t) = +\infty;$ if $g(t) > 0,$ 那么
$$
u(t)g(t) = h(t) + \varepsilon \geq f(\pi(t))g(t) = f(x)g(t),
$$

从而所断言的不等式。在这些条件下，对于每个$x \in X$，令$v(x)$为$u(t)$对于$t \in \pi^{-1}(\{x\}) \cap K$的下确界。通过前述，函数$v$是$\geq f$，它在$X$上是引理的下半连续（适用于$\pi$到$K$的限制），并且$v(\pi(t))g(t) \leq h(t) + \varepsilon$适用于所有$t \in K$（回想一下第一个成员）按照惯例，如果$g(t) = 0$，则为零）。然后我们应用到§3, No. 1的$v$公式(4)。我们得到：

$$
\int^* f(x)\, d\nu(x) \leq \int^* v(x)\, d\nu(x)
$$
$$
= \int^* v(\pi(t))g(t)\, d\mu(t) \leq \int_K^* (h(t) + \varepsilon)\, d\mu(t)
$$
$$
= \int_K^* h(t)\, d\mu(t) + \varepsilon \mu(1).
$$

由于测度 $\mu$ 是有界的，而 $\varepsilon$ 是任意的，因此不等式 (3) 如下。

B) 现在让我们讨论一般情况。由于 $T$ 的映射 $t \mapsto (\pi(t), g(t))$ 到 $X \times \mathbf{R}_+$ 是 $\mu$ 可测量的（第 IV, §5, No. 3，第 1 章），紧凑的子集 $K$ 的集合 $\mathscr{K}$ $T$使得$\pi$和$g$到$K$的限制连续，是$\mu$稠密（第IV, §5, No. 10章，第15条）。根据§2, No. 3的第4条，$\mu$是可求和族$(\mu_\alpha)_{\alpha \in A}$测度的和，其支持度为$\mathscr{K}$中的元素； 对$(\pi, g)$针对每个$\alpha \in A$进行$\mu_\alpha$调整，让$\nu_\alpha$作为度量$\int g(t) \varepsilon_{\pi(t)}\, d\mu_\alpha(t)$。然后由A），

$$
\int^* f(x)\, d\nu_\alpha(x) = \int^* f(\pi(t))g(t)\, d\mu_\alpha(t).
$$

但是 $\nu_\alpha$ 形式是一个可求和族，其和等于 $\nu$（§3, No. 1，Prop. 1 的 Cor.）。因此，根据§2, No. 2的第1条命，

$$
\int^* f(x)\, d\nu(x) = \sum_{\alpha \in A} \int^* f(x)\, d\nu_\alpha(x).
$$

(5) 的第二个成员有一个类似的关系，因此 (1) 通过对 $\alpha$ 求和而从 (5) 得出。

#### 推论{#int-v-s4-n2-cor-1 .statement tag=0925}

— *在阶中，X的子集对于$\nu$来说在局部可以忽略不计，$\pi^{-1}(N)$的交和点$t \in T$的集合是必要且充分的，其中$g(t) > 0$在局部$\mu$可以忽略不计。*

#### 命题 2 {#int-v-s4-prop-2 .statement tag=0926}

— *令$\pi$为T到X的真连续映射（GT，I, §10, No. 1），并令g为T上的连续有限数值函数，使得$g(t) > 0$对于所有$t \in T$。 对 $(\pi, g)$ 则适用于 $\mu$，如果有集合*
$$
\nu = \int g(t) \varepsilon_{\pi(t)}\, d\mu(t),
$$

那么，对于 $X$ 上定义的每个数字函数 $f \geq 0$，

$$
\int^* f(x)\, d\nu(x) = \int^* f(\pi(t))g(t)\, d\mu(t).
$$

显然$\pi$和$g$是$\mu$可测的；此外，对于每个函数 $\psi \in \mathscr{K}(X)$，$\psi \circ \pi$ 都是连续的且有紧支撑，因为 $\pi$ 是合适的；因而，对$(\pi, g)$是$\mu$适合的，此外，映射$t \mapsto g(t)\varepsilon_{\pi(t)}$是模糊连续的。

令$h$为$T$上的下半连续函数，使得

$$
f(\pi(t))g(t) \leq h(t) \quad \text{for all } t \in T.
$$

我们将证明

$$
\int^* f(x)\, d\nu(x) \leq \int^* h(t)\, d\mu(t).
$$

通过上积分的定义，这将意味着不等式

$$
\int^* f(x)\, d\nu(x) \leq \int^* f(\pi(t))g(t)\, d\mu(t),
$$

与 §3, No. 2 的不等式 (7) 结合，可证明 (7)。

为了证明（8），让我们按以下方式在$X$上定义函数$\overline{f}$：$\overline{f}(x)$是集合$\overline{\pi}^{-1}(x)$中$h(t)/g(t)$的下确界（下确界等于$+\infty$，如果$\overline{\pi}^{-1}(x) = \varnothing$）。 函数 $\overline{f}$ 具有以下属性：

$1^\circ$ $\overline{f}(x) \geq f(x)$ 适用于所有 $x \in X$（自 $g(t) > 0$ 适用于所有 $t \in T$）。

$2^\circ$$\overline{f}(\pi(t))g(t) \leq h(t)$适用于所有$t \in T$。

由于引理、函数 $h/g$ 在 $T$ 上是下半连续，$3^\circ$ 函数 $\overline{f}$ 是下半连续。

因而，鉴于§3, No. 1的提案2a）：

$$
\int^* f(x)\, d\nu(x) \leq \int^* \overline{f}(x)\, d\nu(x) = \int^* \overline{f}(\pi(t))g(t)\, d\mu(t) \leq \int^* h(t)\, d\mu(t),
$$

成立 (8)，并完成证明。

### 3. 点测量积分的可测量性

#### 命题 3 {#int-v-s4-prop-3 .statement tag=0927}

— 令$(\pi, g)$为$\mu$改编的对，并让

$$
\nu = \int g(t)\varepsilon_{\pi(t)}\, d\mu(t).
$$

令$f$为$X$的映射进入拓扑空间$G$，并令$S$为点$t \in T$的（$\mu$可测量）集合，使得$g(t) > 0$。在$f$为$\nu$可测的阶中，$f \circ \pi$至$S$中的限制为$\mu$可测是充分必要的。

首先假设$f$是$\nu$可测的。通过$S$的紧致子集$K$的假设、集合$\mathscr{K}$，使得$\pi$到$K$的限制是连续的，在$S$中是$\mu$稠密的（第1章） IV, §5, No. 10，提案 15）。为了证明$f \circ \pi$到$S$的限制是$\mu$可测的，因此只需证明对于每个$K \in \mathscr{K}$，紧致子集$H$的$K$的集合，使得$f \circ \pi$到$H$的限制是连续的，在$K$中是$\mu$稠密的（第IV, §5, No. 8章，第13条命题）。但到假设时，存在紧集$\pi(K)$的划分，由$\nu$可忽略的集合$N$和紧集$(C_n)$的序列组成，使得限制 $f$ 到每个 $C_n$ 是连续的。 $K$的条件、$K \cap \overline{\pi}(N)$和集合$K \cap \overline{\pi}(C_n)$形式划分；但 $K \cap \overline{\pi}(N)$ 是 $\mu$——由于 Cor 的缘故，可以忽略不计。的 Th。 No. 2、集合 $K \cap \overline{\pi}(C_n)$ 的 1 是紧的，$f \circ \pi$ 的限制到后者集合是连续的，这就证明$f \circ \pi$ 到$S$ 的限制是$\mu$-可测量。

相反，假设情况是这样；为了证明$f$是$\nu$可测的，只需证明$X$的紧致子集$L$的集合$\mathscr{L}$，使得$f$到$L$的限制是连续的， $\nu$-密集（第 IV, §5, No. 10 章，第 15 条命题）。令 $N$ 为 $X$ 的子集，使得对于每个 $L \in \mathscr{L}$，$N \cap L$ $\nu$ 可以忽略不计，并且让我们证明 $N$ 局部 $\nu$ 可以忽略不计。为此，我们必须证明$\overline{\pi}(N) \cap S$在局部$\mu$可以忽略不计（No. 2的Th.1的Cor.）。现在，$S$的紧凑子集$H$的集合$\mathscr{H}$，使得$\pi$和$f \circ \pi$的限制到$H$是连续的，是由假设 $\mu$-$S$ 密集（第 IV, §5, No. 10 章，第 15 条命题）。因而，只要证明$\overline{\pi}(N) \cap H$对于每个$H \in \mathscr{H}$来说都是$\mu$，可以忽略不计。现在，$\pi(H)$是紧致的，并且可以用等价关系$\pi(t) = \pi(t')$与$H$的商空间来识别，$\pi$可以用$H$的典范映射来识别到该商空间上（GT， I, §5, No. 2，提案 3）。由于$f \circ \pi$到$H$的限制是连续的，因而$f$到$\pi(H)$的限制是连续的，在其他字$\pi(H) \in \mathscr{L}$中，因而$N \cap \pi(H)$是$\nu$可忽略不计。由科。的 Th。 No. 2、$\overline{\pi}(N \cap \pi(H)) \cap S$ 中的 1 个局部$\mu$-可以忽略不计；因此集合也是如此

$$
H \cap \overline{\pi}(N) \subset \overline{\pi}(N \cap \pi(H)) \cap S;
$$

但由于$H$是紧凑的，$H \cap \overline{\pi}(N)$是$\mu$可以忽略不计，从而完成证明。

#### 注 {#int-v-s4-n3-rem-1 .statement tag=0928}

如果 $f$ 是 $X$ 的映射变成 Banach 空间 $F$，则同样可以说 $f \circ \pi$ 到 $S$ 的限制是 $\mu$ 可测的，或者说函数 $(f \circ \pi)g$（在 $T$ 上定义）是 $\mu$ 可测量的，因为 $g$ 是 $\mu$ 可测量的，在 $S$ 中不是零，并且在 $T - S$ 上是零 （第IV, §5, No. 10，第 15 条提案）。

### 4. 将函数与值整合到 Banach 空间中，相对于点度量的积分

#### 定理 2 {#int-v-s4-thm-2 .statement tag=0929}

*设* $(\pi, g)$ *为$\mu$适应的对，并设*
$$
\nu = \int g(t) \varepsilon_{\pi(t)} \, d\mu(t).
$$
*让*$f$*定义为函数在*$X$，*与值在Banach空间*$F$*或在*$\overline{\mathbf{R}}$。 *对于* $f$ *本质上$\nu$可积，* $t \mapsto f(\pi(t))g(t)$ *本质上$\mu$可积是必要且充分的，在这种情况下*
$$
\int f(x) \, d\nu(x) = \int f(\pi(t))g(t) \, d\mu(t).
$$
*此外，假设* $\pi$ *是连续且正确的，并且* $g$ *是连续的并且使得* $g(t) > 0$ *对于所有* $t \in T$。 *那么，为了* $f$ *成为$\nu$可积，* $t \mapsto f(\pi(t))g(t)$ *成为$\mu$可积是必要且充分的。*

A) 我们首先处理测度 $\mu$ 具有紧支撑 $K$ 的情况，$g$ 是有界的。然后，测度$\mu$和$\nu$是有界的，并且可以通过“可积”将替换“本质上可积”到叙述中。假设$f$是$\nu$可积：函数$f(\pi(t))g(t)$则$\mu$可积，并且关系(9)由Th验证。 §3, No. 3 中的 1 个。相反，假设$f(\pi(t))g(t)$是$\mu$可积：那么$f$是$\nu$可测（No. 3，命题3和*注*），并且
$$
\int^\bullet |f(x)| \, d\nu(x) = \int^\bullet |f(\pi(t))|g(t) \, d\mu(t) < +\infty
$$
（No. 2，第 1）；因此，$f$本质上是$\nu$可积（§1, No. 3，命题9），因此$\nu$可积。 Th。 §3, No. 3 中的 1 意味着 (9)。

B) 让我们讨论一般情况。令 $\mathscr{K}$ 为 $T$ 的紧凑子集 $K$ 的集合，使得 $g|K$ 是连续的：$\mathscr{K}$ 是 $\mu$ 稠密（第 IV, §5, No. 10 章，第 15 条），因此测度 $\mu$ 为一个家庭的$(\mu_\alpha)_{\alpha \in A}$措施的和，其支持是$\mathscr{K}$中的元素（§2, No. 3，提案4）。 对$(g, \pi)$显然对每个$\alpha \in A$进行$\mu_\alpha$调整，并且度量$\nu$是度量家族$\nu_\alpha = \int \varepsilon_{\pi(t)}g(t) \, d\mu_\alpha(t)$的和（§3, No. 1，第1条的Cor.）。由于A)的论证可以应用于措施$\mu_\alpha, \nu_\alpha$，叙述的第一个部分则由§2, No. 2的命题3得出。

对于函数$f$（或$t \mapsto f(\pi(t))g(t)$）对于$\nu$（或$\mu$）可积，它本质上可积是必要且充分的，并且

$$
\int^* |f(x)| d\nu(x) < +\infty \quad (\text{resp. } \int^* |f(\pi(t))|g(t)\,d\mu(t) < +\infty ).
$$

因此，叙述的第二个部分源自第一个部分和命题2。

#### 注 {#int-v-s4-n4-rem-1 .statement tag=092A}

— Let $(\pi, g)$ be a $\mu$-adapted pair, $\pi'$ a mapping of T into X, and $g'$ a finite numerical function $\geq 0$ defined on T, such that $\pi'$ (resp. $g'$) is equal to $\pi$ (resp. $g$) locally almost everywhere for $\mu$. 那么对$(\pi', g')$是$\mu$自适应的，$\lambda_t = g(t)\varepsilon_{\pi(t)}$和$\lambda'_t = g'(t)\varepsilon_{\pi'(t)}$几乎处处局部相等，以及$\int g(t)\varepsilon_{\pi(t)}\,d\mu(t) = \int g'(t)\varepsilon_{\pi'(t)}\,d\mu(t)$。 如果现在 $\pi'$ 和 $g'$ 几乎在所有地方都仅在本地定义（对于 $\mu$），并且如果存在$\mu$ 适应的对 $(\pi, g)$，使得 $\pi'$（分别为 $g'$）等于 $\pi$（分别为 $g$）本地几乎所有地方，有人再次说对$(\pi', g')$是$\mu$适合的，还有一个是集合

$$
\int g'(t)\varepsilon_{\pi'(t)}\,d\mu(t) = \int g(t)\varepsilon_{\pi(t)}\,d\mu(t)
$$

（cf.§3, No. 3，*注*）。第叙述。当仅假设 $\pi$ 和 $g$ 几乎在所有地方都被本地定义时，命题 1 和 2 以及命题 3 仍然有效。

### 习题{#int-v-s4-exercises}

§ 4](exercises/s4/)参见[习题。
