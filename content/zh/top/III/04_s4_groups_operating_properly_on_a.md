---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 4
section_title: Groups operating properly on a topological space; compact ness in topological groups and spaces with operators
lang: zh
source: top-i-iv
book_pages: 250-261, 308-314
pdf_pages: 0256-0267, 0314-0320
extraction: ocr
subsections:
    - "no": 1
      title: GROUPS OPERATING PROPERLY ON A TOPOLOGICAL SPACE
      page: 250
      pdf_page: 256
    - "no": 2
      title: PROPERTIES OF GROUPS ACTING PROPERLY
      page: 253
      pdf_page: 259
    - "no": 3
      title: GROUPS OPERATING FREELY ON A TOPOLOGICAL SPACE
      page: 254
      pdf_page: 260
    - "no": 4
      title: LOCALLY COMPACT GROUPS OPERATING PROPERLY
      page: 255
      pdf_page: 261
    - "no": 5
      title: GROUPS OPERATING CONTINUOUSLY ON A LOCALLY COMPACT SPACE
      page: 257
      pdf_page: 263
    - "no": 6
      title: LOCALLY COMPACT HOMOGENEOUS SPACES
      page: 259
      pdf_page: 265
statements: 33
exercises: 23
content_sha256: 42863e22074036b9e1b84c24da961b3f1f1d18aebe1fda69969db6209944d5cf
translated_from: content/en/top/III/04_s4_groups_operating_properly_on_a.md
translation_method: google
source_content_sha256: 2ea085e7d32aa31b87b7e5e944f3f6487ad556472cc1fd617b46f58ffb5fe66b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 5c2ce31120545ceb0bcd6fc0cba1eb4e0c0d1cc4f89bb13e07791a83cf980eaf
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 4. 群在拓扑空间上正常运行；具有运算符的拓扑群和空间的紧致性

### 1. 群在拓扑空间上正常运行

#### 定义 1 {#top-iii-s4-def-1 .statement tag=0BKR}

令$G$为在拓扑空间$X$上连续运行的拓扑群。如果映射则 $G$ 据说可以在 $X$ 上正常运行

$$
\theta : (s, x) \to (x, s.x) \text{ of } G \times X \text{ into } X \times X
$$

是正确的（章I, § 10, no. 1，定义1）。

设$\Gamma \subset G \times X \times X$为映射$\rho : (s, x) \to s.x$的图。由于$\rho$是连续的，映射$\sigma : (s, x) \to (s, x, s.x)$是$G \times X$到$\Gamma$的同胚，并且复合映射

$$
G \times X \xrightarrow{\sigma} \Gamma \xrightarrow{\mathrm{pr}_{23}} X \times X
$$

只是$\theta$。因此，定义 1 等价于说，$\mathrm{pr}_{23}$到$\Gamma$的限制是$\Gamma$到$X \times X$的真映射。

章 I, § 10, no. 2 中的定理 1 表明，当且仅当满足以下条件时，G 在X 上正确运行：
对于每个集合 A 通过超滤器 $\mathfrak{F}$ 过滤，以及每个映射
$$
\alpha \to (s_\alpha, x_\alpha)
$$
将 A 转化为 $G \times X$，如果映射 $\alpha \to (s_\alpha \cdot x_\alpha, x_\alpha)$ 相对于 $\mathfrak{F}$ 具有极限 $(b, a)$，则 $\alpha \to s_\alpha$ 相对于 $\mathfrak{F}$ 具有极限 $t \in G$，使得 $t.a = b$。

#### 例 1 {#top-iii-s4-n1-exa-1 .statement tag=0BKS}

令 H 为拓扑群 G 的闭子群。如果 G 在 X 上正确运行，那么 H 也能正确运行，因为 $H \times X$ 在 $G \times X$ 中是封闭的 (章 I, § 10, no. 1, 命题 5, 推论 1)。例如，如果我们采用 $X = G$，G 通过左平移对自身进行操作，则映射 $G \times X \to X \times X$ 是同胚，因此是正确的；因此 H 通过左平移在 G 上正确运行。

#### 例 2 {#top-iii-s4-n1-exa-2 .statement tag=0BKT}

如果G在X上正确运行，那么它在X的每个子空间$X'$上正确运行，即X的点的轨道的并（在其他字，$X'$相对于饱和） 等价关系由 G) 定义。对于$G \times X$中$X' \times X'$的逆像是$G \times X'$，我们可以得到章I, § 10, no. 1的应用命题 3。

