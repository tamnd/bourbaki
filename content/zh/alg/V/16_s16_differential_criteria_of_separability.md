---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 16
section_title: Differential criteria of separability
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.127-A V.137, A V.177-A V.180
pdf_pages: 0241-0251, 0291-0294
extraction: ocr
subsections:
    - "no": 1
      title: 'Extension of derivations : the case of rings'
      page: 127
      pdf_page: 241
    - "no": 2
      title: 'Extension of derivations: the case of fields'
      page: 0
      pdf_page: 242
    - "no": 3
      title: Derivations in fields of characteristic zero
      page: 130
      pdf_page: 244
    - "no": 4
      title: Derivations in separable extensions
      page: 131
      pdf_page: 245
    - "no": 5
      title: The index of a linear mapping
      page: 132
      pdf_page: 246
    - "no": 6
      title: Differential properties of finitely generated extensions
      page: 133
      pdf_page: 247
    - "no": 7
      title: Separating transcendence bases
      page: 136
      pdf_page: 250
statements: 32
exercises: 9
content_sha256: 65d0b0828a31a7d69baa06ca3ad221300dc3af975a29eae21bd233ddb7f83713
translated_from: content/en/alg/V/16_s16_differential_criteria_of_separability.md
translation_method: google
source_content_sha256: 74e20434a4632131b94714a4b2546c552d9b686ae8250258434122a026af180b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 422a0004b2311c631ab43605267e2606750bb400a4bac5fc5cad2270436a928e
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 16。可分离性的差异判据

### 1. 推导中的扩张：环的情况

设K为交换环，A交换K-代数和$x = (x_i)_{i \in I}$，A的元素族。进一步，令$A$为K入A-模M的推导，在其他字（III，p. 553）a对于 K 中的 $c, c'$，K 到 M 满足关系 $\Delta(cc') = c \cdot \Delta(c') + c' \cdot \Delta(c)$ 的 Z 线性映射。对于每个$i \in I$，令 $D_i$ 为多项式环 $K[X_i]_{i \in I}$ 中相对于 $X_i$ 的部分推导；这是环自身的唯一推导，它是 K 上的零和 $X_j$ 上的 $j \in I - \{i\}$，并且在 $X_i$ 上取值 1（IV，p. 6）。对于$K[X_i]_{i \in I}$中的每个多项式$f = \sum_{a \in N^{(I)}} c_a \cdot X^\alpha$，我们用M的$f^\Delta(x)$元素$\sum_{\alpha \in N^{(I)}} x^\alpha \cdot \Delta(c_\alpha)$表示。

#### 命题 1 {#alg-v-s16-prop-1 .statement tag=06UK}

— 假设族$x = (x_i)_{i \in I}$、生成K-代数 A。设$(m_i)_{i \in I}$是M的元素族和$(f_\lambda)_\lambda$，多项式族生成的所有多项式$f \in K[X_i]_{i \in I}$的理想$a$，使得$f(x) = 0$。对于 A 到 M 的推导 D 的存在，使得 $D(c \cdot 1) = \Delta(c)$ 对于所有 $c \in K$ 和 $D(x_i) = m_i$ 对于所有 $i \in I$ 是必要且充分的

$$
f_\lambda^\Delta(x) + \sum_{i \in I} D_i f_\lambda(x) \cdot m_i = 0 \quad \text{for all} \quad \lambda \in A .
$$

如果是这样，推导 D 是唯一的并且满足

$$
D(f(x)) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i \quad \text{for all} \quad f \in K[X_i]_{i \in I}
$$

将 $E = K[X_i]_{i \in I}$ 写入 $\varphi$，表示 E 的 K 同态到 A 上，其中对于所有 $i \in I$，映射 $X_i$ 到 $x_i$；因此，对于所有 $f \in E$，我们都有 $\varphi(f) = f(x)$。我们将 M 视为 E 模，通过同态 $\varphi : E \to A$ 和定义映射 $D'$ 将 E 通过 $D'(f) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i$ 转化为 M（注，$(D_i f)_{i \in I}$ 系列中的每个 $f \in E$ 都有有限支撑）。很明显，$D'$是E到M中唯一的推导延伸A，并且对于每个$i \in I$，映射$X_i$到$m_i$。

令 D 为 A 到 M 的推导，使得对于所有 $c \in K$ 为 $D(c \cdot 1) = \Delta(c)$，对于所有 $i \in I$ 为 $D(x_i) = m_i$。那么$D \circ \varphi$是E到M的推导延伸A并且对于所有$i \in I$来说映射$X_i$延伸到$m_i$。因此我们有 $D \circ \varphi = D'$，即关系 (2) 成立。这证明了 D 的唯一性 ；而且(1)是$f, (x) = 0$和(2)中的推论。

反之假设 (1) 成立；在其他字中，我们对所有$\lambda \in A$都有$D'(f_\lambda) = 0$。设 $f \in a$； $E$中存在有限支撑$(q_\lambda)_{\lambda \in \Lambda}$的族，使得$f = \sum_{\lambda \in \Lambda} q_\lambda \cdot f_\lambda$。我们有
$$
D'(f) = \sum_{\lambda \in \Lambda} [f_\lambda(x) \cdot D'(q_\lambda) + q_\lambda(x) \cdot D'(f_\lambda)]
$$
从而 $D'(f) = 0$ 因为$f_\lambda(x)$和$D'(f_\lambda)$对于所有$\lambda \in A$来说都是零。由于$D'$在$a$上消失，因此存在$A$到$M$的$Z$线性映射$D$，使得$D' = D \circ \varphi$；显然$D$是$A$到$M$所需的推导。

### 2. 推导的扩张：域的情况

令$K, L$和$M$为域，使得$K \subset L \subset M$。根据第 21 条命题（III，p. 572），我们有正合序列的向量 $M$ 个空间
$$
(\mathrm{E}_{K,L,M}) \quad \Omega_K(L) \otimes_L M \xrightarrow{\alpha} \Omega_K(M) \xrightarrow{\beta} \Omega_L(M) \to 0 ;
$$
$M$-线性映射$\alpha$和$\beta$的特征为关系
$$
(3) \quad \alpha(d_{L/K} x \otimes 1) = d_{M/K} x \quad \text{for } x \in L \\
(4) \quad \beta(d_{M/K} y) = d_{M/L} y \quad \text{for } y \in M
$$

设$V$为向量$M$-空间，用$K$的$D_K(M, V)$向量空间表示$M$与$V$中值的导数，并类似地引入$D_K(L, V)$和$D_L(M, V)$。通过 III、p. 571、图表 (42) 和 III、p. 572、图表 (44)，我们有图表同态向量空间
$$
\begin{array}{ccccccccc}
0 \to \mathrm{Hom}_M(\Omega_L(M), V) & \xrightarrow{\mathrm{Hom}(\beta, 1)} & \mathrm{Hom}_M(\Omega_K(M), V) & \xrightarrow{\mathrm{Hom}(\alpha, 1)} & \mathrm{Hom}_M(\Omega_K(L) \otimes_L M, V) \\
\downarrow & & \downarrow & & \downarrow \\
0 \to \mathrm{Der}_L(M, V) & \xrightarrow{i_V} & \mathrm{Der}_K(M, V) & \xrightarrow{r_V} & \mathrm{Der}_K(L, V),
\end{array}
$$
其中垂直箭头为同构，$i_V$为典范嵌入，$r_V$限制映射。

因此我们从 II, p. 299, Th 得到。 5 和 II、p. 301、提案 10 以下命题：

#### 命题 2 {#alg-v-s16-prop-2 .statement tag=06UL}

— *以下条件是等效的*：
a) *映射 $\alpha$ 是单射*。
b) *每个$K$-将$L$推导为$M$扩展到$K$-将$M$推导为$M$*。
c) *每个$L$的$K$-推导到向量$M$-空间$V$扩展到$K$-$M$到$V$的推导*。

