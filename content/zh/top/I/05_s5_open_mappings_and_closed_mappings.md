---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 5
section_title: Open mappings and closed mappings
lang: zh
source: top-i-iv
book_pages: 50-57, 127-128
pdf_pages: 0056-0063, 0133-0134
extraction: ocr
subsections:
    - "no": 1
      title: OPEN MAPPINGS AND CLOSED MAPPINGS
      page: 50
      pdf_page: 56
    - "no": 2
      title: OPEN EQUIVALENCE RELATIONS AND CLOSED EQUIVALENCE RELATIONS
      page: 52
      pdf_page: 58
    - "no": 3
      title: PROPERTIES PECULIAR TO OPEN MAPPINGS
      page: 54
      pdf_page: 60
    - "no": 4
      title: PROPERTIES PECULIAR TO CLOSED MAPPINGS
      page: 56
      pdf_page: 62
statements: 24
exercises: 7
content_sha256: bfdd0a04594ebd93604b0e426f48922ac8ce08a8a46eb72aea6735560c39eede
translated_from: content/en/top/I/05_s5_open_mappings_and_closed_mappings.md
translation_method: google
source_content_sha256: 30449acefded09c82f02573834e6808d312199d63f6f407bfcd7aac989b3a9ff
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 2017c15895c40f943a27921a43739b6d71ddff7e78b9689c78e630724897defe
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 5. 开放映射闭馆映射

### 1. 开放映射闭馆映射

#### 定义 1 {#top-i-s5-def-1 .statement tag=0B32}

*令$X, X'$为两个拓扑空间。如果每个打开（或关闭）的$f$下的像打开（或关闭）映射$f : X \to X'$打开（或关闭）$X$的集合在$X'$打开（或关闭）。*

特别地，$f(X)$ 是$X'$ 的开（或闭）子集。

#### 例 1 {#top-i-s5-n1-exa-1 .statement tag=0B33}

设$A$为拓扑空间$X$的子空间。那么典范嵌入 $j : A \to X$ 是开（或闭）的，当且仅当 $A$ 在 $X$ (§ 3, no. 1) 中是开（或闭）的。

#### 例 2 {#top-i-s5-n1-exa-2 .statement tag=0B34}

对于拓扑空间$X$到拓扑空间$X'$的双射$f$成为*同胚*，$f$是*连续且开*，或*连续且闭*是必要且充分的。

#### 例 3 {#top-i-s5-n1-exa-3 .statement tag=0B35}

令$f$为集合$X$到拓扑空间$X'$的满射；如果我们给出$X$拓扑，即$X'$的拓扑的$f$下的逆像（§ 2, no. 3，例1），那么$f$是连续的、开闭的。

#### 例 4 {#top-i-s5-n1-exa-4 .statement tag=0B36}

在乘积空间
$$
X = \prod_{i \in I} X_i,
$$
每个投影$\mathrm{pr}_i : X \to X_i$都是一个连续的开映射，但不一定是闭的（§ 4, no. 2，命题5）。

#### 例 5 {#top-i-s5-n1-exa-5 .statement tag=0B37}

\* $C$ 的开子集 $A$ 上的全纯函数是$A$ 的开映射到$C$。 \*

#### 例 6 {#top-i-s5-n1-exa-6 .statement tag=0B38}

设$X, X'$是两个拓扑空间和$f$，$X$的连续但不是双连续的双射到$X'$。那么逆双射$g : X' \to X$是$X'$到$X$的开闭映射，但不连续。

#### 命题 1 {#top-i-s5-prop-1 .statement tag=0B39}

*令$X, X', X''$为三个拓扑空间，令$f : X \to X', \ g : X' \to X''$为两个映射。然后：*

a) *如果 $f$ 和 $g$ 打开（或关闭），则 $g \circ f$ 也打开。*

b) *如果 $g \circ f$ 开（或闭）并且 $f$ 是连续且满射的，则 $g$ 是开（或闭）。*

c) *如果 $g \circ f$ 开（或闭）并且 $g$ 是连续且单射的，则 $f$ 是开（或闭）。*

