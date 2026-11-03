---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 3
section_title: The field of real numbers
lang: zh
source: top-i-iv
book_pages: 339-342, 387-388
pdf_pages: 0345-0348, 0393-0394
extraction: ocr
subsections:
    - "no": 1
      title: MULTIPLICATION IN $\mathbf{R}$
      page: 339
      pdf_page: 345
    - "no": 2
      title: THE MULTIPLICATIVE GROUP $\mathbf{R}^*$
      page: 340
      pdf_page: 346
    - "no": 3
      title: '*n*TH ROOTS'
      page: 341
      pdf_page: 347
statements: 2
exercises: 3
content_sha256: 1a94ad01bcb2a160e6a25e1195c1cbea244b0c8f62655b11cb1e67451e16052d
translated_from: content/en/top/IV/03_s3_the_field_of_real_numbers.md
translation_method: google
source_content_sha256: afbf19bbf21fbfe05f4ab076c9028768c17367d06c4224c3286d307ed17aa711
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 7c18f9435ec74d5f54d0edef2c6aad35dd916f151230a9761e42fe1ea6d3d7ec
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 3. 域 / 实数

### 1. 乘法 $\mathbf{R}$

有理线$\mathbf{Q}$的拓扑不仅与加法群* 结构兼容，还与$\mathbf{Q}$的*域* 结构兼容。对于函数$xy$在$(0, 0) \in \mathbf{Q} \times \mathbf{Q}$连续，因为对于每个整数$n > 0$关系$|x| \leq 1/n$和$|y| \leq 1/n$一起意味着$|xy| \leq 1/n^2 \leq 1/n$；另一方面，如果 $a$ 是任何非零有理数数，则函数 $ax$ 在 $x = 0$ 处连续，因为对于每个整数 $n > 0$ 关系 $|x| \leq 1/|n|a|$ 都意味着 $|ax| \leq 1/n$。这表明$xy$在$\mathbf{Q} \times \mathbf{Q}$的每点处连续（章III, § 6, no. 3）。

为了证明 $1/x$ 在 $\mathbf{Q}^*$ 上连续，我们应该更精确地证明 $1/x$ 在 0 的任何邻域 V 的补集中是“一致连续”（相对于加法结构）。即我们有 $$
\left| \frac{1}{x} - \frac{1}{y} \right| = \frac{|x-y|}{xy}
$$；存在整数$m > 0$，使得每个$x \in \mathfrak{G}_V$都有$|x| \geq 1/m$；如果$x$和$y$是$\mathfrak{G}_V$中的任意两个点使得$|x-y| \leq 1/m^2 n$，那么我们将有$$
\left| \frac{1}{x} - \frac{1}{y} \right| \leq \frac{1}{n}.
$$

像，在函数 $1/x$ 下，$\mathbf{Q}^*$ 上的任何柯西滤波器（相对于加性均匀性）不具有 0 作为簇点，是柯西滤波器（相对于加性均匀性）。因此 (章 III, , no. 8, 命题 7)

#### 命题 1 {#top-iv-s3-prop-1 .statement tag=0BQF}

*分别在$\mathbf{Q} \times \mathbf{Q}$和$\mathbf{Q}^*$上定义的函数xy和$1/x$，可以通过连续性分别扩展到$\mathbf{R} \times \mathbf{R}$和$\mathbf{R}^*$，以及$\mathbf{R}$上的定义域结构。有了这个结构，$\mathbf{R}$就被称为实数的域。*

在章III的§ 6中建立的拓扑域的所有性质当然都适用；特别是，$n$实数变量的每个*有理数函数*，以及实数系数，在$\mathbf{R}^n$的每个点都是*连续的，其中分母不会消失。

### 2. 乘法群$\mathbf{R}^*$

从章III, § 6, no. 7我们知道，实直线的拓扑在$\mathbf{R}^*$上诱导的拓扑与$\mathbf{R}^*$的乘法群结构*相容的*；由于$\mathbf{R}^*$是局部紧致空间$\mathbf{R}$的*开*子集，因此$\mathbf{R}^*$是*局部紧致*拓扑群（章I, § 9, no. 7，命题13），因此*完整*（章III, § 3, no. 3，推论1到命题4；这也来自章III, § 6, no. 8，命题8）；当然，后者性质涉及$\mathbf{R}^*$上的“乘法”均匀性，而不涉及$\mathbf{R}^*$上由$\mathbf{R}$的加法均匀性引起的均匀性。

函数 $xy$ 映射集合 $\mathbf{Q}_+ \times \mathbf{Q}_+$ 变成$\mathbf{Q}_+$，因此映射 $\mathbf{R}_+ \times \mathbf{R}_+$ 变成$\mathbf{R}_+$ (章 I, § 2, no. 1, 定理 1)；在其他字中，两个实数$\geqslant 0$中的*乘积是$\geqslant 0$*。 公式$(-x)y = -xy$和$(-x)(-y) = xy$则表明数$\geqslant 0$和数$\leqslant 0$的乘积是$\leqslant 0$，以及两个数$\leqslant 0$的乘积是 $\geqslant 0$；由此可见

$$(1)$$
$$|xy| = |x| \cdot |y|$$

