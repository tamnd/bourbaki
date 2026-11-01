---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 1
section_title: Artinian Modules and Noetherian Modules
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.1-A VIII.23
pdf_pages: 0018-0040
extraction: native
subsections:
    - "no": 1
      title: Artinian Modules and Noetherian Modules
      page: 1
      pdf_page: 18
    - "no": 2
      title: Artinian Rings and Noetherian Rings
      page: 4
      pdf_page: 21
    - "no": 3
      title: Countermodule
      page: 8
      pdf_page: 25
    - "no": 4
      title: Polynomials with Coefficients in a Noetherian Ring
      page: 9
      pdf_page: 26
statements: 36
exercises: 28
content_sha256: 041db160fe5b0c6213d54fdd5b66ae52c50c49211f1384c834388af27aa2cf6b
translated_from: content/en/alg/VIII/01_s1_artinian_modules_and_noetherian_modules.md
translation_method: google
source_content_sha256: d64719b4a6721ac9031c6bccd67b196cb6dafe3fc596f4fdebd425f00893c469
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 379a44f8c1a2b7b4bda411c911a9f52ea246c9d23ae431ec365210a526098807
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。 阿廷模与诺特模

### 1. Artinian Modules and Noetherian Modules

#### 定义 1 {#alg-viii-s1-def-1 .statement tag=0001}

设A为环。如果满足以下等价条件，我们称A-模 M 阿廷的（分别为诺特）：

(i) M 的子模中的每个非空集合按包含排序，具有最小（或最大）元素。

(ii) M 的子模中的每个递减（分别为递增）序列都是平稳的。

条件(i)和(ii)的等价由集合理论、III, §6, No. 5、p. 190、命题6得出。

A-模 M 是阿廷的（分别是诺特）当且仅当 M 被视为模超过同位$A_M$ 的环时，是阿廷的（分别是诺特）。

令 M 为阿廷的（分别为诺特）A-模。 M 的子模的每个非空集合，按包含排序，即左向（或右向）至少有元素（或最大元素）（集合理论、III, §1, No. 10、p. 145、命题 10）。

设 M 为阿廷的（分别为诺特）A-模和$(M_i)_{i\in I}$ M 的子模族。左族$(M_i)_{i\in I}$ 形式非空（分别为非空）的有限子族的交（分别为和）。右）M 的子模的有向集合。因而，存在 I 的有限子集 J，使得 $\bigcap_{i\in I}M_i=\bigcap_{i\in J}M_i$（分别为 $\sum_{i\in I}M_i=\sum_{i\in J}M_i$）。

#### 例 1 {#alg-viii-s1-n1-exa-1 .statement tag=0002}

有限维向量空间超过域是阿廷的和诺特。

#### 例 2 {#alg-viii-s1-n1-exa-2 .statement tag=0003}

设M为A-模。 If there exists an infinite family $(M_i)_{i\in I}$ of nonzero submodules of M whose sum is direct, then M is neither Artinian nor Noetherian: indeed, for every strictly decreasing (resp. strictly increasing) infinite sequence $(J_n)$ of subsets of I, the infinite sequence $(\sum_{i\in J_n}M_i)$ of submodules of M is strictly decreasing (resp. strictly increasing). 特别是，无限维向量空间超过域既不是阿廷的也不是诺特。

#### 例 3 {#alg-viii-s1-n1-exa-3 .statement tag=0004}

我们将进一步看到 $\mathbf{Z}$-模块 $\mathbf{Z}$ 是诺特但不是

阿廷的 (VIII, p. 5, 例 3)$.*$

#### 例 4 {#alg-viii-s1-n1-exa-4 .statement tag=0005}

令$p$为素数数，$M_p$为挠元$\mathbf{Z}$-模$\mathbf{Q}/\mathbf{Z}$的$p$主分量（VII, §2, No. 2，p. 7）。对于整数 $n\in \mathbf{N}$ (VII, §2、p. 54、习题 3)，$M_p$ 的每个子模都等于 $M_p$ 或 $p^{-n}\mathbf{Z}/\mathbf{Z}$。因而，$M_p$是阿廷的，但不是诺特$\mathbf{Z}$模。

#### 命题 1 {#alg-viii-s1-prop-1 .statement tag=0006}

A-模 M 有有限长度 (II, §1, No. 10, p. 212) 当且仅当它既是阿廷的又是诺特。

