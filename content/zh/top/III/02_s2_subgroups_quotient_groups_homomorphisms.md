---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 2
section_title: Subgroups, quotient groups, homomorphisms homogeneous spaces, product groups
lang: zh
source: top-i-iv
book_pages: 225-242, 298-305
pdf_pages: 0231-0248, 0304-0311
extraction: ocr
subsections:
    - "no": 1
      title: SUBGROUPS OF A TOPOLOGICAL GROUP
      page: 225
      pdf_page: 231
    - "no": 2
      title: COMPONENTS OF A TOPOLOGICAL GROUP
      page: 227
      pdf_page: 233
    - "no": 3
      title: DENSE SUBGROUPS
      page: 228
      pdf_page: 234
    - "no": 4
      title: SPACES WITH OPERATORS
      page: 228
      pdf_page: 234
    - "no": 5
      title: HOMOGENEOUS SPACES
      page: 231
      pdf_page: 237
    - "no": 6
      title: QUOTIENT GROUPS
      page: 232
      pdf_page: 238
    - "no": 7
      title: SUBGROUPS AND QUOTIENT GROUPS OF A QUOTIENT GROUP
      page: 233
      pdf_page: 239
    - "no": 8
      title: CONTINUOUS HOMOMORPHISMS AND STRICT MORPHISMS
      page: 235
      pdf_page: 241
    - "no": 9
      title: PRODUCTS OF TOPOLOGICAL GROUPS
      page: 237
      pdf_page: 243
    - "no": 10
      title: SEMI-DIRECT PRODUCTS
      page: 239
      pdf_page: 245
statements: 46
exercises: 31
content_sha256: 941d8b9549168235f120043f18ca12ff0d6ed59f08ab171c459e52d2c7840c7e
translated_from: content/en/top/III/02_s2_subgroups_quotient_groups_homomorphisms.md
translation_method: google
source_content_sha256: e351a0c8f9f899d8ea24b29a23597820504f125d5656802211af972ada8b6d78
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 0bad4ff69855cd1e2170a76695f8bc62ff4663dd61501a3506dd820cf52738c1
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 2. 子群、商群、同态、均质空间、乘积群

### 1. 拓扑群的子群

