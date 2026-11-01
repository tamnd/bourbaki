---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 3
section_title: Uniform structures on groups
lang: zh
source: top-i-iv
book_pages: 242-250, 306-307
pdf_pages: 0248-0256, 0312-0313
extraction: ocr
subsections:
    - "no": 1
      title: THE RIGHT AND LEFT UNIFORMITIES ON A TOPOLOGICAL GROUP
      page: 242
      pdf_page: 248
    - "no": 2
      title: UNIFORMITIES ON SUBGROUPS, QUOTIENT GROUPS AND PRODUCT GROUPS
      page: 244
      pdf_page: 250
    - "no": 3
      title: COMPLETE GROUPS
      page: 245
      pdf_page: 251
    - "no": 4
      title: COMPLETION OF A TOPOLOGICAL GROUP
      page: 246
      pdf_page: 252
    - "no": 5
      title: UNIFORMITY AND COMPLETION OF A COMMUTATIVE TOPOLOGICAL GROUP
      page: 248
      pdf_page: 254
statements: 18
exercises: 12
content_sha256: fae55b2d40efd2f43bcaa8e1d6337c7fb957310b8935541a6655bc2f07d28624
translated_from: content/en/top/III/03_s3_uniform_structures_on_groups.md
translation_method: google
source_content_sha256: ccad26133e828ceb3575a2c0a99aca5048899ccdf5ec5a7789d9d8ec80447527
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 971abd881c08c316df5e360b6fdb1bb3e0e958e008c955b85ea8de45b838134e
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 3. 制服结构群

### 1. 拓扑群上的左右一致