#### 命题 3 {#alg-v-s16-prop-3 .statement tag=06UM}

— *令$K$为域，$L$为$K$的纯扩张，$(x_i)_{i \in I}$为$L$的纯基*（V，p. 106，Def.2）。

a) 令$V$比$L$除向量空间，$K$的$A$推导变成$V$和$(v_i)_{i \in I}$，元素和$V$的族。 $L$到$V$存在唯一的推导$D$，延伸$A$，这样对于所有$i \in I$都有$D(x_i) = v_i$。

b) $K$-$L$的微分的向量$L$-空间$\Omega_K(L)$具有$(dx_i)_{i \in I}$族基。

断言 b) 已在IV、p. 23 和断言 a) 中得到证明，由此可直接得出。

#### 推论{#alg-v-s16-n2-cor-1 .statement tag=06UN}

— 设 $P$ 为 $K$ 的子域。 $\Omega_P(K) \otimes_K L$典范映射$\alpha$入$\Omega_P(L)$单射且族$(d_{L/P} x_i)_{i \in I}$，是$\Omega_P(L)$子空间基（超过$L$）对$\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$像的补充。

命题 3, a) 表明，在 $L$ 扩展上，每一次将 $K$ $P$ 推导为向量空间 $V$，再将 $L$ $P$ 推导为 $V$； $\alpha$ 的单射性则由命题 2 得出。推论的第二个断言由序列 $(\mathbf{E}_{P,K,L})$ 和命题 3, b) 的精确性得出（考虑到公式 (4)）。

#### 命题 4 {#alg-v-s16-prop-4 .statement tag=06UO}

— 设$K$为域，$L$是$K$和$V$向量空间在$L$上的可分离代数扩张。

a) 每个$L$到$V$的$K$导数都是零。

b) 如果$A$是$K$到$V$的推导，则存在$L$到$V$的唯一推导$D$，其中扩展$A$。

