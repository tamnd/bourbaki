---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 8
section_title: Convergence of the Hausdorff series (ultrametric case)
lang: zh
source: lie-i-iii
book_pages: 170-176, 205-207
pdf_pages: 0188-0194, 0223-0225
extraction: ocr
subsections:
    - "no": 1
      title: $p$-adic upper bounds of the series exp, log and $\mathbf{H}$
      page: 171
      pdf_page: 189
    - "no": 2
      title: NORMED LIE ALGEBRAS
      page: 172
      pdf_page: 190
    - "no": 3
      title: GROUP DEFINED BY A COMPLETE NORMED LIE ALGEBRA
      page: 172
      pdf_page: 190
    - "no": 4
      title: EXPONENTIAL IN COMPLETE NORMED ASSOCIATIVE ALGEBRAS
      page: 174
      pdf_page: 192
statements: 9
exercises: 4
content_sha256: 34e7ee52cd6c6397aeeb129b048196d226d1211a8c13e7857ce228f44f771005
translated_from: content/en/lie/II/08_s8_convergence_of_the_hausdorff_series.md
translation_method: google
source_content_sha256: 4e23a56fb861bed945b01d7c816d0a6e594b96b17aad3c28c11640248838980a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: c64dea22c022d5a22195a17804ae4574ec063b0baed627cbc2c7679f71a91111
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 8。 HAUSDOFF 的收敛性级数（超度量情况）

在本段中，我们假设 K 是特征零* 的非离散*完整值域，具有*超度量*绝对值值。我们用$p$表示K的剩余类域的特征（*交换代数*，章VI, § 3, no. 2）。
如果$p \neq 0$，我们写$a = |p|$；我们知道（*交换代数*，章VI, § 6，第 2 和第 3 个）$0 < a < 1$，并且存在一个且只有一个对 K 的评估$v$，$\mathbf{R}$ 中的值，其限制到 $\mathbf{Q}$ 是$p$-adic 估值$v_p$，对于所有$x \in K$，$|x| = a^{v(x)}$。我们还写：
(1) $\theta = \frac{1}{p-1}.$

如果$p = 0$，我们用$a$实数表示$0 < a < 1$，并用$v$表示对$\mathbf{K}$的评估，值在$\mathbf{R}$中，使得$|x| = a^{v(x)}$对于所有$x \in \mathbf{K}$（*loc.引用。*）。然后$v(x) = 0$换$x \in \mathbf{Q}^*$。我们还写：
$$
\theta = 0.
$$

### 1. 级数 exp、log 和 $\mathbf{H}$ 的 $p$-adic 上界

*在此编号中。我们假设 $p \neq 0$.*

#### 引理 1 {#lie-ii-s8-lem-1 .statement tag=0A6Q}

*令$n$为整数$\geqslant 0$，并令$n = n_0 + n_1 p + \cdots + n_k p^k$与$0 \leqslant n_i \leqslant p - 1$一起成为$n$的$p$进数展开。让$S(n) = n_0 + n_1 + \cdots + n_k$。然后*
$$
v_p(n!) = \frac{n - S(n)}{p - 1}.
$$
整数 $i$ 的 $v_p(n!) = \sum_{i=1}^n v_p(i)$ 和数在 1 和 $n$ 之间，其中 $v_p(i) \geqslant j$ 等于 $n/p^j$ 的积分部分 $[n/p^j]$。然后
$$
v_p(n!) = \sum_{j \geqslant 0} j ([n/p^j] - [n/p^{j+1}]) = \sum_{j \geqslant 1} [n/p^j].
$$
如下$[n/p^j] = \sum_{i \geqslant j} n_i p^{i-j}$，引理。

#### 引理 2 {#lie-ii-s8-lem-2 .statement tag=0A6R}

每整数 $n \geqslant 1$ $v(n) \leqslant v(n!) \leqslant (n - 1)\theta$ 和 $v(n) \leqslant (\log n)/(\log p)$。
$v(n!) = v_p(n!) = (n - S(n))\theta \leqslant (n - 1)\theta$ 引理 1。
另一方面，$n \geqslant p^{v(n)}$、从而$v(n) \leqslant (\log n)/(\log p)$。
令$I = \{ U, V \}$为两个元素中的集合，并令
$$
\mathbf{H} = \sum_{r,s \geqslant 0} H_{r,s}(U, V) \in \hat{\mathbf{L}}_{\mathbf{Q}}(I)
$$
是 Hausdorff 级数 (§ 6, no. 4, 定义 1)。令$\mathbf{Z}_{(p)}$相对于素理想$(p)$为$\mathbf{Z}$的局部环，并且在$\mathbf{Z}$上$\mathbf{L}_{\mathbf{Z}_{(p)}}(I)$为$(e_b)_{b \in B}$基（§ 2, no. 11，定理1）。也是$\mathbf{L}_{\mathbf{Q}}(I)$超过$\mathbf{Q}$的基。

