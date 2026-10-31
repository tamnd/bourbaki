---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: Alternative algebras. Octonions
appendix: true
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 611-617, 654
pdf_pages: 0635-0641, 0678-0678
extraction: ocr
subsections:
    - "no": 1
      title: ALTERNATIVE ALGEBRAS
      page: 611
      pdf_page: 635
    - "no": 2
      title: ALTERNATIVE CAYLEY ALGEBRAS
      page: 613
      pdf_page: 637
    - "no": 3
      title: OCTONIONS
      page: 615
      pdf_page: 639
statements: 11
exercises: 3
content_sha256: 58178019c23b2befa68bd1072bde3844f932055a0109105f010bd48600c9e2dc
translated_from: content/en/alg/III/A_a_alternative_algebras_octonions.md
translation_method: google
source_content_sha256: ae041bbfaebb6710b823bdc0661c24a1124357966f753025f28bd48ab4086bed
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 65ebb810754dfe8d364f1a127adf81fe4c983ce534544a341df92de26cc39b55
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 附录

# 另类代数。八元数

### 1.替代方案代数

设 A 为交换环，F a（不一定结合）A-代数。对于 F 的任意三个元素 $x, y, z$，我们写

$$
a(x, y, z) = x(yz) - (xy)z
$$

（$x, y, z$的关联者）； $a$显然是$F \times F \times F$到$F$的A-三线性映射。

#### 引理 1 {#alg-iii-a0-lem-1 .statement tag=069A}

*对于代数$F$中的所有$p, q, r, s$，*

$$
a(pq, r, s) - a(p, qr, s) + a(p, q, rs) = a(p, q, r)s + pa(q, r, s).
$$

验证立即从定义 (1) 开始。

#### 命题 1 {#alg-iii-a0-prop-1 .statement tag=069B}

*对于 A-代数 $F$，以下条件等效：*
(a) *对于元素 $x, y$ $F$ 的每个有序对，$x$ 和 $y$ 生成的子代数是关联的。*
(b) *三线性映射 $(x, y, z) \mapsto a(x, y, z)$ 为交错的 (§ 7, no. 3)。*
(c) *对于元素 $x, y$ 中的每个有序对，$F$、$x^2y = x(xy)$ 和 $yx^2 = (yx)x$。*

显然（a）意味着（c）。我们证明(c)蕴涵(b)：通过定义(§ 7, no. 3)证明(b)，只需验证$a(x, x, y) = 0$和$a(x, y, y) = 0$，即是(c)。

为了证明 (b) 蕴含 (a)，我们使用以下 4 引理：

#### 引理 2 {#alg-iii-a0-lem-2 .statement tag=069C}

*令$E$为A-代数，使得映射$(x, y, z) \mapsto a(x, y, z)$为交错的，$E$的$S$生成的系统和$U$的子A模$E$ 包含 $S$，这样对于所有 $s \in S$ 都有 $sU \subset U$ 和 $Us \subset U$。然后$U = E$.*

$x \in E$的集合$U'$，使得$xU \subset U$和$Ux \subset U$显然是$E$的子A模块，其中包含$S$乘以假设。另一方面，对于$U'$和$u \in U$中的$x, y$，通过假设

$$
(xy)u = x(yu) + a(x, y, u) = x(yu) - a(x, u, y) = x(yu) - (xu)y + x(uy) \in U;
$$

在经过到反代数，我们有类似的$u(xy) \in U$。因此，$U'$是$E$的子代数，并且由于它是包含$S$，所以$U' = E$。因此$EU \subset U$和*更不必说*$UU \subset U$，证明$U$是$E$的子代数；因为包含$S$，$U = E$，这就证明了引理。

如果 $a(u, v, w) = 0$ 当元素 $u, v, w$ 属于至 $H$ 中*至少两个*时，$F$ 的子集 $H$ 被称为*强关联*。

#### 引理 3 {#alg-iii-a0-lem-3 .statement tag=069D}

*假设映射$a$为交错的。如果$H$是$F$的强关联子集，则$H$生成的$F$的子代数是强关联的。*

