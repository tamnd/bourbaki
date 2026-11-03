---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 4
section_title: Approximation of continuous real-valued functions
lang: zh
source: top-v-x
pdf_pages: 0314-0323, 0343-0352
extraction: ocr
subsections:
    - "no": 1
      title: APPROXIMATION OF CONTINUOUS FUNCTIONS BY FUNCTIONS BELONGING TO A LATTICE
      page: 0
      pdf_page: 314
    - "no": 2
      title: APPROXIMATION OF CONTINUOUS FUNCTIONS BY POLYNOMIALS
      page: 0
      pdf_page: 317
    - "no": 3
      title: 'APPLICATION : APPROXIMATION OF CONTINUOUS REAL-VALUED FUNCTIONS DEFINED ON A PRODUCT OF COMPACT SPACES'
      page: 0
      pdf_page: 320
    - "no": 4
      title: APPROXIMATION OF CONTINUOUS MAPPINGS OF A COMPACT SPACE INTO A NORMED SPACE
      page: 0
      pdf_page: 320
statements: 18
exercises: 21
content_sha256: bd057294683dedf4d6032a024a4fdb23076f764170075979d4ad4a53fce2fe14
translated_from: content/en/top/X/04_s4_approximation_of_continuous_real_valued.md
translation_method: google
source_content_sha256: 949d16c80adeb3bf4fa8d42aa0a09edd31bc61679863b9e79f9e89c41e063551
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 2749825ed67bce395267e734444b72907086a7f2cbc91d84b9ed36a45d196425
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 4. 连续实值函数的近似值

### 1. 将连续函数通过函数属于近似为格子

在这个截面中，我们将研究定义在*紧凑*空间$X$上的连续实值函数(*)的集合$\mathscr{C} = C(X; \mathbf{R})$，并且我们将始终假设$\mathscr{C}$被赋予*均匀收敛*的拓扑。从§ 3, no. 2我们知道这个拓扑是由范数定义的

$$
||f|| = \sup_{x \in X} |f(x)|
$$

并且这个范数与$\mathscr{C}$的$\mathbf{R}$代数结构兼容。有了这个范数和这个代数结构，$\mathscr{C}$是$\mathbf{R}$上的*完整规范的代数*（$§ 1$，no. 6，定理2，推论1）。

(*) 在此截面中考虑的实值函数假定始终是*有限*。

如果$H$是$\mathscr{C}$的子集，我们可以说$X$上的连续实值函数$f$可以统一逼近$H$的函数，如果$f$位于闭包中空间$\mathscr{C}$中的$H$，即，如果对于每个$\varepsilon > 0$，都存在函数$g \in H$，使得$|f(x) - g(x)| \leq \varepsilon$对于所有$x \in X$。说$X$上的每个连续实值函数都可以由$H$的函数统一逼近，因此意味着$H$在$\mathscr{C}$中是稠密的。

在集合$\mathscr{C}$上，关系$f \leq g$[这意味着$f(x) \leq g(x)$对于所有$x \in X$]是序关系，相对于$\mathscr{C}$是一个格子。显然我们有 $|||u| - |v||| \leq ||u - v||$，因此 $u \to |u|$ 是 $\mathscr{C}$ 的均匀连续的映射。由此可见

$$
(u, v) \to \sup (u, v) = \frac{1}{2}(u + v + |u - v|)
$$

和

$$
(u, v) \to \inf (u, v) = \frac{1}{2}(u + v - |u - v|)
$$

在 $\mathscr{C} \times \mathscr{C}$ 上均匀连续。

命题I。令$X$为紧致空间，并令$H$为在$X$上定义的连续实值函数的集合。令$f$为$X$上的连续实值函数，使得对于每个$x \in X$，存在函数$u_x \in H$，使得$u_x(x) > f(x)$[resp。 $u_x(x) < f(x)$]。那么存在函数 $u_{x_i} = f_i \in H$ ($1 \leq i \leq n$) 的有限数，这样，如果 $v = \sup(f_1, f_2, \ldots, f_n)$ [resp. $w = \inf(f_1, f_2, \ldots, f_n)$]，我们有 $v(x) > f(x)$ [分别。 $w(x) < f(x)$] 对于所有$x \in X$。

