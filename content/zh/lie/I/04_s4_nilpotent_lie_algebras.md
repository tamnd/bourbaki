---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 4
section_title: Nilpotent Lie algebras
lang: zh
source: lie-i-iii
book_pages: 38-42, 91-98
pdf_pages: 0056-0060, 0109-0116
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF NILPOTENT LIE ALGEBRAS
      page: 38
      pdf_page: 56
    - "no": 2
      title: ENGEL'S THEOREM
      page: 39
      pdf_page: 57
    - "no": 3
      title: THE LARGEST NILPOTENCY IDEAL OF A REPRESENTATION
      page: 40
      pdf_page: 58
    - "no": 4
      title: THE LARGEST NILPOTENT IDEAL OF A LIE ALGEBRA
      page: 42
      pdf_page: 60
    - "no": 5
      title: EXTENSION OF THE BASE FIELD
      page: 42
      pdf_page: 60
statements: 18
exercises: 27
content_sha256: c48912521aae0ad25b9e91d9ca07eb72055f1dbbe5fae599c5ffddd3b6e6122d
translated_from: content/en/lie/I/04_s4_nilpotent_lie_algebras.md
translation_method: google
source_content_sha256: 9f6dbd6648d7739560a7db8789c8dcacb1593afb46758c4bce763121741c6605
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: fd7282d2d4cace59fe23cd650a0680f0bbe8857b6f5bbb53040efd806e28a8d4
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 幂零李代数

*回想一下，从此以后 $K$ 表示交换域。其余的章李代数被假定为 $K$ 上的有限维。*

### 1.定义幂零李代数

#### 定义 1 {#lie-i-s4-def-1 .statement tag=09WS}

*如果存在 $g$ 与 $g_0 = g, g_p = \{0\}$ 的理想 $(g_i)_{1 \leq i \leq p}$ 递减有限序列，李代数 $g$ 称为幂零，使得* $[g, g_i] \subset g_{i+1}$ *对于* $0 \leq i < p$。

交换律李代数是幂零的。

#### 命题 1 {#lie-i-s4-prop-1 .statement tag=09WT}

*令$g$为李代数。以下条件是等效的：*
(a) $g$ *幂幂；*
(b) $\mathscr{C}^k g = \{0\}$ *对于足够大* $k$；
(c) $\mathscr{C}_k g = g$ *对于足够大* $k$；
(d) *存在整数* $k$ *使得* $\operatorname{ad} x_1 \circ \operatorname{ad} x_2 \circ \cdots \circ \operatorname{ad} x_k = 0$ *对于所有元素* $x_1, x_2, \ldots, x_k$ *在* $g$；
(e) *存在递减序列个理想* $(g_i)_{0 \leq i \leq n}$ *的* $g$ *与* $g_0 = g, g_n = \{0\}$，*使得* $[g, g_i] \subset g_{i+1}$ *和* $\dim g_i / g_{i+1} = 1$ *对于* $0 \leq i < n$。

如果 $\mathscr{C}^k g = \{0\}$（分别为 $\mathscr{C}_k g = g$），显然序列 $\mathscr{C}^1 g, \ldots, \mathscr{C}^k g$（分别为 $\mathscr{C}_k g, \mathscr{C}_{k-1} g, \ldots, \mathscr{C}_0 g$）具有定义 1 的性质，因此 $g$ 是幂零的。反之，假设存在序列 $(g_i)_{0 \leq i \leq p}$，其性质为定义 1。由归纳在$n$上看出$g_i \supset \mathscr{C}^{i+1} g$和$g_{p-i} \subset \mathscr{C}_i g$。因此$\mathscr{C}^{p+1} g = \{0\}$和$\mathscr{C}_p g = g$。由此我们证明条件 (a)、(b) 和 (c) 是等价的。另一方面，$\mathscr{C}^1 g$是形式元素线性组合集合

$$
[x_1, [x_2, \ldots, [x_{i-2}, [x_{i-1}, x_i]] \ldots]]
$$

其中$x_1, x_2, \ldots, x_i$穿过$g$。因此条件 (b) 和 (d) 是等价的。最后，如果存在序列 $(g_i)_{0 \leq i \leq p}$ 具有以下属性的理想