设 G 为拓扑群，并设 H 为 G 的子群。通过 (GT')，G 的拓扑在 H 上诱导的拓扑与 H 的群结构兼容。因此在 $H$ 上定义的拓扑群的结构据说是由以下的拓扑“诱导”的$G$。每当我们将$G$的子群$H$视为拓扑群时，总是在考虑这种诱导的结构，除非则明确指出相反。

#### 命题 1 {#top-iii-s2-prop-1 .statement tag=0BHS}

*拓扑群$G$的子群$H$的闭包$\overline{H}$是$G$的子群。如果$H$是$G$的普通子群，那么$\overline{H}$也是。*

如果$a, b \in \overline{H}$则$ab^{-1} \in \overline{H}$，因为映射$(x, y) \to xy^{-1}$在$G \times G$和变换$H \times H$上连续到$H$（章I, § 2, no. 1，定理1）。同理，映射$x \to axa^{-1}$的连续性表明，如果$H$是正规的，那么$\overline{H}$也是正规的。

特别是，仅$G$的单位元素的集合、$\{ e \}$、由……组成的闭包$N$，是$G$的*正常子群*；和 $N = \{ e \}$ 当且仅当 $G$ 是 *Hausdorff* ($\S$ 1, no. 2, 命题 2)。

#### 命题 2 {#top-iii-s2-prop-2 .statement tag=0BHT}

*如果$G$是豪斯多夫拓扑群，则$G$的交换性子群的闭包是$G$的交换性子群。*

由于命题 1，我们可以将极限变为 $H$ 在 $G$ 中稠密的情况。 The continuous functions $xy$ and $yx$ are equal on $H \times H$, and are therefore equal on $G \times G$, by virtue of the principle of extension of identities (Chapter I, § 8, no. 1, Proposition 2, Corollary 1).

#### 命题 3 {#top-iii-s2-prop-3 .statement tag=0BHU}

*令$G$为Hausdorff拓扑群，并令$M$为$G$的任意子集。那么与$M$的每个元素可交换的$G$的元素的集合$M'$是$G$的闭子群。特别是，$G$的中心在$G$关闭。*

对于$M'$是集合$F_m (m \in M)$的交，其中$F_m$是所有$x \in G$的集合，使得$xm = mx$；并且 $F_m$ 闭合（章 I, § 8, no. 1，命题 2）。

#### 命题 4 {#top-iii-s2-prop-4 .statement tag=0BHV}

*令$G$为拓扑群，并令$H$为$G$的子群，其在$H$的点之一局部闭合（章I, § 3, no. 3，定义2）。然后$H$在$G$关闭。*

通过翻译，$H$在其每个点处局部闭合，即$H$在$G$处局部闭合。令$V$为$G$中$e$的对称开邻域，使得$V \cap H$在$V$中闭。若$x \in \overline{H}$，则$xV$满足$H$；如果$y \in xV \cap H$，我们有$x \in yV$，并且$y(V \cap H) = (yV) \cap H$在$yV$关闭。但$x$位于$(yV) \cap H$的闭包中，因此$x \in H$。

#### 推论{#top-iii-s2-n1-cor-1 .statement tag=0BHW}

*拓扑群的子群是开放的当且仅当它具有内部点。每个打开的子群都关闭。*

如果子群 $H$ 有一个内部点，那么通过翻译，$H$ 的所有点都是内部的，因此 $H$ 是开的。推论的第二个断言是命题4的特例。

#### 命题 5 {#top-iii-s2-prop-5 .statement tag=0BHX}

*拓扑群$G$的子群$H$是离散的当且仅当$H$有一个孤立的点。 Hausdorff 群的每个离散子群都是闭集。*

如果$H$是离散的，则$H$的每个点都是孤立的。相反，如果 $H$ 有一个孤立的点，则通过平移，$H$ 的每个点都是孤立的，因此 $H$ 是离散的。如果$H$是离散的并且$G$是Hausdorff，则$e$存在邻域$V$使得$V \cap H = \{e\}$； $\{e\}$ 在 $G$ 闭合，因此 *更不必说* 在 $V$ 闭合，因此 $H$ 在 $e$ 局部闭合。因此 $H$ 在 $G$ 中被命题 4 关闭。

#### 注 {#top-iii-s2-n1-rem-1 .statement tag=0BHY}

令$H$为拓扑群$G$的任意子群。对于每个$x \in \overline{H}$，我们有$x \overline{H} = x$。 $\overline{H} = \overline{H}$，因为$x$的翻译是$G$到$G$的同胚。在其他字中，对于每个$x \in \overline{H}$，$xH$在$\overline{H}$中是*密集*。由此可见，如果 $H$ 不闭，则 $\overline{H} \cap CH$ 在 $\overline{H}$ 中是“稠密”的。

### 2. 拓扑群的组成部分

令 $V$ 为 $G$ 中 $e$ 的*对称* 邻域。由$V$生成的子群，用$V^\infty$表示，由$V$的元素的有限序列的所有乘积$\prod_{i=1}^n x_i$组成。 $V^\infty$ 是“开”*，因为它有 $e$ 作为内部点，因此被 no. 1 的命题 4“闭”。由此可见：

#### 命题 6 {#top-iii-s2-prop-6 .statement tag=0BHZ}

*连通拓扑群由单位元素的每个邻域生成。*

这个命题的逆命题通常是假的，正如我们将在章 IV (§ 2, no. 5) 中看到的那样。如果单位元素的每一个邻域都生成一个拓扑群$G$，我们最多可以说的是$G$包含*除了$G$之外没有开放的子群*。

\* 作为非连通群$G$的例，其具有与$G$不同的开子群，我们可以引用非零实数的*乘法群* $\mathbf{R}^*$，其中子群实数 $> 0$ 的$\mathbf{R}_+^*$ 既开又闭（参见章 IV, § 3, no. 2）。 \*

#### 命题 7 {#top-iii-s2-prop-7 .statement tag=0BI0}

*在拓扑群$G$中，单位元素$e$的分量$K$是闭法线子群。任何点 $x \in G$ 的分量都是陪集 $x.K = K.x$。*

如果$a \in K$，则$a^{-1}K$连通且包含$e$；因此$K^{-1}K \subset K$，这表明$K$是$G$的子群。这个子群在$G$的所有自同构下是不变的，特别是在所有内自同构下，因此$K$在$G$中是*正常*； $K$ 也已关闭（章 I、、no. 5、命题 9）。最后，左翻译$y \to xy$是$G$的同态，它将$e$发送到$x$，因此$x$的分量是$x.K$

$G$的单位元素$e$分量称为$G$的*恒等分量*。

### 3. 密集子群

下面的命题概括了no. 1的命题1：

#### 命题 8 {#top-iii-s2-prop-8 .statement tag=0BI1}

*令$H$为拓扑群$G$的稠密子群，并令$K$为$H$的正规子群。那么$G$中$K$的闭包$\overline{K}$就是$G$的普通子群。*

对于映射$(z, x) \to zxz^{-1}$在$G \times G$上连续，并且映射$H \times K$进入$K$；因此（章I, § 2, no. 1，定理1）它映射$G \times \overline{K} = \overline{H} \times K$变成$\overline{K}$。

#### 命题 9 {#top-iii-s2-prop-9 .statement tag=0BI2}

*令$H$为拓扑群$G$的稠密子群。如果$H$是由$H$中单位元素的每个邻域生成的，则$G$是由$G$中单位元素的每个邻域生成的。*

令$V$为$G$中$e$的任意对称邻域。那么$V \cap H$是$H$中$e$的邻域，因此生成$H$。由此可见 $V$ 生成子群 $H'$ 其中包含 $H$；但 $H'$ 是开闭的（no. 1，命题 4 的推论），因此包含 $\overline{H} = G$。

### 4. 空间与操作员

令$X$为拓扑空间，并令$G$为拓扑群。如果满足以下条件，则称$G$在$X$上“连续运行”：

1) $X$有$G$为群个操作员；在其他字$X$被赋予合成$(s, x) \to s.x$的外法则，其中$G$是操作员的集合，并且对于所有$s, t \in G$和所有$s.(t.x) = (st).x$和$e.x = x$ $x \in X$。

2) $G \times X$到$X$的映射$(s, x) \to s.x$是*连续*。

#### 引理 1 {#top-iii-s2-lem-1 .statement tag=0BI3}

*如果拓扑群* $G$ *在拓扑空间* $X$ 上连续运行，*则对于每个* $s \in G$ *映射* $x \to s.x$ *是* $X$ *的同态$X$。

对于这个映射是连续的双射，其逆$x \to s^{-1}.x$也是连续的。

我们记得，对于$x$的变换$s.x$的每个$x \in X$集合$G.x$乘以$G$的元素$s$被称为$x$的*轨道*（相对于运算符$G$的群），并且所有$s \in G$的集合使得$s.x = x$是$G$的子群，称为$x$的*稳定子*。 $x"$的关系$R(x, y) : "y$属于到轨道是$X$上的等价关系，称为等价关系*由*$G$定义；相对于此关系等价类是$X$点轨道。拓扑空间$X/R$称为$X$的*轨道空间*（相对于$G$），或*$X$*与群*$G$的*空间商，并且是用$X/G$表示； 拓扑与 $X/G$ 据说是 * 拓扑与* $X$ *除以* $G$ 的商。

#### 引理 2 {#top-iii-s2-lem-2 .statement tag=0BI4}

*如果拓扑群* $G$ *在拓扑空间* $X$ 上连续运行，*则等价关系* $R$ *由* $G$ *定义为开*。

对于$X$的开路子集$U$相对于$R$的饱和度为集合$\bigcup_{s \in G} s.U$，并且每个$s.U$开路引理1。

#### 例 1 {#top-iii-s2-n4-exa-1 .statement tag=0BI5}

令 $H$ 为拓扑群 $G$ 的子群。 $H$于$G$持续运行至外法则$(s, x) \to sx$。 $H$ 也在$G$ 外法则 $(x, s) \to sxs^{-1}$ 持续运行。

#### 例 2 {#top-iii-s2-n4-exa-2 .statement tag=0BI6}

