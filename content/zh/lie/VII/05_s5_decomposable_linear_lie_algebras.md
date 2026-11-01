---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 5
section_title: Decomposable linear Lie algebras
lang: zh
source: lie-vii-ix
book_pages: 34-45, 63-66
pdf_pages: 0044-0055, 0072-0075
extraction: native
subsections:
    - "no": 1
      title: DECOMPOSABLE LINEAR LIE ALGEBRAS
      page: 34
      pdf_page: 44
    - "no": 2
      title: DECOMPOSABLE ENVELOPE
      page: 37
      pdf_page: 47
    - "no": 3
      title: DECOMPOSITIONS OF DECOMPOSABLE ALGEBRAS
      page: 37
      pdf_page: 47
    - "no": 4
      title: LINEAR LIE ALGEBRAS OF NILPOTENT ENDOMORPHISMS
      page: 39
      pdf_page: 49
    - "no": 5
      title: CHARACTERIZATIONS OF DECOMPOSABLE LIE ALGEBRAS
      page: 43
      pdf_page: 53
statements: 29
exercises: 11
content_sha256: caaf271d1475da4c2e5d9d125e6e2682d3a4f6a2ed5e7cdeae5ca12a82f2c034
translated_from: content/en/lie/VII/05_s5_decomposable_linear_lie_algebras.md
translation_method: google
source_content_sha256: 9348eb1c66b5306a2d380eb335d4afb9f19486f3e78d4da673c181842d07b2e0
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 60bd84be27874044644bbed9b4f976f0748c04dec71475df6ec66cdc306e47f3
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。可分解线性李代数

在本段中，假设$k$的特征为0。我们用V表示有限维向量空间。

### 1. 可分解线性李代数

#### 定义 1 {#lie-vii-s5-def-1 .statement tag=00WG}

设$\mathfrak{g}$是$\mathfrak{g}\mathfrak{l}(V)$的谎言子代数。那么 $\mathfrak{g}$ 被认为是可分解的，如果 $\mathfrak{g}$ 包含半单并且它的每个元素的幂零分量（代数，第 VII, §5, no. 8）。

#### 例 1 {#lie-vii-s5-n1-exa-1 .statement tag=00WH}

令$V'$和$V''$为V的向量子空间，使得$V''\supset V'$。 $x\in \mathfrak{g}\mathfrak{l}(V)$的集合使得$x(V'')\subset V'$是$\mathfrak{g}\mathfrak{l}(V)$的可分解谎言子代数；事实上，对于所有$x\in \mathfrak{g}\mathfrak{l}$(V)、半单和$x$的幂零分量都是形式、$P(x)$和$Q(x)$，其中P和Q是没有常数项的多项式。

#### 例 2 {#lie-vii-s5-n1-exa-2 .statement tag=00WI}

假设V有代数结构。 V 的推导的集合是 $\mathfrak{g}\mathfrak{l}(V) ($§1, no. 1 的可分解谎言子代数，命题 4 (ii)）。

#### 例 3 {#lie-vii-s5-n1-exa-3 .statement tag=01KQ}

更一般地，可以证明 $\mathbf{G}\mathbf{L}(V)$ 的任何代数子群的李代数都是可分解的。\*

#### 命题 1 {#lie-vii-s5-prop-1 .statement tag=00WJ}

令$\mathfrak{g}$为$\mathfrak{g}\mathfrak{l}(V),x\in \mathfrak{g},s$和$n$半单的可分解李子子代数以及$x$的幂零分量。

(i) ad$_{\mathfrak{g}}x$的半单和幂零分量分别是ad$_{\mathfrak{g}}s$和ad$_{\mathfrak{g}}n$。

(ii) $x$ 在 $\mathfrak{g}$ 中是正则的当且仅当 $s$ 是。

(iii) 如果$\mathfrak{g}'$是$\mathfrak{g}\mathfrak{l}(V)$包含$\mathfrak{g}$的子代数，则$\mathfrak{g}$扩展的每个初等自同构到$\mathfrak{g}'$的初等自同构。

输入$\mathfrak{a}=\mathfrak{g}\mathfrak{l}(V)$。由章。 ad$_{\mathfrak{a}}x$的I, §5, no. 4、引理2、半单和幂零分量是ad$_{\mathfrak{a}}s$和ad$_{\mathfrak{a}}n$；由此得出断言 (i)。我们推导出ad$_{\mathfrak{g}}x$和ad$_{\mathfrak{g}}s$的特征多项式是相同的；因此(ii)。如果 ad$_{\mathfrak{g}}x$ 幂零的，则 ad$_{\mathfrak{g}}x=$ ad$_{\mathfrak{g}}n$，因此 ad$_{\mathfrak{g}'}n$ 扩展 ad$_{\mathfrak{g}}x$，并且 $n$ 是 $\mathfrak{g}'$ 的幂零元，因此 (iii)。

设$\mathfrak{g}$是$\mathfrak{g}\mathfrak{l}(V)$的谎言子代数。我们知道（第 I, §6, no. 5，第 4 章）以下条件是等效的：

(i) $\mathfrak{g}$的身份表示是半单；

(ii) $\mathfrak{g}$ 是约数，$\mathfrak{g}$ 中心的每元素是半单自同态。

这些条件实际上相当于以下内容：

(iii) $\mathfrak{g}$ 是$\mathfrak{g}\mathfrak{l}(V)$ 中的约子代数。

事实上，(i) $=\Rightarrow$ (iii) 由第 1 章提供。 I, §6, no. 5，科。 3 Th。 4，和（iii）$=\Rightarrow$（i）章。 I, §6, no. 6，科。提案 7 的第 1 条。我们将证明，如果 $\mathfrak{g}$ 满足这些条件，则 $\mathfrak{g}$ 是可分解的。更一般地说：

#### 命题 2 {#lie-vii-s5-prop-2 .statement tag=00WK}

令 $\mathfrak{g}$ 为 $\mathfrak{g}\mathfrak{l}(V)$ 中 $\mathfrak{g}\mathfrak{l}(V)$ 约简的谎言子代数，E 为有限维向量空间，E 上 $\mathfrak{g}$ 的 $\pi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(E)$ 半单线性表示。则：

(i) $\mathfrak{g}$ 和 $\pi (\mathfrak{g})$ 是可分解的。

(ii) The semi-simple (resp. nilpotent) elements of $\pi (\mathfrak{g})$ are the images under $\pi$ of the semi-simple (resp. nilpotent) elements of $\mathfrak{g}$.

(iii) If $\mathfrak{h}$ is a decomposable subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ contained in $\mathfrak{g},\pi (\mathfrak{h})$ is a decomposable subalgebra of $\mathfrak{g}\mathfrak{l}(E)$.

(iv) 如果$\mathfrak{h}'$是$\mathfrak{g}\mathfrak{l}(E),\pi^{-1}(\mathfrak{h}')$的可分解的子代数，则子代数是$\mathfrak{g}\mathfrak{l}(V)$的可分解的子代数。

令$\mathfrak{s}= [\mathfrak{g},\mathfrak{g}]$且$\mathfrak{c}$为$\mathfrak{g}$的中心。 然后是$\mathfrak{g}=\mathfrak{s}\times \mathfrak{c}$和$\pi (\mathfrak{g}) =$$\pi (\mathfrak{s})\times \pi (\mathfrak{c})$。 I, §6, no. 4，科。提案 5。 让$y\in \mathfrak{s}, z\in \mathfrak{c}, y_s$和$y_n$半单以及$y$的幂零分量。 那么$y_s, y_n\in \mathfrak{s}$（第I, §6, no. 3章，提案$3$）$,y_s+z$是半单（代数，第VII, §5, no. 7章，第16号提案的Cor.），并且$y_n$与$y_s+z$通勤。 因此，半单和$y+z$的幂零分量是$y_s+z$和$y_n$。 因此，$\mathfrak{g}$是可分解的。 由于 $\pi (\mathfrak{g})$ 在 $\mathfrak{g}\mathfrak{l}$(E) 中是可还原的，因此相同的论证适用于 $\pi (\mathfrak{g})$ 并表明 $\pi (\mathfrak{g})$ 是可分解的。 此外，$\mathfrak{g}$（或$\pi (\mathfrak{g})$）的幂零元是$\mathfrak{s}$（或$\pi (\mathfrak{s})$）的幂零元。 因此，$\pi (\mathfrak{g})$的幂零元是$\mathfrak{g}$的幂零元的$\pi$下的像（第I, §6, no. 3章，第4条命题）。 The semi-simple elements of $\mathfrak{g}$ (resp. $\pi (\mathfrak{g})$) are the sums of the semi-simple elements of $\mathfrak{s}$ (resp. $\pi (\mathfrak{s})$) and the elements of $\mathfrak{c}$ (resp. $\pi (\mathfrak{c})$). 因此，$\pi (\mathfrak{g})$的半单元素是像在半单元素的$\pi$之下，$\mathfrak{g}$（第I章，前述）。 因此(ii)。

断言 (iii) 和 (iv) 紧随 (i) 和 (ii) 之后。

#### 注 1 {#lie-vii-s5-n1-rem-1 .statement tag=00WL}

$\pi$ 上的半单纯性假设相当于说，对于所有$x\in \mathfrak{c}$，$\pi (x)$ 是半单。 注，当通过连续应用以下运算：张量积、通向对偶、子表示、商、直和，从恒等式表示$\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(V)$获得$\pi$时，满足假设。

#### 注 2 {#lie-vii-s5-n1-rem-2 .statement tag=00WM}

设$\mathfrak{g}\subset \mathfrak{g}\mathfrak{l}$(V)、$\mathfrak{g}'\subset \mathfrak{g}\mathfrak{l}(V')$为可分解李代数、$\varphi$同构，从$\mathfrak{g}$到$\mathfrak{g}'$。 注 $\varphi$ 不一定是 $\mathfrak{g}$ 的变换半单（幂幂）元素到半单（幂幂）元素 $\mathfrak{g}'$（练习 2）。然而，如果$\mathfrak{g}$是半单（第I, §6, no. 3章，第3章），就会出现这种情况。

