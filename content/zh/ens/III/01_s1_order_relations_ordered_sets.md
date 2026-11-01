---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 1
section_title: Order relations. Ordered sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 131-148, 212-221
pdf_pages: 0137-0154, 0218-0227
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN ORDER RELATION
      page: 131
      pdf_page: 137
    - "no": 2
      title: PREORDER RELATIONS
      page: 133
      pdf_page: 139
    - "no": 3
      title: NOTATION AND TERMINOLOGY
      page: 135
      pdf_page: 141
    - "no": 4
      title: ORDERED SUBSETS. PRODUCT OF ORDERED SETS
      page: 136
      pdf_page: 142
    - "no": 5
      title: INCREASING MAPPINGS
      page: 138
      pdf_page: 144
    - "no": 6
      title: MAXIMAL AND MINIMAL ELEMENTS
      page: 139
      pdf_page: 145
    - "no": 7
      title: GREATEST ELEMENT AND LEAST ELEMENT
      page: 140
      pdf_page: 146
    - "no": 8
      title: UPPER AND LOWER BOUNDS
      page: 141
      pdf_page: 147
    - "no": 9
      title: LEAST UPPER BOUND AND GREATEST LOWER BOUND
      page: 141
      pdf_page: 147
    - "no": 10
      title: DIRECTED SETS
      page: 145
      pdf_page: 151
    - "no": 11
      title: LATTICES
      page: 145
      pdf_page: 151
    - "no": 12
      title: TOTALLY ORDERED SETS
      page: 146
      pdf_page: 152
    - "no": 13
      title: INTERVALS
      page: 147
      pdf_page: 153
statements: 52
exercises: 24
content_sha256: 7eafddc995818e9b870051dcac56293889f75ac321f1b7b72bcbeb40d32ff6dc
translated_from: content/en/ens/III/01_s1_order_relations_ordered_sets.md
translation_method: google
source_content_sha256: 14e9fa04ef3714dde5ebc1c24c59c34cba4c8b4444c04468c4103f599e7d160e
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 33e5ce13da55f2f76a792f8ee387086b991ca566b0034749f1cb6feccee1c462
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 1. 序关系。 有序集

### 1. 定义序关系

令$R\{x, y\}$为关系，$x$和$y$是不同的字母。相对于字母 x 和 y*（或 *x 和 y* 之间），R 被称为 *序关系，如果

$$(R\{x,\, y\} \ \text{ and } \ R\{\, y,\, z\}) \Rightarrow R\{x,\, z\},$$
$$(R\{x,\, y\} \ \text{ and } \ R\{\, y,\, x\}) \Rightarrow (x = y),$$
$$R\{x, y\} \Rightarrow (R\{x,\, x\} \ \text{ and } \ R\{\, y,\, y\}).$$

上面的第一个关系表示R对于字母$x$和$y$（章II, § 6, no. 1）是*传递*的。

*例*

(1) 等式*的*关系，$x = y$，是序关系。

(2) 关系$X \subset Y$是X和Y之间的序关系（章II, § 1, no. 2、命题1和2以及公理A1），通常称为*包含关系*。

(3) 令$R\{x, y\}$为序关系，介于$x$和$y$之间。 关系 $R\{\, y,\, x\}$ 则序关系 *位于 x 和 y* 之间，称为序关系 $R\{x,\, y\}$ 的“对立”。

集合* E 上的 *序关系对于两个不同的字母 $x$、$y$ 来说是序关系 $R\{x,\, y\}$，这样关系 $R\{x,\, x\}$ *等于* $x \in E$（在其他字中，是这样$R\{x,\, y\}$ 在 E (章 II, § 6, no. 1) 上是*自反*。那么关系$R\{x,\, y\}$意味着“$x \in E$和$y \in E$”，关系$(R\{x,\, y\}$和$R\{\, y,\, x\})$相当于“$x \in E$和$y \in E$和$x = y$”。

*例*

#### 例 1 {#ens-iii-s1-n1-exa-1 .statement tag=03SH}

等式的关系以及包含在集合上不是序关系，因为关系 $x = x$ 和 $\mathrm{X} \subset \mathrm{X}$ 不是集合化 (章 II, § 1, no. 7)。

#### 例 2 {#ens-iii-s1-n1-exa-2 .statement tag=03SI}

