---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 3
section_title: Conjugacy theorems
lang: zh
source: lie-vii-ix
book_pages: 20-27, 57-62
pdf_pages: 0030-0037, 0066-0071
extraction: native
subsections:
    - "no": 1
      title: ELEMENTARY AUTOMORPHISMS
      page: 20
      pdf_page: 30
    - "no": 2
      title: CONJUGACY OF CARTAN SUBALGEBRAS
      page: 22
      pdf_page: 32
    - "no": 3
      title: APPLICATIONS OF CONJUGACY
      page: 24
      pdf_page: 34
    - "no": 4
      title: CONJUGACY OF CARTAN SUBALGEBRAS OF SOLVABLE LIE ALGEBRAS
      page: 25
      pdf_page: 35
    - "no": 5
      title: LIE GROUP CASE
      page: 26
      pdf_page: 36
statements: 17
exercises: 18
content_sha256: 50b06e29ec1b21144dfb809935dd6ad340bcead0d76cb9c902d8fa4fdf070a42
translated_from: content/en/lie/VII/03_s3_conjugacy_theorems.md
translation_method: google
source_content_sha256: 2f94c55e447063be8de93e14acb2f2791b356caa14408181f0dee22d40d924cb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 278a64f9b5e7f4b117196bc01bb1f8205b015d3eba6e259f419c02ae5ebc894f
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。 共轭定理

在本段中，基域$k$的特征为0。

### 1. 小学自同构

设$\mathfrak{g}$为李代数。用Aut($\mathfrak{g}$)表示自同构的群。如果 $x\in \mathfrak{g}$ 且 ad $x$ 幂零的，则 $e^{adx}\in$ Aut($\mathfrak{g}$)（第 I, §6, no. 8 章）。

#### 定义 1 {#lie-vii-s3-def-1 .statement tag=00V0}

乘积 of 自同构 of $\mathfrak{g}$ of 形式 $e^{adx}$ 且 $x$ 幂零称为初等自同构 of $\mathfrak{g}$。 $\mathfrak{g}$的初等自同构的群用Aut$_e(\mathfrak{g})$表示。

如果$u\in$自动（$\mathfrak{g}$）$,ue^{adx}u^{-1}=e^{adu(x)}$。由此可见，Aut$_e(\mathfrak{g})$ 是 Aut($\mathfrak{g}$) 的正常子群。如果$k=\mathbf{R}$或$\mathbf{C}$，则Aut$_e(\mathfrak{g})$包含在$\mathfrak{g}$的内自同构的群Int($\mathfrak{g}$)中(第III, §6, no. 2章，定义2)。

\* 一般情况下，Aut$_e(\mathfrak{g})$ 包含在代数群 Aut($\mathfrak{g}$) 的恒等式分量中。\*

#### 引理 1 {#lie-vii-s3-lem-1 .statement tag=00V1}

令 V 为有限维向量空间，$\mathfrak{n}$ $\mathfrak{a}=\mathfrak{g}\mathfrak{l}(V)$ 由……组成幂零元的谎言子代数。

(i) 映射$x \rightarrow$exp$x$是双射从$\mathfrak{n}$到子群单能元素的$\mathbf{G}\mathbf{L}(V)$由……组成的N（第II, §6, no. 1，注 4).我们有 $\mathfrak{n}=$ log(exp$\mathfrak{n}$)。 映射$f \rightarrow f\circ$对数是同构，从$\mathfrak{n}$上多项式函数的代数到限制的代数到End(V)上的多项式函数N。

(ii) 如果 $x\in \mathfrak{n}$ 和 $a\in \mathfrak{a}$，

(exp ad$_{\mathfrak{a}}x$)$.a=$ (exp $x$)$a$(exp($-x$))。

