---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 13
section_title: p-radical extensions of height _ 1
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.98-A V.106, A V.170-A V.171
pdf_pages: 0212-0220, 0284-0285
extraction: ocr
subsections:
    - "no": 1
      title: $p$-free subsets and pbases
      page: 98
      pdf_page: 212
    - "no": 2
      title: Differentials and pbases
      page: 100
      pdf_page: 214
    - "no": 3
      title: The correspondence between subfields and Lie algebras of derivations
      page: 104
      pdf_page: 218
statements: 21
exercises: 6
content_sha256: a554c9dab93b0765125bb254db9e12cd67f1164d671299d3a2d3a6d06fc20c4f
translated_from: content/en/alg/V/13_s13_p_radical_extensions_of_height_1.md
translation_method: google
source_content_sha256: d7c5aa125c07daf15aa12374780d959bd9cb9aac8300a2a5e8c9396f60d1751b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 61127bd0d7a39452cec83fdee9d108f5d09c452d5812baef655edc8374e8b467
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 13。 $p$-高度延伸$\leq 1$

在本段中，$p$表示质数数。所有考虑的域都具有特征$p$。

### 1. $p$-无子集和 pbase

#### 定义 1 {#alg-v-s13-def-1 .statement tag=06QX}

设$K$为域，$L$为$K$高度$\leq 1$的$p$根式延伸。 $L$ 元素的家庭 $(x_i)_{i \in I}$ 据说在 $K$ 上没有 $p$（分别是 $L$ $K$ 的 $p$ 基础），如果 $x_i \notin K$ 对于所有 $i \in I$ 并且从典范嵌入 $u_i : K(x_i) \to L$ 导出的 $\bigotimes_{i \in I} K(x_i)$ 到 $L$ 的同态是单射（或双射）。

如果$a$是$L - K$的元素，则它是$p$高度为1的根式，因此它在$K$上的最小多项式是$X^p - a^p$（$V$，p. 24，命题1）；因此，$\{1, a, \ldots, a^{p-1}\}$ 是 $K(a)$ 中的基超过 $K$。令$(x_i)_{i \in I}$为$L - K$的元素和$\mathbf{N}^{(I)}$由……组成的$A$子集为有限支撑$a = (\alpha_i)_{i \in I}$的所有族，使得$\alpha_i < p$对于所有$i \in I$；命题 9（III、p. 471）表明，元素 $\bigotimes_{i \in I} x_i^{\alpha_i}$ 与 $a$ 相比，向量空间 $\bigotimes_{i \in I} K(x_i)$ 超过 $K$ 的$A$ 形式基。此外，$\bigotimes_{i \in I} K(x_i)$到$L$的典范同态有像$K(x_i)_{i \in I}$（$V$，p. 18，Cor.1），因此我们有以下命题：

#### 命题 1 {#alg-v-s13-prop-1 .statement tag=06QY}

令$K$为域，$L$为$K$和$x = (x_i)_{i \in I}$高度$\leq 1$的$p$激进延伸，$L$的元素族。然后$A$中的$a$通过乘积$x'' = \prod_{i \in I} x_i^{\alpha_i}$生成$K$上的向量空间$K(x_i)_{i \in I}$。为了使$(x_i)_{i \in I}$没有$p$（或以$p$为基础），家庭$(x^a)_{a \in A}$应该在$K$上自由（或$L$的基在$K$上）是必要且充分的。

#### 推论{#alg-v-s13-n1-cor-1 .statement tag=06QZ}

— 令 L' 为域 K 的扩张，由两个线性不相交的子扩展 K' 和 L 生成。假设L是K上高度为$\leq 1$的p根； *那么* L' 是 K' 上高度为 $\leq 1$ 的 p 根式。此外，对于L的元素族在K上无p（分别在K上有$L$的p基），它在K'上无p（分别在K'上有L'的p基）是必要且充分的。

