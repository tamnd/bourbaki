---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 1
section_title: Bornology in a topological vector space
lang: zh
source: evt-i-v
pdf_pages: 0133-0143, 0169-0172
extraction: ocr
subsections:
    - "no": 1
      title: Bornologies
      page: 0
      pdf_page: 133
    - "no": 2
      title: Bounded subsets of a topological vector space
      page: 2
      pdf_page: 134
    - "no": 3
      title: Image under a continuous mapping
      page: 4
      pdf_page: 136
    - "no": 4
      title: Bounded subsets in certain inductive limits
      page: 5
      pdf_page: 137
    - "no": 5
      title: The spaces $E_A$ (A bounded)
      page: 7
      pdf_page: 139
    - "no": 6
      title: Complete bounded sets and quasi-complete spaces
      page: 8
      pdf_page: 140
    - "no": 7
      title: Examples
      page: 9
      pdf_page: 141
statements: 30
exercises: 18
content_sha256: 3790a77d702a78671fe577fc4681fef51564ea3bce8c77fba5d0e842731c6b05
translated_from: content/en/evt/III/01_s1_bornology_in_a_topological_vector_space.md
translation_method: google
source_content_sha256: 4e7875bd1f38c0a02c517e1a85849c5df0ef1b2158b71d579dbe784bbc3c6f54
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: c2c102164c1d043dce55ec395ea905a690768a50747a4e7ad1f2b9be6142cffd
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。拓扑中的出生学向量空间

### 1. 出生学

#### 定义 1 {#evt-iii-s1-def-1 .statement tag=07KW}

— *A bornology on a set* $E$ *is a subset* $\mathscr{B}$ *of the set of all subsets of* $E$ *satisfying the following conditions* (cf. GT, X, § 1.2, Remark 2).
(B1) *Every subset of a set of* $\mathscr{B}$ *belongs to* $\mathscr{B}$.
(B2) *Every finite union of a set of* $\mathscr{B}$ *belongs to* $\mathscr{B}$.

*我们说* $\mathscr{B}$ *正在覆盖，如果* $E$ *的每个元素都包含在集合中，其中属于到* $\mathscr{B}$，*或者，这是相同的，如果* $\mathscr{B}$ *是* $E$的覆盖。

#### 例 {#evt-iii-s1-n1-exa-1 .statement tag=07KX}

— 令 E 为度量空间； E (GT, IX, § 2, No. 2) 的所有有界子集的集合是 E 上的覆盖出生学。设 G 为 E 等距的群； G 的所有子集 M 的集合，使得对于每个 $x \in E$，集合 $M.x$ 是 E 的有界子集，是 G 上的覆盖出生学。

如果$\mathscr{B}$是集合E上的出生学，如果$\mathscr{B}$的每个集合都包含在$\mathscr{B}_1$的集合中，则$\mathscr{B}$的子集$\mathscr{B}_1$被称为$\mathscr{B}$的*基*。

E 上出生学家族的交是出生学；因而，对于$\mathfrak{P}(E)$的每一个子集$\mathfrak{S}$，都存在最小的出生学包含$\mathfrak{S}$；这个出生学据说是由*$\mathfrak{S}$*生成的，并承认为$\mathfrak{S}$的集合的有限并的基集合。如果 E 和 E' 是两个集合，且 $\mathscr{B}$（或 $\mathscr{B}'$）是 E（或 E'）上的出生学，乘积出生学是 $E \times E'$ 上的出生学，承认集合 $M \times M'$ 为基，其中 $M \in \mathscr{B}$ 和$M' \in \mathscr{B}'$。

#### 定义 2 {#evt-iii-s1-def-2 .statement tag=07KY}

*设$E$为向量空间。 $E$ 上的出生学 $\mathscr{B}$ 被认为是凸的，如果对于每个 $X \in \mathscr{B}$ 和 $t \in K$，有拟似集合 $tX$ 和 $X$ 的凸平衡包络线 $\Gamma(X)$ (II, p. 10) 属于至 $\mathscr{B}$。*

如果$X$和$Y$是$E$中的两个子集，我们有
$$
X + Y \subset 2\Gamma(X \cup Y)
$$
$$
\lambda X \subset t\Gamma(X) \quad \text{for} \quad |\lambda| \leq t .
$$

因而，如果$\mathscr{B}$是$E$上的凸出生学，如果$A$是$K$的有界子集，并且如果$X, Y$属于到$\mathscr{B}$，则$X + Y \in \mathscr{B}$和$A.X \in \mathscr{B}$。

### 2. 拓扑向量空间的有界子集

#### 定义 3 {#evt-iii-s1-def-3 .statement tag=07KZ}

*设$E$为拓扑向量空间。如果 $E$ 的子集 $A$ 被 $E$ 中 $0$ 的每个邻域吸收（I，p. 7，def. 4）。*

