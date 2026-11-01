---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 1
section_title: Topological vector spaces
lang: zh
source: evt-i-v
pdf_pages: 0009-0019, 0030-0033
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a topological vector space
      page: 0
      pdf_page: 9
    - "no": 2
      title: Normed spaces on a valued division ring
      page: 3
      pdf_page: 11
    - "no": 3
      title: Vector subspaces and quotient spaces of a topological vector space; products of topological vector spaces; topological direct sums of subspaces
      page: 4
      pdf_page: 12
    - "no": 4
      title: Uniform structure and completion of a topological vector space
      page: 5
      pdf_page: 13
    - "no": 5
      title: Neighbourhoods of the origin in a topological vector space over a valued division ring
      page: 6
      pdf_page: 14
    - "no": 6
      title: Criteria of continuity and equicontinuity
      page: 8
      pdf_page: 16
    - "no": 7
      title: Initial topologies of vector spaces
      page: 9
      pdf_page: 17
statements: 27
exercises: 14
content_sha256: 2a92a232991071800877eac152e82f5f37ae7c14256a2f53f5ad08887cf4e51f
translated_from: content/en/evt/I/01_s1_topological_vector_spaces.md
translation_method: google
source_content_sha256: 99f7362e5facc0f5a48166a8143125835c4c5eb7fc7a7fc95d4ea773e2bc3c95
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: d0216f92c0a9bb02ab0685c2c691adf4ac802e11bc206c663ffe031b83f3e71b
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。拓扑向量空间

### 1. 拓扑向量空间的定义

#### 定义 1 {#evt-i-s1-def-1 .statement tag=077V}

— *给定拓扑划分环* $\mathbf{K}$ (GT, III, § 6.7) *和集合* $E$ *使得* $E$ *有*
* $\mathbf{K}$ 上的左向量空间 $1^\circ$ *结构；
$2^\circ$ *拓扑与* $E$ (GT, III, § 1.1) * 的加法群结构和加法中的满足兼容以下公理：*
*(EVT)* *映射* $(\lambda, x) \mapsto \lambda x$ *of* $\mathbf{K} \times E$ *在* $E$ *是连续的，* *则* $E$ *被称为左拓扑向量空间在*（或在）$\mathbf{K}$上。

等价于说，$E$是一个*拓扑左*$\mathbf{K}\text{-module}$（GT，III, § 6.6）。
如果拓扑和 $E$ 的加法群结构兼容，并且如果在加法中，则相对于 $\mathbf{K}$ 的左向量空间结构和集合 $E$ 上的给定拓扑被称为“相容的”公理（EVT）是有效的。 这与说相同，$E$中$E \times E$和$\mathbf{K} \times E$的两个映射$(x, y) \mapsto x + y$和$(\lambda, x) \mapsto \lambda x$分别是连续的，因此映射$x \mapsto -x = (-1)x$是连续的并且$E$的拓扑是兼容的及其加法群结构。

如果$E$是$\mathbf{K}$上的左拓扑向量空间，我们说$E$仅提供其向量空间结构，*底层*拓扑向量空间$E$。

#### 例 {#evt-i-s1-n1-exa-1 .statement tag=077W}

— 1) 如果$E$在*离散*拓扑划分环$\mathbf{K}$上是左向量空间，则$E$上的*离散*拓扑与$E$的向量空间结构兼容（如果$\mathbf{K}$则情况并非如此）是非离散的，且 $E$ 不是单个点 0)。
2) 令$A$为拓扑环（GT，III, § 6.3），并令$\mathbf{K}$为$A$的子环，这也是环的除法，使得拓扑由$A$在$\mathbf{K}$上诱发与$\mathbf{K}$的除法环结构兼容；那么$A$的拓扑与$\mathbf{K}$上的左向量空间结构兼容。
3) 令$\mathbf{K}$为任意拓扑划分环，且$I$为任意集合。在乘积向量空间 $K_s^I(A, II, § 1.5)$ 上，乘积拓扑与向量空间结构（GT、III, § 6.4）相容的。或者我们可以说，$\mathbf{K}$中$I$的映射的空间$K_s^I$通过*逐点*或*简单收敛*拓扑是$\mathbf{K}$上的拓扑向量空间（TG，X， p. 4）。
4) 设$X$为拓扑空间；在 $X$ 上定义的有限实值 *连续* 函数的集合 $E = \mathscr{C}(X; \mathbf{R})$ 上，*紧收敛* 拓扑 (GT, X, § 1.3) 与 E 在 $\mathbf{R}$ 上的向量空间结构兼容。例如，令$u_0$为E的点，令H为X的紧子集，且$\varepsilon$为任意严格正数。实值函数 $u_0$ 有界于 H ；让$a = \sup_{t \in H} |u_0(t)|$；如果 $u$ 是 E 的任意点那么对于所有 $t \in H$

$$
|\lambda u(t) - \lambda_0 u_0(t)| \leq |\lambda| \cdot |u(t) - u_0(t)| + a |\lambda - \lambda_0|.
$$

