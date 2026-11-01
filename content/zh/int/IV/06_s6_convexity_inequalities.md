---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 6
section_title: Convexity inequalities
lang: zh
source: int-i-vi
book_pages: INT IV.89-INT IV.100, INT IV.134-INT IV.142
pdf_pages: 0196-0207, 0241-0249
extraction: ocr
subsections:
    - "no": 1
      title: The convexity theorem
      page: 89
      pdf_page: 196
    - "no": 2
      title: Inequality of the mean
      page: 90
      pdf_page: 197
    - "no": 3
      title: The spaces $L^\infty_F$
      page: 91
      pdf_page: 198
    - "no": 4
      title: Hölder’s inequality
      page: 93
      pdf_page: 200
    - "no": 5
      title: 'Application: relations between the spaces $L^p_F$ ($1 \leq p \leq +\infty$)'
      page: 98
      pdf_page: 205
statements: 22
exercises: 20
content_sha256: 89e18b5f816ed55fd4a1d938f235bb90538999b3c4a1c7d492b5a460205f1960
translated_from: content/en/int/IV/06_s6_convexity_inequalities.md
translation_method: google
source_content_sha256: 5da8e094f0389b678ca69f52f247e8417940837f7695de9c80ebdf9dcbcce321
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 578a3d9460c638ff32b1c1d8d55a1c82246e675227a5b2f28a0591700106fda6
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 6。凸性不等式

### 1.凸度定理

#### 定理 1 {#int-iv-s6-thm-1 .statement tag=08XD}

— 令 $X$ 为局部紧凑空间，$\mu$ $X$ 上的正测度，$F$ 为真正的 Banach 空间，$D$ $F$ 中的闭凸集合，以及 $f$ 函数 $X$使得$f(X) \subset D$。对于每个不可忽略的可积数值函数$g \geqslant 0$，使得$fg$可积，点$\frac{\int fg\, d\mu}{\int g\, d\mu}$属于到$D$。

例如，令 $F'$ 为 $F$ 的对偶，并令 $\langle z, a' \rangle \leqslant \alpha$ ($a' \in F', \alpha \in \mathbf{R}$) 为关系，定义闭半空间包含 $D$。由于 $fg$ 是可积的，因此数值函数 $\langle fg, a' \rangle = \langle f, a' \rangle g$ 也是可积的，并且

$$
\int \langle fg, a' \rangle\, d\mu = \left\langle \int fg\, d\mu, a' \right\rangle
$$

（§ 4, No. 2，第 1 章第 1 条）；但是，通过假设，$\langle f(x), a' \rangle \leqslant \alpha$对于所有$x \in X$，因此$\langle f(x)g(x), a' \rangle \leqslant \alpha g(x)$；在整合方面，我们有

$$
\left\langle \int fg\, d\mu, a' \right\rangle \leqslant \alpha \int g\, d\mu .
$$

这证明了点$\frac{\int fg\, d\mu}{\int g\, d\mu}$属于对于每个闭半空间包含$D$；但是，根据 Hahn-Banach 定理，$D$ 是闭半空间包含的交（TVS，II, §5, No. 3，第 4 条命题 1），从而定理。

#### 推出{#int-iv-s6-n1-cor-1 .statement tag=08XE}

— *如果正测度 $\mu$ 的总质量等于 1 并且 $f$ 可积，则 $\int f\, d\mu$ 属于到 $F$* 中$f(X)$ 的封闭凸包络线。

$g$取常数函数1就足够了。

### 2. 均值的不等式

我们要磨砺Th。 1 表示可数值测量函数（有限或非有限）。

#### 定义 1 {#int-iv-s6-def-1 .statement tag=08XF}

— 令 X 为局部紧致空间，$\mu$ 为 X 的测度。给定一个数值函数 f（有限或非有限），在 X 中几乎所有地方都在本地定义，我们称函数 f 的测量最大值，或 $\mu$-最大值（分别为测量最小值，或 $\mu$-最小值），并用 $M_\infty(f)$（分别为 $m_\infty(f)$）表示， 数 $\alpha$ 的集合的下确界（或最高），使得 $f(x) \leq \alpha$（或$f(x) \geq \alpha$）局部几乎无处不在（对于 $\mu$）。

它立即从定义得出 $m_\infty(f) = -M_\infty(-f)$，因此，从度量中最大值的每一个性质可以推导出度量中最小值的相应的性质。

对于$x \in X$的每个$\alpha > M_\infty(f)$、集合，使得$f(x) > \alpha$局部可忽略不计；现在，$x \in X$的集合使得$f(x) > M_\infty(f)$是集合的并，其中$f(x) > r_n$，$r_n$超过有理数$> M_\infty(f)$的集合；因此，几乎所有地方都存在$f(x) \leq M_\infty(f)$ (§ 5, No. 2)。同样，几乎所有地方都存在$f(x) \geq m_\infty(f)$；由此可见，如果度量 $\mu$ 是非零的，则$m_\infty(f) \leq M_\infty(f)$；此外，关系$m_\infty(f) = M_\infty(f)$等价于说，$f$几乎在任何地方都等于局部常数。显然，如果度量$\mu$是非零的，那么

