---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 3
section_title: Special function spaces
lang: zh
source: top-v-x
pdf_pages: 0299-0314, 0333-0343
extraction: ocr
subsections:
    - "no": 1
      title: SPACES OF MAPPINGS INTO A METRIC SPACE
      page: 0
      pdf_page: 299
    - "no": 2
      title: SPACES OF MAPPINGS INTO A NORMED SPACE
      page: 0
      pdf_page: 301
    - "no": 3
      title: COUNTABILITY PROPERTIES OF SPACES OF CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 304
    - "no": 4
      title: THE COMPACT-OPEN TOPOLOGY
      page: 0
      pdf_page: 306
    - "no": 5
      title: TOPOLOGIES ON GROUPS OF HOMEOMORPHISMS
      page: 0
      pdf_page: 311
statements: 31
exercises: 29
content_sha256: 449c169cd9d088c427c0a7fe762aefa24fa487ab69e167057547071147587c4d
translated_from: content/en/top/X/03_s3_special_function_spaces.md
translation_method: google
source_content_sha256: a35a28b9c26f164aeaf3bf1e204cb5b3731409c5cea341ad50336a5b5719bb98
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: cda6601186686ea461e9cdf56fbf4f7ed0e93f886af4c3c71f96fe13d797242e
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 3. 特别函数空间

### 1. 将映射的空间转换为公制空间

令$X$为集合，$Y$统一空间，$(f_i)_{i \in I}$定义$Y$（章IX, § 1, no. 4）的统一结构的伪度量族，并令$\mathscr{S}$为集合子集共$X$。对于$X$的每个$i \in I$、每个集合$A \in \mathscr{S}$、以及映射的每个对$(u, v)$到$Y$，写

$$
g_{i, A}(u, v) = \sup_{x \in A} f_i(u(x), v(x));
$$

紧接着，$g_{i, A}$是$\mathscr{F}(X; Y)$上的*伪计量*，并且伪计量家族$(g_{i, A})_{i \in I, A \in \mathscr{S}}$定义是$\mathscr{S}$-*收敛*在$\mathscr{F}(X; Y)$上的均匀性。特别是：

#### 命题 1 {#top-x-s3-prop-1 .statement tag=0CD8}

*如果$Y$是可度量的均匀性空间，则$\mathscr{F}(X; Y)$上的一致收敛的均匀性是可度量的。*

因为如果 $d$ 是 $Y$ 上的一个度量，并且与其一致的结构兼容，那么 $\mathscr{F}(X; Y)$ 上一致收敛的结构由单个伪度量定义

$$
\varepsilon(u, v) = \sup_{x \in X} d(u(x), v(x));
$$

一般来说，这个伪度量不是有限的，但它等效于有限的伪度量（章IX, § 1, no. 2），并且由于一致收敛的均匀性是Hausdorff（§ 1, no. 2，命题1），因此它是可度量的。

#### 推论 {#top-x-s3-n1-cor-1 .statement tag=0CD9}

令$X$为拓扑空间，并令$Y$为可度量均匀空间。假设$X$的紧凑子集有序列$(K_n)$，使得$X$的每个紧凑子集都包含在某个$K_n$中。那么$\mathscr{F}(X; Y)$上的紧收敛的均匀性是可度量的。

由于$K_n$覆盖$X$，$\mathscr{F}_c(X; Y)$同构于$\prod_n \mathscr{F}_u(K_n; Y)$的均匀子空间（$§ 1$，no. 2，注3），因此推论从命题1得出（章IX, § 2, no. 4、定理1、推论2）。

请注意，如果 $X$ 是*局部紧致且 σ 紧致*（章 I, § 9, no. 9、命题 15、推论 1），则此推论特别适用。

现在让 $Y$ 成为空间的度量，并让 $d$ 成为它的度量。如果$X$是任何集合和$\mathscr{S}$任何集合或子集或$X$，我们将用所有映射$u : X \to Y$中的$\mathscr{B}_{\mathscr{S}}(X; Y)$集合表示，使得对于每个$A \in \mathscr{S}$，$u(A)$都是*有界*的。 除非相反，我们明确指出，我们将认为$\mathscr{B}_{\mathscr{S}}(X; Y)$ 具有$\mathscr{S}$收敛的一致性，这是由$\mathscr{B}_{\mathscr{S}}(X; Y)$上的以下伪度量族定义的：

$$
d_A(u, v) = \sup_{x \in A} d(u(x), v(x)) \tag{$A \in \mathscr{S}$}
$$

假设 *有限*。当$\mathscr{S} = \{X\}$时，我们写$\mathscr{B}(X; Y)$来代替$\mathscr{B}_{\mathscr{S}}(X; Y)$。如果属于到$\mathscr{B}(X; Y)$，即如果$u(X)$是$Y$的有界子集，则映射$u : X \to Y$被称为“有界”。

#### 命题 2 {#top-x-s3-prop-2 .statement tag=0CDA}

令$X$为集合，并且$Y$为度量空间。有界映射的集合 $\mathscr{B}(X; Y)$ 在空间 $\mathscr{F}_u(X; Y)$ 中既开又闭。

如果 $u$ 有界，则每个映射 $v : X \to Y$ 对于所有 $x \in X$，我们有 $d(u(x), v(x)) \leq 1$ 有界，因为

$$
d(v(x), v(x_0)) \leq d(u(x), u(x_0)) + 2;
$$

因此$\mathscr{B}(X; Y)$是开放的。另一方面，如果$u$位于$\mathscr{F}_u(X; Y)$中$\mathscr{B}(X; Y)$的闭包中，则存在映射$u_0 \in \mathscr{B}(X; Y)$，使得$d(u(x), u_0(x)) \leq 1$对于所有$x \in X$；因此 $u$ 是有界的。

#### 推论 1 {#top-x-s3-prop-2-cor-1 .statement tag=0CDB}

令 $X$ 为集合，并且 $Y$ 为度量空间。然后$\mathscr{B}_{\mathscr{S}}(X; Y)$在$\mathscr{F}_{\mathscr{S}}(X; Y)$关闭。特别是，如果 $Y$ 是完备的，那么 $\mathscr{B}_{\mathscr{S}}(X; Y)$ 就 $\mathscr{S}$ 收敛的均匀性而言是完备的。

对于$\mathscr{B}_\mathfrak{S}(X; Y)$是将$\mathscr{F}_\mathfrak{S}(X; Y)$典范映射下乘积$\prod_{A \in \mathfrak{S}} \mathscr{F}_u(X; Y)$子集$\prod_{A \in \mathfrak{S}} \mathscr{B}(A; Y)$逆像换成$\prod_{A \in \mathfrak{S}} \mathscr{F}_u(A; Y)$；因此，如果我们考虑 § 1, no. 5 的定理 1，第一个断言是从§ 1, no. 2、注3得出的，而第二个断言是从第一个得出的。

