---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 1
section_title: Subgroups and quotient groups of $\mathbf{R}^n$
lang: zh
source: top-v-x
pdf_pages: 0073-0085, 0093-0099
extraction: ocr
subsections:
    - "no": 1
      title: DISCRETE SUBGROUPS OF $\mathbf{R}^n$
      page: 0
      pdf_page: 74
    - "no": 2
      title: CLOSED SUBGROUPS OF $\mathbf{R}^n$
      page: 0
      pdf_page: 77
    - "no": 3
      title: ASSOCIATED SUBGROUPS
      page: 0
      pdf_page: 79
    - "no": 4
      title: HAUSDORFF QUOTIENT GROUPS OF $\mathbf{R}^n$
      page: 0
      pdf_page: 82
    - "no": 5
      title: SUBGROUPS AND QUOTIENT GROUPS OF $T^n$
      page: 0
      pdf_page: 83
    - "no": 6
      title: PERIODIC FUNCTIONS
      page: 0
      pdf_page: 84
statements: 19
exercises: 15
content_sha256: c5444a18fad04bde5110ecbc25e9a4d5d33e8698c23b8a29c2f70e2779f364ad
translated_from: content/en/top/VII/01_s1_subgroups_and_quotient_groups_of_mathbf.md
translation_method: google
source_content_sha256: fe624f0a3e7b7cbf13cf90a248b8acc2a36a832c024d805c9d19b21538d08a71
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: ad7932cba5fa34a4c799eaf70522b3289d3870e0beecdfbe87572d06dfb2b31a
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 1. 子群和商群 $\mathbf{R}^n$

首先介绍一下约定：如果 G 是拓扑群，则对于每个整数 $n > 0$，我们定义 n 因子的 (章 III, § 2) 乘积群 $G^n$ 等于 G。在这个截面中，我们根据$G^0$仅表示一个元素中的群由……组成的约定，将扩展这个定义对应于$n = 0$。如果 H 是任意群，我们将用 H 认同 $G^0 \times H$。

对于集合$\mathbf{R}^n$，我们一方面必须考虑它的（加法）拓扑群结构，另一方面它的向量空间结构超过域$\mathbf{R}$（章VI, § 1, no. 3）。给定$\mathbf{R}^n$的子集 A，我们可以设想由A生成$\mathbf{R}^n$的子群（A的点的所有线性组合的集合，以及整数系数）以及向量 A 生成子空间（A 的点的所有线性组合中的集合，真实的系数）；这两个概念必须仔细区分。根据代数中的定义，A的秩是A生成的$\mathbf{R}^n$的向量子空间V的维数；因此，说 A 是秩 $p$ 就等价于说，其中存在 $p$ 点 $x_i \in A$，其中形式相对于域 $\mathbf{R}$ 是一个自由的系统（在其他字，关系$\sum_i t_i x_i = 0$，其中$t_i$是实数，意味着每个$i$有$t_i = 0$）和V的形式基（这意味着每点 V是$x_i$与真实系数的线性组合）。

接下来我们还必须利用概念、系统、点、$\mathbf{R}^n$，它们相对于有理数数的域、$\mathbf{Q}$是自由的；这样系统是$\mathbf{R}^n$的有限子集$(x_i)$，这样关系$\sum_i r_i x_i = 0$，其中$r_i$是有理数数（或整数 - 它是同一件事），意味着每个 $i$ $r_i = 0$。这个概念必须与关于$\mathbf{R}$的自由系统仔细区分：每个关于$\mathbf{R}$自由的系统对于$\mathbf{Q}$也是自由的，但是逆命题是假的（例如，数1和$\mathbf{R}$ 形式中的$\sqrt{2}$ 相对于 $\mathbf{Q}$ 是免费的系统，但相对于 $\mathbf{R}$ 不是免费的系统）。每当我们无条件地谈论*免费的系统*时，我们总是指的是免费的系统*相对于*$\mathbf{R}$。因此，有必要区分 $\mathbf{R}^n$ 向量空间结构 *相对于* $\mathbf{R}$ 和向量空间结构 *相对于* $\mathbf{Q}$；特别地，向量子空间*相对于*$\mathbf{Q}$由$\mathbf{R}^n$的子集$A$生成，是$A$的所有线性组合的集合$U$，且有*有理* 系数；它包含在$A$生成的向量子空间$V$（相对于$\mathbf{R}$）中，但通常与$V$不同。 $U$的维数（*相对于*$\mathbf{Q}$）称为$A$的*有理秩*；它*至少等于*上面定义的$A$的*秩*（$V$的维数相对于$\mathbf{R}$）；如果$A$是无限集合，则它可能是“无限”，而$\mathbf{R}^n$的任何非空子集的秩始终是$\leq n$；特别是，$\mathbf{R}^n$的任何*不可数*子集的有理秩始终是无限的，因为任何超过$\mathbf{Q}$的有限维向量空间都是可数的。

