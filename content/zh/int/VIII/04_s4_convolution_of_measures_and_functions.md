---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 4
section_title: Convolution of measures and functions
lang: zh
source: int-vii-ix
book_pages: INT VIII.24-INT VIII.45, INT VIII.65-INT VIII.73
pdf_pages: 0124-0145, 0165-0173
extraction: ocr
subsections:
    - "no": 1
      title: Convolution of a measure and a function
      page: 24
      pdf_page: 124
    - "no": 2
      title: Examples of convolvable measures and functions
      page: 28
      pdf_page: 128
    - "no": 3
      title: Convolution and transposition
      page: 34
      pdf_page: 134
    - "no": 4
      title: Convolution of a measure and a function on a group
      page: 37
      pdf_page: 137
    - "no": 5
      title: Convolution of functions on a group
      page: 38
      pdf_page: 138
    - "no": 6
      title: Applications
      page: 42
      pdf_page: 142
    - "no": 7
      title: Regularization
      page: 44
      pdf_page: 144
statements: 38
exercises: 28
content_sha256: b1c8634f08bd53b648fc568387faaf3c3a88742f9d247cb328e70ae7d331d539
translated_from: content/en/int/VIII/04_s4_convolution_of_measures_and_functions.md
translation_method: google
source_content_sha256: 95b7ec6ff7cbef1ba7740490a53cad1a14ca28185aac5574eb562cb861e78110
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 3ff95c696d977a76b03d98f0045104dce30c252638a611fec5380245f2163434
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。测量和函数的卷积

### 1. 测度与函数的卷积

令 X 为局部紧致空间，其上局部紧致群 G 在左侧连续运算。令$\beta$为X上的正测度，在G下准不变。令$\chi$为$G \times X$上的函数$> 0$，可测量$G \times X$上的每个测度，并且对于每个$s \in G$，$\chi(s^{-1}, \cdot)$为$\gamma(s)\beta$相对于$\beta$的密度：

$$
(1) \qquad \gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta,
$$

其中，按照 Ch 的约定。 VII, §1, No. 1，可写为：

$$
(1') \qquad d\beta(sx) = \chi(s, x) \, d\beta(x).
$$

这些数据将保持固定在第 1、2、3 号中（注 2 或 No. 2 除外）。

回想一下（§2, No. 5），如果$\chi$是连续的并且$\beta$有支持$X$，那么$\chi$是乘子。

令$f$为$X$上的局部$\beta$可积复形函数，令$\mu$为$G$的测度。对于每个$s \in G$，测度$\gamma(s)(f \cdot \beta)$有基$\beta$，因为$\beta$是准不变的。因此，如果 $\mu$ 和 $f \cdot \beta$ 可卷积，则 $\mu * (f \cdot \beta)$ 有基 $\beta$（§3, No. 2，命题 10）。

#### 定义 1 {#int-viii-s4-def-1 .statement tag=09K4}

*如果$\mu$和$f \cdot \beta$是可卷积的，则$\mu$和$f$相对于$\beta$来说是可卷积的。 $\mu * (f \cdot \beta)$相对于$\beta$的每个密度称为$\mu$和$f$相对于$\beta$的卷积乘积，并表示为$\mu *_{\beta} f$。*

当不可能混淆时，可以省略 $\beta$。 $G$ 和函数 $X$ 上的多个测度的卷积以类似的方式定义。

$\mu$和$f$的各种卷积乘积在局部$\beta$几乎处处相等。如果$\beta$支持$X$，并且存在$\mu$和$f$的连续卷积乘积，则后者是唯一确定的；然后它被称为$\mu$和$f$相对于$\beta$的*卷积乘积。

令$s \in G$和$f$是$X$上的局部$\beta$可积复形函数。那么$\varepsilon_s$和$f$是可卷积的，并且

$$
\varepsilon_s * (f \cdot \beta) = \gamma(s)(f \cdot \beta) = (\gamma(s)f) \cdot (\gamma(s)\beta) = (\gamma(s)f) \cdot \chi(s^{-1}, \cdot) \cdot \beta,
$$

因此

$$
(2) \qquad (\varepsilon_s * f)(x) = \chi(s^{-1}, x) f(s^{-1}x) = (\gamma_{\chi}(s)f)(x)
$$

局部地$\beta$-几乎无处不在。

#### 引理 1 {#int-viii-s4-lem-1 .statement tag=09K5}

*令 $\mu$ 为$G$ 的度量。那么$\chi$是局部$(\mu \otimes \beta)$可积的，并且$\mu \otimes \beta$的像在$G \times X$到$G \times X$的同胚$(s, x) \mapsto (s, s^{-1}x)$下是$\chi \cdot (\mu \otimes \beta)$。*

我们可以假设$\mu \geqslant 0$。让$F \in \mathscr{K}_+(\mathbf{G} \times \mathbf{X})$。然后
$$
\iint F(s, s^{-1}x) d\mu(s) d\beta(x) = \int d\mu(s) \int F(s, s^{-1}x) d\beta(x)
$$
$$
= \int d\mu(s) \int F(s, x) d(\gamma(s^{-1})\beta)(x) = \int d\mu(s) \int F(s, x)\chi(s, x) d\beta(x).
$$

现在，函数$(s, x) \mapsto F(s, x)\chi(s, x)$具有紧凑的支持并且$(\mu \otimes \beta)$可测量。由 Ch. V, §8, No. 3，命题7，前面的等式证明了这个函数是$(\mu \otimes \beta)$可积的，并且
$$
\iint F(s, s^{-1}x) d\mu(s) d\beta(x) = \iint F(s, x)\chi(s, x) d\mu(s) d\beta(x).
$$
这同时证明了断言和引理 1。

#### 命题 1 {#int-viii-s4-prop-1 .statement tag=09K6}

*令$\mu$为$\mathbf{G}$的测度，$f$为$\mathbf{X}$的局部$\beta$可积复形函数。假设函数$s \mapsto f(s^{-1}x)\chi(s^{-1}, x)$本质上是$\mu$可积的，除了$x$的值的局部$\beta$可忽略的集合，以及函数$x \mapsto \int |f(s^{-1}x)|\chi(s^{-1}, x) d|\mu|(s)$，几乎在任何地方都定义为$\beta$，是局部$\beta$可积的。那么 $\mu$ 和 $f$ 是可卷积的。*

我们可以假设$f \geqslant 0$和$\mu \geqslant 0$。让$h \in \mathscr{K}_+(\mathbf{X})$。我们要证明函数 $(s, x) \mapsto h(sx)$ 对于$\mu \otimes (f \cdot \beta) = (1 \otimes f) \cdot (\mu \otimes \beta)$（第 V, §8, No. 5 章，第 10 条命题）本质上是可积的，即 $\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x) < +\infty$（第 V, §5, No. 3 章，第 3 条命题）；显然足以证明存在一个$a > 0$，使得对于$\mathbf{G}$的每个紧凑子集$K$，
$$
\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x) \leqslant a.
$$
到引理1，
$$
\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x)
$$
$$
= \iint^* h(x)f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x) d\mu(s) d\beta(x).
$$
现在，函数$(s, x) \mapsto h(x)f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x)$是$(\mu \otimes \beta)$可测量的（引理1）并且具有紧凑的支持。因此，前面的表达式等于（第 V, §8, No. 3 章，提案 7）
$$
\int^* h(x) d\beta(x) \int^* f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x) d\mu(s)
$$
$$
\leqslant (\sup h) \int^* d\beta(x) \int^* f(s^{-1}x)\chi(s^{-1}, x) d\mu(s),
$$

其中S表示h的支持度。 从而命题。

#### 命题 2 {#int-viii-s4-prop-2 .statement tag=09K7}

— 令 $\mu$ 为 G 上的测度，f 为 X 上的局部 $\beta$ 可积复数函数。假设满足以下条件之一：
(i) f 和 $\chi$ 连续；
(ii) G 在 X 中正确运行，并且 f 是零，对紧集的可数并的补集；
(iii) $\mu$ 由可数并紧集携带。
如果$\mu$和f是可卷积的，那么函数$s \mapsto f(s^{-1}x)\chi(s^{-1}, x)$本质上是$\mu$可积的，除了x的值的局部$\beta$可忽略不计的集合，并且局部几乎处处都有$\beta$，

$$
(\mu *_{\beta} f)(x) = \int_G f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) = \int_G (\gamma_{\chi}(s)f)(x)\, d\mu(s).
$$