#### 命题 1 {#top-iii-s4-prop-1 .statement tag=0BKU}

设G是在拓扑空间X上连续运行的拓扑群，设K是G的拟紧子集。则$K \times X$的映射$\rho : (s, x) \to s.x$入X是正确的。

$\rho$因式分解为$K \times X \to K \times X \xrightarrow{\mathrm{pr}_2} X$，其中$\alpha(s, x) = (s, s.x)$。 $\alpha$ 是同胚，因为 $\alpha^{-1} : (s, y) \to (s, s^{-1}.y)$ 是连续的。由于 K 是拟紧的，所以 $\mathrm{pr}_2$ 是适当的 (章 I, § 10, no. 2, 定理 1, 推论 5)；因此$\rho$是正确的（章I, § 10, no. 1，命题5）。

#### 推论 1 {#top-iii-s4-prop-1-cor-1 .statement tag=0BKV}

如果 A 是 X 的闭（或紧）子集，则 K.A 在 X 中是闭的（如果 X 是 Hausdorff，则又是紧）。

关于闭集合的断言由命题 1 得出，并且真映射是闭的（章 I, § 10, no. 1，命题 1）。 断言关于紧集是微不足道的。

需要注意的是，如果L是X的紧子集，并且F是G的闭子集，那么F.L不一定在X中闭（$§ 2$，习题29；cf.no. 5， 推论至命题 12)。

#### 推论 2 {#top-iii-s4-prop-1-cor-2 .statement tag=0BKW}

如果 K 是拓扑群 G 的拟紧子群，则等价关系 $x^{-1}y \in K$ 是闭集，典范映射 $\varphi : G \to G/K$ 是正确的。

第一个断言源自推论 1，通过对其自身进行右平移应用于 G，第二个断言则源自章 I, , no. 2, 定理 1

#### 推论 3 {#top-iii-s4-prop-1-cor-3 .statement tag=0BKX}

令 K 为拓扑群 G 的准紧法线子群，并令 φ 为典范映射 G → G/K。那么对于 G 的每个闭子群 A，A/A ∩ K 在 φ(A) 上的规范双射是拓扑群的同构。

由于 x⁻1y ∈ K 是闭等价关系 (推论 2)，推论由章 I, § 5, no. 2、命题 4 得出。

#### 命题 2 {#top-iii-s4-prop-2 .statement tag=0BKY}

令 K 为在 Hausdorff 空间 X 上连续运行的紧致群。然后：

a) K 在X 上正常运行。
b) 将K × X 映射 (s, x) → s.x 化为X 是正确的。
c) X 的典范映射到 X/K 上是合适的。

b) 是命题 1 的推论。对于 a)，由于 K 是紧的，所以 pr2 : (s, x) → x 是正确的 (章 I, § 10, no. 2, 定理 1, 推论 5)；因此，X为豪斯多夫，(s, x) → (x, s.x) 是正确的 (章 I, § 10, no. 1, 命题 5, 推论 3)。仍有待证明c）。从推论 1 到命题 1，典范映射 φ : X → X/K 关闭。如果 Z 是任意拓扑空间并且我们让 K 在 Z 上进行平凡运算，则 K 在 X × Z 上连续运算，因此典范映射 X × Z → (X × Z)/K 是闭合的。但是 (X × Z)/K 可以被规范地识别为 (X/K) × Z (§ 2, no. 4, 引理 2 和章 I, § 5, no. 3, 推论到命题 8)；因此典范映射 X × Z → (X × Z)/K 可以等同于 φ × 1，并且由于它对于所有 Z 都是封闭的，因此 φ 是正确的。

#### 推论 1 {#top-iii-s4-prop-2-cor-1 .statement tag=0BKZ}

在命题 2 的假设下，X 是紧致的（或局部紧致）当且仅当 X/K 是紧致的（或局部紧致）。

这是因为，鉴于章 I, § 10, no. 4 的命题 9，典范映射 X → X/K 是正确的。

#### 推论 2 {#top-iii-s4-prop-2-cor-2 .statement tag=0BL0}

令 G 为豪斯多夫拓扑群，并令 K 为 G 的紧子群。则 G 是紧的（或局部紧的）当且仅当 G/K 是紧的（或局部紧的）。

应用推论 1 到 K 通过右平移在 G 上运算。

### 2. 群的属性正确发挥作用

#### 命题 3 {#top-iii-s4-prop-3 .statement tag=0BL1}