$$
\inf_{x \in X} f(x) \leq m_\infty(f) \leq M_\infty(f) \leq \sup_{x \in X} f(x).
$$

如果两个函数 $f, g$ 几乎处处局部相等，则 $m_\infty(f) = m_\infty(g)$ 和 $M_\infty(f) = M_\infty(g)$。

最后，如果$f$和$g$是两个函数，使得$f + g$几乎在任何地方都被本地定义，那么

(1)
$$
M_\infty(f + g) \leq M_\infty(f) + M_\infty(g)
$$
假设第二个成员已定义，如下所示，立即从 Def 开始。 1;类似地，如果 $f$ 和 $g$ 都是 $\geq 0$ 并且$fg$几乎在所有地方都被本地定义，那么

(2)
$$
M_\infty(fg) \leq M_\infty(f) M_\infty(g)
$$
前提是定义了第二个成员。

如果 $M_\infty(f) < +\infty$，则 $f(x) < +\infty$ 局部几乎无处不在，但不一定几乎无处不在。如果数值函数 $f$ 被称为在测度上有界（对于测度 $\mu$），如果它几乎在任何地方都被定义且有限，而且，如果数 $m_\infty(f)$ 和 $M_\infty(f)$ 都是有限的（后者条件等于说， $M_\infty(|f|) < +\infty$）。

#### 命题 1（平均值的不等式）{#int-iv-s6-prop-1 .statement tag=08XG}

— *令 f 为可测量的数值函数，其测量有界。对于每个可积数值函数 $g \geqslant 0$，函数 $fg$（几乎在任何地方都定义）是可积的并且*

$$
m_\infty(f) \int g d|\mu| \leqslant \int fg d|\mu| \leqslant M_\infty(f) \int g d|\mu|.
$$

此外，*不等式(3)不能的三个成员中的两个等于除非，在$x \in X$的集合中，使得$g(x) \neq 0$，f几乎处处等于$M_\infty(f)$或几乎处处等于$m_\infty(f)$*。

事实上，$fg$是可测量的（§ 5, No. 3，Th.1的Cor.5）；此外，不等式$m_\infty(f)g(x) \leqslant f(x)g(x) \leqslant M_\infty(f)g(x)$不仅在局部几乎所有地方都成立，甚至几乎在所有地方都成立，因为点$x \in X$的集合其中$g(x) \neq 0$是可积集合的可数并（§ 5, No. 6， 引理1)。由此可知 $fg$ 可积（§ 5, No. 6，Th. 5）且不等式 (3) 成立。另一方面，函数$M_\infty(f)g - fg$几乎到处都有定义并且等于$(M_\infty(f) - f)g$；因此，$\geqslant 0$几乎在$X$中无处不在；由于关系$M_\infty(f) \int g d|\mu| = \int fg d|\mu|$等价于$\int (M_\infty(f) - f)g d|\mu| = 0$，因此只有当函数$(M_\infty(f) - f)g$可以忽略不计时，它才能成立，从而完成证明。

设定撇开 $\int g d|\mu| = 0$、不等式 (3) 可以从 Th 推导出来的琐碎情况不谈。 No. 1 中的 1 应用于区间 $D = [m_\infty(f), M_\infty(f)]$。一个人可以把Th. No. 1 中的第 1 条类似于命题 1 的补码，指定点 $(\int fg d\mu)/(\int g d\mu)$ 属于到 D 边界的情况（例 2）。

### 3.空间$L^\infty_F$

#### 定义 2 {#int-iv-s6-def-2 .statement tag=08XH}

*将 $X$ 中的每映射 $f$ 放入 Banach 空间 $F$，即可得到 1 个集合 $N_\infty(f) = M_\infty(|f|)$；如果 $N_\infty(f)$ 是有限的，则 $f$ 被称为在测度上有界（对于测度 $\mu$）。 $X$ 的映射到 $F$ 的集合是可测量的并且在测量上有界，表示为 $\mathscr{L}_F^\infty(X, \mu)$（或 $\mathscr{L}_F^\infty(\mu)$，或简称为 $\mathscr{L}_F^\infty$）。*

因此，$\mathscr{L}_F^\infty$中的函数$f$的特征可能是存在一个“有界可测”的函数，几乎处处都等于$f$。

从 (1) 可以立即得出

$$
N_\infty(f + g) \leqslant N_\infty(f) + N_\infty(g);
$$

另一方面，对于每个标量 $\alpha$，$N_\infty(\alpha f) = |\alpha| N_\infty(f)$。因此，集合$\mathscr{L}_F^\infty$是$X$的所有映射到$F$的空间的*线性子空间*，而$N_\infty(f)$是这个向量空间的半范数。令$(f_n)$为$\mathscr{L}_F^\infty$中函数的序列，对于由半范数$N_\infty(f)$定义的拓扑，收敛到$f \in \mathscr{L}_F^\infty$；对于每个整数 $m$，都存在局部可忽略的集合 $H_m$ 和整数 $n_0$，使得$|f(x) - f_n(x)| \leq 1/m$ 对于每个整数 $n \geq n_0$ 和每个$x \notin H_m$（每个可数） 并局部可忽略集合局部可忽略）； $H_m$ 的并 $H$ 局部可忽略不计，并且可以看到 $f_n(x)$ 在局部可忽略不计的集合 $H$ 的补集上“一致”趋向于 $f(x)$； 逆命题是直接的。

