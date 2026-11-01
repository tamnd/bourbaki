---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 7
section_title: Convergence of the Hausdorff series (real or complex case)
lang: zh
source: lie-i-iii
book_pages: 164-170, 204
pdf_pages: 0182-0188, 0222-0222
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS-POLYNOMIALS WITH VALUES IN $g$
      page: 164
      pdf_page: 182
    - "no": 2
      title: GROUP GERM DEFINED BY A COMPLETE NORMED LIE ALGEBRA
      page: 165
      pdf_page: 183
    - "no": 3
      title: Exponential in Complete Normed Associative Algebras
      page: 169
      pdf_page: 187
statements: 4
exercises: 1
content_sha256: 2972a2da66626ba3e20037ed99b90d2f21ed2537ef09e3e22ee4609e6b4ce0d6
translated_from: content/en/lie/II/07_s7_convergence_of_the_hausdorff_series.md
translation_method: google
source_content_sha256: 88835ad1fbae7ef0a5c13987bac0f6fc980b84197bf24b3bc093b8842e1a4906
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 8f17d60a27dfb141222d007e65e84f1abab15e365146c79ce9d87afbd662639e
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 7。 HAUSDOFF 的收敛性级数（真实或复杂的情况）

在本段中，我们假设 $K$ 是域 $\mathbf{R}$ 或 $\mathbf{C}$ 之一，其通常的绝对值值。回想一下，$K$ 上的可规范代数是 $K$ 上的（不一定是关联的）代数和拓扑 $\mathscr{T}$，具有以下属性：
(1) $\mathscr{T}$可由范数定义：
(2) $A \times A$到$A$的映射$(x, y) \mapsto xy$是连续的。
代数超过$K$是代数$A$超过$K$和范数，使得$\|xy\| \leq \|x\|\ \|y\|$对于$A$中的所有$x, y$。
我们用$g$表示$K$上的完全可范化李代数。我们对 $g$ 和数 $M > 0$ 选择范数这样
$$
\|[x, y]\| \leq M \|x\|\ \|y\| \quad \text{for } x, y \text{ in } g.
$$

### 1. $g$ 中值的连续多项式

设 $I$ 为有限集合，并令 $P(g^I; g)$（分别为 $\hat{P}(g^I; g)$）为向量空间的*连续多项式*（分别为*形式幂级数，具有连续分量*）在 $g^I$ 和值上在$g$。回忆一下（*可微分和解析流形*，R，附录），$P(g^I; g)$的毕业为型$\mathbf{N}^I$，并且$\hat{P}(g^I; g)$是通过过滤定义的向量空间$P(g^I; g)$和拓扑的完成来识别的与$P(g^I; g)$的毕业有关。此外，$P(g^I; g)$是分级的李代数，其括号由$[f, g](x) = [f(x), g(x)]$定义，对于f, g in P(g^I; g), x \in g^I;这个李代数结构可以通过连续性扩展到$\hat{P}(g^I; g)$，并使其成为完整的Hausdorff过滤李代数。

到§ 6, no. 3的命题 2，$\hat{L}(I)$的李代数同态$\phi_I : u \mapsto \tilde{u}$到$\hat{P}(g^I; g)$映射指标i到$\mathrm{pr}_i$的不定从 $\mathrm{pr}_i \in P(g^I; g)$ 开始，所有$i \in I$。由此可知 $\tilde{u} \in P(g^I; g)$ 对应 $u \in L(I)$；更准确地说，当$u \in L(I)$时，$\tilde{u}$只是§ 2, no. 4的多项式映射$(t_i) \mapsto u((t_i))$。另一方面，显然 $\phi_I$ 与 $L(I)$ 和 $P(g^I; g)$ 的多级数兼容。如果$u = \sum_{v \in \mathbf{N}^I} u_v$，其中$u_v \in L^v(I)$代表$v \in \mathbf{N}^I$，那么

$$
\tilde{u} = \sum_{v \in \mathbf{N}^I} \tilde{u}_v, \quad \text{where } \tilde{u}_v \in P_v(g^I; g).
$$

