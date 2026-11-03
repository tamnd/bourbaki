---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 7
section_title: Limits
lang: zh
source: top-i-iv
book_pages: 68-74, 132-133
pdf_pages: 0074-0080, 0138-0139
extraction: ocr
subsections:
    - "no": 1
      title: LIMIT OF A FILTER
      page: 68
      pdf_page: 74
    - "no": 2
      title: CLUSTER POINT OF A FILTER BASE
      page: 69
      pdf_page: 75
    - "no": 3
      title: LIMIT POINT AND CLUSTER POINT OF A FUNCTION
      page: 70
      pdf_page: 76
    - "no": 4
      title: LIMITS AND CONTINUITY
      page: 72
      pdf_page: 78
    - "no": 5
      title: LIMITS RELATIVE TO A SUBSPACE
      page: 73
      pdf_page: 79
    - "no": 6
      title: LIMITS IN PRODUCT SPACES AND QUOTIENT SPACES
      page: 74
      pdf_page: 80
statements: 23
exercises: 7
content_sha256: 43c1cf70eabea30dca6ab37cefe631d6984e6f68ca59d0c70584c9aa3950239c
translated_from: content/en/top/I/07_s7_limits.md
translation_method: google
source_content_sha256: 2a27ef734a6a1ff91fe8d3fb848961a85b666a83e64858598552c6dd593c2d9d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 5f129749452ee1bfa1f407af92da77b2bc1a02b646f4c9a350a5be1840796bda
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 7. 极限

### 1. 过滤器的极限

#### 定义 1 {#top-i-s7-def-1 .statement tag=0B5B}

令$X$为拓扑空间，$\mathfrak{F}$为$X$上的过滤器。 点$x \in X$据说是$\mathfrak{F}$的极限点（或简称极限），如果$\mathfrak{F}$是更细比邻域过滤$x$的$\mathfrak{B}(x)$； $\mathfrak{F}$ 也被称为收敛（或将收敛）到 $x$。 *点* $x$ *据说是滤波器基* $\mathfrak{B}$ *在* $X$上的极限，*并且* $\mathfrak{B}$ *据说收敛到* $x$，*如果滤波器的基是* $\mathfrak{B}$ *收敛到* $x$。

这个定义与 § 6, no. 3 的命题 4 一起给出以下标准：

#### 命题 1 {#top-i-s7-prop-1 .statement tag=0B5C}

*过滤基* $\mathfrak{B}$ *在拓扑空间* $X$ *收敛到* $x$ *当且仅当* $x$ *邻域基本系统的每组都包含一组* $\mathfrak{B}$。

根据§ 1, no. 2中引入的术语，我们可以用以下方式陈述命题1：当且仅当$\mathfrak{B}$有集合*尽可能接近*$x$时，$\mathfrak{B}$收敛于$x$。

如果过滤器$\mathfrak{F}$收敛到$x$，则由于定义 1，每个过滤器*更细*比$\mathfrak{F}$也会收敛到$x$。同样，如果$X$的拓扑被*粗略*拓扑替换， $x$的邻域过滤器被*粗化*过滤器（$\S$2、no. 2、命题3）取代，因此在这个新的拓扑中$\mathfrak{F}$仍然收敛到$x$。

因此我们可以说*更细拓扑，这个拓扑*中的收敛滤波器越少。特别是，在离散拓扑中，唯一的收敛滤波器是邻域滤波器，因为这些是$X$（$\S$6，no. 4）上的普通超滤波器。

令$\Phi$为$X$上滤波器的集合，所有这些都收敛到相同的点$x$； 邻域过滤器$\mathfrak{B}(x)$比$\Phi$的所有过滤器更粗糙，因此也比这些过滤器的*交*$\mathfrak{J}$更粗糙；在其他字中，$\mathfrak{J}$也收敛于$x$。

#### 命题 2 {#top-i-s7-prop-2 .statement tag=0B5D}

*过滤器* $\mathfrak{F}$ *在拓扑空间* $X$ *收敛到点* $x$ *当且仅当每个更细比* $\mathfrak{F}$ *收敛到* $x$。

这是前面的注的直接的推论和§ 6, no. 4的命题7。

一般来说，一个过滤器可以有*几个不同的极限点*；我们将在§ 8, no. 1回到这个问题。

### 2. 过滤器基的集群点

#### 定义 2 {#top-i-s7-def-2 .statement tag=0B5E}

