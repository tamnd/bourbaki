---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 6
section_title: Equivalence relations
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 112-122, 127-129
pdf_pages: 0119-0129, 0134-0136
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN EQUIVALENCE RELATION
      page: 113
      pdf_page: 120
    - "no": 2
      title: EQUIVALENCE CLASSES ; QUOTIENT SET
      page: 114
      pdf_page: 121
    - "no": 3
      title: RELATIONS COMPATIBLE WITH AN EQUIVALENCE RELATION
      page: 116
      pdf_page: 123
    - "no": 4
      title: SATURATED SUBSETS
      page: 117
      pdf_page: 124
    - "no": 5
      title: MAPPINGS COMPATIBLE WITH EQUIVALENCE RELATIONS
      page: 118
      pdf_page: 125
    - "no": 6
      title: INVERSE IMAGE OF AN EQUIVALENCE RELATION; INDUCED EQUIVALENCE RELATION
      page: 119
      pdf_page: 126
    - "no": 7
      title: QUOTIENTS OF EQUIVALENCE RELATIONS
      page: 119
      pdf_page: 126
    - "no": 8
      title: PRODUCT OF TWO EQUIVALENCE RELATIONS
      page: 120
      pdf_page: 127
    - "no": 9
      title: CLASSES OF EQUIVALENT OBJECTS
      page: 121
      pdf_page: 128
statements: 13
exercises: 11
content_sha256: b920f9bf2237025d477ddc85ddc545c97b7a1d158bc6d2359c68da01657a7adb
translated_from: content/en/ens/II/06_s6_equivalence_relations.md
translation_method: google
source_content_sha256: f7ce72a4dfc4c2df0edb07393e9d9b7234a3b676d35f6cff417c9f89092d2c5a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 5aa504a9a978f5da40c807066b637df9edf5587d8e59527279be4dd80925b35a
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 6. 等价关系

在原理中，今后不再使用粗体斜体字母来表示未确定的组合；读者将能够从上下文中轻松辨别断言适用于未确定的字母或关系。

### 1. 定义等价关系

令$R\{x, y\}$为关系，$x$和$y$是不同的字母。 关系 $R$ 被认为是*对称*（相对于字母 $x$ 和 $y$）如果

$$R\{x, y\} \Rightarrow R\{y, x\}.$$

如果是这样，用两个字母$x'$和$y'$代替$x$和$y$，这两个字母彼此不同，并且与$R$中出现的所有字母不同，然后用$y$和$x$代替$x'$和$y'$，分别，我们看到

$$R\{y, x\} \Rightarrow R\{x, y\}.$$

因此$R\{x, y\}$和$R\{y, x\}$是等价的。

¶ 令$z$ 为$R$ 中未出现的字母。 关系 $R$ 被认为是*及物*（相对于字母 $x, y$）如果我们有

$$(R\{x, y\} \text{ and } R\{y, z\}) \Rightarrow R\{x, z\}.$$

#### 例 {#ens-ii-s6-n1-exa-7 .statement tag=077S}

关系 $x = y$ 是对称且传递的。 关系 $X \subset Y$ 是传递性的，但不对称。 关系 $X \cap Y = \emptyset$ 对称但不传递。

如果 $R\{x, y\}$ 既对称又传递，则称为 *等价关系* （相对于字母 $x$ 和 $y$）。在这种情况下，记号$x \equiv y \pmod{R}$是有时用作$R\{x, y\}$的同义词；它被读作“*x 等于 y modulo* $R$”。如果$R$是等价关系，我们有$R\{x, y\} \Rightarrow (R\{x, x\}$和$R\{y, y\})$，因为$R\{x, y\}$隐含$R\{y, x\}$，而$(R\{x, y\}$和$R\{y, x\})$凭借定义隐含$(R\{x, x\}$和$R\{y, y\})$。

¶ 令 $R\{x, y\}$ 为关系；如果关系 $R\{x, x\}$ 等于 $x \in E$，则可以说它是*$E$（相对于字母$x, y$）的自反。如果$E$没有任何可能的歧义，人们可以滥用语言简单地说$R$是反身的。