我们有${L'}^p \subset K \subset K'$和$L' = K'(L)$，从而${L'}^p = {K'}^p({L'}^p) \subset K'$。在其他字中，L'是K'的高度$\leq 1$的p根延伸。推论的其他断言立即由命题 1 和V、p. 14、命题 5 得出。

#### 注 {#alg-v-s13-n1-rem-1 .statement tag=06R0}

设K为域，L是K的高度$\leq 1$的p根延伸，$(x_i)_i$是L的元素族。令 A 为多项式代数 $K[(X_i)_{i \in I}]$，a 由多项式 $X_i^p - x_i^p$ 和 $\varphi : A \to L$ K-代数同态生成的 A 的理想值，使得每个 $i \in I$ 都有 $\varphi(X_i) = x_i$。当且仅当$\varphi$的核等于a时，族$(x_i)_i$是无p的。对于 $K[(X_i)]/a$ 可以用代数 $\bigotimes_{i \in I} K[X_i]/(X_i^p - x_i^p)$ 来识别。

令 L 为域 K 的高度 $\leq 1$ 的 p 根延伸。如果由 S 的恒等映射定义的族本身是 p 无的（或 p 基），则 $L$ 的子集 S 被称为是 p 无的（或 p 基）。对于$(x_i)_i$，元素或$L$是无p的（分别是p基础），映射$i \mapsto x_i$应该是I的双射，在无p的子集（分别是p基础）上是必要且充分的L。根据命题 1，无 p 的集合中的每个子集都是无 p 的；相反，如果 S 是 L 中的子集，且所有有限子集都是 p-free，则 S 是 p-free。最后，K 上 L 的 p 基是无 p 子集 B，使得 $L = K(B)$。

#### 命题 2 {#alg-v-s13-prop-2 .statement tag=06R1}

— 令 K 为域，$L$ K 的高度 $\leq 1$ 和 S 子集 L 的 p 根延伸。为了使 S 是无 p 的，对于 S 的每个子集 $T \neq S$，$K(T) \neq K(S)$ 是必要且充分的。

首先假设 S 是无 p 的，并令 $T \neq S$ 为 S 的子集。用 A 集合表示整数的有限支撑 $a = (\alpha_s)_{s \in S}$ 在 0 和 $p-1$ 之间；令$A'$为$a = (\alpha_s)_{s \in S}$族的由……组成的子集，使得$a_s = 0$适用于$S - T$中的所有s。我们还将 $u_a = \prod_{s \in S} s^{\alpha_s}$ 替换为 $a \in A$。那么（V，p. 98，命题1）族$(u_a)_{a \in A'}$在K上是$K(S)$的基，亚族$(u_a)_{a \in A'}$在K上是$K(T)$的基。从$A' \neq A$开始，我们有$K(T) \neq K(S)$。

现在假设 S 不是无 p 的。那么 S 的元素 $x_1, ..., x_n$ 存在整数 $n \geq 1$ 和序列，使得 $(x_1, ..., x_{n-1})$ 是 p 自由的，但 $(x_1, ..., x_n)$ 不是。我们有$[K(x_1, ..., x_{n-1}):K] = p^{n-1}$和$[K(x_1, ..., x_n):K] < p^n$。由于$[K(x_1, ..., x_n):K]$是$[K(x_1, ..., x_{n-1}):K]$的倍数，因此我们有

$$
[K(x_1, ..., x_n):K] = [K(x_1, ..., x_{n-1}):K].
$$

从而$x_n \in K(x_1, ..., x_{n-1})$。这表明$K(S - \{x_n\}) = K(S)$。

#### 命题 3 {#alg-v-s13-prop-3 .statement tag=06R2}

— 令 K 为域，L K 和 S 的高度$\leq 1$ 的 p 根延伸，T 为 L 的两个子集。以下条件是等效的：
a) 子集 S 在 K 上无 p，T 在 K(S) 上无 p。
b) $S \cap T = \varnothing$ *并且* S U T 在 K 上是无 p 的。
如果 T 在 K(S) 上是无 p 的，则我们有 $T \cap K(S) = \varnothing$ 和更不必说 $S \cap T = \varnothing$。因此我们可以假设 S 和 T 不相交的。令A为所有$a = (a_x)_{x \in S \cup T}$家庭的$N^{(S \cup T)}$由……组成的子集，所有$x \in S \cup T$的$a_x < p$，以及$N^{(S)}$的定义子集$A'$和$A''$ $N^{(T)}$ 以类似的方式。我们可以很自然地将认同$N^{(S \cup T)}$与$N^{(S)} \times N^{(T)}$进行比较，然后将A与$A' \times A''$进行识别。对于$a \in A$，输入$u_a = \prod_{x \in S \cup T} x^{\alpha_x}$，类似地，对于$\beta \in A'$和$\gamma \in A''$，输入定义、$u'_\beta$和$u''_\gamma$。我们在 $A = A' \times A''$ 中有 $u_a = u'_\beta u''_\gamma$ 对应 $a = (\beta, \gamma)$。此外还有$(u'_\beta)_{\beta \in A'}$生成向量K空间K(S)（V，p. 94，命题1）。为了使 S U T 在 K 上无 p，族 $(u'_\beta u''_\gamma)_{\beta \in A', \gamma \in A''}$ 在 K 上无 p 是必要且充分的（V，p. 98，命题 1）；假设族 $(u'_\beta)_{\beta \in A'}$ 在 K 上是自由的，族 $(u''_\gamma)_{\gamma \in A''}$ 在 K(S) 上是自由的，则得到相同的 (II, p. 222)。现在，a) 和 b) 的等价由命题 1 得出（V，p. 98）。