让$h \in \mathscr{H}(X)$。由于$\mu$和f是可卷积的，函数$(s, x) \mapsto h(sx)f(x)$本质上是$(\mu \otimes \beta)$可积。到引理 1，函数 $(s, x) \mapsto h(x)f(s^{-1}x)\chi(s^{-1}, x)$ 本质上是 $(\mu \otimes \beta)$ 可积。在叙述的假设 (i) 或 (ii) 下，可以推断出该函数是 $(\mu \otimes \beta)$ 可积的；因为，在第一种情况下它是连续的并且适用第 3 章的命题 3。 V, §1, No. 1，在第二种情况下，它是零在紧集的可数并之外，并且应用No. 2的第7、2）条，loc。引用。由勒贝格-富比尼定理，

$$
\iint h(sx)\, d\mu(s)\, d(f \cdot \beta)(x) = \iint h(x)f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)\, d\beta(x)
= \int h(x)\, d\beta(x) \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s),
$$

函数 $x \mapsto g(x) = \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)$ 而且$\beta$ 是可积的。由此可见

$$
\langle h, \mu * (f \cdot \beta) \rangle = \langle h, g \cdot \beta \rangle,
$$

从而$g = \mu *_{\beta} f$。

现在假设$\mu$由紧集的序列的并 S携带。 函数

$$
(s, x) \mapsto h(x)f(s^{-1}x)\chi(s^{-1}, x)\varphi_S(s)
$$

本质上是$(\mu \otimes \beta)$可积，并且零在紧集的可数并之外，因此$(\mu \otimes \beta)$可积。从$\mu = \varphi_S \cdot \mu$开始，参数结论为之前。

#### 注 {#int-viii-s4-n1-rem-1 .statement tag=09K8}

当$\mu$有界时，命题2的假设(iii)尤其得到满足。因为，对于每个 $n > 0$，都存在一个 $G$ 的紧凑子集 $K_n$，使得
$$
|\mu|(G - K_n) \leq \frac{1}{n}
$$
（第 IV, §4, No. 7 章），$\mu$ 由 $K_n$ 的并承载。更一般地，令$\rho$是$G$上的下半连续有限函数$> 0$，使得$\rho(st) \leq \rho(s)\rho(t)$；如果满足$\mu \in \mathscr{M}^\rho$、假设(iii)；因为，$\rho \cdot \mu$是有界的，并且$\mu$由与$\rho \cdot \mu$相同的子集携带，因为在$G$的每个紧凑子集上，$\rho$在下面由常数$> 0$界定。

### 2. 例可卷积措施和函数

在道具中。如图3和图4所示，$\mathscr{C}'(G)$和$\mathscr{M}(G)$分别在$\mathscr{C}(G)$和$\mathscr{K}(G)$配备了紧凑收敛的拓扑。

#### 命题 3 {#int-viii-s4-prop-3 .statement tag=09K9}

— 假设 $\chi$ 连续。让$\mu \in \mathscr{C}'(G)$，$f \in \mathscr{C}(X)$。然后：
(i) $\mu$ 和 $f$ 相对于 $\beta$ 是可卷积的。
(ii) No. 1 定义的公式 (3) 对于每个$x \in X$，有一个连续的卷积乘积$\mu *_{\beta} f$，并且正是由连续表示定义的元素$\gamma_\chi(\mu)f$ $\mathscr{C}(X)$中的$G$中的$\gamma_\chi$；此外，相对于$\mathscr{C}'(G)$的等连续子集和$\mathscr{C}(X)$的紧致子集，映射$(\mu, f) \mapsto \mu *_{\beta} f$是低连续的。
(iii) 如果在加法 $f \in \mathscr{K}(X)$ 中，则 (ii) 属于至 $\mathscr{K}(X)$ 和映射 $(\mu, f) \mapsto \mu *_{\beta} f$ 的乘积 $\mu *_{\beta} f$ 相对于等连续的子集是低连续的$\mathscr{C}'(G)$ 和 $\mathscr{K}(X)$ 的紧凑型子集。

我们知道 $\mu$ 和 $f$ 是可卷积的（§3, No. 2，命题 8 (i)）。另一方面，对于 §2 的记号，我们有
$$
\gamma_\chi(\mu)f = \int (\gamma_\chi(s)f)d\mu(s) \in \mathscr{C}(X)
$$
因为 $\mathscr{C}(X)$ 已经完成。特别是，对于每个 $x \in X$，
$$
(\gamma_\chi(\mu)f)(x) = \int (\gamma_\chi(s)f)(x)\,d\mu(s).
$$
这与命题 2 (i) 和§2, No. 6 相结合，证明了 (ii)。最后，如果$f \in \mathscr{K}(X)$则$\mu * (f \cdot \beta)$具有紧支持（§3, No. 2，命题9），因此$\mu *_{\beta} f \in \mathscr{K}(X)$。例如，让我们考虑通过连续扩展$\mathscr{K}(X)$中的连续算子$\gamma_\chi(s)$而获得的补全$\mathscr{K}(X)^{\sim}$中$G$的连续表示$U$（§ 2, No. 1，*注3*）。设$S$为$\mu$的支撑。 函数$\gamma_\chi(s)f$，对于$s \in S$，其支持包含在固定的紧集$K$中。 集合$\mathscr{K}(X, K)$是$\mathscr{K}(X)$的完全线性子空间。因此$U(\mu)f \in \mathscr{K}(X)$。人们将$U(\mu)f = \mu *^\beta f$视为之前，并且(iii)再次从§ 2, No. 6得出。

#### 命题 4 {#int-viii-s4-prop-4 .statement tag=09KA}

*假设G在X内正确运行，并且$\chi$是连续的。让 $\mu \in \mathscr{M}(G)$ 和 $f \in \mathscr{K}(X)$.*

(i) $\mu$ 和 $f$ 相对于 $\beta$ 是可卷积的。

(ii) *No. 1定义的公式(3)对于每个$x \in X$一个连续的卷积乘积$\mu *^\beta f$。*

(iii) $\mathscr{M}(G) \times \mathscr{K}(X)$到$\mathscr{C}(X)$的*映射$(\mu, f) \mapsto \mu *^\beta f$相对于$\mathscr{M}(G)$的有界子集和包含在某些子空间$\mathscr{K}(X, L)$中的紧子集和$\mathscr{K}(X)$的紧凑子集来说是低连续的（其中$L$是$X$的可变紧凑子集）。*

我们知道$\mu$和$f$是可卷积的（§ 3, No. 2，命题8（ii）），并且很明显，对于每个$x \in X$，（3）中出现的积分都存在。令$K$和$L$是$X$的两个紧凑的子集。存在$G$的紧子集$H$，使得关系$x \in K$和$s^{-1}x \in L$隐含$s \in H$；让$\varphi \in \mathscr{K}_+(G)$和$\varphi(s) = 1$得到$s \in H$。然后，对于$f \in \mathscr{K}(X, L)$和$x \in K$，

$$
\int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) = \int f(s^{-1}x)\chi(s^{-1}, x)\varphi(s)\, d\mu(s)
= ((\varphi \cdot \mu) *^\beta f)(x).
$$

因此，$\int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)$是$x$的连续函数，定义是乘积$\mu *^\beta f \in \mathscr{C}(X)$的卷积。此外，对于紧收敛拓扑，$\mathscr{M}(G)$到$\mathscr{C}'(G)$的映射$\mu \mapsto \varphi \cdot \mu$是连续的。因此，第 3 (iii) 条意味着，对于 $X$ 的每个紧致子集 $L$，$\mathscr{M}(G) \times \mathscr{K}(X, L)$ 的映射 $(\mu, f) \mapsto \mu *^\beta f$ 进入 $\mathscr{C}(X)$ 相对于 $\mathscr{K}(X, L)$ 的紧致子集是低连续的。特别地，$\mathscr{M}(G) \times \mathscr{K}(X)$到$\mathscr{C}(X)$的映射$(\mu, f) \mapsto \mu *^\beta f$是单独连续的。由于 $\mathscr{K}(X)$ 是桶状的，因此这个映射相对于 $\mathscr{M}(G)$ 的有界子集是低连续的（TVS，III, § 5, No. 3，命题 6）。

#### 注 1 {#int-viii-s4-n2-rem-1 .statement tag=09KB}

