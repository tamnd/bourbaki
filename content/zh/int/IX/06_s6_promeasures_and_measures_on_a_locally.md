---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 6
section_title: Promeasures and measures on a locally convex space
lang: zh
source: int-vii-ix
book_pages: INT IX.72-INT IX.101, INT IX.117
pdf_pages: 0254-0283, 0299-0299
extraction: ocr
subsections:
    - "no": 1
      title: Promeasures on a locally convex space
      page: 72
      pdf_page: 254
    - "no": 2
      title: Image of a promeasure
      page: 74
      pdf_page: 256
    - "no": 3
      title: Fourier transform of a promeasure
      page: 75
      pdf_page: 257
    - "no": 4
      title: Calculation of Gaussian integrals
      page: 77
      pdf_page: 259
    - "no": 5
      title: Gaussian promeasures and measures
      page: 78
      pdf_page: 260
    - "no": 6
      title: Examples of Gaussian promeasures
      page: 82
      pdf_page: 264
    - "no": 7
      title: Wiener measure
      page: 85
      pdf_page: 267
    - "no": 8
      title: Continuity of the Fourier transform
      page: 92
      pdf_page: 274
    - "no": 9
      title: Minlos’s lemma
      page: 93
      pdf_page: 275
    - "no": 10
      title: Measures on the dual of a nuclear space
      page: 96
      pdf_page: 278
    - "no": 11
      title: Measures on a Hilbert space
      page: 97
      pdf_page: 279
statements: 33
exercises: 1
content_sha256: 27faf3f6b63ddfb4197ce1a4cd83989bbc90d76c788e1532c185587930e6afaf
translated_from: content/en/int/IX/06_s6_promeasures_and_measures_on_a_locally.md
translation_method: google
source_content_sha256: e617c5fb964b4dfa4c93d927e10519f76530432982d0dd1d298de1585dc144da
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: d3755bcf479bbdb3a79a913582bfdf4f2a04b831b0d0488948da9cc0bb853e42
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 6。局部凸空间上的测度和测度

在整个截面中，仅考虑实数中超过域的向量空间。局部凸空间是指$\mathbf{R}$上的拓扑向量空间，即豪斯多夫且局部凸。局部凸空间 E 的拓扑对偶将表示为 $E'$；对于$x \in E$和$x' \in E'$，写为$\langle x, x' \rangle = x'(x)$。

### 1. 局部凸空间上的 Promeasures

令 E 为局部凸空间。我们用有限余维的E的闭合线性子空间的$\mathscr{F}(E)$集合表示，按关系$\supset$排序。对于每个$V \in \mathscr{F}(E)$，$p_V$表示E到$E/V$的典范映射。令V和W为$\mathscr{F}(E)$的两个元素，使得$V \supset W$；我们用 $E/W$ 的 $p_{VW}$ 映射表示为通过商从 E 的恒等映射推导出来的 $E/V$。族$\mathscr{Q}(E) = (E/V, p_{VW})$是局部凸空间的逆系，由$\mathscr{F}(E)$索引。它被称为 E* 的有限维商的 *逆系。

可以证明，逆系 $\mathscr{Q}(E)$ 的逆极限与$E'$ 的代数对偶$E'{}^*$ 自然同构，并配备弱拓扑 $\sigma(E'{}^*, E')$。

#### 定义 1 {#int-ix-s6-def-1 .statement tag=09S6}

*设$E$为局部凸空间。在 $E$ 的有限维商的逆系上，每逆系$^{(1)}$ 的测度（§ 4, No. 2，定义 1）对 $E$ 调用 promeasure。*

在其他字中，$E$上的promeasure$\mu$是一个族$(\mu_V)_{V \in \mathscr{F}(E)}$，其中$\mu_V$是有限维空间$E/V$上的有界（正）测度，并且当$V \supset W$时$\mu_V = p_{VW}(\mu_W)$。所有措施 $\mu_V$ 具有相同的总质量，称为前措施 $\mu$ 的*总质量*。

对于$E$的子空间$V$到属于到$\mathscr{F}(E)$，存在$E'$的元素$x'_1, \ldots, x'_n$的有限数是充分必要的，使得$V$由$x \in E$组成满足 $\langle x, x'_i \rangle = 0$ for $1 \leq i \leq n$（TVS、II, § 6, No. 3、第 1 条的 Cor.2 和 No. 5、第 7 号提案的 Cor.2）。此外，在有限维向量空间上存在且仅有一个豪斯多夫拓扑向量空间拓扑（TVS，I, § 2, No. 3，Th.2）。因而，$E$的promeasure概念仅取决于$E$的对偶$E'$。

令 $\lambda$ 为 $E$ 上的有界测度。对于每个$V \in \mathscr{F}(E)$，让我们用$E$的典范映射$p_V$到$E/V$下的$\lambda$的$\widetilde{\lambda}_V$像来表示。对于 $\mathscr{F}(E)$ 中的任意两个元素 $V$ 和 $W$，一个人有$p_V = p_{VW} \circ p_W$，使得 $V \supset W$；因而，族$\widetilde{\lambda} = (\widetilde{\lambda}_V)_{V \in \mathscr{F}(E)}$是$E$的赞成计划。我们可以说$\widetilde{\lambda}$是与措施$\lambda$*相关联的promeasure。人们立即看出 $\lambda$ 和 $\widetilde{\lambda}$ 具有相同的总质量。

#### 命题 1 {#int-ix-s6-prop-1 .statement tag=09S7}

*设$E$为局部凸空间。 映射$\lambda \mapsto \widetilde{\lambda}$是$E$上有界措施集合双射到$E$满足上的优惠措施$(\mu_V)_{V \in \mathscr{F}(E)}$集合以下条件：

对于每个 $\varepsilon > 0$，都存在 $E$ 的紧凑子集 $K$，使得 $\mu_V(E/V - p_V(K)) \leq \varepsilon$ 对于所有 $V \in \mathscr{F}(E)$。*

已知$E$上连续的线性形式的核的交等于0（TVS，II, § 4, No. 1，第2条命题的Cor.1）；因而$\bigcap_{V \in \mathscr{F}(E)} V = \{0\}$和家庭$(p_V)_{V \in \mathscr{F}(E)}$既是连贯又是分离的。然后从 Th 得出命题。 § 4, No. 2 中的 1 个。

特别地，映射$\lambda \mapsto \widetilde{\lambda}$是单射的。如果$\mu$是$E$的一个promeasure，并且如果$E$存在有界测度$\lambda$使得$\mu = \widetilde{\lambda}$，我们会滥用语言说$\mu$是一个测度。如果$E$是有限维的，则每个promeasure$\mu = (\mu_V)_{V \in \mathscr{F}(E)}$都是一个测度：对于$\{0\} \in \mathscr{F}(E)$，$E/\{0\} = E$和$p_{V,\{0\}} = p_V$，从而$\mu_V = p_V(\mu_{\{0\}})$对于所有$V \in \mathscr{F}(E)$；在其他字，$\mu = \widetilde{\lambda}$与$\lambda = \mu_{\{0\}}$。

(1) 也称为“射影系统”。

#### 命题 2 {#int-ix-s6-prop-2 .statement tag=09S8}

— 设 T 为可数集合，T 上实数函数的 E 向量空间，配备逐点收敛的拓扑。 E 上的每一个测度都是一个测度。

对于每个$t \in T$，令$\varepsilon_t$为E上的线性形式$f \mapsto f(t)$。我们知道（TVS，II, §6, No. 6，第8条命题的Cor.2）族$(\varepsilon_t)_{t \in T}$是向量空间$E'$的基。用'T'的有限子集的$\Phi$集合表示，对于每个$J \in \Phi$，让$E_J$为T上的函数的集合，在J的每个点处为零。让$F \in \mathscr{F}(E)$；由于F的正交$F^\circ$是$E'$的有限维子空间，因此存在$J \in \Phi$，使得$F^\circ$包含在由$\varepsilon_t$为$t \in J$生成的$E'$的线性子空间G中。从$F^\circ \subset G$开始，我们有$E_J = G^\circ \subset F^{\circ\circ} = F$，可数族$(E_J)_{J \in \Phi}$在$\mathscr{F}(E)$中并列。 命题然后从 Th 开始。 §4, No. 3 中的 2 个。

### 2. 像的优惠措施

设E和$E_1$是两个局部凸空间，$u$是E到$E_1$的连续线性映射。对于E 属于到$\mathscr{F}(E)$的每个$V_1 \in \mathscr{F}(E_1)$、子空间$V = \overline{u}^{-1}(V_1)$和$u$定义，通过商，将$E/V$的线性映射$u_{V_1}$代入$E_1/V_1$。令$\mathscr{F}(E_1)$中的$V_1$和$W_1$使得$V_1 \supset W_1$； 集合$V = \overline{u}^{-1}(V_1)$和$W = \overline{u}^{-1}(W_1)$。我们有 $V \supset W$，还有一个可交换的图表

$$
\begin{array}{ccccc}
E & \xrightarrow{pw} & E/W & \xrightarrow{pvw} & E/V \\
\downarrow u & & \downarrow u_{W_1} & & \downarrow u_{V_1} \\
E_1 & \xrightarrow{pw_1} & E_1/W_1 & \xrightarrow{pv_{1W_1}} & E_1/V_1
\end{array}
$$

现在让 $\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ 成为 E 上的配度。对于每个 $V_1 \in \mathscr{F}(E_1)$，集合

(1)
$$
\nu_{V_1} = u_{V_1}(\mu_{u^{-1}(V_1)}).
$$

前面图表的交换律表明家庭$\nu = (\nu_{V_1})_{V_1 \in \mathscr{F}(E_1)}$是$E_1$的亲生。我们说$\nu$是$u$下$\mu$的像，并用$u(\mu)$表示。

令$\lambda$为E上的有界测度，$u(\lambda)$为$E_1$上的测度，即$u$下$\lambda$的像。如果promeasure $\mu$ 与$\lambda$ 关联，则promeasure $u(\mu)$ 与$u(\lambda)$ 关联。这是从前面的图表的交换律得出的。

让$V \in \mathscr{F}(E)$。 典范映射$p_V : E \to E/V$下的优惠措施$\mu$的$E/V$上的像优惠措施与措施$\mu_V$相关联的是直接的。

令 $u_1$ 为 $E_1$ 的连续线性映射到局部凸空间 $E_2$。轻松建立关系

$$
(u_1 \circ u)(\mu) = u_1(u(\mu))
$$

*（优惠措施像中的传递性）*。

### 3. 傅里叶变换的优惠

