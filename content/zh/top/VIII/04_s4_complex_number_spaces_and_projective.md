---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 4
section_title: Complex number spaces and projective spaces
lang: zh
source: top-v-x
pdf_pages: 0124-0128, 0133-0136
extraction: ocr
subsections:
    - "no": 1
      title: THE VECTOR SPACE $\mathbf{C}^n$
      page: 0
      pdf_page: 124
    - "no": 2
      title: TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $\mathbf{C}$
      page: 0
      pdf_page: 125
    - "no": 3
      title: COMPLEX PROJECTIVE SPACES
      page: 0
      pdf_page: 125
    - "no": 4
      title: SPACES OF COMPLEX PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 127
statements: 3
exercises: 8
content_sha256: aecbb556e327f05c8e6e374a6ae44b68cbd5a6f3e4c702db323eaf413f7ae737
translated_from: content/en/top/VIII/04_s4_complex_number_spaces_and_projective.md
translation_method: google
source_content_sha256: a0635aa3afab1817d675f46cf3f74b8d72a27d4aefcae7dd03e7963e1016fe2d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 5621216e6639b54ba0fd9986317b03f762ba1eefc93b28d8bbfca40d340a4a64
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 4. 复数空间和射影空间

### 1. 向量空间$\mathbf{C}^n$

由于拓扑空间$\mathbf{C}$可以用$\mathbf{R}^2$来识别，$n$空间与$\mathbf{C}$相同的拓扑乘积$\mathbf{C}^n$可以用$\mathbf{R}^{2n}$qua拓扑空间来识别；同样，$\mathbf{C}^n$的拓扑群结构，$n$因子的加法（拓扑）群结构的乘积，可以与加法群$\mathbf{R}^{2n}$的拓扑识别。但由于$\mathbf{C}$是域，我们可以在$n$维向量空间的$\mathbf{C}^n$结构上定义，在$\mathbf{C}$上，乘积$az$上复数 $\mathbf{C}^n$的$a$和点$z = (z_i)$为点$(az_i)$；这个向量空间结构应该与$\mathbf{R}$上的$2n$维向量空间的结构仔细区分，定义在$\mathbf{R}^{2n}$（章VI, § 1, no. 3）上。我们将为拓扑空间保留记号$\mathbf{C}^n$，即$n$空间中的乘积与$\mathbf{C}$相同，在加法中赋予向量空间结构超过$\mathbf{C}$刚刚定义的； $\mathbf{C}^n$称为$n$维数的复数空间。请注意，映射 $(t, z) \to tz$ 在 $\mathbf{C} \times \mathbf{C}^n$ 上连续。

$\mathbf{C}^n$到$\mathbf{C}^m$的仿射线性映射也是$\mathbf{R}^{2n}$到$\mathbf{R}^{2m}$的仿射线性映射，但逆命题是假的。

例如，映射 $z \to \overline{z}$ 是向量空间 $\mathbf{R}^2$ 的线性映射自身，但不是向量空间 $\mathbf{C}$ 的线性映射自身。

因此，$\mathbf{C}^n$到$\mathbf{C}^m$的每个仿射线性映射都是一致连续的；特别是，$\mathbf{C}^n$对自身的每个仿射线性映射都是同胚。

向量空间 $\mathbf{C}^n$ 中$p$ 维数 ($p \leq n$) 的每个仿射线性簇也是向量空间 $\mathbf{R}^{2n}$ 中$2p$ 维数的仿射线性簇；再次强调，逆命题是假的。为了避免混淆，$\mathbf{C}^n$中$p$维数的（仿射）线性簇将被称为$p$维数的复杂线性簇（$\mathbf{R}^{2n}$的线性簇在必要时被称为实线性簇以防止误解）。特别是，一个维数（或两个维数）的复线性簇称为复直线（或复平面），而$n - 1$维数的复线性簇称为复超平面。

通过将$\mathbf{R}^n$与关系定义的$\mathbf{C}^n$的子集进行识别，通常可以方便地将实数空间$\mathbf{R}^n$视为嵌入复数空间$\mathbf{C}^n$ $J(z_k) = 0$（$1 \leq k \leq n$）。由$\mathbf{C}^n$ 重合的拓扑群结构与$\mathbf{R}^n$ 的拓扑群结构在此子集上诱导出拓扑群结构。

请注意，嵌入到 $\mathbf{C}^n$ 中的 $\mathbf{R}^n$ 并不是 $\mathbf{C}^n$ 中的复杂线性簇。

