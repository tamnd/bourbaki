---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 3
section_title: Representations
lang: zh
source: lie-i-iii
book_pages: 25-38, 85-91
pdf_pages: 0043-0056, 0103-0109
extraction: ocr
subsections:
    - "no": 1
      title: REPRESENTATIONS
      page: 25
      pdf_page: 43
    - "no": 2
      title: TENSOR PRODUCT OF REPRESENTATIONS
      page: 28
      pdf_page: 46
    - "no": 3
      title: REPRESENTATIONS ON HOMOMORPHISM MODULES
      page: 29
      pdf_page: 47
    - "no": 4
      title: EXAMPLES
      page: 31
      pdf_page: 49
    - "no": 5
      title: INVARIANT ELEMENTS
      page: 32
      pdf_page: 50
    - "no": 6
      title: INVARIANT BILINEAR FORMS
      page: 33
      pdf_page: 51
    - "no": 7
      title: CASIMIR ELEMENT
      page: 35
      pdf_page: 53
    - "no": 8
      title: EXTENSION OF THE BASE RING
      page: 36
      pdf_page: 54
statements: 24
exercises: 12
content_sha256: 0eb90d55caca6e180e1e803cd82574a5b06ccdeaac0dd6661a76263b83fa854b
translated_from: content/en/lie/I/03_s3_representations.md
translation_method: google
source_content_sha256: a021ec46ba121f306f571608589128b59fe9512dee7105b93f2d9f49b1ae24bd
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 788dfc3ecde3637e35c06042c5cc287a9739c47b77af638ac0c40533d8cfba51
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 3。 表示

### 1. REPRESENTATIONS

#### 定义 1 {#lie-i-s3-def-1 .statement tag=09VS}

*令$g$为李代数超过$K$且$M$为$K$模。 $g$的同态进入李代数$gl(M)$在模$M$上称为$g$的表示。单射表示称为忠实的。如果$K$是域，$M$超过$K$的维数（有限或无限）被称为表示的维数。 $K$模$g$上$g$的表示$x \mapsto \operatorname{ad} x$称为$g$的伴随表示。*

因此，$M$上$g$的表示是$g$的$K$线性映射$\rho$到自同态模的$M$，使得

$$
\rho([x, y]) \cdot m = \rho(x) \rho(y) \cdot m - \rho(y) \rho(x) \cdot m
$$

对于所有$x \in g, y \in g, m \in M$。

#### 例 {#lie-i-s3-n1-exa-1 .statement tag=09VT}

设 G 为实李群，g 为李代数，θ 为 G 在有限维实数向量空间 E 上的解析表示。那么 g 的相应的同态到 gl(E) 中就是 g 在 E 上的表示。*

令 U 为 g 的包络代数。 M 上 g 的表示集合和 M 上 U 的表示集合之间的§ 2, no. 1 定义命题 1 是一对一的对应。 另一方面，我们知道 (代数, 章) VIII, § 13, no. 1) 关联性代数 U 与左 U 模的表示的概念之间存在等价。

#### 定义 2 {#lie-i-s3-def-2 .statement tag=09VU}

*设 g 为 K 上的李代数，U 为它的包络线代数。 U 上的酉左模称为左 g 模，或简称为 g 模。*

如果 M 是 g 模且 x ∈ U，则 x_M 将表示由 x (cf. 代数, 章 VIII, § 1, no. 2) 定义的 M 的位似。

U 上的酉右模称为右 g 模。这样的模用左U^0模来标识，即(§ 2, no. 4)用左g^0模来标识。

令 φ 为 U 的主要反自同构。如果 M 是右 g 模，则通过对 m ∈ M 和 a ∈ U 写出 a.m = m.φ(a) 来在 M 上定义左 g 模结构。

概念和模的理论结果可以翻译成表示的语言：

(1) 如果 g 模 M 和 M' 同构的，则 M 和 M' 上 g 的两个表示 ρ 和 ρ' 被称为“相似”或“同构的”。为此，存在 K-模 M 的同构 u 到 K-模 M' 是必要且充分的，使得

$$
\rho'(x) = u \circ \rho(x) \circ u^{-1}
$$

对于所有 x ∈ g。

(2) 对于所有 i ∈ I，令 ρ_i 为 M_i 上 g 的表示。令 M 为 g 模 M_i 的 g 模直和。 M 上存在 g 的相应的表示 ρ，称为 ρ_i 的 *直和*，并用 $\sum_{i \in I} \rho_i$ 表示（或在 n 表示 $\rho_1, \ldots, \rho_n$ 的情况下用 $\rho_1 + \cdots + \rho_n$ 表示）。如果 $m = (m_i)_{i \in I}$ 是 M 的元素且 x ∈ g，则 $\rho(x).m = (\rho_i(x).m_i)_{i \in I}$。

(3) 如果相关的 g 模很简单，则 M 上 g 的表示 ρ 称为“简单”或“不可约”。这相当于说在所有$\rho(x), x \in g$下不存在稳定的M（除了{0}和M）的子K模。简单 g 模的类 (代数, 章 VIII, § 3, no. 2) 定义 g* 的简单表示的 *类。

(4) 如果相关的 g 模为半单，则 M 上 g 的表示 ρ 称为 *半单* 或 *完全可约化*。这相当于说 ρ 类似于简单表示的直和或者每个子 K 模

M 在$\rho(x)$ ($x \in g$) 下稳定，在$\rho(x)$ ($x \in g$) 下稳定补充 (cf. *代数*, 章 VIII, § 3, no. 3)。

