---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 4
section_title: Spectra of rings and supports of modules
lang: zh
source: ac-i-vii
book_pages: 94-107, 140-146
pdf_pages: 0114-0127, 0160-0166
extraction: ocr
subsections:
    - "no": 1
      title: IRREDUCIBLE SPACES
      page: 94
      pdf_page: 114
    - "no": 2
      title: NOETHERIAN TOPOLOGICAL SPACES
      page: 97
      pdf_page: 117
    - "no": 3
      title: THE PRIME SPECTRUM OF A RING
      page: 98
      pdf_page: 118
    - "no": 4
      title: THE SUPPORT OF A MODULE
      page: 104
      pdf_page: 124
statements: 49
exercises: 28
content_sha256: cb48bb68c8d4f83af777f61c1993387fd4bba6c96c1554366bbc8dd7c858883c
translated_from: content/en/ac/II/04_s4_spectra_of_rings_and_supports_of_modules.md
translation_method: google
source_content_sha256: aa56aa107c641a6f533bca5b5920334a1f4dfec7d2788424e0037a9fcb53cc7b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: f29a86e1fb438b7f14c564e05c4fbcfbb681f8d63162cd20872fd8c28bc67d3b
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 4. 环的光谱和模的支持

### 1.不可约空间

#### 定义 1 {#ac-ii-s4-def-1 .statement tag=0498}

如果 $X$ 的非空开集合的每个有限交都是非空的，则拓扑空间 $X$ 称为不可约。

通过考虑$X$的开集合的空族，可以看出不可约空间是非空的；对于一个拓扑空间$X$是不可约的，它是非空的并且$X$的两个非空开集合的交总是非空（或者，相当于同一件事，两个闭集合的并不同于$X$ 始终与 $X$ 不同）。

#### 命题 1 {#ac-ii-s4-prop-1 .statement tag=0499}

令$X$为非空拓扑空间。以下条件是等效的：
(a) $X$ 是不可约的；
(b) $X$ 的每个非空开集合都稠密于 $X$；
(c) $X$ 的每个开路集合均已连接。

通过定义，在$X$中密集的集合是集合，满足每个非空开集合，因此(a)和(b)是等价的。 (c) 蕴含 (a) 的是直接的，因为如果$U_1$和$U_2$是不相交的非空开集合，$U_1 \cup U_2$是断开连接集合。最后让我们证明（a）意味着（c）：如果$U$是一个断开的开集集合，它是两个不相交的非空集$U', U''$的并，这两个集在$U$中开集，因此也在$X$中开集，这意味着$X$不是不可约的。

仅当 Hausdorff 空间由单个点组成时，它才是不可约的。

如果 $X$ 的子空间 $E$ 是不可约的，则拓扑空间 $X$ 的子集 $E$ 称为不可约集合。为此，对于集合 $U, V$ 中的每个对在 $X$ 中开放并满足 $E$，$U \cap V$ 也满足 $E$，或者（相当于同一件事），对于每个对集合$F, G$，$X$和满足$E \subset F \cup G$、$E \subset F$或$E \subset G$关闭。通过$n$上的归纳，我们推断，如果$(F_i)_{1 \leq i \leq n}$是$X$的闭集合的有限族，使得$E \subset \bigcup_{i=1}^n F_i$，则存在指标$i$使得$E \subset F_i$。

#### 命题 2 {#ac-ii-s4-prop-2 .statement tag=049A}

在拓扑空间$X$中，对于集合$E$是不可约的，其闭包$\overline{E}$是不可约的并且是充分必要的。

对于$X$的开集合要满足$E$，满足$\overline{E}$是充分必要的；那么命题是从上面的注得出的。

#### 命题 3 {#ac-ii-s4-prop-3 .statement tag=049B}

(i) *如果$X$是不可约空间，则$X$的每个非空开子集都是不可约的。*

(ii) *令$(U_\alpha)_{\alpha \in A}$为开集合的拓扑空间$X$由……组成的非空覆盖，使得$U_\alpha \cap U_\beta = \emptyset$对于指标$(\alpha, \beta)$的每个对。如果集合 $U_\alpha$ 不可约，则空间 $X$ 不可约。*

(i) 如果 $X$ 不可约，$U \subset X$ 非空且在 $X$ 开，$V \subset U$ 非空且在 $U$ 开，$V$ 在 $X$ 也开，因而$X$ 稠密且 *更不必说* 稠密$U$。那么 $U$ 是不可约的 (命题 1)。

(ii) 让我们证明，对于$X$中的每个非空开集合$V$，对于所有$\alpha \in A$，$V \cap U_\alpha \neq \emptyset$：可以得出结论，$V \cap U_\alpha$在$U_\alpha$中稠密，假设，因而$V$在$X$中稠密，并且这证明 $X$ 是不可约的 (命题 1)。现在至少存在一个指标$y$使得$V \cap U_y \neq \emptyset$；因为对于所有$\alpha$和$V \cap U_y$来说$U_\alpha \cap U_y \neq \emptyset$在$U_y$、$U_y \cap V \neq \emptyset$和*更不必说*$U_y \cap V \neq \emptyset$都是稠密的，从而完成了(ii)的证明。

#### 命题 4 {#ac-ii-s4-prop-4 .statement tag=049C}

*令$X$和$Y$是两个拓扑空间和$f$从$X$到$Y$的连续映射。对于$X$的每个不可约子集$E$，$f(E)$是$Y$的不可约子集。*

如果$U, V$是满足$f(E)$的$Y$的两个开集合，则$f^{-1}(U)$和$f^{-1}(V)$是满足$E$的$X$的开集合。因而，$f^{-1}(U) \cap f^{-1}(V) = f^{-1}(U \cap V)$满足$E$，这意味着$U \cap V$满足$f(E)$并证明命题。

#### 定义 2 {#ac-ii-s4-def-2 .statement tag=049D}

*拓扑空间 $X$ 的每个最大不可约子集称为 $X$ 的不可约分量。*

从命题 2 可以得出，$X$ 的每个不可约分量在 $X$ 中都是*封闭*的。

#### 命题 5 {#ac-ii-s4-prop-5 .statement tag=049E}

