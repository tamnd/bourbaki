---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 5
section_title: Compactness criteria
lang: zh
source: evt-i-v
book_pages: TVS IV.32-TVS IV.38, TVS IV.67-TVS IV.71
pdf_pages: 0214-0220, 0249-0253
extraction: ocr
subsections:
    - "no": 1
      title: General remarks
      page: 32
      pdf_page: 214
    - "no": 2
      title: Simple compactness of sets of continuous functions
      page: 33
      pdf_page: 215
    - "no": 3
      title: The Eberlein and Šmulian theorems
      page: 35
      pdf_page: 217
    - "no": 4
      title: The case of spaces of bounded continuous functions*
      page: 36
      pdf_page: 218
    - "no": 5
      title: Convex envelope of a weakly compact set
      page: 37
      pdf_page: 219
statements: 8
exercises: 18
content_sha256: 0b622924f89957714a627d57aa8b9d4d24cb39c99648a46e51d832efceeeea8a
translated_from: content/en/evt/IV/05_s5_compactness_criteria.md
translation_method: google
source_content_sha256: 109a4d05718fd73c2e0104fdb772994f028706b89a9a4001b0f091a0d03c8b4b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: dc61db6ecc55eea03817a6a1039f4b5ca763dab929e116d638abd7b0fb5cec48
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 5。紧凑度判据

### 1. 一般注

设A为拓扑空间E的子集。对于A的点的序列$(x_n)_{n \in \mathbf{N}}$，使E的点x为极限点，满足以下条件是必要且充分的（GT，I, § 7, No. 3）：

(A) 对于 x 的每个整数 $m \geq 0$ 和每个邻域 U，都存在整数 $n \geq m$，使得 $x_n \in U$。

对于正整数的严格递增序列$(n_k)_{k \in \mathbf{N}}$，形式为$(y_k)_{k \in \mathbf{N}}$和$y_k = x_{n_k}$的序列称为序列$(x_n)_{n \in \mathbf{N}}$的提取序列。 若存在提取的序列$(x_n)_{n \in \mathbf{N}}$的序列收敛于x，则x为$(x_n)$的极限点；相反，如果 x 具有可数基数系统邻域，并且 x 是序列 $(x_n)$ 的极限点，则存在收敛于 x 的$(x_n)$ 的提取序列。

由于GT，IX, § 2, No. 9，推论，我们结论，当E可度量时，以下条件是等价的：
a) 集合 A 在 E 中相对紧；
b) A 的点的每个无限序列在 E 中都有极限点；
c) 从A的点的每个无限序列中，我们可以提取序列，它收敛到E的点。

在这个截面中，我们将扩展这个准则应用于某些不可度量的拓扑向量空间。下面的命题使我们能够在数的情况下约化研究紧集到弱紧集的研究。

#### 命题 1 {#evt-iv-s5-prop-1 .statement tag=07VR}

— 令 E 为 Hausdorff 局部凸空间，且 E 的 A 子集。令 $E_\sigma$ 表示带有弱化拓扑的空间 E。
a) 如果 A 的点的每个无限序列在 E 中都有极限点，则 A 在 E 中是预紧的。
b) 在阶中，A在E中相对紧，其在E中预紧且在$E_\sigma$中相对紧是充分必要的。

我们将通过反证法证明a)。如果 A 不是预紧的，则通过 th。 GT 的 3，II, § 3, No. 7，因此 E 中存在 0 的对称凸邻域 V，使得不能被V 的有限平移数覆盖。

在其他字中，如果$x_0, x_1, ..., x_{n-1}$是A的点，则$A \notin \bigcup_{0 \leq i < n} (x_i + V)$，因此存在A的点$x_n$，使得$x_n - x_i \notin V$对应于$0 \leq i < n$。然后，通过整数$n$上的归纳，我们可以构造A的点的无限序列$(x_n)_{n \in \mathbf{N}}$，使得每当$n > m$时$x_n - x_m \notin V$；由于 V 是对称的，因此对于 $m \neq n$ 也有 $x_m - x_n \notin V$，并且集合 $x_n + \frac{1}{2} V$ 是不相交的。对于E中的每一个点$x$，最多存在一个整数$n \geq 0$使得$x_n \in x + \frac{1}{2} V$，因此序列$(x_n)_{n \in \mathbf{N}}$不存在任何极限点。这证明了*a)*。

