---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 5
section_title: Groups operating on a set
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 52-65, 140-147
pdf_pages: 0076-0089, 0164-0171
extraction: ocr
subsections:
    - "no": 1
      title: MONOID OPERATING ON A SET
      page: 52
      pdf_page: 76
    - "no": 2
      title: STABILIZER, FIXER
      page: 54
      pdf_page: 78
    - "no": 3
      title: INNER AUTOMORPHISMS
      page: 55
      pdf_page: 79
    - "no": 4
      title: ORBITS
      page: 56
      pdf_page: 80
    - "no": 5
      title: HOMOGENEOUS SETS
      page: 58
      pdf_page: 82
    - "no": 6
      title: HOMOGENEOUS PRINCIPAL SETS
      page: 60
      pdf_page: 84
    - "no": 7
      title: PERMUTATION GROUPS OF A FINITE SET
      page: 61
      pdf_page: 85
statements: 32
exercises: 29
content_sha256: 72a66888a6774560ccbf0dd66fe2250691ab2ccc62182ac4eef255625076569e
translated_from: content/en/alg/I/05_s5_groups_operating_on_a_set.md
translation_method: google
source_content_sha256: dfbb9d78abb1e74cb8df10a3c8d7099cfe102e2e7a75bb6d300412ab223621fa
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 47ae2aa73c86eb9a43c64fede365a1aa7f44b471de317253e9d06ef5b3d7b97b
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 5。 群运行于集合

### 1. 幺半群在集合上运行

#### 定义 1 {#alg-i-s5-def-1 .statement tag=05B1}

设 M 为幺半群，律乘法书写，单位元素表示为 e，E 集合。如果对于所有$\alpha, \beta \in M$，$f_e = \mathrm{Id}_E$ 和$f_{\alpha \beta} = f_\alpha \circ f_\beta$（或$f_{\alpha \beta} = f_\beta \circ f_\alpha$），M 在 E 上的作用 $\alpha \mapsto f_\alpha$ 称为 M 在 E 上的左（或右）运算。

在其他字中，集合E上幺半群M的左（右）运算是M的幺半群同态进入幺半群$E^E$（分别是$E^E$的相反幺半群），其中合成为映射。如果M的作用相应的到作用的律用左（或右）乘法表示，那么这个作用是左（或右）运算的事实可以用公式来表示

(1)
$$
e.x = x; \quad \alpha.(\beta.x) = (\alpha \beta).x \quad \text{for } \alpha, \beta \in M \text{ and } x \in E.
$$
（分别$x.e = x; \quad (x.\alpha).\beta = x.(\alpha \beta) \quad \text{for } \alpha, \beta \in M \text{ and } x \in E$）。

在这些条件下，还可以说M对E的左侧（或右侧）进行操作，并且作用的相应的律是E上幺半群M的左侧（或右侧）运算的律。

设 M 为幺半群； 集合 E 以及 E 上 M 的左（或右）运算称为左（或右）M 集。如果 M 到 $E^E$ 的映射 $\alpha \mapsto f_\alpha$ 是单射的，那么幺半群 M 就可以忠实地在左（或右）操作。

#### 例 {#alg-i-s5-n1-exa-1 .statement tag=05B2}

(1) 设E为集合； E (§ 3, no. 1, 例 3) 上$E^E$的规范作用是左运算。

(2) 设M为幺半群。 M 自身的左（或右）作用由 M 上的律（§ 3, no. 3，例 7）导出，是 M 自身的左（或右）运算。当考虑这个运算时，我们说 M 通过左（或右）平移对自身进行操作。

令 E 为左（或右）M 集，$M^0$ 与 M 相反的幺半群。在相同的作用下，幺半群 $M^0$ 作用于右（或左）E。获得的$M^0$集合被称为与M集合E相反。当经过到相反的结构时，定义和与左M集合相关的结果转移到右$M^0$集合。

在本段的其余部分中，我们将考虑，除非，否则，仅留下 M 集，我们将其简称为 M 集。它们的作用的律将由左乘法表示。

令 E 为集合。令G为在E上运行的群。对于G中的所有$\alpha$，由$\alpha$定义的$E^E$的元素是E的置换（$\S$2，no. 3，例2）。因此，在 E 上给予 G 的运算相当于将 G 的同态给予$\mathfrak{S}_E$。

根据$\S$3、no. 3，我们作如下定义：

#### 定义 2 {#alg-i-s5-def-2 .statement tag=05B3}

*设 M 为幺半群，E 和 E' M 集。将 E 的映射 f 转化为 E'，使得对于所有 $x \in E$ 和所有 $\alpha \in M$，$f(\alpha.x) = \alpha.f(x)$ 称为 M 集同态（或 M 态射，或与 M 的运算兼容的映射）。*

M-集合的恒等映射是M-态射。两个 M 态射的合成是一个 M 态射。对于另一个中的一个M-集合的映射为同构，它是双射M-态射并且其逆映射是M-态射是充分必要的。

令 $(E_i)_{i \in I}$ 为 M 集族，令 E 为 $E_i$ 的乘积集合。幺半群 M 通过 $\alpha.(x_i)_{i \in I} = (\alpha.x_i)_{i \in I}$ 对 E 进行操作，并且 E 与作用一起，是一个 M 集；令 E' 为 M 集；当且仅当对于所有 $i \in I$，E' 到 E 的映射 f 是 M 态射，当且仅当 $pr_i \circ f$ 是 E' 到 $E_i$ 的 M 态射。

设 E 为 M 集，F 为 M 的作用下 E 的稳定子集；借助导出的律，F 是 M 集合，典范嵌入 $F \to E$ 是 M 态射。

设 E 为 M 集，E 上的 R 等价关系与 M 的作用兼容；商 $E/R$ 与商作用是 M 集，典范映射 $E \to E/R$ 是 M 态射。

