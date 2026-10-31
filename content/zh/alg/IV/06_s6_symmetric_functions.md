---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 6
section_title: Symmetric functions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.98-A IV.105
pdf_pages: 0070-0095, 0107-0114
extraction: ocr
subsections:
    - "no": 1
      title: Symmetric polynomials
      page: 61
      pdf_page: 70
    - "no": 2
      title: Symmetric rational fractions
      page: 67
      pdf_page: 76
    - "no": 3
      title: Symmetric formal power series
      page: 67
      pdf_page: 76
    - "no": 4
      title: Sums of powers
      page: 70
      pdf_page: 79
    - "no": 5
      title: Symmetric functions in the roots of a polynomial
      page: 72
      pdf_page: 81
    - "no": 6
      title: The resultant
      page: 75
      pdf_page: 84
    - "no": 7
      title: The discriminant
      page: 81
      pdf_page: 90
statements: 43
exercises: 15
errata:
    - says: then $w$ is an automorphism of the $A$-module $S_q \times S_p$
      read: then $\omega$ is an automorphism of the $A$-module $S_q \times S_p$
      why: The map is introduced as omega in the same sentence — "if we write omega(u, v) = (u, uh + v) ... then w is an automorphism" — and the display that follows on page 86 gives its inverse as omega^{-1}(u, v). The French of 2007 (A IV.71) sets omega throughout.
    - says: The matrix of $w$ with respect to the basis $B_1$
      read: The matrix of $\omega$ with respect to the basis $B_1$
      why: Same automorphism as the display above it, which page 86 sets round.
    - says: $\varphi \circ w$ maps $(u, v)$ to $u(f + gh) + vg$
      read: $\varphi \circ \omega$ maps $(u, v)$ to $u(f + gh) + vg$
      why: Same automorphism, composed with phi. Page 86 sets phi round and the omega beside it roman.
    - says: representing $\varphi$ and $\varphi \circ w$ have the same determinant and this follows from the relation $\det w = 1$
      read: representing $\varphi$ and $\varphi \circ \omega$ have the same determinant and this follows from the relation $\det \omega = 1$
      why: The last two occurrences of the same automorphism on page 86, both roman.
content_sha256: 6d6320b2f60939fe575c69230ee3f3d7a37162e46491bd5a2cf3e93ce3fbe918
translated_from: content/en/alg/IV/06_s6_symmetric_functions.md
translation_method: google
source_content_sha256: b6c3b59be706d899df8c14677f2a1f585996a74c952028c811d04e381a1ed6be
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 2230651e800e9e5a857fb4eb554b5446d54dcb9d4cf8d210d9a89176335b6290
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 6。对称函数

### 1. 对称多项式

设$n$为正整数。对于每个置换$\sigma \in \mathfrak{S}_n$，令$\varphi_\sigma$为A-代数$A[X_1, \ldots, X_n]$中的自同构，其中映射$X_i$到$X_{\sigma(i)}$为$1 \leq i \leq n$。显然，$\sigma \mapsto \varphi_\sigma$是$\mathfrak{S}_n$的同态变成$A[X_1, \ldots, X_n]$的自同构的群。我们将$\sigma f = \varphi_\sigma(f)$代替$\sigma \in \mathfrak{S}_n$和$f \in A[X_1, \ldots, X_n]$。如果 $\sigma f = f$ 对于所有 $\sigma \in \mathfrak{S}_n$ ，则称多项式 f 是对称的；对称多项式形式单位分级子代数 $A[X_1, \ldots, X_n]$ ；我们将在本段的其余部分用$A[X_1, \ldots, X_n]^{\mathrm{sym}}$表示它。
对于每个正整数 k，我们用集合 $\{1, 2, \ldots, n\}$ 的 k 元素子集的 $\mathfrak{P}_k$ 集合表示，并把

(1)
$$
s_k = \sum_{H \in \mathfrak{P}_k} \prod_{i \in H} X_i .
$$

当我们希望指定整数 n 时，我们应该写 $s_{k,n}$ 而不是 $s_k$。我们特别有

$$
\begin{aligned}
s_0 &= 1 \\
s_1 &= \sum_{1 \leq i \leq n} X_i \\
s_2 &= \sum_{1 \leq i < j \leq n} X_i X_j \\
&\ \ \cdots \cdots \cdots \cdots \cdots \\
s_n &= X_1 \ldots X_n
\end{aligned}
$$

$s_k = 0$ 对应 $k > n$。显然$s_k$是次数 k 的齐次对称多项式；我们将其称为次数 k 的初等对称多项式。
在环$A[X_1, \ldots, X_n, U, V]$我们有关系

(2)
$$
\prod_{i=1}^{n} (U + V X_i) = \sum_{k=0}^{n} U^{n-k} V^k s_k ;
$$

通过适当的代换我们推导出关系

(3)
$$
\prod_{i=1}^{n} (1 + T X_i) = \sum_{k=0}^{n} s_k T^k ,
$$

(4)
$$
\prod_{i=1}^{n} (\mathbf{X} - \mathbf{X}_i) = \sum_{k=0}^{n} (-1)^{n-k} s_{n-k} \mathbf{X}^k .
$$

#### 定理 1 {#alg-iv-s6-thm-1 .statement tag=06EE}

— 让我们输入 $E = A[\mathbf{X}_1, \ldots, \mathbf{X}_n]$ 和 $S = A[\mathbf{X}_1, \ldots, \mathbf{X}_n]^{\text{sym}}$。

a) 对称多项式的$A$-代数$S$由$s_1, \ldots, s_n$生成。

b) $E$ 的元素 $s_1, \ldots, s_n$ 在$A$ (IV, p. 4) 上是代数独立的。

c) 单项式$X^\nu = X_1^{\nu(1)} \ldots X_n^{\nu(n)}$族，使得$1 \leq i \leq n$的$0 \leq \nu(i) < i$是$S$模$E$的基。特别是，$E$是秩$n!$的免费$S$模块。

我们将在$n$上用归纳证明定理，$n = 0$的情况是微不足道的。让我们写出$B = A[X_n]$并用$s_k'$表示次数$k$在$X_1, \ldots, X_{n-1}$中的初等对称多项式；因此我们有$B[X_1, \ldots, X_{n-1}] = A[X_1, \ldots, X_n]$。如果我们在 Th 的叙述替换 $n$ $n-1$ 和 $A$ $B$。 1、我们可以将归纳假设表述如下：

(A) $X_1, \ldots, X_{n-1}$的所有置换下多项式$f \in A[\mathbf{X}_1, \ldots, \mathbf{X}_n]$不变量$B$-代数$S'$由$s_1', \ldots, s_{n-1}'$生成。

(B) $E$ 中的元素 $s_1', \ldots, s_{n-1}'$ 在代数上独立于$B$。

(C) 单项式$X_1^{\nu(1)} \ldots X_{n-1}^{\nu(n-1)}$族，使得$1 \leq i \leq n-1$的$0 \leq \nu(i) < i$是$S'$模$E$的基。

我们有明显的关系

(5)
$$
s_k = s_k' + s_{k-1}' X_n \quad (1 \leq k \leq n-1),
$$
从中我们可以在 $k$ 获得归纳

(6)
$$
s_k' = (-1)^k X_n^k + \sum_{i=1}^k (-1)^{k-i} s_i X_n^{k-i} \quad (1 \leq k \leq n-1).
$$

我们有 $S \subset S'$，因此 $s_1, \ldots, s_n$ 属于到 $S'$；通过 (A) 和公式 (6)，B 代数 $S'$ 因此由 $s_1, \ldots, s_{n-1}'$ 生成。

由 (B) 存在 B 代数 $S'$ 的自同态 $\mu$ 使得

(7)
$$
u(s_k') = (-1)^k X_n^k + \sum_{i=1}^k (-1)^{k-i} s_i' X_n^{k-i} \quad (1 \leq k \leq n-1).
$$

到式(5)，通过简单的计算我们就得到$u(s_k) = u(s_k') + u(s_{k-1}') X_n$，从而$u(s_k) = s_k'$。令 $P \in B[Y_1, \ldots, Y_{n-1}]$；然后从$P(s_1, \ldots, s_{n-1}) = 0$我们推导出
$$
0 = u(P(s_1, \ldots, s_{n-1})) = P(s_1', \ldots, s_{n-1}'),
$$
从而$P = 0$（B）。由此可见，B 代数 $S'$ 由代数独立的元素 $s_1, \ldots, s_{n-1}$ 生成。该性质可以重新表述如下：
(D) $A$-代数$S'$由代数独立的元素$s_1, \ldots, s_{n-1}, X_n$生成。

因此，我们可以用多项式环$C[X_n]$来计算认同S'，其中$C$是由$s_1, ..., s_{n-1}$生成的E的子A代数。

为了证明 a)，令 $f \in S$ 为次数 $m$ 的齐次对称多项式。我们有$f \in S' = C[X_n]$，所以存在C的元素$g = P(s_1, ..., s_{n-1})$，$X_1, ..., X_n$中的次数$m$齐次，使得$f - g$能被$X_n$整除。由于$f - g$是对称的，它的每个项也可以被$X_1, ..., X_{n-1}$整除，因此$f - g$可以被$s_n = X_1 ... X_n$整除。在其他字中，存在$h \in S$使得$f = g + hs_n$，从而$\deg h < m$。 $m$ 归纳 $f$ 属于到

$$
C[s_n]_E = A[s_1, ..., s_{n-1}, s_n]_E .
$$

因此我们已经证明A-代数 S是由$s_1, ..., s_n$生成的。

接下来我们证明b)。如果我们用$X$代替(4)中的$X$，我们发现

$$
(-1)^{n+1}s_n = X_n^n + \sum_{k=1}^{n-1} (-1)^{n-k} s_{n-k} X_n^k ;
$$

在其他字中，$(-1)^{n+1}s_n$是$X$中的次数$n$的一元多项式，系数为$C$。通过 IV，p. 11，我们有以下性质：
(E) $C[T]$ 到 $C[X_n] = S'$ 的 C 代数同态 $\varphi$，其中映射 T 到 $s_n$ 是单射，并且 $S'$ 是自由模超过 $\varphi$ 的像，其中基 $(1, X_n, ..., X_n^{n-1})$。

$C$ 的元素 $s_1, ..., s_{n-1}$ 在代数上独立于 A，由 (D) 得到；因此$\varphi$的单射性意味着$s_1, ..., s_{n-1}, s_n$在代数上独立于A，从而 b)。