令$u = (u_j)_{j \in J}$是$\hat{L}(I)$的元素的有限族，令$v \in \hat{L}(J)$并令$w = v \circ u$(§ 6, no. 3)。我们写$\tilde{u} = (\tilde{u}_j)_{j \in J} \in \mathfrak{g}$。然后

(2)
$$
\tilde{v} \circ \tilde{u} = (v \circ u)^{\sim}.
$$

接下来是通过 § 6, no. 3 的连续性公式 (7) 以及可微分和解析流形、R、附录、no. 6 进行扩展。

### 2. 群由完整规范定义的细菌李代数

令 $H = \sum_{r,s \geq 0} H_{r,s} \in \hat{L}(U, V)$ 为 Hausdorff 级数 (§ 6, no. 4, 定义 1)。我们将证明相应的正式幂级数

(3)
$$
\tilde{H} = \sum_{r,s \geq 0} \tilde{H}_{r,s} \in \hat{P}(g \times g, g)
$$

是收敛的（可微且解析流形，R，3.1.1）。

我们介绍以下正式的幂级数$\eta \in \mathbf{Q}[[U, V]]$

(4)
$$
\eta(U, V) = -\log(2 - \exp(U + V))
$$
(5)
$$
= \sum_{m \geq 1} \frac{1}{m} (\exp(U + V) - 1)^m
$$
(6)
$$
= \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1, \ldots, r_m \\ s_1, \ldots, s_m}} \frac{U^{r_1} V^{s_1}}{r_1!} \frac{U^{r_2} V^{s_2}}{r_2!} \cdots \frac{U^{r_m} V^{s_m}}{s_m!}.
$$

因此

(7)
$$
\eta(U, V) = \sum_{r,s \geq 0} \eta_{r,s} U^r V^s,
$$

哪里
$$
\eta_{r,s} = \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_i + s_i \geq 1}} \frac{1}{r_1! \ldots r_m! s_1! \ldots s_m!}.
$$
现在让$u$和$v$是两个正的实数，使得$u + v < \log 2$；然后$0 \leq \exp(u + v) - 1 < 1$；将$U$替换为$u$，将$V$替换为$v$，由(5)和(6)推导出级数是收敛的，上述计算意味着：
$$
\sum_{r, s \geq 0} \eta_{r,s} u^r v^s = -\log(2 - \exp(u + v)) < +\infty.
$$
令 $r, s \geq 0$ 且令 $\| \tilde{H}_{r,s} \|$ 为连续多项式 $\tilde{H}_{r,s}$ 的范数（可微且解析流形、R、附录、no. 2）。

#### 引理 1 {#lie-ii-s7-lem-1 .statement tag=0A6L}

$$
\| \tilde{H}_{r,s} \| \leq M^{r+s-1} \eta_{r,s}.
$$
令$r_i, s_i$在$\mathbf{N}$中，对于$1 \leq i \leq m$，有$s_m = 1$；我们写 $r = \sum_i r_i, s = \sum_i s_i$ 并考虑 $L(\{U, V\})$ 的以下元素：
$$
Z = \left( \left( \sum_{i=1}^{m-1} (\mathrm{ad}\ U)^{r_i} (\mathrm{ad}\ V)^{s_i} \right) (\mathrm{ad}\ U)^{r_m} \right)(V).
$$
然后是$\tilde{Z} = f \circ p$，其中$f$是$g^{r+s}$到$g$的以下$(r+s)$线性映射：
$$
(x_1, \ldots, x_r, y_1, \ldots, y_s) \mapsto (\mathrm{ad}(x_1) \circ \cdots \circ \mathrm{ad}(x_r) \circ \mathrm{ad}(y_1) \circ \cdots \circ \mathrm{ad}(y_s))(y_s)
$$
其中 $p$ 是 $g^2$ 的映射到 $g^{r+s}$ 的结果：
$$
(x, y) \mapsto (\underbrace{x, \ldots, x}_{r}, \underbrace{y, \ldots, y}_{s});
$$
因此$\| \tilde{Z} \| \leq \| f \| \leq M^{r+s-1}$（可微分和解析流形，R，附录）。将应用这些不等式与§ 6, no. 4的公式(9)右侧的各个项，我们得到：
$$
\|(H'_{r,s})\sim\|
\leq \frac{M^{r+s-1}}{r+s} \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}} \frac{1}{r_1! \ldots r_m! s_1! \ldots s_m!}.
$$
类似的论证给出
$$
\|(H''_{r,s})\sim\|
\leq \frac{M^{r+s-1}}{r+s} \sum_{m \geq 1} \frac{1}{m} \sum_{\substack{r_1 + \cdots + r_{m-1} = r-1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}} \frac{1}{r_1! \ldots r_{m-1}! s_1! \ldots s_{m-1}!}
$$

