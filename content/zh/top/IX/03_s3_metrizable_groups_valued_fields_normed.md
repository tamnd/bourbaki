---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 3
section_title: Metrizable groups, valued fields, normed spaces and algebras
lang: zh
source: top-v-x
pdf_pages: 0167-0185, 0242-0245
extraction: ocr
subsections:
    - "no": 1
      title: METRIZABLE TOPOLOGICAL GROUPS
      page: 0
      pdf_page: 167
    - "no": 2
      title: VALUED DIVISION RINGS
      page: 0
      pdf_page: 171
    - "no": 3
      title: NORMED SPACES OVER A VALUED DIVISION RING
      page: 0
      pdf_page: 175
    - "no": 4
      title: QUOTIENT SPACES AND PRODUCT SPACES OF NORMED SPACES
      page: 0
      pdf_page: 178
    - "no": 5
      title: CONTINUOUS MULTILINEAR FUNCTIONS
      page: 0
      pdf_page: 179
    - "no": 6
      title: ABSOLUTELY SUMMABLE FAMILIES IN A NORMED SPACE
      page: 0
      pdf_page: 180
    - "no": 7
      title: NORMED ALGEBRAS OVER A VALUED FIELD
      page: 0
      pdf_page: 181
statements: 40
exercises: 13
content_sha256: 93a782e65acd9343f4856dadefe19c1dc582ffb0ecf26e92b96598989f6e5b24
translated_from: content/en/top/IX/03_s3_metrizable_groups_valued_fields_normed.md
translation_method: google
source_content_sha256: e6d9b744abb34c62818d886d27e40a745dc5749b1c99e6edf0894934f40987ea
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 9571cd6295b53f2b0142507dd8998886e8787d4f661cdcf6f659440cac953ac3
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 3. 可度量群，有价值域，标准化空间和代数

### 1. 可度量拓扑群

#### 命题 1 {#top-ix-s3-prop-1 .statement tag=0C3Y}

拓扑群 $G$ 的左均匀性和右均匀性可度量当且仅当 $G$ 是 Hausdorff 并且 $G$ 的单位元素 $e$ 具有可数基波系统为邻域。

条件显然是必要的。反之，如果满足，则令$(V_n)$为$e$的邻域的基本系统；如果$U_n$表示对$(x, y) \in G \times G$的集合使得$x^{-1}y \in V_n$，则$U_n$形式是$G$的左均匀性的可数基数系统；由于该均匀性是 Hausdorff，因此从 § 2, no. 4, 定理 1 可以得出它是可度量的。对于 $G$ 的右均匀性也是如此。

如果拓扑群 $G$ 的拓扑可度量，则称其为“可度量”。 命题 1 那么表明它的两个均匀性是可度量的。

可以借助以下概念来锐化此结果：

#### 定义 1 {#top-ix-s3-def-1 .statement tag=0C3Z}

*度量* $d$ *在群* $G$ *（乘法书写）* *据说是左不变*（或*右不变*）*如果我们有*

$$
d(zx, zy) = d(x, y) \quad [\text{resp. } d(xz, yz) = d(x, y)]
$$

*对于所有人*$x, y, z$*在*$G$。

#### 命题 2 {#top-ix-s3-prop-2 .statement tag=0C40}

*左*（或*右*）*可度量群* $G$的均匀性*可以通过左不变量*（或*右不变量*）*$G$上的度量来定义。

假设$e$的邻域的基本系统$(V_n)$由对称的邻域组成，使得每个$n$都有$V_{n+1}^3 \subset V_n$。那么左均匀性的相应的周边$U_n$是对称周边，使得$U_{n+1} \subset U_n$。 方法用于§ 1, no. 4 命题 2 的证明允许我们从$(U_n)$ 的序列构造，到$G$ 上的度量$d$ 与左均匀性兼容$G$；并且由于对于每个 $z \in G$ 映射 $(x, y) \to (zx, zy)$ 都留下每个 $U_n$ 不变量，$d$ 的定义表明它是左不变度量。这个方法也适用于正确的均匀性。

请注意，如果 $G$ 的两个均匀性不同，则度量 $d$ 不是右不变的，因此通常是 $d(x^{-1}, y^{-1}) \neq d(x, y)$。

特别是，如果$G$是可度量的阿贝尔的群，则其均匀性由不变度量$d$定义：如果$G$是相加的，我们有

$$
d(x, y) = d(0, y - x) = d(0, x - y).
$$

我们经常将$d(0, x)$写为$|x|$（或$||x|$）；那么我们有

$$
d(x, y) = |x - y|.
$$

函数$|x|$满足以下三个条件：

a) $|-x| = |x|$ 对于所有 $x \in G$。

b) $|x + y| \leq |x| + |y|$ 适用于所有 $x \in G$ 和所有 $y \in G$。

c) $|x| = 0$当且仅当$x = 0$。

反之：

#### 命题 3 {#top-ix-s3-prop-3 .statement tag=0C41}

*令$G$为阿贝尔的群，相加写成，$x \to |x|$为映射$G \to \mathbf{R}$，满足上述条件a)、b)和c)。那么函数$d(x, y) = |x - y|$是$G$上的不变度量； $G$上的定义与$G$上的群结构兼容，拓扑$\mathscr{T}$，$d$定义的均匀性与$G$赋予拓扑得到的拓扑群的均匀性相同$\mathscr{T}$.*

函数 $d(x, y)$ 是 $G$ 的度量，因为关系 $d(x, y) = 0$ 等价于 c) 的 $x = y$；通过 a) 我们有 $d(x, y) = d(y, x)$；和

$$
d(x, y) = |(x - z) + (z - y)| \leq |x - z| + |z - y| = d(x, z) + d(z, y)
$$

由b）。此外，由于$(x + z) - (y + z) = x - y$，$d$ 是不变的。
对于每个实数$x > 0$，令$V_x$为所有$x \in G$的集合，使得$|x| < x$；那么$V_x$形式是$0$的邻域的基本系统$\mathfrak{S}$对于拓扑$\mathscr{T}$，并且由于$d$是不变的，所以$a + \mathfrak{S}$是系统的基本系统邻域 / $a$ 为拓扑 $\mathscr{T}$，每个$a \in G$。根据a)，$V_x$是对称的，根据b)，我们有$V_a + V_x \subset V_{2a}$；因此拓扑$\mathscr{T}$与$G$（章III, § 1, no. 2）的群结构兼容。紧接着是命题的最后一个部分。

条件 a'、b' 和 c' 相当于 c) 与条件一起

$$
|x - y| \leq |x| + |y|.
$$

因为a'和b'清楚地暗示了b')；相反，在 b') 中取 $x = 0$ 并使用 c)，我们看到 $|-y| \leq |y|$； 替换 $y$ by $-y$ 由此得出 $|-y| = |y|$，即 a)； b') 中的替换 $y$ by $-y$ 然后我们得到 b')。

#### 命题 4 {#top-ix-s3-prop-4 .statement tag=0C42}

*如果 G 是可度量的群，则 G 的每个 Hausdorff 商群 G/H 都是可度量的。如果 G 也完整，则 G/H 完整 (*)。*

命题的第一个部分是G/H的单位元素在G/H中具有邻域的可数基数系统这一事实的推论；因为如果 (V_n) 是 G 中 e 的邻域的基数系统，则 G/H 中集合 V_n 的典范像 $\dot{V}_n$ 形式 G/H 的单位元素的邻域的基数系统 （章III, § 2, no. 6，命题17）。

