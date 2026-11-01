---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 2
section_title: Linear varieties in a topological vector space
lang: zh
source: evt-i-v
book_pages: TVS I.11-TVS I.16, TVS I.25-TVS I.28
pdf_pages: 0019-0024, 0033-0036
extraction: ocr
subsections:
    - "no": 1
      title: The closure of a linear variety
      page: 11
      pdf_page: 19
    - "no": 2
      title: Lines and closed hyperplanes
      page: 12
      pdf_page: 20
    - "no": 3
      title: Vector subspaces of finite dimension
      page: 13
      pdf_page: 21
    - "no": 4
      title: Locally compact topological vector spaces
      page: 15
      pdf_page: 23
statements: 26
exercises: 15
content_sha256: e5dcfd5e5822906ad8d88022e8fe728d21f8aa92620cfff903452a25a970dcd8
translated_from: content/en/evt/I/02_s2_linear_varieties_in_a_topological.md
translation_method: google
source_content_sha256: 438dff7c2c2dba855400a153f59cbab307df95dd640041fd5d11902a2c5c357e
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: e2b10f2d3a6a0bb0ed8c13ee0bd834974c4e9a0b68d5808ed863ee911d6db6cd
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。拓扑中的线性簇向量空间

### 1. 线性簇的闭包

回想一下 (A, II, § 9.3)，在环 $K$ 的除法向量空间 $E$ 中，非空仿射线性簇（称为“线性簇”，当这不会引起混淆时）是向量子空间的 $E$ 平移下的像。

#### 命题 1 {#evt-i-s2-prop-1 .statement tag=0790}

— *在拓扑向量空间$E$中，线性簇的闭包是线性簇。*

由于每个翻译都是$E$的同态，因此只需证明$E$的向量子空间$M$命题就足够了，在这种情况下，命题已在I、p. 4中得到证明。

#### 推论{#evt-i-s2-n1-cor-1 .statement tag=0791}

— *在拓扑向量空间$E$中，每个超平面要么是闭的，要么是处处稠密的。*

事实上，齐次超平面$H$的闭包只能是$H$或整个空间$E$，因为它是向量子空间包含$H$（命题1）。

当且仅当 $\complement H$ 包含一个内部点时，超平面 $H$ 在 $E$ 中“闭合”。

由集合$A$生成的向量子空间$M$，在拓扑向量空间$E$中，是$A$点线性组合集合 (A, II, § 1.7，道具 9)； $E$ 中 $M$ 的闭包是，根据命题。 1、最小的关闭向量子空间包含$A$；我们说这是*$A$生成的*封闭的向量子空间。

#### 定义 1 {#evt-i-s2-def-1 .statement tag=0792}

— *集合 $A$，在拓扑向量空间 $E$ 中，当且仅当由 $A$ 重合与 $E$* 生成的闭向量子空间（即线性组合的集合）是总的元素的$A$ *处处密集*）。

#### 例 {#evt-i-s2-n1-exa-1 .statement tag=0793}

— 1) 在函数的标准化空间$\mathscr{C}(I; \mathbf{C})$（在域$\mathbf{C}$上），在$I = \{0, 1\}$上连续，值在$\mathbf{C}$、限制到函数的$I$ $x^n \ (n \in \mathbf{N})$ 形式总共集合，由 Weierstrass-Stone 定理制作（GT，X, § 4.2，第 3 个）。同样，函数 $e^{2n\pi ix} \ (n \in \mathbf{Z})$ 形式中的限制至 $I$ 总共集合（GT，X, § 4.4，第 8 条），在 $\mathscr{C}(I, \mathbf{C})$ 的子空间 $P$ 中由函数组成这样$f(0) = f(1)$。

2) 拓扑向量空间 $E$ 中的每个吸收剂集合在非离散值除法环上（特别是 $E$ 中 0 的每个邻域）都是总集合，因为它生成 $E$ （I，p. 7）。因此，在$E$中不稠密的线性簇必然是在$E$（GT，IX, § 5.1）中无处稠密的集合，因为它的闭包不能包含是一个内部点。

#### 定义 2 {#evt-i-s2-def-2 .statement tag=0794}

