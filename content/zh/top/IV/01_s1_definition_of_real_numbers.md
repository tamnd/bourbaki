---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 1
section_title: Definition of real numbers
lang: zh
source: top-i-iv
book_pages: 329-334, 378-381
pdf_pages: 0335-0340, 0384-0387
extraction: ocr
subsections:
    - "no": 1
      title: THE ORDERED GROUP OF RATIONAL NUMBERS
      page: 329
      pdf_page: 335
    - "no": 2
      title: THE RATIONAL LINE
      page: 330
      pdf_page: 336
    - "no": 3
      title: THE REAL LINE AND REAL NUMBERS
      page: 331
      pdf_page: 337
    - "no": 4
      title: PROPERTIES OF INTERVALS IN $\mathbf{R}$
      page: 332
      pdf_page: 338
    - "no": 5
      title: LENGTH OF AN INTERVAL
      page: 333
      pdf_page: 339
    - "no": 6
      title: ADDITIVE UNIFORMITY OF $\mathbf{R}$
      page: 334
      pdf_page: 340
statements: 10
exercises: 4
content_sha256: c367cd463732b7ce94f70ebc70101e6596b16a604421fae5d59bfd7a8b73b7a7
translated_from: content/en/top/IV/01_s1_definition_of_real_numbers.md
translation_method: google
source_content_sha256: f4c12bd1cb845b5f3c66dbac6fe917b0b8b7c5cafbedd83622f13c0a4a7e7248
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: c7022abfdb41f922b813dc3929be55a20ce5e94b93127cafb95884d60d199939
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 1.定义 / 实数

### 1. 有理数数的有序群

我们定义了有理数在集合$\mathbf{Q}$上的排序$x \leq y$；我们已经看到，这种排序使得$\mathbf{Q}$成为*线性排序*集合，并且它与$\mathbf{Q}$的*加法群*结构*相容的*，即对于每个$z \in \mathbf{Q}$关系$x \leq y$等价于$x + z \leq y + z$（即， *顺序在翻译下保持不变*）。我们回想一下记号（用于任何线性排序的群）

$$
x^+ = \sup (x, 0), \\
x^- = \sup (-x, 0) = (-x)^+, \\
|x| = \sup (x, -x);
$$

$|x|$ 被称为 $x$ 的*绝对值*，我们有

$$
x = x^+ - x^-, \qquad |x| = x^+ + x^-
$$

和*三角形不等式*

(1)
$$
|x + y| \leq |x| + |y|,
$$
与不等式一起
(2)
$$
||x| - |y|| \leq |x - y|
$$
这是 (1) 的直接的推论；而且
(3)
$$
|x^+ - y^+| \leq |x - y|.
$$

关系 $x \geq 0,\ x = x^+,\ x^- = 0,\ |x| = x$（分别为$x \leq 0,\ x = -x^-,\ x^+ = 0,\ |x| = -x$）*等效*。 关系 $|x| = 0$相当于$x = 0$；如果$a \geq 0$，关系$|x| \leq a$相当于$-a \leq x \leq a$，关系$|x| \geq a$相当于“$x \geq a$或$x \leq -a$”。对于$\mathbf{Q}$中的所有$x, y$，我们有

(4)
$$
\sup (x, y) + z = \sup (x + z, y + z),
$$
(5)
$$
\inf (x, y) = - \sup (-x, -y),
$$

并且，作为特殊情况，

(6)
$$
\sup (x, y) = x + (y - x)^+ = x + (x - y)^-,
$$
(7)
$$
\inf (x, y) = x - (y - x)^- = x - (x - y)^+.
$$

最后，让$\mathbf{Q}_+$表示有理数数$\geq 0$的集合；那么我们有

(8)
$$
\mathbf{Q}_+ + \mathbf{Q}_+ \subset \mathbf{Q}_+,
$$
(9)
$$
\mathbf{Q}_+ \cap (- \mathbf{Q}_+) = \{ 0 \},
$$
(10)
$$
\mathbf{Q}_+ \cup (- \mathbf{Q}_+) = \mathbf{Q}.
$$

关系 $x \leq y$ *等于* $y - x \in \mathbf{Q}_+$。

我们将在 $\mathbf{Q}$ 上使用此排序来定义 *拓扑与其加法群结构* 相容的。

### 2. 有理线

