---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 4
section_title: Normal spaces
lang: zh
source: top-v-x
pdf_pages: 0185-0196, 0245-0255
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF NORMAL SPACES
      page: 0
      pdf_page: 185
    - "no": 2
      title: EXTENSION OF A CONTINUOUS REAL-VALUED FUNCTION
      page: 0
      pdf_page: 188
    - "no": 3
      title: LOCALLY FINITE OPEN COVERINGS OF A CLOSED SET IN A NORMAL SPACE
      page: 0
      pdf_page: 191
    - "no": 4
      title: PARACOMPACT SPACES
      page: 0
      pdf_page: 193
    - "no": 5
      title: PARACOMPACTNESS OF METRIZABLE SPACES
      page: 0
      pdf_page: 194
statements: 25
exercises: 30
content_sha256: 93dc5777d1ce87bda79cf473f7267f17bdaeb6cbff66962c2c299f78baf071e1
translated_from: content/en/top/IX/04_s4_normal_spaces.md
translation_method: google
source_content_sha256: 9659cfc8beeaee4a3f7b73b432335f6ffd60e7f82a5d2d879d79d7ffdfda75df
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 0c6d7f665532a0f5527d9f993c4aa2e37e1088fd4ca3b43196a3d09ef7107d7c
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 4. 正常空间

### 1. 定义正常空间

可均匀化空间 ($§ 1$, no. 5) 的公理 ($O_{IV}$) 可以用以下形式表示： *给定任何闭集合* $A$ *和任何点* $x \in \mathbf{C}A$，*有一个连续* $X$ *到* $[0, 1]$ *的映射 *等于* 0 *在* $x$ *并且等于* 1 *在* $A$的每点；这个性质可以再次用说来表达，在可统一的空间中，我们可以通过连续实值函数来分离点和封闭的集合（不是包含点）。

现在我们要研究空间，其中可以用相同的方式将两个不相交的封闭的集合通过连续实值函数分开：

#### 定义 1 {#top-ix-s4-def-1 .statement tag=0C5F}

*如果拓扑空间$X$是豪斯多夫且满足以下公理，则称其为正规：*

$(O_v)$ *如果$A$和$B$是$X$的任意两个不相交的闭子集，则存在$X$到$[0, 1]$的连续映射，每次都等于$0$ 点/$A$，每点/$B$前往$1$。*

显然每个正态空间都是完全正则的；但也有完全规则的空间，但不规则（参见习题 9、10、13、26 和 § 5、习题 15 和 16）。

Axiom $(O_v)$ 的叙述与 $(O_{IV})$ 一样，涉及实直线 $\mathbf{R}$ 作为辅助集合。但有条件等价于 $(O_v)$，其中不涉及辅助集合：

#### 定理 1（尤里索恩）{#top-ix-s4-thm-1 .statement tag=0C5G}

*公理$(O_v)$等价于：*

