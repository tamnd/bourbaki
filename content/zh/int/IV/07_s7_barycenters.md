---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 7
section_title: Barycenters
lang: zh
source: int-i-vi
book_pages: INT IV.142-INT IV.148
pdf_pages: 0208-0225, 0249-0255
extraction: ocr
subsections:
    - "no": 1
      title: Definition of barycenters
      page: 101
      pdf_page: 208
    - "no": 2
      title: Extremal points and barycenters
      page: 102
      pdf_page: 209
    - "no": 3
      title: 'Applications: I. Vector spaces of continuous real functions'
      page: 106
      pdf_page: 213
    - "no": 4
      title: 'Applications: II. Vector spaces of continuous complex functions'
      page: 110
      pdf_page: 217
    - "no": 5
      title: 'Applications: III. Algebras of continuous functions'
      page: 111
      pdf_page: 218
    - "no": 6
      title: Uniqueness of integral representations
      page: 115
      pdf_page: 222
statements: 31
exercises: 10
content_sha256: 35239c8d0fc02dd4661e7b491a6fc0b09c4708520e68d10a504e71de8b5183f2
translated_from: content/en/int/IV/07_s7_barycenters.md
translation_method: google
source_content_sha256: a0b29318ee51bbadb84b433570743b81dc51c686140364de87fd714982b23900
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: abe05df311fcfcf6dba0226da04f16b4b7e2d3e9c085970b00f3cbb881d710a6
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 7。重心

### 1. 定义重心

