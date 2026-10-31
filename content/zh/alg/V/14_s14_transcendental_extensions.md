---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 14
section_title: Transcendental extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.106-A V.118, A V.171-A V.175
pdf_pages: 0220-0232, 0285-0289
extraction: ocr
subsections:
    - "no": 1
      title: Algebraically free families. Pure extensions
      page: 106
      pdf_page: 220
    - "no": 2
      title: Transcendence bases
      page: 107
      pdf_page: 221
    - "no": 3
      title: The transcendence degree of an extension
      page: 110
      pdf_page: 224
    - "no": 4
      title: Extension of isomorphisms
      page: 111
      pdf_page: 225
    - "no": 5
      title: Algebraically disjoint extensions
      page: 112
      pdf_page: 226
    - "no": 6
      title: Algebraically free families of extensions
      page: 115
      pdf_page: 229
    - "no": 7
      title: Finitely generated extensions
      page: 117
      pdf_page: 231
statements: 51
exercises: 20
content_sha256: d345c4566a50d003dc75301c38f0fa484678ae426223c8dcdea1c4b141fb06a5
translated_from: content/en/alg/V/14_s14_transcendental_extensions.md
translation_method: google
source_content_sha256: 36caeafec2b80f55f4d81aa8a08ac8e916c9c8c954ea1d9374f4336f63f99e7d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: c9f21829cc98db6a0b54e92470b54cf34450a6363f3e0db39aa799968785e59f
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 14。超越扩张

### 1. 代数自由族。纯扩张

让我们回忆一下 (IV, p. 4) 以下定义：

#### 定义 1 {#alg-v-s14-def-1 .statement tag=06RO}

*设E为域K中的扩张；如果关于 $x_i$（对于 $a = (\alpha_i)_{i \in I}$，在 $\mathbf{N}^{(I)}$）的单项式 $\mathbf{x}^a = \prod_{i \in I} x_i^{a_i}$ 在 K 上线性独立，则 E 的元素的族 $\mathbf{x} = (x_i)_{i \in I}$ 被认为在 K 上是代数自由的。反之，该族被称为在 K 上代数相关。*

定义1也可以表示如下：

#### 命题 1 {#alg-v-s14-prop-1 .statement tag=06RP}

*For a family $(x_i)_{i \in I}$ of elements of an extension E of a field K to be algebraically free over K it is necessary and sufficient for the relation $f((x_i)) = 0$, where $f$ is a polynomial in $K[X_i]_{i \in I}$, to imply $f = 0$.*

#### 定义 2 {#alg-v-s14-def-2 .statement tag=06RQ}

*设 E 为域 K 的扩张。如果 E 的元素的 $(x_i)_{i \in I}$ 族被称为 E 的纯基（在 K 上），如果它是代数自由且 $E = K(x_i)_{i \in I}$。 K 的扩张 E 也称为纯的，如果它具有纯基。*

空族在代数上是自由的，因此 K 本身是纯扩张。具有记号的 Def。 2、每个元素$x_i$都超越于K；如果 $I$ 非空，则 E 是 K 的超越扩张。

#### 命题 2 {#alg-v-s14-prop-2 .statement tag=06RR}

*设E和$E'$是E的子域K的两个域和u同构到$E'$的子域$K'$。令$\mathbf{x} = (x_i)_{i \in I}$（或$\mathbf{x}' = (x'_i)_{i \in I}$）为E（或$E'$）的元素族，它在K（或$K'$）上是代数自由的。然后存在一个唯一的$L = K(x_i)_{i \in I}$到$L' = K'(x'_i)_{i \in I}$的同构$v$，对于每个$i \in I$，$K$有诱导$u$，映射$x_i$到$x'_i$。

$v$的唯一性清晰。让我们放置$A = K[x_i]_{i \in I}$和$A' = K'[x'_i]_{i \in I}$。通过假设，向量 K 空间$A$ 的单项式$x'' = \prod_{i \in I} x_i^{\alpha_i}$（对于$\alpha = (\alpha_i)_{i \in I}$，在$\mathbf{N}^{(I)}$）形式基，还有$A'$ 的类似性质。因此，存在环同构$w : A \to A'$映射每个元素$\sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha x^\alpha$到$\sum_{\alpha \in \mathbf{N}^{(I)}} u(c_\alpha) {x'}^\alpha$。由于$L$是$A$的分数的域和$L'$是$A'$的同构$w$扩展到同构$v$ 域$L$到域$L'$。

#### 推论{#alg-v-s14-n1-cor-1 .statement tag=06RS}

— *为了使域 K 的扩张 E 是纯的，E 在 K 上与有理分式的域 K 同构是必要且充分的。更准确地说，如果族 $(x_i)_{i \in I}$ 是 E 的纯基，则存在 $K(X_i)_{i \in I}$ 在 E 上的唯一 K 同构的，其中每个 $i \in I$ 映射 $X_i$ 至 $x_i$。*

#### 注 {#alg-v-s14-n1-rem-1 .statement tag=06RT}

很明显，在 K 的扩张 E 中，K 上的代数自由族由 $K$ 上的*线性独立* 元素组成（因此成对不同）；在其他字中，它也是$E$的*向量空间* 结构的自由族（相对于K）。但逆命题是假的，因为如果E是K的代数扩张，则E的元素的任何非空族（以及*更不必说* K上线性无关的元素的非空族）在K上永远不会在代数上自由。当存在混淆的风险时，我们应该说子集是K 的扩张 E 对于 E 的向量空间结构相对于 K 是自由的，在 K 上是“线性自由”。

