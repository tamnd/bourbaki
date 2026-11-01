---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 10
section_title: Proper mappings
lang: zh
source: top-i-iv
book_pages: 97-107, 150-155
pdf_pages: 0103-0113, 0156-0161
extraction: ocr
subsections:
    - "no": 1
      title: PROPER MAPPINGS
      page: 97
      pdf_page: 103
    - "no": 2
      title: CHARACTERIZATION OF PROPER MAPPINGS BY COMPACTNESS PROPERTIES
      page: 101
      pdf_page: 107
    - "no": 3
      title: PROPER MAPPINGS INTO LOCALLY COMPACT SPACES
      page: 104
      pdf_page: 110
    - "no": 4
      title: QUOTIENT SPACES OF COMPACT SPACES AND LOCALLY COMPACT SPACES
      page: 105
      pdf_page: 111
statements: 30
exercises: 21
content_sha256: 863ef4215a2aaca7e186fb2abd7889016f9d913bb214d7384f5ec723cba25a12
translated_from: content/en/top/I/10_s10_proper_mappings.md
translation_method: google
source_content_sha256: 5a1cc21b1eb39135e8b2b41344fcaf3ba40ecd043ec0192b77c8b672b5efb1a1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 38d7abd8b6c0d7fc9123fff3a7041e5efc6ee793db05d5644393397491b22765
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 10. 正确映射

*在这个截面中，我们用集合$X$的$\iota_X$恒等映射本身来表示。*

### 1. 正确映射

如果$f : X \to Y$和$f' : X' \to Y'$是两个*连续闭*映射，乘积$f \times f' : X \times X' \to Y \times Y'$不一定是闭映射，即使$f$是形式$\iota_X$。

#### 例 {#top-i-s10-n1-exa-1 .statement tag=0BA1}

Hausdorff 空间中的每个常数映射都是闭的。但它$f$是常数映射$Q \to 0$，那么$f \times \iota_Q$就是$Q^2$入$Q^2$的映射$(x, y) \to (0, y)$，所以是第二个投影，不是闭的（§ 4, no. 2，注） 1）。

#### 定义 1 {#top-i-s10-def-1 .statement tag=0BA2}

*设$f$是拓扑空间$X$到拓扑空间$Y$的映射。对于每个拓扑空间 $Z$，如果 $f$ 是连续的且映射 $f \times \iota_Z : X \times Z \to Y \times Z$ 是闭集，则 $f$ 被认为是正确的。*

我们将在no. 2和3中给出适当的映射的其他刻画。

如果在定义 1 中，我们将空间 $Z$ 组成单个点，我们会看到：

#### 命题 1 {#top-i-s10-prop-1 .statement tag=0BA3}

*每个正确的映射都是关闭的。*

#### 命题 2 {#top-i-s10-prop-2 .statement tag=0BA4}

*令$f : X \to Y$为连续的单射。那么下面三个叙述是等价的：*
a) $f$ 是正确的。
b) $f$ 关闭。
c) $f$ 是 $X$ 到 $Y$ 的闭子集的同胚。

我们刚刚看到a) 蕴涵b)。由于等价关系$f(x) = f(x')$是等式关系，$X$相对于这个关系的商空间可以用$X$来识别；因此，b) 由于 § 5, no. 2、命题 3 隐含了 c)。最后，如果 c) 满足，则 $f \times \iota_Z$ 是 $X \times Z$ 同胚到 $Y \times Z$ 的闭子空间，因此是闭映射；因此c)意味着a)。

#### 命题 3 {#top-i-s10-prop-3 .statement tag=0BA5}

*令$f : X \to Y$为连续的映射。如果$T$是$Y$中的任何子集，则让$f_T$表示映射$\overline{f}^{-1}(T) \to T$，它与$\overline{f}^{-1}(T)$上的$f$一致。*
a) *如果 $f$ 合适，则 $f_T$ 也合适。*
b) *设$(T(i))_{i \in I}$是$Y$的子集族，其内部覆盖$Y$，或者是$Y$的局部有限封闭覆盖；那么如果映射 $f_{T(i)}$ 中的每一个都是正确的，那么 $f$ 也是正确的。*

