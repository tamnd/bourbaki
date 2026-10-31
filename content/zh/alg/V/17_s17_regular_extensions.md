---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 17
section_title: Regular extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.180-A V.181
pdf_pages: 0251-0259, 0294-0295
extraction: ocr
subsections:
    - "no": 1
      title: Complements on the relative separable algebraic closure
      page: 137
      pdf_page: 251
    - "no": 2
      title: The tensor product of extensions
      page: 139
      pdf_page: 253
    - "no": 3
      title: Regular algebras
      page: 140
      pdf_page: 254
    - "no": 4
      title: Regular extensions
      page: 141
      pdf_page: 255
    - "no": 5
      title: Characterization of regular extensions
      page: 142
      pdf_page: 256
    - "no": 6
      title: Application to composite extensions
      page: 143
      pdf_page: 257
statements: 20
exercises: 5
content_sha256: 358a68ae37a73edfa59f33ed07d0a9f3ff489e463b3421d57cf1a3ac7c3f3efa
translated_from: content/en/alg/V/17_s17_regular_extensions.md
translation_method: google
source_content_sha256: c3f351f5e813a393d1fb207cf121c6dd2bc4e8303d881b9cf4b097b0c621cb53
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: a493264b83e29dc553be440d579517d8af8057f10b75f0ec8ddb0c34ee6e3e4b
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 17。常规扩张

### 1. 相对可分代数闭包的补集

#### 定理 1（扎里斯基）{#alg-v-s17-thm-1 .statement tag=06VP}

— *令 K 为 K 的域、L 扩张，$K_1$ L 中 K 的相对可分代数闭包 (V、p. 44)，$K_2$ 代数闭包中 K 的相对可分L (V, p. 19) 和 $(X_i)_{i \in I}$ 不定族。那么$K_1(X_i)_{i \in I}$就是$L(X_i)_{i \in I}$中$K(X_i)_{i \in I}$的相对可分代数闭包，$K_2(X_i)_{i \in I}$就是$L(X_i)_{i \in I}$中$K(X_i)_{i \in I}$的相对代数闭包。

A) 假设 E 是 E 的域且 F 扩张域，并且 F 的每个元素是 E 属于到 E 上的可分代数。 设$u$为$F(X)$的元素，它是$E(X)$上的可分代数；我们将证明$u$属于到$E(X)$。 $F(X)$ 中存在两个互素多项式 P 和 Q，使得 $u = P/Q$ 且我们可以取 Q 为一元多项式。 令 S 为 P 和 Q 的系数 F 由……组成的*有限* 子集，$F_0 = E(S)$，并令 A 为$F_0$ 到 $F_0$ 的 E 导数。 令$D$为$F_0(X)$的推导自身，与$F_0$上的$A$和映射$X$到$0$一致（V，p. 128，命题3）。

由于$u \in F_0(X)$是$E(X)$上的可分代数，并且$D$在$E(X)$上是零，因此我们有$D(u) = 0$（V，p.129，命题4），从而$D(P) . Q = P . D(Q)$。由于$P$和$Q$互质，我们结论$Q$除$D(Q)$（IV，p. 13，Cor.4）。现在$Q$可以写成形式
$$
Q(X) = X^n + a_1 X^{n-1} + \ldots + a_{n-1} X + a_n
$$
$a_1, \ldots, a_n$ 位于$F_0$；从$D(x) = 0$开始，我们有
$$
D(Q) = \Delta(a_1) X^{n-1} + \cdots + \Delta(a_{n-1}) X + \Delta(a_n)
$$
从而$\deg D(Q) < \deg Q$。由于$Q$除$D(Q)$，只有$D(Q) = 0$才有可能。但然后$D(P) = 0$因为$D(P) . Q = P . D(Q)$。现在（1）和$P$的类似公式表明，$A$消灭了$P$和$Q$、从而$A = 0$的系数集合$S$，因为$F_0 = E(S)$。 V，p. 135，Cor。 2、有限生成的$E$的扩张$F_0$因此是可分代数的；根据$E$和$F$的假设，我们有$F_0 = E$，所以最终$u \in E(X)$。

