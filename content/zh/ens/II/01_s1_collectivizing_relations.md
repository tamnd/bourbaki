---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 1
section_title: Collectivizing relations
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 65-72, 123
pdf_pages: 0072-0079, 0130-0130
extraction: ocr
subsections:
    - "no": 1
      title: THE THEORY OF SETS
      page: 65
      pdf_page: 72
    - "no": 2
      title: INCLUSION
      page: 66
      pdf_page: 73
    - "no": 3
      title: THE AXIOM OF EXTENT
      page: 67
      pdf_page: 74
    - "no": 4
      title: COLLECTIVIZING RELATIONS
      page: 67
      pdf_page: 74
    - "no": 5
      title: THE AXIOM OF THE SET OF TWO ELEMENTS
      page: 69
      pdf_page: 76
    - "no": 6
      title: THE SCHEME OF SELECTION AND UNION
      page: 69
      pdf_page: 76
    - "no": 7
      title: COMPLEMENT OF A SET. THE EMPTY SET
      page: 71
      pdf_page: 78
statements: 10
exercises: 6
content_sha256: 3cef84002c7cda9d0c817b070eaa3315f7559a3b03f03a54bef60eddd7306f3c
translated_from: content/en/ens/II/01_s1_collectivizing_relations.md
translation_method: google
source_content_sha256: 15e4c05cbeaa37f947e4dd88b319dfea58ef5aed00b479f31e5cbe9ae7b53342
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: c363be80fb669661935fdb582382ddc61757f0b84b116b5b66a8369ce4eddba5
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 1. 集合化关系

### 1. 集合论

*集合论*是一个理论，其中包含关系符号$=$、$\in$和实体符号$\supset$（所有这些符号都是权2）；在章I中给出的加法到概形S1到S7中，包含概形S8，将在no. 6中介绍，以及显式公理A1（no. 3。）A2（no. 5）， A3（§ 2, no. 1）、A4（§ 5, no. 1）和A5（章III, § 6, no. 1），这些明确的公理包含没有字母；在其他字中，集合论是一个*没有常数*的理论。

由于集合论是平等的理论，所以章I的结果是适用的。

¶ 从现在开始，除非明确指出相反，我们将始终以比集合论更强的理论（章I, § 2, no. 4）进行论证；如果没有提及理论，则假定隐含集合论。在许多情况下，显然这个假设是多余的，读者应该不难确定在哪个弱于集合论的理论中所陈述的结果是有效的。

如果$T$和$U$是项，则集合$\in TU$是关系（称为成员的*关系*），实际上我们用以下方式之一编写：$T \in U$，$(T) \in (U)$，“$T$属于到 $U$”，“$T$ 是 $U$ 的元素”。 关系“不是$(T \in U)$”写为$T \notin U$。

从“朴素”点的角度来看，许多数学实体可以被视为对象的集合或“集合”。我们并不寻求形式化这个概念，并且在接下来的形式主义解释中，字“集合”被视为严格与“项”同义。特别是，诸如“let X be 集合”之类的短语在原理中是相当多余的，因为每个字母都是项。引入这些短语只是为了帮助直观地解释文本。

### 2. 包容性

#### 定义 1 {#ens-ii-s1-def-1 .statement tag=03H5}

*关系表示为* $(\forall z)((z \in x) \Rightarrow (z \in y))$，*其中仅出现字母$x$和$y$，以下列方式之一书写：* $x \subset y$、$y \supset x$、*“$x$包含在$y$”、“$y$” 包含于 $x$”，“$x$ 是 $y$ 的子集”。 关系*“不是$(x \subset y)$”*写为*$x \not\subset y$*或*$y \not\supset x$。

根据章I, § 1, no. 1中提到的约定，这个定义需要以下元数学约定。设$T$和$U$为组合；如果我们在集合$x \subset y$中用$T$代替$x$，用$U$代替$y$，我们得到一个用$T \subset U$表示的集合；如果我们用$\mathbf{x}$、$\mathbf{y}$字母表示，它们与$x$、$y$不同，并且彼此不同，并且既不在$T$中也不在$U$中出现，则汇编$T \subset U$与$(T|\mathbf{x})(U|\mathbf{y})(\mathbf{x}|x)(\mathbf{y}|y)(x \subset y)$相同，因此由CS8、CS9组成(章 I, § 4, no. 1)，以及 CS5 (章 I, § 1, no. 2) 与 $(\forall z)((z \in T) \Rightarrow (z \in U))$，前提是 $z$ 是既不在 $T$ 也不在 $U$ 中出现的字母。

