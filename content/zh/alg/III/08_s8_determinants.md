---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 8
section_title: Determinants
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 522-541, 637-644
pdf_pages: 0546-0565, 0661-0668
extraction: ocr
subsections:
    - "no": 1
      title: DETERMINANTS OF AN ENDOMORPHISM
      page: 522
      pdf_page: 546
    - "no": 2
      title: CHARACTERIZATION OF AUTOMORPHISMS OF A FINITE-DIMENSIONAL FREE MODULE
      page: 523
      pdf_page: 547
    - "no": 3
      title: DETERMINANT OF A SQUARE MATRIX
      page: 524
      pdf_page: 548
    - "no": 4
      title: CALCULATION OF A DETERMINANT
      page: 526
      pdf_page: 550
    - "no": 5
      title: MINORS OF A MATRIX
      page: 528
      pdf_page: 552
    - "no": 6
      title: EXPANSIONS OF A DETERMINANT
      page: 530
      pdf_page: 554
    - "no": 7
      title: APPLICATION TO LINEAR EQUATIONS
      page: 534
      pdf_page: 558
    - "no": 8
      title: CASE OF A COMMUTATIVE FIELD
      page: 536
      pdf_page: 560
    - "no": 9
      title: THE UNIMODULAR GROUP $\mathbf{SL}(n, A)$
      page: 537
      pdf_page: 561
    - "no": 10
      title: THE $\mathbf{A}[X]$-MODULE ASSOCIATED WITH AN $\mathbf{A}$-MODULE ENDOMORPHISM
      page: 538
      pdf_page: 562
    - "no": 11
      title: CHARACTERISTIC POLYNOMIAL OF AN ENDOMORPHISM
      page: 540
      pdf_page: 564
statements: 36
exercises: 26
content_sha256: 1bda74a96c64409a114be597d2e61326d982b04c5b17882ef80ae749b245f7de
translated_from: content/en/alg/III/08_s8_determinants.md
translation_method: google
source_content_sha256: a8722fe29a021a8f3f62eb7c41ed5736542a85db99ded2b20167525ac22836eb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 842c553f12f6e257c7097d87f36a00a3280802058d0b07ab161f79aaa5bdf8f8
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 8。决定因素

### 1. 自同态的决定因素

令$M$为$A$模，其有限基为$n$元素，$u$自同态为$M$。 $A$-模块$\bigwedge^n(M)$是单生的自由模，即与$A$同构的（no. 8，推论1到定理1）； $\bigwedge^n(u)$是该模的自同态，因此是唯一确定的比率$\lambda \in A$的位似$z \mapsto \lambda z$（II, § 2, no. 3，命题5）。

#### 定义 1 {#alg-iii-s8-def-1 .statement tag=0642}

*有限维的$n$的自由$A$模块$M$的自同态$u$的行列式*（II, § 7, no. 2，命题3和注1的推论），*表示为* $\det u$，*是标量$\lambda$，使得*$\bigwedge^n(u)$*是比率*$\lambda$的位似。

通过 § 7, no. 2 的公式 (4)，$\det u$ 是唯一标量，使得

(1)
$$
u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n) = (\det u) \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$
对于 $n$ 元素 $M$ 的每序列 $(x_i)_{1 \leq i \leq n}$。如果 $\det(u) = 1$，$u$ 被称为*单模*。

#### 命题 1 {#alg-iii-s8-prop-1 .statement tag=0643}

(i) *如果$u$和$v$是有限维自由$A$模$M$的两个自同态，则*

(2)
$$
\det(u \circ v) = (\det u)(\det v).
$$

(ii) $\det(1_M) = 1$； *对于每个自同构* $u$ *of* $M$, $\det u$ *可逆于* $A$ *和*

(3)
$$
\det(u^{-1}) = (\det u)^{-1}.
$$

如果 $n$ 是 $M$ 的维数，则紧随关系 $\bigwedge^n(u \circ v) = (\bigwedge^n(u)) \circ (\bigwedge^n(v))$ § 7, no. 2、公式 (3))。

设 $M$ 为自由 $A$ 模，具有有限基 $(e_i)_{1 \leq i \leq n}$；给定 $n$ 元素的序列 $(x_i)_{1 \leq i \leq n}$ $M$，这个序列 *相对于*给定的基 $(e_i)$ 的行列式，当不会引起混淆时用 $\det(x_1, x_2, \ldots, x_n)$ 表示基，是自同态 $u$ 与 $M$ 的行列式，使得 $u(e_i) = x_i$ 对应 $1 \leq i \leq n$。然后公式 (1)

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = \det(x_1, x_2, \ldots, x_n) \ e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

这个关系将$M^n$的映射$(x_i) \mapsto \det(x_1, x_2, \ldots, x_n)$表征为$A$。它表明这个映射是一个 *交错的 n 线性形式*。由于，凭借§ 7, no. 4、命题 7，交错的 $n$线性形式的$A$模与$\bigwedge^n(M)$的对偶同构，而$\bigwedge^n(M)$与$A$同构，可见*每$M^n$ 上的交错的 n 线性形式可以写成*

$$(x_1, \ldots, x_n) \mapsto \alpha \det(x_1, x_2, \ldots, x_n)$$

对于一些$\alpha \in A$。

#### 命题 2 {#alg-iii-s8-prop-2 .statement tag=0644}

*设 $M$ 为自由 $A$ 模块，其有限基 $(e_i)_{1 \leq i \leq n}$ 和 $v$ 自同态为 $M$。对于 $n$ 元素 $M$ 中的每序列 $(x_i)_{1 \leq i \leq n}$，*

$$
\det(v(x_1), \ldots, v(x_n)) = (\det v) \det(x_1, \ldots, x_n).
$$

如果 $u$ 是 $M$ 的自同态，使得 $u(e_i) = x_i$ 对于所有 $i$，则

$$
v(x_i) = (v \circ u)(e_i)
$$

因此，(5) 由(2) 得出。

### 2. 有限维自由模的自同构的刻画

#### 定理 1 {#alg-iii-s8-thm-1 .statement tag=0645}

*令$M$为有限维自由$A$模，且$u$自同态为$M$。以下条件是等效的：*
(a) $u$ 是双射；
(b) $u$ 是右可逆的（II, § 1, no. 9，推论 1 到命题 15）；
(c) $u$ 是可逆的（II, § 1, no. 9，推论 2 到命题 15）；
(d) $u$ 是满射；
(e) $\det u$ 在 $A$ 中是可逆的。

设$(e_i)_{1 \leq i \leq n}$为$M$中的基。如果 $x_i = u(e_i)$ 对应 $1 \leq i \leq n$，则

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det u) e_1 \wedge e_2 \wedge \cdots \wedge e_n.
$$

由§ 7, no. 9、定理 2 $M$的$x_i$到形式基的充要条件是，$\det u$是$A$的可逆元；这就证明了(a)和(e)的等价。观察到 (a) 显然隐含了条件 (b)、(c) 和 (d) 中的每一个；仍有待证明条件 (b)、(c) 和 (d) 中的每一个都蕴涵 (e)。现在，如果存在$M$的自同态$v$使得$v \circ u = 1_M$或$u \circ v = 1_M$，则$(\det v)(\det u) = 1$以及$\det u$在$A$中是可逆的。如果 $u$ 是满射，$\bigwedge^n(u)$ (§ 7, no. 2, 命题 3) 也是满射，在 $A$ 中 det $u$ 的其他字位似是满射，这立即意味着 det $u$ 是可逆的。