令 $E$ 为局部凸空间，而 $\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ 为 $E$ 的等度。对于$E$上的每个连续线性形式$x'$，我们用$\mu_{x'}$表示$\mathbf{R}$上的测度，即$E$上的测度$\mu$的$x'$下的像。 $\mu$ 的傅里叶变换是 $E'$ 上的函数 $\mathscr{F}\mu$ 定义为

$$
(\mathscr{F}\mu)(x') = \int_{\mathbf{R}} e^{it} d\mu_{x'}(t).
$$

令 $\lambda$ 为 $E$ 上的有界测度。 $\lambda$ 的傅里叶变换是 $E'$ 上的函数定义为

$$
(\mathscr{F}\lambda)(x') = \int_E e^{i\langle x, x' \rangle} d\lambda(x).
$$

令 $\mu$ 为与 $\lambda$ 相关的比例。对于每个$x' \in E'$，$\mathbf{R}$上的措施$\mu_{x'}$是像，在$E$上的措施$\lambda$的$x' : E \to \mathbf{R}$下；从公式(2)和(3)，立即推导出$\mathscr{F}\mu = \mathscr{F}\lambda$。

令 $\mu$ 为 $E$ 的任意比例，并且 $u$ 将 $E$ 的连续线性映射变为局部凸空间 $E_1$。用$E'_1$的$^t u$线性映射表示为$E'$，即$u$的转置，并用$\nu$表示$E_1$的比例$u(\mu)$。对于每个 $x'_1 \in E'_1$，我们有 $^t u(x'_1) = x'_1 \circ u$、从而

$$
\nu_{x'_1} = x'_1(\nu) = x'_1(u(\mu)) = (x'_1 \circ u)(\mu) = \mu_{^t u(x'_1)}.
$$

因而，

$$
\mathscr{F}(u(\mu)) = (\mathscr{F}\mu) \circ {}^t u.
$$

特别是，让我们将$E$的$u$典范映射$p_V$代入$E/V$（$V \in \mathscr{F}(E)$）。 $E/V$ 上的原测度$p_V(\mu)$ 与测度$\mu_V$ 相关联，$^t p_V$ 是$E/V$ 到与$E'$ 正交于$V$ 的子空间 $V^\circ$ 的对偶的同构。如果通过$^t p_V$将$(E/V)'$与$V^\circ$进行识别，则

$$
(\mathscr{F}\mu)(x') = \int_{E'/V} e^{i\langle x, x' \rangle} d\mu_V(x)
$$

对于所有$x' \in V^\circ$。其中一个具有$E' = \bigcup_{V \in \mathscr{F}(E)} V^\circ$，因此前面的公式表征了$E'$上的函数$\mathscr{F}\mu$。最后，如果（5）中的集合$x' = 0$，则可以看出$\mu$的总质量等于$(\mathscr{F}\mu)(0)$。

#### 命题 3 {#int-ix-s6-prop-3 .statement tag=09S9}

*令$E$为局部凸空间。将$E$上的集合映射$\mu \mapsto \mathscr{F}\mu$变为$E'$上的函数集合单射。*

公式 (5) 允许简化为$E$ 是有限维的情况；由于每个有限维空间都同构于空间$\mathbf{R}^n$，我们甚至可以假设存在整数$n \geqslant 0$使得$E = \mathbf{R}^n$。因此，我们必须证明如果$\mu$是$\mathbf{R}^n$上的有界测度（不一定是正数）并且如果

$$
\int_{\mathbf{R}^n} e^{i\langle x, y \rangle} d\mu(x) = 0
$$

对于$\mathbf{R}^n$上的每个线性形式$y$，然后$\mu = 0$。

对于每个整数 $m \geqslant 0$，令 $G_m$ 为 $\mathbf{R}^n$ 的子群 $m \cdot \mathbf{Z}^n$。用$\mathbf{R}^n$上连续的函数$f$的$\mathscr{C}_m$向量空间表示，使得$f(x + a) = f(x)$代表$x \in \mathbf{R}^n$和$a \in G_m$。根据GT第8条，X, §4, No. 4，$\mathscr{C}_m$中的每一个函数是型$x \mapsto e^{2\pi i \langle x, q \rangle}$的函数有限线性组合与$q \in m^{-1} \cdot \mathbf{Z}^n$的一致极限。因此，每函数 $f \in \mathscr{C}_m$ 就有 $\mu(f) = 0$。

令 $f$ 为 $\mathbf{R}^n$ 上具有紧支撑的连续函数。对于每个整数 $m \geqslant 0$，集合 $f_m(x) = \sum_{q \in G_m} f(x + q)$。 直接的，对于每个$x \in \mathbf{R}^n$，前面的级数只有有限多个项，而$f_m$属于到$\mathscr{C}_m$。此外，很容易看出，序列$(f_m)$在每个紧集上均匀地趋于$f$，并且存在一个常数$C \geqslant 0$，使得对于所有$m$都有$|f_m| \leqslant C$。因而，根据 §5, No. 6 的第 12 号提案，$\mu(f) = \lim_{m \to \infty} \mu(f_m)$。从$f_m \in \mathscr{C}_m$开始，我们有$\mu(f_m) = 0$，从而最后$\mu(f) = 0$。因而$\mu = 0$。

#### 注 {#int-ix-s6-n3-rem-1 .statement tag=09SA}

— 当$E$是有限维时，$E$的每个特征标都是形式$x \mapsto e^{i\langle x, x' \rangle}$和$x' \in E'$（*Théor.spect.*，Ch.II, §1, No. 9，Prop.12的Cor.3）。在这种情况下，命题 3 是从用于傅里叶变换的唯一性定理得出的（*loc. cit.*，§1, No. 6，命题 6 的 Cor.）。*

### 4.高斯积分的计算

#### 引理 1 {#int-ix-s6-lem-1 .statement tag=09SB}

对于每个整数 $n \geqslant 0$，

$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2^{n+1 \over 2} \Gamma \left( {n+1 \over 2} \right)
$$
(6)

$$
\int_{\mathbf{R}} x^{2n} e^{-x^2/2} dx = (2\pi)^{1/2} \frac{(2n)!}{2^n n!}
$$
(7)

$$
\int_{\mathbf{R}} x^{2n+1} e^{-x^2/2} dx = 0.
$$
(8)

回忆公式

$$
\Gamma(s) = \int_0^\infty u^{s-1} e^{-u} du
$$
(9)

适用于每个实数 $s > 0$（FRV、VII, §1, No. 3、提案 3）。将变量 $x = (2u)^{1/2}$ 设为变换时，由 (9) 得出

$$
\int_0^\infty x^n e^{-x^2/2} dx = \int_0^\infty (2u)^{n/2} e^{-u} {1 \over 2} 2^{1/2} u^{-1/2} du = 2^{n-1 \over 2} \Gamma \left( {n+1 \over 2} \right),
$$

从而公式 (6) 自

$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2 \int_0^\infty x^n e^{-x^2/2} dx.
$$

公式 (7) 由 (6) 和关系得出

$$
\Gamma \left( n + \frac{1}{2} \right) = \pi^{1/2} \frac{(2n)!}{2^{2n} n!}.
$$
(10)

对于$n = 0$，这个关系约化到$\Gamma(\frac{1}{2}) = \pi^{1/2}$，即到FRV的公式(21)，VII, §1, No. 3。一般情况下，在考虑到关系 $\Gamma(x+1) = x \cdot \Gamma(x)$（前述，§1, No. 1）的情况下，在$n$上遵循归纳。

最后，公式 (8) 由函数 $x \mapsto x^{2n+1} e^{-x^2/2}$ 是奇数这一事实得出。

#### 引理 2 {#int-ix-s6-lem-2 .statement tag=09SC}

对于每个复数 $y$，

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{ixy} dx = e^{-y^2/2}.
$$
(11)

特别是，

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} dx = 1.
$$

变量 $x \mapsto -x$ 的变换产生

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{i xy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{-ixy} dx;
$$

由于 $\cos u = \frac{e^{iu} + e^{-iu}}{2}$ 对于每个复数 $u$，因而

$$
(12) \quad (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{i xy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy \, dx .
$$

对于每个整数 $n \geqslant 0$，集合

$$
g_n(x) = (-1)^n (2\pi)^{-1/2} \frac{(xy)^{2n}}{(2n)!} e^{-x^2/2}.
$$

由(7)，

$$
(13) \quad \int_{\mathbf{R}} |g_n(x)| \, dx = \frac{1}{n!} \left( \frac{|y|^2}{2} \right)^n
$$
$$
(14) \quad \int_{\mathbf{R}} g_n(x) \, dx = \frac{1}{n!} \left( -\frac{y^2}{2} \right)^n,
$$

从而

$$
\sum_{n=0}^{\infty} \int_{\mathbf{R}} |g_n(x)| \, dx = e^{|y|^2/2} < +\infty.
$$

而且，因为，

$$
(2\pi)^{-1/2} e^{-x^2/2} \cos xy = \sum_{n=0}^{\infty} g_n(x),
$$

这个等式可以通过项、从而积分项

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy \, dx = \sum_{n=0}^{\infty} \int_{\mathbf{R}} g_n(x) \, dx = e^{-y^2/2}
$$

由(14)。 公式 (11) 然后从 (12) 得出。

### 5.高斯算子和测度

#### 命题 4 {#int-ix-s6-prop-4 .statement tag=09SD}

*设 E 为局部凸空间。对于 E' 上的每个正二次方形式 Q，在 E 上存在且仅有一个 Promeasure $\Gamma_Q$ 使得 $\mathscr{F} \Gamma_Q = e^{-Q/2}$。 $\Gamma_Q$的总质量等于1.*

$\Gamma_Q$的唯一性源自No. 3的第3条命题。 $\Gamma_Q$的总质量等于$(\mathscr{F}\Gamma_Q)(0) = e^{-Q(0)/2} = 1$。我们将分阶段证明存在。

A) E 为有限维 n，Q 非简并。

通过 No. 4 的引理 2，具有密度 $t \mapsto (2\pi)^{-1/2}e^{-t^2/2}$ 的 $\mathbf{R}$ 上的测度 $\gamma_1$ 受到限制，总质量为 1。 集合 $\gamma = \gamma_1 \otimes \cdots \otimes \gamma_1$ (n 因子)。从引理 2 of No. 4 推导出

$$
\int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n) = \prod_{j=1}^n \int_{\mathbf{R}} e^{ia_j t} d\gamma_1(t)
$$
$$
= \prod_{j=1}^n (2\pi)^{-1/2} \int_{\mathbf{R}} e^{ia_j t} e^{-t^2/2} dt
$$
$$
= \prod_{j=1}^n e^{-a_j^2/2}
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right).
$$

由于 Q 是正的且非简并，因而 Q 存在 E' 正交的基 $(e'_1, \ldots, e'_n)$（Alg.，Ch. IX, §7, No. 1）。让我们用 E 到 $\mathbf{R}^n$ 的 f 同构 $x \mapsto (e'_1(x), \ldots, e'_n(x))$ 表示，并用 $\Gamma_Q$ 表示 E 上的 $f^{-1}(\gamma)$ 测度。令 $x' = a_1 e'_1 + \cdots + a_n e'_n$ 在 E' 中；那么 $x'(f^{-1}(t_1, \ldots, t_n)) = \sum_{j=1}^n t_j a_j$ 为$t_1, \ldots, t_n$实数，从而

$$
\int_E e^{i\langle x, x' \rangle} d\Gamma_Q(x) = \int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n)
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right) = \exp \left( -\frac{1}{2}Q(x') \right).
$$

因而，$\mathscr{F}\Gamma_Q = e^{-Q/2}$。

B) E 有限维的。

令 N 为由 $x'$ 形成的 E' 的线性子空间，使得 $Q(x') = 0$。用 M 表示 E 中 N 的正交，并用 j 典范嵌入 M 到 E 的正交。线性映射 ${}^t j : E' \to M'$ 是满射，与核 N，因此在$M'$ 上存在非简并正二次形式 q，使得 $Q = q \circ {}^t j$。由上可知，M 上存在有界测度$\Gamma$，使得$\mathscr{F}\Gamma = e^{-q/2}$。 设定$\Gamma_Q = j(\Gamma)$，我们有

$$
\mathscr{F}\Gamma_Q = (\mathscr{F}\Gamma) \circ {}^t j = \exp(-q \circ {}^t j/2) = e^{-Q/2}
$$

由公式 (4) 共 No. 3。

C) *一般情况。*
让$V \in \mathscr{F}(E)$。用$E/V$上的$E$的$p_V$典范映射表示，并用$Q_V$表示$(E/V)'$上的正二次方形式$Q \circ {}^t p_V$；最后，令 $\mu_V$ 为 $E/V$ 与傅里叶变换 $e^{-Q_V/2}$ (cf. B)) 的度量。若$W \in \mathscr{F}(E)$包含在$V$中，则$p_V = p_{VW} \circ p_W$、从而$Q_V = Q_W \circ {}^t p_{VW}$；通过No. 3的公式(4)，测度$p_{VW}(\mu_W)$有傅里叶变换函数$(e^{-Q_W/2}) \circ {}^t p_{VW} = e^{-Q_V/2}$，因此等于$\mu_V$。因而，族$(\mu_V)_{V \in \mathscr{F}(E)}$是$\mu$右$E$的赞成措施。 No. 3的公式(5)表明$\mathscr{F}\mu$等于$e^{-Q/2}$。

#### 定义 2 {#int-ix-s6-def-2 .statement tag=09SE}

*设$E$为局部凸空间。对于 $E'$ 上的每个正二次方形式 $Q$，傅里叶变换等于 $e^{-Q/2}$ 的 $E$ 上的测度称为 $E$ 上方差为 $Q$ 的高斯测度，并表示为 $\Gamma_Q$。如果 $E'$ 上存在正二次方形式 $Q$ 使得 $\mu = \Gamma_Q$，则 $E$ 上的测度 $\mu$ 被称为高斯分布。*

通过滥用语言，如果相关的 promeasure $\widetilde{\mu}$ 等于 $\Gamma_Q$，则 $E$ 上的有界测度 $\mu$ 将被称为具有方差 $Q$ 的高斯分布。

#### 注 {#int-ix-s6-n5-rem-1 .statement tag=09SF}

— 1) 令$E$为有限维向量空间，并令$\mu$为质量1的$E$的正测度，使得$E$属于到$\mathscr{L}^2(E, \mu)$上的每个线性形式。 One defines an element $m$ of $E$ and a positive quadratic form $V$ on $E'$ by the formulas
$$
\langle m, x' \rangle = \int_E \langle x, x' \rangle d\mu(x), \quad V(x') = \int_E \langle x - m, x' \rangle^2 d\mu(x).
$$
In the traditional terminology of Probability Theory, $m$ is called the *mean* and $V$ the *variance* of $\mu$; $\mu$ is said to be *centered* if $m = 0$.

现在让$a$是$E$的元素，并且$Q$是$E'$上的正二次方形式。让我们用$\Gamma_{a,Q}$像来表示翻译$x \mapsto x + a$下的度量$\Gamma_Q$。很容易看出，$\Gamma_{a,Q}$是质量1的$E$的正测度，其中傅里叶变换$x' \mapsto e^{i\langle a, x' \rangle - \frac{1}{2} Q(x')}$和平均值$a$。此外，下面的命题6暗示$Q$是$\Gamma_{a,Q}$的方差。传统上，$\Gamma_{a,Q}$ 是均值 $a$ 和方差 $Q$ 的高斯测度，$\Gamma_Q = \Gamma_{0,Q}$ 是方差 $Q$ 的“中心”高斯测度。由于我们只考虑“中心”高斯测度，因此我们将省略此限定符。

2) 设$Q$是局部凸空间$E$的对偶$E'$上的二次形式。如果$E$与傅里叶变换$e^{-Q/2}$存在配度，则二次形式$Q$必然为正：对于，函数$e^{-Q/2}$有界于$E'$；因此，对于每个$x' \in E'$，$\mathbf{R}$上的函数$t \mapsto e^{-t^2 Q(x')/2} = e^{-Q(tx')/2}$是有界的，从而$Q(x') \geq 0$。

3) $\mathbf{R}$ 的对偶与$\mathbf{R}$ 自然同构，$\mathbf{R}$ 上的正二次形式是形式 $t \mapsto at^2$ 与$a \geq 0$ 的函数。因此，对于每一个$a \geq 0$，在$\mathbf{R}$上都存在一个且唯一的有界测度$\gamma_a$，其傅里叶变换等于函数$t \mapsto e^{-at^2/2}$；通过滥用语言，$\gamma_a$被认为是*$\mathbf{R}$的高斯测度，方差为$a$*。

$\gamma_0$的傅里叶变换是常数1，从而$\gamma_0 = \varepsilon_0$（单位在$\mathbf{R}$原点的质量）。假设$a > 0$，用$u_a$线性映射$x \mapsto a^{1/2} x$表示；然后$\mathscr{F}\gamma_a = \mathscr{F}\gamma_1 \circ {}^t u_a$，从而$\gamma_a = u_a(\gamma_1)$。 引理2表明$\gamma_1$是密度$x \mapsto (2\pi)^{-1/2} e^{-x^2/2}$相对于勒贝格测度的测度；由此，人们很容易推断出

$$
(15) \quad d\gamma_a(x) = (2\pi a)^{-1/2} e^{-x^2/2a} dx .
$$

连续线性映射下的高斯测度的像是高斯测度。更准确地说，我们得到以下结果：

#### 命题 5 {#int-ix-s6-prop-5 .statement tag=09SG}

*设E和E₁为两个局部凸空间，u为E到E₁的连续线性映射。令 Q 为 E' 上的正二次方程形式，Q₁ 为 E'₁ 上的正二次方程形式 Q $\circ {}^t u$。然后$u(\Gamma_Q) = \Gamma_{Q_1}$.*

集合$\mu = u(\Gamma_Q)$。通过No. 3的公式(4)，

$$
\mathscr{F}\mu = (\mathscr{F}\Gamma_Q) \circ {}^t u = e^{-Q/2} \circ {}^t u = e^{-Q_1/2} = \mathscr{F}\Gamma_{Q_1} ,
$$

从而 $\mu = \Gamma_{Q_1}$ 根据 No. 3 的第 3 号提案。

#### 推出{#int-ix-s6-n5-cor-1 .statement tag=09SH}

*设 E 为局部凸空间，Q 为 E' 上的正二次方形式。对于每个$x' \in E'$，$x'$下的$\Gamma_Q$的像是$\mathbf{R}$上的高斯测度，方差为$Q(x')$。*

#### 命题 6 {#int-ix-s6-prop-6 .statement tag=09SI}

*设 E 为局部凸空间，$\mu$ E 上的高斯测度，方差为 Q。对于每个整数 $n \geq 0$ 和每个 $x' \in E'$，都有关系*

$$
\begin{align*}
(16) & \quad \int_E |\langle x, x' \rangle|^n d\mu(x) = \pi^{-1/2} 2^{n/2} \Gamma\left( \frac{n+1}{2} \right) Q(x')^{n/2} \\
(17) & \quad \int_E \langle x, x' \rangle^{2n} d\mu(x) = \frac{(2n)!}{2^n n!} Q(x')^n \\
(18) & \quad \int_E \langle x, x' \rangle^{2n+1} d\mu(x) = 0 .
\end{align*}
$$

*特别是，*

$$
(19) \quad \int_E \langle x, x' \rangle^2 d\mu(x) = Q(x') \qquad (x' \in E') .
$$

如果这些公式对于 $E'$ 的元素 $x'$ 为真，那么它们对于其所有倍数 $t \cdot x'$ 都为真（其中 $t$ 为实数）。因此，当 $Q(x')$ 等于 0 或 1 时，我们可能会满足于建立它们。

a) 假设$Q(x') = 0$。度量值$x'(\mu)$等于$\gamma_0 = \varepsilon_0$，因此$x'$等于零$\mu$——几乎无处不在； 公式 (16) 到 (19) 则显而易见。

b) 假设$Q(x') = 1$，从而$x'(\mu) = \gamma_1$。然后
$$
\int_E |\langle x, x' \rangle|^n d\mu(x) = \int_{\mathbf{R}} |t|^n d\gamma_1(t) = (2\pi)^{-1/2} \int_{\mathbf{R}} |t|^n e^{-t^2/2} dt
$$
(16) 紧随 (6) (No 4, 引理 1)。类似地，从（7）和（8）得出公式（17）和（18）。最后由(17)中的设定$n = 1$得到(19)。

我们现在可以证明 Cor 的逆命题。提案 5。

#### 命题 7 {#int-ix-s6-prop-7 .statement tag=09SJ}

*设 E 为局部凸空间，$\mu$ E 上的算子。假设 $x'(\mu)$ 是$\mathbf{R}$ 对于每个 $x' \in E'$ 的高斯测度。那么 $\mu$ 是 E 上的高斯测度。*

对于每个$x' \in E'$，令$Q(x')$为$\mathbf{R}$上高斯测度$x'(\mu)$的方差。一个有$x'(\mu) = \gamma_{Q(x')}$，从而
$$
(\mathscr{F}\mu)(x') = \int_{\mathbf{R}} e^{it \cdot 1} d\gamma_{Q(x')}(t) = e^{-Q(x') \cdot 1^2 / 2}
$$
由 $\mathscr{F}\mu$ 的定义 (No. 3, 公式 (2))。其他字、$\mathscr{F}\mu = e^{-Q/2}$，还有待证明$Q$是$E'$上的正二次形式。

对于 E 与有限余维的每个闭线性子空间 V，用 E 到 $E/V$ 的 $p_V$ 典范映射表示，用 $\mu_V$ $E/V$ 上的测度$p_V(\mu)$ 和集合表示$Q_V = Q \circ {}^t p_V$。由于$E' = \bigcup_{V \in \mathscr{F}(E)} \operatorname{Im}({}^t p_V)$和${}^t p_V$是单射的，因此足以证明$Q_V$是$(E/V)'$上的正二次方形式。设$u \in (E/V)'$和$x' = {}^t p_V(u)$。我们有
$$
u(\mu_V) = u(p_V(\mu)) = x'(\mu) = \gamma_{Q(x')} ;
$$
那么，命题 6 意味着
$$
Q_V(u) = Q(x') = \int_{\mathbf{R}} t^2 d\gamma_{Q(x')}(t) = \int_{E/V} u(x)^2 d\mu_V(x),
$$
因此$Q_V$是$(E/V)'$的正二次方形式。