令$D$为$L$到$V$的$K$导数。如果$E$是有限次数的$L$在$K$上的子扩展，则$K$-代数$E$是etale，因此$\Omega_K(E) = 0$（$V$，p. 33，Th.3），从而 $D|_E = 0$乘泛性质共$\Omega_K(E)$（III，p. 569）。由于$L$是有限次数在$K$上的子扩展族的并，所以我们有$D = 0$，从而a)。

设$A$为$K$的推导入$V$。 如果$D'$和$D''$是$A$的两个扩张到$L$的推导到$V$，那么差$D' - D''$是$L$到$V$的$K$推导；因此 a) 等于零，所以 $D' = D''$。

还需要证明$A$的扩张的存在性。 Zorn 的引理 (E, III, p. 20) 意味着存在在 $L$ 包含的子域 $L_0$ 上定义的 $A$ 到推导的最大扩张 $D_0$ $K$。

令 $x$ 位于 $L$ 和 $g$ 中，$x$ 在 $L_0$ 上的最小多项式。由于 $L$ 是代数且在 $K$ 上可分，$x$ 是代数且在 $L_0$ 上可分（$V$、p. 39，第 6 条命题和 p. 39，Cor. 2）；因此$x$是$g$（$V$，p. 39，命题5），从而$g'(x) \neq 0$（IV，p. 17，命题7）的简单根。如果我们像$V$、p. 127一样定义$g^{D_0}(x)$，则存在$V$的元素$u$使得$g^{D_0}(x) + g'(x) \cdot u = 0$；根据命题1（V，p. 127），存在$L_0(x)$的推导$D$延伸到$V$延伸$D_0$，从而$D(x) = u$。鉴于 $(L_0, D_0)$ 的最大特征标，我们因此有 $L_0(x) = L_0$、从而 $x \in L_0$。由于$x$是任意的，我们结论即$L_0 = L$。

#### 推论 1 {#alg-v-s16-prop-4-cor-1 .statement tag=06UP}

— 如果 $L$ 是代数且可在 $K$ 上分离，则我们有 $\Omega_K(L) = 0$。

推论源自命题 4，a)，因为向量$L$-空间$\Omega_K(L)$是由规范$K$-推导$d_{L/K} : L \to \Omega_K(L)$的像生成的。

#### 推论 2 {#alg-v-s16-prop-4-cor-2 .statement tag=06UQ}

— *如果 L 是代数，并且域 K 的可分扩张，则对于 K 的每个子域 P，典范映射 $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ 是同构。*

映射 $\alpha$ 由命题 2 (V, p. 128) 和命题 4, *b*) 内射；由于 $\Omega_K(L)$ 约化到 0（Cor. 1），序列 $(E_{P.K.L})$ 的精确性意味着 $\alpha$ 是满射的。

#### 推论 3 {#alg-v-s16-prop-4-cor-3 .statement tag=06UR}

— *令 E 为域 K 的扩张，将 E 的 D 推导转化为 E，将映射 K 转化为 K。如果 L 是 E 的子扩展，且是代数且可在 K 上分离，则 $D(L) \subset L$。*

设A为K的推导到L，与K上的D一致。根据命题4（V，p. 129），存在L的推导D'到L延伸A。现在我们可以考虑将D'和限制D''延伸到L将 $L$ 的推导代入 E ；因为他们在 K 上达成一致，所以根据第 4 条命题我们有 $D' = D''$，从而

$$
D(L) = D''(L) = D'(L) \subset L .
$$

#### 注 {#alg-v-s16-n2-rem-1 .statement tag=06US}

— 1）稍后（V，p. 131，Cor.3和p. 135，Cor.2）我们将向Cor.证明逆命题。提案 4 中的 1 条。

2) 素数域的每个代数扩张都是可分的（V，p. 37，Cor.）。由于素数域的每个推导都是零，所以素数域的代数扩张的每个推导都是零（命题4）。

### 3. 特征零域中的推导

#### 定理 1 {#alg-v-s16-thm-1 .statement tag=06UT}

— *令 K 为特征 0 的域、K 的 L 扩张以及 L 上的 V 向量空间。设A是K的推导到V，$(x_i)_{i \in I}$，L对K的超越基和$(u_i)_{i \in I}$，V的元素族。那么存在一个唯一的L到V延伸A的推导D，并且对于所有$i \in I$都有$D(x_i) = u_i$。*

把$E = K(x_i)_{i \in I}$；命题3（V，p. 128）表明，扩展到E的唯一推导$D_0$到V，使得$D_0(x_i) = u_i$对于所有$i \in I$。 域 $L$ 是 E 的代数扩张，并且由于 L 的特征为 0，L 在 E 上可分（V，p. 37，Cor.）。因此（V，p. 129，命题4）$D_0$扩展到$L$的唯一推导D到V。