从现在开始，每当我们陈述一个数学定义时，我们都不会提及它所蕴含的元数学约定。

CS12。 *令$T$、$U$、$V$为组合，并令$x$为字母。那么组装$(V|x)(T \subset U)$与$(V|x)T \subset (V|x)U$相同。*

这紧随 CS9 (章 I, § 4, no. 1) 和 CS5 (章 I, § 1, no. 2)。

CF13。 *如果$T$和$U$是项，$T \subset U$就是关系。*

这紧随 CF8 (章 I, § 1, no. 4)。

¶ 形式 $T \subset U$ 中的每个关系（其中 $T$ 和 $U$ 是项）称为*包含关系*。

从现在开始，我们不再明确地写出代换判据以及定义之后的构成判据。然而，应该注意的是，这些判据经常会在证明中隐式使用。

为了证明$\mathscr{T}$理论中的关系$x \subset y$，通过C27（章I, § 4, no. 1），证明通过将$\mathscr{T}$的$z \in x$与公理邻接而获得的理论中的$z \in y$就足够了，其中$z$是与 $x$、$y$ 和理论常数不同的字母。在实践中，我们说“让$z$是$x$的元素”，并且我们尝试证明$z \in y$。

#### 命题 1 {#ens-ii-s1-prop-1 .statement tag=03P9}

$x \subset x$。

显然。

#### 命题 2 {#ens-ii-s1-prop-2 .statement tag=03PA}

$(x \subset y$ 和 $y \subset z) \Rightarrow (x \subset z)$。

毗邻假设 $x \subset y$、$y \subset z$ 和 $u \in x$。然后关系

$$(u \in x) \Rightarrow (u \in y), \qquad (u \in y) \Rightarrow (u \in z),$$

为真，因此关系 $u \in z$ 为真。

### 3. 外延公理

*外延公理* 是以下公理：

A1。 $\qquad (\forall x)(\forall y)((x \subset y \text{ and } y \subset x) \Rightarrow (x = y))$。

直观上，这个公理表达了这样的事实：两个具有相同元素的集合是相等的。

因此，为了证明$x = y$，只需在通过邻接假设$z \in x$获得的理论中证明$z \in y$，以及在通过邻接假设$z \in y$获得的理论中证明$z \in x$就足够了，其中$z$是与$x$、$y$不同的字母，并且常数。

C48。 *设$\mathbf{R}$为关系，$x$为字母，$y$为与$x$不同的字母，$\mathbf{R}$中未出现。那么关系 $(\forall x)((x \in y) \Leftrightarrow \mathbf{R})$ 在 $y$ 中是单值。*

设$z$是与$x$不同的字母，它没有出现在$\mathbf{R}$中。毗邻假设

$$(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\forall x)((x \in z) \Leftrightarrow \mathbf{R}).$$

那么我们依次有定理

$$(\forall x)(((x \in y) \Leftrightarrow \mathbf{R}) \text{ and } ((x \in z) \Leftrightarrow \mathbf{R})),$$
$$(\forall x)((x \in y) \Leftrightarrow (x \in z)),$$
$$y \subset z, \qquad z \subset y.$$

到A1我们就有$y = z$。这就证明了C48。

### 4. COLLECTIVIZING RELATIONS

令$\mathbf{R}$为关系，令$x$为字母。如果 $y$ 和 $y'$ 表示不同于 $x$ *且未出现在 $\mathbf{R}$* 中的字母，则关系

$$(\exists y)(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\exists y')(\forall x)((x \in y') \Leftrightarrow \mathbf{R})$$

与 CS8 相同 (章 I, §4, no. 1)。由此定义的关系（不包括包含$x$）由$\operatorname{Coll}_xR$表示。