在拓扑群 G 中，我们可以通过如下操作感知定义“足够接近点”的概念，从而定义统一结构的可能性：如果x和y是G的任意两个点，我们将翻译应用于两个点，将其中一个（例如x）发送到单位元素e；然后，x 和 y 的“接近度”在某种意义上可以通过 y 翻译成的 e 的邻域 V 来评估。这种平移包括将 x 和 y 乘以$x^{-1}$，可以在右侧或左侧进行，我们将看到，在任何一种情况下，我们都可以有效地获得 G 上的均匀性，该一致性与 G 的拓扑兼容。让我们以在右侧进行平移的情况为例；那么对于 e 的每个邻域 V 都有对 $(x, y) \in G \times G$ 的对应集合 $V_d$ 使得$yx^{-1} \in V$。令$\mathfrak{G}_d$为集合$V_d$的族，因为V穿过e的邻域过滤器$\mathfrak{B}$。那么$\mathfrak{G}_d$就是随行人员的基本系统（章II, § 1, no. 1）。因为从$e \in V$开始，$G \times G$的对角线$\Delta$对于每个$V \in \mathfrak{B}$都包含在$V_d$中，因此$\mathfrak{G}_d$是一个过滤器基并且满足公理$(U'_1)$；由于关系$yx^{-1} \in V$和$xy^{-1} \in V^{-1}$是等价的，我们有$\overline{V}_d^1 = (V^{-1})_d$，因此通过(GV$_{\text{II}}$)得到$\overline{V}_d^1 \in \mathfrak{G}_d$，因此满足(U'$_{\text{II}}$)；最后，关系$zx^{-1} \in V$和$yz^{-1} \in V$意味着$yx^{-1} \in V.V$；因此$V_d \circ V_d$包含在(V.V)$_d$中，并且(GV$_{\text{I}}$)表明$\mathfrak{G}_d$满足(U'$_{\text{III}}$)。

$\mathfrak{G}_d$定义的均匀性与G的拓扑兼容，因为关系、$y \in V_d(x)$和$y \in V.x$等价于定义；其他字$V_d(x) = V.x$。

当翻译在左边时，论证是类似的，因此我们可以做出以下定义：

#### 定义 1 {#top-iii-s3-def-1 .statement tag=0BJX}

*拓扑群 G 上的右（左）均匀性是通过对单位元素 e、集合的每个邻域 V 进行对应获得基本系统周边的均匀性V$_d$（分别V$_s$）对$(x, y)$，使得$yx^{-1} \in V$（分别$x^{-1}y \in V$）。*

如果V贯穿e的邻域的基本系统，则集合V$_d$（分别V$_s$）形式右随行人员的基本系统 （左）均匀性。

到制服空间的拓扑上的每个命题，还有群的拓扑上的对应命题；根据定义 1 和公式 $V_d(x) = V.x,\ V_d(A) = V.A,\ V_s(x) = x.V,\ V_s(A) = A.V,$ 进行翻译，即定义的直接的推论。对于例，如果A是G的任何非空子集，那么我们有（章II, § 1, no. 2，推论1到命题2）

$$
\overline{A} = \bigcap_{V \in \mathfrak{B}} V.A = \bigcap_{V \in \mathfrak{B}} A.V.
$$

再次（章 II, § 1, no. 2，推论 3 到命题 2），*每个 Hausdorff 群都是正则*。

拓扑群上的左右均匀性通常是不同的（参见习题 4）。显然，如果群是*可交换的*，则重合，那么$V_d = V_s$；如果群是*紧凑*（章II, § 4, no. 1，定理1），它们也重合。

一般来说，我们用$G_s$（或$G_d$）表示通过赋予集合 G 左（或右）均匀性而获得的*均匀空间*。

#### 命题 1 {#top-iii-s3-prop-1 .statement tag=0BJY}

*左平移和右平移是右均匀性自身的同构。*

至于正确的翻译，结果很清楚，因为关系$yx^{-1} \in V$相当于$(ya)(xa)^{-1} \in V$[在其他字，映射$(x, y) \to (xa, ya)$留下$V_d$固定]。对于左翻译，结果来自$(GV_{\text{III}})$；对于$yx^{-1} \in V$当且仅当$(ay)(ax)^{-1} \in aV a^{-1}$；因此$x \to ax$在$G_d$上一致连续。

类似地，右平移和左平移是左均匀性自身的同构。

因此，对于$G$的群结构、$G$的拓扑以及$G$的均匀性，$G$的每个*内自同构* $x \to axa^{-1}$都是自同构。

#### 命题 2 {#top-iii-s3-prop-2 .statement tag=0BJZ}

*对称性* $x \to x^{-1}$ *右侧均匀度与左侧均匀度的同构。*

这是定义 1 中的直接的推论。

读者应该注意，假设一致空间$G_d \times G_d$到一致空间$G_d$的映射$(x, y) \to xy$通常是一致连续的。类似地，对称性 $x \to x^{-1}$（被视为 $G_d$ 在 $G_d$ 上的映射）通常不是一致连续的（参见习题 3 和 4）。

#### 命题 3 {#top-iii-s3-prop-3 .statement tag=0BK0}

*拓扑群* $G$ *到拓扑群* $G'$ *的每个连续同态* $f$ *在被视为映射 of* $G_d$ *到* $G'_d$ *（或 of*）时是一致连续的$G_s$*变成*$G'_s$）。

因为如果$V'$是$G'$中单位元素的邻域，并且$V = \overline{f}^{-1}(V')$，那么关系$yx^{-1} \in V$意味着
$$
f(y)(f(x))^{-1} = f(yx^{-1}) \in V'.
$$

### 2. 子群、商群和乘积群的均匀性

如果$H$是拓扑群$G$的子群，那么$G$的右均匀性在$H$上引起的均匀性正是拓扑群$H$的右均匀性。

如果$H$是$G$的正常子群，并且如果$\varphi$是$G$到$G/H$的典范映射，我们得到商群$G/H$右均匀性的基本系统：与$G/H$的所有对$(\dot{x}, \dot{y})$中的$G$、集合中单位元素中的每个邻域$V$相关联，使得$\dot{x}\dot{y}^{-1} \in \varphi(V)$(§ 2, no. 6，命题) 17）。这个条件意味着至少有一个点$x \in \dot{x}$和至少一个点$y \in \dot{y}$使得$yx^{-1} \in V$[即这样$(x, y) \in V_d$]。特别是，如果$N$是子集$\{e\}$对$G$的闭包，那么$G/N$上的右均匀性同构于与$G$上的右均匀性*相关联的豪斯多夫均匀性（cf.章） II, § 3, no. 8）。

最后，在拓扑群的族$(G_i)$的乘积上，右均匀性是$G_i$右均匀性的*乘积* (cf. 章 II, , no. 6)

左均匀性也有类似的结果。

当且仅当每个因子 $G_i$ 重合上的左右均匀性时，乘积群 $\prod_{i \in I} G_i$ 的左右均匀性相同。如果某些 $G_i$ 是可交换的而其他是紧的，情况总是如此。

### 3. 完成群

#### 定义 2 {#top-iii-s3-def-2 .statement tag=0BK1}

*如果拓扑群的左右均匀性是完整空间的结构，则称拓扑群是完整的。*

从 no. 1 的命题 2 开始，对于群来说，只要其一致性中的*一个*是完整的空间的结构就足够了。当且仅当其关联的 Hausdorff 群 ($§\ 2$, no. 6) 完备时，$G$ 才是完备的。

完整的群的每个*闭合* 子群都是完整的（章 II, § 3, no. 4、命题 8）。完整的群中的每一个乘积都是完整的（章II, § 3, no. 5，命题10）。

另一方面，如果$G$是完整的群并且$H$是$G$的闭法线子群，则商群$G/H$不一定是完整的（但是，参见章IX, § 3, no. 1， 命题4)。

#### 命题 4 {#top-iii-s3-prop-4 .statement tag=0BK2}

*如果在拓扑群 $G$ 中，$e$ 中存在邻域 $V$ 且其右均匀性或左均匀性是完整的，则 $G$ 是完整的。*

假设对于例，$V$关于右均匀性是完备的，并令$\mathfrak{F}$是$G_d$上的柯西滤波器；那么$\mathfrak{F}$包含一个$V_d$小集合$M$，如果$x_1 \in M$我们因此有$M \subset Vx_1$。因此$\mathfrak{F}$在$G_d$的完整子空间$Vx_1$上的迹是一个柯西滤波器，它收敛到点$x_0$；由于$x_0$是$\mathfrak{F}$的集群点，因此它是$\mathfrak{F}$的极限（章II, § 3, no. 2，推论2到命题5）。

#### 推论 1 {#top-iii-s3-prop-4-cor-1 .statement tag=0BK3}

*局部紧凑群已完成。*

对于每个紧凑型空间而言，其独特的一致性都是完整的（章 II, § 4, no. 1、定理 1）。

#### 推论 2 {#top-iii-s3-prop-4-cor-2 .statement tag=0BK4}

*Hausdorff 拓扑群 $G$ 的每个局部紧致子群都在 $G$ 中闭合。*

对于每一个完整的 Hausdorff 制服子空间，空间都是封闭的 (章 II, , no. 4, 命题 8)

#### 命题 5 {#top-iii-s3-prop-5 .statement tag=0BK5}

令$G_1$为拓扑群，让$G_2$为完整的Hausdorff拓扑群，并令$H_1$（或$H_2$）为$G_1$（或$G_2$）的稠密子群。那么$H_1$到$H_2$的每一个连续同态$u$都可以唯一地扩展到$G_1$到$G_2$的连续同态$\bar{u}$。此外，如果$G_1$是豪斯多夫且完备，并且如果$u$是$H_1$到$H_2$的同构，那么$\bar{u}$是$G_1$到$G_2$的同构。

$\bar{u}$ 相对于 $H_1$ 和 $H_2$ (no. 1, 命题 3) 一致连续，因此将 $G_1$ 的唯一扩张到映射 $\bar{u}$ 接纳到$G_2$ 相对于这些群 (章 II, § 3, no. 6, 定理 2) 的右一致性一致连续。此外，凭借扩张的原理恒等式（章I, § 8, no. 1，推论1到命题2），$\bar{u}$是$G_1$的同态变成$G_2$， 从而命题的第一个断言。为了证明第二个断言，只需将$H_2$的同构$v$考虑到$H_1$，这是$u$的逆，并且它的扩张$\bar{v}$到连续的同态就足够了$G_2$ 变为$G_1$；由于扩张的唯一性，$\bar{v} \circ \bar{u}$和$\bar{u} \circ \bar{v}$分别是$G_1$和$G_2$的恒等映射，因此（集合理论，R，§ 2, no. 12）$\bar{u}$是双射。

#### 注 {#top-iii-s3-n3-rem-1 .statement tag=0BK6}

如果连续同态 $u$ 是双射的，则一般不得出 $\bar{u}$ 是单射或满射 (cf. 习题 12)；但请参阅no. 5、命题 9。

### 4. 完成拓扑群

令 $G$ 为 Hausdorff 拓扑群。均匀的空间$G_d$可以被认为是其补全$\hat{G}_d$的密集子空间。我们将研究$G$是否可以被视为完整Hausdorff群$G'$的稠密子群。如果是这样，那么一致的空间$G'_d$必须同构于$\hat{G}_d$（章II, § 3, no. 6，推论定理2），因此我们必须能够在$\hat{G}_d$上实现定义拓扑群结构， 诱导 $G$ 上的给定拓扑群结构。因此我们必须检查：
1）是否可以通过函数、$xy$和$x^{-1}$分别将扩展连续到$\hat{G}_d \times \hat{G}_d$和$\hat{G}_d$； 2) 这样扩展的函数是否确实在$\hat{G}_d$上做定义群结构（然后它们必然在$\hat{G}_d$上定义拓扑群结构诱导$G$上给定的结构）。接下来我们要确定3）当前面的运算可能时，它们定义的拓扑群是完整的。最后，我们将看到4）如果给定的条件存在完整的群满足，那么它在同构之前都是唯一的。

