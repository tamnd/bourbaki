---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 6
section_title: Integration on compact Lie groups
lang: zh
source: lie-vii-ix
book_pages: 333-346, 409-414
pdf_pages: 0340-0353, 0416-0421
extraction: native
subsections:
    - "no": 1
      title: PRODUCT OF ALTERNATING MULTILINEAR FORMS
      page: 333
      pdf_page: 340
    - "no": 2
      title: INTEGRATION FORMULA OF H. WEYL
      page: 334
      pdf_page: 341
    - "no": 3
      title: INTEGRATION ON LIE ALGEBRAS
      page: 339
      pdf_page: 346
    - "no": 4
      title: INTEGRATION OF SECTIONS OF A VECTOR BUNDLE
      page: 341
      pdf_page: 348
    - "no": 5
      title: INVARIANT DIFFERENTIAL FORMS
      page: 344
      pdf_page: 351
statements: 25
exercises: 13
content_sha256: f244aa3ca5cea5d1255e3a868808bd30dbf887a09b6c49d5a36ebb4b2a83ea51
translated_from: content/en/lie/IX/06_s6_integration_on_compact_lie_groups.md
translation_method: google
source_content_sha256: 746c6186434593ae87ea52347a193f0e294cca0a933dcfbfbd4549276c4b772c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 9dabd1fb71674dfc0601873d6f7a1a2f1cf2a5d0b30e9253532a12db00e7a224
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 6。集成紧李群

我们保留§4中的记号；放入$w(G) =$卡(W$_G(T)$)。用 $dg$（分别为 $dt$）表示总质量为 1 的 G（分别为 T）的 Haar 测度，并用 $n$（分别为 $r$）和 G（分别为 T）的维数表示。

### 1. 乘积交替多重线性形式

设A为交换环，M为A-模。对于每个整数$r\geq 0$，用M上的交错的$r$的Alt$^r(M)$A-模-线性形式表示；它可以用A-模$\wedge \wedge^r(M) ($代数的对偶来识别，第1章。 III, §7, no. 4，提案 7）。设 $u\in$ Alt$^s(M)$ 和 $v\in$ Alt$^r(M)$；回想一下（代数，第III, §11, no. 2，例 3），$u$和$v$的交错的乘积是元素$u\wedge v\in$Alt$^{s+r}(M)$，定义为

$$
(u\wedge v)(x_1, . . . , x_{s+r}) =\sum_{\sigma\in\mathfrak{S}_{s,r}}\varepsilon_{\sigma}u(x_{\sigma(1)}, . . . , x_{\sigma(s)})v(x_{\sigma(s+1)}, . . . , x_{\sigma(s+r)})
$$

其中$\mathfrak{S}_{s,r}$是置换的对称群$\mathfrak{S}_{s+r}$由……组成的子集，其中限制到$1, s$和$s+ 1, s+r$是递增。

现在让

0 $\longrightarrow M'\longrightarrow^i$ 中号 $\longrightarrow^pM''\longrightarrow$ 0

分别为正合序列、自由A-模、秩、$r, r+s$ 和$s$。

#### 引理 1 {#lie-ix-s6-lem-1 .statement tag=01EX}

从 Alt$^s(M'')\times$ Alt$^r(M')$ 到 Alt$^{s+r}(M)$ 存在一个 A 双线性映射，用 $(u, v) \rightarrow u\cap v$ 表示，其特征为以下两个性质之一：

a) 用$u_1\in$ Alt$^s(M)$ 形式 $(x_1, . . . , x_s) \rightarrow u(p(x_1), . . . , p(x_s))$ 表示，并令$v_1\in$ Alt$^r(M)$ 为形式，使得$M'$中的$x'_1, . . . , x'_r$为$v_1(i(x'_1), . . . , i(x'_r)) =v(x'_1, . . . , x'_r)$；然后$u\cap v=u_1\wedge v_1$。

b) 对于 M 中的所有 $x_1, . . . , x_s$ 和 $M'$ 中的 $x'_1, . . . , x'_r$，

$$
(u\cap v)(x_1, . . . , x_s, i(x'_1), . . . , i(x'_r)) =u(p(x_1), . . . , p(x_s))v(x'_1, . . . , x'_r) \tag{1}
$$

映射$\varphi :$Alt$^s(M'')\otimes_A$Alt$^r(M')\rightarrow$Alt$^{s+r}(M)$使得$\varphi (u\otimes v) =u\cap v$是秩自由A-模同构一。

形式 $v_1$ 满足条件 a) 的存在源于$\wedge \wedge^r(i)$ 诱导同构从$\wedge \wedge^r(M) ($代数的$\wedge \wedge^r(M')$到直因子子模，第1章。 III, §7, no. 2）。令$v_1$为形式；把$u\cap v=u_1\wedge v_1$。然后满足公式 (1)，因为如果我们将$i(x'_k) =x_{s+k}$代替$1\leq k\leq r$，则$\mathfrak{S}_{s,r}$中唯一的元素$\sigma$使得$1\leq i\leq s$的$p(x_{\sigma(i)})\not= 0$是恒等式置换。另一方面，公式 (1) 确定 $u\cap v$ 是唯一的：确实，令 $(e'_1, . . . , e'_r)$ 为 $M''$ 的 $M', (f''_1, . . . , f''_s)$ 基的基，以及 M 的 $f_1, . . . , f_s$ 元素，使得$p(f_i) =f''_i$ 换$1\leq i\leq s$。那么$(f_1, . . . , f_s, i(e'_1), . . . , i(e'_r))$是M的基（代数，第II, §1, no. 11章，第21条命题），并且公式（1）可以写成

$$
(u\cap v)(f_1, . . . , f_s, i(e'_1), . . . , i(e'_r)) =u(f''_1, . . . , f''_s)v(e'_1, . . . , e'_r) \tag{2}
$$

但 Alt$^{s+r}(M)$ 的元素由其基上的值决定。

由上可知，条件 a) 和 b) 确定乘积 $u\cap v$ 都是唯一的；很明显，这个乘积是双线性的。最后，引理的最后一个断言由公式(2)得出。

### 2. 积分公式 H. 韦尔

令$e$为G的单位元素，$\overline{e}$为$G/T$中的类。 认同 G 在 $e$ 与 $\mathfrak{g}$ 的切线空间，T 在 $e$ 与 $\mathfrak{t}$ 的切线空间，以及 $G/T$ 在 $\overline{e}$ 与 $\mathfrak{g}/\mathfrak{t}$ 的切线空间。用 $(u, v) \rightarrow u\cap v$ 表示 $\mathbf{R}$-双线性映射

Alt$^{n-r}(\mathfrak{g}/\mathfrak{t})\times$ Alt$^r(\mathfrak{t})\rightarrow$ Alt$^n(\mathfrak{g})$

