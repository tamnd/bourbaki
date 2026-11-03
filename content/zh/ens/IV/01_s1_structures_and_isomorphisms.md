---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 1
section_title: Structures and isomorphisms
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 259-271, 289
pdf_pages: 0264-0276, 0294-0294
extraction: ocr
subsections:
    - "no": 1
      title: ECHELONS
      page: 259
      pdf_page: 264
    - "no": 2
      title: CANONICAL EXTENSIONS OF MAPPINGS
      page: 260
      pdf_page: 265
    - "no": 3
      title: TRANSPORTABLE RELATIONS
      page: 261
      pdf_page: 266
    - "no": 4
      title: SPECIES OF STRUCTURES
      page: 262
      pdf_page: 267
    - "no": 5
      title: ISOMORPHISMS AND TRANSPORT OF STRUCTURES
      page: 264
      pdf_page: 269
    - "no": 6
      title: DEDUCTION OF STRUCTURES
      page: 266
      pdf_page: 271
    - "no": 7
      title: EQUIVALENT SPECIES OF STRUCTURES
      page: 268
      pdf_page: 273
statements: 17
exercises: 1
content_sha256: fd1e706c7a509b4cf2d669cefd2f93dd46f979aca990a9cde9c3bf6c095ac3ce
translated_from: content/en/ens/IV/01_s1_structures_and_isomorphisms.md
translation_method: google
source_content_sha256: 0afa8f8b2eeacc6c331a25088f06579b838538c263fddf5f044dbaa9e0fb2b95
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 23684532a46876882160f1d5bd1b5ac13409f6ce3cfc2f5563c36160cb97faa6
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 1. 结构和同构

这个章的目的是一劳永逸地描述数学中经常出现的形成性构造和证明（cf.章I, § 1, no. 3和§ 2, no. 2）中的某个数。

### 1. 阶梯

*梯队构造概形*为自然整数[^1]$c_i = (a_i,\ b_i)$、满足序列$c_1$、$c_2$、…、有序对、$c_m$如下条件：

(a)若$b_i = 0$，则$1 \leqslant a_i \leqslant i - 1$。
(b)若$a_i \neq 0$和$b_i \neq 0$，则$1 \leqslant a_i \leqslant i - 1$和$1 \leqslant b_i \leqslant i - 1$。

这些条件意味着$c_1 = (0,\ b_1)$，还有$b_1 > 0$。如果$n$是出现在对$(0,\ b_i)$中的整数$b_i$中的最大的，则$c_1, c_2, ..., c_m$被称为构造概形*在$n$上项*。

给定 $n$ 项上的梯队构造概形 $\mathrm{S} = (c_1,\ c_2,\ \ldots,\ c_m)$，并在理论上给定 $n$ 项 $\mathrm{E}_1$、$\mathrm{E}_2$、...、$\mathrm{E}_n$ $\mathscr{T}$ 比集合论更强，概形* $\mathrm{S}$ *on* $\mathrm{E}_1$, ..., $\mathrm{E}_n$ 的*梯队构造定义为序列 $\mathrm{A}_1$, $\mathrm{A}_2$, ..., 理论 $\mathscr{T}$ 中的 $m$ 项的$\mathrm{A}_m$，由以下条件逐步定义：

(a)若$c_i = (0,\ b_i)$，则$\mathrm{A}_i$为项$\mathrm{E}_{b_i}$。
(b)若$c_i = (a_i,\ 0)$，则$\mathrm{A}_i$为项$\mathfrak{P}(\mathrm{A}_{a_i})$。
(c)若$c_i = (a_i,\ b_i)$，其中$a_i \neq 0$和$b_i \neq 0$，则$\mathrm{A}_i$为项$\mathrm{A}_{a_i} \times \mathrm{A}_{b_i}$。

$\mathrm{E}_1$、...、$\mathrm{E}_n$ 上概形 S 的梯队构造的最后一个项 $\mathrm{A}_m$ 称为基集合* 上概形* S 的*梯队$\mathrm{E}_1$，...，$\mathrm{E}_n$；在随后的一般论证中，它将被表示为记号$\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n)$。

#### 例 {#ens-iv-s1-n1-exa-1 .statement tag=03V4}

给定两个集合 E、F，集合 $\mathfrak{P}(\mathfrak{P}(\mathrm{E})) \times \mathfrak{P}(\mathrm{F})$ 是 E、F 上的一个梯队，其中概形

$$(0, 1), \quad (0, 2), \quad (1, 0), \quad (3, 0), \quad (2, 0), \quad (4, 5).$$

也是E、F上概形的梯队

$$(0, 2), \quad (0, 1), \quad (1, 0), \quad (2, 0), \quad (4, 0), \quad (5, 3).$$

因此，不同的概形可能会在相同的项上产生相同的梯队。

### 2. 典范扩张 / 映射

设$\mathrm{S} = (c_1, c_2, \ldots, c_m)$为$n$项上的梯队构造概形。 令 $\mathrm{E}_1$, ..., $\mathrm{E}_n$, $\mathrm{E}'_1$, ..., $\mathrm{E}'_n$ 为集合（$\mathscr{T}$ 中的项），并令 $f_1$, ..., $f_n$ 为 $\mathscr{T}$ 中的项，使得关系“$f_i$是$\mathrm{E}_i$的映射到$\mathrm{E}'_i$”对于$1 \leqslant i \leqslant n$来说是$\mathscr{T}$中的定理。 令$\mathrm{A}_1$，...，$\mathrm{A}_m$（分别为$\mathrm{A}'_1$，...，$\mathrm{A}'_m$）为$\mathrm{E}_1$，...，$\mathrm{E}_n$（分别为$\mathrm{E}'_1$，...，$\mathrm{E}'_n$）上概形 S 的梯队构造。 我们一步步对$m$项$g_1$，...，$g_m$进行定义序列，使得$g_i$是*$\mathrm{A}_i$*进入*$\mathrm{A}'_i$（对于$1 \leqslant i \leqslant m$）的*映射，如下所示条件：

