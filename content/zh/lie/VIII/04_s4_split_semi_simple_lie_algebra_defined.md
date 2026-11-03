---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 4
section_title: Split semi-simple Lie algebra defined by a reduced root system
lang: zh
source: lie-vii-ix
book_pages: 95-106, 231-233
pdf_pages: 0103-0114, 0239-0241
extraction: native
subsections:
    - "no": 1
      title: FRAMED SEMI-SIMPLE LIE ALGEBRAS
      page: 95
      pdf_page: 103
    - "no": 2
      title: A PRELIMINARY CONSTRUCTION
      page: 96
      pdf_page: 104
    - "no": 3
      title: EXISTENCE THEOREM
      page: 100
      pdf_page: 108
    - "no": 4
      title: UNIQUENESS THEOREM
      page: 104
      pdf_page: 112
statements: 23
exercises: 7
content_sha256: 94523059fd25b4052fce601dd72251f924a968ed8e16b215291b4540de97bf3f
translated_from: content/en/lie/VIII/04_s4_split_semi_simple_lie_algebra_defined.md
translation_method: google
source_content_sha256: d31efd9ddbb6c9db525488b6ea28a82ed909217def1e86239e848957a5f5eb01
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 396b571201ca38a7edf7cf4e8e6d8a317e8c4ff92205b097bb4b88d259188440
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 4。 分裂的半单李代数由约化根系定义

### 1. 镶框半单李代数

#### 命题 1 {#lie-viii-s4-prop-1 .statement tag=010T}

设$(\mathfrak{g},\mathfrak{h})$为分裂的半单李代数，R为根系，R的B基，$(n(\alpha , \beta ))_{\alpha ,\beta\in B}$相应的嘉当矩阵。对于所有$\alpha \in B$，设$X_{\alpha}\in \mathfrak{g}^{\alpha}, X_{-\alpha}\in \mathfrak{g}^{-\alpha}$。那么，对于 $\alpha , \beta \in B$，

$$
[H_{\alpha}, H_{\beta}] = 0 \tag{1}
$$

$$
[H_{\alpha}, X_{\beta}] =n(\beta , \alpha )X_{\beta} \tag{2}
$$

$$
[H_{\alpha}, X_{-\beta}] =-n(\beta , \alpha )X_{-\beta} \tag{3}
$$

$[X_{-\alpha}, X_{\beta}] = 0$ 如果 $\alpha \not=\beta$ (4)

(广告$X_{\alpha}$)$^{1-n(\beta ,\alpha)}X_{\beta}= 0$如果$\alpha \not=\beta$ (5)

（广告$X_{-\alpha}$）$^{1-n(\beta ,\alpha)}X_{-\beta}= 0$如果$\alpha \not=\beta$。 (6)

家庭$(H_{\alpha})_{\alpha\in B}$是$\mathfrak{h}$中的基。如果$X_{\alpha}\not= 0$和$X_{-\alpha}\not= 0$对于所有$\alpha \in B$，李代数$\mathfrak{g}$由$X_{\alpha}$和$X_{-\alpha}(\alpha \in B)$生成。

（回想一下，如果 $\alpha , \beta \in B$ 和 $\alpha \not=\beta ,n(\beta , \alpha )$ 是整数 $\leq 0$，那么公式 (5) 和 (6) 就有意义。）

公式 (1)、(2)、(3) 清楚。如果$\alpha \not=\beta ,\beta -\alpha$不是根，因为R的每个元素都是B的元素的线性组合，并且整数系数都具有相同的符号（第VI, §1, no. 6，第3章）。这就证明了(4)。鉴于章。 VI, §1, no. 3，命题9，这也证明了$\beta$定义的$\alpha$链是

$$
\{\beta , \beta +\alpha , . . . , \beta -n(\beta , \alpha )\alpha \}
$$

因此$\beta +(1-n(\beta , \alpha ))\alpha  \notin R$，证明了(5)。 等式 (6) 类似地成立。族$(H_{\alpha})_{\alpha\in B}$是$R^{\vee}$的基，因此也是$\mathfrak{h}$。如果 $X_{\alpha}\not= 0$ 和 $X_{-\alpha}\not= 0$ 对于所有 $\alpha \in B$，则 $[X_{\alpha}, X_{-\alpha}] =\lambda_{\alpha}H_{\alpha}$ 与 $\lambda_{\alpha}\not= 0$，因此最后一个断言由 §3, no. 3 得出，命题 9 (iii)。

#### 定义 1 {#lie-viii-s4-def-1 .statement tag=010U}

设$(\mathfrak{g},\mathfrak{h})$为分裂的半单李代数，R为根系。 A framing of $(\mathfrak{g},\mathfrak{h})$ is a pair $(B,(X_{\alpha})_{\alpha\in B})$, where B is a basis of R, and where, for all $\alpha \in B,X_{\alpha}$ is a non-zero element of $\mathfrak{g}^{\alpha}$. 框架半单李代数是序列$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$，其中$(\mathfrak{g},\mathfrak{h})$是分裂的半单李代数，而$(B,(X_{\alpha})_{\alpha\in B})$是$(\mathfrak{g},\mathfrak{h})$的框架。

$\mathfrak{g}$ 的框架是$(\mathfrak{g},\mathfrak{h})$ 的框架，其中$\mathfrak{h}$ 是$\mathfrak{g}$ 的分裂嘉当子代数。

让$a_1= (\mathfrak{g}_1,\mathfrak{h}_1,B_1,(X_{\alpha}^1)_{\alpha\in B_1})$和$a_2= (\mathfrak{g}_2,\mathfrak{h}_2,B_2,(X_{\alpha}^2)_{\alpha\in B_2})$被框定为半单李代数。 从$a_1$到$a_2$的同构是从$\mathfrak{g}_1$到$\mathfrak{g}_2$的同构$\varphi$，这需要$\mathfrak{h}_1$到$\mathfrak{h}_2, B_1$到$B_2$，以及$X_{\alpha}^1$到$X_{\psi \alpha}^2$ $\alpha \in B_1$（其中$\psi$是$\varphi |\mathfrak{h}_1$的同余映射）。 在这种情况下，$\varphi$被称为变换，框架$(B_1,(X_{\alpha}^1)_{\alpha\in B_1})$到框架$(B_2,(X_{\alpha}^2)_{\alpha\in B_2})$。