在这个截面中，我们首先要对加法群$\mathbf{R}^n$*关闭的子群*进行确定结构。

### 1. 离散子群 OF $\mathbf{R}^n$

我们在章V（§ 1, no. 1，命题1）中看到，除了$\mathbf{R}$本身之外，$\mathbf{R}$唯一闭合的子群是由*单个*元素生成的*离散*子群。我们首先考虑 $\mathbf{R}^n$ 的*离散* 子群。

首先，$\mathbf{R}^n$的$p$向量（$p \leq n$）典范基（章VI, § 1, no. 3）生成的$\mathbf{R}^n$子群是与乘积同构的离散群 $p$ 群中的 $\mathbf{Z}^p$ 等于 $\mathbf{Z}$。更一般地，考虑由 $p$ 点 $a_i$ ($1 \leq i \leq p$) 生成的子群 $G$，其中形式是免费的系统。存在一个 $\mathbf{R}^n$ 的双射线性映射，其中映射 $a_i$ 到 $e_i$ ($1 \leq i \leq p$)；由于这样的映射是拓扑群$\mathbf{R}^n$的自同构，$G$与$e_i$（$1 \leq i \leq p$）生成的拓扑群到子群是同构的，因此是一个*离散* 秩 $p$ 的子群与 $\mathbf{Z}^p$ 同构。

群 $\mathbf{Z}^p$的结构，以及$G$的代数已被研究。我们回顾一下这项研究的主要结果。 $G$相对于环$\mathbf{Z}$的*基*为$p$点系统

$$
b_i = \sum_{j=1}^p r_{ij} a_j,
$$

其中 $r_{ij}$ 为整数，使得行列式 $\det (r_{ij})$ 等于 $+1$ 或 $-1$。 $G$ 的每个 *子群* $H$ 都是离散的，并且秩 $q \leq p$；此外，如果$H$是给定的子群秩$q$，则存在$p$点$b_i$（$1 \leq i \leq p$）的空闲系统，其中生成 $G$，以及 $q$ 点 $c_i$ ($1 \leq i \leq q$) 的系统，其中生成 $H$，这样我们就有 $c_i = e_i b_i$ 对应 $1 \leq i \leq q$，其中 $e_i$ 是整数（$H$相对于$G$的不变量因子）使得
$$
e_{i+1} \equiv 0 \pmod{e_i} \quad \text{for} \quad 1 \leq i \leq q - 1.
$$
商群$G/H$是与$\mathbf{Z}^{p-q} \times F$同构的离散群，其中$F$是有限阿贝尔的群，$q$循环子群的直接乘积各自阶$e_1, \ldots, e_q$。

现在我们将证明，我们刚才考虑的 $\mathbf{R}^n$ 的离散子群是唯一存在的。

#### 命题 1 {#top-vii-s1-prop-1 .statement tag=0BY4}

*令$G$为秩$p$的$\mathbf{R}^n$的离散子群，令$(a_i)_{1 \leq i \leq p}$为$G$的$p$点的自由系统，令$P$为闭集具有中心 $o$ 和基向量 $a_i$ (章 VI, § 1, no. 3) 的平行曲面。那么集合 $G \cap P$ 是有限的，生成 $G$，$G$ 的每个点都是 $a_i$ 的线性组合，有理数系数。*

$G \cap P$ 是紧凑且离散的，因此*有限*。令$x$为$G$中的任意点；它等于$a_i$与实系数的线性组合$\sum_{i=1}^p t_i a_i$。对于每个整数$m > 0$，考虑点
$$
z_m = mx - \sum_{i=1}^p [mt_i] a_i = \sum_{i=1}^p (mt_i - [mt_i]) a_i \ (*) ;
$$
它位于属于到$G$，从$0 \leq mt_i - [mt_i] < 1$开始，它位于$P$。因此，首先是$x = z_1 + \sum_{i=1}^p [t_i] a_i$，从而由$G \cap P$生成$G$；其次，由于$G \cap P$是有限的，因此存在两个不同整数$h, k$使得$z_h = z_k$，从而$(h - k)t_i = [ht_i] - [kt_i]$小于（$1 \leq i \leq p$），因此$t_i$是有理数。

#### 推论 {#top-vii-s1-n1-cor-1 .statement tag=0BY5}

*设$(a_i)_{1 \leq i \leq p}$是$p$点的免费系统和$\mathbf{R}^n$，并让*
$$
b = \sum_{i=1}^p t_i a_i
$$
*是$a_i$的线性组合，与真实的系数。那么由 $p + 1$ 点 $a_1, a_2, \ldots, a_p$ 和 $b$ 生成的 $\mathbf{R}^n$ 的子群 $G$ 是离散的当且仅当数 $t_i$ 是有理数。*

(*) 我们记得 (章 IV, § 8, no. 2)，对于每个实数 $x, [x]$ 是 $x$ 的积分部分，即最大的有理整数 $\leq x$。