从定义 1.a) 开始，紧随其后。为了证明b)，只要注意到$X'$的每个开（或闭）子集$A'$都可以写成$f(A)$，其中$A = f^{-1}(A')$在$X$（§ 2, no. 1，定理1）中开（或闭）；因此$g(A') = g(f(A))$在$X''$中打开（或关闭）。最后，为了证明c)，我们注意到对于$X$的每一个子集$A$都有$f(A) = g^{-1}(g(f(A)))$；到假设，如果$A$在$X$打开（或关闭），则$g(f(A))$在$X''$打开（或关闭），因此$f(A)$在$X'$通过§ 2, no. 1，定理打开（或关闭） 1.

#### 命题 2 {#top-i-s5-prop-2 .statement tag=0B3A}

*设$X, Y$为$X$到$Y$的两个拓扑空间、$f$映射。对于$Y$的每个子集$T$，让$f_T$表示$f^{-1}(T)$的映射进入$T$，这与$f^{-1}(T)$上的$f$一致。*

a) *如果 $f$ 打开（或关闭），则 $f_T$ 打开（或关闭）。*

b) *设$(T(i))_{i \in I}$是$Y$的子集族，其内部覆盖$Y$，或者是$Y$的局部有限封闭覆盖；如果所有 $f_{T(i)}$ 都打开（或关闭），则 $f$ 也打开（或关闭）。*

a) 如果 $A$ 是 $f^{-1}(T)$ 的开（或闭）子集，则存在 $X$ 的开（或闭）子集 $B$，使得 $A = B \cap f^{-1}(T)$，因此 f_T(A) = f(B) \cap T； 假设时，$f(B)$ 打开（或关闭），因此 $f_T(A)$ 在 $T$ 打开（或关闭）。

b) 令$B$为$X$的开（或闭）子集，并令$B_i$表示$B \cap f^{-1}(T(i))$；然后$f(B) \cap T(i) = f_{T(i)}(B_i)$。由于 $f_{T(i)}(B_i)$ 在 $T(i)$ 到假设处开（或闭），因此，$f(B)$ 在 $Y$ 处，到 § 3, no. 1 的命题 3 处开（或闭）。

#### 推论 {#top-i-s5-n1-cor-1 .statement tag=0B3B}

*设$(T(i))_{i \in I}$是$Y$的子集族，其内部覆盖$Y$，或者是$Y$的局部有限封闭覆盖。如果$f : X \to Y$是连续的，并且每个$f_{T(i)}$是$f^{-1}(T(i))$到$T(i)$的同态，那么$f$是$X$到$Y$的同态。*

因为 $f$ 显然是双射的，并且凭借命题 2 是开集。

### 2. 打开等价关系关闭等价关系

#### 定义 2 {#top-i-s5-def-2 .statement tag=0B3C}

*如果 $X$ 到 $X/R$ 上的典范映射是开路（或闭路），则等价关系 $R$ 在拓扑空间 $X$ 上被称为开路（或闭路）。*

说$X$相对于$R$的每个开（或闭）子集的“饱和度”在$X$（§ 3, no. 4）中开（或闭），这也是同样的道理。

#### 例 1 {#top-i-s5-n2-exa-1 .statement tag=0B3D}

令 $X$ 为拓扑空间，$\Gamma$ $X$ 的同胚 *群到自身，并令 $R$ 为等价关系

“存在$\sigma \in \Gamma$使得$y = \sigma(x)$”

在$x$和$y$之间（因此$R$是等价关系，其中类是$X$中$\Gamma$的*轨道*。关系$R$是*开*，对于子集的饱和$X$ 的 $A$ 相对于 $R$ 是开放的，因此每个 $\sigma(A)$ 也是开放的，因此它们的并也是开放的。

\* 在实直线 $\mathbf{R}$ 等价关系 $x \equiv y \pmod{1}$ 上是开放的，因为它是从群的翻译中导出的

$$
x \to x + n \qquad (n \in \mathbf{Z})
$$

（参见章III, § 2, no. 4）。 \*

#### 例 2 {#top-i-s5-n2-exa-2 .statement tag=0B3E}

