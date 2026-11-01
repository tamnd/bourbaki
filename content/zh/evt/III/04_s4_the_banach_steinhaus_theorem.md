---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 4
section_title: The Banach-Steinhaus theorem
lang: zh
source: evt-i-v
book_pages: TVS III.23-TVS III.28, TVS III.43-TVS III.46
pdf_pages: 0155-0160, 0175-0178
extraction: ocr
subsections:
    - "no": 1
      title: Barrels and barrelled spaces
      page: 24
      pdf_page: 156
    - "no": 2
      title: The Banach-Steinhaus theorem
      page: 25
      pdf_page: 157
    - "no": 3
      title: Bounded subsets of $\mathscr{L}(E; F)$ (quasi-complete case)
      page: 27
      pdf_page: 159
statements: 24
exercises: 22
content_sha256: c13a7c17bb1f025b8de79bcc57cd616f1c38eb6e890c42153ef22953790bda8b
translated_from: content/en/evt/III/04_s4_the_banach_steinhaus_theorem.md
translation_method: google
source_content_sha256: 60bbc08b0bba45d478ba940cb18808c44414344f01456f8e5401229c26b9224a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: e7260023cfde1cfc25d7a1a5ce277ec13e067ae27dbbbb6650fe1531078ce0c7
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。巴纳赫-斯坦豪斯定理