$p$系统$\mathbf{R}^n$向量$\mathbf{R}$以上免费，$\mathbf{C}$以上免费。 $\mathbf{R}^n$ 生成中$p$ 维数的每个实线性簇$V$ $\mathbf{C}^n$ 中$p$ 维数的复线性簇$V'$，使得$V$ 是$V'$ 的迹$\mathbf{R}^n$；如果$V$由$n - p$线性方程$f_k(x) = a_k$的系统定义，其中$f_k$是$\mathbf{R}^n$上的线性形式（具有实数系数，并且在$\mathbf{R}$上线性无关）并且$a_k$是实数，然后是相同的方程定义$V'$，但现在$x$的坐标采用复数值。

相反，如果$p$维数的复线性簇有一个非空的交和$\mathbf{R}^n$，则这个交是一个真正的线性簇，但它的维数可能是$< p$。

### 2. 拓扑向量空间和代数超过域 $\mathbf{C}$

所有定义以及第 79 号的所有结果。 章 VI, § 1 的 5 和 6，相对于域 $\mathbf{R}$ 上的向量空间和代数上的拓扑，特别是矩阵的空间和代数以及元素 $\mathbf{R}$，当我们在替换 $\mathbf{R}$ 到 $\mathbf{C}$ 时始终保持有效，无需任何修改。

### 3. 复射影空间

通过在章 VI, § 3, no. 1 中回忆记号，我们得到以下定义，类似于实射影空间的定义：

#### 定义 1 {#top-viii-s4-def-1 .statement tag=0C0W}

*射影空间* $\mathbf{P}_n(\mathbf{C})$，*赋予拓扑，即* $\mathbf{C}_{n+1}^*$的商 *通过等价关系* $\Delta_n(\mathbf{C})$，*称为* $n$的复射影空间 *维数.*

射影空间 $\mathbf{P}_1(\mathbf{C})$ 称为*复射影线*，$\mathbf{P}_2(\mathbf{C})$ 称为*复射影平面*。

大多数参数与实射影空间扩展有关，对复射影空间进行了非常微小的修改。

首先，根据章VI, § 3的命题1的论证，我们看到拓扑空间$P_n(\mathbf{C})$是*Hausdorff*。 no. 1，只需将字乘以替换，将$\mathbf{R}$乘以$\mathbf{C}$即可应用字。同样，证明 / 命题 2 / 章 VI, § 3。 no. 1表明$P_n(\mathbf{C})$是*紧且连通的*，并且与球体$S_{2n-1}$的商同胚（被认为嵌入在空间$C_{n-1}^*$中，用$R_{2n-2}^*$识别），由等价关系在该球体上诱导$\Delta_n(\mathbf{C})$；唯一的点不同之处在于，现在，如果 $n \geqslant 0$，则关系的等价类与圆 $S_1$ 同胚。

因此，章VI中的命题3。 § 3, no. 1 没有复射影空间的类似物。

下一个表明，如章VI, § 3, no. 2，空间$P_n(\mathbf{C})$中的每个$p$维射影线性簇都是一个闭集合，同胚于$P_r \mathbf{C}$，并且如果$p < n$，它的补集在$P_n(\mathbf{C})$中是稠密的。 章 VI, § 3, no. 2 的命题 5 的证明可以按原样转置，只需用 $\mathbf{C}$ 代替 $\mathbf{R}$，并表明（如果 $n \geqslant 0$）射影超平面在 $P_n(\mathbf{C})$ 中的补集同胚于$\mathbf{C}^*$，因此每个点都有邻域同胚于$\mathbf{C}^*$。这个结果允许我们将复数空间$\mathbf{C}^n$嵌入到复射影空间$P_n(\mathbf{C})$中，通过将$\mathbf{C}^*$与射影超平面的补集识别，称为“无穷远的超平面”（通常是超平面，其等式为$x_0 = 0$）。在特殊情况下$n = 1$，无穷远的超平面是*点*，并且Alexandroff的定理表明$P_1 \mathbf{C}$同胚于空间$\tilde{\mathbf{C}}$，通过压缩局部紧致空间$\mathbf{C}$获得：毗邻“无穷远处点”，用$\infty$表示。 命题 4 个，共章 VI。 § 2, no. 4 然后表明*复射影线* $P_1(\mathbf{C})$ *同胚于球体* $S_2$。

我们将阐明与章 VI 类似的结果的任务留给读者。 § 3。 no. 4，对于函数，将其值放入$\mathbf{C}$。

