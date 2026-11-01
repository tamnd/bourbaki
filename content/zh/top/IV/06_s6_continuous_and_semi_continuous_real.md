---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 6
section_title: Continuous and semi-continuous real-valued functions
lang: zh
source: top-i-iv
book_pages: 359-363, 393-397
pdf_pages: 0365-0369, 0399-0403
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS REAL-VALUED FUNCTIONS
      page: 359
      pdf_page: 365
    - "no": 2
      title: SEMI-CONTINUOUS FUNCTIONS
      page: 360
      pdf_page: 366
statements: 15
exercises: 15
content_sha256: 0843833086c743480ae10ca744007f30f6015009bcea86adcfb1499d218a2018
translated_from: content/en/top/IV/06_s6_continuous_and_semi_continuous_real.md
translation_method: google
source_content_sha256: a4a4561480f34bbe62b92e5864816f73a0e123a5320283ae8272978222d04a91
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 3893623cb4905cce5f7c6cbf32df8c02d1502f2c7c96324609eca9ddd35259ef
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 6. 连续和半连续实值函数

### 1. 连续实值函数

除了任意拓扑空间 (章 I, § 2) 中连续函数和值的一般性质外，连续实值函数还具有以下两个基本性质：

#### 定理 1（威尔斯特拉斯）{#top-iv-s6-thm-1 .statement tag=0BSF}

令$f$为定义在非空准紧空间$X$上的连续实值函数。那么至少有一个点$a \in X$使得$f(a) = \sup_{x \in X} (f(x))$，并且至少有一个点$b \in X$使得$f(b) = \inf_{x \in X} f(x)$。因为 $f(X)$ 是紧致的 (章 I, § 9, no. 4, 定理 2)，因此在 $\overline{\mathbf{R}}$ 中闭合；因此 $f(X)$ 包含它的界限。

这个定理经常在形式中表述，非空拟紧空间上的连续实值函数达到其界限。

#### 推论 {#top-iv-s6-n1-cor-1 .statement tag=0BSG}

如果在非空准紧空间 $X$ 上定义的实值函数在 $X$ 上是连续且有限的，则它在 $X$ 内有界。

#### 定理 2（博尔扎诺）{#top-iv-s6-thm-2 .statement tag=0BSH}

令 $f$ 为定义在连接的空间 $X$ 上的连续实值函数。如果$a$和$b$是$X$中的任意两个点，并且如果$\alpha$是实数属于到端点为$f(a)$和$f(b)$的闭区间，则至少有一个点$x \in X$使得$f(x) = \alpha$。

因为 $f(X)$ 是连通的 (章 I, § 11, no. 2, 命题 4)，因此是$\overline{\mathbf{R}}$ (§ 4, no. 2, 命题 5) 的区间；因此它是包含，端点为$f(a)$和$f(b)$的闭区间。

这个定理通常用形式来表示，即连接的空间不能上的连续实值函数从一个值传递到另一个，而无需经过通过所有中间值*。

这个性质绝不是连续函数的特征；在连接的空间上定义了函数的例，并且*在每个点*处不连续，其中有这个性质（习题2）。

### 2. 半连续函数

令$f$为定义在拓扑空间$X$上的实值函数。要使 $f$ 在点 $a \in X$ 连续，满足以下条件是充分必要的：
(i) 给定任何实数$h < f(a)$，存在$a$的邻域$V$，使得在每个点$x \in V$我们有$h < f(x)$；
(ii) 给定任何实数$k > f(a)$，存在$a$的邻域$W$，使得在每个点$x \in W$我们有$k > f(x)$。

函数，其中满足*其中只有一个*条件在数学分析中发挥重要的部分作用。准确地说，我们做了以下定义：

#### 定义 1 {#top-iv-s6-def-1 .statement tag=0BSI}

*实值函数$f$，定义在拓扑空间$X$上，据说是下半连续*（或*上半连续*）*在点$a \in X$，如果对于每个$h < f(a)$[或。每个$k > f(a)$]都有邻域$V$/$a$，这样$h < f(x)$[分别。 $k > f(x)$] *每个* $x \in V$。

*实值函数被称为下半连续*（或*上半连续*）*在$X$上，如果它是下半连续*（或*上半连续*）*在$X$*的每个点*。

因此，实值函数$f$在点$a$处*连续*当且仅当它在$a$处*上半连续*和下半连续*。

如果$f$在点处是下半连续，则$-f$在点处是上半连续，反之亦然；因此，我们可以在接下来的内容中限制自己，只考虑*下半连续*函数的性质。

很明显，在$X$上是下半连续的函数在$X$的每个*子空间*上也是下半连续的。

