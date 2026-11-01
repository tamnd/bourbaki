---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 4
section_title: Natural integers. Finite sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 166-171, 230-234
pdf_pages: 0172-0177, 0236-0240
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF INTEGERS
      page: 166
      pdf_page: 172
    - "no": 2
      title: INEQUALITIES BETWEEN INTEGERS
      page: 166
      pdf_page: 172
    - "no": 3
      title: THE PRINCIPLE OF INDUCTION
      page: 168
      pdf_page: 174
    - "no": 4
      title: FINITE SUBSETS OF ORDERED SETS
      page: 170
      pdf_page: 176
    - "no": 5
      title: PROPERTIES OF FINITE CHARACTER
      page: 170
      pdf_page: 176
statements: 15
exercises: 11
content_sha256: 64e2a2f21b13a549bb934303352d828029af204421f9fa2da8a3d76d4b5ee959
translated_from: content/en/ens/III/04_s4_natural_integers_finite_sets.md
translation_method: google
source_content_sha256: b07b7ce28c5ec4cebf51e51a369145ff5f0d99cab971bd69c71b3b417b968e57
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: a4059062375a279deb2d56011bf5ed0b00be8460e31d526b645325c871200707
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 4.自然整数。有限集合

### 1.整数的定义

#### 定义 1 {#ens-iii-s4-def-1 .statement tag=03R9}

*如果 $\alpha \ne \alpha + 1$，基数 $\alpha$ 被认为是有限的。有限基数也称为自然整数（如果不存在混淆风险，则简称为整数 [^1]）。如果 $\operatorname{Card}(E)$ 是有限基数，则集合 $E$ 被称为有限； $\operatorname{Card}(E)$则称为$E$的元素的数。*

如果一个家庭 (章 II, § 3, no. 4) 的指标集合是有限的，则称其为“有限”。

*当我们说某个型的对象的数是整数$m$时，我们的意思是这些对象是有限集合的元素，其元素的数是$m$。 元素的数为$m$的集合也称为$m$元素的集合。*

#### 命题 1 {#ens-iii-s4-prop-1 .statement tag=03RA}

*基数$\alpha$是有限的当且仅当$\alpha + 1$是有限的。*

对于关系$\alpha = \mathfrak{b}$和$\alpha + 1 = \mathfrak{b} + 1$，基数$\alpha$和$\mathfrak{b}$之间是等价的（§ 3, no. 4，命题8）；因此，关系 $\alpha \ne \alpha + 1$ 和 $\alpha + 1 \ne (\alpha + 1) + 1$ 是等价的。

¶ 显然$0 \ne 1$；因此$0$是整数。由此可见$1$和$2$是整数。基数$2 + 1$和$(2 + 1) + 1$是整数，分别用$3$和$4$表示。

### 2. 整数之间的不等式

#### 命题 2 {#ens-iii-s4-prop-2 .statement tag=03RB}

*令$n$为整数。那么每个基数$\alpha$使得$\alpha \le n$是整数。如果$n \ne 0$，则存在唯一的整数$m$，使得$n = m + 1$，并且关系$\alpha < n$相当于$\alpha \le m$。*

如果$\alpha \le n$，则存在基数$\mathfrak{b}$使得$n = \alpha + \mathfrak{b}$（§ 3, no. 6，命题13）。那么 $(\alpha + 1) + \mathfrak{b} = (\alpha + \mathfrak{b}) + 1 = n + 1$ (§ 3, no. 3, 命题 5, 推论);从$n \ne n + 1$开始，我们有

$$
(\alpha + 1) + \mathfrak{b} \ne \alpha + \mathfrak{b}.
$$

因此$\alpha + 1 \ne \alpha$，这意味着$\alpha$是整数。如果$n \ne 0$，我们有$n \ge 1$（§ 3, no. 2），因此存在一个唯一的基数$m$，使得$n = m + 1$（§ 3, no. 6，命题13和no. 4，命题8）。从$m \leqslant n$开始，$m$就是整数，已经证明。最后，如果整数$a$使得$a < n$，我们有$n = a + b$，其中$b \neq 0$（§ 3, no. 6，命题13）；因为$b$是整数，所以我们有$b = c + 1$和$n = m + 1 = (a + c) + 1$。由此可见$m = a + c$ (§ 3, no. 4, 命题 8)，因此$a \leqslant m$。相反，如果$a \leqslant m$，我们有

