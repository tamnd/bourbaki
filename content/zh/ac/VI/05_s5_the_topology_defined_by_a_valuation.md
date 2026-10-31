---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 5
section_title: The topology defined by a valuation
lang: zh
source: ac-i-vii
book_pages: 399-403, 454-459
pdf_pages: 0417-0421, 0472-0477
extraction: ocr
subsections:
    - "no": 1
      title: THE TOPOLOGY DEFINED BY A VALUATION
      page: 399
      pdf_page: 417
    - "no": 2
      title: TOPOLOGICAL VECTOR SPACES OVER A FIELD WITH A VALUATION
      page: 401
      pdf_page: 419
    - "no": 3
      title: THE COMPLETION OF A FIELD WITH A VALUATION
      page: 402
      pdf_page: 420
statements: 10
exercises: 10
content_sha256: 1222353c4fbafa89cfeaa45230181946b23b914be91d8ff10ac050902b7e6423
translated_from: content/en/ac/VI/05_s5_the_topology_defined_by_a_valuation.md
translation_method: google
source_content_sha256: f97824efc1e49c2f3f557cc487ce4e195405a030102d3750617c5a288f2ba3cd
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 7c40e68f02edba739b3e87d1171f5b45057179dc99cb40c1b33ee1ba37acc422
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 5. 由估值定义的拓扑

### 1. 由估值定义的拓扑

令 K 不一定为交换域，v 为 K 和 G 的全序群 $v(K^*)$ 的估值。对于所有$a \in G$，令V为$x \in K$的集合，使得$v(x) > a$；这个集合是K（§ 3, no. 1）的添加剂子群。 K 上存在唯一的拓扑 $\mathscr{T}_v$，其中 V、形式邻域的基本系统为 0（*一般拓扑*、章 III, § 1, no. 2、例）。要使 v 不恰当，$\mathscr{T}_v$ 是离散的拓扑是充分必要的。

#### 引理 1 {#ac-vi-s5-lem-1 .statement tag=04UQ}

*设$x \in K^*, y \in K^*$和$\alpha \in G$。如果*
$$
v(x - y) > \sup(\alpha + 2v(y), v(y)),
$$
*然后*$v(x^{-1} - y^{-1}) > a$。

$x^{-1} - y^{-1} = x^{-1}(y - x)y^{-1}$ 因此
$$
v(x^{-1} - y^{-1}) = v(x - y) - v(x) - v(y).
$$
如果$v(x - y) > v(y)$，§ 3, no. 1的命题 1意味着$v(x) = v(y)$，从$x = y + (x - y)$开始。此外，如果$v(x - y) > a + 2v(y)$，那么
$$
v(x^{-1} - y^{-1}) > a + 2v(y) - 2v(y) = a.
$$

#### 命题 1 {#ac-vi-s5-prop-1 .statement tag=04UR}

*拓扑 $\mathscr{T}_v$ 是 Hausdorff，并且与 K 上的域结构兼容。如果给 G 提供离散拓扑，则映射 $v : K^* \to G$ 是连续的。*

设$x \in K^*$和$a = v(x)$；然后$x \notin V_a$表明$\mathscr{T}_v$是Hausdorff。对于所有$x_0 \in K$和$a \in G$，存在$\beta \in G$使得$x_0 V_\beta \subset V_\alpha$和$V_\beta x_0 \subset V$，（取$\beta \geqslant a - v(x_0)$就足够了）。另一方面，如果$a \geqslant 0$，则$V_\alpha V_\alpha \subset V_v$。满足*通用拓扑*、章III, § 6, no. 3的公理(AV_I)和(AV_{II})，$\mathscr{T}_v$与$K$上的环结构兼容。让$x_0 \in K^*$；如果$x \in K^*$满足$v(x - x_0) > \sup(\alpha + 2v(x_0), v(x_0))$，则$v(x^{-1} - x_0^{-1}) > a$（引理1），这表明$x \mapsto x^{-1}$是连续的，因此$\mathscr{T}_v$与$K$上的域结构兼容。最后，单个条件$v(x - x_0) > v(x_0)$意味着$v(x) = v(x_0)$（$§ 3$，no. 1，命题1），因此如果$G$被赋予离散的拓扑，则映射$v : K^* \to G$是连续的。

令$\alpha \in G$和$V'_\alpha$为$x \in K$的集合，使得$v(x) \geq \alpha$。如果$\beta < a$，则$V_\beta \supset V'_\alpha \supset V_v$。如果$v$不是不恰当的，那么可以看出，$V'_\alpha$形式对于$\mathscr{T}_v$来说邻域的基本系统为0。