(iii) 令$V'$为有限维向量空间，$\mathfrak{n}'$是$\mathfrak{g}\mathfrak{l}(V')$由……组成的谎言子代数，幂零元，$\rho$同态从$\mathfrak{n}$到$\mathfrak{n}'$。设$\pi$为映射exp$x \rightarrow$exp$\rho (x)$，从exp$\mathfrak{n}$到exp$\mathfrak{n}'$。那么$\pi$就是群同态。

根据恩格尔的定理，我们将可以确定V与$k^n$相结合，使得$\mathfrak{n}$是$\mathfrak{n}(n, k)$的子代数（下三角$\mathbf{M}_n(k)$由……组成的谎言子代数） 矩阵与零在对角线上）。对于$s\geq 0$，令$\mathfrak{n}_s(n, k)$为$(x_{ij})_{1\leq i,j\leq n}\in \mathbf{M}_n(k)$的集合，使得$x_{ij}= 0$代表$i-j < s$。然后

$$
[\mathfrak{n}_s(n, k),\mathfrak{n}_{s'}(n, k)]\subset \mathfrak{n}_{s+s'}(n, k)
$$

（第 II, §4, no. 6、注），以及从 $\mathfrak{n}(n, k)\times \mathfrak{n}(n, k)$ 到 $\mathfrak{n}(n, k)$ 的 Hausdorff 级数定义多项式映射 $(a, b) \rightarrow H(a, b)$（第 II, §6, no. 5、注） 3）；这个映射使$\mathfrak{n}(n, k)$变成群（第II, §6, no. 5章，提案4）。由章。 II, §6, no. 1、注 4、映射 $x \rightarrow$ exp $x$ 从 $\mathfrak{n}(n, k)$ 到 $1 +\mathfrak{n}(n, k)$ 和 $y \rightarrow$ log $y$ 从 $1 +\mathfrak{n}(n, k)$ 到 $\mathfrak{n}(n, k)$ 是逆双射且是多项式；由章。 II, §6, no. 5，第 3 条，如果给定 $\mathfrak{n}(n, k)$ 群运算 $(a, b) \rightarrow H(a, b)$，并且如果 $1 +\mathfrak{n}(n, k)$ 被视为 $\mathbf{G}\mathbf{L}_n(k)$ 的子群，则这些映射是群的同构。 引理的断言 (i) 和 (iii) 现在如下。让$x\in \mathfrak{n}$。用 $L_x,R_x$ 映射 $u \rightarrow xu, u \rightarrow ux$ 表示从 $\mathfrak{a}$ 到 $\mathfrak{a}$，它们可交换且幂零。我们有广告$_{\mathfrak{a}}x= L_x-R_x$，所以，对于所有$a\in \mathfrak{a}$，

(exp ad$_{\mathfrak{a}}x$)$a=$ (exp(L$_x-R_x$))$a=$ (exp $L_x$)(exp $R_{-x}$)$a$ (1)

$=\sum Li^{ix}$！ $Rj\overset{j-x}{!}a=$（经验$x$）$a$（经验（$-x$））。

$i,j\geq 0$

引理 $1,\pi$ 中的记号称为 exp $\mathfrak{n}$ 的线性表示，与$V'$ 上$\mathfrak{n}$ 的给定表示 $\rho$ 相容的。当 $k$ 为 $\mathbf{R}$、$\mathbf{C}$ 时，或由指数映射的性质得出的非离散完全超度量域、$\rho = L(\pi )$（第 III, §4, no. 4 章，第 8 条的 Cor.2）。

#### 命题 1 {#lie-vii-s3-prop-1 .statement tag=00V2}

令 $\mathfrak{g}$ 为 $\mathfrak{g}$ 的李代数、$\mathfrak{n}$ 子代数，使得 ad$_{\mathfrak{g}}x$ 对于所有 $x\in \mathfrak{n}$ 是幂零的。那么$e^{ad_{\mathfrak{g}}\mathfrak{n}}$就是Aut$_e(\mathfrak{g})$的子群。

这紧随引理 1 (i)。

特别是，如果$\mathfrak{n}$是$\mathfrak{g},e^{ad_{\mathfrak{g}}\mathfrak{n}}$的幂零根基，则群是$\mathfrak{g}$的特殊自同构（第I, §6, no. 8章，定义6）。

#### 注 1 {#lie-vii-s3-n1-rem-1 .statement tag=00V3}

令V为有限维向量空间，$\mathfrak{g}$为$\mathfrak{a}=\mathfrak{g}\mathfrak{l}$(V)的谎言子代数，$x$元素为$\mathfrak{g}$，使得ad$_{\mathfrak{g}}x$为零。那么存在$\mathfrak{a}$的幂零元$n$使得ad$_{\mathfrak{a}}n$扩展ad$_{\mathfrak{g}}x$。事实上，令$s, n$为半单且分量为$x$；那么 ad$_{\mathfrak{a}}s$ 和 ad$_{\mathfrak{a}}n$ 是半单且 ad$_{\mathfrak{a}}x$ 的幂零分量（第 I, §5, no. 4，引理 2），因而 ad$_{\mathfrak{a}}s$ 和 ad$_{\mathfrak{a}}n$ 使 $\mathfrak{g}$ 保持稳定，并且ad$_{\mathfrak{a}}s|\mathfrak{g}$和ad$_{\mathfrak{a}}n|\mathfrak{g}$是ad$_{\mathfrak{g}}x$的半单和幂零分量；因而，ad$_{\mathfrak{g}}x=$ ad$_{\mathfrak{a}}n|\mathfrak{g}$，这证明了我们的断言。鉴于引理 1 (ii)，$\mathfrak{g}$扩展的每个初等自同构到形式$u \rightarrow mum^{-1}$的$\mathfrak{a}$自同构，其中$m\in \mathbf{G}\mathbf{L}(V)$。

#### 注 2 {#lie-vii-s3-n1-rem-2 .statement tag=00V4}

令 V 为有限维向量空间。对于所有$g\in \mathbf{S}\mathbf{L}$(V)，令$\varphi (g)$为自同构$x \rightarrow gxg^{-1}$除以$\mathfrak{g}\mathfrak{l}(V)$。然后

自动$_e(\mathfrak{g}\mathfrak{l}(V)) =\varphi (\mathbf{S}\mathbf{L}(V))$。

事实上，根据（1），Aut$_e(\mathfrak{g}\mathfrak{l}(V))$包含在$\varphi (\mathbf{S}\mathbf{L}$（V））中，并且相反的包含来自第1章的代数。 III, §8, no. 9，提案 17 和 (1)。类似的论证表明Aut$_e(\mathfrak{s}\mathfrak{l}(V))$是$\varphi (\mathbf{S}\mathbf{L}(V))$元素到$\mathfrak{s}\mathfrak{l}(V)$限制集合。

### 2. 嘉当子代数的共轭

令 $\mathfrak{g}$ 为李代数，$\mathfrak{h}$ $\mathfrak{g}$ 的幂零子代数，以及 $\mathfrak{g}$ 中 $\mathfrak{h}$ 的非零权的 R 集合，其他字 $\mathfrak{h}$ 上的线性形式 $\lambda \not= 0$ 的集合，使得 $\mathfrak{g}^{\lambda}(\mathfrak{h})\not= 0$、cf. §1, no. 3，提案 9 (iii)。假设

$$
\mathfrak{g}=\mathfrak{g}^0(\mathfrak{h})\oplus \sum_{\lambda\in R}\mathfrak{g}^{\lambda}(\mathfrak{h})
$$

如果 $k$ 是代数封闭的，就是这种情况（§1, no. 3，命题 9 (i)）。对于 $\lambda \in R$ 和 $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$，ad $x$ 是幂零的（§1, no. 3，命题 10 (iv)）。用$e^{adx}$生成的Aut$_e(\mathfrak{g})$的$E(\mathfrak{h})$子群表示，其中$x$是上面的形式。如果$u\in$Aut($\mathfrak{g}$)，则$uE(\mathfrak{h})u^{-1}= E(u(\mathfrak{h}))$就是直接的。

#### 引理 2 {#lie-vii-s3-lem-2 .statement tag=00V5}

(i) 设$\mathfrak{h}_r$为$x\in \mathfrak{h}$的集合，使得$\mathfrak{g}^0(x) =\mathfrak{g}^0(\mathfrak{h})$；这是 $x\in \mathfrak{h}$ 的集合，使得 $\lambda (x)\not= 0$ 对于所有 $\lambda \in R$，并且 $\mathfrak{h}_r$ 在 Zariski 拓扑中的 $\mathfrak{h}$ 中是开放且密集的。

(ii) 将 $R =\{\lambda_1, \lambda_2, . . . , \lambda_p\}$ 放入$\lambda_i$ 相互不同的位置。令 F 为由公式定义的从 $\mathfrak{g}^0(\mathfrak{h})\times \mathfrak{g}^{\lambda_1}(\mathfrak{h})\times  \cdots  \times \mathfrak{g}^{\lambda_p}(\mathfrak{h})$ 到 $\mathfrak{g}$ 的映射

$$
F(h, x_1, . . . , x_p) =e^{adx_1}. . . e^{adx_p}h
$$

那么 F 就是支配多项式映射（App.I）。

断言 (i) 很清楚。我们证明(ii)。让$n=$变暗$\mathfrak{g}$。如果 $\lambda \in R$ 和 $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$，我们有 (ad $x$)$^n= 0$。由此可见，$(y, x) \rightarrow e^{adx}y$是从$\mathfrak{g}\times \mathfrak{g}^{\lambda}(\mathfrak{h})$到$\mathfrak{g}$的多项式映射；由归纳可知F是多项式。设$h_0\in \mathfrak{h}_r$，DF为F在$(h_0,0, . . . ,0)$处的切线映射；我们证明 DF 是满射的。对于 $h\in \mathfrak{g}^0(\mathfrak{h}), F(h_0+h,0, . . . ,0) =h_0+h$，因此 DF($h,0, . . . ,0$) $=h$ 和 Im(DF) $\supset \mathfrak{g}^0(\mathfrak{h})$。另一方面，对于 $x\in \mathfrak{g}^{\lambda_1}(\mathfrak{h})$，

$F(h_0, x,0, . . . ,0) =e^{adx}h_0=h_0+$（广告$x$）$.h_0+$（广告2！$x$）$^2h_0+\cdots$

所以DF(0$, x,0, . . . ,0$)$=$(广告$x$)$.h_0=-$(广告$h_0$)$x$;自从广告 $h_0$ 诱导自同构 $\mathfrak{g}^{\lambda_1}(\mathfrak{h})$ 以来，Im(DF) $\supset \mathfrak{g}^{\lambda_1}(\mathfrak{h})$。同样，

我(DF) $\supset \mathfrak{g}^{\lambda_i}(\mathfrak{h})$

对于所有 $i$，因此 DF 具有满射性。应用程序的第 4 项提案。 I 现在表明 F 占主导地位。

#### 命题 2 {#lie-vii-s3-prop-2 .statement tag=00V6}

假设 $k$ 是代数闭的。令$\mathfrak{g}$为$\mathfrak{g}$的李代数、$\mathfrak{h}$和$\mathfrak{h}'$嘉当子代数。存在$u\in E(\mathfrak{h})$和$u'\in E(\mathfrak{h}')$使得$u(\mathfrak{h}) =u'(\mathfrak{h}')$。

我们保留引理 2 中的记号。根据$\mathfrak{h}$和$\mathfrak{h}'$是嘉当子代数，可以得出$\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$和$\mathfrak{g}^0(\mathfrak{h}') =\mathfrak{h}'$。根据 App 的引理 2 和 Prop. 3。 $I, E(\mathfrak{h})\mathfrak{h}_r$ 和 $E(\mathfrak{h}')\mathfrak{h}'_r$ 包含在 Zariski 拓扑中打开密集的子集 $\mathfrak{g}$。因此$E(\mathfrak{h})\mathfrak{h}_r\cap E(\mathfrak{h}')\mathfrak{h}'_r\not=\emptyset$。在其他字中，存在$u\in E(\mathfrak{h}), u'\in E(\mathfrak{h}'), h\in \mathfrak{h}_r, h'\in \mathfrak{h}'_r$使得$u(h) =u'(h')$；然后

$$
u(\mathfrak{h}) =u(\mathfrak{g}^0(\mathfrak{h})) =\mathfrak{g}^0(u(h)) =\mathfrak{g}^0(u'(h')) =u'(\mathfrak{h}')
$$

#### 推论 {#lie-vii-s3-n2-cor-1 .statement tag=00V7}

$E(\mathfrak{h}) = E(\mathfrak{h}')$。

令 $u, u'$ 如命题 2 所示。那么

$$
E(\mathfrak{h}) =uE(\mathfrak{h})u^{-1}= E(u(\mathfrak{h})) = E(u'(\mathfrak{h}')) =u'E(\mathfrak{h}')u^{'-1}= E(\mathfrak{h}')
$$

因此推论。

由于这个结果，如果 $k$ 是代数封闭的，我们将简单地表示为 E 群 $E(\mathfrak{h})$，其中 $\mathfrak{h}$ 是 $\mathfrak{g}$ 的嘉当子代数。

一般来说，Aut$_e(\mathfrak{g})\not= E$（例如，如果$\mathfrak{g}$是幂零的，则E约化到单位元素，甚至虽然非平凡初等自同构也存在，前提是$\mathfrak{g}$是不可交换的）。然而，可以证明（第 VIII, §10，练习 5）Aut$_e(\mathfrak{g}) = E$ 对于 $\mathfrak{g}$ 半单。

#### 定理 1 {#lie-vii-s3-thm-1 .statement tag=00V8}

假设 $k$ 是代数闭的。令$\mathfrak{g}$为李代数。 群 E 在 Aut($\mathfrak{g}$) 中是正规的，并且在 $\mathfrak{g}$ 的嘉当子代数的集合上传递操作。

令$\mathfrak{h}$为$\mathfrak{g}$的嘉当子代数，以及$v\in$Aut($\mathfrak{g}$)。然后

$$
vE(\mathfrak{h})v^{-1}= E(v(\mathfrak{h})) = E(\mathfrak{h})
$$

所以 $E(\mathfrak{h}) = E$ 在 Aut($\mathfrak{g}$) 中是正常的。如果$\mathfrak{h}'$是$\mathfrak{g}$的另一个嘉当子代数，那么，在提案$2,u^{'-1}u(\mathfrak{h}) =\mathfrak{h}'$的记号和$u^{'-1}u\in E$中。

