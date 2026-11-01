---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 3
section_title: Simple Modules
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.45-A VIII.54
pdf_pages: 0062-0071
extraction: native
subsections:
    - "no": 1
      title: Simple Modules
      page: 45
      pdf_page: 62
    - "no": 2
      title: Schur’s Lemma
      page: 47
      pdf_page: 64
    - "no": 3
      title: Maximal Submodules
      page: 48
      pdf_page: 65
    - "no": 4
      title: Simple Modules over an Artinian Ring
      page: 50
      pdf_page: 67
    - "no": 5
      title: Classes of Simple Modules
      page: 51
      pdf_page: 68
statements: 23
exercises: 10
content_sha256: 297ae059133b3e0ce8554ab8da3d5cc64c03dad16f724687518f0a608981e831
translated_from: content/en/alg/VIII/03_s3_simple_modules.md
translation_method: google
source_content_sha256: 0317407d0c3ced7b2648e2b8d2e1ca2a46c305400b4715365d0e28e9e8310de8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 16b650362485e8878470031f92d26d9eb257701074426a48db92e243594141bd
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。 单模

### 1.单模

回忆一下下面的定义（II, §1, No. 10，p. 212）。

#### 定义 1 {#alg-viii-s3-def-1 .statement tag=0035}

设 A 为环。如果A-模 M 是非零的并且没有不同于 0 和 M 的子模，则称 M 为简单。

A-模 M 是简单的当且仅当 M 是单模超过其同位环 $A_M$。每个单模都是不可分解的，长度 1，因此是原始的 (VIII, p. 31, 命题 4, b))。

#### 例 1 {#alg-viii-s3-n1-exa-1 .statement tag=0036}

模$A_s$是单A-模当且仅当A是域（I, §9, No. 1，p. 115，定理1）。 单A-模则向量空间等于维数 1 除以域 A。

#### 例 2 {#alg-viii-s3-n1-exa-2 .statement tag=0037}

设 A 为主理想整环 (VII, §1, No. 1, p. 1, 定义 1)，而不是域。对于A的每个不可约元$\pi$，A-模$A_s/(\pi )$是简单的，并且每个单A-模同构于这样的模（VII, §4, No. 8，p. 25，注4）。对于 $n\geqslant 2$、A-模 $A_s/(\pi^n)$ 是不可分解的（VII, §4, No. 8、p. 24、命题 8），但并不简单。

#### 例 3 {#alg-viii-s3-n1-exa-3 .statement tag=0038}

令 K 为域、V 非零的右向量空间超过域 K，且 A 子环为环 End$_K(V)$ 包含自同态为 V 有限秩（对于例，A = 结束$_K(V)$）。让我们证明V是单A-模：令W是V的非零的A-子模和W的$x$非零元素；在V上存在线性形式$\varphi$使得$\varphi (x)\not= 0$（II, §7, No. 5，p. 300，定理6）。对于V、映射$z\mapsto y\varphi (z)$中的每个$y$，其与秩$\leqslant 1$、属于与A呈线性关系；因此我们有$Ax= V$，因此更不必说 W = V，这证明V是单A-模。

#### 命题 1 {#alg-viii-s3-prop-1 .statement tag=00QZ}

设 A 为环。

a) 令 $\mathfrak{m}$ 为 A 的左理想。当且仅当 $\mathfrak{m}$ 为最大左理想时，A-模 $A_s/\mathfrak{m}$ 是简单的。

b) 设M为单A-模，$x$为M的非零元素。我们有等式$M = Ax$，$x$的湮没子$\mathfrak{m}$是A的最大左理想，映射 $a\mapsto ax$ 定义，由经过得到商，同构由 $A_s/\mathfrak{m}$ 得到 M。

c) 设 M 为非零的 A-模。如果 M 的每个非零元素 $x$ 都有 $M = Ax$，那么 M 是简单的。