如果 G 是完备的，为了证明 G/H 是完备的，通过 § 2, no. 6、命题 9，足以证明每个柯西序列 $(\dot{x}_n)$（相对于 G/H 的左均匀性）是收敛的。如有必要，我们可以通过经过到$(\dot{x}_n)$的子序列假设，对于指标$p, q$的每个对，使得$p \geq n$和$q \geq n$，我们有$\dot{x}_p^{-1}\dot{x}_q \in \dot{V}_n$；这意味着对于点$y \in \dot{x}_p, z \in \dot{x}_q$中的每个对，我们有$y^{-1}z \in HV_n = V_nH$；因此，对于每个$y \in \dot{x}_p$，$\dot{x}_q$的交和$y$的邻域$yV_n$不为空。假设选择序列(V_n)，使得$V_{n+1}^2 \subset V_n$，并且定义归纳G的点的序列$(x_n)$，使得$x_n \in \dot{x}_n$和$x_{n+1} \in x_n V_n$；根据上述内容，这是可能的。接下来是归纳，对于每个$p > 0$，我们有$x_{n+p} \in x_n V_n V_{n+1} \ldots V_{n+p-1} \subset x_n V_{n-1}$。因此序列$(x_n)$是G中的柯西序列，因此收敛到点$a$；紧接着G/H中$a$的典范像$\dot{a}$是序列$(\dot{x}_n)$的极限。

#### 推论 1 {#top-ix-s3-prop-4-cor-1 .statement tag=0C43}

*令 G 为完全可度量群，令 G_0 为 G 的密集子群，令 H_0 为 G_0 的闭法线子群。如果 H 是 G 中 H_0 的闭包，则商群 G_0/H_0 与 G/H 具有完全同构。*

H 是 G 的正规子群（章 III, § 2, no. 3、命题 8），命题 4 表明 G/H 是完备的。另外，如果$\varphi$是G在G/H上的典范映射，很明显$\varphi(G_0)$在G/H中是稠密的。因此，结果来自章 III, § 2, no. 7、命题 21。

令 G、G' 为两个 Hausdorff 阿贝尔的拓扑群和 $\hat{G}, \hat{G}'$ 它们各自的完成。我们记得（章III, § 3, no. 3，命题5），如果$u$是G到G'中的连续同态，那么$u$是一致连续的并且扩展唯一到$\hat{G}$的连续同态到$\hat{G}'$，余下的我们用$\hat{u}$表示

(*) 存在不可计量的完整群 G 包含一个封闭的子群 H，使得 G/H 不完整。

其中小节。 图表

$$
\begin{array}{ccc}
G & \xrightarrow{u} & G' \\
i \downarrow & & i' \downarrow \\
\hat{G} & \xrightarrow{\hat{u}} & \hat{G}'
\end{array}
$$

其中 $i, i'$ 是典范嵌入) 是可交换的。如果$v$是$G'$的连续同态到豪斯多夫阿贝尔的拓扑群$G''$，并且如果$w = v \circ u$，则紧接着$\hat{w} = \hat{v} \circ \hat{u}$。

令$H$为$G$的闭子群，并令$E = G/H$。令$j : H \to G$和$p : G \to E$为典范映射。设$\overline{H}$为$H$在$\hat{G}$的闭包； $\overline{H}$是完整的群，我们用$H$的完成$\hat{H}$来完成认同。 $j$到$\hat{H}$的连续扩张$\hat{j}$显然是$\hat{G}$中$\hat{H}$的典范嵌入。

假设从现在开始$G$是可度量的。那么$E = GH$到$\hat{G}\hat{H}$的典范映射到$E$的拓扑同构到完整群$\hat{G}/\hat{H}$（推论1）的密集子群上，因此我们可以将认同$\hat{G}\hat{H}$与$\hat{E}$以及$p$到$\hat{G}$的连续扩张$\hat{p}$以及$\hat{G}$的典范映射到$\hat{G}/\hat{H}$。

#### 推论 2 {#top-ix-s3-prop-4-cor-2 .statement tag=0C44}

*令$G, G'$为两个可度量的阿贝尔的拓扑群；让 $u : G \to G'$ 成为严格的态射，其中核 $N$ 和像 $P$。那么 $\hat{u} : \hat{G} \to \hat{G}'$ 是严格的态射，其中包含核 $\hat{N}$ 和像 $\hat{P}$。*

令$u = j \circ v \circ p$为$u$的规范因式分解，其中$v$是拓扑群$G/N$到拓扑群$u(G) = P$的同构。我们有$\hat{u} = \hat{j} \circ \hat{v} \circ \hat{p}$，我们已经看到$\hat{p}$是$\hat{G}$到$\hat{G}\hat{N}$的典范映射，$\hat{j}$是$\hat{P}$到$\hat{G}$的典范映射。另一方面，$\hat{v}$是$\hat{G}/\hat{N}$的同构到$\hat{P}$（章III, § 3, no. 4，命题5），从而结果。

#### 推论 3 {#top-ix-s3-prop-4-cor-3 .statement tag=0C45}

*令$G, G', G''$为三个可度量的阿贝尔的拓扑群，并让$u : G \to G'$和$v : G' \to G''$为两个严格的态射，使得序列$G \xrightarrow{u} G' \xrightarrow{v} G''$是精确的[即$u(G) = \overline{v}(0)$]。那么序列 $\hat{G} \xrightarrow{\hat{u}} \hat{G}' \xrightarrow{\hat{v}} \hat{G}''$ 就是准确的。*

因为如果我们输入$N = u(G) = \overline{v}(0)$，则从推论2可以得出$\hat{N}$既是$\hat{u}$的像又是$\hat{v}$的核。

#### 注 1 {#top-ix-s3-n1-rem-1 .statement tag=0C46}

令 $G$ 为非 Hausdorff 拓扑群，使得与 $G$ 相关的 Hausdorff 群是可度量的；等价地，使得$G$的单位元素在G中具有邻域的可数基波系统。命题4的证明无需修改即可应用于这种情况，H是G的任意法线子群，并表明Hausdorff与 G/H 相关的群是可度量的，并且只要 G 是完备的，G/H 就是完备的群（一般不是 Hausdorff）。

#### 注 2 {#top-ix-s3-n1-rem-2 .statement tag=0C47}

设 d 为可度量群 G 的左不变度量，其中定义拓扑，并令 H 为 G 的闭法线子群。如果 $\dot{x}$ 和 $\dot{y}$ 是 G/H 的任意两个点，请考虑距离两个中的$d(\dot{x}, \dot{y})$在G中关闭了子集$\dot{x}, \dot{y}$（§ 2, no. 2）；我们将看到，这个函数是G/H的左不变度量，而定义拓扑是这个商群。

