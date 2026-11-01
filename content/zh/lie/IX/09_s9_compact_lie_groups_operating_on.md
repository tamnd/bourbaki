---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 9
section_title: Compact Lie groups operating on manifolds
lang: zh
source: lie-vii-ix
book_pages: 369-381, 419-424
pdf_pages: 0376-0388, 0426-0431
extraction: native
subsections:
    - "no": 1
      title: EMBEDDING OF A MANIFOLD IN THE NEIGHBOURHOOD OF A COMPACT SET
      page: 369
      pdf_page: 376
    - "no": 2
      title: EQUIVARIANT EMBEDDING THEOREM
      page: 373
      pdf_page: 380
    - "no": 3
      title: TUBES AND TRANSVERSALS
      page: 375
      pdf_page: 382
    - "no": 4
      title: ORBIT TYPES
      page: 377
      pdf_page: 384
statements: 19
exercises: 21
errata:
    - says: §5, no. 2, Cor. of Prop. 2
      read: §5, no. 2, Cor. 1 of Prop. 2
      why: No. 2 of section 5 prints three numbered corollaries of Proposition 2 and the reference does not say which. The sentence citing it has G simply-connected and A an alcove, and says that the composite map from A to $G_r/$Int(G) is a homeomorphism. That is Corollary 1 b), whose homeomorphisms run $A/H_A$ to $T_r/W$ to $G_r/$Int(G) and whose $H_A$ is trivial for a simply-connected group. Corollary 2 is the same statement for the Lie algebra, over a chamber rather than an alcove, and Corollary 3 is about existence and uniqueness and names no map at all.
content_sha256: 155154fc71627ae3dcd4cdbf99bb0f882a72e82a1f166f29c76f3852c49da526
translated_from: content/en/lie/IX/09_s9_compact_lie_groups_operating_on.md
translation_method: google
source_content_sha256: dbd6a8fe77e36a2dde3d4d956d5fc6fd2a6bf284a5e6f34dca83531dabcebd7f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 0a1863b474fa0ae484f27bea1b6c459e391cacbf4571fe0f827d1247bd24c4df
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 9。 作用的紧李群开流形

在本段中，X表示类$C^r(1\leq r\leq \omega )$的分离的局部有限维实数流形。

### 1. 将流形嵌入到紧集的邻域中

#### 引理 1 {#lie-ix-s9-lem-1 .statement tag=01HE}

设T和$T'$为两个拓扑空间，T和$T'$分别为A和$A'$紧子集，$T\times T'$中$A\times A'$的W邻域。在 T 中存在 A 的开邻域 U，在 $T'$ 中存在 $A'$ 的开邻域 $U'$，使得 $U\times U'\subset W$。

令 $x\in A$；存在T的开子集$U_x$和$T'$的$U'_x$，使得$\{x\} \times A'\subset U_x\times U'_x\subset W:$确实，$T\times T'$的紧子集$\{x\} \times A'$可以被包含在W中的开集合的有限数覆盖， 形式$U_i\times U'_i$，含$x\in U_i$；取$U_x=\bigcap_iU_i$和$U'_x=\bigcup_iU'_i$就足够了。

由于 A 是紧的，因此 A 存在点 $x_1, . . . , x_m$，使得 $A\subset \bigcup_iU_{x_i}$；输入$U =\bigcup_iU_{x_i}$和$U'=\bigcap_iU'_{x_i}$。然后$A\times A'\subset U\times U'\subset W$，因此引理。

在这个数的剩余部分中，Y表示类$C^r$的分离的流形。

#### 命题 1 {#lie-ix-s9-prop-1 .statement tag=01HF}

令$\varphi : X\rightarrow Y$为类$C^r$的态射，A是X的紧致子集。以下条件是等效的：

(i) $\varphi$ 的限制对 A 是单射的，$\varphi$ 是 A 的每点处的浸没；

(ii) A 存在一个开放的邻域 U，使得 $\varphi$ 诱导将 U 嵌入到 Y 中。

当满足这些条件时，$\varphi$被称为A的邻域的嵌入。

我们证明 (i) 蕴涵 (ii)，另一个蕴涵是明确的。假设 (i)，存在 X 包含于 A 的开放邻域 V，使得 $\varphi$ 到 V 的限制是浸没（可微分和解析流形，结果，5.7.1）。用$V\times V$中点$(x, y)$的$\Gamma$集合表示，使得$\varphi (x) =\varphi (y)$，并用$\Delta$表示$V\times V$中的对角线。那么$\Delta$确实是$\Gamma :$的开子集，对于所有$x\in V$，存在$x$的开邻域$U_x$，使得$\varphi$到$U_x$的限制是单射的，即，这样 $\Gamma \cap (U_x\times U_x) =$ $\Delta \cap (U_x\times U_x)$。

由于Y是分离的，$\Gamma$在$V\times V$中闭；因而 $V\times V$ 中$\Gamma$ **--** $\Delta$ 的补集 W 是开集。 假设出发，西包含$A\times A$； 引理 1 意味着存在V 包含于 A 的开子集 $U'$，使得$U'\times U'\subset W$，即$\varphi$ 到$U'$ 的限制是单射的。此外，存在 A 的开邻域 U，其闭包是紧的，并且包含在$U'($一般拓扑，第 1 章中。 I, §9, no. 7，提案 10）。那么 $\varphi$ 诱导从 U 到 $\varphi$(U) 的同胚，因此从 U 到 $\varphi (U)$；由此可见，$\varphi$到U的限制是一个嵌入（可微分和解析流形，结果，5.8.3）。

#### 命题 2 {#lie-ix-s9-prop-2 .statement tag=01HG}

假设流形 Y 是仿紧的；设A为X的子集，并令$\varphi :X\rightarrow Y$为类$C^r$的态射，诱导从A到$\varphi (A)$的同胚，并且在A的每个点处都是étale。那么存在一个开A 的邻域 U，使得 $\varphi$ 诱导同构从 U 到 Y 的开子流形。