*如果拓扑群* $G$ *在拓扑空间* $X$ 上正确运行，*则轨道空间* $X/G$ *是 Hausdorff*。 *如果也* $G$ *是豪斯多夫*，*则* $X$ *是豪斯多夫*。

设$C \subset X \times X$为$G$在$X$上定义的等价关系$R$的图；那么$C$是映射$\theta : (s, x) \to (x, s.x)$下$G \times X$的像。由于 $\theta$ 是正确的，$C$ 在 $X \times X$ 中闭合（章 I, § 10, no. 1，命题 1）。由于关系 $R$ 是开集 ($§ 2$, no. 4, 引理 2)，因此 $X/G$ 是 Hausdorff (章 I, § 8, no. 3, 命题 8)。

现在假设 $G$ 是 Hausdorff。那么$X$的映射$x \to (e, x)$到$G \times X$是$X$到$G \times X$的闭子空间的同胚，因此是正确的（章I, § 10, no. 1，命题2）。如果我们将这个映射与$G \times X$的映射$(s, x) \to (x, s.x)$组合成$X \times X$，其中假设是正确的，我们得到$X$的真映射到$X \times X$，即对角线映射 $x \to (x, x)$。因此，$X \times X$的对角线$\Delta$在$X$中闭合，因此$X$是Hausdorff。

#### 命题 4 {#top-iii-s4-prop-4 .statement tag=0BL2}

*设* $G$ *为拓扑群，在拓扑空间* $X$上正确运行，*并让* $x$ *为* $X$的点。 *令*$G.x$*表示*$x$的轨道，*并令*$K_x$*表示*$x$的稳定子。 *然后*：

a) *映射* $s \to s.x$ *属于* $G$ *进入* $X$ *是正确的*。

b) $K_x$ *是准紧凑*。

c) *$G/K_x$ *到* $G.x$ *的典范映射 *是同胚*。

d) *轨道* $G.x$ *于* $X$ 关闭。

$\theta : (s, x) \to (x, s.x)$下$\{ x \} \times X$的逆像为$G \times \{ x \}$；因此，通过章I, § 10, no. 1的命题3，$\theta$到$G \times \{ x \}$的限制是$G \times \{ x \}$到$\{ x \} \times X$的真映射，从而如下：由于$K_x$是$s \to s.x$下$x$的逆像，b)由章I, § 10, no. 2、定理1得出。c)和d)是a)的推论，根据章 I, § 10, no. 1、命题 2 和 5 b)。

#### 注 {#top-iii-s4-n2-rem-1 .statement tag=0BL3}

命题 4 表明，如果拓扑群 $G$ 在齐次空间 $G/H$ 上正确运行，则子群 $H$ 是拟紧的（因此如果 $G$ 是 Hausdorff，则也是紧的）。可以证明，这也是 $G$ 在 $G/H$（习题 3）上正常运行的充分条件。

#### 命题 5 {#top-iii-s4-prop-5 .statement tag=0BL4}

*令* $G$ *（分别* $G'$）*成为在拓扑空间* $X$ *（分别* $X'$）上连续运行的拓扑群。 *令* $\varphi$ *为$G$到$G'$的连续同态*，并让$\psi$为$X$到$X'$的连续映射，与$\varphi$（§ 2, no. 4）相容的。然后：

(i) *如果 $\varphi$ 是满射且 $\psi$ 是满射且正确，并且如果 $G$ 在 $X$ 上正确运行，则 $G'$ 在 $X'$ 上正确运行。*

(ii) *如果$\varphi$是正确的，如果$G'$在$X'$上正确运行，并且如果$X$是Hausdorff，那么$G$在$X$上正确运行。*

为了证明 (i)，考虑交换律图表

$$
\begin{array}{ccc}
G \times X & \xrightarrow{\theta} & X \times X \\
\alpha \downarrow & & \downarrow \beta \\
G' \times X' & \xrightarrow{\theta'} & X' \times X'
\end{array}
$$

其中 $\alpha = \varphi \times \psi$ 和 $\beta = \psi \times \psi$。 假设时，$\theta$为宜； $\beta$ [章 I, § 10, no. 1, 命题 4 a)]；因此 $\beta \circ \theta = \theta' \circ \alpha$ 是正确的 [章 I, § 10, no. 1, 命题 5 a)]。由于 $\alpha$ 是满射，因此 $\theta'$ 是正确的 [章 I, § 10, no. 1, 命题 5 b)]。

为了证明 (ii) 考虑在 $G \times X$ 上使用超滤器 $U$，使得映射

$$
(s, x) \to s.x \quad \text{and} \quad (s, x) \to x
$$

