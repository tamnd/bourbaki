---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 6
section_title: Symmetric algebras
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 497-506, 632-633
pdf_pages: 0521-0530, 0656-0657
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE SYMMETRIC ALGEBRA OF A MODULE
      page: 497
      pdf_page: 521
    - "no": 2
      title: FUNCTORIAL PROPERTIES OF THE SYMMETRIC ALGEBRA
      page: 498
      pdf_page: 522
    - "no": 3
      title: n-th symmetric power of a module and symmetric multilinear mappings
      page: 500
      pdf_page: 524
    - "no": 4
      title: EXTENSION OF THE RING OF SCALARS
      page: 502
      pdf_page: 526
    - "no": 5
      title: DIRECT LIMIT OF SYMMETRIC ALGEBRAS
      page: 503
      pdf_page: 527
    - "no": 6
      title: SYMMETRIC ALGEBRA OF A DIRECT SUM. SYMMETRIC ALGEBRA OF A FREE MODULE. SYMMETRIC ALGEBRA OF A GRADED MODULE
      page: 503
      pdf_page: 527
statements: 17
exercises: 5
content_sha256: 99f99b2de96fe1898e62273bc5d5b765bacb3b3bb19d72795cc0d9729d0889b3
translated_from: content/en/alg/III/06_s6_symmetric_algebras.md
translation_method: google
source_content_sha256: a716a1c3cf99e3d34241000d92ee39248d92a3c9503fa59066fb7f864e19044c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: e0a2c075987c842239e35bb77d26baba4c42bc5cfc396e06fd62bc6f5ef7565c
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 6。对称代数

### 1. 模的对称代数的定义

#### 定义 1 {#alg-iii-s6-def-1 .statement tag=0626}

*设A为交换环，M为A-模。 M 的对称代数，表示为 S(M)、Sym(M) 或 S_A(M)，是由元素生成的双边理想 $\mathfrak{J}'$（也表示为 $\mathfrak{J}'_M$）对张量代数 T(M) 与 A 的商代数 T(M) 的 $xy - yx = x \otimes y - y \otimes x$，其中 x 和 y 穿过 M。*

由于理想$\mathfrak{J}'$是由次数2的齐次元素生成的，因此它是一个分级理想（II, § 11, no. 3，命题2）；我们写$\mathfrak{J}'_n = \mathfrak{J}' \cap T^n(M)$；然后，代数 S(M) 根据 $S^n(M) = T^n(M)/\mathfrak{J}'_n$ 的分级（称为规范）由……组成进行分级。现在 $\mathfrak{J}'_0 = \mathfrak{J}'_1 = \{0\}$ 以及$S^0(M)$ 被规范地标识为 A，$S^1(M)$ 被规范地标识为 $T^1(M) = M$；我们将始终在下面进行这些识别，并用$\phi'$或$\phi'_M$典范嵌入$M \to S(M)$表示。

#### 命题 1 {#alg-iii-s6-prop-1 .statement tag=0627}

*代数 S(M) 是可交换的。*

对于M中的$x, y$，通过定义$\phi'(x)\phi'(y) = \phi'(y)\phi'(x)$，如元素$\phi'(x)$，其中x穿过M，生成S(M)，从§ 1, no. 7得出结论。

#### 命题 2 {#alg-iii-s6-prop-2 .statement tag=0628}

*令 E 为 A-代数和 $f : M \to E$ A-线性映射，使得*
$$(1)$$
$$ f(x)f(y) = f(y)f(x) \text{ for all } x, y \text{ in } M. $$
*存在且仅有一个A-代数同态$g : S(M) \to E$使得$f = g \circ \phi'$。*