### 6. 例高斯算子

1) 令 E 为真正的希尔伯特空间。 映射 $x' \mapsto \|x'\|^2$ 是 $E'$ 上的正二次方形式。 相应的高斯测度被称为 E 上的*规范高斯测度*。可以证明，如果 E 是无限维的，则该测度不是测度。

令 $A$ 为 $E$ 上的连续线性算子。 映射 $x' \mapsto \|{}^tA \cdot x'\|^2$ 是 $E'$ 上的正二次方形式。当且仅当$A$是希尔伯特-施密特算子时，相应的promeasure$\mu_A$ on $E$是一个测度（cf.No. 11，Th.3的Cor.2）。

2) *正型的核。*设$T$为集合，$T$上的实函数的$E = \mathbf{R}^T$向量空间，配备逐点收敛的拓扑。对于每个 $t \in T$，1 表示 $E$ 上的 $\varepsilon_t$ 线性形式 $f \mapsto f(t)$。族$(\varepsilon_t)_{t \in T}$是$E'$的基（TVS，II, §6, No. 6，第8号提案的Cor.2）。

在$T$上对$T \times T$满足关系上的每一个实数函数$K$调用（实数）核或正值型

$$
\text{(20)} \qquad K(t, t') = K(t', t) \quad \text{for } t, t' \text{ in } T,
$$
$$
\text{(21)} \qquad \sum_{i,j=1}^p c_i c_j K(t_i, t_j) \geqslant 0
$$

