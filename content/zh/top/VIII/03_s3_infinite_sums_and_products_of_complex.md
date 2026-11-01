---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 3
section_title: Infinite sums and products of complex numbers
lang: zh
source: top-v-x
pdf_pages: 0121-0124, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: INFINITE SUMS OF COMPLEX NUMBERS
      page: 0
      pdf_page: 121
    - "no": 2
      title: MULTIPLIABLE FAMILIES IN $\mathbf{C}^*$
      page: 0
      pdf_page: 121
    - "no": 3
      title: INFINITE PRODUCTS OF COMPLEX NUMBERS
      page: 0
      pdf_page: 123
statements: 9
exercises: 5
content_sha256: 2d41d7c14761bbae4aad7aa57ef23a2997d4006666b72ecacdb789dd6aa1108b
translated_from: content/en/top/VIII/03_s3_infinite_sums_and_products_of_complex.md
translation_method: google
source_content_sha256: 07d4fe8c1f201c515f0cbf75d3cd066fc09084c3035b0204be862ef63ea6d88e
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: b2b08c621c1c47a5a5c660911d793b4cfb62bdbc702a387884cc585b26aea884
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 3. 复数的无限和和乘积

### 1. 复数的无限和

由于域$\mathbf{C}$的加法群与加法群$\mathbf{R}^2$相同，因此无需专门研究$\mathbf{C}$中的可和族和级数，因为这已包含在章VII, § 3的一般理论中；我们留给读者习题将该理论的结果翻译成复数理论的语言。我们仅陈述以下命题，它是章VII, § 3, no. 1 命题 3 的推论：

#### 命题 1 {#top-viii-s3-prop-1 .statement tag=0C0I}

*如果* $(u_\lambda)_{\lambda \in L}$ *和* $(v_\mu)_{\mu \in M}$ *是复数的两个可求和族，则族* $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M}$ *可求和，我们有*

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right).
$$

我们让读者来陈述四元数的相应的结果。

### 2. $\mathbf{C}^*$ 的多个家庭

在非零复数族$(z_i)_{i \in I}$不能乘法群$\mathbf{C}^*$中，相对于$I$(章III, § 5, no. 2)有限子集的补集的过滤器可乘除非$\lim z_i = 1$， 命题1);此外，由于$\mathbf{C}^*$的每个点都有邻域的可数基数系统，指标$i$的集合，因此如果族$(z_i)$是可乘的（章），则$z_i \neq 1$是可数的III, § 5, no. 2，命题 1) 的推论。

#### 命题 2 {#top-viii-s3-prop-2 .statement tag=0C0J}

*复数* $z_i = r_i (\cos \theta_i + i \sin \theta_i)$ *的族* $(z_i)$ *可乘当且仅当* $z_i$ *的绝对值的族* $(r_i)$ *可乘于* $\mathbf{R}_+^*$ *且* $z_i$ *的振幅族* $(\theta_i)$ *是可按群角度* $\mathfrak{A}$ 求和。

鉴于群$\mathbf{C}^*$($\S$1、no. 3、命题1)的结构，命题为章的命题4直接的推论 III、$\S$5、no. 4。

如果我们映射每个角度 $\theta$ 到它的一个度量（对于任何给定的基 $a$），属于到间隔 $] - \frac{1}{2} a, \frac{1}{2} a ]$，我们就有一个 $\mathfrak{A}$ 的*局部同构* 和 $\mathbf{R}$ ($\S$ 2， no. 2);由于$\lim \theta_i = 0$相对于$I$的有限子集的补集过滤器，我们可以替换条件（在命题2的叙述中）$\theta_i$应该可以通过条件在$\mathfrak{A}$中求和角度$\theta_i$的*测量*族$(t_i)$，其中属于到$] - \frac{1}{2} a, \frac{1}{2} a ]$应可在$\mathbf{R}$中求和。

下面的定理给出了复数族的另一个标准，放入形式$(1 + u_i)$，可与$\mathbf{C}^*$相乘。 （它概括了章 IV、$\S$ 7、no. 4 中的定理 4；另请参见章 IX、附录、no. 2、命题 1）：

#### 定理 1 {#top-viii-s3-thm-1 .statement tag=0C0K}

*族* $(1 + u_i)_{i \in I}$ *可乘于* $\mathbf{C}^*$ *当且仅当族* $(|u_i|)$ *可求和于* $\mathbf{R}$。

对于 $I$ 中的每个有限子集 $J$，将

$$
p_J = \prod_{i \in J} (1 + a_i), \quad s_J = \sum_{i \in J} a_i, \quad \sigma_J = \sum_{i \in J} |a_i|.
$$

#### 引理 1 {#top-viii-s3-lem-1 .statement tag=0C0L}

*对于每个有限子集* $J$ *of* $I$，*令* $\varphi(J) = \sup_{L \subset J} (p_L - 1)$。 *然后对于每个子集* $L$ *of* $J$ *我们有*

