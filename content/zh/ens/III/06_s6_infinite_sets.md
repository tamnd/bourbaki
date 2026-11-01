---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 6
section_title: Infinite sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 183-190, 241-251
pdf_pages: 0189-0196, 0247-0257
extraction: ocr
subsections:
    - "no": 1
      title: THE SET OF NATURAL INTEGERS
      page: 183
      pdf_page: 189
    - "no": 2
      title: DEFINITION OF MAPPINGS BY INDUCTION
      page: 184
      pdf_page: 190
    - "no": 3
      title: PROPERTIES OF INFINITE CARDINALS
      page: 186
      pdf_page: 192
    - "no": 4
      title: COUNTABLE SETS
      page: 188
      pdf_page: 194
    - "no": 5
      title: STATIONARY SEQUENCES
      page: 189
      pdf_page: 195
statements: 26
exercises: 32
content_sha256: db0422503f9ca2a0f86da9f14cafd8972994f7c362e3af7a16f1692a1e6237cf
translated_from: content/en/ens/III/06_s6_infinite_sets.md
translation_method: google
source_content_sha256: 567e0c5f3b6c1ecb2bc3cd823e4e97976fc38f1c07ab89e7b0f38f5f38c28c46
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0e0b4dfb
glossary_version: 34
glossary_terms_sha256: b9cf08d87b59c46e671f65c89fee81ebef1649f869b5e27a4ed21a38a0ddd6d7
prompt_sha256: 133cd3fc3c262b082830ff023554f589fe553d569c36079625221572907a2124
---

## 6.无限集合

### 1. 自然整数的集合

#### 定义 1 {#ens-iii-s6-def-1 .statement tag=03MV}

*集合如果不是有限的就说是无限的。*

特别是，如果基数不是整数，则它是无限的。

关系“存在无限集合”意味着关系“$x$是整数”是*集合化*（章II, § 1, no. 4）；因为如果$\mathfrak{a}$是无限基数并且$n$是任意整数，那么我们不能有$\mathfrak{a} \leqslant n$（§ 4, no. 2，命题2）。因此，我们对所有整数$n$有$n < \mathfrak{a}$，这表明整数$< \mathfrak{a}$中的集合（§ 3, no. 2，注在定理1之后）包含所有整数。相反，如果关系“$x$是整数”是集合化，则整数的集合E是*无限*集合。对于每个整数$n$，区间$[0, n]$是E的$n + 1$元素的子集（§ 5, no. 3，命题5）。因此卡片(E)$\geqslant n + 1 > n$。但如果说 Card(E) $\neq n$ 对于每个整数 $n$ 意味着 E 是无限的。

¶ 我们现在介绍以下公理：

A5（“无穷大公理”。）*存在无限集合。*

不知道这个公理是否可以从前面介绍的公理和公理概形推出；尽管这个问题尚未得到明确解决，但可以假定该公理独立于其他公理。

前面的注再证明下面的定理：

#### 定理 1 {#ens-iii-s6-thm-1 .statement tag=03MW}

*关系“$x$是整数”是集合化。*

我们将用整数的$\mathbf{N}$集合来表示（必要时也称为“自然整数的集合”以避免歧义）。 $\mathbf{N}$的基数用$\aleph_0$表示。每当$\mathbf{N}$被认为是有序的集合时，总是考虑在§ 3, no. 2中定义的排序（称为*通常*排序），除非则明确说明相反。

#### 定义 2 {#ens-iii-s6-def-2 .statement tag=03MX}

*序列*（集合*E 元素*序列）*是一个家庭*（分别*E 元素*家庭）*其指标集合为子集* $\mathbf{N}$。 *如果指标集合是*$\mathbf{N}$的无限子集，则称序列是无限的。