很明显，在 $\mathscr{L}_F^\infty$ 属于到 $\mathscr{L}_F^\infty$ 中，每个函数几乎在任何地方都等于函数。特别是，在$X$上定义的*局部可忽略的*函数和$F$形式中的值是$\mathscr{L}_F^\infty$的线性子空间$\mathscr{N}_F^\infty$，其特征在于关系$N_\infty(f) = 0$（闭包0 表示拓扑由 $N_\infty(f)$ 定义）。与 $\mathscr{L}_F^\infty$ 伴随的 Hausdorff 空间，即商空间 $\mathscr{L}_F^\infty / \mathscr{N}_F^\infty$，表示为 $L_F^\infty(X, \mu)$（或 $L_F^\infty(\mu)$ 或 $L_F^\infty$）；它的拓扑是由从 $N_\infty$ 通过商推导出来的 *范数* 定义的； 类$\dot{f} \in L_F^\infty$中的范数表示为$N_\infty(\dot{f})$，也可以表示为$\| \dot{f} \|_\infty$。当$F = \mathbf{R}$（或$\mathbf{C}$）时，如果不会造成混淆，我们会写成$\mathscr{L}^\infty$和$L^\infty$来代替$\mathscr{L}_\mathbf{R}^\infty$和$L_\mathbf{R}^\infty$（或$\mathscr{L}_\mathbf{C}^\infty$和$L_\mathbf{C}^\infty$）。

#### 命题 2 {#int-iv-s6-prop-2 .statement tag=08XI}

*空间* $\mathscr{L}_F^\infty$ *已完成； 空间* $L_F^\infty$ *是巴纳赫空间*。

例如，令$(f_n)$为$\mathscr{L}_F^\infty$中的柯西序列；对于每个整数$n$，都存在整数$k_n$，使得$N_\infty(f_r - f_s) \leq 1/n$对于$r \geq k_n$和$s \geq k_n$；因此，存在局部可忽略的集合$A_{rs}$，使得$|f_r(x) - f_s(x)| \leq 1/n$对于所有$x \notin A_{rs}$。如果$A_n$是集合$A_{rs}$的并（对于$r \geq k_n$和$s \geq k_n$），则$A_n$局部可忽略不计，并且对于每个$x \notin A_n$，$|f_r(x) - f_s(x)| \leq 1/n$对于所有指标 $r \geq k_n, s \geq k_n$。令$A$为$A_n$的并形成的局部可忽略的集合，$x \notin A$为集合$g_n(x) = f_n(x)$，$x \in A$为$g_n(x) = 0$；然后$g_n$属于到$\mathscr{L}_F^\infty$，并且通过$A$的定义，序列$(g_n)$*均匀地*在$X$收敛到函数$g$。由此可见函数 $g$ 是可测的（§ 5, No. 4，Th.2）；此外，$g$以$x \in X$的集合为界，其中$|g_{k_1}(x)| \leq N_\infty(g_{k_1})$，并且由于该集合的补集局部可忽略不计，$g$属于到$\mathscr{L}_F^\infty$。很明显，在$\mathscr{L}_F^\infty$中，序列$(g_n)$有极限$g$，因此序列$(f_n)$也是如此，因为$N_\infty(f_n - g_n) = 0$对于所有$n$都是如此。由此可以立即推导出命题的第二个部分。

#### 注 {#int-iv-s6-n3-rem-1 .statement tag=08XJ}

— 1) 每个*有界连续*函数$f$在$X$上，值在$F$属于到$\mathscr{L}_F^\infty$，并且

$$
N_\infty(f) \leq \| f \| = \sup_{x \in X} |f(x)| .
$$

在阶中，$N_\infty(f) = \|f\|$对于每个有界连续函数$f$，测度$\mu$的支持度等于$X$是必要且充分的。 For, if there exists a continuous 函数 $f$ with negligible compact support and not identically 零, then $N_\infty(f) = 0$ and $\|f\| > 0$.相反，如果$\mu$的支持度等于$X$，则对于每个有界连续函数$f$和每个数$\alpha < \|f\|$，$x \in X$的集合使得$|f(x)| > \alpha$开且非空，因此有外部测量$> 0$，显示$N_\infty(f) = \|f\|$。

