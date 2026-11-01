---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 6
section_title: Weak topologies
lang: zh
source: evt-i-v
book_pages: TVS II.40-TVS II.53, TVS II.81-TVS II.86
pdf_pages: 0077-0090, 0118-0123
extraction: ocr
subsections:
    - "no": 1
      title: Dual vector spaces
      page: 40
      pdf_page: 77
    - "no": 2
      title: Weak topologies
      page: 42
      pdf_page: 79
    - "no": 3
      title: Polar sets and orthogonal subspaces
      page: 44
      pdf_page: 81
    - "no": 4
      title: Transposition of a continuous linear mapping
      page: 46
      pdf_page: 83
    - "no": 5
      title: Quotient spaces and subspaces of a weak space
      page: 48
      pdf_page: 85
    - "no": 6
      title: Products of weak topologies
      page: 50
      pdf_page: 87
    - "no": 7
      title: Weakly complete spaces
      page: 51
      pdf_page: 88
    - "no": 8
      title: Complete convex cones in weak spaces
      page: 52
      pdf_page: 89
statements: 41
exercises: 20
content_sha256: 70b152ad63ceca6fd0b7d027e0efe9f024cc299deca5d372a0d6469d0d61312e
translated_from: content/en/evt/II/06_s6_weak_topologies.md
translation_method: google
source_content_sha256: 99514709d3c5833b248b220057a632a5ff5dc72f7ecf8af9bb7a09eddc3274a1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: e01badec337f4d8bc9d6446b7d6ee20bc123fcb8eb108d43601c119e9cf394f1
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 6。弱拓扑

### 1.双向量空间

令$F$和$G$为两个实数向量空间，并令$(x, y) \mapsto B(x, y)$为$F \times G$上的*双线性*形式。我们说双线性形式$B$*将向量空间*$F$*和*$G$*置于对偶性*，或者说F和G处于对偶性（相对于B）。回想一下，如果 $B(x, y) = 0$，我们说 $x \in F$ 和 $y \in G$ 是正交的（对于 B 定义的对偶性）；如果每个$x \in M$都与每个$y \in N$正交（A，IX, § 1.2），我们就说F的子集M和G的子集N是正交的。

如果 B 定义的对偶性满足以下条件 ，我们就说 B 定义的对偶性在 F 中（或在 G 中）是分离的：

(D_I) *对于 F 中的每个 $x \neq 0$，都存在 $y \in G$ 使得 $B(x, y) \neq 0$.* （分别为

(D_{II}) *对于 G 中的每个 $y \neq 0$，存在 $x \in F$ 使得 $B(x, y) \neq 0$。）

如果 B 定义的对偶性在 F 和 G 中都分离，则称其为分离的。为此，双线性形式 B 在 A、IX, § 1.1 的意义上分离是充分必要的。更准确地说，我们得到以下结果：

#### 命题 1 {#evt-ii-s6-prop-1 .statement tag=07H0}

*设F、G为$F \times G$上的两个实数向量空间和B双线性形式。让*

$$
d_B : y \mapsto B(., y),
$$
$$
s_B : x \mapsto B(x, .)
$$

*是F的对偶$F^*$中的G的线性映射和G的对偶$G^*$中的F，分别关联到B*的右侧和左侧（A，IX, § 1.1）。然后 B 将 F 和 G 置于 G 中（或 F 中）分离的对偶性中，当且仅当 $d_B$（或 $s_B$）是单射的。*

当F和G被B置于分离对偶性时，我们经常通过$s_B$（或$d_B$）将认同F（或G）与$G^*$（或$F^*$）的子空间。当我们将 F（或 G）视为 $G^*$（或 $F^*$）的子空间而不指定如何进行这种识别时，我们总是使用前面的识别；然后，双线性形式 B 被标识为规范双线性形式的限制到 $F \times G$：

$$
(x^*, x) \mapsto \langle x, x^* \rangle \quad (\text{resp. } (x, x^*) \mapsto \langle x, x^* \rangle).
$$

#### 例 {#evt-ii-s6-n1-exa-1 .statement tag=07H1}

— 1) 令 E 为向量空间，并令 E* 为其对偶。 $E \times E^*$ (A, II, § 2.3) 上的规范双线性形式 $(x, x^*) \mapsto \langle x, x^* \rangle$ 将 E 和 E* 置于分离对偶性中：因为 (D_{II}) 为真，因为关系 $x^* \neq 0$ 的定义，另一方面我们知道，对于E中所有$x \neq 0$，存在线性形式$x^* \in E^*$使得$\langle x, x^* \rangle \neq 0$(A, II, § 7.5, th.6)，证明(D_I)； E 与子空间的$E^{**}$ 的识别是通过典范映射 $c_E$ 进行的（*loc.cit.*）。

当 E 为 *有限* 维数时，E* 中唯一的子空间 G 处于正则双线性形式的限制到 $E \times G$ 分离对偶性，是空间 E* 本身；因为，E 被规范地标识为 $E^{**}$ (*loc.cit.*)，如果我们有 $G \neq E^*$，那么 E 中就会存在 $a \neq 0$，这样 $\langle a, x^* \rangle = 0$ 对于所有 $x^* \in G$ (A, II, § 7.5, th. 7)，其中与……矛盾假设。

2) 当E是*无限*维向量空间，并且E'是E*的向量子空间时，由规范双线性形式的限制到$E \times E'$定义的E和E'之间的对偶性总是在E'中分离；即使$E' \neq E^*$，它也可以在E中分离。最重要的情况发生在 E 是拓扑向量空间的情况下。

#### 定义 1 {#evt-ii-s6-def-1 .statement tag=07H2}

— *所谓拓扑向量空间 E 的对偶，我们指的是 E* 的子空间 E'，向量空间 E 的对偶，由 E 上的连续线性形式形成。*

当 E 是 *Hausdorff 局部凸* 空间时，E 与其对偶 E' 之间的对偶性是分离的：这根据 Hahn-Banach 定理（II，p. 24，cor. 1）得出，对于 E 中的每个$x \neq 0$，都存在$x' \in E'$，使得$\langle x, x' \rangle \neq 0$。

#### 注 {#evt-ii-s6-n1-rem-1 .statement tag=07H3}

— 1) 当E是*拓扑*向量空间时，*向量空间*E的对偶$E^*$将被称为E的*代数对偶*以避免混淆。我们注还知道$E^*$是拓扑向量空间的对偶，通过给E提供*最佳*局部凸拓扑（II，p. 25，*例*2）。
2) 拓扑向量空间的对偶E'本身不携带拓扑，除非，这是明确说明的。
3) 如果 F 和 $G \subset F^*$ 通过规范双线性形式分离对偶性，那么 F 和 $G_1$ 也是如此，对于 $F^*$ 的每个子空间 $G_1$ 使得 $G \subset G_1$。

### 2. 弱拓扑

#### 定义 2 {#evt-ii-s6-def-2 .statement tag=07H4}

