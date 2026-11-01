---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 1
section_title: Convolution
lang: zh
source: int-vii-ix
pdf_pages: 0101-0108, 0159-0159
extraction: ocr
subsections:
    - "no": 1
      title: Definition and examples
      page: 0
      pdf_page: 101
    - "no": 2
      title: Associativity
      page: 3
      pdf_page: 103
    - "no": 3
      title: The case of bounded measures
      page: 6
      pdf_page: 106
    - "no": 4
      title: Properties concerning supports
      page: 6
      pdf_page: 106
    - "no": 5
      title: Vectorial expression of the convolution product
      page: 7
      pdf_page: 107
statements: 13
exercises: 2
content_sha256: 37524fd945ed51adf2a01c7b17cbda22665f109e7f94bee5701cfc643b1efcfc
translated_from: content/en/int/VIII/01_s1_convolution.md
translation_method: google
source_content_sha256: cafcb1e20437900405f17cddf757448f37ab32581cc26e5e2a03bda1d34c2c66
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 34dbf3cd795775435f5f17a2d8911112d23702de64b98fbb83ea744ddd14a994
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。卷积

### 1.定义和例

回想一下（第 V, §6，第 1 和第 4 章；第 VI, §2, No. 10），如果 X 和 Y 局部紧致空间，$\mu$ X 上的测度，以及$\varphi$ 映射 X 到 Y 中， $\varphi$ 被认为是 $\mu$-适当的，如果： a) $\varphi$ 是 $\mu$-可测的； b) 对于 Y 的每个紧凑子集 K，$\varphi^{-1}(K)$ 本质上是 $\mu$ 可积。则 Y 上的像测度$\nu = \varphi(\mu)$存在，并具有以下性质：对于 Y 上的函数 f，与 Banach 空间或$\overline{\mathbf{R}}$ 中的值，对于 $\nu$ 本质上可积，$f \circ \varphi$ 是充分必要的所以对于$\mu$，在这种情况下，

$$
\int_Y f(y)\, d\nu(y) = \int_X f(\varphi(x)) d\mu(x).
$$

#### 定义 1 {#int-viii-s1-def-1 .statement tag=09I0}

*令$X_1, \ldots, X_n$局部紧致空间，$\mu_i$对$X_i$（$1 \leq i \leq n$）的测度；设X为$X_i$的乘积，$\mu$为$\mu_i$的乘积。令 $\varphi$ 为 X 的映射成为局部紧致空间 Y。有人说序列 $(\mu_i)$ 是 $\varphi$ 可卷积的，或者 $\mu_1, \ldots, \mu_n$ 是 $\varphi$ 可卷积的，如果 $\varphi$是$\mu$-正确的；在这种情况下，$\varphi$下$\mu$的像$\nu = \varphi(\mu)$称为$\mu_i$对$\varphi$的卷积乘积，并表示为$*_{\varphi}(\mu_i)_{1 \leq i \leq n}$，或$*_{i=1}^n \mu_i$，或$\mu_1 * \mu_2 * \cdots * \mu_n$。

当然，只有当$\varphi$毫无疑问时才使用最后两个记号。

设 f 为 Y 上的函数，值为 Banach 空间或 $\overline{\mathbf{R}}$。在阶中，f对于$\mu_1 * \cdots * \mu_n$本质上可积，函数是充分必要的

$$
(x_1, \ldots, x_n) \mapsto f(\varphi(x_1, \ldots, x_n))
$$

对于 $\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n$ 来说基本上是可积的，在这种情况下

$$
(1) \quad \int f\ d(\mu_1 * \cdots * \mu_n) = \int f(\varphi(x_1, \ldots, x_n)) d\mu_1(x_1) \ldots d\mu_n(x_n),
$$

当采用 $f \in \mathscr{K}(Y)$ 时，公式可以被视为*定义* $\mu_1 * \cdots * \mu_n$。

定义立即暗示$\mu_i$是可卷积的当且仅当$|\mu_i|$是可卷积的。当这种情况发生时，

$$
|\varphi(\mu_1 \otimes \cdots \otimes \mu_n)| \leq \varphi(|\mu_1 \otimes \cdots \otimes \mu_n|) = \varphi(|\mu_1| \otimes \cdots \otimes |\mu_n|)
$$
（第VI, §2, No. 10），即

$$
(2) \quad |*_i \mu_i| \leq *_i |\mu_i|.
$$

