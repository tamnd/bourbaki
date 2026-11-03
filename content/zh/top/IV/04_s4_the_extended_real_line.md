---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 4
section_title: The extended real line
lang: zh
source: top-i-iv
book_pages: 342-347, 388-389
pdf_pages: 0348-0353, 0394-0395
extraction: ocr
subsections:
    - "no": 1
      title: HOMEOMORPHISMS OF OPEN INTERVALS OF $\mathbf{R}$
      page: 342
      pdf_page: 348
    - "no": 2
      title: THE EXTENDED LINE
      page: 343
      pdf_page: 349
    - "no": 3
      title: ADDITION AND MULTIPLICATION IN $\overline{\mathbf{R}}$
      page: 345
      pdf_page: 351
statements: 11
exercises: 7
content_sha256: 782dbed07719f652e594d4921c13c11e2cc54783b8f36afbe6e1db2d0b5f90f2
translated_from: content/en/top/IV/04_s4_the_extended_real_line.md
translation_method: google
source_content_sha256: 91dd5beb94c7b102f68de8b003d98eed8682578549dc7b95cc038872a79f0294
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 44dd10c616cc691f9f95145cb6f3e77f6bddd1d93ee7a6cf6170493ac094f602
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 4. 扩展的实直线

### 1. $\mathbf{R}$ 的开区间同态

#### 命题 1 {#top-iv-s4-prop-1 .statement tag=0BQK}

$\mathbf{R}$ 的所有非空开区间都同胚于 $\mathbf{R}$。