为了证明 c)，$\varphi$ 的像等于 $C[s_n]_E = S$，因此根据 (E)，$S'$ 是基 $(1, X_1, ..., X_n^{n-1})$ 上 S 上的自由模。现在断言 c) 源自归纳假设 (C) 和 II 的第 25 条，p. 222。这样就完成了证明。

令 $f$ 为 $X_1, ..., X_n$ 的对称多项式，次数 $m$ 齐次。由 Th. 1 (IV, p. 62) 存在多项式$Q \in A[Y_1, ..., Y_n]$使得$f = Q(s_1, ..., s_n)$。前面的证明提供了一种显式计算$Q$的方法，通过双归纳对$n$和$m$进行显式计算。正如我们所看到的，存在一个多项式 $P \in A[Y_1, ..., Y_{n-1}]$ 和一个在 $X_1, ..., X_n$ 中对称的多项式 h，其齐次于次数 $m-n$，使得

$$
f = P(s_1, ..., s_{n-1}) + s_n h .
$$

对于每个多项式 $u \in A[X_1, ..., X_n]$ 我们将

$$
u'(X_1, ..., X_{n-1}) = u(X_1, ..., X_{n-1}, 0)
$$

那么$s'_1, ..., s'_{n-1}$是$X_1, ..., X_{n-1}$和公式中的初等对称多项式 (8) 蕴含

$$
f' = P(s'_1, ..., s'_{n-1})
$$

因此，$P$的确定被简化为$n - 1$不定式中的对称多项式的计算，并且$h$由(8)获得。

我们用两个例来说明方法。

**例。 — 1)** 让 $n = 3$ 和

$$
f = X_1^2(X_2 + X_3) + X_2^2(X_3 + X_1) + X_3^2(X_1 + X_2).
$$

我们有

$$
f' = X_1^2X_2 + X_1X_2^2 = X_1X_2(X_1 + X_2) = s'_1s'_2.
$$

让我们写$g = f - s_1s_2$；我们有

$$
g = f - (X_1 + X_2 + X_3)(X_1X_2 + X_1X_3 + X_2X_3) = -3X_1X_2X_3,
$$

因此终于

$$
f = s_1s_2 - 3s_3.
$$

2）再次让$n = 3$并放入$p = X_1^3 + X_2^3 + X_3^3$。
我们有$p(X_1, 0, 0) = X_1^3 = s_1(X_1, 0, 0)^3$。写$q = p - s_1^3$，我们得到

$$
q = -3f - 6X_1X_2X_3 = -3s_1s_2 + 3s_3
$$

最后

$$
p = s_1^3 - 3s_1s_2 + 3s_3.
$$

令 $S_1, ..., S_n$ 不确定。我们将为多项式代数$A[S_1, ..., S_n]$配备型$N$的刻度，其中$S_k$为权$k$为$1 \leq k \leq n$（IV，p. 3），并为$A[X_1, ..., X_n]$配备通常的刻度。对于 $1 \leq k \leq n$，$X_1, ..., X_n$ 中的初等对称多项式 $s_{k,n}$ 是齐次的次数 $k$。由 Th. 1 (IV, p. 62) 映射 $g \mapsto g(s_{1,n}, ..., s_{n,n})$ 因此是分级代数的同构

$$
\varphi_n : A[S_1, ..., S_n] \to A[X_1, ..., X_n]^{\text{sym}}
$$

令$m$为整数，使得$0 \leq m \leq n$。对于每个整数 $k$ 使得 $1 \leq k \leq m$ 我们有

$$
s_{k,m}(X_1, ..., X_m) = s_{k,n}(X_1, ..., X_m, 0, ..., 0)
$$

通过 $s_k$ 的定义 (IV, p. 61, 公式 (1))。因此图表

$$
\begin{array}{ccc}
A[S_1, ..., S_m] & \xrightarrow{j} & A[S_1, ..., S_n] \\
\varphi_m \downarrow & & \varphi_n \downarrow \\
A[X_1, ..., X_m]^{\text{sym}} & \xleftarrow{p} & A[X_1, ..., X_n]^{\text{sym}}
\end{array}
$$

（其中 j 表示规范包含，$p$ 同态
$$
g \mapsto g (X_1, \ldots, X_m, 0, \ldots, 0)
$$
是可交换的。

#### 命题 1 {#alg-iv-s6-prop-1 .statement tag=06EF}

*对于正整数 k, n 的每个对，令 $S_k^{(n)}$ 为 $X_1, \ldots, X_n$ 中所有对称多项式的 A-模由……组成，这些对称多项式是次数 k 的齐次。如果整数 m 满足$0 \leq k \leq m \leq n$，则映射 $f \mapsto f (X_1, \ldots, X_m, 0, \ldots, 0)$ 是$S_k^{(n)}$ 的同构到$S_k^{(m)}$。

通过图表 (10) 的交换律足以证明$S_1, \ldots, S_n$ 中权 k 的每个等量多项式仅取决于假设 $0 \leq k \leq m \leq n$ 下的$S_1, \ldots, S_m$。现在单项式 $S_1^{\alpha(1)} \cdots S_n^{\alpha(n)}$ 的权等于整数 $\alpha(1) + 2\alpha(2) + \ldots + n\alpha(n)$；由于整数 $\alpha(1), \ldots, \alpha(n)$ 为正，关系
$$
\alpha(1) + 2\alpha(2) + \cdots + n\alpha(n) = k \leq n
$$
意味着$\alpha(j) = 0$代表$k < j \leq n$，从而断言。

#### 例 3 {#alg-iv-s6-n1-exa-3 .statement tag=06EG}

根据 IV 的例 2、p. 64 和上面的命题 1，我们有
$$
\sum_{i=1}^n X_i^3 = s_{1,n}^3 - 3s_{1,n}s_{2,n} + 3s_{3,n}
$$
对于每个整数 $n \geq 3$。 图表 (10) 交换律另外给出公式
$$
X_1^3 + X_2^3 = s_{1,2}^3 - 3s_{1,2}s_{2,2},
$$
$$
X_1^3 = s_{1,1}^3.
$$

#### 注 {#alg-iv-s6-n1-rem-1 .statement tag=06EH}

— 令 n 和 k 为两个正整数。 我们用$N^n$中长度 k 元素的$\Delta_{k,n}$集合表示，并进一步装备$A$，，与序关系，写成$a \leq \beta$，由$N^n$上的词典阶诱导（*集合理论*，III，p. 157），以及$\sigma \in \mathfrak{S}_n, a \in N^n$和$l \leq i \leq n$在$N^n$上的群$\mathfrak{S}_n$的定义作用通过$(\sigma a)(i) = a(\sigma^{-1}(i))$。 此外，我们用元素$a = (\alpha(1), \ldots, \alpha(k))$或$\mathbf{N}^k$的$D_k$集合表示，这样
$$
\alpha(1) \geq \alpha(2) \geq \cdots \geq \alpha(k), \quad \alpha(1) + \cdots + \alpha(k) = k.
$$

假设$k \leq n$，让我们认同$\mathbf{N}^k$，其中子集为$N^n$乘以映射$(a(1), \ldots, a(k)) \mapsto (a(1), \ldots, a(k), 0, \ldots, 0)$。那么 $D_k$ 由元素 $a$ 和 $\Delta_{k,n}$ 组成，使得 $\sigma a \leq a$ 代表所有 $\sigma \in \mathfrak{S}_n$。由此可见，$A$、包含、唯一元素、$D_k$中的群$\mathfrak{S}_n$中的每个轨道。对于每个$a \in D_k$，令$O(a)$为$\mathfrak{S}_n$的运算下的$\Delta_{k,n}$中$a$的轨道；把
$$
M(\alpha) = \sum_{\beta \in O(\alpha)} X^\beta.
$$

从 IV 的引理 1、p. 47 可知，$(\mathbf{M}(\alpha))_{\alpha \in D_k}$ 是A-模 $S_k^{(n)}$ 中的基。

每 $\alpha \in D_k$ 投入

$$
(12)\quad S(\alpha) = \prod_{i=1}^k s_i^{\alpha(i) - \alpha(i+1)} \quad \text{(where it is understood that } a\ (k+1) = 0 \text{)} ;
$$

因为我们有 $\sum_{i=1}^k i \cdot (a(i) - a(i+1)) = \sum_{i=1}^k a(i) = k$，所以对称多项式 $S(\alpha)$ 是齐次的次数 $k$。它直接来自 Th。 1（IV，p. 62）家庭$(S(\alpha))_{\alpha \in D_k}$是A-模$S_k^{(n)}$中的基。

令$\alpha, \beta$位于$D_k$中，并令$c_{\alpha\beta}$为在$A = \mathbf{Z}$和$k = n$情况下由(12)定义的多项式$S(\alpha)$中的单项式$X^\beta$的系数。这就是正整数，*独立于环 A 和整数 n*。到公式 (9) (IV, p. 64) 我们有

$$
(13)\quad S(\alpha) = \sum_{\beta \in D_k} c_{\alpha\beta} \cdot \mathbf{M}(\beta) \quad (\alpha \in D_k) .
$$

可以证明(cf. IV, p. 101, 习题 13) 矩阵 $C = (c_{\alpha\beta})_{\alpha,\beta \in D_k}$使得$c_{\alpha\alpha} = 1$和$c_{\alpha\beta} = 0$对于$\alpha < \beta$；将 II p. 351 中引入的术语推广，我们可以说 $C$ 属于到下总三角形群。 矩阵 D 与 C 互逆也是如此。 当 $2 \leq k \leq 5$ 时，矩阵 C 和 D 的值在表 (IV, p. 103-105) 中给出。

现在假设$n < k$，让我们认同$N^n$，其中子集为$N^k$乘以映射$(a(1), \ldots, a(n)) \mapsto (a(1), \ldots, a(n), 0, \ldots, 0)$。对于$D_k \cap N^n$中的每个$a$，我们再次用$\Delta_{k,n}$中的$a$的$O(\alpha)$轨道在$\mathfrak{S}_n$的运算和定义$\mathbf{M}(\alpha)$下用（11）表示。进一步，我们通过（12）计算定义$S(\alpha)$，则$(\mathbf{M}(a))_{a \in D_k \cap N^n}$和$(S(a))_{a \in D_k \cap N^n}$族是A-模$S_k^{(n)}$的基。通过 IV 的公式 (9)，p. 64，我们有公式，类似于 (13)，其中 $D_k$ 被 $D_k \cap N^n$ 替代，具有相同的整数 $c_{\alpha\beta}$。