$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_L.
$$

如果 $L$ 为空，这一点就很清楚了。我们从$(L)$卡上的归纳出发。设$L = K \cup \{ \lambda \}$，其中$\lambda \notin K$；然后$p_L = p_K (1 + a_\lambda)$和$s_L = s_K + a_\lambda$，从而$p_L - 1 - s_L = (p_K - 1 - s_K) + (p_K - 1)a_\lambda$；因此，通过$\varphi(J)$的归纳假设和定义，我们有

$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_K + \varphi(J)|a_\lambda| = \varphi(J) \sigma_L,
$$

这就证明了引理。

#### 引理 2 {#top-viii-s3-lem-2 .statement tag=0C0M}

*如果*$J$*是*$I$的有限子集*使得*$\varphi(J) < 1/4$，*那么*

$$
|\sigma_J| \leq 4 \varphi(J)/(1 - 4 \varphi(J)).
$$

因为从$\sigma_L \leq \sigma_J$开始，对于$J$的所有子集$L$，从(2)可以得出$|s_L| \leq \varphi(J) \sigma_J + |p_L - 1| \leq (1 + \sigma_J)\varphi(J)$；但凭借章VII、$\S$3、no. 1、命题2，我们有$|\sigma_J| \leq 4 \sup_{L \subset J} |s_L|$，因此$\sigma_J \leq 4 \varphi(J)(1 + \sigma_J)$，结果如下。

现在让我们证明定理 1 中的条件就足够了。 假设族$(|u_i|)$在$\mathbf{R}$中可求和意味着族$(1 + |u_i|)$在$\mathbf{R}_+^*$中可相乘（章IV, § 7, no. 4，定理4）；因此，对于每个$\varepsilon > 0$，$I$有有限子集$J_0$，这样，对于不满足$J_0$的$I$的每个有限子集$L$，我们有$\prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon$。但我们可以将形式$\sum_M \left( \prod_{i \in M} u_i \right)$写成$\prod_{i \in L} (1 + u_i) - 1$，其中$M$贯穿$L$的所有非空子集；从$\left| \prod_{i \in M} u_i \right| = \prod_{i \in M} |u_i|$开始，我们有

$$
\left| \prod_{i \in L} (1 + u_i) - 1 \right| \leq \sum_M \left( \prod_{i \in M} |u_i| \right) = \prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon.
$$

这根据柯西准则证明了我们的断言，因为$\mathbf{C}^*$是完整的群。

我们仍然需要证明定理 1 中的条件是必要的。如果$(1 + u_i)_{i \in I}$是$\mathbf{C}^*$中的可乘族，则存在$I$的有限子集$J$，这样，对于$I$的每个不满足$J$的有限子集$H$，我们有$\left| \prod_{i \in H} (1 + u_i) - 1 \right| \leq 1/8$。到引理 2，$\sum_{i \in H} |u_i| \leq 1$对于$I$的每个有限子集$H$不满足$J$，因此族$(|u_i|)$可在$\mathbf{R}$中求和（章IV, § 7, no. 1， 定理1)。

上面的证明也比照适用于某些非交换除法环和代数中的（有序）无限乘积（参见习题6和章IX、附录）。

### 3. 复数的无限乘积

对于非零复数的无限乘积与一般因子$z_n = r_n (\cos \theta_n + i \sin \theta_n)$收敛于$\mathbf{C}^*$，从群$\mathbf{C}^*$的结构，乘积与一般因子是必要且充分的$r_n$收敛于$\mathbf{R}_+^*$和级数，一般项$t_n$（$\theta_n$的测度位于]$-\frac{1}{2}a$、$\frac{1}{2}a$]）收敛于$\mathbf{R}$。

#### 定义 1 {#top-viii-s3-def-1 .statement tag=0C0N}

*复数的无限乘积，与一般因子* $1 + u_n$，*如果乘积与一般因子* $1 + |u_n|$ *收敛*（或等价地，如果级数与一般项，则称其绝对收敛） $|u_n|$ 收敛）。

#### 命题 3 {#top-viii-s3-prop-3 .statement tag=0C0O}

*复数的无穷大乘积可交换收敛当且仅当它绝对收敛。*

#### 注 1 {#top-viii-s3-n3-rem-1 .statement tag=0C0P}

乘积与一般因子$|1 + u_n|$可以收敛，并且确实在$\mathbf{R}_i^*$绝对收敛，而乘积不与一般因子$1 + |u_n|$收敛（见习题4）；当然，如果所有$u_n$都是真实的并且从某个指标开始$> 0$，就会发生这种不能。

#### 注 2 {#top-viii-s3-n3-rem-2 .statement tag=0C0Q}

正如已经针对因子$> 0$的乘积所述，级数与一般项$u_n$的收敛对于乘积与一般因子$1 + u_n$的收敛既不是必要的也不是充分的。

### 习题 {#top-viii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