$A_s/\mathfrak{m}$的子模是形式$\mathfrak{n}/\mathfrak{m}$，其中$\mathfrak{n}$是包含$\mathfrak{m}$的左理想（I, §4, No. 6，p. 41，定理4）；因而，A-模$A_s/\mathfrak{m}$是简单的当且仅当我们有$\mathfrak{m}\not= A$并且包含$\mathfrak{m}$的每个左理想$\mathfrak{n}$满足$\mathfrak{n}/\mathfrak{m}= 0$或$\mathfrak{n}/\mathfrak{m}= A_s/\mathfrak{m}$，即$\mathfrak{n}=\mathfrak{m}$或$\mathfrak{n}= A$。这就证明了a）。

在b)的假设下，$Ax$是M的非零的子模，因此等于M。因而，映射$a\mapsto ax$定义，通过经过除商，同构 $A_s/\mathfrak{m}$ 至 M；因而 A-模 $A_s/\mathfrak{m}$ 是简单的，并且左理想 $\mathfrak{m}$ 最大为 a)。这证明了b)。

在c)的假设下，令N为M的非零的子模。如果$x$是N的非零元素，则我们有$Ax\subset N$和$Ax= M$，因此M = N。因此M是简单的。

#### 推论 1 {#alg-viii-s3-prop-1-cor-1 .statement tag=0039}

若环 A不减至0，则存在单A-模。

事实上，根据克鲁尔的定理（I, §8, No. 6，p. 104，定理1），存在A的最大左理想。

#### 推论 2 {#alg-viii-s3-prop-1-cor-2 .statement tag=003A}

设 A 为局部环 (VIII, p. 26, 定义 1) 和 $\mathfrak{r}$ 其最大理想。 A-模 $A_s/\mathfrak{r}$ 很简单，每个单A-模都与 $A_s/\mathfrak{r}$ 同构。

#### 注 1 {#alg-viii-s3-n1-rem-1 .statement tag=003B}

设A为交换环且$\mathfrak{m}$是A的理想。则$\mathfrak{m}$为A-模$A_s/\mathfrak{m}$的湮没子（II, §1, No. 12，p. 219，定义11）。因而，如果 $\mathfrak{m}$ 和 $\mathfrak{m}'$ 是 A 的不同理想，则 A-模 $A_s/\mathfrak{m}$ 和 $A_s/\mathfrak{m}'$ 不是同构的。当且仅当 (0) 是 A 的最大理想，即 A 是域时，存在忠实的单A-模 (II, §1, No. 12, p. 219)。

#### 注 2 {#alg-viii-s3-n1-rem-2 .statement tag=003C}

我们可以给出非交换环 A 的例和 A 的两个不同的最大左理想 $\mathfrak{m}$ 和 $\mathfrak{m}'$，使得 A-模 $A_s/\mathfrak{m}$ 和 $A_s/\mathfrak{m}'$ 同构（VIII、p. 52、习题） 3）。

### 2.舒尔的引理

#### 命题 2 {#alg-viii-s3-prop-2 .statement tag=003D}

设A为环，M和N为两个A-模，并且从M到N为$f$非零的同态。

a) 如果 M 是简单的，则 $f$ 是单射的。

b) 如果 N 是简单的，则 $f$ 是满射。

c) 如果 M 和 N 很简单，则 $f$ 是同构。

$f$的核是M的真子模，$f$的像是N的非零的子模。

a) 如果 M 是简单的，那么我们有 Ker($f$) $= 0$，所以 $f$ 是单射的。

b) 如果 N 是简单的，那么我们有 Im($f$) $= N$，所以 $f$ 是满射的。

c) 如果 M 和 N 很简单，则 $f$ 既是单射又是满射。

#### 推论（Schur 引理）{#alg-viii-s3-n2-cor-1 .statement tag=00RZ}

单模中的自同态环是域。

如果M是单A-模，那么非零环End$_A(M)$的每个非零元素都是可逆的(命题2, c))，所以End$_A(M)$是域。

#### 定理 1 {#alg-viii-s3-thm-1 .statement tag=003E}

令 K 为代数闭交换域、A K-代数和 M 单A-模。假设 M 的维数作为 K 上的向量空间是有限的，或者更一般地，严格小于 K 的基数。则 A-模 M 的自同态环由同位$\alpha_M$ 与 $\alpha \in K$ 组成。

