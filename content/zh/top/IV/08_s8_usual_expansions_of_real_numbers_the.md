---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 8
section_title: Usual expansions of real numbers; the power of R
lang: zh
source: top-i-iv
book_pages: 373-377
pdf_pages: 0379-0383, 0407-0411
extraction: ocr
subsections:
    - "no": 1
      title: APPROXIMATIONS TO A REAL NUMBER
      page: 373
      pdf_page: 379
    - "no": 2
      title: EXPANSIONS OF REAL NUMBERS RELATIVE TO A BASE SEQUENCE
      page: 373
      pdf_page: 379
    - "no": 3
      title: DEFINITION OF A REAL NUMBER BY MEANS OF ITS EXPANSION
      page: 374
      pdf_page: 380
    - "no": 4
      title: COMPARISON OF EXPANSIONS
      page: 376
      pdf_page: 382
    - "no": 5
      title: EXPANSIONS TO BASE A
      page: 376
      pdf_page: 382
    - "no": 6
      title: THE POWER OF R
      page: 377
      pdf_page: 383
statements: 3
exercises: 17
content_sha256: c89964a8b80d456d223f494c5591faedbf56053baea7ad7051e749c823da83f5
translated_from: content/en/top/IV/08_s8_usual_expansions_of_real_numbers_the.md
translation_method: google
source_content_sha256: fc201404a7a205db6f15d21fa9d01ef19669eb40041bcaa87ccd2d1c2e452490
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 5b28cb82d7716a6e713d3a5a8a4205eb1a02ced188d99e10ed66ca6ed2a478f1
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 8. 通常展开的实数； R 的幂

### 1. 实数的近似值

#### 定义 1 {#top-iv-s8-def-1 .statement tag=0BUG}

Given a number $\varepsilon > 0$, a real number $r$ is said to be an approximation to within $\varepsilon$ to a real number $x$, if $|x - r| \leq \varepsilon$; $r$ is said to be an approximation by defect if $r \leq x$, by excess if $r \geq x$.