#### 例 1 {#top-iv-s6-n2-exa-1 .statement tag=0BSJ}

如果$f$在点$a$有一个*相对最小值*，也就是说，如果$a$有邻域$V$，这样，对于每个$x \in V$，我们有$f(a) \leq f(x)$，那么$f$是下半连续的$a$。特别是，如果$f(a) = -\infty$，则$f$在$a$处是下半连续的。

#### 例 2 {#top-iv-s6-n2-exa-2 .statement tag=0BSK}

定义 $\mathbf{R}$ 上的实值函数 $f$，如果 $x$ 是无理数，则放入 $f(x) = 0$；如果 $x$ 是有理数且等于不可约分数 $p/q$，则放入 $f(x) = 1/q$ （$q > 0$）。对于每个整数$n > 0$，有理数$p/q$的集合使得$q < n$是封闭的，并且其点是孤立的；因此，对于每个无理数$x$，邻域$V$为$x$，使得$f(y) \leq 1/n$对于所有$y \in V$，这表明$f$在$x$连续；另一方面，$f$ 在每个有理数点 $x$ 处都有一个“相对最大值”。因此$f$是$\mathbf{R}$上的上半连续。

对于$f$在$a$处的下半连续，条件可以用说来表示，对于每个$h < f(a)$，集合$\overline{f}([h, +\infty])$必须是$a$的邻域。

对于倾向于$f(a)$的实数$< f(a)$的递增序列$(h_n)$来说，这个条件就足够了。

将$\overline{\mathbf{R}}$赋予拓扑，其中开集合为$\varnothing$，并且$\overline{\mathbf{R}}$的所有开区间在右侧无界（即有限$a$的所有区间$]a, +\infty[$，以及区间$[--\infty, +\infty] = ]\leftarrow, \rightarrow[]$）。那么实值函数$f$在$a$处是下半连续的当且仅当它在$a$处连续时，将映射考虑到赋予此拓扑的$\overline{\mathbf{R}}$。

#### 命题 1 {#top-iv-s6-prop-1 .statement tag=0BSL}

*拓扑空间 $X$ 上的实值函数 $f$ 是下半连续当且仅当，对于每个有限实数 $k$，$\overline{f}([k, +\infty])$ [所有 $x \in X$ 的集合使得$f(x) > k$] 是$X$ 中的开集合 [或者，等效地，$\overline{f}([-\infty, k])$ 是$X$ 中的闭集合]。*

对于这个条件表明$\overline{f}([k, +\infty])$是其每个点的邻域。

为了使 $f$ 在 $X$ 上成为下半连续，对于所有实数 $k$ 属于到$\mathbf{R}$ 的稠密子集，$f^{-1}([k, +\infty])$ 在 $X$ 中开路就足够了。

#### 推论{#top-iv-s6-n2-cor-1 .statement tag=0BSM}

*拓扑空间$X$的子集$A$在$X$中是开（或闭）当且仅当其特征函数（*）$\varphi_A$在$X$上是下（或上）半连续。*

因为$\overline{f}_A([k, +\infty])$对于$k \geq 1$来说是空的，对于$0 \leq k < 1$来说等于$A$，对于$k < 0$来说等于$X$。

#### 定理 3 {#top-iv-s6-thm-3 .statement tag=0BSN}

*令$f$为非空准紧空间$X$上的下半连续函数。那么至少有一个点$a \in E$使得$f(a) = \inf_{x \in X} f(x)$（在其他字中，$f$在$X$中达到其下确界）。*

对于每个 $k \in f(X)$，请考虑集合 $A_k = \overline{f}([-\infty, k])$。这些集合非空，并且形式是$X$上的过滤器基；因为它们被命题 1 封闭，所以它们至少有一个公共的点 $a$ [准紧空间的公理 (C'')]。因此，对于每个$x \in X$，我们有$f(a) \leq f(x)$，然后是定理。

(*) 我们记得（集合理论，章III, § 5, no. 5）集合$X$的子集$A$的特征函数$\varphi_A$是在$X$上定义的函数这样$\varphi_A(x) = 1$ 代表所有 $x \in A$，$\varphi_A(x) = 0$ 代表所有 $x \in \complement_A$。

#### 推论{#top-iv-s6-n2-cor-2 .statement tag=0BSO}

令$f$为非空准紧空间$X$上的下半连续函数。如果 $f(x) > -\infty$ 对于所有 $x \in X$，则 $f$ 的边界在 $X$ 内。

注，对于上半连续函数，此定理和相应的定理包括Weierstrass的定理作为特殊情况（no. 1，定理1）。

#### 命题 2 {#top-iv-s6-prop-2 .statement tag=0BSP}