令 E 为 $\mathbf{R}$ 上的 Hausdorff 局部凸空间，$E'$ 其对偶，${E'}^*$ $E'$ 的代数对偶，E 被规范地识别为 ${E'}^*$ 的线性子空间。令 K 为 E 的紧子集； K 的典范嵌入到 E 中是连续的且有紧支撑，因此对于 K 上的每个测度 $\mu$，整的 $\int x\, d\mu(x)$ 被定义并且是 ${E'}^*$ 的元素（第 III, §3, No. 1）。而且，在K上，弱拓扑$\sigma({E'}^*, E')$诱发的拓扑与原来的拓扑相同。最后，如果C是配备$\sigma({E'}^*, E')$的${E'}^*$中K的闭凸包络，则对于原始拓扑（或弱化的拓扑$\sigma(E, E')$），$C \cap E$是E中K的闭凸包络。

#### 定义 1 {#int-iv-s7-def-1 .statement tag=08YJ}

*令 K 为 Hausdorff 局部凸空间 E 的紧子集。对于总质量等于 1 的 K 上的每个正测度 $\mu$，向量 $b_\mu = \int x\, d\mu(x)$（属于到 ${E'}^*$）称为 $\mu$ 的重心。*

#### 例{#int-iv-s7-n1-exa-1 .statement tag=08YK}

— 令 $\mu$ 为 K 的*离散*测量值，正数且总质量为 1；因此，它是形式$\mu = \sum_{i=1}^n \lambda_i \varepsilon_{x_i}$，其中$x_i \in K$和$\lambda_i$是实数，使得$\lambda_i \geq 0$对于所有$i$和$\sum_{i=1}^n \lambda_i = 1$。从$\int x\, d\varepsilon_y(x) = y$（第III, §3, No. 1，*例 3*）开始，$b_\mu = \int x\, d\mu(x) = \sum_i \lambda_i x_i$。特别是，对于每个 $x \in K$，x 是度量 $\varepsilon_x$ 的重心。

#### 命题 1 {#int-iv-s7-prop-1 .statement tag=08YL}

*设 E 为 Hausdorff 局部凸空间，K 为 E 的紧凑子集，C E 中 K 的封闭凸包络线。集合 C 那么由 E 的点组成，这些点是 K 上质量 1 的至少一个正测量的重心。*

这只不过是第 5 章的提案 5。将III, §3, No. 2应用于K的典范嵌入到E中。

#### 推论{#int-iv-s7-n1-cor-1 .statement tag=08YM}

*如果 E 中 K 的闭凸包络C 是紧的，则 K 属于到 E 上总质量 1 的每个正测量的重心。*

因为，C 也是 ${E'}^*$ 中 K 的闭凸包络，配备了弱拓扑 $\sigma(E', E')$，并且足以将 K 的典范嵌入应用到 E 第 4 章的 Prop. 4 中。 III, §3, No. 2。

#### 注 {#int-iv-s7-n1-rem-1 .statement tag=08YN}

科。当 K 是凸的或者 E 是准完备的时候，命题 1 的特别适用。

#### 命题 2 {#int-iv-s7-prop-2 .statement tag=08YO}

— 令 K 为 Hausdorff 局部凸空间 E 的紧凸子集，$\mu$ K 上总质量 1 的正测量，$b_\mu$ 其重心。对于 K 上的下半连续的每个凸数值函数 $f \geq 0$，
$$
f(b_\mu) \leq \int^* f d\mu.
$$
已知（TVS，II, §5, No. 4，命题 5）$f$ 是连续仿射线性函数 $h_\alpha : x \mapsto c_\alpha + \langle x, z'_\alpha \rangle$ 的限制到 K 族的上包络线。然后
$$
\int h_\alpha(x) d\mu(x) \leq \int^* f(x) d\mu(x)
$$
每$\alpha$；现在，$\int h_\alpha(x) d\mu(x) = c_\alpha + \int \langle x, z'_\alpha \rangle d\mu(x)$ 自 $\mu$ 的总质量为 1；但是 $\int \langle x, z'_\alpha \rangle d\mu(x) = \langle b_\mu, z'_\alpha \rangle$ 乘以重心定义。因此$\sup_\alpha \int h_\alpha(x) d\mu(x) = \sup_\alpha h_\alpha(b_\mu) = f(b_\mu)$、从而结论。

当 $\mu$ 是总质量 1 的 K 上的离散正测度时，命题 2 重新产生不等式，即定义 K 上的凸函数。

#### 推论{#int-iv-s7-n1-cor-2 .statement tag=08YP}

— 对于 K 上的每个有界且下半连续的凸数值函数函数 g，$g(b_\mu) \leq \int g d\mu$。

只要 $\inf_{x \in K} g(x) = a$ 是有限的，就足以满足注的要求，并应用第 2 条命题到 $g - a$。

### 2. 极值点和重心

#### 命题 3 {#int-iv-s7-prop-3 .statement tag=08YQ}

— 令 K 为 Hausdorff 局部凸空间 E 的紧凸子集，K 的 x 点。总质量 1 的 K（正）上的每个测量 $\mu$，并承认 x 作为重心，都位于承认 x 作为重心的总质量 1 的离散正测量的集合的模糊闭包中。

对于模糊拓扑，令U为$\mu$的邻域；我们可以假设 U 由 K 上的测量 $\nu$ 组成，使得
$$
|\mu(f_i) - \nu(f_i)| \leq \delta
$$
对于函数 $f_i \in \mathscr{C}(K; \mathbf{C})$ ($1 \leq i \leq p$) 和数 $\delta > 0$ 的有限数。对于每个点 $a \in K$，E 中存在一个闭凸邻域 $V_a$ 0，使得
$$
|f_i(y) - f_i(a)| \leq \delta/2
$$

for $1 \leq i \leq p$ and for every $y \in W_a = K \cap (a + V_a)$.由于$K$是紧致的，因此存在$K$的点$a_j$（$1 \leq j \leq r$）的有限数，使得$W_{a_j}$形式覆盖$K$（$1 \leq j \leq r$）。 Consider a continuous 划分 of 单位元 $(g_j)_{1 \leq j \leq r}$ on $K$, subordinate to the covering $(W_{a_j})$, and 集合 $\alpha_j = \mu(g_j)$ for all $j$; if $\alpha_j \neq 0$ 集合 $\mu_j = \alpha_j^{-1} g_j \cdot \mu$, and if $\alpha_j = 0$ 集合 $\mu_j = \varepsilon_{a_j}$.每个度量$\mu_j$都是正数，总质量为1，其支撑包含在紧凸凸集合$W_{a_j}$中；此外，通过定义，

$$
\mu = \sum_{j=1}^r \alpha_j \mu_j
$$

since $g_j \cdot \mu = 0$ if $\mu(g_j) = 0$; the $\alpha_j$ are $\geq 0$ and

$$
\sum_{j=1}^r \alpha_j = \sum_{j=1}^r \mu(g_j) = \mu \left( \sum_{j=1}^r g_j \right) = \mu(1) = 1 .
$$

令$x_j$为$\mu_j$的重心，其中属于到$W_{a_j}$（No. 1，命题1），并考虑离散测度$\nu = \sum_{j=1}^r \alpha_j \varepsilon_{x_j}$；它是正数，总质量为1，其重心为$\sum_{j=1}^r \alpha_j x_j$，根据式(3)，它也是$\mu$的重心，因此等于$x$。 Moreover, by (2), $|f_i(y) - f_i(a_j)| \leq \delta/2$ for all $y \in W_{a_j}$ and for all $i$, 从而, since $\operatorname{Supp}(\mu_j) \subset W_{a_j}$, $|\mu_j(f_i) - f_i(a_j)| \leq \delta/2$ for $1 \leq i \leq p$. On the other hand, since $x_j \in W_{a_j}$, one also has

$$
|\varepsilon_{x_j}(f_i) - f_i(a_j)| \leq \delta/2
$$

对于 $1 \leq i \leq p$、从而 $|\mu_j(f_i) - \varepsilon_{x_j}(f_i)| \leq \delta$ 对于所有 $i$ 和 $j$。 Since the $\alpha_j$ are $\geq 0$ and have 和 1, it follows from (3) and 定义 of $\nu$ that $\nu$ satisfies 不等式 (1).

Q.E.D.

#### 推论{#int-iv-s7-n2-cor-1 .statement tag=08YR}

— *Let $K'$ be a compact 子集 of $K$ such that $K$ is the closed convex envelope of $K'$.在阶中，$x \in K'$是$K$的极值点，$\varepsilon_x$是总质量为1、以$x$为重心的$K'$上的唯一正测度是必要且充分的。*

假设$x$是$K$的极值点；为了证明 $\varepsilon_x$ 是总质量为 1 的 $K'$ 上唯一的正测量，以 $x$ 作为重心，根据命题 3，只要看到*离散*的集合在 $K'$ 上的测量$\nu$ 是正的，总质量为 1，且 $x$ 为重心，约化至 $\varepsilon_x$。但这样的测度$\nu$是形式$\sum_{i=1}^r \lambda_i \varepsilon_{x_i}$，$\lambda_i > 0$代表$1 \leq i \leq r$和$\sum_{i=1}^{r} \lambda_i = 1$，假设$x$是$\nu$的重心可以写成$x = \sum_{i=1}^{r} \lambda_i x_i$。由于$x$是极值，这意味着$x_i = x$对于所有$i$，从而$\nu = \varepsilon_x$。

相反，让我们假设 $\varepsilon_x$ 是总质量为 1 的 $K'$ 的唯一正测度，以 $x$ 作为重心，并让我们证明 $x$ 是极值。相反的情况下，将存在$K$和实数$\lambda$的两个不同的点$x', x''$，使得$0 < \lambda < 1$和$x = \lambda x' + (1 - \lambda) x''$。根据命题 1，$x'$（或$x''$）是总质量 1 的 $K'$ 上的正测度 $\mu'$（或$\mu''$）的重心。则 $x$ 是 $\lambda \mu' + (1 - \lambda) \mu''$ 的重心。因此$\lambda \mu' + (1 - \lambda) \mu'' = \varepsilon_x$。因此$\mu'$和$\mu''$与$\varepsilon_x$、从而$x' = x'' = x$成正比，这是荒谬的。

#### 定理 1（巧克力）{#int-iv-s7-thm-1 .statement tag=08YS}

— *令 E 为 $\mathbf{R}$ 上的 Hausdorff 局部凸空间，K 为 E 的可度量紧凸子集，M 集合为 K 的极值点。集合 M 为可数开集合族的交，其中K，并且 K 的每个点都是 K 上度量 $\mu$ 的重心，使得 $\mu(K - M) = 0$。*

为了证明第一个断言，用I表示$\mathbf{R}$的区间$[0, 1]$；由于 K 是紧凑且可度量的，因此 $K \times K \times I$ 也是如此；由三元组$(x, y, \lambda)$构成$K \times K \times I$的子集 U，使得$x \neq y$和$0 < \lambda < 1$在$K \times K \times I$中开，因此在$K \times K \times I$中存在闭集合的序列$(F_n)$，其并是U （GT，IX, §2, No. 5，提案 7）。由$q(x, y, \lambda) = \lambda x + (1 - \lambda) y$定义的映射$q : K \times K \times I \to K$是连续的，并且由极值点的定义，$K - M = q(U) = \bigcup_n q(F_n)$；但 $F_n$ 是紧的，因为它在 $K \times K \times I$ 中是闭的，因此 $q(F_n)$ 是紧的，因此在 K 中是闭的；因此，集合 $U_n = K - q(F_n)$ 在 K 中开，我们有 $M = \bigcap_n U_n$。

在证明的延续中，我们将用$u$表示K上的连续且*凸*数值函数，用$G \subset E \times \mathbf{R}$表示$u$的图，并用S表示$E \times \mathbf{R}$中G的*封闭凸包络*。

#### 引理 1 {#int-iv-s7-lem-1 .statement tag=08YT}

— *令 $\overline{u}$ 为 E 上的连续仿射线性函数的下包络，其为 K 上的 $\geq u$。则 S 为点 $(a, b) \in E \times \mathbf{R}$ 的集合，使得 $a \in K$ 和 $u(a) \leq b \leq \overline{u}(a)$。*

根据Hahn-Banach 定理，对于$(a, b)$到属于到S，对于$E \times \mathbf{R}$上的每个连续仿射线性函数$h$，$h(a, b) \geq 0$是必要且充分的，使得$h(x, u(x)) \geq 0$对于$x \in K$。 设定$h(x, t) = f(x) - \lambda t$，其中$f$是E上的连续仿射线性函数，我们看到关系$(a, b) \in S$等价于以下性质：关系

$$
f(x) \geq \lambda u(x) \quad \text{for all } x \in K
$$

意味着

(5)
$$
f(a) \geq \lambda b .
$$

首先集合$\lambda = 0$； (4) 蕴含 (5) 的事实对于 $E$ 上的每个连续仿射线性函数 $f$ 等价于 Hahn-Banach 定理的关系 $a \in K$。接下来，集合$\lambda = -1$和替换$f$乘$-f$；那么$K$中的关系$f(x) \leq u(x)$必然隐含$f(a) \leq b$。但由于 $u$ 在 $K$ 上是凸且连续的，$u(a)$ 等于 $f(a)$ 的上界，对于 $E$ 上的连续仿射线性函数 $f$，使得 $f(x) \leq u(x)$ 在 $K$ 上（TVS， II, §5, No. 4，提案 5)；因此我们得到关系$b \geq u(a)$。最后，集合$\lambda = 1$；如果说 (4) 蕴含 (5)，那么通过定义就意味着 $b \leq \overline{u}(a)$。这证明了引理，因为关系 (4)（或(5)）等价于两边都乘以标量$> 0$。

#### 引理 2 {#int-iv-s7-lem-2 .statement tag=08YU}

*If $u$ is strictly convex on $K$, then $u(x) < \overline{u}(x)$ for every non-extremal point $x$ of $K$.*

因为，$K$存在两个不同的点$y, z$，使得$x = (y + z)/2$、从而$u(x) < (u(y) + u(z))/2$，因为$u$是严格凸的。如果$f$是$E$上的仿射线性函数，则$f(x) = (f(y) + f(z))/2$；将应用这个关系代入$K$上$\geq u$的连续仿射线性函数$f$，我们得到

$$
\overline{u}(x) \geq (\overline{u}(y) + \overline{u}(z))/2 \geq (u(y) + u(z))/2 > u(x) .
$$

这些引理成立，因此我们（引理1）对于所有$a \in K$有$(a, \overline{u}(a)) \in S$。 Since $G$ is compact, being the image of $K$ under the continuous mapping $x \mapsto (x, u(x))$, there exists, by Prop. 1 of No. 1, a positive measure $\nu$ on $G$, of total mass 1 , having $(a, \overline{u}(a))$ as barycenter. 由于投影 $pr_1$ 到 $G$ 的限制是 $G$ 到 $K$ 的同胚，因此测度 $\nu$ 可以通过该同胚传输，从而在 $K$（正且总质量为 1 ）上产生测度 $\mu$，使得

(6)
$$
a = \int x \, d\mu(x) \quad \text{and} \quad \overline{u}(a) = \int u(x) \, d\mu(x) .
$$

关系 (6) 中的第一个表示$a$ 是$\mu$ 的重心。 函数 $\overline{u}$ 是上半连续且有界于 $K$，因此是 $\mu$ 可积（§4, No. 4，第 5 条命题的 Cor. 1）；此外，由于函数 $-\overline{u}$ 是定义凸的，所以根据 Cor，我们有： No. 1第2号提案，

(7)
$$
\overline{u}(a) \geq \int \overline{u}(x) \, d\mu(x) ,
$$

从而，与公式(6)中的第二个比较，

$$
\int u(\mathbf{x})\, d\mu(\mathbf{x}) \geq \int \overline{u}(\mathbf{x})\, d\mu(\mathbf{x}) .
$$

但由于$u(\mathbf{x}) \leq \overline{u}(\mathbf{x})$在K上，关系(8)意味着$u(\mathbf{x}) = \overline{u}(\mathbf{x})$几乎处处对于$\mu$。考虑到引理 2，一旦建立了引理，就可以证明定理 1：

#### 引理 3 {#int-iv-s7-lem-3 .statement tag=08YV}

*设E是$\mathbf{R}$上的豪斯多夫局部凸空间，K是E的可度量紧凸子集。那么，K上存在严格凸数值函数。*

For, the Banach 空间 $\mathscr{C}(K; \mathbf{R})$ is separable (GT, X, §3, No. 3, Th. 1), therefore so is 子空间 $\mathscr{A}$ of $\mathscr{C}(K; \mathbf{R})$ formed by 限制 to K of the *continuous affine linear 函数 on* E. Thus let $(h_n)$ 是序列稠密于 $\mathscr{A}$，并设 $\alpha_n > \sup_{\mathbf{x} \in K} |h_n(\mathbf{x})|$。 Then each of 函数 $h_n^2 / n^2 \alpha_n^2$ is convex in K (TVS, II, §2, No. 8, *例*), and 级数 with general 项 $h_n^2 / n^2 \alpha_n^2$ is normally convergent, therefore its 和 $u$ is continuous and convex in K. It remains to see that $u$ is strictly convex, and for this it suffices to prove that for any two distinct 点 $\mathbf{x}, \mathbf{x}'$ of K, there is 整数 $n$ such that 限制 of $h_n^2$ to the segment with endpoints $\mathbf{x}, \mathbf{x}'$ is strictly convex;但为此，$h_n(\mathbf{x}) \neq h_n(\mathbf{x}')$就足够了（*loc.cit.*）。 Now, there exists 函数 $h \in \mathscr{A}$ such that $h(\mathbf{x}) \neq h(\mathbf{x}')$ (TVS, II, §4, No. 1, Cor. 1 of Prop. 2) and since 序列 $(h_n)$ is dense in $\mathscr{A}$, there exists an $n$ such that $h_n(\mathbf{x}) \neq h_n(\mathbf{x}')$.

Q.E.D.

#### 推论{#int-iv-s7-n2-cor-2 .statement tag=08YW}

*Let E be a Hausdorff locally convex 空间 over $\mathbf{R}$, C a proper convex cone in E with vertex 0, that is complete and metrizable for the uniform 结构 induced by the weakened uniform 结构 of E. Let M be 并 of the extremal 生成元 C。 For every $\mathbf{x} \in C$ there exist a compact convex 子集 K of C and a measure $\lambda \geq 0$ on K of total mass 1, such that $K - (M \cap K)$ is $\lambda$-negligible and the barycenter of $\lambda$ is equal to $\mathbf{x}$.

For, $\mathbf{x}$ 属于 to a cap K of C (TVS, II, §7, No. 2, Prop. 5), and $M \cap K$ 包含集合 of extremal 点 of K (*loc. cit.*, Cor. 1 of Prop. 4）。然后应用 Th 就足够了。 1.

### 3. 应用：I。连续实数向量空间函数

Let X be 非空 compact 空间, $\mathscr{H}$ a linear 子空间 of the Banach 空间 $\mathscr{C}(X; \mathbf{R})$ that 包含 the constants and *separates* 点 of X （GT，X, §4, No. 1，默认 1）。我们为$\mathscr{H}$配备由$C(X; \mathbf{R})$诱导的范数空间拓扑，并用$\mathscr{H}'$表示该范数空间的对偶。 For every $x \in X$, 映射 $f \mapsto f(x)$ is a continuous 线性形式 on $\mathscr{H}$ (限制 to $\mathscr{H}$ of the Dirac measure $\varepsilon_x$), thus is 元素 of $\mathscr{H}'$ that will be表示为 $i_{\mathscr{H}}(x)$，因此

$$
\langle f, i_{\mathscr{H}}(x) \rangle = f(x)
$$

对于每个函数$f \in \mathscr{H}$和每个$x \in X$。

当$\mathscr{H}'$配备弱拓扑$\sigma(\mathscr{H}', \mathscr{H})$时，X到$\mathscr{H}'$的映射$i_{\mathscr{H}}$是单射且连续的；第二个断言紧接在定义和(9)之后； as for the first, 注 that if $x, x'$ are two distinct 点 of X, by 假设 there exists 函数 $h \in \mathscr{H}$ such that $h(x) \neq h(x')$, therefore, by (9), $\langle h, i_{\mathscr{H}}(x) \rangle \neq \langle h, i_{\mathscr{H}}(x') \rangle$ and *更不必说*$i_{\mathscr{H}}(x) \neq i_{\mathscr{H}}(x')$。 像 $i_{\mathscr{H}}(X)$ is therefore a *compact* 子集 of $\mathscr{H}'$ (for the weak 拓扑), and $i_{\mathscr{H}}$ is a *homeomorphism* of X onto $i_{\mathscr{H}}(X)$.

#### 命题 4 {#int-iv-s7-prop-4 .statement tag=08YX}

(i) *闭凸包络* C *of* $i_{\mathscr{H}}(X)$ *in* $\mathscr{H}'$ *（对于弱拓扑* $\sigma(\mathscr{H}', \mathscr{H})$）*是紧凑的*。

(ii) *对于点* $i_{\mathscr{H}}(x)$ *作为* C 的极值点，*唯一的正测量* $\lambda$ *在* X *上是必要且充分的*

$$
h(x) = \int h \, d\lambda
$$

*对于每个函数* $h \in \mathscr{H}$（这特别意味着$\lambda$的总质量为1，因为$1 \in \mathscr{H}$）*是狄拉克测度*$\varepsilon_x$。

由此可见，对于每个$h \in \mathscr{H}$，C上的函数$z' \mapsto \langle h, z' \rangle$至少在C的一个极值点处达到其极值（TVS，II, §7, No. 1，命题1），并且这个点属于至 $i_{\mathscr{H}}(X)$（*loc. cit.*，Cor. of Prop. 2）。

(i) 根据(9)，$\| i_{\mathscr{H}}(x) \| \leq 1$在范数空间$\mathscr{H}'$中，在其他字$i_{\mathscr{H}}(X)$中是有界的，并且断言从$\mathscr{H}'$配备弱拓扑$\sigma(\mathscr{H}', \mathscr{H})$的事实得出，是*准完整*（TVS，III, §4, No. 2，Th.1 的 Cor.5）。

(ii) 质量 1 在 $i_{\mathscr{H}}(X)$ 上的每一个正测度 $\mu$，通过结构的迁移，通过同胚 $i_{\mathscr{H}}$，由质量 1 在 X 上的正测度 $\lambda$ 产生，狄拉克测度 $\varepsilon_{i_{\mathscr{H}}(x)}$ 产生于$\varepsilon_x$。说$\mu$承认$i_{\mathscr{H}}(x)$作为重心意味着，通过定义，

$$
\int_X \langle h, i_{\mathscr{H}}(z) \rangle \, d\lambda(z) = \langle h, i_{\mathscr{H}}(x) \rangle
$$

每函数$h \in \mathscr{H}$。考虑到(9)，断言(ii)只是No. 2标准的翻译，Cor.根据第 3 条命题，$i_{\mathscr{H}}(x)$ 是 C 的极值点。

我们可以说，第 4 条命题的点 $x \in X$ 满足条件 (ii) 是$\mathscr{H}$-极值；我们用$\mathrm{Ch}_{\mathscr{H}}(X)$（或简称为$\mathrm{Ch}(X)$）集合表示这些点，并用$\check{S}_{\mathscr{H}}(X)$（或简称为$\check{S}(X)$）表示$X$中的$\mathrm{Ch}_{\mathscr{H}}(X)$的闭包。

#### 命题 5 {#int-iv-s7-prop-5 .statement tag=08YY}

*每个函数* $h \in \mathscr{H}$ *至少达到一个* $\mathscr{H}$*-极值点*。

令$x$为$X$中的点，$h$函数在$\mathscr{H}$中。对于所有$z \in X$，关系$h(z) \leq h(x)$ 对于所有$z \in X$，可以写成$\langle h, i_{\mathscr{H}}(z) \rangle \leq \langle h, i_{\mathscr{H}}(x) \rangle$，因此意味着$\mathscr{H}'$的弱闭超平面与方程$\langle h, t' \rangle = \langle h, i_{\mathscr{H}}(x) \rangle$是一个*支持超平面* $i_{\mathscr{H}}(X)$。已知（TVS，II, §7, No. 1，Prop. 1），这样的超平面包含至少有一个$i_{\mathscr{H}}(X)$的封闭凸包络的极值点，并且这样的点$i_{\mathscr{H}}(y)$是一个像 $\mathscr{H}$-极值点 $y$ by 定义；因此$h(y)$等于$h$在$X$中的上界。

#### 命题 6 {#int-iv-s7-prop-6 .statement tag=08YZ}

*对于每个点* $x \in X$，*以下属性是等效的*：

a) $x$ *是* $\mathscr{H}$*-极值*。

b) *对于每个开放邻域* $U$ ** $x$ *在* $X$ *和每个* $\varepsilon > 0$，*存在函数* $h \geq 0$ *在* $\mathscr{H}$ *这样* $h(x) \leq \varepsilon$ *和* $h(y) \geq 1$ *对于每个* $y \in X - U$。

令$x$为$\mathscr{C}(X; \mathbf{R})$中$X$、$f$函数中的任意点；已知（TVS，II, §3, No. 1，命题 1）数 $\lambda(f)$ 的下确界，对于 $X$ 上的所有正测量，使得对于每个函数 $h \in \mathscr{H}$，$\lambda(h) = h(x)$ 等于数的上界$h(x)$，其中$h$超过函数$h \in \mathscr{H}$的集合，从而得到$h \leq f$。假设$x$是$\mathscr{H}$-极值；然后根据命题 4，(ii) 对于每一个函数 $f \in \mathscr{C}(X; \mathbf{R})$，

$$
f(x) = \sup_{h \in \mathscr{H}, h \leq f} h(x).
$$

为了证明 *a)* 蕴含 *b)*，我们将 $f$ 取 $X$ 的连续映射放入 $[0, 1]$，并在 $U$ 中包含支持，使得 $f(x) = 1$；那么，根据(11)，存在函数$h' \in \mathscr{H}$使得$h' \leq f$和$h'(x) \geq 1 - \varepsilon$。由于$1 \in \mathscr{H}$，函数$h = 1 - h'$满足*b)*的条件。