— *设 F 和 G 是通过双线性形式 B 进行对偶的两个向量空间。F 上使所有线性形式 $B(., y): x \mapsto B(x, y)$ 连续的最粗糙拓扑，其中 y 在 G 中变化，称为 F 上的弱拓扑，由 F 和 G 之间的对偶性定义，我们将其表示为$\sigma(F, G)$.*

同样，我们在定义 1 中的 G、交换 F 和 G 上定义弱拓扑 $\sigma(G, F)$； 交换 F 和 G 的这种可能性适用于本段后面的所有结果和定义。

我们使用形容词“weak”和副词“weakly”来表示与弱拓扑$\sigma(F, G)$相关的属性，前提是不存在混淆的可能性。对于例，我们将谈论“弱收敛”和“弱连续函数”等。

当$G \subset F^*$时，记号$\sigma(F, G)$将始终表示由规范双线性形式$(x, x^*) \mapsto \langle x, x^* \rangle$的对偶性相应的到限制到$F \times G$定义的弱拓扑。

在没有对 F 和 G 进行额外假设的情况下，我们经常将双线性形式 B 的值 $B(x, y)$ 写成 $\langle x, y \rangle$ 在 $(x, y)$ 处，前提是没有歧义；我们将在本段的其余部分通过这项公约。

向量空间 F 携带弱拓扑 $\sigma(F, G)$ 将被称为*弱空间*。

弱拓扑 $\sigma(F, G)$ 是*局部凸*（II，p. 26，道具 4）；更准确地说，是$\mathbf{R}^G$中F的线性映射$\phi : x \mapsto (\langle x, y \rangle)_{y \in G}$乘以$\mathbf{R}^G$的*乘积*拓扑的逆像。当 y 在 G 中变化时（II，p. 5），它由 *半范数* $x \mapsto |\langle x, y \rangle|$ 的集合定义。对于每个$\alpha > 0$，以及G的点的每个有限族$(y_i)_{1 \leq i \leq n}$，令$W(y_1, ..., y_n; \alpha)$为$x \in F$的集合，使得$|\langle x, y_i \rangle| \leq \alpha$对应于$1 \leq i \leq n$；这些集合（对于$\alpha, n$和$y_i$任意）形式*0的邻域的*基本系统对于$\sigma(F, G)$。 注 $W(y_1, ..., y_n; \alpha)$ 包含 F 的 *向量子空间*，属于*有限*余维，由 $1 \leq i \leq n$ 的方程 $\langle x, y_i \rangle = 0$ 定义。

#### 命题 2 {#evt-ii-s6-prop-2 .statement tag=07H5}

— *弱拓扑* $\sigma(F, G)$ *是 Hausdorff 当且仅当* $F$ *和* $G$ *之间的对偶性在* $F$ 中分离。

这是 II、p. 3 属性的特例。 2.

#### 命题 3 {#evt-ii-s6-prop-3 .statement tag=07H6}

— *设* $F$ *和* $G$ *是对偶中的两个实数向量空间。每个线性形式在*$F$上，*对于*$\sigma(F, G)$是连续的，*可以写成*$x \mapsto \langle x, y \rangle$*对于某些*$y \in G$。 *元素* $y \in G$ *当对偶性在* $G$ 中分离时是唯一的。

因为，说$F$上的线性形式$f$对于$\sigma(F, G)$是连续的，意味着存在点$y_i \in G$（$1 \leq i \leq n$）的有限集合，这样，对于$F$中的所有$x$， $|f(x)| \leq \sup_{1 \leq i \leq n} |\langle x, y_i \rangle|$（II，p. 6，道具 5）。因此，$n$关系$\langle x, y_i \rangle = 0$（$1 \leq i \leq n$）意味着$f(x) = 0$，因此（A，II, § 7.5，cor.1），存在线性组合$y = \sum_{i=1}^n \lambda_i y_i$，使得$f(x) = \langle x, y \rangle$对于所有$x \in F$。 唯一性由 (D$_\text{II}$) 得出。

在其他字中，当对偶性在$G$中分离时，$F$有拓扑$\sigma(F, G)$，那么我们可以确定$G$规范地与$F$的对偶对于这个拓扑（II， p. 42，定义 1)。

#### 推论 1 {#evt-ii-s6-prop-3-cor-1 .statement tag=07H7}

— *家庭* $(a_i)$ *的点的* $F$ *总计为拓扑* $\sigma(F, G)$ *当且仅当，对于每个* $y \neq 0$ *在* $G$，*存在指标* $i$ *这样* $\langle a_i, y \rangle \neq 0$。

用于使用道具。 3 和 I、p. 13、th。 1、性质表示对于$\sigma(F, G)$没有封闭的超平面包含所有$a_i$；因此，推论是从 cor 得出的。 3 个II、p. 38。

#### 推论 2 {#evt-ii-s6-prop-3-cor-2 .statement tag=07H8}

— *族* $(a_i)$ *的点的* $F$ *对于拓扑* $\sigma(F, G)$，*当且仅当，对于每个指标* $i$，*存在元素* $b_i \in G$ *这样* ：$\langle a_i, b_i \rangle \neq 0$ *和* $\langle a_\kappa, b_i \rangle = 0$ *所有* $\kappa \neq i$。

这意味着，对于所有 $i$，$\sigma(F, G)$ 中存在一个封闭的超平面，其中包含所有 $a_\kappa$ 与指标 $\kappa \neq i$，但不存在包含 $a_i$。

#### 推论 3 {#evt-ii-s6-prop-3-cor-3 .statement tag=07H9}

— *让* $G_1$ *和* $G_2$ *成为* $F^*$的两个向量子空间，*与* $F$ *（对于规范双线性形式的限制）*。 *那么*$\sigma(F, G_2)$*更细比*$\sigma(F, G_1)$*当且仅当*$G_1 \subset G_2$。

条件显然就足够了；相反，如果$\sigma(F, G_2)$比更细大于$\sigma(F, G_1)$，则对于$\sigma(F, G_1)$连续的每个线性形式对于$\sigma(F, G_2)$也是连续的，因此通过道具$G_1 \subset G_2$。 3.

#### 推论 4 {#evt-ii-s6-prop-3-cor-4 .statement tag=07HA}

— *令* $G$ *为对偶* $F^*$ 的向量子空间，*向量空间* $F$。 *然后* $F$ *和* $G$ *处于分离对偶性*（对于规范双线性形式）*当且仅当* $G$ *密集于* $F^*$ *于拓扑* $\sigma(F^*, F)$。

这是从 cor 得出的。 1.

### 3. 极坐标集合和正交子空间

#### 定义 2 {#evt-ii-s6-def-2-bis .statement tag=07HB}

设 F 和 G 为对偶性中的两个（实数）向量空间。对于 F 的每个集合 M，我们将其称为 M 的极坐标，y ∈ G 的集合，其中 $\langle x, y \rangle \geq -1$ 对于所有 $x \in M$。 （对于复杂的向量空间、cf.、II、p. 64。）

