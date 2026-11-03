---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 4
section_title: Strict morphisms of Fréchet spaces
lang: zh
source: evt-i-v
book_pages: TVS IV.26-TVS IV.32, TVS IV.62-TVS IV.67
pdf_pages: 0208-0214, 0244-0249
extraction: ocr
subsections:
    - "no": 1
      title: Characterizations of strict morphisms
      page: 27
      pdf_page: 209
    - "no": 2
      title: Strict morphisms of Fréchet spaces
      page: 28
      pdf_page: 210
    - "no": 3
      title: Criteria for surjectivity
      page: 31
      pdf_page: 213
statements: 13
exercises: 23
content_sha256: 391eb2f9dfac6ad0bcb05489a6a2cf0dde551e73b38f6effab53345ac558b6ee
translated_from: content/en/evt/IV/04_s4_strict_morphisms_of_frechet_spaces.md
translation_method: google
source_content_sha256: c407d8cd0dfb8dde36f5bdedd16c24376ca0dd13486d65d99b3e2de383541cec
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 48909e0b97912a054781c7908d06774a10669d58d004c411bc33f9dd4a5ec445
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 4。严格 frÉchet 态射空间

对于每个局部凸空间 E，令S(E) 表示E 上所有连续半范数的集合。对于每个$p \in S(E)$，令$H_p$ 表示E 上所有线性形式 f 的集合，使得$|f| \leqslant p$。对于$E'$的等连续子集的出生学由……组成，族$(H_p)_{p \in S(E)}$是基。

### 1. 严格刻画态射

#### 命题 1 {#evt-iv-s4-prop-1 .statement tag=07UR}

设E和F是两个局部凸空间，u是从E到F的连续线性映射。在阶中，u是严格的态射，满足以下条件是充分必要的：

(MS) 对于每个半范数 $p \in S(E)$（在 u 的核上为空），S(F) 中存在 q 使得 $p \leq q \circ u$。

设 N 为 u 的核，M 像；我们引入u的规范分解，让

$$
E \xrightarrow{\pi} E/N \xrightarrow{\tilde{u}} M \xrightarrow{} F .
$$

E 上的连续半范数在 N 上为零，是半范数 $p_1 \circ \pi$，其中 $p_1$ 范围超过 S(E/N)；类似地，S(M) 由半范数 $q_1$ 组成，其中存在 $q \in S(F)$ 和 $q_1 \leq q/F$。最后，u 是严格的态射当且仅当双射连续线性映射 $\tilde{u}$ 具有连续逆元；这也意味着 S(E/N) 中的每个半范数都是形式 $q_1 \circ \tilde{u}$，其中 S(M) 中的$q_1$。命题 1 紧随这些注而来。

#### 命题 2 {#evt-iv-s4-prop-2 .statement tag=07US}

设E和F是两个Hausdorff局部凸空间，u是从E到F的连续线性映射。在阶中，u是严格的态射，其转置$^t u : F' \to E'$满足以下条件是充分必要的：

a) $^t u$ 的像在 $E'$ 中关闭，对于 $\sigma(E', E)$。

b) $^t u$ 的像中包含的$E'$ 的每个等连续子集是$F'$ 的等连续子集的$^t u$ 下的像。

如果是这样，我们有 $\operatorname{Ker} ^t u = (\operatorname{Im} u)^{\circ}$ 和 $\operatorname{Im} ^t u = (\operatorname{Ker} u)^{\circ}$，并且存在从 Coker $^t u$ 到 Ker u 的对偶以及从 Ker $^t u$ 到 Coker u 的对偶的典范同构。