首先考虑有界开区间 $I = ]a, b[$ ($a < b$)。对于每个$x \in I$，放入$f(x) = -\left( \frac{1}{x-a} + \frac{1}{x-b} \right)$。这个函数是连续的，严格递增的在$I$上，因为我们已经看到$\frac{1}{x-b}$在$]-, b[$中是严格递减，而$\frac{1}{x-a}$在$]a, \to[$中是严格递减。由此可见，$f$是$I$到$\mathbf{R}$的区间$f(I)$的同胚（§ 2, no. 6，定理5）。 $f(I)$ 既不上界也不下界；例如，如果我们对所有 $x \in I$ 都有 $f(x) \leq c$，那么从 $b-x > 0$ 开始，就会得出 $1 - \frac{b-x}{x-a} \leq c(b-x)$；当$x$足够接近$b$时（由于不等式两侧的连续性，在点$b$处是有理函数），这会导致矛盾。因此$f(I) = \mathbf{R}$，因此每个有界开区间同胚于$\mathbf{R}$。令$g$是$f$的逆：它映射$\mathbf{R}$的每个无界开区间到$I$中包含的区间$J$并在$I$中开。由于$I$在$\mathbf{R}$开放，$J$也在$\mathbf{R}$开放；因为它是有界的，所以它同胚于 $\mathbf{R}$；因此我们证明了每个无界开区间同胚于$\mathbf{R}$。

#### 注 {#top-iv-s4-n1-rem-1 .statement tag=0BQL}

为了证明所有*有界*开区间彼此同胚，只需指出，如果 $a \neq b$ 和 $a' \neq b'$，则存在 $\mathbf{R}$ 自身同胚，形式 $x \to ax + \beta$（且只有一个），其中映射 $a$ 与$a'$ 和 $b$ 到 $b'$，因此映射带有端点 $a, b$ 的开路（分别为半开、闭路） 区间到开路（分别为半开、闭路）区间与端点 $a', b'$；读者可以通过计算$\alpha$和$\beta$轻松验证这一点。

### 2. 延长线

现在，我们将通过将两个新元素“邻接”到$\mathbf{R}$来定义一个拓扑空间$\overline{\mathbf{R}}$，使得$\mathbf{R}$在$\mathbf{R}$的有界开区间$I$上的每个同态都可以扩展到与$I$具有相同端点的闭区间上的$\overline{\mathbf{R}}$同态。

设$\overline{\mathbf{R}}$为集合，通过将(*集合理论*, R, § 4, no. 5)两个新的元素与$\mathbf{R}$相邻而获得，记为$-\infty$和$+\infty$。我们将$-\infty < a$和$a < +\infty$放在所有$a \in \mathbf{R}$和$-\infty < +\infty$上，对$\mathbf{R}$到$\overline{\mathbf{R}}$进行扩展排序；显然，我们由此得到了一个线性排序的集合，其排序诱导是实直线在$\mathbf{R}$上的排序。接下来，考虑由 $\overline{\mathbf{R}}$ 的开放区间的集合生成的 $\overline{\mathbf{R}}$ 上的拓扑。由于$\overline{\mathbf{R}}$的开区间在$\mathbf{R}$上的轨迹是$\mathbf{R}$的开区间，因此实直线的$\mathbf{R}$拓扑上的拓扑诱导。

#### 定义 1 {#top-iv-s4-def-1 .statement tag=0BQM}

*集合* $\overline{\mathbf{R}}$ *赋予上面定义的阶结构和拓扑称为扩展实直线。*

当使用延长线$\overline{\mathbf{R}}$时，通常为了方便而将其点称为*实数*，这是滥用语言； $\mathbf{R}$ 的点被称为*有限实数*。我们将在这个截面以及这个章的以下三个截面*中采用这个约定；将来每当我们采用此约定时，我们都会明确指出文本中的哪个部分是扩展。

如果$a$是有限实数，$\overline{\mathbf{R}}$的区间、$[a, +\infty[$和]—$\infty, a]$（分别为]$a, +\infty[$和]—$\infty, a[$）包含在$\mathbf{R}$和重合中$\mathbf{R}$的区间迄今为止由$[a, \rightarrow[$和]$\leftarrow, a]$表示（分别为]$a, \rightarrow[$和]$\leftarrow, a[$）；这个新的记号使用得更频繁。再次，$\mathbf{R}$重合与$\overline{\mathbf{R}}$的区间]—$\infty, +\infty[$，并且有时如此表示。

#### 命题 2 {#top-iv-s4-prop-2 .statement tag=0BQN}

*每个同态* $f$ *of* $\mathbf{R}$ *到区间* ]$a, b[$ *都可以扩展到同态* $\overline{f}$ *of* $\overline{\mathbf{R}}$ *到* $[a, b]$。 *如果*$f$*是递增函数，那么*$\overline{f}$*是*$\overline{\mathbf{R}}$*的阶同构*到*$[a, b]$。

设$f$为递增同胚。如果我们将$\overline{f}(-\infty) = a$和$\overline{f}(+\infty) = b$从扩展$f$到$\mathbf{R}$，很明显$\overline{f}$是$\overline{\mathbf{R}}$的严格递增的映射（因此双射） $[a, b]$。因此$\overline{f}$映射每个$\overline{\mathbf{R}}$的开区间到区间，区间相对于$[a, b]$开，因此由于定义1而成为$\mathbf{R}$到$[a, b]$的同胚命题 5 个，共 § 1, no. 4。

如果$f$是递减，我们将$\mathbf{R}$的递增同胚$x \to -f(x)$应用到]$-b, -a[$。

在§ 2中获得的区间$[a, b]$的所有属性，仅涉及区间的阶结构和拓扑，因此可以转移到$\overline{\mathbf{R}}$；因此有以下命题：

#### 命题 3 {#top-iv-s4-prop-3 .statement tag=0BQO}

*扩展的实直线是紧凑的。*

因此 (章 II, § 4, no. 1, 定理 1) $\overline{\mathbf{R}}$ 具有与其拓扑兼容的独特一致性；该均匀性与 $\mathbf{R}$ 的加法均匀性在 $[a, b]$ 上引起的均匀性是同构的。但需要注意的是，$\overline{\mathbf{R}}$在$\mathbf{R}$上*诱导*的均匀性*不是*$\mathbf{R}$的加法均匀性（尽管它与实直线的拓扑兼容）；因为 $\mathbf{R}$ 就其加性均匀性而言是一个*完整* 空间，但不是 $\overline{\mathbf{R}}$ 的完整子空间，因为它在 $\overline{\mathbf{R}}$ 中不是封闭的。

#### 命题 4 {#top-iv-s4-prop-4 .statement tag=0BQP}

** $\overline{\mathbf{R}}$ *中的每个非空子集 *至少有上界和下确界。*

$\mathbf{R}$ 的非空子集 $A$ 中的最小上界（或下确界）由$\sup A$（或$\inf A$）表示。显然

(1)
$$
\inf A \leq \sup A.
$$

如果$A \subset B$，则$\sup A \leq \sup B$和$\inf A \geq \inf B$（*集合理论*，章III, § 1, no. 9，命题4）。

#### 命题 5 {#top-iv-s4-prop-5 .statement tag=0BQQ}

*当且仅当$A$为区间时，$\overline{\mathbf{R}}$的子集$A$连通。*

#### 推论 {#top-iv-s4-n2-cor-1 .statement tag=0BQR}

*扩展实直线是一个连接的、本地连接的空间。*

#### 命题 6 {#top-iv-s4-prop-6 .statement tag=0BQS}

*$\overline{\mathbf{R}}$的区间$I$到$\overline{\mathbf{R}}$的映射$f$是$I$到$f(I)$的同胚当且仅当$f$在$I$上严格单调且连续；那么$f(I)$就是$\overline{\mathbf{R}}$的区间。

最后，函数$\sup(x, y)$和$\inf(x, y)$在$\overline{\mathbf{R}} \times \overline{\mathbf{R}}$上*连续*。

### 3. 加法和乘法 $\overline{\mathbf{R}}$

注首先根据公式$-(-\infty) = +\infty$和$-(+\infty) = -\infty$，函数$-x$可以通过连续性扩展到$\overline{\mathbf{R}}$；由此扩展出的函数是$\overline{\mathbf{R}}$自身的同胚。

接下来，考虑函数、$x + y$和$xy$，定义在$\mathbf{R} \times \mathbf{R}$上，值定义在$\mathbf{R}$上；通过考虑它们在拓扑空间* $\overline{\mathbf{R}}$中取值*，我们将看到它们也可以通过$\overline{\mathbf{R}} \times \overline{\mathbf{R}}$的某些点的连续性进行扩展。

就$x + y$而言，设$A' = ]-\infty, +\infty]$和$A'' = [-\infty, +\infty[$。那么我们有以下命题：

#### 命题 7 {#top-iv-s4-prop-7 .statement tag=0BQT}

*函数$x + y$可以根据公式通过连续性扩展到集合$A' \times A'$和$A'' \times A''$*

$$
(2)
\begin{cases}
x + (+\infty) = (+\infty) + x = +\infty & (x \neq -\infty), \\
x + (-\infty) = (-\infty) + x = -\infty & (x \neq +\infty).
\end{cases}
$$

例如，让我们证明，当 $(x, y)$ 趋向于点 $(a, +\infty)$ ($a \neq -\infty$)，同时保持在 $\mathbf{R} \times \mathbf{R}$ 时，$x + y$ 趋向于 $+\infty$。存在有限的数$b < a$，区间$]b, +\infty[$是$\mathbf{R}$中$a$的邻域；给定任何有限的$c$、关系、$x > b$和$y > c - b$意味着$x + y > c$，这表明只要$(x, y)$足够接近$(a, +\infty)$，$x + y$就尽可能接近$+\infty$。其他情况下的论证也类似。

相反，$x + y$在$\overline{\mathbf{R}} \times \overline{\mathbf{R}}$的点$(-\infty, +\infty)$和$(+\infty, -\infty)$*没有限制*。 因为如果$x + y$有极限$k$（有限或无限），因为$(x, y)$趋向于$(+\infty, -\infty)$，同时保持在$\mathbf{R} \times \mathbf{R}$，那么对于每个有限的$a$，函数$(x + a) - x$将趋向于$k$，如下$x$趋于$+\infty$，同时保持在$\mathbf{R}$；这是荒谬的，因为 $(x + a) - x = a$ 和 $a$ 是任意的。

函数 $x + y$ 映射 $A' \times A'$（分别$A'' \times A''$）到$A'$（分别$A''$）。因此，$A'$（或$A''$）上的合成的律，以及$\mathbf{R}$上的加法的扩展律。通过恒等式扩张的原理 (章 I, , no. 1, 推论 1 到命题 2)，这个律是可交换和结合的； o 对于这个律来说是单位元素； $A'$ 的唯一非常规元素 (代数, 章 I, § 2, no. 2) 是 $+ \infty$, by 公式 (2)

如果$x, y, z, t$是$\overline{\mathbf{R}}$的点，使得$x \leq y$和$z \leq t$，则只要定义了不等式的两侧，$x + z \leq y + t$。

请注意，仅当 $z$ 是有限的（通过公式 (2)）时，$\overline{\mathbf{R}}$ 关系 $x < y$ 才意味着 $x + z < y + z$；很容易验证只要定义了不等式的两边，关系$x < y$和$z < t$就意味着$x + z < y + t$。

在$\overline{\mathbf{R}}$中我们放入$x^+ = \sup (x, 0), x^- = \sup (-x, 0), |x| = \sup (x, -x)$；因此$(+\infty)^+ = (-\infty)^- = +\infty$和$(+\infty)^- = (-\infty)^+ = 0$，以及$|+\infty| = |- \infty| = +\infty$。 和、$x^+ - x^-$和$x^+ + x^-$是为所有$x \in \overline{\mathbf{R}}$定义的，因此分别等于$x$和$|x|$等式的原理或扩张。此外，每当定义和 $x + y$ 时，我们就有 $|x + y| \leq |x| + |y|$。

注相反，§ 1, no. 1的公式（6）和（7）对于$\overline{\mathbf{R}}$中的$x$和$y$的某些值可能不再有意义；例如，如果$x = -\infty$和$y = 0$我们有$\sup (x, y) = 0$，但和$x + (y - x)^+$没有定义，因为$(y - x)^+ = +\infty$。

令$\overline{\mathbf{R}}^*$表示$\overline{\mathbf{R}}$中o的补集。那么命题 7 对应乘法的模拟运行如下：

#### 命题 8 {#top-iv-s4-prop-8 .statement tag=0BQU}

*函数 xy 可以根据公式连续性扩展到集合$\overline{\mathbf{R}}^* \times \overline{\mathbf{R}}^*$*

$$
\begin{cases}
x.(+\infty) = (+\infty).x = \begin{cases} +\infty & \text{if } x > 0 \\ -\infty & \text{if } x < 0 \end{cases} \\
x.(-\infty) = (-\infty).x = \begin{cases} -\infty & \text{if } x > 0 \\ +\infty & \text{if } x < 0. \end{cases}
\end{cases}
$$

(3)

我们把证明留给读者；它类似于命题 7 的证明。

同样，我们看到$xy$在$\overline{\mathbf{R}} \times \overline{\mathbf{R}}$的点$(0, +\infty), (+\infty, 0), (0, -\infty), (-\infty, 0)$处没有极限。

函数 $xy$ 是$\overline{\mathbf{R}}^*$ 合成律，其中 $\mathbf{R}$ 乘法扩展律；这个律是结合律和交换律的（恒等式的扩张中的原理）；它的 1 为单位元素； $\overline{\mathbf{R}}^*$中的非常规元素是$+\infty$和$-\infty$。

如果$x \leq y$和$z > 0$，只要定义了不等式的两边，我们就有$xz \leq yz$。如果定义了乘积$xy$，那么$|x| \cdot |y|$也定义了，我们就有了$|xy| = |x| \cdot |y|$。

最后分配律公式

$$
x(y + z) = xy + xz
$$

凭借恒等式的原理或扩张，只要定义了两侧的所有运算，仍然有效。

请注意，可能会发生 (4) 的左侧已定义而右侧未定义的情况：例如，考虑 $x = +\infty$、$y = 2$ 和 $z = -1$ 的情况。因此，在 $\overline{\mathbf{R}}$ 中应谨慎使用分配律公式。

### 习题 {#top-iv-s4-exercises}

请参阅[习题为 § 4](exercises/s4/)。