令 E 为 A-模 M 的自同态环；根据命题 2 和代数的推论，域超过域 K。如果我们将 M 视为左向量空间超过域 E，则我们有暗淡$_KM =$ (暗淡$_EM$)$[E : K]$ 命题 25 / II, §1, No. 13，p. 222，因此暗淡$_KM\geqslant [E : K]$。由于$_KM<$卡(K)被假设调暗，等式$E = K\cdot 1_M$则为以下引理的推论。

#### 引理 1 {#alg-viii-s3-lem-1 .statement tag=003F}

设E为域，E的中心的K子域不等于E。如果域K是代数闭的，则我们有$[E : K]\geqslant$Card(K)。

令 $x$ 为 E - K 的元素，L 为由 $K\cup  \{x\}$ 生成的 E 的（可交换）子域。由于 K 是代数闭集，$x$ 超越 K。通过 VII, §2, No. 3、p. 10、定理 2 和 p. 11、L 的元素 $(x-\alpha )^{-1}$（其中 $\alpha$ 穿过 K）线性无关因此我们有$[E : K]\geqslant [L : K]\geqslant$卡(K)。

#### 例 {#alg-viii-s3-n2-exa-1 .statement tag=003G}

$*$ 令 A 为由元素可数族生成的 $\mathbf{C}$ 代数；它有可数维数超过 $\mathbf{C}$。设M为单A-模；它是单生的，因此承认基超过 $\mathbf{C}$。由于域$\mathbf{C}$不可数（Gen.Top.，IV, §4, No. 1，p. 44），我们有$[M :\mathbf{C}]<$卡（$\mathbf{C}$）。因此A-模 M 的自同态是$\alpha_M$ 与$\alpha \in \mathbf{C}$ 的同位。这尤其适用于当 A 是有限维李代数在 $\mathbf{C}($Lie、I, §2, No. 7、p. 21、推论 $3).*$ 的通用包络代数时

#### 推论 1 {#alg-viii-s3-lem-1-cor-1 .statement tag=003H}

保持定理 1 中的假设，并且假设代数 A 是可交换的。那么 M 比 K 有维数 1。

由于环 A 是可交换的，因此对于每个 $a\in A$，$a_M$ 是 A-模 M 的自同态。因此，通过定理 1，我们有 $A_M= K\cdot 1_M$，M 是一个简单的 K-模，即域 K 上的一维向量空间。

#### 推论 2 {#alg-viii-s3-lem-1-cor-2 .statement tag=003I}

设 K 为交换域，A K-代数，M A-模。假设对于 K 的每个扩张 L，$A_{(L)}$-模 $M_{(L)}$ 都是简单的。那么M的自同态环由$\alpha_M$与$\alpha \in K$同位。

令I为基数的集合严格大于M的维数超过K（对于例，M的子集的集合）。设L为域$K((X_i)_{i\in I})$之代数闭包（V, §4, No. 3，p. 23，定理2）。 选择 L 上的 K 线性形式$\varphi$，使得 $\varphi (1) = 1$，并令 $v: M_{(L)}\rightarrow M$ 为由 $v(\alpha \otimes m) =\varphi (\alpha )m$ 表征的 K-线性映射。令$u$为M的自同态。$M_{(L)}$对L的维数等于M对K的维数，并且严格小于L的基数。通过定理 1，$A_{(L)}$模块$M_{(L)}$的自同态$1_L\otimes u$为形式$\lambda \otimes 1_M$和$\lambda \in L$。对于每$x\in M$，我们有

$$
u(x) =v(1\otimes u(x))=v((1_L\otimes u)(1\otimes x))
$$

$$
=v((\lambda \otimes 1_M)(1\otimes x))=v(\lambda \otimes x) =\varphi (\lambda )x
$$

这样$u$就是位似$\varphi (\lambda )_M$。

### 3.极大子模

#### 定义 2 {#alg-viii-s3-def-2 .statement tag=003J}

设A为环，M为A-模。 M的极大子模为包含M的真子模的集合的极大元素。

