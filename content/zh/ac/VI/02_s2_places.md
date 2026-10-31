---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 2
section_title: Places
lang: zh
source: ac-i-vii
book_pages: 381-385, 444-446
pdf_pages: 0399-0403, 0462-0464
extraction: ocr
subsections:
    - "no": 1
      title: THE NOTION OF MORPHISM FOR LAWS OF COMPOSITION NOT EVERYWHERE DEFINED
      page: 381
      pdf_page: 399
    - "no": 2
      title: PLACES
      page: 381
      pdf_page: 399
    - "no": 3
      title: PLACES AND VALUATION RINGS
      page: 383
      pdf_page: 401
    - "no": 4
      title: EXTENSION OF PLACES
      page: 384
      pdf_page: 402
    - "no": 5
      title: CHARACTERIZATION OF INTEGRAL ELEMENTS BY MEANS OF PLACES
      page: 385
      pdf_page: 403
statements: 9
exercises: 6
content_sha256: d321ff5fe5073f57509ca06df45a494dc5c74f95f77911b16e14b76819c27a5f
translated_from: content/en/ac/VI/02_s2_places.md
translation_method: google
source_content_sha256: 53c302660c61cd7fef1b70be1d4b1ffa083e7229208dbbe2c386c3d702cdbacb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 764574dc574d23ce551dbc8841cb4afe0a172112c47cd45cf804d8678c27b1f5
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 2. 地点

### 1. 态射的概念对于合成的律并非到处都有定义

#### 定义 1 {#ac-vi-s2-def-1 .statement tag=04SN}

*令 E 和 E' 为两个集合，每个律为合成，用$(x, y) \mapsto x * y$表示，不一定在所有地方都定义。 映射 $f : E \to E'$ 是态射，如果对于 E 中的所有 $x, y$ 且定义了 $f(x) * f(y)$，也定义了合成 $x * y$ 并且：*

(1)
$$
f(x * y) = f(x) * f(y).
$$
更简单地说，我们可以说每当右侧有意义时，公式 (1) 都必须成立。

态射的概念与表示(*代数*, 章I, § 1, no. 1)不同，其中要求只要左边有意义，方程(1)就成立。当然，律和合成的两个概念重合到处都有定义。

#### 定义 2 {#ac-vi-s2-def-2 .statement tag=04SO}

*令 E 和 E' 为两个集合，每个律为合成 $(x, y) \mapsto x *_{\alpha} y, \alpha \in I$。如果对于合成 $(x, y) \mapsto x *_{\alpha} y$ 的每个律都是态射，映射 $f : E \to E'$ 就是态射。*

正如表示一样，*集合理论*的态射满足公理(MO_I)、(MO_{II})、(MO_{III})、章IV, § 2。如果：$E \to E'$是态射，$f(E)$是$\mathbf{R}'$的稳定子集。

### 2.地点

If K is a field, recall that $\mathbf{K}$ denotes the set the sum of K and an element denoted by $\infty$ (*Algebra*, Chapter 11, § 9, no. 9); the laws of composition of K extend to $\mathbf{K}$ by setting (*loc. cit.*)

(2)
$$
a + \infty = \infty \quad \text{for } a \in \mathbf{K}, \quad a \neq \infty,
$$
(3)
$$
\infty . a = a . \infty = \infty \quad \text{for } a \in \tilde{\mathbf{K}}, \quad a \neq 0.
$$

因此，唯一未定义的合成是合成至$+ \infty$、$\infty . 0$和$0 . \infty$。另一方面，映射$x \mapsto -x$和$x \mapsto x^{-1}$扩展类似于$\tilde{K}$设定$-\infty = \infty, 0^{-1} = \infty, \infty^{-1} = 0$。我们还要写$x + (-y) = x - y$。

集合$\tilde{K}$，称为与$K$相关的*射影域*，可以用*射影线*$P_1(K)$来识别（*loc.cit.*）。

#### 定义 3 {#ac-vi-s2-def-3 .statement tag=04SP}

*令$K$和$L$为两个域。每个态射*$f$*的*$K$*到*$\tilde{L}$*（对于加法和乘法）**这样*$f(1) = 1$*被称为*$K$*与值在*$L$的地方。