— 根据命题 4 的假设，对于每个 $f \in \mathscr{K}(X)$，当 $\mathscr{M}_+(G)$ 配备*模糊* 拓扑时，$\mathscr{M}_+(G)$ 到$\mathscr{C}(X)$ 的映射 $\mu \mapsto \mu *^\beta f$ 是连续的。例如，令$K$为$X$的紧致子集，$S$为$f$的（紧致）支持；由于$G$在$X$、$s \in G$的集合中正常运行，因此存在$x \in K$和$s^{-1}x \in S$是$G$的紧凑子集$L$（GT，III, § 4, No. 5，Th.1）。令$\varepsilon$为数$> 0$，$\mathscr{K}_+(G)$中的$\varphi$函数等于1，紧集$L$，$\mathscr{M}_+(G)$的$\mu_0$元素； 集合$W_0$措施$\mu \in \mathscr{M}_+(G)$使得
$$
\left| \int \varphi(s)\, d\mu(s) - \int \varphi(s)\, d\mu_0(s) \right| \leq \varepsilon
$$
是$\mathscr{M}_+(G)$中$\mu_0$的邻域。另一方面，函数$(s, x) \mapsto f(s^{-1}x)\chi(s^{-1}, x)$在$L \times K$上一致连续，因此存在点$x_i \in K$（$1 \leq i \leq n$）的有限数，这样对于每个$x \in K$，都存在一个$i$，其中
$$
|f(s^{-1}x)\chi(s^{-1}, x) - f(s^{-1}x_i)\chi(s^{-1}, x_i)| \leq \varepsilon
$$
对于所有$s \in L$。由于 $\mu(L) \leq \int \varphi(s)\, d\mu_0(s) + \varepsilon$ 对于所有 $\mu \in W_0$，也
$$
\begin{align*}
\left| \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) - \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu(s) \right| \\
\leq \varepsilon \left( \int \varphi(s)\, d\mu_0(s) + \varepsilon \right)
\end{align*}
$$
对于每个$x$满足前面的不等式和每个$\mu \in W_0$。现在令 $W$ 为 $\mathscr{M}_+(G)$ 中$\mu_0$ 的邻域，由测度 $\mu \in W_0$ 形成，使得
$$
\left| \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu(s) - \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu_0(s) \right| \leq \varepsilon
$$
$1 \leq i \leq n$。很明显，对于每一个度量 $\mu \in W$ 和每一个 $x \in K$，
$$
\begin{align*}
\left| \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) - \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu_0(s) \right| \\
\leq \varepsilon \left( 2 \int \varphi(s)\, d\mu_0(s) + 2\varepsilon + 1 \right),
\end{align*}
$$
由于$\varepsilon$是任意的，这证明了我们的断言。

#### 命题 5 {#int-viii-s4-prop-5 .statement tag=09KC}

*假设 $\chi$ 是连续的乘子并且每个函数 $\chi(s, \cdot)$ 有界。*
(i) *$G$上的函数$s \mapsto \rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$是下半连续$> 0$并且对于$G$中的所有$s, t$满足$\rho(st) \leq \rho(s)\rho(t)$。*
(ii) *设 $\mu \in \mathscr{M}^\rho(G)$ 和 $f \in L^\infty(X, \beta)$。*1 *则 $\mu$ 和 $f$ 是可卷积的，并且 $\mu *^\beta f$ 几乎在任何地方都由 No. 1 的公式 (3) 局部给出。一个有$\mu *^\beta f \in L^\infty(X, \beta)$，还有$\| \mu *^\beta f \|_\infty \leq \| \mu \|_\rho \| f \|_\infty$。*

1对于函数$f$，表达方式“$f \in L^\infty(X, \beta)$”是对记号的滥用，表示根据上下文，符号$f$将被解释为函数或函数的等价类。 In particular, the symbol $\mu *^\beta f$ can stand for either a function defined locally $\beta$-almost everywhere, or the equivalence class of such a function for the relation of equality locally $\beta$-almost everywhere.

(iii) *If, moreover, $f \in \mathscr{C}^\infty(X)$ (resp. $\overline{\mathscr{K}(X)}$), then formula (3) of No. 1 defines for every $x$ a convolution product $\mu *^\beta f$ that belongs to $\mathscr{C}^\infty(X)$ (resp. $\mathscr{K}(X)$).

(iv) *如果$f \in \mathscr{K}(X)$，则(3)定义的卷积乘积$\mu *^\beta f$就是$\overline{\mathscr{K}(X)}$中$G$的连续表示$\gamma_\chi$定义的元素$\gamma_\chi(\mu)f$。

恒等式$\chi(st, x) = \chi(s, tx)\chi(t, x)$立即意味着$\rho(st) \leq \rho(s)\rho(t)$。另一方面，$\rho$是下半连续的，是连续函数的上包络线。

让$\mu \in \mathscr{M}^\rho(G)$。根据No. 1的命题1，$\mu$和1是可卷积的；命题 2 (i) 表明 $(|\mu| *^\beta 1)(x) \leq \int_G \rho(s) d|\mu|(s)$ 局部$\beta$——几乎无处不在。因此，如果$f$是$\beta$可测且$|f| \leq 1$，则$\mu$和$f$是可卷积的且$N_\infty(\mu *^\beta f) \leq \int \rho(s) d|\mu|(s)$。此外，$\mu *^\beta f$几乎处处都由No. 1的公式(3)局部给出，因为满足No. 1的命题2的条件(iii)。这意味着(ii)。

假设 $f$ 连续，并且在绝对值中以 1 为界。很明显，对于所有$x \in X$，(3) 中出现的积分都存在。让我们证明它们持续依赖于 $x$。我们可以假设$\mu \geq 0$。设$x_0 \in X$和$\varepsilon > 0$。令 $K$ 为 $G$ 的紧凑子集，使得 $\int_{G - K} \rho(s) d\mu(s) \leq \varepsilon$。在$X$中存在$x_0$的邻域$V$，使得$x \in V$意味着

$$
|f(s^{-1}x)\chi(s^{-1}, x) - f(s^{-1}x_0)\chi(s^{-1}, x_0)| \leq \varepsilon / \mu(K)
$$

对于$s \in K$。那么，对于$x \in V$，

$$
\left| \int f(s^{-1}x)\chi(s^{-1}, x) d\mu(s) - \int f(s^{-1}x_0)\chi(s^{-1}, x_0) d\mu(s) \right|
$$
$$
\leq 2 \int_{G - K} \rho(s) d\mu(s) + \int_K \frac{\varepsilon}{\mu(K)} d\mu(s) \leq 3\varepsilon,
$$

从而我们的断言。假设在加法$f \in \overline{\mathscr{K}(X)}$。令 $H$ 为 $X$ 的紧凑子集，使得 $|f(y)| \leq \varepsilon$ 为 $y \notin H$。让$x \notin KH$。然后 $s^{-1}x \notin H$ 对应 $s \in K$，因此

$$
\left| \int_G f(s^{-1}x)\chi(s^{-1}, x) d\mu(s) \right| \leq \int_{G - K} \rho(s) d\mu(s) + \int_K \varepsilon \rho(s) d\mu(s)
$$
$$
\leq \varepsilon \left( 1 + \int_G \rho(s) d\mu(s) \right),
$$

从而完成 (iii) 的证明。

最后，如果 $f \in \mathscr{K}(X)$ 那么，由于 $\varepsilon_x \in \mathscr{M}^1(X)$ 对于所有 $x \in X$，我们有

$$
(\gamma_\chi(\mu)f)(x) = \int (\gamma_\chi(s)f)(x) d\mu(s),
$$

因此$\gamma_\chi(\mu)f$是(3)定义的卷积乘积$\mu *^\beta f$。

#### 命题 6 {#int-viii-s4-prop-6 .statement tag=09KD}

*假设 $\chi$ 是连续的乘子并且每个函数 $\chi(s, \cdot)$ 有界。让$\rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$。令 $p$ 和 $q$ 为两个共轭指数 ($1 \leq p < +\infty$)。设$\mu \in \mathscr{M}^{\rho^{1/q}}(G)$和$f \in L^p(X, \beta)^2$则：
(i) $\mu$ 和 $f$ 是可卷积的；
(ii) 卷积乘积$\mu *^\beta f$在局部$\beta$-几乎处处由公式(3)给出，并且局部$\beta$-几乎处处等于函数$g \in L^p(X, \beta)$，使得$\|g\|_p \leq \|\mu\|_{\rho^{1/q}} \|f\|_p$；
(iii) $g$等于$L^p(X, \beta)$中$G$的连续表示$\gamma_\chi$定义的元素$\gamma_\chi(\mu)f$。