如果 $\mu_i$ 是可卷积的且为正数，并且如果 $\nu_i$ 是 $X_i$ 上的测度，使得 $0 \leq \nu_i \leq \mu_i$，则 $\nu_i$ 是可卷积的并且

$$
*_i \nu_i \leq *_i \mu_i.
$$

假设 $\mu_1, \mu_2, \ldots, \mu_n$ 是可卷积的，并且 $\mu'_1, \mu_2, \ldots, \mu_n$ 是可卷积的（$\mu'_1$ 是$X_1$ 上的度量）。由 Ch. V, §6, No. 3，科。命题 6 中的 1，$\mu_1 + \mu'_1, \mu_2, \ldots, \mu_n$ 是可卷积的并且

$$
(\mu_1 + \mu'_1) * \mu_2 * \cdots * \mu_n = \mu_1 * \mu_2 * \cdots * \mu_n + \mu'_1 * \mu_2 * \cdots * \mu_n.
$$

#### 例 {#int-viii-s1-n1-exa-1 .statement tag=09I1}

— 1) 对于任何$\varphi$，测量$\varepsilon_{x_i}$（其中$x_i \in X_i$代表$1 \leq i \leq n$）始终是可卷积的，并且具有与$y = \varphi(x_1, x_2, \ldots, x_n)$的卷积乘积$\varepsilon_y$。因而，如果每个$\mu_i$都有有限支撑，那么$\mu_i$是可卷积的，并且$\mu_1 * \cdots * \mu_n$有有限支撑。特别地，令 $M$ 为幺半群$^1$，配备局部紧致拓扑；如果在$M$中取$\varphi$为合成的律，则$M$与有限支撑形式的测量，对于卷积，代数正是幺半群的*代数* $M$（超过$\mathbf{R}$或超过$\mathbf{C}$，根据考虑实际或复杂的措施）（A，III, §2, No. 6）。

2) 令$M$为配备离散拓扑的幺半群；假设对于每个$m \in M$，只有有限多个对$(m', m'') \in M \times M$使得$m'm'' = m$；这等于说，$M$中合成的律是$M \times M$到$M$的真映射； $M$ 然后形式代数用于卷积，代数就是*总计*

(1) Monoïde，Exer 意义上的。第 17 章。 VII, §1。

幺半群 $M$ (A, III, §2, No. 10) 的代数；我们注以下两种特殊情况：

a) $M = N$，合成中的律为加法。对于$N$上的每一个小节$\mu$，让我们将正式的级数联系起来

$$
S(\mu) = \sum_{n=0}^{\infty} \mu(\{n\}) t^n
$$

在不确定的 $t$ 中。然后$S(\mu * \mu') = S(\mu)S(\mu')$。类似的注适用于任何数不定式中的正式级数。

$*b)$$M = N^*$，合成中的律为乘法。对于$N^*$上的每一个小节$\mu$，让我们将形式狄利克雷级数联系起来

$$
D(\mu) = \sum_{n=1}^{\infty} \mu(\{n\}) n^{-s}.
$$

然后$D(\mu * \mu') = D(\mu)D(\mu')$。

3) 让$X, Y, Z$局部紧致空间，$\varphi$将$X \times Y$的连续映射变成$Z$。如果$x \in X$和$\mu$是$Y$的测度，则说$\varepsilon_x$和$\mu$是$\varphi$可卷积的，则说将$Y$的映射$\varphi(x, \cdot)$转化为说 $Z$ 是$\mu$-正确的。那么就有$\varepsilon_x * \mu = \varphi(x, \cdot)(\mu)$。

### 2.结合性

以下引理完成了第 11 章的命题 11。 V, §8, No. 5:²

#### 引理 1 {#int-viii-s1-lem-1 .statement tag=09I2}

对于$1 \leq i \leq n$，令$X_i, Y_i$为两个局部紧凑的空间，$\mu_i$为$X_i$的测度，$\varphi_i$为$X_i$到$Y_i$的连续映射。将$X$的$X = \prod_i X_i$、$Y = \prod_i Y_i$、$\mu = \bigotimes_i \mu_i$、$\varphi$映射代入$Y$，即$\varphi_i$的乘积。如果对于每个 $i$，$\varphi$ 是 $\mu$ 正值且 $\mu_i \neq 0$，则 $\varphi_i$ 是 $\mu_i$ 正值和 $\varphi(\mu) = \bigotimes_i \varphi_i(\mu_i)$。