B) 现在假设 $E$ 在扩张域 $F$ 中是相对代数封闭的，并用 $p$ 表示 $E$ 的特征指数。令$u$为$F(X)$的元素，它是$E(X)$的代数。存在整数 $f \geq 0$，使得 $v = u^{p^f}$ 是 $E(X)$ 上的可分代数（V，p. 44，命题 13）。根据 A)，我们有 $v \in E(X)$。 形式 $P/Q$ 中存在唯一的 $u$ 表示，且$F[X]$ 和 $Q$ 摩尼式中存在互质多项式 $P$ 和 $Q$；我们有一个类似的分解$v = P_1/Q_1$，其中$P_1$和$Q_1$在$E[X]$和$Q_1$莫尼克中相对素数。由此可知$P_1/Q_1 = P^{p^f}/Q^{p^f}$；多项式 $P^{p^f}$ 和 $Q^{p^f}$ 在 $F[X]$ 中互质（IV、p. 13，Cor. 6），如 $P_1$ 和 $Q_1$，并且 $Q^{p^f}$ 是单调的。由此可见$P^{p^f} = P_1 \in E[X]$和$Q^{p^f} = Q_1 \in E[X]$。因此，$P$和$Q$的系数是$E$上的$p$根，因此属于到$E$，因为$E$在$F$中是相对代数封闭的。因此我们有$P \in E[X]$、$Q \in E[X]$，最后是$u \in E(X)$。这证明$E(X)$在$F(X)$中是相对代数封闭的。

C) 我们使用定理的记号 1. 由于 $K_1$ 是 $K$ 的可分代数扩张，$K(X_i)_{i \in I}$ 的扩张 $K_1(X_i)_{i \in I}$ 是代数且可分的 (V, p. 39，提案 6）。此外，$L$的每个元素在$K$、属于到$K$上都是代数且可分的，（V、p. 44，命题13，a））。设$J$为$I$的有限子集；通过 $J$ 基数上的直接的归纳，我们从 A) 中推出$L(X_i)_{i \in I}$ 的每个元素，它是代数且可在 $K(X_i)_{i \in I}$、属于到 $K_1(X_i)_{i \in J}$ 上分离。最后令$u$为$L(X_i)_{i \in I}$的元素，在$K(X_i)_{i \in I}$上代数且可分；存在$I$的有限子集$J$使得$u$属于到$L(X_i)_{i \in I}$并且是代数且在$K(X_i)_{i \in J}$上可分；据所说，$u$属于到$K_1(X_i)_{i \in J}$，以及更不必说到$K_1(X_i)_{i \in I}$。

因此，我们从 A) 推出$K_1(X_i)_{i \in I}$ 是$L(X_i)_{i \in I}$ 中$K(X_i)_{i \in I}$ 的相对可分闭包；同样地，从 B) 可以得出，$K_2(X_i)_{i \in I}$ 是$L(X_i)_{i \in I}$ 中$K(X_i)_{i \in I}$ 的相对代数闭包。

### 2. 张量积 / 扩张

#### 命题 1 {#alg-v-s17-prop-1 .statement tag=06VQ}

— 令 $\Omega$ 为域 $K$ 的扩张，并令 $L, M$ 为 $\Omega$ 的两个子扩展，它们在代数上是不相交的在 $K$ 上。假设$L$中$K$的相对可分代数闭包等于$K$^1。令$\varphi$为$L \otimes_K M$到$\Omega$映射$x \otimes y$到$xy$的$K$代数同态，对于$x \in L, y \in M$，令$p$为核 $\varphi$。那么$p$就是$L \otimes_K M$的幂零元集合，这是$L \otimes_K M$的最小的素理想。

如果有必要的话，在替换 $\Omega$ 到代数闭包上，我们可以假设 $\Omega$ 是代数闭的。令$B$是$M$对$K$的超越基，$N$是$\Omega$和$N_r$（或$N_s$）集合中$K(B)$的相对代数闭包 $N$ 中的元素在 $K(B)$ 上可分离（分别为 p 根式）。我们注认为$M$是$K(B)$的代数，因此$N$是$\Omega$中$M$的相对代数闭包。

$$
\begin{array}{ccccccccc}
L & \longrightarrow & L(B) & \longrightarrow & L(B \cup N_s) \\
\uparrow & & \uparrow & & \uparrow \\
K & \longrightarrow & K(B) & \longrightarrow & N_s \\
& & \downarrow & & \downarrow \\
& & M & \longrightarrow & N \\
\uparrow & & \downarrow & & \downarrow \\
N_r & \longrightarrow & N & \longrightarrow & \Omega
\end{array}
$$