由于 $F$ 的强关联子集的集合是归纳性的，因此只要证明 $H$ 是 $F$ 的*极大*强关联子集，则 $H$ 就是 $F$ 的 *子代数*。由于$H$显然是$F$的子A模，因此足以验证对于$H$的任意两个元素$u, v$，$H \cup \{uv\}$也是强关联的，因为凭借$H$的定义，这将意味着$uv \in H$。现在，对于所有 $z \in H$ 和所有 $t \in F$，通过 (2)

$$
a(uv, t, z) - a(u, vt, z) + a(u, v, tz) = 0
$$

因为 $\mathbf{H}$ 是强结合的；因为 $u, v, z$ 在 $\mathbf{H}$ 中，也
$$
a(u, vt, z) = a(u, v, tz) = 0,
$$
从而$a(uv, t, z) = 0$。利用$a$是交错的的事实，这表明每当元素$p, q, r$属于到$\mathbf{H} \cup \{uv\}$从而引理中至少两个时$a(p, q, r) = 0$。

#### 引理 4 {#alg-iii-a0-lem-4 .statement tag=069E}

*假设映射$a$为交错的。那么，对于所有$x \in \mathbf{F}$，$x$生成的$\mathbf{F}$的子代数是强关联的。*

$a(u, v, w) = 0$ 每当三个元素 $u, v, w$ 中的两个等于$x$ 且应用引理 3 即可。

#### 引理 5 {#alg-iii-a0-lem-5 .statement tag=069F}

*假设映射$a$是交错的，并让$\mathbf{X}, \mathbf{Y}$是$\mathbf{F}$的两个强关联子代数。那么$\mathbf{X} \cup \mathbf{Y}$生成的$\mathbf{E}$的子代数是结合律。*