如果$G_1, G_2$是$F^*$的两个子空间，使得$G_1 \subset G_2$，则$G_1$中M的极坐标是$G_1$中的交，而M在$G_2$中的极坐标。

在不存在混淆的情况下，我们使用 $M^\circ$ 来表示 G 中 F 的子集 M 的极坐标。同样，我们也用定义 F 中 G 的集合的极坐标。

显然，对于每个标量 $\lambda \neq 0$ 和所有 $M \subset F$，我们都有 $(\lambda M)^\circ = \lambda^{-1} M^\circ$。 关系$M \subset N \subset F$意味着$N^\circ \subset M^\circ$；如果 N 吸收 M，则 $M^\circ$ 吸收 $N^\circ$；对于F的集合的每个家庭$(M_\alpha)$，$\bigcup \alpha M_\alpha$的极地集合是极地集合$M_\alpha^\circ$的交。因为，对于 $y \in M^\circ$，由关系 $\langle x, y \rangle \geq -1$ 包含 0 和 M 定义的闭半空间，我们看到如果 $M_1$ 是 $M \cup \{0\}$ 的凸包络，则$M_1^\circ = M^\circ$。

显然$M \subset M^{\circ \circ}$。因此
$$
(M^{\circ \circ})^\circ \subset M^\circ \subset (M^\circ)^{\circ \circ} = (M^{\circ \circ})^\circ
$$
即 $M^{\circ \circ \circ} = M^\circ$（cf. S，III, § 1.5，道具 2）。

如果M是F的对称子集，则$M^\circ$是G的对称子集；在这种情况下，$M^\circ$也是$y \in G$的集合，使得$|\langle x, y \rangle| \leq 1$对于所有$x \in M$。

#### 命题 4 {#evt-ii-s6-prop-4 .statement tag=07HC}

(i) 对于 F 的任何集合 M，极集合 $M^\circ$ 是包含 0 的凸集合，并且在 G 中对于拓扑 $\sigma(G, F)$ 是封闭的。

(ii) 如果 M 是顶点 0 的圆锥体，则 $M^\circ$ 是顶点 0 的圆锥体，并且它也是 $y \in G$ 的集合，使得 $\langle x, y \rangle \geq 0$ 对于所有 $x \in M$。

(iii) 如果 M 是 F 的向量子空间，则 $M^\circ$ 是 G 的向量子空间，并且它也是 $y \in G$ 的集合，使得对于所有 $x \in M$ 来说$\langle x, y \rangle = 0$。

(i) 由于线性形式 $y \mapsto \langle x, y \rangle$ 对于 $\sigma(G, F)$ 叙述是连续的，因此直接从定义得出，并且由超平面确定的半空间是凸的。

(ii) 如果 M 是顶点为 0 的圆锥体，并且如果 $x \in M, y \in M^\circ$，则作为 $\lambda x \in M$，对于所有 $\lambda > 0$，我们有 $\langle \lambda x, y \rangle \geq -1$，即 $\lambda \langle x, y \rangle \geq -1$。由于这对于所有 $\lambda > 0$ 都成立，因此$\langle x, y \rangle \geq 0$ 和 (ii) 被证明。

(iii) 类似地，如果 M 是 F 的向量子空间，关系 $x \in M, y \in M^\circ$ 意味着，这一次，对于所有实数$\lambda$，$\lambda \langle x, y \rangle \geq -1$ 只有在 $\langle x, y \rangle = 0$ 时才有可能。

如果M是F的向量子空间，我们说$M^\circ$是M在G中的正交；如果$G \subset F^*$，则$M^\circ$是G的交，并且是F的代数对偶$F^*$中与M正交的子空间（A，II, § 2.4，def.4）。

对于 F 的向量子空间 M 和 G 的向量子空间 N，如果 $M \subset N^o$（或者等效地，如果 $N \subset M^\circ$），我们说 M 和 N 正交。

#### 定理 1（双相定理）{#evt-ii-s6-thm-1 .statement tag=07HD}

设F，G为对偶性中的两个实数向量空间。对于 F 的每个子集 M，G 中 M 的极坐标集合 $M^\circ$ 的 F 中的极坐标集合 $M^{\circ \circ}$ 是 $M \cup \{0\}$ 的封闭凸包络（对于 $\sigma(F, G)$）。

我们已经看到，我们只需要考虑$M$是凸的并且$0 \in M$的情况。用$\overline{M}$表示$M$的拓扑$\sigma(F, G)$中的闭包，则$\overline{M}$是$F$中的凸集合；支柱。 II、p. 44中的4个表明$M^{\circ\circ} \supseteq \overline{M}$。另一方面，如果$a \in F$不属于到$\overline{M}$，那么$F$中存在一个封闭的超平面$H$，它严格地将$a$与$\overline{M}$分开（II，p. 38，道具4）；由于 $H$ 不等于包含 0，因此存在 $y \in G$，使得 $H$ 具有方程 $\langle x, y \rangle = -1$（II，p. 43，命题 3）；因此 $\langle x, y \rangle > -1$ 对于所有 $x \in \overline{M}$ 和 $\langle a, y \rangle < -1$。这意味着$y \in M^\circ$和$a \notin M^{\circ\circ}$，以及关系$M^{\circ\circ} = \overline{M}$。

#### 推论 1 {#evt-ii-s6-thm-1-cor-1 .statement tag=07HE}

*对于任何族* $(M_\alpha)$ *的闭凸集合的* $F$ *（在拓扑* $\sigma(F, G)$*），每个包含* 0，*交* $M = \bigcap \limits_{\alpha} M_\alpha$ *的极坐标集合是凸闭包络* （*对于* $\sigma(G, F)$）* 并的* $M_\alpha^\circ$。

因为，如果 $N$ 是这个凸封闭包络线，那么

$$
N^\circ = \bigcap \limits_{\alpha} M_\alpha^{\circ\circ} = \bigcap \limits_{\alpha} M_\alpha = M
$$

从而$N = N^{\circ\circ} = M^\circ$。

Cor的结论。如果 $M_\alpha$ 不是凸的，则 1 不一定成立。

#### 推论 2 {#evt-ii-s6-thm-1-cor-2 .statement tag=07HF}

*对于* $F$的每个向量子空间* $M$ *，*子空间* $M^{\circ\circ}$ *是拓扑* $\sigma(F, G)$中* $M$ *的闭包。

#### 注 {#evt-ii-s6-n3-rem-1 .statement tag=07HG}