设 N 为 u 的核和 I 像。由科。 $^t u$的II、p. 47、核的2是I的正交，$\sigma(E', E)$的$^t u$的像的闭包是N的正交$N^{\circ}$。a)的合取和b) 则等价于以下条件：

b') $N^{\circ}$ 中包含的$E'$ 的每个等连续子集是$F'$ 的等连续子集的$^t u$ 下的像。

由于 $N^{\circ}$ 可以用 E/N 的对偶来识别，道具。 9、IV、p. 8的(i)，表明$N^{\circ}$中包含的$E'$的等连续子集是集合，它们包含在形式$H_p$的集合中，其中p是E上的连续半范数，消失在 N 上。 条件 b') 然后说，对于 N 上为空的每个半范数 $p \in S(E)$，存在 $q \in S(F)$ 使得 $H_p \subset ^t u(H_q)$。根据 Hahn-Banach 定理（II、p. 23、cor.1 和 2、p. 63、th.1 和 cor.1），我们有 $^t u(H_q) = H_{q \circ u}$，并且关系 $H_p \subset H_{p'}$ 和 $p \leq p'$ 对于所有半范数都是等价的S(E) 中的 $p$ 和 $p'$。因而，关系$H_p \subset ^t u(H_q)$相当于关系$p \leq q \circ u$。通过道具。 1, 性质 b') 意味着 u 是严格的态射。

假设 u 是严格的态射。我们已经知道，$^t u$的核是I的正交，$^t u$的像是N的正交。$u$的余核是空间$F/I$，它的对偶可以被识别为$I^\circ = \mathrm{Ker}\ ^t u$。类似地，$N = \mathrm{Ker}\ u$的对偶可以用$E'/N^\circ$（IV，p. 8）来识别，*即*用$^t u$的余核来识别，因为$N^\circ$是$^t u$的像。

#### 注 {#evt-iv-s4-n1-rem-1 .statement tag=07UT}

— 具有记号的支柱。 2, 性质 $b'$) 也意味着 $u$ 是弱化拓扑的严格态射 (II, p. 49, cor. 3)。

#### 命题 3 {#evt-iv-s4-prop-3 .statement tag=07UU}

*设E和F是两个局部凸空间，u是从E到F的连续线性映射。我们假设E是Hausdorff并且F是可度量的。为了让你成为严格的态射，$^t u$的像在$E'$对弱拓扑$\sigma(E', E)$关闭是必要且充分的。*

必要性来自于道具。 2.

相反，假设$^t u$的像对于$\sigma(E', E)$是封闭的，并引入$u$的规范分解，如prop的证明所示。 1. 由上述注，$\tilde{u}$的逆映射$\tilde{u}^{-1}$对于弱化拓扑是连续的。但是 F 的子空间 $M = u(E)$ 是可度量的，因此是出生学的（III，p. 12，道具 2）；因而 (IV, p. 7, 命题 7, (ii))，$\tilde{u}^{-1}$ 是连续的，因而 $u$ 是严格的态射。

### 2. 严格 Fréchet 态射空间

#### 定理 1 {#evt-iv-s4-thm-1 .statement tag=07UV}

*设E和F是两个Fréchet 空间，u是从E到F的连续线性映射。以下条件是等价的：

a) $u$ 是严格的态射。
b) 对于弱化拓扑，$u$ 是严格的态射。
c) $u$ 的像在 F 中闭。
d) 对于弱拓扑，$^t u$ 是从$F'$ 到$E'$ 的严格态射。
e) $^t u$的像在$E'$关闭，对于弱拓扑$\sigma(E', E)$。
f) $^t u$的像在$E'$关闭，对于强拓扑$\beta(E', E)$。
g) $^t u$是从$F'_c$到$E'_c$的严格态射（赋予拓扑紧收敛的对偶）。