#### 命题 3 {#lie-vii-s5-prop-3 .statement tag=00WN}

令$\mathfrak{a}$为$\mathfrak{g}\mathfrak{l}(V)$的可分解谎言子代数，并令$\mathfrak{b}$和$\mathfrak{c}$为$\mathfrak{g}\mathfrak{l}(V)$的向量子空间，使得$\mathfrak{b}\subset \mathfrak{c}$。令$\mathfrak{a}'$为$x\in \mathfrak{a}$的集合，使得$[x,\mathfrak{c}]\subset \mathfrak{b}$。那么$\mathfrak{a}'$是可分解的。

把$\mathfrak{g}=\mathfrak{g}\mathfrak{l}(V)$； $z\in \mathfrak{g}\mathfrak{l}(\mathfrak{g})$的$\mathfrak{g}\mathfrak{l}(\mathfrak{g})$由……组成的子代数$\mathfrak{h}'$使得$z(\mathfrak{c})\subset \mathfrak{b}$可分解（例1）。令$\pi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(\mathfrak{g})$为$\mathfrak{g}$的伴随表示。应用于 $\pi$ 的命题 2 (iv) 表明 $\pi^{-1}(\mathfrak{h}')$ 是可分解的。因而$\mathfrak{a}'=\mathfrak{a}\cap \pi^{-1}(\mathfrak{h}')$也是如此。

#### 推论 1 {#lie-vii-s5-prop-3-cor-1 .statement tag=00WO}

如果$\mathfrak{a}$是$\mathfrak{g}\mathfrak{l}(V)$的可分解谎言子代数，并且$\mathfrak{n}$是$\mathfrak{a}$的谎言子代数，则$\mathfrak{a}$中$\mathfrak{n}$的归一化器（或中心化器）是可分解的。

这是通过取$\mathfrak{c}=\mathfrak{n},\mathfrak{b}=\mathfrak{n}$（或$\mathfrak{c}=\mathfrak{n},\mathfrak{b}=\{0\}$）得出的命题3。

#### 推论 2 {#lie-vii-s5-prop-3-cor-2 .statement tag=00WP}

可分解谎言的嘉当子代数 $\mathfrak{g}\mathfrak{l}(V)$ 的子代数是可分解的。

这是从推论 1 得出的。

#### 注 {#lie-vii-s5-n1-rem-3 .statement tag=00WQ}

我们稍后将证明 Cor 的 (no. 5, Th.2) 逆命题。 2.

### 2. 可分解包络

可分解李族的交$\mathfrak{g}\mathfrak{l}(V)$的子代数显然是可分解的。因而，如果$\mathfrak{g}$是$\mathfrak{g}\mathfrak{l}$(V)的谎言子代数，则$\mathfrak{g}\mathfrak{l}(V)$包含$\mathfrak{g}$的可分解谎言子代数的集合有最小的元素，称为$\mathfrak{g}$的可分解包络；在本段中，该信封将用 $e(\mathfrak{g})$ 表示。

#### 命题 4 {#lie-vii-s5-prop-4 .statement tag=00WR}