¶ * $E$ 上的 *等价关系被定义为等价关系，它在 $E$ 上自反。如果$R\{x, y\}$是$E$上的等价关系，我们有$R\{x, y\} \Rightarrow ((x, y) \in E \times E)$，因而$R$有一个图（相对于字母$x, y$）。相反，假设等价关系 $R\{x, y\}$ 有一个图 $G$。观察关系$R\{x, x\}$相当于关系$(\exists y)R\{x, y\}$；因为前者意味着后者（章 I, § 4, no. 2、概形 S5），反之，由于$R\{x, y\}$意味着$R\{x, x\}$，$(\exists y) R\{x, y\}$意味着$(\exists y) R\{x, x\}$，因此也意味着$R\{x, x\}$。因而 $R\{x, x\}$ 等价于 $x \in \mathrm{pr}_1 G$，因而 $R$ 在 $\mathrm{pr}_1 G$ 上是等价关系。

¶ 集合 E 上的 *等价* 是对应，其源和目标都等于 E，并且其图 F 使得关系 $(x, y) \in F$ 是 E 上的等价关系。

*例*

#### 例 1 {#ens-ii-s6-n1-exa-1 .statement tag=03IX}

关系 $x = y$ 是等价关系，它没有图表，因为如果有的话，该图表的第一个投影将是所有对象中的集合。

#### 例 2 {#ens-ii-s6-n1-exa-2 .statement tag=03SC}

关系“$x = y$和$x \in E$”是E上的等价关系，其图形是$E \times E$的对角线。

#### 例 3 {#ens-ii-s6-n1-exa-3 .statement tag=03TQ}

关系“Y 上存在X的双射”是等价关系，它没有图（cf.章III, § 3）。

#### 例 4 {#ens-ii-s6-n1-exa-4 .statement tag=03TR}

关系“$x \in E$和$y \in E$”是E上的等价关系，其图为$E \times E$。

#### 例 5 {#ens-ii-s6-n1-exa-5 .statement tag=03TS}

假设$A \subset E$；然后关系

$$(x \in E - A \text{ and } y = x) \text{ or } (x \in A \text{ and } y \in A)$$

是 E 上的等价关系。

#### 例 6 {#ens-ii-s6-n1-exa-6 .statement tag=03TP}

\* 关系“$x \in \mathbf{Z}$和$y \in \mathbf{Z}$和$x - y$能被4整除”是等价关系在$\mathbf{Z}$上。\*

#### 命题 1 {#ens-ii-s6-prop-1 .statement tag=03QH}

*对应* $\Gamma$ *在* X *和* X *之间等价在* X *当且仅当它满足以下条件 :* (a) X *是的域* $\Gamma$； (b) $\Gamma = \overset{-1}{\Gamma}$； (c) $\Gamma \circ \Gamma = \Gamma$。
令$\Gamma$为X和X之间的对应，并令G为其图。如果$\Gamma$在X上是等价，则$(x, x) \in G$对于所有$x \in X$；因此X是$\Gamma$的域。 关系 $(x, y) \in G$ 相当于 $(y, x) \in G$，因此相当于 $(x, y) \in \overset{-1}{G}$，因而 $G = \overset{-1}{G}$ 以及$\Gamma = \overset{-1}{\Gamma}$。 关系$(x, y) \in G$和$(y, z) \in G$暗示$(x, z) \in G$，因而$G \circ G \subset G$；相反，$(x, y) \in G$意味着$(x, x) \in G$，因此意味着$(x, y) \in G \circ G$，因而$G \subset G \circ G$；因而$G = G \circ G$，因而$\Gamma = \Gamma \circ \Gamma$。
¶ 相反，假设满足条件 (a)、(b) 和 (c)。 关系 $(x, y) \in G$ 是对称的（根据 (b)）且传递（根据 (c)）；因此它是等价关系，并且通过(a)它是X上的等价关系。

### 2. 等价类; 商集

令 $f$ 为函数，E 为域，F 为图。 关系“$x \in E$和$y \in E$和$f(x) = f(y)$”是E上的等价关系，称为等价关系*与f*相关。它相当于关系$(\exists z)((x, z) \in F$和$(y, z) \in F)$，即$(\exists z)((x, z) \in F$和$(z, y) \in \overset{-1}{F})$，因此它的图是$\overset{-1}{F} \circ F$。