a)、b) 和 e) 的等价由命题得出。其前面的 IV、p. 28 和注中的 3 个。 a) 和 c) 正是对应的。 3 个I、p. 19。 IV、p. 28的注，也表明d)相当于$u$的像对于F的弱化的拓扑$\sigma(F, F')$是闭合的； c) 和 d) 的等价则由命题得出。 2 个IV、p. 4。

现在我们证明 e) 和 f) 的等价。只要证明 f) 蕴涵 e) 就足够了。假设$^t u$的像对于$E'$中的$\beta(E', E)$是闭合的。由于 Banach-Dieudonné 定理 (IV, p. 25, cor. 2)，足以证明对于 E 中 0 的每个凸平衡邻域 U，交 $B = ^t u(F') \cap U$ 对于 $\sigma(E', E)$ 是紧致的。 Fréchet 空间 E 的强对偶 $E'_b$ 是完备的（IV、p. 22，命题 2），因而 $E'_b$ 的闭子集 B 是完备的，因此赋范的空间 $E'_B$ 是完备的（III、p. 8、推论）。令$(V_n)$为递减序列，形成F中0的邻域的基本系统。然后$F'$是集合$C = V_n^\circ$的并，对于$\sigma(F', F)$来说是紧致的，因而$E'_B = \bigcup_n B_n$，与$B_n = E'_B \cap ^t u(C_n)$。由于 $E'_B$ 是贝尔空间，且集合 $B_n$ 都是凸平衡且闭的，因此存在实数 $r > 0$ 和整数 $n$，使得 $B \subset r.B_n$。那么我们就有$B = U^\circ \cap {}^t u(r.C_n)$；由于集合 $U^\circ$ 和 $r.C_n$ 是紧致的，并且 ${}^t u$ 对于弱拓扑是连续的，因而 $B$ 对于 $\sigma(E', E)$ 是紧致的。这样就完成了 e) 和 f) 的等价的证明。

最后 g) 的等价和前面的条件由 prop. 得出。 GT 18，X, § 2, No. 10 及以下引理。

#### 引理 1 {#evt-iv-s4-lem-1 .statement tag=07UW}

*设 E 和 F 为两个 Hausdorff 局部凸准完备空间，u 为从 E 到 F 的连续线性映射。为了使 ${}^t u$ 成为从 $F'_c$ 到 $E'_c$ 的严格态射，像是充分必要的u 的$u(E)$是封闭的，并且$u(E)$的每个紧凑子集是E的紧凑子集的u下的像。*

麦基的那一天。 (IV, p. 2, th. 1) 以及在紧致收敛重合的 $E'$ (分别为 F) 拓扑和凸紧致收敛 (IV, p. 4) 上，我们可以将 E (分别为 F) 与对偶 $E'_c$ 等价（分别$F'_c$）。那么$u$是${}^t u$的转置，E（或F）的等连续子集是相对的紧集。然后从 prop 得出引理 1。 2 (IV, p. 27)，因为 $u(E)$ 在 F 中是闭的，当且仅当它对于弱化的拓扑 $\sigma(F, F')$ 是闭的（IV，p. 4，命题 2）。

#### 推论 1 {#evt-iv-s4-lem-1-cor-1 .statement tag=07UX}

*第假设以下。 1、以下条件等价：*
(i) *u 是严格单射态射 ;*
(ii) *${}^t u$ 是弱拓扑的严格满射态射。*
(iii) *${}^t u$ 是满射。*

蕴涵 (i) $\Rightarrow$ (ii) 紧随 th 的条件 a)、d) 和 e) 的等价而来。 1 和从IV，p. 6，道具。 5. 显然，(ii) 意味着(iii)。最后，我们证明(iii)蕴涵(i)：如果${}^t u$是满射，$u$是a)和e)中的等价的严格态射。 1 ; $u$ 是单射的，由命题得出。 5 个IV、p. 6。

#### 推论 2 {#evt-iv-s4-lem-1-cor-2 .statement tag=07UY}

*第假设以下。 1、以下条件等价：*
(i) *u 是满射；*
(ii) *u 是严格满射态射；*
(iii) *${}^t u$ 是弱拓扑的严格内射态射。*

(i) 和 (ii) 的等价源自 Banach 的 th。 （I，p. 17，第 1）。