对于每个 $x \in X$，令 $G_x$ 为所有 $z \in X$ 的开集合由……组成，使得 $u_x(z) > f(z)$ [resp. $u_x(z) < f(z)$]。由于$x \in G_x$乘以假设，$X$是集合$G_x$的并，因为$x$穿过$X$。由于$X$是紧的，因此存在点$x_i$（$1 \leq i \leq n$）的有限数，使得$G_{x_i}$覆盖$X$，并且很明显函数$f_i = u_{x_i}$满足条件共命题。

定理I（迪尼）。令$X$为紧致空间，并令$H$为$X$上连续实值函数的集合，其相对于关系$\leq$（或$\geq$）有向。如果 $H$ 的上（或下）包络线 $f$ 在 $X$ 上是有限且连续的，则 $f$ 可以通过函数属于均匀逼近到 $H$（或者，等价地，$H$ 的截面滤波器收敛）统一为$X$中的$f$）。

给定任何$\varepsilon > 0$，对于每个$x \in X$，都存在函数$u_x \in H$，使得$u_x(x) > f(x) - \varepsilon$。根据命题I以及$H$相对于关系$\leq$有向，存在$g \in H$使得$g(x) > f(x) - \varepsilon$对于所有$x \in X$；另一方面，我们有$g(x) \leq f(x)$乘以定义，因此定理被证明。

#### 推论 {#top-x-s4-n1-cor-1 .statement tag=0CEW}

令$(u_n)$为$X$上连续实值函数的递增（分别为递减）序列。如果序列 $(u_n)$ 的上（或下）包络线 $f$ 在 $X$ 上是有限且连续的，则序列 $(u_n)$ 在 $X$ 中均匀收敛到 $f$。

显然，如果不再假设$X$是紧的，则定理 1的结论不再必然有效，如$\mathbf{R}_+$中函数$x/(n + x)$的递减序列的例所示。

#### 命题 2 {#top-x-s4-prop-2 .statement tag=0CEX}

令$X$为紧致空间，并令$H$为$X$上连续实值函数的集合，使得给定任意两个函数$u \in H, v \in H$、函数$\sup(u, v)$和$\inf(u, v)$为在$H$。那么 $X$ 上的连续实值函数 $f$ 可以通过函数属于统一逼近到 $H$ 当且仅当，对于每个实数 $\varepsilon > 0$ 和每个对 $x, y$ $X$的点，有函数$u_{x, y} \in H$使得$|f(x) - u_{x, y}(x)| < \varepsilon$和$|f(y) - u_{x, y}(y)| < \varepsilon$。

条件显然是必要的；让我们证明这已经足够了。对于每个$\varepsilon > 0$，我们将证明存在函数$g \in H$，使得所有$z \in X$都有$|f(z) - g(z)| < \varepsilon$。令$x$为$X$中的任意点，并令$H_x$为所有函数$u \in H$中的集合，使得$u(x) < f(x) + \varepsilon$。到假设，对于每个$y \in X$、函数、$u_{x, y}$、属于到$H_x$，我们有$u_{x, y}(y) > f(y) - \varepsilon$。因此，到命题 1，存在$H_x$的函数的有限数，其上包络$v_x$使得对于所有$z \in X$来说$v_x(z) > f(z) - \varepsilon$；另一方面，我们有 $v_x(x) < f(x) + \varepsilon$ 乘定义的 $H_x$；最后，$v_x \in H$乘假设。因此，命题 1 表明存在函数 $v_{x_i}$ 的有限数，其下包络$g$ 使得对于所有$z \in X$ 都有$g(z) < f(z) + \varepsilon$；但由于我们对所有 $z \in X$ 和每个指标 $i$ 都有 $v_{x_i}(z) > f(z) - \varepsilon$，所以我们对所有 $z \in X$ 也有 $g(z) > f(z) - \varepsilon$。由于 $g \in H$ 到假设，证明已完成。