令$\mathrm{P}\{n\}$为关系，并令I表示整数$n$的集合，使得$\mathrm{P}\{n\}$为真。那么I就是$\mathbf{N}$的子集。 序列$(x_n)_{n\in\mathrm{I}}$则将有时写成$(x_n)_{\mathrm{P}\{n\}}$，$x_n$称为序列中的*n个项*。 序列，其指标集合是整数$n \geqslant k$的集合，通常写成$(x_n)_{k \leqslant n}$或$(x_n)_{n \geqslant k}$，甚至如果$k = 0$或则直接写成$(x_n)$ $k = 1$。同样条件下，对于例，用记号$\prod_{\mathrm{P}\{n\}} \mathrm{X}_n$和$\prod_{n=k}^{\infty} \mathrm{X}_n$来表示集合$(\mathrm{X}_n)_{n\in\mathrm{I}}$的序列乘积，类似的还有记号对于并、交、基数乘积和基数和。

序列的每个子族都是序列，称为给定序列的*子序列*。

两个序列 $(x_n)_{n\in\mathrm{I}}$、$(y_n)_{n\in\mathrm{I}}$ 具有相同的指标集合据说*仅在其项的序不同* 如果存在指标的置换 $f$ 集合I，使得$x_{f(n)} = y_n$对于所有$n \in \mathrm{I}$。