令$f$和$g$为两个实值函数，在点$a \in X$处下半连续。那么函数$\inf(f, g)$和$\sup(f, g)$在$a$处是下半连续；每当定义$f + g$时，它也是如此；如果定义$f$和$g$是$\geq 0$并且乘积$fg$，$fg$也是如此。

我们给证明换取$f + g$；这个论点在其他情况下也是类似的。如果$f(a)$或$g(a)$等于$-\infty$，结果就清楚了；如果不是，则$f(a) + g(a) > -\infty$。每个有限的数$h < f(a) + g(a)$都可以写成$h = r + s$，其中$r < f(a)$和$s < g(a)$是有限的[取$s$就足够了$h - f(a) < s < g(a)$]；到假设，$a$有邻域$V$，这样，对于每个$x \in V$，我们有$r < f(x)$，并且邻域$W$，这样对于每个$x \in W$，我们有$s < g(x)$；因此 $h = r + s < f(x) + g(x)$ 对于邻域 $V \cap W$ 中的所有点 $x$。

以同样的方式我们看到，如果$f$在点$a$处是下半连续，并且如果$f \geq 0$，则$1/f$在$a$处是上半连续。

#### 定理 4 {#top-iv-s6-thm-4 .statement tag=0BSQ}

函数的族$(f_i)$的上包络线在点$a \in X$处是下半连续，在$a$处是下半连续。

设 $g$ 为上层信封。对于每个$h < g(a)$，有指标$i$使得$h < f_i(a) \leq g(a)$，以及$a$的邻域$V$使得$h < f_i(x)$对于所有$x \in V$；因此，对于所有 $x \in V$，$a$ 更不必说 $h < g(x)$。

从命题 2 可以得出，下半连续函数的有限数的下包络线同样是下半连续；但对于下半连续函数的无限族的下包络线来说，这通常不是正确的。对于例，如果$r$是任何有理数数，则让$f_r$表示函数，它在$r$等于0，并且对于所有实数$x \neq r$等于1； $f_r$ 的下包络为函数 $g$，对于每个有理数数等于 0，对于每个无理数数等于 1（“狄利克雷函数”），并且这个函数在无理数处不是下半连续的点。

#### 推论{#top-iv-s6-n2-cor-3 .statement tag=0BSR}

空间 $X$ 上的连续实值族函数的上包络线在 $X$ 上是下半连续的。

在章 IX, § 1, no. 6、命题 5 中，我们将证明，如果 $X$ 是可统一的（并且仅在这种情况下），则此命题的逆命题为真：可统一的空间上的每个下半连续函数是连续族的上包络线函数。

#### 命题 3 {#top-iv-s6-prop-3 .statement tag=0BSS}

*实值函数 f，在拓扑空间X上定义，当且仅当*$\liminf_{x \to a} f(x) = f(a)$时在点$a \in X$处是下半连续的[或者，等效地，当且仅当$\liminf_{x \to a} f(x) \geq f(a)$]。

条件是*必要的*。因为，给定任何$h < f(a)$，$a$有邻域V，使得$h < f(x)$对于所有$x \in V$；因此
$$
h \leq \inf_{x \in V} f(x) \leq \liminf_{x \to a} f(x)
$$
（§ 5, no. 6，公式（12）），等等$f(a) \leq \liminf_{x \to a} f(x)$。 条件*足够*；因为如果满足，则对于每个$h < f(a)$，$a$都有邻域V，使得$h \leq \inf_{x \in V} f(x)$，因此$f$在$a$处是下半连续的。

#### 命题 4 {#top-iv-s6-prop-4 .statement tag=0BST}

*设 f 是在拓扑空间 X 的稠密子集 A 上定义的任意实值函数。如果对于每个 $x \in X$，我们放置* $g(x) = \liminf_{y \to x, y \in A} f(y)$，*则 g 在 X* 上是下半连续的。

因为，给定任何$h < g(x)$，都存在$x$的*开*邻域V，这样，对于所有$z \in V \cap A$，我们有$h < f(z)$；现在 V 是其每个点 $y$ 的邻域；因此，我们对所有 $y \in V$ 都有 $\liminf_{z \to y, z \in A} f(z) = g(y) \geq h$，结果如下。

函数$g$称为$f$的*下半连续正则化*。我们类似地对定义 $f$ 进行*上半连续正则化*。

我们也可以将定义$g$作为X上下半连续函数$\varphi$的*最大的*，对于所有$x \in A$来说$\varphi(x) \leq f(x)$。如果 $f$ 是 A 上的*下半连续*，则 $g$ 是 $f$ 到 X 命题 3 的 *扩张*。

### 习题{#top-iv-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