#### 推论 1 {#alg-v-s16-thm-1-cor-1 .statement tag=06UU}

— *K 的每个推导转换为 V 扩展到推导 L 转换为 V*

#### 推论 2 {#alg-v-s16-thm-1-cor-2 .statement tag=06UV}

— *令 E 为 L 和 U 向量 L 子空间$\Omega_K(L)$ 的子扩展，由 E 的元素微分生成。对于元素 x 在 E 上的代数，$dx \in U$ 是充分必要的。*

对于每个 $y \in L$ 令 D(y) 为 $dy$ mod U 的剩余类类。则 D 是 L 到 $\Omega_K(L)/U$ 的 E 导数。由于 K 的特征为 0，因此 E 的每个代数扩张都是可分的 (V, p. 37, Cor.) ；如果$x \in L$是E上的代数，则根据命题4（V，p. 129）我们有$Dx = 0$，即$dx \in U$。

如果$x \in L$超越$E$，则存在$E(x)$到$L$的E推导$A$，使得$\Delta(x) = 1$（$V$，p. 128，命题3）；通过 Th。 1、 $A$ 扩展到 $L$ 的 E 导数 D 到 L。令$\varphi$为$\Omega_K(L)$上的线性形式，使得$D = \varphi \circ d$；我们有 $\varphi(dy) = 0$ 对应 $y \in E$ 和 $\varphi(x) = 1$，从而 $dx \notin U$。

#### 推论 3 {#alg-v-s16-thm-1-cor-3 .statement tag=06UW}

— *为了使 L 的元素 x 成为 K 上的代数，$dx = 0$ 在 $\Omega_K(L)$ 中是必要且充分的。特别是，对于L是K的代数扩张来说，$\Omega_K(L) = 0$是充分必要的。
这立即来自Cor。 2 服用$E = K$。

#### 推论 4 {#alg-v-s16-thm-1-cor-4 .statement tag=06UX}

— *令 K、L 和 M 为特征 0 的域，使得 $K \subset L \subset M$：则典范映射 $a : \Omega_K(L) \otimes_L M \to \Omega_K(M)$ 是单射的。
这是从 Cor 立即得出的结论。 1 和 $V$、p. 128、提案 2。

#### 定理 2 {#alg-v-s16-thm-2 .statement tag=06UY}

— *令K为特征0的域、K的L扩张和$(x_i)_{i \in I}$，即L的元素族。
a) 对于 $(x_i)_{i \in I}$，要在 K 上保持代数自由，$\Omega_K(L)$ 中的微分 $dx_i$（对于 $i \in I$）在 L 上线性自由是必要且充分的。
b) 为了使L成为$K(x_i)_{i \in I}$上的代数，对于$i \in I$生成向量空间$\Omega_K(L)$在L上的微分$dx_i$是必要且充分的。
c) 为了使$(x_i)_{i \in I}$成为L对K的超越基，族$(dx_i)_{i \in I}$应该是$\Omega_K(L)$对L的基是充分必要的。
对于每个$i \in I$，令$E_i$为子域$K(x_j)_{j \in I, j \neq i}$ / L。对于族 $(x_i)_{i \in I}$，要在 K 上保持代数自由，对于每个 $i \in I$，$x_i$ 应该超越 $E_i$ 是必要且充分的（$V$，p. 108，命题 5）。由科. 2 Th。 1 这意味着对于每个$i \in I$，微分$dx_i$不是线性组合，其系数在L中，$dx_j$与$j \neq i$在I中的微分；后者条件仅意味着家庭$(dx_i)_{i \in I}$在L、从而 a) 上是免费的。
断言 b) 立即来自 Cor. 2 Th。 1和c)是a)和b)的推论。

#### 推论{#alg-v-s16-n3-cor-1 .statement tag=06UZ}

— *当 K 的特征为 0 时，我们有 $[\Omega_K(L) : L] = \operatorname{tr} \cdot \deg_K L$。

### 4.推导在可分扩张

We have seen ($V$, p. 122, Th. 1) that every extension $L$ of a field $K$ of characteristic 0 is separable; moreover, every derivation of K into a vector space over $L$ extends then to a derivation of $L$ ($V$, p. 130, Cor. 1). 更一般地，我们有以下叙述：

#### 定理 3 {#alg-v-s16-thm-3 .statement tag=06V0}

— *令 K 为 K 的域和 L 扩张。为了使 L 可在 K 上分离，K 的每个推导进入向量 L 空间应为扩展至推导 L。
我们可以假设 K 具有特征$\neq 0$。首先假设L在K上可分。令$V$在L上成为向量空间，并且将K的$A$推导变成$V$。通过Mac

Lane 准则 (V、p. 124、注)、域、$L^p$ 和 $K$ 与不相交的与 $K^p$ 呈线性关系。 由于$A$是$K$到$V$的$K^p$线性映射，因此扩展以独特的方式将$K[L^p] = K(L^p)$到$V$的$L^p$线性映射$A'$。 很明显，$A'$是$K(L^p)$的推导进入$V$，在$L^p$上消失；因此，它将$L$的扩展（V，p. 103，Cor.3）到推导转换为$V$。

