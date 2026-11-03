---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 3
section_title: Infinite sums in the groups $\mathbf{R}^n$
lang: zh
source: top-v-x
pdf_pages: 0089-0092, 0101-0102
extraction: ocr
subsections:
    - "no": 1
      title: SUMMABLE FAMILIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 89
    - "no": 2
      title: SERIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 92
statements: 9
exercises: 2
content_sha256: b21f7e2ff1990b574333b6ee8bee2e743b022021e41f998c85c73f90c1f13c8d
translated_from: content/en/top/VII/03_s3_infinite_sums_in_the_groups_mathbf_r_n.md
translation_method: google
source_content_sha256: 469c822cd0058ba2bb0510721ee43c3d335b871a5db27467e63bfe955b6c2715
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: af8f716f043410e1cb2bec722f7a4246647bca2d8e1c6d1b7164d4516ad4b2e0
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 3. 无限和群 $\mathbf{R}^n$

### 1. $\mathbf{R}^n$ 中的可求和族

由于$\mathbf{R}^n$的每个点都有邻域的*可数*基本系统，因此仅当指标$t$的集合时，加法群$\mathbf{R}^n$的点的族$(x_t)$才可求和这样$X_t \neq 0$是*可数的*（章III, § 5, no. 2，推论到命题1）；因此，本质上，$\mathbf{R}^n$中可求和族的研究被简化为序列中可求和族的研究。然而，出于与章IV中给出的相同原因，对于$\mathbf{R}$中的可求和族，我们不应在下文中对指标集合的基数强加任何限制

#### 命题 1 {#top-vii-s3-prop-1 .statement tag=0BZK}

*family* $(x_i)_{i \in I}$ *of 点* $x_i = (x_{i,k})_{1 \leq k \leq n}$ *of* $\mathbf{R}^n$ *可求和当且仅当每个* $n$ *families* $(x_{i,k})_{i \in I}$ *of 实数可在* $\mathbf{R}$ 中求和。

这是从章 III, § 5, no. 4、命题 4 得出的。

命题 1 的条件可以变换如下：

#### 定理 1 {#top-vii-s3-thm-1 .statement tag=0BZL}

* $\mathbf{R}^n$ * 的点 * 的 * $(x_i)_{i \in I}$ * 可求和当且仅当 * $x_i$ * 的欧氏范数的 * $(||x_i||)$ * 可在* $\mathbf{R}$ 中求和。

对于实数 (章 IV, § 7, no. 2, 定理 3) 族的可求性，这可以毫无困难地从命题 1, 条件得出，不等式

$$
\sup_{1 \leq k \leq n} |x_{i,k}| \leq ||x_i|| \leq \sum_{i=1}^n |x_{i,i}|,
$$

以及比较原理 (章 IV, § 7, no. 1, 定理 2)。

我们还可以采取一些不同的方式，首先建立以下命题：

#### 命题 2 {#top-vii-s3-prop-2 .statement tag=0BZM}

*如果* $(x_i)_{i \in I}$ *是* $\mathbf{R}^n$ 中点的任意有限族，*则*

$$
\sum_{i \in I} ||x_i|| \leq 2n \cdot \sup_{J \subset I} \left| \sum_{i \in J} x_i \right|.
$$

因为如果$x_i = (x_{ij})_{1 \leq j \leq n}$，我们有$||x_i|| \leq \sum_{j=1}^n |x_{ij}|$，因此

$$
\sum_{i \in I} ||x_i|| \leq \sum_{j=1}^n \left( \sum_{i \in I} |x_{ij}| \right).
$$

现在$\sum_{i \in I} |x_{ij}| = \sum_{i \in I} x_{ij}^+ + \sum_{i \in I} x_{ij}^-$，因为对于$I$的每个子集$J$，我们有

$$
-\sum_{i \in I} x_{ij}^- \leq -\sum_{i \in J} x_{ij}^- \leq \sum_{i \in J} x_{ij}^+ \leq \sum_{i \in I} x_{ij}^+
$$

由此可见

$$
\sum_{i \in I} |x_{ij}| \leq 2 \cdot \sup_{J \subset I} \left| \sum_{i \in J} x_{ij} \right|.
$$

但是$\left| \sum_{i \in J} x_{ij} \right| \leq \left| \sum_{i \in J} x_{ij} \right|$，因此不等式 (1)。

