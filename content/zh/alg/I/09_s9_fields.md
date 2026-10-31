---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 9
section_title: Fields
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 114-118, 174-179
pdf_pages: 0138-0142, 0198-0203
extraction: ocr
subsections:
    - "no": 1
      title: FIELDS
      page: 114
      pdf_page: 138
    - "no": 2
      title: INTEGRAL DOMAINS
      page: 116
      pdf_page: 140
    - "no": 3
      title: PRIME IDEALS
      page: 116
      pdf_page: 140
    - "no": 4
      title: THE FIELD OF RATIONAL NUMBERS
      page: 117
      pdf_page: 141
statements: 17
exercises: 21
content_sha256: 2836a17c387ff868e38dbd0e8db94af345851e99314b0c44f13123ac7830ecd3
translated_from: content/en/alg/I/09_s9_fields.md
translation_method: google
source_content_sha256: 622420ff5a6f546db44026f2ba8fbe2960bad17825f8f2a2110f89182676f0dd
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: c476a0d370c209a17e22ffa0dc5bae95af1106293b372ecf591a42f60a53cdc7
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 9。 域

### 1.域

#### 定义 1 {#alg-i-s9-def-1 .statement tag=05IF}

*如果环$K$不只由$0$组成，并且$K$的每个非零元素都是可逆的，则称为域。*

域 $K$ 的非零元素与乘法的集合是群，正好是环 $K$ (§ 8, no. 1) 的乘法群 $K^*$。 域中的逆环是域。如果乘法是可交换的，则域称为*可交换的*；这样的域与它的对立面相同。非交换域是有时 ，称为*偏斜域*。

#### 例 {#alg-i-s9-n1-exa-1 .statement tag=05IG}

*(1)* 我们将在*理性数*的no. 4域中定义；在 *General 拓扑* 域 of 实数将被定义 (*General 拓扑*, IV, § 1, no. 3), 域 of 复数 (*General 拓扑*, VIII, § 1, no. 1) 和域四元数（*常规拓扑*、VIII, § 1, no. 4）。除了四元数的域之外，这些域是可交换的。*
*(2)* 环 $\mathbf{Z}/2\mathbf{Z}$ 显然是域。

设$K$为域。 $K$的每个子环$L$即域称为$K$的*子域*，$K$称为$L$的*扩张域*；相当于说，$L$是$K$的子环，并且对于$L$的每个非零元素$x$来说，$x^{-1} \in L$是相同的。如果$(L_i)_{i \in I}$是$K$的子域的家族，那么$\bigcap_{i \in I} L_i$就是$K$的子域；对于$K$的每个子集$X$，因此存在$K$包含$X$的最小的子域；据说它是由*$X$*生成的。

#### 命题 1 {#alg-i-s9-prop-1 .statement tag=05IH}

*令$K$为域。对于$K$的每个子集$X$，$X$的扶正器（§ 8, no. 5，例3）$X'$是$K$的子域。*

我们知道（*loc.cit.*）$X'$ 是 $K$ 的子环。另一方面，如果 $x \neq 0$ 可与 $z \in X$ 置换，则 $x^{-1}$ (I, § 2, no. 3, 命题 5) 也可置换，因此 $X'$ 包含是 $X'$ 的每个非零元素的逆。

#### 推论{#alg-i-s9-n1-cor-1 .statement tag=05II}

*域 $K$ 的中心是 $K$ 的（可交换）子域。*

#### 定理 1 {#alg-i-s9-thm-1 .statement tag=05IJ}

设$\mathbf{A}$为环。以下条件是等效的：

(a) $\mathbf{A}$ 为域；
(b) $\mathbf{A}$ 不会减少到 0，并且 $\mathbf{A}$ 的唯一左理想是 0 和 $\mathbf{A}$。

假设$\mathbf{A}$是域。那么$\mathbf{A}$不会减少到0。令$a$为不同于0的$\mathbf{A}$的左理想。存在非零$a$属于到$a$。对于所有$x \in \mathbf{A}$、$x = (xa^{-1})a \in a$；因此$a = \mathbf{A}$。

