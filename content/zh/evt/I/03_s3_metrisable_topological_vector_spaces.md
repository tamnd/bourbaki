---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 3
section_title: Metrisable topological vector spaces
lang: zh
source: evt-i-v
book_pages: TVS I.28-TVS I.29
pdf_pages: 0024-0030, 0036-0037
extraction: ocr
subsections:
    - "no": 1
      title: Neighbourhoods of 0 in a metrisable topological vector space
      page: 16
      pdf_page: 24
    - "no": 2
      title: Properties of metrisable vector spaces
      page: 17
      pdf_page: 25
    - "no": 3
      title: Continuous linear functions in a metrisable vector space
      page: 17
      pdf_page: 25
statements: 11
exercises: 9
content_sha256: bffbbeaad154b477da234b5973d1116df36b88b555fd1c4079611931d3de75a6
translated_from: content/en/evt/I/03_s3_metrisable_topological_vector_spaces.md
translation_method: google
source_content_sha256: 78359984fd72f570938f28fdd80715c249ddc585d312089e4556c2677edeb57f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 06577a377b9b4d15737985608d2ad6f8897fc1ed0ca3087f64a4911bb379e63e
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。可度量拓扑向量空间

### 1. 可度量拓扑向量空间中 0 的邻域

如果一个拓扑向量空间 E 的拓扑是可度量的，我们就说它是“可度量的”。因此，相对于其加法群和拓扑的结构，E 是可度量的群 (GT, IX, § 3.1)。

我们知道，要使拓扑群可度量，存在中性元素$e$的邻域的可枚举基本系统是必要且充分的，其中交是单个元素$e$（GT，IX, § 3.1，prop. 1）。

我们还知道，可度量拓扑向量空间 E 的均匀结构可以通过*不变距离* $d(x, y) = |x - y|$ 来定义，其中 $x \mapsto |x|$ 是 E 在 $\mathbf{R}_+$ 中的连续映射，满足条件 ： 1) $|-x| = |x|$； 2）$|x + y| \leq |x| + |y|$； 3) 关系 $|x| = 0$ 相当于 $x = 0$（GT，IX, § 3.1，第 3 条）。

我们看到（GT，IX.§ 3.1，道具2）如何使用E中0的邻域的递减序列$(W_n)$来定义这样的距离d，形成邻域的基本系统，并使得$W_{n+1} + W_{n+1} + W_{n+1} \subset W_n$。当 E 是非离散值除法环 K 上的可度量向量空间时，我们还可以假设 $W_n$ 是平衡的（I、p. 7，命题 4）；如果我们回到 $d$ (*loc.cit.*) 的定义的过程，我们可以看到 *关系* $|\lambda| \leq 1 \implies |\lambda x| \leq |x|$。此外，I、p. 2的条件（EVT$_I$）和（EVT$_{II}$）意味着$|\lambda x_0|$*趋于0，因为对于每个$x_0 \in E$，$\lambda$在K*中趋于0，并且$|\lambda_0 x|$*趋于0因为对于每个 $\lambda_0 \in K$，$|x|$ 趋向于 0*。相反，如果函数 $|x|$ 具有所有前述属性，并且如果 $W_n$ 是 $x \in E$ 的集合，使得 $|x| \leq 2^{-n}$，则 $W_n$ 形式是平衡 0 的邻域的基本系统，对于E 上的可度量拓扑与 E 的向量空间结构兼容。

#### 注 {#evt-i-s3-n1-rem-1 .statement tag=07A5}

可度量向量空间中最重要的类之一是标准化的空间 (I, p. 3)。但必须注意，存在可度量向量空间，其拓扑不能由范数定义（I, § 3，执行1）；稍后我们会学习重要的例。

### 2. 可测量向量空间的属性

可度量拓扑向量空间 E 的每个向量子空间都是可度量的；对于 E 的每个商空间 E/M 与闭向量子空间 M 的商（GT，IX, § 3.1，道具 4）也是如此。可度量拓扑向量空间的可枚举族中的每个乘积都是可度量的（GT，IX, § 2.4，cor.2）。如果 K_0 是全值除法环，并且 K 是 K_0 中处处稠密的细分环，则 K 上的可度量向量空间 E 的补全 $\hat{E}$ 是 K_0 上的可度量向量空间（I、p. 6 和 GT、IX, § 2, No. 1，道具1）。最后，如果 E 是完备的可度量向量空间，则对于 E 的每个闭向量子空间 M，商空间 E/M 是完备的（GT，IX, § 3.1，命题 4）。

### 3. 可度量向量空间中的连续线性函数

#### 定理 1（巴纳赫）{#evt-i-s3-thm-1 .statement tag=07A6}