¶ 我们现在将证明集合 $\mathrm{E}$ 上的每个等价关系 $\mathrm{R}$ 都属于这个型。设$\mathrm{G}$为$\mathrm{R}$的图。对于每个$x \in \mathrm{E}$，（非空）集合$\mathrm{G}(x) \subset \mathrm{E}$被称为$x$相对于*$\mathrm{R}$的*等价类；因此，它是所有$y \in \mathrm{E}$中的集合，使得$\mathrm{R}\{x, y\}$。对于某些$x \in \mathrm{E}$，每个可以写为$\mathrm{G}(x)$的集合称为等价类（相对于$\mathrm{R}$）。 等价类的元素被称为这个类的*代表元*。 等价类相对于$\mathrm{R}$的集合（即，对于某些$x \in \mathrm{E}$，形式$\mathrm{G}(x)$的所有对象的集合）被称为$\mathrm{E}$的*商集* $\mathrm{R}$ 并用$\mathrm{E}/\mathrm{R}$ 表示。 映射 $x \to \mathrm{G}(x)$ $(x \in \mathrm{E})$，域为$\mathrm{E}$，目标为$\mathrm{E}/\mathrm{R}$，称为$\mathrm{E}$到$\mathrm{E}/\mathrm{R}$的*典范映射*。

C55。 *让*$\mathrm{R}$*成为集合*$\mathrm{E}$上的等价关系，*并让$p$成为*$\mathrm{E}$*上的典范映射*$\mathrm{E}/\mathrm{R}$。 *然后*

$$\mathrm{R}\{x, y\} \Leftrightarrow (p(x) = p(y)).$$

对于上面的记号，令$x$和$y$为元素除以$\mathrm{E}$，使得

$$(x, y) \in \mathrm{G}.$$

然后$x \in \mathrm{E}$和$y \in \mathrm{E}$；让我们证明$\mathrm{G}(x) = \mathrm{G}(y)$。从 $y \in \mathrm{G}(x)$ 开始，我们有 (命题 1) $\mathrm{G}(y) \subset (\mathrm{G} \circ \mathrm{G})(x) = \mathrm{G}(x)$。另一方面，我们还有 $(y, x) \in \mathrm{G}$、从而 $\mathrm{G}(x) \subset \mathrm{G}(y)$，因此

$$\mathrm{G}(x) = \mathrm{G}(y),$$

即$p(x) = p(y)$。相反，如果$\mathrm{G}(x) = \mathrm{G}(y)$，我们有$y \in \mathrm{G}(y) = \mathrm{G}(x)$，所以$(x, y) \in \mathrm{G}$。这样就完成了证明。

¶ 典范映射 $p$ $\mathrm{E}$ 到$\mathrm{E}/\mathrm{R}$ (§ 3, no. 8, 定义 11) 的截面更简单地称为$\mathrm{E}$ 的*截面*（相对于关系 $\mathrm{R}$）。

*例*

#### 例 1 {#ens-ii-s6-n2-exa-1 .statement tag=03SD}

令$\mathrm{R}$为等价关系“$x \in \mathrm{E}$和$y \in \mathrm{E}$和$x = y$”在集合$\mathrm{E}$上。 $x \in \mathrm{E}$的等价类则为集合$\{x\}$，$\mathrm{E}$的典范映射$x \to \{x\}$到$\mathrm{E}/\mathrm{R}$是双射的。

#### 例 2 {#ens-ii-s6-n2-exa-2 .statement tag=03SE}

令$\mathrm{E}$、$\mathrm{F}$为两个集合，并令$\mathrm{R}$为与$\mathrm{E} \times \mathrm{F}$的映射$\mathrm{pr}_1$相关联的$\mathrm{E} \times \mathrm{F}$到$\mathrm{E}$上的等价关系。 等价类相对于$\mathrm{R}$是形式$\{x\} \times \mathrm{F}$中的集合，其中$x \in \mathrm{E}$； 映射 $x \to \{x\} \times \mathrm{F}$ 是 $\mathrm{E}$ 的双射到 $(\mathrm{E} \times \mathrm{F})/\mathrm{R}$。

令集合 $\mathrm{E}$ 上的 $\mathrm{R}$ 为等价关系。 商集$\mathrm{E}/\mathrm{R}$是$\mathfrak{P}(\mathrm{E})$的子集，$\mathrm{E}/\mathrm{R}$的恒等映射是$\mathrm{E}$(§ 4, no. 7)的*划分*；因为如果$\mathrm{G}$是$\mathrm{R}$的图，对于所有$x \in \mathrm{E}$我们有$x \in \mathrm{G}(x)$，如果两个等价类$\mathrm{G}(x)$和$\mathrm{G}(y)$有公共的元素$z$，那么$\mathrm{R}\{x,\ z\}$和$\mathrm{R}\{y,\ z\}$，所以$\mathrm{G}(x) = \mathrm{G}(y)$。此外，关系