— *拓扑向量空间$E$的点的族$(a_i)_{i \in I}$被称为拓扑独立，如果对于任何$\kappa \in I$，由$a_i$和$i \neq \kappa$生成的闭合向量子空间不包含 $a_\kappa$.*

#### 例 3 {#evt-i-s2-n1-exa-3 .statement tag=0795}

在$I = \{0, 1\}$、限制到I（函数$e^{2n\pi i x}$（$n \in \mathbf{Z}$）形式）定义的连续函数的规范空间$\mathscr{C}(I; \mathbf{C})$中，一个拓扑独立族。 如果 $f(x)$ 是线性组合 $\sum_{k \neq n} c_k e^{2k\pi i x}$（其中几乎所有 $c_k$ 都是零），那么
$$
\int_0^1 |e^{2n\pi i x} - f(x)|^2 \, dx = 1 + \sum_{k \neq n} |c_k|^2 \geq 1
$$
并且，*更不必说*，平均为值定理
$$
\sup_{x \in I} |e^{2n\pi i x} - f(x)| \geq 1
$$
这表明$e^{2\pi i n x}$不会属于到$e^{2k\pi i x}, \ k \neq n$生成的$\mathscr{C}(I; \mathbf{C})$的封闭向量子空间。

拓扑独立族的元素的集合称为E的*拓扑独立集合*。拓扑独立子集的每个子集都是拓扑独立的；如果 E 是 Hausdorff 空间，则单个点 $x \neq 0$ 的每个子集由……组成是拓扑独立的。

拓扑独立族是独立的（在代数意义上；*cf.* A、II, § 7.1、*注*），但逆命题不正确。

#### 例 4 {#evt-i-s2-n1-exa-4 .statement tag=0796}

在函数的规范空间$\mathscr{C}(I; \mathbf{C})$中，在$I = \{0, 1\}$、限制到I（函数$x^n$（$n \in \mathbf{N}$）形式）上连续，是一个代数独立族。但多项式$(p_n)$存在序列使得$p_n(x^2)$在I（GT，X, § 4.2，引理2）中一致收敛到$x$，这表明$x$属于到闭向量子空间 / $\mathscr{C}(I; \mathbf{C})$ 由函数 $x^{2n}$ ($n \in \mathbf{N}$) 生成。

#### 注 1 {#evt-i-s2-n1-rem-1 .statement tag=0797}

拓扑向量空间的拓扑独立集合族*不一定是归纳*，对于包含关系（I，p. 25，练习2）；因此，这种情况与代数独立集合的情况不同。此外，E 中不一定存在最大拓扑独立子集（I，p. 25，练习 4），因此不一定存在“完全”且拓扑独立的子集。

#### 注 2 {#evt-i-s2-n1-rem-2 .statement tag=0798}

设 M 是 E 的闭向量子空间，并且 $(\dot{a}_i)_{i \in I}$ 是商空间 E/M 中的拓扑独立族。如果 $a_i$ 是类 $\dot{a}_i$ 中的任意元素，则来自 def。 2，并且E在E/M上的典范映射是连续的，因此族$(a_i)_{i \in I}$是拓扑独立的。但是注如果 N 是由 $a_i$ 生成的*封闭* 向量子空间，则可能发生 $M \cap N \neq \{0\}$ (I, p. 25, exerc.2)，因此和 $M + N$ 在代数意义上不一定是直接的（也不是*更不必说*在拓扑意义上）。

### 2. 线路和关闭超平面

#### 命题 2 {#evt-i-s2-prop-2 .statement tag=0799}

*每个 Hausdorff 拓扑向量空间* E *of 维数* 1 *在非离散值除法环* K *同构于* $K_s$； *事实上，对于每个* $a \neq 0$ *在* E 中，*映射* $\xi \mapsto \xi a$ *的* $K_s$ *在* E *上是同构*（在其他字中，* $K_s$ *在* E *上的每个线性映射是同构*）。