当$\mu$的支持度等于$X$时，我们可以因此认同有界连续函数在$X$上的规范空间$C^b(X; F)$，值在$F$上，子空间为空间$L_F^\infty$。由于 $L_F^\infty$ 不是一般的 Hausdorff，所以子空间 $C^b(X; F)$ 在 $L_F^\infty$ 中一般不是闭的，但它在 $L_F^\infty$ 中的典范像是 $L_F^\infty$ 的闭子空间（在这种情况下还可以用 $C^b(X; F)$ 来识别）考虑）。一般来说，$C^b(X; F)$与$L_F^\infty$不同，也就是说，对于任意有界可测函数$f$，一般不存在几乎处处局部等于$f$的连续函数$g$（§ 5，Exer.12）。这意味着$X$的映射到$F$的空间$\mathscr{H}(X; F)$，连续有紧支撑，在$L_F^\infty$中通常不稠密，而在$1 \leq p < +\infty$的空间$L_F^p$中是稠密的（§ 3, No. 4。默认 2）。

2) 半范数$N_\infty$定义的拓扑比更细比拓扑在$L_F^\infty$上由测度收敛拓扑诱导的直接的（§ 5, No. 11）来说是直接的。

### 4. 霍尔德的不等式

在此编号中，$p$和$q$将表示两个实数，使得$1 \leq p \leq +\infty$、$1 \leq q \leq +\infty$，受关系$1/p + 1/q = 1$约束；因此，如果$1 < p < +\infty$则为$q = p/(p-1)$，如果$p = 1$则为$q = +\infty$，如果$p = +\infty$则为$q = 1$； $p$和$q$将被称为共轭指数。 注即关系$1 \leq p \leq 2$等价于$2 \leq q \leq +\infty$；仅当$p$和$q$等于2时$p = q$。

#### 定理 2（霍尔德的不等式）{#int-iv-s6-thm-2 .statement tag=08XK}

— 令 $f$ 和 $g$ 为两个几乎处处有限的数值函数，并且使得 $f$ 几乎处处等于 $L^p$ 中的函数以及 $g$ 至 $L^q$ 中的函数。那么，函数 $fg$（几乎在任何地方都定义）是可积的，并且

$$
N_1(fg) \leq N_p(f) N_q(g).
$$

Let $f_1$ (resp. $g_1$) be a function in $L^p$ (resp. $L^q$) to which $f$ (resp. $g$) is equal almost everywhere; $fg$ is equal almost everywhere to the function $f_1 g_1$, which is everywhere defined and finite, and which is measurable, being the product of two measurable functions (§ 5, No. 3, Cor. 5 of Th. 1). 如果 $1 < p < +\infty$，则 Hölder 的不等式用于上积分（第 1 章） I, No. 3, 命题 4) 产生不等式 (4), 关系 $N_1(fg) < +\infty$ 然后表明 $fg$ 是可积的 (§ 5, No. 6, Th. 5)。 如果 $p = 1$、$q = +\infty$、不等式 (4) 且$fg$ 可积，则为不等式的平均值的直接的推论（No. 2，命题 1）；因此定理在所有情况下都得到证明。

#### 推论 1 {#int-iv-s6-thm-2-cor-1 .statement tag=08XL}

— 令$F, G, H$为三个Banach空间，并令$(u, v) \mapsto \Phi(u, v)$为$F \times G$到$H$的连续双线性映射，使得$|\Phi(u, v)| \leq |u| \cdot |v|$。如果 $f \in \mathscr{L}_F^p$ 和 $g \in \mathscr{L}_G^q$，则函数 $\Phi(f, g)$ 可积且

$$
\left| \int \Phi(f, g)\, d\mu \right| \leq \int |\Phi(f, g)|\, d|\mu| \leq N_p(f) N_q(g).
$$

对于，$\Phi(f, g)$是可测量的（§ 5, No. 3，Th.1的Cor.5）；从 $|\Phi(f, g)| \leq |f| \cdot |g|$ 开始，推论由 Th 得出。 2 和 § 5, No. 6, Th 的可积准则。 5.

Cor 的两个特殊情况。 1 在应用中很重要：

#### 推论 2 {#int-iv-s6-thm-2-cor-2 .statement tag=08XM}

— 令$F$为实数（或复数）Banach空间，$F'$其强对偶（TVS，III, § 3, No. 1），并令$(z, z') \mapsto \langle z, z' \rangle$为$F \times F'$上的规范双线性形式。如果 $f \in \mathscr{L}_F^p$ 和 $g \in \mathscr{L}_{F'}^q$，则实数（或复数）函数 $\langle f, g \rangle$ 可积且

$$
\left| \int \langle f, g \rangle\, d\mu \right| \leq \int |\langle f, g \rangle|\, d|\mu| \leq N_p(f) N_q(g).
$$

对于，$|\langle z, z' \rangle| \leq |z| \cdot |z'|$。

当$F$是实数或复数希尔伯特空间时，我们知道它可以用它的对偶$F'$（TVS，V, § 1, No. 7）规范地识别。由于空间 $L_F^2$ 已完成，我们得到以下结果：

#### 推论 3 {#int-iv-s6-thm-2-cor-3 .statement tag=08XN}

— 令 $\mu$ 为$X$ 的正测度，$F$ 为实数（或复数）希尔伯特空间。在空间 $L_F^2$ 上，对称（分别为厄米特）形式

$$
(\widetilde{f}, \widetilde{g}) \mapsto \int \langle f, g \rangle\, d\mu
$$

定义希尔伯特空间结构，其中范数等于 $\| \widetilde{f} \|_2$。

#### 推论 4 {#int-iv-s6-thm-2-cor-4 .statement tag=08XO}

— 令 $F$ 为 Banach 空间，$f$ 函数 $\mathscr{L}_F^p$，$g$ 函数属于至 $\mathscr{L}^q$；那么函数 $fg$ 可积且

$$
\left| \int fg\, d\mu \right| \leq \int |fg|\, d|\mu| \leq N_p(f) N_q(g).
$$

#### 推论 5 {#int-iv-s6-thm-2-cor-5 .statement tag=08XP}

— 令$f_1, f_2, \ldots, f_n$为n正可积函数，并令$\alpha_1, \alpha_2, \ldots, \alpha_n$为n数$> 0$，使得$\sum_{i=1}^n \alpha_i = 1$；在这些条件下，函数$f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$是可积的并且

$$
\int f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n} d|\mu| \leqslant
\left( \int f_1 d|\mu| \right)^{\alpha_1} \left( \int f_2 d|\mu| \right)^{\alpha_2} \cdots \left( \int f_n d|\mu| \right)^{\alpha_n}.
$$