假设 M 有有限长度 $d$。那么M的子模中的每一个严格递增的或严格递减序列最多有$d+ 1$项（I, §4, No. 7，p. 44）。因而，M 为阿廷的和诺特。

相反，假设M是阿廷的和诺特。设$\mathscr{S}$为有限长度M的子模集合。 零子模是$\mathscr{S}$的元素，并且由于M是诺特，所以$\mathscr{S}$有极大元素N。让我们通过反证法给出证明并假设$M\not= N$。 M 的子模中的集合与 N 和包含 N 不同，则具有最小元素 P，因为 M 是阿廷的。 模$P/N$有长度1，并且由于N是有限长度的模，因此同样适用于P（II, §1, No. 10，p. 212，命题16）。 N的这个与……矛盾定义。

#### 命题 2 {#alg-viii-s1-prop-2 .statement tag=0007}

A-模 M 是诺特当且仅当 M 的每个子模都是有限生成的。

首先假设 M 的每个子模都是有限生成的。令$(P_n)_{n\in\mathbf{N}}$为M的子模的递增序列，并令P为其并。这是 M 的子模。到假设时，存在 M 生成的模 P 的有限子集 F；令$n\in \mathbf{N}$为整数，使得$F\subset P_n$。然后我们有 $P_n= P$，并且序列 $(P_n)_{n\in\mathbf{N}}$ 是静止的。这就证明模 M 是诺特。

逆命题是以下更精确的叙述中的推论。

#### 引理 1 {#alg-viii-s1-lem-1 .statement tag=0008}

设M为M的诺特A-模和E子集。存在E生成的的有限子集F与E相同的子模。

事实上，根据VIII，p. 2，存在E的有限子集 F，使得$\sum_{x\in E}Ax=\sum_{x\in F}Ax$。

#### 命题 3 {#alg-viii-s1-prop-3 .statement tag=0009}

设 M 为 M 的 A-模且 N 子模。则 M 为阿廷的（或诺特）当且仅当 N 和 $M/N$ 为。

如果是阿廷模，我们就给出证明； 诺特模的情况类似。

假设M是阿廷的。由于 N 的每个子模都是 M 的子模，因此模 N 是阿廷的。令$(P_n)_{n\in\mathbf{N}}$为$M/N$的子模中的递减序列。 M 包含 N 中存在子模的递减序列 $(Q_n)_{n\in\mathbf{N}}$，使得对于每个 $n\in \mathbf{N}$ (I, §4, No. 6, p. 41, 定理 4) 都有$P_n= Q_n/N$。由于 M 是阿廷的，序列 $(Q_n)$ 是平稳的，因此序列 $(P_n)$ 也是平稳的。因而，模$M/N$是阿廷的。

相反，假设模 N 和$M/N$ 为阿廷的，并考虑M 的子模的递减序列 $(P_n)$。N 的子模序列 $P'_n= N\cap P_n$ 是平稳的。同样，$M/N$的子模的序列$P''_n= (N + P_n)/N$是静止的。因而，存在整数$m\in \mathbf{N}$，这样对于每个整数$n\geqslant m$，我们都有$P'_n= P'_m$和$P''_n= P''_m$。 序列 $(P_n)$ 然后通过以下引理静止。

#### 引理 2 {#alg-viii-s1-lem-2 .statement tag=00QV}

设 M 为 A-模，M 的 N、P 和 Q 子模。假设我们有 $P\subset Q$、$N\cap P = N\cap Q$，且 N + P = N + Q。则有 P = Q。

令 $x$ 为 Q 的元素。属于为 N + P；因而，存在 P 的元素$y$使得$x-y\in N$。由于 Q 包含于 P，差 $x-y$ 属于到 $N\cap Q$，因此到 P。因而，$x$ 属于到 P。

#### 推论{#alg-viii-s1-n1-cor-1 .statement tag=000A}

设 M 为 A-模和 $(M_i)_{i\in I}$ M 的子模的有限族。

a) 如果模 $M_i$ 是阿廷的（分别是诺特），那么它们的和 $\sum_{i\in I}M_i$ 也是。

b) 如果模 $M/M_i$ 是阿廷的（分别是诺特），那么模 $M/\bigcap_{i\in I}M_i$ 也是。