现在假设 A 是 E 中的预紧式，并且包含在 $E_\sigma$ 的紧式子集 B 中。那么 B 在 $E_\sigma$ 中是完整的，因此在 E 中也是完整的 (IV, p. 5, *注 2*)。我们有 $\overline{A} \subset B$，因此 A 在 E 中相对紧凑。逆命题是明显的，*b)* 如下。

### 2. 连续函数的集合简单紧性

在这个截面中，X表示X上连续函数的*紧凑*空间和$\mathscr{C}_s(X)$空间，其中值在域K中（等于$\mathbf{R}$或$\mathbf{C}$）。 空间 $\mathscr{C}_s(X)$ 被赋予X 上简单收敛的拓扑。

#### 命题 2 {#evt-iv-s5-prop-2 .statement tag=07VS}

*设 D 为 X 的稠密子集，A 子集空间 $\mathscr{C}_s(X)$。以下条件是等效的：*
(i) *在 $\mathscr{C}_s(X)$ 中相对紧凑。*
(ii) *从A的元素的每个无限序列，我们可以提取收敛于$\mathscr{C}_s(X)$的序列。*
(iii) *A 的元素的每个无限序列在 $\mathscr{C}_s(X)$ 中都有极限点。*
(iv) *设$(f_n)_{n \in \mathbf{N}}$为A的函数属于的序列和D的点的$(x_m)_{m \in \mathbf{N}}$序列。如果迭代极限*

$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$

*存在，则它们相等。在加法中，我们对所有 $x \in X$ 都有 $\sup_{f \in A} |f(x)| < + \infty$。*

(i) $\Rightarrow$ (ii) ：令 $\overline{A}$ 为$\mathscr{C}_s(X)$ 中 A 的闭包。假设 A 是紧致的，并考虑函数 $f_n \in A$ 中的序列（对于 $n \in \mathbf{N}$）。令 $\phi$ 为从 X 到可度量空间 $K^\mathbf{N}$ 的连续映射 $x \mapsto (f_n(x))_{n \in \mathbf{N}}$。 $\phi$下的X的像$X'$是一个紧凑的可度量空间，因为X是紧凑的。令E为X上连续函数$f$的$\mathscr{C}_s(X)$由……组成的闭子空间，使得对于点的每个对，关系$\phi(x) = \phi(y)$意味着$f(x) = f(y)$ $x, y$ X。由科。 2 GT，I, § 9, No. 4 和道具。 GT 中的 3，I, § 5, No. 2、映射 $f' \mapsto f' \circ \phi$ 是从 $\mathscr{C}_s(X')$ 到 E 的同胚 $\phi^*$。因而，集合 $A' = (\phi^*)^{-1}(\overline{A})$ 在 $\mathscr{C}_s(X')$ 中是紧的，显然存在元素 $A'$中的$f'_n$使得$\phi^*(f'_n) = f'_n \circ \phi$等于$f_n$。

由于 $X'$ 是紧致可度量空间，因而 $X'$ 中存在可数稠密子集 D'（GT、IX, § 2, No. 8，第 12 条命题和 § 2, No. 9，第 16 条命题）。令$\mathscr{T}_1$（分别$\mathscr{T}_2$）为$A'$上的拓扑，由D'（分别$X'$）上简单收敛的拓扑引起。那么$\mathscr{T}_1$是可度量的，$\mathscr{T}_2$是紧致的，更细比$\mathscr{T}_1$强，因而$\mathscr{T}_1$和$\mathscr{T}_2$重合；在其他字中，$A'$是$\mathscr{C}_s(X')$的紧凑*可度量*子空间。因而，存在从$(f'_n)$提取并收敛到$\mathscr{C}_s(X')$的元素$f'$的序列$(f'_{n_k})$。因而，序列$(f_{n_k})$在$\mathscr{C}_s(X)$收敛到$f = f' \circ \phi$。