#### 例 4 {#alg-iv-s6-n1-exa-4 .statement tag=06EI}

到 IV 的例 3，p. 65，我们有

$$
\mathbf{M}(3,0,0) = S(3,0,0) - 3S(2,1,0) + 3S(1,1,1)
$$

对于每个整数 $n \geq 3$，依此类推

$$
\mathbf{M}(3,0) = S(3,0) - 3S(2,1)
$$

对于$n = 2$。

### 2.对称有理分式

令$K$为交换域且$X_1, X_2, \ldots, X_n$不确定。对于每个$\sigma \in S_n$，我们在$K[X_1, X_2, \ldots, X_n]$的No. 1（IV，p. 61）自同构$\varphi_\sigma$中定义。这个自同构有一个独特的扩张$\psi_\sigma$到域$K(X_1, \ldots, X_n)$，$\sigma \mapsto \psi_\sigma$是$S_n$的单同态变成$K(X_1, \ldots, X_n)$的自同构群。对于每个$f \in K(X_1, \ldots, X_n)$，我们有$(\psi_\sigma f)(X_1, \ldots, X_n) = f(X_{\sigma(1)}, \ldots, X_{\sigma(n)})$。 有理分式 $f$，使得所有$\sigma \in S_n$的$\psi_\sigma(f) = f$称为对称有理分式。 $X_1, \ldots, X_n$中所有对称有理分式的集合是$K(X_1, \ldots, X_n)$的子域。

#### 命题 2 {#alg-iv-s6-prop-2 .statement tag=06EJ}

— *$X_1, \ldots, X_n$中的对称有理分式的域是$X_1, \ldots, X_n$中的对称多项式环分数域。*。

令$f \in K(X_1, \ldots, X_n)$为对称有理分数，并令$u_1, v_1$为$K[X_1, \ldots, X_n]$的两个元素，使得$f = \frac{u_1}{v_1}$。我们放入$v = \prod_{\sigma \in S_n} \psi_\sigma(v_1) \in K[X_1, \ldots, X_n]$和$u = fv \in K[X_1, \ldots, X_n]$；那么$v$是对称的，因此$u$是对称的，因为$f$是对称的，而$f = \frac{u}{v}$，从而的结果。

#### 推论{#alg-iv-s6-n2-cor-1 .statement tag=06EK}

— *令 $s_1, s_2, \ldots, s_n$ 为 $X_1, \ldots, X_n$ 中的初等对称多项式。对于每个有理分式 $g \in K(S_1, S_2, \ldots, S_n)$ 序列 $(s_1, s_2, \ldots, s_n)$ 都可代入 $g$ 且映射 $g \mapsto g(s_1, s_2, \ldots, s_n)$ 是 $K(S_1, S_2, \ldots, S_n)$ 的同构到对称有理分式的域 $X_1, \ldots, X_n$.*

这是从 Prop. 2 和 Th. 得出的。 IV 中的 1，p. 62。

### 3.对称形式幂级数

设$I$为集合，$X = (X_i)_{i \in I}$为不定族，$A[[X]]$代数为$X_i$中的正式幂级数。对于每个置换$a \in S_I$，存在一个唯一的代数$A[[X]]$连续自同构$\varphi_a$，其中映射$X_i$到$X_{a(i)}$对于每个$i \in I$（IV，p. 28，命题4）；显然，$\sigma \mapsto \varphi_\sigma$是$S_I$的同态变成代数$A[[X]]$的连续自同构的群。设$f \in A[[X]]$为正式的幂级数；我们放入$af = \varphi_a(f)$，我们可以说，如果每个$\sigma \in S_I$都有$\sigma f = f$，则正式的幂级数$f$是对称的。对称形式幂级数形式 $A[[X]]$ 的闭子代数，用 $A[[X]]^{\text{sym}}$ 表示，并配有由 $A[[X]]$ 诱导的拓扑。

设 T 为不定式。在形式幂级数$A[[X, T]]$的环中，族$(X_i T)_{i \in I}$是可求和的，因此族$(1 + X_i T)_{i \in I}$是可乘的（IV，p. 27，命题2）；此外我们还有

$$
\prod_{i \in I} (1 + X_i T) = 1 + \sum_{k \geq 1} s_k T^k,
$$

其中正式的幂级数 $s_k \in A[[X]]$ 定义为

$$
s_k = \sum_{H \in \mathscr{P}_k} \left( \prod_{i \in H} X_i \right) \quad (k \geq 1)
$$

（我们用 I 的所有 k 元素子集的 $\mathscr{P}_k$ 集合表示）。特别是我们有$s_1 = \sum_{i \in I} X_i$。当 I 为 $n$ 元素时，我们有 $s_k = 0$ 对应 $k > n$；更准确地说，当$I = \{1, \ldots, n\}$时，形式的幂级数$s_k$只不过是$X_1, \ldots, X_n$中次数k的初等对称多项式。

设 $S = (S_k)_{k \geq 1}$ 为不定数的序列。由于正式的幂级数$s_k$为阶$\geq k$，以及属于到$A[[X]]^{\text{sym}}$，条件a）和b）IV的Prop.4，p. 28满足$E = A[[X]]^{\text{sym}}$；因此存在唯一的连续 A-代数同态

$$
\varphi_I : A[[S]] \to A[[X]]^{\text{sym}}
$$

这样每个整数$k \geq 1$就有$\varphi_I(S_k) = s_k$。

#### 定理 2 {#alg-iv-s6-thm-2 .statement tag=06EL}

**a)** *如果 I 是 n 元素的有限集合，则 $\varphi_I$ 诱导 $A[[S_1, \ldots, S_n]]$ 的双连续同构到 $A[[X]]^{\text{sym}}$*。

*b)* *如果 I 是无限的，$\varphi_I$ 是 $A[[S]]$ 到 $A[[X]]^{\text{sym}}$* 的双连续同构。

在情况a）中，我们放置$B = A[[S_1, \ldots, S_n]]$，并用由$A[[S]]$引起的拓扑装备这个代数；我们还用 $\varphi_I$ 的 $\psi_I$ 限制表示 B。在情况 b) 中，我们放置 $B = A[[S]]$ 和 $\psi_I = \varphi_I$。我们将为多项式代数$A[S]$配备型N的分度，其中$S_k$对于每个整数$k \geq 1$来说是权k。

#### 引理 1 {#alg-iv-s6-lem-1 .statement tag=06EM}

**设 J 为 I 的有限子集，r 整数，使得 Card $J \geq r$ 和 fa 对称形式幂级数，其与 $X_i$ ($i \in I$) 中的次数 r 齐次。令$\bar{f}$为形式的幂级数，通过用0替换$X_i$中$I - J$中的每个i而获得。如果$\bar{f} = 0$，那么我们就有$f = 0$。**

让我们输入$f = \sum_{|\alpha| = r} a_\alpha X^\alpha$（其中$|\alpha|$是多索引$a = (\alpha_i)_{i \in I}$的长度$\sum_{i \in I} \alpha_i$）。如果$a$是长度$r$的多重索引，$J'$是$a$的支持（$i \in I$的集合使得$\alpha_i \neq 0$），则卡$J' \leq r$，因此存在置换 $\sigma \in S_I$使得$\sigma(J') \subset J$。将$\beta_i = \alpha_{\sigma^{-1}(i)}$代入$i \in I$，则单项式$X^\beta = \prod_{i \in I} X_{\sigma(i)}^{\alpha_i}$仅取决于不定式$X_j$ ($j \in J$)、从而$a_\beta = 0$乘以假设$\overline{f} = 0$。由于$f$是对称的，所以我们有$a_\alpha = a_\beta$，并且由于$\alpha$是任意的，所以我们有结论即$f = 0$。

#### 引理 2 {#alg-iv-s6-lem-2 .statement tag=06EN}

*令$f$为$X_i (i \in I)$中次数$r$的对称形式幂级数。存在唯一的多项式 $P \in B \cap A[S]$，等压于权 $r$，使得 $f = \psi_1(P)$。*

$I$ 有限的情况由 Th 得出。 1（IV，p. 62）。

假设$I$是无限的，并且$I$中的选择有限子集$J$、包含$r$元素。我们保留引理 1 中的记号；我们注，$S_n \ (n \geq 1)$中权$r$的每个等量多项式仅依赖于$S_1, \ldots, S_r$，而$\overline{s}_1, \ldots, \overline{s}_r$是$r$不定式$X_j \ (j \in J)$中的初等对称多项式。如果$P$是$S_n$和$h = f - \psi_1(P)$中权$r$的等量多项式，则$\overline{h} = \overline{f} - P(\overline{s}_1, \ldots, S_r)$和引理1表明关系$f = \psi_1(P)$等于$\overline{f} = P(\overline{s}_1, \ldots, \overline{s}_r)$。由 Th. 1 (IV, p. 62) 存在唯一的多项式 $P \in A[S]$，等压于权 $r$，结果为 $\overline{f} = P(\overline{s}_1, \ldots, \overline{s}_r)$，从而。

#### 引理 3 {#alg-iv-s6-lem-3 .statement tag=06EO}

*对于每个整数$m \geq 0$，令$c_m$为阶$\geq m$的所有对称形式幂级数的代数$A[[X]]^{sym}$由……组成的理想。 序列$(c_m)_{m \geq 0}$是$A[[X]]^{sym}$中$0$的邻域的基本系统。*

当 $I$ 有限时，引理显然成立，因此让我们假设 $I$ 是无限的。对于每个$I$有限子集$J$、$m$元素由……组成，用长度$N^{(1)}$元素$\tilde{J}$集合表示$< m$ 以及$J$ 的支持。进一步用幂级数包含的$a_J'$集合表示，没有项$aX^\alpha$与$a \in \tilde{J}$。由于$\tilde{J}$是$N^{(1)}$的有限子集，并且$N^{(1)}$的每个有限子集都包含在形式$\tilde{J}$的集合中，所以$(a_J')$是邻域的基 $A[[X]]$ 中的$0$（IV、p. 26）。现在，对于每个子集$J$和$m$元素，引理1意味着关系$a_J' \cap A[[X]]^{sym} = c_m$，这证明了引理3。