#### 推论 2 {#top-x-s3-prop-2-cor-2 .statement tag=0CDC}

*设X为拓扑空间，Y为度量空间。则X到Y的所有有界连续映射的空间在$C_u(X; Y)$中既开又闭；如果 Y 完整，则它完整。*

问题中的空间是$\mathscr{B}(X; Y) \cap C_u(X; Y)$；第一个断言源自命题 2；第二个紧随第一个（$§ 1$、no. 6、定理 2、推论 1）。

### 2. 将映射的空间转换为规范的空间

更具体地，考虑 Y 是非离散值除法环 K (章 IX, § 3, no. 3) 上的 *范数* 向量空间的情况。让我们用$y \in Y$的$||y||$范数来表示。 集合 $\mathscr{F}(X; Y) = Y^X$ 则被规范地赋予K-向量空间结构。 映射 $u : X \to Y$ 是有界的当且仅当实值函数 $x \mapsto ||u(x)||$ 在 X 内有界。如果$u, v$将X的映射有界入Y，则显然$u + v$和$\lambda u (\lambda \in K)$有界；在其他字中，$\mathscr{B}(X; Y)$是$\mathscr{F}(X; Y)$的*向量子空间*。而且，$||u|| = \sup_{x \in X} ||u(x)||$是$\mathscr{B}(X; Y)$上的*范数*；因为它满足三角形不等式和$||u|| = 0$意味着$u = 0$，并且对于每个$\lambda \in K$我们有

$$
||\lambda u|| = \sup_{x \in X} ||\lambda u(x)|| = \sup_{x \in X} |\lambda| \cdot ||u(x)|| = |\lambda| \cdot \sup_{x \in X} ||u(x)|| = |\lambda| \cdot ||u||.
$$

而且，立即验证了这个范数定义的$\mathscr{B}(X; Y)$上的均匀性就是一致收敛的均匀性。 除非相反，明确指出，每当$\mathscr{B}(X; Y)$被视为规范的空间时，它就是上面定义的范数，这是有问题的。

#### 命题 3 {#top-x-s3-prop-3 .statement tag=0CDD}

*如果赋范空间 Y 是完整的，则 X 有界映射的每个级数 $(u_n)$ 都绝对收敛于赋范空间 $\mathscr{B}(X; Y)$（即，$\sum_{n=0}^\infty ||u_n|| < +\infty$； cf. 章 IX, § 3, no. 6) 一致收敛于X。*

因为由于 $\mathscr{B}(X; Y)$ 是完备的（no. 1、命题 2、推论 1），因此结果来自一致收敛的级数的章 IX, § 3, no. 6、命题 11 和定义。

#### 注 1 {#top-x-s3-n2-rem-1 .statement tag=0CDE}

如果$\sum_{n=0}^{\infty} \|u_n\| < +\infty$，则$\sum_{n=0}^{\infty} |u_n(x)| \leq \sum_{n=0}^{\infty} |u_n| < +\infty$
对于每个$x \in X$；在其他字中，对于每个$x \in X$级数与一般项$u_n(x)$绝对收敛于空间$Y$。 逆命题是假的。为了避免所有混淆，我们将有时说级数与一般项$u_n$*通常收敛*，这意味着级数与一般项$\|u_n\|$收敛。 级数可以一致收敛于$X$，无需常收敛；例如，对于空间 $\mathscr{B}(\mathbf{R}, \mathbf{R})$ 中的级数 $(u_n)$，定义如下：
如果$x \in [n\pi, (n+1)\pi]$则为$u_n(x) = (1/n) \sin x$，否则为$u_n(x) = 0$。

当 $Y$ 是非离散值域 $K$ 上的*范数代数* (章 IX, § 3, no. 7) 时，则 $\mathscr{B}(X; Y)$ 是 $K$ 代数，范数 $\|u\|$ 是与代数结构兼容，因为
$$
\|uv\| = \sup_{x \in X} \|u(x)v(x)\| \leq \sup_{x \in X} \|u(x)\| \cdot \|v(x)\|
\leq \sup_{x \in X} \|u(x)\| \cdot \sup_{x \in X} \|v(x)\| = \|u\| \cdot \|v\|.
$$
因此，$\mathscr{B}(X; Y)$ 现在是 $K$ 的*范数代数*。

#### 命题 4 {#top-x-s3-prop-4 .statement tag=0CDF}

*让$X_i$ ($1 \leq i \leq n$) 和$Y$ 在非离散值除法环 $K$ 上标准化向量空间，并令$X = \prod_{i=1}^n X_i$。那么$X$到$Y$的所有多重线性映射的集合在空间$\mathscr{F}_s(X; Y)$中闭合。*

这个集合由所有$u \in F(X; Y)$组成，其中满足所有关系
$$
\begin{align*}
u(x_1, \ldots, x_i' + x_i'', \ldots, x_n) &= u(x_1, \ldots, x_i', \ldots, x_n) \\
&\quad + u(x_1, \ldots, x_i'', \ldots, x_n), \\
u(x_1, \ldots, \lambda x_i, \ldots, x_n) &= \lambda u(x_1, \ldots, x_i, \ldots, x_n)
\end{align*}
$$
（$1 \leq i \leq n,\ x_i,\ x_i',\ x_i''$$X_i$中的任意元素，$\lambda$$K$中的任意元素）；由于关系(1)两边都是$\mathscr{F}_s(X; Y)$上$u$的函数连续(§ 1, no. 2，注6)，所以结果如下(章I, § 8, no. 1，命题2)。

#### 命题 5 {#top-x-s3-prop-5 .statement tag=0CDG}

*在命题 4的假设下，$X$到$Y$的连续多线性映射的集合$\mathscr{L}(X_1, \ldots, X_n; Y)$相对于有界收敛的拓扑在$\mathscr{F}(X; Y)$闭合；如果 $Y$ 是完备的，那么它就有界收敛的一致性而言是完备的。*

因为如果$\mathscr{G}$是$X$的所有有界子集的集合，则$\mathscr{L}(X_1, \ldots, X_n; Y)$是$X$的所有多重线性映射的集合交到$Y$并且集合$\mathscr{B}_\mathscr{G}(X; Y)$（章IX, § 3, no. 5，定理1）；因此，结果由命题 4 和命题 2、推论 1 得出。

对于小节的其余部分，$K$ 表示非离散值域。

那么$\mathscr{L}(X_1, \ldots, X_n; Y)$就是$\mathscr{F}(X; Y)$的向量子空间。令$B$为所有$(x_i)_{1 \leq i \leq n}$中$X$、集合中的单位球，使得$\sup_{1 \leq i \leq n} \|x_i\| \leq 1$。