1) Extension of $xy$ and $x^{-1}$ by continuity. 由于函数$xy$和$x^{-1}$一般不是均匀连续的，我们不能应用均匀连续函数的扩张的定理（章II, § 3, no. 6，定理2）。 尽管如此，我们可以凭借章II, § 3, no. 6的命题11和以下命题来扩展$xy$：

#### 命题 6 {#top-iii-s3-prop-6 .statement tag=0BK7}

令$\mathfrak{F}$和$\mathfrak{G}$为$G_d$上的两个柯西滤波器。那么映射$(x, y) \to xy$下的滤波器$\mathfrak{F} \times \mathfrak{G}$的像就是$G_d$上的柯西滤波器基。

让我们评估$xy$和$x'y'$在$G_d$中的“接近度”；在其他字，让我们形式乘积$(x'y')(xy)^{-1} = x'y'y^{-1}x^{-1}$。对于每个$a \in G$，我们也可以写成$(x'y')(xy)^{-1} = (x'a^{-1})(ay'y^{-1}a^{-1})(ax^{-1})$。我们将看到，通过适当的$a$的选择，当对$(x, y)$和$(x', y')$属于足够小到$\mathfrak{F} \times \mathfrak{G}$的集合时，这个乘积的三个因子都非常小。令$V$为$G$中$e$的任意邻域；然后是$V_d$-小集合$A \in \mathfrak{F}$。 选择$a$在$A$中，那么如果$x$和$x'$是$A$中的任意两个点，我们有$x'a^{-1} \in V$和$ax^{-1} \in V$。另一方面，关系$ay'y^{-1}a^{-1} \in V$相当于
$$
y'y^{-1} \in a^{-1}Va = W,
$$
由于$W$是$e$的邻域，所以有一个$W_d$小集合$B \in \mathfrak{G}$。因而，对于$A \times B$中的所有$(x, y)$和$(x', y')$，我们有$(x'y')(xy)^{-1} \in V^3$，这完成了证明。