令$\mathrm{R}\}x,\ y\{$为$x$和$y$之间的序关系，并令E为集合，使得$x \in \mathrm{E}$蕴含$\mathrm{R}\}x,\ x\{$（注意空集满足条件）。 关系“$\mathrm{R}\}x,\ y\{$和$x \in \mathrm{E}$和$y \in \mathrm{E}$”则E上的序关系，立即得到验证；它在 E (cf. no. 4) 上被 $\mathrm{R}\}x,y\{$ *诱发* 称为序关系。通过滥用语言，短语“E 的元素之间的关系 $\mathrm{S}\}x,\ y\{$ 是序关系”经常用来代替“E 上的关系（$\mathrm{S}\}x,\ y\{$ 和 $x \in \mathrm{E}$ 和 $y \in \mathrm{E}$）是序关系”。对于例，如果A是集合，则关系“$\mathrm{X} \subset \mathrm{Y}$和$\mathrm{X} \subset \mathrm{A}$和$\mathrm{Y} \subset \mathrm{A}$”是A的子集之间的序关系。

#### 例 3 {#ens-iii-s1-n1-exa-3 .statement tag=03SJ}

设E、F为集合。 关系“*g 扩展 f*”是 E 的子集映射集合到 F 上的序关系（$f$ 和 $g$ 之间）。

#### 例 4 {#ens-iii-s1-n1-exa-4 .statement tag=03V3}

在集合E子集集合集合$\mathfrak{P}(\mathfrak{P}(\mathrm{E}))$中，令$\mathscr{P}$为E(章II, § 4, no. 7)*划分*集合。我们记得，如果给定任何$\mathrm{Y} \in \varpi'$，则存在$\mathrm{X} \in \varpi$使得$\mathrm{Y} \subset \mathrm{X}$（章II, § 4, no. 6），划分$\varpi$据说比划分$\varpi'$*粗糙*。对于E的每个划分$\varpi$，令$\tilde{\varpi}$为E上$\varpi$定义的等价关系图（章II, § 6, no. 2），也就是说，（互为不相交的）集合的并 $\mathrm{A} \times \mathrm{A}$，其中 A 穿过$\varpi$。 关系“$\varpi$比$\varpi'$更粗糙”立即被视为相当于$\tilde{\varpi} \supset \tilde{\varpi}'$，因此序关系位于集合$\mathscr{P}$之间，介于$\varpi$和$\varpi'$之间。

集合 E 上的*排序*是对应 $\Gamma = (\mathrm{G},\ \mathrm{E},\ \mathrm{E})$，以 E 作为源和目标，并且关系 $(x,\ y) \in \mathrm{G}$ 是 E 上的序关系。通过滥用语言，我们将有时将 $\Gamma$ 的图 G 称为 E 上的排序。如果$\mathrm{R}\}x,\ y\{$ 是 E 上的序关系，它有一个在 E 上排序的图。

#### 命题 1 {#ens-iii-s1-prop-1 .statement tag=03JA}

*对应* $\Gamma$ *在* E *和* E *之间是对* E *的排序当且仅当其图* G *满足以下条件 :*

（一）$\mathrm{G} \circ \mathrm{G} = \mathrm{G}$。

(b) *集合* $\mathrm{G} \cap \overset{-1}{\mathrm{G}}$ *是* $\mathrm{E} \times \mathrm{E}$ 的对角线* $\Delta$ *。

对于关系 $((x,\ y) \in \mathrm{G}$ 和 $(y,\ z) \in \mathrm{G}) \Rightarrow ((x,\ z) \in \mathrm{G})$ 可以写成 $\mathrm{G} \circ \mathrm{G} \subset \mathrm{G}$ 和关系

$$((x,\ y) \in \mathrm{G} \text{ and } (y,\ x) \in \mathrm{G}) \Leftrightarrow (x = y \text{ and } x \in \mathrm{E} \text{ and } y \in \mathrm{E})$$

可以写成$\mathrm{G} \cap \overset{-1}{\mathrm{G}} = \Delta$。然后从$\mathrm{G} \cap \overset{-1}{\mathrm{G}} = \Delta$推出$\Delta \subset \mathrm{G}$、从而$\mathrm{G} = \Delta \circ \mathrm{G} \subset \mathrm{G} \circ \mathrm{G}$；因为也$\mathrm{G} \circ \mathrm{G} \subset \mathrm{G}$，我们有

$$\mathrm{G} \circ \mathrm{G} = \mathrm{G}.$$

### 2. 预序关系

令$R\{x, y\}$为关系，$x$和$y$是不同的字母。如果 $R$ 是传递性的，并且如果我们有 $R\{x, y\} \Rightarrow (R\{x, x\}$ 和 $R\{y, y\})$，则并不一定得出 $R$ 是序关系，因为关系

$$(R\{x, y\} \text{ and } R\{y, x\})$$

并不一定意味着$x = y$。 $R\{x, y\}$据说是$x$和$y$之间的*预序关系*；那么$R\{y, x\}$也是$x$和$y$之间的预序关系，称为关系$R\{x, y\}$的*对立*。

对于例，令$\mathfrak{R}$为$\mathfrak{P}(E)$的子集的集合，它们是E的覆盖（章II, § 4, no. 6）。 关系“$\mathfrak{R}$比$\mathfrak{R}'$粗”在元素$\mathfrak{R}$之间，$\mathfrak{R}$（章II, § 4, no. 6）的$\mathfrak{R}'$是及物和自反的。但两种不同的覆盖物可能会比另一种更粗糙。对于例，当$\mathfrak{R}'$是$\mathfrak{R}$的并（在$\mathfrak{P}(E)$中）和$\mathfrak{R}$的集合中包含的E的子集但不是属于到$\mathfrak{R}$时，就是这种情况。

但无论如何，关系$(R\{x, y\}$和$R\{y, x\})$相对于$x$和$y$来说都是*等价关系*$S\{x, y\}$。令 $x'$、$y'$ 为不同于 R 中未出现的$x$、$y$ 的字母。则 $R\{x, y\}$ 与等价关系 $S\{x, x'\}$ *相容的*（相对于 $x$ 和 $y$） $S\{y, y'\}$；其他字（章II, § 6, no. 8）、关系

$$(R\{x, y\} \text{ and } S\{x, x'\} \text{ and } S\{y, y'\})$$

意味着$R\{x', y'\}$。

¶ A *预序关系在集合* E 上是预序关系 $R\{x, y\}$，使得关系 $R\{x, x\}$ 相当于 $x \in E$。 关系$R\{x, y\}$则意味着“$x \in E$和$y \in E$”。

¶ 如果$R\{x, y\}$在集合E上是预序关系，那么上面定义的关系$S\{x, y\}$就是E上的等价关系。让$R'\{X, Y\}$表示关系

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\exists x)(\exists y)(x \in X \text{ and } y \in Y \text{ and } R\{x, y\}),$$

也就是说，关系由R在经过上导出商（相对于$x$和$y$）；我们在章II, § 6, no. 3中看到，它相当于关系

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\forall x)(\forall y)((x \in X \text{ and } y \in Y) \Rightarrow R\{x, y\}).$$

¶ 让我们证明 $R'\{X, Y\}$ 是 E/S 的元素之间的 *序关系*。 关系 $(R'\{X, Y\}$ 和 $R'\{Y, Z\})$ 相当于

$$X \in E/S \text{ and } Y \in E/S \text{ and } Z \in E/S \text{ and }$$
$$(\forall x)(\forall y)(\forall z)((x \in X \text{ and } y \in Y \text{ and } z \in Z) \Rightarrow (R\{x, y\} \text{ and } R\{y, z\}))$$

（章I, § 4、判据C40、C41）。由于 $R\{x, y\}$ 是及物性的，并且 $Y \in E/S \Rightarrow Y \neq \emptyset$ (章 II, § 6, no. 2)，因此可以立即得出 $R'\{X, Y\}$ 是及物性的。接下来，$(R'\{X, Y\}$和$R'\{Y, X\})$相当于

$$X \in E/S \text{ and } Y \in E/S \text{ and }$$
$$(\forall x)(\forall y) \ ((x \in X \text{ and } y \in Y) \Rightarrow (R\{x, y\} \text{ and } R\{y, x\})),$$

因此相当于

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\forall x)(\forall y)((x \in X \text{ and } y \in Y) \Rightarrow S\{x, y\}),$$

因此意味着

$$X \in E/S \quad \text{and} \quad Y \in E/S \quad \text{and} \quad X = Y.$$

此外，$R\{x, y\}$意味着$R\{x, x\}$和$R\{y, y\}$，因此$R'\{X, Y\}$意味着关系中的每一个

$$X \in E/S \text{ and } (\forall x)((x \in X) \Rightarrow R\{x, x\}),$$
$$Y \in E/S \text{ and } (\forall y)((y \in Y) \Rightarrow R\{y, y\}),$$

从而$R'\{X, Y\}$意味着$(R'\{X, X\}$和$R'\{Y, Y\})$。最后，由于$x \in E$蕴含$R\{x, x\}$，$X \in E/S$蕴含$R'\{X, X\}$，断言的证明是完整的。据说$R'\{X, Y\}$与序关系*关联*于$R\{x, y\}$。

¶ 集合 E 上的 *预排序* 是对应 $\Gamma = (G, E, E)$，以 E 作为源和目标，并且 $(x, y) \in G$ 在 E 上是预序关系。通过滥用语言，我们将有时称为 $\Gamma$ 的图 G 作为 E 上的预排序。为此，有必要并且足以满足$\Delta \subset G$和$G \circ G \subset G$（这意味着$G \circ G = G$）。 等价关系 S 相应的到预序关系 $(x, y) \in G$ 则有 $G \cap \overset{-1}{G}$ 作为其图；与$(x, y) \in G$相关的序关系具有$(E/S) \times (E/S)$的图子集G'，其中对应（章II, § 6, no. 8）到像在$E \times E$的典范映射下