定义1，存在维数$n, n-1, n-2, \ldots, 0$$g$向量子空间递减序列$(\mathfrak{h}_i)_{0 \leq i \leq n}$和指标序列
$$
i_0 < i_1 < \cdots < i_p
$$
与 $g_0 = \mathfrak{h}_{i_0}, g_1 = \mathfrak{h}_{i_1}, \ldots, g_p = \mathfrak{h}_{i_p}$；那么 $[g, \mathfrak{h}_{i_k}] \subset \mathfrak{h}_{i_{k+1}}$ $\mathfrak{h}_i$ 是理想的，$[g, \mathfrak{h}_i] \subset \mathfrak{h}_{i+1}$ 对于所有 $i$ 来说都是理想的。因此条件 (a) 和 (e) 是等价的。

#### 推论 1 {#lie-i-s4-prop-1-cor-1 .statement tag=09WU}

*非零幂零李代数的中心是非零。*

#### 推论 2 {#lie-i-s4-prop-1-cor-2 .statement tag=09WV}

*杀死幂零李代数中的形式是零。*
对于幂零李代数中的所有$x$和$y$，$\operatorname{ad} x \circ \operatorname{ad} y$都是幂零的，因此零迹。

#### 命题 2 {#lie-i-s4-prop-2 .statement tag=09WW}

*子代数、幂零李代数的商代数和中心扩张是幂零的。 A finite product of nilpotent Lie algebras is a nilpotent Lie algebra.*
Let $g$ be a Lie algebra, $g'$ a subalgebra of $g$, $\mathfrak{h}$ an ideal of $g$, $\mathfrak{k} = g/\mathfrak{h}$ and $\phi$ the canonical mapping of $g$ onto $\mathfrak{k}$. 如果$g$是幂零的，那么$\mathscr{C}^k g = \{0\}$对于某些整数$k$，因此$\mathscr{C}^k g' \subset \mathscr{C}^k g = \{0\}$和$\mathscr{C}^k \mathfrak{k} = \phi(\mathscr{C}^k g) = \{0\}$以及$g'$和$\mathfrak{k}$是幂零的。 如果$\mathfrak{k}$是幂零的，并且$\mathfrak{h}$包含在$g$的中心中，则$\mathscr{C}^k \mathfrak{k} = \{0\}$对于某些整数$k$，因此$\mathscr{C}^k g \subset \mathfrak{h}$，因此$\mathscr{C}^{k+1} g \subset [\mathfrak{h}, g] = \{0\}$，因此$g$是幂零的。 最后，关于乘积的断言从命题1的断言(a)$\Leftrightarrow$(d)得出例。

定义 1 和命题 2 证明幂零李代数恰好是由中心扩张的李代数交换序列得到的代数。

#### 命题 3 {#lie-i-s4-prop-3 .statement tag=09WX}

*令$g$为幂零李代数且$g$的$\mathfrak{h}$子代数与$g$不同。 $g$ 中$\mathfrak{h}$的归一化器与$\mathfrak{h}$不同。*
令$k$为最大的整数，使得$\mathscr{C}^k g + \mathfrak{h} \neq \mathfrak{h}$。然后
$$
[\mathscr{C}^k g + \mathfrak{h}, \mathfrak{h}] \subset \mathscr{C}^{k+1} g + \mathfrak{h} \subset \mathfrak{h}
$$
因此$g$包含于$\mathscr{C}^k g + \mathfrak{h}$中的$\mathfrak{h}$标准化。

### 2.恩格尔的定理

#### 引理 1 {#lie-i-s4-lem-1 .statement tag=09WY}

*令 $V$ 为向量空间超过 $\mathbf{K}$。如果$x$是$V$的幂零自同态，$\mathscr{L}(V)$的映射$y \mapsto [x, y]$到$\mathscr{L}(V)$是幂幂的。*
如果$f$表示该映射，则$f^m(y)$与$i + j = m$为形式$\pm x^i y x^j$项和。如果$x^k = 0$，则$f^{2k-1}(y) = 0$适用于所有$y$。