图 1.

让我们定义下面的同态链：

$$
L \otimes_K M \xrightarrow{\alpha} L \otimes_K N \xrightarrow{\beta} (L \otimes_K K(B)) \otimes_{K(B)} N \xrightarrow{\gamma} L(B) \otimes_{K(B)} N
$$
$$
\rightarrow L(B) \otimes_{K(B)} N_s \otimes_{K(B)} N_r \xrightarrow{\varepsilon} L(B \cup N_s) \otimes_{K(B)} N_r \xrightarrow{\zeta} \Omega .
$$

我们有$\alpha = \mathrm{Id}_L \otimes u$，其中$u$是$M$到$N$的典范嵌入，因此$\alpha$是单射的。 映射 $\beta$ 是群的交换律同构，其中映射 $x \otimes y$ 到 $(x \otimes 1) \otimes y$（II、p. 278，命题 2）对于 $x \in L$ 和 $y \in N$。我们有$\gamma = v \otimes \mathrm{Id}_N$，其中$v$是$L \otimes_K K(B)$到$L(B)$的$K$代数同态，对于$x \in L$和$y \in K(B)$，映射$x \otimes y$到$xy$；由于 $L$ 和 $M$ 在 $K$ 上是代数上的不相交的，因此第 14 条命题（V，p. 114）表明 $L$ 和 $K(B)$ 在 $K$ 上是线性的不相交的，在其他情况下字, $v$ 是单射的，因此 $y$ 是单射的。由于 $N$ 是 $K(B)$ 的拟伽罗瓦扩展，因此存在 (V, p. 76, 命题 13) $N_s \otimes_{K(B)} N_r$ 的 $K(B)$ 代数同构 $w$ 到 $N$ 映射 $x \otimes y$ 至

1 这个假设是用说表示的有时，即$L$是$K$的主扩张。

xy 为 $x \in \mathbf{N}$ 和 $y \in \mathbf{N}_r$；我们用 6 表示 *同构* $\mathrm{Id}_{L(B)} \otimes w \ ^1$。由 Th. 1 (V, p. 137) 和假设在K的扩张L上，$L(B)$的每个元素是代数且在$K(B)$属于到$K(B)$上可分；特别是，我们有 $L(B) \cap N_s = K(B)$。由于$N_r$是$K(B)$的伽罗瓦扩张，Th。 5 (V, p. 71) 表明对于$x \in L(B)$，存在$L(B) \otimes_{K(B)} N_s$到$L(B U N_r)$映射$x \otimes y$到$xy$的$K(B)$代数同构$w'$，并且$y \in N_r$；我们用 $\varepsilon$ 表示 *同构* $w' \otimes \mathrm{Id}_{N_r}$。最后，对于$x \in L(B U N_r)$和$y \in N_r$，$\zeta$是K-代数同态映射$x \otimes y$到$xy$。

如上所述，$\eta = \varepsilon \delta \gamma \beta \alpha$是$L \otimes_K M$到$L(B U N_r) \otimes_{K(B), N_r}$的单射K-代数同态。进一步，M的每个元素都是形式$\sum_{i=1}^n a_i b_i$，$a_i \in \mathbf{N}$，$b_i \in \mathbf{N}_r$对于$1 \leq i \leq n$；因此我们得到$\varphi = \zeta \eta$。

$\varphi$的核$p$是$L \otimes_K M$的素理想，因此根据第2条命题，$L \otimes_K M$属于到$p$的每一个幂零元（V，p. 118）。反之，令$a$为$p$的元素；将 $\eta(a) = \sum_{r=1}^s b_i \otimes c_i$ 与 $b_i \in L(B U N_r)$ 和 $c_i \in N_r$ 组合为 $1 \leq i \leq s$。由于$N_r$是$K(B)$的p根扩展，因此存在整数$f \geq 0$，使得$c_i^{p^f}$属于到$K(B)$对于$1 \leq i \leq s$（其中$p$是K的特征指数）。但我们有

$$
\eta(a^{p^f}) = \sum_{i=1}^s b_i^{p^f} \otimes c_i^{p^f} = \left( \sum_{i=1}^s b_i^{p^f} c_i^{p^f} \right) \otimes 1 - \zeta \eta(a)^{p^f} \otimes 1 = 0
$$