如有必要，限制X和Y，我们可以假设$\varphi$是étale和满射的。用$\sigma :\varphi (A)\rightarrow A$表示$\varphi |A$的逆同胚。由于 Y 是可度量的（可微且解析流形，结果，5.1.6），$\varphi (A)$ 承认仿紧凑邻域的基本系统；因而，将军拓扑，第。 XI，Y 中存在$\varphi (A)$的开邻域V和连续映射$s: V\rightarrow X$，重合与$\sigma$在$\varphi (A)$上，且对于所有$\varphi (s(y)) =y$ $y\in V$。此外，$s$在拓扑上是étale的，所以$s(V)$是开集合U包含A。那么$\varphi$诱导是从U到V的同胚$\varphi '$；通过可微分和解析流形，结果$, 5.7.8,\varphi '$为同构。

在这个数的剩余部分，我们假设$r\not=\omega$。

#### 命题 3 {#lie-ix-s9-prop-3 .statement tag=01HH}

令 A 为 X 的紧凑子集。作为A的邻域中的嵌入的态射$\varphi \in \mathscr{C}^r(X;Y)$的集合$\mathscr{P}$在紧凑$C^r$收敛(§ 6, no. 4)的拓扑中的$\mathscr{C}^r(X;Y)$中是开放的。

显然，只要证明命题就足以证明$r= 1$。

a) 我们首先证明$\mathscr{C}^1(X;Y)$由……组成或态射的子集J是A的每个点的浸没点是开路的。考虑映射 $j_A:\mathscr{C}^1(X;Y)\times A\rightarrow J^1(X;Y)$，使得 $j_A(\varphi , x) =j_x^1(\varphi ) ($可微且可解析流形，结果，12.1）。

由$\mathscr{C}^1$(X;Y)上拓扑的定义，从$\mathscr{C}^1(X;Y)$到$\mathscr{C}(A;J^1(X;Y))$连续映射$\widetilde{j}_A:\varphi \rightarrow j_A(\varphi , .)$；现在它来自将军拓扑，第 1 章。 X, §3, no. 4，周四。 3、$j_A$是连续的。

另一方面，令 M 为 $J^1(X;Y)$ 中射流 $j$ 的集合，其切线映射 $T(j) : T_{\mathbf{s}(j)}(X)\rightarrow T_{\mathbf{b}(j)}(Y) ($可微且解析流形，结果，12.3.4) 是单射的。 集合 M $J^1(X;Y)$ 开放；事实上，当X是有限维向量空间E的开子集，并且Y是Banach空间F的开子集时，足以验证这个断言；然后，我们将（可微分和解析流形，结果，12.3.1）减少到证明，单射连续线性映射的集合在$\mathscr{L}$（E;F）中开放，这是从谱理论，第1章得出的。 III, §2, no. 7，提案 16。

我们从前面的结论得知集合$j_A^{-1}(M)$在$\mathscr{C}^1(X;Y)\times A$中开，因此它的补集$\mathscr{F}$是闭的。由于 A 是紧的，投影 pr$_1:\mathscr{C}^1(X;Y)\times A\rightarrow \mathscr{C}^1(X;Y)$ 是真态射，因此是闭集；因而，集合 J 等于 $\mathscr{C}^1(X;Y)$ **--** pr$_1(\mathscr{F})$，在 $\mathscr{C}^1(X;Y)$ 打开。

b) 令 H 为 $J\times A\times A$ 由……组成或元素 $(f, x, y)$ 的子集，使得 $f(x) =f(y)$。显然，H包含$J\times \Delta$，其中$\Delta$表示乘积$A\times A$中的对角线；我们证明 $H'= H$ **--** $(J\times \Delta )$ 在 $J\times A\times A$ 中闭合。由于$\mathscr{P}$是$H'$在J中的像的补集，在适当的投影pr$_1: J\times A\times A\rightarrow J$下，这将意味着命题。

$\mathscr{C}^1(X;Y)$的拓扑是更细比紧凑收敛的拓扑，从$\mathscr{C}^1(X;Y)\times A$到Y的映射$(\varphi , x) \rightarrow \varphi (x)$是连续的（一般拓扑，第X, §3, no. 4章，第3章的Cor.1）；由此可见，H 在 $J\times A\times A$ 是封闭的。因此，只要证明$J\times \Delta$在H中开，在其他字中，对于所有$\varphi \in J$和所有$x\in A$，存在J中$\varphi$的邻域$\Omega$和$x$中的邻域B X，使得对于$\Omega$中的任何态射$\psi$，$\psi$到$A\cap B$的限制是单射的。

因此，命题由以下引理推出：

#### 引理 2 {#lie-ix-s9-lem-2 .statement tag=01HI}

令$x$为X$,\varphi : X\rightarrow Y$态射或类$C^1$的点，这是$x$的浸没。 $\mathscr{C}^1(X;Y)$ 中存在 $\varphi$ 的邻域 $\Omega$，X 中存在 $x$ 的邻域 B，因此，对于所有 $\psi \in \Omega$，$\psi$ 的限制对 B 是单射的。

令 U 为 $x$ 的相对紧开邻域，同构于有限维向量空间，并且$\varphi (U)$包含在图表的域V中。 $\psi \in \mathscr{C}^1(X;Y)$的集合$\Omega_0$使得$\psi (U)\subset V$在$\mathscr{C}^1$(X;Y)中开路，并且限制映射$\Omega_0\rightarrow \mathscr{C}^1(U;V)$是连续的；因此，当X = U且Y = V时，我们被简化为证明引理，在其他字中，我们可以假设X是有限维向量空间，Y是Banach空间。 选择范数于 X 和 Y。