到归纳时，处理$I =\{1,2\}$时的情况就足够了。 模$M_2/(M_1\cap M_2)$，$M_2$的商，与$M/M_1$的子模$(M_1+M_2)/M_1$同构的（I, §4, No. 6，p. 41，定理4）。

在部分a)中，我们假设$M_1$和$(M_1+ M_2)/M_1$是阿廷的（分别是诺特）；同样的情况也适用于$M_1+ M_2$ (命题 3)。

在部分 b)中，我们假设$M/M_2$和$M_2/(M_1\cap M_2)$是阿廷的（分别是诺特）；同样的情况也适用于$M/(M_1\cap M_2)$（前述）。

#### 例 5 {#alg-viii-s1-n1-exa-5 .statement tag=000B}

令$(M_i)_{i\in I}$为A-模的有限族。如果模 $M_i$ 是阿廷的（分别是诺特），那么它们的直和 $\bigoplus_{i\in I}M_i$ 也是。

#### 注 {#alg-viii-s1-n1-rem-1 .statement tag=000C}

定义以及此小节扩展到任意阿贝尔的群的结果，其中叙述中的替换子模具有稳定的子群。

### 2. 阿廷环和诺特环

#### 定义 2 {#alg-viii-s1-def-2 .statement tag=000D}

如果左A-模 $A_s$ 为阿廷的（分别为诺特），则环 A 被称为左阿廷的（分别为左诺特的）。同样，如果右A-模 $A_d$ 为阿廷的（分别为诺特），则环 A 被称为右阿廷（分别为右诺特）。

环 A 是右阿廷（或右诺特）当且仅当其逆环 $A^o$ 是左阿廷的（或左诺特的）。对于交换环 A，左阿廷的和右阿廷重合的性质，当它们成立时，我们说环 A 是阿廷的；我们对“诺特”采用了类似的约定。存在左阿廷的但不是右阿廷的非交换环，以及左诺特的但不是右诺特的非交换环（VIII、p. 14、习题 3）。

设A为环。通过定义，以下性质是等价的：

(i) 环 A 是左阿廷的。

(ii) A 的左理想的每个非空集合按包含排序，具有最小元素。

(iii) A 的每个递减序列左理想都是平稳的。

由于VIII、p. 3的命题 2，以下性质是等价的：

(i) 环 A 是左诺特的。

(ii) A 的左理想中的每个非空集合按包含排序，都有极大元素。

(iii) A 的每个递增序列都是平稳的。

(iv) A 的每个左理想都是由 A 的有限子集生成的。

#### 例 1 {#alg-viii-s1-n2-exa-1 .statement tag=000E}

域是环，即左和右阿廷和诺特。

#### 例 2 {#alg-viii-s1-n2-exa-2 .statement tag=000F}

设 A 为 A 的环和 D 子环。假设 D 为域，A 为 D 上的有限维左向量空间。则环 A 为左阿廷的和左诺特的，因为 A 的每个左理想都是 A 的 D 向量子空间。 代数超过交换域是环，即左和右阿廷和诺特。

#### 例 3 {#alg-viii-s1-n2-exa-3 .statement tag=000G}

主理想整环 (VII, §1, No. 1, p. 1, 定义 1) 为诺特。 整环不是域的 A 也不是阿廷环：对于 A 的每个非零的不可逆元素 $a$，理想 $a^nA$（对于$n\in \mathbf{N}$）的序列是严格递减。 特别是，整数的环$\mathbf{Z}$是诺特，但不是阿廷的。

#### 例 4 {#alg-viii-s1-n2-exa-4 .statement tag=000H}

设M为A-模，即非零的子模的无限族$(M_i)_{i\in I}$的直和。 令 E 为 M 的自同态环。 对于每个$i\in I$，令$\mathfrak{a}_i$（或$\mathfrak{b}_i$）为E 的元素的集合，其中核包含$\sum_{j\not=i}M_j$（或$M_i$中包含像）。 那么$(\mathfrak{a}_i)$是E的非零的左理想的无限族，其和是直接的，$(\mathfrak{b}_i)$是E的非零的右理想的无限族，其和是直接的。 因而，环 E 既不左也不右阿廷（分别为诺特）（VIII、p. 2、例 2）。 特别是，无限维向量空间的自同态环既不左也不左右阿廷（分别为诺特）。

#### 定理 1 {#alg-viii-s1-thm-1 .statement tag=00QW}

