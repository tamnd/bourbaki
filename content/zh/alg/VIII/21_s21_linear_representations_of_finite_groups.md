---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 21
section_title: Linear Representations of Finite Groups
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.397-A VIII.434
pdf_pages: 0414-0451
extraction: native+ocr
subsections:
    - "no": 1
      title: Linear Representations
      page: 397
      pdf_page: 414
    - "no": 2
      title: Maschke’s Theorem
      page: 401
      pdf_page: 418
    - "no": 3
      title: Induced and Coinduced Representations
      page: 402
      pdf_page: 419
    - "no": 4
      title: Representations and the Grothendieck Group
      page: 404
      pdf_page: 421
    - "no": 5
      title: Fourier Inversion Formula
      page: 406
      pdf_page: 423
    - "no": 6
      title: Schur Orthogonality Relations
      page: 409
      pdf_page: 426
    - "no": 7
      title: Orthogonality Relation for Characters
      page: 410
      pdf_page: 427
    - "no": 8
      title: Central Functions on a Finite Group
      page: 411
      pdf_page: 428
    - "no": 9
      title: The Case of Abelian Groups
      page: 414
      pdf_page: 431
    - "no": 10
      title: Characters and Grothendieck Groups
      page: 415
      pdf_page: 432
    - "no": 11
      title: Dimension of Simple Representations
      page: 415
      pdf_page: 432
    - "no": 12
      title: Change of Base Field
      page: 416
      pdf_page: 433
    - "no": 13
      title: Complex Linear Representations
      page: 421
      pdf_page: 438
statements: 36
exercises: 30
content_sha256: 35974cffb08ca339eeb985b8f519ac14398ec49e318366a77c0ab1910a6d8160
translated_from: content/en/alg/VIII/21_s21_linear_representations_of_finite_groups.md
translation_method: google
source_content_sha256: 9b88499ec4cd1b75b385f04753440e80043e0341bcb3af756c5dd1b9f9bd76d6
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 8ac888c32e1f9ee868cf2df2352aa3a953a139ef8e592f607d24476cc0bc2356
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 21。 线性表示有限群

在这个截面中，G是群，K是交换环。如果G是有限群，那么我们用K的$|G|$元素Card(G)$\cdot 1$来表示。从No. 5开始，我们假设群G是有限的，环K是代数闭域，并且$|G|$不是零。

### 1.线性表示

#### 定义 1 {#alg-viii-s21-def-1 .statement tag=00NC}

设M为K-模。 M 中 G 的线性表示是从 G 到线性群 $\mathbf{G}\mathbf{L}(M)$ (II, §1, No. 2, p. 195) 的群同态。

设$\pi$为K-模M中G的线性表示。我们还说对$(M, \pi )$是G的线性表示。当K为非零的且M为自由K-模时，M的维数称为次数（或维数）表示$\pi$。

回想一下，从 G 到群 G 的代数 K[G] 的典范映射 $g\mapsto e_g$ 是 K-模 K[G] 的基。通过滥用记号，我们还用$g$表示K[G]的元素$e_g$。给定G的线性表示$\pi : G\rightarrow \mathbf{G}\mathbf{L}(M)$，从K[G]到End$_K(M)$存在K-代数的唯一同态即扩展$\pi$(III, §2, No. 6，p. 447，例)；我们也用 $\pi$ 表示这个扩张。它是 M 中代数 K[G] 的表示 (VIII, p. 373, 定义 1)，因而 M 是 K[G] 模。相反，M 中 G 的定义线性表示的每一个代数 K[G] 线性表示 $\rho$ 由 $g\mapsto \rho (g)$ 给出。

我们将关于K[G]-模结构的术语自由地应用于群G的线性表示。对于例，我们谈论子表示，简单的表示，表示的直和等。令$(M, \pi )$和$(M', \pi ')$为G 的线性表示；我们用 K[G]-模块的同态的 Hom$_G(\pi , \pi ')$ K-模 Hom$_{K[G]}(M,M')$ 表示从 M 到 $M'$.[^1]

如果对于 G 的元素的每个对 $(g, g')$ 有 $f(gg') =$ $f(g'g)$，则从 G 到 K 的映射 $f$ 称为中心函数；等价地，对于G的元素$g, h$的每个对，我们有$f(ghg^{-1}) =$$f(h)$。因此中心函数是G上的函数，其限制到每个共轭类是恒定的。它们从G到K的形式子模、空间、映射，记为$\mathscr{Z}_K(G)$。当G有限时，K-代数$\mathscr{Z}_K(G)$是G的共轭类维数数自由K-模。代数K[G]的中心Z(K[G])由元素$a=\sum a_gg$组成K[G]使得对于每个$h\in G$有$hah^{-1}=a$。现在，我们有

$$
hah^{-1}=\sum_{g\in G}a_{h^{-1}gh}g
$$

因而，当 G 有限时，代数 K[G] 的中心 Z(K[G]) 由中心函数组成。

令$(M, \pi )$为G的线性表示。假设M为有限维自由K-模。 $\pi$的迹是K[G]的表示与$\pi$相关的迹，即K[G]上的(VIII，p. 382)、线性形式$a\mapsto$Tr($\pi (a)$)。这个线性形式是由G到K的映射$g\mapsto$Tr($\pi (g)$)决定的，我们称之为表示$\pi$的特征标并用$\chi_{\pi}$表示。 表示的特征标是中心函数（II, §4, No. 3、p. 273、命题 3）。

设 M 和 $M'$ 为有限维自由K-模。令$\pi$和$\pi '$分别为M和$M'$中G的线性表示。那么$M\oplus M'$就是有限维自由K-模，并且通过III, §9, No. 2、p. 543的命题 1，我们有

$$
\chi_{\pi\oplus\pi'}=\chi_{\pi}+\chi_{\pi'}
$$

更一般地，让

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

为 K[G] 模的正合序列，并令 $\pi ,\pi '$ 和 $\pi ''$ 分别为与 $M, M'$ 和 $M''$ 伴随的 G 的线性表示。假设 K-模 $M'$ 和 $M''$ 是自由且有限维的。那么 M (II, §1, No. 11, p. 218, 命题 21) 也是如此，我们有

$$
\chi_{\pi}=\chi_{\pi'}+\chi_{\pi''} \tag{1}
$$

#### 命题 1 {#alg-viii-s21-prop-1 .statement tag=00ND}

假设K是交换域。令 $\pi$ 和 $\pi '$ 为 G 的有限维半单 K 线性表示。

a) 如果对于每个$g\in G$，$\pi (g)$和$\pi '(g)$的特征多项式都相同，则表示、$\pi$和$\pi '$同构的。

b) 此外，假设 K 具有特征 0。如果特征标 $\chi_{\pi}$ 和 $\chi_{\pi'}$ 相等，则表示 $\pi$ 和 $\pi '$ 同构的。

断言 a) 由VIII、p. 386的推论1得出； 断言 b) 由VIII、p. 384 的推论部分 a) 得出。

#### 例 1 {#alg-viii-s21-n1-exa-1 .statement tag=00NE}

G 的单位或平凡表示是表示 $(K, \varepsilon )$，其中对于每个 $g\in G$ 都有 $\varepsilon (g) =$ Id$_K$。它的特征标是常数函数，值为1。

#### 例 2 {#alg-viii-s21-n1-exa-2 .statement tag=00NF}

G 的（左）正则表示是 K[G] 中 G 的表示 $\boldsymbol{\gamma }$，由 $\boldsymbol{\gamma }(g)(x) =gx$ 对于 $g\in G$ 和 $x\in K[G]$ 定义。它位于代数 K[G] (VIII, p. 375) 的左侧正则表示对应。假设群 G 是有限的。 正则表示则有有限次数。对于与恒等式不同的 G 的每一个元素$g$，K[G]中乘法距$g$相对于典范基的矩阵是置换的矩阵，没有固定的点。因此我们有

$|G|$ 如果 $g$ 是单位元素，

$$
\chi_{\boldsymbol{\gamma }}(g) = \tag{2}
$$

否则为 0。