令$\mathfrak{g}$为$\mathfrak{g}\mathfrak{l}(V)$的谎言子代数，而$\mathfrak{n}$为$\mathfrak{g}$的理想。那么$\mathfrak{n}$和$e(\mathfrak{n})$是$e(\mathfrak{g})$和$[e(\mathfrak{g}), e(\mathfrak{n})] = [\mathfrak{g},\mathfrak{n}]$的理想。

令$\mathfrak{g}_1$为$x\in \mathfrak{g}\mathfrak{l}(V)$的集合，使得$[x,\mathfrak{n}]\subset [\mathfrak{g},\mathfrak{n}]$。这是 $\mathfrak{g}\mathfrak{l}$(V)、包含 $\mathfrak{g}$ 的可分解谎言子代数，因而$e(\mathfrak{g})$、cf. no. 1，命题 3；其他字、$[e(\mathfrak{g}),\mathfrak{n}]\subset [\mathfrak{g},\mathfrak{n}]$。令 $\mathfrak{n}_1$ 为 $y\in \mathfrak{g}\mathfrak{l}(V)$ 的集合，使得

$$
[e(\mathfrak{g}), y]\subset [\mathfrak{g},\mathfrak{n}]
$$

这是前面的 $\mathfrak{g}\mathfrak{l}(V)$ 包含 $\mathfrak{n}$ 的可分解谎言子代数，因此是包含 $e(\mathfrak{n})$；其他字$[e(\mathfrak{g}), e(\mathfrak{n})]\subset [\mathfrak{g},\mathfrak{n}]$，所以

$$
[e(\mathfrak{g}), e(\mathfrak{n})] = [\mathfrak{g},\mathfrak{n}]
$$

由此可见$[e(\mathfrak{g}),\mathfrak{n}]\subset [e(\mathfrak{g}), e(\mathfrak{n})]\subset \mathfrak{n}$，因而$\mathfrak{n}$和$e(\mathfrak{n})$是$e(\mathfrak{g})$的理想。

#### 推论 1 {#lie-vii-s5-prop-4-cor-1 .statement tag=00WS}

(i) $\mathscr{D}^i\mathfrak{g}=\mathscr{D}^ie(\mathfrak{g})$ 代表$i\geq 1$，$\mathscr{C}^i\mathfrak{g}=\mathscr{C}^ie(\mathfrak{g})$ 代表$i\geq 2$。

(ii) 如果 $\mathfrak{g}$ 是可交换的（或幂零、或可解），则 $e(\mathfrak{g})$ 是可交换的（或幂零、或可解）。

断言 (i) 由 $i$ 上的归纳由第 4 条命题得出，(ii) 由 (i) 得出。

#### 推论 2 {#lie-vii-s5-prop-4-cor-2 .statement tag=00WT}

设$\mathfrak{r}$为$\mathfrak{g}$的根式。如果 $\mathfrak{g}$ 可分解，则 $\mathfrak{r}$ 也可分解。

事实上，$e(\mathfrak{r})$ 是第 4 号提案和 Cor.4 的 $\mathfrak{g}$ 的可解理想。 1，因而$e(\mathfrak{r}) =\mathfrak{r}$。

### 3. 分解 / 可分解代数

如果$\mathfrak{g}$是$\mathfrak{g}\mathfrak{l}(V)$的谎言子代数且带有根$\mathfrak{r}$，则$\mathfrak{r}$的幂零元的集合是$\mathfrak{g}$的幂零理想，最大的恒等式表示的幂零理想$\mathfrak{g}$（第 I, §5, no. 3 章，第 1 章第 6 章）。在本段中，我们将用$\mathfrak{n}_V(\mathfrak{g})$来表示这个理想。它包含$\mathfrak{g}$的幂零根$[\mathfrak{g},\mathfrak{g}]\cap \mathfrak{r}$（第I, §5, no. 3章，第1章）。

#### 命题 5 {#lie-vii-s5-prop-5 .statement tag=00WU}

令 $\mathfrak{g}$ 为 $\mathfrak{g}\mathfrak{l}(V)$ 的可分解幂零谎言子代数。令$\mathfrak{t}$为集合/半单元素/$\mathfrak{g}$。那么$\mathfrak{t}$是$\mathfrak{g}$的中心子代数，$\mathfrak{g}$是$\mathfrak{t}$的乘积，$\mathfrak{n}_V(\mathfrak{g})$是李代数。

如果$x\in \mathfrak{t}$，ad$_{\mathfrak{g}}x$是半单且幂零，因此零，因而$x$是$\mathfrak{g}$的中心。因而，$\mathfrak{t}$是$\mathfrak{g}$和$\mathfrak{t}\cap \mathfrak{n}_V(\mathfrak{g}) = 0$的理想。由于$\mathfrak{g}$可分解，$\mathfrak{g}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$，因此命题。

#### 命题 6 {#lie-vii-s5-prop-6 .statement tag=00WV}

令 $\mathfrak{g}$ 为 $\mathfrak{g}\mathfrak{l}(V)$ 的可分解谎言子代数。设$\mathscr{T}$为半单元素$\mathfrak{g}$由……组成交换子代数集合，以及$\mathscr{T}$极大元素$\mathscr{T}_1$集合。令$\mathscr{H}$为$\mathfrak{g}$的嘉当子代数中的集合。

(i) 对于$\mathfrak{h}\in \mathscr{H}$，令$\varphi (\mathfrak{h})$为集合/半单元素/$\mathfrak{h}$。然后$\varphi (\mathfrak{h})\in \mathscr{T}_1$。

(ii) 对于$\mathfrak{t}\in \mathscr{T}_1$，令$\psi (\mathfrak{t})$为$\mathfrak{t}$在$\mathfrak{g}$的交换子。然后$\psi (\mathfrak{t})\in \mathscr{H}$。

(iii) 映射$\varphi$和$\psi$是从$\mathscr{H}$到$\mathscr{T}_1$以及从$\mathscr{T}_1$到$\mathscr{H}$的逆双射。

(iv) 如果 $k$ 是代数闭集，则 Aut$_e(\mathfrak{g})$ 在 $\mathscr{T}_1$ 上传递运算。

设$\mathfrak{h}\in \mathscr{H}$，并放入$\mathfrak{t}=\varphi (\mathfrak{h})$。根据 Prop. 5 和 Cor. $3,\mathfrak{t}\in \mathscr{T}$ 和 $\mathfrak{h}=\mathfrak{t}\times \mathfrak{n}_V(\mathfrak{h})$ 提案 2。对于$\mathfrak{g}$的任何子代数$\mathfrak{u}$，我们用$\psi (\mathfrak{u})$表示$\mathfrak{u}$在$\mathfrak{g}$的交换子。那么$\mathfrak{h}\subset \psi (\mathfrak{t})$和$\psi (\mathfrak{t})\subset \mathfrak{g}^0(\mathfrak{h})$，因为$\mathfrak{n}_V(\mathfrak{h})$的元素是幂零的，所以$\mathfrak{h}=\psi (\mathfrak{t})$。如果$\mathfrak{t}'\in \mathscr{T}$和$\mathfrak{t}\subset \mathfrak{t}'$，我们有$\mathfrak{t}'\subset \psi (\mathfrak{t}) =\mathfrak{h}$，所以$\mathfrak{t}'=\mathfrak{t}$，因此有$\mathfrak{t}\in \mathscr{T}_1$。