— 拓扑 $\sigma(G, F)$ 包含邻域 $V$ 中$G$中的每个邻域由形式$|\langle x_i, y \rangle| \leq 1$ ($1 \leq i \leq n$) 的有限不等式数定义，其中$x_i$是$F$中的任意点。如果$A$是$x_i$的集合的*对称凸包络*，那么$V$就是$G$中$A$的*极集合* $A^\circ$。我们可以说，$F$（或其凸包络）中的有限对称集合（或其凸包络）形式中的*$G$*极坐标是$G$中0的邻域基本系统对于$\sigma(G, F)$。如果对偶性在 $F$ 中分离，则这些凸包络对于 $\sigma(F, G)$（II、p. 14，第 15 条命题的第 1 条）和有限维来说是“紧凑”的。相反，$F$中的有限维* $C$的*紧凑凸集合（以及$\sigma(F, G)$拓扑）包含在$F$的*有限子集*的凸包络中。例如，令$M$为有限维包含$C$中的向量子空间。如果$(e_i)_{1 \leq i \leq n}$是$M$的基，我们可以假设$C$包含在闭平行六边形中心0中，并构造在基$e_i$的向量上（GT，VI, § 1.3）；现在这个平行四边形是直接的点 $\sum \limits_{i=1}^n \varepsilon_i e_i$ 和 $\varepsilon_i = \pm 1$ 的凸包络线。

因此我们可以说（如果 $\sigma(F, G)$ 是 Hausdorff）* 有限维极坐标，凸，紧集 in* $F$（对于 $\sigma(F, G)$ 或对于任何 Hausdorff 局部凸拓扑更细比 $F$ 上的 $\sigma(F, G)$）对于 $\sigma(G, F)$，形式邻域的基本系统为 0。

#### 推论 3 {#evt-ii-s6-thm-1-cor-3 .statement tag=07HH}

*设* $\mathscr{T}$ *为局部凸空间* $E$ *的拓扑，并让* $E'$ *为其对偶*（II，p. 42，默认为1）。

(i) *E 中的闭凸集合对于拓扑 $\mathscr{T}$ 和弱拓扑 $\sigma(E, E')$ 是相同的。

(ii) *对于E的每个子集M，$E'$中M的极集合$M^\circ$的E中的极集合$M^{\circ\circ}$，是拓扑$\mathscr{T}$的$M \cup \{0\}$的凸闭包络。

显然，(ii) 由 (i) 和 th 推出。 1. 从对偶 $E'$ 的定义出发，由 II、p. 43 推出。 3 E 上拓扑 $\mathscr{T}$ 的连续线性形式与$\sigma(E, E')$ 的连续线性形式相同。因此，E 中的闭半空间对于 $\mathscr{T}$ 和 $\sigma(E, E')$ 是相同的（II，p. 15，命题 17），并且断言 (i) 因此可以从 II，p. 38，cor. 得出。 1.

### 4.连续线性映射的转置

在这个数中，我们假设(F,G)和$(F_1, G_1)$是对偶的两个向量空间。

#### 命题 5 {#evt-ii-s6-prop-5 .statement tag=07HI}

*令u为$F_1$中F的线性映射。以下属性是等效的：*

a) *u 对于弱拓扑 $\sigma(F, G)$ 和 $\sigma(F_1, G_1)$ 是连续的；*

b) *there exists 映射 $v : G_1 \to G$ such that*

$$
\langle u(y), z_1 \rangle = \langle y, v(z_1) \rangle
$$

对于所有 $y \in F$ 和 $z \in G_1$。

*如果这些性质成立并且 F 和 G 之间的对偶性在 G 中分离，则映射 v 满足 (1) 是唯一的，并且 v 是线性的。*

如果u对于弱拓扑是连续的，那么，对于所有$z_1 \in G_1$，F上的线性形式$y \mapsto \langle u(y), z_1 \rangle$对于$\sigma(F, G)$来说是连续的，因此（II，p. 43，命题3）可以写成$y \mapsto \langle y, v(z_1) \rangle$和$v(z_1) \in G$，这表明a）蕴涵b）。相反，如果 b) 为真，则对于所有 $z_1 \in G_1$、线性形式

$$
y \mapsto \langle y, v(z_1) \rangle = \langle u(y), z_1 \rangle
$$

对于$\sigma(F, G)$是连续的：从弱拓扑的定义可以得出，u对于$\sigma(F, G)$和$\sigma(F_1, G_1)$是连续的（I，p. 10，cor.1）。 v 的唯一性由 (D_{II}) 得出，这个唯一性意味着 v 是线性的。

#### 注 {#evt-ii-s6-n4-rem-1 .statement tag=07HJ}

— 假设 F 和 G 之间的对偶性在 G 中分离，并且 $F_1$ 和 $G_1$ 之间的对偶性在 $G_1$ 中分离。如果我们认同 G 和$G_1$ 以及子空间分别为$F^*$ 和$F_1^*$，则条件 a) 和b) 等价于$^t u(G_1) \subset G$； v 是 u (A, II, § 2.5) 的转置 $^t u$ 到 $G_1$ 的限制。

我们简单地说（当不存在混淆的情况下）v 是 u 的 *转置*（一方面相对于 F 和 G 之间的对偶性，另一方面相对于 $F_1$ 和 $G_1$ 之间的对偶性），并且我们再次使用 $^t u$ 来表示它。

#### 推论{#evt-ii-s6-n4-cor-1 .statement tag=07HK}

*假设F和G之间的对偶性在G中分离。如果u是$F_1$中F的线性映射，即对于$\sigma(F, G)$和$\sigma(F_1, G_1)$连续，则其*转置是$G$中$G_1$的线性映射，对于$\sigma(G_1, F_1)$连续， $\sigma(G, F)$。此外，如果$F_1$和$G_1$之间的对偶性在$F_1$中分离，则${}^t({}^t u) = u$。

将 $F$ 和 $F_1$ 与 prop 中的 $G$ 和 $G_1$ 交换就足够了。 5.

#### 命题 6 {#evt-ii-s6-prop-6 .statement tag=07HL}

*假设$F$和$G$（分别是$F_1$和$G_1$）之间的对偶性在$G$（分别是$F_1$）中分离。令$u$为$F_1$中$F$的线性映射，对于$\sigma(F, G)$和$\sigma(F_1, G_1)$连续。令$F$中的$A$为集合，$F_1$中的$A_1$集合；然后*：

(i) *我们有$(u(A))^{\circ} = {}^t u^{-1}(A^{\circ})$。*

(ii) *我们有 ${}^t u(A_1^{\circ}) \subset (u^{-1}(A_1))^{\circ}$；此外，如果 $A$ 是闭集，（对于 $\sigma(F_1, G_1)$）凸，并且包含原点，那么我们有 ${}^t u(A_1^{\circ}) = (u^{-1}(A_1))^{\circ}$。*

令$z_1 \in G_1$、关系$z_1 \in (u(A))^{\circ}$等价于所有$y \in A$的$\langle u(y), z_1 \rangle \geq -1$，关系${}^t u(z_1) \in A^{\circ}$等价于所有$y \in A$的$\langle y, {}^t u(z_1) \rangle \geq -1$，并且我们的断言(i)遵循使用(1)。接下来交换$u$和${}^t u$和应用（i）到$G_1$的集合$A_1^{\circ}$我们得到

$$
({}^t u(A_1^{\circ}))^{\circ} = u^{-1}(A_1^{\circ \circ}) \supset u^{-1}(A_1)
$$

从那里，在采取极地

