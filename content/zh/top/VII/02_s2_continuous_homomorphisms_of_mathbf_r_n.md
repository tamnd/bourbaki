---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 2
section_title: Continuous homomorphisms of $\mathbf{R}^n$ and its quotient groups
lang: zh
source: top-v-x
pdf_pages: 0085-0089, 0099-0101
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS HOMOMORPHISMS OF THE GROUP $\mathbf{R}^m$ INTO THE GROUP $\mathbf{R}^n$
      page: 0
      pdf_page: 85
    - "no": 2
      title: LOCAL DEFINITION OF A CONTINUOUS HOMOMORPHISM OF $\mathbf{R}^n$ INTO A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 85
    - "no": 3
      title: CONTINUOUS HOMOMORPHISMS OF $\mathbf{R}^m$ INTO $\mathbf{T}^n$
      page: 0
      pdf_page: 87
    - "no": 4
      title: AUTOMORPHISMS OF $\mathbf{T}^n$
      page: 0
      pdf_page: 88
statements: 10
exercises: 7
content_sha256: 965c7f756760f6a904648b5bb37f57f8ce00cc1b15e0164f346d8051b6256a55
translated_from: content/en/top/VII/02_s2_continuous_homomorphisms_of_mathbf_r_n.md
translation_method: google
source_content_sha256: 3f006ad7fa82d9c7e014ebfbbac1ca9f11dfb28040f438d97d56329bb57b038d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 707fa862900a21ed4bfc8e7db17674ce0444ce64f72f2090baeae445714015e8
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 2. $\mathbf{R}^n$ 的连续同态及其商群

### 1. 将群$\mathbf{R}^m$连续同态进入群$\mathbf{R}^n$

$\mathbf{R}^m$到$\mathbf{R}^n$的每个线性映射（cf.章VI，§i，no. 3）显然是加法群$\mathbf{R}^m$到加法群的连续同态 $\mathbf{R}^n$。反之：

#### 命题 1 {#top-vii-s2-prop-1 .statement tag=0BZ3}

*每个连续同态* $f$ * 的加法群* $\mathbf{R}^m$ * 到加法群* $\mathbf{R}^n$ * 是线性映射的 * $\mathbf{R}^m$ * 到* $\mathbf{R}^n$。

对于所有$x \in \mathbf{R}^n$和所有$t \in \mathbf{R}$，足以证明$f(tx) = tf(x)$。如果我们通过$x$ 替换 $x$ 和$\mathbf{R}$ 通过$\mathbf{R}^m$，则该参数与章 V、§ i、no. 3 的命题 5 相同。

### 2. 将$\mathbf{R}^n$的连续同态的局部定义转换为拓扑群

章V中的命题6，§i，no. 4可以推广到所有群$\mathbf{R}^n$。

#### 命题 2 {#top-vii-s2-prop-2 .statement tag=0BZ4}

*设* $A$ *是* $\mathbf{R}^n$ *其中包含* $o$的平行光； *并让* $f$ *成为* $A$ *的连续映射 *转换为拓扑群* $G$ *（乘法书写）* *使得* $f(x + y) = f(x)f(y)$ *对于点* $x, y$的每个对 *这样*$x \in A,\ y \in A$*和*$x + y \in A$。 *则存在* $\mathbf{R}^n$ *到* $G$ *其中扩展* $f$的唯一连续同态。

通过与章V的命题6相同的推理，§i，no. 4，我们证明延伸$f$的同态，如果存在的话，是*唯一的*。接下来，由$f(A)$生成的$G$的子群$G_1$是*可交换的*；因为如果$x$和$y$是$A$中的任意两个点，那么$\frac{1}{2} x, \frac{1}{2} y$和$\frac{1}{2} (x + y)$属于到$A$，因此

$$
f \left( \frac{1}{2} (x + y) \right) = f \left( \frac{1}{2} x \right) \quad (f \frac{1}{2} y) = f \left( \frac{1}{2} y \right) f \left( \frac{1}{2} x \right),
$$

这表明 $f \left( \frac{1}{2} x \right)$ 和 $f \left( \frac{1}{2} y \right)$ 通勤；因此$f(x) = (f \left( \frac{1}{2} x \right))^2$和$f(y) = (f \left( \frac{1}{2} y \right))^2$也是如此，这证明了断言。