首先注意，如果$x \in \dot{x}$和$y \in \dot{y}$我们有$d(\dot{x}, \dot{y}) = d(x, Hy)$；对于 $d(x, Hy) = \inf_{h \in H} d(x, h y)$，因此 $d(h'x, Hy) = d(x, Hy)$ 对于所有 $h' \in H$，因为 d 是左不变的；这就证明了断言 (§ 2, no. 2)。因此，对于每个 $\dot{z} \in G/H$，我们有 [§ 2, no. 2, 公式 (2)]

$$
|d(\dot{x}, \dot{z}) - d(\dot{y}, \dot{z})| = |d(x, \dot{z}) - d(y, \dot{z})| \leq d(x, y);
$$

由于这个不等式对于所有$x \in \dot{x}$和所有$y \in \dot{y}$都有效，所以我们有$|d(\dot{x}, \dot{z}) - d(\dot{y}, \dot{z})| \leq d(\dot{x}, \dot{y})$，这表明$d(\dot{x}, \dot{y})$是G/H的度量。此外，对于任意 $z \in \dot{z}$，我们有

$$
d(\dot{z}x, \dot{z}y) = \inf_{h \in H} d(zx, hzy)
$$

从上面；但由于 $hzy = z(z^{-1}hz) y$ 和 $z^{-1}hz$ 穿过 H，就像 h 穿过 H（H 是正常的）一样，$d(x, y)$ 的左不变性表明我们有 $d(zx, Hz y) = d(x, Hy) = d(\dot{x}, \dot{y})$。最后，如果V是$d(e, x) < \alpha$定义的G中e的邻域，则G/H中V的像V就是$d(e, \dot{x}) < \alpha$定义的集合；这样就完成了证明。

### 2. 有价值的除法环

#### 定义 2 {#top-ix-s3-def-2 .statement tag=0C48}

除法环 K 上的绝对值是 K 到 $\mathbf{R}_+$ 的映射 $x \to |x|$，满足以下条件：

(VM_I) $|x| = 0$ 当且仅当$x = 0$。
(VM_II) $|xy| = |x| \cdot |y|$ 对于 K 中的所有 $x, y$。
(VM_III) $|x + y| \leq |x| + |y|$ 对于 K 中的所有 $x, y$。

通过(VM_II)我们有$|x| = |1| \cdot |x|$，并且由于通过(VM_I)至少有一个x使得$|x| \neq 0$，我们有$|1| = 1$；由此可知$1 = |1|^2$，因而$|1| = 1$，因而

$$
|-x| = |-1| |x| = |x|;
$$

因而$|x - y| \leq |x| + |y|$对于K中的所有$x, y$。因此我们可以说$d(x, y) = |x - y|$是加法群K上的不变度量，并且映射$x \to |x|$是非零的乘法群$K^*$的同态将$K$中的元素转换为乘法群$\mathbf{R}_+^*$中的实数$> 0$。

不变度量$|x - y|$定义是$K$上的度量空间拓扑，与其加法群结构兼容（no. 1，命题3）；但是，此外，这个拓扑与$K$的除法环结构兼容。因为$xy$在$K \times K$上的连续性来自关系

$$
xy - x_0 y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0),
$$

这给出了

$$
|xy - x_0 y_0| \leq |x - x_0| \cdot |y - y_0| + |x_0| \cdot |y - y_0| + |y_0| \cdot |x - x_0|.
$$

同样，$x^{-1}$在每个点$x_0 \neq 0$的连续性源自恒等式$x^{-1} - x_0^{-1} = x^{-1}(x_0 - x)x_0^{-1}$，由(VM_{II})给出，

$$
|x^{-1} - x_0^{-1}| = \frac{|x - x_0|}{|x_0| \cdot |x|};
$$

现在如果$\varepsilon > 0$使得$\varepsilon < |x_0|$、关系$|x - x_0| \leq \varepsilon$意味着$|x| \geq |x_0| - \varepsilon$、从而$|x^{-1} - x_0^{-1}| \leq \varepsilon / |x_0|(|x_0| - \varepsilon)$；这就建立了$x^{-1}$在点$x_0$的连续性。

#### 定义 3 {#top-ix-s3-def-3 .statement tag=0C49}

*有值除法环是除法环* $K$ *赋予由给定绝对值值在* $K$ 定义的结构。

有价值的除法环将始终被认为具有由其绝对值值定义的拓扑，这使其成为*拓扑*除法环。如果$K_0$是取值除法环$K$的除法子环，则$K$上的绝对值值的限制到$K_0$是$K_0$上的绝对值值，其中定义在由$K$的拓扑诱发$K_0$拓扑。

#### 例 1 {#top-ix-s3-n2-exa-1 .statement tag=0C4A}

设$K$为任意除法环。对于每个$x \in K$，如果$x \neq 0$，则放入$|x| = 1$，并且$|0| = 0$。 映射$x \to |x|$如此定义是$K$上的绝对值，称为*不正确*绝对值。当且仅当 $|x|$ 是不正确的绝对值值时，由绝对值值 $|x|$ 在除法环 $K$ 上定义的拓扑才是*离散*。这个条件显然已经足够了；反之，如果$K$的拓扑是离散的，则$|x|$不能取除1以外的值$\alpha > 0$；因为如果我们有 $|x_0| = \alpha < 1$，序列 $(x_0^n)$ 将由非零项组成，并且会收敛到 0；要处理$\alpha > 1$的情况，请考虑用$x_0^{-1}$代替$x_0$。

#### 例 2 {#top-ix-s3-n2-exa-2 .statement tag=0C4B}

实数 (章 IV, § 1, no. 6) 的绝对值值满足公理 (VM_I)、(VM_{II}) 和 (VM_{III})，且拓扑定义在域上$\mathbf{R}$ 是拓扑 / 实直线。在复数的域$\mathbf{C}$（用$\mathbf{R}^2$标识）[分别。四元数的除法环 $\mathbf{H}$（用 $\mathbf{R}^4$ 标识）] 欧氏范数又是值和域 $\mathbf{C}$ 的绝对除法定义拓扑 （分别为除法环$\mathbf{H}$)（章VIII, § 1，第 2 和第 4 号）。

#### 例 3 {#top-ix-s3-n2-exa-3 .statement tag=0C4C}