在阶中，$x^{-1}$可以通过连续性扩展到$\hat{G}_d$，在对称性*$x \to x^{-1}$下，$G_d$上的柯西滤波器*像是$G_d$*上的柯西滤波器（章II, § 3, no. 6， 命题11)。拓扑群中存在例，其中条件不满足（cf.章X, § 3，习题16）；我们假设证明的剩余部分已经满足。

2) *在* $\hat{G}_d$ 上扩展函数* $xy$ 和 $x^{-1}$ *定义群结构。因为如果我们将恒等式（章I, § 8, no. 1，命题2，推论1）中的扩张的原理应用于函数$x(yz)$和$(xy)z$，在$\hat{G}_d \times \hat{G}_d \times \hat{G}_d$上定义并且在密集子空间上相等$G_d \times G_d \times G_d$，我们看到合成$(x, y) \to xy$的律在$\hat{G}_d$上*关联*。出于同样的原因，函数$x, ex, xe$在$\hat{G}_d$上是相同的，函数$e, xx^{-1}, x^{-1}x$在$\hat{G}_d$上是相同的。

3) *拓扑群* $\hat{G}_d$ *已完成*。令$\mathfrak{U}_d$为其*右均匀度*，并令$\mathfrak{U}$为通过*完备的*$G$的右均匀度而获得的$\hat{G}_d$上的均匀度。那么 $\mathfrak{U}$ 和 $\mathfrak{U}_d$ 诱导在 $G$ 上具有*相同的*均匀性，因此每个柯西滤波器基 $\mathfrak{B}$ *在* $G$ *相对于* $\mathfrak{U}_d$ *也是一个柯西滤波器基到* $\mathfrak{U}$。现在$\mathfrak{B}$收敛于$\hat{G}_d$，因为$\mathfrak{U}$是完全一致的；并且由于 $\mathfrak{U}$ 和 $\mathfrak{U}_d$ 诱导在 $\hat{G}_d$ 上具有相同的拓扑，因此 (章 II, , no. 4, 命题 9) $\mathfrak{U}_d$ 是完全一致的。该结论还表明 $\mathfrak{U}$ 和 $\mathfrak{U}_d$ 重合（章 II, § 3, no. 6，定理 2 的推论）