反之，假设条件 *b)* 被验证；这个条件意味着$1 - h \leq \varphi_U$；对于 $X$ 满足条件 (10) 上的每一个积极措施$\lambda$，我们因此有

$$
\lambda(U) = \lambda(\varphi_U) \geq \lambda(1 - h) = 1 - h(x) \geq 1 - \varepsilon.
$$

因为，到假设，这个关系适用于每个$\varepsilon > 0$以及$x$的每个开放邻域$U$，因此

$$
\lambda(\{x\}) = \inf_U \lambda(U) \geq 1 - \varepsilon
$$

对于每个$\varepsilon > 0$，因此$\lambda(\{x\}) = 1$。由于 $\lambda$ 为正且总质量为 1，必然为 $\lambda = \varepsilon_x$，根据命题 4 (ii)，证明 $x$ 是 $\mathscr{H}$-极值。

#### 命题 7 {#int-iv-s7-prop-7 .statement tag=08Z0}

*设 F 为 X 的闭子集。以下属性是等效的：*

a) *F 包含于 $\check{S}_{\mathscr{H}}(X)$.*

b) *对于每个函数 $h \in \mathscr{H}$，集合 F 与 X 的点的集合相交，其中 h 达到其最高值。*

c) *对于每个点 $x \in X$，在 X 上存在总质量 1 的正测量值 $\mu$，使得每个函数 $h \in \mathscr{H}$ 都有 $\operatorname{Supp}(\mu) \subset F$ 和 $h(x) = \int h \, d\mu$。*

