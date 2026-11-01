---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 2
section_title: Summable families of positive measures
lang: zh
source: int-i-vi
book_pages: INT V.95-INT V.96
pdf_pages: 0266-0270, 0350-0351
extraction: ocr
subsections:
    - "no": 1
      title: Definition of summable families of measures
      page: 11
      pdf_page: 266
    - "no": 2
      title: Integration with respect to a sum of positive measures
      page: 12
      pdf_page: 267
    - "no": 3
      title: Decomposition of a measure as a sum of measures with compact support
      page: 14
      pdf_page: 269
statements: 12
exercises: 4
content_sha256: 30d2c2ce0f63b49e4fbdcd23e754927300d02bce77ca6bc39a4489de6bedb2dd
translated_from: content/en/int/V/02_s2_summable_families_of_positive_measures.md
translation_method: google
source_content_sha256: ec7d58f4d9ead5ad76e61a986e1e25bc88d93ca5a6598bf0f04e740c0b11cee4
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 675fb60e8175ca5b8c302921a81cea7a7d8f97aaa29b1129dff046bda5d29544
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。积极措施的总结系列

### 1. 可求和测度族的定义

设$(\lambda_\alpha)_{\alpha \in A}$为局部契约空间X上的一系列积极措施；如果$(\lambda_\alpha)_{\alpha \in A}$族可以在X上的实际测度向量空间$\mathscr{M}(X)$中求和，并配备模糊的拓扑（GT，III, §5, No. 1），则称其为*可求和的测度族*。 这相当于说，对于每个函数 $f \in \mathscr{K}(X)$，数 $\lambda_\alpha(f)$ 的族可在 $\mathbf{R}$ 中求和。 因为，这个条件显然是必要的；相反，如果满足，则$\mathscr{K}(X)$上的线性形式$f \mapsto \sum_{\alpha \in A} \lambda_\alpha(f)$为正，因此是正测度$\nu$（第1章） III, §1, No. 5，Th。 1)，并且立即验证族$(\lambda_\alpha)$的有限部分和模糊地收敛到$\nu$，相对于A的有限子集的集合的截面滤波器（GT，III, §5, No. 1，Def.1）。

由于$\mathscr{K}(X)$的每个元素都是$\mathscr{K}_+(X)$的两个元素之差，因此族$(\lambda_\alpha)$可求和当且仅当
$$
\sum_{\alpha \in A} \lambda_\alpha(f) < +\infty
$$

对于每个函数 $f \in \mathscr{K}_+(X)$。这个条件也等价于：

(2)
$$
\sum_{\alpha \in A} \lambda_\alpha(K) < +\infty
$$
对于每个紧集 $K \subset X$。

对于，(2) 蕴涵(1)，因为$f \leq \|f\| \cdot \varphi_S$，其中S 表示$f$ 的紧支持。反之，若K为紧集，则存在函数$f \in \mathscr{K}_+(X)$使得$\varphi_K \leq f$(Ch.III, §1, No. 2，引理1)，因此(1)蕴涵(2)。

#### 注 1 {#int-v-s2-n1-rem-1 .statement tag=090G}

直接的，当族$(\lambda_\alpha)_{\alpha \in A}$可求和时，其和是有限部分和$\sum_{\alpha \in J} \lambda_\alpha$的$\mathscr{M}_+(X)$中的上界，其中J运行于A的有限子集的集合。

#### 注 2 {#int-v-s2-n1-rem-2 .statement tag=090H}

令 $(\theta_\alpha)_{\alpha \in A}$ 为 X 上的一系列复杂测度；如果正测量的族$(|\theta_\alpha|)$是可求和的，则称族$(\theta_\alpha)$是“可求和的”； *为此，族 $(\theta_\alpha)$ 可以在向量空间 $\mathscr{M}(X; \mathbf{C})$ 中求和，并配备模糊拓扑 (cf. Exer. 3)，这还不够*。

### 2. 积极措施和的整合

*在这个No.*中，X表示局部紧凑空间，$(\lambda_\alpha)_{\alpha \in A}$表示X上的正测度的可求和族，$\nu$表示测度$\sum_{\alpha \in A} \lambda_\alpha$。

#### 命题 1 {#int-v-s2-prop-1 .statement tag=090I}

— *令 f 为在 X 上定义的正数值函数。然后*
$$
\nu^\bullet(f) = \sum_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

这是从注 1、§1, No. 3的第11号提案和§1, No. 1的第3号提案得出的。

#### 推论 1 {#int-v-s2-prop-1-cor-1 .statement tag=090J}

— *对于每个紧凑型（分别是开放型和相对紧凑型）子集 M of X，
$$
\nu(M) = \sum_{\alpha \in A} \lambda_\alpha(M).
$$*