设A为左阿廷的环。 A-模$A_s$有有限长度。

我们将在证明中使用以下引理。

#### 引理 3 {#alg-viii-s1-lem-3 .statement tag=000I}

设 A 为环和 $n$ 自然数。 长度$\leqslant n$子模家族的和阿廷的A-模M有有限长度。

我们$n$使用归纳法。首先，假设$n= 1$。如果 M 不是有限长度，那么我们可以为每个 $m\in \mathbf{N}$ 长度 1 的 M 的子模构造序列 $(M_m)_{m\in\mathbf{N}}$ 和$M_m\not\subset (\sum_{i<m}M_i)$。然后，每个$m$就有$M_m\cap \sum_{i<m}M_i= 0$，而家庭$(M_m)_{m\in\mathbf{N}}$的和将是直接的。然而，这个与……矛盾事实上A-模M是阿廷的（VIII，p. 2，例2）。

现在，假设$n\geqslant 2$。设$(M_i)_{i\in I}$为长度$\leqslant n$M子模和和M。对于每一个$i\in I$，长度$M_i$选择子模$M'_i$ $\leqslant n-1$使得$M_i/M'_i$有长度$\leqslant 1$。 集合$M'=\sum M'_i$，并用$M''_i$表示$M''= M/M'$中$M_i$的像。 模$M''_i$是长度$\leqslant 1$，而和是$M''$。 模$M'$和$M''$为阿廷的（VIII、p. 3、命题3）；到归纳假设时，它们的数量为有限长度。因而，M 有有限长度 (II, §1, No. 10, p. 212, 命题 16)。

现在让我们证明定理 1。让$\mathscr{S}$表示A的左理想$\mathfrak{a}$的集合，使得模$A_s/\mathfrak{a}$有有限长度。令 $(\mathfrak{a}_i)_{i\in I}$ 为元素和 $\mathscr{S}$ 的有限族。到 VIII、p. 2、A-模 $A_s/\mathfrak{a}_i$ 的命题 1 时，每$i\in I$ 为阿廷的和诺特。因而，$A_s/\bigcap_{i\in I}\mathfrak{a}_i$是阿廷的和诺特（VIII，p. 4，命题3的推论），因此是有限长度（VIII，p. 2，命题1）。这证明$\mathscr{S}$是包含的左有向集合。由于环 A 是左阿廷的，集合 $\mathscr{S}$ 至少有元素 $\mathfrak{b}$。我们用$n$表示A-模$A_s/\mathfrak{b}$中的长度。

令$x$为$A_s$的元素，且$\mathfrak{a}$为湮没子（II, §1, No. 12，p. 219）。 A-模 $Ax$ 与 $A_s/\mathfrak{a}$ 同构的。如果$Ax$有有限长度，则$\mathfrak{a}$属于到$\mathscr{S}$，所以$\mathfrak{a}$包含于$\mathfrak{b}$和$Ax$有长度$\leqslant n$。因而，有限长度的A的每个单生左理想都有长度$\leqslant n$。令$\mathfrak{c}$为这些理想中的和；这是有限长度的A的左理想乘以引理 3。有限长度的A的每个左理想都是有限长度的单生左理想的和，因此包含在$\mathfrak{c}$中。因而，$\mathfrak{c}$是有限长度的A的最大的左理想。

如果 $\mathfrak{c}$ 与 A 不同，则包含 $\mathfrak{c}$ 的左理想的集合且与 $\mathfrak{c}$ 不同，将具有最小元素 $\mathfrak{c}'$。那么A-模$\mathfrak{c}'/\mathfrak{c}$将有长度1，$\mathfrak{c}'$将有有限长度，与……矛盾事实上$\mathfrak{c}$是最大的。因此我们有 $\mathfrak{c}= A$； A-模$A_s$有有限长度。

#### 推论 {#alg-viii-s1-n2-cor-1 .statement tag=000J}

每个左阿廷的环就是左诺特的。

设 A 为左阿廷的环。到定理 1，A-模 $A_s$ 已有限长度。然后我们应用命题 1 of VIII, p. 2。

设 A 为左（或右）阿廷环； A-模 $A_s$（或$A_d$）（I, §4, No. 7，p. 44）的长度称为环 A 的左（或右）长度。当 A 是交换律阿廷环时，这两个长度重合，简称为A的长度。当A左且右阿廷不可交换时，A的左与右长度不一定相等（VIII、p. 14、习题3）。

