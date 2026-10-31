---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 1
section_title: Laws of composition; associativity; commutativity
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 1-12, 124-126
pdf_pages: 0025-0036, 0148-0150
extraction: ocr
subsections:
    - "no": 1
      title: LAWS OF COMPOSITION
      page: 1
      pdf_page: 25
    - "no": 2
      title: COMPOSITION OF AN ORDERED SEQUENCE OF ELEMENTS
      page: 3
      pdf_page: 27
    - "no": 3
      title: ASSOCIATIVE LAWS
      page: 4
      pdf_page: 28
    - "no": 4
      title: STABLE SUBSETS. INDUCED LAWS
      page: 6
      pdf_page: 30
    - "no": 5
      title: PERMUTABLE ELEMENTS. COMMUTATIVE LAWS
      page: 7
      pdf_page: 31
    - "no": 6
      title: QUOTIENT LAWS
      page: 11
      pdf_page: 35
statements: 31
exercises: 16
content_sha256: 7cee8826f7f11b901418d6322c728ec455045d9a4db1b8f6583306fa1e1125a9
translated_from: content/en/alg/I/01_s1_laws_of_composition_associativity.md
translation_method: google
source_content_sha256: 5e673d0115ec27e87cd42d00b10d88a67c6691b3b1a9b1ee5776c4a964875bff
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 9ec1b58f8bd0d617f77c0a5fca42a1a8e67b6d99fea299a92d654c751ffbd2ae
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。 律合成； 结合性； 交换律

### 1. 律的合成

#### 定义 1 {#alg-i-s1-def-1 .statement tag=055B}

令 E 为集合。 E × E 的映射 f 变成 E 称为 E 上的合成律。 有序对 (x, y) ∈ E × E 的 f 的值 f(x, y) 在此律下称为 x 和 y 的合成。 集合与律合成称为岩浆。

x 和 y 的合成通常通过将 x 和 y 写在定义的阶中并用所讨论的律特征符号（可以同意省略的符号）将它们分开来表示。最常用的符号是 + 和 .，如果需要，通常对流是省略后者； x和y的这些符号合成分别写为x + y和x.y或xy。用符号+表示的律通常称为加法（合成x + y称为x和y的和），我们说它是相加写的； 律用符号 表示。通常被称为乘法 （合成 x.y = xy 被称为 x 和 y 的乘积），我们说它是乘法写的。在这个章第1至第3段的一般论点中，我们通常使用符号⊔和⊓来表示合成中的任意律。

通过滥用语言，E × E 的子集映射到 E 中是有时称为合成的律，并非在 E 上到处都有定义。

#### 例 {#alg-i-s1-n1-exa-1 .statement tag=055C}

(1) 映射 (X, Y) ↦ X ∪ Y 和 (X, Y) ↦ X ∩ Y 是集合上的合成律子集 / 集合 E。

(2) 在自然数、加法、乘法、幂运算的集合 N 上，合成的律 (律下 x ∈ N 和 y ∈ N 的合成为分别用 x + y、xy 或 x.y 和 x^y) 表示（集合理论，III, § 3, no. 4）。

(3) 设E为集合； 映射 (X, Y) ↦ X ⋅ Y 为 E × E 子集集合上合成律 (集合理论，II, § 3, no. 3， 定义6); 映射 (f, g) ↦ f ⋅ g 为 E 的映射集合上的合成律变为 E (集合理论，II, § 5, no. 2)。

(4) 设E为格子（集合理论，III, § 1, no. 11）；如果sup(x, y)表示集合 {x, y}中的最小上界，则映射 (x, y) ↦sup(x, y)是E上合成的律。对于下确界 inf(x, y)也是如此。上面的例 1 是这种情况的一个特例，$\mathfrak{P}(E)$ 按包含排序。

(5) 令$(E_t)_{t \in I}$为岩浆族。让$\tau_t$表示$E_t$上合成的律。 映射
$$
((x_i), (y_i)) \mapsto ((x_i \tau_t y_i))
$$
乘积$E = \prod_{t \in I} E_t$上合成的律，称为律$\tau_t$的*乘积*。 集合 E 与律称为岩浆$E_t$ 的*乘积岩浆*。特别地，如果所有的岩浆$E_t$都等于同一个岩浆M，我们从M*得到I的*岩浆映射。

设$(x, y) \mapsto x \tau y$为集合E上合成的律。给定E的任意两个子集X，Y，$X \tau Y$（前提是记号不会导致混淆†）将表示集合 E 中的元素 $x \tau y$，其中 $x \in X, y \in Y$（在其他字中，$X \times Y$ 中的像在映射 $(x, y) \mapsto x \tau y$ 下）。