$$
({}^t u(A_1^{\circ}))^{\circ \circ} \subset (u^{-1}(A_1))^{\circ} .
$$

我们有 ${}^t u(A_1^{\circ}) \subset ({}^t u(A_1^{\circ}))^{\circ \circ}$ 和双极定理（II，p. 44，第 1）；最终的叙述由 (2) 得出，自此之后的双极定理 $A_1^{\circ \circ} = A_1$ 和 ${}^t u(A_1^{\circ})$ 是凸的，包含是原点。

#### 推出 1 {#evt-ii-s6-prop-6-cor-1 .statement tag=07HM}

*带有记号的支柱。 6、关系$u(A) \subset A_1$暗示${}^t u(A_1^{\circ}) \subset A^{\circ}$；如果进一步 $A_1$ 是凸的、闭合的（对于 $\sigma(F_1, G_1)$）和包含原点，那么这两个关系是等价的。*

事实上，关系$u(A) \subset A_1$等价于$A \subset u^{-1}(A_1)$，因此意味着

$$
{}^t u(A_1^{\circ}) \subset {}^t u(A_1^{\circ}) \subset (u^{-1}(A_1))^{\circ} \subset A^{\circ}
$$

相反关系 ${}^t u(A_1^{\circ}) \subset A^{\circ}$ 意味着

$$
A^{\circ \circ} \subset ({}^t u(A_1^{\circ}))^{\circ} = u^{-1}(A_1^{\circ \circ})
$$

来自（2）。当$A_1 = A_1^{\circ \circ}$时，我们推导出$A \subset u^{-1}(A_1)$。

#### 推出 2 {#evt-ii-s6-prop-6-cor-2 .statement tag=07HN}

*令$u$为$F_1$中$F$的线性映射，对于$\sigma(F, G)$和$\sigma(F_1, G_1)$连续。那么我们有*

(3)

$$
\operatorname{Ker}({}^t u) = (\operatorname{Im}(u))^{\circ} ,
$$

(4)

$$
\overline{\operatorname{Im}({}^t u)} = (\operatorname{Ker}(u))^{\circ} .
$$

*假设$F$和$G$之间以及$F_1$和$G_1$之间的对偶性是分离的；那么 $u(F)$ 在 $F_1$ 中是稠密的（对于 $\sigma(F_1, G_1)$），当且仅当 ${}^t u$ 是单射的。*

应用道具。 6 与 $A = F$ 和 $A_1 = \{0\}$，利用弱拓扑 $\sigma(G, F)$ 和 $\sigma(F_1, G_1)$ 是 Hausdorff 的事实。 最后一个断言由 (4)、交换 $u$ 和 $^t u$ 得出。

### 5.弱空间的商空间和子空间

设$F, G$是对偶性中的两个实数向量空间。令$M$为$F$的向量子空间，并考虑$G$中正交$M^\circ$的子空间$N$；如果 $y_1, y_2$ 是 $G$ 中的两个点，它们是全等的 mod。 $N$ 然后$\langle x, y_1 \rangle = \langle x, y_2 \rangle$ 对于所有$x \in M$。对于每个类 $\dot{y}$ 模。 $N$，表示当$y$在$\dot{y}$变化$\langle x, \dot{y} \rangle$时，$\langle x, y \rangle$的公共的值；显然，$(x, \dot{y}) \mapsto \langle x, \dot{y} \rangle$ 是 $M \times (G/N)$ 上的双线性形式。

#### 命题 7 {#evt-ii-s6-prop-7 .statement tag=07HO}

— *令$M$为$F$的向量子空间，以及$G$的$N$向量子空间，其中$F$和$G$是对偶中的两个向量空间。假设$M$和$N$是正交的（相当于说、$N \subset M^\circ$或$M \subset N^\circ$）。 向量空间 $M$ 和 $G/N$ 则通过双线性形式* $(x, \dot{y}) \mapsto \langle x, \dot{y} \rangle$ 成为对偶。

(i) *拓扑$\sigma(M, G/N)$，这种对偶性是由$\sigma(F, G)$引发的（特别是我们有$\sigma(F, G) = \sigma(F, G/F^\circ)$）。

(ii) *拓扑 $\sigma(G/N, M)$ 对于这种对偶性比 $\sigma(G, F)$ 与 $N$ 的商拓扑更粗糙；当且仅当$M + G^\circ = N^\circ$时，这些拓扑是相同的。

(i) $G/N$ 的每个元素都是类 mod。 $G$元素$N$；如果$z_i (1 \leq i \leq n)$是$G$的元素，$\dot{z}_i (1 \leq i \leq n)$是$G/N$中$z_i$的类，则$y \in M$的集合，使得$1 \leq i \leq n$的$|\langle y, \dot{z}_i \rangle| \leq \alpha$是迹那些$x \in F$中的集合中的$M$使得$|\langle x, z_i \rangle| \leq \alpha$对应$1 \leq i \leq n$；结论是从弱拓扑为0的定义或邻域得出的。