定义于数 1。

回忆一下（第 III, §3, no. 13 章，第 50 条命题），映射 $\omega  \rightarrow \omega (e)$ 是同构，来自 G（或 T）上次数 $n$（或 $r$）的左不变微分形式的向量空间到空间 Alt$^n(\mathfrak{g})$（或 Alt$^r(\mathfrak{t})$）。此外，观察到，由于$\mathbf{R}^*$约化到单位元素的每个连通紧凑子群，对所有$g\in G$都det Ad$g= 1$，因此G上次数$n$的左不变微分形式也是右不变的，并且内自同构下的不变量（第 III, §3, no. 16 章，Prop. 54 的 Cor.）：从现在开始，我们将简单地讨论 G 不变微分形式。

同样，它是从第 1 章得出的。 III, §3, no. 16、第 56 条命题以及前述内容，映射 $\omega  \rightarrow \omega (\overline{e})$ 是从空间空间次数 $n-r$ 的 G 不变微分形式在 $G/T$ 到空间 Alt$^{n-r}(\mathfrak{g}/\mathfrak{t})$ 的同构。

如果$\omega_{G/T}$是$G/T$上次数$n-r$的G不变微分形式，并且$\omega_T$是T上次数$r$的不变微分形式，则用$\omega_{G/T}\cap \omega_T$表示唯一不变微分G 上次数 $n$ 的形式使得

$$
(\omega_{G/T}\cap \omega_T)(e) =\omega_{G/T}(\overline{e})\cap \omega_T(e)
$$

最后回想一下，$f: (G/T)\times T\rightarrow G$表示由映射$(g, t) \rightarrow gtg^{-1}$通过商（§5, no. 4）从$G\times T$到G引起的流形的态射。如果$\alpha$和$\beta$分别在$G/T$和T上微分形式，则简单地用$\alpha \wedge \beta$形式pr$^*_1\alpha \wedge$pr$^*_2\beta$在$(G/T)\times T$上表示。

对于 $t\in T$，用 Ad$_{\mathfrak{g}/\mathfrak{t}}(t)$ 自同态表示由 Ad $t$ 通过通向商而引发的 $\mathfrak{g}/\mathfrak{t}$。放

$\delta_G(t) =$ det（广告$_{\mathfrak{g}/\mathfrak{t}}(t)-1$）$=\prod_{\alpha\in R(G,T)}(t^{\alpha}-1)$。 (3)

设$x\in \mathfrak{t}$和$\alpha \in R(G,T)$；用 $\mathfrak{t}^*$ 的 $\widehat{\alpha}$ 元素 $(2\pi i)^{-1}\delta (\alpha )$ 表示，因此

((exp $x$)$^{\alpha}-$ 1)((exp $x$)$^{-\alpha}-1$) $= (e^{2\pi i\widehat{\alpha}(x)}-1)(e^{-2\pi i\widehat{\alpha}(x)}-1) = 4$ sin$^2\pi \widehat{\alpha}(x)$。

如果$R_+(G,T)$表示$R(G,T)$相对于基B的正根的集合，我们有

$\delta_G$(exp $x$)$=\prod_{\alpha\in R_+(G,T)}4$罪$^2\pi \widehat{\alpha}(x)$,

因此，特别是 $\delta_G(t)>0$ 对于所有 $t\in T_r$。我们注也将$\delta_G(t) =\delta_G(t^{-1})$换成$t\in T$。

#### 命题 1 {#lie-ix-s6-prop-1 .statement tag=01EY}

令$\omega_G, \omega_{G/T}$和$\omega_T$分别为次数、$n, n-r$和$r$在$G,G/T$和T上的不变微分形式。如果 $\omega_G=$ $\omega_{G/T}\cap \omega_T$，那么

$$
f^*(\omega_G) =\omega_{G/T}\wedge \delta_G\omega_T
$$

显然我们可以假设$\omega_{G/T}$和$\omega_T$非零；那么 $(G/T)\times T$ 上的微分形式 $(u, t) \rightarrow \omega_{G/T}(u)\wedge \omega_T(t)$ 为次数 $n$ 并且处处非零；因此 $(G/T)\times T$ 上存在一个数值函数 $\delta$ 使得

$$
f^*(\omega_G)(u, t) =\delta (u, t)\omega_{G/T}(u)\wedge \omega_T(t)
$$

现在观察，对于 $h\in G,u\in G/T,t\in$ T，我们有 $f(h.u, t) =$ (Int $h$)$f(u, t)$；由于$\omega_G$在内自同构下是不变的，因此紧随$\delta (h.u, t) =\delta (u, t)$，所以$\delta (u, t) =\delta (\overline{e}, t)$。

用 $p:\mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{t}$ 表示商映射并用 $\varphi :\mathfrak{g}/\mathfrak{t}\rightarrow \mathfrak{g}$ 映射定义

$\varphi (p(X)) =$（广告$t^{-1}$）$X-X$为$X\in \mathfrak{g}$；回想一下 (§5, no. 4, 引理 4) 切线映射

$$
T_{(e,t)}(f) : T_e(G/T)\times T_t(T)\rightarrow T_t(G)
$$

需要 $(z, tH)$ 到 $t(\varphi (z) +H)$ 才能获得 $z\in \mathfrak{g}/\mathfrak{t}, H\in \mathfrak{t}$。

令 $z_1, . . . , z_{n-r}$ 为 $\mathfrak{g}/\mathfrak{t},H_1, . . . , H_r$ 元素 $\mathfrak{t}$ 中的元素。然后

$$
f^*\omega_G(\overline{e}, t)(z_1, . . . , z_{n-r}, tH_1, . . . , tH_r)
$$

$=\omega_G(t)(t\varphi (z_1), . . . , t\varphi (z_{n-r}), tH_1, . . . , tH_r)$ 由$T_{(\overline{e},t)}(f)$计算

$=\omega_G(e)(\varphi (z_1), . . . , \varphi (z_{n-r}), H_1, . . . , H_r)$ 因为 $\omega_G$ 是不变的

$=\omega_{G/T}(\overline{e})(p\varphi (z_1), . . . , p\varphi (z_{n-r})).\omega_T(e)(H_1, . . . , H_r)$（无$.1$、引理 1）

= det($p\varphi$)$\omega_{G/T}(\overline{e})(z_1, . . . , z_{n-r}).\omega_T(e)(H_1, . . . , H_r)$

$$
=\delta_G(t)\omega_{G/T}(\overline{e})(z_1, . . . , z_{n-r}).\omega_T(t)(tH_1, . . . , tH_r)
$$

因为 $\omega_T$ 是不变的

$$
=\delta_G(t)(\omega_{G/T}\wedge \omega_T)(\overline{e}, t)(z_1, . . . , z_{n-r}, tH_1, . . . , tH_r)
$$