鉴于a)和c)中的等价。 1、条件(ii)表示$u$是严格的态射，并且它的像在F中对于$\sigma(F, F')$来说是稠密的。 (ii)和(iii)的等价由a)和d)的等价推出。 1 和来自道具。 5 个IV、p. 6。

如果$u : E \to F$是Fréchet 空间的严格态射，则转置${}^t u$不一定是从$F'_b$到$E'_b$的严格态射（IV，p. 62，执行。 3）。然而，我们得到以下部分结果：

#### 推论 3 {#evt-iv-s4-lem-1-cor-3 .statement tag=07UZ}

— 根据 th 的假设。 1、下面的性质隐含了a)到g)的性质：
h) $^t u$ 是从 $F'_b$ 到 $E'_b$ 的严格态射。
当 E 和 F 均为 Banach 空间或均为 Montel 空间时，性质 h) 等价于 th 的性质 a) 至 g)。 1.
假设$^t u$是从$F'_b$到$E'_b$的严格态射。我们将证明$^t u$的像H在$E'_b$是封闭的，由此cor的第一个断言。 3 将跟随。
令 G 为 F 中 $u$ 的像闭包； 空间 G，加上由 F 分配给它的拓扑，是一个 Fréchet 空间。 映射 $u : E \to F$ 因式分解为 $u = j \circ v$，其中 j 是从 G 到 F 的典范嵌入，并且其中 $v \in \mathscr{L}(E; G)$。然后我们有 $^t u = ^t v \circ ^t j$，其中 $^t j$ 是满射，由 Hahn-Banach th 提出。 （II，p. 24，道具 2）；另外，$^t v$ 是单射的，因为 $v(E)$ 在 G 中是稠密的（IV，p. 6，道具 5）。 假设、映射 $^t u$ 由 $F'_b$ 开往 H 已开通；因为 $^t j$ 是满射且连续的，映射 $^t v$ 诱导是从 $G'_b$ 到 H 的同胚。但是 Fréchet 空间 G 的对偶 $G'_b$ 是完备的（IV，p. 22，道具）。 2）；因而 H 是完备的，因此在 $E'_b$ 内闭合。
如果 E 和 F 是 Montel 空间，则$E'$（分别为 $F'$）重合和拓扑上的强拓扑具有紧收敛性，并且 h) 只是 g) 的重新表述。
如果 E 和 F 是 Banach 空间，则 $E'_b$ 和 $F'_b$ 也是如此，并且条件 h) 等价于 f)，将 a) 和 c) 的等价应用于 $^t u : F'_b \to E'_b$。

#### 推论 4 {#evt-iv-s4-lem-1-cor-4 .statement tag=07V0}

— 假设 E 和 F 是 Banach 空间。对于$^t u$是满射，存在实数$r > 0$使得$\| x \| \leq r. \| u(x) \|$对于所有$x \in E$是必要且充分的。
这只是cor的条件(i)和(iii)的等价的重新表述。 1.

#### 推论 5 {#evt-iv-s4-lem-1-cor-5 .statement tag=07V1}

— 令 E 和 F 为两个 Fréchet 空间，u 为从 E 到 F 的连续线性映射。以下条件是等价的：
a) u 是从 E 到 F 的同构。
b) 对于弱化拓扑，从 E 到 F，u 是同构。
c) 对于弱拓扑，$^t u$ 是从$F'$ 到$E'$ 的同构。
d) 对于强拓扑，$^t u$ 是从$F'$ 到$E'$ 的同构。
e) 从$F'_c$到$E'_c$，$^t u$是同构。
由于同构正是严格双射态射，a) 和 b) 的等价由 th 的条件 a) 和 b) 的等价推出。 1.
很明显，a) 蕴涵条件 c)、d) 和 e) 中的每一个。
相反，假设满足条件 c)、d) 或 e) 之一。由此可见。 1 及其相关。 3 u 是从 E 到 F 的严格态射，并且 $^t u$ 显然是双射的。设 N（分别为 I）为 u 的核（分别为像）。由于 $^t u$ 是双射的，因此我们有 $\operatorname{Im} ^t u = E'$ 和 $\operatorname{Ker} ^t u = \{ 0 \}$，因此通过道具有 $N^\circ = E'$ 和 $I^\circ = \{ 0 \}$。 2 个IV、p. 27。但 N（分别I）是 E（分别F）的闭向量子空间，双极子（II，p. 44）的定理意味着$N = \{ 0 \}$和$I = F$，因此u是双射的。因此我们证明了u是同构。