#### 推论 {#alg-v-s13-n1-cor-2 .statement tag=06R3}

— 令 L 为 K 的高度 $\leq 1$ 的 p 根延伸，M 为 L 的子延伸。那么 L 是 M 上高度为 $\leq 1$ 的 p 基，M 是 K 上高度为 $\leq 1$ 的 p 基。此外，如果 B 是 M 在 K 上的 p 基，C 是 M 上L 的 p 基，则 $B \cap C = \varnothing$ 和 $B \cup C$ 是p-基础为 K 上的 L。

令 K 为域。 A family $(x_i)_{i \in I}$, is said to be a (absolute) p-basis of K if it is a p-basis of K over $K^p$. 对于每个整数$n \geq 1$，我们用所有$a = (\alpha_i)_{i \in I}$的$N^{(I)}$由……组成中的$\Lambda(n)$子集表示，这样$\alpha_i < p^n$代表所有$i \in I$。

#### 命题 4 {#alg-v-s13-prop-4 .statement tag=06R4}

— 令 $x = (x_i)_{i \in I}$ 为 K 的 p 基。对于每个整数 $n \geq 1$，族 $(x^u)_{u \in \Lambda(n)}$ 是 K 的基超过 $K^{p^n}$。

对于 $n = 1$ 断言约化到提案 1 (V、p. 98)。 集合$\Lambda(n)$由形式$a = \beta + p^{n-1}\gamma$$N^{(I)}$元素与$\beta \in \Lambda(n-1)$和$\gamma \in \Lambda(1)$组成。这样的分解是独一无二的，我们有$x^\alpha = x^\beta (x^\gamma)^{p^{n-1}}$。此外，族$(x_i^{p^{n-1}})_{i \in I}$显然是$K^{p^{n-1}}$超过$K^{p^n}$的p基，因此族$(x^\gamma)^{p^{n-1}}$是$K^{p^{n-1}}$的基超过$K^{p^n}$。因此，我们利用II、p. 222、命题25得出归纳的结论。

### 2. 差异和 pbase

令 K 为域（特征 p）且 V 向量空间超过 K。我们记得 (III, p. 552) K 到 V 的推导是 K 到 V 满足关系的映射 D
$$
\begin{align*}
D(x + y) &= D(x) + D(y) \\
D(xy) &= xD(y) + yD(x)
\end{align*}
$$

对于$x,\ y \in K$。由此可见，$D(1) = 0$和$D(x^n) = nx^{n-1}D(x)$适用于所有$x \neq 0$和所有$n \in \mathbf{Z}$（III、p. 557和558）。由于$K$具有特征$p$，因此我们对于所有$x \in K$

$$
D(x^p) = 0 .
$$

此外，对于 (III, p. 558)，我们有$x,\ y \in K,\ y \neq 0$，

$$
D(x/y) = (yD(x) - xD(y))/y^2
$$

由上式，$D$的公式核为$K$包含$K^p$的子域$E$。设$M$为$K$的子域；如果 $M$ 是线性的，我们就说 $D$ 是 $M$ 的导数；由(2)可知，假设$D$到$M$中的限制是零。