令$Z$为$z \in \mathbf{E}$的集合，使得$a(u, v, z) = 0$对于所有$u \in \mathbf{X}$和$v \in \mathbf{Y}$，这显然是一个子A-模块包含、$\mathbf{X}$和$\mathbf{Y}$，因为$\mathbf{X}$和$\mathbf{Y}$是强的联想的；到引理 2，就足以验证$u \in \mathbf{X}$和$v \in \mathbf{Y}$、$uZ \subset Z, vZ \subset Z, Zu \subset Z$和$Zv \subset Z$。现在，对于 $\mathbf{X}$、$v \in \mathbf{Y}$ 和 $z \in Z$ 中的 $u, u'$，通过 (2)
$$
a(u'u, z, v) - a(u', uz, v) + a(u', u, zv) = a(u', u, z)v + u'a(u, z, v) = 0
$$
由于 $\mathbf{X}$ 具有强结合性，并且定义是 $Z$。但由于 $\mathbf{X}$ 具有强结合性，$a(u', u, zv) = 0$ 并且从 $u'u \in \mathbf{X}$ 开始，$a(u'u, z, v) = 0$ 乘以 $Z$ 的定义。因此$a(u', uz, v) = 0$，它表明$uZ \subset Z$。 应用 (2) 现在有了$(p, q, r, s) = (v, z, u, u')$，我们类似地得到$Zu \subset Z$。 交换$\mathbf{X}$和$\mathbf{Y}$的角色，并利用$a$是交错的的事实，我们得到$vZ \subset Z$和$Zv \subset Z$； 从而引理。

现在只需证明 (b) 在命题 1 中蕴含 (a)，即可使用引理 4 取 $\mathbf{X} = \{x\}$ 和 $\mathbf{Y} = \{y\}$。

#### 定义 1 {#alg-iii-a0-def-1 .statement tag=069G}

*如果代数$\mathbf{F}$满足命题1的等价条件，则称为替代。*

联想词代数显然是替代方案。在no. 3中，我们将给例一个替代的代数，它不是结合性的。

如果$\mathbf{F}$是替代的A-代数，则通过扩展标量（§ 1, no. 5）从$\mathbf{F}$获得的每个A-代数$\mathbf{F} \otimes_A A'$都是替代的$A'$-代数，如下从命题1的条件（b）。

### 2.凯莱代数代数

#### 命题 2 {#alg-iii-a0-prop-2 .statement tag=069H}

*令 $\mathbf{A}$ 为环，$\mathbf{F}$ 凯莱 $\mathbf{A}$ 代数，e 为单位元，$s : x \mapsto \overline{x}$ 共轭，$\mathbf{N} : \mathbf{F} \to \mathbf{A}$ 为凯莱范数 (§ 3, no. 4)。

(i) 要使 $\mathbf{F}$ 成为替代方案，对于元素 $x, y$ $\mathbf{F}$ 中的每一个有序对，$x^2y = x(xy)$ 来说，这是必要且充分的。*

(ii) *如果 F 是替代项，则对于 F 中的所有 x、y，N(xy) = N(x)N(y)。*
(iii) *假设 F 是替代项。为了使元素 x ∈ F 可逆，N(x) 在 Ae 中可逆是充分必要的； x 的倒数是唯一的并且等于 N(x)^{-1}\overline{x}；用 x^{-1},* 表示
$$
x^{-1}(xy) = x(x^{-1}y) = y
$$
*或所有 y ∈ F。*

条件 $x^2y = x(xy)$ 显然对于 F 的替代是必要的 (no. 1, 命题 1)。相反，如果它对于 F 的元素、应用到 $\overline{x}$ 和 $\overline{y}$ 的每个有序对都成立，则给出 $\overline{x}^2\overline{y} = \overline{x}(\overline{xy})$； 应用与关系共轭，我们得到$yx^2 = (yx)x$，从而满足no. 1的命题1的条件(c)。

显然对于 F 中的所有 $x, y$ 都有$a(e, x, y) = 0$。如果 F 是可替代的，我们因此从命题 1 (no. 1) 推出由 e、x 和 y 生成的 F 的子代数 G 是结合律。作为$\overline{x} = -x + T(x) \in -x + Ae, \overline{x} \in G$，类似地$\overline{y} \in G$。然后$N(xy) = (xy)(\overline{xy}) = xy.\overline{y}.\overline{x} = N(y)x\overline{x} = N(y)N(x)$，利用$N(y) \in Ae$这一事实。这就证明了(ii)。

最后我们证明(iii)。如果$N(x)$在Ae中是可逆的，并且我们写为$x' = N(x)^{-1}\overline{x}$，那么$xx' = x'x = e$，对于$N(x) = x\overline{x} = \overline{x}x$。相反，如果 x 承认左逆 $x''$，则 (ii) 的 $N(x'')N(x) = N(e) = e$ 和 $N(x)$ 在 Ae 中是可逆的；此外，由于$x' = N(x)^{-1}\overline{x}$位于由x和e生成的子代数中，元素$x, x', x''$属于到由x、$x''$和e生成的关联子代数，因此$x'' = x''(xx') = (x''x)x' = x'$、从而唯一性断言。 公式 $x^{-1}(xy) = x(x^{-1}y) = y$ 由$x^{-1}, x$和y是由x、y和e生成的子代数的元素得出，这是结合律。

#### 命题 3 {#alg-iii-a0-prop-3 .statement tag=069I}

*设 E 为 A 的 Cayley A-代数、γ 元素，F 为由 γ 和 E 的共轭定义的 E 的 Cayley 扩张 (§ 2, no. 5、命题 5)。对于 F 是可替代的，E 是结合的是必要且充分的。*

令$u = (x, y), v = (x', y')$为F的两个元素（其中x、y、$x', y'$在E中）。那么(§ 2, no. 5,公式(27))

$$
\begin{cases}
u^2v = ((x^2 + \gamma \overline{y}y)x' + \gamma \overline{y}'(y\overline{x} + yx), (y\overline{x} + yx)\overline{x}' + y'(x^2 + \gamma \overline{y}y)) \\
u(uv) = (x(xx' + \gamma \overline{y}'y) + \gamma (x'\overline{y} + \overline{x}.\overline{y}')y, y(\overline{x}'\overline{x} + \gamma \overline{y}y') + (y\overline{x}' + y'x)x).
\end{cases}
$$

利用$\overline{y}y$和$\overline{x} + x$在Ae中的事实，检查这些公式表明E的结合性意味着$u^2v = u(uv)$，因此F是替代的事实（命题2）。相反，如果 F 是可替代的，则当 $y' = 0$ 给出时，应用等式 $u^2v = u(uv)$
$$
(y\overline{x} + yx)\overline{x}' = y(\overline{x}'\overline{x}) + (y\overline{x}')x.
$$
现在左边等于 $(yT(x))\overline{x}' = y(\overline{x}'T(x)) = y(\overline{x}'x + \overline{x}'\overline{x});$