设$Z$为拓扑空间。如果$T$是$Y$中的任意子集，我们有
$$
f_T \times \iota_Z = (f \times \iota_Z)_{T \times Z};
$$
如果$f$成立，则$f \times \iota_Z$是闭集，因此$(f \times \iota_Z)_{T \times Z}$也是闭集[§ 5, no. 1，命题 2 a)]，从而 a)得证。如果现在$(T(i))_{i \in I}$满足b)中所述的两个条件之一，则$Y \times Z$的覆盖$(T(i) \times Z)_{i \in I}$具有相同的性质；如果 $f_{T(i)}$ 正确则映射
$$
(f \times \iota_Z)_{T(i) \times Z}
$$
关闭，从而 $f \times \iota_Z$ 关闭 [§ 5, no. 1, 命题 2 b)]。这样就完成了证明。

#### 命题 4 {#top-i-s10-prop-4 .statement tag=0BA6}

*令$I$为有限集合，对于每个$i \in I$，令$f_i : X_i \to Y_i$为连续映射。令 $X = \prod_{i \in I} X_i, \ Y = \prod_{i \in I} Y_i,$ 并令 $f : X \to Y$* 为乘积映射 $(x_i) \to (f_i(x_i))$。然后：
a) *如果 $f_i$ 中的每一个都是正确的，那么 $f$ 都是正确的。*
b) *如果$f$是正确的并且$X_i$非空，那么每个$f_i$都是正确的。*

（我们将在no. 2，定理 1，推论3中看到，这个命题扩展到无限乘积。）

到归纳就足以考虑$I = \{1, 2\}$的情况了。
a) 假设$f_1, f_2$是适当的，并令$Z$是拓扑空间； $f_1 \times f_2 \times \iota_Z$ 是 $\iota_{Y_1} \times f_2 \times \iota_Z$ 中的合成且
$$
f_1 \times \iota_{X_2} \times \iota_Z;
$$
这两个映射被假设封闭，因此$f_1 \times f_2 \times \iota_Z$[§ 5, no. 1，命题 1 a)]，从而$f_1 \times f_2$是正确的。

b) 现在假设 $f$ 是正确的。令$F$为$X_2 \times Z$的闭子集，并令$G$为$F$中$Y_2 \times Z$中映射$f_2 \times \iota_Z$的像。那么$f_1 \times f_2 \times \iota_Z$下的$Y_1 \times Y_2 \times Z$中的$X_1 \times F$的像就是$f_1(X_1) \times G$。 假设，$Y_1 \times Y_2 \times Z$关闭；如果$X_1 \neq \emptyset$，则$f_1(X_1)$不为空，这意味着$G$在$Y_2 \times Z$中闭合（§ 4, no. 3，命题7的推论）；因此 $f_2$ 是正确的。同样，如果 $X_2 \neq \emptyset$ 则 $f_1$ 是正确的。

#### 命题 5 {#top-i-s10-prop-5 .statement tag=0BA7}

*令$f : X \to X'$和$g : X' \to X''$为两个连续的映射。*
a) *如果$f$和$g$是正确的，那么$g \circ f$是正确的。*
b) *如果 $g \circ f$ 是真且 $f$ 是满射，则 $g$ 是真。*
c) *如果 $g \circ f$ 是正确的并且 $g$ 是单射的，那么 $f$ 是正确的。*
d) *如果 $g \circ f$ 是正确的且 $X'$ 是 Hausdorff，则 $f$ 是正确的。*

设$Z$为拓扑空间。我们有
$$
(g \circ f) \times \iota_Z = (g \times \iota_Z) \circ (f \times \iota_Z);
$$
如果$f$和$g$是正确的，则$f \times \iota_Z$和$g \times \iota_Z$是闭的；因此 [§ 5, no. 1, 命题 1 a)] $(g \circ f) \times \iota_Z$ 是闭合的；这证明了a）。 b) 的证明 [分别。 c)] 沿着同样的路线运行，使用部分 b) [resp. 命题 1 of § 5, no. 1，并指出如果 $f$ 是满射的（或者如果 $g$ 是单射的），则 $f \times \iota_Z$ 是满射的（或者 $g \times \iota_Z$ 是单射的）。最后，为了证明 d)，考虑交换律图表