如果$a \in E$，我们通常写$a \tau Y$代替$\{a\} \tau Y$，写$X \tau a$代替$X \tau \{a\}$。 映射$(X, Y) \mapsto X \tau Y$是E的子集集合上合成律。

#### 定义 2 {#alg-i-s1-def-2 .statement tag=055D}

*设 E 为岩浆，$\tau$ 表示其合成的律。 E 上的合成 $(x, y) \mapsto y \tau x$ 的律称为上面的相反。 集合 E 与律称为 E 的对向岩浆。*

令E和E'为两股岩浆；我们将用相同的符号 $\tau$ 来表示它们的律。符合一般定义 (*集合理论*, IV, § 1, no. 5)，E 的双射映射 f 到 E' 上，使得
$$
f(x \tau y) = f(x) \tau f(y)
$$
对于每个有序对 $(x, y) \in E \times E$ 被称为 E 到 E'* 的 *同构的。如果 E 到 E' 上存在同构，则称 E 和 E' 是“同构的”。

更一般地说：

#### 定义 3 {#alg-i-s1-def-3 .statement tag=055E}

*将 E 的映射 f 转化为 E'，使得关系 (1) 对于每个有序对 $(x, y) \in E \times E$ 成立，称为同态或态射，将 E 转化为 E'；如果 $E = E'$，则 f 称为 E 的自同态。*

岩浆E的恒等映射是同态，两个同态的合成是同态。

† 以下是例，其中原理会导致混乱，因此不应使用。假设所讨论的合成的律是在集合E的子集之间的律$(A, B) \mapsto A \cup B$； 律 / 合成
$$
(\mathscr{A}, \mathscr{B}) \mapsto F(\mathscr{A}, \mathscr{B})
$$
在子集与 $\mathfrak{P}(E)$ 之间导出，$F(\mathscr{A}, \mathscr{B})$ 是 $A \cup B$ 的集合与 $A \in \mathscr{A}, B \in \mathscr{B}$；但$F(\mathscr{A}, \mathscr{B})$不应该用$\mathscr{A} \cup \mathscr{B}$表示，因为这个记号已经有不同的含义（$\mathscr{A}$的并和$\mathscr{B}$被视为$\mathfrak{P}(E)$的子集）。

为了使 E 到 E' 的映射 $f$ 成为同构，它是双射同态是充分必要的，并且 $f^{-1}$ 是 E' 到 E 的同构。

### 2. 合成有序序列元素

回想一下，集合 E 的元素族是集合 I 的映射 $i \mapsto x_i$（称为索引集合）到 E 中；如果索引集合是有限的，则族 $(x_i)_{i \in I}$ 称为有限族。

E 的元素的有限族 $(x_i)_{i \in I}$ 其下标集合 I 是全序的，称为 E 的有序序列 of 元素。

特别是，每个有限序列$(x_i)_{i \in H}$，其中H是集合$\mathbf{N}$或自然数的有限子集，如果H由关系诱导给出序关系，则可以将其视为有序序列 $m \leq n$ 自然数之间。

如果存在 I 的有序集合同构 $\phi$ 到 K 上，使得 $y_{\phi(i)} = x_i$ 对于所有 $i \in I$，则两个有序序列 $(x_i)_{i \in I}$ 和 $(y_k)_{k \in K}$ 被称为相似。

每个有序的序列$(x_\alpha)_{\alpha \in A}$都类似于合适的有限序列。因为在 $\mathbf{N}$ 的区间 $[0, n]$ 上存在 A 的递增双射。

#### 定义 4 {#alg-i-s1-def-4 .statement tag=055F}

*令*$(x_\alpha)_{\alpha \in A}$*为岩浆E中元素的有序序列，其索引集合A非空。有序序列* $(x_\alpha)_{\alpha \in A}$的合成（在律 T下），*表示为*$\prod_{\alpha \in A} x_\alpha$，*是A中元素的数上的归纳定义的E的元素，如下：*

(1) *如果* $A = \{\beta\}$ *则* $\prod_{\alpha \in A} x_\alpha = x_\beta$;

(2) *如果* A *有* $p > 1$ *元素，$\beta$是* A *和* $A' = A - \{\beta\}$的最小元素，*则* $\prod_{\alpha \in A} x_\alpha = x_\beta \ T \left( \prod_{\alpha \in A'} x_\alpha \right)$。