假设$\mathbf{A}$满足条件(b)。设$x \neq 0$在$\mathbf{A}$中。我们需要证明$x$是可逆的。左理想$Ax$包含$x$，因此不是零、从而$Ax = \mathbf{A}$。因此存在$x' \in \mathbf{A}$使得$x'x = 1$。然后从 $1 \neq 0$ 开始$x' \neq 0$。将上述结果应用代入$x'$，可知存在$x'' \in \mathbf{A}$使得$x''x' = 1$。然后$x'' = x'' . 1 = x''x'x = 1 . x = x$，因此$xx' = 1$。因此$x'$是$x$的倒数。

#### 注 {#alg-i-s9-n1-rem-1 .statement tag=05IK}

在定理1中，左理想可以被右理想代替。在章VIII, § 5, no. 2中，我们将研究非零环$\mathbf{A}$，它们没有不同于0和$\mathbf{A}$的“双面”理想；这样的环（称为*拟单*）不一定是域*（对于例，带有有理系数的阶2的方阵的环$\mathbf{M}_2(\mathbf{Q})$是拟单但不是域）*。

#### 推论 1 {#alg-i-s9-thm-1-cor-1 .statement tag=05IL}

令$\mathbf{A}$为环，且$a$为$\mathbf{A}$的双面理想。为了使环$\mathbf{A}/a$成为域，$a$是$\mathbf{A}$的最大左理想是充分必要的。

$\mathbf{A}/a$ 的左理想为形式 $b/a$，其中 $b$ 是 $\mathbf{A}$ 包含 $a$ 的左理想（$§ 8$、no. 8，命题 5 的推论）。说$\mathbf{A}/a \neq 0$意味着$a \neq \mathbf{A}$。在这个假设下，$\mathbf{A}/a$是域当且仅当$\mathbf{A}$包含$a$的唯一左理想是$a$和$\mathbf{A}$（定理1），从而的推论。

#### 推论 2 {#alg-i-s9-thm-1-cor-2 .statement tag=05IM}

令$\mathbf{A}$为交换环，且不为0。在交换域上存在$\mathbf{A}$的同态。

根据克鲁尔的定理（$§ 8$，no. 6，定理1），$\mathbf{A}$中存在最大理想$a$。那么$\mathbf{A}/a$就是域（推论1）。

#### 推论 3 {#alg-i-s9-thm-1-cor-3 .statement tag=05IN}

设$a$为整数$\geqslant 0$。为了使环$\mathbf{Z}/a\mathbf{Z}$成为域，$a$是素数是充分必要的。

这是从推论 1 和$§ 8$、no. 11 得出的。

对于$p$素数域$\mathbf{Z}/p\mathbf{Z}$表示为$\mathbf{F}_p$。

#### 定理 2 {#alg-i-s9-thm-2 .statement tag=05IO}

令$\mathbf{K}$为域且$\mathbf{A}$为非零环。如果$f$是$\mathbf{K}$的同态进入$\mathbf{A}$，那么$\mathbf{A}$的子环$f(\mathbf{K})$是域并且$f$定义同构进入$\mathbf{K}$ $f(\mathbf{K})$。

设$a$为$f$的核。然后 $\mathbf{A}$ 中的 $f(1) = 1 \neq 0$ 为 $1 \notin a$，并且由于 $a$ 是 $\mathbf{K}$ 的左理想，$a = \{0\}$乘以定理 1。因此 $f$ 是单射的，因此 $\mathbf{K}$ 的同构到子环$f(\mathbf{K})$共$\mathbf{A}$；因此，后者环是域。

### 2.整环

#### 定义 2 {#alg-i-s9-def-2 .statement tag=05IP}

*如果环$\mathbf{A}$可交换、非零，并且$\mathbf{A}$的两个非零元素的乘积非零，则称为整环（或完整性域）。*

有理数整数的环$\mathbf{Z}$为整环；它是可交换的且非零的；两个整数 $> 0$ 中的乘积非零；每个非零整数都是形式$a$或$-a$，其中$a > 0$和$(-a)b = -ab,\ (-a)(-b) = ab$代表$a > 0,\ b > 0$，从而我们的断言。

每个交换域就是整环。 整环中的子环是整环。特别地，交换域中的子环是整环。相反，我们将证明每个整环$\mathbf{A}$同构于交换域的子环。回想一下 (§ 8, no. 12)，$\mathbf{A}$ 已被识别为其总环分数中的子环。然后我们的断言由以下命题得出：