$$(E \times E)/(S \times S).$$

#### 例 {#ens-iii-s1-n2-exa-1 .statement tag=03JB}

\* 令 A 为环和单位元素。两个元素$x$之间的关系$(\exists z)(z \in \mathrm{A}$和$y = zx)$，A的$y$是A上的预序关系；它被读作“$x$是$y$的右除子”或“$y$是$x$的左倍数”。 \*

### 3. 记号与术语

截面其余部分给出的定义适用于$x$和$y$之间的任意序（或预序）关系$\mathrm{R}\{x, y\}$，但主要用于写有$\mathrm{R}\{x, y\}$的情况$x \leqslant y$ \*（与整数或实数之间通常的序关系类比）\*（或$x \subset y$，或通过一些类似的符号）；因此，我们将仅针对记号$x \leqslant y$陈述它们，并留给读者将它们转录成其他记号的任务。当$\mathrm{R}\{x, y\}$写成$x \leqslant y$时，$y \geqslant x$与$x \leqslant y$同义，这些关系读作“$x$*小于*$y$”，或“$x$*小于*$y$”，或“$y$*大于*$x$”或“$y$*大于*$x$”。 关系$x \geqslant y$则预序关系（*介于*$x$*和*$y$）*与*$x \leqslant y$相对。

由于语言滥用，我们经常会说“the 关系 $\leqslant$”而不是“the 关系 $x \leqslant y$”；在这种情况下，“关系$\geqslant$”与“关系$\leqslant$”相反。我们注还指出，在同一个证明中，在不存在混淆风险的情况下，我们可能经常使用相同的符号$\leqslant$来表示多个不同的序关系。

将关系的条件写成$x \leqslant y$在集合E上写成序关系如下：

(RO$_{\mathrm{I}}$) *关系“$x \leqslant y$和$y \leqslant z$”意味着$x \leqslant z$。*
(RO$_{\mathrm{II}}$) *关系“$x \leqslant y$和$y \leqslant x$”意味着$x = y$。*
(RO$_{\mathrm{III}}$) *关系 $x \leqslant y$ 意味着“$x \leqslant x$ 和 $y \leqslant y$”。*
(RO$_{\mathrm{IV}}$) *关系 $x \leqslant x$ 相当于 $x \in \mathrm{E}$.*

如果我们省略条件 (RO$_{\mathrm{II}}$)，我们在 E 上有条件，$x \leqslant y$ 为预序关系。
¶ 当序关系写为$x \leqslant y$时，我们将为关系写为$x < y$（或$y > x$）“$x \leqslant y$和$x \neq y$”；这些关系被读作“$x$*严格小于*$y$”，或“$x$*严格小于*小于$y$”，或“$y$*严格大于*$x$”，或“$y$*严格大于*” $x$”。

包含关系的例表明$x \leqslant y$的否定（用$x \nleqslant y$表示的有时）*不一定等于*$y < x$（cf.no. 12）。

C58。 *令$\leqslant$为序关系，并令$x$、$y$为两个不同的字母。 关系 $x \leqslant y$ 相当于“$x < y$ 或 $x = y$”。 关系“$x \leqslant y$和$y < z$”、“$x < y$和$y \leqslant z$”均意味着$x < z$。*