(ii) $\Rightarrow$ (iii) ：这很清楚。

(iii) $\Rightarrow$ (iv) ：假设 A 的元素的每个无限序列在 $\mathscr{C}_s(X)$ 中都有极限点。让$x \in X$。从A到K的映射$\phi_x : f \mapsto f(x)$是连续的。因而，$\phi_x(A)$中的每个无限序列都有极限点；由于域 K（等于$\mathbf{R}$或$\mathbf{C}$）是可度量的，集合$\phi_x(A)$在K中相对紧凑，因此是有界的。在其他字中，我们有$\sup_{f \in A} |f(x)| < \infty$。

令$f_n, x_m, \gamma$和$\delta$如(iv)中所示。令$\mathscr{C}_s(X)$中$f$为序列$(f_n)$的极限点，并令$x$为紧凑空间中序列$(x_m)$的极限点 X。对于每个$m$，从$\mathscr{C}_s(X)$到K的映射$h \mapsto h(x_m)$是连续的。根据假设，我们有$f(x_m) = \lim_{n \to \infty} f_n(x_m)$，因此有$\gamma = \lim_{m \to \infty} f(x_m)$；因为$f : X \to K$是连续的，并且$x$是序列$(x_m)$的极限点，所以我们得到$\gamma = f(x)$。类似地，我们证明等式$\delta = f(x)$，从而$\gamma = \delta$。

(iv) $\Rightarrow$ (i)：假设数$f(x)$的集合，因为$f$范围在A上，对于所有$x \in X$来说，在K中是有界的。这相当于假设 A 在乘积空间 $K^X$ 中的闭包 $\overline{A}$ 是紧凑的（GT，I, § 9, No. 5）。假设 A * 在 * $\mathscr{C}_s(X)$ 中不是相对紧的。这意味着存在函数$u \in \overline{A}$和点$a \in X$，使得$u$在$a$处不连续。因此，存在实数$\varepsilon > 0$，使得在$a$的每个邻域U中，都存在点$x$和$|u(x) - u(a)| \geq \varepsilon$。

我们将D中的点归纳序列$(x_n)_{n \in \mathbf{N}}$构造和A中的元素序列$(f_n)_{n \in \mathbf{N}}$，满足以下关系：

(1)$_m$$$ |u(x_m) - u(a)| \geq \varepsilon \quad \text{for} \quad m \geq 1 ; $$

(2)$_m$$$ |u(x_i) - f_m(x_i)| \leq \frac{1}{m + 1} \quad \text{for} \quad 0 \leq i \leq m - 1 ; $$

(3)$_{m,i}$$$ |f_m(x_i) - f_m(a)| \leq \frac{1}{i + 1} \quad \text{for} \quad 0 \leq m \leq i . $$

我们在A中任意取$x_0 = a$和$f_0$（集合A不为空，否则在$\mathscr{C}_s(X)$中会相对紧凑）。让$n \geq 1$和$x_0, x_1, ..., x_{n-1}, f_0, f_1, ..., f_{n-1}$满足关系（1）$_m$，（2）$_m$代表$1 \leq m < n$，（3）$_{m,i}$代表$0 \leq m \leq i < n$。从$u$属于到$\overline{A}$，存在$f_n \in A$满足(2)$_n$。令$V_n$为所有$x \in X$中的集合，使得$|f_m(x) - f_m(a)| \leq \frac{1}{n + 1}$对应$0 \leq m \leq n$。由于$f_n$是连续的，$V_n$是$a$的邻域； 选择点$x_n$在$D \cap V_n$中使得$|u(x_n) - u(a)| \geq \varepsilon$，因此满足(1)$_n$和(3)$_{m,n}$。因而，构造可以继续。