那么$\mathscr{L}(X_1, \ldots, X_n; Y)$到$\mathscr{B}(B; Y)$的映射$u \to u|B$是单射的；而且，逆像，在此映射下，$\mathscr{B}(B; Y)$上一致收敛的均匀性就是$\mathscr{L}(X_1, \ldots, X_n; Y)$上有界收敛的均匀性。对于$X$的每个有界子集都包含在形式$\mu B$的集合中（对于某些$\mu \in K^*$），并且如果$u$是$\mathscr{L}(X_1, \ldots, X_n; Y)$的元素，则可以说对于所有$\|u(z)\| \leq a$ $z \in \mu B$ 相当于说，$\|u(z)\| \leq a/|\mu|^n$ 对于所有 $z \in B$。很容易验证数
$$
\|u\| = \sup_{z \neq 0} \frac{\|u(z)\|}{\|z\|}
$$
是 $\mathscr{L}(X_1, \ldots, X_n; Y)$ 和定义上的范数集合有界收敛的一致性，显然我们有
$$
(2) \quad \|u(x_1, \ldots, x_n)\| \leq \|u\| \cdot \|x_1\| \cdots \|x_n\|.
$$

除非相反，明确指出，每当$\mathscr{L}(X_1, \ldots, X_n; Y)$被视为规范的空间时，它就是上面定义的范数，这是有问题的。

#### 命题 6 {#top-x-s3-prop-6 .statement tag=0CDH}

*多线性映射*
$$
(u, x_1, \ldots, x_n) \to u(x_1, \ldots, x_n)
$$
*规范的空间* $\mathscr{L}(X_1, \ldots, X_n; Y) \times X_1 \times \cdots \times X_n$ *到* $Y$ *是连续的*。

这是不等式 (2) 的直接的推论 (章 IX, § 3, no. 5, 定理 1)。

#### 命题 7 {#top-x-s3-prop-7 .statement tag=0CDI}

*让*$X, Y, Z$*成为三范数空间超过*$K$。 *规范空间* $\mathscr{L}(X, Y; Z)$ *到* $X$ *到* $\mathscr{L}(Y; Z)$ *的线性映射空间*将每个* $u \in \mathscr{L}(X, Y; Z)$ *发送到映射* $x \to u(x, .)$ *是* $\mathscr{L}(X; Y; Z)$ *到* $\mathscr{L}(X; \mathscr{L}(Y; Z))$的等距。

这紧接着定义和关系
$$
\sup_{\|x\| \leq 1} \left( \sup_{\|y\| \leq 1} \|u(x, y)\| \right) = \sup_{\|x\| \leq 1, \|y\| \leq 1} \|u(x, y)\|.
$$

#### 命题 8 {#top-x-s3-prop-8 .statement tag=0CDJ}

令$X, Y, Z$为空间除以$K$的三范数。 $\mathscr{L}(X; Y) \times \mathscr{L}(Y; Z)$ 到 $\mathscr{L}(X; Z)$ 的双线性映射 $(u, v) \to v \circ u$ 是连续的。

对于如果 $u \in \mathscr{L}(X; Y)$ 和 $v \in \mathscr{L}(Y; Z)$ 我们有
$$
||v \circ u|| \leq ||u|| \cdot ||v||,
$$
因为对于所有$x \in X$，由于（2），我们有$||v(u(x))|| \leq ||v|| \cdot ||u(x)|| \leq ||v|| \cdot ||u|| \cdot ||x||$。

特别是，在空间$X$超过$K$的连续自同态的集合$\mathscr{L}(X)$上，范数$||u||$与$\mathscr{L}(X)$的$K$代数结构兼容。

#### 注 2 {#top-x-s3-n2-rem-2 .statement tag=0CDK}

集合 $\mathscr{L}(\mathbf{R}^m; \mathbf{R}^n)$ 线性（必须连续） $\mathbf{R}^m$ 的映射进入 $\mathbf{R}^n$ 可以用矩阵的集合 $M_{n,m}(\mathbf{R})$ 与 $n$ 行和 $m$ 列识别系数在$\mathbf{R}$中，因此可以与$\mathbf{R}^{mn}$识别；在$\mathscr{L}(\mathbf{R}^m; \mathbf{R}^n)$上，有界收敛的均匀性（相对于$\mathbf{R}^m$上的欧氏度量）、紧凑收敛和逐点收敛的均匀性然后用$\mathbf{R}^{mn}$上的*加性*均匀性来确定。取$x = (x_i) \in \mathbf{R}^n$中的范数为
$$
||x|| = \sup_i |x_i|,
$$
令$(e_j)$为$\mathbf{R}^m$中的典范基；如果$u$和$v$是$\mathbf{R}^m$到$\mathbf{R}^n$的两个线性映射，使得$\|u(e_j) - v(e_j)\| \leq \epsilon$对应$1 \leq j \leq m$，那么对于每个对$(i, j)$我们有$|\alpha_{ij} - \beta_{ij}| \leq \epsilon$[$U = (\alpha_{ij})$和$V = (\beta_{ij})$分别为$u, v$的矩阵]；相反，如果满足这些不等式，对于 $\mathbf{R}^m$ 中中心 o 和边 $a$ 的立方体的每个点 $x$，我们都有$\|u(x) - v(x)\| \leq ma\epsilon$。

### 3. 连续函数空间的可数性

#### 定理 1 {#top-x-s3-thm-1 .statement tag=0CDL}

设$X$为紧凑的空间。
a) *如果 $X$ 是可度量的，并且如果 $Y$ 是可数型* (章 IX, § 2, no. 8) 的任意可度量均匀空间，*则连续映射的可度量空间 $C_u(X; Y)$ $X$转化为$Y$，赋予拓扑一致收敛性，型*可数。
b) *相反，如果可度量的空间 $C_u(X; \mathbf{R})$ 是可数的型，则 $X$ 是可度量的*。