命题 1 表明条件是必要的。这也是足够的，因为如果满足，我们可以写$t_i = m_i/d$，其中$d$和$m_i$是整数（$1 \leq i \leq p$）；因此，$b$ 是线性组合，以及 $p$ 点 $(1/d)a_i$ 中的整数系数；因此$G$是这些$p$点生成的离散群的子群，因此它本身也是离散的。

命题 1 的结果可以表示如下：如果 $\mathbf{R}^n$ 形式系统的*离散* 子群 $G$ 的 $q$ 点 $x_i$ ($1 \leq i \leq q$) 则 *依赖于* $\mathbf{R}$，那么它们形式系统*依赖于*$\mathbf{Q}$。紧接着，$\mathbf{R}^n$ 的离散子群的*有理秩* 等于它的*秩*。

推论到命题 1，应用于$a_i$是$\mathbf{R}^n$的典范基的$n$向量$e_i$的情况，给出以下命题：

#### 命题 2（克罗内克）{#top-vii-s1-prop-2 .statement tag=0BY6}

*令$\theta_1, \theta_2, \ldots, \theta_n$为$n$实数。在阶中，对于每个$\varepsilon > 0$，都存在整数$q$和$n$整数*
$$
p_i \quad (1 \leq i \leq n)
$$
*这样*
$$
|q\theta_i - p_i| \leq \varepsilon \quad (1 \leq i \leq n),
$$
*如果这些不等式中至少有一个的左侧没有消失，则 $\theta_i$ 中至少有一个是无理数是必要且充分的。*

#### 定理 1 {#top-vii-s1-thm-1 .statement tag=0BY7}

*$\mathbf{R}^n$、秩等于$p$的每个离散子群$G$，都是由$p$点的空闲系统生成。*

凭借前面回忆的群与$\mathbf{Z}^p$同构的性质，足以证明$G$是由$p$点的自由系统生成的离散群的*子群*。现在，由于$G$是秩$p$，因此存在$p$点$a_i$（$1 \leq i \leq p$）$G$的自由系统，使得每个$x \in G$等于线性组合 $a_i$与真实系数的$\sum_{i=1}^p t_i a_i$；由于 $G$ 是离散的，命题 1 表明 $t_i$ 是*有理数*。此外，命题 1 表明$G$ 是由点的*有限* 数生成的；由于这些点是$a_i$的线性组合和有理系数，因此存在整数$d$，使得它们是线性组合和$p$的*整数*系数点$(1/d)a_i = a'_i$。由此可见，$G$是由$a'_i$生成的群中的子群。

定理 1 也可以在不依赖于不变量因子 (cf. 习题 1) 的理论的情况下得到证明。

$\mathbf{R}^n$ 的离散子群秩 $n$ 也称为 $\mathbf{R}^n$ 中的*格子*。

### 2. 已关闭子群 $\mathbf{R}^n$

我们已经知道 $\mathbf{R}^n$ 的关闭子群的两个型；一方面，$\mathbf{R}^n$的*向量子空间*，同构于群$\mathbf{R}^p$（$p \leq n$）（章IV, § 1, no. 4，命题2）；另一方面，正如我们刚才所看到的，*离散* 子群 (章 III, § 2, no. 1, 命题 5) 同构于群 $\mathbf{Z}^q$ ($q \leq n$)。现在，我们将通过证明这样的子群与形式的 *乘积* 同构，来闭合 $\mathbf{R}^n$ 的 *任意* 子群的确定结构

$$
\mathbf{R}^p \times \mathbf{Z}^q \quad \text{where} \quad 0 \leq p + q \leq n.
$$

证明取决于以下命题：

#### 命题 3 {#top-vii-s1-prop-3 .statement tag=0BY8}

** $\mathbf{R}^n$ *包含的每个非离散闭子群一条线经过穿过* $o$。

令$(x_p)_{p \in \mathbf{N}}$为$G$的点的无限序列，使得$x_p \neq o$和$\lim_{p \to \infty} x_p = o$；到假设这样的序列就存在了。令 $P$ 为一个开放立方体，其中包含中心 $o$、包含和 $x_p$。令$k_p$表示最大的整数$h > 0$，使得$hx_p \in P$（因为$P$是有界框且$x_p \neq o$，$k_p$的存在性遵循阿基米德公理）。 点$k_p x_p$位于紧集$\overline{P}$，因此序列$(k_p x_p)_{p \in \mathbf{N}}$有一个集群点$a \in \overline{P}$。如果$\| (k_p + 1)x_p - a \| \leq \varepsilon$，我们有

$$
\| (k_p + 1)x_p - a \| \leq \varepsilon + \| x_p \|,
$$