对于 $T$ 中的任意正整数 $p$、元素 $t_1, \ldots, t_p$ 和实数 $c_1, \ldots, c_p$。如果是这样的话公式

$$
\text{(22)} \qquad q\left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t,t' \in T} c_t c_{t'} K(t, t')
$$

定义 $E'$ 上的正二次形式。相反，如果$q$是$E'$上的正二次形式，则公式

$$
\text{(23)} \qquad K(t, t') = \frac{1}{2} [q(\varepsilon_t + \varepsilon_{t'}) - q(\varepsilon_t) - q(\varepsilon_{t'})]
$$

$T$ 上的正型定义核 $K$。由此，在$T$上的正型的核的集合和$E'$上的正二次方形式之间，得到两个互为逆双射。

令 $K$ 为 $T$ 上的正型的核，$q$ 为 $E'$ 上的相关二次方形式。 $E$ 上具有方差 $q$ 的高斯测度也称为*$E$ 上具有协方差* $K$ 的高斯测度。如果$T$是可数的，No. 1的命题2意味着这个测度是一个测度。

3) 令$T$为可数集合。正型的$T$上的核$\delta$由设定定义

$$
\text{(24)} \qquad \delta(t, t') = \begin{cases}
1 & \text{if } t = t' \\
0 & \text{if } t \neq t'.
\end{cases}
$$

相应的二次形式由$q\left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t \in T} c_t^2$ 给出。对于每个$t \in T$，让我们用$\mu_t$表示$\mathbf{R}$上方差为1的高斯测度；

很容易证明，$\mathbf{R}^T$ 上协方差为 $\delta$ 的高斯测度等于 $\bigotimes_{t \in T} \mu_t$。

4) 设$n \geq 1$为整数。如果阶 $n$ 是对称的，则称平方矩阵 $C = (c_{ij})$ 为“正对称”，对于任何实数 $x_1, \ldots, x_n$ 则称$\sum_{i,j=1}^n c_{ij} x_i x_j \geq 0$；同样的，映射$(i, j) \mapsto c_{ij}$是核在集合$\{1, 2, \ldots, n\}$上的正型。因此，我们可以谈论 $\mathbf{R}^n$ 上的高斯测度 $\gamma_C$，协方差为 $C$；其特点是公式

$$
(25) \quad \int_{\mathbf{R}^n} e^{i(x_1 t_1 + \cdots + x_n t_n)} d\gamma_C(t_1, \ldots, t_n) = \exp \left( - \frac{1}{2} \sum_{j,k=1}^n c_{jk} x_j x_k \right),
$$

对于 $x_1, \ldots, x_n$ 实数。由No. 5(公式(19))的第6条推论

$$
(26) \quad \int_{\mathbf{R}^n} t_j t_k d\gamma_C(t_1, \ldots, t_n) = c_{jk} \quad (1 \leq j, k \leq n).
$$

从No. 5的第5条命题，推导出公式

$$
(27) \quad u(\gamma_C) = \gamma_{UC^t U},
$$

其中$u$是$\mathbf{R}^n$到$\mathbf{R}^m$的线性映射和矩阵$U$。此外，我们很容易看出（No. 5第四条命题cf.第一个证明的第一个部分），如果$I_n$是阶$n$的恒等式矩阵，那么测度$\gamma_{I_n}$承认密度

$$
(2\pi)^{-n/2} \exp \left( - \frac{1}{2}(t_1^2 + \cdots + t_n^2) \right)
$$

关于$\mathbf{R}^n$的勒贝格测度$\lambda_n$。

我们将证明，如果矩阵 $C$ 是可逆的，并且 $D = (d_{jk})$ 是可逆的，那么

$$
(28) \quad d\gamma_C(t_1, \ldots, t_n) =
(2\pi)^{-n/2} (\det D)^{1/2} \left( \exp \left( - \frac{1}{2} \sum_{j,k=1}^n d_{jk} t_j t_k \right) \right) dt_1 \cdots dt_n.
$$

因为，如果 $C$ 可逆，则 $\mathbf{R}^n$ 上的二次形式 $q$ 定义为

$$
q(x_1, \ldots, x_n) = \sum_{j,k=1}^n c_{jk} x_j x_k
$$

是非简并的。利用$\mathbf{R}^n$正交于$q$的基的存在性，证明阶$n$的平方矩阵$U$的存在性使得$C = U \cdot {}^tU$、从而$\gamma_C = u(\gamma_{I_n})$通过(27) （其中$u$表示$\mathbf{R}^n$与矩阵$U$的自同构）。令 $Q$ 为 $\mathbf{R}^n$ 的二次方形式，定义为
$$
Q(t_1, \ldots, t_n) = t_1^2 + \cdots + t_n^2;
$$
然后
$$
\gamma_{I_n} = (2\pi)^{-n/2} e^{-Q/2} \cdot \lambda_n,
$$
从而
$$
u(\gamma_{I_n}) = (2\pi)^{-n/2} e^{-(Qou^{-1})/2} \cdot u(\lambda_n).
$$
形式$Q \circ u^{-1}$在$\mathbf{R}^n$上的二次方直接的在点$(t_1, \ldots, t_n)$处取值$\sum_{j,k=1}^n d_{jk} t_j t_k$，以及第15章的提案。 VII, §1, No. 10表明
$$
u(\lambda_n) = (\det U)^{-1} \cdot \lambda_n = (\det D)^{1/2} \cdot \lambda_n.
$$
由此得出公式 (28)。

### 7. 维纳测度

在这个数中，我们用$T$表示$\mathbf{R}$的区间$]0, 1]$，用$\mathscr{H}$表示实数函数在$T$可平方可积的关于勒贝格测度的希尔伯特空间，其中标量乘积表示$(f|g)$。我们还用$T$上的连续实数函数的$\mathscr{C}$空间表示，在点0处趋于0；我们为$\mathscr{C}$配备了范数$\|f\| = \sup_{t \in T} |f(t)|$。紧区间 $[0, 1] = T \cup \{0\}$ 是局部紧但非紧区间 $T$ 的 Alexandroff 紧致化；因而，具有紧支撑的$T$上的连续函数的集合在$\mathscr{C}$中密集，并且$\mathscr{C}$的对偶可以用$T$上的有界测度（不一定是正数）的空间$\mathscr{M}^1$来识别（Ch. III, §1, No. 8，Def. 3）。

对于每函数 $f \in \mathscr{H}$，$T$ 上有一个定义函数 $Pf$
$$
(Pf)(t) = \int_0^t f(x) \, dx = (f|I_t),
$$
其中$I_t$是区间$]0, t]$的特征函数。柯西-施瓦茨不等式意味着不等式
$$
|(Pf)(t)| \leq \|f\|_2 \cdot t^{1/2}
$$
$$
|(Pf)(t) - (Pf)(t')| \leq \|f\|_2 \cdot |t - t'|^{1/2};
$$

因而，$Pf$属于到$\mathscr{C}$，以及$\mathscr{H}$到$\mathscr{C}$的线性映射$P$与范数$\leqslant 1$连续。

让我们认同希尔伯特空间$\mathscr{H}$及其对偶（TVS，V, §1, No. 7，Th.3），并用$P : \mathscr{H} \to \mathscr{C}$的$\Pi : \mathscr{M}^1 \to \mathscr{H}$转置表示。对于每个测量$\mu \in \mathscr{M}^1$和每个函数$f \in \mathscr{H}$，我们有

$$
(\Pi \mu | f) = \mu(Pf) = \int_{\mathbf{T}} d\mu(t) \int_{\mathbf{T}} I_t(x) f(x) \, dx
$$
$$
= \int_{\mathbf{T}} f(x) \, dx \int_{\mathbf{T}} I_t(x) \, d\mu(t)
$$

由勒贝格-富比尼定理。现在，

$$
I_t(x) = \begin{cases}
1 & \text{if } 0 < x \leq t \leq 1 \\
0 & \text{otherwise},
\end{cases}
$$

终于从而

(34) $$ (\Pi \mu)(x) = \mu([x, 1]) \quad \text{for } x \in \mathbf{T}. $$

令$\mu, \nu$位于$\mathscr{M}^1$中。然后

$$
(\Pi \mu | \Pi \nu) = \int_{\mathbf{T}} \Pi \mu(x) \Pi \nu(x) \, dx = \int_{\mathbf{T}} dx \int_{\mathbf{T}} I_t(x) \, d\mu(t) \int_{\mathbf{T}} I_{t'}(x) \, d\nu(t')
$$
$$
= \int_{\mathbf{T}} \int_{\mathbf{T}} d\mu(t) \, d\nu(t') \int_{\mathbf{T}} I_t(x) I_{t'}(x) \, dx.
$$

现在，$I_t \cdot I_{t'}$是区间$]0, t] \cap ]0, t']$的特征函数，立即从而

(35) $$ \int_{\mathbf{T}} I_t(x) I_{t'}(x) \, dx = \inf(t, t'). $$

由此可见

(36) $$ (\Pi \mu | \Pi \nu) = \int_{\mathbf{T}} \int_{\mathbf{T}} \inf(t, t') \, d\mu(t) \, d\nu(t'). $$

根据前面的结果，一个定义在$\mathscr{M}^1$乘公式的正二次形式$W$

(37) $$ W(\mu) = \int_{\mathbf{T}} \int_{\mathbf{T}} \inf(t, t') \, d\mu(t) \, d\mu(t') = \| \Pi \mu \|_2^2. $$

特别是，如果 $t_1, \ldots, t_n$ 是 T 的元素，且 $c_1, \ldots, c_n$ 是实数，则
$$
W \left( \sum_{j=1}^n c_j \varepsilon_{t_j} \right) = \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k)
$$
并且由于 W 是正数，因此 T 上的函数 $(t, t') \mapsto \inf(t, t')$ 是正型的核。