4) *唯一性.* 这是从命题 5 of no. 3 得出的。

到和向上，我们证明了以下定理：

#### 定理 1 {#top-iii-s3-thm-1 .statement tag=0BK8}

*豪斯多夫拓扑群$G$同构于完整群$\hat{G}$的稠密子群当且仅当像，在对称性$x \to x^{-1}$下，关于柯西滤波器的正确均匀性$G$ 是关于这种均匀性的柯西滤波器。完整的群$\hat{G}$（称为$G$的完成）是唯一的（最多同构）。*

#### 命题 7 {#top-iii-s3-prop-7 .statement tag=0BK9}

*令 $G$ 为 Hausdorff 拓扑群，其完成性为 $\hat{G}$。然后是$G$形式中的$\hat{G}$、邻域、单位元素的闭包，以及$\hat{G}$中的邻域、单位元素的基本系统。*

由于$\hat{G}$是正则，$\hat{G}$包含中单位元素的每个邻域都是$\hat{G}$中$e$的开邻域$U$的闭包$V$，并且$V$也是$U$在$G$上的迹线的闭合。

令$G$为群，这不一定是Hausdorff；设 $N = \overline{\{e\}}$，并设 $G' = G/N$ 为与 $G$ (§ 2, no. 6) 伴随的 Hausdorff 群。如果$G'$有一个补全$\hat{G}'$，这个补全称为$G$的*豪斯多夫补全*，记为$\hat{G}$； $\hat{G}'_d$（分别$\hat{G}'_s$）是均匀空间$G_d$（分别$G_s$）的*豪斯多夫完成*（章II, § 3, no. 7）。

#### 命题 8 {#top-iii-s3-prop-8 .statement tag=0BKA}

*令$G$为拓扑群，具有豪斯多夫完成$\hat{G}'$。然后，$G$的每个连续同态$u$转化为完全Hausdorff群$H$都可以唯一分解为$u = v \circ \varphi$，其中$v$是$\hat{G}'$的连续同态分解为$H$并且$\varphi$ 将$G$ 典范映射放入$\hat{G}'$（将$G'$ 典范嵌入合成放入$\hat{G}'$ 和$G$ 典范同态 $\psi$ 放入$G/N = G'$).*

由于$u$的核是闭集，包含$e$，所以包含$N$，因此$u$可以写成$u = w \circ \psi$，其中$w$是同态的连续同态 $G'$ 变为$H$；现在应用命题 5 / no. 3 至 $w$。

### 5. 可交换拓扑群的均匀性和完备性

我们已经说过，交换拓扑群 $G$ 上的左右一致重合；每当我们谈到$G$的“均匀性”时，我们指的就是这种独特的均匀性。

#### 定理 2 {#top-iii-s3-thm-2 .statement tag=0BKB}

令 $G$ 为交换拓扑群。那么函数$x^{-1}$和$xy$分别在$G$和$G \times G$上均匀连续。此外，$G$承认Hausdorff完成$\hat{G}$，并且$\hat{G}$是可交换的。

$x^{-1}$ 的一致连续性源自 no. 1 的命题 2，$xy$ 的一致连续性源自 no. 1 的命题 3，因为 $(x, y) \to xy$ 是 $G \times G$ 到 $G$ 的连续同态。如果 $G$ 是 Hausdorff，则它满足条件 of 定理 1 of no. 4（每个 Hausdorff 群其左右均匀性为重合）；此外，函数$xy$和$yx$在$\hat{G} \times \hat{G}$乘以扩张的原理等式上相等；因此，通过在一般情况下考虑与$G$相关的Hausdorff群，定理的第二个部分。