*设$X$为拓扑空间。 $X$ 的每个不可约子集都包含在 $X$ 的不可约组件中，$X$ 是其不可约组件的并。*

为了证明第一个断言，凭借佐恩的引理，足以证明$X$的不可约子集的集合 3是*归纳*。设$\mathscr{G}$为$\mathfrak{S}$的子集，全包含排序；我们证明集合 $F \in \mathscr{G}$ 的并 $E$ 是不可约的。令$U, V$为满足$E$的两个$X$开集合；由于$\mathscr{G}$是全序的，因此存在集合$F \in \mathscr{G}$满足$U$和$V$；由于$F$是不可约的，$U \cap V$满足$F$，因此也满足$E$，这证明$E$是不可约的，因此3是归纳的。第二个断言紧随第一个，因为单个点的$X$由……组成中的每个子集都是不可约的。

#### 推论{#ac-ii-s4-n1-cor-1 .statement tag=049F}

*拓扑空间 $X$ 的每个连通分量都是 $X$ 的不可约分量的并。*

$X$ 的每个不可约子空间都由命题 1 连接，因此包含在 $X$ 的连通分量中。

注 $X$ 的两个不同的不可约分量在公共的 (习题 11) 中可能有点。

#### 命题 6 {#ac-ii-s4-prop-6 .statement tag=049G}

*设$X$是空间和$(P_i)_{1 \leq i \leq n}$ajinite覆盖$X$由……组成和不可约闭集合。那么$X$的不可约分量是$P_i$的集合的极大元素（相对于包含）。*

我们可以将自己限制在没有两个 $P_i$ 具有可比性的情况。如果$E$是$X$的不可约子集，则$E \subset \bigcup_{i=1}^n P_i$，因此$E$包含在闭集合$P_i$之一中；这证明$P_i$是$X$唯一最大不可约子集。

#### 推论{#ac-ii-s4-n1-cor-2 .statement tag=049H}

*设$X$为拓扑空间和$E$子空间，仅具有不同不可约成分$Q_i$（$1 \leq i \leq n$）的ajinite数；那么$X$中闭包$\overline{E}$的不可约分量是$Q_i$（$1 \leq i \leq n$）的闭包$\overline{Q}_i$和$i \neq j$的$\overline{Q}_i \# \overline{Q}_j$。*

$\overline{E}$ 是 $\overline{Q}_i$ 的并，它们是不可约的 (命题 2)；因为$Q_i$在$E$、$\overline{Q}_i \cap E = Q_i$关闭；作为 $Q_i \notin Q_j$ 对于 $i \neq j$、$\overline{Q}_i \notin \overline{Q}_j$、从而命题 6 的推论。

#### 注 {#ac-ii-s4-n1-rem-1 .statement tag=049I}

假设 $X$ 仅具有不同不可约成分 $X_i$ ($1 \leq i \leq n$) 的 ajinite 数；那么从 $X_i \notin \bigcup_{j \neq i} X_j$ 开始，$U_+ = \mathbf{C}(\bigcup_{j \neq i} X_j)$ 在 $X$ 开，在 $X_i$ 稠密；因此，$U_i$（$1 \leq i \leq n$）是$X$的非空开集合，它们是不可约的（命题2），成对的不相交的，并且它们的并稠密于$X$。

#### 命题 7 {#ac-ii-s4-prop-7 .statement tag=049J}

*设$U$是拓扑空间$X$的开子集。 映射$V \mapsto \overline{V}$（在$X$闭合）是集合的双射和$U$的不可约子集，它们在$U$到集合上闭合并且不可约子集和$X$于$X$关闭并满足$U$； 逆双射是 $Z \mapsto Z \cap U$。特别是，这个双射映射集合 & 不可约分量 & $U$ 到集合 & 不可约分量 & $X$ 满足 $U$。*

如果 $V$ 在 $U$ 内闭且不可约，则 $\overline{V}$ 不可约 (命题 2) 且$V = \overline{V} \cap U$。相反，如果 $Z$ 是不可约且在 $X$ 内闭且满足 $U$，则 $Z \cap U$ 是 $Z$ 的非空开子集，因此不可约 (命题 3) 且在 $Z$ 是稠密的，并且， $Z$已关闭，$Z = \overline{Z} \cap U$。这就证明了命题。

### 2.诺特拓扑空间

#### 定义 3 {#ac-ii-s4-def-3 .statement tag=049K}

如果按包含排序的 $X$ 的每个非空闭集子集具有最小元素，则拓扑空间 $X$ 称为诺特。

这相当于说，$X$的每个非空开集子集，按包含排序，都有极大元素，或者闭集（或开集）集合的每个递减（或递增）序列都是平稳的（集合理论， 章 111、§ 6, no. 5、命题 6)。

#### 命题 8 {#ac-ii-s4-prop-8 .statement tag=049L}

(i) 诺特空间中的每个子空间都是诺特。
(ii) 令 $(A_i)_{i \in I}$ 为拓扑空间 $X$ 的有限覆盖。如果$X$中的子空间$A_i$为诺特，则$X$为诺特。

(i) 设$X$为诺特空间、$X$中的$A$子空间和$A$中的子集中的$(F_i)$递减序列，其闭合时间为$A$；然后是$F_i = \overline{F_n} \cap A$以及$X$形式递减序列中$F_i$的闭包$\overline{F_n}$，以及$X$的已关闭的子集。由于序列是静止的，所以序列 $(F_i)$ 也是静止的。

(ii) 设$(G_n)_{n \geq 0}$为$X$的闭子集的递减序列；到假设时，序列 $(G_n \cap A_i)_{n \geq 0}$ 中的每一个都是静止的。由于$I$是有限的，因此存在整数$n_0$，使得对于$n \geq n_0$，$G_n \cap A_i = G_{n_0} \cap A_i$，对于所有$i \in I$。但是
$$
G_n = \bigcup_{i \in I} (G_n \cap A_i)
$$
因此序列 $(G_n)$ 是静止的，$X$ 是诺特。

#### 命题 9 {#ac-ii-s4-prop-9 .statement tag=049M}

对于拓扑空间 $X$ 为诺特，$X$ 中的每个开集合是拟紧的是必要且充分的。