因此，如果$|\lambda - \lambda_0| \leq \varepsilon$和$|u(t) - u_0(t)| \leq \varepsilon$对于所有$t \in H$，那么对于$t \in H$，
$|\lambda u(t) - \lambda_0 u_0(t)| \leq \varepsilon (\varepsilon + |\lambda_0| + a)$，表明满足公理（EVT）；类似地可以验证紧收敛拓扑与E的加法群结构兼容。

另一方面，如果 X 不是紧致的，则 *一致收敛* 拓扑（在 X 中）不一定与 E 的向量空间结构兼容；对于例，如果$X = \mathbf{R}$且$u_0$是$\mathbf{R}$中的无界连续函数，则E中$\mathbf{R}$的映射$\lambda \mapsto \lambda u_0$在E上的一致收敛拓扑中不是连续的。

5) 令 E 为拓扑划分环 K 上的有限维 $n$ 的向量空间；存在向量 K 空间中的同构 $u : K_s^n \to E$，而且，如果 $v$ 是 E 上$K_s^n$ 的第二个同构，那么我们可以写 $v = u \circ f$，其中 $f$ 是向量的自同构 K-空间$K_s^n$。考虑在 $K_s^n$ 上，*乘积* 拓扑与其向量空间结构 (*例 3*) 相容的；由于$K_s^n$的每个线性映射本身对于这个拓扑来说都是连续的，因此向量空间$K_s^n$的每个自同构都是*双连续*。因此，如果我们将$K_s^n$的乘积拓扑*转移*到E，通过E上的$K_s^n$中的任何同构，在E上获得的拓扑是*独立于所使用的特定同构；我们称其为 E 上的*规范拓扑* ；当 K 是带有估值的非离散完全除法环时，我们将对其进行不同的描述（I, § 1.3）。 K 上的拓扑向量空间中 E 的每个线性映射对于 E 上的规范拓扑都是*连续的。

与 def 中的方式相同。 1、可以定义K上的*右*拓扑向量空间，拓扑划分环；但 K 上的每个右向量空间都可以被视为与 K (A, II, § 1.1) 相对的除法环 $K^0$ 上的左向量空间，并且 K 的拓扑与除法环 $K^0$ 的结构兼容。因此我们通常只考虑左拓扑向量空间 ；当我们无条件地谈论“拓扑向量空间”时，可以理解我们指的是左向量空间。

如果 K' 是 K 的子划分环，并且 E 是 K 上的拓扑向量空间，则显然 E 的拓扑仍然与 E 相对于 K' 的向量空间结构兼容，这是通过将标量的域限制为 K' 获得的；我们说，通过此过程获得的 K' 上的拓扑向量空间 *是 K 上的拓扑向量空间 E 的基础。

在阶中，拓扑向量空间 E 为 *Hausdorff*，对于 E 的所有 $x \neq 0$，存在 0 的邻域而不是包含 $x$ (GT, III, § 1.2) 是充分必要的。

考虑拓扑，在向量空间 E 上的拓扑划分环 K，与 E 的加法群结构兼容。由于恒等式

$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0) x_0 + \lambda_0 (x - x_0) + (\lambda - \lambda_0) (x - x_0)
$$

公理（EVT）等价于以下三个公理中的系统。