相对于$U$分别收敛到$y_0$和$x_0$。由此可知$(s, x) \to \varphi(s).\psi(x)$和$(s, x) \to \psi(x)$相对于$U$收敛。由于$G'$在$X'$上正确运行，这意味着（no. 1）$(s, x) \to \varphi(s)$相对于$U$收敛到点$s'_0 \in G'$。由于$\varphi$是正确的，我们推断(章I, § 10, no. 2,定理1)$(s, x) \to s$相对于$U$收敛到点$s_0 \in G$。 $X$中极限的唯一性则显示$y_0 = s_0 x_0$，因此$G$在$X$（no. 1）上正常运行。

### 3. 群在拓扑空间上自由运行

#### 定义 2 {#top-iii-s4-def-2 .statement tag=0BL5}

*令$G$为群，在集合$X$上运行。如果$X$的每个元素的稳定子是$\{e\}$，则$G$可以在$X$上自由运行，在其他字，如果关系$s.x = x,\ s \in G,\ x \in X$暗示$s = e$。*

#### 例 {#top-iii-s4-n3-exa-1 .statement tag=0BL6}

令$G$为群，令$H$为$G$的子群。然后$H$通过（左或右）平移在$G$上自由操作。

令$G$为在集合$X$上自由运算的群，令$R$为由$G$在$X$上定义的等价关系，令$C \subset X \times X$为$R$的图。如果$(x, y) \in C$，则存在$s \in G$使得$s.x = y$；并且$s$是*唯一的*，因为$s.x = s'.x$意味着${s'}^{-1}s.x = x$，因此${s'}^{-1}s = e$（因为$G$自由运行）。如果我们使对应到$(x, y) \in C$唯一的$s \in G$使得$s.x = y$，我们定义映射$\varphi : C \to G$，我们将把$C$的典范映射称为$G$。有了这个记号：

#### 命题 6 {#top-iii-s4-prop-6 .statement tag=0BL7}

*令$G$为在拓扑空间$X$上连续运行的拓扑群，并假设$G$在$X$上自由运行。那么当且仅当满足以下条件时，$G$才能在$X$上正常运行：*

(FP) *由$G$定义的等价关系的图$C$在$X \times X$中闭合，并且典范映射$\varphi : C \to G$是连续的。*

集合$C$是$G \times X$的映射$\theta : (s, x) \to (x, s.x)$到$X \times X$的像。我们知道 (章 I, § 10, no. 1, 命题 2) $\theta$ 是正确的当且仅当 $C$ 在 $X \times X$ 中闭合并且（如果 $\theta'$ 表示映射 $\theta$ 被视为映射 $G \times X$ 变为 $C$) $\theta'$ 是同胚。现在假设意味着$\theta'$是双射并且它的逆是映射$(x, y) \to (\varphi(x, y), x)$。因此，当且仅当 $\varphi$ 连续时，$\theta'$ 是同胚。

### 4. 局部紧凑群正常运行

#### 命题 7 {#top-iii-s4-prop-7 .statement tag=0BL8}

*令 $G$ 为局部紧凑的群，在 Hausdorff 空间 $X$ 上连续运行。那么$G$在$X$上正确运行当且仅当对于$X$的点$x, y$的每个对，存在$x$的邻域$V_x$和邻域$V_y$ $y$使得所有$s \in G$中的集合$K$，其中$s.V_x \cap V_y \neq \emptyset$在$G$中相对紧凑。*

令$F$为将点在无穷远$\omega$与$G$邻接而获得的紧空间，令$\Gamma$为$\rho : (s, x) \to s.x$视为$F \times X \times X$的子集的图。让我们证明，如果 $\mathrm{pr}_{23}$ 到 $\Gamma$ 的限制是正确的，那么 $\Gamma$ *闭于* $F \times X \times X$。事实上，这个假设意味着$F \times \Gamma$到$F \times X \times X$的映射$u : (t, s, x, y) \to (t, x, y)$是封闭的。如果$\Gamma'$是$F \times G$中点$(s, s)$的集合，其中$s \in G$，则$\Gamma'$在$F \times G$中闭合，因为它是典范嵌入$G \to F$ (章) I, § 8, no. 1、推论 2 至命题 2)；因此交$(\Gamma' \times X \times X) \cap (F \times \Gamma)$在$F \times \Gamma$关闭，立即可以看出其$u$下的像是集合$\Gamma$视为$F \times X \times X$的子集；因此$\Gamma$在$F \times X \times X$关闭。现在，我们有$(\{\omega\} \times X \times X) \cap \Gamma = \emptyset$。因此，从 $F$ 的定义开始，对于每个点 $(x, y) \in X \times X$，$X \times X$ 中存在 $(x, y)$ 的邻域 $W$ 以及 $G$ 的紧凑子集 $K$，使得

$$
((G - K) \times W) \cap \Gamma;
$$

是空的；因为我们可以将$W$视为邻域$V_x \times V_y$，其中$V_x$和$V_y$分别是$X$、叙述中$x$和$y$的邻域“((G — K) × W) ∩ Γ = ∅”变为“如果 s ∉ K，则 s · V_x ∩ V_y = ∅”。这样我们就证明了命题中所说的条件的必要性。反之，假设满足这个条件；令A经超滤器$\mathfrak{F}$过滤为集合，并令α → (s_α, x_α)为A的映射进入G × X，使得lim_$\mathfrak{F}$ x_α = x且lim_$\mathfrak{F}$ s_α · x_α = y。假设 K、V_x 和 V_y 满足条件命题。到假设时，有集合 M ∈ $\mathfrak{F}$，如果 α ∈ M 则 x_α ∈ V_x 且 s_α · x_α ∈ V_y，因此 s_α ∈ K。这表明 α → s_α 相对于 $\mathfrak{F}$ 收敛，证明是完备的。

如果 G 是紧致的，则命题 7 的条件基本满足；因此我们检索命题 2 a)。