设$\mathfrak{t}\in \mathscr{T}_1$，并放入$\mathfrak{c}=\psi (\mathfrak{t})$。设$\mathfrak{h}$为$\mathfrak{c}$中的嘉当子代数。根据§2, no. 3、提案$10,\mathfrak{h}\in \mathscr{H}$ 和$\mathfrak{t}\subset \mathfrak{h}$。把$\mathfrak{t}_1=\varphi (\mathfrak{h})\in \mathscr{T}$。然后$\mathfrak{t}\subset \mathfrak{t}_1$所以$\mathfrak{t}=\mathfrak{t}_1$，以及前面的$\mathfrak{h}=\psi (\mathfrak{t}_1) =\psi (\mathfrak{t}) =\mathfrak{c}$。因此，$\psi (\mathfrak{t})\in \mathscr{H}$和$\varphi (\psi (\mathfrak{t})) =\mathfrak{t}$。

这样我们就证明了(i)、(ii)和(iii)。假设 $k$ 是代数闭的。由于 Aut$_e(\mathfrak{g})$ 在 $\mathscr{H}($§3, no. 2 上传递操作，Th。 1)、Aut$_e(\mathfrak{g})$在$\mathscr{T}_1$上传递操作。

#### 推论 1 {#lie-vii-s5-prop-6-cor-1 .statement tag=00WW}

$\mathfrak{g}$的嘉当子代数是半单元素的$\mathfrak{g}$的集中器。

如果$x\in \mathfrak{g}$是正则，则$\mathfrak{g}^0(x)$是$\mathfrak{g}($§2, no. 3的嘉当子代数，Th。 1（一））；此外，如果$x$是半单，则$\mathfrak{g}^0(x)$是$x$在$\mathfrak{g}$的集中器。相反，令$\mathfrak{h}$为$\mathfrak{g}$的嘉当子代数。存在$\mathfrak{t}\in \mathscr{T}_1$使得$\mathfrak{h}=\psi (\mathfrak{t})$。根据第7条命题§1, no. 2，存在$x\in \mathfrak{t}$使得$\mathfrak{h}=\mathfrak{g}^0(x)$；从$x\in \mathfrak{t}$、$\mathfrak{g}^0(x) =\mathfrak{g}_0(x)$开始。星期四 §3, no. 3 之前2 (ii), $x$ 是正则。

#### 推论 2 {#lie-vii-s5-prop-6-cor-2 .statement tag=00WX}

假设加法中$\mathfrak{g}$是可解的。然后：

(i) The subgroup of Aut($\mathfrak{g}$) consisting of the $e^{adx}, x\in \mathscr{C}^{\infty}\mathfrak{g}$ (cf. §3, no. 4), operates transitively on $\mathscr{T}_1$.

(ii) 如果$\mathfrak{t}\in \mathscr{T}_1,\mathfrak{g}$是$\mathfrak{t}$和$\mathfrak{n}_V(\mathfrak{g})$的半直接乘积。

断言 (i) 源自以下事实：$e^{adx},x\in \mathscr{C}^{\infty}\mathfrak{g}$ 的群在$\mathscr{H}($§3, no. 4、Th 上传递操作。 3）。

我们证明(ii)。令$\mathfrak{t}\in \mathscr{T}_1$，并令$\mathfrak{h}=\psi (\mathfrak{t})$为$\mathfrak{g}$的相应的嘉当子代数。鉴于提案$5,\mathfrak{h}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{h})\subset \mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$。另一方面，$\mathfrak{g}=\mathfrak{h}+ [\mathfrak{g},\mathfrak{g}] ($§2, no. 1，Cor。命题 4 中的 3) 和 $[\mathfrak{g},\mathfrak{g}]\subset \mathfrak{n}_V(\mathfrak{g})$，因此 $\mathfrak{g}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$。但很明显$\mathfrak{t}\cap \mathfrak{n}_V(\mathfrak{g}) =\{0\}$。因此，代数$\mathfrak{g}$是$\mathfrak{t}$的半直接乘积和理想的$\mathfrak{n}_V(\mathfrak{g})$。

#### 命题 7 {#lie-vii-s5-prop-7 .statement tag=00WY}

令 $\mathfrak{g}$ 为 $\mathfrak{g}\mathfrak{l}(V)$ 的可分解谎言子代数。

(i) 存在$\mathfrak{g}$的谎言子代数$\mathfrak{m}$，在$\mathfrak{g}\mathfrak{l}(V)$中还原，使得$\mathfrak{g}$是$\mathfrak{m}$和$\mathfrak{n}_V(\mathfrak{g})$的半直接乘积。

(ii) 具有 (i) 中属性的 $\mathfrak{g}$ 的任何两个谎言子代数在 Aut$_e(\mathfrak{g})$ 下都是共轭。

$\mathfrak{g}$的部首$\mathfrak{r}$是可分解的（no. 2，第4条命题的Cor.2）。由科.根据命题6的2，存在$\mathfrak{r}$的交换子代数$\mathfrak{t}$，半单元素的由……组成，使得$\mathfrak{r}=\mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{r})$。由于 ad$_{\mathfrak{g}}\mathfrak{t}$ 由半单元素组成，$\mathfrak{g}$ 是 $[\mathfrak{t},\mathfrak{g}]$ 的直和以及 $\mathfrak{t}$ 的扶正器 $\mathfrak{z}$（第 I, §3, no. 5 章，第 6 条）。从$[\mathfrak{t},\mathfrak{g}]\subset \mathfrak{r},\mathfrak{g}=\mathfrak{z}+\mathfrak{r}$开始。因而，如果$\mathfrak{s}$是$\mathfrak{z}$的李维子代数（第I, §6章，第$8$）$,\mathfrak{g}=\mathfrak{s}+\mathfrak{r}$，那么$\mathfrak{s}$是$\mathfrak{g}$的李维子代数。输入$\mathfrak{m}=\mathfrak{s}\oplus \mathfrak{t}$。由于$[\mathfrak{s},\mathfrak{t}] =\{0\},\mathfrak{m}$是$\mathfrak{g}$的谎言子代数，由第1章在$\mathfrak{g}\mathfrak{l}(V)$中还原。 I, §6, no. 5，周四。 4. 此外，