(ii) 设$p : G \to G/N$为典范满射。我们证明* $\sigma(G, F)$ *与* $N$ *的商拓扑* $\mathscr{T}$ *与* $\sigma(G/N, N^\circ)$ 相同。因为，对于$z \in G, y \in N^\circ$，我们有$\langle y, p(z) \rangle = \langle y, z \rangle$，因此$\sigma(G/N, N^\circ)$的每个0的邻域都是形式$p(V)$，其中$V$是$\sigma(G, F)$的0的邻域，对于关系饱和$z - z' \in N$，因此$\mathscr{T}$ 比$\sigma(G/N, N^\circ)$ 更细。相反，对于$\sigma(G, F)$，令$U = W(y_1, ..., y_n; \alpha)$为$G$中0的邻域，其中$y_i \in F$对于$1 \leq i \leq n$和$\alpha > 0$；我们将看到，对于$1 \leq i \leq n$，存在元素$t_i \in N^\circ$，这样如果有人放入$U' = W(t_1, ..., t_n; \alpha)$，则$p(U') \subset p(U)$；这将表明 $\sigma(G/N, N^\circ)$ 比 $\mathscr{T}$ 更细，因此实际上与 $\mathscr{T}$ 相同。现在，令$L$为$N^\circ$和$y_i$生成的$F$的向量子空间，并用$P$表示$L$中$N^\circ$的补子空间；它是有限维，比如说$m$。设$(x_j)_{1 \leq j \leq m}$为$P$中的基； 线性形式 $x \mapsto \langle x_j, z \rangle$ 的限制到 $N$ 是线性独立的，因为否则 $P$ 中存在 $x \neq 0$，使得 $\langle x, z \rangle = 0$ 对于所有 $z \in N$，也就是说 $x \in N^\circ$，其中与……矛盾定义共 $P$。因此我们结论，对于所有$z' \in G$，存在$s \in N$，使得$\langle x_j, z' \rangle = \langle x_j, s \rangle$对于所有$j$；如果$z' = z + s$，我们对所有$x \in P$有$\langle x, z \rangle = 0$。既然如此，则放入$y_i = t_i + w_i$，其中$t_i \in N^\circ$和$w_i \in P$；我们有$\langle y_i, z \rangle = \langle t_i, z \rangle = \langle t_i, z' \rangle$换$1 \leq i \leq n$；因此，对于所有$z' \in U'$，存在$z \in U$使得$z' - z \in N$，也就是说我们有$p(U') \subset p(U)$。

回到M是N°中任意子空间的情况，注显然是$\sigma(G/N, M) = \sigma(G/N, M + G^\circ)$；进一步，从道具。 II、p. 43的3，我们看到，如果$y \in N^\circ$使得线性形式$\dot{z} \mapsto \langle y, \dot{z} \rangle$对于$\sigma(G/N, M)$连续，则必然$y \in M + G^\circ$。我们结论认为条件$M + G^\circ = N^\circ$对于商拓扑$\mathscr{T}$等于$\sigma(G/N, M)$是必要且充分的。

#### 注 {#evt-ii-s6-n5-rem-1 .statement tag=07HP}

— M 和 G/N 之间的对偶性（其中 M 和 N 是两个正交子空间）在 M 中分离，当且仅当 $M \cap G^\circ = \{0\}$；当且仅当 $N = M^\circ$ 时，它在 G/N 中分离。

#### 推论 1 {#evt-ii-s6-prop-7-cor-1 .statement tag=07HQ}

— 假设 F 和 G 之间的对偶性在 F 中分离。对于 F 拓扑 $\sigma(G/M^\circ, M)$ 的向量子空间 M 与 $\sigma(G, F)$ 的商拓扑除以$M^\circ$，当且仅当 M 对于拓扑是闭集$\sigma(F, G)$。

这是从道具得出的。 7 放入$N = M^\circ$，并回顾$M^{\circ \circ}$是M对于$\sigma(F, G)$的闭包（II，p. 45，cor.2）。

#### 推论 2 {#evt-ii-s6-prop-7-cor-2 .statement tag=07HR}

— 如果 M 为有限维 n 并且对偶性在 F 中分离，则 $M^\circ$ 在 G 中具有余维 n。如果 M 对于 $\sigma(F, G)$ 且为有限余维 n 是闭的，并且如果对偶性在 G 中分离，则 $M^\circ$ 为维数 n。

对于，$G/M^0$与M处于分离对偶性；如果 M 为维数 n，则$G/M^\circ$ (II, p. 41, 例 1) 也同样如此。如果M是闭集，则$F/M = F/M^{\circ \circ}$与$M^\circ$处于分离对偶性；如果 F/M 为维数 n，则对于 $M^\circ$ (II、p. 41、例 1) 来说是相同的。

#### 推论 3 {#evt-ii-s6-prop-7-cor-3 .statement tag=07HS}

— 令 (F, G), (F_1, G_1) 为分离对偶中空间的两个对，令 u 为 F_1 中 F 的线性映射，对于 $\sigma(F, G)$ 和 $\sigma(F_1, G_1)$ 连续。那么 u 是 F_1 中 F 的严格态射，当且仅当，Im($^t u$) 是 G 中$\sigma(G, F)$ 的闭子空间。

让$N = \operatorname{Im}(^t u) \subset G$；我们知道 F 中的 $N^0 = \operatorname{Ker}(u)$ (II, p. 47, 公式 (3))。令 $p : F \to F/N^\circ$ 为典范映射，以便 u 因式分解为

$$
u : F \xrightarrow{p} F/N^\circ \xrightarrow{w} F_1,
$$

其中 w 是单射。 空间$F/N^\circ$和N处于分离对偶性，并且通过II、p. 48的公式(1)，我们对所有$\dot{y} \in F/N^\circ$和$z_1 \in G_1$有$\langle w(\dot{y}), z_1 \rangle = \langle \dot{y}, ^t u(z_1) \rangle$。这个关系表明w是$F/N^\circ$的同构，携带拓扑$\sigma(F/N^\circ, N)$，在$u(F)$上，并由$\sigma(F_1, G_1)$诱导拓扑。因此结论来自cor。 1 和严格的态射的定义。

#### 推论 4 {#evt-ii-s6-prop-7-cor-4 .statement tag=07HT}

— 令 (F, G), (F_1, G_1) 为分离对偶中的两个对，并令 u 为 F_1 中 F 的线性映射，对于 $\sigma(F, G)$ 和 $\sigma(F_1, G_1)$ 连续。那么u是满射的，当且仅当，$^t u$是$G_1$的同构（与拓扑$\sigma(G_1, F_1)$）在$^t u(G_1)$上，并且由$\sigma(G, F)$诱导拓扑。

因为，如果说$u(F) = F_1$等价于说，那么对于$\sigma(F_1, G_1)$，$u(F)$是封闭的且在$F_1$处处密集；科。 4 随后来自 cor。 3 适用于 $^t u$ 和 II、p. 47，cor。 2.

#### 注 {#evt-ii-s6-n5-rem-2 .statement tag=07HU}

— 1) 在分离对偶性时，令$(F_1, G_1), (F_2, G_2), (F_3, G_3)$为空间中的三个对，并考虑两个线性映射中的序列

$$
F_1 \xrightarrow{u} F_2 \xrightarrow{v} F_3
$$

对于弱拓扑相应的分别与$G_1, G_2, G_3$连续；我们考虑转置映射的序列

$$
G_3 \xrightarrow{^tv} G_2 \xrightarrow{^tu} G_1 .
$$

显然$^t(v \circ u) = ^t u \circ ^t v$，因此关系$v \circ u = 0$等价于$^t u \circ ^t v = 0$。 序列 (5) 是精确的当且仅当满足以下三个条件

a）$^t u \circ ^t v = 0$；
b) $\operatorname{Im}(^t v)$ 在 $\operatorname{Ker}(^t u)$ 中是稠密的；
c) $^t u$ 是$G_1$ 中$G_2$ 的严格态射。

这实际上遵循cor。 II、p. 49和公式中的3个（3）和（4）中的II、p. 47。

2) 千万不能认为当$u$是$F_1$中$F$的严格态射时，$^t u$就一定是$G$中$G_1$的严格态射；在其他情况下，字$u$可以是严格的态射，而无需在$F_1$中针对$\sigma(F_1, G_1)$关闭$u(F)$。这由例表示，其中$F$是$F_1$和$G = G_1 / F^\circ$的非闭子空间，$u$是典范嵌入。类似地，序列 (5) 精确并不一定意味着 (6) 精确，但是，如果序列 (5) 精确且 $v$ 是严格的态射，则序列 (6) 精确，通过注 1 和 II， p. 49，科尔。 3.

### 6. 乘积弱拓扑

#### 命题 8 {#evt-ii-s6-prop-8 .statement tag=07HV}