*在拓扑空间* $X$中，*点* $x$ *是过滤器基* $\mathfrak{B}$ *在* $X$ *上的集群点，如果它位于* $\mathfrak{B}$的所有集合的闭包中。

如果$x$是过滤器基$\mathfrak{B}$的集群点，则由于§ 6, no. 3、推论到命题4，它也是每个“等效”过滤器基的集群点；特别地，$x$是*过滤器*的集群点，其基是$\mathfrak{B}$。

#### 命题 3 {#top-i-s7-prop-3 .statement tag=0B5F}

*点 x 是滤波器基 B 的簇点当且仅当 x 的邻域的基本系统的每个集合满足 B 的每个集合。*

这立即从定义开始。

§ 6, no. 2的命题和推论2到命题1表明，性质“x是过滤器$\mathfrak{F}$的簇点”相当于性质“有一个比两者都更细的过滤器” x”的$\mathfrak{F}$和邻域过滤器。其他字：

#### 命题 4 {#top-i-s7-prop-4 .statement tag=0B5G}

*点 x 是过滤器$\mathfrak{F}$的簇点当且仅当存在一个过滤器更细比$\mathfrak{F}$收敛到x时。*

特别是，过滤器$\mathfrak{F}$的每个*极限点*都是$\mathfrak{F}$的*集群点*。

#### 推出 {#top-i-s7-n2-cor-1 .statement tag=0B5H}

*当且仅当 x 是 $\mathfrak{U}$ 的簇点时，ultrafilter $\mathfrak{U}$ 收敛于点 x。*

如果 x 是过滤器$\mathfrak{F}$的集群点，那么它也是每个比$\mathfrak{F}$*粗糙*的过滤器的集群点；同样，如果我们通过*粗略* 拓扑对X进行替换拓扑，则x在新的拓扑中仍然是$\mathfrak{F}$的点集群。

X 上的过滤器基 $\mathfrak{B}$ 的集群点的集合由定义集合 $\bigcap_{M \in \mathfrak{B}} \overline{M}$、从而组成

#### 命题 5 {#top-i-s7-prop-5 .statement tag=0B5I}

*拓扑空间X上过滤器基的集群点的集合在X中闭合。*

#### 命题 6 {#top-i-s7-prop-6 .statement tag=0B5J}

*令$\mathfrak{B}$为拓扑空间X的子集A上的过滤器基。然后X属于到$\overline{A}$中$\mathfrak{B}$的每个簇点；相反，$\overline{A}$ 的每个点都是 A 上过滤器的极限点。*

第一个断言是微不足道的；另一方面，如果$x \in \overline{A}$，则X中x的邻域滤波器在A上的迹是A上的滤波器，显然收敛于x。

#### 注 {#top-i-s7-n2-rem-1 .statement tag=0B5K}

拓扑空间上的过滤器不需要集群点（并且*更不必说*没有极限点）；例如，在*无限离散空间*中，有限子集的补集过滤器没有簇点。 空间，其中每个滤波器都有一个簇点，在数学中发挥着重要作用，我们将在§ 9中研究它们。

### 3. 极限点以及函数的集群点

#### 定义 3 {#top-i-s7-def-3 .statement tag=0B5L}

*设f为集合X的映射到拓扑空间Y，并令$\mathfrak{F}$为X上的过滤器。如果 y 为极限点（或简称为极限），则相对于过滤器 $\mathfrak{F}$，点 $y \in Y$ 被认为是 f 的极限点（或简称为极限）（分别为点）（分别为点）。过滤器基$f(\mathfrak{F})$的簇点）。*

关系“y 是 f 相对于过滤器 $\mathfrak{F}$ 的极限”如果不存在混淆的风险，则写作 $\lim_{\mathfrak{F}} f = y$、或$\lim_{x, \mathfrak{F}} f(x) = y$、或$\lim_x f(x) = y$。

从定义 3 和命题 1 (no. 1) 和 3 (no. 2) 我们推导出以下判据：

#### 命题 7 {#top-i-s7-prop-7 .statement tag=0B5M}

*点$y \in Y$相对于过滤器$\mathfrak{F}$是$f$的极限当且仅当，对于$Y$中$y$的每个邻域$V$，有集合 $M \in \mathfrak{F}$使得$f(M) \subset V$（即$\overline{f}(V) \in \mathfrak{F}$对应邻域$V$/$y$）。*
*点$y \in Y$是$f$相对于$\mathfrak{F}$的集群点当且仅当对于$y$的每个邻域$V$和每个$M \in \mathfrak{F}$都有点 $x \in M$ 这样 $f(x) \in V$.*

