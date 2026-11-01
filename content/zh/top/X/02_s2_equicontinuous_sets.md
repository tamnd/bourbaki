---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 2
section_title: Equicontinuous sets
lang: zh
source: top-v-x
pdf_pages: 0289-0299, 0327-0333
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION AND GENERAL CRITERIA
      page: 0
      pdf_page: 289
    - "no": 2
      title: SPECIAL CRITERIA FOR EQUICONTINUITY
      page: 0
      pdf_page: 293
    - "no": 3
      title: CLOSURE OF AN EQUICONTINUOUS SET
      page: 0
      pdf_page: 295
    - "no": 4
      title: POINTWISE CONVERGENCE AND COMPACT CONVERGENCE ON EQUICONTINUOUS SETS
      page: 0
      pdf_page: 295
    - "no": 5
      title: COMPACT SETS OF CONTINUOUS MAPPINGS
      page: 0
      pdf_page: 296
statements: 24
exercises: 20
content_sha256: 25ca74d651b2a3973b9c65b1a79d21205c3fb0fbe8c74a670f70b7f50d5df1d5
translated_from: content/en/top/X/02_s2_equicontinuous_sets.md
translation_method: google
source_content_sha256: 4982c8683a57cc9618968d6d7725ed752a8ecf12b1eb39707fd8d6b4de136d18
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 568c6ae6750cd4a6877322bd36a068a6670159ba91b95c68bb338d6fda67399a
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 2. 等连续集合

### 1. 定义和一般判据

#### 定义 1 {#top-x-s2-def-1 .statement tag=0CC0}

*设$X$为拓扑空间，$Y$为均匀空间。 $\mathscr{F}(X; Y)$ 的子集 $H$ 被认为在点 $x_0 \in X$ 处等连续，如果对于 $Y$ 的每个随行人员 $V$，$X$ 中存在 $x_0$ 的邻域 $U$，使得* $(f(x_0), f(x)) \in V$ 适用于所有 $x \in U$ 和所有 $f \in H$。如果 H 在 $X$ 的每点等连续，则称 H 是等连续的。

#### 定义 2 {#top-x-s2-def-2 .statement tag=0CC1}

令X和Y为两个一致的空间。 $\mathscr{F}(X; Y)$ 的子集 H 被认为是一致等连续的，如果对于 Y 的每个周边V，存在一个 X 的周边 U，使得每当 $(x, x') \in U$ 和 $f \in H$ 时我们都有 $(f(x), f(x')) \in V$。

如果 $f_i$ 的集合在 $x_0$ 等连续（分别等连续、一致等连续），则 X 的映射到 Y 的族 $(f_i)_{i \in I}$ 被称为在点 $x_0$ 等连续（分别等连续、一致等连续）。

显然，如果$H \subset \mathscr{F}(X; Y)$在$x_0$等连续，则每个$f \in H$在$x_0$连续；如果 H 等连续，则每个 $f \in H$ 在 X 上连续，即 $H \subset C(X; Y)$。同样，如果 H 一致等连续（X 是一致的空间），则每个 $f \in H$ 在 X 上一致连续。还清楚的是，映射的一致等连续集合是等连续的；但均匀连续映射的集合可以是等连续的，但不是均匀等连续的（参见习题 1；推论 2 至命题 1；以及 no. 2、命题 4）。

#### 例 1 {#top-x-s2-n1-exa-1 .statement tag=0CC2}

令X为拓扑空间（分别为均匀空间），Y为均匀空间。 X 到 Y 中的连续（或一致连续）映射的每个有限集合都是等连续的（或一致等连续）。

#### 例 2 {#top-x-s2-n1-exa-2 .statement tag=0CC3}