为了证明条件是必要的，凭借命题8，证明每个诺特空间$X$是拟紧的就足够了。设$(U_i)_{i \in I}$是$X$的开覆盖； 集合 $U_i$ 的有限并的集合非空，因此承认极大元素 $V = \bigcup_{i \in H} U_i$，其中 $H$ 是 $I$ 的有限子集。 定义，$V \cup U_i = V$ 为所有$i \in I$，因此$V = X$。

相反，假设$X$的每个开集合都是拟紧的，并令$(U_i)$为$X$的开子集的递增序列。 $U_i$ 的并 $V$ 是开放的，因此是准紧凑的；由于$(U_i)$是$V$的开覆盖，因此存在$(U_i)$的有限子族，它是$V$的覆盖，因此对于某些指标$n$有$V = U_n$，这证明序列$(U_i)$是平稳的。

#### 引理 1（“诺特归纳中的原理”）{#ac-ii-s4-lem-1 .statement tag=049N}

*令 E 为有序集合，每个非空子集都允许最小元素。令 F 为 E 的子集，并具有以下性质 ：如果 $a \in E$ 使得关系 $x < a$ 蕴含 $x \in F$，则$a \in F$。然后$F = E$.*

假设$F \neq E$；那么$CF$将有一个最小的元素$b$。由定义，$x \in F$为所有$x < b$，这意味着$b \in F$，这是一个矛盾。

#### 命题 10 {#ac-ii-s4-prop-10 .statement tag=049O}

*如果 X 为诺特空间，则 X 的不可约分量集合（以及 X 的连通分量更不必说集合）是有限的。*

足以证明 X 是不可约闭子集的有限并（编号 **1**，命题 6）。让我们证明，诺特归纳的原理可以应用，取E为X的闭子集的集合，按包含排序，F为不可约闭子集的有限并的集合。设Y是X的闭子集，使得Y属于到F的每个闭子集$\neq Y$到F。如果Y是不可约的，则$Y \in F$乘以定义；否则，Y 是与 Y 不同的两个闭子集 $Y_1,\ Y_2$ 的并。则 F 的$Y_1 \in F$ 和$Y_2 \in F$ 乘以假设，从而 $Y \in F$ 乘以定义。

特别是，*Hausdorff* 诺特空间必然是“有限”。

### 3. 环的主光谱

设A为A的素理想的环和X集合。对于A的每个子集M，我们用包含M的素理想$V(M)$集合来表示；显然，如果$a$是M生成的A的理想，则$V(M) = V(a)$；如果 M 由单个元素 f 组成，我们写 $V(f)$ 而不是 $V(\{f\})$，我们就有 $V(f) = V(Af)$。 映射$M \mapsto V(M)$关于包含在A和X中是*递减*。此外，以下公式成立：

(1)
$$
V(0) = X, \quad V(1) = O;
$$

(2)
$$
V\left(\bigcup_{i \in I} M_i\right) = V\left(\sum_{i \in I} M_i\right) = \bigcap_{i \in I} V(M_i)
$$
对于 A 的每个家庭 $(M_i)_{i \in I}$ 子集；