$$
\begin{array}{ccc}
X & \overset{\varphi}{\to} & X \times X' \\
f \downarrow & & \downarrow (g \circ f) \times \iota_{X'} \\
X' & \underset{\psi}{\to} & X'' \times X'
\end{array}
$$

其中 $\varphi(x) = (x, f(x))$ 和 $\psi(x') = (g(x'), x')$。 映射 $\varphi$（分别为 $\psi$）是 $X$（分别为 $X'$）到 $f$ 图（分别为 $g$ 图的反射）的同胚 (§ 4, no. 1, 命题 1,推论2）。此外，由于$X'$是Hausdorff，$f$的图$\varphi(X)$在$X \times X'$中是封闭的（§ 8, no. 1，命题2，推论2）。因此 (命题 2) $\varphi$ 是正确的；另一方面，命题 4 表明$(g \circ f) \times i_{X'}$ 是正确的。由a)上式和图表(1)中的交换律，$\psi \circ f$为宜；但 $\psi$ 是单射的，因此 $f$ 由上面的 c) 是正确的。

#### 注 {#top-i-s10-n1-rem-1 .statement tag=0BA8}

如果 $X'$ 不是 Hausdorff，则可能发生 $g \circ f$ 是正确的而 $f$ 不是；对于例，取$X$和$X''$由一个点组成，$X'$由两个点组成，其中拓扑最粗。

#### 推论 1 {#top-i-s10-prop-5-cor-1 .statement tag=0BA9}

*如果$f : X \to Y$是真映射，则$f$的限制到$X$的闭子集$F$是$F$到$Y$的真映射。*

对于这个限制是合成$f \circ j$，其中$j : F \to X$是典范嵌入，这是正确的命题2。

#### 推论 2 {#top-i-s10-prop-5-cor-2 .statement tag=0BAA}

*令$f : X \to Y$为真映射，其中$X$为Hausdorff。那么 $Y$ 的子空间 $f(X)$ 就是 Hausdorff。*

由于命题 5 c)，我们只需要考虑$f(X) = Y$的情况。那么$Y \times Y$的对角线在$X$的对角线的$f \times f$之下是像，是闭的（§ 8, no. 1，命题1）； $f \times f$ 是正确的（命题 4）；因此$Y \times Y$的对角线是闭的（命题1），因此$Y$是豪斯多夫（§ 8, no. 1，命题1）。

#### 推论 3 {#top-i-s10-prop-5-cor-3 .statement tag=0BAB}

*令$I$为有限集合，对于每个$i \in I$，令$f_i : X \to Y_i$为真映射。如果 $X$ 是 Hausdorff，则 $X$ 的映射 $x \mapsto (f_i(x))$ 到 $\prod_{i \in I} Y_i$ 是正确的。*

这个映射是$X^I$的乘积映射$(x_i) \mapsto (f_i(x_i))$到$\prod_i Y_i$的合成和$X$的对角线映射到$X^I$；因为后者是正确的（通过命题 2 和 § 8, no. 1，命题 1），结论由命题 4 和命题 5 a) 得出。

#### 推论 4 {#top-i-s10-prop-5-cor-4 .statement tag=0BAC}

*令$X$和$Y$为两个拓扑空间，$f : X \to Y$在$X$上连续的映射，$R$等价关系$f(x) = f(y)$，并且*
$$
X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y
$$
* $f$ 的规范分解。* *那么，要使 $f$ 正确，$p$ 正确，$h$ 同胚，$f(X)$ $Y$ 的闭子集是必要且充分的。*

根据命题 5 a) 和命题 2，条件是充分的。反之，如果$f$ 是适当的，则$f$ 是闭的；因此 $f(X)$ 在 $Y$ 中闭合，$h$ 是同胚 ($§ 5$, no. 2, 命题 3)； $h \circ p$ 也适用于命题 5 c)；因此 $p = h^{-1} \circ (h \circ p)$ 是命题 5 a) 的真值。

### 2. 按紧性性质计算的刻画的适当映射

在这个小节中，我们将用单个点的$P$空间由……组成来表示，其具有唯一的拓扑。