由于$S_k$中给定权的单项式只有有限数，因此每个形式的幂级数$f \in B$都可以以独特的方式写为$f = \sum_{r \geq 0} P_r$，其中$P_r$是权$r$在$B \cap A[S]$。对于每个整数$m \geq 0$，让$b_m$成为上述型的所有正式幂级数的$B$由……组成的理想，这样$P_r = 0$对于$0 \leq r < m$。 序列$(b_m)_{m \geq 0}$是$B$中$0$邻域基。

上面的记号$\psi_1(P_r)$是$X_i$中的对称形式幂级数，齐次于次数$r$，所以这是次数$r$的齐次分量$\psi_1(f)$。 引理 2 显示，对于每个整数 $m \geq 0$，$\psi_1$ 是 $B$ 的代数同态到 $A[[X]]^{sym}$、映射 $b_m$ 到 $c_m$；现在引理 3 显示 $\psi_1$ 是双连续的，这完成了定理 2 的证明。

### 4. 和 / 幂

我们再次为不确定的家庭写$X = (X_i)_{i \in I}$。对称形式幂级数 $s_k$ 定义为之前

$$
s_k = \sum_{H \in \mathfrak{P}_k} \prod_{i \in H} X_i \quad (k \geq 1),
$$

其中$\mathfrak{P}_k$是$I$的所有k元素子集的集合。我们也写

$$
p_k = \sum_{i \in I} X_i^k \quad (k \geq 1)
$$

这是对称形式幂级数，它是次数 k 的齐次。

#### 引理 4 (« 牛顿关系 ») {#alg-iv-s6-lem-4 .statement tag=06EP}

— *对于每个整数 $d \geq 1$ 我们有*

$$
p_d = \sum_{k=1}^{d-1} (-1)^{k-1} s_k p_{d-k} + (-1)^{d+1} d s_d
$$

让我们通过$A(u) = \sum_{n \geq 0} n u_n$在$\mathbf{A}[[\mathbf{X}]]$中构建定义连续的推导$A$，其中对于$\mathbf{A}[[\mathbf{X}]]$中的每个$u$，$u_n$是$u$的次数$n$的齐次分量。根据 (16) 和 *IV* 的命题 2，p. 27 我们有

$$
1 + \sum_{k \geq 1} s_k = \prod_{i \in I} (1 + X_i)
$$

根据 *IV* 的第 9 条命题，p. 34 我们有

$$
\left( \sum_{k \geq 1} k s_k \right) \cdot \left( 1 + \sum_{k \geq 1} s_k \right)^{-1} = \sum_{i \in I} \Delta(X_i)/(1 + X_i).
$$

我们有$A(X_i) = X_i$和$X_i/(1 + X_i) = \sum_{k \geq 1} (-1)^k \ X_i^k$。因此，(20) 的右侧等于 $\sum_{k \geq 1} (-1)^{k-1} p_k$。因此，由 (20) 我们有

$$
\sum_{k \geq 1} k s_k = \left( 1 + \sum_{k \geq 1} s_k \right) \cdot \left( \sum_{k \geq 1} (-1)^{k-1} p_k \right)
$$

现在引理 4 接下来是次数 d 的同质成分的比较。

#### 注 {#alg-iv-s6-n4-rem-1 .statement tag=06EQ}

— 有了上面证明的记号，我们有

$$
\Delta u = \sum_{i \in I} X_i \cdot D_i(u)
$$

（IV，p. 33，Cor.1）。在其他字中，*欧拉关系（IV，p. 8，命题6）*扩展到形式幂级数：如果$u \in A[X]$齐次于次数$n$，则

(21)
$$
n \cdot u = \sum_{i \in I} X_i \cdot D_i(u) .
$$

当 I 有限时，$n$ 元素中的由……组成，我们有 $s_k = 0$ 对应 $k > n$。那么牛顿的关系可以写成

$$
\begin{aligned}
p_2 &= s_1 p_1 - 2 s_2 \\
p_3 &= s_1 p_2 - s_2 p_1 + 3 s_3 \\
&\ \ \cdots \cdots \cdots \cdots \cdots \cdots \cdots \\
p_{n-1} &= s_1 p_{n-2} - s_2 p_{n-3} + \cdots + (-1)^{n-1} s_{n-2} p_1 + (-1)^n (n-1) s_{n-1} \\
p_n &= s_1 p_{n-1} - s_2 p_{n-2} + \cdots + (-1)^n s_{n-1} p_1 + (-1)^{n+1} n s_n
\end{aligned}
$$

和

(22)
$$
p_k = s_1 p_{k-1} - s_2 p_{k-2} + \cdots + (-1)^{n+1} s_n p_{k-n} \quad (\text{for } k > n) .
$$

上述关系的第一个$n$对于任何$I$都成立；我们找到例

$$
p_1 = s_1 , \quad p_2 = s_1^2 - 2 s_2 , \quad p_3 = s_1^3 - 3 s_1 s_2 + 3 s_3 .
$$

更一般地，令 $S = (S_n)_{n \geq 1}$ 为不定族。让我们通过 $P_1 = S_1$ 递归地计算定义多项式 $P_d \in \mathbf{Z}[S_1, \ldots, S_d]$ 并且

$$
P_d = \sum_{k=1}^{d-1} (-1)^{k-1} S_k P_{d-k} + (-1)^{d+1} d S_d \quad (d \geq 2) .
$$

那么我们就有了 « *通用公式* » $p_d = P_d(s_1, \ldots, s_d)$ 涵盖任何环 A 和不定族 X。
令 $P = (P_k)_{k \geq 1}$ 为不定数的序列。由于 $p_k$ 是 $A[[X]]$ 中次数 k 的齐次，因此恰好存在一个连续 A-代数同态

$$
\lambda_I : A[[P]] \to A[[X]]^{\mathrm{sym}}
$$

这样对于每个整数 $k \geq 1$ *(IV, p. 28)* 都有 $\lambda_I(P_k) = p_k$。 If we assign to $P_k$ the weight k, then $\lambda_I$ transforms an isobaric polynomial of weight $n$ in the $P_k$ into a formal power series which is homogeneous of degree $n$ in the $X_i$.

#### 命题 3 {#alg-iv-s6-prop-3 .statement tag=06ER}

— *a) 如果 I 是有限集合，且 n 元素且 $n! \cdot 1$ 在 A 中可逆，则 $\lambda_I$ 诱导 $A[[P_1, \ldots, P_n]]$ 的双连续同构到 $A[[X]]^{\mathrm{sym}}$。*
*b) 如果 I 是无穷大且 A 是 Q 代数，则 $\lambda_I$ 是 $A[[P]]$ 到 $A[[X]]^{\mathrm{sym}}$ 的双连续同构。*
我们将只处理*a)* 的情况，*b)* 的情况非常相似。

由 Th. 2（IV，p. 68）我们可以确定$\mathbf{A}[[\mathbf{X}]]^{\text{sym}}$与正式幂级数$\mathbf{A}[[S_1, \ldots, S_n]]$的代数，与$S_k$相应的到$s_k$。到 IV 的引理 4，p. 70，不定式 $s_1, \ldots, s_n$ 中存在阶 $\geq 2$ 的形式幂级数 $g_1, \ldots, g_s$，使得

$$
p_k = (-1)^{k+1} k s_k + g_k(s_1, \ldots, s_s) \quad (1 \leq k \leq n).
$$

由于$k! . 1$在IV的$\mathbf{A}$、引理 2中是可逆的，p. 35证明了拓扑$\mathbf{A}$-代数$\mathbf{A}[[\mathbf{X}]]^{\text{sym}}$的自同构$T$的存在性，其中映射$s_k$为$p_k$ 为 $l \leq k \leq n$。现在，第 3 条命题 a) 是直接的推论。

#### 推论{#alg-iv-s6-n4-cor-1 .statement tag=06ES}

— *令$\xi_1, \ldots, \xi_n, \eta_1, \ldots, \eta_n$为$\mathbf{A}$的元素，并假设$\mathbf{A}$为整环。*

a) *如果$s_k(\xi_1, \ldots, \xi_n) = s_k(\eta_1, \ldots, \eta_n)$对应$1 \leq k \leq n$，则存在置换$\sigma \in \mathfrak{S}_n$，使得$\eta_i = \xi_{\sigma(i)}$对应$1 \leq i \leq n$。*

b) *假设$n! . 1 \neq 0$在$\mathbf{A}$中并且*

$$
\xi_1^k + \cdots + \xi_n^k = \eta_1^k + \cdots + \eta_n^k
$$

$1 \leq k \leq n$。 *那么存在置换$\sigma \in \mathfrak{S}_n$使得$\eta_i = \xi_{\sigma(i)}$对应$1 \leq i \leq n$。*

在假设 a) 下，我们有 $\prod_{i=1}^n (X - \xi_i) = \prod_{i=1}^n (X - \eta_i)$。如果我们用$\eta_n$代替$X$，我们会发现$\prod_{i=1}^n (\eta_n - \xi_i) = 0$，并且由于$\mathbf{A}$是整环，所以存在整数$\sigma(n)$使得$l \ s \ \sigma(n) \leq n$和$\eta_n = \xi_{\sigma(n)}$。现在断言a)很容易跟在归纳后面，因为$\mathbf{A}[X]$是整环。

在 b) 的假设下，存在 $n$ 不定式中的命题 3 首一多项式 $\Pi_1, \ldots, \Pi_n$，其中$\mathbf{A}$ 的分数的域中的系数使得 $1 \leq k \leq n$ 具有$s_k = \Pi_k(p_1, \ldots, p_n)$。现在关系 (23) 意味着

$$
s_k(\xi_1, \ldots, \xi_n) = s_k(\eta_1, \ldots, \eta_n)
$$

对于$1 \leq k \leq n$，因此 b) 由 a) 得出。

### 5. 多项式的根中对称函数

考虑一个次数 $n$ 的一元多项式，系数为 $\mathbf{A}$：

$$
f = X^n + a_1 X^{n-1} + \cdots + a_{n-1} X + a_n.
$$

我们定义一个结合律、交换律和单位 $\mathbf{A}$-代数 $E_f$ 与生成元 $x_1, \ldots, x$ 和关系

$$
\sum_{i_1 < \ldots < i_k} x_{i_1} \ldots x_{i_k} = (-1)^k a_k \quad (1 \leq k \leq n).
$$

