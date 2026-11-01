---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 8
section_title: Complex locally convex spaces
lang: zh
source: evt-i-v
book_pages: TVS II.95
pdf_pages: 0097-0102, 0132-0132
extraction: ocr
subsections:
    - "no": 1
      title: Topological vector spaces over $\mathbf{C}$
      page: 60
      pdf_page: 97
    - "no": 2
      title: Complex locally convex spaces
      page: 62
      pdf_page: 99
    - "no": 3
      title: The Hahn-Banach theorem and its applications
      page: 63
      pdf_page: 100
    - "no": 4
      title: Weak topologies on complex vector spaces
      page: 64
      pdf_page: 101
statements: 10
exercises: 3
content_sha256: 6b174be35110ec2bc775d062526ced92fb4dd21ee885973e3a7775f5bef56d80
translated_from: content/en/evt/II/08_s8_complex_locally_convex_spaces.md
translation_method: google
source_content_sha256: 5d9e93b1130d665e5ef5a49bee7fa6d59d2370123e602805e4b774a529b5d3c0
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 419349e884250b03fafa99994d28287951ffd94293d6540932fbf927d563c580
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 8。复局部凸空间

### 1. 拓扑向量空间超过$\mathbf{C}$

设$E$是复数的$\mathbf{C}$域上的拓扑向量空间； $E$的拓扑也与$\mathbf{R}$上的向量空间的结构兼容，这是通过将标量的域限制为$\mathbf{R}$获得的。我们用$E_0$表示$\mathbf{R}$上的拓扑向量空间，它*位于*E（I，p. 2）。 注，在$E_0$中，映射$x \mapsto ix$（不是位似）是$E_0$的拓扑向量空间结构的*自同构*$u$，使得$u^2(x) = -x$。

相反，令F是$\mathbf{R}$上的拓扑向量空间，并假设F存在自同构$u$，使得$u^2 = -1_F$（$1_F$是F的恒等式自同构）。我们知道（A，IX, § 3, No. 2），那么对于所有$\lambda = \alpha + i\beta \in \mathbf{C}$和所有$x \in F$，可以相对于$\mathbf{C}$在F上定义向量空间结构写出$\lambda x = \alpha x + \beta u(x)$。进一步，由于F中$\mathbf{R}^2 \times F$的映射$(\alpha, \beta, x) \mapsto \alpha x + \beta u(x)$是连续的，因此F的拓扑相对于上面定义的$\mathbf{C}$与向量空间结构兼容；如果 E 表示以这种方式定义的 $\mathbf{C}$ 上的拓扑向量空间，则 F 是 E 之下的 $\mathbf{R}$ 上的拓扑向量空间。

#### 注 {#evt-ii-s8-n1-rem-1 .statement tag=07KJ}

— 给定一个在 $\mathbf{R}$ 上的拓扑向量空间 F，并不总是存在自同构 $u$ 的 F，其平方是 $-1_F$；对于例，定义向量空间结构相对于$\mathbf{C}$在向量空间上不可能超过有限*奇数*维数的$\mathbf{R}$。

设E是$\mathbf{C}$上的拓扑向量空间，$E_0$是$\mathbf{R}$上的拓扑向量空间，它是E的基础。E中的每个线性簇M也是$E_0$中的线性簇，但逆命题是假的。为了避免混淆，我们说向量空间结构相对于 $\mathbf{C}$（或相对于 $\mathbf{R}$）的线性簇是*复数*（或*实数*）线性簇。复线性簇有限维 $n$（分别为有限余维 $n$）是实线性簇维数 $2n$（分别为余维 $2n$）。在阶中，E的实向量子空间M也应该是复数向量子空间，$iM \subset M$是充分必要的。

回想一下，如果 E 和 F 是 $\mathbf{C}$ 上的两个拓扑向量空间，则 F 中 E 的映射被称为 $\mathbf{C}$ 线性（或 $\mathbf{R}$ 线性），如果对于 E 和 F 的向量空间结构来说它是线性映射至$\mathbf{C}$（分别为$\mathbf{R}$）；每个$\mathbf{C}$线性映射显然都是$\mathbf{R}$线性，但逆命题是错误的。我们说 E 上的 $\mathbf{C}$ 线性形式是*复数* 线性形式，而 E 上的 $\mathbf{R}$ 线性形式（*即* $E_0$ 上的线性形式）是*实数* 线性形式。如果$f$是E上的复数线性形式，则显然实部部分$g = \Re f$和$f$的虚部部分$h = \Im f$是实部线性形式；进一步地，关系$f(ix) = if(x)$暗示身份$h(x) = -g(ix)$；在其他字我们有