*倍数序列* 是指标集合是子集 / 乘积 $\mathbf{N}^p$ ($p$ 整数) ("双序列”代表$p = 2$，“三重序列”代表$p = 3$，依此类推）。

令I等于$\mathbf{N}$的集合，并令$f$为$\mathbf{N}$的双射到I。对于由集合I索引的每个族$(x_\iota)_{\iota\in\mathrm{I}}$，序列$n \to x_{f(n)}$据说是通过*排列族*$(x_\iota)_{\iota\in\mathrm{I}}$*在由*$f$定义的序中获得的。 序列，其中对应以这种方式与$\mathbf{N}$的两个不同的双射到I的不同之处仅在于它们的项的序。对于由 $n$ 元素的集合 I 索引的有限族，我们可以类似地将定义有限序列与 $[1, n]$ 或 $[0, n-1]$ 作为指标集合，通过安排序中的家庭由这些间隔中的一个或另一个的双射定义到I。

### 2. 定义映射截至归纳

由于集合$\mathbf{N}$是良序的，我们可以应用标准C60（§ 2, no. 2），它现在采用以下形式（具有相同的记号）：

C62。 *令$u$为字母，令*$\mathrm{T}\{u\}$*为项。那么存在集合* U *和* $\mathbf{N}$ *到* U *的映射 $f$，这样对于每个整数 $n$，我们有* $f(n) = \mathrm{T}\{f^{(n)}\}$，*其中$f^{(n)}$表示* $[0, n[$的映射 *到* $f([0, n[)$ *与* $[0, n[$ 上的$f$ 一致。 *此外，集合* U *和映射$f$是由这个条件唯一确定的。*

我们将从中推出以下标准：

C63。 *令*$S\{v\}$*和*$a$*为两个项。那么对于每个整数* $n \geqslant 1$，存在集合* $V$ *和映射* $f$ *of* $\mathbf{N}$ *到* $V$ *这样* $f(0) = a$ *和* $f(n) = S\{f(n-1)\}$ *。 *此外，集合* $V$ *和映射* $f$ *由这些条件唯一确定。*

要从 C62 [^1] 推导出 C63，令

$$D(u) = \mathscr{E}_x(x \in \mathbf{N} \ \text{and} \ (\exists y)((x, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))))$$

每个字母$u$。如果$u$是$\mathbf{N}$子集到集合的映射，那么$D(u)$就是$u$(章II, § 3, no. 1)的域。令$M(u)$为$\mathbf{N}$[^2]中$D(u)$中最小的上界。令$\varphi$为空映射，以$\emptyset$为源和目标，即（章II, § 3，第1和4），三元组$(\emptyset, \emptyset, \emptyset))$并考虑关系

$$(u = \varphi \ \text{and} \ y = a) \ \text{or} \ (u \neq \varphi \ \text{and} \ y = S\{u(M(u))\})$$

我们用 $R\{y, u\}$ 表示；最后，令$T\{u\}$为项$\tau_y(R\{y, u\})$。将C62应用于项$T\{u\}$。由于$f^{(0)}$等于$\varphi$，所以我们有$T\{f^{(0)}\} = a$；因此$f(0) = a$。另一方面，如果$n > 0$，我们有$D(f^{(n)}) = [0, n-1]$和$M(f^{(n)}) = n-1$，从而

$$T\{f^{(n)}\} = S\{f^{(n)}(n-1)\} = S\{f(n-1)\}.$$

*例*

#### 例 1 {#ens-iii-s6-n2-exa-1 .statement tag=03TC}

假设$a$是集合$E$的元素，$S\{u\}$是项$g(u)$，其中$g$是$E$自身[^3]的映射。然后归纳立即在$n$上看到，对于所有$n \in \mathbf{N}$，我们有$f(n) \in E$；因而，$f$是$\mathbf{N}$的映射到$E$，这样对于所有整数$n$，$f(0) = a$和$f(n+1) = g(f(n))$。

同样，令$h$为$\mathbf{N} \times E$的映射到$E$，并令$\psi$为$\mathbf{N} \times E$的映射到由$\psi(n, x) = (n+1, h(n, x))$定义的自身。通过前面的讨论，$\mathbf{N}$存在唯一映射$g = (\theta, f)$进入$\mathbf{N} \times E$，使得所有$n$都有$g(0) = (0, a)$和$g(n+1) = \psi(g(n))$，由此得出映射$f$的存在性和唯一性 $\mathbf{N}$ 代入 E，使得每个整数 $n$ 都有 $f(0) = a$ 和 $f(n + 1) = h(n, f(n))$。

#### 例 2 {#ens-iii-s6-n2-exa-2 .statement tag=03TD}

令X为集合，并令E为X的映射的集合自身。令$e$将X的恒等映射表示为自身，并令$f$为E的任意元素。将$S\{u\}$视为项$f \circ u$[^4]。通过应用 C63，我们看到E中存在$\mathbf{N}$的唯一映射，用$n \to f^n$表示，这样$f^0 = e$和$f^{n+1} = f \circ f^n$。 映射 $f^n$ 被称为映射 $f$ 的*n 次迭代*。

#### 例 3 {#ens-iii-s6-n2-exa-3 .statement tag=03TE}

如果我们取$S\{u\}$为项$\mathfrak{P}(u)$，$a$为集合E，则同样存在$\mathbf{N}$到集合的映射，记为$n \to \mathfrak{P}^n(\mathrm{E})$。 V(E)，使得每个整数$n$都有$\mathfrak{P}^0(\mathrm{E}) = \mathrm{E}$、$\mathfrak{P}^1(\mathrm{E}) = \mathfrak{P}(\mathrm{E})$和$\mathfrak{P}^{n+1}(\mathrm{E}) = \mathfrak{P}(\mathfrak{P}^n(\mathrm{E}))$。

#### 注 {#ens-iii-s6-n2-rem-1 .statement tag=03MY}

令E为集合，令A为E的子集，令$g$为A到E的映射，令$a$为A的元素。取$S\{u\}$为项$g(u)$。准则 C63 适用并证明 $\mathbf{N}$ 的映射 $f$ 存在于集合 V 上，使得对于每个整数 $n$ 都有$f(0) = a$ 和 $f(n + 1) = g(f(n))$。可能会发生$\mathrm{V} \subset \mathrm{A}$；如果不是，则令$p$为最大的整数，使得$f([0, p]) \subset \mathrm{A}$。那么$f(p + 1) = g(p) \notin \mathrm{A}$，$g(g(p))$就是项，无话可说。因此，在这种情况下，$f$被认为仅在区间$[0, p + 1]$上定义（“限制归纳”）。

### 3. 无限基数的性质

#### 定理 2 {#ens-iii-s6-thm-2 .statement tag=03MZ}

*对于每个无限基数$\mathfrak{a}$，我们有$\mathfrak{a}^2 = \mathfrak{a}$。*

我们将使用以下两个引理 ：

#### 引理 1 {#ens-iii-s6-lem-1 .statement tag=03N0}

*每个无限集合 E 包含集合等价于 $\mathbf{N}$。*

E 上存在一个良序关系（§ 2, no. 3，定理 1），我们将其表示为$x \leqslant y$。 假设意味着良序集 E 不能同构于不同于 $\mathbf{N}$ 的$\mathbf{N}$ 段，因为这样的段是形式 $[0, n]$ (§ 2, no. 1, 命题 1)，因此是有限的。由此可见，$\mathbf{N}$同构于E的一段（§ 2, no. 3，定理3），从而结果。

#### 引理 2 {#ens-iii-s6-lem-2 .statement tag=03N1}

*集合 $\mathbf{N} \times \mathbf{N}$ 相当于$\mathbf{N}$。*

由于$\mathbf{N} \times \mathbf{N}$包含集合$\{0\} \times \mathbf{N}$（与$\mathbf{N}$等价），我们有$\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(\mathbf{N} \times \mathbf{N})$。要完成证明，只需将$\mathbf{N} \times \mathbf{N}$中的定义单射$f$转化为$\mathbf{N}$即可。为此，我们注存在$\mathbf{N}$的单射$\varphi$到$\mathbf{N}$的映射到集合到$\mathrm{I} = \{0, 1\}$，得到如下：如果$r$是最小的整数，使得$n > 2^r$，如果 $\sum_{k=0}^{r-1} \varepsilon_k 2^{r-k-1}$ 是 $n$ (§ 5, no. 7) 的二元展开，$\varphi(n)$ 定义为序列 $(u_m)_{m \in \mathbf{N}}$，使得 $u_m = \varepsilon_{r-m-1}$ 对于 $m < r$ 且$u_m = 0$ 换$m \geqslant r$。 命题 8 of § 5, no. 7 表明 $\varphi$ 是单射的。对于每个对$(n, n') \in \mathbf{N} \times \mathbf{N}$，我们定义$f(n, n')$如下：如果$\varphi(n) = (u_m)$和$\varphi(n') = (v_m)$，则令$f(n, \; n')$为整数$s$，使得$\varphi(s) = w_m$，其中$w_{2m} = u_m$和$w_{2m+1} = v_m$ 对于所有$m \in \mathbf{N}$。显然，关系$f(n, \; n') = f(n_1, \; n_1')$蕴涵$\varphi(n) = \varphi(n_1)$和$\varphi(n') = \varphi(n_1')$；因此$(n, n') = (n_1, n_1')$，因此$f$是单射的。

¶ 现在我们来讨论定理 2 中的证明。令 E 为集合，使得 $\mathrm{Card}(\mathrm{E}) = \mathfrak{a}$。令 D 为 E 的子集等价于 $\mathbf{N}$ (引理 1)。那么在 $\mathrm{D} \times \mathrm{D}$ (引理 2) 上存在 D 的双射 $\psi_0$。令$\mathfrak{M}$为对$(\mathrm{X}, \psi)$的集合，其中X为E包含D的子集，$\psi$为X到$\mathrm{X} \times \mathrm{X}$的双射，其中扩展$\psi_0$。 序集合 $\mathfrak{M}$ 通过关系

$$\text{``} \mathrm{X} \subset \mathrm{X}' \text{ and } \psi' \text{ is an extension of } \psi \text{''}$$

介于 $(\mathrm{X}, \psi)$ 和 $(\mathrm{X}', \psi')$ 之间。然后立即看出$\mathfrak{M}$是*归纳*（cf.§ 2, no. 4，例2）。因此，根据佐恩的引理（§ 2, no. 4，定理2），$\mathfrak{M}$有极大元素$(\mathrm{F}, f)$。我们将证明$\mathrm{Card}\,(\mathrm{F}) = \mathfrak{a}$，这足以证明定理。如果$\mathrm{Card}\,(\mathrm{F})$不等于$\mathfrak{a}$，则设$\mathrm{Card}\,(\mathrm{F}) = \mathfrak{b} < \mathfrak{a}$。那么$\mathfrak{b} = \mathfrak{b}^2$和$\mathfrak{b}$是无限的，$\mathfrak{b} \leqslant 2\mathfrak{b} \leqslant 3\mathfrak{b} \leqslant \mathfrak{b}^2 = \mathfrak{b}$（§ 3, no. 6，命题14）；因此$2\mathfrak{b} = \mathfrak{b}$和$3\mathfrak{b} = \mathfrak{b}$。从假设$\mathfrak{b} < \mathfrak{a}$得出$\mathrm{Card}\,(\mathrm{E} - \mathrm{F}) > \mathfrak{b}$，否则我们应该有$\mathrm{Card}\,(\mathrm{E}) \leqslant 2\mathfrak{b} = \mathfrak{b}$，并且我们假设$\mathfrak{b} < \mathrm{Card}\,(\mathrm{E})$。因此，子集 $\mathrm{Y} \subset \mathrm{E} - \mathrm{F}$ 等价于 F。令 $\mathrm{Z} = \mathrm{F} \cup \mathrm{Y}$；我们将证明Z在$\mathrm{Z} \times \mathrm{Z}$上存在双射$g$，其中扩展$f$。我们有

$$\mathrm{Z} \times \mathrm{Z} = (\mathrm{F} \times \mathrm{F}) \cup (\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y}),$$

右边的四个乘积互为不相交的。由于 F 和 Y 等价，所以我们有

$$\mathrm{Card}(\mathrm{F} \times \mathrm{Y}) = \mathrm{Card}(\mathrm{Y} \times \mathrm{F}) = \mathrm{Card}(\mathrm{Y} \times \mathrm{Y}) = \mathfrak{b}^2 = \mathfrak{b},$$

从而

$$\mathrm{Card}((\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y})) = 3\mathfrak{b} = \mathfrak{b}.$$

因此 Y 的双射 $f_1$ 到集合

$$(\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y});$$

将 Z 的映射 $g$ 转换为 Z $\times$ Z，等于 F 上的 $f$ 和 Y 上的 $f_1$，因此是双射，扩展 $f$，与 $f$ 的定义相反。因此$\mathrm{Card}(\mathrm{F}) = \mathfrak{a}$和证明是完整的。

#### 推论 1 {#ens-iii-s6-thm-2-cor-1 .statement tag=03N2}

*如果 $\mathfrak{a}$ 是无限基数，则 $\mathfrak{a}^n = \mathfrak{a}$ 对于每个整数 $n \geqslant 1$。*

$n$归纳。

#### 推论 2 {#ens-iii-s6-thm-2-cor-2 .statement tag=03N3}

*非零基数有限族$(\mathfrak{a}_i)_{i \in \mathrm{I}}$的乘积，其中最大的是无限基数$\mathfrak{a}$，等于$\mathfrak{a}$。*

令$\mathfrak{b}$表示乘积，并令$n$为I中元素的数。然后$\mathfrak{b} \leqslant \mathfrak{a}^n = \mathfrak{a}$（§ 3, no. 6，命题14）。另一方面，由于 $\mathfrak{a}_i \geqslant 1$ 对于所有 $i \in \mathrm{I}$，我们有 $\mathfrak{b} \geqslant \mathfrak{a}$（§ 3, no. 6，命题 14）。

#### 推论 3 {#ens-iii-s6-thm-2-cor-3 .statement tag=03N4}

*设 $\mathfrak{a}$ 为无限基数，$(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ 为$\leqslant \mathfrak{a}$ 基数家族，其中指标集合 I 有一个基数 $\leqslant \mathfrak{a}$。然后$\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \leqslant \mathfrak{a}$；如果 $\mathfrak{a}_\iota = \mathfrak{a}$ 至少有一个指标 $\iota \in \mathrm{I}$，则 $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \mathfrak{a}$。*

令$\mathfrak{b}$为I的基数；那么我们就有 $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \leqslant \mathfrak{a}\mathfrak{b} \leqslant \mathfrak{a}^2 = \mathfrak{a}$ (§ 3, no. 6, 命题 14)，以及所有 $\varkappa \in \mathrm{I}$ 的 $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \geqslant \mathfrak{a}_\varkappa$。

#### 推论 4 {#ens-iii-s6-thm-2-cor-4 .statement tag=03N5}

*如果 $\mathfrak{a}$ 和 $\mathfrak{b}$ 是两个非零基数，其中之一是无穷大，则我们有 $\mathfrak{a}\mathfrak{b} = \mathfrak{a} + \mathfrak{b} = \sup\,(\mathfrak{a},\,\mathfrak{b})$。*

这直接从推论 2 和推论 3 得出。

### 4.可数集

#### 定义 3 {#ens-iii-s6-def-3 .statement tag=03N6}

*如果集合与集合$\mathbf{N}$等价于子集或整数，则称其为可数。*

#### 命题 1 {#ens-iii-s6-prop-1 .statement tag=03N7}

*可数集合中的每个子集都是可数的。 可数集有限族中的乘积是可数的。 可数集序列并是可数的。*

第一个断言是显而易见的。其他的则从推论到定理 2、no. 3。

¶ 我们已经证明 (no. 3, 引理 1) 如果 $\mathfrak{a}$ 是任意无限基数，则$\mathrm{Card}(\mathbf{N}) \leqslant \mathfrak{a}$。它具有以下推论 ：

#### 命题 2 {#ens-iii-s6-prop-2 .statement tag=03N8}

*每个可数无限集合 E 等价于 $\mathbf{N}$。*

$\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathbf{N})$ 定义；和$\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(\mathrm{E})$，因为 E 是无限的。

#### 命题 3 {#ens-iii-s6-prop-3 .statement tag=03N9}

*每个无限集合有划分* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *由可数无限集合* $\mathrm{X}_\iota$、*指标集合* I *等价于* E。

对于$\mathrm{Card}(\mathrm{E}) = \mathrm{Card}(\mathrm{E})\ \mathrm{Card}(\mathbf{N})$（no. 3，定理2，推论4）。

#### 命题 4 {#ens-iii-s6-prop-4 .statement tag=03NA}

*让*$f$*成为集合*E*的映射到无限集合*F*，使得对于每个*$y \in \mathrm{F}$，$\overset{-1}{f}(y)$*是可数的。那么* F * 等价于* E。

对于E的集合$\overset{-1}{f}(y)$$(y \in \mathrm{F})$形式划分；因此

$$\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathrm{F})\mathrm{Card}(\mathbf{N}) = \mathrm{Card}(\mathrm{F}),$$

和$\mathrm{Card}(\mathrm{F}) \leqslant \mathrm{Card}(\mathrm{E})$乘命题 3 / § 3, no. 2。

#### 命题 5 {#ens-iii-s6-prop-5 .statement tag=03NB}

集合* $\mathfrak{F}(\mathrm{E})$ * 无限集合* E * 有限子集等价于* E。

对于每个整数$n$，让$\mathfrak{F}_n$表示E的子集中的集合，其中E具有$n$元素。对于每个$\mathrm{X} \in \mathfrak{F}_n$，$[1, n]$中存在双射到X。因此$\mathfrak{F}_n$的基数至多等于$[1, n]$的映射到E的集合的基数，即$\mathrm{Card}(\mathrm{E}^n) = \mathrm{Card}(\mathrm{E})$（no. 3，定理2，推论1）。因此

$$\mathrm{Card}(\mathfrak{F}(\mathrm{E})) = \sum_{n \in \mathbf{N}} \mathrm{Card}(\mathfrak{F}_n) \leqslant \mathrm{Card}(\mathrm{E})\mathrm{Card}(\mathbf{N}) = \mathrm{Card}(\mathrm{E}).$$

另一方面，由于$x \to \{x\}$是E到$\mathfrak{F}(\mathrm{E})$的单射映射，所以我们有$\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathfrak{F}(\mathrm{E}))$。