#### 注{#top-x-s4-n1-rem-1 .statement tag=0CEY}

当集合$H$满足条件或命题2时，它是相对于排序$f \leq g$的格子。但应该注意的是，$C$的子集$H$可以是关于这种排序的格子，而不一定是两个函数$u, v$中$H$中最小的上界（分别为下确界） $H$ 与$C$ 中的最小上界（分别为下确界）相同。 \* 例由 $\mathbf{R}$ 的紧致体区间到$\mathbf{R}$ 的凸映射提供。 \*

#### 推论 {#top-x-s4-n1-cor-2 .statement tag=0CEZ}

假设$H$是这样的，每当$u \in H$和$v \in H$时，我们就有$\sup(u, v) \in H$和$\inf(u, v) \in H$；并且是这样的，给定$X$的任何两个不同的点$x, y$和任何两个实数$\alpha, \beta$，存在函数$g \in H$使得$g(x) = \alpha$和$g(y) = \beta$。那么$X$上的每个连续实值函数都可以由函数属于统一逼近到$H$。

#### 定义 1 {#top-x-s4-def-1 .statement tag=0CF0}

*如果X是任何集合，X的映射的集合H到集合Y被认为是分离X的子集A的元素（或者是分离集合 A 的元素) 如果给定 A 的任何两个不同的元素 x, y，则有函数 f ∈ H 使得 f(x) ≠ f(y)。*

例如，如果 X 是完全正则空间 (章 IX, § 1, no. 5)，则 X 的所有连续映射的集合将 X 的点分开。

#### 定理 2（石头）{#top-x-s4-thm-2 .statement tag=0CF1}

*设X为紧空间，并令H为$\mathscr{C}(X; \mathbf{R})$的向量子空间，使得1)常数函数属于为H； 2) 如果$u \in H$，则$|u| \in H$； 3) H 分隔点和 X。那么X上的每个连续实值函数都可以用H的函数统一逼近。*

只要证明H满足推论到命题2的条件就足够了。到假设，如果$u \in H$和$v \in H$，我们有

$$
\sup (u, v) = \frac{1}{2} (u + v + |u - v|) \in H
$$
和
$$
\inf (u, v) = \frac{1}{2} (u + v - |u - v|) \in H.
$$

另一方面，令x和y为X中任意两个不同的点，并令α、β为任意两个实数。到假设，有函数$h \in H$，这样$h(x) \neq h(y)$：比如说$h(x) = \gamma$和$h(y) = \delta$。由于常数属于到 H，函数
$$
g(z) = \alpha + (\beta - \alpha) \frac{h(z) - \gamma}{\delta - \gamma}
$$
属于到 H 并且使得 $g(x) = \alpha$ 和 $g(y) = \beta$。

### 2. 用多项式逼近连续函数

给定在集合 X 上定义的实值函数的集合 H，我们说在 X 上定义的实值函数是一个具有实数的多项式（分别是没有常数项的多项式） 系数，在 H 的函数中，如果它是形式 $x \to g(f_1(x), f_2(x), \ldots, f_n(x))$，其中 g 是 n 个不定式（n 任意）且实数系数的多项式（分别是没有常数项的多项式），并且 $f_i$ ($1 \leq i \leq n$) 属于至 H.

#### 定理 3（威尔斯特拉斯石）{#top-x-s4-thm-3 .statement tag=0CF2}

*令X为紧致空间，并令H为X上连续实值函数的集合，它将点与X分开。那么X上的每个连续实值函数都可以通过H的函数中的多项式（具有实数系数）统一逼近。*