在$A$有界的阶中，$A$被$0$的邻域的基本系统的每个邻域吸收就足够了。由于存在$0$的平衡邻域的基本系统（I，p. 7，命题4），这与说相同，对于$E$中$0$的每个邻域$V$，存在$\lambda \in K$使得$A \subset \lambda V$。

假设 $E$ 的拓扑由半范数 (II, p. 3) 的基本系统 $\Gamma$ 定义；则 $E$ 的子集 $A$ 是有界的当且仅当每个半范数 $p \in \Gamma$ 都在 $A$ 上有界。

特别是，如果$E$是半范数空间，则$E$的子集$A$是有界的当且仅当它包含在球中时。在其他字中，如果 $E$ 已标准化，这意味着 $A$ 的界限为 $E$ 的度量空间结构（GT，IX, § 2, No. 2）。

#### 注 {#evt-iii-s1-n2-rem-1 .statement tag=07L0}

— 1) 如果$E$是半范数空间，则球形式是$E$中$0$的有界邻域的基本系统。相反，如果$E$是局部凸拓扑向量空间，并且如果$E$中存在$0$有界邻域，则该邻域包含是凸平衡邻域$W$，并且规范为那么$W$是定义拓扑的$E$的半范数。

因此，如果 $E$ 是局部凸且可度量的，并且如果其拓扑不能由单个范数定义，则 $E$ 上不存在定义其拓扑的距离，并且使得 $d$ 的有界子集 (GT, IX, § 2, No. 2）是$E$的有界子集。更准确地说，对于 $E$ 上的每个距离 $d$（这是平移不变性的，并且 $E$ 的定义拓扑），$E$ 的有界子集的有界为 $d$ (III， p. 38，执行 3)，但逆命题为假。

2) 令$M$为$E$的向量子空间，并赋予拓扑。在阶中，$M$的子集以$M$为界，它以$E$为界是充分必要的。

3) 令$N$为$E$中$0$的所有邻域中的交，因此$\tilde{E} = E/N$是与$E$相关的豪斯多夫向量空间。那么$N$是有界的；如果 $\pi : E \to \tilde{E}$ 是典范同态，则 $E$ 的子集 $B$ 是有界的当且仅当 $\pi(B)$ 有界。

4) 令$E$为Hausdorff局部凸空间；那么对于$E$中的每个$x \neq 0$，都存在一个连续的半范数$p$使得$p(x) \neq 0$；该半范数不受 $x$ 生成的实半线 $\mathbf{R}_+ . x$ 的限制。因此，$E$ 的非空子空间没有界限。特别是，有界子集不包含包含任何线。

#### 定义 4 {#evt-iii-s1-def-4 .statement tag=07L1}

*设$E$为局部凸空间。 $E$上的出生学$\mathscr{B}$据说适用于$E$，如果它是凸的，则由$E$的有界子集组成，并且如果$\mathscr{B}$属于到$\mathscr{B}$的每个集合闭包。*

#### 命题 1 {#evt-iii-s1-prop-1 .statement tag=07L2}

*设$E$为局部凸空间。 $E$ 的有界子集的集合是适应的出生学。*

我们需要建立以下属性：
a) 如果$B$是$E$的有界子集，则$B$的每个子集都是有界的。
b) 两个有界子集的并是有界的。
c) 每个与有界集合位似的集合都是有界的。
d) 有界子集的闭凸平衡包络线 (II, p. 13) 是有界的。
如果 $p$ 是 $E$ 上的连续半范数，则 $p$ 的球是凸球、平衡球、闭球，并且集合拟似球是球。因此，如果 $p$ 有界于 $E$ 的两个子集 $X$ 和 $Y$，则它也有界于 $X \cup Y$ 的闭凸平衡包络线，以及与它们拟似的集合上。这就建立了性质 $b), c)$ 和 d)，并且 a) 是显而易见的。

#### 定义 5 {#evt-iii-s1-def-5 .statement tag=07L3}

*设$E$为局部凸空间。 $E$的所有有界子集的集合被称为$E$的规范出生学。*

如果$\mathscr{B}$是$E$有界子集的集合，则存在适应$E$和包含$\mathscr{B}$的最小的出生学$\tilde{\mathscr{B}}$。 $\tilde{\mathscr{B}}$ 的集合是那些包含在与 $\mathscr{B}$ 集合的有限并的闭凸平衡包络相似的集合中的值。

每一种改编的出生学都包含在规范的出生学中。

#### 命题 2 {#evt-iii-s1-prop-2 .statement tag=07L4}

*在局部凸空间 $E$ 中，每个预紧式集合都是有界的。*
令$A$为$E$的预紧子集，$V$为$0$的凸平衡邻域。存在 $A$ 的点中的有限序列 $(a_i)_{1 \leq i \leq n}$ 使得
$$
A \subset \bigcup_{1 \leq i \leq n} (a_i + V).
$$
由于 $B = \{a_1, ..., a_n\}$ 有界，因此存在标量 $\lambda$ 使得 $0 < \lambda < 1$ 和 $\lambda B \subset V$；我们有 $\lambda A \subset \lambda B + \lambda V \subset V + V$，然后是命题。