#### 例 1 {#top-i-s7-n3-exa-1 .statement tag=0B5N}

拓扑空间的点$(x_n)_{n \in \mathbf{N}}$序列是$\mathbf{N}$映射$n \to x_n$到$X$。在数学分析中，人们经常使用极限点的概念和映射的集群点*相对于$\mathbf{N}$上的Fréchet滤波器*（§ 6, no. 1）；如果相对于 Fréchet 滤波器，$y$ 是 $n \to x_n$ 的极限，则$y$ 被称为序列* $(x_n)$ *极限 *因为 n 趋于无穷大*，我们写为 $\lim_{n \to \infty} x_n = y$。相对于 Fréchet 滤波器，映射 $n \to x_n$ 的集群点称为序列* $(x_n)$ 的 *集群点。

因此，如果点 $y \in X$ 是与* $(x_n)$ (§ 6, no. 8) 伴随的*基本过滤器的限制点（或簇点），则它是 $X$ 点的序列 $(x_n)$ 的限制点（或簇点）。

点$y$是$X$中序列$(x_n)$的极限当且仅当，对于$X$中$y$的*每个*邻域$V$，*除了有限的数之外序列* $(x_n)$ *中的项在* $V$中，即存在整数 $n_0$，使得所有$n \geq n_0$都有$x_n \in V$。同样，$y$是序列$(x_n)$的集群点当且仅当，对于$X$中$y$的*每个*邻域$V$和*每个*整数$n_0$，有整数$n \geq n_0$使得$x_n \in V$。

#### 例 2 {#top-i-s7-n3-exa-2 .statement tag=0B5O}

更一般地，令$f$是*有向*集合$A$到拓扑空间$X$的映射。如果相对于$A$的*截面过滤器*，$x \in X$是$f$的极限（分别是簇点），则$x$被称为*极限*（分别是*簇点*） $f$ *相对于有向集合* $A$，我们写为$x = \lim_{z \in A} f(z)$。

如果相对于$X$上的过滤器$\mathfrak{F}$，$y$是映射$f : X \to Y$的极限（分别是集群点），则$y$仍然是$f$的极限（分别是集群点）相对于$\mathfrak{F}$，如果我们通过*粗略*拓扑对$Y$进行替换拓扑，或者如果我们通过*更细*（或*粗略*）过滤器对替换进行过滤$\mathfrak{F}$。

#### 命题 8 {#top-i-s7-prop-8 .statement tag=0B5P}

*令$f$为集合$X$的映射变成拓扑空间$Y$；那么$y \in Y$是$f$相对于$\mathfrak{F}$的集群点当且仅当$X$上有一个过滤器$\mathfrak{G}$，它比$\mathfrak{F}$更细并且$y$是$f$的极限关于$\mathfrak{G}$.*

因为如果$y$是$f$相对于$\mathfrak{F}$的集群点，并且如果$\mathfrak{B}$是$y$的邻域过滤器，则$\overline{f}^{-1}(\mathfrak{B})$是$X$上的过滤器基，因为每集合 $\overline{f}^{-1}(\mathfrak{B})$ 满足$\mathfrak{F}$ (§ 6, no. 6) 中的每一个集合。这个注还表明$X$上有一个过滤器$\mathfrak{G}$，它比$\mathfrak{F}$和带有基$\overline{f}^{-1}(\mathfrak{B})$的过滤器更细（§ 6, no. 2，命题1，推论2），因此$y$相对于$\mathfrak{G}$是$f$的极限点。

最后注意，如果$f$是集合$X$的映射进入拓扑空间$Y$，集合属于$f$的集群点相对于过滤器$\mathfrak{F}$ $X$ 在 $Y$（no. 2、命题 5）中*关闭*，并且可能是空的。

#### 注 {#top-i-s7-n3-rem-1 .statement tag=0B5Q}

如果相对于$X$上的过滤器$\mathfrak{F}$，$y \in Y$是映射$f : X \to Y$的极限（分别是点），那么$y$也是每个的极限（分别是点） 函数 $g : X \to Y$ 与 $f$ 相对于 $\mathfrak{F}$ (§ 6, no. 9) 具有*相同的胚芽*；相对于$\mathfrak{F}$，$y$ 据说是*极限*（分别是*簇点*）*胚芽*$\tilde{f}$**$f$。