### 3. 判据满射性

#### 命题 4 {#evt-iv-s4-prop-4 .statement tag=07V2}

— 令 E 和 F 为两个 Fréchet 空间，u 为从 E 到 F 的连续线性映射。以下条件是等价的：

(i) u 是满射的。

(ii) 对于每个半范数$p \in S(E)$，都存在$q \in S(F)$，这样对于每个线性形式$f \in F'$满足$|f \circ u| \leq p$，我们都有$|f| \leq q$。

(iii) 对于每个半范数$p \in S(E)$，存在$q \in S(F)$满足以下性质：如果线性形式$f \in F'$满足$|f \circ u| \leq p$，则$f$在点上为空，其中$q$为空，并且对于所有$y \in F$、$r \in S(F)$，存在$x \in E$和$r(u(x) - y) = 0$。

(iv) 对于每个半范数$p \in S(E)$，我们有

$$
\sup_{\substack{f \in F \\ |f \circ u| \leq p}} |f(y)| < +\infty \quad \text{for all} \quad y \in F .
$$

我们根据以下逻辑概形证明命题

![图表显示 (i)、(ii)、(iii) 和 (iv) 之间的逻辑关系](https://i.imgur.com/3Q5z5QG.png)

如果 $u$ 是满射，则它是严格的态射 (IV, p. 28, th. 1)，则对于每个半范数 $p \in S(E)$，都存在一个半范数 $q \in S(F)$，使得对于所有 $y \in F$ 满足 $q(y) \leq 1$，存在$x \in E$、满足、$p(x) \leq 1$、$u(x) = y$。我们立即推断出 (i) 意味着 (ii) 和 (iii)。显然，(ii) 暗示着(iv)。

为了证明(iii)蕴含(iv)，令$p$和$q$如(iii)中所示。令$y \in F$，由(iii)，在$E$中存在$x$，使得$q(u(x) - y) = 0$。如果$f \in F'$满足$|f \circ u| \leq p$，那么我们有$f(u(x) - y) = 0$，因此

$$
|f(y)| = |f(u(x))| \leq p(x)
$$

且满足关系(1)。

最后我们证明(iv)蕴涵(i)。令$p \in S(E)$和$q$为$f \in F'$满足$|f \circ u| \leq p$的函数$|f|$的上包络线。由(iv)可知，$q$在$F$上是有限的，显然是$F$上的下半连续半范数；由于$F$是桶装的（III、p. 25、推论），所以我们有$q \in S(F)$。让$B_p$（或$B_q$）表示所有$x \in E$（或$y \in F$）中的集合，使得$p(x) \leq 1$（或$q(y) \leq 1$）。我们有$q \circ u \leq p$，所以还有$u(B_p) \subset B_q$。 $F'$中$u(B_p)$的极线由线性形式$f \in F'$组成，因此$|f \circ u| \leq p$，因此$|f| \leq q$；在其他字中，我们得到 $u(B_p)^{\circ} \subset B_q^{\circ}$，最后 $\overline{u(B_p)} = B_q$ 源自双极性的定理（II，p. 45，cor.3）。如果$U$是$E$中0的邻域，则存在$p \in S(E)$使得$B_p \subset U$，因此$F$中0的$\overline{u(U)}$包含邻域$B_q$。这意味着$u$是满射（I，p. 17，th.1）。

#### 推论 {#evt-iv-s4-n3-cor-1 .statement tag=07V3}

— 假设 E 和 F 是 Banach 空间。以下条件是等效的：
(i) u 是满射的。
(ii) 存在实数 r > 0，使得$\|f\| \leq r.\|^{t}u(f)\|$对于所有$f \in F'$。
(iii) 对于所有 $y \in F$，我们有 $\sup_{\substack{f \in F' \\ \|f \circ u\| \leq 1}} |f(y)| < + \infty$。

条件(ii)和(iii)实际上是道具条件(ii)和(iv)的重新表述。 4 代表巴拿赫空间。

### 习题{#evt-iv-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