$$
\mathfrak{g}=\mathfrak{s}\oplus \mathfrak{r}=\mathfrak{s}\oplus \mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{r}) =\mathfrak{s}\oplus \mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{g}) =\mathfrak{m}\oplus \mathfrak{n}_V(\mathfrak{g})
$$

从$\mathfrak{n}_V(\mathfrak{g}) =\mathfrak{n}_V(\mathfrak{r})$开始。因而(i)。

现在让$\mathfrak{m}'$是$\mathfrak{g}$的谎言子代数与$\mathfrak{n}_V(\mathfrak{g})$互补并在$\mathfrak{g}\mathfrak{l}(V)$中还原。我们证明，在 Aut$_e(\mathfrak{g})$ 下，$\mathfrak{m}'$ 是共轭到 $\mathfrak{m}$。我们有$\mathfrak{m}'=\mathfrak{s}'\oplus \mathfrak{t}'$，其中$\mathfrak{s}'= [\mathfrak{m}',\mathfrak{m}']$是半单，$\mathfrak{m}'$的中心$\mathfrak{t}'$由半单元素组成。然后$\mathfrak{r}=\mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{g}) =\mathfrak{t}'\oplus \mathfrak{n}_V(\mathfrak{g})$。鉴于科尔。根据第 6 条命题 2，我们被简化为情况$\mathfrak{t}=\mathfrak{t}'$。然后$\mathfrak{s}'\subset \mathfrak{z}$；由于dim$\mathfrak{s}'=$dim$\mathfrak{s}$，$\mathfrak{s}'$是$\mathfrak{z}$的Levi 子代数。由章。 I, §6, no. 8，周四。 5、存在$x\in \mathfrak{n}_V(\mathfrak{z})$使得$e^{adx}(\mathfrak{s}) =\mathfrak{s}'$；由于$x$与$\mathfrak{t}$通勤，我们还有$e^{adx}(\mathfrak{t}) =\mathfrak{t}$。

### 4. 线性李代数幂零自同态

#### 引理 1 {#lie-vii-s5-lem-1 .statement tag=00WZ}