我们有
$$
\int^* \|\gamma_\chi(s)f\|_p d|\mu|(s) \leq \left( \int^* \rho(s)^{1/q} d|\mu|(s) \right) \|f\|_p < +\infty
$$
由 §2, No. 5、公式 (5)。另一方面，$G$到$L^p(X, \beta)$的映射$s \mapsto \gamma_\chi(s)f$是连续的（§2, No. 5，命题9）。因此这个映射是$\mu$可积的。让
$$
g = \int_G (\gamma_\chi(s)f) d\mu(s) \in L^p(X, \beta).
$$
我们有$\|g\|_p \leq (\int \rho^{1/q}(s) d|\mu|(s)) \|f\|_p$。 应用前面的注到$|f|$，可以看出，$G$到$L^p(X, \beta)$的映射$s \mapsto \varepsilon_s * |f|$是$\mu$可积的，因此，对于每个$h \in \mathscr{H}(X)$，映射$s \mapsto \langle h, \varepsilon_s * (|f| \cdot \beta) \rangle$是 $\mu$ 可积的。 §1, No. 5的第7条命题证明了$\mu$和$f \cdot \beta$是可卷积的。而且，
$$
\int_X g(x)h(x) d\beta(x) = \int_G d\mu(s) \int_X (\gamma_\chi(s)f)(x)h(x) d\beta(x)
= \int_G \langle h, \varepsilon_s * (f \cdot \beta) \rangle d\mu(s),
$$
根据 §1, No. 5 的命题 7，最后一个积分等于 $\langle h, \mu * (f \cdot \beta) \rangle$。因此，可以看出$g$是$\mu$和$f$的卷积乘积。这个卷积乘积是局部$\beta$ 给出的——几乎所有地方都由 (3)、命题 2 和其后面的 *注* 给出。

2对于函数$f$，表达方式“$f \in L^p(X, \beta)$”是对记号的滥用，表示根据上下文，符号$f$将被解释为$\beta$定义的函数-几乎无处不在，或者解释为此类的等价类函数关系等式 $\beta$ - 几乎无处不在。因此$f \in L^p$可以象征$f \in \mathscr{L}^p$或$\dot{f} \in L^p$。

通过滥用记号，它通常是叙述的函数$g$之一，表示为$\mu *^\beta f$，它允许写入

$$
\| \mu *^\beta f \|_p \leq \| \mu \|_{\rho^{1/q}} \| f \|_p .
$$

此外，如果 $X$ 在无穷大处可数，那么记号的这种风格是完全合理的。

#### 推论{#int-viii-s4-n2-cor-1 .statement tag=09KE}

*根据第 6 号提案的假设，左模的映射* $(\mu, f) \mapsto \mu *^\beta f$ *定义于* $L^p(X, \beta)$ *结构超过* $\mathscr{M}^{\rho^{1/q}}(G)$ $(1 \leq p \leq +\infty)$。

这是从 Props 得出的。 5和6以及卷积乘积的结合性。

#### 注 2 {#int-viii-s4-n2-rem-2 .statement tag=09KF}

— 设 $X$ 为局部紧致空间，其上局部紧致群 $G$ 在右侧连续运行 $(x, s) \mapsto xs$。令 $\beta$ 为$X$ 的正测度。令 $\chi$ 为 $G \times X$ 上的函数 $> 0$，对于 $G \times X$ 上的每个度量都可测量，这样对于每个 $s \in G$ 都有 $\delta(s)\beta = \chi(s, \cdot) \cdot \beta$。令$f$为$X$上的局部$\beta$可积函数，令$\mu$为$G$的测度。如果$f \cdot \beta$和$\mu$可卷积（将$X \times G$的映射$(x, s) \mapsto xs$转化为$X$），则$(f \cdot \beta) * \mu$有基$\beta$。然后我们说$f$和$\mu$相对于$\beta$是可卷积的； $(f \cdot \beta) * \mu$相对于$\beta$的每个密度称为$f$和$\mu$相对于$\beta$的卷积乘积，并表示为$f *^\beta \mu$或简称为$f * \mu$。

令 $G^0$ 为与 $G$ 相反的群。到$(s, x) \mapsto xs$时，$G^0$在$X$的左侧连续运行。说$f$和$\mu$在上述意义上是可卷积的，相当于说对于$X$中在左侧运算的$G^0$来说，$\mu$和$f$是可卷积的；而卷积乘积$f *^\beta \mu$正是$G^0$在$X$左侧操作的卷积乘积$\mu *^\beta f$。另一方面，对于 $s \in G^0$ 来说，有 $\gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta$。第 1 项和第 2 项的结果可以立即转化为有关乘积 $f *^\beta \mu$ 的结果。特别是：

1) 如果$s \in G$和$f$是局部$\beta$可积的，那么$f$和$\varepsilon_s$是可卷积的并且

$$
(f * \varepsilon_s)(x) = \chi(s^{-1}, x)f(xs^{-1}) .
$$

2) 如果 $f$ 和 $\mu$ 是可卷积的，并且满足命题 2 的条件 (i), (ii), (iii) 之一，则 $f *^\beta \mu$ 局部给出 $\beta$ - 几乎处处由下式给出

$$
(f *^\beta \mu)(x) = \int_G f(xs^{-1})\chi(s^{-1}, x)\, d\mu(s) .
$$

我们把翻译另一个叙述的任务留给读者。 注如果$\chi$是连续的并且$\beta$有支持$X$，那么

$$
\chi(ts, x) = \chi(s, xt)\chi(t, x) \quad (x \in X; \ s, t \text{ in } G) .
$$

### 3. 卷积和转置

让我们回到No. 1开始时的假设和记号，但让我们假设在加法中，$\beta$*与乘子*$\chi$相对不变；因此$\chi$是$G$上的连续函数。

#### 命题 7 {#int-viii-s4-prop-7 .statement tag=09KG}

*令$f$为$X$上的局部$\beta$可积函数，$\nu$为$X$上的测度，$\mu$为$G$上的测度。假设：
(i) $\mu$ 和 $f$ 是可卷积的，公式 (3) 的 No. 1 定义局部$\beta$ - 几乎处处都是卷积乘积 $\mu *_{\beta} f$。
(ii) $\chi \cdot \check{\mu}$ 和 $\nu$ 是可卷积的。
(iii) *函数* $g(s, x) = f(s^{-1}x)\chi(s^{-1})$ *是* $(\mu \otimes \nu)$*-可积。
*然后* $f$ *本质上可积* $(\chi \cdot \check{\mu}) * \nu$，*函数* $\mu *_{\beta} f$ *由 (3) 定义是* $\nu$*可积，并且*

$$
\nu(\mu *_{\beta} f) = ((\chi \cdot \check{\mu}) * \nu)(f).
$$

由于$g(s, x)$对于$\mu \otimes \nu$可积，函数$f(sx)$对于$(\chi \cdot \check{\mu}) \otimes \nu$本质上可积，$f$对于$(\chi \cdot \check{\mu}) * \nu$本质上可积。根据 Lebesgue–Fubini 定理，$\mu *_{\beta} f = \int g(s, x) d\mu(s)$ 是 $\nu$ 可积且

$$
\begin{align*}
\nu(\mu *_{\beta} f) &= \iint f(s^{-1}x)\chi(s^{-1}) d\mu(s) d\nu(x) \\
&= \iint f(sx)\chi(s) d\check{\mu}(s) d\nu(x) = ((\chi \cdot \check{\mu}) * \nu)(f).
\end{align*}
$$

#### 例 {#int-viii-s4-n3-exa-1 .statement tag=09KH}

— 1) 根据第 3 条命题可以取 $f \in \mathscr{C}(X)$、$\nu \in \mathscr{C}'(X)$ 和 $\mu \in \mathscr{C}'(G)$，Cor. §1, No. 4 的第 5 号提案。 公式(7)则意味着$\mathscr{C}'(X)$的自同态$\nu \mapsto (\chi \cdot \check{\mu}) * \nu$是$\mathscr{C}(X)$的自同态$f \mapsto \mu * f$的*转置*。

2) 根据§3, No. 2、注的第3、第8条命题，可取$f \in \mathscr{K}(X)$、$\nu \in \mathscr{M}(X)$、$\mu \in \mathscr{C}'(G)$，连续函数$g(s, x)$的支持度与$\mu \otimes \nu$的支持度相交于紧集。 公式(7)则意味着$\mathscr{M}(X)$的自同态$\nu \mapsto (\chi \cdot \check{\mu}) * \nu$是$\mathscr{K}(X)$的自同态$f \mapsto \mu * f$的*转置*。

3) 如果$G$在$X$上运行正常，则可以根据§3, No. 2的第4、8条命题取$f \in \mathscr{K}(X)$、$\nu \in \mathscr{C}'(X)$和$\mu \in \mathscr{M}(G)$，以及与*例2*中相同的注。

#### 命题 8 {#int-viii-s4-prop-8 .statement tag=09KI}

*设$f$和$g$是$X$上的两个局部$\beta$可积函数，并设$\mu \in \mathscr{M}(G)$。假设：*

(i) $\mu$ 和 $f$ 是可卷积的，公式 (3) 的 No. 1 定义局部 $\beta$ - 几乎处处都是卷积乘积 $\mu *_{\beta} f$。