令 E 为域 K 的扩张。如果 S 的恒等映射定义的族本身是代数自由的，则 E 的子集 S 被称为“代数自由”（超过 $K$）。 E 的代数自由子集的元素也称为“代数独立”。如果 E 的子集不是代数自由的，则称其“代数相关”，并且其元素是“代数相关”。对于 E 的元素的族 $(x_i)_{i \in I}$ 来说，要实现代数自由，$i \mapsto x_i$ 应该是 I 的双射到 E 的代数自由的子集上，这是充分必要的。

代数自由的集合的每个子集都是代数自由的。此外：

#### 命题 3 {#alg-v-s14-prop-3 .statement tag=06RU}

— *对于$(x_i)_{i \in I}$、扩张 E、域 K 的元素族在 K 上代数上自由，$(x_i)_{i \in I}$ 的每个有限子族在 K 上代数上自由是必要且充分的。*

这个命题紧接着 Def. 1.

### 2.超越基

#### 命题 4 {#alg-v-s14-prop-4 .statement tag=06RV}

— *令 E 为域 K 的扩张，S 和 T 为 E 的两个子集。那么以下性质是等价的：
a) $S \cup T$ 在 K 和 $S \cap T = \varnothing$ 上是代数自由的。*

b) $S$ 在$K$ 上是代数自由的，$T$ 在$K(S)$ 上是代数自由的。
c) $T$ 在$K$ 上是代数自由的，$S$ 在$K(T)$ 上是代数自由的。

显然只要证明a)和b)是等价的就足够了。

$a) \Rightarrow b)$：假设a)成立。由于$S$包含在$S \cup T$中，因此它在$K$上是代数自由的。如果$T$在$K(S)$上不是代数自由的，则存在（命题3）$T$的不同元素的有限族$(y_j)_{1 \leq j \leq n}$，它在$K(S)$上代数相关。因此，环$K(S)[Y_1, ..., Y_n]$中存在非零多项式$f$，使得$f(y_1, ..., y_n) = 0$；如果需要的话，之后乘以$f$乘以$K[S]$的非零元素，我们可以假设所有系数都在属于到$K[S]$。 $S$ 的不同元素 $x_i \ (1 \leq i \leq m )$ 的有限数中的票价多项式系数，系数为 $K$。 元素 $x_1, ..., x_m, y_1, ..., y_n$ 成对不同，因为 $S \cap T = (21$。 关系 $f(y_1, ..., y_n) = 0$ 可以写成

$$
g(x_1, ..., x_m ; y_1, ..., y_n) = 0 ,
$$

其中 $g$ 是 $K[X_1, ..., X_m, Y_1, ..., Y_n]$ 的非零多项式，并且关系与……矛盾假设 $S \cup T$ 是代数自由的。

$b) \Rightarrow a)$：假设b)成立。首先很明显$T \cap K(S) = \varnothing$和$a fortiori \ S \cap T = (21$。只要证明 $x_i \ (1 \leq i \leq m )$ 与 $S$ 不同的元素，在数中有限，并且 $y_j \ (1 \leq j \leq n )$ 与 $T$ 不同的元素在数中有限，则 $x_i$ 的集合和$y_j$ 在$K$ 上是代数自由的（命题 3）。考虑一个多项式 $f \in K[X_1, ..., X_m, Y_1, ..., Y_n]$ 使得 $f(x_1, ..., x_m, y_1, ..., y_n) = 0$ 并将 $f = \sum \varphi_\alpha Y_1^{\alpha_1} ... Y_n^{\alpha_n}$ 与 $\varphi_\alpha \in K[X_1, ..., X_m]$ 对于所有 $\alpha = (\alpha_1, ..., \alpha_n) \in \mathbf{N}^n$。让$g = f(x_1, ..., x_m, Y_1, ..., Y_n)$；那么$g$是环$K[S][Y_1, ..., Y_n]$的多项式，关系$f(x_1, ..., x_m, y_1, ..., y_n) = 0$可以写成$g(y_1, ..., y_n) = 0$。由于$T$在$K(S)$上是代数自由的，$g$的每个系数$\varphi_\alpha(x_1, ..., x_m)$都是零；由于$S$在$K$上是代数自由的，因此对于所有$\alpha \in \mathbf{N}^n$我们有$\varphi_\alpha = 0$，因此$f = 0$。

#### 推论 {#alg-v-s14-n2-cor-1 .statement tag=06RW}

— *令 E 为域 K 的扩张和 E 的 S 子集，它在 K 上代数上自由。如果 x \in E 在 K(S) 上超越，则 S U {x} 在 K 上代数上自由。*

#### 命题 5 {#alg-v-s14-prop-5 .statement tag=06RX}

— *令 E 为域 K 的扩张。为了使 E 的子集 S 在 K 上是代数自由的，对于 S 中的每个 x \in，元素 x 应超越域 K(S - {x}) 是必要且充分的。*

根据命题 4，条件是必要的。

为了证明充分性，只需证明 $S$ 的不同元素中的每个有限序列 $(x_1, ..., x_n)$ 是代数自由的就足够了（命题 3）。现在假设$x_i$超越$K(x_1, ..., x_{i-1})$对于$1 \leq i \leq n$，现在我们的断言跟随来自Cor的$n$上的归纳。到提案 4。

#### 命题 6 {#alg-v-s14-prop-6 .statement tag=06RY}

— *令 E 为域 K 的扩张，且 X 是 E 在 K 上的代数自由的子集。如果 K' \子集 E 是 K 的代数扩张，则 X 在 K' 上是代数自由的。*

通过矛盾论证，我们假设 X 在代数上与 K' 相关。根据命题 5，存在元素 $x \in X$，它是域 $K'(M)$ 的代数，其中 $M = X - \{x\}$。由于 $K'(M) = K(M)(K')$ 和 $K'$ 是 $K$ 上的代数，Cor. V、p. 18的2表明$K'(M)$是$K(M)$的代数；由于$x$是$K'(M)$的代数，因此根据V、p. 19的命题3，它也是$K(M) = K(X - \{x\})$的代数。现在，第 5 条命题表明 X 在 K 上是代数相关的，我们有一个矛盾。