在其他字中，如果$x$和$y$是$K$和$f(x) + f(y)$（或$f(x)f(y)$）的元素，则定义$x + y$（或$xy$），并且

$$
f(x + y) = f(x) + f(y)
$$
$$
f(xy) = f(x)f(y).
$$

由于$\infty + \infty$没有定义，$f(\infty) + f(\infty)$也没有定义，这表明
$$
f(\infty) = \infty.
$$

类似地，由于$0 \cdot \infty$没有定义，$f(0)f(\infty)$也没有定义，根据(6)，这意味着
$$
f(0) = 0.
$$

另一方面
$$
f(a^{-1}) = f(a)^{-1} \quad \text{for all } a \in \tilde{K}.
$$

如果定义了$f(a)f(a^{-1})$，则定义了$aa^{-1}$，因此等于 1；然后$f(a)f(a^{-1}) = f(1) = 1$，在这种情况下证明了（8）。如果$f(a)f(a)^{-1}$未定义，则$f(a) = 0$和$f(a^{-1}) = \infty$或$f(a) = \infty$和$f(a^{-1}) = 0$以及(8)仍然成立。

类似地可以证明
$$
f(-a) = -f(a) \quad \text{for all } a \in K.
$$

从公式 (8) 和 (9) 可以得出，对于合成 $(x, y) \mapsto x - y$ 和 $(x, y) \mapsto xy^{-1}$ 的律，$f$ 也是态射。

对于$x \in \tilde{K}$，如果$f(x) \neq \infty$，则$f$在$x$称为有限；这意味着 (6) $x \in K$。

如果$f : K \to \tilde{L}$是一个地方，$f(K)$是$\tilde{L}$的子集，对于合成$(x, y) \mapsto x + y, (x, y) \mapsto x - y, (x, y) \mapsto xy$的律和$(x, y) \mapsto xy^{-1}$是稳定的，并且包含1。如果E是有限元素的集合 $f(\tilde{K})$，E是L和$f(\tilde{K}) = \tilde{E}$的子域。通过滥用语言 E 被称为“值域”。

两个地方的*复合* 映射就是一个地方。

令 F 为域 K 的同构到域 L 的子域；让我们通过设定$f(\infty) = \infty$从扩展$f$到$K$。因此，我们在 L 中获得了具有值的 K 位置，称为“平凡”，并且通常用同构 $f$ 来标识。

### 3.地点和估价环

#### 命题 1 {#ac-vi-s2-prop-1 .statement tag=04SQ}

令 K 为域，$\mathbf{A}$ K 的估值环，$\kappa(\mathbf{A})$ 剩余类域 $\mathbf{A}$。我们通过等式 $h_{\mathbf{A}}(x) = \infty$ if $x \notin \mathbf{A}$ 将 $\mathbf{A}$ 的扩展典范映射转移到 $\kappa(\mathbf{A})$ 到映射 $h_{\mathbf{A}} : \tilde{K} \to (\kappa(\mathbf{A}))$。由此定义的映射$h_{\mathbf{A}}$是K的一个位置，其值字段为$\kappa(\mathbf{A})$。

显然$h_{\mathbf{A}}(1) = 1$。

我们证明对于加法，$h_{\mathbf{A}}$ 是态射。令$x, y$为$\tilde{K}$的两个元素，从而定义$h_{\mathbf{A}}(x) + h_{\mathbf{A}}(y)$。两个元素$x, y$属于之一然后到$\mathbf{A}$，因此$x + y$被定义。如果$x \in \mathbf{A}$和$y \in \mathbf{A}$，显然

$$
h_{\mathbf{A}}(x) + h_{\mathbf{A}}(y) = h_{\mathbf{A}}(x + y)
$$

成立。如果$x \in \mathbf{A}$和$y \notin \mathbf{A}$，则$x + y \notin \mathbf{A}$和上面公式的两侧等于$\infty$。

