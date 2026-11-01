---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 0
section_title: Infinite products in normed algebras
appendix: true
lang: zh
source: top-v-x
book_pages: 268-270
pdf_pages: 0217-0223, 0274-0276
extraction: ocr
subsections:
    - "no": 1
      title: MULTIPLIABLE SEQUENCES IN A NORMED ALGEBRA
      page: 0
      pdf_page: 217
    - "no": 2
      title: MULTIPLIABILITY CRITERIA
      page: 0
      pdf_page: 218
    - "no": 3
      title: INFINITE PRODUCTS
      page: 0
      pdf_page: 221
statements: 16
exercises: 8
content_sha256: 6a0b9a080bf5085dd0c5524a29c5efc33da4952c859669286b2deb10e2c4f7f7
translated_from: content/en/top/IX/A_a_infinite_products_in_normed_algebras.md
translation_method: google
source_content_sha256: 4891adafb991bbb34168be7fb8caef2435567acb2d9b3db3045a912f02678465
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 54832ef30141cb7824920e1b825571990fc62528c3969636325cc476e317c1f7
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 附录

# 无限乘积标准代数

### 1. 在范数代数中可乘序列

令 $A$ 为非离散值域 $K$ 上的规范代数 (章 IX, § 3, no. 7, 定义 9)；我们用元素$x \in A$的$||x||$范数来表示，并且我们假设这个范数满足不等式$||xy|| \leq ||x|| \cdot ||y||$；我们还假设$A$有单位元素$e$。

令$(x_n)_{n \in \mathbf{N}}$为$A$的点的无限序列。 $\mathbf{N}$的每有限子集$J$，按$\mathbf{N}$、$A$的点的定义序列$(x_n)_{n \in J}$的顺序线性排序，我们定义乘积

$$
p_J = \prod_{n \in J} x_n
$$

其中序列；这个乘积被称为序列$(x_n)_{n \in \mathbf{N}}$的有限部分乘积，相应的到$\mathbf{N}$的有限子集$J$（回想一下，如果$J = \varnothing$我们放入$\prod_{n \in \varnothing} x_n = e$）。

#### 定义 1 {#top-ix-a0-def-1 .statement tag=0CA3}

*序列* $(x_n)_{n \in \mathbf{N}}$ *据说在范数代数* $A$ *如果映射* $J \to p_J$ *相对于集合*的截面的过滤器有极限 $\mathfrak{F}(\mathbf{N})$ *共有限子集共* $\mathbf{N}$，*按关系* $\subset$ 排序； *这个极限称为序列*$(x_n)_{n \in \mathbf{N}}$的乘积，*并表示为*$\prod_{n \in \mathbf{N}} x_n$*（或简称为*$\prod_n x_n$）； *这个乘积的*$x_n$*被称为因子。*

定义 1 等价于： *序列* $(x_n)$ *可乘，其乘积为* $p$ *如果对于每个* $\varepsilon > 0$ *存在有限子集* $J_0$ *of* $\mathbf{N}$ *这样对于每一个有限子集* $J \supset J_0$ *of* $\mathbf{N}$，*我们有* $||p_J - p|| \leq \varepsilon$。

#### 注 1 {#top-ix-a0-n1-rem-1 .statement tag=0CA4}

当$A$为交换代数时，定义1与章III, § 5, no. 1、注3相同；但当$A$不可交换时，指标集合$\mathbf{N}$的阶结构本质上参与定义1。如果$\sigma$是置换的任意置换 $\mathbf{N}$，我们不能一般断言，如果序列(x_n)是可乘的，则序列$(x_{\sigma(n)})$是可乘的；如果两个序列都是可乘的，那么它们的乘积通常会不同。

#### 注 2 {#top-ix-a0-n1-rem-2 .statement tag=0CA5}

定义 1 可以立即推广到一个族 (x_n)_{n \in I} 的情况，其指标集合 I 是 \mathbf{Z} 的子集（由阶线性排序） \mathbf{Z})。我们将扩展留给读者，在这种情况下，结果如下（cf.习题1和2）。