a) 令$d$（或$d'$）为与$X$的拓扑兼容的度量（或具有$Y$的一致性）；那么 $\delta(f, g) = \sup_{x \in X} d'(f(x), g(x))$ 是定义空间 $C(X; Y)$、函数上$C(X; Y)$ 有界一致收敛的均匀性的度量，因为 $X$ 是紧致的 (no. 1)。 对于整数$m > 0, n > 0$的每个对，令$G_{mn}$为函数$f \in \mathscr{C}(X; Y)$的集合，使得关系$d(x, x') \leq 1/m$蕴涵$d(f(x), f(x')) \leq 1/n$。 每个函数 $f \in \mathscr{C}(X; Y)$ 都是一致连续的 (章 II, § 4, no. 1, 定理 2)，因此，对于每个 $n > 0$，$\mathscr{C}(X; Y)$ 是集合 $G_{mn}$ ($m > 0$) 的并。 令$\{a_1, \ldots, a_{p(m)}\}$为$X$的有限子集，使得具有中心$a_i$和半径$1/m$的开球覆盖$X$（$1 \leq i \leq p(m)$）；令$(b_r)_{r \in \mathbf{N}}$为可数序列，其在$Y$中稠密。 对于每个映射$\varphi : [1, p(m)] \to \mathbf{N}$，令$H_\varphi$为那些$f \in G_{mn}$中的集合，使得$d'(f(a_k), b_{\varphi(k)}) \leq 1/n$对应于$1 \leq k \leq p(m)$。 由$b_r$的定义，$G_{mn}$为$\varphi \in \mathbf{N}^{p(m)}$为集合$H_\varphi$并；令$C_{mn}$为映射$\varphi \in \mathbf{N}^{p(m)}$的集合，使得$H_\varphi \neq \emptyset$，并且对于每个$\varphi \in C_{mn}$令$g_\varphi$为$H_\varphi$的元素；最后，让$L_{mn}$表示$g_\varphi$对于$\varphi \in C_{mn}$的可数集合。 令$f \in G_{mn}$，并令$\varphi$为$C_{mn}$的元素，使得$f \in H_\varphi$；那么从定义可以立即得出，所有 $x \in X$ 都有 $d'(f(x), g_\varphi(x)) \leq 4/n$，即 $\delta(f, g_\varphi) \leq 4/n$。 因此，集合$L_{mn}$的并在$\mathscr{C}_u(X; Y)$中是稠密的，因为对于每个整数$n > 0$和每个$f \in \mathscr{C}(X; Y)$，都存在$m$使得$f \in G_{mn}$，并且我们刚刚看到从$f$到$L_{mn}$的距离是$\leq 4/n$。

b) 设 $I = [0, 1]$。由于$\mathscr{C}_u(X; I)$是$\mathscr{C}_u(X; \mathbf{R})$的一致子空间，因此它是可数的型。令$(f_n)$为序列，它在$\mathscr{C}_u(X; I)$中是稠密的。考虑$X$的乘积空间$K = \mathbf{N}$和映射$\psi : x \to (f_n(x))$进入$K$，这显然是连续的。 映射 $\psi$ 是单射；因为，对于所有$n$，通过序列$(f_n)$、关系$f_n(x) = f_n(x')$的定义意味着，在经过到极限上，对于每个函数$f \in \mathscr{C}(X; I)$，$f(x) = f(x')$；但如果 $x \neq x'$ 凭借公理 (OIV) 应用于点 $x$ 和 $x$ 的邻域 $V$，而包含 $x'$ (章 IX, § 1, no. 5， 定理2)。由此可见，紧凑空间 $X$ 同胚于 $K$ 的子空间 $\psi(X)$ (章 I, § 9, no. 4, 定理 2, 推论 2)；因为 $K$ 是可度量的并且型是可数的，所以 $\psi(X)$ 也是可数的，因而 $X$ 也是可数的。

Q.E.D.

#### 推论 {#top-x-s3-n3-cor-1 .statement tag=0CDM}

令$X$为局部紧致空间，其拓扑承认可数基，并令$Y$为可数型的可度量均匀空间。

a) $X$的连续映射进入$Y$，极限无穷大，空间$\mathscr{L}$，赋予$X$一致收敛的拓扑，是可数的可度量空间型。

b) $X$的连续映射到$Y$的空间$\mathscr{C}_c(X; Y)$，赋予拓扑紧收敛性，是可数型的可度量空间。

a) 令$X'$为将点无限邻接至$X$所获得的紧空间（章I, § 9, no. 8，定理4）；通过定义，每个函数$f \in \mathscr{L}$都可以唯一地扩展到连续的函数$\overline{f} : X' \to Y$，因而$f \to \overline{f}$是L的双射到$C(X'; Y)$；而这个双射是空间L通过§ 1, no. 6的命题6到$C_u(X'; Y)$的同胚。由于 $X'$ 是可度量的（章 IX, § 2, no. 9、命题 16、推论），因此结果来自定理 1，应用于 $X'$ 和 Y。

b) 设$(U_n)$是相对紧开集合覆盖X，使得X的每个紧致子集都包含在一些$U_n$中（章I, § 9, no. 9，命题15， 推论1)。如果$S$是$\overline{U}_n$的集合，则$C(X; Y)$上紧致收敛的拓扑与$S$收敛的拓扑相同。因而 ($§ 1,$ no. 2, 注 3) 空间 $C_c(X; Y)$ 同胚于乘积 $\prod_n C_u(\overline{U}_n; Y)$ 的子空间；因为每个紧凑空间$\overline{U}_n$都有一个可数基，所以它是可度量的（章IX, § 2, no. 9，命题16）；因而，每个 $C_u(\overline{U}_n; Y)$ 都是可度量的，并且可以通过定理 1 可数型，因而 $C_c(X; Y)$ 也是如此。

请注意，$\mathbf{R}$上所有有界连续实值函数的空间，赋予拓扑一致收敛性，不是可数的型（习题4）。

### 4. 紧凑开放式拓扑

#### 定理 2 {#top-x-s3-thm-2 .statement tag=0CDN}

*设X为拓扑空间，Y为均匀空间。对于 X 的每个紧致子集 K 和 Y 的每个开子集 U，让 T(K, U) 表示所有连续映射 $u : X \to Y$ 的集合，使得 $u(K) \subset U$。然后 $C(X; Y)$ 上的集合 $T(K, U)$ 生成拓扑紧凑收敛。*