同样，我们定义 G 的右正则表示。 G 的双正则表示是 K[G] 中 $G\times G$ 的表示 $\rho$，由 $\rho (g, g')(x) =gxg^{'-1}$ 对于$(g, g')\in G\times G$ 和 $x\in K[G]$ 定义。

#### 例 3 {#alg-viii-s21-n1-exa-3 .statement tag=00NG}

给定 G 的线性表示 $(M, \pi )$，$\pi$ 的同余或对偶表示 $\pi^{\vee}$ 是 K-模中 G 的表示对偶于由关系 $\pi^{\vee}(g) =^t\pi (g^{-1})$ 定义的每个$g\in G$ (cf.) II, §2, No. 5，p. 234）。 如果 M 是有限维自由K-模，那么它的对偶也是如此，并且对于每个 $g\in G$，我们都有 $\chi_{\pi^{\vee}}(g) =\chi_{\pi}(g^{-1})$。

#### 例 4 {#alg-viii-s21-n1-exa-4 .statement tag=00NH}

令$(M, \pi )$和$(M', \pi ')$为G的线性表示。在VIII、p. 198的例 1中，我们在$M\otimes_KM'$上定义了一个K[G]-模结构。 相应的线性表示称为$\pi$和$\pi '$的张量积，记为$\pi \otimes \pi '$。对于$g\in G,x\in M$和$x'\in M'$，我们有$((\pi \otimes \pi ')(g))(x\otimes x') =\pi (g)x\otimes \pi '(g)x'$。

如果M和M'是有限维自由K-模，那么通过III, §9, No. 2，p. 543的命题 2，我们有

(3)
$$
\chi_{\pi \otimes \pi'} = \chi_{\pi} \chi_{\pi'}.
$$

#### 例 5 {#alg-viii-s21-n1-exa-5 .statement tag=00NI}

假设 G 是两个群中的乘积 $G' \times G''$。 K-线性映射从$K[G'] \otimes_K K[G'']$到$K[G]$，将$g' \otimes g''$发送到$(g', g'')$，对于$g' \in G'$和$g'' \in G''$是代数同构。令$(M', \pi')$为$G'$之线性表示，且$(M'', \pi'')$线性表示为$G''$。 $\pi'$和$\pi''$的外部张量积，用$\pi' \otimes \pi''$表示，是$(g', g'') \in G' \times G''$由$(\pi' \otimes \pi'')(g', g'') = \pi'(g') \otimes \pi''(g'')$定义的向量空间$M' \otimes M''$中$G' \times G''$的表示。如果$M'$和$M''$是有限维自由K-模，则$M' \otimes_K M''$是有限维自由K-模，表示$\pi' \otimes \pi''$的特征标由公式给出
$$
\chi_{\pi' \otimes \pi''}(g', g'') = \chi_{\pi'}(g') \chi_{\pi''}(g'')
$$
对于$g' \in G'$和$g'' \in G''$（III, §9, No. 2、p. 542中的命题 2）。

#### 例 6 {#alg-viii-s21-n1-exa-6 .statement tag=00NJ}

令$(V, \pi)$为G的线性表示，使得V为有限维自由K-模。我们在 $\operatorname{End}_K(V)$ 公式 $G \times G$ 定义表示 $\rho$
$$
\rho(g, g')(u) = \pi(g') \circ u \circ \pi(g^{-1}).
$$
II, §4, No. 2的K-模同构$\theta_V : V^* \otimes_K V \to \operatorname{End}_K(V)$，p. 271从外部张量积$\pi^\vee \otimes \pi$到$\rho$是表示的同构。 映射 $g \mapsto \rho(1, g)$（分别为 $g \mapsto \rho(g, 1)$）是 G 的表示同构于 $\pi^{\dim_K V}$（分别为 $(\pi^\vee)^{\dim_K V}$）。

令L为交换K-代数，令$(M, \pi)$为群G的线性表示。由$g \mapsto \operatorname{Id}_L \otimes \pi(g)$定义的群同态$\pi_{(L)} : G \to \mathbf{GL}(M_{(L)})$是L模块中G的线性表示 $M_{(L)}$，称为G的线性表示，由标量K的环的扩张从表示$\pi$推导出到L。

假设 K 为域并且 L 为非零的可交换 K 代数。设$(M, \pi)$和$(M', \pi')$为G的线性表示。表示$\pi$和$\pi'$同构当且仅当$\pi_{(L)}$和$\pi'_{(L)}$为(VIII, p. 37, 定理3)。

此外，假设代数L是K的扩张。考虑在VIII、p. 198的例1中定义的环$R_K(G)$和$R_L(G)$。标量的扩张定义环同态
$$
u : R_K(G) \longrightarrow R_L(G).
$$

这个同态是单射的，元素$\xi \in R_K(G)$有效当且仅当$u(\xi )$是（VIII，p. 195，定理1）。

### 2.马施克定理

#### 定理 1 {#alg-viii-s21-thm-1 .statement tag=00NK}

假设群 G 是有限的。设 M 为 K[G]-模，N 为 M 的 K[G]-子模。假设 N 是 K-模 M 的直因子，并且 $|G|$ 在 K 中可逆。则 N 是 K[G]-模 M 的直因子。

令 $p$ 为 M 中与像 N 的 K 线性投影算子。我们通过设定计算 K-模 M 的定义自同态 $q$

$$
q(x) =|G|^{-1}\sum_{g\in G}g p(g^{-1}x)
$$

每$x\in M$。由于 N 在 G 的作用和 N 上的恒等式$p$ 诱导下是稳定的，因此我们看到 $q$ 将 M 发送到 N 中，并且在 N 上的恒等式诱导下。

因而，K-模 M 是$q$ 的像 N 的直和和$q$ 的核。对于每个$x\in M$和$g\in G$，我们都有$g q(x) =q(gx)$，因而$q$的核是M的K[G]子模。这证明N是K[G]-模M的直因子。

#### 推论 1 (Maschke) {#alg-viii-s21-thm-1-cor-1 .statement tag=00SC}

假设群 G 是有限的并且 K 是交换域。 代数 K[G] 是半单当且仅当域 K 中的元素 $|G|$ 不是零。

假设$|G| \not= 0$。到定理 1 时，$K[G]_s$ 的每个 K[G]-子模都是直因子。因而 K[G] 是半单。

反之，假设$|G|$为零，并用K[G]的中心的$\varepsilon$元素$\sum_{g\in G}g$来表示。我们有$\varepsilon \not= 0$但有$\varepsilon^2=|G|\varepsilon = 0$，所以K[G]不是半单（VIII，p. 153，命题3，a）和VIII，p. 157，注1）。

#### 推论 2 {#alg-viii-s21-thm-1-cor-2 .statement tag=00NL}

假设群 G 是有限的，并且 $|G|$ 在 K 中是可逆的。K[G]-模分裂的的正合序列当且仅当它分裂的作为 K-模的正合序列。

给定正合序列的 K[G]-模块

0 // ${M'}^f$ // M // $M''$ // $0$,

满足态射$f$中的应用定理1至像即可。

#### 推论 3 {#alg-viii-s21-thm-1-cor-3 .statement tag=00NM}

假设群 G 是有限的，并且 $|G|$ 在 K 中是可逆的。K[G]-模是射影的当且仅当它射影为 K-模时。

设 P 为 K[G]-模。如果 P 是自由 K[G]-模 M 的直因子，则它是自由K-模 M 的更不必说直因子。鉴于 II, §2, No. 2、p. 231、命题 4，逆命题由推论 2 得出， d).

#### 推论 4 {#alg-viii-s21-thm-1-cor-4 .statement tag=00NN}

a) 假设群 G 是有限的，并且 K 是特征 0 的交换域。G 的两个有限维线性表示同构当且仅当它们具有相同的特征标。

b) 假设 K 是完美域，其特征为素数数 $p$，并且群 G 是有限的，是$p$ 的基数素数。 G 的有限维线性表示的特征标是零当且仅当该表示同构于 $p$ 成对同构表示的直和。

在推论假设下，G的每个有限维线性表示都是半单。推论由VIII、p. 384 的推论得出。

#### 推论 5 {#alg-viii-s21-thm-1-cor-5 .statement tag=00NO}

假设群 G 是有限的，并且 K 是交换域，其中 $|G| \not= 0$。令$\pi$和$\pi '$是G的有限维线性表示。则$\pi$和$\pi '$同构当且仅当对于G中的每个$g$，自同态$\pi (g)$和$\pi '(g)$具有相同的特征多项式。

这是从VIII、p. 386 的推论 1 得出的。

### 3.诱导和上诱导表示

令 H 为群 G 的子群。

如果$(V, \pi )$是G的线性表示，那么$\pi$到H的限制就是V中H的线性表示；我们用 Res$^G_H(\pi )$ 表示它。与 Res$^G_H(\pi )$ 伴随的 K[H]模只是从 K[G] 模 V 通过标量的限制 (II, §1, No. 13、p. 221) 推导出来的模。如果V是有限维自由K-模，则Res$^G_H(\pi )$的特征标对H来说是$\pi$的特征标限制。

令 $(M, \sigma )$ 为 H 的表示。

我们将 K[G] 视为 $(K[G]$，K[H]) 双模，将 M 视为 K[H]-模。 G 的 K[G]-模 $\mathscr{T}(M) = K[G]\otimes_{K[H]}M$ (VIII, p. 58) 定义线性表示，记为 Ind$^G_H(\sigma )$，称为由 $\sigma$ 诱导的 G 的表示。如果$(V, \pi )$是G的线性表示，则K[H]-模块$\mathscr{H}(V) =$Hom$_{K[G]}(K[G],V)$可以用K[H]-模块相应的到表示Res$^G_H(\pi )$来识别。因而， 伴随态射 (VIII, p. 59) 给出 K-模同构，称为规范，从 Hom$_H(\sigma$、Res$^G_H(\pi ))$ 到 Hom$_G$(Ind$^G_H(\sigma ), \pi$ ) （“弗罗贝尼乌斯互易律”）。

我们将 K[G] 视为 $(K[H]$, K[G])-双模。 G 的 K[G]-模 $\mathscr{H}(M) =$ Hom$_{K[H]}(K[G],M)$ 定义表示，记为 Coind$^G_H(\sigma )$，称为由 $\sigma$ 共同诱导的 G 的表示。如果$(V, \pi )$是G的线性表示，则K[H]-模$\mathscr{T}(V) = K[G]\otimes_{K[G]}V$可以用K[H]-模相应的到表示Res$^G_H(\pi )$来识别。因而，伴随态射（loc.cit.）给出K-模同构，称为规范，从Hom$_H$（Res$^G_H(\pi ), \sigma$）到Hom$_G(\pi$，Coind$^G_H(\sigma ))$。

令 $\varepsilon : K[G]\rightarrow K[H]$ 为 K-模同态，如果 $h\in$ H，则为关系 $\varepsilon (h) =h$；如果 $g\in G$ - H，则为 $\varepsilon (g) = 0$。 映射 $\varepsilon$ 为同态 $(K[H]$, K[H])-双模。令$(M, \sigma )$为H的线性表示。映射$v\mapsto v\circ \varepsilon$从Hom$_{K[H]}(K[H],M)$到Hom$_{K[H]}(K[G],M)$是K[H]-模的同态。通过将 M 与 Hom$_{K[H]}(K[H],M)$ 进行识别，我们获得了从 M 到 Res$^G_H$(Coind$^G_H(\sigma )$) 的 K[H]-模的同态。 弗罗贝尼乌斯互易律将其发送到从Ind$^G_H(\sigma )$到特征为关系的Coind$^G_H(\sigma )$的K[G]模块的同态$\iota$

$$
\iota (g\otimes m)(g') =\varepsilon (g'g)m
$$

对于 $g, g'\in G$ 和 $m\in M$。这个同态被称为规范的。

#### 命题 2 {#alg-viii-s21-prop-2 .statement tag=00NP}

令 H 为 G 的子群，并令 $(M, \sigma )$ 为 H 的线性表示。 典范同态 $\iota :$ Ind$^G_H(\sigma )\rightarrow$ Coind$^G_H(\sigma )$ 是单射的。如果子群 H 在 G 中具有有限的指标，则 $\iota$ 是 K[G]-模的同构。

设$S\subset G$为$G/H$的代表的系统。族$(s)_{s\in S}$是右K[H]-模K[G]的基。由此可见，$(m_s)_{s\in S}\mapsto \sum_{s\in S}s\otimes m_s$定义的映射$M^{(S)}\rightarrow$Ind$^G_H(\sigma )$是K-模的同构。对于所有 $s, s'\in S$ 和每个 $m\in M$，我们有关系