相反，假设$K$的每个推导和$L$扩展中的值到$L$的推导都进入$L$。 Let $B$ be a p-basis of $K$ (V, p. 99) and let $A$ be the set of families $(\alpha_h)_{h \in R}$ with finite support consisting of integers between $()$ and $p - 1$. 对于每个$b \in B$，存在$K$到$K$的推导$\Delta_b$，其特征在于每个$b' \in B$（V，p. 103）的$\Delta_b(b') = \delta_{bb'}$（克罗内克符号）。 到假设，$L$的每个$b \in B$推导$D_b$都存在延伸$\Delta_b$的$L$。 对于$B$中的$b, b'$，我们有$D_b(b') = \delta_{bb'}$，这证明在$\Omega_{1/p}(L)$中，微分$db$（对于$b \in B$）在$L$上是线性无关的。 因此 (V, p 102, Th.1), $B$ 在 $L^p$ 上是无 p 的。 由此可见（V，p. 98，命题1和p. 124，注）$K$的扩张$L$是可分的。

#### 推论{#alg-v-s16-n4-cor-1 .statement tag=06V1}

— *如果$L$是$K$的可分扩张，则典范映射$\alpha_p : \Omega_p(K) \otimes_K L \to \Omega_p(L)$对于$K$的每个子域$P$是单射的。相反，如果存在 $K$ 的完美子域 $P$（对于例 $K$ 的素数子域），使得映射 $\alpha_p$ 是单射的，则 $L$ 在 $K$ 上可分。*

第一个断言源自 Prop. 2 (V, p. 128) 和 Th。 3.反之，令$P$为$K$的完美子域；我们有$P = P^p \subset K^p$，因此$K$到向量$L$空间的每个推导都是$P$衍生；现在，推论的第二个断言来自Cor。 2 (V、p. 130) 和 Th。 3.

### 5. 指标 / 线性映射

令$L$为域$^1$，令$U$和$V$为$L$和$f : U \to V$上的两个向量空间$^2$，一个$L$线性映射；如果$f$的核$N$和余核$C$有有限维和整数，则称$f$有*有限指标*

$$
\chi(f) = [C : L] - [N : L]
$$

称为$f$的*指标*。

#### 引理 1 {#alg-v-s16-lem-1 .statement tag=06V2}

— *令$U$和$V$为有限维中的两个向量空间超过域$L$。每个线性映射$f : U \to V$拥有指标等于$[V : L] - [U : L]$。*

令$N$为核、$I$像和$C$余核/$f$。我们有$C = V/I$，$I$与$U/N$同构的；因此我们有$[U : L] = [N : L] + [I : L]$和$[V : L] = [C : L] + [I : L]$，从而结果。

$^1$ 不一定可交换。
$^2$ 在左边。

#### 引理 2 {#alg-v-s16-lem-2 .statement tag=06V3}

令 $f : U \to V$ 和 $g : V \to W$ 为两个 L 线性映射。 iff 和 g 各有指标，$g \circ f$ 也是如此，我们有

$$
\chi(g \circ f) = \chi(f) + \chi(g).
$$

设$h = g \circ f$，分别用N、N'、N''核off、g、h表示，并用C、C'、C''表示它们的余核。我们有$N \subset N'' \subset U$和$f(N'') = f(U) \cap N'$；因此存在线性映射$\bar{f} : N'' \to N'$与N''上的f一致并且与核N一致。V的典范映射$\pi$到N'的$C = V / f(U)$诱导映射$\pi'$到C，其核是 $f(U) \cap N' = \bar{f}(N'')$。通过将 $C = V/f(U)$ 的商 g 定义映射 $\bar{g}$ 代入 $C'' = W/g(f(U))$，其中核显然是 $(N' + f(U))/f(U) = \pi'(N')$。最后，$C'' = W/g(f(U))$到$C' = W/g(V)$的典范映射$\rho$有核$g(V)/g(f(U)) = \bar{g}(C)$。到和以上，我们已经确定了序列的正确性

$$
0 \to N \xrightarrow{i} N'' \xrightarrow{\bar{f}} N' \xrightarrow{\pi'} C \xrightarrow{\bar{g}} C'' \xrightarrow{\rho} C' \to 0
$$

（其中 i 是 N 中 N 的典范嵌入”）。

![图表显示N、N'、N''、U、V、W、C、C'、C''之间的关系，箭头表示映射和核](../images/fig_1.png)

图1

假设 N、N'、C 和 C' 为有限维；因此 N'' 和 C 也是如此。由科. 2 (II, p. 295) 那么我们有

$$
[N : L] - [N'' : L] + [N' : L] - [C : L] + [C'' : L] - [C' : L] = 0
$$