令 $Y'$ 为与 Y (章 II, § 3, no. 8) 相关的豪斯多夫均匀空间，并令 $i : Y \to Y'$ 为 Y 在 $Y'$ 上的典范映射。紧致收敛的拓扑是最粗糙的拓扑，其中$C(X; Y)$到$C_u(K; Y')$的映射$u \to (i \circ u)|K$是连续的，因为K遍历X的所有紧致子集的集合（$§ 1,$） no. 4、命题 4)。因此，我们通过对X的每个紧凑子集 K取$C_c(K; Y')$的拓扑子基，然后在这些子基中的逆像中取并[在$\mathfrak{B}(C(X; Y))$]，从而获得$C_c(X; Y)$的拓扑子基$C(X, Y)$。另一方面，Y 的每个开子集都是形式 $\overline{i}^{-1}(U')$，其中$U'$ 在$Y'$ 中开路（章 II, § 3, no. 7，命题 12）；因此，对于每个紧凑子集$K' \supset K$，$T(K, \overline{i}^{-1}(U'))$是映射下$T(K, U')$的逆像

$$
C(X; Y) \to C_a(K'; Y').
$$

因此，当X是*紧*且Y是*Hausdorff*时，我们仍然需要证明定理；从现在开始我们要做这些假设。

我们首先证明$T(K, U)$在$C_c(X; Y)$开放。令$u_0$为这个集合的点；由于$u_0(K)$是紧致的（章I, § 9, no. 4、定理2、推论1）并且包含在开集合$U$中，因此存在$Y$的对称周边$V$使得$V(u_0(K)) \subset U$ （章II, § 4, no. 3、命题4、推论）。令$W$为所有连续映射$u : X \to Y$的$C_c(X; Y)$由……组成中$u_0$的邻域，使得$(u(x), u_0(x)) \in V$对于所有$x \in K$。对于这样的映射，我们显然有$u(K) \subset V(u_0(K)) \subset U$；因此$u \in T(K, U)$，因此$W \subset T(K, U)$，这证明了我们的断言。

相反，如果$W$是点$u_0 \in C_c(X; Y)$的邻域，让我们证明形式$T(K, U)$的邻域的有限数的$W$包含交。我们可以假设$W$是所有$u \in C(X; Y)$中的集合，这样$(u(x), u_0(x)) \in V$对于所有$x \in X$来说，$V$是$Y$的给定随从。由于$u_0$在$X$上连续，因此它是一致连续的（章II, § 4, no. 1，定理2）。设$V_1$是$Y$的对称周边，在$Y \times Y$开，使得$V_1^2 \subset V$。 $X$ 可以被紧集 $K_i$ ($1 \leq i \leq n$) 的有限数覆盖，使得每个$u_0(K_i)$ 都是$V_1$-小($1 \leq i \leq n$)。令$U_i$为开集合$V_1(u_0(K_i))$，并令$u : X \to Y$为包含在$n$集合$T(K_i, U_i)$的交中的连续映射（即邻域 $u_0$）。然后，对于每个$x \in K_i$，$u(x)$属于到$U_i$，因此$u_0(x)$和$u(x)$是$V_1^2$-闭，因此$V$-闭。由于每个$x \in X$属于到一些$K_i$，我们有$u \in W$并且证明是完整的。

这个结果使我们得出以下定义：

#### 定义 1 {#top-x-s3-def-1 .statement tag=0CDO}

*令$X, Y$为两个拓扑空间，不一定可统一。对于$X$的每个紧致子集$K$和$Y$的每个开子集$U$，令$T(K, U)$为所有$u \in C(X; Y)$的集合，使得$u(K) \subset U$。由集合 $T(K, U)$生成的$C(X; Y)$上的拓扑称为紧致收敛的拓扑或紧致开拓扑；我们用$C_c(X; Y)$表示通过赋予$C(X; Y)$以拓扑获得的拓扑空间。*

如果$Y$是统一的空间，则从定理2可以得出，这个定义与§ 1, no. 3中给出的一致。

如果$H$是$C(X; Y)$的子集，我们可以说由$C_c(X; Y)$在$H$上诱导的拓扑是$H$上的紧开拓扑。

#### 例{#top-x-s3-n4-exa-1 .statement tag=0CDP}

令$\mathbf{R}$中的$I$为区间$[0, 1]$。如果$Y$是任何拓扑空间，则空间$C_c(I; Y)$称为$Y$中路径*的*空间。对于路径$u$的$C_c(I; Y)$由……组成的每个$y \in Y$、子空间$\Omega_y(Y)$，使得$u(0) = u(1) = y$称为循环*空间（在$Y$中）*在点*$y$。

#### 注 1 {#top-x-s3-n4-rem-1 .statement tag=0CDQ}

同样，由$Y^X = \mathscr{F}(X; Y)$上的乘积拓扑在$C(X; Y)$上诱导的拓扑被称为逐点收敛的*拓扑*（$Y$不一定是可一致的）；它是由形式$T(\{x\}, U)$的集合生成的，因为$x$穿过$X$，$U$穿过$Y$的所有开子集的集合，因此它比紧凑开拓扑更粗糙。我们推断，*如果 $Y$ 是 Hausdorff，空间 $C_c(X; Y)$ 是 Hausdorff* (章 I, § 8, no. 1, 命题 5, 推出)。

#### 注 2 {#top-x-s3-n4-rem-2 .statement tag=0CDR}

令$\mathscr{S}$为$Y$的拓扑的子底，并令$\mathscr{K}$为$X$的紧凑子集的集合，其中性质如下：

(R) 如果$L$是$X$的任何紧致子集，并且$V$是$L$的任何邻域，则存在集合$K_i \in \mathscr{K}$的*有限*数使得$L \subset \bigcup_i K_i \subset V$。

然后集合$T(K, U)$，其中$K \in \mathscr{K}$和$U \in \mathscr{S}$，形式是$C(X; Y)$上紧凑开放拓扑的*子库*。为了证明这一点，我们必须证明，如果$L$是$X$的任意紧子集和$V$$Y$的任意开子集，并且如果$u \in T(L, V)$，则存在对$(K_i, U_i)$的有限数，使得$K_i \in \mathscr{K}$、$U_i \in \mathscr{S}$ 和 $u \in \bigcap_i T(K_i, U_i) \subset T(L, V)$。 注首先，对于$\mathscr{S}$的集合的每个有限序列$(s_k)$以及$X$的每个紧凑子集$M$，我们有$T\left(M, \bigcap_k S_k\right) = \bigcap_k T(M, S_k)$乘定义。因此，我们首先可以将替换$\mathscr{S}$乘以$\mathscr{S}$的集合的有限交的集合，即我们可以假设$\mathscr{S}$是$Y$的拓扑的*基*。到假设，$u(L)$是拟紧的并且包含在$V$中，因此存在包含在覆盖$u(L)$的$V$中的集合$U_i \in \mathscr{S}$的有限数。

集合$\overline{u}^{-1}(U_i)$在$X$打开并覆盖$L$。因此，对于每个$x \in L$，$L$中都有一个$x$的紧凑邻域$N_x$，包含在$\overline{u}^{-1}(U_i)$中的某个中。我们可以用这些集合 $N_{x_j} = L_j$ 中的有限数覆盖 $L$；对于每个$j$，让我们用$i(j)$表示指标$i$之一，这样$L_j \subset \overline{u}^{-1}(U_i)$。因此，对于每个指标$j$，[通过（R）]存在集合$K_{jk} \subset \overline{u}^{-1}(U_{i(j)})$、属于到$\mathscr{K}$的有限数，其中覆盖了$L_j$。对于每个$v \in \bigcap_{j,k} T(K_{jk}, U_{i(j)})$，我们有$\bigcup_k v(K_{jk}) \subset U_{i(j)}$，因此有$v(L_j) \subset U_{i(j)}$和$v(L) = \bigcup_j v(L_j) \subset \bigcup_j U_{i(j)} \subset V$；这样我们的断言就被证明了。

#### 定理 3 {#top-x-s3-thm-3 .statement tag=0CDS}

*令$X, Y, Z$为三个拓扑空间，令$f$为$X \times Y$到$Z$的映射。如果$f$是连续的，那么$\tilde{f}: x \to f(x, .)$是$X$到$C_c(Y; Z)$的连续映射。如果 $Y$ 是局部紧凑的，则逆命题为真。*

假设$f$是连续的。为了证明$\tilde{f}$是连续的，我们必须证明，对于$Y$的每个紧致子集$K$和$Z$的每个开子集$U$，$\tilde{f}$下$T(K, U)$的逆像$V$是开的$X$。令 $x_0 \in V$；对于每个$y \in K$，我们有$f(x_0, y) \in U$，并且由于$f$是连续的，因此在$X$中存在$x_0$的邻域$V_y$，在$Y$中存在$y$的邻域$W_y$，这样那个$f(V_y \times W_y) \subset U$。由于$K$是紧致的，因此存在点$y_i \in K$的有限数，使得集合$W_{y_i} (1 \leq i \leq n)$覆盖$K$。设$V'$为$x_0$的邻域$V_{y_i}$的交，即$x_0$的邻域；如果$x \in V'$和$y \in K$，我们有$f(x, y) \in U$，因为$y$包含在$W_{y_i}$中的某个中，并且$x$包含在每个$V_{y_i}$中；因而$V' \subset V$，因而$V$是其每个点的邻域，因此在$X$中开路。

相反，假设 $\tilde{f}$ 是连续的并且 $Y$ 是局部紧致的，让我们证明 $f$ 是连续的。设$x_0 \in X$、$y_0 \in Y$、$U$为$Z$中$f(x_0, y_0)$的开邻域；我们将证明$X$中有$x_0$的邻域$V$，$Y$中有$y_0$的邻域$W$，使得$f(V \times W) \subset U$。由于$y \to f(x_0, y)$是连续的，因此存在$y_0$的*紧凑*邻域$W$使得$f(\{x_0\} \times W) \subset U$。另一方面，由于 $\tilde{f}$ 是连续的，集合 $V$ of $x \in X$ 使得 $f(x, .) \in T(W, U)$ [即这样，对于所有$y \in W$]，$f(x, y) \in U$是$X$的开子集，因此邻域是$x_0$；我们有$f(V \times W) \subset U$。

Q.E.D.

#### 推论 1 {#top-x-s3-thm-3-cor-1 .statement tag=0CDT}

*令$X$为空间的局部紧致空间，$Y$为$C(X; Y)$的拓扑空间，$H$子集。那么$H$上的紧开拓扑是最粗糙的，其中$H \times X$到$Y$的映射$(u, x) \to u(x)$是连续的。*

因为，到定理 3，这个映射是连续的当且仅当典范嵌入$H \to C_c(X; Y)$是连续的。

#### 注 3 {#top-x-s3-n4-rem-3 .statement tag=0CDU}

令$X$为局部紧致空间，$Y$为豪斯多夫拓扑空间。如果$\mathscr{T}$在$C(X; Y)$的子集$H$上是拓扑，使得映射$(u, x) \to u(x)$在$H \times X$上连续，并且如果$H$相对于$\mathscr{T}$是*紧凑*，则$\mathscr{T}$ 是紧凑开放式拓扑。因为它比后者更细多了推论1，并且由于紧开拓扑是Hausdorff，因此两种拓扑是相同的。请注意，如果在加法 $Y$ 中是*完全正则*，则 $H$ 对于与 $Y$ 的拓扑兼容的每个均匀性（§ 2, no. 5、定理 2、推论 3）以及每个紧致来说都是“等连续”的子集$K$共$X$集合

$$
H(K) = \bigcup_{x \in K} H(x)
$$

是紧凑的，因为它是连续映射 $(u, x) \to u(x)$ 下的 $H \times K$ 的像。

#### 推论 2 {#top-x-s3-thm-3-cor-2 .statement tag=0CDV}

*令$X, Y, Z$为三个拓扑空间，使得$X$是豪斯多夫且$Y$是局部紧致的。那么规范双射 $\mathscr{F}(X \times Y; Z) \to \mathscr{F}(X; \mathscr{F}(Y; Z))$ (集合理论, R, § 4, no. 14) 的限制到$C(X \times Y; Z)$是$C_c(X \times Y; Z)$到$C_c(X; C_c(Y; Z))$的同胚。*

这个限制肯定是双射

$$
\rho : \mathscr{C}(X \times Y; Z) \to \mathscr{C}(X; \mathscr{C}_c(Y; Z))
$$

定理 3；因此，仍然需要证明，$\mathscr{C}(X \times Y; Z)$上的紧凑开拓扑是$\mathscr{C}(X; \mathscr{C}_c(Y; Z))$上的紧凑开拓扑的$\rho$下的逆像。由于集合$T(K, U)$，其中$K$是$Y$的紧子集，$U$是$Z$的开子集，形式是$\mathscr{C}_c(Y; Z)$的拓扑的子底，因此可以得出注 2 $\mathscr{C}_c(X; \mathscr{C}_c(Y; Z))$的拓扑是由形式$T(J, T(K, U))$的集合生成，其中$K$和$U$如上，$J$是$X$的紧凑子集。现在$\rho$下的$T(J, T(K, U))$的像恰好是$T(J \times K, U)$，因此是开集合；所以我们证明了 $\rho$ 是连续的。为了证明$\rho$是同胚，我们首先注意到$X \times Y$中形式$J \times K$的集合（其中$J$是$X$的紧致子集，$K$是子集的紧致） $Y$) 注 2 的满足条件 (R): 因为如果 $L$ 是$X \times Y$ 的紧子集并且$V$ 是 $L$ 的邻域 $X \times Y$、投影 $M = \operatorname{pr}_1(L)$、$N = \operatorname{pr}_2(L)$ 是紧致的，因为 $X$ 和 $Y$ 是 Hausdorff，并且 $V \cap (M \times N)$ 是紧致空间 $M \times N$ 中 $L$ 的邻域，使得$L$的每个点在形式$J \times K \subset V$的$M \times N$中都有邻域，其中$J \subset M$和$K \subset N$是紧致的；由于$L$可以被这些邻域中的有限数覆盖，断言被证明。因此形式$T(J \times K; U)$的集合，其中$J$是$X$的紧致子集，$K$是$Y$的紧致子集，$U$是子集的开子集 $Z$，生成拓扑共$\mathscr{C}_c(X \times Y; Z)$。但我们已经看到，$\rho$下的$T(J \times K, U)$的像是$\mathscr{C}_c(X; \mathscr{C}_c(Y; Z))$中的开集合$T(J, T(K, U))$；因此 $\rho$ 是同胚。