In other words, $(S(M), \phi')$ is a solution of the *universal mapping problem* (*Set Theory*, IV, § 3, no. 1), where $\Sigma$ is the species of A-algebra structure, the $\alpha$-mappings being the linear mappings of the A-module M to an A-algebra satisfying (1).

g 的唯一性由 $\phi'(M) = M$ 生成 S(M) 得出。证明 g, 注的存在性，根据 § 5, No. 1, 命题 1 存在 A-代数同态 $g_1 : T(M) \to E$ 使得 $f = g_1 \circ \phi;$

需要证明的是，在理想的$\mathfrak{J}'$上，$g_1$是零，那么，如果$p : T(M) \to S(M) = T(M)/\mathfrak{J}'$是典范同态，我们可以写成$g_1 = g \circ p$，其中$g : S(M) \to E$是代数同态，并且从$p \circ \phi = \phi'$得出结论。现在$g_1$的核是一个双面理想，根据(1)和关系$g_1 \circ \phi = f$，包含元素$x \otimes y - y \otimes x$对于$M$中的$x, y$。这样就完成了证明。

#### 注 {#alg-iii-s6-n1-rem-1 .statement tag=0629}

(1) 假设$E$是型$\mathbf{Z}$的分级$A$代数，毕业为$(E_n)$，并假设线性映射$f$（假设满足(1)）是这样的：
(2)
$$
f(M) \subset E_1.
$$
然后关系 $g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p)$ 与 $x_i \in M$ 表明 $g(S^p(M)) \subset E_p$ 对于所有 $p \geq 0$，因此 $g$ 是分级的代数同态。

(2) $S(M)$的每元素是形式$x_1 x_2 \ldots x_n$的乘积的和，其中$x_i$属于到$M$；应注意不要将$S(M)$中采用的乘积与$T(M)$中采用的类似乘积相混淆。

(3) 如果$n!.1$在$A$中可逆，则$A$模$S^n(M)$由形式$x^n$的元素生成，其中$x \in M$；这是从上面的注和I, § 8, no. 2，命题2得出的。

### 2.对称代数的函数性质

#### 命题 3 {#alg-iii-s6-prop-3 .statement tag=062A}