#### 引理 1 {#top-i-s10-lem-1 .statement tag=0BAD}

*设$X$为拓扑空间，使得常数映射$X \to P$是正确的。那么 $X$ 是拟紧的。*

（稍后我们将看到（定理 1，推论 1），这个性质表征了准紧凑空间。）

我们可以将自己限制在$X$不为空的情况。令$\mathfrak{F}$为$X$上的过滤器，$X' = X \cup \{ \omega \}$为与$\mathfrak{F}$（$§ 6$、no. 5、例）关联的拓扑空间。令$\Delta$为$x \in X$中所有$(x, x)$的$X \times X'$由……组成的子集，并令$F = \overline{\Delta}$为$X \times X'$中$\Delta$的闭包。鉴于$X$假设，投影$X \times X' \to X'$下$F$的像已于$X'$关闭；这个像包含$X$因此包含$\omega$，它位于$X$的闭包中；在其他字中，有点$x \in X$使得$(x, \omega) \in F$。通过$X \times X'$的拓扑的定义，这意味着，对于$X$中$x$的每个邻域$V$和每个$M \in \mathfrak{F}$，我们有$(V \times M) \cap \Delta \neq \emptyset$，即$V \cap M \neq \emptyset$，因此$x$是滤波器$\mathfrak{F}$的簇点，因此$X$是拟紧的。

Q.E.D.

#### 定理 1 {#top-i-s10-thm-1 .statement tag=0BAE}

*令$f : X \to Y$为连续的映射。那么下面四个叙述是等价的：

a) $f$ 是正确的。
b) $f$ 是闭集，$\overline{f}^{-1}(y)$ 对于每个 $y \in Y$ 是拟紧的。
c) *如果$\mathfrak{F}$是$X$上的过滤器，并且如果$y \in Y$是$f(\mathfrak{F})$的集群点，则存在$\mathfrak{F}$的集群点$x$，使得$f(x) = y$。*
d) *如果$\mathfrak{U}$是$X$上的超滤器，并且如果$y \in Y$是超滤器基$f(\mathfrak{U})$的极限点，则有极限点$x$ $\mathfrak{U}$ 这样 $f(x) = y$.*

a) $\Longrightarrow$ b)：如果 $f$ 是正确的，则 $f$ 是闭合的 (no. 1, 命题 1)，并且对于每个 $y \in Y$ 映射 $f_{|y|} : \overline{f}^{-1}(y) \to \{ y \}$ 是正确的 [no. 1, 命题 3a)]。到引理 1，这意味着$\overline{f}^{-1}(y)$ 是拟紧的。

b) $\Longrightarrow$ c)：假设 $\mathfrak{F}$ 和 $y$ 满足 c) 的假设。令$\mathfrak{B}$为$X$上的过滤器基，由$\mathfrak{F}$的集合闭包形成。由于 $f$ 是封闭的，因此每个 $M \in \mathfrak{F}$ 都有 $f(\overline{M}) = f(M)$（§ 5, no. 4，命题 9）。这表明集合$\overline{M} \cap \overline{f}^{-1}(y)$对于所有$M \in \mathfrak{F}$都是非空的，因此形式是$\overline{f}^{-1}(y)$上的过滤器基，其元素对$\overline{f}^{-1}(y)$的子集是封闭的。由于$\overline{f}^{-1}(y)$是拟紧的，因此存在点$x \in \overline{f}^{-1}(y)$，其中属于对所有集合$M$，因为$M$贯穿$\mathfrak{F}$。因此$f(x) = y$和$x$是$\mathfrak{F}$的集群点。

c) $\Longrightarrow$ d)：微不足道。