让$G = i_{\mathscr{H}}(F)$。 条件 *a)* 表示 C 的极值点的 G 包含集合。 条件 *b)* 表示 G 满足$i_{\mathscr{H}}(X)$ 的交与$i_{\mathscr{H}}(X)$ 的每个闭支撑超平面。最后，条件 *c)* 表示$i_{\mathscr{H}}(X)$的每个点都是G中包含支持的测度的重心；根据命题 1 No. 1，这也相当于说，$i_{\mathscr{H}}(X)$ 的闭凸包络等于 G 的闭凸包络。因此，条件 *a)*、*b)* 和 *c)* 的等价由 TVS、II, §7, No. 1、Cor 得出。提案 2。

#### 命题 8 {#int-iv-s7-prop-8 .statement tag=08Z1}

*假设X是可度量的。那么X的$\mathscr{H}$-极值点的集合$\operatorname{Ch}_{\mathscr{H}}(X)$是X中开集合可数族的交，并且对于每个$x \in X$，存在总质量1的正测度$\mu$ X 这样*

$$
\mu(X - \operatorname{Ch}_{\mathscr{H}}(X)) = 0 \quad \text{and} \quad \int h \, d\mu = h(x)
$$

*对于每个$h \in \mathscr{H}$。*

这是Th的翻译。 No. 2 的 1，通过同胚 $x \mapsto i_{\mathscr{H}}(x)$ 乘以结构的迁移，如命题 5 所示。