令$X$为$X$子空间族$(X_i)$之和，令$X/R$为通过双射$h_{ix}$ (§ 2, no. 5)沿着*开放*子集$A_{ix}$*粘贴*$X_i$获得的空间；并假设对于每对索引 $(i, x)$，$h_{ix}$ 是 $A_{ix}$ 到 $A_{x'}$ 的*同胚*。

那么关系 R 开。因为如果U在X开路，则U的饱和度是$h_{x!}(U \cap A_{ix})$的并；由于$U \cap A_{ix}$在$A_{ix}$中开放，$h_{x!}(U \cap A_{ix})$在$A_{ix}$中开放，因此在X中开放。

#### 例 3 {#top-i-s5-n2-exa-3 .statement tag=0B3F}

当记号为例 2 时，现在假设 $A_{ix}$ 是闭集且 $h_{x!}$ 是同胚；进一步假设对于每个指标 i，只有指标 x 的有限数，使得$A_{ix} \neq \varnothing$（即每个$X_i$“卡”到仅$X_x$的有限数）。则关系 R 闭合。因为如果F是X的任意闭子集，则F的饱和度是集合$h_{x!}(F \cap A_{ix}) \subset A_{ix}$的并； 假设意味着这个族是局部有限的，$h_{x!}(F \cap A_{ix})$在$A_{ix}$中是封闭的，因此在X中是封闭的。因此，结果来自命题 4 of § 1, no. 5。

#### 命题 3 {#top-i-s5-prop-3 .statement tag=0B3G}

令X，Y为两个拓扑空间，令$f : X \to Y$为连续映射，令R为X上的等价关系$f(x) = f(y)$，令$X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y$为f的规范分解。那么下面三个叙述是等价的：

a) f 是一个开映射。

b) 三个映射 p、h、i 开。

c) 等价关系 R 是开集，h 是同胚，$f(X)$ 是 Y 的开子集。

此外，如果“开放”始终被“封闭”替换，则前面的命题仍然为真。

由于单射 i 是连续的，因此从 no. 1 的命题 1 c) 可以得出，如果 f 是开路的，那么 $h \circ p$ 也是开路；由于 p 是满射且连续的，命题 1 b) 表明 h 是开集； h 在任何情况下都是连续的双射；因此 h 是同胚，因此，从 no. 1 的命题 1 a) 出发，$p = \overline{h}^{-1} \circ (h \circ p)$ 是开映射。另外 [no. 1, 命题 1 b)] $i \circ h$ 已打开；因此 [no. 1, 命题 1 a)] $i = (i \circ h) \circ \overline{h}^{-1}$ 也是如此。这证明a)蕴涵b)。相反，no. 1的命题 1 a)表明b)蕴涵a)。最后，b)和c)的等价紧随定义而来。

证明在闭合的情况下映射是类似的，加以必要的修改。

#### 命题 4 {#top-i-s5-prop-4 .statement tag=0B3H}

令 R 为拓扑空间 X 上的开（或闭）等价关系，且 f 典范映射 $X \to X/R$。令A为X的子集，并假设满足以下两个条件之一：

a) A 在 X 处开（或闭）。

b) A 相对于 R 是饱和的。

那么在 A 上诱导的关系 $R_A$ 是开（或闭）的，并且 $A/R_A$ 到 $f(A)$ 的典范映射是同胚。

考虑 § 3, no. 6 的交换律图表 (i)，它给出了 $f \circ j$ 的规范分解。在条件 a) 下，$j$ 开（或闭），$f$ 乘假设也是如此；因此 $f \circ j$ 开（或闭）[no. 1, 命题 1 a)]，结果由命题 3 得出。在条件 b) 下，我们有
$$
A = \overline{f}^{-1}(f(A)),
$$
$h \circ \varphi$是$A$到$f(A)$的映射，与$A$上的$f$一致；由于no. 1的命题 2 a)，$h \circ \varphi$打开（或关闭），并且结果再次从命题 3得出，应用于$h \circ \varphi$。

### 3. 打开特有的属性映射

#### 命题 5 {#top-i-s5-prop-5 .statement tag=0B3I}