从而，由 (8)

$$
\|\tilde{H}_{r,s}\| < \eta_{r,s} \frac{M^{r+s-1}}{r+s} \leq \eta_{r,s} M^{r+s-1},
$$

这就证明了引理。

#### 命题 1 {#lie-ii-s7-prop-1 .statement tag=0A6M}

*形式幂级数* $\tilde{H}$ *是收敛的级数* (*可微分和解析流形*, R, 3.1.1); *其绝对收敛域*（*可微分和解析流形*，R，3.1.4）*包含开集合*

$$
\Omega = \left\{ (x, y) \in g \times g \mid \|x\| + \|y\| < \frac{1}{M} \log 2 \right\}.
$$

令$u, v$为两个实数$> 0$，使得$u + v < \frac{1}{M} \log 2$；那么(引理1)

$$
\text{(12)} \quad M \sum_{r,s \geq 0} \|\tilde{H}_{r,s}\| u^r v^s \\
\leq \sum_{r,s \geq 0} \eta_{r,s} M^{r+s} u^r v^s = -\log(2 - \exp M(u + v)) < +\infty
$$
由（9）。

令$h : \Omega \to g$表示由$\tilde{H}$定义的*解析函数*（*可微分且解析流形*，R，3.2.9），即由公式定义

$$
\text{(13)} \quad h(x, y) = \sum_{r,s \geq 0} \tilde{H}_{r,s}(x, y) = \sum_{r,s \geq 0} H_{r,s}(x, y) \quad \text{for } (x, y) \in \Omega.
$$

这个函数被称为 $g$ 相对于 $M$ 的 *Hausdorff 函数*（或者在不会引起混淆的情况下简称为 $g$ 的 Hausdorff 函数）。 注 $H_{r,s}(U, -U) = 0$ 如果 $r + s \geq 2$ 因此

$$
\text{(14)} \quad h(x, -x) = 0 \quad \text{for } \|x\| < \frac{1}{2M} \log 2.
$$

同样

$$
\text{(15)} \quad h(0, x) = h(x, 0) = x \quad \text{for } \|x\| < \frac{1}{M} \log 2.
$$

#### 命题 2 {#lie-ii-s7-prop-2 .statement tag=0A6N}

*让*

$$
\Omega' = \left\{ (x, y, z) \in g \times g \times g \mid \|x\| + \|y\| + \|z\| < \frac{1}{M} \log \frac{3}{2} \right\}.
$$

*如果*$(x, y, z) \in \Omega'$，*那么*

$$
\text{(16)} \quad (x, y) \in \Omega, \quad (h(x, y), z) \in \Omega, \quad (y, z) \in \Omega, \quad (x, h(y, z)) \in \Omega
$$
*和*
$$
\text{(17)} \quad h(h(x, y), z) = h(x, h(y, z)).
$$

设 $(x, y, z) \in \Omega'$；显然$(x, y) \in \Omega$和$(y, z) \in \Omega$。此外：

$$
\|h(x, y)\| \leq \sum_{r, s} \|H_{r,s}\| \|x|r\|y|s,
$$

因此由 (13)

$$
\|h(x, y)\| \leq -\frac{1}{M} \log(2 - \exp M(\|x\| + \|y\|)).
$$

现在$M(\|x\| + \|y\|) < \log \frac{3}{2} - M\|z\|$；我们写$u = \exp(M\|z\|)$；然后 $1 \leq u \leq \frac{3}{2}$ 和