定理的等价叙述是*$\mathscr{C}(X; \mathbf{R})$的任何子代数，其中包含常量函数并分隔X的点在$\mathscr{C}(X; \mathbf{R})$*中是稠密的。

令$H_0$为H的函数中所有多项式的集合，令$\overline{H}_0$为$\mathscr{C}$中$H_0$的闭包。如果 g 是 n 个变量中具有实数系数的任意多项式，则 $(u_1, u_2, \ldots, u_n) \to g(u_1, u_2, \ldots, u_n)$ 是 $\mathscr{C}^n$ 到 $\mathscr{C}$ 的连续映射，其中映射 $H_0^n$ 到 $H_0$，因此映射 $\overline{H}_0^n$ 变为 $\overline{H}_0$（章 I, § 2, no. 1、定理 1）。特别地，$\overline{H}_0$是$\mathscr{C}$的向量子空间，显然满足定理2的第一个和第三个条件；我们将证明它也满足第二个条件，这将证明$\overline{H}_0 = \mathscr{C}$。

由于每个函数$u \in \overline{H}_0$都有界于$X$，因此足以证明以下引理：

#### 引理 1 {#top-x-s4-lem-1 .statement tag=0CF3}

*对于每个实数$\varepsilon > 0$和每个紧凑区间$I \subset \mathbf{R}$，都存在一个多项式$p(t)$，没有常数项，使得$|p(t) - |t|| \leq \varepsilon$对于所有$t \in I$。*

证明形式 $I = [-a, +a]$ 的区间引理就足够了，因此，替换 $t$ $at$，区间 $I = [-1, +1]$。由于 $|t| = \sqrt{t^2}$，引理 1 是以下结果的推论：

#### 引理 2 {#top-x-s4-lem-2 .statement tag=0CF4}

*令 $(P_n)$ 为没有常数项定义的多项式的序列*
$$
(1) \quad p_0(t) = 0, \quad p_{n+1}(t) = p_n(t) + \frac{1}{2} (t - (p_n(t))^2), \qquad n \geq 0.
$$
*在区间 $[0, 1]$ 序列 $(p_n)$ 中，递增一致收敛到 $\sqrt{t}$。*

为了证明引理 2 就足以证明，对于所有 $t \in [0, 1]$，我们有
$$
(2) \qquad 0 \leq \sqrt{t} - p_n(t) \leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}},
$$
(2) 意味着 $0 \leq \sqrt{t} - p_n(t) \leq 2/n$。

我们通过$n$上的归纳证明(2)。对于 $n = 0$ 来说也是如此。如果$n \geq 0$，则从归纳假设（2）得出$0 \leq \sqrt{t} - p_n(t) \leq \sqrt{t}$，因此$0 \leq p_n(t) \leq \sqrt{t}$，因此从（1）我们有
$$
\sqrt{t} - p_{n+1}(t) = (\sqrt{t} - p_n(t)) (1 - \frac{1}{2} (\sqrt{t} + p_n(t))),
$$
使得 $\sqrt{t} - p_{n+1}(t) \geq 0$，并且从 (2)
$$
\begin{align*}
\sqrt{t} - p_{n+1}(t) &\leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2} \right) \\
&\leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2 + (n+1) \sqrt{t}} \right) \\
&= \frac{2 \sqrt{t}}{2 + (n+1) \sqrt{t}}.
\end{align*}
$$
Q.E.D.

如果$X$不是紧的，定理3的结论不一定成立。例如，$\mathbf{R}$上的连续实值函数是有界且非常数不能，可以通过多项式在$\mathbf{R}$中统一近似（cf.习题6）。

#### 命题 3 {#top-x-s4-prop-3 .statement tag=0CF5}

*设*$(K_i)_{i \in I}$*为*$\mathbf{R}$、$K = \prod_{i \in I} K_i$*其乘积*的紧凑区间族，并令$X$*为*$K$的紧凑子空间。 *则* $X$ 上的每一个连续实值函数 *都可以用坐标* $x_i = \mathrm{pr}_i x$ 上的多项式统一逼近。

