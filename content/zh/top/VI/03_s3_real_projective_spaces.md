---
book: top
book_title: General Topology
chapter: VI
chapter_title: Real number spaces and projective spaces
section: 3
section_title: Real projective spaces
lang: zh
source: top-v-x
pdf_pages: 0050-0060, 0067-0069
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGY OF REAL PROJECTIVE SPACES
      page: 0
      pdf_page: 51
    - "no": 2
      title: PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 53
    - "no": 3
      title: EMBEDDING REAL NUMBER SPACE IN PROJECTIVE SPACE
      page: 0
      pdf_page: 54
    - "no": 4
      title: APPLICATION TO THE EXTENSION OF REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 55
    - "no": 5
      title: SPACES OF PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 56
    - "no": 6
      title: GRASSMANNIANS
      page: 0
      pdf_page: 59
statements: 14
exercises: 10
content_sha256: 085dbb6eb2238da5b8580ddbd3e42470d72ee0e70c7076584c30743c8e06ace4
translated_from: content/en/top/VI/03_s3_real_projective_spaces.md
translation_method: google
source_content_sha256: 8a7a0642504d2c2735e8c21f04b3ffc8f7148755423f71666653ec4a58ab65fb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 26c06e803d895ce490a6927f9e955c137adc394f498c390b421bd9e7cd59bdbb
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 3. 真实投影空间

在这个截面中，我们需要不断调用概念并得出*商空间*（章I, § 3），特别是以下两个属性，为了方便起见，我们将其声明为引理：

令 $E$ 为由 $R$ 在 $A$ 上诱发的 $E$、$R_A$ 等价关系在 $E$、$A$ 子集上的拓扑空间、$R$ 等价关系，并让$f$是$E$的典范映射到$E/R$。然后：

#### 引理 1 {#top-vi-s3-lem-1 .statement tag=0BXG}

*如果$A$中相对于$R_A$饱和的每个开（或闭）集合是$E$中相对于$R$饱和的开（或闭）集合在$A$上的迹，则商空间 $A/R_A$ 同态于 $E/R$ 的子空间 $f(A)$。特别是如果 $A$ 在 $E$ 中开或闭并且相对于 $R$ 饱和。*

这是从章 I, § 3, no. 6 的命题 10 得出的。

#### 引理 2 {#top-vi-s3-lem-2 .statement tag=0BXH}

*如果有一个连续的映射* g *of* E *到* A *使得，对于所有* x ∈ E，g(x) *属于到等价类 of* x，*那么商空间* A/R_A *同胚于* E/R。

这是章I, § 3, no. 6的命题10的推论2。

### 1. 实投影的拓扑空间

我们回忆一下代数中的以下定义：给定环或域K的划分，左向量空间K_s^{n+1}中*行*经过到o的集合（即维数1的向量子空间） K 上的 n 维数* 的左投影空间被称为 K 上的 *左投影空间，并表示为 P_n(K)。

如果我们将 K_s^{n+1} 中从经过到 o 的每条线都设为对应，并且*省略原点*，我们就可以将 P_n(K) 的双射与 K_{n+1}^* 的*商*（K_s^{n+1} 中 {o} 的补集）通过以下等价关系 Δ_n(K) 进行比较K_{n+1}^* 的向量 x 和 y：“存在 t ∈ K 使得 t ≠ o 且 y = tx”。接下来我们将*认同* P_n(K) 与这个商集。在射影空间理论中，对于K_{n+1}^*的点坐标，我们取N的区间[0, n]为指标集合。 K_{n+1}^* 的点中任意一个的坐标 x_i (0 ≤ i ≤ n) 的典范像为 x ∈ P_n(K)，构成所谓的点 x 的齐次坐标*系统。

