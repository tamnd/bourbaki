---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 2
section_title: Negligible functions and sets
lang: zh
source: int-i-vi
book_pages: INT IV.11-INT IV.17
pdf_pages: 0118-0124
extraction: ocr
subsections:
    - "no": 1
      title: Negligible positive functions
      page: 11
      pdf_page: 118
    - "no": 2
      title: Negligible sets
      page: 12
      pdf_page: 119
    - "no": 3
      title: Properties true almost everywhere
      page: 12
      pdf_page: 119
    - "no": 4
      title: Classes of equivalent functions
      page: 13
      pdf_page: 120
    - "no": 5
      title: Functions defined almost everywhere
      page: 15
      pdf_page: 122
    - "no": 6
      title: Equivalence classes of functions with values in $\overline{\mathbf{R}}$
      page: 16
      pdf_page: 123
statements: 15
exercises: 0
content_sha256: 2983205bbbda558589771256a06a9bfd0dcd2f42a23d3b15495ec511b117e299
translated_from: content/en/int/IV/02_s2_negligible_functions_and_sets.md
translation_method: google
source_content_sha256: 48a74bb29ea2e0671914af4710029a73eeba8926caa6ba8d663276f288e2e1b1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 3c614828c2fdcec369cbf178111c61494ee86e9f2b88110498b2587f8bb79fa1
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。可以忽略不计的函数和集合

### 1. 可忽略不计的正值函数

#### 定义 1 {#int-iv-s2-def-1 .statement tag=08Q8}

— *给定局部紧凑空间 X* 上的测度 $\mu$，*数值函数* $f \geq 0$（*是否有限*）*如果* $|\mu|^*(f) = 0$，则在 X 上定义的测度 $\mu$ 可以忽略不计。

然后，我们还说 $f$ 是 $\mu$*-可忽略*，或者如果不会导致混淆，则简称为“可忽略”。

#### 命题 1 {#int-iv-s2-prop-1 .statement tag=08Q9}

— *如果* $f$ *是可忽略不计的函数* $\geq 0$，*则每个数值函数* $g$ *使得* $0 \leq g \leq \alpha f$（$\alpha$ *标量* $> 0$）*可以忽略不计*。对于，$0 \leq |\mu|^*(g) \leq \alpha |\mu|^*(f) = 0$。

#### 命题 2 {#int-iv-s2-prop-2 .statement tag=08QA}

— *和和序列* $(f_n)$ *可忽略不计的函数* $\geq 0$ *可忽略不计*。

对于，$|\mu|^*(\sum_n f_n) \leq \sum_n |\mu|^*(f_n) = 0$（§ 1, No. 3，提案 13）和$\sup_n f_n \leq \sum_n f_n$。

#### 命题 3 {#int-iv-s2-prop-3 .statement tag=08QB}

*为了使$X$上的下半连续函数$f \geq 0$可以忽略不计，在$\mu$的支持下$f$为零是必要且充分的。*

如果$|\mu|^*(f) = 0$，则对于每个函数$g \in \mathscr{K}_+$，$|\mu|(g) = 0$使得$g \leq f$；由此得出（第 III, § 2, No. 3 章，第 9 条命题）$g$ 在$\mu$ 的支撑$S$ 上是零；因为 $f$ 是函数 $g \in \mathscr{K}_+$ 的上包络线，因此 $g \leq f$ (§ 1, No. 1, 引理), $f(x) = 0$ on $S$。相反，如果$f(x) = 0$在$S$上，那么对于每个函数$g \in \mathscr{K}_+$，$g(x) = 0$在$S$上，使得$g \leq f$，因此（第III, § 2, No. 3，第8条命题）$|\mu|(g) = 0$，其中， 定义，意味着$|\mu|^*(f) = 0$。

### 2. 可以忽略不计集合

#### 定义 2 {#int-iv-s2-def-2 .statement tag=08QC}

*给定局部紧凑空间$X$上的措施$\mu$，如果$|\mu|^*(A) = 0$，则$X$的子集$A$对于措施$\mu$来说可以忽略不计。*

也有人说 $A$ 是 $\mu$ - 可以忽略不计，或者如果不会导致混淆，则可以忽略不计。说特征函数 $\varphi_A$ 可以忽略不计也是同样的道理。