令$\phi : M \to M'$为幺半群同态，E为M集合，E'为$M'$集合。将 E 的映射 f 转化为 E'，使得对于所有 $x \in E$ 和 $\alpha \in M$，

$$
f(\alpha.x) = \phi(\alpha).f(x)
$$

称为 E 到 E' 的 $\phi$ 态射 (cf. $\S$ 3, no. 1)。

* 运算律扩张。* 分别给定（对于例）三个集合 $F_1, F_2, F_3$、置换 $f_1, f_2, f_3$ $F_1, F_2, F_3$ 以及基集合的梯队F $F_1, F_2, F_3$ (*集合理论*, IV, $\S$ 1, no. 1)，我们可以将定义，逐级进行到梯队F的构造，F的置换称为$f_1, f_2, f_3$到F的*规范扩张* (*集合理论*, IV, $\S$ 1, no. 2);我们用$\phi_F(f_1, f_2, f_3)$来表示它。

然后将G的群和$h_i$同态转化为$F_i$（$i = 1, 2, 3$）的对称群，在$F_i$上G的其他字运算。 映射$x \mapsto x_F = \phi_F(h_1(x), h_2(x), h_3(x))$是G的同态到$\mathfrak{S}_F$，在F上G的其他字运算，称为$h_1, h_2, h_3$到F的*扩张*。令P是F的子集，使得对于所有$x \in G$， $x_F(P) = P$；令 $x_P$ 为 $x_F$ 中的限制至

P;则映射$x \mapsto x_P$是G在P上的运算，也称为$h_1, h_2, h_3$对P的扩张。

对于例，令K和L为$F_1, F_2, F_3$上的两个阶梯；取F为$K \times L$的子集集合，P为K的映射集合代入L，用它们的图来识别。如果$w \in P$和$x \in G$，则$x_P(w)$是K到L中的映射$k \mapsto x_L(w(x_K^{-1}(k)))$。

### 2.稳定子，修复者

#### 定义 3 {#alg-i-s5-def-3 .statement tag=05B4}

*设 M 为在集合 E 和 A 以及 B 子集 E 上运行的幺半群。$\alpha \in M$ 的集合，使得 $\alpha A \subset B$（或 $\alpha A = B$）称为 A 到 B 的传输器（或严格传输器）。从 A 到 A 的传输器（或严格传输器）称为A 的稳定子（或严格的稳定子）。$\alpha \in M$的集合，使得所有$a \in A$的$\alpha a = a$被称为A的修复者。*

M 的元素 $\alpha$ 被称为稳定（严格稳定，固定） E 的子集 A 如果 $\alpha$ 属于到 A 的稳定子（严格稳定子，固定）。 M 的子集 P 被称为稳定（分别严格稳定，分别固定）E 的子集 A，如果 P 的所有元素都稳定（分别严格稳定，分别固定）A。A 的固定器包含在 A 的严格稳定子中，而 A 的严格稳定子本身又包含在 A 的稳定子中。

#### 命题 1 {#alg-i-s5-prop-1 .statement tag=05B5}

*设 M 为在 E 的集合 E 和 E 的 A 子集上运行的幺半群。*
(a) *A的稳定子、严格稳定子和固定者是M的子幺半群。*
(b) *令$\alpha$为M的可逆元；如果 $\alpha$ 属于到 A 的严格稳定子（或固定器），$\alpha^{-1}$ 也是如此。*

令 e 为 M 的单位元素；那么 $ea = a$ 对于每个元素 $a \in A$，因此 e 属于到 A 的固定器。令 $\alpha$ 和 $\beta$ 为稳定 A 的 E 的元素。然后 $(\alpha \beta)A = \alpha(\beta A) \subset \alpha A \subset A$ 以及因此 A 的稳定子为M 的子幺半群。类似地，对于 A 的严格稳定子和固定器，从而 (a)。如果$\alpha A = A$，则$A = \alpha^{-1}(\alpha A) = \alpha^{-1}A$。如果对于所有$a \in A$，$\alpha a = a$，则$a = \alpha^{-1}(\alpha a) = \alpha^{-1}a$，从而 (b)。

#### 推论 {#alg-i-s5-n2-cor-1 .statement tag=05B6}

*令G为群在集合E上运行，A为E的子集。A的严格稳定子S和固定器F是G的子群，F是S的正规子群。*

第一个断言源自命题，F是S的同态的核进入与A上S的运算相关的$\mathfrak{S}_A$。

群 G 忠实地在集合 E 上运行当且仅当 E 的固定器由 G 的单位元素组成。E 的固定器是将给定的 G 的同态的核放入$\mathfrak{S}_E$；这个同态是单射的当且仅当它的核由单位元素（§ 4, no. 5，定理3）组成。

设 M 为幺半群，E 为 M 集，E 的 $a$ 元素。固定器、$\{a\}$ 的严格稳定子和稳定子相等；这个幺半群同样被称为 $a$ 的固定者或稳定子。 E 的子集 A 的固定器是 A 的元素的固定器的交。如果 $a$ 的固定器是幺半群 M，则$a$ 称为 E 的不变量元素。如果 E 的每元素，则称 M 对 E 进行平凡操作是不变的。

#### 命题 2 {#alg-i-s5-prop-2 .statement tag=05B7}

*令 G 为群在集合 E 上运行，并且对于所有 $x \in E$，令 $S_x$ 为 x 的稳定子。对于所有 $\alpha \in G$、$S_{\alpha x} = \alpha S_x \alpha^{-1}$。*

如果$s \in S_x$，则$\alpha s \alpha^{-1}(\alpha x) = \alpha s x = \alpha x$，从而$\alpha S_x \alpha^{-1} \subset S_{\alpha x}$。如 $x = \alpha^{-1}(\alpha x)$、$\alpha^{-1} S_{\alpha x} \alpha \subset S_x$、从而 $S_{\alpha x} \subset \alpha S_x \alpha^{-1}$。

