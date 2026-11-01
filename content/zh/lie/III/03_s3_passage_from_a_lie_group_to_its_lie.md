---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 3
section_title: Passage from a Lie group to its Lie algebra
lang: zh
source: lie-i-iii
book_pages: 238-279, 372-376
pdf_pages: 0256-0297, 0390-0394
extraction: ocr
subsections:
    - "no": 1
      title: CONVOLUTION OF POINT DISTRIBUTIONS ON A LIE GROUP
      page: 238
      pdf_page: 256
    - "no": 2
      title: FUNCTIORAL PROPERTIES
      page: 241
      pdf_page: 259
    - "no": 3
      title: CASE OF A GROUP OPERATING ON A MANIFOLD
      page: 244
      pdf_page: 262
    - "no": 4
      title: CONVOLUTION OF POINT DISTRIBUTIONS AND FUNCTIONS
      page: 245
      pdf_page: 263
    - "no": 5
      title: FIELDS OF POINT DISTRIBUTIONS DEFINED BY THE ACTION OF A GROUP ON A MANIFOLD
      page: 248
      pdf_page: 266
    - "no": 6
      title: INVARIANT FIELDS OF POINT DISTRIBUTIONS ON A LIE GROUP
      page: 249
      pdf_page: 267
    - "no": 7
      title: LIE ALGEBRA OF A LIE GROUP
      page: 251
      pdf_page: 269
    - "no": 8
      title: FUNCTIORIAL PROPERTIES OF THE LIE ALGEBRA
      page: 254
      pdf_page: 272
    - "no": 9
      title: LIE ALGEBRA OF THE GROUP OF INVERTIBLE ELEMENTS OF AN ALGEBRA
      page: 257
      pdf_page: 275
    - "no": 10
      title: LIE ALGEBRAS OF CERTAIN LINEAR GROUPS
      page: 258
      pdf_page: 276
    - "no": 11
      title: LINEAR REPRESENTATIONS
      page: 259
      pdf_page: 277
    - "no": 12
      title: ADJOINT REPRESENTATION
      page: 264
      pdf_page: 282
    - "no": 13
      title: TENSORS AND INVARIANT FORMS
      page: 268
      pdf_page: 286
    - "no": 14
      title: MAURER–CARTAN FORMULAE
      page: 269
      pdf_page: 287
    - "no": 15
      title: CONSTRUCTION OF INVARIANT DIFFERENTIAL FORMS
      page: 271
      pdf_page: 289
    - "no": 16
      title: HAAR MEASURE ON A LIE GROUP
      page: 271
      pdf_page: 289
    - "no": 17
      title: LEFT DIFFERENTIAL
      page: 274
      pdf_page: 292
    - "no": 18
      title: LIE ALGEBRA OF A LIE GROUP GERM
      page: 276
      pdf_page: 294
statements: 111
exercises: 9
content_sha256: 4a29ca82ca192c821473c9ee964e17a9d83aa5e13c3eb9d35aa296879f552164
translated_from: content/en/lie/III/03_s3_passage_from_a_lie_group_to_its_lie.md
translation_method: google
source_content_sha256: 193928cff06a2ceb18dda5088dbb423a5350969e2aae51ddb6917c3c9500b0c0
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 7755fe647ddf25c70963bb23e4bdf221a81985f9c836b7a7a17bf2dde3244e99
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。从李群到李代数的通道

### 1.点分布在李群上的卷积

#### 定义 1 {#lie-iii-s3-def-1 .statement tag=0A98}

