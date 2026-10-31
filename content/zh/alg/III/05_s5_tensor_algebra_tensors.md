---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 5
section_title: Tensor algebra. Tensors
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 484-497, 627-632
pdf_pages: 0508-0521, 0651-0656
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE TENSOR ALGEBRA OF A MODULE
      page: 484
      pdf_page: 508
    - "no": 2
      title: FUNCTORIAL PROPERTIES OF THE TENSOR ALGEBRA
      page: 485
      pdf_page: 509
    - "no": 3
      title: EXTENSION OF THE RING OF SCALARS
      page: 489
      pdf_page: 513
    - "no": 4
      title: DIRECT LIMIT OF TENSOR ALGEBRAS
      page: 490
      pdf_page: 514
    - "no": 5
      title: TENSOR ALGEBRA OF A DIRECT SUM. TENSOR ALGEBRA OF A FREE MODULE. TENSOR ALGEBRA OF A GRADED MODULE
      page: 491
      pdf_page: 515
    - "no": 6
      title: TENSORS AND TENSOR NOTATION
      page: 492
      pdf_page: 516
statements: 15
exercises: 10
content_sha256: 3d28fa433a06aa2b8120633a18fd469f0f983647da5554d9c15e284517232bc8
translated_from: content/en/alg/III/05_s5_tensor_algebra_tensors.md
translation_method: google
source_content_sha256: d99f913e6231ffa43f0356d794c4b307be8a5cb9b275a18c87c2f41e23c6d2fe
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 49bb204824de13b60ca72d29222c0d1ea59bcba3b0d05096dbbdfeb3e2e025d5
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 5。 张量代数、张量

### 1. 张量代数中的定义模

设A为交换环，M为A-模。对于每个整数$n \geqslant 0$，$n$模的A-模张量积等于M（也称为M的第n个张量幂*）由$\bigotimes^n M$或$M^{\otimes n}$表示，或$T^n(M)$、或$T^n_A(M)$、或$\mathrm{Tens}^n(M)$；然后$T^1(M) = M$；我们也写$T^0(M) = A$。 A-模 *直和* $\bigoplus_{n \geqslant 0} T^n(M)$ 用$T(M)$ 或$\mathrm{Tens}(M)$ 表示。我们将在$T(M)$上对定义进行型$\mathbf{N}$的分级A-代数结构，通过定义整数$p \geqslant 0, q \geqslant 0$、A-线性映射的每个有序对
$$
m_{pq} : T^p(M) \otimes_A T^q(M) \to T^{p+q}(M)
$$
（$§ 3$、no. 1、*注*）。对于 $p > 0$ 和 $q > 0$，$m_{pq}$ 为结合性同构（II、$§ 3$、no. 9），当 $p = 0$（分别为 $q = 0$）时，$m_{0,q}$ 为$A \otimes_A T^q(M)$的典范同构到$T^q(M)$（$m_{p,0}$是$T^p(M) \otimes_A A$的典范同构到$T^p(M)$（II、$§ 3$、no. 4、命题 4））。然后，对于$x_i \in M$，$\alpha \in A$，
$$
\begin{align}
(x_1 \otimes \cdots \otimes x_p) \cdot (x_{p+1} \otimes \cdots \otimes x_{p+q}) &= x_1 \otimes \cdots \otimes x_p \otimes x_{p+1} \otimes \cdots \otimes x_{p+q} \\
\alpha \cdot (x_1 \otimes \cdots \otimes x_p) &= \alpha(x_1 \otimes \cdots \otimes x_p).
\end{align}
$$
因此在 $T(M)$ 上定义的乘法是直接的，它是*结合的*，并且承认为 $A = T^0(M)$ 的单位元单位元 1。

#### 定义 1 {#alg-iii-s5-def-1 .statement tag=061H}

对于交换环 $A$、张量代数 $M$ 上的每个模 $M$，用 $T(M)$、或$\mathrm{Tens}(M)$、或$T_A(M)$ 表示，则为代数 $\bigoplus_{n \geq 0} T^n(M)$ 和乘法在 (1) 中定义。 典范嵌入 $\phi : T^1(M) \to T(M)$ (II, § 1, no. 12)（也用$\phi_M$表示）被称为$M$的典范嵌入到$T(M)$。

#### 命题 1 {#alg-iii-s5-prop-1 .statement tag=061I}

令 $E$ 为（单位）$A$-代数，而 $f : M \to E$ 为 $A$-线性映射。存在且仅有一个$A$-代数同态$g : T(M) \to E$使得$f = g \circ \phi$。

在其他字中，$(T(M), \phi)$是普遍映射问题的解（集合理论，IV, § 3, no. 1），其中$\Sigma$是$A$-代数结构的类， $\alpha$-映射是从模$M$到$A$-代数的$A$-线性映射。请注意，这里不存在 $T(M)$ 毕业的问题。