#### 命题 4 {#int-iv-s2-prop-4 .statement tag=08QD}

*每一个子集可以忽略不计的集合都是可以忽略不计的；每个可数的并可以忽略不计的集合都是可以忽略不计的。*

这是道具的直接的推论。 1 和 2。

#### 例 {#int-iv-s2-n2-exa-1 .statement tag=08QE}

— 令 $\mu$ 为$\mathbf{R}$ 的勒贝格测度。每集合 $\{x_0\}$ 减少到点都可以忽略不计（cf. § 1, No. 3，*注* 1）。因此，*$\mathbf{R}$ 中的每个可数子集对于勒贝格测度来说都是可以忽略不计的*。这个命题中的逆命题不正确（§ 4，Exer.4 b））。

#### 命题 5 {#int-iv-s2-prop-5 .statement tag=08QF}

*$\mu$的支持$S$的补集是最大的，在$X$中打开集合可以忽略不计。*

因为，根据命题3，在阶中，开集合$G$可以忽略不计，$G \cap S = \varnothing$即$G \subset \mathbf{C}S$是充分必要的。

### 3.属性几乎在任何地方都是正确的

令 $X$ 为局部紧致空间，$\mu$ 为$X$ 的测度。如果 $P\{x\}$ 是性质，性质 « $P\{x\}$ 几乎处处（相对于 $\mu$）» 通过定义等价于 x 的性质 « *集合，使得* $(x \in X \text{ and not } P\{x\})$ * 是 $\mu$*-可忽略 »。

#### 定理 1 {#int-iv-s2-thm-1 .statement tag=08QG}

— 在阶中，$X$ 上定义的数值函数（有限或非有限）$f \geqslant 0$ 可以忽略不计，$f(x) = 0$ 几乎无处不在是必要且充分的。

条件是必要的。例如，假设$f$可以忽略不计，并令$N$为$x \in X$的集合，使得$f(x) \neq 0$；那么 $\varphi_N \leqslant \sup_n (n f)$，因此 $\varphi_N$ 可以忽略不计（No. 1，提案 1 和 2）。

条件就足够了。假设点的集合 $N$，其中 $f(x) \neq 0$ 可以忽略不计；那么 $f \leqslant \sup_n n \varphi_N$，因此 $f$ 可以忽略不计（No. 1，提案 1 和 2）。

#### 命题 6 {#int-iv-s2-prop-6 .statement tag=08QH}

— 如果$f$和$g$是在$X$上定义的两个函数$\geqslant 0$（有限或非有限），使得$f(x) = g(x)$几乎无处不在，则$|\mu|^*(f) = |\mu|^*(g)$。

令 $N$ 为点 $x \in X$ 的可忽略不计的集合，使得 $f(x) \neq g(x)$。除了$N$的点之外，函数$\inf(f, g)$和$\sup(f, g)$相等，只要假设$f \leqslant g$即可证明命题。令$h$在$N$的点处函数等于$+\infty$，并在$CN$处等于0；那么$f \leqslant g \leqslant f + h$，因此

$$
|\mu|^*(f) \leqslant |\mu|^*(g) \leqslant |\mu|^*(f + h) \leqslant |\mu|^*(f) + |\mu|^*(h) = |\mu|^*(f)
$$

（因为 $h$ 可以忽略不计），从而命题。

#### 命题 7 {#int-iv-s2-prop-7 .statement tag=08QI}

— 如果 $f$ 是在 $X$ 上定义的函数 $\geqslant 0$，使得 $|\mu|^*(f) < +\infty$，则 $f(x)$ 几乎处处是有限的。

例如，令$N$为点$x \in X$中的集合，使得$f(x) = +\infty$；对于每个整数 $n$、$n \varphi_N \leqslant f$、从而 $n |\mu|^*(\varphi_N) \leqslant |\mu|^*(f)$；因为$n$是任意大的，$|\mu|^*(N) = 0$。

然而，即使 $X$ 是紧致的，函数 $f \geqslant 0$ 定义在 $X$ 上并且在任何地方有限都可以有无限上积分，如例 $X = [0, 1]$、$f(x) = 1/x$ 对于 $x > 0$ 和 $f(0) = 0$ 所示，$\mu$ 是勒贝格测度$X$。