*(EVT$_1'$)* *对于所有* $x_0 \in E$，*映射* $\lambda \mapsto \lambda x_0$ *在* $\lambda = 0$ 处连续。

*(EVT$_2'$)* *对于所有* $\lambda_0 \in K$，*映射* $x \mapsto \lambda_0 x$ *在* $x = 0$ 处连续。

*(EVT$_3'$)* *映射* $(\lambda, x) \mapsto \lambda x$ *在* $(0, 0)$ 连续。

特别是：

#### 命题 1 {#evt-i-s1-prop-1 .statement tag=077X}

— 对于所有 $\alpha \in K$ 和每个点 $b \in E$，$E$ 的映射 $x \mapsto \alpha x + b$ 本身是连续的。此外，如果$\alpha \neq 0$，则这个映射是$E$自身的同胚。

命题的第二个部分是这样的结果：如果 $\alpha \neq 0$，则 $x \mapsto \alpha^{-1}x - \alpha^{-1}b$ 是 $x \mapsto \alpha x + b$ 的逆映射。

#### 推论{#evt-i-s1-n1-cor-1 .statement tag=077Y}

— 如果 $A$ 在 $E$ 中是开（或闭）集合，则对于 $K$ 中的每个 $\alpha \neq 0$，$\alpha A$ 在 $E$ 中是开（或闭）。

设$E$和$F$是同一拓扑划分环$K$上的两个拓扑向量空间。 $F$上$E$的双射$f$是拓扑向量空间$F$上拓扑向量空间$E$的同构当且仅当$f$是线性且双连续的。特别地，如果$K$的$\gamma \neq 0$属于到中心，则位似$x \mapsto \gamma x$是$E$的拓扑向量空间结构的自同构。

### 2. 标准化空间在有价值的除法环上

回想一下（GT，IX, § 3.2），环$K$上的绝对值是$\mathbf{R}_+$中$K$的映射$\xi \mapsto |\xi|$，使得$|\xi| = 0$当且仅当$\xi = 0$，还有$|\xi \eta| = |\xi| \cdot |\eta|$和$|\xi + \eta| \leq |\xi| + |\eta|$； $K$上的绝对值定义距离$|\xi - \eta|$，因此豪斯多夫拓扑与$K$的除法环结构兼容。如果$|\xi| = 1$对所有$\xi \neq 0$来说，绝对的值称为不恰当的，而拓扑则称它在$K$上的定义是离散的拓扑；另一方面，如果$K$中存在$\alpha \neq 0$使得$|\alpha| \neq 1$，则$K$中存在$\beta \neq 0$使得$|\beta| < 1$（取$\beta = \alpha$或$\beta = \alpha^{-1}$就足够了），并且序列 $(\beta^n)_{n \geq 1}$收敛于0，因此$K$的拓扑不是离散的。

另一方面（GT，IX, § 3.3），如果$E$在非离散值除法环$K$上是向量空间，那么$E$上的范数是映射$x \mapsto \|x\|$ $\mathbf{R}_+$中的$E$，使得$\|x\| = 0$当且仅当$x = 0$，并且使得$\|\lambda x\| = |\lambda| \cdot \|x\|$对于每个标量$\lambda \in K$和$\|x + y\| \leq \|x\| + \|y\|$。距离$\|x - y\|$由范数在$E$上定义，因此拓扑与$E$的向量空间结构兼容（前述）。 除非相反，明确指出，范数空间被认为是由其范数定义的拓扑向量空间的结构的项。规范化的空间是最重要的拓扑向量空间之一。

已知（GT，IX, § 3.3），$E$上的两个不同的范数可以在$E$上定义相同的拓扑；为此，两个范数相等是必要且充分的（参见上文）。因此，范数空间的结构比拓扑向量空间的结构更丰富；如果$E$和$F$是两个范数空间，则必须小心区分$E$范数空间结构的同构思想与$F$的同构思想， $E$的拓扑向量空间结构与$F$的拓扑向量空间结构。

#### 例 {#evt-i-s1-n2-exa-1 .statement tag=077Z}

令I为指标的任意一个集合；已知（GT，X, § 3.2）范数$\|x\|$可以在K，$\mathscr{B}(I; K)$（也写为$\mathscr{B}_K(I)$或$\ell_K^\infty(I)$）中的I有界映射$x = (\xi_i)$的集合上定义， $\|x\| = \sup_{i \in I} |\xi_i|$。当I是拓扑空间时，K中I的有界连续映射的集合是空间$\mathscr{B}(I; K)$的闭子空间（GT，X, § 3.1，cor.2）。 $\mathscr{B}(I; K)$的另一个子空间是绝对可和族$x = (\xi_i)$的集合$\ell_K^1(I)$（GT，X, § 3.6）；我们可以对这个子空间另一个范数$\|x\|_1 = \sum_{i \in I} |\xi_i|$定义，一般来说不等于范数$\|x\| = \sup_{i \in I} |\xi_i|$（I，p. 23，练习6）；当将 $\ell_K^1(I)$ 视为规范的空间时，如果不指定其范数，则它始终是范数 $\|x\|$。我们写 $\mathscr{B}(I)$ 和 $\ell^1(I)$ 来代替 $\mathscr{B}(I; \mathbf{R})$ 和 $\ell_R^1(I)$。

### 3. 拓扑向量空间的向量子空间和商空间；拓扑向量空间的乘积； 子空间的拓扑直和

对于拓扑模（GT，III, § 6.6）所说的一切都特别适用于拓扑向量空间。如果 M 是拓扑向量空间 E 的向量子空间，则 E 的拓扑在 M 上诱导的拓扑与 M 的向量空间结构兼容，并且 E 中 M 的闭包 $\overline{M}$ 是 E 的向量子空间。 M 的 E 的拓扑与 E/M 的向量空间结构兼容。

如果E是拓扑向量空间，则E中$\{0\}$的闭包N（0的邻域的交）是E的闭向量子空间；商向量子空间 E/N，无论 E 是否存在，都必然是 Hausdorff，被称为与 E 相关的 Hausdorff 向量空间。

令$(E_i)_{i \in I}$为同一拓扑划分环K上的拓扑向量空间族，并令E为$E_i$的乘积向量空间。 $E_i$拓扑的乘积拓扑与E的向量空间结构兼容。在乘积空间E，子空间F，直和处$E_i$处处稠密（GT， III, § 2.9，第 25 条）。

对于拓扑向量空间在域$\mathbf{R}$或域$\mathbf{C}$上的某些型，我们在$(E_i)$的直和上定义（在II，p. 29）拓扑拓扑向量空间，一般来说，与$E_i$的乘积拓扑诱导的拓扑不同。

关于带有运算符（GT，III, § 6.2）的拓扑群的稳定子群的有限直和所说的一切都适用于《向量子空间》中的拓扑向量空间，替换“稳定子群”。

#### 注 {#evt-i-s1-n3-rem-1 .statement tag=0780}

给定 Hausdorff 拓扑向量空间 E 的封闭向量子空间 M，不一定存在 E 中封闭的 M 的（代数）互补向量子空间（即使 E 是范数空间；cf. IV， p. 55，执行 16 (c))； 更不必说 E 中不一定存在 M 的拓扑补集（cf. I，p. 26，练习 8）。然而，我们将在§ 2中看到，当K是非离散值除法环时，则E的每个闭子空间M，与有限余维，在E中确实有一个拓扑补（I，p. 14，命题3）。

### 4. 统一结构并完成拓扑向量空间

由于拓扑向量空间 E 的拓扑与E 上的加法群结构兼容，因此定义是E 上的一致结构 (GT, III, § 3)；当我们谈到拓扑向量空间的一致结构时，我们总是指的是结构除非，但明确指出了相反的情况。拓扑向量空间 F 中拓扑向量空间 E 的每个连续线性映射都是一致连续的（GT，III, § 3.1，第 3 条）； 形式 $x \mapsto \alpha x + b$ 的 E 本身的每个映射都是一致连续的。 F 中 E 的线性映射等连续集合一致等连续（GT，X, § 2.2，道具 5）。

#### 注 1 {#evt-i-s1-n4-rem-1 .statement tag=0781}

如果 B 是 K 的预压缩集合，则对于 E 中每个 0 的邻域 V，E 中存在 0 的邻域 U，使得 BU $\subset$ V。对于，如果 W 是 E 中 0 的邻域，则 W + W $\subset$ V；那么从 (EVT$_{\text{III}}$) 中，K 中存在 0 的邻域 T$_0$ 和 E 中 0 的邻域 U$_0$，使得 T$_0$U$_0$ $\subset$ W。由于 B 是预紧的，因此存在有限多个点 $\lambda_i \in B$ ($1 \leq i \leq n$)使得$\lambda_i + T_0$覆盖B；从 (EVT$_{\text{II}}$) 可以得出，E 中存在 0 的邻域 U $\subset$ U$_0$，因此对于所有 $i$ 都有 $\lambda_i U \subset W$；显然 U 具有所需的属性。以类似的方式（使用（EVT$_{\text{I}}$）而不是（EVT$_{\text{II}}$））可以证明，如果H是E的预紧集合，则对于E中每个0的邻域V，K中存在0的邻域T，使得TH$\subset$ V。

#### 注 2 {#evt-i-s1-n4-rem-2 .statement tag=0782}

从 1) 可以得出，如果 B 是 K 的预紧集合并且 H 是 E 的预紧集合，则映射 $(\lambda, x) \mapsto \lambda x$ 限制为 B $\times$ H 是一致连续的。例如，如果 E 中 V 为 0 的邻域，则 K 中存在 0 的邻域 T，E 中存在 0 的 U，使得 TH + BU $\subset$ V。由于我们可以写出$\lambda x - \lambda' x' = (\lambda - \lambda') x + \lambda'(x - x')$，我们看到对于B中的$\lambda, \lambda'$，H中的x，x'，$\lambda - \lambda' \in T$和$x - x' \in U$，我们有$\lambda x - \lambda' x' \in V$，这证明了我们的断言。

如果考虑到其一致结构，拓扑向量空间是完全一致空间，则称其为完全一致向量空间。

#### 定义 2 {#evt-i-s1-def-2 .statement tag=0783}

*非离散值除法环上的完全赋范空间称为 Banach 空间。*

#### 例 {#evt-i-s1-n4-exa-1 .statement tag=0784}

如果 K 是非离散值除法环，则空间 $\mathscr{B}(I ; K)$ (I, p. 4, 例) 是完整的 (GT, X, § 3.1, cor. 1)。对于空间 $\ell_K^1(I)$ (I, p. 4, 例) 和范数 $\|x\|_1 = \sum_{i \in I} |\xi_i|$ 也是如此：对于，如果 $x_n$ 是这个空间和 $x_n = (\xi_{m_i})_{i \in I}$ 中的柯西序列，那么对于所有$i \in I$

$$
|\xi_{m_i} - \xi_{n_i}| \leq \|x_m - x_n\|_1;
$$

因此，对于每个$i \in I$，序列$(\xi_{m_i})_{n \geq 1}$收敛到K中的极限$\xi_i$。此外，对于I的每个有限子集J

$$
\sum_{i \in J} |\xi_{m_i} - \xi_{n_i}| \leq \|x_m - x_n\|_1;
$$

紧接着，存在一个常数 $a > 0$，与 J、m、n 无关，使得 $\sum_{i \in J} |\xi_{m_i} - \xi_{n_i}| \leq a$。令m趋于$+ \infty$，由$\sum_{i \in I} |\xi_i| \leq a + \|x_n\|_1$推导出$\sum_{i \in J} |\xi_i - \xi_{m_i}| \leq \varepsilon$，即$z = (\xi_i)_{i \in I}$属于到$\ell_K^1(I)$；此外，对于所有$\varepsilon > 0$，都存在$n_0$，因此对于$n \geq n_0$和I的每个有限集合 J，我们有$\sum_{i \in J} |\xi_i - \xi_{m_i}| \leq \varepsilon$；相对于I的有限子集有向集合，经过到极限，我们看到$\|z - x_n\|_1 \leq \varepsilon$对于$n \geq n_0$，这表明$z$是序列$(x_n)$的极限标准空间$\ell_K^1(I)$。

令$K$为豪斯多夫拓扑除法环，$E$为$K$上的拓扑向量空间，并假设完整的环$\hat{K}$是*除法环*（当$K$是值除法时就是这样环, GT, IX, § 3.3) 那么$E$的Hausdorff补全$\hat{E}$携带$\hat{K}$上的*完全拓扑向量空间*的结构 (GT, III, § 6.5);我们说$\hat{E}$和结构是拓扑向量空间$E$的*豪斯多夫完成*，或者当$E$是*豪斯多夫*时，$E$的*完备的*。

### 5. 拓扑向量空间中的原点邻域在有价值的除法环上

#### 定义 3 {#evt-i-s1-def-3 .statement tag=0785}

*令$K$为环和$E$左向量空间除以$K$；我们说$E$的子集$M$是平衡的，如果对于所有$x \in M$和所有$\lambda \in K$使得$|\lambda| \leq 1$，$\lambda x \in M$为真（或者在其他字如果$\lambda M \subset M$当$|\lambda| \leq 1$).*

#### 命题 2 {#evt-i-s1-prop-2 .statement tag=0786}

*在有值除法环$K$上的拓扑向量空间$E$中，平衡集合$M$的闭包是平衡集合。*

如果$B$是$\xi \in K$的集合和$|\xi| \leq 1$；那么$B$在$K$关闭。但$B \times M$通过连续的映射$(\lambda, x) \mapsto \lambda x$映射到$M$；因此$B \times \overline{M}$映射到$\overline{M}$（GT，I, § 2.1，第1），这证明$\overline{M}$是平衡的。

当 $M$ 是向量空间 $E$ 中的任意集合时，$\lambda x$ 与 $x \in M$ 和 $\lambda \in K$ 的定值除法环 $K$、集合 $M_1$ 使得$|\lambda| \leq 1$，显然是最小的平衡集合包含$M$； $M_1$ 称为 $M$ 的*平衡包络*。

#### 命题 3 {#evt-i-s1-prop-3 .statement tag=0787}

*令 $K$ 为局部紧致非离散除法环，$E$ 为 $K$ 上的 Hausdorff 拓扑向量空间（或拓扑向量空间）。对于 $E$ 中的每个紧致（或预紧致）集合 $H$，$H$ 的平衡包络是紧致的（或预紧致）。

如果$B$表示$K$中的球$|\xi| \leq 1$，则$H$的平衡包络线为$H_1$，连续映射$m : (\lambda, x) \mapsto \lambda x$下$B \times H$的像。如果 $E$ 是 Hausdorff，如果 $B$ 是紧的，并且如果 $H$ 是紧的，那么 $B \times H$ 也是紧的，因此 $H_1$ 也是紧的。如果 $H$ 是预紧，则 $m$ 到 $B \times H$ 的限制是均匀连续的（I、p. 5、*注* 2），并且由于 $B \times H$ 是预紧，因此它的像也是预紧的$m$（GT，II, § 4.2，道具 2）。

注闭合集合的平衡包络线不一定是闭合的。对于例，在$\mathbf{R}^2$中，由方程$xy = 1$定义的双曲线的平衡包络线不是封闭的。

$E$中的平衡集合族中的并是平衡的，这意味着对于$E$的每个集合$M$，$M$的最大的平衡子集$N$称为*的平衡核心* $M$；当且仅当$0 \in M$时$N$不为空。说$x \in N$意味着对于所有$\lambda \in K$使得$|\lambda| \leq 1$，我们有$\lambda x \in M$，或者再次（如果$0 \in M$）对于所有带有|μ|的$\mu \in K$ ≥ 1，我们有 x ∈ μM。如果 0 ∈ M，则 M 的平衡核心 N 为交 $\bigcap_{|\mu| \geq 1} \mu M$。这特别表明，如果 M 是封闭的，那么 N 也是封闭的。

#### 定义 4 {#evt-i-s1-def-4 .statement tag=0788}

*设 K 为非离散值除法环，E 为 K 上的左向量空间，具有两个子集 A 和 B。如果存在 α > 0，则对于每个 λ ∈ K 且 |λ|，我们说 A 吸收 B，使得 λA ⊃ B ≥ α（或等效地，如果 μB ⊂ A，μ ≠ 0 且 |μ| ≤ α⁻1）。如果 E 的集合 A 吸收单个点的每集合由……组成，则称为吸收剂。*

设A是E的平衡集合；为了让它吸收 E 的集合 B，只要存在 λ ≠ 0 使得 λA ⊃ B 就足够了；事实上，对于 |μ| ≥ |λ|，我们有 λA = (λμ⁻1) μA，并且由于 μA 是平衡的并且 |λμ⁻1| ≤ 1，则 λA ⊂ μA，因此 B ⊂ μA。特别是对于 E 的平衡集合 A 来说，对于每个 x ∈ E，K 中存在 λ ≠ 0 使得 λx ∈ A 是必要且充分的。E 生成向量空间 E 的每个吸收剂集合。吸收剂集合的每个有限交都是一个吸收剂集合。

#### 命题 4 {#evt-i-s1-prop-4 .statement tag=0789}

*在非离散值除法环 K 上的拓扑向量空间 E 中，存在 0 的闭邻域的基本系统 $\mathfrak{B}$，使得：
*(EV₁)* 每个集合 V ∈ $\mathfrak{B}$ 都是平衡且吸收性的。
*(EV2)* 对于 K 中的每个 V ε $\mathfrak{B}$ 且 λ ≠ 0，我们有 λV ε $\mathfrak{B}$（$\mathfrak{B}$ 在非零比率的相似性下的不变性）。
*(EV₃)* 对于每个 V ∈ $\mathfrak{B}$，存在 W ∈ $\mathfrak{B}$ 使得 W + W ⊂ V。

相反，令 E 为 K 上的向量空间，并令 $\mathfrak{B}$ 为 E 满足条件 (EV₁)、(EV2) 和 (EV₃) 上的滤波器基。那么E上存在拓扑（并且是唯一的），与E的向量空间结构兼容，并且$\mathfrak{B}$是0的邻域的基本系统。

通过公理（EVT'₃），我们首先证明*平衡核心*，V的V₁，0的邻域本身就是0的邻域。 因为存在 α > 0 且邻域 W 为 0，因此，如果 |λ| ≤ α 且 x ∈ W，则 λx ∈ V。 由于 K 是非离散的，因此 K 中存在 μ ≠ 0，其中 |μ| ≤ α 且 μW 为 0 的邻域，其中 μW ⊂ V。 另外，如果 v ∈ K 且 |v| ≤ 1 则|vμ| ≤ α，因此 vμW ⊃ V。 因此 μW ⊃ V₁ 和 V₁ 是 0 的邻域。 由于 V 是封闭的，所以 V₁ 也是封闭的。 因此，在 E 中，*封闭平衡* 邻域 0 形式的集合 $\mathfrak{B}$ 是 0 的邻域基本系统。 由 (EVT₁') 0 的每邻域都是*吸收性*；此外，$\mathfrak{B}$满足（EV2）（*cf.*I，p. 3，cor.）；最后，由于 (x, y) ↦ x + y 在点 (0, 0) 处的连续性，E 中 0 的邻域的每个基本系统都满足 (EV₃)。 集合$\mathfrak{B}$满足命题中的条件。