对于每个整数 p，使得 −1 ≤ p ≤ n，K_s^{n+1} 的 p + 1 维数（无原点）的向量子空间的 P_n(K) 中的典范像称为 p 维数的*投影线性簇*。 P_n(K) 的 p 点的系统被称为“自由”，如果它由 K_{n+1}^* 的 p 点的典范像组成，其中向量空间 K_s^{n+1} 中的形式一个*自由* 系统组成。由 p + 1 点的自由系统生成的 P_n(K) 的投影线性簇（即最小的包含这些 p + 1 点的投影线性簇）具有维数 p。

当K为域R时，相应的射影空间可以拓扑化，我们要研究的就是这些。

#### 定义 1 {#top-vi-s3-def-1 .statement tag=0BXI}

*射影空间* P_n(R) *赋予* R_{n+1}^* 的拓扑商拓扑 *通过等价关系* Δ_n(R) *称为 n 维数的实射影空间。*

射影空间 P_1(R) 称为*实射影线*，P_2(R) 称为*实射影平面*。

只要不存在混淆的风险，我们就写 P_n 和 Δ_n 而不是 P_n(R) 和 Δ_n(R)。

#### 命题 1 {#top-vi-s3-prop-1 .statement tag=0BXJ}

射影空间 $P_n$ 是豪斯多夫。

我们首先显示关系 $\Delta_n$ 已打开 (章 I, § 5, no. 2)。令$A$为$\mathbf{R}_{n+1}^*$中的开集合；为了使$A$相对于$\Delta_n$饱和，我们必须将集合$tA$的并与$A$拟似，因为$t$穿过实数$\neq 0$的集合；由于每个集合都是开放的，因此它们的并也是开放的。

