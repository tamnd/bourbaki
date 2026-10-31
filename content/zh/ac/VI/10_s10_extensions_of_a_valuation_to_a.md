---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 10
section_title: Extensions of a valuation to a transcendental extension
lang: zh
source: ac-i-vii
book_pages: 434-440, 471-473
pdf_pages: 0452-0458, 0489-0491
extraction: ocr
subsections:
    - "no": 1
      title: THE CASE OF A MONOGENOUS TRANSCENDENTAL EXTENSION
      page: 434
      pdf_page: 452
    - "no": 2
      title: THE RATIONAL RANK OF A COMMUTATIVE GROUP
      page: 437
      pdf_page: 455
    - "no": 3
      title: THE CASE OF ANY TRANSCENDENTAL EXTENSION
      page: 438
      pdf_page: 456
statements: 14
exercises: 2
content_sha256: b463b8d48b460735a39c4c1162972ec52d47ba9d1d9d3e062821987b15c067f7
translated_from: content/en/ac/VI/10_s10_extensions_of_a_valuation_to_a.md
translation_method: google
source_content_sha256: d3545f7135c1b975d777e05ac5e9cc067935aed03dd234e1d2fffc43e8d3d49f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: f21bab5d2b31c6bd3eefb542dfebf6f7ccc578db9f64ecda7099ce11701f5ffe
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 10. 扩张对超越扩张的评价

### 1.单一超越论扩张的案例

#### 引理 1 {#ac-vi-s10-lem-1 .statement tag=04Y5}

令 $K$ 为 *域*，$v$ 右 $K$、$\Gamma$ *其* 阶群、$\Gamma'$ 的全序群包含 $\Gamma$ 和 $\xi$ *元素*$\Gamma'$。在*$K(X)$上存在*一个*独特的估值，例如*那个*，*对于*$P = \sum_j a_j X^j$（$a_j \in K$），$w(P) = \inf_j (v(a_j) + j\xi)$。

命题 4 of § 3, no. 2，足以证明公式

$$
w\left( \sum_j a_j X^j \right) = \inf_j (v(a_j) + j\xi)
$$

定义的估值为环$K[X]$。作为

$$
v(a_j + b_j) + j\xi \geq \inf(v(a_j), v(b_j)) + j\xi = \inf(v(a_j) + j\xi, v(b_j) + j\xi),
$$

由此可见

$$
w(P + Q) \geq \inf(w(P), w(Q))
$$

对于$K[X]$中的$P, Q$，如果$w(P) \neq w(Q)$则保持等式。我们表明

$$
w(PQ) = w(P) + w(Q)
$$

对于 $P = \sum a_j X^j$ 和 $Q = \sum b_j X^j$。令 $i$（分别为 $k$）为整数 $j$ 中的最小值，使得 $v(a_j) + j\xi$（分别为 $v(b_j) + j\xi$）达到其最小值；让$a$（或$\beta$）表示这个最小值。对于$\mathbf{N}$中的$j, j'$，