命题 7 特别表明，在 Hausdorff 空间 X 上连续运行的离散群 G，当且仅当对于 X 的点的每个对 (x, y)，存在 x 的邻域 V_x 时，才能在 X 上正确运行和 y 的邻域 V_y，使得点 s ∈ G 的集合，其中 s · V_x ∩ V_y ≠ ∅ 是有限的。

#### 命题 8 {#top-iii-s4-prop-8 .statement tag=0BL9}

设 G 是在 Hausdorff 空间 X 上正常运行的离散群。令 x 为 X 的点，令 K_x 为 x 的稳定子。然后：

a) 子群 K_x 是有限的，并且存在一个开集合 U ⊂ X、包含 x，在 K_x 下稳定，并且在其上由 G 定义的关系诱发的等价关系是由 K_x 定义的等价关系。

b) 典范映射 U/K_x → X/G 是 U/K_x 到 X/G 中 x 的类的开邻域的同胚。

到命题7，K_x 是有限的。对于满足所需条件的构造开集合 U，首先请注意，到命题 7 时，存在一个开集合 U_0 包含 x，并且使得 s ∈ G 的集合 K，其中 s · U_0 ∩ U_0 ≠ ∅ 是有限的。显然 K_x ⊂ K；令 s_1, ..., s_n 为 K — K_x 的元素。如果我们设 x_i = s_i · x (1 ≤ i ≤ n)，则对于每个 i，x_i ≠ x；由于 X 是 Hausdorff，因此对于每个指标 i，存在 x 的开邻域 V_i 和 s_i · x 的开邻域 V'_i，使得 V_i ∩ V'_i = ∅。设 U_i = V_i ∩ s_i^{-1} · V'_i；则 U_i 显然开且包含 x，并且我们有 U_i ∩ s_i · U_i ⊂ V_i ∩ V'_i = ∅。设 U' = U_0 ∩ U_1 ∩ ... ∩ U_n； U' 是开集，包含 x，且对于 s ∉ K_x，U' ∩ s · U' = ∅。将 U = ⋂_{t ∈ K_x} t · U' 我们最终得到一个开集合，在 K_x、包含 x 下稳定，并且使得 U ∩ s · U = ∅ 对于 s ∉ K_x：U 是所需的开集合。

事实上，典范映射 U/K_x → X/G 是 U/K_x 到 X/G 中的开集合的同胚，从章 I, § 5, no. 2、命题 4 得出，因为 U 是开路且 G 定义的等价关系是开路（§ 2, no. 4，引理2）。

#### 推论 {#top-iii-s4-n4-cor-1 .statement tag=0BLA}

*如果我们假设在加法中$K_x = \{ e \}$，则点$x$有一个开邻域$U$，使得典范映射$X \to X/G$的限制到$U$是$U$到开的同胚子集共 $X/G$。*

### 5. 群在局部紧凑的空间上连续运行

#### 命题 9 {#top-iii-s4-prop-9 .statement tag=0BLB}

*令$G$为拓扑群，在局部紧凑的空间$X$上连续运行。那么如果 $X/G$ 是 Hausdorff，那么它是局部紧的。*