线性映射 $D\varphi (x) : X\rightarrow$ Y 是单射的；用 $q($谱理论，第 1 章表示它的conorm。 III, §2, no. 6），这样到定义时，我们就有了所有 $t\in X$ 的 $\|D\varphi (x).t\| \geq q\|t\|$。令$\varepsilon \in \mathbf{R}$使得$0< \varepsilon  < q/2$，并令B是具有中心$x$的闭球，使得$\|D\varphi (u)-D\varphi (x)\| \leq \varepsilon$对于所有$u\in B$。用态射$\psi$的$\mathscr{C}^1(X;Y)$由……组成的$\Omega$子集表示，使得$\|D\psi (u)-D\varphi (u)\| \leq \varepsilon$对于所有$u\in B$； $\mathscr{C}^1(X;Y)$拓扑定义开放。对于$\psi \in \Omega$，输入$\psi_0=\psi -D\varphi (x)$。我们对所有 $u\in B$ 有 $\|D\psi_0(u)\| \leq 2\varepsilon$，因此对 B 中的所有 $u$ 和 $v$ 有$\|\psi_0(u)-\psi_0(v)\| \leq 2\varepsilon \|u-v\|$（可微分和解析流形，结果，2.2.3）。由此可见

$$
\|\psi (u)-\psi (v)\| \geq  \|D\varphi (x).(u-v)\| - \|\psi_0(u)-\psi_0(v)\| \geq (q-2\varepsilon )\|u-v\|
$$

因而，$\psi$到B的限制是单射的，因此引理。

#### 命题 4 {#lie-ix-s9-prop-4 .statement tag=01HJ}

令 A 为 X 的紧凑子集。存在有限维向量空间 E 和态射 $\varphi \in \mathscr{C}^r(X;E) (r\not=\omega )$，它是 A 的邻域中的嵌入。

令 $(U_i, \varphi_i,E_i)_{i\in I}$ 为 X 的有限图族，其域涵盖 A。 我们通过将$\varphi_i(x) = 0$替换为$x \notin U_i$，将扩展$\varphi_i$到映射从X到$E_i$（也用$\varphi_i$表示）。 Let $(V_i)_{i\in I}$ be a covering of A by open subsets of X such that $\overline{V}_i\subset U_i$ for all $i\in I$ (the existence of such a covering follows from General Topology, Chap. IX, §4, no. 3, Cor. 1 of Th. 3, applied to the compact space $X'$ obtained by adjoining to X a point at infinity and the covering of $X'$ consisting of the open sets $U_i(i\in I)$ and $X'$ **--** A). 对于所有$i\in I$，令$\alpha_i$为X上类$C^r$的数值函数，在$V_i$的每个点等于1，并在$U_i($可微分和解析流形，结果中包含支持， 5.3.6）。

考虑映射 $\varphi : X\rightarrow \bigoplus_{i\in I}(E_i\oplus \mathbf{R})$ 定义为

$$
\varphi (x) = (\alpha_i(x)\varphi_i(x), \alpha_i(x))_{i\in I}
$$

对于所有$i\in I$，映射$\alpha_i\varphi_i$是类$C^r$（因为它的限制到$U_i$以及$\alpha_i$的支持补集），并且它的限制到$V_i$是一个嵌入；由此可见，$\varphi$是类$C^r$的态射，并且是A的每个点处的浸没。我们证明$\varphi$的限制对A是单射的。令$x, y$是A的两个点，使得$\varphi (x) =\varphi (y)$，并令$i\in I$使得$x\in V_i$。那么$\alpha_i(x) = 1$，所以$\alpha_i(y) = 1$，这意味着$y\in U_i$；但我们也有 $\varphi_i(x) =\varphi_i(y)$，所以从 $\varphi_i$ 诱导开始，$x=y$ 将 $U_i$ 嵌入到 $E_i$ 中。

可以证明$^9$，每个分离的流形，可数无穷大且

纯维数$n$，嵌入$\mathbf{R}^{2n}$；对于较弱的结果，cf. 习题 2。

$^9$ 参见 H. WHITNEY，平滑 $n$ 流形在 $2n$ 空间中的自交，

安.数学，45 (1944)，第 220-246 页。

### 2. 等变嵌入定理

在这个数中，我们假设$r\not=\omega$。

#### 引理 3 {#lie-ix-s9-lem-3 .statement tag=01HK}

设 G 是在拓扑空间 X 上连续运行的紧拓扑群；设A为X的子集，在G下稳定，且A的W邻域。则存在A在G下稳定且包含在$_{\circ}W$中的开邻域V。

设 F = X **--** W 和 V = X**--** GF。那么V是开放的（一般拓扑，第III, §4, no. 1章，第1号提案的Cor.1），在G下稳定，并且$A\subset V\subset W$。

#### 定理 1 {#lie-ix-s9-thm-1 .statement tag=01HL}

设G为X上G的类$C^r$左运算的紧李群，$(g, x) \rightarrow gx$律，A为X的紧凑子集。在有限维向量空间 E 上存在 G 的解析线性表示 $\rho$，类 $C^r$ 的态射 $\varphi : X\rightarrow E$，与 G 的运算兼容，以及 A 的开邻域 U，在 G 下稳定，使得 $\varphi$ 到 U 的限制是嵌入。

替换 A 通过紧集 GA，我们被简化为 A 在 G 下稳定的情况。

令$E_0$为有限维向量空间，使得存在$\mathscr{C}^r(X;E_0)$的元素，它是A的邻域中的嵌入（no. 1，命题4）； 态射的集合$\mathscr{P}$有这个性质是$\mathscr{C}^r(X;E_0)$的非空开子集（no. 1，命题3）。考虑紧致群 G 在空间 $\mathscr{C}^r(X;E_0) ($§6, no. 4、引理 4) 上的连续线性表示。根据 Peter-Weyl 定理（谱理论，准备中），G 下稳定的有限维子空间的并在 $\mathscr{C}^r(X;E_0)$ 是稠密的；因此，存在$\mathscr{P}$的元素$\varphi_0$使得映射$x \rightarrow \varphi_0(gx)$，对于$g\in G$，生成有限维向量子空间$E_1$ $\mathscr{C}^r(X;E_0)$，在G的运算下显然是稳定的。

取E为空间Hom$_{\mathbf{R}}(E_1,E_0),\rho$为$E_1$上作用诱导的G在E上的表示，$\varphi : X\rightarrow E$为与$x\in X$线性映射相关联的映射 $\psi  \rightarrow \psi (x)$从$E_1$到$E_0$。这是类$C^r$中的态射；对于$x\in X,g\in G,\psi \in E_1$，我们有（用X的$\tau (g)$自同构$x \rightarrow gx$表示）：

$$
\varphi (gx)(\psi )-\psi (gx) =\varphi (x)(\psi \circ \tau (g)) = (\rho (g)\varphi (x))(\psi )
$$

令 $\alpha :$ Hom$_{\mathbf{R}}(E_1,E_0)\rightarrow E_0$ 为线性映射 $u \rightarrow u(\varphi_0)$；我们有$\alpha \circ \varphi =\varphi_0$，所以$\varphi$是A的邻域的嵌入，因为$\varphi_0$是一。因此，存在 A 的开邻域 U，使得 $\varphi$ 的限制到 U 是一个嵌入；我们可以通过引理 3 使选择 U 在 G 下稳定，因此定理。

#### 推论 1 {#lie-ix-s9-thm-1-cor-1 .statement tag=01HM}

假设 X 是紧致的。在有限维向量空间 E 上存在 G 的解析线性表示 $\rho$ 和嵌入 $\varphi : X\rightarrow E$，使得 $\varphi (gx) =\rho (g)\varphi (x)$ 对应于 $g\in G, x\in X$。

#### 推论 2 {#lie-ix-s9-thm-1-cor-2 .statement tag=01HN}

设 H 是 G 的闭子群。在有限维向量空间 E 和点 $v\in E$ 上，存在固定器 H 的 G 解析线性表示。

适用 Cor. 1 到紧致流形 $G/H$ 上 G 的规范运算。这给出了解析线性表示 $\rho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ 和嵌入 $\varphi : G/H\rightarrow E$，使得$\varphi (gx) =\rho (g)\varphi (x),g\in G, x\in G/H$。设$\overline{e}\in G/H$为$e\in G$的类，$v=\varphi (\overline{e})$为像。对于所有 $g\in G$，我们有 $\rho (g)v=v\Leftarrow \Rightarrow \varphi (g\overline{e}) =\varphi (\overline{e})\Leftarrow \Rightarrow g\overline{e}= \overline{e}\Leftarrow \Rightarrow g\in H$。

#### 推论 3 {#lie-ix-s9-thm-1-cor-3 .statement tag=01HO}

假设 X 是仿紧的。存在实希尔伯特空间 E、E 上 G 的连续酉表示 $^{10}\rho$ 以及类 $C^r$ 的嵌入$\varphi : X\rightarrow E$，使得$\varphi (gx) =\rho (g)\varphi (x)$ 对于所有$g\in G$ 和所有$x\in X$。

空间 $X/G$ 是局部紧致的（一般拓扑，第 III, §4, no. 5 章，第 11 条命题）。 其连通分量是X连通分量的像，无穷大可数（通论拓扑，第I, §9, no. 10，第5章）；因此，它们本身在无穷大处是可数的，这意味着$X/G$是仿紧的（loc.cit.）。 Hence, there exists a locally finite covering $(U'_{\alpha})_{\alpha\in I}$ of $X/G$ by relatively compact open sets, and a covering $(V'_{\alpha})_{\alpha\in I}$ such that $\overline{V}'_{\alpha}\subset U'_{\alpha}$ for all $\alpha \in I ($General Topology, Chap. IX, §4, no. 3, Cor. 1 of Th. 3); taking the inverse image, we obtain two locally finite coverings $(U_{\alpha})_{\alpha\in I}$ and $(V_{\alpha})_{\alpha\in I}$ of X by relatively compact open sets stable under G, such that $\overline{V}_{\alpha}\subset U_{\alpha}$ for all $\alpha \in I$.

对于所有$\alpha \in I$，在有限维实数向量空间$E_{\alpha}$和态射$\varphi_{\alpha}\in \mathscr{C}^r(X;E_{\alpha})$上存在G的表示$\rho_{\alpha}$，与G的运算兼容，其限制到$U_{\alpha}$是嵌入（Th. 1）。对于$\alpha \in I$，令$a_{\alpha}$为X上类$C^r$的数值函数，在$V_{\alpha}$上等于1，在$U_{\alpha}($可微分和解析流形之外等于0，结果，5.3.6）。将 $b_{\alpha}(x) =\int_Ga_{\alpha}(gx)dg$ 替换为 $x\in X$。 函数$b_{\alpha}$属于类$C^r$，在G下不变（§6, no. 4，Cor.2），在$V_{\alpha}$上等于1，在$U_{\alpha}$之外等于0。给每个$E_{\alpha}$一个G（§1, no. 1）下的希尔伯特标量乘积不变量，以及$\mathbf{R}$其规范希尔伯特结构；令E为族$(E_{\alpha}\oplus \mathbf{R})_{\alpha\in I}$的希尔伯特和，并令$\rho$为G在E上的表示，由$\rho_{\alpha}$和G在$\mathbf{R}$上的平凡作用引起。对于$x\in X$，输入$\varphi (x) = (b_{\alpha}(x)\varphi_{\alpha}(x), b_{\alpha}(x))_{\alpha\in I}$。那么$\varphi$从X到E就是类$C^r$的态射，兼容G的运算；我们按照命题 4 的证明 (no. 1) 验证$\varphi$ 是一个嵌入，这意味着推论。

$^{10}$即（谱理论，准备中）连续线性表示（积分，第VIII, §2, no. 1），使得算子$\rho (g)$对于所有的都是酉的

$$
g\in G
$$

### 3. 管与横截面

#### 引理 4 {#lie-ix-s9-lem-4 .statement tag=01HP}

令 H 为紧李群，$\rho : H\rightarrow \mathbf{G}\mathbf{L}(V)$ H 在有限维实数向量空间上的连续（因此是解析的）表示，以及 V 中原点的 W 邻域。存在原点的开邻域 B，包含在 W 中并在 H 下稳定，以及解析同构 $u: V\rightarrow B$，与 H 的运算兼容，使得 $u(0) = 0$ 和 $Du(0) =$ Id$_V$。

选择 H (§1, no. 1) 下 V 不变量上的标量乘积。存在实数$r >0$，使得半径为$r$的开球B包含在W中；它在 H 下显然是稳定的。对所有 $v\in V$ 放置 $u(v) =r(r^2+\|v\|^2)^{-1/2}v$；则$u$是从V到B的双射解析映射，与H的运算兼容，并且其逆映射$w \rightarrow r(r^2- \|w\|^2)^{-1/2}w$是解析的。此外，$u(0) = 0$和$Du(0) =$Id$_V$。

#### 命题 5 {#lie-ix-s9-prop-5 .statement tag=01HQ}

设H为X上H的紧李群、类$C^r$左运算$(h, x) \rightarrow hx$律，以及X固定下的$x$点 H 的运算。则群 H 在向量空间 $T = T_x(X)$ 上线性运算；存在类$C^r$的开放嵌入$\varphi : T\rightarrow X$，与H的运算兼容，使得$\varphi (0) =x$和$T_0(\varphi )$是T的身份映射。

令$(U, \psi ,E)$为X在$x$的图表，使得U在H（no. 2，引理3）下稳定且$\psi (x) = 0$。 认同 E 与 T 乘以$T_x(\psi )$，并把

$\psi^{\sharp}(y) =\int_Hh.\psi (h^{-1}y)dh$ 为 $y\in U$，

其中 $dh$ 是总质量 1 的 H 的哈尔测度。

那么(§6, no. 4，Cor.$1$)$\psi^{\sharp}$是从U到T的类$C^r$的态射，与H的运算兼容，使得$\psi^{\sharp}(x) = 0$和$d_x\psi^{\sharp}=$Id$_T$。因此，T 中存在开集合 $U'\subset U$ 包含 $x$，以及开邻域 V 0，使得$\psi^{\sharp}$ 诱导同构 $\theta : U'\rightarrow V$。如果必要的话限制$U'$和V，我们可以假设它们在H下是稳定的，并且存在与H的运算兼容的同构$u: T\rightarrow V$（引理4）。现在拿$\varphi =\theta^{-1}\circ u$就够了。

回想一下（可微分和解析流形，结果，6.5.1），如果 G 是李群，H 是 G 和 Y 流形的谎言子群，H 在左侧进行运算，我们用 $G\times^HY$ 表示乘积流形的商$G\times Y$ 在 H 的右侧运算 $((g, y), h) \rightarrow (gh, h^{-1}y)$；这是流形，李群 G 自然在左边运算； 投影 $G\times^HY\rightarrow G/H$ 是具有纤维 Y 的丛。此外，如果 Y 是 H 线性运算的有限维向量空间，则 $G\times^HY$ 具有自然结构向量 G 丛，其中基 $G/H ($ 可微且解析流形，结果，7.10.2）。

令 G 为李群在流形 X 上正确运行（一般拓扑，第 III, §4, no. 1，定义 1），使得运算 $(g, x) \rightarrow gx$ 的律为类 $C^r$。那么，对于X的每个点$x$，$x$的轨道$Gx$是X的闭子流形，同构于李齐次空间$G/G_x$，其中$G_x$ 是 G 中 $x$ 的固定器（cf. 第 III, §1, no. 7 章，第 14 (ii) 条提案，以及一般拓扑，第 III, §4, no. 2 章，第 4 条提案）；这是紧李群（前述）。

#### 命题 6 {#lie-ix-s9-prop-6 .statement tag=01HR}

假设流形 X 是仿紧的；设$x$为X的点，$G_x$为其固定器。存在有限维解析线性表示$\tau : G_x\rightarrow \mathbf{G}\mathbf{L}(W)$，以及类$C^r$的开放嵌入$\alpha : G\times^{G_x}W\rightarrow X$，与G的运算兼容，$(e,0)\in G\times W$的映射类 $x$。

把$T = T_x(X)$。令W为T中$T_x(Gx)$的补子空间，在$G_x$下稳定（对于例，$T_x(Gx)$相对于$G_x$下T不变量上的标量乘积的正交补）。另一方面，令 $\varphi : T\rightarrow X$ 为态射，具有第 5 条中所述的属性（相对于 $H = G_x$）。考虑由 $\lambda (g, w) =g\varphi (w)$ 定义的态射 $\lambda : G\times W\rightarrow X$。将诱导通过类$C^r$的商态射$\mu: G\times^{G_x}W\rightarrow X$，与G的运算兼容，将$(e,0)$的映射类$z$得$x$。

我们证明 $\mu$ 是点 $z$ 的 étale。我们有

暗淡(G $\times^{G_x}W$) $=$ 暗淡(G) + 暗淡(W) $-$ 暗淡(G$_x$)

= 暗淡(G$x$) $+$ 暗淡(W) = 暗淡(T),

因此只要证明$\mu$在$z$处是淹没的，或者等效地$\lambda$在$(e,0)$处是淹没的。 But, the tangent 映射 $T_{(e,0)}(\lambda ) : T_e(G)\oplus W\rightarrow T$ is equal to $T_e(\rho (x)) +i$, where $\rho (x)$ is the orbital 映射 $g \rightarrow gx$ and $i$ 典范嵌入 from W to T; since Im $T_e(\rho (x)) = T_x(Gx)$, 映射 $T_{(e,0)}(\lambda )$ is surjective, and $\mu$ is étale at $z$.

我们将证明$G\times^{G_x}W$中存在$Gz$的开邻域$\Omega$，在G下稳定，使得$\mu$诱导同构从$\Omega$到X的开子集。这意味着命题：事实上，$G\times W$中$\Omega$的逆像在G下是稳定的，因此是形式$G\times B$，其中B是W包含原点的开子集并且在$G_x$下稳定；如果需要限制$\Omega$，我们可以假设存在同构$u: W\rightarrow B$，与$G_x$（引理4）的运算兼容。显然，复合态射$\alpha : G\times^{G_x}W\overset{(Id,u)}{\longrightarrow}G\times^{G_x}B\longrightarrow^\mu$X在命题的叙述中满足条件。

因此，命题是以下引理的推论：

#### 引理 5 {#lie-ix-s9-lem-5 .statement tag=01HS}

设Z为类$C^r$的分离流形，配备类$C^r$的左运算$m: G\times Z\rightarrow Z$的律，以及$\mu: Z\rightarrow X$态射（类） $C^r$）与G的运算兼容。令$z$为Z的点，且$x=\mu(z)$。假设$\mu$在$z$处是étale，并且G中$z$的固定器等于$x$的固定器$G_x$。那么，存在轨道$Gz$的开邻域$\Omega$，在G下稳定，使得$\mu$诱导同构从$\Omega$到X的开子集。

由于$\mu$与G的运算兼容，因此在$Gz$的每个点都是étale；由于规范的映射 $G/G_x\rightarrow Gx$ 是同胚，因此由 $\mu$ 引发的从 $Gz$ 到 $Gx$ 的映射也是同胚。因此，根据no. 1的命题2可知，Z中存在$Gz$的开放邻域U，使得$\mu$诱导U到X的开放嵌入。

由于G在X上正确运行，因此存在$x$的开邻域V和G的紧子集K，使得$gV\cap V =\emptyset$对于$g \notin K ($一般拓扑，第1章。 III, §4, no. 4，提案 7)；特别是$e\in K$。 点 $y\in Z$的集合 $W_1$，使得$Ky\subset U$在Z中开：确实，Z**--** $W_1$是闭集合 $(K\times Z)$ **--** $m^{-1}(U)$在适当的条件下的像投影 pr$_2: K\times Z\rightarrow Z$。把$W = W_1\cap \mu^{-1}(V)$；这是 Z 的开子集、包含 $z$ 和满足以下条件：

(i) KW $\subset U$，特别是$W\subset U$；

(ii) $\mu(W)\subset V$。

放入$\Omega =$ GW，并考虑$\mu$到$\Omega$的限制。 这是一个étale 态射，因为$\Omega$的每个点都是G到U的点下的共轭。 我们证明它是单射的：设 G 中的 $g, h$ 和 W 中的 $u, v$ 使得 $\mu(gu) =$ $\mu(hv)$。 把$k=g^{-1}h$；然后 $\mu(u) =k\mu(v)$，所以 $k\in K$ 由 (ii) 得到。 但是 $kv$ 和 $u$ 属于通过 (i) 到 U；因而，$u=kv$因为$\mu$到V的限制是单射的，所以$gu=hv$。 因而，$\mu$到$\Omega$的限制是单射的，因而（可微分和解析流形，结果，5.7.8）是同构到X的开子流形上，从而完成证明。

根据第6条的条件，$\alpha$的像是$x$的轨道A的开放邻域T，配备向量丛的结构和基A，其中零截面是轨道 A 本身。这样的邻域称为线性管（大约在所讨论的轨道附近）。对于每个点$a\in A$，该向量丛的纤维$Y_a$是X的子流形，在$a$的固定器$G_a$下稳定，并且使得态射从$G\times^{G_a}Y_a$到X $(g, y)\in G\times Y_a$ 的映射类到 $gy\in X$ 诱导态射类 $C^r$ 从 $G\times^{G_a}Y_a$ 到 T。然后 $Y_a$ 被认为是在 $a$ 处的横截面管 T. 我们注，$Y_a$在$a$处的切线空间与$Y_a$正则同构，并且它是$T_a(X)$中$T_a(A)$的补集；因而，向量丛 T 与基 A 与 X 中 A 的正规丛规范同构（可微分和解析流形，结果，8.1.3）。

### 4. ORBIT TYPES

设G是在分离拓扑空间E上连续运行的拓扑群。对于E的每个点$x$，用$G_x$表示G中$x$的固定器，并假设规范映射$G/G_x\rightarrow Gx$是同胚；在以下两种情况下尤其如此：

a) G和E的拓扑是离散的；

$b) G$ 在 E 上正确运行（通则拓扑，第 III, §4, no. 2，命题 4），对于例，G 是紧致的（通则拓扑，第 III, §4, no. 1，命题 2）。

用G的闭子群的共轭类的$\mathscr{T}$集合表示。对于每个$x\in E$，我们称$x$的轨道型，或$x$的有时型， $\mathscr{T}$中$G_x$的类；相同的轨道中的两个点具有相同的轨道型（代数，第 I, §5, no. 2 章，第 2 条）；两个轨道具有相同的型当且仅当它们与 G 集同构（代数，第 I, §5, no. 5，第 1 章）。对于每个$t\in \mathscr{T}$，用型$t$E点$E_{(t)}$集合表示，即型$t$轨道并；这是E的稳定子集。对于$H\in t$，我们也将$E_{(t)}$写成$E_{(H)}$；对于例，$E_{(G)}$ 是由 G 确定的点的 E 由……组成的闭子空间。

给$\mathscr{T}$以下预序关系：

$t\leq t'\Leftarrow \Rightarrow$ 存在$H\in t$ 和$H'\in t'$ 使得$H\supset H'$。

设$\Omega$和$\Omega '$是G在$E,t$和$t'$其型上的两个轨道；那么 $t\leq t'$ 当且仅当存在从 $\Omega '$ 到 $\Omega$ 的 G 态射（必然是满射且连续的）。

Let $x, x'$ be in E, and $t, t'$ their types; then $t\leq t'$ if and only if there exists $a\in G$ such that $aG_{x'}a^{-1}\subset G_x$.

#### 引理 6 {#lie-ix-s9-lem-6 .statement tag=01HT}

设G为李群。

a) G 的紧凑子群的每个递减序列都是平稳的。