\* 如果$K$是拓扑划分环（$§ 6$，no. 7），则乘法群$K^*$在$K$上连续运行外法则$(s, x) \to sx$。 \*

#### 例 3 {#top-iii-s2-n4-exa-3 .statement tag=0BI7}

令$G$为拓扑群，$X$为拓扑空间。那么$G \times X$到$X$的映射$(s, x) \to x$就是$X$上的合成外法则，$G$相对于这个律继续在$X$上运行； $G$ 据说可以在 $X$ 上*简单地*操作。

#### 注 {#top-iii-s2-n4-rem-1 .statement tag=0BI8}

与拓扑群$G$在拓扑空间$X$上连续运行的说不同，人们常说$G$在$X$上*在左侧*连续运行。当与$G$相反的拓扑群$G^0$在$X$上连续运行时，我们说$G$在$X$上*在右侧*连续运行。说$X$有一个合成$(s, x) \to s.x$的连续外法则，其中$G$作为集合运算符，这样$s.(t.x) = (ts).x$和$e.x = x$，这也是同样的道理。这样的律经常写在*右边*：$(s, x) \to x.s$（从而术语），然后我们就有了$(x.t).s = x.(ts)$。如果 $G$ 通过律 $(s, x) \to x.s$ 在 $X$ 的右侧连续运行，则根据公理 (GT$_{II}$)，$G$ 根据外法则 $(s, x) \to x.s^{-1}$ 在 $X$ 的左侧连续运行。

令$X$（分别$X'$）为集合，其中运算符$G$（分别$G'$）的群，并令$f : G \to G'$为同态和$g : X \to X'$映射。如果$g(s.x) = f(s).g(x)$对于所有$s \in G$和所有$x \in X$来说，$f$和$g$被认为是“相容的”的。如果$X''$是运算符$G''$的第三个集合和群，如果$f' : G' \to G''$是同态，$g' : X' \to X''$映射，并且如果$f'$和$g'$相容的，则$f' \circ f$ 和 $g' \circ g$ 相容的。当$X, X'$是拓扑空间和$G, G'$是拓扑群分别在$X, X'$上连续运行时，$(f, g)$被认为是空间的*态射*（带有运算符）$X$到带有运算符的空间 $X'$，前提是$f$和$g$*连续*且*相容的*。 经过到商，$g$ 然后诱导连续映射 $X/G \to X'/G'$ (章 I, , no. 4, 命题 6 的推论)

令$G$为在拓扑空间$X$上连续运行的拓扑群，并令$\varphi$为$X$的典范映射到轨道空间$X/G$。令$A$为$X$的任意子集，并令$A'$为$X$的子空间，这是$A$相对于由$G$定义的等价关系$R$的饱和度（因此$A'$为$A$ 点轨道并，据说是$A$相对于$G$的*饱和度*）。 $G$于$A'$持续运行至$(s, x) \to s.x$至$G \times A'$的限制。此外，由于$R$开路（引理2）且$A'$饱和，因此从章I, § 5, no. 2的命题4，以及关系$\varphi(A) = \varphi(A')$可以得出：

#### 命题 10 {#top-iii-s2-prop-10 .statement tag=0BI9}

* 子空间 $\varphi(A)$ $X/G$ 到轨道空间 $A'/G$ 的规范双射是同胚。*

现在让$S$在$X$上为等价关系，这样，对于每个$s \in G$，映射$x \to s.x$与$S$*相容的*[在其他字中，这样关系$x \equiv y \pmod{S}$意味着$s.x \equiv s.y \pmod{S}$]；为了简洁起见，我们会说关系 $S$ *与群* $G$ 相容的。如果$\psi$是$X$的典范映射到$X/S$，并且如果$s.\psi(x)$表示$s.x$的类模$S$，那么$X/S$有$G$作为运算符的群尊重外法则$(s, \psi(x)) \to s.\psi(x) = \psi(s.x)$。而且：

#### 命题 11 {#top-iii-s2-prop-11 .statement tag=0BIA}

*如果$X$上的等价关系$S$开放并兼容$G$，则$G$将在$X/S$上持续运行。*

由于$G$上等式的关系和$X$上的关系$S$开路，因此足以证明$G \times X$到$X/S$的映射$(s, x) \to s.\psi(x) = \psi(s.x)$是连续的（章） I, § 5, no. 3，命题 8 的推论）；但这是由 $\psi$ 和映射的连续性得出的

$$
(s, x) \to s.x.
$$

#### 注 {#top-iii-s2-n4-rem-2 .statement tag=0BIB}

令$G'$为另一个拓扑群在$X$上连续运行，并假设$s.(s'x) = s'(s.x)$对于所有$s \in G, s' \in G'$和X中的x \。那么由 G' 定义的等价关系 S 与 G 相容的，并且由于 S 是开路（引理 2），因此 G 会连续运行在 X/G' 上。类似地，G' 在 X/G 上连续运行。在这种情况下，X 上的两个群 G 和 G' 中的两个运算被称为可交换。

### 5. 同质空间

设G为拓扑群，G的H子群。H根据外法则$(t, x) \to xt$在G上连续运算，点$x \in G$的轨道为左陪集$xH$。因此，轨道的集合就是我们在代数中所说的齐次空间$G/H$。每当我们将$G/H$视为拓扑空间时，我们总是指G的轨道空间（相对于H）除非，但明确指出相反；即 G 的空间除以等价关系 $x^{-1}y \in H$。根据一般的定义，我们说这个空间的拓扑是G的拓扑与H的商。

#### 命题 12 {#top-iii-s2-prop-12 .statement tag=0BIC}

群 G 在每个齐次空间 $G/H$ 上连续运行。

由于等价关系$x^{-1}y \in H$开路（no. 4，引理2），这是no. 4的命题11的特例。

#### 命题 13 {#top-iii-s2-prop-13 .statement tag=0BID}

设 G 为拓扑群，并设 H 为 G 的子群。则齐次空间 $G/H$ 是豪斯多夫当且仅当 H 在 G 中闭。

对于关系 $x^{-1}y \in H$，H 是等价类，因此，如果 $G/H$ 是 Hausdorff，则 H 在 G 中是闭的。相反，如果 H 是闭的，则该关系的图在 $G \times G$ 中是闭的，因为它是连续映射下 H 的逆像 $(x, y) \to x^{-1}y$。由于关系 $x^{-1}y \in H$ 是开集，因此从章 I, § 8, no. 3、命题 8 可以得出 $G/H$ 是 Hausdorff。