因为，乘积$f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$是可测量的，是可测量的函数（§ 5, No. 3，Th.1及其Cor.5）的乘积；由于不等式 (8) 对于上积分成立（I、No. 2，命题 2 的修正），函数 $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ 是可积的（§ 5, No. 6，Th.5），从而是推论。

科。 2 Th。 2 通过以下命题进行锐化：

#### 命题 3 {#int-iv-s6-prop-3 .statement tag=08XQ}

— 令 $\mu$ 为X 上的正测度，F 为实数或复数 Banach 空间，F' 为强对偶，$(z, z') \mapsto \langle z, z' \rangle$ $F \times F'$ 上的规范双线性形式。

1° 对于每函数 $f \in \mathscr{L}_F^p$ ($1 \leq p \leq +\infty$)，

$$
N_p(f) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$

因为 g 在 $\mathscr{L}_{F'}^q$ 中运行超过函数的集合，因此$N_q(g) \leq 1$。

2° 对于每函数 $g \in \mathscr{L}_{F'}^q$ ($1 \leq q \leq +\infty$)，

$$
N_q(g) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$

因为 f 在 $\mathscr{L}_F^p$ 中运行超过函数的集合，从而得到 $N_p(f) \leq 1$。

我们先证明关系(9)；我们区分两种情况。

（一）$1 \leq p < +\infty$。当 $N_p(f) = 0$ 时，关系 (9) 是微不足道的（因为 f 和 $\langle f, g \rangle$ 可以忽略不计），我们总是可以假设，在将 f 乘以标量时，$N_p(f) = 1$。首先假设 f 是可积步骤函数，$f = \sum_{k=1}^n a_k \varphi_{A_k}$，其中$A_k$是成对的不相交的（§ 4, No. 9，引理）。因此$\sum_{k=1}^n |a_k|^p \mu(A_k) = 1$乘假设。对于每个$\varepsilon > 0$，存在（对于每个指标 k）向量$a'_k \in F'$，使得$|a'_k|^q = |a_k|^p$如果$p > 1$（或$|a'_k| = 1$如果$p = 1$）和$\langle a_k, a'_k \rangle \geq (1 - \varepsilon)|a_k| \cdot |a'_k|$（TVS，IV,

§1, No. 3，提案 8）。 设定 $g = \sum_{k=1}^n a_k' \varphi_{A_k}$，如果$p > 1$，我们有$\sum_{k=1}^n |a_k'|^q \mu(A_k) = 1$（如果$p = 1$，则有$\sup_{1 \leq k \leq n} |a_k'| = 1$），因此$N_q(g) = 1$；另一方面，

$$
\int \langle f, g \rangle d\mu = \sum_{k=1}^n \langle a_k, a_k' \rangle \mu(A_k) \geq (1 - \varepsilon) \sum_{k=1}^n |a_k| \cdot |a_k'| \mu(A_k)
$$

并且，由于 $|a_k'| = |a_k|^{p/q} = |a_k|^{p-1}$ if $p > 1$ （或 $|a_k'| = 1$ if $p = 1$），我们有

$$
\int \langle f, g \rangle d\mu \geq (1 - \varepsilon) \sum_{k=1}^n |a_k|^p \mu(A_k) = (1 - \varepsilon) N_p(f) = 1 - \varepsilon,
$$

在这种情况下证明了关系 (9)。

让我们讨论$f$是$\mathscr{L}_F^p$中的任意元素使得$N_p(f) = 1$。对于每个$\varepsilon > 0$，都存在一个步骤函数$f_1 \in \mathscr{L}_F^p$，使得$N_p(f - f_1) \leq \varepsilon$（§ 4, No. 10，第19号提案的Cor.1）。根据我们刚才看到的，存在函数 $g \in \mathscr{L}_F^q$，使得 $N_q(g) = 1$ 和

$$
\int \langle f_1, g \rangle d\mu \geq N_p(f_1) - \varepsilon \geq 1 - 2\varepsilon.
$$

现在，

$$
\int \langle f, g \rangle d\mu = \int \langle f_1, g \rangle d\mu + \int \langle f - f_1, g \rangle d\mu
$$

并且，通过(6)，

$$
\left| \int \langle f - f_1, g \rangle d\mu \right| \leq N_p(f - f_1) N_q(g),
$$

从而

$$
\left| \int \langle f, g \rangle d\mu \right| \geq 1 - 3\varepsilon,
$$

这就证明了(9)。

(ii) $p = +\infty$。我们可以再次将自己限制在$N_\infty(f) > 0$的情况。令$\alpha$为任意数，使得$0 < \alpha < N_\infty(f)$；通过 $x \in X$ 的假设、集合，使得 $|f(x)| > \alpha$ 是可测量的且不可局部忽略，因此它是测量 $> 0$ 的包含紧集 $K$。由于$f$是可测的，因此存在测度$> 0$的紧集$K_1 \subset K$，使得$f$到$K_1$的限制是连续的。由此可见，对于每个$\varepsilon > 0$，在可积集合的有限数中存在$K_1$的划分，其中每个$f$的振荡为$\leq \varepsilon$； 集合 $A$ 中至少一个的度量 > 0。令 $a$ 为 $A$ 中 $f$ 的值之一；然后 $|a| > \alpha$ 和 $|f(x) - a| \leq \varepsilon$ 对于所有 $x \in A$。存在向量$a' \in F'$使得$|a'| = 1$和$|\langle a, a' \rangle| \geq |a| - \varepsilon$； 函数 $g = \varphi_A \cdot a'/\mu(A)$ 可积且 $N_1(g) = 1$；另一方面，

$$
\int \langle f, g \rangle d\mu = \frac{1}{\mu(A)} \int \langle f, a' \rangle \varphi_A d\mu.
$$

现在，人们可以写

$$
\int \langle f, a' \rangle \varphi_A d\mu = \langle a, a' \rangle \mu(A) + \int \langle f - a, a' \rangle \varphi_A d\mu,
$$

自从

$$
|\langle f - a, a' \rangle \varphi_A| \leq \varepsilon \varphi_A,
$$

我们看到

$$
\left| \int \langle f, g \rangle d\mu \right| \geq |\langle a, a' \rangle| - \varepsilon \geq |a| - 2\varepsilon > \alpha - 2\varepsilon;
$$

由于$\varepsilon$是任意的并且$\alpha$是任何数<$N_\infty(f)$，因此在这种情况下关系(9)也得到验证。

人们以完全相同的方式证明关系（10），分别考虑情况$1 \leq q < +\infty$和情况$q = +\infty$，并使用这样的事实：对于每个$z' \in F'$，$|z'| = \sup_{|z| \leq 1} |\langle z, z' \rangle|$乘以$F'$中范数的定义。

#### 注 {#int-iv-s6-n4-rem-1 .statement tag=08XR}

— 1) 令$\mathscr{E}$为$\mathscr{L}_{F'}^q$的稠密线性子空间；那么当$g$超过$\mathscr{E}$的交且$\mathscr{L}_{F'}^q$中函数的集合$B$时，公式(9)成立，使得$N_q(g) \leq 1$。因为，只要观察到$B$的内部$\overset{\circ}{B}$在$B$中是稠密的，并且$\overset{\circ}{B} \cap \mathscr{E}$在$\overset{\circ}{B}$中是稠密的，因为$\overset{\circ}{B}$是开放的。当$1 \leq q < +\infty$（即$1 < p \leq +\infty$）时，此注尤其适用于具有紧凑支撑（$F'$中的值）的连续函数的集合$\mathscr{E} = \mathscr{K}(X; F')$。但在这种情况下，公式 (9) 为真，因为 $g$ 超过 $B \cap \mathscr{K}(X; F')$，即使对于 $p = 1$ 也是如此。因为，如上所述，我们可以将自己限制在$f$是步长函数的情况。然后我们看到，如果$N_1(f) = 1$，那么对于每个$\varepsilon > 0$，都存在一个步骤函数$g \in \mathscr{L}_{F'}^\infty$，使得$|g(x)| \leq 1$对于所有$x \in X$和$|\int \langle f, g \rangle d\mu| \geq 1 - \varepsilon$。存在成对不相交的紧集$K_i$的有限数，使得$g$在每个$K_i$上都有一个常数值$a'_i$，并且这样，如果$K$是并 $K_i$，然后$\int |f| \varphi_{\mathscr{C}_K} d\mu \leq \varepsilon$。令$U_i$为$K_i$的邻域，使得集合$U_i$是成对不相交的，并令$h_i$为$X$到$[0, 1]$的连续映射，支持度包含在$U_i$且等于1 $K_i$。 设定 $h = \sum a'_i h_i$，我们在$K$上有$h(x) = g(x)$，在$X$上有$|h(x)| \leq 1$，因而