#### 命题 3 {#alg-iii-s8-prop-3 .statement tag=0646}

*令$M$为有限维自由$A$模。对于 $M$ 的每个自同态 $u$，以下条件是等效的：*
  (f) $u$ 是单射的；
  (g) det $u$ 不是 $A$ 中零的除子。

与定理 1 的证明相同的记号，对于$u$是单射的，$x_i$线性无关是充分必要的。通过§ 7, no. 9，命题 12，关系$\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$（与$\lambda \in A$）暗示$\lambda = 0$是必要且充分的。但这相当于$\lambda (\det u) = 0$，因为$e_1 \wedge \cdots \wedge e_n$是$\Lambda^n(M)$的基； 从而命题。

#### 注 {#alg-iii-s8-n2-rem-1 .statement tag=0647}

当$A$为域时，定理2的条件(e)相当于命题3的条件(g)，因为它们都意味着$\det u \neq 0$。因而，在这种情况下，定理 1 和命题 3 的所有条件都是等价的（cf. II, § 7, no. 4，命题 9 的推论）。

### 3. 平方矩阵的行列式

#### 定义 2 {#alg-iii-s8-def-2 .statement tag=0648}

*令$I$为型$(I, I)$在环$A$上的有限集合、$A$交换环和$X$平方矩阵 （II, § 10, no. 7）。 $A$模$A^I$的自同态$u$的行列式，其矩阵相对于$A^I$的典范基为$X$，称为$X$的行列式，表示为$\det X$.*

如果$X = (\xi_{ij})_{(i,j) \in I \times I}$和$(e_i)_{i \in I}$是$A^I$的典范基，则自同态$u$由下式给出
$$
u(e_i) = \sum_{j \in J} \xi_{ji} e_j.
$$

当$I = \{1, n\} \subset \mathbf{N}$时，如果我们将$i \in I$写成$x_i = u(e_i)$，那么$X$的行列式就定义在关系中
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det X) e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$
在其他字中，$\det X$等于$A^n$相对于典范基的行列式$\det(x_1, x_2, \ldots, x_n)$。因而：

#### 命题 4 {#alg-iii-s8-prop-4 .statement tag=0649}

*对于 $A^n$ 的 $n$ 向量 $x_1, \ldots, x_n$，令 $X(x_1, \ldots, x_n)$ 表示阶 $n$ 的平方矩阵，其第 $i$-第列为$x_i$ 换$1 \leq i \leq n$。然后映射*
$$
(x_1, \ldots, x_n) \mapsto \det(X(x_1, \ldots, x_n))
$$
*$(A^n)^n$到$A$的交错的和$n$是线性的。*

特别地，其中两个列相等的矩阵的行列式是零。如果对矩阵的列执行置换，则新矩阵的行列式等于旧矩阵的行列式乘以$\varepsilon_{\sigma}$。如果向矩阵中的一个列添加一个不同指标的列的标量倍数，则新矩阵的行列式等于旧的行列式。

更一般地，令$M$为有限维$n$的自由$A$模，并令$(e_i)_{i \in I}$为$M$的基；对于$M$的每个自同构$u$，如果相对于基$(e_i)$，$X$是$u$的矩阵，那么

$$
\det(u) = \det(X)
$$

从定义开始如下。

当$I = \{1, n\}$时，$X$的行列式也表示为

$$
\det(\xi_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}
$$

或者简单地 $\det(\xi_{ij})$ 如果这不会引起混乱，或者也

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} & \ldots & \xi_{1n} \\
\xi_{21} & \xi_{22} & \ldots & \xi_{2n} \\
\ldots & \ldots & \ldots & \ldots \\
\xi_{n1} & \xi_{n2} & \ldots & \xi_{nn}
\end{vmatrix}
$$

当$X = 1$时，矩阵$X$称为幺模。

#### 例 {#alg-iii-s8-n3-exa-1 .statement tag=064A}

(1)空矩阵的行列式等于1； 阶 1 的平方矩阵的行列式等于这个矩阵的唯一元素。对于阶 2 中的矩阵

$$
\begin{pmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{pmatrix}
$$

那么，在上面的记号中，

$$
x_1 \wedge x_2 = (\xi_{11} e_1 + \xi_{21} e_2) \wedge (\xi_{12} e_1 + \xi_{22} e_2) = \xi_{11} \xi_{22} e_1' \wedge e_2 + \xi_{21} \xi_{12} e_2 \wedge e_1
$$

whence

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{vmatrix} = \xi_{11} \xi_{22} - \xi_{12} \xi_{21}.
$$

我们将 nos 的一些结果翻译成矩阵的语言。 1 和 2：

#### 命题 5 {#alg-iii-s8-prop-5 .statement tag=064B}

*如果$X$和$Y$是交换环$A$上的两个方阵且具有相同的有限索引集合，则*

$$
\det(XY) = (\det X)(\det Y).
$$

要使 X 可逆，满足 X 是 A 的可逆元是充分必要的，然后

(9) $$
\det(X^{-1}) = (\det X)^{-1}.
$$

这紧接着no. 1、命题 1 和no. 2、定理 1。

#### 推论{#alg-iii-s8-n3-cor-1 .statement tag=064C}

*两个相似的方阵具有相同的行列式。*

如果 P 是可逆的平方矩阵，则 $\det(PXP^{-1}) = \det X$ 由 (8) 和 (9) 得到。

#### 命题 6 {#alg-iii-s8-prop-6 .statement tag=064D}

*为了使有限阶的平方矩阵 X 的列线性无关，条件 X 不为 A 中的零除子是充分必要的。*

这是从no. 2、命题 3 得出的。

### 4. 行列式的计算

#### 引理 1 {#alg-iii-s8-lem-1 .statement tag=064E}

*设 A 为交换环，M 自由A-模以及基 $(e_j)_{j \in J}$，其中索引集合 J 是全序的。对于每个整数 $p \leq \mathrm{Card}(J)$、每个交错的 p 线性函数 $f : M^p \to N$（其中 N 为 A-模）以及 M $(1 \leq i \leq p)$ 的 p 元素 $x_i = \sum_{j \in J} \xi_{ji} e_j$ 的每个族，

$$
f(x_1, x_2, \ldots, x_p)
= \sum_{j_1 < j_2 < \cdots < j_p} \left( \sum_{\sigma \in S_p} \varepsilon_\sigma \cdot \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(p)}, p} \right) f(e_{j_1}, \ldots, e_{j_p})
$$

*其中* $(j_k)_{1 \leq k \leq p}$ *穿过 J 的 p 元素的严格递增的序列的集合。*

现在

$$
f(x_1, \ldots, x_p) = \sum_{(j_k)} \xi_{j_1, 1} \xi_{j_2, 2} \cdots \xi_{j_p, p} f(e_{j_1}, e_{j_2}, \ldots, e_{j_p})
$$

其中 $(j_k)_{1 \leq k \leq p}$ 贯穿 J 的 p 元素的*所有* 序列；那么只需将 § 7, no. 4 的推论 1 到命题 7 应用到 f​​ 即可。

特别地，如果 J 是有限的并且有 n 元素和 $x_i = \sum_{j \in J} \xi_{ji} e_j$ $(1 \leq i \leq n)$ 是 M 的 n 元素，则

(11) $$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
= \left( \sum_{\sigma \in S_n} \varepsilon_\sigma \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n} \right) e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_n}
$$