由于$u(X)$是K的紧子集，因此存在从$(x_m)$提取的序列$(y_k)$，并且存在极限$\gamma = \lim_{k \to \infty} u(y_k)$。到 (2)$_m$，我们对所有 $i \in \mathbf{N}$ 都有 $u(x_i) = \lim_{n \to \infty} f_n(x_i)$，因而

(4) $$
\gamma = \lim_{k \to \infty} \lim_{n \to \infty} f_n(y_k) .
$$

另一方面，我们通过 (3)$_{m,i}$ 得到 $f_n(a) = \lim_{i \to \infty} f_n(x_i)$，因此有 $f_n(a) = \lim_{k \to \infty} f_n(y_k)$。从$x_0 = a$开始，我们从(2)$_m$推出$\lim_{n \to \infty} f_n(a) = u(a)$。最后，

$$
u(a) = \lim_{n \to \infty} \lim_{k \to \infty} f_n(y_k) .
$$

最后，从(1)$_m$，我们得到$|\gamma - u(a)| \geq \varepsilon$，所以$\gamma \neq u(a)$。这个与……矛盾断言(iv);这样我们就证明了(iv)蕴涵(i)。

### 3. 埃伯莱因和斯穆利安定理

#### 定理 1（埃伯莱因）{#evt-iv-s5-thm-1 .statement tag=07VT}

— *设 E 为 Hausdorff 且 E 上的拟完全局部凸空间、$\mathscr{T}$ 拓扑，这与 E 和 E' 之间的对偶性以及 E 的 A 子集兼容。为了使 A 对于 $\mathscr{T}$ 相对紧，必要且充分的是 A 的点的每个无限序列有E 中的极限点代表 $\mathscr{T}$。*

条件的规定显然是必要的。