令 $\mathfrak{n}$ 为 $\mathfrak{g}\mathfrak{l}(V)$ 由……组成幂零自同态的谎言子代数，以及 $\mathbf{G}\mathbf{L}(V) ($§3, no. 1、引理 1 的 N 子群 exp$\mathfrak{n}$。

(i) 设$\rho$为W上$\mathfrak{n}$的有限维线性表示，使得$\rho (\mathfrak{n})$的元素幂零，W的$W'$向量子空间在$\rho ,\rho_1$和$\rho_2$下稳定子表示和由 N 的 $W',\pi , \pi_1, \pi_2$ 表示定义的 $\rho$ 的商表示与 $\rho , \rho_1, \rho_2($§3, no. 1 相容的）。那么$\pi_1, \pi_2$就是子表示和$W'$定义的$\pi$的商表示。

(ii) 令$\rho_1, \rho_2$为$\mathfrak{n}$的有限维线性表示，使得$\rho_1(\mathfrak{n})$和$\rho_2(\mathfrak{n})$的元素幂零，并且N的$\pi_1, \pi_2$表示与$\rho_1, \rho_2$相容的。那么$\pi_1\otimes \pi_2$是N中与$\rho_1\otimes \rho_2$兼容的表示。

(iii) 设$\rho_1, \rho_2$为向量空间$V_1,V_2$上$\mathfrak{n}$的有限维线性表示，使得$\rho_1(\mathfrak{n})$和$\rho_2(\mathfrak{n})$的元素幂零，$\rho$表示 $\mathfrak{n}$ 在 Hom(V$_1,V_2$) 由 $\rho_1, \rho_2$ 确定。令$\pi_1, \pi_2$为与$\rho_1, \rho_2$兼容的N的表示，以及由$\pi_1, \pi_2$确定的Hom(V$_1,V_2$)上的N的$\pi$表示。那么$\pi$是N中与$\rho$兼容的表示。

断言 (i) 很清楚。让 $\rho_1, \rho_2, \pi_1, \pi_2$ 如 (ii) 中所示。如果$x\in \mathfrak{n}$，自从$\rho_1(x)\otimes 1$和$1\otimes \rho_2(x)$通勤以来，我们有，

指数（$\rho_1(x)\otimes 1 + 1\otimes \rho_2(x)$）$=$ 指数（$\rho_1(x)\otimes 1$）。经验值(1 $\otimes \rho_2(x)$)

= (经验$\rho_1(x)$)$\otimes 1.1\otimes$ (经验$\rho_2(x)$)

= (经验$\rho_1(x)$)$\otimes$ (经验$\rho_2(x)$)

$=\pi_1$(预计$x$)$\otimes \pi_2$(预计$x$)

$= (\pi_1\otimes \pi_2$)(exp $x$),

因而(ii)。令 $\rho_1, \rho_2, \rho , \pi_1, \pi_2, \pi ,V_1,V_2$ 如 (iii) 中所示。如果 $v_1\in$ EndV$_1$ 和 $v_2\in$ EndV$_2$，则用 $R_{v_1}$ 和 $L_{v_2}$ 映射 $u \rightarrow uv_1$ 和 $u \rightarrow v_2u$ 从 Hom(V$_1,V_2$) 到自身；这些映射通勤和$\rho (x)u= (L_{\rho_2(x)}-R_{\rho_1(x)})u$，所以

经验$\rho (x).u=$ 经验$L_{\rho_2(x)}$。经验$R_{-\rho_1(x)}.u$

$$
= L_{exp\rho_2(x)}.R_{exp(-\rho_1(x))}.u
$$

$$
= L_{\pi_2(expx)}.R_{\pi_1(exp(-x))}.u
$$

$=\pi$(exp $x$)$.u$,

因而(iii)。

#### 引理 2 {#lie-vii-s5-lem-2 .statement tag=01JS}

$^2$ (i) 令W为维数$d$V向量子空间，D线$\bigwedge^dW\subset \bigwedge^dV,\theta$$\bigwedge V$上$\mathfrak{g}\mathfrak{l}(V)$标准表示（第1章） III，应用程序。）。让$x\in \mathfrak{g}\mathfrak{l}(V)$。那么$x(W)\subset W$当且仅当$\theta (x)(D)\subset D$。

(ii) 令$(e_1, . . . , e_n)$为$k^n,\theta$的典范基，以及$\bigwedge(k^n)$上$\mathfrak{g}\mathfrak{l}(n, k)$的规范表示，以及$x\in \mathfrak{g}\mathfrak{l}(n, k)$。那么 $x\in \mathfrak{n}(n, k)$ 当且仅当

$$
\theta (x)(e_{n-d+1}\wedge  \cdots  \wedge e_n) = 0
$$

$1\leq d\leq n$。

(i) 如果$x(W)\subset W$，则显然$\theta (x)D\subset D$。相反，假设$\theta (x)D\subset D$。令$u$为D的非零元素，并令$y\in W$。然后$y\wedge u= 0$。由于 $\theta (x)$ 是 $\bigwedge V$ 的推导，这意味着

$$
\theta (x)y\wedge u+y\wedge \theta (x)u= 0
$$

现在$\theta (x)u\in ku$，所以$y\wedge \theta (x)u= 0$，最终$\theta (x)y\wedge u= 0$。 代数，第 1 章III, §7, no. 9，第13条命题，这意味着$\theta (x)y\in W$，即$x(y)\in W$，从而证明了$x(W)\subset W$。

(ii) (ii) 中所述的条件对于$x\in \mathfrak{n}(n, k)$显然是必要的。假设它是满意的。到(i)为止，$x$离开

$^2$ 在这个引理中，$k$可以是任意（可交换的）域。

$$
ke_{n-d+1}+\cdots +ke_n
$$

稳定，因为 $d= 1, . . . , n,x$ 是下三角的。放

$$
x= (x_{ij})_{1\leq i,j\leq n}
$$

我们有$0 =x(e_n) =x_{nn}e_n$，所以$x_{nn}= 0$。让$i < n$，并假设我们已经证明了$x_{jj}= 0$对于$j > i$。然后

$$
0 =\theta (x)(e_i\wedge e_{i+1}\wedge  \cdots  \wedge e_n) =x_{ii}(e_i\wedge e_{i+1}\wedge  \cdots  \wedge e_n)
$$

所以$x_{ii}= 0$。因此，$x\in \mathfrak{n}(n, k)$。

#### 命题 8 {#lie-vii-s5-prop-8 .statement tag=00X0}

令$\mathfrak{n}$为$\mathfrak{g}\mathfrak{l}(V)$由……组成或幂零元的谎言子代数，$\mathfrak{q}$为$\mathfrak{g}\mathfrak{l}(V)$中$\mathfrak{n}$的归一化器。 E 上存在有限维向量空间 E、$\mathfrak{g}\mathfrak{l}(V)$ 的表示 $\rho$，E 上存在向量子空间 F，满足以下条件：

(i) V的位似的$\rho$下的像可对角化；

(ii) F 在 $\rho (\mathfrak{q})$ 下稳定；

(iii) $\mathfrak{n}$ 是$x\in \mathfrak{g}\mathfrak{l}(V)$ 的集合，使得$\rho (x)(F) = 0$。

让$n=$变暗V。根据恩格尔的定理，V可以与$k^n$等同，$\mathfrak{n}\subset \mathfrak{n}(n, k)$。令 P 为 $\mathfrak{g}\mathfrak{l}(n, k)$ 上多项式函数的代数。对于$i= 0,1, . .$.，令$P_i$为次数$i$的P齐次的元素集合。令N = exp $\mathfrak{n}$，即严格下三角群 T 的子群。令J 为P 的元素的集合，其在N 上为零；这是 P 中的理想。设 $N_J$ 为 $x\in \mathfrak{g}\mathfrak{l}(n, k)$ 的集合，这样对于所有 $p\in J$ 来说，$p(x) = 0$。然后$N\subset N_J$。相反，设$x\in N_J$。用 $p_{ij}$ 多项式函数表示，给出 $\mathfrak{g}\mathfrak{l}(n, k)$ 的元素条目。理想的 J 包含、$p_{ij}$（对于 $i < j$）和 $p_{ii}-1$；因此$x\in T$。另一方面，如果$u$在$\mathfrak{g}\mathfrak{l}(n, k)$上是线性形式，即$\mathfrak{n}$上的零，则存在$p_u\in P$，使得对于所有$z\in T ($§3, no. 1，$p_u(z) =u$(log $z$)， 引理 1 (i));我们有 $p_u\in J$，所以 $u$(log $x$) $= 0$。因此，将$x$属于记录到$\mathfrak{n}$，因此$x\in N$、证明即$N = N_J$。

对于所有$p\in P$和$g\in \mathbf{G}\mathbf{L}_n(k)$，令$\lambda (g)p$为$\mathfrak{g}\mathfrak{l}(n, k)$上的函数$x \rightarrow p(g^{-1}x)$；那么$\lambda (g)p\in P,\lambda (g)$是代数P的自同构，$\lambda$是P上$\mathbf{G}\mathbf{L}_n(k)$的表示，这使得每个$P_i$稳定。我们表明

$$
N =\{x\in \mathbf{G}\mathbf{L}_n(k)|\lambda (x)J = J\} \tag{1}
$$

如果$x\in N, p\in J, y\in N$，则从$x^{-1}y\in N$起$(\lambda (x)p)(y) =p(x^{-1}y) = 0$；因此$\lambda (x)p\in J$，所以$\lambda (x)J = J$。设$x\in \mathbf{G}\mathbf{L}_n(k)$使得$\lambda (x)J = J$；让 $p\in J$；然后$p(x^{-1}) = (\lambda (x)p)(e) = 0$，所以$x^{-1}\in N_J= N$和$x\in N$。这就证明了(i)。

理想的 J 是有限的型（交换代数，第 III, §2, no. 10 章，Th.2 的 Cor.2）。因此，存在整数 $q$，如果 $W = P_0+ P_1+\cdots + P_q$，则 $J\cap W$ 生成 J 作为理想。表示由$P_J$（分别由W）定义的$\lambda$的$\lambda_j$（分别$\lambda '$）子表示。由(1)，

$$
N =\{x\in \mathbf{G}\mathbf{L}_n(k)|\lambda '(x)(J\cap W) = J\cap W\} \tag{2}
$$

我们证明，对于所有$j$，$P_j$上存在李代数$\mathfrak{g}\mathfrak{l}(n, k)$的表示$\sigma_j$，使得：

$\sigma_j|\mathfrak{n}(n, k)$ 与 $\lambda_j|T$ 相容的（§$3$，无$.1$）。 (3)

对于所有 $x\in k.1_n, \sigma_j(x)$ 都是位似。 (4)

由于$\lambda_j$是$\lambda_1$的第$j$对称幂，因此足以证明$\sigma_1$、cf.引理1的存在性。现在$\lambda_1$是表示的同余表示 $\mathfrak{g}\mathfrak{l}(n, k)$ 上的 $\mathbf{G}\mathbf{L}_n(k)$ 的 $\gamma$ 给出

$$
\gamma (x)y=xy, x\in \mathbf{G}\mathbf{L}_n(k), y\in \mathfrak{g}\mathfrak{l}(n, k)
$$

设$c$为$\mathfrak{g}\mathfrak{l}(n, k)$上李代数$\mathfrak{g}\mathfrak{l}(n, k)$的表示，由下式给出

$$
c(x)y=xy, x, y\in \mathfrak{g}\mathfrak{l}(n, k)
$$

$c|\mathfrak{n}(n, k)$和$\gamma |T$兼容的是直接的，并且对于所有$x\in k.1_n$来说$c(x)$是位似。因此，只需将$c$的对偶表示视为$\sigma_1$即可（第I, §3, no. 3章）。

现在让 $\sigma '$ 为由 $\sigma_j, 0\leq j\leq q$ 的直和给出的 W 上 $\mathfrak{g}\mathfrak{l}(n, k)$ 的表示。鉴于 (2) 和关系

$\lambda '$(exp($x$)) $=$ exp($\sigma '(x)$) 和 $\sigma '$(log($y$)) $=$ log($\lambda '(y)$)$, x\in \mathfrak{n}(n, k), y\in T$,

我们有

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\sigma '(x)(J\cap W)\subset J\cap W\} \tag{5}
$$

让 $d=$ 变暗（J $\cap W$），并让 $\tau =\bigwedge^d\sigma '$。让$D =\bigwedge^d(J\cap W)$。由 (5) 和引理 2 (i)，

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\tau (x)(D)\subset D\} \tag{6}
$$