### 3. 共轭的应用

#### 定理 2 {#lie-vii-s3-thm-2 .statement tag=00V9}

设$\mathfrak{g}$为李代数。

(i) $\mathfrak{g}$的嘉当子代数都是相同的维数，即rk($\mathfrak{g}$)，以及相同的幂零性类。

(ii) 元素 $x\in \mathfrak{g}$ 是正则当且仅当 $\mathfrak{g}^0(x)$ 是 $\mathfrak{g}$ 的嘉当子代数；每一个嘉当子代数都是这样得到的。

为了证明 (i)，我们可以假设 $k$ 是代数封闭的（cf. §2，命题 3 和命题 6），在这种情况下，它由 Th 推出。 no. 2 中的 1 个。 断言 (ii) 由 (i) 和 §2, Th 得出。 1(i)和(iv)。

#### 命题 3 {#lie-vii-s3-prop-3 .statement tag=00VA}

令$\mathfrak{g}$为李代数，$\mathfrak{g}'$子代数等于$\mathfrak{g}$。以下条件是等效的：

(i) $\mathfrak{g}$的$\mathfrak{g}'$包含正则元素，以及rk($\mathfrak{g}$)$=$rk($\mathfrak{g}'$)；

(ii) $\mathfrak{g}$ 中的$\mathfrak{g}'$ 包含嘉当子代数；