$V_v$和$V'_\alpha$是开加法子群，因此在$K$中是封闭的，因此拓扑域$K$是*完全断开的*。由于$v$包含和$V_v$的环的每个非零理想，它在$K$中是“开和闭”。因此，$v$ 与剩余类域的商拓扑是*离散*。

令 $A$ 为 $u$ 的环。如果$v$是离散的，$§ 3$、no. 6的命题 8表明$\mathscr{T}_v$在$A$上诱导拓扑是$m(A)$进数拓扑。一般来说情况并非如此（习题4）。

#### 命题 2 {#ac-vi-s5-prop-2 .statement tag=04US}

*设$K$不一定是交换域，$v$是$v$的$K$，$A$环的非不当估值，$m$是$v$的理想值。为了使$K$和拓扑$\mathscr{T}_v$局部紧致，满足以下条件是必要且充分的：*

(i) $K$ 已完成；
(ii) $v$ 是离散的；
(iii) *剩余类域 $\kappa(A)$ 是有限的。*

*如果是这样*，$A$ 是紧致的。

假设 $K$ 是局部紧致的。那么就完成了（*一般拓扑*、章111、$§ 3$、no. 3、推论1到命题4）；进一步存在0的紧邻域，其中包含邻域$V'_a$，其中$v$的$a$属于到值群；在其他字中，$K^*$中存在$a \neq 0$，使得$A . a$是紧的，因此$A = (A . a)a^{-1}$是紧的。由于$A$的每个理想$b \neq (0)$都是开放的，$A/b$是紧凑且离散的（*一般拓扑*、章 III、$§ 2$、no. 5、命题 14），因此是有限的，特别是$\kappa(A) = A/m$是有限的。此外，对于$m$中的$y \neq 0$，环$A/Ay$是有限的，只有有限的数理想$A$包含$Ay$和集合$P$ 元素形式 $v(x)$ 使得

$$
0 < v(x) \leq v(y)
$$

是有限的；由于 $v(K^*)$ 是全序的，$P$ 至少有元素 $y$。然后对于所有$x \in A$，使得$v(x) > 0$、$v(x) > v(y) \geq y$或$v(x) \leq v(y)$，然后将$v(x) \geq y$乘以定义，这样$y$是$v(K^*)$的元素$> 0$中最小的一个。 *由于* $P$ *是*有限的，因此存在最大的整数 $m \geq 0$，使得 $my \in P$，从而我的 \leq v(y) < (m+1)\gamma。我们推导出 0 \leq v(y) - my < y 并且通过 y 的定义这意味着 $v(y) = my$。因此$v(K^*) = \mathbf{Z}.\gamma$和估值$v$是离散的。

相反，假设条件 (i), (ii), (iii) 成立。我们可以将注意力限制在$v$被范化的​​情况；让 $u$ 成为 $v$ 的均匀化器。那么 $\kappa(A) = A/Au$ 因而 $A/Au$ 是有限的。由于 $x \mapsto xu^n$ 定义，通过将加法群 $A/Au$ 的商同构取到 $Au^n/Au^{n+1}$ 上，$A/Au^j$ 对于所有 $j \geq 0$ 都是有限的。由于 $A$ 在 $K$ 中闭合，因此它是完备的，因此与 $A/Au^j$ 的逆极限同构（通用拓扑、章 111、§ 7, no. 3、命题 2），因此是紧凑的。由于$A$在$K$中开路，因此可以看出$K$是局部紧的。

#### 注 {#ac-vi-s5-n1-rem-1 .statement tag=04UT}

注在这个证明中假设$A$ 是完整的就足够了。

我们将在§ 9中看到域$K$满足命题2的条件承认中心，它要么是$p$进数域的有限代数扩张，要么正式幂级数超过有限域的域$\mathbf{F}_q((T))$；此外，$K$ 的有限秩超过其中心。

### 2. 拓扑向量空间超过域并进行评估

自始至终，让$K$是（不一定可交换的）域，$v$对$K$和$G$的估值阶群。 $K$ 给出拓扑 $\mathscr{T}_v$。

#### 命题 3 {#ac-vi-s5-prop-3 .statement tag=04UU}

令$E$为$K$上的左拓扑向量空间，即Hausdorff且维数1。假设$v$不是不恰当的。对于$E$中的所有$x_0 \neq 0$，$K_s$的映射$a \mapsto ax_0$到$E$是拓扑同构。