d) $\Longrightarrow$ a)：我们首先证明，如果满足 d)，则 $f$ 是闭映射。令$A$为$X$的非空闭子集，令$\mathfrak{F}$为$X$的子集的过滤器，其中包含$A$。那么$A$就是$\mathfrak{F}$的簇点的集合。令$B$为$Y$上过滤器基$f(\mathfrak{F})$的簇点的集合； $B$关闭，明确包含$f(A)$；我们将证明$B = f(A)$。设$y \in B$且$\mathfrak{B}$为$Y$中$y$的邻域滤波器；然后到假设，$\mathfrak{W} = \overline{f}^{-1}(\mathfrak{B})$的每一个集合满足$\mathfrak{F}$的每一个集合；因此$\mathfrak{W}$是$X$上的过滤器基，$X$上有一个超滤器$U$，它比$\mathfrak{F}$和基为$\mathfrak{W}$的过滤器更细（§ 6, no. 2， 命题 1，推论 1 和 no. 4，定理 1)。 基为$f(U)$的超滤器是更细大于$\mathfrak{B}$，因此收敛于$y$。凭借d)，存在点$x \in X$，使得$f(x) = y$和$U$收敛于$x$；由于 $U$ 比 $\mathfrak{F}$ 更细，$x$ 是 $\mathfrak{F}$ 的集群点；因此$x \in A$。这表明 $B = f(A)$ 因而 $f$ 是封闭的。

为了完成证明，我们必须证明$f \times \iota_Z$对于每个拓扑空间$Z$都是封闭的。从已经证明的情况来看，只要$f$满足条件d)，那么$f \times \iota_Z$也满足。这是以下一般引理中的推论：

#### 引理 2 {#top-i-s10-lem-2 .statement tag=0BAF}

*如果* $(f_i)_{i \in I}$ *是一系列连续的映射* $f_i : X_i \to Y_i$，*每个都满足定理 1 的条件 d)*，*则乘积映射*
$$
f : (x_i) \to (f_i(x_i))
$$
*也满足*d)。

令$U$为$X = \prod_i X_i$上的超滤器，并令$y = (y_i)$为$Y = \prod_i Y_i$的点，使得$f(U)$收敛于$y$。这意味着每个超滤器基$\operatorname{pr}_i(f(U)) = f_i(\operatorname{pr}_i(U))$收敛到$y_i$（§ 7, no. 6，命题10，推论1）。凭借条件 d)，对于每个$i \in I$，都存在$x_i \in X_i$，使得$f_i(x_i) = y_i$和$\operatorname{pr}_i(U)$收敛于$x_i$；但随后$U$收敛到$x = (x_i)$（*loc.cit.*），我们有$f(x) = y$。这样就完成了引理 2 的证明，从而完成了定理 1。

#### 推论 1 {#top-i-s10-lem-2-cor-1 .statement tag=0BAG}

*拓扑空间* $X$ *是准紧当且仅当映射* $X \to P$ *是适当的*。

将a) $\iff$ b) 应用于$X \to P$。

#### 推论 2 {#top-i-s10-lem-2-cor-2 .statement tag=0BAH}

*准紧凑空间* $X$ *的每个连续映射* $f$ *到 Hausdorff 空间* $Y$ *都是合适的*。

根据推论 1，合成 $X \xrightarrow{f} Y \to P$ 是正确的；因此 $f$ 是 no. 1, 命题 5 d) 的真值。或者，我们可以应用定理 1 的标准 b)，使用 § 9, no. 4、定理 2、推论 2。

#### 推论 3 {#top-i-s10-lem-2-cor-3 .statement tag=0BAI}

*如果* $(f_i)$ *是真映射的族，则乘积映射* $(x_i) \to (f_i(x_i))$ *是真*。

鉴于定理 1，这只是上面的引理 2。

如果我们将此推论应用于映射$X_i \to P$族并使用推论1，我们就有吉洪诺夫的定理（§ 9，无5，定理3）。

#### 推论 4 {#top-i-s10-lem-2-cor-4 .statement tag=0BAJ}

*让*$X$*成为豪斯多夫空间，让*$f_i : X \to Y_i$*成为正规映射的家庭。那么映射* $f : x \to (f_i(x))$ *of* $X$ *进入* $\prod_i Y_i$ *是正确的*。

证明与有限族的情况相同（no. 1，命题 5，推论 3），使用上面的推论 3 以及 $X^1$ 的对角线是闭合的事实（§ 8, no. 1，命题 1）。

#### 推论 5 {#top-i-s10-lem-2-cor-5 .statement tag=0BAK}

*如果* $X$ *是任何拟紧空间并且* $Y$ *是任何拓扑空间，则投影* $\mathrm{pr}_2 : X \times Y \to Y$ *是正确的*。