#### 例 5 {#alg-viii-s1-n2-exa-5 .statement tag=000K}

域的左边和右长度等于1。

#### 命题 4 {#alg-viii-s1-prop-4 .statement tag=000L}

a) 设 A 为左诺特环，M 为有限生成的左A-模。 模 M 是诺特，M 的每一个子模都是有限生成的。

b) 设 A 为左阿廷的环，M 左A-模。以下性质是等价的： 模 M 是有限生成的； 模 M 为阿廷的； 模 M 有有限长度； 模 M 是诺特。

让我们证明a）。 M 的每个单生子模都同构于商 $A_s$，因此是诺特乘以 VIII、p. 3 的命题 3。 模 M 是这样的子模的有限和；因而，通过命题 3 的推论 (VIII, p. 4) 得到诺特。然后，M 的每个子模都是有限生成的 (VIII, p. 3, 命题 2)

现在，假设环 A 是左阿廷的。我们看到，就像前面的截面一样，如果A-模 M是有限生成的，那么它就是阿廷的。如果它是阿廷的，那么它有有限长度：事实上，它的单生子模与$A_s$的商同构，因此有限长度小于$A_s$，并且断言从引理3得出。每模有限长度是诺特，并且每个诺特模都是有限生成的。这证明了b)。

#### 命题 5 {#alg-viii-s1-prop-5 .statement tag=000M}

a) 设 A 为左阿廷的（分别为左诺特的）环，并令 $\varphi : A\rightarrow B$ 为环同态，这使得 B 成为有限生成的左A-模。 环 B 为左阿廷的（分别为左诺特的）。

b) 设A为左阿廷的（分别为左诺特的）环，并令$\mathfrak{a}$为A的两侧理想； 环 $A/\mathfrak{a}$ 是左阿廷的（分别是左诺特的）。

c) 令$(A_i)_{i\in I}$为左阿廷的（分别为左诺特的）环的族。 环 $\prod_{i\in I}A_i$ 是左阿廷的（分别是左诺特的）。

我们将处理阿廷环的情况； 诺特环的情况类似。

让我们证明a）。到命题 4 时，环 $B_s$ 为阿廷的左A-模和更不必说阿廷的左B-模。

断言 b) 从断言 a) 得出，应用于从 A 到 $A/\mathfrak{a}$ 的典范同态。

让我们证明c）。 集合$A =\prod_{i\in I}A_i$。 到假设，$(A_i)_s$是阿廷的左$A_i$-模块和更不必说阿廷的左A-模。 VIII、p. 4、A-模$A_s$中的例 5 为阿廷的。

#### 推论{#alg-viii-s1-n2-cor-2 .statement tag=000N}

阿廷的交换环的素理想是它的极大理想。

在任何交换环中，最大理想是素数。设A为阿廷的交换环。令 $\mathfrak{p}$ 为 A 的素理想。环 $A/\mathfrak{p}$ 为整环，为阿廷的 (命题 5)，因此为域 (VIII, p. 5, 例 3)。因而，理想的 $\mathfrak{p}$ 是最大的。

多项式环$\mathbf{Q}[(X_n)_{n\in\mathbf{N}}]$为整环； it is not 诺特 (or 阿廷的) (VIII, p. 15, 习题 9). It is 子环 of its 域 of 分数, which is 阿廷的 (and 诺特) 环.

### 3. Countermodule

#### 定义 3 {#alg-viii-s1-def-3 .statement tag=000O}

设 A 为 M 的环，M A-模，E = End$_A(M)$ 自同态环。M 的对模是左 E 模块，其底层加法群与 M 和外法则 $(c, x)\mapsto c(x)$ 相同。

设 Z 为环 A 的中心。对于 E 的每个 $a\in Z$、位似 $a_M$ 属于。因而，E 被规范地赋予 Z 代数的结构。特别是，如果 M 是有限生成的 Z 模，则 M 的对模是有限生成的。

#### 引理 4 {#alg-viii-s1-lem-4 .statement tag=000P}

设 M 为左A-模，且对模是有限生成的。存在自然数$m$和从$(A_M)_s$到$M^m$的单射$A_M$线性映射。