#### 命题 14 {#top-iii-s2-prop-14 .statement tag=0BIE}

设 G 为拓扑群，并设 H 为 G 的子群。则齐次空间 $G/H$ 是离散的当且仅当 H 在 G 中开集。

对于典范映射下$G/H$的点的G中的逆像来说，是陪集$xH$($x \in G$)；当且仅当 H 在 G 中开时，这些集合在 G 中开。

令X为拓扑空间，拓扑群G在其上连续且传递地运行；那么X（在代数意义上）是G的齐次空间。设x是X的点，H_x是稳定子。 G 到 X 上的连续满射 s → s.x 正则因式分解为

$$
G \xrightarrow{f_x} G/H_x \xrightarrow{g_x} X
$$

其中 f_x 是 G 的典范映射到齐次空间 G/H_x 上，g_x 是 G/H_x 的双射 s.H_x → s.x 到 X 上；而且(章I, § 3, no. 4,命题6)g_x是连续的映射。但 g_x 不一定是 G/H_x 在 X (习题 29) 上的同胚。如果 g_x 是每个 x ∈ X 的同态，那么我们说 X 是拓扑齐次空间（拓扑群 G）；为此，对于每个 x ∈ E，G 的映射 s → s.x 到 X 应该是开的。

#### 命题 15 {#top-iii-s2-prop-15 .statement tag=0BIF}

令X为拓扑空间，拓扑群G在其上连续且传递地运行。对于 X 是拓扑齐次空间（相对于 G），对于某些点 x_0 ∈ X 映射 s → s.x_0 变换 G 中 e 的每个邻域到 x_0 中 x_0 的邻域就足够了X。

对于某些 t ∈ G，每个 x ∈ X 都可以写成 x = t.x_0。如果 V 是 e 的邻域，则 V.x = (Vt).x_0 是 x 的邻域，因为我们可以写成 (Vt).x_0 = t((t^{-1}Vt).x_0)，并且断言根据以下事实得出：t^{-1}Vt 是 G 中 e 的邻域，并且 y → t.y 是 X 自身的同胚 (no. 4，引理 1)。由此可知，如果 U 是 G 的任意开子集，并且 x 是X 中的任意点，则 U.x 在 X 中开；因为如果 t ∈ U，则 t^{-1}U 是 e 的邻域，因此 (t^{-1}U).x 是 x 的邻域，并且 t.((t^{-1}U).x) = U.x 是 t.x 的邻域。因此 U.x 在 X 中是开集，因此 G 到 X 的映射 s → s.x 是开集。这样就完成了证明。

### 6. QUOTIENT GROUPS

#### 命题 16 {#top-iii-s2-prop-16 .statement tag=0BIG}

设G是拓扑群，H是G的正规子群。则G的拓扑与H的商与G/H的群结构兼容。

如果 x → x̂ 是 G 到 G/H 的典范映射，那么我们必须证明 (x̂, ŷ) → x̂ŷ^{-1} 是 (G/H) × (G/H) 到 G/H 的连续映射。由于等价关系 x^{-1}y ∈ H 是开集 (no. 4, 引理 2)，因此足以证明 (x, y) → x̂ŷ^{-1} 是 G × G 到 G/H 的连续映射 (章 I, § 5, no. 3，推论到命题 8，并且§ 3, no. 4、命题6)。但 (x, y) → x̂ŷ^{-1} 是连续映射 x → x̂ 和 (x, y) → xy^{-1} 的合成，因此是连续的。

Whenever in the sequel we consider a quotient group $G/H$ of a topological group $G$ as a topological group, it is always to be understood that the topology of $G/H$ is the quotient by $H$ of the topology of $G$, unless the contrary is expressly stated.

#### 命题 17 {#top-iii-s2-prop-17 .statement tag=0BIH}

*Let $\varphi$ be the canonical mapping of a topological group $G$ onto a quotient group $G/H$. If $\mathfrak{B}$ is a fundamental system of neighbourhoods of $e$ in $G$, then $\varphi(\mathfrak{B})$ is a fundamental system of neighbourhoods of the identity element $\varphi(e)$ of $G/H$.*

这是命题 5 of 章 I, § 5, no. 3 的特例。

对于商群，命题 13 和 14 特别给出：

#### 命题 18 {#top-iii-s2-prop-18 .statement tag=0BII}

*令$G$为拓扑群，令$H$为$G$的正规子群。
a) *商群 $G/H$ 是 Hausdorff 当且仅当 $H$ 在 $G$ 内闭。
b) *商群 $G/H$ 是离散的当且仅当 $H$ 在 $G$ 中开路。*

如果$G$是拓扑群，$N$是$\{e\}$在$G$的闭包，那么$N$是$G$的闭法线子群（no. 1，命题1），因此$G/N$ 是豪斯多夫； $G/N$ 被称为与* $G$ 相关的 *Hausdorff 群。

#### 命题 19 {#top-iii-s2-prop-19 .statement tag=0BIJ}

*如果 $H$ 是拓扑群 $G$ 的离散法线子群，则 $G/H$ 与 $G$ 局部同构。*

令$V$为$G$中$e$的邻域，除了$e$之外，不存在包含$H$中的任何点，并令$W$为邻域的对称开邻域 $e$在$G$中，使得$W^2 \subset V$。那么限制到 $W$ 的典范映射 $\varphi$ 的 $G$ 到 $G/H$ 是*内射*；因为如果$x, y \in W$和$\varphi(x) = \varphi(y)$，则$x^{-1}y \in W^2 \subset V$和$x^{-1}y \in H$，因此$x = y$。到命题 17，$\varphi$到$W$的限制是$W$到$\varphi(W)$的同胚；此外，由于$\varphi(xy) = \varphi(x)\varphi(y)$对于所有$x, y \in W$，我们结论认为$G$和$G/H$是局部同构的（§ 1, no. 3，命题3）。

### 7. 子群和商群商群