当X上定义的函数中的集合$\mathscr{P}$替换$\mathscr{H}$时，可以扩展该编号的某些数，其中$\mathbf{R} \cup \{+\infty\}$中的值是下半连续的，$\mathscr{P}$假设为包含常数和满足 $\mathscr{P} + \mathscr{P} \subset \mathscr{P}$（例 2）。

#### 例 {#int-iv-s7-n3-exa-1 .statement tag=08Z2}

— 取$\mathbf{R}^3$中X为单位球$\|x\| \leq 1$，令$\mathscr{H}$为仿射线性X、包含限制至X上连续函数的向量空间 $\mathbf{R}^3$和满足上的函数*最大原理*，即对于每个非常数函数$h \in \mathscr{H}$，X的点的集合（其中h达到其上等）包含在球体内$S_2$。然后很容易从 Props 中得出结论。 5和7即$\operatorname{Ch}_{\mathscr{H}}(X) = \check{S}_{\mathscr{H}}(X) = S_2$。 向量空间 $\mathscr{H}$ 满足前面的条件的一个重要例是X 上连续的函数的集合以及开球$\|x\| < 1$ 中的*谐波*。对于这些函数，可以证明质量 1 的正测度 $\mu$，使得所有 $h \in \mathscr{H}$ 的 $\operatorname{Supp}(\mu) \subset S_2$ 和 $h(x) = \int h \, d\mu$ 均已给出，如果 $\|x\| < 1$，由泊松公式给出

$$
d\mu(z) = \frac{1 - \|z\|^2}{\|z - x\|^3} d\sigma(z),
$$

其中 $\sigma$ 是在正交群下对 $S_2$ 不变的测量，并且使得 $\sigma(S_2) = 1$（Ch. VII, §3，Exer. 8）。*

### 4. 应用：II。连续复形函数的向量空间

令$X$为非空紧凑空间，$\mathscr{H}$复数Banach空间$\mathscr{C}(X; \mathbf{C})$的线性子空间，包含为常量并分隔$X$的点。 函数$f \in \mathscr{H}$的实数部分$\Re(f)$的集合是实数向量空间$\mathscr{C}(X; \mathbf{R})$的线性子空间$\mathscr{H}_r$；对于每个 $f \in \mathscr{H}$、集合 $\mathscr{H}_r$ 以及包含 $\mathscr{I}(f) = \Re(-if)$；由此可见，$\mathscr{H}_r$将点与$X$分开，因为关系$h(x) = h(y)$对于所有$h \in \mathscr{H}_r$意味着$\Re(f(x)) = \Re(f(y))$和$\mathscr{I}(f(x)) = \mathscr{I}(f(y))$，因此$f(x) = f(y)$对于所有$f \in \mathscr{H}$。 $X$中的$\mathscr{H}_r$-极值点又称为$\mathscr{H}$-极值，其中集合记为$\mathrm{Ch}_{\mathscr{H}}(X)$，后者集合的闭包记为$\check{S}_{\mathscr{H}}(X)$。 Props 的类似物。 5和7如下：

#### 命题 9 {#int-iv-s7-prop-9 .statement tag=08Z3}

*对于每个函数$f \in \mathscr{H}$，$\mathrm{Ch}_{\mathscr{H}}(X)$与点的集合相交，其中$|f|$达到其最高值。*

我们可以将极限自己考虑到$f$不是常数0的情况。令$a$为$X$的点，其中$|f|$达到其最高值，并且集合$g = f/f(a)$；然后 $g(a) = 1$ 和 $|g(x)| \leq 1$ 对于所有 $x \in X$、从而

$$
\Re(g(a)) = 1 \quad \text{and} \quad \Re(g(x)) \leq 1 \quad \text{for all } x \in X.
$$

根据No. 3的第5条法则应用于$\mathscr{H}_r$，存在$b \in \mathrm{Ch}_{\mathscr{H}}(X)$，其中$\Re((g(x))$达到其上等1，自$|g(b)| \leq 1$起从而$|g(b)| = 1$；由此可见，对于所有$x \in X$，$|f(b)| = |(f(a)| \geq |f(x)|$。

#### 命题 10 {#int-iv-s7-prop-10 .statement tag=08Z4}

*令$F$为$X$的闭子集。以下属性是等效的：
a）$F$包含$\check{S}_{\mathscr{H}}(X)$。
b) 对于每个函数$f \in \mathscr{H}$，$F$与$X$的点的集合相交，其中$|f|$达到其最高值。
c) 对于每个点$x \in X$，$X$上存在总质量1的正测量$\mu$，使得每个函数$f \in \mathscr{H}$都有$\mathrm{Supp}(\mu) \subset F$和$f(x) = \int f d\mu$。
让我们证明条件a)和c)的等价：让$f = f_1 + i f_2$和$f_1, f_2$在$\mathscr{H}_r$中； 关系$f(x) = \int f d\mu$相当于两个关系$f_1(x) = \int f_1 d\mu$和$f_2(x) = \int f_2 d\mu$；因此，适用于No. 3第7号提案的条件a)和c)中的$\mathscr{H}_r$等价就足够了。 a) 蕴含 b) 的事实由命题 9 得出。让我们证明 b) 蕴含 a)；这是一个问题，如果 b) 得到验证，那么对于每个 $h \in \mathscr{H}_r$，F 与点的集合相交，其中 $h$ 在 X 中达到其下确界。 条件 b) 意味着 F 是非空；由于 F 是紧致的，因此存在 $a \in F$，使得对于所有 $y \in F$ 都有 $h(a) \leq h(y)$。令 $f \in \mathscr{H}$ 使得 $h = \mathscr{R}(f)$；对于每个 $\varepsilon > 0$、函数 $g = f - h(a) + \varepsilon$ 属于到 $\mathscr{H}$，以及
$$
\mathscr{R}(g(y)) = h(y) - h(a) + \varepsilon \geq \varepsilon
$$
对于所有$y \in F$。设$c$为$|g|$在X中的上乘，集合$b = c^2 / 2\varepsilon$；每$y \in F$，
$$
|g(y) - b|^2 = |g(y)|^2 - 2b \mathscr{R}((g(y))) + b^2 \leq c^2 - 2b\varepsilon + b^2 = b^2,
$$
在其他字中，函数$|g - b|$的F中上界为$\leq b$。由于F上的$g - b \in \mathscr{H}$，假设意味着$|g - b| \leq b$，从而
$$
b^2 \geq |g - b|^2 = |g|^2 - 2b \mathscr{R}(g) + b^2
$$
所以$\mathscr{R}(g) \geq |g|^2 / 2b \geq 0$；由于$\mathscr{R}(g) = h - h(a) + \varepsilon$和$\varepsilon > 0$是任意的，所以我们有$h \geq h(a)$，$h(a)$是X中$h$的下确界，从而完成证明。