#### 推论{#evt-iii-s1-n2-cor-1 .statement tag=07L5}

*在局部凸空间中，柯西序列的点的集合是有界的。*
事实上，这个集合是预紧的（GT，II, § 4, No. 2）。

#### 注 5 {#evt-iii-s1-n2-rem-5 .statement tag=07L6}

— 一般来说，局部凸空间 $E$ 的有界子集并不都是预紧的（对于例，如果 $E$ 是一个无限维范数空间，则其单位球不是紧的（I、p. 15、th. 3））。然而，如果$E$是弱空间（II，p. 42）：对于与E相关的豪斯多夫拓扑向量空间，则同构于乘积K^l的子空间，其有界子集是预紧的（*cf.* III，p. 4，cor.2）。
对于其他例，请参阅IV、p. 18。

#### 命题 3 {#evt-iii-s1-prop-3 .statement tag=07L7}

— *设 A 为局部凸空间 E 的子集。假设 A 有界；那么对于 A 的点的每一个序列 (x_n) 以及每一个序列 (\lambda_n) 趋向于 0 的标量，序列 (\lambda_n x_n) 趋于 0。反之，如果存在序列 (\lambda_n) 个非零标量，使得对于每一个序列 A 的点 (x_n)，序列 (\lambda_n x_n) 有界，则 A 有界。*

假设 A 有界。如果 (\lambda_n) 是趋于 0 的标量中的序列，并且 V 是 0 的邻域，则只要 n 足够大，我们就有 \lambda_n A \子集 V，并且紧随其后的是第一个断言。

相反，如果 A 无界且 (\lambda_n) 是标量 \neq 0 的序列，则存在 A 的点的连续半范数 p 和序列 (x_n)，使得 $p(x_n) \geq \frac{n}{|\lambda_n|}$。那么我们就知道 $p(\lambda_n x_n) \geq n$ 和序列 (\lambda_n x_n) 是无界的。

#### 推论{#evt-iii-s1-n2-cor-2 .statement tag=07L8}

— *E 的子集 A 是有界的当且仅当 A 的每个可数子集都是有界的。*

### 3. 连续映射下的像

#### 命题 4 {#evt-iii-s1-prop-4 .statement tag=07L9}

— *令 E 和 F 为两个局部凸空间且 f : E \to F 为连续映射。假设 f(0) = 0 并且存在实数 m \geq 0 使得对于每个 lambda > 0 都有 f(\lambda x) = \lambda^m f(x)。然后，如果 A 是 E 的有界子集，则 f(A) 在 F 中有界。*

事实上，如果F中V是0的邻域，那么$f^{-1}(V)$是E中0的邻域。如果A在E中有界，则存在\lambda > 0使得A\子集\lambda f^{-1}(V)，这意味着$f(A) \subset \lambda^m V$。

#### 推论 1 {#evt-iii-s1-prop-4-cor-1 .statement tag=07LA}

— *令 E 和 F 为两个局部凸空间，且 u : E \to F 为连续线性映射。如果 A 是 E 的有界子集，则 u(A) 在 F 中有界。*

#### 推论 2 {#evt-iii-s1-prop-4-cor-2 .statement tag=07LB}

— *令 E = \prod_{i \in I} E_i 为局部凸空间族的乘积。那么 E 的子集是有界的当且仅当其所有投影都是有界的。*

更一般地说：

#### 推论 3 {#evt-iii-s1-prop-4-cor-3 .statement tag=07LC}

— *令 E 为向量空间，(F_i)_{i \in I} 是从 E 到 F_i 的局部凸空间和 f_i 线性映射族（对于 i \in I）。假设 E 被分配最粗糙的拓扑（局部凸），其中所有 f_i 都是连续的（II，p. 26）。那么，对于 E 的子集 A 有界，对于所有 i \in I，f_i(A) 在 F_i 中有界是必要且充分的。*

事实上，如果 A 有界，则 f_i(A) （cor. 1）也是有界的。相反，如果 f_i(A) 有界且 p 是 E 上的连续半范数，则存在 I 的有限子集 J 和族 $(q_j)_{j \in J}$，其中 $q_j$ 是 $F_j$ 上的连续半范数，使得 $p \leq \sup_{j \in J} (q_j \circ f_j)$ 因而 $p$ 有界$A$。

#### 推论 4 {#evt-iii-s1-prop-4-cor-4 .statement tag=07LD}

*令$E_i$ ($1 \leq i \leq n$) 和$F$ 为局部凸空间，且$f$ 为从$\prod_{i=1}^n E_i$ 到$F$ 的连续多重线性映射。如果$B_i$是$E_i$的有界子集，对于$1 \leq i \leq n$，则$f(\prod_{i=1}^n B_i)$有界于$F$。*