令$G$为拓扑群，令$H$为$G$的正规子群，令$\varphi : G \to G/H$为典范映射。我们知道，如果$A'$是$G/H$的子群，那么$\overline{\varphi}(A')$就是$G$的子群，其中包含$H$。相反，如果$A$是$G$的子群，则$\varphi(A)$是$G/H$的子群；此外，还有商群 $A/(A \cap H)$ 的规范双射到 $G/H$ 的子群 $\varphi(A)$，以及 $\varphi(A)$ 的规范双射到商群 $AH/H$，并且这两个双射是同构 *对于群结构*。

#### 命题 20 {#top-iii-s2-prop-20 .statement tag=0BIK}

令$A$为拓扑群$G$的子群，令$H$为$G$的正规子群，并令$\varphi$表示$G$的典范映射到$G/H$。那么$\varphi(A)$到$AH/H$的规范双射就是拓扑群的同构。

这是从前面的注和命题 10 of no. 4 得出的。

$A/(A \cap H)$到$\varphi(A)$的规范双射是一个连续的同态，因为它是从$\varphi$的限制到$A$乘经过到商产生的；但一般来说，拓扑群$A/(A \cap H)$和$AH/H$不是同构的（cf.§ 4, no. 1，命题1，推论3）。

\* 对于例，取$G$为实数的加法群$\mathbf{R}$，取$H$为整数的群$\mathbf{Z}$，并取$A$为群无理数数 $\theta$ 的 $\theta \mathbf{Z}$ 整数倍数。然后$A \cap H = \{0\}$，使得$A/(A \cap H)$是一个离散的群，与$\mathbf{Z}$同构；另一方面，$A + H$在$\mathbf{R}$中是稠密的（正如我们将在章V, § 1, no. 1，命题1中看到的那样），因而$(A + H)/H$与$A + H$（no. 6，命题19）局部同构，是不是离散的群，因此与 $A/(A \cap H)$ 不同构。 \*

尽管如此，我们还是有以下命题：

#### 命题 21 {#top-iii-s2-prop-21 .statement tag=0BIL}

令$G$为拓扑群，$G_0$为$G$的稠密子群，$H_0$为$G_0$的正常子群，$H$为$G$中$H_0$的闭包，并且$\varphi$典范映射$G \to G/H$。那么规范的双射$G_0/H_0 \to \varphi(G_0)$就是拓扑群$G_0/H_0$的同构到$G/H$的稠密子群。

从$H_0 = H \cap G_0$开始，只要证明$U_0$是$G_0$的任意开子集且相对于关系$x^{-1}y \in H_0$饱和，则$U_0$是$G_0$的交和开子集 $G$相对于关系$x^{-1}y \in H$（章I, § 3, no. 6，命题10）饱和。令$U$为$G$的开子集，使得$U_0 = U \cap G_0$。从$U_0 = U_0 H_0$开始，很容易看出$U_0 = U H_0 \cap G_0$；但是$U H_0$在$G$开放，所以我们可以假设$U = U H_0$。 集合$U H$在$G$开放，相对于关系$x^{-1}y \in H$饱和；因此，如果我们证明$U H \cap G_0 = U_0$，命题就能得到证明。现在，如果$u \in U$和$h \in H$使得$u h \in G_0$，那么在$G$中存在$e$的对称邻域$V$使得$u V \subset U$；由于$V h$是$G$中$h$的邻域，因此存在$z \in V$使得$z h \in H_0$。但是我们有 $u z^{-1} \in U$ 和 $u h = (u z^{-1})(z h)$；因此$U H \cap G_0 \subset U H_0$。但是$U H_0 = U$，因此$U H \cap G_0 \subset U \cap G_0 = U_0$。这样就完成了证明。

令$G$为在拓扑空间$X$上连续运行的拓扑群，并令$K$为$G$的正常子群，其包含在$X$的每个点的稳定子中。因此，对于每个$x \in X$，关系$s \equiv t \pmod{K}$意味着$s.x = t.x$，而经过意味着我们将$G/K$的定义映射$s \to s.x$除以$X$。立即验证，对于外法则$(s', x) \to s'.x$，X有G/K作为群的算子。而且，相对于这个律，G/K在X上持续运行；对于X上的等式的关系和G上的关系$s \equiv t \pmod{K}$都是开等价关系，因此结果由映射的连续性得出

$$(s, x) \to s'.x = s.x$$

$G \times X$ 变为X（章 I, § 5, no. 3，推论命题 8，以及§ 3, no. 4、命题 6）。

现在令 G 为在拓扑空间 X 上连续运行的拓扑群，并令 H 为 G 的任意正规子群；则H在X上连续运算。令 S 为 H 在 X 上定义的等价关系；则 S 开路（no. 4，引理 2）。 关系 S 兼容群 G (no. 4)；因为如果$y \equiv x \pmod{S}$则存在$t \in H$使得$y = t.x$；因此对于所有$s \in G$，我们有$s.y = (sts^{-1}).s.x$和$sts^{-1} \in H$，因为H在G中是正规的；因此$s.y \equiv s.x \pmod{S}$。如果$\psi$是X的典范映射到X/S，群G因此相对于外法则在X/S上连续运行

$$(s, \psi(x)) \to \psi(s.x)$$

（no. 4，命题11）。另外，X/S的点各自的稳定子中含有群H。正如我们在上面看到的，G/H 相对于外法则 $(s', \psi(x)) \to \psi(s.x)$ 连续运行在 $X/S = X/H$ 上。如果R在G定义的X上表示等价关系，则关系S意味着R，X/S上的等价关系R/S是由群G/H定义的。因此（章I, § 3, no. 4，命题7）：

#### 命题 22 {#top-iii-s2-prop-22 .statement tag=0BIM}

*设G是在拓扑空间X上连续运行的拓扑群，并令H是G的正规子群。那么X/G到$(X/H)/(G/H)$的规范双射是同胚。*

#### 推论 {#top-iii-s2-n7-cor-1 .statement tag=0BIN}

*设G是拓扑群，H是G的法线子群，K是G的法线子群，其中包含H。那么G/K到$(G/H)/(K/H)$的规范双射就是拓扑的同构群.*

我们已经知道，这个双射是群的同构，而命题22（应用于在G右边运算的群K）表明它是同胚。

### 8. 连续同态和严格态射

#### 命题 23 {#top-iii-s2-prop-23 .statement tag=0BIO}

*拓扑群 G 的同态 f 转换为拓扑群 $G'$ 在 G 上连续当且仅当它在 G 的一个点处连续。*

假设$f$在点$a \in G$连续；那么如果$V'$是$f(a)$中的任意邻域，则$V = \overline{f^{-1}}(V')$是$a$中的邻域。因此，如果 $x$ 是 $G$ 中的任意点，我们有
$$
f(xa^{-1}V) = f(x)[f(a)]^{-1}f(V) \subset f(x)[f(a)]^{-1}V',
$$
因此$f$在$x$连续。

拓扑群$G$到拓扑群$G'$的连续同态也称为拓扑群结构的$G$到$G'$的*态射*。

设$f$是拓扑群$G$到拓扑群$G'$的连续同态； $G'$的单位元素$e'$的逆像$H = \overline{f^{-1}}(e')$是$G$的*普通子群*，$f(G)$是$G'$的*子群*。考虑正则分解$f = \psi \circ \dot{f} \circ \varphi$，其中$\varphi$是典范映射$G \to G/H$，$\psi$是典范嵌入$f(G) \to G'$，最后$\dot{f}$是商群的*连续双射同态* $G/H$到子群$f(G)$（章I, § 3, no. 5）； $\dot{f}$ 据说是与 $f$ *关联*的双射同态。一般来说，$\dot{f}$不是拓扑群的同构。