如果$(B,(X_{\alpha})_{\alpha\in B})$是$(\mathfrak{g},\mathfrak{h})$的框架，则对于$\mathfrak{g}^{-\alpha}$的所有$\alpha \in B$、唯一元素$X_{-\alpha}$，存在$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}($§2, no. 2、Th。 1（四））。 $(X_{\alpha})_{\alpha\in B\cup(-B)}$族被称为由框架（cf. Prop.1）定义的生成的族。这也是由框架$(-B,(X_{\alpha})_{\alpha\in -B})$定义的生成的族。对于所有$\alpha \in B\cup (-B)$，令$t_{\alpha}\in k^*$，并假设$t_{\alpha}t_{-\alpha}= 1$对于所有$\alpha \in B$。那么$(t_{\alpha}X_{\alpha})_{\alpha\in B\cup(-B)}$就是由框架$(B,(t_{\alpha}X_{\alpha})_{\alpha\in B})$定义的生成的族。

### 2. 一个预备构造

在这个数和下一个向量空间V中，我们用R约化根系表示，并用R的B基表示。我们用$(n(\alpha , \beta ))_{\alpha ,\beta\in B}$表示相对于B的嘉当矩阵。回想一下$n(\alpha , \beta ) =\langle \alpha , \beta^{\vee}\rangle$。我们将证明 R 是分裂的半单李代数的根系，直到同构为止都是唯一的。总的来说，我们将考虑提案 1 中由关系定义的李代数。

数中的构造适用于$k$上的任何平方矩阵$(n(\alpha , \beta ))_{\alpha ,\beta\in B}$且行列式非零，并且$n(\alpha , \alpha ) = 2$适用于所有$\alpha \in B$（cf.第VI, §1, no. 10，公式） (14))。

令 E 为集合 B 在 $k$ 上的自由结合律代数。回想一下，E 是 $\mathbf{N}$ 分次的（代数，第 III, §3, no. 1，例 3）。我们将分别关联到向量空间 E、次数 $1,0,-1$ 的每个 $\alpha \in B$ 自同态 $X_{-\alpha}^0, H_{\alpha}^0, X_{\alpha}^0$。对于 B 的元素中的任意字 $(\alpha_1, . . . , \alpha_n)$，将

$$
X_{-\alpha}^0(\alpha_1, . . . , \alpha_n) = (\alpha , \alpha_1, . . . , \alpha_n) \tag{7}
$$

$$
H_{\alpha}^0(\alpha_1, . . . , \alpha_n) =(-\sum_{i=1}^nn(\alpha_i, \alpha ))(\alpha_1, . . . , \alpha_n) \tag{8}
$$

另一方面，$X_{\alpha}^0(\alpha_1, . . . , \alpha_n)$由归纳在$n$上使用公式定义

$$
X_{\alpha}^0(\alpha_1, . . . , \alpha_n) = (X_{-\alpha_1}^0X_{\alpha}^0-\delta_{\alpha ,\alpha_1}H_{\alpha}^0)(\alpha_2, . . . , \alpha_n) \tag{9}
$$

其中 $\delta_{\alpha ,\alpha_1}$ 是克罗内克符号；可以理解，如果$(\alpha_1, . . . , \alpha_n)$是空的字，则$X_{\alpha}^0(\alpha_1, . . . , \alpha_n)$就是零。

#### 引理 1 {#lie-viii-s4-lem-1 .statement tag=010V}

对于所有$\alpha , \beta \in B$，我们有

$$
[X_{\alpha}^0, X_{-\alpha}^0] =-H_{\alpha}^0 \tag{10}
$$

$$
[H_{\alpha}^0, H_{\beta}^0] = 0 \tag{11}
$$

$$
[H_{\alpha}^0, X_{\beta}^0] =n(\beta , \alpha )X_{\beta}^0 \tag{12}
$$

$$
[H_{\alpha}^0, X_{-\beta}^0] =-n(\beta , \alpha )X_{-\beta}^0 \tag{13}
$$

$[X_{\alpha}^0, X_{-\beta}^0] = 0$如果$\alpha \not=\beta$。 (14)

事实上，关系 (9) 可以写成

$$
(X_{\alpha}^0X_{-\alpha_1}^0)(\alpha_2, . . . , \alpha_n) = (X_{-\alpha_1}^0X_{\alpha}^0)(\alpha_2, . . . , \alpha_n)-\delta_{\alpha ,\alpha_1}H_{\alpha}^0(\alpha_2, . . . , \alpha_n)
$$

从而证明(10)和(14)。 关系(11) 清楚了。下一个

$$
[H_{\alpha}^0, X_{-\beta}^0](\alpha_1, . . . , \alpha_n) =H_{\alpha}^0(\beta , \alpha_1, . . . , \alpha_n)+(\sum_{i=1}^nn(\alpha_i, \alpha ))(\beta , \alpha_1, . . . , \alpha_n)
$$

$$
=-n(\beta , \alpha )(\beta , \alpha_1, . . . , \alpha_n)
$$

$$
=-n(\beta , \alpha )X_{-\beta}^0(\alpha_1, . . . , \alpha_n)
$$

因此（13）。最后，

$0 = [H_{\alpha}^0,[X_{\beta}^0, X_{-\gamma}^0]]$ $(10),(11),(14)$ (15)

$$
= [[H_{\alpha}^0, X_{\beta}^0], X_{-\gamma}^0] + [X_{\beta}^0,[H_{\alpha}^0, X_{-\gamma}^0]]
$$

$= [[H_{\alpha}^0, X_{\beta}^0]-n(\gamma , \alpha )X_{\beta}^0, X_{-\gamma}^0]$ (13)