令 X、Y 为两个度量空间，d（分别为 $d'$）为 X（分别为 Y）上的度量，并令 k、$\alpha$ 为两个实数 > 0。则所有映射 $f : X \to Y$ 中的集合使得
$$
d'(f(x), f(x')) \leq k(d(x, x'))^\alpha
$$
对于点 $x, x'$ X 中的每个对 ，是一致等连续的。对于例，X到Y的子集的所有等距（章IX, § 2, no. 2）的集合一致等连续。

\* 令 H 为在区间 $I \subset \mathbf{R}$ 上定义的实值函数的集合，其在I上可微，并且对于所有$x \in I$和所有$f \in H$来说$|f'(x)| \leq k$。那么 H 是一致等连续的，因为如果 $x_1, x_2$ 是 I 中的任意两个点，我们对于每个 $f \in H$ 都有 $|f(x_1) - f(x_2)| \leq k|x_1 - x_2|$，平均为值定理。 \*

#### 例 3 {#top-x-s2-n1-exa-3 .statement tag=0CC4}

设 G 为拓扑群，令 Y 为一致空间，并令 $f : G \to Y$ 为一致连续映射 [G 被赋予左一致性 (章 III, § 3, no. 1)]。对于每个$s \in G$，令$f_s$为G到Y的映射$x \to f(sx)$。则映射$f_s (s \in G)$的集合一致等连续，因为关系$x^{-1}x' \in V$等价于$(sx)^{-1}(sx') \in V$。

#### 命题 1 {#top-x-s2-prop-1 .statement tag=0CC5}

设T为集合，令$\mathscr{S}$为T的子集集合，令Y为均匀空间，X拓扑（或均匀）空间，并令f为$T \times X$的映射 $Y$。对于每个$A \in \mathscr{S}$，令$H_A \subset \mathscr{F}(X; Y)$为所有映射$x \to f(t, x)$的集合，因为$t$贯穿$A$。那么 $X$ 到 $\mathscr{F}_\mathscr{S}(T; Y)$ 的映射 $x \to f(., x)$ 在点 $x_0 \in X$ 连续（或一致连续）当且仅当集合 $H_A$ 在 $x_0$ 等连续（或一致等连续） 对于所有$A \in \mathscr{S}$。

首先考虑$\mathscr{S} = \{ T \}$的特殊情况，即$\mathscr{F}_\mathscr{S}(T; Y) = \mathscr{F}_u(T; Y)$。对于$Y$中的每个随行人员$V$，条件$(f(., x), f(., x')) \in W(V)$表示所有$t \in T$的$(f(t, x), f(t, x')) \in V$。因此，说 $x \to f(., x)$ 在 $x_0$ 处连续（或一致连续）相当于说，对于 $Y$ 的每个随行人员 $V$，$X$ 中存在 $x_0$ 的邻域 $U$（或称说）。随行人员 $M$ $X$) 使得关系 $x \in U$ [分别。 $(x, x') \in M$] 意味着$(f(t, x), f(t, x_0)) \in V$ [分别。对于所有$t \in T$，命题是从定义1和2得出的$(f(t, x), f(t, x')) \in V$]。在一般情况下，我们必须表达，对于每个$A \in \mathscr{S}$，$X$的映射$x \to f(., x)|A$到$\mathscr{F}_u(A; Y)$是连续的$x_0$（一致连续），凭借§ 1, no. 2；根据上文所述，这相当于说，对于每个 $A \in \mathscr{S}$，$H_A$ 在 $x_0$ 处等连续（或一致等连续）。

命题 1 允许我们将定义 1 和 2 翻译成形式，有时有用，通过应用将其翻译成$T = H$ 和 $f$ 是映射 $(h, x) \to h(x)$ 的情况，将 $H \times X$ 翻译成$Y$；由于 $f(., x)$ 是 $H$ 的映射 $h \to h(x)$ 到 $Y$，我们看到：

#### 推论 1 {#top-x-s2-prop-1-cor-1 .statement tag=0CC6}

令$X$为拓扑（或均匀）空间，$Y$为均匀空间，$H$子集为$\mathscr{F}(X; Y)$。对于每个 $x \in X$，令 $\tilde{x}$ 表示 $H$ 中的映射 $h \to h(x)$ 到$Y$。那么 $H$ 在 $x_0$ 处等连续（或一致等连续）当且仅当 $X$ 的映射 $x \to \tilde{x}$ 进入一致空间 $\mathscr{F}_u(H; Y)$ 在 $x_0$ 连续（或一致连续）。