从而$\chi(h) = \chi(f) + \chi(g)$。

### 6. 有限生成的扩张的微分性质

#### 定理 4 {#alg-v-s16-thm-4 .statement tag=06V4}

令 P 为 P 的完美域、L 扩张，K 为 L 的子扩展；我们假设L是K的有限生成的扩张。那么规范的L线性映射$a : \Omega_p(K) \otimes_K L \to \Omega_p(L)$的指标等于L在K上的超越次数。

如果$E$和$F$是$L$的两个子扩展，使得$E \subset F$，我们用$\alpha(F/E)$表示$\Omega_p(E) \otimes_E F$到$\Omega_p(F)$的规范$F$线性映射，并且当它被定义时，指标 $\alpha(F/E)$将被写成$d(F/E)$。如果$E, F$和$G$是$L$的三个子扩展，使得$E \subset F \subset G$，我们有一个可交换的图表

$$
\begin{array}{ccc}
\Omega_p(F) \otimes_F G & \xrightarrow{\alpha(G/F)} & \Omega_p(G) \\
\uparrow \alpha(F/E) \otimes_F \mathrm{Id}_G & & \uparrow \alpha(G/E) \\
(\Omega_p(E) \otimes_E F) \otimes_F G & \xrightarrow{\beta} & \Omega_p(E) \otimes_E G
\end{array}
$$

其中 $\beta$ 是提案 2 中定义的典范同构（II，p. 278）。由于指标在扩张下通过标量显然是不变的，并且同构的指标是零，引理2（$V$，p. 133）表明指标当 $d(F/E)$ 和 $d(G/F)$ 时，$d(G/E)$ 被定义，然后

$$
d(G/E) = d(G/F) + d(F/E).
$$

由于 $L$ 是 $K$、公式 (5) 的有限生成的扩张，并且 Cor. $V$、p. 111表明，考虑$x$存在使得$L = K(x)$的情况就足够了；进一步，如果$x$是$K$上的代数，则存在$L$的特征指数幂$q$，使得$x^q$是$K$上的可分代数（$V$，p. 44，命题1） 13）。因此，在以下三种特殊情况下，建立等式 $d(L/K) = \operatorname{tr} . \deg_K L$ 就足够了：

a) $x$ 超越 $K$：则 $a$ 是单射，其余核是秩 1 超过 $L$（$V$，p. 129，Cor.）；所以我们有$d(L/K) = 1$，还有$\operatorname{tr} . \deg_K L = 1$。

b) $x$ 是 $K$ 上的可分代数：则 $a$ 是双射 ($V$, p. 130, Cor. 2), 从而 $d(L/K) = 0$;显然也是$\operatorname{tr} . \deg_K L = 0$。

c) *域$L$具有特征$p \neq 0$，$x \notin K$和$x^p = a$在$K$*中：$a$的余核$C$与$\Omega_K(L)$同构的，并且因为$\{ x \}$是$p$-$L$超过$K$、空间$C$的基础是维数1超过$L$（$V$、p. 102、Th.1）。由于$a$是$L$中的第$p$幂，因此我们有$a$包含子空间$R$生成$U = \Omega_p(K) \otimes_K L$的$d_{L/pa} = 0$和核 $d_{K/pa} \otimes 1$。对于每个 $y \in K$ 令 $\Delta(y)$ 为剩余类类 of $d_{K/p}y \otimes 1$ mod $R$；那么$A$是$K$到$U/R$的$P$衍生，这样$\Delta(a) = 0$。命题5（$V$，p. 101）表明$A$扩展到$L$的$P$衍生$D$到$U/R$。因此，存在$L$线性映射$\beta : \Omega_p(L) \to U/R$，使得$D = \beta \circ d_{L/P}$和$\beta \circ a$是$U$到$U/R$的典范映射。这证明$R$是$a$的核。由于 $P$ 是完美的，所以我们有 $P(K^P) = K^p$、从而 $a \notin P(K^P)$，最后是 $d_{K/pa} \neq 0$（$V$、p. 103，第 6 条）。因此，$a$的核和余核是维数1，从而$d(L/K) = 0$，并且我们还有$\operatorname{tr} . \deg_K L = 0$。

#### 推论 1 {#alg-v-s16-thm-4-cor-1 .statement tag=06V5}

— *令$L$是超越次数$s$的域$K$的有限生成的扩张。 向量空间 $\Omega_K(L)$ 是维数 $\geq s$ 超过$L$，等式当且仅当$L$ $K$ 可分离。*

设 P 为 K 的素数子域。设 N 为 α 的核，然后通过序列 $(\mathbf{E}_{P,K,L})$ (V, p. 128) 和 Th 的精确性。 4、我们有$[ \Omega_K(L) : L ] = s + [N : L]$；通过V，p. 132，Cor.，扩张L，K 是可分离的当且仅当$N = 0$。现在推论如下。

#### 推出 2 {#alg-v-s16-thm-4-cor-2 .statement tag=06V6}