令 E 和 F 为非离散值除法环 K 上的两个可度量向量空间，并令 u 为 F 中 E 的连续线性映射。假设 E 是完备的。那么下面的条件是等价的：
(i) u 是严格的满射态射。
(ii) F 是完备的且 u 是满射的。
(iii) u 的像在 F 中并不微不足道 (GT, IX, § 5.2)。
(iv) 对于 E 中每个 0 的邻域 V，集合 $\overline{u(V)}$ 是 F 中 0 的邻域。

首先，(i) 意味着 (ii)，因为令 u 为严格满射态射，N 为 u 的核。那么 F 上的 E/N 的 u 诱导同构。但 E 是可度量且完备的，因此 E/N 是完备的（GT，IX, § 3.1，命题 4），因此 F 是完备的。

接下来的（ii）意味着（iii）。设 F 是完备的，u 是满射的。 u 的像恰好是 F，因此从 Baire 的定理 (GT, IX, § 5.3) 来看，F 并不微薄。

下面的引理表明(iii)蕴涵(iv)。

#### 引理 1 {#evt-i-s3-lem-1 .statement tag=07A7}

令 E 和 F 为非离散值除法环 K 上的两个拓扑向量空间，并令 u 为 F 中 E 的连续线性映射，使得 E 的像并不微薄。那么，对于 E 中每个 0 的邻域 V，集合 $\overline{u(V)}$ 都是 F 中 0 的邻域。

令 W 为 E 中 0 的平衡邻域，使得 W + W ⊂ V（I, § 1.5，道具 4）。令 α 为 K 的元素，使得 |α| > 1；则 E 是集合 $\alpha^n W$ 的并，其中 n 在 $\mathbf{N}$ 中变化；事实上，对于所有 x ∈ E，存在 β ∈ K 使得 x ∈ βW (I, p. 7, 命题 4) 并且存在整数 n ≥ 0 使得 |β| < |α|^n，则 x ∈ $\alpha^n W$ 因为 W 是平衡的。因此，u(E) 是集合 $u(\alpha^n W) = \alpha^n u(W)$ 的序列的并，并且由于 u(E) 在 F 中并不微薄，因此集合 $\alpha^n \overline{u(W)}$ 中的至少一个拥有内部点 (GT, IX, § 5.3, def. 2)，因此$\overline{u(W)}$ 有一个内部点。

令$y_0$为$\overline{u(W)}$的内部点；因为$-u(W) = u(W)$，因此$-\overline{u(W)} = \overline{u(W)}$，因此$0 = y_0 + (-y_0)$是$\overline{u(W)} + \overline{u(W)}$的内部点。由于向量加法是$F$中$F \times F$的连续映射，集合$\overline{u(W)} + \overline{u(W)}$包含在集合的闭包中

$$
u(W) + u(W) = u(W + W) \subset u(V);
$$

因此$\overline{u(V)}$是$F$中0的邻域。

(iv) 意味着 (i) 之前证明，我们证明以下引理，其中我们约定，在所有度量空间中，$B_r(x)$表示中心$x$和半径$r$的*闭合*球。

#### 引理 2 {#evt-i-s3-lem-2 .statement tag=07A8}

*设E和F是两个度量空间，并假设E也是完备的。令u为F中E的线性映射，具有以下性质：无论数$r > 0$，都存在数$\rho(r) > 0$，这样，对于所有$x \in E$，我们有*

$$
B_{\rho(r)}(u(x)) \subset \overline{u(B_r(x))}.
$$

*在这些条件中，对于所有$a > r$、像$u(B_a(x))$包含球$B_{\rho(r)}(u(x))$。*

令$(r_n)$为数$> 0$的无限序列，使得$r_1 = r$和$a = \sum_{n=1}^{\infty} r_n$。对于每个指标$n$，都存在数$\rho_n > 0$（与$\rho_1 = \rho(r)$），使得

$$
B_{\rho_n}(u(x)) \subset \overline{u(B_{r_n}(x))}
$$

对于所有人$x \in E$；我们可以并且将会假设$\lim_{n \to \infty} \rho_n = 0$。

设$x_0$为E的点，$y$为$B_{\rho(r)}(u(x_0))$的点。我们将证明$y$属于到$u(B_a(x_0))$。

为此，E 的点的序列 $(x_n)_{n>0}$ 被归纳定义，使得对于所有 $n \geq 1$，我们有 $x_n \in B_{r_n}(x_{n-1})$ 和 $u(x_n) \in B_{\rho_{n+1}}(y)$。如果$x_i$已经为$0 \leq i \leq n-1$满足这些关系定义，那么我们就有$y \in B_{\rho_n}(u(x_{n-1}))$；自从

$$
B_{\rho_n}(u(x_{n-1})) \subset \overline{u(B_{r_n}(x_{n-1}))},
$$

存在点$x_n \in B_{r_n}(x_{n-1})$，其中像$u(x_n)$属于到$y$的邻域$B_{\rho_{n+1}}(y)$，从而证明序列$(x_n)$的存在。