(a) 如果$c_i = (0, b_i)$，使得$\mathrm{A}_i = \mathrm{E}_{b_i}$和$\mathrm{A}'_i = \mathrm{E}'_{b_i}$，则$g_i$是映射$f_{b_i}$。

(b) 如果$c_i = (a_i, 0)$，使得$\mathrm{A}_i = \mathfrak{P}(\mathrm{A}_{a_i})$和$\mathrm{A}'_i = \mathfrak{P}(\mathrm{A}'_{a_i})$，则$g_i$是$g_{a_i}$到子集的集合的*规范扩张*$\hat{g}_{a_i}$（章II, § 5, no. 1）。

(c) 如果$c_i = (a_i, b_i)$，其中$a_i \neq 0$和$b_i \neq 0$，使得

$$\mathrm{A}_i = \mathrm{A}_{a_i} \times \mathrm{A}_{b_i} \qquad \text{and} \qquad \mathrm{A}'_i = \mathrm{A}'_{a_i} \times \mathrm{A}'_{b_i},$$

那么 $g_i$ 是 $g_{a_i}$ 和 $g_{b_i}$ 到 $\mathrm{A}_{a_i} \times \mathrm{A}_b$ (章 II, § 3, no. 9) 的*规范扩张* $g_{a_i} \times g_{b_i}$。

这个序列的最后一个项$g_m$被称为*规范扩张，与概形* S，*映射* $f_1$，...，$f_n$，并用$\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$表示。

¶ 下面的判据可以一步步验证：

CST1。 *如果* $f_i$ *是映射的* $\mathrm{E}_i$ *进入* $\mathrm{E}'_i$，*并且如果* $f'_i$ *是映射的* $\mathrm{E}'_i$ *进入* $\mathrm{E}''_i$ *(*$1 \leqslant i \leqslant n$*)，则对于每个梯队构造概形* S *上* $n$ *项我们有*

$$\langle f'_1 \circ f_1, f'_2 \circ f_2, \ldots, f'_n \circ f_n \rangle^{\mathrm{S}} = \langle f'_1, f'_2, \ldots, f'_n \rangle^{\mathrm{S}} \circ \langle f_1, f_2, \ldots, f_n \rangle^{\mathrm{S}}.$$

CST2。 *如果$f_i$是单射*（或*满射*）*对于* $1 \leqslant i \leqslant n$，*则*$\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$ *是单射*（或*满射*）。

该标准源自扩张 $\hat{g}$ (章 II, § 5, no. 1, 命题 1) 和扩张 $g \times h$ (章 II, § 3, no. 9) 的相应的属性。

CST3。 *如果$f_i$是*$\mathrm{E}_i$*的双射*到*$\mathrm{E}'_i$，*并且如果$f_i^{-1}$是逆双射*[^2]，*那么*$\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$*是双射并且*$\langle f_1^{-1}, \ldots, f_n^{-1} \rangle^{\mathrm{S}}$*是它的逆；在其他字*，

$$(\langle f_1, \ldots, f_n \rangle^{\mathrm{S}})^{-1} = \langle f_1^{-1}, \ldots, f_n^{-1} \rangle^{\mathrm{S}}.$$

这紧接着 CST1 和 CST2。

### 3. 可运输关系

令$\mathscr{T}$为比集合论强的理论，令$x_1, \ldots, x_n$、$s_1, \ldots, s_p$为与$\mathscr{T}$常数不同的不同字母，并令$\mathrm{A}_1, \ldots, \mathrm{A}_m$为$\mathscr{T}$中的项，其中没有字母$x_i$ $(1 \leqslant i \leqslant n)$ 和 $s_j$ $(1 \leqslant j \leqslant p)$ 出现。令$\mathrm{S}_1, \ldots, \mathrm{S}_p$为$n + m$项上的构造概形梯队。然后关系$\mathrm{T}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$：