所以$f^*\omega_G(\overline{e}, t) =\delta_G(t)(\omega_{G/T}\wedge \omega_T)(\overline{e}, t)$；因此，$\delta (\overline{e}, t) =\delta_G(t)$，因此命题。

分别给出流形 $G,T$ 和 $G/T$ 形式 $\omega_G, \omega_T$ 和 $\omega_{G/T}$ 定义的方向。这些形式定义对$G,T$和$G/T$（第III, §3, no. 16章，第55条和第56条提案）的不变测度，也用$\omega_G, \omega_T$和$\omega_{G/T}$表示。

#### 引理 2 {#lie-ix-s6-lem-2 .statement tag=01EZ}

如果$\omega_G=\omega_{G/T}\cap \omega_T$，那么

$$
\int_G\omega_G=\int_{G/T}\omega_{G/T}.\int_T\omega_T
$$

用 $\pi$ 表示从 G 到 $G/T$ 的规范态射。设$g\in G$，并令$t_1, . . . , t_{n-r}$为$T_{\pi(g)}(G/T)$的元素。 认同纤维$\pi^{-1}(\pi (g)) =gT$，翻译为$\gamma (g)$。 关系 $\omega_G=\omega_{G/T}\cap \omega_T$ 现在意味着等式（可微分和解析流形，结果，11.4.5）：

$$
\omega_G\llcorner (t_1, . . . , t_{n-r}) = (\omega_{G/T}(t_1, . . . , t_{n-r}))\omega_T
$$

因此$\int_{\pi}\omega_G=(\int_T\omega_T)\omega_{G/T}($可微分和解析流形，结果，11.4.6），以及

$$
\int_G\omega_G=\int_{G/}\int_{T\pi}\omega_G=\int_T\omega_T.\int_{G/T}\omega_{G/T}
$$

（可微分和解析流形，结果，11.4.8）。

#### 引理 3 {#lie-ix-s6-lem-3 .statement tag=01F0}

逆像在$(G/T)\times T_r$上的测量$dg$在$G_r$下的局部同胚$f_r($积分，第1章。 V, §6, no. 6）是$\mu\otimes \delta_Gdt$的测度，其中$\mu$是总质量1的$G/T$上唯一的G不变测度。

Choose an invariant differential form $\omega_T$ (resp. $\omega_{G/T}$) on T (resp. $G/T$) of maximal degree, such that the measure defined by $\omega_T$ (resp. $\omega_{G/T}$) is equal to $dt$ (resp. $\mu$). 输入$\omega_G=\omega_{G/T}\cap \omega_T$。 引理 2 意味着$\omega_G$ 定义的度量等于$dg$。 设U是$(G/T)\times T_r$的开子集，使得$f_r$诱导同构从U到$G_r$的开子集V。 设$\varphi$为连续函数，且V有紧支撑；也用 $\varphi$ 到 $G_r$ 的 $\varphi$ 扩张表示，它消失在 V 之外。 我们有

$$
\int_V\varphi  dg=\int_V\varphi  \omega_G=\int_U(\varphi \circ f_r)f_r^*(\omega_G)
$$

$=\int_U(\varphi \circ f_r)\omega_{G/T}\wedge \delta_G\omega_T$（道具$.1$）

$$
=\int_U(\varphi \circ f_r)d\mu.\delta_Gdt
$$

因此引理。

#### 定理 1（H.韦尔）{#lie-ix-s6-thm-1 .statement tag=01F1}

G 上的测度 $dg$ 是测度 $dg\otimes \frac{1}{w(G)}\delta_Gdt$ 的 $G\times T$ 到 G 的映射 $(g, t) \rightarrow gtg^{-1}$ 下的像，其中

$\delta_G(t) =$ det（广告$_{\mathfrak{g}/\mathfrak{t}}(t)-1$）$=\prod_{\alpha\in R(G,T)}(t^{\alpha}-1)$。

等效地（积分，第 V, §6, no. 3 章，命题 $4$）$,dg$ 是$\mu\otimes \frac{1}{w(G)}\delta_Gdt$ 的映射 $f: (G/T)\times T\rightarrow G$ 下的像。

我们证明最后一个断言。从§5, no. 1和可微分析流形、结果$, 10.1.3c)$可以得出，G**--** $G_r$在G中可以忽略不计，而T **--** $T_r$在T中可以忽略不计。此外，映射$f_r$使$(G/T)\times T_r$成为$G_r$，与群 W（§5, no. 4，提案$4b$）$)$。 定理现在接续于引理 3 和集成，第 1 章。 V, §6, no. 6，提案 11。

#### 推论 1 {#lie-ix-s6-thm-1-cor-1 .statement tag=01F2}

(i) 设$\varphi$为G上的可积函数，且值位于Banach空间或$\overline{\mathbf{R}}$中。对于几乎所有 $t\in T$，G 上的函数 $g \rightarrow \varphi (gtg^{-1})$ 对于 $dg$ 都是可积的。 函数 $t \rightarrow \delta_G(t)\int_G\varphi (gtg^{-1})dg$ 在 T 上可积，我们有

$$
\int_G\varphi (g)dg=\frac{1}{w(G)}\int_T(\int_G\varphi (gtg^{-1})dg)\delta_G(t)dt \tag{4}
$$

（“赫尔曼·韦尔的积分公式”）。

(ii) 令$\varphi$为G上的正可测函数。对于几乎所有$t\in T$，G上的函数$g \rightarrow \varphi (gtg^{-1})$都是可测的。 T 上的函数 $t \rightarrow \int_G^*\varphi (gtg^{-1})dg$ 是可测的，我们有

$$
\int_G^*\varphi (g)dg=\frac{1}{w(G)}\int_T^*(\int_G^*\varphi (gtg^{-1})dg)\delta_G(t)dt \tag{5}
$$

由于映射 $f$ 是通过从 $G\times T\rightarrow G$ 到映射 $(g, t) \rightarrow gtg^{-1}$ 的商而导出的，因此只需应用第 1 章的积分即可。 V, §5、6、8 和积分，第 1 章VII, §2。

#### 推论 2 {#lie-ix-s6-thm-1-cor-2 .statement tag=01F3}

令$\varphi$为G上的中心函数（即，对于G中的所有$g$和$h$，$\varphi (gh) =$$\varphi (hg)$），值位于Banach空间或$\overline{\mathbf{R}}$中。

a$)\varphi$ 是可测的，当且仅当其限制到 T 是可测的。

b$)\varphi$ 是可积的当且仅当函数 $(\varphi |T)\delta_G$ 在 T 上可积，在这种情况下我们有

$$
\int_G\varphi (g)dg=\frac{1}{w(G)}\int_T\varphi (t)\delta_G(t)dt \tag{6}
$$