#### 定理 1（恩格尔）{#lie-i-s4-thm-1 .statement tag=09WZ}

*设$V$是$\mathbf{K}$上的向量空间，$g$是$\mathfrak{gl}(V)$的有限维子代数，其元素是$V$的幂零自同态。如果$V \neq \{0\}$，$V$中存在$u \neq 0$，使得$x.u = 0$对于所有$x \in g$。*

证明在$g$的维数$n$继续进行归纳。如果$n = 0$，则定理是明显的。假设对于维数 $< n$ 的代数成立。

设$h$是维数$m < n$的$g$的谎言子代数。如果 $x \in h$ 和 $\mathrm{ad}_g x$ 映射 $h$ 自身和定义对经过的商自同态 $\sigma(x)$ 与空间 $g/h$。到引理 1 $\mathrm{ad}_g x$ 是幂零的，因此 $\sigma(x)$ 是幂零的。到归纳假设时，存在 $g/h$ 的非零元素，它被所有 $\sigma(x),\ x \in h$ 湮灭。由此可见，$h$是$g$的某个$(m+1)$维子代数中的理想。

我们结论（通过从$h = \{0\}$开始迭代）$g$的理想$h$为维数$n-1$。让$a \in g,\ a \notin h$。我们再次使用归纳假设：$u \in V$，使得$x.u = 0$对于所有$x \in h$形式，向量子空间U为V的非零向量子空间U。这个子空间在$a$（§ 3, no. 5，命题5）下是稳定的。由于$a$是V的幂零自同态，因此存在U的非零元素，它被$a$湮灭，因此被$g$的每个元素湮灭。

#### 推论 1 {#lie-i-s4-thm-1-cor-1 .statement tag=09X0}

*For a Lie algebra g to be nilpotent, it is necessary and sufficient that, for all $x \in g$, $\mathrm{ad}\ x$ be nilpotent.*

条件是必要的 (命题 1)。假设对于维数$< n$($n \neq 0$)的李代数已证明其充分性。令$g$为$n$维李代数，使得对于所有$x \in g$，$\mathrm{ad}\ x$是幂零的。 定理 1，应用于$\mathrm{ad}\ x\ (x \in g)$的集合，证明$g$的中心$c$非零。那么$g$是李代数$g/c$的中心扩张，它对于我们的归纳假设是幂幂的。 证明由应用命题 2 完成。

#### 推论 2 {#lie-i-s4-thm-1-cor-2 .statement tag=09X1}

*设 g 为李代数，h 为 g 的理想。假设 $g/h$ 是幂零的，并且对于所有 $x \in g$，$\mathrm{ad}\ x$ 到 h 的限制是幂零的。那么 g 是幂零的。*