“$s_1 \in \mathrm{S}_1(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$、$s_2 \in \mathrm{S}_2(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$、$\ldots$、$s_p \in \mathrm{S}_p(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$”

被称为字母$s_1, \ldots, s_p$的*典型化*。

¶ 令 $\mathrm{R}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ 为 $\mathscr{T}$ 中的关系，其中包含某些字母 $x_i$、$s_j$（也可能还有其他字母）。那么 R 被认为是*可转移* (*in* $\mathscr{T}$) *相对于典型化* T，*$x_i$ $(1 \leqslant i \leqslant n)$ 被视为主要基集合和* $\mathrm{A}_h$ $(1 \leqslant h \leqslant m)$ *作为辅助基集合*，如果满足以下条件：令$y_1, \ldots, y_n, f_1, \ldots, f_n$为不同于$x_i$$(1 \leqslant i \leqslant n)$、$s_j$$(1 \leqslant j \leqslant p)$、$\mathscr{T}$的常量以及出现在R或项中的所有字母的不同字母$\mathrm{A}_h$$(1 \leqslant h \leqslant m)$，并令$\mathrm{Id}_h$$(1 \leqslant h \leqslant m)$表示$\mathrm{A}_h$自身的恒等映射。然后关系

(1)“$\mathrm{T}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$和（$f_1$是$x_1$到$y_1$的双射）和$\ldots$和（$f_n$是$x_n$到$y_n$的双射）”

*意味着，在*$\mathscr{T}$，*关系*

(2) $\mathrm{R}\{x_1, \ldots, x_n, s_1, \ldots, s_p\} \Leftrightarrow \mathrm{R}\{y_1, \ldots, y_n, s'_1, \ldots, s'_p\}$，其中

$$(3) \qquad s'_j = \langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^s{}_j(s_j) \qquad (1 \leqslant j \leqslant p).$$

在没有辅助集合的情况下，还有一个类似但更简单的定义。

例如，如果$n = p = 2$并且如果典型化T是“$s_1 \in x_1$和$s_2 \in x_1$”，则关系$s_1 = s_2$是可传输的。另一方面，关系$x_1 = x_2$不可运输。

### 4. 结构种

令$\mathscr{T}$为理论，它比集合论强。 *$\mathscr{T}$中的*结构种*是由以下组合组成的文本$\Sigma$：

(1) 某个数字母$x_1, \ldots, x_n, s$，彼此不同且与$\mathscr{T}$常数不同； $x_1, \ldots, x_n$称为结构种$\Sigma$的*本色基集合*；

(2) $\mathscr{T}$中项$\mathrm{A}_1, \ldots, \mathrm{A}_m$中的某个数，其中没有$x_1, \ldots, x_n, s$出现，称为$\Sigma$的*辅助基集合*； $\Sigma$ 可能包含无辅助基集合（但必须包含至少一个主基集合）；

(3) 典型化$\mathrm{T}\{x_1, \ldots, x_n, s\}$：

$$s \in \mathrm{S}(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m),$$

其中 S 是 $n + m$ 项 (no. 1) 上的梯队构造概形； $\mathrm{T}\{x_1, \ldots, x_n, s\}$被称为结构种$\Sigma$的*典型刻画*；

(4) 关系 $\mathrm{R}\{x_1, \ldots, x_n, s\}$ 相对于典型 T 来说是*可移动的*（在 $\mathscr{T}$ 中），$x_i$ 是主基集合，$\mathrm{A}_h$ 是辅助基集合 （no. 3）； R 称为结构种 $\Sigma$ 的*公理*。

理论$\mathscr{T}_\Sigma$与$\mathscr{T}$具有相同的公理概形，并且其显式公理是$\mathscr{T}$的公理，与公理“T和R”一起称为结构种*$\Sigma$的*理论。因此，$\mathscr{T}_\Sigma$的常数是$\mathscr{T}$的常数以及T或R中出现的字母。

¶ 令$\mathscr{T}'$为理论，其强于$\mathscr{T}$，并令$\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}$为$\mathscr{T}'$中的项。在理论$\mathscr{T}'$中，U据说是类*$\Sigma$*的*结构*在主体基集合*$\mathrm{E}_1, \ldots, \mathrm{E}_n$，*与*$\mathrm{A}_1, \ldots, \mathrm{A}_m$*作为辅助基集合*，如果关系

$$\text{"}\mathrm{T}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\} \text{ and } \mathrm{R}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\}\text{"}$$

是*$\mathscr{T}'$中的*定理。如果是这样，那么对于理论$\mathscr{T}_\Sigma$关系$\mathrm{B}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\}$中的每个定理$\mathrm{B}\{x_1, \ldots, x_n, s\}$来说，都是*$\mathscr{T}'$中的*定理（章I, § 2, no. 3）。在$\mathscr{T}_\Sigma$中，常数$s$称为类* $\Sigma$的*泛型结构。

¶ 在理论 $\mathscr{T}'$ 中，校长基集合 $\mathrm{E}_1, \ldots, \mathrm{E}_n$ 据说*被赋予结构* $\mathrm{U}$。显然，$\mathrm{U}$ 是元素 / 集合

$$\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{A}_1, \ldots, \mathrm{A}_m).$$

$\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$ 元素 $\mathrm{V}$ 集合，因此满足关系 $\mathrm{R}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{V}\}$ 是类* $\Sigma$ * 上的结构 *集合 * $\mathrm{E}_1, \ldots, \mathrm{E}_n$（它可能是空的）。

*例*

#### 例 1 {#ens-iv-s1-n4-exa-1 .statement tag=03V5}

取$\mathscr{T}$为集合论，并考虑结构种没有辅助基集合，一个主基集合$\mathrm{A}$，典型的刻画$s \in \mathfrak{P}(\mathrm{A} \times \mathrm{A})$，以及公理

$$s \circ s = s \quad \text{and} \quad s \cap \overset{-1}{s} = \Delta_{\mathbf{A}}$$

（$\Delta_{\mathbf{A}}$是$\mathrm{A} \times \mathrm{A}$的对角线），相对于典型化$s \in \mathfrak{P}(\mathrm{A} \times \mathrm{A})$，它是可移动的关系，这很容易验证。显然，这个结构种的理论正好是*有序集*的理论（章III, §1, no. 3）；因此这样定义的结构的类也称为$\mathrm{A}$上序结构*的*类。在章III中，我们看到许多集合中的例都被赋予了这个类中的结构。

#### 例 2 {#ens-iv-s1-n4-exa-2 .statement tag=03V6}

取$\mathscr{T}$为集合论，并考虑结构种没有辅助基集合，一个主基集合$\mathrm{A}$，典型的刻画$\mathrm{F} \in \mathfrak{P}((\mathrm{A} \times \mathrm{A}) \times \mathrm{A})$，并且为可传输公理关系 “F 是一个函数图，其定义域为 $\mathrm{A} \times \mathrm{A}$”。这个类的结构是所谓的*代数结构*的特殊情况，而函数其图是$\mathrm{F}$（$\mathrm{A} \times \mathrm{A}$到$\mathrm{A}$的映射）被称为*the*（*处处定义*）*内部这样结构的合成*律。

#### 例 3 {#ens-iv-s1-n4-exa-3 .statement tag=03V7}

作为之前，令$\mathscr{T}$为集合论，并考虑结构种，它没有辅助基集合，一个主基集合$\mathrm{A}$，典型的刻画 $\mathrm{V} \in \mathfrak{P}(\mathfrak{P}(\mathrm{A}))$，并且作为公理，可运输关系

$$(\forall \mathrm{V}) \, ((\mathrm{V}' \subset \mathrm{V}) \Rightarrow ((\bigcup_{\mathrm{X} \in \mathrm{V}'} \mathrm{X}) \in \mathrm{V}))$$
$$\text{and} \quad (\forall \mathrm{X})(\forall \mathrm{Y})((\mathrm{X} \in \mathrm{V} \text{ and } \mathrm{Y} \in \mathrm{V}) \Rightarrow ((\mathrm{X} \cap \mathrm{Y}) \in \mathrm{V})).$$