特别是，如果$X$是紧的，则$X$到$\mathscr{F}_u(H; Y)$的每个连续映射都是一致连续的（章II, § 4, no. 1，定理2）。因此：

#### 推论 2 {#top-x-s2-prop-1-cor-2 .statement tag=0CC7}

令$X$为紧凑空间，$Y$为均匀空间。那么 $\mathscr{F}(X; Y)$ 的每个等连续子集都是一致等连续的。

现在假设我们有集合$T$，拓扑空间$X$，均匀空间$Y$和映射$f : T \times X \to Y$。让$\tilde{f}$表示$X$的映射$x \to f(., x)$到$\mathscr{F}_u(T; Y)$，并让我们考虑$T \times \mathscr{F}_u(T; Y)$的典范映射$\theta : (t, g) \to g(t)$到$Y$。很明显图表

$$
\begin{array}{ccc}
T \times X & \xrightarrow{f} & Y \\
\downarrow_{\iota_T \times \tilde{f}} & & \uparrow \theta \\
T \times \mathscr{F}_u(T; Y)
\end{array}
$$

（其中 $i_T$ 是 T 的恒等映射）是可交换的。现在假设 T 被赋予拓扑，并且对于每个 $x \in X$，映射 $f(., x) : t \to f(t., x)$ 是连续的；然后我们可以在上面的图表中通过$\mathscr{C}_u(T; Y)$来替换$\mathscr{F}_u(T; Y)$。但我们知道$\theta$是从§ 1, no. 6、命题9连续而来；因此，如果 $\tilde{f}$ 是连续的，则$f$ 是连续的。由于$\tilde{f}$的连续性可以借助命题1来表达，我们得到以下结果：

#### 推论 3 {#top-x-s2-prop-1-cor-3 .statement tag=0CC8}

*设T，X为拓扑空间，设Y为均匀空间，设f为T × X到Y的映射。则f是连续的，前提是满足以下条件：*

1) *对于每个$x \in X$，部分映射$t \to f(t, x)$是连续的。*

2) *当 t 贯穿 T 时，映射 $x \to f(t, x)$ 形式 $\mathscr{F}(X; Y)$ 的等连续子集。*

具体地，取T为$\mathscr{F}(X; Y)$的子集H，f为$H \times X$的典范映射$(h, x) \to h(x)$代入Y；推论3的条件1)意味着H比逐点收敛具有拓扑更细，条件2)意味着H是等连续的。因此：

#### 推论 4 {#top-x-s2-prop-1-cor-4 .statement tag=0CC9}

*设X为拓扑空间，Y为均匀空间，H为X的映射到Y的等连续集合。若H赋予点向收敛的拓扑，则映射 Y 中的 $H \times X$ 的 $(h, x) \to h(x)$ 是连续的。*

更直观地，这表达了这样一个事实：如果$h \in H$*逐点*收敛到$h_0 \in H$，并且如果$x \in X$收敛到$x_0$，那么$h(x)$收敛到$h_0(x_0)$。

#### 推论 5 {#top-x-s2-prop-1-cor-5 .statement tag=0CCA}

*设X为拓扑空间，设Y、Z为两个一致的空间，设H为Y的映射到Z的等连续集合。如果H、$\mathscr{C}(X; Y)$和$\mathscr{C}(X; Z)$被赋予逐点收敛的拓扑，则$H \times \mathscr{C}(X; Y)$到$\mathscr{C}(X; Z)$的映射$(u, v) \to u \circ v$是连续的。*

我们必须证明，对于 Z 中的每个 $x \in X$，$H \times \mathscr{C}(X; Y)$ 的映射 $(u, v) \to u(v(x))$ 是连续的。现在 $v \to v(x)$ 在 H (§ 1, no. 2, 注 6) 上连续，由推论 4 可知 $(u, y) \to u(y)$ 是 $H \times Y$ 在 Z 上的连续映射；由于$(u, v) \to u(v(x))$是$(u, y) \to u(y)$和$(u, v) \to (u, v(x))$的合成，结果得证。