— 设$(F_i, G_i)_{i \in I}$是对偶性中空间的对族。设$F = \prod_{i \in I} F_i$为$F_i$的乘积空间，$G = \bigoplus_{i \in I} G_i$为$G_i$的直和。如果对于所有 $x = (x_i) \in F$ 和所有 $y = (y_i) \in G$，我们写 $\langle x, y \rangle = \sum_{i \in I} \langle x_i, y_i \rangle$ （和只有有限多个非零项），那么拓扑 $\sigma(F, G)$ （相对于双线性形式 $(x, y) \mapsto \langle x, y \rangle$）是乘积拓扑$\sigma(F_i, G_i)$。

对于，给定$F$上的拓扑$\mathscr{T}$；在阶中，对于所有 $y \in G$，线性形式 $x \mapsto \langle x, y \rangle$ 应连续于 $\mathscr{T}$，通过 $\langle x, y \rangle$ 的定义，映射 $x \mapsto \langle \operatorname{pr}_i x, y_i \rangle$ 应连续于$\mathscr{T}$，其中$i$在$I$中任意，而$y_i$在$G_i$中任意；但这意味着$F_i$中$F$的映射$\operatorname{pr}_i$对于$\mathscr{T}$和$\sigma(F_i, G_i)$都是连续的（I，p. 10，cor.1）；这样就完成了演示。

#### 注 {#evt-ii-s6-n6-rem-1 .statement tag=07HW}

— $F$ 和 $G$ 之间的对偶性在 $F$ 中分离（分别在 $G$ 中）当且仅当对于所有 $i \in I$，$F_i$ 和 $G_i$ 之间的对偶性在 $F_i$ 中分离（分别在 $G_i$ 中）。如果$F$和$G$之间的对偶性在$F$（分别$G$）中分离，那么，在$F$（分别$G$）中，子空间与一$G_i$（分别$F_i$）正交，规范地用$G$（或$F$）的子空间来识别是$F_\kappa$的乘积的子空间，其中$\kappa \neq i$（或$G_\kappa$的直和，使得$\kappa \neq i$）。

#### 推论 1 {#evt-ii-s6-prop-8-cor-1 .statement tag=07HX}

— 令 F 和 G 为分离对偶性中的两个向量空间。如果空间 F（与$\sigma(F, G)$）是两个子空间 M、N 的直接拓扑和，则空间 G（与$\sigma(G, F)$）是分别与M 和N 正交的子空间 $M^\circ, N^\circ$ 的直接拓扑和。

令$p : F \to M, q : F \to N$为F的投影算子相应的到分解到M和N的直和；其中条件映射$(p, q) : F \to M \times N$是拓扑同构。如果$M_1 = G/M^\circ, N_1 = G/N^\circ$，则M和N上的拓扑（由F的拓扑诱导）分别与$\sigma(M, M_1)$、$\sigma(N, N_1)$相同（II、p. 48，命题7）。当我们通过prop给$M_1, N_1$和G拓扑$\sigma(M_1, M)$、$\sigma(N_1, N)$和$\sigma(G, F)$时，映射$^t(p, q) : M_1 \times N_1 \to G$是拓扑同构。 8.在此下，映射$M_1$（分别$N_1$）在G中具有像子空间$N^\circ$（分别$M^\circ$）和拓扑$\sigma(M_1, M)$（分别$\sigma(N_1, N)$） 像拓扑由 $\sigma(G, F)$ 在 $N^\circ$（或$M^\circ$）上诱发，由此得出推论。

#### 推论 2 {#evt-ii-s6-prop-8-cor-2 .statement tag=07HY}

— 令 $(e_i)_{i \in J}$ 为向量空间 F 与对偶 $F^*$ 的基，并令 $u : \mathbf{R}^{(I)} \to F$ 为由此基定义的（代数）同构。那么当$F^*$携带拓扑$\sigma(F^*, F)$和$\mathbf{R}^I$乘积拓扑时，转置的映射$^t u : F^* \to \mathbf{R}^I$是拓扑同构。

我们知道（A，II, § 2.6，道具10）$^t u$是双射，并且如果对于$x^* \in F^*$，我们为所有$i \in I$放置$\langle e_i, x^* \rangle = \xi_i^*$，那么像$^t u(x^*)$是向量$(\xi_i^*)$ $\mathbf{R}^I$，因此，对于 F 中的所有 $x = \sum_i \xi_i e_i$，我们有 $\langle x, x^* \rangle = \sum_i \xi_i \xi_i^*$。然后从这个公式和道具得出推论。 8.

### 7. 弱完全空间

#### 命题 9 {#evt-ii-s6-prop-9 .statement tag=07HZ}

— 令 F, G 为分离对偶性中的两个向量空间。如果$\hat{F}$是拓扑$\sigma(F, G)$的空间F的完成，并且如果我们考虑典范嵌入$j : F \to G^*$，其中$G^*$有拓扑$\sigma(G^*, G)$，那么j的连续扩张$\hat{j} : \hat{F} \to G^*$是拓扑向量空间的同构。

因为，我们看到 $G^*$ 赋予 $\sigma(G^*, G)$，是 Hausdorff 且完备的（II，p. 51，cor. 2）；如果我们通过j 认同 F 且$G^*$ 的向量子空间则$\sigma(G^*, G)$ 在F 上诱导的拓扑为$\sigma(F, G)$，并且F 在拓扑 $\sigma(G^*, G)$ 中的$G^*$ 是稠密的（II， p. 43，4)；由此得出命题。

因此，对于弱拓扑来说完备的向量空间是任意向量空间 G 赋予 $\sigma(G^*, G)$ 的对偶 $G^*$； 之后II，p. 51，相关。 2，它们（拓扑）同构于乘积 $\mathbf{R}^I$ 或实直线。为了简化语言，我们将它们称为线的乘积（有关这些空间的内在特征，请参见II，p. 85，执行13和II，p. 81，执行1）。

我们注在$G^*$上，$\sigma(G^*, G)$拓扑在豪斯多夫弱拓扑中是最小的；因为，比$\sigma(G^*, G)$更粗糙的弱拓扑必然是形式$\sigma(G^*, H)$，其中$H \subset G$（II，p. 43，cor.3）；但如果$H \neq G$，则存在非空且与$H$正交的线性形式$x^* \in G^*$（A，II, § 7.3，命题8），因此$\sigma(G^*, H)$不是Hausdorff。

我们从这个注推断出，如果$F, G$是两个向量空间，那么对于拓扑$\sigma(G^*, G)$和$\sigma(F^*, F)$来说连续的*线性双射*$u : G^* \to F^*$必然是*双连续*。

#### 命题 10 {#evt-ii-s6-prop-10 .statement tag=07I0}

*令$G$为实数向量空间，$F = G^*$与拓扑$\sigma(G^*, G)$对偶。*

(i) *The mapping $V \mapsto V^\circ$ is a bijection of the set of vector subspaces of $G$ on the set of closed vector subspaces of $F$.*

(ii) *$F$的每个闭向量子空间都是乘积条线，并且有一个拓扑补集。*