因为如果$x = (x_i)$和$y = (y_i)$是$X$的两个不同的点，则至少有一个指标$i$使得$x_i \neq y_i$；因此，连续函数$\mathrm{pr}_i$的族满足条件或定理3。

#### 命题 4 {#top-x-s4-prop-4 .statement tag=0CF6}

*设* $X$ *为紧空间，让* $A$ *为* $X$的闭子空间，*并令* $H$ *为集合在* $X$ *上的连续实值函数 *将其分开* $C_A$ *的点 *并且使得* $A$ *是集合* $\overline{u}^{-1}(0)$ *的交 *作为* $u$ *贯穿* $H$。 *则* $X$ *上的每个连续实值函数 *即* $A$ *上的零 *都可以通过* $H$的函数中没有常数项的多项式统一逼近。

首先考虑$A$由单个点$x_0$组成的特殊情况。然后，假设意味着 $H$ 分离点和 $X$；因为，如果$x \neq x_0$，那么到假设就有函数$u \in H$使得$u(x) \neq 0 = u(x_0)$。因此，对于每个$\varepsilon > 0$和$X$上的每个连续实值函数$f$，使得$f(x_0) = 0$，存在（定理3）一个$H$的函数中的多项式$g$，使得$|f(x) - g(x)| \leq \varepsilon$对于所有$x \in X$。特别是$|g(x_0)| \leq \varepsilon$，所以

$$
|f(x) - (g(x) - g(x_0))| \leq 2\varepsilon
$$

对于所有$x \in X$；由于$g(x) - g(x_0)$是$H$的函数多项式，没有常数项，因此在这种情况下结果成立。

在一般情况下，考虑$X$上的等价关系$R$，其类为集合$A$，集合$\{x\}$为$x \notin A$。 商空间 $X/R$ 是 Hausdorff (章 I, § 8, no. 6, 命题 15)，因此是紧凑的。令$\varphi : X \to X/R$为典范映射。 $X$上的每个连续实值函数$f$在$A$消失都可以写成形式$f = f_1 \circ \varphi$，其中$f_1$是$X/R$上的连续实值函数在点消失$x_0' = \varphi(A)$。 应用的结果已经证明给空间$X/R$和点$x_0'$，我们得到最终的结果。

### 3. 应用：在紧凑空间的乘积上定义的连续实值函数的近似

#### 定理 4 {#top-x-s4-thm-4 .statement tag=0CF7}

设 $(X_i)_{i \in I}$ 为紧空间族，并令
$$
X = \prod_{i \in I} X_i.
$$
那么$X$上的每个连续实值函数都可以由形式的函数的有限数的和统一近似
$$
(x_i) \to \prod_{\alpha \in J} u_\alpha(x_\alpha),
$$
其中$J$是$I$的（任意）有限子集，$u_\alpha$是每个$\alpha \in J$在$X_\alpha$上的连续实值函数。

考虑“一个变量的函数”$(x_i) \to u_\alpha(x_\alpha)$（任何$\alpha \in I$）的集合$H$，它们在$X$上连续。这个集合分隔了$X$的点，因为如果$x = (x_i)$和$y = (y_i)$是$X$的任意两个不同的点，则存在$\alpha \in I$使得$x_\alpha \neq y_\alpha$并且存在连续实值函数 $h_\alpha$ 于$X_\alpha$，使得 $h_\alpha(x_\alpha) \neq h_\alpha(y_\alpha)$。 函数$x \to h_\alpha(\operatorname{pr}_\alpha x)$，然后属于到$H$，并在$x$和$y$取不同的值。由于$H$的函数中的每个多项式都是定理中所述的形式，因此结果由定理3得出。

如果不是所有$X_i$都是紧的，定理4的结论不一定有效（cf.习题9）。

### 4. 将紧致空间的连续映射近似为标准化空间