令$A$为$\mathbf{R}$的稠密子集。对于每个$x \in \mathbf{R}$和每个$\varepsilon > 0$，从缺陷（或过量）到$x$到$\varepsilon$属于到$A$之间都有一个近似值，因为间隔$]x - \varepsilon, x[$（或$]x, x + \varepsilon[$）包含至少有一个点 $A$。如果我们现在考虑给定的严格递减序列 $(\varepsilon_n)$ 的数 $> 0$，趋向于 0，并且如果 $r_n$ 是 $x$ 在 $\varepsilon_n$ 内的近似值，则序列 $(r_n)$ 有$x$、极限、$n$趋于无穷大。

In the case where $A$ is a subgroup of the additive group $\mathbf{R}$, and we restrict the $\varepsilon_n$ to belong to $A$, we can define canonically for each $x \in \mathbf{R}$ a sequence $(r_n)$ of approximations to $x$ by defect, belonging to $A$.

根据阿基米德公理 (§ 2, no. 1, 定理 1)，整数 $p$ 的集合使得 $p \varepsilon_n \leq x$ 有最大元素 $p_n$；在其他字中，有一个独特的整数$p_n$使得

$$
p_n \varepsilon_n \leq x < (p_n + 1) \varepsilon_n.
$$

从 $|x - p_n \varepsilon_n| \leq \varepsilon_n$ 开始，$p_n \varepsilon_n$ 是$x$ 的近似值，通过缺陷在 $\varepsilon_n$ 范围内，以及属于通过假设到 $A$ 的近似值；同样，$(p_n + 1) \varepsilon_n$ 是$x$ 到$\varepsilon_n$ 的近似值，属于到$A$，并且两个序列、$(p_n \varepsilon_n)$ 和$((p_n + 1) \varepsilon_n)$ 将$x$ 作为其极限。

### 2. 实数的展开相对于基序列

我们将极限自己研究$\varepsilon_n = 1/d_n$的情况，其中$(d_n)$是整数的严格递增的序列，使得$d_0 = 1$和$d_n$对于$n \geq 1$来说是$d_{n-1}$的倍数。令 $a_n = d_n / d_{n-1}$ ($n \geq 1$): $a_n$ 为整数 $> 1$。在这种情况下，缺陷$r_n = p_n / d_n$的近似值序列是递增，因为$p_n$是最大的整数，使得$p_n / d_n \leq x$；但我们有

$$
\frac{p_{n-1}}{d_{n-1}} = \frac{p_{n-1} a_n}{d_n} \leq x < \frac{p_{n-1} + 1}{d_{n-1}} = \frac{p_{n-1} a_n + a_n}{d_n}
$$

这样$a_n p_{n-1} \leq p_n < a_n p_{n-1} + a_n$，因此$r_{n-1} \leq r_n \leq x$。让
$$
p_n = a_n p_{n-1} + u_n;
$$
那么$0 \leq u_n - a_n$，相当于$0 \leq u_n \leq a_n - 1$，因为$u_n$是整数。因此
$$
r_n = r_{n-1} + \frac{u_n}{d_n} = p_0 + \sum_{k=1}^n \frac{u_k}{d_k},
$$
并且，从$x = \lim_{n \to \infty} r_n$开始，
$$
x = p_0 + \sum_{n=1}^\infty \frac{u_n}{d_n}.
$$
(4)右边的级数，其和为$x$，相对于基序列$(d_n)$，称为$x$的展开。所有系数$u_n$均为$\geq 0$； $p_0$除以定义，最大的整数$p$使得$p \leq x$；它被称为$x$的积分部分，通常用$[x]$表示。

### 3. 定义实数通过其展开

相反，假设我们给出了整数的整数 $q_0$ 和序列 $(v_n)$ ($n \geq 1$)，使得 $0 \leq v_n \leq a_n - 1$；我们问是否存在数 $x$，其展开 (4) 对于所有 $n$ 都满足 $p_0 = q_0$ 和 $u_n = v_n$。如果这样的数存在，那么它是唯一的，因为它等于
$$
q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}.
$$
对于每个整数$m > 0$，我们有（通过比较原理）
$$
\sum_{n=m+1}^\infty \frac{v_n}{d_n} \leq \sum_{n=m+1}^\infty \frac{a_n - 1}{d_n} = \sum_{n=m+1}^\infty \left( \frac{1}{d_{n-1}} - \frac{1}{d_n} \right) = \frac{1}{d_m}
$$
仅当每个$n > m$（§ 7, no. 1，定理 2）都有$v_n = a_n - 1$时，最左边和最右边的项才相等。因此级数其通项是$\frac{v_n}{d_n}$是收敛的；此外，如果$x = q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}$，我们有
$$
s_m = q_0 + \sum_{n=1}^m \frac{v_n}{d_n} \leq x \leq s_m + \frac{1}{d_m}
$$
并且仅当每个 $n > m$ 都有 $v_n = a_n - 1$ 时，$x = s_m + \frac{1}{d_m}$。由于$s_m$是分母为$d_m$的分数，因此通过缺陷将$r_m$到$x$在$1/d_m$内的近似值等于$s_m$或$s_m + \frac{1}{d_m}$；而后一种选择仅当 $v_n = a_n - 1$ 对于所有 $n > m$ 时才会发生。因此：
(i) $n$ 的值存在“无穷大”，使得 $v_n < a_n - 1$：则级数 $q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$ 与其和 $x$ 的展开相同。
(ii) 存在整数 $m \geq 0$，每当 $n > m$ 时，$v_n = a_n - 1$，以及 $v_m < a_m - 1$（如果 $m > 0$）；那么级数 $q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$ 的和 $x$ 等于有理数数
$$
q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \frac{1}{d_m}
$$
其中形式$k/d_m$（$k$整数）； $x$的*展开*与级数(5)相同，其中所有项和指标$> m$都是零；这样的展开被称为*终止*，或*终止*。 级数
$$
q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} = q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \sum_{n=m+1}^{\infty} \frac{a_n - 1}{d_n}
$$
被称为数$x$的*不正确的展开*。

相反，令$x$为有理数数，对于$n$的某些值，可以将其写成分母为$d_n$的分数的形式。令 $m$ 为最小的整数，使得 $x$ 为形式 $k/d_m$ ($k$ 整数)；我们对$n < m$和$r_m = x$有$r_n < x$，因此$x$的展开是形式（5），并且$x$有一个由（6）给出的不正确的展开；此外，这个不正确的展开是*独特的*。

有理数数，用不可约形式 $p/q$ 写成，等于分母为 $d_n$ 的分数当且仅当 $q$ *除* $d_n$（数 $m$ 因此将是最小的整数$n$使得$q$除$d_n$）。可能会发生*每个有理数*都有这个性质（对于适当选择的$n$）：当且仅当每个整数$> 0$除一些$d_n$，例如，如果$d_n = n!$如果$d_n$有这个性质，那么数是有理数当且仅当它的展开相对于序列$(d_n)$终止。

总结一下：对于每个序列$s$，其初始项$q_0$是任意整数，并且其项$v_n (n \geq 1)$使得$0 \leq v_n \leq a_n - 1$，对应实数等于$q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$；如果 $I_n$ 表示 $\mathbf{N}$ 的区间 $[0, a_n - 1]$，则我们将 $X = \mathbf{Z} \times \prod_{n=1}^{\infty} I_n$ 的定义映射 $\varphi$ *onto* 实直线 $\mathbf{R}$；此外，如果$x$不是分母为$d_n$的分数（对于某些$n$），则方程$\varphi(s) = x$（其中给定$x \in \mathbf{R}$）有*一*解，否则有*二*解。

### 4. 展开比较

如果我们知道两个不同的实数、$x$和$y$的展开，我们就可以确定，无论是$x < y$还是$x > y$。

设$x = p_0 + \sum_{n=1}^{\infty} u_n / d_n$、$y = q_0 + \sum_{n=1}^{\infty} v_n / d_n$为$x$和$y$中的展开。如果 $p_0 < q_0$ 那么 $x < y$，因为