#### 定义 3 {#alg-v-s14-def-3 .statement tag=06RZ}

* 扩张 E 域 K 的子集 B 是 E 的超越基（在 K 上），如果 B 在 K 上是代数自由的且 E 在 K(B) 上是代数的。*

#### 例 {#alg-v-s14-n2-exa-1 .statement tag=06S0}

— *纯粹的基是一种超越基。另一方面，如果 E 是 K 的纯扩张，则 E 对 K 的超越基并不总是 E 的纯基。对于例，在 $K(X)$ 中，$\{X^2\}$ 是超越基，但不生成$K(X)$.*

#### 命题 7 {#alg-v-s14-prop-7 .statement tag=06S1}

*设 E 为域 K 的扩张。E 的每个超越基都是 E 的子集集合（按包含排序）的极大元素，在代数上自由于 K。相反，如果 S 是 E 的子集，则 E 为超过 $K(S)$ 的代数，S 的每个最大代数自由子集都是 E 的超越基。*

设 B 是 E 对 K 和 $x \in E - B$ 的超越基。那么$x$是$K(B)$的代数；由V，p. 107，命题4，E 的子集$B \cup \{x\}$ 在K 上不是代数自由的，从而命题的第一个部分。其次，如果 E 是超过 $K(S)$ 的代数，并且 B 是 S 的最大代数自由部分，则可以从 Cor 得出。命题4的每一个$x \in S$都是$K(B)$上的代数；因此 (V, p. 18, Cor. 1) $K(S)$ 是$K(B)$ 上的代数，因此 (V, p. 19, 命题 3)，E 是$K(B)$ 上的代数。

#### 定理 1（斯坦尼茨）{#alg-v-s14-thm-1 .statement tag=06S2}

— *域 K 的每个扩张 E 都承认对 K 的超越基。在其他字中，域 K 的每个扩张都是 K 的纯扩张的代数扩张。*

相比之下，扩张并不总是代数扩张的纯扩张（V，p. 171，例2）。

这个定理是以下更精确结果的推论：

#### 定理 2 {#alg-v-s14-thm-2 .statement tag=06S3}

*设 E 为域 K 的扩张，E 的 S 子集，使得 E 在 $K(S)$ 上是代数，S 的 T 子集在 K 上是代数自由的；那么存在 E 对 K 的超越基 B，使得 $T \subset B \subset S$.*

对于 S 的代数自由子集的集合，按包含排序，是根据命题 3 的有限特征标 (E, III, p. 34) 的集合。 E, III, p. 35 的 1 有极大元素 B 包含 T，并且根据命题 7，B 是 E 对 K 的超越基。

#### 推论 (« 交换定理 ») {#alg-v-s14-n2-cor-2 .statement tag=06S4}

— 令 E 为 K 的扩张，E 的 S 子集，使得 E 在 K(S) 上是代数，E 的 T 子集在 K 上是代数自由的；则存在 S 的子集 S'，使得 T ∪ S' 是 E 对 K 的超越基，并且 T ∩ S' = ∅。

因为 E 是 K(T U S) 上的代数，并且我们有 T ⊂ T U S。

### 3. 扩张的超越次数

#### 定理 3 {#alg-v-s14-thm-3 .statement tag=06S5}

— 令 E 为域 K 的扩张。E 对 K 的所有超越基具有相同的基数。