这个结构种称为拓扑结构*的*类。这个类的结构又称为*拓扑*，关系$\mathrm{X} \in \mathrm{V}$用说表示$\mathrm{X}$是拓扑$\mathrm{V}$中的*开集合* （*一般拓扑*、章I, § 1）。

#### 例 4 {#ens-iv-s1-n4-exa-4 .statement tag=03V8}

\* 取$\mathscr{T}$为环结构除法的类的理论，它有（除其他外）一个常数K作为唯一（主）基集合。 *左向量空间超过* K 的结构类，有 K 作为辅助基集合，主要基集合E，以及典型的刻画关系

$$V \in \mathfrak{P}((E \times E) \times E) \times \mathfrak{P}((K \times E) \times E)$$

（pr$_1$V是E中加法的图，pr$_2$V是标量乘法的图）；我们不会在这里陈述这个结构种的公理。

#### 例 5 {#ens-iv-s1-n4-exa-5 .statement tag=03V9}

再次令$\mathscr{T}$为集合论；在这个理论中，复数的域$\mathbf{C}$是项，其中包含没有字母。 维数 n* 的*复杂解析流形的结构类具有$\mathbf{C}$作为辅助基集合，以及一个主体基集合 V。我们不会在这里指出典型的刻画或类或结构的公理。 \*

*注*

#### 注 1 {#ens-iv-s1-n4-rem-1 .statement tag=03VA}

在应用中，经常出现这样的情况（如上面的例 4），梯队$S(E_1, \ldots, E_n, A_1, \ldots, A_m)$是乘积或阶梯

$$S_1(E_1, \ldots, A_m) \times \cdots \times S_p(E_1, \ldots, A_m).$$

如果是这样，$\Sigma$的定义中的字母$s$通常会被替换为“$p$元组”$(s_1, \ldots, s_p)$（cf.章II, § 2, no. 1）。

此外，结构种$\Sigma$公理最常被写为几个可运输关系中的合取（如上面的例3）。这些关系称为类$\Sigma$的*公理*。

#### 注 2 {#ens-iv-s1-n4-rem-2 .statement tag=03VB}

命名为数学中最常用的结构种，以及赋予这些类中的结构的集合。因此，*有序的集合* (章 III, § 1) 是集合且赋予序结构 (例 1)； \* 在本级数的后续书籍中，我们将*群、域、拓扑空间、可微流形*等定义概念，所有这些都表示集合被赋予了一定的性质。 结构。 \*

#### 注 3 {#ens-iv-s1-n4-rem-3 .statement tag=03VC}

通过滥用语言，在集合论$\mathscr{T}$中，给出$n$不同的字母$x_1, \ldots, x_n$（没有典型的刻画也没有公理）被认为是结构$\Sigma_0$的类，称为集合*的*结构*在$n$本金基集合$x_1, \ldots, x_n$。

### 5. 同构和迁移 / 结构

设$\Sigma$为理论$\mathscr{T}$中的结构种，在$n$主体基集合$x_1, \ldots, x_n$，$m$辅助基集合$A_1, \ldots, A_m$。令S为$n + m$字母上的梯队构造概形，其特征在于$\Sigma$的典型刻画，并令R为$\Sigma$的公理。在比$\mathscr{T}$强的理论$\mathscr{T}'$中，令U为集合$E_1, \ldots, E_n$上类$\Sigma$的结构（作为主体基集合）并令U$'$为结构 *与集合 $E'_1, \ldots, E'_n$ 相同的类*。最后，让$f_i$（在$\mathscr{T}'$中）是$E_i$到$\mathrm{E}'_i$$(1 \leqslant i \leqslant n)$的*双射*。那么 $(f_1, \ldots, f_n)$ 被称为集合 $\mathrm{E}_1, \ldots, \mathrm{E}_n$ 的 *同构的*，赋有结构 U，到集合 $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$，赋有结构 $\mathrm{U}'$，如果我们有（在 $\mathscr{T}'$ 中）