因为我们可以将认同$Y$与$P \times Y$和$\mathrm{pr}_2$与乘积或$X \to P$和$\iota_Y$进行组合，两者都是正确的映射。

#### 例 {#top-i-s10-n2-exa-1 .statement tag=0BAL}

令$X$为集合，并令$f : X \to X'$为$X$的映射到拓扑空间$X'$；将$X$与逆像拓扑在$X'$的拓扑的$f$下。那么$f$是*正确的*，因为$f$是闭合的（§ 5, no. 1，例3）并且$X'$的点的逆像是$X$的子空间，其拓扑是最粗拓扑，因此是准紧的。

#### 注 {#top-i-s10-n2-rem-1 .statement tag=0BAM}

当$Y$为*Hausdorff*时，定理1的条件d)等价于：

d') *如果* $\mathfrak{U}$ *是* $X$ *上的超滤波器，使得* $f(\mathfrak{U})$ *是收敛滤波器基，则* $\mathfrak{U}$ *收敛*。

因为如果$\mathfrak{U}$收敛于$x$且$f(\mathfrak{U})$收敛于$y$，则$Y$中极限的唯一性以及$f$的连续性表明我们必须有$y = f(x)$。同样，Y 为 Hausdorff，条件 c) of 定理 1 等价于：

c') *如果 $\mathfrak{F}$ 是 X 上的过滤器，使得 $f(\mathfrak{F})$ 具有集群点，则 $\mathfrak{F}$ 具有集群点。*

对于 c) $\Longrightarrow$ c') $\Longrightarrow$ d') $\Longrightarrow$ d) $\Longrightarrow$ c)。

另一方面，如果 Y 不是 Hausdorff，则 d') 不再隐含 d)；对于例，取X由一个点组成，Y由两个点组成，其中拓扑最粗。

#### 命题 6 {#top-i-s10-prop-6 .statement tag=0BAN}

*设$f : X \to Y$为真映射，令K为Y的拟紧子集，则$\overline{f}^{-1}(K)$为拟紧。*

由no. 1的命题3，映射$f_K : \overline{f}^{-1}(K) \to K$是正确的。 由于 $K \to P$ 是真映射（定理 1，推论 1），因此从 no. 1、命题 5 a) 可以得出合成 $\overline{f}^{-1}(K) \xrightarrow{f_K} K \to P$ 是真从而 $\overline{f}^{-1}(K)$ 是定理 1 的准紧，推论1。

### 3. 适当的映射进入局部紧凑空间

#### 命题 7 {#top-i-s10-prop-7 .statement tag=0BAO}

*设 f 是 Hausdorff 空间 X 到局部紧致空间 Y 的连续映射。则 f 是正确的当且仅当 Y 的每个紧致子集的 f 下的逆像都是紧致的。此外，如果 f 是正确的，则 X 是局部紧致的。*

如果 f 是适当的且 K 是 Y 的紧致子集，则 $\overline{f}^{-1}(K)$ 是 no. 2 的命题 6 紧致。相反，如果满足条件，则令$(\mathbf{U}_\alpha)$是Y被相对紧开的集合覆盖。那么集合$\overline{f}^{-1}(\overline{\mathbf{U}}_\alpha)$在X中紧凑，并且它们的内部覆盖X；由于 X 是 Hausdorff，这表明 X 是局部紧致的。此外，映射 $f_{\overline{\mathbf{U}}_\alpha} : \overline{f}^{-1}(\alpha \overline{\mathbf{U}}) \to \overline{\mathbf{U}}_\alpha$ 都是真值（no. 2，定理 1，推论 2），因此 f 是 no. 1 的命题 3 b) 真值。

#### 推论{#top-i-s10-n3-cor-1 .statement tag=0BAP}

*令X、X'为两个局部紧致空间，并令Y（分别为Y'）为通过在无穷大$\omega$（分别为$\omega'$）与X（分别为X'）邻接点而获得的紧致空间。 （§ 9, no. 8）。 那么连续的映射 $f : X \to X'$ 是正确的当且仅当它的扩张 $\overline{f} : Y \to Y'$ ，使得 $\overline{f}(\omega) = \omega'$ 是连续的。*