### 4. 极限和连续性

设$X, Y$为点$a \in X$$X$中$X$、$Y$、$\mathfrak{B}$邻域的两个拓扑空间、$f$映射过滤。我们使用特殊的记号，而不是$y \in Y$是$f$的极限相对于过滤器$\mathfrak{B}$并写入$y = \lim_{\mathfrak{B}} f$，而不是说

$$
y = \lim_{i \in I} f(x),
$$

我们说$y$是*$f$*在点*$a$的*极限，或者说$f(x)$*倾向于*$y$*作为*$x$*倾向于*$a$。类似地，$y$是$f$相对于$\mathfrak{B}$的集群点，而不是说，我们说$y$*是点*的集群点*$f$*在点* $a$。

考虑定义的连续性 (§ 2, no. 1, 定义 1) 命题 7 of no. 3 表明：

#### 命题 9 {#top-i-s7-prop-9 .statement tag=0B5R}

*映射* $f$ *拓扑空间* $X$ *到拓扑空间* $Y$ *在点* $a \in X$ *当且仅当* $\lim_{i \in I} f(x) = f(a)$ 处连续。

#### 推论 1 {#top-i-s7-prop-9-cor-1 .statement tag=0B5S}

*设*$X, Y$*为*$X$*的两个拓扑空间、$f$映射*入*$Y$*，在点*$a \in X$连续； *然后，对于每个过滤器基* $\mathfrak{B}$ *在* $X$ *上收敛到* $a$，*过滤器基* $f(\mathfrak{B})$ *收敛到* $f(a)$。 *相反，如果对于每个超滤器* $\mathfrak{U}$ *在* $X$ *收敛到* $a$，*超滤器基* $f(\mathfrak{U})$ *收敛到* $f(a)$，*则* $f$ *在* $a$ 处连续。

第一个断言是命题9的直接的推论。为了证明第二个$f$在$a$不连续；那么Y中存在$f(a)$的邻域W，使得$\overline{f}^{-1}(W)$不属于到X中$a$的邻域的过滤器$\mathfrak{B}$。因此 (§ 6, no. 4, 命题 7) 存在超滤器$\mathfrak{U}$, 更细，而不是$\mathfrak{B}$，而包含$\overline{f}^{-1}(W)$，因此包含其补码$A = X - \overline{f}^{-1}(W)$ (§ 6, no. 4, 命题) 5);由于$f(A) \cap W = \varnothing$，$f(\mathfrak{U})$不会收敛到$f(a)$。

#### 推论 2 {#top-i-s7-prop-9-cor-2 .statement tag=0B5T}

*设g为集合Z的映射，形成拓扑空间X，其相对于Z上的过滤器$\mathfrak{F}$有极限a；那么如果映射 $f : X \to Y$ 在 a 处连续，则合成 $f \circ g$ 的 $f(a)$ 相对于 $\mathfrak{F}$ 具有极限点。*

### 5. 极限相对于子空间

令X、Y为两个拓扑空间，令A为X的子集，令$a \in X$为A的*闭包*的点（但不一定在A中）。令$\mathfrak{F}$为X中$a$的邻域过滤器A上的*迹*。如果$f$是A到Y的映射，那么$y \in Y$相对于$\mathfrak{F}$并写成$y = \lim_{\mathfrak{F}} f$，而不是说，而是$f$的极限，我们写

$$
y = \lim_{x \to a, x \in A} f(x)
$$

我们说 $y$ 是 f 在 a 处的 *极限，相对于子空间* A，或者说 $f(x)$ *趋向 y，因为 x 趋向于 a，而留在* A 中。那么我们有 $y \in f(A)$。

如果 $A = \mathbf{C}\{a\}$ 其中 $a$ *不是* X 的孤立点，那么我们写

$$
y = \lim_{x \to a, x \neq a} f(x)
$$

而不是$y = \lim_{x \to a, x \in A} f(x)$。

我们对簇点进行类似的定义。

如果$f$是映射$g : X \to Y$到A的*限制*，我们说$g$有极限（分别是簇点）$y$相对于A在点$a \in \overline{A}$，如果$y$是 $a$ 处$f$ 的极限（分别是簇点），相对于 A。