*设$G$为李群、$g$和$g'$$G$的两个点，并让$t \in T_g^{(\infty)}(G)$$t' \in T_{g'}^{(\infty)}(G)$为$G$上$g$和$g'$的两个点分布（*可微分和解析流形*，R，13.2.1）。 $t$和$t'$的卷积乘积，用$t * t'$表示，是$G \times G$的映射$(h, h') \mapsto hh'$下$t \otimes t'$的像到$G$（*可微分和解析流形*，R，13.2.3).*

#### 命题 1 {#lie-iii-s3-prop-1 .statement tag=0A99}

(i) *如果 $t \in T_g^{(s)}(G)$ 和 $t' \in T_{g'}^{(s')}(G)$，则 $t * t' \in T_{gg'}^{(s+s')}(G)$。*

(ii) *如果 $t$ 或 $t$ 没有常数项，则 $t * t'$ 没有常数项。*

（三）$\varepsilon_g * \varepsilon_{g'} = \varepsilon_{gg'}$。

(iv) *令 $t \in T_g^{(s)}(G)$、$t' \in T_{g'}^{(s')}(G)$ 且令 $f$ 为类 $C^{s+s'}$ 的函数，位于 $gg'$ 的开邻域与值的 Hausdorff 多范数空间中。然后*

$$
\langle t * t', f \rangle = \langle t', h' \mapsto \langle t, h \mapsto f(hh') \rangle \rangle \\
= \langle t, h \mapsto \langle t', h' \mapsto f(hh') \rangle \rangle.
$$

这是从可微分和解析流形、R、13.4.1、13.2.3 和 13.4.4 得出的。

假设 K = \mathbf{R} 或 \mathbf{C} 并且 G 是有限维的。则 G 是局部紧的。如果 t、t' 是点度量，则 t \* t' 的定义与积分的章 VIII, § 1 一致。稍后我们将看到，度量的卷积乘积和点分布的卷积是分布乘积的卷积的两种特殊情况，而这些分布不一定是点分布。

令 \mathscr{T}^{(\infty)}(G) 为 g \in G 的 T_g^{(\infty)}(G) 的直和（cf. 可微分和解析流形，R，13.6.1）。我们将 \mathscr{T}^{(\infty)}(G) 中的定义卷积乘积作为 \mathscr{T}^{(\infty)}(G) \times \mathscr{T}^{(\infty)}(G) 的双线性映射化为\mathscr{T}^{(\infty)}(G) 扩展定义 1 的卷积乘积。我们也用*表示它。因此，\mathscr{T}^{(\infty)}(G) 有代数结构经过 \mathscr{T}^{(s)}(G) 过滤。 子代数 \mathscr{T}^{(0)}(G) = \bigoplus_{g \in G} T_g^{(0)}(G) 与 K 上的群 G 的代数 K^{(G)} 等价。

#### 命题 2 {#lie-iii-s3-prop-2 .statement tag=0A9A}

代数 \mathscr{T}^{(\infty)}(G) 是结合律。当且仅当 G 是可交换的时，它才是可交换的。

设 t \in \mathscr{T}^{(\infty)}(G)，t' \in \mathscr{T}^{(\infty)}(G)，t'' \in \mathscr{T}^{(\infty)}(G)。那么 t \* (t' \* t'') 是 t \otimes t' \otimes t'' 在映射 (g, g', g'') \mapsto g(g'g'') of G \times G \times G 到 G 下的像和 (t \* t') \* t'' 是像 t \otimes t' \otimes t'' 在映射 (g, g', g'') \mapsto (gg')g'' of G \times G \times G 到 G 中。因此 (t \* t') \* t'' = t \* (t' \* t'')。类似地可以看出，如果 G 是可交换的，则 t \* t' = t' \* t。如果卷积乘积是可交换的，则G可按命题1交换 (iii)。

#### 命题 3 {#lie-iii-s3-prop-3 .statement tag=0A9B}

如果 t \in \mathscr{T}^{(\infty)}(G) 和 g \in G，则 $\gamma(g)_* t = \varepsilon_g * t, \delta(g)_* t = t * \varepsilon_{g^{-1}}$，(Int g)_* t = $\varepsilon_g * t * \varepsilon_{g^{-1}}$。特别地，$\varepsilon_e$是\mathscr{T}^{(\infty)}(G)的单位元。

考虑图表

$$
\begin{array}{ccccc}
G & \xrightarrow{\phi} & G \times G & \xrightarrow{\psi} & G \\
\end{array}
$$

其中$\phi$是映射$h \mapsto (g, h)$，$\psi$是映射$(h', h) \mapsto h'h$。然后$\gamma(g) = \psi \circ \phi$，因此$\gamma(g)_* t = \psi_*(\phi_*(t))$。但是$\phi_*(t) = \varepsilon_g \otimes t$，因此$\psi_*(\phi_*(t)) = \varepsilon_g * t$。 $\delta(g)_* t$ 的论证类似。最后，

$$
\operatorname{Int} g = \gamma(g) \circ \delta(g)
$$

因此$(\operatorname{Int} g)_* = \gamma(g)_* \circ \delta(g)_*$。

因此可以看出，对于$t \in T(G)$，$\varepsilon_g * t$和$t * \varepsilon_g$等于群 T(G) (§ 2, no. 2)中计算的$gt$和$tg$。但需要注意的是，对于T(G)中的$t, t'$，§ 2意义上的乘积$tt'$总体上与$t * t'$不同。

#### 定义 2 {#lie-iii-s3-def-2 .statement tag=0A9C}

令 G 为李群。 e 中包含支持的分布的 $\mathscr{T}^{(\infty)}(G)$ 由……组成的子代数表示为 $U(G)$。

此代数已被子空间过滤
$$
U_s(G) = U(G) \cap \mathscr{T}^{(s)}(G) = T_e^{(s)}(G).
$$
我们写 $U^+(G) = T_e^{(\infty)+}(G)$，$U_s^+(G) = U^+(G) \cap U_s(G)$（cf.可微分和解析流形，R，13.2.1）。回想一下，$U_0(G)$ 用 K 标识，$U_1^+(G)$ 用切线空间 $T_e(G)$ 标识。在$U(G)$中，$U^+(G)$是$U_0(G)$的双面理想补充。

#### 例 {#lie-iii-s3-n1-exa-1 .statement tag=0A9D}

令 E 为完全可范化空间，视为李群。然后向量空间 $U(E)$ 被规范地标识为向量空间 TS(E)（可微分和解析流形，R，13.2.4）。令 E 上的 $m : E \times E \to E$ 为加法，则
$$
m_* : TS(E \times E) \to TS(E)
$$
等于 TS(m)（可微分和解析流形，R，13.2.4）。对于$U(E) = TS(E)$中的$t, t'$，$m_*$下的对称张量积$t \otimes t'$的像$t * t'$因此为TS(m)($t \otimes t'$)。到代数、章 IV, § 5, no. 6、命题 7，这个像只是代数 TS(E) 中的乘积 $tt'$。因此代数$U(E)$被识别为代数TS(E)。

#### 命题 4 {#lie-iii-s3-prop-4 .statement tag=0A9E}

考虑 $U(G) \otimes K^{(G)}$ 到 $\mathscr{T}^{(\infty)}(G)$ 的双线性映射 $(u, v) \mapsto u * v$（分别为 $(u, v) \mapsto v * u$）。 $U(G) \otimes K^{(G)}$到$\mathscr{T}^{(\infty)}(G)$的相应的线性映射是向量空间同构。

$K^{(G)}$ 是 $x \in G$ 的 $K_{e_x}$ 的直和。另一方面，映射$u \mapsto u * \varepsilon_g$（或$u \mapsto \varepsilon_g * u$）是向量空间$U(G) = \mathscr{T}_e^{(\infty)}(G)$到向量空间$\mathscr{T}_g^{(\infty)}(G)$乘命题3的同构。最后，$\mathscr{T}^{(\infty)}(G)$是$T_g^{(\infty)}(G)$ 的直和为 $g \in G$。

设X为类$C^r$($r \geq \infty$)和$x \in X$中的流形。我们定义了（可微分和解析流形，R，13.3.1）对关联分级向量空间的向量空间$\mathscr{T}_x^{(\infty)}(X)$和典范同构$i_{X,x}$到分级向量空间的规范过滤TS(T_x(X))。特别是令 $T_e(G) = L$；那么 $i_{G,e}$ 是分级向量空间 gr U(G) 的同构到分级向量空间 TS(L) 上。但 U(G) 是经过过滤的代数，从中我们可以得到 gr U(G) 上的分级代数结构。

#### 命题 5 {#lie-iii-s3-prop-5 .statement tag=0A9F}

同构$i_{G,e} : \mathrm{gr}\ U(G) \to \mathrm{TS}(L)$是代数同构。

设$p$为$U(G) \times U(G)$的映射$(t, t') \mapsto t \otimes t'$到$U(G \times G)$。令c为$U(G) \times U(G)$到$U(G)$的映射$(t, t') \mapsto t * t'$。设m为G中$G \times G$的映射$(g, g') \mapsto gg'$，然后乘以定义1
$$
c = m_* \circ p.
$$

考虑图表
$$
\begin{array}{ccc}
\mathrm{gr}\,\mathrm{U}(G) \times \mathrm{gr}\,\mathrm{U}(G) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}\,\mathrm{U}(G \times G) \\
\downarrow i_{G,e} \times i_{G,e} & & \downarrow i_{G \times G,e} \\
\mathrm{TS}(L) \times \mathrm{TS}(L) & \xrightarrow{q} & \mathrm{TS}(L \times L) \\
& & \xrightarrow{\mathrm{TS}(T(m))} \mathrm{TS}(L)
\end{array}
$$
其中$q$是从$\mathrm{TS}(L) \times \mathrm{TS}(L)$的典范同构派生到$\mathrm{TS}(L \times L)$的映射。由*可微分和解析流形*，R，13.4.6和13.3.5，图表的两个平方是可交换的。因此由 (1) 图表
$$
\begin{array}{ccc}
\mathrm{gr}\,\mathrm{U}(G) \times \mathrm{gr}\,\mathrm{U}(G) & \xrightarrow{\mathrm{gr}(c)} & \mathrm{gr}\,\mathrm{U}(G) \\
\downarrow i_{G,e} \times i_{G,e} & & \downarrow i_{G,e} \\
\mathrm{TS}(L) \times \mathrm{TS}(L) & \xrightarrow{\mathrm{TS}(T(m)) \circ q} & \mathrm{TS}(L)
\end{array}
$$
是可交换的。现在$T(m): L \times L \to L$映射$(x, y)$到$x + y$（§ 2, no. 1，命题2（ii））。通过*代数*，章IV, § 5, no. 6，命题7，$\mathrm{TS}(T(m)) \circ q$因此是代数$\mathrm{TS}(L)$的乘法。

### 2. 功能特性

#### 命题 6 {#lie-iii-s3-prop-6 .statement tag=0A9G}

令$G, H$为李群，并将$G$的$\phi$态射代入$H$。对于$\mathscr{T}^{(\infty)}(G)$、$\phi_*(t * t') = \phi_*(t) * \phi_*(t')$中的$t, t'$。

考虑图表
$$
\begin{array}{ccc}
G \times G & \xrightarrow{m} & G \\
\phi \times \phi \downarrow & & \downarrow \phi \\
H \times H & \xrightarrow{n} & H
\end{array}
$$
其中$m(g, g') = gg'$，$n(h, h') = hh'$。这个图表是可交换的。因此
$$
\begin{align*}
\phi_*(t * t') &= \phi_*(m_*(t \otimes t')) = n_*((\phi \times \phi)_*(t \otimes t')) \\
&= n_*(\phi_*(t) \otimes \phi_*(t')) = \phi_*(t) * \phi_*(t').
\end{align*}
$$

李群 $G$ 和 $G^\vee$ 具有相同的底层流形，因此向量空间 $\mathscr{T}^{(\infty)}(G)$ 和 $\mathscr{T}^{(\infty)}(G^\vee)$ 是相同的。令$\theta$为映射$g \mapsto g^{-1}$，即李群$G$到李群$G^\vee$的同构。那么$\theta^*$就是向量空间$\mathscr{T}^{(\infty)}(G)$的自同构，自同构我们用$t \mapsto t^\vee$表示。然后$(\varepsilon_g)^\vee = \varepsilon_{g^{-1}}$。如果$t \in T_e(G)$，那么
$$
t^\vee = -t \quad (§ 2, \text{Proposition 2}).
$$

#### 例 {#lie-iii-s3-n2-exa-1 .statement tag=0A9H}

假设$G$是由完全可范化空间$E$定义的李群。然后，$\mathrm{U}(G)$ 用 $\mathrm{TS}(E)$ 标识，限制 $\theta_*$ 到 $\mathrm{U}(G)$ 用 $\mathrm{TS}(T_e(\theta))$ 标识（*可微分和解析流形*，R，13.2.4）。因此，如果$t \in \mathrm{TS}^s(E)$，则$t^\vee = (-1)^s t$。

#### 命题 7 {#lie-iii-s3-prop-7 .statement tag=0A9I}

令 G 为李群。令 t, t' 位于 $\mathscr{T}^{(\infty)}(G)$ 中。

(i) 相对于$G^\vee$计算的乘积$t * t'$等于相对于G计算的乘积$t' * t$。

(ii) $(t * t')^\vee = {t'}^\vee * t^\vee$。

考虑图表

$$
\begin{array}{ccc}
(G_1 \times G_2) \times (G_1 \times G_2) & \xrightarrow{m} & G_1 \times G_2 \\
\downarrow n & & \uparrow p_1 \times p_2 \\
(G_1 \times G_1) \times (G_2 \times G_2)
\end{array}
$$

其中 $s(g, g') = (g', g)$、$m(g, g') = gg'$、$n(g, g') = g'g$ 对于 G 中的所有 $g, g'$。这个图表是可交换的。因此$n_*(t \otimes t') = m_*(s_*(t \otimes t')) = m_*(t' \otimes t)$。这个等式正是(i)。 断言 (ii) 由 (i) 和命题 6 得出。

#### 命题 8 {#lie-iii-s3-prop-8 .statement tag=0A9J}

设G、H为G到H的李群和$\phi$态射。如果$t \in \mathscr{T}^{(\infty)}(G)$，则$\phi_*(t^\vee) = (\phi_*(t))^\vee$。

Let $\theta$ (resp. $\theta'$) be the mapping $g \mapsto g^{-1}$ of G into G (resp. of H into H). 然后$\phi \circ \theta = \theta' \circ \phi$，从而$\phi_*(\theta_*(t)) = \theta'_*(\phi_*(t))$。

#### 命题 9 {#lie-iii-s3-prop-9 .statement tag=0A9K}

设$G_1, \ldots, G_n$为李群和$G = G_1 \times \cdots \times G_n$。如果向量空间$\mathscr{T}^{(\infty)}(G)$和$\mathscr{T}^{(\infty)}(G_1) \otimes \cdots \otimes \mathscr{T}^{(\infty)}(G_n)$被规范地识别，则代数$\mathscr{T}^{(\infty)}(G)$是代数$\mathscr{T}^{(\infty)}(G_1), \ldots, \mathscr{T}^{(\infty)}(G_n)$中的张量积。如果 $t_i \in \mathscr{T}^{(\infty)}(G_i)$ 对应 $i = 1, \ldots, n$，则

$$
(t_1 \otimes \cdots \otimes t_n)^\vee = t_1^\vee \otimes \cdots \otimes t_n^\vee.
$$

考虑$n = 2$的情况就足够了。令$t_1, t_1'$在$\mathscr{T}^{(\infty)}(G_1)$中，$t_2, t_2'$在$\mathscr{T}^{(\infty)}(G_2)$中。我们需要证明$(t_1 \otimes t_2) * (t_1' \otimes t_2') = (t_1 * t_1') \otimes (t_2 * t_2')$和$(t_1 \otimes t_2)^\vee = t_1^\vee \otimes t_2^\vee$。考虑图表

$$
\begin{array}{ccc}
G \times G & \xrightarrow{s} & G \times G \\
\downarrow n & & \downarrow m \\
G & & G
\end{array}
$$

其中$m((x_1, x_2), (x_1', x_2')) = (x_1 x_1', x_2 x_2')$，

$$
n((x_1, x_2), (x_1', x_2')) = ((x_1, x_1'), (x_2, x_2')),
$$

$p_1(x_1, x_1') = x_1 x_1'$，$p_2(x_2, x_2') = x_2 x_2'$。这个图表是可交换的。因此

$$
m_*((t_1 \otimes t_2) \otimes (t_1' \otimes t_2')) = (p_1 \otimes p_2)_*(n_*((t_1 \otimes t_2) \otimes (t_1' \otimes t_2'))),
$$

那是

$$
\begin{align*}
(t_1 \otimes t_2) * (t_1' \otimes t_2') &= (p_1 \otimes p_2)_*((t_1 \otimes t_1') \otimes (t_2 \otimes t_2')) \\
&= p_1*(t_1 \otimes t_1') \otimes p_2*(t_2 \otimes t_2') \\
&= (t_1 * t_1') \otimes (t_2 * t_2').
\end{align*}
$$

类似地可以看出$(t_1 \otimes t_2)^\vee = t_1^\vee \otimes t_2^\vee$。

#### 命题 10 {#lie-iii-s3-prop-10 .statement tag=0A9L}

设 H 是 G 的谎言子群和 $i : H \to G$ 典范嵌入。那么对于所有 $t \in \mathscr{T}^{(\infty)}(H)$，$i_*$ 就是代数 $\mathscr{T}^{(\infty)}(H)$ 的单同态到代数 $\mathscr{T}^{(\infty)}(H)$ 和 $i_*(t^\vee) = (i_*(t))^\vee$。

这是从命题 6 和 8 以及可微分和解析流形，R，13.2.3 得出的。

$\mathscr{T}^{(\infty)}(H)$通过命题10的同构与$\mathscr{T}^{(\infty)}(G)$的子代数进行识别。

#### 注 {#lie-iii-s3-n2-rem-1 .statement tag=0A9M}

如果 H 是李准子群，命题 10 仍然有效。

我们回想一下（可微分和解析流形，R，13.5.1），如果V是K上的解析流形，则$\mathscr{T}^{(\infty)}(V)$在K上具有规范的余代数结构和余单位； 余单位是 $\mathscr{T}^{(\infty)}(G)$ 的线性映射到 K 中，它与 $T_x^{(\infty)}(V)$ 的每个元素其常数项相关联。

#### 命题 11 {#lie-iii-s3-prop-11 .statement tag=0A9N}

令 G 为李群。
(i) 余代数 $\mathscr{T}^{(\infty)}(G)$，通过卷积，是一个大数 (代数, 章 III, § 11, no. 4)。
(ii) 令 c 为 $\mathscr{T}^{(\infty)}(G)$ 上的余积。设 $t \in \mathscr{T}^{(\infty)}(G)$ 并写
$$
c(t) = \sum_{i=1}^n t_i \otimes t_i'.
$$
然后$c(t^\vee) = \sum_{i=1}^n t_i^\vee \otimes t_{i'}^\vee$。

我们证明（i）。在提到的bigebra的定义中，条件（1）从命题2和3得出，条件（2）从可微分和解析流形，R，13.5.1得出。令d为G到$G \times G$的映射$g \mapsto (g, g)$。那么 $c = d_*$ ，因此 c 是代数态射（命题 6 和 9），即条件 (3)。令$t \in T_g^{(\infty)}(G)$、$t' \in T_{g'}^{(\infty)}(G)$没有常数项且$\lambda, \lambda'$为K的元素；则 $\varepsilon_g \otimes t', t \otimes \varepsilon_{g'}, t \otimes t'$ 没有常数项（可微且解析流形，R，13.4.1），因此 $(\lambda \varepsilon_g + t) * (\lambda' \varepsilon_{g'} + t')$ 的常数项为 $\lambda \lambda'$；因此条件 (4) 成立。

我们证明(ii)。到命题 8 和 9 时，
$$
c(t^\vee) = d_*(t^\vee) = (d_*(t))^\vee = \left( \sum_{i=1}^n t_i \otimes t_i' \right)^\vee = \sum_{i=1}^n t_{i'}^\vee \otimes t_{i'}^\vee.
$$

#### 命题 12 {#lie-iii-s3-prop-12 .statement tag=0A9O}

设G，H是G到H的两个李群和$\phi$态射。则$\phi_*$是$\mathscr{T}^{(\infty)}(G)$到$\mathscr{T}^{(\infty)}(H)$的大数态射。

这是从命题 6 和可微分与解析流形, R, 13.5.1 得出的。

令 G 为李群。卷积的限制和U(G)上的余积定义U(G)上的大数结构。我们有 U(G)^{\vee} = U(G)。若$\phi : G \to H$为李群态射，我们将U(G)的U($\phi$)映射$t \mapsto \phi_*(t)$表示为U(H)；这是一个大胸罩态射。如果 $\psi : H \to L$ 是另一个李群态射，则 U($\psi \circ \phi$) = U($\psi$) \circ U($\phi$)。如果 $\phi$ 是浸没（或浸没），则 U($\phi$) 是通过 *可微分和解析流形* 的单射（或满射），R, 13.2.3。特别是，如果 H 是 G 的谎言子群，则 U(H) 可以用 U(G) 的子代数来识别，U(H) 上的余积是 U(G) 上余积的限制。如果 H 在 G 中开集，则 U(H) = U(G)。如果G_1，G_2是李群，则U(G_1 \times G_2)等于U(G_1) \times U(G_2)。 U(G) 的原语元素是 T_e(G) 的原语元素 (*可微分和解析流形*, R, 13.5.3)。

再次令$\phi : G \to H$为李群态射。如果 gr U(G) 被识别为 TS(T_e(G)) 并且 gr U(H) 被识别为 TS(T_e(H))，那么 gr U($\phi$) 被识别为 TS(T_e($\phi$)) (*可微分和解析流形*, R, 13.3.5)。我们将其应用于 G 的同构 $g \mapsto g^{-1}$ 到 G^{\vee} 上；那么 T_e($\phi$) = -1 因此

$$
t \in U_s(G) \Rightarrow t^{\vee} \equiv (-1)^s t \mod U_{s-1}(G).
$$

### 3. 群在流形上运行的情况

令G为类C^r的李群、X流形以及X上G的类C^r的左运算的f律。如果$t \in T^{(s)}_g(G)$和$u \in T^{(s')}_x(X)$和$s + s' \leq r$，我们用$f_*$下的$t \otimes u$的$t * u$像来表示。我们将扩展乘积 \* 转换为$\mathscr{T}^{(s)}(G) + \mathscr{T}^{(s')}(X)$ 的双线性映射（也用 * 表示）到$\mathscr{T}^{(s+s')}(X)$。 命题 1 of no. 1 可以通过对当前情况进行明显修改来扩展。

当G通过左平移对自身进行操作时，我们恢复no. 1的定义1。

#### 命题 13 {#lie-iii-s3-prop-13 .statement tag=0A9P}

令 $t \in \mathscr{T}^{(s)}(G)$, $t' \in \mathscr{T}^{(s')}(G)$, $u \in \mathscr{T}^{(s'')}(X)$, 使得

$$
s + s' + s'' \leq r.
$$

然后$(t * t') * u = t * (t' * u)$。

这可以证明为命题 2 of no. 1。

特别是，如果$r \leq \infty$、向量空间$\mathscr{T}^{(\infty)}(X)$是左模超过代数$\mathscr{T}^{(\infty)}(G)$且乘积*。

#### 命题 14 {#lie-iii-s3-prop-14 .statement tag=0A9Q}

(i) 设$g_0 \in G$和$\tau(g_0)$为X的映射$x \mapsto f(g_0, x)$到X。如果$u \in \mathscr{T}^{(r)}(X)$，则$\tau(g_0)*u = \varepsilon_{g_0}*u$。

(ii) 设$x_0 \in X$和$\varrho(x_0)$为G到X的映射$g \mapsto f(g, x_0)$。如果$t \in T^{(r)}(G)$，则$\varrho(x_0)*t = t*\varepsilon_{x_0}$。

这可以证明为命题 3 of no. 1。

特别地，如果$u \in T(X)$和$t \in T(G)$，则$\varepsilon_{g_0} * u$和$t * \varepsilon_{x_0}$等于§ 2, no. 2中定义的乘积、$g_0u$和$tx_0$。

#### 命题 15 {#lie-iii-s3-prop-15 .statement tag=0A9R}

设 G（分别为 G'）为李群和 X（分别为 X'）流形或类 C^r。假设给定X（或X'）上G（或G'）的类 C^r 的左运算的律。令$\phi$是G到G'的态射，$\psi$是X到X'的$\phi$态射。设$t \in \mathscr{T}^{(s)}(G)$、$u \in T^{(s')}(X)$使得$s + s' \leq r$。然后
$$
\psi_*(t * u) = \phi_*(t) * \psi_*(u).
$$
这可以证明为命题 6 of no. 2。

#### 注 {#lie-iii-s3-n3-rem-1 .statement tag=0A9S}

令f为X上G的类C^r的右运算的律。如果$t \in \mathscr{T}^{(s)}(G)$和$u \in \mathscr{T}^{(s')}(X)$，以及$s + s' \leq r$，我们用$f_*$下的$u \otimes t$的$u * t$像来表示。 命题 13, 14, 15 以明显的方式回顾这种情况。

#### 命题 16 {#lie-iii-s3-prop-16 .statement tag=0A9T}

令 G、G' 为李群、X 流形或类 C^r，并假设 G（或 G'）在左侧（或右侧）的 X 上运行，对所有 $x \in X, g \in G, g' \in G'$ 使用 $(gx)g' = g(xg')$。让$t \in \mathscr{T}^{(s)}(G)$，$t' \in \mathscr{T}^{(s')}(G')$，$t'' \in T^{(s'')}(X)$，还有$s + s' + s'' \leq r$。然后
$$
(t * t'') * t' = t * (t'' * t').
$$
$(t * t'') * t'$（或$t * (t'' * t')$）是$t \otimes t'' \otimes t'$的像在映射$(g, x, g') \mapsto (gx)g'$（或$g(xg')$）下的$G \times X \times G'$到X。

### 4.点分布和函数的卷积

令G为X上类C^r的李群、X流形以及G的类C^r的左运算的$(g, x) \mapsto gx$律。对于所有 $x \in X$，令 $\varrho(x)$ 表示 x 的轨道映射。

#### 定义 3 {#lie-iii-s3-def-3 .statement tag=0A9U}

让 $t \in \mathscr{T}^{(s)}(G)$ 与 $s \leq r$。令 $f : X \to F$ 为类 C^r 的函数，其中值在豪斯多夫多项式空间中（对于例 $F = \mathbf{K}$）。 t 和 f 的卷积（用 $t * f$ 表示）是 X 上的函数，F 中的值定义为
$$
(t * f)(x) = \langle t^\vee * \varepsilon_x, f \rangle.
$$
然后
$$
\begin{align*}
(t * f)(x) &= \langle \varrho(x)_*(t^\vee), f \rangle \quad \text{(no. 3, Proposition 14 (ii))} \\
&= \langle t^\vee, f \circ \varrho(x) \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)} \\
&= \langle t, (f \circ \varrho(x))^\vee \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)}.
\end{align*}
$$
注定义 3 也可以写成更对称的形式
$$
\langle \varepsilon_x, t * f \rangle = \langle t^\vee * \varepsilon_x, f \rangle.
$$
函数$(g, x) \mapsto f(gx) = (f \circ \varrho(x))(g)$在$G \times X$上是类C^r。通过可微分和解析，流形，R，13.4.4，如果$s < \infty$，则函数$x \mapsto \langle t^\vee, f \circ \varrho(x) \rangle$因此为类$C^{r-s}$。在其他字中，如果$s < \infty$，则$t * f$是类$C^{r-s}$。

显然 $t * f$ 线性依赖于 $t$ 和 $f$。

公式 (4) 特别意味着，对于 $g \in G$，
$$
(\varepsilon_g * f)(x) = f(g^{-1}x)
$$
那就是
$$
\varepsilon_g * f = \gamma(g)f.
$$

假设$K = \mathbf{R}$或$\mathbf{C}$，$G$和$X$是有限维的，并且$X$在$G$下具有正测度不变量。 $\varepsilon_g * f$的定义与积分的章VIII, § 4, no. 1一致（cf.公式（2），前述）。

#### 命题 17 {#lie-iii-s3-prop-17 .statement tag=0A9V}

让类$C^r$中的$t \in \mathscr{T}^{(s)}(G)$、$t' \in \mathscr{T}^{(s')}(X)$和$f : X \to F$函数与$s + s' \leq r$。然后
$$
\langle t', t * f \rangle = \langle t^\vee * t', f \rangle.
$$
$$
\begin{align*}
\langle t', t * f \rangle &= \langle t', x \mapsto \langle t, g \mapsto f(g^{-1}x) \rangle \rangle \quad \text{by (4)} \\
&= \langle t \otimes t', (g, x) \mapsto f(g^{-1}x) \rangle \quad (\text{Diff. \& Anal. Man., R, 13.4.4}) \\
&= \langle t^\vee \otimes t', (g, x) \mapsto f(gx) \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3}) \\
&= \langle t^\vee * t', f \rangle.
\end{align*}
$$

#### 命题 18 {#lie-iii-s3-prop-18 .statement tag=0A9W}

设类$C^r$中的$t \in \mathscr{T}^{(s)}(G)$、$t' \in \mathscr{T}^{(s')}(G)$和$f : X \to F$函数，以及$s + s' \leq r$。然后
$$
(t * t') * f = t * (t' * f).
$$
对于所有$x \in X$，
$$
\begin{align*}
\langle \varepsilon_x, (t * t') * f \rangle &= \langle ((t * t')^\vee * \varepsilon_x), f \rangle \quad \text{by (5)} \\
&= \langle {t'}^\vee * (t^\vee * \varepsilon_x), f \rangle \quad (\text{Propositions 2 and 7}) \\
&= \langle t^\vee * \varepsilon_x, t' * f \rangle \quad (\text{Proposition 17}) \\
&= \langle \varepsilon_x, t * (t' * f) \rangle \quad (\text{Proposition 17}).
\end{align*}
$$

如果$r \geq \infty$，我们看到$X$上的类$C^\infty$函数的集合和$F$中的值是左模超过代数$\mathscr{T}^{(\infty)}(G)$。

#### 命题 19 {#lie-iii-s3-prop-19 .statement tag=0A9X}

让$t \in \mathscr{T}^{(s)}(G)$，与$s \leq r$。令 $f$（分别为 $f'$）为 $X$ 上的类 $C^r$ 的函数，其中值在 Hausdorff 多范数空间 $F$（分别为 $F'$）中。令 $(u, u') \mapsto uu'$ 为 $F \times F'$ 的连续双线性映射为 Hausdorff 多范数空间 $F''$，因此 $ff'$ 为 $X$ 上类 $C^r$ 的函数，其中值在$F''$。让
$$
\sum_{i=1}^n t_i \otimes t'_i \text{ be the image of } t \text{ in } \mathscr{T}^{(s)}(G) \otimes \mathscr{T}^{(s)}(G) \text{ under the coproduct. Then}
$$
$$
t * (ff') = \sum_{i=1}^n (t_i * f)(t'_i * f').
$$

让$x \in X$和$\rho(x)$表示$x$的轨道映射。然后
$$
\langle \varepsilon_x, t * (ff') \rangle = \langle t^\vee, (ff') \circ \rho(x) \rangle \quad \text{by (4)} \\
= \langle t^\vee, (f \circ \rho(x))(f' \circ \rho(x)) \rangle \\
= \sum_{i=1}^n \langle t_i^\vee, f \circ \rho(x) \rangle \langle t_{i'}^\vee, f' \circ \rho(x) \rangle \tag{Diff. \& Man. Anal., R, 13.5.2} \\
= \sum_{i=1}^n \langle \varepsilon_x, t_i * f \rangle \langle \varepsilon_x, t_i' * f' \rangle \quad \text{by (4).}
$$

#### 注 1 {#lie-iii-s3-n4-rem-1 .statement tag=0A9Y}

令G为X上G的类$C^r$的李群、X流形和$(x, g) \mapsto xg$律以及类$C^r$的右运算。如果$t \in \mathscr{T}^{(s)}(G)$与$s \leq r$和$f : X \to F$是X上类$C^r$的函数，我们用X上的$f * t$函数表示，定义为
$$
\langle \varepsilon_x, f * t \rangle = \langle \varepsilon_x * t^\vee, f \rangle \\
= \langle \rho(x) * (t^\vee), f \rangle \\
= \langle t^\vee, f \circ \rho(x) \rangle \\
= \langle t, (f \circ \rho(x))^\vee \rangle.
$$
特别是
$$
(f * \varepsilon_g)(x) = f(xg^{-1})
$$
那就是
$$
f * \varepsilon_g = \delta(g)^{-1} f.
$$
命题 17, 18, 19 显然变成了记号，
$$
\langle t', f * t \rangle = \langle t' * t^\vee, f \rangle \tag{11}
$$
$$
f * (t * t') = (f * t) * t' \tag{12}
$$
$$
(ff') * t = \sum_{i=1}^n (f * t_i)(f' * t_i') \tag{13}
$$

#### 命题 20 {#lie-iii-s3-prop-20 .statement tag=0A9Z}

*设 G、G' 为类 $C^r$ 的李群、X 流形以及类的左（或右）运算 $(g, x) \mapsto gx$（分别$(x, g') \mapsto xg'$）律 G（或 G'）在 X 上的$C^r$。假设 $(gx)g' = g(xg')$ 代表所有 $x \in X, g \in G, g' \in G'$。令$t \in \mathscr{T}^{(s)}(G)$、$t' \in \mathscr{T}^{(s')}(G')$和$f : X \to F$为类$C^r$中的函数，使得$s + s' \leq r$。然后*
$$
(t * f) * t' = t * (f * t').
$$
对于所有$x \in X$，
$$
\langle \varepsilon_x, (t * f) * t' \rangle = \langle \varepsilon_x * {t'}^\vee, t * f \rangle \quad \text{by (8)} \\
= \langle t^\vee * (\varepsilon_x * {t'}^\vee), f \rangle \quad \text{(Proposition 17)} \\
= \langle t^\vee * \varepsilon_x, f * t' \rangle \quad \text{(Proposition 2 and (11))} \\
= \langle \varepsilon_x, t * (f * t') \rangle \quad \text{by (5).}
$$

特别是，将 G 视为通过左平移和右平移对其自身进行操作。如果$f : G \to F$是G上类$C^r$的函数并且$t \in \mathscr{T}^{(s)}(G)$（与$s \leq r$），$t * f$和$f * t$，如果$s < \infty$，类$C^{r-s}$的函数在G.进一步，令$t' \in \mathscr{T}^{(s')}(G)$，与$s + s' \leq r$。然后
$$
(t * f) * t' = t * (f * t').
$$
特别是，$\mathscr{C}^\infty(G)$是$(\mathscr{T}^{(\infty)}(G), \mathscr{T}^{(\infty)}(G))$双模。 公式 (5) 和 (8) 承认为特殊情况
$$
\langle t, f \rangle = \langle \varepsilon_e, t^\vee * f \rangle = \langle \varepsilon_e, f * t^\vee \rangle.
$$

#### 注 2 {#lie-iii-s3-n4-rem-2 .statement tag=0AA0}

令$(g, x) \mapsto gx$为X上G的类$C^r$的左运算的律。设$t \in U_s(G)$与$s \leq r$、$\Omega$为X的开子集以及类$C^r$的$f : \Omega \to F$函数。 $t * f$也可以由公式(4)或(5)定义；它是在 $\Omega$ 上定义的函数，F 中的值，如果$s < \infty$，则为类 $C^{r-s}$。这个结果没有。 扩展以明显的方式应对这种情况。

### 5. 点的域分布由群的作用在流形上定义

令$(g, x) \mapsto \lambda(g, x) = gx$为X上G的类$C^r$的左运算的律。设$s \leq r$和$t \in U_s(G)$。对于所有$x \in X$，$t * \varepsilon_x \in T^{(s)}_x(X)$。 映射 $x \mapsto t * \varepsilon_x$ 称为点分布的域，由 X 上的 G 的 t 和作用定义，并用 $D_t^\lambda$ 或简称为 $D_t$ 表示有时。令 $\Omega$ 为 X 的开子集，且 F 为 Hausdorff 多范数空间。如果$f : \Omega \to F$是类$C^r$和$s \leq r$，则$\Omega$上的函数$t^\vee * f$也用$D_t f$表示。然后
$$
(D_t f)(x) = \langle t * \varepsilon_x, f \rangle.
$$
如果$s < \infty$，则$D_t f \in \mathscr{C}^{r-s}(\Omega, F)$乘以no. 4。因此，$f \mapsto D_t f$ 是$\mathscr{C}^r(\Omega, F)$ 的映射变成$\mathscr{C}^{r-s}(\Omega, F)$（通常通过滥用记号来表示为$D_t$）。
如果$t \in U_s(G)$、$t' \in U_{s'}(G)$和$s + s' \leq r$，则通过no. 4的命题 18，
$$
D_{t*t'} = D_{t'}(D_t f)
$$
因此，使用上面指出的记号的滥用，
$$
D_{t*t'} = D_{t'} \circ D_t.
$$
假设 G 和 X 是有限维的。将$T^{(s)}(G) \times X$的映射$(t, x) \mapsto t \otimes \varepsilon_x$转化为向量丛$T^{(s)}(G \times X)$（cf.可微分和解析流形，R，13.2.5）是类$C^{r-s}$。因此（可微分和解析流形，R，13.2.5）$T^{(s)}(G) \times X$的映射$(t, x) \mapsto t * \varepsilon_x$到向量丛$T^{(s)}(X)$是类$C^{r-s}$。特别是，$D_t$是阶$\leq s$和类$C^{r-s}$在可微分和解析流形，R，14.1.6意义上的微分算子。通过公式 (16)，函数 $D_t f$ 则在此微分算子下是 $f$ 的像（可微和解析流形，R，14.1.4）。

我们现在不再假设 G 和 X 是有限维的。令 $\psi$ 为 X 上流形 X 的自同构和点分布的 $\Delta$ 域。与一般的定义一致，$\psi$下$\Delta$的变换是X上点分布的域，其$\psi(x)$下的值是$\psi_*(\Delta(x))$；我们用$\psi(\Delta)$表示这个映射。如果$g \in G$和$\tau(g)$表示X的自同构$x \mapsto gx$，则$\tau(g)$下的$\Delta$的变换也称为g下的$\Delta$的变换。

#### 命题 21 {#lie-iii-s3-prop-21 .statement tag=0AA1}

*设$\psi$为X与G的运算通勤的自同构，则$D_t$在$\psi$下不变。*

对于所有$x \in X$，

$$
\begin{align*}
(\psi(D_t))(\psi(x)) &= \psi_*(D_t(x)) = \psi_*(t * \varepsilon_x) \\
&= t * \psi_*(\varepsilon_x) \tag{Proposition 15} \\
&= t * \varepsilon_{\psi(x)} = D_t(\psi(x)).
\end{align*}
$$

#### 命题 22 {#lie-iii-s3-prop-22 .statement tag=0AA2}

*如果$g \in G$，则g下$D_t$的变换为$D_{\varepsilon_g * t * \varepsilon_g^{-1}}$。*

这个变换在$gx$的值是

$$
\begin{align*}
\tau(g)_*(D_t(x)) &= \tau(g)_*(t * \varepsilon_x) \\
&= \varepsilon_g * (t * \varepsilon_x) \quad \text{(Proposition 14 (i))} \\
&= (\varepsilon_g * t * \varepsilon_g^{-1}) * \varepsilon_{gx} \quad \text{(Propositions 1 and 2)} \\
&= D_{\varepsilon_g * t * \varepsilon_g^{-1}}(gx).
\end{align*}
$$

令$(x, g) \mapsto \mu(x, g) = xg$为X上G的类$C'$右运算的律。设$s \leq r$和$t \in U_s(G)$。对于所有 $x \in X$、$\varepsilon_x * t \in T^{(s)}_x(X)$。 映射 $x \mapsto \varepsilon_x * t$ 被称为 X 上 G 的 t 和作用定义的分布的域，有时表示为 $D_t^u$ 或简称为 $D_t$。设$\Omega$是X的开子集。如果$f : \Omega \to F$是类$C'$，则函数$f * t^\vee$表示为$D_t f$。然后

$$(19)$$
$$(D_t f)(x) = \langle \varepsilon_x * t, f \rangle$$

并且，在明显的记号中，

$$(20)$$
$$D_{t * t'} f = D_t(D_{t'} f)$$

$$(21)$$
$$D_{t * t'} = D_t \circ D_{t'}.$$

命题21 仍然有效。让$g \in G$。 g下的$D_t$的变换（即X的自同构$x \mapsto xg$）是$D_{\varepsilon_g^{-1} * t * \varepsilon_g}$。

### 6. 李群上点的不变域分布

#### 定义 4 {#lie-iii-s3-def-4 .statement tag=0AA3}

*设G为李群。如果 G 上的分布域在 G 的左（或右）平移下保持不变，则称为左（或右）不变。*

在其他字中，$G$上的分布$g \mapsto \Delta_g$的域保持不变，如果
$$
\Delta_{gg'} = \gamma(g) * \beta_{g'}
$$
对于$G$中的$g, g'$，
或者再次如果
$$
\Delta_{gg'} = \varepsilon_g * \Delta_{g'}
$$
$G$ 中的 $g, g'$。
它是右不变式如果
$$
\Delta_{gg'} = \delta({g'}^{-1}) * \Delta_g
$$
对于$G$中的$g, g'$，
或者再次如果：
$$
\Delta_{gg'} = \Delta_g * \varepsilon_g,
$$
对于 $G$ 中的 $g, g'$。

#### 定义 5 {#lie-iii-s3-def-5 .statement tag=0AA4}

*令$G$为李群和$t \in U(G)$。让$L_t$表示$G$上的分布$g \mapsto \varepsilon_g * t$的域和$R_t$域的$G$上的分布$g \mapsto t * \varepsilon_g$。*

在其他字中，$L_t$（或$R_t$）是$t$和$G$定义的分布的域，通过映射$(g, g') \mapsto gg'$在右侧（或左侧）操作$G$。令 $\Omega$ 为 $G$ 的开子集，且 $F$ 为 Hausdorff 多范数空间；如果 $f \in C^\omega(\Omega, F)$，则 $L_t f = f * t^\vee \in C^\omega(\Omega, F)$ 且
$$
R_t f = t^\vee * f \in C^\omega(\Omega, F)
$$
（no. 5）。如果 $G$ 是有限维的，则微分算子 $L_t$ 和 $R_t$ 为类 $C^\omega$ (no. 5)。

#### 命题 23 {#lie-iii-s3-prop-23 .statement tag=0AA5}

(i) *映射$t \mapsto L_t$（或$t \mapsto R_t$）是向量空间$U(G)$的同构到$G$上左（或右）不变分布的向量域。*
(ii) *对于$U(G)$、$L_{t*t'} = L_t \circ L_{t'}$、$R_{t*t'} = R_{t'} \circ R_t$、$L_t \circ R_{t'} = R_{t'} \circ L_t$中的$t, t'$（滥用记号或no. 5）。*
(iii) *如果 $\theta$ 是 $G$ 的映射 $g \mapsto g^{-1}$ 到 $G$，则$\theta(L_t) = R_{t^\vee}$。*
(iv) *如果$t \in U(G)$和$g \in G$，则$(L_t)_g = (R_{\varepsilon_g * t * \varepsilon_g^{-1}})_g$。*

在 $G$ 中，每个右翻译都与每个左翻译进行交换。因此，到 no. 5 的命题 21 时，$L_t$ 保持不变。由于 $(L_t)_e = t$，映射 $t \mapsto L_t$ 是单射的。令$\Delta$为$G$上左不变分布的域；让 $t = \Delta_e$；那么$\Delta$和$L_t$在$e$处具有相同的值并且保持不变，因此$\Delta = L_t$。这证明了$L_t$的(i)，并且对于$R_t$的论证类似。 公式 $L_{t*t'} = L_t \circ L_{t'}$、$R_{t*t'} = R_{t'} \circ R_t$ 由 (21) 和 (18) 得出。设$t \in U_s(G)$、$t' \in U_{s'}(G)$、$f \in C^r(\Omega, F)$，其中$\Omega$在$G$和$s + s' \leq r$开；然后
$$
\begin{align*}
L_t R_{t'} f &= L_t ({t'}^\vee * f) = ({t'}^\vee * f) * t \\
&= {t'}^\vee * (f * t^\vee) \tag{Proposition 20} \\
&= R_{t'} L_t f
\end{align*}
$$
因此$L_t \circ R_{t'} = R_{t'} \circ L_t$。由于$\theta$是$G$在$G^\vee$上的同构，$\theta(L_t)$是$G$上的右不变分布的域；它的值在$e$是$\theta(t) = t^\vee$；因此$\theta(L_t) = R_{t^\vee}$。最后，
$$
(L_t)_g = \varepsilon_g * t = (\varepsilon_g * t * \varepsilon_g^{-1}) * \varepsilon_g = (R_{\varepsilon_g * t * \varepsilon_g^{-1}})_g.
$$

#### 注 1 {#lie-iii-s3-n6-rem-1 .statement tag=0AA6}

它是 G 本身的作用右平移，即左不变分布的定义域。

#### 注 2 {#lie-iii-s3-n6-rem-2 .statement tag=0AA7}

假设 G 是有限维的。 映射

$$(t, g) \mapsto (\mathbf{R}_t)_g = t * \varepsilon_g$$

$U_s(G) \times G$ 化为 $T^{(s)}(G)$ 是解析向量丛的同构；对于这个映射是双射的，在每个纤维上都是线性的并且是解析的（no. 5）；另一方面，令$\phi : T^{(s)}(G) \to U_s(G) \times G$为逆双射；如果$t \in T^{(s)}_g(G)$，则$\phi(t) = (t * \varepsilon_{g^{-1}}, g)$，因此$\phi$是解析的。 同构 $\phi$ 称为 $T^{(s)}(G)$ 的右平凡化。同样，将$U_g(G) \times G$中的映射$(t, g) \mapsto (\mathbf{L}_t)_g = \varepsilon_g * t$考虑为$T^{(s)}(G)$； 逆同构称为$T^{(s)}(G)$的左平凡化。到限制，我们恢复了$T(G)$（§ 2, no. 2）的右和左平凡化。

### 7.李代数李群

令 G 为李群。在 $U(G)$ 中，与任何联想词代数一样，我们写为 $[t, t'] = t * t' - t' * t$。由于$T_e(G)$是$U(G)$、$[T_e(G), T_e(G)] \subset T_e(G)$的原语元素的集合(章II, § 1, no. 2、命题4)。支架的限制到$T_e(G)$，因此定义在$T_e(G)$李代数结构。

#### 引理 1 {#lie-iii-s3-lem-1 .statement tag=0AA8}

令X和$X'$完全可规范空间，$X_0$是X中0的开邻域，并且将$X_0$的解析映射引入$X'$，使得$f(0) = 0$。令 $f = f_1 + f_2 + f_3 + \cdots$ 为 f 的展开作为级数关于 0 的积分，其中 $f_i$ 是次数 i 在 X 上的齐次连续多项式，值在 $X'$ 上。令t为TS$^2(X)$的元素，被视为X上的点分布，且支持包含在\{0\}中。让$t' = f_*(t) \in TS(X')$。 次数 1 的$t'$的齐次分量是$\langle f_2, t \rangle$。

让 $t'_1$ 成为这个分量。然后，对于 $X'$ 的每个连续线性映射 u 到多范数空间，

$$
u(t'_1) = \langle t', u \rangle \quad \text{because } u \text{ is continuous and linear}
$$
$$
= \langle t, u \circ f \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3})
$$
$$
= \langle t, u \circ f_2 \rangle \quad \text{because } t \in TS^2(X)
$$
$$
= u(\langle t, f_2 \rangle) \quad (\text{Diff. \& Anal. Man., R, 13.2.2}),
$$

从而引理。

#### 命题 24 {#lie-iii-s3-prop-24 .statement tag=0AA9}

令 G 为李群和 $(U, \phi, E)$ G 上的图表，使得 $\phi(e) = 0$。令 V 为 e 的开邻域，使得 $V^2 \subset U$。令 m 为 $\phi(V) \times \phi(V)$ 对 E 的解析映射 $(a, b) \mapsto \phi(\phi^{-1}(a)\phi^{-1}(b))$。令

$$
m = \sum_{i, j \geq 0} m_{i, j}
$$

是 m 的展开作为关于 (0, 0) 的积分级数，其中 $m_{i,j}$ 是 $E \times E$ 上的二次 $(i, j)$ 的双齐次连续多项式，$E$ 上的值。

(i) $m_{i,0} = m_{0,j} = 0$ 适用于所有 $i \neq 1$ 和 $j \neq 1$。
(ii) $m_{1,0}(a, b) = a$ 和 $m_{0,1}(a, b) = b$ 对于所有 $a \in E, b \in E$。
(iii) *令 $\psi : T_e(G) \to E$ 为 $\phi$ 在 e 处的微分。对于$T_e(G)$中的所有$u, v$，

$$
\psi([u, v]) = m_{1,1}(\psi(u), \psi(v)) - m_{1,1}(\psi(v), \psi(u)).
$$

$m(a, 0) = a,\ m(0, b) = b$对于$\phi(V)$中的所有$a, b$，这证明了(i)和(ii)。
令$u, v$位于$T_e(G)$中。让 $T_0(E)$ 等同于 $E$，因此 $\psi$ 等同于 $T_e(\phi)$：
$T_e(\phi)$下的$u$和$v$中的像是$\psi(u)$和$\psi(v)$。这些像的张量积点分布是$(\psi(u), 0)$和$(0, \psi(v))$在$TS(E \times E) = TS(E) \times TS(E)$的对称乘积，即

$$
(\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0).
$$

因此，$\phi * (u * v)$是上述元素的像在$\phi(V) \times \phi(V)$的映射$m$下到$E$。 $TS(E)$ 中次数 1 的分量是引理 1，

$$
x = \langle m_{1,1}, (\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0) \rangle.
$$

我们定义双线性映射 $n : (E \times E)^2 \to E$

$$
n((a, b), (a', b')) = m_{1,1}(a, b').
$$

然后$n((a, b), (a, b)) = m_{1,1}(a, b)$，因此

$$
x = \langle n, (\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0) \rangle \\
= m_{1,1}(\psi(u), \psi(v)) + m_{1,1}(0, 0) = m_{1,1}(\psi(u), \psi(v)).
$$

类似地，$\phi * (v * u)$承认$m_{1,1}(\phi(v), \phi(u))$是$TS(E)$中次数1的组成部分。由于 $\phi([u, v])$ 是次数 1，这就证明了 (iii)。

#### 推论{#lie-iii-s3-n7-cor-1 .statement tag=0AAA}

*normable 空间 $T_e(G)$ 与括号一起，是normable 李代数。*

#### 定义 6 {#lie-iii-s3-def-6 .statement tag=0AAB}

*可范化空间$T_e(G)$与括号一起称为G的可范化李代数，或简称为G的李代数，记为$L(G)$。*

#### 命题 25 {#lie-iii-s3-prop-25 .statement tag=0AAC}

*设 G 为李群和 $E(G)$ $L(G)$ 的包络代数。将$L(G)$的典范嵌入转换为$E(G)$定义同态$\theta$将代数$E(G)$转换为代数$U(G)$。如果 K 的特征为 0，则 $\eta$ 是大数同构。*

bigebra $U(G)$ 是可交换的（*可微分和解析流形*，R，13.5.1），并且过滤 $(U_s(G))$ 与 bigebra 结构兼容。 $U(G)$的原语元素的集合是$L(G)$。然后应用章 II, § 1, no. 6、定理 1 即可。

当 K 的特征为 0 时，我们将来将用 $L(G)$ 包络代数来实现认同 $U(G)$。由(2)和命题7(ii)，$U(G)$到$U(G)$的映射$t \mapsto t^\vee$然后被识别为$U(G)$(章I, § 2, no. 4)的主要反自同构。

#### 命题 26 {#lie-iii-s3-prop-26 .statement tag=0AAD}

*假设K的特征为$p > 0$。对于所有 $a \in L(G)$、$a^p \in L(G)$ 和 $\operatorname{ad}(a^p) = (\operatorname{ad} a)^p$（幂 $a^p$ 按 $U(G)$ 计算）。*

如果$a \in L(G)$，$a$在$U(G)$中是原语，因此$a^p$在$U(G)$中是原语（章II, § 1, no. 2，*注1*），因此$a^p \in L(G)$。令$\sigma_a$（或$\tau_a$）为$U(G)$的线性映射$x \mapsto a * x$（或$x \mapsto x * a$）到$U(G)$。对于所有$x \in U(G)$，$(\operatorname{ad} a)(x) = (\sigma_a - \tau_a)(x)$，因此$(\operatorname{ad} a)^p = (\sigma_a - \tau_a)^p$。但$\sigma_a$和$\tau_a$通勤，因此$(\sigma_a - \tau_a)^p = (\sigma_a)^p - (\tau_a)^p = \tau_a^p - \sigma_a^p$、从而是第二个断言。

#### 定义 7 {#lie-iii-s3-def-7 .statement tag=0AAE}

*设X为类$C^r$($r \geq 2$)的流形，且$g$为完全规范李代数。 A law of infinitesimal left (resp. right) operation of class $C^{r-1}$ of $g$ on X is a mapping $a \mapsto D_a$ of $g$ into the set of vector fields on X with the following properties:*

(a) *映射 $(a, x) \mapsto D_a(x)$ 是向量丛 $g \times X$ 的类 $C^{r-1}$ 的态射到向量丛 $T(X)$；*

(b) $[D_a, D_b] = -D_{[a, b]}$（$[D_a, D_b] = D_{[a, b]}$适用于$g$中的所有$a, b$）。

特别地，每个向量域$D_a$都是类$C^{r-1}$。

#### 注 {#lie-iii-s3-n7-rem-1 .statement tag=0AAF}

令X为类$C^r$的流形，$g$为有限维李代数，将$g$的$a \mapsto D_a$线性映射转换为向量域的向量空间类$C^{r-1}$于X。那么定义7中的条件(a)成立。因为，通过考虑$g$和应用*可微分和解析流形*的基，R，7.7.1，问题被简化为情况$\dim g = 1$，然后我们的断言是显而易见的。

#### 命题 27 {#lie-iii-s3-prop-27 .statement tag=0AAG}

*设 G 为类 $C^r$ 中的李群和 X 流形。 Suppose that a law of left (resp. right) operation of class $C^r$ of G on X is given. 对于所有 $a \in L(G)$，令 $D_a$ 为由 X 定义的点分布的域。*

(i) *映射 $(a, x) \mapsto D_a(x)$ 是类 $C^{r-1}$ 的态射，将琐碎的向量丛 $L(G) \times X$ 化为向量丛 $T(X)$。*

(ii) *令I为K包含0的开子集和类$C^r$的$\gamma : I \to G$映射，使得$\gamma(0) = e$。让$a = T_0(\gamma)1 \in L(G)$。如果 f 在 X 的开子集上是类 $C^r$ 的函数，则*
$$
(D_a f)(x) = \lim_{k \in \mathbf{K}^*, k \to 0} k^{-1}(f(\gamma(k)x) - f(x)) \quad \text{if G operates on the left,}
$$
$$
(D_a f)(x) = \lim_{k \in \mathbf{K}^*, k \to 0} k^{-1}(f(x\gamma(k)) - f(x)) \quad \text{if G operates on the right.}
$$

(iii) *If $r \geq 2$, the mapping $a \mapsto D_a$ is a law of infinitesimal left (resp. right) operation of class $C^{r-1}$ of $L(G)$ on X.*

假设G对左边的X进行运算。设$\phi : G \times X \to X$为运算的律。那么$T(\phi)$是向量丛$T(G) \times T(X)$到向量丛$T(X)$的类$C^{r-1}$的$\phi$态射（*可微分和解析*

流形，R，8.1.2）。诱导的向量丛 $(\mathrm{T}(G) \times \mathrm{T}(X))|_{\{\epsilon\} \times X}$ 被识别为 $E = L(G) \times T(X)$。因此$T(\phi)|E$是类$C^{r-1}$的向量丛态射。对于 $(a, x) \in L(G) \times X, T(\phi)(a, x) = D_a(x)$，从而 (i)。

公式给出 $(D_a f)(x)$ 从 § 2 得出，no. 2 的末尾，以及可微分和解析流形，R，8.4.5。

假设$r \geqslant 2$。令$a, b$在$L(G)$中，并且$f$在$X$的开子集上，为类$C^r$中的函数。然后
$$
\begin{align*}
D_{[a, b]}f &= D_b(D_a f) - D_a(D_b f) \quad \text{by (17)} \\
&= [D_b, D_a]f \tag{Diff. \& Anal. Man., R, 8.5.3}.
\end{align*}
$$
让$x \in X$。将$f$视为$x$的开邻域上的图表，可得出$D_{[a, b]}(x) = [D_b, D_a](x)$、从而 (iii)。如果$G$对右侧的$X$进行运算，则论证类似。

当$r \geqslant 2$时，映射$a \mapsto D_a$被称为无穷小运算的律，与运算的给定律相关联。

### 8. 李代数的功能特性

设$G$和$H$为$G$的李群和$\phi$态射到$H$。 $U(\phi)$到$L(G)$的限制，即$T_e(\phi)$，是$L(G)$到$L(H)$的连续态射，我们用$L(\phi)$表示。如果$\psi$是$H$的态射到李群，则$L(\psi \circ \phi) = L(\psi) \circ L(\phi)$。

为了使$\phi$成为浸没，$L(\phi)$是$L(G)$的同构到$L(H)$的子代数上，并承认拓扑补充是必要且充分的。特别地，如果$G$是$H$的谎言子群并且$\phi$是典范嵌入，则通过$L(\phi)$将$L(G)$与$L(H)$的谎言子代数进行识别。更具体地，如果$G$是$H$的开子群，则$L(G) = L(H)$。

如果$G$是$H$的李准子群，则$L(G)$也可以用$L(H)$的闭李子群来标识。

对于$\phi$是淹没，$L(\phi)$是满射并且其核承认拓扑补充是必要且充分的。在这种情况下，$\phi$的核$N$是$G$和$L(N) = \operatorname{Ker} L(\phi)$的谎言子群。特别是，如果 $H$ 是 $G$ 与普通李子子群 $P$ 的商李群，则 $L(P)$ 是 $L(G)$ 的理想，并且，如果 $\phi$ 是 $G$ 的典范满射到当经过商时，$H$、$L(G/P)$通过从$L(\phi)$导出的态射与$L(G)/L(P)$等同。

令$I$是有限的集合，$(G_i)_{i \in I}$是李群的族，$G$是它们的乘积，$p_i$是$G$到$G_i$的规范态射。则$(L(p_i))_{i \in I}$化为李代数$\prod_{i \in I} L(G_i)$为李代数$L(G)$态射且可规范空间为同构。因此，$L(G)$ 通过$(L(p_i))_{i \in I}$ 与$\prod_{i \in I} L(G_i)$ 进行识别。

#### 命题 28 {#lie-iii-s3-prop-28 .statement tag=0AAH}

设G和H为李群，G到H的φ态射。假设K的特征为0，H是有限维的。

(i) φ 的核 N 是 G 的谎言子群，并且 L(N) = Ker L(φ)。

(ii) 当经过到商是浸没时，从 φ 导出 G/N 的态射 ψ 到 H。

(iii) 如果 φ(G) 在 H 中闭，并且 G 的拓扑具有可数基，则 φ(G) 是 H 的谎言子群，ψ 是李群 G/N 到李群 φ(G) 上的同构，且 L(φ(G)) = Im L(φ)。

让 G 对左侧的 H 进行映射 (g, h) ↦ φ(g)h 运算。满足§ 1, no. 7的应用命题14、e的轨道。

#### 命题 29 {#lie-iii-s3-prop-29 .statement tag=0AAI}

设G和H为李群，G到H的φ态射。假设K的特征为0，H是有限维的。如果 H' 是 H 的谎言子群，则 G' = φ⁻1(H') 是 G 的谎言子群，并且 L(G') = L(φ)⁻1(L(H'))。

令 π 为 H 的典范映射到齐次空间 X = H/H'。让 G 对左侧的 X 进行映射 (g, x) ↦ φ(g)x 运算。 π(e) 的稳定子是 G'，因此是 G 的谎言子群 (§ 1, no. 7, 命题 14)。 π(e) 的轨道映射为 π ∘ φ。通过 § 1 的命题 14，L(G') 等于 L(π ∘ φ) = T_e(π) ∘ L(φ) 的核。 T_e(π) 的核为 L(H') (§ 1, no. 6, 命题 11 (i))，因此 Ker L(π ∘ φ) = L(φ)⁻¹(L(H'))。

#### 推论 1 {#lie-iii-s3-prop-29-cor-1 .statement tag=0AAJ}

设G、H为李群，G的φ₁和φ2态射为H。假设K的特征为0，H是有限维的。 g ∈ G 的集合使得 φ₁(g) = φ2(g) 是 G 的李子子群 G'，并且 L(G') 是 x ∈ L(G) 的集合，使得 L(φ₁)x = L(φ2)x。

对于所有 g ∈ G，我们写 φ(g) = (φ₁(g), φ2(g))，因此 φ 是 G 的态射到 H × H 中。令 Δ 为 H × H 的对角线子群。则 G' = φ⁻1(Δ) 且 L(φ)x = (L(φ₁)x， L(φ2)x) 对于所有 x ∈ L(G)。现在足以应用命题 29。

#### 推论 2 {#lie-iii-s3-prop-29-cor-2 .statement tag=0AAK}

设G是有限维李群，G₁和G2是G的两个谎言子群。假设K的特征为0。则G₁∩G2是G的谎言子群，其中李代数L(G₁)∩L(G2)。

我们将G₁的应用命题29到典范嵌入转化为G和子群G2。

#### 推论 3 {#lie-iii-s3-prop-29-cor-3 .statement tag=0AAL}

令 G、G'、H 为李群，且 φ : G → H 且 φ' : G' → H 李群态射。假设 K 的特征为 0，并且 H 是有限维的。令 F 为 (g, g') ∈ G × G' 的集合，使得 φ(g) = φ'(g')。那么 F 是 G × G' 的谎言子群，L(F) 是 (x, x') ∈ L(G) × L(G') 的集合，使得 L(φ)x = L(φ')x'。

我们将推论 1 应用于 G × G' 的态射 (g, g') ↦ φ(g) 和 (g, g') ↦ φ'(g') 到 H 中。

#### 命题 30 {#lie-iii-s3-prop-30 .statement tag=0AAM}

设 G 是有限维李群且具有可数基且

H 和 H' 位于 G 的子群。假设 K 的特征为 0，并且 HH' 在 G 中局部闭。

(i) HH' 是 G 和 $T_e(HH') = L(H) + L(H')$ 的子流形。

(ii) 假设 H 的每元素与 H' 的每元素都可交换。那么 HH' 是 G 的谎言子群。设 $\phi$ 是 $H \times H'$ 的映射 $(h, h') \mapsto hh'$ 到 HH' 上。 $\phi$的核是$(m, m^{-1})$的集合，其中$(H \times H')/\mathrm{Ker}\ \phi$的$m \in H \cap H'$和态射到HH'上，从$\phi$通过经过得到的商是李群同构。

让$H \times H'$对右边的G进行映射$((h, h'), g) \mapsto hg{h'}^{-1}$运算。 e 的轨道映射 $\rho$ 为 $(h, h') \mapsto h{h'}^{-1}$。由§ 1, no. 7的命题14(iii)，HH'是G和$T_e(HH') = \mathrm{Im}\ T_e(\rho)$的子流形。现在

$$
T_e(\rho)(L(H) \times \{0\}) = L(H) \quad \text{and} \quad T_e(\rho)(\{0\} \times L(H')) = L(H')
$$

因此$T_e(HH') = L(H) + L(H')$。假设 H 的每个元素与 H' 的每个元素都可交换。那么HH'是G的子群。通过(i)，它是G的谎言子群。叙述的其余部分从命题28得出。

#### 命题 31 {#lie-iii-s3-prop-31 .statement tag=0AAN}

设 G 为有限维李群，可数基，H 为 G 的正规谎言子群，A 为 G 的谎言子群。假设 K 的特征为 0，且 AH 是闭集。令 $\phi$ 为 G 在 G/H 上的规范态射。然后典范映射

$$
A/(H \cap A) \to \phi(A), \qquad AH/H \to \phi(A)
$$

是李群同构。

到命题 30，AH 是G 的谎言子群。根据推论2 到命题 29，$H \cap A$ 是G 的谎言子群。因此，谈论群 $AH/H$ 和$A/(H \cap A)$ 是有意义的。另一方面，$\phi(A)$，即 G/H 中 AH 的典范像，是闭集，因此是 G/H 的谎言子群 (命题 28 (iii))。 命题 28，应用于复合态射$A \to G \to G/H$和$AH \to G \to G/H$，证明命题的典范映射是李群同构。

#### 命题 32 {#lie-iii-s3-prop-32 .statement tag=0AAO}

令 G 和 H 为李群，k 为 K 的非离散闭子域和 G 的 $\phi$ 态射到 H 中，对于 k 上的李群结构。假设 K 的特征为 0。如果 $L(\phi)$ 是 K 线性的，则对于 K 上的李群结构，$\phi$ 是态射。

对于所有$g \in G$，

$$
T_g(\phi) = T_e(\gamma(\phi(g))) \circ L(\phi) \circ T_g(\gamma(g)^{-1})
$$

因此 $T_g(\phi)$ 是 K 线性的。 命题然后从可微分和解析流形，R，5.14.6 得出。

### 9. 群的可逆元代数的李代数

设$A$是代数与单位元$e$的完全规范关联。令$A^*$为$A$的可逆元中的群。我们已经看到（§ 1, no. 1）$A^*$是$A$的开子流形，并且是李群。令$G$为李群，并将李群$G$中的$f$态射转化为李群$A^*$。 $f$ 可以被视为 $G$ 的解析映射到完全可范化空间 $A$。因此，如果$t \in \mathscr{T}^{(\infty)}(G)$，我们可以形式$\langle t, f \rangle$，即元素除以$A$。

#### 命题 33 {#lie-iii-s3-prop-33 .statement tag=0AAP}

*映射$t \mapsto \langle t, f \rangle$是代数$\mathscr{T}^{(\infty)}(G)$中的态射变成代数$A$。*

只要验证一下，如果$t$和$t'$是$G$上的点分布，则$\langle t * t', f \rangle = \langle t, f \rangle \langle t', f \rangle$。但是
$$
\begin{align*}
\langle t * t', f \rangle &= \langle t \otimes t', (g, g') \mapsto f(gg') \rangle \\
&= \langle t \otimes t', (g, g') \mapsto f(g)f(g') \rangle \\
&= \langle t, f \rangle \langle t', f \rangle
\end{align*}
$$
*（差异和肛门曼，R，13.4.3）*。

命题 33 中的态射据说与 $f$ *相关联。

将$G$视为群$A^*$本身，并将$f$视为$A^*$的恒等映射$i$。我们获得态射，称为*规范*，将代数$\mathscr{T}^{(\infty)}(A^*)$转化为代数$A$。切线空间 $T_e(A^*)$ 规范地等同于 $A$；如果$t \in T_e(A^*)$，则该识别的定义使得$\langle t, i \rangle = t$。那么命题 33 意味着以下推论：

#### 推论{#lie-iii-s3-n9-cor-1 .statement tag=0AAQ}

*$L(A^*)$的典范映射$\zeta$到$A$是李代数的同构，$L(A^*)$到李代数$A$。在其他字，
$$
\zeta([a, b]) = \zeta(a)\zeta(b) - \zeta(b)\zeta(a)
$$
对于$L(A^*)$中的所有$a, b$。如果 $K$ 具有特征 $p > 0$，则 $\zeta(a^p) = \zeta(a)^p$ 对于所有 $a \in L(A^*)$。*

从此以后，$L(A^*)$和$A$通过同构$\zeta$来识别。

$\mathscr{T}^{(\infty)}(A^*)$到$A$的规范态射已经作为命题33的态射的特例获得。但也可以从相反的方向争论：

#### 命题 34 {#lie-iii-s3-prop-34 .statement tag=0AAR}

*设 $H$ 为李群，$A$ 为单位完全规范结合律代数和 $\phi : H \to A^*$ 李群态射。通过将$\phi_*$与$\mathscr{T}^{(\infty)}(A^*)$的规范态射组合到$A$中，获得$\mathscr{T}^{(\infty)}(H)$的相关态射$\phi'$到$A$的关联。特别是，$\phi'(x) = L(\phi)(x)$适用于所有$x \in L(H)$。*

设$i$为$A^*$到$A$的恒等映射。那么，对于所有$t \in \mathscr{T}^{(\infty)}(H)$，
$$
\begin{align*}
\phi'(t) &= \langle t, \phi \rangle = \langle t, i \circ \phi \rangle \\
&= \langle \phi_*(t), i \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)}.
\end{align*}
$$

### 10. 李代数某些线性群

令 E 为完全范数空间。那么$\mathscr{L}(E)$是单位完全范数代数，$\mathbf{GL}(E)$是李群。根据命题 33、no. 9的推论，如果$T_1(\mathbf{GL}(E))$与$\mathscr{L}(E)$规范地一致，$\mathbf{L}(\mathbf{GL}(E))$上的李代数结构由两个元素的括号$(x, y) \mapsto xy - yx$给出$\mathscr{L}(E)$。特别是，$\mathbf{L}(\mathbf{GL}(n, K))$ 被规范地标识为 $\mathfrak{gl}(n, K)$ (章 I, § 1, no. 2)。

#### 命题 35 {#lie-iii-s3-prop-35 .statement tag=0AAS}

*设E为有限维向量空间。令$\phi$为李群$\mathbf{GL}(E)$中的态射$g \mapsto \det g$变成李群$K^*$。 $\mathscr{L}(E)$到K中的映射$\mathbf{L}(\phi)$为映射$x \mapsto \operatorname{Tr} x$。 $\phi$的核$\mathbf{SL}(E)$是$\mathbf{GL}(E)$的谎言子群与李代数$\mathfrak{sl}(E)$。*

我们行列式的E.展开的选择范数和基证明了
$$
\det(1 + u) \in 1 + \operatorname{Tr} u + o(\|u\|)
$$
当$u$在$\mathscr{L}(E)$趋于0时。因此，使用命题 34、no. 9 来表示 $x \in \mathscr{L}(E) = \mathbf{L}(\mathbf{GL}(E))$：
$$
\mathbf{L}(\phi)(x) = \langle x, \phi \rangle = \operatorname{Tr} x.
$$
由此可见$\phi$是淹没。因此，$\operatorname{Ker} \phi = \mathbf{SL}(E)$是$\mathbf{GL}(E)$的谎言子群，其李代数是$\operatorname{Ker} \mathbf{L}(\phi) = \mathfrak{sl}(E)$。

令 $E_1, \ldots, E_n$ 完全可范化空间且 E 为直和。每个$x \in \mathscr{L}(E)$都可以用矩阵$(x_{ij})_{1 \leq i, j \leq n}$来表示，其中$x_{ij} \in \mathscr{L}(E_i, E_j)$。

#### 命题 36 {#lie-iii-s3-prop-36 .statement tag=0AAT}

*设I为$\{1, 2, \ldots, n\}$的子集，G子群为$g = (g_{ij})_{1 \leq i, j \leq n} \in \mathbf{GL}(E)$的$\mathbf{GL}(E)$由……组成，这样$g_{ij} = 0$为$i < j$，$g_{ii} = 1$为$i \in I$。那么 G 是 $\mathbf{GL}(E)$ 的谎言子群，$\mathbf{L}(G)$ 是 $x = (x_{ij})_{1 \leq i, j \leq n} \in \mathscr{L}(E)$ 的集合，这样 $x_{ij} = 0$ 对应 $i < j$，$x_{ii} = 0$ 对应 $i \in I$。

令 S 为 $(x_{ij}) \in \mathscr{L}(E)$ 的集合，使得 $i < j$ 为 $x_{ij} = 0$，$i \in I$ 为 $x_{ii} = 0$。那么G就是$\mathbf{GL}(E)$的交和$\mathscr{L}(E)$的仿射子空间$1 + S$。因此，G 是 $\mathbf{GL}(E)$ 的子流形，G 在 1 处的切线空间用 S 标识。*

特别是，在 $\mathbf{GL}(n, K)$ 中，总下三角子群和下严格三角形子群（如积分中定义的章 VII, § 3, no. 3）是谎言子群以及李代数 $t(n, K)$ 和 $n(n, K)$ （章I, § 1, no. 2）。

#### 命题 37 {#lie-iii-s3-prop-37 .statement tag=0AAU}

*设 A 是完全规范单位结合律代数和 $x \mapsto x^t$ A 到 A 中的连续线性映射，使得 A 中所有 $x, y$ 都有 $(x^t)^t = x$ 和 $(xy)^t = y^t x^t$。假设 K 具有特征 $\neq 2$。令 G 为 $x \in A$ 的 $A^*$ 由……组成的子群，使得 $xx^t = x^t x = 1$。那么 G 是 $A^*$ 的谎言子群，并且 $\mathbf{L}(G)$ 是 $y \in A$ 的集合，使得 $y^t = -y$。*

令 S（或 S'）为 $y \in A$ 的集合，使得 $y = y^t$（或 $y = -y^t$）。那么 S, S' 闭合 A 的向量子空间。 公式

$$
y = \frac{1}{2}(y + y^t) + \frac{1}{2}(y - y^t)
$$

证明A是S和S'的拓扑直和。令 f 为由 $f(x) = xx^t$ 定义的 A 到 S 的映射。这个映射是分析性的。对于所有$y \in A$、$f(1 + y) = 1 + y + y^t + yy^t$； A 上的选择范数与其代数结构兼容；然后

$$
f(1 + y) \in 1 + y + y^t + o(\|y\|) \quad \text{for } y \text{ tending to } 0.
$$

因此，$T_1(f)(y) = y + y^t$，因此 f 是 1 处的淹没。因此，A 中存在 1 的开邻域 U，使得 $U \cap G$ 是 U 的子流形。因此 (§ 1, no. 3, 命题 6) G 是 A* 的谎言子群。而且，$L(G) = T_e(G) = \operatorname{Ker} T_1(f)$。

#### 推论 1 {#lie-iii-s3-prop-37-cor-1 .statement tag=0AAV}

*假设K的特征为$\neq 2$。设 E 为 K 上的有限维向量空间，且 $\phi$ 为 E 上的非简并对称（分别为交错的）双线性形式。对于所有 $u \in \mathscr{L}(E)$，令 $u^*$ 为 u 相对于 $\phi$ 的伴随。令 G 为 $\phi$ 的正交（或辛）群。那么 G 是 $\mathbf{GL}(E)$ 的谎言子群，并且 $L(G)$ 是 $x \in \mathscr{L}(E)$ 的集合，使得 $x^* = -x$。

我们应用命题 37 与 $A = \mathscr{L}(E)$ 和 $x^t = x^*$。*

#### 注 {#lie-iii-s3-n10-rem-1 .statement tag=0AAW}

令 B 为 E 的基和 $\phi$ 的 J 矩阵关于 B。则 $L(G)$ 为 $\mathscr{L}(E)$ 的元素集合，其中关于 B 的矩阵 X 满足等式

$$
{}^tX = -JXJ^{-1}.
$$

这是从 *代数*、章 IX, § 1、公式 (50) 得出的。

#### 推论 2 {#lie-iii-s3-prop-37-cor-2 .statement tag=0AAX}

*令 E 为复数（或实数）希尔伯特空间，U 为 E 的酉群。则 U 为 $\mathbf{GL}(E)$ 的实数子群，$L(U)$ 为 $x \in \mathscr{L}(E)$ 的集合，使得 $x^* = -x$。

我们应用命题 37 和 $A = \mathscr{L}(E)$ 被视为代数超过 $\mathbf{R}$ 和 $x^t = x^*$。*

#### 推论 3 {#lie-iii-s3-prop-37-cor-3 .statement tag=0AAY}

*设 E 为有限维复数向量空间，$\phi$ 为 E 上的非简并厄米特倍半线性形式，U 为 $\phi$ 的酉群。那么 U 是 $\mathbf{GL}(E)$ 的实谎言子群，$L(U)$ 是 $x \in \mathscr{L}(E)$ 的集合，使得 $ix$ 是厄米特。*

当$E \neq \{0\}$时，U*不是*复数李群$\mathbf{GL}(E)$的谎言子群，因为$L(U)$不是$\mathscr{L}(E)$的复数向量子空间。

### 11.线性表示

设 G 为李群，E 为完全可范化空间，$\pi$ 为 G 在 E (§ 1, no. 2) 上的解析线性表示。 $\mathscr{T}^{(\infty)}(G)$到$\mathscr{L}(E)$的关联态射$t \mapsto \langle t, \pi \rangle$是代数态射（no. 9，命题33），其限制到$L(G)$是$L(\pi)$。因此$L(\pi)$是$E$上$L(G)$的表示（章I, § 3，定义1）。

#### 命题 38 {#lie-iii-s3-prop-38 .statement tag=0AAZ}

将$G$视为在映射$(g, x) \mapsto \pi(g)x$左侧的$E$上进行操作。设$b \in E$和$\varphi(b)$为其轨道映射。让 $T_b(E)$ 与 $E$ 被规范地识别。对于所有$t \in L(G)$，

$$
(L(\pi)t)(b) = \langle t, \varphi(b) \rangle = \varphi(b)*t = t * \varepsilon_b.
$$

特别是，$t$在$E$上定义的向量域是域$b \mapsto (L(\pi)t)(b)$。

$L(\pi)t = \langle t, \pi \rangle$（no. 9，命题34）。由于$\mathscr{L}(E)$到$E$的映射$A \mapsto Ab$是连续且线性的，因此

$$
\begin{align*}
(L(\pi)t)(b) &= \langle t, g \mapsto \pi(g)b \rangle \\
&= \langle t, \mathrm{Id}_E \circ \varphi(b) \rangle \\
&= \langle \varphi(b)*t, \mathrm{Id}_E \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3}) \\
&= \varphi(b)*t.
\end{align*}
$$

最后，$\varphi(b)*t = t * \varepsilon_b$（no. 3，命题14（ii））。

#### 命题 39 {#lie-iii-s3-prop-39 .statement tag=0AB0}

假设$K$的特征为0。令$G$为李群，$E$有限维向量空间，$\pi$为$G$在$E$上的解析线性表示。令$E_1, E_2$为$E$的向量子空间，使得$E_2 \subset E_1$。 $g \in G$ 的集合 $G_1$，使得$\pi(g)x \equiv x$（模$E_2$）对于所有$x \in E_1$ 是$G$ 的谎言子群，并且$L(G_1)$ 是$a \in L(G)$ 的集合，这样$L(\pi)a$映射$E_1$变成$E_2$。

这是从命题 29 (no. 8) 和 36 (no. 10) 开始的。

#### 推论 1 {#lie-iii-s3-prop-39-cor-1 .statement tag=0AB1}

在命题 39 的记号、$g \in G$ 的集合中，$\pi(g)(E_1) \subset E_1$ 是$G$ 的谎言子群，并且它的李代数是$a \in L(G)$ 的集合，这样$L(\pi)a$映射$E_1$变为$E_1$。

我们应用命题 39 和 $E_1 = E_2$。

#### 推论 2 {#lie-iii-s3-prop-39-cor-2 .statement tag=0AB2}

令$G, E, \pi$ 与命题 39 相同。令$F$ 为$E$ 的子集。 $g \in G$的集合，使得对于所有$x \in F$来说，$\pi(g)x = x$是$G$的谎言子群，并且它的李代数是$a \in L(G)$的集合，使得对于所有$(L(\pi)a)(x) = 0$ $x \in F$。

我们应用命题 39 与 $E_2 = \{0\}$ 和 $F$ 生成的 $E$ 的 $E_1$ 向量子空间。

令$\pi_1, \pi_2, \ldots, \pi_n$ 为$G$ 的解析线性表示。显然，$\pi_i$（代数，章VIII, § 13, no. 1）的直和$\pi$是$G$的解析线性表示，$L(\pi)$是$L(\pi_1), L(\pi_2), \ldots, L(\pi_n)$的直和 （章I, § 3, no. 1）。

#### 命题 40 {#lie-iii-s3-prop-40 .statement tag=0AB3}

令 $G$ 为李群，$E$ 完全可范空间，$\pi$ $G$ 在$E$ 上的解析线性表示，以及$F$ 闭向量 $E$的子空间稳定在$\pi(G)$以下。假设$K$的特征为0，或者$F$是$E$的直因子。

(i) *子表示* $\pi_1$ *和* $\pi$ *由* $F$ *定义的商表示* $\pi_2$ *是解析的表示*。

(ii) $F$ *在* $L(\pi)(L(G))$ 下稳定。

(iii) *令* $\varrho_1$ *和* $\varrho_2$ *为子表示和* $L(\pi)$ *由* $F$ 定义的商表示。 *然后*$L(\pi_1) = \varrho_1, L(\pi_2) = \varrho_2$。

令$A$为$u \in \mathscr{L}(E)$的集合，使得$u(F) \subset F$。那么$A$是$\mathscr{L}(E)$的闭向量子空间，并且$\pi$在$A$中取其值。根据$K$和$F$的假设，与$\pi$同图的映射$\pi': G \to A$是解析的（*可微且解析流形*，R，5.8.5）。 典范映射 $\theta_1 : A \to \mathscr{L}(F)$ 和 $\theta_2 : A \to \mathscr{L}(E/F)$ 是连续且线性的，因此是解析的。这就证明了(i)。 映射 $T_e(\pi)$ 和 $T_e(\pi')$ 有相同的图，因此$L(\pi)(L(G)) \subset A$，这证明了 (ii)。我们有
$$
T_e(\pi_1) = T_e(\theta_1 \circ \pi') = \theta_1 \circ T_e(\pi') = \varrho_1 \\
T_e(\pi_2) = T_e(\theta_2 \circ \pi') = \theta_2 \circ T_e(\pi') = \varrho_2.
$$

#### 命题 41 {#lie-iii-s3-prop-41 .statement tag=0AB4}

*设*$G$*为李群且*$\pi_1, \pi_2, \ldots, \pi_n, \pi$*在完全可规范空间*$E_1, E_2, \ldots, E_n, E$上解析*$G$的线性表示。 *让*
$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n
$$
*是* $E_1 \times E_2 \times \cdots \times E_n$ *到* $E$ 的连续多重线性映射。 *假设*
$$
\pi(g)(x_1 x_2 \ldots x_n) = (\pi_1(g)x_1)(\pi_2(g)x_2) \ldots (\pi_n(g)x_n)
$$
*对于所有人*$g \in G, x_1 \in E_1, \ldots, x_n \in E_n$。 *然后*
$$
(L(\pi)a)(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 x_2 \ldots x_{i-1} ((L(\pi_i)a)x_i) x_{i+1} \ldots x_n
$$
*对于所有人*$a \in L(G), x_1 \in E_1, \ldots, x_n \in E_n$。

作为例，我们执行$n = 2$的计算。
$$
\begin{align*}
(L(\pi)a)(x_1 x_2) &= \langle a, g \mapsto \pi(g)(x_1 x_2) \rangle & \text{(Proposition 38)} \\
&= \langle a, (g \mapsto \pi_1(g)x_1)(g \mapsto \pi_2(g)x_2) \rangle \\
&= \langle a, g \mapsto \pi_1(g)x_1 \rangle \cdot x_2 + x_1 \cdot \langle a, g \mapsto \pi_2(g)x_2 \rangle & \text{(*Diff.* \& *Anal.* *Man.*, R, 5.5.6)} \\
&= ((L(\pi_1)a)x_1) \cdot x_2 + x_1 \cdot ((L(\pi_2)a)x_2) & \text{(Proposition 38)}.
\end{align*}
$$

#### 推论 1 {#lie-iii-s3-prop-41-cor-1 .statement tag=0AB5}

*设*$G$*为李群，*$E_1, \ldots, E_{n+1}$*完全可范化空间和*$\pi_1, \ldots, \pi_{n+1}$*对*$G$*解析线性表示*$E_1, \ldots, E_{n+1}$。 *让*
$$
E = \mathscr{L}(E_1, \ldots, E_n; E_{n+1})
$$
*将* $E_1 \times \cdots \times E_n$ *的连续多线性映射的完整可规范空间转化为* $E_{n+1}$ *（一般拓扑、章X, § 3, no. 2）*。 *对于所有* $g \in G$，*让* $\pi(g)$ *成为* $E$ *的自同构 *定义为*
$$
(\pi(g)u)(x_1, \ldots, x_n) = \pi_{n+1}(g)(u(\pi_1(g)^{-1}x_1, \ldots, \pi_n(g)^{-1}x_n)).
$$

那么$\pi$是$G$在$E$上的解析线性表示并且
$$
((L(\pi)a)u)(x_1, \ldots, x_n) = -\sum_{i=1}^n u(x_1, \ldots, x_{i-1}, (L(\pi_i)a)x_i, x_{i+1}, \ldots, x_n)
$$
$$
\quad + (L(\pi_{n+1})a)(u(x_1, \ldots, x_n))
$$
对于所有 $a \in L(G)$、$u \in E$、$x_1 \in E_1, \ldots, x_n \in E_n$。

$\mathscr{L}(E_1) \times \cdots \times \mathscr{L}(E_{n+1})$ 定义的每个元素 $(A_1, \ldots, A_{n+1})$ $E$ 的连续自同态 $\theta(A_1, \ldots, A_{n+1})$ 公式
$$
(\theta(A_1, \ldots, A_{n+1})u)(x_1, \ldots, x_n) = A_{n+1}(u(A_1x_1, \ldots, A_nx_n)).
$$
$\mathscr{L}(E_1) \times \cdots \times \mathscr{L}(E_{n+1})$到$\mathscr{L}(E)$的映射$\theta$是连续且多重线性的。那么，对于所有$g \in G$，
$$
\pi(g) = \theta(\pi_1(g^{-1}), \ldots, \pi_n(g^{-1}), \pi_{n+1}(g))
$$
因此 $\pi$ 是解析的。我们应用命题41到映射
$$
(x_1, \ldots, x_n, u) \mapsto u(x_1, \ldots, x_n)
$$
$E_1 \times \cdots \times E_n \times E$ 变为 $E_{n+1}$。然后
$$
\pi_{n+1}(g)(u(x_1, \ldots, x_n)) = (\pi(g)u)(\pi_1(g)x_1, \ldots, \pi_n(g)x_n)
$$
因此
$$
(L(\pi_{n+1})a)(u(x_1, \ldots, x_n)) = \sum_{i=1}^n u(x_1, \ldots, (L(\pi_i)a)x_i, \ldots, x_n)
$$
$$
\quad + ((L(\pi)a)u)(x_1, \ldots, x_n).
$$

当$E_i$为有限维时，$L(G)$的表示$L(\pi)$是由表示$L(\pi_1), \ldots, L(\pi_{n+1})$根据章I, § 3、命题3的过程推导出来的。

#### 推论 2 {#lie-iii-s3-prop-41-cor-2 .statement tag=0AB6}

令$G$为李群，且$\pi$为$G$在完全可规范空间$E$上的解析线性表示。 Then $g \mapsto {}^t\pi(g)^{-1}$ is an analytic linear representation $\rho$ of $G$ on the complete normable space $\mathscr{L}(E, K)$\footnote{As when $K = \mathbf{R}$ or $\mathbf{C}$, the transpose ${}^t\pi(g)$ considered here is the restriction to $\mathscr{L}(E, K)$ of the transpose of $\pi(g)$ in the purely algebraic sense.} and $L(\rho)a = -{}^t(L(\pi)a)$ for all $a \in L(G)$.

这是推论 1 的一个特例。

$\rho$ 被称为 $\pi$ 的*反对* 表示。

当$E$是有限维时，$L(\rho)$是$L(\pi)$的对偶表示，即章I, § 3, no. 3。

#### 推论 3 {#lie-iii-s3-prop-41-cor-3 .statement tag=0AB7}

令$G$为李群，并且$\pi_1, \ldots, \pi_n$在有限维向量空间$E_1, \ldots, E_n$上解析$G$的线性表示。则$G$(附录)的表示$\pi_1 \otimes \cdots \otimes \pi_n$解析，$L(\pi_1 \otimes \cdots \otimes \pi_n)$为$L(\pi_1), \ldots, L(\pi_n)$的张量积。

$\mathscr{L}(E_1) \times \cdots \times \mathscr{L}(E_n)$到$\mathscr{L}(E_1 \otimes \cdots \otimes E_n)$的映射$(A_1, \ldots, A_n) \mapsto A_1 \otimes \cdots \otimes A_n$是多线性的，从而$\pi$是解析的。考虑$E_1 \times \cdots \times E_n$中的映射$(x_1, \ldots, x_n) \mapsto x_1 \otimes \cdots \otimes x_n$
$$
E_1 \otimes \cdots \otimes E_n.
$$
到命题41，我们看到
$$
(L(\pi)a)(x_1 \otimes \cdots \otimes x_n) = \sum_{i=1}^n x_1 \otimes \cdots \otimes (L(\pi_i)a)x_i \otimes \cdots \otimes x_n
$$
对于所有$a \in L(G)$，$x_i \in E_i$对于$1 \leq i \leq n$。因此$L(\pi)$是$L(\pi_i)$的张量积。

#### 推论 4 {#lie-iii-s3-prop-41-cor-4 .statement tag=0AB8}

令$G$为李群，且$\pi$为$G$在有限维向量空间$E$上的解析线性表示。然后对$G$(附录)的表示$T^n(\pi)$、$S^n(\pi)$和$\wedge^n(\pi)$进行解析，
$$
L(T^n(\pi)) = T^n(L(\pi)), \quad L(S^n(\pi)) = S^n(L(\pi)), \quad L(\wedge^n(\pi)) = \wedge^n(L(\pi)).
$$
这是从推论 3 和命题 40 得出的。

#### 推论 5 {#lie-iii-s3-prop-41-cor-5 .statement tag=0AB9}

令 $A$ 为有限维代数。假设$K$的特征为0。$A$的自同构群$\mathrm{Aut}(A)$是$\mathbf{GL}(A)$的谎言子群，$L(\mathrm{Aut}(A))$是$A$的推导的李代数。

这是从推论1（适用于$E = \mathscr{L}(A, A; A)$）和命题39的推论2（仅适用于$E$由……组成的子集，$A$上的乘法）得出的。

#### 注 {#lie-iii-s3-n11-rem-1 .statement tag=0ABA}

我们将推论 1 应用于 $G = \mathbf{GL}(F)$（$F$ 一个完整的可范数空间）、$\pi_1 = \pi_2 = \mathrm{Id}_G$ 和 $\pi_3$ $G$ 的平凡表示在 $K$ 上。我们在 $\mathscr{L}(F, F; K)$ 上获得 $\mathbf{GL}(F)$ 的解析表示 $\pi$。我们假设$F$是有限维的，$K$的特征为0。应用推论2到命题39到$\pi$，我们将推论1的部分恢复到命题37。

#### 命题 42 {#lie-iii-s3-prop-42 .statement tag=0ABB}

令$G$为李群，$X$为$X$上$G$的解析左（或右）运算的解析流形，$(g, x) \mapsto gx$（或$xg$）律，并且$X$的$x_0$点在$G$下不变。对于所有$g \in G$，令$\tau(g)$为$X$的自同构$x \mapsto gx$（分别为$xg$），令$\pi(g)$为$T_{x_0}(X)$在$x_0$处的切线自同构到$\tau(g)$。
(i) $\pi$ 是$G$（或$G^\vee$）在$T_{x_0}(X)$ 上的解析表示。
(ii) 对于所有$a \in L(G)$和所有$\xi_0 \in T_{x_0}(X)$，$L(\pi)a.\xi_0$可以计算如下：令$D_a$为向量域，由$a$在$X$和$\xi$向量上定义类 $C^1$ 的域在$x_0$ 的开邻域中，使得$\xi(x_0) = \xi_0$；然后
$$
L(\pi)a.\xi_0 = -[D_a, \xi](x_0).
$$

$\tau(gg') = \tau(g)\tau(g')$（或$\tau(g')\tau(g)$），因此$\pi(gg') = \pi(g)\pi(g')$（或$\pi(g')\pi(g)$）。另一方面，由于$TX$是类$C^\omega$（§ 1, no. 8，命题16）的向量G丛，$\pi$是解析的，从而(i)。

为了证明(ii)，假设G在左边运算。 K 中存在 0 的开邻域 I，G 中存在 I 的解析映射 $\gamma$，使得 $\gamma(0) = e, T_0(\gamma)1 = a$。那么 $D_a$ 就是 X 上的向量域，由 $I \times X$ 的映射 $\phi : (\lambda, x) \mapsto \gamma(\lambda)x$ 定义为 X (§ 2, no. 2)。如果 $\phi_\lambda$ 表示 X 的双射 $x \mapsto \gamma(\lambda)x$ 到 X，则

$$
[D_a, \xi](x_0) = \left( \frac{d}{d\lambda} (T_{\phi_\lambda(x_0)}(\phi_\lambda^{-1})\xi(\phi_\lambda(x_0))) \right)_{\lambda=0} \quad (\text{Diff. \& Anal. Man., R,}
$$
$$
= \left( \frac{d}{d\lambda} (T_{x_0}(\phi_\lambda^{-1})\xi_0) \right)_{\lambda=0}
$$
$$
= \left( \frac{d}{d\lambda} (\pi(\gamma(\lambda))^{-1}\xi_0) \right)_{\lambda=0}.
$$

由于映射$\lambda \mapsto \gamma(\lambda)^{-1}$和$\lambda \mapsto \gamma(-\lambda)$在0处相切，这也等于
$$
- \left( \frac{d}{d\lambda} (\pi(\gamma(\lambda))\xi_0) \right)_{\lambda=0}
$$
$$
= - \left( \frac{d}{d\lambda} (\pi \circ \gamma)(\lambda) \right)_{\lambda=0} \xi_0
$$
$$
= -L(\pi)a.\xi_0.
$$

### 12. 伴随表示

令 G 为李群。考虑解析左运算的律
$$
(g, g') \mapsto gg'g^{-1} = (\operatorname{Int} g)g'
$$
这个运算定义的律，通过no. 3，$\mathscr{T}^{(\infty)}(G) \times \mathscr{T}^{(\infty)}(G)$到$\mathscr{T}^{(\infty)}(G)$的双线性映射，我们将在这个数中用$\tau$表示。截至命题 13 / no. 3，
$$
(t * t') \tau t'' = t \tau (t' \tau t'')
$$
对于$\mathscr{T}^{(\infty)}(G)$中的所有$t, t', t''$。截至命题 14 (i) / no. 3，
$$
\varepsilon_g \tau t = (\operatorname{Int} g)_*t
$$
对于所有 $g \in G$ 和 $t \in \mathscr{T}^{(\infty)}(G)$。特别是，$\mathscr{T}^{(\infty)}(G)$到$\mathscr{T}^{(\infty)}(G)$的映射$t \mapsto \varepsilon_g \tau t$是大数$\mathscr{T}^{(\infty)}(G)$的自同构。其限制至$U(G), U_s(G), L(G)$用$\operatorname{Ad}_{U(G)}(g), \operatorname{Ad}_{U_s(G)}(g), \operatorname{Ad}_{L(G)}(g)$表示。为了避免混淆，我们经常写 $\operatorname{Ad}(g)$ 而不是 $\operatorname{Ad}_{L(G)}(g)$。根据(23)，$\operatorname{Ad}(g)$是映射在e到$\operatorname{Int}(g)$的切线。正常的自同构

李代数$\mathbf{L}(G)$。当$K$的特征为0时，$\mathrm{Ad}_{\mathbf{U}(G)}(g)$是$\mathbf{U}(G)$唯一的自同构，即扩展$\mathrm{Ad}(g)$。

如果$\phi$是李群$G$到李群$H$的态射，那么
$$
\phi_*(t \top t') = \phi_*(t) \top \phi_*(t')
$$
对于 $\mathscr{T}^{(\infty)}(G)$ 中的所有 $t, t'$；这是从命题 15 of no. 3 得出的。

#### 命题 43 {#lie-iii-s3-prop-43 .statement tag=0ABC}

*让$t, u$位于$\mathscr{T}^{(\infty)}(G)$中。设$\sum_{i=1}^n t_i \otimes t'_i$为余积下$t$的像。然后*
$$
t \top u = \sum_{i=1}^n t_i * u * {t'_i}^\vee.
$$

到定义，$t \top u$是$G \times G$的映射$(g, g') \mapsto gg'g^{-1}$下的$t \otimes u$像变成$G$。现在这个映射是通过组合以下映射得到的：
$$
\begin{aligned}
\alpha & : (g, g') \mapsto (g, g, g') & \text{of } G \times G \text{ into } G \times G \times G \\
\beta & : (g, g', g'') \mapsto (g, {g'}^{-1}, g'') & \text{of } G \times G \times G \text{ into } G \times G \times G \\
\gamma & : (g, g', g'') \mapsto gg''g' & \text{of } G \times G \times G \text{ into } G.
\end{aligned}
$$

另一方面：
$$
\begin{aligned}
\alpha_*(t \otimes u) &= \sum_{i=1}^n (t_i \otimes t'_i) \otimes u = \sum_{i=1}^n t_i \otimes t'_i \otimes u \\
\beta_* \left( \sum_{i=1}^n t_i \otimes t'_i \otimes u \right) &= \sum_{i=1}^n t_i \otimes {t'_i}^\vee \otimes u \\
\gamma_* \left( \sum_{i=1}^n t_i \otimes {t'_i}^\vee \otimes u \right) &= \sum_{i=1}^n t_i * u * {t'_i}^\vee.
\end{aligned}
$$

#### 推论 1 {#lie-iii-s3-prop-43-cor-1 .statement tag=0ABD}

*设$u \in \mathbf{L}(G)$和$u' \in \mathscr{T}^{(\infty)}(G)$。然后$u \top u' = u * u' - u' * u$.*

余积下的$u$中的像是$u \otimes \varepsilon_e + \varepsilon_e \otimes u$、从而
$$
u \top u' = u * u' * \varepsilon_e + \varepsilon_e * u' * u^\vee = u * u' - u' * u.
$$

#### 推论 2 {#lie-iii-s3-prop-43-cor-2 .statement tag=0ABE}

*设$t \in \mathscr{T}^{(\infty)}(G)$和$g \in G$。然后$\varepsilon_g \top t = \varepsilon_g * t * \varepsilon_{g^{-1}}$。如果$t \in \mathbf{L}(G)$，则$\varepsilon_g \top t = gtg^{-1}$（其中后者乘积在群$\mathbf{T}(G)$中计算）。*

余积下的$\varepsilon_g$的像是$\varepsilon_g \otimes \varepsilon_g$。

#### 推论 3 {#lie-iii-s3-prop-43-cor-3 .statement tag=0ABF}

*设$a \in \mathbf{L}(G)$。 向量域由$a$定义，$G$在$G$上的左边运算$g \mapsto \mathrm{Int}\, g$是域$\mathbf{R}_a - \mathbf{L}_a$。*

这个域在$g$的值是
$$
\begin{aligned}
a \top \varepsilon_g &= a * \varepsilon_g - \varepsilon_g * a & \text{(Corollary 1)} \\
&= (\mathbf{R}_a)_g - (\mathbf{L}_a)_g & \text{(Definition 5)}.
\end{aligned}
$$

对于所有$g \in G$和所有$t \in L(G)$，
$$
(\mathrm{Ad}\,g)(t) = \varepsilon_g \top t = \varepsilon_g * t * \varepsilon_g^{-1} = gtg^{-1}.
$$
由于$\mathrm{Ad}\,g = T_e(\mathrm{Int}\,g)$，no. 11的命题 42证明$\mathrm{Ad}$是$G$在可范空间$L(G)$上的解析线性表示。

#### 定义 8 {#lie-iii-s3-def-8 .statement tag=0ABG}

*表示 G 在 L(G) 上的 Ad 称为 G 的伴随表示。*

#### 命题 44 {#lie-iii-s3-prop-44 .statement tag=0ABH}

*对于所有$a \in L(G)$，*
$$
(L(\mathrm{Ad}))(a) = \mathrm{ad}_{L(G)}a.
$$
让$b \in L(G)$。由 no. 11 的命题 42 (ii) 以及推论 3 至命题 43，
$$
(L(\mathrm{Ad}))(a).b = -[R_a - L_{a_1}L_b](e).
$$
现在$R_a \circ L_b = L_b \circ R_a$（no. 6、命题23（ii））、从而$[R_a, L_b] = 0$；然后，使用命题 23 (ii)，
$$
(L(\mathrm{Ad}))(a).b = [L_a, L_b](e) = L_{[a, b]}(e) = [a, b] = (\mathrm{ad}_{L(G)}a)b.
$$

#### 命题 45 {#lie-iii-s3-prop-45 .statement tag=0ABI}

*假设G是有限维的并且K的特征为0。令s为整数$\geqslant 0$。那么映射 $\pi : g \mapsto \mathrm{Ad}_{U_s(G)}(g)$ 是 G 在 $U_s(G)$ 和 $L(\pi)a = \mathrm{ad}_{U_s(G)}a$ 上对所有 $a \in L(G)$ 的解析线性表示。*

线性表示 $\pi$ 是 $\bigoplus_{r=0}^s \mathrm{Tr}(\mathrm{Ad})$ 的商，因此是解析的。对于$L(G)$中的$a \in L(G)$和$x_1, x_2, \ldots, x_s$，
$$
\begin{align*}
(L(\pi)a)(x_1x_2\ldots x_s) &= \sum_{i=1}^s x_1 \ldots (L(\mathrm{Ad})a.x_i) \ldots x_s & \text{(Proposition 41)} \\
&= \sum_{i=1}^s x_1 \ldots ([a, x_i]) \ldots x_s & \text{(Proposition 44)} \\
&= (\mathrm{Ad}_{U_s(G)}a)(x_1x_2\ldots x_s).
\end{align*}
$$

#### 命题 46 {#lie-iii-s3-prop-46 .statement tag=0ABJ}

*设$h \in G, x \in T_h(G)$和$a \in L(G)$。设 $\phi$ 为 $G \times G$ 的映射 $(g, g') \mapsto gg'g^{-1}$ 到 $G$。 $T_{(e, h)}(\phi)$下$(a, x) \in T_e(G) \times T_h(G)$的像y是$y = x + h((\mathrm{Ad}\,h^{-1})a - a)$。
我们有*
$$
\begin{align*}
y &= (T_{(e, h)}\phi)(a \otimes \varepsilon_h + \varepsilon_e \otimes x) \\
&= a \top \varepsilon_h + \varepsilon_e \top x \\
&= a * \varepsilon_h - \varepsilon_h * a + x \\
&= h((\mathrm{Ad}\,h^{-1})a) - ha + x.
\end{align*}
$$

#### 命题 47 {#lie-iii-s3-prop-47 .statement tag=0ABK}

设 G 为李群，H 和 E 为 G 的子群，并假设对于所有 h \in H，hEh$^{-1}$ = E。则$\mathscr{T}^{(\infty)}(H) \subset \mathscr{T}^{(\infty)}(E) \subset \mathscr{T}^{(\infty)}(E)$。特别是$\mathrm{Ad}(H)(L(E)) \subset L(E)$和$[L(H), L(E)] \subset L(E)$。

如果$t \in \mathscr{T}^{(\infty)}(H)$和$t' \in \mathscr{T}^{(\infty)}(E)$，则映射$(g, g') \mapsto gg'g^{-1}$下$H \times E$的$t \otimes t' \in \mathscr{T}^{(\infty)}(H \times E)$和像包含在E中。

#### 命题 48 {#lie-iii-s3-prop-48 .statement tag=0ABL}

设 G 为李群，H 和 E 位于 G 的子群。假设 G 是 H 通过 E 的半直乘积，如李群。设 $\varphi$ 为李群 G 在 $L(E)$ 上的线性表示 $g \mapsto (\mathrm{Ad}\, g) \mid L(E)$ (cf. 命题 47) 并设$\sigma$为$\varphi$到H的限制。则：
(i) $L(G)$是$L(H)$和$L(E)$的拓扑直和；
(ii) $L(H)$是$L(G)$的子代数，并且$L(E)$是$L(G)$的理想；
(iii) $L(\sigma)$为$L(E)$推导李代数上$L(H)$线性表示；
(iv) $L(G)$ 是由$L(\sigma)$ (章 I, § 1, no. 8) 定义的$L(E)$ 对$L(H)$ 的半直接乘积。

(i) 是显而易见的，并且 (ii) 由命题 47. $L(\sigma) = L(\varphi) \mid L(H)$ 得出。现在，通过命题 40 (no. 11) 和 44 (no. 12)，对于所有 $t \in L(G)$，$L(\varphi)(t)$ 是 $\mathrm{ad}_{L(G)} t$ 到 $L(E)$ 的限制。这就证明了(iii)。利用(i)和(ii)，这也证明了(iv)。

#### 推论{#lie-iii-s3-n12-cor-1 .statement tag=0ABM}

令 G 为李群。让 $T_e(G)$ 被赋予其唯一的交换律李代数结构。设$\tau$是$L(G)$的伴随表示。那么$T(G)$的李代数就是$\tau$定义的$T_e(G)$对$L(G)$的半直接乘积。在其他字中，对于$L(G)$中的$x, x'$和$T_e(G)$中的$y, y'$，

$$
[(x, y), (x', y')] = ([x, x'], [x, y'] + [y, x'])
$$

（其中左侧括号在 $L(T(G))$ 中计算，右侧括号在 $L(G)$ 中计算）。

这是从 § 2, no. 2 的命题 48 和命题 6 得出的。

#### 命题 49 {#lie-iii-s3-prop-49 .statement tag=0ABN}

设 A 是完全规范单位结合律代数。我们认同 A 与$L(A^*)$。那么，如果$g \in A^*$和$y \in A$，则$(\mathrm{Ad}\, g)y = gyg^{-1}$。

回想一下$\mathrm{Ad}\, g = T_1(\mathrm{Int}\, g)$。令$u_g$为A到A的映射$x \mapsto gxg^{-1}$。$A^*$到变换$\mathrm{Int}\, g$到$u_g \mid A^*$的恒等图。 $A^*$的每个点与此映射的切线映射等于$u_g$、从而命题。

#### 推论{#lie-iii-s3-n12-cor-2 .statement tag=0ABO}

对于所有 $g \in A^*$，令 $i(g)$ 为 A 的自同构 $y \mapsto gyg^{-1}$，因此 $i$ 是 A 上 $A^*$ 的解析线性表示。对于所有 $z \in L(A^*) = A, L(i)z$ 为内部推导 A 的$y \mapsto zy - yz$。

这是从命题 49 和 44 得出的。

### 13. 张量和不变形式

令 G 为李群。我们认为 G 通过左（或右）平移对其自身进行操作。令$\lambda$为同构的类$C^\omega$的向量函子。那么 $\lambda(\mathrm{TG})$ 是解析左（或右）向量 G 丛（§ 1, no. 8，命题 16 的推论）。 $G \times \lambda(\mathrm{L}(G))$到$\lambda(\mathrm{TG})$的映射$(g, u) \mapsto gu$（分别$ug$）是向量G束（§ 7, no. 8）的同构$\phi$（分别$\psi$），推论2到命题17)。 $\lambda(\mathrm{TG})$ 的每个 G 不变量截面都是解析的，并由其在 $e$ 处的值确定（§ 1, no. 8，推论 1 到命题 17）。这样的截面被称为*左*（或*右*）*不变*。令$\sigma$为$\lambda(\mathrm{TG})$的左不变量截面； $\sigma$的变换$\sigma'$在正确翻译$\delta(g)$下由$\sigma'(\delta(g)h) = \lambda(\mathrm{T}_h(\delta(g)))\sigma(h)$定义为所有$h \in G$；它也是保持不变的；它也是从 $\sigma$ 到 $\gamma(g) \circ \delta(g) = \mathrm{Int}(g)$ 衍生而来，因此

$$
\sigma'(e) = \lambda(\mathrm{Ad}\ g)\cdot \sigma(e).
$$

类似地，令$\tau$为$\lambda(\mathrm{TG})$的右不变量截面；左翻译 $\gamma(g)$ 下的 $\tau$ 变换 $\tau'$ 也是右变体并且

$$
\tau'(e) = \lambda(\mathrm{Ad}\ g)\cdot \tau(e).
$$

现在，我们将 $G \times G$ 视为在左侧的 $G$ 上进行操作

$$
((g, g'), g'') \mapsto gg''{g'}^{-1}.
$$

那么 G 是 $G \times G$ (§ 1, no. 6, *例*) 的左李齐次空间。因此$\lambda(\mathrm{TG})$是解析左向量$(G \times G)$丛。如果$\lambda(\mathrm{TG})$的截面在$\lambda(\mathrm{TG})$上的$G \times G$的作用下是不变的，则称为*双不变*，在其他字中，如果它在左右平移下是不变的。设$\lambda(\mathrm{L}(G))_0$为$\lambda(\mathrm{L}(G))$元素集合在$\lambda(\mathrm{Ad}(G))$下不变。对于所有$u \in \lambda(\mathrm{L}(G))_0$，令$\sigma_u$为$G$的映射进入由$\sigma_u(g) = gu = ug$定义的$\lambda(\mathrm{TG})$。那么$u \mapsto \sigma_u$是$\lambda(\mathrm{L}(G))_0$的双射到$\lambda(\mathrm{TG})$的双不变截面的集合（§ 1, no. 8，推论1到命题17）。

#### 命题 50 {#lie-iii-s3-prop-50 .statement tag=0ABP}

*设 G 为李群（如果 K 的特征 > 0，则假定为有限维）。 令E为$\mathrm{T}_e(G)$上次数 k 的连续交替多重线性形式的向量空间。 对于所有$u \in E$，令$\omega^u$为G上次数k的微分形式，使得$(\omega^u)_g$是$\mathrm{T}_g(G)$上的多重线性形式，通过平移$h \mapsto gh$（或$h \mapsto hg$）从u导出。 那么 $\omega^u$ 在 G 上是解析的且左（或右）不变的。 映射 $u \mapsto \omega^u$ 是 E 的同构到 G 上次数 k 的左（或右）不变微分形式的向量空间。*

这是我们上面所说的一个特例。

设 F 是完全可范空间。如果 G 上的微分形式和 K 中的值被 G 上的微分形式和 F 中的值替换，命题 50 仍然为真。 对于 F 中 $\mathrm{T}_e(G)$ 的每个连续线性映射 $u$，都存在一个微分形式 G 上次数 1 的 $\omega^u$，F 上有值，使得 $(\omega^u)_g = u \circ \mathrm{T}_g(\gamma(g)^{-1})$。特别是取$F = \mathrm{T}_e(G)$和$u = \mathrm{Id}_{\mathrm{T}_e(G)}$。然后我们获得$G$上的微分形式$\omega$，使得$\omega_g = T_g(\gamma(g^{-1}))$；这个微分形式是左不变的和解析的；它被称为$G$的*左规范微分形式*。 $\omega_g(t) = g^{-1}t$ 对于所有$t \in T_g(G)$。

如果 $F$ 又是任意完全范数空间和 $u \in \mathscr{L}(T_e(G), F)$，则 $\omega^u = u \circ \omega$。特别是（取$F = K$），映射$v \mapsto v \circ \omega$是$T_e(G)$的对偶到向量空间的线性双射，次数1的微分形式与$K$中的值保持不变$G$以下。

类似地，$G$上的微分形式$\omega'$使得$\omega'_g = T_g(\delta(g))$被称为$G$的*右规范微分形式*。 $\omega$ 也有类似的性质，我们留给读者来说明。将$G$的映射$g \mapsto g^{-1}$转换为$G$变换$\omega$转换为$\omega'$。

### 14.毛雷尔-嘉当公式

如果$K$具有特征$> 0$，则令$X$为类、$C^r$的流形、有限维，并令$L$为完全规范的李代数。令$\alpha$为$X$上次数1的微分形式与类$C^{r-1}$的$L$中的值。让$x \in X$。 映射

$$
(u_1, u_2) \mapsto [\alpha_x(u_1), \alpha_x(u_2)]
$$

$T_x(X) \times T_x(X)$到$L$是$T_x(X)$上的连续交错的双线性形式，$L$中有值。我们用$[\alpha]^2_x$来表示它，因此$[\alpha]^2$是$X$上的次数2与$L$上的值的微分形式。识别$X$中$x$的开邻域与Banach空间的开子集，我们立即发现$[\alpha]^2$是类$C^{r-1}$。如果$X'$是类$C^r$中的流形并且$f : X' \to X$是态射，那么

$$
[f^*(\alpha)]^2 = f([\alpha]^2).
$$

令$\alpha, \beta$为$X$上次数1的二微分形式与类$C^{r-1}$的$L$中的值。 $\alpha$ 和 $\beta$ 的外部乘积 $\alpha \wedge \beta$（*可微分和解析流形*，R，7.8.2）是 $X$ 上次数 2 的微分形式与值 $L$ 类 $C^{r-1}$；我们有

$$
(\alpha \wedge \beta)_x(u_1, u_2) = [\alpha_x(u_1), \beta_x(u_2)] - [\alpha_x(u_2), \beta_x(u_1)]
$$

对于 $T_x(X)$ 中的 $u_1, u_2$。就是直接的

$$
[\alpha + \beta]^2 = [\alpha]^2 + [\beta]^2 + \alpha \wedge \beta
$$
$$
\alpha \wedge \alpha = 2[\alpha]^2.
$$

#### 命题 51 {#lie-iii-s3-prop-51 .statement tag=0ABQ}

*如果$K$具有特征$> 0$，则令$G$为有限维的李群，并令$a_1, \ldots, a_p$为$L(G)$的元素，$F$为完全规范的空间，并且$\alpha$ $G$ 上次数 $p-1$ 的形式与$F$ 上值的差值。如果 $\alpha$ 保持不变，则*

$$
(d\alpha)_e(a_1, \ldots, a_p) = \sum_{i<j} (-1)^{i+j} \alpha_e([a_i, a_j], a_1, \ldots, a_{i-1}, a_{i+1}, \ldots, a_{j-1}, a_{j+1}, \ldots, a_p).
$$

如果 $\alpha$ 是右不变量，那么
$$
(d\alpha)_e(a_1, \ldots, a_p)
= - \sum_{i < j} (-1)^{i+j} \alpha_e([a_i, a_j], a_1, \ldots, a_{i-1}, a_{i+1}, \ldots, a_{j-1}, a_{j+1}, \ldots, a_p).
$$
假设 $\alpha$ 保持不变。由 *可微分和解析流形*, R, 8.5.7, 则
$$
(d\alpha)(L_{a_1}, \ldots, L_{a_p}) = \sum_i (-1)^{i-1} L_{a_i} \alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p})
+ \sum_{i < j} (-1)^{i+j} \alpha([L_{a_i}, L_{a_j}], L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_{j-1}}, L_{a_{j+1}}, \ldots, L_{a_p}).
$$
但是 G 上的函数 $\alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p})$ 保持不变，因此是常数。因此
$$
L_{a_i} \alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p}) = 0.
$$
此外，$[L_{a_i}, L_{a_j}] = L_{[a_i, a_j]}$ (命题 23)、从而命题 51 中的第一个公式。第二个可以类似地建立，这次使用关系 $[R_{a_i}, R_{a_j}] = -R_{[a_i, a_j]}$。

#### 推论 1 {#lie-iii-s3-prop-51-cor-1 .statement tag=0ABR}

*如果K的特征> 0，则令G为有限维的李群，并且$\omega$和$\omega'$为G的左右规范微分形式。则*
$$
d\omega + [\omega]^2 = 0, \qquad d\omega' - [\omega']^2 = 0.
$$
到命题51，
$$
(d\omega)_e(a_1, a_2) = -\omega_e([a_1, a_2]) = -[a_1, a_2] = -[\omega_e(a_1), \omega_e(a_2)]
= -[\omega]^2_e(a_1, a_2)
$$
从而第一个公式。第二个可以类似地建立。

#### 推论 2 {#lie-iii-s3-prop-51-cor-2 .statement tag=0ABS}

*假设 G 是有限维的。令$(e_1, \ldots, e_n)$为$L(G)$、$(e_1^*, \ldots, e_n^*)$对偶基、$(c_{ijk})$的基、$L(G)$的结构相对于基、$(e_1, \ldots, e_n)$和$\omega_i$的常数（分别为： $\omega'_i$) G 上的左（或右）不变微分形式与 K 中的值，使得$(\omega_i)_e = e_i^*$（或$(\omega'_i)_e = e_i^*$）。然后*
$$
d\omega_k + \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j = 0 \quad (k = 1, 2, \ldots, n)
$$
$$
d\omega'_k - \sum_{i < j} c_{ijk} \omega'_i \wedge \omega'_j = 0 \quad (k = 1, 2, \ldots, n).
$$
如果$r < s$，
$$
(d\omega_k)_e(e_r, e_s) = -(\omega_k)_e([e_r, e_s])
= -\sum_i c_{rsi} (\omega_k)_e(e_i)
= -c_{rsk}
= -\sum_{i < j} c_{ijk} (\omega_i \wedge \omega_j)_e(e_r, e_s).
$$
$\omega'_k$ 的论证类似。

### 15. 不变微分形式的构造

#### 引理 2 {#lie-iii-s3-lem-2 .statement tag=0ABT}

设G为李群，U为G中e的对称开邻域，E为完全规范空间，$\phi : U^2 \to E$为解析映射。对于所有$g \in U$，令$\omega_g$为映射$h \mapsto \phi(g^{-1}h)$在点g处的微分。那么$\omega$对于G上的左不变微分形式的U来说是限制，其在e处的值是$d_e \phi$。

显然$\omega_e = d_e \phi$。对于所有$g \in U$和所有$t \in T_e(G)$，

$$
\langle \omega_g, T_e(\gamma(g))t \rangle = \langle d_g(\phi \circ \gamma(g)^{-1}), T_e(\gamma(g))t \rangle \\
= \langle d_e \phi \circ T_g(\gamma(g)^{-1}), T_e(\gamma(g))t \rangle = \langle d_e \phi, t \rangle
$$

因此 $\omega_g$ 是由 $d_e \phi$ 通过 $T_e(\gamma(g))$ 衍生而来。

#### 命题 52 {#lie-iii-s3-prop-52 .statement tag=0ABU}

令 n 为整数 > 0，G 为 n 维李群，U 为 G 中 e 的对称开邻域，$\psi : U^2 \to K^n$ 为 G 的图，使得 $\psi(e) = 0$。如果$(x_1, \ldots, x_n)$是$x \in \psi(U)$的坐标，$(y_1, \ldots, y_n)$是$y \in \psi(U)$的坐标，我们表示为

$$
m_1(x_1, \ldots, x_n, y_1, \ldots, y_n), \ldots, m_n(x_1, \ldots, x_n, y_1, \ldots, y_n)
$$

$\psi(\psi^{-1}(x)^{-1}\psi^{-1}(y))$的坐标。那么，如果我们写，对于 $1 \leq k \leq n$，

$$
\varpi_k(x_1, \ldots, x_n) = D_{n+1} m_k(x_1, \ldots, x_n, x_1, \ldots, x_n) dx_1 + \cdots \\
+ D_{2n} m_k(x_1, \ldots, x_n, x_1, \ldots, x_n) dx_n,
$$

$\psi(U)$上的微分形式$\varpi_k$是通过$\psi$从G上的左不变微分形式导出的，并且使得$\varpi_k(0, \ldots, 0) = dx_k$。

我们将引理 2 与$E = K$ 相乘，将$\phi(g)$ 作为指标 k 的$\psi(g)$ 的坐标。我们得到微分形式 $\omega_k$；设$\varpi_k$为$\psi$下的变换。 $(x_1, \ldots, x_n)$处$\varpi_k$的值是函数$y \mapsto m_k(x_1, \ldots, x_n, y_1, \ldots, y_n)$在$(x_1, \ldots, x_n)$的微分；因此，这个值由公式 (32) 给出。然后使用引理 2 的结论就足够了。

#### 命题 53 {#lie-iii-s3-prop-53 .statement tag=0ABV}

设G为李群，A为G的完全可规范代数和$\phi$李群态射为$A^*$。对于所有$g \in G$，令$\omega_g = \phi(g)^{-1} d_g \phi$。那么$\omega$是G上的左不变微分形式，其在e处的值是$d_e \phi$。

我们将引理 2 与$E = A$ 和$U = G$ 一起应用。 映射 $h \mapsto \phi(g^{-1}h) = \phi(g)^{-1} \phi(h)$ 处的 g 差为 $\phi(g)^{-1} d_g \phi$。

### 16.HAAR 测量李群

令 G 为有限维 n 的李群。则 $\bigwedge^n(T_e(G))$ 为维数 1。因此，G 上次数 n 的左不变微分形式的 (no. 13) 向量空间 S 为维数 1。令 $(\omega_1, \ldots, \omega_n)$ 为空间的基 G 上次数 1 的左不变微分形式；那么 $\omega_1 \wedge \omega_2 \wedge \cdots \wedge \omega_n$ 就是 S 的基。

#### 命题 54 {#lie-iii-s3-prop-54 .statement tag=0ABW}

令 G 为有限维 n 的李群，ω 为 G 上次数 n 的左不变微分形式和 G 的 φ 自同态。则

$$
\phi^*(\omega) = (\det L(\phi)) \omega.
$$

我们写 $L(\phi) = u$、$\omega_e = f$ 和 $\phi^*(\omega)_e = g$。对于 $L(G)$ 中的所有 $x_1, \ldots, x_n$，

$$
g(x_1, \ldots, x_n) = f(ux_1, \ldots, ux_n) = (\det u)f(x_1, \ldots, x_n)
$$

因此$\phi^*(\omega)_e = \det L(\phi) \cdot \omega_e$。另一方面，如果$g \in G$，

$$
\phi \circ \gamma(g) = \gamma(\phi(g)) \circ \phi
$$

因此$\gamma(g)^*\phi^*(\omega) = \phi^*(\omega)$。因此$\phi^*(\omega)$保持不变，从而命题。

#### 推论{#lie-iii-s3-n16-cor-1 .statement tag=0ABX}

对于所有$g \in G$，

$$
\delta(g)^*\omega = (\det \mathrm{Ad}\, g) \omega.
$$

$$
\delta(g)^*\omega = \delta(g)^*\gamma(g)^*\omega = (\mathrm{Int}\, g)^*\omega \text{ and } L(\mathrm{Int}\, g) = \mathrm{Ad}\, g.
$$

设G是G的局部紧致群和φ自同态。假设存在e的开邻域V、$V'$，使得$\phi(V) = V'$和$\phi|V$是G到G的局部同构。令μ为G上的左Haar测度。通过积分， 章 VII, § 1，推论命题 9，存在唯一的数 $a > 0$，使得$\phi(\mu|V) = a^{-1}\mu|V'$。显然 a 独立于 V、$V'$ 和 μ 中的选择。它称为 φ 的模数，用 $\mathrm{mod}_G \phi$ 或简称为 $\mathrm{mod}\, \phi$ 表示。当 φ 是 G 的自同构时，我们恢复积分的定义 4，章 VII, § 1。

#### 命题 55 {#lie-iii-s3-prop-55 .statement tag=0ABY}

假设 K 是局部紧致的。令 μ 为 K 的加法群上的 Haar 测度。令 G 为有限维 n 的李群。

(i) 令 ω 为 G 上次数 n 的非零左不变微分形式。则测度 $\mathrm{mod}(\omega)_\mu$（可微且解析流形, R, 10.1.6）是 G 上的左 Haar 测度。如果 $K = \mathbf{R}$ 且 G 具有由 ω 定义的方向，则测度由 ω（可微且解析流形, R, 10.1.6）定义。解析流形, R, 10.4.3) 是 G 上的左 Haar 测度。

(ii) 令 φ 为 G 的 etale 自同态。然后为 $\mathrm{mod}\, \phi = \mathrm{mod}\, \det L(\phi)$。

(i) 是显而易见的。令V、$V'$为e的开邻域，使得$\phi(V) = V'$和$\phi|V$是G到G的局部同构。则

$$
\phi^{-1}(\mathrm{mod}(\omega)_\mu|V') = \mathrm{mod}(\phi^*(\omega))_\mu|V) \quad \text{by transport of structure}
$$
$$
= \mathrm{mod}(\det L(\phi)\omega|V)_\mu \quad \text{(Proposition 54)}
$$
$$
= \mathrm{mod}\, \det L(\phi)(\mathrm{mod}(\omega)_\mu|V)
$$

从而$\mathrm{mod}\, \phi = \mathrm{mod}\, \det L(\phi)$乘定义共$\mathrm{mod}\, \phi$。

#### 推论{#lie-iii-s3-n16-cor-2 .statement tag=0ABZ}

对于所有$g \in G$，$\Delta_G(g) = (\operatorname{mod} \det \operatorname{Ad} g)^{-1}$。 In particular, for $G$ to be unimodular, it is necessary and sufficient that $\operatorname{mod} \det \operatorname{Ad} g = 1$ for all $g \in G$.

$$
\Delta_G(g) = (\operatorname{mod} \operatorname{Int} g)^{-1} \quad \text{(Integration, Chapter VII, § 1, formula (33))}
= (\operatorname{mod} \det L(\operatorname{Int} g))^{-1} \quad \text{(Proposition 55)}
= (\operatorname{mod} \det \operatorname{Ad} g)^{-1}.
$$

#### 注 {#lie-iii-s3-n16-rem-1 .statement tag=0AC0}

保留命题 52 的假设和记号，假设 $K$ 是局部紧致的。设 $\mu$ 为度量
$$
\operatorname{mod} \det(D_{n+i}m_k(x_1, \ldots, x_n, x_1, \ldots, x_n))_{1 \leq i, k \leq n} dx_1 \ldots dx_n
$$
在$\psi(U)$。那么$\psi^{-1}(\mu)$是$G$上哈尔测度的限制到$U$。

#### 命题 56 {#lie-iii-s3-prop-56 .statement tag=0AC1}

令$G$为有限维$n$的李群，$H$一个$p$维李子群和$X$李齐次空间$G/H$。假设
$$
\det \operatorname{Ad}_{L(G)} h = \det \operatorname{Ad}_{L(H)} h
$$
对于所有$h \in H$。然后：
(i) 次数 $n - p$在$X$上的微分形式在$G$下不变，是解析的。
(ii) 这些形式中的向量空间是维数 1。
(iii) 如果$\omega$是这样一个非零形式并且$K$是局部紧致的，$\operatorname{mod}(\omega)_\mu$是$X$上的非零测度，它在$G$下是不变的。

由 § 1, no. 8、例、$\operatorname{Alt}^{n-p}(TX, K)$ 是解析的向量 $G$ 丛。令$x_0$为$X$中$e$的典范像；它的稳定子是$H$。 $\operatorname{Alt}^{n-p}(TX, K)$在$x_0$处的纤维是$\bigwedge^{n-p} T_{x_0}(X)^*$，$T_{x_0}(X)$被规范地识别为$L(G)/L(H)$。如果$h \in H$，$h$定义的$X$的自同构$\tau_h$是在经过与$G$的自同构$g \mapsto hgh^{-1}$的商导出的。因此，当经过与 $\operatorname{Ad}_{L(G)}(h)$ 的商时，可得出自同构 $T_{x_0}(\tau_h)$。作为
$$
\det \operatorname{Ad}_{L(G)} h = (\det \operatorname{Ad}_{L(H)} h) \cdot (\det T_{x_0}(\tau_h)),
$$
假设意味着$\det T_{x_0}(h) = 1$。因此，$\bigwedge^{n-p} T_{x_0}(X)^*$的每个元素在$H$下都是不变的。那么(i)和(ii)从§ 1, no. 8，推论1到命题17，(iii)是显而易见的。

$G$ 下$X$ 不变量存在非零正测度，可从积分章 VII, § 2，推论 2 到定理 3 得出，对于命题 56 的假设意味着 $\Delta_G|H = \Delta_H$（推论命题55）。

#### 命题 57 {#lie-iii-s3-prop-57 .statement tag=0AC2}

设$G$为有限维$n$中的李群。 选择基 $\bigwedge^n T_e(G)^*$；通过$\bigwedge^n T(G)^*$的右（或左）平凡化，我们用平凡的向量丛$G \times K$来可以确定这个向量丛，这样标量微分算子的转置就可以用标量微分算子来标识。

那么，如果$u \in U(G)$，$L_u$（或$R_u$）的转置是$L_u^\nu$（或$R_u^\nu$）。

我们将考虑使用右不变量形式 $\omega$ 来简化 $\Lambda^n T(G)^*$ 的情况。

假设命题已被证明适用于$U(G)$的元素$u_1, u_2$。然后，

$$
\begin{align*}
t(L_{u_1 * u_2}) &= t(L_{u_1} \circ L_{u_2}) & \text{(Proposition 23)} \\
&= t(L_{u_2}) \circ t(L_{u_1}) & \text{(\emph{Diff. \& Anal. Man.}, R, 14.3.3)} \\
&= L_{u_2}^\nu \circ L_{u_1}^\nu & \text{by hypothesis} \\
&= L_{u_2 * u_1}^{\nu \nu} & \text{(Proposition 23)} \\
&= L_{(u_1 * u_2)^\nu} & \text{(Proposition 7)}
\end{align*}
$$

因此命题对于 $u_1 * u_2$ 是正确的。因此，当$u \in T_e(G)$时，证明命题就足够了。现在$L_u$是由$G$在右侧（no. 6）操作$G$定义的，因此$\theta_{L_u} \omega = 0$是因为$\omega$是右不变的（\emph{可微分和解析流形}，R，8.4.5）；因此，如果 $f$ 是 $e$ 的开邻域中的解析函数，且 $K$ 中有值，则 $\theta_{L_u}(f \omega) = (\theta_{L_u} f) \omega$ (\emph{可微分且解析流形}, R, 8.4.8)。利用所做的辨识和\emph{可微分解析流形}，$L_u$的R，14.4.1，转置是$-L_u$，即$L_u^\nu$。

#### 推论{#lie-iii-s3-n16-cor-3 .statement tag=0AC3}

令 $G$ 为有限维实李群，$\mu$（分别为 $\nu$）为 $G$、$k$ 整数 $\geqslant 0$、$u \in U_k(G)$ 和 $f$ 的左（或右）Haar 测度，并且$G$ 上的类 $C^k$ 的$g$ 实值函数具有紧凑的支持。然后

$$
\int_G (R_u f) g \, d\mu = \int_G f (R_u^\nu g) \, d\mu
$$
$$
\int_G (L_u f) g \, d\nu = \int_G f (L_u^\nu g) \, d\nu.
$$

这是从命题 57 和 \emph{可微分和解析流形}, R, 14.3.8 得出的。

### 17. 左差速器

#### 定义 9 {#lie-iii-s3-def-9 .statement tag=0AC4}

设$G$为李群，类$C^r$的$M$流形以及$M$的类$C^r$的$f$映射入$G$。 $f$ 的左（或右）微分是 $M$ 上次数 1 的微分形式与 $L(G)$ 中的值的微分形式，它与每个向量 $u \in T_m(M)$ 元素 $f(m)^{-1} \cdot (T_m f)(u)$（或元素）相关联。 $(T_m f)(u) \cdot f(m)^{-1}$）。

在这个章中，我们将只考虑左微分，我们将其表示为$f^{-1}.df$，并将将结果转换为右微分的任务留给读者。

如果$f$是$G$的恒等映射，则$f^{-1}.df$是$G$的规范左微分形式$\omega$。回到定义 8 的一般情况，

$$
(f^{-1}.df)_m = \omega_{f(m)} \circ T_m(f)
$$

因此$f^{-1}.df = f^*(\omega)$。这意味着 $f^{-1}.df$ 是类 $C^{r-1}$。

#### 例 {#lie-iii-s3-n17-exa-1 .statement tag=0AC5}

(1) 如果 $G$ 是完全可规范空间的加法群，并且 $T_0(E)$ 与 $E$ 规范地一致，则 $f^{-1}.df$ 是微分和解析流形, R, 8.2.2 中定义的微分 $df$。

(2) 假设$G$ 是乘法群 $A^*$ 与完全可规范代数 $A$ 相关联。 Then $f$ can be considered as a mapping of $M$ into $A$ and hence the differential $df$ in the sense of Differentiable and Analytic Manifolds, R, 8.2.2 is defined and the product $f^{-1}df$ in the sense of Differentiable and Analytic Manifolds, R, 8.3.2 is defined. 显然，后者形式与$f$的左微分相同。

#### 命题 58 {#lie-iii-s3-prop-58 .statement tag=0AC6}

设$G$和$H$为两个李群、类$C^r$$M$流形、$M$类$C^r$$f$映射》将$G$的$G$和$h$态射转换为$H$。然后

$$
(h \circ f)^{-1}.d(h \circ f) = L(h) \circ (f^{-1}.df) = (h^{-1}.dh) \circ T(f).
$$

对于所有$x \in M$和$u \in T_x(M)$，

$$
(h \circ f)^{-1}.d(h \circ f)(u) = ((h \circ f)(x))^{-1}.T(h \circ f)(u).
$$

一方面，后一个表达式等于

$$
T(h)(f(x)^{-1}.T(f)(u)) \quad (§ 2, \text{Proposition 5})
$$
$$
= T_e(h)((f^{-1}.df)(u))
$$

另一方面，

$$
h(f(x))^{-1}T(h)(T(f)u)
$$
$$
= (h^{-1}.dh)(T(f)u).
$$

#### 命题 59 {#lie-iii-s3-prop-59 .statement tag=0AC7}

令$G$为李群、类$C^r$、$f$、$M$流形以及$M$的类$C^r$$g$映射代入$TM$ 的$G$ 和$p$ 典范满射到$M$。

（一）$(fg)^{-1}.d(fg) = (\mathrm{Ad} \circ g \circ p)^{-1} \circ (f^{-1}.df) + g^{-1}.dg.$

(ii) 为所有 $m \in M$ 写 $h(m) = f(m)^{-1}$，

$$
h^{-1}.dh = -(\mathrm{Ad} \circ f \circ p) \circ (f^{-1}.df).
$$

断言 (i) 从§ 2, no. 2、命题 7 得出。断言 (ii) 从 (i) 得出$g = h$。

#### 推论 1 {#lie-iii-s3-prop-59-cor-1 .statement tag=0AC8}

设$s \in G$和$sg$为$M$的映射$x \mapsto sg(x)$到$G$。然后

$$
(sg)^{-1}.d(sg) = g^{-1}.dg.
$$

这是从命题 59 (i) 将$f$作为$M$的常数映射$x \mapsto s$到$G$得出。

#### 推论 2 {#lie-iii-s3-prop-59-cor-2 .statement tag=0AC9}

*如果$M$到$G$的映射$f$和$g$具有相同的左微分，则映射到$fg^{-1}$的切线处处都是零。如果进一步 $K$ 的特征为 0，则 $fg^{-1}$ 是局部常数。*

到命题59，

$$
(fg^{-1})^{-1} \cdot d(fg^{-1}) = (\mathrm{Ad} \circ g \circ p) \circ (f^{-1}.df) - (\mathrm{Ad} \circ g \circ p) \circ (g^{-1}.dg).
$$

如果$f^{-1}.df = g^{-1}.dg$，则$(fg^{-1})^{-1} \cdot d(fg^{-1}) = 0$，即所有$x \in M$的$T_x(fg^{-1}) = 0$。这就证明了第一个断言。第二个是*可微分和解析流形*，R，5.5.3。

#### 命题 60 {#lie-iii-s3-prop-60 .statement tag=0ACA}

*如果$K$的特征> 0，则令$G$为有限维的李群，类$C^r$的$M$流形，类的$f$映射将$M$的$C^r$分解为$G$和$\alpha$$f$的左微分。然后$d\alpha + [\alpha]^2 = 0$.*

令 $\omega$ 为 $G$ 的规范左微分形式。使用推论 1 到命题 51, no. 14，我们有

$$
d\alpha = d(f^*(\omega)) = f^*(d\omega) = f^*(-[\omega]^2)
= -[f^*(\omega)]^2 = -[\alpha]^2.
$$

### 18. 李代数李群胚芽

在这个没有。 $(G, e, \theta, m)$表示李群胚芽。 § 的大部分结果部分对于相同的证明仍然成立。我们将回顾那些我们认为有用的内容。

18.1。令$\Omega$为$m$的定义中的集合。让$(g, g') \in \Omega,\ t \in T_e^{(\infty)}(G),\ t' \in T_{g'}^{(\infty)}(G)$。如no. 1，$t$和$t'$的卷积乘积，用$t * t'$表示，是$t \otimes t'$在$m$下的像。我们写$U(G) = T_e^{(\infty)}(G),\ U_s(G) = T_e^{(s)}(G),\ U^+(G) = T_e^{(\infty)+}(G),\ U_s^+(G) = T_e^{(s)+}(G)$。对于$U(G)$中的$t, t'$，定义$t * t'$以及属于至$U(G)$。通过卷积乘积，$U(G)$是代数与单位元$\varepsilon_e$的关联，并由$U_s(G)$过滤。 $U(G)$ 到$TS(T_e(G))$ 的典范同构 $i_{G,e}$ 是代数同构。

18.2.设$G, H$为李群细菌，$\phi : G \to H$态射。如果$\phi_*$下的$t$$t \in U(G)$、像$U(\phi)(t)$为$U(H)$元素且$U(\phi)$为代数为代数$U(G)$态射 $U(H)$。将$G$的映射$\theta : x \mapsto x^{-1}$转换为$G$定义映射$t \mapsto t^\vee$将$U(G)$转换为$U(G)$。对于$U(G)$中的$t, t'$，相对于$G^\vee$评估的乘积$t * t'$等于相对于$G$和$(t * t')^\vee = {t'}^\vee * t^\vee$评估的乘积$t' * t$。然后$U(\phi)(t^\vee) = (U(\phi)t)^\vee$。如果$G_1, \ldots, G_n$是李群细菌并且$G = G_1 \times \cdots \times G_n$，则$U(G_1) \otimes \cdots \otimes U(G_n)$到$U(G)$的典范同构是代数同构；

$U(G)$、$(t_1 \otimes \cdots \otimes t_n)^{\vee} = t_1^{\vee} \otimes \cdots \otimes t_n^{\vee}$ 中的$t_1, \ldots, t_n$。设$H$是$G$和$i : H \to G$典范嵌入的谎言子群胚芽。那么$U(i)$就是代数$U(H)$的单同态变成$U(G)$并且
$$
U(i)(t^{\vee}) = (U(i)(t))^{\vee}
$$
对于所有$t \in U(H)$。通过$G$上流形结构定义的卷积乘积和余积，$U(G)$是一个大数，$U(\phi)$是一个大数态射。

18.3。设$G$为李群胚芽，类$C^r$$X$流形和$G$类$C^r$左运算块$\psi$律 $X$。令$\Omega$为$\psi$的定义中的集合。如果$t \in T^{(s)}_g(G)$、$u \in T^{(s')}_x(X)$、$(g, x) \in \Omega$和$s + s' \leq r$，令$t * u$表示$\psi_*$下$t \otimes u$的像。设$t \in T^{(s)}_g(G)$，$t' \in T^{(s')}_x(G)$，$u \in T^{(s'')}_x(X)$；如果定义了$s + s' + s'' \leq r$和$gg'$、$(gg')x$、$g'x$、$g(g'x)$，则
$$
(t * t') * u = t * (t' * u).
$$
设$x_0 \in X$和$\rho(x_0)$为映射$g \mapsto gx_0$，它是在$e$的开邻域中定义的。如果$t \in U_r(G)$，则$\rho(x_0)_*t = t * \varepsilon_{x_0}$。在这里以及本篇的其余部分，我们将把翻译右运算的律块的结果的任务留给读者。

18.4。保留 18.3 的记号，令 $t \in U_s(G)$ 与 $s \leq r$。令 $f$ 为类 $C^r$ 在 $X$ 上的函数，其中值在 Hausdorff 多范数空间中。让 $t * f$ 表示 $X$ 上的函数定义为
$$
\begin{align*}
(t * f)(x) &= \langle t, g \mapsto f(\psi(\theta(g), x)) \rangle \\
&= \langle t^{\vee}, f \circ \rho(x) \rangle = \langle \rho(x)_*(t^{\vee}), f \rangle = \langle t^{\vee} * \varepsilon_x, f \rangle.
\end{align*}
$$
如果$t \in U_s(G)$、$t' \in U_{s'}(G)$和$s + s' \leq r$，则$\langle t', t * f \rangle = \langle t^{\vee} * t', f \rangle$和$(t * t') * f = t * (t' * f)$。令$t \in U_s(G)$、$f$和$f'$为$X$上类$C^r$的函数，其中值在Hausdorff多范数空间$F, F'$和$(u, u') \mapsto u.u'$为将$F \times F'$的连续双线性映射转换为豪斯多夫多范数空间；让
$$
\sum_{i=1}^n t_i \otimes t'_i
$$
是余积下$t$的像；如果$s \leq r$，那么
$$
t * (ff') = \sum_{i=1}^n (t_i * f)(t'_i * f').
$$

18.5。保留 18.3 的记号，令 $t \in U_s(G)$ 与 $s \leq r$。 映射 $x \mapsto t * \varepsilon_x$ 称为 $t$ 和律运算块定义的点分布的域，并且有时由 $D_t^{\psi}$ 或 $D_t$ 表示。如果$f : X \to F$是类$C^r$中的函数，则$X$上的函数$t^{\vee} * f$也表示为$D_t f$；如果$s < \infty$，则为类$C^{r-s}$。如果$t \in U_s(G)$、$t' \in U_{s'}(G)$和$s + s' \leq r$，则$D_{t*t'} f = D_{t'}(D_t f)$。如果$G$和$X$是有限维的，则$D_t$是阶$\leq s$和类$C^{r-s}$的$X$上的微分算子（如果$s < \infty$）。那么在这个微分算子下，函数$D_t f$就是$f$的变换。

18.6。令 G 为李群胚芽和$t \in U(G)$。 $L_t$ 表示 G 上点分布 $g \mapsto \varepsilon_g * t$ 的域和 G 上点分布 $g \mapsto t * \varepsilon_g$ 的 $R_t$ 域。如果 $f \in C^\omega(G, F)$，则 $L_t f \in C^\omega(G, F)$ 和$R_t f \in C^\omega(G, F)$。对于 $U(G)$、$L_{t \circ t'} = L_t \circ L_{t'}$、$R_{t \circ t'} = R_{t'} \circ R_t$、$L_t \circ R_{t'} = R_{t'} \circ L_t$、$\theta(L_t) = R_t^V$ 中的$t, t'$。

18.7。由于$T_e(G)$是$U(G)$的原语元素的集合，

$$
[T_e(G), T_e(G)] \subset T_e(G).
$$

可范空间$T_e(G)$与括号一起是可范李代数，称为G的可范李代数（或G的李代数），记为$L(G)$。令$E(G)$为$L(G)$的包络代数。将$L(G)$的典范嵌入转换为$U(G)$定义同态$\eta$将代数$E(G)$转换为代数$U(G)$；如果K的特征为0，则$\eta$是一个大数同构，通过它$U(G)$可以与$E(G)$识别。使用 18.3 的记号，对于所有 $a \in L(G)$，令 $D_a$ 为 $a$ 在 X 上定义的点分布的域。 映射$(a, x) \mapsto D_a(x)$是向量丛$L(G) \times X$的类$C^{r-1}$到向量丛$T(X)$的态射。令I是K包含0的开子集和类$C^r$的$\gamma : I \to G$映射，使得$\gamma(0) = e$。让$a = T_0(\gamma) l \in L(G)$。如果$f : X \to F$是类$C^r$中的函数，那么

$$
(D_a f)(x) = \lim_{k \in K^*, k \to 0} k^{-1}(f(\gamma(k)x) - f(x)).
$$

若$r \geq 2$，映射$a \mapsto D_a$为X上$L(G)$的类$C^{r-1}$左无穷小运算律。

18.8。设G和H为李群细菌，G的$\phi$态射为H。$U(\phi)$到$L(G)$的限制，即$T_e(\phi)$，是$L(G)$到$L(H)$的连续态射，其中我们用$L(\phi)$表示。如果$\psi$是态射的H进入李群胚芽，则$L(\psi \circ \phi) = L(\psi) \circ L(\phi)$。为了使$\phi$成为浸没，$L(\phi)$是$L(G)$的同构到$L(H)$的谎言子代数上是必要且充分的，该谎言承认拓扑补充。特别是，如果 G 是 H 的李子群胚芽，并且 $\phi$ 是典范嵌入，则$L(G)$ 可以通过 $L(\phi)$ 与$L(H)$ 的李子代数进行识别。如果 $(G_i)_{i \in I}$ 是李群细菌的有限家族，G 是它们的乘积，则 $L(G)$ 被规范地识别为 $\prod_{i \in I} L(G_i)$。

18.9。 如果 K 的特征 > 0，则令 G 为有限维的李群胚芽。 设 F 为完全可范空间。 令 $\alpha$ 为 G 上次数 k 的微分形式与 F 中的值。 如果 $\alpha_g$ 由 $\alpha_e$ 通过 e 的邻域的映射 $h \mapsto gh$ 推导出来，则$\alpha$ 称为 G 上的左不变量邻域克。 如果 $\alpha$ 保持不变，则 $\alpha$ 是解析的。 The mapping $\alpha \mapsto \alpha_e$ is a bijection of the set of left invariant differential forms of degree k on G with values in F onto the set of continuous alternating k-linear mappings of $T_e(G)$ into F. 如果$\alpha_e = \mathrm{Id}_{T_e(G)}$，$\alpha$称为G*的*左规范微分形式。 右不变微分形式的定义和G的右典型微分形式是类似的。 如果$\omega$是G的左规范微分形式，则$d\omega + [\omega]^2 = 0$。 设M为G中的类$C^r$之流形和M的类$C^r$之$f$映射。 $f$的左微分，用$f^{-1}.df$表示，是M上次数1与$L(G)$中值的微分形式，与每个向量$u \in T_m(M)$元素$f(m)^{-1}.(T_{m,f})(u)$相关联。 然后是$f^{-1}.df = f^*(\omega)$和$d\alpha + [\alpha]^2 = 0$。 如果M到G中的两个映射、$f$和$g$具有相同的左微分且K的特征为0，则$fg^{-1}$局部常数。

### 习题{#lie-iii-s3-exercises}

§ 3](exercises/s3/)参见[习题。