(ii) $\chi \cdot \check{\mu}$ 和 $g$ 是可卷积的，公式 (3) of No. 1（其中 $\mu$ 被 $\chi \cdot \check{\mu}$ 替代，$f$ $g$）定义局部$\beta$ - 几乎所有地方卷积乘积$(\chi \cdot \check{\mu}) *_{\beta} g$。

(iii) 在$G$上存在函数$\psi$，局部等于$\mu$——几乎处处等于1，使得函数

$$
h(s, x) = g(x) f(s^{-1} x) \chi(s^{-1}) \psi(s)
$$

是$(\mu \otimes \beta)$可积的。

那么函数 $g(x)((\mu *_{\beta} f)(x))$ 和 $f(x)(((\chi \cdot \check{\mu}) *_{\beta} g)(x))$ 本质上是 $\beta$ 可积的，并且

$$
(8) \quad \int f(x)(((\chi \cdot \check{\mu}) *_{\beta} g)(x)) d\beta(x) = \int g(x)((\mu *_{\beta} f)(x)) d\beta(x).
$$

对于 (iii) 和 Lebesgue-Fubini 定理、函数

$$
x \mapsto g(x) \int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s)
$$

是$\beta$可积，并且

$$
\begin{align*}
\mathrm{I} &= \iint f(s^{-1} x) g(x) \chi(s^{-1}) \psi(s) d\mu(s) d\beta(x) \\
&= \int g(x) d\beta(x) \int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s).
\end{align*}
$$

但是$\psi \cdot \mu = \mu$，因而

$$
\int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s) = (\mu *_{\beta} f)(x)
$$

当地$\beta$-几乎无处不在。这表明函数

$$
x \mapsto g(x)((\mu *_{\beta} f)(x))
$$

本质上是 $\beta$ 可积的

$$
\mathrm{I} = \int g(x)((\mu *_{\beta} f)(x)) d\beta(x).
$$

另一方面，引理1表明函数

$$(s, x) \mapsto g(sx)f(x)\chi(s^{-1})\psi(s)$$

可积 $(\chi \cdot \mu) \otimes \beta$。因此函数 $(s, x) \mapsto g(s^{-1}x)f(x)\psi(s^{-1})$ 对于 $\check{\mu} \otimes \check{\beta}$ 可积，并且

$$
\begin{align*}
\mathrm{I} &= \iint g(s^{-1}x)f(x)\psi(s^{-1})\, d\check{\mu}(s)\, d\beta(x) \\
&= \int f(x)\, d\beta(x) \int g(s^{-1}x)\psi(s^{-1})\, d\check{\mu}(s).
\end{align*}
$$

但是 $\check{\psi} \cdot \check{\mu} = \check{\mu}$ 以及本地 $\int g(s^{-1}x)\psi(s^{-1})\, d\check{\mu}(s) = ((\chi \cdot \check{\mu}) *^\beta g)(x)$ $\beta$ - 几乎无处不在。这表明函数

$$x \mapsto f(x)(((\chi \cdot \check{\mu}) *^\beta g)(x))$$

本质上是 $\beta$ 可积的

$$\mathrm{I} = \int f(x)(((\chi \cdot \check{\mu}) *^\beta g)(x))\, d\beta(x).$$

这就证明了命题。

#### 例 {#int-viii-s4-n3-exa-2 .statement tag=09KJ}

— 4) 可以取$f \in \mathscr{C}(X)$、$g \in \mathscr{K}(X)$和$\mu \in \mathscr{C}'(G)$（与$\psi = 1$一起）。

5) 如果G在X上运行正常，则可以取$f \in \mathscr{K}(X)$、$g \in \mathscr{K}(X)$和$\mu \in \mathscr{M}(G)$（与$\psi = 1$）。

6) 可以取$f \in \mathbf{L}^p(X, \beta)$、$g \in \mathbf{L}^q(X, \beta)$和$\mu \in \mathscr{M}^\rho(G)$，其中$1 \leq p < +\infty$、$\frac{1}{p} + \frac{1}{q} = 1$、$\rho = \chi^{-1/q}$。 条件 (i) 和 (ii) 由 Props 满足。 5和6。 让我们证明(iii)。 我们已经看到，$\mu$由集合 S携带，它是紧集的可数并。 让我们将 S 的特征函数视为$\psi$。 函数 $h$ 是 $(\mu \otimes \beta)$ 可测量的：对于函数 $(s, x) \mapsto g(x)\chi(s^{-1})\psi(s)$ 来说，函数 $(s, x) \mapsto f(s^{-1}x)$ 引理 1 也是如此。 Moreover, $g$ being zero outside a countable union of $\beta$-integrable sets, $h$ is zero outside a countable union of $(\mu \otimes \beta)$-integrable sets. 然后我们就有了（Ch. V, §8, No. 3，命题 7)：

$$
\begin{align*}
\mathrm{J} &= \iint^* |g(x)f(s^{-1}x)|\chi(s^{-1})\psi(s)\, d|\mu|(s)\, d\beta(x) \\
&= \int^* |g(x)|\, d\beta(x) \int^* |f(s^{-1}x)|\chi(s^{-1})\psi(s)\, d|\mu|(s).
\end{align*}
$$

但由于 $g$（分别为$\psi$）是零，位于可积集合的可数并之外，所以（9）的第二个成员的上积分等于基本上积分（第V, §1, No. 2，命题7）。现在（第 V, §5, No. 3 章，第 3 条命题）

$$
\int^\bullet |f(s^{-1}x)| \chi(s^{-1}) \psi(s) d|\mu|(s) = \int^\bullet |f(s^{-1}x)| \chi(s^{-1}) d|\mu|(s)
$$

从$\mu = \psi \cdot \mu$开始。根据命题 6，最后一个积分是有限的，并且局部等于 $(|\mu| *^\beta |f|)(x)$ $\beta$——几乎在任何地方。所以

$$
J = \int^\bullet |g(x)|(|\mu| *^\beta |f|)(x) d\beta(x),
$$

并且 J 是有限的，因为 $g \in L^q$ 和 $|\mu| *^\beta |f| \in L^p$（命题 6）。因此 h 是 $(\mu \otimes \beta)$ 可积的。

公式 (8) 那么意味着$L^q(X, \beta)$ 的自同态 $g \mapsto (\chi \cdot \check{\mu}) * g$ 是$\mu \in \mathscr{M}^\rho(G)$，转置自同态 $f \mapsto \mu * f$ $L^p(X, \beta)$。

### 4. 测度和函数在群上的卷积

令 G 为局部紧致群。在第 4 条和第 5 条中，我们在 G 上固定了一个相对不变的正测度 $\beta \neq 0$；设 $\chi$ 和 $\chi'$ 分别为它的左侧和右侧乘子（回想一下$\chi' = \chi \Delta_G$）。如果 $\mu$ 是 G 上的测度，$f$ 是 G 上的局部 $\beta$ 可积函数，则 $\mu$ 和 $f$ 以及乘积 $\mu * f$ 的可卷积性（分别是 $f$ 和 $\mu$ 的可卷积性和乘积$f * \mu$）可以通过将 G 视为通过平移在左侧（或右侧）对其自身进行操作来定义。让我们在这种情况下明确前面的一些结果：

1) 令$\mu$为G上的测度，$f$为G上的局部$\beta$可积复形函数。假设已验证以下条件之一：
   (i) $f$ 是连续的；
   (ii) $f$ 是零对紧集的可数并的补集；
   (iii) $\mu$ 由可数并紧集携带。
如果 $\mu$ 和 $f$ 可卷积，那么，局部 $\beta$ - 几乎处处，

$$
(\mu * f)(x) = \int_G f(s^{-1}x) \chi(s^{-1}) d\mu(s).
$$

如果 $f$ 和 $\mu$ 可卷积，那么，局部 $\beta$ - 几乎处处，

$$
(f * \mu)(x) = \int_G f(xs^{-1}) \chi'(s^{-1}) d\mu(s).
$$

2) 令$p$和$q$为两个共轭指数($1 \leq p \leq +\infty$)。如果$\mu \in \mathscr{M}^{\chi^{-1/q}}(G)$和$f \in L^p(G, \beta)$，则$\mu$和$f$可卷积，并且$\mu * f$局部等于$\beta$——几乎处处等于$L^p(G, \beta)$中的函数；一个有（已经注意到滥用记号）

$$
\| \mu * f \|_p \leq \| \mu \|_{\chi^{-1/q}} \| f \|_p .
$$