$$(\exists \mathrm{X})(\mathrm{X} \in \mathrm{E}/\mathrm{R} \text{ and } x \in \mathrm{X} \text{ and } y \in \mathrm{X})$$

相当于$\mathrm{R}\{x,\ y\}$。

¶ 相反，令$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$为集合E的划分。立即验证关系$(\exists \iota)(\iota \in \mathrm{I}$和$x \in \mathrm{X}_\iota$和$y \in \mathrm{Y}_\iota)$为E上的等价关系R； 等价类相对于R正好是划分的集合$\mathrm{X}_\iota$，而映射$\iota \to \mathrm{X}_\iota$在E/R上是I的双射。 E 的每个子集 S，对于每个 $\iota \in \mathrm{I}$，集合 $\mathrm{S} \cap \mathrm{X}_\iota$ 都由单个元素组成，称为等价类相对于 R 的 *系统代表*（或 *横向*）。该名称也用于表示任何单射将集合 K代入E，使得该单射下的K的像是关于R的等价类代表的系统；对于例，E 的任何 *截面* 相对于 R。

### 3. 关系与等价关系兼容

令$\mathrm{R}\{x,\ x'\}$为等价关系，令$\mathrm{P}\{x\}$为关系。 关系 $\mathrm{P}\{x\}$ 据说与等价关系* $\mathrm{R}\{x,\ x'\}$（相对于$x$）*相容的，如果我们有

$$(\mathrm{P}\{x\} \text{ and } \mathrm{R}\{x,\ y\}) \Rightarrow \mathrm{P}\{y\},$$

其中$y$表示既不在P也不在R中出现的字母。

对于例，从 C43 (章 I, §5)、no. 1) 可以得出，每个关系 $\mathrm{P}\{x\}$ 都与等价关系 $x = x'$ 相容的。