(3)
$$
V(a \cap a') = V(aa') = V(a) \cup V(a')
$$
对于A中的每一个对理想$a,\ a'$。公式 (1)和(2)是明显的；另一方面，公式(3)意味着，对于A的素理想$p$到包含理想$a$或$a'$之一，它包含$aa'$或包含$a \cap a'$是充分必要的；那么它是§ 1, no. 1、命题 1 的推论。第二个公式 (1) 具有以下逆命题：如果$a$ 是$A$ 的理想，使得$V(a) = \varnothing$，则$a = A$，因为没有最大理想$A$包含$a$。最后，如果 $a$ 是 $A$ 的理想且 $r(a)$ 是它的*根式*（$§ 2$、no. 6、定义 4），那么

$$
V(a) = V(r(a))
$$

如下从$§ 2$，no. 6，推论1到命题13。

公式 (1) 到 (3) 表明 $X$ 满足的子集 $V(M)$ 拓扑的 * 闭集合* 公理 (*一般拓扑*, 章 I, $§ 1$, no. 4）。

#### 定义 4 {#ac-ii-s4-def-4 .statement tag=049P}

*令$A$为环。 $A$素理想的集合$X$，其中拓扑的闭集合为集合$V(M)$，其中$M$贯穿$\mathfrak{P}(A)$，称为$A$的素谱，记为$\mathrm{Spec}(A)$。这样定义的拓扑称为 $X$ 上的光谱或 Zariski 拓扑。*

显然关系$\mathrm{Spec}(A) = \varnothing$等价于$A = \{0\}$。

设$X$为环$A$的素谱；对于所有$f \in A$，让我们用$X_f$集合表示$A$的素理想*而不是包含*$f$；那么$X_f = X - V(f)$和$X_f$因此是一个*开*集合。根据(2)，$X$的每个闭子集是形式$V(f)$的闭集合的交，因此谱拓扑的$X$，形式a *基* $X$。此外，从定义可以立即得出：

$$
X_0 = O,\quad X_1 = X,
$$

更一般地，$A$中每可逆元$f$对应$X_{f^{-1}} = X$；

$$
X_{g^{-1}} = X, nX, \quad \text{for all } f, g \text{ in } A.
$$

对于$X$的每个子集$Y$，让我们用$\mathfrak{J}(Y)$交表示$A$的素理想，其中属于到$Y$。显然，$\mathfrak{J}(Y)$是$A$的理想，映射$Y \mapsto \mathfrak{J}(Y)$是*递减*关于包含在$X$和$A$中。明显关系

$$
\mathfrak{J}(\varnothing) = A
$$
$$
\mathfrak{J}\left( \bigcup_{\lambda \in L} Y_\lambda \right) = \bigcap_{\lambda \in L} \mathfrak{J}(Y_\lambda)
$$

为每个家庭持有$X$子集$(Y_\lambda)_{\lambda \in L}$。此外：

#### 命题 11 {#ac-ii-s4-prop-11 .statement tag=049Q}

*令$A$为环，$a$为$A$的理想，$Y$子集为$X = \mathrm{Spec}(A)$。
(i) $V(a)$ 在 $X$ 中闭合，$\mathfrak{J}(Y)$ 是 $A$ 的理想，等于其根式。
(ii) $\mathfrak{J}(V(a))$ *是* $a$ *的根式，并且* $V(\mathfrak{J}(Y))$ *是* $Y$ *在* $X$中的闭包。

(iii) 映射 3 和 V 定义递减双射，其中一个是另一个的逆，位于 X 的闭子集的集合和 A 的理想集合之间，且等于其根式。

断言 (i) 和 (ii) 的第一个断言是从定义和 § 2, no. 6 得出的，推论 1 到命题 13。如果有一个封闭的集合 V(M)（对于某些 M ⊂ A）包含 Y，则对于每个素理想，M ⊂ p p ∈ Y, 从而 M ⊂ J(Y) 因而 V(M) ⊃ V(J(Y))；因为 Y ⊂ V(J(Y))，V(J(Y)) 是 X 包含 Y 的最小的闭集合，从而完成 (ii) 的证明。最后，从 (ii) 可以得出，如果 a 是等于其根式的素理想，则 J(V(a)) = a，如果 Y 闭于 X，则 V(J(Y)) = Y；这就证明了(iii)。

从命题 11 可以立即得出，如果 M 是 A 的任意子集并且 Y 是 X 的任意子集，则 V(M) = V(J(V(M))) 且 J(Y) = J(V(J(Y)))。

#### 推论 1 {#ac-ii-s4-prop-11-cor-1 .statement tag=049R}

对于 X 的闭子集的每个族 (Y_λ)_{λ ∈ L}，J(∩_{λ ∈ L} Y_λ) 是理想 J(Y_λ) 的和的根式。

由命题 11 (iii) 可知 J(∩_{λ ∈ L} Y_λ) 是最小的理想，等于它的根式，且包含所有 J(Y_λ)；这个理想则包含 Σ_{λ ∈ L} J(Y_λ) ，因此也是 Σ_{λ ∈ L} J(Y_λ) 的根式（§ 2, no. 6，推论 2 到命题 13），从而推论。

#### 推论 2 {#ac-ii-s4-prop-11-cor-2 .statement tag=049S}

设 r(a) 表示 A 的理想 a 的根式；如果 a 和 b 是 A 的两个理想，则关系 V(a) ⊂ V(b) 等价于 b ⊂ r(a) 和 r(b) ⊂ r(a)。

直接的关系 b ⊂ r(a) 和 r(b) ⊂ r(a) 是等价的，并且，当 V(a) = V(r(a)) 时，推论立即从命题 11, (iii) 得出。

#### 推论 3 {#ac-ii-s4-prop-11-cor-3 .statement tag=049T}

令 (f_λ)_{λ ∈ L} 为 A 的元素族。对于元素 g ∈ A 到满足 X_g ⊂ ∪_{λ ∈ L} X_{f_λ}，存在整数 n > 0 且 g^n 是充分必要的属于为 f_λ 生成的理想值。

关系 X_g ⊂ ∪_{λ ε L} X_{f_λ} 等价于 V(g) ⊃ ∩_{λ ∈ L} V(f_λ) 并且应用推论 2 就足够了。

推论 4，对于 A 的两个元素 f, g 到满足 X_f = X_g，存在两个整数 m > 0, n > 0 使得 f^m ∈ Ag 且 g^n ∈ Af 是充分必要的。

#### 推论 5 {#ac-ii-s4-prop-11-cor-5 .statement tag=049U}

对于$f \in A$到满足$X_f = \varnothing$，$f$幂零是充分必要的。

这直接从推论 4 得出。

#### 推论 6 {#ac-ii-s4-prop-11-cor-6 .statement tag=049V}

点$p \in X = \mathrm{Spec}(A)$的集合由……组成的闭包是素理想包含$p$的集合$V(p)$。对于集合 $\{p\}$ 在 $X$ 的闭点（或者，正如我们也会滥用语言所说，$p$ 是 $X$ 的闭点），$p$ 是最大值是必要且充分的。

#### 推论 7 {#ac-ii-s4-prop-11-cor-7 .statement tag=049W}

如果 $A$ 为诺特环，则 $X = \mathrm{Spec}(A)$ 为诺特空间。

#### 命题 12 {#ac-ii-s4-prop-12 .statement tag=049X}

对于所有$f \in A$，$X = \mathrm{Spec}(A)$中的开集合$X_f$是拟紧的；特别是，空间$X$是准紧的。

作为拓扑的$X_g$形式基，足以证明，如果$(g_\lambda)_{\lambda \in L}$是$A$的元素的族，使得$X_f \subset \bigcup_{\lambda \in L} X_{g_\lambda}$，则存在有限子族$(g_{\lambda_i})_{i \in I}$使得$X_f = \bigcup_{i \in I} X_{g_{\lambda_i}}$。但关系$X_f = \bigcup_{\lambda \in L} X_{g_\lambda}$意味着存在整数$n > 0$和有限子族$(g_{\lambda_i})_{i \in I}$，使得“f”属于达到该子族生成的理想（推论3至命题11）； 从而命题。

#### 命题 13 {#ac-ii-s4-prop-13 .statement tag=049Y}

设$A, A'$是从$A$到$A'$的两个环、$X = \mathrm{Spec}(A), X' = \mathrm{Spec}(A')$和$h$同态； 映射 $^a h : p' \mapsto \overline{h}(p')$从$X'$到$X$是连续的。