令$a_1, a_2, \ldots, a_n$为$n$非零向量包含在$A$中并与平行四面体的基向量成比例，并且对于每个指标$i$令$D_i$为通过$o$的线并且$a_i$，即点$ta_i$的集合，因为$t$贯穿$\mathbf{R}$。令$A_i$为所有$t \in \mathbf{R}$中的集合，使得$ta_i \in A$；那么$A_i$是$\mathbf{R}$包含于$[0, 1]$的区间，函数

$$
f_i(t) = f(ta_i)
$$

在 $A_i$ 上定义且连续，并且满足关系

$$
f_i(t + t') = f_i(t) f_i(t')
$$

每当$t, t'$和$t + t'$都是属于到$A_i$。到章V, § 1, no. 4的命题6，存在$\mathbf{R}$到$G$的连续同态$\bar{f}_i$，其中扩展$f_i$。由于$\mathbf{R}^n$是子群$D_i$的直和，我们可以根据规则将$\mathbf{R}^n$的定义同态$\bar{f}$化为阿贝尔的群$G_1$ $\bar{f}(x) = \prod_{i=1}^n \bar{f}_i(t_i)$，其中$x = \sum_{i=1}^n t_i a_i$； $\bar{f}$是$f$的扩张，因为如果$x \in A$，$x$的所有分量$x_i$在$D_i$线上，也从属于到$A$，由于选择 $a_i$；此外，$\bar{f}$在$\mathbf{R}^n$上是连续的，因为它在$D_i$的每条线上都是连续的，并且$x_i$是$x$的线性函数（因此是连续的）。

#### 推论 1 {#top-vii-s2-prop-2-cor-1 .statement tag=0BZ5}

*令$V$为$\mathbf{R}^n$中$o$的邻域，并令$f$为$V$的连续映射，形成拓扑群$G$，使得*

$$
f(x + y) = f(x) f(y)
$$

*对于点$x, y$中的每个对，使得$x \in V, y \in V$和$x + y \in V$。 Then there exists a unique continuous homomorphism of $\mathbf{R}^n$ into $G$ which agrees with $f$ at all points of a neighbourhood $W$ of $o$.*

取$W$为一个开箱，中心$o$包含在$V$中，应用命题2到$W$。

稍后我们将看到，$\mathbf{R}^n$扩展的性质到拓扑群的更大类，即“单连通”群。

#### 推论 2 {#top-vii-s2-prop-2-cor-2 .statement tag=0BZ6}

*令$f$是$\mathbf{R}^n$的局部同构，具有拓扑群$G$。 Then there exists a unique strict morphism of $\mathbf{R}^n$ onto an open subgroup of $G$ which agrees with $f$ at all the points of some neighbourhood of $o$.*

令$\overline{f}$为$\mathbf{R}^n$到$G$的连续同态，与$f$在$o$的邻域的点一致； $\overline{f}(\mathbf{R}^n)$包含于，通过假设，单位元素的邻域到$G$，因此（章III, § 2, no. 1，命题4的推论）是$G$的开子群；此外，$\overline{f}$是$\mathbf{R}^n$到$\overline{f}(\mathbf{R}^n)$的严格态射，通过章III, § 2, no. 8，命题24。

#### 定理 1 {#top-vii-s2-thm-1 .statement tag=0BZ7}

*每个与 $\mathbf{R}^n$ 局部同构的连通的群 $G$ 也同构于群 $\mathbf{R}^p \times \mathbf{T}^{n-p}$ ($0 \leqslant p \leqslant n$)。*

适当选择$\mathbf{R}^n$的局部同构$f$和$G$扩展到$\mathbf{R}^n$的严格态射到$G$的开放子群（命题2，推论2），因此到$G$ 本身，因为 $G$ 已连接。由此可见，$G$与$\mathbf{R}^n$的商群$\mathbf{R}^n/H$同构：$H$是*离散*，否则将存在任意接近$o$的$H$的点$x \neq o$，并且使得$f(x) = f(o)$，与假设相反，$f$是本地同构。因此，定理是推论 / 定理 1 / § 1, no. 1。