b) 令H和$H'$是G的两个紧子群，使得$H\subset H'$并且存在从$H'$到H的同构（拓扑群）。然后是$H = H'$。

c) 对于关系 $t\leq t'$，集合 $\mathscr{T}$ 是诺特有序的集合（集合论，第 III, §6, no. 5 章，第 7 条提案之前的文本）。

a) 设$(H_i)_{i\geq 1}$为G的紧致子群的递减序列；这些是 G 的谎言子群（第 III, §8, no. 2 章，第 2 章）。 整数（暗淡$H_i$）$_{i\geq 1}$的序列是递减，因此是平稳的，因此存在整数 N，使得子群$H_i$对于$i\geq N$具有相同的恒等分量。那么正整数 $(H_i: (H_i)_0)_{i\geq N}$ 的递减序列是平稳的，因此 $H_i= H_{i+1}$ 对于 $i$ 足够大。

b) 设$f$是从$H'$到H的同构。序列$(f^n(H))_{n\geq 0}$是G的紧致子群的递减序列，所以$f^n(H) =f^{n+1}(H)$对于$n$足够大，通过a)。由于$f$是同构，这意味着$f(H) = H =f(H')$，所以$H = H'$。

c) 令$t, t'\in \mathscr{T}$满足$t\leq t'$和$t'\leq t$。那么，存在$H,H_1\in t$和$H',H'_1\in t'$使得$H\supset H'$和$H_1\subset H'_1$。令$g$和$g'$是G的两个元素，使得$H_1=gHg^{-1}$和$H'_1=g'H'g^{'-1}$；输入$u=g^{'-1}g$。然后