由于 $\eta$ 是单射的，我们最终得到 $a^{p^f} = 0$。因此，我们证明$p$是$L \otimes_K M$的所有幂零元中的集合。现在，根据第 2 条命题，$L \otimes_K M$ 包含 $p$ 的每个素理想（V，p. 118）。

#### 推论{#alg-v-s17-n2-cor-1 .statement tag=06VR}

*设L和M为域K的两个扩张。假设L中K的相对可分代数闭包等于K。则$L \otimes_K M$的幂零元的集合p是素理想。此外，如果L或M可通过K分离，则$L \otimes_K M$是整环。*

我们可以假设L和M在代数上是K的扩张$\Omega$的不相交的子扩展（V，p. 116，Th.5）；则根据命题 1，p 是素理想 (V, p. 139)。此外，如果L或M可通过K分离，则$L \otimes_K M$是环减去定义的可分扩张（V，p. 119，Def.1）；所以$p = 0$和$L \otimes_K M$是整环，因为p是素数。

### 3.常规代数

#### 定义 1 {#alg-v-s17-def-1 .statement tag=06VS}

*令 K 为域。如果对于 K 的每个扩张 L，$L \otimes_K A$ 是整环，则称代数 A over K 是正则的。*

正则代数特别是整环，因此是可交换的。

#### 命题 2 {#alg-v-s17-prop-2 .statement tag=06VT}

— 令$A$和$B$等于代数除以域$K$。如果 $A$ 是整环并且 $B$ 是正则，则 $A \otimes_K B$ 是整环。

设$L$为$A$的分数中的域。由于$B$是正则$K$代数，$L \otimes_K B$是整环，因此$A \otimes_K B$也是，因为它与$L \otimes_K B$的子环同构。

#### 命题 3 {#alg-v-s17-prop-3 .statement tag=06VU}

— 令 $K$ 为域。
a) 正则 $K$ 代数的每个子代数本身都是正则的。
b) 两个正则 $K$ 代数的张量积又是正则的。
c) 设$A$为$K$代数，且$K'$扩张为$K$。为了使 $A$ 是正则的，从 $A$ 通过扩张标量导出的 $K'$-代数 $A_{(K')}$ 应该是正则的，这是必要且充分的。

a) (resp. c)) 的证明与第 3 号提案的部分 a) (resp. d)) 相同，V、p. 119、之后替换处处都通过 « 整环 » 和 « 减少了环 »可通过“常规代数”分离代数 »。让我们证明b)。

令 $A$ 和 $B$ 为两个正则 $K$ 代数。令 $L$ 为 $K$ 的扩张。由于$A$是正则，环$L \otimes_K A$是整环。根据命题 2，环 $(L \otimes_K A) \otimes_K B$ 是整环，因为 $B$ 是正则。最后，环$L \otimes_K (A \otimes_K B)$与$(L \otimes_K A) \otimes_K B$同构的，因此是整环。这表明 $A \otimes_K B$ 是正则 $K$ 代数。

### 4.常规扩张

#### 定义 2 {#alg-v-s17-def-2 .statement tag=06VV}

— 域 $K$ 的扩张被认为是正则的，如果它是正则的 $K$-代数。

#### 命题 4 {#alg-v-s17-prop-4 .statement tag=06VW}

— 令 $A$ 为代数超过域 $K$，即整环，并且 $E$ 为分数的域。令$L$为$K$中的扩张；如果环$L \otimes_K A$是整环，$L \otimes_K E$也是如此。

如果$L \otimes_K A$是整环，则可以将其嵌入到分数$F$的域中。 将$x \in L$写成$u(x) = x \otimes 1$，并用$v$表示$E$到$F$的$K$同态，其中$A$的扩展单同态$y \mapsto 1 \otimes y$到$F$。 根据第 6 条命题 (V, p. 14) 子域 $u(L)$ 和 $v(E)$ 的$F$ 是线性不相交的超过$K$；因此，$L \otimes_K E$到$F$（V，p. 12）的同态$u * v$是单射的。 这表明 $L \otimes_K E$ 为整环。

#### 推论{#alg-v-s17-n4-cor-1 .statement tag=06VX}

— 要使 $A$ 成为正则 $K$ 代数，其分数的域应该是 $K$ 的正则扩张是充分必要的。

根据命题 4，条件是必要的，并且根据命题 3, a)，条件是充分的。