类似地，如果A和B是E的两个子集，并且T是A到B的传输子（或严格传输子），则$\alpha A$到$\alpha B$的传输子（或严格传输子）等于$\alpha T \alpha^{-1}$。

### 3.内自同构

令 G 为群。 群G自同构集合Aut(G)是$\mathscr{G}_G$(§ 4, no. 1，例2)子群。

#### 命题 3 {#alg-i-s5-prop-3 .statement tag=05B8}

*设G为群。对于 G 的每个元素 x，映射 Int(x): $y \mapsto xyx^{-1}$ G 到其本身就是 G 的自同构。 映射 Int: $x \mapsto \operatorname{Int}(x)$ 到 Aut(G) 是群同态，其核是G 的中心且其像是 Aut(G) 的正常子群。*

如果$x, y$和$z$是G的元素，则$(xyx^{-1})(xz x^{-1}) = xyz x^{-1}$，因此Int(x)是G的自同态。对于G的$x$和$y$元素，

$$
\operatorname{Int}(x) \circ \operatorname{Int}(y) = \operatorname{Int}(xy):
$$

对于所有$z \in G$，$x(yzy^{-1})x^{-1} = (xy)z(xy)^{-1}$。另一方面，$\operatorname{Int}(e)$是G的恒等映射。映射Int因此是从G到群G的自同态的幺半群End(G)的幺半群同态。由于G的元素是可逆的，映射Int取其End(G)(§ 2, no. 3)的可逆元的集合Aut(G)中的值。现在$xyx^{-1} = y$当且仅当$x$和$y$通勤，因此$\operatorname{Int}(x)$是G的恒等映射当且仅当$x$是中心元素。最后，令$\alpha$为G的自同构，并令$x \in G$；然后

$$
\operatorname{Int}(\alpha(x)) = \alpha \circ \operatorname{Int}(x) \circ \alpha^{-1}.
$$

对于$y \in G$，

$$
\alpha(x) \cdot y \cdot \alpha(x)^{-1} = \alpha(x) \cdot \alpha(\alpha^{-1}(y)) \cdot \alpha(x)^{-1} = \alpha(x \cdot \alpha^{-1}(y) \cdot x^{-1}).
$$

因此$\alpha \cdot \operatorname{Int}(G) \cdot \alpha^{-1} \subset \operatorname{Int}(G)$。

#### 定义 4 {#alg-i-s5-def-4 .statement tag=05B9}

*设 G 为群和 $x \in G$。 自同构 $y \mapsto xyx^{-1}$ 称为 x 定义的 G 的内自同构，记为 $\operatorname{Int} x$。*

对于$x, y \in G$，我们也写为$x^y = y^{-1}xy = (\operatorname{Int} y^{-1})(x)$。

G 的子群是正常的当且仅当它在 G 的所有内自同构（§ 4, no. 4，定义 5）下稳定。如果G的子群在G的所有自同构下稳定，则称为特征。群G的中心是特征子群（公式（2））。

群 G 的中心在 G 的所有自同态 (习题 22) 下不一定稳定。特别是，带有运算符的群的中心不一定是稳定的子群。

#### 命题 4 {#alg-i-s5-prop-4 .statement tag=05BA}

设 G 为群，H 为 G 的特征（或正常）子群，K 为 H 的特征子群。则 K 为 G 的特征（或正常）子群。

G 的自同构（或内自同构）的限制到 H 是 H 的自同构，因此 K 不变。

令 G 为群，A $\subset$ G 和 $b \in G$。如果 $bAb^{-1} = A$，则 b 被称为标准化 A；如果对于所有 $a \in A$，$bab^{-1} = a$，则称 b 集中 A。设A和B是G的子集；如果 B 的每个元素都归一化（或集中）A，则称 B 归一化（或集中）A。

$g \in G$的集合对A进行归一化（或中心化），称为A的归一化器（或中心化器）（cf.§ 1, no. 5，定义9）；它通常用 $N_G(A)$ 或简称 $N(A)$（分别为 $C_G(A)$ 或 $C(A)$）表示。它是G的子群。当A是G的子群时，$N_G(A)$可以表征为G的最大的子群，其中包含A且其中A是正规的。

#### 注 {#alg-i-s5-n3-rem-1 .statement tag=05BB}

(1) 当 G 通过内自同构对自身进行操作时，A 的归一化器（或中心化器）是 A 的严格稳定子（或固定器）。特别地，扶正器是正常化器的子群。

(2) 元素 $b \in G$的集合使得$bAb^{-1} \subset A$是G的子幺半群。即使当A是G的子群时，这个集合也不一定是G的子群(习题27)。

### 4.轨道

#### 定义 5 {#alg-i-s5-def-5 .statement tag=05BC}

设 G 为群，E 为 G 集，$x \in G$。如果存在元素$\alpha \in G$使得$y = \alpha x$，则元素$y \in E$是共轭到G的运算下的x。 x的共轭元素的集合在E中称为x的轨道。

关系“y 是共轭到 x”是等价关系。对于$x = ex$；如果$y = \alpha x$，则$x = \alpha^{-1} y$；如果$y = \alpha x$和$z = \beta y$，则$z = \beta \alpha x$。在这个关系下有轨道是等价类。

E 的子集 X 是稳定的当且仅当它相对于共轭关系是饱和的。

G 到 E 的映射 $\alpha \mapsto \alpha x$ 有时称为由 x 定义的轨道映射。它是 G 的 G 态射（通过左翻译将 G 的运算置于自身上）到 E。在此映射下，G 的像 $G . x$ 是 x 的轨道。

如果对于所有$x \in E$，由x定义的轨道映射是单射的，或者如果$G \times E$到$E \times E$的映射$(g, x) \mapsto (gx, x)$是单射的，则称G在E上自由运行。