我们定义了（III，p. 570）$M$的模$\Omega_M(K)$-$K$的微分以及规范的$M$-从$K$到$\Omega_M(K)$的推导$d = d_{K/M}$。 $d_{K/M}$生成向量$K$-空间$\Omega_M(K)$的像。为了使$K$到$V$的映射$D$成为$M$导数，存在$K$线性映射$u : \Omega_M(K) \to V$使得$D = u \circ d_{K/M}$是必要且充分的；这个映射$u$是唯一确定的。

#### 命题 5 {#alg-v-s13-prop-5 .statement tag=06R5}

*令 $K$ 为域和由元素 $x$ 生成的 $K$ 的 $L$ 扩张，使得 $x \notin K,\ x^p \in K$。令$V$为向量空间除以$L$，并将$K$的$A$推导代入$V$，使得$\Delta(x^p) = 0$。那么存在一个唯一的推导$D$，将$L$延伸到$V$，延伸$A$，使得$D(x) = 0$。

根据$V$、p. 24、第 1 条，$\{1,\ x,\ \ldots,\ x^{p-1}\}$ 是 $L$ 中的基，超过$K$。对于$L$的每个元素$u = a_0 + a_1x + \ldots + a_{p-1}x^{p-1}$（$a_0,\ \ldots,\ a_{p-1}$在$K$中），我们放入$D(u) = A(a_0) + x\Delta(a_1) + \ldots + x^{p-1}\Delta(a_{p-1})$。显然$D$扩展$A$且满足(1)；所以建立关系就足够了

$$
D(uv) = u \cdot D(v) + v \cdot D(u)
$$

当$u$为形式$ax^i$且$v$为形式$bx^j$且$a,\ b$为$K,\ 0 \leq i < p$及$0 \leq j < p$时。

当$i + j < p$时，我们有$uv = x^{i+j}ab$，从而$D(uv) = x^{i+j}\Delta(ab)$。否则我们有$0 \leq i + j - p < p$，所以$uv = x^{i+j-p}(abx^p)$，还有$abx^p \in K$，但是从$A(x^p) = 0$开始，我们有$A(abx^p) = x^pA(ab)$，从而，还有$D(uv) = x^{i+j}\Delta(ab)$。所以我们在所有情况下都有

$$
\begin{align*}
D(uv) &= x^{i+j}\Delta(ab) = x^i x^j (a \cdot A(b) + b \cdot \Delta(a)) \\
&= (ax^i)x^j \cdot \Delta(b) + (bx^j)x^i \cdot \Delta(a) = u \cdot D(v) + v \cdot D(u) .
\end{align*}
$$

#### 推论 1 {#alg-v-s13-prop-5-cor-1 .statement tag=06R6}

*令$K$为域，$L$是$p$高度$\leq 1$对$K$和$V$向量空间在$L$上的径向延伸。每$K$的推导$A$进入$V$消失在$L^p$扩展到推导的$L$进入$V$。

根据 Zorn 的引理 (E, III, p. 20)，存在最大扩张为 $A$ 到推导 $D_0 : L_0 \to V$，其中 $L_0$ 为子域为 $L$ 包含 $K$。设 $x \in L$；我们有$x^p \in L_0$和$A(x^p) = 0$，从而$D_0(x^p) = 0$。根据提案 5，

D_0 扩展到推导定义在 L_0(x) 上；通过 D_0 的最大值特征标，我们有 L_0(x) = L，从而 x ∈ L_0。由于 x 是任意的，我们结论 L_0 = L。

#### 推论 2 {#alg-v-s13-prop-5-cor-2 .statement tag=06R7}

—令 L 为域 K 的高度 ≤ l 的 p 根延伸，并令 E 为 L 的子延伸。设 U 是由 E 的元素微分生成的 Ω_K(L) 的子空间。则 E 由 L 的元素组成，其与 U 的微分属于。特别是，对于所有 x ∈ L − K，我们有 d_{L/K}x ≠ 0。