$$
\int |\langle f, h \rangle| \varphi_{\mathscr{C}_K} d\mu \leq \varepsilon
$$

因而$|\int \langle f, h \rangle d\mu| \geq 1 - 3\varepsilon$，这证明了我们的断言。类似的注可以制作为公式 (10)。

2) 设$\mu$是$X$的正测度，$f$是可测量的函数$\geq 0$（有限或非有限），其支持包含在紧集$K_n$的可数并中。然后，对于每个$p$使得$1 \leq p \leq +\infty$，

$$
(11) \quad N_p(f) = \sup \int^* |fg| d\mu,
$$

因为 $g$ 超过 $\mathscr{H}(X; \mathbf{R})$ 中函数的集合，因此$N_q(g) \leq 1$。因为，当$N_p(f) < +\infty$时，公式(11)是(9)的特例，因为$f$相当于$\mathscr{L}^p$中的函数（§ 5, No. 6，Th.5）。如果$N_p(f) = +\infty$，对于每个整数$n > 0$集合$f_n = \inf(n, f \varphi_{K_n})$。然后

$$
N_p(f_n) = \sup \int^* |f_n g| d\mu \leq \sup \int^* |f g| d\mu,
$$

从而，在经过到极限（假设序列$(K_n)$是递增），我们有$\sup \int^* |f g| d\mu = +\infty$（§ 1, No. 3，Th.3）。