并且从$\lim_{p \to \infty} x_p = o$开始，$a$也是序列$((k_p + 1)x_p)$的集群点，其点属于到闭集合$\mathbf{C}P$，通过定义 $k_p$；因而$a \in \overline{P} \cap \mathbf{C}P$（$P$的边界，图5），这意味着$a \neq o$。此外，由于$G$关闭，我们还有$a \in G$。设$t$为任意实数；因为$|tk_p - [tk_p]| < 1$，关系$\| k_p x_p - a \| \leq \varepsilon$意味着$\| [tk_p]x_p - ta \| \leq |t| \varepsilon + \| x_p \|$；由于 $\lim_{p \to \infty} x_p = o$，$ta$ 是

![图5](https://i.imgur.com/5z5z5z5.png)
图 5.

![图6](https://i.imgur.com/6z6z6z6.png)
图 6.

序列 ([tk_p]x_p) 的集群点；但是这个序列属于的点到 G，因而 ta ∈ G，因为 G 是闭集的。这样就完成了证明。

#### 定理 2 {#top-vii-s1-thm-2 .statement tag=0BY9}

设 G 为 $\mathbf{R}^n$、秩 r ($0 \leq r \leq n$) 的闭子群。那么G中包含最大的向量子空间 V；对于每个与 ​​V 互补的向量子空间 W，$W \cap G$ 是离散的，G 是 V 和 $W \cap G$ 的直和。

让我们首先证明V的存在性，证明G中通过o的所有线的并是向量子空间：实际上，这些线的并生成的向量子空间与它们的子群相同生成。 群G是V和$W \cap G$中的直和；对于如果$x \in G$，我们有$x = y + z$，其中$y \in V$和$z \in W$；从$V \subset G$、$z = x - y \in G$开始，因而$z \in W \cap G$。仍有待证明 $W \cap G$ 是离散的；这是从命题 3开始的，因为$W \cap G$是一个封闭的子群，而包含没有线路，因为定义是V。

如果$G \neq V$，我们可以说G是可数无穷线性簇的并，平行于离散群$W \cap G$的V和经过到点（图6）。

如果$p$是向量子空间V的维数，我们有$p \leq r$，$W \cap G$是秩$r - p$的离散群。

#### 推论 1 {#top-vii-s1-thm-2-cor-1 .statement tag=0BYA}

$\mathbf{R}^n$ 存在基 $(a_i)_{1 \leq i \leq n}$，使得
$$
a_i \in G \quad (1 \leq i \leq r), \qquad a_i \in V \quad (1 \leq i \leq p)
$$
使得G是点$\sum_{i=1}^p t_i a_i + \sum_{j=p+1}^r n_j a_j$的集合，其中$t_i$取所有实值，$n_j$取所有整数值。

这是从应用于离散群 $W \cap G$ 的定理 2 和定理 1 或 no. 1 得出的。

#### 推论 2 {#top-vii-s1-thm-2-cor-2 .statement tag=0BYB}

存在$\mathbf{R}^n$的自同构，其中映射G到群$G'$，与$\mathbf{R}^p \times \mathbf{Z}^{r-p}$同构的，它是由$e_1, e_2, \ldots, e_p$和（离散）加法生成的向量子空间的直和子群由$e_{p+1}, e_{p+2}, \ldots, e_r$ 生成。

这是推论 1 的直接的推论。 定理 2 的推论 2 表明$\mathbf{R}^n$ 的闭子群 G 完全由两个整数 $\geq 0$ 确定至同构： 秩，我们用$r(G)$表示，G中包含的最大的向量子空间的维数，我们称为G的维数，用$d(G)$表示。

这些整数必须满足唯一的条件是不等式$0 \leq d(G) \leq r(G) \leq n$。

### 3. 相关子群

令$G$为$\mathbf{R}^n$的任意子群（封闭或非封闭）。考虑点$u = (u_i) \in \mathbf{R}^n$的集合$G^*$，使得对于所有$x = (x_i) \in G$，数$(u|x) = \sum_{i=1}^n u_i x_i$是整数。立即看出$G^*$是$\mathbf{R}^n$的子群；它被称为与 $G$ (*) 关联的子群。如果$G$和$H$是$\mathbf{R}^n$的两个子群使得$H \subset G$，则显然$G^* \subset H^*$。

#### 命题 4 {#top-vii-s1-prop-4 .statement tag=0BYC}

*与$\mathbf{R}^n$的子群$G$关联的子群$G^*$已关闭，我们有$(\overline{G})^* = G^*$。*

对于每个$x \in G$，让$f_x(u)$表示$(u|x)$； $f_x$ 是线性形式，因此是连续的。由于$G^*$是集合$f_x^{-1}(z)$的交，因为$x$贯穿$G$，并且由于这些集合中的每一个都是闭的，因此$G^*$也是闭的。另一方面，如果$u \in G^*$，对于所有$x \in G$，我们有$(u|x) \in \mathbf{Z}$，因此，由于$\mathbf{Z}$在$\mathbf{R}$中闭合，因此对于所有$y \in \overline{G}$，$(u|y) \in \mathbf{Z}$；因此$u \in (G)^*$。但我们有$(\overline{G})^* \subset G^*$（从$G \subset \overline{G}$开始），所以$(\overline{G})^* = G^*$。

当$G$*关闭*时，考虑$G^*$的结构。通过no. 2的推论1到定理2，存在$\mathbf{R}^n$的基$(a_i)_{1 \leq i \leq n}$使得$G$重合与集合为点

$$
x = \sum_{i=1}^p t_i a_i + \sum_{j=p+1}^{p+q} n_j a_j,
$$

其中$t_i$取所有实数值，$n_j$取所有整数值。因此，对于*所有*这些点$x$，$(u|x)$是整数当且仅当$(u|a_i) = 0$对于$1 \leq i \leq p$并且$(u|a_i)$对于$p+1 \leq i \leq p+q$是整数。让我们用 $\mathbf{R}^n$ 的 $(a'_i)_{1 \leq i \leq n}$ 基表示，这样 $(a'_i|a_j) = 0$ 代表 $i \neq j$ 并且

$$
(a'_i|a_i) = 1 \quad \text{for} \quad 1 \leq i \leq n
$$

(*) 这个概念是局部紧致阿贝尔的群的*对偶性*的理论中的一般概念的特殊情况，相应的到群$\mathbf{R}^n$（参见，例如，A. Weil，“L'Integration dans les） 群拓扑和应用”，*Act. Sci. et Ind.* no. 869，Paris，Hermann，1950 年，第 108-109 页）。读者将观察到 $\mathbf{R}^n$ 中关联的子群的属性与向量空间及其对偶的*正交* 向量子空间的属性之间存在密切的类比。

[基“对偶”到$(\mathbf{a}_i)$]；如果我们放入$u = \sum_{i=1}^n u_i a'_i$，很明显，点$u \in G^*$具有以下条件的特征：$u_i = 0$代表$1 \leq i \leq p$，$u_i \in \mathbf{Z}$代表
$$
p + 1 \leq i \leq p + q;
$$
因此$G^*$是向量子空间$W$的直和和$a'_i$的基由……组成使得$p + q + 1 \leq i \leq n$，以及由$a'_i$生成的离散子群使得$p + 1 \leq i \leq p + q$。在其他字中：

#### 命题 5 {#top-vii-s1-prop-5 .statement tag=0BYD}

*对于每个闭合的子群* $G$ *of* $\mathbf{R}^n$，
$$
r(G^*) = n - d(G) \quad \text{and} \quad d(G^*) = n - r(G).
$$
让我们将相同的推理应用到$G^*$。 注意到基对偶$(a'_i)$ 是$(a_i)$，我们看到：

#### 命题 6 {#top-vii-s1-prop-6 .statement tag=0BYE}

*对于每个子群* $G$ *of* $\mathbf{R}^n$，*我们有* $(G^*)^* = \overline{G}$。

#### 推论 {#top-vii-s1-n3-cor-1 .statement tag=0BYF}

*点* $x$ *位于子群* $G$ *of* $\mathbf{R}^n$ *当且仅当* $(u|x)$ *对于所有都为整数* $u \in \mathbf{R}^n$ *使得* $(u|y)$ *对于所有都为整数* $y \in G$。

让我们将位于子群$G$闭包中的点的刻画应用于由典范基$(1 \leq j \leq n)$的$n$向量$e_j$和任意生成的子群$G$的情况数$m$共点$a_i$$(1 \leq i \leq m)$共$\mathbf{R}^n$。说$1 \leq j \leq n$的$(u|e_j)$是整数，意味着$u$的$n$坐标是整数；所以：

#### 命题 7（克罗内克）{#top-vii-s1-prop-7 .statement tag=0BYG}

*设* $a_i = (a_{ij})$ $(1 \leq i \leq m,\ 1 \leq j \leq n)$ *为* $m$ *点为* $\mathbf{R}^n$ *并令* $b = (b_j)$ $(1 \leq j \leq n)$ *为点为* $\mathbf{R}^n$。 *在阶中，对于每个* $\varepsilon > 0$，*存在* $m$ *整数* $g_i$ $(1 \leq i \leq m)$ *和* $n$ *整数* $p_j$ $(1 \leq j \leq n)$ *这样*
$$
|q_1 a_{1j} + q_2 a_{2j} + \cdots + q_m a_{mj} - p_j - b_j| \leq \varepsilon \quad (1 \leq j \leq n)
$$
*对于* $n$ *整数的每个有限序列* $(r_j)$ $(1 \leq j \leq n)$ * 使得* $m$ *数* $\sum_{j=1}^n a_{ij} r_j$ $(1 \leq i \leq m)$ * 都是整数， 数* $\sum_{j=1}^n b_j r_j$ *也应该是整数*。

#### 推论 1 {#top-vii-s1-prop-7-cor-1 .statement tag=0BYH}

*在阶中，对于每个*$x = (x_j)$$(1 \leq j \leq n)$*和每个*$\varepsilon > 0$，*存在*$m$*整数*$q_i$$(1 \leq i \leq m)$*和*$n$*整数* $p_j$ ($1 \leq j \leq n$) *这样*

$$
|q_1 a_{1j} + q_2 a_{2j} + \cdots + q_m a_{mj} - p_j - x_j| \leq \varepsilon \quad (1 \leq j \leq n)
$$

$n$ 整数中不存在有限序列 $(r_j)$，而不是全部零，是充分必要的，使得$m$ 数 $\sum_{j=1}^n a_{ij} r_j$ 中的每一个都是整数。

因为如果$G$在$\mathbf{R}^n$中稠密，即如果$\overline{G} = \mathbf{R}^n$，则$G^* = \{0\}$，反之亦然。

特别是$(m = 1)$：

#### 推论 2 {#top-vii-s1-prop-7-cor-2 .statement tag=0BYI}

*令$\theta_1, \theta_2, \ldots, \theta_n$为$n$实数。在阶中，给定任何$n$实数$x_1, x_2, \ldots, x_n$和实数$\varepsilon > 0$，应该存在整数$q$和$n$整数$p_j$这样*

$$
|q \theta_j - p_j - x_j| \leq \varepsilon \quad (1 \leq j \leq n)
$$

* 不存在形式* $\sum_{j=1}^n r_j \theta_j = h$ 中的关系是必要且充分的，*其中 $r_j$ 是 $n$ 整数不全是零，并且 $h$ 是整数* [这特别意味着$\theta_j$ 和比率$\theta_j / \theta_k$ ($j \neq k$) 必须是*无理数*]。

我们可以这样解释这个结果：对于每个整数$q \in \mathbf{Z}$，让$x_q$表示点，坐标为$q \theta_j - [q \theta_j]$（$1 \leq j \leq n$）； then 推论 2 gives a necessary and sufficient 条件 for 集合 of 点 $x_q$ to be *dense* in the cube which is 乘积 of $n$ 区间 $[0, 1]$ in 因子 of $\mathbf{R}^n$。

#### 命题 8 {#top-vii-s1-prop-8 .statement tag=0BYJ}

*如果$G_1, G_2$是$\mathbf{R}^n$的任何闭子群，我们有*

$$
(G_1 = G_2)^* + G_1^* \cap G_2^* \quad \text{and} \quad (G_1 \cap G_2)^* = G_1^* + G_2^*.
$$

实数 $(u|x + y)$ is 整数 for all $x \in G_1$ and all $y \in G_2$ if and only if $(u|x)$ is 整数 for all $x \in G_1$ and $(u|y)$ is 整数 for all $y \in G_2$, because $(u|x + y) = (u|x) + (u|y)$；因而

$$
(G_1 + G_2)^* = G_1^* \cap G_2^*
$$

for any two 子群 $G_1, G_2$ of $\mathbf{R}^n$. If now we suppose that $G_1$ and $G_2$ are closed, we have $(G_1^* + G_2^*)^* = G_1 \cap G_2$ by 命题 6;因而，再次取相关的子群和应用命题 6，

$$
(G_1 \cap G_2)^* = \overline{G_1^* + G_2^*}.
$$

#### 注 {#top-vii-s1-n3-rem-1 .statement tag=0BYK}

Let $G_1, G_2$ be two *lattices* in $\mathbf{R}^n$ (no. 1) such that $G_2 \subset G_1$: then (命题 5) $G_1^*$ and $G_2^*$ are *lattices* in $\mathbf{R}^n$ such that $G_1^* \subset G_2^*$.我们在no. 1中看到，存在整数$m > 0$使得$m G_1 \subset G_2$；

因而，对于$x \in G_1$和$u \in G_2^*$，我们有$m(u|x) \in \mathbf{Z}$，因此有$(u|x) \in \mathbf{Q}$。 If $x \in G_2$ and $u \in G_2^*$, or if $x \in G_1$ and $u \in G_1^*$, we have $(u|x) \in \mathbf{Z}$ by 定义. Consequently on 经过 to 商 the $\mathbf{Z}$-bilinear 映射 $(x, u) \to (u|x)$ of $G_1 \times G_2^*$ into $\mathbf{Q}$ 定义 a $\mathbf{Z}$-bilinear 映射 $B$ of $(G_1/G_2) \times (G_2^*/G_1^*)$ 变为$\mathbf{Q}/\mathbf{Z}$。此外，很明显，如果$\bar{x}_0 \in G_1/G_2$（或$\bar{u}_0 \in G_2^*/G_1^*$）是这样的，对于*每个* $\bar{u} \in G_2^*/G_1^*$（或每个$\bar{x} \in G_1/G_2$）我们有

$$
B(\bar{x}_0, u) = 0 \quad [\text{resp. } B(\bar{x}, \bar{u}_0) = 0],
$$

那么必然是$\bar{x}_0 = 0$（或$\bar{u}_0 = 0$）。由此可见，$G_2^*/G_1^*$的$\mathbf{Z}$线性*双射* $h$位于$G_1/G_2$的*对偶*上，使得$\langle \bar{x}, h(\bar{u}) \rangle = B(\bar{x}, \bar{u})$适用于$\bar{x} \in G_1/G_2$和$\bar{u} \in G_2^*/G_1^*$；特别是，有限群$G_1/G_2$和$G_2^*/G_1^*$是*同构的*。

### 4. 豪斯多夫商群 $\mathbf{R}^n$

$\mathbf{R}^n$ 的每个 Hausdorff 商群都是形式 $\mathbf{R}^n/H$，其中 $H$ 是 $\mathbf{R}^n$ 的闭子群（章 III, § 2, no. 6，命题 18）。到no. 3的推论2、定理2，存在$\mathbf{R}^n$的自同构$f$，其中变换$H$变成子群$H'$、直和典范基的向量$e_i$的$p$生成向量子空间以及$n - p$剩余的向量的$g$生成的离散群

$$
e_i, \quad 0 \leq p + q \leq n.
$$

经过至商、$\mathbf{R}^n/H$的$f$诱导同构至$\mathbf{R}^{n-p-q} \times T^q$（章III, § 2, no. 8、注3）；现在，$\mathbf{R}^n/H'$与$\mathbf{R}^{n-p-q} \times T^q$同构的（章III, § 2, no. 9、推论到命题26）。最后：

#### 命题 9 {#top-vii-s1-prop-9 .statement tag=0BYL}

*$\mathbf{R}^n$ 的每个 Hausdorff 商群都同构于乘积群* $\mathbf{R}^h \times T^k$ ($0 \leq h + k \leq n$)。

乘积空间 $T^n$（滥用语言，拓扑群 $T^n$）被称为*n维环面*；通过章 V, § 1, no. 2 的命题 4，$T^n$ 是紧凑、连通且局部连通的。

此外，如果$C$表示$\mathbf{R}^n$中第1边的封闭立方体，则$T^n$通过点之间的等价关系“$x_i \equiv y_i \pmod{1}$（$1 \leq i \leq n$）”与$C$的商空间同胚$C$的$x = (x_i)$和$y = (y_i)$。因而$T^n$是由立方体$C$通过“相对面的识别”形成的。

#### 命题 10 {#top-vii-s1-prop-10 .statement tag=0BYM}

*拓扑群* $T^n$ *局部同构于* $R^n$。

因为$T^n = (R/Z)^n$与$R^n/Z^n$同构的（章III, § 2, no. 9，推论到命题26），$Z^n$是$R^n$的离散子群（章III, § 2, no. 6，命题） 19）。

由此可见群 $R^p \times T^{n-p}$ 都局部同构于 $R^n$ ($0 \geq p \geq n$)；在§ 2, no. 2中，我们将看到它们是唯一具有此性质的*连接*群。

### 5. 子群和商群的 $T^n$

让我们用$R^n/Z^n$来计算认同$T^n$，并让$\varphi$是$R^n$的典范同态到$R^n/Z^n$。 $T^n$的每个子群都是形式$G = \varphi(H)$，其中$H$是$R^n$的子群，其中包含$Z^n$并且同构于$H/Z^n$（章） III, § 2, no. 7、命题20)；为了使$G$在$T^n$中“关闭”，$H$在$R^n$中关闭是必要且充分的（章I, § 3, no. 4）。因而，在阶中，要找到$T^n$的闭子群，我们必须确定所有$R^n$的闭子群$H$，其中包含$Z^n$；为此，我们需要 no. 3 中的应用命题 6，并且我们首先确定与 $H$ 关联的子群 $H^*$。由于 $Z^n$ 与其自身相关联，因此我们有 $H^* \subset Z^n$；因而(no. 1)存在$R^n$的基$(a_i)_{1 \leq i \leq n}$，其中生成$Z^n$，以及$H^*$的基(相对于环$Z$)由……组成 $p$ 点 $b_i$ ($1 \leq i \leq p$) 使得$b_i = e_i a_i$ ($1 \leq i \leq p$)，其中$e_i$ 是整数满足 $e_{i+1} \equiv 0 \pmod{e_i}$ 与$1 \leq i \leq p-1$ 的同余。设$(a'_i)$是基对数$(a_i)$；那么$u = \sum_{i=1}^n u_i a_i$属于到$(H^*)^* = H$当且仅当$u_i e_i \in Z$对于$1 \leq i \leq p$；在其他字中，$H$是$a'_{p+1}, \ldots, a_n$生成的向量子空间$V$的直和，以及$p$点生成的离散子群$K$
$$
e_i^{-1} a'_i \quad (1 \leq i \leq p).
$$
另一方面，$Z^n$是$V \cap Z^n$和$K \cap Z^n$的直和，因为$a'_i$($1 \leq i \leq n$)生成$Z^n$。因而，商群$H/Z^n$同构于$(V/(V \cap Z^n)) \times (K/(K \cap Z^n))$（章III, § 2, no. 9，推论到命题26）； $V/(V \cap Z^n)$与$T^{n-p}$同构的，$K/(K \cap Z^n)$分别是群、直和、$p$循环群、阶、$e_i$ ($1 \leq i \leq p$) （cf.no. 1）。

使用相同的记号，$T^n$的每个Hausdorff商群都是形式$T^n/\varphi(H)$并且同构于$R^n/H$（章III, § 2, no. 7，推论到命题22）；如果$W$是$K$生成的向量子空间，$R^n/H$同构于$W/K$（章III, § 2, no. 9，推论到命题26），即$T^p$。至和以上：

命题II。 ** $\mathbf{T}^n$ *的每个闭子群同构于以下形式的群* $\mathbf{T}^h \times F$ *(0 \leq h \leq n)* *其中* $F$ *是有限阿贝尔群，使得* $F$ *为直和的循环子群的最小数量为* $\leq n - h$。 ** $\mathbf{T}^n$ * 的每个 Hausdorff 商群 * 都同构于形式* $\mathbf{T}^h$ *(0 \leq h \leq n)* 的群。

特别是（$n = 1$）：

#### 推论 {#top-vii-s1-n5-cor-1 .statement tag=0BYN}

** $\mathbf{T}$ 的每个闭子群，*除了* $\mathbf{T}$ *本身，都是有限循环群。* ** $\mathbf{T}$ 的每个 Hausdorff 商群，*除了* $\{0\}$，*同构于* $\mathbf{T}$。

### 6. 定期函数

定义I。 *函数* $f$，*定义在* $\mathbf{R}^n$，*与值在任意集合* $E$，*如果存在点* $a \neq 0$ *在* $\mathbf{R}^n$ *这样*

$$
f(x + a) = f(x)
$$

*对于所有人*$x \in \mathbf{R}^n$。 *如果* $f$ *是周期性的，则每个点* $a \in \mathbf{R}^n$ *其中关系* (1) *是* $x$ *中的恒等式，称为* $f$的周期。

周期函数$f$的所有周期的集合$G$显然是加法群$\mathbf{R}^n$的*子群*（到假设不只由0组成）。如果$f$是$\mathbf{R}^n$的*连续*周期映射到*豪斯多夫*拓扑空间$E$，则其周期$G$的群是*闭*的。因为如果 $G_x$ 表示所有 $a \in \mathbf{R}^n$ 中的集合，使得 $f(x + a) = f(x)$ 对于*给定点* $x \in \mathbf{R}^n$，则 $G$ 是 $G_x$ 的交，因为 $x$ 贯穿$\mathbf{R}^n$，每个$G$都是*封闭*（章I, § 8, no. 1，命题2）。令$V$为最大的向量子空间包含在$G$中（no. 2，定理2）； 函数 $f$ 在每个陪集 mod $V$ 上都是*常数*；如果$W$是向量子空间与$V$互补，则$f$由其限制到$W$确定。在其他字（对于某些$p$，$W$是与$\mathbf{R}^p$同构的拓扑群），对$\mathbf{R}^n$上连续周期函数的研究被简化为对周期为群的函数的研究$G$ 是*离散*；如果这个群是秩$g$，函数$f$被称为*q-ply周期性*，并且$q$点的每个空闲系统其中生成$G$被称为*第 $f$ 期*的本金系统。

如果$(a_i)$和$(b_i)$是$f$周期的两个主要系统，我们已经看到（no. 1），每个都可以通过整数系数和行列式$\pm 1$的线性变换从另一个获得。

设$\varphi$是$\mathbf{R}^n$的典范映射到$\mathbf{R}^n/G$；将 $\mathbf{R}^n/G$ 的每映射 $g$ 转换为集合 $E$ 对应函数 $\dot{g} = g \circ \varphi$，这是一个周期映射将 $\mathbf{R}^n$ 转换为 $E$，有群个周期其中包含$G$；相反，$\mathbf{R}^n$ 到 $E$ 的每个映射都有群个周期包含 $G$ 属于这个形式，因为它与关系 $x \equiv y \pmod{G}$ (集合) 兼容理论、R、、no. 7）。这样我们就可以将$\mathbf{R}^n/G$的所有映射的集合的定义双射映射$g \to \dot{g}$转化为$E$到$\mathbf{R}^n$的所有映射的集合转化为$E$其中群个周期包含 $G$。为了使$\dot{g}$连续（$E$是拓扑空间），$g$连续是必要且充分的（章I, § 3, no. 4，命题6）

### 习题{#top-vii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