只要证明不等式 Card(B) ≥ Card(B')，当B和B'是E对K的两个超越基时，我们可以假设B'不为空。我们首先假设 B 是有限的并且使用归纳法位于其基数 n 上；对于 n = 0，E 是 K 上的代数，B' 为空。现在假设 n ≥ 1；给定 x ∈ B'，交换定理提供 B 的子集 C，使得 x ∉ C 和 {x} U C 是 E 对 K 的超越基；根据命题 7 从而卡 C < n，我们有 C ≠ B。让 K_1 = K(x) 且 C' = B' - {x}；那么 C 和 C' 在域 K_1 (V, p. 107, 命题 4) 上是代数自由的，并且 E 在 K_1(C) = K(C U {x})) 和 K_1(C') = 上都是代数的K(B')。在其他字中，C和C'是E对K_1的两个超越基。由于 Card(C) < n，归纳假设意味着不等式 Card(C') ≤ Card(C) ≤ n - 1，从而 Card(B') ≤ n = Card(B)。

现在假设 B 是无限的。每个 x ∈ B 都是 K(B') 上的代数，因此存在 B' 的有限子集 S(x)，使得 x 是 K(S(x)) 上的代数。写 S = U_{x ∈ B} S(x)，则 S ⊂ B' 并且由于 B 是无限的，所以我们有 Card(S) ≤ Card(B) (E, III, p. 49, Cor. 3)。但由于 B 的每个元素都是 K(S) 上的代数，并且 E 都是 K(B) 上的代数，因此我们结论 E 是 K(S) 上的代数（V，p. 19，命题 3）。现在，第 7 条命题意味着 S = B'，从而所需的不等式 C​​ard(B') ≤ Card(B)。

#### 定义 4 {#alg-v-s14-def-4 .statement tag=06S6}

— 令 E 为域 K 的扩张。E 对 K 的每个超越基的基数称为 E 对 K 的超越次数，写作 tr。 deg_K E。

Th。 2 和 3 以及 Def。 4 意味着以下推论，其中 E 表示域 K 的扩张，有限超越次数 n。

#### 推论 1 {#alg-v-s14-def-4-cor-1 .statement tag=06S7}

— 令 S 为 E 的子集，使得 E 是 K(S) 上的代数。则 Card(S) ≥ n；如果 S 的基数等于 n，则 S 在 K 上是代数自由的（因此它是 E 对 K 的超越基）。

#### 推论 2 {#alg-v-s14-def-4-cor-2 .statement tag=06S8}

— 假设 E = K(x_1, ..., x_m)，则 m ≥ n；此外，如果 m = n，则 (x_1, ..., x_m) 是 E 在 K 上的纯基，并且 E 是 K 的纯扩张。

#### 推论 3 {#alg-v-s14-def-4-cor-3 .statement tag=06S9}

— $E$ 的每个子集在 $K$ 上是代数自由的，至多有 $n$ 元素，并且如果它恰好有 $n$ 元素，则它是 $E$ 在 $K$ 上的超越基。

#### 定理 4 {#alg-v-s14-thm-4 .statement tag=06SA}

— 令$K, E$和$F$为三个域，使得$K \subset E \subset F$。如果$S$是$E$对$K$的超越基，$T$是$F$对$E$的超越基，则$S \cap T$为空，$S \cup T$为超越基中的 $F$ 超过 $K$。

因为$F$是$E(T)$的代数；此外，$E(T)$是域$K(S \cup T) = K(S)(T)$的代数，因为$E$是$K(S)$的代数（$V$，p. 18，Cor.2）；因此 ($V$, p. 19, 命题 3) $F$ 是$K(S \cup T)$ 上的代数。另一方面，$T$在$E$上是代数自由的，因此$a fortiori$在$K(S)$上是代数自由的，因此（$V$，p. 107，命题4）$S \cup T$在$K$和$S \cap T = \varnothing$上是代数自由的。

#### 推论{#alg-v-s14-n3-cor-1 .statement tag=06SB}

— 令$K, E$和$F$为三个域，使得$K \subset E \subset F$。然后我们有
$$
\text{tr. deg}_K F = \text{tr. deg}_K E + \text{tr. deg}_E F
$$

### 4. 扩张 / 同构

#### 命题 8 {#alg-v-s14-prop-8 .statement tag=06SC}

— 令$\Omega$为域、$K$、$E$和$F$的代数闭扩张，$\Omega$和$u$的两个子扩展，$E$到$F$的$K$同构。为了使$O$存在扩展$u$的$K$自同构$v$，$\Omega$对$E$和$F$具有相同的超越性次数是必要且充分的。

条件显然是必要的。

假设$\Omega$对$E$和$F$具有相同的超越次数，并且让我们选择对$\Omega$对$E$的超越基$B$和超越基 $\Omega$ 中的$C$ 超过$F$。由于 $B$ 和 $C$ 等价，命题 2 ($V$, p. 106) 表明 $u$ 扩展是 $E(B)$ 到 $F(C)$ 的 $K$ 同构 $u'$。由于 $C?$ 是 $E(B)$ 和 $F(C)$ 的代数闭包，因此 Cor. $V$、p. 23表示$\Omega$的$u'$扩展到自同构$v$。

#### 推论 1 {#alg-v-s14-prop-8-cor-1 .statement tag=06SD}

— 令$O$为域$K$的代数闭扩张，并且$E$为$\Omega$的子扩展。 $E$扩展的每个$K$自同构到$\Omega$的$K$自同构。

#### 推论 2 {#alg-v-s14-prop-8-cor-2 .statement tag=06SE}

— 令$\Omega$为域、$K$、$E$和$F$的代数闭扩张，$\Omega$和$u$的两个子扩展，$E$的$K$同构到$F$。如果$E$在$K$上的超越次数是有限的（特别是如果$E$是$K$上的代数），则存在$\Omega$延伸$u$的$K$自同构。

让我们用$n, d(E)$和$d(F)$分别表示$E$对$K$的超越次数、$O$对$E$的超越以及$C?$对$F$的超越。 $K$同构$u$的存在表明，$F$对$K$的超越次数等于$n$。由科。的 Th。 4 $\Omega$对$K$的超越次数等于$d(E) + n$，也等于$d(F) + n$。因此（$E$，III，p. 28，第8条命题）我们有$d(E) = d(F)$，我们可以应用第8条命题。

#### 命题 9 {#alg-v-s14-prop-9 .statement tag=06SF}

— 令 K 为 K 的域和 $\Omega$ 代数闭扩张。假设 $\Omega$ 不是 K 上的代数；则超越 K 的 $\Omega$ 的元素的集合是无限的。此外，如果 x 和 y 是 $\Omega$ 中超越 K 的两个元素，则在 K 上存在 $\Omega$ 的自同构 u 使得 $u(x) = y$。

由于 $\Omega$ 不是 K 上的代数，因此存在 $\Omega$ 超越 K 的元素 x；则元素 $x^n$ ($n \in \mathbf{N}$) 在 K 上不同且超越。假设 x 和 y 在 K 上不同且超越；根据命题 2 (V, p. 106)，存在 $K(x)$ 到 $K(y)$ 的 K 同构$\tilde{u}$，使得 $\tilde{u}(x) = y$；因为 $K(x)$ 超越次数 1 K，Cor。命题 8 的 2 显示 $\tilde{u}$ 扩展到 $\Omega$ 的 K-自同构 u。

#### 命题 10 {#alg-v-s14-prop-10 .statement tag=06SG}

— 令 K 为 K 的域、$\Omega$ 代数闭扩张，以及 $\Omega$ 的 K 自同构的 G 群。让$x \in \Omega$。

a) 对于 x 在 K 上的代数，当 u 在 G 上运行时，元素 $u(x)$ 的集合是必要且充分的，

b) 对于 x 是 K 上的 p 自由基，对于所有 $u \in G$ $u(x) = x$ 是必要且充分的。

特别是，如果 K 是完美的，则群 G 的不变量集合等于 K。

首先假设 x 是超越的。根据命题 9，$\Omega$ 的元素的集合 T 在 K 上的超越是无限的，并且对于每个 $y \in T$ 都存在$u \in G$，使得 $u(x) = y$。因此，当 u 运行在 G 上时，元素 $u(x)$ 的集合是无限的。

现在假设 x 是 K 上的代数，并表示为 K 上的拟合最小多项式； $\Omega$ 中 f 的根的集合是有限的，对于每个 $u \in G$，我们有 $f(u(x)) = u(f(x)) = 0$。因此，当 u 在 G 上运行时，元素 $u(x)$ 的集合是有限的。这就证明了a）。

令L为$\Omega$的元素y的集合，使得$u(y) = y$对于所有$u \in G$，并令$\bar{K}$为$\Omega$中K的相对代数闭包。如上所述，L是$\bar{K}$在K上的子扩展。进一步（Cor. 1到Prop. 8）$\bar{K}$的每个K自同构现在是G. 元素的限制到$\bar{K}$。 Prop. 10的断言 b)遵循 Cor. 3 个V、p. 53。