如果$\mu \in \mathscr{M}^{{\chi'}^{-1/q}}(G)$和$f \in L^p(G, \beta)$，那么$f$和$\mu$是可卷积的，并且$f * \mu$局部等于$\beta$——几乎处处等于$L^p(G, \beta)$中的函数；一个有 $\| f * \mu \|_p \leq \| \mu \|_{{\chi'}^{-1/q}} \| f \|_p$。

3) 映射$(\mu, f) \mapsto \mu * f , (f, \mu) \mapsto f * \mu$定义在$L^p(G, \beta)$结构上左模超过$\mathscr{M}^{\chi^{-1/q}}(G)$和右模超过$\mathscr{M}^{{\chi'}^{-1/q}}(G)$。 $L^p(G, \beta)$上的两个外法则可以通过卷积的结合性进行置换。

4) 如果$\mu * f$是连续的并且在每个点由(10)给出，那么

$$
(\mu * f)(e) = \int f(s^{-1}) \chi(s^{-1}) d\mu(s) .
$$

如果 $f * \mu$ 是连续的并且在每点处由 (11) 给出，则

$$
(f * \mu)(e) = \int f(s^{-1}) \chi'(s^{-1}) d\mu(s) .
$$

### 5. 函数对群的卷积

我们节省 No. 4 中的记号 $G, \beta, \chi, \chi'$。

回想一下，如果$f$是$G$上的复数函数，则$\beta$局部可积的性质独立于$\beta$的选择。令 $\mathscr{L}(G)$ 为具有该性质的函数的集合。如果$f \in \mathscr{L}(G) , g \in \mathscr{L}(G)$，关系

« $f \cdot \beta$ 和 $g \cdot \beta$ 是可卷积的 »

独立于 $\beta$ 的选择（§ 3, No. 1，命题 6）。然后我们会说$f$和$g$是*可卷积的*。到No. 1，$(f \cdot \beta) * (g \cdot \beta)$为形式$h \cdot \beta$，其中$h \in \mathscr{L}(G)$，$h$被确定为局部$\beta$-可忽略的集合。我们将写成$h = f *^{\beta} g$，并且我们将说$h$是$f$和$g$相对于$\beta$的*卷积乘积*。 （在不会混淆的情况下，可以省略 $\beta$。）如果将 $\beta$ 替换为 $\psi \cdot \beta$，则 $\psi$ 是 $\mathbf{R}_+^*$ 中 $G$ 的连续表示，$h$ 不是变换（§ 3, No. 1，提案 6)；如果 $\beta$ 替换为 $a \beta$ ($a \in \mathbf{R}_+^*$)，则 $h$ 替换为 $ah$。多个函数在$G$上的卷积乘积以类似的方式定义。

如果$f$和$g$的卷积之一是连续的，则它是唯一确定的，因为$\beta$的支持度是$G$。然后，它被称为$f$和$g$相对于$\beta$的*卷积乘积。

很明显，

$$
f *_{\beta}^{\beta} g = (f \cdot \beta) *_{\beta}^{\beta} g = f *_{\beta}^{\beta} (g \cdot \beta).
$$

#### 命题 9 {#int-viii-s4-prop-9 .statement tag=09KK}

*让$f, g$位于$\mathscr{L}(G)$中。假设函数$s \mapsto g(s^{-1}x)f(s)\chi(s^{-1})$本质上是$\beta$可积的，除了$x$的值的局部$\beta$可忽略的集合，并且函数*

$$
x \mapsto \int |g(s^{-1}x)f(s)|\chi(s^{-1})\, d\beta(s),
$$

*本地定义$\beta$-几乎无处不在，局部地$\beta$-可积。那么 $f$ 和 $g$ 是可卷积的。*

这是从No. 1 的第 1 条命题得出的。

#### 命题 10 {#int-viii-s4-prop-10 .statement tag=09KL}

*让$f, g$位于$\mathscr{L}(G)$中。假设这两个函数之一是连续的，或者是零在紧集的可数并的补集上。如果 $f$ 和 $g$ 是可卷积的，则函数 $f * g$ 局部给出 $\beta$ - 几乎到处都是*

$$
(f * g)(x) = \int_G g(s^{-1}x)f(s)\chi(s^{-1})\, d\beta(s)
= \int_G f(xs^{-1})g(s)\chi'(s^{-1})\, d\beta(s).
$$

这是从No. 1中的第2条命和No. 4中的注得出的。

特别是，如果 $f * g$ 是连续的并且在每个点处由 (15) 给出，则

$$
(f * g)(e) = \int g(s^{-1})f(s)\chi(s^{-1})\, d\beta(s) = \int f(s^{-1})g(s)\chi'(s^{-1})\, d\beta(s).
$$

更具体地，如果$\beta$是左右哈尔测度，并且如果$f * g$和$g * f$是连续的并且在每个点处由(15)给出，并且对于$g * f$来说类似的公式，则

$$
(f * g)(e) = (g * f)(e) = \int f(s)g(s^{-1})\, d\beta(s).
$$

#### 命题 11 {#int-viii-s4-prop-11 .statement tag=09KM}

— 令 $f, g$ 在 $\mathscr{L}(G)$ 中。假设函数$f, g$之一是连续的，并且函数$f, g$之一具有紧支撑。那么$f$和$g$是可卷积的。 公式 (15) 定义对于所有连续的 $x \in G$ 乘积 $f * g$。如果$f \in \mathscr{K}(G)$和$g \in \mathscr{K}(G)$，则$f * g \in \mathscr{K}(G)$。

这是从 Props 得出的。 No. 2 的 3 和 4。

#### 命题 12 {#int-viii-s4-prop-12 .statement tag=09KN}