由于 $x_n$ 到 $x_{n+p}$ 的距离小于 $r_{n+1} + r_{n+2} + \cdots + r_{n+p}$（当 $n$ 大时，该距离任意小），因此序列 $(x_n)$ 是 E 中的柯西序列。当 E 完备时，序列 $(x_n)$ 收敛为E 的点 $x$。$x_0$ 与$x$ 的距离小于$\sum_{n=1}^{\infty} r_n = a$，因此$x \in B_a(x_0)$。但$u$是连续的，因此序列$u(x_n)$收敛于$u(x)$；也$u(x_n) \in B_{\rho_{n+1}}(y)$，因此$y = u(x)$，并且引理被证明。

我们回到定理并证明 (iv) 蕴涵 (i)。假设$u$满足条件(iv)。对于空间 E 和 F 中的每一个，考虑平移下不变的距离，并且定义其拓扑 (I, p. 16)。通过假设，对于每个$r > 0$，集合$\overline{u(B_r(0))}$是F中0的邻域，因此存在数$\rho(r) > 0$使得$B_{\rho(r)}(0) \subset u(B_r(0))$。通过翻译，我们将结论表示为所有$r > 0$和所有$x \in E$的$B_{\rho(r)}(u(x)) \subset \overline{u(B_r(x))}$。从引理 2开始，对于每一个对实正数$(a, r), a > r > 0$，我们有$B_{\rho(r)}(0) \subset u(B_a(0))$；因此$u$是E在F上的严格态射。我们已经证明(iv)蕴涵(i)并且定理的证明是完备的。

#### 推论 1 {#evt-i-s3-lem-2-cor-1 .statement tag=07A9}

*如果 E 和 F 是非离散值除法环上的两个完全可度量向量空间，则 E 在 F 上的每个双射连续线性映射都是同构。*

特别是，如果 E 和 F 是两个完整的*标准化*空间，则存在数$a > 0$，使得对于所有$x \in E$都有$\|u(x)\| \geq a.\|x\|$。

#### 推论 2 {#evt-i-s3-lem-2-cor-2 .statement tag=07AA}

*令 E 为非离散值除法环上的向量空间，令 $\mathscr{T}_1$ 和 $\mathscr{T}_2$ 为 E 上与其向量空间结构兼容的两个拓扑，并且对于每个拓扑，E 都是可度量且完备的。然后，如果 $\mathscr{T}_1$ 和 $\mathscr{T}_2$ 具有可比性，则它们是相同的。*

#### 推论 3 {#evt-i-s3-lem-2-cor-3 .statement tag=07AB}

*设 E 和 F 是非离散值除法环上的两个完整可度量向量空间。在阶中，F中E的连续线性映射u应该是严格的态射，$u(E)$在F中闭是充分必要的。*

条件是必要的，因为如果 $u$ 是严格的态射，则像 $u(E)$ 同构于商 $E/u^{-1}(0)$，是完备的 (I，p. 17)，因此在 F 中闭合。条件是足够的，因为，如果 $u(E)$ 在 F 中闭，那么 $u(E)$ 必定是一个完全可度量的向量空间，因此通过定理 1 $u$ 是 E 在 $u(E)$ 上的严格态射。

#### 推论 4 {#evt-i-s3-lem-2-cor-4 .statement tag=07AC}

*令 E 为非离散值除法环上的完整可度量向量空间。如果 M 和 N 是两个闭向量子空间，即 E 中的（代数）补集，则 E 是 M 和 N 的直接拓扑和。*

因为 $M \times N$ 是一个完全可度量的向量空间，并且 $M \times N$ 在 E 上的映射 $(y, z) \mapsto y + z$ 是连续且双射的，因此同构（cor. 1）。

#### 推论5（封闭图定理）{#evt-i-s3-lem-2-cor-5 .statement tag=07AD}

— *令 E 和 F 是非离散值除法环上的两个完整可度量向量空间。在阶中，F 中 E 的线性映射 u 是连续的，则其图在乘积空间 $E \times F$ 中是闭合的充要条件。*

条件是必要的，因为连续映射到 Hausdorff 空间的图是封闭的（GT，I, § 8.1，cor.2）。要看出它是足够的，注意味着$u$的图G，它是完整可度量空间$E \times F$的封闭向量子空间，本身是可度量和完备的。 G 在 E 上的投影 $z \mapsto \mathrm{pr}_1(z)$ 是双射连续线性映射，因此同构 (cor. 1)；因为它的逆映射是$x \mapsto (x, u(x))$，所以$u$在E中是连续的。

我们可以用下面的形式来表达这个推论：如果满足以下情况，$u$是连续的：如果E的点的序列$(x_n)$都收敛到0并且*使得序列*$(u(x_n))$*收敛到* $y$，那么必然是$y = 0$。