$$a \leqslant m + 1 = n;$$

如果$a = n = m + 1$，我们就会有$a > m$，与假设相反。

#### 推论 1 {#ens-iii-s4-prop-2-cor-1 .statement tag=03RC}

*有限集合中的每个子集都是有限的。*

#### 推论 2 {#ens-iii-s4-prop-2-cor-2 .statement tag=03RD}

*如果* X *是有限集合* E *和* X $\neq$ E 的子集，*则*

$$\mathrm{Card}\ (\mathrm{X})\ <\ \mathrm{Card}\ (\mathrm{E}).$$

因为X包含在单个元素的E 由……组成的子集的补集X$'$中；我们有 $\mathrm{Card}\,(\mathrm{X}) \leqslant \mathrm{Card}\,(\mathrm{X}')$ 和 $\mathrm{Card}\,(\mathrm{E}) = \mathrm{Card}\,(\mathrm{X}') + 1$，因此 (命题 2) $\mathrm{Card}\,(\mathrm{X}') < \mathrm{Card}\,(\mathrm{E})$ 和 *更不必说* $\mathrm{Card}\,(\mathrm{X}) < \mathrm{Card}\,(\mathrm{E})$。

定义 1 表明，相反，如果 E 是集合使得

$$\mathrm{Card}\ (\mathrm{X}) < \mathrm{Card}\ (\mathrm{E})$$

对于 E 的每个子集 X 使得 X $\neq$ E，则 E 是有限的。

#### 推论 3 {#ens-iii-s4-prop-2-cor-3 .statement tag=03RE}

*如果* $f$ *是有限集合* E 的映射 *到集合* F，*则* $f(\mathrm{E})$ *是* F 的有限子集。

对于 $\mathrm{Card}\ (f(\mathrm{E})) \leqslant \mathrm{Card}\ (\mathrm{E})$（§ 3, no. 2、命题 3）。

#### 推论 4 {#ens-iii-s4-prop-2-cor-4 .statement tag=03RF}

*设* E *和* F *为两个有限集合，且数与元素相同，并让* $f$ *为* E *的映射入* F。 *则以下叙述是等价的：*

(a) $f$ *为单射*；
(b) $f$ *是一个满射*；
(c) $f$ *为双射。*

只要证明(a)和(b)是等价的就足够了。如果$f$是单射的，则$\mathrm{Card}(f(\mathrm{E})) = \mathrm{Card}\,(\mathrm{E}) = \mathrm{Card}\,(\mathrm{F})$，从而$f(\mathrm{E}) = \mathrm{F}$（推论2）。如果$f$不是单射，则令$x$和$x'$是E的两个元素，使得$x \neq x'$和$f(x) = f(x')$。然后，代入$\mathrm{E}' = \mathrm{E} - \{x\}$，根据推论2，我们有$f(\mathrm{E}') = f(\mathrm{E})$，从而$\mathrm{Card}(f(\mathrm{E})) \leqslant \mathrm{Card}\,(\mathrm{E}') < \mathrm{Card}\,(\mathrm{E})$；但从$\mathrm{Card}\,(\mathrm{F}) = \mathrm{Card}\,(\mathrm{E})$开始，就得出$f(\mathrm{E}) \neq \mathrm{F}$。

### 3.归纳原理

C61（原理 / 归纳）。 *令* $R\{n\}$ *理论上为关系* $\mathscr{T}$ *（其中n不是* $\mathscr{T}$*的常量）。* *假设关系*

$$R\{0\} \quad \text{and} \quad (\forall n)((n \text{ is an integer and } R\{n\}) \Rightarrow R\{n+1\})$$

* 定理等于* $\mathscr{T}$。 *在这些条件关系*

$$(\forall n)((n \text{ is an integer}) \Rightarrow R\{n\})$$

*是定理在*$\mathscr{T}$。

我们将通过矛盾来论证。假设关系

$$(\exists n)(n \text{ is an integer and } (\text{not } R\{n\}))$$

是真的。令$q$为整数，使得“不是$R\{q\}$”（辅助常数的方法；cf.章I, § 3, no. 3和§ 4, no. 1）。 整数$n$，其中“$n \leqslant q$和（不是$R\{n\}$）”形式是一个良序非空集合（§ 3, no. 2，注），因此它至少有元素$s$。如果$s = 0$，则“不是$R\{0\}$”，与假设相反。如果 $s > 0$，则$s = s' + 1$，其中 $s'$ 是整数，使得 $s' < s$ (no. 2，命题 2)。通过$s$的定义，我们有$R\{s'\}$，但是假设意味着$R\{s\}$为真，这与$s$的定义相反。