由双极定理（II、p. 45，cor.2）$V \mapsto V^\circ$为$G$的向量子空间$V$集合双射，$\sigma(G, G^*)$*关闭* 集合关闭向量子空间 $F$。但是，到定义，$G$上的*每个*线性形式对于$\sigma(G, G^*)$都是连续的，因此$G$中的每个向量子空间都是封闭的，由方程$\langle y, y_\lambda^* \rangle = 0$的系统定义（其中$y_\lambda^* \in G^*$）；这就证明了(i)。

现在让$W$是$F$的闭子空间；然后我们就有 $W = V^\circ$ 和 $G$ 中的 $V = W^\circ$。设$V'$是$G$中$V$的补集。我们知道$F = G^*$可以与$V^* \oplus {V'}^*$规范地识别，${V'}^*$可以与$V^\circ = W$识别（A，II, § 2.6，对应第10条）；进一步（II，p. 50，道具8）拓扑$\sigma(G^*, G)$可以与拓扑$\sigma(V^*, V)$和$\sigma({V'}^*, V')$中的乘积识别；这就证明了断言(ii)。

虽然，对于拓扑 $\sigma(G, G^*)$，$G$的每一个向量子空间都是闭合的，我们注如果$G$是无限的维数那么拓扑$\sigma(G, G^*)$不是$G$上最好的局部凸拓扑，对于无限维数的$\sigma(G, G^*)$包含向量子空间，每个邻域为0：然而，它是$G$上最好的“弱”拓扑（II，p. 43，cor.3）。

### 8.弱空间中的完全凸锥

#### 引理 1 {#evt-ii-s6-lem-1 .statement tag=07I1}

*令$E$为豪斯多夫弱空间，$C$为$E$中顶点为0的真圆锥，对于由$E$诱导的均匀结构来说是完整的。 $E$ 中的每个连续线性形式是 $E$ 中两个连续线性形式之间的差，且$C$ 中为正数。*

令 $E'$ 为 $E$ 的对偶，$F$ 为 $E'$ 的代数对偶，其中拓扑 $\sigma(F, E')$。令$H = C^\circ - C^\circ$为$E'$的向量子空间，由线性形式的差形成，线性形式在$E$中连续且在$C$中为正（II，p. 44，道具4）。只要证明$F$中与$H$正交的是$\{0\}$（II，p. 41，*例* 1）即可。然后令$a \in F$与$H$正交；由于 $a$ 与 $C^\circ$ 正交，因此它必须属于于 $F$ 中 $C$ 的双极性。但是$E$可以识别为$F$的子空间，并且由于$C$是完整的，因此在$F$中闭合，我们有$a \in C$（II，p. 44，第1）。类似地，$a$ 与$-C^\circ$ 正交，因此$a \in -C$。由于$C$是正确的，所以我们有$a = 0$。

#### 命题 11 {#evt-ii-s6-prop-11 .statement tag=07I2}

*令$E$为Hausdorff弱空间，$C$为$E$中顶点为0的真凸锥，并且在由$E$诱导的一致结构中是完全的。*

那么在乘积空间$\mathbf{R}^I$中存在集合I和E的连续线性映射u，具有以下性质：

a) u 是 $u(C)$ 上C 的同构，分别由 E 和$\mathbf{R}^I$ 的均匀结构引起。

b) 我们有 $u(C) \subset \mathbf{R}_+^I$。

此外，如果由 E 在 C 上导出的一致结构是可度量的，那么我们可以取 $I = \mathbf{N}$。

令$(f_i)_{i \in I}$为E中的连续线性形式族，使得形式$(x, y) \mapsto |f_i(x - y)|$在$C \times C$定义上的伪度量的有限和是C的一致结构。 （如果结构可度量，我们可以取$I = \mathbf{N}$。）到引理1，我们可以进一步假设每个$f_i$在C中都是正数。令u为$\mathbf{R}^I$中E的线性映射$x \mapsto (f_i(x))_{i \in I}$。显然 u 是连续的并且 $u(C) \subset \mathbf{R}_+^I$。 限制 $u|C$ 是一致连续的映射，它是从 C 到 $u(C)$ 的满射。此外，如果C中的$x, y$对于所有$i \in I$来说是$f_i(x) = f_i(y)$，则$x = y$，因为C的均匀结构是Hausdorff；因此 $u|C$ 是双射的。最后，如果 W 是 C 的均匀结构的周围，则存在I和数$\varepsilon > 0$的有限集合 J，使得$i \in J$的关系$|f_i(x) - f_i(y)| \leq \varepsilon$意味着$(x, y) \in W$；因此，对于所考虑的制服结构，$u|C$ 是 $u(C)$ 上的 C 的同构。

#### 推论 1 {#evt-ii-s6-prop-11-cor-1 .statement tag=07I3}

— 令 E 为 Hausdorff 弱空间和 C E 中顶点 0 的真凸锥，对于 E 的一致结构是完全的。则 C 中$C \times C$ 的映射 $(x, y) \mapsto x + y$ 是正确的。

因为道具。 11，我们可以假设$E = \mathbf{R}^I$和$C = \mathbf{R}_+^I$（GT，I, § 10.1，cor.1和4）。但是C中$C \times C$的映射$(x, y) \mapsto x + y$写成$((\xi_i), (\eta_i)) \mapsto (\xi_i + \eta_i)$，我们可以将自己限制为证明，$\mathbf{R}_+$中$\mathbf{R}_+ \times \mathbf{R}_+$的连续映射$f : (\xi, \eta) \mapsto \xi + \eta$是正确的（GT，I, § 10.1，cor.3），现在，对于所有$\zeta \in \mathbf{R}_+$，我们看到$f(\zeta)$是对$(\xi, \zeta - \xi)$的集合，使得$0 \leq \xi \leq \zeta$，因此逆像除以区间$[0, \zeta]$的f是$(\xi, \eta) \in \mathbf{R}_+ \times \mathbf{R}_+$的集合使得$\xi + \eta \leq \zeta$，这是紧致的。结论如下应用（GT，I, § 10.3，第7条）。

#### 推论 2 {#evt-ii-s6-prop-11-cor-2 .statement tag=07I4}

— 令 E 为 Hausdorff 弱空间，以及 C 一个在 E 中顶点为 0 的真凸锥，对于由 E 导出的均匀结构是完整的。

(i) 对于 E 的每个点 a，交 $C \cap (a - C)$ 是紧致的。

(ii) 令 A、B 为C 中的两个闭集合。那么$A + B$就是C中的闭集合。

(i) $(x, y) \in C \times C$ 的集合使得 $x + y = a$ 是紧凑的。 1 和来自 GT，I, § 10.2，th。 1、b）。现在这个集合也是$(x, a - x)$对于$x \in C \cap (a - C)$的集合，这就证明了(i)。

(ii) 如果 A 和 B 在 C 内闭，则 $A \times B$ 在 $C \times C$ 内闭，因此 $A + B$ 在 C 之后内闭。 1 和 GT，I, § 10.1，道具。 1.

### 习题{#evt-ii-s6-exercises}

§ 6](exercises/s6/)参见[习题。