以下命题及其推论是命题1的推论3和4的类似物，对于映射的一致等连续集合：

#### 命题 2 {#top-x-s2-prop-2 .statement tag=0CCB}

令 T、X、Y 一致空间，令 f 为 T × X 到 Y 的映射。则 f 一致连续当且仅当满足以下两个条件：

1) 映射 x → f(t, x) (t ∈ T) 形式 $\mathscr{F}(X; Y)$ 的一致等连续子集。

2) 映射 t → f(t, x) (x ∈ X) 形式 $\mathscr{F}(T; Y)$ 的一致等连续子集。

很容易看出条件是必要的。相反，假设他们感到满意。设W为Y的随从；则存在 T 的随行人员 U 和 X 的随行人员 V，使得：

1) $(t', t'') \in U$ 意味着，对于每个 $x \in X$，
$$
(f(t', x), f(t'', x)) \in W.
$$

2) $(x', x'') \in V$ 意味着对于每个 $t \in T$，
$$
(f(t, x'), f(t, x'')) \in W.
$$

现在很清楚，关系“$(t', t'') \in U$和$(x', x'') \in V$”意味着$(f(t', x'), f(t'', x'')) \in \hat{W}$、从而的结果。

特别地，取T为$\mathscr{F}(X; Y)$的子集H，具有一致收敛的一致性，取f为典范映射$(h, x) \to h(x)$；那么命题 2 的条件 2) 自动满足，因为对于 Y 的每个随行人员 W，对 $(h', h'')$ 的集合，使得所有 $x \in X$ 的 $(h'(x), h''(x)) \in W$ 都是由定义制服的随行人员H 的结构。因此只需表达条件 1)；其他字：

#### 推论{#top-x-s2-n1-cor-1 .statement tag=0CCC}

令X，Y为两个一致的空间，并令H为$\mathscr{F}(X; Y)$的子集。则 H 是一致等连续的，当且仅当 $H \times X$ 到 Y 中的映射 $(h, x) \to h(x)$ 是一致连续的，H 具有一致收敛的一致性。

### 2. 等连续性的特殊判据

很明显，等连续（或一致等连续）集合的每个子集都是等连续（或一致等连续）的。同样，如果 X 是拓扑（或一致）空间并且 Y 是一致空间，则 $\mathscr{F}(X; Y)$ 的等连续（或一致等连续）子集的每个有限并都是等连续（或一致等连续）。

令X，X'为两个拓扑（或均匀）空间，令Y，Y'为两个均匀空间，令$f : X \to X'$为连续（或均匀连续）映射，并令$g : Y \to Y'$为均匀连续映射。

紧随定义，$\mathscr{F}(X; Y)$的映射$u \to g \circ u \circ f$进入$\mathscr{F}(X'; Y')$变换等连续（或一致等连续）集合进入等连续（或一致等连续）集合。

#### 命题 3 {#top-x-s2-prop-3 .statement tag=0CCD}

*令$X$为拓扑（或制服）空间，让$(Y_i)_{i \in I}$为制服空间的族，让$Y$为集合，对于每个$i \in I$，令$f_i$为映射 $Y$ 变为$Y_i$。令 $Y$ 具有最粗糙的均匀性，使得所有 $f_i$ 均匀连续。为了使 $\mathscr{F}(X; Y)$ 的子集 $H$ 等连续（或一致等连续），对于每个 $i \in I$，映射 $u \to f_i \circ u$ 下的 $H$ 的像是等连续（或一致等连续）是必要且充分的等连续）子集 / $\mathscr{F}(X; Y_i)$。*

这是定义1和2的直接的推论和$Y$随从的定义。

#### 命题 4 {#top-x-s2-prop-4 .statement tag=0CCE}

*令$X, Y$为两个均匀的空间，并令$H$为$X$均匀连续的映射到$Y$的集合。令$\hat{X}, \hat{Y}$分别为$X, Y$的Hausdorff完成，并让$\tilde{H}$表示映射$\hat{u} : \hat{X} \to \hat{Y}$的集合，因为$u$贯穿$H$（章II, § 3, no. 7，命题） 15）。那么 $H$ 是一致等连续的当且仅当 $\tilde{H}$ 是一致等连续的。*

我们记得图表

$$
\begin{array}{ccc}
X & \xrightarrow{u} & Y \\
i \downarrow & & j \downarrow \\
\hat{X} & \xrightarrow{\hat{u}} & \hat{Y}
\end{array}
$$

是可交换的，其中 $i$ 和 $j$ 是典范映射；此外，$X$（分别为$Y$）的均匀度在$i$（分别为$j$）和$\hat{X}$（分别为$\hat{Y}$）的均匀度下为逆像。因此，$H$ 是一致等连续的，当且仅当映射 $u \to j \circ u$ 下的像一致等连续（命题 3），并且我们可能已经将自己限制在 $Y$ 是 Hausdorff 且完备的情况；此外，如果$\tilde{H}$一致等连续，那么$H$也是一致等连续的，因为它是映射$\hat{u} \to \hat{u} \circ i$下$\tilde{H}$的像；因此，当$Y = \hat{Y}$时，仍然需要证明逆命题。令$V$为$Y$的封闭随从；到假设时，有$X$的随从$U$，这样关系$(x, x') \in U$和$u \in H$意味着$(u(x), u(x')) \in V$。现在，如果$U'$是$i \times i$下$U$的像，则$\hat{X} \times \hat{X}$中$U'$的闭包$\overline{U'}$是$\hat{X}$的随从（章II, § 3, no. 7，命题） 12); 假设意味着，每当$(z, z') \in U'$和$u \in H$时，我们就有$(\hat{u}(z), \hat{u}(z')) \in V$。由于 $V$ 是闭集且 $\hat{u}$ 是连续的，因此对于所有 $(t, t') \in \overline{U'}$ 和所有 $u \in H$，我们也有 $(\hat{u}(t), \hat{u}(t')) \in V$；这样就完成了证明。

#### 命题 5 {#top-x-s2-prop-5 .statement tag=0CCF}

令$G, G'$为两个具有左均匀性的拓扑群，并令$H$为$G$的同态到$G'$的集合。那么下面的条件是等价的：
a) $H$ 在 $G$ 的单位元素 $e$ 处等连续，
b) $H$ 等连续，
c) $H$ 一致等连续。