$$
\iota (s'\otimes m)(s^{-1}) =\begin{cases} m & \text{if } s=s',\\ 0 & \text{otherwise.}\end{cases}
$$

由此可见 $\iota '$ 是单射的。

假设 H 在 G 中具有有限的指标。则集合 S 是有限的；令$\rho$为映射，从Coind$^G_H(\sigma )$到由$u\mapsto \sum_{s\in S}s\otimes u(s^{-1})$给出的Ind$^G_H(\sigma )$。它满足$(\iota \circ \rho (u))(s^{-1}) =u(s^{-1})$对于$u\in$硬币$^G_H(\sigma )$和$s\in S$。由于族$(s^{-1})_{s\in S}$是左K[H]-模K[G]的基，所以映射$\iota \circ \rho$是恒等映射。因而，$\iota$ 与逆双射 $\rho$ 是双射的。

令 H 为有限指标的 G 的子群。设$u$为H上的中心函数；用G上的$u^0$函数表示扩展$u$，并且在G - H的每个点处表示零。令S为$G/H$的代表的系统。 $g\in G$、集合

(4)工业$^G_H(u)(g) =\sum_{s\in S}u^0(s^{-1}gs)$。

注对于所有$x, g\in G$ 和每个$h\in H$，我们有$u^0((xh)^{-1}gxh) =$ $u^0(x^{-1}gx)$。由此可见，Ind$^G_H(u)$是G上的中心函数，不依赖于S的选择。因此，我们将定义K-线性映射Ind$^G_H$从$\mathscr{Z}_K(H)$到$\mathscr{Z}_K(G)$。

#### 命题 3 {#alg-viii-s21-prop-3 .statement tag=00NQ}

令 H 为有限指标的 G 的子群。令$(M, \sigma )$为H的线性表示。假设M为有限维自由K-模。用$\sigma$诱导的G的$(V, \pi )$表示表示。那么 K-模 V 是自由且有限维的，并且

(5)$\chi_{\pi}=$工业$^G_H(\chi_{\sigma})$。

令S为$G/H$的代表系统。正如我们在上面看到的，$(m_s)_{s\in S}\mapsto \sum_{s\in S}s\otimes m_s$给出的线性映射$M^S\rightarrow$Ind$^G_H(M)$是K-模同构。特别地，V是有限维自由K-模。对于任何$g\in G$，用映射$m\mapsto g\otimes m$表示M的$M_g$像。对于所有$g, g'\in G$，当且仅当$gH =g'H$时，我们才有$M_g= M_{g'}$，并且对于$s\in S$，V是子模$M_s$的直和。对于所有$g, g'\in G$，我们还有$\pi (g)M_{g'}= M_{gg'}$。对于任何$g\in G$，用S的元素$s$的$S_g$集合表示，使得$s^{-1}gs\in H$。对于所有$g, g'\in G$，使得V诱导自同构$\pi (g)_{g'}$$M_{g'}$中的$g^{'-1}gg'\in H$、自同构$\pi (g)$，并且我们有

Tr($\pi (g)$) $=\sum_{s\in S_g}$ Tr($\pi (g)_s$) $=\sum_{s\in S_g}$ Tr($\sigma (s^{-1}gs)$)。

命题的最后一个断言如下。

### 4.表示与Grothendieck群

在这个小节中，我们假设K是交换域。给定 G 的有限维线性表示 $(M, \pi )$，我们用 Grothendieck 环 $R_K(G)$ (VIII, p. 198, 例 1) 中 K[G]-模 M 的 $[\pi ]$ 类表示。

通过环 $R_K$(G)上合成的律的定义，如果$\pi$和$\pi '$是G的有限维线性表示，那么我们有

$$
[\pi \oplus \pi '] = [\pi ] + [\pi '],[\pi \otimes \pi '] = [\pi ] [\pi ']
$$

环$R_K(G)$的单位元是G的单位表示类(VIII，p. 399，例1)。

环 $R_K(G)$ 是一个自由 $\mathbf{Z}$ 模，其中基集合为类的简单 K[G] 模，有限维在 K 上。当 $|G|$ 在 K 中可逆时，两个有限维表示同构当且仅当它们具有相同的性质$R_K(G)$中的类（VIII、p. 190，推论和p. 401，推论1）。

对于 G 的每个有限维线性表示 $(M, \pi )$，其矛盾 $\pi^{\vee}$ 也是有限维的。 表示 $\pi$ 和 $(\pi^{\vee})^{\vee}$ 同构的。如果$\pi '$也是G的有限维线性表示，则表示$(\pi \otimes \pi ')^{\vee}$和$\pi^{\vee}\otimes \pi^{'\vee}$同构的。如果

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

是 K[G]-模的正合序列在 K 上的有限维，则同余表示给出 K[G]-模的正合序列

$$
0\longrightarrow M^{''\vee}\longrightarrow M^{\vee}\longrightarrow M^{'\vee}\longrightarrow 0
$$

（II, §7, No. 5，p. 299，定理 5 的推论）。对于格罗滕迪克群 (VIII, p. 186, 命题 4) 的泛性质，对于每个有限维线性表示，存在环 $R_K(G)$ 的自同构 $c\mapsto c^{\vee}$，其特征为$[\pi ]^{\vee}= [\pi^{\vee}]$ G 的$\pi$； $R_K(G)$中每元素$c$就有$(c^{\vee})^{\vee}=c$。

令 H 为 G 的子群。限制保留正合序列。通过格罗滕迪克群的泛性质（前述），因此存在群同态，用Res$^G_H$表示，从$R_K(G)$到$R_K(H)$，其特征为关系

(6) 分辨率$^G_H[\pi ] =$ [分辨率$^G_H(\pi )]$

对于 G 的每个有限维线性表示 $\pi$；是环同态。如果H在G中具有有限的指标，那么通过II, §7, No. 7、p. 306的命题 14，我们可以得到定义，类似地，群同态Ind$^G_H$从$R_K(H)$到$R_K(G)$的特征为关系

(7) 工业$^G_H[\sigma ] =$ [工业$^G_H(\sigma )]$

对于 H 的每个有限维线性表示 $\sigma$。

由上述VIII、p. 399的关系(1)和VIII、p. 400以及格罗滕迪克群的泛性质，存在环同态$\Theta_G$ G 上中心函数的$R_K(G)$到代数$\mathscr{Z}_K(G)$，其特征在于G的每个有限维表示$\pi$有$\Theta_G([\pi ]) =\chi_{\pi}$。

如果 H 是 G 的子群，则与群 G 和 H 关联的同态 $\Theta_G$ 和 $\Theta_H$ 与运算 Res$^G_H$ 和 Ind$^G_H$ 相容的（VIII、p. 402 和VIII、p. 404、命题 3)。

假设 G 是两个群中的乘积 $G'\times G''$。由VIII、p. 213、注 2，存在从$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')$到群$R_K(G'\times G'')$的$\mathbf{Z}$线性映射$\kappa$，其特征为关系$\kappa ([\pi ']\otimes [\pi '']) = [\pi '\pi '']$ $\pi '$（分别$\pi ''$）有限维表示或$G'$（分别$G''$）和$\pi '\pi ''$外部张量积（VIII、p. 400、例5）。是环同态。如果域 K 是代数闭的，则映射 $\kappa$ 是同构 (VIII, p. 213, 注 2)。

假设 G 是两个群中的乘积 $G'\times G''$。用$\psi$同态表示从$\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')$到$\mathscr{Z}_K(G)$发送$f'\otimes f''$到函数$(g', g'')\mapsto f'(g')f''(g'')$。以下图表通勤：

$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')^{\kappa}$ // $R_K(G)$

$\Theta_{G'}\otimes \Theta_{G''}\Theta_G$

$\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')^{\psi}$/$/\mathscr{Z}_K(G)$。

### 5.傅里叶反演公式

对于这个截面的余数，我们假设群G是有限的，并且K是代数闭域，其特征不是G的除阶，因此K的元素$|G|$不是零。

代数 K[G] 是半单 (马施克定理) 并且是有限维的。用简单 K[G]-模的类的 $\widehat{G}$ 集合表示。对于 G 的每个 $\lambda \in \widehat{G}$，选择线性表示 $(V_{\lambda}, \pi_{\lambda})$，使得关联的 K[G]-模有类 $\lambda$。 集合 $\widehat{G}$ 是有限的，向量空间 $V_{\lambda}$ 是有限维的（VIII、p. 141、例）。对于任意$\lambda \in \widehat{G}$，用表示$\pi_{\lambda}$中的$d_{\lambda}$次数表示，即K-向量空间$V_{\lambda}$中的维数，并用$\chi_{\lambda}$表示其特征标。

由 $F(\widehat{G})$ 乘积代数 $\prod_{\lambda \in \widehat{G}} \operatorname{End}_K(V_\lambda)$ 表示，并由 $\overline{\mathscr{F}}$ 映射表示，从 $K[G]$ 到 $F(\widehat{G})$ 由 $\overline{\mathscr{F}}(a) = (\pi_\lambda(a))_{\lambda \in \widehat{G}}$ 定​​义。由于域 $K$ 是代数闭集，因此 *映射 $\overline{\mathscr{F}}$ 是代数同构*（前述）。

对于每个$\lambda \in \widehat{G}$，代数$\operatorname{End}_K(V_\lambda)$的维数是$d_\lambda^2$； 代数 $K[G]$ 是 $\operatorname{Card}(G)$。因此我们有关系

$$
\operatorname{Card}(G) = \sum_{\lambda \in \widehat{G}} d_\lambda^2.
$$

用$\tau$表示代数$K[G]$中的迹线；通过定义，$K[G]$的元素$a$的迹$\tau(a)$就是$K[G]$的自同态$x \mapsto ax$的迹（III, §7, No. 7，p. 515）。设$a = \sum_{g \in G} a_g g$为$K[G]$的元素；通过公式 (2)，每 $g \in G$ 就有 $\tau(ag^{-1}) = |G| a_g$，因此关系

$$
a = |G|^{-1} \sum_{g \in G} \tau(ag^{-1})\ g.
$$

用$\widehat{\tau}$表示代数$F(\widehat{G})$中的轨迹。设$A = (A_\lambda)_{\lambda \in \widehat{G}}$为$F(\widehat{G})$的元素；我们有 (cf. III, §9, No. 3, p. 545, 例 3)

$$
\widehat{\tau}(A) = \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}(A_\lambda).
$$

由于映射 $\overline{\mathscr{F}}$ 是 $K$ 代数同构，所以我们有 $\widehat{\tau} \circ \overline{\mathscr{F}} = \tau$，因此

$$
\tau(a) = \widehat{\tau}(\overline{\mathscr{F}}(a)) = \widehat{\tau}\left((\pi_\lambda(a))_{\lambda \in \widehat{G}}\right) = \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}(\pi_\lambda(a)) = \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}_\lambda(a)
$$