与右边比较，我们得到$(y \bar{x}') x = y (\bar{x}' x)$，这证明了E的结合性，因为$x, y$和$\bar{x}'$是E的任意元素。

### 3.八元数

设 E 为 A 上型 $(\alpha, \beta, \gamma)$ 的四元数代数（$§ 2$、no. 5、例 2），并令 $\delta \in A$。 E 与 $\delta$ 的 Cayley 扩张 F 以及 E 的共轭被称为 A 上的八元数代数，据说是型 $(\alpha, \beta, \gamma, \delta)$。通过 no. 2 的命题 3，F 是替代代数。它的基 $(e_i)_{0 \leq i \leq 7}$ 为 8 元素，定义为
$$
\begin{align*}
e_0 &= (e, 0), & e_1 &= (i, 0), & e_2 &= (j, 0), & e_3 &= (k, 0) \\
e_4 &= (0, e), & e_5 &= (0, i), & e_6 &= (0, j), & e_7 &= (0, k)
\end{align*}
$$
其中$(e, i, j, k)$是E定义的loc的基。引用。；显然$e_0$（也用$e$表示）是F的单位元。如果$u = \sum_{i=0}^{7} \xi_i e_i$是F的元素（与$\xi_i \in A$），则$§ 2$的公式（23），（24）和（31）， no. 5，给出共轭，八元数$u$的迹和范数