更准确地说，我们有

$$
E_f = A[X_1, ..., X_n]/a
$$

其中理想的$a$由$1 \leq k \leq n$的多项式$s_k + (-1)^{k+1} a_k$生成，$x_i$是$X_i$ mod $a$的剩余类类（对于$1 \leq i \in n$）。 关系(24)也相当于$f(X) = \prod_{i=1}^n (X - x_i)$。当存在任何歧义风险时，我们用 $x_{1,f}, ..., x_{n,f}$ 代替 $x_1, ..., x_n$。

#### 命题 4 {#alg-iv-s6-prop-4 .statement tag=06ET}

*设B为A到B的交换环、$\rho$同态和B的$\xi_1, ..., 5$、元素。假设关系$^\rho f(X) = \prod_{i=1}^n (X - \xi_i)$在B[X]中成立。那么存在且仅有一个环同态 $u : E_f \to B$，使得$\rho(a) = u(a . 1)$适用于所有$a \in A$，$u(x_i) = \xi_i$适用于$1 \leq i \leq n$。

我们通过 $\rho$ 认为 B 是结合律、交换律和单位A-代数。那么关系$^\rho f(X) = \prod_{i=1}^n (X - \xi_i)$也可以写成形式

$$
\sum_{i_1 < ... < i_k} \xi_{i_1} ... \xi_{i_k} = (-1)^k a_k . 1 \quad (1 \leq k \leq n)
$$

B 中。由于关系 (24) 定义 $E_f$ 的呈现，因此提出了第 4 条命题。

提案 4 证明了 $E_f$ 的名称“分解代数 of $f$”是合理的。 关系$f(X) = \prod_{i=1}^n (X - x_{i,f})$被称为“$f$的通用分解”。设$\sigma \in S_n$为置换；从$f(X) = \prod_{i=1}^n (X - x_{\sigma(i),f})$开始，存在A-代数$E_f$的自同构$t_\sigma$，其特征为$t_\sigma(x_{i,f}) = x_{\sigma(i),f}$代表$1 \leq i \leq n$。我们在$S_n$中有$\sigma, \tau$对应$t_{\sigma \tau} = t_\sigma \circ t_\tau$，因此获得群$\mathscr{G}$的作用，即A-代数$E_f$。

#### 命题 5 {#alg-iv-s6-prop-5 .statement tag=06EU}

*在通用的分解代数$E_f$单项式$x_1^{\nu(1)} ... x_n^{\nu(n)}$家族中，$1 \leq i \leq n$的$0 \leq \nu(i) < i$是A-模$E_f$的基。特别地，$E_f$是秩$n!$中的自由A-模。

写出$B = A[X_1, ..., X_n]$和$C = A[X_1, ..., X_n]^{\text{sym}}$。由 Th. 1 (*IV*, p. 62) 我们有$C = A[s_1, ..., s_n]$和$s_1, ..., s_n$在代数上独立于A。$s_1, ..., s_n$形式中没有常数项的多项式是C中的理想$C^+$，补充于A并由$s_1, ..., s_n$生成。令c为由$s_1 + a_1, s_2 - a_2, ..., s_n + (-1)^{n+1} a_n$生成的C的理想。 C 存在 A-代数自同构，其中 $1 \leq k \leq n$ 存在映射 $s_k$ 到 $s_k + (-1)^{k+1} a_k$，因此映射 $C^+$ 到 c ；因此我们有$C = A \oplus c$。此外，Th。 *IV*, p. 62 的 1, c) 表明

$$
B = \bigoplus_{\nu \in S} CX^\nu
$$

其中 S 是所有 $\nu \in \mathbf{N}^n$ 中的集合，使得 $0 \leq \nu(i) < i$ 对应于 $1 \leq i \leq n$。 B 的理想 a 由 c 生成，从而 $a = Bc = \bigoplus_{\nu \in S} c \cdot X^\nu$。从$C = A \oplus c$开始，我们发现
$$
B = a \oplus \bigoplus_{\nu \in S} AX^\nu,
$$
从而提案 5，因为 $E_f = B/a$。

#### 推论{#alg-iv-s6-n5-cor-1 .statement tag=06EV}

— *A 的典范同态到一元多项式 $f \in A[X]$ 的通用分解代数是单射的。*

对于$E_f$形式单位元部分基A-模$E_f$。

#### 命题 6 {#alg-iv-s6-prop-6 .statement tag=06EW}

— *令 $f \in A[X]$ 为次数 n 的一元多项式，并令 P 为 $X_1, ..., X_n$ 中的对称多项式，系数在 A 中。则恰好存在 A 的一个元素 a ，其性质如下：
(FS) 对于 B[X] 中的任意环同态 $\rho : A \to B$ 和分解 $^0f(X) = \prod_{i=1}^n (X - \xi_i)$，我们有 $\rho(a) = P(\xi_1, ..., \xi_n)$。*

写 $f = X^n + \sum_{k=1}^n a_k X^{n-k}$，然​​后写 Th。 1, IV, p. 62 存在n个不定式中的多项式$\Pi$，系数在A中，使得$P = \Pi(s_1, ..., s_n)$。输入$a = \Pi(-a_1, a_2, ..., (-1)^n a_n)$。在假设 (FS) 下我们有
$$
s_k(\xi_1, ..., \xi_n) = (-1)^k \rho(a_k)
$$
从而
$$
\begin{align*}
\rho(a) &= \Pi(-\rho(a_1), \rho(a_2), ..., (-1)^n \rho(a_n)) \\
&= \Pi(s_1(\xi_1, ..., \xi_n), ..., s_n(\xi_1, ..., \xi_n)) \\
&= P(\xi_1, ..., \xi_n) .
\end{align*}
$$

这就证明了元素满足(FS)的存在。 a 的唯一性来自 Cor。到提案 5，因为我们在通用分解代数 $E_f$ 中有 $a \cdot 1 = P(x_{1,f}, ..., x_{n,f})$。

对于第 6 条命题的记号，其中一个有时写为$a = P^*(f)$。这里有一些例。

#### 例 {#alg-iv-s6-n5-exa-1 .statement tag=0DHL}

*1) 如果$P = s_k$，则$P^*(f) = (-1)^k a_k$。
\* 2) 令 g 为 $A[X]$ 中的多项式并放入
$$
P(X_1, ..., X_n) = g(X_1) ... g(X_n) .
$$
那么 $P^*(f)$ 就是结果 $\operatorname{res}(f, g)$，Cor. IV 中的 1，p. 80。
3) 代入$A(X_1, ..., X_n) = \prod_{i < j} (X_i - X_j)^2$，那么$\Delta^*(f)$就是一元多项式$f$(IV,p. 82,公式(46))的判别式。 \*

4）放入$P(X_1, \ldots, X_n) = X_1^k + \ldots + X_n^k$；另外，将$E$中的$X$的像记入定义代数$E = A[X]/(f)$并记入$x$。我们记得$A$-模块$E$是免费的，还有基$(1, x, \ldots, x^{n-1})$（IV，p. 11，Cor.）。让我们展示一下

$$
\text{Tr}_{E/A}(x^k) = P^*(f)
$$

将$\pi_k = \text{Tr}_{E/A}(x^k)$对应于每个整数$k \geq 1$。考虑到牛顿的关系 (IV, p. 70) 我们只需要建立关系

$$
\begin{align*}
&\pi_k + a_1 \pi_{k-1} + \cdots + a_{k-1} \pi_1 + k a_k = 0 \quad \text{for } 1 \leq k \leq n \\
&\pi_k + a_1 \pi_{k-1} + \cdots + a_{n-1} \pi_{k-n+1} + a_n \pi_{k-n} = 0 \quad \text{for } k > n
\end{align*}
$$

（我们也将其称为“牛顿关系”）。 关系 (27) 很清楚，因为左边是

$$
x^{k-n}(x^n + a_1 x^{n-1} + \cdots + a_{n-1} x + a_n) = 0 .
$$

假设 $1 \leq k \leq n$ 并把

$$
y = x^k + a_1 x^{k-1} + \cdots + a_{k-1} x + a_k \cdot 1 ;
$$

令$M = (m_{ij})$为$E$中线性映射$u \mapsto yu$相对于基$(x')_{0,\ldots,n}$的矩阵。我们很容易得到关系

$$
\begin{align*}
&m_{ii} = a_k \quad \text{for } 0 \leq i < n - k \\
&m_{ii} = 0 \quad \text{for } n - k \leq i < n ,
\end{align*}
$$

whence

$$
\text{Tr}_{E/A}(y) = \sum_{i=0}^{n-1} m_{ii} = (n-k) a_k .
$$

此外我们还有

$$
\text{Tr}_{E/A}(y) = \pi_k + a_1 \pi_{k-1} + \cdots + a_{k-1} \pi_1 + n a_k ,
$$

从而公式 (26)如下。

### 6. 结果

在这个数中，我们假设给定两个正整数$p, q$和形式的$A[X]$中的两个多项式$f, g$

$$
\begin{align*}
f &= t_p X^p + t_{p-1} X^{p-1} + \cdots + t_0 \\
g &= u_q X^q + u_{q-1} X^{q-1} + \cdots + u_0
\end{align*}
$$

这样$\deg f \leq p, \deg g \leq q$。对于每个整数$n \geq 0$，我们用$S$表示，次数$< n$所有多项式的$A[X]$由……组成的子$A$模；它的族$(X')_{0 \leq i < n}$为基，因此属于秩$n$。

我们提供 $S, \times S_p$ 和基
$$
B_1 = ((X^{q-1}, 0), ..., (X, 0), (1, 0), (0, X^{p-1}), ..., (0, X), (0, 1))
$$
和 $S_{p+q}$ 与基
$$
B_2 = (X^{p+2-1}, ..., X, 1).
$$
我们定义线性映射$\varphi : S, \times S_p \to S_{p+q}$
$$
\varphi(u, v) = uf + vg
$$
对于基$B_1$和$B_2$，我们用$\varphi$的$M(f, g, p, q)$矩阵来表示。这是阶 $p + q$ 中的平方矩阵，由集合 $\{0, 1, ..., p + q - 1\}$ 索引。它的元素$a_{ij}$由规则给出：
a) $a_{ij} = t_{p-i+j}$ 为$0 \leq j \leq q-1$，
b) $a_{ij} = u_{j-i}$ 为$q \leq j \leq p + q - 1$，
其中，如果 $k \notin (0, p)$，$t_k$ 被视为 0；如果 $k \notin (0, q)$，$u_k = 0$。