#### 定义 4 {#ens-iii-s6-def-4 .statement tag=03NC}

*如果集合与* $\mathbf{N}$的所有子集中的集合等价，则称其具有连续统的幂。

具有幂连续统的集合不可数（§ 3, no. 6，定理 2）。

\* “连续统的幂”这个名称源自于实数的集合与$\mathfrak{P}(\mathbf{N})$等价（*一般拓扑*，章IV, § 8）。 \* *连续统假设*是断言，每个不可数集合包含子集都有连续统的幂； *广义连续统假设*是断言，对于每个无限基数$\mathfrak{a}$，每个基数$> \mathfrak{a}$都是$\geqslant 2^{\mathfrak{a}}$。

### 5.平稳序列

#### 定义 5 {#ens-iii-s6-def-5 .statement tag=03ND}

*序列* $(x_n)_{n \in \mathbf{N}}$ *of 元素 of 集合* E *如果存在整数* $m$ *使得* $x_n = x_m$ *对于所有整数* $n \geqslant m$，则称其为平稳。

#### 命题 6 {#ens-iii-s6-prop-6 .statement tag=03NE}

*令* E *为有序集合。那么下面的叙述是等价的：*

(a) ** E *的每个非空子集都有极大元素。*
(b) ** E *的元素中的每个递增序列* $(x_n)$ *都是静止的。*