### 5. 代数不相交的扩张

#### 定义 5 {#alg-v-s14-def-5 .statement tag=06SH}

— 设L为域K的扩张，E和F为L的两个子扩展。那么，E 和 F 被称为代数不相交的（在 K 上），并且 E 被称为从 F 在 K 上的代数不相交的，如果对于 E（分别 F）的每个子集 A（分别 B）在 K 上代数自由，A 和 B 是不相交的并且 $A \cup B$ 是代数自由的超过K。

#### 注 1 {#alg-v-s14-n5-rem-1 .statement tag=06SI}

如果 E 是 L 的子外延，并且是 K 上的代数，那么从 L 的每个子外延 F 来看，它在代数上都是不相交的。对于 K 的扩张来说，它是代数的，它本身应该是代数的不相交的是充分必要的。

#### 注 2 {#alg-v-s14-n5-rem-2 .statement tag=06SJ}

可能会发生 E 是从 F 到 K 的代数不相交的，但不超过 K 的子域 $K_{\|}$。 \* 对于例 C 从自身到 R 的代数不相交的，但不超过 $\mathbf{Q}$。 \*

#### 注 3 {#alg-v-s14-n5-rem-3 .statement tag=06SK}

显然，如果E在K上从$F$代数不相交的，则当E和F被视为L的子扩张时，当它们被视为$K(E \cup F)$的子扩张时也是如此，反之亦然。

#### 命题 11 {#alg-v-s14-prop-11 .statement tag=06SL}

— *如果 E 和 F 在 K 上是代数不相交的，则* $E \cap F$ *在 K* 上是代数。

这是从 Def 得出的。 5.

#### 命题 12 {#alg-v-s14-prop-12 .statement tag=06SM}

— *令 L 为域 K 的扩张以及 L 的 E、F 子扩展。那么下面的条件是等价的*：

a) *E 和 F 在代数上是不相交的*；

b) *存在 E 对 K 的超越基，它在 F* 上是代数自由的；

c) *E 中在 K 上代数自由的每个子集在 F* 上代数自由。

下面我们来介绍一下条件：

$b'$') *存在 F 对 K 的超越基，它在 E* 上是代数自由的；

$c'$') *F 中在 K 上代数自由的每个子集在 E* 上代数自由。

$a) \Rightarrow b'$') : 假设E和F在代数上是不相交的。设 B（分别为 C）为 E（分别为 $F$）在 K 上的超越基。则 $B \cap C = \varnothing$ 和 $B \cup C$ 在 K 上是代数自由的，因此 C 在 $K(B)$ 上是代数自由的（V， p. 107，命题 4)；由于 E 在 $K(B)$ 上是代数的，V、p. 108 的命题 6 表明 C 在 E 上是代数自由的。

$b'$') $\Rightarrow$ c) : 假设存在 F 对 K 的超越基 C，其在 E 上代数自由。设 A 为 E 的子集在 K 上代数自由。则 C 在 $K(A)$ 上代数自由，因此 A 在代数上自由超过$K(C)$（V，p. 107，命题4），因此超过$F$（V，p. 108，命题6），因为F是$K(C)$上的代数。