请注意，如果假设加法 $Z$ 是可统一的，则推论 2 是 § 1, no. 4、命题 2 的平凡推论。

#### 命题 9 {#top-x-s3-prop-9 .statement tag=0CDW}

*令$X, Y, Z$为三个拓扑空间，$Y$为局部紧致。那么$\mathscr{C}_c(X; Y) \times \mathscr{C}_c(Y; Z)$到$\mathscr{C}_c(X; Z)$的映射$(u, v) \to v \circ u$是连续的。*

我们必须证明，对于$X$的每个紧凑子集$K$和$Z$的每个开子集$U$，对$(u, v)$的集合$R$，使得$v(u(K)) \subset U$在$\mathscr{C}_c(X; Y) \times \mathscr{C}_c(Y; Z)$。让$(u_0, v_0) \in R$；则$u_0(K)$是局部紧致空间$Y$的紧致子集，包含在开集合$\overline{v_0^{-1}}(U)$中，因此$\overline{v_0^{-1}}(U)$中包含$u_0(K)$的紧致邻域$L$ （章I, § 9, no. 7，命题10）。所有$u \in \mathscr{C}_c(X; Y)$中的集合$V$使得$u(K) \subset L$是$u_0$的邻域，并且所有$v \in \mathscr{C}_c(Y; Z)$中的集合$W$使得$v(L) \subset U$是邻域 $v_0$；此外，关系$(u, v) \in V \times W$意味着$v(u(K)) \subset U$。于是就有了这样的结果。