By Proposition 7, f is proper if and only if, for each compact subset K' of X', $\overline{f}^{-1}(X' - K') = X - \overline{f}^{-1}(K')$ is the complement of a compact subset of X; by the definition of the neighbourhoods of $\omega$ (resp. $\omega'$) in Y (resp. Y') this is so if and only if $\overline{f}$ is continuous at $\omega$.

### 4. 紧致空间和局部紧致空间的商空间

#### 命题 8 {#top-i-s10-prop-8 .statement tag=0BAQ}

设$X$是$X$、$C$上$R$在$X \times X$、$f$典范映射$X \to X/R$上的紧致空间、$R$等价关系。那么下面的条件是等价的：

a) $C$ 在 $X \times X$ 关闭。

b) $R$ 闭合。

c) $f$ 是正确的。

d) $X/R$ 是豪斯多夫。

此外，如果满足这些条件，则$X/R$是紧凑的。

当且仅当$f$闭时，$R$闭；因此，由于定理 1b) of no. 2，b) 隐含了 c)。 c) 意味着 d) 是 no. 1, 命题 5 的特殊情况，推论 2。d) 意味着 a) 对于任何拓扑空间 $X$ ($\S$ 8, no. 3, 命题 8)。仍有待证明 a) 蕴涵 b)。如果$F$是$X$的闭子集，则其饱和度（相对于$R$）为$\mathrm{pr}_2(C \cap (F \times X))$；通过假设，$C \cap (F \times X)$ 是紧致空间 $X \times X$ 的闭子集，因此是紧致的 ($\S$ 9, no. 3, 命题 3)；现在的结果来自$\mathrm{pr}_2$的连续性（$\S$9，no. 4，定理2，推论2）。

最后很清楚，如果$X/R$是Hausdorff，那么它是紧的（$\S$9，no. 4，定理2）。

#### 命题 9 {#top-i-s10-prop-9 .statement tag=0BAR}

设$X$为$X$、$C$上$R$在$X \times X$、$f$典范映射$X \to X/R$上的局部紧凑空间、$R$等价关系；令$X'$为在无穷大$\omega$与$X$邻接点所获得的紧空间，并令$R'$为图为$C' = C \cup \{(\omega, \omega)\}$的$X'$上的等价关系。那么下面的条件是等价的：

a) $f$ 是正确的。

b) $X$的每个紧致子集相对于$R$的饱和是紧致的。

c) $R'$ 已关闭。

d) $\mathrm{pr}_2$到$C$中的限制是合适的。

e) $R$ 是闭集，等价类相对于 $R$ 是紧致的。

此外，如果满足这些条件，则$X/R$是局部紧致的。

a) $\Longrightarrow$ b)：由于$X/R = f(X)$和$f$是适当的，$X/R$是Hausdorff（no. 1，命题 5，推论2）；因此，$X$的每个紧凑子集$K$的$f$下的像是紧凑的（$\S$9，no. 4，定理2，推论1）。

$K$相对于$R$的饱和度为$\overline{f}^{-1}(f(K))$，因此由no. 2、命题 6 压缩。

b) $\Longrightarrow$ c) : 如果 $F'$ 在 $X'$ 内闭，且不存在包含 $\omega$，则 $F'$ 是 $X$ 的紧凑子集；因此，它相对于$R'$的饱和度与它相对于$R$的饱和度相同，是紧凑的并且*更不必说*在$X'$封闭。如果$\omega \in F'$并且如果$F = F' \cap X = F' - \{ \omega \}$，则$F'$相对于$R'$的饱和度是$\{ \omega \}$的并，以及$F$相对于$R$的饱和度$H$；因此，足以证明 $H$ 在 $X$ 中是*封闭*的（即 $R$ 是一个*封闭* 关系）。为此，只要证明如果$K$是$X$的任何紧致子集，则$H \cap K$是紧致的（$§ 9$，no. 7，命题11）。现在$K$相对于$R$的饱和度$L$紧致假设，$H \cap L$是$F \cap L$的饱和度，也是紧致的； *更不必说* $H \cap K = (H \cap L) \cap K$ 紧凑。