只要证明 a) 蕴涵 c) 就足够了。设$V'$为$G'$的单位元素$e'$的邻域；那么，到假设时，$G$中有$e$的邻域$V$，使得所有$u \in H$都有$u(V) \subset V'$；因为 $H$ 的元素是同态，关系 $x^{-1} y \in V$ 意味着我们有
$$
(u(x))^{-1} u(y) = u(x^{-1} y) \in V'.
$$
鉴于$G$和$G'$（章III, § 3, no. 1）左侧均匀性的随行人员定义，结果如下。

### 3. 等连续集合的闭包

#### 命题 6 {#top-x-s2-prop-6 .statement tag=0CCG}

令$X$为拓扑（或均匀）空间，令$Y$为均匀空间，并令$H$为$\mathscr{F}(X; Y)$的子集。那么 $H$ 在点 $x_0 \in X$ 等连续（或一致等连续）当且仅当 $\mathscr{F}_s(X; Y)$ 中 $H$ 的闭包 $\overline{H}$ 在 $x_0$ 等连续（或一致等连续）。

条件就足够了，微不足道。为了表明这是必要的，考虑 $Y$ 的随行人员 $V$，它在 $Y \times Y$ 关闭；通过假设，$X$中有$x_0$的邻域$U$（分别为$X$的随行人员$M$），这样关系$x \in U$（分别为$(x', x'') \in M$）意味着$(h(x_0), h(x)) \in V$ [分别。 $(h(x'), h(x'')) \in V$] 对于所有$h \in H$。由于$V$已关闭，映射$h \in \mathscr{F}(X; Y)$，其中满足关系$(h(x_0), h(x)) \in V$适用于所有$x \in U$[分别。 关系 $(h(x'), h(x'')) \in V$ 对于所有 $(x', x'') \in M$] 形式 $\mathscr{F}_s(X; Y)$ 的封闭子集（§ 1, no. 2、注 6）；由于此关闭子集包含$H$，它包含$\overline{H}$。因此，结果是，由于$Y$形式的封闭随从成为基本的系统随从（章II, § 1, no. 2，命题2，推论2）。

### 4.等连续集合上的点收敛和紧收敛

#### 定理 1 {#top-x-s2-thm-1 .statement tag=0CCH}

令$X$为拓扑（或一致）空间，令$Y$为一致空间，并令$H$为$\mathscr{C}(X; Y)$的等连续（或一致等连续）子集。那么 $H$ 上的以下均匀性是相同的：紧致（或预紧致）收敛的均匀性、点状收敛的均匀性以及 $X$ 密集子集 $D$ 中的点状收敛的均匀性。

足以表明$H$上的最后一个均匀度比第一个均匀度为更细；在其他字中，给定 $Y$ 的随行人员 $V$ 和 $X$ 的紧凑（或预紧式）子集 $A$，存在 $Y$ 的随行人员 $W$ 和有限子集 $F$ $D$使得关系

$$
(2)\quad u \in H,\ v \in H\ \text{and}\ (u(x), v(x)) \in W\ \text{for all}\ x \in F
$$

意味着

$$
(3)\quad (u(x),\ v(x)) \in V\ \text{for all}\ x \in A.
$$

首先假设 $A$ 是紧致的且 $H$ 等连续。给定$Y$的对称随行$W$，每个点$x \in X$都有邻域$U(x)$，这样关系$x' \in U(x)$意味着所有$u \in H$的$(u(x),\ u(x')) \in W$。因此，我们可以通过开集合$U_i$的有限数覆盖紧集$A$，这样，对于相同集合$U_i$的点$x',\ x''$中的每个对，我们有$(u(x'),\ u(x'')) \in \hat{W}$ 对于所有 $u \in H$。令$a_i$为$D \cap U_i$的点，令$F$为$a_i$的集合，并假设(2)为真；那么对于每个$x \in A$，都存在指标 $i$，使得$a_i$和$x$属于到相同的集合$U_i$，因此我们有$(u(x),\ u(a_i)) \in \hat{W}$和$(v(a'),\ v(x)) \in \hat{W}$；因此，只要选择$W$使得$\hat{W} \subset V$，（2）就意味着（3）。

如果 $A$ 是预紧的且 $H$ 一致等连续，则我们应用命题 4 of no. 2； $i(A)$在$\hat{X}$中紧凑，$i(D)$在$\hat{X}$中密集，并且$Y$的随行人员是映射$j \times j$下的$\hat{Y}$随行人员的逆像，注就足够了。

#### 推论{#top-x-s2-n4-cor-1 .statement tag=0CCI}

*在定理 1 的假设下，$\mathscr{F}(X; Y)$中$H$相对于点式收敛拓扑的闭包$\overline{H}$与$\mathscr{C}(X; Y)$中$H$相对于紧致（或预紧致）拓扑的闭包相同收敛。*

因为集合 $\overline{H}$ 与 no. 3 的命题 6 等连续（或一致等连续），因此包含在 $\mathscr{C}(X; Y)$ 中；结果直接来自以下事实：在 $\overline{H}$ 上，由于定理 1，所考虑的两种拓扑是相同的。

### 5. 连续紧集映射

#### 定理 2（阿斯科利）{#top-x-s2-thm-2 .statement tag=0CCJ}

*令$X$为拓扑（或均匀）空间，令$\mathscr{S}$为$X$的覆盖，令$Y$为均匀空间和$X$的映射的$H$集合 $Y$使得对于每个$A \in \mathscr{S}$和每个$u \in H$，$u$到$A$的限制是连续的（分别是均匀连续的）。然后，为了使$H$相对于$\mathscr{S}$收敛的均匀性是预紧的，在所有情况下都是必要的，并且如果集合$A \in \mathscr{S}$是紧的（分别是预紧的），则满足以下条件也是充分的*：

a) 对于每个$A \in \mathscr{S}$，限制的集合$H|A \subset \mathscr{F}(A; Y)$到$H$的函数的$A$是等连续的（或者一致等连续的）。

b) 对于每个 $x \in X$，点 $u(x)$ ($u \in H$) 中的集合 $H(x) \subset Y$ 是预紧的。