对于每个 $a \in K[G]$，即

$$
\tau = \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}_\lambda.
$$

因此，通过VIII、p. 399的(2)，对于$g \in G$，我们有

$$
\sum_{\lambda \in \widehat{G}} d_\lambda \chi_\lambda(g) = \begin{cases}
|G| & \text{if } g \text{ is the identity element,} \\
0 & \text{otherwise.}
\end{cases}
$$

对于$a \in K[G]$，关系 (9) 取以下形式：

$$
a = |G|^{-1} \sum_{g \in G} \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}(\pi_\lambda(a)\pi_\lambda(g^{-1}))\ g;
$$

由此可见，对于 $F(\widehat{G})$ 中的每一个元素 $A = (A_\lambda)_{\lambda \in \widehat{G}}$，我们有

$$
\overline{\mathscr{F}}^{-1}(A) = |G|^{-1} \sum_{g \in G} \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}(A_\lambda \pi_\lambda(g^{-1}))\ g
$$

（“傅里叶反演公式”）。

对于$\mu\in \widehat{G}$，用$j_\mu:$End$_K(V_\mu)\longrightarrow \prod_{\lambda\in\widehat{G}}$End$_K(V_{\lambda})$映射表示，使得$j_\mu(u) = (v_{\lambda})$，其中$v_{\lambda}= 0$如果$\lambda \not=\mu$和$v_\mu=u$。到公式 (14)，我们有

(15)$\overline{\mathscr{F}}^{-1}(j_\mu(u)) =|G|^{-1}d_\mu\sum_{g\in G}$Tr($u\pi_\mu(g^{-1})$)$g$。

代数$F(\widehat{G}) =\prod_{\lambda\in\widehat{G}}$的中心结束$_K(V_{\lambda})$由$(a_{\lambda}1_{V_{\lambda}})_{\lambda\in\widehat{G}}$家族组成，其中$(a_{\lambda})$是K的元素家族。它是像乘以中心的$\overline{\mathscr{F}}$ 代数K[G]。因此，中心具有基$(e_{\lambda})_{\lambda\in\widehat{G}}$，其特征为关系

$$
\pi_{\lambda}(e_\mu) =\delta_{\lambda \mu}1_{V_{\lambda}} \tag{16}
$$

对于 $\lambda , \mu\in \widehat{G}$，其中 $\delta_{\lambda \mu}$ 是克罗内克三角洲函数。到公式 (15)，对于每 $\mu\in \widehat{G}$，我们有，

$$
e_\mu=|G|^{-1}d_\mu\sum_{g\in G}\chi_\mu(g^{-1})g \tag{17}
$$

这些元素满足关系

(18)$\sum_{\lambda\in\widehat{G}}e_{\lambda}= 1,e^2_\mu=e_\mu$、$e_\mu e_{\nu}= 0$

对于所有$\mu, \nu \in \widehat{G}$使得$\mu\not=\nu$；它们是 Z(K[G]) 的不可分解幂等 (VIII, p. 147, 命题 15)

#### 注 {#alg-viii-s21-n5-rem-1 .statement tag=00NR}

设$(V, \pi )$为G的线性表示。到马施克定理，K[G]-模V为半单。对于任何$\lambda \in \widehat{G}$，用$V^{\lambda}$表示K[G]-模V的型$\lambda$的同型组件；我们有$V =\bigoplus_{\lambda\in\widehat{G}}V^{\lambda}$。通过VIII、p. 147和公式的命题 15 (17)，V的投影算子以及与此相关的V的分解等于像$V^{\lambda}$

$$
\pi (e_{\lambda}) =|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})\pi (g) \tag{19}
$$

应用这个公式到$\pi =\pi_{\lambda}$，我们得到K的元素$d_{\lambda}\cdot 1$不是零。我们将进一步从（VIII，p. 420，推论2）看到$d_\mu$除是G的基数。

设$\lambda$为$\widehat{G}$中的元素。从 K[G] 到 End$_K(V_{\lambda})$ 映射 $\pi_{\lambda}$ 诱导同构 of $(K[G]$, K[G])-从 $e_{\lambda}K[G]$ 到 End$_K(V_{\lambda})$ 的双模。由VIII、p. 147的命题 15，K[G]-子模块$e_{\lambda}K[G]$是型$\lambda$的K[G]的同型组件。它也是 G 右侧正则表示 (VIII, p. 143, 命题 11) 的型 $\lambda^{\vee}$ 的同型成分，以及双正则表示的型 $\lambda \times \lambda^{\vee}$ 的同型成分（VIII、p. 381、命题 4）。

### 6.Schur正交关系

我们保留之前的小节的记号。令$\lambda$为$\widehat{G}$的元素，令$u$和$v$为End$_K(V_{\lambda})$的元素；到公式 (10)，我们有

$\widehat{\tau}(j_{\lambda}(u)j_{\lambda}(v)) =d_{\lambda}$Tr($uv$)。从 $\tau =\widehat{\tau}\circ \mathscr{F}$ 开始，我们从公式推出 (2) 和 (15) 关系

$d^2_{\lambda}|G|^{-1}\sum_{g\in G}$Tr($u\pi_{\lambda}(g)$)Tr($v\pi_{\lambda}(g^{-1})$)$=d_{\lambda}$Tr($uv$)。

我们之前观察到域 K 中的 $d_{\lambda}.1\not= 0$；由此可知 (20) $|G|^{-1}\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_{\lambda}(g^{-1})$) $=d^{-1}_{\lambda}$ Tr($uv$)。

