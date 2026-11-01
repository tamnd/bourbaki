---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 9
section_title: Commutators, centralizers and normalizers in a Lie group
lang: zh
source: lie-i-iii
book_pages: 342-359, 397-409
pdf_pages: 0360-0377, 0415-0427
extraction: ocr
subsections:
    - "no": 1
      title: COMMUTATORS IN A TOPOLOGICAL GROUP
      page: 342
      pdf_page: 360
    - "no": 2
      title: COMMUTATORS IN A LIE GROUP
      page: 343
      pdf_page: 361
    - "no": 3
      title: CENTRALIZERS
      page: 346
      pdf_page: 364
    - "no": 4
      title: NORMALIZERS
      page: 347
      pdf_page: 365
    - "no": 5
      title: NILPOTENT LIE GROUPS
      page: 347
      pdf_page: 365
    - "no": 6
      title: SOLVABLE LIE GROUPS
      page: 352
      pdf_page: 370
    - "no": 7
      title: RADICAL OF A LIE GROUP
      page: 354
      pdf_page: 372
    - "no": 8
      title: SEMI-SIMPLE LIE GROUPS
      page: 355
      pdf_page: 373
statements: 54
exercises: 42
content_sha256: be58a3328d27f2be71db1665a8a0ac0e32d3a57d60ecb7bbac29c2914abee2d6
translated_from: content/en/lie/III/09_s9_commutators_centralizers_and.md
translation_method: google
source_content_sha256: 5160b395f31c39ef9f1ad5f95ebd21b2c6f9dc63a62483b154ec6113d26d8afa
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 302d57ed5eb4966cc6022e3de63cd88fef4ec238a58ddf43387e1bc07e90ed66
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 9。 换位子，李群的集中器和标准化器

在本段中，K 假设为特征零。

### 1.拓扑中的换位子群

令 G 为拓扑群。我们定义群$\overline{D^0G}, \overline{D^1G}, \overline{D^2G}, \ldots$和$\overline{C^1G}, \overline{C^2G}, \overline{C^3G}, \ldots$由公式

$$
\begin{aligned}
\overline{D^0G} &= G, & \overline{D^{i+1}G} &= (\overline{D^iG}, \overline{D^iG}) \\
\overline{C^1G} &= G, & \overline{C^{i+1}G} &= (G, \overline{C^iG}).
\end{aligned}
$$

#### 命题 1 {#lie-iii-s9-prop-1 .statement tag=0AII}

*设G是G的拓扑群，A和B子群。那么*$(\overline{A}, \overline{B}) = (\overline{A}, \overline{B}), \overline{D^iA} = \overline{D^iA}, \overline{C^iA} = \overline{C^iA}$。

令$\phi$为$G \times G$在G中的连续映射$(x, y) \mapsto x^{-1}y^{-1}xy$。然后$\phi(A \times B) \subset (A, B)$，因此$\phi(\overline{A} \times \overline{B}) \subset (\overline{A}, \overline{B})$，因此

$$
(\overline{A}, \overline{B}) \subset (\overline{A}, \overline{B});
$$

相反的包含是明显的，因此 $(\overline{A}, \overline{B}) = (\overline{A}, \overline{B})$。显然$\overline{D^0A} = \overline{D^0A}$；假设等式 $\overline{D^iA} = \overline{D^iA}$，则

$$
\overline{D^{i+1}A} = (\overline{D^iA}, \overline{D^iA}) = (\overline{D^iA}, \overline{D^iA}) = (\overline{D^iA}, \overline{D^iA}) = \overline{D^{i+1}A}
$$

因此对于所有 $i$ 来说，$\overline{D^iA} = \overline{D^iA}$。 公式 $\overline{C^iA} = \overline{C^iA}$ 的证明类似。

#### 推论 1 {#lie-iii-s9-prop-1-cor-1 .statement tag=0AIJ}

*如果 G 是 Hausdorff，则以下条件等价*：
(i) *G 是可解的*（分别是*幂零的*）；
(ii) $\overline{D^iG} = \{e\}$（分别为 $\overline{C^iG} = \{e\}$）*对于足够大* $i$。
$D^iG \subset \overline{D^iG}, C^iG \subset \overline{C^iG}$，因此 (ii) $\Rightarrow$ (i)。 $\{e\} = \{\overline{e}\}$，因此 (i) $\Rightarrow$ (ii) 命题 1。

#### 推论 2 {#lie-iii-s9-prop-1-cor-2 .statement tag=0AIK}

*设 G 是 G 的豪斯多夫拓扑群和 A 子群。对于 A 可解*（分别为*幂零的、可交换*，*必要且充分* $\overline{A}$ *如此*。

§ 9.2

这紧接着命题 1。

#### 命题 2 {#lie-iii-s9-prop-2 .statement tag=0AIL}

设 G 为拓扑群，G 的 A 和 B 子群。如果 A 连通，则 (A, B) 连通。

对于 B 中的固定 y，(x, y) 的集合 M_y 与 x ∈ A 是连通的（对于 A 到 G 的映射 x ↦ (x, y) 是连续的）。 e ∈ M_y，因此 M_y 的并 R 与 y ∈ B 是相连的。但(A, B)是R生成的G的子群，从而命题。

### 2.换位子在李群

#### 命题 3 {#lie-iii-s9-prop-3 .statement tag=0AIM}

设 G 为 G 的有限维李群，H_1 和 H_2 子群。设 h_1、h_2 和 h 分别为在 e 处与 H_1、H_2 和 (H_1, H_2) 相切的李子代数。那么 [h_1, h_2] ⊂ h。

令a ∈ h_1, b ∈ h_2。 K 中存在 0 的开邻域 I，并且解析 I 的映射 f_1, f_2 到 G 中，使得

$$
f_1(0) = f_2(0) = e, \quad f_1(I) \subset H_1, \quad f_2(I) \subset H_2,
$$
$$
(T_0 f_1)1 = a, \quad (T_0 f_2)1 = b.
$$

我们写
$$
f(\lambda, \mu) = (f_1(\lambda), f_2(\mu)) \in (H_1, H_2) \quad \text{for } \lambda, \mu \text{ in I}.
$$

我们通过映射 e 到 0 的图表，将 G 中 e 的开邻域与 K' 的开子集认同映射 e 到 0。然后L(G) 被识别为 K'。将 f(\lambda, \mu) 的 § 5, no. 2, 命题 1, 展开作为关于原点的级数积分为
$$
f(\lambda, \mu) = \lambda \mu [a, b] + \sum_{i \geq 1, j \geq 1, i+j \geq 2} \lambda^i \mu^j a_{ij}
$$
其中 a_{ij} ∈ K'（f(\lambda, \mu) 的展开中 \lambda^i 中的项和 \mu^j 为零，因为 f(\lambda, 0) = f(0, \mu) = 0）。我们修复I中的\mu。令 lambda 趋于 0，我们看到
$$
\mu [a, b] + \sum_{j \geq 2} \mu^j a_{1j} \in h.
$$
由于这对于所有 \mu ∈ I 都是正确的，因此 [a, b] ∈ h。

#### 注 {#lie-iii-s9-n2-rem-1 .statement tag=0AIN}

即使 H_1 和 H_2 连接为 G 的 Lie 子群，[h_1, h_2] 生成的 L(G) 的 Lie 子代数通常与 h 不同。

#### 命题 4 {#lie-iii-s9-prop-4 .statement tag=0AIO}

令 G 为有限维实数或复数李群。令 A, B, C 为 G 的积分子群，使得 [L(A), L(C)] ⊂ L(C) 且
$$
[L(B), L(C)] \subset L(C).
$$
如果 [L(A), L(B)] ⊂ L(C)，则 (A, B) ⊂ C。如果 [L(A), L(B)] = L(C)，则 (A, B) = C。