*在本段中，E 表​​示局部凸空间，E' 表示其对偶。每当我们谈论 E' 上的弱拓扑时，我们指的是 $\sigma(E', E)$。*

### 1.桶装和桶装空间

#### 命题 1 {#evt-iii-s4-prop-1 .statement tag=07NZ}

令 T 为 E 的子集。以下条件是等效的：

(i) T 是凸形的、平衡的、封闭的和吸收性的。

(ii) T 是 E' 中凸、平衡且弱有界集合 M 的极坐标。

(iii) E 上存在一个下半连续半范数 p，使得 T 是所有 x ∈ E 满足 p(x) ≤ 1 的集合。

(i) ⇒ (ii) : 在(i)的假设下，令M = T°；则 M 是凸的并且在 E' 中平衡。对于每个 x ∈ E，存在实数 r > 0 使得 rx ∈ T，因此 |u(x)| ≤ $\frac{1}{r}$ 对于所有 u ∈ M；在其他字 M 是弱有界的。来自科。 3 of II, p. 45，我们有 T = M°，因此 T 满足 (ii)。

(ii) ⇒ (iii) : 在 (ii) 的假设下，令 $p(x) = \sup_{u \in M} |u(x)|$ 对于所有 x ∈ E。T = M° 由所有 x ∈ E 组成且 p(x) ≤ 1 为直接的。E' 上的半范数 p 是下半连续的，是连续族函数 (GT, IV, § 6, No. 2，推论）。

(iii)⇒(i)：这很清楚。

#### 推论{#evt-iii-s4-n1-cor-1 .statement tag=07O0}

以下条件是等价的：

(i) E' 的每个弱有界子集都是等连续的；

(ii) E 中每个凸、平衡、闭、吸收的集合都是 0 的邻域；

(iii) E 上的每个下半连续半范数都是连续的。

#### 定义 1 {#evt-iii-s4-def-1 .statement tag=07O1}

集合 T 满足相当于 prop 的条件。 1 据说是 E 中的一个桶。

#### 定义 2 {#evt-iii-s4-def-2 .statement tag=07O2}

如果空间 E 满足 prop 推论的等价条件，则称 E 为桶状。 1.

我们知道（III，p. 22，命题 9）E 的对偶 E' 的每个等连续子集都是强有界和弱有界的。因此，我们可以将桶装空间的定义重述如下：

#### 学院{#evt-iii-s4-n1-sch-1 .statement tag=07O3}

在桶状空间的对偶中，等连续集合的类、强有界集合的类、弱有界集合的类以及弱拓扑的相对紧集的类都是相同的。如果 E 是 Hausdorff 且桶状的，并且如果 E'_b 是其强对偶，则 0 的邻域极坐标位于另一个规范出生学的空间形式基之一中，以及空间形式之一中的有界子集极坐标基为其他空间的0的邻域的过滤器。

#### 命题 2 {#evt-iii-s4-prop-2 .statement tag=07O4}

每个局部凸空间 E（即 Baire 空间 (GT, IX, § 5, No. 3)）都是桶状的。

设T为E中的一个桶；由于 T 是吸收性的，E 是闭集合 nT 的并 (n 整数 > 0)；因为 E 是 Baire 空间，所以这些集合包含中至少有一个是内部点，因此 T 本身有一个内部点 x。如果$x \neq 0$，因为$-x \in T$，并且0是具有端点x和$-x$的开段的点，则0是凸集合T的内部点（II，p. 14，道具16）。因此 T 是 0 的邻域。

#### 推论{#evt-iii-s4-n1-cor-2 .statement tag=07O5}

— *每个 Fréchet 空间（特别是每个 Banach 空间）都是桶装的。*这源自 Baire 的定理（GT，IX, § 5, No. 3，第 1）。

#### 命题 3 {#evt-iii-s4-prop-3 .statement tag=07O6}

— *令$(F_i)_{i \in I}$为桶状空间族，对于每个$i \in I$，令$f_i$为从$F_i$到向量空间E的线性映射。空间E具有最细的局部凸拓扑，其中$f_i$是连续的（II、p. 27、道具 5），是桶装空间。*

设T为E中的桶。由于$f_i$是连续的，因此$f_i^{-1}(T)$是$F_i$中的凸、平衡、封闭且可吸收的集合；其他字，$F_i$一桶；由于$F_i$是桶装的，对于所有$i \in I$，$f_i^{-1}(T)$是$F_i$中0的邻域。这意味着 T 是 E 中 0 的邻域（II，p. 27，道具 5）。

#### 推论 1 {#evt-iii-s4-prop-3-cor-1 .statement tag=07O7}

— *桶装空间的每个商空间都是桶装。*

#### 推论 2 {#evt-iii-s4-prop-3-cor-2 .statement tag=07O8}

— *令$(E_i)_{i \in I}$为局部凸空间族，并令E为该族的拓扑直和。为了使 E 被桶装，每个 $E_i$ 被桶装是必要且充分的。*

凭借 prop，条件显然是足够的。 3； cor. 这也是必要的。 1，因为每个$E_i$同构于E的商空间（II，p. 31，道具8）。

#### 推论 3 {#evt-iii-s4-prop-3-cor-3 .statement tag=07O9}

— *桶装空间的每个感应极限都是桶装空间。*

稍后我们将证明（IV，p. 14，推论）桶装空间的每一个乘积都是桶装的。

### 2.巴纳赫斯坦豪斯定理

#### 定理 1 {#evt-iii-s4-thm-1 .statement tag=07OA}

— *令 E 为桶状空间，F 为局部凸空间。 $\mathscr{L}(E; F)$ 的每个简单有界子集 H 都是等连续的。*

设 $p$ 为 F 上的连续半范数；让$q = \sup_{u \in H} (p \circ u)$。由于 H 是简单有界的，因此对于所有 $x \in E$，我们有 $q(x) < +\infty$，并且 $q$ 是下半连续半范数，是连续半范数的有限上包络。由于 E 是桶形的，$q$ 是连续半范数，因此 H 是等连续的。

#### 推论 1 {#evt-iii-s4-thm-1-cor-1 .statement tag=07OB}

— *设E和F是两个Banach空间，H是从E到F的连续线性映射族；如果对于所有 $x \in E$，我们有 $\sup_{u \in H} \|u(x)\| < +\infty$，那么我们也有 $\sup_{u \in H} \|u\| < +\infty$。*

事实上，假设表示H是简单有界的并且结论是它是等连续的。在加法中，每个 Banach 空间都经过桶装（III，p. 25）。

#### 推论 2 {#evt-iii-s4-thm-1-cor-2 .statement tag=07OC}

—（巴纳赫-斯坦豪斯定理）。 — *令 E 为桶状空间，F 为局部凸 Hausdorff 空间，并令 $(u_n)$ 为从 E 到 F 的连续线性映射* 的序列，它简单地收敛到从 E 到 F 的映射 u。然后 $u \in \mathscr{L}(E; F)$ 和 $(u_n)$ 在每个点上均匀地收敛到 u E 的预紧子集。

事实上，序列$(u_n)$是简单有界的，因此是等连续的，并且推论来自cor。的道具。 III、p. 18 中的 5 个。

#### 注 1 {#evt-iii-s4-n2-rem-1 .statement tag=07OD}

性质用cor表示。 2并不意味着E是桶装的：我们稍后会看到Fréchet 空间的强对偶拥有这个性质，但不一定是桶装的（IV，p. 23，对应于道具2和p. 58，执行。

#### 注 2 {#evt-iii-s4-n2-rem-2 .statement tag=07OE}

设E和F是两个Banach空间，以及从E到F的连续线性映射的$(u_n)$序列，使得$\sup \|u_n\| = + \infty$。那么所有$x \in E$的集合X使得$\sup \|u_n(x)\| = + \infty$在E中是稠密的并且是E中开集合的序列的交。对于，令$X_k$表示所有$x \in E$的集合使得$\sup \|u_n(x)\| > k$（对于 k 整数 $> 0$）。每个$X_k$都是开放的，X是$X_k$的交。由于 E 是 Baire 空间，因此足以证明每个 $X_k$ 在 E 中都是稠密的。但是，如果 $X_k$ 包含的补集是一个非空开集合 U，则对于 $x \in U - U$，我们将有 $\|u_n(x)\| \leq 2k$，并且，因为 $U - U$ 是邻域为0，我们将有$\sup \|u_n\| < + \infty$。

#### 推论 3 {#evt-iii-s4-thm-1-cor-3 .statement tag=07OF}

— *令 E 为桶状空间，F 为局部凸 Hausdorff 空间，$\Phi$ $\mathscr{L}(E; F)$ 上的滤波器，它简单地收敛于 E 到映射 u，从 E 到 F。如果 $\Phi$ 包含为 $\mathscr{L}(E; F)$ 的简单有界子集，或者如果$\Phi$有一个可数基，那么u是从E到F的连续线性映射，并且$\Phi$在E的每个预紧子集上一致收敛到u。*

首先假设 $\Phi$ 包含 a 简单有界集合 H ；由于 H 是等连续的 (th. 1)，因此推论来自于 prop 的推论。 5（III，p. 18）。 If $\Phi$ has a countable base, every elementary filter $\Psi$ associated with a sequence $u_n$ (GT, I, § 6, No. 8) which is finer than $\Phi$ is then simply convergent to u in E and it follows from cor. 2 that u is a continuous linear mapping from E into F, and that $\Psi$ converges to u for the topology of uniform convergence on precompact subsets of E. 因而，对于$\Phi$同样成立，因为后者是基本滤波器的交，每个更细比$\Phi$（GT，I, § 6, No. 8）。

我们观察到，$\mathscr{L}(E; F)$上简单收敛且具有可数基的滤波器不一定是包含简单有界的集合：要看到这一点，请考虑当F的拓扑可度量时，$\mathscr{L}(K; F)$中0的邻域滤波器的例，但不能由单个范数定义。

#### 例 {#evt-iii-s4-n2-exa-1 .statement tag=07OG}

— 令 E 为连续复形函数的 Banach 空间（超过 $\mathbf{C}$）由……组成，其中 $\mathbf{R}$ 具有周期 1，且范数 $\|f\| = \sup_x |f(x)|$。

对于每个整数$n \in \mathbf{Z}$和每个函数$f \in E$，令$c_n(f) = \int_0^1 f(x) e^{-2i\pi nx} dx$（$n$-$f$的第一个傅立叶系数）；每个映射$f \mapsto c_n(f)$都是E上的连续线性形式。令$(\alpha_n)$为复数的序列，这样，对于每个函数$f \in E$，与一般项$\alpha_n c_n(f) + \alpha_{-n} c_{-n}(f)$的级数是收敛的。在这些条件下，映射$u : f \mapsto \alpha_0 c_0(f) + \sum_{n \geq 1} [\alpha_n c_n(f) + \alpha_{-n} c_{-n}(f)]$是E上的连续线性形式； \* 在其他字中，$[0, 1]$上存在一个测度$\mu$，使得$u(f) = \int f(x) d\mu(x)$对于每个函数$f \in E$，$\alpha_n$是$\mu$的第$n$个傅里叶系数。*事实上，对于每个整数 $m > 0$、映射 $f \mapsto \sum_{k = -m}^m \alpha_k c_k(f)$ 是 E 上的连续线性形式 $u_m$，并且对于所有 $f \in E$，序列 $(u_m(f))$ 通过假设收敛到 $u(f)$。 断言然后是 Banach-Steinhaus 定理，因为 E 是桶装的。

#### 推论 4 {#evt-iii-s4-thm-1-cor-4 .statement tag=07OH}

— *令 E 和 F 为两个局部凸空间，$\mathfrak{S}$ 有界子集的 E 由……组成的覆盖。如果 E 是桶装的且 F 是 Hausdorff 且准完备的，则空间 $\mathscr{L}_{\mathfrak{S}}(E; F)$ 是 Hausdorff 且准完备。*

事实上，$\mathscr{L}_{\mathfrak{S}}(E; F)$的每个有界和闭子集都是简单有界的（因为$\mathfrak{S}$是E的覆盖），因此是等连续的（III，p. 25，第1），因此是$\mathscr{L}_{\mathfrak{S}}(E; F)$的完整子空间，因为prop。 11（III，p. 22）。

#### 推论 5 {#evt-iii-s4-thm-1-cor-5 .statement tag=07OI}

— *桶装空间的强对偶和弱对偶是准完整的。*

### 3. 有界子集 of $\mathscr{L}(E; F)$（准完全情况）

#### 定理 2 {#evt-iii-s4-thm-2 .statement tag=07OJ}

— *设 E 为局部凸 Hausdorff 空间，F 为局部凸空间和 $\mathfrak{S}$ E 的闭、凸、平衡、有界和半完备子集族（III，p. 7）。 $\mathscr{L}(E; F)$ 的每个简单有界子集 H 都针对 $\mathfrak{S}$ 拓扑有界。*

让$A \in \mathfrak{S}$。 空间 $E_A$ 则为 Banach 空间（III、p. 8，推论），因此是桶装的。另一方面，$\mathscr{L}(E_A; F)$中H的典范像是简单有界的，因此是等连续的（III，p. 25，th.1）。因而，$u \in H$和$x \in A$的所有$u(x)$中的集合在F中有界，这证明H对于$\mathfrak{S}$拓扑是有界的。

#### 推论 1 {#evt-iii-s4-thm-2-cor-1 .statement tag=07OK}

— *设 E 为局部凸 Hausdorff 空间，F 为局部凸空间，$\mathfrak{S}$ E 的有界子集系列。如果 E 是半完备的，则 $\mathscr{L}(E; F)$ 的每个简单有界子集都有界$\mathfrak{S}$-拓扑。*

应用th就足够了。 2、 $\mathfrak{S}$ 的之后替换集合由其封闭、凸、平衡的包络线组成，因为这不是变换 $\mathfrak{S}$ 拓扑。

当 E 是半完备的（对于例准完备）时，我们可以讨论$\mathscr{L}(E; F)$的*有界子集*，而无需指定$\mathfrak{S}$拓扑，因为只要$\mathfrak{S}$是E的覆盖，这些对于所有$\mathfrak{S}$拓扑都是相同的。

#### 推论 2 {#evt-iii-s4-thm-2-cor-2 .statement tag=07OL}

— *每一个半完整的出生学空间都是桶装的。*

此类空间的对偶的每个单有界子集都是强有界的（cor. 1），因此等连续（III，p. 22，道具 10）。

#### 推论 3 {#evt-iii-s4-thm-2-cor-3 .statement tag=07OM}

— *令 E 为局部凸空间。 E 的每个子集的边界为 $\sigma(E, E')$ 都是有界的。*

设 A 为 E 的子集。说 A 的边界为 $\sigma(E, E')$ 意味着 E 上的每个连续线性形式都边界为 A ； 说 A 有界意味着 E 上的每个连续半范数都在 A 上有界。令 N 为 E 中 0 的闭包，以及从 E 到 E/N 的 $\pi$ 典范映射。 E 上的连续线性形式是形式 $f \circ \pi$ 与 $f \in (E/N)'$ 的映射，我们有一个类似的 E 上的连续半范数刻画。 替换 E 由 E/N 和 A 由 $\pi(A)$ 我们可以因此极限我们自己的情况是 E 是 Hausdorff。

设$\mathfrak{S}$为$E'$等连续子集的集合；当$E'$被分配拓扑$\sigma(E', E)$时，$E$可以用$(E')_{\mathfrak{S}}'$来识别（III，p. 19，cor.1）。 $E'$ 的每个闭等连续子集对于 $\sigma(E', E)$ 都是紧致的（III，p. 17，cor. 2），因此对于 $\sigma(E', E)$ 来说是完备的。现在应用 th 就足够了。 2.

### 习题 {#evt-iii-s4-exercises}

§ 4](exercises/s4/)参见[习题。