其中$(j_k)_{1 \leq k \leq n}$是J的n个元素中唯一的序列排列在递增阶，从而

(12) $$
\det(x_1, x_2, \ldots, x_n) = \sum_{\sigma \in S} \varepsilon_\sigma \cdot \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n}.
$$

当记号为引理 1 时，比较公式 (10) 和 (12) 得出

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathscr{F}_p(J)} \det(x_{H,1}, x_{H,2}, \ldots, x_{H,p}) e_H
$$

其中$\mathscr{F}_p(J)$是$J$的子集的集合，$p$元素，对于每个子集$H \in \mathscr{F}_p(J)$，我们写出$x_{H,i} = \sum_{j \in H} \xi_{ji} e_j$和$e_H = e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_p}$，$(j_k)_{1 \leq k \leq p}$是序列 $H$的元素排列在递增阶中，应当理解，$\det(x_{H,1}, \ldots, x_{H,p})$是相对于基$(e_{jk})_{1 \leq k \leq p}$取的。

#### 命题 7 {#alg-iii-s8-prop-7 .statement tag=064F}

*令 $I$ 为交换环 $A$ 的型 (I, I) 的有限集合和 $X = (\xi_{ji})_{(j, i) \in I \times I}$ 平方矩阵。然后*

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I} \xi_{\sigma(i), i} \right)
$$

*其中$\sigma$贯穿$I$的置换的群$S_I$，$\varepsilon_\sigma$是$\sigma$*（I, § 5, no. 7）的签名。

注意可能仅限于$I = \{1, n\} \subset \mathbf{N}$的情况，然后足以应用公式（12），其中$(e_i)_{1 \leq i \leq n}$是$A^n$的典范基，$x_i$是$X$的列（cf.no. 3， 公式 (6))。

特别是，对于阶 3 的矩阵行列式

$$
X = \begin{pmatrix}
\xi_{11} & \xi_{12} & \xi_{13} \\
\xi_{21} & \xi_{22} & \xi_{23} \\
\xi_{31} & \xi_{32} & \xi_{33}
\end{pmatrix}
$$

我们有

$$
\det(X) = \xi_{11} \xi_{22} \xi_{33} + \xi_{12} \xi_{23} \xi_{31} + \xi_{21} \xi_{32} \xi_{13} - \xi_{13} \xi_{22} \xi_{31} - \xi_{12} \xi_{21} \xi_{33} - \xi_{11} \xi_{23} \xi_{32}.
$$

#### 命题 8 {#alg-iii-s8-prop-8 .statement tag=064G}

*对于超过交换环的每个平方矩阵 $X$，转置矩阵 ${}^t X$的行列式等于$X$的行列式。*

假设$X$等于型(I, I)。对于置换 $\sigma, \tau$ $S_I$ 的每个有序对，（因为乘法是可交换的）

$$
\prod_{i \in I} \xi_{\sigma(i), i} = \prod_{j \in I} \xi_{\sigma(\tau(j)), \tau(j)}.
$$

特别是取$\tau = \sigma^{-1}$；利用 $\varepsilon_{\sigma^{-1}} = \varepsilon_\sigma$ 的事实，可以看出

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I, i} \xi_{i, \sigma(i)} \right),
$$

这就证明了命题。

#### 推论 1 {#alg-iii-s8-prop-8-cor-1 .statement tag=064H}

对于$\mathbf{A}^n$的n向量$x_1, \ldots, x_n$，令$Y(x_1, \ldots, x_n)$表示第i行为$x_i$的阶n的平方矩阵，对于$1 \leq i \leq n$。然后映射
$$
(x_1, \ldots, x_n) \mapsto \det(Y(x_1, \ldots, x_n))
$$
从 $(\mathbf{A}^n)^n$ 到 $\mathbf{A}$ 是交错的并且是 n 线性的。

#### 推论 2 {#alg-iii-s8-prop-8-cor-2 .statement tag=064I}

对于平方矩阵 $X$ 的有限阶超过交换环 $\mathbf{A}$，以下条件是等效的：
(i) $X$ 的行是线性无关的；
(ii) $X$ 的列是线性无关的；
(iii) $\det X$ 不是$\mathbf{A}$ 中零的除子。

这紧接着上面的no. 3、命题 6 和命题 8。

#### 推论 3 {#alg-iii-s8-prop-8-cor-3 .statement tag=064J}

设 $u$ 为有限维自由 $\mathbf{A}$-模 $M$ 的自同态和对偶 $M^*$ (II, § 2, no. 5, 定义 5) 的 $^t u$ 转置自同态；然后
$$
\det(^t u) = \det(u).
$$
如果$X$相对于$M$的基是$u$的矩阵，则$^t X$相对于对偶基是$^t u$的矩阵（II, § 10, no. 4，命题） 3）；如$\det(u) = \det(X)$和$\det(^t u) = \det(^t X)$，由命题8得出结论。

### 5. 矩阵的未成年人

令$X$为型(I, J)的矩形矩阵$(\xi_{ij})_{(i,j) \in I \times J}$，其索引集合I和J是全序的。如果$H \subset I$和$K \subset J$是有限子集且数$p$相同元素，则存在唯一的递增双射$\phi : H \to K$（集合理论，III, § 5, no. 3， 命题6);我们用型 (H, H) 中的$X_{H,K}$ 平方矩阵表示等于$(\xi_{i,\phi(j)})_{(i,j) \in H \times H}$。若$X$ 属于的元素到交换环$\mathbf{A}$，则行列式$\det(X_{H,K})$称为指标H、K的矩阵$X$的小数；这些行列式（对于 I 和 J 的子集的所有有序对 (H, K) 分别与 $p$ 元素）也称为阶 $p$ 的 $X$ 次要因素。有了这个记号：

#### 命题 9 {#alg-iii-s8-prop-9 .statement tag=064K}

令$M$为基$(e_i)_{i \in J}$（有限或其他）的$\mathbf{A}$模，其索引集合$J$是全序的。对于每个整数 $p > 0$，令 $(e_H)_{H \in \mathfrak{S}_p(J)}$ 为 $\wedge^p(M)$ (§ 7, no. 8) 的相应的基。设$(x_i)_{1 \leq i \leq p}$为$p$的序列，$M$的元素；让
$$
x_i = \sum_{j \in J} \xi_{ji} e_j \quad \text{for } i \in I = \{1, p\}
$$

令$X$表示型$(J, I)$中的矩阵$(\xi_{ji})$。然后

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathfrak{F}_p(J)} (\det X_{H,I}) e_H.
$$

其中$H$穿过$J$的子集的集合$\mathfrak{F}_p(J)$和$p$元素。

这紧随no. 4的公式(12)和no. 3的公式(6)。

#### 命题 10 {#alg-iii-s8-prop-10 .statement tag=064L}

令$M$和$N$分别为$u$的维数、$m$和$n$、$u : M \to N$、线性映射和$X$矩阵的两个自由$A$模块，其中尊重$M$的基$(e_i)_{1 \leq i \leq m}$和$N$的基$(f_j)_{1 \leq j \leq n}$。然后，对于每个整数$p \leq \inf(m, n)$，$\wedge^p(u)$的矩阵相对于$\wedge^p(M)$的基$(e_K)_{K \in \mathfrak{F}_p(I)}$和$\wedge^p(N)$的基$(f_H)_{H \in \mathfrak{F}_p(J)}$（我们写成$I = \{1, m\}$和$J = \{1, n\}$）是型$(\mathfrak{F}_p(J), \mathfrak{F}_p(I))$的矩阵$(\det(X_{H,K}))$（因此有$\binom{n}{p}$行和$\binom{m}{p}$列）。