让我们将这个关系应用到$u$和$v$有秩$\leqslant 1$的情况；我们得到 (21) $|G|^{-1}\sum_{g\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_{\lambda}(g^{-1})y\rangle =d^{-1}_{\lambda}\langle x^*, y\rangle \langle y^*, x\rangle$

对于$V_{\lambda}$中的$x,y$和$V_{\lambda}$的对偶$V^*_{\lambda}$中的$x^*, y^*$。

对于每个$\lambda \in \widehat{G}$，令$(e_{\lambda ,j})_{1\leqslant j\leqslant d_{\lambda}}$为$V_{\lambda}$的基；相对于该基用$V_{\lambda}$自同态$\pi_{\lambda}(g)$$(\pi^{\lambda}_{ij}(g))$矩阵表示。如果我们用 $V^*_{\lambda}$ 对偶 $(e_{\lambda ,j})$ 的$(e^*_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ 基表示，那么我们有 $\pi^{\lambda}_{ij}(g) =\langle e^*_{\lambda ,i}, \pi_{\lambda}(g)e_{\lambda ,j}\rangle$，因此 (22) $|G|^{-1}\sum_{g\in G}\pi_{ij}^{\lambda}(g)\pi^{\lambda}_{k\ell}(g^{-1}) =d^{-1}_{\lambda}\delta_{i\ell}\delta_{jk}$。

现在让$\lambda$和$\mu$是$\widehat{G}$的两个不同的元素，并让$u\in$End$_K(V_{\lambda})$和$v\in$End$_K(V_\mu)$。再次通过关系 (15)，我们有 (23) $\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_\mu(g^{-1})$) $= 0$。

如上所述，我们推导出 (24) $\sum_{g\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_\mu(g^{-1})y\rangle = 0$

$x\in V_{\lambda},x^*\in V^*_{\lambda},y\in V_\mu$和$y^*\in V^*_\mu$。对于$[1, d_{\lambda}]$中的$i, j$和$[1, d_\mu]$中的$k, \ell$，我们还有(25)$\sum_{g\in G}\pi^{\lambda}_{ij}(g)\pi^\mu_{k\ell}(g^{-1}) = 0$。

关系 (20) 到 (25) 称为 Schur正交关系。

#### 注 {#alg-viii-s21-n6-rem-1 .statement tag=00NS}

我们认同代数结束$_K(V_{\lambda})$与矩阵代数$\mathbf{M}_{d_{\lambda}}(K)$经基$(e_{\lambda ,j})$$V_{\lambda}$。 映射$\mathscr{F}^{-1}$是同构从代数$\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$到代数K[G]。对于$\mu\in \widehat{G}$，用$\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$的$E^\mu_{ij}$元素表示，其指标$\mu$的分量为$\mathbf{M}_{d_\mu}(K)$的矩阵单位$E_{ij}$（II, §10, No. 3，p. 341），其其他分量为零； 集合$u^\mu_{ij}=\mathscr{F}^{-1}(E^\mu_{ij})$。 元素$u^{\lambda}_{ij}$的族，对于$\lambda \in \widehat{G}, 1\leqslant i\leqslant d_{\lambda}$、$1\leqslant j\leqslant d_{\lambda}$来说，是代数K[G]的基； 乘法表是

$$
u^{\lambda}_{ij}u^\mu_{k\ell}=\delta_{\lambda \mu}\delta_{jk}u^{\lambda}_{i\ell} \tag{26}
$$

此外，通过公式 (15)，我们有

$$
u^{\lambda}_{ij}=|G|^{-1}d_{\lambda g}\sum_{\in G}\pi^{\lambda}_{ji}(g^{-1})g \tag{27}
$$

### 7. 正交关系代表特征标

我们保留小节 5 和 6 的记号。回想一下，Z(K[G]) 由中心函数组成。

我们通过公式从 $K[G]\times K[G]$ 到 K 定义对称双线性映射

$$
\langle f, f'\rangle_G=|G|^{-1}\sum_{g\in G}f_gf'_{g^{-1}} \tag{28}
$$

对于每个 $f=\sum f_gg$ 和 $f'=\sum f_g'g$ 属于到 K[G]。我们有$\langle f, f'\rangle_G=$$|G|^{-2}\tau (f f')$。

#### 命题 4（正交关系特征标）{#alg-viii-s21-prop-4 .statement tag=00SG}

对于$\widehat{G}$中的$\lambda$和$\mu$，我们有$\langle \chi_{\lambda}, \chi_\mu\rangle_G=\delta_{\lambda \mu}$。

这是当自同态$u$和$v$被视为恒等式时关系(20)和(23)的具体情况。

#### 推论{#alg-viii-s21-n7-cor-1 .statement tag=00NT}

令 $\pi$ 和 $\pi '$ 为 G 的有限维线性表示。在域 K 中，我们有

（29）$\langle \chi_{\pi}, \chi_{\pi'}\rangle_G=$（昏暗$_K$坎$_G(\pi , \pi ')$）$\cdot 1$。

我们首先假设$\pi$和$\pi '$是简单的表示。根据$\pi$和$\pi '$是否同构，向量空间Hom$_G(\pi , \pi ')$有维数1或0（Schur的引理，VIII，p. 47，命题2）。在这种情况下，公式 (29) 由命题 4 得出。

在一般情况下，表示$\pi$（或$\pi '$）是简单的表示$\pi_1, . . . , \pi_m$（或$\pi '_1, . . . , \pi '_n$）的直和。对于 $1\leqslant i\leqslant m$、$1\leqslant j\leqslant n$，空间 Hom$_G(\pi , \pi ')$ 同构于空间 Hom$_G(\pi_i, \pi '_j)$ 的直和，并且我们有

$$
\chi_{\pi}=\chi_{\pi_1}+\cdots +\chi_{\pi_m},\chi_{\pi'}=\chi_{\pi'_1}+\cdots +\chi_{\pi'_n}
$$

通过线性，公式(29)的证明被简化为简单表示的情况。

### 8. 中环函数有限群

#### 命题 5 {#alg-viii-s21-prop-5 .statement tag=00NU}

家庭$(\chi_{\lambda})_{\lambda\in\widehat{G}}$是中央函数的向量空间的基。 G的简单线性表示类数等于G的共轭类数。

对于$a=\sum_{g\in G}a_gg\in K[G]$，写为$a^{\vee}=\sum_{g\in G}a_{g^{-1}}g$； 映射 $a\mapsto a^{\vee}$ 是代数 K[G] 的内合反自同构。到公式 (17) 时，每 $\lambda \in \widehat{G}$ 就有 $e_{\lambda}=|G|^{-1}d_{\lambda}\chi^{\vee}_{\lambda}$。 命题则可从以下事实得出：$(e_{\lambda})_{\lambda\in\widehat{G}}$ 是 K[G] 的中心的基。

用G的共轭类$\mathscr{C}$集合表示。设C为$\mathscr{C}$元素； C除以映射$g\mapsto g^{-1}$，像$C^{-1}$为共轭类。 C的元素互为G的共轭子群；他们的基数 $d(C)$ 满足

(30) 卡(G) = 卡(C)$d(C)$。

特别是，我们在域 K 中有 $d(C)\cdot 1\not= 0$。

设$f$为G上的中心函数。对于任何共轭类C，用$x\in C$的$f(x)$的$f(C)$公共的值表示。有了这个记号，正交关系对于特征标（VIII，p. 410，命题4）可以写成

$$
\sum_{C\in\mathscr{C}}\chi_{\lambda}(C^{-1})\chi_\mu(C)d(C)^{-1}=\delta_{\lambda \mu} \tag{31}
$$

对于$\widehat{G}$中的$\lambda$和$\mu$。

用型 $\widehat{G}\times \mathscr{C}$ 的 A 矩阵和条目 $\chi_{\lambda}(C)$ 表示，并用型 $\mathscr{C}\times \widehat{G}$ 的 B 矩阵和条目 $\chi_{\lambda}(C^{-1})d(C)^{-1}$ 表示。 集合 $\widehat{G}$ 和 $\mathscr{C}$ 具有相同的基数 (命题 5)； 关系(31)表示矩阵乘积AB是型$\widehat{G}\times \widehat{G}$的矩阵单位。 II, §10, No. 12、p. 360、矩阵乘积的命题11 BA为型$\mathscr{C}\times \mathscr{C}$矩阵单位；在其他字，我们有关系

$$
\sum_{\lambda\in\widehat{G}}\chi_{\lambda}(C^{-1})\chi_{\lambda}(C') =d(C)\delta_{CC'} \tag{32}
$$

$\mathscr{C}$中的C和$C'$（有时称为“特征标的第二个正交关系”）。

设H是G的子群。让我们注整数Card(H)除Card(G)并且$|G|$不是K中的零；因此，K 中有$|H| \not= 0$。

用Res$^G_H$线性映射表示，从Z(K[G])到Z(K[H])，将G上的中心函数发送到其限制到H。我们已经看到，如果$\chi_{\pi}$是有限维表示$\pi$的特征标 G，则 Res$^G_H(\chi_{\pi})$ 就是 H 的表示 Res$^G_H(\pi )$ 的特征标。

#### 命题 6 {#alg-viii-s21-prop-6 .statement tag=00NV}

设$f$为G上的中心函数，$u$为H上的中心函数。我们有

(33) $\langle$工业$^G_H(u), f\rangle_G=\langle u$，研究$^G_H(f)\rangle_H$。

G 的简单表示 Z(K[G]) 的形式基 (VIII, p. 411, 命题 5) 的特征标，对于 H 也同样成立。因此，在以下情况下成立 (33) 即可： $f$ 是 G 的简单表示 $\pi$ 的特征标 $\chi_{\pi}$，$u$ 是 H 的简单表示 $\sigma$ 的特征标 $\chi_{\sigma}$。在这种情况下， Ind$^G_H(u)$ 是 G 的表示 Ind$^G_H(\sigma )$ 的特征标，并且，由 VIII，p. 410，推论，我们有

$\langle$Ind$^G_H(u), f\rangle_G=$（昏暗$_K$坎$_G$（Ind$^G_H(\sigma ), \pi$））$\cdot 1$。

我们展示关系

$\langle u$，分辨率$^G_H(f)\rangle_H=$（昏暗$_K$坎$_H(\sigma$，分辨率$^G_H(\pi )$））$\cdot 1$

同样，等式 (33) 后面跟着弗罗贝尼乌斯互易律。

#### 命题 7 {#alg-viii-s21-prop-7 .statement tag=00NW}

令从G到K的$f$为映射。以下断言是等价的：

(i) K 中有 $\widehat{G}$ 的元素 $\lambda$ 和元素 $a$，使得$f=a\chi_{\lambda}$。

(ii) 对于 G 的元素中的每一个对 $(g, g')$，我们有

$$
f(g)f(g') =|G|^{-1}f(1)\sum_{h\in G}f(hgh^{-1}g') \tag{34}
$$

设$\lambda$为$\widehat{G}$的元素；对于$V_{\lambda}$中的每自同态$u$，集合

$$
u^{\natural}=|G|^{-1}\sum_{h\in G}\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1}) \tag{35}
$$

自同态 $u^{\natural}$ 或 $V_{\lambda}$ 是 K[G]-线性。根据 Schur 的引理（VIII、p. 47、定理 1）$,u^{\natural}$ 为位似。由于 $u$ 和 $u^{\natural}$ 具有相同的迹，因此我们有

$u^{\natural}=d^{-1}_{\lambda}$Tr($u$)$1_{V_{\lambda}}$。

设$u$和$v$为$V_{\lambda}$中的自同态；由此可见

（36）Tr（$u$）Tr（$v$）$=d_{\lambda}$Tr（$u^{\natural}v$）$=d_{\lambda}|G|^{-1}\sum_{h\in G}$Tr（$\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1})v$）。

在公式(36)中取$u=\pi_{\lambda}(g)$和$v=\pi_{\lambda}(g')$； 关系 (34) 对应$f=\chi_{\lambda}$如下。

相反，假设断言 (ii) 成立。如果我们有$f(1) = 0$，那么对于G的元素的每一个对$(g, g')$，$f(g)f(g') = 0$，因而$f= 0$。因此我们可以假设$f(1)\not= 0$。将$g'= 1$代入(34)，我们得到关系

$$
f(g) =|G|^{-1}\sum_{h\in G}f(hgh^{-1})
$$

对于每个$g\in G$，这意味着$f$是中心函数。到命题 5，存在 K 的元素族$(a_{\lambda})$，使得$f=\sum_{\lambda\in\widehat{G}}a_{\lambda}\chi_{\lambda}$。让我们用公式 (34) 中的这个表达式来替换 $f$；考虑到特征标$\chi_{\lambda}$中的每一个也满足这个关系，我们发现

$$
\sum_{\lambda ,\mu\in\widehat{G}}a_{\lambda}a_\mu\chi_{\lambda}(g)\chi_\mu(g') =\sum_{\lambda\in\widehat{G}}a_{\lambda}d^{-1}_{\lambda}f(1)\chi_{\lambda}(g)\chi_{\lambda}(g') \tag{37}
$$

$g, g'\in G$。这个关系也可以写成

$$
\sum_{\lambda ,\mu}(a_{\lambda}a_\mu-\delta_{\lambda \mu}a_{\lambda}d^{-1}_{\lambda}f(1))\chi_{\lambda}(g)\chi_\mu(g') = 0 \tag{38}
$$

$g, g'\in G$。现在，函数$\chi_{\lambda}$，对于$\lambda \in \widehat{G}$，是线性独立的（命题 5 of VIII，p. 411）；由此可见

$$
a_{\lambda}a_\mu=\delta_{\lambda \mu}a_{\lambda}d^{-1}_{\lambda}f(1)
$$

$\lambda , \mu\in \widehat{G}$。特别是，每当 $\lambda \not=\mu$ 时，$a_{\lambda}a_\mu= 0$。因而，$\widehat{G}$中最多存在一个元素$\lambda$使得$a_{\lambda}\not= 0$，并且我们有$f=a_{\lambda}\chi_{\lambda}$，因而(i)。

### 9.阿贝尔群的情形

在这个小节中，我们假设群G是阿贝尔的。

根据Schur的引理（VIII，p. 48，推论1），G的每个简单表示都有维数1。令$(M, \pi )$为表示，$\chi$为其特征标；对于每个$g\in G$和$x\in M$，我们有$\pi (g)(x) =\chi (g)x$。因而，特征标$\chi$是从G到K的乘法群$K^*$的同态。相反，从G到$K^*$的每个同态是次数1的G的表示的特征标。所以集合简单K[G]-模的类的$\widehat{G}$可以用从G到$K^*$的同态的集合Hom(G$,K^*$)来识别。我们从阿贝尔的群结构推论$\widehat{G}$； $\widehat{G}$ 对应至张量积（共表示）中的乘积。 群 G 和 $\widehat{G}$ 在 VIII、p. 411 的命题 5 中具有相同的基数。 G 上的每个函数都是中心，从 G 到 K $\widehat{G}$ 是映射向量空间基（见上文）。由于正交关系对应于特征标，这样的映射$f$相对于基$\widehat{G}:$有以下独特的分解

$$
f=\sum_{\chi\in\widehat{G}}\langle \chi , f\rangle_G\chi \tag{39}
$$

对于从 G 到 K 的映射 $f$ 和 $f'$，我们有关系

$$
\langle f, f'\rangle_G=\sum_{\chi\in\widehat{G}}\langle \chi , f\rangle_G\langle \chi , f'\rangle_G \tag{40}
$$

令$(V, \pi )$为G的线性表示。对于任何$\chi \in \widehat{G}$，用向量$v$的V由……组成的$V^{\chi}$子空间表示，使得对于每个$g\in G$都有$\pi (g)(v) =\chi (g)v$。 空间 $V^{\chi}$ 是 K[G]-模 V 型 $\chi$ 的同型组件。 空间V是$(V^{\chi})_{\chi\in\widehat{G}}$族的直和，V的投影算子$p_{\chi}$以及与此分解相关联的像$V^{\chi}$由下式给出

$$
p_{\chi}=|G|^{-1}\sum_{g\in G}\chi (g^{-1})\pi (g) \tag{41}
$$

因为关系 (19)。

#### 注 {#alg-viii-s21-n9-rem-1 .statement tag=00NX}

Let $n$ be the cardinal of the group G, and let $\mu_n(K)$ be the group of $n$-th roots of unity in K. 对于每个$g\in G$，我们有$g^n= 1$；因而，$\widehat{G}$可以识别为群Hom(G$, \mu_n(K)$)。 群$\mu_n(K)$是阶$n$（V, §11, No. 2，p. 78，定理1）的循环。 因此群 $\widehat{G}$ 同构于群 D(G) = Hom(G$,\mathbf{Q}/\mathbf{Z}$)。 由VII, §4, No. 9、p. 26、命题 10、群$\widehat{G}$与群G同构，映射将G的元素$g$发送到同态$\chi \mapsto \chi (g)$从G到$\widehat{\widehat{G}}$，$\widehat{G}$到$K^*$是同构。

### 10.特征标和格罗滕迪克群

用$\theta_G$K-代数同态表示，从$K\otimes_{\mathbf{Z}}R_K(G)$到$\mathscr{Z}_K(G)$，每有限维表示$\pi$发送$1\otimes [\pi ]$到$\chi_{\pi}$。

#### 命题 8 {#alg-viii-s21-prop-8 .statement tag=00NY}

a) 从$K\otimes_{\mathbf{Z}}R_K(G)$到$\mathscr{Z}_K(G)$，同态$\theta_G$是同构。

b) 假设 K 的特征为 0。 Then $\theta_G$ defines an isomorphism from $R_K(G)$ to the subring of $\mathscr{Z}_K(G)$ consisting of the linear combinations of the characters $\chi_{\lambda}$ for $\lambda$ in $\widehat{G}$ with integer coefficients.

族$([\lambda ])_{\lambda\in\widehat{G}}$是$\mathbf{Z}$模块$R_K$(G)的基，族$(\chi_{\lambda})_{\lambda\in\widehat{G}}$是K-向量空间$\mathscr{Z}_K(G)$的基。 断言 a) 和 b) 遵循 (VIII, p. 411, 命题 5)。