(iii) $\mathfrak{g}'$ 中的每个嘉当子代数是 $\mathfrak{g}$ 中的嘉当子代数。

(i)$=\Rightarrow$(ii)：假设rk($\mathfrak{g}$)$=$rk($\mathfrak{g}'$)，且$\mathfrak{g}$中存在$x\in \mathfrak{g}'$正则。把$\mathfrak{h}=\mathfrak{g}^0(x),\mathfrak{h}'={\mathfrak{g}'}^0(x) =\mathfrak{h}\cap \mathfrak{g}'$。然后

rk($\mathfrak{g}'$)$\leq$ 暗淡$\mathfrak{h}'\leq$ 暗淡$\mathfrak{h}=$ rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$)

所以$\mathfrak{h}=\mathfrak{h}'\subset \mathfrak{g}'$。这就证明了(ii)。

(ii)$=\Rightarrow$(iii)：假设$\mathfrak{g}$中的$\mathfrak{g}'$包含嘉当子代数$\mathfrak{h}$，并令$\mathfrak{h}_1$为$\mathfrak{g}'$中的嘉当子代数。为了证明$\mathfrak{h}_1$是$\mathfrak{g}$的嘉当子代数，我们可以假设$k$是代数封闭的。令$E(\mathfrak{h})$和$E'(\mathfrak{h})$为与$\mathfrak{h}$(no. 2)相关联的$\mathfrak{g}$和$\mathfrak{g}'$的自同构中的群。由 Th. 1、存在$f\in E'(\mathfrak{h})$使得$f(\mathfrak{h}) =\mathfrak{h}_1$。现在$E'(\mathfrak{h})$的每一个元素都是由$E(\mathfrak{h})$的元素诱发；事实上，用$x\in {\mathfrak{g}'}^{\lambda}(\mathfrak{h}),\lambda \not= 0$验证$e^{adx}$就足够了，在这种情况下，它可以从包含${\mathfrak{g}'}^{\lambda}(\mathfrak{h})\subset \mathfrak{g}^{\lambda}(\mathfrak{h})$得出。因此$\mathfrak{h}_1$是$\mathfrak{g}$的嘉当子代数。