### 5. 同胚群的拓扑

#### 命题 10 {#top-x-s3-prop-10 .statement tag=0CDX}

令$X$为一致的空间，并令$H$为$X$自身同胚的等连续集合。如果$H$和$H^{-1}$赋予$X$逐点收敛的拓扑，则$H^{-1}$的映射$u \to u^{-1}$在$H$上是连续的。

足以证明，对于每个$x_0 \in X$，$H^{-1}$到$X$的映射$u \to u^{-1}(x_0)$在每个点$u_0 \in H^{-1}$是连续的。设$V$是$X$的对称周边，并设$y_0 = u_0^{-1}(x_0)$。到假设时，存在$X$的对称随行人员$U$，使得关系$(x, x_0) \in U$意味着所有$u \in H^{-1}$的$(u^{-1}(x), u^{-1}(x_0)) \in V$。取元素$u \in H^{-1}$，即$W(\{y_0\}, U)$-接近$u_0$；那么我们就有$(u(y_0), u_0(y_0)) \in U$，即$(u(y_0), x_0) \in U$。由此可见$(y_0, u^{-1}(x_0)) \in V$，即$(u_0^{-1}(x_0), u^{-1}(x_0)) \in V$；这样就完成了证明。

#### 推论 {#top-x-s3-n5-cor-1 .statement tag=0CDY}

令$X$为一致的空间，并令$H$为$X$自身同胚的等连续群。那么$X$中逐点收敛的拓扑与$H$中的群结构兼容。

这是命题 10 中的推论，以及§ 2, no. 1、命题 1、推论 5。

#### 命题 11 {#top-x-s3-prop-11 .statement tag=0CDZ}

令$X$为紧空间，令$\Gamma$为$X$自身同胚的群。那么$X$中一致收敛的拓扑与$\Gamma$中的群结构兼容。

我们已经知道（no. 4，命题 9）$\Gamma \times \Gamma$到$\Gamma$的映射$(u, v) \to v \circ u$相对于这个拓扑是连续的；因此我们必须证明$u \to u^{-1}$在$\Gamma$的每一个点$u_0$都是连续的。由于$u_0^{-1}$在$X$上一致连续，给定$X$的任何对称周边$V$，存在$X$的周边$W$，使得关系$(x, x') \in W$蕴含$(u_0^{-1}(x), u_0^{-1}(x')) \in V$。因此，如果$u \in \Gamma$对于所有$x \in X$来说是$(u_0(x), u(x)) \in W$，那么对于所有$x \in X$来说$(x, u_0^{-1}(u(x))) \in V$是这样的，因此（因为$u$是双射）对于所有$x \in X$来说$(u^{-1}(x), u_0^{-1}(x)) \in V$。这样就完成了证明。

现在令 $X$ 为局部紧致空间，令 $\Gamma$ 为 $X$ 自身同胚的群。 $X$中紧致收敛的拓扑不一定与$\Gamma$（习题17）的群结构兼容。让$X'$表示通过在无穷大$\omega$到$X$处邻接点获得的紧凑空间。 $X$ 的每个同态 $u$ 自身扩展与 $X'$ 的同态 $u'$ 自身唯一，使得 $u'(\omega) = \omega$ (章 I, § 10, no. 3, 推论到命题 7)，因此$\Gamma$可以与$X'$自身同胚的群$\Gamma'$中的子群，以及使$\omega$固定的所有同胚中的由……组成来识别。因此，由 $C_u(X'; X')$ 在 $\Gamma$ 上引发的拓扑与 $\Gamma'$ (命题 11) 的群结构兼容，并且 $\Gamma$ 在 $\Gamma'$ 中闭合 [相对于由拓扑引发的拓扑 $C_u(X'; X')$] 因为它是由方程$u(\omega) = \omega$ (§ 1, no. 2, 注 6) 定义的。我们用在$\Gamma$上定义的$\mathscr{T}_\beta$群拓扑表示；它是紧收敛的更细比拓扑，并且还可以（凭借§ 1, no. 6，命题6）被定义为$X$上一致收敛的拓扑，当$X$被赋予由$X'$的唯一均匀性引起的均匀性时。

拓扑 $\mathscr{T}_\beta$ 可以表征如下：

#### 命题 12 {#top-x-s3-prop-12 .statement tag=0CE0}

*在局部紧致空间$X$的所有同胚的群$\Gamma$上，拓扑$\mathscr{T}_\beta$是最粗糙的，其中映射$u \to u$和$u \to u^{-1}$入$\Gamma$ $C_c(X; X)$ 是连续的。*

让我们暂时用 $\mathscr{C}'$ 来表示后者拓扑。由于$u \to u^{-1}$相对于$\mathscr{T}_\beta$是连续的，并且由于紧致收敛性$\mathscr{T}_\beta$比拓扑更更细，所以很明显$\mathscr{T}_\beta$比$\mathscr{C}'$更更细。为了证明逆命题，赋予$X'$独特的均匀性；设$u_0 \in \Gamma$和$V$为$X'$的随从；那么我们必须证明存在一个$X$的紧致子集$K$和一个$X'$的对称周边$W$使得关系

$$
u \in \Gamma, \ (u_0(x), u(x)) \in W \text{ and } (u_0^{-1}(x), u^{-1}(x)) \in W \text{ for all } x \in K
$$