现在让 E 为 K 上的向量空间，并且 $\mathfrak{B}$ 为 E 满足 (EV₁)、(EV2) 和 (EV₃) 上的滤波器基。公理 (EV₁) 首先表明，对于所有 V ∈ $\mathfrak{B}$，我们有 −V = V 且 0 ∈ V；这些关系和公理（EV₃）表明$\mathfrak{B}$是0的邻域的基本系统，对于E上的拓扑与E的*加法群* 结构兼容（GT，III, § 1.2）。另一方面，公理(EVT'_I)、(EVT'_II)和(EVT'_III)是(EV_I)和(EV_II)的直接的推论，因此上面定义的拓扑满足公理(EVT)，并且命题被证明。

#### 注 1 {#evt-i-s1-n5-rem-1 .statement tag=078A}

在具有中心 0 的开球（分别为闭球）的非离散值划分环集合的规范空间中，中心 0 是 0 的邻域的基本系统，其中满足条件 (EV_I)、(EV_II) 和(EV_III)。

#### 注 2 {#evt-i-s1-n5-rem-2 .statement tag=078B}

当标量 K 的除法环为域 \mathbf{R} 或域 \mathbf{C} 时，E 上仅满足两个公理 (EV_I) 和 (EV_III) 的每个过滤器基 \mathfrak{B} 都是基本系统 0的邻域的拓扑与E的向量空间结构兼容。事实上，我们只需要证明，在这些条件中，对于K中的每个$\lambda \neq 0$和每个$V \in \mathfrak{B}$，都存在$W \in \mathfrak{B}$使得$\lambda W \subset V$。现在从 (EV_III) 存在 $W_1 \in \mathfrak{B}$ 和 $2\,W_1 \subset V$，我们归纳推断，对于每个正整数 $n$，都存在 $W_n \in \mathfrak{B}$ 使得 $2^n W_n \subset V$。由于V是平衡的，如果我们取$n$大到$2^n = |2^n| > |\lambda|$，那么$W = W_n$满足条件，如所要求的。

这个结果并不适用于每个非离散值除法环 K，因为在这样的除法环中，对于每个正整数$m$，$|m\varepsilon| = m$不再一定成立（$\varepsilon$表示除法环的单位元；cf.） I，p. 22，练习 1)。