在除法环 $K$ 上，实际估值是在 $K^*$ 上定义的函数 $v$，$\mathbf{R}$ 中的值满足以下条件： a) 如果 $x \in K^*$ 和 $y \in K^*$，则$v(xy) = v(x) + v(y)$； b) 如果在加法$x + y \neq 0$，则$v(x + y) \geq \inf(v(x), v(y))$。如果$a$是任何实数$> 1$，那么我们可以通过将$|x| = a^{-v(x)}$代替$x \neq 0$和$|0| = 0$来将定义绝对值值放在$K$上。对于 $x \neq 0$ 和 $y \neq 0$ 的关系 $v(xy) = v(x) + v(y)$ 意味着关系 $|xy| = |x|.|y|$ 对于 $x$ 和 $y$ 的这些值，并且如果满足以下条件之一，那么这个关系是非常正确的： $x, y$为零；同样，从$x \neq 0, y \neq 0$和$x + y \neq 0$的关系$v(x + y) \geq \inf(v(x), v(y))$我们推导出$|x + y| \leq \sup(|x|, |y|) \leq |x| + |y|$，如果$x, y, x + y$之一是零，这些不等式仍然满足。特别是，如果$v_p(x)$是有理数的域$\mathbf{Q}$的$p$-adic估值（将$x$的分解中的$p$的指数转换为素数的乘积） 因子)，则相应的绝对值值 $|x|_p = p^{-v_p(x)}$ 称为 $p$-进数绝对值值在域 $\mathbf{Q}$ (cf. 章 III, § 6， 习题23）。

#### 注 {#top-ix-s3-n2-rem-1 .statement tag=0C4D}

如果在定值除法环中，$x$是单位元的根，则$|x| = 1$，因为$x^n = 1$意味着$|x|^n = 1$，因此意味着$|x| = 1$。特别是，有限域上唯一的绝对值是不正确的绝对值，因为这样的域的每个元素$\neq 0$都是单位元的根。

#### 定义 4 {#top-ix-s3-def-4 .statement tag=0C4E}

除法环 $K$ 上的两个绝对值被认为是等价的，如果它们定义与$K$ 上的拓扑相同。

#### 命题 5 {#top-ix-s3-prop-5 .statement tag=0C4F}

除法环 $K$ 上的两个绝对值值 $|x|_1, |x|_2$，两者都不是不正确的绝对值值，当且仅当关系 $|x|_1 < 1$ 蕴含 $|x|_2 < 1$ 时，它们是等价的。则存在实数 $\rho > 0$，使得 $|x|_2 = |x|_1^\rho$ 对于所有 $x \in K$。

条件是必要的，对于所有$x \in K$中的集合，使得$|x|_1 < 1$与所有$x$中的集合相同，使得对于由绝对值$|x|_1$定义的拓扑， $\lim_{n \to \infty} x^n = 0$。

反过来假设$|x|_1 < 1 \Longrightarrow |x|_2 < 1$。然后$|x|_1 > 1 \Longrightarrow |x|_2 > 1$，因为$|x^{-1}|_1 < 1$，因此$|x^{-1}|_2 < 1$。由于到假设，绝对值$|x|_1$并无不当，因此存在$x_0 \in K$使得$|x_0|_1 > 1$。设 $a = |x_0|_1, b = |x_0|_2$ 并设 $\rho = \log b / \log a > 0$。设$x \in K^*$并放入$|x|_1 = |x_0|_1^\gamma$。如果$m$和$n$是整数，使得$n > 0$和$m/n > \gamma$，则$|x|_1 < |x_0|_1^{m/n}$，因此$|x^n x_0^{-m}|_1 < 1$；因此$|x^n x_0^{-m}|_2 < 1, |x|_2 < |x_0|_2^{m/n}$。类似地，如果$m/n < \gamma$，我们看到$|x|_2 > |x_0|_2^{m/n}$；因此$|x|_2 = |x_0|_2^\gamma$；其他字

$$
\log |x|_2 = \gamma \log b = \gamma \rho \log a = \rho \log |x|_1,
$$

即$|x|_2 = |x|^p_1$。 现在很清楚，$|x|_1$和$|x|_2$在$K$上定义的拓扑的零邻域是相同的。

相反，如果$|x|$是$K$上的任何绝对值，则对于所有$p$，函数$|x|^p$是$K$上的绝对值（相当于$|x|$），使得$0 < p \leq 1$。我们只需验证不等式$|x + y|^p \leq |x|^p + |y|^p$；并且由于 $|x + y|^p \leq (|x| + |y|)^p$ 就足以证明，如果 $a > 0$ 和 $b > 0$，对于任何 $p$ ，我们有 $(a + b)^p \leq a^p + b^p$ 使得 $0 < p \leq 1$ 。如果我们把$c = a/(a + b)$和$d = b/(a + b)$放进去，就有$c + d = 1$，要证明的不等式就是$c^p + d^p \geq 1$；但这紧随关系、$c^p \geq c$和$d^p \geq d$而来，它们自$0 < c \leq 1$、$0 < d \leq 1$、$0 < p \leq 1$起有效。

因此，$r > 0$的值的集合使得$|x|^r$是绝对值，值是$\mathbf{R}$的有限或无限区间，其左端点为$0$；如果它是有限的，那么它显然是封闭的；因为如果我们对$K$中的任何$x, y$和所有$r$有$|x + y|^r \leq |x|^r + |y|^r$使得$0 < r < r_0$，那么通过连续性不等式对于$r = r_0$仍然有效。如果$|x|^r$对于所有$r > 0$来说是绝对的值，那么我们有
$$
|x + y| \leq (|x|^r + |y|^r)^{1/r}
$$
对于 $K$ 和所有 $r > 0$ 中的所有 $x$ 和 $y$。现在，如果$a, b$是两个实数$\geq 0$，我们就有$\lim_{r \to \infty} (a^r + b^r)^{1/c} = \sup (a, b)$；例如，假设$a \geq b$，我们有$a \leq (a^r + b^r)^{1/r} \leq 2^{1/r} a$，让$r \to + \infty$得出结果。

因此，如果 $|x|^r$ 是所有 $r > 0$ 的绝对值，我们有
$$
|x + y| \leq \sup (|x|, |y|)
$$
可以用说表示，$v(x) = -\log |x| \ (x \neq 0)$是$K$的估值。

#### 注 {#top-ix-s3-n2-rem-2 .statement tag=0C4G}

命题 5 的证明表明，如果$|x|_2$定义的拓扑比$|x|_1$定义的粗，且$|x|_1$不不当，则$|x|_1$和$|x|_2$等价，对于关系 $|x|_2 < 1$则意味着$|x|_2 < 1$。因此，$K$上的两个绝对值定义的拓扑（两者都不是不恰当的）不能具有可比性，但并不完全相同。

#### 命题 6 {#top-ix-s3-prop-6 .statement tag=0C4H}

*除法环* $K$ *的完成* $\hat{K}$ *具有绝对值值* $|x|$ *是除法环，并且函数* $|x|$ *可以通过连续性扩展到绝对值值* $\hat{K}$，*其中定义拓扑*$\hat{K}$。

令 $\mathfrak{F}$ 为 $K$ 上的柯西滤波器（相对于加法均匀性），它不具有 $0$ 作为集群点；要证明 $\hat{K}$ 是除环，只需确定映射 $x \to x^{-1}$ 下$\mathfrak{F}$ 的像是柯西滤波器基 (章 III, § 6, no. 8, 命题 7)。现在，到假设时，存在实数 $\alpha > 0$ 和集合 $A \in \mathfrak{F}$，使得 $|x| \geq \alpha$ 对于所有 $x \in A$；另一方面，对于每个$\varepsilon > 0$，都存在集合$B \in \mathfrak{F}$，使得所有$x \in B$都存在$B \subset A$和$|x - y| \leq \varepsilon$。

和$y \in B$；因此

$$
|x^{-1} - y^{-1}| = \frac{|x - y|}{|x| \cdot |y|} \leq \frac{\varepsilon}{a^2},
$$

接下来是命题的第一个部分。不变度量$|x - y| = d(x, y)$扩展通过连续性到$\hat{K}$（§ 2, no. 1，命题1）上的度量，其中$\hat{K}$的定义拓扑并且通过扩张的原理不变身份；我们继续用 $d(x, y)$ 表示这个不变度量。如果我们用$|x| = d(0, x)$代替$x \in \hat{K}$，很明显，通过函数$|x|$在$K$上的连续性，$|x|$是扩张，因此是$\hat{K}$上的绝对值乘以扩张的原理身份。

### 3. 标准化空间超过一个有价值的除法环

#### 定义 5 {#top-ix-s3-def-5 .statement tag=0C4I}

*如果 E 是非离散值除法环 K 上的（左）向量空间，则 E 上的范数是 E 到 $\mathbf{R}_+$ 的映射 $x \to p(x)$，满足以下公理*：

(NO_I) $p(x) = 0$当且仅当$x = 0$；
(NO_{II}) $p(x + y) \leq p(x) + p(y)$ 对于 E 中的所有$x, y$；
（NO_{III}）$p(tx) = |t|p(x)$适用于所有$t \in K$和所有$x \in E$。

最常遇到的标准化空间有$\mathbf{R}$或$\mathbf{C}$作为标量的域（通常是绝对值值）。

从 (NO_{III}) 可以得出 $p(-x) = p(x)$；因此，如果我们将$d(x, y) = p(x - y)$，$d$是加法群E上的*不变度量*，并且定义是与E的加法群结构兼容的度量空间拓扑（no. 1，命题） 3）；而且，映射

$$(t, x) \to tx$$

在 $K \times E$ 上*连续*；因为我们有

$$tx - t_0 x_0 = (t - t_0)(x - x_0) + (t - t_0)x + t_0(x - x_0)$$

因此

$$p(tx - t_0 x_0) \leq |t - t_0| p(x - x_0) + |t - t_0| p(x) + |t_0| p(x - x_0),$$

这表明，通过将 $|t - t_0|$ 和 $p(x - x_0)$ 足够小，左侧可以变得尽可能小。

令 E 为 K 的子集。函数 $f : E \to K$ 称为 K 上的范数空间。

规范化的空间被赋予拓扑以及由其范数定义的均匀性。

考虑有限维除法环 K。将其视为实数向量空间，绝对值 $|x|$ 为范数。

范数$\|x\| = \sqrt{\sum x_i^2}$，我们在空间$\mathbf{R}^n$（章VI, § 2）上称为欧氏范数，显然是范数在定义3的意义上。 函数$\sup |x_i|$和$\sum |x_i|$。

令$S(E; K')$为集合E上所有函数$f$的集合，将其值除以环$K'$，并且使得实值函数$x \mapsto f(x)$以 E 为界。这个集合显然是向量空间超过 $K'$。让我们用$p(f) = \sup_{x \in E} f(x)$表示，那么$p$是向量空间$S(E; K')$上的范数（cf.章X, § 1）。

\* 4) 在$\mathbf{R}$、函数的区间$I = [0, 1]$上定义的所有有限连续实值函数的向量空间$C(I; \mathbf{R})$上