— *令 L 为域 K 的有限生成扩张。对于 L 是代数且可在 K 上分离，$\Omega_K(L) = 0$ 是充分必要的。* 这直接从 Cor 得出。 1.

#### 推出 3 {#alg-v-s16-thm-4-cor-3 .statement tag=06V7}

— *令 K 为特征 $p \neq 0$ 的域和L 超越次数 s 的 K 的有限生成的扩张。如果$[K : K^p]$是有限的，$[L : L^p]$也是有限的，我们有$[L : L^p] = p^s$。 $[K : K^p]$.* 令 P 为 K 的素数子域。如果 $[K : K^p]$ 是有限的，则向量空间 $\Omega_P(K) = \Omega_{K^p}(K)$ 在 K 上有有限维 m，并且我们有 $[K : K^p] = p^m$ (V, p. 103, Th. 2)； 向量空间 $\Omega_P(K) \otimes_K L$ 则有限维 m 超过 L。此外，由于K在$K^p$上为有限次数，所以域$K(L^p)$在$K^p(L^p) = L^p$上为有限次数；由于域L是K的有限生成的扩张并且是$K(L^p)$上的代数，因此它是$K(L^p)$的有限次数的扩张(V，p. 18，Th.2)；因此，我们结论，L是有限次数超过$L^p$（V，p. 10，Th.1）。那么$\Omega_P(L)$是有限维n的向量空间除以L，我们有$[L : L^p] = p^n$（V，p. 103，Th.2）。通过引理 1 (V, p. 132)，L线性映射$\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$因此具有指标$n - m$，从而$n - m = s$。 4（V、p. 133）和$p^n = p^s \cdot p^m$。

#### 注 1 {#alg-v-s16-n6-rem-1 .statement tag=06V8}

令 K 为特征 $p \neq 0$ 的域和 K 的L 扩张。当且仅当$L = K(L^p)$（V，p. 103，命题 6）时，我们才有$\Omega_K(L) = 0$。因此，如果L是在K上有限生成的，那么它是一个代数，并且可分扩张当且仅当我们有$L = K(L^p)$。当L不是在K上有限生成时，这个结果通常不再成立，如L是K的完美闭包的情况所示。

#### 注 2 {#alg-v-s16-n6-rem-2 .statement tag=06V9}

令K为由元素$x_1, \ldots, x_n$生成的K的$K[X_1, \ldots, X_n]$和L扩张中的域、$F_1, \ldots, F_m$多项式。假设多项式 $F_1, \ldots, F_m$ 生成是所有多项式 F 的$K[X_1, \ldots, X_n]$ 由……组成的理想，使得$F(x_1, \ldots, x_n) = 0$。从命题1（V，p. 127）和模的微分（III，p. 569）的泛性质，我们很容易推导出以下结果：向量空间$\Omega_K(L)$超过L的生成方式为$dx_1, \ldots, dx_n$；我们有关系

$$
\sum_{i=1}^n D_i F_j(x_1, \ldots, x_n) \cdot dx_i = 0 \quad \text{(for } 1 \leq j \leq m \text{)} ;
$$

最后，如果$u_1, \ldots, u_n$是L的元素使得$\sum_{i=1}^n u_i \cdot dx_i = 0$，则存在L的元素$v_1, \ldots, v_m$使得$u_i = \sum_{j=1}^m D_i F_j(x_1, \ldots, x_n) \ v_j$对于$1 \leq i \leq n$。让我们用 n 行和 m 列的矩阵 $(D_i F_j(x_1, \ldots, x_n))$ 的 r 秩表示；令 s 为 $L$ 对 $K$ 的超越次数。那么我们就有$[ \Omega_K(L) : L ] = n - r$。因此，当且仅当 $r + s = n$（Cor. 1）时，$K$ 的扩张 $L$ 是可分离的。当且仅当 $r = n$（Cor. 2）时，它是代数且可分离的。

### 7.分离超越基

#### 定义 1 {#alg-v-s16-def-1 .statement tag=06VA}

*设$L$为域$K$中的扩张。如果 $K(B)$ 的代数扩张 $L$ 可分离，则 $L$ 对 $K$ 的超越基 $B$ 被认为是可分离的。*

如果$K$具有特征0，则$L$对$K$的每个超越基都是可分离的，因为特征0的域的每个代数扩张都是可分离的（$V$，p. 37，Cor.）。如果扩张承认分离超越基，它是可分离的（$V$，p. 121，命题6和p. 122，命题9）。下面的定理表明，每个*有限生成的*可分扩张都承认一个分离的超越基；这个限制是必不可少的（$V$，p. 177，例1）。

#### 定理 5 {#alg-v-s16-thm-5 .statement tag=06VB}