¶ 如果在理论$\mathscr{T}$中$\operatorname{Coll}_xR$是定理，则$R$在$x$*中被称为*集合化在$\mathscr{T}$中。在这种情况下，我们可以引入一个辅助常数$a$，与$x$和$\mathscr{T}$的常数不同，并且它不会出现在$R$中，并带有介绍性公理$(\forall x)((x \in a) \Longleftrightarrow R)$，或者等效地（如果$x$不是$\mathscr{T}$的常数）$(x \in a) \Longleftrightarrow R$。

直观地说，说$x$中$R$是集合化，就是说存在集合$a$，使得拥有性质$R$的对象$x$恰好是元素 $a$。

*例*

#### 例 1 {#ens-ii-s1-n4-exa-1 .statement tag=03RZ}

关系 $x \in y$ 显然是 $x$ 中的集合化。

#### 例 2 {#ens-ii-s1-n4-exa-2 .statement tag=03S0}

关系 $x \neq x$ *不是 $x$* 中的集合化；在其他字，（不是$\operatorname{Coll}_x(x \neq x)$）是定理。让我们用反证法来论证，假设$x \neq x$是集合化。令 $a$ 为辅助常数，与 $x$ 和理论常数不同，具有介绍性公理

$$
(\forall x)((x \neq x) \Longleftrightarrow (x \in a)).
$$

然后关系

$$
(a \neq a) \Longleftrightarrow (a \in a)
$$

由 C30 成立 (章 I, §4, no. 3)。格析取的方法（章I, §3, no. 3）首先证明关系$a \neq a$为真，然后关系$a \in a$为真，这是荒谬的。

**C49.** *令 $R$ 为关系，$x$ 为字母。如果$R$在$x$中是集合化，关系$(\forall x)((x \in y) \Longleftrightarrow R)$，其中$y$是与$x$不同的字母，它不会出现在$R$中，但在$y$中起作用。*

这紧接着 C48。

在下文中，我们经常可以使用定理或形式 $\operatorname{Coll}_xR$。代表项

$$
\tau_y(\forall x)((x \in y) \Longleftrightarrow R),
$$

它不依赖于字母$y$的选择（与$x$不同，并且不出现在$R$中），我们将引入一个功能符号$\mathscr{E}_x(R)$； 相应的项不包含 $x$。这个项由“所有$x$的集合使得$R$”表示。 定义 (章 I, §4, no. 1) 关系

$$
(\forall x)((x \in \mathscr{E}_x(R)) \Longleftrightarrow R)
$$

与 $\mathrm{Coll}_x R$ *相同*；因此关系 $R$ *等于*

$$x \in \mathscr{E}_x(R).$$

C50。 *令$R$、$S$为两个关系，令$x$为一个字母。如果$R$和$S$是$x$中的集合化，则关系$(\forall x)(R \Rightarrow S)$相当于*

$$\mathscr{E}_x(R) \subset \mathscr{E}_x(S),$$

*and 关系 $(\forall x)(R \Leftrightarrow S)$ is equivalent to $\mathscr{E}_x(R) = \mathscr{E}_x(S)$.*

这紧接着前面的注以及定义 1 和公理 A1。

### 5. THE AXIOM OF THE 集合 OF TWO 元素

A2。 $\qquad\qquad (\forall x)(\forall y)\ \mathrm{Coll}_z(z = x \text{ or } z = y).$

该公理说，如果$x$和$y$是对象，则存在集合，其唯一的元素是$x$和$y$。

#### 定义 2 {#ens-ii-s1-def-2 .statement tag=03H6}

*集合$\mathscr{E}_z (z = x \text{ or } z = y)$，其中元素只有$x$和$y$，用$\{x, y\}$表示。*

因而，关系$z \in \{x, y\}$相当于“$z = x$或$z = y$”；从 C50 可以得出 $\{y, x\} = \{x, y\}$。

令$R\{z\}$为关系，并令$x, y$为与$z$不同的字母。从判据 C32、C33 (章 I, §4, no. 3) 和 C43 (章 I, §5, no. 1) 很容易得出关系 $(\exists z)((z \in \{x, y\})$ 和 $R\{z\})$ 相当于“$R\{x\}$ 或 $R\{y\}$”；因此关系 $(\forall z)((z \in \{x, y\}) \Rightarrow R\{z\})$ 相当于“$R\{x\}$ 和 $R\{y\}$”。