集合 E = 结束$_A(M)$。令$(x_1, . . . , x_m)$为E模M的有限生成族。映射$\varphi :a\mapsto (ax_1, . . . , ax_m)$从$(A_M)_s$到$M^m$是$A_M$线性。令$a$为$A_M$的元素，使得$\varphi (a) = 0$。 M 的元素 $x$ 的集合，使得 $ax= 0$ 是 M 包含于 $x_1, . . . , x_m$ 的 E 子模，因此等于 M，这意味着 $a= 0$。

#### 命题 6 {#alg-viii-s1-prop-6 .statement tag=000Q}

令 M 为阿廷的（分别为诺特）左A-模，并有限生成对模。 M 的同位$A_M$ 的环为左阿廷的（分别为左诺特的）。

这是从VIII、p. 3 的引理 4 和命题 3 得出的。

#### 推论{#alg-viii-s1-n3-cor-1 .statement tag=000R}

设A为交换环。

a) 设 M 为诺特 A-模。 环$A_M$是诺特。

b) 令 M 为 A-模或有限长度。 环$A_M$是阿廷的。

设M为A-模。在a)或b)的假设下，A-模M是有限生成的。由于A是可交换的，$A_M$包含在环End$_A$(M)中，因此M的对模是有限生成的。那么就足以应用命题 6。

#### 注 {#alg-viii-s1-n3-rem-1 .statement tag=000S}

设A为环。有限生成对模的阿廷的左A-模 M 有有限长度：事实上，M 的同位$A_M$的环是左阿廷的（命题 6），并且M是阿廷模超过$A_M$；通过VIII、p. 7、命题 4、模 M 的有限长度超过$A_M$，因此也超过 A。

特别是，每个在交换环上有限生成的阿廷模都有有限长度。相比之下，在非交换环上有限生成的阿廷模不一定是有限长度 (VIII, p. 16, 习题 12)。

### 4. 系数为诺特环的多项式

设A为环A的环、$\sigma$自同态、以及满足关系的加法群$d$自同态

$$
d(ab) =\sigma (a)d(b) +d(a)b \tag{1}
$$

对于所有$a, b\in A$。在其他字中，$d$是推导从环A到$(A$，A)-双模，将A的加法群赋予作用$(a, x)\mapsto \sigma (a)x$的左律和律的右律作用$(x, a)\mapsto xa$。我们有$d(1) = 0$（III, §10, No. 5、p. 557、命题 3）。

回想一下 (IV, §1, No. 1, p. 2)，A[X] 表示系数在 A 中的一个变量中的多项式的 $\mathbf{Z}$ 模$A\otimes_{\mathbf{Z}}\mathbf{Z}[X]$。我们赋予它左A-模的自然结构。对于A[X]来说，家庭$(X^n)_{n\in\mathbf{N}}$是基，超过A。我们认同A及其像低于映射$a\mapsto a\otimes 1$。

#### 命题 7 {#alg-viii-s1-prop-7 .statement tag=00QX}

Let A$,\sigma ,d$ be as above. 群 A[X] 上存在唯一的环结构，具有以下属性：

a) 环中的加法是A[X]通常的加法。

b) 乘法 in this 环扩展 that of A.

c) 乘积 in this 环 of 序列 $(a,X, . . . ,X)$, 由……组成 of 元素 $a$ of A followed by $n$ 项 equal to X, is the polynomial $aX^n$.

d) 在这个环中，每$a\in A$有$Xa=\sigma (a)X +d(a)$。

令 E 为加法群 A[X] 的自同态环。 映射 that sends $a\in A$ to 位似 $a_M$ of 左A-模 M = A[X] is 环同态 from A to E. Consider 元素 $u,\sigma_M$, and $d_M$ of E defined by $u(\sum b_nX^n) =\sum b_nX^{n+1},\sigma_M(\sum b_nX^n) =\sum\sigma (b_n)X^n$，$d_M(\sum b_nX^n) =\sum d(b_n)X^n$。 For every $a\in A$, we have

$$
u a_M=a_Mu ,\sigma_Ma_M=\sigma (a)_M\sigma_M,d_Ma_M=\sigma (a)_Md_M+ (d(a)_M) \tag{2}
$$

集合

$$
X_M=\sigma_Mu+d_M \tag{3}
$$

从 (2) 可以看出，对于每 $a\in A$，我们有

$$
X_Ma_M=\sigma (a)_MX_M+ (d(a)_M) \tag{4}
$$