*设$K$为域，$K$的$L$扩张和$(x_i)_{i \in I}$，$L$的元素一家。如果家庭$(x_i)_{i \in I}$，是$L$超过$K$的分离超越基，那么家庭$(dx_i)_{i \in I}$，就是向量空间$\Omega_K(L)$超过$L$的基。如果 $L$ 是 $K$ 的有限生成的可分扩张，则逆命题成立。

将$M = K(x_i)_{i \in I}$代入$\Omega_K(L)$，并用$\Omega_K(M) \otimes_M L$的$\alpha$典范映射表示。如果$(x_i)_{i \in I}$是$L$在$K$上的分离超越基，则家庭$(d_{M/K} x_i)_{i \in I}$，是向量$M$-空间$\Omega_K(M)$的基（$V$， p. 128，命题 3)，$\alpha$ 是向量 $L$ 空间的同构，因为 $L$ 是代数且可在 $M$ 上分离（$V$、p. 130，Cor.2）。从$\alpha(d_{M/K} x_i \otimes 1) = d_{L/K} x_i$开始，族$(d_{L/K} x_i)_{i \in I}$因此是$\Omega_K(L)$的基超过$L$。

相反，假设$L$是$K$的可分离有限生成的扩张，并且族$(d_{L/K} x_i)_{i \in I}$是向量空间$\Omega_K(L)$在$L$上的基。由科. $V$、p. 134的1，$L$对$K$的超越次数等于$\Omega_K(L)$对$L$的维数，因此是$I$的基数。从正合序列$(E_{K,M,L})$（$V$，p. 128）我们有$\Omega_M(L) = 0$；因为$L$是$M$的有限生成的扩张，Cor。 $V$、p. 135 的 2 表明 $L$ 是代数且在 $M = K(x_i)_{i \in I}$ 上可分；由于$L$对$K$的超越次数是有限的并且等于$I$的基数，因此族$(x_i)_{i \in I}$是$L$对$K$的超越基（$V$， p. 110，Cor.1)。

#### 推出 {#alg-v-s16-n7-cor-1 .statement tag=06VC}

*令$L$为$K$的可分离有限生成扩张，并令$S$为$L$的子集，使得$L = K(S)$。那么存在$L$对$K$的分离超越基$B$，包含在$S$中。

由于$\Omega_K(L)$是由元素与$S$的微分生成的，因此存在$S$的$s$元素$x_1, \ldots, x_s$，使得$(dx_1, \ldots, dx_s)$是$\Omega_K(L)$的基 $L$。现在应用 Th 就足够了。 5.

#### 注 {#alg-v-s16-n7-rem-1 .statement tag=06VD}

— 设$L$是特征$p \neq 0$的域$K$的可分离有限生成扩张；可能存在不分离的基对$L$的超越。只要观察到$\{X^p\}$是$K(X)$的超越基，而$K(X)$是$K(X^p)$的次数$p$的p根式扩展就足够了。

#### 命题 5 {#alg-v-s16-prop-5 .statement tag=06VE}

— *令 L 和 M 为给定扩张中包含的域 K 中的两个扩张，并且在 K 上代数上不相交的。如果 M 在 K 上可分，则 L(M) 在 L 上可分。*

足以证明对于 M 的每个有限子集 S，$L(S)$ 在 L 上是可分的（V，p. 122，命题 8）。令S为M的有限子集。由于域$K(S)$可在K上分离，因此它具有分离超越基B（Th.5的Cor.）。由于L和M在K上的代数不相交的，B是$L(B)$在L上的超越基（V，p. 113，命题12）。此外，S 的每个元素都是代数且在 $K(B)$ 上可分，因此在 $L(B)$ 上（V，p. 39，Cor. 2）。我们推论（V，p. 39，命题 6）$L(S) = L(B)(S)$ 是代数且在 $L(B)$ 上可分，因此 $L(S)$ 在 L 上可分。

#### 推出{#alg-v-s16-n7-cor-2 .statement tag=06VF}

— *如果 L 和 M 是可分扩张，在 K 上代数不相交的，则域 $K(L \cup M)$ 在 K 上可分。*

因为 $K(L \cup M) = L(M)$ 可以通过命题 5 在 L 上分离（因为 M 可以在 K 上分离），并且 L 可以在 K 上分离，从而的推论（V、p. 122、命题 9）。

假设扩张L和M在代数上不相交的在命题5及其推论中是不可或缺的。 令 K 为特征 $p \neq 0$ 的不完美域和形式 $K(x, a)$ 的 E 扩张，其中 x 超越 K 且在 K 上高度为 1 的 p 根式；输入$L = K(x)$和$M = K(x + a)$。 那么$x + a$是K上的超越（如果不是，$x = (x + a) - a$将是K上的代数）并且域L和M在K上可分。 然而，$K(L \cup M) = K(x, a)$ 是次数 $p$ 在 $L = K(x)$ 上的 p 根式，并且在 L 上不可分，在 K 上也不可分。

### 习题{#alg-v-s16-exercises}

§ 16](exercises/s16/)参见[习题。