### 2.多重性判据

从现在开始，我们假设规范的代数 A 是完备的。

#### 定理 1 {#top-ix-a0-thm-1 .statement tag=0CA6}

令 (x_n)_{n \in \mathbf{N}} 为完全范数代数 A 中的点的序列。
a) 如果 (x_n) 是可乘的，且其乘积是 A 的单位，则对于每个$\varepsilon > 0$，存在 \mathbf{N} 的有限子集 J_0，这样，对于 \mathbf{N} 的每个不满足 J_0 的有限子集 L，我们有$\|e - p_L\| \leq \varepsilon$。
b) 相反，如果序列 (x_n) 满足条件，则它是可乘的。此外，如果每个x_n是单位，那么$\prod_{n \in \mathbf{N}} x_n$就是单位。

a) 令p为可乘数序列(x_n)的乘积，并假设p在A中为单位；那么 (章 IX, § 3, no. 7, 命题 13) 存在 $\alpha > 0$ 和 $a > 0$，这样，对于我们有的所有 $y \in A$
$$
\|y - p\| \leq \alpha,
$$
y 为单位和 $\|y^{-1}\| \leq a$。到假设，对于每个$\varepsilon$使得$0 < \varepsilon < \alpha$，有\mathbf{N}的有限子集H_0，这样，对于\mathbf{N}包含H_0的每个有限子集H，我们有$\|p_H - p\| \leq \varepsilon$。令 $J_0 = [0, m]$ 为 \mathbf{N} 的区间，其中包含 H_0；对于\mathbf{N}中每一个不满足J_0的有限子集L，整数属于到L都大于属于到H_0；因而，如果$H = H_0 \cup L$，我们有$p_H = p_{H_0} p_L$。现在，由于$\|p_{H_0} - p\| \leq \varepsilon \leq \alpha$，$p_{H_0}$是单位，并且
$$
\|e - p_{H_0}^{-1} p\| \leq \varepsilon \|p_{H_0}^{-1} p\| \leq a \varepsilon;
$$
从$\|p_{H_0} p_L - p\| \leq \varepsilon$开始，我们推断
$$
\|p_L - p_{H_0}^{-1} p\| \leq \varepsilon \|p_{H_0}^{-1}\| \leq a \varepsilon,
$$
最后$\|e - p_L\| \leq 2a \varepsilon$。

b) 假设对于每个$\varepsilon > 0$，\mathbf{N} 都存在有限子集 J_0，这样，对于\mathbf{N} 的每个不满足J_0 的有限子集 L，我们有$\|e - p_L\| \leq \varepsilon$。令 $H_0 = [0, p]$ 为 \mathbf{N} 的区间，其中包含 J_0；那么\mathbf{N}中的每一个有限子集 H，其中包含 H_0都可以写成形式$H_0 \cup L$，其中L中的整数都大于H_0中的整数；因此我们有$p_H = p_{H_0} p_L$，并且由于L不满足$J_0$、$\|p_H - p_{H_0}\| \leq \varepsilon \|p_{H_0}\|$，因此不满足$\|p_H\| = (1 + \varepsilon)\|p_{H_0}\|$。若$p_{H_0} = 0$、序列$(x_n)$明显可乘且乘积为0；除了这个简单的情况，还有一个区间 $H_1 = [0, q]$ 包含 $H_0$，这样，对于 $\mathbf{N}$ 的每一个有限子集 $L$ 不满足 $H_1$，我们就有 $\|e - p_L\| \leq \varepsilon (\|p_{H_0}\|)^{-1}$。如上所述，对于每个有限子集 $H \supset H_1$，

$$
\|p_H - p_{H_1}\| \leq (\|p_{H_0}\|)^{-1}\|p_{H_1}\|\varepsilon \leq \varepsilon (1 + \varepsilon).
$$

因而，柯西准则表明，相对于有向集合 $\mathfrak{F}(\mathbf{N})$，$J \to p_J$ 在 $A$ 中具有极限。