(4) $$\langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(\mathrm{U}) = \mathrm{U}'$$

其中 $\mathrm{Id}_h$ 表示 $\mathrm{A}_h$ 的恒等映射到自身 $(1 \leqslant h \leqslant m)$ 上。

¶ 令 $f'_i$ 为双射 $f_i$ $(1 \leqslant i \leqslant n)$ 的倒数。它直接从 (4) 和标准 CST3 (no. 2) 得出

$$\langle f'_1, \ldots, f'_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(\mathrm{U}') = \mathrm{U}$$

因而，$(f'_1, \ldots, f'_n)$是$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$的*同构的*，赋予$\mathrm{U}'$，到$\mathrm{E}_1, \ldots, \mathrm{E}_n$，赋予U。同构的$(f_1, \ldots, f_n)$和$(f'_1, \ldots, f'_n)$据说是彼此的“逆”。

如果存在 $\mathrm{E}_1, \ldots, \mathrm{E}_n$ 的同构到 $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$，则赋有 $\mathrm{U}'$ 的$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ 被认为与赋有 U 的 $\mathrm{E}_1, \ldots, \mathrm{E}_n$ *同构的*；在这种情况下，结构 U 和 $\mathrm{U}'$ 被称为“同构的”。

¶ 上述定义与CST1一起意味着以下标准：

CST4。 *令* U、$\mathrm{U}'$、$\mathrm{U}''$ *分别为主体基集合* $\mathrm{E}_1, \ldots, \mathrm{E}_n$、$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$、$\mathrm{E}''_1, \ldots, \mathrm{E}''_n$*上相同类* $\Sigma$ *的三个结构。让*$f_i$*成为*$\mathrm{E}_i$*的双射*$\mathrm{E}'_i$，*并让*$g_i$*成为*$\mathrm{E}'_i$*的双射*$\mathrm{E}''_i$$(1 \leqslant i \leqslant n)$。 *如果*$(f_1, \ldots, f_n)$*和*$(g_1, \ldots, g_n)$*是同构，那么*$(g_1 \circ f_1, \ldots, g_n \circ f_n)$也是。

$\mathrm{E}_1, \ldots, \mathrm{E}_n$的同构到$\mathrm{E}_1, \ldots, \mathrm{E}_n$（相对于*相同*结构）被称为$\mathrm{E}_1, \ldots, \mathrm{E}_n$的*自同构*。 $\mathrm{E}_1, \ldots, \mathrm{E}_n$的两个自同构的合成是自同构，自同构的逆也是自同构，\*使得$\mathrm{E}_1, \ldots, \mathrm{E}_n$形式的自同构有*群*。 \*

#### 注 {#ens-iv-s1-n5-rem-1 .statement tag=03VD}

通过滥用语言，如果$f_i$是$\mathrm{E}_i$到$\mathrm{E}'_i$$(1 \leqslant i \leqslant n)$的任何双射，则相对于类，$(f_1, \ldots, f_n)$被称为是$\mathrm{E}_1, \ldots, \mathrm{E}_n$到$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$的同构结构共集合（no. 4、注 3）。

CST5。 *在理论*$\mathscr{T}'$*哪个比*$\mathscr{T}$强，*让*U*成为类*$\Sigma$*的结构，*在*$\mathrm{E}_1, \ldots, \mathrm{E}_n$，*并让*$f_i$*成为*的双射* $\mathrm{E}_i$ *到集合* $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$。 *则存在类* $\Sigma$ *在* $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ *上的唯一结构，使得* $(f_1, \ldots, f_n)$ *是* $\mathrm{E}_1, \ldots, \mathrm{E}_n$ *到* $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ 的同构。

对于这个结构，如果存在的话，只能是关系(4)定义的项$\mathrm{U}'$；这个项确实是类$\Sigma$的结构还有待验证，即关系$\mathrm{R}\{\mathrm{E}'_1, \ldots, \mathrm{E}'_n, \mathrm{U}'\}$在$\mathscr{T}'$中为真。但这是基于 $\mathrm{R}\{x_1, \ldots, x_n, s\}$ 是*可运输*的事实，对于