对于例，当$p = 2$和$q = 3$时，我们有矩阵
$$
\begin{pmatrix}
t_2 & 0 & 0 & u_3 & 0 \\
t_1 & t_2 & 0 & u_2 & u_3 \\
t_0 & t_1 & t_2 & u_1 & u_2 \\
0 & t_0 & t_1 & u_0 & u_1 \\
0 & 0 & t_0 & 0 & u_0
\end{pmatrix}.
$$

#### 定义 1 {#alg-iv-s6-def-1 .statement tag=06EX}

*对于上述记号，矩阵$M(f, g, p, q)$的行列式被称为次数$p$和$q$的对$(f, g)$的结果，或者简称为$f$和$g$的结果，如果$p = \deg f$ 和$q = \deg g$。*

当 $p = \deg f$、$q = \deg g$ 时，结果表示为 $\operatorname{res}_{p,q}(f, g)$ 或简称为 $\operatorname{res}(f, g)$。

#### 例 1 {#alg-iv-s6-n6-exa-1 .statement tag=06EY}

给定 $\Lambda$ 中的 $\Lambda, \mu$，我们有公式
$$
\operatorname{res}_{p,0}(f, \lambda) = \lambda^p, \quad \operatorname{res}_{0,q}(\mu, g) = \mu^q
$$
$$
\operatorname{res}_{p,1}(f, \lambda) = \lambda^p t_p, \quad \operatorname{res}_{1,q}(\mu, g) = (-1)^q \mu^q u_q,
$$
其证明为直接的。

#### 例 2 {#alg-iv-s6-n6-exa-2 .statement tag=06EZ}

当$p = q = 1$时，我们有
$$
\operatorname{res}_{1,1}(t_1 X + t_0, u_1 X + u_0) = t_1 u_0 - t_0 u_1
$$

#### 注 1 {#alg-iv-s6-n6-rem-1 .statement tag=06F0}

矩阵 $M(g, f, q, p)$ 是由 $M(f, g, p, q)$ 通过列、从而 $pq$ 转置获得
$$
\operatorname{res}_{q,p}(g, f) = (-1)^{pq} \operatorname{res}_{p,q}(f, g)
$$

#### 注 2 {#alg-iv-s6-n6-rem-2 .statement tag=06F1}

设$\rho : A \to B$为环同态。定义。 / 直接暗示公式
$$
\operatorname{res}_{p,q}(\rho f, \rho g) = \rho(\operatorname{res}_{p,q}(f, g)) .
$$

#### 注 3 {#alg-iv-s6-n6-rem-3 .statement tag=06F2}

给定 $A$ 中的 $\lambda, \mu$，我们有
$$
\operatorname{res}_{p,q}(\lambda f, \mu g) = \lambda^q \mu^p \operatorname{res}_{p,q}(f, g) .
$$
(28)

#### 注 4 {#alg-iv-s6-n6-rem-4 .statement tag=06F3}

假设$p + q \geq 1$。由III、p. 532、公式(28)、像的$\varphi$包含常数多项式$\operatorname{res}_{p,q}(f, g)$。因此存在多项式 $(u, v)$ 的对，其中 $u \in S_q, v \in S_p$ 使得
$$
\operatorname{res}_{p,q}(f, g) = uf + vg ,
$$
从而
$$
\operatorname{res}_{p,q}(f, g) \in A \cap (f, g) .
$$
当 $\operatorname{res}_{p,q}(f, g)$ 在 $A$ 中可取消时，对 $(u, v)$ 是唯一的：因为此时 $\varphi$ 是单射的（III，p. 524，命题 3）。

#### 注 5 {#alg-iv-s6-n6-rem-5 .statement tag=06F4}

假设$p \geq q$，并令$h \in A[X]$为次数$\leq p - q$的多项式。让我们证明
$$
\operatorname{res}_{p,q}(f, g) = \operatorname{res}_{p,q}(f + gh, g) .
$$
(29)
因为如果我们将$(u, v) \in S_q \times S_p$写成$\omega(u, v) = (u, uh + v)$，那么$w$就是$A$模块$S_q \times S_p$的自同构，并且我们有
$$
\omega^{-1}(u, v) = (u, -uh + v) .
$$
$w$相对于基$B_1$的矩阵是下三角形，其对角线元素等于$1$。另一方面，$\varphi \circ w$映射$(u, v)$至$u(f + gh) + vg$。现在公式(29)意味着代表$\varphi$和$\varphi \circ w$的矩阵具有相同的行列式，这是从关系$\det w = 1$得出的。

假设$f$是次数$p$的单调；将$E = A[X]/(f)$放入$E$中，用$X$的$x$典范像表示。我们知道（IV，p. 11）$E$是一个免费的$A$模块，具有基$(1, x, \ldots, x^{p-1})$。因此，我们可以对 $E$ 的任意元素 $u$ 进行定义范数 $N_{E/A}(u)$ (III, p. 543, Def. 2)。

#### 命题 7 {#alg-iv-s6-prop-7 .statement tag=06F5}

— *假设 f 是次数 p 的一元函数；有了上面的记号我们就有了*¹
$$
\operatorname{res}_{p,q}(f, g) = N_{E/A}(g(x)) .
$$
(30)

1 因此，当 $f$ 是次数 $p$ 的单调时，所得$\operatorname{res}_{p,q}(f, g)$ 独立于$q$。然后我们简单地用 $\operatorname{res}(f, g)$ 来表示它。

让我们将$S_q \times S_p$的定义A-线性映射$0$通过$\theta(u, v) = uf + v$转化为$S_{p+q}$。然后将$S_q \times S_s$中的$0$映射基$B_1$转化为序列
$$
(fX^{q-1}, \ldots, fX, f, X^{p-1}, \ldots, X, 1)
$$
元素 $S_{p+q}$；因此矩阵$M$，$0$相对于基$B_1, B_2$是下三角形，其对角线元素等于1，从而$\det M = 1$。

由此可知 $\theta$ 是双射且 $\operatorname{res}_{p,q}(f, g)$ 等于自同态 $\varphi' = \varphi \circ \theta^{-1}$ 的行列式 $S_{p-q}$。明确地，我们有
$$
\varphi'(uf + v) = uf + vg
$$
对于$S_q \times S_s$中的任何对$(u, v)$。现在我们有$A[X] = S_{p+q} + (f)$和$fS_q = S_s \cap (f)$，因此通过将$S_{p+q}/fS_q$的商同构$\gamma$到E上，将$S_{p-s}$的典范嵌入转化为$A[X]$定义。令$\psi$为E 中的乘法与 $g(x)$。 公式 (31) 表明 $\varphi'$ 诱导 $fS_q$ 上的恒等式和 $S_{p+q}/fS_q$ 上的 $\gamma^{-1}\psi\gamma$ 恒等式。因此，我们有$\det \varphi' = \det \psi$，从而 (30)，因为$\det \varphi' = \operatorname{res}_{p,q}(f, g)$和$\det \psi = N_{E/A}(g(x))$，通过定义。

#### 推论 1 {#alg-iv-s6-prop-7-cor-1 .statement tag=06F6}

— 令 $f \in A[X]$ 为一元多项式；对于每个多项式 $g \in A[X]$，以下条件是等效的：
(i) $\operatorname{res}(f, g)$ 在 $A$ 中可逆；
(ii) $A[X]$中存在多项式$u, v$使得$uf + vg = 1$；
(iii) $g(x)$ 在代数 $A[X]/(f)$ 中可逆。
(i)和(iii)的等价源自III的第3条、p. 545和第7条提案； (ii) 和 (iii) 的内容很简单。

#### 推论 2 {#alg-iv-s6-prop-7-cor-2 .statement tag=06F7}

— 假设 $A$ 为域并设 $f, g \in A[X]$，则当 $f, g$ 非零时，以下条件等价：
（一）$\operatorname{res}(f, g) \neq 0$；
(ii) 首一多项式$f$和$g$在$A[X]$互质；
\* (iii) 对于 A 的任何扩张 L，首一多项式 $f$ 和 $g$ 在 L 中没有公共的根。 \*

我们可以立即将约化转换为 $f$ 是单调的情况（IV，p. 77，注 3）。
(i)和(ii)的等价只是Cor的翻译。 1，由Def。 IV 中的 1 个，p. 12； (ii) 和 (iii) 的等价就是 Cor。 IV 之 7，p. 13。

#### 推论 3 {#alg-iv-s6-prop-7-cor-3 .statement tag=06F8}

— 对于每一个$\lambda \in A$，我们有
$$
\operatorname{res}_{p,1}(f, \lambda - X) = f(\lambda), \quad \operatorname{res}_{1,q}(X - \lambda, g) = g(\lambda).
$$
当$f(X) = X - \lambda$时，代数E等于A，我们有$x = A$；第二个公式 (32) 现在来自第 7 号提案 (IV, p. 77)。到注 1 和 3（IV、p. 76、77）我们结论
$$
\operatorname{res}_{p,1}(f, \lambda - X) = (-1)^p \operatorname{res}_{1,p}(\lambda - X, f) = (-1)^{p+p} \operatorname{res}_{1,p}(X - A, f) = f(A).
$$

现在假设 f 和 g 是单调的。我们用 F A-代数 $A[X, Y]/(f(X), g(Y))$ 表示，并用 F 中的 X（分别 Y）的 x（分别 y）典范像表示。

#### 命题 8 {#alg-iv-s6-prop-8 .statement tag=06F9}

— 假设 f 和 g 分别是次数 p 和 q 的一元函数。有了上面的记号，A-模 F 与基 $(x^i y^j)_{0 \leq i < p,\ 0 \leq j < q}$ 是免费的，我们有

$$
\text{res}(f, g) = N_{F/A}(x - y).
$$

输入$E = A[X]/(f)$和$E' = A[Y]/(g)$。作者：II，p. 253，Cor。 1、从典范同态$A[X] \otimes A[Y] \to A[X, Y]$导出$E @ E'$入F的同态$\sigma$是双射的；这证明了F的断言关于基。我们现在认同E及其在$\sigma$下的F中的像。那么$E[Y]/(g(Y))$到F的E-代数同态，其中映射Y到y是同构。

到范数（III，p. 546）的传递性，我们有