$$
\begin{align*}
M(\|h(x, y)\| + \|z\|) &< -\log(2 - \exp(\log \frac{3}{2} - M\|z\|)) + M\|z\| \\
&= -\log\left(2 - \frac{3}{2u}\right) + \log u = \log \frac{2u^2}{4u - 3} \\
&= \log\left(2 + \frac{2(u - 1)(u - 3)}{4u - 3}\right) \leq \log 2.
\end{align*}
$$

我们也看到类似的$(x, h(y, z)) \in \Omega$。

现在我们证明(17)。在李代数$\hat{L}(\{U, V, W\})$，

$$
H(H(U, V), W) = H(U, H(V, W))
$$

命题 4 / § 6, no. 5。根据 no. 1、公式 (2)，我们有 $\hat{P}(g \times g \times g, g)$ 关系

$$
\tilde{H} \circ (\tilde{H} \times \mathrm{Id}_g) = \tilde{H} \circ (\mathrm{Id}_g \times \tilde{H}).
$$

通过*可微分和解析流形*，R，3.1.9，存在数$\varepsilon > 0$，使得当$\|x\|, \|y\|$和$\|z\|$为$\leq \varepsilon$时，公式(17)为真。但函数$(x, y, z) \mapsto h(h(x, y), z)$和$(x, y, z) \mapsto h(x, h(y, z))$在$\Omega'$上是解析函数，在$g$上是值（*可微且解析流形*，R，3.2.7）。由于 $\Omega'$ 已连通，并且它们重合位于 0 的邻域中，因此它们相等（*可微且解析流形*，R，3.2.5）。

上述结果意味着：

令$\alpha$为实数，使得$0 < \alpha \leq \frac{1}{3M} \log \frac{3}{2}$。让

$$
G = \{x \in g \mid \|x\| < \alpha\},
$$

$$
\Theta = \{(x, y) \in G \times G \mid h(x, y) \in G\}
$$
并且$m : \Theta \to G$是$h$至$\Theta$中的限制。然后：
(1) $\Theta$ 在 $G \times G$ 开，$m$ 解析。
(2) $x \in G$ 意味着$(0, x) \in \Theta$、$(x, 0) \in \Theta$ 和$m(0, x) = m(x, 0) = x$。
(3) $x \in G$ 意味着$-x \in G$、$(x, -x) \in \Theta$、$(-x, x) \in \Theta$ 和

$$
m(x, -x) = m(-x, x) = 0.
$$

(4) 设 x, y, z 为 G 的元素，使得 (x, y) ε θ，(m(x, y), z) ε θ，(y, z) ε θ 且 (x, m(y, z)) ε θ。然后 m(m(x, y), z) = m(x, m(y, z))。

*在其他字 (章 III, § 1) 中，如果我们写 −x = σ(x)，则四元组 (G, 0, σ, m) 是 K 上的李群胚芽。*

### 3. 完全范数结合律中的指数代数

在这个没有。我们用 A 表示一个完全规范的单位结合词代数（一般拓扑、章 IX, § 3, no. 7）。然后\|x.y\| ≤ \|x\|。 \|y\|对于 A 中的 x、y。

令 I 为有限集合，并令 $\hat{P}(A^I; A)$ 为形式幂级数的向量空间，其中连续分量在 $A^I$ 上，值在 A 中（可微分和解析流形，R， 附录, no. 5) 和代数结构通过写得到

$$
f.g = m \circ (f, g) \quad \text{for } f, g \text{ in } \hat{P}(A^I; A),
$$

其中$m : A \times A \to A$表示A上的乘法。按照no. 1中的论证并使用§ 5, no. 1的命题1，我们定义是单位代数$u \mapsto \tilde{u}$的连续同态 $\hat{A}(I)$ 变为 $\hat{P}(A^I; A)$ 映射指标 i 到 $pr_i$ 的不定；将$\hat{L}(I)$的同态扩展李代数同态转换为no. 1中定义的$\hat{P}(A^I; A)$。如果 $u = \sum_v u_v$ 和 $u_v \in A^v(I)$ 对应 $v \in \mathbf{N}^I$，则 $\tilde{u} = \sum_v \tilde{u}_v$，其中 $\tilde{u}_v$ 是多项式映射 $(t_i)_{i \in I} \mapsto u_v((t_i))$。