让$x \in g$。由于$g/h$幂零，因此存在整数$k$使得$(\mathrm{ad}\ x)^k(g) \subset h$。到假设时，存在整数$k'$使得$(\mathrm{ad}\ x)^{k'}(h) = \{0\}$。因此$(\mathrm{ad}\ x)^{k+k'}(g) = \{0\}$。因此，推论 2 是推论 1 的推论。

#### 推论 3 {#lie-i-s4-thm-1-cor-3 .statement tag=09X2}

*令V为向量空间，g为$\mathfrak{gl}(V)$的有限维子代数，其元素为V的幂零自同态。那么 g 就是幂零李代数.*

这直接从引理 1 和推论 1 得出。

#### 例 {#lie-i-s4-n2-exa-1 .statement tag=09X3}

代数 $\mathfrak{n}(n, K)$ (§ 1, no. 2, 例 2 (3)) 幂零。

### 3. 最大的表示的幂零理想

#### 引理 2 {#lie-i-s4-lem-2 .statement tag=09X4}

*设 g 为李代数，g 的一个理想，M 是一个简单的 g 模。如果对于所有 $x \in a,\ x_M$ 都是幂零的，那么 $x_M = 0$ 对于所有 $x \in a$.*

令 N 为 $m \in M$ 的 M 由……组成的子空间，使得所有 $x \in a$ 都有 $x_M.m = 0$。 定理1、$N \neq \{0\}$。另一方面，对于所有$y \in g$，N 在$y_M$（§ 3, no. 5，命题 5）下是稳定的。因此$N = M$，证明了引理。

#### 引理 3 {#lie-i-s4-lem-3 .statement tag=09X5}

*设g为李代数，g的一个理想，M为有限维的g模*

K 和 $(M_i)_{0 \leq i \leq n}$ $g$-模块 $M$ 的 Jordan-Hölder 级数。以下条件是等效的：

(a) 对于所有 $x \in a$，$x_M$ 是幂零的；
(b) 对于所有 $x \in a$，$x_M$ 位于由 1 和 $y_M$ 生成的结合词代数 $A$ 的雅各布森根式中，其中 $y \in g$；
(c) 对于所有$x \in a$，
$$
x_M(M_0) \subset M_1, x_M(M_1) \subset M_2, \ldots, x_M(M_{n-1}) \subset M_n.
$$

如果满足这些条件，则$a$相对于与$g$模块$M$相关联的双线性形式正交于$g$。

(b) $\Rightarrow$ (a)：由于 $A$ 是 $K$ 上的有限维，$A$ 的雅各布森根是幂零理想 (*代数*, 章 VIII, § 6, no. 4, 定理 3)，因此每个元素这个根式是幂幂的。

(a) $\Rightarrow$ (c)：每个 $Q_i = M_i/M_{i+1}$ ($0 \leq i < n$) 都是一个简单的 $g$ 模块。对于所有$x \in a$，如果条件 (a) 成立，则自同态$x_{Q_i}$（通过将$M_i$和经过限制为商而从$x_M$导出）是幂零的，因此零乘以引理 2；其他字、$x_M(M_i) \subset M_{i+1}$。

(c) $\Rightarrow$ (b)：假设条件 (c) 成立；让$x \in a$和$z \in A$。然后$z(M_i) \subset M_i$（$0 \leq i < n$），因此$(zx_M)^n(M) = \{0\}$；因此 $Ax_M$ 是 $A$ 的左 Nilideal，因此包含在 $A$ 的 Jacobson 根式中（*代数*，章 VIII, § 6, no. 3，推论 3 到定理 1）。

最后，假设条件 (a)、(b) 和 (c) 成立。设$x \in a$和$y \in g$。我们刚刚看到$y_M x_M$是幂零的，因此$\operatorname{Tr}(y_M x_M) = 0$，它证明了最后一个断言或引理。

#### 命题 4 {#lie-i-s4-prop-4 .statement tag=09X6}

令$g$为李代数，$M$为有限维在$K$上的$g$模，$A$由$x_M$（$x \in g$）的1和集合生成的关联代数。

(a) $g$ 的理想$a$ 使得$x_M$ 对所有$x \in a$ 幂幂都包含在其中一个$n$ 中。

(b) 理想的$n$是$x \in g$的集合，使得$x_M$属于为$A$的雅各布森根式。

(c) 设$(M_i)_{0 \leq i \leq n}$为$g$模块$M$的Jordan-Hölder级数；那么 $n$ 也是 $x \in g$ 的集合，使得 $(x)_{M_i/M_{i+1}} = 0$ 对于所有 $i$。

(d) $n$关于与$\varphi$相关的双线性形式与$g$正交。

$x \in g$的集合使得$x_M$属于对于$A$的雅各布森根显然是$g$的理想。 命题紧接着是引理 3。

#### 定义 2 {#lie-i-s4-def-2 .statement tag=09X7}

命题 4 的理想$n$称为$g$模$M$的最大的幂零理想或相应的表示的最大的幂零理想。

显然这个表示的$n$包含核。当 $M$ 为半单 (命题 4 (c)) 时，它等于它，但一般情况下不等于。应该注意的是，$g$的$x$的元素使得$x_M$幂零，并不一定是属于到$n$。

我们还发现注引理 3 的特殊情况立即给出以下结果：

#### 命题 5 {#lie-i-s4-prop-5 .statement tag=09X8}

令$V$是$K$上有限维$n$的向量空间，并且$g$是$gl(V)$的李子代数，其元素是$V$的幂零自同态。那么存在向量子空间 $V_0, V_1, \ldots, V_n$ $V$ 、维数 $n, n-1, \ldots, 0$ 的递减序列，使得$x(V_i) \subset V_{i+1}$ 对于所有$x \in g$ 和$i = 0, 1, \ldots, n-1$。

### 4. 最大的李代数的无能理想

令$g$为李代数，且$a$为$g$的理想。 对于$a$幂零，对于所有$x \in a$，$\operatorname{ad}_g x$幂幂是充分必要的； 条件显然是充分且必要的，因为，如果$a$是幂零的，$x \in a$，$\operatorname{ad}_a x$是幂零的，并且$\operatorname{ad}_g x$映射$g$入$a$，因此$\operatorname{ad}_g x$是幂零的。 然后将命题 4 应用于 $g$ 的伴随表示给出以下结果：

#### 命题 6 {#lie-i-s4-prop-6 .statement tag=09X9}

令 $g$ 为李代数，$E$ 为由 1 和 $\operatorname{ad}_g x$ ($x \in g$) 生成的 $\mathscr{L}(g)$ 的关联子代数。 Let $R$ be the Jacobson radical of $E$.
(a) The set $n$ of $y \in g$ such that $\operatorname{ad}_g y \in R$ is the largest nilpotent ideal of $g$.
(b) It is orthogonal to $g$ under the Killing form.

应该注意的是，$g/n$可以有非零幂零理想。

### 5. 基域的扩张

令$g$为李$K$代数，$K_1$扩张为$K$和$g' = g_{(K_1)}$。由于$\mathscr{C}^k g' = (\mathscr{C}^k g)_{(K_1)}$，$g$是幂零的当且仅当$g'$是幂零的。

令$M$是有限维在$K$、$n$最大的幂零上的$g$模，对于$M$和$M' = M_{(K_1)}$来说是理想的。令 $(M_i)_{0 \leq i \leq n}$ 为 $g$-模块 $M$ 的 Jordan-Hölder 级数。然后$x_M(M_i) \subset M_{i+1}$对于所有$i$和所有$x \in n$，因此

$$
x'_{M'}((M_i)_{(K_1)}) \subset (M_{i+1})_{(K_1)}
$$