#### 例 {#alg-i-s5-n4-exa-1 .statement tag=05BD}

(1) 令 G 为群，并通过内自同构考虑 G 的运算本身。 G 中的两个元素，在运算下为共轭，称为内自同构下的共轭，或简称为共轭。 轨道称为共轭类。类似地，如果存在元素 $\alpha \in G$使得$H' = \alpha . H . \alpha^{-1}$，G的两个子集 H和H'被称为共轭，即如果它们在G的运算的扩张到$\mathscr{P}(G)$下是共轭，则通过内自同构。

(2) *在空间$\mathbf{R}^n$中，群$\mathbf{O}(n, \mathbf{R})$正交的作用下点x的轨道是半径为$\|x\|_*$的欧氏球面。

E 的两个共轭元素中的稳定子是 G 的共轭子群 (no. 2, 命题 2)。

共轭关系下E的商集是E的轨道的集合；它是有时，用E/G或G\|E表示。 （有时记号 E/G 保留用于 E 是右 G 集合的情况，记号 G\|E 保留用于 E 是左 G 集合的情况。）

令G为群在右边的集合E上运算。令H为G的正规子群。群G对右边的E/H进行运算，右作用的相应的律为$(xH, g) \mapsto xHg = xgH$；在这个运算下，H的操作很简单，从而是G/H对E/H的权利运算。令$\phi$为E/H到E/G的典范映射； E/G的点的$\phi$下的逆像是E/H中的G（或G/H）的轨道。因此，当经过与 $(E/H)/G = (E/H)/(G/H)$ 在 E/G 上的商双射（称为正则）时，$\phi$ 定义。

令 G（或 H）为群在左侧（或右侧）的集合 E 上运行。假设G和H的作用在E上可通勤，即

$$
(g.x).h = g.(x.h) \quad \text{for } g \in G, x \in E \text{ and } h \in H.
$$

E 上 H 的作用也是 H 的对立群 $H^0$ 的左运算。然后从 § 4, no. 9、命题 12 得出与元素 $(g, h) \in G \times H^0$ 映射关联的映射 E 的 $x \mapsto g . x . h$ 到自身就是 E 上 $G \times H^0$ 的左运算。在这个运算下元素 $x \in E$ 的轨道是集合 $GxH$。其中轨道中的集合用$G\|E/H$表示。另一方面，G（分别为 H）的运算与关于 H（分别为 G）的运算的共轭关系相容，并且轨道 $G\|(E/H)$（分别为 $(G\|E)/H$）的集合与 $G\|E/H$ 相同： 图表

$$
\begin{array}{ccc}
& & E \\
& \swarrow_{\alpha} & \searrow_{\beta} \\
G\|E & & E/H \\
& \downarrow_{\varepsilon} & \\
& & G\|E/H \\
& \searrow_{\delta} & \swarrow_{\gamma}
\end{array}
$$

（其中$\alpha, \beta, \gamma, \delta, \varepsilon$表示取商的典范映射），$\gamma \circ \alpha = \delta \circ \beta = \varepsilon$。

设G为G的群和H子群。通过右平移考虑H在G上的右运算（no. 1，例2）。 轨道 $G/H$ 的集合是左陪集模 H 的集合； 注，G 在 $G/H$ 左边进行律 $(g, xH) \mapsto gxH$ (cf. no. 5) 的操作。类似地，右陪集模H的集合通过左平移是G上H的左运算的轨道的集合$H\backslash G$。如果 K 是 G 包含 H 的子群，且 $\Gamma$ 是模 H 的左（或右）陪集，则 $\Gamma K$（或 $K\Gamma$）是模 K 的左（或右）陪集。 映射 $\Gamma \mapsto \Gamma K$（或 $\Gamma \mapsto K\Gamma$）被称为$G/H$的典范映射到$G/K$（或$H\backslash G$到$K\backslash G$）。它是主观的。

令G为群，H和K为G的两个子群。令H通过左平移对左侧的G进行操作，通过右平移对右侧的K进行操作；这两个运算通勤，这让我们可以考虑集合$H\backslash G/K$。 $H\backslash G/K$的元素称为G模H和K的双陪集。当$K = H$时，我们简单地说双模H的陪集。对于$G/H$到$H\backslash G/H$的典范映射为双射，H是充分必要的是 G 的正规子群。

### 5.同质集合

#### 定义 6 {#alg-i-s5-def-6 .statement tag=05BE}

*设G为群。如果存在元素 $x \in E$，其轨道为 E，则 G 在集合 E 上的运算称为传递性。如果 G 在 E 上的运算是传递性的，则称 G 集合 E 是齐次的。*

也有人说 G 在 E 上*传递操作*；或者说 E 是 *G 下的 *齐次集合。这相当于说 E *非空*，并且对于 E 的所有元素 $x$ 和 $y$，存在元素 $\alpha \in G$ 使得 $\alpha.x = y$。

#### 例 {#alg-i-s5-n5-exa-1 .statement tag=05BF}

如果 E 是 G 集，则 E 的每个轨道以及导出的运算都是 G 下的齐次集合。

令 G 为 G 的群和 H 子群。考虑以 H 为模的左陪集的集合 $G/H$。群 G 在 $(g, xH) \mapsto gxH$ 左侧对 $G/H$ 进行运算。令 N 为 H 的归一化器。群 N 对右侧的 $G/H$ 进行$(xH, n) \mapsto xHn = xnH$ 运算。 H 上的这个运算诱导是平凡的运算，因此，在经过上的商，$N/H$ 对右边的 $G/H$ 进行运算。令 $\phi : (N/H)^0 \to S_{G/H}$ 为同态相应的到此运算。

#### 命题 5 {#alg-i-s5-prop-5 .statement tag=05BG}