*设$X, Y$为$X$拓扑$Y, \mathfrak{B}$基为空间、$X$$f$映射。那么下面的叙述是等价的*：

a) *$f$是一个开放的映射*。

b) *对于每个$U \in \mathfrak{B}$，$f(U)$在$Y$开放*。

c) *对于$X$中$x$的每个$x \in X$和邻域$V$，$f(V)$是$Y$中$f(x)$的邻域*。

a) 和 b) 的等价紧接在定义和$(O_1)$之后； a)和c)的等价是§ 1, no. 2的命题1中的推论。

#### 命题 6 {#top-i-s5-prop-6 .statement tag=0B3J}

*在拓扑空间$X$上设$R$为等价关系；那么以下三个条件是等价的*：

a) *关系 $R$ 已开放*。

b) *相对于$R$饱和的每个子集的内部相对于$R$也饱和*。

c) *每个相对于$R$饱和的子集的闭包相对于$R$也是饱和的*。

通过补集 ($§ 1$, no. 6, 公式 (2))，我们看到 b) 和 c) 是等价的。让我们证明 b) 蕴含 a)：假设条件 b) 满足，并令 $U$ 为 $X$ 的开子集，$V$ 相对于 $R$ 饱和；然后$\dot{V} \supset U$，并且由于到假设$\dot{V}$饱和，因此$\dot{V} = V$，因此$U$的饱和是开放的。反之，假设满足条件a)，则令$A$为饱和的集合；如果$B$是$\dot{A}$的饱和度，则$\dot{A} \subset B \subset A$，并且由于$B$由假设打开，因此$B = \dot{A}$。

#### 命题 7 {#top-i-s5-prop-7 .statement tag=0B3K}

令$R$为拓扑空间$X$上的开等价关系，并令$\varphi : X \to X/R$为典范映射。如果$A$是$X$的任何子集，并且相对于$R$饱和，则$X/R$中$\varphi(A)$的闭合（分别是内部）是$\varphi(\overline{A})$（分别是$\varphi(\overset{\circ}{A})$）。

命题的两个断言中的每一个都可以通过求补并使用 § 1, no. 6 的公式 (2) 以及如果 $B$ 是 $X$ 的饱和子集那么 $\varphi(\complement B) = \complement_{\varphi}(B)$ 的事实来推导出来。由于命题6，$\overline{A}$饱和；因此$\varphi(\overline{A})$在$X/R$关闭，并且从$A \subset \overline{A}$开始我们有$\varphi(A) \subset \varphi(\overline{A})$，所以$\varphi(A) \subset \varphi(\overline{A})$。但由于 $\varphi$ 是连续的，$\varphi(\overline{A}) \subset \varphi(A)$ (§ 2, no. 1, 定理 1)，结果如下。

#### 命题 8 {#top-i-s5-prop-8 .statement tag=0B3L}

令$(X_i)_{i \in I}, (Y_i)_{i \in I}$是拓扑空间的两个族，由相同的集合$I$索引。 对于每个$i \in I$，令$f_i$是$X_i$到$Y_i$的开放映射，并假设$f_i$对于除了有限数量的索引之外的所有索引都是满射的。 那么$\prod_{i \in I} X_i$到$\prod_{i \in I} Y_i$的乘积映射$f : (x_i) \to (f_i(x_i))$是开放的。

凭借命题 5，我们只需证明$\prod_{i \in I} X_i$中任意初等集合$\prod_{i \in I} A_i$在$f$下的像在$\prod_{i \in I} Y_i$中都是开的。 但是这个像是$\prod_{i \in I} f_i(A_i)$，并且假设意味着对于每个$i \in I$，$f_i(A_i)$在$Y_i$中是开放的，并且对于除了指标的有限数之外的所有$f_i(A_i) = Y_i$； 从而结果。

#### 推论 {#top-i-s5-n3-cor-1 .statement tag=0B3M}

令$(X_i)_{i \in I}$为拓扑空间族，对于每个$i \in I$，令$R_i$为$X_i$上的等价关系，并令$f_i$为典范映射$X_i \to X_i/R_i$。设$X = \prod_{i \in I} X_i$中的$R$为等价关系