#### 推论 {#int-iv-s6-n4-cor-1 .statement tag=08XS}

— *令$\mu$为$X$的正测度，$F$为Banach空间，$F'$其强对偶，$g$为$\mathscr{L}^q_{F'}$中的任何函数。然后，$L^p_F$上的线性形式，由$\mathscr{L}^p_F$上的线性形式$f \mapsto \int \langle f, g \rangle d\mu$通过商推导出来，是连续的，有范数$N_q(g)$。*

### 5.申请：关系空间 $L^p_F$ ($1 \leq p \leq +\infty$)

#### 命题 4 {#int-iv-s6-prop-4 .statement tag=08XT}

— *令 $f$ 为可测量的函数，其中值在 Banach 空间 $F$ 中； 数 $p$的集合$I$，使得$1 \leq p \leq +\infty$和$N_p(f)$是有限的，要么是空的，要么是$\overline{\mathbf{R}}$的区间。若$I$为非空，则映射$p \mapsto N_p(f)$中的限制至$I$是连续的；此外，如果$f$不可忽略，则$\log N_p(f)$是$1/p$在$\bar{I}$上的凸函数。

我们已经知道（I，No. 3，命题 5）*有限* 数 $p \geq 1$ 的集合 $J$，使得 $N_p(f) < +\infty$ 要么是空的，要么是一个区间，并且 $\log N_p(f)$ 是一个凸函数 $1/p$ on $J$（当$f$不可忽略时）；这当然意味着$p \mapsto N_p(f)$在$J$上的连续性。

如果$J$为空，则$I = \varnothing$或$I = \{+\infty\}$，并且命题在这种情况下是显而易见的；假设从此以后$J$是非空。如果 $f$ 可以忽略不计，命题也是明显的；假设从此以后 $f$ 不可忽略。如果 $s \in J$ 那么，对于每个有限的数 $p > s$、$|f|^p = |f|^s |f|^{p-s}$ 和不等式均值表明

$$
(12) \quad N_p(f) \leq (N_s(f))^{s/p} (N_\infty(f))^{(p-s)/p}.
$$

令$p$趋于$+\infty$，则有：

$$
\limsup_{p \to +\infty} N_p(f) \leq N_\infty(f).
$$

这就证明了如果$+\infty \in I$则$J$包含任意大数；因此$I$确实是$\overline{\mathbf{R}}$和$\overline{I} = \overline{J}$的区间。如果我们证明$p \mapsto N_p(f)$在$\overline{J}$上连续，并且足以在$J$的端点建立连续性，则命题得到证明。此外，我们可以假设$J$不约化到点。设$r$和$s$为$J$($r < s \leq +\infty$)的左右端点。令$A$为$x \in X$的（可测量）集合，使得$|f(x)| \geq 1$；然后

$$
\int |f|^p d|\mu| = \int |f|^p \varphi_A d|\mu| + \int |f|^p \varphi_{C_A} d|\mu|.
$$

由于$p \in J$趋向于$r$，$|f|^p \varphi_A$趋向于$|f|^r \varphi_A$，而递减，以及$|f|^p \varphi_{C_A}$趋向于$|f|^r \varphi_{C_A}$，而递增。因此$\int |f|^p \varphi_{C_A} d|\mu|$趋向于$\int^* |f|^r \varphi_{C_A} d|\mu|$（§ 1, No. 3，Th.3）。另一方面，$|f|^p \varphi_A$对于$p \in J$可积，$\int |f|^p \varphi_A d|\mu|$趋于$\int |f|^r \varphi_A d|\mu|$（§ 4, No. 3，命题4）。因此$\int |f|^p d|\mu|$趋于$\int^* |f|^r d|\mu|$，这就证明了$p \mapsto N_p(f)$在$r$的连续性。