*对于上述记号，G/H 是齐次 G 集。 $(N/H)^0$ 的映射 $\phi$ 诱导同构到 G 组 G/H 的自同构群。*

元素$e = H$中$G/H$中的轨道为$G/H$、从而第一个断言。我们现在证明第二个。若$n \in N$定义右译恒等映射于$G/H$，则$e.n = e$，即$H.n = H$、从而$n \in H$。所以

N/H 忠实地在右侧的 G/H 上运行，且 $\phi$ 是单射的。 G 的左运算和 N/H 的右运算在 G/H 上交换，因此 G/H 的 N/H 定义 G 态射算子自身，它们必然是 G 自同构，因为它们是双射的。因此$\phi$在G/H的G自同构的群$\Phi$中取其值。我们证明$\phi$的像是$\Phi$。让$f \in \Phi$。通过传输结构，G 中$f(\dot{e})$ 的稳定子等于$\dot{e}$ 的稳定子，因此等于H。令$n \in G$ 使得$f(\dot{e}) = n\dot{e}$。 G中$n\dot{e}$的稳定子是$nHn^{-1}$（no. 2，命题2），从而$nHn^{-1} = H$和$n \in N$。对于 G/H 的每个元素 $xH$，$f(xH) = f(x.\dot{e}) = x.f(\dot{e}) = xnH = xHn$ 和 $f$ 重合，其中映射由 $n$ 定​​义。

#### 注 {#alg-i-s5-n5-rem-1 .statement tag=05BH}

(1) 令G为G的群、H子群以及G/H上G的$\phi : G \to \mathscr{S}_{G/H}$同态相应的至运算。 $\phi$的核是H的共轭交(no. 2，命题2)。也是H（no. 3）中包含的最大的正常子群。特别是，G 忠实地在 G/H 上运行当且仅当 H 约化到 $\{e\}$ 的共轭中的交。

(2) 令 G 为群，H 和 K 子群，使得 H 是 K 的正规子群。然后 K/H 对右侧的 G 集 G/H 进行运算，将 G/H 的典范映射运算到经过上的 G/K 定义，得到 G 集同构的商$(G/H)/(K/H) \to G/K$（cf.no. 4）。

#### 命题 6 {#alg-i-s5-prop-6 .statement tag=05BI}

*设G为群，E为齐次G集合，a的$a \in E$，H稳定子和H中包含的G的K子群。存在且仅有一个G/K到E的G-态射f使得$f(e.K) = a$。如果 K = H，则 f 为同构。*

如果f是解，则$f(x.K) = x.a$对于G中的所有x，从而唯一性；我们展示存在。由a定义的轨道映射与G上的等价关系$y \in xK$相容的。对于，如果$y = xk, k \in K$，则
$$
y.a = xk.a = x.a.
$$
因此，映射 f 由 G/K 导出为 H，对于 G 中的所有 x 满足 $f(x.K) = x.a$。这个映射是 G 态射并且$f(K) = a$。这个映射是满射的，因为它的像是E的非空稳定子集。现在假设K = H，让我们证明f是单射的。如果$f(x.H) = f(y.H)$，则$x.a = y.a$，从而$x^{-1}y.a = a$和$x^{-1}y \in H$，从而$x.H = y.H$。

#### 定理 1 {#alg-i-s5-thm-1 .statement tag=05BJ}

*设 G 为群。*
(a) *每个齐次 G 集同构于形式 G/H 的齐次 G 集，其中 H 是 G 的子群。*
(b) *设 H 和 H' 是 G 的两个子群。G 集 G/H 和 G/H' 同构当且仅当 H 和 H' 是共轭。*

由于齐次 G 集非空，断言 (a) 由命题 6 得出。我们展示 (b)。设$f : G/H \to G/H'$为G集同构。 子群 H 是 H 的稳定子，因此，通过结构的迁移，稳定子元素 $G/H'$。因此，子群 $H$ 和 $H'$ 为共轭（no. 2，命题 2）。如果$H' = \alpha H \alpha^{-1}$，$H'$是元素$\alpha . H$的稳定子或$G/H$（no. 2，命题2），因此$G/H'$同构于$G/H$ （命题6）。

#### 例 {#alg-i-s5-n5-exa-2 .statement tag=05BK}

(1) 令$E$为非空集。 群 $S_E$ 在 $E$ 上传递操作。如果$x$和$y$是$E$、映射$\tau : E \to E$的两个元素，则$\tau(x) = y$、$\tau(y) = x$和$\tau(z) = z$对于$z \neq x, y$来说，是$E$的置换。让$a \in E$。 $a$的稳定子用$S_F$标识，其中$F = E - \{a\}$。因此齐次$G$集合$E$同构于$S_E / S_F$。

(2) 设$E$为$n$元素和$(p_i)_{i \in I}$的集合，整数$> 0$的有限族，使得$\sum_i p_i = n$。令$X$为集合/划分$(F_i)_{i \in I}$/$E$，使得$\mathrm{Card}(F_i) = p_i$对于所有$i$。 群 $S_E$ 在 $X$ 上传递操作。 稳定子 $H$ 元素 $(F_i)_{i \in I}$ $X$ 与 $\prod_{i \in I} S_{F_i}$ 自然同构，因此是阶 $\prod_{i \in I} p_i!$。 应用定理 1 和§ 4, no. 4，推论命题 4，得到新的证明：

$$
\mathrm{Card}(X) = \frac{n!}{\prod_{i \in I} p_i!}
$$

特别是取$I = \{1, 2, \ldots, r\}$、$E = \{1, 2, \ldots, n\}$、

$$
F_i = \{p_1 + \cdots + p_{i-1} + 1, \ldots, p_1 + \cdots + p_i\}
$$

