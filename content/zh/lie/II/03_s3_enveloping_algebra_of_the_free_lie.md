---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 3
section_title: Enveloping algebra of the free Lie algebra
lang: zh
source: lie-i-iii
book_pages: 136-142, 186-187
pdf_pages: 0154-0160, 0204-0205
extraction: ocr
subsections:
    - "no": 1
      title: ENVELOPING ALGEBRA OF $L(X)$
      page: 136
      pdf_page: 154
    - "no": 2
      title: PROJECTOR OF $A^+(X)$ ONTO $L(X)$
      page: 138
      pdf_page: 156
    - "no": 3
      title: DIMENSION OF THE HOMOGENEOUS COMPONENTS OF L(X)
      page: 140
      pdf_page: 158
statements: 11
exercises: 4
content_sha256: 330aa833f60978584692ff021c355835a414a4d2aa6a9c625e8d9a80cf44a19c
translated_from: content/en/lie/II/03_s3_enveloping_algebra_of_the_free_lie.md
translation_method: google
source_content_sha256: 1d39611cf30ae9228e327035d9d7254aba6ff04ead058f79653b16b5bbbadc54
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 389e7b6e5a8214fc104f226850e1d6eab76d00ccdfd8b01a71ecb95eae76a6de
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。包围免费李代数的代数

在本段中，$A(X) = A_K(X)$表示集合$X$在环$K$上的自由结合代数Libas(X) (代数、章III, § 2, no. 7、定义) 2）。 $X$ 与$A(X)$ 中的典范像进行识别；回想一下，$K$-模块$A(X)$承认从$X$派生的自由幺半群$Mo(X)$为基； $A^+(X)$表示由非空字生成的$A(X)$的子模。

### 1. 包络代数的 $L(X)$

#### 定理 1 {#lie-ii-s3-thm-1 .statement tag=0A42}

*令*$\alpha : L(X) \to A(X)$*成为唯一的李代数同态将*$X$*的典范嵌入延伸到*$A(X)$*(§ 2, no. 2,命题1)*。 *令* $\sigma : L(X) \to U(L(X))$ 为 $L(X)$ 的典范映射入其包络线代数，并令 $\beta : U(L(X)) \to A(X)$ 为唯一单位代数同态，使得 $\beta \circ \sigma = \alpha$ (章 I, § 2, no. 1, 命题) 1).然后：
(a) $\alpha$ 是单射的，$\alpha(L(X))$ 是 $A(X)$ 的直因子子模。
(b) $\beta$ 是双射的。

令B为B的X的单位K-代数和$\phi$映射；通过§ 2, no. 2的命题 1，存在李代数同态$\psi : L(X) \to B$使得$\psi | X = \phi$；通过章I, § 2, no. 1的命题1，存在一个单位代数同态$\theta : U(L(X)) \to B$使得$\theta \circ \sigma = \psi$因此使得$(\theta \circ \sigma) | X = \phi$。由于$\sigma(X)$生成是单位代数$U(L(X))$，同态$\theta$是唯一的单位代数同态满足后者条件。这表明有序对$(U(L(X)), \sigma | X)$是解，普遍映射问题与$A(X)$相同；将$\phi$取X的典范嵌入代入$A(X)$，可推导出$\beta$为同构，从而证明(b)。

最后，由于$L(X)$是自由K-模（§ 2, no. 11，推论到定理1），$\sigma$是单射的，$\sigma(L(X))$是$U(L(X))$的直因子子模（章） I, § 2, no. 7、推论 3 至定理 1)。 By (b), this proves (a).

#### 推论 1 {#lie-ii-s3-thm-1-cor-1 .statement tag=0A43}

代数 $A(X)$ 上存在唯一的余积，使$A(X)$ 成为一个大数，使得X 的元素是原始的。此外，$\beta$是大数$U(L(X))$的同构到$A(X)$与这个大数结构。

这是从定理的断言(b)以及X生成单位代数$A(X)$的事实得出的。

从此以后，$A(X)$被赋予了这个大数结构，而$L(X)$则用$\alpha$下的像来识别，即用X生成的$A(X)$的谎言子代数来识别。

#### 推论 2 {#lie-ii-s3-thm-1-cor-2 .statement tag=0A44}

如果$K$是特征0的域，则$L(X)$是$A(X)$的原语元素的李代数。