$$
N_{F/A}(x - y) = N_{E/A}(N_{F/E}(x - y)).
$$

根据命题 7 (IV, p. 77)，$N_{F/E}(x - y)$ 是 E[Y] 中多项式 g(Y) 和 x − Y 的结果，因此等于 g(x) (IV, p. 78，Cor. 3)。根据公式 (34) 和命题 7 (IV, p. 77)，我们有

$$
N_{F/A}(x - y) = N_{E/A}(g(x)) = \text{res}(f, g)
$$

#### 命题 9 {#alg-iv-s6-prop-9 .statement tag=06FA}

— 设$p_1$和$q_1$为正整数和$f_1, g_1$多项式$A[X]$，使得$\deg f_1 \leq p_1, \deg g_1 \leq q_1$；那么我们有

$$
\text{res}_{p, q + q_1}(f, gg_1) = \text{res}_{p, q}(f, g) \cdot \text{res}_{p, q_1}(f, g_1)
$$
$$
\text{res}_{p + p_1, q}(ff_1, g) = \text{res}_{p, q}(f, g) \cdot \text{res}_{p_1, q}(f_1, g).
$$

我们有$\text{res}_{p, q}(f, g) = (-1)^{pq} \text{res}_{q, p}(g, f)$（IV，p. 76）；所以证明(35)就足够了。同样，注 3（前述）表明，如果公式 (35) 对于多项式 $f$ 成立，则它适用于形式 Af 的所有多项式，其中 $A \in A$。最后，当 f 是次数 p 的 monic 时，公式 (35) 由命题 7 (IV, p. 77) 得出公式 $N_{E/A}(ab) = N_{E/A}(a) \cdot N_{E/A}(b)$。总之，当 f 中 $X^p$ 的系数 $t_p$ 可逆时，我们结论成立（35）。

#### 引理 5 {#alg-iv-s6-lem-5 .statement tag=06FB}

令t为A的元素。存在交换环C包含A作为C子环，C包含A的子环B，B的元素$\tau$可逆于C和环同态$p : B \to A$使得p到A的$p(\tau) = t$和限制等于Id。

只需取幺半群$\mathbf{N}$的B代数$A^{(\mathbf{N})}$，即一个不定$\tau$中的多项式代数$A[\tau]$，对于群的C代数$A^{(\mathbf{Z})}$就足够了$\mathbf{Z}$ 并将 $A(\tau)$ 的 p 同态 $P \mapsto P(t)$ 放入 A 中。

记号为引理 5，我们取 t = t_p，让我们把
$$
F = \tau X^p + t_{p-1} X^{p-1} + \cdots + t_1 X + t_0
$$
在 B[X] 中。 F 中的 $X^p$ 系数在 C 中可逆；如果我们将 F, g, $g_1$ 视为 C[X] 的多项式，我们有
$$
\operatorname{res}_{p,q+q_1}(F, gg_1) = \operatorname{res}_{p,q}(F, g) \cdot \operatorname{res}_{p,q_1}(F, g_1)
$$
根据已经说过的内容。如果我们将 F、g 和 $g_1$ 视为 B[X] 中的多项式，则结果不变。由于 $^\rho F = f$、$^\rho g = g$、$^\rho g_1 = g_1$、公式 (35) 由 (38) 和注 2 (IV, p. 77) 得出。

#### 推论 1 {#alg-iv-s6-lem-5-cor-1 .statement tag=06FC}

— (i) 令 $\lambda, \alpha_1, \ldots, \alpha_p$ 为 A 的元素，并假设 $f(X) = \lambda (X - \alpha_1) \ldots (X - \alpha_p)$。我们有
$$
\operatorname{res}_{p,q}(f, g) = \lambda^q g(\alpha_1) \ldots g(\alpha_p) .
$$
(ii) 设$\mu, \beta_1, \ldots, \beta_q$为A的元素，并进一步假设$g(X) = \mu (X - \beta_1) \ldots (X - \beta_q)$。然后我们有
$$
\operatorname{res}_{p,q}(f, g) = \lambda^q \mu^p \prod_{\substack{1 \leq i \leq p \\ 1 \leq j \leq q}} (\alpha_i - \beta_j) .
$$
断言 (i) 直接从公式 (28)、(32) 和 (36) 得出。现在断言 (ii) 由 (i) 得出。

#### 推论 2 {#alg-iv-s6-lem-5-cor-2 .statement tag=06FD}

— 对于每整数 $r \geq 0$，我们有
$$
\operatorname{res}_{p,q+r}(f, g) = t_p^r \cdot \operatorname{res}_{p,q}(f, g) .
$$
记住例 1 (IV, p. 76)，我们只需要在(35)中取$q_1 = r, g_1 = 1$。

假设 f 是单调的，并令 B 的 $\rho : A \to B$ 为环同态和 $\xi_1, \ldots, \xi_p$ 元素，这样我们就有分解
$$
^\rho f(X) = (X - \xi_1) \ldots (X - \xi_p)
$$
由注2（IV，p. 77）和Cor。 1 上面我们有
$$
\rho(\operatorname{res}(f, g)) = g(\xi_1) \ldots g(\xi_p)
$$
这个注特别适用于通用分解关闭（IV，p. 73），并且由于$\rho$是单射的，这提供了计算$\operatorname{res}(f, g)$的方法。

#### 例 3 {#alg-iv-s6-n6-exa-3 .statement tag=06FE}

让我们证明公式
$$
\operatorname{res}_{2,2}(aX^2 + bX + c, a'X^2 + b'X + c') =
(ac' - ca')^2 + (bc' - cb')(ba' - ab')
$$

对于第 9 条命题（IV，p. 79）的论证，我们发现当 $a$ 可逆时，证明公式就足够了。那么存在形式中的分解

$$
aX^2 + bX + c = a(X - x)(X - y)
$$

在$B[X]$中，其中$B$是适当的环包含$A$作为子环。由科. 1 上面，所需的结果等于

$$
R = a^2(a'x^2 + b'x + c')(a'y^2 + b'y + c') .
$$

现在我们有

$$
ax + ay = -b , \quad axy = c
$$

由（43），从而$(ax)^2 + (ay)^2 = b^2 - 2ac$。

由 (44) 我们有

$$
R = {a'}^2(axy)^2 + a{b'}^2(axy) + a^2{c'}^2 + a'b'(axy)(ax + ay) +
$$
$$
+ a'c'((ax)^2 + (ay)^2) + ab'c'(ax + ay)
$$
$$
= {a'}^2c^2 + a{b'}^2c + a^2{c'}^2 - a'b'cb + a'c'(b^2 - 2ac) - ab'c'b
$$
$$
= (ac' - ca')^2 + (ab' - a'b)(b'c - c'b) ,
$$

由此得出所需的结果。

### 7. 判别式

#### 定义 2 {#alg-iv-s6-def-2 .statement tag=06FF}

*令$f$为次数$m$的$A[X]$的一元多项式，并用$E$表示$A$代数$A[X]/(f)$，并用$X$的$x$典范像表示$E$。我们将定义$f$的判别式写为$\operatorname{dis}(f)$，作为$A$-代数$E$的基$(1, x, \ldots, x^{m-1})$的判别式$D_{E/A}(1, x, \ldots, x^{m-1})$。*

对于每个正整数 $k$，我们写 $\rho_k = \operatorname{Tr}_{E/A}(x^k)$。由 III，p. 549，Def。 2 相当于公式

$$
\operatorname{dis}(f) = \det(p_{i+j})_{0 \leq i,j < m}
$$

*例。 — 1) 如果 $f$ 是次数 0 或 1 的一元多项式，则由 (45) 得到 $\operatorname{dis}(f) = 1$。
2) 令 $f(X) = X^2 + \alpha X + \beta$ 为次数的一元多项式 2. 牛顿的关系可以写成形式 (IV, p. 75)

$$
p_0 = 2 \\
p_1 + \alpha = 0 \\
p_2 + \alpha p_1 + 2\beta = 0 ,
$$

从而$p_1 = -a$、$p_2 = a^2 - 2p$。由此可见我们有

$$
\operatorname{dis}(f) = \det \begin{pmatrix} 2 & -\alpha \\ -a & \alpha^2 - 2p \end{pmatrix} = \alpha^2 - 4\beta
$$

令 B 为从 A 到 B 的交换环、$\rho$ 同态以及 B 的 $\xi_1, \ldots, \xi_m$ 元素，使得
$$
\rho f(X) = (X - \xi_1) \cdots (X - \xi_m).
$$
让我们将矩阵 $(\rho(p_{i + j}))_{0 \leq i, j < m}$ 写为 M，将 Van der Monde 矩阵 $(\xi_i^{j+1})_{0 \leq i, j < m}$ 写为 D。到 IV 的例 4，p. 75 我们有
$$
\rho(p_k) = \xi_1^k + \cdots + \xi_m^k,
$$
从而$M = 'D . D ;$由III，p. 532我们有$D = \prod_{i > j} (\xi_i - \xi_j)$和$\det M = (\det D)^2$，即
$$
\rho(\operatorname{dis}(f)) = \prod_{i < j} (\xi_i - \xi_j)^2
$$
此外（在为推导 $\frac{d}{dX}$ 写 D 时）我们有
$$
D(\rho f)(\xi_i) = (\xi_i - \xi_1) \cdots (\xi_i - \xi_{i-1})(\xi_i - \xi_{i+1}) \cdots (\xi_i - \xi_m)
$$
$1 \leq i \leq m$、从而
$$
\rho(\operatorname{dis}(f)) = (-1)^{m(m-1)/2} \prod_{i \neq j} (\xi_i - \xi_j) = (-1)^{m(m-1)/2} \prod_{i=1}^m D(\rho f)(\xi_i).
$$
由科. IV的1，p. 80应用到$f$的通用分解，我们最终得到
$$
\operatorname{res}(f, Df) = \operatorname{res}(Df, f) = (-1)^{m(m-1)/2} \operatorname{dis}(f).
$$

#### 命题 10 {#alg-iv-s6-prop-10 .statement tag=06FG}

让$m \geq 1$。存在一个唯一的多项式 $A \in \mathbf{Z}[A_1, \ldots, A_m]$ ，其性质 ：对于任何交换环 A 和 $A[X]$ 中的 *monic* 首一多项式 $f = X^m + \sum_{i=1}^m a_i X^{m-i}$，我们有
$$
\operatorname{dis}(f) = \Delta(a_1, \ldots, a_m).
$$
此外，A 是次数 $\leq 2m-2$，如果我们将权 i 分配给 $A_i$，则 A 是权 $m(m-1)$ 的同量异位。
a) A 的唯一性 ：如果 A 满足 (48)，我们特别有 $A = \operatorname{dis}(F)$，其中 F 是系数为 $\mathbf{Z}[A_1, \ldots, A_m]$ 的多项式 $X^m + \sum_{i=1}^m A_i X^{m-i}$。
b) **A* 的存在性：令 $s_1, \ldots, s_m$ 为不定式 $X_1, \ldots, X_m$ 中的初等对称多项式。存在一个多项式 $A \in \mathbf{Z}[A_1, \ldots, A_m]$，等压于权 $m(m-1)$，使得
$$
\Delta(-s_1, s_2, \ldots, (-1)^m s_m) = \prod_{i < j} (X_i - X_j)^2;
$$