对于子集$K \subset J$和$p$元素，设$(j_k)_{1 \leq k \leq p}$为递增阶排列的$K$元素序列； $\wedge^p(u)$ 定义、§ 7, no. 2、公式 (4)

$$
\wedge^p(u)(e_K) = u(e_{j_1}) \wedge u(e_{j_2}) \wedge \cdots \wedge u(e_{j_p}).
$$

因此指标$H$行中的$\wedge^p(u)$的矩阵元素和指标$K$的列是元素$u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p})$的指标$H$的分量；因此它等于$\det(X_{H,K})$乘命题9。

矩阵$(\det(X_{H,K}))$称为矩阵$X$的第$p$外部幂，记为$\wedge^p(X)$。当$p = m = n$、$\wedge^n(X)$为矩阵时，单个元素$\det(X)$。

#### 命题 11 {#alg-iii-s8-prop-11 .statement tag=064M}

设$M$为有限维$n$的自由$A$模块；对于$M$中的每自同态$u$和$A$中元素$\xi, \eta$中的每有序对，

$$
\det(\xi 1_M + \eta u) = \sum_{k \geq 0} \operatorname{Tr}(\wedge^k(u)) \xi^{n-k} \eta^k.
$$

令$(e_i)_{1 \leq i \leq n}$为$M$的基，并令$I = \{1, n\}$；到计算 (18) 的左侧，我们必须形式乘积

$$
(\xi e_1 + \eta u(e_1)) \wedge (\xi e_2 + \eta u(e_2)) \wedge \cdots \wedge (\xi e_n + \eta u(e_n))
$$

等于项 $\xi^{n-p} \eta^p z_K$ 的和，其中

$$
z_K = x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

其中$x_i = u(e_i)$代表$i \in K$，$x_i = e_i$代表$i \in H = I - K$，其中整数$p$穿过区间$[0, n]$，并且对于每个$p$，$K$穿过I的子集的集合， $p$元素。如果$i_1 < i_2 < \cdots < i_{n-p}$（或$j_1 < j_2 < \cdots < j_p$）是H（或K）的元素排列在递增阶，我们可以写（$§ 7$，no. 8，推论1到定理1和公式（19））

$$
z_K = \rho_{H, K} e_{i_1} \wedge e_{i_2} \wedge \cdots \wedge e_{i_{n-p}} \wedge u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}).
$$

但如果 $X$ 是 $u$ 的矩阵相对于基 $(e_i)$，则命题 10

$$
u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}) = \sum_{L \in \mathfrak{F}_p(I)} (\det X_{L, K}) e_L
$$

因此

$$
z_K = \rho_{H, K} \sum_{L \in \mathfrak{F}_p(I)} (\det X_{L, K}) e_H \wedge e_L.
$$

Now $H \cap L \neq \varnothing$ except for $L = K$; it therefore follows from $§ 7$, no. 8, formula (20) that $z_K = (\det X_{K, K}) e_1 \wedge e_2 \wedge \cdots \wedge e_n$ and formula (18) then follows from Proposition 10 and the definition of the trace of a matrix (II, $§ 10$, no. 11, formulae (49) and (50)).

#### 推论{#alg-iii-s8-n5-cor-1 .statement tag=064N}

*在与命题 11 相同的假设下，对于 A-模 $\bigwedge(M)$ 的自同态 $\bigwedge(u)$*

$$(19)$$
$$
\operatorname{Tr}(\bigwedge(u)) = \det(1_M + u).
$$

在(18)中，替换$\xi$和$\eta$乘以1就足够了，并且观察到$\bigwedge(u)$的矩阵相对于$e_H$($H \in \mathfrak{F}(I)$)的基是矩阵的对角矩阵 $\bigwedge^k(u)$ 对应 $\geq k$ 0（II、$§ 10$、no. 7、*例* IV）。

### 6.行列式的展开

令 I 为全序有限索引集合。对于 I 的每个子集 H，令 H' 表示补集 I - H。令 $X = (\xi_{ij})$ 为型 (I, I) 的平方矩阵，可以将其视为自同态的矩阵 $M = A^I$ 的$u$ M 的典范基 $(e_i)_{i \in I}$。令 $n = \operatorname{Card}(I)$ 且令 H 为 I 与 $q \leq n$ 元素的子集以及 I 与 $n - q$ 元素的 K 子集；那么我们可以写(no. 5,命题10)

$$
(\bigwedge^q(u))(e_H) = \sum_R \det(X_{R, H}) e_R
$$
$$
(\bigwedge^{n-q}(u))(e_K) = \sum_S \det(X_{S, K}) e_S
$$

其中 R（分别为 S）穿过 I 的子集的集合，其中 $q$（分别为 $n - q$）元素。由 $§ 7$, no. 8, 公式 (19) 和 (20) 得出

$$
e_R \wedge e_S = 0
$$

$S = R'$、从而公式时除外

$$
(20) \quad (\wedge^q(u)(e_H)) \wedge (\wedge^{n-q}(u)(e_K)) = \sum_R \rho_{R, R'} \det(X_{R, H}) \det(X_{R', K}) e_I
$$

其中$R$穿过$I$的子集的集合$\mathscr{F}_q(I)$和$q$元素。

如果我们取$K = H'$，则从$\wedge^n(u)$（§ 7, no. 2，公式（4））和§ 7, no. 3的定义得出，推论1到命题5，（20）的右侧是$\rho_{H, H'} \wedge^n(u)(e_I)$。因此 (no. 1, 公式 (1) 和 § 7, no. 2, 公式 (4))

$$
(21) \quad \det(X) = \rho_{H, H'} \sum_{R \in \mathscr{F}_q; R' \neq R} \rho_{R, R'} \det(X_{R, H}) \det(X_{R', H'}).
$$

另一方面，如果$K \neq H'$，则$H \cap K \neq \varnothing$；因为(20)的左边是$\pm \wedge^n(u)(e_H \wedge e_K)$，所以它是零，从而

$$
(22) \quad \sum_R \rho_{R, R'} \det(X_{R, H}) \det(X_{R', K}) = 0 \quad \text{for } K \neq H'.
$$

(21) 的右侧称为矩阵 $X$ 行列式的*拉普拉斯展开* *由q 列（其指标属于到H）和n - q 列（其指标） 属于到 H* 的补码 H'。次要的 $\det(X_{R, H})$ 和 $\det(X_{R', H'})$ 是有时称为*互补*。

拉普拉斯展开的一个重要简单情况是，其中$I = \{1, n\}$和$q = 1$，因此$H = \{i\}$；对于$I$中的每一个子集$R = \{j\}$，其中一个元素然后是$\det X_{R, H} = \xi_{ji}$。 $\det X_{R', H'}$的小数是平方矩阵的行列式，从矩阵规范导出（no. 5），通过在$X$中抑制指标$j$和列的行获得指标$i$。我们用$X^{ji}$表示这个平方矩阵。显然$\rho_{H, H'} = (-1)^{i-1}$和$\rho_{R, R'} = (-1)^{j-1}$；因此（21）在这种情况下变成