在序申请归纳原理特别需要证明关系

$$(n \text{ is an integer and } R\{n\}) \Rightarrow R\{n+1\}.$$

为此，通常使用辅助假设（章I, § 3, no. 3）的方法，也正是因为这个原因，关系“$n$是整数和$R\{n\}$”（甚至$R\{n\}$）被称为*归纳法假设*。

#### 注 {#ens-iii-s4-n3-rem-1 .statement tag=077T}

有各种判据，经常以“归纳的原理”的名义使用。它们都可以很容易地从 C61 推导出来，我们在这里指出其中最重要的：

(1) 设$S\{n\}$为关系

$$(\forall p)((n \text{ is an integer and } p \text{ is an integer and } p < n) \Rightarrow R\{p\})$$

并假设 $S\{n\}$ *暗示* $R\{n\}$。然后关系

$$(\forall n)((n \text{ is an integer}) \Rightarrow R\{n\})$$

是真的。对于关系$S\{0\}$为真，假设$S\{n\}$意味着$R\{n\}$；由于关系$m < n + 1$等价于$m \leqslant n$（no. 2，命题2），关系$S\{n + 1\}$等价于“$S\{n\}$和$R\{n\}$”，因而，$S\{n\}$意味着$S\{n + 1\}$。因而，标准 C61 证明关系

$$(\forall n)\ ((n \text{ is an integer}) \Rightarrow S\{n\})$$

是真的，并且由于$S\{n\}$意味着$R\{n\}$，关系

$$(\forall n)\ ((n \text{ is an integer}) \Rightarrow R\{n\})$$

是真的。

(2) 令$k$为整数，并令$R\{n\}$为关系，使得关系

$$R\{k\} \text{ and } (\forall n)\ ((n \text{ is an integer} \geqslant k \text{ and } R\{n\}) \Rightarrow R\{n + 1\})$$

是真的。然后关系

$$(\forall n)\ ((n \text{ is an integer} \geqslant k) \Rightarrow R\{n\})$$

为 true（“*归纳从 k* 开始”）。让 $S\{n\}$ 为关系

$$(n \geqslant k) \Rightarrow R\{n\}.$$

然后通过案例析取方法，我们发现$S\{0\}$为真。另一方面，很容易验证关系

$$(n \text{ is an integer and } S\{n\}) \Rightarrow S\{n + 1\}$$

是真的。从 C61 可以得出关系

$$(n \text{ is an integer}) \Rightarrow S\{n\}$$

是真的，这就证明了我们的断言。

(3) 令$a$和$b$为两个整数，使得$a \leqslant b$，并令$R\{n\}$为关系，使得

$$R\{a\} \text{ and } (\forall n)((n \text{ is an integer and } a \leqslant n < b \text{ and } R\{n\}) \Rightarrow R\{n + 1\}).$$

然后关系

$$(\forall n)((n \text{ is an integer and } a \leqslant n \leqslant b) \Rightarrow R\{n\})$$

是真的。 证明与上例类似；我们将$S\{n\}$视为关系“$(a \leqslant n < b) \Rightarrow R\{n\}$”（“*归纳限制在一个区间*”）。

(4) 设$a$、$b$为两个整数，使得$a \leqslant b$，并令$\mathrm{R}\{n\}$为关系，使得

$\mathrm{R}\{b\}$和$(\forall n)((n$是整数和$a \leqslant n < b$和$\mathrm{R}\{n+1\}) \Rightarrow \mathrm{R}\{n\})$。

然后关系

$$(\forall n)((n \text{ is an integer and } a \leqslant n \leqslant b) \Rightarrow \mathrm{R}\{n\})$$

是真的。因为我们有关系