$$
uHu^{-1}\subset H'\subset H
$$

由b)，这意味着$uHu^{-1}= H$，因此$H'= H$和$t'=t$。因此，集合$\mathscr{T}$是有序的，并且由a)得到诺特。

#### 定理 2 {#lie-ix-s9-thm-2 .statement tag=01HU}

令G为李群在X上正常运行，使得运算$(g, x) \rightarrow gx$的律为类$C^r$。假设 X 是仿紧的。

a) The map which associates to any point of X its orbit type has the following semi-continuity property: let $x\in X$ and let $t\in \mathscr{T}$ be its orbit type; there exists a stable open neighbourhood U of $x$ such that, for any $u\in U$, the type of $u$ is $\geq t$.

b) 对于所有$t\in \mathscr{T},X_{(t)}$是X的子流形，由G的运算诱导的$X_{(t)}$上的等价关系是正则的（可微分和解析流形，结果，5.9.5），并且态射$X_{(t)}\rightarrow X_{(t)}/G$是一个丛。

c) 假设$X/G$已连接。则X元素轨道型集合有最大的元素$\tau$；而且，$X_{(\tau)}$是X的密集开子集，并且$X_{(\tau)}/G$是连通的。

令$x$为X的点，$t\in \mathscr{T}$为型。为了证明a)和b)，我们可以通过稳定开集合包含$x$来替换X，因此（命题6）可以假设X是形式$G\times^HW$，其中W是有限维的空间 G 的紧致子群 H 的解析线性表示，在规范投影 $p: G\times W\rightarrow G\times^HW$ 下，点 $x$ 是 $(e,0)\in G\times W$ 的像 $p(e,0)$。如果$u=p(g, y)\in G\times^HW$和$a\in G$，则$au=u$当且仅当存在$h\in H$和$(ag, y) = (gh^{-1}, hy)$，即如果$a\in gH_yg^{-1}$。因此，$G_u=gH_yg^{-1}$；特别是$G_x= H$，所以$G_u$是$G_x$的共轭到子群，这证明$u$的型是$\geq t$，因此a)。