令 B 为 A 的子集，令 $a \in X$ 为 B 闭包的点；如果$y$是$a$处的极限，*相对于*A，映射$f : A \to Y$，则$y$也是$f$在$a$处的极限，*相对于*B； 逆命题不一定是真的。

但是，如果 V 是点 $a \in \overline{A}$ X 中的 *邻域*，并且如果 $f$ 在 $a$ 处有极限 $y$，*相对于* $V \cap A$，则$y$ 仍然是 $f$ 在 $a$ 的极限，*相对于* A。

设$a$是X的*非孤立*点，因此$a$位于$\mathbf{C}\{a\}$的闭包中。那么映射$f : X \to Y$在*$a$*连续当且仅当我们有$f(a) = \lim_{x \to a, x \neq a} f(x)$；这紧随定义而来。

### 6. 极限乘积空间和商空间

#### 命题 10 {#top-i-s7-prop-10 .statement tag=0B5U}

令$X$为集合，令$(Y_i)_{i \in I}$为空间的拓扑族，对于每个$i \in I$，令$f_i$为$X$到$Y_i$的映射。让 $X$ 被赋予最粗糙的拓扑 $\mathfrak{T}$，其中 $f_i$ 是连续的。那么，对于$X$上的滤波器$\mathfrak{F}$收敛到$a \in X$的必要且充分的条件是，对于每个$i \in I$，滤波器基$f_i(\mathfrak{F})$应该收敛到$Y_i$中的$f_i(a)$。

条件是必要的，因为 $f_i$ 是连续的（no. 4、命题 9、推论 1）。相反，假设满足条件，并令$V$为$a$在$X$中的开邻域。通过$\mathfrak{T}$的定义（§ 2, no. 3，命题 4），存在$I$的有限子集$J$，并且对于每个$i \in J$，有$Y_i$的开子集$U_i$，这样$f_i(a) \in U_i$ $i \in J$ $V$ 包含集合
$$
\bigcap_{i \in J} f_i^{-1}(U_i).
$$
假设意味着 $f_i^{-1}(U_i) \in \mathfrak{F}$ (no. 3, 命题 7)；由于 $J$ 是有限的，因此
$$
M = \bigcap_{i \in J} f_i^{-1}(U_i)
$$
属于至$\mathfrak{F}$和$M \subset V$。这样就完成了证明。

#### 推论 1 {#top-i-s7-prop-10-cor-1 .statement tag=0B5V}

乘积空间 $X = \prod_{i \in I} X_i$ 上的滤波器$\mathfrak{F}$ 收敛到点 $x$ 当且仅当对于每个$i \in I$，滤波器基 $\operatorname{pr}_i(\mathfrak{F})$ 收敛到$\operatorname{pr}_i(x)$。

#### 推论 2 {#top-i-s7-prop-10-cor-2 .statement tag=0B5W}

令$f = (f_i)$为集合$X$的映射变成乘积空间$Y = \prod_{i \in I} Y_i$。那么$f$相对于$X$上的过滤器$\mathfrak{F}$具有极限$y = (y_i)$当且仅当对于每个$i \in I$$f_i$相对于$\mathfrak{F}$具有极限$y_i$。

#### 命题 11 {#top-i-s7-prop-11 .statement tag=0B5X}

令$R$为拓扑空间$X$上的开等价关系，并令$\varphi$为典范映射$X \to X/R$。然后，对于每个$x \in X$和$X/R$上的每个过滤器基$\mathfrak{B}'$收敛到$\varphi(x)$，$X$上有一个过滤器基$\mathfrak{B}$收敛到$x$并且$\varphi(\mathfrak{B})$是等价的到$\mathfrak{B}'$。

如果$U$是$X$中$x$的任意邻域，则$\varphi(U)$是$X/R$中$\varphi(x)$的邻域（§ 5, no. 3，命题5），因此有集合 $M' \in \mathfrak{B}'$使得$M' \subset \varphi(U)$；如果我们放入$M = U \cap \varphi^{-1}(M')$，则$M' = \varphi(M)$。这表明，当$M'$穿过$\mathfrak{B}'$并且$U$穿过$x$的邻域过滤器时，集合$U \cap \varphi^{-1}(M')$形式过滤器基$\mathfrak{B}$在$X$上；显然$\mathfrak{B}$收敛于$x$，并且$\varphi(\mathfrak{B})$等价于$\mathfrak{B}'$。

### 习题 {#top-i-s7-exercises}

参见[习题为 § 7](exercises/s7/)。