#### 推论 5 {#evt-iii-s1-prop-4-cor-5 .statement tag=07LE}

*设$E$和$F$为两个局部凸空间，$u : E \to F$为连续多项式映射。如果 $A$ 是 $E$ 的有界子集，则 $u(A)$ 是有界的。*

### 4. 在某些归纳极限内有界子集

#### 命题 5 {#evt-iii-s1-prop-5 .statement tag=07LF}

*令$(E_i)_{i \in I}$为Hausdorff局部凸空间族，并令$E$为该族的拓扑直和（II，p. 29）。在$E$的子集$B$有界的阶中，存在$I$的有限子集$J$使得$\operatorname{pr}_i(B)$对于$i \in J$在$E_i$有界是充分必要的并且$\operatorname{pr}_i(B) \subset \{0\}$ 对于所有$i \notin J$。

设$J$为$I$中的有限子集。由于$\prod_{j \in J} E_j$上的$E$诱导乘积拓扑的拓扑（II，p. 30，第7条和p. 31，第8条），它由III推出， p. 4，科尔。 2 条件就足够了。

相反，令 $B$ 为 $E$ 的有界子集。那么 $\operatorname{pr}_i(B)$ 对于所有 $i$ 有界（III，p. 4，cor.1）。因而，只要证明$I$存在有限子集$J$，使得所有$i \notin J$都有$\operatorname{pr}_i(B) \subset \{0\}$。如果不是，则存在$I$的不同元素的无限序列$(i_n)$和$B$的元素的无限序列$(x_n)$，使得$\operatorname{pr}_{i_n}(x_n) \neq 0$。由于$E_{i_n}$是Hausdorff，因而$E_{i_n}$上存在连续半范数$p_n$使得$p_n(\operatorname{pr}_{i_n}(x_n)) \geq n$。因而，$p = \sum_{n \geq 1} p_n \circ \operatorname{pr}_{i_n}$是$E$上的连续半范数，而$p$在$B$上无界，这是一个矛盾。*

#### 命题 6 {#evt-iii-s1-prop-6 .statement tag=07LG}

*令$E$为局部凸空间，它是$E$的闭向量子空间（II，p. 33）的递增序列$(E_n)$的严格归纳极限。 $E$的子集$B$是有界的当且仅当它包含在子空间$E_n$之一中，并且在这个子空间中是有界的。

条件是足够的，因为 $E$ 在$E_n$ 上诱导的拓扑正是$E_n$ 的给定拓扑（II，p. 32，道具 9）。要看出条件是必要的，只要证明如果$E$的点的序列$(x_m)$不包含在子空间$E_n$中，那么它就足够了（III，p. 4，命题3） 不能趋于0。通过提取序列$(x_m)$的子序列，我们可以假设整数存在严格递增的序列$(n_k)$，这样，对于每个指标$k$，我们有$x_k \notin E_{n_k}$ 和 $x_k \in E_{n_{k+1}}$。那么凸集合存在(II,p. 33,引理2)递增序列$(V_k)$使得$V_k$是$E_{n_k}$,$V_{k+1} \cap E_{n_k} = V_k$中0的邻域这样，每指标 $k$ 就有 $x_k \notin V_{k+1}$。 $V_k$的并$V$则邻域等于$E$中的0，并且对于所有$k$我们有$x_k \notin V$。这证明序列$(x_k)$不趋于0.*

道具的结论。 6 对于空间 E 来说不一定成立，它是 E 的闭子空间的不可数有向集合的归纳极限（cf. III，p. 38，执行 7）。

#### 命题 7 {#evt-iii-s1-prop-7 .statement tag=07LH}

— 令 $(E_n)_{n \geq 0}$ 为 Hausdorff 局部凸空间的序列，并且对于每个 $n$，令 $u_n : E_n \to E_{n+1}$ 为紧的单射线性映射（即，$E_n$ 中存在 0 的邻域，其$u_n$下的像相对紧凑；这意味着$u_n$是连续的）。令$E$为系统$(E_n, u_n)$（II，p. 29）的归纳极限，并令$v_n$为从$E_n$到$E$的典范映射。那么局部凸空间 $E$ 就是 Hausdorff。此外，对于$E$的每个子集$A$，以下条件是等价的：
(i) $A$ 有界；
(ii) 存在整数$n$，使得$A$是$E_n$的有界子集的$v_n$下的像；
(iii) $A$ 相对紧凑。
我们认同$E_n$与向量子空间为$E$（赋予拓扑更细比诱导的拓扑）。

#### 引理 1 {#evt-iii-s1-lem-1 .statement tag=07LI}

在支柱的假设下。 7、$E$中的拓扑是最精细的拓扑，其中所有映射$v_n : E_n \to E$都是连续的。