但$\tau (\mathfrak{n}(n, k))$由幂零自同态组成，所以(6)也可以写成

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\tau (x)(D) = 0\} \tag{7}
$$

现在让 $E =\bigwedge^dW\oplus \bigwedge^1V\oplus \bigwedge^2V\oplus  \cdots  \oplus \bigwedge^nV$；令$\rho$为$\tau$的直和，以及$\bigwedge^1V, . . . ,\bigwedge^nV$上$\mathfrak{g}\mathfrak{l}(n, k)$的规范表示。令$E_0\subset E$为$D =\bigwedge^d(J\cap W)$的和以及$e_{n-j+1}\wedge  \cdots  \wedge e_n$为$j= 1, . . . , n$生成的线。由(7)和引理2(ii)，

$$
\mathfrak{n}=\{x\in \mathfrak{g}\mathfrak{l}(V)|\rho (x)(E_0) = 0\} \tag{8}
$$

如果$x\in k.1_n,\rho (x)$可对角化的，则直接的。最后，如果 F 是被 $\rho (\mathfrak{n}), F$ 湮灭的 E 的元素的集合，则在 $\rho (\mathfrak{q})$ 下是稳定的（第 I, §3, no. 5 命题 5），并且通过 (8)，

$$
\mathfrak{n}=\{x\in \mathfrak{g}\mathfrak{l}(V)|\rho (x)(F) = 0\} \tag{9}
$$

### 5. 刻画可分解李代数

每个可分解李代数都由其元素的集合生成为向量空间（更不必说生成为李代数），元素要么是半单，要么是幂零的。反之：

#### 定理 1 {#lie-vii-s5-thm-1 .statement tag=00X1}

令$\mathfrak{g}$为$\mathfrak{g}\mathfrak{l}(V)$的谎言子代数，令X为$\mathfrak{g}$生成的$\mathfrak{g}$的子集，因为李代数超过$k$。如果X的每个元素都是半单或幂零，$\mathfrak{g}$是可分解的。

a$)\mathfrak{g}$ 是可交换的。

半单（或幂零）元素或 $\mathfrak{g}$ 形式向量子空间 $\mathfrak{g}_s$（或$\mathfrak{g}_n$）。 假设等价于$\mathfrak{g}=\mathfrak{g}_s\oplus \mathfrak{g}_n$，因此$\mathfrak{g}$ 是可分解的。

b$)\mathfrak{g}$ 是还原性的。

然后$\mathfrak{g}=\mathfrak{g}'\times \mathfrak{c}$与$\mathfrak{g}'$半单和$\mathfrak{c}$可交换。根据命题 $2,\mathfrak{g}'$ 是可分解的。让 $x=a+b\in \mathfrak{g}$ 与 $a\in \mathfrak{g}',b\in \mathfrak{c}$。令$a_s, a_n, b_s, b_n$为半单以及$a, b$的幂零分量。由于$a_s, a_n, b_s, b_n$相互可交换，半单和$x$的幂零分量为$a_s+b_s, a_n+b_n$。现在$a_s, a_n\in \mathfrak{g}'$。若$x$为半单，则$x=a_s+b_s$；从$a_s\in \mathfrak{g}'$开始，我们有$b_s\in \mathfrak{g}$，所以$b_s\in \mathfrak{c}$从$b_s$开始与$\mathfrak{g}$通勤；因而，$a=a_s$和$b=b_s$。类似地，如果 $x$ 幂零，则 $a=a_n$ 和 $b=b_n$。由此可见，X的元素的$\mathfrak{c}$上的投影要么是半单，要么是幂零的；由 a) 可知 $\mathfrak{c}$ 是可分解的。保留前面的记号，但在$x$上没有假设，我们现在有$b_s, b_n\in \mathfrak{c}$，所以$a_s+b_s, a_n+b_n\in \mathfrak{g}$，在这种情况下证明了定理。

c) 一般情况。

我们假设定理被证明为维数$<$暗淡$\mathfrak{g}$的李代数，并证明$\mathfrak{g}$。

设$\mathfrak{n}$为$\mathfrak{g}$恒等式表示的幂零理想最大的。如果 $\mathfrak{n}= 0,\mathfrak{g}$ 具有单射半单表示，则可还原。假设$\mathfrak{n}\not= 0$。令 $\mathfrak{p}$ 为 $\mathfrak{g}\mathfrak{l}(V)$ 中 $\mathfrak{n}$ 的归一化器。命题 8 存在$E, \rho ,F$ 满足条件。由于 $\mathfrak{g}\subset \mathfrak{p},\rho (\mathfrak{g})$ 使 F 保持稳定；令F上的$\rho_0$为$\mathfrak{g}$的表示$u \rightarrow \rho (u)|F$；我们有$\mathfrak{n}=$ Ker$\rho_0$。 $\mathfrak{g}\mathfrak{l}(V)$的每个半单（或幂零）元素在$\rho$下的像是半单（或幂幂）（命题2）。因而，代数$\rho_0(\mathfrak{g})$是由其半单元素及其幂零元生成的。到归纳假设时，$\rho_0(\mathfrak{g})$ 可分解。