我们最终证明对于乘法，$h_{\mathbf{A}}$ 是态射。令 $x \in K, y \in K$ 使得 $h_{\mathbf{A}}(x)h_{\mathbf{A}}(y)$ 被定义。如果$x \in \mathbf{A}$和$y \in \mathbf{A}$，则明确定义了$xy$和$h_{\mathbf{A}}(x)h_{\mathbf{A}}(y) = h_{\mathbf{A}}(xy)$。现在假设元素$x, y$之一，对于例$y$，不属于到$\mathbf{A}$；如$h_{\mathbf{A}}(y) = \infty$、$h_{\mathbf{A}}(x) \neq 0$，即$x \notin m(\mathbf{A})$、从而$x^{-1} \in \mathbf{A}$；由此可知 $xy$ 已定义，且 $xy \notin \mathbf{A}$、从而

$$
h_{\mathbf{A}}(xy) = \infty = h_{\mathbf{A}}(x)h_{\mathbf{A}}(y).
$$

这就证明了命题1。

如果$j$是$\kappa(\mathbf{A})$的同构到域L的子域，则$j \circ h_{\mathbf{A}} : \tilde{K} \to \tilde{L}$是L中K与值的位置。上述过程实际上提供了K上的所有位置。准确地说：

#### 命题 2 {#ac-vi-s2-prop-2 .statement tag=04SR}

令K和L为两个域，f为L中K与值的位置。那么存在对 K 的评估环 $\mathbf{A}$ 和对 L 的子域的同构 $j$ $\kappa(\mathbf{A})$ 的评估，使得 $f = j \circ h_{\mathbf{A}}$；这些条件确定 $\mathbf{A}$ 和 $j$ 是独一无二的。 环$\mathbf{A}$是$x \in K$的集合，使得$f(x) \neq \infty$和$m(\mathbf{A})$是$x \in K$的集合，使得$f(x) = 0$。

如果$f = j \circ h_{\mathbf{A}}$，条件$f(x) \neq \infty$（或$f(x) = 0$）相当于条件$h_{\mathbf{A}}(x) \neq \infty$（或$h_{\mathbf{A}}(x) = 0$），因此相当于条件$x \in \mathbf{A}$（或$x \in m(\mathbf{A})$）。因此 $\mathbf{A}$ 是唯一确定的，并且由于 $h_{\mathbf{A}}$ 是满射，$j$ 也是唯一的。

现在令$f$为K中L中任意有值的位置；让$\mathbf{A}$表示$x \in K$的集合，使得$f(x) \neq \infty$。如果定义了$x \in \mathbf{A}$和$y \in \mathbf{A}$、合成、$f(x) - f(y)$和$f(x)f(y)$以及$\neq \infty$，则表明$x - y \in \mathbf{A}$和$xy \in \mathbf{A}$；因此$\mathbf{A}$是K的子环。如果$x \notin \mathbf{A}$，则$f(x) = \infty$，因此通过限制获得同态$f'$的$f(x^{-1}) = 0$和$x^{-1}$属于到核$m$ $f$至$\mathbf{A}$。反之，如果$y \in m$，则$y^{-1} \notin \mathbf{A}$。这表明$\mathbf{A}$是K的评估环，而$m$是其最大理想。设 $j$ 为从 $\kappa(\mathbf{A})$ 到 L 的单同态，由 f' 除以经过的商得出。那么 $f(x) = j(h_A(x))$ 对于所有 $x \in A$ 来说，这个方程对于 $x \notin A$ 仍然成立，那么两侧就等于 $\infty$。

分解 $f = j \circ h_A$ 被称为placef 的规范分解。 $A$称为环关，$m(A)$是$f$和$\kappa(A)$剩余类域关的理想值。对于两个地方$f : \mathbf{K} \to \mathbf{L}$和$f' : \mathbf{K} \to \mathbf{L}'$具有相同的环，充分必要的是，存在值域中的同构，使得$f' = s \circ f$；那么$f$和$f'$称为等价。可以看出，每一个估价环的结果都可以转化为地点的结果，反之亦然；这就是我们在以下编号中要做的事情。