令 x 为 L 的元素而不是属于到 E。则 {1, x, ..., x^{p^{l-1}}} 为 E(x) 在 E 上的基。令 A 为 E(x) 到 L 的 E 线性映射，使得 Δ(x^i) = ix'（0 ≤ i < p）。我们立即验证 A 是 E(x) 到 L 的 E 导数，特别是 K 导数。由科.从命题1到命题5，存在L到L延伸A的K-导数D。通过Ω_K(L)的泛性质，在向量L空间上存在线性形式u，使得D = u∘ d_{L/K}。我们有 D(x) = x 且 D|E = 0；因此，我们有 u(d_{L/K}x) ≠ 0 且 u|U = 0，从而 d_{L/K}x ∉ U。

最后一个断言是特殊情况 E = K；那么我们有 U = 0。

#### 定理 1 {#alg-v-s13-thm-1 .statement tag=06R8}

—令 L 为域 K 的高度 ≤ l 的 p 根扩展， (a_i)_{i ∈ I}，元素 L 的族。

a) 对于 (x_i)_{i ∈ I} 在 K 上是 p-free 的，族 (dx_i)_{i ∈ I} 在向量 L-空间 Ω_K(L) 中是自由的是必要且充分的。

b) 对于 K 上的 (x_i)_{i I} 到生成 L，族 (dx_i)_{i I} 应该生成向量 L-空间 Ω_K(L) 是充分必要的。

c) 为了使 (x_i)_{i I} 成为 K 上 L 的 p 基，族 (dx_i)_{i I} 应该是向量 L 空间 Ω_K(L) 的基是充分必要的。

首先让我们注，域 K((x_i)_{i ∈ I}) 的元素的微分dx为线性组合，系数在微分dx_i、i I的L中。对于族 (x_i)_{i ∈ I} 是 p-free 的，对于所有 i ∈ I，x_i ∉ K(x_j)_{j ∈ I - {i}} 是必要且充分的（V，p. 99，命题 2）。由科.根据 Prop. 5 的 2，这意味着 dx_i 不是 dx_j 的线性组合，因为 I 中 j ≠ i。 断言 a) 由此得出。现在 b) 立即从 Cor. 开始。提案 2 至提案 5 和 c) 由 a) 和 b) 得出。

以下推论使得 Cor.提案 5 中的第 1 条更具体：

#### 推论{#alg-v-s13-n2-cor-1 .statement tag=06R9}

—设 (x_i)_{i ∈ I} 为 L 在 K 上的 p 基。设 V 为 L 上的向量空间，K 的 A 推导进入 V，其在 L^p 和 (u_i)_{i ∈ 上消失I} V 元素的家庭。那么V中存在L的唯一推导D，其中扩展A和映射x_i到u_i，对于所有i∈I。

由科.根据命题 5 的 1，存在 L 的推导 D_0 延伸至 V 延伸 A。V 延伸 A 中的L 推导恰好是形式 D 的映射 = D_0 + u ∘ d_{L/K}其中 u 是 Ω_K(L) 到 V 的 L 线性映射。我们有 D(x_i) = u_i 当且仅当线性映射 u 满足条件 u(dx_i) = u_i − D_0(x_i)。由于族 dx_i 是 Ω_K(L) 的基，因此确定 u 是唯一的，推论如下。

设 L 为 K 的高度 $\leq 1$ 的 p 根延伸，$(x_i)_{i \in I}$ 为 L 在 K 上的 p 基。至 Th。 1 对于每个$i \in I$，存在L到L的K-导数$D_i$，其特征为$D_i(x_j) = \delta_{ij}$（克罗内克符号）； $D_i$ 是有时，称为*推导相对于*$x_i$的部分。当$I$是*有限*时，$(D_i)_{i \in I}$族是向量空间的基超过L由……组成的L到L的K-导数。

Th。 1 允许对 p 碱基的研究简化为对基或向量空间的研究。对于例，我们有以下结果：

#### 定理 2 {#alg-v-s13-thm-2 .statement tag=06RA}

— *令 L 为$\leq 1$ 域 K 的 p 根延伸。*
  *a)* *在 K 上存在 L 的 p 基。更准确地说，如果 S 是 K 上 L 的无 p 子集和 L 的 T 子集，使得 $S \subset T$ 和 $L = K(T)$，则在 K 上存在L 的 p 基 B，使得$S \subset B \subset T$.*
  *b)* *K 上 L 的两个 p 碱基具有相同的基数。*
  *c)* *要使$[L:K]$是有限的，向量空间$\Omega_K(L)$超过L应该是有限维超过L，然后我们有*