令$u = (u_j)_{j \in I}$为$\hat{A}(I)$的元素的有限族，令$v \in \hat{A}(J)$并写作$w = v \circ u$(§ 5, no. 1)。然后

$$
(v \circ u)^{\sim} = \tilde{v} \circ \tilde{u}.
$$

接下来通过 § 5, no. 1 的连续性公式 (2) 以及可微分和解析流形、R、附录、no. 6 进行扩展。

特别是，我们取 I = {U}、认同 A 和 $A^{(U)}$，并考虑 $\hat{P}(A; A)$ 中级数 $e(U) = \sum_{n \geq 1} U^n/n!$ 和 $l(U) = \sum_{n \geq 1} (-1)^{n-1} U^n/n$ 的像 $\tilde{e}$ 和 $\tilde{l}$。然后$\|\tilde{U}^n\| \leq 1$对于$\|x_1 \ldots x_n\| \leq \|x_1\| \ldots \|x_n\|$对于A中的$x_1, \ldots, x_n$。因此$\tilde{e}$（或$\tilde{l}$）的绝对收敛半径是无穷大（或$\geq 1$）。

我们将用$e_A$（或$l_A$）表示由收敛级数$\tilde{e}$（或$\tilde{l}$）定义的A到A（或B到A，其中B是A的开单位球）的解析映射，我们将写成$\exp_A(x) = 1 + e_A(x)$（对于$x \in A$）和

$$
\log_A(x) = l_A(x - 1)
$$

（对于 $x \in A, \|x - 1\| < 1$）。然后

$$
\exp_A x = \sum_{n \geq 0} \frac{x^n}{n!} \quad (x \in A)
$$

(20) $\log_A x = \sum_{n \geq 1} (-1)^{n-1} \frac{(x-1)^n}{n} \quad (x \in A, \|x-1\| < 1).$

作为 $(e \circ l)(U) = (l \circ e)(U) = U$ (cf. § 6, no. 1)，除以 (18) $\tilde{e} \circ \tilde{l} = \tilde{l} \circ \tilde{e} = \mathrm{Id}_A$。
因此（*可微分和解析流形*，R，3.1.9）
(21) $\exp_A(\log_A(x)) = x \quad (x \in A, \|x-1\| \leq 1)$
(22) $\log_A(\exp_A(x)) = x \quad (x \in A, \|x\| < \log 2)$
因为$\|x\| < \log 2$意味着$\|\exp_A(x) - 1\| \leq \exp \|x\| - 1 < 1$。

最后我们将 A 视为完全范数李代数。然后
$$
\|[x, y]\| = \|xy - yx\| \leq 2\|x\|\cdot\|y\|.
$$
命题 1 of no. 2 意味着形式幂级数 $\tilde{H}$ 包含集合的绝对收敛域
$$
\Omega = \{x, y) \in A \times A \mid \|x\| + \|y\| < \frac{1}{2} \log 2\}.
$$
因此 $\tilde{H}$ 定义是解析的函数 $h : \Omega \to A$。然后$h(x, y) = \sum_{r,s} H_{r,s}(x, y)$（cf.§ 3, no. 1，*注4*）。

#### 命题 3 {#lie-ii-s7-prop-3 .statement tag=0A6O}

*对于$\|x\| + \|y\| < \frac{1}{2} \log 2$，*
(23) $\exp_A x \cdot \exp_A y = \exp_A h(x, y).$
由 (18) 和关系 $e^u e^v = e^{u+v}$ 得出
$$
m \circ (1 + \tilde{e}, 1 + \tilde{e}) = (1 + \tilde{e}) \circ \tilde{H}
$$
在$\hat{P}(A \times A; A)$。因此，我们从 *可微分和解析流形*, R, 3.1.9 中推断出 (23) 对于足够接近 $(0, 0)$ 的 $(x, y)$ 成立，从而命题遵循解析延拓 (*可微分和解析流形*, R, 3.2.5）。

### 习题 {#lie-ii-s7-exercises}

参见[习题为 § 7](exercises/s7/)。