我们需要证明，如果$U$是$E$的子集，使得对于每个$n$，$U \cap E_n$在$E_n$中开，那么$U$在$E$中开；在其他字，我们必须证明，对于每个$x \in U$，存在一个*凸平衡*集合$V$，使得$x + V \subset U$和$V \cap E_n$对于每个足够大的$n$来说$E_n$中的邻域为0 （II，p. 27，第 5 条）。 对于每个$n$，令$W_n$是$E_n$中0的凸平衡邻域，使得$E_{n+1}$中$W_n$的闭包$H_n$是紧凑的。 令 $x \in U$ 且令 $n_0$ 为整数，使得 $x \in E_{n_0}$。 We shall construct, by induction, a sequence $(\varepsilon_n)_{n \geq 0}$ of scalars $> 0$ such that $x + \sum_{n_0 \leq i \leq n} \varepsilon_i H_i$ is contained in $U$ for $n \geq n_0$. 假设$i < n$的$\varepsilon_i$已经构造完毕。 若$n = n_0$、集合$V_{n-1} = \{0\}$；如果没有，集合
$$
V_{n-1} = \sum_{n_0 \leq i \leq n-1} \varepsilon_i H_i.
$$
那么$V_{n-1}$在$E_n$中是紧致的，并且*更不必说*在$E_{n+1}$中是紧致的。 由于$U \cap E_{n+1}$在$E_{n+1}$中开，因此存在标量$\varepsilon_n > 0$，使得$x + V_n = x + V_{n-1} + \varepsilon_n H_n$包含在$U$中（GT，II, § 4, No. 3，cor.）。 让$V = \bigcup_{n \geq n_0} V_n$。 那么$V$是凸且平衡的；对于$n \geq n_0$，我们有$V \cap E_n \supset \varepsilon_n H_n \cap E_n \supset \varepsilon_n W_n$，因此$V \cap E_n$是$E_n$中0的邻域。 这样就完成了引理的证明。

集合$U = E - \{0\}$使得集合$U \cap E_n = E_n - \{0\}$对于每个$n$在$E_n$中开，因此$U$在$E$中开，这证明$E$是Hausdorff（GT，III, § 1, No. 3，道具2）。显然，性质 (ii) 蕴含 (iii)，而 (iii) 蕴含 (i)。最后我们证明 (i) 蕴涵 (ii)。为此，足以证明，如果 $E$ 的子集 $A$ 不被集合 $\sum_{0 \leq i \leq n} H_i$ 中的任何一个吸收，则 $A$ 是无界的。但是，存在序列 $(x_n)_{n \geq 1}$ 或点或 $A$，这样，对于每个 $n$，我们就有 $x_n \notin n^2 \sum_{0 \leq i \leq n} H_i$。

那么$x_n / n$的集合凭借引理1而闭合，因为它的交和$E_m$对于每个整数$m$都是离散的。 $x_n / n$ 的集合的补集是 0 的开邻域，它不吸收序列 $(x_n)$，因此 $A$ 是无界的。

#### 注 1 {#evt-iii-s1-n4-rem-1 .statement tag=07LJ}

有了上面的记号，让$F_n$是$H_n$生成的向量空间，范数等于$H_n$的规格。我们将看到（III，p. 8，cor.）$F_n$是Banach空间。从$F_n$到$E_{n+1}$的单射是紧凑的，因此*更不必说*也是从$F_n$到$F_{n+1}$的单射$w_n$。此外，$E$是Banach空间*的归纳法系统*$(F_n, w_n)$*的*归纳法极限。例如，$E$ 中凸平衡邻域 $V$ 为 0，使得 $V \cap E_n$ 吸收所有 $n \geq 1$ 的 $H_{n-1}$，反之，如果 $E$ 中凸平衡集合 $W$ 使得$W \cap E_n$吸收$H_{n-1}$，则$W \cap E_{n-1}$包含集合对于所有$n \geq 1$与$W_{n-1}$拟似，因此$W$是$E$中0的邻域。

#### 注 2 {#evt-iii-s1-n4-rem-2 .statement tag=07LK}

令 $F$ 为局部凸空间，$k$ 整数 $\geq 0$，$f : E^k \to F$ 为多线性映射。为了使$f$连续，$f$到$E_n^k$中的限制对于每个$n$连续是必要且充分的。我们立即验证$E^k$对于线性映射$v_n \times \cdots \times v_n : E_n \times \cdots \times E_n \to E \times \cdots \times E$族具有最终的局部凸拓扑（II，p. 28，cor.2和p. 30，道具7），并且$u_n \times \cdots \times u_n$是紧单射线性映射从$(E_n)^k$变为$(E_{n+1})^k$。现在应用引理 1 就足够了。

### 5. 空间 $E_A$（有界）