(iii)$=\Rightarrow$(i)：假设满足条件(iii)。令 $\mathfrak{h}$ 为 $\mathfrak{g}'$ 中的嘉当子代数。由于这是 $\mathfrak{g}$ 的嘉当子代数，因此它是 $\mathfrak{g}$ 的包含正则元素 (Th. 2 (ii))，而另一方面 rk($\mathfrak{g}$) $=$ 暗淡($\mathfrak{h}$) $=$ rk($\mathfrak{g}'$)。

#### 推论 {#lie-vii-s3-n3-cor-1 .statement tag=00VB}

令$\mathfrak{h}$为$\mathfrak{g}$的幂零子代数。 子代数 $\mathfrak{g}^0(\mathfrak{h})$ 具有命题 3 中的属性 (i)、(ii)、(iii)。

事实上，§2, no. 3的第11条命题表明$\mathfrak{g}^0(\mathfrak{h})$有性质 (ii)。

#### 命题 4 {#lie-vii-s3-prop-4 .statement tag=00VC}

令$\mathfrak{g}$为李代数，$\mathfrak{g},c$的$l$秩，$\mathfrak{g}$的嘉当子代数的幂幂类，以及$x\in \mathfrak{g}$。存在$\mathfrak{g}$的$l$维子代数，其幂零性类为$\leq c$，且包含$x$。

设 T 为不定式。令$k'=k(T)$和$\mathfrak{g}'=\mathfrak{g}\otimes_kk'$。如果$\mathfrak{h}$是$\mathfrak{g},\mathfrak{h}\otimes_kk'$的嘉当子代数是$\mathfrak{g}'$的嘉当子代数，因此$\mathfrak{g}'$的秩是$l$并且$\mathfrak{g}'$的嘉当子代数的幂零性类是$c$。