$$
\left\{
\begin{aligned}
\bar{u} &= (\xi_0 + \beta \xi_1) e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 + \beta \xi_1 \\
N_F(u) &= \xi_0^2 + \beta \xi_0 \xi_1 - \alpha \xi_1^2 - \gamma (\xi_2^2 + \beta \xi_2 \xi_3 - \alpha \xi_3^2) \\
&\quad - \delta (\xi_4^2 + \beta \xi_4 \xi_5 - \alpha \xi_5^2) + \gamma \delta (\xi_6^2 + \beta \xi_6 \xi_7 - \alpha \xi_7^2).
\end{aligned}
\right.
$$

现在让 $u = (x, y)$、$u' = (x', y')$ 和 $u'' = (x'', y'')$ 为三个八元数（其中元素 $x, x', x'', y, y', y''$ 属于到 E）。 $§ 2$、no. 5 的公式 (24) 和 (27) 给出
$$
\begin{align*}
T_F((uu')u'') &= T(xx'x'') + \delta T(\bar{y}'y x'') + \delta T(\bar{y}''y \bar{x}') + \delta T(\bar{y}''y' x) \\
T_F(u(u'u'')) &= T(xx'x'') + \delta T(x''\bar{y}'y) + \delta T(\bar{x}'\bar{y}''y) + \delta T(x\bar{y}''y')
\end{align*}
$$
（其中 T 表示 E 中的迹，并且利用了 E 是结合律这一事实）。对于所有四元数 $x, y$ ($§ 2$, no. 4, 公式 (17))，$T(xy) = T(yx)$，可得出以下结论
$$
T_F((uu')u'') = T_F(u(u'u''))
$$
我们特别研究型 $(-1, 0, -1, -1)$ 的八元数； 公式 (4) 然后化简为
$$
\left\{
\begin{aligned}
\bar{u} &= \xi_0 e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 \\
N_F(u) &= \sum_{i=0}^{7} \xi_i^2.
\end{aligned}
\right.
$$

*如果我们取$\mathbf{A}$为实数的域$\mathbf{R}$，则型$(-1, 0, -1, -1)$超过$\mathbf{R}$的八元数称为*凯莱八元数*（或*八度数*）。从 no. 2 的命题 2 (ii) 可以得出，每个凯莱八元数 $\neq 0$ 都是*可逆的。**

#### 命题 4 {#alg-iii-a0-prop-4 .statement tag=069J}

*令$F$为型$(-1, 0, -1, -1)$超过$\mathbf{A}$的八元数代数。在域上存在维数 3个向量空间$V$，其中两个元素$\mathbf{Z}/2\mathbf{Z}$和$V$的双射$\lambda \mapsto e'_\lambda$到基$(e_i)_{0 \leq i \leq 7}$，使得*
$$
e'_0 = e_0, \qquad e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}
$$
*适用于$V$中的所有$\lambda, \mu$。在阶和$e'_\lambda (e'_\mu e'_\nu) = (e'_\lambda e_\mu) e'_\nu$中，在$V$中，$\lambda, \mu, \nu$线性依赖于$\mathbf{Z}/2\mathbf{Z}$就足够了；如果 $2 \neq 0$ 位于 $\mathbf{A}$ 中，则此条件是必需的。*

我们在这个编号的开头保留记号。由§ 2, no. 5的公式(33)可知，元素$\pm e_0, \pm e_1, \pm e_2, \pm e_3$的集合$S$由……组成在乘法下是稳定的。此外，对于$E$中的$x, y, y'$，乘以§ 2, no. 5的公式(22)，
$$
(x, 0)(0, y') = (0, y'x), \quad (0, y')(x, 0) = (0, y'\overline{x}), \quad (0, y)(0, y') = (-\overline{y}'y, 0)
$$
使得元素$\pm e_i$($0 \leq i \leq 7$)的集合$T$由……组成稳定在乘法以下；此外，它的乘法表“独立”于环$\mathbf{A}$。

特别地，令$\mathbf{A}''$为带有两个元素的域$\mathbf{Z}/2\mathbf{Z}$，并令$E''$为八元数的$\mathbf{A}''$和$F''$代数上的型$(1, 0, 1)$的四元数代数型$(1, 0, 1, 1)$超过$\mathbf{A}''$；令$(e''_i)_{0 \leq i \leq 7}$为如上所述形成的$F''$中的基。从$-e''_i = e''_i$开始，$e''_i$的集合$T''$有8个元素，稳定在乘法以下；此外，从上面可以立即得出映射$\theta : T \to T''$，使得$0 \leq i \leq 7$的$\theta(e_i) = \theta(-e_i) = e''_i$对于乘法来说是同态。此外，四元数代数$E''$在这种情况下是可交换的，因此$F''$是结合律（§ 2, no. 5，命题5）；此外，在这种情况下，$F''$中的共轭就是恒等式。因此 $T''$ 是 *群* 且公式 (8) 表明它是*可交换的*； § 2, no. 5的这些公式和公式(33)表明，$T''$的每个元素中的平方是单位。如果 $V$ 用于表示群 $T''$ 相加，$V$ 可以在 $\mathbf{Z}/2\mathbf{Z}$ 上被赋予唯一的向量空间结构，必然为维数 3，因为
$$
\operatorname{Card}(V) = 8 = 2^{\dim(V)}.
$$

对于所有$\lambda \in V$，令$e'_\lambda$表示$(e_i)_{0 \leq i \leq 7}$的元素，使得$\theta(e'_\lambda) = \lambda$；然后$e'_0 = e_0$；此外，由于$\theta$是同态，关系$\theta(x) = \theta(y)$相当于$x = \pm y$、$e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}$。如果$\lambda, \mu, \nu$与$\mathbf{Z}/2\mathbf{Z}$线性无关，则它们形式基与$V$，因此所有元素$e_i$（$0 \leq i \leq 7$）将由$e'_\lambda, e'_\mu$生成属于到子代数并且$e'_\nu$；当 $2 \neq 0$ 在 $\mathbf{A}$ 中时，$e'_\lambda (e'_\mu e'_\nu) = (e'_\lambda e'_\mu) e'_\nu$ 是不可能的，因为 $F$ 是结合律，因此 $E$ 是可交换的 (§ 2, no. 5, 命题 5)，其中与……矛盾关系 (33) § 2, no. 5。另一方面，如果 $\lambda, \mu, \nu$ 在 V 中线性相关，则三个元素 $e'_\lambda, e'_\mu, e'_v$ 属于到子代数与 F 的 2 个生成元相关，因此是关联的 (no. 1, 命题 1)； 从而结论。

#### 注 {#alg-iii-a0-n3-rem-1 .statement tag=069K}

作为 $\bar{e}'_\lambda = -e'_\lambda$ 对应 $\lambda \neq 0$，

$$
e'_\lambda{}^2 = -e_0 \quad \text{for } \lambda \neq 0,
$$
$$
e'_\mu e'_\lambda = -e'_\lambda e'_\mu \quad \text{for } \lambda \neq 0, \mu \neq 0 \text{ and } \mu \neq \lambda.
$$

### 习题{#alg-iii-a0-exercises}

请参阅[习题附录 0](exercises/a0/)。