令$E$为局部凸空间，$A$为$E$的凸平衡子集。我们记得$E_A$表示由$A$生成的向量空间，$p_A$是$A$的规范，作为半范数（II，p. 26，*例3*）。我们立即验证当且仅当$A$有界时，$E_A$到$E$的典范嵌入是连续的。如果在加法中，$E$ 是 Hausdorff，则有界集合 $A$ 不是包含一条线 (III, p. 2, *注 4*)，因此 $p_A$ 是范数（II，*loc.cit.*）。

如果$X$中的每个柯西序列收敛，我们可以说一致空间$X$是“半完备”的。完整的制服空间是半完整的；但逆命题并不总是正确的（GT，II, § 4，练习4）；然而，可度量的半完备空间是完备的（GT，IX, § 2, No. 6，道具9）。

#### 命题 8 {#evt-iii-s1-prop-8 .statement tag=07LL}

*令$E$为Hausdorff局部凸空间，并令$A$为$E$的封闭、平衡、有界且凸子集。设$(x_n)$为$E_A$中的柯西序列。那么这个序列收敛于$E_A$当且仅当它收敛于$E$。*

典范嵌入从$E_A$到$E$是连续的。因此，如果$(x_n)$收敛于$E_A$，它也收敛于$E$。相反，假设$(x_n)$在$E$中收敛到$y$。存在整数$(n_k)$的递增序列，使得$p_A(x_m - x_n) \leq 2^{-k-1}$如果$m \geq n_k$和$n \geq n_k$。因此序列$(x_{n_k} + 2^{-k}A)$是递减。由于$A$在$E$中闭合，我们有$y \in \bigcap_k (x_{n_k} + 2^{-k}A)$，这证明了$(x_{n_k})$，因此$(x_n)$，在$E_A$中收敛到$y$。

#### 推论{#evt-iii-s1-n5-cor-1 .statement tag=07LM}

— *如果 A 是半完备的（特别是完备的），则 E_A 是 Banach 空间。*
    事实上，E_A 中的柯西序列也是 E 的拓扑的柯西序列，并且包含在与 A 相似的集合中，因此收敛于 E。

### 6. 完全有界集合和准完全空间

#### 定义 6 {#evt-iii-s1-def-6 .statement tag=07LN}

— *如果 E 的每个闭有界子集都是完备的，则称局部凸空间 E 是准完备的（对于由 E 导出的一致结构）。*
    完全局部凸空间是准完备的，但逆命题并不总是正确的。 *对于例，如果 E 是无限维 Hilbert 空间，或者更一般地说，是无限维自反 Banach 空间，则带有弱化拓扑的 E 是准完备但不完备（II，p. 51，道具 9）。*
    准完备空间是半完备的，因为每个柯西序列都包含在一个封闭且有界的子集中（III，p. 3，推论和命题 1）。特别是，局部凸可度量且准完备的空间是完备的。
    在 Hausdorff 准完备空间中，预紧式子集的闭包和封闭凸平衡包络线是紧致的；事实上，它们是预紧的（II，p. 25，命题3），并且是完全闭集和有界的（III，p. 3，命题2）。

#### 命题 9 {#evt-iii-s1-prop-9 .statement tag=07LO}

— (i) *准完备局部凸空间的闭向量子空间是准完备的。*
    (ii) *准完全局部凸空间的乘积是准完全的。*
    (iii) *拟完备局部凸空间的拓扑直和是准完备的。*
    (iv) *局部凸空间，闭拟完备子空间的序列的严格归纳极限是准完备的。*
    断言 (i) 源自 *注 2* (III, p. 2), (ii) 源自 III, p. 4，cor。 2，（iii）来自道具。 5 (III, p. 5) 和 (iv) 来自道具。 6（III，p. 5）。

    稍后我们将看到，准完备局部凸空间与闭向量空间的商空间不一定是准完备的（IV，p. 63，执行10）。

#### 命题 10 {#evt-iii-s1-prop-10 .statement tag=07LP}

— *令 E 为 E 的局部凸空间，M 向量子空间，使得 E 的每个点都位于 M 的有界子集的闭包内。则从 M 开始的每个连续线性映射 f 变为 Hausdorff 拟完全局部凸空间 F 唯一扩展到从 E 到 F 的连续线性映射。*
假设意味着 M 在 E 中是稠密的，因此 f 扩展唯一地从 E 到 F 的完成$\hat{F}$ 的连续线性映射 $\hat{f}$（GT，III, § 3, No. 4，推论）。但每个 $x \in F$ 都位于 M 的有界子集 B 的闭包中；因此$\hat{f}(x)$位于$\hat{F}$中$f(B)$的闭包中。但$f(B)$在F中有界，因此它在F中的闭包是完全的，重合在$\hat{F}$中是完全闭包的。这就证明了$\hat{f}(x) \in F$。

### 7. 例