**定理 1 (维纳).** — *令 w 为希尔伯特空间 $\mathscr{H}$ 正则高斯测度的$P : \mathscr{H} \to \mathscr{C}$下的像。那么 w 是 $\mathscr{C}$ 上的高斯测度，方差为 W。*

构造、$W(\mu) = \|^tP(\mu)\|_2^2$； No. 5的命题5表明，w是方差为W的高斯测度。还需要证明w是$\mathscr{C}$上的测度。

A) *构造辅助测量空间*^{(2)} $(\Omega, m)$：
对于每个整数$n \geqslant 0$，用形式$k/2^n$的数和$k = 1, 2, 3, \ldots, 2^n$表示$D_n$集合。 集合 $D = \bigcup_{n \geqslant 0} D_n$（T 中包含的二元数的集合）和$\Omega = \mathbf{R}^D$。对于每个$t \in D$，在$\Omega$上用$X(t)$线性形式$f \mapsto f(t)$表示。

对于D中的$t, t'$，集合$M(t, t') = \inf(t, t')$；我们已经看到，M 是 D 上正型的核。由于集合 D 是可数的，因此可以用协方差 M (No. 6, *例 2*) 定义 $\Omega$ 上的高斯*测量* m。

#### 引理 3 {#int-ix-s6-lem-3 .statement tag=09SK}

*对于 D 中的任意 $t, t'$，
$$
\int_\Omega \left| X\left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2} \right|^3 dm = \frac{1}{(8\pi)^{1/2}} |t - t'|^{3/2}.
$$
注，$\frac{t + t'}{2}$属于到D。人们知道（No. 6，*例2*）族$(X(t))_{t \in D}$是$\Omega$的拓扑对偶$\Omega'$的基；因此，在$\Omega' \times \Omega'$上存在对称双线性形式$\widehat{M}$，其特征为$\widehat{M}(X(t), X(t')) = \inf(t, t')$。到构造时，$\Omega$ 上的高斯测度 m 的方差是 $\Omega'$ 上的二次方形式 $\xi \mapsto \widehat{M}(\xi, \xi)$。 集合，特别是，
$$
\xi = X\left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2};
$$
简单计算得出
$$
\widehat{M}(\xi, \xi) = \frac{|t - t'|}{4}.
$$

(2) *Espace mesuré*：一个局部紧凑的空间，配有一个措施（第III，第 1 版，§2, No. 2，p. 52）。

根据No. 5(公式(16))第6条，

$$
\int_{\Omega} |\xi|^3 \, dm = \pi^{-1/2} 2^{3/2} \Gamma(2) \widehat{M}(\xi, \xi)^{3/2};
$$

引理紧随公式 (40) 和 (41)。

B) *将$\Omega$的映射u构造转化为$\mathscr{C}$：*
对于每个整数$n \geqslant 0$，用函数形成的$\mathscr{C}$的$E_n$子空间表示，它们在$1 \leqslant k \leqslant 2^n$的每个区间$\left[ \frac{k-1}{2^n}, \frac{k}{2^n} \right]$上仿射。 $\mathbf{R}$ 紧致区间 I 上的仿射函数在I 端点处达到其边界；因而，

$$
\|f\| = \sup_{1 \leqslant k \leqslant 2^n} \left| f\left( \frac{k}{2^n} \right) \right|
$$

$f \in E_n$。

对于每一个函数$g \in \Omega$和每一个整数$n \geqslant 0$，存在且仅有一个函数$u_n(g)$，属于到$E_n$和重合以及每点的$g$ $D_n$；我们将写$T_n g = u_{n+1}(g) - u_n(g)$。由于$D_n$是有限的，$\Omega$到$\mathscr{C}$的映射$T_n$是连续的，因而$m$是可测的。

#### 引理 4 {#int-ix-s6-lem-4 .statement tag=09SL}

— *对于每个整数 $n \geqslant 0$，*

$$
\int_{\Omega} \|T_n g\|^3 \, dm(g) \leqslant \frac{1}{(8\pi)^{1/2}} 2^{-n/2}.
$$

设$g \in \Omega$和$n \in \mathbf{N}$。一个有$E_n \subset E_{n+1}$；因而，函数$T_n g$属于到$E_{n+1}$，并且在$D_n$的每点处为零；因而，根据 (42)，

$$
\|T_n g\|^3 = \sup_{1 \leqslant k \leqslant 2^n} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \leqslant \sum_{k=1}^{2^n} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3.
$$

让我们约定$g(0) = 0$。 $u_n(g)$的构造通过$g$的线性插值意味着关系

$$
T_n g\left( \frac{2k-1}{2^{n+1}} \right) = g\left( \frac{2k-1}{2^{n+1}} \right) - \frac{1}{2} \left( g\left( \frac{k-1}{2^n} \right) + g\left( \frac{k}{2^n} \right) \right)
$$

$1 \leqslant k \leqslant 2^n$。由此，通过积分推论，

$$
\int_{\Omega} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \, dm(g) = \int_{\Omega} \left| X\left( \frac{2k-1}{2^{n+1}} \right) - \frac{1}{2} \left( X\left( \frac{k-1}{2^n} \right) + X\left( \frac{k}{2^n} \right) \right) \right|^3 \, dm;
$$

!【图1](../images/figure_1.png)

图1

然后可以应用引理 3 和 $t = \frac{k-1}{2^n}$、$t' = \frac{k}{2^n}$、从而

$$
\int_{\Omega} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^{-\frac{3n}{2}} .
$$

由(44)，我们有

$$
\int_{\Omega} \| T_n g \|^3 dm(g) \leq \sum_{k=1}^{2^n} \int_{\Omega} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^n \cdot 2^{-\frac{3n}{2}} ,
$$

从而引理。

由引理 4、$\Omega$的映射$T_n$进入巴纳赫空间$\mathscr{C}$属于至$L^3_{\mathscr{C}}(\Omega, m)$和$N_3(T_n) \leq \frac{1}{(8\pi)^{1/6}} (2^{-1/6})^n$、从而$\sum_{n=0}^{\infty} N_3(T_n) < +\infty$。根据第 6 章的提案。 IV, §3, No. 3，存在集合$\Omega_0 \subset \Omega$，使得$\Omega - \Omega_0$可以忽略$m$，并且对于每个$g \in \Omega_0$，级数$\sum_{n=0}^{\infty} T_n(g)$绝对收敛于$\mathscr{C}$。然后将$\Omega$的定义和$m$可测量的映射$u$转化为$\mathscr{C}$

$$
u(g) = \begin{cases}
\sum_{n=0}^{\infty} T_n g = \lim_{n \to \infty} u_n(g) & \text{for } g \in \Omega_0 \\
0 & \text{for } g \in \Omega - \Omega_0 .
\end{cases}
$$

由于$0 \leq m \leq n$在$D_m \subset D_n$上有$u_n(g)$和$g$重合，对于每个$g \in \Omega_0$，$u(g)$到$D$的限制等于$g$，因此直接的。

C) 构造 $\mathscr{C}$ 上的高斯测度：
令 $w'$ 为 $\mathscr{C}$ 上的有界测度，即 $m$ 可测映射 $u : \Omega \to \mathscr{C}$ 下 $m$ 的像。 我们将证明$w'$是$\mathscr{C}$的高斯测度，方差为$W$、从而$w = w'$。 用$\mathscr{D}$表示$\mathscr{M}^1$的线性子空间，该线性子空间由$t$的测量$\varepsilon_t$生成超过$D$。

#### 引理 5 {#int-ix-s6-lem-5 .statement tag=09SM}

对于每一个度量$\mu \in \mathscr{D}$，

$$
\int_{\mathscr{C}} e^{i \langle f, \mu \rangle} \, dw'(f) = e^{-W(\mu)/2}.
$$

集合 $\mu = c_1 \varepsilon_{t_1} + c_2 \varepsilon_{t_2} + \cdots + c_n \varepsilon_{t_n}$，其中$t_1, \ldots, t_n$位于$D$，$c_1, \ldots, c_n$位于$\mathbf{R}$。对于每个 $g \in \Omega_0$、函数 $u(g)$ 重合，其中 $g$ 位于 $D$；所以

$$
\langle u(g), \mu \rangle = \sum_{j=1}^n c_j g(t_j) \qquad (g \in \Omega_0).
$$

还，

$$
W(\mu) = \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k),
$$

并且，由于 $m$ 是 $\Omega$ 的高斯测度，协方差为 $M$，并且 $\Omega - \Omega_0$ $m$ 可忽略不计，因此我们有

$$
\int_{\Omega_0} e^{i \sum_{j=1}^n c_j g(t_j)} \, dm(g) = \exp \left( - \frac{1}{2} \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k) \right).
$$

现在，$\Omega - \Omega_0$ $m$ 可以忽略不计，$w' = u(m)$；由此可见

$$
\int_{\mathscr{C}} e^{i \langle f, \mu \rangle} \, dw'(f) = \int_{\Omega_0} e^{i \langle u(g), \mu \rangle} \, dm(g).
$$