令 $X$ 为紧致空间，令 $Y$ 为域 $\mathbf{R}$ (章 IX, § 3) 上的规范向量空间； 空间 $C(X; Y)$ 将始终被假定携带由范数 $\|u\| = \sup_{x \in X} \|u(x)\|$ ($§ 3$, no. 2) 定义的一致收敛性拓扑。

给定在$X$上定义的连续实值函数的集合$H$，函数属于到$H$的有限族$(u_i)_{1 \leq i \leq n}$，以及点的有限族$(a_i)_{1 \leq i \leq n}$ $Y$：$X$到$Y$的映射$x \to \sum_{i=1}^n a_i u_i(x)$则连续；我们用$\sum_{i=1}^n a_i u_i$来表示，我们说它是$H$中的函数中的线性组合和$Y$中的系数。我们说，连续的映射 $f : X \to Y$ 可以通过 $H$ 的函数的线性组合统一近似（系数在 $Y$ 中），如果 $f$ 位于向量子空间的闭包中由这些线性组合组成$C(X; Y)$。

#### 命题 5 {#top-x-s4-prop-5 .statement tag=0CF8}

令$X$是一个紧凑的空间，$Y$是$\mathbf{R}$和$H$子集上$\mathscr{C}(X; \mathbf{R})$的规范空间。如果$X$上的每一个连续实值函数都可以用$H$的函数统一逼近，那么$X$到$Y$的每一个连续映射$f$都可以用线性组合统一逼近$H$ 中的函数，$Y$ 中包含系数。

给定任何实数$\varepsilon > 0$，对于每个$x \in X$，都存在$x$的开邻域，其中$f$的振荡为$\leq \varepsilon$。因此，存在$X$的有限开覆盖​​$(A_i)_{1 \leq i \leq n}$，使得$f$在每个$A_i$中的振荡为$\leq \varepsilon$。令$a_i$为$A_i$（$1 \leq i \leq n$）中$f$的值，并令$(u_i)_{1 \leq i \leq n}$为单位元的连续划分，从属于覆盖$(A_i)$（章IX, § 4, no. 4， 推论至命题 4)。令$x$为$X$中的任意点。对于每个指标$i$使得$x \notin A_i$，我们有$u_i(x) = 0$，并且对于每个指标$i$使得$x \in A_i$我们有$\|f(x) - a_i\| \leq \varepsilon$;由此可见

$$
\left\| f(x) - \sum_{i=1}^n a_i u_i(x) \right\| = \left\| \sum_{i=1}^n (f(x) - a_i) u_i(x) \right\| \leq \varepsilon \sum_{i=1}^n u_i(x) = \varepsilon.
$$

另一方面，到假设时，有函数 $v_i \in H$ 使得

$$
|u_i(x) - v_i(x)| \leq \frac{\varepsilon}{\sum_{j=1}^n \|a_j\|}
$$

对于所有 $x \in X$ ($1 \leq i \leq n$)；因此我们有

$$
\left\| f(x) - \sum_{i=1}^n a_i v_i(x) \right\| \leq 2\varepsilon \quad \text{for all } x \in X,
$$

证明已完成。

从命题 5 可以得出结论，对于命题中的每一个，我们已经证明$\mathscr{C}(X; \mathbf{R})$的某个子集$H$是稠密的，对应有一个类似的命题，用于将$X$的连续映射转换为任意范数空间$Y$。我们将仅显式地写出命题和对应以这种方式到定理 3。给定 $X$ 上实值函数的集合 $H$，$H$ 函数中的多项式， $Y$中的系数，被定义为函数属于到$H$的有限（可能为空）族中的乘积中的任意线性组合，$Y$中包含系数。然后：

#### 命题 6 {#top-x-s4-prop-6 .statement tag=0CF9}

令$X$为紧致空间，令$H$为$X$上连续实值函数的集合，它分隔$X$的点。然后，$X$的每个连续映射到$\mathbf{R}$上的标准化空间$Y$都可以通过$H$的函数中的多项式与$Y$中的系数一致近似。