第一个断言源自标准$A \Rightarrow ((A$和（不是$B$））或$B$）（章I, § 3，标准C24）。为了证明第二个断言，我们注每个假设都蕴涵$x \leqslant z$，通过传递性；和关系（$x = z$和$x \leqslant y$和$y \leqslant z$）将意味着$x = y = z$，与假设相反。

¶ 在序中，为了让事情变得更容易，并通过数学定理来实现替换元数学判据，我们通常会考虑一个理论$\mathscr{T}$，其中包含公理和集合论的公理概形，并且加法，两个常数 E 和 $\Gamma$ 满足公理

“$\Gamma$ 是集合 E 上的订单”(no. 1)。

我们用$x \leqslant y$关系$y \in \Gamma\langle x \rangle$表示，我们可以说集合E*按顺序*$\Gamma$排序（或按序关系$y \in \Gamma\langle x \rangle$）（cf.章） IV, § 1）。

¶ 每当在 $\mathscr{T}$ 中，$\Gamma$ 是 E 上的预排序时，我们同样可以说 E 是由预排序* $\Gamma$ *预排序的。

在某些情况下（对于下面的定义中的例），我们要考虑的理论会稍微复杂一些。我们将让读者明确这些理论的常数和公理。

令 E、E$'$ 为按顺序 $\Gamma$、$\Gamma'$ 排序的两个集合。 * E *到* E$'$ 的 *同构（对于顺序 $\Gamma$ 和 $\Gamma'$）是 E 的双射 $f$ 到 E$'$，这样关系 $x \leqslant y$ 和 $f(x) \leqslant f(y)$ 是等价的（cf.章IV, § 1）。

### 4. 有序子集。 乘积有序集

设 E 是按排序 $\Gamma$ 排序的集合，有图 G。对于 E 的每个子集 A，$G \cap (A \times A)$ 是 A 上的排序； 相应的序关系相当于“$x \leqslant y$和$x \in A$和$y \in A$”，我们简单地用$x \leqslant y$来表示（滥用语言）。在 A 上定义的排序和序关系据说是由 E 上给出的排序和序关系 *诱导的； E 上的排序和序关系据说是 A 上排序的 *扩张* 和序关系，它们是诱导。 每当我们将 A 视为有序的集合时，我们都会想到由 E 上的除非在 A 上引发的排序，则明确指出了相反的情况。

*例*。由关系$X \subset Y$包含在子集的各种集合上引起的关系非常重要。这里有一些例：

#### 例 1 {#ens-iii-s1-n4-exa-1 .statement tag=03WB}

设E、F为两个集合，并令$\Phi(E, F)$为E到F中子集的所有映射中的集合。对于每个$f \in \Phi(E, F)$，令$G_f$为$f$的图，即子集 $E \times F$。如果我们在 $f$ 和 $g$ (no. 1, 例 3) 之间赋予 $\Phi(E, F)$ 序关系“*g 扩展 f*”，则 $f \to G_f$ 是有序的同构集合 $\Phi(E, F)$ 到 $\mathfrak{P}(E \times F)$ 的子集，按包含顺序排列。

#### 例 2 {#ens-iii-s1-n4-exa-2 .statement tag=03WC}

对于集合 E 的每个划分 $\varpi$，令 $\tilde{\varpi}$ 为由 $\varpi$ 在 E 上定义的等价关系的图。 映射 $\varpi \to \tilde{\varpi}$ 是集合的同构 E 的划分的 $\mathfrak{L}$，在 $\varpi$ 和 $\varpi'$ 之间按关系“$\varpi$ 更细 $\varpi'$”排序（no. 1、例 4）到子集 / $\mathfrak{P}(E \times E)$，按包含顺序排列。

#### 例 3 {#ens-iii-s1-n4-exa-3 .statement tag=03WD}

设 E 为集合，$\Omega \subset \mathfrak{P}(E \times E)$ 为 E 上*预购*图的集合（no. 2）（或者，滥用语言，E 上所有预购的集合）。 $s$和$t$之间的序关系$s \subset t$，在$\Omega$上由$\mathfrak{P}(E \times E)$上包含关系诱导，由说表示“$s$的预排序是*更细*” $t$”（或者“$t$比$s$*粗糙*”）。令$x(s)y$和$x(t)y$分别表示E上的预序关系、$(x, y) \in s$和$(x, y) \in t$；那么说 $s$ 比 $t$ 更细相当于说，关系 $x(s)y$ *暗示* $x(t)y$。

令$(E_\iota)_{\iota \in I}$为集合的族，对于每个指标$\iota \in I$，令$\Gamma_\iota$为$E_\iota$的排序；令$G_\iota \subset E_\iota \times E_\iota$为其图，令$x_\iota \leqslant y_\iota$表示序关系$(x_\iota, y_\iota) \in G_\iota$在$E_\iota$上。 乘积集合$F = \prod_{\iota \in I} E_\iota$、关系

$$(\forall \iota) \, ((\iota \in I) \Rightarrow (x_\iota \leqslant y_\iota))$$

经立即验证，序关系介于$x = (x_\iota)$和$y = (y_\iota)$之间。在 F 上如此定义的排序和序关系称为排序* $\Gamma_\iota$ 的 *乘积和序关系* $x_\iota \leqslant y_\iota$ 的 *乘积；这个关系写为$x \leqslant y$，而集合F，按$\Gamma_\iota$排序中的乘积排序，称为有序集*$E_\iota$的*乘积。

立即验证F上的乘积排序图是乘积集合$\prod_{\iota \in I} G_\iota$下$\prod_{\iota \in I} (E_\iota \times E_\iota)$的典范映射到$F \times F$（章II, § 5, no. 5）的像。

有序集的乘积的一个重要的例是集合 E 的映射图到有序集合 F 的集合 $F^E$。 $F^E$ 的规范双射到将 E 的映射的集合 $\mathfrak{F}(E, F)$ 转换为 F，而这个映射是有序的集合 $F^E$ 到 $\mathfrak{F}(E, F)$ 的同构，赋予由关系定义的排序“对于所有E的两个映射、$f$、$g$之间的$x \in E$、$f(x) \leqslant g(x)$”进入F。这个关系写成$f \leqslant g$。

☡

值得注意的是，在有序的集合 $\mathfrak{F}(E, F)$ 中，关系 $f < g$ 表示
$$\text{"for all } x \in E, f(x) \leqslant g(x), \text{ and there exists } y \in E \text{ such that } f(y) < g(y)\text{"}$$
*而不是*
$$\text{"for all } x \in E, f(x) < g(x)\text{"}.$$

在序中，为避免混淆，在这种情况下最好不要使用记号$f < g$。

当“订购”自始至终替换为“预订”时，此小节的定义无需变换就适用于预订的集合。

### 5. 单调递增映射

#### 定义 1 {#ens-iii-s1-def-1 .statement tag=03JC}

*让*E*和*F*被预先排序集合*（*预序关系，每个都用*$\leqslant$表示）。 *E *到* F *的映射 f *据说是递增*（或*顺序保留*）*如果关系*$x \leqslant y$*意味着*$f(x) \leqslant f(y)$； *它是递减*（或*顺序反转*）*如果关系*$x \leqslant y$*意味着*$f(x) \geqslant f(y)$。 * E *到* F *的*映射如果是递增或递减，则被认为是单调的。*

当我们通过相反的预排序对 E 或 F 上的替换 *一个*预排序时，E 到 F 的递增映射就变成递减（反之亦然）。  每个*常数*函数既是递增又是递减；这个叙述的逆命题通常是不正确的。

对于例，如果集合 E 按等式关系排序，则 E 本身的恒等映射既是递增又是递减，但如果 E 具有多个元素 (cf.)，则不是常数习题7)。

#### 定义 2 {#ens-iii-s1-def-2 .statement tag=03JD}

*设*E*和*F*为两个有序集。 * E *到* F *的映射 f *据说是严格递增的*（或*严格保序*）*如果关系* $x < y$ *意味着* $f(x) < f(y)$； *f 据说是严格递减*（或*严格顺序颠倒*）*如果关系* $x < y$ *意味着* $f(x) > f(y)$。 * E *的映射到* F *如果是严格递增的或严格递减，则被认为是严格单调的。*

*例*

#### 例 1 {#ens-iii-s1-n5-exa-1 .statement tag=03SK}

令 E 为集合。  $\mathfrak{P}(E)$（按包含排序）的映射$X \rightarrow E - X$自身为严格递减。

#### 例 2 {#ens-iii-s1-n5-exa-2 .statement tag=03SL}

令 E 为有序集合。对于每个$x \in E$，令$U_x$为所有$y \in E$中的集合，使得$y \geqslant x$。 映射 $x \to U_x$ 是 E 的严格递减映射进入$\mathfrak{P}(E)$（按包含排序）；事实上，关系$x \leqslant y$相当于$U_x \supset U_y$。

有序集合 E 到有序集合 F 的单射单调映射 *严格单调*； 逆命题通常不为真，因为当关系、$x \leqslant y$、$x \geqslant y$都不为真时，可能会出现$f(x) = f(y)$（cf.no. 12、命题11）。

¶ 有序集合 E 到有序集合 E' 的双射映射 $f$ 是 E 到 E' (no. 3) 的同构，当且仅当 $f$ 及其逆映射均为递增。

¶ 如果 I 是 *有序* 指标集合，则集合 E 的子集* $(X_\iota)_{\iota \in I}$ 的 * 族被称为 *递增* 如果 $\iota \to X_\iota$ 是递增映射 I 进入$\mathfrak{P}(E)$，按包含顺序排列（在其他字中，如果 $\iota \leqslant \varkappa$ 暗示$X_\iota \subset X_\varkappa$）。同样，我们定义是子集$(X_\iota)_{\iota \in I}$的*递减、严格递增的、*或*严格递减*家族。

#### 命题 2 {#ens-iii-s1-prop-2 .statement tag=03JE}

*让* E，E' *为两个有序集，并让*$u : E \to E'$*和*$v : E' \to E$*为两个递减映射，这样对于所有*$x \in E$*和所有*$x' \in E'$*我们有*$v(u(x)) \geqslant x$*和*$u(v(x')) \geqslant x'$。 *然后*

$$u \circ v \circ u = u \quad \textit{and} \quad v \circ u \circ v = v.$$