$$
f(x) = (\Re f)(x) - i(\Re f)(ix).
$$

相反，如果$g$是E上的实数线性形式，则$f(x) = g(x) - ig(ix)$是E上的唯一复形线性形式，使得$\Re f = g$；并且 $f$ 是连续的当且仅当 $g$ 是连续的。

现在让 H 为 E 中的*复数超平面*，方程为 $f(x) = \alpha + i\beta$，其中 $f$ 是 E 上的复数线性形式；放入$g = \Re f$，我们可以看到H是两个*实数超平面*$H_1, H_2$的交，分别为$g(x) = \alpha$和$g(ix) = -\beta$；如果 H 是*闭*，则 $H_1$ 和 $H_2$ 也是闭的（I，p. 13，第 1）。相反，令 $H_0$ 为齐次 *实数* 超平面，方程为 $g(x) = 0$（其中 $g$ 是 E 上的实数线性形式）；则 H，$H_0$ 和 $iH_0$ 的交是齐次*复数*超平面，并且如果 $f$ 是复数线性形式，使得 $\Re f = g$，则 $f(x) = 0$ 是 H 的方程；如果 $H_0$ 闭合，则 H 也闭合。

设G是$\mathbf{R}$上的拓扑向量空间，并令$G_{(c)}$是$\mathbf{C}$上的向量空间，通过将标量域扩展到$\mathbf{C}$（A，II, § 5.1）从G获得。 认同 G 作为 $G_{(c)}$ 的子集乘以映射 $x \mapsto 1 \otimes x$。 $\mathbf{R}$-线性映射$(x, y) \mapsto x + i.y$则为$G \times G$在$G_{(c)}$上的双射，由此我们将$G \times G$的乘积拓扑转移到$G_{(c)}$。那么$G_{(c)}$加上这个拓扑就是$\mathbf{C}$上的拓扑向量空间。我们说$G_{(c)}$是*G的*复杂拓扑向量空间。

### 2. 复局部凸空间

说复数向量空间 E 的子集 A 是*平衡的*，意味着对于所有 $x \in A$，我们对 $0 \leq \rho \leq 1$ 有 $\rho x \in A$，对所有实数 $\vartheta$ 有 $e^{i\vartheta}x \in A$。

如果 E 的集合 A 在位于 E 之下的实数空间 $E_0$ 中是凸的，我们就说 E 的集合 A 是*凸*。在阶中，E 的凸集合 $A \neq \varnothing$ 是平衡的，对于所有实数 $\vartheta$ $e^{i\vartheta}A \subset A$ 就足够了；因为这首先意味着 $-A = A$；由于 A 是凸的，我们看到 0 属于到 A，因此 $\rho A \subset A$ $0 \leq \rho \leq 1$。

令 E 为复拓扑向量空间。 E 的最小的平衡凸（或闭平衡凸）集合包含集合 A 称为 A 的*平衡凸包络*（或*平衡闭凸包络*）； A 的平衡闭凸包络是 A 的平衡凸包络的闭包。最后是集合 $e^{i\vartheta}A$ 的并凸包络；因此，当$(x_i)$是A的点的任何有限族，并且$(\lambda_i)$是复数的族，使得$\sum_i |\lambda_i| \leq 1$时，我们可以将定义视为线性和$\sum_i \lambda_i x_i$的集合。如果 A 是预紧的，那么它的平衡包络也是如此（I，p. 6，道具 3）。

We say that a complex topological vector space E is *locally convex* if the real underlying topological vector space $E_0$ is locally convex, that is to say if every neighbourhood of 0 in E contains a convex neighbourhood of 0; a topology $\mathscr{T}$ on E is *locally convex* if it is compatible with the vector space structure of E (relative to $\mathbf{C}$) and if E, with topology $\mathscr{T}$, is locally convex. 在这种情况下，0 包含的每个闭凸邻域 V 都有一个平衡的邻域 W（I，p. 7，道具 4），我们看到 V 也是包含 U，W 的平衡闭凸包络；在其他字中，0形式的*平衡、封闭、凸*邻域是E中0的邻域的基本系统，在比率$\neq 0$的每个位似下不变。