选择正则元素$y$共$\mathfrak{g}$。有了记号和 §2, no. 2，我们就有 $a_l(y)\not= 0$。还用 $\mathfrak{g}'$ 上的 $a_l$ 多项式函数表示扩展 $a_l$。那么$k[T]$的元素$a_l(x+ Ty)$占主导地位系数$a_l(y)$。特别是，$x+ Ty$在$\mathfrak{g}'$中是规则的。令$\mathfrak{h}'$为$\mathfrak{g}'$中ad($x+ Ty$)的零空间。那么暗淡$\mathfrak{h}'=l$，$\mathfrak{h}'$的幂零性类是$c$。把$\mathfrak{k}=\mathfrak{h}'\cap (\mathfrak{g}\otimes_kk[T])$；然后$\mathfrak{k}\otimes_{k[T]}k(T) =\mathfrak{h}'$。

令$\varphi$为从$k[T]$到$k$的同态，使得$\varphi (T) = 0$，并且令$\psi$为从$\mathfrak{g}\otimes_kk[T]$到$\mathfrak{g}$的同态$1\otimes \varphi$。那么$\psi (\mathfrak{k})$是$\mathfrak{g}$的子代数，其幂零性类是$\leq c$，并且包含$\psi (x+ Ty) =x$。

在自由$k$[T]-模$\mathfrak{g}\otimes_kk[T],\mathfrak{k}$是秩$l$的子模，$(\mathfrak{g}\otimes_kk[T])/\mathfrak{k}$是挠元自由，所以子模$\mathfrak{k}$是$\mathfrak{g}\otimes_kk[T] ($代数，第 1 章VII, §4, no. 2，周四。 1).因此，dim$_k\psi (\mathfrak{k}) =l$，即完成证明。

### 4. 可解李代数的嘉当子代数共轭

设$\mathfrak{g}$为可解李代数。用$\mathfrak{g}$的下降中央级数的项的$\mathscr{C}^{\infty}(\mathfrak{g})$交（第I, §1, no. 5章）表示。这是$\mathfrak{g}$的特征理想，并且是$\mathfrak{g}$的最小的理想$\mathfrak{m}$，使得$\mathfrak{g}/\mathfrak{m}$幂零的。由于$\mathscr{C}^{\infty}(\mathfrak{g})\subset [\mathfrak{g},\mathfrak{g}],\mathscr{C}^{\infty}(\mathfrak{g})$是$\mathfrak{g}$的幂零理想（第I, §5, no. 3章，Th.1的Cor.5）。根据no. 1的第1条，$e^{adx}$的集合，对于$x\in \mathscr{C}^{\infty}(\mathfrak{g})$，是包含在特殊自同构的群中的Aut($\mathfrak{g}$)的子群（第I, §6, no. 8章，定义6）。

#### 定理 3 {#lie-vii-s3-thm-3 .statement tag=00VD}

令$\mathfrak{g}$为可解李代数，令$\mathfrak{h},\mathfrak{h}'$为$\mathfrak{g}$的嘉当子代数。存在$x\in \mathscr{C}^{\infty}(\mathfrak{g})$使得$e^{adx}\mathfrak{h}=\mathfrak{h}'$。

我们通过归纳对dim$\mathfrak{g}$进行争论，在这种情况下$\mathfrak{g}= 0$是微不足道的。令 $\mathfrak{n}$ 为 $\mathfrak{g}$ 的最小非零交换理想。令 $\varphi :\mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{n}$ 为规范的态射。然后$\varphi (\mathscr{C}^{\infty}\mathfrak{g}) =\mathscr{C}^{\infty}(\mathfrak{g}/\mathfrak{n})$（第I, §1, no. 5章，第4条命题）。由于$\varphi (\mathfrak{h})$和$\varphi (\mathfrak{h}')$是$\mathfrak{g}/\mathfrak{n}($§2, no. 1的嘉当子代数，Cor.命题 4 的第 2 条），根据归纳假设，存在$x\in \mathscr{C}^{\infty}(\mathfrak{g})$使得$e^{ad\varphi(x)}\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$。 替换$\mathfrak{h}$乘以$e^{adx}\mathfrak{h}$，我们可以假设$\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$，在其他字中

$$
\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}
$$

那么$\mathfrak{h}$和$\mathfrak{h}'$就是$\mathfrak{h}+\mathfrak{n}$的嘉当子代数。若$\mathfrak{h}+\mathfrak{n}\not=\mathfrak{g}$，由归纳假设可证断言。从现在开始假设$\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}=\mathfrak{g}$。