对于所有$i$和所有$x' \in n_{(K_1)}$；因此$x'_{M'}$对于$x' \in n_{(K_1)}$是幂零的，因此$n_{(K_1)}$包含在最大的对于$M'$的幂零理想$n'$中。我们现在将看到，*如果 $K_1$ 在 $K$ 上可分，则 $n' = n_{(K_1)}$*。设 $E$ 为 1 与 $x_M$ ($x \in g$) 生成的结合 $K$ 代数，$E'$ 为 1 与 $x_{M'}$ ($x' \in g'$) 和 $R$ 生成的结合 $K$ 代数以及 $R'$ $E$ 和 $E'$ 的雅各布森部首。 代数 $E'$ 被规范地标识为 $E_{(K_1)}$。然后$R' = R_{(K_1)}$（*代数*，章VIII, § 7, no. 2，推论2（c）到命题3）。然后令 $y' \in n'$ 并写

$$
y' = \sum_{i=1}^n \lambda_i y_i,
$$

其中 $y_i$ 在 $g$ 中，$\lambda_i \in K_1$ 在 $K$ 上线性无关。然后是$y'_{M'} = \sum_{i=1}^n \lambda_i (y_i)_{M'}$和$y'_{M'} \in R' = R_{(K_1)}$。因此，对于所有 $i$，$(y_i)_M \in R$ 以及$y_i \in n$。由此可见$y' \in n_{(K_1)}$、从而$n' \subset n_{(K_1)}$。

特别是，如果$K_1$在$K$上可分，$g_{(K_1)}$的最大的幂零理想是通过将基域从$K$延伸到$K_1$而从$g$的幂幂理想导出的。

### 习题 {#lie-i-s4-exercises}

§ 4 的约定仍然有效，除非另有提及。

§ 4](exercises/s4/)参见[习题。