c) $\Rightarrow$ a) ：这立即来自第 4 条命题 (V，p. 107)。

同理可以证明蕴涵$a) \Rightarrow b) \Rightarrow c' ) \Rightarrow a)$。

#### 推论{#alg-v-s14-n5-cor-1 .statement tag=06SN}

— *令 E 和 F 在 K 上为不相交的。令 E' 为 E 在 L 中的相对代数闭包，F' 为 F* 中的相对代数闭包 (V, p. 19)。 *那么* E' * 和 F'* * 在 K* 上是代数不相交的。

设 B 是 E 对 K 的超越基；这也是 E' 对 K 的超越基。由于 E 在代数上是 F 在 K 上的不相交的，因此 B 在 F 上是代数自由的，因此在 F' 上是自由的（V，p. 108，命题 6）；现在我们可以应用提案 12。

#### 命题 13 {#alg-v-s14-prop-13 .statement tag=06SO}

— *令 L 为域 K 和 E、F L* 的两个子扩展的扩张。

a) *我们有* $\operatorname{tr. deg}_L F(E) \leq \operatorname{tr. deg}_K E$。 *当 E 和 F 是 K 上的代数不相交的时，则 E 对 K 的每一个超越基都是 * 的超越基

F(E) 超过 F，我们有 tr 。 deg_F F(E) = tr 。 deg_K E。相反，这个等式意味着当 tr 时，E 和 F 在 K 上是代数不相交的。 deg_K E 是有限的。

b) 我们有 tr 。 deg_KK(EU F) ≤ tr 。 deg_KE + tr 。 deg_K F。当 E 和 F 在 K 上代数不相交的时，我们有 tr 。 deg_KK(EU F) = tr 。 deg_KE + tr 。 deg_K F。相反，这个等式意味着当E和F对K具有有限超越次数时，E和F在K上代数不相交的。

a) 设B是E对K的超越基；那么 E 是 K(B) 上的代数，Cor 。 V、p. 18 的 2 表明 F(E) 是 F(K(B)) = F(B) 上的代数。由 Th. 2 (V, p. 109) B 包含 F(E) 对 F 的超越基；当 E 从 F 到 K 的代数不相交的时，B 在 F 上代数上自由（命题 12），这就是 F(E) 对 F 的超越基。a) 的前三个断言由此而来。现在假设 E 对 K 具有有限超越次数，等于 F(E) 对 F 的超越；因为 F(E) 是 F(B) 的代数且 Card B = tr 。 deg_F F(E)，Cor。 V, p. 110 的 1 表明 B 在 F 上是代数上自由的，因此 E 在 F 上在 K 上是代数上的不相交的（命题 12）。

b) 我们有 K(E U F) = F(E) ，所以 Cor。 V、p. 110 意味着等式：

$$
\text{tr . deg}_K K(E \cup F) = \text{tr . deg}_F F(E) + \text{tr . deg}_K F .
$$

现在 b) 紧随 a) 和这个等式。

#### 命题 14 {#alg-v-s14-prop-14 .statement tag=06SP}

— *令 L 为域 K 的扩张，E 和 F 是 L 和 B 的两个子扩展，是 E 对 K 的超越基。对于 E 和 F 在 K 上的代数不相交的，K(B) 和 F 在 K 上线性不相交的是充分必要的。*

为了使 E 和 F 在 K 上代数上不相交的，B 在 F 上代数上自由是必要且充分的（命题 12），也就是说，B 的元素中的单项式在 F 上线性无关。 由于向量 K 空间 K[B] 的这些单项式形式基，因此可以说 K[B] 和 F 在 K 上是线性的不相交的。 最后，由于 K(B) 是 K[B] 的分数的域，V、p. 14 的命题 6 表明 K[B] 和 F 是线性的不相交的当且仅当对于 K(B) 和 F 也是如此。

#### 推论 1 {#alg-v-s14-prop-14-cor-1 .statement tag=06SQ}

— *如果 E 和 F 是线性不相交的，则 E 是 F 在 K 上的代数不相交的。相反，如果 E 是 K 的纯扩张，并且是 F 在 K 上的代数不相交的，则 E 和 F 在 K 上是线性不相交的。*

#### 推论 2 {#alg-v-s14-prop-14-cor-2 .statement tag=06SR}

— *K 的每个纯扩张都与 K 的每个代数扩张线性相关不相交的；特别是，K 在 K 的每个纯扩张中都是相对代数封闭的。*

### 6. 扩张的代数自由族

#### 定义 6 {#alg-v-s14-def-6 .statement tag=06SS}

— 设$L$为域$K$和$(E_i)_{i \in I}$的扩张，$L$的子扩展族。如果满足以下条件，则称族$(E_i)_{i \in I}$是代数自由的：

(AF) 对于每个$i \in I$，令$A_i$为$E_i$的子集，它在$K$上是代数自由的。那么$A_i \cap A_j = \varnothing$对于$i \neq j$和$\bigcup_{i \in I} A_i$在$K$上是代数自由的。

#### 注 {#alg-v-s14-n6-rem-1 .statement tag=06ST}