由此我们推论：

#### 命题 7 {#top-x-s4-prop-7 .statement tag=0CFA}

令$X$为紧致空间，并令$H$为$X$上连续复值函数的集合，它分隔点与$X$。然后，$X$的每个连续映射到$\mathbf{C}$上的标准化空间$Y$都可以通过函数$f \in H$及其共轭$\overline{f}$中的多项式统一近似系数在$Y$。

我们只需注意，$Y$也是$\mathbf{R}$之上的规范空间，以及实部部分的应用命题6到集合和函数$f \in H$的虚部部分，使用公式

$$
\Re f = \frac{1}{2} (f + \overline{f}), \quad \Im f = \frac{1}{2i} (f - \overline{f}).
$$

#### 推论 1 {#top-x-s4-prop-7-cor-1 .statement tag=0CFB}

如果$X$是空间$\mathbf{C}^n$的紧凑子集，则$X$的每个连续映射$(z_1, z_2, \ldots, z_n) \to f(z_1, z_2, \ldots, z_n)$到域$\mathbf{C}$上的规范空间$Y$可以统一近似为$z_k$ 和 $\overline{z}_k$ 中的多项式以及 $Y$ 中的系数。

稍后我们将看到，一般来说，即使是 $Y = \mathbf{C}$，也不可能仅通过变量 $z_k$ 中的多项式（$Y$ 中的系数）统一近似 $f$。

#### 推论 2 {#top-x-s4-prop-7-cor-2 .statement tag=0CFC}

令$X$为局部紧致空间，并令$C_0(X)$为$X$到$\mathbf{C}$的连续映射的规范$\mathbf{C}$代数，其在无穷大趋于0。令$A$为$C_0(X)$的子代数，它将点与$X$分开，并且使得(i)每当$f \in A$时就有$\overline{f} \in A$，(ii)对于每个$x \in X$，有一个$f \in A$使得$f(x) \neq 0$。那么$A$在$C_0(X)$中是稠密的。

如果$X'$是点在无穷远$\omega$与$X$邻接而得到的紧空间，则$C_0(X)$可以等同于连续映射的$C(X; \mathbf{C})$由……组成的子空间，其消失于映射 $\omega$、范数 on $C_0(X)$ 定义为

$$
\|f\| = \sup_{x \in X} |f(x)| = \sup_{x \in X} |f(x)|.
$$

凭借命题 7，每个$f \in C_0(X)$都可以由函数属于至$A$内的复数系数多项式统一逼近；而且，从$f(\omega) = 0$开始，no. 2、命题 4 的论证表明，我们可以假设这些多项式没有常数项，然后它们属于到$A$。

另一个命题 7 的应用如下：

#### 命题 8 {#top-x-s4-prop-8 .statement tag=0CFD}

令P为$\mathbf{R}^m$到$\mathbf{C}$的所有周期连续映射的集合，其周期为包含$\mathbf{Z}^m$的群。那么对于 P 的每个函数属于都可以在 $\mathbf{R}^m$ 中用线性组合均匀逼近，其中复数系数，函数形式

$$
(x_1, x_2, \ldots, x_m) \to e(h_1 x_1 + h_2 x_2 + \cdots + h_m x_m),
$$

其中$h_i$是有理整数（这样的线性组合称为m变量的三角多项式）。

我们只需观察 P（赋予一致收敛的拓扑）与紧空间$\mathbf{T}^m$的所有连续映射到$\mathbf{C}$（章VII, § 1, no. 6）的空间规范同构，并且将$\mathbf{T}^m$的映射的应用命题7至集合转换为$\mathbf{C}$，其中对应将$\mathbf{R}^m$的映射$(x_1, x_2, \ldots, x_m) \to e(x_i) \quad (1 \leq i \leq m)$转换为$\mathbf{C}$。

### 习题{#top-x-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