“对于每个$i \in I$，$\operatorname{pr}_i(x) = \operatorname{pr}_i(y)$（模$R_i$）”

$x$和$y$之间，并令$f$为$X$的乘积映射$(x_i) \to (f_i(x_i))$到$\prod_{i \in I} (X_i/R_i)$。如果关系 $R_i$ 中的每一个都是开路，则关系 $R$ 都是开路，并且与$f$相关的双射是$X/R$到$\prod_{i \in I} (X_i/R_i)$的同胚。

$R$ 是关系 $f(x) = f(y)$。由于$f$是连续的，并且通过上面的命题 8和§ 4, no. 1、推论 1 of 命题 1开，所以结果来自于no. 2的命题 3。

特别是，如果 $R$（或 $S$）是拓扑空间 $X$（或 $Y$）上的开等价关系，则规范的双射

$$
(X \times Y)/(R \times S) \quad \text{onto} \quad (X/R) \times (Y/S)
$$

是同胚。如果R和S不假设为开集，则这个双射是连续的，但不一定是同胚，即使关系R，S之一是等式（习题6）的关系。

### 4. 闭映射特有的性质

#### 命题 9 {#top-i-s5-prop-9 .statement tag=0B3N}

设X、X'为两个拓扑空间。对于映射 f : X → X' 连续且封闭的充分必要条件是，对于 X 的每个子集 A，f(Ā) = f(A)。

条件是充分的，因为它显然意味着 f 是闭集的，并且还意味着 f 由于§ 2, no. 1、定理 1 是连续的。相反，如果 f 是连续且闭集的，则通过 § 2, no. 1、定理 1 有 f(A) ⊂ f(Ā) ⊂ f(A)； f(Ā) 也在 X' 中被假设封闭；因此 f(Ā) = f(A)。

#### 命题 10 {#top-i-s5-prop-10 .statement tag=0B3O}

令 R 为拓扑空间 X 上的等价关系。那么 R 是闭合的，当且仅当每个等价类 M mod R 拥有邻域的基系统，并且相对于 R 是饱和的。

假设R是闭集，设U是M的任意开邻域；由于 F = ĈU 在 X 中闭合，因此 F 相对于 R 的饱和度 S 在 X 中闭合。由于 M 相对于 R 是饱和的，所以我们有 M ∩ S = ∅，因此 V = ĈS 是 M 的开邻域，相对于 R 是饱和的并包含在 U 中。

为了证明逆命题，令 F 为 X 的任意闭子集。令T为F相对于R的饱和度，令x为ĈT的点，并令M为x的等价类；则 M ∩ T = ∅ 且更不必说 M ∩ F = ∅，因此 U = ĈF 是 M 的邻域。因此，M 存在邻域 V ⊂ U，使得 V 相对于 R 饱和； V 不满足 F，因此不满足 T，因此 ĈT 是 M 的邻域，因此也是 x 的邻域。这表明 ĈT 是开集 (§ 1, no. 2, 命题 1)，即 T 是闭集。

#### 注 {#top-i-s5-n4-rem-1 .statement tag=0B3P}

命题 10 意味着以下内容：如果 R 是闭集，且 φ 表示典范映射 X → X/R，则对于X 中 x 的每个 x ∈ X 以及等价类的每个邻域 U，φ(U) 为X/R 中 φ(x) 的邻域。需要注意的是，这个叙述绝不意味着对于x的每一个邻域V，φ(V)就是φ(x)的邻域；在其他字 (no. 3, 命题 5) 中，封闭的等价关系不一定是开放的 (习题 2)。相反，开的等价关系不一定是闭的（no. 1，例4）；

因为如果等价类$M$的$X$中$U$是邻域，那么对于$x$的每个$x \in M$和邻域$V \subset U$，$V$的饱和度肯定是邻域 $M$在$X$中，但是这个邻域*不一定包含在*$U$中。

最后，除了等式之外，还有既开又闭的等价关系（习题3）和既不开又不闭的等价关系（$§ 8$，习题10）。

### 习题{#top-i-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