（也可能是通过 $\mathbf{Q} \times \mathbf{Q}$ 相应的关系的扩张获得的）。

如果$x > 0$和$y > 0$我们有$xy \neq 0$，因此$xy > 0$；同样，如果$x < 0$和$y > 0$，则$xy < 0$；如果$x < 0$和$y < 0$，则$xy > 0$。特别是，如果$x \neq 0$我们有$x^2 > 0$，那么实数不能的平方*的*和是零除非，每个数都是零。

如果$x > 0$和$y \leqslant z$（或$y < z$），我们在其他字、*位似的比率* $> 0$ *保留阶在* $\mathbf{R}$上有$xy \leqslant xz$（或$xy < xz$）。从$(-x)y = -xy$开始，位似的比率为$< 0$变换，对$\mathbf{R}$的排序变为相反的排序。

如果$x > 0$我们有$1/x > 0$，因为$x.(1/x) = 1 > 0$。如果$0 < x < y$我们有$xy > 0$，因此$x.(1/xy) < y.(1/xy)$，那就是$1/y < 1/x$。因此，实数$> 0$的集合$\mathbf{R}_+^*$的映射$x \to 1/x$本身就是严格递减。

我们以同样的方式看到，函数$1/x$在]$\leftarrow, 0[$中是严格递减，因此函数$\frac{1}{x-a}$在区间]$\leftarrow, a[$和$]a, \to[$中都是严格递减。

由上可知，$\mathbf{R}_+^*$是乘法群$\mathbf{R}^*$的子群；此外，序关系$x \leq y$与$\mathbf{R}_+^*$的乘法群结构兼容；在其他字中，$\mathbf{R}_+^*$是线性有序的群。

两个实数$\geq 0$中的乘积是$\geq 0$，可以用说表示$\mathbf{R}$是有序域：以上所有性质对于所有有序域来说都是公共的。

#### 命题 2 {#top-iv-s3-prop-2 .statement tag=0BQG}

*实数$\neq 0$的乘法群$\mathbf{R}^*$是群拓扑同构于其子群$\mathbf{R}_+^*$和$\mathbf{U}_0$的乘积，其中*

$$
\mathbf{U}_0 = \{ -1, +1 \}.
$$

对于每个$x \neq 0$，让$\operatorname{sgn} x$表示$\frac{x}{|x|}$（*$x$的符号*）。 函数 $\operatorname{sgn}$ 是 $\mathbf{R}^*$ 的同态到 $\mathbf{U}_0$。我们有$x = |x|\operatorname{sgn} x$，$x$的这个分解与$\mathbf{R}_+^*$的元素乘积和$\mathbf{U}_0$的元素是唯一的；因此$\mathbf{R}^*$的群结构是$\mathbf{R}_+^*$和$\mathbf{U}_0$的群结构的乘积。另一方面，映射$x \to |x|$是连续的，$x \to \operatorname{sgn} x = \frac{x}{|x|}$也是连续的，因为$x \neq 0$。于是就有了这样的结果。
我们通过放入 $\operatorname{sgn} 0 = 0$ 将扩展函数 $\operatorname{sgn}$ 变为整个 $\mathbf{R}$。

我们将在章V（§ 4, no. 1，定理1）中看到拓扑群$\mathbf{R}_+^*$与*加法*群$\mathbf{R}$*同构的；这将完成拓扑群$\mathbf{R}_*$的结构的确定。

### 3. *n*TH 根

令 $n$ 为任意整数 $> 0$。从关系$0 < x < y$，我们通过$n$上的归纳推出$0 < x^n < y^n$。在其他字中，函数$x \to x^n$对于$x \geq 0$来说是*严格递增的*；它显然在每个点连续，因此（§ 2, no. 6，定理5）它是$\mathbf{R}_+$到区间$I$的同胚。另一方面，由于 $x \geqslant 1$ 蕴涵 $x^{n-1} \geqslant 1$ 并因此蕴含 $x^n \geqslant x$，因此 $I$ 是无界的，因此$I = \mathbf{R}_+$ 也是无界的。 值，对于$x \geqslant 0$，映射$x \to x^n$的倒数用$x^{1/n}$或$\sqrt[n]{x}$表示，称为$x$到幂$1/n$或第n个根 $x$（对于$n = 2, 3$，我们说平方根，立方根；对于$n = 2$，我们写$\sqrt{x}$代替$\sqrt[2]{x}$）。因此，正值数 $x^{1/n}$ 被定义为方程的唯一正值解

$$
y^n = x \quad (x \geqslant 0).
$$

特别是我们看到存在实数$x$使得$x^2 = 2$，而没有有理数有这个性质；这样我们就恢复了有理线$\mathbf{Q}$不是完整的空间这一事实。

$\mathbf{R}_+$的映射$x \to x^{1/n}$自身是严格递增的且连续。由(2)我们有$0^{1/n} = 0, 1^{1/n} = 1$，也

$$
(xy)^{1/n} = x^{1/n} y^{1/n};
$$

因此$x \to x^{1/n}$是拓扑群$\mathbf{R}_+^*$的自同构。

在章V, § 4, no. 1中，我们将通过找到乘法群$\mathbf{R}_+^*$的所有自同构来推广这个结果。

### 习题 {#top-iv-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