暗示

$$
(u_0(x), u(x)) \in V \text{ for all } x \in X.
$$

设$V_1$是$X'$的对称开环，使得$\overset{2}{V}_1 \subset V$；那么$K_1 = X' - V_1(\omega)$是$X$的紧致子集。 选择 $X'$ 的对称开放周边$W$，使得$W \subset V$ 和$W(\omega) \cap W(u_0^{-1}(K_1)) = \emptyset$；这可以通过章 II, § 4, no. 3 中的命题 4 实现。让$K_2 = X' - W(\omega)$，它是$X$的紧凑子集。我们将看到 $W$ 和紧集 $K = K_1 \cup K_2$ 执行所需操作。从$W \subset V$开始，足以证明关系

$$
(u_0^{-1}(x), u^{-1}(x)) \in W \text{ for all } x \in K_1 \quad (u \in \Gamma)
$$

意味着

$$
(u(y), \omega) \in V_1 \text{ for all } y \in W(\omega);
$$

因为我们也将有$(u_0(y), \omega) \in V_1$，然后

$$
(u_0(y), u(y)) \in \overset{2}{V}_1 \subset V
$$

对于所有$y \in W(\omega) = X' - K_2$。现在如果我们有 $y \in W(\omega)$ 并且

$$
u(y) \in X' - V_1(\omega) = K_1,
$$

由此可知$y \in u^{-1}(K_1) \subset W(u_0^{-1}(K_1))$，与$W$的选择相反；因此证明是完整的。

一般来说，群$\Gamma$，赋予$\mathscr{T}_\beta$，不是局部紧致的；但我们有以下标准：

#### 定理 4 {#top-x-s3-thm-4 .statement tag=0CE1}

*令$G$为局部紧致空间$X$的所有同胚中群$\Gamma$的子群。假设在空间$C_c(X; X)$中，存在恒等映射$e$的邻域$V$，使得$V \cap G = H$在$G$中对称，在$C_c(X; X)$中相对紧。那么$\Gamma$中$G$相对于拓扑$\mathscr{T}_\beta$的闭包$\overline{G}$是由$\mathscr{T}_\beta$引发的关于拓扑的局部紧致群；在$\overline{G}$上导出的这个拓扑与紧致收敛的拓扑相同，$C_c(X; X)$中$H$的闭包$\overline{H}$相对于此拓扑来说是$\overline{G}$中$e$的邻域。

让我们首先证明$\overline{H}$包含在$\Gamma$中，并且$\mathscr{T}_\beta$在$\overline{H}$上诱导的拓扑*与紧致收敛的拓扑相同*。设 $u_0 \in \overline{H}$；因此，$C_c(X; X)$ 中的$u_0$ 是$H$ 上的超滤器$\Phi$ 的极限。由于$\Phi^{-1}$（$u \to u^{-1}$下$\Phi$的像）是$H \subset \overline{H}$上的超滤器基，它收敛于$C_c(X; X)$的紧凑子空间$\overline{H}$到元素$v_0$。 映射$(u, v) \to uv$相对于$\Phi \times \Phi^{-1}$收敛到$u_0 v_0$（no. 4，命题9）； *更不必说*，$u \to uu^{-1} = e$相对于$\Phi$收敛到$u_0 v_0$，因此$u_0 v_0 = e$，因为$C_c(X; X)$是Hausdorff。同样$v_0 u_0 = e$；因此$u_0$是$X$的同胚，即$u_0 \in \Gamma$。因此$\overline{H}$包含在$\Gamma$中。此外，这个论证表明$\overline{H}^{-1} = \overline{H}$，并且对于$\overline{H}$上的每个超滤器$\Phi$收敛到$u_0$，$\Phi^{-1}$在$C_c(X; X)$收敛到$u_0^{-1}$；因此，当$\overline{H}$带有紧收敛的拓扑时，$\overline{H}$到$C_c(X; X)$的映射$u \to u^{-1}$是连续的（章I, § 7, no. 4，命题9，推论1）。 命题 12 则表明，在$\overline{H}$ 上，紧致收敛的拓扑与$\mathscr{T}_\beta$ 引起的拓扑相同。

此外，由于$\Gamma$上的拓扑$\mathscr{T}_\beta$是更细比紧致收敛的拓扑，所以$\overline{H}$也是$H$相对于$\mathscr{T}_\beta$的闭包。但$H$相对于紧收敛的拓扑，是$G$中$e$的邻域，以及$\mathscr{T}_\beta$相对于拓扑的*更不必说*；由此可见 (章 I, § 3, no. 1, 命题 2) $\overline{H}$ 是 $\overline{G}$ 中$e$ 的邻域，相对于$\mathscr{T}_\beta$ 引发的拓扑，因此 $\overline{G}$ 在此是局部紧致的拓扑。如果$W$是$V$相对于拓扑紧致收敛的内部，则$W \cap \Gamma$在$\mathscr{T}_\beta$中开，因此$W \cap \overline{G}$包含在$H = V \cap G$相对于$\mathscr{T}_\beta$的闭包中（章） I, § 1, no. 6、命题5)；这表明，相对于紧致收敛的拓扑，$\overline{H}$也是$\overline{G}$中$e$的邻域。最后，对于 $C_c(X; X)$ 的每个 $u_0 \in \Gamma$、双射、$v \to u_0 \circ v$ 和 $v \to u_0^{-1} \circ v$ 其自身都是连续的 (no. 4、命题 9)，因此，如果 $u_0 \in \overline{G}$、$u_0 \overline{H}$ 是邻域 $\overline{G}$ 中的 $u_0$ 相对于拓扑的紧致收敛。这样就完成了证明。

#### 推论 {#top-x-s3-n5-cor-2 .statement tag=0CE2}

*令$G$为局部紧致空间$X$的同胚的群。如果$C_c(X; X)$中$G$的闭包$\overline{G}$是紧的，则$\overline{G}$是$X$同胚的群，紧收敛的拓扑与$\overline{G}$的群结构兼容，因此是紧拓扑群.*

局部紧致空间 $X$ 的同胚的群是局部紧致的，但相对于紧致收敛的拓扑不是紧致的，由于章 I, § 9, no. 7、命题 12，在 $C_c(X; X)$ 中*局部封闭*，*但不一定关闭*。

例如，在$\mathbf{R}^n$的自同态的环$\mathscr{L}(\mathbf{R}^n)$中，用平方$n \times n$矩阵的环$M_n(\mathbf{R})$超过$\mathbf{R}$进行识别，并赋予紧凑的拓扑收敛，群$GL(n, \mathbf{R})$，用非奇异矩阵的群来识别，是局部紧致但密集的（章VI, § 1, no. 6，命题6）。

### 习题{#top-x-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