$= [[H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0, X_{-\gamma}^0]$ 由 (14);

现在，考虑空的字立即给出

$$
([H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0)(\emptyset ) = 0
$$

所以 (15) 意味着

$$
([H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0)X_{-\gamma_1}^0X_{-\gamma_2}^0. . . X_{-\gamma_n}^0(\emptyset ) = 0
$$

对于所有$\gamma_1, . . . , \gamma_n\in B$；这就证明了(12)。

#### 引理 2 {#lie-viii-s4-lem-2 .statement tag=010W}

自同态 $X_{\alpha}^0,H_{\beta}^0,X_{-\gamma}^0$，其中$\alpha , \beta , \gamma \in B$，是线性无关的。

从 $X_{-\alpha}^0(\emptyset ) =\alpha$ 开始，很明显 $X_{-\alpha}^0$ 是线性无关的。

假设$\sum_{\alpha}a_{\alpha}H_{\alpha}^0= 0$；那么，对于所有$\beta \in B$，

$$
0 =[\sum_{\alpha}a_{\alpha}H_{\alpha}^0, X_{-\beta}^0]=-\sum_{\alpha}a_{\alpha}n(\beta , \alpha )X_{-\beta}^0
$$

由于 det($n(\beta , \alpha )$)$\not= 0$，因此对于所有 $\alpha$，$a_{\alpha}$ = 0。假设$\sum_{\alpha}a_{\alpha}X_{\alpha}^0= 0$。鉴于公式 (7), (8), (9),

$$
X_{\alpha}^0(\beta ) = 0
$$

$$
X_{\alpha}^0(\beta , \beta ) = 2\delta_{\alpha \beta}\beta
$$

对于所有$\beta \in B$。由此可见，对于所有$\beta$，$a_{\beta}= 0$。由于 $X_{\alpha}^0, H_{\alpha}^0, X_{-\alpha}^0$ 分别是次数 $-1,0,1$，因此引理是从之前中得出的。

设I为集合$B\times  \{-1,0,1\}$。输入$x_{\alpha}= (\alpha ,-1),h_{\alpha}= (\alpha ,0)$和$x_{-\alpha}= (\alpha ,1)$。令$\mathfrak{a}$为由生成的族I和以下关系器集合$\mathscr{R}$定义的李代数：

$$
[h_{\alpha}, h_{\beta}]
$$

$$
[h_{\alpha}, x_{\beta}]-n(\beta , \alpha )x_{\beta}
$$

$$
[h_{\alpha}, x_{-\beta}] +n(\beta , \alpha )x_{-\beta}
$$

$$
[x_{\alpha}, x_{-\alpha}] +h_{\alpha}
$$

$[x_{\alpha}, x_{-\beta}]$ 如果$\alpha \not=\beta$

（cf.章节II, §2, no. 3）。到引理 1 时，E 上存在唯一的线性表示 $\rho$ $\mathfrak{a}$，使得

$$
\rho (x_{\alpha}) =X_{\alpha}^0, \rho (h_{\alpha}) =H_{\alpha}^0, \rho (x_{-\alpha}) =X_{-\alpha}^0
$$

鉴于引理2，证明以下结果：

#### 引理 3 {#lie-viii-s4-lem-3 .statement tag=010X}

元素 $x_{\alpha}, h_{\beta}, x_{-\gamma}$ 中的 $\mathfrak{a}$ 中的典范像，其中 $\alpha , \beta , \gamma \in B$ 是线性无关的。

接下来，我们将认同$x_{\alpha}, h_{\alpha}, x_{-\alpha}$及其典范像放在$\mathfrak{a}$中。

#### 引理 4 {#lie-viii-s4-lem-4 .statement tag=010Y}

存在 $\mathfrak{a}$ 的唯一对合自同构 $\theta$，使得

$$
\theta (x_{\alpha}) =x_{-\alpha}, \theta (x_{-\alpha}) =x_{\alpha}, \theta (h_{\alpha}) =-h_{\alpha}
$$

对于所有$\alpha \in B$。

事实上，存在自由的李代数L(I)满足这些条件的内卷自同构。它使$\mathscr{R}\cup (-\mathscr{R})$保持稳定，因此定义通过到商的内卷自同构为$\mathfrak{a}$满足条件为引理。 唯一性源自$\mathfrak{a}$是由元素$x_{\alpha}, h_{\alpha}, x_{-\alpha}(\alpha \in B)$生成的。

这个自同构称为$\mathfrak{a}$的规范对合自同构。

令 Q 为 R 的根基权的集合；这是一个免费的 $\mathbf{Z}$ 模块，带有基 B（第 VI, §1, no. 9 章）。在自由李代数 L(I) 上存在型 Q 的分级，使得 $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ 分别为次数 $\alpha ,0,-\alpha$（第 II, §2, no. 6 章）。现在 $\mathscr{R}$ 中的元素是齐次的。因此，$\mathfrak{a}$上存在唯一的型 Q 与$\mathfrak{a}$的李代数结构兼容，并且$x_{\alpha}, h_{\alpha}, x_{-\alpha}$分别为次数$\alpha ,0,-\alpha$。对于任何$\mu\in Q$，用次数$\mu$的齐次$\mathfrak{a}$的元素的$\mathfrak{a}^\mu$集合表示。

#### 引理 5 {#lie-viii-s4-lem-5 .statement tag=010Z}

让$z\in \mathfrak{a}$。那么$z\in \mathfrak{a}^\mu$当且仅当$[h_{\alpha}, z] =\langle \mu, \alpha^{\vee}\rangle z$对于所有$\alpha \in B$。

对于$\mu\in Q$，令$\mathfrak{a}^{(\mu)}$为集合除以$x\in \mathfrak{a}$，这样$[h_{\alpha}, x] =\langle \mu, \alpha^{\vee}\rangle x$对于所有$\alpha \in B$。 $\mathfrak{a}^{(\mu)}$的和是直达。因此，要证明引理，只需证明$\mathfrak{a}^\mu\subset \mathfrak{a}^{(\mu)}$即可。让$\alpha \in B$。 向量空间 $\mathfrak{a}$的自同态$u$，使得$u|\mathfrak{a}^\mu=\langle \mu, \alpha^{\vee}\rangle .1$是$\mathfrak{a}$的推导，使得$ux=$（广告$h_{\alpha}$）$.x$对于$x=x_{\beta}, x=h_{\beta}, x=x_{-\beta}$；因此$u=$广告$h_{\alpha}$，这证明了我们的断言。

#### 注 {#lie-viii-s4-n2-rem-1 .statement tag=0110}

从引理 5 可以得出，$\mathfrak{a}$ 的每个理想都是齐次的，因为它在 ad $h_{\alpha}$ 下是稳定的。

用 B 的元素线性组合 $Q_+$ (或 $Q_-$) 集合表示正数 (或负数) 整数系数，并非全部零。把$\mathfrak{a}_+=$$\sum_{\mu\in Q_+}a^\mu$和$\mathfrak{a}_-=\sum_{\mu\in Q_-}\mathfrak{a}^\mu$。从$Q_++ Q_+\subset Q_+$和$Q_-+ Q_-\subset Q_-,\mathfrak{a}_+$开始

和$\mathfrak{a}_-$是$\mathfrak{a}$的谎言子代数。

#### 命题 2 {#lie-viii-s4-prop-2 .statement tag=0111}

(i) 李代数 $\mathfrak{a}_+$ 是由$(x_{\alpha})_{\alpha\in B}$ 家族产生的。

(ii) 李代数 $\mathfrak{a}_-$ 由家庭$(x_{-\alpha})_{\alpha\in B}$ 产生。

(iii) 家庭$(h_{\alpha})_{\alpha\in B}$ 是基向量空间 $\mathfrak{a}^0$。

(iv) 向量空间$\mathfrak{a}$是$\mathfrak{a}_+,\mathfrak{a}^0,\mathfrak{a}_-$中的直和。

令$\mathfrak{r}$（或$\mathfrak{n}$）为$(x_{\alpha})_{\alpha\in B}$（或$(x_{-\alpha})_{\alpha\in B}$）生成的$\mathfrak{a}$的谎言子代数，以及$(h_{\alpha})_{\alpha\in B}$生成的$\mathfrak{a}$的$\mathfrak{h}$、向量、子空间。由于$x_{\alpha}$是同质的，$\mathfrak{a}_+,\mathfrak{r}$的元素是$\mathfrak{a}_+$的分级子代数；因此，$[\mathfrak{h},\mathfrak{r}]\subset \mathfrak{r}$，所以$\mathfrak{h}+\mathfrak{r}$是$\mathfrak{a}$的子代数；自从

$$
[x_{-\alpha}, x_{\beta}] =\delta_{\alpha \beta}h_{\alpha}
$$

$[x_{-\alpha},\mathfrak{r}]\subset \mathfrak{h}+\mathfrak{r}$ 对于所有$\alpha \in B$。同样，$\mathfrak{n}$ 是$\mathfrak{a}_-$ 的分级子代数，$[\mathfrak{h},\mathfrak{n}]\subset \mathfrak{n},\mathfrak{h}+\mathfrak{n}$ 是$\mathfrak{n}$ 的子代数，$[x_{\alpha},\mathfrak{n}]\subset \mathfrak{h}+\mathfrak{n}$ 是所有$\alpha \in B$。输入$\mathfrak{a}'=\mathfrak{r}+\mathfrak{h}+\mathfrak{n}$。上式表明，对于所有 $\alpha \in B$，$\mathfrak{a}'$ 在 ad $x_{\alpha}$、ad $h_{\alpha}$ 和 ad $x_{-\alpha}$ 下都是稳定的，因此是 $\mathfrak{a}$ 的理想值。从 $\mathfrak{a}'$ 包含 $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ 开始，对于所有 $\alpha \in B,\mathfrak{a}'=\mathfrak{a}$。由此可见，包含$\mathfrak{r}\subset \mathfrak{a}_+,\mathfrak{h}\subset \mathfrak{a}^0$、$\mathfrak{n}\subset \mathfrak{a}_-$是等式，从而证明了命题。

#### 命题 3 {#lie-viii-s4-prop-3 .statement tag=0112}

李代数$\mathfrak{a}_+$（分别$\mathfrak{a}_-$）是免费的李代数，带有基本家庭$(x_{\alpha})_{\alpha\in B}$（分别$(x_{-\alpha})_{\alpha\in B}$）（cf.章节II, §2, no. 3）。

令 L 为 B 生成的 E 的谎言子代数。 II, §3，周四。 1、L可以与B生成的自由李代数等同。E对自身的左正则表示显然是单射的，而定义由限制到L是李代数的单射表示$\rho '$ E 上的L。设$\varphi$ 为从L 到$\mathfrak{a}_-$ 的唯一同态，对于所有$\alpha \in B$，需要从$\alpha$ 到$x_{-\alpha}$。那么，对于所有 $\alpha \in B,\rho (\varphi (\alpha ))$ 来说，在 E 上，乘法乘以$\alpha$ 等于自同态，所以$\rho \circ \varphi =\rho '$，这证明$\varphi$ 是单射的。因此，$(x_{-\alpha})_{\alpha\in B}$是$\mathfrak{a}_-$的基本族。因为$\theta (x_{-\alpha}) =x_{\alpha}$对于所有$\alpha$（cf.引理$4$）$, (x_{\alpha})_{\alpha\in B}$是$\mathfrak{a}_+$的基本家庭。

### 3. 存在定理

我们保留前面数的假设和记号。回想一下，如果 $\alpha , \beta \in B$ 且 $\alpha \not=\beta$，则 $n(\beta , \alpha )\leq 0$；此外，如果$n(\beta , \alpha ) = 0$，则$n(\alpha , \beta ) = 0$（第VI, §1, no. 1，公式（8）章）。对于 B 的任意对 $(\alpha , \beta )$ 不同的元素，将

$x_{\alpha \beta}=$（广告$x_{\alpha}$）$^{1-n(\beta ,\alpha)}x_{\beta}y_{\alpha \beta}=$（广告$x_{-\alpha}$）$^{1-n(\beta ,\alpha)}x_{-\beta}$。

然后$x_{\alpha \beta}\in \mathfrak{a}_+, y_{\alpha \beta}\in \mathfrak{a}_-$。如果$\theta$表示$\mathfrak{a}$、$\theta (x_{\alpha \beta}) =y_{\alpha \beta}$的规范自同构。

#### 引理 6 {#lie-viii-s4-lem-6 .statement tag=0113}

让 $\alpha , \beta \in B$ 与 $\alpha \not=\beta$。然后

$$
[\mathfrak{a}_+, y_{\alpha \beta}] = 0[\mathfrak{a}_-, x_{\alpha \beta}] = 0
$$

第二个公式是从第一个自同构$\theta$开始的。为了证明第一点，只要证明 $[x_{\gamma}, y_{\alpha \beta}] = 0$ 对于所有 $\gamma \in B$ 就足够了。我们区分三种情况。

情况1$:\gamma \not=\alpha$和$\gamma \not=\beta$。在这种情况下，$x_{\gamma}$与$x_{-\alpha}$和$x_{-\beta}$交换，因此与$y_{\alpha \beta}$交换。

案例2$:\gamma =\beta$。在这种情况下，$x_{\gamma}$与$x_{-\alpha}$通勤，所以

$[x_{\gamma}, y_{\alpha \beta}] =$（广告$x_{-\alpha}$）$^{1-n(\beta ,\alpha)}[x_{\gamma}, x_{-\beta}]$

$=-$（广告$x_{-\alpha}$）$^{1-n(\beta ,\alpha)}h_{\beta}=-n(\alpha , \beta$）（广告$x_{-\alpha}$）$^{-n(\beta ,\alpha)}x_{-\alpha}$。

如果 $n(\beta , \alpha )<0$，则此表达式为零，因为 (ad $x_{-\alpha}$)$.x_{-\alpha}= 0$。如果$n(\beta , \alpha ) = 0$，则$n(\alpha , \beta ) = 0$。在这两种情况下，$[x_{\gamma}, y_{\alpha \beta}] = 0$。

案例3$:\gamma =\alpha$。 $\mathfrak{a}$自同态代数、$[$-广告$h_{\alpha}$、广告$x_{-\alpha}] = 2$广告$x_{-\alpha}$

和[广告$x_{\alpha}$，广告$x_{-\alpha}] =$-广告$h_{\alpha}$；因而，通过 §1，引理 1，

[广告$x_{\alpha}$，（广告$x_{-\alpha}$）$^{1-n(\beta ,\alpha)}] = (1-n(\beta , \alpha$））（广告$x_{-\alpha}$）$^{-n(\beta ,\alpha)}($-广告$h_{\alpha}-n(\beta , \alpha ))$。

最后，

$[x_{\gamma}, y_{\alpha \beta}] =$ [广告$x_{\alpha}$，（广告$x_{-\alpha}$）$^{1-n(\beta ,\alpha)}]x_{-\beta}+$（广告$x_{-\alpha}$）$^{1-n(\beta ,\alpha)}$（广告$x_{\alpha}$）$x_{-\beta}$

$=-(1-n(\beta , \alpha$))(广告$x_{-\alpha}$)$^{-n(\beta ,\alpha)}$(广告$h_{\alpha}+n(\beta , \alpha )$)$x_{-\beta}$

+（广告$x_{-\alpha}$）$^{1-n(\beta ,\alpha)}$（广告$x_{\alpha}$）$x_{-\beta}$。

现在$[h_{\alpha}, x_{-\beta}] +n(\beta , \alpha )x_{-\beta}= 0$和$[x_{\alpha}, x_{-\beta}] = 0$，所以$[x_{\gamma}, y_{\alpha \beta}] = 0$。

#### 引理 7 {#lie-viii-s4-lem-7 .statement tag=0114}

由$x_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$生成的$\mathfrak{a}_+$的理想$\mathfrak{n}$是$\mathfrak{a}$的理想。由$y_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$生成的$\mathfrak{a}_-$的理想是$\mathfrak{a}$的理想，并且等于$\theta (\mathfrak{n})$。

让$\mathfrak{n}'=\sum_{\alpha ,\beta\in B,\alpha\not=\beta}kx_{\alpha \beta}$。由于每个 $x_{\alpha \beta}$ 在 $\mathfrak{a}, [\mathfrak{a}^0,\mathfrak{n}']\subset \mathfrak{n}'$ 中都是齐次的

（引理 5 和提案 2）。设 U（分别为 V）为 $\mathfrak{a}$（分别为 $\mathfrak{a}_+$）的包络代数，以及由 $\mathfrak{a}$ 的伴随物表示定义的 $\mathfrak{a}$ 上 U 的 $\sigma$ 表示。由$\mathfrak{n}'$生成的$\mathfrak{a}$的理想值是$\sigma (U)\mathfrak{n}'$。现在$\mathfrak{a}=\mathfrak{a}_++\mathfrak{a}^0+\mathfrak{a}_-$（提案$2$）$,\sigma (\mathfrak{a}_-)\mathfrak{n}'= 0$（引理6），以及前面的$\sigma (\mathfrak{a}^0)\mathfrak{n}'\subset \mathfrak{n}'$。通过Poincaré-Birkhoff-Witt 定理，$\sigma (U)\mathfrak{n}'=\sigma (V)\mathfrak{n}'$，证明了引理的第一个断言。由此可见，由$\theta (x_{\alpha \beta}) =y_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$生成的$\theta (\mathfrak{a}_+) =\mathfrak{a}_-$的理想是$\mathfrak{a}$的理想$\theta (\mathfrak{n})$。 Q.E.D.

$\mathfrak{a}$ 的理想$\mathfrak{n}+\theta (\mathfrak{n})$ 是分级的，因为它是由齐次元素生成的。因而，李代数$\mathfrak{a}/(\mathfrak{n}+\theta (\mathfrak{n}))$是Q级李代数；在本段的其余部分中，它由$\mathfrak{g}_B$表示，或简称为$\mathfrak{g}$。根据命题 2，如果 $\mathfrak{g}^\mu\not= 0$，则$\mu\in Q_+$、或 $\mu\in Q_-$、或 $\mu= 0$。用$\mathfrak{g}$中$x_{\alpha}$（或$h_{\alpha}, x_{-\alpha}$）的$X_{\alpha}$（或$H_{\alpha}, X_{-\alpha}$）典范像表示。鉴于$\mathfrak{a},\mathfrak{n}$和$\theta (\mathfrak{n})$的定义，可以得出$\mathfrak{g}$是由生成的族$((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$和关系定义的李代数

$$
[H_{\alpha}, H_{\beta}] = 0 \tag{16}
$$

$$
[H_{\alpha}, X_{\beta}]-n(\beta , \alpha )X_{\beta}= 0 \tag{17}
$$

$$
[H_{\alpha}, X_{-\beta}] +n(\beta , \alpha )X_{-\beta}= 0 \tag{18}
$$

$$
[X_{\alpha}, X_{-\alpha}] +H_{\alpha}= 0 \tag{19}
$$

$$
[X_{\alpha}, X_{-\beta}] = 0(\alpha \not=\beta ) \tag{20}
$$

（广告$X_{\alpha}$）$^{1-n(\beta ,\alpha)}X_{\beta}= 0(\alpha \not=\beta )$ (21)

（广告$X_{-\alpha}$）$^{1-n(\beta ,\alpha)}X_{-\beta}= 0(\alpha \not=\beta )$。 (22)

设$z\in \mathfrak{g}$和$\mu\in Q$。那么$z\in \mathfrak{g}^\mu$当且仅当$[H_{\alpha}, z] =\langle \mu, \alpha^{\vee}\rangle z$对于所有$\alpha \in B$。这是从引理 5 得出的。

从$\mathfrak{a}^0\cap (\mathfrak{n}+\theta (\mathfrak{n})) = 0$开始，从$\mathfrak{a}^0$到$\mathfrak{g}^0$的规范映射是同构。因而，$(H_{\alpha})_{\alpha\in B}$ 是向量空间 $\mathfrak{g}^0$ 中的基。 $\mathfrak{g}_B$中的交换子代数$\mathfrak{g}^0$将由$\mathfrak{h}_B$或简称为$\mathfrak{h}$表示。从V到$\mathfrak{h}^*$存在唯一的同构$\mu \rightarrow \mu_B$，使得$\langle \mu_B, H_{\alpha}\rangle =\langle \mu, \alpha^{\vee}\rangle$适用于所有$\mu\in V$和所有$\alpha \in B$。

$\mathfrak{a}$ 定义的对合律自同构 $\theta$ 通过传递到商 $\mathfrak{g}$ 的对合律自同构也将由 $\theta$ 表示。我们有 $\alpha \in B\cup (-B)$ 和 $\theta (H_{\alpha}) =-H_{\alpha}$ 的 $\theta (X_{\alpha}) =X_{-\alpha}$。

#### 定理 1 {#lie-viii-s4-thm-1 .statement tag=0115}

令R为R的约化根系，B基。令$\mathfrak{g}$为由生成的族$((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$和关系(16)至(22)定义的李代数。让$\mathfrak{h}=\sum_{\alpha\in B}kH_{\alpha}$。那么$(\mathfrak{g},\mathfrak{h})$就是分裂的半单李代数。 同构$\mu \rightarrow \mu_B$从V到$\mathfrak{h}^*$映射R到$(\mathfrak{g},\mathfrak{h})$的根系。对于所有 $\mu\in R,\mathfrak{g}^\mu$ 是相对于根 $\mu$ 的特征空间。

证明遵循引理 8、9、10、11。

#### 引理 8 {#lie-viii-s4-lem-8 .statement tag=0116}

让$\alpha \in B\cup (-B)$。那么 ad $X_{\alpha}$ 是局部幂零的。$^1$

假设$\alpha \in B$。令 $\mathfrak{g}'$ 为 $z\in \mathfrak{g}$ 的集合，使得 (ad $X_{\alpha}$)$^pz= 0$ 为足够大 $p$。由于广告$X_{\alpha}$是$\mathfrak{g},\mathfrak{g}'$的推导，是$\mathfrak{g}$的子代数。到 (21)，$X_{\beta}\in \mathfrak{g}'$ 对于所有 $\beta \in B$。对于所有 $\beta \in B$，按 (17)、(19)、(20)、$H_{\beta}\in \mathfrak{g}'$ 和 $X_{-\beta}\in \mathfrak{g}'$。因此 $\mathfrak{g}'=\mathfrak{g}$ 和 ad $X_{\alpha}$ 是局部幂零的。由于 ad $X_{-\alpha}=\theta$(ad $X_{\alpha}$)$\theta^{-1}$，我们看到 ad $X_{-\alpha}$ 是局部幂零的。

我们将看到 $\mathfrak{g}$ 是有限维的，因此 ad $X_{\alpha}$ 实际上是幂零的。

#### 引理 9 {#lie-viii-s4-lem-9 .statement tag=0117}

令$\mu, \nu \in Q$和$w\in W(R)$使得$w\mu=\nu$。存在 $\mathfrak{g}$ 中的自同构，需要 $\mathfrak{g}^\mu$ 到 $\mathfrak{g}^{\nu}$。

对于所有$\alpha \in B$，令$s_{\alpha}$为由$\alpha$定义的V的反射。由于W(R)是由$s_{\alpha}$（第VI, §1, no. 5，注1）生成的，所以当$w=s_{\alpha}$时证明引理就足够了。鉴于引理8，我们可以定义

$$
\theta_{\alpha}=e^{adX_{\alpha}}e^{adX_{-\alpha}}e^{adX_{\alpha}}
$$

已验证如章节所示。 I, §6, no. 8，$\theta_{\alpha}$ 是 $\mathfrak{g}$ 的自同构。我们有

向量空间 V 的 $^1$ 自同态 $u$ 被称为局部幂零（或几乎

幂零）如果对于每个$v\in V$，存在正整数$n$使得$u^n(v) = 0$

（cf.交换代数，第IV, §1, no. 4章，定义2）。那么 exp($u$) 或 $e^u$ 就是

由公式 $e^u(v) =\sum_{n\geq 0}(1/n$!)$u^n(v)$ 定义为所有 $v\in V$。 $\theta_{\alpha}(H_{\alpha}) =e^{adX_{\alpha}}e^{adX_{-\alpha}}(H_{\beta}-n(\alpha , \beta )X_{\alpha})$

$$
=e^{adX_{\alpha}}(H_{\beta}-n(\alpha , \beta )X_{\alpha}+n(\alpha , \beta )X_{-\alpha}-n(\alpha , \beta )H_{\alpha}-\frac{n(\alpha , \beta)}{2}2X_{-\alpha})
$$

$$
=e^{adX_{\alpha}}(H_{\beta}-n(\alpha , \beta )H_{\alpha}-n(\alpha , \beta )X_{\alpha})
$$

$$
=H_{\beta}-n(\alpha , \beta )H_{\alpha}-n(\alpha , \beta )X_{\alpha}-n(\alpha , \beta )X_{\alpha}-n(\alpha , \beta )(-2X_{\alpha})
$$

$$
=H_{\beta}-n(\alpha , \beta )H_{\alpha}
$$

如果$z\in \mathfrak{g}^\mu$，

$$
[H_{\beta}, \theta_{\alpha}^{-1}z] =\theta_{\alpha}^{-1}[H_{\beta}-n(\alpha , \beta )H_{\alpha}, z]
$$

$$
=\theta_{\alpha}^{-1}(\langle \mu, \beta^{\vee}\rangle z-n(\alpha , \beta )\langle \mu, \alpha^{\vee}\rangle z)
$$

$$
=\langle \mu- \langle \alpha^{\vee}, \mu\rangle \alpha , \beta^{\vee}\rangle \theta^{-1}_{\alpha}z=\langle s_{\alpha}\mu, \beta^{\vee}\rangle \theta^{-1}_{\alpha}z
$$

所以$\theta_{\alpha}^{-1}z\in \mathfrak{g}^{s_{\alpha}\mu}$。这表明$\theta^{-1}_{\alpha}\mathfrak{g}^\mu\subset \mathfrak{g}^{s_{\alpha}\mu}$。由于$\theta_{\alpha}$是自同构，并且由于这个包含对于所有$\mu\in Q$都成立，所以我们看到$\theta_{\alpha}^{-1}\mathfrak{g}^\mu=\mathfrak{g}^{s_{\alpha}\mu}$，这证明了引理。

#### 引理 10 {#lie-viii-s4-lem-10 .statement tag=0118}

设$\mu\in Q$，并假设$\mu$不是根的倍数。存在$w\in W(R)$，使得$w\mu$相对于基 B 的某些坐标为$>0$，其中某些为$<0$。

令$V_{\mathbf{R}}$为向量空间$Q\otimes_{\mathbf{Z}}\mathbf{R}$，其中R为根系。到假设，存在$f\in V^*_{\mathbf{R}}$，使得$\langle f, \alpha \rangle  \not= 0$对于所有$\alpha \in R$和$\langle f, \mu\rangle = 0$。存在 $R^{\vee}$ 的室C，使得 $f\in C$。由章。 VI, §1, no. 5，周四。如图2(i)所示，存在$w\in W(R)$使得$wf$属于到与B相关的室，在其他字中使得$\langle wf, \alpha \rangle >0$对于所有$\alpha \in B$。写$w\mu=\sum_{\alpha\in B}t_{\alpha}\alpha$。然后

$$
0 =\langle f, \mu\rangle =\langle wf, w\mu\rangle =\sum_{\alpha\in B}t_{\alpha}\langle wf, \alpha \rangle
$$

这证明某些$t_{\alpha}$是$>0$，而其他$<0$。

#### 引理 11 {#lie-viii-s4-lem-11 .statement tag=0119}

让$\mu\in Q$。如果$\mu \notin R\cup \{0\}$，则$\mathfrak{g}^\mu= 0$。如果$\mu\in R$，则变暗$\mathfrak{g}^\mu= 1$。

1) 如果$\mu$不是R的元素的倍数，则存在$w\in W$使得$w\mu \notin Q_+\cup Q_-$(引理10)，因此$\mathfrak{a}^{w\mu}= 0,\mathfrak{g}^{w\mu}= 0$，因此$\mathfrak{g}^\mu= 0$(引理9)。

2) 设$\alpha \in B$且$m$为整数。由于 $\mathfrak{a}_+$ 是一个免费的李代数以及基本系列 $(x_{\alpha})_{\alpha\in B}$，因此我们为 $m >1$ 提供了暗淡的$\mathfrak{a}^{\alpha}= 1$ 和 $\mathfrak{a}^{m\alpha}= 0$（第 II, §2, no. 6 章，第 4 条）。因而$\mathfrak{g}^{\alpha}\leq 1$和$\mathfrak{g}^{m\alpha}= 0$对于$m >1$来说是暗淡的。我们不能有$\mathfrak{g}^{\alpha}= 0$，因为这意味着$x_{\alpha}\in \mathfrak{n}+\theta \mathfrak{n}$，因此意味着$\mathfrak{n}+\theta \mathfrak{n}$包含于$h_{\alpha}=-[x_{\alpha}, x_{-\alpha}]$，而$\mathfrak{a}^0\cap (\mathfrak{n}+\theta \mathfrak{n}) = 0$。因而，暗淡$\mathfrak{g}^{\alpha}= 1$。

3）如果$\mu\in R$，存在$w\in W(R)$使得$w(\mu)\in B$（第VI, §1, no. 5章，第15条命题），所以暗淡$\mathfrak{g}^\mu=$暗淡$\mathfrak{g}^{w\mu}= 1$。此外，如果$n$是整数$>1$，那么$\mathfrak{g}^{nw(\mu)}= 0$，所以$\mathfrak{g}^{n\mu}= 0$。

证明共定理 1。

由于dim$\mathfrak{g}^0=$卡B，从引理11得出$\mathfrak{g}$等于有限维等于卡B+卡R。我们证明$\mathfrak{g}$是半单。设$\mathfrak{k}$是$\mathfrak{g}$的交换理想。由于$\mathfrak{k}$在ad($\mathfrak{h}$)$,\mathfrak{k}= (\mathfrak{k}\cap \mathfrak{h}) +\sum_{\mu\in R}(\mathfrak{k}\cap \mathfrak{g}^\mu)$下是稳定的。

很明显，对于所有 $\alpha \in B,\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}+kH_{\alpha}$ 来说，它与 $\mathfrak{s}\mathfrak{l}(2, k)$ 同构。鉴于引理 9，对于所有$\mu\in R,\mathfrak{g}^\mu$都包含在与$\mathfrak{s}\mathfrak{l}(2, k)$同构的$\mathfrak{g}$的子代数中；因而，$\mathfrak{k}\cap \mathfrak{g}^\mu= 0$，所以$\mathfrak{k}\subset \mathfrak{h}$；因而

$$
[\mathfrak{k},\mathfrak{g}^\mu]\subset \mathfrak{k}\cap \mathfrak{g}^\mu= 0
$$

所以 $\mu_B(\mathfrak{k}) = 0$ 对于所有$\mu\in R$。由此得出$\mathfrak{k}= 0$，从而证明$\mathfrak{g}$是半单。

让$\mu\in R$。存在$\alpha \in B$使得$\langle \mu, \alpha^{\vee}\rangle  \not= 0$，并且(ad$H_{\alpha}$)$|\mathfrak{g}^\mu$是非零位似。因而，$\mathfrak{h}$等于$\mathfrak{g}$中其自身的归一化器，因此是$\mathfrak{g}$的嘉当子代数。对于所有 $u\in \mathfrak{h}$，ad $u$ 是可对角化的，因而 $(\mathfrak{g},\mathfrak{h})$ 是分裂的半单李代数。

对于所有$\mu\in R$，很明显$\mu_B$是$(\mathfrak{g},\mathfrak{h})$的根，$\mathfrak{g}^\mu$是相应的特征空间。 $(\mathfrak{g},\mathfrak{h})$根数暗淡$\mathfrak{g}-$暗淡$\mathfrak{h}=$卡R。因此，映射$\mu \rightarrow \mu_B$从V到$\mathfrak{h}^*$映射R到$(\mathfrak{g},\mathfrak{h})$的根系。

### 4. 唯一性定理

#### 命题 4 {#lie-viii-s4-prop-4 .statement tag=011A}

设$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$为带框的半单李代数。设$(n(\alpha , \beta ))_{\alpha ,\beta\in B}$和$(X_{\alpha})_{\alpha\in B\cup(-B)}$为相应的嘉当矩阵和生成的族。

(i) no. 3的族$((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$和关系(16)至(22)构成$\mathfrak{g}$的呈现。

(ii) no. 3的族$(X_{\alpha})_{\alpha\in B}$和关系(21)构成由$(X_{\alpha})_{\alpha\in B}$生成的$\mathfrak{g}$的子代数的表示。

令 R 为 $(\mathfrak{g},\mathfrak{h})$ 的根系。 应用至 R 和 B 构造。 2和3，我们得到对象，我们用$\mathfrak{a}',\mathfrak{g}', X'_{\alpha}, H'_{\alpha}, . .$表示。而不是$\mathfrak{a},\mathfrak{g}, X_{\alpha}, H_{\alpha}, . .$..

存在从李代数$\mathfrak{g}'$到李代数$\mathfrak{g}$的同态$\varphi$，使得$\varphi (X'_{\alpha}) =X_{\alpha},\varphi (H'_{\alpha}) =H_{\alpha},\varphi (X'_{-\alpha}) =X_{-\alpha}$对于所有$\alpha \in B$（命题1）。因为 dim $\mathfrak{g}'$ = Card R + Card B = dim$\mathfrak{g},\varphi$ 是双射的。这就证明了(i)。

$(X'_{\alpha})_{\alpha\in B}$生成的$\mathfrak{g}'=\mathfrak{a}'/(\mathfrak{n}'\oplus \theta '\mathfrak{n}') = (\mathfrak{a}'_+\oplus {\mathfrak{a}'}^0\oplus \mathfrak{a}'_-)/(\mathfrak{n}'\oplus \theta '\mathfrak{n}')$中的子代数可以用$\mathfrak{a}'_+/\mathfrak{n}'$来识别。根据命题3和$\mathfrak{n}'$的定义，证明(ii)。

#### 推论 {#lie-viii-s4-n4-cor-1 .statement tag=011B}

每个框架半单李代数都是通过$\mathbf{Q}$到$k$标量的扩张从框架半单$\mathbf{Q}$-李代数获得的。

这紧随命题而来。

#### 定理 2 {#lie-viii-s4-thm-2 .statement tag=011C}

设$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$和$(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$为半单李代数，设R和$R'$为$(\mathfrak{g},\mathfrak{h})$和$(\mathfrak{g}',\mathfrak{h}')$的根系，设$(n(\alpha , \beta ))_{\alpha ,\beta\in B}$（或$(n'(\alpha , \beta ))_{\alpha ,\beta\in B'}$）为R的嘉当矩阵 （分别$R'$）相对于B（分别$B'$），并令$\Delta$（分别$\Delta '$）为R（分别$R'$）相对于B（分别$B'$）的Dynkin图。

(i) 如果从$\mathfrak{h}^*$到$\mathfrak{h}^{'*}$$\varphi$是同构，使得$\varphi (R) = R'$和$\varphi (B) = B'$，则存在从$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$到$(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$唯一的同构$\psi$，使得$\psi |\mathfrak{h}=^t\varphi^{-1}$。

(ii) 如果从B到$B'$$f$是双射，使得$n'(f(\alpha ), f(\beta )) =n(\alpha , \beta )$对于所有$\alpha , \beta \in$B，存在从$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$到$(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$的同构。

(iii) 如果从$\Delta$到$\Delta '$存在同构，则从$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$到$(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$存在同构。

这紧随提案 4 (i)（利用第 VI, §4, no. 2 章，第 1 条提案部分 (iii)）。

#### 学院{#lie-viii-s4-n4-sch-1 .statement tag=011D}

任何可分割的半单李代数$\mathfrak{g}$都与一个Dynkin图相关联，其中确定$\mathfrak{g}$一直到同构（Th.2（iii））。当且仅当 $\mathfrak{g}$ 是简单的（§3, no. 2，命题 6 的 Cor. 1）时，该图才是非空且连通的。由 Th. no. 3 的第 1 章，以及第 1 章。 VI, §4, no. 2，周四。 3、可分割的简单李代数为型$A_l(l\geq 1), B_l(l\geq 2), C_l(l\geq 3), D_l(l\geq 4)$、$E_6, E_7, E_8, F_4, G_2$的代数。此列表中没有两个代数是同构的。

#### 命题 5 {#lie-viii-s4-prop-5 .statement tag=011E}

设$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$为框架半单李代数，$(X_{\alpha})_{\alpha\in B\cup(-B)}$相应的生成的家庭。存在唯一的 $\mathfrak{g}$ 自同构 $\theta$，使得 $\theta (X_{\alpha}) =X_{-\alpha}$ 对于所有$\alpha \in B\cup (-B)$。我们有 $\theta^2=$ Id$_{\mathfrak{g}}$，以及所有 $h\in \mathfrak{h}$ 的 $\theta (h) =-h$。

唯一性自 $(X_{\alpha})_{\alpha\in B\cup(-B)}$ 生成李代数 $\mathfrak{g}$ 开始清晰。根据命题 4，$\theta$ 的存在源自我们在 no. 3 之前 Th 中所说的。 1.

#### 推论 {#lie-viii-s4-n4-cor-2 .statement tag=011F}

设$(\mathfrak{g},\mathfrak{h})$为分裂的半单李代数。那么$(\mathfrak{g},\mathfrak{h})$拥有Chevalley系统（§2, no. 4，Def.3）。

令 R 为 $(\mathfrak{g},\mathfrak{h})$ 的根系。对于所有 $\alpha \in R$，令 $X_{\alpha}$ 为 $\mathfrak{g}^{\alpha}$ 的非零元素。假设选择了 $X_{\alpha}$，使得 $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ 对于所有 $\alpha \in R ($§2, no. 4、引理 2)。令 B 为 R 的基和 $\mathfrak{g}$ 的 $\theta$ 自同构，这样对于所有 $\alpha \in B\cup (-B)$ 来说，$\theta (X_{\alpha}) =X_{-\alpha}$。我们有$\theta |\mathfrak{h}=-$Id$_{\mathfrak{h}}$。因此，对于所有$\alpha \in R$，都存在$t_{\alpha}\in k^*$，使得$\theta X_{\alpha}=t_{\alpha}X_{-\alpha}$。我们有

$$
t_{\alpha}t_{-\alpha}H_{\alpha}= [t_{\alpha}X_{-\alpha}, t_{-\alpha}X_{\alpha}] = [\theta X_{\alpha}, \theta X_{-\alpha}] =\theta ([X_{\alpha}, X_{-\alpha}])
$$

$$
=\theta (-H_{\alpha}) =H_{\alpha}
$$

所以 $t_{\alpha}t_{-\alpha}= 1$ 对于所有$\alpha \in R$。像§2, no. 4一样引入$N_{\alpha \beta}$。如果$\alpha , \beta , \alpha +\beta \in R$，

$$
N_{-\alpha ,-\beta}t_{\alpha}t_{\beta}X_{-\alpha-\beta}=t_{\alpha}t_{\beta}[X_{-\alpha}, X_{-\beta}] = [\theta X_{\alpha}, \theta X_{\beta}] =\theta ([X_{\alpha}, X_{\beta}])
$$

$$
= N_{\alpha \beta}\theta X_{\alpha+\beta}= N_{\alpha \beta}t_{\alpha+\beta}X_{-\alpha-\beta}
$$

所以，鉴于§2, no. 4，引理 4，

$$
(q+ 1)^2t_{\alpha}t_{\beta}= N^2_{\alpha \beta}t_{\alpha+\beta}
$$

其中$q$是整数。由此可见，如果$t_{\alpha}$和$t_{\beta}$在$k^*$中是平方，则$t_{\alpha+\beta}$也是。从 $t_{\alpha}= 1$ 开始，对于所有 $\alpha \in B$，第 19 章的提案 19。 VI, §1, no. 6，证明对于所有$\alpha \in R$，$t_{\alpha}$ 都是平方。 选择，对于所有$\alpha \in R$，$u_{\alpha}\in k$使得$u^2_{\alpha}=t_{\alpha}$。这个选择可以被制作成 $u_{\alpha}u_{-\alpha}= 1$ 适合所有 $\alpha \in R$。把$X'_{\alpha}=u^{-1}_{\alpha}X_{\alpha}$。那么，对于所有$\alpha \in R$，

$$
X'_{\alpha}\in \mathfrak{g}^{\alpha},[X'_{\alpha}, X'_{-\alpha}] = [X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

和$\theta (X'_{\alpha}) =\theta (u^{-1}_{\alpha}X_{\alpha}) =u^{-1}_{\alpha}t_{\alpha}X_{-\alpha}=u_{\alpha}X_{-\alpha}=u_{\alpha}u_{-\alpha}X'_{-\alpha}=X'_{-\alpha}$，因此$(X'_{\alpha})_{\alpha\in R}$是$(\mathfrak{g},\mathfrak{h})$的Chevalley 系统。

### 习题 {#lie-viii-s4-exercises}

本段中考虑的李代数不一定是有限维的。

参见[习题为 § 4](exercises/s4/)。