### 4. 类相当于函数

令 $\mu$ 为局部紧凑空间 $X$ 的测度。给定集合$F$，$X$的两个映射$f, g$进入$F$被认为是*等价于*$\mu$（或$\mu$-*等价*，或者简单地*等价*，如果不会出现混淆）如果$f(x) = g(x)$*几乎$X$ 中随处*。由于两个可以忽略不计的集合并可以忽略不计，这样一来确实可以将定义中的一个等价关系中的$X$所有映射中的集合$F^X$转化为$F$；当我们谈到这样的函数$f$的*等价类*时（没有进一步说明），它将被理解为所有函数中的类几乎在任何地方都等于$f$；在这个章以及随后的那些中，我们将用记号$\tilde{f}$来表示这个类。

#### 命题 8 {#int-iv-s2-prop-8 .statement tag=08QJ}

*设*$(F_n)$*为集合的可数族（有限或无限）。对于每个指标 n，让* $f_n, g_n$ *成为X的两个等价的映射到* $F_n$； *然后，存在一个可忽略的集合 H，使得对于每个* $x \notin H$，$f_n(x) = g_n(x)$ *对于所有 n*。

对于$x \in X$的集合$H_n$，使得$f_n(x) \neq g_n(x)$可以忽略不计，因此它们的并H也可以忽略不计（No. 2，命题4），而这个集合满足要求。

#### 推论{#int-iv-s2-n4-cor-1 .statement tag=08QK}

*If* $\varphi$ *is a mapping of* $\prod_n F_n$ *into a set G, then the mappings* $\varphi((f_n))$ *and* $\varphi((g_n))$ *of X into G are equivalent*.

我们用每个函数$\varphi((f_n))$的$\varphi((\tilde{f}_n))$等价类来表示，其中$f_n$是类$\tilde{f}_n$中的任意函数。

特别是，如果 F 是 $\mathbf{R}$ 上的 *向量空间*，则定义 $\tilde{f} + \tilde{g}$ 和 $\alpha \tilde{f}$ 分别为 $f + g$ 和 $\alpha f$ 的等价类（$f$ 和 $g$ 分别为映射） X 代入 F，$\alpha$ 为标量）；这样，我们将X映射等价类集合代入F，得到一个*向量空间*结构：而且，这是$F^X$的*商空间*结构通过线性映射 $f$的子空间使得$\tilde{f} = \tilde{0}$（函数几乎到处都是零），我们也称之为*可忽略*函数（F中的值）。 一个定义类似地乘积$\tilde{g} \tilde{f}$，其中$\tilde{f}$是F中X的映射的等价类，$\tilde{g}$是在X上定义的（有限）数值函数的等价类：因此，F 中的 X 映射等价类集合在 X 上定义的有限数值函数的等价类集合上配备有*模* 结构（其本身配备有*环*结构）。 如果F是$\mathbf{R}$上的*代数*，则将X的映射等价类集合上的代数结构类似地变成F中的一个定义。

设 F 是一个*可度量*拓扑空间，并考虑 F 上的统一结构与其拓扑兼容，并由伪计量学$\rho_n$（GT、IX, §§1 和 2）的*可数*族定义；在阶中，X 的两个映射 $f, g$ 等价于 F 中，函数 $\rho_n(f, g)$ 的数值*可忽略不计*是充分必要的；因为，这相当于说，X中存在一个可忽略不计的集合 H，这样，对于每个$x \notin H$，对于所有$n$，$\rho_n(f(x), g(x)) = 0$，即$f(x) = g(x)$。 特别地，如果 F 是可度量的局部凸空间，且 $(q_n)$ 是定义 F 的拓扑的可数半范数族（TVS，II, §4, No. 1），则在阶中，X 的两个映射 $f, g$ 等价于 F，则所有数值是充分必要的函数 $q_n(f(x) - g(x))$ 可以忽略不计。

#### 命题 9 {#int-iv-s2-prop-9 .statement tag=08QL}

— 设$f$和$g$为$X$的两个连续映射，形成豪斯多夫拓扑空间$F$；为了使$f$和$g$等价，$\mu$的支持度每点有$f(x) = g(x)$是必要且充分的。