1) 让我们首先证明条件 a) 和 b) 是必要的。我们知道(§ 1, no. 2, 注 6)，$\mathscr{F}_{\mathscr{S}}(X; Y)$到$Y$的映射$u \to u(x)$是一致连续的；因此，如果 $H$ 是预紧的，$H(x)$ 也是预紧的（章 II, § 4, no. 2, 命题 2），这就证明了 b)。为了证明a)，考虑集合$A \in \mathscr{S}$、点$x_0 \in A$以及$Y$的随行人员$V$；由于$H$是预紧的，它可以被$W(A, V)$-小集合的有限数覆盖；在其他字中，有有限序列$(u_i)$ / 元素 / $H$，这样，对于每个$u \in H$，我们有

$$
(u(x),\ u_i(x)) \in V \quad \text{for all } x \in A
$$

至少一个指标 $i$。

由于每个$u_i|A$在$x_0$处连续（或均匀连续），因此$A$中有$x_0$的邻域$U_i$（或$A$的随行人员$M_i$），使得

$$
x \in U_i \implies (u_i(x), u_i(x_0)) \in V,
$$

（分别这样

$$
(x', x'') \in M_i \implies (u_i(x'), u_i(x'')) \in V.)
$$

令$U$（或$M$）为$U_i$（或$M_i$）的交；它是$A$中$x_0$的邻域（分别是$A$的随行人员）。对于每个$u \in H$，有指标$i$，其中（4）成立；为$x_0$和$x$（分别为$x'$和$x''$）写出条件（4），并考虑（5）[分别。 (6)]，我们立即看到关系 $x \in U$ [分别。 $(x', x'') \in M$] 意味着$(u(x),\ u(x_0)) \in \overset{\circ}{V}$ [分别。 $(u(x'),\ u(x'')) \in \overset{\circ}{V}$]，每个$u \in H$；这就建立了a)。

2) 现在让我们证明，如果集合 $A \in \mathscr{S}$ 是紧致的（分别是预紧致的），则条件 a) 和 b) 是充分的。 条件 b) 意味着 $H$ 相对于逐点收敛的均匀性是预紧的 (章 II, § 4, no. 2, 命题 3)。但从条件a)和no. 4的定理1可以得出，在$H|A$上，$A$重合中点向收敛的一致性与$A$中一致收敛的一致性；因此$H|A$在$\mathscr{F}_u(A; Y)$中是预紧的，这意味着$H$相对于$\mathscr{S}$收敛的均匀性（§ 1, no. 2）是预紧的。