$$
p_0 \leq x < p_0 + 1 \leq q_0 \leq y.
$$

更一般地，假设 $p_0 = q_0$ 和 $u_n = v_n$ 对应 $1 \leq n \leq m$，但$u_m < v_m$；如果

$$
r_n = p_0 + \sum_{k=1}^{n} u_k / d_k, \quad s_n = q_0 + \sum_{k=1}^{n} v_k / d_k,
$$

然后$r_n = s_n$代表$n < m$，从$u_m + 1 \leq v_m$开始，$r_m + \frac{1}{d_m} \leq s_m$；但是$r_m \leq x < r_m + \frac{1}{d_m} \leq s_m \leq y$，因此我们又得到了$x < y$。在其他字中，$x$和$y$的*阶与它们各自的展开*的前两个不同的项的阶相同。

由此可见，如果$p_0 = q_0$和$u_n = v_n$对于$n < m$，则到端点为$x$和$y$的闭区间的每个数$z$属于的展开的第一个$m$项为与$x$和$y$的展开*相同*。

我们还注，在这种情况下，我们有$|y - x| \leq \frac{1}{d_{m-1}}$。如果我们赋予$\mathbf{Z}$和间隔$I_n$*离散*拓扑，那么上面定义的映射$\varphi$是*乘积空间*$X$上的*连续*。

### 5. 展开至基 A

最重要的基序列是$d_n = a^n$，其中$a$ 是整数 $> 1$； $a$ 则被称为相应的展开的 *基数*（或简称为 *基*）。对于数值计算，使用展开到基10，称为*十进制展开*；还经常使用展开至基2（*二元*展开）和基3（*三元*展开）。

为了表示缺陷$r_n$至数$x \geq 0$的近似值，在其展开至基$a$中，采用以下符号：每个整数$u$使得$0 \leq u \leq a - 1$由特定符号表示；如果

$$
r_n = p_0 + \sum_{k=1}^{n} \frac{u_k}{d_k},
$$

我们首先借助这些符号记下整数$p_0 = [x] \geq 0$的表示到基$a$（*集合理论*，章III, § 5, no. 7），然后我们把点（“十进制”） 点”），我们依次写出代表数$u_1, u_2, \ldots, u_n$的符号。如果S是由此获得的符号，则习惯上写为$x = S...$，这是滥用语言。应该一劳永逸地理解，这样的关系只是方法的缩写，表示右边是缺陷到$1/a^n$以内的对$x$的近似。

对于负数数，既定用法有所不同：我们在上述符号体系中写出$x' = -x > 0$的近似值，并在其前面加上符号“—”；因此，它是 $x$ 的近似值，在 $1/a^n$ 内，超出了如此表示的值。

这种用法对于数值计算有其不便。在记号中，负对数采用与正数相同的符号，通过在积分部分上放置一条横线，表示它等于所写的数的负数。

### 6. R 的幂

我们有 $\mathbf{R} = \bigcup_{n \in \mathbf{Z}} [n, n+1[$，所有区间 $[n, n+1[$ 都等价于 $[0, 1[$。由于 $[0, 1[$ 是无限集合，因此 $\mathbf{R}$ 等价于区间 $[0, 1[$。通过考虑区间$[0, 1[$的数的二进展开，我们将证明该区间等价于所有序列$(u_n)$的集合S，其中每个项等于0或1。

首先，它与序列 $(u_n)$ 的 S 由……组成的子集 $S'$ 等价，使得 $u_n = 0$ 对于值 $n$ 的无穷大。另一方面，S 中$S'$的补$S''$等价于有理数的所有假展开的集合，它们等于分母$2^n$的分数； $\mathbf{Q}$的这些数形式子集，因此其中集合是可数的，因此$S''$也是可数的。由于 $S'$ 是无穷大，因此它与 S 等价，因此得出结果。

现在S等价于$\mathfrak{P}(\mathbf{N})$；因为我们可以将$\mathfrak{P}(\mathbf{N})$的定义双射通过映射到$\mathbf{N}$的每个子集A到序列$(u_n)$，使得$u_n = 0$如果$n \in A$并且$u_n = 1$ 如果$n \notin CA$。由此我们证明了：

#### 定理 1（康托尔）{#top-iv-s8-thm-1 .statement tag=0BUH}

*实数中的集合等价于可数无限集合中所有子集中的集合。*

#### 推论 {#top-iv-s8-n6-cor-1 .statement tag=0BUI}

*实数的集合的基数严格大于可数集合的基数。*

集合等价于 $\mathbf{R}$ 据说有幂的连续统。通过§ 4, no. 1的命题 1，包含多于一个点的每个区间都有幂的连续统。同样，$\mathbf{R}$的可数子集的补集尤其具有连续统的幂，所有无理数数的*集合具有连续统*的幂。

### 习题{#top-iv-s8-exercises}

参见[习题为 § 8](exercises/s8/)。