这个映射是一个连续代数同构。只要证明它是双连续的就足够了。让$\alpha \in G$。我们需要证明$E$中存在0的邻域$V$，使得关系$ax_0 \in V$蕴含$v(a) > a$。设$a, \in K^*$使得$v(a_0) = a$。由于$E$是豪斯多夫，$E$中存在0的邻域$W$使得$a_0x_0 \notin W$。由于$v$并非不恰当，$E$中存在0的邻域$W'$和$G$中的元素$\beta$，因此关系$y \in W'$、$v(a) \geq \beta$意味着$ay \in W$。令 $a, \in K^*$ 等于 $v(a_1) = -\beta$。 关系 $ax_0 \in a_1^{-1}W'$和$v(a) \leq a$意味着$a_1ax_0 \in W$和$v(a_0a^{-1}a_1^{-1}) = \alpha + \beta - v(a) \geq \beta$，因此意味着$a_0x_0 = a_0a^{-1}a_1^{-1}(a_1ax_0) \in W$，这是荒谬的；在其他字，关系$ax, \in a_1^{-1}W$意味着$v(a) > a$。

#### 推论{#ac-vi-s5-n2-cor-1 .statement tag=04UV}

设$E$是$K$上的左拓扑向量空间，$H$是$E$的闭超平面，$D$是$E$的一维向量子空间，补充的代数补充 $H$。假设$v$并无不当。那么$D$是$H$的拓扑补充。

考虑命题 1和3，证明与拓扑向量空间、章I, § 2相同，推论2至定理1。

#### 命题 4 {#ac-vi-s5-prop-4 .statement tag=04UW}

假设$v$不是不恰当的并且$K$是完整的。令$E$为$K$上的左拓扑向量空间，这是Hausdorff且为有限维$n$。对于$E$的每个基$(e_i)_{1 \leq i \leq n}$超过$K$，$K^n_s$的映射$(a_i) \mapsto \sum_{i=1}^n a_i e_i$到$E$是一个拓扑向量空间同构。

考虑到命题 3 及其推论，证明与拓扑向量空间、章 I, § 2、定理 2 相同。

#### 推论{#ac-vi-s5-n2-cor-2 .statement tag=04UX}

假设$v$不是不恰当的并且$K$是完整的。令$E$是$K$上的豪斯多夫拓扑向量空间，而$F$是$E$的有限维向量子空间。然后$F$关闭。

$F$已完成。

### 3. 完成域并进行估值

#### 命题 5 {#ac-vi-s5-prop-5 .statement tag=04UY}

令$K$不一定是交换域，$v$是对$K$和$G$群$v(K^*)$与离散拓扑的评估。

(a) $K$（与$\mathscr{T}_v$）的补全环$\hat{K}$是拓扑域。

(b) 映射 $v : K^* \to G$ 可以唯一地扩展为连续的映射 $8 : \hat{K}^* \to G$。 映射 $0$（由$\hat{v}(0) = +\infty$扩展）是$\hat{K}$和$\hat{v}(\hat{K}^*) = v(K^*)$的估值。

(c) $\hat{K}$ 上的拓扑是由估价$0$ 定义的拓扑。

(d) 对于所有$a \in G$，令$V_\alpha, V'_\alpha$为由条件$v(x) > a, v(x) \geq a$定义的$K$中的子群。那么$\hat{K}$中$V_\alpha, V'_\alpha$的闭包$\overline{V}_\alpha, \overline{V}'_\alpha$分别由条件$\hat{v}(x) > a, \hat{v}(x) \geq a$定义。

(e) $0$的环是$v$的环$A$的完成$\hat{A}$； $0$的理想是$v$的理想$m$的完成$\hat{m}$。

(f) $\hat{A} = A + m$； $8$ 的剩余类域与 $v$ 的规范一致。

To prove (a) it suffices (General 拓扑, 章 III, § 6, no. 8, 命题 7) to show the following: let $\mathfrak{F}$ be a Cauchy filter (with respect to the additive uniform 结构) on $K^*$ for which $0$ is not a cluster 点；那么双射$x \mapsto x^{-1}$下$\mathfrak{F}$的像是柯西滤波器（相对于加性均匀结构）。因为由于$0$不是$\mathfrak{F}$的簇点，因此存在$M \in \mathfrak{F}$和$\beta \in G$，使得$\beta$是$v(M)$的上界。让$a \in G$。 If $M'$ is 元素 of $\mathfrak{F}$ contained in $M$ and such that $v(x - y) > \sup(\alpha + 2\beta, \beta)$ for $x \in M'$ and $y \in M'$, then $v(x^{-1} - y^{-1}) > a$ for $x \in M'$ and $y \in M'$ (no. 1, 引理1)。 从而（一）。