用 $p: G/T\times T\rightarrow T$ 表示第二个投影。我们有 $\varphi \circ f$ = $(\varphi |T)\circ p$；此外，$\mu\otimes \frac{1}{w(G)}\delta_Gdt$措施的$p$下的像为$\frac{1}{w(G)}\delta_Gdt$。现在可以从 Th 得出推论。上述 1 和 Th.集成，第 1 章。 V, §6, no. 2，应用于两个真映射$f$和$p$。

#### 推论 3 {#lie-ix-s6-thm-1-cor-3 .statement tag=01F4}

设 H 为 G 包含 T 的连通闭子群，$\mathfrak{h}$ 李代数，以及$dh$ 总质量 1 的 H 上的 Haar 测度。设 $\varphi$ 为 G 上的可积中心函数，其中值在 Banach 中空间或$\overline{\mathbf{R}}$。那么函数 $h \rightarrow \varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1$) 可积且以 H 为中心，我们有

$\int_G\varphi (g)dg=\frac{w(H)}{w(G)}\int_H\varphi (h$）det（广告$_{\mathfrak{g}/\mathfrak{h}}(h)-1$）$dh$。 (7)

事实上，函数$h \rightarrow \varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1$)是H上的中心函数，其限制到T是函数$t \rightarrow \varphi (t)\delta_G(t)\delta_H(t)^{-1}$。因此，推论由 Cor 得出。 2适用于G和H。

#### 注 1 {#lie-ix-s6-n2-rem-1 .statement tag=01F5}

如果我们在 Cor 中取$\varphi = 1$。 3、我们得到

$\int_H$ det(广告$_{\mathfrak{g}/\mathfrak{h}}(h)-1$)$dh=w(G)/w(H)$ (8)

特别是

$$
\int_T\delta_G(t)dt=w(G) \tag{9}
$$

#### 注 2 {#lie-ix-s6-n2-rem-2 .statement tag=01F6}

令 $\nu$ 为商 $T/W$ 的度量，定义为

$$
\int_{T/W}\psi (\tau )d\nu (\tau ) =\frac{1}{w(G)}\int_T\psi (\pi (t))\delta_G(t)dt
$$

其中 $\pi$ 表示 T 在 $T/W$ 上的规范投影。科。 2 表示同态 $T/W\rightarrow G/$Int(G)（§2, no. 5，第 5 条的 Cor.1）迁移规范投影 $G\rightarrow G/$Int(G) 下测度 $dg$ 的测度 $\nu$ 到像。

#### 注 3 {#lie-ix-s6-n2-rem-3 .statement tag=01F7}

假设 G 是单连通的。令 A 为 $\mathfrak{t}$ 的凹室，$dx$ 对 $\mathfrak{t}$ 的 Haar 测度使得 $\int_Adx= 1$。那么度量$\nu$也可以通过在$\overline{A}$上传输度量$\frac{1}{w(G)}\prod_{\alpha\in R_+(G,T)}4$sin$^2\pi \widehat{\alpha}(x)dx$来获得：