公式 (48) 紧随公式 (49) 到 (52)。

#### 引理 6 {#int-ix-s6-lem-6 .statement tag=09SN}

让$\mu \in \mathscr{M}^1$。存在序列措施$\mu_n \in \mathscr{D}$，使得$\mu(f) = \lim_{n \to \infty} \mu_n(f)$ 对于所有$f \in \mathscr{C}$ 和$W(\mu) = \lim_{n \to \infty} W(\mu_n)$。

让$I = [0, 1]$。 $T = ]0, 1[$上的有界测度的空间$\mathscr{M}^1$将被识别为$\mathscr{M}(I)$的子空间，该测度由在$0$放置没有权的测度形成。 (3) 我们为$\mathscr{M}(I)$配备了模糊的拓扑。 映射

(3) 即$I$上的措施集中在$T = I - \{0\}$上。

$I$到$\mathscr{M}(I)$的$t \mapsto \varepsilon_t$是连续的（第III, §1, No. 9章，第13条命题）；由于 D 在 I 中是稠密的，因此 $\mathscr{D}$ 包含的闭包 $\overline{\mathscr{D}}$ 所有点措施。令 A 为 $\nu \in \mathscr{D}$ 的集合，使得 $\| \nu \| \leq \| \mu \|$；措施$\mu$位于A的闭包中（第III, §2, No. 4章，Th.1的Cor.1）。 集合 A 在 $\mathscr{M}(I)$ 中相对紧致（第 III, §1, No. 9，第 15 章），而 $\mathscr{M}(I)$ 的紧致子集是可度量的（TVS，III, §3, No. 4，第 6 条第（4）条的 Cor.2 和 GT，X, §3, No. 3，Th.1）。因此，在$\mathscr{M}(I)$中存在序列个测度$\mu_n \in A$收敛于$\mu$。由于 $\mathscr{C}$ 与原点 I 零上的连续函数的子空间进行识别，因此对于所有 $f \in \mathscr{C}$，我们都有 $\mu(f) = \lim_{n \to \infty} \mu_n(f)$。此外，由于$\mathscr{C}(I) \otimes \mathscr{C}(I)$在范数空间$\mathscr{C}(I \times I)$（第III, §4, No. 1，引理1）中是密集的，关系$\lim_{n \to \infty} \mu_n = \mu$和$\| \mu_n \| \leq \| \mu \|$意味着$\lim_{n \to \infty} (\mu_n \otimes \mu_n) = \mu \otimes \mu$（第III, §1, No. 10，提案 17)；由于措施 $\mu_n$ 和 $\mu$ 将权置于 0，我们有

$$
W(\mu_n) = \int_I \int_I \inf(t, t') d\mu_n(t) d\mu_n(t'),
$$
$$
W(\mu) = \int_I \int_I \inf(t, t') d\mu(t) d\mu(t'),
$$

从而$\lim_{n \to \infty} W(\mu_n) = W(\mu)$。

还需要证明$w'$的傅里叶变换等于$e^{-W/2}$。令 $\mu \in \mathscr{M}^1$； 选择测量$\mu_n \in \mathscr{D}$，如引理 6。测量$w'$是有界的，并且$|e^{i \langle f, \mu_n \rangle}| = 1$对于所有$n$； 引理 5 和勒贝格收敛定理（Ch. IV, §4, No. 3，Th. 2）则意味着

$$
\int_{\mathscr{C}} e^{i \langle f, \mu \rangle} dw'(f) = \lim_{n \to \infty} \int_{\mathscr{C}} e^{i \langle f, \mu_n \rangle} dw'(f)
= \lim_{n \to \infty} e^{-W(\mu_n)/2} = e^{-W(\mu)/2}.
$$

Q.E.D.

$\mathscr{C}$上的$w$测度，其傅里叶变换等于$e^{-W/2}$，称为*$\mathscr{C}$*上的维纳测度。

#### 注 {#int-ix-s6-n7-rem-1 .statement tag=09SO}

— 对于 T 中包含的每个半开区间$J = ]a, b]$，让我们集合$l(J) = b - a$（J 的长度）并在$\mathscr{C}$上用$A_J$线性形式$f \mapsto f(b) - f(a)$表示。可以证明，维纳测度具有以下性质的特征：

*令 $J_1, \ldots, J_n$ 为包含在 T 和成对不相交的中的半开区间。 $\mathscr{C}$到$\mathbf{R}^n$的线性映射$f \mapsto (A_{J_1}(f), \ldots, A_{J_n}(f))$下的测量w的像等于$\gamma_{a_1} \otimes \cdots \otimes \gamma_{a_n}$，$a_i = l(J_i)^{1/2}$对于$1 \leq i \leq n$。*

### 8. 傅里叶变换的连续性

#### 命题 8 {#int-ix-s6-prop-8 .statement tag=09SP}

— 令 E 为局部凸空间，$\mu$ E 的比例，$\Phi$ 傅里叶变换为 $\mu$。一个人存在不平等

$$
|\Phi(x')| \leq \Phi(0)
$$
$$
|\Phi(x') - \Phi(y')|^2 \leq 2\Phi(0)\left(\Phi(0) - \Re \Phi(x' - y')\right)
$$

$E'$ 中的 $x', y'$。

No. 3的公式(5)允许简化为E是有限维且$\mu$是测度的情况。然后

$$
|\Phi(x')| = \left| \int_E e^{i\langle x, x' \rangle} d\mu(x) \right| \leq \int_E |e^{i\langle x, x' \rangle}| d\mu(x) = \int_E d\mu(x) = \Phi(0),
$$

从而 (53)。此外，如果$a$和$b$是实数，那么

$$
|e^{ia} - e^{ib}|^2 = |e^{ib}|^2|e^{i(a-b)} - 1|^2 = (e^{i(a-b)} - 1)(e^{-i(a-b)} - 1) = 2 - 2\cos(a - b);
$$

根据柯西-施瓦茨不等式，我们有

$$
|\Phi(x') - \Phi(y')|^2 = \left| \int_E (e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}) d\mu(x) \right|^2
$$
$$
\leq \int_E |e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}|^2 d\mu(x) \int_E 1^2 d\mu(x)
$$
$$
= \int_E (2 - 2\cos\langle x, x' - y' \rangle)) d\mu(x) \cdot \Phi(0)
$$
$$
= 2\Phi(0)\left(\Phi(0) - \Re \Phi(x' - y')\right),
$$

从而 (54)。

#### 推论{#int-ix-s6-n8-cor-1 .statement tag=09SQ}

— 为$E'$配备与其向量空间结构兼容的拓扑。为了使 $\Phi$ 连续，其实数部分 $\Re \Phi$ 在原点连续是必要且充分的，在这种情况下 $\Phi$ 是一致连续的。

这是从不等式 (54) 得出的。

令 F 为局部凸空间。我们为F的对偶$F'$配备拓扑，与F和$F'$之间的对偶性兼容，并且我们为认同F配备$F'$的对偶。因而，$F'$上的有界测度$\mu$的傅里叶变换是F上的函数$\mathscr{F}\mu$，定义为