### 11.简单表示的维数

用 $n$ 表示群 G 的基数。 令 $\pi$ 为 G 在有限维 K-向量空间 M 中的线性表示。 对于每个$g\in G$，我们有$\pi (g)^n= 1_M$，因此$\pi (g)$除$T^n-1$的最小多项式。 由于 K 中存在 $n\cdot 1\not= 0$，因此该最小多项式是可分的 (V, §11, No. 2、p. 78)，并且由于域 K 是代数闭的，因此 M 的自同态 $\pi (g)$ 可对角化的 (VII, §5, No. 7、p. 40、命题 12)。 $\pi (g)$的特征值是单位元的$n$-第根，并且对于每个$\alpha \in K$，$\alpha$的几何重数为$\pi (g)$的特征值（VII, §5, No. 2，p. 30， 定义 1) 等于$\alpha$的重数，即$\pi (g)$的特征多项式的根。 Denote by $\mathscr{O}_n$ the subgroup of K generated by the set $\mu_n(K)$ of $n$-th roots of unity; it is a finitely generated $\mathbf{Z}$-module and a subring of K. $\pi$的特征标取$\mathscr{O}_n$中的值。

#### 命题 9 {#alg-viii-s21-prop-9 .statement tag=00NZ}

假设域 K 有特征零。那么 G 的每个简单表示的次数除 G 的基数。

令$(V, \pi )$为G的简单表示，$\chi$为其特征标。对于 Z(K[G]) 的每个元素 $a$，V 的自同态 $\pi (a)$ 为位似 (VIII, p. 47, 定理 1)；用 $\varphi (a)$ 表示满足 $\pi (a) =\varphi (a)_V$ 的标量。从 Z(K[G]) 到 K 的所得的映射 $\varphi$ 是代数同态。让我们取$a=\sum_{g\in G}\chi (g^{-1})g$；到VIII、p. 408的注，我们有$\varphi (a) =$（暗淡$V$）$^{-1}|G|$。另一方面，K[G]的$a$属于到子环$\mathscr{O}_n[G]\cap Z(K[G])$，它是有限生成的$\mathbf{Z}$-模块（VII, §3，p. 15，推论）。因此，K 属于的元素 $\varphi (a) =$ (dim $V$)$^{-1}|G|$ 到 K 的子环是有限生成的 $\mathbf{Z}$ 模。我们利用得出以下引理。

#### 引理 {#alg-viii-s21-n11-lem-1 .statement tag=00O0}

设L为$\mathbf{Q}$的扩张。设 A 为 L 的子环。假设 A 是有限生成的 $\mathbf{Z}$ 模块。我们有$A\cap \mathbf{Q}=\mathbf{Z}$。

由于$\mathbf{Z}$-模$A\cap \mathbf{Q}$是有限生成的，因此存在严格的正整数 N，使得$A\cap \mathbf{Q}$包含在$\frac{1}{N}\mathbf{Z}$中。设$x$为$\mathbf{Q}-\mathbf{Z}$的元素；我们将其写为$x=\frac{p}{q}$，其中$p$和$q$互质整数和$q\geqslant 2$。我们有$q^N\geqslant 2^N>N ($集合理论，III, §3, No. 6、p. 165、定理2)、整数$p^N$和$q^N$互质，因而$x^N\notin\frac{1}{N}\mathbf{Z}$。由此可见，$x$ 不属于到 A。结论证明引理。

在接下来的小节中，我们扩展命题9的情况，我们只假设K的特性不除阶G。

### 12.基域变换

我们保留之前的小节的记号。令$K'$为代数闭域，使得$K'$的元素$n\cdot 1$不是零。 群$\mu_n(K)$和$\mu_n(K')$是阶$n$（V, §11, No. 2，p. 78，定理1）的循环。 选择同构$\varphi$从$\mu_n(K)$到$\mu_n(K')$。令$\pi$为有限维K-向量空间中G的线性表示，并令$\pi '$为有限维$K'$向量空间中G的线性表示。我们说，$\pi$和$\pi '$相关（通过$\varphi$），如果对于每个$g\in G$和$\omega \in \mu_n$(K)，$\omega$的重数，因为$\pi (g)$的特征值等于重数 $\varphi (\omega )$ 相当于 $\pi '(g)$ 的特征值。在这种情况下，$\pi$和$\pi '$具有相同的维数，通过取$g= 1$可以看出。

令 $\pi_1$ 和 $\pi_2$（分别为 $\pi '_1$ 和 $\pi '_2$）为 G 在有限维向量空间上的线性表示在 K 上（分别为 $K'$）。我们有以下属性：

a) 如果$\pi_1$与$\pi '_1$和$\pi '_2$相关，则$\pi '_1$和$\pi '_2$同构的。

b) 如果$\pi_1$与$\pi '_1$相关，$\pi_2$与$\pi '_2$相关，则$\pi_1\oplus \pi_2$与$\pi '_1\oplus \pi '_2$相关，$\pi_1\otimes \pi_2$与$\pi '_1\otimes \pi '_2$相关。

断言 a) 由VIII、p. 402 和断言 b) 的推论 5 得出是明确的。

在这里，我们用简单 K[G]-模块的类的 $\mathscr{S}_K(G)$ 集合表示，之前用 $\widehat{G}$ 表示，并且我们同样用定义 $\mathscr{S}_{K'}(G)$ 表示。 集合 $\mathscr{S}_K(G)$ 和 $\mathscr{S}_{K'}(G)$ 都是有限的，基数数为共轭类（VIII、p. 411、命题 5）。

#### 命题 10 {#alg-viii-s21-prop-10 .statement tag=00O1}

从$\mathscr{S}_K(G)$到$\mathscr{S}_{K'}(G)$存在唯一映射$\varphi_G$，使得对于$\mathscr{S}_K(G)$中的每个$\lambda$，$\lambda$和$\varphi_G(\lambda )$通过$\varphi$相关。此外，$\varphi_G$是双射的。

$\varphi_G$ 的唯一性由上面的性质 a) 得出。

A) 假设域 K 的特征为 0。

群$\mu_n(K)$是循环的（V, §11, No. 2，p. 78，定理1）；这个群的选择生成元$\zeta$。考虑将 X 发送到 $\zeta$ 的环同态 $\rho :\mathbf{Z}[X]\rightarrow \mathscr{O}_n$。它是主观的。分圆多项式 $\Phi_n(X)$ 在 $\mathbf{Q}[X]$ (V, §11, No. 5, p. 84, 定理 2) 中不可约；因此它是 $\zeta$ 在 $\mathbf{Q}$ 上的最小多项式。多项式 $\Phi_n$ 是具有整数系数 (V, §11, No. 4, p. 81) 的一元多项式。令 $P\in \mathbf{Z}[X]$ 为多项式，使得 $P(\zeta ) = 0$；由多项式 (IV, §1, No. 6, p. 10) 的欧几里得除法，$\mathbf{Z}[X]$ 中存在两个多项式 Q 和 R，使得 P = QΦ$_n+ R$ 和 deg(R) $<$ deg(Φ$_n$)。我们有 $R(\zeta ) = 0$，因而 R = 0，因为 $\Phi_n$ 是 $\zeta$ 的最小多项式。因而，$\rho$的核是$\mathbf{Z}[X]$的理想$\Phi_n\mathbf{Z}[X]$，并且从$\mathbf{Z}[X]/\Phi_n\mathbf{Z}[X]$到$\mathscr{O}_n$是$\rho$诱导环同构。