由于$G$定义的$X$上的等价关系是开路（$§ 2$、no. 4、引理 2），命题由章、I、$§ 10$、no. 4、命题得出10.

#### 命题 10 {#top-iii-s4-prop-10 .statement tag=0BLC}

*令$G$为在局部紧凑空间$X$上连续运行的拓扑群，并假设$X/G$为Hausdorff。设$\varphi$是$X$到$X/G$的典范映射。那么如果 $K'$ 是 $X/G$ 的任何紧致子集，则存在 $X$ 的紧致子集 $K$，使得 $\varphi(K) = K'$。*

由于$G$定义的等价关系是开路（$§ 2$、no. 4、引理2），命题是章I、$§ 10$、no. 4的命题10的特例。

#### 命题 11 {#top-iii-s4-prop-11 .statement tag=0BLD}

*令$G$为在非空空间$X$上正常运行的豪斯多夫拓扑群。如果 $X$ 是紧致的（或局部紧致），那么 $G$ 和 $X/G$ 也是紧致的。*

由假设、$G \times X$的映射$\theta : (s, x) \to (x, s.x)$变为$X \times X$为宜；如果 $X \times X$ 是紧致的（或局部紧致），则章 I、$§ 10$、no. 4 的推论到命题 9 表明 $G \times X$ 也是紧致的（或局部紧致），因此 $G$ 也是紧致的，因为$X \neq \emptyset$。 由于 $X/G$ 是 Hausdorff (no. 2, 命题 3)，$X$ 的紧致性（或局部紧致性）意味着 $X/G$ 的紧致性（或局部紧致性）[章 I, $§ 10$, no. 4, 命题 8（分别为命题 9）]（参见$§ 2$、习题 29）。

现在我们给出判据，它允许我们断言豪斯多夫拓扑群$G$在局部紧致空间$X$上正确运行。对于子集 $K, L$ $X$ 中的每个对，我们用所有 $s \in G$ 中的 $P(K, L)$ 集合表示，使得$s.K \cap L \neq \emptyset$。

#### 定理 1 {#top-iii-s4-thm-1 .statement tag=0BLE}

*令$G$为豪斯多夫拓扑群，它在拓扑空间$X$上连续运行。令$K$为$X$的紧子集，并令$L$为$X$的闭子集。然后：
a) 集合 $P(K, L)$ $G$ 关闭。*

b) *如果 G 在 X 上正确运行并且 L 是紧的，则 P(K, L) 是紧的。*

c) *相反，如果 X 是局部紧致的，并且对于 X 的紧致子集的每个对 K、L，P(K, L) 在 G 中相对紧致 [因此通过 a) 紧致]；那么 G 在 X 上正确运行（如果 X 不为空，则 G 被命题 11 局部压缩）。*

$G \times K$的映射$(s, x) \to s.x$到$X$是连续的，因此在这个映射下的$L$的逆像$L'$是封闭的。由于$K$是紧的，所以投影$\operatorname{pr}_1 : G \times K \to G$是正确的（章I, § 10, no. 2，定理1中的推论5），因此$\operatorname{pr}_1$下的$L'$的像是闭的。这个像是$P(K, L)$，因此a)得证。

证明 b)：$X$ 是 Hausdorff (no. 2, 命题 3)。由$G \times X$的假设映射$\theta : (s, x) \to (x, s.x)$变为$X \times X$为宜；因为 $K \times L$ 是紧的，所以 $\overline{\theta}(K \times L)$ 也是紧的，因为 $X$ 是 Hausdorff (章 I, § 10, no. 2, 命题 6)。因此，$\overline{\theta}(K \times L)$到$G$的投影$P(K, L)$是紧集。

证明 c)：由于 $K \times L$ 在 $X \times X$ 中闭合，因此 $\overline{\theta}(K \times L)$ 在 $P(K, L) \times K$ 中闭合，因此在 c) 的假设下是紧的。由于$X \times X$的每个紧凑子集都包含在形式$K \times L$的紧凑子集中，因此$\theta$下的$X \times X$的任何紧凑子集的逆像都是紧凑的，并且因为$X \times X$ 是局部紧致的，这表明 $\theta$ 是正确的（章 I, § 10, no. 3, 命题 7）[参见章 IV, § 1, 习题 4c)]。

#### 注 {#top-iii-s4-n5-rem-1 .statement tag=0BLF}