由于E上$K_s$的映射$\xi \mapsto \xi a$是双射且连续的（I，p. 1，def.1），因此足以证明它是双连续的。令$\alpha$为实数$> 0$，我们证明E中存在0的邻域V，这样如果$\xi a \in V$则$|\xi| < \alpha$。由于 K 不是离散的，因此存在元素 $\xi_0 \in K$ 使得 $0 < |\xi_0| < \alpha$；但是，由于 E 是 Hausdorff，因此存在 0 的邻域 V，使得 $\xi_0 a$ 不会属于到 V。我们可以假设 V 是平衡的（I，p. 7，命题 4）。但是如果$\xi a \in V$和$|\xi| \geq |\xi_0|$我们有$|\xi_0 \xi^{-1}| \leq 1$和$\xi_0 a = (\xi_0 \xi^{-1}) (\xi a) \in V$；由于最后一个叙述是假的，我们看到$\xi a \in V$意味着$|\xi| < |\xi_0| < \alpha$。这样就完成了证明。

#### 推论 1 {#evt-i-s2-prop-2-cor-1 .statement tag=079A}

*在 Hausdorff 拓扑向量空间 E 中，在非离散值除法环 K 上，维数 1 的每个向量子空间 D 与 $K_s$ 同构的。*

#### 推论 2 {#evt-i-s2-prop-2-cor-2 .statement tag=079B}

*令 E 为非离散值除法环上的拓扑向量空间。每个向量子空间 D（维数 1）是闭齐次超平面 H 的代数补，也是 H 的拓扑补。*

在 D 中，集合 $\{0\}$ 是闭集，是 D 的交和闭集集合 H；因此 D 是豪斯多夫。但由于 E/H 也是 Hausdorff，所以 D 在 E/H 上的典范映射是线性的，根据命理也是同构。 2，由此得出结论（GT，III, § 6.2）。

#### 定理 1 {#evt-i-s2-thm-1 .statement tag=079C}

*令 E 为非离散值除法环上的拓扑向量空间。令 H 为由方程 $f(x) = \alpha$ 定义的 E 中的超平面，其中 f 为线性形式，但不等于零。那么当且仅当 f 连续时 H 在 E 中是闭的。*

条件显然就足够了（GT，I, § 2.1，第1）；我们表明这是必要的。我们可以假设 H 是闭齐次超平面，方程为 $f(x) = 0$。那么商空间 E/H 就是 K 上维数 1 的豪斯多夫拓扑向量空间。我们可以写成 $f = g \circ \phi$，其中 $\phi$ 是 E 在 E/H 上的典范映射，g 是 E/H 在 $K_s$ 上的线性映射；来自道具。 2、g是连续的，因此f也是如此。

#### 推论{#evt-i-s2-n2-cor-1 .statement tag=079D}

*E 上的每个连续线性形式与零不同，都是 E 在 $K_s$ 上的严格态射。*

#### 注 {#evt-i-s2-n2-rem-1 .statement tag=079E}

— 在完整的非离散值除法环上有例的规范拓扑向量空间，其中每个连续的线性形式都相同零（I，p. 25，练习4）；因此，在这样的空间中，每个超平面处处都是稠密的（I，p. 11，推论）。

### 3.向量子空间共有限维

#### 定理 2 {#evt-i-s2-thm-2 .statement tag=079F}

*有限维 n 的每个豪斯多夫拓扑向量空间 E，在完全非离散值除法环 K 上，与 $K_s^n$ 同构的；事实上，对于 K 上的 E 的每个基 $(e_i)_{1 \leq i \leq n}$，线性映射 $(\xi_i) \mapsto \sum_{i=1}^n \xi_i e_i$ 是 E 上的 $K_s^n$ 同构的。*

命题 2 of I, p. 12，意味着 th。 2 对于 $n = 1$ 成立；我们在$n$上争论归纳。设$H$为$e_1, e_2, ..., e_{n-1}$生成的$E$的向量子空间； 归纳假设是$H$ 上$K_s^{n-1}$ 的同构映射 $(\xi_i)_{1 \leq i \leq n-1} \mapsto \sum_{i=1}^{n-1} \xi_i e_i$ 。 子空间 $H$，同构于完整的空间的乘积，是完整的（GT，II, § 3.5，道具10）；因此它在$E$（GT，II, § 3.4，道具8）中*封闭*。设$D$与$E$中的$H$互补，为子空间$Ke_n$； $E$是$H$和$D$的拓扑直和（I，p. 13，cor.2），因此映射