#### 推论 2 {#int-v-s2-prop-1-cor-2 .statement tag=090K}

— *为了使 X 的子集 N 局部 $\nu$ 可忽略不计，对于每个 $\alpha \in A$，N 局部 $\lambda_\alpha$ 可忽略不计是充分必要的。*

#### 推论 3 {#int-v-s2-prop-1-cor-3 .statement tag=090L}

— *对于每个函数 $f \in \mathscr{F}_+(X)$，
$$
\nu^*(f) \geq \sum_{\alpha \in A} \lambda_\alpha^*(f).
$$*

如果 $f$ 不是 $\nu$ 调节的，不等式是显而易见的，因为那么 $\nu^*(f) = +\infty$ ($§ 1$, No. 2, 命题 7)。如果$f$是$\nu$-调节的，那么对于每个$\alpha \in A$，$f$是$\lambda_\alpha$-调节的，因为每个$\nu$-可积开集合都是$\lambda_\alpha$-可积； 关系 (4) 则立即从 (3) 和$§ 1$、No. 2 的第 7 条命题得出。

即使$A$是可数的并且每个$\lambda_\alpha$都是点测度（$§ 1$，Exer.4 a）），（4）的两个成员也可能不相等。

#### 命题 2 {#int-v-s2-prop-2 .statement tag=090M}

— *令 $f$ 为 $X$ 的映射成为拓扑空间 $G$。为了使 $f$ $\nu$ 可测量，对于每个 $\alpha \in A$，$f$ $\lambda_\alpha$ 可测量是必要且充分的。*

这是从 Cor 立即得出的结论。 $§ 1$第11号提案第2条。

#### 命题 3 {#int-v-s2-prop-3 .statement tag=090N}

— *为了将 $X$ 的映射 $f$ 转化为 Banach 空间 $F$ 本质上 $\nu$ 可积，$f$ 对于每个$\alpha \in A$ 本质上$\lambda_\alpha$ 可积是必要且充分的，并且*

$$
\sum_{\alpha \in A} \int^\bullet |f| \, d\lambda_\alpha < +\infty .
$$

*家庭$(\int f \, d\lambda_\alpha)_{\alpha \in A}$在$F$中绝对可求和，并且*

$$
\int f \, d\nu = \sum_{\alpha \in A} \int f \, d\lambda_\alpha .
$$

事实上，对于$f$本质上$\nu$可积（或本质上$\lambda_\alpha$可积），$f$对于测量$\nu$（或$\lambda_\alpha$）和$\nu^\bullet(|f|) < +\infty$（或$\lambda_\alpha^\bullet(|f|) < +\infty$）是可测量的，这是必要且充分的，根据命题。 $§ 1$、No. 3 中的 9 个。因此，叙述的第一个部分立即来自Props。 2 和 1. 如果 $f$ 本质上是 $\nu$ 可积，则不等式

$$
\sum_{\alpha \in A} \left| \int f \, d\lambda_\alpha \right| \leq \sum_{\alpha \in A} \int |f| \, d\lambda_\alpha = \nu(|f|)
$$

意味着族$(\int f \, d\lambda_\alpha)$在$F$中绝对可求和，并且和中的范数小于或等于$\mathscr{L}_F^1(\nu)$中$f$的范数。 $f \in \mathscr{L}_F^1(\nu)$的集合，因此满足(6)是$\mathscr{L}_F^1(\nu)$的闭线性子空间$\mathscr{H}$；现在，这个子空间在$\mathscr{L}_F^1(\nu)$中也是稠密的，因为它是形式$f \cdot a$的包含函数，其中$a \in F$和$f$表示有限可积正函数（命题1）。因此$\mathscr{H} = \mathscr{L}_F^1(\nu)$和命题成立。

命题3也可以从积分上的一般定理推导出来，这将在§3（No. 3，Th.1）中证明。

#### 推论 1 {#int-v-s2-prop-3-cor-1 .statement tag=090O}

— 假设$f$是$\nu$可积；那么$f$ 对于每个$\alpha \in A$ 都是$\lambda_\alpha$ 可积的，且公式 (6) 成立。相反，如果集合 $A$ 是有限的，并且 $f$ 对于每个 $\alpha \in A$ 是 $\lambda_\alpha$ 可积，则函数 $f$ 是 $\nu$ 可积。

如果$f$是$\nu$可积，那么$f$本质上是$\nu$可积且$\nu$可调节（§ 1, No. 3，Prop.9的Cor.）；因此，对于每个$\alpha \in A$，$f$本质上是$\lambda_\alpha$可积且$\lambda_\alpha$可调节的，因此$\lambda_\alpha$可积。相反，如果$A$是有限的，并且$f$对于所有$\alpha \in A$来说是$\lambda_\alpha$可积，那么$f$本质上是根据命题3的$\nu$可积，并且足以验证$\nu^*(|f|) < +\infty$；这立即来自关系 $\nu^* = \sum_{\alpha \in A} \lambda_\alpha^*$（第 IV, §1, No. 3 章，第 15 条提案）。