$$
p(x) = \int_0^1 |x(t)| \, dt
$$

是范数。

在规范化的空间 E 中，具有中心 o 且半径为 1 的封闭球 B，即所有 $x$ 中的集合，使得$p(x) \leq 1$，将称为 E 的单位球。我们将证明邻域的基本系统 o 由单位球平移 K 的元素形成。 中心 o 且半径为 1 的开球是中心 o 且半径为 1 的闭球；因此，足以证明对于每个实数 $r > 0$ 都存在 $k \in \mathbf{N}$ 使得 $0 < |k| < r$；取$k = \lfloor c/r \rfloor$就足够了，其中$c$是足够大整数，在阶中$|k|^2 < r$。

令 E 为非离散值域 $K$ 上的标准化空间。

#### 命题 7 {#top-ix-s3-prop-7 .statement tag=0C4J}

向量空间 $E$ 上的两个范数 $p, q$ 等价当且仅当存在两个数 $a > 0, b > 0$ 使得

(I)
$$
a . p(x) \leq q(x) \leq b . p(x)
$$
对于所有$x \in E$。

这些不等式是足够的，因为从关系$a . p(x) \leq q(x)$可以得出，对于每个$r > 0$，具有中心o和半径$ar$（相对于范数$q$）的封闭球包含在具有中心o和半径$r$的封闭球中（相对于范数$p$）；因此，$q$定义的拓扑比$p$定义的拓扑为更细。类似地，不等式$q(x) \leq b . p(x)$表明$p$定义的拓扑比$q$定义的更细小，因此$p$和$q$是等价的。

现在让我们证明不等式 (I) 是必要的。如果 $q$ 定义的拓扑比 $p$ 定义的拓扑更细，则单位相对于 $p$ 的球包含中心 o 且半径为 $\alpha > 0$ 的闭球$q$；即，关系$q(x) \leq \alpha$意味着$p(x) \leq 1$。如果$t_0 \in K$使得$0 < |t_0| < 1$，那么对于$E$中的每个$x \neq o$，都有一个唯一的有理数整数$k$使得$\alpha |t_0| < q(t_0^k x) \leq \alpha$；因此$p(t_0^k x) \leq 1$，因此
$$
p(x) \leq \frac{1}{|t_0|^k} \leq \frac{1}{\alpha |t_0|} q(x);
$$
因此，对于所有$x \neq o$，我们有$a = \alpha |t_0|$，因此$a . p(x) \leq q(x)$，并且这个不等式在$x = o$时也有效。类似地，我们证明，如果$p$定义的拓扑比$q$定义的更细小，则存在$b > 0$使得$q(x) \leq b . p(x)$。

#### 例 {#top-ix-s3-n3-exa-1 .statement tag=0C4K}

在空间$\mathbf{R}^n$，三个范数
$$
\sqrt{\sum_{i=1}^n x_i^2}, \quad \sup_{1 \leq i \leq n} |x_i| \quad \text{and} \quad \sum_{i=1}^n |x_i|
$$
是等价的，因为我们有
(2)
$$
\sup_{1 \leq i \leq n} |x_i| \leq \sqrt{\sum_{i=1}^n x_i^2} \leq \sum_{i=1}^n |x_i| \leq n . \sup_{1 \leq i \leq n} |x_i|.
$$

#### 命题 8 {#top-ix-s3-prop-8 .statement tag=0C4L}

令$E$为非离散值除法环上的赋范空间，令$p$为$E$上的范数，并令$\hat{E}$为加法拓扑群，即加法群的完成$E$。那么函数$(t, x) \to tx$可以在$\hat{K}$上通过连续性扩展到$\hat{E}$向量空间结构上的$\hat{K} \times \hat{E}$和定义； 范数$p$可以通过连续性扩展到$\hat{E}$上的范数$\bar{p}$，其中$\hat{E}$的定义拓扑。

$tx$的扩张通过连续性是扩张的定理的特殊情况，其中乘积的连续双线性映射将两个阿贝尔的群转换为第三个（章III, § 6, no. 5， 定理1);对于$t \in \hat{K}$、$u \in \hat{K}$和$x \in \hat{E}$，通过扩张的原理，我们有$1.x = x$和$t(u x) = (t u)x$；因此外法则$(t, x) \to t x$确实是定义在$\hat{E}$结构上向量空间超过$\hat{K}$。另一方面，将不变度量$\overline{d}(x, y) = \overline{p}(x - y)$扩展转换为$\hat{E}$上的不变度量$\overline{d}$（§ 2, no. 1，命题1），其中$\hat{E}$的定义拓扑；如果我们集合$\overline{p}(x) = \overline{d}(0, x)$，则$\overline{p}$通过连续性是$p$的扩张，并且满足公理(NO_I)和(NO_{II})；由于$t x$在$\hat{K} \times \hat{E}$上的连续性，$\overline{p}$也满足(NO_{III})（扩张恒等式的原理），因此范数在$\hat{E}$上。

当我们必须考虑向量空间$E$上的确定范数空间结构时，我们通常会用$||x||$来表示向量$x$的范数，除非这个记号很可能会导致混乱。

### 4. 标准空间的商空间和乘积空间

#### 命题 9 {#top-ix-s3-prop-9 .statement tag=0C4M}