$A_s$的极大子模只是A的左最大理想。

设 N 为 M 的子模。$M/N$ 的子模为形式 $P/N$，其中 P 为 M 包含于 N 的子模（I, §4, No. 6、p. 41、定理） 4).因而，N 是 M 的极大子模当且仅当模 $M/N$ 是简单的。

#### 命题 3 {#alg-viii-s3-prop-3 .statement tag=003K}

令 M 为有限生成A-模。 M 的每个真子模都包含在极大子模中。

设N为M的真子模。用M包含N的真子模$\mathscr{S}$集合表示，按包含排序；让我们证明 $\mathscr{S}$ 是归纳性的。令$\mathscr{F}$等于$\mathscr{S}$的总有序子集。如果$\mathscr{F}$为空，则对于$\mathscr{S}$中的$\mathscr{F}$，N为上界。相反的情况，用$\mathscr{F}$的元素的Q并来表示。那么 Q 是 M 的子模。设 F 是 M 的有限生成子集。如果 Q 等于 M，则 F 将包含在子模 $P\in \mathscr{F}$ 中，这意味着 P = M，与 $\mathscr{F}$ 的定义相反。因此我们有$Q\in \mathscr{S}$，这证明$\mathscr{S}$是归纳性的。然后从集合理论的推论1、III, §2, No. 4、p. 155得出命题3。

#### 推论 1 {#alg-viii-s3-prop-3-cor-1 .statement tag=003L}

设 M 为非零的有限生成A-模。存在 A 的双面理想$\mathfrak{a}$，单A-模的湮没子，使得 $\mathfrak{a}M$ 不等于 M。

令N为M(命题3)的极大子模，并令$\mathfrak{a}$为单A-模$M/N$的湮没子；它是 A 的双面理想，我们有 $\mathfrak{a}(M/N) = 0$、从而 $\mathfrak{a}M\subset N$，因此有 $\mathfrak{a}M\not= M$。

#### 推论 2 {#alg-viii-s3-prop-3-cor-2 .statement tag=003M}

设A为交换环，B为A-代数。设M为单B-模即有限生成A-模，并令$\mathfrak{m}$为A-模M的湮没子。则$\mathfrak{m}$是A的极大理想，且M为域$A/\mathfrak{m}$之上的有限维向量空间。

由于环 A 是可交换的，单A-模的湮没子是 A 的最大理想 (VIII, p. 46, 命题 1)。将推论 1 应用于 A-模 M，存在 A 的最大理想 $\mathfrak{a}$，使得 $\mathfrak{a}M\not= M$。但$\mathfrak{a}M$是单B-模M的子模；因此我们有 $\mathfrak{a}M = 0$ 以及$\mathfrak{a}\subset \mathfrak{m}$。由于理想的$\mathfrak{m}$与A不同，它等于$\mathfrak{a}$，因而$\mathfrak{m}$最大。 模 M 是有限生成模超过域 $A/\mathfrak{m}$；接下来是最后一个断言。

### 4.单模超过阿廷环

设 A 为环。通过滥用语言，我们说左理想$\mathfrak{a}$是A的最小左理想，如果它是A的非零的左理想中集合的最小元素，并按包含排序。我们定义类比右极小理想和两侧极小理想。

设 $\mathfrak{a}$ 为 A 的左理想。则 $\mathfrak{a}$ 为单A-模当且仅当它是 A 的最小左理想。

左阿廷的 (VIII, p. 1, 定义 1) 环包含的每个非零的左理想都有一个最小左理想。

#### 命题 4 {#alg-viii-s3-prop-4 .statement tag=003N}

设 A 为环，其具有最小左理想$\mathfrak{a}$。每个忠实的单A-模都与A-模$\mathfrak{a}$同构的。

让M成为忠实的单A-模。设$\alpha$为$\mathfrak{a}$的非零元素。由于 A-模 M 是忠实的，因此存在 M 的元素 $x$，使得 $\alpha x\not= 0$。从$\mathfrak{a}$到M的同态$a\mapsto ax$则为非零的；因而，它是 VIII、p. 47 中的同构乘以命题 2。