$$
[L : K] = p^{[\Omega_K(L) : L]}
$$

断言 *a)* 和 *b)* 为直接的 (II, p. 292)。 如果 $[L : K]$ 是有限的，则 *a)* 存在 $K$ 上 $L$ 的有限 p 基 $(x_1, ..., x_n)$；那么$L$的单项式$x_1^{\alpha_1} ... x_n^{\alpha_n}$和$0 \leq \alpha_i < p$超过$K$的$1 \leq i \leq n$形式基以及$\Omega_K(L)$的微分$dx_1, ..., dx_n$形式基超过$L$。 因此我们有$[L : K] = p^n$和$[\Omega_K(L) : L] = n$。 相反，如果 $\Omega_K(L)$ 是 $L$ 上的有限维，则存在 K 上 L 的有限 p 基（V、p. 102、Th.1），且 $[L : K]$ 是有限的。

#### 推出{#alg-v-s13-n2-cor-2 .statement tag=06RB}

— *对于每个 $x \in L - K$，存在 L 超过 K 包含 X 的 p 基。*

因为$\{x\}$是$L$超过$K$的无p子集，因此应用Th就足够了。 2、*a)*。

令 K 为 K 的域和 $L$ 扩张。如果 $D$ 是 L 的 K 导数，值在向量 L 空间中，那么对于所有 $x \in L$，我们有 $D(x^p) = 0$，依此类推$D$是$K(L^p)$的导数；由此可见$\Omega_K(L) = \Omega_{K(L^p)}(L)$。由于$L$是$\leq 1$高度$K(L^p)$的p根延伸，我们可以应用上面的结果。对于例，从 Th 开始。 1, *c)* 我们推论如下：设$(x_i)_{i \in I}$是$L$的元素的族；为了使$(dx_i)_{i \in I}$成为向量L-空间$\Omega_K(L)$的基，$(x_i)_{i \in I}$应该是L在$K(L^p)$上的p基是充分必要的。同样，科。提案 5 的第 2 条意味着：

#### 命题 6 {#alg-v-s13-prop-6 .statement tag=06RC}

— *令 K 为域（特征 p）和 K 的 L 扩张。*
  *a)* *令 $x \in L$;当且仅当 x 属于到 $K(L^p)$ 时，微分 $d_{L/K}x$ 消失。*
  *b)* $\Omega_K(L) = 0$当且仅当$L = K(L^p)$。*
  *c)* *假设L是K上有限高度的p根；那么 $\Omega_K(L) = 0$ 当且仅当 $L = K$.*

### 3. 推导的子域和李代数之间的对应

我们将 E 的所有推导表示为 E 域并用 g 集合表示为自身。我们记得 g 是 E 上的向量空间，其中运算定义为