现在假设 A 的点的每个无限序列对于 $\mathscr{T}$ 都有极限点，因此也对于较粗糙的拓扑 $\sigma(E, E')$。那么 A 对于 $\mathscr{T}$ (IV, p. 32, prop. 1) 是预紧的；在阶中，A 对于$\mathscr{T}$ 是相对紧凑的，对于 $\sigma(E, E')$ 来说是相对紧凑的（*loc.cit.*）。因而，当$\mathscr{T}$是弱化的拓扑$\sigma(E, E')$时，证明定理就足够了。

令 $\hat{E}$ 表示 E 的完备性，我们将照常将其认同与 E' 的代数对偶 ${E'}^*$ 的子空间 (III, p. 21, th.2)。令$E_\sigma$、$\hat{E}_\sigma$和${E_\sigma'}^*$分别表示空间E、$\hat{E}$和${E'}^*$，分别赋予拓扑$\sigma(E, E')$、$\sigma(\hat{E}, E')$和$\sigma({E'}^*, E')$。

设$(x'_i)_{i \in I}$是向量空间E'在域K上的基。映射$f \mapsto (f(x'_i))_{i \in I}$是从${E_\sigma'}^*$到$K^I$的同胚$\phi$；对于从 E 到 K 的映射 $x'_i$ 下的 A 的每个 $i \in I$、像是相对紧凑的：因为，K 是可度量的，$x'_i(A)$ 的元素的每个无限序列都有极限点。由此可见，$\phi(A)$在$K^I$中相对紧致，因此A在${E_\sigma'}^*$中的闭包$\overline{A}$是紧致的。

*接下来我们要证明$\overline{A}$包含在$\hat{E}$中。*设H是E'的等连续子集；设 X 为 $\sigma(E', E)$ 的闭包； X 是紧凑的（III，p. 17，cor.2）。对于每个$x \in {E'}^*$，令$\phi_x$为$x' \mapsto \langle x, x' \rangle$到X中的限制；当x在A范围内时，令$\tilde{A} \subset \mathscr{C}_s(X)$为函数$\phi_x$的集合。鉴于A上的假设，$\tilde{A}$的元素的每个无限序列在$\mathscr{C}_s(X)$中都有极限点；通过道具。 2 (IV, p. 33), 集合 $\tilde{A}$ 因此在 $\mathscr{C}_s(X)$ 中相对紧凑。 *因此，对于每个$a \in \overline{A}$，函数$\phi_a$在X上是连续的。*包含于$\overline{A} \subset \hat{E}$然后从th开始。 2 个III、p. 21。

*现在我们将证明 $\overline{A}$ 包含在 E 中。* 由于 A 在 $E_\sigma$ (IV, p. 32, 命题 1) 中是预紧的，它的边界在 $E_\sigma$ (III, p. 3, 命题 2) 中，因此也在 E (IV, p. 1，道具 1)。 令 C 为 A 在 E 中的封闭凸平衡包络线。 那么 C 是有界的，因为 A 是有界的，因此是完备的，因为 E 是准完备的。 在其他字中，C是$\hat{E}$的凸且封闭的子集，因此也是$\hat{E}_\sigma$（IV，p. 1，道具1）。 由于$A \subset C$和$\hat{E}_\sigma$的拓扑是由${E_\sigma'}^*$的拓扑归纳的，所以我们有$\overline{A} \subset C$，因此有$\overline{A} \subset E$。

由于$E_\sigma$的拓扑是由${E'_\sigma}^*$的拓扑归纳而来，$E_\sigma$的子集$\overline{A}$是紧的，并且th。 1如下。

#### 定理 2 (Šmulian) {#evt-iv-s5-thm-2 .statement tag=07VU}

— *令 E 为 E 的 Fréchet 空间和 A 子集。令 $E_\sigma$ 表示赋予弱化拓扑的空间 E。以下条件是等效的*：

(i) *在 $E_\sigma$ 中相对紧凑；*
(ii) *A 的点的每个无限序列在 $E_\sigma$ 中都有极限点；*
(iii) *从A的点的每个无限序列，我们可以提取收敛于$E_\sigma$的序列。*

(i) 和 (ii) 的等价由 Eberlein 的定理得出，而 (iii) 显然意味着 (ii)。

我们将证明(i)蕴涵(iii)。假设$E_\sigma$中A的闭包B是紧的，并且$(x_n)_{n \in \mathbf{N}}$是A的点的序列。设F表示E 包含和$x_n$的最小的闭包向量子空间，这是一个Fréchet 空间满足可数性第一公理。由于 F 在 $E_\sigma$ 上闭，并且 F 上的拓扑 $\sigma(F, F')$ 由 $\sigma(E, E')$ 诱发，因此集合 $B \cap F$ 对于 $\sigma(F, F')$ 是紧致的。由于IV、p. 32中的注，从$(x_n)_{n \in \mathbf{N}}$收敛到$\sigma(E, E')$（或者，对于$\sigma(F, F')$也是一样）提取的序列的存在性是以下引理的推论：

#### 引理 1 {#evt-iv-s5-lem-1 .statement tag=07VV}

— *设 F 是 Fréchet 空间满足可数性第一公理。 F 的每个子集 C 对于$\sigma(F, F')$ 引起的拓扑 $\mathscr{T}$ 是紧致的，对于这个拓扑都是可度量的。*

由于 $F'$ 上预紧收敛的拓扑比拓扑 $\sigma(F', F)$ 更细，因此$F'_s$ 中存在处处稠密可数子集（III，p. 18，cor.1）。 因此，集合C可以与$K^D$的子集识别，并且由$K^D$在C上诱导的拓扑，可度量（GT，IX, § 2, No. 8）比$\sigma(F, F')$诱导的拓扑更粗糙，其中C 是紧凑的。 因此，这两种拓扑是相同的（GT，I, § 9, No. 4，cor.3）。

Šmulian 的定理可以推广到 E 是 Fréchet 空间的序列的严格归纳极限（IV，p. 67，练习 2）的情况。

### \*4。有界连续函数* 空间的情况

对于每个拓扑空间 X，令 $\mathscr{C}^b(X)$ 表示从 X 到 K 的所有连续和*有界* 映射的 Banach 空间，其中范数定义为

$$
\| f \| = \sup_{x \in X} |f(x)|
$$

（GT，X, § 3, No. 2）。当X紧致时，X上的每个连续函数都是有界的（GT，IV, § 6, No. 1），我们将$\mathscr{C}^b(X)$写为$\mathscr{C}(X)$。

在这个和下面的截面中，我们将使用下面的引理，这是勒贝格的定理（INT，IV，第二版§ 4, No. 3，第2版）的特例，因为将$\mathscr{C}(X)'$的元素解释为X的措施。

#### 引理 2 {#evt-iv-s5-lem-2 .statement tag=07VW}

设 X 为紧致空间。如果序列 $(f_n)_{n \in \mathbf{N}}$ 有界于 $C(X)$ 并简单地在 X 上收敛到连续的函数 f，则对于 $C(X)'$ 中的每个 $\mu$ 都有 $\mu(f) = \lim_{n \to \infty} \mu(f_n)$。

#### 命题 3 {#evt-iv-s5-prop-3 .statement tag=07VX}

令X为紧致空间，并令A为$C(X)$的有界子集。为了使 A 对于简单收敛的拓扑相对紧凑，它对于 $\sigma(C(X), C(X)')$ 相对紧凑是充分必要的。

简单收敛的拓扑是 Hausdorff，并且比 $\sigma(C(X), C(X)')$ 更粗糙，因此规定的条件是足够的（GT，I, § 9, No. 4，cor. 3）。

现在假设 A 对于拓扑的简单收敛来说是相对紧凑的。令 $(f_n)_{n \in \mathbf{N}}$ 为 A 的元素序列。 2（IV，p. 33），存在从$(f_n)$提取的序列$(f_{n_k})$并简单地收敛到连续的函数f。到引理 2 时，有界序列 $(f_{n_k})$ 趋向于 f 对于 $\sigma(C(X), C(X)')$。那么 Šmulian 的定理 (IV, p. 36, th. 2) 表明 A 对于 $\sigma(C(X), C(X)')$ 是相对紧凑的。

#### 推论 {#evt-iv-s5-n4-cor-1 .statement tag=07VY}

设 S 为拓扑空间，A 为 $C^b(S)$ 有界子集。以下条件是等价的：
(i) A 对于 $\sigma(C^b(S), C^b(S'))$ 是相对紧凑的；
(ii) 如果$(f_n)_{n \in \mathbf{N}}$是A的元素的序列并且$(x_m)_{m \in \mathbf{N}}$是S的点的序列，使得迭代的极限
$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$
存在，则$\gamma = \delta$。

令 X 为 S (GT, IX, § 1, No. 6) 和 $\alpha$ 典范映射从 S 到 X 的 Stone-Čech 紧化。设 D = $\alpha(S)$。 映射 $\phi : f \mapsto f \circ \alpha$ 是从范数空间 $C(X)$ 到范数空间 $C^b(S)$ 的同构；把$\tilde{A} = \phi^{-1}(A)$。由于 X 是紧致的，并且 D 在 X 中是稠密的，所以道具。 2 (IV, p. 33) 表明条件 (ii) 等价于$\tilde{A}$ 对于简单收敛的拓扑的紧致性。 (i) 和 (ii) 的等价由命题得出。 3.\*

### \*5。弱紧集的凸包络

#### 定理 3（克林）{#evt-iv-s5-thm-3 .statement tag=07VZ}

令 E 为 Hausdorff 且拟完全局部凸空间，并令 $\mathscr{T}$ 为 E 上的拓扑，与 E 和 E' 之间的对偶性兼容。设 A 为 E 的子集，它对于 $\mathscr{T}$ 是紧致的。那么 A 的闭凸平衡包络线 C 对于 $\mathscr{T}$ 是紧致的。

我们首先要进行一些削减。
A) 集合 C 是 $\mathscr{T}$ 的预紧式（II、p. 25，命题 3），而 A 是 $\sigma(E, E')$ 的紧式。由于道具。 1 (IV, p. 32)，足以证明C对于$\sigma(E, E')$是紧的，因此我们简化为$\mathscr{T} = \sigma(E, E')$的情况。
B) 由于 C 是预紧的并且对于 $\sigma(E, E')$ 是封闭的，因此它对于 E 的初始拓扑是有界且封闭的（III，p. 3，道具 2 和 IV，p. 1，道具 1）；因此它是完备的，因为 E 是准完备的。在其他字中，C是$E$的补全$\hat{E}$中$A$的闭凸平衡包络线。从$E$上的拓扑$\sigma(\hat{E}, E')$诱导$\sigma(E, E')$开始，我们已经减少*到$E$完成时的情况*。

C) 设$\Gamma$为$A$的凸平衡包络线。那么$C$就是$\Gamma$对于$\sigma(E, E')$的闭包。由Eberlein的定理（IV，p. 35，第1），足以证明$\Gamma$的点的每个序列$(x_n)_{n \in \mathbf{N}}$对于$\sigma(E, E')$有极限点 $E$。但是$x_n$属于到$A$的凸平衡包络线有限子集$B_n$。令$F$为由可数集合$B = \bigcup_n B_n$生成的$E$的闭向量子空间。然后$F$是完整的，$F$上的拓扑$\sigma(F, F')$是由$\sigma(E, E')$诱导的，并且对于所有$n \in \mathbf{N}$我们有$x_n \in F$。因此，只要证明$(x_n)_{n \in \mathbf{N}}$对于$\sigma(F, F')$有极限点，当$E$*中存在可数稠密集合时，就可以归约到*情况。

让$A$被分配由$\sigma(E, E')$诱导的拓扑，这使其成为紧凑的空间。我们定义线性映射$u : E' \to \mathscr{C}(A)$

$$
u(x')(a) = \langle a, x' \rangle \quad (a \in A, x' \in E') .
$$

令$(x'_n)_{n \in \mathbf{N}}$为$E'$中的等连续序列，对于$\sigma(E', E)$收敛于0。那么函数 $u(x'_n)$ 的序列以 $\mathscr{C}(A)$ 为界，简单地收敛于 0。对于每个 $\mu \in \mathscr{C}(A)'$，我们有 $\lim_{n \to \infty} \mu(u(x'_n)) = 0$ × 引理 2 (IV, p. 37)。根据III、p. 21、线性形式、$\mu \circ u$中$E'$中注给出的标准，对于每个$\mu \in \mathscr{C}(A)'$，对于$\sigma(E', E)$是连续的。因此存在线性映射 $v : \mathscr{C}(A)' \to E$ 满足关系

$$
\langle u(x'), \mu \rangle = \langle v(\mu), x' \rangle \quad (x' \in E', \mu \in \mathscr{C}(A)') .
$$

显然，如果$\mathscr{C}(A)'$被赋值为拓扑$\sigma(\mathscr{C}(A)', \mathscr{C}(A))$和$E$拓扑$\sigma(E, E')$，则$v$是连续的。

Banach 空间 $\mathscr{C}(A)$ 的单位球（闭合）$B$ 紧凑适用于拓扑 $\sigma(\mathscr{C}(A)', \mathscr{C}(A))$（III、p. 17、cor.3）。因而，$v(B)$ 是$\sigma(E, E')$ 的$E$ 的凸平衡且紧凑的子集。对于每个$a \in A$，$\mathscr{C}(A)$属于到$B$的连续线性形式$\varepsilon_a : f \mapsto f(a)$，我们通过公式（7）和（8）得到$v(\varepsilon_a) = a$。因而，$A \subset v(B)$，等等$C \subset v(B)$。这证明$C$对于$\sigma(E, E')$是紧致的。

Q.E.D.

### 习题 {#evt-iv-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