根据命题3（$V$，p. 107），足以验证条件（AF）对于有限子集$A_i$。因此，我们得到以下结果：如果$(E_i)_{i \in I}$是代数自由族，则$(E'_i)_{i \in I}$也是如此，如果$E'_i$是每个$i \in I$的$E_i$的子扩展；相反，如果每个族$(E'_i)_{i \in I}$（其中$E'_i$是每个$i \in I$的有限生成的$E$子扩展）是代数自由的，则$(E_i)_{i \in I}$是代数自由的。另一方面，对于 $(E_i)_{i \in I}$ 来说，对于 $I$ 的每一个有限子集 $J$ 来说，$(E_i)_{i \in J}$ 应该是代数上自由的，这是必要且充分的。直观地说，我们可以说扩张的代数独立性是有限特征标的性质 «。

#### 命题 15 {#alg-v-s14-prop-15 .statement tag=06SU}

— 令 $(E_i)_{i \in I}$ 为域 $K$ 的给定扩张 $L$ 的子扩展族。那么下面的条件是等价的：

a) 族$(E_i)_{i \in I}$在代数上是自由的。

b) 对于每个 $i \in I$ 扩张 $E_i$，从 $E_j$ 为 $j \neq i$ 生成的扩张 $F_i$ 代数上不相交的超过 $K$。

c) 存在不相交的子集的$L$族$(B_i)_{i \in I}$，使得对于每个$i \in I$，$B_i$是$E_i$对$K$的超越基，并且$B = \bigcup_{i \in I} B_i$是$K$ 上代数自由。

显然，a) 隐含着 c)。

假设c)，让我们在$I$中有选择$i$；把$C_i = \bigcup_{j \neq i} B_j$。对于每个$j \neq i$，$E_j$的每个元素都是超过$K(B_j)$的代数，更不必说超过$K(C_i)$的代数。由科.因此，$V$、p. 18、域 $F_i$ 中的 1 是$K(C_i)$ 上的代数。此外，我们有$B_i \cap C_i = \varnothing$并且$B - B_i \cup C_i$在$K$上是代数自由的；因此，$B_i$在$K(C_i)$（$V$，p. 107，命题4）上是代数自由的，因此根据$V$，p. 108的命题6，$F_i$（在$K(C_i)$上是代数）。因此，我们证明了$E_i$在代数上是$F_i$到$K$的不相交的（$V$，p. 113，命题12），因此c）蕴含b）。

现在让我们假设 b) 并证明 a)。足以证明，如果$i_1, \ldots, i_n$与$I$不同元素，则扩张$(E_{i_1}, \ldots, E_{i_n})$族是代数自由的；我们通过归纳对$n$进行争论，$n = 1$的情况是微不足道的。假设$n > 1$和族$(E_{i_1}, \ldots, E_{i_{n-1}})$是代数自由的；对于 $E_{i_k}$ 的 $1 \leq k \leq n$ 选择子集 $A_k$ 在 $K$ 上的代数自由并把

B = A, U ... U A_{n-1}。由归纳假设子集 A_1, ..., A_{n-1} 成对不相交的并且 B 在 K 上是代数自由的； b) E_{i_n} 在 F_i 上是代数不相交的，并且由于 B 包含在 F_{i_n} 中，我们有 B \cap A_i = \varnothing 和 B \cup A_i = A, U ... U A_i 在 K 上是代数自由的。因此，我们证明族 (E_{i_1}, ..., E_{i_n}) 在代数上是自由的。

下面的命题概括了第13条命题的部分 b) (V, p. 113)。

#### 命题 16 {#alg-v-s14-prop-16 .statement tag=06SV}

— *令* (E_i)_{i \in I} *为域 K* 的扩张的子扩展族，并令E为由$\bigcup_{i \in I} E_i$生成的域。

a) *我们有* tr 。 deg_K E \leq \和_{i \in I} \text{tr . deg}_K E_i，*当族* (E_i)_{i \in I} *在 K* 上是代数自由时，*与等式。

b) *相反，假设* tr 。 deg_K E = \和_{i \in I} \text{tr . deg}_K E_i *和那个* tr 。 deg_K E * 是有限的；那么族* (E_i)_{i \in I}, *在 K* 上是代数自由的。

对于每个 $i \in I$ 令 B_i 为 E_i 对 K 的超越基并放入 $B = \bigcup_{i \in I} B_i$。对于每个$i \in I$，E_i 的每个元素都是 K(B_i) 上的代数，因此是 K(B) 上的代数。现在科. V、p. 18 中的 1 表明 E 是 K(B) 上的代数；由 V、p. 109、Th。 2, B 因此包含 E 对 K 的超越基。此外，如果族 (E_i)_{i \in I} 在 K 上是代数自由的，则 B_i 是不相交的并且集合 B 在 K 上是代数自由的。这建立了 a) (*集合理论*，III，p. 160，Prop. 4）。

在 b) 的假设下，E 是 K(B) 上的代数，并且是 K 上的有限超越次数，并且我们有 Card(B) \leq \text{tr 。 deg}_K E. 作者：Cor。 1 of V, p. 110, B 在 K 上是代数自由的，并且 B_i 是不相交的。现在，第 15 条命题表明族 (E_i)_{i \in I} 在 K 上是代数自由的。

之前陈述下一个定理让我们注存在任意超越次数的K的代数闭扩张，对于有理分式的适当域的例代数闭包。

#### 定理 5 {#alg-v-s14-thm-5 .statement tag=06SW}

— *设* (E_i)_{i \in I}，*为域 K 的扩张和 * \Omega *代数闭扩张 K* 的族。 *假设不等式*