我们首先证明（a）蕴涵（b）。令X为序列$(x_n)$元素集合，并令$x_m$为X极大元素。如果$n \geqslant m$，我们有假设$x_n \geqslant x_m$，因此$x_n = x_m$的最大$x_m$。相反，假设 E 存在一个非空子集 A，且没有极大元素。对于每个$x \in A$，令$T_x$为所有$y \in A$中的集合，使得$y > x$。 假设之前，$x \in A$ 全部为 $T_x \neq \emptyset$；因此，存在 A 到 A 中的映射 $f$，使得对于所有 $x \in A$ 都有$f(x) > x$（章 II, § 5, no. 4，命题 6）。如果$a \in A$，则序列$(x_n)_{n \in \mathbf{N}}$由条件$x_0 = a$归纳定义，$x_{n+1} = f(x_n)$显然是递增并且不是平稳的。

#### 推论 1 {#ens-iii-s6-prop-6-cor-1 .statement tag=03NF}

*全序集* E *是良序的当且仅当* E *的元素的每个递减序列都是平稳的。*

因为说 E 是良序的，相当于说，E 的每个非空子集都有一个最小元素（§ 1, no. 10，命题 10），因此从命题 6 可以得出断言。

#### 推论 2 {#ens-iii-s6-prop-6-cor-2 .statement tag=03NG}