#### 命题 1 {#lie-ii-s8-prop-1 .statement tag=0A6S}

*令$r$和$s$为两个整数$\geqslant 0$。如果 $H_{r,s} = \sum_{b \in B} \lambda_b e_b$（其中 $\lambda_b \in \mathbf{Q}$）相对于基 $(e_b)_{b \in B}$ 是 $\mathbf{H}$ 的分解，则*
$$
v_p(\lambda_b) \geqslant -(r + s - 1)\theta \quad \text{for all } b \in B.
$$
环$\mathbf{A}_{\mathbf{Z}_{(p)}}(I)$与字$w \in \mathrm{Mo}(I)$生成的$\mathbf{A}_{\mathbf{Q}}(I)$的子$\mathbf{Z}_{(p)}$模块进行标识。由于$\mathbf{L}_{\mathbf{Z}_{(p)}}(I)$是$\mathbf{A}_{\mathbf{Z}_{(p)}}(I)$中的直因子，
$$
\mathbf{L}_{\mathbf{Z}_{(p)}}(I) = \mathbf{A}_{\mathbf{Z}_{(p)}}(I) \cap \mathbf{L}_{\mathbf{Q}}(I).
$$

令$f$为整数，使得$f \leq (r + s - 1)\theta < f + 1$。对于所有 $b \in B$，关系 (4) 相当于 $v_p(\lambda_b) \geq -f$，即 $H_{r,s} \in p^{-f}L_{\mathbf{Z}(p)}$。但这也等价于 (5) 到 $H_{r,s} \in p^{-f}A_{\mathbf{Z}(p)}(I)$。

通过§ 6, no. 4的公式(11)，足以证明，对于每个整数$m \geq 1$和所有整数$r_1, \ldots, r_m, s_1, \ldots, s_m$，这样
$$
r_1 + \cdots + r_m = r, \quad s_1 + \cdots + s_m = s,
$$
$$
r_i + s_i \geq 1 \quad \text{for } 1 \leq i \leq m,
$$
我们有
$$
v_p(m!r!\ldots r_m!s_1!\ldots s_m!) \leq f.
$$
但是引理2、$v_p(r_i!s_i!) \leq (r_i + s_i - 1)\theta$和$v_p(m!) \leq v_p(m!) \leq (m - 1)\theta$；因此，(7) 的左侧的边界为
$$
\theta(m - 1 + \sum_{i=1}^m (r_i + s_i - 1)) = \theta(r + s - 1);
$$
因为它是整数，所以它是$\leq f$，从而完成了证明。

### 2.规范李代数

#### 定义 1 {#lie-ii-s8-def-1 .statement tag=0A6T}

*K* 上的李代数范数为李代数和范数，使得
$$
\|x + y\| \leq \sup(\|x\|, \|y\|)
$$
$$
\|[x, y]\| \leq \|x\| \cdot \|y\|
$$
对于$g$中的所有$x, y$。

*在本段的其余部分中，g 表示完整的标准化李代数。*

对于每个有限的集合I，我们定义就像§ 7, no. 1一样，将$\hat{L}(I)$的连续李代数同态$u \mapsto \tilde{u}$变成$\hat{P}(g^I; g)$。我们在§ 7中看到，如果$u = \sum_v u_v$，其中$u_v \in L^v(I)$代表$v \in \mathbf{N}^I$，则$\tilde{u} = \sum_v \tilde{u}_v$，其中$\tilde{u}_v$是在§ 2, no. 4中定义的多项式映射$(t_i)_{i \in I} \mapsto u_v((t_i))$。 合成公式 (2) of § 7, no. 1，仍然有效。

### 3. 群由完整规范李代数定义

令 $H = \sum_{r, s \geq 0} H_{r,s} \in \hat{L}(\{U, V\})$ 为 Hausdorff 级数 (§ 6, no. 4, 定义 1)。我们将证明相应的形式幂级数具有连续成分
$$
\tilde{H} = \sum_{r, s \geq 0} \tilde{H}_{r,s} \in \hat{P}(g \times g, g)
$$
是收敛的（*可微且解析流形*，R，4.1.1）。

令 $r \geq 0, s \geq 0$ 满足 $r + s \neq 0$，并令 $\| \tilde{H}_{r,s} \|$ 为连续多项式 $\tilde{H}_{r,s}$ 的范数（可微且解析流形、R、附录、no. 2）。

#### 引理 3 {#lie-ii-s8-lem-3 .statement tag=0A6U}

$$
\| \tilde{H}_{r,s} \| \leq a^{-(r+s-1)\theta}.
$$