集合$\{x, x\}$，简称为$\{x\}$，称为*集合，其唯一的元素为$x$*； 关系 $z \in \{x\}$ 相当于$z = x$，关系 $x \in \mathrm{X}$ 相当于$\{x\} \subset \mathrm{X}$。

### 6. 选择并集方案

选择和并*的*概形如下：

S8。 *令$R$为关系，令$x$和$y$为不同的字母，并令$X$和$Y$为与$R$中未出现的$x$和$y$不同的字母。然后关系*

(1) $\quad (\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ and } R))$ *是一个公理。*

我们首先证明这个规则确实是概形。令$S$表示关系（1），并用项$T$代替$S$中的字母$z$；根据 CS8 (章 I, §4, no. 1)，我们可以假设 $x$、$y$、$X$、$Y$ 与 $z$ 不同，并且不会出现在 $T$ 中。那么 $(T|z)S$ 与

$$(\forall y)(\exists X)(\forall x)(R' \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ and } R')),$$

其中$R'$是$(T|z)R$。

直观上，关系$(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$意味着对于每个对象$y$都存在集合$X$（可能取决于$y$），使得对象$x$与给定对象位于关系$R$中$y$是$X$的元素（但不一定是$X$的全部）。 选择并集方案断言，如果是这种情况，并且$Y$是任何集合，则存在集合，其元素恰好是对象$x$，它们位于关系$R$中，并且至少有一个对象$y$为集合$Y$。

C51。 *令$P$为关系，令$A$为集合，令$x$为$A$中未出现的字母。那么关系“$P$和$x \in A$”就是$x$中的集合化。*

让$R$表示关系“$P$和$x = y$”，其中$y$是一个不同于$x$的字母，它既不出现在$P$也没有出现在$A$中。 关系

$$(\forall x)(R \Rightarrow (x \in \{y\}))$$

由 C27 (章 I, §4, no. 1) 成立。令$X$为与$x$和$y$不同的字母，其未出现在$P$中。前面的关系与$(\{y\}|X)((\forall x)(R \Rightarrow (x \in X)))$相同（因为$x$与$y$不同），因此根据S5和C27，关系$(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$为真（章I, §4，编号1和2）。如果从 S8 和 C30 (章 I, §4, no. 3) 得出关系

$$(A|Y)\ \mathrm{Coll}x(\exists y)(y \in Y \text{ and } R)$$

（其中$Y$是一个没有出现在$R$中的字母）为真，并且这个关系与$\mathrm{Coll}_x(\exists y)(y \in A \text{ and } R)$相同（因为$x$和$y$都没有出现在$A$中）。最后，关系“$y \in A$和$R$”相当于C43的“$x = y$和$x \in A$和$P$”（章I, §5, no. 1）；因为$x$既不在$P$中出现，也不在$A$、关系中出现

$$(\exists y)(x = y \text{ and } x \in A \text{ and } P)$$

等价于 C33 (章 I, §4, no. 3) 的“$((\exists y)(x = y))$ 和 $x \in A$ 和 $P$”，因此等价于“$P$ 和 $x \in A$”，因为 $(\exists y)(x = y)$ 为真。

¶ 集合 $\mathscr{E}_x(P$ 和 $x \in A)$ 被称为所有 $x \in A$ 的 *集合，使得 $P$* （\* 因此我们可以说所有实数的集合，使得 $P_*$）。

C52。 *令$R$为关系，$A$为集合，$x$为$A$中未出现的字母。如果关系$R \Rightarrow (x \in A)$是定理，那么$R$在$x$中就是集合化。*

对于$R$则相当于“$R$和$x \in A$”。

#### 注 {#ens-ii-s1-n6-rem-1 .statement tag=03H7}

令$R$为关系，即$x$中的集合化，并令$S$为关系，使得$(\forall x)(S \Rightarrow R)$为定理。那么$S$在$x$中就是集合化；对于 $R$ 等价于 $x \in \mathscr{E}_x(R)$，因此

$$S \Rightarrow (x \in \mathscr{E}_x(R))$$

是定理，断言由 C52 得出。另请注意，在这种情况下，我们通过 C50 得到 $\mathscr{E}_X(S) \subset \mathscr{E}_X(R)$。

C53。 *令 $T$ 为项、$A$ 集合、$x$ 和 $y$ 不同的字母。假设$x$没有出现在$A$中，并且$y$没有出现在$A$和$T$中。那么关系$(\exists x)(y = T$和$x \in A)$就是$y$中的集合化。*

设$R$为关系$y = T$。 关系 $(\forall y)(R \Rightarrow (y \in \{T\}))$ 为真，因此 $(\forall x)(\exists X)(\forall y)(R \Rightarrow (y \in X))$ 也为真，其中 $X$ 是一个字母，与 $y$ 不同，$R$ 中没有出现。凭借S8，关系$(\exists x)(x \in A$和R)在$y$中为集合化，并证明了C53。

¶ 关系 $(\exists x)(y = T$ 和 $x \in A)$ 通常读作如下：“对于某些 $x$ 属于至 $A$，$y$ 可以放入形式 $T$”。 集合

$$\mathscr{E}_y((\exists x)(y = T \text{ and } x \in A))$$

一般称为$x \in A$* 形式 $T$ 对象 *集合。如此表示的组件包含既不是$x$也不是$y$，并且不依赖于C53的字母$y$满足条件的选择。

### 7. 集合的补集。 空集

通过 C51，关系 $(x \notin \mathrm{A}$ 和 $x \in \mathrm{X})$ 是 $x$ 中的集合化。

#### 定义 3 {#ens-ii-s1-def-3 .statement tag=03H8}

*设*$\mathrm{A}$*为集合*$\mathrm{X}$中的子集。 * $\mathrm{X}$ * 元素 *集合不属于到* $\mathrm{A}$，*也就是说集合* $\mathscr{E}x$ $(x \notin \mathrm{A}$ *和* $x \in \mathrm{X})$，*称为* $\mathrm{A}$ *中的补集$\mathrm{X}$，*并用* $\complement_{\mathrm{X}}\mathrm{A}$ *或* $\mathrm{X} - \mathrm{A}$ 表示（如果不存在混淆风险，则用$\complement\mathrm{A}$ 表示）。

设A为集合X中的子集； 关系“$x \in \mathrm{X}$和$x \notin \mathrm{A}$”和$x \in \complement_{\mathrm{X}}\mathrm{A}$是等价的。因而，关系“$x \in \mathrm{X}$和$x \notin \complement_{\mathrm{X}}\mathrm{A}$”相当于“$x \in \mathrm{X}$和$(x \notin \mathrm{X}$或$x \in \mathrm{A})$”，因此相当于$x \in A$。在其他字中，$A = \complement_X(\complement_X A)$是真正的关系。类似地，如果B是X的子集，则关系$A \subset B$和$\complement_X B \subset \complement_X A$是等价的。

#### 定理 1 {#ens-ii-s1-thm-1 .statement tag=03H9}

*关系* $(\forall x)(x \notin X)$ *在* X 中起作用。

对于关系$(\forall x)(x \notin X)$意味着$(\forall Y)(X \subset Y)$；根据范围公理，关系$(\forall x)(x \notin X)$因此在X中是单值。另一方面，关系$(\forall x)(x \notin \complement_Y Y)$为真，这证明$(\exists X)(\forall x)(x \notin X)$为真。

¶ 项 $\tau_x((\forall x)(x \notin X))$ 相应的对于这个泛函关系，用函数符号$\emptyset$表示，称为*空集* [^1]； 关系 $(\forall x)(x \notin X)$，相当于$X = \emptyset$，读作如下：“*集合* X *为空*”。我们有定理$x \notin \emptyset$、$\emptyset \subset X$、$\complement_X X = \emptyset$、$\complement_X \emptyset = X$。 关系 $X \subset \emptyset$ 相当于$X = \emptyset$。如果 $R\{x\}$ 是关系，则关系 $(\forall x)((x \in \emptyset) \Rightarrow R\{x\})$ 为真。

#### 注 {#ens-ii-s1-n7-rem-1 .statement tag=03PB}

不存在每个对象都是元素的集合；在其他字中，“不是$(\exists X)(\forall x)(x \in X)$”是定理。因为如果存在这样的集合，那么通过C52，每个关系将是集合化。但我们已经看到（no. 4）关系$x \notin x$不是集合化。

### 习题{#ens-ii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。

[^1]: The term denoted by $\emptyset$ is therefore $\tau \neg \neg \in \tau \neg \neg \in \square\square\square$.
