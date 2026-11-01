---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 3
section_title: Integrals of continuous vector-valued functions
lang: zh
source: int-i-vi
book_pages: INT III.32-INT III.40, INT III.60
pdf_pages: 0077-0085, 0105-0105
extraction: ocr
subsections:
    - "no": 1
      title: Definition of the integral of a vector-valued function
      page: 32
      pdf_page: 77
    - "no": 2
      title: Properties of the vectorial integral
      page: 34
      pdf_page: 79
    - "no": 3
      title: Criteria for the integral to belong to $E$
      page: 37
      pdf_page: 82
    - "no": 4
      title: Continuity properties of the integral
      page: 39
      pdf_page: 84
statements: 17
exercises: 4
content_sha256: da15b0f46771974127c1877c775fb947b7ad3855dc090b833b89bdead0e402aa
translated_from: content/en/int/III/03_s3_integrals_of_continuous_vector_valued.md
translation_method: google
source_content_sha256: fe78ffc7611951df252f5590889a4a16218a67a71377a0b79b5c7914e9bc3371
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 63bea6c02c0ae20b3084b9214d4d674932e4f1320739545d1ce55d58ed3dbe6e
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。连续向量值函数的积分

*在此过程中，截面、X表示局部紧致空间，E 表示$\mathbf{R}$或$\mathbf{C}$上的局部凸空间。我们用$E'$表示E的对偶（E上连续线性形式的空间），用${E'}^*$表示$E'$的代数对偶（$E'$上所有线性形式的空间）；对于$z \in E$、$z' \in E'$、${z'}^* \in {E'}^*$，我们写为$\langle z, z' \rangle = z'(z)$、$\langle {z'}^*, z' \rangle = {z'}^*(z')$。

回想一下，如果 E 是 Hausdorff，则可以通过将元素 $z \in E$ 与 $E'$ 上的线性形式 $z' \mapsto \langle z, z' \rangle$ 识别为 ${E'}^*$ 的线性子空间来识别 E，并且配备弱拓扑 $\sigma({E'}^*, E')$ 的 ${E'}^*$ 可以是规范地认为E的完成配备了削弱的拓扑$\sigma(E, E')$。

### 1.向量值函数积分的定义

Recall that a mapping f of X into E is said to be *weakly continuous* if, for every $z' \in E'$, the mapping $x \mapsto \langle f(x), z' \rangle$ of X into $\mathbf{C}$ (in other words the mapping $z' \circ f$, also denoted $\langle f, z' \rangle$) is continuous. 如果对于每个 $z' \in E'$，映射 $x \mapsto \langle f(x), z' \rangle$ 具有紧致支持，我们可以说 X 的映射 f 进入 E 是*紧致支持的标量*。 我们将 X 的映射的 $\widetilde{\mathscr{K}}(X; E)$ 空间表示为 E，它们是*弱连续且紧致支持的标量*；显然$\widetilde{\mathscr{K}}(X; E) \supset \mathscr{K}(X; E)$，但这两个空间不一定相同（见下面的*例*2）；然而，当 E 是有限维时，它们是相等的。

注在函数的定义是弱连续的（分别是紧支持的标量），E的拓扑仅通过E的对偶$E'$的中介进行干预；因此，当 E 的拓扑被对偶相同的任何局部凸拓扑替换时，这些函数中的集合不会改变。

如果E和F是对偶中的两个向量空间，我们注说，X到E中的映射对于$\sigma(E, F)$来说是“连续”，并且说它是“弱连续”，这意味着相同的意思。

令$f$为$X$到$E$的映射，紧支持的弱连续和标量，并令$\mu$为$X$的测度；对于每个$z' \in E'$，我们有$z' \circ f \in \mathscr{K}(X)$； 集合

$$
\varphi(z') = \int \langle f(x), z' \rangle d\mu(x) = \mu(z' \circ f).
$$

很明显，$\varphi$是$E'$上的线性形式，因此是${E'}^*$*的*元素。

#### 定义 1 {#int-iii-s3-def-1 .statement tag=08NN}

*对于每个函数$f \in \widetilde{\mathscr{K}}(X;E)$，我们称$f$相对于$\mu$的积分，并用$\int f d\mu$或$\int f(x) d\mu(x)$，或$\int f \mu$，或$\int f(x)\mu(x)$，元素定义的${E'}^*$表示*

$$
\left\langle \int f d\mu, z' \right\rangle = \int \langle f, z' \rangle d\mu \quad \text{for all } z' \in E'.
$$

我们注即使$E$是*Hausdorff*和$f \in \mathscr{K}(X;E)$，*也不一定有*$\int f d\mu \in E$（例1；cf.No. 3）。

#### 例 {#int-iii-s3-n1-exa-1 .statement tag=08NO}

— 1) 假设$E$是$\mathbf{C}$和Hausdorff上的*有限维的*，因此如果$(e_i)_{1 \leq i \leq n}$是$E$的基，则映射

$$
(\xi_1, \ldots \xi_n) \mapsto \sum_{i=1}^n \xi_i e_i
$$

是$\mathbf{C}^n$到$E$的*同构*。然后我们知道$E$上的每个线性形式都是连续的，在其他字中，$E'$与$E$的代数对偶$E^*$相同，并且${E'}^*$可以规范地与$E$等同。令$(e'_i)_{1 \leq i \leq n}$为$E'$对$(e_i)$的基；为了使$X$到$E$的映射$f$是弱连续且具有紧支撑的标量，函数$f_i = e'_i \circ f$是具有紧支撑连续的充分必要；那么我们对所有 $x \in X$ 都有 $f(x) = \sum_{i=1}^n f_i(x) e_i$，并且

$$
\int f d\mu = \sum_{i=1}^n \mu(f_i) e_i.
$$

2) 让我们在$X$采取$E$空间$\mathscr{M}(X; \mathbf{C})$的措施，配备*模糊*拓扑（§ 1, No. 9）；然后，$E$的对偶$E'$可以被规范地识别为空间$\mathscr{K}(X; \mathbf{C})$（TVS，II, § 6, No. 2，提案3）。 $X$到$E$的映射$x \mapsto \varepsilon_x$是*连续的*（§ 1, No. 9，命题13），但是如果$X$不是紧致的，那么它的支持不是紧致的；然而，它是*紧凑*支持，因为对于每个函数 $f \in E'$ 函数 $x \mapsto \langle \varepsilon_x, f \rangle = f(x)$ by 定义都有紧凑支持。而且，

$$
\int \langle \varepsilon_x, f \rangle d\mu = \int f(x) d\mu(x) = \langle \mu, f \rangle
$$

对于每个函数 $f \in \mathscr{K}(X; \mathbf{C}) = E'$，这证明了

$$
\int \varepsilon_x d\mu(x) = \mu
$$

对于 $X$ 上的每个小节 $\mu$。

3）如果$E$是Hausdorff，那么对于每个点$y \in X$和每个函数$f \in \widetilde{\mathscr{K}}(X; E)$，我们有

$$
\int f d\varepsilon_y = f(y)
$$

因为$\int \langle f, z' \rangle d\varepsilon_y = \langle f(y), z' \rangle$乘定义。

#### 注 1 {#int-iii-s3-n1-rem-1 .statement tag=08NP}

如果$E$是局部凸空间，$N$是$\{0\}$在$E$的闭包，那么$E_1 = E/N$是与$E$相关的Hausdorff局部凸空间，我们知道对偶$E'$和$E'_1$ 相同；对于函数$f$至属于至$\widetilde{\mathscr{K}}(X; E)$，$f_1 = \pi \circ f$（其中$\pi : E \to E_1$为典范同态）属于至$\widetilde{\mathscr{K}}(X; E_1)$是必要且充分的，在这种情况下为$\int f d\mu = \int f_1 d\mu$。因此，我们可以自己极限只考虑*Hausdorff*局部凸空间。

#### 注 2 {#int-iii-s3-n1-rem-2 .statement tag=08NQ}

令$E$为空间*over*$\mathbf{C}$的局部凸，并令$E_0$为$E$底层的局部凸空间*over*$\mathbf{R}$；我们知道映射$z' \mapsto \Re z'$，对于$E$上的每个连续（复数）线性形式$z'$，使对应成为$E_0$上的连续（实数）线性形式$z \mapsto \Re \langle z, z' \rangle$，是对偶的$\mathbf{R}$同构$E'$ 到$E_0$ 的双$E'_0$（TVS，II, §8, No. 1）。类似地，实向量空间 $E'_0$ 的代数对偶 $E'_0*$ 可以与 $E'$ 的代数对偶 $E'*$ 下的实数空间规范地等同。由此可见，如果 $\mu$ 是一个*实测度*并且 $f$ 映射在 $\widetilde{\mathscr{K}}(X; E)$ 中，则当 $f$ 被视为在 $E_0$ 中取其值以及在两者中的规范双线性形式时，公式 (1) 再次有效成员分别相对于第一个成员的$E'_0$和$E'_0*$之间的对偶性以及第二个成员的$E_0$和$E'_0$之间的对偶性。

### 2.矢量积分的性质

#### 命题 1 {#int-iii-s3-prop-1 .statement tag=08NR}

— *映射*

$$
(f, \mu) \mapsto \int f d\mu
$$

$\widetilde{\mathscr{K}}(X; E) \times \mathscr{M}(X; \mathbf{C})$ 到 $E'*$ *是双线性*。

命题紧随 Def. 之后。 No. 1 中的 1 个。

令$u$为$E$的连续线性映射变为局部凸空间$F$；我们知道转置$^t u$是$F$的对偶$F'$到$E$的对偶$E'$的线性映射；我们用 $^{tt} u$ 映射 ${E'}^* \to {F'}^*$、转置或 $^t u$ 表示（代数意义上）；当$E$和$F$是Hausdorff并且分别用${E'}^*$和${F'}^*$的子空间规范地识别时，$^{tt} u$扩展映射$u$。有了这些记号：

#### 命题 2 {#int-iii-s3-prop-2 .statement tag=08NS}

— 令$u$为$E$的连续线性映射变为局部凸空间$F$；对于每个函数 $f \in \widetilde{\mathscr{K}}(X;E)$、函数 $u \circ f$ 属于到 $\widetilde{\mathscr{K}}(X;F)$ 以及

$$
\int u(f(x))\, d\mu(x) = ^{tt} u \left( \int f(x)\, d\mu(x) \right).
$$

对于每个连续的线性形式$z' \in F'$，我们在设定$y' = z' \circ u = {}^t u(z') \in E'$上有$z' \circ u \circ f = y' \circ f$，从而第一个断言；此外，对于所有$z' \in F'$，

$$
\left\langle \int (u \circ f)\, d\mu, z' \right\rangle = \int \langle u \circ f, z' \rangle\, d\mu = \int \langle f, {}^t u(z') \rangle\, d\mu \\
= \left\langle \int f\, d\mu, {}^t u(z') \right\rangle = \left\langle {}^{tt} u \left( \int f\, d\mu \right), z' \right\rangle,
$$

从而公式 (2)。

#### 命题 3 {#int-iii-s3-prop-3 .statement tag=08NT}

— 对于每个函数 $g \in \mathscr{C}(X;\mathbf{C})$ 和每个函数 $f \in \widetilde{\mathscr{K}}(X;E)$、函数 $gf$ 属于到 $\widetilde{\mathscr{K}}(X;E)$ 以及

$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$

事实上，对于每个$z' \in E'$、$\langle gf, z' \rangle = g \langle f, z' \rangle$、从而，第一个断言；此外，

$$
\left\langle \int f\, d(g \cdot \mu), z' \right\rangle = \int \langle f, z' \rangle\, d(g \cdot \mu) = \int g \langle f, z' \rangle\, d\mu \\
= \int \langle gf, z' \rangle\, d\mu = \left\langle \int gf\, d\mu, z' \right\rangle,
$$

从而 (3)。

#### 命题 4 {#int-iii-s3-prop-4 .statement tag=08NU}

— 令$\mu$为$X$的积极测度，$S$其支持度，$f$函数为$\widetilde{\mathscr{K}}(X;E)$。假设$E$是Hausdorff，并用弱拓扑$\sigma({E'}^*, E')$装备空间${E'}^*$。

(i) *f(S) 生成的凸锥体的*整的* $\int f\, d\mu$ *属于到闭包* C *在* E'** *中。

(ii) *如果* $\mu$ *有界，则积分* $\int f\, d\mu$ *属于到集合* $\| \mu \| \cdot D$，*其中* D *是* f(S) *在* E'** 中的闭凸包络。

如果 E 是复数，我们为 E 配备其底层 *real* 向量空间结构，正如我们所见，它不会修改公式 (1)。

(i) 我们知道C是E'**中包含f(S)的闭半空间的交，并且由闭超平面经过通过0确定；因此，足以证明，对于 $z' \in E'$，关系 $\langle f(x), z' \rangle \geq 0$ 对于所有 $x \in S$ 意味着

$$
\left\langle \int f\, d\mu, z' \right\rangle \geq 0;
$$

但自从

$$
\left\langle \int f\, d\mu, z' \right\rangle = \int \langle f, z' \rangle\, d\mu,
$$

这是从 §2, No. 3，Cor. 得出的。提案 8 中的第 2 条。

(ii) 我们知道 D 是 E'** 中包含 f(S) 的闭半空间的交；因此，足以证明，对于$z' \in E'$，关系$\langle f(x), z' \rangle \leq a$对于所有$x \in S$意味着

$$
\left\langle \int f\, d\mu, z' \right\rangle \leq a \| \mu \|;
$$

但这是从 §2, No. 3，Cor. 得出的。提案 8 中的第 3 条。

#### 推论 {#int-iii-s3-n2-cor-1 .statement tag=08NV}

*让*$\mu$*成为*X、$f$*映射属于到*$\mathscr{K}(X;E)$、*和*D*在*E'**中*f(X)*的封闭凸包络。 *存在数*$a > 0$*使得*$\int f\, d\mu \in a \cdot D$。

*如果*$\nu$*是对*X的任何测量，*存在数*$a_1, a_2, a_3, a_4 > 0$*使得*$\int f\, d\nu \in a_1 D - a_2 D + i a_3 D - i a_4 D$。

首先假设$\mu$为正；通过假设，f的支撑K是紧的；如果 $\nu$ 是 $\mu$ 的限制到 K 的相对紧开邻域，则 $\nu$ 有界，$\int f\, d\mu = \int f\, d\nu \in \| \nu \| \cdot D$ 受命题 4 (ii) 约束。第二个结果由此得出，因为任何复杂的测度都可以写为$\mu_1 - \mu_2 + i \mu_3 - i \mu_4$，其中$\mu_j$为正。

#### 命题 5 {#int-iii-s3-prop-5 .statement tag=08NW}

*假设空间* X *是紧致的，并且让* f *成为* X *的连续映射 *进入豪斯多夫局部凸空间* E。 *闭凸包络* f(X) *在* E'** *(for* $\sigma(E', E')$) *是等于向量* $\int f\, d\mu$ *对于所有正测量* $\mu$ *在* X *总质量* 1 上的集合。

令 C 为 E'** 中 f(X) 的闭凸包络；由于 f(X) 是紧致的且 E'** 是*完全*，因此 C 是紧致的。我们已经知道（命题 4），对于总质量的 $X$ 上的正测量，$\mu$ 属于的每个测量值 $\int f d\mu \in C$ 到凸集合 $H$ 等于 1。另一方面，$H$ 是凸的，并且对于模糊拓扑是“紧凑”的（§ 1, No. 9，第 15 条命题的 Cor. 3），并且是质量 1 和*有限*支撑的正测量的凸集合 $H_0$ 的闭包（为此拓扑）（§ 2, No. 4，第 1 条的 Cor.3）。现在，映射$\mu \mapsto \int f d\mu$下$H_0$的像就是${E'}^*$中$f(X)$的凸包络$C_0$。另一方面，这个映射对于$\mathscr{M}(X; C)$上的模糊拓扑和${E'}^*$上的拓扑$\sigma({E'}^*, E')$来说是连续的，从$\langle \int f d\mu, z' \rangle = \int \langle f, z' \rangle d\mu$到定义；因此$H = \overline{H_0}$的像是一个*紧凑*凸集合包含$C_0$并且包含在$C$中；从$C = \overline{C_0}$开始，这个像等于$C$。

#### 命题 6 {#int-iii-s3-prop-6 .statement tag=08NX}

*对于每个连续映射，将$X$的紧凑支撑$f$转化为Hausdorff局部凸空间$E$，$E$上的每个连续半范数$q$以及$X$上的每个测度$\mu$，使得$\int f d\mu \in E$,*

$$
q \left( \int f d\mu \right) \leq \int (q \circ f) \ d|\mu|.
$$

令$D$为$z \in E$的集合，使得$q(z) \leq 1$； $D$ 是闭凸的，包含于 0，因此 $D = D^{o o}$（TVS，II, § 6, No. 3，Th.1 的 Cor.3）。因此足以证明对于每个 $z' \in D^o$，

$$
\left| \left\langle \int f d\mu, z' \right\rangle \right| \leq \int (q \circ f) \ d|\mu|;
$$

自从

$$
\left\langle \int f d\mu, z' \right\rangle = \int \langle f, z' \rangle d\mu,
$$

从定义到 $D^o$ 开始，

$$
|\langle f(x), z' \rangle| \leq q(f(x))
$$

对于所有$x \in X$，所需的不等式来自不等式（13）或§ 1, No. 6。

### 3. 判据属于到 $E$ 的积分

#### 命题 7 {#int-iii-s3-prop-7 .statement tag=08NY}

*令 $E$ 为 Hausdorff 局部凸空间，且$f \in \mathscr{K}(X; E)$。如果$f(X)$包含在$E$的完全凸子集$A$中，则$\int f d\mu \in E$。*

设 K 为 f 的支持，f 是由假设紧致的。由于 f 在 X − K 上为零，因此 f(X) 等于 f(K) 或 f(K) ∪ {0}，因此是紧的，因为 f 是连续的且 E 是 Hausdorff；然后，E 中 f(X) 的封闭凸包络C 是预紧的（对于由 E 引起的均匀结构）（TVS，II, §4, No. 1，命题 3）。但由于 C 是完整的空间 A 的闭子集，因此 C 是完整的，因此是紧致的； 更不必说, C 对于弱化的拓扑 σ(E, E′) 是紧的；但由于拓扑是由 σ(E′*, E′) 导出的，C 是 f(X) 在 E′* 中对于拓扑 σ(E′*, E′) 的闭凸包络；因此，证明由No. 2命题4的推论得出。

#### 推论 1 {#int-iii-s3-prop-7-cor-1 .statement tag=08NZ}

— 令 E 为 Hausdorff 局部凸空间；对于每个函数 f ∈ $\mathscr{K}(X; E)$，$\int f d\mu$ 属于到完成 E 的$\widehat{E}$。

由于E和$\widehat{E}$的对偶是相同的，因此只要将f视为在$\widehat{E}$中取其值，就可以应用第7条命题。

#### 推论 2 {#int-iii-s3-prop-7-cor-2 .statement tag=08O0}

— 如果 E 是局部凸准完备 Hausdorff 空间，则对于每个函数 f ∈ $\mathscr{K}(X; E)$，$\int f d\mu \in E$。

正如第 7 条证明开头所述，f(X) 是紧的，并且 E 中的闭凸包络C 是预紧的，因此是有界的；但由于集合 C 是闭集且有界的，因此它由假设完成，并且足以应用第 7 条命题。

我们将在第 1 章中看到。 VI, §1, No. 2，其他判据适用于$\int f d\mu$至属于至E，特别适用于$\widetilde{\mathscr{K}}(X; E)$中的函数，而不仅仅是$\mathscr{K}(X; E)$中的函数。

命题7的推论2可以应用于以下两种情况：
1° E 是巴拿赫空间； 2° E 是桶状 Hausdorff 局部凸空间 G 的对偶，E 配备$\mathscr{S}$ 拓扑，其中 $\mathscr{S}$ 是有界子集对 G 的覆盖（TVS，III, §4, No. 2，Th.1 的 Cor. 4）。对于例，科。当 E 是配备模糊拓扑的 Banach 空间或测度 $\mathscr{M}(Y; \mathbf{C})$ 的空间的弱对偶时，可以应用第 7 条命题 2。

如果X = $\mathbf{R}$，$\mu$是$\mathbf{R}$上的勒贝格测度，且E是巴纳赫空间，则函数在$\mathscr{K}(X; E)$的积分$\int f d\mu$就是积分

$$
\int_{-\infty}^{+\infty} f(x)\, dx
$$

FRV 中定义，II, §2, No. 1；这是从公式 (1) 和 FRV, I, §1, No. 2, Cor. 得出的。提案 2。

### 4.积分的连续性性质

#### 命题 8 {#int-iii-s3-prop-8 .statement tag=08O1}

— 假设 E 是豪斯多夫；令 $\mu$ 为X 的度量。 $\mathscr{K}(X;E)$的映射$f \mapsto \int f d\mu$到$\widehat{E}$（No. 3，第7条的Cor.1）是唯一的连续线性映射$\Phi$，使得$\Phi(g \cdot a) = \mu(g) \cdot a$对于每个向量$a \in E$和每个函数$g \in \mathscr{K}(X;\mathbf{C})$。

为了证明映射$f \mapsto \int f d\mu$的连续性，只需证明它的限制到$\mathscr{K}(X,K;E)$对于X的每个紧致子集K是连续的（TVS，II, §4, No. 4，命题5）。我们注如果E的拓扑由半范数族$(q_\alpha)$定义，则$\mathscr{K}(X,K;E)$由半范数族定义

$$
p_\alpha(f) = \sup_{x \in K} q_\alpha(f(x)) .
$$

现在，让$h$是X到$[0,1]$的连续映射，具有紧支撑，使得$h(x) = 1$在K上；根据 No. 2，第 6 号提案，对于每一个函数 $f \in \mathscr{K}(X,K;E)$，我们有，

$$
q_\alpha \left( \int f d\mu \right) = q_\alpha \left( \int h f d\mu \right) \leq \int h(x) q_\alpha(f(x)) d|\mu|(x) \leq |\mu|(h) \cdot p_\alpha(f)
$$

（$q_\alpha$通过连续性扩展到$\widehat{E}$），这证明了$f \mapsto \int f d\mu$的连续性。另一方面，当记号为叙述时，

$$
\int (g(x) \cdot a) d\mu(x) = \mu(g) \cdot a
$$

凭借No. 1、例 1 和No. 2 的第 2 条适用于典范嵌入 $\mathbf{C} \cdot a \to E$。此外，由线性组合$\sum_i g_i \cdot a_i$（其中$a_i \in E$和$g_i \in \mathscr{K}(X;\mathbf{C})$）形成的$\mathscr{K}(X;E)$的子空间在$\mathscr{K}(X;E)$（§1, No. 2，命题5）中稠密，从而完成证明。

#### 命题 9 {#int-iii-s3-prop-9 .statement tag=08O2}

— 假设 E 是豪斯多夫；设 $f$ 是 X 的连续映射到 E 中，具有紧支撑。当空间$\mathscr{M}(X;\mathbf{C})$配备严格紧收敛的拓扑（§1, No. 10）时，$\mathscr{M}(X;\mathbf{C})$入$\widehat{E}$的映射$\mu \mapsto \int f d\mu$是唯一连续的线性映射$\Psi$使得$\Psi(\varepsilon_x) = f(x)$对于所有$x \in X$。

每$z' \in E'$，

$$
\left\langle \int f d\varepsilon_x, z' \right\rangle = \int (z' \circ f) d\varepsilon_x = z'(f(x)) = \langle f(x), z' \rangle ,
$$

从而 $\int f\, d\varepsilon_x = f(x)$.此外，我们知道，对于严格紧致收敛的拓扑，点措施中的集合总计在$\mathscr{M}(X; \mathbf{C})$中（§ 2, No. 4，Th.1的Cor.4）。因此，这一切都归结为证明线性映射$u : \mu \mapsto \int f\, d\mu$的连续性。为此，将 $E'$ 的线性映射 $v : z' \mapsto \langle f, z' \rangle$ 考虑到 $\mathscr{K}(X; \mathbf{C})$ 中，并让我们证明 $E'$ 的等连续子集 $H$ 的 $v$ 下的像包含在严格紧凑的子集中$\mathscr{K}(X; \mathbf{C})$。因为，如果$K$是$f$的支持，则函数$\langle f, z' \rangle$对于$z' \in H$的支持包含在$K$中；另一方面，这些函数形式是一个等连续的集合，并且对于 $z'(f(x))$ 的每个 $x \in X$ 集合都是有界的；因此，我们的断言源自Ascoli的定理（GT，X, § 2, No. 5，Th.2的Cor.3）。现在，从No. 1的公式(1)得出$u$正是限制到转置$^t v$的$\mathscr{M}(X; \mathbf{C})$（代数意义上）；因此，其连续性源自前述内容（TVS，IV, § 1, No. 3，提案 6）。

#### 推论{#int-iii-s3-n4-cor-1 .statement tag=08O3}

— *With hypotheses and notations as in Prop. 9, the restriction of the mapping* $\mu \mapsto \int f\, d\mu$ *to the set* $\mathscr{M}_+(X)$ *of positive measures, or to a vaguely bounded subset B of* $\mathscr{M}(X; \mathbf{C})$, *is vaguely continuous.*

因为，它来自 § 1, No. 10，Props。由图17和图18可知，在$\mathscr{M}_+(X)$或$B$上，严格紧致收敛的拓扑诱导的拓扑与模糊拓扑诱导的拓扑相同。

然而，对于模糊的拓扑（示例2），映射$\mu \mapsto \int f\, d\mu$不一定在所有$\mathscr{M}(X; \mathbf{C})$上连续。

### 习题{#int-iii-s3-exercises}

§ 3](exercises/s3/)参见[习题。