假设$[L(A), L(B)] \subset L(C)$。 和$L(A) + L(B) + L(C)$是$L(G)$的谎言子代数。通过考虑 $G$ 的积分子群与李代数 $L(A) + L(B) + L(C)$，问题被简化为以下情况：

$$
L(A) + L(B) + L(C) = L(G)
$$

且$G$已连接。那么$L(C)$就是$L(G)$的理想。首先假设 $G$ 是单连通的。那么 $C$ 就是 $G$ (§ 6, no. 6, 命题 14) 的正常谎言子群。令$\phi$为$G$到$G/C$的规范态射。然后

$$
[L(\phi)(L(A)), L(\phi)(L(B))] = \{0\}
$$

因此 $\phi(A)$ 和 $\phi(B)$ 乘坐 Hausdorff 公式通勤；因此$(A, B) \subset C$。在一般情况下，令$G'$为$G$和$A', B', C'$的全覆盖，$G'$的积分子群使得$L(A') = L(A), L(B') = L(B), L(C') = L(C)$。那么$(A', B') \subset C'$和$A, B, C$分别是$G$、从而$(A, B) \subset C$中$A', B', C'$的典范像。另一方面，$(A, B)$是$G$的积分子群（§ 6, no. 2，命题4的推论）及其李代数包含$[L(A), L(B)]$（命题3）的基础集合。如果

$$
[L(A), L(B)] = L(C),
$$

然后$(A, B) \supset C$，从而$(A, B) = C$。

#### 推论 {#lie-iii-s9-n2-cor-1 .statement tag=0AIP}

*设 G 为与李代数 g 连接的有限维实数或复数李群。 子群 $D^iG$（分别为 $C^iG$）是子群与李代数 $D^i\mathfrak{g}$（分别为 $C^i\mathfrak{g}$）的积分。如果 G 是单连通的，则它们是谎言子群。*

第一个断言是从命题 4 到 $i$ 上的归纳之后的。第二个紧接第一个和§ 6, no. 6、命题 14。

#### 命题 5 {#lie-iii-s9-prop-5 .statement tag=0AIQ}

*设 G 为有限维实数或复数李群，A 为 G 的积分子群。然后为 $DA = DA$。特别是，A 是 $\overline{A}$ 的正规子群，并且 $\overline{A}/A$ 是可交换的。*

让$a = L(A)$。令 $G_1$ 为 $g \in G$ 的集合，使得

$$(\mathrm{Ad}\, g)x \equiv x \pmod{\mathscr{D}a} \quad \text{for all } x \in a.$$

那么$G_1$是$G$的闭子群。如果$y \in a$，则$\exp y \in G_1$，通过§ 6, no. 4，推论3 (ii) 到命题 10。因此$G_1$包含$A$，因此$\overline{A}$。因此，对于$g \in \overline{A}$，$L(\mathrm{Int}\, g)$使$a$稳定，因此$\mathrm{Int}\, g$使$A$稳定；更准确地说，$L(\mathrm{Int}\, g)$定义是$a/\mathscr{D}a$的恒等式自同构，因此$\mathrm{Int}\, g$定义是$A/DA$的恒等式自同构。这就证明了$(\overline{A}, A) \subset DA$。 实李群结构在$G$上，$\overline{A}$是谎言子群（§ 8, no. 2，定理2）；令$b$为其李代数。令 $G_2$ 为 $g \in G$ 的集合，使得

$$(\mathrm{Ad}\, g)x \equiv x \pmod{\mathscr{D}a} \quad \text{for all } x \in b.$$

由上可知，$G_2 \supseteq A$，因此$G_2 \supseteq \overline{A}$。因此，对于 $g \in \overline{A}$，Int $g$ 使 DA 保持稳定，并且定义 $\overline{A}/DA$ 的恒等式自同构。因此$DA \supseteq D\overline{A}$。

#### 命题 6 {#lie-iii-s9-prop-6 .statement tag=0AIR}

*假设 K 是超量度的。令 G 为有限维李群。设 A, B, C 为 G 的谎言子群，使得 $[L(A), L(C)] \subset L(C)$, $[L(B), L(C)] \subset L(C)$。若$[L(A), L(B)] \subset L(C)$，则存在A、B的开子群A'、B'使得$(A', B') \subset C$。如果$[L(A), L(B)] \subset L(C)$，则存在A、B、C的开子群 A'、B'、C'，使得$(A', B') = C'$。*

假设$[L(A), L(B)] \subset L(C)$。如命题 4 的证明所示，问题约化对于$L(C)$ 是$L(G)$ 的理想的情况。然后，通过替换 G 通过开子群，约化到C 在 G 中正常的情况（$§ 7$，no. 1，命题 2）。令 $\phi$ 为 G 在 $G/C$ 上的规范态射。然后
$$
[L(\phi)(L(A)), L(\phi)(L(B))] = \{0\}.
$$
由豪斯多夫公式，存在A、B的开子群A'、B'，使得$\phi(A')$和$\phi(B')$通勤，从而$(A', B') \subset C$。进一步假设
$$
[L(A), L(B)] = L(C).
$$
到命题 3 时，谎言子代数在 $e$ 包含 $L(C)$ 与 $(A', B')$ 相切。因此$(A', B')$包含是G的谎言子群胚芽与李代数$L(C)$。因此$(A', B')$是C的开子群。

#### 推论{#lie-iii-s9-n2-cor-2 .statement tag=0AIS}

*假设 K 是超量度的。令 G 为有限维李群且李代数 g。存在 G 的开子群 $G_0$，使得对于所有 $i$，$D^iG_0$（分别为 $C^iG_0$）是 G 的谎言子群，其中李代数 $\mathscr{D}^ig$（分别为 $\mathscr{C}^ig$）。*

(a) 通过命题 3 归纳应用，对于 G 的每个开路子群 $G_1$ 以及所有 $i$、$D^iG_1$ 包含，G 的谎言子群芽与李代数 $\mathscr{D}^ig$。

(b) 令$G'$为G的开子群，使得对于$i \leq n$，$D^iG'$是G的谎言子群且李代数$\mathscr{D}^ig$。 到命题 6，存在$D^nG'$的开子群$H_1, H_2$，使得$(H_1, H_2)$是一个谎言子群与李代数$\mathscr{D}^{n+1}g$。 令$G''$是$G'$的开子群，对于$D^nG'' \subset H_1 \cap H_2$来说足够小。 然后$D^{n+1}G'' \subset (H_1, H_2)$。 The relations
$$
D^0G'' \subset D^0G', D^1G'' \subset D^1G', \ldots, D^nG'' \subset D^nG', D^{n+1}G'' \subset (H_1, H_2)
$$
prove, using (a), that $D^iG''$ is, for $i \leq n + 1$, a Lie subgroup of G with Lie algebra $\mathscr{D}^ig$.

(c) 存在整数$p$使得$\mathscr{D}^pg = \mathscr{D}^{p+1}g = \cdots$。由上可知，存在 G 的开子群 $G_0$，使得 $D^iG_0$ 对于 $i \leq p$ 来说是 G 的一个谎言子群与李代数 $\mathscr{D}^ig$。但是，根据 (a)，自 $D^pG_0 \supset D^iG_0$ 对于 $i > p$ 以来，相同的断言对于$i > p$ 仍然成立。

(d) $C^i$ 的论证类似。

### 3. 集中器

回想一下，如果 $(x, y) = e$、$(\mathrm{Int}\, x)y = y$、或 $(\mathrm{Int}\, y)x = x$，则群中的两个元素 $x, y$ 被称为可置换；如果 $[a, b] = 0$、$(\mathrm{ad}\, a).b = 0$、$(\mathrm{ad}\, b).a = 0$，则李代数中的两个元素 $a, b$ 被称为可置换。令$G$为李群、$x \in G$、$a \in \mathbf{L}(G)$；如果$(\mathrm{Ad}\, x).a = a$，即如果$\mathbf{T}(G)$中有$xa = ax$，则$x$和$a$称为可置换。