Consider 映射 $\varphi : A[X]\rightarrow E$ defined by

$$
\varphi (\sum a_nX^n)=\sum(a_n)_M(X_M)^n \tag{5}
$$

这是群同态。 归纳论证表明，对于每个 $n\in \mathbf{N}$，我们有 $(X_M)^n(1) = X^n$。因而，对于每个$P\in A[X]$，我们都有$\varphi (P)(1) = P$，这证明同态$\varphi$是单射的。我们将其像记为B。集合B是E的子群；它包含 1，并且在左乘法下通过$a_M$对于$a\in A$和$X_M$是稳定的（参见（4））。 It is therefore 子环 of E. The unique 环结构 on A[X] derived from that on B by transfer of 结构 via $\varphi$ has the properties of 命题 7, where 性质 d) results from 关系 (4).

If A[X] is endowed with 环结构 that has the properties of 命题 7, then the left 位似 $\boldsymbol{\gamma }_X$ of this 环 (I, §8, No. 1, p. 97) necessarily sends $bX^n$ to $\sigma (b)X^{n+1}+d(b)X^n$ 对于 $b\in A$ 和 $n\in \mathbf{N}$，因此等于 $X_M$。对于每个 $a\in A$，位似 $\boldsymbol{\gamma }_a$ 必然等于 $a_M$。因而，每 $P\in A[X]$ 就有 $\boldsymbol{\gamma }_P=\varphi (P)$； 唯一性 in 命题 7 follows.

集合 A[X], endowed with the unique 环结构 with the properties of 命题 7, is denoted by $A[X]_{\sigma ,d}$ and called 多项式环 in X with coefficients in A, relative to $\sigma$ and $d$。 We simply denote it by $A[X]_{\sigma}$ when $d$ is 零映射 and by A[X] when, moreover, $\sigma$ is 恒等映射 on A. This 记号 is compatible with that introduced in IV, §1, No. 1, p. 1 for 交换环 A.

#### 注 {#alg-viii-s1-n4-rem-1 .statement tag=000T}

环 $A[X]_{\sigma ,d}$ has the following 泛性质: given 环 $A'$, 环同态 $f: A\rightarrow A'$, and 元素 $x$ of $A'$ such that $xf(a) =f(\sigma (a))x+f(d(a))$ 对于每个 $a\in A$，都存在一个唯一的环同态 $g: A[X]_{\sigma ,d}\rightarrow A'$，扩展 $f$ 和映射 X 到 $x$。

唯一性很清楚。因而，让我们证明由 $g(\sum a_nX^n) =\sum f(a_n)x^n$ 定义的映射 $g: A[X]_{\sigma ,d}\rightarrow A'$ 具有所需的属性。它扩展$f$，映射X到$x$，并且是群同态。我们有$g(1) = 1$。对于$A[X]_{\sigma ,d}$中的$a\in A$和$Q =\sum a_nX^n$，我们有

$$
g(aQ) =g(\sum aa_nX^n)=\sum f(aa_n)x^n=f(a)\sum f(a_n)x_n=g(a)g(Q)
$$

以及

$g$(XQ) $=g(\sum (\sigma (a_n)X^{n+1}+d(a_n)X^n))$

$$
=\sum(f(\sigma (a_n))x^{n+1}+f(d(a_n))x^n) =x\sum f(a_n)x^n=g(X)g(Q)
$$

由此可见，对于 $A[X]_{\sigma ,d}$ 中的 $P,Q$，我们有 $g(P)g(Q) =g$(PQ)，因而 $g$ 是环同态。

#### 定理 2 {#alg-viii-s1-thm-2 .statement tag=000U}

设A为左诺特环，设$\sigma$为A的自同构和满足关系的加法群$d$自同态(1)。 环$A[X]_{\sigma ,d}$为左诺特的。

集合$B = A[X]_{\sigma ,d}$。对于任何整数$n\geqslant 0$，我们用形式$a_0+a_1X +\cdots +a_nX^n$B元素$B_n$集合来表示。它是B的左A-子模。由$\varphi_n(a_0+a_1X +\cdots +a_nX^n) =a_n$定义的映射$\varphi_n: B_n\rightarrow A_s$是A线性的。

令 $\mathfrak{b}$ 为 B 的左理想。对于每个整数 $n\geqslant 0$，集合 $\mathfrak{a}_n=\varphi_n(\mathfrak{b}\cap B_n)$ 为 A 的左理想。由于对于每个 $a\in A$，我们有 $Xa=\sigma (a)X +d(a)$，因此我们有