紧接着（通过索引集合中元素的数上的归纳）两个相似有序序列的合成相等；特别是，任何有序的序列的合成等于有限序列的合成。如果 $A = \{\lambda, \mu, \nu\}$ 有三个元素 ($\lambda < \mu < \nu$) 合成 $\prod_{\alpha \in A} x_\alpha$ 则为 $x_\lambda \ T \ (x_\mu \ T \ x_\nu)$。

#### 注 {#alg-i-s1-n2-rem-1 .statement tag=055G}

注有序序列的定义、合成存在一定的任意性； 归纳我们“从右到左”介绍了收益。如果我们“从左到右”进行，则上面排序的序列 $(x_\lambda, x_\mu, x_\nu)$ 中的合成将是 $(x_\lambda \ T \ x_\mu) \ T \ x_\nu$。

作为记号，有序序列$(x_\alpha)_{\alpha \in A}$的合成写成$\prod_{\alpha \in A}$，律表示为$\perp$；对于相加的律，通常用$\sum_{\alpha \in A} x_\alpha$表示，称为有序的序列$(x_\alpha)_{\alpha \in A}$的和（$x_\alpha$称为和的项）；对于乘法书写的律，通常用$\prod_{\alpha \in A} x_\alpha$表示，并称为有序序列$(x_\alpha)$的*乘积*（$x_\alpha$称为乘积的*因子*）。†

当索引集合（也不是其顺序）可能出现混淆时，通常会在记号中省略有序序列的合成，然后我们写，对于例，律附加地写，
$\sum_\alpha x_\alpha$代替$\sum_{\alpha \in A} x_\alpha$；对于其他记号也是如此。

对于由序列* $(x_i)$ 的 $\top$ 合成表示且索引为集合的律，$\mathbf{N}$ 的非空区间 $[p, q]$ 由 $\prod_{p \leq i \leq q} x_i$ 或 $\prod_{i=p}^q x_i$ 表示；类似地对于用其他符号表示的律。

设E和F为两颗岩浆，其合成的律分别用E的$\top$和$f$同态表示为F。对于E的元素的每个有序序列$(x_\alpha)_{\alpha \in A}$
$$
f\left( \prod_{\alpha \in A} \right) = \prod_{\alpha \in A} f(x_\alpha).
$$

### 3.联想律

#### 定义 5 {#alg-i-s1-def-5 .statement tag=055H}

*合成* $(x, y) \mapsto x \top y$ *在集合* E 上的 *律被称为结合性，如果对于所有元素* $x, y, z$ *在* E 中，
$$
(x \top y) \top z = x \top (y \top z).
$$
*律具有缔合性的岩浆称为缔合性岩浆*。

结合律律的相反律是结合律。

#### 例 {#alg-i-s1-n3-exa-1 .statement tag=055I}

(1) 自然数的加法和乘法在 $\mathbf{N}$ 上与合成的律结合（*集合理论*、III, § 3, no. 3、命题 5 的推论）
(2) no. 1 例 (1)、(3) 和 (4) 中引用的律是结合律。

#### 定理 1 (结合性定理) {#alg-i-s1-thm-1 .statement tag=055J}

*设* E *为缔合岩浆，其律表示为* $\top$。 *设* A *是一个全序非空有限集合，它是非空子集* $(B_i)_{i \in I}$的有序序列的并，使得关系* $\alpha \in B_i, \beta \in B_j, i < j$ *隐含* $\alpha < \beta$； *让*$(x_\alpha)_{\alpha \in A}$*成为*E*中元素的有序序列，其中*A*作为索引集合*。 *然后*
$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right)
$$

† 如果存在与集合论（*集合理论*、II, § 5, no. 3）中定义的乘积或集合$x_\alpha$混淆的风险，则必须避免使用此术语和记号$\prod_{\alpha \in A} x_\alpha$。然而，如果$x_\alpha$是基数，加法（或乘法）是基数和（或乘积），则上面记号中$\sum_{\alpha \in A} x_\alpha$（或$\prod_{\alpha \in A} x_\alpha$）表示的基数是基数$(x_\alpha)_{\alpha \in A}$家族的和（分别为红衣主教乘积）（*集合理论*，III, § 3, no. 3）。

§ 1.3

我们通过归纳在$A$的基数$n$上证明定理。设$p$为$I$的基数，$h$是其最小的元素；让$J = I - \{h\}$。如果$n = 1$，由于$B_i$非空，必然$p = 1$和定理是明显的。否则，假设定理对于最多 $n - 1$ 元素的索引集合成立，我们区分两种情况：

(a) $B_h$ 有一个元素 $\beta$。让$C = \bigcup_{i \in J} B_i$。 (3) 的左侧等于定义，等于$x_\beta \top \left( \prod_{\alpha \in C} x_\alpha \right)$；右边等于定义，
$$
x_\beta \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right);
$$
结果源自假设 $C$ 和 $(B_i)_{i \in J}$ 定理为真。