考虑*对称开区间* $]-a, +a[$的集合$\mathfrak{F}$，其中$a$穿过有理数$> 0$的集合；我们将证明$\mathfrak{F}$是拓扑中*$0$的邻域的*基本系统与$\mathbf{Q}$的加法群结构兼容。

群$\mathbf{Q}$是可交换的，显然满足公理$(\mathrm{GV}'_{\mathrm{II}})$；因此，足以证明公理$(\mathrm{GV}'_{\mathrm{I}})$在其他字中也满足，对于每个$a > 0$，都存在$b > 0$，使得条件$|x| < b$和$|y| < b$一起意味着$|x + y| < a$。三角形不等式表明我们可以取$b = a/2$。

#### 定义 1 {#top-iv-s1-def-1 .statement tag=0BP1}

*有理线是集合$\mathbf{Q}$和加法群拓扑的拓扑空间由……组成，其中对称开区间$]-a, +a[$$(a > 0)$形式是基本系统邻域 $0$。*

*这样定义的拓扑群$\mathbf{Q}$称为有理线的加法群。*

如果$a$是任意有理数数$> 0$，则存在整数$n > 0$使得$1/n < a$；因此，开区间 $]-\frac{1}{n}, +\frac{1}{n}[$ $(n = 1, 2, \ldots)$ 形式是有理线上$0$ 的邻域的基本系统。

通过取开区间$]x - a, x + a[$，我们可以得到任何点$x \in \mathbf{Q}$的邻域的基本系统，其中$a$穿过有理数$> 0$的集合（或数的集合） $1/n$）。

因此，定义 1 相当于章 I, § 1, no. 2 中给出的值。

对于有理数$(a, b)$的每个对使得$a < b$，存在$c \in \mathbf{Q}$使得$a < c < b$[对于例$c = (a + b)/2$]；由此可见，有理线是非离散 Hausdorff 空间。

对于每个$a > 0$，令$U_a$为$\mathbf{Q} \times \mathbf{Q}$中对$(x, y)$的集合，使得$|x - y| < a$。由于$a$贯穿有理数数$> 0$的集合（或者只是数$1/n$的集合），集合$U_a$形式基本系统的一致性有理线的加法群$\mathbf{Q}$。 关系(2)和(3)表明$|x|, x^+$和$x^-$在$\mathbf{Q}$上均匀连续。由此可见，函数、$\sup(x, y)$和$\inf(x, y)$在$\mathbf{Q} \times \mathbf{Q}$上一致连续。

### 3. 实直线和实数

#### 定义 2 {#top-iv-s1-def-2 .statement tag=0BP2}

让$\mathbf{R}$表示拓扑群，它是有理线加法群$\mathbf{Q}$的完成。 $\mathbf{R}$中的元素称为实数；作为拓扑空间，$\mathbf{R}$称为实直线；作为拓扑群，$\mathbf{R}$被称为实直线的加法群。

我们总是将认同$\mathbf{Q}$与$\mathbf{R}$的稠密子群进行规范同构。根据这个约定，每个有理数数都是实数。每个非有理数的实数都被称为无理数；我们在章II, § 3, no. 3中看到这样的数存在（我们将在章的§ 3, no. 3中以另一个的方式展示这一点；另见习题2到§ 2）；因此，无理数数的 (章 III, § 2, no. 1) 集合 $\mathbf{CQ}$ 在 $\mathbf{R}$ 中是稠密的。

我们将证明$\mathbf{Q}$的阶结构可以扩展到$\mathbf{R}$，使得扩展排序仍然与$\mathbf{R}$的加法群结构兼容：

#### 命题 1 {#top-iv-s1-prop-1 .statement tag=0BP3}

关系 $y - x \in \overline{\mathbf{Q}}_+$ 是$\mathbf{R}$ 的排序，使得$\mathbf{R}$ 成为线性排序的集合；与$\mathbf{R}$上的加法群结构兼容，以及$\mathbf{Q}$上的诱导排序$x \leq y$。

我们首先证明关系$y - x \in \overline{\mathbf{Q}}_+$和$z - y \in \overline{\mathbf{Q}}_+$蕴含$z - x \in \overline{\mathbf{Q}}_+$。事实上，函数$x + y$在$\mathbf{R} \times \mathbf{R}$上连续，因此根据(8)我们有$\overline{\mathbf{Q}}_+ + \overline{\mathbf{Q}}_+ \subset \overline{\mathbf{Q}}_+$(章I, § 2, no. 1，定理1)。接下来，我们将证明关系$y - x \in \overline{\mathbf{Q}}_+$和$x - y \in \overline{\mathbf{Q}}_+$蕴含$x = y$；这将确定 $y - x \in \overline{\mathbf{Q}}_+$ 是对 $\mathbf{R}$ 的排序。足以证明$\overline{\mathbf{Q}}_+ \cap (-\overline{\mathbf{Q}}_+) = \{0\}$。现在函数 $x \to x^+$ 和 $x \to x^-$ 在 $\mathbf{Q}$ 上一致连续，因此可以通过连续性扩展到 $\mathbf{R}$ (章 II, , no. 6, 定理 2)；令$f$和$g$分别为扩张。到扩张时，我们为所有 $x \in \mathbf{R}$ 提供了 $x = f(x) - g(x)$； if $x \in \overline{\mathbf{Q}}_+$ then $g(x) = 0$，并且由于 $-\overline{\mathbf{Q}}_+$ 是 $-x$ 连续性对 $-\mathbf{Q}_+$ 的闭包，因此可以得出 if $x \in -\overline{\mathbf{Q}}_+$ then $f(x) = 0$。因此，如果 $x \in \overline{\mathbf{Q}}_+ \cap (-\overline{\mathbf{Q}}_+)$ 我们有 $f(x) = g(x) = 0$ 因此 $x = 0$

根据 (10)，我们得到 $\overline{\mathbf{Q}}_+ \cup (-\overline{\mathbf{Q}}_+) = \mathbf{R}$，因此 $\mathbf{R}$ 按$y - x \in \overline{\mathbf{Q}}_+$ *线性排序*。

此外，由于关系$y - x \in \overline{\mathbf{Q}}_+$和$(y + z) - (x + z) \in \overline{\mathbf{Q}}_+$是等价的，因此$y - x \in \overline{\mathbf{Q}}_+$的排序与$\mathbf{R}$的加法群结构兼容。

最后，如果 $x$ 和 $y$ 属于到 $\mathbf{Q}$ 关系 $y - x \in \overline{\mathbf{Q}}_+$ 和 $y - x \in \mathbf{Q}_+$ 等价，因此关系 $y - x \in \overline{\mathbf{Q}}_+$ 诱导关系 $x \leq y$ $\mathbf{Q}$。这样就完成了证明。

关系$y - x \in \overline{\mathbf{Q}}_+$再次表示为$x \leq y$。 集合$\overline{\mathbf{Q}}_+$是$\mathbf{R}$中所有$x \geq 0$的集合，记为$\mathbf{R}_+$；这是一个*封闭的集合*。所有$x > 0$中的集合用$\mathbf{R}_+^*$表示；它是$-\mathbf{R}_+$的补集，因此在$\mathbf{R}$中“开”。

### 4. $\mathbf{R}$ 中的区间性质

#### 命题 2 {#top-iv-s1-prop-2 .statement tag=0BP4}

*$\mathbf{R}$ 中的每个闭（或开）区间都是 $\mathbf{R}$ 中的闭（或开）集合。*

集合 $[a, \to[ = a + \mathbf{R}_+$和$]\leftarrow, a] = a - \mathbf{R}_+$分别由$\mathbf{R}_+$和$-\mathbf{R}_+$翻译得到，因此是闭的（章III, § 1, no. 1）； 集合 $]\leftarrow, a[$ 和 $]a, \to[,$ 是它们的补集，开；最后，闭区间$[a, b]$（或开区间$]a, b[$）是$[a, \to[$和$]\leftarrow, b]$（分别是$]a, \to[$和$]\leftarrow, b[$）的交，因此是闭（或开）集合。

因此，$\mathbf{R}$ 中的闭区间 $[-a, +a]$ ($a > 0$) 为 0 的邻域。 让我们证明，当 $a$ 穿过 $\mathbf{R}_+^*$ 时，它们形式和邻域* 的 *基本系统为 0。为此，建立以下命题就足够了：

#### 命题 3 {#top-iv-s1-prop-3 .statement tag=0BP5}

*由于$r$贯穿有理数$> 0$的集合，$\mathbf{R}$形式中的区间$s_r = [-r, +r]$是邻域的基本系统为0。*

通过章III, § 3, no. 4的命题7，我们通过在$\mathbf{R}$中取区间的*闭包*，获得$\mathbf{R}$中0的邻域的基本系统

S_r \cap \mathbf{Q} = [-r, +r] \textit{of} \mathbf{Q}。如果我们证明 S_r 是 S_r \cap \mathbf{Q} 的闭包，证明就完整了。现在 S_r 在 \mathbf{R} 中是闭包，因此我们只需证明，如果 x 是实数且 -r < x < r，则 x 在 S_r \cap \mathbf{Q} 的闭包中。区间 ]-r, +r[ 是 \mathbf{R} 中的开集合，因此对于 \mathbf{R} 中所有足够小的 o 邻域 V，我们有 x + V \子集 ]-r, +r[;但 \mathbf{Q} 在 \mathbf{R} 中是稠密的，因此在 x + V 中存在有理数数 r' \，因此 -r < r' < r，因此在 S_r \cap \mathbf{Q} 中存在 r' \。

#### 推论{#top-iv-s1-n4-cor-1 .statement tag=0BP6}

*实直线的每个点都有一个邻域的可数基数系统。*

#### 命题 4 {#top-iv-s1-prop-4 .statement tag=0BP7}

*如果 (x, y) 是实数中的任意对，并且 x < y，则存在有理数数 r，使得 x < r < y。*

由于 \mathbf{Q} 在 \mathbf{R} 中是稠密的，因此只要证明 ]x, y[ 不为空即可；通过翻译，我们可以假设 x = 0 且 y > 0。现在 \mathbf{R} 是 Hausdorff 空间，因此，通过命题 3，存在有理数数 r > 0，使得 y \notin ]-r, +r[，这意味着 0 < r < y。

#### 命题 5 {#top-iv-s1-prop-5 .statement tag=0BP8}

*设I为\mathbf{R}中的任意区间。然后由I的开区间生成\mathbf{R}的拓扑在I上诱导的拓扑（其中I被认为是按关系 x \leq y线性排序）。*

每个I开区间都是\mathbf{R}开区间在I上的迹。对于有界区间来说这是很清楚的，I的无界区间 ]a, \to[ 是 \mathbf{R} 的无界区间 ]a, \to[ 的迹。因此，我们可以将自己限制在 I = \mathbf{R} 的情况；但在这种情况下，结果来自命题 3，因为点 x \in \mathbf{R} 包含的每个邻域都是开区间 ]x - a, x + a[。

#### 注 {#top-iv-s1-n4-rem-1 .statement tag=0BP9}

如果 A 是 \mathbf{R} 的稠密子集，则 \mathbf{R} 的拓扑由其端点属于到 A 的开区间生成。

$$ ]x - a, x + a[ $$

是开区间包含 x，A 存在两个点 y, z 使得 x - a < y < x 且 x < z < x + a；因此 ]y, z[ 包含于 x 并且包含在 ]x - a, x + a[ 中。此外，这个证明还显示了\mathbf{R}的拓扑所考虑的区间形式基(章I, § 1, no. 3)。特别是，如果我们取 A = \mathbf{Q}，我们会看到 \mathbf{R} 的拓扑具有可数的基。

### 5. 区间的长度

#### 定义 3 {#top-iv-s1-def-3 .statement tag=0BPA}

*具有端点 a 和 b (a \leq b) 的有界区间的长度定义为 b - a。*

因此，包含大于 1 个点的每个有界区间都具有长度 > 0。如果 $a \leq b$，则四个区间 $[a, b], ]a, b[, [a, b[$ 和 $]a, b[$ 都具有相同的长度。端点为 $a + c$ 和 $b + c$ 的区间与端点为 $a$ 和 $b$ 的区间具有相同的长度；在其他字中，间隔的*长度在平移下是不变的*。

如果$a \leq c \leq d \leq b$我们有$d - c \leq b - a$。因此，如果有界区间$I$包含在有界区间$I'$中，则$I$的长度小于或等于$I'$的长度。

如果$n$互为不相交的开区间$I_1, I_2, \ldots, I_n$包含在区间$[a, b]$（$a < b$）中，则由$n$上的归纳很容易看出，如果$I_k = ]c_k, d_k[$，则存在指标的置换$\sigma$ $k$ ($1 \leq k \leq n$) 使得$d_{\sigma(k)} \leq c_{\sigma(k+1)}$ 为$1 \leq k \leq n - 1$。紧接着，区间$I_k$的长度的和至多等于$[a, b]$的长度，并且等式成立当且仅当对于$1 \leq k \leq n - 1$有$c_{\sigma(1)} = a, d_{\sigma(n)} = b$和$d_{\sigma(k)} = c_{\sigma(k+1)}$。

### 6. $\mathbf{R}$ 的加性均匀性

由于群 $\mathbf{R}$ 是线性排序的，函数 $x^+, x^-$ 和 $|x|$ 在 $\mathbf{R}$ 上的定义方式与 $\mathbf{Q}$ 和满足相同，上面为 $\mathbf{Q}$ 列出了所有关系，特别是关系 (1)至(7)。令$a$为实数 > 0，并令$U_a$为所有对$(x, y) \in \mathbf{R} \times \mathbf{R}$中的集合，使得$|x - y| < a$；由于$a$贯穿实数>0的集合（或数$1/n$的集合），集合$U_a$形式基本系统的一致性实直线的加法群$\mathbf{R}$（称为*实直线*的加性均匀性）。

函数 $|x|$、$x^+$ 和 $x^-$ 在 $\mathbf{R}$ 上“均匀连续”，函数 $\sup(x, y)$ 和 $\inf(x, y)$ 在 $\mathbf{R} \times \mathbf{R}$ 上“均匀连续”；这些函数因此重合以及通过分别在$\mathbf{Q}$和$\mathbf{Q} \times \mathbf{Q}$上定义的连续性扩展相应的函数获得的相应的函数。

### 习题 {#top-iv-s1-exercises}

§ 1](exercises/s1/)参见[习题。