这是从推论 1 和推论到 § 1, no. 5 的命题 9。

#### 注 {#lie-ii-s3-n1-rem-1 .statement tag=0A45}

(1) 设$K'$为交换环包含K。如果$A(X)$、$L(X)$和$L_{K'}(X)$与$A_{K'}(X)$的子集一致，我们可以从部分推出 (a) 定理 1 关系

$$
L(X) = L_{K'}(X) \cap A(X).
$$

(2) 如果仅假设环 K 的加法群无扭转，推论 2 至定理 1 仍然有效。首先假设$K = \mathbf{Z}$； $A(X)$ 的每个原语元素都是 $A_q(X)$ 的原语元素，因此位于 $L_q(X) \cap A(X) = L(X)$ 中（推论 2 和公式 (1)）。一般情况下，K 在 $\mathbf{Z}$ 上是平坦的，我们应用 § 1, no. 2 的注 2 和 § 2, no. 5 的命题 3。

(3) 令$\Delta$为可交换幺半群，将$X$的$\phi_0$映射转化为相关幺半群的$\Delta$和$\phi : Mo(X) \to \Delta$同态；如果$A(X)$被赋予*代数*、章III, § 3, no. 1、*例* 3中定义的毕业$(A^\delta(X))_{\delta \in \Delta}$以及$L(X)$在§ 2, no. 6中定义的毕业$(L^\delta(X))_{\delta \in \Delta}$，我们立即有，对于$\delta \in \Delta$， $L^\delta(X) \subset L(X) \cap A^\delta(X)$。由于$L$是$\delta \in \Delta$的$L^\delta(X)$的和，而$\delta \in \Delta$的$L(X) \cap A^\delta(X)$的和是直接的，这意味着

$$
L^\delta(X) = L(X) \cap A^\delta(X).
$$

(4) 设$A$为单位结合律代数，且$t = (t_i)_{i \in I}$为元素和$A$的族。我们有图表

$$
\begin{array}{ccc}
L(I) & \xrightarrow{f_t} & A \\
i \downarrow & & \downarrow g_t \\
A(I)
\end{array}
$$

其中$i$是典范嵌入，$f_t$是李代数同态，由$t$定义，$g_t$是单位代数同态，使得$g_t(i) = t_i$代表$i \in I$。 图表对于 $g_t \circ i$ 和 $f_t$ 重合在 $I$ 上是可交换的。因此，如果 § 2, no. 4、重合中定义了 $P \in L(I)$、元素 $P((t_i)_{i \in I})$，而 *代数*、章 III, § 2, no. 8、*例* 中定义了元素 $P((t_i)_{i \in I})$ 2。

### 2. 投影算子 $A^+(X)$ 到 $L(X)$

令 $\pi$ 为 $A^+(X)$ 的线性映射到 $L(X)$ 定义为

$$
\pi(x_1 \ldots x_n) = (\operatorname{ad}(x_1) \circ \cdots \circ \operatorname{ad}(x_{n-1}))(x_n)
$$

$X$ 中的 $n > 0, x_1, \ldots, x_n$。

#### 命题 1 {#lie-ii-s3-prop-1 .statement tag=0A46}

(a) * $\pi$ 到 $L(X)$ 中的限制 $\pi_0$ 是 $L(X)$ 中的推导。*
(b) *对于整数$n \geq 1$以及$L^n(X)$、$\pi(u) = n.u$中的所有$u$。*

(a) 令$E$为模$L(X)$的内同态代数和$A(X)$的$\theta$同态进入$E$，使得$\theta(x) = \operatorname{ad} x$对于所有$x \in X$。 $\theta$到$L(X)$的限制是$L(X)$的李代数同态到$E$，其中$X$上的重合与$L(X)$的伴随表示， 从而

$$
\theta(u).v = [u, v] \quad \text{for } u, v \text{ in } L(X).
$$

设$a$在$A(X)$中，$b$在$A^+(X)$中；然后

$$
\pi(a.b) = \theta(a).\pi(b).
$$

考虑$a = x_1 \ldots x_p, \ b = x_{p+1} \ldots x_{p+q}$与$p \geq 0, q \geq 1$和$x_1, \ldots, x_{p+q}$在$X$中的情况就足够了；但 (5) 紧随 (3) 而来，因为 $\theta(x) = \operatorname{ad} x$ 对于 $x \in X$。

设$u$和$v$在$L(X)$中；由(4)和(5)，

$$
\pi_0([u, v]) = \pi(uv - vu) = \theta(u) \cdot \pi(v) - \theta(v) \cdot \pi(u)
= [u, \pi(v)] - [v, \pi(u)] = [u, \pi_0(v)] + [\pi_0(u), v],
$$

因此$\pi_0$是$L(X)$的推导。

(b) 设$\pi_1$为模$L(X)$的自同态，其中重合在$L^n(X)$上，乘法乘以整数$n \geq 1$。 公式 $[L^n(X), L^m(X)] \subset L^{n+m}(X)$ 显示 $\pi_1$ 为推导（*代数*、章 III, § 10, no. 3、*例* 6）。 $L(X)$的推导$\pi_1 - \pi_0$是$X$上的零，如$X$生成$L(X)$、$\pi_0 = \pi_1$、从而(b)。

#### 推论 {#lie-ii-s3-n2-cor-1 .statement tag=0A47}

*假设 K 是 Q 代数。令 P 为线性映射或 $A^+(X)$ 自身，使得*

$$
P(x_1 \ldots x_n) = \frac{1}{n} (\operatorname{ad} x_1 \circ \cdots \circ \operatorname{ad} x_{n-1})(x_n)
$$

*适用于X中的$n \geq 1$和$x_1, \ldots, x_n$。那么 P 就是 $A^+(X)$ 的投影算子到 $L(X)$。*

P的像包含在$L(X)$中。此外，对于 $L^n(X)$、$P(u) = \frac{1}{n} \pi(u)$、从而 $P(u) = u$ 中的所有 $n \geq 1$ 和所有 $u$ by 命题 1。

$$
L(X) = \sum_{n \geq 1} L^n(X),
$$

我们看到P到$L(X)$的限制是恒等式。

#### 注 {#lie-ii-s3-n2-rem-1 .statement tag=0A48}

假设 K 是特征零的域，并让 Q 是 $A(X) = U(L(X))$ 的投影算子到 $L(X)$，与 $U(L(X))$、cf. § 1, no. 5 的规范分级相关。 *对于$\alpha \in \mathbf{N}^{(X)}$，$Q(A^\alpha(X)) \subset L^\alpha(X)$。*只要验证Q的像和核的等级为$A(X)$的子模，等级为型$\mathbf{N}^{(X)}$即可。这对于像来说是显而易见的，它等于 $L(X)$。另一方面，令$n$为整数$\geq 1$。 $y^n$生成的$A(X)$的向量子空间，其中$y \in L(X)$，等于$\sum_{\sigma \in S_n} y_{\sigma(1)} y_{\sigma(2)} \cdots y_{\sigma(n)}$生成的$A(X)$的向量子空间，其中$y_1, y_2, \ldots, y_n$是齐次元素 $L(X)$；那么这个子空间就是$A(X)$的分级子模。

（请注意，如果 Card(X) $\geq 2$、投影算子 P 和 Q *不在 $A^+(X)$ 上实现重合*。让 $x, y$ 位于 X 和 $x \neq y$ 中并写入

$$
z = x[x, y] + [x, y]x = x^2y - yx^2.
$$

然后$Q(z) = 0$和$P(z) = \frac{1}{3}[x, [x, y]] \neq 0$、cf.§ 2, no. 10、*例*和no. 11、*定理* 1。）

### 3. L(X)的齐次分量的维数

令X为集合，$\mathbf{N}^{(X)}$的$\alpha$元素，且d整数 > 0。如果存在$\beta \in \mathbf{N}^{(X)}$使得$\alpha = d\beta$，则写为$d|\alpha$。 元素$\beta$是唯一的，则用$\alpha/d$表示。

#### 引理 1 {#lie-ii-s3-lem-1 .statement tag=0A49}

令 n 为整数 > 0，$T_1, \ldots, T_n$ 不确定，$u_1, \ldots, u_n$ 元素为 $\mathbf{Z}$。令 $(c(\alpha))_{\alpha \in \mathbf{N}^n - \{0\}}$ 为元素和 $\mathbf{Z}$ 的族，使得

$$
1 - \sum_{i=1}^n u_i T_i = \prod_{\alpha \neq 0} (1 - T^\alpha)^{c(\alpha)}.
$$

对于所有$\alpha \in \mathbf{N}^n - \{0\}$，

$$
c(\alpha) = \frac{1}{|\alpha|} \sum_{d|\alpha} \mu(d) \frac{(|\alpha|/d)!}{(\alpha/d)!} u^{\alpha/d}
$$

其中 $\mu$ 是莫比乌斯函数 (附录)。

公式 (7) 两边取对数 (代数, 章 IV, § 6, no. 9) 等价于：

$$
\log \left( 1 - \sum_{i=1}^n u_i T_i \right) = \sum_{\alpha \neq 0} c(\alpha) \log (1 - T^\alpha).
$$

现在

$$
-\log \left( 1 - \sum_{i=1}^n u_i T_i \right) = \sum_{j \geq 1} \frac{1}{j} \left( \sum_{i=1}^n u_i T_i \right)^j
$$
$$
= \sum_{j \geq 1} \frac{1}{j} \sum_{|\beta|=j} \frac{|\beta|!}{\beta!} u^\beta T^\beta
$$
$$
= \sum_{|\beta|>0} \frac{1}{|\beta|} \frac{|\beta|!}{\beta!} u^\beta T^\beta.
$$

另一方面

$$
-\sum_{\alpha \neq 0} c(\alpha) \log (1 - T^\alpha) = \sum_{|\alpha|>0, k \geq 1} \frac{1}{k} c(\alpha) T^{k\alpha}
$$
$$
= \sum_{|\beta|>0, k|\beta} \frac{1}{k} c\left( \frac{\beta}{k} \right) T^\beta.
$$

因此 (7) 等价于

$$
\sum_{k|\beta} \left| \frac{\beta}{k} \right| c\left( \frac{\beta}{k} \right) = \frac{|\beta|!}{\beta!} u^\beta \quad \text{for all } \beta \in \mathbf{N}^n - \{0\}.
$$

令 $\Lambda$ 为 $(\lambda_1, \lambda_2, \ldots, \lambda_n) \in \mathbf{N}^n - \{0\}$ 的集合，这样 g.c.d. $\lambda_1, \lambda_2, \ldots, \lambda_n$ 等于 1。 $\mathbf{N}^n - \{0\}$ 的每个元素都可以唯一地写成形式 $m\lambda$，其中 $m$ 是整数 $\geqslant 1$ 和 $\lambda \in \Lambda$。 条件 (12) 等价于

$$
\sum_{k|m} \left| \frac{m\lambda}{k} \right| c\left( \frac{m\lambda}{k} \right) = \frac{(m|\lambda|)!}{(m\lambda)!} u^{m\lambda} \quad \text{for all } \lambda \in \Lambda \text{ and all } m \geqslant 1.
$$

根据莫比乌斯反演公式 (附录)，条件 (13) 等价于

$$
|m\lambda| c(m\lambda) = \sum_{d|m} \mu(d) \frac{\left| \frac{m\lambda}{d} \right|!}{\left( \frac{m\lambda}{d} \right)!} u^{\frac{m\lambda}{d}}
$$

对于所有$\lambda \in \Lambda$和所有$m \geqslant 1$。

#### 定理 2 {#lie-ii-s3-thm-2 .statement tag=0A4A}

*令 $X$ 为有限集合和 $n = \mathrm{Card}(X)$。*

(a) *对于每个整数 $r \geqslant 1$，$K$-模块 $L^r(X)$ 不含秩*

$$
c(r) = \frac{1}{r} \sum_{d|r} \mu(d) n^{r/d},
$$

*其中$\mu$是莫比乌斯函数。*

(b) *对于所有$\alpha \in \mathbf{N}^X - \{0\}$，$K$-模块$L^\alpha(X)$ (§ 2, no. 6) 不包含秩*

$$
c(\alpha) = \frac{1}{|\alpha|} \sum_{d|\alpha} \mu(d) \frac{(|\alpha|/d)!}{(\alpha/d)!}.
$$

我们已经知道模$L^r(X)$（其中$r \in \mathbf{N}$）和$L^\alpha(X)$（其中$\alpha \in \mathbf{N}^X$）是免费的（§ 2, no. 11、推论到定理1）。考虑由$Mo(X)$的典范同态$\phi$定义为$\mathbf{N}^X$的多级渐变$A(X)$$(A^\alpha(X))_{\alpha \in \mathbf{N}^X}$ (*代数*, 章 III, § 3, no. 1, *例 3*);然后 $A^\alpha(X) \cap L(X) = L^\alpha(X)$ 乘以 no. 1 的 *注 3*。对于$\alpha \in \mathbf{N}^X$，$K$-模块$A^\alpha(X)$承认为字的基集合，其中$X$的每个字母$x$出现了$\alpha(x)$次。令$d(\alpha)$为这些字中的数，即$A^\alpha(X)$中的秩；我们将以两种不同的方式计算正式的幂级数

$$
P((T_x)_{x \in X}) \in \mathbf{Z}[[((T_x)_{x \in X})]]
$$

定义为

$$
P(T) = \sum_{\alpha \in \mathbf{N}^X} d(\alpha) T^\alpha.
$$

(1) 我们有

$$
P(T) = \sum_{m \in Mo(X)} T^{\phi(m)} = \sum_{r=0}^\infty \sum_{x_1, \ldots, x_r} T_{x_1} \cdots T_{x_r} = \sum_{r=0}^\infty \left( \sum_{x \in X} T_x \right)^r
$$

从而

$$
P(T) = \left( 1 - \sum_{x \in X} T_x \right)^{-1}.
$$

(2) 对于所有$\alpha \in \mathbf{N}^X - \{0\}$，令$(e_{\alpha,j})_{1 \leq j \leq c(\alpha)}$为$L^\alpha(X)$的基，并给出有序对$(\alpha, j)$的集合$I$，使得$\alpha \in \mathbf{N}^X - \{0\}$和$1 \leq j \leq c(\alpha)$有全序。由 no. 1 的定理 1 和庞加莱-伯霍夫-维特定理（章 I, § 2, no. 7、推出 3 至定理 1）、元素
$$
y_m = \prod_{(\alpha, j) \in I} (e_{\alpha, j})^{m(\alpha, j)},
$$
其中指标$m$穿过$\mathbf{N}^{(I)}$、形式基或$A(X)$。每个$y_m$都是多次$\sum_{(\alpha, j) \in I} m(\alpha, j) \alpha$。让 $u(m)$ 表示这个多次。由此可见
$$
P(T) = \sum_{m \in \mathbf{N}^{(I)}} T^{u(m)} = \sum_{m \in \mathbf{N}^{(I)}} \prod_{(\alpha, j) \in I} T^{m(\alpha, j)\alpha}
= \prod_{(\alpha, j) \in I} \sum_{r=0}^\infty T^{r\alpha} = \prod_{(\alpha, j) \in I} (1 - T^\alpha)^{-1},
$$
从而终于
$$
P(T) = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - T^\alpha)^{-c(\alpha)}.
$$
比较(18)和(19)，我们得到
$$
1 - \sum_{x \in X} T_x = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - T^\alpha)^{c(\alpha)}.
$$
引理 1 然后给出 (b)。