#### 注 3 {#evt-i-s1-n5-rem-3 .statement tag=078C}

如果 K 是离散除法环，则条件 (EVT'_I) 和 (EVT'_III) 对于 E 上的任何拓扑均成立。由图4可知，如果E是K上的拓扑向量空间，则E满足条件(EV_II)和(EV_III)中存在$\mathfrak{B}$，即0的闭邻域的基本系统。相反，如果向量空间 E 上的 K 上的过滤器基 $\mathfrak{B}$ 使得 0 属于到 $\mathfrak{B}$ 和 (EV_II)、(EV_III) 的所有集合为真，则 $\mathfrak{B}$ 是邻域的基本系统拓扑中的 0 与 E 的向量空间结构兼容。

### 6. 判据连续性和等连续性

令 E 和 F 是同一划分环 K 上的拓扑向量空间 ；为了使 F 中的 E 的线性映射 $f$ 连续，只要它在原点连续就足够了（GT，III, § 2.8，第 23 条）。这个命题概括如下：

#### 命题 5 {#evt-i-s1-prop-5 .statement tag=078D}

— 令 $E_i (1 \leq i \leq n)$ 和 F 在非离散值域 K 上是拓扑向量空间。在阶中，F 中 $\prod_{i=1}^n E_i$ 的多线性映射 $f$ 应在乘积空间 $\prod_{i=1}^n E_i$ 中连续，足以使其连续于$(0, 0, ..., 0)$。