令B为相对于I的大厅集合，并令$H_{r,s} = \sum_{b \in B} \lambda_b e_b$为$H_{r,s}$相对于相应的基的分解为$L(\{U, V\})$。然后
$$
|\lambda_b| \leq a^{-(r+s-1)\theta}.
$$
这对于$p = 0$、对于$\lambda_b \in \mathbf{Q}$来说是微不足道的；它是从命题 1 of no. 1 得出$p \neq 0$。

而且，
$$
\| \tilde{e}_b \| \leq 1 \quad \text{for } b \in B.
$$
我们通过$n$上的归纳更一般地表明，对于两个不定U和V（§ 2, no. 6）中次数$n$的每个交替$b$，$\| \tilde{b} \| \leq 1$。如果$n = 1$，$\tilde{b}$是$g \times g$到$g$的投影之一，因此是范数$\leq 1$；如果$n > 1$，则存在次数$< n$的两个替代$b_1$和$b_2$，使得$b = [b_1, b_2]$。由于$g \times g$到$g$的映射$\gamma : (x, y) \mapsto [x, y]$是范数$\leq 1$的双线性，我们有（可微分和解析流形，R，附录，no. 4）
$$
\| \tilde{b} \| = \| \gamma \circ (\tilde{b}_1, \tilde{b}_2) \| \leq \| \tilde{b}_1 \| \cdot \| \tilde{b}_2 \| \leq 1.
$$
关系 (11) 和 (12) 意味着引理。

#### 命题 2 {#lie-ii-s8-prop-2 .statement tag=0A6V}

形式幂级数 $\tilde{H}$ 是收敛的级数（可微分和解析流形，R，4.1.1）。如果 G 是球 $\{ x \in g \mid \| x \| < a^\theta \}$，则$\tilde{H}$ 的绝对收敛域（可微分和解析流形，R，4.1.3）包含 $G \times G$。

如果$u$和$v$是两个实数$> 0$使得$u < a^\theta$和$v < a^\theta$，那么(引理3)
$$
\| \tilde{H}_{r,s} \| u^r v^s \leq a^\theta (u a^{-\theta})^r (v a^{-\theta})^s
$$
当$r + s$趋于无穷大时，$\| H_{r,s} \| u^r v^s$趋于0。

我们用$h : G \times G \to g$表示由$\tilde{H}$定义的解析函数（可微分和解析流形，R，4.2.4），即公式
$$
h(x, y) = \sum_{r, s \geq 0} \tilde{H}_{r,s}(x, y) = \sum_{r, s \geq 0} H_{r,s}(x, y) \quad \text{for } (x, y) \in G \times G.
$$
这个函数称为$g$的Hausdorff函数。

让$(x, y) \in G \times G$。然后
$$
\| \tilde{H}_{r,s}(x, y) \| \leq \sup(\| x \|, \| y \|) \\
\| h(x, y) \| \leq \sup(\| x \|, \| y \|).
$$

(17) 紧随 (16) 而来，并且 (16) 对于 $r = s = 0$ 来说是微不足道的；如果$r \geq 1$，那么
$$
\| \tilde{H}_{r,s}(x, y) \| \leq \| \tilde{H}_{r,s} \| \| x \|^{r} \| y \|^{s}
$$
$$
\leq \| x \| \left( \frac{\| x \|}{a^{\theta}} \right)^{r-1} \left( \frac{\| y \|}{a^{\theta}} \right)^{s}
$$
$$
\leq \| x \|;
$$
如果$s \geq 1$，我们也有类似的争论。

特别是，$\| h(x, y) \| < a^{\theta}$对应$(x, y) \in G \times G$。

#### 命题 3 {#lie-ii-s8-prop-3 .statement tag=0A6W}

*设$G$为球$\{ x \in g | \| x \| < a^{\theta} \}$。解析映射*
$$
h : G \times G \to G
$$
*将$G$变成群，其中$0$是单位元素，$-x$是所有$x \in G$的$x$的逆。此外，如果$R$是实数使得$0 < R < a^{\theta}$，球*
$$
\{ x \in g | \| x \| < R \}
$$
*（分别为 $\{ x \in g | \| x \| \leq R \}$）是 $G$* 的开放子群。

作为$H(U, -U) = 0$和$H(0, U) = H(U, 0) = U$，$h(x, -x) = 0$和
$$
h(0, x) = h(x, 0) = x
$$
对于所有$x \in G$。因此还有待证明结合性公式
$$
h(h(x, y), z) = h(x, h(y, z)) \quad \text{for } x, y, z \text{ in } G.
$$
作为
$$
H(H(U, V), W) = H(U, H(V, W))
$$
在 $\hat{L}(\{ U, V, W \})$ (§ 6, no. 5, 命题 4) 中，我们有
$$
\tilde{H} \circ (\tilde{H} \times \mathrm{Id}_g) = \tilde{H} \circ (\mathrm{Id}_g \times \tilde{H})
$$
在 $\hat{P}(g \times g \times g; g)$ (no. 2) 和 (19) 中通过 (16) 隐含 (18) 和 *可微分和解析流形*, R, 4.1.5。