(5) 令$\delta$为$g$相应的的简单表示到简单$g$模块的类C的类。另一方面，令$\rho$为M上$g$的表示。$g$模M的类C的同型组件$M_C$（*代数*，章VIII, § 3, no. 4）也称为* 类* $\delta$ 的 M 的同型成分。该组件是 $\rho(x)$ 下稳定的 M 子 K 模块中的和，其上有类 $\delta$ 的 $\rho(x)$ 诱导表示；它是其中某些子模中的直和；如果$M_C$是长度$n$，则$\rho$被称为*包含*$\delta$*n次*。不同$M_C$的和是直接的；当且仅当$\rho$是半单时，它才等于M。

(6) 设$\rho, \rho'$为$g$之二表示。如果$\rho'$的模是$\rho$的模的子模（或商模），$\rho'$被称为$\rho$的*子表示*（或表示*）。

令 M 为 K-模。 M 上的定义上的 $g$ 的零表示 $g$ 模块结构。这样结构 M 就被称为*平凡* $g$ 模块。

设 M 为 $g$ 模。 M 的子$g$模的商$g$模也是M的商模的子$g$模：它们是通过考虑M的两个子$g$模U、$U'$使得$U \supset U'$并形成$g$模而获得的$U/U'$。那么，如果上述型的所有单模同构于给定的简单$g$模块N，则M称为类* N的*纯*$g$模块*。如果$\rho$和$\sigma$是表示 $g$相应的对于M和N，我们也说$\rho$是类*$\sigma$的*纯。