### 3. 连续同态的 $\mathbf{R}^m$ 进入 $\mathbf{T}^n$

#### 命题 3 {#top-vii-s2-prop-3 .statement tag=0BZ8}

*$\mathbf{R}^m$到$\mathbf{T}^n$的每个连续同态都是形式$x \to \varphi(u(x))$，其中$\varphi$是$\mathbf{R}^n$到$\mathbf{T}^n$的典范同态（用$\mathbf{R}^n/\mathbf{Z}^n$标识），$u$是将 $\mathbf{R}^m$ 的线性映射转换为 $\mathbf{R}^n$。*

令$f$是$\mathbf{R}^m$到$\mathbf{T}^n$的连续同态。我们将证明，$\mathbf{R}^m$中存在线性映射$u$进入$\mathbf{R}^n$，使得同态$x \to f(x)$和$x \to \varphi(u(x))$重合在点的*邻域*$o$中$\mathbf{R}^m$；然后，命题将从no. 2的推论1到命题2。现在令$V$为$\mathbf{R}^n$中$o$的邻域，使得限制为$V$的$\varphi$是$\mathbf{R}^n$与$\mathbf{T}^n$的局部同构，并令$\psi$为$\varphi$，定义于$\varphi(V)$。由于$f$是连续的，$V' = \overline{f}^{-1}(\varphi(V))$是$\mathbf{R}^m$中$o$的邻域； 映射

$$
x \to \psi(f(x)),
$$

限制为$V'$，是$V'$到$\mathbf{R}^n$的连续映射，使得$\psi(f(x+y)) = \psi(f(x)) + \psi(f(y))$对于$\mathbf{R}^m$中点$x, y$的每个对，使得$x \in V', y \in V'$和$x + y \in V'$；因此（no. 2，推论1到命题2）这个映射重合具有确定的连续$\mathbf{R}^m$的同态$u$到$\mathbf{R}^n$的点邻域 $\mathbf{R}^m$ 中 o 的$W$。将命题 1 (no. 1) $u$ 等于 $\mathbf{R}^m$ 中的线性映射变为 $\mathbf{R}^n$；因此，对于所有$x \in W$，我们有$f(x) = \varphi(u(x))$，从而完成证明。

#### 注 {#top-vii-s2-n3-rem-1 .statement tag=0BZ9}

更一般地，相同的论点表明，如果 $\varphi$ 是 $\mathbf{R}^n$ 到群 $G$ 的严格态射，其限制到 o 的合适邻域是 $\mathbf{R}^n$ 与 $G$ 的局部同构，则每个连续$\mathbf{R}^n$到$G$的同态等于形式$x \mapsto \varphi(u(x))$，其中$u$是$\mathbf{R}^m$到$\mathbf{R}^n$的线性映射。

在 $m = n = 1$ 的情况下，命题 3 给出：

#### 命题 4 {#top-vii-s2-prop-4 .statement tag=0BZA}

*如果$\varphi$是$\mathbf{R}$的典范同态到$\mathbf{T}$，$\mathbf{R}$到$\mathbf{T}$的每个连续同态都是形式$x \mapsto \varphi(ax)$，其中$a \in \mathbf{R}$；如果 $a \neq 0$，则严格将 $\mathbf{R}$ 态射放到 $\mathbf{T}$。*

### 4. 自同构 / $\mathbf{T}^n$

令$H$为$\mathbf{R}^n$的闭子群，并令$\varphi$为$\mathbf{R}^n$的典范同态到商群$\mathbf{R}^n/H$。如果$f$是$\mathbf{R}^n/H$到拓扑群$G$的连续同态，那么$f = f \circ \varphi$是$\mathbf{R}^n$到$G$的连续同态，它是周期性的并且有群个周期包含$H$；相反，$\mathbf{R}^n$到$G$的每个周期连续同态，其周期包含$H$的群都是这个形式。

在$H = \mathbf{Z}^n$、商群$\mathbf{R}^n/\mathbf{Z}^n = \mathbf{T}^n$是*紧凑*的情况下，因此$\mathbf{T}^n$的每个连续同态$f$进入拓扑群$G$都是$\mathbf{T}^n$的*严格态射* $G$，前提是$G$是豪斯多夫（章III, § 2, no. 8，注1）； $f = f \circ \varphi$ 是 $\mathbf{R}^n$ 到 $G$ 的严格态射；此外，$f(\mathbf{T}^n) = f(\mathbf{R}^n)$是$G$的*紧凑*子群，同构于群$\mathbf{T}^p$（$0 \leq p \leq n$）。