#### 注 {#int-iv-s7-n4-rem-1 .statement tag=08Z5}

如果$f$是连续实数函数，则$|f|$达到其最高值的点就是点，其中函数$f, -f$之一达到其最高值。对于连续实数函数满足的向量空间$\mathscr{H}$，No. 3的假设，Props。因此，9 和 10 是 Props 的微不足道的推论。分别为5和7。

### 5. 应用：III。 代数连续函数

#### 引理 4 {#int-iv-s7-lem-4 .statement tag=08Z6}

令 X 为紧致空间，$\mathscr{H}$ 为 Banach 空间 $\mathscr{C}(X; \mathbf{C})$（或 $\mathscr{C}(X; \mathbf{R})$）的闭合线性子空间。设a为X的点，承认可数基本邻域系统；假设，对于任何数 c 和 d，使得 $0 < c < d < 1$ 和 a 的任何开邻域 U，存在一个 $f \in \mathscr{H}$ 使得
$$
|f| \leq 1,\quad |f(a)| \geq d,\quad |f(x)| \leq c \text{ for all } x \in X - U.
$$
那么存在函数 $u \in \mathscr{H}$，使得 $|u(x)| < |u(a)|$ 对于所有 $x \neq a$。

令$(V_n)$ ($n \geq 1$) 为$a$邻域的基本系统，并令$\lambda, \mu, \varepsilon$为数，使得
$$
0 < \lambda < 1,\quad 1 < \mu < \mu + \varepsilon \leq 1 + \lambda.
$$
因此$0 < \lambda / \mu < 1 / \mu < 1$。我们将在 $n$ ($n \geq 1$)、递减序列 $(U_n)$ 前往定义、归纳 $a$ 的开放社区，这样$U_n \subset V_n$ 适合所有 $n$，以及序列 $\mathscr{H}$ 满足关系函数中的$(h_n)$
$$
\begin{align*}
(13_n) &\quad |h_n(x)| \leq \mu \quad \text{for all } x \in X \\
(14_n) &\quad h_n(a) = 1 \\
(15_n) &\quad |h_n(x)| \leq \lambda \quad \text{for all } x \in X - U_n \\
(16_n) &\quad \left| \sum_{j=1}^n \lambda^j h_j(y) \right| < \sum_{j=1}^{n+1} \lambda^j \quad \text{for all } y \in X.
\end{align*}
$$
假设为$1 \leq m < n$、满足前面四个条件定义了$h_m$和$U_m$（其中$n$替换为$m$）；另一方面，集合$U_0 = X$。
函数 $\sum_{j=1}^{n-1} \lambda^j h_j$（如果$n = 1$则等于0）是连续的并且在点$a$处取值$\sum_{j=1}^{n-1} \lambda^j$；因此存在$a$的开邻域$U_n$，包含在$U_{n-1} \cap V_n$中，使得
$$
\left| \sum_{j=1}^{n-1} \lambda^j h_j(y) \right| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n \quad \text{for all } y \in U_n.
$$
到假设时，存在函数 $f \in \mathscr{H}$ 使得
$$
\begin{align*}
|f(x)| &\leq 1 \quad \text{for all } x \in X , \quad |f(a)| \geq 1 / \mu , \\
|f(x)| &\leq \lambda / \mu \quad \text{for } x \in X - U_n .
\end{align*}
$$
集合$h_n = f / f(a)$； 关系 $(13_n)$、$(14_n)$ 和 $(15_n)$ 然后按住； 集合
$$
g = \sum_{j=1}^n \lambda^j h_j = \sum_{j=1}^{n-1} \lambda^j h_j + \lambda^n h_n .
$$
通过 (17) 和 $(13_n)$，对于 $y \in U_n$ 我们有
$$
|g(y)| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n + \mu \lambda^n \leq \sum_{j=1}^{n+1} \lambda^j ,
$$

从 $\varepsilon + \mu \leq 1 + \lambda$ 开始；对于$x \in X - U_n$，我们还有$|h_p(x)| \leq \lambda$对于$1 \leq p \leq n$，还有从而
$$
|g(x)| \leq \sum_{j=2}^{n+1} \lambda^j < \sum_{j=1}^{n+1} \lambda^j,
$$
完备的$(16_n)$的证明。

因此，对于所有 $n$ 和所有 $x \in X$，自 $\lambda < 1$ 和 $|h_n(x)| \leq \mu$ 起，级数 $\sum_{n=1}^{\infty} \lambda^n h_n$ 通常收敛于 $X$；设$u$为其和，由于$\mathscr{H}$是封闭的，所以属于到$\mathscr{H}$。到关系$(14_n)$，我们有$u(a) = \sum_{n=1}^{\infty} \lambda^n$；另一方面，如果$x \neq a$，则存在整数$n$使得$x \notin U_{n+1}$；因此 $|h_{n+k}(x)| \leq \lambda$ 对于所有 $k \geq 1$ 乘以关系 $(15_n)$；由此可见，使用$(16_n)$，
$$
|u(x)| \leq \left| \sum_{j=1}^n \lambda^j h_j(x) \right| + \left| \sum_{j=n+1}^{\infty} \lambda^j h_j(x) \right| < \sum_{j=1}^{n+1} \lambda^j + \lambda \sum_{j=n+1}^{\infty} \lambda^j
$$
$$
= \sum_{j=1}^{\infty} \lambda^j = |u(a)|.
$$

#### 定理 2（E.主教）{#int-iv-s7-thm-2 .statement tag=08Z7}

— *令$X$是复数Banach代数$\mathscr{C}(X; \mathbf{C})$的紧空间，$\mathscr{A}$闭子代数。假设 $\mathscr{A}$ 包含为常量并分隔点和 $X$。设$a$为$X$的点；以下条件是等效的：

a) 存在函数$f \in \mathscr{A}$，使得$|f(x)| < |f(a)|$对于所有$x \neq a$。

b) 点 $a$ 是 $\mathscr{A}$ 极值，并且承认邻域的可数基本系统。

a) $\Rightarrow$ b): 设$f \in \mathscr{A}$使得$|f(a)| > |f(x)|$对应于$x \neq a$；根据No. 4第9条，$a$是$\mathscr{A}$极值点。另一方面，如果$U_n$是$x \in X$的集合使得$|f(x)| > |f(a)| - 1/n$，则$U_n$是$a$的开邻域，并且交是$U_n$约化到$a$的开邻域；由于$X$是紧凑的，$U_n$形式是$a$邻域的基本系统（GT，I, §9, No. 1，Th.1）。

b) $\Rightarrow$ a)：只要验证 b) 蕴含引理 4 的假设即可。 引理中的记号，集合 $\varepsilon = \log d / \log c$；因此$0 < \varepsilon < 1$。由于$a$是$\mathscr{A}_r$极值点，因此存在函数$g \in \mathscr{A}$使得
$$
\mathscr{R}(g) \geq 0,\quad \mathscr{R}(g(a)) \leq \varepsilon,\quad \mathscr{R}(g(x)) \geq 1 \text{ for } x \in X - U
$$

（No. 3，提案 6，b））。 集合$f = c^g$；因为$f$是正常收敛的级数$\sum_{n=0}^{\infty} (\log c)^n g^n / n!$的和，所以我们有$f \in \mathscr{A}$并且