将空间 $\mathbf{R}^{n+1}$ 视为 *嵌入* $\mathbf{C}^{n+1}$ (no. 1) 中。让$f$是$C_{n-1}^*$的典范映射到它的商空间$P_n(\mathbf{C})$上。 子空间 $f(\mathbf{R}_{n-1}^*)$ 由 $P_n(\mathbf{C})$ 的点组成，其中至少有一个系统*实*齐次坐标；让我们证明 $f(\mathbf{R}_{n-1}^*)$ 与实射影空间 $P_n(\mathbf{R})$ 同胚，这将允许我们将空间 $P_n(\mathbf{R})$ 视为 *嵌入* 于 $P_n(\mathbf{C})$ 中。现在$\Delta_n(\mathbf{C})$在$\mathbf{R}_{n+1}^*$上诱发关系是$\Delta_n(\mathbf{R})$； 典范映射 $\varphi$ 共

$$
\mathbf{R}_{n+1}^*/\Delta_n(\mathbf{R}) = P_n(\mathbf{R})
$$

到 $f(\mathbf{R}_{n-1}^*)$ 是*连续* (章 I, § 3, no. 6, 命题 10)；自从

$P_n(\mathbf{R})$ 是紧致的，$\varphi$ 必须是同胚 (章 I, § 9, no. 4, 定理 2, 推论 2)。

我们还可以通过调用章 I, § 3, no. 6 的命题 10 准则，在不使用$P_n(\mathbf{R})$的紧性的情况下证明$\varphi$是双连续的（参见习题 3）。

由于 $\mathbf{R}^{n+1}$ 生成的 $p + 1$ 维数的每个向量子空间 $\mathbf{C}^{n+1}$ 中的 $p + 1$ 维数的复数向量子空间，我们看到每个射影线性簇$P_n(\mathbf{R})$ 中 $p$ 维数的 $V$（$V$ 称为*实*射影线性簇） 生成射影线性簇 $P_n(\mathbf{C})$ 中 $p$ 维数的 $V'$（$V'$ 称为*实*射影线性簇） *复*射影线性簇），这样$V$是$V'$在$P_n(\mathbf{R})$上的迹。此外，当我们允许变量取复数值时，$V$的（齐次）方程的每个系统也是$V'$的（齐次）方程的系统。

### 4. 复射影线性簇的空间

通过在章 VI, § 3, no. 5 中回顾记号，我们在复射影空间中对射影线性簇进行定义类似的空间：

#### 定义 2 {#top-viii-s4-def-2 .statement tag=0C0X}

*商空间* $P_{n,p}(\mathbf{C})$ *拓扑空间* $L_{n+1,\ p+1}(\mathbf{C})$ *通过等价关系* $\Delta_{n,p}(\mathbf{C})$ *在射影空间*中被称为* $p \geqslant 0$ *维数的射影线性簇的空间 $P_n(\mathbf{C})$。

通过章VI, § 3, no. 5的命题6的论证，我们首先看到$P_{n,p}(\mathbf{C})$是*Hausdorff*。接下来我们通过替换子空间$V_{n+1,\ p+1}$（章VI, § 3, no. 5命题7证明）通过$L_{n+1,\ p+1}(\mathbf{C})$由……组成子空间$W_{n+1,\ p+1}$来证明它是*紧致的* $p + 1$ 向量的系统，其中形式是向量子空间的*正交厄米特基*，它们生成；也就是说，$W_{n+1,\ p+1}$ 由矩阵 $X = (x_{ij})$ 组成，其中满足条件

$$
\sum_{j=0}^n x_{ij} \overline{x}_{ij} = 1 \quad (1 \leq i \leq p + 1),
$$
$$
\sum_{j=0}^n x_{ij} \overline{x}_{kj} = 0 \quad (i \neq k).
$$

章 VI, § 3, no. 5 扩展中的命题 8 个证明对于空间 $P_{n,p}(\mathbf{C})$ 未改变，并显示此空间是*连接* 和*本地连接* 并且它的每个点都有邻域同态于 $\mathbf{C}^{p+1,(n-p)}$。最后，章VI, § 3, no. 6的命题9的证明在没有变换的情况下适用，因此格拉斯曼$G_{n,p}(\mathbf{C})$同胚于$\mathbf{P}_{n,p}(\mathbf{C})$。

#### 注 {#top-viii-s4-n4-rem-1 .statement tag=0C0Y}

大多数属性公共的到实数和复数空间（或射影空间）也适用于数空间（或射影空间），以与四元数 $\mathbf{H}$ 的除法环相同的方式定义；事实上，它们能够对许多其他拓扑域进行扩张和环除法（cf.习题2和6）。

### 习题{#top-viii-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