集合$\zeta '=\varphi (\zeta )$；它是$K'$中单位元的原始$n$-第根，因此我们有$\Phi_n(\zeta ') = 0$（V, §11, No. 5，p. 83，引理3）。因而，存在从环$\mathscr{O}_n$到域$K'$，变换$\zeta$到$\zeta '$的同态$\varphi_0$；从$\mu_n(K)$到$\mu_n(K')$扩展映射$\varphi$。设$\mathscr{O}$为元素$\frac{a}{n^r}$的K由……组成与$a\in \mathscr{O}_n$和$r\in \mathbf{N}$的子环。由于$n\cdot 1$在$K'$中可逆，因此从$\mathscr{O}$到$K'$，同态$\varphi_0$扩展到同态$\varphi_1$。

我们将群G的认同代数$\mathscr{O}[G]$超过$\mathscr{O}$，将代数K[G]的子环和定义环同态Φ从$\mathscr{O}[G]$到$K'[G]$ 公式

$$
\Phi (\sum_{g\in G}a_gg)=\sum_{g\in G}\varphi_1(a_g)g \tag{42}
$$

用G的共轭类的$\mathscr{C}$集合表示。 For C in $\mathscr{C}$, denote by $u_C$ the element $\sum_{g\in C}g$ of $\mathscr{O}[G]$; the family $(u_C)_{C\in\mathscr{C}}$ is a basis over $\mathscr{O}$ of the center $Z(\mathscr{O}[G])$ of the algebra $\mathscr{O}[G]$ (VIII, p. 398). 对于 $\mathscr{S}_K$(G) 的任何元素 $\lambda$，用 $\chi_{\lambda}$ 表示其特征标，用 $d_{\lambda}$ 表示其维数，并用 $e_{\lambda}$ 元素表示，其定义为 K[G]

$$
e_{\lambda}=|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})g \tag{43}
$$

族$(e_{\lambda})$是基超过环K[G]的中心Z(K[G])的K(VIII，p. 408)。我们有

$$
e_{\lambda}=\sum_{C\in\mathscr{C}}\alpha_{\lambda ,C}u_C \tag{44}
$$

和

$$
\alpha_{\lambda ,C}=|G|^{-1}d_{\lambda}\chi_{\lambda}(C^{-1}) \tag{45}
$$

对于 $C\in \mathscr{C}$ 和 $\lambda \in \mathscr{S}_K$(G)、集合 $\beta_{C,\lambda}=|G|d^{-1}_{\lambda}d(C)^{-1}\chi_{\lambda}(C)$。 矩阵 $(\alpha_{\lambda ,C})$ 的条目在 $\mathscr{O}$ 中，由 VIII、p. 411 的公式 (31) 得出其逆矩阵是矩阵 $(\beta_{C,\lambda})$，其条目也在 $\mathscr{O}$ 中命题 9 个，共 VIII、p. 415。因而，家族$(e_{\lambda})$是$\mathscr{O}$模块$Z(\mathscr{O}[G])$的基。

$K'[G]$形式基元素$\Phi (u_C) =\sum_{g\in C}g$超过环$K'[G]$中心$Z(K'[G])$$K'$。我们有

$$
\Phi (e_{\lambda}) =\sum_{C\in\mathscr{C}}\varphi_1(\alpha_{\lambda ,C}) \Phi (u_C) \tag{46}
$$

且矩阵与条目 $\varphi_1(\alpha_{\lambda ,C})$ 是可逆的。因此，$\Phi (e_{\lambda})$的家族是$Z(K'[G])$的基。族 $(e_{\lambda})$ 是 Z(K[G]) 中幂等 1 的划分（VIII、p. 146 和 p. 408）；在其他字中，我们有

$\sum_{\lambda}e_{\lambda}= 1,e^2_{\lambda}=e_{\lambda},e_{\lambda}e_\mu= 0$如果$\lambda \not=\mu$。

由此可见，$\Phi (e_{\lambda})$的族是$Z(K'[G])$中幂等1的划分；由于该族的$Z(K'[G])$的基大于$K'$，因此其元素是$Z(K'[G])$中不可分解的幂等（VIII，p. 148，注4）。

对于 $\mathscr{S}_{K'}$(G)、定义 $\chi_{\lambda'},d_{\lambda'}$ 和 $e_{\lambda'}$ 中的$\lambda '$，如上所述。由 VIII、p. 408、元素 $e_{\lambda'}$ 是 $Z(K'[G])$ 中不可分解的幂等。因此，从$\mathscr{S}_K(G)$到$\mathscr{S}_{K'}(G)$存在双射$\varphi_G$，使得$\Phi (e_{\lambda}) =e_{\varphi_G(\lambda)}$对应于$\mathscr{S}_K(G)$中的每个$\lambda$。

将$\lambda$代入$\mathscr{S}_K(G)$； 集合$\lambda '=\varphi_G(\lambda )$。令$(V_{\lambda}, \pi_{\lambda})$（或$(V_{\lambda'}, \pi_{\lambda'})$）为G 的线性表示，其关联的K[G]-模（或$K'$[G]-模）具有类 $\lambda$（或$\lambda '$）。让我们证明$\lambda$和$\lambda '$是相关的。令$g$为G的元素。令$\delta (T)$为K[T]-模$K[T]\otimes_KV_{\lambda}$的自同态$1 + T\pi_{\lambda}(g)$的行列式。令$\omega_1, . . . , \omega_{d_{\lambda}}$为$\pi_{\lambda}(g)$中的特征值；我们有

$$
\delta (T) = (1 + T\omega_1)\cdots (1 + T\omega_{d_{\lambda}})
$$

同样，定义$\delta '(T)$，我们用$\omega '_1, . . . , \omega '_{d_{\lambda'}}$表示$\pi_{\lambda'}(g)$的特征值。 $\mathscr{O}$模$\mathscr{O}[G]$与基G自由，K-向量空间K[G]有基G。用Δ(T)表示$\mathscr{O}$[T]模$\mathscr{O}[T]\otimes_{\mathscr{O}}\mathscr{O}[G]$中$1 +e_{\lambda}gT$对乘法的行列式。它也是 K[T]-模 $K[T]\otimes_KK[G]$ 中乘法与 $1 +e_{\lambda}gT$ 的行列式。令$\overline{\varphi}_1$为同态，从$\mathscr{O}[T]$到$K'[T]$即扩展$\varphi_1$，并将T发送到T。由于G是$K'$向量空间$K'[G]$的基，因此多项式$\overline{\varphi}_1(\Delta (T))$等于$K'$向量空间$K'[G]$中$1 +e_{\lambda'}gT$对乘法的行列式$\Delta '(T)$。

代数 K[G] 是直和的简单组件$e_\mu K[G]$，其中$\mu$ 贯穿$\mathscr{S}_K(G)$。对于与$\lambda$不同的$\mu$，元素$e_{\lambda}g$消灭$e_\mu K[G]$。此外，在$e_{\lambda}K[G]$中，乘法乘$e_{\lambda}g$重合，以及乘法乘$g$。鉴于$e_{\lambda}K[G]$中G的VIII、p. 400、表示的VIII、p. 409和例6为类中的$d_{\lambda}$表示直和 $\lambda$。因此我们有 $\Delta (T) =\delta (T)^{d_{\lambda}}$。

类似地，我们有$\Delta '(T) =\delta '(T)^{d_{\lambda'}}$。

从关系 $\Delta '(T) =\overline{\varphi}_1$(Δ(T))，我们首先推导出 $d^2_{\lambda}=d^2_{\lambda'}$，进而推导出 $d_{\lambda}=d_{\lambda'}$，然后可以从序列 $(\omega '_1, . . . , \omega '_{d'_{\lambda'}})$ 通过集合的置换推导出序列 $\varphi (\omega_1), . . . , \varphi (\omega_{d_{\lambda}})$ 指标。

由于这对于 G 的每个元素 $g$ 都是成立的，因此表示 $\lambda$ 和 $\lambda '$ 是相关的。因而，当域 K 的特征为 0 时，我们证明了命题 10。

B) 一般情况。

令L为特征0的代数闭域（对于例，$\mathbf{Q}$的代数闭包）。用简单L[G]-模块的类的$\mathscr{S}_L(G)$集合表示。 选择同构$\eta$从群$\mu_n(L)$到群$\mu_n$(K)，以及集合$\eta '=\varphi \circ \eta$。到证明的部分A)，存在双射

$$
\eta_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_K(G),\eta '_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_{K'}(G)
$$

性质：对于$\mathscr{S}_L$(G)中的每个$\lambda$，表示$\lambda$和$\eta_G(\lambda )$通过$\eta$相关，表示$\lambda$和$\eta '_G(\lambda )$通过$\eta '$相关。 双射 $\varphi_G=\eta '_G\circ \eta_G^{-1}$ 具有所需的属性。

双射$\varphi_G$从$\mathscr{I}_K(G)$到$\mathscr{I}_{K'}(G)$扩展到同构，也用$\varphi_G$表示，从格罗滕迪克群$R_K(G)$到群$R_{K'}(G)$。

#### 注 1 {#alg-viii-s21-n12-rem-1 .statement tag=00O2}

假设$K'$是$K$的扩张，同构$\varphi$是映射$\xi \mapsto \xi \cdot 1$；那么映射 $\varphi_G$ 由从 $K$ 到 $K'$ 的标量扩张给出。

#### 推论 1 {#alg-viii-s21-prop-10-cor-1 .statement tag=00O3}

*从$R_K(G)$到$R_{K'}(G)$，映射$\varphi_G$是环同构。对于$K$向量空间中$G$的每个有限维表示$\pi$，我们有$\varphi_G([\pi]) = [\pi']$，其中$\pi'$是与$\pi$到$\varphi$*相关的表示。

这是从 $G$ 的表示和 VIII、p. 416 的性质 b) 得出的结论。

#### 推论 2 {#alg-viii-s21-prop-10-cor-2 .statement tag=00O4}

$G$*$G$除阶每个简单表示*维数。

这是从VIII、p. 415 的命题 10 和命题 9 开始的。

#### 注 2 {#alg-viii-s21-n12-rem-2 .statement tag=00O5}

假设群$G$是*阿贝尔的*。我们在VIII、p. 414的注中看到，$\mathscr{I}_K(G)$可以与集合$\operatorname{Hom}(G, \mu_n(K))$识别。同样，$\mathscr{I}_{K'}(G)$可以与$\operatorname{Hom}(G, \mu_n(K'))$识别。有了这些标识，双射$\varphi_G$就简单地变成了映射$\chi \mapsto \varphi \circ \chi$。

#### 注 3 {#alg-viii-s21-n12-rem-3 .statement tag=00O6}

令$\pi_1$和$\pi_2$为有限维向量空间中$G$的线性表示超过$K$。对于$i = 1, 2$，令$\pi_i'$为与$\pi_i$到$\varphi$相关的表示。我们有
$$
\dim_K \operatorname{Hom}_K(\pi_1, \pi_2) = \dim_{K'} \operatorname{Hom}_{K'}(\pi_1', \pi_2') .
$$
证明遵循推论VIII、p. 410，通过简化为$\pi_i$（因而$\pi_i'$）很简单的情况。

#### 注 4 {#alg-viii-s21-n12-rem-4 .statement tag=00O7}

设$H$为基数$m$的$G$子群。从$\mu_m(K)$到$\mu_m(K')$，同构$\varphi$限制到同构，因而，从$R_K(H)$到$R_{K'}(H)$环同构$\varphi_H$。以下图表通勤：

$$
\begin{array}{ccc}
R_K(G) & \xrightarrow{\operatorname{Res}_H^G} & R_K(H) \\
\downarrow \varphi_G & & \downarrow \varphi_H \\
R_{K'}(G) & \xrightarrow{\operatorname{Res}_H^{G'}} & R_{K'}(H) ,
\end{array}
$$

$$
\begin{array}{ccc}
R_K(H) & \xrightarrow{\operatorname{Ind}_H^G} & R_K(G) \\
\downarrow \varphi_H & & \downarrow \varphi_G \\
R_{K'}(H) & \xrightarrow{\operatorname{Ind}_H^{G'}} & R_{K'}(G) .
\end{array}
$$

第一个图表的交换律是显而易见的，第二个弗罗贝尼乌斯互易律和公式是从它得出的（47）。

#### 注 5 {#alg-viii-s21-n12-rem-5 .statement tag=00O8}

假设 G 是两个有限群中的乘积 $G'\times G''$。我们定义同构$\varphi_{G'}$和$\varphi_{G''}$与之前的例一样。