设$M'$是M的子$g$模。对于M是类N的纯模，$M'$和$M/M'$是类N的纯模是充分必要的。对于条件显然是必要的。假设它成立并令U，$U'$是M的子$g$模，使得$U' \subset U$和$U/U'$是简单的；设$\phi$是M的典范同态到$M/M'$；如果$\phi(U) \neq \phi(U')$，$U/U'$是同构到$\phi(U)/\phi(U')$，因此与N同构；如果$\phi(U) = \phi(U')$，则$U \subset U' + M'$，因此$U/U'$同构于$(U' + M')/U'$的简单子模，而后者模本身同构于$M'/(U' \cap M')$；因此 $U/U'$ 再次同构于 N，因此 M 是类 N 的纯元素。

从此以后，让M是一个$g$模块，并假设M的子$g$模块中的集合是纯粹的类N，承认极大元素$M'$。那么纯类 N 的M 的每一个子模 $M''$ 都包含在$M'$ 中。因为 $M''/(M' \cap M'')$ 和 $M'$ 是类 N 的纯原子，因此根据上述，$M' + M''$ 是类 N 的纯原子，因此 $M' + M'' \subset M'$。

假设 $g$-模 M 承认 Jordan-Hölder 级数 $(M_i)_{0 \leq i \leq n}$。为了使 M 是类 N 的纯元素，$M_0/M_1, M_1/M_2, \ldots, M_{n-1}/M_n$ 与 N 同构是充分必要的；因为条件显然是必要的，从我们上面看到的来看，它的充分性紧随 $n$ 上的归纳。

#### 命题 1 {#lie-i-s3-prop-1 .statement tag=09VV}

*设 g 为 K 上的李代数，且 a 为 g 的理想值。设 M 为 g 模块*，$N$ 为简单的 $a$ 模块。将$M$视为$a$模块，并假设$M$的子$a$模块中的集合是纯类$N$承认极大元素$M'$。那么$M'$是$M$的子$g$模块。

让$y \in g$。令$\phi$为$M$的典范映射到$M/M'$，并将$M'$的$f$映射$m \mapsto \phi(y_M \cdot m)$到$M/M'$。只要证明$f(M') = \{0\}$就足够了。让$x \in a$。那么，对于$m \in M$，

$$
x_{M/M'} \cdot f(m) = \phi(x_M y_M \cdot m) = \phi(y_M x_M \cdot m) + \phi([x, y]_M \cdot m).
$$

现在$[x, y] \in a$，从而$\phi([x, y]_M \cdot m) = 0$；另一方面，

$$
\phi(y_M x_M \cdot m) = f(x_M \cdot m).
$$

因此$x_{M/M'} \cdot f(m) = f(x_M \cdot m)$。由此可见，$f(M')$是$M/M'$的子$a$模，与$M'$的商同构，因此是类$N$的纯模；因此$f(M') = \{0\}$。

#### 推论{#lie-i-s3-n1-cor-1 .statement tag=09VW}

*令 $g$ 为李代数超过 $K$，并且 $a$ 为 $g$ 的理想值。令 $M$ 为简单的 $g$ 模块，有限长度为 $K$ 模块。存在一个简单的$a$-模块$N$，使得$M$是类$N$的纯$a$-模块。*

由于$a$模块$M$属于有限长度，因此$M$的子$a$模块的集合中存在最小元素$N$：它是$M$的简单子$a$模块。 The largest sub-$a$-module of $M$ which is pure of species $N$ is therefore $\neq \{0\}$ and is a sub-$g$-module of $M$ (Proposition 1) and is therefore identical with $M$.

### 2. 张量积表示

我们在no. 1直和中定义了$g$的表示族。我们现在将定义其他运算放在表示上。

令$g_1, g_2$是$K$上的两个李代数，并且$M_i$是一个$g_i$模（$i = 1, 2$）。令$U_i$为$g_i$的代数和$g_i$的$\sigma_i$典范映射到$U_i$的包络。那么 $M_i$ 是左 $U_i$ 模块，因此 $M_1 \otimes_K M_2$ 具有规范的左 $(U_1 \otimes_K U_2)$ 模块结构。现在$U_1 \otimes_K U_2$是$g_1 \times g_2$的包络代数，映射$(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)$是$g_1 \times g_2$的典范映射进入这个包络代数（§ 2, no. 2）。因此，$M = M_1 \otimes_K M_2$上存在一个$(g_1 \times g_2)$模块结构，使得：

$$
\begin{align*}
(1) \quad (x_1, x_2)_M \cdot (m_1 \otimes m_2) &= (\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot (m_1 \otimes m_2) \\
&= ((x_1)_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes ((x_2)_{M_2} \cdot m_2).
\end{align*}
$$

$M$$g_1 \times g_2$的结构定义表示。

如果现在将$g$的$g_1 = g_2 = g$、同态$x \mapsto (x, x)$放入$g \times g$，由上述$M$上的$g$的表示、定义表示组成，因此是$g$模块$M$ 上的结构使得：

$$
(2) \quad x_M \cdot (m_1 \otimes m_2) = (x_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes (x_{M_2} \cdot m_2).
$$

通过类似的论证，我们看到：

#### 命题 2 {#lie-i-s3-prop-2 .statement tag=09VX}

令$g$是李代数超过$K$和$M_i$一个$g$模（$1 \leq i \leq n$）。在张量积 $M_1 \otimes_K M_2 \otimes \cdots \otimes M_n$ 上，存在且仅有一个 $g$ 模块结构，使得

$$
x_M \cdot (m_1 \otimes \cdots \otimes m_m) = \sum_{t=1}^n m_1 \otimes \cdots \otimes (x_{M_t} \cdot m_i) \otimes \cdots \otimes m_n
$$

对于所有$x \in g, m_1 \in M_1, \ldots, m_n \in M_n$。

相应的表示称为$M_i$ 上$g$ 的给定表示的*张量积*。

特别是，如果$M$是一个$g$模块，则命题2定义在每个$M_p = \bigotimes^p M$上有一个$g$模块结构，因此在$M$的张量代数$T$上。

公式 (3) 表明，对于所有 $x \in g, x_T$ 来说，代数 $T$ 扩展 $x_M$ 都是唯一的 *推导*。我们知道（§ 2, no. 8）经过上的$x_T$定义除以$M$的对称代数$S$的商推导。因此，$S$可以被视为$T$的商$g$模，而$x_S$是$S$的推导。

更具体地，通过$g$的伴随表示将$g$视为$g$模。令$U$为$g$的包络代数。通过 § 2 的命题 7，经过上的 $x_M$ 定义到 $U$ 的商推导，即由 $\sigma(x)$ 定义的内部推导（$\sigma$ 表示$g$ 的典范映射变为 $U$）。那么$U$可以被认为是$T$的商$g$模。如果$K$是特征0的域，则$S$到$U$的典范同构是$g$模同构（§ 2, no. 8）。

### 3. 表示同态模

再次让$g_1$和$g_2$是李代数超过$K$和$M_i$一个$g_i$模（$i = 1, 2$）。令$U_i$为$g_i$的代数和$g_i$的$\sigma_i$典范映射到$U_i$的包络。那么 $M_i$ 是左 $U_i$ 模块，因此 $\mathscr{L}_K(M_1, M_2)$ 具有规范的左 $(U_1^0 \otimes U_2)$ 模块结构。现在$U_1^0 \otimes_K U_2$是$g_1^0 \times g_2$和映射的包络代数

$$
(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)
$$

是典范映射的 $g_1^0 \times g_2$ 到这个包络线代数中。因此，$M = \mathscr{L}_K(M_1, M_2)$上存在一个$(g_1^0 \times g_2)$模块结构，使得

$$
((x_1, x_2)_M \cdot u) \cdot m_1 = ((\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot u) \cdot m_1 \\
= u((x_1)_{M_1} \cdot m_1) + (x_2)_{M_2} \cdot u(m_1)
$$

对于所有$u \in \mathscr{L}_K(M_1, M_2), m_1 \in M_1$。 $M$ $g_1^0 \times g_2$ 的结构定义表示。

如果现在将$g$的$g_1 = g_2 = g$、同态$x \mapsto (-x, x)$放入$g^0 \times g$，由上述$M$上的$g$的表示、定义表示组成，因此是$g$模块$M$ 上的结构使得

$$
(x_M \cdot u) \cdot m_1 = x_{M_2} \cdot u(m_1) - u(x_{M_1} \cdot m_1)
$$

或

$$
x_M \cdot u = x_{M_2} u - u x_{M_1}.
$$

将这些结果与命题 2 结合起来，我们可以看到：

#### 命题 3 {#lie-i-s3-prop-3 .statement tag=09VY}

*设$g$是李代数超过$K$和$M_i$一个$g$模（$1 \leq i \leq n + 1$）。令$N$为$\prod_{i=1}^n M_i$到$M_{n+1}$的多线性映射的$K$模$\mathscr{L}_K(M_1, \ldots, M_n; M_{n+1})$。 $N$ 上存在且仅有一个 $g$ 模块结构，使得*

$$
(x_N \cdot u)(m_1, \ldots, m_n) = - \sum_{i=1}^n u(m_1, \ldots, x_{M_i} \cdot m_i, \ldots, m_n)
$$
$$
+ x_{M_{n+1}} \cdot u(m_1, \ldots, m_n)
$$

*对于所有* $x \in g, u \in N$ *和* $m_i \in M_i$ ($1 \leq i \leq n$)。

特别是，让$g$比$K$和$M$是$g$模块的李代数，并将$K$视为平凡的$g$模块。 命题 3 定义 $\mathscr{L}_K(M, K) = M^*$ 上的 $g$ 模块结构。 相应的表示被称为表示$x \mapsto x_M$的*对偶的*表示。我们有：

$$
(x_{M^*} \cdot f)(m) = -f(x_M \cdot m)
$$

对于所有$x \in g, f \in M^*, m \in M$。在其他字中：

$$
x_{M^*} = -{}^t x_M.
$$

当$K$为域且$M$为有限维时，$g$-模$M$是简单的（或半单）当且仅当$g$-模$M^*$是简单的（或半单）。

#### 命题 4 {#lie-i-s3-prop-4 .statement tag=09VZ}

*令$M_1, M_2$为两个$g$模块。典范的 $K$ 线性映射*（代数、章 II, § 4, no. 2、命题 2 和 no. 1、命题 1）：

$$
M_1^* \otimes_K M_2 \xrightarrow{\phi} \mathscr{L}_K(M_1, M_2), \quad \mathscr{L}_K(M_1, M_2^*) \xrightarrow{\psi} (M_1 \otimes_K M_2)^*
$$

*（其中第二个是双射）* 是$g$-模块同态。

我们写

$$
N = M_1^* \otimes M_2, \quad P = \mathscr{L}(M_1, M_2), \quad Q = \mathscr{L}(M_1, M_2^*), \quad R = (M_1 \otimes M_2)^*.
$$

那么，对于$x \in g, f \in M_1^*, m_1 \in M_1, m_2 \in M_2$，

$$
((\phi x_N)(f \otimes m_2)) \cdot m_1 = (\phi(x_{M_1^*} f \otimes m_2 + f \otimes x_{M_2} m_2)) \cdot m_1 \\
= \langle x_{M_1^*} f, m_1 \rangle m_2 + \langle f, m_1 \rangle x_{M_2} m_2
$$

$$
((x_P \phi)(f \otimes m_2)) \cdot m_1 = x_{M_2}(\phi(f \otimes m_2) \cdot m_1) - \phi(f \otimes m_2)(x_{M_1} m_1) \\
= \langle f, m_1 \rangle x_{M_2} m_2 - \langle f, x_{M_1} m_1 \rangle m_2
$$

因此$\phi x_N = x_P \phi$。另一方面，对于$x \in g, u \in \mathscr{L}(M_1, M_2^*), m_1 \in M_1, m_2 \in M_2$：

$$
(\psi x_Q u)(m_1 \otimes m_2) = \langle (x_Q u) \cdot m_1, m_2 \rangle = \langle x_{M_2^*} u m_1 - u x_{M_1} m_1, m_2 \rangle \\
(x_R \psi u)(m_1 \otimes m_2) = -\langle \psi u, x_{M_1} m_1 \otimes m_2 + m_1 \otimes x_{M_2} m_2 \rangle \\
= -\langle u x_{M_1} m_1, m_2 \rangle - \langle u m_1, x_{M_2} m_2 \rangle
$$

因此$\psi x_Q = x_R \psi$，它完成了证明。

$g$-模块$\mathscr{L}(M_1, M_2^*)$和$(M_1 \otimes M_2)^*$在同构$\psi$下标识。如果$M_1$和$M_2$有有限的基，则$\phi$是同构（代数，章II, § 4, no. 2，命题2），这允许我们对$g$模块进行认同 $M_1^* \otimes M_2$和$\mathscr{L}(M_1, M_2)$；在这种情况下，我们可以使用认同、$g$模块$M_1^* \otimes M_2^*, \mathscr{L}(M_1, M_2^*)$和$(M_1 \otimes M_2)^*$。

### 4. 例

#### 例 1 {#lie-i-s3-n4-exa-1 .statement tag=09W0}

令$g$为李代数超过$K$，并且$M$为$g$模。 $M$ 上的$g$-模块结构和$K$ 定义上的普通$g$-模块结构以及$M$ 上双线性形式的$K$-模块$N = \mathscr{L}(M, M; K)$ 上的$g$-模块结构。然后

$$
(x_N \cdot \beta)(m, m') = -\beta(x_M \cdot m, m') + \beta(m, x_M \cdot m')
$$

对于$M, \beta \in N$中的所有$x \in g, m, m'$。如果$\beta$是$N$的给定元素，$x \in g$的集合，则$x_N \cdot \beta = 0$是$g$的子代数。

令$M$为$K$模块，$\beta$双线性形式位于$M$上。由上可知，集合 / $x \in gl(M)$ 使得

$$
\beta(x \cdot m, m') + \beta(m, x \cdot m') = 0
$$

对于所有 $m \in M$ 和 $m' \in M$ 是 $gl(M)$ 的谎言子代数。假设 $K$ 是域，$M$ 是有限维的，$\beta$ 是非简并的。那么每个$x \in gl(M)$承认一个左伴随$x^*$（相对于$\beta$），它到处都有定义，并且所讨论的子代数是$x \in gl(M)$的集合，使得$x^* = -x$。通过这个过程我们可以得到构造和李代数两个重要的例：

(a) 取 $M = K^n$ 并

$$
\beta((\xi_1, \ldots, \xi_n), (\eta_1, \ldots, \eta_n)) = \xi_1 \eta_1 + \cdots + \xi_n \eta_n.
$$

我们典型地认同 $gl(K^n)$ 与 $M_n(K)$。那么得到的李代数就是斜对称矩阵的李代数。 *（当$K = \mathbf{R}$时，这个代数是正交群$O(n, \mathbf{R})$的李代数）。*

(b) 取 $M = K^{2m}$ 并且
$$
\beta((\xi_1, \ldots, \xi_{2m}), (\eta_1, \ldots, \eta_{2m})) = \xi_1 \eta_{m+1} - \eta_1 \xi_{m+1} + \cdots + \xi_m \eta_{2m} - \eta_m \xi_{2m}.
$$
$\beta$的矩阵相对于$K^{2m}$的典范基为矩阵
$$
\begin{pmatrix}
0 & I_m \\
-I_m & 0
\end{pmatrix}.
$$
令$U = \begin{pmatrix} A & B \\ C & D \end{pmatrix}$相对于$\mathrm{gl}(M)$的元素$u$$K^{2m}$典范基为矩阵（$A, B, C, D$位于$\mathbf{M}_m(K)$）。由*代数*的公式(50)、章IX, § 1, no. 10、$u^*$相对于同样的基矩阵有
$$
\begin{pmatrix}
0 & -I_m \\
I_m & 0
\end{pmatrix}
\begin{pmatrix}
tA & tC \\
tB & tD
\end{pmatrix}
\begin{pmatrix}
0 & I_m \\
-I_m & 0
\end{pmatrix}
= \begin{pmatrix}
tD & -tB \\
-tC & tA
\end{pmatrix}.
$$
因此，条件 $u^* = -u$ 相当于条件
$$
D = -tA \quad B = tB \quad C = tC.
$$
*当$K = \mathbf{R}$时，得到的李代数是辛群$\mathbf{Sp}(2m, \mathbf{R})$的李代数。*

#### 例 2 {#lie-i-s3-n4-exa-2 .statement tag=09W1}

我们保留 *例 1* 的记号。

$M$的自同态的$K$-模块$P = \mathscr{L}_K(M, M)$上的$g$-模块结构$M$定义上的$g$-模块结构。根据 (6)，对于所有 $x \in g$ 和 $u \in P$：
$$(11)$$
$$
x_P \cdot u = [x_M, u] = (\mathrm{ad}\, x_M) \cdot u
$$
其中$\mathrm{ad}\, x_M$表示在$\mathrm{gl}(M)$的伴随表示下的$x_M$的像。其他字：
$$(12)$$
$$
x_P = \mathrm{ad}\, x_M
$$
在$\mathscr{L}(\mathscr{L}(M, M)) = \mathscr{L}(\mathrm{gl}(M))$。

### 5. 不变量元素

#### 定义 3 {#lie-i-s3-def-3 .statement tag=09W2}

*令$g$为李代数，且$M$为$g$模。如果 $x_M \cdot m = 0$ 对于所有 $x \in g$，元素 $m \in M$ 被称为不变性（相对于 $M$ 上的 $g$ 模块结构或相对于 $g$ 的相应的表示）。*

*设$G$是连通的实李群，$g$是李代数，$\theta$是$G$在有限维实数向量空间$E$和$\rho$相应的上的解析表示 $E$ $g$ 的表示。让$m \in E$。 元素$m$相对于$\rho$不变，当且仅当$\theta(g) \cdot m = m$对于所有$g \in G$。这证明了使用字“不变”的合理性。*

#### 例 1 {#lie-i-s3-n5-exa-1 .statement tag=09W3}

令$M, N$为两个$g$模块和$P = \mathscr{L}_K(M, N)$。为了使$P$的元素$f$保持不变，根据(6)，$f$是$g$-模块$M$到$g$-模块$N$的同态是必要且充分的。特别是，如果$M = N$和$x_M = x_N$对于所有$x \in g$，当且仅当$f$可与$x_M$置换时，$f$是不变的。

#### 例 2 {#lie-i-s3-n5-exa-2 .statement tag=09W4}

设 M 为 K-模，且基有限。如果M具有g模结构，则$\mathscr{L}(M, M)$和$M^* \otimes M$具有g模结构，并且$M^* \otimes M$到$\mathscr{L}(M, M)$的典范映射是g模同构（命题4）。由于$1 \in \mathscr{L}(M, M)$显然是一个不变量（cf.例1），$M^* \otimes M$的相应的元素$u$是一个不变量。如果$(e_i)_{1 \leq i \leq n}$是M的基并且$(e_i^*)_{1 \leq i \leq n}$是对偶基，我们有$u = \sum_{i=1}^n e_i^* \otimes e_i$。

#### 例 3 {#lie-i-s3-n5-exa-3 .statement tag=09W5}

设 M 为 g 模。令 M 上的 $\beta$ 为双线性形式，并且 $\mathscr{L}(M, M^*)$ 的 f 相应的元素。为了使$\beta$保持不变，f是g模同态（命题4和例1）是充分必要的。假设 K 为域且 $\dim_K M < +\infty$。 g 模块 M 的 M 定义同构上的非简并不变双线性形式 $\beta$ 到 g 模块 $M^*$ 上，因此 g 模块 $M \otimes M$ 的同构到 g 模块 $M^* \otimes M$ 上。因此，通过例 2，在g-模$M \otimes M$中给$\beta$定义规范地一个不变量元素c，其可以构造如下：令$(e_i)_{1 \leq i \leq n}$为M的基且为M的$(e'_i)_{1 \leq i \leq n}$基，这样那个$\beta(e_i, e'_j) = \delta_{ij}$；然后$c = \sum_{i=1}^n e_i \otimes e'_i$。

#### 命题 5 {#lie-i-s3-prop-5 .statement tag=09W6}

*设g是谎言K-代数，h是g的理想，g在M上的$\rho$表示以及$\rho$到h的$\rho'$限制。那么M关于$\rho'$的不变量的元素的集合N在$\rho(g)$下是稳定的。*

设 $n \in N$ 和 $y \in g$；对于所有 $x \in h, [x, y] \in h$ 因此
$$
\rho(x)\rho(y)n = \rho([x, y])n + \rho(y)\rho(x)n = 0;
$$
因此$\rho(y)n \in N$。

#### 命题 6 {#lie-i-s3-prop-6 .statement tag=09W7}

*设 M 为半单 g 模。那么M的不变量元素的子模$M_0$承认唯一一个在$x_M$下稳定的补充，即由$x_M.m$（$x \in g, m \in M$）生成的子模$M_1$。

令$M'$为M的子模，它在M中$M_0$的$x_M$和补充下是稳定的。对于所有具有$m_0 \in M_0, m' \in M'$的$m \in M, m = m_0 + m'$，因此$x_M m = x_M m' \in M'$。因此$M_1 \subset M'$。设$M_2$为$M'$的子模，在$x_M$下稳定，并补充$M'$中的$M_1$。对于所有$m \in M_2$，
$$
x_M m \in M_2 \cap M_1 = \{0\}
$$
对于所有$x \in g$，因此$m \in M_0$，因此$m = 0$。因此$M_2 = \{0\}$，证明了$M_1 = M'$。

### 6. INVARIANT BILINEAR FORMS

令 g 为 K 上的李代数。 g 在 g 上的伴随表示和 g 在 K 上的零表示定义 K-模上的 g 模结构

$g$ 上的双线性形式 $N = \mathscr{L}(g, g; K)$。简而言之，如果表示$x \mapsto x_N$下不变，则$g$上的双线性形式$\beta$是“不变量”。根据公式 (10)，必要且充分的条件为：

$$
\beta([x, y], z) = \beta(x, [y, z])
$$

对于$g$中的所有$x, y, z$。

现在令$\mathfrak{d}$为$g$的推导的李代数。 The identity representation of $\mathfrak{d}$ and the zero representation of $\mathfrak{d}$ on $K$ define a representation $D \mapsto D_N$ of $\mathfrak{d}$ on $N$. 简而言之，如果表示$D \mapsto D_N$下不变，那么$g$上的双线性形式是*完全不变的*。 完全的不变双线性形式是不变的。 为了使$g$上的双线性形式$\beta$完全不变，有必要且充分：

$$
\beta(Dx, y) + \beta(x, Dy) = 0
$$

对于$g$和$D \in \mathfrak{d}$中的所有$x, y$。

#### 命题 7 {#lie-i-s3-prop-7 .statement tag=09W8}

*令$g$为李代数，$\beta$为$g$上的不变对称双线性形式，而$a$为$g$的理想。*

(a) *$a$相对于$\beta$正交的$a'$是$g$的理想。*
(b) *如果 $a$ 是特征性且 $\beta$ 完全不变，则 $a'$ 是特征性。*
(c) *如果 $\beta$ 是非简并的，$a \cap a'$ 是可交换的。*

设$D$为$g$的推导。假设 $a$ 在 $D$ 下稳定，并且 $\beta(Dx, y) + \beta(x, Dy) = 0$ 在 $g$ 下稳定于 $x, y$。那么$z \in a'$意味着$Dz \in a'$，因为对于所有$t \in a$、$Dt \in a$，因此$\beta(Dz, t) = -\beta(z, Dt) = 0$。因此$a'$在$D$下是稳定的。这就建立了(a)和(b)。

现在令$b$为$g$的理想，并假设$\beta$到$b$中的限制为零。对于$b$和$z \in g$中的$x, y$，$\beta([x, y], z) = \beta(x, [y, z]) = 0$，对于$[y, z] \in b$。因此$[b, b]$与$g$正交。如果 $\beta$ 是非简并的，则 $b$ 是可交换的。这个结果应用于$a \cap a'$证明了(c)。

#### 定义 4 {#lie-i-s3-def-4 .statement tag=09W9}

*令$g$为李$K$代数，$M$为$g$模。假设 $M$ 被视为 $K$ 模，承认有限的基。与$g$模块$M$（或与相应的表示）相关联的双线性形式是$g$上的对称双线性形式$(x, y) \mapsto \operatorname{Tr}(x_M y_M)$。如果所讨论的表示是伴随表示，则相关的双线性形式称为$g$的杀戮形式。*

#### 命题 8 {#lie-i-s3-prop-8 .statement tag=09WA}

*令$g$为李代数，且$M$为$g$模块。假设 $M$ 被视为 $K$ 模，承认有限的基。与 $M$ 相关的双线性形式是不变的。*

对于$g$中的$x, y, z$，我们有：

$$
\begin{align*}
\operatorname{Tr}([x, y]_M z_M) &= \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(y_M x_M z_M) = \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(x_M z_M y_M) \\
&= \operatorname{Tr}(x_M [y, z]_M).
\end{align*}
$$

#### 命题 9 {#lie-i-s3-prop-9 .statement tag=09WB}

*假设 $K$ 是域并且李代数 $g$ 是超过 $K$ 的有限维*。 *令$a$为$g$的理想，$\beta$为$g$的杀戮形式，以及$\beta'$为$a$的杀戮形式。那么$\beta'$就是$\beta$到$a$的限制。

令 $u$ 为向量空间 $g$ 的自同态，这使得 $a$ 保持稳定。设$v$为$u$到$a$的限制，以及当经过为商时从$u$导出的向量空间$g/a$的$w$自同态。然后$\operatorname{Tr} u = \operatorname{Tr} v + \operatorname{Tr} w$，如通过取$g$的基$(x_1, \ldots, x_n)$所示，其中第一个$p$元素形式基$a$。然后让$x \in a, y \in a$并将上面的公式应用到$u = (\operatorname{ad}_g x)(\operatorname{ad}_g y)$的情况。然后是$v = (\operatorname{ad}_a x)(\operatorname{ad}_a y)$和$w = 0$。因此$\beta(x, y) = \beta'(x, y)$。

#### 命题 10 {#lie-i-s3-prop-10 .statement tag=09WC}

*假设$K$是域并且李代数$g$是$K$上的有限维。 $g$的杀戮形式$\beta$是完全不变的。*

令 $D$ 为 $g$ 中的推导。存在李代数 $g'$ 包含 $g$ 作为余维 1 的理想和 $g'$ 的元素 $x_0$，使得 $Dx = [x_0, x]$ 对于所有 $x \in g$ (§ 1, no. 8， 例 1)。令$\beta'$为$g'$的杀戮形式。对于$g$、$\beta'([x, x_0], y) = \beta'(x, [x_0, y])$中的$x, y$，即$\beta'(Dx, y) + \beta'(x, Dy) = 0$。现在$\beta'$到$g$的限制是$\beta$（命题9）。因此命题。

### 7. 卡西米尔元素

#### 命题 11 {#lie-i-s3-prop-11 .statement tag=09WD}

*设$g$为域$K$之上的李代数，$U$其包络代数，$h$为$g$和$\beta$不变双线性形式的有限维理想$g$，其限制到$h$是非简并的。令$(e_i)_{1 \leq i \leq n}, (e'_j)_{1 \leq j \leq n}$为$h$的两个基，使得$\beta(e_i, e'_j) = \delta_{ij}$。那么$U$属于的元素$c = \sum_{i=1}^n e_i e'_i$到$U$的中心并且独立于基$(e_i)$的选择。

对于$x \in g$，令$x_h$为$\operatorname{ad}_g x$的限制到$h$。 那么$x \mapsto x_h$是向量空间$h$上$g$的表示，并且$\beta$到$h$的限制$\beta'$在这个表示下是不变的。 通过no. 5、*例 3*，张量$\sum_{i=1}^n e_i \otimes e'_i$独立于基$(e_i)$的选择，并且是$h$的张量代数的不变量元素。 它也是张量代数 $T$ $g$ 的元素，对于源自$g$ 的伴随表示的表示是不变的。 因此，$U$中的典范像，即$c$，独立于基$(e_i)$的选择，并且是no. 2末尾考虑的$U$上$g$的表示的不变量。 因此，这个元素可以与$g$的每一个元素进行置换，因此可以对$U$的属于到中心进行置换。

当$\beta$是双线性形式与$g$-模块$M$相关联时，命题11的元素$c$被称为与$M$（或与相应的）相关联的*卡西米尔元素* 表示）。如果$\beta$到$h$的限制是非简并的，则元素存在。

#### 命题 12 {#lie-i-s3-prop-12 .statement tag=09WE}

*令 $g$ 为域 $K$ 上的李代数，$h$ 有限维 n 的 $g$ 的理想以及有限维的 M g 模在 K 上。令 c 为与 M 和 h 相关的卡西米尔元素（假定存在）。

（一）$\operatorname{Tr}(c_M) = n$。
(b) *如果M是简单的并且n不能被K的特征整除，则$c_M$是M*的自同构。

在命题11的记号中，

$$
\operatorname{Tr}(c_M) = \sum_{i=1}^n \operatorname{Tr}((e_i)_M(e'_i)_M) = \sum_{i=1}^n \beta(e_i, e'_i) = n.
$$

因此，如果 n 不能被 K 的特征整除，则$c_M \neq 0$。另一方面，由于 U 的 c 属于到中心，$c_M$ 可以与所有 $x_M, x \in g$ 置换。如果进一步 M 是简单的，则 $c_M$ 因此在 $\mathscr{L}(M)$ 中是可逆的 (*代数*, 章 VIII, § 4, no. 3, 命题 2)。

### 8. 扩张基环

设$K_1$为交换环，K的单位元和$\phi$同态变为$K_1$映射1比1。设g为谎言K-代数，U为其包络代数，M为左g模，即左U 型模块。那么$M_{(K_1)}$有一个规范的左$U_{(K_1)}$模块结构，因此有一个左$g_{(K_1)}$模块结构。设$\rho$和$\rho_{(K_1)}$为g的表示，$g_{(K_1)}$相应的为M和$M_{(K_1)}$：$\rho_{(K_1)}$据说是通过*扩展基环*从$\rho$导出的，结果为*代数*、章VIII, § 13, no. 4均可适用。如果$x \in g$，$\rho_{(K_1)}(x)$只是自同态$\rho(x) \otimes 1$ / $M_{(K_1)} = M \otimes_K K_1$。

假设 K 是域，$K_1$ 是 K 的扩张，$\phi$ 是 K 的典范嵌入到 $K_1$。令V和V'为M的向量子空间。令a为$x \in g$的g由……组成的向量子空间，使得$\rho(x)(V) \subset V'$。令$a'$为$x' \in g_{(K_1)}$的$g_{(K_1)}$由……组成之向量子空间，使得$\rho_{(K_1)}(x')(V_{(K_1)}) \subset V'_{(K_1)}$。然后$a' = a_{(K_1)}$。显然是$a_{(K_1)} \subset a'$。现在让$x' \in a'$。我们可以写成$x' = \sum_{i=1}^n \lambda_i x_i$，其中$x_i$在g中，$\lambda_i$是$K_1$的元素，与K线性无关。对于所有$u \in V$，$\rho(x') \cdot u \in V'_{(K_1)}$，即$\sum_{i=1}^n \lambda_i \rho(x_i) \cdot u \in V'_{(K_1)}$，从而$\rho(x_i) \cdot u \in V'$，因此$x_i \in a$和$x' \in a_{(K_1)}$。这表明$a' = a_{(K_1)}$。特别地，$g_{(K_1)}$的*中心*是通过将K扩展到$K_1$而从g的中心导出的：将以上应用于g的伴随表示就足够了。由此可见，对于所有$p$，$\mathscr{C}_p(g_{(K_1)}) = (\mathscr{C}_p g)_{(K_1)}$。类似地，令 h 为 g 的子代数，n 为 g 中 h 的*归一化器*。那么$g_{(K_1)}$中$h_{(K_1)}$的归一化器就是$n_{(K_1)}$。

设 K、$K_1$、g、$\rho$、M 如上一段所示。令 b 为 g 的向量子空间，W 向量子空间为 M。令 V 为 $m \in M$ 的 M 由……组成的向量子空间，使得 $\rho(b) \cdot m \subset W$。令V'为$m' \in M_{(K_1)}$的$M_{(K_1)}$由……组成中的向量子空间，使得$\rho_{(K_1)}(b_{(K_1)}) \cdot m' \subset W_{(K_1)}$。如上所示，$V' = V_{(K_1)}$。特别是，$M_{(K_1)}$的*不变量*的向量子空间是通过将基域从$K$延伸到$K_1$而从$M$的不变量向量子空间导出的。

令 $K, K_1$ 和 $\phi$ 与此编号的开头相同。令 $g$ 为李$K$-代数，以及 $M$ 和 $N$ $g$-模。如果$M$和$N$是同构的$g$模块，则$M_{(K_1)}$和$N_{(K_1)}$是同构的$g_{(K_1)}$模块。反之：

#### 命题 13 {#lie-i-s3-prop-13 .statement tag=09WF}

*令$K$为$K$的域、$K_1$扩张、$g$一个李$K$代数和$M, N$$K$上有限维的两个$g$模。如果 $M_{(K_1)}$ 和 $N_{(K_1)}$ 是同构 $g_{(K_1)}$ 模块，则 $M$ 和 $N$ 是同构 $g$ 模块。*

证明分两步。

(1) 首先假设$K_1$是*有限次数*$n$的$K$的扩张。 令$U$为$g$的包络代数，使得$g_{(K_1)}$的包络代数为$U_{(K_1)} = U \otimes_K K_1$(§ 2, no. 9)。 由于 $M_{(K_1)}$ 和 $N_{(K_1)}$ 与 $U_{(K_1)}$ 模块同构，因此它们与 $U$ 模块同构 *更不必说*；但作为 $U$ 模块，它们分别与 $M^n$ 和 $N^n$ 同构的。 Now $M$ and $N$ are $U$-modules of finite length; $M$ (resp. $N$) is therefore the direct sum of a family $(P_i^{r_i})_{1 \leq i \leq p}$ (resp. $(Q_j^{s_j})_{1 \leq j \leq q}$) of submodules such that the $P_i$ (resp. $Q_j$) are indecomposable and two $P_i$ (resp. $Q_j$) of different indices are not isomorphic (*Algebra*, Chapter VIII, § 2, no. 2, Theorem 1). 那么$M^n$（分别$N^n$）同构于$P_i^{n r_i}$（分别$Q_j^{n s_j}$）的直和； (*loc.cit.*) $p = q$ 和之后在必要时置换 $Q_j$ $n r_i = n s_i$ 和 $P_i$ 同构于 $Q_i$ for $1 \leq i \leq p$，因此 $M$ 同构于 $N$。

(2) *一般情况。*设$P$为$P$的不变量的$g$模块$\mathscr{L}_K(M, N)$和$Q$子空间，即$g$模块$M$的同态的集合进入$g$-模块$N$。在$g_{(K_1)}$-模块$\mathscr{L}_{K_1}(M_{(K_1)}, N_{(K_1)}) = (\mathscr{L}_K(M, N))_{(K_1)}$中，不变量的子空间是$Q_{(K_1)}$。 $M_{(K_1)}$和$N_{(K_1)}$同构假设意味着$M$和$N$在$K$上具有相同的维数，并且存在于$Q_{(K_1)}$元素$g$，即$M_{(K_1)}$ 的同构到$N_{(K_1)}$。令$(f_1, \ldots, f_d)$为$Q$的基超过$K$，并且选择基为$M$和$N$超过$K$。如果 $\lambda_k \in K_1$ 对于 $1 \leq k \leq d$，$f = \sum_{k=1}^d \lambda_k f_k$ 的矩阵对于这些基具有行列式，该行列式是多项式 $D(\lambda_1, \ldots, \lambda_d)$，系数 *in* $K$。当 $f = g$ 时，该行列式不为零，因此 $D$ 的系数并非全部非零。因此，如果 $\Omega$ 是 $K$ 的代数闭包，则存在（因为 $\Omega$ 无限）元素 $\mu_k \in \Omega$ $(1 \leq k \leq d)$，使得 $D(\mu_1, \ldots, \mu_d) \neq 0$ (*代数*, 章 IV, § 2, no. 5、命题 8)。如果$K_2$是由$\mu_k$$(1 \leq k \leq d)$生成$K$的代数扩张，则$\sum_{k=1}^d \mu_k f_k$是$M_{(K_2)}$到$N_{(K_2)}$的同构；但$K_2$是有限次数超过$K$（*代数*，章V, § 3, no. 2，命题5），因此$M$和$N$与参数的第一个部分同构。

再次让$K, K_1$和$\phi$作为这个编号的开头。令 $\rho$ 为 $K$ 模块 $M$ 上 $g$ 的表示，且具有有限基 $(x_1, \ldots, x_n)$。然后，与 $\rho_{(K_1)}$ 相关联的 $g_{(K_1)}$ 上的双线性形式是从与 $\rho$ 相关联的双线性形式通过将基环扩展到 $K_1$ 导出的（因为，如果 $u \in \mathscr{L}_K(M)$，$u$ 具有相同的矩阵 ） $(x_1, \ldots, x_n)$ 与 $(x_1 \otimes 1, \ldots, x_n \otimes 1)$ 的$u \otimes 1$ 相同，因此 $u$ 和 $u \otimes 1$ 具有相同的轨迹）。特别是，如果$K$-模块$g$具有有限的基，则$g_{(K_1)}$的*杀死形式*是通过将基环延伸到$K_1$而从$g$的杀死形式*导出的。

### 习题 {#lie-i-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