对于$x \in X$的集合，使得$f(x) \neq g(x)$是开集合（GT，I, §8, No. 1）；为了使其可以忽略不计，它不与 $\mu$ 的支持相交是必要且充分的（No. 2，命题 5）。

#### 命题 10 {#int-iv-s2-prop-10 .statement tag=08QM}

— 令$F$为$\mathbf{R}$上的Hausdorff局部凸空间，使得$F$序列$(a'_n)$的对偶$F'$中存在弱拓扑$\sigma(F', F)$稠密（TVS，II, §6, No. 2）。在阶中，$X$到$F$的两个映射$f, g$是等价的，对于每个$n$，数值函数、$\langle f(x), a'_n \rangle$和$\langle g(x), a'_n \rangle$是等价的充分必要。

条件显然是必要的。相反，如果满足，则存在可忽略的集合$H$，使得对于每个$x \notin H$，对于每个$n$有$\langle f(x), a'_n \rangle = \langle g(x), a'_n \rangle$；这意味着$F'$上的弱连续线性形式$z' \mapsto \langle f(x), z' \rangle$和$z' \mapsto \langle g(x), z' \rangle$在每个点$a'_n$处都是相等的，因此凭借假设是相同的，这证明了$f(x) = g(x)$对于所有$x \notin H$。

注，第 10 条命题的假设尤其适用于当 $F$ 是可度量且可分离的局部凸空间时（TVS，III, §3, No. 4，第 6 条命题的 Cor.2）。

### 5. 函数几乎无处不在

In conformity with the definition in No. 3, a mapping $f$ of a subset $A$ of $X$ into a set $F$ is said to be defined almost everywhere if the complement of the set $A$ on which it is defined is a negligible set. 我们再次调用$f$的等价类，并用$\tilde{f}$表示，在所有$X$上定义的每个函数的等价类等于定义$f$的点$x \in X$处的$f(x)$；显然，这个类仅取决于$f$。 如果$\tilde{f} = \tilde{g}$，则几乎在任何地方定义的两个函数$f, g$再次被认为是等价的：因此，这意味着点的集合，其中$f(x)$和$g(x)$都已定义并且相等，其补数可以忽略不计。

It follows at once that Prop. 8 of No. 4 and its corollary may be generalized to the case where in their statements it is assumed only that each of the functions $f_n, g_n$ is defined almost everywhere; then the functions $\varphi((f_n))$

1 原文为 de 型 dénombrable，也可译为“可数型”（GT、IX, §2, No. 8、Def.4）或“第二可数”，或“满足可数性第二公理”。在此处引用的 TVS 推论中，项“满足可数性第一公理”应替换为前述项之一。

和 $\varphi((g_n))$ 本身几乎到处都有定义； $\varphi((f_n))$的等价类又是$\varphi((\tilde{f}_n))$。

函数几乎到处都有定义，向量空间 F 中的值，如果等于 0，则再次被称为“可忽略”。如果 f 是可忽略的函数，且值在 F 中，并且 u 是 F 到向量空间 G 中的线性映射，则复合函数 $u \circ f$（几乎到处都有定义）可以忽略不计；类似地，对于每个（有限）数值函数 g（几乎在任何地方都定义），函数 $gf$（几乎在任何地方都定义）可以忽略不计。

必须注意观察到，在函数的集合以及 F 中的值且几乎到处都有定义的情况下，合成 $(f, g) \mapsto f + g$ 的内部律 * 不是群运算*，因为，而函数 0 确实是一个中性元素律，如果 f 不是处处定义，则不存在函数 g 使得 $f + g = 0$。这就是等价类 $\tilde{f}$ 引入的动机，形式向量空间的作用。

让$(f_n)$是映射的序列变成*拓扑空间*F，其中每个在X中几乎到处都有定义。我们说序列 $(f_n)$ *几乎处处收敛于 f in* X，如果点 $x \in X$ 的集合其中定义了所有 $f_n(x)$ 并且序列 $(f_n(x))$ 的极限等于$f(x)$，补数可以忽略不计。很明显，如果对于每个 n，函数 $g_n$（几乎处处定义）等价于 $f_n$，则序列 $(g_n)$ 几乎处处收敛于 $f$。

如果F是*拓扑向量空间*，一个定义类似地是一个*几乎处处收敛的级数*，其一般项是函数$f_n$几乎处处定义在X中，值在F中；这个级数的和是在点定义的函数，其中定义了部分和$\sum_{k=1}^n f_k(x)$并具有极限，并且其类仅依赖于类$\tilde{f}_n$。

### 6. 函数中的等价类，值位于 $\overline{\mathbf{R}}$ 中

与 No. 3 中的定义一致，我们说 X 中几乎所有地方都定义的函数 $f$ 以及 $\overline{\mathbf{R}}$ 中的值，如果定义了 $f(x)$ 的 $x \in X$ 的集合则“几乎处处有限”并且有限的补数可以忽略不计。几乎处处有限的函数等价于*处处有限*的函数；因此，我们可以将认同其类$\tilde{f}$与类的*有限*数值函数定义在X（或X中的几乎所有地方）。特别地，几乎处处定义了有限的函数的两个类的和和乘积，并且这些类的集合是$\mathbf{R}$上的*代数*。如果 $(f_n)$ 是函数的序列，值在 $\overline{\mathbf{R}}$ 中，几乎处处定义且有限，则部分和 $\sum_{k=1}^n f_k(x)$ 几乎处处定义；如果，对于几乎每个$x \in X$，它们在$\overline{\mathbf{R}}$中有极限$f(x)$，我们再次说级数与一般项$f_n$几乎处处收敛，并且$f$是级数的和 （注 $f$ 几乎在任何地方都不一定是有限的）。

如果$f$和$g$是两个数值函数，在$X$中几乎处处定义且有限，则$\tilde{f} + \tilde{g}$（分别$\tilde{f} \tilde{g}$）是每个函数的类等于$f(x) + g(x)$（分别$f(x)g(x)$） 点 $x \in X$ 这个表达式有意义。 注$f$和$g$都可以“随处定义”，而无需为所有$x$（GT，IV, §4, No. 3）定义$f(x) + g(x)$（分别为$f(x)g(x)$）；通过定义 $f + g$（分别为 $fg$），函数等于 $f(x) + g(x)$（分别为 $f(x)g(x)$），在定义此表达式的位置为点；因此，它几乎在所有地方都被定义。

令 $f$ 和 $g$ 为两个数值函数（有限或非有限），在 $X$ 中几乎处处定义，使得 $f(x) \leq g(x)$ 几乎处处；如果$f_1$等价于$f$，并且$g_1$等价于$g$，那么显然$f_1(x) \leq g_1(x)$几乎无处不在。因此，所讨论的关系仅取决于$f$和$g$中的类；一写$\tilde{f} \leq \tilde{g}$，立刻验证这个关系是函数的等价类的集合中的*序关系*和$\overline{\mathbf{R}}$中的值。如果$(\tilde{f}_n)$是此类类的可数族（有限或无限），并且如果对于每个$n$，$f_n$和$g_n$是几乎处处定义的两个函数，并且属于到类$\tilde{f}_n$，则可以从命题1得出。 No. 4中的8个函数、$\sup_n f_n$和$\sup_n g_n$几乎在任何地方都有定义，是等价的；因此，它们的类仅取决于类$\tilde{f}_n$，并且立即验证它是函数的类的集合中的这些类的*最高值*$\sup_n \tilde{f}_n$和值 $\overline{\mathbf{R}}$，以刚刚描述的方式排序（集合，因此，特别是*网格排序*）。一种类似地表明了下确界 $\inf_n \tilde{f}_n$ 的存在，另一种则具有 $\inf_n \tilde{f}_n = -\sup_n (-\tilde{f}_n)$。由此可见，$\limsup_{n \to \infty} f_n$和$\limsup_{n \to \infty} g_n$也是等价的，它们的类记为$\limsup_{n \to \infty} \tilde{f}_n$，等于$\inf_n (\sup_{p \geq 0} \tilde{f}_{n+p})$； $\liminf_{n \to \infty} \tilde{f}_n$ 的定义类似。

如果数值函数 $f$（无论是否有限）等于 0，则称其为“可忽略”；这个定义相当于Def。 1 对于函数是正的并且到处都有定义，凭借 Th. 1. 要使$f$可以忽略不计，$|f|$可以忽略不计（或者$f^+$和$f^-$都可以忽略）是充分必要的。