$$
(\mathscr{F}\mu)(x) = \int_{F'} e^{i\langle x, x' \rangle} d\mu(x').
$$

#### 命题 9 {#int-ix-s6-prop-9 .statement tag=09SR}

— *如果 F 是桶状的，则 F' 上每个有界测度的傅里叶变换是 F* 上均匀连续的函数。

令$\mu$为$F'$的有界测度，$\Phi$为傅里叶变换。让$\varepsilon > 0$。存在 $F'$ 的紧子集 K，使得 $\mu(F' - K) \leq \varepsilon$。现在，K 对于弱拓扑 $\sigma(F', F)$ 是紧致的，因此是等连续的，因为 F 是桶形的（TVS，III, §4, No. 2，Th.1）。因而，F 中存在一个对称邻域 U 为 0，其极坐标为 $U^\circ$ 包含 K。设 x 在 $\varepsilon U$ 内；然后

$$
\Phi(0) - \Re \Phi(x) = \int_{F'} (1 - \cos \langle x, x' \rangle) d\mu(x').
$$

现在，每个$x' \in F' - K$对应$0 \leq 1 - \cos \langle x, x' \rangle \leq 2$，并且

$$
1 - \cos \langle x, x' \rangle \leq \frac{1}{2} \langle x, x' \rangle^2 \leq \frac{\varepsilon^2}{2}
$$

$x' \in K \subset U^\circ$；由此可见

$$
0 \leq \Phi(0) - \Re \Phi(x) \leq 2 \mu(F' - K) + \frac{\varepsilon^2}{2} \mu(K) \leq 2\varepsilon + \frac{\varepsilon^2}{2} \mu(F').
$$

这个不等式的第二个成员随着$\varepsilon$趋于0；因而 $\Re \Phi$ 在 0 处连续，命题由 Cor 得出。提案 8。

### 9. 米洛斯的引理

令 T 为有限维向量空间且 $\mu$ 为 $T'$ 上的有界测度；我们将认同 T 与$T'$ 进行对偶，使得$\mu$ 的傅里叶变换 $\Phi$ 是T 上的函数。我们假设给定T 上的两个正二次方形式 h 和q 以及数 $\varepsilon > 0$。对于每个实数$r > 0$，我们用$x' \in T'$的$C_r$集合表示，这样$\langle x, x' \rangle^2 \leq r^2 h(x)$代表所有$x \in T$。

#### 命题 10 {#int-ix-s6-prop-10 .statement tag=09SS}

— *在假设 $\Phi(0) - \Re \Phi \leq \varepsilon + q$ 下，我们有*

$$
\mu(T' - C_r) \leq 3 (\varepsilon + r^{-2} \operatorname{Tr}(q/h))
$$

*对于每个*$r > 0$。

q 右 h 的迹可写为 $\operatorname{Tr}(q/h)$（cf. 附件，No. 1）。当 $\operatorname{Tr}(q/h)$ 无穷大时，公式 (55) 是微不足道的。从此以后，我们假设 $\operatorname{Tr}(q/h)$ 是有限的，因而 $h(x) = 0$ 意味着 $x \in T$ 的 $q(x) = 0$。

令$a_1, \ldots, a_n$为$T$的元素，且$D$集合为$x' \in T'$，使得$\sum_{j=1}^n \langle a_j, x' \rangle^2 > 1$。对于每个实数$t \geq 0$，我们都有$3(1 - e^{-t/2}) \geq 0$，甚至还有

$$
3(1 - e^{-t/2}) \geq 3(1 - e^{-1/2}) \geq 3\left(1 - \left(\frac{9}{4}\right)^{-1/2}\right) = 1
$$

对于$t > 1$，因为$e > \frac{9}{4}$。 应用这些不等式到$t = \sum_{j=1}^n \langle a_j, x' \rangle^2$，我们得到

$$
\mu(D) \leq 3 \int_{T'} \left(1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right)\right) d\mu(x').
$$

令 $\gamma$ 为 $\mathbf{R}$ 的测度，相对于勒贝格测度，具有密度 $t \mapsto (2\pi)^{-1/2} e^{-t^2/2}$。截至引理 2 / No. 4，

$$
\int_{\mathbf{R}} e^{iut} d\gamma(t) = e^{-u^2/2}
$$

对于所有真实的$u$。因而，

$$
\begin{align*}
1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right) \\
&= \int \cdots \int \left(1 - e^{i \sum_{j=1}^n \langle a_j, x' \rangle t_j}\right) d\gamma(t_1) \cdots d\gamma(t_n)
\end{align*}
$$

对于所有$x' \in T'$。要整合到第二个成员中的$x', t_1, \ldots, t_n$的函数是连续的，并且在绝对值上以2为界，并且度量$\mu$和$\gamma$有界；因而，我们可以对$d\mu(x')$整的(57)的两个成员，并互换对$\mu$和$\gamma$的积分；一个获得

$$
\begin{align*}
\int_{T'} \left(1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right)\right) d\mu(x') \\
&= \int \cdots \int \left(\Phi(0) - \Phi\left(\sum_{j=1}^n t_j a_j\right)\right) d\gamma(t_1) \cdots d\gamma(t_n).
\end{align*}
$$

由于$q$是$T$上的二次形式，因此存在实数$q_{jk}$使得
$$
q \left( \sum_{j=1}^n t_j a_j \right) = \sum_{j,k} q_{jk} t_j t_k
$$
$t_1, \ldots, t_n$真实；特别是，$q_{jj} = q(a_j)$代表$1 \leq j \leq n$。此外，对于$n = 0, 1, 2$，整的$\int_{\mathbf{R}} t^n d\gamma(t)$分别有值 1、0、1（No. 4、引理 1）。由此，立即推断出
$$
\int \cdots \int \left( \varepsilon + q \left( \sum_{j=1}^n t_j a_j \right) \right) d\gamma(t_1) \ldots d\gamma(t_n) = \varepsilon + \sum_{j=1}^n q(a_j).
$$
现在，(58)和$\Phi(0)$的第一个成员是实数；因而，在（58）的第二个成员中，可以通过替换$\Phi$乘$\Re \Phi$。 不等式 $\Phi(0) - \Re \Phi \leq \varepsilon + q$ 和公式 (56), (58) 和 (59) 那么意味着
$$
\mu(D) \leq 3 \left( \varepsilon + \sum_{j=1}^n q(a_j) \right).
$$
让我们修复数$r > 0$。由于二次方形式 $h$ 为正，因此在 0 和 $n$ 之间存在 $T$ 和整数 $m$ 的基 $(e_1, \ldots, e_n)$，使得
$$
h \left( \sum_{j=1}^n t_j e_j \right) = \sum_{j=1}^m t_j^2
$$
$t_1, \ldots, t_n$实数（附件，No. 1，提案2）。那么直接的 $C_r$ 由 $x' \in T'$ 组成，这样
$$
\sum_{j=1}^m \langle e_j, x' \rangle^2 \leq r^2, \qquad \sum_{j=m+1}^n \langle e_j, x' \rangle^2 = 0.
$$
对于每个整数 $l \geq 1$，令 $D_l$ 为 $x' \in T'$ 满足不等式中的集合
$$
\sum_{j=1}^m \langle r^{-1} e_j, x' \rangle^2 + \sum_{j=m+1}^n \langle l e_j, x' \rangle^2 > 1.
$$
人们很容易看出序列$(D_l)_{l \geq 1}$是递增与并$T' - C_r$，从而
$$
\mu(T' - C_r) = \lim_{l \to \infty} \mu(D_l).
$$

但到了(60)，

$$
\mu(D_l) \leq 3 \left( \varepsilon + \sum_{j=1}^m r^{-2} q(e_j) + \sum_{j=m+1}^n l^2 q(e_j) \right);
$$

对于$j = m+1, \ldots, n$，我们有$h(e_j) = 0$，因此$q(e_j) = 0$。此外，$\operatorname{Tr}(q/h) = \sum_{j=1}^m q(e_j)$（附件，No. 1，提案 2）。然后从 (61) 和 (62) 得出关系 (55)。

Q.E.D.

### 10.对核空间的双重措施

令 F 为局部凸空间。令$\mathscr{T}_s$为$F'$上的弱拓扑$\sigma(F', F)$，以及F的紧凸子集上一致收敛的$\mathscr{T}_c$拓扑。由Mackey的定理（TVS，IV, §1, No. 1，Th.1）拓扑$F'$上的$\mathscr{T}_s$和$\mathscr{T}_c$与F和$F'$之间的对偶性兼容；因此，对于$\mathscr{T}_s$和$\mathscr{T}_c$中间的$F'$上的每个局部凸拓扑$\mathscr{T}$也是如此。如果$\mathscr{T}$是这样的拓扑，并且$F'_{\mathscr{T}}$表示空间$F'$配备$\mathscr{T}$，我们将认同F与$F'_{\mathscr{T}}$的对偶。因此，对于前面型的所有拓扑 $\mathscr{T}$，$F'$ 的算术都是相同的，如果 $\mu$ 是这样的算术，那么它的傅里叶变换就是 F 上的函数。

我们将 F 上的 Sazonov 拓扑称为由连续半范数 N 满足定义的局部凸拓扑 $\mathscr{S}$，如下条件：$N^2$ 是 F 上的正二次方形式，并且 F 上存在连续正二次方形式 H，使得$\operatorname{Tr}(N^2/H) < +\infty$。 拓扑 $\mathscr{S}$ 比 F 上给定的拓扑更粗糙；如果这些拓扑相同，则 F 被称为核。这个空间的类稍后会详细研究。

#### 定理 2（米洛斯）{#int-ix-s6-thm-2 .statement tag=09ST}

— *设 F 为空间的局部凸空间，$\mathscr{T}$ $F'$ 上的局部凸拓扑，介于 $\mathscr{T}_s$ 和 $\mathscr{T}_c$ 之间，以及 $\mu$ $F'_{\mathscr{T}}$ 上的近似值。假设对于 Sazonov 拓扑，$\mu$ 的傅里叶变换 $\Phi$ 在 F 上连续。那么 $\mu$ 是 $F'_{\mathscr{T}}$ 的度量。*

让$\varepsilon > 0$。由于 $\Phi$ 对于 F 上的 Sazonov 拓扑是连续的，因此在 F 上存在两个连续正二次形式 Q 和 H，使得 $\operatorname{Tr}(Q/H) < +\infty$ 和

$$
\Phi(0) - \mathscr{R}\Phi(x) \leq \varepsilon/6
$$

对于每个$x \in F$，使得$Q(x) \leq 1$。根据 No. 8、$|\mathscr{R}\Phi(x)| \leq \Phi(0)$ 的第 8 号提案，适用于所有 $x \in F$、从而

$$
\Phi(0) - \mathscr{R}\Phi(x) \leq \varepsilon/6 + 2\Phi(0)Q(x)
$$

对于所有$x \in F$。

集合 $r = (12\Phi(0)\operatorname{Tr}(Q/H)\varepsilon^{-1})^{1/2}$ 并用 $x' \in F'_\mathscr{T}$ 的 K 集合表示，使得 $\langle x, x' \rangle^2 \leq r^2 H(x)$ 对于所有 $x \in F$。由于$H^{1/2}$是$F$上的连续半范数，集合K在$F'_\mathscr{T}$上等连续且闭；因此，它在 Ascoli 的定理中是紧凑的 $F'_\mathscr{T}$（GT，X, §2, No. 5，Th.2 的 Cor.1）。

设V是$F'_\mathscr{T}$与有限余维的闭线性子空间；则 V 是 F 的有限维线性子空间 T 的正交。 Let $\mu_V$ be the measure on $T'$ that is the image of the promeasure $\mu$ on $F'_\mathscr{T}$ under the mapping $p_V$ that is the transpose of the canonical injection of T into F; its Fourier transform is the restriction of $\Phi$ to T. 最后，根据 Hahn–Banach 定理（TVS，II, §3, No. 2，Th.1 的 Cor.1），$p_V(K)$ 等于 $x' \in T'$ 的集合 $C_r$，使得对于所有 $x \in T$ 都有 $\langle x, x' \rangle^2 \leq r^2 H(x)$。 根据不等式 (63)，可以将No. 9的第10条命题应用到$T'$上的测度$\mu_V$，将$2\Phi(0)Q$的q限制取为T，将h取H。 然后$\operatorname{Tr}(q/h) \leq 2\Phi(0)\operatorname{Tr}Q/H)$，从而

$$
\mu_V(T' - C_r) \leq 3 \left( \frac{\varepsilon}{6} + 2\Phi(0)\operatorname{Tr}(Q/H)\,r^{-2} \right) = \varepsilon.
$$

由于$p_V$定义，通过将$F'_\mathscr{T}/V$的商同构推到$T'$，No. 1的命题1则表明$\mu$是$F'_\mathscr{T}$的测度。

Q.E.D.

#### 推论{#int-ix-s6-n10-cor-1 .statement tag=09SU}

— *令 F 为桶状核空间，$\mathscr{T}$ $F'$ 上的局部凸拓扑，介于 $\mathscr{T}_s$ 和 $\mathscr{T}_c$ 之间，$\mu$ $F'_\mathscr{T}$ 上的算子，以及 $\Phi$ 傅里叶变换 $\mu$。为了使 $\mu$ 成为一个测度，$\Phi$ 在 F 上连续是必要且充分的。*

必要性来自于No. 8的第9条命题，充分性来自于Th。 2.

#### 注 {#int-ix-s6-n10-rem-1 .statement tag=09SV}

— 令 F 为桶状空间和 $\mathscr{T}$ 拓扑上的局部凸拓扑，位于 $F'$ $\mathscr{T}_s$ 和 $\mathscr{T}_c$ 中间。 $\mathscr{T}$ 的 $F'$ 紧凑中的每个子集对于较粗糙的拓扑 $\mathscr{T}_s$ 都是紧凑的。相反，令 K 为 $\mathscr{T}_s$ 的 $F'$ 紧凑型子集。由于F是桶形的，所以K是等连续的（TVS，III, §4, No. 2，Th.1）；但根据阿斯科利的定理，$F'$的每个等连续子集对于$\mathscr{T}_c$都是相对紧的，对于$\mathscr{T}$来说*更不必说*是相对紧的，因此K包含在对于$\mathscr{T}$来说紧的$F'$的子集中。由此不难推断，$F'_\mathscr{T}$的恒等映射落在这两个空间的措施集合之间的$F'_{\mathscr{T}_s}$定义双射之间。

### 11.希尔伯特空间的措施

令 E 为实希尔伯特空间，其中标量乘积表示为 $(x|y)$。 E 的对偶 $E'$ 上存在同构 j，其特征在于 E 中的 $x, y$ 具有公式 $\langle x, j(y) \rangle = (x|y)$（TVS、V, §1, No. 7、Th. 3）。我们将通过 j 计算认同 E 和 $E'$。因此，E 上的promeasure $\mu$ 的傅里叶变换是E 上的函数 $\mathscr{F}\mu$；当 $\mu$ 是一个测度时，我们有

$$(64)$$
$$(\mathscr{F}\mu)(x) = \int_{E} e^{i(x|y)} d\mu(y) \quad (x \in E).$$

#### 定理 3（普罗霍罗夫-萨佐诺夫）{#int-ix-s6-thm-3 .statement tag=09SW}

*设 E 为希尔伯特空间，Es 空间 E 配备弱化拓扑。设 μ 为 E 的配度，Φ 为傅里叶变换。以下条件是等效的*：

a) 对于 Sazonov 拓扑*，*函数 Φ 在 E 上连续。

b) *对于每个 ε > 0，E 上存在一个核正二次方程形式 Q，使得 Φ(0) − $\Re \Phi$ ≤ ε + Q*。

c) *promeasure μ 是对 Es* 的测量。

$b) \Rightarrow a)$：这是从No. 8 (cf. 不等式 (54)) 的第 8 条命题得出的。