a) 设X为拓扑空间。让X上的数值（有限）函数的$\mathscr{R}(X)$，向量空间被分配为紧致收敛（GT，X, § 1, No. 3）的拓扑：这是最粗糙的拓扑，其中限制映射 $\mathscr{R}(X) \to \mathscr{R}(H)$ 是连续的（其中 H 贯穿 X 的紧子集族，并且其中$\mathscr{R}(H)$被指定一致收敛的拓扑）。科。 III、p. 4 的 3 表明，子集 $\mathscr{R}(X)$ 的 A 是有界的当且仅当，对于每个紧致子集 H of X、集合 of 限制到 H of 函数属于到 A 是一致有界的。

*b) (无限可微函数的空间。)令$n \geqslant 1$为整数。对于 $\mathbf{R}^n$ 中的每个开集合 U，令 $\mathscr{C}^\infty(U)$ 表示 U 上无限可微函数的向量空间 (VAR, R, 2.3)。令 f 在 $\mathscr{C}^\infty(U)$ 中。对于$\mathbf{N}^n$中的每个多索引$\alpha = (\alpha_1, ..., \alpha_n)$，$\partial^\alpha f$表示偏导数$\partial^{|\alpha|} f / \partial x_1^{\alpha_1} ... \partial x_n^{\alpha_n}$；这是 U（VAR、R、2.3 和 2.4）上的连续函数。对于每个整数 $m \geqslant 0$，以及 U 的每个紧凑子集 H，集合

$$
p_{m,H}(f) = \sup_{\substack{|\alpha| \leqslant m \\ x \in H}} |\partial^\alpha f(x)| .
$$

那么$p_{m,H}$是$\mathscr{C}^\infty(U)$的半范数。

让$\mathscr{C}^\infty(U)$被分配由半范数$p_{m,H}$定义的拓扑。这是最粗糙的拓扑，其中从 $\mathscr{C}^\infty(U)$ 到 $\mathscr{R}(U)$ 的映射 $f \to \partial^\alpha f$ 是连续的，其中$\mathscr{R}(U)$ 被分配紧致收敛的拓扑。 U 中存在递增序列的紧凑子集 $(H_n)_{n \geqslant 0}$，其内部覆盖 U； $\mathscr{C}^\infty(U)$ 的半范数族$p_{m,H_n}$定义拓扑，然后成为局部凸可度量空间。 空间$\mathscr{C}^\infty(U)$已完成；在其他字中，它是Fréchet空间（II，p. 24）：实际上，让$(f_k)$是$\mathscr{C}^\infty(U)$中的柯西序列；对于每个$\alpha \in \mathbf{N}^n$，序列$(\partial^\alpha f_k)$收敛于完整的空间$\mathscr{R}(U)$（TG，X, § 1, No. 5，第1）到连续的函数$g_\alpha$。到$|\alpha|$的归纳，我们从 th 推导出来。 FVR 的 1，II、p. 2，每 $\alpha \in \mathbf{N}^n$ $g_\alpha = \partial^\alpha g_0$。在其他字中，序列$(f_k)$收敛于$\mathscr{C}^\infty(U)$中的$g_0$。

设 A 为 $\mathscr{C}^\infty(U)$ 的子集。在阶中，A是有界的，对于U的每个整数$m \geqslant 0$和每个紧致子集H，数$\sup_{f \in A} p_{m,H}(f)$是有限的是充分必要的；这个条件意味着对于每个$\alpha \in \mathbf{N}^n$，函数$\partial^\alpha f|H$对于$f \in A$的集合对于每个紧凑的$H \subset U$是统一有界的。

令 $H \subset U$ 是紧致的。我们用函数的 $\mathscr{C}^\infty(U)$ 由……组成的 $\mathscr{C}_H^\infty(U)$ 子空间表示，其支持位于 H 中。 无限可微函数的空间 $\mathscr{C}_c^\infty(U)$ 在 U 中具有紧支持，是有向递增并子空间$\mathscr{C}_H^\infty(U)$，其中 H 穿过 U 的紧致子集族。每个空间$\mathscr{C}_H^\infty(U)$将被分配由$\mathscr{C}^\infty(U)$诱导的拓扑，以及$\mathscr{C}_c^\infty(U)$与相应的诱导的极限拓扑。如果集合$H_n$使得它们的内部形式是U的覆盖，那么空间$\mathscr{C}_c^\infty(U)$是Fréchet空间$\mathscr{C}_{H_n}^\infty(U)$的严格归纳极限；因此它是完整的（II，p. 32，第 9 条），并且 $\mathscr{C}_c^\infty(U)$ 的每个有界子集都包含在子空间 $\mathscr{C}_{H_n}^\infty(U)$ 之一（III，p. 5，第 6 条）。 \*