令$(a_1, a_2, ..., a_n)$为$\prod_{i=1}^n E_i$的任意点；我们必须证明，对于 F 中 0 的每个邻域 W，$E_i$ ($1 \leq i \leq n$) 中存在 0 的邻域 $V_i$，使得关系 $z_i \in V_i$ 意味着

$$
f(a_1 + z_1, a_2 + z_2, ..., a_n + z_n) - f(a_1, a_2, ..., a_n) \in W .
$$

现在，我们可以写

$$
f(a_1 + z_1, ..., a_n + z_n) - f(a_1, ..., a_n) = \sum_H u_H
$$

其中$H$在整数$\{ 1, 2, ..., n \}$的集合的$2^n - 1$子集上变化，不包括集合$\{ 1, 2, ..., n \}$本身，并且其中$u_H = f(y_1, y_2, ..., y_n)$，如果$i \in H$则为$y_i = a_i$且$y_i = z_i$ 如果$i \notin H$。 $F$中存在0的$2^n - 1$平衡邻域$W_H$使得$\sum_H W_H \subset W$；另一方面，由于$f$在$(0, 0, ..., 0)$处连续假设，因此每个$E_i$邻域$U_i$都存在0（$1 \leq i \leq n$），因此$n$关系$x_i \in U_i$意味着$f(x_1, ..., x_n) \in \bigcap_H W_H$。由于$U_i$具有吸收性，因此$K$中存在$\lambda_i \neq 0$，从而$\lambda_i a_i \in U_i$。令$\lambda$为$K$的元素，使得每个子集$H$都有$|\lambda| \geq \prod_{i \in H} |\lambda_i|^{-1}$；我们证明邻域$V_i = \lambda^{-n} U_i$满足要求的条件。我们可以将$1 \leq i \leq n$和$\mu = \lambda^{-np} (\prod_{i \in H} \lambda_i^{-1})$写成$u_H = \mu f(x_1, ..., x_n)$，其中$x_i \in U_i$，$p$是$\{ 1, 2, ..., n \}$的整数的数，不在$H$中。从上面的$|\mu| \leq 1$，因此$u_H \in \mu W_H \subset W_H$，因为$W_H$是平衡的。 命题成立。