$(O'_v)$ *如果$A$和$B$是$X$中任意两个不相交的闭子集，则存在两个不相交的开集合$U, V$使得$A \subset U$和$B \subset V$.*

紧接着，$(O_v)$蕴含$(O'_v)$，因为如果$f$是$X$到$[0, 1]$的连续映射，等于$A$上的$0$和$B$上的$1$，则开分别为集合 $\overline{f}^{-1}([0, 1/2[)$ 和 $\overline{f}^{-1}(]1/2, 1])$ 包含 $A$ 和 $B$，且不相交。

为了证明逆命题，首先注意$(O'_v)$等价于以下公理：

$(O''_v)$ *给定任何闭集合$A$和$A$的任何开邻域$V$，存在$A$的开邻域$W$使得$\overline{W} \subset V$。*

如果存在连续的映射$f : X \to [-1, +1]$，它在$A$上等于$-1$，在$B$上等于$+1$，并且如果我们为每个$t \in [0, 1]$放置$U(t) = \overline{f}^{-1}([-1, t[)$，那么我们就在$X$中定义了一个开族集合，索引为$[0, 1]$，使得 (i) $A \subset U(0)$，(ii) $B \subset \mathbf{C}U(1)$ 和 (iii) 对于实数 $t, t'$ 中的每个对，使得 $0 \leq t < t' \leq 1$ 我们有

$$(1)$$
$$
\overline{U}(t) \subset U(t');
$$

因为$U(t)$包含在封闭的集合$\overline{f}^{-1}([-1, t])$中。相反，假设我们用这三个属性 (i)、(ii) 和 (iii) 定义了一个开放集合 $(0 \leq t \leq 1)$ 的族 $(U(t))$。对于每个$x \in X$，如果$x \in \mathbf{C}U(1)$，则放入$g(x) = 1$，如果$x \in U(1)$，则让$g(x)$为$t$的值的下确界，使得$x \in U(t)$。显然每个$x \in X$有$0 \leq g(x) \leq 1$，$A$有$g(x) = 0$，$B$有$g(x) = 1$；而且$g$在$X$上是连续的，因为如果我们放入$g(x) = a$，我们对所有$y \in U(a + \varepsilon) \cap \overline{\mathbf{C}U}(a - \varepsilon)$有$|g(y) - g(x)| \leq \varepsilon$，这是$x$的邻域乘以（i）[约定，$U(a + \varepsilon) = X$如果$a + \varepsilon > 1$，并且$U(a - \varepsilon) = \varnothing$如果$a - \varepsilon < 0$]。

因此，如果我们能够定义 $(U(t))$ 开集合满足条件 (i)、(ii) 和 (iii)，则定理 1 将得到证明；为此，我们使用 Axiom $(\mathrm{O}'_V)$。取$U(1) = \mathbf{C}B$；由于$A \subset U(1)$，存在一个开集合$U(o)$，使得$A \subset U(o)$和$U(o) \subset U(1)$乘以$(\mathrm{O}'_V)$。假设对于每个二元数$k/2^n$（$k = 0, 1, \ldots, 2^n$），我们定义了一个开放的集合$U(k/2^n)$，这些集合对于$0 \leq k \leq 2^n - 1$来说是$\overline{U}(k/2^n) \subset U((k+1)/2^n)$。对于每个二元数
$$
(2k + 1)/2^{n+1} \quad (0 \leq k \leq 2^n - 1)
$$
$(\mathrm{O}'_V)$ 存在一个开集合 $U((2k + 1)/2^{n+1})$ 使得
$$
\overline{U}(k/2^n) \subset U((2k + 1)/2^{n+1})
$$
和
$$
\overline{U}((2k + 1)/2^{n+1}) \subset U((k + 1)/2^n).
$$
因此，对于每个二元数$r$，使得$0 \leq r \leq 1$，我们可以定义一个开放的集合$U(r)$，使得$A \subset U(o)$，$B \subset \mathbf{C}U(1)$，和
$$(2)$$
$$
\overline{U}(r) \subset U(r')
$$
对于二元数$r, r'$中的每个对，使得$0 \leq r < r' \leq 1$。

现在定义，对于每个实数$t \in [0, 1]$，
$$
U(t) = \bigcup_{r \leq t} U(r) \quad (r \text{ dyadic});
$$
由(2)可知，这个定义与前面的$t$二元一致；另外，如果$0 \leq t < t' \leq 1$，则存在两个二元数$r, r'$使得$t \leq r < r' \leq t'$；由 (2) 我们有 $U(t) \subset U(r)$，因此
$$
\overline{U}(t) \subset \overline{U}(r) \subset U(r') \subset U(t');
$$
这就证明了 (1)，从而完成证明。

定理 1 将使我们能够证明拓扑空间的两个重要类别是正规的。首先：

#### 命题 1 {#top-ix-s4-prop-1 .statement tag=0C5H}

*紧凑空间是正常的。*

紧致空间通过章 I, § 9, no. 2 的命题 2 满足公理 $(\mathrm{O}'_V)$。

至于*局部紧致*空间，这样的空间的每个点都有一个紧致的邻域，这是一个普通的子空间；但是局部紧凑的空间中有例*不正常*（cf.习题9和26，以及§ 5，习题15）。

#### 命题 2 {#top-ix-s4-prop-2 .statement tag=0C5I}

*可测量空间是正常的。*

令$X$为可度量的空间，并令$d$为与$X$的拓扑兼容的度量。 Let $A, B$ be two disjoint closed subsets of $X$; since the functions $d(x, A)$ and $d(x, B)$ are continuous, the set $U$ (resp. $V$) of points $x$ such that $d(x, A) < d(x, B)$ [resp. $d(x, B) < d(x, A)$] is open; clearly $A \subset U$ and $B \subset V$ and $U \cap V = \varnothing$, hence Axiom $(O'_V)$ is satisfied.

#### 注 1 {#top-ix-s4-n1-rem-1 .statement tag=0C5J}

命题 2 给出另一个 *必要* 条件的可度量性；但是这个条件，即使在合取中，在§ 2中给出了所有必要的条件，也没有为集合提供足够的条件以实现可度量性（cf.习题6和§ 5，习题10）。

#### 注 2 {#top-ix-s4-n1-rem-2 .statement tag=0C5K}

正常空间存在例，它们既不可度量，也不可局部紧致（参见§ 5、习题 16）。

到$(O'_V)$，正常空间的每个*闭合*子集都是*正常子空间*；但对于正常空间的*任意* 子集情况并非总是如此。

对于例，非正规的完全正则空间同胚于紧致空间（§ 1, no. 5，命题3）的子空间，而后者是正规的。

最后我们记录两个正常的空间的*乘积*不一定是正常的（参见习题9和§ 5、习题16）。

### 2. 连续实值函数的扩张

令$X$和$Y$为两个拓扑空间，并令$A \neq X$为$X$的*封闭*子集。如果$f$是$A$到$Y$的连续映射，则并不总是可以*扩展*$f$到整个$X$到$Y$的连续映射。当$Y = \overline{\mathbf{R}}$时，这种扩张的可能性由以下定理决定：

#### 定理 2（尤里索恩）{#top-ix-s4-thm-2 .statement tag=0C5L}

*Axiom* $(O_V)$ *等价于以下性质*： $(O''_V)$ *给定任何闭子集* $A$ *of* $X$ *和任何连续实值函数* $f$ *（有限或非有限）* *定义于* $A$，*存在*$f$*的扩张* $g$*到整个空间*$X$，*这是*$X$*到*$\overline{\mathbf{R}}$的连续映射。

容易看出$(O''_V)$蕴涵$(O_V)$；因为如果$B$和$C$是$X$的两个不相交的闭子集，则函数在$B$上等于0并且在$C$上等于$i$是定义的并且在闭集合上连续$B \cup C$，因此到$(O''_{V})$有连续的扩张$f$到$X$。如果$g = \inf (f^{+}, 1)$，则$g$在$X$上连续，在$[0, 1]$中取其值，并且等于$B$上的$o$以及$C$上的$i$。

让我们反过来证明$(O_{V})$蕴含$(O''_{V})$。由于$\overline{\mathbf{R}}$和区间$[ -i, +i ]$同胚，我们只需考虑连续映射$f : A \to \overline{\mathbf{R}}$在$[ -i, +i ]$取值的情况。我们将$f$到$X$的构造扩张$g$通过在$X$上形成连续函数的序列$(g_{n})$，使得序列$(g_{n}(x))$收敛于所有区间$[ -i, +i ]$的$x \in X$至点；到定义，这个极限将在$x$处成为$g$的值，并且从$g_{n}$的选择开始，函数$g$满足所需的条件。

$g_{n}$的定义依赖于以下引理：

#### 引理 1 {#top-ix-s4-lem-1 .statement tag=0C5M}

*设$u$为$A$到$[ -i, +i ]$的连续映射；那么$X$到$[ -i/3, +i/3 ]$有一个连续的映射$v$，这样$|u(x) - v(x)| \leq 2/3$对于所有$x \in A$。*

令$H$为所有$x \in A$的集合，使得$-i \leq u(x) \leq -i/3$，并令$K$为所有$x \in A$的集合，使得$i/3 \leq u(x) \leq i$； $H$ 和 $K$ 在 $A$ 中封闭，因此在 $X$ 中封闭，并且不相交；因此，到$(O_{V})$时，$X$到$[ -i/3, +i/3 ]$有一个连续的映射$v$，它等于$H$上的$-i/3$和$K$上的$+i/3$。 映射$v$满足引理中的条件。

我们现在定义函数$g_{n}$到归纳。 应用引理和$u = f$，我们将定义$g_{0}$作为$X$到$[ -i/3, +i/3 ]$的连续映射，这样$|f(x) - g_{0}(x)| \leq 2/3$对于所有$x \in A$。现在假设连续映射 $g_{n}$ 的 $X$ 进入区间

$$
[-i + (\frac{2}{3})^{n+1}, i - (\frac{2}{3})^{n+1}]
$$

已定义，使得 $|f(x) - g_{n}(x)| \leq (\frac{2}{3})^{n+1}$ 对于所有$x \in A$。 应用引理到函数$u(x) = (\frac{2}{3})^{n+1} (f(x) - g_{n}(x))$，我们看到区间中存在连续的映射$h_{n+1}$$X$

$$
\left[ -\frac{2^{n+1}}{3^{n+2}}, \frac{2^{n+1}}{3^{n+2}} \right]
$$

这样

$$
|f(x) - g_{n}(x) - h_{n+1}(x)| \leq (2/3)^{n+2}
$$

对于所有$x \in A$； 归纳通过取$g_{n+1} = g_{n} + h_{n+1}$来完成，因为对于所有$x \in X$，函数满足不等式$|g_{n+1}(x)| \leq 1 - (2/3)^{n+2}$，凭借$h_{n+1}$的定义。

由此定义可以得出，对于 $m \geq p$ 和 $n \geq p$，我们有

$$
|g_{m}(x) - g_{n}(x)| \leq \frac{2^{p+1}}{3^{p+2}} \sum_{k=0}^{\infty} (2/3)^{k} = (2/3)^{p+1}
$$

在每个点 $x \in X$；因此序列$(g_n(x))$对于每个$x \in X$来说都是柯西序列，因此收敛到区间$[ -1, +1 ]$的点$g(x)$；并且由于对于所有$x \in A$和$n \to \infty$，$f(x) - g_n(x)$趋于0，$g$是$f$到$X$的扩张。因此，只需证明 $g$ 在 $X$ 上连续。

现在让$x$为$X$中的任意点；那么，给定任何$\varepsilon > 0$，都存在整数$n_0$，使得$|g_m(y) - g_n(y)| \leq \varepsilon$对于所有$y \in X$、所有$m \geq n_0$和所有$n \geq n_0$；因此，让$m$趋于$+\infty$，我们有

$$
|g(y) - g_n(y)| \leq \varepsilon.
$$

令 $V$ 为 $x$ 的邻域，使得 $|g_n(y) - g_n(x)| \leq \varepsilon$ 对于所有 $y \in V$；那么，对于每个 $y \in V$ 我们将有

$$
|g(y) - g(x)| \leq |g(y) - g_n(y)| + |g_n(y) - g_n(x)| + |g(x) - g_n(x)| \leq 3\varepsilon,
$$

这表明$g$在$x$连续，并完成定理2的证明。（证明的最后一个部分在特定情况下使用一致收敛的思想，我们将在章X中一般性地研究它， no. 1。）

#### 推论 {#top-ix-s4-n2-cor-1 .statement tag=0C5N}

*如果$f$是定义在$A$上的有限连续实值函数，则存在定义在$X$上的有限连续实值函数$g$，即扩展$f$。*

首先考虑$f(x) \geq 0$对于所有$x \in A$的情况；那么就有$f$到$X$的连续扩张$g_1$，在$[0, +\infty]$中取其值。如果我们放入 $B = \overline{g_1}(+\infty)$，则 $B$ 是闭集，并且到假设不会满足 $A$；因此，函数$h$在$A$上等于$f$，在$B$上等于0，因此是闭集合$A \cup B$上的连续函数。令$g_2$为$h$到$X$的连续扩张，再次取$[0, +\infty]$中的值；那么函数$g = \inf(g_1, g_2)$是$f$到$X$的连续扩张，其值是$\geq 0$并且在$X$的每个点处*有限*。

为了传递到一般情况，注就足够了，如果$f$在$A$上是有限且连续的，那么$f^+$和$f^-$也是有限且连续的；将$f^+$和$f^-$分别通过有限连续函数、$g_1$和$g_2$延伸到$X$，我们看到函数$g_1 - g_2$在$X$和扩展$f$上是有限连续的。

#### 注 {#top-ix-s4-n2-rem-1 .statement tag=0C5O}

如果$X$是正常的空间并且$A$是$X$的闭子集，则$A$的每个连续映射$f$也存在一个连续的扩张到$X$到*立方体* $K^1$（§ 1, no. 5）；因为我们有$f = (f_i)_{i \in I}, f_i$是$A$的连续映射进入$\mathbf{R}$的紧致区间$K$；由于存在连续的映射$g_i : X \to K$，其中扩展$f_i$，映射$g = (g_i)$是$f$到$X$的连续扩张。

### 3. 正常空间中闭集合的局部有限开覆盖

#### 定理 3 {#top-ix-s4-thm-3 .statement tag=0C5P}

令 $(A_i)_{i \in I}$ 为正常空间 $X$ 中闭集合 $Y$ 的局部有限开覆盖。然后有一个 $Y$ 的开覆盖$(B_i)_{i \in I}$，使得每个 $i \in I$ 都有 $\overline{B}_i \subset A_i$。

良序指标集合$I$（集合理论，章III, § 2, no. 3，定理1）。我们将在$X$中将定义一个家庭$(B_i)_{i \in I}$开放为集合，到超限归纳，使得(i)每个$i \in I$有$\overline{B}_i \subset A_i$； (ii) 对于每个$i \in I$，由$B_\lambda$形成的族，使得$\lambda \leq i$和由$A_\lambda$形成的族，使得$\lambda > i$是$Y$的开覆盖。假设我们已经为$i < \gamma$定义了$B_i$，使得所有$i < \gamma$都满足(i)和(ii)，并且让我们证明我们可以以这样的方式来定义$B_\gamma$，使得$i = \gamma$也满足(i)和(ii)。让我们首先证明，$i < \gamma$的$B_i$和$i \geq \gamma$形式的$A_i$覆盖了$Y$。到假设，对于每个$x \in Y$，只有指标$\lambda \in I$的有限数，这样$x \in A_\lambda$，比如说$\lambda_1 < \lambda_2 < \cdots < \lambda_n$；令$\lambda_h$为$\lambda_i$的最大的，使得$\lambda_i < \gamma$；如果$h < n$我们有$x \in A_{\lambda_n}$和$\lambda_n \geq \gamma$，并且如果$h = n$归纳假设表明$x$属于到一些$B_\lambda$使得$\lambda \leq \lambda_n < \gamma$，并且我们的断言紧随其后。

现在输入$C = (\complement Y) \cup \left( \bigcup_{i < \gamma} B_i \right) \cup \left( \bigcup_{i > \gamma} A_i \right)$； $C$已开放，根据前面所说我们有$\complement A_\gamma \subset C$；根据正常空间的公理$(O''_V)$，因此存在一个开集合$V$，使得$\complement A_\gamma \subset \overline{V} \subset V \subset C$。如果我们放入$B_\gamma = \complement \overline{V}$，我们就有$\overline{B}_\gamma \subset \complement V \subset A_\gamma$和$B_\gamma \cup C = X$，这样$B_i$使得$i \leq \gamma$和$A_i$使得$i > \gamma$覆盖$Y$。

#### 注 {#top-ix-s4-n3-rem-1 .statement tag=0C5Q}

注，我们仅使用覆盖$(A_i)$是点有限的事实，即$X$属于的每个点到集合$A_i$的有限数。

#### 定义 2 {#top-ix-s4-def-2 .statement tag=0C5R}

令$X$为拓扑空间，并令$f$为在$X$上定义的实值函数。 $f$的支持度用$\operatorname{Supp}(f)$表示，在$X$中最小的闭集合$S$，使得$f(x) = 0$对于所有$x \notin S$。

在其他字中，$\operatorname{Supp}(f)$是所有$x \in X$的集合在$X$中的闭包，使得$f(x) \neq 0$；或者再次，它是所有$x \in X$中的集合，使得$x$包含点$y$的每个邻域其中$f(y) \neq 0$。

令$(f_i)_{i \in I}$是$X$上的有限实值函数族，其支持形式局部有限族；然后为每个$x \in X$定义和$\sum_{i \in I} f_i(x)$（因为包含只是非零项的有限数）。有限实值函数$x \to \sum_{i \in I} f_i(x)$称为$(f_i)$族的和，记为$\sum_{i \in I} f_i$。如果$f_i$中的每一个都是连续的，那么$f = \sum_{i \in I} f_i$也是连续的；因为如果$x$是$X$中的任意点，则存在$x$的邻域$V$仅满足$f_i$的有限数支撑，因此存在有限子集$H$ $I$使得$f(y) = \sum_{i \in H} f_i(y)$对于所有$y \in V$。

#### 定义 3 {#top-ix-s4-def-3 .statement tag=0C5S}

*给定一个拓扑空间* $X$的族*$(A_i)_{i \in I}$*的子集，*族*$(f_i)_{i \in I}$*定义在*$X$*上的实值函数*据说从属于该族*$(A_i)_{i \in I}$*如果我们有* $\operatorname{Supp}(f_i) \subset A_i$ *每个指标* $i \in I$。

* 单位元的连续划分在* $X$ * 是任意族* $(f_i)_{i \in I}$ * 实值连续函数* $\geq 0$ * 在* $X$ * 支持形式一个局部有限族并且满足* $\sum_{i \in I} f_i(x) = 1$ *对于所有人*$x \in X$。

#### 命题 3 {#top-ix-s4-prop-3 .statement tag=0C5T}

*给定任何局部有限开覆盖* $(A_i)_{i \in I}$ *正常的空间* $X$，*存在单位元* $(f_i)_{i \in I}$ *在* $X$上的连续划分，*从属于覆盖* $(A_i)_{i \in I}$。

到定理 3 时，存在$X$ 的开覆盖$(B_i)_{i \in I}$，使得每个$i \in I$ 都有$\overline{B}_i \subset A_i$，并且很明显，覆盖$(B_i)$ 是局部有限的。根据公理$(O''_V)$，对于每个$i \in I$，都存在一个开集合$C_i$，使得$\overline{B}_i \subset C_i \subset \overline{C}_i \subset A_i$。根据公理$(O_V)$，对于每个$i \in I$，存在$X$到$[0,1]$的连续映射$g_i$，使得$g_i(x) = 1$在$\overline{B}_i$上，并且$\overline{g}_i$的支持包含在$\overline{C}_i$中，并且因此包含在$A_i$中。由于$(B_i)$是$X$的覆盖，因此每个$x \in X$有$\sum_{i \in I} g_i(x) > 0$；如果我们把
$$
f_i(x) = \frac{g_i(x)}{\sum_{i \in I} g_i(x)}
$$
对于所有$i \in I$和所有$x \in X$，则$f_i$形式是单位元的连续划分，从属于覆盖$(A_i)$。

#### 推论{#top-ix-s4-n3-cor-1 .statement tag=0C5U}

*给定任何局部有限开覆盖* $(A_i)$ *闭合集合* $F$ *在正常空间* $X$，*存在一个族* $(f_i)$ *连续实值函数* $\geq 0$ *在* $X$，*从属到覆盖物*$(A_i)_{i \in I}$*并且使得*$\sum_{i \in I} f_i(x) = 1$*对于所有*$x \in F$*和*$\sum_{i \in I} f_i(x) \leq 1$*对于所有*$x \in X$。

$CF$和$A_i$的集合由……组成族是$X$的局部有限开覆盖​​。因此，有一个连续的单位元的划分从属于这个覆盖，一个家庭$(f_i)_{i \in I}$的由……组成使得每个$i \in I$有$\operatorname{Supp}(f_i) \subset A_i$，以及函数$g$，其支持包含在$F$的补数中。家庭$(f_i)$显然满足要求的条件。

### 4. 超紧凑型空间

我们回想一下（章I, § 9, no. 10），如果拓扑空间$X$是豪斯多夫且$X$的每个开覆盖都具有局部有限开细化，则称其为“仿紧”。

#### 命题 4 {#top-ix-s4-prop-4 .statement tag=0C5V}

*每个副紧致空间都是正常的。*

这是以下引理中的推论：

#### 引理 2 {#top-ix-s4-lem-2 .statement tag=0C5W}

*令 $A, B$ 为仿紧紧凑空间 $X$ 的两个不相交的闭子集。 If for each $x \in A$ there is an open neighbourhood $V_x$ of $x$ and an open neighbourhood $W_x$ of $B$ which do not intersect, then there exists an open neighbourhood $T$ of $A$ and an open neighbourhood $U$ of $B$ which do not intersect.*

暂时假设引理为真，我们可以将其应用于$B$由单个点组成的情况，因为$X$是Hausdorff，并且它表明$X$是*正则*。然后我们可以再次将引理 2 应用于$X$的任意两个不相交的闭子集，这表明公理$(O'_V)$是满足的。

为了证明引理，请考虑$CA$和$V_x$的$X$由……组成的开覆盖，其中$x \in A$；令 $(T_i)_{i \in I}$ 为该覆盖层的局部有限开放细化。然后，到定义，如果$A \cap T_i \neq \emptyset$存在$x_i \in A$使得$T_i \subset V_{x_i}$。令$T$为满足$A$的$T_i$的开集合，即并，并证明$B$存在不满足$T$的开邻域$U$。对于每个$y \in B$，都有一个$y$的开邻域$S_y$，仅满足集合$T_i$的有限数；令$J$为指标$i$中$I$由……组成中的有限子集，使得$T_i$同时满足$S_y$和$A$；如果我们放入$U_y = S_y \cap \bigcap_{i \in J} W_{x_i}$，那么$U_y$是$y$的开邻域，它不满足满足$A$的$T_i$，因此$U_y \cap T = \emptyset$。让$U = \bigcup_{y \in B} U_y$；则$U'$是$B$的开邻域，且不满足$T$，且引理得证。

存在非仿紧的正规空间 (习题 19)。

#### 推论 1 {#top-ix-s4-lem-2-cor-1 .statement tag=0C5X}

*给定副紧致空间$X$的任何开放覆盖$(A_i)_{i \in I}$，$x$上存在单位元$(f_i)_{i \in I}$的连续划分，从属于覆盖$(A_i)$。*

令$(U_\lambda)_{\lambda \in L}$为$X$的局部有限开覆盖​​，它细化了覆盖$(A_i)_{i \in I}$；那么就有映射$\varphi : L \to I$，这样每个$\lambda \in L$就有$U_\lambda \subset A_{\varphi(\lambda)}$。到命题 3 和 4，存在从属于 $(U_\lambda)$ 的连续划分单位元 $(g_\lambda)_{\lambda \in L}$。对于每个 $i \in I$，放入

$$
f_i = \sum_{\varphi(\lambda) = i} g_\lambda;
$$

由于 $g_\lambda$ 形式的支撑是局部有限覆盖，因此和是定义且连续的；此外，$g_\lambda$的支撑的并$B_i$使得$\varphi(\lambda) = i$被章I, § 1, no. 6的命题4封闭，并且被包含在$A_i$中。由于每当$x \in \mathbf{C}B_i$时我们就有$f_i(x) = 0$，因此$f_i$的支持包含在$B_i$中，因此也包含在$A_i$中。另一方面，族$B_i$是局部有限的，因为对于每个$x \in X$，$x$有邻域$V$和$I$有有限子集$H$，这样对于所有$\lambda \notin H$都有$V \cap U_\lambda = \emptyset$，并且如下因此，对于所有$i \notin \varphi(H)$，$V \cap B_i = \emptyset$。最后，对于每个$x \in X$，我们有

$$
1 = \sum_{\lambda \in L} g_\lambda(x) = \sum_{i \in I} \left( \sum_{\varphi(\lambda) = i} g_\lambda(x) \right) = \sum_{i \in I} f_i(x),
$$

证明就完成了。

#### 推论 2 {#top-ix-s4-lem-2-cor-2 .statement tag=0C5Y}

*如果 F 是仿紧致空间 X 的闭子集，则 X 包含中 F 的每个邻域都是 F 的闭（因此是仿紧致）邻域。*

到章I, § 9, no. 10的命题16，X的任何闭子空间都是仿紧的；因此，推论来自命题 4 和 Axiom $(O_v')$。

### 5. Metrizable 空间的仿紧性

以下定理锐化命题 2 of no. 1 的结果：

#### 定理 4 {#top-ix-s4-thm-4 .statement tag=0C5Z}

*每个可度量的空间都是仿紧的。*

定理是以下四个引理中的推论。

#### 引理 3 {#top-ix-s4-lem-3 .statement tag=0C60}

*令 $\mathscr{R} = (U_\alpha)_{\alpha \in A}$ 为可测量的空间 X 的开覆盖。然后存在X的开子集的局部有限族序列$(\mathscr{G}_n)$，这样$\mathscr{S} = \bigcup_n \mathscr{S}_n$是X的开覆盖，它细化了$\mathscr{R}$。

令 $d$ 为 X 与其拓扑兼容的度量。对于每个$\alpha \in A$和每个整数$n$，令$F_{n\alpha}$表示所有$x \in U_\alpha$中的集合，使得$d(x, X - U_\alpha) \geq 2^{-n}$。由于$X - U_\alpha$已关闭，我们有$U_\alpha = \bigcup_n F_{n\alpha}$。

有序集合$A$；对于每个$\alpha \in A$和每个整数$n$，令$G_{n\alpha}$为所有$x \in F_{n\alpha}$的集合，使得$x \notin F_{n+1,\beta}$对于所有$\beta < \alpha$，并令$V_{n\alpha}$为所有$y \in X$的集合，使得$d(y, G_{n\alpha}) > 2^{-n-3}$。 $V_{n\alpha}$显然是一个开集合；另一方面，$V_{n\alpha} \subset U_\alpha$，因为对于每个$y \in V_{n\alpha}$，都存在$x \in G_{n\alpha}$使得$d(x, y) \leq 2^{-n-1}$，并且从$x \in F_{n\alpha}$开始，我们有

$$
d(y, X - U_\alpha) \geq d(x, X - U_\alpha) - d(x, y) \geq 2^{-n-1},
$$

这样$y \in U_\alpha$。此外，对于每个$x \in X$，令$\alpha$为$A$中的最小的指标，使得$x \in U_\alpha$；那么有整数$n$使得$x \in F_{n\alpha}$，$\alpha$的定义意味着$x \in G_{n\alpha}$，所以$x \in V_{n\alpha}$。这表明，如果我们放入$\mathfrak{S}_n = (V_{n\alpha})_{\alpha \in A}$，那么$\mathfrak{S} = \bigcup_n \mathfrak{S}_n$是$X$的开覆盖，它细化了$\mathscr{R}$；因此，仍有待证明每个族 $\mathfrak{S}_n$ 都是“局部有限”。为此，我们首先要证明 $d(G_{n\alpha}, G_{n\beta}) \geq 2^{-n-1}$ if $\alpha \neq \beta$。假设$\beta < \alpha$；那么如果$x \in G_{n\alpha}$和$y \in F_{n\beta}$我们有$x \notin F_{n+1,\beta}$乘以定义，因此有$d(x, X - U_\beta) < 2^{-n-1}$和$d(y, X - U_\beta) \geq 2^{-n}$，因此有$d(x, y) \geq 2^{-n-1}$；从$G_{n\beta} \subset F_{n\beta}$开始，断言紧随其后。由此紧接着，使用$V_{n\alpha}$和$V_{n\beta}$中的定义，即$d(V_{n\alpha}, V_{n\beta}) \geq 2^{-n-2}$。从最后的不等式我们推断出，对于每个$z \in X$，具有中心$z$和半径$2^{-n-3}$的开球最多与$\mathfrak{S}_n$族中的一个集合相交；因此$\mathfrak{S}_n$是局部有限族，证明是完备族。

#### 引理 4 {#top-ix-s4-lem-4 .statement tag=0C61}

*令* $(\mathfrak{S}_n)$ *为拓扑空间* $X$ 中开集合局部有限族的序列，*这样*
$$
\mathfrak{S} = \bigcup_n \mathfrak{S}_n
$$
*覆盖* $X$。 *然后存在一个局部有限（但不一定是开放的）覆盖*$\mathscr{B}$*的*$X$*它细化了*$\mathfrak{S}$。

设$E_n$为$X$中的开集合，即$\mathfrak{S}_n$的所有集合中的并；让$U_n$表示$\bigcup_{k=1}^n E_k$，让$A_n$表示$U_n - U_{n-1}$（与$U_0 = \varnothing$）。考虑子集$V \cap A_n$的集合$\mathscr{B}$，其中$V \in \mathfrak{S}_n$和$n$是任意整数；我们将证明$\mathscr{B}$满足条件或引理。对于每个$x \in X$，有整数$n$，使得$x \in A_n$，因为$X$的$A_n$形式划分；因此$x \in E_n$并且存在$V \in \mathfrak{S}_n$使得$x \in V$；所以$x \in V \cap A_n$，我们已经证明了$\mathscr{B}$是$X$的覆盖。显然，这个覆盖精炼了$\mathfrak{S}$。另一方面，对于每个$x \in X$，都存在整数$n$，使得$x \in U_n$；由于 $U_n$ 是开集且 $\mathfrak{S}_m$ 是局部有限族，因此对于$x$ 中的每个$m$，存在邻域 $W_m$，包含在$U_n$ 中，仅满足集合的有限数 $\mathfrak{S}_m$；因此，$x$的邻域$W = \bigcap_{m=1}^n W_m$仅满足$\mathscr{B}$的集合的有限数，因为$W \cap A_p = \varnothing$对于$p > n$。因此$\mathscr{B}$是局部有限的，并且引理4被证明。

#### 引理 5 {#top-ix-s4-lem-5 .statement tag=0C62}

*让* $X$ *成为一个正则空间，使得对于每个开覆盖* $\mathscr{R}$ *of* $X$，*存在一个（不一定是开放的）局部有限覆盖* $\mathscr{U}$ *of* $X$ *精炼* $\mathscr{R}$。 *然后，对于每个开覆盖* $\mathscr{R}$ *of* $X$ *存在一个局部有限的闭覆盖* $\mathfrak{F}$ *of* $X$ *其细化* $\mathscr{R}$。

令$\mathfrak{R}$为$X$的任意开覆盖。对于每个$x \in X$，都有一个开集合$U \in \mathfrak{R}$，其中包含$x$，因此（因为$X$是正则）$x$的开邻域$V_x$，使得$\overline{V}_x \subset U$。由$V_x$形成的族$\mathscr{B}$是$X$的开覆盖，因此到假设时，存在局部有限覆盖$\mathscr{B}'$，其更细比$\mathscr{B}$大。令$\mathscr{F}$为$\mathscr{B}$的集合的闭包族。由于$\overline{V}_x$形成的覆盖$\mathscr{B}'$比$\mathfrak{R}$是更细，并且由于$\mathscr{F}$比$\mathscr{B}'$是更细，所以$\mathscr{F}$是$X$的封闭覆盖，它细化了$\mathfrak{R}$。但$\mathscr{F}$也是局部有限的，因为如果开集合不满足集合$B \in \mathscr{B}$，那么它也不满足其闭包$\overline{B}$。

#### 引理 6 {#top-ix-s4-lem-6 .statement tag=0C63}

*令 $X$ 为 Hausdorff 空间，这样，给定 $X$ 的任何开覆盖 $\mathfrak{R}$，都存在 $X$ 的局部有限闭覆盖 $\mathscr{F}$，它细化了 $\mathfrak{R}$。那么 $X$ 是仿紧的。*

令$\mathfrak{R}$为$X$的任意开覆盖。我们必须证明$X$存在局部有限开覆盖​​，它细化了$\mathfrak{R}$。令 $\mathscr{A}$ 为 $X$ 的局部有限覆盖（封闭或非封闭），它细化了 $\mathfrak{R}$；对于每个$x \in X$，令$W_x$是$x$的开邻域，它仅满足$\mathscr{A}$的集合的有限数。 集合$W_x$的族$\mathscr{W}$是$X$的开覆盖。令 $\mathscr{F}$ 为 $X$ 的局部有限*封闭*覆盖，它细化了 $\mathscr{W}$。对于每个$A \in \mathscr{A}$，令$U_A$为$\mathfrak{R}$的集合，其中包含$A$，并让$C_A$为集合$F \in \mathscr{F}$的并，使得$A \cap F = \varnothing$。由于$\mathscr{F}$是局部有限的，$C_A$在$X$（章I, § 1, no. 6，命题4）中是闭的，因此$A' = U_A \cap (X - C_A)$是开的。由于我们有$A \cap C_A = \varnothing$和$A \subset U_A$，因此$A \subset A'$以及集合$A'$的族$\mathscr{A}'$，因为$A$贯穿$\mathscr{A}$，是$X$的开覆盖；此外，从$A' \subset U_A \in \mathfrak{R}$开始，$\mathscr{A}'$精炼了$\mathfrak{R}$。仍有待证明 $\mathscr{A}'$ 是*局部有限*。对于每个$x \in X$，$x$有邻域$T$，仅满足$\mathscr{F}$的集合的有限数，例如$F_1, \ldots, F_n$。由于每个$F_i$都包含在形式$W_{y_i}$的集合中，因此定义$F_i$仅满足$\mathscr{A}$的集合的有限数；令 $A_{ij}$ ($1 \leq j \leq s_i$) 为集合。如果$A$是$\mathscr{A}$的集合，而不是$A_{ij}$（$1 \leq i \leq n,\ 1 \leq j \leq s_i$）之一，则从定义可以得出，$A'$不满足$F_i$中的任何一个，因此不满足$T \subset \bigcup_{i=1}^n F_i$。这样就完成了引理 6 和定理 4 的证明。

### 习题{#top-ix-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