#### 命题 2 {#alg-i-s9-prop-2 .statement tag=05IQ}

*如果$\mathbf{A}$为整环，则$\mathbf{A}$的分数$\mathbf{K}$的总环为交换环。*

环 $\mathbf{K}$ 是可交换的。从 $\mathbf{A} \neq \{0\}$ 开始它就不为零。由于$\mathbf{A}$是整环，$\mathbf{A}$的每个非零元素都是可取消的，$\mathbf{K}$由分数$a/b$和$b \neq 0$组成。现在$a/b \neq 0$意味着$a \neq 0$，而分数$b/a$则为$a/b$的倒数。

整环的分数之和环称为分数*的*域。这样的环与分数的域中的像进行识别。

#### 命题 3 {#alg-i-s9-prop-3 .statement tag=05IR}

*令$\mathbf{B}$为非零环，$\mathbf{A}$为$\mathbf{B}$的可交换子环，使得$\mathbf{A}$的每个非零元素在$\mathbf{B}$中可逆。
(a) $\mathbf{A}$ 是整环。
(b) *令$\mathbf{A}'$为分数$\mathbf{A}$中的域。 $\mathbf{A}$的典范嵌入到$\mathbf{B}$可以唯一地扩展到$\mathbf{A}'$的同构$f$到$\mathbf{B}$的子域。
(c) *$f(\mathbf{A}')$中的元素是$xy^{-1}$，其中$x \in \mathbf{A},\ y \in \mathbf{A},\ y \neq 0$。*

断言 (a) 是显而易见的。 The canonical injection of $\mathbf{A}$ into $\mathbf{B}$ extends uniquely to a homomorphism $f$ of $\mathbf{A}'$ into $\mathbf{B}$ (§ 8, no. 12, Theorem 5). 断言 (b) 然后从 no. 1, 定理 2 得出。 $\mathbf{A}'$中的元素是分数$x/y$以及$x \in \mathbf{A},\ y \in \mathbf{A},\ y \neq 0$和$f(x/y) = xy^{-1}$、从而 (c)。

### 3. 素理想

#### 命题 4 {#alg-i-s9-prop-4 .statement tag=05IS}

*令$\mathbf{A}$为交换环，且$\mathfrak{p}$为$\mathbf{A}$的理想值。以下条件是等效的：
(a) *环$\mathbf{A}/\mathfrak{p}$为整环；
(b) $\mathbf{A} \neq \mathfrak{p}$，如果$x \in \mathbf{A} - \mathfrak{p}$和$y \in \mathbf{A} - \mathfrak{p}$，则$xy \in \mathbf{A} - \mathfrak{p}$。
(c) $\mathfrak{p}$ 是$\mathbf{A}$ 同态核变成域。*

(c) ⇒ (b) ⇒ (a) 的含义是显而易见的。若$A/p$为整环，则设$f$为$A/p$的典范嵌入入其分数的域及$A$的$g$典范同态入$A/p$；那么$p$是$f \circ g$的核，从而蕴涵(a)⇒(c)。

#### 定义 3 {#alg-i-s9-def-3 .statement tag=05IT}

*在交换环$A$中，命题4的理想$p$满足条件称为素理想。*

#### 例 {#alg-i-s9-n3-exa-1 .statement tag=05IU}

(1) 设$A$为交换环。如果$m$是$A$的极大理想，则$m$是素数； 环 $A/m$ 是域（no. 1，推论 1 到定理 1）。

(2) 如果$A$是整环，则$A$的理想$\{0\}$是素数（但一般不是最大，如环$\mathbf{Z}$的例证明）。

### 4. 有理数数的域

#### 定义 4 {#alg-i-s9-def-4 .statement tag=05IV}

*有理整数的环$\mathbf{Z}$分数域称为有理数的域并记为$\mathbf{Q}$。 $\mathbf{Q}$的元素称为有理数。*

因而，每个有理数都是形式$a/b$，其中$a$和$b$是有理整数和$b \neq 0$（我们甚至可以将$b > 0$视为关系）

$$
a/b = (-a)/(-b)
$$

证明）。 $\mathbf{Q}_+$用于与$a \in \mathbf{N}$和$b \in \mathbf{N}^*$表示形式$a/b$的有理数的集合。

我们有关系：

(1) $$ \mathbf{Q}_+ + \mathbf{Q}_+ = \mathbf{Q}_+ $$
(2) $$ \mathbf{Q}_+ \cdot \mathbf{Q}_+ = \mathbf{Q}_+ $$
(3) $$ \mathbf{Q}_+ \cap (-\mathbf{Q}_+) = \{0\} $$
(4) $$ \mathbf{Q}_+ \cup (-\mathbf{Q}_+) = \mathbf{Q} $$
(5) $$ \mathbf{Q}_+ \cap \mathbf{Z} = \mathbf{N} $$

前两个源自公式、$a/b + a'/b' = (ab' + a'b)/bb'$、$(a/b)(a'/b') = aa'/bb'$、$0 \in \mathbf{Q}_+$、$1 \in \mathbf{Q}_+$，以及$\mathbf{N}$在加法和乘法以及$\mathbf{N}^*$在乘法下稳定的事实。显然$0 \in \mathbf{Q}_+$，从而$0 \in (-\mathbf{Q}_+)$；让$x$在$\mathbf{Q}_+ \cap (-\mathbf{Q}_+)$中；则存在正整数 $a, b, a', b'$ 以及 $b \neq 0,\ b' \neq 0$ 和 $x = a/b = -a'/b'$；然后$ab' + ba' = 0$、从而$ab' = 0$（对于$ab' \geq 0$和$ba' \geq 0$），因此从$b' \neq 0$开始为$a = 0$；其他字、$x = 0$。最后，显然是$\mathbf{N} \subset \mathbf{Z}$和$\mathbf{N} \subset \mathbf{Q}_+$。反之，如果$x$属于到$\mathbf{Z} \cap \mathbf{Q}_+$，则是有理数整数；存在两个有理数整数$a$和$b$，其中$a \geq 0,\ b > 0$和$x = a/b$，从而$a = bx$；如果$x \notin \mathbf{N}$，则$-x > 0$，从而$-a = b(-x) > 0$，因而$a < 0$与假设相反。

给定两个有理数数 $x$ 和 $y$，如果 $y - x \in \mathbf{Q}_+$，我们就写 $x \leq y$。由公式（1）、（3）、（4）很容易推导出$x \leq y$是对的全序

Q，从（5）得知，这个关系诱导是Z上通常的序关系。最后，从（1）得出关系$x \leq y$和$x' \leq y'$暗示$x + x' \leq y + y'$，从（2）得出关系$x \leq y$暗示$xz \leq yz$对于所有$z \geq 0$和$xz \geq yz$对于$z \leq 0$（cf.VI, § 2, no. 1）。

设 $x$ 为有理数数。如果 $x \geq 0$，$x$ 被称为“正”，如果 $x > 0$，则“严格正”，如果 $x \leq 0$，则“负”，如果 $x < 0$.† 集合，正有理数为 $\mathbf{Q}_+$，负有理数是$-\mathbf{Q}_+$。如果$\mathbf{Q}^*$表示非零有理数数的集合，严格正数数的集合$\mathbf{Q}_+^*$等于$\mathbf{Q}^* \cap \mathbf{Q}_+$，$-\mathbf{Q}_+^*$是严格负数数的集合。

集合$\mathbf{Q}_+^*$和$\{1, -1\}$是乘法群$\mathbf{Q}^*$中的子群。每个有理数$x \neq 0$都可以在形式$1.y, (-1).y$中以一种且唯一的方式表达，其中$y > 0$;因此乘法群$\mathbf{Q}^*$是子群$\mathbf{Q}_+^*$和$\{1, -1\}$的乘积，$\mathbf{Q}_+^*$中$x$的分量称为$x$的*绝对值*，并表示为$|x|$； $\{-1, 1\}$中$x$的分量（如果$x > 0$则等于1，如果$x < 0$则等于$-1$）称为$x$的*符号*，并用$\operatorname{sgn}\, x$表示。

通常这两个函数通过设定$|0| = 0$和$\operatorname{sgn}\, 0 = 0$扩展到整个$\mathbf{Q}$。

### 习题 {#alg-i-s9-exercises}

§ 9](exercises/s9/)参见[习题。