c) （Gevrey 的空间。）令 I 为 $\mathbf{R}$ 中的紧区间。对于每个整数 $n \geqslant 0$，$D^n f$ 表示在 I 上定义的数值函数 $f$ 的 $n$ 导数（只要该导数存在）。令$s \geqslant 1$和$M \geqslant 0$为两个实数。令 $\mathscr{G}_{s,M}(I)$ 表示 I (FVR, I, p. 28) 上的无限可微函数 $f$ 中的向量空间，其中序列 $(|D^n f|/M^n(n!)^s)_{n \geqslant 0}$ 的边界为所有连续的空间 $\mathscr{C}(I)$ 函数 on I（拓扑一致收敛）。 空间 $\mathscr{G}_{s,M}(I)$ 是 Banach 空间与范数

$$
\|f\|_{s,M} = \sup_{n \geqslant 0, x \in I} |D^n f(x)|/M^n(n!)^s .
$$

对于$M \leqslant M'$，我们有$\mathscr{G}_{s,M}(I) \subset \mathscr{G}_{s,M'}(I)$，并且

$$
\|f\|_{s,M'} \leqslant \|f\|_{s,M}
$$

每$f \in \mathscr{G}_{s,M}(I)$。让$\mathscr{G}_s(I)$表示空间$\mathscr{G}_{s,M}(I)$的并，并赋予它$\mathscr{G}_{s,M}(I)$拓扑的归纳极限拓扑。

设 $M < M'$ 并设 B 为 $\mathscr{G}_{s,M}(I)$ 中的单位球（闭合）。我们将证明 B 是 Banach 空间 $\mathscr{G}_{s,M'}(I)$ 的紧子集。显然，B 在$\mathscr{G}_{s,M'}(I)$ 是闭集，因此只需证明 B 在$\mathscr{G}_{s,M'}(I)$ 是预紧的。令 $\varepsilon > 0$ 并令 N 为正整数，使得 $(M/M')^N \leqslant \varepsilon/2$。设$k$为正整数；所有函数 $D^{k+1} f$ 中的集合（因为 $f$ 范围在 B 上）的边界在 $\mathscr{C}(I)$ 内，因此所有函数 $D^k f$ 中的集合（因为 $f$ 范围在 B 上）在 $\mathscr{C}(I)$ 中相对紧凑：这是从有限增量的定理（FVR，I，p. 23，cor.1）和Ascoli的定理（GT，X, § 2, No. 5）得出的。我们定义范数于$\mathscr{G}_{s,M}(I)$

$$
q(f) = \sup_{0 \leqslant n \leqslant N, x \in I} |D^n f(x)|/M^n(n!)^s .
$$

上述论证表明，B 对于与范数 $q$ 关联的拓扑是预紧的；在其他字中，存在B的有限子集C，使得对于每个$f \in B$，存在$g \in C$使得$q(f - g) \leqslant \varepsilon$。最后，对于每 $n > N$，我们有

$$
|D^n f(x) - D^n g(x)|/M^n(n!)^s \leqslant 2(M/M')^n \leqslant \varepsilon ,
$$

从中我们得到$\|f - g\| \leqslant \varepsilon$。这证明了 B 在 $\mathscr{G}_{s,M'}(I)$ 中是预紧的。

空间$\mathscr{G}_s(I)$是空间$\mathscr{G}_{s,k}(I)$的归纳极限，因为$k$范围超过$\mathbf{N}$；通过道具。 7 (III, p. 6) $\mathscr{G}_s(I)$的每个有界子集都包含在空间$\mathscr{G}_{s,k}(I)$之一中，并且在这个空间中相对紧凑。

\* d) （全纯函数的空间。）令$n \geqslant 1$为整数。对于$\mathbf{C}^n$的每个开子集 U，$\mathscr{H}(U)$表示U中函数全纯的空间，并分配U中紧致收敛的拓扑。对于$\mathbf{C}^n$的每个紧致子集L， $\mathscr{H}(L)$表示L的邻域中全纯函数的胚空间；我们赋予这个空间以最精细的局部凸拓扑，其中典范映射$\pi_U : \mathscr{H}(U) \to \mathscr{H}(L)$是连续的，其中U的范围超过L的开邻域的集合。

对于每个整数$m \geq 1$，令$U_m$为$\mathbf{C}^n$的点中的集合，其与L的距离为$< 1/m$。可以证明，从$\mathscr{H}(U_m)$到$\mathscr{H}(L)$的典范映射$\pi_{U_m}$是*单射的*，而从$\mathscr{H}(U_m)$到$\mathscr{H}(U_p)$的限制映射对于$p \geq m$来说是*紧致*。然后我们就可以应用 prop. 7（III，p. 6）。设 A 为 $\mathscr{H}(L)$ 有界子集；则存在整数$m \geq 1$，使得A由L的邻域中的函数的胚芽、属于到$\mathscr{H}(U_m)$中的有界集合B组成。此外，从$\mathscr{H}(L)$到拓扑空间T的映射$\phi$是连续的，当且仅当从$\mathscr{H}(U)$到T的映射$\phi \circ \pi_U$对于L的每个开邻域U是连续的。 \*

### 习题 {#evt-iii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