通过章 I, § 8, no. 3的命题 8，如果我们证明由关系$\Delta_n$定义的$\mathbf{R}_{n+1}^* \times \mathbf{R}_{n+1}^*$的子集$M$是闭集，命题就被证明。设 $(x, y)$ 为 $\mathbf{R}_{n+1}^* \times \mathbf{R}_{n+1}^*$ 的点，位于 $M$ 的闭包中。如果$x = (x_i)$，则有指标$i$使得$x_i \neq 0$；因此，$(x, y)$存在邻域$V$，使得对于每个点$(x', y') \in M \cap V$，$x'$的第i个坐标$x'_i$不为0。由于$(x', y')$趋于$(x, y)$，同时保持在$M$， $y'_i {x'}^{-1}_i$趋于$t = y_i x_i^{-1}$；从$y' = (y'_i {x'}^{-1}_i) x'$开始，我们从经过到极限看到$y = x$，这表明$(x, y) \in M$。

#### 命题 2 {#top-vi-s3-prop-2 .statement tag=0BXK}

射影空间 $P_n$ 是紧致连通的，并且同胚于球体 $S_n$ 与等价关系在球面上由 $\Delta_n$ 引出的商。

设$\Delta'_n$是$\Delta_n$在$S_n$上诱发的等价关系（$\Delta'_n$的等价类是$S_n$的完全相反的点的对）。 $\mathbf{R}_{n+1}^*$到$S_n$的映射$x \to x/||x||$是连续的，因此(引理2)$P_n$同胚于$S_n / \Delta'_n$。由于$S_n$是紧连通的，$S_n$的每个豪斯多夫商空间也是紧连通的（章I, § 9, no. 4，定理2，推论1；§ 11, no. 3，命题7）。

#### 命题 3 {#top-vi-s3-prop-3 .statement tag=0BXL}

如果$n \geq 0$，射影空间$P_n$同胚于球$B_n$的商空间，通过识别$S_{n-1}$的每个点与其相反的点而获得。

令 $H$ 为由 $x_0 \leq 0$ 定义的 $S_n$ 的闭合半球。 $P_n$同态于$S_n$的空间除以关系$\Delta'_n$的商，也同态于$S_n$的子集$H$除以关系的商$\Delta''_n$ 由 $\Delta'_n$ 在 $H$ 引发。对于$\Delta'_n$的每一个等价类在至少一个点中满足$H$，因此（引理1）就足以验证我们是否相对于$\Delta'_n$饱和，$H$的开路子集$U$是饱和的对于 $V''_n$，我们得到 $S_n$ 的开放子集 $V$。现在如果$a = (a_i) \in U$和$a_0 < 0$，则$U$中包含$S_n$中有$a$的邻域$W$，$W$和$-W$的并是邻域 $a$相对于$\Delta'_n$饱和并包含在$V$中。另一方面，如果$a_0 = 0$，我们有$-a \in U$，并且存在$r > 0$使得点$x \in H$的集合其中满足关系中的一个或另一个||x - a|| < r, ||x + a|| < r 包含在 U 中； 点 x \in S_n 的集合，其中满足关系中的一个或另一个关系是 a 的邻域，其相对于 $\Delta'_n$ 饱和并包含在 V 中。

观察到，商空间$H / \Delta''_n$是通过在H中将H的交$S_{n-1}$和超平面$x_0 = 0$中的每个点与其相反的点进行识别而获得的。为了完成证明，只要注，顶点$e_0$（$\S$ 2，no. 4）的立体投影是H到$B_n$的同胚，这使得点保持不变$S_{n-1}$。

### 2. 投影线性簇

$\mathbf{R}^{n+1}$的每个单射线性映射$f$进入$\mathbf{R}^{m+1}$（$m \geq n$）定义，通过限制到$\mathbf{R}_{n+1}^*$，然后通过关系$\Delta_n$和$\Delta_m$的商（集合理论，R，$\S$5，无8），$P_n$的单射映射g到$P_m$，称为*射影线性映射*。如果$\varphi$（或$\psi$）是$\mathbf{R}_{n+1}^*$到$P_n$（或$\mathbf{R}_{m+1}^*$到$P_m$）的典范映射，我们有$g \circ \varphi = \psi \circ f$，这表明g在$P_n$上*连续* （章I、$\S$3、no. 4、命题6 的推论）。特别是，$P_n$的每个“射影线性变换”（即$P_n$的射影线性映射到自身）都是$P_n$到自身的“同胚”。

我们还记得，如果V和V'是$P_n$中p维数的两个射影线性簇，则存在$P_n$的射影线性变换，其中变换V到V'。特别是，如果$p \geq 0$，则存在射影线性变换，将变换V转换为*坐标*射影线性变换，也就是说$p + 1$维数（没有点o）的$\mathbf{R}^{n+1}$的坐标变换W'的典范像。如果我们将认同 W' 与 $\mathbf{R}_{p+1}^*$ 相结合，则 $\Delta_n$ 在 W' 上诱发的关系恰好是 $\Delta_p$；由于 W' 对于 $\Delta_n$ 是闭集且饱和的，引理 1 表明 V' 同胚于 $P_p$ 并且在 $P_n$ 中闭集；此外，如果 $p < n$，它的补集在 $P_n$ 中是稠密的（$\S$ 1，no. 4，命题 3 的推论）。因此：

#### 命题 4 {#top-vi-s3-prop-4 .statement tag=0BXM}

*射影空间 $P_n$ 中的 p 维数的每个射影线性簇在 $P_n$ 中闭集并且同胚于 $P_p$；如果 $p < n$ 其补集在 $P_n$ 中是稠密的。*

![图表显示射影空间 P_n 中的超平面 H，以及点 x_0^{-1}x、x 和 o，以及另一个平面 B。](https://i.imgur.com/3Q5z5QG.png)

图 4.

形式 $\sum_{i=0}^{n} a_i x_i = 0$的齐次坐标满足关系，其中$a_i$不全是零（超平面的“方程”）。

#### 命题 5 {#top-vi-s3-prop-5 .statement tag=0BXN}

*在射影空间* $\mathbf{P}_n$ ($n \geq 0$) 中，*射影超平面* $\mathbf{H}$ *同态于* $\mathbf{R}^n$。

通过进行投影线性变换，我们可以假设$\mathbf{H}$是超平面，其方程是$x_0 = 0$。 点 $x = (x_i)$ $\mathbf{R}_{n+1}^*$ 的集合 $A$，使得$x_0 \neq 0$相对于$\Delta_n$开路且饱和； $\mathbf{P}_n$中的典范像$C$是$\mathbf{P}_n$中$\mathbf{H}$的补集，因此同胚于等价关系$\Theta$在$A$上由$\Delta_n$导出的$A$的商（引理1）。设$B$为超平面，其方程为$\mathbf{R}^{n+1}$中的$x_0 = 1$。对于每个点$x \in A$，让对应点$x_0^{-1} x$，其中通过$0$和$x$的线切割$B$（图4）；这样，我们将$A$的定义连续映射$g$放到$B$上，这样$g(x)$是$B$中唯一与$x$模$\Theta$全等的点。由此可见 $B$ 同态于 $A/\Theta$ (引理 2)，因此也同态于 $C$；由于$B$与$\mathbf{R}^n$同胚，证明是完备的。

#### 推论{#top-vi-s3-n2-cor-1 .statement tag=0BXO}

** $\mathbf{P}_n$ 的每个点 *都有一个开邻域同构于* $\mathbf{R}^n$。

特别是，实射影空间是*局部连通的*（这也可从章 I、§ II、no. 6、命题 12 得出）。

### 3. 将实数空间嵌入投影空间

no. 2的命题 5表明，如果我们在$\mathbf{P}_n$（$n \geq 0$）中给出一个射影超平面$\mathbf{H}$，则$\mathbf{R}^n$同胚到这个超平面的补集$\mathbf{C}H$。一旦选择了 $\mathbf{H}$，通常可以方便地通过命题 5 中定义的同胚来 *认同* $\mathbf{R}^n$ 和 $\mathbf{C}H$；射影超平面 $H$ 被称为“无穷远”，它的点和子集也是如此。通常取$H$为“坐标”超平面，其方程为$x_0 = 0$；然后将$\mathbf{R}^n$的点$z = (z_1)$与齐次坐标为$1, z_1, z_2, \ldots, z_n$的$P_n$的点进行识别。

一旦完成此识别，$\mathbf{R}^n$中$p$维数的任何仿射线性簇$V$在$P_n$中的闭包是$p$维数的射影线性簇，不包含在无穷远处的超平面中，并且与由下式生成的射影线性簇相同$V$。相反，$p$ 维数的每个射影线性簇$P$（不包含在无穷远超平面中）在$\mathbf{R}^n$ 上都有一个仿射线性簇$p$ 维数，其在$P_n$ 中的闭包为$P$。

在特定情况下$n = 1$，超平面在无穷远处是点；由于 $P_1$ 是紧致的，因此从 Alexandroff 的定理 (章 I, § 9, no. 8, 定理 4) 可以得出，$P_1$ 同胚于空间 $\tilde{\mathbf{R}}$，通过紧致局部紧致空间 $\mathbf{R}$ 得到： 伴随 of 点（“无穷远的点”）。通过§ 2, no. 4的命题 4，我们还看到实射影线$P_1' \mathbf{R}$同胚于圆$S_1$和环面$T$。

另一方面，如果 $n > 1$，$P_n(\mathbf{R})$ 与 $S_n$ 不同胚，我们稍后会看到 (cf. 习题 4)。

空间 $\tilde{\mathbf{R}}$ 的“无穷远点”用$\infty$ 表示，不附加任何符号。重要的是不要将$\tilde{\mathbf{R}}$与章IV, § 4中定义的扩展实直线$\mathbf{R}$混淆，后者有两个“无穷远点”；事实上，$\tilde{\mathbf{R}}$同态于通过识别两个点$+\infty$和$-\infty$而获得的$\mathbf{R}$的商空间。

### 4. 应用于实值函数的扩张

Since $\mathbf{R}$ can be considered as a subset of $\tilde{\mathbf{R}}$, every mapping of a set $E$ into $\mathbf{R}$ (i.e. every real-valued function on $E$) can be considered as a mapping of $E$ into $\tilde{\mathbf{R}}$; in particular, if $E$ is a subset of a topological space $F$ and $f$ is a mapping of $E$ into $\mathbf{R}$, it may happen that at some points of the closure $F_c$ of $E$, $f(x)$ tends to the limit $\infty$ as $x$ tends to one of these points while remaining in $E$; we may then extend the function $f$ by continuity by assigning it the value $\infty$ at these points (Chapter I, § 8, no. 5, Theorem 1).

特别考虑$E$是$\mathbf{R}^n$的子集的情况，空间$\mathbf{R}^n$本身被认为嵌入射影空间$P_n$中；如果我们假设无穷大处的超平面是$x_0 = 0$，则定义在$E$上的实值函数$f$可以用映射来标识

$$
(x_0, x_1, x_2, \ldots, x_n) \to f \left( \frac{x_1}{x_0}, \frac{x_2}{x_0}, \ldots, \frac{x_n}{x_0} \right)
$$

将$E$转化为$\tilde{\mathbf{R}}$；根据上一段所述，可能不仅可以对扩展这个函数，不仅对$E$闭包中$\mathbf{R}^n$的一些点，而且对$E$闭包中$\mathbf{P}_n$的一些“无穷大点”。

让我们证明，对于例，扩张，通过连续到实数变量的有理函数的整个$\tilde{\mathbf{R}}$，已经在代数中定义，我们可以通过这种方式获得例，扩张。 让我们认同$\tilde{\mathbf{R}}$和$\mathbf{P}_1$，每个实数$x \in \mathbf{R}$都用点来识别，其齐次坐标是$(1, x)$。以及点 $\infty$ 和点，其齐次坐标为 $(0, 1)$。 设$u(x, y)$为有理函数，$u$和$v$分别为次数、$m$和$n$的两个互质多项式；如果我们假设例是$m \leq n$，并且如果我们放入$u_1(x, y) = x^n u(x, y)$，$v_1(x, y) = x^n v(x, y)$，则有理数函数$u/v$可以被视为限制，到实数$x$的集合，这样$v(x) \neq 0$，映射$(x, y) \to (u_1(x, y), v_1(x, y))$。 在其他字中，我们通过连续性来扩展$u/v$，通过在点$x \in \mathbf{R}$（其中$v(x) = 0$）处给出值$\infty$，并在点$\infty$值处给出它如果$m < n$则为$0$，如果$m > n$则为值$\infty$，如果$m = n$则为值。

特别是，函数$1/x$可以通过在那里取值$\infty$扩展到点$0$，通过在那里取值$0$可以扩展到$\infty$；这个扩展的函数显然是$\tilde{\mathbf{R}}$自身的同胚。当$ad - bc \neq 0$时，单应性函数$(ax + b)/(cx + d)$也是如此。

同样，如果$n$是整数$> 0$，则通过取值$\infty$，将函数$x^n$扩展变为点$\infty$。

On the other hand, it is in general impossible to extend by continuity a rational function of two real variables either to the space $\mathbf{P}_1 \times \mathbf{P}_1$ or to the space $\mathbf{P}_2$ (cf. Exercise 5).

### 5. 射影线性簇的空间

给定左射影空间$\mathbf{P}_n(K)$的射影线性簇$p \geq 0$维数的除法环$K$、集合$\mathbf{P}_{n,p}(K)$显然是一对一的对应与集合 $p - 1$ 维数向量子空间左向量空间 $K_s^{p-1}$。令$L_{s-1,s-1}(K)$表示$K_s^{p-1}$的免费系统$(x_i)_{1 \leq i \leq s-1}$$p - 1$向量集合；那么集合 $\mathbf{P}_{n,p}(K)$ 再次与 $L_{n+1,\ p+1}(K)$ 除以等价关系 $\Delta_{n,\ p}(K)$ 的商一对一对应：“ $(x^k)$ 和 $(y^k)$ 生成相同的向量子空间 $p + 1$ 维数 $K_s^{n+1}$”。接下来我们将认同$P_{n,\ p}(K)$与这个商集。另一方面，如果对于$K_s^{n+1}$的$p + 1$向量的每个空闲系统$(x_k)$，我们制作$p + 1$行的对应矩阵$X$和$n + 1$列，其中$x_k$是第k行（$1 \leq k \leq p + 1$），我们在$p + 1$行的所有矩阵和$n + 1$列的$L_{n+1,\ p+1}(K)$和集合之间有一个一对一的对应，其中秩 $p + 1$；我们将认同$L_{n+1,\ p+1}(K)$与矩阵的集合，以及两个矩阵$X, Y$之间的关系$\Delta_{n,\ p}(K)$则如下：“存在非奇异平方矩阵 $T$ 阶 $p + 1$ 使得$Y = T.X$”。

下面我们将$K$取为域$\mathbf{R}$，并省略上面记号中的字母$K$。我们可以通过推广实投影空间的拓扑的定义的过程，在$P_{n,\ p}$上得到定义拓扑。即，$p + 1$行的所有矩阵和$n + 1$列中的空间$M_{p+1,\ n+1}$包含于$L_{n+1,\ p+1}$，其中元素为实数；我们赋予$L_{n+1,\ p+1}$以拓扑，这是由矩阵空间（$\S \ 1$，no. 6）的拓扑引起的。

#### 定义 2 {#top-vi-s3-def-2 .statement tag=0BXP}

*空间$P_{n,\ p}$，即拓扑空间$L_{n+1,\ p+1}$除以等价关系$\Delta_{n,\ p}$的商，在实射影中称为$p \geq 0$维数的射影线性簇的空间空间$P_n$.*

我们将使用以下记号：给定$p + 1$行和$n + 1$列的矩阵$X$，以及任何严格递增的序列

$$
\sigma = (i_1, \ldots, i_{p+1})
$$

$p + 1$指标属于到$\mathbf{N}$的区间$[0, n]$，我们用$X_\sigma$平方表示由列构成的$X$子矩阵，其指标为$i_1, i_2, \ldots, i_{p+1}$。我们用矩阵 $X$ 中的 $L_{p+1,\ p+1}$ 由……组成中的$A_\sigma$ 子集来表示，使得 $X_\sigma$ 是非奇异的。通过 $\S \ 1$、no. 6、$A_\sigma$ 的命题 6，$M_{p+1,\ n+1}$ 中的集合是*密集开路* 集合，函数 $X \to X_\sigma^{-1}$ 是$A_\sigma$ 上的*连续*。

集合 $A_\sigma$ 的几何解释如下：令 $E_\sigma$ 为由典范基的向量 $e_i$ 生成的 $\mathbf{R}^{n+1}$ 的向量子空间，使得 $i \in \sigma$，并且让$E'_\sigma$是$e_i$生成的互补子空间，使得$i \notin \sigma$；然后说矩阵$x$属于到$A_\sigma$意味着投影在其$p + 1$行$x_k$形式的$E_\sigma$上是一个免费的系统，或者再次向量由 $x_k$ 生成的子空间是 $E'_\sigma$ 的*补码*（或者说它的交与 $E'_\sigma$ 仅由 0 组成）。

#### 命题 6 {#top-vi-s3-prop-6 .statement tag=0BXQ}

*空间 $P_{n,\ p}$ 是豪斯多夫。*

我们首先证明关系 $\Delta_{n,p}$ 是开放的。如果$U$是$L_{n+1,p+1}$中的开集合，要相对于$\Delta_{n,p}$饱和$U$，我们必须在映射$X \to T.X$下取$U$的像的并，其中$T$贯穿阶$p+1$的非奇异方阵的集合；由于每个映射都是双连续的，因此所有这些像都是开路集合，因此它们的并也是开路。

到章 I, § 8, no. 3 的命题 8 时，如果我们证明由 $\Delta_{n,p}$ 定义的 $L_{n+1,p+1} \times L_{n+1,p+1}$ 的子集 $N$ 是闭合的，则证明将是完整的。令$(X, Y)$为乘积空间的点，它位于$N$的闭包中，并让$\sigma$为指标的序列，使得$X_\sigma$是非奇异的：因为$A_\sigma$ 开，邻域 $V$ 与 $(X, Y)$ 使得对于每个对 $(X', Y') \in N \cap V$，矩阵 $X'_\sigma$ 都是非奇异的；由于$(X', Y')$趋向于$(X, Y)$，同时保持在$N$，矩阵$Y'_\sigma {X'_\sigma}^{-1}$因此趋于$T = Y_\sigma X_\sigma^{-1}$；因为我们有$Y' = (Y'_\sigma {X'_\sigma}^{-1}) X'$，所以我们从经过到极限看到$Y = T.X$，并且证明是完整的。

#### 命题 7 {#top-vi-s3-prop-7 .statement tag=0BXR}

*空间$P_{n,p}$紧凑。*

足以证明存在一个$L_{n+1,p+1}$的紧子空间，它满足至少一个点中的每个等价类 mod $\Delta_{n,p}$；因为 $P_{n,p}$ 那么是这个子空间的像在 $L_{n+1,p+1}$ 的典范映射上到 $P_{n,p}$ 上，因此是紧致的（章 I, § 9, no. 4，定理 2）。

令$V_{n+1,p+1}$为$L_{n+1,p+1}$的子空间，其元素为$p+1$向量的系统$(x_k)$，形成向量的*正交欧氏基* 子空间它们生成也就是说，每当$h \neq k$时，$(x_h/x_k) = 0$，对于$1 \leq h \leq p+1$，$(x_h/x_k) = 1$。 $p+1$ 维数 $\mathbf{R}^{n+1}$ 的每个向量子空间都有这样的基，因此每个类 mod。 $\Delta_{n,p}$ 满足 $V_{n+1,p+1}$。另一方面，$V_{n+1,p+1}$的矩阵$X = (x_{ij})$由关系定义

$$
\sum_{j=0}^n x_{ij}^2 = 1 \quad (1 \leq i \leq p+1),
$$
$$
\sum_{j=0}^n x_{ij} x_{kj} = 0 \quad (i \neq k);
$$

因此，它们在 $M_{p+1,n+1}$ 中形式 *关闭* 集合；并且由于这些关系意味着$|x_{ij}| \leq 1$对于指标$(i, j)$的每个对，因此这个集合是*有界的*，因此是*紧凑的*。

#### 命题 8 {#top-vi-s3-prop-8 .statement tag=0BXS}

$P_{n,p}$ * 是连通且局部连通的，并且每个点都有一个开邻域同构于* $\mathbf{R}^{(p+1)(n-p)}$。

对于指标$\sigma$的每个(严格递增的)序列，集合$A_\sigma$在$L_{n+1,p+1}$中开，并且相对于$\Delta_{n,p}$饱和； 典范像

因此，P_{n,p} 中的 C_σ 是开集合同态于 A_σ 与等价关系 θ_σ 的商，该商是由 Δ_{n,p} (引理 1) 在 A_σ 上导出的。

设 B_σ 为矩阵 X 的 A_σ 由……组成子集，使得 X_σ 为阶 p + 1 的单位矩阵； X中除了X_σ之外的元素是任意的，因此B_σ与空间R^{(p+1)(n-p)}同胚。对于每个矩阵 X ∈ A_σ 让我们制作对应矩阵 Y = X_σ^{-1}X，其中属于到 B_σ；那么我们定义了 A_σ 到 B_σ 上的连续映射 g，使得 g(X) 是 B_σ 中唯一与 X mod θ_σ 全等的矩阵。由此可见，B_σ 同胚于 A_σ/θ_σ (引理 2)，因此也同胚于 C_σ。

因此集合 C_σ 是连通的。由于 A_σ 在 L_{n+1,p+1} 中是稠密的，C_σ 在 P_{n,p} 中是稠密的，因此 P_{n,p} 也是连通的 (章 I, § 11, no. 1, 命题 1)。另一方面，对于指标 σ 的至少一个序列，P_{n,p} 属于的每个点到 C_σ，因此具有与 R^{(p+1)(n-p)} 同态的开邻域。

矩阵 Y = g(X) 可以解释如下：为了简单起见，让我们假设序列 σ 由 p + 1 指标 n − p, n − p + 1, ..., n 组成，并让 a_{ij} (1 ≤ i ≤ p + 1, 0 ≤ j ≤ n − p − 1) 表示y 的第一个 n − p 列的元素；那么 x 的行生成的 R^{n+1} 的向量子空间就是由方程定义的

$$
x_j = \sum_{i=1}^{p+1} a_{ij} x_{n-p+i-1} \quad (0 \leq j \leq n-p-1).
$$

### 6. 格拉斯曼尼亚人

如果K是域并且X是L_{n+1,p+1}(K)中的任意矩阵，则令c_σ(X)表示X_σ的行列式；这样，对于L_{n+1,p+1}(K) 对应的每一个矩阵X

$$
h = \binom{n+1}{p+1}
$$

行列式，不是所有零（X的p + 1行的外部乘积的分量）。如果我们将齐次坐标为 c_σ(X) 的射影空间 P_{n-1}(K) 的对应变为 X 点，我们就将 L_{n+1,p+1}(K) 的映射定义为 P_{n-1}(K)，兼容于关系 Δ_{n,p}(K); 经过为商，因此我们将 P_{n,p}(K) 的映射 f 化为 P_{n-1}(K)。这个映射下的P_{n,p}(K)的像G_{n,p}(K)称为指标n,p的格拉斯曼。我们还记得映射 f 是单射的，因为如果 X 是矩阵，使得 X_σ 是非奇异的，则 B_σ 的矩阵 Y = X_σ^{-1}X，其中 X mod 的对应到类。 Δ_{n,p}(K) 为矩阵 (d_{ij}/c_σ(X)) (1 ≤ i ≤ p + 1, 0 ≤ j ≤ n)，其中 d_{ij} 表示从 $X_{\sigma}$ 通过替换得到的矩阵的行列式$X_{\sigma}$的第$i$第列乘以$X$的第$j$第列[这意味着$d_{ij}$在符号范围内等于$c_{\tau}(X)$之一]。

当$K$为域$\mathbf{R}$时，这个映射$f$显然是*连续的*。逆矩阵映射 $g$ 也是连续的；对于矩阵属于至 $B_{\sigma}$ 的元素 ，是其对应的格拉斯曼坐标点齐次坐标的有理数函数；由于$f(B_{\sigma}) = B'_{\sigma}$是$G_{n,p}$的点的集合，其与指标$\sigma$的齐次坐标不为0，所以是$G_{n,p}$中的开集合；因此，$g$在$B'_{\sigma}$的每一个点连续，并且由于$G_{n,p}$属于的每一个点到至少一个集合$B'_{\sigma}$，$g$在每点连续。因此：

#### 命题 9 {#top-vi-s3-prop-9 .statement tag=0BXT}

*格拉斯曼* $G_{n,p}$ *同胚于空间* $P_{n,p}$。

最后我们回想一下，格拉斯曼函数$G_{n,p}(K)$和$G_{n,n-p-1}(K)$是同一个射影空间$P_{n-1}(K)$的子集，并且可以通过射影线性变换转换为另一个射影；由此可见 $G_{n,p}$ 和 $G_{n,n-p-1}$ 是*同胚*。

### 习题{#top-vi-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