$$
|f| \leq 1,\quad |f(a)| \geq c^{\varepsilon} = d,\quad |f(x)| \leq c \text{ for } x \in X - U.
$$

Q.E.D.

#### 推论{#int-iv-s7-n5-cor-1 .statement tag=08Z8}

— *假设在加法中 $X$ 是可度量的。那么以下属性是等效的*：

a) *$a$ 是 $X$* 的 $\mathscr{A}$ 极值点。

b) *存在$u \in \mathscr{A}$，使得$|u(x)| < |u(a)|$对于所有$x \neq a$*。

c) *令$\mathfrak{M}$为子集$M$或$X$的集合，使得对于每一个函数$f \in \mathscr{A}$，$|f|$在$X$中至少达到一个点 $M$。然后 $a$ 属于到所有集合 $M \in \mathfrak{M}$*。

d) *令$\mathfrak{N}$为子集$N$或$X$的集合，使得对于每一个函数$f \in \mathscr{A}$，$\mathscr{R}(f)$在$X$中至少在一个点处达到其最高值$N$。然后 $a$ 属于到所有集合 $N \in \mathfrak{N}$*。

*在其他字*中，

$$
\mathrm{Ch}_{\mathscr{A}}(X) = \bigcap_{M \in \mathfrak{M}} M = \bigcap_{N \in \mathfrak{N}} N.
$$

因为，在可度量的空间中，每个点都承认邻域的可数基本系统，a) 和 b) 的等价由 Th 得出。 2. 让我们证明b)蕴涵c)：事实上，$a$是唯一的点，其中$|u|$达到其至高；另一方面，c) 意味着 a)，因为对于每个 $f \in \mathscr{A}$，$\mathrm{Ch}_{\mathscr{A}}(X)$ 与点的集合相交，其中 $|f|$ 达到其最高值（No. 4，命题 9）。同样的推理，使用No. 3的命题5，表明d）蕴涵a）。最后，要看到 b) 蕴涵 d)，我们可以将自己限制在 $X$ 不约化到单个点 $a$ 的情况，因此 $u(a) \neq 0$； 函数$v = u/u(a)$，然后属于到$\mathscr{A}$，我们有$v(a) = 1$和$|v(x)| < 1$对应$x \neq a$，从而$\mathscr{R}(v(a)) = 1$和$\mathscr{R}(v(x)) < 1$对应$x \neq a$。由于函数 $\mathscr{R}(v)$ 仅在点 $a$ 时达到其最高值，因此对于每个 $N \in \mathfrak{N}$，我们确实有 $a \in N$。

#### 例 {#int-iv-s7-n5-exa-1 .statement tag=08Z9}

— 令$X_1$为点$(z_1, z_2) \in \mathbf{C}^2$的集合，使得$|z_1|^2 + |z_2|^2 \leq 1$（$\mathbf{R}^4$中的单位球），并令$\mathscr{A}_1'$为全纯的限制至$X_1$的集合函数，$\mathbf{C}$中的值，定义在$\mathbf{C}^2$中的$X_1$邻域内（考虑的邻域取决于函数）；设$\mathscr{A}_1$为$\mathscr{C}(X_1; \mathbf{C})$中$\mathscr{A}_1'$的闭包，这显然是$\mathscr{C}(X_1; \mathbf{C})$的闭复形子代数，并分隔$X_1$的点。应用全纯函数的“最大原理”表明$\mathrm{Ch}_{\mathscr{A}_1}(X_1)$是球体$S_3$。

在前面的定义中，让我们通过关系$|z_1| \leq 1$和$|z_2| \leq 1$定义的“多盘”$X_2$来计算替换$X_1$，从而产生子代数$\mathscr{A}_2'$和$\mathscr{A}_2$（ $\mathscr{C}(X_2; \mathbf{C})$的$\mathscr{A}_2'$。这里，最大原理表明$\mathrm{Ch}_{\mathscr{A}_2}(X_2)$是由关系$|z_1| = 1$和$|z_2| = 1$定义的“环面”。

From these results, one deduces that there does not exist an *analytic isomorphism* of an open neighborhood of $X_1$ onto an open neighborhood of $X_2$ that *transforms* $X_1$ *into* $X_2$; for, if $v$ were the restriction to $X_1$ of such a mapping, one would have $\mathscr{A}_2 = v \mathscr{A}_1 v^{-1}$ and so $v$ would transform $S_3$ into a space homeomorphic to $T^2$, which is absurd since $S_3$ is simply connected but $T^2$ is not. 然而，我们会观察到空间 $X_1$ 和 $X_2$ 是“同胚”，两者都是 $\mathbf{R}^4$ 中的有界凸集合，内部为非空。*

### 6. 表示积分的唯一性

设E为豪斯多夫弱局部凸空间（TVS，II, §6, No. 2），C为E中的真尖凸锥。我们知道C是E的元素$\geqslant 0$的集合，对于序关系与向量空间结构兼容当 C 被称为晶格有序时，它当然是由所理解的 E 在 C 上诱导的阶 。

#### 引理 5 {#int-iv-s7-lem-5 .statement tag=08ZA}

*假设C是弱完备的。令$\mathscr{A}$为E上连续线性形式的限制到C的集合。令$(f_\lambda)_{\lambda \in \Lambda}$为$\mathscr{A}$和$f = \sup(f_\lambda)$的元素的有限族。每$x \in C$、定义*

$$
\overline{f}(x) = \sup \left( f(x_1) + f(x_2) + \cdots + f(x_n) \right),
$$

* 超越 C 元素序列 $(x_1, x_2, \ldots, x_n)$ 的集合 $S_x$，使得$x_1 + x_2 + \cdots + x_n = x$。让$\mathrm{Card}\, \Lambda = p$。那么存在$(y_1, \ldots, y_p) \in S_x$使得$\overline{f}(x) = f(y_1) + \cdots + f(y_p)$。

用$(f_\lambda)$族的$f_1, f_2, \ldots, f_p$元素表示。对于 $k = 1, 2, \ldots, p$，令 $C_k$ 为 $y \in C$ 的集合，使得

$$
f_1(y) < f(y),\ f_2(y) < f(y),\ \ldots,\ f_{k-1}(y) < f(y),\ f_k(y) = f(y).
$$

$C_k$ 是不相交的凸锥体，其中并 C。令C中的$x_1, x_2, \ldots, x_n$满足$x_1 + x_2 + \cdots + x_n = x$。令$y_k$为属于至$C_k$的$x_i$中的和。然后$y_1 + y_2 + \cdots + y_p = x$。由于 $f$ 仿射于 $C_k$、$f(y_1) + \cdots + f(y_p) = f(x_1) + \cdots + f(x_n)$。所以

$$
f(x) = \sup \left( f(y_1) + \cdots + f(y_p) \right),
$$

其中$(y_1, y_2, \ldots, y_p)$超过C的$p$点的序列的集合，使得$y_1 + y_2 + \cdots + y_p = x$。 集合$D = C \cap (x - C)$。由于 D 是紧致的（TVS，II, §6, No. 8，命题 11 的 Cor. 2），元素 $(y_1, \ldots, y_p)$ 的集合 $D^p$ 也紧致$y_1 + \cdots + y_p = x$，从而得到上等（19）。

#### 引理 6 {#int-iv-s7-lem-6 .statement tag=08ZB}

我们维持引理 5 的假设和记号，并假设$f_\lambda$ 为正。 函数 $\overline{f}$ 在 $C$ 中是正齐次凹上半连续。如果 $C$ 是格序的，那么它是仿射的。