设$G$为李群，$g$为李代数，$G$为$A$子集，$a$子集为$g$。让$Z_G(A)$（或$Z_G(a)$）表示$G$的元素的集合，它们可以与$A$（或$a$）的所有元素进行置换。这是 $G$ 的闭合子群。让$\mathfrak{z}_g(A)$（或$\mathfrak{z}_g(a)$）表示$g$的元素的集合，它们可以与$A$（或$a$）的所有元素进行置换。这是 $g$ 的封闭谎言子代数。

#### 命题 7 {#lie-iii-s9-prop-7 .statement tag=0AIT}

*令$G$为有限维李群，$g$为李代数，$a$为$g$的子集。那么 $Z_G(a)$ 是 $G$ 的谎言子群与李代数 $\mathfrak{z}_g(a)$。*

这是从§ 3、命题 44 和推论 2 到命题 39 得出的。

#### 命题 8 {#lie-iii-s9-prop-8 .statement tag=0AIU}

*令$G$为有限维实数或复数李群，$g$为李代数，$A$子集为$G$。那么 $Z_G(A)$ 是 $G$ 的谎言子群与李代数 $\mathfrak{z}_g(A)$。*

假设 $A$ 由单个点 $a$ 组成。则$Z_G(A)$为$\mathrm{Int}\, a$固定点集合；因此，$Z_G(A)$是$G$的谎言子群，$\mathbf{L}(Z_G(A))$是$\mathrm{Ad}\, a$的固定点的集合，即$\mathfrak{z}_g(A)$（§ 3, no. 8，推论1到命题29）。一般情况通过§ 6, no. 2，推论3到命题1。

#### 命题 9 {#lie-iii-s9-prop-9 .statement tag=0AIV}

*令$G$为有限维实数或复数李群，$g$为李代数，$A$为$G$和$a = \mathbf{L}(A)$的积分子群。那么$Z_G(A) = Z_G(a)$、$\mathfrak{z}_g(A) = \mathfrak{z}_g(a)$和$Z_G(A)$是$G$的谎言子群和李代数$\mathfrak{z}_g(a)$。*

让$x \in G$。然后
$$
x \in Z_G(A) \iff A \subset Z_G(\{x\}) \\
\iff a \subset \mathbf{L}(Z_G(\{x\})) \quad (\text{§ 6, Corollary 2 to Proposition 3}) \\
\iff a \subset \mathfrak{z}_g(\{x\}) \quad (\text{Proposition 8}) \\
\iff x \in Z_G(a)
$$
因此$Z_G(A) = Z_G(a)$。让$u \in g$。然后
$$
u \in \mathfrak{z}_g(A) \iff A \subset Z_G(\{u\}) \\
\iff a \subset \mathbf{L}(Z_G(\{u\})) \quad (\text{§ 6, Corollary 2 to Proposition 3}) \\
\iff a \subset \mathfrak{z}_g(\{u\}) \quad (\text{Proposition 7}) \\
\iff u \in \mathfrak{z}_g(a)
$$
因此$\mathfrak{z}_g(A) = \mathfrak{z}_g(a)$。然后从命题 7 或命题 8 得出最后一个断言。

### 4. 标准化器

设G为李群，$g$其李代数，G的A子集和$g$的$a$子集。在这个截面中，$N_G(A)$将表示$g \in G$的集合，使得$gAg^{-1} = A$。它是 G 的子群，如果 A 是闭的，则 G 也是闭的。 $n_g(a)$将表示$x \in g$的集合，使得$[x, a] \subset a$（cf.章I, § 1, no. 4）。是$g$的子代数，如果$a$闭，则闭。 $N_g(a)$将表示$g \in G$的集合，使得$gag^{-1} = a$。

#### 命题 10 {#lie-iii-s9-prop-10 .statement tag=0AIW}

*设 G 为有限维李群，g 为李代数，g 为向量子空间。那么 $N_G(a)$ 是 G 的谎言子群与李代数 $n_g(a)$。*这是从 § 3、命题 44 和推论 1 到命题 39 得出的。

#### 命题 11 {#lie-iii-s9-prop-11 .statement tag=0AIX}

*设 G 为有限维实数或复数李群，g 为李代数，A 为 G 和 $a = L(A)$ 的积分子群。那么 $N_G(A) = N_G(a)$ 和 $N_G(A)$ 是 G 包含 $\overline{A}$ 的谎言子群，其中李代数 $n_g(a)$。* 等式 $N_G(A) = N_G(a)$ 由 § 6, no. 2 推出，推论 2 为命题 3. 到命题 10，$N_G(A)$ 就是 G 的谎言子群和李代数 $n_g(a)$。因此 $N_G(A)$ 是闭合的。如$N_G(A) \supset A$、$N_G(A) \supset \overline{A}$。

#### 推论{#lie-iii-s9-n4-cor-1 .statement tag=0AIY}

*如果 $a = n_g(a)$，A 是 G 的谎言子群，并且是 $N_G(A)$ 的恒等分量。* 该恒等分量是一个谎言子群，其中李代数 $n_g(a)$ (命题 11)，因此等于 A § 6, no. 2， 定理 2 (i)。

### 5. NILPOTENT 李群

#### 命题 12 {#lie-iii-s9-prop-12 .statement tag=0AIZ}

*设 G 为有限维李群。为了使$L(G)$幂零，G有一个幂零开子群是充分必要的。*假设G有一个幂零开子群$G_0$。根据命题 4 和 6、no. 2、$C^iL(G_0) = \{0\}$ 的推论，足够大 $i$。因此$L(G_0) = L(G)$是幂零的。

假设 $L(G)$ 幂零。如果 $K = \mathbf{R}$ 或 $\mathbf{C}$，G 的恒等分量 $G_0$ 是幂零的，命题 4、no. 2 的推论，$G_0$ 在 G 中是开的。如果 K 是超度量的，命题 6、no. 2 的推论证明存在打开 G 的子群 $G_1$，G 中 e 的整数 $i > 0$ 和邻域 V，使得 $C^iG_1 \cap V = \{e\}$。那么，如果$G_0$是$G_1$、$C^iG_0 \subset V$足够小的子群，因此$C^iG_0 = \{e\}$和$G_0$是幂零的。

设$g$为幂零李代数。 Hausdorff 级数 $H(X, Y)$ 相应的到 $g$ 只有非零项的有限数并且我们知道 (章 II, § 6, no. 5, *注 3*) 律合成$(x, y) \mapsto H(x, y)$定义群结构$g$。进一步假设 $g$ 是完备且规范的。显然律 H 是连续多项式（*可微且解析流形*，R，附录）。因此，$g$与律 H一起，是李群 G，据说与*$g$*相关。 § 4, no. 2、引理 2 和 3、$L(G) = g$。 $g$的恒等映射$\phi$到$G$是$G$的指数映射，使得$\phi(\lambda x)\phi(\lambda'x) = \phi((\lambda + \lambda')x)$对于所有$x \in g, \lambda \in K, \lambda' \in K$。 $g$的每个谎言子代数$\mathfrak{h}$承认拓扑补充都是$G$和$L(H) = \mathfrak{h}$的谎言子群$H$。

#### 命题 13 {#lie-iii-s9-prop-13 .statement tag=0AJ0}

*令$G$为$\mathbf{R}$或$\mathbf{C}$上的有限维单连通幂零李群。*

(i) $\exp_G$ 是李群中的同构，与$L(G)$ 关联到$G$。

(ii) *$G$ 的每个积分子群都是 $G$ 的单连通李子子群。*

设 $g = L(G)$，它是幂零的 (命题 12)。由于$\mathbf{R}$或$\mathbf{C}$上的两个单连通李群具有相同的李代数，它们是同构的（$§ 6$，no. 3，定理 3 (ii)），当$G$为群时，只需证明命题即可与$g$相关。然后（i）和（ii）从所说的之前命题得出。

#### 命题 14 {#lie-iii-s9-prop-14 .statement tag=0AJ1}