通过no. 1的命题 1，$v|K^*$是从$K^*$到$G$的连续同态，因此可以唯一地扩展到从$K^*$到$G$的连续同态$0$。 关系

$$
\hat{v}(x + y) \geq \inf(\hat{v}(x), \hat{v}(y))
$$

在 $K^*$ 中成立，因此通过连续性也在 $\hat{K}^*$ 中成立。因此 0（扩展$\hat{v}(0) = +\infty$）是$\mathbf{K}$的估值，并且 (b) 得到证明。

我们现在展示(d)。设$a \in G$和$x \in \mathscr{S}, -\{0\}$。对于$V$中的$y$，足够接近$x$、$\hat{v}(x) = \hat{v}(y) = v(y)$，因此也接近$\hat{v}(x) > a$。相反，令 $x \in \hat{K}^*$ 使得 $\hat{v}(x) > a$；对于$K^*$中的$y$足够接近$x$、$v(y) = \hat{v}(y) = \hat{v}(x)$，因此$y \in V$、从而$x \in \mathscr{S}$。因此$\mathscr{S}$是$x \in \hat{K}$的集合，使得$\hat{v}(x) > a$。该论证与 $V'_a$ 类似。这就证明了(d)。

考虑一般拓扑的命题7、章III, § 3, no. 4，断言(c)是(d)的推论。 断言 (e) 是 (d) 的特例。最后让$x \in \hat{A}$；存在$y \in A$使得$\hat{v}(x - y) > 0$；然后$z = x - y \in \hat{m}$，因此$x = y + z \in A + \hat{m}$；因此$\hat{A} = A + \hat{m}$，显示(f)。

#### 注 {#ac-vi-s5-n3-rem-1 .statement tag=04UZ}

对于所有$x \in \hat{K}$而非属于到$\hat{A}$，存在$x_0 \in K$使得$\hat{v}(x - x_0) > 0$，$\hat{v}(x) = \hat{v}(x_0) = v(x_0) < 0$；那么$x_0^{-1} x \in \hat{A}$，以及$x_0^{-1} \in A$，可以看出，如果我们集合$S = A - \{0\}$，就可以写成$\hat{K} = S^{-1} \hat{A}$。

### 习题 {#ac-vi-s5-exercises}

次数 $n > 1$ 且$a_i \neq 0$；证明在区间 $[0, n]$ 中存在整数的严格递增的序列 $(i_k)_{0 \leq k \leq r}$，使得： (1) $i_0 = 0$，$i_r = n$； (2) $v(a_{i_k})$ 对于$0 \leq k \leq r$ 是有限的； (3) 对于每个指标$j$，使得$0 \leq j \leq n$不同于$i_k$，使得$v(a_j)$是有限的，点
$$
(j, v(a_j)) \in \mathbf{R}^2
$$
位于线经过至点 $(i_k, v(a_{i_k}))$ 和 $(i_{k+1}, v(a_{i_{k+1}}))$ 上方，并且如果 $j < i_k$ 或 $j > i_{k+1}$ 则严格位于该线上方。 段的并连接点$(i_k, v(a_{i_k}))$和$(i_{k+1}, v(a_{i_{k+1}}))$称为P的牛顿多边形，上面的段称为边，点$(i_k, v(a_{i_k}))$称为多边形的顶点。

(b) 假设 P 属于的所有零到 K。 证明要使 P 的所有零的估值相同，$r = 1$ 是充分必要的（在其他字中，牛顿多边形约化为单边）。 （为了证明条件是足够的，请考虑乘积$P_1P_2$的牛顿多边形，其中$P_1$的所有零在$v$的环中可逆，而$P_2$属于的所有$v$的理想。）

(c) 假设 P 属于的所有零到 K； 形式 P 的牛顿多边形并写出。
$$
\rho_k = i_{k+1} - i_k, \quad \sigma_k = (v(a_{i_{k+1}}) - v(a_{i_k}))/\rho_k.
$$
证明，对于$0 \leq k \leq r - 1$，P 恰好承认$\rho_k$零（用重数的阶来计算），其估值都等于$\sigma_k$（使用（b）并通过归纳对$r$进行论证）。

(d) 推广到任何估值$v$的情况（在向量 Q-空间$\Gamma_{(0)}$中嵌入$v$的阶群$\Gamma$，其具有自然全序群结构）。

95

§ 5](exercises/s5/)参见[习题。