*令$E$为非离散值除法环$K$上的规范空间，并令$H$为$E$的闭向量子空间。如果，对于每个类$\dot{x} \in E/H$，我们将$||\dot{x}|| = \inf_{x \in \dot{x}} ||x||$，函数$||\dot{x}||$是范数放在向量空间$E/H$上，并且由此范数定义的拓扑是商 $H$ 拓扑 $E$。*

通过no. 1的注2，$d(\dot{x}, \dot{y}) = ||\dot{x} - \dot{y}||$是$E/H$上的不变度量，其中定义商乘以$E$的拓扑的$H$。剩下的只是显示 $||t \dot{x}|| = |t| \cdot ||\dot{x}||$，并且这紧随 $||\dot{x}||$ 的定义 [章 IV, § 5, no. 7，公式 (23)]。

范数 $||\dot{x}||$ 也可以解释如下：它是每个点* $x \in \dot{x}$ *与子空间* $H$ 的距离（以$E$为单位），因为点与 $\dot{x}$ 的距离为点$x - z$，其中$z$贯穿$H$。

#### 命题 10 {#top-ix-s3-prop-10 .statement tag=0C4N}

*令$(E_i)_{1 \leq i \leq n}$为非离散值除法环$K$上的范数空间的有限族，并令$E = \prod_{i=1}^n E_i$为乘积向量空间。如果对于每个$x = (x_i) \in E$，我们放置$||x|| = \sup_{1 \leq i \leq n} ||x_i||$，那么函数$||x||$是$E$上的范数，拓扑它在$E$上的定义是乘积的拓扑结构$E_i$。

对于如果 $x = (x_i)$ 和 $y = (y_i)$，我们有 $x + y = (x_i + y_i)$，因此
$$
||x + y|| = \sup_i ||x_i + y_i|| \leq \sup_i (||x_i|| + ||y_i||)
\leq \sup_i ||x_i|| + \sup_i ||y_i|| = ||x|| + ||y||.
$$

另一方面，很明显，$||tx|| = |t|.||x||$，并且如果$||x|| = 0$，则$||x_i|| = 0$，因而$x_i = 0$对于$1 \leq i \leq n$，因而$x = 0$；因而$||x||$是$E$上的范数。此外，关系 $||x|| < a$ 相当于 $n$ 关系 $||x_i|| < a$，因而 $E$ 上的范数 $||x||$ 定义乘积拓扑。

类似地，我们可以证明函数$\sum_{i=1}^n ||x_i||$和$\sqrt{\sum_{i=1}^n ||x_i||^2}$在$E$上是范数；不等式 (2) 表明所有三个范数都是*等价的*。

特别是，在（左或右）向量空间$K^n$，如果我们把

$$
p_1(x) = \sup_i |x_i|, \quad p_2(x) = \sum_{i=1}^n |x_i|, \quad p_3(x) = \sqrt{\sum_{i=1}^n |x_i|^2}
$$

对于$x = (x_i)_{1 \leq i \leq n}$，则三个函数$p_1, p_2, p_3$等价于范数，其中定义在$K^n$拓扑上，即因子$K$拓扑的乘积。

### 5. 连续多重线性函数

#### 定理 1 {#top-ix-s3-thm-1 .statement tag=0C4O}

*让$E_i (1 \leq i \leq n)$和$F$在非离散值除法环$K$上标准化空间，并让$f$是$\prod_{i=1}^n E_i$到$F$的多线性映射。那么 $f$ 在 $\prod_{i=1}^n E_i$ 上连续当且仅当存在实数 $a > 0$ 这样，对于所有 $x_i \in E_i \ (1 \leq i \leq n)$，我们有*

$$
||f(x_1, x_2, \ldots, x_n)|| \leq a . ||x_1|| . ||x_2|| \ldots ||x_n||
$$

(3)

条件是*必要的*。因为如果$f$在点$(0, 0, \ldots, 0)$连续，则存在数$b > 0$，使得关系$||x_i|| \leq b \ (1 \leq i \leq n)$暗示$||f(x_1, \ldots, x_n)|| \leq 1$。令$t_0$为$K$的元素，使得$0 < |t_0| < 1$；那么对于*每个* 点 $(x_i) \in \prod_{i=1}^n E_i$，使得$x_i$都不是零，存在$n$有理整数$k_i$使得$b|t_0| < ||t_0^{k_i} x_i|| \leq b$；因此我们有

$$
|t_0|^{k_1 + k_2 + \cdots + k_n} ||f(x_1, x_2, \ldots, x_n)|| \leq 1;
$$

另一方面，我们有 $\frac{1}{|t_0|^{k_i}} \leq \frac{1}{b|t_0|} ||x_i||$，因此关系 (3) 如下，即 $a = (1/b|t_0|)^n$。当$x_i$之一是零时，这个关系显然仍然有效。

条件就足够了。我们将证明，如果满足，则$f$在$\prod_{i=1}^n E_i$的每点$(a_i)$连续。我们可以写

$$
f(x_1, \ldots, x_n) - f(a_1, \ldots, a_n) = \sum_{i=1}^n f(a_1, \ldots, a_{i-1}, x_i - a_i, x_{i+1}, \ldots, x_n).
$$

现在，使用 (3)，条件 $||x_i - a_i|| \leq r$ ($1 \leq i \leq n$) 意味着

$$
||f(a_1, \ldots, a_{i-1}, x_i - a_i, x_{i+1}, \ldots, x_n)|| \leq ar \prod_{k \neq i}^n (||a_k|| + r);
$$

因而，如果 $c$ 是数 $||a_i||$ ($1 \leq i \leq n$) 中的最大值，我们有

$$
||f(x_1, \ldots, x_n) - f(a_1, \ldots, a_n)|| \leq nar (c + r)^{n-1}.
$$

由于这个不等式的右边是$r$中的多项式，其中零常数为项，所以当$r$趋于0时，它也趋于0；因而$f$是连续的。

#### 注 {#top-ix-s3-n5-rem-1 .statement tag=0C4P}

先前证明的命题中的两个是定理的推论：凭借关系$xr = t \cdot x$，双线性函数$tr$的连续性；和命题7，由$E$的应用定理1到恒等映射，视为空间$E$的线性映射，赋予范数$p$到空间 $E$ 赋予范数 $q$（反之亦然）。

### 6. 范数空间中的绝对可和族

#### 定义 8 {#top-ix-s3-def-8 .statement tag=0C4Q}

在规范的空间 $E$ 中，如果 $x_i$ 的范数的族 $(||x_i||)$ 在 $\mathbf{R}$ 中可求和，则 $E$ 的点的族 $(x_i)$ 被认为是绝对可和的。

这个概念似乎取决于在$E$上选择的范数；但通过 no. 3 的命题 7 以及实数可求和族的比较原理，对于 $E$ 上的范数 $p$ 绝对可求和的族对于 $E$ 上的任何范数绝对可求和，这相当于$p$。

如果 $(x_i)_{i \in I}$ 是 $E$ 的点的族，且可求和且绝对可求，我们有

$$
\left\| \sum_{i \in I} x_i \right\| \leq \sum_{i \in I} \|x_i\|.
$$

事实上，对于$I$的每个有限子集$J$，我们有$\left\| \sum_{i \in J} x_i \right\| \leq \sum_{i \in J} \|x_i\|$，并且不等式（4）相对于$I$的有限子集的有向集合，遵循经过到极限。

#### 命题 11 {#top-ix-s3-prop-11 .statement tag=0C4R}