显然，我们有 $P(K, L) \subset P(K \cup L, K \cup L)$；因此，为了使$G$在局部紧致空间$X$上正确运行，对于$X$的每个紧致子集$K$，集合$P(K, K)$在$G$中相对紧致就足够了。特别是，*离散* 群 $G$ 在局部紧致空间 $X$ 上正确运行当且仅当，对于 $X$ 的每个紧致子集 $K$，集合 $s \in G$ 使得$s.K \cap K \neq \emptyset$ 是*有限*。

#### 例 {#top-iii-s4-n5-exa-1 .statement tag=0BLG}

令$X$为复解析流形，解析同构于$\mathbf{C}^n$的有界开子集，并令$G$为$X$的解析自同构的群。紧致收敛的拓扑与$G$的群结构兼容，可以证明$G$在$X$上可以正常运行。特别是，$G$的每个离散子群都可以在$X$上正常运行。

以$X$为例，它是上半平面$\mathscr{J}(z) > 0$，它在解析上与$\mathbf{C}$中的开圆盘同构。那么$G$是所有变换$z \to (az + b)/(cz + d)$的群，其中$a, b, c, d$是实数，$ad - bc \neq 0$。 $G$的子群$H$，由所有此类变换组成，其中$a, b, c, d$是整数，$ad - bc = 1$是$G$的离散子群，称为*模群*。综上所述，在上半平面$\mathscr{J}(z) > 0$上运行正常。*

#### 命题 12 {#top-iii-s4-prop-12 .statement tag=0BLH}

令 G 为 Hausdorff 拓扑群，它在拓扑空间 X 上连续运行。令K为X的紧致子集，并令$\rho_K$为$G \times K$的映射$(s, x) \to s.x$到X。然后：

a) 如果G在X上正确运行，则$\rho_K$是正确的。

b) 如果 X 是局部紧致的，并且 $\rho_K$ 对于 X 的每个紧致子集 K 是合适的，则 G 在 X 上正确运行。

映射 $\rho_K$ 因式分解为 $G \times K \xrightarrow{\theta_K} K \times X \xrightarrow{\mathrm{pr}_2} X$，其中 $\theta_K$ 是 $G \times X$ 的映射 $\theta : (s, x) \to (x, s.x)$ 的限制到 $G \times K$ 到 $X \times X$。由于 $\theta^{-1}(K \times X) = G \times K$，如果 $\theta$ 是真值，则 $\theta_K$ 是真值（章 I, § 10, no. 1，命题 3）。另一方面，由于 K 是紧的，投影 $\mathrm{pr}_2 : K \times X \to X$ 是真值（章 I, § 10, no. 2、定理 1、推论 5），因此 $\rho_K$ 是真值（同上、no. 1、命题 5）。

相反，假设 $\rho_K$ 对于每个紧致 $K \subset X$ 都是合适的。如果L是X的紧致子集，则$\rho_K^{-1}(L)$是$G \times K$的紧致子集，其投影到G中是$P(K, L)$；因此 $P(K, L)$ 是紧的。因此，如果 X 是局部紧致的，则从定理 1 可以得出 G 在 X 上正确运行。

#### 推论 {#top-iii-s4-n5-cor-1 .statement tag=0BLI}

令 G 为在拓扑空间 X 上正确运行的豪斯多夫拓扑群。如果 K 是 X 的任何紧致子集，并且如果 F 是 G 的任何闭子集，则 F.K 在 X 中是闭的。

这是从命题 12 和章 I, § 10, no. 1、命题 1 得出的。

### 6. 局部紧致齐次空间

#### 命题 13 {#top-iii-s4-prop-13 .statement tag=0BLJ}

设G是局部紧致群，并令H是G的闭子群。则齐次空间$G/H$是局部紧致和拟紧致。

由于 $G/H$ 是 Hausdorff (§ 2, no. 5, 命题 13)，因此它是局部紧致的，通过 no. 5 的命题 9 应用于在右侧 G 上运算的 H。因此，仍然需要证明 $G/H$ 是仿紧的。令V为G中e的对称紧邻域，令$G_0 = V^\infty$为由V生成的G的子群。 $G_0$ 已开通（§ 2, no. 1、推论至命题 4）并在 $G/H$（§ 2, no. 5、命题 12）上持续运行。如果我们可以证明轨道$G_0.z \ (z \in G/H)$中的每一个都是$G/H$的开子集和紧集的可数并，那么$G/H$是不同轨道$G_0.z$的*拓扑和*因此是仿紧的 (章 I, , no. 10, 定理 5)。 $G_0 . z$ 在 $G/H$ 中开路是因为 $G_0$ 在 $G$ 中开路并且等价关系 $x^{-1} y \in H$ 是开路（$\S 2$、no. 4、引理 2）。另一方面，$G_0 z$是集合$V^n . z$($n \geq 1$)的并，由于$V^n$在$G$中是紧的，并且$G/H$是Hausdorff，所以$V^n . z$是紧的。这样就完成了证明