如果$s < +\infty$，则可以在点、$s$应用相同的推理。最后，假设$s = +\infty$。由式（13）可知，

$$
\liminf_{p \to +\infty} N_p(f) \geq N_\infty(f).
$$

现在，令$a$为数，使得$0 < a < N_\infty(f)$。因为，到假设，存在$p$的有限值，使得$N_p(f) < +\infty$、$x \in X$的集合$A$，使得可测量且不可忽略的$|f(x)| \geq a$可凭借不等式进行积分$\varphi_A \leq (|f|/a)^p$；此外，我们由此不等式推断出$N_p(f) \geq a \cdot (|\mu|(A))^{1/p}$；让$p$趋向于$+\infty$，则可以得出$\liminf_{p \to +\infty} N_p(f) \geq a$，从而完成证明。

#### 推论{#int-iv-s6-n5-cor-1 .statement tag=08XU}

— *如果* $r, s, p$ *是三个数这样*

$$
1 \leq r < p < s \leq +\infty,
$$

*然后交* $\mathscr{L}_F^r \cap \mathscr{L}_F^s$ *包含在* $\mathscr{L}_F^p$中。

注一般来说，$\mathscr{L}_F^p$ ($r < p < s$) 的拓扑在交 $\mathscr{L}_F^r \cap \mathscr{L}_F^s$ 上引发的拓扑是*不同的*。如果在$\mu$上不再进行假设，$\mathscr{L}_F^r$和$\mathscr{L}_F^s$在$\mathscr{L}_F^r \cap \mathscr{L}_F^s$上导出的拓扑通常是不可比较的（在其他字中，比率$N_r(f)/N_s(f)$可以取任意大的值和任意小的值） $\mathscr{L}_F^r \cap \mathscr{L}_F^s$；cf. 8）。

当 $\mu$ 是有界测度时，命题 4 可以被锐化：

#### 命题 5 {#int-iv-s6-prop-5 .statement tag=08XV}

— 令 $\mu$ 为有界测度，并令 $f$ 为 $\mu$ 可测函数，且值位于 Banach 空间 $F$ 中。 数 $p$的集合I，使得$1 \leq p \leq +\infty$和$N_p(f)$是有限的，或者是空的或者是左端点$p = 1$和包含这个点的区间；而且，$(|\mu|(X))^{-1/p} N_p(f)$是I上$p$的递增函数。

这是上述第 4 条和 Cor. 的直接的推论。第 4 章的提案 4 I，No. 3。

#### 推论{#int-iv-s6-n5-cor-2 .statement tag=08XW}

— 如果测度 $\mu$ 有界，关系 $r < s$ 意味着 $\mathscr{L}_F^s \subset \mathscr{L}_F^r$；此外，阶$s$的均值收敛性拓扑比阶$r$的均值收敛性拓扑（在$\mathscr{L}_F^s$上）更细大。

可以证明，一般来说，以阶 $s$ 为平均值的收敛性拓扑严格地为更细为以阶 $r$ 为平均值的收敛性拓扑（例 8）。

#### 命题 6 {#int-iv-s6-prop-6 .statement tag=08XX}

— 令 $X$ 为离散的空间，$\mu$ 为 $X$ 上的度量，通过在 $X$ 的每个点放置质量 $+1$ 来定义。如果 $f$ 是 $X$ 的映射到 Banach 空间 $F$、数 $p$ 的集合 I，使得 $1 \leq p \leq +\infty$ 和 $N_p(f)$ 是有限，要么是空的，要么是右端点$+\infty$和包含这个点的区间；此外，$N_p(f)$是I上$p$的递减函数。

对于每个函数$f$（§ 1, No. 1，例）和$N_\infty(f) = \|f\| = \sup_{x \in X} |f(x)|$，$\mu^*(|f|) = \sum_{x \in X} |f(x)|$；如果存在数 $\alpha > 0$，使得$|f(x)| \geq \alpha$对于$x \in X$的无限多个值，则$N_p(f) = +\infty$对于每个有限的$p$；相反的情况下，存在$x_0 \in X$使得$|f(x_0)| = \|f\|$，从而

$$
N_\infty(f) = |f(x_0)| \leq N_p(f)
$$

对于每个有限的$p$。由于函数$\log N_p(f)$相对于$1/p$是凸的，并且在点$+\infty$处取最小的值，因此必然是$p$的递减函数 I（FRV，I, § 4, No. 3，第 5 号提案），完成证明。

#### 推论{#int-iv-s6-n5-cor-3 .statement tag=08XY}

— 如果 $X$ 是离散的，并且度量 $\mu$ 由 $X$ 的每个点处的质量 $+1$ 定义，则关系 $r < s$ 意味着$\mathscr{L}_F^r \subset \mathscr{L}_F^s$；此外，阶 $r$ 的平均值收敛性拓扑比阶 $s$ 的平均值收敛性拓扑更细（在$\mathscr{L}_F^r$ 上）。

### 习题 {#int-iv-s6-exercises}

请参阅 § 6](exercises/s6/) 的 [习题。