$R\{E'_1, \ldots, E'_n, U'\}$ 在 $\mathscr{T}'$ 中相当于关系 $R\{E_1, \ldots, E_n, U\}$ (no. 3)，在$\mathscr{T}'$ 和假设中也是如此。

¶ 结构 $U'$ 据说是通过通过双射映射* $f_1, \ldots, f_n$ *将结构* $U$ *传输到集合* $E'_1, \ldots, E'_n$ *获得。因此，相同类的两个结构是同构的，当且仅当每个迁移或结构从另一个迁移获得时。

类$\Sigma$的*任意*两个结构*必然同构*； 类或结构 $\Sigma$ 则被称为“单价”。 \* 这是无限循环群的结构（与$\mathbf{Z}$同构的）、特征零的素数域的结构（与$\mathbf{Q}$同构的）、完整阿基米德有序域的结构的情况（同构于$\mathbf{R}$），代数闭的、连通、局部紧拓扑域的结构（同构于$\mathbf{C}$），以及非交换、连通、局部紧拓扑除法的结构环（同构于$\mathbf{H}$，除法） 环四元数）。对于结构中的一些类，例如特征零的素数域，或者完整的阿基米德有序域，除了恒等映射之外，甚至没有任何自同构；但上面给出的其他例确实存在这样的自同构（例如，$\mathbf{Z}$中的对称性$x \rightarrow -x$）。 \*

可以看出，上面的类和结构本质上都是经典数学中的基。另一方面，群结构的\* 类、有序集合的结构种和拓扑结构的类不是单价的。 \*

### 6. 结构的演绎

设理论 $\mathscr{T}$ 中的 $\Sigma$ 为结构种，在 $n$ 主基集合 $x_1, \ldots, x_n$，$m$ 辅助基集合 $A_1, \ldots, A_m$。令$s$为$\Sigma$的泛型结构，令$T$为$n + m$项上的梯队构造概形。 项 $V\{x_1, \ldots, x_n, s\}$ 其中包含除了 $\mathscr{T}_\Sigma$ 的常数之外没有任何字母被认为是型 $T(x_1, \ldots, x_n, A_1, \ldots, A_m)$ $s$ 的*内在*，如果它满足以下条件 ：

(1) 关系 $V\{x_1, \ldots, x_n, s\} \in T(x_1, \ldots, x_n, A_1, \ldots, A_m)$ 是 $\mathscr{T}_\Sigma$ 中的定理；

(2) 设$\mathscr{T}'_\Sigma$为理论，通过将$\mathscr{T}_\Sigma$公理的公理邻接“$f_i$是$x_i$的双射到$y_i$”$(1 \leqslant i \leqslant n)$（其中字母$y_i$ 和 $f_i$ 彼此不同，并且与 $\mathscr{T}_\Sigma$ 的常数不同，对于 $1 \leqslant i \leqslant n$）；如果$s'$是$s$通过$(f_1, \ldots, f_n)$（no. 5）运输结构，则

$$V\{y_1, \ldots, y_n, s'\} = \langle f_1, \ldots, f_n. \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{T}}(V\{x_1, \ldots, x_n, s\})$$

$\mathscr{T}'_\Sigma$ 中有定理。

结构种的理论中的项中的 1 个通向定义的大部分是内在的项。

¶ 设$\Theta$为理论$\mathscr{T}$中的另一个结构种，在$r$主体基集合$u_1,\ldots,u_r$，$p$辅助基集合$B_1,\ldots,B_p$，并令$t\in T(u_1,\ldots,u_r,B_1,\ldots,B_p)$为$\Theta$（no. 4）的典型刻画。然后 $r+1$ 项 $P,U_1,\ldots,U_r$ 的系统，$s$ 的固有值，并且使得 $P$ 是 $U_1,\ldots,U_r$ 上的类 $\Theta$ 的结构， 理论$\mathscr{T}_\Sigma$，从类$\Sigma$结构称为类$\Theta$结构演绎的过程。由于滥用语言，项$P$通常被称为演绎的过程。

¶ 令$\mathscr{T}'$ 理论强于$\mathscr{T}$。如果$E_1,\ldots,E_n$上类$\Sigma$$\mathscr{T}'$中$\mathscr{S}$为结构，则$P\{E_1,\ldots,E_n,\mathscr{S}\}$为$r$集合上类$\Theta$结构 $F_j=U_j\{E_1,\ldots,E_n,\mathscr{S}\}$$(1\leq j\leq r)$，据说是通过过程$P$从$\mathscr{S}$推导出来的，或者从属于$\mathscr{S}$。 假设项 $P,U_1,\ldots,U_r$ 是 $s$ 的内在特征，此外还意味着以下标准：

**CST6.** 设$(g_1,\ldots,g_n)$为$E_1,\ldots,E_n$的同构，赋予类$\Sigma$的结构$\mathscr{S}$，到$E'_1,\ldots,E'_n$，赋予相同的类的结构$\mathscr{S}'$。如果 $U_j$ 是型 $\mathfrak{P}(T_j)$，则将

$$
h_j=\langle g_1,\ldots,g_n,\mathrm{Id}_1,\ldots,\mathrm{Id}_{m}\rangle^{T_j}\quad(1\leq j\leq r),
$$

并让 $F'_j=U_j\{E'_1,\ldots,E'_n,\mathscr{S}'\}$ $(1\leq j\leq r)$。然后，当集合的这些系统被赋予分别从$\mathscr{S}$和$\mathscr{S}'$推导出的类$\Theta$的结构时，$(h_1,\ldots,h_r)$是$F_1,\ldots,F_r$的同构到$F'_1,\ldots,F'_r$上$P$。

很明显，项$x_1,\ldots,x_n$是$s$的内在特征。在很多情况下，项$U_1,\ldots,U_r$是某些字母$x_1,\ldots,x_n$；通过过程$P$从$s$推导出类$\Theta$的结构则被称为$s$基础上的结构。

*例*

#### 例 1 {#ens-iv-s1-n6-exa-1 .statement tag=03VE}

\* 拓扑群结构的种类只有一个主基集$A$，没有辅助基集，对应的泛型结构是一对$(s_1,s_2)$（$s_1$是$A$上的合成律图，$s_2$是$A$拓扑中的开集集合；cf.一般拓扑，章节III, § 1）。 每个项$s_1,s_2$都是演绎的过程，并分别提供拓扑群结构$(s_1,s_2)$底层的群结构和拓扑。

同样，从向量空间结构可以推导出潜在的交换律群结构。从环结构可以推导出一个基础交换律群结构和一个（乘法）半群

IV
结构

结构。从可微流形的结构可以推导出底层拓扑等。

#### 例 2 {#ens-iv-s1-n6-exa-2 .statement tag=03VF}

$\mathbf{C}$（或$\mathbf{R}$）上的向量空间结构种类具有主基集$E$、等于$\mathbf{C}$（或$\mathbf{R}$）的辅助基集，以及典型的表征

$$
s_1\in\mathfrak{P}((E\times E)\times E)\qquad\text{and}\qquad s_2\in\mathfrak{P}((\mathbf{C}\times E)\times E)
$$

（分别为$s_1\in\mathfrak{P}((E\times E)\times E)$和$s_2\in\mathfrak{P}((\mathbf{R}\times E)\times E)$）。

对$(s_1,s_2\cap((\mathbf{R}\times E)\times E))$是向量空间结构的演绎在$\mathbf{R}$上从向量空间结构在$\mathbf{C}$上的过程（“标量域的限制到$\mathbf{R}$”）。 \*

#### 例 3 {#ens-iv-s1-n6-exa-3 .statement tag=03VG}

假设$\Theta$与$\Sigma$具有相同的（主要和辅助）基集合，以及相同的典型刻画。 此外，如果$\Sigma$公理隐含（在$\mathscr{T}$中）$\Theta$公理，那么很明显，项$s$是从物种$\Sigma$的结构中演绎物种$\Theta$的结构的过程。 $\Theta$ 则被认为比 $\Sigma$ 更穷，$\Sigma$ 比 $\Theta$ 更富有。 类 $\Sigma$中的每个结构，在理论$\mathscr{T}'$中比$\mathscr{T}$强，则也是类$\Theta$中的结构。 例如，全有序集合的结构种类（以有序结构公理（no. 4，例1）与关系式$s\cup s^{-1}=A\times A$合取为公理而得）比有序结构的种类更丰富。 \*交换群结构的种类比群结构的种类更丰富。 紧凑拓扑空间结构的类比拓扑结构的类丰富，等等\*

#### 例 4 {#ens-iv-s1-n6-exa-4 .statement tag=077U}

\* 当$\Sigma$和$\Theta$中的每一个是群结构（或环结构）的类时，在代数中定义了演绎的过程，它与每个群结构（或环结构）群结构相关联（分别为环结构）在其中心上。当$\Sigma$在域$K$上是向量空间结构的类时，以及当$\Theta$在$K$上是代数结构的类时，存在演绎的定义过程，其关联每个向量空间超过$K$，其张量代数或其外部代数。稍后我们将在这个级数中遇到许多其他例。 \*

#### 注 {#ens-iv-s1-n6-rem-1 .statement tag=03VH}

当$P$是“q元组”$(P_1,\ldots,P_q)$时，还可以说项$P_1,\ldots,P_q$从类$\Sigma$的结构构成类$\Theta$的结构的演绎的过程。

### 7. 等价种 / 结构

令$\Sigma$和$\Theta$为两个结构种，在同一个理论$\mathscr{T}$中，具有相同的主体基集合$x_1,\ldots,x_n$。令$s,t$分别为类$\Sigma,\Theta$的泛型结构。假设满足以下条件：

(1) 我们有一个从$x_1,\ldots,x_n$上物种$\Sigma$的结构演绎$x_1,\ldots,x_n$上物种$\Theta$的结构$P\{x_1,\ldots,x_n,s\}$的过程。

(2) 我们有一个从$x_1,\ldots,x_n$上的物种$\Theta$的结构推导$x_1,\ldots,x_n$上的物种$\Sigma$的结构$Q\{x_1,\ldots,x_n,t\}$的过程。

(3) 关系 $Q\{x_1,\ldots,x_n,P\{x_1,\ldots,x_n,s\}\}=s$ 是$\mathscr{T}_{\Sigma}$ 中的定理，关系 $P\{x_1,\ldots,x_n,Q\{x_1,\ldots,x_n,t\}\}=t$ 是$\mathscr{T}_{\Theta}$ 中的定理。

通过演绎$P$和$Q$的过程，结构种$\Sigma$和$\Theta$就被认为是等价的。在这种情况下，对于理论$\mathscr{T}_{\Sigma}$中的每个定理$B\{x_1,\ldots,x_n,s\}$，关系$B\{x_1,\ldots,x_n,Q\}$是$\mathscr{T}_{\Theta}$中的定理；相反，对于理论$\mathscr{T}_{\Theta}$中的每个定理$C\{x_1,\ldots,x_n,t\}$，关系$C\{x_1,\ldots,x_n,P\}$在$\mathscr{T}_{\Sigma}$中是定理。

☡

如果$U$是类$\Sigma$的结构，则通过过程$P$从$U$推导出结构相当于$U$。标准 CST6 意味着以下内容：

CST7。 *令$\mathscr{S},\mathscr{S}'$分别为基集合$(E_1,\ldots,E_n),(E'_1,\ldots,E'_n)$上的类$\Sigma$中的两个结构。设$\mathscr{S}_0,\mathscr{S}'_0$为类$\Theta$中的结构，分别相当于$\mathscr{S}$和$\mathscr{S}'$。在序中，$(g_1,\ldots,g_n)$相对于结构$\mathscr{S}_0$和$\mathscr{S}'_0$应该是同构，$(g_1,\ldots,g_n)$相对于结构$\mathscr{S}$应该是同构是必要且充分的，并且$\mathscr{S}'$.*

在实践中，我们对结构的两个等价种的理论$\mathscr{T}_{\Sigma}$和$\mathscr{T}_{\Theta}$没有区别。

*例*

#### 例 1 {#ens-iv-s1-n7-exa-1 .statement tag=03VI}

\* 令 $\Sigma$ 为可交换的群结构的类； $\Sigma$有一个（主）基集合$A$，其通用结构由单个字母$F$组成； $\Sigma$的典型刻画是$F\in\mathfrak{P}((A\times A)\times A)$，我们用$R\{A,F\}$表示$\Sigma$的公理。这个公理特别意味着$F$是函数的图（群的“合成的律”；cf.no. 4，例2）。在理论$\mathscr{T}_{\Sigma}$（其中$\mathscr{T}$表示集合论），我们定义项$M\{A,F\}$是$\mathfrak{P}((\mathbf{Z}\times A)\times A)$中的函数图，并且满足以下关系$B\{M,A,F\}$：

$$
(\forall x)(\forall y)(\forall n)((x\in A\ \text{and}\ y\in A\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(n,F(x,y))=F(M(n,x),M(n,y))))
$$

和

$$
(\forall x)(\forall m)(\forall n)((x\in A\ \text{and}\ m\in\mathbf{Z}\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(m+n,x)=F(M(m,x),M(n,x))))
$$

和

$$
(\forall x)(\forall m)(\forall n)((x\in A\ \text{and}\ m\in\mathbf{Z}\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(m,M(n,x))=M(mn,x)))
$$

和

$$
(\forall x)((x\in A)\Rightarrow (M(1,x)=x)).
$$

（“乘法元素 $A$ 整数”）。

考虑$\mathbf{Z}$模块结构中的类$\Theta$，它具有单一主体基集合$A$，$\mathbf{Z}$作为辅助集合，其泛型结构包含两个字母G，L，典型的刻画

$G \in \mathfrak{P}((A \times A) \times A)$ 和 $L \in \mathfrak{P}((\mathbf{Z} \times A) \times A)$

和公理

“$R \mid A, G$和$(L$是函数图）和$B \mid L, A, G$”。

立即验证，项F、M从类$\Sigma$结构构成类$\Theta$结构演绎的过程，项G是结构演绎的过程类$\Sigma$从结构类$\Theta$。此外，上面的条件(3)也基本满足。因此，我们可以说可交换的群结构的类和$\mathbf{Z}$模结构的类是等价的。

#### 例 2 {#ens-iv-s1-n7-exa-2 .statement tag=03VJ}

令$\Sigma$为拓扑结构（no. 4，例3）的类，令$A$为（主）基集合，令$V$为$\Sigma$的泛型结构。考虑关系

$$x \in A \text{ and } X \subset A \text{ and } (\forall U)((U \in V \text{ and } x \in U) \Rightarrow (X \cap U \neq \varnothing)).$$

这个关系有一个关于对$(X, x)$的图$P \subset \mathfrak{P}(A) \times A$； $P \mid A, V$ 被项称为“所有对 $(X, x)$ 的集合，使得 $x$ 位于 $X$ 相对于拓扑 $V$ 的闭包”。然后我们可以证明（cf.一般拓扑，章I, § 1）以下关系是$\mathscr{T}_{\Sigma}$中的定理：

$$P(\varnothing)=\varnothing,$$

$$(\forall Y)((Y \subset A) \Rightarrow (\forall Y \subset P(Y))),$$

$$(\forall Y)((Y \subset A) \Rightarrow (P(P(Y))=P(Y))),$$

$$(\forall Y)(\forall Z)((Y \subset A \text{ and } Z \subset A) \Rightarrow (P(Y \cup Z)=P(Y)\cup P(Z))).$$

考虑结构种$\Theta$，有一个（主要）基集合$A$，其泛型结构由单个字母$W$组成，它具有典型的刻画$W \in \mathfrak{P}(\mathfrak{P}(A) \times A)$和公理

$$W(\varnothing)=\varnothing \text{ and } (\forall Y)((Y \subset A) \Rightarrow (Y \subset W(Y)))$$

和

$$(\forall Y)((Y \subset A) \Rightarrow (W(W(Y))=W(Y)))$$

和

$$(\forall Y)(\forall Z)((Y \subset A \text{ and } Z \subset A) \Rightarrow (W(Y \cup Z)=W(Y)\cup W(Z))).$$

还要考虑关系

$$U \subset A \text{ and } (\forall x)((x \in U) \Rightarrow x \notin W(A-U)).$$

所有$U \in \mathfrak{P}(A)$中的集合，其中满足这个关系是$\mathfrak{P}(A)$中的子集$Q \mid A, W$。然后我们可以证明（一般拓扑，章I, § 1，习题10）以下关系是$\mathscr{T}_{\Theta}$中的定理：

$$A \in Q,$$

$$(\forall M)((M \subset Q) \Rightarrow ((\bigcup_{X \in M} X) \in Q)),$$

$$(\forall X)(\forall Y)((X \in Q \text{ and } Y \in Q) \Rightarrow ((X \cap Y) \in Q)).$$

因此，项$P\{A,V\}$和$Q\{A,W\}$满足条件（1）和（2），并且很容易看出它们也是满足条件（3）。因此，结构种$\Sigma$和$\Theta$是等价的，因此我们将类$\Theta$中的每个结构视为拓扑，即按照演绎$Q\{A,W\}$的程序将对应加到拓扑。 \*

### 习题{#ens-iv-s1-exercises}

参见[习题为 § 1](exercises/s1/)。

[^1]: We use the notion of integer in the same manner as in Chapter I, that is to say, in the metamathematical sense of marks arranged in a certain order; this use has nothing to do with the mathematical theory of integers which was developed in Chapter III.
[^2]: For typographical reasons we write here $f^{-1}$ instead of $\overset{-1}{f}$.