设$x\in \mathfrak{g}$，并令$x_s, x_n$为其半单和幂零分量。根据命题 2，半单和 $\rho (x)$ 的幂零分量为 $\rho (x_s), \rho (x_n)$。由于 $\rho_0(\mathfrak{g})$ 可分解，因此存在 $y, z\in \mathfrak{g}$ 使得

$$
\rho_0(y) =\rho (x_s)|F, \rho_0(z) =\rho (x_n)|F
$$

然后$x_s\in y+\mathfrak{n}, x_n\in z+\mathfrak{n}$，所以$x_s, x_n\in \mathfrak{g}$。 Q.E.D.

#### 推论 1 {#lie-vii-s5-thm-1-cor-1 .statement tag=00X2}

由其可分解的子代数生成的$\mathfrak{g}\mathfrak{l}(V)$的每个子代数都是可分解的。

这很清楚。

#### 推论 2 {#lie-vii-s5-thm-1-cor-2 .statement tag=00X3}

设$\mathfrak{g}$是$\mathfrak{g}\mathfrak{l}(V)$的谎言子代数。那么$[\mathfrak{g},\mathfrak{g}]$是可分解的。

令$\mathfrak{r}$为$\mathfrak{g},\mathfrak{s}$的根式$\mathfrak{g}$的列维子代数（第I, §6, no. 8章）。然后

$$
[\mathfrak{g},\mathfrak{g}] = [\mathfrak{s},\mathfrak{s}] + [\mathfrak{s},\mathfrak{r}] + [\mathfrak{r},\mathfrak{r}] =\mathfrak{s}+ [\mathfrak{g},\mathfrak{r}]
$$

代数 $[\mathfrak{g},\mathfrak{r}]$ 是可分解的，因为它的所有元素都是幂零的（第 I, §5, no. 3 章）。另一方面，$\mathfrak{s}$是可分解的（命题2）。由此可见 $[\mathfrak{g},\mathfrak{g}]$ 是可分解的（Cor. 1）。

#### 推论 3 {#lie-vii-s5-thm-1-cor-3 .statement tag=00X4}

令$\mathfrak{g}$为$\mathfrak{g}\mathfrak{l}(V)$的谎言子代数，并令X为$\mathfrak{g}$生成的$\mathfrak{g}($作为李代数超过k)的子集。

(i) $\mathfrak{g}$的可分解包络$e(\mathfrak{g})$由半单和X的元素的幂零分量生成。

(ii) 如果$k'$是$k,e(\mathfrak{g}\otimes_kk') =e(\mathfrak{g})\otimes_kk'$中的扩张；并且$\mathfrak{g}$可分解当且仅当$\mathfrak{g}\otimes_kk'$可分解。

令$\widetilde{\mathfrak{g}}$为半单生成的$\mathfrak{g}\mathfrak{l}(V)$的子代数以及X的元素的幂零分量。然后$\mathfrak{g}\subset \widetilde{\mathfrak{g}}\subset e(\mathfrak{g})$；通过 Th。 $1, \widetilde{\mathfrak{g}}$ 可分解，所以$\widetilde{\mathfrak{g}}=e(\mathfrak{g})$，证明(i)。 断言 (ii) 如下，因为 X 生成 $k'$-代数 $\mathfrak{g}\otimes_kk'$。

#### 推论 4 {#lie-vii-s5-thm-1-cor-4 .statement tag=00X5}

令 $\mathfrak{g}$ 为 $\mathfrak{g}\mathfrak{l}(V)$ 的可分解谎言子代数。令$\mathscr{T}$为半单元素$\mathfrak{g}$由……组成交换子代数集合（cf.命题6）。 $\mathscr{T}$中的极大元素都有相同的维数。

设$k'$为$k$和$V'= V\otimes_kk',\mathfrak{g}'=$$\mathfrak{g}\otimes_kk'$的代数闭扩张。设$\mathfrak{t}_1,\mathfrak{t}_2$为$\mathscr{T},\mathfrak{t}'_i=\mathfrak{t}_i\otimes_kk',\mathfrak{h}_i$的极大元素，$\mathfrak{t}_i$在$\mathfrak{g},\mathfrak{h}'_i=\mathfrak{h}_i\otimes_kk'$的交换子。那么$\mathfrak{h}_i$是$\mathfrak{g}$的嘉当子代数（命题6），所以$\mathfrak{h}'_i$是$\mathfrak{g}'$的嘉当子代数。然后$\mathfrak{h}_i=\mathfrak{t}_i\times \mathfrak{n}_V(\mathfrak{h}_i)$，因此$\mathfrak{h}'_i=\mathfrak{t}'_i\times \mathfrak{n}_{V'}(\mathfrak{h}'_i)$，因此$\mathfrak{t}'_i$是半单元素$\mathfrak{h}'_i$的集合。由于$\mathfrak{g}'$是可分解的（Cor.$3$）$,\mathfrak{t}'_1$和$\mathfrak{t}'_2$在Aut$_e(\mathfrak{g}')$（第6条）下是共轭，所以dim$\mathfrak{t}_1=$dim$\mathfrak{t}_2$。

#### 定理 2 {#lie-vii-s5-thm-2 .statement tag=00X6}

设$\mathfrak{g}$是$\mathfrak{g}\mathfrak{l}(V)$的谎言子代数。以下条件是等效的：

(i) $\mathfrak{g}$ 可分解；

(ii) $\mathfrak{g}$中的每一个嘉当子代数都是可分解的；

(iii) $\mathfrak{g}$ 可分解嘉当子代数；

(iv) 部首$\mathfrak{g}$可分解。

(i) $=\Rightarrow$ (ii)：这源自 Cor.提案 3 中的第 2 条。

(ii) $=\Rightarrow$ (i)：这源自 Cor. 1 Th。 1，因为$\mathfrak{g}$是由它的嘉当子代数生成的（§2, no. 3，Th.1的Cor.3）。

(ii) $=\Rightarrow$ (iii)：这很清楚。

(iii) $=\Rightarrow$ (ii)：Cor. 3 Th。 1，我们可以假设$k$是代数封闭的。 $\mathfrak{g}$ 的嘉当子代数那么共轭在$\mathfrak{g}($§3, no. 2 的初等自同构下，Th。 1）；鉴于 §3, no. 1 的注 1，可以得出结论，如果其中之一是可分解的，那么它们都是可分解的。

(i) $=\Rightarrow$ (iv)：这源自 Cor.提案 4 中的第 2 条。

(iv) $=\Rightarrow$ (i)：假设$\mathfrak{g}$的部首$\mathfrak{r}$可分解。令$\mathfrak{s}$为$\mathfrak{g}$的列维子代数；它是可分解的（命题 2）。因此$\mathfrak{g}=\mathfrak{s}+\mathfrak{r}$是可分解的（Th.1的Cor.1）。

### 习题 {#lie-vii-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