$$
\text{tr . deg}_K \Omega \geq \sum_{i \in I} \text{tr . deg}_K E_i
$$

*成立。那么存在一个代数自由族* (F_i)_{i \in I}，*的子扩展* \Omega *使得* F_i *与* E_i *对于所有* i \in I 是K同构的。

对于每个 $i \in I$ 令 B_i 为 E_i 对 K 的超越基。令 B 为 \Omega 对 K 的超越基。通过 (2) 我们有 Card B \geq \和_{i \in I} \text{Card} B_i; *因此*存在一个族 (B'_i)_{i \in I}，*B 的成对不相交的子集和双射* u_i : B_i \to B'_i *for* i \in I。 *根据 V、p. 106、u、扩展的命题 2 到 K 同构* v_i *of* K(B_i) *onto* K(B'_i)； *因为* \Omega *是代数封闭的并且* E_i *代数超过*

K(B_i)，Cor。 (V, p. 23) 表明 $v_i$ 扩展到 $E_i$ 的 K 同构到 $\Omega$ 的子外延 $F_i$。由构造 $B'_i$ 是 $F_i$ 在 K 上的超越基，并且第 15 条命题（V，p. 115）表明$\Omega$ 的子扩张族 $(F_i)_{i \in I}$ 在 K 上是代数上自由的。

#### 推论 1 {#alg-v-s14-thm-5-cor-1 .statement tag=06SX}

— *设 E 和 R 为域 K 的两个扩张。假设 $\Omega$ 是代数闭集，超越性次数至少等于 E 的超越性。则 E 与 R 的子外延 K 同构的。*

#### 推论 2 {#alg-v-s14-thm-5-cor-2 .statement tag=06SY}

— *令 R 为代数闭域，无限超越次数超过其素数子域。那么每一个与$\Omega$具有相同特征的域都是域的升向有向并，同构于R的子域。*

对于每个域是有限生成的子域在其素数域上的升序定向并，现在足以应用Cor. 1.
\* 例。 — 这尤其适用于采用 $\Omega = \mathbf{C}$ (« Lefschetz' 原理 ») 的特征 0。 \*

### 7. 有限生成扩张

#### 命题 17 {#alg-v-s14-prop-17 .statement tag=06SZ}

— *令 E 为域 K 的扩张，B 为 E 对 K 的超越基。为了使 E 在 K (V, p. 11, Def. 2) 上有限生成，B 是有限的且次数 $[E : K(B)]$ 是有限的，这是必要且充分的。*

假设 E 在 K 上有限生成，并令 S 为 E 的有限子集，使得 $E = K(S)$。由 Th. 2 (V, p. 109) S 包含 E 对 K 的超越基 $B'$，并且与 B (V, p. 110, Th. 3) 具有相同的基数。因此B是有限的。把$K' = K(B)$；那么 E 是 $K'$ 的代数，我们有 $E = K'(S)$；由于 S 是有限的，Th。 V、p. 18中的2表明$[E : K']$是有限的。

相反，假设 B 是有限的并且 $[E : K(B)]$ 是有限的。如果C是向量空间E在$K(B)$上的（有限）基，我们有$E = K(B)(C) = K(B \cup C)$，所以E是K的有限生成的扩张。

#### 推论 1 {#alg-v-s14-prop-17-cor-1 .statement tag=06T0}

— *假设E是K的有限生成的扩张，并令$K'$为E中K的相对代数闭包（V，p. 19）。那么 $K'$ 的有限次数大于 K。*

设 B 是 E 对 K 的超越基。 V、p. 114、$K'$ 的 2 在 K、从而 $[K' : K] = [K'(B) : K(B)] \leq [E : K(B)]$ 上从 $K(B)$ 线性地不相交的，现在$[K' : K]$ 的有限性源自 $[E : K(B)]$。

#### 推论 2 {#alg-v-s14-prop-17-cor-2 .statement tag=06T1}

— *域在其素数子域包含上有限生成单位元的有限多个根。*

由科. 1 我们被简化为证明，即域L，即其素数子域的有限次数的扩张仅拥有单位元的根的有限数。当L具有特征$\neq 0$时，这一点很明显，因为它是有限的。如果L的特征为0且包含单位元的无穷多个根，则它是任意高阶的单位元原语包含根。 V、p. 84、周四。 2 因此，存在无穷大的整数 $n > 0$，使得$\varphi(n) \leq [L : \mathbf{Q}]$，这是荒谬的（V、p. 80、公式 (2) 和 (3)）。

#### 推论 3 {#alg-v-s14-prop-17-cor-3 .statement tag=06T2}

— *如果 E 是域 K 的有限生成的扩张，则 E 的每个子扩展 E' 都是有限生成的。*

设 B' 是 E' 对 K 的超越基。通过 V、p. 109、Th。 2、B' 包含在 E 对 K 的超越基 B 中，因此根据命题 17 是有限的。因为 E' 是 K(B') 上的代数，并且 E 是 K(B') 的有限生成的扩张。科。图 1 显示 $[E' : K(B')]$ 是有限的。现在，命题 17 表明 E' 是在 K 上有限生成的。

命题 17 可以用说来解释：K 的有限生成的扩张是纯粹超越的扩张 $K(x_1, \ldots, x_n)$ 的有限次数的代数扩张。

### 习题 {#alg-v-s14-exercises}

§ 14](exercises/s14/)参见[习题。