— 令 $p$ 和 $q$ 为两个共轭指数 ($1 \leq p \leq +\infty$)。如果$f \chi^{-1/q} \in L^1(G, \beta)$和$g \in L^p(G, \beta)$，那么$f$和$g$是可卷积的，$f * g$局部等于$\beta$——在$L^p(G, \beta)$中几乎处处等于函数，并且
$$
\|f * g\|_p \leq \|f \chi^{-1/q}\|_1 \|g\|_p.
$$
如果$f \in L^p(G, \beta)$和$g {\chi'}^{-1/q} \in L^1(G, \beta)$，那么$f$和$g$是可卷积的，$f * g$局部等于$\beta$——在$L^p(G, \beta)$中几乎处处等于函数，并且
$$
\|f * g\|_p \leq \|f\|_p \|g {\chi'}^{-1/q}\|_1.
$$
这是从 Props 得出的。 No. 4中的No. 2和注的5和6。

#### 命题 13 {#int-viii-s4-prop-13 .statement tag=09KO}

— 如果 $f \chi^{-1} \in L^1(G, \beta)$ 和 $g \in \overline{\mathscr{K}(G)}$，或者 $f \in \mathscr{K}(G)$ 和 $g {\chi'}^{-1} \in L^1(G, \beta)$，则 $f$ 和 $g$ 可卷积，并且 (15) 定义对于每个$x \in G$ 乘积 $f * g$ 属于至 $\mathscr{K}(G)$。

这是从No. 2中的第5条命以及No. 4中的注得出的。

#### 命题 14 {#int-viii-s4-prop-14 .statement tag=09KP}

— 如果 $f \chi^{-1} \in L^1(G, \beta)$ 和 $g \in L^\infty(G, \beta)$，则对于每个 $x \in G$ 乘积 $f * g$，公式 (15) 定义有界且对于$G$ 的右均匀结构一致连续。

我们已经知道 $f * g$ 属于到 $L^\infty(G, \beta)$（No. 2，提案 5）；此外，$(f * g)(x) = \int f(xs^{-1})g(s)\, d\nu(s)$，设定$\nu = {\chi'}^{-1} \cdot \beta$； $\nu$ 是正确的哈尔测度。因此
$$
|(f * g)(x) - (f * g)(x')| \leq \|g\|_\infty \int |f(xs^{-1}) - f(x's^{-1})|\, d\nu(s)
$$
$$
= \|g\|_\infty \int |(f(s^{-1}) - f(x'x^{-1}s^{-1}))\, d\nu(s)
$$
如果 $x'x^{-1}$ 位于 $e$ 的合适邻域内（§ 2, No. 5，命题 8），则后一个积分是任意小的。

#### 命题 15 {#int-viii-s4-prop-15 .statement tag=09KQ}

— 令 $p$ 和 $q$ 为两个共轭指数 ($1 < p < +\infty$)。假设 $\beta$ 是左不变的。令$f \in L^p(G, \beta)$，$g \in L^q(G, \check{\beta})$。那么$f$和$g$是可卷积的。 公式 (15) 定义，对于每个 $x \in G$、乘积 $f * g$ 属于到 $\mathscr{K}(G)$ 并且是这样的
$$
\|f * g\|_\infty \leq \|f\|_p \|g\|_q.
$$

因为，我们有$\dot{g} \in L^q(G, \beta)$，因此函数$s \mapsto g(s^{-1}x)f(s)$对于每个$x \in G$来说是$\beta$可积。而且，

$$
\int |g(s^{-1}x)f(s)| d\beta(s) \leq \left( \int |f(s)|^p d\beta(s) \right)^{1/p} \left( \int |g(s^{-1}x)|^q d\beta(s) \right)^{1/q}
= \|f\|_p \left( \int |\dot{g}(x^{-1}s)|^q d\beta(s) \right)^{1/q} = \|f\|_p \|\dot{g}\|_q,
$$

因此 $f$ 和 $g$ 是可卷积的（命题 9）。人们同时看到，对于每个 $x$ 乘积 $f * g$，(15) 定义使得

$$
|(f * g)(x)| \leq \|f\|_p \|\dot{g}\|_q.
$$

对于$\mathscr{K}(G)$中的$f, g$，我们有$f * g \in \mathscr{K}(G)$（命题11）；因此，对于$f \in L^p(G, \beta)$和$g \in L^q(G, \dot{\beta})$，(15)提供的乘积$f * g$是$\mathscr{K}(G)$中函数的统一极限，因此属于到$\overline{\mathscr{K}(G)}$。

#### 推论{#int-viii-s4-n5-cor-1 .statement tag=09KR}

— 让 $f \in L^2(G, \beta)$，$g \in L^2(G, \beta)$。那么$f$和$\dot{g}$是可卷积的。 $f * \dot{g}$ 属于到 $\overline{\mathscr{K}(G)}$ 的卷积之一及其在 $e$ 处的值是 $\int_G f(s)g(s) d\beta(s)$。

只需取第 15 条提案中的$p = q = 2$ 并应用（16）即可。

我们不再假设 $\beta$ 是左不变的。令$\rho$为$G$上的下半连续有限函数$> 0$，使得$\rho(st) \leq \rho(s)\rho(t)$适用于$G$中的所有$s, t$。我们用$G$上的复数函数的等价类的$L^\rho(G, \beta)$集合来表示，它们可积为$\rho \cdot \beta$。通过映射$f \mapsto f \cdot \beta$，$L^\rho(G, \beta)$可以与$\mathscr{M}^\rho(G)$的元素的集合识别，其具有基$\beta$（独立于$\beta$的选择的集合）。如果一个集合

$$
\|f\|_\rho = \int_G |f(s)| \rho(s) d\beta(s)
$$

对于$f \in L^\rho(G, \beta)$，该标识与范数兼容，因此$L^\rho(G, \beta)$表现为$\mathscr{M}^\rho(G)$的完整规范的子代数。它甚至是§3, No. 2第10号提案所提出的$\mathscr{M}^\rho(G)$的双面理想。 （对于$\rho = 1$，可以恢复断言或No. 4之一。）特别是，$L^1(G, \beta)$可以用$\mathscr{M}^1(G)$的封闭两侧理想来识别。

#### 命题 16 {#int-viii-s4-prop-16 .statement tag=09KS}

— 令 $U$ 为 Banach 空间 $E$ 中 $G$ 的连续表示。 集合 $\rho(s) = \|U(s)\|$ 对于所有 $s \in G$。对于每个 $f \in L^\rho(G, \beta)$，集合 $U(f) = U(f \cdot \beta)$。那么$f \mapsto U(f)$就是$E$中代数$L^\rho(G, \beta)$的线性表示，这样$\|U(f)\| \leq \|f\|_\rho$。

这是从第 11 条提案§2, No. 6 和§3, No. 3 得出的。

### 6. 应用

#### 命题 17 {#int-viii-s4-prop-17 .statement tag=09KT}

— 令 G 为 G 的局部紧凑群，A 子集，可测量且对于 Haar 测度而言不可局部忽略。那么$A \cdot A^{-1}$是e的邻域。

令 $\beta$ 为左哈尔测度。存在 G 的紧致子集 K，使得 $B = A \cap K$ 可与 $\beta$ 的测度 > 0 可积。让我们应用 Cor. 15 号提案的 $f = g = \varphi_B$。 函数 $F = \varphi_B * \check{\varphi}_B$ 是连续的并且在 e 处 > 0。因此，存在 e 的邻域 V，使得 $F(x) > 0$ 对于 $x \in V$。现在，

$$
F(x) = \int \varphi_B(s) \varphi_B(x^{-1}s) d\beta(s) = \beta(B \cap xB).
$$

因此，对于$x \in V$，有$B \cap xB \neq \emptyset$、从而$x \in B \cdot B^{-1}$。因此$V \subset B \cdot B^{-1} \subset A \cdot A^{-1}$。

#### 推论 1 {#int-viii-s4-prop-17-cor-1 .statement tag=09KU}

— 令 H 为可通过 Haar 测度 $\beta$ 测量的 G 的子群。那么 H 要么是开路，要么是局部$\beta$-可忽略不计。

对于 $H = H \cdot H^{-1}$，因此如果 H 不是局部 $\beta$ 可忽略的，则 H 包含 e 的邻域（命题 17）因此是开集（GT，III, §2, No. 1，命题 4 的 Cor.）。

#### 推论 2 {#int-viii-s4-prop-17-cor-2 .statement tag=09KV}

— 令 L 为乘法稳定的 G 的子集，并且其补集对于 Haar 测度 $\beta$ 来说局部可忽略不计。然后$L = G$。

因为，$L^{-1}$和$L \cap L^{-1}$局部有$\beta$可忽略的补集。现在，$L \cap L^{-1}$ 是子群，因此是开放的（Cor. 1），因此是封闭的。因此，$G - (L \cap L^{-1})$是开路且局部$\beta$可以忽略不计，是空的。因此$G = L \cap L^{-1}$。

#### 命题 18 {#int-viii-s4-prop-18 .statement tag=09KW}

— 令 G 为局部紧凑群、$\Gamma$ 集合，配备乘法 $(u, v) \mapsto uv$ 和 Hausdorff 拓扑，使得：
1) $\Gamma$的拓扑在平移下不变；
2) 乘法的限制对于$\Gamma \times \Gamma$的每个紧凑子集是连续的。

令 $f : G \to \Gamma$ 为 G 到 $\Gamma$ 的映射，使得 G 中的 $x, y$ 为 $f(xy) = f(x)f(y)$，且可测量 G 上的哈尔测度 $\beta$。则 $f$ 是连续的。

集合$g(x) = f(x^{-1})$代表$x \in G$。由于$f$和$g$是$\beta$可测的，因此存在G的不可$\beta$可忽略的紧子集 K，使得$f$和$g$到K的限制是连续的。 $K \times K$的映射$(x, y) \mapsto f(xy^{-1}) = f(x)g(y)$到$\Gamma$是连续的，因为$\Gamma$的乘法在$f(K) \times g(K)$是连续的；现在，这个映射可以写成$\varphi \circ \psi$，其中$\psi$是$K \times K$到$K \cdot K^{-1}$的映射$(x, y) \mapsto xy^{-1}$，$\varphi$是$f$到$K \cdot K^{-1}$的限制。令$R$ 为$\psi$ 在$K \times K$ 上定义的等价关系。 $(K \times K)/R$的映射$\psi'$到$K \cdot K^{-1}$由$\psi$通过通向商推导出来是连续的，因此$(K \times K)/R$是Hausdorff，$\psi'$是同胚。由于$\varphi \circ \psi$是连续的，因此可以看出$f$到$K \cdot K^{-1}$的限制是连续的。现在，$K \cdot K^{-1}$是$e$的邻域（命题17），因此$f$在$e$连续。对于每个$x_0 \in G$，$f(x_0x) = f(x_0)f(x)$，因此$f$在$x_0$连续，因为$\Gamma$的拓扑在平移下是不变的。

#### 推论 1 {#int-viii-s4-prop-18-cor-1 .statement tag=09KX}

*令$G$为局部紧致群，$\beta$为$G$，$E$的Haar测度，$E$中$G$的Hausdorff桶状局部凸空间，$U$线性表示，这样，当$\mathscr{L}(E;E)$配备了拓扑逐点收敛时，$U(s) \in \mathscr{L}(E;E)$对于所有$s \in G$，$\beta$是可测量的。那么$U$就是连续的线性表示。*

设$\Gamma$为$E$的自同构的群，配备逐点收敛的拓扑。这个拓扑是Hausdorff并且在翻译下是不变的。令 $K$ 为 $\Gamma$ 的紧致子集。那么 $K$ 有界于 $\mathscr{L}(E;E)$，具备逐点收敛的拓扑，因此是等连续的 (TVS, III, §4, No. 2, Th. 1)；因此，$K \times K$到$\mathscr{L}(E;E)$的映射$(u,v) \mapsto v \circ u$是连续的（*loc.cit.*，§5, No. 5，第9号提案的Cor.1）。因此，对于每个$x \in E$，$G$到$E$的映射$s \mapsto U(s)x$是连续的（命题18）。由于 $E$ 是桶状的，$U$ 是连续的（§2, No. 1，命题 1）。

#### 推论 2 {#int-viii-s4-prop-18-cor-2 .statement tag=09KY}

*令$G$为局部紧凑群，$\beta$为$G$的哈尔测度，$E$为可分离的Banach空间，以及$E$中$G$的$U$线性表示，使得$U(s) \in \mathscr{L}(E;E)$ 对于所有$s \in G$。令$(a_m)$为$E$中的总序列，并令$(a'_n)$为$E$的对偶$E'$的单位球$B'$中的密集序列，配备弱拓扑。假设$G$上的函数$s \mapsto \langle U(s)a_m, a'_n \rangle$是$\beta$可测的。那么$U$就是连续的线性表示。*

让我们首先证明对于每个 $z' \in E'$，标量函数

$$
s \mapsto \langle U(s)a_m, z' \rangle
$$

$\beta$-可测量；我们可以将自己限制在$\|z'\| \leq 1$的情况，并且，由于$B'$对于弱拓扑是可度量的（TVS，III, §3, No. 4，第6号命题的Cor.2），因此存在$(a'_n)$的子序列$(a'_{n_k})$弱收敛到$z'$； 函数

$$
s \mapsto \langle U(s)a_m, z' \rangle
$$

因而，$\beta$的序列的极限可测量函数，从而我们的断言。由此可见，对于每个$m$，$G$到$E$的映射$s \mapsto U(s)a_m$是$\beta$可测量的（第IV, §5, No. 5，命题10）。另一方面，存在$E$的元素、$a_i$的线性组合、序列$(b_m)$，即密集在$E$的单位球中。对于每个 $s \in G$，$\|U(s)\| = \sup_m \|U(s)b_m\|$，因而 $s \mapsto \|U(s)\|$ 是可测量的。令$K$ 为$G$ 的紧致子集，并令$\varepsilon > 0$。存在$K$的紧子集$K_0$，使得$\beta(K - K_0) \leq \varepsilon$并且函数$s \mapsto U(s)a_m$和$s \mapsto \|U(s)\|$的限制到$K_0$是连续的。那么$s \in K_0$的$U(s)$是等连续的，拓扑的点向收敛诱导在$U(K_0)$拓扑上的$a_m$的集合的点向收敛（TVS，III, §3, No. 4，命题5）。因而，$K_0$到$\mathscr{L}_s(E; E)$的映射$s \mapsto U(s)$是连续的。然后应用Cor就足够了。 1.

### 7. 正则化

#### 命题 19 {#int-viii-s4-prop-19 .statement tag=09KZ}

— *令$G$为局部紧致群，$\beta$为$G$，$\mathscr{B}$基上相对不变的正测度$\neq 0$，用于过滤$G$，由……组成中的$e$邻域的紧凑邻里。对于每个$V \in \mathscr{B}$，令$f_V$是$G$上的连续函数$\geq 0$，并且支持包含在$V$中，使得$\int f_V d\beta = 1$。如果$\mu$是$G$的测度，那么，在$\mathscr{M}(G)$配备有$\mathscr{H}(G)$紧致收敛的拓扑，

$$
\mu = \lim_V (\mu * f_V) \cdot \beta = \lim_V (f_V * \mu) \cdot \beta,
$$

极限是相对于$\mathscr{B}$的截面过滤器而取的。

对于$\mathscr{C}(G)$中的紧凑收敛的拓扑，相对于$\mathscr{B}$的截面滤波器，$f_V \cdot \beta$趋于$\varepsilon_e$（§ 2, No. 7，引理4的Cor.1）。因而，$\mathscr{M}(G)$中的$\mu = \lim_V \mu * (f_V \cdot \beta) = \lim_V (f_V \cdot \beta) * \mu$配备了$\mathscr{H}(G)$中紧致收敛的拓扑（§ 3, No. 3，Prop.12的Cor.）。

#### 注 1 {#int-viii-s4-n7-rem-1 .statement tag=09L0}

因而，我们看到$G$上的每个测度都是极限的测度，对于每个哈尔测度来说，承认*连续的密度*（对于第19号提案中指出的拓扑和对于模糊的拓扑来说*更不必说*）。

#### 注 2 {#int-viii-s4-n7-rem-2 .statement tag=09L1}

如果$G$可度量，则$\mathscr{B}$可取为序列$(V_n)$邻域。那么 $\mu$ 是具有连续密度的测度 $(\mu * f_{V_n}) \cdot \beta$ 的序列的极限。 *若$G$为实李群，则$f_{V_n}$可视为无限可微；稍后我们将看到密度 $\mu * f_{V_n}$ 是无限可微的。*

#### 命题 20 {#int-viii-s4-prop-20 .statement tag=09L2}

— *我们保留命题 19 的假设和记号。*令 $p \in [1, +\infty[$ 和 $g \in L^p(G, \beta)$。然后

$$
g = \lim_V g *^\beta f_V = \lim_V f_V *^\beta g
$$

在范数$N_p$的意义上，极限是相对于$\mathscr{B}$的截面过滤器而取的。

只需应用第 6 (iii) 号提案和 Cor. §2, No. 7。 引理 4 中的 3 个。

#### 注 3 {#int-viii-s4-n7-rem-3 .statement tag=09L3}

根据第 15 号提案，函数 $g * f_V$、$f_V * g$ 属于至 $\mathscr{K}(G)$。

#### 推论{#int-viii-s4-n7-cor-1 .statement tag=09L4}

— 令 $W$ 为 $L^1(G, \beta)$ 的闭线性子空间。为了使$W$成为$L^1(G, \beta)$的左（或右）理想，$W$在$G$的左（或右）平移下保持不变是必要且充分的。

假设$W$是左理想。设$s \in G$和$g \in W$。我们有$\varepsilon_s * g = \lim_V f_V * (\varepsilon_s * g) = \lim_V (f_V * \varepsilon_s) * g$和$(f_V * \varepsilon_s) * g \in W$，因此有$\varepsilon_s * g \in W$，因此有$\gamma(s)g \in W$。相反，如果$W$在左平移下不变，则$\mu *^\beta g \in W$对于$\mu \in \mathscr{M}^1(G)$和$g \in W$来说，因此$W$是更不必说$L^1(G, \beta)$的左理想。人们对正确的理想也有类似的争论。

#### 例 {#int-viii-s4-n7-exa-1 .statement tag=09L5}

我们取$G = \mathbf{R}$。让我们定义函数$F_n \in \mathscr{K}(\mathbf{R})$
$$
F_n(x) = (1 - x^2)^n \quad \text{if } x \in [-1, 1] \\
F_n(x) = 0 \qquad \text{if } x \notin [-1, 1].
$$
设$A_n = \int_{-1}^{+1} F_n(x) dx$和$G_n = A_n^{-1} F_n$。 §2, No. 7的措施$G_n(x) dx$满足条件，Cor.是直接的。 引理 4 中的 1。令$\mu$ 为$\mathbf{R}$ 的测度，其支持包含在$[-1/2, 1/2]$ 中。然后
$$
(\mu * G_n)(x) = \int_{\mathbf{R}} G_n(x - y) d\mu(y)
= A_n^{-1} \int_{-1/2}^{1/2} F_n(x - y) d\mu(y).
$$
如果$-1/2 \leq x \leq 1/2$，那么
$$
(\mu * G_n)(x) = A_n^{-1} \int_{-1/2}^{1/2} [1 - (x - y)^2]^n d\mu(y),
$$
因此 $\mu * G_n$ 重合在 $[-1/2, 1/2]$ 上用多项式计算。特别是，如果 $f$ 是连续的函数，且支持包含在 $[-1/2, 1/2]$ 中，则 $f * G_n$ 重合在 $[-1/2, 1/2]$ 中，具有多项式；此外，根据提案 5 (iv) 和 §2, No. 7，Cor. 引理 4 中的 3 个，$f * G_n$ 一致收敛到 $f$。
*如果$f$为类$C^r$，则$0 \leq s \leq r$的导数$D^s(f * G_n)$统一趋于$D^s f$。*

### 习题{#int-viii-s4-exercises}

§ 4](exercises/s4/)参见[习题。