如果所有的$x_n$都是单位，那么所有的有限部分积$p_J$也是；因此对于每个有限子集 $H$ 包含 $H_0$ 我们有

$$
\|e - p_{H_0}^{-1}p_H\| \leq \varepsilon,
$$

这表明，在$A$的单位的乘法群$G$中，$\mathfrak{F}(\mathbf{N})$的截面滤波器的映射$J \to p_J$下的像相对于左均匀性是柯西滤波器基 $G$；但由于$G$是*完整的*（章IX, § 3, no. 7，命题13），极限映射$J \to p_J$属于到$G$。

#### 注 {#top-ix-a0-n2-rem-1 .statement tag=0CA7}

如果$(x_n)$是可乘的且乘积不是单位，定理1的条件不一定满足：对于例，如果所有$x_n$都等于相同的元素$x$，其中$\|x\| < 1$， 序列$(x_n)$是可乘的，其乘积为0，对于$\mathbf{N}$的每个非空有限子集$H$，我们有$\|p_H\| \leq \|x\| < 1 \leq \|e\|$。

#### 推出 1 {#top-ix-a0-thm-1-cor-1 .statement tag=0CA8}

*如果*$(x_n)$*是一个可乘的序列，其乘积是*$A$的单位，*则*$\lim_{n \to \infty} x_n = e$。

#### 推论 2 {#top-ix-a0-thm-1-cor-2 .statement tag=0CA9}

*如果* $(x_n)$ *是一个可乘的序列，其乘积是* $A$的单位，*则每个子序列* $(x_{n_k})_{k \in \mathbf{N}}$ *of* $(x_n)$ *[$(n_k)$是严格递增的序列 of 整数]* *可乘*。

这直接遵循定理 1 的标准。

#### 定理 2 {#top-ix-a0-thm-2 .statement tag=0CAA}

*让*$A$*成为一个完全规范的代数*。 *如果*$(u_n)$*是*$A$的元素的绝对收敛级数，*则序列*$(e + u_n)$*可乘于*$A$； *如果所有元素* $e + u_n$ *都是单位在* $A$，*那么也是* $\prod_{n \in \mathbf{N}} (e + u_n)$。

让我们应用定理1的标准。对于$\mathbf{N}$的每个有限子集$L$，我们有$p_L - e = \prod_{n \in L} (e + u_n) - e = \sum_M \left( \prod_{n \in M} u_n \right)$，其中$M$贯穿$L$的所有非空子集的集合（通过诱导的线性排序）订购）。从$\prod_{n \in M} u_n \leq \prod_{n \in M} |u_n|$开始，我们可以写

$$
||p_1 - e|| = \sum_M (\prod_{n \in M} u_n) \cdot \prod_{i \in I} (1 + |u_i|) - 1.
$$

现在，由于级数（其通项为$|u_n|$）收敛于假设，序列$1 - |u_n|$可乘于$\mathbf{R}_+^*$（章IV, § 7, no. 4，定理4）。因此，对于每个$\varepsilon > 0$，都存在$\mathbf{N}$的有限子集$J_0$，这样，对于不满足$J_0$的$\mathbf{N}$的每个有限子集$L$，我们有$\left| \prod_{n \in L} (1 + ||u_n||) - 1 \right| \leq \varepsilon$；因此结果。

#### 推论{#top-ix-a0-n2-cor-1 .statement tag=0CAB}

*如果级数的通项为$u_n$是绝对收敛的，并且如果在$A$中元素$e - u_n$都不为零因子，则乘积$\prod_{n \in \mathbf{N}} (e + u_n)$在零因子中不是零因子 $A$.*

只有整数 $n$ 的有限数使得 $|u_n| > 1$。令$J = [a, m]$为$\mathbf{N}$包含所有这些整数的区间。 序列$(e + u_n)$的乘积是$p_J$和元素$\prod_{n \notin J} (e - u_n)$的乘积，所有因子都是单位（章IX, § 3, no. 7， 命题 12) 的推论，因此本身就是单位；由于$p_J$是有限非零除数数的乘积，因此它不是零因子，因此$\prod_{n \in \mathbf{N}} (e + u_n)$不是零因子。