现在，定理 1 等价于以下命题（因为$\mathbf{R}^n$是完整的群）：族$(x_i)$满足柯西准则（章III, § 5, no. 2，定理1）当且仅当族$(||x_i||)$也满足柯西准则。现在三角形不等式表明这个条件是足够的，不等式（1）表明它是必要的。

此外，我们还有不等式

$$
\left| \sum_i x_i \right| \leq \sum_i ||x_i||
$$

它来自于有限部分和的类似不等式的经过到极限。

#### 推论 {#top-vii-s3-n1-cor-1 .statement tag=0BZN}

*族* $(x_i)$ *的点的* $\mathbf{R}^n$ *可求和当且仅当族的有限部分和的集合有界于* $\mathbf{R}^n$。

由定理 1和三角形不等式，这个条件是必要的；由不等式 (1) 和定理 1 就足够了。

#### 命题 3 {#top-vii-s3-prop-3 .statement tag=0BZO}

*设*$(x_\lambda)_{\lambda \in L}$*为*$\mathbf{R}^m$、$(y_\mu)_{\mu \in M}$*可求和的点族*$\mathbf{R}^n$、*并令*$f$*为*$\mathbf{R}^m \times \mathbf{R}^n$*到*$\mathbf{R}^p$的双线性映射。 *然后家庭* $(f(x_\lambda, y_\mu))_{(\lambda, \mu) \in L \times M}$ *可求和，我们有*

$$
\sum_{(\lambda, \mu) \in L \times M} f(x_\lambda, y_\mu) = f \left( \sum_{\lambda \in \mu} x_\lambda, \sum_{\mu \in M} y_\mu \right).
$$

为了证明族$(f(x_\lambda, y_\mu))$是可求和的，通过命题 1就足以确定由$\mathbf{R}^n$中点$f(x_\lambda, y_\mu)$的坐标形成的每个$p$族是可求和的：在其他字中，我们可以将自己限制在$f$是双线性的情况*形式*;但对于这样的形式 $f$ 我们有

$$
f(x, y) = \sum_{i, j} a_{ij} x_i y_j,
$$

因此我们回到案例$f(x, y) = x_i y_j$，在这种情况下结果已经被证明了（章IV, § 7, no. 3，命题1）。

通过专门化函数 $f$，我们特别得到以下推论：

#### 推论 1 {#top-vii-s3-prop-3-cor-1 .statement tag=0BZP}

*如果* $(a_\lambda)_{\lambda \in L}$ *是实数的可求和族，并且如果* $(x_\mu)_{\mu \in M}$ *是* $\mathbf{R}^n$的点的可求和族，*那么该族* $(a_\lambda x_\mu)_{(\lambda, \mu) \in L \times M}$ *是可求和的，我们有*

$$
\sum_{(\lambda, \mu) \in L \times M} a_\lambda x_\mu = \left( \sum_{\lambda \in L} a_\lambda \right) \left( \sum_{\mu \in M} x_\mu \right).
$$

#### 推论 2 {#top-vii-s3-prop-3-cor-2 .statement tag=0BZQ}

*如果* $(x_\lambda)_{\lambda \in L}$ *和* $(y_\mu)_{\mu \in M}$ *是* $\mathbf{R}^n$的点的两个可求和族，*则族* $(x_\lambda | y_\mu)$ *(cf. 章 VI, § 2, no. 2)* *可求和于* $\mathbf{R}$，*我们有*

$$
\sum_{(\lambda, \mu) \in L \times M} (x_\lambda | y_\mu) = \left( \sum_{\lambda \in L} x_\lambda \middle| \sum_{\mu \in M} y_\mu \right).
$$

### 2. 级数在 $\mathbf{R}^n$

当且仅当每个$n$、级数、$(x_{mi})_{m \in \mathbf{N}}$收敛于$\mathbf{R}$时，级数的通项为$x_m = (x_{mi})_{1 \leq i \leq n}$收敛于$\mathbf{R}^n$。

#### 定义 1 {#top-vii-s3-def-1 .statement tag=0BZR}

** $\mathbf{R}^n$ 的点级数 *如果其项的欧氏范数级数收敛，则称其绝对收敛。*

#### 命题 4 {#top-vii-s3-prop-4 .statement tag=0BZS}

* 点的* $\mathbf{R}^n$ * 级数交换收敛当且仅当绝对收敛。*

这是上面的章III, § 5, no. 7和定理1的命题9中的推论和定理1。

章 IV, § 7 中给出的例表明$\mathbf{R}^n$ 中的级数可以*收敛*，但不*绝对收敛*。

### 习题{#top-vii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