For every finite family $(x_i)_{1 \leq i \leq n}$ of $n$ elements of $M$, by definition of the product in $T(M)$, $x_1 \otimes x_2 \otimes \cdots \otimes x_n = \phi(x_1)\phi(x_2)\ldots\phi(x_n)$; then necessarily $g(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1)f(x_2)\ldots f(x_n)$ for $n \geq 1$ and $g(\alpha) = \alpha e$ (if $e$ is the unit element of $E$) for $\alpha \in A$, which proves the uniqueness of $g$. Conversely, note that, for all $n > 0$, the mapping
$$
(x_1, \ldots, x_n) \mapsto f(x_1)f(x_2)\ldots f(x_n)
$$
of $M^n$ into $E$ is $A$-multilinear; hence there corresponds to it an $A$-linear mapping $g_n : T^n(M) \to E$ such that
$$
g(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1)f(x_2)\ldots f(x_n).
$$
Also we define the mapping $g_0 : T^0(M) \to E$ as equal to $\eta_E$ ($§ 1$, no. 3), in other words $g_0(\alpha) = \alpha e$ for $\alpha \in A$. 令$g$为$T(M)$到$E$的唯一$A$线性映射，其限制到$T^n(M)$为$g_n$（$n \geq 0$）； $g \circ \phi = g_1 = f$就是直接的，还有待验证$g$是$A$代数同态。 通过构造 $g(1) = e$ 并且通过线性足以表明 $g(uv) = g(u)g(v)$ 对于 $u \in T^p(M)$ 和 $v \in T^q(M)$ ($p > 0, q > 0$)；现在从公式 (1) 和 (2) 可以得出，当 $u = x_1 \otimes x_2 \otimes \cdots \otimes x_p$ 和 $v \in x_{p+1} \otimes \cdots \otimes x_{p+q}$（其中 $x_i$ 属于到 $E$）时，关系为真。 因此，对于 $u \in T^p(M)$ 和 $v \in T^q(M)$ 来说，线性关系成立。

#### 注 {#alg-iii-s5-n1-rem-1 .statement tag=061J}

假设 $E$ 是型 $\mathbf{Z}$ 的分级 $A$ 代数，毕业为 $(E_n)$，并且还假设
$$
f(M) \subset E_1.
$$
然后从 (2) 得出，$g(T^p(M)) \subset E_p$ 对于所有 $p \geq 0$，因此 $g$ 是分级的代数同态。

### 2. 张量代数的函数性质

#### 命题 2 {#alg-iii-s5-prop-2 .statement tag=061K}

令$A$为交换环、$M$和$N$两个$A$模块，并且
$$
u : M \to N
$$

A-线性映射。存在且仅有一个 A-代数同态

$$
u': \mathbf{T}(M) \to \mathbf{T}(N)
$$