如果$Y$是预紧空间，则注自动满足定理2的条件b)。

#### 推论 1 {#top-x-s2-thm-2-cor-1 .statement tag=0CCK}

令$X$为拓扑（或一致）空间，令$Y$为豪斯多夫一致空间，并令$H$为$C(X; Y)$的等连续（或一致等连续）子集。假设对于每个$x \in X$，$H(x)$ 在$Y$ 中相对紧凑。那么 $H$ 相对于拓扑的紧凑（或预紧致）收敛而言，在 $C(X; Y)$ 中是相对紧凑的。

设$\overline{H}$为$\mathscr{F}_s(X; Y)$中$H$的闭包。 $\overline{H}$ 等连续（或一致等连续）（no. 3、命题 6）。此外，我们有$\overline{H}(x) \subset \overline{H(x)}$（§ 1, no. 2，注6），因此$\overline{H}(x)$也相对紧凑；因此定理 2表明$\overline{H}$相对于$\mathscr{S}$收敛是预紧的，其中$\mathscr{S}$表示$X$的所有紧（或预紧）子集的集合。此外，由于 $\overline{H(x)}$ 是紧致的，因此是完备的，$\overline{H}$ 对于逐点收敛的均匀性（章 II, § 3, no. 5、命题 10 和 no. 4、命题 8）是完备的，因此对于 $\mathscr{S}$ 收敛的均匀性也是完备的（§ 1, no. 5，命题5，推论2）；因此 $\overline{H}$ 是紧致的，因为它是预紧致的、完备的和 Hausdorff (§ 1, no. 2, 命题 1)。