#### 命题 14 {#top-iii-s4-prop-14 .statement tag=0BLK}

*在局部紧凑群$G$中，恒等式分量$C$是$G$的开子群的交。*

$C$ 是$G$ ($§ 2$, no. 2, 命题 7) 的闭法线子群，因此$G/C$ 是局部紧致 (命题 13) 且完全不连通 (章) I、$§ 11$、no. 5、命题 9)。由于$G/C$的开子群的逆像，在$G$的典范映射到$G/C$上，是$G$包含于$C$的开子群，我们看到我们可以限制自己到证明命题群 $G/C$。在其他字中，我们可以假设$G$完全断开。然后我们知道（章II，$§ 4$，no. 4，推论到命题6）$e$包含的每个紧凑邻域$V$ 邻域 $U$ 或 $e$ 既可开也可闭。由于$U$是紧的并且$B = C U$是闭的，因此$e$存在对称开邻域$W$，使得$W \subset U$和$UW \cap BW = \varnothing$（$§ 3$、no. 1和章） II、$§ 4$、no. 3、命题 4) 和 *更不必说* $UW \subset U$。到 $n$ 上的归纳时，每整数 $n > 0$ 就有 $W^n \subset U$。因此，由$W$生成的子群$W^\infty = \bigcup_{n > 0} W^n$包含在$U$中；但$W^\infty$在$G$（$§ 2$、no. 1、推论至命题4）开放。这样就完成了证明。

我们还证明了：

#### 推论 1 {#top-iii-s4-prop-14-cor-1 .statement tag=0BLL}

*如果$G$是完全断开的局部紧凑群，则$G$包含中$e$的每个邻域是$G$的开子群。*

#### 推论 2 {#top-iii-s4-prop-14-cor-2 .statement tag=0BLM}

*如果由单位元素的每个邻域生成，则局部紧凑群是连通的。*

#### 推论 3 {#top-iii-s4-prop-14-cor-3 .statement tag=0BLN}

*令$G$为局部紧致群，令$H$为$G$的闭子群，令$\varphi$为$G$到$G/H$的典范映射。那么$G/H$的分量就是$G$的分量的$\varphi$下像的闭包。*

令$C$为$G$的恒等式分量。 $G$中的分量是集合$sC$，其中$s \in G$（$§ 2$，no. 2，命题7）； $\varphi(sC)$ 是明显相连的，因此 $\varphi(sC)$ 也是如此（章 I, $§ 11$, no. 1, 命题 1）。但是$\varphi(sC) = \varphi(sCH)$，并且由于$sCH$相对于$H$定义的等价关系是饱和的，并且由于这个等价关系是开放的（§ 2, no. 4，引理2），所以我们有$\overline{\varphi(sCH)} = \varphi(\overline{sCH}) = \varphi(s.\overline{CH})$（章I, § 5, no. 3， 命题7)。

把$L = CH$。 $L$是$G$的闭子群，其中包含$C$和$H$；因此，要证明集合$\varphi(s.L) = s.\varphi(L)$是$G/H$的分量，只需证明$G/H$的商空间乘以等价关系，其中类是集合$s.\varphi(L)$完全断开连接。现在这个商空间同态于齐次空间 $G/L$ (章 I, § 3, no. 4, 命题 7)；因此，我们被简化为证明，当 $C \subset H$ 时，$G/H$ *完全断开连接*。由于$G/H$可以与$(G/C)/(H/C)$（§ 2, no. 7，命题22）等同，我们甚至可以假设$G$本身是完全断开的。 $G/H$ 包含邻域形式 $\varphi(V)$ 中的每个 $\varphi(e)$ 邻域，其中 $V$ 是 $G$ 中$e$ 的邻域，因此(推论 1) 形式 $\varphi(K)$ 的包含邻域，其中 $K$ 是 $G$ 的*紧凑开* 子群。因此，$\varphi(K)$在$G/H$中既开又闭，这表明$G/H$中$\varphi(e)$的分量仅由$\varphi(e)$组成。通过翻译，对于$G/H$的每一个点的分量也是如此，推论得证。

### 习题{#top-iii-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