#### 推论 2 {#int-v-s2-prop-3-cor-2 .statement tag=090P}

— 令$\theta$为$X$的复测度； 集合$\theta_1 = (\Re \theta)^+$、$\theta_2 = (\Re \theta)^-$、$\theta_3 = (\Im \theta)^+$、$\theta_4 = (\Im \theta)^-$。在阶中，$X$ 的映射 $f$ 转换为拓扑空间 $G$（分别转换为 Banach 空间 $F$）对于测度 $\theta$ 是可测的（分别是本质上可积、可积），则对于每个测量值 $\theta_i$ ($i = 1, 2, 3, 4$) 来说，它是可测量的（分别是本质上可积的、可积的）是必要且充分的。

If $f$ is measurable (resp. essentially integrable, integrable) for $\theta$, then $f$ is by definition measurable (resp. essentially integrable, integrable) for the measure $|\theta|$, hence also for the measures $\theta_i$, which are $\leq |\theta|$. 相反，如果 $f$ 对于测度 $\theta_i$ 是可测的（分别是本质上可积的、可积的），则命题 2（分别是可积的）。 提案 3，Cor。命题 3 的第 1 条）意味着对于测度 $\theta_1 + \theta_2 + \theta_3 + \theta_4$，$f$ 是可测的（或者本质上可积、可积），即 $\geq |\theta|$。

### 3. 分解的度量相当于和具有紧凑支持的度量

#### 命题 4 {#int-v-s2-prop-4 .statement tag=090Q}

— 令$\mu$为局部紧致空间$T$的正测度，并令$\mathfrak{K}$为$T$的紧致子集的$\mu$密集集合。在$T$上存在一个正测度的可和族$(\mu_\alpha)_{\alpha \in A}$，使得$\mu = \sum_{\alpha \in A} \mu_\alpha$，并且使得测度$\mu_\alpha$属于到$\mathfrak{K}$和形式的支持是成对的不相交的紧集的局部可数族。

如果措施$\mu$是缓和的，指标集合$A$可以被认为是可数的。

考虑$\mathfrak{K}$的成对不相交的元素的局部可数族$(K_\alpha)_{\alpha \in A}$，使得集合$N = T - \bigcup_{\alpha \in A} K_\alpha$在局部$\mu$可以忽略不计

（第 IV, §5, No. 9 章，第 14 条提案）。对于每个函数 $f \in \mathscr{K}(T)$、集合
$$
\mu_\alpha(f) = \mu(f \varphi_{K_\alpha});
$$
$\mathscr{K}(T)$上的线性形式$\mu_\alpha$为正，因此是一项积极措施，$K_\alpha$中包含支持。由于$\mathfrak{K}$属于到$\mathfrak{K}$的元素中包含每个紧集，因此$\operatorname{Supp}(\mu_\alpha) \in \mathfrak{K}$代表所有$\alpha \in A$。剩下的只是证明族$(\mu_\alpha)$是可求和的，并且它的和等于$\mu$，在其他字中，对于每个函数$f \in \mathscr{K}_+(T)$，$\sum_{\alpha \in A} \mu_\alpha(f) = \mu(f)$。

现在，令$S$为$f$的（紧）支持，并让$A'$为由$\alpha \in A$形成的可数集合，使得$S \cap K_\alpha \neq \varnothing$。由于集合$N \cap S$是$\mu$-可以忽略不计，
$$
\begin{align*}
\mu(f) &= \mu(f \varphi_S) = \sum_{\alpha \in A'} \mu(f \varphi_{S \cap K_\alpha}) = \sum_{\alpha \in A'} \mu(f \varphi_{K_\alpha}) \\
&= \sum_{\alpha \in A} \mu(f \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha(f).
\end{align*}
$$
这样就完成了一般情况的证明。如果 $\mu$ 受到调节，则集合 $T$ 是 $\mu$ 调节，因此 $T$ 是序列的并紧集的 $(L_n)$ 以及可忽略不计的集合 （§ 1, No. 2，提案 5）；令$A'$为$\alpha \in A$的可数集合，使得$K_\alpha$与$L_n$之一相交。然后$\mu_\alpha = 0$对应$\alpha \notin A'$，紧接着是叙述的最后一句。

#### 注 {#int-v-s2-n3-rem-1 .statement tag=090R}

积极措施可能是序列措施中的和具有紧凑支持，并且不进行缓和（参见§ 1 的Exer. 4 a））。

### 习题{#int-v-s2-exercises}

§ 2](exercises/s2/)参见[习题。