#### 推论 2 {#top-x-s2-thm-2-cor-2 .statement tag=0CCL}

令$X$为拓扑（或均匀）空间，令$Y$为完整的豪斯多夫均匀空间，并令$H$为$C(X; Y)$的等连续（或均匀等连续）子集。假设对于所有$x \in D$，$H(x)$ 在$Y$ 中相对紧凑，其中$D$ 是$X$ 的稠密子集。那么 $H$ 在 $C(X; Y)$ 中相对于拓扑的紧致（或预紧致）收敛是相对紧致的。

足以证明$H(x)$对于所有$x \in X$来说是相对紧的，因为我们可以应用推论1。由于$Y$是完整的，因此足以证明$H(x)$对于所有$x \in X$来说是预紧的。现在，如果$V$是$Y$的任何对称周边，则存在$x$的邻域$U$，使得$(u(x), u(x')) \in V$对于所有$x' \in U$和所有$u \in H$。到假设时，存在$x' \in U \cap D$，并且由于$H(x')$在$Y$中相对紧凑，因此存在点$y_k \in Y$的有限数，使得$H(x')$包含在集合的并中$V(y_k)$；因此$H(x)$包含在集合$V(y_k)$的并中，证明是完整的。

#### 推论 3 {#top-x-s2-thm-2-cor-3 .statement tag=0CCM}

令 $X$ 为局部紧致空间，$Y$ 为 $C(X; Y)$ 的 Hausdorff 均匀空间，$H$ 子集。那么 $H$ 在 $C_c(X; Y)$ 中相对紧，当且仅当 $H$ 等连续，并且对于所有 $x \in X$，$H(x)$ 在 $Y$ 中相对紧。

鉴于推论1，足以证明，如果$H$在$C_c(X; Y)$中相对紧，则$H$是等连续的。现在每个点$x \in X$都有一个紧邻域$A$，并且从定理2可以得出$H/A$是等连续的；这意味着$H$在$x$等连续，结果得到证明。

#### 注 {#top-x-s2-n5-rem-1 .statement tag=0CCN}

令$X$为拓扑空间，$Y$为均匀空间，$\mathscr{S}$为$X$的子集集合。 然后，在 $\mathscr{F}_{\mathscr{S}}(X; Y)$ 的每个 *预紧* 子集 $H$ 上，$\mathscr{S}$ 收敛的均匀性与 $B = \bigcup_{A \in \mathscr{S}} A$ 中逐点收敛的均匀性相同。 我们可以将约化转化为$B = X$和$Y$是Hausdorff且完备的情况；因为如果$j$为典范嵌入$B \to X$且$i$典范映射$Y \to \hat{Y}$，则$\mathscr{S}$在$\mathscr{F}(X; Y)$上收敛的均匀性是$\mathscr{S}$在$\mathscr{F}(B; \hat{Y})$上收敛的均匀性的逆像映射 $\theta : u \to i \circ u \circ j$ (§ 1, no. 4, 命题 4)，并且 $H$ 是预紧的当且仅当 $\theta(H)$ 是 (章 II, § 4, no. 2, 命题 3)。 既然如此，如果$B = X$和$Y$是Hausdorff且完备，$\mathscr{F}_{\mathscr{S}}(X; Y)$是Hausdorff且完备（§ 1, no. 2，命题1和no. 5，定理1）；因而，这个空间中$H$的闭包$\overline{H}$是*紧凑的*。 在$\overline{H}$、拓扑逐点收敛是Hausdorff(§ 1, no. 2、命题1)并且比$\mathscr{S}$收敛更粗糙；因而，这两个拓扑重合（章I, § 9, no. 4，定理2，推论3），因而$\mathscr{S}$收敛和逐点收敛的一致性（章II, § 4, no. 1，定理1）。

### 习题{#top-x-s2-exercises}

§ 2](exercises/s2/)参见[习题。