$$
(23) \quad \det X = \sum_{j=1}^n (-1)^{i+j} \xi_{ji} \det(X^{ji})
$$

我们从 (22) 中得到类似的结果

$$
(24) \quad \sum_{j=1}^n (-1)^{ji} \xi_{ji} \det(X^{jk}) = 0 \quad \text{for } k \neq i.
$$

公式 (23) 被称为指标 i* 的列的 X 行列式的 *展开。标量$(-1)^{i+j} \det(X^{ji})$被称为指标、$j$和$i$的*辅因子*（或者，滥用语言，$\xi^{ji}$的辅因子）在$X$中。

$X$的辅因子**矩阵是矩阵

$$
(25) \quad Y = ((-1)^{i+j} \det(X^{ji}))
$$

其中第$j$行的元素和第$i$第列是指标$j$和$i$的辅因子。 公式 (23) 和 (24) 等价于公式

$$(26)$$
$$
{}^tY . X = (\det X) I_n.
$$

所以：

#### 命题 12 {#alg-iii-s8-prop-12 .statement tag=064O}

*对于型 $(n, n)$ 的每个可逆平方矩阵 $X$，$X$ 的逆由公式给出*

$$(27)$$
$$
X^{-1} = (\det X)^{-1} {}^t Y
$$

*其中$Y$是$X$的辅因子矩阵。*

通过考虑$X$的*转置*并使用no. 5的命题 8，可以相对于两个互补的集合行，特别是$\det X$的展开，获得拉普拉斯展开，因此有公式等价于

$$(28)$$
$$
X . {}^t Y = (\det X) I_n,
$$

在上面的记号中。

容易验证，如果$X$是维数$n$的自由$\mathbf{A}$-模块$M$的自同态$u$相对于基$(e_i)_{1 \leq i \leq n}$的矩阵，则${}^t Y$是矩阵 / 自同态 $\tilde{u}$ / $M$ 由以下条件定义：对于$n$ 元素 $x, y_2, \ldots, y_n$ / $M$的每个集合，

$$
\tilde{u}(x) \wedge y_2 \wedge \cdots \wedge y_n = x \wedge u(y_2) \wedge \cdots \wedge u(y_n).
$$

$\tilde{u}$ 称为$u$ 的*共转置*（cf. § 11, no. 11，命题 13 的推论）。

#### 例 {#alg-iii-s8-n6-exa-1 .statement tag=064P}

(1) *Vandermonde 行列式。* 给定 $\mathbf{A}$ 的 $n$ 元素的序列 $(\zeta_i)_{1 \leq i \leq n}$，则该序列的 *Vandermonde 行列式* 是行列式

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \ldots & 1 \\
\zeta_1 & \zeta_2 & \ldots & \zeta_n \\
\zeta_1^2 & \zeta_2^2 & \ldots & \zeta_n^2 \\
\vdots & \vdots & \ddots & \vdots \\
\zeta_1^{n-1} & \zeta_2^{n-1} & \ldots & \zeta_n^{n-1}
\end{vmatrix}
$$

我们将证明

$$(29)$$
$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \prod_{i < j} (\zeta_j - \zeta_i).
$$

由于命题对于$n = 1$来说是直接的，因此我们通过归纳对$n$进行论证。

对于每个指标$k \geq 2$，我们从指标$k$的行中减去指标$k - 1$的行乘以$\zeta_1$；行列式的值不变，因此

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \cdots & 1 \\
0 & \zeta_2 - \zeta_1 & \cdots & \zeta_n - \zeta_1 \\
0 & \zeta_2(\zeta_2 - \zeta_1) & \cdots & \zeta_n(\zeta_n - \zeta_1) \\
\cdots & \cdots & \cdots & \cdots \\
0 & \zeta_2^{n-2}(\zeta_2 - \zeta_1) & \cdots & \zeta_n^{n-2}(\zeta_n - \zeta_1)
\end{vmatrix}
$$

从而，通过第一个列展开，然后从指标$k - 1$的列中取出因子$\zeta_k - \zeta_1$，这样得到的次要（$2 \leq k \leq n$）

$$
V(\zeta_1, \ldots, \zeta_n) = (\zeta_2 - \zeta_1)(\zeta_3 - \zeta_1) \cdots (\zeta_n - \zeta_1) V(\zeta_2, \ldots, \zeta_n)
$$

由归纳成立 (29)。

(2) 考虑阶$n$的平方矩阵，它在“矩阵的上三角矩阵”的形式中呈现（II, § 10, no. 7，例 IV）

$$
X = \begin{pmatrix} Y & T \\ 0 & Z \end{pmatrix}
$$

我们表明

$$
\det X = (\det Y)(\det Z).
$$

设$n$为矩阵$X$的阶，$h$为$Y$，$(e_i)_{1 \leq i \leq n}$典范基为$\mathbf{A}^n$，$x_i$($1 \leq i \leq n$)列 $X$； 假设意味着 $\mathbf{A}^n$ 的列 $x_1, \ldots, x_h$ 属于到子模与基 $e_1, \ldots, e_h$，然后定义 (no. 3, 公式 (6))

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h.
$$

另一方面，对于每个指标$i > h$，我们可以写成$x_i = y_i + z_i$，其中$y_i$是$e_1, e_2, \ldots, e_h$的线性组合，$z_i$是$e_{h+1}, \ldots, e_n$的线性组合。通过 (30)，$x_1 \wedge x_2 \wedge \cdots \wedge x_n \wedge y_i = 0$ 对于所有 $i > h$，因此

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h \wedge z_{h+1} \wedge \cdots \wedge z_n.
$$

但到定义

$$
z_{h+1} \wedge z_{h+2} \wedge \cdots \wedge z_n = (\det Z)e_{h+1} \wedge e_{h+2} \wedge \cdots \wedge e_n
$$

从而公式 (30)。

根据$p$上的归纳，如果$X$是矩阵的上三角形矩阵的形式：

$$
X = \begin{pmatrix}
X_{11} & X_{12} & \cdots & X_{1p} \\
0 & X_{22} & \cdots & X_{2p} \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & X_{pp}
\end{pmatrix}
$$

(31) $$
\det X = (\det X_{11})(\det X_{22}) \ldots (\det X_{pp}).
$$

这尤其适用于三角形矩阵（其中所有 $X_{ii}$ 均为阶 1），更具体地适用于对角矩阵：

(32) $$
\det(\operatorname{diag}(\alpha_1, \alpha_2, \ldots, \alpha_n)) = \alpha_1 \alpha_2 \ldots \alpha_n.
$$

(3) 设$M, M'$为维数$n, n'$、$M$的$u$自同态和$M'$的$u'$自同态的两个自由$A$模块。然后