我们可以假设 $\mu_i$ 为正且$n = 2$。让$f_1 \in \mathscr{K}_+(Y_1)$。由于$\mu_2 \neq 0$，存在$f_2 \in \mathscr{K}_+(Y_2)$，使得$f_2 \circ \varphi_2$不是$\mu_2$可以忽略不计。 函数$(x_1, x_2) \mapsto f_1(\varphi_1(x_1)) f_2(\varphi_2(x_2))$本质上是$\mu$可积且连续的，因此$\mu$可积。因此，存在$x_2 \in X_2$使得$f_2(\varphi_2(x_2)) \neq 0$并且使得函数$x_1 \mapsto f_1(\varphi_1(x_1)) f_2(\varphi_2(x_2))$是$\mu_1$可积。因此 $f_1 \circ \varphi_1$ 是 $\mu_1$ 可积，

²在引理之后是引用的第11号提案的部分b)中的归纳，即$n = 2$的情况； 相应的导致第 1 章第一版。 V（§8, No. 3，提案 7）不包括部分 b) 的结果。

这证明$\varphi_1$是$\mu_1$-正确的。有人对 $\varphi_2$ 也有类似的争论。然后是第 11 章第 11 章的 $\varphi(\mu) = \bigotimes_i \varphi_i(\mu_i)$。 V, §8, No. 5。

以下引理完成了第 4 章的命题 4。 V, §6, No. 3。\脚注{这个引理的断言实际上是引用的第4条提案中的部分*b*)，部分未包含在第1章第1版中。 V.}

#### 引理 2 {#int-viii-s1-lem-2 .statement tag=09I3}

*设 T、T'、T'' 为三个局部紧凑空间、$\mu$ T 上的度量、$\pi$ 将 T 的 $\mu$ 可测量的映射放入 T'、$\pi'$ 将 T' 的连续映射放入 T'' 以及 $\pi'' = \pi' \circ \pi$。如果$\pi''$是$\mu$-本征，则$\pi$是$\mu$-本征，$\pi'$是$\pi(\mu)$-本征，并且$\pi''(\mu) = \pi'(\pi(\mu))$。