$1 \leq i \leq r$。令$S$为$\tau \in S_E$的集合，使得$\tau|_{F_i}$对于$1 \leq i \leq r$来说是递增。如果$(G_1, \ldots, G_r) \in X$，则存在且仅有一个$\tau \in S$，其中映射$(F_1, \ldots, F_r)$至$(G_1, \ldots, G_r)$。在其他字中，$S_E$模$H$的每个左陪集在一个且唯一的点中满足$S$。

(3) *设$n$为整数$\geq 1$。正交群 $O(n, \mathbf{R})$ 在 $\mathbf{R}^n$ 中的单位球体 $S_{n-1}$ 上传递运算。 点 $(0, \ldots, 0, 1)$ 的稳定子与正交群 $O(n-1, \mathbf{R})$ 一致。因此齐次 $O(n, \mathbf{R})$-集 $S_{n-1}$ 同构于 $O(n, \mathbf{R})/O(n-1, \mathbf{R})$。*

### 6.同质本金集合

#### 定义 7 {#alg-i-s5-def-7 .statement tag=05BL}

*令$G$为群。如果存在$E$的元素$x$，使得$x$定义的轨道映射为双射，则集合$E$上$G$的运算称为简单传递。 集合 $E$，与$E$上$G$的简单传递左作用一起，称为左齐次主体$G$集合（或$G$下的左齐次主体集合）。*

相当于说，$G$在$E$上自由传递地运行，或者也存在元素$x \in E$，使得$x$定义的轨道映射是$G$集$G$的同构（其中$G$通过左平移操作）到$E$；或者还满足以下两个条件：

(i) $E$ 非空。
(ii) 对于$E$的所有元素$x$和$y$，存在且仅有一个元素$\alpha \in G$使得$\alpha x = y$。

条件 (ii) 也等价于以下条件：

(iii) 映射 $(\alpha, x) \mapsto (\alpha x, x)$ 是$G \times E$ 中的双射到$E \times E$。

我们将定义右齐次主 G 集的任务留给读者。

#### 例 {#alg-i-s5-n6-exa-1 .statement tag=05BM}

(1) 让 G 通过左（或右）平移对自身进行运算。因此，在 G 上定义了左（或右）齐次主 G 集结构，其有时表示为 $G_s$（或 $G_d$）。

(2) 设 E 是*可交换* 群 G 下的齐次集合。如果 G 忠实地在 E 上运行，则后者是齐次主 G 集。

(3) 令E和F是两个同构的集合，其中结构具有相同的类，并令Isom(E, F)是E到F上的同构的集合（给定结构）。 E 的自同构的群 Aut(E)（给定结构）在右侧的 Isom(E, F) 上通过律 $(\sigma, f) \mapsto f \circ \sigma$ 进行运算，并且 Isom(E, F) 是右齐次主 Aut(E) 集。类似地，群 Aut(F) 对左侧的 Isom(E, F) 进行律 $(\sigma, f) \mapsto \sigma \circ f$ 操作，并且 Isom(E, F) 是左齐次主 Aut(F) 集。

(4) *向量空间的加法群下的齐次本金集合称为*仿射空间* (cf. II, § 9, no. 1)。*

同质主 G 集$G_s$ (例 1) 的自同构的群是用$G^0$ (no. 5, 命题 5) 标识的 G 右平移的群。设E是齐次主G集，E的$a$元素。由$a$定义的轨道映射$\omega_a$是G集$G_s$的同构到E上。通过传输结构同构 $\psi_a$ 由 $G^0$ 导出至 Aut(E)。需要注意的是，$\psi_a$*一般取决于a*；更准确地说，对于$\alpha \in G$，

$$
\psi_{\alpha a} = \psi_a \circ \operatorname{Int}_{G^0}(\alpha) = \psi_a \circ \operatorname{Int}(\alpha^{-1}).
$$

例如，在 G 上写 $\delta_a$ 翻译$x \mapsto x \alpha$，

$$
\omega_{\alpha a} = \phi \omega_a \circ \delta_\alpha
$$
和
$$
\psi_a(x) = \omega_a \circ \delta_x \circ \omega_a^{-1}, \quad x \in G,
$$
从而
$$
\psi_{\alpha a}(x) = \omega_a \circ \delta_\alpha \circ \delta_x \circ \delta_\alpha^{-1} \circ \omega_a^{-1} = \omega_a \circ \delta_{\alpha^{-1} x \alpha} \circ \omega_a^{-1} = \psi_a(\alpha^{-1} x \alpha).
$$

### 7. 有限集合的置换群

如果 E 是有限集合且 $n$ 元素，则对称群 $\mathfrak{S}_E$ (§ 4, no. 1) 是阶 $n!$ 的有限群。当E为集合$\mathbf{N}$自然数的区间$\{1, n\}$时，相应的对称群记为$\mathfrak{S}_n$；任何集合与$n$元素的对称群与$\mathfrak{S}_n$同构的。

#### 定义 8 {#alg-i-s5-def-8 .statement tag=05BN}

令 E 为 E 的有限集合、$\zeta \in \mathfrak{S}_E$ 置换以及由 $\zeta$ 生成的 $\mathfrak{S}_E$ 的 $\bar{\zeta}$ 子群。如果在 E 上 $\bar{\zeta}$ 的运算下，存在且仅有一个轨道且不被简化为单个元素，则$\zeta$ 称为循环。这个轨道称为$\zeta$的支撑。

令$\zeta$为一个循环。 $\zeta$的支持度$\operatorname{supp}(\zeta)$是$x \in E$的集合，使得$\zeta(x) \neq x$。

一个周期的阶$\zeta$等于其支持度的基数。由$\zeta$生成的子群$\bar{\zeta}$在$\operatorname{supp}(\zeta)$上传递且忠实地运行。由于$\zeta$是可交换的，$\operatorname{supp}(\zeta)$是$\bar{\zeta}$（no. 6，例2）下的主集合，因此$\operatorname{Card}(\operatorname{supp}(\zeta)) = \operatorname{Card}(\bar{\zeta})$。