如果我们现在用相同的不确定 $U$ 替换公式 (20) 中的 $T_x$ $x \in X$，我们得到
$$
1 - nU = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - U^{|\alpha|})^{c(\alpha)} = \prod_{r > 0} (1 - U^r)^{c(r)}.
$$
再次应用引理1，我们推导出(a)。

#### 例 {#lie-ii-s3-n3-exa-1 .statement tag=0A4B}

我们有
$$
\begin{align*}
c(1) &= n, & c(2) &= \frac{1}{2}(n^2 - n), & c(3) &= \frac{1}{3}(n^3 - n), \\
c(4) &= \frac{1}{4}(n^4 - n^2), & c(5) &= \frac{1}{5}(n^5 - n), & c(6) &= \frac{1}{6}(n^6 - n^3 - n^2 + n).
\end{align*}
$$

#### 注 {#lie-ii-s3-n3-rem-1 .statement tag=0A4C}

令$X$为集合，并令$\alpha \in \mathbf{N}^{(X)}$；自由的 $K$ 模块 $L^\alpha(X)$ 的秩也由公式 (16) 给出。这紧随定理 2 (b) 和§ 2, no. 6 的命题 4。

### 习题{#lie-ii-s3-exercises}

字母$X$表示集合。

参见[习题为 § 3](exercises/s3/)。