此外，$u$是型$t$当且仅当$G_u$对于G中的H是共轭，或者等价地$H_y$对于G中的H是共轭；由引理$6b)$，这意味着$H_y= H$，因而$y$由H固定。如果$W'$是由H固定的元素的W由……组成的向量子空间，那么$X_{(t)}$可以被识别为$G\times^HW'$，因此也有 $G/H\times W'$，因而 b)。

为了证明 c)，观察 $X/G$ 连接的假设意味着 X 是有限维的纯值：事实上，对于所有 $k\geq 0$，用点 $x\in X$ 的 $X_k$ 集合表示，使得暗淡$_xX =k$；则$X_k$在X开闭，且在G下稳定，所以X等于$X_k$之一。

现在我们通过X的维数上的归纳，断言对于昏暗的X = 0是清楚的。设$\tau$为点的轨道型中的极大元素 X（这样的元素存在于引理$6c$）$)$。我们将证明如下：

$c')$ 对于 $X_{(t)}$ 的每个子集 A，在 $X_{(\tau)}$ 中开闭且在 G 下稳定，则 A 在 X 中的闭包 $\overline{A}$ 是开的。

这个断言意味着c)。事实上，注首先在X中打开$X_{(\tau)}$，由a)； 断言$c')$意味着$\overline{X}_{(\tau)}$在X中开闭，因此等于X，因为它在G下稳定并且$X/G$是连通的。设A是G下$X_{(\tau)}$的非空开闭子集稳定； $c'),\overline{A}$ 在 X 开闭，且在 G 下稳定，因此等于 X；这意味着 A 在 $X_{(\tau)}$ 中是稠密的，因此等于 $X_{(\tau)}$。因而，$X_{(\tau)}/G$的每个非空开闭子集都等于$X_{(\tau)}/G$，这证明$X_{(\tau)}/G$是连通的。最后，由于$X_{(\tau)}$在X中是稠密的，因此从a)可以得出，X的每个点都是型$\leq \tau$；其他字、$\tau$为X点轨道型中的最大的元素。