#### 命题 5 {#alg-v-s17-prop-5 .statement tag=06VY}

— 域 $K$ 的每个纯扩张都是正则。

通过前面的推论，足以证明每个多项式代数$A = K[X_i]_i$，都是正则$K$代数。设$L$为$K$的扩张； 环 $L \otimes_K A$ 与 $L[X_i]_{i \in I}$ (III, p. 449, 注 2) 同构，因此整环 (IV, p. 9, 命题 8)。

#### 命题 6 {#alg-v-s17-prop-6 .statement tag=06VZ}

— 令 L 为域 K 的扩张。如果 L 是正则的，则 L 的每个子扩展都是正则的。相反，如果 L 的每个有限生成的子扩展都是正则的，则 L 也是正则的。

第一个断言由命题 3, a) 得出。

设 M 为 K 的扩张，并令 $\mathscr{U}$ 为 L 的所有有限生成的子扩展的集合。对于每个E$\in \mathscr{U}$，环$M \otimes_K E$可以用$M \otimes_K L$的子环来识别，因此我们有$M \otimes_K L$的子环的递增有向族，其并是$M \otimes_K L$。现在第二个断言紧随其后。

#### 命题 7 {#alg-v-s17-prop-7 .statement tag=06W0}

— 令 L 为域 K 的扩张，且 M 为 L 代数（对于例、扩张 L）。如果 L 在 K 上是正则且 M 是正则 L 代数，则 M 是正则 K-代数。

令 E 为 K 的扩张；由于 L 在 K 上是正则，$E \otimes_K L$ 是整环。根据命题 2 (V, p. 141) 环 $(E \otimes_K L) \otimes_L M$ 因此是整环并且与它同构的环 $E \otimes_K M$ 也是如此 (II. p. 278, 命题 2)。于是就有了这样的结果。

#### 命题 8 {#alg-v-s17-prop-8 .statement tag=06W1}

— 令 L 和 M 为域 K 中的两个扩张。

a) 如果 M 在 K 上是正则，则整环 $L \otimes_K M$ 的分数域是 L 的正则扩张。

b) 如果L和M是K的正则扩张，则$L \otimes_K M$的分数的域也是如此。

断言 a) 由命题 3, c) (V, p. 141) 和 Cor. 得出。 V、p. 141； 断言 b) 由命题 3, b) (V, p. 141) 和 Cor. 得出。 V、p. 141。

### 5.常规扩张的刻画

#### 命题 9 {#alg-v-s17-prop-9 .statement tag=06W2}

— 令 K 为 K 的域、K 的 $\overline{K}$ 代数闭包和 K 的 L 扩张。则以下条件是等价的：

a) L 在 K 上可分，且 K 在 L 中相对代数封闭。

b) L 是 K 的正则扩张。

c) 环 $\overline{K} \otimes_K L$ 是整环。

d) 设$\overline{L}$为L的代数闭包。那么 L 与 $\overline{L}$ 中 K 的相对代数闭包在 K 上是线性的不相交的。

而且，当这些条件成立时，$\overline{K} \otimes_K L$就是域。

a) $\Rightarrow$ b)：设M为K的扩张。在a)的假设下，环$M \otimes_K L$为整环，由V，p. 140，得。

b) $\Rightarrow$ c)：这是从 Def 得出的。 2.

c) $\Rightarrow$ d)：通过 d) 的记号，我们将可以确定 $\overline{K}$ 与 $\overline{L}$ 中 K 的相对代数闭包相结合（V、p. 22，例 2）。假设环$A = \overline{K} \otimes_K L$是整环。令 E 为 K 在 K 上的有限次数子扩展； 子环

A 的 E $\otimes_K$ L 为整环，因此有限次数的代数大于 L；由科。 V、p. 10 就是域。由于$\bar{K}$是上述型的扩张E中的并递增有向集合，因此A是域（V，p. 11，命题3）。因此，A 的典范同态到 $\bar{L}$ 映射 $x \otimes y$ 到 $xy$（对于 $x \in \bar{K}$ 和 $y \in L$）是单射的，因此 L 和 $\bar{K}$ 在 K 上是线性的不相交的。