同胚$\overline{A}\rightarrow T/W ($§5, no. 2，Cor.提案 2 中的 1）。

#### 例 {#lie-ix-s6-n2-exa-1 .statement tag=01F8}

取G为群$\mathbf{S}\mathbf{U}(2,\mathbf{C})$，T为矩阵对角线子群（§3, no. 6）； 认同$\mathfrak{t}$与$\mathbf{R}$乘以$\mathfrak{t}($loc的基$\{iH\}$选择。引用。）。把$A = 0, \pi$；这是$\mathfrak{t}$的壁龛。区间$A = 0, \pi$可以用G的共轭类的空间、G的元素$\theta$来识别

$(e^{i\theta}$ 0 $)$

$\overline{A}$相应的至共轭类共$-_{i\theta}$。设 $d\theta$ 为勒贝格

0 $e$

测量$0, \pi$；由上可知，G 上 Haar 测度的 $\overline{A}$ 上的像就是测度 $\frac{2}{\pi}$ sin$^2\theta  d\theta$。

### 3. 整合李代数

#### 命题 2 {#lie-ix-s6-prop-2 .statement tag=01F9}

令 H 为维数 $m,\mathfrak{h}$ 的（实数）李群李代数。令$\omega_H$为H上次数$m$的右不变微分形式，令$\omega_{\mathfrak{h}}$为次数$m$在$\mathfrak{h}$上的平移不变微分形式， 重合，原点为 $\omega_H(e)$。我们有

(经验$_H$)$^*\omega_H=\lambda_{\mathfrak{h}}\omega_{\mathfrak{h}}$ (10)

其中 $\lambda_{\mathfrak{h}}$ 是 $\mathfrak{h}$ 上的 Ad(H) 不变式函数，使得

$\lambda_{\mathfrak{h}}(x) =$ det $\sum(p+$ 1)!1（广告 $x$）$^p$ 为 $x\in \mathfrak{h}$。

$p\geq 0$

设$x, x_1, . . . , x_m$为$\mathfrak{h}$中的元素。我们有

(经验$^*\omega_H$)$_x(x_1, . . . , x_m) = (\omega_H$(经验$x$))$(T_x$(经验)($x_1$)$, . . . ,T_x$(经验)($x_m$))。用 $\varpi (x) :\mathfrak{h}\rightarrow \mathfrak{h}$ 表示 $x$ 处指数的右微分（第 III, §3, no. 17 章，定义 8）； 定义，

$T_x$(exp)($y$)。(exp $x$)$^{-1}=\varpi (x).y$适用于所有$y\in \mathfrak{h}$。

形式 $\omega_H$ 是右不变量，我们得到

$(\omega_H$(经验$x$))$(T_x$(经验)($x_1$)$, . . . ,T_x$(经验)($x_m$))

$=\omega_H(e)(\varpi (x).x_1, . . . , \varpi (x).x_m) =$（检测$\varpi (x)$）$\omega_{\mathfrak{h}}(x_1, . . . , x_m)$；

因此，exp$^*\omega_H=\lambda_{\mathfrak{h}}\omega_{\mathfrak{h}}$，与$\lambda_{\mathfrak{h}}(x) =$ det $\varpi (x) =$ det$\frac{exp ad x-1}{ad x}$（第III, §6, no. 4章，第12条命题）。

设 $h\in H$；由于广告$h$是自同构/$\mathfrak{h}$，我们有

广告（（广告$h$）$(x)$）$=$广告$h\circ$广告$x\circ$（广告$h$）$^{-1}$，

所以$\lambda_{\mathfrak{h}}$((广告$h$)$(x)$)$=\lambda_{\mathfrak{h}}(x)$。因此，函数$\lambda_{\mathfrak{h}}$在Ad(H)下是不变的；这样就完成了命题中的证明。

#### 注 {#lie-ix-s6-n3-rem-1 .statement tag=01FA}

考虑函数$\lambda_{\mathfrak{g}}$与紧李群G相关；鉴于§2, no. 1，Th。 1、对于计算$\lambda_{\mathfrak{g}}$只要知道$\mathfrak{t}$上的值就足够了。但是，对于$x\in \mathfrak{t}$，自同态和$\mathfrak{g}$的$x$是半单，并且有特征值0（与重数$r$），并且对于所有$\alpha \in R(G,T),\delta (\alpha )(x)$（与重数1）。紧随其后的是

$$
\lambda_{\mathfrak{g}}(x) =\prod\frac{e^{\delta(\alpha)(x)} - 1}{\delta(\alpha)(x)}=\frac{\delta_{\mathfrak{g}}(x)}{\pi_{\mathfrak{g}}(x)} \tag{11}
$$

$\alpha \in R(G,T)$

与 $\delta_{\mathfrak{g}}(x) =\delta_G$(exp $x$) 和 $\pi_{\mathfrak{g}}(x) =\prod_{\alpha\in R(G,T)}\delta (\alpha )(x) =$ det ad$_{\mathfrak{g}/\mathfrak{t}}(x)$。

设$\omega_{G/T}$为$G/T$上次数$n-r$的不变微分形式，$\omega_{\mathfrak{t}}$为$\mathfrak{t}$上次数$r$的平移不变微分形式。对于no. 1的记号，用$\omega_{G/T}\cap \omega_{\mathfrak{t}}$表示$\mathfrak{g}$上次数$n$的唯一平移不变微分形式$\omega_{\mathfrak{g}}$，使得$\omega_{\mathfrak{g}}(0) =\omega_{G/T}(\overline{e})\cap \omega_{\mathfrak{t}}(0)$。

最后，用映射 $(g, x) \rightarrow$ (Ad $g$)$(x)$ 从 $G\times \mathfrak{t}$ 到 $\mathfrak{g}$ 通过商的传递来表示流形的 $\psi : (G/T)\times \mathfrak{t}\rightarrow \mathfrak{g}$ 态射。

#### 命题 3 {#lie-ix-s6-prop-3 .statement tag=01FB}

令$\omega_{\mathfrak{g}},\omega_{\mathfrak{t}},\omega_{G/T}$分别为次数$n, r, n-r$在$\mathfrak{g},\mathfrak{t}$、$G/T$上的不变微分形式。如果$\omega_{\mathfrak{g}}=\omega_{G/T}\cap \omega_{\mathfrak{t}}$，我们有

$$
\psi^*\omega_{\mathfrak{g}}=\omega_{G/T}\wedge \pi_{\mathfrak{g}}\omega_{\mathfrak{t}}
$$

其中 $\pi_{\mathfrak{g}}$ 是由 $\pi_{\mathfrak{g}}(x) =\prod_{\alpha\in R(G,T)}\delta (\alpha )(x)$ 定义的 $\mathfrak{t}$ 上的函数。

用$\omega_G$（或$\omega_T$）表示G（或T）上最大次数的不变微分形式，重合与$\omega_{\mathfrak{g}}$（或$\omega_{\mathfrak{t}}$）在原点。考虑交换律图表

$$
(G/T)\times \mathfrak{t}\longrightarrow^{\psi}\mathfrak{g}
$$

(Id,exp$_T$)exp$_G$。

$(G/T)\times T\longrightarrow^f$G

根据no. 2命题1和关系exp$^*_T\omega_T=\omega_{\mathfrak{t}}$，我们推导出等式

$\psi^*$exp$^*_G\omega_G=\omega_{G/T}\wedge \delta_{\mathfrak{g}}\omega_{\mathfrak{t}}$。

根据提案$2,\psi^*$exp$^*_G\omega_G= (\psi^*\lambda_{\mathfrak{g}})\psi^*\omega_{\mathfrak{g}}$。由于函数$\lambda_{\mathfrak{g}}$在Ad(G)下是不变的，所以对于$\overline{g}\in G/T, x\in \mathfrak{t}$我们有$(\psi^*\lambda_{\mathfrak{g}})(\overline{g}, x) =\lambda_{\mathfrak{g}}(x) =\frac{\delta_{\mathfrak{g}}(x)}{\pi_{\mathfrak{g}}(x)}$。

由此得出形式$\psi^*\omega_G(\overline{g}, x)$和$\omega_{G/T}(\overline{g})\wedge \pi_{\mathfrak{g}}(x)\omega_{\mathfrak{t}}(x)$重合，其中$\delta_{\mathfrak{g}}(x)$非零，即在密集开子集$(G/T)\times \mathfrak{t}_r$上；因此，它们是相等的，因此命题。

Choose invariant differential forms $\omega_G$ on G and $\omega_T$ on T, of maximum degree, such that $|\omega_G|=dg$ and $|\omega_T|=dt$; denote by $\omega_{\mathfrak{g}}$ (resp. $\omega_{\mathfrak{t}}$) the translation-invariant differential form on $\mathfrak{g}$ (resp. $\mathfrak{t}$) that coincides with $\omega_G(e)$ (resp. $\omega_T(e)$) at the origin, and $dz$ (resp. $dx$) the Haar measure $|\omega_{\mathfrak{g}}|$ (resp. $|\omega_{\mathfrak{t}}|$). 推理如no. 2，经必要修正后，给出以下命题：

#### 命题 4 {#lie-ix-s6-prop-4 .statement tag=01FC}

$\mathfrak{g}$ 上的度量$dz$ 是度量$dg\otimes \frac{1}{w(G)}\pi_{\mathfrak{g}}dx$ 的适当映射 $(g, x) \rightarrow$（Ad $g$）$(x)$ 下的像，从$G\times \mathfrak{t}$ 到$\mathfrak{g}$。

我们将Cor的类似物留给读者叙述和证明。 no. 2的1至3和注1至3。对于例，令$\varphi$为$\mathfrak{g}$上的可积函数（值位于Banach空间或$\overline{\mathbf{R}}$）；然后

$\int_{\mathfrak{g}}\varphi (z)dz=\frac{1}{w(G)}\int_{\mathfrak{t}}(\int_G\varphi$((广告$g$)$x$)$dg)\pi_{\mathfrak{g}}(x)dx$, (12)

并且，特别是，如果 $\varphi$ 在 Ad(G) 下是不变的，

$$
\int_{\mathfrak{g}}\varphi (z)dz=\frac{1}{w(G)}\int_{\mathfrak{t}}\varphi (x)\pi_{\mathfrak{g}}(x)dx \tag{13}
$$

### 4. 截面向量丛的积分

In this number and the next, we denote by X a real manifold of class $C^r$ $(1\leq r\leq  \infty )$, locally of finite dimension.

令 Y 为类 $C^r$ 中的流形。如果$r <\infty$，请考虑映射$f \rightarrow$$j^r(f)$从$\mathscr{C}^r(X; Y)$到$\mathscr{C}(X; J^r(X,Y)) ($可微分和解析流形，结果，12.3.7）。 $\mathscr{C}(X; J^r(X,Y))$上紧致收敛的拓扑的映射下的逆像称为$C^r$紧致收敛的拓扑-$\mathscr{C}^r(X; Y)$上收敛；它是 K 上均匀 $C^r$ 收敛拓扑的上界（可微分和解析流形，结果，12.3.10），其中 K 穿过 X 的紧凑子集的集合。

当$r$ = $\infty$时，我们称紧致$C^{\infty}$收敛于紧致$C^k$收敛拓扑的$\mathscr{C}^{\infty}(X; Y)$上界上的拓扑，在其他字中称为最粗拓扑，其中典范嵌入 $\mathscr{C}^{\infty}(X; Y)\rightarrow \mathscr{C}^k(X; Y)$对于$0\leq k <\infty$是连续的。

令E为实数向量丛和基X、类$C^r$，并令$\mathscr{S}^r(X; E)$为类$C^r$E的截面向量空间。在这个数中，我们给出由$C^r$收敛的拓扑在$\mathscr{C}^r(X; E)$上诱导的$\mathscr{S}^r(X; E)$拓扑，也称为紧凑$C^r$收敛的拓扑；它将$\mathscr{S}^r(X; E)$变成完全分离的局部凸拓扑向量空间（cf.可微分和解析流形，结果，15.3.1和谱理论，正在准备中）。

现在令H为李群，类$C^r$左运算的$m: H\times X\rightarrow X$律；将 $hx=m(h, x)$ 替换为 $h\in H, x\in X$。令 E 为向量 H-丛，其中基 X，属于类 $C^r$（第 III, §1, no. 8 章，定义 4）。对于$s\in \mathscr{S}^r(X; E)$和$h\in H$，用E的$^hs$截面$x \rightarrow h.s(h^{-1}x)$表示； 映射$(h, s) \rightarrow^hs$是空间$\mathscr{S}^r(X; E)$上H的运算律。

#### 引理 4 {#lie-ix-s6-lem-4 .statement tag=01FD}

运算 $H\times \mathscr{S}^r(X; E)\rightarrow \mathscr{S}^r(X; E)$ 的律是连续的。

鉴于$\mathscr{S}^r(X; E)$的拓扑和拓扑的定义，第1章。 X, §3, no. 4，周四。 3、只要证明对于任意整数$k\leq r$，映射$f: H\times X\times \mathscr{S}^k(X; E)\rightarrow J^k(X; E)$使得$f(h, x, s) =j_x^k(^hs)$是连续的。对于$h\in H$，用X（分别是E）的$\tau_h$（分别是$\theta_h$）自同构$x \rightarrow hx$表示。 定义映射

$$
f_1:H\times X\rightarrow J^k(X,X)
$$

$$
f_2:H\times E\rightarrow J^k(E,E)
$$

$$
g:H\times X\times \mathscr{S}^k(X; E)\rightarrow J^k(X,E)
$$

$f_1(h, x) =j^k_x(\tau_h), f_2(h, v) =j_v^k(\theta_h), g(h, x, s) =j_{hx}^k(s)$。我们有

$$
f(h, x, s) =f_2(h, s(h^{-1}x))\circ g(h^{-1}, x, s)\circ f_1(h^{-1}, x)
$$

因而，通过可微分和解析流形，结果，12.3.6，足以证明 $f_1, f_2$ 和 $g$ 是连续的。

现在$g$是复合映射

$$
H\times X\times \mathscr{S}^k(X; E)-------\longrightarrow^{(m,Id)}X\times \mathscr{S}^k(X; E)
$$

$$
-------\longrightarrow^{(Id,j^k)}X\times \mathscr{C}(X; J^k(X,E))\longrightarrow^{\varepsilon}J^k(X,E)
$$

与 $\varepsilon (x, u) =u(x)$； 映射 $\varepsilon$ 是连续的（总论拓扑，第 X, §3, no. 4 章，$3$ 的 Cor. 1）$,g$ 是连续的。

设 $(h_0, x_0)\in H\times X$；我们将证明$f_1$在$(h_0, x_0)$连续。存在X的图表$(U, \psi ,F)$和$(V, \chi ,F')$以及H的开子集$\Omega$，使得$x_0\in U, h_0\in \Omega$和$m(\Omega \times U)\subset V$。通过使用这些图表中$J^k(X,X)$的表达式，我们可以简化为证明，对于$1\leq l\leq k$，映射$(h, x) \rightarrow \Delta^l_x(\tau_h)$在$(h_0, x_0)$处的连续性从$\Omega \times U$到$P_l(F; F')$，其中$\Delta^l_x(\tau_h)(v) =$$\frac{1}{l!}D^l\tau_h(x).v$为$v\in F ($可微分和分析流形，结果，12.2）。但$D^l\tau_h(x)$只是$m(h, x)$关于$x$的第$l$偏导数，它连续于假设；因而，$f_1$是连续的。 $f_2$连续的证明是相似的，因此引理。

#### 命题 5 {#lie-ix-s6-prop-5 .statement tag=01FE}

假设群 H 是紧致的，并用 $dh$ 表示总质量 1 的 H 的 Haar 测度。令 $s$ 为类 $C^r$ E 的截面。用$s^{\sharp}$向量积分$\int_H^hs dh$表示。则$s^{\sharp}$为类$C^r$E的截面，在H下不变；对于$x\in X$，我们有$s^{\sharp}(x) =\int_Hhs(h^{-1}x)dh\in E_x$。 $\mathscr{S}^r(X; E)$的自同态$s \rightarrow s^{\sharp}$是投影到H不变量截面的子空间。

考虑从 H 到 $\mathscr{S}^r(X; E)$ 映射 $h \rightarrow^hs$；它连续引理 4。由于空间$\mathscr{S}^r(X; E)$是分离且完整的，因此积分$s^{\sharp}=$$\int_H^hs dh$属于到$\mathscr{S}^r(X; E) ($积分，第1章。 III, §3, no. 3，科。 2）。从$\mathscr{S}^r(X; E)$到$E_x$的线性映射$s \rightarrow s(x)$是连续的，对于所有$x\in X$，我们有$s^{\sharp}(x) =$$\int_H^hs(x)dh$。显然$s^{\sharp}$在H下是不变的；如果 $s$ 是 H 不变量截面，我们有 $s^{\sharp}=s$，因此有最后一个断言。

#### 推论 1 {#lie-ix-s6-prop-5-cor-1 .statement tag=01FF}

设 F 为 Banach 空间、$\rho : H\rightarrow \mathbf{G}\mathbf{L}(F)$ 解析线性表示、$f\in \mathscr{C}^r(X; F)$。对于$x\in X$，输入

$$
f^{\sharp}(x) =\int_H\rho (h).f(h^{-1}x)dh
$$

则$f^{\sharp}$从X到F就是类$C^r$的态射，与H的运算兼容；对于$x\in X$，我们有（$\tau_h$表示自同构$x \rightarrow hx$ of X）

$$
d_xf^{\sharp}=\int_H(\rho (h)\circ d_{h^{-1}x}f\circ T_x(\tau_{h^{-1}}))dh\in \mathscr{L}(T_x(X); F) \tag{14}
$$

第一个断言源自应用于捆绑包 $X\times$ F 的命题，配备有运算 $(h; (x, f)) \rightarrow (hx, \rho (h).f)$ 的律。第二个来自集成，第 1 章。 III, §3, no. 2，命题 2，通过应用到向量积分 $f^{\sharp}$ 同态 $d_x:\mathscr{C}^r(X; F)\rightarrow \mathscr{L}(T_x(X); F)$，由紧致 $C^r$ 收敛的拓扑的定义连续。

#### 推论 2 {#lie-ix-s6-prop-5-cor-2 .statement tag=01FG}

设 F 为 Banach 空间, $f\in \mathscr{C}^r(X; F)$；放

$$
f^{\sharp}(x) =\int_Hf(hx)dh
$$

对于$x\in X$。 函数$f^{\sharp}$为类$C^r$，$f^{\sharp}(hx) =f^{\sharp}(x)$为$x\in X$、$h\in H$。

#### 推论 3 {#lie-ix-s6-prop-5-cor-3 .statement tag=01FH}

Let F be a Banach space, $p$ an integer $\geq 0,^k\Omega^p(X; F)$ the space of differential forms of degree $p$ on X, with values in F, and of class $C^k(2\leq k+ 1\leq r)$. 对于$\omega \in^k\Omega^p(X; F)$，输入$\omega^{\sharp}=\int_H\tau_h^*\omega  dh$。 那么映射$\omega  \rightarrow \omega^{\sharp}$是$^k\Omega^p(X; F)$上的投影，其像是H不变形式的子空间。 我们对所有$\omega \in^k\Omega^p(X; F)$都有$d(\omega^{\sharp}) = (d\omega )^{\sharp}$。

第一个断言源自应用于向量 H-bundle Alt$^p(T(X); F)$的命题（第III, §1, no. 8，例）。 为了证明第二个断言，鉴于积分，第 1 章就足够了。 III, §3, no. 2，命题 2，证明当第一个（或第二个）空间给出紧凑 $C^k$ 收敛（或$C^{k-1}$-收敛）的拓扑时，映射 $d:^k\Omega^p(X; F)\rightarrow^{k-1}\Omega^{p+1}(X; F)$ 是连续的。 但这是通过半范数（谱理论，准备中）和$d$是阶$\leq 1 ($可微分和解析流形，结果，14.4.2）的微分算子这一事实直接从这些拓扑的定义得出的。

### 5. 不变微分形式

令X为类$C^{\infty}$的局部有限维实数流形，并令$(g, x) \rightarrow gx$为X上连通的紧李群G的类$C^{\infty}$的左运算的律。对于$g\in G$，用X的$\tau_g$自同构$x \rightarrow gx$表示。用X上类$C^{\infty}$的实微分形式的$\Omega (X)$代数表示（可微分和解析流形，结果，8.3.1）。

对于$\mathfrak{g}$的任何元素$\xi$，用X（III, §3, no. 5）上的$D_{\xi}$相应的向量域和$\theta (\xi ), i(\xi )$相应的运算符表示$\Omega$(X)，这样我们就有公式（可微分和解析流形，结果，8.4.5 和 8.4.7）

$$
\theta (\xi )\omega =d(i(\xi )\omega ) +i(\xi )d\omega \tag{15}
$$

$$
d_**
$$

$$
(\tau_{expt\xi}\omega ) =\tau_{expt\xi}(\theta (\xi )\omega ) \tag{16}
$$

$$
dt
$$

如果 $\tau_g^*\omega =\omega$ 对于所有 $g\in G$，则微分形式 $\omega \in \Omega (X)$ 是不变的；通过公式 (16)，这相当于所有 $\xi \in \mathfrak{g}$ 的 $\theta (\xi )\omega = 0$。用X上不变微分形式的$\Omega (X)^G$空间表示；如果$\omega \in \Omega (X)^G$，我们有$d\omega \in \Omega (X)^G$，所以$\Omega (X)^G$是复形$(\Omega (X), d)$的子复形。

#### 定理 2 {#lie-ix-s6-thm-2 .statement tag=01FI}

典范嵌入 $\iota :\Omega (X)^G\rightarrow \Omega (X)$ 是复数的同伦（阿尔盖布尔，第 X，p. 33，déf. 5）； 映射 $\omega  \rightarrow \omega^{\sharp}=\int_G\tau_g^*\omega  dg$ 是同伦，与其逆同伦。特别地，映射$H(\iota ) : H(\Omega (X)^G)\rightarrow H(\Omega (X))$是双射的。

由科. no. 4、映射$\omega  \rightarrow \omega^{\sharp}$中的3个是从$\Omega (X)$到$\Omega (X)^G$的复合体中的态射，即诱导子复合体$\Omega (X)^G$上的恒等式；因此，要证明定理就足以满足构造同态$s:\Omega (X)\rightarrow \Omega$(X)，分级为次数$-1$，这样

$\omega^{\sharp}-\omega = (d\circ s+s\circ d)(\omega )$ 对于所有$\omega \in \Omega (X)$。 (17)

通过积分的引理 1，章 IX, §2, no. 4和§2, no. 2的注 1，在紧支撑$\mathfrak{g}$上存在正测度$d\xi$，其指数映射下的像等于$dg$。对于 $\omega \in \Omega$(X)，将

$$
s(\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(i(\xi )\omega ).d\xi \}dt
$$

我们必须证明公式 (17) 是满足的。如《Cor》的证明所示。 1 (no. 4)，我们验证公式

$$
ds(\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*d(i(\xi )\omega ).d\xi \}dt
$$

我们现在从公式 (15) 和 (16) 推出等式

$$
ds(\omega ) +s(d\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(d(i(\xi )\omega ) +i(\xi )d\omega ).d\xi \}dt
$$

$$
=\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(\theta (\xi )\omega ).d\xi \}dt
$$

$$
=\int_{\mathfrak{g}}\{\int_0^1\frac{d}{dt}(\tau_{expt\xi}^*\omega )dt\}d\xi
$$

$$
=\int_{\mathfrak{g}}(\tau_{exp\xi}^*\omega -\omega )d\xi
$$

$$
=\omega^{\sharp}-\omega
$$

因此Th。 2.

我们在 X = G 的情况下应用定理，对于 G 的作用进行左平移。 Recall (Chap. III, §3, no. 13, Prop. 50) that associating to a differential form on G its value at the identity element gives an isomorphism from $\Omega (G)^G$ to the graded algebra Alt($\mathfrak{g}$) of alternating multilinear forms on $\mathfrak{g}$. 认同 $\Omega (G)^G$ 与 Alt($\mathfrak{g}$) 通过此同构。 运算符 $d$ 由公式给出（第 III, §3, no. 14 章，第 51 条命题）

$$
d\omega (a_1, . . . , a_{p+1})
$$

$$
=\sum_{i<j}(-1)^{i+j}\omega ([a_i, a_j], a_1, . . . , a_{i-1}, a_{i+1}, . . . , a_{j-1}, a_{j+1}, . . . , a_{p+1})
$$

对于 Alt$^p(\mathfrak{g})$ 中的 $\omega$ 和 $\mathfrak{g}$ 中的 $a_1, . . . , a_{p+1}$。

对于$\xi \in \mathfrak{g}$，令$L_{\xi}$为相应的左不变向量域（通过右平移G的作用本身来定义，cf.章节III, §3, no. 6）。运算符$\theta (L_{\xi}), i(L_{\xi})$与G的作用在由左平移定义的$\Omega (G)$上交换，因此诱导运算符$\theta (\xi ), i(\xi )$在$\Omega (G)^G$上；通过前面的标识，这些由公式表示（可微分和解析流形，结果，8.3.2 和 8.4.2）

$$
(\theta (\xi )\omega )(a_1, . . . , a_p) =-\sum_i\omega (a_1, . . . , a_{i-1},[\xi , a_i], a_{i+1}, . . . , a_p)
$$

$$
(i(\xi )\omega )(a_1, . . . , a_{p-1}) =\omega (\xi , a_1, . . . , a_{p-1})
$$

对于 Alt$^p(\mathfrak{g})$ 中的 $\omega$ 和 $\mathfrak{g}$ 中的 $a_1, . . . , a_p$。

The subcomplex $^G\Omega (G)^G$ of biinvariant forms (Chap. III, §3, no. 13) can be identified with the subcomplex Alt($\mathfrak{g}$)$^G$ of alternating multilinear forms on $\mathfrak{g}$ invariant under the adjoint representation (that is, such that $\theta (\xi )\omega = 0$ for all $\xi \in \mathfrak{g}$). 因此，我们有一个可交换的复数图表

$$
^G\Omega (G)^G\longrightarrow \Omega (G)^G\longrightarrow \Omega (G)
$$

(18)

Alt($\mathfrak{g}$)$^G\longrightarrow$ Alt($\mathfrak{g}$)

其中水平箭头是典范嵌入，垂直箭头是由映射$\omega  \rightarrow \omega (e)$引起的同构。

#### 推论 1 {#lie-ix-s6-thm-2-cor-1 .statement tag=01FJ}

a) 在图表(18)中，所有态射都是同伦。

b) 令 $\omega \in$ Alt($\mathfrak{g}$)。然后$\omega$属于到Alt($\mathfrak{g}$)$^G$当且仅当$d\omega = 0$和$d(i(\xi )\omega ) = 0$对于所有$\xi \in \mathfrak{g}$。复数 Alt($\mathfrak{g}$)$^G$ 的微分是零。

c) 分级的向量空间$H(\Omega (G))$同构于Alt($\mathfrak{g}$)$^G$。

定理，通过左平移应用于 G 上的 G 的作用（对应于 G 上$G\times G$ 的作用 $((g, h);x) \rightarrow gxh^{-1}$）意味着典范嵌入 $\Omega (G)^G\rightarrow \Omega (G)$（对应于 $^G\Omega (G)^G\rightarrow \Omega (G)$）是同伦；鉴于阿尔盖布尔，第一章。 X、p. 34、Cor.、断言 a) 如下。

我们证明b）。根据第 51 章提案。 III, §3, no. 14，对于 G 上左右不变的每个微分形式 $\alpha$，我们有 $d\alpha =-d\alpha$，即 $d\alpha = 0$。因而，如果 $\omega \in$ Alt($\mathfrak{g}$)$^G$，则$d\omega = 0$，因而$d(i(\xi )\omega ) =$ $\theta (\xi )\omega -i(\xi )d\omega = 0$。相反，如果$d\omega = 0$和$d(i(\xi )d\omega ) = 0$，则$\theta (\xi )\omega = 0$。

断言 c) 由 a) 和 b) 得出。