*令 $G$ 为在 $\mathbf{R}$ 或 $\mathbf{C}$ 上连接的有限维李群。*

(i) *如果 $G$ 幂零，$\exp_G$ 是 étale 和满射。*

(ii) *如果 $K = \mathbf{C}$ 和 $\exp_G$ 是 étale，则 $G$ 幂零。*

令$G'$为$G$的通用覆盖空间。令$\phi$为$G'$到$G$的规范态射。然后 $\exp_G = \phi \circ \exp_{G'}$ ($§ 6$, no. 4, 命题 10)，因此从命题 13 (i) 得出 (i)。

如果$K = \mathbf{C}$和$\exp$是étale，那么，对于所有$x \in L(G)$和$x$，没有特征值、属于到$2i\pi(\mathbf{Z} - \{0\})$（$§ 6$、no. 4，命题12的推论）。 应用到$\lambda x$，其中$\lambda$变化到$\mathbf{C}$，因此$\mathrm{ad}\, x$的所有特征值都是零，因此$\mathrm{ad}\, x$是幂零的。因此$L(G)$是幂零的（章I，$§ 4$，推论1到定理1），因此$G$是幂零的（命题12）。

#### 命题 15 {#lie-iii-s9-prop-15 .statement tag=0AJ2}

*设$G$是$\mathbf{R}$或$\mathbf{C}$上的有限维连通幂零李群，并且$A$是$G$的积分子群。那么$Z_G(A)$就是$G$与李代数$\mathfrak{z}_G(L(A))$的连通谎言子群。*

通过命题 9 of no. 3就足以证明$Z_G(A)$是连通的。让$g \in Z_G(A)$。存在$x \in L(G)$使得$g = \exp x$(命题14)。然后 $\mathrm{Ad}\, g|L(A) = 1$ (no. 3, 命题 9)，因此对于所有 $n \in \mathbf{Z}$ 是 $\mathrm{Ad}\, g^n|L(A) = 1$，对于所有 $n \in \mathbf{Z}$ 是 $\exp(\mathrm{ad}\, nx)|L(A) = 1$。作为映射

$$
\lambda \mapsto \exp(\mathrm{ad}\, \lambda x)|L(A)
$$

$K$ 到 $\mathscr{L}(L(A), L(G))$ 的乘积是多项式，$\exp(\mathrm{ad}\, \lambda x)|L(A) = 1$ 对于所有 $\lambda \in K$，即 $\exp(\lambda x) \in Z_G(A)$ 对于所有 $\lambda \in K$。

#### 命题 16 {#lie-iii-s9-prop-16 .statement tag=0AJ3}

*设$G$是$\mathbf{R}$或$\mathbf{C}$上的有限维幂零李群，并且$A$是$G$的积分子群，与$G$不同。那么$N_G(A)$是$G$的连通谎言子群，与$A$不同。*

$N_G(A) \neq A$（代数、章I, § 6，推论 1 至命题 8）。通过no. 4的命题11，我们只需证明$N_G(A)$是连通的。让$g \in N_G(A)$。存在$x \in L(G)$使得$g = \exp x$(命题14)。令$E$为$u \in \mathscr{L}(L(G))$的$\mathscr{L}(L(G))$由……组成之向量子空间，使得$u(L(A)) \subset L(A)$。然后$\mathrm{Ad}\, g^n \in E$，因此对于所有$n \in \mathbf{Z}$，$\exp(\mathrm{ad}\, nx) \in E$。因此，对于所有$\lambda \in K$，$\exp(\mathrm{ad}\, \lambda x) \in E$，即对于所有$\lambda \in K$，$\exp(\lambda x) \in N_G(A)$。

#### 命题 17 {#lie-iii-s9-prop-17 .statement tag=0AJ4}

*设$g$是$g$理想的$K$和$(g_0, g_1, \ldots, g_n)$递减序列的有限维幂零李代数，使得$g_0 = g, g_n = \{0\}$和$[g, g_i] \subset g_{i+1}$对于$0 \leq i < n$。令$a_1, a_2, \ldots, a_p$为$g$的向量子空间，使得每个$g_i$是其交与$a_j$的直和。让 $g$ 被赋予合成 $H$ 的 Hausdorff 律。令 $\phi$ 为映射*

$$
(x_1, x_2, \ldots, x_p) \mapsto x_1 \mathbf{H} x_2 \mathbf{H} \cdots \mathbf{H} x_p
$$

$a_1 \times a_2 \times \cdots \times a_p$ 变为 $g$。

(i) $\phi$ 是 $a_1 \times a_2 \times \cdots \times a_p$ 的双射到$g$；
(ii) $\phi$和$\phi^{-1}$是多项式映射；
(iii) $(a_1 \times a_2 \times \cdots \times a_p)^2$ 到$a_1 \times a_2 \times \cdots \times a_p$ 的映射 $(x, y) \mapsto \phi^{-1}(\phi(x) \cdot \phi(y)^{-1})$ 是多项式。

命题对于$\dim g = 0$来说是显而易见的。假设已经为维数$< \dim g$建立了$\dim g > 0$和命题。可以假设$g_{n-1} \neq \{0\}$和$g_{n-1}$是$g$的非零中心理想。存在指标$j$使得$h = g_{n-1} \cap a_j \neq \{0\}$。令$g' = g/h$、$\theta$为$g$到$g'$、$g'_i = \theta(g_i)$和$a'_i = \theta(a_i)$的规范态射。那么$(g'_0, g'_1, \ldots, g'_n)$是$g'$理想的递减序列使得$g'_0 = g', g'_n = \{0\}$，

$$
[g', g'_i] \subset g'_{i+1}
$$

对于$0 \leq i < n$，每个$g'_i$是其交的直和和$a'_j$。设$\phi'$为映射

$$
(x'_1, x'_2, \ldots, x'_p) \mapsto x'_1 \mathbf{H} x'_2 \mathbf{H} \cdots \mathbf{H} x'_p
$$

将$a'_1 \times a'_2 \times \cdots \times a'_p$转化为$g'$。根据归纳假设，$\phi'$是双射，$\phi', {\phi'}^{-1}$是多项式映射。

让$x \in g$。我们写

(1)
$$
{\phi'}^{-1}(\theta(x)) = (x'_1(x), x'_2(x), \ldots, x'_p(x)).
$$
Then
(2)
$$
\theta(x) = x'_1(x) \mathbf{H} x'_2(x) \mathbf{H} \cdots \mathbf{H} x'_p(x).
$$
Let $h_1$ be a vector subspace supplementary to $h$ in $g$, the sum of the $a_k$ with $k \neq j$ and a supplement of $h$ in $a_j$. 存在 $g'$ 的双射 $\eta$ 到 $h_1$ 使得 $\theta \circ \eta = \mathrm{Id}_{g'}$。 对于$x \in g$，我们写
(3)
$$
\zeta(x) = \eta(x'_1(x)) \mathbf{H} \eta(x'_2(x)) \mathbf{H} \cdots \mathbf{H} \eta(x'_p(x)) \in g.
$$
(4)
$$
y(x) = \zeta(x)^{-1} \mathbf{H} x = (-\zeta(x)) \cdot x.
$$

由（2）和（3），$\theta(\zeta(x)) = \theta(x)$，因此$y(x) \in \mathfrak{h}$。最后我们写
$$
(5) \quad \psi(x) = (\eta(x_1'(x)), \ldots, \eta(x_p'(x)) + y(x), \ldots, \eta(x_p'(x))) \in a_1 \times \cdots \times a_p.
$$
由于$y(x)$是$\mathfrak{g}$的中心，
$$
\begin{align*}
\phi(\psi(x)) &= \eta(x_1'(x)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \eta(x_p'(x)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \eta(x_p'(x)) \mathbin{\mathbf{H}} y(x) \\
&= \zeta(x) \mathbin{\mathbf{H}} y(x) & \text{by (3)} \\
&= x & \text{by (4).}
\end{align*}
$$
因此$\phi \circ \psi = \mathrm{Id}_g$。现在设$(x_1, x_2, \ldots, x_p) \in a_1 \times a_2 \times \cdots \times a_p$并写出$x = \phi(x_1, x_2, \ldots, x_p) = x_1 \mathbin{\mathbf{H}} x_2 \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} x_p$。然后
$$
\theta(x) = \theta(x_1) \mathbin{\mathbf{H}} \theta(x_2) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \theta(x_p),
$$
因此 $x_i'(x) = \theta(x_i)$ 代表 $1 \leq i \leq p$ 因此
$$
\begin{align*}
\zeta(x) &= x_1 \mathbin{\mathbf{H}} x_2 \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} (\eta \theta(x_j)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} x_p \\
y(x) &= x_j - \eta \theta(x_j).
\end{align*}
$$
然后由(5)
$$
\psi(x) = (x_1, \ldots, \eta \theta(x_j) + x_j - \eta \theta(x_j), \ldots, x_p) = (x_1, x_2, \ldots, x_p).
$$
因此$\psi \circ \phi = \mathrm{Id}_{a_1 \times \ldots \times a_p}$。这就证明了(i)。由于 Hausdorff 律是多项式，$\phi$ 也是多项式。由归纳假设，${\phi'}^{-1}$为多项式；由公式 (1)、函数 $x_j'$ 是多项式，因此 $\zeta$ 是多项式 (公式 (3))、$y$ 是多项式 (公式 (4)) 和 $\psi$ 是多项式 (公式) (5))。这就证明了(ii)。 断言 (iii) 由 (i) 和 (ii) 得出，并且 Hausdorff 律是多项式。

**幂零李群的例。**令$G$为$\mathbf{GL}(n, K)$的下严格三角形子群。它是 $\mathbf{GL}(n, K)$ 的谎言子群，$L(G) \subset \mathfrak{gl}(n, K)$ 是具有零对角线（§ 3, no. 10，命题 36）的下三角矩阵的李代数。到章 II, § 4, no. 6，*注*，$G$ 幂零。假设此后$K = \mathbf{R}$或$\mathbf{C}$。由于$G$与$K^{n(n-1)/2}$同胚，$G$是单连通的。 $L(G)$ 到 $G$ 的指数映射只是映射
$$
u \mapsto \exp u = \sum_{k \geq 0} \frac{u^k}{k!} = \sum_{k=0}^{n-1} \frac{u^k}{k!}
$$
（§ 6, no. 4，*例*）。到命题 13 时，流形 $L(G)$ 到流形 $G$ 的指数为同构。 § 6, no. 9 中的命题 17 给出逆双射 $\log$。我们给$K^n$范数。根据*光谱理论*，章I, § 4, no. 9，对于$g \in G$和$\|g - 1\| < 1$，
$$
\log g = \sum_{k \geq 1} \frac{(-1)^{k-1}}{k} (g - 1)^k
$$

那就是
$$
\log g = \sum_{k=1}^{n-1} \frac{(-1)^{k-1}}{k} (g-1)^k.
$$
但 (6) 的两侧是 $g$ 对 $g \in G$ 的解析函数，因此对于所有 $g \in G$ 都是相等的。

#### 命题 18 {#lie-iii-s9-prop-18 .statement tag=0AJ5}

*令k为交换域。 V 向量空间 of 有限维的 > 0 over k 且 G 子群 of $\mathbf{GL}(V)$ 其元素是单能的。*
  (i) *存在 V 的非零元素 v，使得对于 G 中的所有 g，gv = v。*
  (ii) *存在V的基B，使得对于G中的所有g \in，g相对于B的矩阵是下三角且其所有对角线元素等于1。*
  (iii) *群 G 幂零。*
    (a) 首先假设 k 是代数闭的并且 G 的恒等式表示是简单的。设a,b在G中，则
    $$
    \operatorname{Tr}(a(b-1)) = \operatorname{Tr}(ab-1) - \operatorname{Tr}(a-1) = 0 - 0 = 0
    $$
    因为 $ab - 1$ 和 $a - 1$ 是幂零的。由于G生成的$\mathscr{L}(V)$的向量子空间是$\mathscr{L}(V)$（*代数*，章VIII, § 4，推论1到命题2），$\operatorname{Tr}(u(b-1)) = 0$对于所有$u \in \mathscr{L}(V)$，因而$b = 1$。因而$G = \{1\}$。
    (b) 现在我们讨论一般情况。令$\bar{k}$为k的代数闭包，对于$a \in G$，$\bar{V} = V \otimes_k \bar{k}$和$\bar{G} \subset \mathbf{GL}(\bar{V})$集合为$a \otimes 1$。设W（分别$W'$）为V（分别$\bar{V}$）元素集合在G（分别$\bar{G}$）下不变。然后用$W' = W \otimes_k \bar{k}$换$W = \bigcap_{g \in G} \operatorname{Ker}(g-1)$和$W' = \bigcap_{g \in G} \operatorname{Ker}(g-1) \otimes 1$。如果$V_1$表示$\bar{V}$的非零向量子空间的集合中的最小元素且在$\bar{G}$下稳定，则$V_1 \subset W'$乘以证明的部分(a)；因而$W \neq \{0\}$，证明了(i)。
    (c) 通过$\dim V$上的归纳，从(i)得出，存在V的向量子空间的递增序列$(V_1, V_2, \ldots, V_n)$，它们在G下是稳定的，使得$V_n = V$和自同构群对于所有 $i$，$V_i/V_{i-1}$ 规范地从 G 约化到 $\{1\}$（我们约定 $V_r = \{0\}$ 代表 $r \leq 0$）。这意味着首先是 (ii)，然后是 (iii) (章 II, § 4, no. 6，*注*)。

#### 推论 1 {#lie-iii-s9-prop-18-cor-1 .statement tag=0AJ6}

*设 G 为有限维连通实数或复数李群。要使 G 幂零，Ad G 的每个元素都是幂零的必要且充分。*

如果 Ad G 的每个元素都是单能的，则 Ad G 是幂零的 (命题 18)，因此作为 Ad G 的中心扩张的 G 也是幂零的。如果 G 是幂零的，则 $L(G)$ 是幂零的，因此 $\operatorname{ad} x$ 对于所有 $x \in L(G)$ 来说是幂零的，因此 $\operatorname{Ad}(\exp x) = \exp \operatorname{ad} x$ 是单能的；但对于某些 $x \in L(G)$ (命题 14)，G 的每个元素都是形式 $\exp x$。

#### 推论 2 {#lie-iii-s9-prop-18-cor-2 .statement tag=0AJ7}

*单能元素的$\mathbf{GL}(n, K)$由……组成的每个解析子群都是单连通谎言子群。*

这是从命题 13 (ii) 和 18 (ii) 以及下严格三角形群是单连通的事实得出的。

### 6.可解李群

#### 命题 19 {#lie-iii-s9-prop-19 .statement tag=0AJ8}

*令 $G$ 为有限维李群。为了使$L(G)$可解，$G$拥有可解开子群是必要且充分的。*

证明类似于 no. 5 的命题 12。

#### 命题 20 {#lie-iii-s9-prop-20 .statement tag=0AJ9}

*设$G$是有限维$n$在$\mathbf{R}$或$\mathbf{C}$和$g = L(G)$上的单连通可解李群。令$(g_n, g_{n-1}, \ldots, g_0)$为维数$n, n-1, \ldots, 0$$g$子代数序列，使得$g_{i-1}$是$g_i$对于$i = n, n-1, \ldots, 1.\dagger$的理想令$G_i$为子群的积分$G$相应的至$g_i$。令$x_i$为$g_i$中的向量，而不是属于到$g_{i-1}$。令 $\phi_i$ 为映射*

$$
(\lambda_1, \lambda_2, \ldots, \lambda_i) \mapsto (\exp \lambda_1 x_1)(\exp \lambda_2 x_2) \cdots (\exp \lambda_i x_i)
$$

*将 $K^i$ 变为 $G$。那么对于所有 $i$，$\phi_n$ 是解析流形和 $\phi_i(K^i) = G_i$ 的同构。*

对于 $n = 0$ 命题是显而易见的。我们在$n$上争论归纳。令$H$为$G$的积分子群，使得$L(H) = Kx_n$。通过§ 6, no. 6，推论1到命题14，$H$和$G_{n-1}$是简单连接$G$的谎言子群，并且，如李群，$G$是乘积的半直接乘积 $H$ $G_{n-1}$。因此 $\lambda \mapsto \exp(\lambda x_n)$ 是 $K$ 的同构到 $H$ 并由归纳假设映射

$$
(\lambda_1, \lambda_2, \ldots, \lambda_{n-1}) \mapsto (\exp \lambda_1 x_1)(\exp \lambda_2 x_2) \cdots (\exp \lambda_{n-1} x_{n-1})
$$

是解析式流形$K^{n-1}$的同构到解析式流形$G_{n-1}$，其中映射$K^i \times \{0\}$到$G_i$对于$i = 1, 2, \ldots, n-1$。因此命题。

#### 命题 21 {#lie-iii-s9-prop-21 .statement tag=0AJA}

*设$G$是$\mathbf{R}$或$\mathbf{C}$上的单连通有限维可解李群，并且$M$是$G$的积分子群。那么 $M$ 是 $G$ 的谎言子群并且是单连通的。*

我们继续使用命题20的记号$n, g, g_i, x_i, \phi$，但对$x_i$施加以下补充条件：令$i_p > i_{p-1} > \cdots > i_1$为整数$i$，使得$L(M) \cap g_i \neq L(M) \cap g_{i-1}$；然后我们采取

$$
x_{i_k} \in L(M) \cap g_{i_k}
$$

\dagger 这样的序列由章 I, § 5、命题 2 存在。

$k = 1, 2, \ldots, p$。到$n$上的归纳，很容易看出$(x_{i_p}, x_{i_{p-1}}, \ldots, x_{i_1})$是$L(M)$的基。令$N$为单连通李群，使得$L(N)$存在同构$h$到$L(M)$。让
$$
y_p = h^{-1}(x_{i_p}), \ldots, y_1 = h^{-1}(x_{i_1}).
$$
命题20、映射
$$
(\lambda_1, \lambda_2, \ldots, \lambda_p) \mapsto (\exp \lambda_1 y_1)(\exp \lambda_2 y_2) \cdots (\exp \lambda_p y_p)
$$
是流形$K^p$的同构到流形$N$。 $G$中存在$N$的李群态射$\tau$，使得$h = L(\tau)$和$\tau(N) = M$（§ 6, no. 2，推论1到命题1）。因此$M$是形式$G$元素集合
$$
\tau((\exp \lambda_1 y_1) \cdots (\exp \lambda_p y_p)) = \exp(\lambda_1 L(\tau)y_1) \cdots \exp(\lambda_p L(\tau)y_p)
= \exp(\lambda_1 x_{i_1}) \cdots \exp(\lambda_p x_{i_p}).
$$
因此$M = \phi(T)$，其中$T$是$K^n$的向量子空间。

#### 命题 22 {#lie-iii-s9-prop-22 .statement tag=0AJB}

*假设$K = \mathbf{R}$或$\mathbf{C}$。令$V$为有限维向量空间，且$G$为$\mathbf{GL}(V)$的连通可解子群。假设$G$的恒等式表示很简单。*
(i) *如果 $K = \mathbf{R}$，则 $\dim V \leq 2$ 和 $G$ 是可交换的。*
(ii) *如果$K = \mathbf{C}$，则$\dim V = 1$。*
(i) 假设$K = \mathbf{R}$。那么$\mathbf{GL}(V)$中$G$的闭包$H$是$\mathbf{GL}(V)$的可解连通李子群（no. 1，推论2到命题1）。因此 $L(H)$ 是可解的 (命题 19)。 $L(G)$的恒等式表示很简单（§ 6, no. 5，推论2到命题13）。因此$\dim V \leq 2$和$L(G)$是可交换的（章I, § 5，推论1和4到定理1）。因此 $G$ 是可交换的。
(ii) 假设$K = \mathbf{C}$。令$W$为$V$的非零实数向量子空间中最小的元素，其在$G$下稳定。由$W$生成的$V$的复数向量子空间等于$V$，因为$G$的恒等式表示很简单。通过(i)，$G|W$是可交换的。因此 $G$ 是可交换的。因此，$G$的每个元素都是位似（*代数*，章VIII, § 4，推论1到命题2），因此$\dim V = 1$。

#### 推论{#lie-iii-s9-n6-cor-1 .statement tag=0AJC}

*令 $V$ 为有限维 $> 0$ 的复数向量空间和 $G$ $\mathbf{GL}(V)$ 的连通可解子群。*
(i) *存在 $V$ 的非零元素 $v$，使得 $gv \in Cv$ 对于所有 $g \in G$。*
(ii) *存在$V$的基$B$，使得对于所有$g \in G$，$g$相对于$B$的矩阵是下三角形。*
令$V_1$为$V$的非零向量子空间中最小的元素，其在$G$下稳定。 命题 22 (ii)，$\dim V_1 = 1$。这就证明了(i)。通过$\dim V$上的归纳，可以得出结论，存在$V$的向量子空间的递增序列$(V_1, V_2, \ldots, V_n)$，它们在$G$下是稳定的，使得$\dim V_{i+1}/V_i = 1$对于$i < n$和$V_n = V$；因此(ii)。

### 7. 李群的根式

#### 命题 23 {#lie-iii-s9-prop-23 .statement tag=0AJD}

*设$G$为有限维实数或复数李群，$r$$L(G)$*的根式（章I, § 5，定义2）*和$n$最大的$L(G)$*的幂零理想（章I, § 4, no. 4）。 *令$R$（或$N$）为$G$与李代数$r$（或$n$）的积分子群。那么$R$（或$N$）是$G$的可解（或幂零）谎言子群，它在$G$的每个连续自同构下是不变的。 *$G$ 的每个可解（或幂零）连接法线子群都包含在 $R$（或$N$）中。*

群 $R$ 是可解的（$§ 6$，命题 19）。假设$K = R$。令 $G'$ 为 $G$ 的连通可解法线子群。那么$\overline{G'}$是$G$（$§ 8$，no. 2，定理2）的连通可解（no. 1，推论2到命题1）正常谎言子群。因此，$L(\overline{G'})$是$L(G)$、从而、$L(\overline{G'}) \subset r$和$\overline{G'} \subset R$的可解理想。特别是，$\overline{R} \subset R$，因此$R$是封闭的，因此是$G$的谎言子群。假设$K = C$。令 $H$ 为 $G$ 的底层真实谎言子群。若$r'$是$L(H)$的根式，则$ir'$是$L(H)$、从而$r' = ir'$的可解理想；因此 $r \subset r' \subset r$ 并且，根据上述，$R$ 在 $H$ 中闭合，因此在 $G$ 中闭合；因此$R$是$G$的谎言子群。 $G$ 的每个连通可解法线子群都是 $H$ 的连通可解法线子群，因此包含在 $R$ 中。因此，我们已经证明对于$K = C$和$K = R$，$R$是最大的连通的$G$的可解法线子群；因此$R$在$G$的每一个连续的自同构下都是不变的。 证明与 $N$ 完全类似。

#### 定义 1 {#lie-iii-s9-def-1 .statement tag=0AJE}

*令$G$为有限维实数或复数李群。 $G$的根式是最大的连接$G$的可解正规子群。*

#### 注 {#lie-iii-s9-n7-rem-1 .statement tag=0AJF}

即使$G$是连通的，也可能存在不包含在$G$的根式中的$G$的可解法线子群。

#### 命题 24 {#lie-iii-s9-prop-24 .statement tag=0AJG}

*假设$K = R$或$C$。令$G_1, G_2$是两个有限维连接的李群、$R_1$和$R_2$它们的根式，以及$\phi$是$G_1$到$G_2$的满射态射。然后$\phi(R_1) = R_2$.*

到 $§ 3$、no. 8、命题 28，$L(\phi)$ 是满射。因此$L(\phi)(L(R_1)) = L(R_2)$（章I，$§ 6$，推论3到命题2）。设$i$为$R_1$到$G_1$的典范嵌入。那么$\phi \circ i$的像就是$R_2$（$§ 6$，no. 2，推论1到命题1）。

#### 命题 25 {#lie-iii-s9-prop-25 .statement tag=0AJH}

*假设$K = R$或$C$。令 $G_1, G_2$ 为有限维连接的李群和 $R_1$ 以及 $R_2$ 它们的根式。 $G_1 \times G_2$的根部是$R_1 \times R_2$。*

这是从章 I、$§ 5$、命题 4 开始的。

### 8.半单李群

#### 命题 26 {#lie-iii-s9-prop-26 .statement tag=0AJI}

令 G 为有限维连通实数或复数李群。以下条件是等效的：
(i) $L(G)$ 为半单；
(ii) G的根是$\{e\}$；
(iii) G 的每个正规交换积分子群等于$\{e\}$。
条件 (ii) 意味着 $L(G)$ 的根部是 $\{0\}$，因此 (i) $\Leftrightarrow$ (ii) (章 I, § 6, 定理 1)。 (i)和(iii)的等价由§ 6, no. 6、命题14得出。

#### 定义 2 {#lie-iii-s9-def-2 .statement tag=0AJJ}

如果连通实数或复数李群是有限维且满足命题 26 的条件，则称为半单。

#### 注 1 {#lie-iii-s9-n8-rem-1 .statement tag=0AJK}

令 G 为有限维连通实数或复数李群。如果 G 不是半单，则 G 具有交换连通李子群 $G'$，它在每个连续自同构下都是不变的，使得 $G' \neq \{e\}$。令 n 为 $L(G)$ 的最大的幂零理想；那么$n \neq \{0\}$和相应的解析子群N是一个谎言子群，它在G的每个连续自同构下保持不变（no. 7，命题23）； N 的中心 $G'$ 具有所需的性质。

#### 命题 27 {#lie-iii-s9-prop-27 .statement tag=0AJL}

令 G 为有限维连通实数或复数李群。以下条件是等效的：
(i) $L(G)$ 很简单；
(ii) G 的唯一正规积分子群是 $\{e\}$ 且 G 且 G 不可交换。
这是从§ 6, no. 6、命题 14 开始的。

#### 定义 3 {#lie-iii-s9-def-3 .statement tag=0AJM}

如果连通实数或复数李群是有限维的并且满足命题 27 的条件，则称为几乎简单。

#### 命题 28 {#lie-iii-s9-prop-28 .statement tag=0AJN}

令 G 为单连通实数或复数李群。以下条件是等效的：
(i) G 为半单；
(ii) G 同构于几乎简单的群的有限数的乘积。
如果 G 是几乎简单李群的有限乘积，则 $L(G)$ 是简单李代数的有限乘积，因此是半单。如果 G 是半单，则 $L(G)$ 同构于简单李代数 $L_1, \ldots, L_n$ 的乘积。令 $G_i$ 为李群与李代数 $L_i$ 的简单连接，因此这几乎是简单的。则 G 和 $G_1 \times \cdots \times G_n$ 是单连通的，并且具有同构李代数，因此是同构的。

#### 引理 1 {#lie-iii-s9-lem-1 .statement tag=0AJO}

设G是连通拓扑群，Z是中心，$Z'$是Z的离散子群。那么$G/Z'$的中心是$Z/Z'$。
设 y 为 G 的元素，其类模 $Z'$ 是 的中心元素

G/Z'。令 $\phi$ 为 G 的映射 $g \mapsto gyg^{-1}y^{-1}$ 进入 G。然后 $\phi(G)$ 连接并包含在 $Z'$ 中，因此也包含在 $\phi(G) = \phi(\{e\}) = \{e\}$ 中。因此$y \in Z$。

#### 命题 29 {#lie-iii-s9-prop-29 .statement tag=0AJP}

*令 G 为半单连接实数或复数李群。*
（一）$G = (G, G)$。
(ii) *G 的中心 Z 是离散的。*
(iii) *$G/Z$的中心是$\{e\}$*。
断言 (i) 由命题 4、no. 2 和章 I, § 6、定理 1 的推论得出。
断言 (ii) 由§ 6, no. 4、推论4 到命题 10 和章 I, § 6, no. 1、*注 2*。
断言 (iii) 由 (ii) 和引理 1 得出。

#### 命题 30 {#lie-iii-s9-prop-30 .statement tag=0AJQ}

(i) *令$\mathfrak{g}$为半单实数或复数李代数。那么 Int $\mathfrak{g}$ 就是 Aut $\mathfrak{g}$.* 的恒等分量。
(ii) *令 G 为半单连接实数或复数李群。 G 的伴随群是Aut $L(G)$ 的恒等分量。 中心约化至单位元素。*
$\mathfrak{g}$的每个推导都是内部（章I, § 6，推论3到命题1），因此$L(\mathrm{Int}\,\mathfrak{g}) = L(\mathrm{Aut}\,\mathfrak{g})$，这证明了（i）。 (ii) 的第一个断言由 (i) 得出。第二个是从命题 29 (iii) 和§ 6, no. 4、推论4 (ii) 到命题 10。

#### 注 2 {#lie-iii-s9-n8-rem-2 .statement tag=0AJR}

令$\mathfrak{g}$为复半单李代数，$\mathfrak{g}_0$其底层实数李代数。然后Aut$(\mathfrak{g})$在Aut$(\mathfrak{g}_0)$中打开，对于Int$(\mathfrak{g}_0) \subset \mathrm{Aut}(\mathfrak{g})$。

#### 命题 31 {#lie-iii-s9-prop-31 .statement tag=0AJS}

*设 G 为单连通有限维实数或复数李群，R 为其根式。 G 存在半单单连通李子群 S，使得 G 作为李群，是 R 对 S 的半直乘积。如果 S' 是 G 的半单积分子群，则$L(G)$的幂零根中存在 x，使得*
$$
(\mathrm{Ad}\exp x)(S') \subset S.
$$
这是从§ 6, no. 6，推论1到命题14和章I, § 6，定理5和推论1。

#### 引理 2 {#lie-iii-s9-lem-2 .statement tag=0AJT}

*设 G 为群（或拓扑群），G' 为 G 的法线子群，V 有限维向量空间在交换域 k 上（或在 K 上），$\rho$ 线性表示（或连续V 和 $\rho' = \rho|_{G'}$ 上的 G 的线性表示)。*
(i) *如果 $\rho$ 为半单，则 $\rho'$ 为半单。*
(ii) *如果 $\rho'$ 为半单，且 $G/G'$（或 $G/\overline{G}'$）的每个有限维线性 k 表示（或连续线性 K 表示）为半单，则 $\rho$ 为半单。*
假设$\rho$是半单；我们证明$\rho'$是半单。考虑$\rho$很简单的情况就足够了。令$V'$为V的最小非零子G'模。对于所有$g \in G$、$\rho(G')\rho(g)V' = \rho(g)\rho(G')V' = \rho(g)V'$，其他字$\rho(g)V'$稳定在$\rho(G')$以下；如果$V''$是$\rho(g)V'$的子$G'$模块，则$\rho(g)^{-1}V''$是$V'$的子$G'$模块，因此$V''$等于$\{0\}$或$\rho(g)V'$。

因此，对于所有 $g \in G$，$\rho(g)V'$ 是一个简单的 $G'$ 模块。但$\sum_{g \in G} \rho(g)V'$是$V$、从而$V = \sum_{g \in G} \rho(g)V'$的非零子$G$模。因此$\rho'$是半单。

假设$\rho'$是半单。令$W$为$V$的非零子$G$模。由于$\rho'$是半单，因此$V$存在投影算子$f_0$到与$\rho'(G)$通勤的$W$。令$E$为$f \in \mathscr{L}(V, V)$的集合，与$\rho(G')$可交换，映射$V$进入$W$，限制到$W$为位似；对于$f \in E$，让$\alpha(f)$表示位似$f|W$的比率。然后是$f_0 \in E$和$\alpha(f_0) = 1$。显然 $\alpha$ 是 $E$ 上的线性形式。让$F = \mathrm{Ker}\, \alpha$，它是$E$的超平面。对于$f \in E$和$g \in G$，我们写为$\sigma(g)f = \rho(g) \circ f \circ \rho(g)^{-1}$；那么$\sigma(g)f$映射$V$化为$W$，其限制与$W$的比值为$\alpha(f')$的位似；如果$g' \in G'$，那么
$$
\begin{align*}
\sigma(g)f \circ \rho(g') &= \rho(g) \circ f \circ \rho(g)^{-1} \circ \rho(g') \\
&= \rho(g) \circ f \circ \rho(g^{-1}g'g) \circ \rho(g^{-1}) \\
&= \rho(g) \circ \rho(g^{-1}g'g) \circ f \circ \rho(g^{-1}) \\
&= \rho(g') \circ \rho(g) \circ f \circ \rho(g^{-1}) \\
&= \rho(g') \circ \sigma(g)f.
\end{align*}
$$
因此$\sigma(g)f \in E$。因此，$\sigma$是$E$上$G$的线性$k$表示（分别是连续线性$K$表示），而$F$保持稳定。然后，在拓扑情况下，$\sigma(g) = \mathrm{Id}_E$代表$g \in G'$，因此也代表$g \in \overline{G'}$。假设$G/G'$（或$G/\overline{G'}$）的每个有限维$k$线性表示（或连续$K$线性表示）都是半单。那么$F$中存在$E$补充，在$G$下是稳定的。在其他字中，存在$f \in E$使得$\alpha(f) = 1$在$G$下不变。那么$f$是$V$到$W$的投影算子，并且，对于$g \in G$，$\rho(g) \circ f \circ \rho(g^{-1}) = f$，即$f$与$\rho(G)$通勤。因此$\rho$是半单。

#### 定理 1 {#lie-iii-s9-thm-1 .statement tag=0AJU}

*设$G$为有限维实数或复数李群，$G_0$其单位分量，$R$其根式以及$r$$L(G)$的根式；假设 $G/G_0$ 是有限的。令 $\rho$ 为 $G$ 的有限维解析线性表示。以下条件是等效的：*
(i) $\rho$ 为半单；
(ii) $\rho|G_0$ 为半单；
(iii)$\rho|R$为半单；
(iv)$L(\rho)$为半单；
(v) $L(\rho)|r$ 是半单。
(i) $\Leftrightarrow$ (ii) 通过引理 2 和积分，章 VII, § 3、命题 1。
(ii) $\Leftrightarrow$ (iv) 和 (iii) $\Leftrightarrow$ (v) 由 § 6, no. 5，推论 2 至命题 13。
(iv) $\Leftrightarrow$ (v) 章 I, § 6、定理 4。

#### 推论 1 {#lie-iii-s9-thm-1-cor-1 .statement tag=0AJV}

*令 $\rho, \rho_1, \rho_2$ 为有限维半单解析线性表示

李群

$G$和$n$整数$\geq 0$的句子。那么 $\rho_1 \otimes \rho_2, T^n \rho, S^n \rho, \wedge^n \rho$ (附录) 就是半单。

$\rho_1 \otimes \rho_2$ 的半单纯性源自定理 1 和章 I, § 6，推论 1 至定理 4。 $T^n \rho, S^n \rho, \wedge^n \rho$ 的半单纯性源自 $\rho_1 \otimes \rho_2$ 的半单纯性。

稍后我们将看到，如果$k$是特征0的交换域，$\Gamma$群和$\rho_1$和$\rho_2$有限维半单线性$k$-$\Gamma$的表示，那么$\rho_1 \otimes \rho_2$是半单。

#### 推论 2 {#lie-iii-s9-thm-1-cor-2 .statement tag=0AJW}

*设$\rho$为$G$在向量空间$V$上的有限维半单解析线性表示，$S$$V$和$S^G$的对称代数 $S$ 的子代数元素的由……组成在$(S\rho)(G)$ 下不变。那么$S^G$就是有限生成的代数。*

这是从定理 1、章 I, § 6、定理 6 (a) 和 *交换代数*、章 V, § 1、定理 2 得出。

#### 推论 3 {#lie-iii-s9-thm-1-cor-3 .statement tag=0AJX}

*设$G$为实数或复数李群，$G_0$为其恒等分量。假设 $G_0$ 是半单并且 $G/G_0$ 是有限的。那么$G$的每个有限维解析线性表示都是半单。*

#### 命题 32 {#lie-iii-s9-prop-32 .statement tag=0AJY}

*令$G$为有限维连通的实李群。假设 $L(G)$ 是可还原的。以下条件是等效的：

(i) $G/\overline{D^1}G$ 是紧的；
(ii) (resp. (ii')) 复数（resp. real）向量空间上 $G$ 的每个有限维解析线性表示都是半单。

(i) $\Rightarrow$ (ii')：假设$G/\overline{D^1}G$ 是紧的。那么在有限维实数向量空间上$G/\overline{D^1}G$的每个连续线性表示都是半单（*积分*，章VII, § 3，命题1）。令 $\rho$ 为 $G$ 在实向量空间上的有限维解析线性表示。那么$\rho|D^1G$是解析的，$D^1G$是半单（章I, § 6，命题5），因此$\rho|D^1G$是半单（推论3到定理1）。因此$\rho$是半单（引理2）。

类似地可以看出(i)$\Rightarrow$(ii')。

(i) $\Rightarrow$ (ii)：假设 $G/\overline{D^1}G$ 不是紧的，因此与形式 $\mathbf{R}^p \times \mathbf{T}^q$ 的群与 $p > 0$ ($§ 6$, no. 4, 命题 11 (ii)) 同构的。那么在$\mathbf{R}$上存在$G/\overline{D^1}G$的满射态射，因此在$\mathbf{R}$上存在$G$的满射态射。 映射

$$
g \mapsto \sigma(g) = \begin{pmatrix} 1 & 0 \\ \rho(g) & 1 \end{pmatrix}
$$

是$\mathbf{R}^2$上$G$的解析线性表示，它不是半单，因为$\mathbf{R}^2$的唯一一维向量子空间在$\sigma(G)$下稳定，是$\mathbf{R}(0, 1)$。

类似地可以看出(ii)$\Rightarrow$(i)。

#### 命题 33 {#lie-iii-s9-prop-33 .statement tag=0AJZ}

令 G 为有限维复数李群，其连通分量的数是有限的，$\varphi$ G 的有限维解析线性表示和 $G'$ 实李群 G 的积分子群，使得 $L(G')$ 生成 $L(G)$超过$\mathbf{C}$。那么，为了使$\varphi$成为半单，$\varphi|G'$成为半单是充分必要的。

让$\varphi' = \varphi|G'$。为了使$\varphi$（或$\varphi'$）成为半单，$L(\varphi)$（或$L(\varphi')$）为半单（定理 1）是必要且充分的。令 V 为 $\varphi$ 的空间。为了使V的向量子空间在$L(\varphi)(L(G))$下稳定，其在$L(\varphi')(L(G'))$下稳定是充分必要的。因此命题。

### 习题{#lie-iii-s9-exercises}

§ 9](exercises/s9/)参见[习题。