*令$A$为交换环、$M$和$N$两个$A$-模块和$u : M \to N$一个$A$-线性映射。存在且仅有一个 $A$-代数同态 $u' : S(M) \to S(N)$ 使得图表*

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi'_M & & \downarrow \phi'_N \\
S(M) & \xrightarrow{u'} & S(N)
\end{array}
$$

*is commutative.此外，$u'$是分级的代数同态。*

$u'$的存在性和唯一性源自no. 1、命题2应用于交换代数、$S(N)$和$f = \phi'_N \circ u : M \to S(N)$；作为
$$
f(M) \subset S^1(N) = N,
$$
事实上，$u'$ 是分级的代数同态，源自 no. 1，*注* 1。

命题 3 中的同态 $u'$ 今后将用$S(u)$ 表示。如果 $P$ 是$A$-模且 $v : N \to P$ $A$-线性映射，则
$$
S(v \circ u) = S(v) \circ S(u)
$$

对于 $S(v) \circ S(u)$ 是代数同态渲染可交换图表

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\downarrow \phi'_M & & \downarrow \phi'_P \\
S(M) & \xrightarrow{S(v) \circ S(u)} & S(P)
\end{array}
$$

由于$S(M)$包含$M = S^1(M)$，$S(u)$是有时，称为$u$到$S(M)$的*规范扩张*。 限制 $S^n(u): S^n(M) \to S^n(N)$ 是这样的
$$
S^n(u)(x_1 x_2 \ldots x_n) = u(x_1) u(x_2) \ldots u(x_n)
$$
其中$x_i \in M$，因为$S(u)$是代数同态和$S^1(u) = u$； 限制 $S^0(u)$ 至 $A$ 为恒等映射。 注 $S^n(u)$ 可以由 $T^n(u): T^n(M) \to T^n(N)$ 通过经过得到商。

#### 命题 4 {#alg-iii-s6-prop-4 .statement tag=062B}

*如果$u: M \to N$是满射$A$线性映射，则同态$S(u): S(M) \to S(N)$是满射，其核是由核$P \subset M \subset S(M)$生成$u$生成的$S(M)$的理想。*

我们写$v = T(u): T(M) \to T(N)$；我们知道 (§ 5, no. 2, 命题 3) $v$ 是满射的，因此从定义得出 $v(\mathfrak{J}'_M) = \mathfrak{J}'_N$；如果$\mathfrak{R}$是$v$的核，则$v^{-1}(\mathfrak{J}'_N) = \mathfrak{R} + \mathfrak{J}'_M$。由于$S(u): T(M)/\mathfrak{J}'_M \to T(N)/\mathfrak{J}'_N$是由$v$乘以经过的商得出的，所以它是满同态，其核是$\mathfrak{R}' = (\mathfrak{R} + \mathfrak{J}'_M)/\mathfrak{J}'_M$。由于$\mathfrak{R}$是由$u$（§ 5, no. 2）的核$P$生成，$\mathfrak{R}'$也是如此。

如果 $u: M \to N$ 是*单射* 线性映射，则 $S(u)$ 并不总是真单射映射 (习题 1)。然而，当$u$是单射时，$u(M)$是$N$中的*直因子*，然后$S(u)$的像（与$S(M)$同构的）是$S(N)$的*直因子*； 证明与 $T(u)$ (§ 5, no. 2) 替换 $T$ by $S$ 的类似断言相同。

#### 命题 5 {#alg-iii-s6-prop-5 .statement tag=062C}

*令$N$和$P$是$A$模块$M$的两个子模，这样它们的和$N + P$是$M$中的直因子，并且它们的交$N \cap P$是$N$和$P$中的直因子。然后同态 $S(N) \to S(M)$、$S(P) \to S(M)$ 和*
$$
S(N \cap P) \to S(M),
$$
* 典范嵌入的典范扩张是单射的；如果$S(N)$、$S(P)$和$S(N \cap P)$通过这些同态与$S(M)$中的子代数进行识别，那么*
$$
S(N \cap P) = S(N) \cap S(P).
$$
(4)

证明约化到 § 5, no. 2、命题 4 替换 $T$ $S$。当$A$为域时，命题5的假设对于$M$的*任意*子模$N, P$始终成立。

#### 推论{#alg-iii-s6-n2-cor-1 .statement tag=062D}

*设 K 为交换域且 M 向量空间超过 K。对于每个元素 $z \in S(M)$，存在 M 的最小的向量空间 N，使得 $z \in S(N)$ 和 N 是有限维的。*

证明源自§ 5, no. 2，由S推论命题4替换T。

N 称为 M 与 z *关联*的向量子空间。

### 3. 模的第 n 个对称幂和对称多线性映射

令X、Y为两个集合和$n$整数$\geqslant 1$。 $X^n$ 到 Y 的*对称映射* 是任意映射 $f : X^n \to Y$，使得对于每个置换 $\sigma \in \mathscr{S}_n$ 和每个元素 $(x_i) \in X^n$，

$$
f(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = f(x_1, x_2, \ldots, x_n).
$$

作为交换两个连续的整数生成群$\mathscr{S}_n$(I, § 5, no. 7)的转置，当$\sigma$是这样的转置时，条件(5)成立就足够了。

当Y是交换环A上的*模*时，显然$X^n$的对称映射到Y的集合是$X^n$的所有映射到Y的A-模$Y^{X^n}$的*子模*。

#### 命题 6 {#alg-iii-s6-prop-6 .statement tag=062E}

*设A为交换环，M和N为A-模。如果与每个 A-线性映射 $g : S^n(M) \to N$ ($n \geqslant 1$) 相关联，则 n 线性映射*

$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 x_2 \ldots x_n)
$$

*（在右侧，乘积取自代数$S(M)$），双射A-线性映射是从A-模$\operatorname{Hom}_A(S^n(M), N)$到A-模的$M^n$到N的对称n线性映射获得的。*

回想一下 (II, § 3, no. 9)，A-模 $\operatorname{Hom}_A(T^n(M), N)$ 的规范双射到 A-模 $\mathscr{L}_n(M, \ldots, M; N)$ 的*所有* n 线性映射$M^n$ 到 N 的映射是通过与每个 A-线性映射 $f : T^n(M) \to N$ 关联获得的 n 线性映射

$$
\tilde{f} : (x_1, x_2, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n).
$$

另一方面，A-线性映射$g : S^n(M) \to N$与A-线性映射$f : T^n(M) \to N$是一对一的对应，这样通过与$g$映射关联，$f$是零*on*$\mathfrak{J}'_n$ $f = g \circ p_n$，哪里

$$
p_n : T^n(M) \to S^n(M) = T^n(M)/\mathfrak{J}'_n
$$

是典范同态 (II, § 2, no. 1, 定理 1)。但由于$\mathfrak{J}'_n$是形式元素线性组合

$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes y - y \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$

n 个对称幂

(x, y, u_i, v_j in M)，说函数 f 是形式 g \circ p_n 意味着相应的 n-线性函数 $\bar{f}$ 满足关系

$$
\bar{f}(u_1, \ldots, u_p, x, y, v_1, \ldots, v_{n-p-2}) = \bar{f}(u_1, \ldots, u_p, y, x, v_1, \ldots, v_{n-p-2});
$$

在其他字中，根据上面的内容，这意味着$\bar{f}$是*对称*； 从而命题，考虑到这一事实

$$
p_n(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = x_1 x_2 \ldots x_n
$$

与$x_i \in M$。

A-模 $S^n(M)$ 被称为 M 的第 n 个对称幂*。对于每个 A-模同态 $u : M \to N$、映射 $S^n(u) : S^n(M) \to S^n(N)$ 其中重合与 $S(u)$ $S^n(M)$ 称为 u* 的第 n 个对称幂。

#### 注 {#alg-iii-s6-n3-rem-1 .statement tag=062F}

令$\mathfrak{S}_n$中的$\sigma$为置换；如映射

$$
(x_1, x_2, \ldots, x_n) \mapsto x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \cdots \otimes x_{\sigma^{-1}(n)}
$$

$M^n$ 到 $T^n(M)$ 是 A-多重线性，它可以唯一地写为

$$
(x_1, \ldots, x_n) \mapsto u_\sigma(x_1 \otimes x_2 \otimes \cdots \otimes x_n),
$$

其中$u_\sigma$是A-模$T^n(M)$的*自同态*，也用$z \mapsto \sigma . z$表示。显然，如果$\sigma$是$\mathfrak{S}_n$的单位元素，则$u_\sigma$就是恒等式；另一方面，写 $y_i = x_{\sigma^{-1}(i)}$，对于每个置换 $\tau \in \mathfrak{S}_n, y_{\tau^{-1}(i)} = x_{\sigma^{-1}(\tau^{-1}(i))}$，我们得到 $\tau . (\sigma . z) = (\tau \sigma) . z$；其他字、A-模$T^n(M)$是运算$(\sigma, z) \mapsto \sigma . z$（I, § 5, no. 1）下的左$\mathfrak{S}_n$-*集合*。 $T^n(M)$ 的元素使得 *所有* $\sigma \in \mathfrak{S}_n$ 的 $\sigma . z = z$ 被称为（逆变）* 阶 n* 的对称张量；它们形式是$T^n(M)$的子A模块$S'_n(M)$。

对于所有$z \in T^n(M)$，我们写成$s . z = \sum_{\sigma \in \mathfrak{S}_n} \sigma . z$并称$s . z$为张量$z$的*对称化*；显然$s . z$是对称的张量，因此$z \mapsto s . z$是$T^n(M)$的自同态，其中像$S''_n(M)$包含在$S'_n(M)$中；一般来说，$S''_n(M) \neq S'_n(M)$（习题5）。如果$z$是对称张量，则$s . z = n! z$；由此可知 *当 n!在A*中是可逆的，自同态$z \mapsto (n!)^{-1} s . z$是$T^n(M)$(II, § 1, no. 8)的*投影算子*，其像是$S'_n(M) = S''_n(M)$；而且这个投影算子上的*核*只是$\mathfrak{J}'_n$。因为，显然所有$\sigma \in \mathfrak{S}_n$和$\mathfrak{J}'_n$的$\sigma(\mathfrak{J}'_n) \subset \mathfrak{J}'_n$都是由张量$z - \rho . z$生成定义，其中$\rho$是$\{1, n\}$中两个连续数的转置；另外，如果$\sigma, \tau$是$\mathfrak{S}_n$中的两个置换，则$z - (\sigma \tau) . z = z - \sigma . z + \sigma . (z - \tau . z)$，从而（因为$\mathfrak{S}_n$中的每个置换都是交换两个连续数的换位的乘积）$z - \sigma . z \in \mathfrak{J}'_n$对于所有 $z \in T^n(M)$ 和 $\sigma \in \mathfrak{S}_n$。因此（始终假设 n! 在 A 中可逆），可以看出

$$
z - (n!)^{-1} s . z = \sum_{\sigma \in \mathfrak{S}_n} (n!)^{-1} (z - \sigma . z) \in \mathfrak{J}'_n
$$

对于所有$z \in T^n(M)$，这证明了我们的断言。

当$n!$在$A$可逆时，$T^n(M)$的子模、$S'_n(M)$和$\mathfrak{g}'_n$因此是互补的，并且典范同态$T^n(M) \to S^n(M) = T^n(M)/\mathfrak{g}'_n$的限制到$S'_n(M)$是一个$A$-模块同构，它允许我们在设想的情况下将阶$n$的认同对称张量与$M$的第$n$对称幂进行元素。 注然而，该标识与两个对称张量的乘法、乘积（在$T(M)$中）不兼容，一般来说不对称，因此不具有对称对称的像的$S(M)$乘积中的像考虑张量。

### 4. 标量的环中的扩张

令$A, A'$为两个交换环、$\rho : A \to A'$环同态、$M$一个$A$模、$M'$一个$A'$模和$f : M \to M'$一个$A$同态（相对于$\rho$）的$M$变成$M'$。复合映射$M \xrightarrow{f} M' \xrightarrow{\phi_{M'}} S_{A'}(M')$是$M$到交换代数$\rho_*(S_A(M'))$的$A$线性映射；则存在 no. 1, 命题 2) 唯一一个 $A$ 同态代数 $f' : S_A(M) \to S_{A'}(M')$ 呈现可交换图表

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\downarrow \phi_M' & & \downarrow \phi_{M'}' \\
S_A(M) & \xrightarrow{f'} & S_{A'}(M')
\end{array}
$$

紧接着，如果$\sigma : A' \to A''$是另一个环同态，$M''$是$A''$模，$g : M' \to M''$是$A'$同态（相对于$\sigma$）和$g' : S_{A'}(M') \to S_{A''}(M'')$ 相应的 $A'$-代数的同态，则复合$A$-代数的同态

$$
S_A(M) \xrightarrow{f'} S_{A'}(M') \xrightarrow{g'} S_{A''}(M'')
$$

对应到复合$A$-同态$g \circ f : M \to M''$（相对于$\sigma \circ \rho$）。

#### 命题 7 {#alg-iii-s6-prop-7 .statement tag=062G}

让$A, B$是两个交换环，$\rho : A \to B$环同态和$M$一个$A$模块。规范的扩张

$$
\psi : S_B(B \otimes_A M) \to B \otimes_A S_A(M)
$$

$B$-线性映射$l_B \otimes \phi_M' : B \otimes_A M \to B \otimes_A S_A(M)$是分级的$B$-代数同构。

证明是由 § 5, no. 3、命题 5 替换 $T$ 衍生自 $S$ 以及 $\phi_M$ 衍生自 $\phi_M'$。

### 5. 直极限对称代数

令$(A_\alpha, \phi_{\beta\alpha})$为交换环、$(M_\alpha, f_{\beta\alpha})$直接系统的$A_\alpha$模块、$A = \lim \rightarrow A_\alpha$和$M = \lim \rightarrow M_\alpha$的有向直接系统。对于 $\alpha \leq \beta$，我们从 $A_\alpha$ 同态 $f_{\beta\alpha}: M_\alpha \to M_\beta$ 和 $A_\alpha$ 代数同态 (no. 4, 公式 (8)) $f'_{\beta\alpha}: S_{A_\alpha}(M_\alpha) \to S_{A_\beta}(M_\beta)$ 推导出来，并从 (9) (no. 4) 得出 $(S_{A_\alpha}(M_\alpha), f'_{\beta\alpha})$是 $A_\alpha$-代数*的 *直接系统。另一方面，$f_\alpha: M_\alpha \to M$是规范的$A$同态；我们推导出 (no. 4, 公式 (8)) $A_\alpha$-代数同态

$$
f'_\alpha: S_{A_\alpha}(M) \to S_A(M)
$$

并且从(9)还可以得出，$f'_\alpha$构成$A_\alpha$同态的直接系统。

#### 命题 8 {#alg-iii-s6-prop-8 .statement tag=062H}

*$A$-同态* $f' = \lim \rightarrow f'_\alpha : \lim \rightarrow S_{A_\alpha}(M_\alpha) \to S_A(M)$ *是分级的代数同构。*

证明与 § 5, no. 5、命题 6 替换在整个 $T$ 和 $S$ 以及 $\phi$ 和 $\phi'$ 之间是相同的，并且考虑到交换代数的直极限是可交换的。

### 6. 直和对称代数。对称代数自由模。对称代数分级模

令$A$为交换环、$M = \bigoplus_{\lambda \in L} M_\lambda$直和，属于$A$模块族，以及$j_\lambda: M_\lambda \to M$典范嵌入；我们推导出代数$S(j_\lambda): S(M_\lambda) \to S(M)$的$A$同态。由于$S(M)$是可交换的，§ 4, no. 5的命题 8可以应用于同态$S(j_\lambda)$，因此存在唯一代数同态

$$
g: \bigotimes_{\lambda \in L} S(M_\lambda) \to S(M)
$$
（也用 $g_M$ 表示）使得 $S(j_\lambda) = g \circ f_\lambda$ 对于所有 $\lambda \in L$，其中

$$
f_\lambda: S(M_\lambda) \to \bigotimes_{\lambda \in L} S(M_\lambda)
$$

表示典范同态。

#### 命题 9 {#alg-iii-s6-prop-9 .statement tag=062I}

*典范同态* $g$ *(公式 (10))* *是分级的代数同构* (cf. § 4, no. 8, *注 1*)。

为了证明$g$是双射的，我们定义代数同态

$$
h: S(M) \to \bigotimes_{\lambda \in L} S(M_\lambda)
$$

这样$g \circ h$和$h \circ g$分别是$S(M)$和$\bigotimes_{\lambda \in L} S(M_\lambda)$上的恒等映射。 对于每个 $\lambda \in L$，令 $u_\lambda$ 为复合线性映射
$$
M_\lambda \xrightarrow{\phi'_M} S(M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L} S(M_\lambda).
$$
存在且仅有一个$A$-线性映射$u : M \to \bigotimes_{\lambda \in L} S(M_\lambda)$，使得$u \circ j_\lambda = u_\lambda$对于所有$\lambda \in L$。 As the $S(M_\lambda)$ are commutative, so is their tensor product (§ 4, no. 5) and hence (no. 1, Proposition 2) there exists a unique algebra homomorphism $h : S(M) \to \bigotimes_{\lambda \in L} S(M_\lambda)$ such that $h \circ \phi'_M = u$; on the other hand, it is immediate that $u(M)$ is contained in the submodule of elements of degree 1 of the graded algebra $\bigotimes_{\lambda \in L} S(M_\lambda)$ and hence $h$ is a graded algebra homomorphism. 对于$x_\lambda \in M_\lambda$，
$$
h(g(u_\lambda(x_\lambda))) = h(g(f_\lambda(\phi'_M(x_\lambda)))) = h(S(j_\lambda)(\phi'_M(x_\lambda))) = h(\phi'_M(j_\lambda(x_\lambda))) = u_\lambda(x_\lambda);
$$
因为$u_\lambda(x_\lambda)$生成代数$\bigotimes_{\lambda \in L} S(M_\lambda)$（§ 4, no. 5，命题8），$h \circ g$肯定是恒等映射。 同样，
$$
g(h(\phi'_M(j_\lambda(x_\lambda)))) = g(u_\lambda(x_\lambda)) = g(f_\lambda(\phi'_M(x_\lambda))) = S(j_\lambda)(\phi'_M(x_\lambda)) = \phi'_M(j_\lambda(x_\lambda))
$$
并且，由于元素$\phi'_M(j_\lambda(x_\lambda))$生成代数$S(M)$，$g \circ h$肯定是恒等映射。

注 (1) 令$N = \bigoplus_{\lambda \in L} N_\lambda$为$A$模块另一个系列的直和，并以$L$作为索引集合，并且对于所有$\lambda \in L$，令$v_\lambda : M_\lambda \to N_\lambda$为$A$线性映射， 从而存在$A$线性映射$v = \bigoplus_\lambda v_\lambda : M \to N$（II, § 1, no. 6，命题 6）。然后图表
$$
\begin{array}{ccc}
\bigotimes_{\lambda \in L} S(M_\lambda) & \xrightarrow{g_M} & S(M) \\
\downarrow & & \downarrow S(v) \\
\bigoplus_{\lambda \in L} S(v_\lambda) & \xrightarrow{g_N} & S(N)
\end{array}
$$
是可交换的，如下从定义（§ 4, no. 5，推论到命题 8）。

可以更精确地描述$\bigotimes_{\lambda \in L} S(M_\lambda)$的子$A$模块，通过同构$g$来识别$S^n(M)$。对于$L$的每个有限子集$J$，我们写$E_J = \bigotimes_{\lambda \in J} S(M_\lambda)$，因此$\bigotimes_{\lambda \in L} S(M_\lambda) = \varprojlim E_J$相对于$L$的有限子集的有向集合$\mathscr{F}(L)$，乘以定义（§ 4, no. 5）。对于每个家庭$\nu = (n_\lambda) \in \mathbf{N}^{(L)}$（因此有*有限*支持），使得$\sum_{\lambda \in L} n_\lambda = n$和$L$包含中的每个有限子集$J$家庭$\nu$的支持，我们写

$$
S^{J,\nu}(M) = \bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)
$$

因此，$E_J$中次数$n$的元素的子模$E_{J,n}$是$J$中包含的所有支持家庭$\nu$的$S^{J,\nu}(M)$的*直和*，并且使得$\sum_{\lambda \in L} n_\lambda = n$ （§ 4, no. 7、命题 10 和 § 4, no. 8）。按照惯例，我们为$J$中未包含赡养费的家庭$\nu$写$S^{J,\nu}(M) = \{0\}$；那么$E_{J,n}$也可以称为*所有*$S^{J,\nu}(M)$的*直和*，其中$\nu$贯穿*所有*家族$\nu = (n_\lambda)_{\lambda \in L}$的集合$H_n$，使得$\sum_{\lambda \in L} n_\lambda = n$。由于$S^0(M_\lambda)$与$A$相同，显然，对于$L$的两个有限子集$J \subset J'$和$J$中包含的$\nu$家庭的支持，典范映射$S^{J,\nu}(M) \to S^{J',\nu}(M)$（限制典范映射 $E_J \to E_J$ 到 $S^{J,\nu}(M)$) 是*双射的*。如果我们写，对于所有 $\nu \in H_n$，

$$
S^\nu(M) = \varprojlim S^{J,\nu}(M)
$$

可以看出，考虑II, § 6, no. 2、命题 5：

#### 推论{#alg-iii-s6-n6-cor-1 .statement tag=062J}

*The A-module* $S^n(M)$ *is the image under isomorphism* (10) *of the submodule of* $\bigotimes_{\lambda \in L} S(M_\lambda)$ *the direct sum of the submodules* $S^\nu(M)$ *for all the families* $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$ *such that* $\sum_{\lambda \in L} n_\lambda = n$; *if* $J$ *is the support of* $\nu$, $S^\nu(M)$ *is canonically isomorphic to* $\bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)$.

一般来说，$S^n(M)$中的$S^\nu(M)$、$\bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)$及其像都被识别。