对于例，令$G'$为非离散拓扑群，$G$为通过给$G'$赋予离散拓扑而得到的拓扑群；那么$G$到$G'$的恒等映射是连续双射同态，但不是双连续的。

#### 定义 1 {#top-iii-s2-def-1 .statement tag=0BIP}

*拓扑群$G$到拓扑群$G'$的连续同态被认为是$G$到$G'$的严格态射，如果$G/\overline{f^{-1}}(e')$的双射同态$\dot{f}$到$f(G)$，与$f$相关，是拓扑群的同构（在其他字，如果$\dot{f}$是双连续的）。*

因此，拓扑群$G$到拓扑群$G'$的同构是$G$到$G'$的双射严格态射。

#### 命题 24 {#top-iii-s2-prop-24 .statement tag=0BIQ}

*设$f$是拓扑群$G$到拓扑群$G'$的连续同态。那么下面三个叙述是等价的：*
a) $f$ *是严格的态射。*
b) *$G$中每个开路集合的$f$下的像是$f(G)$中的开路集合。*
c) *$G$中单位元素每邻域$f$下像是$G'$中单位元素邻域。*

鉴于no. 4的引理2，a）和b）的等价紧随定义（章I, § 5, no. 3，命题5）。 b) 和 c) 的等价是 no. 5 的命题 15 的特例，如果我们观察到 $G$ 在 $f(G)$ 上连续运行外法则 $(s, f(t)) \to f(st)$。

#### 注 1 {#top-iii-s2-n8-rem-1 .statement tag=0BIR}

从命题 24 的条件 b) 可以得出，拓扑群到离散群的每个连续同态都是严格的态射。

如果 G 是紧致的且 $f(G)$ 是 Hausdorff，则与 $f$ 关联的双射同态 $f$ 是双连续的（章 I, § 10, no. 2、定理 1，推论 2，以及 no. 1、命题 5，推论 4）。因此，紧致群到 Hausdorff 群的每个连续同态都是严格的态射。

#### 注 2 {#top-iii-s2-n8-rem-2 .statement tag=0BIS}

令$f$是G到$G'$的严格态射，并让$g$是$G'$到$G''$的严格态射。如果 $f$ 是满射或者 $g$ 是单射，则从命题 24 立即得出 $g \circ f$ 是 G 到 $G''$ 的严格态射。但如果前面两个条件都不满足，即使$f$是单射且$g$满射（习题 19），这个结论也不一定有效。

#### 注 3 {#top-iii-s2-n8-rem-3 .statement tag=0BIT}