这样图表

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M & & \downarrow \phi_N \\
\mathbf{T}(M) & \xrightarrow{u'} & \mathbf{T}(N)
\end{array}
$$

是可交换的。此外，$u'$是分级的代数同态。

$u'$的存在性和唯一性从no. 1、命题1出发，应用于代数$\mathbf{T}(N)$和线性映射$\phi_N \circ u : M \to \mathbf{T}(N)$；作为

$$
u(M) \subset \mathbf{T}^1(N) = N,
$$

事实上，$u'$ 是分级的代数同态，是从 no. 1 的注得出的。

命题 2 中的同态 $u'$ 今后将用$\mathbf{T}(u)$ 表示。如果 P 为 A-模且 $v : N \to P$ A-线性映射，则

$$
\mathbf{T}(v \circ u) = \mathbf{T}(v) \circ \mathbf{T}(u)
$$

对于 $\mathbf{T}(v) \circ \mathbf{T}(u)$ 是代数同态渲染可交换图表

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\downarrow \phi_M & & \downarrow \phi_P \\
\mathbf{T}(M) & \xrightarrow{\mathbf{T}(v) \circ \mathbf{T}(u)} & \mathbf{T}(P)
\end{array}
$$

$\mathbf{T}(u)$ 是有时，称为 $u$ 到 $\mathbf{T}(M)$ 的规范扩张（其中包含 $M = \mathbf{T}^1(M)$）。 注限制 $\mathbf{T}^n(u) : \mathbf{T}^n(M) \to \mathbf{T}^n(N)$ 只是线性映射 $u^{\otimes n} = u \otimes u \otimes \cdots \otimes u$（n 次），对于

$$
\mathbf{T}^n(u)(x_1 \otimes \cdots \otimes x_n) = u(x_1) \otimes \cdots \otimes u(x_n)
$$

因为$\mathbf{T}(u)$是代数同态和$\mathbf{T}^1(u) = u$； 限制$\mathbf{T}^0(u)$到A是恒等映射。 $\mathbf{T}^n(u)$称为$u$的第$n$第张量幂。

#### 命题 3 {#alg-iii-s5-prop-3 .statement tag=061L}

*如果$u : M \to N$是满射A-线性映射，则同态$\mathbf{T}(u) : \mathbf{T}(M) \to \mathbf{T}(N)$是满射，其核是由$u$的核$P \subset M \subset \mathbf{T}(M)$生成的$\mathbf{T}(M)$的两侧理想。*

$\mathbf{T}^0(u) : \mathbf{T}^0(M) \to \mathbf{T}^0(N)$ 是双射且对于每个整数 $n > 0$，

$$
\mathbf{T}^n(u) : \mathbf{T}^n(M) \to \mathbf{T}^n(N)
$$

是满射的，正如使用 II, § 3, no. 6、命题 6 在 $n$ 上看到的归纳一样；后者命题还通过$n$上的归纳显示，$T^n(u)$的核$\mathfrak{I}_n$是乘积生成的$T^n(M)$的子模
$$
x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$
其中 $x_i$ 属于至 $P$ 中至少之一。由此可见，$T(u)$的核$\mathfrak{I} = \bigoplus_{n \geq 1} \mathfrak{I}_n$是$P$在$T(M)$生成的双边理想。

如果 $u : M \to N$ 是*单射* 线性映射，则 $T(u)$ 并不总是真单射映射 (习题 1)。然而，当$u$是单射使得$u(M)$是$N$的*直因子*时，这是正确的，因为那么存在线性映射$v : N \to M$使得$v \circ u$是$M$上的恒等映射，因此
$$
T(v \circ u) = T(v) \circ T(u)
$$
是$T(M)$上的恒等映射，因此$T(u)$是单射的，其像（与$T(M)$同构的）是$T(N)$的*直因子*（II, § 1, no. 9，命题15）。更准确地说：

#### 命题 4 {#alg-iii-s5-prop-4 .statement tag=061M}

*令$N$和$P$是$A$模块$M$的两个子模，这样它们的和$N + P$是$M$中的直因子，并且它们的交$N \cap P$是$N$和$P$中的直因子。然后同态 $T(N) \to T(M)$、$T(P) \to T(M)$ 和*
$$
T(N \cap P) \to T(M),
$$
* 典范嵌入的典范扩张是单射的；如果$T(N)$、$T(P)$和$T(N \cap P)$通过这些同态与$T(M)$中的子代数进行识别，那么*
(5)
$$
T(N \cap P) = T(N) \cap T(P).
$$

到假设，存在子模$N' \subset N$和$P' \subset P$使得$N = N' \oplus (N \cap P)$，$P = P' \oplus (N \cap P)$；然后
$$
N + P = N' \oplus P' \oplus (N \cap P)
$$
并且存在 $M$ 的假设子模 $M'$ 使得
$$
M = M' \oplus (N + P) = M' \oplus N' \oplus P' \oplus (N \cap P) \\
= M' \oplus P' \oplus N = M' \oplus N' \oplus P.
$$

特别是，$N + P$、$N$、$P$和$N \cap P$是$M$中的直因子，这意味着，正如上面所见，典范同态
$$
T(N + P) \to T(M), \quad T(N) \to T(M),
$$
$$
T(P) \to T(M), \quad T(N \cap P) \to T(M)
$$
是单射的。因此，三个代数、$T(N)$、$T(P)$和$T(N \cap P)$被识别为子代数或$T(N + P)$，而后者则被识别为子代数或$T(M)$；

写成$Q = N \cap P$，还需要证明，如果$T(Q)$、$T(N' \oplus Q)$、$T(P' \oplus Q)$与$T(N' \oplus P' \oplus Q)$的子代数一致，则

$$
T(N' \oplus Q) \cap T(P' \oplus Q) = T(Q).
$$

现在，考虑交换律图表

$$
\begin{array}{ccc}
N' \oplus Q & \longrightarrow & N' \oplus P' \oplus Q \\
\downarrow & & \downarrow \\
Q & \longrightarrow & P' \oplus Q
\end{array}
$$

其中水平箭头是典范嵌入，垂直箭头是规范的投影。我们推导出可交换的图表

$$
\begin{array}{ccc}
T(N' \oplus Q) & \overset{u}{\longrightarrow} & T(N' \oplus P' \oplus Q) \\
\downarrow r & & \downarrow s \\
T(Q) & \overset{v}{\longrightarrow} & T(P' \oplus Q)
\end{array}
$$

其中$r$和$s$是满同态（命题3）和$u$和$v$单同态。因此，要证明(6)，注右手边显然包含在左手边；因此只需验证如果

$$
x \in T(N' \oplus Q) \cap T(P' \oplus Q),
$$

然后$x \in T(Q)$。现在同态$s$的定义显示其限制到$T(P' \oplus Q)$（用$T(N' \oplus P' \oplus Q)$的子代数识别）为恒等映射；因此，$x$上的假设意味着$s(u(x)) = x$。但还有$v(r(x)) = x$，其他字，$x$，属于到像，$T(Q)$在$T(P' \oplus Q)$，这有待证明。

#### 注 {#alg-iii-s5-n2-rem-1 .statement tag=061N}

注特别是，当$A$为域（II, § 7, no. 3，命题4）时，命题4的假设对于$M$的任意子模$N, P$始终成立。此外，如果$N \subset P$和$N \neq P$，则$T^n(N) \neq T^n(P)$对于所有$n \geq 1$，因为如果$R$是$N$中$P$的补集，则$T^n(P) \cap T^n(R) = \{0\}$通过(4)和$T^n(R) \neq \{0\}$。

#### 推论{#alg-iii-s5-n2-cor-1 .statement tag=061O}

*令$K$为交换域且$M$向量空间大于$K$。对于每个元素$z \in T(M)$，都存在$M$的最小的向量空间$N$，使得$z \in T(N)$和$N$的有限秩超过$K$。*

在这个叙述中可以理解，对于$M$的每个向量子空间$P$，$T(P)$被规范地标识为$T(M)$的子代数。让$z \in T(M)$； $z$可以表示为线性组合 of 元素，其中每一个都是$M = T^1(M)$的元素的有限乘积； $M$ 中的所有元素出现在有限秩和 $z \in T(Q)$ 中的乘积生成向量子空间 $Q$。

令 $\mathscr{F}$ 为向量子空间 $P$ 有限秩的（非空）集合，使得 $z \in T(P)$。 $\mathscr{F}$ 的元素中的每个递减序列都是静止的，因为它们是有限秩中的向量空间。因此 $\mathscr{F}$ 具有最小元素 $N$（集合理论，III, § 6, no. 5）。还需要验证每个 $P \in \mathscr{F}$ 包含于 $N$；现在，$z \in T(P) \cap T(N) = T(P \cap N)$（命题4）；鉴于$N$的定义，这意味着$N \cap P = N$，即$P \supset N$。

$M$ 的子空间 $N$ 据说与 $z$ *相关联。

### 3. 标量的环中的扩张

令$A, A'$为两个交换环和$\rho : A \to A'$环同态。令$M$为$A$模，$M'$为$A'$模，$u : M \to M'$为$A$同态；因为典范嵌入 $\phi_{M'} : M' \to T_{A'}(M')$ 也是 $A$ 同态（通过标量的限制），合成 $M \xrightarrow{u} M' \xrightarrow{\phi_{M'}} T_{A'}(M')$ 也是如此。推导出$A$-代数同态$T_A(M) \to \rho^*(T_{A'}(M'))$（no. 2），也记为$T(u) : T_A(M) \to T_{A'}(M')$，这是唯一的$A$-同态渲染交换交换图表

$$
\begin{array}{ccc}
M & \xrightarrow{u} & M' \\
\downarrow \phi_M & & \downarrow \phi_{M'} \\
T_A(M) & \xrightarrow{T(u)} & T_{A'}(M')
\end{array}
$$

如果$\sigma : A' \to A''$是交换环同态，$M''$是$A''$模，$v : M' \to M''$是$A'$同态，则上面的唯一性性质表明：

$$
T(v \circ u) = T(v) \circ T(u).
$$

#### 命题 5 {#alg-iii-s5-prop-5 .statement tag=061P}

*令$A, B$为两个交换环、$\rho : A \to B$、环、同态和$M$一个$A$模块。规范的扩张*

$$
\psi : T_B(B \otimes_A M) \to B \otimes_A T_A(M)
$$

*B-线性映射* $l_B \otimes \phi_M : B \otimes_A M \to B \otimes_A T_A(M)$ *是分级 B 代数的同构*。

考虑两个 $A$ 代数同态：典范嵌入 $j : B = T^0(B \otimes_A M) \to T(B \otimes_A M)$ 和同态

$$
h = T(i) : T(M) \to T(B \otimes_A M)
$$

从规范 $A$ 线性映射导出 (cf. 公式 (8))

$$
i : M \to B \otimes_A M.
$$

由于$T^0(B \otimes_A M)$包含在$T(B \otimes_A M)$中的中心中，因此可以应用§ 4, no. 2中的命题 5个以及A-代数同态

$$
\psi': B \otimes_A T(M) \to T(B \otimes_A M)
$$

得到这样的结果，对于$\beta \in B, x_i \in M$对于$1 \leq i \leq n$，

$$
\psi'(\beta \otimes (x_1 \otimes x_2 \otimes \cdots \otimes x_n)) = \beta((1 \otimes x_1) \otimes (1 \otimes x_2) \otimes \cdots \otimes (1 \otimes x_n)),
$$

这立即表明 $\psi'$ 也是 B 代数同态。只需证明$\psi \circ \psi'$和$\psi' \circ \psi$分别在$B \otimes_A T(M)$和$T(B \otimes_A M)$上是恒等映射即可。现在，这两个代数是由$B \otimes_A M$生成的，显然是$\psi \circ \psi'$和$\psi' \circ \psi$重合与恒等映射在$B \otimes_A M$、从而的结论。

### 4. 直极限张量代数

设$(A_\alpha, \phi_{\beta \alpha})$为交换环的有向直接系统和$A_\alpha$模块(II, § 6, no. 2)的$(M_\alpha, f_{\beta \alpha})$直接系统；让$A = \lim \rightarrow A_\alpha$和$M = \lim \rightarrow M_\alpha$，这是一个$A$模块。对于 $\alpha \leq \beta$，$A_\alpha$-代数同态 (no. 3, 公式 (8)) $f'_{\beta \alpha} = T(f_{\beta \alpha}): T_{A\alpha}(M_\alpha) \to T_{A\beta}(M_\beta)$ 是从 $A_\alpha$-同态 $f_{\beta \alpha}: M_\alpha \to M_\beta$ 规范导出的，并且从 (9) (no. 3) 可以得出 $(T_{A\alpha}(M_\alpha), f'_{\beta \alpha})$ 是*$A_\alpha$-代数的直接系统*。另一方面，令 $f'_\alpha: M_\alpha \to M$ 为规范的 $A_\alpha$ 同态；推导出$A_\alpha$-代数同态$f'_\alpha: T_{A\alpha}(M_\alpha) \to T_A(M)$ (no. 3, 公式 (8))，并且还可以从 (9) (no. 3) 得出$f'_\alpha$构成$A_\alpha$同态的直接系统。

#### 命题 6 {#alg-iii-s5-prop-6 .statement tag=061Q}

*A-同态* $f' = \lim \rightarrow f'_\alpha : \lim \rightarrow T_{A\alpha}(M_\alpha) \to T_A(M)$ *是分级的代数同构*。

为了简化，我们写 $E = T_A(M)$ 和 $E' = \lim \rightarrow T_{A\alpha}(M_\alpha)$ 并让

$$
g_\alpha: T_{A\alpha}(M_\alpha) \to E'
$$

是规范的$A_\alpha$同态。显然，复合 $A_\alpha$-线性映射 $M_\alpha \xrightarrow{\phi_{M_\alpha}} T_{A\alpha}(M_\alpha) \xrightarrow{g_\alpha} E'$ 形式直接系统，因此存在且仅有一个 $A$-线性映射 $u = \lim \rightarrow (g_\alpha \circ \phi_{M_\alpha}): M \to E'$ 使得

$$
u \circ f_\alpha = g_\alpha \circ \phi_{M_\alpha}
$$

对于所有$\alpha$。这个映射本身将 (no. 1, 命题 1) 唯一分解为 $M \xrightarrow{\phi_M} E \to E'$，其中 $h$ 是 $A$ 代数同态。只要证明$h \circ f' = 1_{E'}$和$f' \circ h = 1_E$就足够了。

为此注，对于每个指标 $\alpha$，(no. 3, 公式 (8))

$$
h \circ f'_\alpha \circ \phi_{M_\alpha} = h \circ \phi_M \circ f_\alpha = u \circ f_\alpha = g_\alpha \circ \phi_{M_\alpha}
$$

从而，由no. 1、命题 1 的唯一性断言，

$$
h \circ f'_\alpha = g_\alpha
$$

对于所有$\alpha$；由此可见，$(h \circ f') \circ g_\alpha = g_\alpha$对于所有$\alpha$，因此$h \circ f' = 1_{E'}$乘以定义或直极限。

另一方面，凭借no. 3，公式 (8)，

$$
f' \circ u \circ f_\alpha = f' \circ g_\alpha \circ \phi_{M_\alpha} = f'_\alpha \circ \phi_{M_\alpha} = \phi_M \circ f_\alpha,
$$

直极限定义又$f' \circ u = \phi_M$ 从而；我们将no. 1、命题 1 的$f' \circ h \circ \phi_M = \phi_M$和唯一性性质结论给出$f' \circ h = 1_E$。

命题 6 也可以由注意到证明，对于每个整数 $n \geq 1$，都有一个规范的 $A$-模块同构 $\lim \rightarrow T^n_{A_\alpha}(M_\alpha) \to T^n_A(M)$，如下由 II, § 6, no. 3、命题的 $n$ 上的归纳表示7.立即验证这些同构是$f'$中的限制。

### 5.张量代数直和。 张量代数自由模。 张量代数已分级模

令$A$为$A$模块族中的交换环和$M = \bigoplus_{\lambda \in L} M_\lambda$直和。从II, § 3, no. 7，命题 7，到$n$上的归纳，$T^n(M)$是子模直和典范嵌入像

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n} \to T^n(M) = M^{\otimes n}
$$

相对于*所有* 序列 $(\lambda_i) \in L^n$。将$M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n}$与这个像进行识别，可知$T(M)$是所有模*中的*直和

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n}
$$

其中$n$穿过$\mathbf{N}$，对于每个$n$，$(\lambda_i)$穿过$L^n$。

我们首先推导出以下推论：

#### 定理 1 {#alg-iii-s5-thm-1 .statement tag=061R}

*令$A$为交换环，$M$为免费的$A$模块，$(e_\lambda)_{\lambda \in L}$基为$M$。 然后元素$e_s = e_{\lambda_1} \otimes e_{\lambda_2} \otimes \cdots \otimes e_{\lambda_n}$，其中$s = (\lambda_1, \ldots, \lambda_n)$贯穿$L$的元素和$e_\varnothing$的所有有限序列的集合，用来表示$T(M)$的单位元，形式基 $A$-模块$T(M)$.*

这个基的元素显然是齐次的，乘法表由下式给出

$$
e_s e_t = e_{st}
$$

其中$st$表示通过*并置*序列$s$和$t$（I, § 7, no. 2）获得$L$的元素的序列。

可以看出，$T(M)$的基$(e_s)$与律(10)的乘法同构于集合$L$(I, § 7, no. 2)的*自由幺半群*，同构由映射每个获得这个幺半群的字$s$到元素$e_s$。由此可知 (§ 2, no. 7) 自由模 $M$ 的 *张量代数 $T(M)$，以及索引集合 $L$ 的基，规范地同构于 的自由结合律代数 $L$超过$A$*。特别是（§ 2, no. 7，命题 7），对于从$L$到$A$-代数$E$的每个映射$f : L \to E$，存在且仅有一个$A$-代数同态$\bar{f} : T(M) \to E$，使得$\bar{f}(e_\lambda) = f(\lambda)$。

#### 注 {#alg-iii-s5-n5-rem-1 .statement tag=061S}

上述结果同样可以作为张量代数的自由结合律代数的普遍性质的推论，使用II, § 3, no. 7、推论2到命题7得到。

#### 推出{#alg-iii-s5-n5-cor-1 .statement tag=061T}

*如果 $M$ 是射影 $A$ 模，则 $T(M)$ 是射影 $A$ 模。*

$M$ 是自由 $A$ 模块 $N$ (II, § 2, no. 2, 命题 4) 的直因子，因此 $T(M)$ 是 $T(N)$ (no. 2) 的直因子；由于 $T(N)$ 是自由的 (定理 1)，这表明 $T(M)$ 是射影 (II, § 2, no. 2)。

#### 命题 7 {#alg-iii-s5-prop-7 .statement tag=061U}

*令$\Delta$为可交换幺半群，$M$为型$\Delta$的分级$A$模，以及$(M_\alpha)_{\alpha \in \Delta}$其毕业。对于每个有序对$(\alpha, n) \in \Delta \times \mathbf{N}$，令$T^{\alpha, n}(M)$为$T^n(M)$的子模$M_{\alpha_1} \otimes M_{\alpha_2} \otimes \cdots \otimes M_{\alpha_n}$的（直接的）和，使得$\sum_{i=1}^n \alpha_i = \alpha$；那么 $(T^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ 是型 $\Delta \times \mathbf{N}$ 的唯一分级，与 $T(M)$ 上的代数结构兼容，并在 $M = T^1(M)$ 上引入给定的分级。*

在本号的开头已经看到了。 $T(M)$是$T^{\alpha, n}(M)$的直和，并且这是与代数结构兼容的毕业事实，紧随定义而来。如果$({T'}^{\alpha, n})$是型$\Delta \times \mathbf{N}$在$T(M)$上的另一个分级，与代数结构兼容，并且${T'}^{\alpha, 1}(M) = {T'}^{\alpha, 1}$对于$\alpha \in \Delta$，则立即从定义得出，对于所有$n \geq 1$ 以及所有 $\alpha \in \Delta$、$T^{\alpha, n}(M) \subset {T'}^{\alpha, n}$；但由于$T(M)$也是$T^{\alpha, n}(M)$的直和，这意味着${T'}^{\alpha, n} = T^{\alpha, n}(M)$（II, § 1, no. 8，*注*）。

### 6.张量和张量记号

令$A$为交换环，$M$为$A$模，$M^*$为$M$（II, § 2, no. 3）的*对偶*，以及$I$和$J$两个*不相交的有限* 集合； $A$-模块$\bigotimes_{i \in I \cup J} E_i$，其中，如果$i \in I$则为$E_i = M$，如果$i \in J$则为$E_i = M^*$，由$T^I_J(M)$表示； $T^I_J(M)$的元素在$M$上被称为型*$(I, J)$的*张量。如果 $J = \varnothing$，则称为“逆变”；如果 $I = \varnothing$，则称为“协变”；否则称为“混合”。

令$I', I''$为$I$的两个子集和$J', J''$为$J$的两个子集，使得$I' \cup I'' = I$，

$I' \cap I'' = \varnothing,\ J' \cup J'' = J,\ J' \cap J'' = \varnothing$；那么有一个规范的结合性同构 (II, § 3, no. 9)

$$
T_J^I(M) \to T_{J'}^{I'}(M) \otimes_A T_{J''}^{I''}(M).
$$

考虑到张量代数 $T(M \oplus M^*)$，从 no. 5 可以得出，$T^n(M \oplus M^*)$ 与 $T_J^I(M)$ 的直和被规范地识别，其中我遍历区间 $\{1, n\}$ 的子集的集合 $\mathbf{N}$和$J$是$\{1, n\}$中I的补集。

当 $I = \{1, p\}$ 和 $J = \{p + 1, p + q\}$ 与整数 $p \geq 0,\ q \geq 0$ 时（其中替换 I（分别为 J）乘以 $\varnothing$，当 $p = 0$（分别为 $q = 0$））时，A-模 $T_J^I(M)$ 也表示为$T_q^p(M)$；因此，A-模$T_0^n(M)$和$T_n^0(M)$分别是定义A-模$T^n(M)$和$T^n(M^*)$。当 I 和 J 是基数 $p = \mathrm{Card}(I)$ 和 $q = \mathrm{Card}(J)$ 的任意有限集合时，我们给它们每个人一个全序；那么存在 I（或 J）的递增双射到 $\{1, p\}$（或 $\{p + 1, p + q\}$），并且这些双射因此定义同构

$$
T_J^I(M) \to T_q^p(M).
$$

当M是*有限生成射影*A-模时，从II, § 2, no. 7，推论4到命题13和II, § 4, no. 4，推论1到命题4，有典范同构

$$
(T_J^I(M))^* \to T_I^J(M).
$$

现在假设 M 是一个*有限生成的自由*A-模，并让 $(e_\lambda)_{\lambda \in L}$ 是 M 的基（因此 L 是一个*有限*集合）。 $M^*$ *对偶* 到$(e_\lambda)$ (II, § 2, no. 6) 的基由$(e^\lambda)_{\lambda \in L}$ 表示。 M 和 $M^*$ 的基 $(e_\lambda)$ 和 $(e^\lambda)$ 分别为 $T_J^I(M)$ 的定义 (no. 5) 基，我们明确给出如下：给定两个映射 $f : I \to L$ 和$g : J \to L$，令 $e_f^g$ 为 $T_J^I(M)$ 的元素 $\bigotimes_{i \in I \cup J} x_i$ 定义为

$$
x_i = e_{f(i)} \quad \text{if } i \in I, \qquad x_i = e_{g(i)} \quad \text{if } i \in J.
$$

当$(f, g)$穿过映射$f : I \to L$和$g : J \to L$的有序对的集合时，$e_f^g$形式A-模$T_J^I(M)$的一个*基*，说是*关联*给定 M 的基 $(e_\lambda)$。对于 $z \in T_J^I(M)$，我们可以这样写

$$
z = \sum_{(f, g)} \alpha_g^f(z) \cdot e_f^g
$$

其中$\alpha_g^f$是相对于基$(e_f^g)$的坐标形式；通过滥用语言，$\alpha_g^f(z)$被称为张量$z$*相对于模M的基*$(e_\lambda)$的坐标。$\alpha_g^f$构成$(e_f^g)$的对偶基，在其他字中它们被识别为$T_I^J(M)$ 的基的元素，与$(e_\lambda)$ *关联*。当 I 和 J 互补时，$\mathbf{N}$ 的区间 $\{1, n\}$ 的子集，$\alpha_g^f$（或$\alpha_g^f(z)$）表示如下：$i \in I$ 的每个元素 $f(i)$ 写为第 i 个位置的上指标，其中第 i 个位置的点为 $i \in J$；类似地，$i \in J$的$g(i)$在第i个位置写为较低的指标，并在第i个位置写一个点作为$i \in I$。对于例，对于$I = \{1, 4\}, J = \{2, 3\}$，我们写为$\alpha_{v\rho}^{\lambda\cdot\cdot\mu}$：如果$f(1) = \lambda, f(4) = \mu, g(2) = \nu, g(3) = \rho$。

设$(\tilde{e}_{\lambda})_{\lambda \in L}$为M的另一个基，从$(e_{\lambda})$到$(\tilde{e}_{\lambda})$（II, § 10, no. 8），经过为P矩阵。那么从$(e^{\lambda})$到$(\tilde{e}^{\lambda})$（$(\tilde{e}_{\lambda})$的对偶基）的经过的矩阵就是P（II, § 10, no. 8，命题5）的同余$^tP^{-1}$。由此可知 (II, § 10, no. 10) 经过的矩阵从 $T^{I}_{J}(M)$ 的基 $(e^{g}_{f})$ 到基 $(\tilde{e}^{g}_{f})$（其中 $f$（分别为 $g$）穿过集合 I 到 L 的映射（分别是 J 到 L））是矩阵

$$
\bigotimes_{i \in I \cup J} Q_{i}, \quad \text{where } Q_{i} = P \text{ if } i \in I, Q_{i} = {}^{t}P^{-1} \text{ if } i \in J.
$$

因此，这个矩阵中的转置被识别为

$$
\bigotimes_{i \in I \cup J} R_{i}, \quad \text{where } R_{i} = {}^{t}P^{-1} \text{ if } i \in I, R_{i} = P \text{ if } i \in J.
$$

现在假设 M 是任意模。设$i \in I, j \in J$并写出$I' = I - \{i\}, J' = J - \{j\}$；我们将定义规范的A-线性映射

$$
c^{i}_{j}: T^{I}_{J}(M) \to T^{I'}_{J'}(M),
$$

称为指标 i 和指标 j 的缩写。为此，$M^{I} \times (M^{*})^{J}$的注、映射，与每个家庭$(x_{i})_{i \in I \cup J}$相关联，其中$x_{i} \in M$如果$i \in I$和$x_{i} \in M^{*}$如果$i \in J$、元素

$$
\langle x_{i}, x_{j} \rangle_{k \in (I \cup J) - \{i, j\}} x_{k}
$$

$T^{I'}_{J'}(M)$，是A-多重线性； $c^{i}_{j}$ 是相应的 A-线性映射。

现在假设 M 是自由且有限生成的，并令 $(e_{\lambda})_{\lambda \in L}$ 为 M 的基。给定两个映射 $f: I \to L, g: J \to L$，令 $f_{i}$ 表示 $f$ 到 $I' = I - \{i\}$ 和 $g_{j}$ 的限制限制至 $g$ 至 $J' = J - \{j\}$；那么根据 (12)

$$
c^{i}_{j}(e^{g}_{f}) = \begin{cases} 0 & \text{if } f(i) \neq g(j) \\ e^{g_{j}}_{f_{i}} & \text{if } f(i) = g(j) \end{cases}
$$

得到$c^{i}_{j}(z)$坐标为z坐标函数的表达式；对于每个映射$f'$（分别$g'$）到L（或J'到L）和每个$\lambda \in L$，令$(f', \lambda)$（或$(g', \lambda)$）表示I到L（或J到L）的映射，其限制到I' (resp. J') 是 $f'$ (resp. $g'$) 并且在元素 i (resp. j) 处需要值 $\lambda$。那么，如果$T^{I'}_{J'}(M)$相对于基$(e^{g'}_{f'})$的坐标形式用$\beta^{f'}_{g'}$表示，

$$
\beta^{f'}_{g'}(c^{i}_{j}(z)) = \sum_{\lambda \in L} \alpha^{(f'; \lambda)}_{(g'; \lambda)}(z).
$$

例共张量。 (1) 设 M 为有限生成射影 A-模。我们知道（II, § 4, no. 2，命题 2 的推论），存在一个规范的 A-模同构

$$
\theta_M : M^* \otimes_A M \to \operatorname{End}_A(M)
$$

这样$\theta_M(x^* \otimes x)$（对于$x \in M, x^* \in M^*$）是自同态

$$
y \mapsto \langle y, x^*\rangle x.
$$

因此，通过$\theta_M$，$T^{(2)}_{\{1\}}(M)$（与$T^1_1(M)$同构的）可以与A-模$\operatorname{End}_A(M)$识别。假设M为自由模，令$(e_\lambda)_{\lambda \in L}$为M的基；那么张量$z \in M^* \otimes M$相对于这个模的基$(e^\mu \otimes e_\lambda)$的坐标就用$\zeta_{\mu \cdot \lambda}$来表示。由于$\theta_M(e^\mu \otimes e_\lambda)$为自同态$y \mapsto \langle y, e^\mu\rangle e_\lambda$，自同态$u = \theta_M(z) = \theta_M\left( \sum_{\lambda, \mu} \zeta_{\mu \cdot \lambda} e^\mu \otimes e_\lambda \right)$映射$y$至$\sum_{\lambda, \mu} \zeta_{\mu \cdot \lambda} \langle y, e^\mu\rangle e_\lambda$；写$y = e_\lambda$，我们得到关系

$$
u(e_\lambda) = \sum_{\mu \in L} \zeta_{\lambda \cdot \mu} e_\mu
$$

其它字、线性映射*$u = \theta_M(z)$*的*矩阵是指标*$\mu$*和指标*$\lambda$*行中的元素和列* $\zeta_{\lambda \cdot \mu}$。

$u$ (II, § 4, no. 3) 的*轨迹*的定义立即表明

$$
\operatorname{Tr}(\theta_M(z)) = c_1^2(z).
$$

因此元素$z_0 = \sum_{\lambda \in L} e^\lambda \otimes e_\lambda$（其坐标$\zeta_{\mu \cdot \lambda}$对于$\lambda \neq \mu$来说是零，对于$\lambda = \mu$等于1），这样$\theta_M(z_0) = 1_M$就是元素$1 \in A = T^0_0(M)$的像映射收缩的*转置*

$$
c_1^2 : T^{(2)}_{\{1\}}(M) \to A.
$$

(2) 假设M总是有限生成射影A-模；有一个规范的 A-模同构

$$
\mu : M^* \otimes_A M^* \to (M \otimes_A M)^*
$$

（II, § 4, no. 4，推论 1 至命题 2）和典范同构

$$
\theta : (M \otimes_A M)^* \otimes_A M \to \operatorname{Hom}_A(M \otimes_A M, M)
$$

（II, § 4, no. 2，命题 2 的推论）； $\operatorname{Hom}_A(M \otimes_A M, M)$ 也与 $M \times M$ 的 A-*双线性* 映射的 A-模 $\mathscr{L}_2(M, M; M)$ 典型地同构为 $M$ (II, § 3, no. 9)。组合这些同构，得到典范同构

$$
\chi_M : T^{(3)}_{\{1, 2\}}(M) = M^* \otimes M^* \otimes M \to \mathscr{L}_2(M, M; M)
$$

这样，对于 $M^*$、$z \in M$、$\chi_M(x^* \otimes y^* \otimes z)$ 中的 $x^*, y^*$ 来说，映射是双线性的
$$
(u, v) \mapsto \langle u, x^*\rangle \langle v, y^*\rangle z.
$$
因此，通过$\chi_M$，$T_{\{1, 2\}}^{(3)}(M)$（与$T_2^1(M)$同构的）可以与A-模$\mathscr{L}_2(M, M; M)$识别。假设M是自由A-模，令$(e_\lambda)_{\lambda \in L}$是M的基；那么张量$z \in M^* \otimes M^* \otimes M$相对于这个模的基$(e^\lambda \otimes e^\mu \otimes e_\nu)$的坐标就用$\zeta_{\lambda \mu \nu}$来表示。双线性映射 $\chi_M(z)$ 映射有序对 $(e_\lambda, e_\mu)$ 至
$$
\sum_{\nu \in L} \zeta_{\lambda \mu \nu} e_\nu
$$
因此 $\zeta_{\lambda \mu \nu}$ 只是由双线性映射 $\chi_M(z)$ 在 M 上定义的（通常是非关联的）代数的 * 结构* 常数，相对于基 $(e_\lambda)$ (§ 1, no. 7)。

#### 注 2 {#alg-iii-s5-n6-rem-2 .statement tag=061V}

设$(e_\lambda)_{\lambda \in L}$、$(\bar{e}_\lambda)_{\lambda \in L}$为从$(e_\lambda)$到$(\bar{e}_\lambda)$的通道的M和P矩阵的两个基。 根据*例 1*中的情况，指标$\lambda$和指标$\mu$的列行中出现的P的元素被表示为对手${}^tP^{-1}$的$\alpha_\mu^\lambda$和元素出现在指标$\mu$行中的指标$\lambda$和列的行记为$\beta_\lambda^\mu$。 然后（上面记号介绍过）
$$
\begin{cases}
\bar{e}_\mu = \sum_\lambda \alpha_\mu^\lambda e_\lambda \\
\bar{e}^\mu = \sum_\lambda \beta_\lambda^\mu e_\lambda
\end{cases}
$$
$$
\bar{e}_{f'}^{g'} = \sum_{(f', g)} \left( \prod_{i \in I} \alpha_{f'(i)}^{f(i)} \right) \left( \prod_{j \in J} \beta_{g(j)}^{g'(j)} \right) e_f^g
$$
对于所有映射 $f': I \to L$ 和 $g': J \to L$。 因此，张量 $z \in T_J^I(M)$相对于基$(e_\lambda)$的坐标$\zeta_g^f$可以使用公式表示为z相对于基$(\bar{e}_\lambda)$的坐标$\bar{\zeta}_{g'}^{f'}$的项
$$
\zeta_g^f = \sum_{(f', g')} \left( \prod_{i \in I} \alpha_{g'(i)}^{g(i)} \right) \left( \prod_{j \in J} \beta_{f'(j)}^{f(j)} \right) \bar{\zeta}_{g'}^{f'}
$$
从基$(\bar{e}_\lambda)$到基$(e_\lambda)$的矩阵$P^{-1}$是${}^tP^{-1}$的转置，所以$\beta_\lambda^\mu$就是列中出现的元素指标$\lambda$和$P^{-1}$的指标$\mu$行。 因此，在上述计算中，$\bar{e}_{f'}^{g'}$的项中的$e_f^g$和$\zeta_g^f$的项中的$\bar{\zeta}_{g'}^{f'}$的计算是由替换、$\alpha_\mu^\lambda$由$\beta_\lambda^\mu$和$\beta_\lambda^\mu$由$\alpha_\mu^\lambda$进行计算，交换$f$和$f'$以及$g$和$g'$的角色。 然后
$$
e_f^g = \sum_{(f', g')} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f'(i)}^{f(i)} \right) \bar{e}_{f'}^{g'}
$$

(23)
$$
\bar{\zeta}_{g'}^{f'} = \sum_{(f,g)} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f(i)}^{f'(i)} \right) \zeta_g^f.
$$

上述公式使得总和超过指标，其中一次作为下指标出现一次，一次作为上指标出现。由于这种情况，某些作者允许自己抑制求和符号。

### 习题{#alg-iii-s5-exercises}

§ 5](exercises/s5/)参见[习题。