特别是从定理可以得出，如果$f$和$g$是统一空间$X$到可交换群$G$的两个一致连续的映射，加法书写，则函数$-f$和$f + g$ 一致连续。

#### 命题 9 {#top-iii-s3-prop-9 .statement tag=0BKC}

令$G$为可交换的群，并令$\mathfrak{T}_1, \mathfrak{T}_2$为与$G$的群结构兼容的两个豪斯多夫拓扑。假设 $\mathfrak{T}_1$ 比 $\mathfrak{T}_2$ 更更细，并且$\mathfrak{T}_1$ 存在$o$ 的邻域基本系统，对于 $\mathfrak{T}_2$ 是封闭的。令$G_1, G_2$分别为$G$相对于拓扑$\mathfrak{T}_1, \mathfrak{T}_2$的补全，令$f : G_1 \to G_2$为$G$的连续同态，其中扩展恒等映射（no. 3，命题5）。那么 $f$ 是单射的。

假设$G$是加法写的。令 $\mathfrak{U}_1$ 为 $G$ 相应的 (no. 1) 到拓扑 $\mathfrak{T}_1$ 的均匀性：足以证明，如果 $\mathfrak{F}$ 和 $\mathfrak{F}'$ 是两个最小柯西滤波器 (章 II, § 3, no. 2)，则$\mathfrak{U}_1$，在$G_2$收敛到相同的点$a$，然后$\mathfrak{F} = \mathfrak{F}'$（章II, § 3, no. 7）。为此，只要证明 $\mathfrak{F} \cap \mathfrak{F}'$ 是关于 $\mathfrak{U}_1$ 的柯西滤波器即可。令$V$为$G$中$o$相对于$\mathfrak{T}_1$的邻域，使得$V$在$\mathfrak{T}_2$中闭合，并令$W$为$o$的对称邻域 $G$相对于$\mathfrak{T}_1$，使得$W + W \subset V$。到假设时，$\mathfrak{F}$（或$\mathfrak{F}'$）中存在$W_d$小集合$M$（或$M'$）；如果$x \in M$和$y \in M$我们有$y - x \in W$，即$y \in x + W$。如果$\overline{W}$和$\overline{V}$是$G_2$中$W$和$V$的闭包，那么$y \in x + \overline{W}$，因此，由于$a$在$M$的闭包中，因此$a \in x + \overline{W}$对于每个$x \in M$。类似地，对于每个$x' \in M'$，$a \in x' + \overline{W}$，因此$x - x' \in \overline{W} + \overline{W}$；但由于$(x, y) \to x + y$是$G_2 \times G_2$到$G_2$的连续映射，所以我们有$\overline{W} + \overline{W} \subset \overline{W} + \overline{W} \subset \overline{V}$。由此可见，如果$x \in M$和$x' \in M'$，则$x - x' \in \overline{V} \cap G = V$，因为$V$在$\mathfrak{T}_2$中闭合；这样就完成了证明。

#### 推论 1 {#top-iii-s3-prop-9-cor-1 .statement tag=0BKD}

在命题 9的假设下，如果$A$是$G$的子集，对于$U_2$相应的到$\mathfrak{T}_2$的均匀性来说是完全的子空间，那么$A$对于均匀性来说也是完全的子空间 $U_1$相应的至$\mathfrak{T}_1$。

如果$A_1$是$G_1$中$A$的闭包，则$f(A_1)$包含在$G_2$中$A$的闭包中，假设等于$A$。由于$f(A) = A$乘以定义和$f$是单射的，所以我们有$A_1 = A$。

#### 推论 2 {#top-iii-s3-prop-9-cor-2 .statement tag=0BKE}

令$G$为可交换的群，并令$\mathfrak{T}_1, \mathfrak{T}_2$为与$G$的群结构兼容的两个拓扑。假设 $\mathfrak{T}_1$ 比 $\mathfrak{T}_2$ 更细，并且存在 $O$ 的邻域的基本系统 $\mathfrak{B}$ 关于 $\mathfrak{T}_1$ 的均匀性 $U_2$ 相应的是完整的$\mathfrak{T}_2$。那么$G$相对于均匀性$U_1$相应的到$\mathfrak{T}_1$来说是完整的。

$\mathfrak{B}$的集合在拓扑$\mathfrak{T}_2$中闭合，因此完成推论1的均匀性$U_1$；因此，结果来自 no. 3 的命题 4。

### 习题{#top-iii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