$$
w(a_j b_{j'} X^{j+j'}) = v(a_j) + j\xi + v(b_{j'}) + j'\xi \geq a + \beta,
$$

从而 $w(PQ) \geq a + \beta$ 由 (2) 得出。现在考虑$PQ$中次数$i + k$的项$c X^{i+k}$；然后$c = \sum_{n \in \mathbf{Z}} a_{i+n} b_{k-n}$；由$i$和$k$中的选择、元素

$$
w(a_{i+n} b_{k-n} X^{i+k}) = v(a_{i+n}) + (i+n)\xi + v(b_{k-n}) + (k-n)\xi
$$

一次且仅一次使用 $n = 0$ 取最小值值 $a + \beta$；因此 $w(c X^{i+k}) = a + \beta$, 从而, 由 (1),

$$
w(PQ) = \alpha + \beta = w(P) + w(Q).
$$

#### 命题 1 {#ac-vi-s10-prop-1 .statement tag=04Y6}

令 $K$ 为 *域*、$v$ *评估* $K$、$\Gamma$ *其阶群*、$\Gamma'$ *全序群包含* $\Gamma$ *和* $\xi$*元素*$\Gamma'$*使得关系*$n\xi \in \Gamma, n \in \mathbf{Z}$*意味着*$n = 0$。那么存在*一个*独特的估值w *在* $K(X)$ *与值在* $\Gamma'$ *并延伸* $v$ *这样* $w(X) = \xi$。 * w *的*剩余类域等于*$v$*的*阶群是*$\Gamma'$的子群*$\Gamma + \mathbf{Z}\xi$*。

我们展示w的第一个唯一性。令 $P = \sum_j a_j X^j$ 为 $K[X]$ 的元素。然后是$w(a_j X^j) = v(a_j) + j\xi$，它表明单项式$a_j X^j$使得$a_j \neq 0$对于w具有不同的值。由此得出 $w(P) = \inf_j (v(a_j) + j\xi)$，它既显示了 w 在 $K[X]$ 上的唯一性（因此也在 $K(X)$ 上），也显示了 w 的阶群是 $\Gamma + \mathbf{Z}\xi$。进一步看出，如果$P \neq 0$，我们可以写成$P = a X^n (1 + u)$，其中$a \in K^*, n \in \mathbf{N}, u \in K(X)$和$w(u) > 0$；因此，$K(X)$中的每个元素$R \neq 0$都可以写成形式
$$
R = b X^n (1 + u'),
$$
其中 $b \in K^*, n \in \mathbf{Z}, u' \in K(X)$ 和 $w(u') > 0$；那么$w(R) = v(b) + n \xi$，因此$w(R) = 0$当且仅当$v(b) = 0$和$n = 0$；因此，当$w(R) = 0$、$R$和$b$对$w$的理想模取模时全等，这表明$w$的剩余类域等于$v$的剩余类域。

最后从引理 1 得出$w$ 的存在性。

#### 命题 2 {#ac-vi-s10-prop-2 .statement tag=04Y7}

*令$K$为域，$v$为$K$，$\Gamma$为阶群，$k$为剩余类域。 $K(X)$上存在唯一的估值$w$延伸$v$，使得$X$的$w(X) = 0$和像$t$在$w$的剩余类域$k'$超越$k$。 $w$的阶群等于$v$，其剩余类域为$k(t)$。*

为了显示$w$的唯一性，我们只需证明，如果$P = \sum_j a_j X^j$是$K[X]$的非零元素，那么
$$
w(P) = \inf_j (v(a_j)).
$$
我们可以将$K^*$中的除$P$乘以元素，并假设$v(a_j) \geq 0$对于所有$j$，并且$v(a_j)$之一是零。 作为$w(X) = 0$，$P$，然后$w$的属于到环；将$k$中$a_j$的典范像写成$\bar{a}_j$，将剩余类域$k'$中$P$的典范像写成$\sum_j \bar{a}_j t^j$；由于$t$超越$k$，并且$\bar{a}_j$之一非零，因此像非零，从而
$$
w(P) = 0 = \inf_j (v(a_j)).
$$
现在我们证明$w$的存在。 公式$w(P) = \inf_j (v(a_j))$（对于$P = \sum_j a_j X^j$）定义凭借引理1对$K(X)$的估值$w$，并且$w$显然与$v$具有相同的阶群。 然后$w(X) = 0$。 我们证明$w$的剩余类域$k'$中$X$的典范像$t$超越$k$：如果$\sum_j \bar{a}_j t^j = 0$，其中$\bar{a}_j \in k$对于所有$j$，则用$a$表示，a $v$、$w \left( \sum_j a_j X^j \right) > 0$中的环代表$\bar{a}_j$； 从而$v(a_j) > 0$对于所有$j$，因此$\bar{a}_j = 0$对于所有$j$。 We show finally that $k' = k(t)$: every element $R$ of $K(X)$ may be written $R = c \left( \sum_j a_j X^j \right) / \left( \sum_j b_j X^j \right)$, where $c, a_j, b_j$ are in $K$, $v(a_j) \geq 0$ and $v(b_j) \geq 0$ for all $j$, one of the $v(a_j)$ and one of the $v(b_j)$ being zero; then $w(R) \geq 0$ if and only if $v(c) \geq 0$; denoting by $f$ the canonical homomorphism of the ring of $w$ onto $k'$,
$$
f(R) = f(c) \left( \sum_j f(a_j) t^j \right) / \left( \sum_j f(b_j) t^j \right),
$$

这证明了我们的断言。

#### 注 {#ac-vi-s10-n1-rem-1 .statement tag=04Y8}

不应该认为我们刚刚遇到的v到K(X)的两个型或扩张是唯一的；可能存在扩张的第三个型，其中$\Gamma'/\Gamma$是挠元群和$k'$$k$的（不一定是有限的）代数扩张。第三个型不一定由引理1中描述的过程提供（cf.§ 3，习题1）。

### 2.交换式群的有理秩

#### 定义 1 {#ac-vi-s10-def-1 .statement tag=04Y9}

*交换群 G 的有理秩是向量 Q 空间* $G \otimes_{\mathbf{Z}} \mathbf{Q}$ 的维数。

这个维数也可以定义为基数$r$的最小上界（有限或无限），使得G存在$r$元素，它们与$\mathbf{Z}$线性无关（*代数*，章II, § 7, no. 10， 命题26)。当且仅当 G 是挠元群时，G 的有理数秩是 *零*。对于加法群 $\mathbf{R}^n$ 的子群、有理数秩重合的概念，其定义见*一般拓扑*、章 VII, § 1。

在本段的其余部分中，我们将用$r(G)$表示交换性群G的有理秩。如果$G'$是G的子群，那么（因为$\mathbf{Q}$是平$\mathbf{Z}$模）我们有加法方程

$$
r(G) = r(G') + r(G/G').
$$

#### 命题 3 {#ac-vi-s10-prop-3 .statement tag=04YA}

*设G是G的全序交换群和H子群。如果$h(G)$和$h(H)$表示G和H*的高度（$§ 4$，no. 4），*则不等式*

$$
h(G) \leq h(H) + r(G/H)
$$

*持有*。

事实上，令$G_0 \subset G_1 \subset \ldots \subset G_n$为G的孤立子群的严格递增的序列，则需要建立不等式

$$
n \leq h(H) + r(G/H).
$$

对于$n = 0$来说这是显而易见的。假设$n \geq 1$，让我们用归纳对$n$进行争论。 应用归纳假设到群$G_{n-1}$及其子群$H \cap G_{n-1}$，我们得到

$$
n - 1 \leq h(H \cap G_{n-1}) + r(G_{n-1}/(H \cap G_{n-1})).
$$

那么我们区分两种情况：

(a) $H \cap G_{n-1} = H$，其他字$H \subset G_{n-1}$。 不等式 (7) 可以写成

$$
n \leq h(H) + r(G_{n-1}/H) + 1.
$$

现在$G/G_{n-1}$是一个完全有序的群，没有减少到0；因此它不是挠元群和 $r(G/G_{n-1}) \geq 1$。 (4) 从而，$r(G/H) \geq r(G_{n-1}/H) + 1$。代入(8)，我们当然得到所需的不等式(6)。

(b) $H \cap G_{n-1} \neq H$。由于$H \cap G_{n-1}$是$H$的孤立子群，因此我们将结论视为$h(H) > h(H \cap G_{n-1}) + 1$。另一方面，显然$r(G/H) \geq r(G_{n-1}/(H \cap G_{n-1}))$。代入(7)，再次得到(6)。

#### 推论{#ac-vi-s10-n2-cor-1 .statement tag=04YB}

*对于每个全序交换群 G，$h(G) \leq r(G)$。*我们在命题 3 中集合 $H = (0)$。

#### 命题 4 {#ac-vi-s10-prop-4 .statement tag=04YC}

*设 G 是全序交换律群。假设 G 是有限生成的且 $h(G) = r(G)$。那么 G 同构于按字典顺序排序的 $\mathbf{Z}^{r(G)}$。*

让我们写$r = r(G) = h(G)$。如果$r = 0$，则$G = (0)$。如果有限生成交换式群的$r = 1$、结构表明G有同构$j$到Z上（*代数*、章VII, § 4, no. 6、定理3）。现在Z只有两种与其群结构兼容的总序，即通常的序及其相反。因此，按照通常的顺序，$j$或$-j$是有序的群G到Z上的同构。

现在假设$r \geq 2$，让我们用归纳对$r$进行争论。令 H 为高度为 $r - 1$ 的 G 的孤立子群。然后是 $r(H) + r(G/H) = r$ (公式 (4))、$r(H) \geq h(H) = r - 1$ 和 $r(G/H) \geq h(G/H) = 1$（命题 3 的推论）、从而 $r(H) = r - 1$ 和 $r(G/H) = 1$。 归纳假设表明H与按字典顺序排序的$\mathbf{Z}^{r-1}$同构的，而情况$r = 1$表明$G/H$与Z同构。由于Z是自由Z模，因此H是G的*直因子*（*代数*，章11， § 1, no. 11，命题21)。下面的引理则表明G与词典乘积$H \times (G/H)$同构的（非规范），从而完成了证明。