#### 例 {#evt-i-s3-n3-exa-1 .statement tag=07AE}

— 令 E 为 $I = [0, 1]$ 上定义的实值函数的空间向量子空间；令E上的$\| f \|$为范数，在此情况下E是*完全*的，并且其拓扑是更细，而不是简单收敛的拓扑。进一步假设函数的 E 包含集合 $\mathscr{C}^\infty(I)$ 在 I 上无限可微；我们将证明存在整数$k \geq 0$，使得所有函数的E包含集合$\mathscr{C}^k(I)$在I中具有连续的第$k$导数。

对于整数$m > 0,\ n \geq 0$的每个对，令$V_{mn}$为函数$f \in \mathscr{C}^\infty(I)$的集合，这样对于$0 \leq h \leq n$和所有$x \in I$来说$|f^{(h)}(x)| \leq 1/m$。 $V_{m,n}$ 形式 0 的邻域的基本系统对于可测量的拓扑与 $\mathscr{C}^\infty(I)$ 的向量空间结构兼容，进一步$\mathscr{C}^\infty(I)$ 在这个拓扑中是“完整的”（FVR， II，p. 2，第 1)。设E中$u$为$\mathscr{C}^\infty(I)$的典范映射；我们证明 $u$ 是*连续的*。来自科。上面的5足以证明，如果序列$(f_n)$在$\mathscr{C}^\infty(I)$中收敛到0，在E中收敛到极限$f$，那么必然是$f = 0$。但这是直接的，因为通过假设，$f$是$(f_n)$的简单收敛极限。因此存在整数$k \geq 0$和数$a > 0$使得关系

$$
p_k(f) = \sup_{\substack{x \in I \\ 0 \leq h \leq k}} |f^{(h)}(x)| \leq a
$$

意味着所有 $f \in \mathscr{C}^\infty(I)$ 都有 $\| f \| \leq 1$。

但是$p_k$是空间$\mathscr{C}^k(I)$上的范数，而$\mathscr{C}^\infty(I)$是子空间，对于这个范数来说，它在$\mathscr{C}^k(I)$中处处稠密（多项式的集合已经在$\mathscr{C}^k(I)$中处处稠密，维尔斯特拉斯石直接的推论定理）。通过之前，$\mathscr{C}^\infty(I)$的恒等映射（携带范数$p_k$）在E中是连续的，因此可以连续扩展到整个空间$\mathscr{C}^k(I)$（因为E是完备的）。这证明了我们的断言。

#### 命题 1 {#evt-i-s3-prop-1 .statement tag=07AF}

*设 E、F 是非离散值除法环 K 上的两个拓扑向量空间。我们假设：*

1) E *是可度量的且完整的*。
2) *在 K 上存在序列* $(F_n)$ *完全可度量向量空间，并且对于每个 n，F 中存在一个单射连续线性映射* $v_n$ *of* $F_n$ *，使得 F 是子空间* 的并* $v_n(F_n)$。

*然后设 u 为 F 中 E 的线性映射。如果 u 的图在* $E \times F$ 中闭合，*则存在整数 n 和 E 在* $F_n$ *中的连续线性映射* $u_n$ *使得* $u = v_n \circ u_n$ *（这意味着 u 是连续的并且* $u(E) \subset v_n(F_n)$).*

令 G 为$E \times F$ 中$u$ 的图。对于所有$n$，我们考虑$E \times F$中$E \times F_n$的连续线性映射$w_n : (x, y) \mapsto (x, v_n(y))$；由于 G 是闭集，集合 $w_n^{-1}(G) = G_n$ 是 $E \times F_n$ 的闭集向量子空间；如果$p_n$是第一个投影$\mathrm{pr}_1$的限制到$G_n$，我们有$p_n(G_n) = u^{-1}(v_n(F_n))$。由于 $p_n$ 是连续的且 $G_n$ 是完备的（因为 $G_n$ 在完备的空间 $E \times F_n$ 中是封闭的），$p_n(G_n)$ 到定理 1，要么是 E 中的微不足道，要么是 E 的全部。但是，到假设时，E 是$p_n(G_n)$的并，并且由于E是完整的，所以Baire的定理在E中$p_n(G_n)$不能都是微不足道的（GT，IX, § 5.3，第1）。因此存在整数 n 使得$p_n(G_n) = E$，或其他字 $u(E) \subset v_n(F_n)$。进一步，由于$v_n$是单射的，$G_n$是E在$F_n$中的线性映射$u_n$的图，由闭图定理(I，p. 19，cor.5)$u_n$是*连续的*；然后从定义得出$u = v_n \circ u_n$。

习题

### 习题{#evt-i-s3-exercises}

§ 3](exercises/s3/)参见[习题。