#### 命题 5 {#alg-viii-s3-prop-5 .statement tag=003O}

令 A 为左阿廷的环，M 为忠实的 A-模。

a) $M^m$的$A_s$到子模存在自然数$m$和同构。

b) 如果 M 承认 Jordan–Hölder 级数 $(M_i)_{0\leqslant i\leqslant n}$，则每个单A-模同构于商 $M_i/M_{i+1}$ 之一。

将VIII、p. 2应用于M的A-模、$A_s$和元素的湮没子，存在M的元素$x_1, . . . , x_m$，使得M的湮没子是交 $x_i$ 的湮没子。由于 A-模 M 是忠实的，A-线性映射 $a\mapsto (ax_1, . . . , ax_m)$ 从 $A_s$ 到 $M^m$ 是单射的，从而 a)。

在b)的假设下，$A_s$的每个简单商都同构于Jordan–Hölder级数对$M^m$的商（I, §4, No. 7，p. 43，推论），因此与模$M_i/M_{i+1}$之一同构（I, §4, No. 7、p. 43、定理 6）。我们结论，每个单A-模同构于$A_s$的商。

#### 注 {#alg-viii-s3-n4-rem-1 .statement tag=003P}

命题 5 特别适用于以下两种情况：

a) 设 A 为交换域 K 上的代数，并令 M 为 K 上的忠实有限维模。则 M 为有限长度的 A-模，并且 M 的对模是有限生成的。 环 A 为左阿廷的（VIII、p. 9、命题 6）。存在 A-模 M 的 Jordan–Hölder 级数 $(M_i)_{0\leqslant i\leqslant n}$，并且每个单A-模都同构于 $0\leqslant i\leqslant n-1$ 的模 $M_i/M_{i+1}$ 之一。

b) 设 A 为左阿廷的环。 模$A_s$有有限长度（VIII、p. 6、定理1）。由于A-模$A_s$有有限长度，因此存在A的左理想递减序列$(\mathfrak{a}_i)_{0\leqslant i\leqslant n}$，使得$\mathfrak{a}_0= A$和$\mathfrak{a}_n= 0$以及A-模$S_i=\mathfrak{a}_{i-1}/\mathfrak{a}_i$对于$1\leqslant i\leqslant n$来说是简单的。那么每个单A-模都同构于模 $S_1, . . . ,S_n$ 之一。

### 5.单模类

表示为 Is$_A(X,Y)$ 关系

“A 是环和 $X,Y$ 同构的 A-模。”

这是相对于X和Y的等价关系。如果X是A-模，那么我们用cl(X)表示对象的类相当于Is$_A$的X，并将其称为类 A-模 X（集合理论、II, §6, No. 9、p. 122）。通过定义，cl(X)与A-模同构于X；此外，两个 A-模 X 和 Y 同构当且仅当我们有 cl(X) = cl(Y)。

设 A 为环。 关系

“$\lambda$ 是类 / 有限生成A-模”

$\lambda ($集合理论中的集合化，II, §1, No. 4，p. 68）。事实上，每个有限生成A-模都同构于形式$A^n_s/R$的A-模，其中$n$是自然数，R子模是$A^n_s$，因此我们的断言来自集合理论，II, §6, No. 9，p. 122。

我们用$\mathscr{F}(A)$表示有限生成A-模的类的集合。每个单A-模都是单生的（VIII，p. 46，命题1），因此单A-模类形式子集$\mathscr{F}$（A），从现在开始我们将其表示为$\mathscr{S}(A)$（或简称为$\mathscr{S}$）。当环 A 是可交换的时，映射 $\mathfrak{m}\mapsto$ cl(A$/\mathfrak{m}$) 是从 A 的最大理想的集合到集合 $\mathscr{S}(A)$ (loc. cit. 和 VIII) 的双射， p. 46、注 1)。当 A 为左阿廷的时，集合 $\mathscr{S}(A)$ 是有限的 (VIII, p. 51, 注 b))。

### 习题{#alg-viii-s3-exercises}

§ 3](exercises/s3/)参见[习题。