#### 引理 1 {#alg-i-s5-lem-1 .statement tag=05BO}

令 $(\zeta_i)_{i \in I}$ 为一个循环族，其支持度为成对不相交的。那么 $\zeta_i$ 是成对可置换的。令$\sigma = \prod_{i \in I} \zeta_i$和$\bar{\sigma}$为由$\sigma$生成的子群。然后$\sigma(x) = \zeta_i(x)$对应$x \in S_i, i \in I$，$\sigma(x) = x$对应$x \notin \bigcup_{i \in I} S_i$。 映射$i \mapsto S_i$是I的双射到$\bar{\sigma}$轨道的集合，而不是单个元素的由……组成。

设$\zeta$和$\zeta'$为两个环，其支持度为不相交的。 如果
$$
x \notin \operatorname{supp}(\zeta) \cup \operatorname{supp}(\zeta'),
$$
然后$\zeta \zeta'(x) = \zeta' \zeta(x) = x$。 如果$x$属于对$\zeta$的支持，则$\zeta'(x) = x$和$\zeta(x)$属于对$\zeta$、从而$\zeta \zeta'(x) = \zeta' \zeta(x) = \zeta(x)$的支持。 同理，当$x$属于得到$\zeta'$的支撑时，则$\zeta' \zeta(x) = \zeta \zeta'(x) = \zeta'(x)$。 因此$\zeta \zeta' = \zeta' \zeta$。 因此，$\zeta_i$是成对可置换的，对于$i \in I$和$x \in S_i$，$\sigma(x) = \zeta_i(x) \in S_i$。 映射$\sigma$和$\zeta_i$重合在$S_i$上，因此$S_i$在$\sigma$和$\mathfrak{S}_{S_i}$的子群下是稳定的，$\sigma$到$S_i$的限制产生的子群传递运行$S_i$；因此$S_i$是一个$\bar{\sigma}$轨道。 由于 $S_i$ 非空且成对不相交的，因此映射 $i \mapsto S_i$ 是单射的。 由于$\bigcup_i S_i$是$x$的集合，使得$\sigma(x) \neq x$，每个$\bar{\sigma}$轨道而不是单个元素的由……组成都是$S_i$之一。

#### 命题 7 {#alg-i-s5-prop-7 .statement tag=05BP}

设 E 是 E 的有限集合和 $\sigma$ 置换。存在且仅有一个由循环满足和以下两个条件组成的有限集合 C：

(a) C 的元素的支持是成对的不相交的；

(b) $\sigma = \prod_{\zeta \in C} \zeta$（C 的元素可通过引理 1 成对置换）。

令$\bar{\sigma}$为$\sigma$生成的子群，并令S为$\bar{\sigma}$轨道的集合，而不是单个元素的由……组成。对于$s \in S$，如果$x \in s$则写$\zeta_s(x) = \sigma(x)$，如果$x \notin s$则写$\zeta_s(x) = x$。对于所有$s \in S$，$\zeta_s$是一个循环，其支持度为$s$和$\sigma = \prod_{s \in S} \zeta_s$，如应用所示，是E的任何元素的两侧。C的唯一性从引理1得出。

#### 定义 9 {#alg-i-s5-def-9 .statement tag=05BQ}

*阶2的循环称为转置。*

令$x$和$y$是E的两个*不同*元素。令$\tau_{x,y}$表示支持$\{x, y\}$的唯一转置。

对于 E 置换 $\sigma \cdot \tau_{x,y} \cdot \sigma^{-1}$ 的每个置换 $\sigma$ 都是一个转置，其支持度为 $\{\sigma(x), \sigma(y)\}$。因此：

(4)
$$
\sigma \cdot \tau_{x,y} \cdot \sigma^{-1} = \tau_{\sigma(x), \sigma(y)}.
$$

因此，形式共轭类换位为群$\mathfrak{S}_E$。

#### 命题 8 {#alg-i-s5-prop-8 .statement tag=05BR}

*设 E 为有限集合。 群 $\mathfrak{S}_E$ 由转置生成。*

对于每个置换$\sigma$，令$F_\sigma$为$x \in E$的集合，使得$\sigma(x) = x$。我们通过在$p$上降序归纳来证明，每个置换$\sigma$使得$\mathrm{Card}(F_\sigma) = p$是乘积转置。如果$p \geq \mathrm{Card}(E)$，置换$\sigma$是E的恒等映射；它是转置空族中的乘积。如果$p < \mathrm{Card}(E)$，假设性质对于每个置换$\sigma'$都被证明，使得$\mathrm{Card}(F_{\sigma'}) > p$。现在$E - F_\sigma \neq \varnothing$；让$x \in E - F_\sigma$和$y \in \sigma(x)$。然后是$y \neq x$和$y \in E - F_\sigma$。让$\sigma' = \tau_{x,y} \cdot \sigma$。 集合$F_{\sigma'}$包含$F_\sigma$和$x$，因此$\mathrm{Card}(F_{\sigma'}) > \mathrm{Card}(F_\sigma) = p$。通过归纳假设$\sigma'$是乘积转置，因此$\sigma = \tau_{x,y} \cdot \sigma'$是乘积转置。

#### 命题 9 {#alg-i-s5-prop-9 .statement tag=05BS}

*令n为整数$\geq 0$。 群 $\mathfrak{S}_n$ 由转置* $(\tau_{i, i+1})_{1 \leq i \leq n-1}$ 生成。

凭借命题 8，足以证明$\tau_{p,q}$、$1 \leq p < q \leq n$、属于到子群 H 由$\tau_{i, i+1}$、$1 \leq i \leq n-1$生成。我们通过$q-p$上的归纳展示这一点。对于$q-p = 1$来说，这是显而易见的。如果 $q-p > 1$，则 (公式 (4)) $\tau_{p,q} = \tau_{q-1,q} \tau_{p,q-1} \tau_{q-1,q}$。 归纳假设$\tau_{p,q-1} \in H$，因此$\tau_{p,q} \in H$。

如果$\sigma \in \mathfrak{S}_n$，$\{1, n\}$的元素的每个有序对$(i, j)$，使得$i < j$和$\sigma(i) > \sigma(j)$被称为$\sigma$的*反转*。让$\nu(\sigma)$表示$\sigma$的反转的数。

令 P 为从$\mathbf{Z}^n$到$\mathbf{Z}$的映射中的加法群。对于 $f \in P$ 和 $\sigma \in \mathfrak{S}_n$，令 $\sigma f$ 为由下式定义的 P 的元素

(5)
$$
\sigma f(z_1, \ldots, z_n) = f(z_{\sigma(1)}, \ldots, z_{\sigma(n)}).
$$

由此定义的P上$\mathfrak{S}_n$的作用为运算；对于所有 $\sigma, \tau \in \mathfrak{S}_n$ 和 $f \in P$、$\sigma f = f$ 和
$$
\begin{align*}
(\tau(\sigma f))(z_1, \ldots, z_n) &= \sigma f(z_{\tau(1)}, \ldots, z_{\tau(n)}) = f(z_{\tau \sigma(1)}, \ldots, z_{\tau \sigma(n)}) \\
&= ((\tau \sigma) f)(z_1, \ldots, z_n).
\end{align*}
$$
公式 (5) 表明$\sigma(-f) = -\sigma f$ 对应$\sigma \in \mathfrak{S}_n$ 和$f \in P$。

设 $p$ 为 P 的元素，定义为

$$
p(z_1, \ldots, z_n) = \prod_{i < j} (z_j - z_i).
$$

#### 引理 2 {#alg-i-s5-lem-2 .statement tag=05BT}

$p \neq 0$ 和 $\sigma p = (-1)^{\nu(\sigma)}$ 对应 $\sigma \in \mathfrak{S}_n$。

$p(1, 2, \ldots, n) = \prod_{i < j} (j - i) \neq 0$，因此$p \neq 0$。另一方面，如果$\sigma \in \mathfrak{S}_n$，那么

$$
\sigma p(z_1, \ldots, z_n) = p(z_{\sigma(1)}, \ldots, z_{\sigma(n)}) = \prod_{i < j} (z_{\sigma(j)} - z_{\sigma(i)}).
$$

令 C 为有序对 $(i, j)$ 的集合，使得 $1 \leq i \leq n,\ 1 \leq j \leq n,\ i < j$。如果 $(i, j)$ 不是反转，置换 $\theta$ 在 C 上由设定 $\theta(i, j) = (\sigma(i), \sigma(j))$ 定义，如果 $(i, j)$ 是反转，则由 $\theta(i, j) = (\sigma(j), \sigma(i))$ 定义。这意味着$\sigma p = (-1)^{\nu(\sigma)} p$。

#### 定理 2 {#alg-i-s5-thm-2 .statement tag=05BU}

*设 E 为有限集合。从 $\mathfrak{S}_n$ 到乘法群 $\{-1, +1\}$，存在且仅有一个同态 $\varepsilon$，使得每一个转置 $\tau$ 都有 $\varepsilon(\tau) = -1$。*

唯一性由命题 8 推出。我们证明存在性。通过传输结构，可以假设$E = \{1, n\}$。使用上面的记号，令$\varepsilon(\sigma) = (-1)^{\nu(\sigma)}$。然后（引理2）

$$
\sigma(\sigma' p) = \sigma(\varepsilon(\sigma') p) = \varepsilon(\sigma') (\sigma p) = \varepsilon(\sigma') \varepsilon(\sigma) p.
$$

另一方面，

$$
\sigma(\sigma' p) = (\sigma \sigma') p = \varepsilon(\sigma \sigma') p.
$$

作为$p \neq -p$，可以得出$\varepsilon(\sigma \sigma') = \varepsilon(\sigma) \varepsilon(\sigma')$，因此$\varepsilon$是同态。我们现在证明，对于每个转置$\tau$，$\varepsilon(\tau) = -1$。 $\nu(\tau_{n-1, n}) = 1$、从而$\varepsilon(\tau_{n-1, n}) = -1$。由于每个转置$\tau$都是共轭到$\tau_{n-1, n}$，并且群$\{-1, +1\}$是可交换的，$\varepsilon(\tau) = \varepsilon(\tau_{n-1, n}) = -1$。

#### 定义 10 {#alg-i-s5-def-10 .statement tag=05BV}

*在定理2的记号中，数$\varepsilon(\sigma)$（也记为$\varepsilon_\sigma$）称为置换$\sigma$的签名。 同态$\varepsilon$的核称为E的交错的群。*

如果$\varepsilon(\sigma) = 1$（或$\varepsilon(\sigma) = -1$），则$\sigma$ 称为*偶*（或*奇*）。 E的交错的群用$\mathfrak{A}_E$表示。这是正常的子群 $\mathfrak{S}_E$。当$E = \{1, n\}$时，简称为$\mathfrak{A}_n$。当E的基数$n$是$\geq 2$时，它是指标2的子群，因此是阶$n! / 2$。可以证明，对于$n = 3$或$n \geq 5$，群$\mathfrak{A}_n$是一个简单的群（*cf.习题16*）。

#### 例 {#alg-i-s5-n7-exa-1 .statement tag=05BW}

若$\sigma$是阶$d$的循环，则
$$
\varepsilon(\sigma) = (-1)^{d-1}.
$$
数置换的反转
$$
(1, 2, 3, \ldots, d) \mapsto (d, 1, 2, \ldots, d-1)
$$
等于$d-1$。

### 习题{#alg-i-s5-exercises}

§ 5](exercises/s5/)参见[习题。