C56。 *让* $\mathrm{R}\{x,\ x'\}$ *在集合* E 上成为等价关系，*并让* $\mathrm{P}\{x\}$ *成为关系，它不是包含字母* $x'$ *并且与等价关系*相容的（相对于* $x$*） $\mathrm{R}\{x,\ x'\}$。 *那么，如果*$t$*没有出现在*$\mathrm{P}\{x\}$，*关系“*$t \in \mathrm{E}/\mathrm{R}$*和*$(\exists x)(x \in t$*和*$\mathrm{P}\{x\})$*”相当于关系“*$t \in \mathrm{E}/\mathrm{R}$*和*$(\forall x)((x \in t) \Rightarrow \mathrm{P}\{x\})$*”。*

让$t \in \mathrm{E}/\mathrm{R}$。如果存在$a \in t$使得$\mathrm{P}\{a\}$，那么对于每个$x \in t$我们有$\mathrm{R}\{a,\ x\}$，因此有$\mathrm{P}\{x\}$。因此$(\exists x)(x \in t$和$\mathrm{P}\{x\})$意味着$(\forall x)((x \in t) \Rightarrow \mathrm{P}\{x\})$。 逆命题是显而易见的，因为 $t \in \mathrm{E}/\mathrm{R}$ 意味着 $t \neq \emptyset$。

¶ 关系

$$t \in \mathrm{E}/\mathrm{R} \text{ and } (\exists x)(x \in t \text{ and } \mathrm{P}\{x\})$$

据说是由*$P\{x\}$*在经过上与R的商*（相对于$x$）引起。如果这个关系由$P'\{t\}$表示，并且如果$f$是E在E/R上的典范映射，则关系

$$y \in E \text{ and } P'\{f(y)\}$$

（其中 $y$ 未出现在 $P\{x\}$ 中）与（$y \in E$ 和 $P\{y\}$）“等效”，已立即验证。

### 4. 饱和子集

令$R\{x, y\}$为集合E上的等价关系，并令A为E的子集。如果关系$x \in A$与$R\{x, y\}$相容的（相对于$x$），则称A相对于*R是*饱和的；或者，等效地，如果*对于$x$的每个$x \in A$等价类都包含在*A中。在其他字中，集合相对于R饱和当且仅当它是等价类的集合的*并相对于*R。

¶ 令 $f$ 为 E 到 E/R 的典范映射。如果 A 相对于 R 是饱和的，则每个 $x \in A$ 的等价类（等于$\overset{-1}{f}\langle\{f(x)\}\rangle$）包含在 A 中，因此$\overset{-1}{f}\langle f\langle A\rangle\rangle \subset A$；因为无论如何我们都有$A \subset \overset{-1}{f}\langle f\langle A\rangle\rangle$，所以随之而来的是$\overset{-1}{f}\langle f\langle A\rangle\rangle = A$。相反，如果$A = \overset{-1}{f}\langle f\langle A\rangle\rangle$，则对于$x$的每个$x \in A$等价类$K = f(x)$，相对于R来说，是$f\langle A\rangle$的元素；从 $K = \overset{-1}{f}\langle\{K\}\rangle$ 开始，我们就有了 $K \subset \overset{-1}{f}\langle f\langle A\rangle\rangle = A$。因此，相对于 R 饱和的 E 的子集恰好是 E 的子集 A，使得 $A = \overset{-1}{f}\langle f\langle A\rangle\rangle$。等价地，它们是形式$\overset{-1}{f}\langle B\rangle$的E的子集，其中$B \subset E/R$；对于关系$A = \overset{-1}{f}\langle B\rangle$意味着$B = f\langle A\rangle$，因此$A = \overset{-1}{f}\langle f\langle A\rangle\rangle$。

¶ 如果 $(X_\iota)_{\iota \in I}$ 是 E 的饱和子集族，则集合 $\bigcup_{\iota \in I} X_\iota$ 和 $\bigcap_{\iota \in I} X_\iota$ 饱和（§4、命题 3 和 4）。如果 A 是 E 的饱和子集，则 $\complement_E A$ (§4，命题 6) 也是如此。

¶ 现在设 A 为 E 的任意子集。则集合 $\overset{-1}{f}\langle f\langle A\rangle\rangle$ 包含于 A 且饱和。相反，如果 A′ 是 E 的饱和子集，其中包含 A，则我们有 $f\langle A'\rangle \supset f\langle A\rangle$，因此

$$A' = \overset{-1}{f}\langle f\langle A'\rangle\rangle \supset \overset{-1}{f}\langle f\langle A\rangle\rangle.$$

因此，我们可以说$\overset{-1}{f}\langle f\langle A\rangle\rangle$是E的“最小的”饱和子集，其中包含A（cf.章III）；这个集合被称为A相对于关系R的*饱和度*。可以立即看出，A的饱和度是A的元素的等价类的并。如果$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$是E的子集族，并且如果$\mathrm{A}_\iota$是$\mathrm{X}_\iota$相对于R，则$\bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$的饱和度为$\bigcup_{\iota \in \mathrm{I}} \mathrm{A}_\iota$（§4，命题3）。

### 5. 映射兼容等价关系

设 R 为集合 E 上的等价关系，并令 $f$ 为函数，且域 E。则如果关系 $y = f(x)$ 相容的（相对于 $x$），则称 $f$ 与关系* R *兼容关系$\mathrm{R}\{x,\ x'\}$。

¶ 说 $f$ 的限制到每个等价类是一个常数映射也是同样的事情，在这种情况下，我们说 *$f$ 对于每个等价类相对于* R 来说是常数。如果 $g$ 是 E 到 E/R 上的典范映射，则等价叙述是关系$g(x) = g(x')$隐含$f(x) = f(x')$；因此 (§3, 命题 9) 我们有以下标准：

C57。 *令* R *为集合* E 上的等价关系，*并让g 为* E *到* E/R 上的典范映射。 *则映射 f of* E *into* F * 与* R *兼容当且仅当 f 可以放入形式 h $\circ$ g 中，其中 h 是映射 of* E/R *into* F。 *映射 h 由 f 唯一确定；如果 s 是 g 的任意截面，则我们有 h $= f \circ s$。*

映射 $h$ 据说是由 f 在经过上*导出关于 R 的商*。

¶ 设 $f$ 为集合 E 的映射到集合 F，并设 $\mathrm{A} = f\langle \mathrm{E}\rangle \subset \mathrm{F}$。令 R 为等价关系与 $f$ (no. 2) 相关联；显然，$f$ 与 R 相容的。此外，$f$ 在经过上引发的映射 $h$ 的商是 E/R 到 F 的 *单射*：因为如果 $t$、$t'$ 相对于 R 是等价类，使得$h(t) = h(t')$，对于所有$x \in t$和$x' \in t'$，我们有$f(x) = f(x')$，这意味着$t = t'$除以R的定义。令$k$为E/R的映射到A，其与$h$具有相同的图；那么 $k$ 是*双射的*。如果$j$是A到F的典范嵌入，并且如果$g$是E到E/R的典范映射，那么我们可以写

$$f = j \circ k \circ g.$$

这个关系被称为f*的*规范分解。

¶ 令$f$为集合E的映射到集合F，令R为E上的等价关系，并令S为F上的等价关系。令$u$为E到E/R的典范映射，并令$v$为$F$ 的典范映射到$F/S$。如果 $v\mathbin{\circ}f$ 与 $R$ 相容的，则映射 $f$ 据说与等价关系* $R$ 和 $S$ 相容的；这意味着关系 $x\equiv x'$ (mod $R$) *意味着* $f(x)\equiv f(x')$ (mod $S$)。将$E/R$的映射$h$代入$F/S$，由$v\mathbin{\circ}f$在经过上引出，与$R$的商，则称为*映射，由$f$在经过上引出，与尊重$R$和$S$*；其特点是关系$v\mathbin{\circ}f=h\mathbin{\circ}u$。

### 6. 逆像等价关系；诱导等价关系

设$\varphi$为集合$E$的映射到集合$F$，并令$S$为$F$上的等价关系。 If $u$ is the canonical mapping of $F$ onto $F/S$, the equivalence relation associated with the mapping $u\mathbin{\circ}\varphi$ of $E$ into $F/S$ is called the *inverse image* of $S$ under $\varphi$; if $R$ is this relation, $R\{x,y\}$ is equivalent to $S\{\varphi(x),\varphi(y)\}$, and the equivalence classes with respect to $R$ are the inverse images under $\varphi$ of the equivalence classes with respect to $S$ which meet $\varphi\langle E\rangle$.

¶ 特别地，考虑集合$E$上的等价关系$R$，并令$A$为$E$的子集；那么$A$的单射$j$下的$R$到$E$的逆像被称为$A$上的$R$*诱导*等价关系，并记为$R_A$。

¶ 等价类相对于$R_A$ 是等价类的$A$ 上相对于$R$ 与$A$ 相交的*迹*。 单射的$j$显然与关系$R_A$和$R$相容的； $A/R_A$的映射$h$到$E/R$由$j$在经过上引出关于$R_A$和$R$的商是$A/R_A$的*单射的*映射到$E/R$：如果$f$（或$g$）是$E$到$E/R$（或$A$到$A/R_A$）的典范映射，则关系$h(g(x))=h(g(x'))$，其中$x\in A$ 和 $x'\in A$ 等价于 $f(x)=f(x')$，因此也等价于 $g(x)=g(x')$。 像$h\langle A/R_A\rangle$等于$f\langle A\rangle$。如果$k$是$A/R_A$到$f\langle A\rangle$的双射映射，并且与$h$具有相同的图，则$k$及其逆被称为*规范*。

### 7. 等价关系的商

令$R$、$S$是关于两个字母$x$、$y$的两个等价关系。如果关系 $S\Rightarrow R$为真，我们可以说$S$比$R$*更细*（或者$R$比$S$*粗糙*）。如果$R$和$S$是等价关系在同一个集合$E$上，叙述$S$比更细比$R$意味着$S$的图包含在$R$，或者再次，关于$S$的每个等价类都包含在关于$R$的等价类中；或者，等价地，关于$R$的每个等价类对于$S$都是饱和的。

*例*

#### 例 1 {#ens-ii-s6-n7-exa-1 .statement tag=03SF}

关系“$x \in E$和$y \in E$和$x = y$”比E上的每个等价关系为更细。关系“$x \in E$和$y \in E$”比E上的每个等价关系更粗糙。

#### 例 2 {#ens-ii-s6-n7-exa-2 .statement tag=03SG}

\* 等价关系“$x \in \mathbf{Z}$和$y \in \mathbf{Z}$和$x - y$可以被4整除”是更细比等价关系“$x \in \mathbf{Z}$和$y \in \mathbf{Z}$和$x - y$可以被2整除”。 \*

令R和S为同一集合E上的两个等价关系，使得S比R更细。令$f$和$g$分别为E到E/R和E到E/S的典范映射；则函数 $f$ 与 S 相容。令 $h$ 为函数由 $f$ 在经过上导出关于 S 的商；那么$h$是E/S到E/R的映射。 E/S 上与 $h$ 相关的等价关系称为 *R *除* S 的商，并用 R/S 表示。 关系$x \equiv y \pmod{R}$等价于$g(x) \equiv g(y) \pmod{R/S}$，等价类相对于R/S是像低于等价类相对于R的$g$。令$h = j \circ h_2 \circ h_1$为规范的分解（no. 5） 映射$h$。那么$h_1$是E/S到(E/S)/(R/S)的典范映射，$j$是E/R的恒等映射，$h_2$是(E/S)/(R/S)到E/R的一对一映射。 映射 $h_2$ 及其逆被认为是*规范*。

¶ 相反，考虑集合 E/S 上的任意等价关系 T，并令 R 为 E 上的等价关系，即关系 T (no. 6) 的$g$ 下的逆像。由于关系$x \equiv y \pmod{R}$等价于$g(x) \equiv g(y) \pmod{T}$，因此T等价于R/S。

### 8. 乘积两个等价关系

令$R\{x, y\}$和$R'\{x', y'\}$为两个等价关系。让 $S\{u, v\}$ 表示关系

$$(\exists x)(\exists y)(\exists x')(\exists y')(u = (x, x') \text{ and } v = (y, y') \text{ and } R\{x, y\} \text{ and } R'\{x', y'\});$$

立即验证$S\{u, v\}$为等价关系，称为R和R'的*乘积*，记为$R \times R'$。假设 R 是集合 E 上的等价关系，R' 是集合 E' 上的等价关系。那么关系 $S\{u, u\}$ 相当于

$$(\exists x)(\exists x')(u = (x, x') \text{ and } R\{x, x\} \text{ and } R'\{x', x'\})$$

即，到$(\exists x)(\exists x')(u = (x, x')$、$x \in E$和$x' \in E')$，因此到$u \in E \times E'$。由此可见，$R \times R'$ 是$E \times E'$ 上的等价关系。如果

$$u = (x, x')$$

是 $E \times E'$ 的元素，关系 $S\{u, v\}$ 相当于

$$(\exists y)(\exists y')(v = (y, y') \text{ and } R\{x, y\} \text{ and } R'\{x', y'\});$$

如果$G$和$G'$分别是$R$和$R'$的图，那么这个关系又相当于$v \in G(x) \times G(x')$。因此*每个等价类相对于*$R \times R'$*是等价类的乘积相对于*$R$*和等价类相对于*$R'$，*反之亦然。*

¶ 令$f$和$f'$分别为$E$的典范映射到$E/R$和$E'$到$E'/R'$，并令$f \times f'$为$f$和$f'$的规范扩张到乘积集合（§ 3, no. 9）。然后 $(f \times f')(x, x') = (f(x), f'(x'))$ 代表所有 $(x, x') \in E \times E'$。 $(E/R) \times (E'/R')$的元素$(u, u')$$f \times f'$下的逆像相对于$R$和等价类正好是等价类$u$乘积$u \times u'$ $u'$相对于$R'$。由此可见，与 $f \times f'$ 关联的等价关系相当于 $R \times R'$。因此映射$f \times f'$可以写成$h \circ g$，其中$g$是$E \times E'$的典范映射到

$$(E \times E')/(R \times R')$$

并且 $h$ 是 $(E \times E')/(R \times R')$ 的一对一映射到

$$(E/R) \times (E'/R');$$

这个映射 $h$ 及其逆据说是*典范的*。

#### 注 {#ens-ii-s6-n8-rem-1 .statement tag=03IY}

令$P\{x, x'\}$为关系，其中字母$y$、$y'$不出现。如果关系 $(P\{x, x'\}$ 和 $R\{x, y\}$ 和 $R'\{x', y'\})$ 隐含 $P\{y, y'\}$，则 P 被认为与等价关系 $R\{x, y\}$ 和 $R'\{x', y'\}$（相对于 $x$ 和 $x'$）“相容的”。设$Q\{u\}$为关系$(\exists x)(\exists x')(u = (x, x')$和$P\{x, x'\})$；那么，$Q\{u\}$（相对于$u$）与等价关系、$S\{u, v\}$、乘积、$R$和$R'$相容的，这也是同样的道理。

### 9. 等价对象类

令 $R\{x, y\}$ 为等价关系，无需图表。显然，如果$x$、$x'$、$y$是三个不同的字母，则关系$R\{x, x'\}$意味着“$R\{x, y\} \Longleftrightarrow R\{x', y\}$”，因此也意味着关系$(\forall y)(R\{x, y\} \Longleftrightarrow R\{x', y\})$。由概形 S7 (章 I, § 5, no. 1)，如果我们放入 $\theta\{x\} = \tau_y(R\{x, y\})$，关系 $R\{x, x'\}$ 意味着

$$\theta\{x\} = \theta\{x'\}.$$

另一方面，注，定义$R\{x, \theta\{x\}\}$等于关系$(\exists y)(R\{x, y\})$，因而（no. 1）等于$R\{x, x\}$。由此可见，关系$(R\{x, x\}$、$R\{x', x'\}$和$\theta\{x\} = \theta\{x'\})$“等价”于$R\{x, x'\}$，因为这意味着，通过 S6 (章I, §5, no. 1)，关系

$$(R\{x, x\} \text{ and } R\{x', x'\} \text{ and } (R\{x', \theta\{x\}\} \Leftrightarrow R\{x', \theta\{x'\}\})),$$

因此还有$(R\{x, \theta\{x\}\}$和$R\{x', \theta\{x\}\})$，最后通过传递性和对称性得到$R\{x, x'\}$。相反，由于$R\{x, x'\}$蕴含$R\{x, x\}$和$R\{x', x'\}$，因此断言得到证明。 项$\theta\{x\}$称为对象的*类等价于x*（相对于关系R）。

¶ 现在假设 T 是项使得关系

(1) $$(\forall y)(R\{y, y\} \Rightarrow (\exists x)(x \in T \text{ and } R\{x, y\}))$$

是真的。那么关系$(\exists x)(R\{x, x\}$和$z = \theta\{x\})$在z*中是*集合化。因为我们可以假设$x \in T$意味着$R\{x, x\}$；将所有 $x \in T$ 中的替换 T 乘以集合就足够了，从而得到 $R\{x, x\}$（$R\{x, y\}$ 意味着$R\{x, x\}$ 的注意到）。令$\Theta$为$x \in T$（§1, no. 6）的形式$\theta\{x\}$的所有对象中的集合。假设$R\{y, y\}$为真；那么存在$x \in T$使得$R\{x, y\}$因此存在$\theta\{y\} = \theta\{x\} \in \Theta$。 集合$\Theta$相对于R称为等价对象类*的*集合；对于每个$x$，使得$R\{x, x\}$，$\theta\{x\}$是*唯一*元素$z \in \Theta$，使得$R\{x, z\}$。

在相同的假设下，令$A\{x\}$为项，使得$R\{x, y\}$蕴涵$A\{x\} = A\{y\}$。那么关系$(\exists x)(R\{x, x\}$和$z = \{x\})$是$z$中的集合化，因为$R\{x, x\}$等价于$R\{x, \theta\{x\}\}$，意味着$A\{x\} = A\{\theta\{x\}\}$，因此如果E是对象的集合形式 $A\{t\}$ 代表 $t \in \Theta$，则 $R\{x, x\}$ 意味着 $A\{x\} \in E$。如果$f$是函数$t \to A\{t\}$$(t \in \Theta, A\{t\} \in E)$，那么关系$R\{x, x\}$意味着$A\{x\} = f(\theta\{x\})$。

特别是，如果 R 是等价关系 *在集合* F 上，我们可以将 $A\{x\}$ 视为 x 相对于* R (no. 2) 的 *等价类，而函数 $f$ 则是$\Theta$ 上的 *双射* 商集前/后；这证明了引入术语的合理性。

\* *例*。设$R\{x, y\}$为等价关系“$x$和$y$是相同有限维在$\mathbf{C}$上的两个向量空间”；这个关系没有图表。当T是$\mathbf{C}^{(\mathbf{N})}$的所有向量子空间中的集合时，或者当T的子集T'由空间$\mathbf{C}^n$$(n \in \mathbf{N})$组成且$\mathbf{C}^0$组成的约定时，它满足条件(1) $\mathbf{C}^{(\mathbf{N})}$的点 0，并且$\mathbf{C}^n$$(n > 0)$是直和$\mathbf{C}^{(\mathbf{N})}$的前$n$分量的和。有了第二个选择，我们就有了$\Theta = T'$。\*

### 习题 {#ens-ii-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