#### 定理 1 {#alg-iii-s6-thm-1 .statement tag=062K}

*让*$A$*成为交换环并且*$M$*自由*$A$-*模和基*$(e_\lambda)_{\lambda \in L}$。 *对于映射* $\alpha : L \to \mathbf{N}$ *有限支撑，我们写*

$$
e^\alpha = \prod_{\lambda \in L} e_\lambda^{\alpha(\lambda)}
$$

（*乘积在交换代数* $S(M)$）。 *然后，当*$\alpha$*穿过*$L$*的映射*的集合*$\mathbf{N}^{(L)}$*进入*$\mathbf{N}$、*有限支撑时，*的*$e^\alpha$*形式基* $A$-*模*$S(M)$。

由于$M$是$M_\lambda = Ae_\lambda$的直和，当$L$减少为单个元素，然后应用命题9时，足以证明定理。但是当$M = Ae$（*e*一个免费的元素）时，则$x \otimes y - y \otimes x = 0$适用于$M$中的所有$x, y$；因此，理想的$\mathfrak{g}'$是零、从而、$T(Ae) = S(Ae)$和定理，然后从§ 5, no. 5、定理1得出。

基 (14) 的乘法表由下式给出

(15)
$$
e^\alpha e^\beta = e^{\alpha + \beta}
$$
其中$\alpha + \beta$是$L$到$\mathbf{N}$的映射$\lambda \mapsto \alpha(\lambda) + \beta(\lambda)$。在其他字中，$S(M)$ 的基 $(e^\alpha)$ 与乘法律 (15) 规范同构于源自 $L$ 的自由交换幺半群 $N^{(L)}$； (§ 2, no. 9) 自由模$M$与基的对称代数$S(M)$其下标集合为$L$，与多项式代数规范同构$A[(X_\lambda)_{\lambda \in L}]$、典范同构由映射$e_\lambda$到$X_\lambda$获得。特别是（§ 2, no. 7，命题 7），对于$L$的每一个映射$f : L \to E$到可交换的$A$-代数$E$，存在且仅有一个$A$-代数同态$\tilde{f} : S(M) \to E$，使得$\tilde{f}(e_\lambda) = f(\lambda)$。