(6)$\varphi_{n+1}$(XQ)$=\sigma (\varphi_n(Q))$

对于每个$Q\in B_n$，因而$\sigma (\mathfrak{a}_n)\subset \mathfrak{a}_{n+1}$。因而，A 的理想序列 $\mathfrak{a}'_n=\sigma^{-n}(\mathfrak{a}_n)$ 为递增。由于环 A 是左诺特的，因此存在整数 $m\geqslant 0$，这样我们就有 $\mathfrak{a}'_n=\mathfrak{a}'_{n+1}$ 对应 $n\geqslant m$。由于 $\sigma$ 是满射，所以我们有关系

$$
\sigma (\mathfrak{a}_n) =\mathfrak{a}_{n+1} \tag{7}
$$

每整数 $n\geqslant m$。

令$\mathfrak{c}$为由$\mathfrak{b}\cap B_m$生成的B的左理想。由于左A-模 $B_m$ 是有限生成的且环 A 是左诺特的，因此左A-模 $\mathfrak{b}\cap B_m$ 是有限生成的（VIII、p. 7、命题 4 a)）。因而，左理想$\mathfrak{c}$是由B的有限子集生成的。显然它包含在$\mathfrak{b}$中。让我们证明它等于$\mathfrak{b}$乘证明乘归纳，对于每个整数$n\geqslant 0$，我们有

$$
\mathfrak{b}\cap B_n\subset \mathfrak{c} \tag{8}
$$

对于$n\leqslant m$，关系 (8) 到构造成立。从现在开始，我们假设$n$是整数$\geqslant m$，使得$\mathfrak{b}\cap B_n\subset \mathfrak{c}$。令 P 为 $\mathfrak{b}\cap B_{n+1}$ 的元素。然后$\varphi_{n+1}(P)$属于到$\mathfrak{a}_{n+1}=\sigma (\mathfrak{a}_n)$，因此存在$\mathfrak{b}\cap B_n$的元素Q使得$\varphi_{n+1}(P) =\sigma (\varphi_n(Q))$。 集合$R = P-$XQ。因为关系(6)，我们有$\varphi_{n+1}(R) = 0$，即$R\in B_n$。由于 P 和 Q 属于到 B 的左理想$\mathfrak{b}$，因此对于 R 也是如此；因而，R 和 Q 属于到 $\mathfrak{b}\cap B_n$，其中归纳假设包含在理想 $\mathfrak{c}$ 中。因而，P 属于至 $\mathfrak{c}$。这证明我们有$\mathfrak{b}\cap B_{n+1}\subset \mathfrak{c}$。

由此可知$\mathfrak{b}$等于$\mathfrak{c}$；因此它是 B 的有限生成理想。这证明环 B 是左诺特的。

如果环 A 的自同态 $\sigma$ 不是自同构，则环 $A[X]_{\sigma ,d}$ 不一定是左诺特的，即使 A 是诺特交换环 (VIII, p. 22, 习题26)。

#### 推论 1（希尔伯特）{#alg-viii-s1-thm-2-cor-1 .statement tag=00RW}

设 A 为诺特交换环。对于每个整数 $n\geqslant 0$，多项式代数 $A[X_1, . . . ,X_n]$ 为诺特环。

接下来是定理 2 中的归纳，考虑到 III, §2, No. 9、p. 453 中的命题 8。

#### 推论 2 {#alg-viii-s1-thm-2-cor-2 .statement tag=000V}

设 A 为诺特交换环。由有限多个元素生成的交换A-代数是诺特环。

这样的代数同构于形式$A[X_1, . . . ,X_n]/\mathfrak{a}$的代数，其中$n\geqslant 0$和$\mathfrak{a}$是$A[X_1, . . . ,X_n]$的理想。然后我们应用VIII、p. 7的推论1和命题5。

#### 推论 3 {#alg-viii-s1-thm-2-cor-3 .statement tag=000W}

每个交换环都是诺特子环右向有向族的并。

事实上，令 A 为交换环。由有限多个元素生成的A的子环（作为$\mathbf{Z}$-代数）是由推论2得出的诺特。它们形式是A的子环的右有向族，其中并A。

### 习题{#alg-viii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