#### 引理 2 {#ac-vi-s10-lem-2 .statement tag=04YD}

*设H是全序交换群 G的孤立子群。如果H是G的直因子，则有序群G与按字典顺序排序的群$(G/H) \times H$同构的。*

令$j$为$(G/H) \times H$的同构到G上，使得$j(0, x) = x$对于所有$x \in H$和$j(y, x)$属于到H的陪集。由于$(G/H) \times H$是全序的，这相当于表明$j$是*递增* （*集合理论*、章III, § 1, no. 12、命题11）。令 $(y, x)$ 为 $(G/H) \times H$ 的元素 $\geq 0$ 按字典顺序排序。如果$y > 0$，则H包含$j(y, x)$的陪集为元素$> 0$，从而$j(y, x) > 0$，否则为$y \leq 0$（§ 4, no. 2，命题3）。如果$y = 0$和$x \geq 0$，则$j(y, x) = x \geq 0$。因此$j$肯定是递增。

### 3.任何超验的案例扩张

在这个没有。我们将使用以下记号：$K$为域，$K'$扩张为$K$，$v$对$K$，$v'$扩张的$v$进行评估$K$、$\Gamma$ 和 $k$（分别为 $\Gamma'$ 和 $k'$） 阶群和剩余类域或 $v$（分别为 $v'$）。我们将写：