显然$\overline{f}$是正齐次的。让$x, y$属于到$C$。如果$C$中的$x_1, \ldots, x_m, y_1, \ldots, y_n$使得$x_1 + \cdots + x_m = x,\ y_1 + \cdots + y_n = y$，则$x_1 + \cdots + x_m + y_1 + \cdots + y_n = x + y$，因此

$$
f(x_1) + \cdots + f(x_m) + f(y_1) + \cdots + f(y_n) \leq \overline{f}(x + y);
$$

由此可见 $\overline{f}(x) + \overline{f}(y) \leq \overline{f}(x + y)$，因此 $\overline{f}$ 是凹的。令$L$（或$L_\lambda$）为$(t, x) \in \mathbf{R} \times E$的集合，使得$x \in C$和$0 \leq t \leq \overline{f}(x)$（或$0 \leq t \leq f_\lambda(x)$）。每个$L_\lambda$在弱完全真凸锥$\mathbf{R}_+ \times C$中都是封闭的，因此和$\sum_{\lambda \in \Lambda} L_\lambda$是封闭的（TVS，II, §6, No. 8，第11条命题的Cor.2）。到引理 5，这个和等于$L$。因此$L$是闭集，证明$\overline{f}$是上半连续的。最后，假设$C$是格序的，并证明$\overline{f}$是凸的。令 $x, y$ 属于到 $C$ 并令 $\varepsilon > 0$。 $C$中存在$z_1, z_2, \ldots, z_n$，使得$f(z_1) + \cdots + f(z_n) \geq \overline{f}(x + y) - \varepsilon$和$z_1 + \cdots + z_n = x + y$。 向量空间 $C - C$ 是阶的晶格有序，由$E$ 的晶格有序（A，VI, §1, No. 9，命题 8）。通过分解定理（*loc.cit.*，No. 10，Th.1），$C$中存在$x_1, \ldots, x_n, y_1, \ldots, y_n$，使得

$$
x_1 + y_1 = z_1,\ \ldots,\ x_n + y_n = z_n,\ x_1 + \cdots + x_n = x,\ y_1 + \cdots + y_n = y.
$$

那么，由于 $f$ 是正齐次且凸的，

$$
\begin{align*}
\overline{f}(x + y) &\leq \varepsilon + f(z_1) + \cdots + f(z_n) \\
&\leq \varepsilon + f(x_1) + f(y_1) + \cdots + f(x_n) + f(y_n) \\
&\leq \varepsilon + \overline{f}(x) + \overline{f}(y).
\end{align*}
$$

由于$\varepsilon$是任意的数$> 0$，我们证明了$\overline{f}$确实是凸的。

#### 定理 3（乔凯）{#int-iv-s7-thm-3 .statement tag=08ZC}

*令$E$为Hausdorff弱局部凸空间，$C$弱完全真凸锥，顶点0位于$E$，$G$并，$C$的极值生成元，$K$紧凸$C$、$\lambda$ 和 $\lambda'$ 的子集在 $K$ 上质量 1 的正测量，承认相同的重心，使得 $\lambda^*(K - (K \cap G)) = {\lambda'}^*(K - (K \cap G)) = 0$。假设 $C$ 是晶格有序的。然后，对于$C$、$\lambda^*(f|K) = {\lambda'}^*(f|K)$上的每个下半连续、正齐次凸函数$f \geq 0$。*

令$\mathscr{A}$（或$\mathscr{A}'$）为$E$上连续线性形式（或仿射函数）的限制到$C$的集合。我们知道（TVS，II, §5, No. 4，注 2）$f$是$\mathscr{A}$的元素集合的上包络线，即$\leq f$。 形式$\sup(f_1, \ldots, f_p)$的函数的集合，其中$f_1, \ldots, f_p$属于到$\mathscr{A}$、$f_1 \geq 0, \ldots, f_p \geq 0$，是递增有向集合并且以$f$作为其上包络线。考虑到§1, No. 1，Th。 1、当$f$是前面的形式时，验证等式$\lambda(f|K) = \lambda'(f|K)$就足够了。

定义 $\overline{f}$ 如引理 5。显然，如果$y \in G$则$\overline{f}(y) = f(y)$。从 $\lambda^*(K - (K \cap G)) = 0$ 开始，我们就有了 $\lambda(f|K) = \lambda(\overline{f}|K)$。到引理 6，$\overline{f}$ 是仿射且上半连续的。因此$\overline{f}|K$是$\mathscr{A}'$的元素到K的递减有向集合到限制的下包络线（TVS，II, §5, No. 4，第6条）。令 $x \in K$ 为 $\lambda$ 的重心。如果$g \in \mathscr{A}$则$\lambda(g|K) = g(x)$。因此 $\lambda(\overline{f}|K) = \overline{f}(x)$（§ 4, No. 4，第 5 条命题第 2 条）。因此$\lambda(f|K) = \overline{f}(x)$，人们也可以看到类似的$\lambda'(f|K) = \overline{f}(x)$。

#### 推论{#int-iv-s7-n6-cor-1 .statement tag=08ZD}

*设 E 为 Hausdorff 局部凸空间，C E 中顶点为 0 的真凸锥，承认紧底 M，并设 G 为 C 极值生成元的并。让$x \in M$。如果 C 是晶格有序的，则 M 上最多存在一个质量 1 的正测度 $\lambda$，使得 $\lambda^*(M - (G \cap M)) = 0$，并承认 x 作为重心。*

E 的替换拓扑被弱化的拓扑 （这不是 M 的变换拓扑），可以假设 E 是一个弱空间。令 $\lambda$ 和 $\lambda'$ 为 M 上具有所述属性的两个度量，并令 h 为 E 上的连续线性形式，使得 M 为 C 和超平面的交，且方程为 $h(x) = 1$。令$\mathscr{S}$为C上正齐次且连续的凸函数$\geq 0$的M的$\mathscr{C}(M)$由……组成或限制的子集。圆锥体 C 是弱完备的（TVS，II, §7, No. 3）。由 Th. 3、每$f \in \mathscr{S}$对应$\lambda(f) = \lambda'(f)$。

如果 $f_1, f_2, f_3, f_4$ 属于到 $\mathscr{S}$，则
$$
\begin{align*}
\sup(f_1 - f_2, f_3 - f_4) &= \sup(f_1 + f_4, f_3 + f_2) - (f_2 + f_4) \in \mathscr{S} - \mathscr{S} \\
\inf(f_1 - f_2, f_3 - f_4) &= -\sup(f_2 - f_1, f_4 - f_3) \in \mathscr{S} - \mathscr{S}.
\end{align*}
$$
从$h|M \in \mathscr{S}$开始，$\mathscr{S} - \mathscr{S}$包含为常数函数。如果x和y是M的两个不同的点，则E上存在一个连续的线性形式将x和y分开，并且这个形式是两个在C上为正的连续线性形式的差（TVS，II, §6, No. 8，引理1）。由上可知，对于$\alpha, \beta$实数，存在$f \in \mathscr{S} - \mathscr{S}$使得$f(x) = \alpha, f(y) = \beta$。那么$\mathscr{S} - \mathscr{S}$在$\mathscr{C}(M)$中对于拓扑一致收敛是稠密的（GT，X, §4, No. 1，Prop.2的Cor.）。从 $\mathscr{S} - \mathscr{S}$ 上的 $\lambda$ 和 $\lambda'$ 重合开始，我们有 $\lambda = \lambda'$。

习题

### 习题{#int-iv-s7-exercises}

§ 7](exercises/s7/)参见[习题。