相反，令 E 为复数向量空间，并令 $\mathfrak{S}$ 为 E 上由*吸收性*、*平衡凸* 集合形成的滤波器基。然后我们知道（II，p. 23，命题1）$\mathfrak{S}$的集合变换与$> 0$的同位比，集合$\mathfrak{B}$是0的邻域的基本系统 E 上的实向量空间 $E_0$ 上的局部凸拓扑 $\mathscr{T}$。此外，由于$\mathfrak{B}$ 的集合是平衡的，因此它们在每个位似 $x \mapsto e^{i\vartheta}x$ 下都是不变的，这表明$\mathscr{T}$ 与向量空间兼容E 的结构（超过 $\mathbf{C}$）（I、p. 7，道具 4）。

复数向量空间 E 上的每个局部凸拓扑都可以由半范数集合定义，因为开平衡凸邻域的规范为 0 是 E 上的半范数。

实局部凸空间的想法和结果在II、p. 25到36、扩展到复局部凸空间中有详细介绍，除了用平衡凸集合替换对称凸集合之外没有任何修改。

如果复数局部凸空间是可度量且完备的 Fréchet 空间。

### 3. Hahn-Banach 定理及其应用

#### 定理 1（哈恩-巴纳赫）{#evt-ii-s8-thm-1 .statement tag=07KK}

— 令 V 为 E 的向量子空间，复数向量空间，并令 f 为 V 上的（复数）线性形式，p 为 E 上的半范数，使得 $|f(y)| \leq p(y)$ 对于所有 $y \in V$。那么在扩展 f 的 E 上存在线性形式 $f_1$，并且对于所有 $x \in E$ 都有 $|f_1(x)| \leq p(x)$。

因为$g = \Re f$是在V和满足$|\cdot(y)| \leq p(y)$中定义的实数线性形式，位于V的每个点；因此，在扩展 g 的 E 中存在实数线性形式 $g_1$，并且对于所有 $x \in E$ $|g_1(x)| \leq p(x)$（II，p. 23，cor. 1）。令$f_1(x) = g_1(x) - ig_1(ix)$为E上的复数线性形式，其中$g_1$为实数部分（II，p. 61）。对于所有真实的$\vartheta$

$$
|\Re(e^{i\vartheta}f_1(x))| = |\Re(f_1(e^{i\vartheta}x))| = |g_1(e^{i\vartheta}x)| \leq p(e^{i\vartheta}x) = p(x)
$$

因为 $p$ 是复数空间 E 的半范数；这意味着关系$|f_1(x)| \leq p(x)$，并且定理被证明。

#### 推论 1 {#evt-ii-s8-thm-1-cor-1 .statement tag=07KL}

— 设 $x_0$ 为复拓扑向量空间 E 的点，p 为 E 中的连续半范数；那么在 E 中存在定义的连续（复数）线性形式 f，使得所有$x \in E$都有$f(x_0) = p(x_0)$和$|f(x)| \leq p(x)$。

#### 推论 2 {#evt-ii-s8-thm-1-cor-2 .statement tag=07KM}

— 设 V 为复数局部凸空间 E 的向量子空间，f 为在 V 中定义且连续的（复数）线性形式；则存在定义于 E 并延伸 f 的连续线性形式 $f_1$。如果 E 被赋范，则存在也满足 $\|f_1\| = \|f\|$ 的形式 $f_1$。

#### 推论 3 {#evt-ii-s8-thm-1-cor-3 .statement tag=07KN}

— 令 M 为局部凸 Hausdorff 复数空间 E 的有限维向量子空间。则存在 E 的闭向量子空间 N，它是 E 中 M 的拓扑补集。

使用定理 1、p. 24 的证明与II、p. 23 相同。 2 和相关。 3、p. 24，道具。 2 和 p. 25，cor。 2.

#### 命题 1 {#evt-ii-s8-prop-1 .statement tag=07KO}

— 设 A 为复拓扑向量空间 E 中的开非空凸集合，M 为不满足 A 的非空（复）线性簇。则存在一个闭复形超平面 H，包含 M 且不满足 A。

我们可以假设$0 \in M$。则存在闭实数超平面$H_0$包含M且不满足A（II，p. 36；第1）。作为$M = iM$，封闭复合体超平面$H = H_0 \cap (iH_0)$具有所需的属性。

#### 推论{#evt-ii-s8-n3-cor-1 .statement tag=07KP}