(b) 否则，令 $\beta$ 为 $A$ 中最小的元素（因此也是 $B_h$）；让 $A' = A - \{\beta\}$ 并让 $B'_i = A' \cap B_i$ 得到 $i \in I$；然后$B'_i = B_i$换$i \in J$。 集合 $A'$ $n - 1$ 元素和条件定理持有$A'$ 及其子集 $B'_i$；因此通过假设：
$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{\alpha \in B'_h} x_\alpha \right) \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right).
$$
用每条边形成$x_\beta$的合成，我们在左侧使用定义、$\prod_{\alpha \in A} x_\alpha$，在右侧使用结合性，
$$
\left( x_\beta \top \left( \prod_{\alpha \in B'_h} x_\alpha \right) \right) \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right)
$$
它等于定义 3，等于公式 (3) 的右侧。

对于序列 $(x_i)_{i \in [p, q]}$ 的 $\top$ 合成 $\prod_{p \leq i \leq q} x_i$ 表示的结合词律也表示（因为不会产生混淆）
$$
x_p \top \cdots \top x_q.
$$
定理 1 的一个特例是公式
$$
x_0 \top x_1 \top \cdots \top x_n = (x_0 \top x_1 \top \cdots \top x_{n-1}) \top x_n.
$$
考虑$n$项的有序序列，其所有项都等于相同的元素$x \in E$。该序列中的合成用$\prod^n x$表示，对于律用$\top$表示，$\prod^n x$对律用$\perp$表示。对于律乘法书写，合成表示为$x^n$，称为$x$的第$n$*幂*。对于律加法写成合成通常用 $nx$ 表示。将结合性定理应用于有序序列，其所有项都相等，给出等式

$$
\frac{n_1 + n_2 + \cdots + n_p}{T} x = \left( \frac{n_1}{T} x \right) T \left( \frac{n_2}{T} x \right) T \cdots T \left( \frac{n_p}{T} x \right).
$$

特别是，如果$p = 2$，

$$
\frac{m+n}{T} x = \left( \frac{m}{T} x \right) T \left( \frac{n}{T} x \right)
$$
如果$n_1 = n_2 = \cdots = n_p = m$，
$$
\frac{pm}{T} x = \frac{p}{T} \left( \frac{m}{T} x \right).
$$

如果$X$是$E$的子集，我们用有时表示，与上面的记号一致，用$\frac{p}{T} X$集合$X_1 T X_2 T \cdots T X_p$，其中
$$
X_1 = X_2 = \cdots = X_p = X;
$$
因此，它是所有合成 $x_1 T x_2 T \cdots T x_p$ 和 $x_1 \in X, x_2 \in X, \ldots, x_p \in X$ 中的集合。

重要的是不要将此集合与 $\frac{p}{T} x$ 的集合混淆，其中 $x$ 穿过 $X$。

### 4.稳定子集。诱导律

#### 定义 6 {#alg-i-s1-def-6 .statement tag=055K}

* 集合$E$子集$A$若$A$属于两个元素合成在$E$上合成$T$律下称为稳定$A$。 $A \times A$到$A$的映射$(x, y) \mapsto x T y$则称为律在$A$上由律$T$诱导。由$T$诱发的集合$A$和律称为$E$的次岩浆。*

在其他字中，要使$A$稳定在律$T$下，$A T A \subset A$是充分必要的。经常会发现稳定的子集 $E$ 和相应的次岩浆。

$E$稳定子集家庭交稳定；特别是对于给定的子集$X$，存在$E$包含的最小的稳定子集$A$；据说它是由$X$*生成*的，$X$被称为$A$的*生成的系统*或$A$的*生成的集合*。 相应的子岩浆也据说是由 $X$ *生成*的。

#### 命题 1 {#alg-i-s1-prop-1 .statement tag=055L}

*令$E$和$F$为两块岩浆，将$E$的$f$同态放入$F$。
(i) $E$ 的稳定子集的$f$ 下的像是$F$ 的稳定子集。
(ii) 稳定的子集$F$的$f$下的逆像是$E$的稳定的子集。
(iii) 设$X$为$E$中的子集。 $X$生成的$E$的稳定子集在$f$下的像是$f(X)$生成的$F$的稳定子集。
(iv) 如果$g$是$E$的第二个同态，来自$E$的元素$x$的$F$集合，使得$f(x) = g(x)$是子集的稳定子集 $E$.*

断言 (i)、(ii) 和 (iv) 是显而易见的；我们证明(iii)。令$\overline{X}$为X生成的E的稳定子集，$\overline{f(X)}$为$f(X)$生成的F的稳定子集。由 (i) $\overline{f(X)} \subset f(\overline{X})$ 和 (ii) $\overline{X} \subset f^{-1}(\overline{f(X)})$、从而 $f(\overline{X}) \subset \overline{f(X)}$。

#### 命题 2 {#alg-i-s1-prop-2 .statement tag=055M}

*设 E 为关联岩浆，E 的 X 子集。设 X' 为 $x_1 \top x_2 \top \cdots \top x_n$ 的集合，其中 $n \geq 1$ 和 $x_i \in X$ 为 $1 \leq i \leq n$。 X生成的稳定子集等于X'._

紧接着n上的归纳，n项属于到X属于的有序序列的合成到X生成的稳定子集；因此足以验证 X' 是稳定的。 现在，如果 u 和 v 为 X' 的元素，则它们为形式 $u = x_0 \top x_1 \top \cdots \top x_{n-1}$、$v = x_n \top x_{n+1} \top \cdots \top x_{n+p}$，$x_i \in X$ 为 $0 \leq i \leq n + p$；然后 (定理 1) $u \top v = x_0 \top x_1 \top \cdots \top x_{n+p}$ 属于到 X'。

#### 例 {#alg-i-s1-n4-exa-1 .statement tag=055N}

(1) 在自然数的集合$\mathbf{N}$中，{1}生成的加法下稳定的子集为整数$\geq 1$的集合； 乘法集合{1}以下是稳定的。

(2) 给定集合 E 上的律$\top$，对于单个元素的子集{h}由……组成要在律$\top$下稳定，$h \top h = h$是充分必要的； h 被称为“幂等”。对于例，格子的每个元素对于律sup和inf都是幂等的。

(3) 对于集合 E 上的结合律$\top$，单个元素的集合{a}由……组成生成的稳定子集是元素$\overline{\top}^n a$的集合，其中n经过集合整数 $> 0$。

### 5.可变换元素。可交换律

#### 定义 7 {#alg-i-s1-def-7 .statement tag=055O}

*设 E 为岩浆，其律表示为 $\top$。如果 $y \top x = x \top y$*，则 E 的两个元素 x 和 y 被称为可交换（或可置换）。

#### 定义 8 {#alg-i-s1-def-8 .statement tag=055P}

* 集合 E 上合成的律称为可交换的，如果 E 中的任意两个元素在该律下可交换。 律或合成可交换的岩浆称为可交换岩浆。*

交换律律等于它的相反数。

#### 例 {#alg-i-s1-n5-exa-1 .statement tag=055Q}

(1) 自然数的加法和乘法在$\mathbf{N}$上可交换律（*集合理论*，III, § 3, no. 3，命题5的推论）。

(2) 在格上律sup 和inf 是可交换的；因此，特别是律 $\cup$ 和 $\cap$ 位于子集和集合 E 之间。

(3) 令E为基数$> 1$的集合。 E 到 E 的映射之间的律 $(f, g) \mapsto f \circ g$ 不可交换，如将 f 和 g 视为不同常数映射所示，但恒等映射对于每个映射都是可置换的。

(4) 设$(x, y) \mapsto x \top y$是$E$上的交换律律； 律
$$
(X, Y) \mapsto X \top Y
$$
$E$ 的子集之间是可交换的。

#### 定义 9 {#alg-i-s1-def-9 .statement tag=055R}

*令$E$为岩浆，$X$子集为$E$。 $E$的元素的集合与$X$的每个元素可交换，称为$X$的集中器。*

令$X$和$Y$是$E$和$X'$和$Y'$各自的中心化器中的两个子集。如果$X \subset Y$，则$Y' \subset X'$。

令$(X_i)_{i \in I}$为$E$的子集族，对于所有$i \in I$，令$X'_i$为$X_i$的集中器。 $\bigcup_{i \in I} X_i$的扶正器是$\bigcap_{i \in I} X'_i$。

设$X$为$E$的子集，$X'$为$X$的中心化器。 $X'$的扶正器$X''$称为$X$的*双中心化器*。然后$X \subset X''$。 $X''$的扶正器$X'''$等于$X'$。因为$X'$包含在其双中心化器$X'''$中，并且关系$X \subset X''$意味着$X'''' \subset X'$。

#### 命题 3 {#alg-i-s1-prop-3 .statement tag=055S}

*令$E$为缔合岩浆，其律用$\top$表示。如果$E$的元素$x$与元素$y$和$E$的$z$分别通勤，则与$y \top z$通勤。*

对于
$$
x \top (y \top z) = (x \top y) \top z = (y \top x) \top z \\
= y \top (x \top z) = y \top (z \top x) = (y \top z) \top x.
$$

#### 推论{#alg-i-s1-n5-cor-1 .statement tag=055T}

*令 $E$ 为联想岩浆。 $E$ 的任何子集的扶正器都是 $E$ 的稳定子集。*

#### 定义 10 {#alg-i-s1-def-10 .statement tag=055U}

*岩浆$E$的集中器称为$E$的中心。 $E$的中心元素称为$E$的中央元素。*

如果 $E$ 是缔合岩浆，则根据命题 3 的推论，其中心是稳定的子集，并且在其中心上诱导的律是可交换的。

#### 命题 4 {#alg-i-s1-prop-4 .statement tag=055V}

*令$E$为关联岩浆，$X$和$Y$为$E$的两个子集。如果$X$的每个元素与$Y$的每个元素进行交换，$X$生成的稳定子集的每个元素与$Y$生成的稳定子集的每个元素进行交换。*

设$X'$和$X''$为$X$的中心化器和双中心化器。它们稳定子集或 $E$。现在$X \subset X''$和$Y \subset X'$，因此$X''$（分别为$X'$）包含是由$X$（分别为$Y$）生成的$E$的稳定子集。由于$X''$的每元素与$X'$的每元素通勤，因此命题紧随其后。

#### 推论 1 {#alg-i-s1-prop-4-cor-1 .statement tag=055W}

*如果 $x$ 和 $y$ 在结合律律 $\top$ 下是可置换的，那么对于所有整数 $m > 0$ 和 $n > 0$，$\top^m x$ 和 $\top^n y$ 也是可置换的；特别是$\top^m x$和$\top^n x$对于所有$x$和所有整数$m > 0$和$n > 0$都是可置换的。*

#### 推论 2 {#alg-i-s1-prop-4-cor-2 .statement tag=055X}

*如果子集 X 的元素的所有对在结合律律 T 下都是可置换的，则 T 在由 X 生成的稳定子集上诱导的律是结合律和交换律的。*

#### 定理 2 (交换律定理) {#alg-i-s1-thm-2 .statement tag=055Y}

*设 T 是 E 上合成的结合律律；令 $(x_\alpha)_{\alpha \in A}$ 为 E 的元素非空有限族，且可成对置换；设 B 和 C 是两个全序集，其中 A 作为底层集合。然后*
$$
\prod_{\alpha \in B} x_\alpha = \prod_{\alpha \in C} x_\alpha.
$$

由于如果 A 有一个元素，则定理为真，因此我们通过归纳对 A 中元素的数 $p$ 进行论证。令 $p$ 为整数 > 1，并假设当卡片 A < $p$ 时，定理为真。我们证明卡 A = $p$。可以假设A是$\mathbf{N}$中的区间$[0, p - 1]$； A 上的自然序关系定​​义的有序序列 $(x_\alpha)_{\alpha \in A}$ 的合成是$\prod_{i=0}^{p-1} x_i$。

令 A 具有另一个全排序，并令 h 为该排序下 A 的最小元素以及 A 的其他元素的 A' 集合（通过诱导排序全排序）。假设首先 $0 < h < p - 1$ 并令 P = $\{0, 1, \ldots, h - 1\}$ 且 Q = $\{h + 1, \ldots, p - 1\}$；假设定理对于A'为真，应用结合性定理，我们得到（自$A' = P \cup Q$）

$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{i=0}^{h-1} x_i \right) \circ \left( \prod_{i=h+1}^{p-1} x_i \right)
$$

从而，与T的两边重复组成$x_h$，并重复应用交换律和结合性：

$$
\begin{align*}
\prod_{\alpha \in A} x_\alpha &= x_h \circ \left( \prod_{\alpha \in A'} x_\alpha \right) = x_h \circ \left( \prod_{i=0}^{h-1} x_i \right) \circ \left( \prod_{i=h+1}^{p-1} x_i \right) \\
&= \left( \prod_{i=0}^{h-1} x_i \right) \circ x_h \circ \left( \prod_{i=h+1}^{p-1} x_i \right) = \prod_{i=0}^{p-1} x_i,
\end{align*}
$$

这证明了这种情况下的定理。如果$h = 0$或$h = p - 1$，则结果相同，但更简单，项由P产生，或项由Q未出现在公式中产生。

Under a commutative associative law on a set E the *composition* of a *finite family* $(x_\alpha)_{\alpha \in A}$ of elements of E is by definition the common value of the composition of all the *ordered sequences* obtained by totally ordering A in all possible ways. 这个合成在T表示的律下仍然会用$\prod_{\alpha \in A} x_\alpha$表示；对于其他记号也是如此。

#### 定理 3 {#alg-i-s1-thm-3 .statement tag=055Z}

*设 T 是 E 上的结合律律和 $(x_\alpha)_{\alpha \in A}$ E 的元素非空有限族，它们是成对可置换的。 If A is a union of non-empty subsets $(B_i)_{i \in I}$ which are pairwise disjoint, then*

$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right).
$$

如果 $A$ 和 $I$ 完全有序，则定理 2 可以得出定理 1 的 $B_i$ 满足条件。

我们挑出这个定理的两个重要的特殊情况：

1. 如果$(x_{\alpha \beta})_{(\alpha, \beta) \in A \times B}$是关联岩浆的可置换元素的有限族，其索引集合是两个非空有限集合$A, B$的乘积（“双族”），则

$$
\prod_{(\alpha, \beta) \in A \times B} x_{\alpha \beta} = \prod_{\alpha \in A} \left( \prod_{\beta \in B} x_{\alpha \beta} \right) = \prod_{\beta \in B} \left( \prod_{\alpha \in A} x_{\alpha \beta} \right)
$$

通过一方面将$A \times B$视为集合$\{\alpha\} \times B$的并，另一方面将集合$A \times \{\beta\}$的并，从定理3如下：

对于例，如果$B$有$n$元素，并且对于每个$\alpha \in A$，所有$x_{\alpha \beta}$有相同的值$x_\alpha$，那么

$$
\prod_{\alpha \in A} \left( \prod^n_{\beta=1} x_\alpha \right) = \prod^n_{\alpha=1} \left( \prod_{\alpha \in A} x_\alpha \right).
$$

如果$B$有两个元素，我们得到以下结果：令$(x_\alpha)_{\alpha \in A}, (y_\alpha)_{\alpha \in A}$是$E$的元素的两个非空族。如果 $x_\alpha$ 和 $y_\beta$ 是成对可置换的，那么

$$
\prod_{\alpha \in A} x_\alpha \prod_{\alpha \in A} y_\alpha = \left( \prod_{\alpha \in A} x_\alpha \right) \prod_{\alpha \in A} y_\alpha.
$$

因为双序列 $(x_{ij})$ 的公式 (7) 合成其下标集合是 $\mathbf{N}$ 中两个区间 $\{p, q\}$ 和 $\{r, s\}$ 的乘积，通常表示为交换结合词律附加编写

$$
\sum_{i=p}^q \sum_{j=r}^s x_{ij} \quad \text{or} \quad \sum_{j=r}^s \sum_{i=p}^q x_{ij}
$$

类似地，律用其他符号表示。

2. 令$n$为整数$> 0$，并令$A$为整数$(i, j)$的有序对的集合，使得$0 \leq i \leq n, 0 \leq j \leq n$和$i < j$； $(x_{ij})_{(i, j) \in A}$族的合成（在交换结合词律下）也可以用$\prod_{0 \leq i < j \leq n} x_{ij}$表示（或者简单地用$\prod_{i < j} x_{ij}$表示，如果不引起混淆的话）； 定理 3 这里给出公式

$$
\prod_{0 \leq i < j \leq n} x_{ij} = \prod_{i=0}^{n-1} \left( \prod_{j=i+1}^n x_{ij} \right) = \prod_{j=1}^n \left( \prod_{i=0}^{j-1} x_{ij} \right).
$$

对于索引集合是大于两个集合的乘积的族，有与(7)类似的公式，对于索引集合是*严格递增的的集合$S_p$的族，有与(10)类似的公式。 $p$ 整数的序列* $(i_k)_{1 \leq k \leq p}$，使得 $0 \leq i_k \leq n$ ($p \leq n + 1$)：在后一种情况下，$(x_{i_1 i_2 \ldots i_p})_{(i_1, \ldots, i_p) \in S_p}$ 族的合成表示为

$$
\prod_{0 \leq i_1 < i_2 < \cdots < i_p < n} x_{i_1 i_2 \ldots i_p} \quad \text{or simply} \quad \prod_{i_1 < i_2 < \cdots < i_p} x_{i_1 i_2 \ldots i_p}.
$$

#### 命题 5 {#alg-i-s1-prop-5 .statement tag=0560}

设E和F为岩浆，其律用T表示，并令f和g为E到F的同态。设f T g为E到F的映射 x ↦ f(x) T g(x)。如果F是结合律和交换律，则f T g是同态。

对于 E 的所有元素 x 和 y：

$$(f T g)(x T y) = f(x T y) T g(x T y) = f(x) T f(y) T g(x) T g(y)$$
$$= f(x) T g(x) T f(y) T g(y) = ((f T g)(x)) T ((f T g)(y)).$$

### 6.商律

#### 定义 11 {#alg-i-s1-def-11 .statement tag=0561}

令 E 为集合。 合成 T 的律和 E 上的等价关系 R 被认为是兼容的，如果关系 x ≡ x' (mod R) 和 y ≡ y' (mod R) （对于 x, x', y, y' ∈ E）意味着 x T y ≡ x' T y' (mod R)； 商集 E/R 上合成的律，其中x和y的映射等价类除以x T y的等价类，称为律T相对于R的商律。 集合 E/R 与律的商称为 E 相对于 R 的商岩浆。

说E上的等价关系R与合成f的内部律兼容：E × E→E on E意味着映射f与乘积等价关系R×相容的（在集合理论意义上，II, § 6, no. 5） R 在 E × E 上，等价关系 R 在 E 上。（集合理论，II, § 6, no. 8）。这也意味着R的图是E×E的子岩浆。

如果律 T 是结合律（或交换律），则商律也是结合律（更简单地说，当经过为商时，结合性或交换律被保留）。

从岩浆E到岩浆E/R的典范映射是同态。

对于进入岩浆 F 的映射 g E/R 为同态，g 的合成与 E/R 上的 E/R 的典范映射为同态是必要且充分的。

以下两个命题是来自定义的直接的：

#### 命题 6 {#alg-i-s1-prop-6 .statement tag=0562}

设 E 和 F 为两颗岩浆，E 的 f 同态进入 F。令 R[x, y] 表示 E 的元素 x, y 之间的关系 f(x) = f(y)。则 R 在 E 上为等价关系，与 E 上的律和 E/R 的映射兼容到 f(E) 上，通过经过与岩浆 E/R 到 F 子岩浆 f(E) 的商的同构求商。

#### 命题 7 {#alg-i-s1-prop-7 .statement tag=0563}

设 E 为岩浆，E 上的 R 等价关系与 E 上的律兼容。为了使 E/R 上的等价关系 S 与商律兼容，S 为形式 T/R 是充分必要的，其中 T 为 R 所暗示的 E 上的等价关系并与E 上的律。E/T 到 (E/R)/(T/R) 上的典范映射（集合理论，II, § 6, no. 7）则为岩浆同构。

#### 命题 8 {#alg-i-s1-prop-8 .statement tag=0564}

设E是岩浆，A是E的稳定子集，E上的R等价关系与E上的律兼容。A相对于R的饱和度B（集合

理论上，II, , no. 5) 是稳定的子集。 $R$在$A$和$B$分别诱导的等价关系$R_A$和$R_B$与从$A$的典范嵌入导出的律和映射兼容$B$乘以经过商是$A / R_A$的岩浆同构到$B / R_B$

让$\top$表示$E$上的律。如果$x$和$y$是$B$的两个元素，则存在$A$的两个元素、$x'$和$y'$，使得$x \equiv x' \pmod{R}$和$y \equiv y' \pmod{R}$；然后$x \top y \equiv x' \top y' \pmod{R}$和$x' \top y' \in A$，从而$x \top y \in B$。因此$B$是$E$的稳定子集，其他断言是明显的。

令$M$为岩浆，$((u_\alpha, v_\alpha))_{\alpha \in I}$为$M \times M$的元素族。考虑$M$上的所有等价关系$S$与$M$上的律兼容，并且$u_\alpha \equiv v_\alpha \pmod{S}$适用于所有$\alpha \in I$。这些关系的图的交是等价关系$R$的图，它与$M$上的律兼容，并且$u_\alpha \equiv v_\alpha \pmod{R}$。因此，$R$是具有这两个属性的最好的（集合理论，III, § 1，第3和7）等价关系。它被称为等价关系，与$(u_\alpha, v_\alpha)$生成的$M$上的律兼容。

#### 命题 9 {#alg-i-s1-prop-9 .statement tag=0565}

保留上面的记号，让$f$成为岩浆中$M$的同态，使得$f(u_\alpha) = f(v_\alpha)$代表所有$\alpha \in I$。那么$f$与$R$相容的。

让$T$是与$f$相关联的等价关系。那么所有$\alpha \in I$和$T$的$u_\alpha \equiv v_\alpha \pmod{T}$与$M$上的律兼容，因此$T$比$R$更粗糙；这就证明了命题。

### 习题 {#alg-i-s1-exercises}

§ 1](exercises/s1/)参见[习题。