$(n$ 是整数和$a \leqslant n < b$ 并且（不是$\mathrm{R}\{n\}$））$\Rightarrow$ 不是$\mathrm{R}\{n+1\}$。

如果对于某些$n$，这样我们有$a \leqslant n \leqslant b$（不是$\mathrm{R}\{n\}$），则可以从（3）得出（不是$\mathrm{R}\{b\}$），与假设、从而相反，结果（*“降序归纳”*）。

### 4.有限子集有序集

#### 命题 3 {#ens-iii-s4-prop-3 .statement tag=03L9}

*令* E *为右向预序集合*（分别为*格子*，分别为*全序集*）。 *然后* E *的每个非空有限子集都在上方*（分别*具有至少上界和下确界*，分别*具有最大元素和至少元素*）。

证明正在考虑子集元素数$n$的归纳。对于 $n = 1$ 来说，结果是微不足道的。令X为E的$n + 1$元素的子集（与$n \geqslant 1$），并放入$\mathrm{X} = \mathrm{Y} \cup \{x\}$，其中Y有$n$元素，因此不为空。归纳假设意味着Y存在上界（分别至少上界、最大元素）$y$。由于E是右向的（分别是格子、全序），$\{x, y\}$有上界（分别至少上界， 最大元素），显然是X的上界（至少上界，最大元素）。

#### 推论 1 {#ens-iii-s4-prop-3-cor-1 .statement tag=03LA}

*每个全序有限集合都是良序的并且有最大元素。*

#### 推论 2 {#ens-iii-s4-prop-3-cor-2 .statement tag=03LB}

*每个有限有序集合都有极大元素。*

对于这样的集合由推论 1 (cf. § 2, no. 4, 定理 2) 归纳。

### 5.有限特征标的性质

#### 定义 2 {#ens-iii-s4-def-2 .statement tag=03LC}

*令*E *为集合。 集合* $\mathfrak{S}$ *of 子集 of* E * 被认为是有限的特征标，如果关系* $\mathrm{X} \in \mathfrak{S}$ *等价于关系“每有限子集 of* X *属于到* $\mathfrak{S}$”。

A property $P\{X\}$ of a subset $X$ of a set $E$ is said to be *of finite character* if the set of subsets $X$ of $E$ for which $P\{X\}$ is true is of finite character.

*例*

#### 例 1 {#ens-iii-s4-n5-exa-1 .statement tag=03T9}

有序集合 $E$ 的总共有序子集中的集合是有限的特征标。事实上，$E$的子集$X$是全有序的当且仅当两个元素的$X$由……组成中的每一个子集都是全有序的。

#### 例 2 {#ens-iii-s4-n5-exa-2 .statement tag=03TA}

\* 模的所有自由子集中的集合是有限的特征标。对于域的扩张的所有代数自由子集的集合也是如此。

#### 例 3 {#ens-iii-s4-n5-exa-3 .statement tag=03TB}

模$E$子模集合不是有限的特征标，因为$E$子模有限子集不一定是$E$子模。 \*

#### 定理 1 {#ens-iii-s4-thm-1 .statement tag=03LD}

*集合$E$的子集的每个集合$\mathfrak{S}$，其有限特征标都有极大元素（按包含排序时）。*

通过定理 2 of § 2, no. 4 足以证明 $\mathfrak{S}$ 是归纳性的。为此，我们将证明，如果$\mathfrak{G}$是完全按包含排序的$\mathfrak{S}$中的任何子集，则$\mathfrak{G}$属于到$\mathfrak{S}$的集合到并$X$（§ 2, no. 4，定理） 2、推论2)。由于$\mathfrak{S}$是有限的特征标，因此足以证明$X$属于到$\mathfrak{S}$的每一个有限子集$Y$。现在，对于每个$y \in Y$，都存在集合$Z_y \in \mathfrak{G}$，这样$y \in Z_y$。由于集合 $Z_y$ $(y \in Y)$ 的集合是有限的且按包含全序，因此有最大元素 $S$（no. 4，推论 1 至命题 3）；在其他字中，存在集合$S \in \mathfrak{G}$使得$Y \subset S$。但是由于 $S \in \mathfrak{S}$ 和 $Y$ 是 $S$ 的有限子集，我们有 $Y \in \mathfrak{S}$，因为 $\mathfrak{S}$ 是有限的特征标；这样就完成了证明。

### 习题{#ens-iii-s4-exercises}

§ 4](exercises/s4/)参见[习题。

“整数”的[^1]:概念稍后将在代数中推广，其中我们将定义*有理数整数*和*代数整数*。