*在其他字（章III, § 1）中，$G$与豪斯多夫函数是李群。*

### 4. 完全范数结合指数代数

在这个没有。 A 将表示单位结合词代数与范数 $x \mapsto \| x \|$ 满足条件：
$$
\| x + y \| \leq \sup(\| x \|, \| y \|) \\
\| xy \| \leq \| x \| \cdot \| y \| \\
\| 1 \| = 1
$$

对于$A$中的$x, y$，并用这个范数*完备的*。 § 7, no. 3第二段和第三段的结果仍然有效。

我们取$I = \{ U \}$并考虑$\hat{P}(A; A)$中级数$e(U) = \sum_{n \geq 1} \frac{U^n}{n!}$和$l(U) = \sum_{n \geq 1} (-1)^{n-1} \frac{U^n}{n}$的像$\tilde{e}$和$\tilde{l}$。然后：

$$
\left\| \left( \frac{U^n}{n!} \right)^{\sim} \right\| \leq a^{-(n-1)\theta}
$$
$$
\left\| \left( \frac{U^n}{n} \right)^{\sim} \right\| \leq a^{-\frac{\log n}{\log p}}
$$

引理 2 / no. 1。因此，级数$\tilde{e}$（分别$\tilde{l}$）的*绝对收敛半径*是$\geq a^\theta$（分别$\geq 1$）（*可微分和解析流形*，R，4.1.3）。对于$R > 0$，设$G_R = \{ x \in A \mid \|x\| < R \}$；我们写$G = G_0$。 级数$\tilde{e}$（分别$\tilde{l}$）定义将$G$（分别$G_1$）解析为$A$的映射$e_A$（分别$l_A$）。我们写：
$$
\exp_A(x) = 1 + e_A(x) = \sum_{n \geq 0} \frac{x^n}{n!} \quad \text{for } x \in G
$$
$$
\log_A(x) = l_A(x-1) = \sum_{n \geq 1} (-1)^{n-1} \frac{(x-1)^n}{n} \quad \text{for } x-1 \in G_1'
$$
（当不会引起混淆时，我们省略指标 $A$）。对于 $x \in G_R$ 和 $n \geq 1$，
$$
\left\| \frac{x^n}{n} \right\| \leq \left\| \frac{x^n}{n!} \right\| < R^n a^{-(n-1)\theta} = R \left( \frac{R}{a^\theta} \right)^{n-1}
$$
因此$e_A(G_R) \subset G_R$，$l_A(G_R) \subset G_R$代表$R \leq a^\theta$。

#### 命题 4 {#lie-ii-s8-prop-4 .statement tag=0A6X}

*令$R$为实数，使得$0 < R \leq a^\theta$。 映射 $\exp_A$ 定义 $G_R$ 到 $1 + G_R$ 的解析同构，逆同构是 $\log_A$ 到 $1 + G_R$ 的限制。*

$e(l(X)) = l(e(X)) = X$。通过 (20), (21) 和 *可微分和解析流形*, R, 4.1.5，我们推导出 $e_A(l_A(x)) = l_A(e_A(x))$ 对于 $x \in G_R$。然后
$$
\exp_A(\log_A x) = x \quad \text{for } x \in 1 + G_R \\
\log_A(\exp_A x) = x \quad \text{for } x \in G_R
$$
完成证明。

如果给$A$加上括号$[x, y] = xy - yx$，对于$\|xy - yx\| \leq \sup(\|xy\|, \|yx\|) \leq \|x\| \cdot \|y\|$，$A$将成为完整的规范李代数。 no. 3的命题2意味着$\tilde{H}$包含$G \times G$和$\tilde{H}$的绝对收敛域，因此定义是解析函数$h : G \times G \to A$；然后
$$
h(x, y) = \sum_{r, s \geq 0} H_{r,s}(x, y).
$$

#### 命题 5 {#lie-ii-s8-prop-5 .statement tag=0A6Y}

对于 G 中的 x、y，
$$
\exp_A \cdot \exp_A y = \exp_A h(x, y).
$$
$e^{U e^V} = e^{H(U, V)}$ 因此
$$
m \circ (1 + \tilde{\epsilon}, 1 + \tilde{\epsilon}) = (1 + \tilde{\epsilon}) \circ \tilde{H}
$$
$\tilde{H}(A \times A; A)$（其中 m 表示 A 上的乘法）。然后从命题 2、引理 3 以及可微分和解析流形，R，4.1.5 得出命题。

### 习题 {#lie-ii-s8-exercises}

我们假设域$K$的残差特征$p$>0。我们用$\mathfrak{o}_K$环表示$K$的估值$v$。

§ 8](exercises/s8/)参见[习题。