定理 2 给出的足够的条件乘法性一般来说是不必要的 (cf. 习题 6)。然而，在重要情况下，$A$是有限秩的代数超过域$\mathbf{R}$（即$A$是有限维的，向量空间超过$\mathbf{R}$）；特别是如果 $A$ 是四元数 $\mathbf{H}$ 的除法环，或矩阵代数 $\mathbf{M}_n(\mathbf{R})$：

#### 命题 1 {#top-ix-a0-prop-1 .statement tag=0CAC}

*令$A$为有限秩超过$\mathbf{R}$的标准化代数。如果$(e + u_n)$是$A$中的可乘序列，其乘积是$A$的单位，则级数其一般项是$u_n$是绝对收敛的。*

从章VII, § 3, no. 1，命题2，存在数$c > 0$，这样，对于$A$的点的每个有限族$(x_i)_{i \in I}$，我们有

$$
\sum_{i \in I} \|x_i\| \leq c \sup_{J \subset I} \left| \sum_{i \in J} x_i \right|.
$$

令$(a_i)_{i \in \mathbf{N}}$为$A$的元素的任意序列。对于 $\mathbf{N}$ 中的每个有限子集 $I$，将

$$
p_I = \prod_{i \in I} (e + a_i), \quad s_I = \sum_{i \in I} a_i, \quad \sigma_I = \sum_{i \in I} \|a_i\|.
$$

#### 引理 1 {#top-ix-a0-lem-1 .statement tag=0CAD}

对于$\mathbf{N}$中的每个有限子集$I$，令$\varphi(I) = \sup_{J \subset I} ||p_J - e||$。 Then for each 子集 $J$ of $I$ we have

$$
||p_J - e - s_J|| \leq \varphi(I)\sigma_J.
$$

如果$J$为空，引理是明显的；我们将通过$J$中元素的数上的归纳来证明。设$J = K \cup \{j\}$，其中$\{j\}$严格大于每个$i \in K$。然后 $p_J = p_K(e + a_j)$ 和

$$
s_J = s_K + a_j,
$$

以便

$$
p_J - e - s_J = p_K - e - s_K + (p_K - e)a_j,
$$

通过 $\varphi(I)$ 的归纳假设和定义，我们有

$$
||p_J - e - s_J|| \leq \varphi(I)\sigma_K + \varphi(I)||a_j|| = \varphi(I)\sigma_J,
$$

这就证明了引理。

#### 引理 2 {#top-ix-a0-lem-2 .statement tag=0CAE}

如果$I$是$\mathbf{N}$的有限子集使得$\varphi(I) < 1/c$，那么

$$
\sigma_I \leq c\varphi(I)/(1 - c\varphi(I)).
$$

因为从$\sigma_J \leq \sigma_I$开始，对于$I$的每个子集$J$，我们有（2）

$$
||s_J|| \leq \varphi(I)\sigma_I + ||p_J - e|| \leq (1 + \sigma_I)\varphi(I);
$$

并且由于 $\sigma_I \leq c \cdot \sup_{J \subset I} ||s_J||$，由 (1) 可知

$$
\sigma_I \leq c\varphi(I)(1 + \sigma_I),
$$

这导致了结果。

现在令$(e + u_n)$为$A$中的可乘序列，其乘积为单位；通过定理 1，存在$\mathbf{N}$的有限子集$J_0$，这样，对于$\mathbf{N}$的每个有限子集$H$不满足$J_0$，我们有

$$
\left| \prod_{i \in H} (e + u_i) - e \right| \leq 1/2c.
$$

By Lemma 2, it follows that $\sum_{i \in H} ||u_i|| - 1$ for every finite subset $H$ of $\mathbf{N}$ which does not meet $J_0$, and hence (Chapter IV, § 7, no. 1, Theorem 1) the family $(||u_n||)$ is summable in $\mathbf{R}$.