c) $\Longrightarrow$ d) : 由于 $X'$ 是正则 ($§ 9$, no. 2, 命题 1 的推论), $C'$ 在$X' \times X'$ ($§ 8$, no. 6, 命题) 中*闭* 14）因此紧凑。由此可见，$C'$是$C$的一点紧化（$§ 9$，no. 8，定理 4）。由于$pr_2 : X' \times X' \to X'$的限制到$C'$在$\omega$连续，因此结果由no. 3得出，推论到命题7。

d) $\Longrightarrow$ e) : 如果$F$是$X$的任意闭子集，则$C \cap (F \times X)$在$C$中闭，从而$F$相对于$R$的饱和度，等于$pr_2(C \cap (F \times X))$，$X$关闭（no. 1，命题1）。此外，$x \in X$ mod $R$ 的等价类同胚于 $pr_2$ 至 $C$ 的限制下的 $\{ x \}$ 逆像，因此是紧致的 [no. 2, 定理 1 b)]。

e) $\Longrightarrow$ a) : 如果 $R$ 是闭集，那么定义 $f$ 也是闭集，并且对于每个$z \in X/R$，$f^{-1}(z)$ 是等价类 mod $R$，因此是紧致的；因此 $f$ 是 no. 2 的定理 1 b) 的真值。

最后我们必须证明$X/R$是局部紧的。 $X'/R'$ 由 c) 和命题 8 压缩； 关系 $R$ 是由 $R'$ 在 $X$ 上诱发的； $X$在$X'$开，相对于$R'$饱和；因此$X/R$在典范映射$f' : X' \to X'/R'$下同胚于$X$的像$f'(X)$（$§ 3$，no. 6，命题10，推论1）。现在$f'(X)$在$X'/R'$中开，因此是$X'/R'$的局部紧凑子空间。

Q.E.D.

#### 推论{#top-i-s10-n4-cor-1 .statement tag=0BAS}

*令$X$为豪斯多夫空间，$Y$为拓扑空间，$f : X \to Y$为真映射。那么对于$X$是紧致的（或局部紧致），$f(X)$是紧致的（或局部紧致）是必要且充分的，并且$Y$是紧致的（或局部紧致）是充分的。*

f_z : X \to f(X) 是正确的 [no. 1, 命题 3 a)] 由于 no. 2 的命题 6 和 no. 3 的命题 7，X 是紧致的（或局部紧致）。最后，如果 Y 是紧致的（或局部紧致），那么 f(X) 也是紧致的，它在 Y (no. 1, 命题 1 和 , no. 7, 命题 13) 中闭合

#### 注 {#top-i-s10-n4-rem-1 .statement tag=0BAT}

如果 X 是局部紧致但不是紧致的，则 X 上的闭等价关系 R 不必是 Hausdorff (章 IX, § 4, 习题 14)；即使 R 是 Hausdorff，X/R 也不必是局部紧致的 (习题 17)。但是，我们有以下标准：

#### 命题 10 {#top-i-s10-prop-10 .statement tag=0BAU}

令X为局部紧致空间，R为X上的开豪斯多夫等价关系，令f : X \to X/R为典范映射。那么 X/R 是局部紧致的，并且如果 K' 是 X/R 的任意紧致子集，则存在 X 的紧致子集 K，使得 f(K) = K'。

第一个断言是事实中的推论，即X中的每个x都有一个紧凑邻域V，并且f(V)是f(x)的一个紧凑邻域（§ 5, no. 3，命题5和§ 9, no. 4， 定理 2，推论 1)。对于 K' 中的每个 y \in 令 V(y) 为 X 中 f^{-1}(y) 的某个点的紧致邻域，因此 f(V(y)) 是 y 的紧致邻域。 K' 中存在点 y_i \in 的有限数，使得 f(V(y_i)) 覆盖 K'。设K_1为X中的紧集$\bigcup_i V(y_i)$；我们有 K' \子集 f(K_1)；因此 K = K_1 \cap f^{-1}(K') 是紧凑的（因为它在 K_1 中是封闭的）并且 f(K) = K'。

### 习题{#top-i-s10-exercises}

参见[习题为 § 10](exercises/s10/)。