特别是，我们看到，$\mathbf{T}^n$到群$\mathbf{R}^m$的唯一连续同态是*零*映射，因为$\{ o \}$是$\mathbf{R}^m$的唯一紧凑子群。

让我们将其应用于$\mathbf{T}^n$的连续同态到群$\mathbf{T}^p$；如果$f$是这样的同态，$\mathbf{R}^n$的$\varphi$典范同态到$\mathbf{T}^n$上，则$f \circ \varphi$是$\mathbf{R}^n$到$\mathbf{T}^p$的连续同态；因此（no. 3，命题 3）如果$\psi$表示$\mathbf{R}^p$的典范同态到$\mathbf{T}^p$，则存在$\mathbf{R}^n$的线性映射$u$到$\mathbf{R}^p$使得$f \circ \varphi = \psi \circ u$。如果$x \in \mathbf{Z}^n$，$f(\varphi(x))$是$\mathbf{T}^p$的单位元素，那么我们一定有$u(x) \in \mathbf{Z}^p$，即$u(\mathbf{Z}^n) \subset \mathbf{Z}^p$。相反，如果$u$是$\mathbf{R}^n$到$\mathbf{R}^p$的任何线性映射满足条件，则$\psi \circ u$是$\mathbf{R}^n$到$\mathbf{T}^p$的周期连续同态，其周期为群包含 $\mathbf{Z}^n$，因此定义是 $\mathbf{T}^n$ 的连续同态到 $\mathbf{T}^p$。

考虑一下条件$f$是$\mathbf{T}^n$的*同构*到$\mathbf{T}^p$的子群。首先，$u$必须是$\mathbf{R}^n$到$\mathbf{R}^p$的*单射的*映射，否则向量子空间$\overline{u}(0)$将包含点$x \neq 0$任意接近原点，并且在这样的点我们应该有
$$
f(\varphi(x)) = f(\varphi(0)) \quad \text{and} \quad \varphi(x) \neq \varphi(0),
$$
与假设相反。这个条件意味着$p \geq n$。 像$u(\mathbf{Z}^n)$则为群$\mathbf{Z}^p$的秩$n$的离散子群； $u(\mathbf{Z}^n)$相对于$\mathbf{Z}^p$（§ 1, no. 1）的*不变因子*必须全部等于1，否则将存在点$x \in \mathbf{Z}^n$和整数$k > 1$使得$u(k^{-1}x) \in \mathbf{Z}^n$和$k^{-1} \notin \mathbf{Z}^n$，因此$f(\varphi(k^{-1}x)) = f(\varphi(0))$和$\varphi(k^{-1}x) \neq \varphi(0)$，与假设相反。相反，如果满足这个条件，则$u(\mathbf{R}^n) \cap \mathbf{Z}^n = u(\mathbf{Z}^n)$和$f$是$\mathbf{T}^n$的同构到$u(\mathbf{R}^n)/u(\mathbf{Z}^n)$上。

如果我们将此参数应用于案例$p = n$，我们将得到以下命题：

#### 命题 5 {#top-vii-s2-prop-5 .statement tag=0BZB}

*拓扑群$\mathbf{T}^n$到其中一个子群的每个同构都是$\mathbf{T}^n$的自同构，这是通过经过与$\mathbf{R}^n$的线性映射$u$对自身的商获得的，仅限于$\mathbf{Z}^n$，是 $\mathbf{Z}^n$ 的自同构。*

等价地（§ 1, no. 1），如果$u(e_i) = \sum_{j=1}^n a_{ij} e_j$，则$a_{ij}$必须是整数，使得$\det(a_{ij}) = \pm 1$。特别是对于$n = 1$：

#### 命题 6 {#top-vii-s2-prop-6 .statement tag=0BZC}

*拓扑群 $\mathbf{T}$ 中只有同构到其子群之一上是恒等映射和对称性 $x \to -x$。*

### 习题 {#top-vii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