令 $f$ 为拓扑群 G 到拓扑群 $G'$ 的连续同态，并令 H 为 G 的正规子群。$f$ 诱导同态 $g$ 群 $G/H$ 到商群 $f(G)/f(H)$。 这个同态$g$是连续的。 Moreover, if $f$ is a strict morphism of G into $G'$, then $g$ is a strict morphism of $G/H$ onto $f(G)/f(H)$; for if U is open in $G/H$, and if $\varphi$ (resp. $\varphi'$) denotes the canonical mapping of G onto $G/H$ [resp. of $f(G)$ onto $f(G)/f(H)$], then we have $g(u) = \varphi'(f(\overline{\varphi}^{-1}(u)))$, and since $\overline{\varphi}^{-1}(u)$ is open in G, it follows that $g(u)$ is open in $f(G)/f(H)$, which proves our assertion.

### 9. 拓扑乘积群

设$(G_i)_{i \in I}$是拓扑群的族。然后我们可以在乘积集合上定义群结构

$$
G = \prod_{i \in I} G_i
$$

（$G_i$的群结构的乘积）通过定义$(x_i).(y_i) = (x_i y_i)$。如果$e_i$是$G_i$的单位元素，那么$e = (e_i)$就是G的单位元素，并且我们有$(x_i)^{-1} = (x_i^{-1})$。 $G_i$拓扑结构的乘积拓扑（章I, § 2, no. 3）与群结构兼容。对于 $G \times G$ 的映射 $((x_i), (y_i)) \to (x_i, y_i^{-1})$ 到 G 中是映射 $((x_i, y_i)) \to (x_i y_i^{-1})$ 的合成

$$
\prod_{i \in I} G_i \times G_i \text{ into } G,
$$

和典范映射 $((x_i), (y_i)) \to ((x_i, y_i))$

$$
G \times G \text{ onto } \prod_{i \in I} (G_i \times G_i);
$$

并且这两个映射都是连续的（章I, § 4, no. 1，命题1的推论1和命题2）。

#### 定义 2 {#top-iii-s2-def-2 .statement tag=0BIU}

*通过给出乘积集合获得拓扑群*

$$
G = \prod_{i \in I} G_i
$$

*the group structure which is the product of the group structures of the $G_i$ and the topology which is the product of the topologies of the $G_i$ is called the product of the topological groups $G_i$.*

如果$(J_x)_{x \in K}$是$I$的*划分*，则$G$同构于拓扑群$\prod_{i \in J_x} G_i$的乘积（乘积的结合性）。

如果$H_i$是$G_i$的子群，则拓扑群$H_i$的乘积同构于$\prod_{i \in I} G_i$的子群$\prod_{i \in J} H_i$。特别是，如果$J$是$I$和$J' = C J$中的任意子集，则拓扑群$\prod_{i \in J} G_i$同构于$G$的正常子群$G'_J = (\prod_{i \in J} G_i) \times (\prod_{i \in J'} \{e_i\})$。由于每个开集合的投影都是开集合，$G$到$\prod_{i \in J} G_i$的投影$\mathrm{pr}_J$是一个*严格的态射*，因此商群$G/G'$同构于$G'_J$； $G$ 与乘积 $G'_J \times (G/G'_J)$ 同构的。

#### 命题 25 {#top-iii-s2-prop-25 .statement tag=0BIV}

*令$(G_i)_{i \in I}$为群的拓扑族，并令$H$为所有$x = (x_i)$的$G = \prod_{i \in I} G_i$由……组成的正规子群，使得$x_i$等于单位元素$e_i$ $G_i$ 除了有限的数指标。那么子群$H$在$G$中是稠密的。*

这是章 I, § 4, no. 3、命题 8 的特例。

令$(X_i)_{i \in I}$为拓扑空间的族，对于每个$i \in I$，令$G_i$为在$X_i$上连续运行的拓扑群。显然，乘积群 $G = \prod_{i \in I} G_i$ 然后根据律在乘积空间 $X = \prod_{i \in I} X_i$ 上连续运行

$$
((s_i), (x_i)) \to (s_i \cdot x_i)
$$

（章 I, § 4, no. 1、命题 1、推论 1 和命题 2）。另外，$X$的点$x = (x_i)$$G$下的轨道是$x_i$的轨道乘积(相对于群$G_i$)。令$\varphi_i$为$X_i$的典范映射到$X_i/G_i$，令$\varphi = (\varphi_i)$为$X$的乘积映射到$\prod_{i \in I} (X_i/G_i)$；那么前面的注表明双射与$\varphi$映射轨道空间$X/G$规范地关联到$\prod_{i \in I} (X_i/G_i)$。此外：

#### 命题 26 {#top-iii-s2-prop-26 .statement tag=0BIW}

*$X/G$ *到* $\prod_{i \in I} (X_i/G_i)$ *规范地与* $(\varphi_i)$ *相关的双射 *是同胚。* 因为由于 $\varphi_i$ 是满射且开的，因而 $\varphi = (\varphi_i)$ 是开映射 (章) I, , no. 3, 命题 8 的推论)

#### 推论{#top-iii-s2-n9-cor-1 .statement tag=0BIX}

*让* $(G_i)_{i \in I}$ *成为拓扑群的族，并且对于每个* $i \in I$ *让* $H_i$ *成为* $G_i$的正规子群； *让*$\varphi_i$*表示*$G_i$*的典范映射*到*$G_i/H_i$。 *让*$G = \prod_{i \in I} G_i, \ H = \prod_{i \in I} H_i$。 *则* $G/H$ *到* $\prod_{i \in I} (G_i/H_i)$ *与连续同态* $(x_i) \to (\varphi_i(x_i))$ *相关的双射同态 *是拓扑群的同构。*

对于这个同态是群结构中的同构。

#### 注 {#top-iii-s2-n9-rem-1 .statement tag=0BIY}

如果 $G$ 是一个*可交换的*拓扑群，加法书写，那么 $G \times G$ 到 $G$ 的映射 $(x, y) \to x + y$ 是一个*严格的态射*。因为从$(x + x') + (y + y') = (x + y) + (x' + y')$开始，它是$G \times G$到$G$的*同态*；也是连续的，在该映射下，$G \times G$原点的邻域$V \times V$的像是$G$原点的邻域$V + V$。

### 10. 半直接乘积

令$L, N$为群$G$中的两个子群，使得$LN = NL$；那么 $LN$ 是 $G$ 的 *子群*，因为

$$
(LN)(LN)^{-1} = LNN^{-1}L^{-1} = LNL = LLN = LN
$$

此外，$N \times L$到$G$的映射$\varphi : (x, y) \to xy$是*内射*当且仅当$N \cap L = \{e\}$。因为很明显，如果 $\varphi$ 是单射的，则 $N \cap L = \{e\}$；相反，关系$x'y' = xy$，其中$x, x' \in N$和$y, y' \in L$，意味着$x^{-1}x' = {yy'}^{-1} \in N \cap L$；因此，如果$N \cap L = \{e\}$，则$\varphi$是单射的。因此，$\varphi$是*双射的*当且仅当$LN = G$和$N \cap L = \{e\}$。

如果$N$是$G$的*正常*子群（或者更一般地在$G$包含$N \cup L$的某些子群中是正常的），则自动满足条件$LN = NL$。此外，对于每个$y \in L$映射$\sigma_y : x \to yxy^{-1}$都是群$N$的*自同构*，并且对于$L$的任意两个元素$u, v$我们有

$$(1)$$
$$
\sigma_{uv} = \sigma_u \circ \sigma_v;
$$

对于$\mathbf{N}$中的任何$x, x'$和$\mathbf{L}$中的$y, y'$，我们也有

$$(2)$$
$$(xy)(x'y') = (x\sigma_y(x'))(yy').$$

反之：

#### 命题 27 {#top-iii-s2-prop-27 .statement tag=0BIZ}

*令$\mathbf{N}$和$\mathbf{L}$分别为两个群、$e'$和$e''$，它们各自的单位元素。假设我们将$\mathbf{L}$的同态$y \to \sigma_y$赋予$\mathbf{N}$的自同构群$\Gamma$。然后：*

1) *在乘积集合$S = \mathbf{N} \times \mathbf{L}$上，合成的内部律*
$$(3)$$
$$(x, y)(x', y') = (x\sigma_y(x'), yy')$$
*定义群结构，其中$j_1 : x \to (x, e'')$是$\mathbf{N}$的同构到$S$的正常子群，$j_2 : y \to (e', y)$是$\mathbf{L}$的同构到子群 $S$，而$\mathrm{pr}_2 : S \to \mathbf{L}$是满同态，其核是$j_1(\mathbf{N})$，因此$\mathrm{pr}_2 \circ j_2$是$\mathbf{L}$的恒等式自同构。*

2) *设$f : \mathbf{N} \to G$、$g : \mathbf{L} \to G$为同态入群$G$，这样*
$$(4)$$
$$f(\sigma_y(x)) = g(y)f(x)g(y^{-1})$$
*适用于所有 $x \in \mathbf{N}$ 和所有 $y \in \mathbf{L}$。然后有唯一同态$h : S \to G$使得$f = h \circ j_1$和$g = h \circ j_2$。*

如果$x, x', x''$是$\mathbf{N}$的元素并且$y, y', y''$是$\mathbf{L}$的元素，那么
$$
((x, y)(x', y'))(x'', y'') = (x\sigma_y(x'), yy')(x'', y'')
= (x\sigma_y(x')\sigma_{y'}(x''), yy'y'')
$$
和
$$
(x, y)((x', y')(x'', y'')) = (x, y)(x'\sigma_{y'}(x''), y'y'')
= (x\sigma_y(x'\sigma_{y'}(x'')), yy', y'')
$$
因此律 (3) 的结合性可以从$y \to \sigma_y$ 是$\mathbf{L}$ 的同态到$\Gamma$ 以及$\sigma_y$ 是$\mathbf{N}$ 的自同构的事实得出。显然$(e', e'')$是(3)的单位元素，最后
$$(x, y)(\sigma_{y^{-1}}(x^{-1}), y^{-1}) = (\sigma_{y^{-1}}(x^{-1}), y^{-1})(x, y) = (e', e'')$$
这样 $(x, y)$ 在 $S$ 中有一个逆元。 1)的其他断言是清楚的。另一方面，由于$(x, y) = (x, e'') (e', y)$，满足2)的条件的同态$h$必然是满足
$$h(x, y) = f(x)g(y),$$
因此，如果存在的话，它是唯一的；此外，根据 (4) 可知直接的
$$f(x\sigma_y(x'))g(yy') = f(x)g(y)f(x')g(y^{-1})g(y)g(y') = f(x)g(y)f(x')g(y')$$

这表明 $(x, y) \to f(x)g(y)$ 确实是 S 的同态变成 2) 的 G 满足条件。

#### 推论{#top-iii-s2-n10-cor-1 .statement tag=0BJ0}

* 命题 27 的 2) 中定义的同态 h 是单射的当且仅当 f 和 g 是单射且$f(N) \cap g(L) = \{e\}$； h 是满射当且仅当 $f(N)g(L) = G$。

由于$h(x, y) = f(x)g(y)$，第二个断言是明显的；此外，从(4)可以得出$f(N)g(L) = g(L)f(N)$，第一个断言是从本小节开头的注得出的。

The group S defined in Proposition 27 is said to be the *external semi-direct product* of N and L (relative to $\sigma$); we shall generally identify N (resp. L) with the normal subgroup $j_1(N)$ [resp. the subgroup $j_2(L)$] of S. 如果对于所有$y \in L$，$\sigma_y$是$\Gamma$的单位元素，我们检索两个群的*乘积*的通常概念。

现在令 G 为群，并令 L 和 N 为 G 的两个子群，使得 LN = NL 并且 N 在 NL 中是*正常*，因此对于每个 $y \in L$，$\sigma_y : x \to yxy^{-1}$ 是 N 的自同构，$y \to \sigma_y$ 是 N 的同态 L 到 N 的自同构群 $\Gamma$。 从命题 27 可以得出，如果 S 是 N 的外部半直接乘积和 L（相对于 $\sigma$），则 $h : (x, y) \to xy$ 是 S 到 G 的 *同态*。 h 是双射当且仅当我们有 $N \cap L = \{e\}$ 和 $NL = G$ （命题 27 的推论）； G 则被称为其正常子群 N 及其子群 L 的*半直接乘积*，并且我们经常通过 h 与 S 进行认同 G。

#### 命题 28 {#top-iii-s2-prop-28 .statement tag=0BJ1}

*设L、N为两个拓扑群，设$y \to \sigma_y$为N的(非拓扑)群结构的自同构$\Gamma$群L同态；并假设$N \times L$到N中的映射$(x, y) \to \sigma_y(x)$是连续的。然后：

1) *在N和L的外部半直接乘积 S上，相对于$\sigma$，N和L的拓扑的乘积与群结构兼容； 典范嵌入$j_1 : N \to S$和$j_2 : L \to S$分别是拓扑群N和L到S的子群$j_1(N)$和$j_2(L)$的同构，$pr_2$是S到态射的严格态射 L.*

2) *设$f : N \to G$和$g : L \to G$为两个连续的同态组成拓扑群G，满足 (4)；然后同态*

$$
(x, y) \to f(x)g(y)
$$

*S到G是连续的。*

这是定义的直接的推论以及乘积拓扑的属性。

由此定义的拓扑群 S 被认为是 N 和 L 的外部拓扑半直接乘积（相对于 σ）；请注意，对 σ 施加条件意味着 L 根据外法则 $(x, y) \to \sigma_y(x)$ [no. 4] 在 N 的左侧连续运算。

现在令 G 为拓扑群，并令 N 和 L 为 G 的两个子群，使得 G 为 N 和 L 的半直接乘积，即非拓扑群；那么很明显映射$(x, y) \to \sigma_y(x)$在$N \times L$上连续，并且规范双射同态

$$
h : (x, y) \to xy
$$

S 到 G 上是连续的。但这个同态不一定是双连续的；当它是双连续时，G 被称为 N 和 L 的拓扑半直接乘积。为此，如果$p : G \to N$和$q : G \to L$是映射，使得对应到$z \in G$唯一元素$p(z) \in N$和$q(z) \in L$使得$z = p(z)q(z)$，则映射$p, q$之一是连续的（在这种情况下两者都是连续的）。说典范映射$G \to G/N$的限制到L是拓扑群L到拓扑群G/N的同构，也是同样的道理。

### 习题{#top-iii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