$d) \Rightarrow a)$：在d)的假设下，我们有$L \cap \bar{K} = K$，因此K在L中是相对代数封闭的；此外，如果 p 是 K 的特征指数，则域 $L$ 在 $K$ 上与 $K^{p^{-\infty}}$ 呈线性关系不相交的，因此 L 在 K 上可分（V，p. 123，Cor. 1）。

#### 推论 1 {#alg-v-s17-prop-9-cor-1 .statement tag=06W3}

— 令 A 为代数大于域 K。要使 A 成为正则 K-代数，环 $\bar{K} \otimes_K A$ 为整环是充分必要的。

上述条件显然是必要的。反之，假设$\bar{K} \otimes_K A$是整环，并用A的分数的E域表示，根据命题4(V,p. 141)环$\bar{K} \otimes_K E$是整环，因此E是K的正则扩张，根据第 9 号提案；由V、p. 141、Cor.，我们结论 A 是正则K-代数。

#### 推论 2 {#alg-v-s17-prop-9-cor-2 .statement tag=06W4}

— 令 K 为代数闭域。每个K-代数即整环都是常规的K-代数。特别是，K 的每个扩张都是规则的。

这是从 Cor 得出的。 1.

#### 推论 3 {#alg-v-s17-prop-9-cor-3 .statement tag=06W5}

— 设 K 为代数闭域。如果A和B是两个K-代数，即整环，那么$A \otimes_K B$也是如此。

由科. 2、A和B是正则K-代数，只需应用命题2（V，p. 141）即可。

### 6. 复合应用扩张

#### 命题 10 {#alg-v-s17-prop-10 .statement tag=06W6}

— Let L and M be two extensions of a field K and $(E, u, v)$ a composite extension of L and M (V, p. 12). 假设环 $L \otimes_K M$ 为整环，且 E 的子外延 $u(L)$ 和 $v(M)$ 在 K 上代数为不相交的。 那么$u(L)$和$v(M)$在K上是线性的不相交的。

将$w = u * v$(V，p. 12)，用整环$L \otimes_K M$分数F域和认同L(分别M)和F的子域通过映射表示$x \mapsto x \otimes 1$（分别为$y \mapsto 1 \otimes y$）；那么 w 到 L（分别是 M）的限制就是 u（分别是 v）。设 B 是 M 对 K 的超越基 (V, p. 109, Th.1)。

通过假设$u(L)$和$v(M)$在K上的代数不相交的；因此（V，p. 114，命题14），$u(L)$和$v(K(B))$在K上是线性的不相交的。因此，存在一个K同态$u': L(B) \to E$，它在L上与u一致并且与v ou K(B)一致。通过构造 L 和 M 与 F 中的 K 成线性关系不相交的；根据第 8 条命题 (V, p. 15) F 的子域 $L(B)$ 和$M$ 与$K(B)$ 呈线性不相交的关系。由此可见，存在一个 K-同态 $w' : M[L(B)] \to E$，它在 $L(B)$ 上与 $u'$ 一致，在 $M$ 上与 $v$ 一致。但域$F$是由$M \cup L(B)$生成的，$M$是$K(B)$的代数；因此我们有$M[L(B)] = F$（V，p. 18，Cor.2）。因此我们结论认为$w'$是$F$到$E$的K同构，其限制到$L$（或$M$）是$u$（或$v$）。这表明 $u(L)$ 和 $v(M)$ 与 $K$ 呈线性关系不相交的。

#### 推论 1 {#alg-v-s17-prop-10-cor-1 .statement tag=06W7}

*Let $\Omega$ be an extension of a field $K$ and $L$ a subextension of $\Omega$ which is regular over $K$. $\Omega$ 的每个子扩展 $M$（从 $L$ 到 $K$ 的代数不相交的）都是线性的不相交的。*

环$L \otimes_K M$是常规扩张的整环乘定义，现在足以应用第10条提案。

#### 推论 2 {#alg-v-s17-prop-10-cor-2 .statement tag=06W8}

*令$\Omega$为域$K$和$L, M$两个$\Omega$的子扩展的扩张。假设$L$在$K$上可分，并且$M$中$K$的相对值可分闭包等于$K$。如果$L$和$M$在代数上是不相交的超过$K$，那么它们是线性不相交的超过$K$。*

根据第 10 号提案，注环 $L \otimes_K M$ 是整环（V，p. 140，Cor.）。

习题

### 习题 {#alg-v-s17-exercises}

§ 17](exercises/s17/)参见[习题。