(33) $$
\det(u \otimes u') = (\det u)^{n'} (\det u')^n.
$$

因为我们可以写 $u \otimes u' = (u \otimes 1_{M'}) \circ (1_M \otimes u')$ ，然后导致两个自同态 $u, u'$ 之一是恒等式的情况。对于例，如果$u' = 1_{M'}$和$X$相对于$M$的基$(e_i)$是$u$的矩阵，则$u \otimes 1_{M'}$的矩阵相对于张量积 $M'$的$(e_i)$和基可以写成矩阵（有$n'$行和$n'$列）矩阵有$n$行和$n$列

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

从而，凭借*例 2*，

$$
\det(u \otimes 1_{M'}) = (\det X)^{n'} = (\det u)^{n'}
$$

这立即给出公式 (33)。

### 7. 线性方程的应用

考虑在 (*可交换*) 环 $A$ (II, § 2, no. 8) 上的 $n$ 未知数中的系统或 $n$ 标量线性方程：

(34) $$
\sum_{j=1}^n \lambda_{ij} x_j = \eta_i \quad (1 \leq i \leq n).
$$

令$L$为平方矩阵$(\lambda_{ij})$/阶$n$；像往常一样将矩阵与$\xi_i$（分别是$\eta_i$）中的一个列由……组成与$\mathbf{A}^n$中的元素$x = (\xi_i)$（分别是$\mathbf{A}^n$中的元素$y = (\eta_i)$）进行识别， 系统 (34) 也可以写成 (II, § 10, no. 3, 命题 2)

(35)
$$
L.x = y.
$$

令$u$为$\mathbf{A}^n$的自同态$x \mapsto L.x$，$L$相对于典范基为矩阵；说方程（35）对于所有$y \in \mathbf{A}^n$（至少）有一个解意味着$u$是满射的； 定理 1 of no. 2 那么意味着以下命题：

#### 命题 13 {#alg-iii-s8-prop-13 .statement tag=064Q}

*对于$n$关于交换环的未知数中的系统或$n$线性方程，无论其右侧如何，都至少承认一个解，矩阵或系统的行列式是可逆的是必要且充分的；在这种情况下，系统承认单个解。*

若$\mathbf{A}$中$\det L$不是零的除子，则式(34)等价于式
$$
(\det L)L.x = (\det L)y.
$$
如果$M$是$L$的辅因子矩阵，我们可以从no. 6关系的(34)和公式(26)导出
(36)
$$
(\det L)x = {}^tM.y
$$
也可以写成
(37)
$$
(\det L)\xi_i = \sum_{j=1}^n (-1)^{i+j}(\det L^{ij})\eta_j = \det L_i \quad (1 \leq i \leq n)
$$
其中，$L_i$表示矩阵由指标$i$的$L$与$y$的替换列获得。 公式 (37) 被称为 *Cramer 的公式* 对于系统 (34)； (34) 的每个解也是 (37) 的解。相反，我们从 (36) 推导出来，考虑到 no. 6 的公式 (28)，
(38)
$$
(\det L)(L.x - y) = 0
$$
因此，如果$\det L$不是$\mathbf{A}$中零的除子，系统 (34) 和 (37) *等价*；如果 $\det L$ 可逆，则 (34) 的唯一解由下式给出
(39)
$$
\xi_i = (\det L)^{-1}(\det L_i) \quad (1 \leq i \leq n).
$$
系统 (34) 使得 $\det L$ 可逆，也称为 *Cramer 系统*。

特别是令 $y = 0$；然后从 no. 2 的命题 3 得出：

#### 命题 14 {#alg-iii-s8-prop-14 .statement tag=064R}

*对于$n$未知数超过交换环的齐次线性系统的$n$方程要承认非零解，其矩阵的行列式是零的除子是必要且充分的。*

### 8. 交换域的情况

当环$\mathbf{A}$为交换域时，以上均适用；但有一些简化和额外的结果。

因此，在这种情况下，命题 12 of § 7, no. 9 可以表述如下：

#### 命题 15 {#alg-iii-s8-prop-15 .statement tag=064S}

令 $\mathbf{E}$ 大于交换域的向量空间；对于 $p$ 向量 $x_i \in \mathbf{E}$ ($1 \leq i \leq p$) 线性无关，$x_1 \wedge x_2 \wedge \cdots \wedge x_p \neq 0$ 是充分必要的。

#### 推论{#alg-iii-s8-n8-cor-1 .statement tag=064T}

设$X$为型$(m, n)$除交换域的矩阵。 $X$的秩等于最大的整数$p$，使得阶$p$的$X$中至少存在一个小数，即$\neq 0$。

$X$的秩是$X$的线性无关列的最大值数（II, § 10, no. 12，定义7）。然后从 no. 5 的命题 15 和公式 (17) 得出推论。

现在考虑交换域 $\mathbf{K}$ 上 $n$ 未知数中 $m$ 线性方程的系统的情况：

$$
\sum_{j=1}^n \lambda_{ij} \xi_j = \eta_i \quad (1 \leq i \leq m).
$$

(41)

#### 命题 16 {#alg-iii-s8-prop-16 .statement tag=064U}

令 $L = (\lambda_{ij})$ 为系统 (41) 中的矩阵（型 $(m, n)$）。令$M$为型$(m, n+1)$中的矩阵，在$L$上加上第$(n+1)$个列$(\eta_i)$(II, § 10, no. 1)。令 $p$ 为 $L$ 的秩（由应用命题 15 的推论计算）。假设$L$的次要$\Delta$（通过抑制$L$中指标$\geq p + 1$的行和列的行列式矩阵）是$\neq 0$（这总是可以通过在行上合适的置换来实现） $L$ 以及 $L$ 的列上合适的置换）。那么，要使系统 (41) 至少有一个解，$M$ 阶 $p + 1$ 的所有次数，阶 $p + 1$ $M$ 的子矩阵的行列式是充分必要的，其列有指标$1, 2, \ldots, p$和$n+1$，为零。如果是这样，系统(41)中的解就是前$p$方程中的系统由……组成；如果它们被写成

$$
\sum_{j=1}^p \lambda_{ij} \xi_j = \eta_i - \sum_{k=p+1}^n \lambda_{ik} \xi_k \quad (1 \leq i \leq p)
$$

这个系统的所有解都是通过取指标$k > p$任意值和应用Cramer的公式（no. 7，公式（37））的$\xi_k$得到计算$\xi_j$指标$j \leq p$。

我们知道（II, § 10, no. 12，命题 12），系统（41）至少有一个解，矩阵$L$和$M$有相同的秩是充分必要的。将 $L$ 的行和列排列为叙述的满足条件，令 $a_i$ ($1 \leq i \leq p$) 表示 $L$ 的第一个 $p$ 列，并且$y = (\eta_i)$$M$的第$(n+1)$-第列；因为$L$的所有列都由$a_i$的假设线性组合，所以说$M$与$L$有相同的秩$p$意味着$y$是$a_i$的线性组合，或者也可以是（命题15）$a_1 \wedge \cdots \wedge a_p \wedge y = 0$。 叙述中的可能性条件是后者关系的翻译，考虑到no. 5的公式(17)。此外，由于$M$的前$p$行是线性无关的，指标$> p$的行是其中的线性组合，因此(42)的每个解也是(41)的解。 最后一个断言那么直接的推论命题 13 no. 7。

### 9.幺模群$\mathbf{SL}(n, A)$

让$\mathbf{M}_n(A)$表示$A$上的阶$n$的方阵的环。考虑映射$\det : \mathbf{M}_n(A) \to A$。 $\mathbf{M}_n(A)$的可逆元群$\mathbf{GL}(n, A)$（与$A$-模块$A^n$的自同构群同构（II, § 10, no. 7））在这个映射下就是逆像 $A$可逆元乘法群$A^*$（no. 3、命题5）。 注另一方面，映射 $\det : \mathbf{GL}(n, A) \to A^*$ 是群同态（no. 3，命题 5）。

此外，映射$\det : \mathbf{M}_n(A) \to A$是*满射*（因此同态$\det : \mathbf{GL}(n, A) \to A^*$也是）；因为，对于所有 $\lambda \in A$，

$$
\det(\operatorname{diag}(\lambda, 1, \ldots, 1)) = \lambda
$$

凭借no. 6的公式(32)。

满同态 $\det : \mathbf{GL}(n, A) \to A^*$的*核*是$\mathbf{GL}(n, A)$的正规子群，由*单模* 矩阵组成；它用$\mathbf{SL}_n(A)$或$\mathbf{SL}(n, A)$表示，通常称为幺模群*或方阵的*群*或阶$n$在$A$上的特殊线性群*。

在这个没有。我们将检查 $A$ 是 *域* 的情况。回想一下，对于$1 \leq i \leq n, 1 \leq j \leq n$，$E_{ij}$表示阶$n$中的平方矩阵，除了指标$i$行中的那个之外，所有元素都是零并且列指标 $j$，等于 1；其中 $I_n$ 表示阶 $n$ 的单位矩阵，我们为 *不同* 指标 $i, j$ 的每个有序对以及所有 $\lambda \in A$ 写 $B_{ij}(\lambda) = I_n + \lambda E_{ij}$ （II, § 10, no. 13）。

#### 命题 17 {#alg-iii-s8-prop-17 .statement tag=064V}

*令$K$为交换域。 幺模群 $\mathbf{SL}(n, K)$ 由矩阵 $B_{ij}(\lambda)$ 与 $i \neq j$ 和 $\lambda \in K$ 生成。*

由II, § 10, no. 13、命题 14，我们知道$\mathbf{GL}(n, K)$中的每一个矩阵都是形式$B_{ij}(\lambda)$的矩阵乘积和形式的矩阵 $\operatorname{diag}(1, 1, \ldots, 1, \alpha)$ 与 $\alpha \in K^*$。现在$\det(B_{ij}(\lambda)) = 1$和$\det(\operatorname{diag}(1, \ldots, 1, \alpha)) = \alpha$是直接的（no. 6，*例2*）； 从而命题。

#### 推论 {#alg-iii-s8-n9-cor-1 .statement tag=064W}

*群*$\mathbf{SL}(n, K)$*是*$\mathbf{GL}(n, K)$的换位子群，*除了*$n = 2$*和其中*$K$*与2个元素*是域*的情况。

因为$\mathbf{SL}(n, K)$是$\mathbf{GL}(n, K)$的同态的核到群$K^*$、$\mathbf{SL}(n, K)$包含换位子群$\Gamma$$\mathbf{GL}(n, K)$ （I, § 6, no. 2）。 为了证明 $\mathbf{SL}(n, K) = \Gamma$，只需在命题 17 处证​​明，对于所有 $\lambda \in K^*$、$B_{ij}(\lambda)$ 属于到 $\Gamma$。 现在，自$B_{ij}(\lambda) = Q . B_{ij}(1) . Q^{-1}$起，$B_{ij}(\lambda)$是$\mathbf{GL}(n, K)$中的$B_{ij}(1)$共轭，其中$Q$相对于$K^n$的自同构$v$典范基$(e_i)$表示矩阵这样$v(e_i) = \lambda e_i, v(e_k) = e_k$ 对应 $k \neq i$。 另一方面，令$u_{ij}$（对于$i \neq j$）是$K^n$的自同构，使得$u_{ij}(e_i) = -e_j, \ u_{ij}(e_j) = e_i, \ u_{ij}(e_k) = e_k$对于$k \notin \{i, j\}$，其中属于到$\mathbf{SL}(n, K)$；那么$B_{ji}(\lambda) = U_{ij} B_{ij}(-\lambda) U_{ij}^{-1}$，其中$U_{ij}$是$u_{ij}$相对于典范基的矩阵。 类似地，如果$1 < i < j$，则$B_{1j}(\lambda) = U_{1i} B_{ij}(\lambda) U_{1i}^{-1}$，最后，对于$2 < j$，$B_{12}(\lambda) = U_{2j} B_{1j}(\lambda) U_{2j}^{-1}$。 这证明了$\mathbf{GL}(n, K)/\Gamma$中所有$B_{ij}(\lambda)$具有相同的像$s$，并且还需要证明$s$是单位元素。

首先假设$K$包含元素$\lambda$不同于0和1；那么$1 = \lambda + (1 - \lambda)$，右边的两个项就是$\neq 0$； 关系 $B_{12}(1) = B_{12}(\lambda) B_{12}(1 - \lambda)$ 显示$s^2 = s$，因此$s$ 为单位元素。

现在假设$n \geq 3$。 乘积 $B_{21}(1) B_{31}(1)$ 是自同构 $u$ $K^n$ 的矩阵，使得$u(e_1) = e_1 + e_2 + e_3, u(e_i) = e_i$ $i \neq 1$。如果$S$是自同构$u'$或$K^n$的矩阵，使得$u'(e_2) = e_2 + e_3, u'(e_i) = e_i$对应$i \neq 2$，则$S . B_{21}(1) B_{31}(1) . S^{-1} = B_{21}(1)$；我们还推导出$s^2 = s$，从而完成证明。

#### 注 {#alg-iii-s8-n9-rem-1 .statement tag=064X}

(1) $\mathbf{GL}(2, \mathbf{F}_2) = \mathbf{SL}(2, \mathbf{F}_2)$；这是阶 6 的可解群，其换位子群为指标 2 (II, § 10, 习题 14)。

(2) 同上记号，可如I, § 5, no. 7，命题 9 证明，对于$i < j, j - i > 1$，$u_{ij} = u_{j-1, j} u_i, _{j-1} u_{j-1, j}^{-1}$；因此*群*$\mathbf{SL}(n, K)$*由矩阵*$B_{12}(\lambda)$*和*$U_{i, i+1}$*为*$1 \leq i \leq n - 1$生成。

### 10. 与 $\mathbf{A}$-模块自同态关联的 $\mathbf{A}[X]$-模块

令$M$为$\mathbf{A}$模，$u$自同态为$M$。考虑多项式环 $\mathbf{A}[X]$ 在 $\mathbf{A}$ 上的一个不定$X$ 中。对于每个多项式 $p \in \mathbf{A}[X]$ 和所有 $x \in M$，我们写

$$
p . x = p(u)(x).
$$

作为$\mathbf{A}[X]$的两个多项式$p, q$的$(pq)(u) = p(y) \circ q(u)$，$\mathbf{A}[X]$-模结构因此定义在$M$上； 集合$M$，有了这个结构，就用$M_u$表示； $M$给出的$\mathbf{A}$模块结构是通过将$M_u$的运算符的环限制为$\mathbf{A}$而获得的。 注 $M_u$ 的子模只是 $M$ 的子模，在 $u$ 下*稳定*。

由于$A[X] \times M$到$M$的映射$(p, x) \mapsto p.x$是$A$双线性，因此定义典型地是$A$线性映射$\phi : A[X] \otimes_A M \to M$，使得
$$
\phi(p \otimes x) = p.x = p(u)(x).
$$
另一方面，$A[X] \otimes_A M$ 具有规范的 $A[X]$ 模块结构 (II, § 5, no. 1)；我们用$M[X]$来表示这个$A[X]$模块； 映射 $\phi : M[X] \to M_u$ 是 $A[X]$ 线性，因为对于 $A[X]$ 和 $x \in M$ 中的 $p, q$，
$$
\phi(q(p \otimes x)) = \phi((qp) \otimes x) = (qp).x = q(u)(p(u)(x)) = q.\phi(p \otimes x).
$$
此外，$u$是$M_u$的$A[X]$自同态，对于
$$
u(p.x) = u(p(u)(x)) = (up(x))(x) = p.u(x).
$$
最后，$M[X]$的$A[X]$自同态$\bar{u}$通过写作(II, § 5, no. 1)来定义
$$
\bar{u}(p \otimes x) = p \otimes u(x).
$$
此外，从公式 (44) 和 (45) 可以得出，$A[X]$-线性映射 $u, \bar{u}$ 和 $\phi$ 通过关系相关
$$
\phi \circ \bar{u} = u \circ \phi.
$$
让$\psi$表示$M[X]$的$A[X]$自同态$X - \bar{u}$，因此$\psi(p \otimes x) = (Xp) \otimes x - p \otimes u(x)$。我们有以下命题：

#### 命题 18 {#alg-iii-s8-prop-18 .statement tag=064Y}

*序列 / $A[X]$-同态*
$$
M[X] \xrightarrow{\psi} M[X] \xrightarrow{\phi} M_u \longrightarrow 0
$$
是准确的。

由于 $\phi(1 \otimes x) = x$ 对于所有 $x \in M$，显然 $\phi$ 是满射的；另一方面，
$$
\phi(X(p \otimes x)) = X.\phi(p \otimes x) = u(\phi(p \otimes x)),
$$
其他字，$\phi \circ X = u \circ \phi = \phi \circ \bar{u}$由(46)；这证明了$\phi \circ \psi = 0$。仍有待验证$\operatorname{Ker} \phi \subset \operatorname{Im} \psi$。对于这个注，由于$A$模$A[X]$的单项式$X^k$ ($k \geq 0$)形式基，每个元素$z \in M[X]$都可以唯一地写成形式 $z = \sum_k X^k \otimes x_k$，其中$(x_k)$是元素、$M$、有限支撑的家庭。如果$z \in \operatorname{Ker} \phi$，那么$\phi(z) = \sum_k u^k(x_k) = 0$，我们可以写
$$
z = \sum_k (X^k \otimes x_k - 1 \otimes u^k(x_k)) = \sum_k (X^k - \bar{u}^k)(1 \otimes x_k).
$$
但由于$M[X]$的$A[X]$自同态$X$和$\bar{u}$是可置换的，那么

$$
X^k - \bar{u}^k = (X - \bar{u}) \circ \left( \sum_{j=0}^{k-1} X^j \bar{u}^{k-j-1} \right)
$$

这证明存在一个$y \in M[X]$使得$z = \psi(y)$。

现在让$M'$为另一个$A$模，$u'$自同态为$M'$；设$M'_{u'}$、$\phi'$、$\bar{u}'$、$\psi'$为从$M'$和$u'$获得的模和映射，即获得$M_u$、$\phi$、$\bar{u}$、$\psi$从 $M$ 到 $u$。然后：

#### 命题 19 {#alg-iii-s8-prop-19 .statement tag=064Z}

*对于 M 到 M' 的映射 g 是 M_u 到 M'_u 的 A[X]-同态，g 是 M 到 M' 的 A-同态使得 $g \circ u = u' \circ g$ 是必要且充分的。在这种情况下，如果 $\bar{g}$ 是 M[X] 到 M'[X] 的 A[X] 同态，等于 $1_{A[x]} \otimes g$ (II, § 5, no. 1)，则图表*

$$
\begin{array}{cccccc}
M[X] & \xrightarrow{\psi} & M[X] & \xrightarrow{\phi} & M_u & \longrightarrow 0 \\
\downarrow \bar{g} & & \downarrow \bar{g} & & \downarrow g & \\
M'[X] & \xrightarrow{\psi'} & M'[X] & \xrightarrow{\phi'} & M'_{u'} & \longrightarrow 0
\end{array}
$$

是*可交换的*。

条件 $g \circ u = u' \circ g$ 显然是 (43) 所必需的，因为 $g$ 是 A[X]-同态；这就足够了，因为归纳意味着对于每个整数$n > 0$都有$g \circ u^n = {u'}^n \circ g$。另一方面，对于所有$x \in M$和所有$p \in A[X]$，