#### 命题 6 {#evt-i-s1-prop-6 .statement tag=078E}

*对 $E_i (1 \leq i \leq n)$ 和 $F$ 的假设与道具中相同。 5、在$F$中$\prod_{i=1}^n E_i$的多线性映射集合$\mathscr{E}$在阶中等连续，集合在$(0, 0, ..., 0)$等连续就足够了。

对于，在道具的演示中。 5 $U_i (1 \leq i \leq n)$ 可以这样取，使得关系 $x_i \in U_i (1 \leq i \leq n)$ 暗示$f(x_1, ..., x_n) \in \bigcap_H W_H$ 对于*每个* 映射 $f \in \mathscr{E}$。

### 7. 向量空间的初始拓扑

#### 命题 7 {#evt-i-s1-prop-7 .statement tag=078F}

*设 $(E_v)_{v \in I}$ 是拓扑划分环 $K$ 上的拓扑向量空间族。令$E$为$K$上的向量空间，对于每个$v \in I$，令$f_v$为$E_v$中$E$的线性映射。那么$E$上最粗的拓扑使得每个函数$f_v$连续，拓扑$\mathscr{T}$与$E$的向量空间结构兼容。进一步地，如果对于每个$x \in E$，$\phi(x)$表示乘积空间$F = \prod_{v \in I} E_v$的点$(f_v(x))$，则拓扑$\mathscr{T}$是拓扑的逆像子空间 $\phi(E)$ 共 $F$ 线性映射 $\phi$。*

命题的最后一个部分是 GT 的特例，I, § 4.1，道具。 3. 命题接下来是下一个引理。

#### 引理 {#evt-i-s1-n7-lem-1 .statement tag=078G}

— *令$M$和$N$为两个向量空间，以及$N$中$M$的$g$线性映射。如果 $\mathscr{T}_0$ 与拓扑兼容 $N$ 的向量空间结构，则 $\mathscr{T}_0$ 的逆像 $g$ 与 $M$ 的向量空间结构兼容。*

我们证明，对于例，$(\lambda, x) \mapsto \lambda x$在$K \times M$的每个点$(\lambda_0, x_0)$都是连续的。把$y_0 = g(x_0)$。 $M$ 包含邻域形式 $g(U)$ 中的每个邻域为 0，其中 $U$ 为 $N$ 中的 0 邻域；通过假设，$K$中存在0的邻域$V$和$N$中0的邻域$W$，使得关系$\lambda - \lambda_0 \in V$和$y - y_0 \in W$意味着$\lambda y - \lambda_0 y_0 \in U$。因此关系$\lambda - \lambda_0 \in V$，$x - x_0 \in g(W)$意味着$\lambda x - \lambda_0 x_0 \in g(U)$。我们可以类似地证明$(x, y) \mapsto x - y$在$M \times M$中是连续的。