$$
d(K'/K) = \dim.\mathrm{al},\ K' = \text{transcendence degree of } K' \text{ over } K;
$$
$$
s(v'/v) = \dim.\mathrm{al},\ k' = \text{transcendence degree of } k' \text{ over } k;
$$
$$
r(v'/v) = r(\Gamma'/\Gamma) = \text{rational rank of } \Gamma'/\Gamma,
$$

如果右侧是有限的；否则，我们将约定$d(K'/K) = +\infty$（或$s(v'/v) = +\infty, r(v'/v) = +\infty$）。

#### 定理 1 {#ac-vi-s10-thm-1 .statement tag=04YE}

*设$x_1, \ldots, x,$为$v'$的环的元素，其中$k'$中的典范像$\overline{x}_i$在代数上独立于$k$和$K'$的$y_1, \ldots, y_r$元素，这样$\Gamma'/\Gamma$中的$v'(y_j)$的典范像在$\mathbf{Z}$上线性无关。那么$K'$的$r+s$元素$x_1, \ldots, x, y_1, \ldots, y_r$在代数上独立于$K$； $v'$到$K(x_1, \ldots, x, y_1, \ldots, y_r)$中的限制承认$k(\overline{x}_1, \ldots, \overline{x}_s)$为剩余类域并且*

$$
\Gamma + \mathbf{Z}v'(y_1) + \ldots + \mathbf{Z}v'(y_r)
$$

如*阶群*。

如果$r+s = 0$，我们的断言是显而易见的。我们通过归纳对$r+s$进行争论。如果$r' \leq r, s' \leq s$和$r'+s' < r+s$，归纳假设表明，如果$K$被$K(x_1, \ldots, x_s, y_1, \ldots, y_{r'})$取代，族$(x_1, \ldots, x_s), (y_1, \ldots, y_r)$被$(x_{s'+1}, \ldots, x_s), (y_{r'+1}, \ldots, y_r)$取代，定理1的假设成立。因此问题减少为以下两种情况之一：

(a) 环$v'$中存在元素$x$，使得$\overline{x}$超越$k$；那么有必要证明$x$超越$K$，并且$v'$到$K(x)$的限制承认$k(\overline{x})$为剩余类域，$\Gamma$为阶群。

(b) $K'$中有元素$y$，使得关系$nv'(y) \in \Gamma$和$n \in \mathbf{Z}$隐含$n = 0$；有必要证明$y$超越$K$，并且$v'$到$K(y)$的限制承认$k$为剩余类域，$\Gamma + \mathbf{Z}v'(y)$为阶群。

现在§ 8, no. 1的命题 1表明$x$（分别为$y$）不能是$K$的代数。 (a) 的其他断言（分别为 (b)）紧随 no. 1 的命题 2（分别为命题 1）。

#### 推论 1 {#ac-vi-s10-thm-1-cor-1 .statement tag=04YF}

*不等式*

$$
s(v'/v) + r(v'/v) \leq d(K'/K)
$$

*持有。*

*此外，如果$K'$是$K$的有限生成的扩张且等式在(9)中成立，则$\Gamma'/\Gamma$是$\mathbf{Z}$的有限生成的模，而$k'$是$k$的有限生成的扩张。*

令$r$和$s$为自然数，使得$r \leq r(v'/v)$和$s \leq s(v'/v)$；我们证明$r+s \leq d(K'/K)$，这将证明（9）。到假设时，$K'$存在元素$x_1, \ldots, x, y_1, \ldots, y$，其中满足是定理1的假设。

因此，它们在 $K$ 上是代数独立的，这表明不等式 $r + s < d(K'/K)$。

如果$K'$是$K$有限生成的扩张，则$d(K'/K)$是有限的，因此$s(v'/v)$和$r(v'/v)$也是有限的；我们用$s$和$r$表示它们。存在$K'$的元素$x_1, \ldots, x_s, y_1, \ldots, y_r$，其中满足定理1的假设。如果$r + s = d(K'/K)$，这些元素形式超越$K'$的基因此，$K$和$K'$是$K'' = K(x_1, \ldots, y_r)$的有限代数扩张。令$\Gamma''$和$k''$为$v'$到$K''$的限制和阶群和剩余类域。通过定理 1，$\Gamma''/\Gamma$是有限生成的$\mathbf{Z}$模，$k''$是$k$的有限生成的纯扩张。另一方面，由于$K'$是$K$的有限代数扩张，$\Gamma'/\Gamma$是有限群，$k'$是$k''$的有限代数扩张（§ 8, no. 1，引理） 2）。这就证明了推论。

#### 推论 2 {#ac-vi-s10-thm-1-cor-2 .statement tag=04YG}

*令h和h'为v和v'的高度。然后*
$$
s(v'/v) + h' \leq d(K'/K) + h.
$$
命题 3、$h' \leq r(v'/v) + h$。

#### 推论 3 {#ac-vi-s10-thm-1-cor-3 .statement tag=04YH}

*假设$K'$是$K$的有限生成的扩张，$\Gamma$与$\mathbf{Z}^{h'}$同构的（按字典顺序排列），并且公式中有等式（10）。那么 $\Gamma'$ 与 $\mathbf{Z}^{h'}$ 同构的（按字典顺序排序），$k'$ 是 $k$ 的有限生成的扩张。*

如果(10)中有等式，则(9)中有等式，从而事实上$k'$是$k$的有限生成的扩张，并且$\Gamma''$是有限生成的$\mathbf{Z}$模。进一步比较(9)和(10)，可以看出$h' - h = r(\Gamma'/\Gamma)$、从而$h' = r(\Gamma')$和命题 4 (no. 2)则表明$\Gamma'$与按字典顺序排列的$\mathbf{Z}^{h'}$同构的。

#### 推论 4 {#ac-vi-s10-thm-1-cor-4 .statement tag=04YI}

*假设 v 不合适（在这种情况下$k = K$）。然后*
$$
h(\Gamma') + d(k'/K) \leq r(\Gamma') + D(k'/K) \leq d(K'/K).
$$
*特别是，如果 v' 的高度为 1，则*
$$
d(k'/K) \leq d(K'/K) - 1;
$$
*此外，如果$K'$是$K$的有限生成的扩张，并且(12)中有等式，则$v'$是离散估值，$k'$是$K$的有限生成的扩张。*

它是推论1、2、3的特殊情况的级数。

### 习题{#ac-vi-s10-exercises}

§ 10](exercises/s10/)参见[习题。