$$(D + D')(x) = D(x) + D'(x), \quad (aD)(x) = a \cdot D(x)$$

对于$g$中的$D, D'$和$E$中的$a, x$。此外，如果$D$和$D'$是E入E的推导，$[D, D'] = DD' - D'D$（III，p. 554）也是如此。最后，莱布尼茨的公式 (III, p. 556) 给出

$$D^p(xy) = x \cdot D^p(y) + \sum_{j=1}^{p-1} \binom{p}{j} D^j(x) D^{p-j}(y) + D^p(x) \cdot y$$

（$E$中的$x, y$）；由于$1 \leq j \leq p-1$的二项式系数$\binom{p}{j}$可被$p$整除（$V$、p. 4、引理 1），我们看到$D^p$是E到E中的推导。我们立即找到关系（对于$a, a' \in E$）

$$[aD, a'D'] = aa' \cdot [D, D'] + (aD(a')) \cdot D' - (a'D'(a)) \cdot D.$$

特别是，$g \times g$到$g$的映射$(D, D') \mapsto [D, D']$是$E^p$线性的。

我们用子域$K$或$E$的$\mathscr{C}$集合表示，使得$E^p \subset K$和$[E : K]$是有限的；对于每个 $K \in \mathscr{C}$，我们用 E 的 K 导数的 $g(K)$ 集合表示。 Further, we denote by $\mathscr{L}$ the set of vector subspaces $l$ of $g$ of finite dimension over E and such that $[D, D'] \in h$ and $D^p \in h$ for any $D, D'$ in $h$; for each $h \in \mathscr{L}$ we denote by $I(h)$ the set of $x \in E$ such that $D(x) = 0$ for all $D \in h$.

#### 定理 3（雅各布森）{#alg-v-s13-thm-3 .statement tag=06RD}

— *映射$K \mapsto g(K)$和$l \mapsto I(h)$分别是$\mathscr{C}$到$\mathscr{L}$的双射和$\mathscr{L}$到$\mathscr{C}$的双射，它们是互逆的。如果 $K \in \mathscr{C}$ 和 $h \in \mathscr{L}$ 对应彼此成立，则 $[E : K] = p^{[h : E]}$*。

证明需要几个初步的引理。

#### 引理 1 {#alg-v-s13-lem-1 .statement tag=06RE}

— *令 L 为域，V 向量空间超过 L，且 u 自同态为 V，使得 $u^p = u$。对于每个$i \in \mathbf{F}_p$，令$V_i$为$u - i$的核。然后我们有*

$$\mathbf{V} = \bigoplus_{i \in \mathbf{F}_p} V_i.$$

对于每个$i \in \mathbf{F}_p$，用$P_i(X)$表示多项式$- \prod_{j \neq i} (X - j)$。我们有

$$(X - i) P_i(X) = X - X^p$$

由公式 (2) ($V$, p. 94)。在推导引用的公式 (2) 时，我们发现

$$\sum_{i \in \mathbf{F}_p} P_i(X) = 1$$

公式 (8) 和 (9) 表明$V$ 映射 $V$ 的自同态 $P_i(u)$ 进入$V_i$ 以及$\sum_{i \in \mathbf{F}_p} P_i(u) = 1$、从而 $V = \sum_{i \in \mathbf{F}_p} V_i$。 仍有待证明和是直接的。 对于每个 $i \in \mathbf{F}_p$ 让 $v_i \in V_i$；很明显，对于所有 $j \neq i$，$P_i(u)$ 会消灭 $v_j$，并且我们有 $P(u)v_i = av_i$ 和 $a = -\prod_{n \in \mathbf{F}_p^*} n \neq 0$。 因此，关系$\sum_{i \in \mathbf{F}_p} v_i = 0$意味着$v_i = 0$对于所有$i \in \mathbf{F}_p$，因此和是直接的。

#### 引理 2 {#alg-v-s13-lem-2 .statement tag=06RF}

*设 D 为 E 的推导，使得 $D^p = D$，并令 K 为 D 的核。假设 E 中存在一个非零 x，使得 $D(x) = x$。那么 K 是 E 包含 $E^p$ 的子域，我们有 $[E : K] = p$。*

显然，K 是 E 包含 $E^p$ 的子域。用$D - i$的$K_i$核表示$i \in \mathbf{F}_p$。我们有 $K_0 = K$ 和引理 1 表明$E = \bigoplus_{i \in \mathbf{F}_p} K_i$。令$i \in \mathbf{F}_p$且$u$在$K_i$中；我们有
$$
D(xu) = D(x) \cdot u + x \cdot D(u) = xu + x(iu) = (i + 1)xu
$$
从而$xu \in K_{i+1}$。由于x非零，所以x的乘法是向量K空间E的自同构，其中对于所有$i \in \mathbf{F}_p$，映射$K_i$到$K_{i+1}$。从 $[K_0 : K] = 1$ 开始，我们为所有 $i \in \mathbf{F}_p$ 从而 $[E : K] = p$ 提供了 $[K_i : K] = 1$。

#### 引理 3 {#alg-v-s13-lem-3 .statement tag=06RG}

*设 $\mathfrak{h} \in \mathscr{L}$ 是 E 上的维数 s。然后 $I(\mathfrak{h})$ 属于到 $\mathscr{C}$，我们有 $[E : I(\mathfrak{h})] = p^s$。*

显然，$I(\mathfrak{h})$是$E$包含$E^p$中的子域。对于每个$x \in E$，令$f_x$为I上的E线性形式$D \mapsto D(x)$）。由于这些线性形式的 kcrncl 的交等于 0，因此它们生成向量空间对偶于 $\mathfrak{h}$ (II, p. 301, Th. 7)；因此，$E$中存在$x_1, \ldots, x_s$，使得这个对偶的线性形式$f_{x_1}, \ldots, f_{x_s}$形式基。令 $(\Delta_1, \ldots, \Delta_s)$ 为由 $\Delta_i(x_j) = f_{x_j}(\Delta_i) = \delta_{ij}$ 表征的 $\mathfrak{h}$ 的基。把$D_i = x_i \Delta_i$，然后$(D_1, \ldots, D_s)$是基/I)在E上，我们有$D_i(x_j) = x_i \delta_{ij}$。 推导$D_i^p - D_i$和$[D_i, D_j]$（$i, j = 1, \ldots, s$属于至I）并消灭$x_1, \ldots, x_s$；因此我们有
$$
D_i^p = D_i , \quad [D_i, D_j] = 0
$$
对于 0 到 s 范围内的 i，我们用 $K_i$ 交或核或推导 $D_j$ 来表示 $1 \leq j \leq i$。那么$K_i$是E的子域，我们有
$$
E = K_0 \supset K_1 \supset \ldots \supset K_{s-1} \supset K_s = I(\mathfrak{h}) .
$$
令i在0和$s-1$之间；那么$K_i$在$D_{i+1}$下是稳定的，因为$D_{i+1}$与$D_1, \ldots, D_i$通勤。此外，我们还有$D_{i+1}^p = D_{i+1}$、$D_{i+1}(x_{i+1}) = x_{i+1} \neq 0$和$x_{i+1} \in K_i$。因此引理 1 意味着$[K_i : K_{i+1}] = p$，从而最后$[E : K] = [K_0 : K_s] = p^s$。

现在我们来到证明/定理。设 I) $\in \mathscr{L}$ 为 E 上的维数 s，并放入 $K = I(\mathfrak{h})$；然后$[E : K] = p^s$乘引理3，从而$[\Omega_K(E) : E] = s$乘

Th。 2、c) (V、p. 103)。通过微分映射$u \mapsto u \circ d_{E/K}$的模的泛性质是$\Omega_K(E)$对偶$g(K)$的同构，因此$[g(K):E] = s$。现在我们有$[\mathfrak{h}:E] = s$和$\mathfrak{h} \subset g(K)$，从而$\mathfrak{h} = g(K)$，即$\mathfrak{h} = g(I(\mathfrak{h}))$。

相反，对于每个域$K \in \mathscr{C}$，很明显$g(K)$属于到$\mathscr{L}$（V，p. 103，Th.2，c））。 *如果*$x$属于到$I(g(K))$，我们在$\Omega_K(E)$、从而$d_{E/K}x = 0$上为每个线性形式$u$有$u(d_{E/K}x) = 0$，所以最后$x \in K$由Cor.提案 5 中的第 2 条（V、p. 102）。因此我们有$K = I(g(K))$。

#### 注 {#alg-v-s13-n3-rem-1 .statement tag=06RH}

— 1) 逆双射 $K \mapsto g(K)$ 和 $\mathfrak{h} \mapsto I(\mathfrak{h})$ 互为包含反转；因此，$\mathfrak{h} \mapsto I(\mathfrak{h})$是有序集合$\mathscr{L}$的同构到与$\mathscr{C}$相反的有序集合上。因此，我们在$\mathscr{L}$中得到$\mathfrak{h}, \mathfrak{h}'$的关系$I(\mathfrak{h} \cap \mathfrak{h}') = E^p(I(\mathfrak{h}), I(\mathfrak{h}'))$，因为$\mathfrak{h} \cap \mathfrak{h}'$是$\mathfrak{h}$和$\mathfrak{h}'$中包含的$\mathscr{L}$的最大的元素。

2) 可以证明，$g$的有限维、子空间在映射$D \mapsto D^p$下稳定，在运算下也稳定。

### 习题 {#alg-v-s13-exercises}

§ 13](exercises/s13/)参见[习题。