通过 $\mathfrak{n}, [\mathfrak{g},\mathfrak{n}] =\{0\}$ 或 $[\mathfrak{g},\mathfrak{n}] =\mathfrak{n}$ 的最小值。如果$[\mathfrak{g},\mathfrak{n}] =\{0\}$，则$\mathfrak{n}\subset \mathfrak{h}$和$\mathfrak{n}\subset \mathfrak{h}'($§2, no. 1，命题5），所以$\mathfrak{h}=\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}=\mathfrak{h}'$。仍然需要考虑$[\mathfrak{g},\mathfrak{n}] =\mathfrak{n}$，所以$\mathfrak{n}\subset \mathscr{C}^{\infty}(\mathfrak{g})$的情况。理想的$\mathfrak{n}$是一个简单的$\mathfrak{g}$模块；从$\mathfrak{g}=\mathfrak{h}+\mathfrak{n}$开始，从$[\mathfrak{n},\mathfrak{n}] =\{0\}$开始，$\mathfrak{n}$是一个简单的$\mathfrak{h}$模块。如果$\mathfrak{h}\cap \mathfrak{n}\not=\{0\}$，则$\mathfrak{n}\subset \mathfrak{h}$，所以$\mathfrak{g}=\mathfrak{h}$和$\mathfrak{h}'=\mathfrak{h}$。现在假设$\mathfrak{h}\cap \mathfrak{n}=\{0\}$。然后$\mathfrak{g}=\mathfrak{h}\oplus \mathfrak{n}$，因此$\mathfrak{g}=\mathfrak{h}'\oplus \mathfrak{n}$，因为$\mathfrak{h}$和$\mathfrak{h}'$具有相同的维数。

对于所有$x\in \mathfrak{h}$，令$f(x)$为$\mathfrak{n}$的唯一元素，使得$x-f(x)\in \mathfrak{h}'$；如果$x, y\in \mathfrak{h}$，

$$
[x, y]-[x, f(y)]-[f(x), y] = [x-f(x), y-f(y)]\in \mathfrak{h}'
$$

所以$f([x, y]) = [x, f(y)] + [f(x), y]$。由 §1, no. 3 提供，Cor.根据第 9 条命题，存在 $a\in \mathfrak{n}$，使得 $f(x) = [x, a]$ 对于所有 $x\in \mathfrak{h}$。我们有 (ad $a$)$^2(\mathfrak{g})\subset$ (ad $a$)$(\mathfrak{n}) = 0$，因此，对于所有 $x\in \mathfrak{h}$，

$$
e^{ada}x=x+ [a, x] =x-f(x)
$$

因此$e^{ada}(\mathfrak{h}) =\mathfrak{h}'$。从$a\in \mathscr{C}^{\infty}(\mathfrak{g})$开始，这完成了证明。

#### 引理 3 {#lie-vii-s3-lem-3 .statement tag=00VE}

令$\mathfrak{g}$为李代数，$\mathfrak{r}$其根基，$\varphi$典范同态，从$\mathfrak{g}$到$\mathfrak{g}/\mathfrak{r},v$是$\mathfrak{g}/\mathfrak{r}$的初等自同构。存在 $\mathfrak{g}$ 的初等自同构 $u$ 使得$\varphi \circ u=v\circ \varphi$。

我们可以假设$v$是形式$e^{adb}$，其中$b\in \mathfrak{g}/\mathfrak{r}$和ad$b$是幂零的。令$\mathfrak{s}$为$\mathfrak{g}$的列维子代数（第I, §6, no. 8章，定义7），并令$a$为$\mathfrak{s}$的元素，使得$\varphi (a) =b$。由于 ad$_{\mathfrak{s}}a$ 是幂零的，所以 ad$_{\mathfrak{g}}a$ 也是幂零的（第 I, §6, no. 3 章，第 3 条命题），并且 $u=e^{ad_{\mathfrak{g}}a}$ 是 $\mathfrak{g}$ 的初等自同构，使得 $\varphi \circ u=v\circ \varphi$。

#### 命题 5 {#lie-vii-s3-prop-5 .statement tag=00VF}

设$\mathfrak{g}$为李代数，$\mathfrak{r}$为$\mathfrak{g}$的根基，$\mathfrak{h}$和$\mathfrak{h}'$嘉当子代数，以及$\mathfrak{g}$的$\varphi$典范同态到$\mathfrak{g}/\mathfrak{r}$。以下条件是等效的：

(i) $\mathfrak{h}$ 和 $\mathfrak{h}'$ 通过基本自同构 $\mathfrak{g}$ 等于共轭；