— 在复数局部凸空间 E 中，每个闭复数线性簇 M 都是闭复数超平面的交，其中包含它。

事实上，对于所有$x \notin M$，存在$x$的凸开邻域$V$不满足$M$，因此存在一个闭复形超平面$H$包含$M$且不满足$V$； *更不必说* $H$ 不包含 $x$。

#### 命题 2 {#evt-ii-s8-prop-2 .statement tag=07KQ}

*设$A$为复杂拓扑向量空间$E$的非空平衡开凸集合，$B$为不满足$A$的非空凸集合。那么在$E$和数$\alpha > 0$上存在连续复形线性形式$f$，使得$A$中有$|f(x)| < \alpha$，$B$中有$|f(y)| \geq \alpha$。*

因为，在$E$和实数$\alpha$上存在连续的*实数*线性形式$g$，使得$A$中的$g(x) < \alpha$和$B$中的$g(y) \geq \alpha$（II，p. 37，道具1）。作为$0 \in A$，我们有$\alpha > 0$。我们证明连续复形线性形式 $f(x) = g(x) - ig(ix)$ 和数 $\alpha$ 具有所需的性质。因为，从$\Re f = g$开始，我们在$B$中有$|f(y)| \geq \alpha$。另一方面，对于所有$x \in A$和所有实$\vartheta$，点$e^{i\vartheta}x$属于到$A$，因为$A$是平衡的，我们有$f(x) = e^{-i\vartheta}f(e^{i\vartheta}x)$；那么存在数 $\vartheta$ 使得 $|f(x)| = \Re(e^{i\vartheta}f(x)) = g(e^{i\vartheta}x) < \alpha$ 和命题紧随其后。

#### 命题 3 {#evt-ii-s8-prop-3 .statement tag=07KR}

*设 $A$ 为复杂局部凸空间 $E$ 中的平衡、闭凸集合，并令 $K$ 为 $E$ 中不满足 $A$ 的非空紧凑凸集合。那么在$E$和数$\alpha > 0$上存在连续复形线性形式$f$，使得$|f(x)| < \alpha$在$A$中并且$|f(y)| > \alpha$在$K$中。*

命题源自 II、p. 38，道具。 4 作为支柱。 2 源自 II，p. 37，道具。 1.

### 4. 复杂向量空间上的弱拓扑

定义和 II, § 6、第 1 条和第 2 条的结果适用于没有变换的*复杂* 向量空间。如果$F$和$G$是双线性形式$B$的两个复数向量空间，那么底层的空间$F_0$和$G_0$是$\Re B$的对偶性，并且从II得出， p. 61,公式 (1) 弱拓扑$\sigma(F, G)$和$\sigma(F_0, G_0)$是相同的。

#### 定义 1 {#evt-ii-s8-def-1 .statement tag=07KS}

*设$F$和$G$是对偶的两个复数向量空间。对于 $F$ 的任何子集 $M$，$G$ 中$M$ 的极坐标（用 $M^\circ$ 表示）是 $y \in G$ 的集合，这样对于所有 $x \in M$ 来说，$\Re(\langle x, y \rangle) \geq -1$。*

如果$M^\circ$是$G$中$M \subset F$的极坐标，那么$(\lambda M)^\circ = \lambda^{-1}M^\circ$对于所有$\lambda \in \mathbf{C}^*$。

如果 $M$ 是 $E$ 的（复数）向量子空间，则 $M^\circ$ 是闭向量子空间（对于 $\sigma(G, F)$），因为关系 $\Re(\lambda \langle x, y \rangle) \geq -1$ 对于*每个*标量$\lambda \in \mathbf{C}$ 蕴含$\langle x, y \rangle = 0$；我们再次说$M^\circ$是$G$*正交*到$M$的子空间。

如果$M$是$F$中的平衡集合，则$M^\circ$是$G$中的平衡集合；在这种情况下，$M^\circ$是$y \in G$的集合，使得$|\langle x, y \rangle| \leq 1$对于所有$x \in M$；对于这个关系相当于所有$x \in M$和所有$\zeta \in \mathbf{C}$的$\Re(\langle \zeta x, y \rangle) \leq 1$，这样$|\zeta| = 1$。

对于复数向量空间，II、p. 41 到 51 的结果在没有限制的情况下也有效。

习题

### 习题 {#evt-ii-s8-exercises}

§ 8](exercises/s8/)参见[习题。