对于$M \subset A$，集合$(^a h)^{-1}(V(M))$是$A'$的素理想$p'$的集合，使得$M \subset \overline{h}(p')$，相当于$h(M) \subset p'$；那么这个集合等于$V(h(M))$，因此是封闭的。

我们称$^a h$映射与同态$h$相关联。

#### 注 {#ac-ii-s4-n3-rem-1 .statement tag=049Z}

如果$h$是满射并且$a$是它的核，则从谱拓扑的定义得出$^a h$是$X'$到闭子空间$V(a)$的同胚$X$；对于$A'$的素理想$p'$到包含理想的$b'$$A'$，$\overline{h}(p')$包含$\overline{h}(b')$是充分必要的；我们首先看到$^a h$是单射的，取$b'$为素数；此外，对于$A'$的每个理想$b'$，$V(b')$的$^a h$下的像来说，$V(\overline{h}(b'))$，从而我们的断言，形式$\overline{h}(b')$的理想都是$A$ 其中包含 $a$。

#### 推论 {#ac-ii-s4-n3-cor-1 .statement tag=04A0}

令$S$为$A$、$A' = S^{-1}A$和$h$典范同态$i_A^S$的乘法子集；那么$^a h$是$X' = \mathrm{Spec}(A')$到$X = \mathrm{Spec}(A)$由……组成的子空间的同胚，$A$的素理想不满足$S$。

设$f' = f/s$，其中$f \in A, s \in S$；那么 $X'_{f'} = X'_{f/1}$ 因为 $s/1$ 在 $A'$ 中是可逆的。我们已经知道$^a h$是单射的，并且对于所有$p' \in X'$，关系$f/1 \in p'$和$f \in h^{-1}(p') = ^a h(p')$是等价的，因此条件$p' \in X'_{f/1}$和$^a h(p') \in X_f$是等价的；这表明$^a h(X'_{f'})$等于$X_f \cap ^a h(X')$，从而等于第一个断言，因为$X$的拓扑的$X, (resp.\ X'_{f'})$形式基（分别为$X$）。第二个断言源自 , no. 5, 命题 11 (ii)

#### 命题 14 {#ac-ii-s4-prop-14 .statement tag=04A1}

*设$A$为环。为了使 $X = \mathrm{Spec}(A)$ 的子集 $Y$ 不可约，理想的 $\mathfrak{J}(Y)$ 为素数是充分必要的。*

写$p = \mathfrak{J}(Y)$，我们注，对于元素$f \in A$，关系$f \in p$相当于$Y \subset V(f)$。假设$Y$是不可约的，并令$f, g$是$A$的元素，使得$fg \in p$。然后
$$
Y \subset V(fg) = V(f) \cup V(g);
$$
由于$Y$是不可约的，并且$V(f)$和$V(g)$是闭集，$Y \subset V(f)$或$Y \subset V(g)$，因此$f \in p$或$g \in p$，这证明$p$是素数。

现在假设$p$是素数；那么 $\overline{Y} = V(p)$ (命题 11 (ii)) 并且，由于 $p$ 是质数，$p = \mathfrak{J}(\{p\})$、从而 $\overline{Y} = V(\mathfrak{J}(\{p\})) = \{p\}$ (命题 11 (ii))。由于单个点的集合由……组成是不可约的，$Y$是不可约的（no. 1，命题2）。

#### 推论 1 {#ac-ii-s4-prop-14-cor-1 .statement tag=04A2}

*要使环$A$使得$X = \mathrm{Spec}(A)$不可约，$A$与其零根$\mathfrak{N}$的商为整环是必要且充分的。*

由命题 11 (i)，$\mathfrak{J}(X)$是理想$(0)$的根式，即$\mathfrak{N}$。

#### 推论 2 {#ac-ii-s4-prop-14-cor-2 .statement tag=04A3}

*The mapping $p \mapsto V(p)$ is a bijection of $X = \mathrm{Spec}(A)$ onto the set of irreducible closed subsets of $X$; in particular the irreducible components of a closed subset $Y$ of $X$ are the sets $V(p)$, where $p$ runs through the set of minimal elements of the set of prime ideals of $A$ which contain $\mathfrak{J}(Y)$.*

对于$A$的每个素理想$p$和$Y = V(\mathfrak{J}(Y))$对于$X$的每个闭子集$Y$来说$\mathfrak{J}(V(p)) = p$，第一个断言是从命题14得出的； on the other hand, for $Y \supset V(p)$, it is necessary and sufficient that
$$
p = \mathfrak{J}(V(p)) \supset \mathfrak{J}(Y)
$$
（命题11），从而第二个断言。

#### 推论 3 {#ac-ii-s4-prop-14-cor-3 .statement tag=04A4}

*集合 of minimal prime ideals of 诺特环 $A$ is finite.*

$X = \mathrm{Spec}(A)$只有有限的数不可约分量（推论7到命题11和no. 2，命题10），并且推论来自上面的推论2。

#### 命题 15 {#ac-ii-s4-prop-15 .statement tag=04A5}

令 $A$ 为环，$I$ $A$ 幂等$e_i \neq 0$ 的正交族$(e_i)_{i \in I}$ 的有限集合和$E$ 集合，使得$\sum_{i \in I} e_i = 1$。 For all $(e_i)_{i \in I} \in E$, we 集合 $\overline{\omega}((e_i)_{i \in I}) = (\mathrm{V}(A(1 - e_i)))_{i \in I}$, $\sigma((e_i)_{i \in I}) = (Ae_i)_{i \in I}$. Then $\overline{\omega}$ is 双射 of $E$ onto 集合 $P$ of 划分 $(U_i)_{i \in I}$ of $X = \mathrm{Spec}(A)$ into open 集合 and $\sigma$ is 双射 of $E$ onto 集合 $S$ of families $(a_i)_{i \in I}$ of ideals $\neq 0$ of $A$ such that $A$ is 直和 of the $a_i$.

Let $(e_i)_{i \in I}$ be 元素 of $E$ and 集合 $Y_i = \mathrm{V}(A(1 - e_i))$; if $i \neq j$, then $1 = 1 - e_i + e_i(1 - e_j) \in A(1 - e_i) + A(1 - e_j)$, 从而 $Y_i \cap Y_j = \varnothing$ (公式 (1) and (2)).另一方面，

$$
\bigcup_{i \in I} Y_i = \mathrm{V}\left( \prod_{i \in I} A(1 - e_i) \right)
$$

(公式(3));

by 假设 $\prod_{i \in I} (1 - e_i) = 1 - \sum_{i \in I} e_i = 0$, 从而 $\bigcup_{i \in I} Y_i = X$ (公式 (I)). As the $Y_i$ are closed, they are also open, 从而 $\overline{\omega}(E) \subset P$.另外，显然$A = \sum_{i \in I} Ae_i$； if $0 = \sum_{i \in I} a_i e_i$ where $a_i \in A$, we obtain, by multiplying by $e_i$, $O = a_i e_i^2 = a_i e_i$ for all $i$;这证明了$\sigma(E) \subset S$。

#### 引理 2 {#ac-ii-s4-lem-2 .statement tag=04A6}

*如果* $e, f$ *是* $A$ *的两个幂等，使得* $Ae$ *和* $Af$ *具有相同的根式*，则$e = f$。

假设整数 $m \geq 0, n \geq 0$ 存在$e = e^m \in Af$ 和 $f = f^n \in Ae$；设$x, y$为$A$的元素，使得$e = xf, f = ye$；然后$ef = x^2 = x = e$，类似地$ef = ye^2 = ye = f$，从而$e = f$。

引理 2 和推论 2 到命题 11 表明映射 $\overline{\omega}$ 和 $\sigma$ 是*内射*。

让我们证明 $\sigma$ 是满射的。如果$(a_i)_{i \in I}$是$S$的元素，则有元素$e_i \in a_i$使得$1 = \sum_{i \in I} e_i$；如果$i \neq j$，则$e_i e_j \in a_i \cap a_j = \{0\}$，从而

$$
e_i = \sum_{j \in I} e_i e_j = e_i^2;
$$

最后，$Ae_i \subset a_i$，对于所有$i \in I$和$\sum_{i \in I} Ae_i = A$，从而$Ae_i = a_i$。

仍有待证明 $\overline{\omega}$ 是满射。设$(U_i)_{i \in I}$为$P$和集合$Z_i = \bigcup_{j \neq i} U_j$中的元素；由于 $U_i$ 和 $Z_i$ 是闭合的，因此存在 $A$ 的理想$a_i, b_i$，使得 $U_i = \mathrm{V}(a_i), Z_i = \mathrm{V}(b_i)$。现在我们证明可以进一步假设 $a_i \cap b_i = 0$。现在$U_i \cap Z_i = \varnothing$、从而$a_i + b_i = A$；令 $a_i, b_i \in a_i, b_i$ 使得$a_i + b_i = 1$。那么$X = U_i \cup Z_i = \mathrm{V}(a_i b_i)$(公式(3));因此，$a_i b_i$的每一个元素都是幂零的（推论2到命题11）；令$p$为整数，使得$a_i^p b_i^p = 0$。然后$U_i \subset \mathrm{V}(Aa_i) = \mathrm{V}(Aa_i^p)$，

$$
Z_i \subset \mathrm{V}(Ab_i) = \mathrm{V}(Ab_i^p)
$$

和$V(Aa_i) \cap V(Ab_i) = V(Aa_i + Ab_i) = \varnothing$，因此有$U_i = V(Aa_i^p)$和$Z_i = V(Ab_i^p)$，从而通过替换建立我们的断言，通过$Aa_i^p$建立$a_i$，并通过$Ab_i^p$建立$b_i$。由此选择理想$a_i$和$b_i$，从$\sigma$是双射的事实可以得出，存在两个幂等$f_i \in a_i, e_i \in b_i$使得$1 = e_i + f_i, e_i f_i = 0, a_i = Af_i, b_i = Ae_i$。如果$i \neq j$，则$X = Z, \cup Z_j = V(Ae_i e_j)$，并且由于$e_i e_j$是幂等的，引理2表明$e_i e_j = 0$。最后$e = \sum_{i \in I} e_i$是幂等的，$e_i \in Ae$对于所有$i \in I$，从而$V(Ae) \subset Z$，对于所有$i$；由此可见

$$
V(Ae) = \varnothing = V(A.1)
$$

引理 2 也表明$e = 1$。

#### 推论 1 {#ac-ii-s4-lem-2-cor-1 .statement tag=04A7}

令$A$为环，$r$为$A$和$h : A \to A/r$典范同态的零理想。对于$A/r$幂等的每个有限正交族$(e'_i)_{i \in I}$，使得$\sum_{i \in I} e'_i = 1$，存在一个$A$幂等的有限正交族$(e_i)_{i \in I}$，使得对于所有$i \in I$都有$\sum_{i \in I} e_i = 1$和$h(e_i) = e'_i$。

我们写$A' = A/r$。我们知道（注紧随命题13）

$$
ah : \operatorname{Spec}(A') \to \operatorname{Spec}(A)
$$

是一个同胚，$A$包含$r$乘假设的每个素理想。 命题 15 表明，$A$ 中存在一个幂等的有限正交族 $(e_i)_{i \in I}$，使得$\sum_{i \in I} e_i = 1$ 以及$V(A'(1 - e'_i))$ 的$ah$ 下的像为$V(A(1 - e_i))$。但显然 $V(A(1 - e_i))$ 也是 $ah$ 下的像

$$
V(A'(1 - h(e'_i)));
$$

由于$1 - e'_i$和$1 - h(e_i)$是幂等的，引理2表明$e'_i = h(e_i)$、从而的推论。

#### 推论 2 {#ac-ii-s4-lem-2-cor-2 .statement tag=04A8}

对于要连接的环$A$的素谱$X = \operatorname{Spec}(A)$来说，$A$包含除了$0$和$1$之外没有幂等是充分必要的。

说$X$不连通，意味着$X$存在集合，它是开闭的，与$\varnothing$和$X$不同。

### 4. 模的支持

#### 定义 5 {#ac-ii-s4-def-5 .statement tag=04A9}

令 $A$ 为环且 $M$ 为 $A$ 模块。 $A$的素理想$p$的集合，使得$M_p \neq 0$称为$M$的支撑，记为$\operatorname{Supp}(M)$。

由于$A$的每个最大理想都是素数，因此从§ 3, no. 3，推论2到定理1，$A$模$M$等于$0$，$\operatorname{Supp}(M) = \varnothing$是充分必要的。

#### 例 {#ac-ii-s4-n4-exa-1 .statement tag=04AA}

令$a$为$A$的理想；在记号/no. 3中，我们有
$$
V(a) = \operatorname{Supp}(A/a).
$$
如果 $p$ 是 $A$ 的质数，使得 $a \notin p$，则 $(A/a)_p = 0$ (§ 3, no. 1, 注 3)；另一方面，如果$a \subset p$、$aA_p$包含在$A$的最大理想$pA_p$中，且$(A/a)_p$同构于$A_p/aA_p$，因此不为零（§ 3, no. 1、命题3）； 从而我们的断言。
特别是$\operatorname{Supp}(A) = \operatorname{Spec}(A)$。

#### 命题 16 {#ac-ii-s4-prop-16 .statement tag=04AB}

令 $A$ 为环且 $M$ 为 $A$ 模块。
(i) *如果 $N$ 是子模 / $M$，则*
$$
\operatorname{Supp}(M) = \operatorname{Supp}(N) \cup \operatorname{Supp}(M/N).
$$
(ii) *如果 $M$ 是子模家庭$(N_i)_{i \in I}$ 的和，则*
$$
\operatorname{Supp}(M) = \bigcup_{i \in I} \operatorname{Supp}(N_i).
$$
(i) 从正合序列 $0 \to N \to M \to M/N \to 0$，我们推导出对于 $A$ 的每个素理想 $p$，正合序列
$$
0 \to N_p \to M_p \to (M/N)_p \to 0
$$
（§ 2, no. 4，定理1）。对于$M$而言，要减少到0，$N_p$和$(M/N)_p$是必要且充分的。在其他字中，关系$p \notin \operatorname{Supp}(M)$等价于“p$\notin \operatorname{Supp}(N)$和$p \notin \operatorname{Supp}(M/N)$”，从而证明了(i)。
(ii) 对于$A$、$M$的每个素理想$p$，都是子模$(N_i)_p$ (§ 2, no. 4)族的和。说$M, \neq 0$意味着存在$i \in I$使得$(N_i)_p \neq 0$，从而 (ii)。

#### 推论{#ac-ii-s4-n4-cor-1 .statement tag=04AC}

*令$A$为环，$M$为$A$模，$M$的生成元为$(m_i)_{i \in I}$系统，以及$a$，$m_i$的湮没子。然后*
$$
\operatorname{Supp}(M) = \bigcup_{i \in I} V(a_i).
$$
$\operatorname{Supp}(M) = \bigcup_{i \in I} \operatorname{Supp}(Am_i)$ 命题 16 (ii)。另一方面，$Am_i$与$A$模块$A/a_i$同构的，我们已经看到
$$
\operatorname{Supp}(A/a_i) = V(a_i)
$$
（上面例）。

#### 命题 17 {#ac-ii-s4-prop-17 .statement tag=04AD}

*令$A$为环，$M$为$A$模块，$a$为湮没子；如果 $M$ 是有限生成的，则* $\operatorname{Supp}(M) = V(a)$ *和* $\operatorname{Supp}(M)$ *因此封闭于* $\operatorname{Spec}(A)$。
令$(m_i)_{1 \leq i \leq n}$为$M$生成元系统且令$a$为$m_i$湮没子；然后$a = \bigcap_{i=1}^n a_i$，因此$V(a) = \bigcup_{i=1}^n V(a_i)$（no. 3，方程（3））和命题从推论得出命题16。

#### 推论 1 {#ac-ii-s4-prop-17-cor-1 .statement tag=04AE}

令$A$为环，$M$为有限生成的$A$模块，$a$元素为$A$。对于$a$到属于，对于$M$支持的每个素理想，$M$的位似与比率$a$是幂幂的充要条件。

由命题 17 可知，素理想属于到$\operatorname{Supp}(M)$ 的交是$M$ 湮没子 $a$ 的根式（no. 3，命题 11 (ii)）。说$a$属于这个部首相当于说，存在幂$a^k \in a$，因此存在$a^k M = 0$。

#### 推论 2 {#ac-ii-s4-prop-17-cor-2 .statement tag=04AF}

令$A$为诺特环，$M$为有限生成的$A$模，$a$为$A$的理想。对于$\operatorname{Supp}(M) \subset V(a)$，存在整数$k$使得$a^k M = 0$是充分必要的。

如果$b$是$M$的湮没子，则关系$\operatorname{Supp}(M) \subset V(a)$等于$V(b) \subset V(a)$乘命题17，因此等于$a \subset r(b)$，其中$r(b)$是$b$的根式（no. 3，推论 2 至命题 11）。由于$A$是诺特，所以这个条件也等价于整数$k > 0$的存在使得$a^k \subset b$(§ 2, no. 6，命题15)。

#### 命题 18 {#ac-ii-s4-prop-18 .statement tag=04AG}

设$M, M'$是有限生成模除环$A$；那么

$$
\operatorname{Supp}(M \otimes_A M') = \operatorname{Supp}(M) \cap \operatorname{Supp}(M').
$$

我们需要证明，如果$p$是$A$的素理想，则关系$(M \otimes_A M')_p \neq 0$与“$M_p \neq 0$和$M'_p \neq 0$”等价。由于$A_p$-模块$M, \otimes_{A_p} M'_p$和$(M \otimes_A M')_p$是同构的（§ 2, no. 7，命题18），我们的断言来自以下引理：

#### 引理 3 {#ac-ii-s4-lem-3 .statement tag=04AH}

令$B$为局部环以及$E$和$E'$两个有限生成的$B$模块。如果$E \neq 0$和$E' \neq 0$，则$E \otimes_B E' \neq 0$。

设$k$为$B$的剩余类域。凭借§ 3, no. 2、命题4、$k \otimes_B E \neq 0$和$k \otimes_B E' \neq 0$；然后我们推断

$$
(k \otimes_B E) \otimes_k (k \otimes_B E') \neq 0
$$

（代数、章II, § 3, no. 7）。但是，由于张量积是结合律（参见上文，§ 3, no. 8），因此张量积同构于

$$
E \otimes_B ((k \otimes_k k) \otimes_B E') = E \otimes_B (k \otimes_B E')
$$

因此到$k \otimes_B (E \otimes_B E')$、从而引理。

#### 推出{#ac-ii-s4-n4-cor-2 .statement tag=04AI}

令 $M$ 为有限生成的 $A$ 模块，$n$ 为湮没子。对于 $A$、$\operatorname{Supp}(M/aM) = V(a) \cap V(n) = V(a + n)$ 的每个理想 $a$。

$M/aM = M \otimes_A (A/a)$ 和 $A/a$ 是有限生成的。

#### 命题 19 {#ac-ii-s4-prop-19 .statement tag=04AJ}

令 $A, B$ 为两个环、$\phi : A \to B$ 同态且
$$
^{a}\phi : \operatorname{Spec}(B) \to \operatorname{Spec}(A)
$$
与 $\phi$ (命题 13) 关联的连续映射。对于每个$A$-模块$M$，
$$
\operatorname{Supp}(M_{(B)}) \subset ^{a}\phi(\operatorname{Supp}(M)) ; \text{if also } M \text{ is finitely generated, then}
$$
$$
\operatorname{Supp}(M_{(B)}) = ^{a}\phi^{-1}(\operatorname{Supp}(M)).
$$
设$q$为$B$和$p = \phi^{-1}(q)$的素理想。假设$q$属于到$\operatorname{Supp}(M_{(B)})$；然后$M_{(B)} \otimes_B B_q = (M \otimes_A B) \otimes_B B_q = M \otimes_A B_q = (M \otimes_A A_p) \otimes_A B_q$，从同态$A \to B \to B_q$因子变为$A \to A_p \to B_q$（§ 2, no. 1，命题2）；因此，假设$M_{(B)} \otimes_B B_q \neq 0$意味着$M \otimes_A A_q \neq 0$，从而第一个断言。由于同态$\phi_q : A_p \to B_q$是本地的，第二个断言来自以下引理：

#### 引理 4 {#ac-ii-s4-lem-4 .statement tag=04AK}

令$A, B$为两个局部环，$p : A \to B$为本地同态，$E$为有限生成的$A$模块。如果$E \neq 0$，则$E_{(B)} \neq 0$。

设$m$为$A$和$k = A/m$剩余类域的最大理想； 假设意味着$B \otimes_A k = B/mB \neq 0$；由于张量积是结合律，$(E \otimes_A B) \otimes_A k$与$E \otimes_A (B \otimes_A k)$同构的，因此也与$E \otimes_A (k \otimes_k (B \otimes_A k))$同构的，最后与$(E \otimes_A k) \otimes_k (B \otimes_A k)$同构的； § 3, no. 2、命题 4、$E \otimes_A k \neq 0$，因此$(E \otimes_A B) \otimes_A k \neq 0$（代数、章 II, § 3, no. 7）和更不必说 $E \otimes_A B \neq 0$。

#### 命题 20 {#ac-ii-s4-prop-20 .statement tag=04AL}

令 $A$ 为环且 $M$ 为有限生成的 $A$ 模块。对于每个素理想$p \in \operatorname{Supp}(M)$，都存在一个非零$A$同态$w : M \to A/p$。

让$p \in \operatorname{Supp}(M)$。由于$M$是有限生成的并且$M_p \neq 0$，
$$
M_p/pM_p = M_p \otimes_A (A_p/pA_p) \neq 0
$$
（§ 3, no. 2，命题4）。设$K = A_p/pA_p$为整环$A/p$分数域；由于 $M_p/pM_p$ 比 $K$ 向量空间更小，且未减至 0，因此存在非零线性形式 $u : M_p/pM_p \to K$。如果$(x_i)_1 <_n^*$是$M$的生成元系统，$x_i$的$\bar{x}_i$像，则在$(A/p)$-模$M_p/pM_p$中，存在元素$\alpha \neq 0$ $A/p$使得$\alpha u(\bar{x}_i)$属于到$A/p$对于$1 \leq i \leq n$；因此$v = \alpha u$是从$M_p/pM_p$到$A/p$的非零$(A/p)$线性映射。 合成
$$
w : M \longrightarrow M, \longrightarrow M_p/pM_p \overset{v}{\longrightarrow} A/p
$$
因此是所需的同态。

### 习题{#ac-ii-s4-exercises}

(b) 令 $n = \dim(M)$。 维数 1（或$n - 1$）的 M 中的直因子称为*线*（或超平面）。如果 M 中存在超平面 H，其元素在 $u$ 下不变，则自同构 $u \in \mathbf{GL}(M)$ 与恒等式不同，称为*横传*；那么$u(x) = x + a\phi(x)$，其中$\phi$是M上的线性形式，使得$H = \mathrm{Ker}(\phi)$和$a \in H$；获得逆命题。如果 A 是可交换的，则证明行列式 1 的每个自同构 $u \in \mathbf{GL}(M)$ 都是乘积平移（观察到，在 $u$ 的矩阵中，相对于 M 的任何基，每列包含至少有一个A 的可逆元和形式 $I + E_{ij} \ (i \neq j)$ 的矩阵是平移的矩阵）。

(c) 给出自同构$u \in \mathbf{GL}(M)$的例，使得$1 - u$的核不是M的直因子（取A为正式幂级数的局部环$K[[X]]$） 域 K 和 $M = A$ 上的一个不确定值）。

(d) 给出直因子 N 的例，M 的 P（必须是自由的），使得 $N + P$ 和 $N \cap P$ 不是 M 的直因子。（取 $A = K[X]/(X^2)$，其中 K 是域和 $M = A^2$。）

¶ 15. 设 A 为（可交换的）环，M A-模。

(a) 为了使 M 的子模 M' 是纯的（章 I, § 2，习题 24），对于 A 的每个最大理想$m$，$M'_m$ 是 $M_m$ 的纯子模（使用定理 1）是充分必要的no. 3）。

(b) 假设 A 为局部环，最大理想为 $m$，M 为有限生成的自由A-模。对于 M 的有限生成的子模 M' 来说，它是 M 的直因子是充分必要的。（使用 no. 2、约化到证明的推论 1 到命题 5，如果 $M' \subset mM$、$M'$ 只能是如果 $M' = 0$，则为 M 的纯子模。）

16. 令$(A_\lambda, f_{\mu\lambda})$为局部环的直接系统，使得$f_{\mu\lambda}$是本地同态；设$m_\lambda$为$A_\lambda$和$K_\lambda = A_\lambda/m_\lambda$的最大理想。那么$A = \varprojlim A_\lambda$就是局部环，其最大理想是$m = \varprojlim m_\lambda$，剩余类域就是$\bar{K} = \varprojlim K_\lambda$。此外，如果$m_\mu = A_\mu m_\lambda$适用于$\lambda < \mu$，则$m = Am$适用于所有$\lambda$。

94

§ 4](exercises/s4/)参见[习题。