在完全赋范空间 E 中，每个绝对可和族都是可和的。

因为如果$(x_i)$是E中的绝对可求族，那么对于每个$\varepsilon > 0$，指标集合I都有有限子集J，这样，对于不满足J的I的每个有限子集H，我们有$\sum_{i \in H} ||x_i|| \leq \varepsilon$；因而*更不必说* $\left\| \sum_{i \in H} x_i \right\| \leq \varepsilon$，这证明了命题，因为E是完备的（柯西准则，章III, § 5, no. 2，定理1）。

如果一般项为 $||x_n||$ 的级数收敛于 $\mathbf{R}$，或者（等价）如果族 $(x_n)$ 绝对可和，则一般项为 $x_n$ 的级数被称为在 E 中*绝对收敛*；因而（章III, § 5, no. 7，命题9）：

#### 推论 {#top-ix-s3-n6-cor-1 .statement tag=0C4S}

在完全范数空间 E 中，每个绝对收敛级数都是*交换收敛*。

命题 11 的逆命题一般是*假*。

例如，考虑实数的有界序列 $x = (x_n)_{n \in \mathbf{N}}$ 的空间 $\mathscr{B}(\mathbf{N}; \mathbf{R})$，以及范数 $||x|| = \sup_n |x_n|$。令 $x_m$ 为序列 $(x_{mn})_{n \in \mathbf{N}}$，使得 $m \neq n$ 为 $x_{mn} = 0$，$m \geq 1$ 为 $x_{mm} = 1/m$。立即验证序列$(x_m)_{m \in \mathbf{N}}$在$\mathscr{B}(\mathbf{N}; \mathbf{R})$中可求和，并且其和是元素$y = (y_n)$，使得$y_0 = 0$和$y_n = 1/n$如果$n \geq 1$；但由于$||x_m|| = 1/m$，$x_m$的范数的序列在$\mathbf{R}$中不可求和。

然而，我们在章VII, § 3, no. 1中看到，$\mathbf{R}^n$中的每个可求和族都是绝对可求的。

### 7. 标准化代数高于有价值的域

#### 定义 9 {#top-ix-s3-def-9 .statement tag=0C4T}

*如果 A 在非离散值域 K 上为代数，则 A 上的范数 $p(x)$（A 被视为 K 上的向量空间）被认为与 A 的代数结构兼容，如果拓扑定义与环结构兼容A. 代数在 K 上，赋予由范数定义的结构与代数结构兼容，称为规范代数。*

如果 A 是 K 上的范数代数，并且如果 $p(x)$ 是 A 上的范数，则 $A \times A$ 到 A 的双线性映射 $(x, y) \to xy$ 是连续的，假设；因此，通过no. 5的定理1，存在实数$a > 0$使得$p(xy) \leq a \cdot p(x)p(y)$。 替换 $p(x)$ 等价于范数 $a \cdot p(x)$，因此我们可以总是假设范数 $||x||$ 在规范化的代数 A 上是这样的

$$
||xy|| \leq ||x|| \cdot ||y||.
$$

从 (5) 到归纳可以得出，对于每个整数 $n > 0$，我们有

$$
||x^n|| \leq ||x||^n.
$$

#### 例 1 {#top-ix-s3-n7-exa-1 .statement tag=0C4U}

令$K$为有值除法环，并令$K'$为$K$的中心的子域，使得$K$的绝对值值$|x|$在$K'$上的迹不是不正确的绝对值$K'$值。那么$K$，其中$|x|$为范数，是$K'$上的规范代数。

#### 例 2 {#top-ix-s3-n7-exa-2 .statement tag=0C4V}

令$K$为非离散值域，并令$M_n(K)$为阶$n$的方阵与$K$的环。视为向量空间超过$K$，$M_n(K)$与$K^{n^2}$同构的。如果对于每个$X = (x_{ij}) \in M_n(K)$我们定义$\|X\| = \sup_{i,j} |x_{ij}|$，那么$\|X\|$是$M_n(K)$上的范数，并且由此范数定义的拓扑是$K^{n^2}$上的乘积拓扑 （命题10）；由此可见（由于超过 $K$ 的任何数变量中多项式的连续性）该范数与$M_n(K)$的$K$代数结构兼容。

#### 例 3 {#top-ix-s3-n7-exa-3 .statement tag=0C4W}

集合 $X$ 上所有函数 $f$ 的集合 $\mathscr{B}(X; K)$ 以及值位于非离散值域 $K$，使得 $x \to |f(x)|$ 的边界为$X$，代数超过$K$； 范数$\|f\| = \sup_{x \in X} |f(x)|$与$\mathscr{B}(X; K)$的环结构兼容，因为我们有$\|fg\| \leq \|f\|\cdot\|g\|$（cf.章X, § 1）。

令 $a$ 为规范化代数 $A$ 中的封闭两侧理想。如果在商代数 $A/a$ 中放入 $||\dot{x}|| = \inf_{x \in X} ||x||$，则在 $A/a$ 上得到范数，其中定义拓扑是商除以 $a$ 拓扑共 $A$ (命题 9)；由于此商拓扑与 $A/a$ (章 III, § 6, no. 4) 的商环结构兼容，因此商代数 $A/a$， 范数 $||x||$，是标准化的代数。

同样，如果 $(A_i)_{1 \leq i \leq n}$ 是 $n$ 范数代数的一个族，在一个有价值的域 $K$ 上，并且如果在乘积代数 $A = \prod_{i=1}^n A_i$ 中我们放置 $||x|| = \sup_i ||x_i||$，其中 $x = (x_i)$，我们有范数在 $A_i$ (命题 10) 拓扑的$A$ 定义乘积上；由于此拓扑与$A$（章III, § 6, no. 4）的环结构兼容，因此乘积代数$A$与范数$||x||$是规范的代数。

令 $A$ 为已定值域 $K$ 上的标准化代数。 $A$ (章 III, § 6, no. 5, 命题 6) 的补全$\hat{A}$ 也被赋予$\hat{K}$-向量空间结构 (no. 3, 命题 8)，由原理可知对于所有$t \in \hat{K}$和所有$x, y \in \hat{A}$，我们拥有$t(xy) = (tx)y = x(ty)$的扩张个身份。因此$\hat{A}$比$\hat{K}$大于代数；另一方面（no. 3，命题 8），$A$扩展上的范数通过连续性到范数，其中$\hat{A}$的定义拓扑，因此$\hat{A}$，赋予了这个范数，是域$\hat{K}$的*标准化代数*。

如果 $(x_\lambda)_{\lambda \in L}$ 和 $(y_\mu)_{\mu \in M}$ 是赋范代数 $A$ 中的两个绝对可求和族，则$(x_\lambda y_\mu)_{(\lambda, \mu) \in L \times M}$ 族绝对可求和，因为 $||x_\lambda y_\mu|| \leq ||x_\lambda|| \cdot ||y_\mu||$ (章 IV, § 7, no. 3, 命题 1)；如果加法 $A$ 是完备的，则所有三个族都是可求和的，我们有
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = \left( \sum_{\lambda \in L} x_\lambda \right) \left( \sum_{\mu \in M} y_\mu \right)
$$
通过左侧和的结合性（章 III, § 5, no. 3、公式 (2)）。