$$
(\xi_i)_{1 \leq i \leq n} \mapsto \sum_{i=1}^n \xi_i e_i
$$

$E$ 上的 $K_s^{n-1} \times K_s$ 为同构。

当 $n > 1$ 假设时，$K$ *完整* 对于定理 2 的有效性至关重要。事实上，令 $K$ 为非完整值除法环，并令 $\hat{K}$ 为其完成：对于每个 $a \neq 0$ $\hat{K}$ 集合 $K.a$ 在 $\hat{K}$ 中处处稠密，因为 $x \mapsto xa$ 是 $\hat{K}$ 自身的同胚。如果$K$上的拓扑向量空间$\hat{K}$的$a \notin K$、子空间$K + Ka$是$K$上的维数2，但它与$K_s^2$不同构，因为每个$K + Ka$中的维数1的子空间在$K + Ka$中是稠密的。

#### 推论 1 {#evt-i-s2-thm-2-cor-1 .statement tag=079G}

*在完整的非离散值除法环$K$上的豪斯多夫拓扑向量空间$E$中，有限维的每个向量子空间$F$在$E$中闭合。*对于，如果$F$ 是维数 $n$ 那么它与 $K_s^n$ 同构的；因此它是完整的，因此在$E$（GT，II, § 3.4，提案8）中关闭。

#### 推论 2 {#evt-i-s2-thm-2-cor-2 .statement tag=079H}

*令$K$为完全非离散值除法环，$E$为有限维在$K$上的豪斯多夫拓扑向量空间。如果$F$是$K$上的任何拓扑向量空间，则$F$中$E$的每个线性映射都是连续的。*

#### 推论 3 {#evt-i-s2-thm-2-cor-3 .statement tag=079I}

*在 Hausdorff 拓扑向量空间 $E$ 中，在完全非离散值除法环上，每个有限独立集合都是拓扑独立的。*

#### 推论 4 {#evt-i-s2-thm-2-cor-4 .statement tag=079J}

*令 $E$ 为完整非离散值除法环上的拓扑向量空间。 If $M$ is a closed vector subspace of $E$ and $F$ is a vector subspace of $E$ of finite dimension, then the subspace $M + F$ is closed in $E$.* Write $\phi$ for the canonical homomorphism of $E$ on the quotient space $E/M$ (necessarily Hausdorff). 那么子空间$M + F$与$\overline{\phi}^{-1}(\phi(F))$相同。 现在$\phi(F)$在$E/M$中属于有限维，因此（cor.1）$\phi(F)$在$E/M$中闭，并且在推论中，$\overline{\phi}^{-1}(\phi(F))$在$E$中闭。

我们注，如果$M$和$N$是豪斯多夫拓扑向量空间$E$中*任何*两个闭的向量子空间，那么$M + N$不一定在$E$中闭，\*即使$E$是一个希尔伯特空间 \* (cf. IV, p. 64, 练习 13, d))。

#### 命题 3 {#evt-i-s2-prop-3 .statement tag=079K}

*令 $E$ 为完整非离散*值除环 $K$ 上的拓扑向量空间。令$M$为$E$中有限余维$n$的闭向量子空间。那么子空间$N$是$E$中$M$的代数补，也是拓扑补。

在 $N$ 中，集合 $\{0\}$ 闭合，因为它是 $N$ 和集合 $M$ 的交，在$E$ 中闭合；因此 $N$ 是豪斯多夫。由于$E/M$也是Hausdorff，$E/M$上$N$的典范映射是线性双射的，是双连续的（I，p. 14，cor.2），由此得出命题。

#### 推论{#evt-i-s2-n3-cor-1 .statement tag=079L}

*令$E$和$F$是完整非离散值除法环上的两个拓扑向量空间。如果 $F$ 是 Hausdorff 并且属于有限维，则 $F$ 上 $E$ 的每个连续线性映射都是严格的态射。*