$$
\phi'(\bar{g}(p \otimes x)) = \phi'(p \otimes g(x)) = p(u')(g(x)) = g(p(u)(x)) = g(\phi(p \otimes x))
$$
和
$$
\bar{u}'(g(p \otimes x)) = \bar{u}'(p \otimes g(x)) = p \otimes u'(g(x)) = p \otimes g(u(x)) = \bar{g}(\bar{u}(p \otimes x))
$$
这就证明了图表 (48) 的交换律。

### 11. AN 自同态的特征多项式

令$M$为维数$n$和$u$自同态的自由$A$模块$M$。考虑两个不定式$A[X, Y]$和$A[X, Y]$模$M[X, Y] = A[X, Y] \otimes_A M$中的多项式环；令 $\bar{u}$ 为 $A[X, Y]$ 模块 $M[X, Y]$ 的自同态，该模块规范地源自 $u$ (II, § 5, no. 1)。由 no. 5, 命题 11 得出

$$
\det(X - Y \bar{u}) = \sum_{j=0}^n (-1)^j \mathrm{Tr}(\wedge^j(u)) X^{n-j} Y^j
$$

因为如果相对于$M$的基$(e_i)_{1 \leq i \leq n}$，$U$是$u$的矩阵，相对于$M[X, Y]$的基$(1 \otimes e_i)_{1 \leq i \leq n}$，$U$是$\bar{u}$的矩阵，因此

$$
\mathrm{Tr}(\wedge^j(\bar{u})) = \mathrm{Tr}(\wedge^j(u)).
$$

#### 定义 3 {#alg-iii-s8-def-3 .statement tag=0650}

令 $M$ 为有限维自由 $A$ 模，且为 $M$ 的 $u$ 自同态。自由$A[X]$模$M[X]$的自同态$X - \bar{u}$的行列式称为$u$的特征多项式，记为$\chi_u(X)$。

如果 $M$ 为秩 $n$，则由 (49) 得出

$$
\chi_u(X) = \sum_{j=0}^n (-1)^j \operatorname{Tr}(\wedge^j(u)) X^{n-j}
$$

对于 $\det(X - Y \bar{u}) = \det(X . I_n + Y U)$ 和 $\det(X - \bar{u}) = \det(X . I_n - U)$。由此可见，$\chi_u(X)$是次数$n$的一元多项式，其中$X^{n-1}$的系数为$-\operatorname{Tr}(u)$，常数项为$(-1)^n \det(u)$。

#### 命题 20（“凯利-汉密尔顿定理”）{#alg-iii-s8-prop-20 .statement tag=0651}

对于有限维自由 $A$ 模块的每个自同态 $u$，$\chi_u(u) = 0$。

在命题 18 的记号（$§ 3$、no. 10）中，对于所有$x \in M$，$\chi_u(u)(x)$ 是$\chi_u(X) \otimes x$ 的$\phi$ 下的像。但如果 $v$ 是 $M[X]$ 的自同态，$X - \bar{u}$ (no. 6) 的转置，那么

$$
\chi_u(X) \otimes x = \chi_u(X)(1 \otimes x) = (X - \bar{u})(v(1 \otimes x))
$$

结论由命题18 of no. 10得出。

### 习题{#alg-iii-s8-exercises}

§ 8](exercises/s8/)参见[习题。