我们现在证明$c')$。我们可以假设A非空；让$x\in A$。只要证明A是$x$的邻域就足够了。为此，如上所述，我们可以假设$X = G\times^HW$具有H紧凑，$x$是$(e,0)$的典范像。首先假设H对W进行平凡运算：则X可以与$(G/H)\times W$等同，并且$X_{(\tau)}/G = X/G$与W同胚，因此连通；因而，$A/G = X/G$，所以 A = X。从现在起，假设 H 对 W 不进行平凡操作。选择在紧凑群 H 下，W 不变量上的标量乘积；设 S 为 W 中的单位球体（范数向量集合 1）。 注 $S/H$ 是连通的：事实上，如果 dim(W) $\geq 2, S$ 是连通的，并且如果 dim(W) = 1，则 S 是两个点的空间，H 在这两个点上进行了非平凡的运算。把$Y = G\times^HS$；这是余维 1 的 X 的闭子流形，在 G 下稳定，与 $Y/G$ 同胚于 $S/H$，是连通的。因而，到归纳假设，Y 存在最大轨道型 $\theta$，集合 $Y_{(\theta)}$ 在Y 中是开稠密的，并且$Y_{(\theta)}/G$ 是连通的。

考虑X上$\mathbf{R}^*_+$的运算是由$G\times W$上$\mathbf{R}^*_+$的律和运算$(\lambda ,(g, w)) \rightarrow (g, \lambda w)$的商引起的。该运算下的X共轭中的两个点是相同的轨道型；因而，$X_{(\theta)}$包含$\mathbf{R}^*_+Y_{(\theta)}$，这是X的密集开子集。但$X_{(\tau)}$被a)开，因此满足$X_{(\theta)}$，所以$\theta =\tau$。