我们有一个可交换的图表

$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')^{\kappa}$ // $R_K(G)$

$\varphi_{G'}\otimes \varphi_{G''}\varphi_G$

$R_{K'}(G')\otimes_{\mathbf{Z}}R_{K'}(G'')^{\kappa'}$ // $R_{K'}(G)$,

其中同构 $\kappa$ 和 $\kappa '$ 是VIII、p. 406 中定义的内容。

### \*13。 复线性表示

在这个小节中，我们假设K是复数的域$\mathbf{C}$。

令 $(M, \pi )$ 为 G 的线性表示。我们说 M 上的厄米特形式 Φ 在 G 下是不变的，如果我们有

$$
\Phi (\pi (g)x, \pi (g)x') = \Phi (x, x') \tag{48}
$$

对于所有 $x, x'\in M$ 和每个 $g\in G$。这也意味着对于每个$g\in G$，M 的自同构$\pi (g)$ 相对于 Φ 是酉的。

#### 命题 11 {#alg-viii-s21-prop-11 .statement tag=00O9}

令 $(M, \pi )$ 为 G 的有限维线性表示。

a) M 厄米特形式上存在正数、分离且在 G 下不变。

b) 假设表示 $\pi$ 很简单。如果 Φ 和 Ψ 在 M 上为非零的厄米特形式，且在 G 下不变，则存在实数 $a$，使得$\Psi  =a\Phi$。

选择向量空间 M 上的分离正厄米特形式，并用$\Phi_0$ 表示。我们定义一个分离正值厄米特形式 Φ，它在 G 下通过设定保持不变

$$
\Phi (x, x') =\sum_{g\in G}\Phi_0(\pi (g)x, \pi (g)x') \tag{49}
$$

$x, x'\in M$。

令 Ψ 为 M 上的厄米特形式； M 存在唯一内同态 A，使得 M 中的 $x, x'$ $\Psi (x, x') = \Phi (x,Ax')$。此外，如果 Ψ 在 G 下不变，则自同态 A 与自同构 $\pi (g)$ $g\in G$ 交换。如果表示 $\pi$ 是简单的，那么根据 Schur 的引理 (VIII, p. 47, 定理 1)，A 是位似，因此存在复数 $a$，使得$\Psi  =a\Phi$。由于 Φ 和 Ψ 为厄米特，Φ 为非零的，因而 $a$ 为实数。接下来是命题。

我们将复数函数的向量空间$\mathbf{C}[G]$赋予G上的希尔伯特空间结构，其内部乘积由下式给出

$$
\langle f|f'\rangle_G=|G|^{-1}\sum_{g\in G}\overline{f(g)}f'(g) \tag{50}
$$

对于任何函数 $f\in \mathbf{C}[G]$，我们用 $f^*$ 函数表示，定义为

$$
f^*(g) =\overline{f(g^{-1})} \tag{51}
$$

$g\in G$； 映射 $f\mapsto f^*$ 是 $\mathbf{C}[G]$ 的半线性对合。我们还有

$$
\langle f|f'\rangle_G=\langle f^*, f'\rangle_G \tag{52}
$$

对于 $f, f'\in \mathbf{C}[G]$，记号公式 (28) VIII，p. 410。因此我们有

$$
\langle f|f'\rangle_G=|G|^{-2}\tau (f^*f') \tag{53}
$$

令$(M, \pi )$为G的有限维线性表示。我们将希尔伯特空间的结构赋予向量空间M，其中自同态$\pi (g)$是酉的（命题11）。如果我们用$A^*$表示M的自同态A对于这个结构的伴随，那么我们有Tr($A^*$)$=$Tr(A)。对于每个$g\in G$，我们有$\pi (g^{-1}) =\pi (g)^*$，因而$\chi_{\pi}(g^{-1}) =\chi_{\pi}(g)$；在其他字中，我们有$\chi_{\pi}=\chi^*_{\pi}$。 正交关系对应特征标 (VIII, p. 410, 命题 4) 那么有形式

$$
\langle \chi_{\lambda}|\chi_\mu\rangle_G=\delta_{\lambda \mu} \tag{54}
$$

$\lambda , \mu\in \widehat{G}$。它表达了这样一个事实：G 的简单表示的特征标$(\chi_{\lambda})_{\lambda\in\widehat{G}}$族是中心函数的希尔伯特空间$Z(\mathbf{C}[G])$的正交基。

令$\pi$和$\pi '$为G的有限维线性表示。我们有关系$\langle \chi_{\pi}|\chi_{\pi'}\rangle_G=$dim$_{\mathbf{C}}$Hom$_G(\pi , \pi ')$（VIII，p. 410，推论）。 表示 $\pi$ 不可约当且仅当$\langle \chi_{\pi}|\chi_{\pi}\rangle_G= 1$。

对于$\widehat{G}$的每个元素$\lambda$，我们赋予向量空间$V_{\lambda}$一个希尔伯特空间的结构，其中自同构$\pi_{\lambda}(g)$是酉的。我们用$V_{\lambda}$的两个元素$v, v'$的$\langle v|v'\rangle_{\lambda}$内部乘积和$u^*$表示$V_{\lambda}$的自同态$u$的伴随。令$A = (A_{\lambda})_{\lambda\in\widehat{G}}$和$A'= (A'_{\lambda})_{\lambda\in\widehat{G}}$为$F(\widehat{G})$中的元素。我们写$A^*= (A^*_{\lambda})_{\lambda\in\widehat{G}}$。 $\mathbf{C}[G]$中每元素$a$就有$\mathscr{F}(a^*) = (\mathscr{F}(a))^*$。 集合 (55) $\langle A|A'\rangle_{\widehat{G}}=|G|^{-2}\widehat{\tau}(A^*A')$。到 VIII、p. 407 的公式 (10)，我们有

(56)$\langle A|A'\rangle_{\widehat{G}}=\frac{1}{|G|^2}\sum_{\lambda\in\widehat{G}}d_{\lambda}$Tr(A$^*_{\lambda}$A$'_{\lambda}$)。

由于 $\widehat{\tau}\circ \mathscr{F}=\tau$、公式 (53) 和 (55) 意味着映射 $\mathscr{F}$ 是希尔伯特空间从 $\mathbf{C}[G]$ 到 $F(\widehat{G})$ 的同构。

Schur正交关系 (VIII, p. 410) 可以使用希尔伯特内部乘积重新表示。 关系 (21) 和 (24) 然后给出以下断言。对于 $V_{\lambda}$ 中的 $\lambda \in \widehat{G}$ 和 $x, x', y, y'$，我们有 (57) $|G|^{-1}\sum_{g\in G}\overline{\langle x|\pi_{\lambda}(g)x'\rangle}_{\lambda}\langle y|\pi_{\lambda}(g)y'\rangle_{\lambda}=d^{-1}_{\lambda}\overline{\langle x|y\rangle}_{\lambda}\langle x'|y'\rangle_{\lambda}$。

如果$\lambda$和$\mu$是$\widehat{G}$的两个不同的元素，那么对于$V_{\lambda}$中的$x, x'$和$V_\mu$中的$y, y'$，我们有(58) $\sum_{g\in G}\overline{\langle x|\pi_{\lambda}(g)x'\rangle}_{\lambda}\langle y|\pi_\mu(g)y'\rangle_\mu= 0$。

对于每个$\lambda \in \widehat{G}$，我们选择是$V_{\lambda}$的正交基$(e_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$。对于任何$g\in G$，我们相对于这个基用$V_{\lambda}$的自同态$\pi_{\lambda}(g)$$(\pi^{\lambda}_{ij}(g))$矩阵来表示；我们有 (59) $\pi^{\lambda}_{ij}(g) =\langle e_{\lambda ,i}|\pi_{\lambda}(g)e_{\lambda ,j}\rangle_{\lambda}$。

由于自同态 $\pi_{\lambda}(g)$ 是酉，其倒数等于 $\pi_{\lambda}(g)^*$，因此 (60) $\overline{\pi^{\lambda}_{ij}(g)}=\pi^{\lambda}_{ji}(g^{-1})$。然后从VIII、p. 409和(25)、p. 409的公式(22)得出函数$(d_{\lambda})^{1/2}\pi_{ij}^{\lambda}$，对于$\lambda \in \widehat{G},1\leqslant i\leqslant d_{\lambda},1\leqslant j\leqslant d_{\lambda}$，形式希尔伯特空间的正交基 $\mathbf{C}[G].*$

### 习题{#alg-viii-s21-exercises}

§ 21](exercises/s21/)参见[习题。

Hom$_G(\pi , \pi ')$的[^1]:元素是有时，称为$\pi$和$\pi '$的交织算子。