$a) \Rightarrow c)$：这是从 No. 10 的定理 2 开始的。

$c) \Rightarrow b)$：假设 μ 是 Es 上的度量。令 ε > 0。对于 $x \in E$ 的每个整数 $n \geq 1$、集合 $B_n$ 以及范数 $\leq n$，是 $E_s$ 和 $E = \bigcup_{n \geq 1} B_n$ 的闭子集。因此存在整数$n \geq 1$使得$\mu(E - B_n) < \frac{\varepsilon}{2}$。 公式

$$(65)$$
$$ Q(x) = \frac{1}{2} \int_{B_n} (x|y)^2 d\mu(y) $$

定义 E 上的正二次形式 Q。集合 $C = \frac{n^2}{2} \mu(B_n)$。如果 $(e_1, \ldots, e_p)$ 是 E 中的有限正交序列，则

$$
\sum_{j=1}^p (e_j|y)^2 \leq \|y\|^2 \leq n^2
$$

贝塞尔的不等式每$y \in B_n$。通过积分可以得出

$$
\sum_{j=1}^p Q(e_j) = \frac{1}{2} \int_{B_n} \sum_{j=1}^p (e_j|y)^2 d\mu(y) \leq \frac{n^2}{2} \mu(B_n) = C,
$$

因此Q是核。

此外，每实数t$1 - \cos t \leq \inf \left( 2, \frac{t^2}{2} \right)$，从而

$$
\Phi(0) - \Re \Phi(x) = \int_{E} (1 - \cos(x|y)) d\mu(y)
$$
$$
\leq \int_{B_n} \frac{1}{2}(x|y)^2 d\mu(y) + \int_{E - B_n} 2 \cdot d\mu(y)
$$
$$
< Q(x) + \varepsilon
$$

对于所有$x \in E$。从而b)得到验证。

Q.E.D.

#### 推论 1 {#int-ix-s6-thm-2-cor-1 .statement tag=09SX}

— *令$E_1$和$E_2$为两个希尔伯特空间，$u$为$E_1$的希尔伯特-施密特映射到$E_2$，以及$\mu$为$E_1$的折算。假设$\mu$的傅里叶变换$\Phi$在$E_1$上连续。那么promeasure $\nu = u(\mu)$就是在$E_2$上配备弱拓扑的措施。*

通过本文介绍的$E_1$和$E_2$及其对偶的辨识，$\nu$的傅里叶变换等于$\Phi \circ u^*$，其中$u^*$是$u$的伴随。现在，$u^*$是$E_2$到$E_1$的希尔伯特-施密特映射（附件，No. 2），因此$E_2$上的二次形式$y \mapsto \|u^*(y)\|^2$是核的。如果$(E_2)_\mathscr{S}$表示$E_2$配备了Sazonov 拓扑，则$u^*$是$(E_2)_\mathscr{S}$到$E_1$的连续线性映射，$\mathscr{F}_V = \Phi \circ u^*$是$(E_2)_\mathscr{S}$上的连续； 定理 3 则表明$\nu$是在空间$E_2$上配备弱拓扑的测度。

#### 推论 2 {#int-ix-s6-thm-2-cor-2 .statement tag=09SY}

— *令$Q$为希尔伯特空间$E$上的核正二次形式。 $E$ 上的高斯原测度 $\Gamma_Q$ 以及方差 $Q$ 是 $E_s$ 上的测度。*

$\Gamma_Q$的傅里叶变换$\Phi$等于$e^{-Q/2}$。现在，每实数 $t$、从而 $\Phi(0) - \Re \Phi \leq Q/2$ $e^t \geq 1 + t$。因而，定理 3 的条件 b) 得到验证，$\Gamma_Q$ 是$E_s$ 的测度。

#### 注 {#int-ix-s6-n11-rem-1 .statement tag=09SZ}

— 1) 令$E$为希尔伯特空间，$E_s$空间$E$配备弱拓扑，并将$E$的$j$恒等映射配备$E_s$。人们知道，$E$的集合的$j$定义双射到$E_s$的相应的集合。此外，如果$E$是可分的，则它是$E$上有界测度的集合的波兰语空间和$j$定义双射到$E_s$上有界测度的集合（§ 3, No. 3， *注*);可以证明（菲利普斯的定理）如果$E$不可分，则定理仍然成立。因而，定理 3 为$E$ 上的赞成措施提供了判据作为一项措施。

2）可以证明（附件，Exer.7）希尔伯特空间$E$上的萨佐诺夫拓扑由型$Q^{1/2}$的半范数定义，其中$Q$是一个*核*正二次形式 $E$。

*12. 关系且函数为正型*

#### 定义 3 {#int-ix-s6-def-3 .statement tag=09T0}

— *令 $G$ 为群。如果不等式*，则 $G$ 上的复值函数 $\Phi$ 被称为正型

$$
\sum_{j,k=1}^p c_j \overline{c_k} \Phi(x_j x_k^{-1}) \geq 0
$$

*适用于任何* $x_1, \ldots, x_p$ *在* $G$ *和任何复数* $c_1, \ldots, c_p$。

稍后将详细研究这个概念。

#### 命题 11 {#int-ix-s6-prop-11 .statement tag=09T1}

— 令 E 为有限维向量空间，$\mu$ E 的有界（正）测度，$\Phi$ 傅里叶变换为 $\mu$。 函数 $\Phi$ 是连续的，且型在 $E'$ 上。

$\Phi$的连续性源自No. 8的第9条命题。

让我们证明$\Phi$是正型。令$x'_1, \ldots, x'_p$位于$E'$和$c_1, \ldots, c_p$复数中。然后

$$
\sum_{j,k} c_j \overline{c_k} \Phi(x'_j - x'_k) = \int_E \sum_{j,k} c_j \overline{c_k} e^{i \langle x, x'_j - x'_k \rangle} \, d\mu(x)
$$
$$
= \int_E \left| \sum_{j=1}^p c_j e^{i \langle x, x'_j \rangle} \right|^2 \, d\mu(x) \geq 0.
$$

Q.E.D.

一个可以证明逆命题被称为 *Bochner 的定理*：正型的 $E'$ 上的每个连续函数是有界（正）测度的傅里叶变换。 (*) 我们将在 No. 12 的其余部分假设这个结果。

#### 定理 4 {#int-ix-s6-thm-4 .statement tag=09T2}

— 令 E 为局部凸空间。傅立叶变换是 E 上的算子的集合的双射到$E'$ 上的正型的函数的集合，其中限制对于每个有限维子空间都是连续的。

我们知道（No. 3，命题 3）傅里叶变换是单射的。令 $\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ 为 E 的配度，$\Phi$ 为傅里叶变换。令 T 为 $E'$ 的有限维子空间，并令 V 为 T 在 E 中的正交。一个可以确定 T 与 $E/V$ 的对偶； $\Phi$到T的限制$\Phi_T$是$E/V$上有界测度$\mu_V$的傅里叶变换。根据命题 11，$\Phi_T$ 是连续的，且在 T 上为正型。由于 T 是任意的，所以显然$\Phi$ 在$E'$ 上为正型。

相反，令$\Phi$为$E'$上的正型的函数，其限制对于$E'$的每个有限维子空间都是连续的。对于每个$V \in \mathscr{F}(E)$，我们将$E/V$的对偶认同与$E'$中V的正交$V^\circ$； $\Phi$到$V^\circ$的限制$\Phi_V$是连续的并且为正型，因而，根据Bochner的定理，$E/V$上存在有界（正）测度$\mu_V$，其傅里叶变换为$\Phi_V$。令$\mathscr{F}(E)$中的V和W使得$W \subset V$，并令$p_{VW}$为$E/W$的典范映射到$E/V$；经过识别，${}^t p_{VW}$是$V^\circ$到$W^\circ$的单射。到No. 3的公式(4)，我们有

$$
\mathscr{F}(p_{VW}(\mu_W)) = (\mathscr{F}\mu_W) \circ {}^t p_{VW} = \Phi_W \circ {}^t p_{VW} = \Phi_V = \mathscr{F}\mu_V,
$$

(*) 这个问题将在即将出版的《光谱理论》一书中的章中进行研究。关于这个问题读者可以查阅L.H的书。 LOOMIS，*抽象谐波数学分析*，范诺斯特兰德，纽约，1953 年。

从而 $pvw(\mu_w) = \mu_v$ 根据 No. 3 的第 3 号提案。因而，族$\mu = (\mu_v)_{v \in \mathscr{F}(E)}$是$E$的订婚；显然$\Phi$是$\mu$的傅里叶变换。

#### 推论 {#int-ix-s6-n11-cor-1 .statement tag=09T3}

— *令 F 为桶装核空间；为 F' 配备一个局部凸拓扑 $\mathscr{T}$，中间为弱拓扑 $\sigma(F', F)$ 和拓扑，在 F 的紧凸子集上均匀收敛。傅里叶变换是 F' 上有界（正）测度的集合的双射 F 上连续函数的集合正型。*

这紧随定理 4 和 Cor.的 Th。 2 个No. 10。*

### 习题{#int-ix-s6-exercises}

§ 6](exercises/s6/)参见[习题。