例地点
(1) 设$K$为域。 $K$上的恒等映射是一个平凡的地方，有环$K$和理想的$(0)$。
(2) 设$k$为域。对于所有$u \in k((T))^\sim$，如果$u \notin k[[T]]$，我们将$f(u) = \infty$和定义$f(u)$写为$u$的常数项，如果$u \in k[[T]]$。那么$f$是$k((T))$的位置，还有剩余类域$k$和环$k[[T]]$。对于$k[[T]]$，环为$k((T))$（§ 1, no. 4，例 3），限制为$f$至$k[[T]]$，其典范同态为$k[[T]]$确定在其剩余类域。
(3) 令$k$为域、$k$的$a$元素和$u \in k(X)$的$A$集合，使得$a$可在$u$中替换（代数， 章IV, § 3, no. 2）。如果$p$表示$k[X]$的素理想$(X - a)$，则$A = k[X]_p$，因此$A$是$k(X)$的估值环（§ 1, no. 4，命题2）。对于所有 $u \in k(X)^\sim$，如果 $u \notin A$，我们写 $f(u) = \infty$；如果 $u \in A$，我们写 $f(u) = u(a)$。那么$f$就是$k(X)$与剩余类域$k$和环$A$的位置； 限制前往 $A$ 的行程为 $A$ 的同态到核 $pA = m(A)$ 的$k$（代数、章 IV, § 3、命题 2）。据说元素$f(u) \in k$是通过将$X = a$放入$u$得到的。
\* (4) 设$S$为$S$上亚纯函数的维数1和$K$域的连通复解析簇。对于所有$z_0 \in S$，从$K$到$\mathbf{C}$的映射$f \mapsto f(z_0)$是$K$的一个地方，其环距离集合距$\in K$，它们在$z_0$是全纯的，其理想是集合 $\in K$ 零 $z_0$。正是这个例和其他类似物是项“地方”的起源。*

### 4. 扩张个地点

#### 命题 3 {#ac-vi-s2-prop-3 .statement tag=04SS}

令$K$为域、$K$的$S$子环以及从$S$到代数闭域$L$的$f$同态。那么$L$中存在$K$和值的位置，其中扩展$f$。

考虑到命题 1，这是§ 1, no. 2 定理 2 的翻译。

#### 命题 4 {#ac-vi-s2-prop-4 .statement tag=04ST}

令$K$为域，$f$为$K$，值位于域$L$，$K'$扩张为$K$。那么存在$L$的扩张$L'$和$K'$的位置$f'$，其中值位于$L'$，其中扩展$f$。如果$x_1, \ldots, x_n$是$K$的元素，并且在$K$和$a_1, \ldots, a_n$上代数独立，则可以选择任何元素$\in L$、$f'$，使得$f(x_i) = a_i$对于$1 \leq i \leq n.$

令$V$为环关闭，$g$限制关闭至$V$以及$g$至$V[x_1, \ldots, x_n]$的$g'$扩张，使得$g'(x_i) = a,$对于$1 \leq i \leq n.$就足够了$L'$为$L$和应用命题3的代数闭包到$g'$和$L'$：我们得到一个placef'：$K' \to \tilde{L}'$，其中扩展$g'$；如果$x \in K - V,$则$x^{-1} \in m(V),$从而$f(x^{-1}) = g(x^{-1}) = 0$和$f'(x) = \infty = f(x);$因此延伸。

### 5. 刻画积分元素通过位置

#### 命题 5 {#ac-vi-s2-prop-5 .statement tag=04SU}

令$K$为域，$K, h$同态中的$S$子环从$S$到域以及$h.$的$p$核对于元素 $K$的$x$在局部环$S,$上积分，$K$延伸$h$的每个位置在$x.$处是有限的是充分必要的

如果$f$是$K$延伸$h, f$的地方在$S_p$上是有限的，零在$pS_p$上是有限的，因此$f$地方的环占主导地位$S_p.$相反，如果$V$是一个评估环支配$S_p,$$V$的$K$是限制到$S$是同态的位置的环，并且核与$h;$替换$f$具有相同的位置，可以看出，$V$是$K$地方的环，其中扩展$h.$要说，$K$延伸$h$的每个地方在$x$处都是有限的，相当于说那个$x$ 属于到$K$的所有估值环，主导$S_p.$命题，然后从§ 1, no. 3的定理3开始。

#### 命题 6 {#ac-vi-s2-prop-6 .statement tag=04SV}

设$K$为域，$S$子环为$K.$，对于元素$x \in K$来说，要在$S,$上积分，$K$中在$S$上有限的每个位置在$x.$上是有限的，这是充分必要的

这也是§ 1, no. 3的定理3的推论。

### 习题{#ac-vi-s2-exercises}

§ 2](exercises/s2/)参见[习题。