右边是对称多项式 P，在 $Z[X_1, ..., X_m]$ (IV, p. 62, Th. 1) 中齐次于次数 m(m − 1)。现在公式 (46) 意味着 dis(f) = P (f )，在 IV 的记号中，p. 74 和 (48) 直接由此得出。

c) A 的次数：结果 (IV, p. 76) 的关系 (47) 和定义意味着公式

$$
(-1)^{m(m-1)/2} \Delta = \det(a_{ij})_{0 \leq i,j \leq 2m-2}
$$

与 $a_{ij}$ 中的以下值

$$
\begin{align*}
a_{00} &= 1 , \quad a_{0,m-1} = m , \\
a_{ij} &= A_{i-j} & \text{for } 1 \leq i \leq 2m-2 , \quad 0 \leq j \leq m-2 \\
a_{ij} &= (j-i+1) A_{m+i-j-1} & \text{for } 1 \leq i \leq 2m-2 , \quad m-1 \leq j \leq 2m-2 .
\end{align*}
$$

$a_{0j} = 0$ 如果$j \neq 0 , \ j \neq m-1$

在这些公式中，$A_i = 1$和$A_i = 0$被理解为$i < 0$或$i > m$。现在 (50) 立即表明 A 是次数 $\leq 2m-2$，正如我们必须证明的那样。

命题 10 允许我们将判别式扩展定义与非单调多项式。令 $m \geq 1$ 为整数，则在 $Z[A_0, A_1, ..., A_m]$ 中存在唯一齐次多项式次数 $2m-2$、$\tilde{\Delta}$，使得

$$
\Delta(A_1, ..., A_r) = \tilde{\Delta}(1, A_1, ..., A_r)
$$

因为，由于 A 是次数 $\leq 2m-2$，所以有理分数

$$
A_0^{2m-2} \Delta(A_1/A_0, ..., A_m/A_0)
$$

属于至子环 $Z[A_0, A_1, ..., A_m]$ 共 $Q(A_0, A_1, ..., A_m)$。如果 $A_i$ 有权 i 代表 $0 \leq i \leq m$，则 $\tilde{\Delta}$ 是权 $m(m-1)$ 的同量异位素。 Iff 是次数 $\leq m$ 的多项式，例如

$$
f = a_0 X^m + a_1 X^{m-1} + \cdots + a_{m-1} X + a_m ,
$$

我们将把

$$
\operatorname{dis}_m(f) = \tilde{\Delta}(a_0, a_1, ..., a_r).
$$

当$m = \deg f$时，我们只需将$\operatorname{dis}_m(f)$写成dis(f)即可；如果 f 是单调的，则 dis(f) 与 Def 中定义的判别式一致。 2，通过(48)、(51)和(52)。

#### 命题 11 {#alg-iv-s6-prop-11 .statement tag=06FH}

— 设 $A[X]$ 中的 f 为次数 $\leq m$。

(i) *如果* $\rho : A \to B$ 是环同态，我们有 $\operatorname{dis}_m(\rho_f) = \rho(\operatorname{dis}_m(f))$。

(ii) 设 $\lambda, \alpha_1, ..., a_r$ 为 A 的元素。*如果* $f = X(X-\alpha_1) ... (X-a_r)$；那么我们有

$$
\operatorname{dis}_m(f) = \lambda^{2m-2} \prod_{i < j} (\alpha_i - \alpha_j)^2 .
$$

(iii) 令$a_0$为$X^m$在$f$中的系数；那么我们有

$$
\text{res}_{m,m-1}(f, Df) = \text{res}_{m-1,m}(Df, f) = (-1)^{m(m-1)/2} a_0 \text{ dis}_m(f) .
$$

断言 (i) 很清楚。

由于 $\tilde{\Delta}$ 是次数 $2m - 2$ 的齐次，我们有

$$
\text{dis}_m(\lambda f) = \lambda^{2m-2} \text{dis}_m(f)
$$

对于次数 $\leq m$ 的每个多项式 $f \in A[X]$。 断言 (ii) 现在源自公式 (46) 和 (55)。

当$f$是次数$m$的单调时，我们有$a_0 = 1$并且断言(iii)减少到公式(47)。牢记 (55) 和关系

$$
\text{res}_{m,n}(\lambda f, \mu g) = \lambda^n \mu^m \text{res}_{m,n}(f, g),
$$

(IV, p. 77)，我们可以从那里转到$a_0$在$A$中可逆的情况。现在一般情况遵循提案 11, (i) 和引理 5 (IV, p. 79)。

#### 推论 1 {#alg-iv-s6-prop-11-cor-1 .statement tag=06FI}

— 令 $g \in A[X]$ 且令 $n$ 为正整数，使得 $\deg g \leq n$。我们有

$$
\text{dis}_{m+n}(fg) = \text{dis}_m(f) \cdot \text{dis}_n(g) \cdot \text{res}_{m,n}(f,g)^2 .
$$

到推理为之前，我们就被简化为$f$和$g$分别是次数、$m$和$n$的单调。现在输入$B = E_f \otimes E_g$，其中$E_f$（或$E_g$）是$f$（或$g$）的通用分解代数（IV，p. 73）。那么$A$是$B$的子环，在$B[X]$中我们有分解

$$
f = \prod_{i=1}^m (X - \alpha_i), \quad g = \prod_{j=1}^n (X - \beta_j) .
$$

因此我们有

$$
fg = \prod_{k=1}^{m+n} (X - \gamma_k) ,
$$

$\gamma_i = \alpha_i$ 代表$1 \leq i \leq m$，$\gamma_{m+j} = \beta_j$ 代表$1 \leq j \leq n$。我们有明显的身份

$$
\prod_{k < k'} (\gamma_k - \gamma_{k'}) = \prod_{i < i'} (\alpha_i - \alpha_{i'}) \cdot \prod_{j < j'} (\beta_j - \beta_{j'}) \cdot \prod_{i,j} (\alpha_i - \beta_j)
$$

通过对关系进行平方，我们可以通过 (40) 和 (46) 得到 (57)。

#### 推论 2 {#alg-iv-s6-prop-11-cor-2 .statement tag=06FJ}

— 如果$a_0$是$X^m$在$f$中的系数，我们有

$$
\text{dis}_{m+1}(f) = a_0^2 \text{dis}_m(f)
$$

这是从 Cor 得出的。 1 服用$n = 1,\ g = 1$，由公式$\operatorname{res}_{m,1}(f,1) = a_0$（IV、p. 76、例 1）。

#### 推论 3 {#alg-iv-s6-prop-11-cor-3 .statement tag=06FK}

— 令 $A$ 为域，并令 $f$ 为 $A[X]$ 中的非常数多项式。为了使$f$和$Df$互质，$\mathrm{dis}(f) \neq 0$是充分必要的。
这是根据第 11 号提案 (iii) 和 Cor. 得出的。 IV 之 2，p. 78。

#### 注 {#alg-iv-s6-n7-rem-1 .statement tag=06FL}

Cor 的双重应用。上面的 2 显示，对于次数 $\leq m - 2$ 的每个多项式 $f$，我们都有 $\mathrm{dis}_m(f) = 0$。

#### 例 3 {#alg-iv-s6-n7-exa-3 .statement tag=06FM}

让$m = 2$。通过示例 2 (IV, p. 81)，我们有 $\Delta(A_1, A_2) = A_1^2 - 4A_2$，从而 $\tilde{\Delta}(A_0, A_1, A_2) = A_1^2 - 4A_0A_2$。在其他字中，我们有
$$
\mathrm{dis}_2(a_0X^2 + a_1X + a_2) = a_1^2 - 4a_0a_2 .
$$

#### 例 4 {#alg-iv-s6-n7-exa-4 .statement tag=06FN}

考虑多项式
$$
F = A_0X^3 + 3A_1X^2 + 3A_2X + A,
$$
系数为 $Q[A_0, A_1, A_2, A_3]$。我们有
$$
DF = 3(A_0X^2 + 2A_1X + A_2) ,
$$
$$
F - 1/3X \cdot DF = A_1X^2 + 2A_2X + A_3 .
$$
通过公式 (54) (IV, p. 84) 和 (29) (IV, p. 77) 我们有
$$
A_0 \cdot \mathrm{dis}_3(F) = - \mathrm{res}_{2,3}(DF, F) = - \mathrm{res}_{2,3}(DF, F - 1/3X \cdot DF)
$$
应用科。 IV的2，p. 80我们最终得到
$$
\mathrm{dis}_3(F) = - 27 \mathrm{res}_{2,2}(A_0X^2 + 2A_1X + A_2,\ A_1X^2 + 2A_2X + A_3) .
$$
通过 IV 的例 3，p. 80，我们有
$$
\tilde{\Delta}(A_0, 3A_1, 3A_2, A_3) = - 27 (A_0A_3 - A_1A_2)^2 - 108 (A_1A_3 - A_2^2)(A_1^2 - A_0A_2) .
$$
我们发现之后一些计算，如果$f = a_0X^3 + a_1X^2 + a_2X + a_3$，我们有
$$
\mathrm{dis}_3(f) = a_1^2a_2^2 + 18a_0a_1a_2a_3 - 4a_1^3a_3 - 4a_0a_2^3 - 27a_0^2a_3^2 .
$$
特别是，我们有
$$
\mathrm{dis}(X^3 + pX + q) = - (4p^3 + 27q^2) .
$$

习题

### 习题{#alg-iv-s6-exercises}

§ 6](exercises/s6/)参见[习题。