#### 注 {#evt-i-s2-n3-rem-1 .statement tag=079M}

— 当 $K$ 为*离散*时，第 2、3 个结果不再有效。对于例，令$K_1$为非离散值除法环，$K$为通过在$K_1$上赋予$K_1$不正确的绝对值值而获得的离散除法环。那么$K_1$是维数1在$K$上的拓扑向量空间，但它与$K_s$不同构。然而，我们可以证明，即使 $K$ 是离散的，第 2、3 项的结果也是有效的，前提是我们对拓扑向量空间进行考虑，性质的基本系统为 *balanced* 邻域为 0（即邻域 $V$，使得$K.V = V$) (I, p. 27, 练习14);这个条件（当$K$是非离散值除法环 *cf.* I，p. 7，道具4时始终满足）对于所有拓扑向量空间超过$K$都有效，如前面的例显示。

### 4.局部紧拓扑向量空间

#### 定理 3 {#evt-i-s2-thm-3 .statement tag=079N}

*令$K$为完全非离散值除法环。如果$E$是$K$上的豪斯多夫拓扑向量空间，即$E$中0的某些邻域$V$是预紧的，则$E$是有限维。如果$E \neq \{0\}$，则$K$和$E$都是局部紧致的。*

在证明第一个断言中，我们只需要考虑$E$*完整*的情况；因为$E$是其补全$\hat{E}$的处处稠密子空间，并且$\hat{E}$中$V$的闭包$\overline{V}$是紧致的并且是$\hat{E}$中0的邻域（GT，III, § 3.4，道具7）。

我们可以假设 $E$ 中有一个 0 的 *紧凑* 邻域 $V$。令 $\alpha \in K$ 使得 $0 < |\alpha| < 1$；那么有有限多个点 $a_i \in V$ 使得

$$
V \subset \bigcup_i (a_i + \alpha V).
$$

令$M$为$a_i$生成的$E$的有限维子空间； $E$（I、p. 14，cor.1）关闭。在豪斯多夫拓扑中，$V$的向量空间$E/M$典范像是0的紧邻域$W$，使得$W \subset \alpha W$；因此$\alpha^{-1} W \subset W$，并且在$n$上归纳，每正整数$n$有$\alpha^{-n} W \subset W$。由于$W$具有吸水性，我们结论即$W = E/M$；因此 $E/M$ 是*紧凑*。因此，为了完成定理中第一个断言的证明，建立下面的引理就足够了。

#### 引理 1 {#evt-i-s2-lem-1 .statement tag=079O}

— *非离散值除法环上的任何紧凑拓扑向量空间 $E$ 都只是集合 $\{0\}$。*

由于 E 是完整的，我们可以假设 K 是完整的（I，p. 6）。如果 E $\neq \{0\}$ 则 E 包含一条在 E (I, p. 14, cor. 1) 中闭合的线，因此是紧凑的。这条线与 $K_s$ (I, p. 12, 命题 2) 同构的，因此 K 必须是紧致的。现在$\mathbf{R}$中K的映射$\xi \mapsto |\xi|$是连续的，因此K的像必须是有界的，另一方面存在$\gamma \in K$和$|\gamma| > 1$，并且集合$|\gamma^n| = |\gamma|^n, n \in \mathbf{N}$是无界的。这个矛盾表明$E = \{0\}$。

证明定理中的第二个断言，如果$E \neq \{0\}$则从定理的第一个部分开始，E与$K_s^n$与$n > 0$同构的；现在 K 是完备的，因此 E 也是完备的，因此 E 是局部紧的。但 $K_s$ 与 E (I, p. 12, prop. 2) 中的一条线同构，该线在 E (I, p. 14, cor. 1) 中必然闭合；由此可见 K 是局部紧致的。

#### 注 {#evt-i-s2-n4-rem-1 .statement tag=079P}

结果。如果 K 是离散除法环，如 $\mathbf{R}$ 的例所示（通常为拓扑），则 3 不再成立，被视为离散域 $\mathbf{Q}$ 上的拓扑向量空间。

### 习题{#evt-i-s2-exercises}

§ 2](exercises/s2/)参见[习题。