设 K' 是 T' 的紧子集。那么$K'' = \pi'(K')$是紧的，因此$\pi''(K'')$本质上是$\mu$可积，因此$\pi^{-1}(K') \subset \pi''(K'')$本质上是$\mu$可积，因此$\pi$是$\mu$本征。那么 $\pi'$ 是 $\pi(\mu)$-proper，$\pi''(\mu) = \pi'(\pi(\mu))$ 是 Ch 。 V, §6, No. 3，提案 4。

#### 命题 1 {#int-viii-s1-prop-1 .statement tag=09I4}

*令$X_{ij}$ ($1 \leq i \leq m, 1 \leq j \leq n_i$)、$Y_i$ ($1 \leq i \leq m$) 和Z 局部紧致空间；对于每个 i，令 $\varphi_i$ 为 $X_i = \prod_j X_{ij}$ 的映射到 $Y_i$；设$\varphi$为$\varphi_i$、映射$X = \prod_i X_i$的乘积到$Y = \prod_i Y_i$；令 $\psi$ 为 Y 到 Z 的映射。

(i) *令$\mu_{ij}$分别为$X_{ij}$上给出的测度，使得对于每个i，$\mu_{ij}$($1 \leq j \leq n_i$)是$\varphi_i$可卷积的，并且使得测度$*| \mu_{ij} |$是$\psi$可卷积的；那么$\mu_{ij}$对于$1 \leq i \leq m, 1 \leq j \leq n_i$来说是$(\psi \circ \varphi)$可卷积的并且*

$$
*_{i,j} \mu_{ij} = *_i \left( *_j \mu_{ij} \right).
$$

(ii) *假设$\psi$和$\varphi_i$连续，并令$\mu_{ij}$分别为$X_{ij}$和$(\psi \circ \varphi)$可卷积的测度$\neq 0$；那么，对于每个 i，$\mu_{ij}$ ($1 \leq j \leq n_i$) 是 $\varphi_i$ 可卷积的，度量 $*_j |\mu_{ij}|$ 是 $\psi$ 可卷积的，并且公式 (3) 成立。*

考虑所有相关措施都是$\geq 0$的情况就足够了。

让我们将自己置于（i）的假设之下。 映射 $\varphi$ 适合 $\bigotimes_{i,j} \mu_{ij}$，并且

$$
\varphi \left( \bigotimes_{i,j} \mu_{ij} \right) = \bigotimes_i \varphi_i \left( \bigotimes_j \mu_{ij} \right) = \bigotimes_i \left( *_j \mu_{ij} \right)
$$

（第 V, §8, No. 5 章，第 11 条提案）。 映射 $\psi \circ \varphi$ 适合 $\bigotimes_{i,j} \mu_{ij}$，并且
$$
(\psi \circ \varphi)\left( \bigotimes_{i,j} \mu_{ij} \right) = \psi\left( \bigotimes_i (*_j \mu_{ij}) \right) = *_i (*_j \mu_{ij})
$$
（第 V, §6 章，提案 4）。因此$\mu_{ij}$ ($1 \leq i \leq m,\ 1 \leq j \leq n_i$) 是$(\psi \circ \varphi)$可卷积的并且公式 (3) 成立。

让我们将自己置于（ii）的假设之下。首先，引理2证明$\varphi$适合$\bigotimes_{i,j} \mu_{ij}$。 引理 1 然后证明对于每个 $i$，$\varphi_i$ 对于 $\bigotimes_j \mu_{ij}$ 是正确的，并且
$$
\varphi\left( \bigotimes_{i,j} \mu_{ij} \right) = \bigotimes_i (*_j \mu_{ij}).
$$
到引理 2 时，$\psi$ 适合 $\bigotimes_i (*_j \mu_{ij})$。 从而命题。

#### 推论 {#int-viii-s1-n2-cor-1 .statement tag=09I5}

— 令 $X_i, X'_i$ ($1 \leq i \leq n$), $Y, Y'$ 局部紧致空间；设$\varphi, \varphi'$分别是$X = \prod_i X_i$的映射连续到$Y$和$X' = \prod_i X'_i$连续到$Y'$；设$f_i$是$X_i$的连续映射到$X'_i$（$1 \leq i \leq n$），$g$是$Y$的连续映射到$Y'$，这样$\varphi' \circ f = g \circ \varphi$，$f$是将$X$的映射转化为$X'$，即$f_i$的乘积。令$\mu_i$分别为$X_i$、所有$\neq 0$给出的措施。那么下面两个断言是等价的：
(i) $f_i$对于所有$i$来说是$\mu_i$-适当的，并且度量$f_i(|\mu_i|)$是$\varphi'$-可卷积的；
(ii) $\mu_i$ 是 $\varphi$ 可卷积的，$g$ 适用于 $*_{\varphi}(|\mu_i|)$。

而且，当这些断言得到验证后，
$$
*_{\varphi'}(f_i(\mu_i)) = g(*_{\varphi}(\mu_i)) = *_{g \circ \varphi}(\mu_i).
$$

对于，让$h = \varphi' \circ f = g \circ \varphi$。根据命题 1，条件 (i) 和 (ii) 分别等价于以下条件：
(iii) $\mu_i$ 是 $h$ 可卷积的。
当这样的时候，
$$
*_{\varphi'}(f_i(\mu_i)) = *_h(\mu_i) = g(*_{\varphi}(\mu_i)).
$$

### 3. 有界测度的情况

#### 命题 2 {#int-viii-s1-prop-2 .statement tag=09I6}

— 令 $X_1, \ldots, X_n, Y$ 为局部紧致空间，$\mu_i$ $X_i$ ($1 \leq i \leq n$) 上的有界测度，$\mu_i$ 的$\mu$ 乘积，$\varphi$ $\mu$ 可测映射 $\prod_{i=1}^n X_i$ 变成$Y$。那么 $\mu_i$ 是 $\varphi$ 可卷积的，并且
$$
\left\| *_{i=1}^n \mu_i \right\| \leq \prod_{i=1}^n \| \mu_i \|.
$$
如果 $\mu_i$ 而且是正数，那么
$$
\left\| *_{i=1}^n \mu_i \right\| = \prod_{i=1}^n \| \mu_i \|.
$$
对于，$\mu'_i = |\mu_i|$ 有界，$\| \mu'_i \| = \| \mu_i \|$（第 III, §1, No. 8 章，第 10 条命题第 1 条）。一个有 $|\mu_1 \otimes \cdots \otimes \mu_n| = \mu'_1 \otimes \cdots \otimes \mu'_n$（第 III, §4，第 2、4 章），因而 $\mu_1 \otimes \cdots \otimes \mu_n$ 是有界的，并且
$$
\| \mu_1 \otimes \cdots \otimes \mu_n \| = \| \mu_1 \| \cdots \| \mu_n \|
$$
（同上，提案 4）。因而 $\varphi$ 是 $\mu$-固有的（Ch. V, §6, No. 1，注 1），即 $\mu_i$ 是$\varphi$-可卷积的。一个有$\| *_{i=1}^n \mu'_i \| = \| \mu'_1 \otimes \cdots \otimes \mu'_n \|$（第V, §6, No. 2，第1章），因而$\| *_{i=1}^n \mu'_i \| = \| \mu'_1 \| \cdots \| \mu'_n \|$。最后，$| *_{i} \mu_i | \leq *_{i} \mu'_i$ (No. 1, 公式 (2))，因而
$$
\left\| *_{i} \mu_i \right\| \leq \left\| *_{i} \mu'_i \right\| = \prod_{i=1}^n \| \mu_i \|.
$$

#### 命题 3 {#int-viii-s1-prop-3 .statement tag=09I7}

— 令$X_1, \ldots, X_n, Y$局部紧凑空间，$\varphi$将$\prod_{i=1}^n X_i$的连续映射变为$Y$。然后映射
$$
(\mu, \ldots, \mu_n) \mapsto *_{\varphi} (\mu_i)
$$
$\prod_{i=1}^n \mathscr{M}^1(X_i)$ 到 $\mathscr{M}^1(Y)$ 是连续多重线性映射。
这是根据第 2 条命题以及No. 1 中的内容得出的。

### 4. 与支撑有关的属性

#### 命题 4 {#int-viii-s1-prop-4 .statement tag=09I8}

— 令$X_1, \ldots, X_n, Y$局部紧凑空间，$\mu_i$右$X_i$（$1 \leq i \leq n$）的测度，$S_i$其支持，$\varphi$将$\prod_i X_i$连续映射引入$Y$，使得$\varphi$到$\prod_i S_i$中的限制是合适的。那么 $\mu_i$ 是 $\varphi$ 可卷积的。

例如，令 $K$ 为 $Y$ 的紧凑子集。 $\mu = \mu_1 \otimes \cdots \otimes \mu_n$ 的支持度是 $S = \prod_i S_i$（第 III, §4, No. 2 章，提案 2）。因而$\overline{\varphi}(K) \cap \left( \prod_i X_i - S \right)$是$\mu$-可以忽略不计。另一方面，$\overline{\varphi}(K) \cap S$ 是紧凑的。因而$\overline{\varphi}(K)$是$\mu$可积的。

#### 命题 5 {#int-viii-s1-prop-5 .statement tag=09I9}

*令$X_1, \ldots, X_n, Y$局部紧致空间，$\mu_i$右$X_i$（$1 \leq i \leq n$）、$\mu$乘积的测量$\mu_i$，$\varphi$$\mu$-适当的映射 $\prod_i X_i$转化为$Y$，以及$S_i$$\mu_i$的支持。

a) *右$*_{i} \mu_i$的支持包含在$\varphi \left( \prod_i S_i \right)$的闭包中。*

b) *如果$\varphi$连续且$\mu_i$为正，那么$*_{i} \mu_i$的支撑就是$\varphi \left( \prod_i S_i \right)$的闭包。*

设$S = \prod_i S_i$为$\mu$的支撑。 $*_{i} \mu_i$ 的支持由 Ch. 包含在 $\overline{\varphi(S)}$ 中。 V, §6, No. 2，科。命题 2 中的 3。 *如果 $\varphi$ 是连续的并且 $\mu_i$ 是正数，那么 $*_{i} \mu_i$ 的支持度是 $\overline{\varphi(S)}$*（*loc. cit.*，命题 2 的 Cor. 4）。

#### 推论 {#int-viii-s1-n4-cor-1 .statement tag=09IA}

*如果$\varphi$是连续的并且$\mu_i$有紧支撑，那么$\mu_i$是可卷积的并且$*_{i} \mu_i$有紧支撑。*

### 5.卷积的向量表达乘积

#### 命题 6 {#int-viii-s1-prop-6 .statement tag=09IB}

*令$X, Y, Z$局部紧致空间，$\varphi$将$X \times Y$的连续映射引入$Z$，并在$X, Y$上测量$\lambda, \mu$。为了使$\lambda$和$\mu$可$\varphi$可卷积，$X \times Y$的映射$(x, y) \mapsto \varepsilon_{\varphi(x,y)} = \varepsilon_x * \varepsilon_y$进入$\mathscr{M}(Z)$对于拓扑$\sigma(\mathscr{M}(Z), \mathscr{H}(Z))$可标量$(\lambda \otimes \mu)$可积，在这种情况下*

$$
\lambda * \mu = \int_{X \times Y} (\varepsilon_x * \varepsilon_y) \, d\lambda(x) \, d\mu(y).
$$

说 $\lambda$ 和 $\mu$ 是 $\varphi$ 可卷积，意味着对于每个 $f \in \mathscr{H}(Z)$，$f \circ \varphi$ 是 $(\lambda \otimes \mu)$ 可积，也就是说，对于每个 $f \in \mathscr{H}(Z)$ 函数 $(x, y) \mapsto \langle f, \varepsilon_{\varphi(x,y)} \rangle$ 是$(\lambda \otimes \mu)$可积，也就是说，$X \times Y$到$\mathscr{M}(Z)$的映射$(x, y) \mapsto \varepsilon_{\varphi(x,y)}$对于$\sigma(\mathscr{M}(Z), \mathscr{K}(Z))$是可标量$(\lambda \otimes \mu)$可积的。如果是这样的话，那么

$$
\langle \lambda * \mu, f \rangle = \int f(\varphi(x, y)) d\lambda(x) d\mu(y) = \int_{X \times Y} \langle \varepsilon_{\varphi(x,y)}, f \rangle d\lambda(x) d\mu(y),
$$

从而$\lambda * \mu = \int_{X \times Y} \varepsilon_{\varphi(x,y)} d\lambda(x) d\mu(y)$。

#### 命题 7 {#int-viii-s1-prop-7 .statement tag=09IC}

*令 X, Y, Z 局部紧致空间，$\varphi$ $X \times Y$ 的连续映射进入 Z，并且 $\lambda, \mu$ 在 X, Y 上进行测量。假设对于每个 $x \in X$，$\varepsilon_x$ 和 $\mu$ $\varphi$-可卷积。为了使$\lambda$和$\mu$能够$\varphi$可卷积，X的映射$x \mapsto \varepsilon_x * |\mu|$进入$\mathscr{M}(Z)$对于拓扑$\sigma(\mathscr{M}(Z), \mathscr{K}(Z))$是可标量$\lambda$可积的，其中案例$\lambda * \mu = \int_X (\varepsilon_x * \mu) d\lambda(x)$.*

假设$\lambda$和$\mu$是$\varphi$可卷积的。对于每个$f \in \mathscr{K}(Z)$，$f \circ \varphi$是$(|\lambda| \otimes |\mu|)$可积，因此函数$x \mapsto \int_Y f(\varphi(x, y)) d|\mu|(y) = \langle f, \varepsilon_x * |\mu| \rangle$（由假设为所有$x \in X$定义）是$\lambda$可积；因此 $x \mapsto \varepsilon_x * |\mu|$ 对于 $\sigma(\mathscr{M}(Z), \mathscr{K}(Z))$ 是 $\lambda$ 标量可积的，并且

$$
\langle f, \lambda * \mu \rangle = \int_X d\lambda(x) \int_Y f(\varphi(x, y)) d\mu(y) = \int_X \langle f, \varepsilon_x * \mu \rangle d\lambda(x),
$$

从而$\lambda * \mu = \int_X (\varepsilon_x * \mu) d\lambda(x)$。相反，假设 X 的映射 $x \mapsto \varepsilon_x * |\mu|$ 到 $\mathscr{M}(Z)$ 对于 $\sigma(\mathscr{M}(Z), \mathscr{K}(Z))$ 是可标量 $\lambda$ 可积的。让$f \in \mathscr{K}_+(Z)$。那么函数 $(x, y) \mapsto f(\varphi(x, y))$ 是连续的并且（第 V, §8, No. 3 章，第 5 条命题）

$$
\iint^* f(\varphi(x, y)) d|\lambda|(x) d|\mu|(y) = \int^* d|\lambda|(x) \int^* f(\varphi(x, y)) d|\mu|(y)
= \int^* \langle f, \varepsilon_x * |\mu| \rangle d|\lambda|(x) < +\infty.
$$

因此$f \circ \varphi$是$(\lambda \otimes \mu)$可积，因此$\lambda$和$\mu$是$\varphi$可卷积。

### 习题 {#int-viii-s1-exercises}

§ 1](exercises/s1/)参见[习题。