#### 注 {#lie-ix-s6-n5-rem-1 .statement tag=01FK}

考虑 $\Omega (G) ($Algèbre 的子复合体 $Z(\Omega (G))$ 和 $B(\Omega (G))$，第 1 章。 X、p. 25）。从公式给出两个形式的乘积微分（可微分和解析流形，结果，8.3.5），$Z(\Omega (G))$是$\Omega (G)$的子代数，并且$B(\Omega (G))$是$Z(\Omega (G))$；因而，外部乘积诱导在$H(\Omega (G))$上分级为代数结构。前面现在给出了同构分级代数 $H(\Omega (G))\rightarrow$ Alt($\mathfrak{g}$)$^G$。

设 H 为 G 的闭子群；我们应用Th。 2 至 $X = G/H$。由章。 III, §1, no. 8，科。根据第 17 条命题 1，$G/H$ 上的 G 不变微分形式可以与 Alt(T$_e(G/H)$) 的 H 不变元素等同，即与 Alt($\mathfrak{g}$) 的元素相同，它们是 H 不变的并被算子 $i(\xi )$ 湮灭对于所有$\xi \in L(H)$。因而：

#### 推论 2 {#lie-ix-s6-thm-2-cor-2 .statement tag=01FL}

设 H 是 G 的闭子群。

a) 典范嵌入 $\Omega (G/H)^G\rightarrow \Omega (G/H)$ 是同伦。

b) 复数 $\Omega (G/H)^G$ 可以用 Alt($\mathfrak{g}$) 的元素 $\omega$ 的 Alt($\mathfrak{g}$) 由……组成的子复数来识别，它们在 H 的伴随表示下保持不变，并且对于所有的$i(\xi )\omega = 0$ $\xi \in L(H)$。如果在加法中，H是连通的，则该子复合体由$\omega \in$ Alt($\mathfrak{g}$)组成，使得$\theta (\xi )\omega = 0$和$i(\xi )\omega = 0$适用于所有$\xi \in L(H)$。

### 习题{#lie-ix-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