注 (2)。考虑到II, § 1, no. 11、推论3到命题17，上述结果同样可以作为多项式代数和对称代数的通用性质的推论得到。

#### 推论{#alg-iii-s6-n6-cor-2 .statement tag=062L}

*如果 $M$ 是射影 $A$ 模，则 $S(M)$ 是射影 $A$ 模。*

证明与§ 5, no. 5相同，推论为定理1，替换$T$乘以$S$。

#### 命题 10 {#alg-iii-s6-prop-10 .statement tag=062M}

*令$\Delta$为可交换幺半群，$M$为型$\Delta$的分级$A$模，$(M_\alpha)_{\alpha \in \Delta}$其毕业。对于每个有序对$(\alpha, n) \in \Delta \times \mathbf{N}$，令$S^{\alpha, n}(M)$为子模$\bigotimes_{\lambda \in J} S^{n_\lambda}(M_{\alpha_\lambda})$的$S^n(M)$直和的子模，其中$(n_\lambda)_{\lambda \in L}$贯穿整数$\geq 0$的家庭的集合这样$\sum_{\lambda \in L} n_\lambda = n$，$J$是它的支持，并且对于每个$(n_\lambda), (\alpha_\lambda)_{\lambda \in J}$贯穿$\Delta^J$的家庭集合，使得$\sum_{\lambda \in J} \alpha_\lambda = \alpha$。那么 $(S^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ 是型 $\Delta \times \mathbf{N}$ 的唯一刻度，与 $S(M)$ 上的代数结构以及 $M = S^1(M)$ 上的诱导给定的刻度兼容。*

$S(M)$ 是 $S^{\alpha, n}(M)$ 的直和，这一事实由命题 9 的推论得出； 证明的其余部分与§ 5, no. 5、命题7的证明的末尾相同。

更具体地假设 $\Delta = \mathbf{Z}$ 并让 $S(M)$ 被赋予总分级 (型 $\mathbf{Z}$) (II, § 11, no. 1) 相应的到型 $\mathbf{Z} \times \mathbf{N}$ 的分级（因此也定义型 $\mathbf{Z} \times \mathbf{Z}$）上面；因此，在该分级下，次数$n \in \mathbf{Z}$的同质元素是$q + m = n$的$S^{q, m}(M)$的直和。令$f$为分级$A$-模$M$的*次数* 0的*齐次*线性映射转换为型$\mathbf{Z}$的*可交换*分级$A$-代数$F$；那么代数同态$g : S(M) \to F$使得$f = g \circ \phi_M'$是型*$\mathbf{Z}$的分级代数的*同态，如下从公式$g(x_1 x_2 \ldots x_n) = f(x_1) f(x_2) \ldots f(x_n)$对于$M$中的同质$x_i$，从$f$假设开始，以及$S(M)$型$\mathbf{Z}$毕业定义开始。

### 习题 {#alg-iii-s6-exercises}

§ 6](exercises/s6/)参见[习题。