*有限有序集合的元素的每个递增序列都是平稳的。*

对于每个有限有序集合都有极大元素 (§ 4, no. 4, 命题 3, 推论 2)。

¶ 满足命题 6 的等价条件的有序集合 E 是有时，称为 *诺特*。

#### 命题 7（“诺特归纳中的原理”）{#ens-iii-s6-prop-7 .statement tag=03RM}

— *令* E *为诺特集合，并令* F *为* E *的子集，并具有以下性质：如果* $a \in E$ *使得关系* $x > a$ *意味着* $x \in F$，*则* $a \in F$。 *在这些条件下，* F $=$ E。

事实上，假设 E $\neq$ F；那么 E $-$ F 有极大元素 $b$。到定义时，我们为所有 $x > b$ 提供了 $x \in F$；但这意味着$b \in F$，这是荒谬的。

### 习题{#ens-iii-s6-exercises}

参见[习题为 § 6](exercises/s6/)。

[^1]: It is also possible to give a direct proof of C63, analogous to the proof of C60 (§ 2, no. 2).
[^2]: The definition of the least upper bound (§ 1, nos. 7, 8, and 9) can be formulated in such a way that it has a meaning even for a set which is not bounded above (it denotes a term, in the formalized language, of the form $\tau_x(R\{x\})$, which the reader will have no difficulty in writing down).
[^3]: If $g = (G, E, E)$, the term $g(u)$ is the term denoted by $\tau_y((u, y) \in G)$.
[^4]: Here we mean the term denoted by (T, X, X), where T is the term denoted by $\mathfrak{S}_z(z$ is an ordered pair and $(\exists y)((\mathrm{pr}_1 z, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))$ and $(y, \mathrm{pr}_2 z) \in \mathrm{pr}_1(\mathrm{pr}_1(f)))$.