### 3.无限乘积

对于规范化的代数$A$中点的每个序列$(x_n)$，让我们制作*部分积*$p_n = \prod_{k=0}^n x_k$的对应序列；则序列$(x_n)$和$(p_n)$的*右*称为无穷乘积，其通因子为$x_n$。如果序列 $(p_n)$ 收敛于 $A$，则无限乘积与一般因子 $x_n$ 收敛；这个序列的极限被称为序列$(x_n)$的乘积，并用$\prod_{n=0}^\infty x_n$表示。

#### 命题 2 {#top-ix-a0-prop-2 .statement tag=0CAF}

*令* $(x_n)$ *成为完整规范的代数* $A$中点的序列。

a) *如果无限乘积其一般因子是* $x_n$ *收敛，并且如果* $\prod_{n=0}^\infty x_n$ *是单位在* $A$，*则对于每个* $\varepsilon > 0$ *存在整数* $n_0$ *这样*
$$
\left\| \prod_{k=m}^n x_k - e \right\| \leq \varepsilon
$$
*每当*$n_0 \leq m \leq n$。

b) *反之，如果序列* $(x_n)$ *满足这个条件，则无限乘积与一般因子* $x_n$ *收敛；如果*$A$中的每个*$x_n$*是单位，*那么*$\prod_{n=0}^\infty x_n$*是单位*。

这个命题的证明一步步跟随着定理1的证明，留给读者（定理1的证明中的$N$的有限子集$L$要间隔替换）。

#### 推论 1 {#top-ix-a0-prop-2-cor-1 .statement tag=0CAG}

*如果无限乘积与一般因子* $x_n$ *收敛，并且如果* $\prod_{n=0}^\infty x_n$ *是单位*，*则* $\lim_{n \to \infty} x_n = e$。

#### 推论 2 {#top-ix-a0-prop-2-cor-2 .statement tag=0CAH}

*如果无穷大乘积与一般因子* $x_n$ *收敛，并且如果* $\prod_{n=0}^\infty x_n$ *是单位*，*则无穷大乘积与一般因子*
$$
y_n = x_{n+h} \quad (n \geq 0)
$$
*收敛*。

序列$(y_n)$的乘积用$\prod_{n=h}^\infty x_n$表示，与一般的因子$x_n$也称为无限乘积的指标$h$的剩余类。

仍然在假设下，$\prod_{n=h}^\infty x_n$是单位，从命题2得出，如果$(z_n)$是序列，使得$z_n = x_n$除了指标的有限数之外，那么乘积与一般的因子 $z_n$ 收敛。

#### 命题 3 {#top-ix-a0-prop-3 .statement tag=0CAI}

*设*$(k_n)$*为整数*$\geq 0$的严格递增的序列，*使得*$k_0 = 0$； *如果无限乘积与一般因子* $x_n$ *收敛*，*并且*如果我们把

$$
u_n = \prod_{p=k_n}^{k_{n+1}-1} x_p,
$$

那么广义因子为 $u_n$ 的无限乘积是收敛的，我们有

$$
\prod_{n=0}^{\infty} u_n = \prod_{n=0}^{\infty} x_n.
$$

对于序列$(u_n)$的部分积的序列是序列$(x_n)$的部分积的序列的子序列。

最后，与用于阿贝尔的群 (章 III, § 5, no. 7) 的相同论点表明，如果规范化代数 $\mathbf{A}$ 中的序列 $(x_n)$ 是*可乘的*，则乘积的一般因子是 $x_n$是收敛的，并且

$$
\prod_{n=0}^{\infty} x_n = \prod_{n \in \mathbf{N}} x_n
$$

（也写为$\prod_{n=0}^{\infty} x_n$）； 逆命题当然不正确（cf. 习题 7）。

### 习题{#top-ix-a0-exercises}

请参见附录 0](exercises/a0/) 的 [习题。