如果赋范代数$A$具有单位元$e \neq 0$，则映射$t \to te$是$K$的域结构到$A$的子域$Ke$的同构；这种同构也是$K$拓扑域结构与$Ke$拓扑域结构的同构（后者的拓扑由$A$的拓扑导出），因为$A$到$Ke$范数的限制$||te||$是等价于绝对值的范数
$$
|t| = \frac{1}{||e||} ||te||.
$$
如果$||e|| = 1$我们有$||te|| = |t|$，那么我们就可以用$A$的范数子域$Ke$来识别值域$K$，特别是我们可以用符号1来表示$A$的单位元素。

接下来我们只关心有范数的代数，它有单位元素$e$，并且其中范数满足不等式（5）；将$x = y = e$代入不等式，得出$||e|| \geq 1$。

#### 命题 12 {#top-ix-s3-prop-12 .statement tag=0C4X}

*如果级数其通项为$z^n$收敛于$A$，则$e - z$是$A$的单位，我们有*
$$
(e - z)^{-1} = \sum_{n=0}^\infty z^n.
$$
*相反，如果$||z|| < 1$且$e - z$在$A$中为单位，则一般项为$z^n$的级数是收敛的，并且公式(7)有效。*

对于每个 $p > 0$ 我们有
$$
(e - z) \sum_{n=0}^p z^n = e - z^{p+1}.
$$
如果项为$z^n$的级数收敛，且$y$为其和，则$z^n$与$n \to + \infty$一样趋于0；因此，通过（8）中的经过到极限，我们有$(e - z)y = e$；类似地，我们证明$y(e - z) = e$，从而证明$y = (e - z)^{-1}$（请注意，该论证的部分在任何具有单位元素的拓扑环中都是有效的）。

反之，如果$||z|| < 1$，则从$||z^{p+1}|| \leq ||z||^{p+1}$开始，$z^{p+1}$与$p \to +\infty$一样趋于0；将左边两边（8）乘以$(e-z)^{-1}$，并让$p$趋于无穷大，我们可以看到，级数的通项为$z^n$收敛，并且$(e-z)^{-1}$为其和。

#### 推论 {#top-ix-s3-n7-cor-1 .statement tag=0C4Y}

*设 A 为完全范数代数。然后对于每个$z \in A$，使得$||z|| < 1$，$e - z$在A中是单位。*

级数，其通项为$z^n$，是绝对收敛的，因为$||z^n|| \leq ||z||^n$对于$n > 0$，因此也是收敛的，因为A是完备的（no. 6，命题11）。

#### 命题 13 {#top-ix-s3-prop-13 .statement tag=0C4Z}

*设G是完全赋范代数 A的单位的群，则G是A的开子集； A 的拓扑在 G 上诱导的拓扑与 G 的群结构兼容；而G，被赋予了这个拓扑，是一个完整的群*（相对于它的两个均匀性中的每一个）。

推论至命题12表示A中$e$的G包含邻域V；因此，对于每个$x_0 \in G$，$x_0V$的元素是单位，$x_0V$是A中$x_0$的邻域，因为$x \mapsto x_0x$是A自身的同胚（$x_0$是A) 的单位。因此 G 在 A 中开。

为了证明 A 的拓扑在 G 上诱导的拓扑与 G 的群结构兼容，只要证明函数 $x^{-1}$ 在 G 上是“连续”的就足够了。设 $x_0 \in G$，对于每个 $x \in G$，将 $x$ 写成形式$x = x_0(e + u)$，所以$u = x_0^{-1}(x - x_0)$；那么$||u|| \leq ||x_0^{-1}|| \cdot ||x - x_0||$，因此如果$||x - x_0|| \leq 1 / ||x_0^{-1}||$，我们有$||u|| \leq 1$，$e + u = x_0^{-1}x$是单位，级数，其一般项是$(-1)^n u^n$是绝对收敛的，并且

$$
x^{-1} = (e + u)^{-1} x_0^{-1} = x_0^{-1} + \left( \sum_{n=1}^{\infty} (-1)^n u^n \right) x_0^{-1},
$$

由此可见

$$
||x_0^{-1} - x_0^{-1}|| \leq \left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \cdot ||u|| \cdot ||x_0^{-1}|| \\
\leq \left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \cdot ||x_0^{-1}|^2 \cdot ||x - x_0||.
$$

由于 $x$ 趋于 $x_0$，$||x - x_0||$ 趋于 0，并且由于

$$
\left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \leq ||e|| + \frac{||u||}{1 - ||u||}
$$

仍然有界，因此$x^{-1}$趋于$x_0^{-1}$。

最后，为了证明 G 的左均匀性是完整的，让我们证明关于该均匀性的每个柯西滤波器 $\tilde{\mathscr{F}}$ 都是关于 $A$ 的“加性”均匀性的柯西滤波器，并且收敛到 $G$ 的点。对于每个$\varepsilon$使得$0 < \varepsilon < 1$，存在集合$M \in \mathfrak{F}$使得$||x^{-1}y - e|| \leq \varepsilon$对于$M$中的所有$x, y$，即，使得
$$
||y - x|| \leq \varepsilon \ ||x||.
$$
设$a$为$M$的点；对于每个$x \in M$，我们有$||x - a|| \leq \varepsilon \ ||a||$，因此有$||x|| \leq (1 + \varepsilon)||a||$。另一方面，存在集合$N \subset M$属于到$\mathfrak{F}$，并且$||x^{-1}y - e|| \leq \varepsilon/(1 + \varepsilon)||a||$对于$N$中的所有$x$和$y$；由此得出$||y - x|| \leq \varepsilon ||x||/(1 + \varepsilon)||a|| \leq \varepsilon$，这表明$\mathfrak{F}$是关于$A$的加性均匀性的柯西滤波器，因此收敛到点$x_0$，因为$A$是完备的。由于 $x_0$ 是 $\mathfrak{F}$ 中的极限，因此对于所有 $x \in M$，我们通过扩张中的原理不等式得到 $||x^{-1}x_0 - e|| \leq \varepsilon$；从$\varepsilon > 1$开始，$x^{-1}x_0$在$A$中等于单位；因此$x_0$是单位，即$x_0 \in G$。

#### 命题 14 {#top-ix-s3-prop-14 .statement tag=0C50}

*在全值除法环中，非零元素的乘法群是全值群。*

证明与命题13类似；我们只需考虑环除法的绝对值值到 $A$ 的替换范数。

请注意，我们直接不能应用命题 13，因为（非交换）值除法环不一定是代数超过*非离散* 值域（除法的绝对值到中心的限制） 环可能不合适）。

#### 注 {#top-ix-s3-n7-rem-1 .statement tag=0C51}

对于非完全规范的代数来说，命题 13 不一定成立。例如，在$I = [0, 1]$上所有有限连续实值函数的代数$C(I; \mathbf{R})$中[范数为$||x|| = \sup_{t \in I} |x(t)|$]，$t$中所有*多项式*的子代数$P$（仅限于$I$) *不*完整；如果 $x(t)$ 是任何非常数多项式，则当 $\varepsilon$ 任意小时，$1 + \varepsilon x$ 任意接近 $P$ 的单位元素 1，但 $1 + \varepsilon x$ 不是单位 *in* $P$。然而，如果$A$是非完备范式代数，$G$是单位的群，$\hat{A}$是$A$的完备，那么$G$就是群的子群 $\hat{A}$的单位，因此$A$的拓扑在$G$上诱导的拓扑与$G$的群结构兼容。

### 习题 {#top-ix-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