对于每个指标$i \in I$，令$\mathscr{B}_i$是$E_i$中0的邻域的基本系统。从拓扑$\mathscr{T}$的定义，通过族$f_i^{-1}(\mathscr{B}_i)$的集合并生成此拓扑的0的邻域过滤器；在其他形式、$\bigcap_k f_{i_k}^{-1}(V_{i_k})$形式的字、集合中，$\mathscr{T}$为0的基本邻域的系统，$(i_k)_{1 \leq k \leq n}$为指标的任何有限序列 I，并且对于每个指标 $k$，$V_{i_k}$ $\mathscr{B}_{i_k}$ 中的任何集合。

#### 推论 1 {#evt-i-s1-prop-7-cor-1 .statement tag=078H}

*设G是K上的拓扑向量空间。在阶中，E中G的映射的集合H是等连续的，对于所有$i \in I$，当u在H中变化时，集合$f_i \circ u$应该是等连续的。*

这是 GT 的特例，X, § 2.2，道具。 3.

#### 推论 2 {#evt-i-s1-prop-7-cor-2 .statement tag=078I}

*如果空间$E_i$是Hausdorff，那么在阶中$\mathscr{T}$是Hausdorff，对于E中的每个$x \neq 0$，应该存在指标$i \in I$，使得$f_i(x) \neq 0$是充分必要的。

因为$\phi(E)$是Hausdorff空间，并且在阶中$\mathscr{T}$是Hausdorff，显然$\phi$是单射的必要且充分； 注，然后我们可以将认同 E（与$\mathscr{T}$）与$\prod_{i \in I} E_i$的子空间$\phi(E)$乘以映射$\phi$。

#### 推论 3 {#evt-i-s1-prop-7-cor-3 .statement tag=078J}

*假设$E_i$已完成，$\phi(E)$于$F = \prod_{i \in I} E_i$关闭。那么 E 在拓扑 $\mathscr{T}$ 中完成。*

对于 F 的子空间 $\phi(E)$ 则完整（GT，II, § 3.4，第 8 条和 § 3.5，第 10 条），因此逆像拓扑中的 E 也是完整的（GT，I, § 7.6，第 10 条和 GT， II, § 3.1，道具 4)。

#### 例 {#evt-i-s1-n7-exa-1 .statement tag=078K}

— 令 $\mathscr{D}'(\mathbf{R})$ 为 $\mathbf{R}$ 上的分布的空间；对于$p$数使得$1 \leq p \leq +\infty$，令$j : L^p(\mathbf{R}) \to \mathscr{D}'(\mathbf{R})$为典范嵌入，它是连续的（当$L^p(\mathbf{R})$携带其范数空间拓扑和$\mathscr{D}'(\mathbf{R})$强拓扑）。对于每个分布$f \in \mathscr{D}'(\mathbf{R})$，用$D(f)$表示$f$的导数；回想一下，$f \mapsto D(f)$是$\mathscr{D}'(\mathbf{R})$的连续自同态。然后令 E 为 $L^p(\mathbf{R})$ 中的向量子空间，其中 $f \in L^p(\mathbf{R})$ 为 $D(f) \in L^p(\mathbf{R})$，并赋予 E 最粗糙的拓扑，使得典范嵌入 $i : E \to L^p(\mathbf{R})$ 和映射 $D : E \to L^p(\mathbf{R})$ 连续（$L^p(\mathbf{R})$ 带有其规范的空间拓扑）。对于这个拓扑，空间 E 是*完整的*。因为，$F = L^p(\mathbf{R}) \times L^p(\mathbf{R})$中的E的像通过映射$\phi : f \mapsto (f, D(f))$是*封闭的*，因为它是$\mathscr{D}'(\mathbf{R}) \times \mathscr{D}'(\mathbf{R})$中的$\mathscr{D}'(\mathbf{R})$的像G的$L^p(\mathbf{R}) \times L^p(\mathbf{R})$上的迹，通过映射

$$
\phi_0 : f \mapsto (f, D(f));
$$

现在 G 是 $\phi_0$ 的图，因此在 $\mathscr{D}'(\mathbf{R}) \times \mathscr{D}'(\mathbf{R})$ 中闭合（GT，I, § 8.1，第 2 项的相应 2），并且由于 $\phi(E)$ 是 G 的逆像通过 $i \times i$ 的连续，我们看到 $\phi(E)$ 在 F 中闭合。 \*

#### 推论 4 {#evt-i-s1-prop-7-cor-4 .statement tag=078L}

*设E为拓扑划分环K上的向量空间，并令$(\mathscr{T}_i)_{i \in I}$为与E的向量空间结构兼容的拓扑族；那么拓扑$\mathscr{T}_i$的上界$\mathscr{T}$与E的向量空间结构兼容。*

因为，如果$E_t$表示从$E$通过拓扑$\mathscr{T}_t$得到的拓扑向量空间，并且$f_t$表示$E$在$E_t$上的恒等式映射，则$\mathscr{T}$是最粗略的拓扑 $f_t$连续。

### 习题 {#evt-i-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