另一方面，从$\mathbf{R}^*_+\times S$到W **--** $\{0\}($一般拓扑的同态$(\lambda , w) \rightarrow \lambda w$，第1章。 VI, §2, no. 3，命题 3) 诱导从 $\mathbf{R}^*_+\times (S/H)$ 到 $(\mathbf{R}^*_+S)/H$ 的同态，因此也是从 $\mathbf{R}^*_+\times (Y/G)$ 到 $(\mathbf{R}^*_+Y)/G$，以及从 $\mathbf{R}^*_+\times (Y_{(\theta)}/G)$ 到 $(\mathbf{R}^*_+Y_{(\theta)})/G$ 的同态。因而，$(\mathbf{R}^*_+Y_{(\theta)})/G$是连通的，而$X_{(\tau)}/G$（其中包含是连通密集的子集）本身也是连通的（一般拓扑，第I, §11, no. 1，命题1）。因而，A 等于 $X_{(\tau)}$，因此在 X 中是稠密的，并且 A 是 $x$ 的邻域。这样就完成了定理的证明。

Th 中的记号。 $X_{(\tau)}$中的$2c)$、点称为本金，它们的轨道称为本金轨道。如果$x$是X的点，并且如果$G\times^{G_x}W$是X中管围绕$x$的轨道的线性管，点$x$是主要的当且仅当$G_x$ 对 W 的运算很简单，也就是说，如果管是形式 $(G/G_x)\times W$。

#### 例 1 {#lie-ix-s9-n4-exa-1 .statement tag=01HV}

令 G 为连通的紧李群，通过内自同构对自身进行操作。 G 的元素$x$的固定器就是G中$x$的扶正器$Z(x)$；它包含每个最大环面包含$x$。由此可见最大的轨道型$\tau$是G的最大环面的共轭类。开集合$G_{(\tau)}$是G的正则元素的集合 （§5, no. 1，注）。假设 G 是单连通的。则$G_{(\tau)}$等于G的正则元素的集合$G_r$（§5, no. 2，注2）；如果 A 是 $\mathfrak{g}= L(G)$ 的嘉当子代数 $\mathfrak{t}$ 的凹室，则复合映射 $\pi : A\longrightarrow^{exp}G_r\longrightarrow G_r/$Int(G) 是解析流形的同构。事实上，这是同胚（§5, no. 2，Cor. of Prop. 2）；让$a\in A$，通过翻译$\gamma (t)$将$t=$exp$a$和认同$T_t(G)$与$\mathfrak{g}$一起。然后，可以用典范嵌入 $\mathfrak{t}\rightarrow \mathfrak{g}$ 和商映射 $\mathfrak{g}\rightarrow \mathfrak{g}/$Im(Ad $t^{-1}-1$) 的复合来识别正切映射 $T_a(\pi )$。由于 $t$ 是正则，$T_a(\pi )$ 是同构，因此给出了规定的结果（可微分和解析流形，结果，5.7.8）。

#### 例 2 {#lie-ix-s9-n4-exa-2 .statement tag=01HW}

令E为E的超平面的实数欧氏仿射空间、$\mathfrak{H}$集合，W群是E相对于$\mathfrak{H}$的超平面的正交反射产生的位移。假设 $\mathfrak{H}$ 在 W 下稳定，并且群 W 与离散拓扑在 E 上正常运行。

前述可以应用于E上W的运算。E的点$x$的固定器是由$\mathfrak{H}$包含$x$的超平面的反射产生的W的子群（第V, §3, no. 3，道具。） 2）。因而，最大的轨道型$\tau$是子群$\{$Id$_E\}$的类，$E_{(\tau)}$是E室的并。注在这种情况下覆盖$E_{(\tau)}\rightarrow E_{(\tau)}/W$ 是微不足道的，特别是如果 $\mathfrak{H}$ 非空，则$E_{(\tau)}$ 不连通。

### 习题 {#lie-ix-s9-exercises}

参见[习题为 § 9](exercises/s9/)。