对于关系，$v(u(x)) \geqslant x$意味着$(u(v(u(x))) \leqslant u(x)$，因为$u$是递减；另一方面，我们在不等式$u(v(x')) \geqslant x'$中有$u(v(u(x))) \geqslant u(x)$乘替换$x'$乘$u(x)$。因此第一个等式；第二个证明类似。

### 6. 最大和最小元素

#### 定义 3 {#ens-iii-s1-def-3 .statement tag=03JF}

*令* E *为有序集合。 元素* $a \in E$ *据说是* E 的最小*（或*最大*）*元素 *如果关系* $x \leqslant a$（或$x \geqslant a$）*意味着* $x = a$。

E 的每个最小元素相对于相反的顺序都是极大元素，反之亦然。

*例*

#### 例 1 {#ens-iii-s1-n6-exa-1 .statement tag=03SM}

设 A 为集合。在A的非空子集的$\mathfrak{P}(A)$（按包含排序）由……组成的子集中，最小元素是单个元素的子集由……组成。

#### 例 2 {#ens-iii-s1-n6-exa-2 .statement tag=03SN}

E 的子集映射集合 $\Phi(E, F)$ 到 F 中（F 非空），在 $u$ 和 $v$ 之间按关系“$v$ 扩展 $u$”排序， 极大元素是整个 E 到 F 的映射。

#### 例 3 {#ens-iii-s1-n6-exa-3 .statement tag=03SO}

\* 在自然整数 $> 1$的集合中，在$m$和$n$之间按关系“$m$除$n$”排序，最小的元素是素数数。 \*

#### 例 4 {#ens-iii-s1-n6-exa-4 .statement tag=03SP}

\* 实数中的集合没有极大元素也没有最小元素。 \*

### 7. 最大元素至少元素

如果有序集合 E 中存在元素 $a$，使得所有 $x \in E$ 都有 $a \leqslant x$，则 $a$ 是 E 中*唯一*具有该性质的元素；因为如果对于所有$x \in E$也有$b \leqslant x$，那么我们应该有$a \leqslant b$和$b \leqslant a$，因此还有$a = b$。

#### 定义 4 {#ens-iii-s1-def-4 .statement tag=03JG}

*令* E *为有序集合。 元素* $a \in E$ *据说是* E 中*最小（分别为 *最大的*）*元素 *如果对于所有* $x \in E$ *我们有* $a \leqslant x$（分别为 $x \leqslant a$）。

有序的集合不需要有最大元素，也不需要至少有元素。如果 E 至少具有元素 $a$，则相对于相反顺序，$a$ 是最大元素。

¶ 如果 E 具有至少元素 $a$，则 $a$ 是 E 的*唯一最小值元素*；因为如果 $x \in E$ 与 $a$ 不同，我们就有 $a < x$。

*例*

#### 例 1 {#ens-iii-s1-n7-exa-1 .statement tag=03SQ}

令 $\mathfrak{S}$ 为集合 E 的子集的集合 $\mathfrak{P}(E)$ 的非空子集。 如果$\mathfrak{S}$相对于包含关系有至少（或最大的）元素 A，则A是$\mathfrak{S}$的集合的交（或并）。 相反，如果$\mathfrak{S}$属于的集合的交（或并）到$\mathfrak{S}$，则它是$\mathfrak{S}$的最小（或最大的）元素。

#### 例 2 {#ens-iii-s1-n7-exa-2 .statement tag=03SR}

特别地，$\emptyset$是$\mathfrak{P}(E)$的最小元素和E最大元素。 E入F的子集映射集合$\Phi(E, F)$中，按映射扩张(no. 1，例3)排序，空的映射最少元素，且无最大元素除非 F 由单个元素组成。 $E \times E$的对角线$\Delta$是E上等价关系图（或E上预序的集合）的集合的最小元素。

#### 命题 3 {#ens-iii-s1-prop-3 .statement tag=03JH}

*设* E *是一个有序的集合，并让* E$'$ *是* E *和单个元素的不相交的并和集合*$\{a\}$*由……组成。那么在 * E$'$ * 上存在唯一的排序，其中诱导在 * E * 上给定的排序，并且 * $a$ * 是 * E$'$ 的最大元素。

因为如果 G 是 E 上的排序图，则满足命题的条件的 E$'$ 上的排序图必须是 G 的并 G$'$ 和所有对 $(x, a)$ 的集合，其中 $x \in E'$；相反，很明显G$'$是满足给定条件的E$'$的排序图。

¶ 有序的集合 E$'$ 据说是通过*邻接最大元素* $a$ *到* E (cf. 习题 3) 获得的。

¶ 预定的集合 $E$ 的子集 $A$ 被认为是 $E$ 中的 *cofinal*（或 *coinitial*），如果对于每个 $x\in E$ 都存在 $y\in A$，使得 $x\leq y$（或 $y\leq x$）。因此，如果说有序集合 $E$ 具有最大的（或至少）元素，则意味着 $E$ 具有单个元素的共尾（或共初始）子集由……组成。

### 8. UPPER AND LOWER BOUNDS

#### 定义 5 {#ens-iii-s1-def-5 .statement tag=03JI}

*令$E$为预定的集合，令$X$为$E$的子集。任何元素$x\in E$使得所有$y\in X$的$x\leq y$（或$x\geq y$）被称为$E$中$X$的下界（或上界）。*

就相反顺序而言，$X$ 的每个上界都是 $X$ 的下界，反之亦然。

¶ 如果$x$是$X$的下界，则每个元素$z\leq x$也是$X$的下界。 $X$的下界也是$X$的每子集的下界。当且仅当存在 $X$ 中的下界（其中属于到 $X$）时，有序集合 $X$ 具有至少元素。

¶ The set of lower bounds of a subset $X$ of a preordered set $E$ may be empty : this is the case when $X=E$ and $E$ is an ordered set which has no least element.

¶ $E$ 的子集 $X$，其下界（或上界）的集合不为空，则称为 *下界*（或 *上界*）。上下都有界的子集被称为*有界*。如果 $X$ 有界于下（或有界于上，有界），则对于 $X$ 的每个子集也是如此。

单个元素的每个子集由……组成都是有界的。但是两个元素中的子集由……组成不需要在上方或下方 (no. 10) 上界。

令$E$为预定的集合，并让$f$为任意集合$A$到$E$的映射。如果集合 $f(A)$ 在 $E$ 中被限制在下方（或限制在上方，有界），则映射 $f$ 被称为（滥用语言）为*下界*（分别为*上界、有界*）。

### 9. 至少上界和下确界

#### 定义 6 {#ens-iii-s1-def-6 .statement tag=03JJ}

*令$E$为有序的集合，并令$X$为$E$的子集。 $E$的元素被称为下确界或$E$中$X$的下确界（分别为至少上界或上确界），如果它是下限的集合的最大的（或至少）元素 $E$ 中$X$（或上限）的边界。*

给定有序集合$E$的子集$X$，$E$中$X$的最小上界（或下确界）（当存在时）表示为

$$
\sup_E X\quad\text{(resp. }\inf_E X\text{)}
$$

或者通过sup X（或inf X）（如果没有歧义的风险）。两个元素中集合 $\{x, y\}$ 中最小的上界（或下确界），当存在时，用 SU $(x, y)$（或 inf $(x, y)$）表示。同样，对于三个元素中集合中最小的上界和下确界，等等。

¶ 如果 E 的子集 X 有最大元素 $a$，则 $a$ 是 E 中 X 中最小的上界。

¶ 如果 X 在 E 中具有下确界 $a$，则相对于 E 上的相反顺序，$a$ 是 X 中最小的上界。因此，我们可以将自己限制为最大部分，在下文中，考虑最小的属性上界。

*例*

(1)有序集合E中空集$\emptyset$的上界集合显然是E本身；因此，当且仅当 E 具有*最小* 元素（即 $\emptyset$ 的*最小*上界*）时，$\emptyset$ 在 E 中具有上界。

(2) 在集合 E 的子集集合 $\mathfrak{P}(E)$ 中，按包含排序，$\mathfrak{P}(E)$ 的每一个子集 $\mathfrak{S}$ 至少有上界，即 *并* $\mathfrak{S}$的集合，以及下确界，即$\mathfrak{S}$的集合*交*。

(3) 设E、F为两个集合，设$\Theta$为E入F的子集映射$\Phi(E, F)$的子集，按映射扩张排序(no. 1， 例3）。对于每个$u \in \Phi(E, F)$，让$D(u)$作为$u$的域。 条件对于映射属于到 $\Phi(E, F)$ 的家庭中存在公共的扩张 (章 II, § 4, no. 6, 命题 7) 表明 $\Theta$ 至少有$\Phi(E, F)$中的上界当且仅当对于$\Theta$的元素中的每个对$(u, v)$，只要$x \in D(u) \cap D(v)$，我们就有$u(x) = v(x)$。

如果像 $f(A)$ 在 E 中具有至少上界，则将集合 A 的映射 $f$ 转换为有序的集合 E，则称其至少具有上界；这个界限被称为 f* 的*最小上界并写作 $\sup_{x \in A} f(x)$。对于下确界也是如此。

特别地，如果 E 的子集 A 在 E 中具有至少上界，则该界限是 A 的典范嵌入到 E 中的最小上界，因此可以写为 $\sup_{x \in A} x$。

#### 命题 4 {#ens-iii-s1-prop-4 .statement tag=03JK}

*设* E *为有序集合，并令* A *为* E *的子集，其中* E *中既有下确界，且至少有上界。 *则* $\inf A \leqslant \sup A$ *如果* $A \neq \emptyset$； *如果* $A = \emptyset$, $\sup A$ *是* E 的最小且* $\inf A$ *最大元素。

这紧随定义而来。

#### 命题 5 {#ens-iii-s1-prop-5 .statement tag=03JL}

*令* E *为有序集合，并让* A、B *为* E 中的两个子集，*其中每个在* E 中至少有上界*（分别为*下确界*）。*如果* $A \subset B$，*则*$\sup A \leqslant \sup B$（分别为$\inf A \geqslant \inf B$）。

#### 推论{#ens-iii-s1-n9-cor-1 .statement tag=03JM}

*设$(x_\iota)_{\iota \in I}$是有序集合*$\mathrm{E}$的元素族，其中*$\mathrm{E}$中至少有上界。 *如果*$\mathrm{J}$*是*$\mathrm{I}$*的子集*使得家庭*$(x_\iota)_{\iota \in J}$*在*$\mathrm{E}$中至少有上界，*我们有*$\sup\limits_{\iota \in J} x_\iota \leqslant \sup\limits_{\iota \in I} x_\iota$。

#### 命题 6 {#ens-iii-s1-prop-6 .statement tag=03JN}

*让*$(x_\iota)_{\iota \in I}$，$(y_\iota)_{\iota \in I}$*成为有序集合*$\mathrm{E}$的元素的两个族，*由相同的集合*$\mathrm{I}$索引，*并且使得*$x_\iota \leqslant y_\iota$*对于所有*$\iota \in \mathrm{I}$。 *如果两个家庭在* $\mathrm{E}$ 中至少有上界，*则* $\sup\limits_{\iota \in I} x_\iota \leqslant \sup\limits_{\iota \in I} y_\iota$。

对于 $a = \sup\limits_{\iota \in I} y_\iota$ 来说，上界是 $y_\iota$ 的集合，因此 $x_\iota \leqslant y_\iota \leqslant a$ 对于所有 $\iota \in \mathrm{I}$，因此是 $\sup\limits_{\iota \in I} x_\iota \leqslant a$。

#### 命题 7 {#ens-iii-s1-prop-7 .statement tag=03JO}

*让*$(x_\iota)_{\iota \in I}$*成为有序集合*$\mathrm{E}$的元素族，*并让*$(\mathrm{J}_\lambda)_{\lambda \in L}$*成为指标集合*$\mathrm{I}$的覆盖。 *假设每个亚族*$(x_\iota)_{\iota \in J_\lambda}$*在*$\mathrm{E}$中至少有上界。 *对于家庭* $(x_\iota)_{\iota \in I}$ *在* $\mathrm{E}$中至少拥有上界，*家庭* $\left( \sup\limits_{\iota \in J_\lambda} x_\iota \right)_{\lambda \in L}$ *在* $\mathrm{E}$中至少拥有上界是必要且充分的，*然后我们有*

$$(1) \qquad \sup_{\iota \in I} x_\iota = \sup_{\lambda \in L} \left( \sup_{\iota \in J_\lambda} x_\iota \right).$$

让$b_\lambda = \sup\limits_{\iota \in J_\lambda} x_\iota$。假设 $(x_\iota)_{\iota \in I}$ 至少有上界 $a$。然后每个$\lambda \in \mathrm{L}$对应$a \geqslant b_\lambda$（推论命题5）。另一方面，如果每个$\lambda \in \mathrm{L}$都有$c \geqslant b_\lambda$，那么每个$\iota \in \mathrm{I}$就有$c \geqslant x_\iota$，因为$(\mathrm{J}_\lambda)_{\lambda \in L}$是$\mathrm{I}$的覆盖；因此$c \geqslant a$，这证明了

$$a = \sup_{\lambda \in L} b_\lambda.$$

相反，假设家庭$(b_\lambda)_{\lambda \in L}$至少有上界$a'$。然后 $a' \geqslant x_\iota$ 对于所有 $\iota \in \mathrm{I}$。另一方面，如果 $c' \geqslant x_\iota$ 对于所有 $\iota \in \mathrm{I}$，那么我们特别有

$$c' \geqslant \sup_{\iota \in J_\lambda} x_\iota = b_\lambda$$

对于每个 $\lambda \in \mathrm{L}$，因此 $c' \geqslant a'$ 因此

$$a' = \sup_{\iota \in I} x_\iota.$$

#### 推论{#ens-iii-s1-n9-cor-2 .statement tag=03JP}

*让*$(x_{\lambda\mu})_{(\lambda,\ \mu) \in L \times M}$*成为有序集合*$\mathrm{E}$*的元素的“双”家族，使得对于每个*$\mu \in \mathrm{M}$*家族*$(x_{\lambda\mu})_{\lambda \in L}$*在*$\mathrm{E}$中至少有上界。 *对于家庭* $(x_{\lambda\mu})_{(\lambda,\ \mu) \in L \times M}$ *在* $\mathrm{E}$ 中至少拥有上界，*家庭* $\left( \sup\limits_{\lambda \in L} x_{\lambda\mu} \right)_{\mu \in M}$ *在* E 中至少拥有* *上界是充分必要的，*然后我们有*

$$(2) \qquad \sup_{(\lambda,\,\mu)\in L\times M} x_{\lambda\mu} = \sup_{\mu\in M}\left(\sup_{\lambda\in L} x_{\lambda\mu}\right).$$

#### 命题 8 {#ens-iii-s1-prop-8 .statement tag=03QI}

*让*$(E_\iota)_{\iota\in I}$*成为有序集的一家人。令* A *为乘积的子集排序集合* $E = \prod_{\iota\in I} E_\iota$，*并令* $A_\iota = \mathrm{pr}_\iota A$ *对于每个* $\iota \in I$。 *对于* A *在* E 中至少有上界 *对于每个* $\iota \in I$、$A_\iota$ *在* $E_\iota$ 中应该至少有上界，这是必要且充分的，*然后我们有*

$$\sup A = (\sup A_\iota)_{\iota\in I} = \left(\sup_{x\in A} \mathrm{pr}_\iota x\right)_{\iota\in I}.$$

假设对于每个 $\iota \in I$，$A_\iota$ 在 $E_\iota$ 中至少有上界 $b_\iota$。如果说 $c = (c_\iota)$ 是 A 的上界，则意味着对于每个 $\iota \in I$ 都有 $c_\iota \geqslant b_\iota$，因而 $(b_\iota)_{\iota\in I}$ 是 A 的上界。反之，假设 A 至少有上界 $a = (a_\iota)_{\iota\in I}$；对于每个$\varkappa \in I$，$a_\varkappa$是$A_\varkappa$的上界，因为如果$x_\varkappa \in A_\varkappa$，则存在$x \in A$使得$\mathrm{pr}_\varkappa x = x_\varkappa$乘以$A_\varkappa$的定义；另一方面，如果$a'_\varkappa$是$E_\varkappa$中$A_\varkappa$的上界，则元素$c' = (c'_\iota)_{\iota\in I}$，其中

$$c'_\iota = a_\iota \quad \text{for} \quad \iota \neq \varkappa \qquad \text{and} \qquad c'_\varkappa = a'_\varkappa$$

是 A 的上界；因而$c' \geqslant a$，因而$a'_\varkappa \geqslant a_\varkappa$；因而$a_\varkappa$是$E_\varkappa$中$A_\varkappa$的最小上界。

☡

¶ 设 F 为有序集合 E 的子集，并设 A 为 F 的子集。可能会出现两个元素 $\sup_E A$、$\sup_F A$ 之一存在而另一个不存在，或者两者都存在但不相等的情况。

*例*

#### 例 1 {#ens-iii-s1-n9-exa-1 .statement tag=03SS}

\* 在实数的有序集合$E = \mathbf{R}$中，考虑有理数的子集$F = \mathbf{Q}$和有理数$< \sqrt{2}$的集合$A \subset F$； $\sup_E A$存在，但$\sup_F A$不存在。

#### 例 2 {#ens-iii-s1-n9-exa-2 .statement tag=03ST}

在例 1 的记号中，令G为A的并且集合$\{2\}$；那么$G \subset F$和$\sup_G A$存在，但$\sup_F A$不存在。

#### 例 3 {#ens-iii-s1-n9-exa-3 .statement tag=03SU}

与记号、$\sup_E A = \sqrt{2}$、$\sup_G A = 2$相同。 \*

但是，我们得到以下结果：

#### 命题 9 {#ens-iii-s1-prop-9 .statement tag=03QJ}

*设*E*为*E的有序集合，*F*子集，*F的A*子集。 *如果*$\sup_E A$*和*$\sup_F A$*都存在，我们有*$\sup_E A \leqslant \sup_F A$。 *如果*$\sup_E A$*存在并且属于到*F，*则*$\sup_F A$*存在并且等于*$\sup_E A$。

第一个断言源自以下事实：F中A的上界的集合$\mathrm{M}$包含在E中A的上界的集合N中，并且来自命题5。另一方面，如果N的最小元素位于F中，那么它属于到M显然是 M 中最小的元素；这就证明了第二个断言。

### 10. DIRECTED SETS

#### 定义 7 {#ens-iii-s1-def-7 .statement tag=03QK}

*预先排序的集合* E *被认为是右向*（或*左向*）*如果* E 的两个元素中的每一个子集都位于上方*（相应地*位于下方*）。

代替“右向”，我们经常使用“相对于关系$\leqslant$定向”的表达方式，以及当预序关系由其他符号表示时的类似表达方式。对于例，如果$\mathfrak{S}$是集合A的子集的集合，我们说$\mathfrak{S}$是*有向于关系*$\subset$（或$\supset$）如果，对于每个子集 $\mathfrak{S}$的两个元素中的$\{\mathrm{X}, \mathrm{Y}\}$由……组成，存在$\mathrm{Z} \in \mathfrak{S}$使得$\mathrm{X} \subset \mathrm{Z}$和$\mathrm{Y} \subset \mathrm{Z}$（分别为$\mathrm{X} \supset \mathrm{Z}$和$\mathrm{Y} \supset \mathrm{Z}$）。

*例*
(1) 具有最大元素的有序集合是右向的。
\* (2) 在拓扑空间中，点的邻域的基本系统相对于关系$\supset$有向。
(3)任意模的有限型、子模、集合相对于关系$\subset$有向。 \*

#### 命题 10 {#ens-iii-s1-prop-10 .statement tag=03QL}

*在右向有序集合* E 中，*极大元素 a 是* E 的最大元素。

对于每个$x \in \mathrm{E}$，存在假设$y \in \mathrm{E}$，使得$x \leqslant y$和$a \leqslant y$；因为 $a$ 是最大的，$y = a$。

¶ 右向预排序集合相对于相反的排序是左向的。右有向集合的任何乘积都是右向的。另一方面，右有向集合的子集不一定是右向的。然而，右有向集合 E 的 *cofinal* 子集 F 始终是右向的；对于给定的$x$，$y \in \mathrm{F}$，存在$z \in \mathrm{E}$使得$x \leqslant z$和$y \leqslant z$，然后存在$t \in \mathrm{F}$使得$z \leqslant t$。

### 11. 格子

#### 定义 8 {#ens-iii-s1-def-8 .statement tag=03QM}

*有序集合* E *如果* E 的两个元素中的每一个子集由……组成在* E 中至少有上界和下确界，则称其为格子。

每乘积个格子都是一个格子；这是从条件得出的，因为有序集（no. 9，命题8）中的乘积中至少存在上界。 集合 A 的子集集合按包含排序，是一个格，因为 A 的两个子集的并和交又是 A 的子集。

*例*

#### 例 1 {#ens-iii-s1-n11-exa-1 .statement tag=03SV}

\* 整数 $\geqslant 1$的集合，在$m$和$n$之间按关系“$m$除$n$”排序，是一个格； $\{m,n\}$ 中最小的上界是 l.c.m。 $m$ 和 $n$，下确界是他们的 h.c.f.

#### 例 2 {#ens-iii-s1-n11-exa-2 .statement tag=03TT}

群 G 的子群集合按包含排序，是一个格子。

#### 例 3 {#ens-iii-s1-n11-exa-3 .statement tag=03TU}

集合 A 上的拓扑集合，在$\mathscr{T}$和$\mathscr{T}'$之间按关系“$\mathscr{T}$比$\mathscr{T}'$粗”排序，是一个格。 （*一般拓扑*、章I, § 2）。

#### 例 4 {#ens-iii-s1-n11-exa-4 .statement tag=03TV}

在$\mathbf{R}$的区间I上定义的所有实值函数的集合$\mathfrak{F}(I,\mathbf{R})$是关于序关系$f\leqslant g$（no. 4）的格，因此与乘积$\mathbf{R}^{I}$同构的。 \*

#### 注 {#ens-iii-s1-n11-rem-1 .statement tag=03JQ}

格子显然是左向和右向的。但同时向左和向右的有序集合不一定是格子。 \* 后者的例是$\mathbf{R}$的映射$x\mapsto p(x)$的集合自身，其中$p$是$\mathbf{R}[X]$的多项式，这个集合按关系$p\leqslant q$（no. 4）排序。 \*

### 12. TOTALLY ORDERED SETS

#### 定义 9 {#ens-iii-s1-def-9 .statement tag=03JR}

*如果关系“$x\leqslant y$ 或 $y\leqslant x$”为真，则预定的集合 E 的两个元素 $x$、$y$ 被认为是可比较的。如果集合 E 是有序的并且E 的任何两个元素是可比较的，则称E 是完全有序的。 E 上的排序称为全排序，相应的序关系总计序关系。*

如果$x$和$y$是全序集的元素，则$x=y$或$x<y$或$x>y$；因此$x\leqslant y$的否定是$x>y$。

E 上的排序是全排序当且仅当其图 G 满足关系 $G\cup\overset{-1}{G}=E\times E$，以及关系 $G\circ G=G$ 和 $G\cap\overset{-1}{G}=\Delta$。

*例*

#### 例 1 {#ens-iii-s1-n12-exa-1 .statement tag=03SW}

全序集的每个子集都通过归纳排序完全排序。

#### 例 2 {#ens-iii-s1-n12-exa-2 .statement tag=03TW}

令 E 为任意有序的集合。 E 的空子集是全序的，单个元素的 E 由……组成的每个子集也是全序的。

#### 例 3 {#ens-iii-s1-n12-exa-3 .statement tag=03TX}

\* 实数的集合 $\mathbf{R}$ 是完全有序的。 \*

#### 例 4 {#ens-iii-s1-n12-exa-4 .statement tag=03TY}

如果 A 是集合，并且至少有两个不同的元素，则集合 $\mathfrak{P}(A)$（按包含排序）不是全序的，因为如果 $x\neq y$、子集 $\{x\}$ 和 $\{y\}$ 不可比较。

全序集相对于相反的顺序也是全序的；它是一个格子并且 *更不必说* 向左和向右。

#### 命题 11 {#ens-iii-s1-prop-11 .statement tag=03JS}

* 全序集* E * 的每个严格单调映射 $f$ 到有序集合* F * 都是单射的。如果$f$是严格递增的，则$f$是* E *到$f(\mathrm{E})$*的同构。

对于$x \neq y$意味着$x < y$或$x > y$；因此

$$f(x) < f(y) \qquad \text{or} \qquad f(x) > f(y),$$

所以无论哪种情况都是$f(x) \neq f(y)$。尚待证明，如果$f$是严格递增的，则$f(x) \leqslant f(y)$蕴含$x \leqslant y$；如果没有，我们应该有$x > y$，因此$f(x) > f(y)$。

#### 命题 12 {#ens-iii-s1-prop-12 .statement tag=03JT}

*设* E *为全序集并让* X *为* E 的子集。 *对于* E 的元素 $b$ *为* E 中* X *的最小上界，*必要且充分的是* (1) *$b$ 是* X的上界，(2) *对于每个$c \in \mathrm{E}$使得$c < b$，存在$x \in \mathrm{X}$使得$c < x \leqslant b$。*

The second condition says that no element $c < b$ is an upper bound of X, i.e., $b$ is a minimal element of the set M of upper bounds of X; but this is the same as saying that $b$ is the least element of M, since M is totally ordered (no. 10, Proposition 10).

### 13. 间隔

令 E 为有序集合，并令 $a$、$b$ 为 E 的两个元素，使得 $a \leqslant b$。 元素 $x$ 的 E 由……组成的子集使得 $a \leqslant x \leqslant b$ 称为*左端点 a 和右端点 b* 的闭区间，并用 $[a, b]$ 表示。所有$x \in \mathrm{E}$中的集合，使得$a \leqslant x < b$（或$a < x \leqslant b$）被称为*右侧半开区间*（或*左侧*），端点为$a$和$b$，并由$[a, b[$（或$]a, b]$）表示。所有$x \in \mathrm{E}$的集合，使得$a < x < b$称为“开区间”，端点为$a$和$b$，并用$]a, b[$表示。

注闭区间永远不会为空；间隔$[a, a]$为集合$\{a\}$。另一方面，区间$[a, a[$、$]a, a]$、$]a, a[$都是空的；即使当 $a < b$ 时，开区间 $]a, b[$ 也可能为空。

令$a$为E的元素。所有$x \in \mathrm{E}$的集合，使得$x \leqslant a$（分别为$x < a$）被称为*闭合*（分别为*开*）*区间在左侧无界，右侧端点为a*，并由$]{\leftarrow}, a]$（分别为*开*）表示。 $]{\leftarrow}, a[$);同样，所有$x \in \mathrm{E}$中的集合，使得$x \geqslant a$（分别为$x > a$）被称为*闭合*（分别为*开*）*与左端点a的间隔，在右侧无界*，并由$[a, {\rightarrow}[$（分别为$]a, {\rightarrow}[$）表示。最后，E本身可以被视为*左右无界的开区间*，用$]\leftarrow, \rightarrow[$表示。

#### 命题 13 {#ens-iii-s1-prop-13 .statement tag=03JU}

*在格中，两个区间的交是一个区间。*考虑两个闭区间$[a, b]$和$[c, d]$的例交，并令$\alpha = \sup (a, c)$，$\beta = \inf (b, d)$。如果同时有$a \leqslant x \leqslant b$和$c \leqslant x \leqslant d$，则有$\alpha \leqslant x \leqslant \beta$，反之亦然；如果$[a, b]$和$[c, d]$中的$\alpha \not\leqslant \beta$、交为空；如果$\alpha \leqslant \beta$，这个交就是$[\alpha, \beta]$。对于其他情况，我们让读者自行完成证明。

### 习题 {#ens-iii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