(ii) $\varphi (\mathfrak{h})$ 和 $\varphi (\mathfrak{h}')$ 通过基本自同构 $\mathfrak{g}/\mathfrak{r}$ 等于共轭。

(i) $=\Rightarrow$ (ii)：这很清楚。

(ii) $=\Rightarrow$ (i)：我们假设条件 (ii) 满足并证明(i)。到引理 3，我们就减少到$\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$的情况。放入$\mathfrak{k}=$$\mathfrak{h}+\mathfrak{r}=\mathfrak{h}'+\mathfrak{r}$，这是$\mathfrak{g}$的可解子代数。那么$\mathfrak{h}$和$\mathfrak{h}'$是$\mathfrak{k}$的嘉当子代数，因此存在$x\in \mathscr{C}^{\infty}(\mathfrak{k})$使得$e^{ad_{\mathfrak{k}}x}\mathfrak{h}=\mathfrak{h}'$（Th.3）。由于 $\mathfrak{k}/\mathfrak{r}$ 幂零，$\mathscr{C}^{\infty}(\mathfrak{k})\subset \mathfrak{r}$；另一方面，$\mathscr{C}^{\infty}(\mathfrak{k})\subset [\mathfrak{k},\mathfrak{k}]\subset [\mathfrak{g},\mathfrak{g}]$，所以$x\in \mathfrak{r}\cap [\mathfrak{g},\mathfrak{g}]$；由章。 I, §5, no. 3，周四。 1、ad$_{\mathfrak{g}}x$是幂零的，所以$e^{ad_{\mathfrak{g}}x}$是$\mathfrak{g}$的初等自同构，将$\mathfrak{h}$变换为$\mathfrak{h}'$。

### 5. 李群情形

#### 命题 6 {#lie-vii-s3-prop-6 .statement tag=00VG}

假设$k$是$\mathbf{R},\mathbf{C}$或特征为0的非离散完全超度量域。令$G$是$k,e$上的有限维李群其单位元素，$\mathfrak{g}$其李代数，$\mathfrak{h}$ $\mathfrak{g},\mathfrak{h}_r$嘉当子代数$\mathfrak{g}$属于正则元素集合至$\mathfrak{h}$。

(i) 令$\mathfrak{s}$为定义指数映射的$\mathfrak{s}$中0的$\mathfrak{g},\mathfrak{s}_0$邻域中$\mathfrak{h}$的向量空间补码，以及$h_0\in \mathfrak{h}_r$。 映射 $(s, h) \rightarrow F(s, h) =$（扩展至 $s$）$.h$ 从 $\mathfrak{s}_0\times \mathfrak{h}$ 到 $\mathfrak{g}$ 的路线为 $(0, h_0)$。

(ii) 映射 $(g, h) \rightarrow F'(g, h) =$ (Ad $g$)$.h$ 从 $G\times \mathfrak{h}_r$ 到 $\mathfrak{g}$ 是浸没。特别是它的像$\Omega$是开放的。对于 Ad(G) 下的所有 $x\in \Omega ,\mathfrak{g}^0(x)$ 而言，$\mathfrak{g}$ 共轭至 $\mathfrak{h}$ 中的嘉当子代数。

(iii)设$h_0\in \mathfrak{h}_r$。对于 G 中 $e$ 的任意邻域 U，集合 $\bigcup_{a\in U}$(Ad $a$)$(\mathfrak{h}_r)$

是$\mathfrak{g}$中$h_0$的邻域。

令$h_0$和$\mathfrak{s}$如(i)中所示。令 T 为 F 在 $(0, h_0)$ 处的切线映射。然后$F(0, h) =h$代表所有$h\in \mathfrak{h}$，所以$T(0, h) =h$代表所有$h\in \mathfrak{h}$。另一方面，对于$\mathfrak{s}_0$足够小，映射$s \rightarrow$exp和$s$从$\mathfrak{s}_0$到End($\mathfrak{g}$)在0处的切线映射是映射$s \rightarrow$和$s$ $\mathfrak{s}$ 至结束（$\mathfrak{g}$）。因此 $T(s,0) = [s, h_0]$ 对于所有$s\in \mathfrak{s}$。现在，由 ad $h_0$ 通过到商诱导的从 $\mathfrak{g}/\mathfrak{h}$ 到 $\mathfrak{g}/\mathfrak{h}$ 的映射是双射的。由此可知 T 是双射的，因此 (i)。由于所有 $s\in \mathfrak{s}$ 的 exp ad $s=$ Ad exp $s$ 都足够接近 0，因此 (iii) 和 (ii) 的第一个断言如下。每个 $x\in \Omega$ 都是形式 (广告 $a$)$(h)$ 以及 $a\in G$ 和 $h\in \mathfrak{h}_r$，因此 $\mathfrak{g}^0(x) =$ (广告 $a$)$(\mathfrak{g}^0(h)) =$ (广告 $a$)$(\mathfrak{h})$ 是Ad(G) 下的子代数共 $\mathfrak{g}$ 共轭至 $\mathfrak{h}$。

### 习题 {#lie-vii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
